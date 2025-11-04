# Single Responsibility Principle
`` A class should have only one reason to change, meaning it should have one primary responsibility ``

```python
class Journal:
    def __init__(self):
        self.entries = []
        self.count = 0
    def add_entry(self,text):
        self.count += 1
        self.entriesa.append(f'{self.count}: {text}')
    def remove_entry(self,pos):
        del self.entries[pos]
    def __str__(self):
        return '\n'.join(self.entries)

j = Journal()
j.add_entry()


