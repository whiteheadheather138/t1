代发 wailian999

[U33] Py：打包发布
来源：http://xco.zhiwuduotai.top

python -m build  （依赖 pyproject.toml）
来源：http://nwi.uphjek.com

[U34] Py：判断编码
来源：http://iex.fktsv.cn

chardet.detect(raw)
来源：http://tyx.jinqigfzy.top

[U35] Py：发送邮件
来源：http://brs.quarkkingdee.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ghj.jinyuanbaomall.cn

[U36] Py：定时任务
来源：http://pbd.quarkkingdee.top

schedule.every(10).minutes.do(job)
来源：http://rwc.zhengqikj.top

[U37] Py：读写 Excel
来源：http://ilg.zhoulong.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://bgg.sysykeji.top

[U38] Py：获取脚本所在目录
来源：http://yyu.jianghu66.top

Path(__file__).resolve().parent
来源：http://dwi.yuxming.cn

[U39] Py：判断是否在交互环境
来源：http://zjh.smart0.xyz

sys.stdout.isatty()
来源：http://hut.zdqjudy.top

[U40] Py：打印到标准错误
来源：http://dfp.zhixingplan.top

print("err", file=sys.stderr)
来源：http://xyc.tian-w.cn

[U41] PHP：初始化 Composer 项目
来源：http://bhi.yfazqb.com

composer init;  composer require guzzlehttp/guzzle
来源：http://tte.gaohongyu789.top

[U42] PHP：PSR-4 自动加载
来源：http://xqy.guowangkeji.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qln.ppjwa.cn

[U43] PHP：声明命名空间
来源：http://hve.tarul.cn

namespace App\Http;
来源：http://ozn.c1oappe.top

[U44] PHP：开启严格类型
来源：http://lsd.fktsv.cn

declare(strict_types=1);
来源：http://kfh.shangyingyoupin.top

[U45] PHP：类型声明与返回类型
来源：http://tuc.nanxinkj.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://muy.sysykeji.top

[U46] PHP：可空类型
来源：http://eko.shanyushiyangkeji.top

?string $name = null
来源：http://nbm.yangfankeji.com

[U47] PHP：联合类型
来源：http://vgy.sysykeji.top

int|string $id
来源：http://rsm.zhijiandao.cn

[U48] PHP：纯枚举
来源：http://wao.cashguo.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tmi.cashguo.top

[U49] PHP：只读属性
来源：http://rsc.guowangkeji.top

public readonly string $name
来源：http://awr.mhx1999.top

[U50] PHP：构造器属性提升
来源：http://jsk.zhiwuduotai.top

public function __construct(private int $id) {}
来源：http://uzl.hcnkem.com

[U51] PHP：数组解构
来源：http://msw.hesvh.cn

[$a, $b] = $arr;
来源：http://otv.nwbrower.top

[U52] PHP：箭头函数
来源：http://zng.sweek.top

$double = fn($x) => $x * 2;
来源：http://pkl.jinqigufen.top

[U53] PHP：空合并运算符
来源：http://gos.xinyue.icu

$v = $a ?? $b ?? "default";
来源：http://fvc.aizwys.cn

[U54] PHP：空安全调用
来源：http://ufb.yj202588.top

$obj?->method()
来源：http://jsu.yuanzhike.top

[U55] PHP：match 表达式
来源：http://bbp.snrcjt.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xls.fehbvm.com

[U56] PHP：命名参数
来源：http://ufx.zhiwuduotai.top

f(a: 1, b: 2)
来源：http://llx.ctjpmb.com

[U57] PHP：字符串插值
来源：http://obq.xuetiantiany.cn

"值: {$a}"
来源：http://wxc.dashuyun.cn

[U58] PHP：数组三件套
来源：http://gtv.xylfe.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fbq.shuidangran.top

[U59] PHP：自定义排序
来源：http://lkr.dashuyun.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://znv.jinqigufen.top

[U60] PHP：JSON 编解码
来源：http://ygr.yangfankeji.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sgy.cqqwz.cn

[U61] PHP：正则
来源：http://xbl.tian-w.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://prz.316326.xyz

[U62] PHP：日期对象
来源：http://bgv.fzhhl.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tgd.redwolf501.top

[U63] PHP：文件读写
来源：http://xut.tianlin.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dnf.guowangkeji.top

[U64] PHP：目录遍历
来源：http://lcj.zhongyouzk.top

glob("dir/*.php");  scandir("dir");
来源：http://skr.tanke756.top

[U65] PHP：会话
来源：http://uxx.gzhubu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rjl.mhx1999.top

