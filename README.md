import React from 'react';
import { motion } from 'framer-motion';
import { 
    Shield, 
    Zap, 
    PlayCircle, 
    GraduationCap, 
    HelpCircle, 
    Wallet,
    ArrowRight,
    BarChart3,
    Brain
} from 'lucide-react';

const features = [
    {
        icon: Brain,
        title: "IA Avançada",
        description: "Algoritmos de machine learning que analisam milhares de dados em tempo real"
    },
    {
        icon: Shield,
        title: "100% Seguro",
        description: "Seus investimentos protegidos com criptografia de ponta"
    },
    {
        icon: Zap,
        title: "Execução Rápida",
        description: "Operações executadas em milissegundos para máximo aproveitamento"
    },
    {
        icon: BarChart3,
        title: "Análise Profunda",
        description: "Relatórios detalhados e insights sobre seus investimentos"
    }
];

const sections = [
    {
        name: "Tutoriais",
        icon: PlayCircle,
        description: "Aprenda a usar nossa plataforma",
        route: "#/tutoriais",
        color: "from-blue-500 to-blue-600"
    },
    {
        name: "Dúvidas",
        icon: HelpCircle,
        description: "Tire suas dúvidas frequentes",
        route: "#/duvidas",
        color: "from-purple-500 to-purple-600"
    },
    {
        name: "Aprendizado",
        icon: GraduationCap,
        description: "Cursos e materiais educacionais",
        route: "#/aprendizado",
        color: "from-orange-500 to-orange-600"
    },
    {
        name: "Como Sacar",
        icon: Wallet,
        description: "Guia completo de saques",
        route: "#/como-sacar",
        color: "from-pink-500 to-pink-600"
    }
];

export default function Home() {
    return (
        <div className="space-y-16">

            {/* HERO */}
            <motion.section
                initial={{ opacity: 0, y: 30 }}
                animate={{ opacity: 1, y: 0 }}
                transition={{ duration: 0.6 }}
                className="relative overflow-hidden rounded-3xl bg-gradient-to-br from-slate-900 via-slate-800 to-slate-900 border border-slate-700/50 p-8 md:p-14"
            >
                <div className="relative z-10 max-w-3xl">
                    <div className="flex items-center gap-4 mb-6">
                        <img 
                            src="https://qtrypzzcjebvfcihiynt.supabase.co/storage/v1/object/public/base44-prod/public/6967a80b5b403989ae162095/6d5e99cb1_ChatGPTImage14dejande202610_35_15.png"
                            alt="Quona Financeira"
                            className="w-20 h-20"
                        />
                        <span className="px-4 py-2 rounded-full bg-amber-500/10 text-amber-400 text-sm">
                            Powered by IA
                        </span>
                    </div>

                    <h1 className="text-4xl md:text-6xl font-bold text-white mb-6">
                        Invista com
                        <span className="block text-transparent bg-clip-text bg-gradient-to-r from-amber-400 to-amber-600">
                            Inteligência Artificial
                        </span>
                    </h1>

                    <p className="text-slate-400 text-lg mb-8">
                        A Quona Financeira analisa o mercado 24h para maximizar seus resultados.
                    </p>

                    <div className="flex flex-wrap gap-4">
                        <a
                            href="https://wa.me/5567998125878"
                            target="_blank"
                            rel="noreferrer"
                            className="px-8 py-4 rounded-xl bg-gradient-to-r from-amber-500 to-amber-600 text-slate-900 font-semibold flex items-center gap-2"
                        >
                            Começar Agora
                            <ArrowRight />
                        </a>

                        <a
                            href="#/tutoriais"
                            className="px-8 py-4 rounded-xl bg-slate-800 text-white border border-slate-700 flex items-center gap-2"
                        >
                            <PlayCircle />
                            Tutoriais
                        </a>
                    </div>
                </div>
            </motion.section>

            {/* FEATURES */}
            <section className="grid md:grid-cols-4 gap-6">
                {features.map((item, i) => (
                    <motion.div
                        key={i}
                        initial={{ opacity: 0, y: 20 }}
                        animate={{ opacity: 1, y: 0 }}
                        transition={{ delay: i * 0.1 }}
                        className="p-6 bg-slate-900/50 rounded-2xl border border-slate-800"
                    >
                        <item.icon className="w-8 h-8 text-amber-400 mb-4" />
                        <h3 className="text-white font-semibold mb-2">{item.title}</h3>
                        <p className="text-slate-400 text-sm">{item.description}</p>
                    </motion.div>
                ))}
            </section>

            {/* SECTIONS */}
            <section className="grid md:grid-cols-2 lg:grid-cols-3 gap-6">
                {sections.map((s, i) => (
                    <a
                        key={i}
                        href={s.route}
                        className="p-6 rounded-2xl bg-slate-900/40 border border-slate-800 hover:border-slate-600 transition"
                    >
                        <div className={`w-14 h-14 rounded-xl bg-gradient-to-br ${s.color} flex items-center justify-center mb-4`}>
                            <s.icon className="text-white" />
                        </div>
                        <h3 className="text-white font-semibold mb-1">{s.name}</h3>
                        <p className="text-slate-400 text-sm">{s.description}</p>
                    </a>
                ))}
            </section>

        </div>
    );
}
