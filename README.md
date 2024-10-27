# Agentic Adversarial AI Debate System


An automated debate system that leverages OpenAI's GPT-3.5 to simulate structured debates between two AI agents, with a judge to evaluate arguments. The system generates debate topics and conducts a multi-round debate with scoring and evaluation.

## 🌟 Features

- **Automated Topic Generation**: Generates relevant debate topics using GPT-3.5
- **Dual Agent System**: 
  - Affirmative side debater
  - Negative side debater
- **Automated Judging**: Independent AI judge that scores and evaluates arguments
- **Structured Debate Format**: 
  - Initial arguments
  - Rebuttals
  - Multiple rounds of exchanges
- **Automated Scoring**: Round-by-round scoring with justification
- **Persistent Record**: Saves entire debate transcript to a file

## 🛠️ System Requirements

- Python 3.7+
- OpenAI API key
- Internet connection for API access

## 📦 Installation

1. Clone the repository:
```bash
git clone [your-repository-url]
cd [repository-name]
```

2. Install required dependencies:
```bash
pip install openai
```

3. Configure API key:
   - Open `api_keys.py`
   - Replace `"YOUR-OpenAI-API-key"` with your actual OpenAI API key

## 🗂️ Project Structure

```
.
├── main.py              # Main execution file
├── title.py            # Debate topic generation
├── positive.py         # Affirmative side agent
├── negative.py         # Negative side agent
├── judge.py           # Judging agent
├── api_keys.py        # API key configuration
└── record.txt         # Debate transcript output
```

## 💻 Usage

1. Ensure your API key is configured in `api_keys.py`

2. Run the main script:
```bash
python main.py
```

3. The system will:
   - Generate a debate topic
   - Create necessary AI assistants
   - Conduct the debate
   - Save the transcript to `record.txt`

## 🔄 Debate Flow

1. **Topic Generation**
   - System generates a debate topic
   
2. **Initial Round**
   - Affirmative side presents opening argument
   - Negative side responds with counter-argument
   - Judge evaluates and scores
   
3. **Additional Rounds**
   - Two more rounds of exchanges
   - Each round includes:
     - Affirmative response
     - Negative response
     - Judge evaluation
   
4. **Recording**
   - All exchanges are recorded in `record.txt`
   - Includes topic, arguments, and scores

## 📝 Output Format

The debate is recorded in `record.txt` with the following structure:

```
[Debate Topic]

------------------------------------------------------------

Affirmative side:
[Argument]

Negative side:
[Response]

Judge:
[Scores and Evaluation]

------------------------------------------------------------
[Additional rounds...]
```

## ⚙️ Configuration

Current system parameters:
- Model: GPT-3.5-turbo-16k
- Response length: Limited to 1-2 sentences per argument
- Number of rounds: 3 (1 initial + 2 additional)
- Scoring scale: 1-10 points per side

## 🚧 Limitations

- Requires active OpenAI API key
- Limited to text-based arguments
- No real-time interaction
- No fact-checking mechanism
- No persistent memory between debates
- Fixed number of rounds
- No content moderation

## 🔜 Future Improvements

- Add fact-checking mechanism
- Implement real-time user interface
- Add content moderation
- Extend debate rounds configuration
- Add support for different debate formats
- Implement persistent memory for agents
- Add user interaction capabilities
- Implement more sophisticated scoring system

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.


## 🙏 Acknowledgments

- OpenAI for providing the GPT-3.5 API


## 📞 Contact

E-Mail: vimalkrishnarao@gmail.com
