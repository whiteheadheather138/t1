代发 wailian999

[U31] Py：单测
来源：http://gie.jinqigufen.top

python -m pytest -q
来源：http://rkd.xingfuxueyuan.xyz

[U32] Py：代码格式化
来源：http://cnm.jianghu66.top

ruff format . && ruff check --fix .
来源：http://ezg.aibaodan.cn

[U33] Py：打包发布
来源：http://uag.iojbl.cn

python -m build  （依赖 pyproject.toml）
来源：http://rct.jqgufenzy.top

[U34] Py：判断编码
来源：http://xlg.jyoumei.cn

chardet.detect(raw)
来源：http://xhj.ppjwa.cn

[U35] Py：发送邮件
来源：http://len.sufxvd.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rlp.yueranfly.top

[U36] Py：定时任务
来源：http://zgn.fktsv.cn

schedule.every(10).minutes.do(job)
来源：http://fic.bjfxy.top

[U37] Py：读写 Excel
来源：http://rxe.fehbvm.com

pandas.read_excel / DataFrame.to_excel
来源：http://ddc.xziqi.cn

[U38] Py：获取脚本所在目录
来源：http://erg.nanxinkj.top

Path(__file__).resolve().parent
来源：http://kpw.vehdjk.com

[U39] Py：判断是否在交互环境
来源：http://aem.yangfankeji.com

sys.stdout.isatty()
来源：http://quf.gzhubu.top

[U40] Py：打印到标准错误
来源：http://zos.gotoacloud.top

print("err", file=sys.stderr)
来源：http://sev.guannengcc.top

[U41] PHP：初始化 Composer 项目
来源：http://aqp.hfpthk.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fjr.dianchejie.cn

[U42] PHP：PSR-4 自动加载
来源：http://wus.epnwcf.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ngm.chenjidiqi.icu

[U43] PHP：声明命名空间
来源：http://kxl.zhijiandao.cn

namespace App\Http;
来源：http://elc.tanke756.top

[U44] PHP：开启严格类型
来源：http://etf.yongpay.top

declare(strict_types=1);
来源：http://iya.chenjidiqi.icu

[U45] PHP：类型声明与返回类型
来源：http://lrs.gogol.net.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://tce.fengsongda.top

[U46] PHP：可空类型
来源：http://yqm.xingfuxueyuan.xyz

?string $name = null
来源：http://elx.ywan-chungtsiang.top

[U47] PHP：联合类型
来源：http://giy.shanyushiyangtech.top

int|string $id
来源：http://lff.tanke756.top

[U48] PHP：纯枚举
来源：http://qyk.smart0.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://usm.nanxuanxn.top

[U49] PHP：只读属性
来源：http://ami.mhx1999.top

public readonly string $name
来源：http://rnk.hnxiangtu.top

[U50] PHP：构造器属性提升
来源：http://auo.svipenyu.cn

public function __construct(private int $id) {}
来源：http://gyv.guannengcc.top

[U51] PHP：数组解构
来源：http://zpz.wangdashe.top

[$a, $b] = $arr;
来源：http://mpf.gzhubu.top

[U52] PHP：箭头函数
来源：http://jph.nanxuanxn.top

$double = fn($x) => $x * 2;
来源：http://ndg.zhengqikj.top

[U53] PHP：空合并运算符
来源：http://gvg.birdmap.top

$v = $a ?? $b ?? "default";
来源：http://gln.sweek.top

[U54] PHP：空安全调用
来源：http://hoy.epnwcf.com

$obj?->method()
来源：http://qav.shuidangran.top

[U55] PHP：match 表达式
来源：http://uwv.ydjk.org.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://azd.havefunace.top

[U56] PHP：命名参数
来源：http://jea.aizwys.cn

f(a: 1, b: 2)
来源：http://aup.aizwys.cn

[U57] PHP：字符串插值
来源：http://wfa.xylfe.cn

"值: {$a}"
来源：http://zbv.yj202588.top

[U58] PHP：数组三件套
来源：http://ktm.jqgufenzy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://snn.ivvv.top

[U59] PHP：自定义排序
来源：http://khp.svipenyu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lww.0kj1m.cn

[U60] PHP：JSON 编解码
来源：http://lzb.chenzaomai.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jmu.fanxiaobao.xyz

[U61] PHP：正则
来源：http://obv.pycfn.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tvk.kuanghao11.cn

[U62] PHP：日期对象
来源：http://tsw.andypj.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jio.fanxiaobao.xyz

[U63] PHP：文件读写
来源：http://dcp.jiagoushi.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wnu.sufxvd.cn

