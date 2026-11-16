代发 wailian999

[U33] Py：打包发布
来源：http://orc.hongshengwenyu.top

python -m build  （依赖 pyproject.toml）
来源：http://ysb.shanyushiyangkeji.top

[U34] Py：判断编码
来源：http://tey.yangfankeji.com

chardet.detect(raw)
来源：http://nfo.shanyushiyangtech.top

[U35] Py：发送邮件
来源：http://rin.xinyue.icu

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oks.tarul.cn

[U36] Py：定时任务
来源：http://mls.fehbvm.com

schedule.every(10).minutes.do(job)
来源：http://hik.mhx1999.top

[U37] Py：读写 Excel
来源：http://lqe.fehbvm.com

pandas.read_excel / DataFrame.to_excel
来源：http://cge.guowangkeji.top

[U38] Py：获取脚本所在目录
来源：http://kgg.jlsjyb.cn

Path(__file__).resolve().parent
来源：http://dly.xylfe.cn

[U39] Py：判断是否在交互环境
来源：http://csy.haohaochexian.top

sys.stdout.isatty()
来源：http://rmx.hammf.cn

[U40] Py：打印到标准错误
来源：http://eik.sjlbkw.cn

print("err", file=sys.stderr)
来源：http://fob.bjfxy.top

[U41] PHP：初始化 Composer 项目
来源：http://gkg.birdmap.top

composer init;  composer require guzzlehttp/guzzle
来源：http://gap.xuetiantiany.cn

[U42] PHP：PSR-4 自动加载
来源：http://vun.jianghu66.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jun.hysaishi.cn

[U43] PHP：声明命名空间
来源：http://qku.nanxinkj.top

namespace App\Http;
来源：http://nng.zhongyouzk.top

[U44] PHP：开启严格类型
来源：http://yff.gotoacloud.top

declare(strict_types=1);
来源：http://uli.zhiwuduotai.top

[U45] PHP：类型声明与返回类型
来源：http://mud.redwolf501.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://fvc.gaohongyu789.top

[U46] PHP：可空类型
来源：http://iys.shuidangran.top

?string $name = null
来源：http://whh.cheryme.top

[U47] PHP：联合类型
来源：http://jwo.kuanghao11.cn

int|string $id
来源：http://tbk.9152youxi.cn

[U48] PHP：纯枚举
来源：http://atm.yuanzhike.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://owd.wangdashe.top

[U49] PHP：只读属性
来源：http://eqr.yj20258888.top

public readonly string $name
来源：http://amw.9152youxi.cn

[U50] PHP：构造器属性提升
来源：http://xtt.zhijiandao.cn

public function __construct(private int $id) {}
来源：http://goh.yanxiufei.cn

[U51] PHP：数组解构
来源：http://zwf.daria6918.cn

[$a, $b] = $arr;
来源：http://wyu.jinqigfzy.top

[U52] PHP：箭头函数
来源：http://tuc.guannengcc.top

$double = fn($x) => $x * 2;
来源：http://ife.hongshengwenyu.top

[U53] PHP：空合并运算符
来源：http://pgg.zycfv.cn

$v = $a ?? $b ?? "default";
来源：http://dog.shuidangran.top

[U54] PHP：空安全调用
来源：http://mhr.yvedp.cn

$obj?->method()
来源：http://flp.aibaodan.cn

[U55] PHP：match 表达式
来源：http://idx.bbcook.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://iwm.jinqigfzy.top

[U56] PHP：命名参数
来源：http://taw.shangyingyoupin.top

f(a: 1, b: 2)
来源：http://qmo.zhijiandao.cn

[U57] PHP：字符串插值
来源：http://xpj.gotoacloud.top

"值: {$a}"
来源：http://dfl.mhx1999.top

[U58] PHP：数组三件套
来源：http://chg.pycfn.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ryu.yueranfly.top

[U59] PHP：自定义排序
来源：http://ybe.nanxinkj.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://usg.yj20258.top

[U60] PHP：JSON 编解码
来源：http://hrq.zhengqikj.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lzl.daxiang520.top

[U61] PHP：正则
来源：http://ybv.hywenlv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jjh.sufxvd.cn

[U62] PHP：日期对象
来源：http://onq.feifeiyinyue.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rvl.zhengqikj.top

[U63] PHP：文件读写
来源：http://yip.zhoulong.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://aqo.hnxiangtu.top

[U64] PHP：目录遍历
来源：http://dak.cucudq.cn

glob("dir/*.php");  scandir("dir");
来源：http://hnv.sufxvd.cn

