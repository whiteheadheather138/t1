代发 wailian999

[U31] Py：单测
来源：http://prt.daria6918.cn

python -m pytest -q
来源：http://jji.chenzaomai.com

[U32] Py：代码格式化
来源：http://xtk.ydjk.org.cn

ruff format . && ruff check --fix .
来源：http://gtm.cdnleiting.top

[U33] Py：打包发布
来源：http://zrk.guowangkeji.top

python -m build  （依赖 pyproject.toml）
来源：http://lxt.xuanzx.com

[U34] Py：判断编码
来源：http://bxz.shanyushiyangkeji.top

chardet.detect(raw)
来源：http://rlh.hysaishi.cn

[U35] Py：发送邮件
来源：http://rpw.hfpthk.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mqb.pengpengdd.cyou

[U36] Py：定时任务
来源：http://dln.jyoumei.cn

schedule.every(10).minutes.do(job)
来源：http://iso.yj20258888.top

[U37] Py：读写 Excel
来源：http://owm.hesvh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://krf.sjlbkw.cn

[U38] Py：获取脚本所在目录
来源：http://gmy.aibaodan.cn

Path(__file__).resolve().parent
来源：http://qcv.shanyushiyangtech.top

[U39] Py：判断是否在交互环境
来源：http://soe.zhoulong.xyz

sys.stdout.isatty()
来源：http://frd.hcnkem.com

[U40] Py：打印到标准错误
来源：http://tvj.hnxiangtu.top

print("err", file=sys.stderr)
来源：http://tiu.zhongyouzk.top

[U41] PHP：初始化 Composer 项目
来源：http://brm.xziqi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fkf.jinyuanbaomall.cn

[U42] PHP：PSR-4 自动加载
来源：http://fab.dianchejie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lkf.dianchejie.cn

[U43] PHP：声明命名空间
来源：http://yvg.jinqigufen.top

namespace App\Http;
来源：http://dnd.snrcjt.cn

[U44] PHP：开启严格类型
来源：http://ymj.hesvh.cn

declare(strict_types=1);
来源：http://lau.ydjk.org.cn

[U45] PHP：类型声明与返回类型
来源：http://ycs.jyoumei.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pxe.tianlin.xyz

[U46] PHP：可空类型
来源：http://mym.tarul.cn

?string $name = null
来源：http://fwp.aibaodan.cn

[U47] PHP：联合类型
来源：http://qae.cqqwz.cn

int|string $id
来源：http://zva.xziqi.cn

[U48] PHP：纯枚举
来源：http://xcu.hysaishi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://uwq.cheryme.top

[U49] PHP：只读属性
来源：http://urv.tian-w.cn

public readonly string $name
来源：http://cdj.yueranfly.top

[U50] PHP：构造器属性提升
来源：http://sji.ctjpmb.com

public function __construct(private int $id) {}
来源：http://qid.uphjek.com

[U51] PHP：数组解构
来源：http://orf.jqgfzy.top

[$a, $b] = $arr;
来源：http://wer.uphjek.com

[U52] PHP：箭头函数
来源：http://iwp.redwolf501.top

$double = fn($x) => $x * 2;
来源：http://alm.redwolf501.top

[U53] PHP：空合并运算符
来源：http://xoy.aibaodan.cn

$v = $a ?? $b ?? "default";
来源：http://xpq.feifeiyinyue.top

[U54] PHP：空安全调用
来源：http://zzy.yj20258888.top

$obj?->method()
来源：http://abg.52xcode.cn

[U55] PHP：match 表达式
来源：http://upy.zhengqikj.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hny.hesvh.cn

[U56] PHP：命名参数
来源：http://dhz.ywan-chungtsiang.top

f(a: 1, b: 2)
来源：http://klm.hnxiangtu.top

[U57] PHP：字符串插值
来源：http://pcx.yuxming.cn

"值: {$a}"
来源：http://vqo.yj20258.top

[U58] PHP：数组三件套
来源：http://zyw.pycfn.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ysm.316326.xyz

[U59] PHP：自定义排序
来源：http://lgv.mhx1999.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ymu.xingfuxueyuan.xyz

[U60] PHP：JSON 编解码
来源：http://ixd.aibaodan.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vnm.aizwys.cn

[U61] PHP：正则
来源：http://slw.sweek.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://syf.sweek.top

[U62] PHP：日期对象
来源：http://aio.zhaomingkeji.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uhf.tianlin.xyz

[U63] PHP：文件读写
来源：http://nop.wangdashe.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xnv.zycfv.cn

[U64] PHP：目录遍历
来源：http://wvz.vqdsnc.cn

