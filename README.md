"use client";
import React from "react";

function MainComponent() {
  return (
    <div className="min-h-screen bg-[#0d1117] text-white p-8 font-roboto">
      <style jsx global>{`
        @keyframes pulse {
          0% { transform: scale(1); }
          50% { transform: scale(1.05); }
          100% { transform: scale(1); }
        }
        
        @keyframes glow {
          0% { box-shadow: 0 0 5px rgba(255, 121, 198, 0.5); }
          50% { box-shadow: 0 0 20px rgba(255, 121, 198, 0.8); }
          100% { box-shadow: 0 0 5px rgba(255, 121, 198, 0.5); }
        }

        .skill-card:hover {
          transform: translateY(-5px);
          transition: transform 0.3s ease;
        }

        .connect-button:hover {
          animation: pulse 1s infinite;
        }

        .section-card:hover {
          animation: glow 2s infinite;
        }

        .badge:hover {
          transform: scale(1.1);
          transition: transform 0.2s ease;
        }
      `}</style>

      <div className="max-w-4xl mx-auto">
        {/* Header Section */}
        <div className="text-center mb-8">
          <h1 className="text-3xl font-bold mb-4 hover:text-[#ff79c6] transition-colors duration-300">
            👋 Hi, I'm <span className="text-[#ff79c6]">Chandhu Swargam</span>!
          </h1>
          <div className="flex flex-wrap justify-center gap-3 mb-6">
            <span className="badge bg-blue-600 px-3 py-1 rounded-md text-sm hover:bg-blue-700 transition-all duration-300">
              <i className="fas fa-cube mr-2"></i>CAD Automation
            </span>
            <span className="badge bg-[#8A2BE2] px-3 py-1 rounded-md text-sm hover:bg-[#9A3BF2] transition-all duration-300">
              <i className="fas fa-code mr-2"></i>C# | .NET
            </span>
            <span className="badge bg-orange-600 px-3 py-1 rounded-md text-sm hover:bg-orange-700 transition-all duration-300">
              <i className="fas fa-coffee mr-2"></i>Java
            </span>
            <span className="badge bg-[#5cb85c] px-3 py-1 rounded-md text-sm hover:bg-[#6cc86c] transition-all duration-300">
              <i className="fas fa-building mr-2"></i>Fdes Technologies
            </span>
          </div>
        </div>

        {/* About Me Section */}
        <div className="section-card bg-[#161b22] rounded-lg p-6 mb-8 transition-all duration-300">
          <h2 className="text-xl font-bold mb-4 flex items-center">
            <i className="fas fa-lightbulb text-[#ff79c6] mr-2"></i>
            About Me
          </h2>
          <ul className="space-y-3 text-gray-300">
            <li className="flex items-center hover:bg-[#1f2937] p-2 rounded-lg transition-all duration-300">
              <i className="fas fa-bullseye text-[#ff79c6] w-6"></i>
              <span>
                <b>Current Role:</b> Cad Automation Trainee @ Fdes Technologies
                Private Limited
              </span>
            </li>
            <li className="flex items-center hover:bg-[#1f2937] p-2 rounded-lg transition-all duration-300">
              <i className="fas fa-bolt text-[#ff79c6] w-6"></i>
              <span>
                <b>Passion:</b> Creating efficient logic & automating CAD
                workflows for real productivity
              </span>
            </li>
            <li className="flex items-center hover:bg-[#1f2937] p-2 rounded-lg transition-all duration-300">
              <i className="fas fa-puzzle-piece text-[#ff79c6] w-6"></i>
              <span>
                <b>Interests:</b> Exploring new ways to enhance productivity
                with CAD tools & code
              </span>
            </li>
          </ul>
        </div>

        {/* Skills Section */}
        <div className="section-card bg-[#161b22] rounded-lg p-6 mb-8 transition-all duration-300">
          <h2 className="text-xl font-bold mb-4 flex items-center">
            <i className="fas fa-tools text-[#ff79c6] mr-2"></i>
            Top Skills
          </h2>
          <div className="space-y-4">
            <div className="skill-card flex items-start gap-4 p-3 bg-[#1f2937] rounded-lg transition-all duration-300">
              <div className="text-blue-500 text-2xl pt-1">
                <i className="fas fa-drafting-compass"></i>
              </div>
              <div>
                <h3 className="font-bold">AutoCAD Automation</h3>
                <p className="text-sm text-gray-400">
                  Scripting & automating tasks to reduce manual work
                </p>
              </div>
            </div>
            <div className="skill-card flex items-start gap-4 p-3 bg-[#1f2937] rounded-lg transition-all duration-300">
              <div className="text-green-500 text-2xl pt-1">
                <i className="fas fa-code"></i>
              </div>
              <div>
                <h3 className="font-bold">C# .NET Framework</h3>
                <p className="text-sm text-gray-400">
                  Building Windows Forms apps for CAD integration
                </p>
              </div>
            </div>
            <div className="skill-card flex items-start gap-4 p-3 bg-[#1f2937] rounded-lg transition-all duration-300">
              <div className="text-orange-500 text-2xl pt-1">
                <i className="fas fa-coffee"></i>
              </div>
              <div>
                <h3 className="font-bold">Java (Basics)</h3>
                <p className="text-sm text-gray-400">
                  Foundation in OOP & programming logic
                </p>
              </div>
            </div>
          </div>
        </div>

        {/* Notable Project Section */}
        <div className="section-card bg-[#161b22] rounded-lg p-6 mb-8 transition-all duration-300">
          <h2 className="text-xl font-bold mb-4 flex items-center">
            <i className="fas fa-star text-[#ff79c6] mr-2"></i>
            Notable Project
          </h2>
          <div className="bg-[#1f2937] p-4 rounded-lg hover:bg-[#2d3748] transition-all duration-300">
            <h3 className="font-bold text-lg mb-2">
              Automating Block Manipulation in AutoCAD
            </h3>
            <p className="text-gray-300 mb-3">🛠️ Developed a tool that:</p>
            <ul className="list-disc list-inside text-gray-300 space-y-1 ml-4">
              <li className="hover:text-[#ff79c6] transition-colors duration-300">
                Activates external DWG files
              </li>
              <li className="hover:text-[#ff79c6] transition-colors duration-300">
                Fetches all blocks in Model Space
              </li>
              <li className="hover:text-[#ff79c6] transition-colors duration-300">
                Programmatically copies, manipulates dynamic properties, and
                edits block attributes via command-line
              </li>
            </ul>
            <p className="text-sm text-gray-400 mt-3 italic">
              This project demonstrates my drive to automate and optimize
              real-world CAD tasks with code!
            </p>
          </div>
        </div>

        {/* What Drives Me Section */}
        <div className="section-card bg-[#161b22] rounded-lg p-6 mb-8 transition-all duration-300">
          <h2 className="text-xl font-bold mb-4 flex items-center">
            <i className="fas fa-brain text-[#ff79c6] mr-2"></i>
            What Drives Me
          </h2>
          <p className="text-gray-300 hover:text-white transition-colors duration-300">
            I love crafting logical solutions that make complex tasks easier.
            Whether automating repetitive CAD operations or designing smarter
            workflows, I'm always eager to tackle challenges and expand my
            expertise.
          </p>
        </div>

        {/* Connect Section */}
        <div className="text-center">
          <h2 className="text-xl font-bold mb-4">📫 Connect With Me</h2>
          <a
            href="https://www.linkedin.com/in/chandhu-swargam/"
            className="connect-button inline-flex items-center bg-blue-600 px-4 py-2 rounded-md hover:bg-blue-700 transition-all duration-300"
          >
            <i className="fab fa-linkedin mr-2"></i>
            Connect on LinkedIn
          </a>
        </div>

        {/* Fun Fact */}
        <div className="mt-8 text-center">
          <details className="inline-block">
            <summary className="cursor-pointer hover:text-[#ff79c6] transition-colors duration-300">
              🎉 <b>Fun Fact</b>
            </summary>
            <p className="mt-2 hover:text-[#ff79c6] transition-colors duration-300">
              I believe:{" "}
              <b>"A few lines of logic can save hours of manual work!"</b> 💡
            </p>
          </details>
        </div>
      </div>
    </div>
  );
}

export default MainComponent;
