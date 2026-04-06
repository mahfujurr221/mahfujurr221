import React from 'react';

const developer = {
  name: "MD Mahfujur Rahman",
  experience: "4+ Years",
  specialty: "PHP & Laravel",
  techStack: ["Laravel", "Next.js", "React", "Vue", "MySQL"]
};

export default function Portfolio() {
  return (
    <main className="max-w-3xl mx-auto p-6 md:p-12 font-sans text-slate-800">
      <header className="mb-10">
        <h1 className="text-4xl font-extrabold tracking-tight text-slate-900">
          {developer.name}
        </h1>
        <p className="text-xl text-blue-600 font-medium">Full Stack Developer</p>
      </header>

      <section className="mb-8">
        <h2 className="text-2xl font-bold mb-3">Bio</h2>
        <p className="leading-relaxed">
          Senior Developer specializing in **Laravel** ecosystems. I bridge the gap between 
          robust backend architecture and modern frontend frameworks like **Next.js** and **Vue**. 
          Focused on building scalable, high-performance web applications.
        </p>
      </section>

      <section className="mb-10">
        <h2 className="text-2xl font-bold mb-4">Tech Stack</h2>
        <div className="flex flex-wrap gap-2">
          {developer.techStack.map((tech) => (
            <span key={tech} className="px-3 py-1 bg-slate-100 border border-slate-200 rounded-full text-sm font-medium">
              {tech}
            </span>
          ))}
          <span className="px-3 py-1 bg-slate-100 border border-slate-200 rounded-full text-sm font-medium">Docker</span>
          <span className="px-3 py-1 bg-slate-100 border border-slate-200 rounded-full text-sm font-medium">AWS</span>
        </div>
      </section>

      <section className="bg-slate-900 text-slate-50 p-6 rounded-xl shadow-lg font-mono">
        <h2 className="text-blue-400 mb-4 tracking-widest uppercase text-xs">Developer.json</h2>
        <div className="space-y-1 text-sm">
          <p><span className="text-pink-400">const</span> profile = {'{'}</p>
          <p className="ml-4">name: <span className="text-emerald-400">"{developer.name}"</span>,</p>
          <p className="ml-4">core: <span className="text-emerald-400">"{developer.specialty}"</span>,</p>
          <p className="ml-4">exp: <span className="text-emerald-400">"{developer.experience}"</span>,</p>
          <p className="ml-4">status: <span className="text-emerald-400">"Building Great Things"</span></p>
          <p>{'}'};</p>
        </div>
      </section>
    </main>
  );
}
