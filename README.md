```python
import sys, ctypes, asyncio

class readme:
	def __init__(self, username : str, lang : str) -> None:
		self._username = username 
		self._lang = lang
		self._contacts = {
			"discord": {
				"user": "vile#6420",
				"id": "1003643218577068112"
			},
			
			"youtube": {
				"link": "https://www.youtube.com/channel/UCicG4fjprn6t_E1KMjR007A"
			}
			
		}
		
	async def main(self):
	    ctypes.windll.kernel32.SetConsoleTitleW("about-me")
	    sys.stdout.write(f""" 
		username -> {self._username}
		contacts -> discord: {self._contacts['discord']['user']}
		programming language -> {self._lang}
		""")
		
if __name__ == "__main__":
	asyncio.run(readme("vile, syn", "python").main())
```
