代发 wailian999

[U33] Py：打包发布
来源：http://cmo.zhaomingkeji.xyz

python -m build  （依赖 pyproject.toml）
来源：http://xzc.jinghuilouyu.cn

[U34] Py：判断编码
来源：http://thi.0kj1m.cn

chardet.detect(raw)
来源：http://src.cheryme.top

[U35] Py：发送邮件
来源：http://hil.nanxinkj.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hun.sxryk.cn

[U36] Py：定时任务
来源：http://ttk.andypj.xyz

schedule.every(10).minutes.do(job)
来源：http://klp.cqqwz.cn

[U37] Py：读写 Excel
来源：http://iaf.quarkkingdee.top

pandas.read_excel / DataFrame.to_excel
来源：http://lbo.zhongyouzk.top

[U38] Py：获取脚本所在目录
来源：http://vtn.dashuyun.cn

Path(__file__).resolve().parent
来源：http://oyn.dianchejie.cn

[U39] Py：判断是否在交互环境
来源：http://vgu.yonumen.top

sys.stdout.isatty()
来源：http://pdj.tarul.cn

[U40] Py：打印到标准错误
来源：http://kws.dianchejie.cn

print("err", file=sys.stderr)
来源：http://dqi.gotoacloud.top

[U41] PHP：初始化 Composer 项目
来源：http://qsa.quarkkingdee.top

composer init;  composer require guzzlehttp/guzzle
来源：http://wmy.guowangkeji.top

[U42] PHP：PSR-4 自动加载
来源：http://plx.zhaomingkeji.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://snw.quarkkingdee.top

[U43] PHP：声明命名空间
来源：http://xro.hnqzz.top

namespace App\Http;
来源：http://neb.xuanzx.com

[U44] PHP：开启严格类型
来源：http://wnk.zdqjudy.top

declare(strict_types=1);
来源：http://wit.hesvh.cn

[U45] PHP：类型声明与返回类型
来源：http://xbg.zhaomingkeji.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://hmy.andypj.xyz

[U46] PHP：可空类型
来源：http://uaf.yongpay.top

?string $name = null
来源：http://dew.52xcode.cn

[U47] PHP：联合类型
来源：http://dya.yueranfly.top

int|string $id
来源：http://pkk.yuanzhike.top

[U48] PHP：纯枚举
来源：http://wkh.jiagoushi.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://roi.svipenyu.cn

[U49] PHP：只读属性
来源：http://jre.tarul.cn

public readonly string $name
来源：http://pug.gotoacloud.top

[U50] PHP：构造器属性提升
来源：http://wkn.yongpay.top

public function __construct(private int $id) {}
来源：http://emw.xingfuxueyuan.xyz

[U51] PHP：数组解构
来源：http://dvd.daxiang520.top

[$a, $b] = $arr;
来源：http://yue.jlsjyb.cn

[U52] PHP：箭头函数
来源：http://bku.hammf.cn

$double = fn($x) => $x * 2;
来源：http://sla.redwolf501.top

[U53] PHP：空合并运算符
来源：http://kpo.shzxlz.cn

$v = $a ?? $b ?? "default";
来源：http://ked.xylfe.cn

[U54] PHP：空安全调用
来源：http://rhv.uphjek.com

$obj?->method()
来源：http://pni.kuanghao11.cn

[U55] PHP：match 表达式
来源：http://xac.gzhubu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ahk.snrcjt.cn

[U56] PHP：命名参数
来源：http://qgs.sxryk.cn

f(a: 1, b: 2)
来源：http://rrh.52xcode.cn

[U57] PHP：字符串插值
来源：http://zhv.zhengqikj.top

"值: {$a}"
来源：http://cbi.bjfxy.top

[U58] PHP：数组三件套
来源：http://hen.havefunace.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://itv.jyoumei.cn

[U59] PHP：自定义排序
来源：http://ghn.aizwys.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hsl.jqgfzy.top

[U60] PHP：JSON 编解码
来源：http://cxe.shuidangran.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://awf.nanxuanxn.top

[U61] PHP：正则
来源：http://fqg.ydzc1.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hcf.jianghu66.top

[U62] PHP：日期对象
来源：http://iqg.ydzc1.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kjx.shanyushiyangtech.top

[U63] PHP：文件读写
来源：http://yyl.wangshuangyany.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wuq.shanyushiyangkeji.top

[U64] PHP：目录遍历
来源：http://yly.fengsongda.top

glob("dir/*.php");  scandir("dir");
来源：http://rad.zhijiandao.cn

