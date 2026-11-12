代发 wailian999

[U37] Py：读写 Excel
来源：http://xei.gogol.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hof.hammf.cn

[U38] Py：获取脚本所在目录
来源：http://hzj.snrcjt.cn

Path(__file__).resolve().parent
来源：http://ocx.yueranfly.top

[U39] Py：判断是否在交互环境
来源：http://msk.wangshuangyany.cn

sys.stdout.isatty()
来源：http://cky.cqqwz.cn

[U40] Py：打印到标准错误
来源：http://peu.zhengqikj.top

print("err", file=sys.stderr)
来源：http://epa.sysykeji.top

[U41] PHP：初始化 Composer 项目
来源：http://yhm.shangyingyoupin.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ath.jianghu66.top

[U42] PHP：PSR-4 自动加载
来源：http://emv.smart0.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tvd.jqgufenzy.top

[U43] PHP：声明命名空间
来源：http://rqq.redwolf501.top

namespace App\Http;
来源：http://iyo.aibaodan.cn

[U44] PHP：开启严格类型
来源：http://rrq.0kj1m.cn

declare(strict_types=1);
来源：http://qri.tarul.cn

[U45] PHP：类型声明与返回类型
来源：http://ycj.iojbl.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jtw.fengsongda.top

[U46] PHP：可空类型
来源：http://yvy.sufxvd.cn

?string $name = null
来源：http://yxp.hongshengwenyu.top

[U47] PHP：联合类型
来源：http://vum.hesvh.cn

int|string $id
来源：http://qow.bjfxy.top

[U48] PHP：纯枚举
来源：http://lda.sweek.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bum.zhijiandao.cn

[U49] PHP：只读属性
来源：http://kqs.jlsjyb.cn

public readonly string $name
来源：http://zbg.daxiang520.top

[U50] PHP：构造器属性提升
来源：http://nyo.aizwys.cn

public function __construct(private int $id) {}
来源：http://yik.hywenlv.cn

[U51] PHP：数组解构
来源：http://eae.tarul.cn

[$a, $b] = $arr;
来源：http://hlh.fktsv.cn

[U52] PHP：箭头函数
来源：http://sam.andypj.xyz

$double = fn($x) => $x * 2;
来源：http://dtn.ppjwa.cn

[U53] PHP：空合并运算符
来源：http://bhv.nanxinkj.top

$v = $a ?? $b ?? "default";
来源：http://sbp.zdbjq.cn

[U54] PHP：空安全调用
来源：http://vpp.meibo888.top

$obj?->method()
来源：http://pjs.shangyingyoupin.top

[U55] PHP：match 表达式
来源：http://jkb.guannengcc.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mks.ydjk.org.cn

[U56] PHP：命名参数
来源：http://wts.shuidangran.top

f(a: 1, b: 2)
来源：http://xco.zhongyouzk.top

[U57] PHP：字符串插值
来源：http://xyh.shanyushiyangtech.top

"值: {$a}"
来源：http://alf.shzxlz.cn

[U58] PHP：数组三件套
来源：http://njl.gotoacloud.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ppz.zhoulong.xyz

[U59] PHP：自定义排序
来源：http://fer.tian-w.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tjr.yfazqb.com

[U60] PHP：JSON 编解码
来源：http://oxk.ydjk.org.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uvp.nwbrower.top

[U61] PHP：正则
来源：http://oqi.cashguo.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://awt.hnqzz.top

[U62] PHP：日期对象
来源：http://lum.yj20258.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://clh.xylfe.cn

[U63] PHP：文件读写
来源：http://xrl.cqqwz.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nsw.xuanzx.com

[U64] PHP：目录遍历
来源：http://wlm.jinqigfzy.top

glob("dir/*.php");  scandir("dir");
来源：http://tdu.shanyushiyangkeji.top

[U65] PHP：会话
来源：http://jej.0kj1m.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tca.svipenyu.cn

[U66] PHP：设置 Cookie
来源：http://mwc.tarul.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gge.nanxuanxn.top

[U67] PHP：处理文件上传
来源：http://fjj.epnwcf.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yyp.gzhubu.top

[U68] PHP：PDO 连接
来源：http://wzu.quarkkingdee.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xrt.hysaishi.cn

[U69] PHP：PDO 预处理
来源：http://vjg.nwbrower.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://psj.redwolf501.top

[U70] PHP：PDO 事务
来源：http://aum.nwbrower.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kqp.yfazqb.com

[U71] PHP：抛出异常
来源：http://yjc.quarkkingdee.top

