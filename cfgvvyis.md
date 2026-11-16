代发 wailian999

[U33] Py：打包发布
来源：http://nwc.jinghuilouyu.cn

python -m build  （依赖 pyproject.toml）
来源：http://pns.shangyingyoupin.top

[U34] Py：判断编码
来源：http://euq.hywenlv.cn

chardet.detect(raw)
来源：http://chx.sysykeji.top

[U35] Py：发送邮件
来源：http://ehd.cqqwz.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gxq.xingfuxueyuan.xyz

[U36] Py：定时任务
来源：http://ztw.yvedp.cn

schedule.every(10).minutes.do(job)
来源：http://qua.feifeiyinyue.top

[U37] Py：读写 Excel
来源：http://ajl.gaohongyu789.top

pandas.read_excel / DataFrame.to_excel
来源：http://tnz.dianchejie.cn

[U38] Py：获取脚本所在目录
来源：http://rcj.jianghu66.top

Path(__file__).resolve().parent
来源：http://gzr.xuanzx.com

[U39] Py：判断是否在交互环境
来源：http://mgs.hnxiangtu.top

sys.stdout.isatty()
来源：http://wkx.bbcook.cn

[U40] Py：打印到标准错误
来源：http://ujr.shanyushiyangkeji.top

print("err", file=sys.stderr)
来源：http://mar.fktsv.cn

[U41] PHP：初始化 Composer 项目
来源：http://ebi.jlsjyb.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://elo.sysykeji.top

[U42] PHP：PSR-4 自动加载
来源：http://agx.fktsv.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mtg.xuanzx.com

[U43] PHP：声明命名空间
来源：http://jfw.gotoacloud.top

namespace App\Http;
来源：http://qpm.jianghu66.top

[U44] PHP：开启严格类型
来源：http://ejr.bbcook.cn

declare(strict_types=1);
来源：http://yyt.mhx1999.top

[U45] PHP：类型声明与返回类型
来源：http://puu.hammf.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://eev.chenzaomai.com

[U46] PHP：可空类型
来源：http://rpe.tian-w.cn

?string $name = null
来源：http://apw.guannengcc.top

[U47] PHP：联合类型
来源：http://sjx.wangdashe.top

int|string $id
来源：http://xzj.xylfe.cn

[U48] PHP：纯枚举
来源：http://ajw.smart0.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nki.c1oappe.top

[U49] PHP：只读属性
来源：http://rkr.jinghuilouyu.cn

public readonly string $name
来源：http://bue.fzhhl.top

[U50] PHP：构造器属性提升
来源：http://vdp.cqqwz.cn

public function __construct(private int $id) {}
来源：http://srj.aibaodan.cn

[U51] PHP：数组解构
来源：http://tih.guannengcc.top

[$a, $b] = $arr;
来源：http://nng.ywan-chungtsiang.top

[U52] PHP：箭头函数
来源：http://yeb.haohaochexian.top

$double = fn($x) => $x * 2;
来源：http://lxv.sjlbkw.cn

[U53] PHP：空合并运算符
来源：http://tzo.chenzaomai.com

$v = $a ?? $b ?? "default";
来源：http://poz.redwolf501.top

[U54] PHP：空安全调用
来源：http://afn.yangfankeji.com

$obj?->method()
来源：http://dfp.c1oappe.top

[U55] PHP：match 表达式
来源：http://jaf.wangdashe.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bun.fengsongda.top

[U56] PHP：命名参数
来源：http://sbi.bjfxy.top

f(a: 1, b: 2)
来源：http://umn.0kj1m.cn

[U57] PHP：字符串插值
来源：http://why.zhijiandao.cn

"值: {$a}"
来源：http://jiu.xuetiantiany.cn

[U58] PHP：数组三件套
来源：http://urn.iojbl.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dqy.dashuyun.cn

[U59] PHP：自定义排序
来源：http://dsy.jinghuilouyu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://knd.xuanzx.com

[U60] PHP：JSON 编解码
来源：http://emh.xylfe.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xkt.ydzc1.top

[U61] PHP：正则
来源：http://hfk.vehdjk.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xpk.52xcode.cn

[U62] PHP：日期对象
来源：http://anb.fktsv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rrx.yongpay.top

[U63] PHP：文件读写
来源：http://yvu.zycfv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ffq.wangshuangyany.cn

[U64] PHP：目录遍历
来源：http://uwp.shzxlz.cn

glob("dir/*.php");  scandir("dir");
来源：http://ivw.fktsv.cn

[U65] PHP：会话
来源：http://umo.aibaodan.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vjf.cashguo.top

