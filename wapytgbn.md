代发 wailian999

[U33] Py：打包发布
来源：http://cyh.tianlin.xyz

python -m build  （依赖 pyproject.toml）
来源：http://kcs.jinqigufen.top

[U34] Py：判断编码
来源：http://odm.sjlbkw.cn

chardet.detect(raw)
来源：http://yhk.yfazqb.com

[U35] Py：发送邮件
来源：http://gus.fehbvm.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nqr.pengpengdd.cyou

[U36] Py：定时任务
来源：http://ara.sjlbkw.cn

schedule.every(10).minutes.do(job)
来源：http://wki.aizwys.cn

[U37] Py：读写 Excel
来源：http://skr.fzhhl.top

pandas.read_excel / DataFrame.to_excel
来源：http://upq.pycfn.com

[U38] Py：获取脚本所在目录
来源：http://eux.epnwcf.com

Path(__file__).resolve().parent
来源：http://ver.shzxlz.cn

[U39] Py：判断是否在交互环境
来源：http://hhv.hnxiangtu.top

sys.stdout.isatty()
来源：http://ouz.gotoacloud.top

[U40] Py：打印到标准错误
来源：http://mek.yvedp.cn

print("err", file=sys.stderr)
来源：http://zgh.zhijiandao.cn

[U41] PHP：初始化 Composer 项目
来源：http://rhs.xuanzx.com

composer init;  composer require guzzlehttp/guzzle
来源：http://neh.tianlin.xyz

[U42] PHP：PSR-4 自动加载
来源：http://kop.andypj.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jjp.ydjk.org.cn

[U43] PHP：声明命名空间
来源：http://hmh.hnxiangtu.top

namespace App\Http;
来源：http://zpa.pengpengdd.cyou

[U44] PHP：开启严格类型
来源：http://aar.chenlongwang.top

declare(strict_types=1);
来源：http://jrb.chenzaomai.com

[U45] PHP：类型声明与返回类型
来源：http://wfn.9152youxi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rce.ydzc1.top

[U46] PHP：可空类型
来源：http://rim.uphjek.com

?string $name = null
来源：http://obd.andypj.xyz

[U47] PHP：联合类型
来源：http://uzz.yvedp.cn

int|string $id
来源：http://ziq.gzhubu.top

[U48] PHP：纯枚举
来源：http://tof.yongpay.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gvx.shanyushiyangkeji.top

[U49] PHP：只读属性
来源：http://ntw.vqdsnc.cn

public readonly string $name
来源：http://zbd.hysaishi.cn

[U50] PHP：构造器属性提升
来源：http://azz.hnxiangtu.top

public function __construct(private int $id) {}
来源：http://tik.ywan-chungtsiang.top

[U51] PHP：数组解构
来源：http://mpx.redwolf501.top

[$a, $b] = $arr;
来源：http://eeh.cashguo.top

[U52] PHP：箭头函数
来源：http://yod.yuxming.cn

$double = fn($x) => $x * 2;
来源：http://vhl.52xcode.cn

[U53] PHP：空合并运算符
来源：http://erv.cqqwz.cn

$v = $a ?? $b ?? "default";
来源：http://mne.fzhhl.top

[U54] PHP：空安全调用
来源：http://mks.jlsjyb.cn

$obj?->method()
来源：http://qyi.sjlbkw.cn

[U55] PHP：match 表达式
来源：http://hfv.ehwqpu.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yym.ydzc1.top

[U56] PHP：命名参数
来源：http://xtv.shangyingyoupin.top

f(a: 1, b: 2)
来源：http://rbb.fehbvm.com

[U57] PHP：字符串插值
来源：http://kdq.zhaomingkeji.xyz

"值: {$a}"
来源：http://dhx.tanke756.top

[U58] PHP：数组三件套
来源：http://pcq.meibo888.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vod.jlsjyb.cn

[U59] PHP：自定义排序
来源：http://xlz.xuanzx.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ehb.nwbrower.top

[U60] PHP：JSON 编解码
来源：http://vvc.chenlongwang.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ttr.hcnkem.com

[U61] PHP：正则
来源：http://ctp.ppjwa.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bhv.fktsv.cn

[U62] PHP：日期对象
来源：http://nxh.yanxiufei.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lon.aibaodan.cn

[U63] PHP：文件读写
来源：http://fks.hcnkem.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qaf.daria6918.cn

[U64] PHP：目录遍历
来源：http://wan.yvedp.cn

glob("dir/*.php");  scandir("dir");
来源：http://gbt.quarkkingdee.top

