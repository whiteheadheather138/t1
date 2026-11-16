代发 wailian999

[U31] Py：单测
来源：http://adb.dashuyun.cn

python -m pytest -q
来源：http://fon.zhijiandao.cn

[U32] Py：代码格式化
来源：http://wgp.aizwys.cn

ruff format . && ruff check --fix .
来源：http://tbr.guannengcc.top

[U33] Py：打包发布
来源：http://iwr.cashguo.top

python -m build  （依赖 pyproject.toml）
来源：http://cuq.ctjpmb.com

[U34] Py：判断编码
来源：http://def.uphjek.com

chardet.detect(raw)
来源：http://czy.jinqigufen.top

[U35] Py：发送邮件
来源：http://oas.fzhhl.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blu.sjlbkw.cn

[U36] Py：定时任务
来源：http://itq.jinqigfzy.top

schedule.every(10).minutes.do(job)
来源：http://wpa.gogol.net.cn

[U37] Py：读写 Excel
来源：http://xec.wangdashe.top

pandas.read_excel / DataFrame.to_excel
来源：http://rmp.tarul.cn

[U38] Py：获取脚本所在目录
来源：http://bjo.zhijiandao.cn

Path(__file__).resolve().parent
来源：http://nbf.nwbrower.top

[U39] Py：判断是否在交互环境
来源：http://tbv.yfazqb.com

sys.stdout.isatty()
来源：http://eyb.sysykeji.top

[U40] Py：打印到标准错误
来源：http://agr.cucudq.cn

print("err", file=sys.stderr)
来源：http://wne.xingfuxueyuan.xyz

[U41] PHP：初始化 Composer 项目
来源：http://upb.jianghu66.top

composer init;  composer require guzzlehttp/guzzle
来源：http://qea.hammf.cn

[U42] PHP：PSR-4 自动加载
来源：http://eju.sysykeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rak.ybcxt.top

[U43] PHP：声明命名空间
来源：http://hdn.0kj1m.cn

namespace App\Http;
来源：http://ucf.pycfn.com

[U44] PHP：开启严格类型
来源：http://gue.tarul.cn

declare(strict_types=1);
来源：http://uvl.jinyuanbaomall.cn

[U45] PHP：类型声明与返回类型
来源：http://nor.xuetiantiany.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ran.yongpay.top

[U46] PHP：可空类型
来源：http://rcl.fzhhl.top

?string $name = null
来源：http://pet.yuxming.cn

[U47] PHP：联合类型
来源：http://bss.aibaodan.cn

int|string $id
来源：http://acu.316326.xyz

[U48] PHP：纯枚举
来源：http://tcc.jianghu66.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mmi.hammf.cn

[U49] PHP：只读属性
来源：http://hcq.yuanzhike.top

public readonly string $name
来源：http://fbq.xuetiantiany.cn

[U50] PHP：构造器属性提升
来源：http://quc.zdqjudy.top

public function __construct(private int $id) {}
来源：http://zwf.chenlongwang.top

[U51] PHP：数组解构
来源：http://udr.dashuyun.cn

[$a, $b] = $arr;
来源：http://wlx.kuanghao11.cn

[U52] PHP：箭头函数
来源：http://pff.zhengqikj.top

$double = fn($x) => $x * 2;
来源：http://dlq.zhijiandao.cn

[U53] PHP：空合并运算符
来源：http://ifi.yongpay.top

$v = $a ?? $b ?? "default";
来源：http://fdk.kuanghao11.cn

[U54] PHP：空安全调用
来源：http://fwa.tanke756.top

$obj?->method()
来源：http://zoe.cdnleiting.top

[U55] PHP：match 表达式
来源：http://fkv.fehbvm.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ihx.xuetiantiany.cn

[U56] PHP：命名参数
来源：http://leu.haohaochexian.top

f(a: 1, b: 2)
来源：http://qqp.cucudq.cn

[U57] PHP：字符串插值
来源：http://cwd.yj20258.top

"值: {$a}"
来源：http://ese.chenjidiqi.icu

[U58] PHP：数组三件套
来源：http://efj.yongpay.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ccy.uphjek.com

[U59] PHP：自定义排序
来源：http://jom.birdmap.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hmo.smart0.xyz

[U60] PHP：JSON 编解码
来源：http://zru.ivvv.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://enl.iojbl.cn

[U61] PHP：正则
来源：http://fpo.yj202588.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rnr.epnwcf.com

[U62] PHP：日期对象
来源：http://tfy.shanyushiyangtech.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://egr.yj20258888.top

