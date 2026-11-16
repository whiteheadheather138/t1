代发 wailian999

[U31] Py：单测
来源：http://arh.chenzaomai.com

python -m pytest -q
来源：http://ahn.meibo888.top

[U32] Py：代码格式化
来源：http://lse.shuidangran.top

ruff format . && ruff check --fix .
来源：http://hjm.jinqigufen.top

[U33] Py：打包发布
来源：http://uuq.redwolf501.top

python -m build  （依赖 pyproject.toml）
来源：http://lei.ywan-chungtsiang.top

[U34] Py：判断编码
来源：http://bfb.yj20258888.top

chardet.detect(raw)
来源：http://iaj.hywenlv.cn

[U35] Py：发送邮件
来源：http://cma.xinyue.icu

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://csl.shanyushiyangtech.top

[U36] Py：定时任务
来源：http://cio.shuidangran.top

schedule.every(10).minutes.do(job)
来源：http://tec.jqgfzy.top

[U37] Py：读写 Excel
来源：http://kdr.gotoacloud.top

pandas.read_excel / DataFrame.to_excel
来源：http://mya.jinqigfzy.top

[U38] Py：获取脚本所在目录
来源：http://mle.uphjek.com

Path(__file__).resolve().parent
来源：http://rdu.nanxinkj.top

[U39] Py：判断是否在交互环境
来源：http://gmx.ivvv.top

sys.stdout.isatty()
来源：http://jkv.jinqigufen.top

[U40] Py：打印到标准错误
来源：http://mbi.hywenlv.cn

print("err", file=sys.stderr)
来源：http://ihy.jinqigufen.top

[U41] PHP：初始化 Composer 项目
来源：http://lyq.ywan-chungtsiang.top

composer init;  composer require guzzlehttp/guzzle
来源：http://pqf.jlsjyb.cn

[U42] PHP：PSR-4 自动加载
来源：http://yee.daria6918.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://pyy.yonumen.top

[U43] PHP：声明命名空间
来源：http://eeo.shanyushiyangkeji.top

namespace App\Http;
来源：http://qme.hammf.cn

[U44] PHP：开启严格类型
来源：http://fex.shzxlz.cn

declare(strict_types=1);
来源：http://fuw.sysykeji.top

[U45] PHP：类型声明与返回类型
来源：http://gve.jyoumei.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://snj.jinqigufen.top

[U46] PHP：可空类型
来源：http://mdo.316326.xyz

?string $name = null
来源：http://bza.cheryme.top

[U47] PHP：联合类型
来源：http://eeh.tianlin.xyz

int|string $id
来源：http://man.jiagoushi.top

[U48] PHP：纯枚举
来源：http://erp.sysykeji.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bto.cucudq.cn

[U49] PHP：只读属性
来源：http://vvh.c1oappe.top

public readonly string $name
来源：http://oac.52xcode.cn

[U50] PHP：构造器属性提升
来源：http://vbz.svipenyu.cn

public function __construct(private int $id) {}
来源：http://hwo.wangdashe.top

[U51] PHP：数组解构
来源：http://dqj.cashguo.top

[$a, $b] = $arr;
来源：http://uco.sufxvd.cn

[U52] PHP：箭头函数
来源：http://zov.svipenyu.cn

$double = fn($x) => $x * 2;
来源：http://biq.sweek.top

[U53] PHP：空合并运算符
来源：http://cii.hywenlv.cn

$v = $a ?? $b ?? "default";
来源：http://dzp.yj20258888.top

[U54] PHP：空安全调用
来源：http://rmm.xuetiantiany.cn

$obj?->method()
来源：http://kyw.jinyuanbaomall.cn

[U55] PHP：match 表达式
来源：http://sda.svipenyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zeo.andypj.xyz

[U56] PHP：命名参数
来源：http://ehs.sweek.top

f(a: 1, b: 2)
来源：http://wdv.jinqigufen.top

[U57] PHP：字符串插值
来源：http://gzp.fehbvm.com

"值: {$a}"
来源：http://urd.c1oappe.top

[U58] PHP：数组三件套
来源：http://uqp.jinghuilouyu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://bzy.shangyingyoupin.top

[U59] PHP：自定义排序
来源：http://nmk.gaohongyu789.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qjm.redwolf501.top

[U60] PHP：JSON 编解码
来源：http://prm.shangyingyoupin.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://drq.yj202588.top

[U61] PHP：正则
来源：http://koo.ivvv.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pwh.gotoacloud.top

[U62] PHP：日期对象
来源：http://aaf.9152youxi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bhw.guannengcc.top

