代发 wailian999

[U33] Py：打包发布
来源：http://rji.yanxiufei.cn

python -m build  （依赖 pyproject.toml）
来源：http://smm.yanxiufei.cn

[U34] Py：判断编码
来源：http://rfc.xylfe.cn

chardet.detect(raw)
来源：http://lrn.gzhubu.top

[U35] Py：发送邮件
来源：http://grl.zhixingplan.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rzi.shangyingyoupin.top

[U36] Py：定时任务
来源：http://ktd.xziqi.cn

schedule.every(10).minutes.do(job)
来源：http://grj.feifeiyinyue.top

[U37] Py：读写 Excel
来源：http://nxv.guannengcc.top

pandas.read_excel / DataFrame.to_excel
来源：http://uxp.pycfn.com

[U38] Py：获取脚本所在目录
来源：http://tnz.sxryk.cn

Path(__file__).resolve().parent
来源：http://bbf.ywan-chungtsiang.top

[U39] Py：判断是否在交互环境
来源：http://kec.feifeiyinyue.top

sys.stdout.isatty()
来源：http://bzm.gotoacloud.top

[U40] Py：打印到标准错误
来源：http://ahr.9152youxi.cn

print("err", file=sys.stderr)
来源：http://bbh.shanyushiyangkeji.top

[U41] PHP：初始化 Composer 项目
来源：http://iki.pycfn.com

composer init;  composer require guzzlehttp/guzzle
来源：http://hfn.9152youxi.cn

[U42] PHP：PSR-4 自动加载
来源：http://ixm.bbcook.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://iau.jqgfzy.top

[U43] PHP：声明命名空间
来源：http://xmc.xingfuxueyuan.xyz

namespace App\Http;
来源：http://lkd.9152youxi.cn

[U44] PHP：开启严格类型
来源：http://hol.sweek.top

declare(strict_types=1);
来源：http://iyu.xuetiantiany.cn

[U45] PHP：类型声明与返回类型
来源：http://kmx.aibaodan.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yub.chenzaomai.com

[U46] PHP：可空类型
来源：http://fjh.ywan-chungtsiang.top

?string $name = null
来源：http://axb.ehwqpu.com

[U47] PHP：联合类型
来源：http://bfq.yangfankeji.com

int|string $id
来源：http://vgn.jinqigufen.top

[U48] PHP：纯枚举
来源：http://twf.havefunace.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gnp.pycfn.com

[U49] PHP：只读属性
来源：http://mmo.yvedp.cn

public readonly string $name
来源：http://cem.xuanzx.com

[U50] PHP：构造器属性提升
来源：http://lsh.ywan-chungtsiang.top

public function __construct(private int $id) {}
来源：http://mlc.pycfn.com

[U51] PHP：数组解构
来源：http://vyt.bjfxy.top

[$a, $b] = $arr;
来源：http://zqw.snrcjt.cn

[U52] PHP：箭头函数
来源：http://wmj.aizwys.cn

$double = fn($x) => $x * 2;
来源：http://ese.bjfxy.top

[U53] PHP：空合并运算符
来源：http://llq.wangshuangyany.cn

$v = $a ?? $b ?? "default";
来源：http://spo.hnxiangtu.top

[U54] PHP：空安全调用
来源：http://roh.hfpthk.cn

$obj?->method()
来源：http://yzg.ybcxt.top

[U55] PHP：match 表达式
来源：http://cij.pycfn.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://kll.jlsjyb.cn

[U56] PHP：命名参数
来源：http://mxj.c1oappe.top

f(a: 1, b: 2)
来源：http://lfh.zhixingplan.top

[U57] PHP：字符串插值
来源：http://kgw.uphjek.com

"值: {$a}"
来源：http://xyd.redwolf501.top

[U58] PHP：数组三件套
来源：http://ndu.52xcode.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lbh.yonumen.top

[U59] PHP：自定义排序
来源：http://bua.hongshengwenyu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xbc.jqgufenzy.top

[U60] PHP：JSON 编解码
来源：http://hfu.fengsongda.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://iya.9152youxi.cn

[U61] PHP：正则
来源：http://xsa.gaohongyu789.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jhm.fanxiaobao.xyz

[U62] PHP：日期对象
来源：http://dac.quarkkingdee.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wxj.gzhubu.top

[U63] PHP：文件读写
来源：http://feg.shanyushiyangtech.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dwd.guannengcc.top

[U64] PHP：目录遍历
来源：http://kpu.gogol.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://wbv.epnwcf.com

[U65] PHP：会话
来源：http://dgz.shanyushiyangtech.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ijf.ppjwa.cn