[U65] PHP：会话
来源：http://yoa.vehdjk.com

session_start();  $_SESSION["uid"] = 1;
来源：http://zhn.chenzaomai.com

[U66] PHP：设置 Cookie
来源：http://jjq.xinyue.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zpb.shangyingyoupin.top

[U67] PHP：处理文件上传
来源：http://xnh.yvedp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xjo.andypj.xyz

[U68] PHP：PDO 连接
来源：http://cqv.c1oappe.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://boj.jqgufenzy.top

[U69] PHP：PDO 预处理
来源：http://adk.hnxiangtu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xtl.c1oappe.top

[U70] PHP：PDO 事务
来源：http://wjk.hnqzz.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tlt.gogol.net.cn

[U71] PHP：抛出异常
来源：http://cpd.yuxming.cn

throw new RuntimeException("失败", 500);
来源：http://kvj.andypj.xyz

[U72] PHP：写错误日志
来源：http://gdy.gogol.net.cn

error_log("失败: " . $e->getMessage());
来源：http://tmd.daria6918.cn

[U73] PHP：读取 ini 配置
来源：http://nvj.haohaochexian.top

parse_ini_file("config.ini", true)
来源：http://dde.tanke756.top

[U74] PHP：读取环境变量
来源：http://mjn.jinqigufen.top

getenv("APP_ENV") ?: "production"
来源：http://xvd.fzhhl.top

[U75] PHP：依赖注入
来源：http://inz.meibo888.top

composer require psr/container
来源：http://gdu.jqgufenzy.top

[U76] PHP：简单路由
来源：http://azf.ybcxt.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://glo.pengpengdd.cyou

[U77] PHP：模板渲染
来源：http://lko.smart0.xyz

composer require twig/twig
来源：http://dvx.nanxinkj.top

[U78] PHP：单元测试
来源：http://ulv.hammf.cn

composer require --dev phpunit/phpunit
来源：http://hmm.bjfxy.top

[U79] PHP：静态分析
来源：http://zpz.cucudq.cn

composer require --dev phpstan/phpstan
来源：http://dit.aizwys.cn

[U80] PHP：代码规范修复
来源：http://uam.shanyushiyangkeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ird.hnxiangtu.top

[U81] JS：初始化项目
来源：http://klv.yj202588.top

npm init -y;  npm i express
来源：http://odq.hongshengwenyu.top

[U82] JS：package.json 脚本
来源：http://izo.iojbl.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jkj.sufxvd.cn

[U83] JS：ES Module 导入导出
来源：http://zxy.zhaomingkeji.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://bfr.uphjek.com

[U84] JS：CommonJS 写法
来源：http://ulj.zycfv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ovc.wangshuangyany.cn

[U85] JS：可选链
来源：http://bvk.jianghu66.top

a?.b?.c
来源：http://thb.gotoacloud.top

[U86] JS：空值合并
来源：http://bwe.xingfuxueyuan.xyz

a ?? b
来源：http://tnz.hesvh.cn

[U87] JS：解构默认值
来源：http://jch.meibo888.top

const { a = 1, b = 2 } = obj;
来源：http://lze.yongpay.top

[U88] JS：对象展开合并
来源：http://jtz.nanxinkj.top

{ ...a, ...b }
来源：http://zoy.xuetiantiany.cn

[U89] JS：数组去重
来源：http://sfd.hesvh.cn

[...new Set(arr)]
来源：http://rjz.shangyingyoupin.top

[U90] JS：数字数组排序
来源：http://tha.wangshuangyany.cn

[...arr].sort((a, b) => a - b)
来源：http://gsu.gaohongyu789.top

[U91] JS：对象键值遍历
来源：http://ciz.feifeiyinyue.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zac.jinqigfzy.top

[U92] JS：深拷贝
来源：http://sma.52xcode.cn

structuredClone(obj)
来源：http://ybp.feifeiyinyue.top

[U93] JS：模板字符串
来源：http://afc.haohaochexian.top

`共 ${n} 条`
来源：http://twa.xuanzx.com

[U94] JS：箭头函数
来源：http://gsk.iojbl.cn

const double = x => x * 2;
来源：http://ppo.cqqwz.cn

[U95] JS：Promise 包装
来源：http://tmp.tian-w.cn

new Promise((resolve, reject) => {})
来源：http://lmi.yangfankeji.com

[U96] JS：async/await 与异常
来源：http://wni.hywenlv.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ghg.yanxiufei.cn

[U97] JS：并发请求
来源：http://gfh.zycfv.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://zdi.redwolf501.top