[U63] PHP：文件读写
来源：http://wmy.smart0.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hls.jqgufenzy.top

[U64] PHP：目录遍历
来源：http://afg.shanyushiyangtech.top

glob("dir/*.php");  scandir("dir");
来源：http://oyq.tianlin.xyz

[U65] PHP：会话
来源：http://kto.jyoumei.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fie.redwolf501.top

[U66] PHP：设置 Cookie
来源：http://koz.yueranfly.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hld.hcnkem.com

[U67] PHP：处理文件上传
来源：http://dyb.zhengqikj.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uhs.zdqjudy.top

[U68] PHP：PDO 连接
来源：http://mox.yueranfly.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://set.jianghu66.top

[U69] PHP：PDO 预处理
来源：http://lkr.yanxiufei.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ekw.ehwqpu.com

[U70] PHP：PDO 事务
来源：http://diu.mhx1999.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ppx.fengsongda.top

[U71] PHP：抛出异常
来源：http://opj.shangyingyoupin.top

throw new RuntimeException("失败", 500);
来源：http://gnu.shangyingyoupin.top

[U72] PHP：写错误日志
来源：http://xyd.fengsongda.top

error_log("失败: " . $e->getMessage());
来源：http://zlk.jlsjyb.cn

[U73] PHP：读取 ini 配置
来源：http://flu.sjlbkw.cn

parse_ini_file("config.ini", true)
来源：http://rfk.andypj.xyz

[U74] PHP：读取环境变量
来源：http://pej.tian-w.cn

getenv("APP_ENV") ?: "production"
来源：http://myy.yongpay.top

[U75] PHP：依赖注入
来源：http://ecf.vqdsnc.cn

composer require psr/container
来源：http://ipd.aibaodan.cn

[U76] PHP：简单路由
来源：http://rss.hnxiangtu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mqg.wangdashe.top

[U77] PHP：模板渲染
来源：http://qjs.yuxming.cn

composer require twig/twig
来源：http://ljc.nwbrower.top

[U78] PHP：单元测试
来源：http://etw.dianchejie.cn

composer require --dev phpunit/phpunit
来源：http://bqq.nwbrower.top

[U79] PHP：静态分析
来源：http://irl.zhongyouzk.top

composer require --dev phpstan/phpstan
来源：http://ezb.quarkkingdee.top

[U80] PHP：代码规范修复
来源：http://pch.jinghuilouyu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xmm.redwolf501.top

[U81] JS：初始化项目
来源：http://joi.zhijiandao.cn

npm init -y;  npm i express
来源：http://ycx.zhengqikj.top

[U82] JS：package.json 脚本
来源：http://rem.chenlongwang.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://tbe.yangfankeji.com

[U83] JS：ES Module 导入导出
来源：http://jqs.yanxiufei.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rmt.tianlin.xyz

[U84] JS：CommonJS 写法
来源：http://mup.yangfankeji.com

module.exports = { a };  const { a } = require("./m");
来源：http://pet.zhengqikj.top

[U85] JS：可选链
来源：http://zvu.daxiang520.top

a?.b?.c
来源：http://qae.aizwys.cn

[U86] JS：空值合并
来源：http://jhk.fehbvm.com

a ?? b
来源：http://yhf.fanxiaobao.xyz

[U87] JS：解构默认值
来源：http://ugq.andypj.xyz

const { a = 1, b = 2 } = obj;
来源：http://fdh.jlsjyb.cn

[U88] JS：对象展开合并
来源：http://vbv.52xcode.cn

{ ...a, ...b }
来源：http://uzd.yuanzhike.top

[U89] JS：数组去重
来源：http://xrd.bjfxy.top

[...new Set(arr)]
来源：http://eds.zhijiandao.cn

[U90] JS：数字数组排序
来源：http://mgy.jqgfzy.top

[...arr].sort((a, b) => a - b)
来源：http://kjl.tanke756.top

[U91] JS：对象键值遍历
来源：http://hpa.zhaomingkeji.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zka.sweek.top

[U92] JS：深拷贝
来源：http://ffg.hammf.cn

structuredClone(obj)
来源：http://upm.dashuyun.cn

[U93] JS：模板字符串
来源：http://jwi.shangyingyoupin.top

`共 ${n} 条`
来源：http://kft.sjlbkw.cn

[U94] JS：箭头函数
来源：http://fue.jiagoushi.top

const double = x => x * 2;
来源：http://wuy.daxiang520.top

[U95] JS：Promise 包装
来源：http://wrd.guannengcc.top

new Promise((resolve, reject) => {})
来源：http://twv.sufxvd.cn

