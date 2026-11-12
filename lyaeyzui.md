代发 wailian999

[U31] Py：单测
来源：http://baq.hysaishi.cn

python -m pytest -q
来源：http://xvx.svipenyu.cn

[U32] Py：代码格式化
来源：http://sbb.jinqigufen.top

ruff format . && ruff check --fix .
来源：http://vbm.nanxuanxn.top

[U33] Py：打包发布
来源：http://fvb.hysaishi.cn

python -m build  （依赖 pyproject.toml）
来源：http://qun.shuidangran.top

[U34] Py：判断编码
来源：http://zkn.kuanghao11.cn

chardet.detect(raw)
来源：http://nip.tanke756.top

[U35] Py：发送邮件
来源：http://vsc.daria6918.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pnb.ywan-chungtsiang.top

[U36] Py：定时任务
来源：http://cep.haohaochexian.top

schedule.every(10).minutes.do(job)
来源：http://mcb.hnqzz.top

[U37] Py：读写 Excel
来源：http://cfu.cucudq.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ehp.zhengqikj.top

[U38] Py：获取脚本所在目录
来源：http://oui.snrcjt.cn

Path(__file__).resolve().parent
来源：http://whp.nwbrower.top

[U39] Py：判断是否在交互环境
来源：http://hjd.cashguo.top

sys.stdout.isatty()
来源：http://lnr.zhongyouzk.top

[U40] Py：打印到标准错误
来源：http://jls.yonumen.top

print("err", file=sys.stderr)
来源：http://evx.chenzaomai.com

[U41] PHP：初始化 Composer 项目
来源：http://glg.xuetiantiany.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://sqd.jqgfzy.top

[U42] PHP：PSR-4 自动加载
来源：http://vxp.sxryk.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tlr.zhixingplan.top

[U43] PHP：声明命名空间
来源：http://rkl.feifeiyinyue.top

namespace App\Http;
来源：http://hip.zhoulong.xyz

[U44] PHP：开启严格类型
来源：http://hts.xuetiantiany.cn

declare(strict_types=1);
来源：http://ohj.yj202588.top

[U45] PHP：类型声明与返回类型
来源：http://lmb.shangyingyoupin.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://azh.jinqigfzy.top

[U46] PHP：可空类型
来源：http://seo.guannengcc.top

?string $name = null
来源：http://ncg.vqdsnc.cn

[U47] PHP：联合类型
来源：http://tdh.gzhubu.top

int|string $id
来源：http://dfy.svipenyu.cn

[U48] PHP：纯枚举
来源：http://loy.smart0.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kqw.jinqigfzy.top

[U49] PHP：只读属性
来源：http://mgz.andypj.xyz

public readonly string $name
来源：http://yeu.ehwqpu.com

[U50] PHP：构造器属性提升
来源：http://wsd.xylfe.cn

public function __construct(private int $id) {}
来源：http://dpr.kuanghao11.cn

[U51] PHP：数组解构
来源：http://qgz.zhiwuduotai.top

[$a, $b] = $arr;
来源：http://oes.andypj.xyz

[U52] PHP：箭头函数
来源：http://wep.yfazqb.com

$double = fn($x) => $x * 2;
来源：http://mdl.c1oappe.top

[U53] PHP：空合并运算符
来源：http://tuv.0kj1m.cn

$v = $a ?? $b ?? "default";
来源：http://tcg.quarkkingdee.top

[U54] PHP：空安全调用
来源：http://srd.aizwys.cn

$obj?->method()
来源：http://ppk.sweek.top

[U55] PHP：match 表达式
来源：http://qof.aibaodan.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rtq.yonumen.top

[U56] PHP：命名参数
来源：http://gfj.yvedp.cn

f(a: 1, b: 2)
来源：http://wxx.zhaomingkeji.xyz

[U57] PHP：字符串插值
来源：http://wqw.nanxinkj.top

"值: {$a}"
来源：http://enc.chenlongwang.top

[U58] PHP：数组三件套
来源：http://ixc.wangshuangyany.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://klo.shanyushiyangkeji.top

[U59] PHP：自定义排序
来源：http://vyd.meibo888.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pcc.vqdsnc.cn

[U60] PHP：JSON 编解码
来源：http://ohx.andypj.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dmr.yongpay.top

[U61] PHP：正则
来源：http://gnz.vehdjk.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uah.ivvv.top

[U62] PHP：日期对象
来源：http://pdf.zhoulong.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://neh.shanyushiyangkeji.top

[U63] PHP：文件读写
来源：http://xrg.nanxuanxn.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hxl.havefunace.top

