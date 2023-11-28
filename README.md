```python
from typing import NamedTuple

class ContactInfo(NamedTuple):
    discord: str
    telegram: str

class Attributes:
    def __init__(self):
        self._contact_info = ContactInfo(discord="ninjaride_", telegram="t.me/ninjaride")
        self._life_info = (15, ['Romanian', 'English'])
        self._coding_info = {
            'pro': 'python',
            'intermediate': 'go',
            'learning': ['c++', 'js']
        }
        self._specialities = ('web/app reverse engineering', 'automation')
        self._text_editor = ['vscode']

    def get_contact(self) -> ContactInfo:
        return self._contact_info

    def get_life(self):
        return self._life_info

    def get_coding(self):
        return self._coding_info, self._specialities, self._text_editor
```
