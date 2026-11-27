This is the task for day-4
----------------------------
## Part 1 – Sweet Crumbs Home Bakery
-------------------------------------------
In the first part of the workshop, I built an AI agent for a home bakery called Sweet Crumbs.

I connected the Groq LLM and created a Google Sheet to store customer orders. I defined the menu and business hours and created a Pydantic model to structure customer order details like name, item, quantity, pickup date, and eggless preference.

I converted Python functions into tools using LangChain's `@tool` decorator. These tools were used to check item prices, check whether the bakery was open, and save orders to Google Sheets.

I tested the agent with different customer messages, including invalid menu items, missing pickup dates, and zero quantities. I also checked the agent's trace to understand how it selected tools and responded to the customer.

Finally, I placed a sample order for Ravi and verified that the order was successfully saved in Google Sheets.

# Part 2 – Cafe Napoli AI Agent(my own use case)
----------------------------------------------------------------
For the independent task, I created an AI agent for Cafe Napoli, my brother's cafe.

I created a menu with sample prices and implemented two tools: one to check item prices and another to check menu availability. I also created a Pydantic model called `CafeOrder` to extract structured information from customer messages.

I tested the structured output using five different customer messages written in different ways. The model extracted details such as customer name, item, quantity, pickup date, and eggless preference.

I then connected Google Sheets and created an order logging tool to save customer orders along with their total price.

I created the agent using LangChain's `create_agent` and tested its ability to answer menu-related questions and place orders. I successfully tested a chocolate cake order for Priya and verified that the order was saved in Google Sheets.

I also tested an invalid menu item, chicken burger, to check whether the agent would invent a price. It correctly rejected the item.

# Tool Renaming Experiment
----------------------------------------
As part of the workshop, I renamed the price-checking tool to `tool1` and tested the agent again.

Even after renaming it, the agent successfully called the tool and returned the correct price of a latte. I inspected the trace using `pretty_print()` and observed that the agent called `tool1`, received the tool result, and then generated the final response.

After the experiment, I restored the original tool name and agent.

# Day 4 Outcome
---------------------
Through this workshop, I learned how to create tools for an AI agent, use structured output with Pydantic, connect Google Sheets for storing data, test agents with different inputs, and inspect tool calls and traces.

I also understood how an AI agent can use tools to perform actual tasks instead of simply generating text responses.

I created `cafe_napoli_facts.txt` containing business information and operational challenges to prepare for the next day's workshop.
