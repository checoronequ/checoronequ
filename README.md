### Hi there š

<!--
**checoronequ/checoronequ** is a āØ _special_ āØ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- š­ Iām currently working on ...
- š± Iām currently learning ...
- šÆ Iām looking to collaborate on ...
- š¤ Iām looking for help with ...
- š¬ Ask me about ...
- š« How to reach me: ...
- š Pronouns: ...
- ā” Fun fact: ...
-->
```python
class ReadMe:
    def __init__(self, username="oguzhankiyarbi", year=2020):
        self.username = username
        self.name = 'Joem Elias Sanez'
        self.education = {
            'programming': ['Full Stack Software Development', 'Code Institute'],
            'architecture': ['Master of Architecture', 'Columbia University'],
            'art': ['Bachelor of Fine Arts', 'Otis College of Art and Design']
        }
        self.employment = {
            'developer': ['company', 'city'],
            'architect': ['Foster + Partners', ['Singapore', 'New York']],
            'designer': ['Herzog & de Meuron', ['New York', 'Basel']]
        }

    def doing(self, now=2020):
        today = self.year

        if now < today:
            experience = self.employment['architect']
            return """
            I was a design architect with {large_firms} in {big_cities}.
            """.format(large_firms=experience[0], big_cities=experience[1])

        elif now = today:
            dream = self.education['programming']
            return """
            I am currently learning {code} at {code_institute}.
            """.format(code=dream[0], code_institute=dream[1])

        elif now > today:
            goal = self.employment['developer']
            return """
            I am eager to collaborate with {teams} on {projects}.
            """.format(teams=goal[0], projects='software development')
        else:
            return """
            ### Hi there š
            """
        
    def collaborate(self, role, organization, location):
        opportunity = self.employment
        opportunity[role] = [organization, location]

me = ReadMe(2020)
```
