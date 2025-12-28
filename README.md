# HR Buddy - AI Assistant for Recruitment

An intelligent AI assistant built with LangGraph to help HR professionals and startup founders plan effective hiring processes.

## Architecture
![Architecture](data/Hiring_Architecture.png)


## Features

- **Intelligent Conversation Flow**: Ask clarifying questions about hiring needs (budget, skills, timeline)
- **Job Description Generation**: Create tailored job descriptions based on specific requirements
- **Hiring Plan Creation**: Generate comprehensive hiring checklists with timelines
- **Structured Output**: Present results in clean, markdown-formatted outputs
- **Session Memory**: Remember context and details across interactions
- **Analytics Dashboard**: Track usage patterns and hiring trends

## Installation

1. Clone the repository:
```bash
git clone https://github.com/skandvj/hr-hiring-agent.git
cd hr-hiring-agent
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Set up environment variables:
```bash
# Create a .env file with your OpenAI API key
echo "OPENAI_API_KEY=your_api_key_here" > .env
```

## Usage

1. Start the Streamlit app:
```bash
streamlit run app.py
```

2. Open your browser at `http://localhost:8501`

3. Interact with the HR Agent:
   - Describe the roles you need to hire for
   - Answer clarifying questions about skills, budget, and timeline
   - Review generated job descriptions and hiring plans
   - Track analytics on the Analytics tab

## Technical Implementation

This project leverages several key technologies:

- **LangGraph**: For building a stateful, multi-step workflow
- **LangChain**: For agent creation and tool integration
- **OpenAI GPT-4**: The underlying language model
- **Streamlit**: For the web interface
- **Python**: Core programming language

## Project Structure

```
hr-hiring-agent/
├── app.py                  # Main Streamlit application
├── agent/
│   ├── __init__.py
│   ├── agent.py            # Agent implementation with LangGraph
│   ├── tools.py            # Custom tools for HR tasks
│   ├── memory.py           # Session memory management
│   └── prompts.py          # System prompts and templates
├── data/                   # Data storage (git-ignored)
│   ├── session_data/       # For conversation history
│   └── analytics/          # For usage statistics
├── requirements.txt        # Project dependencies
└── README.md               # This file
```

## Configuration

The agent can be configured by modifying:

- `agent/prompts.py`: Change system prompts and templates
- `agent/tools.py`: Add or modify HR-related tools
- `app.py`: Adjust the UI layout and features

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## Future Enhancements

- Integration with real job boards and ATS systems
- More sophisticated analytics and reporting
- Customizable templates for different industries
- Additional tools for candidate evaluation

## License

MIT License

Copyright (c) 2025 Skand Vijay

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

## Contact

Name - [skandvj13@gmail.com](mailto:skandvj13@gmail.com)

Project Link: [https://github.com/skandvj/hr-hiring-agent](https://github.com/skandvj/hr-hiring-agent)