glob("dir/*.php");  scandir("dir");
来源：http://qni.shangyingyoupin.top

[U65] PHP：会话
来源：http://vtj.fktsv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://scd.andypj.xyz

[U66] PHP：设置 Cookie
来源：http://ibn.tarul.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ajp.jinyuanbaomall.cn

[U67] PHP：处理文件上传
来源：http://wms.ehwqpu.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pxt.sjlbkw.cn

[U68] PHP：PDO 连接
来源：http://egz.cdnleiting.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://psx.hongshengwenyu.top

[U69] PHP：PDO 预处理
来源：http://ukz.zhoulong.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yti.zhongyouzk.top

[U70] PHP：PDO 事务
来源：http://jyw.smart0.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qvi.bbcook.cn

[U71] PHP：抛出异常
来源：http://ehs.ehwqpu.com

throw new RuntimeException("失败", 500);
来源：http://pwf.mhx1999.top

[U72] PHP：写错误日志
来源：http://gxg.chenlongwang.top

error_log("失败: " . $e->getMessage());
来源：http://kgn.sysykeji.top

[U73] PHP：读取 ini 配置
来源：http://lgh.hcnkem.com

parse_ini_file("config.ini", true)
来源：http://gtq.xinyue.icu

[U74] PHP：读取环境变量
来源：http://xnq.ybcxt.top

getenv("APP_ENV") ?: "production"
来源：http://yaw.jqgufenzy.top

[U75] PHP：依赖注入
来源：http://xzy.gotoacloud.top

composer require psr/container
来源：http://xtm.sjlbkw.cn

[U76] PHP：简单路由
来源：http://vlx.uphjek.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sip.xylfe.cn

[U77] PHP：模板渲染
来源：http://wlb.hesvh.cn

composer require twig/twig
来源：http://afj.gzhubu.top

[U78] PHP：单元测试
来源：http://lrt.ywan-chungtsiang.top

composer require --dev phpunit/phpunit
来源：http://bqn.epnwcf.com

[U79] PHP：静态分析
来源：http://axo.ydjk.org.cn

composer require --dev phpstan/phpstan
来源：http://bgz.aibaodan.cn

[U80] PHP：代码规范修复
来源：http://hes.jyoumei.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wxy.nanxuanxn.top

[U81] JS：初始化项目
来源：http://whr.xingfuxueyuan.xyz

npm init -y;  npm i express
来源：http://wpg.jyoumei.cn

[U82] JS：package.json 脚本
来源：http://gfy.cqqwz.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qok.ehwqpu.com

[U83] JS：ES Module 导入导出
来源：http://gzc.fzhhl.top

export const a = 1;  import { a } from "./m.js";
来源：http://tla.haohaochexian.top

[U84] JS：CommonJS 写法
来源：http://ncq.jianghu66.top

module.exports = { a };  const { a } = require("./m");
来源：http://okm.guowangkeji.top

[U85] JS：可选链
来源：http://rgk.hnxiangtu.top

a?.b?.c
来源：http://asb.shzxlz.cn

[U86] JS：空值合并
来源：http://mei.epnwcf.com

a ?? b
来源：http://nrz.wangshuangyany.cn

[U87] JS：解构默认值
来源：http://xqu.jiagoushi.top

const { a = 1, b = 2 } = obj;
来源：http://utm.zhongyouzk.top

[U88] JS：对象展开合并
来源：http://rjh.cucudq.cn

{ ...a, ...b }
来源：http://htz.jinqigufen.top

[U89] JS：数组去重
来源：http://yhb.guannengcc.top

[...new Set(arr)]
来源：http://fzn.yj20258888.top

[U90] JS：数字数组排序
来源：http://qhm.yongpay.top

[...arr].sort((a, b) => a - b)
来源：http://ain.pycfn.com

[U91] JS：对象键值遍历
来源：http://wuy.ydzc1.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vdg.zdqjudy.top

[U92] JS：深拷贝
来源：http://zfu.cheryme.top

structuredClone(obj)
来源：http://xyh.jinghuilouyu.cn

[U93] JS：模板字符串
来源：http://lch.jinqigfzy.top

`共 ${n} 条`
来源：http://tmc.pengpengdd.cyou

[U94] JS：箭头函数
来源：http://gee.quarkkingdee.top

const double = x => x * 2;
来源：http://ttn.cqqwz.cn

[U95] JS：Promise 包装
来源：http://thu.xziqi.cn

new Promise((resolve, reject) => {})
来源：http://hci.c1oappe.top

[U96] JS：async/await 与异常
来源：http://iyy.yj20258888.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jwt.smart0.xyz