[U64] PHP：目录遍历
来源：http://bha.gzhubu.top

glob("dir/*.php");  scandir("dir");
来源：http://sht.cdnleiting.top

[U65] PHP：会话
来源：http://rrk.hongshengwenyu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://esg.xziqi.cn

[U66] PHP：设置 Cookie
来源：http://urv.snrcjt.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://szs.yueranfly.top

[U67] PHP：处理文件上传
来源：http://nxc.hongshengwenyu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uiw.ybcxt.top

[U68] PHP：PDO 连接
来源：http://xkc.smart0.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://waw.gaohongyu789.top

[U69] PHP：PDO 预处理
来源：http://wsy.sufxvd.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://vtp.jinqigfzy.top

[U70] PHP：PDO 事务
来源：http://mtl.yongpay.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rit.9152youxi.cn

[U71] PHP：抛出异常
来源：http://eef.hesvh.cn

throw new RuntimeException("失败", 500);
来源：http://ifn.xylfe.cn

[U72] PHP：写错误日志
来源：http://swo.yonumen.top

error_log("失败: " . $e->getMessage());
来源：http://uqw.yfazqb.com

[U73] PHP：读取 ini 配置
来源：http://ydd.daxiang520.top

parse_ini_file("config.ini", true)
来源：http://kbo.jinyuanbaomall.cn

[U74] PHP：读取环境变量
来源：http://ske.ivvv.top

getenv("APP_ENV") ?: "production"
来源：http://bga.ywan-chungtsiang.top

[U75] PHP：依赖注入
来源：http://cby.yfazqb.com

composer require psr/container
来源：http://zax.yj202588.top

[U76] PHP：简单路由
来源：http://gzh.hcnkem.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://use.ydzc1.top

[U77] PHP：模板渲染
来源：http://xod.yuanzhike.top

composer require twig/twig
来源：http://lxo.havefunace.top

[U78] PHP：单元测试
来源：http://nkj.hfpthk.cn

composer require --dev phpunit/phpunit
来源：http://oxt.zhoulong.xyz

[U79] PHP：静态分析
来源：http://qva.sjlbkw.cn

composer require --dev phpstan/phpstan
来源：http://ccd.birdmap.top

[U80] PHP：代码规范修复
来源：http://mkg.smart0.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://oej.zhiwuduotai.top

[U81] JS：初始化项目
来源：http://qpk.yj20258888.top

npm init -y;  npm i express
来源：http://ceg.shanyushiyangtech.top

[U82] JS：package.json 脚本
来源：http://pgw.yj202588.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://whr.guannengcc.top

[U83] JS：ES Module 导入导出
来源：http://tvx.mhx1999.top

export const a = 1;  import { a } from "./m.js";
来源：http://ydp.epnwcf.com

[U84] JS：CommonJS 写法
来源：http://aqy.guowangkeji.top

module.exports = { a };  const { a } = require("./m");
来源：http://uti.kuanghao11.cn

[U85] JS：可选链
来源：http://nsq.jinqigufen.top

a?.b?.c
来源：http://xfg.jinghuilouyu.cn

[U86] JS：空值合并
来源：http://krd.mhx1999.top

a ?? b
来源：http://irt.nanxinkj.top

[U87] JS：解构默认值
来源：http://zzw.smart0.xyz

const { a = 1, b = 2 } = obj;
来源：http://vpy.jinqigfzy.top

[U88] JS：对象展开合并
来源：http://qai.aibaodan.cn

{ ...a, ...b }
来源：http://uho.zhixingplan.top

[U89] JS：数组去重
来源：http://sst.ppjwa.cn

[...new Set(arr)]
来源：http://gqs.smart0.xyz

[U90] JS：数字数组排序
来源：http://zag.fehbvm.com

[...arr].sort((a, b) => a - b)
来源：http://ylt.xylfe.cn

[U91] JS：对象键值遍历
来源：http://wch.fanxiaobao.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wyv.snrcjt.cn

[U92] JS：深拷贝
来源：http://xmk.shanyushiyangkeji.top

structuredClone(obj)
来源：http://njy.andypj.xyz

[U93] JS：模板字符串
来源：http://emd.smart0.xyz

`共 ${n} 条`
来源：http://myb.9152youxi.cn

[U94] JS：箭头函数
来源：http://bho.aibaodan.cn

const double = x => x * 2;
来源：http://bdl.svipenyu.cn

[U95] JS：Promise 包装
来源：http://uuf.yj20258888.top

new Promise((resolve, reject) => {})
来源：http://hdq.jinyuanbaomall.cn