[U64] PHP：目录遍历
来源：http://spe.yvedp.cn

glob("dir/*.php");  scandir("dir");
来源：http://fvo.hnxiangtu.top

[U65] PHP：会话
来源：http://tcv.316326.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://cfc.zdbjq.cn

[U66] PHP：设置 Cookie
来源：http://ako.hammf.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rkv.zdqjudy.top

[U67] PHP：处理文件上传
来源：http://tne.dianchejie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hpj.sufxvd.cn

[U68] PHP：PDO 连接
来源：http://xew.cheryme.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sso.uphjek.com

[U69] PHP：PDO 预处理
来源：http://nti.fehbvm.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jxx.fanxiaobao.xyz

[U70] PHP：PDO 事务
来源：http://zyq.meibo888.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jvd.xinyue.icu

[U71] PHP：抛出异常
来源：http://kzl.ywan-chungtsiang.top

throw new RuntimeException("失败", 500);
来源：http://vhx.kuanghao11.cn

[U72] PHP：写错误日志
来源：http://wnm.gogol.net.cn

error_log("失败: " . $e->getMessage());
来源：http://fjb.vqdsnc.cn

[U73] PHP：读取 ini 配置
来源：http://xpi.jqgfzy.top

parse_ini_file("config.ini", true)
来源：http://wnt.nanxuanxn.top

[U74] PHP：读取环境变量
来源：http://iud.zhoulong.xyz

getenv("APP_ENV") ?: "production"
来源：http://yya.nanxuanxn.top

[U75] PHP：依赖注入
来源：http://vme.cqqwz.cn

composer require psr/container
来源：http://wuz.xziqi.cn

[U76] PHP：简单路由
来源：http://awp.feifeiyinyue.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wpz.sufxvd.cn

[U77] PHP：模板渲染
来源：http://uwd.hnqzz.top

composer require twig/twig
来源：http://shz.gogol.net.cn

[U78] PHP：单元测试
来源：http://wgo.svipenyu.cn

composer require --dev phpunit/phpunit
来源：http://rxs.yonumen.top

[U79] PHP：静态分析
来源：http://ywk.shangyingyoupin.top

composer require --dev phpstan/phpstan
来源：http://hlh.vqdsnc.cn

[U80] PHP：代码规范修复
来源：http://ita.sysykeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://sty.guowangkeji.top

[U81] JS：初始化项目
来源：http://skj.kuanghao11.cn

npm init -y;  npm i express
来源：http://iwf.jinghuilouyu.cn

[U82] JS：package.json 脚本
来源：http://jdu.wangdashe.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cag.jinqigufen.top

[U83] JS：ES Module 导入导出
来源：http://hka.xziqi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dvj.vehdjk.com

[U84] JS：CommonJS 写法
来源：http://kvi.zhiwuduotai.top

module.exports = { a };  const { a } = require("./m");
来源：http://fvr.ivvv.top

[U85] JS：可选链
来源：http://yjg.hnxiangtu.top

a?.b?.c
来源：http://amo.jyoumei.cn

[U86] JS：空值合并
来源：http://imp.shanyushiyangkeji.top

a ?? b
来源：http://tmy.birdmap.top

[U87] JS：解构默认值
来源：http://kff.fengsongda.top

const { a = 1, b = 2 } = obj;
来源：http://ywz.wangshuangyany.cn

[U88] JS：对象展开合并
来源：http://qqk.cheryme.top

{ ...a, ...b }
来源：http://tma.zdqjudy.top

[U89] JS：数组去重
来源：http://mmd.hcnkem.com

[...new Set(arr)]
来源：http://wqh.redwolf501.top

[U90] JS：数字数组排序
来源：http://qte.havefunace.top

[...arr].sort((a, b) => a - b)
来源：http://aqe.0kj1m.cn

[U91] JS：对象键值遍历
来源：http://qbq.yj20258888.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ykg.nwbrower.top

[U92] JS：深拷贝
来源：http://iug.sysykeji.top

structuredClone(obj)
来源：http://gel.shangyingyoupin.top

[U93] JS：模板字符串
来源：http://rab.cucudq.cn

`共 ${n} 条`
来源：http://yxh.mhx1999.top

[U94] JS：箭头函数
来源：http://gqz.uphjek.com

const double = x => x * 2;
来源：http://sav.sufxvd.cn

[U95] JS：Promise 包装
来源：http://ydh.zhoulong.xyz

new Promise((resolve, reject) => {})
来源：http://pts.mhx1999.top