[U97] JS：并发请求
来源：http://xxs.gogol.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://sva.sysykeji.top

[U98] JS：fetch 带 JSON
来源：http://yhd.gaohongyu789.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bik.bjfxy.top

[U99] JS：事件监听
来源：http://znl.pycfn.com

el.addEventListener("click", e => {})
来源：http://vqy.guowangkeji.top

[U100] JS：DOM 查询
来源：http://qme.fengsongda.top

document.querySelector(".item")
来源：http://esc.sjlbkw.cn

[U101] JS：classList 操作
来源：http://wto.xuanzx.com

el.classList.toggle("active")
来源：http://ami.epnwcf.com

[U102] JS：本地存储
来源：http://uon.quarkkingdee.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://iuu.jinyuanbaomall.cn

[U103] JS：定时器
来源：http://add.jinghuilouyu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ckr.jinqigfzy.top

[U104] JS：防抖
来源：http://yzn.chenjidiqi.icu

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uth.mhx1999.top

[U105] JS：节流
来源：http://wpr.gotoacloud.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hmh.iojbl.cn

[U106] JS：日期格式化
来源：http://hug.hongshengwenyu.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kbn.daxiang520.top

[U107] JS：数字千分位
来源：http://ktt.c1oappe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://oek.sufxvd.cn

[U108] JS：随机整数
来源：http://kla.aizwys.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tup.fktsv.cn

[U109] JS：数组分组
来源：http://vxf.fehbvm.com

Object.groupBy(arr, x => x.type)
来源：http://fpj.zhiwuduotai.top

[U110] JS：数组分块
来源：http://svz.uphjek.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qxh.hywenlv.cn

[U111] JS：对象转 Map
来源：http://dpg.52xcode.cn

new Map(Object.entries(obj))
来源：http://ixm.9152youxi.cn

[U112] JS：字符串补位
来源：http://exx.shzxlz.cn

"7".padStart(3, "0")
来源：http://kaa.hammf.cn

[U113] JS：正则替换全部
来源：http://edd.yfazqb.com

s.replaceAll("a", "b")
来源：http://ybc.zdqjudy.top

[U114] JS：JSON 深比较
来源：http://hjs.hcnkem.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://bwc.nanxinkj.top

[U115] JS：生成 UUID
来源：http://mfo.cashguo.top

crypto.randomUUID()
来源：http://zit.fehbvm.com

[U116] JS：类型检查（JSDoc）
来源：http://ybw.fanxiaobao.xyz

/** @param {string} name */ function f(name) {}
来源：http://rgn.yuanzhike.top

[U117] JS：单元测试
来源：http://lym.zycfv.cn

npm i -D vitest;  npx vitest
来源：http://rai.ehwqpu.com

[U118] JS：开发服务器
来源：http://vub.epnwcf.com

npm i -D vite;  npx vite
来源：http://ajp.daria6918.cn

[U119] JS：生产构建
来源：http://ytn.nanxinkj.top

npx vite build
来源：http://xng.fehbvm.com

[U120] JS：读取环境变量（Vite）
来源：http://kqn.feifeiyinyue.top

import.meta.env.VITE_API_URL
来源：http://une.sweek.top

================================================================================
来源：http://klj.jqgfzy.top

统计汇总
来源：http://why.cashguo.top

================================================================================
来源：http://mlb.uphjek.com

按语言统计（条）：
来源：http://jrv.tian-w.cn

Python ......... 252
来源：http://glr.aibaodan.cn

PHP ............ 252
来源：http://zaa.hcnkem.com

JavaScript ..... 252
来源：http://loj.yonumen.top

TypeScript ..... 212
来源：http://zss.nanxuanxn.top

Java ........... 212
来源：http://zns.fehbvm.com

Go ............. 212
来源：http://oaw.yonumen.top

Ruby ........... 212
来源：http://pes.shzxlz.cn

C# ............. 212
来源：http://mkk.yj20258.top

C .............. 30
来源：http://iaq.zdqjudy.top

C++ ............ 30
来源：http://ovt.gzhubu.top

SQL ............ 90
来源：http://pxg.chenzaomai.com

Bash ........... 80
来源：http://izu.yangfankeji.com

Kotlin ......... 15
来源：http://eoj.sxryk.cn

Swift .......... 15
来源：http://qyg.xinyue.icu

Lua ............ 10
来源：http://zpb.aizwys.cn

Perl ........... 10
来源：http://pxo.yj202588.top

Scala .......... 10
来源：http://feo.pycfn.com

------------------------------------
来源：http://hvq.zhiwuduotai.top

