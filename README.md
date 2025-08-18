import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";

export default function HomePage() {
  return (
    <div className="font-sans text-gray-800">
      {/* Hero Section */}
      <section className="bg-pink-100 py-16 text-center">
        <h1 className="text-4xl font-bold mb-4">
          Advancing Breast Imaging and Women’s Health in Sudan
        </h1>
        <p className="text-lg mb-6 max-w-2xl mx-auto">
          The Sudanese Society of Breast Imaging and Women’s Health (SSBIWH) promotes excellence in education, research, and patient care.
        </p>
        <div className="space-x-4">
          <Button className="bg-pink-600 text-white">Join Us</Button>
          <Button variant="outline">Upcoming Events</Button>
        </div>
      </section>

      {/* About Us */}
      <section className="py-12 px-6 md:px-20 text-center">
        <h2 className="text-3xl font-semibold mb-4">Who We Are</h2>
        <p className="max-w-3xl mx-auto mb-6">
          The SSBIWH unites radiologists, oncologists, surgeons, and allied professionals to improve breast imaging and women’s health in Sudan. We provide education, research support, and collaboration opportunities to enhance patient outcomes.
        </p>
        <Button variant="outline">Learn More</Button>
      </section>

      {/* Focus Areas */}
      <section className="grid md:grid-cols-3 gap-6 px-6 md:px-20 py-12 text-center">
        {[
          { icon: "📚", title: "Education & Training", text: "CME, workshops, journal clubs" },
          { icon: "🔬", title: "Research & Innovation", text: "National audits, publications" },
          { icon: "🤝", title: "Collaboration & Support", text: "Multidisciplinary teamwork" },
        ].map((item, idx) => (
          <Card key={idx} className="shadow-md rounded-2xl">
            <CardContent className="p-6">
              <div className="text-4xl mb-3">{item.icon}</div>
              <h3 className="font-bold text-xl mb-2">{item.title}</h3>
              <p>{item.text}</p>
            </CardContent>
          </Card>
        ))}
      </section>

      {/* Events & News */}
      <section className="bg-gray-50 py-12 px-6 md:px-20">
        <h2 className="text-3xl font-semibold text-center mb-6">Latest Updates</h2>
        <ul className="list-disc max-w-2xl mx-auto text-left mb-6">
          <li>Breast Imaging Symposium – November 2025 (Khartoum)</li>
          <li>Monthly Journal Club – First Friday of each month (via Zoom)</li>
          <li>CEM Protocol Update – Published 2025</li>
        </ul>
        <div className="text-center">
          <Button variant="outline">View All Events</Button>
        </div>
      </section>

      {/* Membership */}
      <section className="py-12 px-6 md:px-20 text-center">
        <h2 className="text-3xl font-semibold mb-4">Become a Member</h2>
        <p className="max-w-2xl mx-auto mb-6">
          Join a professional community dedicated to advancing breast imaging and women’s health.
        </p>
        <ul className="max-w-xl mx-auto mb-6 list-disc text-left">
          <li>Access to guidelines and resources</li>
          <li>Reduced fees for workshops and conferences</li>
          <li>Networking and research opportunities</li>
        </ul>
        <Button className="bg-pink-600 text-white">Join Now</Button>
      </section>

      {/* Research */}
      <section className="bg-gray-50 py-12 px-6 md:px-20 text-center">
        <h2 className="text-3xl font-semibold mb-4">Our Research</h2>
        <p className="mb-6">We lead impactful studies and national audits:</p>
        <ul className="max-w-2xl mx-auto list-disc text-left">
          <li>AVOID Audit – Sudanese contribution</li>
          <li>Contrast-Enhanced Mammography (CEM) Protocol</li>
          <li>Breast Cancer in Pregnancy presentations</li>
        </ul>
        <Button variant="outline">Explore Research</Button>
      </section>

      {/* Contact Section */}
      <section className="py-12 px-6 md:px-20 text-center">
        <h2 className="text-3xl font-semibold mb-4">Contact Us</h2>
        <p className="mb-2">For enquiries and membership, reach us at:</p>
        <p className="font-bold text-lg">📧 ssbiwh.1@gmail.com</p>
      </section>

      {/* Footer */}
      <footer className="bg-pink-900 text-white py-8 text-center">
        <p>Email: ssbiwh.1@gmail.com | Address: Khartoum, Sudan</p>
        <p className="mt-2">© 2025 Sudanese Society of Breast Imaging & Women’s Health</p>
      </footer>
    </div>
  );
}
