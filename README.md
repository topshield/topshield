import React from "react";

export default function Dashboard() {
  return (
    <div className="min-h-screen bg-black text-orange-400 p-6 font-mono">
      {/* Header */}
      <header className="flex justify-between items-center mb-8">
        <h1 className="text-3xl font-bold tracking-widest text-orange-500">
          CODE HUB
        </h1>
        <div className="text-sm opacity-70">commit-to-master</div>
      </header>

      {/* Main Grid */}
      <div className="grid grid-cols-1 md:grid-cols-3 gap-6">
        {/* Sidebar */}
        <div className="bg-zinc-900 rounded-2xl p-4 shadow-lg border border-orange-500/20">
          <h2 className="text-lg mb-4 text-orange-300">Navigation</h2>
          <ul className="space-y-2 text-sm">
            <li className="hover:text-orange-500 cursor-pointer">Repositories</li>
            <li className="hover:text-orange-500 cursor-pointer">Commits</li>
            <li className="hover:text-orange-500 cursor-pointer">Pull Requests</li>
            <li className="hover:text-orange-500 cursor-pointer">Issues</li>
          </ul>
        </div>

        {/* Main Content */}
        <div className="md:col-span-2 space-y-6">
          {/* Repo Card */}
          <div className="bg-zinc-900 rounded-2xl p-5 shadow-lg border border-orange-500/20">
            <h2 className="text-xl text-orange-400 mb-2">commit-to-master</h2>
            <p className="text-sm opacity-70">
              A GitHub dashboard styled UI with dark orange aesthetic.
            </p>
          </div>

          {/* Stats */}
          <div className="grid grid-cols-2 gap-4">
            <div className="bg-zinc-900 p-4 rounded-xl border border-orange-500/20">
              <p className="text-sm">Commits</p>
              <h3 className="text-2xl text-orange-500">128</h3>
            </div>
            <div className="bg-zinc-900 p-4 rounded-xl border border-orange-500/20">
              <p className="text-sm">Repos</p>
              <h3 className="text-2xl text-orange-500">12</h3>
            </div>
          </div>

          {/* Activity */}
          <div className="bg-zinc-900 rounded-2xl p-5 border border-orange-500/20">
            <h2 className="text-lg mb-3 text-orange-300">Recent Activity</h2>
            <ul className="text-sm space-y-2 opacity-80">
              <li>✔ Fixed bug in auth system</li>
              <li>✔ Added new dashboard UI</li>
              <li>✔ Updated README</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  );
}
