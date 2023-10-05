## Podświetlanie kodu.
Jak dodać plug in rehype do componentu ReactMarkdown:
```TS
    import ReactMarkdown from 'react-markdown';
    import rehypeRaw from 'rehype-raw';
    import rehypeSanitize from 'rehype-sanitize';
    import rehypeHighlight from 'rehype-highlight';

    const Markdown = ({source}) => {
        return (
            <ReactMarkdown
                rehypePlugins={[rehypeRaw, rehypeSanitize, rehypeHighlight]}
                children={source}
            />
        );
    }
```