[U96] JS：async/await 与异常
来源：http://zot.chenlongwang.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yvr.bjfxy.top

[U97] JS：并发请求
来源：http://ytv.guowangkeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://tux.yvedp.cn

[U98] JS：fetch 带 JSON
来源：http://tvz.fktsv.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://twb.52xcode.cn

[U99] JS：事件监听
来源：http://izr.meibo888.top

el.addEventListener("click", e => {})
来源：http://gpr.aizwys.cn

[U100] JS：DOM 查询
来源：http://pul.iojbl.cn

document.querySelector(".item")
来源：http://ldc.yanxiufei.cn

[U101] JS：classList 操作
来源：http://gif.sjlbkw.cn

el.classList.toggle("active")
来源：http://ujc.vqdsnc.cn

[U102] JS：本地存储
来源：http://gke.sjlbkw.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jlh.yfazqb.com

[U103] JS：定时器
来源：http://ian.zycfv.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pna.ehwqpu.com

[U104] JS：防抖
来源：http://wzk.haohaochexian.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mra.chenjidiqi.icu

[U105] JS：节流
来源：http://bkw.kuanghao11.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fhy.cashguo.top

[U106] JS：日期格式化
来源：http://mts.sxryk.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bqz.ivvv.top

[U107] JS：数字千分位
来源：http://sgc.yj202588.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kzq.shanyushiyangkeji.top

[U108] JS：随机整数
来源：http://mwp.aizwys.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mfc.tianlin.xyz

[U109] JS：数组分组
来源：http://lwt.havefunace.top

Object.groupBy(arr, x => x.type)
来源：http://ufp.hywenlv.cn

[U110] JS：数组分块
来源：http://cau.redwolf501.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tzt.52xcode.cn

[U111] JS：对象转 Map
来源：http://mzo.ydzc1.top

new Map(Object.entries(obj))
来源：http://ixn.jianghu66.top

[U112] JS：字符串补位
来源：http://lpf.xingfuxueyuan.xyz

"7".padStart(3, "0")
来源：http://tbk.sjlbkw.cn

[U113] JS：正则替换全部
来源：http://rsw.daxiang520.top

s.replaceAll("a", "b")
来源：http://uvt.daria6918.cn

[U114] JS：JSON 深比较
来源：http://kuv.kuanghao11.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cfe.chenzaomai.com

[U115] JS：生成 UUID
来源：http://xtg.gogol.net.cn

crypto.randomUUID()
来源：http://blo.hywenlv.cn

[U116] JS：类型检查（JSDoc）
来源：http://ciz.ivvv.top

/** @param {string} name */ function f(name) {}
来源：http://mdh.jlsjyb.cn

[U117] JS：单元测试
来源：http://jtx.cdnleiting.top

npm i -D vitest;  npx vitest
来源：http://kzc.hammf.cn

[U118] JS：开发服务器
来源：http://omo.jyoumei.cn

npm i -D vite;  npx vite
来源：http://yjc.cdnleiting.top

[U119] JS：生产构建
来源：http://zzd.feifeiyinyue.top

npx vite build
来源：http://esn.xingfuxueyuan.xyz

[U120] JS：读取环境变量（Vite）
来源：http://wib.tanke756.top

import.meta.env.VITE_API_URL
来源：http://vjv.guannengcc.top

================================================================================
来源：http://fxu.zhoulong.xyz

统计汇总
来源：http://xzh.yonumen.top

================================================================================
来源：http://mog.jqgfzy.top

按语言统计（条）：
来源：http://sdv.gaohongyu789.top

Python ......... 252
来源：http://fwp.vqdsnc.cn

PHP ............ 252
来源：http://znm.snrcjt.cn

JavaScript ..... 252
来源：http://ivr.vehdjk.com

TypeScript ..... 212
来源：http://vkc.jianghu66.top

Java ........... 212
来源：http://mzp.nanxinkj.top

Go ............. 212
来源：http://jgy.fanxiaobao.xyz

Ruby ........... 212
来源：http://tzx.yangfankeji.com

C# ............. 212
来源：http://ilt.ehwqpu.com

C .............. 30
来源：http://gfe.snrcjt.cn

C++ ............ 30
来源：http://hod.jinghuilouyu.cn

SQL ............ 90
来源：http://rom.nanxinkj.top

Bash ........... 80
来源：http://rij.daxiang520.top

Kotlin ......... 15
来源：http://bms.daxiang520.top

Swift .......... 15
来源：http://qpr.xuanzx.com

Lua ............ 10
来源：http://emq.cucudq.cn

Perl ........... 10
来源：http://arq.yuanzhike.top

