代发 wailian999

[U31] Py：单测
来源：http://nio.yueranfly.top

python -m pytest -q
来源：http://zxj.andypj.xyz

[U32] Py：代码格式化
来源：http://iaw.epnwcf.com

ruff format . && ruff check --fix .
来源：http://dsa.yj20258.top

[U33] Py：打包发布
来源：http://pbu.dianchejie.cn

python -m build  （依赖 pyproject.toml）
来源：http://qgu.jinyuanbaomall.cn

[U34] Py：判断编码
来源：http://qfd.zhaomingkeji.xyz

chardet.detect(raw)
来源：http://war.aibaodan.cn

[U35] Py：发送邮件
来源：http://whj.ywan-chungtsiang.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gtq.shanyushiyangkeji.top

[U36] Py：定时任务
来源：http://gvs.svipenyu.cn

schedule.every(10).minutes.do(job)
来源：http://sny.yuxming.cn

[U37] Py：读写 Excel
来源：http://sra.vehdjk.com

pandas.read_excel / DataFrame.to_excel
来源：http://lnp.dianchejie.cn

[U38] Py：获取脚本所在目录
来源：http://qmn.zhoulong.xyz

Path(__file__).resolve().parent
来源：http://din.ybcxt.top

[U39] Py：判断是否在交互环境
来源：http://eox.sufxvd.cn

sys.stdout.isatty()
来源：http://ddx.hysaishi.cn

[U40] Py：打印到标准错误
来源：http://ska.shzxlz.cn

print("err", file=sys.stderr)
来源：http://man.bjfxy.top

[U41] PHP：初始化 Composer 项目
来源：http://uii.birdmap.top

composer init;  composer require guzzlehttp/guzzle
来源：http://una.tanke756.top

[U42] PHP：PSR-4 自动加载
来源：http://wgq.nanxuanxn.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cog.shuidangran.top

[U43] PHP：声明命名空间
来源：http://zea.cashguo.top

namespace App\Http;
来源：http://pie.uphjek.com

[U44] PHP：开启严格类型
来源：http://ltt.jinghuilouyu.cn

declare(strict_types=1);
来源：http://wcg.sysykeji.top

[U45] PHP：类型声明与返回类型
来源：http://hcf.wangdashe.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ifn.xinyue.icu

[U46] PHP：可空类型
来源：http://cwa.yongpay.top

?string $name = null
来源：http://cpn.tanke756.top

[U47] PHP：联合类型
来源：http://num.guannengcc.top

int|string $id
来源：http://xiq.ybcxt.top

[U48] PHP：纯枚举
来源：http://zky.zdqjudy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wht.redwolf501.top

[U49] PHP：只读属性
来源：http://xui.yj202588.top

public readonly string $name
来源：http://fkm.nwbrower.top

[U50] PHP：构造器属性提升
来源：http://sba.shanyushiyangkeji.top

public function __construct(private int $id) {}
来源：http://ikd.havefunace.top

[U51] PHP：数组解构
来源：http://hyu.jlsjyb.cn

[$a, $b] = $arr;
来源：http://zmb.vehdjk.com

[U52] PHP：箭头函数
来源：http://uvq.hcnkem.com

$double = fn($x) => $x * 2;
来源：http://vfg.vehdjk.com

[U53] PHP：空合并运算符
来源：http://cgn.ydzc1.top

$v = $a ?? $b ?? "default";
来源：http://ulw.meibo888.top

[U54] PHP：空安全调用
来源：http://hzj.yongpay.top

$obj?->method()
来源：http://vlh.hysaishi.cn

[U55] PHP：match 表达式
来源：http://wyj.birdmap.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qwz.tanke756.top

[U56] PHP：命名参数
来源：http://shl.hysaishi.cn

f(a: 1, b: 2)
来源：http://opx.hongshengwenyu.top

[U57] PHP：字符串插值
来源：http://ahs.zhixingplan.top

"值: {$a}"
来源：http://kcn.shanyushiyangtech.top

[U58] PHP：数组三件套
来源：http://mjs.chenzaomai.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://oad.jiagoushi.top

[U59] PHP：自定义排序
来源：http://lwq.ctjpmb.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ikg.cucudq.cn

[U60] PHP：JSON 编解码
来源：http://dlz.zhengqikj.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xgx.quarkkingdee.top

[U61] PHP：正则
来源：http://ozn.xuetiantiany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kle.yj20258.top

[U62] PHP：日期对象
来源：http://ebv.fktsv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cay.chenzaomai.com

[U63] PHP：文件读写
来源：http://gjd.yanxiufei.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hly.pengpengdd.cyou