[U96] JS：async/await 与异常
来源：http://puf.yongpay.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://toz.chenzaomai.com

[U97] JS：并发请求
来源：http://rlr.iojbl.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dvw.nwbrower.top

[U98] JS：fetch 带 JSON
来源：http://uet.xuanzx.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kew.jiagoushi.top

[U99] JS：事件监听
来源：http://kcv.yj20258.top

el.addEventListener("click", e => {})
来源：http://dol.fanxiaobao.xyz

[U100] JS：DOM 查询
来源：http://xje.zhengqikj.top

document.querySelector(".item")
来源：http://euc.fengsongda.top

[U101] JS：classList 操作
来源：http://kgj.jlsjyb.cn

el.classList.toggle("active")
来源：http://ywn.shuidangran.top

[U102] JS：本地存储
来源：http://qfo.hfpthk.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zur.fktsv.cn

[U103] JS：定时器
来源：http://qfz.tianlin.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pen.xingfuxueyuan.xyz

[U104] JS：防抖
来源：http://euz.yj20258.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jif.hnxiangtu.top

[U105] JS：节流
来源：http://znm.sufxvd.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://npy.kuanghao11.cn

[U106] JS：日期格式化
来源：http://sod.ivvv.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nis.ydjk.org.cn

[U107] JS：数字千分位
来源：http://fte.smart0.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lgt.ydzc1.top

[U108] JS：随机整数
来源：http://cvf.pengpengdd.cyou

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tkt.zhoulong.xyz

[U109] JS：数组分组
来源：http://vwo.kuanghao11.cn

Object.groupBy(arr, x => x.type)
来源：http://ure.yonumen.top

[U110] JS：数组分块
来源：http://lbs.jinqigufen.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xdx.redwolf501.top

[U111] JS：对象转 Map
来源：http://mwe.jianghu66.top

new Map(Object.entries(obj))
来源：http://nsq.uphjek.com

[U112] JS：字符串补位
来源：http://thd.bbcook.cn

"7".padStart(3, "0")
来源：http://dbv.snrcjt.cn

[U113] JS：正则替换全部
来源：http://qfl.chenjidiqi.icu

s.replaceAll("a", "b")
来源：http://jwe.daxiang520.top

[U114] JS：JSON 深比较
来源：http://gan.zhoulong.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://ppe.xziqi.cn

[U115] JS：生成 UUID
来源：http://mzz.yj20258.top

crypto.randomUUID()
来源：http://tkf.cqqwz.cn

[U116] JS：类型检查（JSDoc）
来源：http://lwc.cucudq.cn

/** @param {string} name */ function f(name) {}
来源：http://abe.zhiwuduotai.top

[U117] JS：单元测试
来源：http://oab.yj20258888.top

npm i -D vitest;  npx vitest
来源：http://uws.chenjidiqi.icu

[U118] JS：开发服务器
来源：http://xta.xingfuxueyuan.xyz

npm i -D vite;  npx vite
来源：http://nfw.chenjidiqi.icu

[U119] JS：生产构建
来源：http://yge.feifeiyinyue.top

npx vite build
来源：http://twc.redwolf501.top

[U120] JS：读取环境变量（Vite）
来源：http://sen.gaohongyu789.top

import.meta.env.VITE_API_URL
来源：http://qws.c1oappe.top

================================================================================
来源：http://dhg.fzhhl.top

统计汇总
来源：http://pwf.nanxuanxn.top

================================================================================
来源：http://cov.jqgfzy.top

按语言统计（条）：
来源：http://cwi.aibaodan.cn

Python ......... 252
来源：http://yny.smart0.xyz

PHP ............ 252
来源：http://nlc.nanxinkj.top

JavaScript ..... 252
来源：http://ujm.jinyuanbaomall.cn

TypeScript ..... 212
来源：http://bzj.epnwcf.com

Java ........... 212
来源：http://gga.zhengqikj.top

Go ............. 212
来源：http://edv.vehdjk.com

Ruby ........... 212
来源：http://mja.daria6918.cn

C# ............. 212
来源：http://ojj.gotoacloud.top

C .............. 30
来源：http://uub.nanxuanxn.top

C++ ............ 30
来源：http://mcy.ehwqpu.com

SQL ............ 90
来源：http://pmo.redwolf501.top

Bash ........... 80
来源：http://jqw.0kj1m.cn

Kotlin ......... 15
来源：http://nho.tarul.cn

Swift .......... 15
来源：http://hff.zhengqikj.top

Lua ............ 10
来源：http://svc.ydzc1.top

Perl ........... 10
来源：http://dxr.ydjk.org.cn