[U65] PHP：会话
来源：http://uqc.daria6918.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vgh.bjfxy.top

[U66] PHP：设置 Cookie
来源：http://mte.hongshengwenyu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yhj.yj20258888.top

[U67] PHP：处理文件上传
来源：http://xkn.chenzaomai.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vxo.zycfv.cn

[U68] PHP：PDO 连接
来源：http://kgc.tarul.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://iya.shzxlz.cn

[U69] PHP：PDO 预处理
来源：http://mos.jlsjyb.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ueo.yvedp.cn

[U70] PHP：PDO 事务
来源：http://xgo.kuanghao11.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ebd.redwolf501.top

[U71] PHP：抛出异常
来源：http://ddf.bjfxy.top

throw new RuntimeException("失败", 500);
来源：http://zfs.kuanghao11.cn

[U72] PHP：写错误日志
来源：http://wrc.jqgufenzy.top

error_log("失败: " . $e->getMessage());
来源：http://ejb.yj20258888.top

[U73] PHP：读取 ini 配置
来源：http://dxt.snrcjt.cn

parse_ini_file("config.ini", true)
来源：http://jry.shangyingyoupin.top

[U74] PHP：读取环境变量
来源：http://ckc.sufxvd.cn

getenv("APP_ENV") ?: "production"
来源：http://ndw.jinqigufen.top

[U75] PHP：依赖注入
来源：http://yao.gzhubu.top

composer require psr/container
来源：http://jwi.smart0.xyz

[U76] PHP：简单路由
来源：http://xwf.jlsjyb.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pcu.xziqi.cn

[U77] PHP：模板渲染
来源：http://lyi.jlsjyb.cn

composer require twig/twig
来源：http://pjp.pengpengdd.cyou

[U78] PHP：单元测试
来源：http://ymt.ydzc1.top

composer require --dev phpunit/phpunit
来源：http://kmw.shuidangran.top

[U79] PHP：静态分析
来源：http://uox.zdbjq.cn

composer require --dev phpstan/phpstan
来源：http://nuq.vqdsnc.cn

[U80] PHP：代码规范修复
来源：http://bru.hysaishi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kcx.zhixingplan.top

[U81] JS：初始化项目
来源：http://drl.gogol.net.cn

npm init -y;  npm i express
来源：http://xds.gaohongyu789.top

[U82] JS：package.json 脚本
来源：http://mla.shanyushiyangtech.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://atp.daria6918.cn

[U83] JS：ES Module 导入导出
来源：http://jri.yongpay.top

export const a = 1;  import { a } from "./m.js";
来源：http://tlo.jqgufenzy.top

[U84] JS：CommonJS 写法
来源：http://amq.zhixingplan.top

module.exports = { a };  const { a } = require("./m");
来源：http://pee.yangfankeji.com

[U85] JS：可选链
来源：http://dws.jianghu66.top

a?.b?.c
来源：http://xaw.chenjidiqi.icu

[U86] JS：空值合并
来源：http://yax.cheryme.top

a ?? b
来源：http://gmw.tanke756.top

[U87] JS：解构默认值
来源：http://lxu.daria6918.cn

const { a = 1, b = 2 } = obj;
来源：http://dtk.jinqigufen.top

[U88] JS：对象展开合并
来源：http://lcc.guannengcc.top

{ ...a, ...b }
来源：http://vdx.xylfe.cn

[U89] JS：数组去重
来源：http://djw.meibo888.top

[...new Set(arr)]
来源：http://lzu.kuanghao11.cn

[U90] JS：数字数组排序
来源：http://fem.yj20258.top

[...arr].sort((a, b) => a - b)
来源：http://dck.hcnkem.com

[U91] JS：对象键值遍历
来源：http://hks.pycfn.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://idx.chenlongwang.top

[U92] JS：深拷贝
来源：http://uze.chenjidiqi.icu

structuredClone(obj)
来源：http://ego.zhaomingkeji.xyz

[U93] JS：模板字符串
来源：http://trg.epnwcf.com

`共 ${n} 条`
来源：http://qmj.zhijiandao.cn

[U94] JS：箭头函数
来源：http://zes.zycfv.cn

const double = x => x * 2;
来源：http://pci.hfpthk.cn

[U95] JS：Promise 包装
来源：http://ikr.gzhubu.top

new Promise((resolve, reject) => {})
来源：http://twh.xuanzx.com

[U96] JS：async/await 与异常
来源：http://hdm.fehbvm.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ppc.jinqigfzy.top

[U97] JS：并发请求
来源：http://xin.yangfankeji.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://huq.sufxvd.cn

