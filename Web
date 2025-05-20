import React from "react"; import { Card, CardContent } from "@/components/ui/card"; import { Button } from "@/components/ui/button"; import { Input } from "@/components/ui/input"; import { motion } from "framer-motion";

const projects = [ { title: "Logo Design - TechNova", image: "/images/technova-logo.png", description: "A sleek and modern logo for a tech startup." }, { title: "Poster - Earth Day Campaign", image: "/images/earth-day-poster.png", description: "Environmental awareness poster for a local NGO." }, { title: "Business Card - Urban Cafe", image: "/images/urban-cafe-card.png", description: "Minimalist business card design for a coffee shop." } ];

const testimonials = [ { name: "James Mwangi", feedback: "Professional, timely, and truly creative. Highly recommended!" }, { name: "Linet Achieng", feedback: "Delivered a beautiful logo that captured my brand perfectly." }, { name: "Tony Kimani", feedback: "Easy to work with and really understands design needs." } ];

const fadeIn = { hidden: { opacity: 0, y: 20 }, visible: (i = 1) => ({ opacity: 1, y: 0, transition: { delay: i * 0.2, duration: 0.6 } }) };

export default function PortfolioSite() { return ( <div className="p-6 max-w-6xl mx-auto"> <motion.h1 className="text-4xl font-bold mb-4 text-center" initial="hidden" animate="visible" variants={fadeIn} > My Graphic Design Portfolio </motion.h1>

<motion.p
    className="text-center mb-10 text-gray-600"
    initial="hidden" animate="visible" variants={fadeIn} custom={1}
  >
    Showcasing my creativity, design skills, and visual storytelling.
  </motion.p>

  <div className="grid md:grid-cols-3 gap-6">
    {projects.map((project, index) => (
      <motion.div
        key={index}
        className="shadow-lg rounded-2xl overflow-hidden"
        initial="hidden"
        animate="visible"
        variants={fadeIn}
        custom={index + 1}
      >
        <Card>
          <img src={project.image} alt={project.title} className="rounded-t-2xl w-full h-48 object-cover hover:scale-105 transition-transform duration-300" />
          <CardContent>
            <h2 className="text-xl font-semibold mt-2">{project.title}</h2>
            <p className="text-sm text-gray-500 mt-1">{project.description}</p>
          </CardContent>
        </Card>
      </motion.div>
    ))}
  </div>

  <motion.div className="mt-16" initial="hidden" animate="visible" variants={fadeIn} custom={4}>
    <h2 className="text-2xl font-semibold text-center mb-4">Testimonials</h2>
    <div className="grid md:grid-cols-3 gap-6">
      {testimonials.map((testimonial, index) => (
        <motion.div
          key={index}
          className="bg-gray-50 p-4 rounded-2xl shadow-md"
          initial="hidden"
          animate="visible"
          variants={fadeIn}
          custom={index + 5}
        >
          <CardContent>
            <p className="italic text-gray-700">"{testimonial.feedback}"</p>
            <p className="mt-2 text-sm font-semibold text-right">— {testimonial.name}</p>
          </CardContent>
        </motion.div>
      ))}
    </div>
  </motion.div>

  <motion.div className="mt-12 text-center" initial="hidden" animate="visible" variants={fadeIn} custom={8}>
    <h2 className="text-2xl font-semibold mb-2">Let's Work Together</h2>
    <p className="mb-4 text-gray-500">Send me your project idea or inquiry below.</p>
    <div className="flex flex-col md:flex-row justify-center gap-2 max-w-md mx-auto">
      <Input placeholder="Your email" />
      <Button className="transition duration-300 hover:scale-105">Contact Me</Button>
    </div>
  </motion.div>
</div>

); }

