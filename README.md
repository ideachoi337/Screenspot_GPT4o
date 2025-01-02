# Screenspot_GPT4o
<img width="1076" alt="Screenshot 2025-01-02 at 12 20 30 PM" src="https://github.com/user-attachments/assets/25a32c93-3bb3-4fe1-a652-57cfa90be89c" />

### prompt
```
"messages": [
                {
                    "role": "system", 
                    "content": "You are an AI assistant that performs GUI grounding using a GUI screenshot image."
                },
                {
                    "role": "user",
                    "content": [
                        {
                            "type": "text",
                            "text": f"Given a GUI image, what are the relative (0-1000) pixel point coordinates for the element corresponding to the following instruction or description: {inst}. Please provide the response in the format (x, y).",
                        },
                        {
                            "type": "image_url",
                            "image_url": {"url": f"data:image/png;base64,{base64_image}", "detail": f"{detail}"},
                        },
                    ]
                }
            ]
```