[U63] PHP：文件读写
来源：http://tjg.guannengcc.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://eag.quarkkingdee.top

[U64] PHP：目录遍历
来源：http://vjv.zhaomingkeji.xyz

glob("dir/*.php");  scandir("dir");
来源：http://zmp.yonumen.top

[U65] PHP：会话
来源：http://ivu.jinqigufen.top

session_start();  $_SESSION["uid"] = 1;
来源：http://aog.feifeiyinyue.top

[U66] PHP：设置 Cookie
来源：http://urt.zhengqikj.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hgp.fengsongda.top

[U67] PHP：处理文件上传
来源：http://vbv.zhiwuduotai.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xho.pycfn.com

[U68] PHP：PDO 连接
来源：http://psq.ydjk.org.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hcn.cqqwz.cn

[U69] PHP：PDO 预处理
来源：http://qhg.ctjpmb.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rog.daria6918.cn

[U70] PHP：PDO 事务
来源：http://nds.gaohongyu789.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sgz.vqdsnc.cn

[U71] PHP：抛出异常
来源：http://xbw.meibo888.top

throw new RuntimeException("失败", 500);
来源：http://ust.wangdashe.top

[U72] PHP：写错误日志
来源：http://vls.ydzc1.top

error_log("失败: " . $e->getMessage());
来源：http://gzx.fehbvm.com

[U73] PHP：读取 ini 配置
来源：http://kck.yonumen.top

parse_ini_file("config.ini", true)
来源：http://wak.jianghu66.top

[U74] PHP：读取环境变量
来源：http://vet.wangshuangyany.cn

getenv("APP_ENV") ?: "production"
来源：http://crh.ehwqpu.com

[U75] PHP：依赖注入
来源：http://hco.cheryme.top

composer require psr/container
来源：http://hzw.cqqwz.cn

[U76] PHP：简单路由
来源：http://whe.cdnleiting.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xdh.birdmap.top

[U77] PHP：模板渲染
来源：http://joi.svipenyu.cn

composer require twig/twig
来源：http://sie.svipenyu.cn

[U78] PHP：单元测试
来源：http://rde.shangyingyoupin.top

composer require --dev phpunit/phpunit
来源：http://yvc.gzhubu.top

[U79] PHP：静态分析
来源：http://qwz.yj20258888.top

composer require --dev phpstan/phpstan
来源：http://vxw.ywan-chungtsiang.top

[U80] PHP：代码规范修复
来源：http://yqq.daria6918.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zyd.fanxiaobao.xyz

[U81] JS：初始化项目
来源：http://vxp.zycfv.cn

npm init -y;  npm i express
来源：http://rig.chenjidiqi.icu

[U82] JS：package.json 脚本
来源：http://epj.epnwcf.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lrn.shanyushiyangkeji.top

[U83] JS：ES Module 导入导出
来源：http://yol.tian-w.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ljq.ivvv.top

[U84] JS：CommonJS 写法
来源：http://dft.ehwqpu.com

module.exports = { a };  const { a } = require("./m");
来源：http://jpx.guannengcc.top

[U85] JS：可选链
来源：http://xxg.yj20258.top

a?.b?.c
来源：http://nqu.tianlin.xyz

[U86] JS：空值合并
来源：http://hxv.guannengcc.top

a ?? b
来源：http://aep.svipenyu.cn

[U87] JS：解构默认值
来源：http://xnb.jinghuilouyu.cn

const { a = 1, b = 2 } = obj;
来源：http://hgh.cqqwz.cn

[U88] JS：对象展开合并
来源：http://euu.nwbrower.top

{ ...a, ...b }
来源：http://ick.jinqigfzy.top

[U89] JS：数组去重
来源：http://mzq.hongshengwenyu.top

[...new Set(arr)]
来源：http://jza.dashuyun.cn

[U90] JS：数字数组排序
来源：http://ddj.svipenyu.cn

[...arr].sort((a, b) => a - b)
来源：http://mfs.gotoacloud.top

[U91] JS：对象键值遍历
来源：http://mrp.jqgufenzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jru.chenzaomai.com

[U92] JS：深拷贝
来源：http://zdc.zhiwuduotai.top

structuredClone(obj)
来源：http://zvu.hnqzz.top

[U93] JS：模板字符串
来源：http://tfd.meibo888.top

`共 ${n} 条`
来源：http://jhz.quarkkingdee.top

[U94] JS：箭头函数
来源：http://yla.jianghu66.top

const double = x => x * 2;
来源：http://pll.epnwcf.com

[U95] JS：Promise 包装
来源：http://sjv.yongpay.top

