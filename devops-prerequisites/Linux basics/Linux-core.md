## **Linux Core Concepts:

1. ## **Pipes(|)** 
Connected output of one command to another.

**`Command 1 | Command 2`**

eg: **`grep error log.txt | wc -l`**

Finds “error” → counts results

## **Used in real life:**

1. log analysis
2. filtering the output
3. chaning(adding or combining) the commands

2. ## **Redirection**

This is used for:
1. To overwrite the output: **`command > file`**
2. To append the output: **`command >> file`**
3. To Redirect errors: **`command 2> error.txt`**

## **Use in real life:**
1. To capture the errors in production
2. to store script output
3. save logs

3. ## **Search tools**
This is used for searching purpose.

## **1. find → search files**

**`find /path -name file.txt`**

## **2. grep → search inside files**

**`grep "error" log.txt`**

## **Use in real life:**
1. Debugging issues
2. finding configs
3. searching for logs

4. ## **File Handling**

This has following uses:

## **1. Create archive**

**`tar -cf archive.tar folder/`**

## **2. Compress**

**`gzip arhive.tar`**

## **3. Extract**

**`gunzip arhive.tar.gz`**