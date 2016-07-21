# ReverseAndRemoveVowel
import java.util.Scanner;

public class ReverseAndRemoveVowel {

	public static void main(String[] args) {

		Scanner get = new Scanner(System.in);
		System.out.println("Enter input String");
		String input = get.nextLine();
		StringBuffer nn = new StringBuffer(input);
		StringBuffer output = nn.reverse();
		// System.out.println(output);
		String reverseInput = new String(output);
		char[] gg = reverseInput.toCharArray();
		System.out.println("Output :");
		for (int i = 0; i < gg.length; i++) {
			if (gg[i] == 'a' || gg[i] == 'e' || gg[i] == 'i' || gg[i] == 'o'
					|| gg[i] == 'u') {
				continue;
			}
			System.out.print(gg[i]);
		}

	}

}