[U96] JS：async/await 与异常
来源：http://vvz.xylfe.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ihs.shuidangran.top

[U97] JS：并发请求
来源：http://xye.wangshuangyany.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lev.nanxinkj.top

[U98] JS：fetch 带 JSON
来源：http://roz.aizwys.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zgz.xylfe.cn

[U99] JS：事件监听
来源：http://xra.yonumen.top

el.addEventListener("click", e => {})
来源：http://lkd.ydjk.org.cn

[U100] JS：DOM 查询
来源：http://krx.fengsongda.top

document.querySelector(".item")
来源：http://tnw.yueranfly.top

[U101] JS：classList 操作
来源：http://abp.feifeiyinyue.top

el.classList.toggle("active")
来源：http://qnr.aibaodan.cn

[U102] JS：本地存储
来源：http://oma.jyoumei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kmk.ydjk.org.cn

[U103] JS：定时器
来源：http://lvn.sjlbkw.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rfp.shanyushiyangkeji.top

[U104] JS：防抖
来源：http://ajk.xylfe.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xbw.sweek.top

[U105] JS：节流
来源：http://krg.chenjidiqi.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nza.cdnleiting.top

[U106] JS：日期格式化
来源：http://gdt.0kj1m.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xxk.wangshuangyany.cn

[U107] JS：数字千分位
来源：http://owt.shuidangran.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://udm.shanyushiyangkeji.top

[U108] JS：随机整数
来源：http://wsq.yfazqb.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://erq.hesvh.cn

[U109] JS：数组分组
来源：http://tkr.yj20258.top

Object.groupBy(arr, x => x.type)
来源：http://xyj.vqdsnc.cn

[U110] JS：数组分块
来源：http://cdi.jinghuilouyu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://thn.jqgufenzy.top

[U111] JS：对象转 Map
来源：http://mca.zhongyouzk.top

new Map(Object.entries(obj))
来源：http://awa.redwolf501.top

[U112] JS：字符串补位
来源：http://ojg.kuanghao11.cn

"7".padStart(3, "0")
来源：http://jyt.ywan-chungtsiang.top

[U113] JS：正则替换全部
来源：http://ktk.c1oappe.top

s.replaceAll("a", "b")
来源：http://pry.gotoacloud.top

[U114] JS：JSON 深比较
来源：http://tud.xuanzx.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://mfz.bjfxy.top

[U115] JS：生成 UUID
来源：http://qqq.vehdjk.com

crypto.randomUUID()
来源：http://xrv.dianchejie.cn

[U116] JS：类型检查（JSDoc）
来源：http://hdl.sweek.top

/** @param {string} name */ function f(name) {}
来源：http://lut.feifeiyinyue.top

[U117] JS：单元测试
来源：http://pxr.cheryme.top

npm i -D vitest;  npx vitest
来源：http://zcp.xuanzx.com

[U118] JS：开发服务器
来源：http://mbc.zhixingplan.top

npm i -D vite;  npx vite
来源：http://zfy.chenlongwang.top

[U119] JS：生产构建
来源：http://dis.hfpthk.cn

npx vite build
来源：http://cwz.aibaodan.cn

[U120] JS：读取环境变量（Vite）
来源：http://miw.aibaodan.cn

import.meta.env.VITE_API_URL
来源：http://trr.sysykeji.top

================================================================================
来源：http://pue.tianlin.xyz

统计汇总
来源：http://rul.jiagoushi.top

================================================================================
来源：http://jls.gogol.net.cn

按语言统计（条）：
来源：http://zek.fanxiaobao.xyz

Python ......... 252
来源：http://drv.zdbjq.cn

PHP ............ 252
来源：http://lwe.cheryme.top

JavaScript ..... 252
来源：http://hyc.quarkkingdee.top

TypeScript ..... 212
来源：http://jke.iojbl.cn

Java ........... 212
来源：http://ziz.yfazqb.com

Go ............. 212
来源：http://sxp.shanyushiyangtech.top

Ruby ........... 212
来源：http://iwt.cashguo.top

C# ............. 212
来源：http://nbn.zdbjq.cn

C .............. 30
来源：http://gct.uphjek.com

C++ ............ 30
来源：http://gmf.yongpay.top

SQL ............ 90
来源：http://eot.yj20258888.top

Bash ........... 80
来源：http://ema.xingfuxueyuan.xyz

Kotlin ......... 15
来源：http://trm.bjfxy.top

Swift .......... 15
来源：http://bhn.xinyue.icu

Lua ............ 10
来源：http://nho.xylfe.cn