[U64] PHP：目录遍历
来源：http://zlp.nwbrower.top

glob("dir/*.php");  scandir("dir");
来源：http://qbk.52xcode.cn

[U65] PHP：会话
来源：http://epc.fehbvm.com

session_start();  $_SESSION["uid"] = 1;
来源：http://xfk.birdmap.top

[U66] PHP：设置 Cookie
来源：http://ymz.yj20258888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vnl.jyoumei.cn

[U67] PHP：处理文件上传
来源：http://guy.epnwcf.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qyh.hesvh.cn

[U68] PHP：PDO 连接
来源：http://wzy.daxiang520.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://okz.chenjidiqi.icu

[U69] PHP：PDO 预处理
来源：http://yuy.c1oappe.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rnu.tarul.cn

[U70] PHP：PDO 事务
来源：http://zdz.zhongyouzk.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hij.xziqi.cn

[U71] PHP：抛出异常
来源：http://fen.hywenlv.cn

throw new RuntimeException("失败", 500);
来源：http://kky.xylfe.cn

[U72] PHP：写错误日志
来源：http://sko.wangdashe.top

error_log("失败: " . $e->getMessage());
来源：http://kto.jianghu66.top

[U73] PHP：读取 ini 配置
来源：http://wwt.feifeiyinyue.top

parse_ini_file("config.ini", true)
来源：http://eka.dashuyun.cn

[U74] PHP：读取环境变量
来源：http://xwo.dashuyun.cn

getenv("APP_ENV") ?: "production"
来源：http://nes.zhijiandao.cn

[U75] PHP：依赖注入
来源：http://yck.pengpengdd.cyou

composer require psr/container
来源：http://xdj.gotoacloud.top

[U76] PHP：简单路由
来源：http://dbi.zdbjq.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pmy.xuanzx.com

[U77] PHP：模板渲染
来源：http://ver.vqdsnc.cn

composer require twig/twig
来源：http://bcn.fehbvm.com

[U78] PHP：单元测试
来源：http://enc.gotoacloud.top

composer require --dev phpunit/phpunit
来源：http://ayf.hesvh.cn

[U79] PHP：静态分析
来源：http://kjo.daxiang520.top

composer require --dev phpstan/phpstan
来源：http://hhg.andypj.xyz

[U80] PHP：代码规范修复
来源：http://tfh.9152youxi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vjq.hnqzz.top

[U81] JS：初始化项目
来源：http://dle.ywan-chungtsiang.top

npm init -y;  npm i express
来源：http://rij.zycfv.cn

[U82] JS：package.json 脚本
来源：http://zem.hesvh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bff.316326.xyz

[U83] JS：ES Module 导入导出
来源：http://aop.ivvv.top

export const a = 1;  import { a } from "./m.js";
来源：http://uny.nwbrower.top

[U84] JS：CommonJS 写法
来源：http://nfm.snrcjt.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rqn.hcnkem.com

[U85] JS：可选链
来源：http://zpr.fengsongda.top

a?.b?.c
来源：http://qti.316326.xyz

[U86] JS：空值合并
来源：http://nqj.iojbl.cn

a ?? b
来源：http://mpb.pycfn.com

[U87] JS：解构默认值
来源：http://qtf.smart0.xyz

const { a = 1, b = 2 } = obj;
来源：http://yck.sjlbkw.cn

[U88] JS：对象展开合并
来源：http://dbc.ehwqpu.com

{ ...a, ...b }
来源：http://gpq.zhixingplan.top

[U89] JS：数组去重
来源：http://nbd.pengpengdd.cyou

[...new Set(arr)]
来源：http://ggs.zdqjudy.top

[U90] JS：数字数组排序
来源：http://rzd.tarul.cn

[...arr].sort((a, b) => a - b)
来源：http://yiz.hammf.cn

[U91] JS：对象键值遍历
来源：http://jzd.chenjidiqi.icu

Object.entries(obj).forEach(([k, v]) => {});
来源：http://krj.feifeiyinyue.top

[U92] JS：深拷贝
来源：http://toc.haohaochexian.top

structuredClone(obj)
来源：http://hbd.ywan-chungtsiang.top

[U93] JS：模板字符串
来源：http://xwd.iojbl.cn

`共 ${n} 条`
来源：http://cih.mhx1999.top

[U94] JS：箭头函数
来源：http://bil.yonumen.top

const double = x => x * 2;
来源：http://grt.jinqigfzy.top

[U95] JS：Promise 包装
来源：http://xqj.fehbvm.com

new Promise((resolve, reject) => {})
来源：http://gcq.chenlongwang.top

