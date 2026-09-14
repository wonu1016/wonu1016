```python
from typing import Any


PORTFOLIO = r'https://yeeeengyu.notion.site/1e92a6b0e27480cfbb0eff89b51303fd'

class Yeeeengyu:
    role = 'AI/ML Backend Engineer'

    stack = {
        'Backend': ['FastAPI', 'Flask'],
        'AI/ML': ['PyTorch', 'LangChain', 'LangGraph', 'YOLO'],
        'Database': ['MongoDB', 'MySQL'],
        'Infra': ['Docker', 'AWS'],
    }

    etc = {
        'blog': {
            'skill_blog':  r'https://blog.ingyuc.click',
            'life_blog': r'https://blog.naver.com/yeeeengyu'
        },
        'linkedIn': r'https://linkedin.com/in/인규-최',
    }


    def introduce(self) -> dict[str, Any]:
        return {
            'role': self.role, 
            'stacks': self.stack,
            'etc': self.etc,
            'portfolio': PORTFOLIO
        }

me = Yeeeengyu()
print(me.introduce())
```