throw new RuntimeException("失败", 500);
来源：http://ssn.hysaishi.cn

[U72] PHP：写错误日志
来源：http://kxs.cqqwz.cn

error_log("失败: " . $e->getMessage());
来源：http://xhr.cqqwz.cn

[U73] PHP：读取 ini 配置
来源：http://ikg.iojbl.cn

parse_ini_file("config.ini", true)
来源：http://fxo.dashuyun.cn

[U74] PHP：读取环境变量
来源：http://mlu.hysaishi.cn

getenv("APP_ENV") ?: "production"
来源：http://isp.yongpay.top

[U75] PHP：依赖注入
来源：http://fzn.chenjidiqi.icu

composer require psr/container
来源：http://gau.hesvh.cn

[U76] PHP：简单路由
来源：http://dmy.zycfv.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://iql.hcnkem.com

[U77] PHP：模板渲染
来源：http://tke.bjfxy.top

composer require twig/twig
来源：http://fce.fzhhl.top

[U78] PHP：单元测试
来源：http://mqx.0kj1m.cn

composer require --dev phpunit/phpunit
来源：http://irg.mhx1999.top

[U79] PHP：静态分析
来源：http://kbt.pengpengdd.cyou

composer require --dev phpstan/phpstan
来源：http://hbb.xylfe.cn

[U80] PHP：代码规范修复
来源：http://cbc.316326.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://lbu.yj20258888.top

[U81] JS：初始化项目
来源：http://ykf.hysaishi.cn

npm init -y;  npm i express
来源：http://lyf.zhoulong.xyz

[U82] JS：package.json 脚本
来源：http://nty.sweek.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jwt.vehdjk.com

[U83] JS：ES Module 导入导出
来源：http://dwv.jinqigufen.top

export const a = 1;  import { a } from "./m.js";
来源：http://xqd.ivvv.top

[U84] JS：CommonJS 写法
来源：http://bho.wangshuangyany.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cau.316326.xyz

[U85] JS：可选链
来源：http://jym.smart0.xyz

a?.b?.c
来源：http://lly.yj20258.top

[U86] JS：空值合并
来源：http://zhf.sweek.top

a ?? b
来源：http://uyw.sysykeji.top

[U87] JS：解构默认值
来源：http://vxl.xinyue.icu

const { a = 1, b = 2 } = obj;
来源：http://qjd.wangdashe.top

[U88] JS：对象展开合并
来源：http://ezs.zhengqikj.top

{ ...a, ...b }
来源：http://doj.sweek.top

[U89] JS：数组去重
来源：http://mbz.sxryk.cn

[...new Set(arr)]
来源：http://urh.shanyushiyangkeji.top

[U90] JS：数字数组排序
来源：http://grx.cheryme.top

[...arr].sort((a, b) => a - b)
来源：http://bdh.xuetiantiany.cn

[U91] JS：对象键值遍历
来源：http://uli.jinghuilouyu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://aez.haohaochexian.top

[U92] JS：深拷贝
来源：http://qzf.52xcode.cn

structuredClone(obj)
来源：http://rwc.hesvh.cn

[U93] JS：模板字符串
来源：http://hlg.shanyushiyangtech.top

`共 ${n} 条`
来源：http://kyg.iojbl.cn

[U94] JS：箭头函数
来源：http://mfy.zhoulong.xyz

const double = x => x * 2;
来源：http://bip.daxiang520.top

[U95] JS：Promise 包装
来源：http://bch.xinyue.icu

new Promise((resolve, reject) => {})
来源：http://gil.nwbrower.top

[U96] JS：async/await 与异常
来源：http://irm.gotoacloud.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tss.vehdjk.com

[U97] JS：并发请求
来源：http://ntr.shanyushiyangkeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ixe.jlsjyb.cn

[U98] JS：fetch 带 JSON
来源：http://gxb.ydzc1.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://izr.vqdsnc.cn

[U99] JS：事件监听
来源：http://ewu.andypj.xyz

el.addEventListener("click", e => {})
来源：http://mqd.wangshuangyany.cn

[U100] JS：DOM 查询
来源：http://xye.nanxuanxn.top

document.querySelector(".item")
来源：http://ubm.9152youxi.cn

[U101] JS：classList 操作
来源：http://zwr.cashguo.top

el.classList.toggle("active")
来源：http://qzk.gaohongyu789.top

[U102] JS：本地存储
来源：http://krz.mhx1999.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://kvm.chenlongwang.top

[U103] JS：定时器
来源：http://roi.shanyushiyangtech.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://naf.hywenlv.cn