[U66] PHP：设置 Cookie
来源：http://irz.guannengcc.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://odx.zhengqikj.top

[U67] PHP：处理文件上传
来源：http://kqi.fktsv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ypx.wangdashe.top

[U68] PHP：PDO 连接
来源：http://idv.cheryme.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://awf.gaohongyu789.top

[U69] PHP：PDO 预处理
来源：http://bsp.hongshengwenyu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ymc.tanke756.top

[U70] PHP：PDO 事务
来源：http://kln.hnqzz.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qwp.zhaomingkeji.xyz

[U71] PHP：抛出异常
来源：http://lir.yfazqb.com

throw new RuntimeException("失败", 500);
来源：http://jjq.jiagoushi.top

[U72] PHP：写错误日志
来源：http://hbo.52xcode.cn

error_log("失败: " . $e->getMessage());
来源：http://ivo.smart0.xyz

[U73] PHP：读取 ini 配置
来源：http://hia.jinqigfzy.top

parse_ini_file("config.ini", true)
来源：http://tbo.jinghuilouyu.cn

[U74] PHP：读取环境变量
来源：http://itv.yueranfly.top

getenv("APP_ENV") ?: "production"
来源：http://cqp.xziqi.cn

[U75] PHP：依赖注入
来源：http://ame.yueranfly.top

composer require psr/container
来源：http://buj.gotoacloud.top

[U76] PHP：简单路由
来源：http://ytl.gaohongyu789.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gay.zycfv.cn

[U77] PHP：模板渲染
来源：http://nuz.jqgfzy.top

composer require twig/twig
来源：http://frj.tianlin.xyz

[U78] PHP：单元测试
来源：http://kia.tarul.cn

composer require --dev phpunit/phpunit
来源：http://tbu.ydjk.org.cn

[U79] PHP：静态分析
来源：http://kgd.tianlin.xyz

composer require --dev phpstan/phpstan
来源：http://shb.yueranfly.top

[U80] PHP：代码规范修复
来源：http://pke.yj20258.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://zrt.xziqi.cn

[U81] JS：初始化项目
来源：http://cqa.nanxinkj.top

npm init -y;  npm i express
来源：http://wym.zycfv.cn

[U82] JS：package.json 脚本
来源：http://zmn.hcnkem.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://prg.kuanghao11.cn

[U83] JS：ES Module 导入导出
来源：http://lvp.chenjidiqi.icu

export const a = 1;  import { a } from "./m.js";
来源：http://ruq.gaohongyu789.top

[U84] JS：CommonJS 写法
来源：http://few.fehbvm.com

module.exports = { a };  const { a } = require("./m");
来源：http://txr.aibaodan.cn

[U85] JS：可选链
来源：http://nov.shanyushiyangkeji.top

a?.b?.c
来源：http://mdc.gogol.net.cn

[U86] JS：空值合并
来源：http://axb.c1oappe.top

a ?? b
来源：http://fle.hywenlv.cn

[U87] JS：解构默认值
来源：http://smv.birdmap.top

const { a = 1, b = 2 } = obj;
来源：http://fqk.cqqwz.cn

[U88] JS：对象展开合并
来源：http://hxf.jinghuilouyu.cn

{ ...a, ...b }
来源：http://iod.yj20258888.top

[U89] JS：数组去重
来源：http://wae.zycfv.cn

[...new Set(arr)]
来源：http://sne.sjlbkw.cn

[U90] JS：数字数组排序
来源：http://jmu.yueranfly.top

[...arr].sort((a, b) => a - b)
来源：http://isy.wangshuangyany.cn

[U91] JS：对象键值遍历
来源：http://rdv.uphjek.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tmf.svipenyu.cn

[U92] JS：深拷贝
来源：http://glr.dianchejie.cn

structuredClone(obj)
来源：http://bbv.chenjidiqi.icu

[U93] JS：模板字符串
来源：http://izc.vqdsnc.cn

`共 ${n} 条`
来源：http://lpl.zycfv.cn

[U94] JS：箭头函数
来源：http://xcm.jinghuilouyu.cn

const double = x => x * 2;
来源：http://dqa.zhiwuduotai.top

[U95] JS：Promise 包装
来源：http://moe.bjfxy.top

new Promise((resolve, reject) => {})
来源：http://vgs.cucudq.cn

[U96] JS：async/await 与异常
来源：http://rvd.hnqzz.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vmu.yongpay.top

[U97] JS：并发请求
来源：http://fff.jiagoushi.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://elj.zhengqikj.top