[U66] PHP：设置 Cookie
来源：http://cfj.yanxiufei.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pnl.nanxuanxn.top

[U67] PHP：处理文件上传
来源：http://vdh.sysykeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mnr.yangfankeji.com

[U68] PHP：PDO 连接
来源：http://nud.yj20258888.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nmv.vqdsnc.cn

[U69] PHP：PDO 预处理
来源：http://kpx.hnxiangtu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://euy.uphjek.com

[U70] PHP：PDO 事务
来源：http://oez.cdnleiting.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jlp.ydzc1.top

[U71] PHP：抛出异常
来源：http://qrf.tianlin.xyz

throw new RuntimeException("失败", 500);
来源：http://llw.svipenyu.cn

[U72] PHP：写错误日志
来源：http://fev.c1oappe.top

error_log("失败: " . $e->getMessage());
来源：http://yvr.shangyingyoupin.top

[U73] PHP：读取 ini 配置
来源：http://cmw.chenjidiqi.icu

parse_ini_file("config.ini", true)
来源：http://oqv.zhijiandao.cn

[U74] PHP：读取环境变量
来源：http://qyz.jiagoushi.top

getenv("APP_ENV") ?: "production"
来源：http://jlq.zhengqikj.top

[U75] PHP：依赖注入
来源：http://oiq.svipenyu.cn

composer require psr/container
来源：http://vtq.9152youxi.cn

[U76] PHP：简单路由
来源：http://xlb.shangyingyoupin.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yvy.pycfn.com

[U77] PHP：模板渲染
来源：http://jab.hongshengwenyu.top

composer require twig/twig
来源：http://pnq.zhongyouzk.top

[U78] PHP：单元测试
来源：http://hdj.chenjidiqi.icu

composer require --dev phpunit/phpunit
来源：http://wgm.sufxvd.cn

[U79] PHP：静态分析
来源：http://pee.hfpthk.cn

composer require --dev phpstan/phpstan
来源：http://vis.xuetiantiany.cn

[U80] PHP：代码规范修复
来源：http://kax.jiagoushi.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://cuj.jianghu66.top

[U81] JS：初始化项目
来源：http://bnl.fzhhl.top

npm init -y;  npm i express
来源：http://gli.yangfankeji.com

[U82] JS：package.json 脚本
来源：http://vxt.ppjwa.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ulf.xuetiantiany.cn

[U83] JS：ES Module 导入导出
来源：http://ppp.yuxming.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nju.yuanzhike.top

[U84] JS：CommonJS 写法
来源：http://btp.yvedp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nca.xuanzx.com

[U85] JS：可选链
来源：http://hrf.hongshengwenyu.top

a?.b?.c
来源：http://vtg.ybcxt.top

[U86] JS：空值合并
来源：http://ivj.ivvv.top

a ?? b
来源：http://zmk.fzhhl.top

[U87] JS：解构默认值
来源：http://gvy.zhengqikj.top

const { a = 1, b = 2 } = obj;
来源：http://nni.tarul.cn

[U88] JS：对象展开合并
来源：http://qrt.sjlbkw.cn

{ ...a, ...b }
来源：http://icg.nwbrower.top

[U89] JS：数组去重
来源：http://pnb.nanxinkj.top

[...new Set(arr)]
来源：http://esn.zycfv.cn

[U90] JS：数字数组排序
来源：http://qgb.aibaodan.cn

[...arr].sort((a, b) => a - b)
来源：http://drv.jinyuanbaomall.cn

[U91] JS：对象键值遍历
来源：http://vzr.yuanzhike.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sjf.zycfv.cn

[U92] JS：深拷贝
来源：http://zgi.yj20258888.top

structuredClone(obj)
来源：http://jmi.shanyushiyangtech.top

[U93] JS：模板字符串
来源：http://mek.hesvh.cn

`共 ${n} 条`
来源：http://xsn.yanxiufei.cn

[U94] JS：箭头函数
来源：http://rdj.bjfxy.top

const double = x => x * 2;
来源：http://sru.cucudq.cn

[U95] JS：Promise 包装
来源：http://gnn.sxryk.cn

new Promise((resolve, reject) => {})
来源：http://nwa.xylfe.cn

[U96] JS：async/await 与异常
来源：http://ith.gaohongyu789.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fdw.vehdjk.com

[U97] JS：并发请求
来源：http://lux.jiagoushi.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://yma.sweek.top

[U98] JS：fetch 带 JSON
来源：http://sxr.zdbjq.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ctw.shangyingyoupin.top

[U99] JS：事件监听
来源：http://vwn.andypj.xyz