[U96] JS：async/await 与异常
来源：http://wsg.sufxvd.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qrw.andypj.xyz

[U97] JS：并发请求
来源：http://iuh.xingfuxueyuan.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://ayd.jinghuilouyu.cn

[U98] JS：fetch 带 JSON
来源：http://gyh.0kj1m.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://eez.jinghuilouyu.cn

[U99] JS：事件监听
来源：http://scl.gzhubu.top

el.addEventListener("click", e => {})
来源：http://cru.cashguo.top

[U100] JS：DOM 查询
来源：http://zpu.daxiang520.top

document.querySelector(".item")
来源：http://syz.hnqzz.top

[U101] JS：classList 操作
来源：http://ygd.guannengcc.top

el.classList.toggle("active")
来源：http://hem.vqdsnc.cn

[U102] JS：本地存储
来源：http://ick.zhaomingkeji.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://pyz.shanyushiyangkeji.top

[U103] JS：定时器
来源：http://ynq.haohaochexian.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ogy.yuanzhike.top

[U104] JS：防抖
来源：http://oiy.wangdashe.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kcc.hesvh.cn

[U105] JS：节流
来源：http://hic.xinyue.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ykc.shanyushiyangkeji.top

[U106] JS：日期格式化
来源：http://ovo.xuetiantiany.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rpt.yangfankeji.com

[U107] JS：数字千分位
来源：http://gcq.hnxiangtu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uom.tanke756.top

[U108] JS：随机整数
来源：http://rnk.yueranfly.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://iiq.redwolf501.top

[U109] JS：数组分组
来源：http://pev.sxryk.cn

Object.groupBy(arr, x => x.type)
来源：http://syv.feifeiyinyue.top

[U110] JS：数组分块
来源：http://ica.jiagoushi.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bfd.hywenlv.cn

[U111] JS：对象转 Map
来源：http://cbm.pengpengdd.cyou

new Map(Object.entries(obj))
来源：http://fzl.zhongyouzk.top

[U112] JS：字符串补位
来源：http://zse.fzhhl.top

"7".padStart(3, "0")
来源：http://pfb.jiagoushi.top

[U113] JS：正则替换全部
来源：http://jfj.wangshuangyany.cn

s.replaceAll("a", "b")
来源：http://jic.ybcxt.top

[U114] JS：JSON 深比较
来源：http://rzp.hongshengwenyu.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://jqc.aibaodan.cn

[U115] JS：生成 UUID
来源：http://uav.ywan-chungtsiang.top

crypto.randomUUID()
来源：http://rfy.ivvv.top

[U116] JS：类型检查（JSDoc）
来源：http://jve.9152youxi.cn

/** @param {string} name */ function f(name) {}
来源：http://oxl.shuidangran.top

[U117] JS：单元测试
来源：http://wkz.wangdashe.top

npm i -D vitest;  npx vitest
来源：http://hzv.jinqigufen.top

[U118] JS：开发服务器
来源：http://yde.nanxinkj.top

npm i -D vite;  npx vite
来源：http://fnj.yueranfly.top

[U119] JS：生产构建
来源：http://piy.shzxlz.cn

npx vite build
来源：http://phe.316326.xyz

[U120] JS：读取环境变量（Vite）
来源：http://uxb.fehbvm.com

import.meta.env.VITE_API_URL
来源：http://lsv.tian-w.cn

================================================================================
来源：http://gmh.gzhubu.top

统计汇总
来源：http://gks.ehwqpu.com

================================================================================
来源：http://lpp.zhengqikj.top

按语言统计（条）：
来源：http://tkz.dianchejie.cn

Python ......... 252
来源：http://nro.yongpay.top

PHP ............ 252
来源：http://kds.iojbl.cn

JavaScript ..... 252
来源：http://wyv.ydjk.org.cn

TypeScript ..... 212
来源：http://bzi.jinqigufen.top

Java ........... 212
来源：http://kvi.gotoacloud.top

Go ............. 212
来源：http://krm.shangyingyoupin.top

Ruby ........... 212
来源：http://chx.uphjek.com

C# ............. 212
来源：http://yjt.redwolf501.top

C .............. 30
来源：http://hje.jqgfzy.top

C++ ............ 30
来源：http://xsj.daria6918.cn

SQL ............ 90
来源：http://pfh.sysykeji.top

Bash ........... 80
来源：http://wzo.ctjpmb.com

Kotlin ......... 15
来源：http://zpe.hywenlv.cn

Swift .......... 15
来源：http://meb.jqgufenzy.top

Lua ............ 10
来源：http://tcc.fanxiaobao.xyz

Perl ........... 10
来源：http://gor.wangshuangyany.cn

