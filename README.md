# ASR E2E Toolkit


## Encoder output
- Input: `inputs`, `input_lengths`
- Output: `outputs`, `output_lengths`

## Decoder:
- Input: `targets`, `target_lengths`, `encoder_outputs` (optional)
- Output: `decoder_outputs`

- Nếu có `encoder_outputs` thì mới sử dụng attention

Với mỗi lớp `encoder` và `decoder` thì đều phải có tham số `output_dim`

## References
- https://github.com/sooftware/conformer

## Variable
set HYDRA_FULL_ERROR=1

## Run
- `python main.py -cp conf -cn configs`