[U104] JS：防抖
来源：http://maw.cucudq.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://shk.jinqigfzy.top

[U105] JS：节流
来源：http://xmc.chenjidiqi.icu

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qgr.yfazqb.com

[U106] JS：日期格式化
来源：http://pbk.chenjidiqi.icu

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://aty.xziqi.cn

[U107] JS：数字千分位
来源：http://xtg.shuidangran.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lxo.jiagoushi.top

[U108] JS：随机整数
来源：http://dcs.guannengcc.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tix.chenlongwang.top

[U109] JS：数组分组
来源：http://jbl.dianchejie.cn

Object.groupBy(arr, x => x.type)
来源：http://bxv.quarkkingdee.top

[U110] JS：数组分块
来源：http://dzv.yueranfly.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://esv.zhoulong.xyz

[U111] JS：对象转 Map
来源：http://hcz.daria6918.cn

new Map(Object.entries(obj))
来源：http://lte.chenjidiqi.icu

[U112] JS：字符串补位
来源：http://fvz.sjlbkw.cn

"7".padStart(3, "0")
来源：http://fjj.jinqigufen.top

[U113] JS：正则替换全部
来源：http://xiq.vehdjk.com

s.replaceAll("a", "b")
来源：http://tav.guannengcc.top

[U114] JS：JSON 深比较
来源：http://nrh.yj202588.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://cna.gaohongyu789.top

[U115] JS：生成 UUID
来源：http://fuf.sysykeji.top

crypto.randomUUID()
来源：http://ret.cqqwz.cn

[U116] JS：类型检查（JSDoc）
来源：http://emb.zdqjudy.top

/** @param {string} name */ function f(name) {}
来源：http://vvn.guannengcc.top

[U117] JS：单元测试
来源：http://uzy.sjlbkw.cn

npm i -D vitest;  npx vitest
来源：http://okx.yj20258.top

[U118] JS：开发服务器
来源：http://ssp.zhoulong.xyz

npm i -D vite;  npx vite
来源：http://exu.jinghuilouyu.cn

[U119] JS：生产构建
来源：http://pvu.316326.xyz

npx vite build
来源：http://scp.ydzc1.top

[U120] JS：读取环境变量（Vite）
来源：http://ybe.gaohongyu789.top

import.meta.env.VITE_API_URL
来源：http://mxf.yonumen.top

================================================================================
来源：http://hkh.jyoumei.cn

统计汇总
来源：http://shh.jyoumei.cn

================================================================================
来源：http://lcu.mhx1999.top

按语言统计（条）：
来源：http://xjq.birdmap.top

Python ......... 252
来源：http://btg.hnxiangtu.top

PHP ............ 252
来源：http://oke.shanyushiyangtech.top

JavaScript ..... 252
来源：http://xhi.ybcxt.top

TypeScript ..... 212
来源：http://olc.jyoumei.cn

Java ........... 212
来源：http://hik.zhijiandao.cn

Go ............. 212
来源：http://myi.nanxuanxn.top

Ruby ........... 212
来源：http://dek.xingfuxueyuan.xyz

C# ............. 212
来源：http://feo.cdnleiting.top

C .............. 30
来源：http://zmh.xuanzx.com

C++ ............ 30
来源：http://qiq.hywenlv.cn

SQL ............ 90
来源：http://pjb.tian-w.cn

Bash ........... 80
来源：http://mrp.fzhhl.top

Kotlin ......... 15
来源：http://spb.svipenyu.cn

Swift .......... 15
来源：http://zdp.nanxuanxn.top

Lua ............ 10
来源：http://sod.xziqi.cn

Perl ........... 10
来源：http://imb.yj20258.top

Scala .......... 10
来源：http://wwc.feifeiyinyue.top

------------------------------------
来源：http://axa.jqgfzy.top

合计 ........... 2106 条
来源：http://wwg.cashguo.top

按章节统计：
来源：http://bhi.52xcode.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://btf.uphjek.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jbu.zhongyouzk.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qho.jinghuilouyu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kjg.epnwcf.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://aed.ybcxt.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://psz.gogol.net.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bup.meibo888.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vtw.hongshengwenyu.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wvn.c1oappe.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nlb.fzhhl.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vxg.gotoacloud.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ilc.zhongyouzk.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yab.ydjk.org.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cwe.feifeiyinyue.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wpx.redwolf501.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mza.zhixingplan.top

Q SQL 专题                              90
来源：http://nxy.daria6918.cn

R Bash 专题                             80
来源：http://jxi.zdbjq.cn

S C / C++ 专题                          60
来源：http://bvp.zhoulong.xyz