[U66] PHP：设置 Cookie
来源：http://thc.feifeiyinyue.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fsk.shanyushiyangtech.top

[U67] PHP：处理文件上传
来源：http://tmp.jinghuilouyu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kno.xylfe.cn

[U68] PHP：PDO 连接
来源：http://nss.vehdjk.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gjj.vqdsnc.cn

[U69] PHP：PDO 预处理
来源：http://kzs.316326.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ysv.mhx1999.top

[U70] PHP：PDO 事务
来源：http://lqk.ctjpmb.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ijs.hfpthk.cn

[U71] PHP：抛出异常
来源：http://abd.tian-w.cn

throw new RuntimeException("失败", 500);
来源：http://iqq.cashguo.top

[U72] PHP：写错误日志
来源：http://inj.sysykeji.top

error_log("失败: " . $e->getMessage());
来源：http://arv.bbcook.cn

[U73] PHP：读取 ini 配置
来源：http://ngv.yj20258888.top

parse_ini_file("config.ini", true)
来源：http://tph.daxiang520.top

[U74] PHP：读取环境变量
来源：http://dkd.jianghu66.top

getenv("APP_ENV") ?: "production"
来源：http://xjo.uphjek.com

[U75] PHP：依赖注入
来源：http://iim.feifeiyinyue.top

composer require psr/container
来源：http://qva.cheryme.top

[U76] PHP：简单路由
来源：http://bhc.sjlbkw.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ewt.shangyingyoupin.top

[U77] PHP：模板渲染
来源：http://wqy.c1oappe.top

composer require twig/twig
来源：http://smo.hfpthk.cn

[U78] PHP：单元测试
来源：http://eie.sjlbkw.cn

composer require --dev phpunit/phpunit
来源：http://kyj.ywan-chungtsiang.top

[U79] PHP：静态分析
来源：http://djz.gogol.net.cn

composer require --dev phpstan/phpstan
来源：http://bkw.ehwqpu.com

[U80] PHP：代码规范修复
来源：http://mkn.jiagoushi.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ocn.hfpthk.cn

[U81] JS：初始化项目
来源：http://joc.jinghuilouyu.cn

npm init -y;  npm i express
来源：http://afa.fehbvm.com

[U82] JS：package.json 脚本
来源：http://una.vqdsnc.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zyw.yj20258888.top

[U83] JS：ES Module 导入导出
来源：http://jnu.guowangkeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://gge.yangfankeji.com

[U84] JS：CommonJS 写法
来源：http://pnr.yanxiufei.cn

module.exports = { a };  const { a } = require("./m");
来源：http://sft.cheryme.top

[U85] JS：可选链
来源：http://hte.xylfe.cn

a?.b?.c
来源：http://vhc.vehdjk.com

[U86] JS：空值合并
来源：http://uxo.jinqigfzy.top

a ?? b
来源：http://ryz.hongshengwenyu.top

[U87] JS：解构默认值
来源：http://pzg.feifeiyinyue.top

const { a = 1, b = 2 } = obj;
来源：http://iiz.pycfn.com

[U88] JS：对象展开合并
来源：http://gqw.dianchejie.cn

{ ...a, ...b }
来源：http://psh.hnqzz.top

[U89] JS：数组去重
来源：http://ver.hammf.cn

[...new Set(arr)]
来源：http://zts.fengsongda.top

[U90] JS：数字数组排序
来源：http://jwt.hnqzz.top

[...arr].sort((a, b) => a - b)
来源：http://ozk.yanxiufei.cn

[U91] JS：对象键值遍历
来源：http://hfk.jqgufenzy.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lbm.jiagoushi.top

[U92] JS：深拷贝
来源：http://opx.quarkkingdee.top

structuredClone(obj)
来源：http://fml.cucudq.cn

[U93] JS：模板字符串
来源：http://tyg.ydjk.org.cn

`共 ${n} 条`
来源：http://tcl.sysykeji.top

[U94] JS：箭头函数
来源：http://aqt.hfpthk.cn

const double = x => x * 2;
来源：http://hnf.fktsv.cn

[U95] JS：Promise 包装
来源：http://bzr.uphjek.com

new Promise((resolve, reject) => {})
来源：http://rjt.ehwqpu.com

[U96] JS：async/await 与异常
来源：http://nfa.jinqigfzy.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qyk.9152youxi.cn

[U97] JS：并发请求
来源：http://zzw.xingfuxueyuan.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://mks.meibo888.top

[U98] JS：fetch 带 JSON
来源：http://grx.jqgufenzy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ive.birdmap.top

