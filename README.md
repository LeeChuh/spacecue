# SpaceCue Project Repo

Make sure you have installed dependencies:

```
pip install datasets
pip install openai
pip install anthropic
```

To use OpenAI and Anthropic API, you need to define the environment variables:

```
export OPENAI_API_KEY='your_openai_api_key'
```

and 

```
export ANTHROPIC_API_KEY='your_anthropic_api_key'
```

To run the experiments:

```
cd baselines
python main.py
```

This is the header for `main.py` file:

```python
def main(field: str, model: str, visual_prompting: str):
```

where 

```python
field = ['Physics', 'Chemistry', 'Biology', 'Math']
model = ['gpt', 'opus']
visual_prompting = [None, 'scaffold', 'spacecue']
```