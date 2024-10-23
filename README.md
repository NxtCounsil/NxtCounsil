import React from 'react'
import { Card, CardContent } from "@/components/ui/card"
import { Badge } from "@/components/ui/badge"
import { ArrowRight, Code, Cpu, Database, Globe, Lightbulb, Rocket } from 'lucide-react'

export default function Component() {
  return (
    <div className="min-h-screen bg-gradient-to-br from-gray-900 to-gray-800 text-white p-8 font-mono">
      <Card className="max-w-4xl mx-auto bg-black/50 border-gray-700">
        <CardContent className="p-6">
          <h1 className="text-4xl font-bold mb-4 bg-clip-text text-transparent bg-gradient-to-r from-blue-400 to-purple-600">
            Your Name
          </h1>
          <p className="text-xl mb-6 text-gray-300">Full-Stack Developer | AI Enthusiast | Open Source Contributor</p>
          
          <div className="space-y-6">
            <section>
              <h2 className="text-2xl font-semibold mb-3 flex items-center">
                <Rocket className="mr-2" /> Mission
              </h2>
              <p className="text-gray-300">
                Pushing the boundaries of technology to create innovative solutions that shape the future.
              </p>
            </section>

            <section>
              <h2 className="text-2xl font-semibold mb-3 flex items-center">
                <Lightbulb className="mr-2" /> Current Focus
              </h2>
              <ul className="list-disc list-inside text-gray-300">
                <li>Exploring the intersection of AI and web technologies</li>
                <li>Contributing to open-source projects that make a difference</li>
                <li>Building scalable and efficient full-stack applications</li>
              </ul>
            </section>

            <section>
              <h2 className="text-2xl font-semibold mb-3 flex items-center">
                <Code className="mr-2" /> Tech Arsenal
              </h2>
              <div className="flex flex-wrap gap-2">
                {['JavaScript', 'TypeScript', 'React', 'Node.js', 'Python', 'GraphQL', 'Docker', 'Kubernetes', 'AWS'].map((tech) => (
                  <Badge key={tech} variant="secondary" className="text-sm py-1 px-2 bg-gray-700 text-gray-200">
                    {tech}
                  </Badge>
                ))}
              </div>
            </section>

            <section>
              <h2 className="text-2xl font-semibold mb-3 flex items-center">
                <Globe className="mr-2" /> Let's Connect
              </h2>
              <p className="text-gray-300">
                I'm always open to discussing new projects, creative ideas, or opportunities to be part of your visions.
              </p>
            </section>

            <section>
              <h2 className="text-2xl font-semibold mb-3 flex items-center">
                <Cpu className="mr-2" /> Fun Fact
              </h2>
              <p className="text-gray-300">
                I once debugged a production issue while on a roller coaster. Talk about a wild ride!
              </p>
            </section>

            <section>
              <h2 className="text-2xl font-semibold mb-3 flex items-center">
                <Database className="mr-2" /> Latest Project
              </h2>
              <p className="text-gray-300">
                Currently working on a revolutionary AI-powered code assistant that understands context and developer intent.
              </p>
            </section>
          </div>

          <div className="mt-8 text-center">
            <p className="text-lg text-gray-400 flex items-center justify-center">
              Explore my repositories <ArrowRight className="ml-2" />
            </p>
          </div>
        </CardContent>
      </Card>
    </div>
  )
}