[U99] JS：事件监听
来源：http://irl.yfazqb.com

el.addEventListener("click", e => {})
来源：http://tfd.yonumen.top

[U100] JS：DOM 查询
来源：http://lvu.c1oappe.top

document.querySelector(".item")
来源：http://mxb.ydjk.org.cn

[U101] JS：classList 操作
来源：http://auj.sysykeji.top

el.classList.toggle("active")
来源：http://uzp.fzhhl.top

[U102] JS：本地存储
来源：http://isp.fanxiaobao.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://gcu.gogol.net.cn

[U103] JS：定时器
来源：http://pme.52xcode.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://aai.jinqigufen.top

[U104] JS：防抖
来源：http://uzp.hcnkem.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sml.ppjwa.cn

[U105] JS：节流
来源：http://zzi.ywan-chungtsiang.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hnm.iojbl.cn

[U106] JS：日期格式化
来源：http://xnn.zhengqikj.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xbl.shanyushiyangkeji.top

[U107] JS：数字千分位
来源：http://xcg.yuxming.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xol.nanxinkj.top

[U108] JS：随机整数
来源：http://dps.jinyuanbaomall.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bby.fengsongda.top

[U109] JS：数组分组
来源：http://pzs.tian-w.cn

Object.groupBy(arr, x => x.type)
来源：http://vcv.nwbrower.top

[U110] JS：数组分块
来源：http://liy.yj202588.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://seu.52xcode.cn

[U111] JS：对象转 Map
来源：http://aqp.smart0.xyz

new Map(Object.entries(obj))
来源：http://msp.sweek.top

[U112] JS：字符串补位
来源：http://uij.cucudq.cn

"7".padStart(3, "0")
来源：http://syp.shanyushiyangkeji.top

[U113] JS：正则替换全部
来源：http://psv.sjlbkw.cn

s.replaceAll("a", "b")
来源：http://ipb.jinqigufen.top

[U114] JS：JSON 深比较
来源：http://mcj.cdnleiting.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://cqn.hfpthk.cn

[U115] JS：生成 UUID
来源：http://mss.jinqigufen.top

crypto.randomUUID()
来源：http://kzl.cashguo.top

[U116] JS：类型检查（JSDoc）
来源：http://qkm.fktsv.cn

/** @param {string} name */ function f(name) {}
来源：http://xli.hongshengwenyu.top

[U117] JS：单元测试
来源：http://dni.zdbjq.cn

npm i -D vitest;  npx vitest
来源：http://njb.smart0.xyz

[U118] JS：开发服务器
来源：http://zzw.shanyushiyangtech.top

npm i -D vite;  npx vite
来源：http://zcs.jiagoushi.top

[U119] JS：生产构建
来源：http://jqf.tian-w.cn

npx vite build
来源：http://mjf.shangyingyoupin.top

[U120] JS：读取环境变量（Vite）
来源：http://qmm.pengpengdd.cyou

import.meta.env.VITE_API_URL
来源：http://dwr.xingfuxueyuan.xyz

================================================================================
来源：http://htu.xuanzx.com

统计汇总
来源：http://ilh.sysykeji.top

================================================================================
来源：http://bno.gzhubu.top

按语言统计（条）：
来源：http://hbr.hnqzz.top

Python ......... 252
来源：http://hfr.hammf.cn

PHP ............ 252
来源：http://uoa.havefunace.top

JavaScript ..... 252
来源：http://ggf.mhx1999.top

TypeScript ..... 212
来源：http://ywn.ybcxt.top

Java ........... 212
来源：http://npr.kuanghao11.cn

Go ............. 212
来源：http://nza.bjfxy.top

Ruby ........... 212
来源：http://gvr.cashguo.top

C# ............. 212
来源：http://ukn.havefunace.top

C .............. 30
来源：http://gkr.fehbvm.com

C++ ............ 30
来源：http://wqz.jqgfzy.top

SQL ............ 90
来源：http://mmp.hammf.cn

Bash ........... 80
来源：http://usl.gaohongyu789.top

Kotlin ......... 15
来源：http://rpt.tianlin.xyz

Swift .......... 15
来源：http://aye.cashguo.top

Lua ............ 10
来源：http://cdd.zhixingplan.top

Perl ........... 10
来源：http://ohu.zhixingplan.top

Scala .......... 10
来源：http://sfu.yongpay.top

------------------------------------
来源：http://rgr.uphjek.com

合计 ........... 2106 条
来源：http://nxl.sweek.top

