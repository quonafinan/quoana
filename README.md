import React from 'react';
import { Link } from 'react-router-dom';
import { createPageUrl } from '@/utils';
import { motion } from 'framer-motion';
import { 
    TrendingUp, 
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
        page: "Tutoriais",
        color: "from-blue-500 to-blue-600"
    },
    {
        name: "Dúvidas",
        icon: HelpCircle,
        description: "Tire suas dúvidas frequentes",
        page: "Duvidas",
        color: "from-purple-500 to-purple-600"
    },
    {
        name: "Aprendizado",
        icon: GraduationCap,
        description: "Cursos e materiais educacionais",
        page: "Aprendizado",
        color: "from-orange-500 to-orange-600"
    },
    {
        name: "Como Sacar",
        icon: Wallet,
        description: "Guia completo de saques",
        page: "ComoSacar",
        color: "from-pink-500 to-pink-600"
    }
];

export default function Home() {
    return (
        <div className="space-y-16">
            {/* Hero Section */}
            <motion.section
                initial={{ opacity: 0, y: 30 }}
                animate={{ opacity: 1, y: 0 }}
                transition={{ duration: 0.6 }}
                className="relative overflow-hidden rounded-3xl bg-gradient-to-br from-slate-900 via-slate-800 to-slate-900 border border-slate-700/50 p-8 md:p-14"
            >
                <div className="absolute top-0 right-0 w-96 h-96 bg-amber-500/10 rounded-full blur-3xl" />
                <div className="absolute bottom-0 left-0 w-64 h-64 bg-blue-500/10 rounded-full blur-3xl" />
                
                <div className="relative z-10 max-w-3xl">
                    <div className="flex items-center gap-4 mb-6">
                        <img 
                            src="https://qtrypzzcjebvfcihiynt.supabase.co/storage/v1/object/public/base44-prod/public/6967a80b5b403989ae162095/6d5e99cb1_ChatGPTImage14dejande202610_35_15.png" 
                            alt="Quona Financeira"
                            className="w-20 h-20 object-contain"
                        />
                        <div className="inline-flex items-center gap-2 px-4 py-2 rounded-full bg-amber-500/10 border border-amber-500/20 text-amber-400 text-sm">
                            Powered by Artificial Intelligence
                        </div>
                    </div>
                    
                    <h1 className="text-4xl md:text-6xl font-bold text-white mb-6 leading-tight">
                        Invista na Bolsa com 
                        <span className="text-transparent bg-clip-text bg-gradient-to-r from-amber-400 to-amber-600"> Inteligência Artificial</span>
                    </h1>
                    
                    <p className="text-lg md:text-xl text-slate-400 mb-8 leading-relaxed">
                        A Quona Financeira analisa o mercado 24 horas por dia, identificando as melhores oportunidades de investimento para você. Maximize seus lucros com tecnologia de ponta.
                    </p>
                    
                    <div className="flex flex-wrap gap-4">
                        <a 
                            href="https://wa.me/5567998125878?text=Olá! Gostaria de saber mais sobre como investir com a Quona Financeira"
                            target="_blank"
                            rel="noopener noreferrer"
                            className="px-8 py-4 rounded-xl bg-gradient-to-r from-amber-500 to-amber-600 text-slate-900 font-semibold hover:from-amber-400 hover:to-amber-500 transition-all shadow-xl shadow-amber-500/20 flex items-center gap-2"
                        >
                            Começar a Investir
                            <ArrowRight className="w-5 h-5" />
                        </a>
                        <Link 
                            to={createPageUrl('Tutoriais')}
                            className="px-8 py-4 rounded-xl bg-slate-800 text-white font-semibold hover:bg-slate-700 transition-all border border-slate-700 flex items-center gap-2"
                        >
                            <PlayCircle className="w-5 h-5" />
                            Ver Tutoriais
                        </Link>
                    </div>
                </div>
            </motion.section>

            {/* Features */}
            <section>
                <motion.div
                    initial={{ opacity: 0 }}
                    animate={{ opacity: 1 }}
                    transition={{ delay: 0.2 }}
                    className="text-center mb-10"
                >
                    <h2 className="text-3xl font-bold text-white mb-3">Por que escolher a Quona Financeira?</h2>
                    <p className="text-slate-400">Tecnologia avançada para resultados excepcionais</p>
                </motion.div>
                
                <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
                    {features.map((feature, index) => (
                        <motion.div
                            key={feature.title}
                            initial={{ opacity: 0, y: 20 }}
                            animate={{ opacity: 1, y: 0 }}
                            transition={{ delay: 0.3 + index * 0.1 }}
                            className="p-6 rounded-2xl bg-gradient-to-br from-slate-800/50 to-slate-900/50 border border-slate-700/50 hover:border-amber-500/30 transition-all group"
                        >
                            <div className="w-12 h-12 rounded-xl bg-amber-500/10 flex items-center justify-center mb-4 group-hover:bg-amber-500/20 transition-colors">
                                <feature.icon className="w-6 h-6 text-amber-400" />
                            </div>
                            <h3 className="text-lg font-semibold text-white mb-2">{feature.title}</h3>
                            <p className="text-slate-400 text-sm">{feature.description}</p>
                        </motion.div>
                    ))}
                </div>
            </section>

            {/* Sections Navigation */}
            <section>
                <motion.div
                    initial={{ opacity: 0 }}
                    animate={{ opacity: 1 }}
                    transition={{ delay: 0.4 }}
                    className="text-center mb-10"
                >
                    <h2 className="text-3xl font-bold text-white mb-3">Explore Nossa Plataforma</h2>
                    <p className="text-slate-400">Tudo que você precisa para começar a investir</p>
                </motion.div>
                
                <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                    {sections.map((section, index) => (
                        <motion.div
                            key={section.name}
                            initial={{ opacity: 0, y: 20 }}
                            animate={{ opacity: 1, y: 0 }}
                            transition={{ delay: 0.5 + index * 0.1 }}
                        >
                            <Link
                                to={createPageUrl(section.page)}
                                className="block p-6 rounded-2xl bg-slate-900/50 border border-slate-800 hover:border-slate-700 transition-all group"
                            >
                                <div className={`w-14 h-14 rounded-2xl bg-gradient-to-br ${section.color} flex items-center justify-center mb-4 shadow-lg group-hover:scale-110 transition-transform`}>
                                    <section.icon className="w-7 h-7 text-white" />
                                </div>
                                <h3 className="text-xl font-semibold text-white mb-2 group-hover:text-amber-400 transition-colors">
                                    {section.name}
                                </h3>
                                <p className="text-slate-400 text-sm mb-4">{section.description}</p>
                                <span className="text-amber-400 text-sm font-medium flex items-center gap-1">
                                    Acessar <ArrowRight className="w-4 h-4 group-hover:translate-x-1 transition-transform" />
                                </span>
                            </Link>
                        </motion.div>
                    ))}
                </div>
            </section>

            {/* Stats */}
            <motion.section
                initial={{ opacity: 0, y: 20 }}
                animate={{ opacity: 1, y: 0 }}
                transition={{ delay: 0.6 }}
                className="grid grid-cols-2 md:grid-cols-4 gap-6"
            >
                {[
                    { value: "50K+", label: "Investidores" },
                    { value: "R$ 100M+", label: "Investidos" },
                    { value: "98%", label: "Satisfação" },
                    { value: "24/7", label: "Suporte" }
                ].map((stat, index) => (
                    <div key={index} className="text-center p-6 rounded-2xl bg-slate-900/30 border border-slate-800/50">
                        <div className="text-3xl md:text-4xl font-bold text-transparent bg-clip-text bg-gradient-to-r from-amber-400 to-amber-600 mb-1">
                            {stat.value}
                        </div>
                        <div className="text-slate-400 text-sm">{stat.label}</div>
                    </div>
                ))}
            </motion.section>
        </div>
    );
}