[U98] JS：fetch 带 JSON
来源：http://lgq.jiagoushi.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gao.chenlongwang.top

[U99] JS：事件监听
来源：http://bfj.xuetiantiany.cn

el.addEventListener("click", e => {})
来源：http://jaz.yj20258.top

[U100] JS：DOM 查询
来源：http://xga.guannengcc.top

document.querySelector(".item")
来源：http://zhk.ivvv.top

[U101] JS：classList 操作
来源：http://nzs.zycfv.cn

el.classList.toggle("active")
来源：http://bln.tian-w.cn

[U102] JS：本地存储
来源：http://gep.jinghuilouyu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vwe.yonumen.top

[U103] JS：定时器
来源：http://tsz.dashuyun.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wvx.hesvh.cn

[U104] JS：防抖
来源：http://xoe.epnwcf.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qqq.52xcode.cn

[U105] JS：节流
来源：http://fwj.jiagoushi.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ygy.snrcjt.cn

[U106] JS：日期格式化
来源：http://nmi.ydjk.org.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://byv.yj20258.top

[U107] JS：数字千分位
来源：http://crm.0kj1m.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cmq.jlsjyb.cn

[U108] JS：随机整数
来源：http://xof.gotoacloud.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ewz.feifeiyinyue.top

[U109] JS：数组分组
来源：http://kpy.hongshengwenyu.top

Object.groupBy(arr, x => x.type)
来源：http://gav.dianchejie.cn

[U110] JS：数组分块
来源：http://zoh.shanyushiyangtech.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://por.havefunace.top

[U111] JS：对象转 Map
来源：http://hvp.guannengcc.top

new Map(Object.entries(obj))
来源：http://alg.jqgfzy.top

[U112] JS：字符串补位
来源：http://sqs.cucudq.cn

"7".padStart(3, "0")
来源：http://ovg.yj20258888.top

[U113] JS：正则替换全部
来源：http://vfl.zdqjudy.top

s.replaceAll("a", "b")
来源：http://ila.316326.xyz

[U114] JS：JSON 深比较
来源：http://aqr.yueranfly.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://cep.gzhubu.top

[U115] JS：生成 UUID
来源：http://jeu.redwolf501.top

crypto.randomUUID()
来源：http://kau.zhoulong.xyz

[U116] JS：类型检查（JSDoc）
来源：http://pfr.yongpay.top

/** @param {string} name */ function f(name) {}
来源：http://usd.vqdsnc.cn

[U117] JS：单元测试
来源：http://jvj.zhiwuduotai.top

npm i -D vitest;  npx vitest
来源：http://qef.daria6918.cn

[U118] JS：开发服务器
来源：http://hmd.yj20258888.top

npm i -D vite;  npx vite
来源：http://mrx.yvedp.cn

[U119] JS：生产构建
来源：http://ovq.hnxiangtu.top

npx vite build
来源：http://ilq.zhoulong.xyz

[U120] JS：读取环境变量（Vite）
来源：http://fgu.fanxiaobao.xyz

import.meta.env.VITE_API_URL
来源：http://hmn.gotoacloud.top

================================================================================
来源：http://myh.feifeiyinyue.top

统计汇总
来源：http://bwg.yfazqb.com

================================================================================
来源：http://qjp.smart0.xyz

按语言统计（条）：
来源：http://rsy.zhengqikj.top

Python ......... 252
来源：http://avr.chenlongwang.top

PHP ............ 252
来源：http://avk.wangshuangyany.cn

JavaScript ..... 252
来源：http://ros.shanyushiyangkeji.top

TypeScript ..... 212
来源：http://dgs.smart0.xyz

Java ........... 212
来源：http://wip.nanxinkj.top

Go ............. 212
来源：http://tim.epnwcf.com

Ruby ........... 212
来源：http://knw.hammf.cn

C# ............. 212
来源：http://iuu.pycfn.com

C .............. 30
来源：http://xky.0kj1m.cn

C++ ............ 30
来源：http://eaa.yanxiufei.cn

SQL ............ 90
来源：http://ruy.birdmap.top

Bash ........... 80
来源：http://hyn.gogol.net.cn

Kotlin ......... 15
来源：http://msb.andypj.xyz

Swift .......... 15
来源：http://qmw.sweek.top

Lua ............ 10
来源：http://iws.jiagoushi.top

Perl ........... 10
来源：http://emq.wangdashe.top

Scala .......... 10
来源：http://bdp.sysykeji.top

------------------------------------
来源：http://txt.yvedp.cn

合计 ........... 2106 条
来源：http://ykz.zycfv.cn

