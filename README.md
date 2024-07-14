
# IMAGE CIRCLE IN XML

CREATED BY NOYON BISWAS

![esport_24_logo](https://github.com/user-attachments/assets/0478002c-4abf-4a96-a718-7c1dacf93a83)

## STEP : 1

GO TO Registration.Java Part

   ```bash

        imageprofile.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                Intent intent = new Intent();
                intent.setType("image/*");
                intent.setAction(Intent.ACTION_GET_CONTENT);
                startActivityForResult(Intent.createChooser(intent,"Select Profile Picture"),10);
            }
        });



```

## STEP : 2

Make Method In Java

   ```bash

    protected void onActivityResult(int requestCode, int resultCode, @Nullable Intent data) {
        super.onActivityResult(requestCode, resultCode, data);
        if(requestCode==10){
            if(data!=null){
                imageURI = data.getData();
                imageprofile.setImageURI(imageURI);
            }
        }
    }


   ```

   
## 🚀 About Me
I'm a full stack developer..

