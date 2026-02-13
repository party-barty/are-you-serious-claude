## Troubleshooting, minimizing hallucinations, and maximizing performance

1. **Allow Claude to acknowledge uncertainty**
   - Tell Claude that it should say it doesn’t know if it doesn’t know. Ex. “If you're unsure about something, it's okay to admit it. Just say you don’t know.”

2. **Break down complex tasks**
   - If a task seems too large and Claude is missing steps or not performing certain steps well, break it into smaller steps and work through them with Claude one message at a time.

3. **Include all contextual information for new requests**
   - Claude doesn't retain information from previous conversations, so include all necessary context in each new conversation.

## Example good vs. bad prompt examples

These are more examples that combine multiple prompting techniques to showcase the stark difference between ineffective and highly effective prompts.

### Example 1: Marketing strategy development

Bad prompt:
<prompt>
"Help me create a marketing strategy."
</prompt>

Good prompt:
<prompt>
"As a senior marketing consultant, I need your help developing a comprehensive marketing strategy for our new eco-friendly smartphone accessory line. Our target audience is environmentally conscious millennials and Gen Z consumers. Please provide a detailed strategy that includes:

1. Market Analysis:
   - Current trends in eco-friendly tech accessories
   - 2-3 key competitors and their strategies
   - Potential market size and growth projections

2. Target Audience Persona:
   - Detailed description of our ideal customer
   - Their pain points and how our products solve them

3. Marketing Mix:
   - Product: Key features to highlight
   - Price: Suggested pricing strategy with rationale
   - Place: Recommended distribution channels
   - Promotion: 
     a) 5 marketing channels to focus on, with pros and cons for each
     b) 3 creative campaign ideas for launch

4. Content Strategy:
   - 5 content themes that would resonate with our audience
   - Suggested content types (e.g., blog posts, videos, infographics)

5. KPIs and Measurement:
   - 5 key metrics to track
   - Suggested tools for measuring these metrics

Please present this information in a structured format with headings and bullet points. Where relevant, explain your reasoning or provide brief examples.

After outlining the strategy, please identify any potential challenges or risks we should be aware of, and suggest mitigation strategies for each."
</prompt>

Why it's better: This prompt combines multiple techniques including role assignment, specific task breakdown, structured output request, brainstorming (for campaign ideas and content themes), and asking for explanations. It provides clear guidelines while allowing room for Claude's analysis and creativity.

### Example 2: Financial report analysis

Bad prompt:
<prompt>
"Analyze this financial report."
</prompt>

Good prompt:
<prompt>
"I've attached our company's Q2 financial report titled 'Q2_2023_Financial_Report.pdf'. Act as a seasoned CFO and analyze this report and prepare a briefing for our board of directors. Please structure your analysis as follows:

1. Executive Summary (3-4 sentences highlighting key points)

2. Financial Performance Overview:
   a) Revenue: Compare to previous quarter and same quarter last year
   b) Profit margins: Gross and Net, with explanations for any significant changes
   c) Cash flow: Highlight any concerns or positive developments

3. Key Performance Indicators:
   - List our top 5 KPIs and their current status (Use a table format)
   - For each KPI, provide a brief explanation of its significance and any notable trends

4. Segment Analysis:
   - Break down performance by our three main business segments
   - Identify the best and worst performing segments, with potential reasons for their performance

5. Balance Sheet Review:
   - Highlight any significant changes in assets, liabilities, or equity
   - Calculate and interpret key ratios (e.g., current ratio, debt-to-equity)

6. Forward-Looking Statements:
   - Based on this data, provide 3 key predictions for Q3
   - Suggest 2-3 strategic moves we should consider to improve our financial position

7. Risk Assessment:
   - Identify 3 potential financial risks based on this report
   - Propose mitigation strategies for each risk

8. Peer Comparison:
   - Compare our performance to 2-3 key competitors (use publicly available data)
   - Highlight areas where we're outperforming and areas for improvement

Please use charts or tables where appropriate to visualize data. For any assumptions or interpretations you make, please clearly state them and provide your reasoning.

After completing the analysis, please generate 5 potential questions that board members might ask about this report, along with suggested responses.

Finally, summarize this entire analysis into a single paragraph that I can use as an opening statement in the board meeting."
</prompt>

Why it's better: This prompt combines role-playing (as CFO), structured output, specific data analysis requests, predictive analysis, risk assessment, comparative analysis, and even anticipates follow-up questions. It provides a clear framework while encouraging deep analysis and strategic thinking.