Perl ........... 10
来源：http://uxi.hammf.cn

Scala .......... 10
来源：http://nol.yanxiufei.cn

------------------------------------
来源：http://zix.svipenyu.cn

合计 ........... 2106 条
来源：http://ykk.c1oappe.top

按章节统计：
来源：http://reo.dianchejie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://knk.0kj1m.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bho.yfazqb.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zea.hysaishi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sio.yanxiufei.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dvn.haohaochexian.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xwl.epnwcf.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lzp.cqqwz.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dbn.daxiang520.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://kff.fzhhl.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pgg.andypj.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kzy.ydjk.org.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mae.yj20258888.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fmi.yj20258.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hko.316326.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fmi.gaohongyu789.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ycx.gotoacloud.top

Q SQL 专题                              90
来源：http://ghe.guannengcc.top

R Bash 专题                             80
来源：http://oze.wangdashe.top

S C / C++ 专题                          60
来源：http://qqu.shzxlz.cn

T 其他语言补充                          60
来源：http://wig.redwolf501.top

U 高频实用片段                         120
来源：http://zew.ppjwa.cn

------------------------------------
来源：http://tbt.9152youxi.cn

合计                                  2106 条
来源：http://anj.bbcook.cn

--------------------------------------------------------------------------------
来源：http://inu.hywenlv.cn

使用提醒
来源：http://tej.bbcook.cn

--------------------------------------------------------------------------------
来源：http://uqv.cdnleiting.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zjo.shanyushiyangkeji.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gzg.c1oappe.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xbh.daria6918.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://oef.zhiwuduotai.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lxj.jiagoushi.top

—— 文件结束 ——
来源：http://iqs.hnqzz.top

================================================================================
来源：http://lkl.birdmap.top

程序语言常见例子速查手册（2024 版）
来源：http://igx.daria6918.cn

Common Programming Examples Cheat Book
来源：http://ous.sxryk.cn

================================================================================
来源：http://kem.zhixingplan.top

【收录内容】
来源：http://doy.ydzc1.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://llf.yonumen.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://iph.zhaomingkeji.xyz

SQL · Bash · C · C++
来源：http://hbt.xylfe.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dgt.zhoulong.xyz

【使用说明】
来源：http://mgl.dashuyun.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kjj.yangfankeji.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ytz.jqgufenzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://myr.vehdjk.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nay.cashguo.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ors.shangyingyoupin.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kck.sjlbkw.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fmg.nwbrower.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dgt.meibo888.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jvl.aibaodan.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gdw.52xcode.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gdi.shzxlz.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gnm.yvedp.cn

【文件统计】
来源：http://cwc.meibo888.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zsr.bjfxy.top

--------------------------------------------------------------------------------
来源：http://pnr.gotoacloud.top

目  录
来源：http://mmf.ydzc1.top

--------------------------------------------------------------------------------
来源：http://xsn.wangdashe.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dky.gotoacloud.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hgs.hcnkem.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://igo.shuidangran.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ykw.sjlbkw.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qln.jinghuilouyu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gwm.tarul.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mvu.tian-w.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dos.pengpengdd.cyou

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jfg.bbcook.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zla.chenlongwang.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hcc.guannengcc.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hec.jlsjyb.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://skl.jinghuilouyu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pvz.yuxming.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qml.chenzaomai.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zjx.sufxvd.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vax.guowangkeji.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://tme.aibaodan.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dze.sweek.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uyl.bjfxy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://nat.sysykeji.top

================================================================================
来源：http://atb.shuidangran.top

A. 基础语法与类型
来源：http://cmn.ydzc1.top

================================================================================
来源：http://adp.yuxming.cn

[A01] Hello World
来源：http://wcc.ybcxt.top

Py:   print("Hello, World!")
来源：http://mkj.sjlbkw.cn

PHP:  echo "Hello, World!";
来源：http://utg.jyoumei.cn

JS:   console.log("Hello, World!");
来源：http://rva.ehwqpu.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://etj.zhaomingkeji.xyz

Java: System.out.println("Hello, World!");
来源：http://vnm.havefunace.top

Go:   fmt.Println("Hello, World!")
来源：http://eny.hysaishi.cn

Ruby: puts "Hello, World!"
来源：http://tpj.uphjek.com

C#:   Console.WriteLine("Hello, World!");
来源：http://djl.pycfn.com

[A02] 变量声明与赋值
来源：http://owb.hysaishi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://iqk.xuetiantiany.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://uzr.dashuyun.cn

JS:   let name = "Alex"; const age = 20;
来源：http://jkv.yuxming.cn


<!-- 参考信息 -->