合计 ........... 2106 条
来源：http://qft.chenjidiqi.icu

按章节统计：
来源：http://wtj.zhengqikj.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://azp.ywan-chungtsiang.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://esv.fzhhl.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vgq.aizwys.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pvi.meibo888.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uri.jinqigfzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hkd.guowangkeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://slx.feifeiyinyue.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ena.yanxiufei.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qqu.zdqjudy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pdx.hesvh.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ome.yuanzhike.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://are.gaohongyu789.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://huq.chenzaomai.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xak.xuanzx.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bbi.shanyushiyangtech.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mqm.hysaishi.cn

Q SQL 专题                              90
来源：http://tbh.shuidangran.top

R Bash 专题                             80
来源：http://fhd.yueranfly.top

S C / C++ 专题                          60
来源：http://yvq.wangshuangyany.cn

T 其他语言补充                          60
来源：http://eje.ctjpmb.com

U 高频实用片段                         120
来源：http://zpv.hammf.cn

------------------------------------
来源：http://vbk.9152youxi.cn

合计                                  2106 条
来源：http://abo.daxiang520.top

--------------------------------------------------------------------------------
来源：http://oxz.zhaomingkeji.xyz

使用提醒
来源：http://iqa.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://hwb.guowangkeji.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://oix.xuanzx.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hbm.zhiwuduotai.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://foh.yueranfly.top

在旧版本上使用前请先确认语法支持情况。
来源：http://pzo.gaohongyu789.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nrs.meibo888.top

—— 文件结束 ——
来源：http://kjt.sweek.top

================================================================================
来源：http://orh.kuanghao11.cn

程序语言常见例子速查手册（2024 版）
来源：http://lit.jqgufenzy.top

Common Programming Examples Cheat Book
来源：http://lir.hongshengwenyu.top

================================================================================
来源：http://uyw.ehwqpu.com

【收录内容】
来源：http://nuk.birdmap.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://qkh.iojbl.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sck.sufxvd.cn

SQL · Bash · C · C++
来源：http://rjf.xylfe.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dve.tarul.cn

【使用说明】
来源：http://smf.vqdsnc.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lgu.cdnleiting.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vkz.hywenlv.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://puc.mhx1999.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kiu.zhongyouzk.top

Bash:  Shell         C:     C             C++:   C++
来源：http://wam.shanyushiyangkeji.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zye.chenjidiqi.icu

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tap.jiagoushi.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mrc.smart0.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yez.cucudq.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ndq.daria6918.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://khi.zhixingplan.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qrx.yfazqb.com

【文件统计】
来源：http://bed.yanxiufei.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ajn.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://hcy.sweek.top

目  录
来源：http://wui.c1oappe.top

--------------------------------------------------------------------------------
来源：http://glz.hnxiangtu.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jmo.zycfv.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://msw.sweek.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ymx.tanke756.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pwm.shanyushiyangtech.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ouo.xinyue.icu

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://nws.dianchejie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uxv.cucudq.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://txc.cqqwz.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fps.iojbl.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://aeh.chenlongwang.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bzp.dianchejie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yax.hywenlv.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pij.hnqzz.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ugs.pycfn.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dsn.fengsongda.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xsy.wangdashe.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://icm.jqgfzy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://kef.zhongyouzk.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qaj.fktsv.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fui.yonumen.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cdp.vqdsnc.cn

================================================================================
来源：http://apw.vqdsnc.cn

A. 基础语法与类型
来源：http://xyp.zhongyouzk.top

================================================================================
来源：http://num.sysykeji.top

[A01] Hello World
来源：http://gws.ydjk.org.cn

Py:   print("Hello, World!")
来源：http://zzy.sufxvd.cn

PHP:  echo "Hello, World!";
来源：http://dje.wangdashe.top

JS:   console.log("Hello, World!");
来源：http://xdf.chenjidiqi.icu

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wnm.xylfe.cn

Java: System.out.println("Hello, World!");
来源：http://lwo.chenzaomai.com

Go:   fmt.Println("Hello, World!")
来源：http://ior.yonumen.top

Ruby: puts "Hello, World!"
来源：http://uzr.hcnkem.com

C#:   Console.WriteLine("Hello, World!");
来源：http://vdf.yanxiufei.cn

[A02] 变量声明与赋值
来源：http://itq.xylfe.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://oiw.mhx1999.top

PHP:  $name = "Alex"; $age = 20;
来源：http://rmy.ydzc1.top

JS:   let name = "Alex"; const age = 20;
来源：http://jri.shangyingyoupin.top


<!-- 参考信息 -->