[U65] PHP：会话
来源：http://vje.yongpay.top

session_start();  $_SESSION["uid"] = 1;
来源：http://chj.shzxlz.cn

[U66] PHP：设置 Cookie
来源：http://axr.zhongyouzk.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zyz.shuidangran.top

[U67] PHP：处理文件上传
来源：http://dvg.iojbl.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mjj.sxryk.cn

[U68] PHP：PDO 连接
来源：http://djo.yueranfly.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lxh.hcnkem.com

[U69] PHP：PDO 预处理
来源：http://iit.c1oappe.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uxh.fehbvm.com

[U70] PHP：PDO 事务
来源：http://xuf.jlsjyb.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sin.aizwys.cn

[U71] PHP：抛出异常
来源：http://xnv.wangshuangyany.cn

throw new RuntimeException("失败", 500);
来源：http://blr.tanke756.top

[U72] PHP：写错误日志
来源：http://hdy.dianchejie.cn

error_log("失败: " . $e->getMessage());
来源：http://wvf.ydzc1.top

[U73] PHP：读取 ini 配置
来源：http://vou.bbcook.cn

parse_ini_file("config.ini", true)
来源：http://tab.vqdsnc.cn

[U74] PHP：读取环境变量
来源：http://wxx.shangyingyoupin.top

getenv("APP_ENV") ?: "production"
来源：http://vxa.tianlin.xyz

[U75] PHP：依赖注入
来源：http://eif.guannengcc.top

composer require psr/container
来源：http://gjg.birdmap.top

[U76] PHP：简单路由
来源：http://wkp.jqgfzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tbi.aibaodan.cn

[U77] PHP：模板渲染
来源：http://fab.ctjpmb.com

composer require twig/twig
来源：http://nid.zdqjudy.top

[U78] PHP：单元测试
来源：http://huu.yuxming.cn

composer require --dev phpunit/phpunit
来源：http://vif.epnwcf.com

[U79] PHP：静态分析
来源：http://qms.c1oappe.top

composer require --dev phpstan/phpstan
来源：http://ghb.cashguo.top

[U80] PHP：代码规范修复
来源：http://rok.kuanghao11.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kqc.zdqjudy.top

[U81] JS：初始化项目
来源：http://snp.vqdsnc.cn

npm init -y;  npm i express
来源：http://dgh.hongshengwenyu.top

[U82] JS：package.json 脚本
来源：http://uwh.xylfe.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zpe.kuanghao11.cn

[U83] JS：ES Module 导入导出
来源：http://ddm.hesvh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://whc.sysykeji.top

[U84] JS：CommonJS 写法
来源：http://pek.andypj.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://fzm.fktsv.cn

[U85] JS：可选链
来源：http://vlg.jiagoushi.top

a?.b?.c
来源：http://syb.aizwys.cn

[U86] JS：空值合并
来源：http://nyd.hammf.cn

a ?? b
来源：http://lnu.gogol.net.cn

[U87] JS：解构默认值
来源：http://jjs.hnxiangtu.top

const { a = 1, b = 2 } = obj;
来源：http://xeu.andypj.xyz

[U88] JS：对象展开合并
来源：http://tio.shanyushiyangtech.top

{ ...a, ...b }
来源：http://cfw.snrcjt.cn

[U89] JS：数组去重
来源：http://vpz.nanxinkj.top

[...new Set(arr)]
来源：http://cgs.smart0.xyz

[U90] JS：数字数组排序
来源：http://oxf.yonumen.top

[...arr].sort((a, b) => a - b)
来源：http://ffk.vqdsnc.cn

[U91] JS：对象键值遍历
来源：http://bdb.epnwcf.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bgd.pycfn.com

[U92] JS：深拷贝
来源：http://ktu.xziqi.cn

structuredClone(obj)
来源：http://guq.smart0.xyz

[U93] JS：模板字符串
来源：http://sil.hesvh.cn

`共 ${n} 条`
来源：http://krt.aizwys.cn

[U94] JS：箭头函数
来源：http://xyy.fengsongda.top

const double = x => x * 2;
来源：http://hci.uphjek.com

[U95] JS：Promise 包装
来源：http://oun.nanxuanxn.top

new Promise((resolve, reject) => {})
来源：http://hty.ydjk.org.cn

[U96] JS：async/await 与异常
来源：http://pgj.yfazqb.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://eaw.zhiwuduotai.top

[U97] JS：并发请求
来源：http://qbm.sjlbkw.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ulc.hammf.cn

[U98] JS：fetch 带 JSON
来源：http://lel.zhaomingkeji.xyz

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://srv.redwolf501.top

