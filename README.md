# Hi, my name is Sage ([about me](/about))!

### Just checking in with you, seeing how you're doing.

I'm working this summer (2024) at Civil Design Inc. as a Computer Science intern and I'm using the following skills:
 - C#
 - .NET 6
 - MS SQL
 - Database schema design

<a href="https://sphills.github.io/dmz_missions/" target="_blank">Here's a responsive mockup for a web app integration with Activision's Modern Warfare II side mode *DMZ* where a player can keep track of their mission completion status can be found here</a>.

I'm an adult learner returning to higher education after 6 years in the United States Air Force. During my time in the Air Force, I met so many different and awesome people who I still keep in touch with. It turns out that shared experiences, even if they're not the exact same experience, makes for quick and strong bonds. By the end of my enlistment, I was honored to be given a Supervisor of the Month award, named Subject Matter Expert in my mission set, and made the first supervisory rank of Staff Sergeant.

I've been married for going on 10 years to my wonderful wife, who has supported me through thick and thin. We've lived in and traveled to and through so many states in our great, wide, diverse country, and have even hopped across the Atlantic to visit Ireland and France. We've seen Tony Bennett in concert, watched a performance of A Christmas Carol, and gone axe throwing to name a few memorable times.

As a guy who likes to dabble, my latest hobbies are roller skating at our local roller rink and riding my vintage Kawasaki motorcycle. I wear a hi-viz XL helmet and the kind of reflective neon yellow vest that you might see on public works, construction, or road crew workers to try and increase my visibility to the oft distracted and texting automotive drivers, and it's served me well so far.

I first got into programming when I worked the night shift in the USAF, as a hobby. The game [The Division](https://www.ubisoft.com/en-us/game/the-division) came out, and it was the first loot-focused game I'd ever played. I was enthralled, and I sunk so many after-work hours into it because of its addictive gameplay loop. However, as updates were released and new content dropped, the devs began to mess with the balance of the game, and I was not a fan. So, I looked up "best game engines for beginners" and got to work in Unreal Engine 4.6 trying to create a third-person shooter of my own.

This went terribly, and I was awful at programming. The engine was so heavily optimized for first-person shooter development, and had so many new technical terms (*quaternions, anyone?*) that I suffered and toiled through many, many hours of trial and error as I tried to juggle work and beginning hobby game dev.

Eventually, I ceased development (i.e., gave up) and began learning Java, in hopes that I would be better at that. Here's one of my favorite pieces of code I came up with (it creates what looks like hand-written code to test if a number is even or odd for the first 10,000 natural numbers):

    package writeToFile;
    
    import java.io.File;
    import java.io.FileWriter;
    import java.io.IOException;
    
    public class MyJokeFileWriter {
    
    	public static File createFile() {
    		try {
    			File myFile = new File("CS111_EvenOdd.txt");
    			
    			if (myFile.createNewFile()) {
    				System.out.println("File created: " + myFile.getName());
    			} else {
    				System.out.println("File already exists at the following location: " + myFile.getAbsolutePath());
    			}
    			
    			return myFile;
    		} catch (IOException exception) {
    			System.out.println("So sorry, an error occurred:");
    			exception.printStackTrace();
    			return null;
    		}		
    	}
    	
    	public static void writeToFile(File inputFile) {
    		try {
    			FileWriter myFileWriter = new FileWriter("CS111_EvenOdd.txt");
    			
    			myFileWriter.write("//This function checks from 1 - 1M if the input integer is even\npublic boolean isEven(int inputInt) {\n	if (inputInt == 1) {\n		return false;\n	}");
    			
    			for (int i = 0; i < 1000000; i++) {
    				String outputLine;
    				
    				if (i % 2 == 0) {
    					outputLine = ") {\n		return false;\n	}";
    				} else {
    					outputLine = ") {\n		return true;\n	}";
    				}
    				myFileWriter.write(" else if (inputInt == " + (i + 1) + outputLine);
    			}
    			
    			myFileWriter.write("\n}");
    			myFileWriter.close();
    			
    			System.out.println("Successfully wrote to file");
    		} catch (IOException exception) {
    			System.out.println("The following error occurred: ");
    			exception.printStackTrace();
    		}
    	}
    }

And that's a little about me! I hope you enjoyed.

\- *Sage*