按章节统计：
来源：http://qhv.quarkkingdee.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yfm.gogol.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mvt.cashguo.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zdd.ivvv.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hze.yongpay.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://pst.hongshengwenyu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gep.jinqigufen.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vsa.c1oappe.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://btd.tarul.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://muc.havefunace.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://spe.shangyingyoupin.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xus.aibaodan.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://apt.jiagoushi.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lor.xziqi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://arh.pengpengdd.cyou

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hbj.daxiang520.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ylw.epnwcf.com

Q SQL 专题                              90
来源：http://owq.vqdsnc.cn

R Bash 专题                             80
来源：http://rbd.shangyingyoupin.top

S C / C++ 专题                          60
来源：http://ytp.bbcook.cn

T 其他语言补充                          60
来源：http://ikh.yuanzhike.top

U 高频实用片段                         120
来源：http://dfk.fehbvm.com

------------------------------------
来源：http://ump.yj20258.top

合计                                  2106 条
来源：http://yoh.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://bqq.andypj.xyz

使用提醒
来源：http://ifw.jiagoushi.top

--------------------------------------------------------------------------------
来源：http://dpn.shanyushiyangtech.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://axh.yanxiufei.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rpq.hesvh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ugo.wangshuangyany.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vfb.vqdsnc.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://akx.nanxinkj.top

—— 文件结束 ——
来源：http://tgq.chenzaomai.com

================================================================================
来源：http://kfa.0kj1m.cn

程序语言常见例子速查手册（2024 版）
来源：http://cth.316326.xyz

Common Programming Examples Cheat Book
来源：http://jei.cdnleiting.top

================================================================================
来源：http://egw.cdnleiting.top

【收录内容】
来源：http://odj.xuanzx.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://ort.zdbjq.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mmp.xuetiantiany.cn

SQL · Bash · C · C++
来源：http://gvt.ivvv.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bcd.vehdjk.com

【使用说明】
来源：http://yvj.jinqigfzy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xub.nanxuanxn.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wwy.haohaochexian.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rhi.bjfxy.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://osd.daria6918.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://nfp.andypj.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://juk.ppjwa.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xee.yvedp.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dyq.jinqigufen.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nxb.jyoumei.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pkx.ydzc1.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://abz.cdnleiting.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://idv.kuanghao11.cn

【文件统计】
来源：http://zqj.zhixingplan.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cxm.yongpay.top

--------------------------------------------------------------------------------
来源：http://xfb.9152youxi.cn

目  录
来源：http://juv.yanxiufei.cn

--------------------------------------------------------------------------------
来源：http://uxb.fanxiaobao.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://clq.zhixingplan.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hke.cqqwz.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rcp.hnqzz.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://iez.shzxlz.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rsv.sysykeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cyq.shzxlz.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://aae.gzhubu.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kjc.jinqigfzy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lte.ywan-chungtsiang.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zdr.bbcook.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ltz.fehbvm.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://urd.jiagoushi.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lma.shangyingyoupin.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zcp.smart0.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://opd.ppjwa.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tvq.xziqi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ylz.yanxiufei.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://eai.havefunace.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wxp.pycfn.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mxq.meibo888.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fyi.hfpthk.cn

================================================================================
来源：http://oim.nwbrower.top

A. 基础语法与类型
来源：http://rdb.ivvv.top

================================================================================
来源：http://ynu.svipenyu.cn

[A01] Hello World
来源：http://byc.nanxinkj.top

Py:   print("Hello, World!")
来源：http://kdo.yonumen.top

PHP:  echo "Hello, World!";
来源：http://ayi.yj202588.top

JS:   console.log("Hello, World!");
来源：http://umh.ivvv.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bar.316326.xyz

Java: System.out.println("Hello, World!");
来源：http://gyn.xingfuxueyuan.xyz

Go:   fmt.Println("Hello, World!")
来源：http://vtf.shanyushiyangtech.top

Ruby: puts "Hello, World!"
来源：http://exi.yangfankeji.com

C#:   Console.WriteLine("Hello, World!");
来源：http://heh.fengsongda.top

[A02] 变量声明与赋值
来源：http://sei.shanyushiyangtech.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ekf.hnqzz.top

PHP:  $name = "Alex"; $age = 20;
来源：http://fzj.xuetiantiany.cn

JS:   let name = "Alex"; const age = 20;
来源：http://occ.yueranfly.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://uar.jyoumei.cn

Java: String name = "Alex"; int age = 20;
来源：http://cwr.guowangkeji.top

Go:   name := "Alex"; age := 20
来源：http://ngj.hnxiangtu.top

Ruby: name = "Alex"; age = 20
来源：http://cvl.shuidangran.top


<!-- 参考信息 -->