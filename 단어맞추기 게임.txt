package Project;
import java.util.*;
import java.io.*;


public class Word_Game {
	public static void main(String[] args) {
		
	String word[] = {"연필","안경","공책","생각","눈썹"}; 
	int cho; //랜덤 변수 
	int usr;
	
	String[] CHO = {"ㄱ","ㄲ","ㄴ","ㄷ","ㄸ","ㄹ","ㅁ","ㅂ","ㅃ",
			"ㅅ","ㅆ","ㅇ","ㅈ","ㅉ","ㅊ","ㅋ","ㅌ","ㅍ","ㅎ"};
	String[] JOONG = {"ㅏ","ㅐ","ㅑ","ㅒ","ㅓ","ㅔ","ㅕ","ㅖ","ㅗ","ㅘ",
			"ㅙ","ㅚ","ㅛ","ㅜ","ㅝ","ㅞ","ㅟ","ㅠ","ㅡ","ㅢ","ㅣ"};	
	String[] JONG = {"","ㄱ","ㄲ","ㄳ","ㄴ","ㄵ","ㄶ","ㄷ","ㄹ","ㄺ","ㄻ","ㄼ",
			"ㄽ","ㄾ","ㄿ","ㅀ","ㅁ","ㅂ","ㅄ","ㅅ","ㅆ","ㅇ","ㅈ","ㅊ","ㅋ","ㅌ","ㅍ","ㅎ"};

	
	public Word_Game() throws IOException{
		Random r = new Random();				//랜덤으로 출력
		cho = Math.abs(r.nextInt()%word.length);	//cho에 랜덤값을 저장
			
	System.out.print("▶단어 맞추기 게임◀");			//게임 시작
	
	Scanner sc = new Scanner(System.in);
	String usr = sc.next();
	
	//한자리식 비교하면 될듯!
	
	
	switch{
	case 1:
		System.out.print("■■■■■");	//체력바 
		break;
	case 2:
		System.out.print("■■■■□");	//1번 틀릴시
		break;
	case 3:
		System.out.print("■■■□□");	//2번 틀릴시
		break;
	case 4:
		System.out.print("■■□□□");	//3번 틀릴시
		break;
	case 5:
		System.out.print("■□□□□");	//4번 틀릴시
		break;
	case 6:
		System.out.print("□□□□□");	//모두 늘렸을때
		break;
	}
	
	if(usr==cho) 
		System.out.print("성공");	//사용자의 입력값과 컴퓨터 랜덤의 값이 같을 경우.
	else
		System.out.print("실패");//입력값과 랜덤값이 다를경우
	

		}
	}
}
	