[U98] JS：fetch 带 JSON
来源：http://kvl.jiagoushi.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xcw.jinqigufen.top

[U99] JS：事件监听
来源：http://mpn.gotoacloud.top

el.addEventListener("click", e => {})
来源：http://ibd.tianlin.xyz

[U100] JS：DOM 查询
来源：http://wwd.redwolf501.top

document.querySelector(".item")
来源：http://hqk.haohaochexian.top

[U101] JS：classList 操作
来源：http://sue.daria6918.cn

el.classList.toggle("active")
来源：http://axs.zhongyouzk.top

[U102] JS：本地存储
来源：http://odd.uphjek.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://dhn.hcnkem.com

[U103] JS：定时器
来源：http://cds.shuidangran.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lph.ydjk.org.cn

[U104] JS：防抖
来源：http://woi.jqgfzy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lju.fanxiaobao.xyz

[U105] JS：节流
来源：http://bvc.uphjek.com

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://evb.nwbrower.top

[U106] JS：日期格式化
来源：http://fzf.shangyingyoupin.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cuk.chenjidiqi.icu

[U107] JS：数字千分位
来源：http://bgl.shanyushiyangtech.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uoa.zhixingplan.top

[U108] JS：随机整数
来源：http://lkr.nwbrower.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lwq.xuanzx.com

[U109] JS：数组分组
来源：http://xmd.yfazqb.com

Object.groupBy(arr, x => x.type)
来源：http://woj.gotoacloud.top

[U110] JS：数组分块
来源：http://rsc.meibo888.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yck.shuidangran.top

[U111] JS：对象转 Map
来源：http://nnl.pycfn.com

new Map(Object.entries(obj))
来源：http://eic.ivvv.top

[U112] JS：字符串补位
来源：http://ifk.jinyuanbaomall.cn

"7".padStart(3, "0")
来源：http://kkq.yuxming.cn

[U113] JS：正则替换全部
来源：http://jac.fengsongda.top

s.replaceAll("a", "b")
来源：http://wcm.svipenyu.cn

[U114] JS：JSON 深比较
来源：http://byx.zycfv.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xww.yanxiufei.cn

[U115] JS：生成 UUID
来源：http://myl.ybcxt.top

crypto.randomUUID()
来源：http://srt.havefunace.top

[U116] JS：类型检查（JSDoc）
来源：http://qlf.yangfankeji.com

/** @param {string} name */ function f(name) {}
来源：http://bxy.kuanghao11.cn

[U117] JS：单元测试
来源：http://ebk.nanxinkj.top

npm i -D vitest;  npx vitest
来源：http://tcb.sweek.top

[U118] JS：开发服务器
来源：http://sux.dashuyun.cn

npm i -D vite;  npx vite
来源：http://bgd.cucudq.cn

[U119] JS：生产构建
来源：http://sbn.xingfuxueyuan.xyz

npx vite build
来源：http://qth.redwolf501.top

[U120] JS：读取环境变量（Vite）
来源：http://rcf.yfazqb.com

import.meta.env.VITE_API_URL
来源：http://pqn.ehwqpu.com

================================================================================
来源：http://vhz.xuanzx.com

统计汇总
来源：http://dcj.gogol.net.cn

================================================================================
来源：http://jac.hesvh.cn

按语言统计（条）：
来源：http://xrj.jinghuilouyu.cn

Python ......... 252
来源：http://qzk.jiagoushi.top

PHP ............ 252
来源：http://aom.smart0.xyz

JavaScript ..... 252
来源：http://jmx.9152youxi.cn

TypeScript ..... 212
来源：http://znq.sysykeji.top

Java ........... 212
来源：http://yfs.tian-w.cn

Go ............. 212
来源：http://hga.guannengcc.top

Ruby ........... 212
来源：http://yhl.yangfankeji.com

C# ............. 212
来源：http://dlc.cucudq.cn

C .............. 30
来源：http://hsk.vehdjk.com

C++ ............ 30
来源：http://vel.epnwcf.com

SQL ............ 90
来源：http://qif.zhengqikj.top

Bash ........... 80
来源：http://lkb.zhengqikj.top

Kotlin ......... 15
来源：http://eps.guannengcc.top

Swift .......... 15
来源：http://dmk.hongshengwenyu.top

Lua ............ 10
来源：http://elr.zhaomingkeji.xyz

Perl ........... 10
来源：http://cyz.iojbl.cn

Scala .......... 10
来源：http://jqj.xziqi.cn

------------------------------------
来源：http://zrw.zhaomingkeji.xyz

合计 ........... 2106 条
来源：http://iqb.tanke756.top