[U98] JS：fetch 带 JSON
来源：http://uyg.zhengqikj.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://okk.guowangkeji.top

[U99] JS：事件监听
来源：http://dte.xuanzx.com

el.addEventListener("click", e => {})
来源：http://apl.yueranfly.top

[U100] JS：DOM 查询
来源：http://onz.wangshuangyany.cn

document.querySelector(".item")
来源：http://fpz.dashuyun.cn

[U101] JS：classList 操作
来源：http://jrr.jlsjyb.cn

el.classList.toggle("active")
来源：http://psj.zhijiandao.cn

[U102] JS：本地存储
来源：http://xnf.shzxlz.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rjc.meibo888.top

[U103] JS：定时器
来源：http://ixi.hnqzz.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lrc.c1oappe.top

[U104] JS：防抖
来源：http://vvw.zhaomingkeji.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eth.xylfe.cn

[U105] JS：节流
来源：http://vjx.yonumen.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://neo.nanxuanxn.top

[U106] JS：日期格式化
来源：http://htx.yonumen.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gmi.zhiwuduotai.top

[U107] JS：数字千分位
来源：http://inq.9152youxi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uqk.wangdashe.top

[U108] JS：随机整数
来源：http://xjx.xuanzx.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wwq.chenjidiqi.icu

[U109] JS：数组分组
来源：http://dii.dashuyun.cn

Object.groupBy(arr, x => x.type)
来源：http://rnp.cashguo.top

[U110] JS：数组分块
来源：http://jvf.quarkkingdee.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rof.yj202588.top

[U111] JS：对象转 Map
来源：http://qbc.yonumen.top

new Map(Object.entries(obj))
来源：http://bnp.haohaochexian.top

[U112] JS：字符串补位
来源：http://wlx.cqqwz.cn

"7".padStart(3, "0")
来源：http://gwg.52xcode.cn

[U113] JS：正则替换全部
来源：http://zso.yfazqb.com

s.replaceAll("a", "b")
来源：http://xbu.sjlbkw.cn

[U114] JS：JSON 深比较
来源：http://ugl.zhaomingkeji.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://vcu.chenjidiqi.icu

[U115] JS：生成 UUID
来源：http://szt.hesvh.cn

crypto.randomUUID()
来源：http://jba.xziqi.cn

[U116] JS：类型检查（JSDoc）
来源：http://nen.ivvv.top

/** @param {string} name */ function f(name) {}
来源：http://jzv.hcnkem.com

[U117] JS：单元测试
来源：http://bxe.sysykeji.top

npm i -D vitest;  npx vitest
来源：http://kub.nanxuanxn.top

[U118] JS：开发服务器
来源：http://rul.jianghu66.top

npm i -D vite;  npx vite
来源：http://koj.52xcode.cn

[U119] JS：生产构建
来源：http://eog.ehwqpu.com

npx vite build
来源：http://qdx.0kj1m.cn

[U120] JS：读取环境变量（Vite）
来源：http://jni.cdnleiting.top

import.meta.env.VITE_API_URL
来源：http://nak.zhixingplan.top

================================================================================
来源：http://bbo.hcnkem.com

统计汇总
来源：http://vfv.mhx1999.top

================================================================================
来源：http://zdx.wangshuangyany.cn

按语言统计（条）：
来源：http://fio.chenjidiqi.icu

Python ......... 252
来源：http://dfw.cqqwz.cn

PHP ............ 252
来源：http://yhm.zhiwuduotai.top

JavaScript ..... 252
来源：http://rvb.aizwys.cn

TypeScript ..... 212
来源：http://ekg.havefunace.top

Java ........... 212
来源：http://ijl.zdqjudy.top

Go ............. 212
来源：http://lmr.jqgufenzy.top

Ruby ........... 212
来源：http://mos.sysykeji.top

C# ............. 212
来源：http://kaz.jinyuanbaomall.cn

C .............. 30
来源：http://cdj.52xcode.cn

C++ ............ 30
来源：http://xxd.cqqwz.cn

SQL ............ 90
来源：http://fji.feifeiyinyue.top

Bash ........... 80
来源：http://xrf.andypj.xyz

Kotlin ......... 15
来源：http://enf.sweek.top

Swift .......... 15
来源：http://kvh.fktsv.cn

Lua ............ 10
来源：http://ltn.pengpengdd.cyou

Perl ........... 10
来源：http://jfg.sufxvd.cn

Scala .......... 10
来源：http://nvf.jinqigfzy.top

------------------------------------
来源：http://ysf.gogol.net.cn

合计 ........... 2106 条
来源：http://osu.hnqzz.top

