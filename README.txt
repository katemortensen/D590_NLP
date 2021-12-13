
***************************************************************************************/
*    Title: LSTM & Ubuntu Chatbot 
*    Author: Kate Mortensen 
*    Date: 12-11-2021
*    Code version: 1.0
*    Availability: NA
*    
* @article{lowe2015ubuntu,
*  title={The ubuntu dialogue corpus: A large dataset for research in unstructured multi-turn dialogue systems},
*  author={Lowe, Ryan and Pow, Nissan and Serban, Iulian and Pineau, Joelle},
*  journal={arXiv preprint arXiv:1506.08909},
*  year={2015}
*  }
* @article{kadlec2015improved,
*  title={Improved deep learning baselines for ubuntu corpus dialogs},
*  author={Kadlec, Rudolf and Schmid, Martin and Kleindienst, Jan},
*  journal={arXiv preprint arXiv:1510.03753},
*  year={2015}
*  }
* Code Inspiration
* Author: Janina Nuber
* Tile: Chatbot | Retrieval-based Dialog System on the Ubuntu Dialog Corpus | LSTM | PyTorch
* Date: July 31st, 2019
* Availability: https://github.com/Janinanu/Retrieval-based_Chatbot
*
***************************************************************************************/

**Purpose:**
*The purpose of this project’s chatbot, named Chatty Kathy, is to provide technical support to Ubuntu users. Chatbots often sustain the reputation of being robotic and there is ongoing work to improve the human-like quality of responses. Retrieval-based chatbots rely on a set predefined responses to a user’s input question. There are many ways to choose the best response based on a document of input questions and responses. For example, some retrieval based chatbots produce responses based on “intent” via Tf-idf or BOW while others are based on “entity” and use POS tagging or various word embedding methods. Chatty Kathy is a very simple implementation of a retrieval-based chatbot and is judged using Ubuntu Dialog Corpus as a standard. An LSTM model is used to test whether Chatty Kathy’s responses are sufficiently human based training data from the Ubuntu Dialog Corpus.*

**Data:**
*The Ubuntu Dialog Corpus and Ubuntu Dialog Helpchat were used for this project (Lowe 2016). The Ubuntu Dialog Helpchat data was used to produce responses from Chatty Kathy while the Ubuntu Dialog Corpus was uses to train the LSTM model for retrieval-based chatbots. The Ubuntu Dialog Corpus consists of ~1 million bidirectional conversations from internal Ubuntu chat rooms, providing a substantial amount of data. The Ubuntu Dialog Helpchat data underwent data processing steps as part of the chatbot. The Ubuntu Dialog Corpus came processed and labeled (Nuber 2019). The data format is comma separated for both raw and LSTM ready data. The LSTM data and has 3 columns (user input, bot response, 1=true response/0=random response).*

MASTER SCRIPT: LSTM_Ubuntu_Chatbot.ipynb