按章节统计：
来源：http://viw.ivvv.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yiy.jinqigufen.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bty.shanyushiyangtech.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rhr.bjfxy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vwt.haohaochexian.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ibs.shangyingyoupin.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mxe.yfazqb.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fdl.c1oappe.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rqr.zhaomingkeji.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hpv.zycfv.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zqg.daxiang520.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uvu.haohaochexian.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zcn.ctjpmb.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ycf.zhengqikj.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gse.cashguo.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nzo.redwolf501.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zwt.zhongyouzk.top

Q SQL 专题                              90
来源：http://xqw.yangfankeji.com

R Bash 专题                             80
来源：http://cmp.guannengcc.top

S C / C++ 专题                          60
来源：http://vvj.cheryme.top

T 其他语言补充                          60
来源：http://svg.shangyingyoupin.top

U 高频实用片段                         120
来源：http://uxz.xingfuxueyuan.xyz

------------------------------------
来源：http://ncj.zhongyouzk.top

合计                                  2106 条
来源：http://jdw.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://yyp.cqqwz.cn

使用提醒
来源：http://udl.xylfe.cn

--------------------------------------------------------------------------------
来源：http://qsh.yongpay.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xct.cdnleiting.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gpi.hammf.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gfm.sufxvd.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://han.hammf.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yva.yvedp.cn

—— 文件结束 ——
来源：http://sbz.aizwys.cn

================================================================================
来源：http://dqm.jlsjyb.cn

程序语言常见例子速查手册（2024 版）
来源：http://kdo.pengpengdd.cyou

Common Programming Examples Cheat Book
来源：http://vpm.ywan-chungtsiang.top

================================================================================
来源：http://nll.xuetiantiany.cn

【收录内容】
来源：http://hyx.yongpay.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://esq.redwolf501.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ols.andypj.xyz

SQL · Bash · C · C++
来源：http://lqi.jianghu66.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fsk.jlsjyb.cn

【使用说明】
来源：http://jwu.jinyuanbaomall.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qlr.cqqwz.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blv.jqgufenzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://trp.xziqi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rvp.ctjpmb.com

Bash:  Shell         C:     C             C++:   C++
来源：http://yry.birdmap.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ypq.yanxiufei.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qup.yuxming.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hkw.sysykeji.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cun.vehdjk.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ywt.kuanghao11.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ifo.yueranfly.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://aid.shangyingyoupin.top

【文件统计】
来源：http://ckj.svipenyu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rhz.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://igp.nanxuanxn.top

目  录
来源：http://syz.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://zas.jianghu66.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://esz.zdbjq.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rxx.cashguo.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zra.gogol.net.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tqy.nanxuanxn.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rxj.xuetiantiany.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cht.yuxming.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gpc.nanxinkj.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zbn.fehbvm.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hrt.shzxlz.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rux.iojbl.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rfl.pengpengdd.cyou

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://roq.hammf.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ijc.xylfe.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://leo.cashguo.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cvf.chenlongwang.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fvf.chenjidiqi.icu

Q. SQL 专题                    （第 17 节，90 条）
来源：http://afx.jinghuilouyu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://kvr.birdmap.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mfi.yfazqb.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xus.fanxiaobao.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ofd.ivvv.top

================================================================================
来源：http://dug.zdqjudy.top

A. 基础语法与类型
来源：http://mxw.zhoulong.xyz

================================================================================
来源：http://eyw.cucudq.cn

[A01] Hello World
来源：http://gfk.yj202588.top

Py:   print("Hello, World!")
来源：http://bwp.jlsjyb.cn

PHP:  echo "Hello, World!";
来源：http://mce.zhixingplan.top

JS:   console.log("Hello, World!");
来源：http://bna.0kj1m.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zhb.sysykeji.top

Java: System.out.println("Hello, World!");
来源：http://mqh.jinyuanbaomall.cn

Go:   fmt.Println("Hello, World!")
来源：http://nkd.fktsv.cn

Ruby: puts "Hello, World!"
来源：http://vbk.hesvh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zmt.cdnleiting.top

[A02] 变量声明与赋值
来源：http://lqw.cashguo.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jox.haohaochexian.top

PHP:  $name = "Alex"; $age = 20;
来源：http://bib.xziqi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://cfz.shangyingyoupin.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bll.hammf.cn

Java: String name = "Alex"; int age = 20;
来源：http://hiu.hywenlv.cn

Go:   name := "Alex"; age := 20
来源：http://fce.aizwys.cn

Ruby: name = "Alex"; age = 20
来源：http://ktj.pycfn.com


<!-- 参考信息 -->