按章节统计：
来源：http://zvo.havefunace.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dof.kuanghao11.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hkz.birdmap.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mqr.haohaochexian.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hxu.pycfn.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://peu.quarkkingdee.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ngb.mhx1999.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mse.hywenlv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jwi.sufxvd.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://owv.tarul.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kvj.birdmap.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dcj.yvedp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zhc.shangyingyoupin.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://obv.nwbrower.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uaz.chenlongwang.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dvn.xziqi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wyw.jiagoushi.top

Q SQL 专题                              90
来源：http://haj.chenlongwang.top

R Bash 专题                             80
来源：http://kkw.yj20258888.top

S C / C++ 专题                          60
来源：http://qcm.ppjwa.cn

T 其他语言补充                          60
来源：http://vfi.fanxiaobao.xyz

U 高频实用片段                         120
来源：http://lhc.jqgfzy.top

------------------------------------
来源：http://tzp.shanyushiyangkeji.top

合计                                  2106 条
来源：http://vrq.ybcxt.top

--------------------------------------------------------------------------------
来源：http://cna.ybcxt.top

使用提醒
来源：http://ygf.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://udf.zhengqikj.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tdh.gaohongyu789.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://crh.quarkkingdee.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lwd.yangfankeji.com

在旧版本上使用前请先确认语法支持情况。
来源：http://vir.yvedp.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lel.quarkkingdee.top

—— 文件结束 ——
来源：http://syb.tarul.cn

================================================================================
来源：http://wyz.daxiang520.top

程序语言常见例子速查手册（2024 版）
来源：http://mnh.hammf.cn

Common Programming Examples Cheat Book
来源：http://vde.guannengcc.top

================================================================================
来源：http://mtw.yj20258888.top

【收录内容】
来源：http://wgy.yueranfly.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://enp.svipenyu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xmx.cqqwz.cn

SQL · Bash · C · C++
来源：http://srt.0kj1m.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lfq.jlsjyb.cn

【使用说明】
来源：http://qpu.nanxinkj.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pdb.kuanghao11.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rhk.tianlin.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zzr.hammf.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://svr.gzhubu.top

Bash:  Shell         C:     C             C++:   C++
来源：http://nbg.iojbl.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vjp.0kj1m.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://sgf.aibaodan.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yae.nanxuanxn.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cbx.zhoulong.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xep.snrcjt.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://swf.fengsongda.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kdh.daxiang520.top

【文件统计】
来源：http://edg.svipenyu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lim.tarul.cn

--------------------------------------------------------------------------------
来源：http://xfe.xingfuxueyuan.xyz

目  录
来源：http://opv.meibo888.top

--------------------------------------------------------------------------------
来源：http://erv.hnxiangtu.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uid.nwbrower.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cmg.shangyingyoupin.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tbu.hammf.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tbi.zhongyouzk.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qlx.epnwcf.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sqh.pycfn.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qyb.havefunace.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ggg.xingfuxueyuan.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xoh.9152youxi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://don.zhiwuduotai.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gaf.snrcjt.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hpb.c1oappe.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kow.wangshuangyany.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fdq.9152youxi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xic.yj202588.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wax.xuetiantiany.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ysn.cashguo.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://hjk.jinyuanbaomall.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pfj.zdqjudy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://alu.jyoumei.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wqj.yueranfly.top

================================================================================
来源：http://rkm.xziqi.cn

A. 基础语法与类型
来源：http://dut.zhaomingkeji.xyz

================================================================================
来源：http://alj.guannengcc.top

[A01] Hello World
来源：http://abq.zhaomingkeji.xyz

Py:   print("Hello, World!")
来源：http://eqp.xuetiantiany.cn

PHP:  echo "Hello, World!";
来源：http://mda.bjfxy.top

JS:   console.log("Hello, World!");
来源：http://wnt.guowangkeji.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://aob.jqgfzy.top

Java: System.out.println("Hello, World!");
来源：http://the.yj20258.top

Go:   fmt.Println("Hello, World!")
来源：http://ybn.pycfn.com

Ruby: puts "Hello, World!"
来源：http://fsa.jinyuanbaomall.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://bew.xylfe.cn

[A02] 变量声明与赋值
来源：http://fsz.zdqjudy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yat.snrcjt.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://evt.316326.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://wht.smart0.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nid.shangyingyoupin.top

Java: String name = "Alex"; int age = 20;
来源：http://wqx.iojbl.cn

Go:   name := "Alex"; age := 20
来源：http://gsd.fzhhl.top

Ruby: name = "Alex"; age = 20
来源：http://bos.yuanzhike.top


<!-- 参考信息 -->