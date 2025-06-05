function MainComponent() {
  return (
    <div className="min-h-screen bg-[#0d1117] text-white p-8 font-roboto">
      <div className="max-w-3xl mx-auto">
        <div className="bg-[#161b22] rounded-lg p-6 mb-6">
          <div className="flex items-center mb-4">
            <i className="fas fa-code-branch text-[#58a6ff] text-2xl mr-3"></i>
            <h1 className="text-2xl font-bold">Hi there 👋</h1>
          </div>
          <p className="text-gray-300 mb-4">
            I'm a Cad Automation Trainee at Fdes Technologies Private Limited
          </p>
        </div>

        <div className="grid gap-6">
          <div className="bg-[#161b22] rounded-lg p-6">
            <h2 className="flex items-center text-xl mb-3">
              <i className="fas fa-laptop-code text-[#58a6ff] mr-2"></i>
              About Me
            </h2>
            <ul className="space-y-2 text-gray-300">
              <li className="flex items-center">
                <i className="fas fa-briefcase text-gray-500 w-6"></i>
                Currently working on CAD automation and workflow optimization
              </li>
              <li className="flex items-center">
                <i className="fas fa-graduation-cap text-gray-500 w-6"></i>
                Learning advanced CAD automation techniques
              </li>
              <li className="flex items-center">
                <i className="fas fa-heart text-gray-500 w-6"></i>
                Passionate about improving design processes
              </li>
            </ul>
          </div>

          <div className="bg-[#161b22] rounded-lg p-6">
            <h2 className="flex items-center text-xl mb-3">
              <i className="fas fa-chart-line text-[#58a6ff] mr-2"></i>
              Focus Areas
            </h2>
            <div className="grid grid-cols-1 md:grid-cols-2 gap-4 text-gray-300">
              <div className="flex items-center">
                <i className="fas fa-cogs text-green-400 mr-2"></i>
                Process Automation
              </div>
              <div className="flex items-center">
                <i className="fas fa-drafting-compass text-purple-400 mr-2"></i>
                CAD Development
              </div>
              <div className="flex items-center">
                <i className="fas fa-code text-yellow-400 mr-2"></i>
                Workflow Scripting
              </div>
              <div className="flex items-center">
                <i className="fas fa-project-diagram text-blue-400 mr-2"></i>
                System Integration
              </div>
            </div>
          </div>

          <div className="bg-[#161b22] rounded-lg p-6">
            <h2 className="flex items-center text-xl mb-3">
              <i className="fas fa-star text-[#58a6ff] mr-2"></i>
              Goals
            </h2>
            <ul className="space-y-2 text-gray-300">
              <li className="flex items-center">
                <i className="fas fa-check text-green-400 mr-2"></i>
                Enhance team productivity through automation
              </li>
              <li className="flex items-center">
                <i className="fas fa-check text-green-400 mr-2"></i>
                Develop innovative CAD solutions
              </li>
              <li className="flex items-center">
                <i className="fas fa-check text-green-400 mr-2"></i>
                Create efficient design workflows
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  );
}


