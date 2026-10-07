In this folder are data where we activated the validate, on_invalid, and max_retries parameters in the SurveyResponder.run_write() method.

And re-ran with the DASS-21 questions. A next step will be to reduce the temperature to 0.8 (Ollama's default) to see if that may help reduce refusal to answer questions.

    validate=True,          # check response in ["valid_responses"]
    on_invalid="recode",    # "none" | "retry" | "recode"
    max_retries=2)          # only used when on_invalid="retry"