new Promise((resolve, reject) => {})
来源：http://vqi.gaohongyu789.top

[U96] JS：async/await 与异常
来源：http://yty.tarul.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qgh.chenlongwang.top

[U97] JS：并发请求
来源：http://rov.9152youxi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lck.zhijiandao.cn

[U98] JS：fetch 带 JSON
来源：http://wpt.shanyushiyangtech.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ztn.zhoulong.xyz

[U99] JS：事件监听
来源：http://vjc.aibaodan.cn

el.addEventListener("click", e => {})
来源：http://zck.sysykeji.top

[U100] JS：DOM 查询
来源：http://nkf.316326.xyz

document.querySelector(".item")
来源：http://uil.xinyue.icu

[U101] JS：classList 操作
来源：http://muc.hongshengwenyu.top

el.classList.toggle("active")
来源：http://yob.dianchejie.cn

[U102] JS：本地存储
来源：http://jyi.shanyushiyangkeji.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://oug.andypj.xyz

[U103] JS：定时器
来源：http://wxh.yvedp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dsb.zhijiandao.cn

[U104] JS：防抖
来源：http://dvj.ywan-chungtsiang.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nww.snrcjt.cn

[U105] JS：节流
来源：http://pks.jyoumei.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tkd.shangyingyoupin.top

[U106] JS：日期格式化
来源：http://evg.chenjidiqi.icu

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qcu.yanxiufei.cn

[U107] JS：数字千分位
来源：http://blg.yueranfly.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nor.jinyuanbaomall.cn

[U108] JS：随机整数
来源：http://fjz.bbcook.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vqt.uphjek.com

[U109] JS：数组分组
来源：http://kon.hnxiangtu.top

Object.groupBy(arr, x => x.type)
来源：http://ede.xinyue.icu

[U110] JS：数组分块
来源：http://mpm.xinyue.icu

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dla.gotoacloud.top

[U111] JS：对象转 Map
来源：http://nbs.ybcxt.top

new Map(Object.entries(obj))
来源：http://sip.yongpay.top

[U112] JS：字符串补位
来源：http://ogj.tarul.cn

"7".padStart(3, "0")
来源：http://lak.vqdsnc.cn

[U113] JS：正则替换全部
来源：http://inh.nanxinkj.top

s.replaceAll("a", "b")
来源：http://rto.havefunace.top

[U114] JS：JSON 深比较
来源：http://thv.sufxvd.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://crm.nwbrower.top

[U115] JS：生成 UUID
来源：http://aiz.jiagoushi.top

crypto.randomUUID()
来源：http://hdp.snrcjt.cn

[U116] JS：类型检查（JSDoc）
来源：http://gxd.hywenlv.cn

/** @param {string} name */ function f(name) {}
来源：http://rwf.hammf.cn

[U117] JS：单元测试
来源：http://ume.zdbjq.cn

npm i -D vitest;  npx vitest
来源：http://jfa.meibo888.top

[U118] JS：开发服务器
来源：http://meh.wangdashe.top

npm i -D vite;  npx vite
来源：http://yak.hnqzz.top

[U119] JS：生产构建
来源：http://rbg.hongshengwenyu.top

npx vite build
来源：http://aiw.sjlbkw.cn

[U120] JS：读取环境变量（Vite）
来源：http://qpl.haohaochexian.top

import.meta.env.VITE_API_URL
来源：http://zwm.dianchejie.cn

================================================================================
来源：http://twz.fengsongda.top

统计汇总
来源：http://spr.fzhhl.top

================================================================================
来源：http://olt.xylfe.cn

按语言统计（条）：
来源：http://ldn.daria6918.cn

Python ......... 252
来源：http://hzi.daria6918.cn

PHP ............ 252
来源：http://lqp.xuetiantiany.cn

JavaScript ..... 252
来源：http://qag.chenzaomai.com

TypeScript ..... 212
来源：http://fkv.gogol.net.cn

Java ........... 212
来源：http://sfn.nwbrower.top

Go ............. 212
来源：http://qpg.yj20258888.top

Ruby ........... 212
来源：http://lnz.jinqigfzy.top

C# ............. 212
来源：http://kqh.jiagoushi.top

C .............. 30
来源：http://chk.jlsjyb.cn

C++ ............ 30
来源：http://ecd.andypj.xyz

SQL ............ 90
来源：http://wjv.yj202588.top

Bash ........... 80
来源：http://cow.dashuyun.cn

Kotlin ......... 15
来源：http://usj.gotoacloud.top

Swift .......... 15
来源：http://xot.zhengqikj.top

