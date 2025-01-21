# openo1-sft-ultra-35m-data

## Instruction
We have released the openo1-sft-ultra-35m-data, which contains 35 million data points. It is based on existing open-source datasets and synthesized using the openo1-qwen-sft model. We first collected open-source datasets and then annotated the data based on difficulty, quality, and question types using the qwen-2.5-72b-instruct model. To ensure the difficulty and quality of the data, we only retained data where both the difficulty and quality are ≥8.

## Data format
- 'uid': Data ID  
- 'query': Original data query  
- 'response': Long COT response, including detailed thought process  
- 'source': Data source  
- 'difficulty': Question difficulty, range from 1 to 10  
- 'quality': Data quality, range from 1 to 10  
- 'answer': Ground truth answer of the data  
- 'query_len': Length of the question  
- 'response_len': Length of the answer  
- 'Topic': Data topic category, including Math | Code | Reasoning  
- 'answer_type': Answer type annotation  
    - For math domain:  
      - a: Purely numerical answer  
      - b: Purely formulaic answer  
      - c: Long textual explanation  
    - For code domain:  
      - a: Answer that includes code  
      - b: Answer that contains only code-related text  
    - For reasoning domain:  
      - a: Answer consisting of only words/phrases  
      - b: Answer that includes a long textual explanation  
- "cases": Test cases included in the code  

## Data statistics
### Data source
We have used the following sources for the data:  
- WebInstructFull  
- homework  
- infinity-instruct
- math-stack-exchange
- MathInstruct
- mcq


![image/png](https://cdn-uploads.huggingface.co/production/uploads/65d2251f98b4a470bf6a26e3/27aLuIiGoc4onBxkxq2qV.png)

<!-- Insert statistical charts for different sources here -->

