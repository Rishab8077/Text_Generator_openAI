# GPT2(Generative Pre-Trained Transformer 2)

The project is simple we give input as a phrase or sentence or question and as an output we get a small essay generated by this application. Since by name we can understand it is a text generator application. Example 
![screenshot](https://user-images.githubusercontent.com/72625053/134799444-9410c4bf-2c76-404e-b8df-9762b085254b.png)

![screenshot (1)](https://user-images.githubusercontent.com/72625053/134799573-4ed02adb-5664-446c-af11-b3f4317c5927.png)

### As we can see from above example how the application was working. To handle the UI part we imported gradio library which makes work much more easier

## Now lets try to know about its architecture and working of GPT2.
As we know Transformers consists of Encoders and Decoders having Self Attention and Feed Forward Neural Network at Encoders and Masked self attention, Encoder-Decoder self attention and Feed Forward NN at Decoders.<br />
GPT2 has beautiful architecture in a sense that it doesnot have much of Encoders, It relys mostly on Decoders. It is also known as Transformer Decoder since most of the architecture relies on decoders of transformer.
Like in smartphones based on the sentence we are typing it tries to predict the next word GPT2 works in a similary way but one that is much larger and more sophisticated than what our phone has. The way these models actually work is that after each token is produced, that token is added to the sequence of inputs. And that new sequence becomes the input to the model in its next step. This is an idea called “auto-regression”.The common difference between Self attention and masked self attention is self attention block allows to peak at the right side of the word i.e future word but in masked self attention (GPT2) it can onnly peak to the present word and previous word to the left. 
GPT performs way better than berts in generative analysis because GPT gives one token at a time and takes in consideration at next step.<br />
### steps
First we get the Token embedding i.e input embedding we also get Positional Encoding but after that we get Decode transformer block only.
![Screenshot (115)](https://user-images.githubusercontent.com/72625053/134817099-bb7d22b2-a03e-4bee-9a4e-0e8ed96ca454.png)
### This was basic knowledge of how GPT2 works to learn more about the model in depth visit : https://jalammar.github.io/illustrated-gpt2/