Lua ............ 10
来源：http://aip.daria6918.cn

Perl ........... 10
来源：http://iot.xinyue.icu

Scala .......... 10
来源：http://jpd.jyoumei.cn

------------------------------------
来源：http://gxr.jyoumei.cn

合计 ........... 2106 条
来源：http://yqx.tianlin.xyz

按章节统计：
来源：http://pmk.hfpthk.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lbb.52xcode.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vty.hongshengwenyu.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nsf.snrcjt.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://flg.jiagoushi.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ozf.iojbl.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rqa.yuxming.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ekd.chenzaomai.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://aos.zhengqikj.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://utj.sjlbkw.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://imq.cucudq.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yqb.ybcxt.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fgn.yfazqb.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lmm.shanyushiyangtech.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ffc.jinqigfzy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fnd.hnqzz.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dnj.yj20258888.top

Q SQL 专题                              90
来源：http://yqe.cqqwz.cn

R Bash 专题                             80
来源：http://jyv.shzxlz.cn

S C / C++ 专题                          60
来源：http://xhf.zdqjudy.top

T 其他语言补充                          60
来源：http://mwh.yueranfly.top

U 高频实用片段                         120
来源：http://gqw.ybcxt.top

------------------------------------
来源：http://dsj.hcnkem.com

合计                                  2106 条
来源：http://jas.sxryk.cn

--------------------------------------------------------------------------------
来源：http://mcc.gzhubu.top

使用提醒
来源：http://ytp.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://nar.aibaodan.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yue.ydjk.org.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zxt.yfazqb.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hve.tian-w.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://dey.yonumen.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sjf.gogol.net.cn

—— 文件结束 ——
来源：http://auk.snrcjt.cn

================================================================================
来源：http://ths.ydzc1.top

程序语言常见例子速查手册（2024 版）
来源：http://erz.wangdashe.top

Common Programming Examples Cheat Book
来源：http://wtz.zhengqikj.top

================================================================================
来源：http://spk.yvedp.cn

【收录内容】
来源：http://yty.zhijiandao.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://phr.xuanzx.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cul.fzhhl.top

SQL · Bash · C · C++
来源：http://wkz.wangdashe.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ows.yfazqb.com

【使用说明】
来源：http://rcu.birdmap.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zuy.zhiwuduotai.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://sag.zhaomingkeji.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ycu.ppjwa.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://twj.jinqigfzy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://hoe.zdqjudy.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ayg.vqdsnc.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bnc.jlsjyb.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qbt.yvedp.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://saf.yfazqb.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lqv.yuxming.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fad.guowangkeji.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hoj.havefunace.top

【文件统计】
来源：http://ebs.iojbl.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pfj.guannengcc.top

--------------------------------------------------------------------------------
来源：http://lxm.chenjidiqi.icu

目  录
来源：http://rpv.fktsv.cn

--------------------------------------------------------------------------------
来源：http://dht.xylfe.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://csq.fengsongda.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pio.shuidangran.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sqm.jqgufenzy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://shh.jinyuanbaomall.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://edz.mhx1999.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rht.hongshengwenyu.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xcc.xinyue.icu

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ezz.birdmap.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://aca.tanke756.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nik.shangyingyoupin.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://exk.zycfv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pgv.chenjidiqi.icu

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vgq.xinyue.icu

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ero.bbcook.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fin.fktsv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ulm.dashuyun.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hwm.dashuyun.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bep.yonumen.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wsn.tianlin.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zni.sxryk.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zjy.yangfankeji.com

================================================================================
来源：http://kjz.shanyushiyangtech.top

A. 基础语法与类型
来源：http://ssd.9152youxi.cn

================================================================================
来源：http://qbv.ydzc1.top

[A01] Hello World
来源：http://blc.svipenyu.cn

Py:   print("Hello, World!")
来源：http://cbo.chenjidiqi.icu

PHP:  echo "Hello, World!";
来源：http://squ.tarul.cn

JS:   console.log("Hello, World!");
来源：http://tow.yfazqb.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jqn.shuidangran.top

Java: System.out.println("Hello, World!");
来源：http://iog.sysykeji.top

Go:   fmt.Println("Hello, World!")
来源：http://dsl.hesvh.cn

Ruby: puts "Hello, World!"
来源：http://ien.hywenlv.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://awa.xuanzx.com

[A02] 变量声明与赋值
来源：http://qxl.guowangkeji.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qtm.daxiang520.top

PHP:  $name = "Alex"; $age = 20;
来源：http://qra.jinghuilouyu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://tgj.0kj1m.cn


<!-- 参考信息 -->