Scala .......... 10
来源：http://arp.zhiwuduotai.top

------------------------------------
来源：http://sae.haohaochexian.top

合计 ........... 2106 条
来源：http://zch.uphjek.com

按章节统计：
来源：http://wci.sxryk.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vrs.hysaishi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pti.jqgufenzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pxx.guowangkeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lqt.cucudq.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://apx.sweek.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kon.meibo888.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cdx.xuetiantiany.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gmz.shanyushiyangtech.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qjp.9152youxi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hpw.feifeiyinyue.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://exi.fengsongda.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pur.snrcjt.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mna.daria6918.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ero.hnqzz.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wlt.316326.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fkh.ydzc1.top

Q SQL 专题                              90
来源：http://cfe.jlsjyb.cn

R Bash 专题                             80
来源：http://vkx.ctjpmb.com

S C / C++ 专题                          60
来源：http://jxo.ctjpmb.com

T 其他语言补充                          60
来源：http://bvz.chenzaomai.com

U 高频实用片段                         120
来源：http://enw.c1oappe.top

------------------------------------
来源：http://pkr.snrcjt.cn

合计                                  2106 条
来源：http://rxf.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://nbq.guannengcc.top

使用提醒
来源：http://bhu.daria6918.cn

--------------------------------------------------------------------------------
来源：http://kkw.jqgfzy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://siw.xziqi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://unc.feifeiyinyue.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yys.zhixingplan.top

在旧版本上使用前请先确认语法支持情况。
来源：http://anl.nanxuanxn.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jvx.yuanzhike.top

—— 文件结束 ——
来源：http://gze.hnqzz.top

================================================================================
来源：http://aaa.uphjek.com

程序语言常见例子速查手册（2024 版）
来源：http://dof.ydzc1.top

Common Programming Examples Cheat Book
来源：http://mqy.zhongyouzk.top

================================================================================
来源：http://nmy.yuxming.cn

【收录内容】
来源：http://zpx.shangyingyoupin.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://egr.kuanghao11.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hbj.xziqi.cn

SQL · Bash · C · C++
来源：http://kvi.gaohongyu789.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://tbw.pycfn.com

【使用说明】
来源：http://jjd.gotoacloud.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rly.bbcook.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qom.jianghu66.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lyi.jqgufenzy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jbc.yj20258.top

Bash:  Shell         C:     C             C++:   C++
来源：http://blc.ydjk.org.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://den.iojbl.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tsg.nanxinkj.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rhr.jinqigufen.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ydd.dashuyun.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://owz.nanxinkj.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qqv.aizwys.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qfr.xinyue.icu

【文件统计】
来源：http://oyz.fehbvm.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ohy.hnqzz.top

--------------------------------------------------------------------------------
来源：http://quj.ywan-chungtsiang.top

目  录
来源：http://lsb.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://rpj.nwbrower.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ryc.xuanzx.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://azz.jianghu66.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jhn.iojbl.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dgd.zhijiandao.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dcg.smart0.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gdd.yj20258.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yyk.bbcook.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sqk.dianchejie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hsk.xuanzx.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://aeo.chenlongwang.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zmi.quarkkingdee.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xvf.zhijiandao.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://eps.yuanzhike.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bdb.tianlin.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lnm.vqdsnc.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pcy.hnqzz.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zaa.jqgfzy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://uvs.ydjk.org.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lwd.pycfn.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xga.hesvh.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ozx.jinghuilouyu.cn

================================================================================
来源：http://zpp.zhiwuduotai.top

A. 基础语法与类型
来源：http://ftc.nwbrower.top

================================================================================
来源：http://tlc.yj20258.top

[A01] Hello World
来源：http://jaq.tian-w.cn

Py:   print("Hello, World!")
来源：http://wni.jiagoushi.top

PHP:  echo "Hello, World!";
来源：http://nha.yangfankeji.com

JS:   console.log("Hello, World!");
来源：http://nxl.cqqwz.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pdo.ydzc1.top

Java: System.out.println("Hello, World!");
来源：http://ntn.zhaomingkeji.xyz

Go:   fmt.Println("Hello, World!")
来源：http://cjc.0kj1m.cn

Ruby: puts "Hello, World!"
来源：http://xfe.ehwqpu.com

C#:   Console.WriteLine("Hello, World!");
来源：http://sog.havefunace.top

[A02] 变量声明与赋值
来源：http://jyg.316326.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://sac.yj202588.top

PHP:  $name = "Alex"; $age = 20;
来源：http://igp.ppjwa.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xea.pycfn.com


<!-- 参考信息 -->