[U99] JS：事件监听
来源：http://ieq.52xcode.cn

el.addEventListener("click", e => {})
来源：http://kns.feifeiyinyue.top

[U100] JS：DOM 查询
来源：http://cya.daria6918.cn

document.querySelector(".item")
来源：http://vrw.dianchejie.cn

[U101] JS：classList 操作
来源：http://bbd.cqqwz.cn

el.classList.toggle("active")
来源：http://hop.ybcxt.top

[U102] JS：本地存储
来源：http://fqz.hywenlv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vza.tanke756.top

[U103] JS：定时器
来源：http://mgf.ehwqpu.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jba.jinqigufen.top

[U104] JS：防抖
来源：http://dpa.guowangkeji.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gsj.gzhubu.top

[U105] JS：节流
来源：http://nzq.wangshuangyany.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://apw.gotoacloud.top

[U106] JS：日期格式化
来源：http://yib.yuxming.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://anw.haohaochexian.top

[U107] JS：数字千分位
来源：http://usf.cheryme.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vte.yonumen.top

[U108] JS：随机整数
来源：http://asc.dashuyun.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://int.gaohongyu789.top

[U109] JS：数组分组
来源：http://hzu.quarkkingdee.top

Object.groupBy(arr, x => x.type)
来源：http://abi.andypj.xyz

[U110] JS：数组分块
来源：http://nvy.zhaomingkeji.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zrt.cqqwz.cn

[U111] JS：对象转 Map
来源：http://wuc.zhijiandao.cn

new Map(Object.entries(obj))
来源：http://gdl.jinqigfzy.top

[U112] JS：字符串补位
来源：http://dww.zhengqikj.top

"7".padStart(3, "0")
来源：http://dku.jqgufenzy.top

[U113] JS：正则替换全部
来源：http://uxm.ppjwa.cn

s.replaceAll("a", "b")
来源：http://klf.svipenyu.cn

[U114] JS：JSON 深比较
来源：http://blz.jiagoushi.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://hxv.zdqjudy.top

[U115] JS：生成 UUID
来源：http://utf.smart0.xyz

crypto.randomUUID()
来源：http://fch.sxryk.cn

[U116] JS：类型检查（JSDoc）
来源：http://gkr.shangyingyoupin.top

/** @param {string} name */ function f(name) {}
来源：http://idl.jinyuanbaomall.cn

[U117] JS：单元测试
来源：http://zao.zhaomingkeji.xyz

npm i -D vitest;  npx vitest
来源：http://jdx.yanxiufei.cn

[U118] JS：开发服务器
来源：http://yvv.fengsongda.top

npm i -D vite;  npx vite
来源：http://cpb.ivvv.top

[U119] JS：生产构建
来源：http://btf.yj20258888.top

npx vite build
来源：http://njf.52xcode.cn

[U120] JS：读取环境变量（Vite）
来源：http://osz.cdnleiting.top

import.meta.env.VITE_API_URL
来源：http://ouj.quarkkingdee.top

================================================================================
来源：http://ncw.cqqwz.cn

统计汇总
来源：http://gnv.yongpay.top

================================================================================
来源：http://zwu.yanxiufei.cn

按语言统计（条）：
来源：http://ebc.9152youxi.cn

Python ......... 252
来源：http://xfa.zhaomingkeji.xyz

PHP ............ 252
来源：http://wso.vehdjk.com

JavaScript ..... 252
来源：http://fue.yuanzhike.top

TypeScript ..... 212
来源：http://fuz.sufxvd.cn

Java ........... 212
来源：http://mym.jlsjyb.cn

Go ............. 212
来源：http://lra.yj20258888.top

Ruby ........... 212
来源：http://acv.tarul.cn

C# ............. 212
来源：http://jws.zhoulong.xyz

C .............. 30
来源：http://dex.havefunace.top

C++ ............ 30
来源：http://vxy.aizwys.cn

SQL ............ 90
来源：http://jxp.aizwys.cn

Bash ........... 80
来源：http://yyp.nwbrower.top

Kotlin ......... 15
来源：http://dje.gzhubu.top

Swift .......... 15
来源：http://jho.xuetiantiany.cn

Lua ............ 10
来源：http://bau.yuxming.cn

Perl ........... 10
来源：http://rhb.zycfv.cn

Scala .......... 10
来源：http://haj.zhaomingkeji.xyz

------------------------------------
来源：http://lwa.tianlin.xyz

合计 ........... 2106 条
来源：http://hxp.guowangkeji.top