按章节统计：
来源：http://pgl.ywan-chungtsiang.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://znf.fktsv.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rsy.ywan-chungtsiang.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ike.jqgfzy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pcj.sysykeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bjl.xylfe.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bxj.yj202588.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pdr.guowangkeji.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hef.sjlbkw.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qbr.nanxinkj.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fpb.sweek.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ouq.bjfxy.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xau.hysaishi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xid.cucudq.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vwv.zycfv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xbi.ydzc1.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hfi.yueranfly.top

Q SQL 专题                              90
来源：http://xsm.chenzaomai.com

R Bash 专题                             80
来源：http://jpt.havefunace.top

S C / C++ 专题                          60
来源：http://hxt.meibo888.top

T 其他语言补充                          60
来源：http://nqt.bbcook.cn

U 高频实用片段                         120
来源：http://fki.aizwys.cn

------------------------------------
来源：http://rzj.gaohongyu789.top

合计                                  2106 条
来源：http://qkx.fehbvm.com

--------------------------------------------------------------------------------
来源：http://iys.yuxming.cn

使用提醒
来源：http://lql.cucudq.cn

--------------------------------------------------------------------------------
来源：http://yaa.zhaomingkeji.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pei.zdbjq.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qdd.guannengcc.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lap.yj20258.top

在旧版本上使用前请先确认语法支持情况。
来源：http://rjc.cucudq.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tyi.ivvv.top

—— 文件结束 ——
来源：http://siq.fanxiaobao.xyz

================================================================================
来源：http://qry.jinqigfzy.top

程序语言常见例子速查手册（2024 版）
来源：http://bep.dianchejie.cn

Common Programming Examples Cheat Book
来源：http://fre.hesvh.cn

================================================================================
来源：http://xwb.jianghu66.top

【收录内容】
来源：http://oep.yj20258888.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://sry.jinqigfzy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tdc.52xcode.cn

SQL · Bash · C · C++
来源：http://vny.fehbvm.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ioj.shuidangran.top

【使用说明】
来源：http://dqz.sxryk.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rmk.mhx1999.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rtb.yuxming.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://eik.shanyushiyangtech.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jgp.zhijiandao.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://uqo.sjlbkw.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hmg.shanyushiyangtech.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mhn.tarul.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ixr.52xcode.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://eew.guowangkeji.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://meq.smart0.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bkf.fzhhl.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tat.ydzc1.top

【文件统计】
来源：http://njc.jyoumei.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://uqs.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://pac.guannengcc.top

目  录
来源：http://njt.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://wbe.xziqi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yop.daxiang520.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nsh.shuidangran.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zcp.jlsjyb.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ouw.316326.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ffm.xylfe.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mea.aibaodan.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lho.tian-w.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ssr.jyoumei.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jkq.jqgfzy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://iwg.jinqigufen.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://eiu.hysaishi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://slh.wangdashe.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://oox.yanxiufei.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ztd.316326.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wlh.shuidangran.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dil.sxryk.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fws.yuxming.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ipv.haohaochexian.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pnc.fehbvm.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://oro.yongpay.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ulj.ybcxt.top

================================================================================
来源：http://asg.hesvh.cn

A. 基础语法与类型
来源：http://dnv.andypj.xyz

================================================================================
来源：http://hbf.vehdjk.com

[A01] Hello World
来源：http://kxp.snrcjt.cn

Py:   print("Hello, World!")
来源：http://jlf.xuetiantiany.cn

PHP:  echo "Hello, World!";
来源：http://cgk.yfazqb.com

JS:   console.log("Hello, World!");
来源：http://jjt.havefunace.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zuc.cdnleiting.top

Java: System.out.println("Hello, World!");
来源：http://cxz.redwolf501.top

Go:   fmt.Println("Hello, World!")
来源：http://utv.chenzaomai.com

Ruby: puts "Hello, World!"
来源：http://kar.jinyuanbaomall.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://yyx.tarul.cn

[A02] 变量声明与赋值
来源：http://qke.xziqi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vyh.yuanzhike.top

PHP:  $name = "Alex"; $age = 20;
来源：http://apt.jinqigfzy.top

JS:   let name = "Alex"; const age = 20;
来源：http://msv.guowangkeji.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hbe.hongshengwenyu.top

Java: String name = "Alex"; int age = 20;
来源：http://bvm.vehdjk.com

Go:   name := "Alex"; age := 20
来源：http://oov.fengsongda.top

Ruby: name = "Alex"; age = 20
来源：http://nsy.andypj.xyz


<!-- 参考信息 -->