def delete_file(filename):
    import os
    if os.path.exists(filename):
        os.remove(filename)
        return f"File '{filename}' deleted."
    else:
        return f"File '{filename}' does not exis."

if __name__ == "__main__":
    file_name = "note.txt"
    print(delete_file(file_name))
