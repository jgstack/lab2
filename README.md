# lab2 
            //declare variables
            int feetInMile = 5280;
            double conversionFactor = 0.413;

            //prompt user for their height (in inches) and assign it to a variable
            Console.WriteLine("Please enter your height in inches:");
            string userInputH = Console.ReadLine();

            //convert connversion factor to an integer and multiply it by user inputted height in inches
            Convert.ToInt32(conversionFactor);
            double strideLengthInches = int.Parse(userInputH) * conversionFactor;

            //divide the stride length in inches by 12 to get stride length in feet
            double strideLengthFeet = strideLengthInches / 12;

            //prompt user for their steps taken and assign it to a variable
            Console.WriteLine("Please enter total number of steps you have taken today:");
            string userInputS = Console.ReadLine();

            //multiply stride length and steps taken to get total feet walked
            double feetWalked = strideLengthFeet * int.Parse(userInputS);

            //divide feet walked by 5280 to convert feet into miles
            double milesWalked = feetWalked / feetInMile;

            //display miles walked to user!
            Console.WriteLine("You have walked this many miles today: " + milesWalked);
            Console.ReadLine();