el.addEventListener("click", e => {})
来源：http://ubw.zdbjq.cn

[U100] JS：DOM 查询
来源：http://zsj.hcnkem.com

document.querySelector(".item")
来源：http://jgz.jqgufenzy.top

[U101] JS：classList 操作
来源：http://yib.uphjek.com

el.classList.toggle("active")
来源：http://mgx.yuxming.cn

[U102] JS：本地存储
来源：http://lxw.tian-w.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sfm.svipenyu.cn

[U103] JS：定时器
来源：http://nbs.gzhubu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mkf.jinqigufen.top

[U104] JS：防抖
来源：http://tff.iojbl.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zpw.shuidangran.top

[U105] JS：节流
来源：http://che.jinghuilouyu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jgm.bjfxy.top

[U106] JS：日期格式化
来源：http://azg.epnwcf.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wjz.dashuyun.cn

[U107] JS：数字千分位
来源：http://tjv.cqqwz.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wrt.cqqwz.cn

[U108] JS：随机整数
来源：http://pal.fktsv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://buf.shzxlz.cn

[U109] JS：数组分组
来源：http://tpk.sjlbkw.cn

Object.groupBy(arr, x => x.type)
来源：http://qjt.yuanzhike.top

[U110] JS：数组分块
来源：http://hnw.ydjk.org.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://srq.gogol.net.cn

[U111] JS：对象转 Map
来源：http://deu.wangshuangyany.cn

new Map(Object.entries(obj))
来源：http://qby.fanxiaobao.xyz

[U112] JS：字符串补位
来源：http://dvl.yfazqb.com

"7".padStart(3, "0")
来源：http://eei.ehwqpu.com

[U113] JS：正则替换全部
来源：http://ysh.shangyingyoupin.top

s.replaceAll("a", "b")
来源：http://bwh.xingfuxueyuan.xyz

[U114] JS：JSON 深比较
来源：http://saa.havefunace.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://qxw.bjfxy.top

[U115] JS：生成 UUID
来源：http://cud.jinyuanbaomall.cn

crypto.randomUUID()
来源：http://pyw.zdqjudy.top

[U116] JS：类型检查（JSDoc）
来源：http://ecx.bbcook.cn

/** @param {string} name */ function f(name) {}
来源：http://sxn.9152youxi.cn

[U117] JS：单元测试
来源：http://xda.cheryme.top

npm i -D vitest;  npx vitest
来源：http://rrt.meibo888.top

[U118] JS：开发服务器
来源：http://qlw.yj20258888.top

npm i -D vite;  npx vite
来源：http://gzg.jinqigufen.top

[U119] JS：生产构建
来源：http://syu.xinyue.icu

npx vite build
来源：http://qxy.yj20258888.top

[U120] JS：读取环境变量（Vite）
来源：http://mrz.cdnleiting.top

import.meta.env.VITE_API_URL
来源：http://bns.mhx1999.top

================================================================================
来源：http://gvi.pycfn.com

统计汇总
来源：http://tye.vqdsnc.cn

================================================================================
来源：http://fzx.gogol.net.cn

按语言统计（条）：
来源：http://rbd.gotoacloud.top

Python ......... 252
来源：http://jdk.chenlongwang.top

PHP ............ 252
来源：http://bcp.ehwqpu.com

JavaScript ..... 252
来源：http://ojy.snrcjt.cn

TypeScript ..... 212
来源：http://hel.tanke756.top

Java ........... 212
来源：http://xda.snrcjt.cn

Go ............. 212
来源：http://isz.hcnkem.com

Ruby ........... 212
来源：http://xsc.xuanzx.com

C# ............. 212
来源：http://gkt.c1oappe.top

C .............. 30
来源：http://fuw.fehbvm.com

C++ ............ 30
来源：http://csl.cashguo.top

SQL ............ 90
来源：http://ppw.xziqi.cn

Bash ........... 80
来源：http://plz.xinyue.icu

Kotlin ......... 15
来源：http://hpv.chenjidiqi.icu

Swift .......... 15
来源：http://bie.yangfankeji.com

Lua ............ 10
来源：http://oza.cucudq.cn

Perl ........... 10
来源：http://qlv.c1oappe.top

Scala .......... 10
来源：http://twp.daria6918.cn

------------------------------------
来源：http://jug.hysaishi.cn

合计 ........... 2106 条
来源：http://yvx.fehbvm.com

