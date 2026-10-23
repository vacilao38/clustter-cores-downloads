# Componentes de terceiros

- **Whisper / modelos Whisper**: OpenAI, licença MIT, incluída em `assets/licenses/whisper-MIT.txt`. Modelo: https://huggingface.co/ggerganov/whisper.cpp/resolve/main/ggml-base-q5_1.bin
- **Whisper.cpp / GGML**: projeto ggml-org, licença MIT. Integração `whisper_ggml` 2.8.1, licença MIT; as licenças dos pacotes Flutter são incluídas pelo sistema de licenças do Flutter.
- **Silero VAD**: Silero Team, licença MIT. Modelo GGML distribuído por https://huggingface.co/ggml-org/whisper-vad/resolve/main/ggml-silero-v5.1.2.bin ; fonte original: https://github.com/snakers4/silero-vad
- **FFmpeg Windows**: build LGPL obtido de https://github.com/BtbN/FFmpeg-Builds/releases/download/latest/ffmpeg-master-latest-win64-lgpl.zip em 23/10/2026. Binários sem modificações executados como processos separados. A licença LGPL v3 é incluída em `assets/licenses/ffmpeg-LICENSE.txt` e na distribuição Windows. Código-fonte, scripts de configuração e instruções de compilação: https://github.com/FFmpeg/FFmpeg e https://github.com/BtbN/FFmpeg-Builds . O relatório de validação registra versão, configuração e hashes dos binários utilizados. A origem `latest` pode mudar em futuras compilações.
- **FFmpegKit Android**: `ffmpeg_kit_flutter_new_min` 2.1.0 e artefato Maven `com.antonkarpenko:ffmpeg-kit-min:1.0.3`, distribuição LGPL; repositório declarado pelo pacote: https://github.com/sk3llo/ffmpeg_kit_flutter . A integração não inclui variantes GPL. As licenças do pacote acompanham o registro do Flutter.
- **Lato**: fonte sob SIL Open Font License 1.1; licença completa em `assets/fonts/lato-OFL.txt`. Fonte incluída no pacote, sem download em tempo de execução.

As licenças completas dos pacotes Flutter podem ser consultadas em **Modelos e privacidade → Licenças de software livre**. Os componentes e modelos não são de autoria do Folk.