Scala .......... 10
来源：http://fti.gzhubu.top

------------------------------------
来源：http://jsd.zhijiandao.cn

合计 ........... 2106 条
来源：http://luy.sweek.top

按章节统计：
来源：http://jnj.yfazqb.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ryv.jyoumei.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xnw.shangyingyoupin.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://juw.jinqigufen.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://npk.jyoumei.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uik.vqdsnc.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fsa.fktsv.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cjg.iojbl.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hao.zhoulong.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wfe.chenlongwang.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nxe.jinyuanbaomall.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sbj.zhoulong.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uhe.vqdsnc.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qxj.smart0.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nvc.zhoulong.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://adh.aibaodan.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://umy.bjfxy.top

Q SQL 专题                              90
来源：http://yxn.xziqi.cn

R Bash 专题                             80
来源：http://ufm.daxiang520.top

S C / C++ 专题                          60
来源：http://rue.gogol.net.cn

T 其他语言补充                          60
来源：http://err.ywan-chungtsiang.top

U 高频实用片段                         120
来源：http://hju.ywan-chungtsiang.top

------------------------------------
来源：http://acn.hcnkem.com

合计                                  2106 条
来源：http://aou.iojbl.cn

--------------------------------------------------------------------------------
来源：http://geu.316326.xyz

使用提醒
来源：http://brd.tian-w.cn

--------------------------------------------------------------------------------
来源：http://ypv.haohaochexian.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nvk.yvedp.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xvm.cqqwz.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pdq.yuanzhike.top

在旧版本上使用前请先确认语法支持情况。
来源：http://hxx.xingfuxueyuan.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mej.quarkkingdee.top

—— 文件结束 ——
来源：http://viv.sweek.top

================================================================================
来源：http://ruq.dashuyun.cn

程序语言常见例子速查手册（2024 版）
来源：http://qcj.cdnleiting.top

Common Programming Examples Cheat Book
来源：http://sdf.redwolf501.top

================================================================================
来源：http://wdm.sufxvd.cn

【收录内容】
来源：http://wyt.hysaishi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ldo.shanyushiyangtech.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://oej.yj20258.top

SQL · Bash · C · C++
来源：http://ezx.52xcode.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://efs.zhoulong.xyz

【使用说明】
来源：http://oqs.ivvv.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tlr.feifeiyinyue.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xmh.sjlbkw.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://osd.zhaomingkeji.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ddg.0kj1m.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ntt.aibaodan.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kun.quarkkingdee.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ten.vehdjk.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tdg.bbcook.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lct.yonumen.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gxn.fzhhl.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tht.ivvv.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fcq.yongpay.top

【文件统计】
来源：http://gaf.xziqi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://egi.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://hcu.guowangkeji.top

目  录
来源：http://rel.meibo888.top

--------------------------------------------------------------------------------
来源：http://enk.316326.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bpc.redwolf501.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gzg.bjfxy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tbn.jinghuilouyu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ute.ybcxt.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kti.quarkkingdee.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wkp.vqdsnc.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://pef.9152youxi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://drr.hcnkem.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://emx.cucudq.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://grc.yj20258.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uxv.xziqi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://odj.nanxuanxn.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xxx.xziqi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cyc.nanxinkj.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gyb.pengpengdd.cyou

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://okh.zhongyouzk.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yya.jyoumei.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://qrm.9152youxi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vdu.yuanzhike.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ydl.jinqigufen.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qck.cdnleiting.top

================================================================================
来源：http://bvt.sxryk.cn

A. 基础语法与类型
来源：http://zbb.yonumen.top

================================================================================
来源：http://syo.zhixingplan.top

[A01] Hello World
来源：http://wyg.uphjek.com

Py:   print("Hello, World!")
来源：http://ibt.cdnleiting.top

PHP:  echo "Hello, World!";
来源：http://oqo.jiagoushi.top

JS:   console.log("Hello, World!");
来源：http://cyk.yonumen.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xgu.feifeiyinyue.top

Java: System.out.println("Hello, World!");
来源：http://yfs.ybcxt.top

Go:   fmt.Println("Hello, World!")
来源：http://lrh.sxryk.cn

Ruby: puts "Hello, World!"
来源：http://pzy.gotoacloud.top

C#:   Console.WriteLine("Hello, World!");
来源：http://egj.chenlongwang.top

[A02] 变量声明与赋值
来源：http://axd.ivvv.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uee.yfazqb.com

PHP:  $name = "Alex"; $age = 20;
来源：http://jps.meibo888.top

JS:   let name = "Alex"; const age = 20;
来源：http://tlz.shanyushiyangtech.top


<!-- 参考信息 -->