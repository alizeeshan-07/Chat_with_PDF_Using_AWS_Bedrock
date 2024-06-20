# PDF Chat with AWS Bedrock

This project demonstrates how to use the Titan Embeddings Model from AWS Bedrock to generate embeddings and interact with PDF documents. The project includes setting up AWS CLI, configuring the necessary environment, and running a Streamlit application to ask questions about the PDF files using different language models.

## Prerequisites

Before running this script, ensure you have the following:

- Python 3.6 or higher
- AWS SDK for Python (`boto3`)
- Streamlit
- Langchain Community Libraries
- AWS credentials configured with necessary permissions to use Bedrock service

## Installation

1. **Install the required libraries**:

    ```bash
    pip install boto3 streamlit langchain numpy
    ```

2. **Configure AWS credentials**:

    Ensure your AWS credentials are configured. You can do this by setting up the `~/.aws/credentials` file or by using environment variables.


3. **Running the Script**:

    To run the Streamlit application, execute the following command:

    ```bash
    streamlit run app.py
    ```

    Replace `app.py` with the name of your Python file containing the above code.

## Notes

- The script uses the `amazon.titan-embed-text-v1` model for generating embeddings by default.
- The `ai21.j2-mid-v1` and `meta.llama2-70b-chat-v1` models are used for answering questions.

## Example Output

After running the script, you can interact with the Streamlit app to ask questions about the PDF files. The responses will be generated using the specified language models.

## Troubleshooting

- Ensure that your AWS credentials are correctly configured.
- Verify that you have the necessary permissions to access the Bedrock service.
- Check for any network connectivity issues that may prevent reaching the AWS services.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please submit a pull request or open an issue to discuss your ideas.
