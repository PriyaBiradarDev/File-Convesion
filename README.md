# File-Convesion
Excel Read,Excel to CSV,CSV to Excel

public class CreateWorkBook {
	
	public static void main(String[] args)throws Exception {
	      //Create Blank workbook
	      XSSFWorkbook workbook = new XSSFWorkbook(); 

	      //Create file system using specific name
	      FileOutputStream out = new FileOutputStream(new File("createworkbook.xlsx"));

	      //write operation workbook using file out object 
	      workbook.write(out);
	      out.close();
	      System.out.println("createworkbook.xlsx written successfully");
	   }

}
