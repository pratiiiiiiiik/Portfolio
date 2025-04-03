import { useEffect } from "react";
import { motion } from "framer-motion";
import { FaGithub, FaLinkedin, FaEnvelope, FaPhone } from "react-icons/fa";
import { Progress } from "@/components/ui/progress";

export default function Portfolio() {
  useEffect(() => {
    document.body.classList.add("dark");
  }, []);

  return (
    <div className="bg-black text-white min-h-screen flex flex-col items-center p-4">
      <motion.header initial={{ opacity: 0, y: -50 }} animate={{ opacity: 1, y: 0 }} transition={{ duration: 1 }} className="w-full text-center py-6 text-[#39ff14] text-4xl font-extrabold tracking-widest">
        Pratik Gangurde
      </motion.header>
      
      <motion.section initial={{ opacity: 0 }} animate={{ opacity: 1 }} transition={{ duration: 1.2 }} className="text-center my-6">
        <p className="text-xl font-semibold text-[#00f7ff]">Cybersecurity Enthusiast | Bug Bounty Hunter | VAPT Specialist</p>
        <p className="text-gray-400">Manmad, Maharashtra, 423104, India</p>
        <p className="text-gray-400">pratikgangurde2019@gmail.com | 9325569362</p>
        <div className="flex justify-center gap-6 mt-4">
          <a href="https://github.com/pratiiiiiiiik" target="_blank" rel="noopener noreferrer"><FaGithub className="text-4xl text-[#39ff14] hover:text-[#00f7ff] transition-all" /></a>
          <a href="https://linkedin.com/in/pratik" target="_blank" rel="noopener noreferrer"><FaLinkedin className="text-4xl text-[#39ff14] hover:text-[#00f7ff] transition-all" /></a>
          <a href="mailto:pratikgangurde2019@gmail.com"><FaEnvelope className="text-4xl text-[#39ff14] hover:text-[#00f7ff] transition-all" /></a>
          <FaPhone className="text-4xl text-[#39ff14] hover:text-[#00f7ff] transition-all" />
        </div>
      </motion.section>
      
      <motion.section initial={{ x: -100 }} animate={{ x: 0 }} transition={{ duration: 1 }} className="w-full max-w-3xl p-6 bg-gray-900 rounded-lg shadow-lg">
        <h2 className="text-[#00f7ff] text-2xl font-semibold mb-4">Education</h2>
        <p>Sanjivani College of Engineering, Kopargaon - B.Tech (IT) (2022-2025) - GPA: 3.12</p>
        <p>Sanjivani College of Engineering, Kopargaon - Diploma in Mechatronics (2020-2022) - GPA: 3.60</p>
      </motion.section>
      
      <motion.section initial={{ x: 100 }} animate={{ x: 0 }} transition={{ duration: 1 }} className="w-full max-w-3xl p-6 bg-gray-900 rounded-lg shadow-lg mt-6">
        <h2 className="text-[#00f7ff] text-2xl font-semibold mb-4">Technical Skills</h2>
        <p className="text-gray-300">Cybersecurity Fundamentals, Security Frameworks, Networking, VAPT, Incident Response, Threat Detection, Linux, OS Security, Wireshark, Metasploit, Burp Suite, Nmap, SIEM, Log Analysis, Malware Detection, NIST, ISO 27001, CIS, Python, Bash Scripting</p>
      </motion.section>
      
      <motion.section initial={{ y: 100 }} animate={{ y: 0 }} transition={{ duration: 1 }} className="w-full max-w-3xl p-6 bg-gray-900 rounded-lg shadow-lg mt-6">
        <h2 className="text-[#00f7ff] text-2xl font-semibold mb-4">Projects</h2>
        <ul className="list-disc pl-5 text-gray-300 space-y-2">
          <li>Key-Driven Image Encryption</li>
          <li>Caesar Cipher CryptoTool</li>
          <li>Exploiting Security Weaknesses in Vehicles</li>
        </ul>
      </motion.section>
      
      <motion.section initial={{ y: 100 }} animate={{ y: 0 }} transition={{ duration: 1 }} className="w-full max-w-3xl p-6 bg-gray-900 rounded-lg shadow-lg mt-6">
        <h2 className="text-[#00f7ff] text-2xl font-semibold mb-4">Achievements</h2>
        <ul className="list-disc pl-5 text-gray-300 space-y-2">
          <li>Master in Cybersecurity and Penetration Testing – Defence Guru Cyber Education Institute</li>
          <li>CCNA – Defence Guru Cyber Education Institute</li>
          <li>VAPT – Defence Guru Cyber Education Institute</li>
          <li>CEH.v13 – Defence Guru Cyber Education Institute</li>
          <li>Junior Security Analyst – Cisco</li>
          <li>Fundamentals of SOC (Security Operations Center) – Palo Alto</li>
          <li>Fundamentals of NOC (Network Operations Center) – Palo Alto</li>
        </ul>
      </motion.section>
      
      <footer className="text-center py-4 mt-6 text-[#00f7ff] text-lg font-semibold">© 2025 Pratik Gangurde</footer>
    </div>
  );
}