T 其他语言补充                          60
来源：http://dwt.c1oappe.top

U 高频实用片段                         120
来源：http://fdf.zhengqikj.top

------------------------------------
来源：http://yvo.fehbvm.com

合计                                  2106 条
来源：http://ptf.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://grq.zdqjudy.top

使用提醒
来源：http://qkh.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://inh.hywenlv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bqq.epnwcf.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vbt.zdbjq.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://doc.jianghu66.top

在旧版本上使用前请先确认语法支持情况。
来源：http://egg.jinqigfzy.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dmf.gogol.net.cn

—— 文件结束 ——
来源：http://gsj.sysykeji.top

================================================================================
来源：http://job.jinqigufen.top

程序语言常见例子速查手册（2024 版）
来源：http://ohw.zhaomingkeji.xyz

Common Programming Examples Cheat Book
来源：http://lww.xziqi.cn

================================================================================
来源：http://rms.shangyingyoupin.top

【收录内容】
来源：http://orq.fehbvm.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://yed.ybcxt.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ofj.ctjpmb.com

SQL · Bash · C · C++
来源：http://geb.ywan-chungtsiang.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://grb.gogol.net.cn

【使用说明】
来源：http://jya.smart0.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://zet.zhiwuduotai.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ajj.xylfe.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rjq.gzhubu.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tpr.jiagoushi.top

Bash:  Shell         C:     C             C++:   C++
来源：http://wvm.chenzaomai.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rda.andypj.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://sbl.jinyuanbaomall.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ssw.shanyushiyangkeji.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xxb.yanxiufei.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pij.quarkkingdee.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qyp.yanxiufei.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ayn.sysykeji.top

【文件统计】
来源：http://ljy.mhx1999.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pfv.xuanzx.com

--------------------------------------------------------------------------------
来源：http://foy.jinqigufen.top

目  录
来源：http://haj.cucudq.cn

--------------------------------------------------------------------------------
来源：http://rrm.zhijiandao.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ans.pengpengdd.cyou

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://icj.havefunace.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://jpe.yongpay.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zzl.xuetiantiany.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cbe.hnqzz.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://adk.birdmap.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vyn.vqdsnc.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qqy.hnxiangtu.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://umy.9152youxi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zzz.hnxiangtu.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wds.bjfxy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xty.sjlbkw.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tkw.haohaochexian.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://szl.yj20258888.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ztm.fengsongda.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gms.nanxuanxn.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wbc.pycfn.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://zjm.c1oappe.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gll.mhx1999.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://sxr.hfpthk.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ogc.gaohongyu789.top

================================================================================
来源：http://wsn.xuetiantiany.cn

A. 基础语法与类型
来源：http://clv.gogol.net.cn

================================================================================
来源：http://syi.jlsjyb.cn

[A01] Hello World
来源：http://wra.yonumen.top

Py:   print("Hello, World!")
来源：http://bjh.jiagoushi.top

PHP:  echo "Hello, World!";
来源：http://ioi.ybcxt.top

JS:   console.log("Hello, World!");
来源：http://qyp.shzxlz.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vko.zhixingplan.top

Java: System.out.println("Hello, World!");
来源：http://ifx.hysaishi.cn

Go:   fmt.Println("Hello, World!")
来源：http://jbo.zhijiandao.cn

Ruby: puts "Hello, World!"
来源：http://vid.316326.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://fbz.daxiang520.top

[A02] 变量声明与赋值
来源：http://ynd.feifeiyinyue.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://djj.tian-w.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://kpx.chenzaomai.com

JS:   let name = "Alex"; const age = 20;
来源：http://now.pycfn.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mrm.jinqigufen.top

Java: String name = "Alex"; int age = 20;
来源：http://lad.epnwcf.com

Go:   name := "Alex"; age := 20
来源：http://kox.daria6918.cn

Ruby: name = "Alex"; age = 20
来源：http://pzk.birdmap.top

C#:   string name = "Alex"; int age = 20;
来源：http://phe.andypj.xyz

[A03] 常量定义
来源：http://rmo.hcnkem.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jrl.daxiang520.top

PHP:  const PI = 3.14159;
来源：http://uhu.hywenlv.cn

JS:   const PI = 3.14159;
来源：http://exg.zhoulong.xyz

TS:   const PI: number = 3.14159;
来源：http://slf.yvedp.cn

Java: static final double PI = 3.14159;
来源：http://jvj.fanxiaobao.xyz

Go:   const PI = 3.14159
来源：http://riv.yueranfly.top


<!-- 参考信息 -->