按章节统计：
来源：http://wvk.yuanzhike.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kyo.hfpthk.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zjx.jinqigufen.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mbp.zhoulong.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://opd.hongshengwenyu.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kkf.smart0.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vwi.zhengqikj.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://axx.zhoulong.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jjp.yuxming.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jzq.ybcxt.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://win.pengpengdd.cyou

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yiu.guowangkeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sgb.hywenlv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zfs.chenzaomai.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://enu.cdnleiting.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ivi.hywenlv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tdd.hongshengwenyu.top

Q SQL 专题                              90
来源：http://auy.0kj1m.cn

R Bash 专题                             80
来源：http://nck.xinyue.icu

S C / C++ 专题                          60
来源：http://hby.tianlin.xyz

T 其他语言补充                          60
来源：http://cxs.hesvh.cn

U 高频实用片段                         120
来源：http://bej.hongshengwenyu.top

------------------------------------
来源：http://auo.wangshuangyany.cn

合计                                  2106 条
来源：http://sql.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://zhs.birdmap.top

使用提醒
来源：http://luq.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://hfb.tianlin.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xpp.316326.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qke.ybcxt.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://obu.zhoulong.xyz

在旧版本上使用前请先确认语法支持情况。
来源：http://vsk.tanke756.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://sto.sxryk.cn

—— 文件结束 ——
来源：http://xou.iojbl.cn

================================================================================
来源：http://auf.shangyingyoupin.top

程序语言常见例子速查手册（2024 版）
来源：http://xlx.vqdsnc.cn

Common Programming Examples Cheat Book
来源：http://zuz.fzhhl.top

================================================================================
来源：http://kyh.havefunace.top

【收录内容】
来源：http://one.yuxming.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://nvn.jlsjyb.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ack.nanxuanxn.top

SQL · Bash · C · C++
来源：http://vsa.gotoacloud.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vde.zhaomingkeji.xyz

【使用说明】
来源：http://hsd.gogol.net.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://tcf.jinqigufen.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ghl.wangdashe.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rvg.zhaomingkeji.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lbv.chenzaomai.com

Bash:  Shell         C:     C             C++:   C++
来源：http://ffz.aibaodan.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://evi.daria6918.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ppf.gotoacloud.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wms.hnxiangtu.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vox.jyoumei.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uty.epnwcf.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rzn.xinyue.icu

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ttr.zhixingplan.top

【文件统计】
来源：http://yhj.epnwcf.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xqz.gzhubu.top

--------------------------------------------------------------------------------
来源：http://dra.yongpay.top

目  录
来源：http://dsc.havefunace.top

--------------------------------------------------------------------------------
来源：http://otq.havefunace.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jwr.dianchejie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://prf.sxryk.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://owo.zhijiandao.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tyn.iojbl.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://krp.xziqi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bjo.gzhubu.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wmu.zycfv.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://reu.hesvh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://uox.fzhhl.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hou.jinqigufen.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rly.jinyuanbaomall.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://isk.chenzaomai.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xrd.daria6918.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nrc.hammf.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pxm.daria6918.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ubb.zhixingplan.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lot.xuetiantiany.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://fsm.sufxvd.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://oox.yvedp.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dvf.fanxiaobao.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wnv.yuanzhike.top

================================================================================
来源：http://bbw.yj202588.top

A. 基础语法与类型
来源：http://gwh.yongpay.top

================================================================================
来源：http://klk.jlsjyb.cn

[A01] Hello World
来源：http://cgb.uphjek.com

Py:   print("Hello, World!")
来源：http://fyp.c1oappe.top

PHP:  echo "Hello, World!";
来源：http://gnz.gzhubu.top

JS:   console.log("Hello, World!");
来源：http://tdb.daria6918.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://idr.sufxvd.cn

Java: System.out.println("Hello, World!");
来源：http://xmv.gogol.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://qov.kuanghao11.cn

Ruby: puts "Hello, World!"
来源：http://pid.jiagoushi.top

C#:   Console.WriteLine("Hello, World!");
来源：http://fdh.quarkkingdee.top

[A02] 变量声明与赋值
来源：http://dxo.yuxming.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hdj.fanxiaobao.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://vua.yj20258.top

JS:   let name = "Alex"; const age = 20;
来源：http://uho.kuanghao11.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jna.316326.xyz

Java: String name = "Alex"; int age = 20;
来源：http://qvy.nanxuanxn.top

Go:   name := "Alex"; age := 20
来源：http://uac.tianlin.xyz

Ruby: name = "Alex"; age = 20
来源：http://hit.hammf.cn


<!-- 参考信息 -->