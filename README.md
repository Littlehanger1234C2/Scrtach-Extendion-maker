# Scrtach-Extendion-maker
class  Test  {

  constructor ( )  { }

  getInfo ( )  {  // Various information about extensions
    return  {
      id : 'test' ,
      name : 'Test' ,  // extension name
      blocks : [  // Definition of each block
        {
          opcode : 'hello' ,  // When this block is executed, a function called hello is called
          BlockType : Scratch . BlockType . COMMAND , normal instruction blocks, such as // "move 10 steps"　
          text : 'hello'  // Text displayed in the block
        }
      ]
    }
  }

  hello ( )  {
    console . log ( 'hello' ) ;  // console log in hello and output
  }
}

Scratch . Extensions . Register ( New  Test ( ) ) ;
