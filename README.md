# Folder structure
 - Audio files in WAV format are placed in folders named after command labels.
 - The folders are compressed into ZIP format for ease at downloading.
 - The ZIP files are placed under folder `recordings`.
# Labeling
- Command labels are ZIP file names without file extension, e.g., `dat_ho_boi`.
- Each WAV file is named in a format of `[speaker ID]_[utterance ID].wav`, e.g., `002_617cbc489e4abed84832312c.wav`.

# Dataset summary
| **Attribute**       | **Value** |
|---------------------|----------:|
| Valid samples       |    15,556 |
| Invalid samples     |       765 |
| Command classes     |        19 |
| Samples per command |    818.74 |
| Speaker classes     |       218 |
| Samples per speaker |     71.36 |

# Number of samples by command
| **No.** | **Command in Vietnamese** | **Command in English** | **Total samples** |
|----|----|----|----:|
| 1 | mở cửa | open door | 890 |
| 2 | đóng cửa | close door | 838 |
| 3 | mở tivi | turn on TV | 841 |
| 4 | tắt tivi | turn off TV| 836 |
| 5 | mở điều hòa | turn on air conditioner | 830|
| 6 | tắt điều hòa | turn on air conditioner | 823 |
| 7 | mở nhạc | play music | 824 |
| 8 | tắt nhạc | stop music | 818 |
| 9 | mở email | open email | 822 |
| 10 | tắt email | close email | 806 |
| 11 | đọc email | read email | 810 |
| 12 | soạn email | compose email | 809 |
| 13 | trả lời | email reply email | 824 |
| 14 | thanh toán hóa đơn mua hàng | pay order | 809 |
| 15 | thanh toán hóa đơn bảo trì | pay maintenance fee | 806 |
| 16 | thanh toán hóa đơn vệ sinh | pay cleaning up fee | 801 |
| 17 | đặt hồ bơi | book swimming pool | 803 |
| 18 | đặt tiệc | book party | 790 |
| 19 | đặt sân tập | book sport venue | 766 |

# By speaker
- Recordings are reorganized by speaker and placed under folder `by_speaker` for purposes like speech synthesis with personalization. 
- Example usage: synthesized voices with model viXTTS at https://huggingface.co/datasets/huynhlong/VietFake
- Utterances of all commands are concatenated into a single WAV file. Only one utterance is selected for one command.
- Each WAV file is named in a format of `[speaker ID].wav`, e.g., `007.wav`.
- Some speakers with low audio quality are filtered out.