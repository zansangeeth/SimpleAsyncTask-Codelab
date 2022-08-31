<h1 align="center">Create Async Task</h1>

**AsyncTask** is an abstract class, which means you must subclass it in order to use it. In this example the AsyncTask performs a very simple background task: it sleeps for a random amount of time. In a real app, the background task could perform all sorts of work, from querying a database, to connecting to the internet, to calculating the next Go move to beat the current Go champion.

An **AsyncTask** subclass has the following methods for performing work off of the main thread:

**onPreExecute():** This method runs on the UI thread, and is used for setting up your task (like showing a progress bar).

**doInBackground():** This is where you implement the code to execute the work that is to be performed on the separate thread.

**onProgressUpdate():** This is invoked on the UI thread and used for updating progress in the UI (such as filling up a progress bar)

**onPostExecute():** Again on the UI thread, this is used for updating the results to the UI once the AsyncTask has finished loading.

<p align="center">
  <img width="500" src="https://user-images.githubusercontent.com/42418189/187693761-aaeb815c-429c-495d-b6cd-022fd9224600.png" alt="Material Bread logo">
</p>
