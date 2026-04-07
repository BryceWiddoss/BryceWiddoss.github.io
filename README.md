import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Mail, Linkedin, Github } from "lucide-react";

export default function Portfolio() {
return ( <div className="min-h-screen bg-gray-50 text-gray-900 p-6">
{/* Header */} <header className="max-w-5xl mx-auto flex justify-between items-center mb-12"> <h1 className="text-2xl font-bold">Bryce Widdoss</h1> <div className="flex gap-4"> <a href="https://linkedin.com/in/bryce-widdoss" target="_blank"> <Linkedin /> </a> <a href="https://github.com/BryceWiddoss" target="_blank"> <Github /> </a> <a href="mailto:brycewiddoss@gmail.com"> <Mail /> </a> </div> </header>

```
  {/* Hero */}
  <section className="max-w-5xl mx-auto mb-16">
    <h2 className="text-4xl font-bold mb-4">
      Software Engineer
    </h2>
    <p className="text-lg text-gray-600 max-w-2xl">
      I build applications in Python and have a backhground solvimg real-world problems with clean, readable code.
    </p>
  </section>

  {/* Projects */}
  <section className="max-w-5xl mx-auto mb-16">
    <h3 className="text-2xl font-semibold mb-6">Projects</h3>
    <div className="grid md:grid-cols-2 gap-6">

      <Card className="rounded-2xl shadow">
        <CardContent className="p-4">
          <h4 className="text-xl font-bold mb-2">Project One</h4>
          <p className="text-gray-600 mb-3">
            Brief description of what this project does and why it matters.
          </p>
          <div className="flex gap-3">
            <Button asChild>
              <a href="#">Live Demo</a>
            </Button>
            <Button variant="outline" asChild>
              <a href="#">GitHub</a>
            </Button>
          </div>
        </CardContent>
      </Card>

      <Card className="rounded-2xl shadow">
        <CardContent className="p-4">
          <h4 className="text-xl font-bold mb-2">Project Two</h4>
          <p className="text-gray-600 mb-3">
            Another impactful project with clear results.
          </p>
          <div className="flex gap-3">
            <Button asChild>
              <a href="#">Live Demo</a>
            </Button>
            <Button variant="outline" asChild>
              <a href="#">GitHub</a>
            </Button>
          </div>
        </CardContent>
      </Card>

    </div>
  </section>

  {/* Contact */}
  <section className="max-w-5xl mx-auto text-center">
    <h3 className="text-2xl font-semibold mb-4">Get In Touch</h3>
    <p className="text-gray-600 mb-6">
      Open to software engineering opportunities. Let’s connect.
    </p>
    <Button asChild>
      <a href="mailto:your-email@example.com">Email Me</a>
    </Button>
  </section>

  {/* Footer */}
  <footer className="text-center text-sm text-gray-500 mt-16">
    © {new Date().getFullYear()} Bryce Widdoss
  </footer>
</div>
```

);
}