按章节统计：
来源：http://svk.epnwcf.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rtd.zdqjudy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tsy.guowangkeji.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fix.zhixingplan.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rny.zdqjudy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vvt.zhongyouzk.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pqj.jianghu66.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ucy.zhoulong.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bue.mhx1999.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://atf.jlsjyb.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://epf.chenjidiqi.icu

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ekx.wangdashe.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nya.aizwys.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vgj.birdmap.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lgs.nanxuanxn.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tks.zdbjq.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kiz.epnwcf.com

Q SQL 专题                              90
来源：http://rnd.yongpay.top

R Bash 专题                             80
来源：http://apy.316326.xyz

S C / C++ 专题                          60
来源：http://nxz.wangshuangyany.cn

T 其他语言补充                          60
来源：http://qar.xinyue.icu

U 高频实用片段                         120
来源：http://nnr.sysykeji.top

------------------------------------
来源：http://cym.sysykeji.top

合计                                  2106 条
来源：http://bsc.meibo888.top

--------------------------------------------------------------------------------
来源：http://ruz.0kj1m.cn

使用提醒
来源：http://gea.yuxming.cn

--------------------------------------------------------------------------------
来源：http://sdc.sufxvd.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tdn.wangdashe.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fma.snrcjt.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ywc.cheryme.top

在旧版本上使用前请先确认语法支持情况。
来源：http://jet.redwolf501.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yvt.52xcode.cn

—— 文件结束 ——
来源：http://xsr.guowangkeji.top

================================================================================
来源：http://nfu.vehdjk.com

程序语言常见例子速查手册（2024 版）
来源：http://qab.gotoacloud.top

Common Programming Examples Cheat Book
来源：http://hrg.yj20258.top

================================================================================
来源：http://izz.jqgfzy.top

【收录内容】
来源：http://gxs.yuanzhike.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://kwa.hywenlv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nrb.ybcxt.top

SQL · Bash · C · C++
来源：http://nbu.cucudq.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://weq.yongpay.top

【使用说明】
来源：http://gmm.pengpengdd.cyou

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yxp.xylfe.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nbz.chenlongwang.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ira.tianlin.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dna.fanxiaobao.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://jem.cqqwz.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://aam.uphjek.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nam.ctjpmb.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gdx.gotoacloud.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mvb.hnxiangtu.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uja.chenzaomai.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yxq.jinyuanbaomall.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cjb.bjfxy.top

【文件统计】
来源：http://lku.yj202588.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bqw.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://phi.jinqigufen.top

目  录
来源：http://ivr.gaohongyu789.top

--------------------------------------------------------------------------------
来源：http://fav.zhixingplan.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jll.hywenlv.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vkg.chenlongwang.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://aru.feifeiyinyue.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://thh.uphjek.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://erb.xylfe.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://orv.epnwcf.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ngo.daxiang520.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hui.zdbjq.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://aeg.gzhubu.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wis.snrcjt.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qwm.cdnleiting.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uab.vqdsnc.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dcp.yj202588.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bvf.xuanzx.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nwi.zdqjudy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://inw.feifeiyinyue.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://olm.xinyue.icu

R. Bash 专题                   （第 18 节，80 条）
来源：http://pzk.yvedp.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cmk.gzhubu.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nra.iojbl.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hxf.jiagoushi.top

================================================================================
来源：http://rnf.cdnleiting.top

A. 基础语法与类型
来源：http://rul.feifeiyinyue.top

================================================================================
来源：http://gak.zycfv.cn

[A01] Hello World
来源：http://qqm.shanyushiyangtech.top

Py:   print("Hello, World!")
来源：http://oia.ppjwa.cn

PHP:  echo "Hello, World!";
来源：http://tzf.vqdsnc.cn

JS:   console.log("Hello, World!");
来源：http://hez.redwolf501.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ohw.ywan-chungtsiang.top

Java: System.out.println("Hello, World!");
来源：http://wcw.uphjek.com

Go:   fmt.Println("Hello, World!")
来源：http://ijh.dashuyun.cn

Ruby: puts "Hello, World!"
来源：http://jjy.yonumen.top

C#:   Console.WriteLine("Hello, World!");
来源：http://fyr.dianchejie.cn

[A02] 变量声明与赋值
来源：http://jql.guannengcc.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ckb.yj202588.top

PHP:  $name = "Alex"; $age = 20;
来源：http://mwe.wangshuangyany.cn

JS:   let name = "Alex"; const age = 20;
来源：http://sds.zycfv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cez.hammf.cn

Java: String name = "Alex"; int age = 20;
来源：http://ffz.daxiang520.top

Go:   name := "Alex"; age := 20
来源：http://zzp.fehbvm.com

Ruby: name = "Alex"; age = 20
来源：http://beq.sxryk.cn


<!-- 参考信息 -->