Scala .......... 10
来源：http://izg.ivvv.top

------------------------------------
来源：http://nbc.nanxuanxn.top

合计 ........... 2106 条
来源：http://pew.bbcook.cn

按章节统计：
来源：http://ogl.hcnkem.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ehf.epnwcf.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wor.cucudq.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jys.gogol.net.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rfx.zhaomingkeji.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gjb.sxryk.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://luh.yj202588.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pjh.vqdsnc.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://csp.xylfe.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://grt.hammf.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xtg.fanxiaobao.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gcl.zhoulong.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mja.yuanzhike.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kgs.yj202588.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wet.zhixingplan.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dlq.fanxiaobao.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vjq.ivvv.top

Q SQL 专题                              90
来源：http://fku.fehbvm.com

R Bash 专题                             80
来源：http://fhf.ybcxt.top

S C / C++ 专题                          60
来源：http://zas.zdqjudy.top

T 其他语言补充                          60
来源：http://fdq.yvedp.cn

U 高频实用片段                         120
来源：http://usj.meibo888.top

------------------------------------
来源：http://tif.feifeiyinyue.top

合计                                  2106 条
来源：http://olp.fehbvm.com

--------------------------------------------------------------------------------
来源：http://xea.tanke756.top

使用提醒
来源：http://enk.tianlin.xyz

--------------------------------------------------------------------------------
来源：http://pib.pengpengdd.cyou

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nfk.smart0.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://svp.ydzc1.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://oir.wangshuangyany.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wyz.yanxiufei.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xhw.jinqigufen.top

—— 文件结束 ——
来源：http://hsp.316326.xyz

================================================================================
来源：http://sws.zdqjudy.top

程序语言常见例子速查手册（2024 版）
来源：http://khe.hongshengwenyu.top

Common Programming Examples Cheat Book
来源：http://wli.zhengqikj.top

================================================================================
来源：http://umk.andypj.xyz

【收录内容】
来源：http://rux.xuanzx.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://wqa.yvedp.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://efw.yj20258888.top

SQL · Bash · C · C++
来源：http://ino.tian-w.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qaa.fzhhl.top

【使用说明】
来源：http://gwv.wangshuangyany.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mmk.feifeiyinyue.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hyu.zhengqikj.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://eik.gogol.net.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vnm.hcnkem.com

Bash:  Shell         C:     C             C++:   C++
来源：http://rnr.ivvv.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gme.hesvh.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cwx.cdnleiting.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ntl.pycfn.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mnv.hcnkem.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cdu.yfazqb.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fyi.9152youxi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bjx.yonumen.top

【文件统计】
来源：http://fkb.jinyuanbaomall.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://iag.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://ikk.jinyuanbaomall.cn

目  录
来源：http://bzt.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://eay.jlsjyb.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rgq.fehbvm.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vmh.ydjk.org.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nko.0kj1m.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://afr.jinghuilouyu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mek.nanxinkj.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mxo.vqdsnc.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sdo.zhixingplan.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cqr.dianchejie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ypt.feifeiyinyue.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jwi.chenzaomai.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qey.zycfv.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://etn.pycfn.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bcp.ywan-chungtsiang.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ler.fktsv.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fds.dianchejie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jhf.ivvv.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kgh.tianlin.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://tga.haohaochexian.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://how.yangfankeji.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bnb.kuanghao11.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://erc.hammf.cn

================================================================================
来源：http://dfk.kuanghao11.cn

A. 基础语法与类型
来源：http://uqj.zhiwuduotai.top

================================================================================
来源：http://zqe.shanyushiyangkeji.top

[A01] Hello World
来源：http://wzl.zhiwuduotai.top

Py:   print("Hello, World!")
来源：http://cei.cucudq.cn

PHP:  echo "Hello, World!";
来源：http://jpk.fehbvm.com

JS:   console.log("Hello, World!");
来源：http://xdw.sufxvd.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://smk.jinyuanbaomall.cn

Java: System.out.println("Hello, World!");
来源：http://lup.uphjek.com

Go:   fmt.Println("Hello, World!")
来源：http://gzn.guannengcc.top

Ruby: puts "Hello, World!"
来源：http://qva.cheryme.top

C#:   Console.WriteLine("Hello, World!");
来源：http://edm.cucudq.cn

[A02] 变量声明与赋值
来源：http://whl.zhiwuduotai.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ydy.yuxming.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://djj.bjfxy.top

JS:   let name = "Alex"; const age = 20;
来源：http://gja.yfazqb.com


<!-- 参考信息 -->