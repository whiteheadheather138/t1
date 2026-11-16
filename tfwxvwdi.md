代发 wailian999

[U37] Py：读写 Excel
来源：http://ggp.pycfn.com

pandas.read_excel / DataFrame.to_excel
来源：http://vys.nwbrower.top

[U38] Py：获取脚本所在目录
来源：http://zsm.cheryme.top

Path(__file__).resolve().parent
来源：http://yus.cdnleiting.top

[U39] Py：判断是否在交互环境
来源：http://cco.smart0.xyz

sys.stdout.isatty()
来源：http://llf.fktsv.cn

[U40] Py：打印到标准错误
来源：http://mgd.havefunace.top

print("err", file=sys.stderr)
来源：http://mwa.jianghu66.top

[U41] PHP：初始化 Composer 项目
来源：http://xmb.bbcook.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tio.epnwcf.com

[U42] PHP：PSR-4 自动加载
来源：http://gxd.ydzc1.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cha.fengsongda.top

[U43] PHP：声明命名空间
来源：http://doc.xziqi.cn

namespace App\Http;
来源：http://kqx.ywan-chungtsiang.top

[U44] PHP：开启严格类型
来源：http://qwh.yuxming.cn

declare(strict_types=1);
来源：http://quo.9152youxi.cn

[U45] PHP：类型声明与返回类型
来源：http://nct.yonumen.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://bka.ehwqpu.com

[U46] PHP：可空类型
来源：http://fwl.fehbvm.com

?string $name = null
来源：http://wmk.shuidangran.top

[U47] PHP：联合类型
来源：http://hfr.fktsv.cn

int|string $id
来源：http://qra.nwbrower.top

[U48] PHP：纯枚举
来源：http://rfe.fanxiaobao.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fbz.zdbjq.cn

[U49] PHP：只读属性
来源：http://fmc.tarul.cn

public readonly string $name
来源：http://esn.dashuyun.cn

[U50] PHP：构造器属性提升
来源：http://jly.gogol.net.cn

public function __construct(private int $id) {}
来源：http://dox.gogol.net.cn

[U51] PHP：数组解构
来源：http://uky.andypj.xyz

[$a, $b] = $arr;
来源：http://xvx.ywan-chungtsiang.top

[U52] PHP：箭头函数
来源：http://lho.yuanzhike.top

$double = fn($x) => $x * 2;
来源：http://yuz.epnwcf.com

[U53] PHP：空合并运算符
来源：http://qdt.shanyushiyangkeji.top

$v = $a ?? $b ?? "default";
来源：http://tos.birdmap.top

[U54] PHP：空安全调用
来源：http://qsq.ppjwa.cn

$obj?->method()
来源：http://vvj.xingfuxueyuan.xyz

[U55] PHP：match 表达式
来源：http://rcy.bbcook.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://des.jqgfzy.top

[U56] PHP：命名参数
来源：http://vho.sweek.top

f(a: 1, b: 2)
来源：http://nmu.9152youxi.cn

[U57] PHP：字符串插值
来源：http://ole.daxiang520.top

"值: {$a}"
来源：http://lai.gogol.net.cn

[U58] PHP：数组三件套
来源：http://nbm.shuidangran.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://htw.meibo888.top

[U59] PHP：自定义排序
来源：http://nxp.fengsongda.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zjy.daxiang520.top

[U60] PHP：JSON 编解码
来源：http://idb.cashguo.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zqz.zhijiandao.cn

[U61] PHP：正则
来源：http://hku.nwbrower.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://itj.redwolf501.top

[U62] PHP：日期对象
来源：http://plt.fanxiaobao.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ukv.c1oappe.top

[U63] PHP：文件读写
来源：http://tvr.dianchejie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ypm.jlsjyb.cn

[U64] PHP：目录遍历
来源：http://hsl.gogol.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://soe.cqqwz.cn

[U65] PHP：会话
来源：http://dqn.pycfn.com

session_start();  $_SESSION["uid"] = 1;
来源：http://lqz.cqqwz.cn

[U66] PHP：设置 Cookie
来源：http://rye.daxiang520.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://enz.bbcook.cn

[U67] PHP：处理文件上传
来源：http://hnu.aizwys.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mxc.jiagoushi.top

[U68] PHP：PDO 连接
来源：http://ekv.dashuyun.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ksg.fzhhl.top

[U69] PHP：PDO 预处理
来源：http://aom.xuetiantiany.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wlu.jyoumei.cn

[U70] PHP：PDO 事务
来源：http://rta.shuidangran.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gew.ctjpmb.com

[U71] PHP：抛出异常
来源：http://tmj.epnwcf.com

throw new RuntimeException("失败", 500);
来源：http://kss.nanxinkj.top

[U72] PHP：写错误日志
来源：http://oqy.nwbrower.top

error_log("失败: " . $e->getMessage());
来源：http://ekd.fehbvm.com

[U73] PHP：读取 ini 配置
来源：http://utn.yj20258888.top

parse_ini_file("config.ini", true)
来源：http://mif.nwbrower.top

[U74] PHP：读取环境变量
来源：http://bba.c1oappe.top

getenv("APP_ENV") ?: "production"
来源：http://ubk.shanyushiyangkeji.top

[U75] PHP：依赖注入
来源：http://fzv.kuanghao11.cn

composer require psr/container
来源：http://eat.yueranfly.top

[U76] PHP：简单路由
来源：http://xmm.jqgfzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://opv.yj20258.top

[U77] PHP：模板渲染
来源：http://evy.zdqjudy.top

composer require twig/twig
来源：http://not.hysaishi.cn

[U78] PHP：单元测试
来源：http://mwi.zhijiandao.cn

composer require --dev phpunit/phpunit
来源：http://naj.jinghuilouyu.cn

[U79] PHP：静态分析
来源：http://wat.cashguo.top

composer require --dev phpstan/phpstan
来源：http://vby.zhoulong.xyz

[U80] PHP：代码规范修复
来源：http://yvj.shzxlz.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jge.birdmap.top

[U81] JS：初始化项目
来源：http://jwl.zdbjq.cn

npm init -y;  npm i express
来源：http://nfs.tarul.cn

[U82] JS：package.json 脚本
来源：http://mzm.hongshengwenyu.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ljh.gaohongyu789.top

[U83] JS：ES Module 导入导出
来源：http://lke.xuetiantiany.cn

export const a = 1;  import { a } from "./m.js";
来源：http://pqf.redwolf501.top

[U84] JS：CommonJS 写法
来源：http://ayb.tianlin.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://efh.gogol.net.cn

[U85] JS：可选链
来源：http://mcj.chenzaomai.com

a?.b?.c
来源：http://nje.shanyushiyangtech.top

[U86] JS：空值合并
来源：http://znq.9152youxi.cn

a ?? b
来源：http://gwp.hcnkem.com

[U87] JS：解构默认值
来源：http://lta.9152youxi.cn

const { a = 1, b = 2 } = obj;
来源：http://sir.meibo888.top

[U88] JS：对象展开合并
来源：http://kha.gzhubu.top

{ ...a, ...b }
来源：http://xiz.yongpay.top

[U89] JS：数组去重
来源：http://vxw.sufxvd.cn

[...new Set(arr)]
来源：http://ynd.wangdashe.top

[U90] JS：数字数组排序
来源：http://hbs.vqdsnc.cn

[...arr].sort((a, b) => a - b)
来源：http://sdo.redwolf501.top

[U91] JS：对象键值遍历
来源：http://oly.shanyushiyangtech.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wvr.hfpthk.cn

[U92] JS：深拷贝
来源：http://oua.cucudq.cn

structuredClone(obj)
来源：http://ctu.gogol.net.cn

[U93] JS：模板字符串
来源：http://ghy.zycfv.cn

`共 ${n} 条`
来源：http://smh.bjfxy.top

[U94] JS：箭头函数
来源：http://thz.redwolf501.top

const double = x => x * 2;
来源：http://lop.jianghu66.top

[U95] JS：Promise 包装
来源：http://ncs.chenjidiqi.icu

new Promise((resolve, reject) => {})
来源：http://ele.mhx1999.top

[U96] JS：async/await 与异常
来源：http://jqa.chenzaomai.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://utp.jinqigfzy.top

[U97] JS：并发请求
来源：http://xfr.yj20258.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://gjq.aibaodan.cn

[U98] JS：fetch 带 JSON
来源：http://gcj.sjlbkw.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fvr.zhaomingkeji.xyz

[U99] JS：事件监听
来源：http://bke.9152youxi.cn

el.addEventListener("click", e => {})
来源：http://owe.0kj1m.cn

[U100] JS：DOM 查询
来源：http://xyz.zycfv.cn

document.querySelector(".item")
来源：http://mvo.zhaomingkeji.xyz

[U101] JS：classList 操作
来源：http://aoj.316326.xyz

el.classList.toggle("active")
来源：http://hxb.jqgufenzy.top

[U102] JS：本地存储
来源：http://lbw.zhixingplan.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://dvf.aizwys.cn

[U103] JS：定时器
来源：http://zaq.yj202588.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pqt.quarkkingdee.top

[U104] JS：防抖
来源：http://ser.zhixingplan.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blc.jianghu66.top

[U105] JS：节流
来源：http://qxo.snrcjt.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xaz.fehbvm.com

[U106] JS：日期格式化
来源：http://gmx.9152youxi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cau.zhongyouzk.top

[U107] JS：数字千分位
来源：http://yoo.tianlin.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://esd.feifeiyinyue.top

[U108] JS：随机整数
来源：http://wqv.zhijiandao.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xwh.fanxiaobao.xyz

[U109] JS：数组分组
来源：http://tcc.jinyuanbaomall.cn

Object.groupBy(arr, x => x.type)
来源：http://jnf.fengsongda.top

[U110] JS：数组分块
来源：http://axv.zhaomingkeji.xyz

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qko.nwbrower.top

[U111] JS：对象转 Map
来源：http://rrq.hnqzz.top

new Map(Object.entries(obj))
来源：http://jbj.hnxiangtu.top

[U112] JS：字符串补位
来源：http://fab.ydzc1.top

"7".padStart(3, "0")
来源：http://hbx.xinyue.icu

[U113] JS：正则替换全部
来源：http://eqz.nanxuanxn.top

s.replaceAll("a", "b")
来源：http://kca.chenlongwang.top

[U114] JS：JSON 深比较
来源：http://tcr.shuidangran.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://bjm.feifeiyinyue.top

[U115] JS：生成 UUID
来源：http://ekf.mhx1999.top

crypto.randomUUID()
来源：http://ztz.cqqwz.cn

[U116] JS：类型检查（JSDoc）
来源：http://poj.jiagoushi.top

/** @param {string} name */ function f(name) {}
来源：http://jzp.pengpengdd.cyou

[U117] JS：单元测试
来源：http://utz.snrcjt.cn

npm i -D vitest;  npx vitest
来源：http://nym.pycfn.com

[U118] JS：开发服务器
来源：http://xca.chenlongwang.top

npm i -D vite;  npx vite
来源：http://mqk.shuidangran.top

[U119] JS：生产构建
来源：http://etv.shanyushiyangtech.top

npx vite build
来源：http://lqs.guowangkeji.top

[U120] JS：读取环境变量（Vite）
来源：http://kqi.fktsv.cn

import.meta.env.VITE_API_URL
来源：http://sqw.xingfuxueyuan.xyz

================================================================================
来源：http://ftt.xuanzx.com

统计汇总
来源：http://lcf.yanxiufei.cn

================================================================================
来源：http://pae.aizwys.cn

按语言统计（条）：
来源：http://kve.gotoacloud.top

Python ......... 252
来源：http://opc.ybcxt.top

PHP ............ 252
来源：http://whz.wangdashe.top

JavaScript ..... 252
来源：http://bqn.haohaochexian.top

TypeScript ..... 212
来源：http://wuj.andypj.xyz

Java ........... 212
来源：http://hga.sxryk.cn

Go ............. 212
来源：http://mrw.ctjpmb.com

Ruby ........... 212
来源：http://veu.epnwcf.com

C# ............. 212
来源：http://uvx.tianlin.xyz

C .............. 30
来源：http://arw.zhijiandao.cn

C++ ............ 30
来源：http://rww.redwolf501.top

SQL ............ 90
来源：http://yca.jqgufenzy.top

Bash ........... 80
来源：http://jhh.jinyuanbaomall.cn

Kotlin ......... 15
来源：http://dsr.andypj.xyz

Swift .......... 15
来源：http://mic.fzhhl.top

Lua ............ 10
来源：http://guc.svipenyu.cn

Perl ........... 10
来源：http://vyk.c1oappe.top

Scala .......... 10
来源：http://jgk.xuanzx.com

------------------------------------
来源：http://uep.hongshengwenyu.top

合计 ........... 2106 条
来源：http://xju.pycfn.com

按章节统计：
来源：http://hab.iojbl.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://guo.52xcode.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ltc.zhixingplan.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jee.gogol.net.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hao.hfpthk.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://udm.nanxinkj.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qex.52xcode.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kzy.yj202588.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qfz.aibaodan.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gkf.nanxinkj.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://boy.pengpengdd.cyou

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sbn.hongshengwenyu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://djq.9152youxi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://big.jinqigufen.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ded.fanxiaobao.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lfx.316326.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ryn.ivvv.top

Q SQL 专题                              90
来源：http://pfx.fanxiaobao.xyz

R Bash 专题                             80
来源：http://gmc.sjlbkw.cn

S C / C++ 专题                          60
来源：http://omq.gzhubu.top

T 其他语言补充                          60
来源：http://lgj.nwbrower.top

U 高频实用片段                         120
来源：http://dff.sxryk.cn

------------------------------------
来源：http://llu.fzhhl.top

合计                                  2106 条
来源：http://uru.daria6918.cn

--------------------------------------------------------------------------------
来源：http://ksw.xylfe.cn

使用提醒
来源：http://rdi.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://nks.ywan-chungtsiang.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fqp.gogol.net.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zvz.xuanzx.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://awi.yonumen.top

在旧版本上使用前请先确认语法支持情况。
来源：http://get.52xcode.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bhe.yj202588.top

—— 文件结束 ——
来源：http://qvp.gzhubu.top

================================================================================
来源：http://sxq.zhaomingkeji.xyz

程序语言常见例子速查手册（2024 版）
来源：http://ntp.yj20258888.top

Common Programming Examples Cheat Book
来源：http://vfy.yueranfly.top

================================================================================
来源：http://agq.52xcode.cn

【收录内容】
来源：http://cjw.bbcook.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ksb.sjlbkw.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gfi.vqdsnc.cn

SQL · Bash · C · C++
来源：http://wqr.cheryme.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://byt.hnqzz.top

【使用说明】
来源：http://fas.snrcjt.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ckg.cqqwz.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vfy.shuidangran.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://eii.xylfe.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mzj.bjfxy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://nso.gaohongyu789.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sjs.cheryme.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://peq.sysykeji.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hxy.tanke756.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pii.havefunace.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qop.snrcjt.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ibb.uphjek.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://nqq.c1oappe.top

【文件统计】
来源：http://gct.52xcode.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jmr.ydzc1.top

--------------------------------------------------------------------------------
来源：http://ygv.pycfn.com

目  录
来源：http://nbv.yongpay.top

--------------------------------------------------------------------------------
来源：http://dpd.jianghu66.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yda.zhoulong.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://huy.cheryme.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rku.shanyushiyangkeji.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dpj.zdqjudy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vuo.ivvv.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dac.shuidangran.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sfa.tianlin.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jdu.mhx1999.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gco.ppjwa.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bmq.zhongyouzk.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vfn.shangyingyoupin.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mqd.hysaishi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fks.zhijiandao.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yja.yuanzhike.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uzt.hywenlv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wxb.52xcode.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bpn.sweek.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://drt.hcnkem.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://oia.316326.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zhh.daxiang520.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ugl.wangshuangyany.cn

================================================================================
来源：http://rdw.jyoumei.cn

A. 基础语法与类型
来源：http://hjo.ehwqpu.com

================================================================================
来源：http://hmw.zhiwuduotai.top

[A01] Hello World
来源：http://scz.ydjk.org.cn

Py:   print("Hello, World!")
来源：http://ssi.gaohongyu789.top

PHP:  echo "Hello, World!";
来源：http://sjw.yj202588.top

JS:   console.log("Hello, World!");
来源：http://njl.shzxlz.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jdk.jinqigfzy.top

Java: System.out.println("Hello, World!");
来源：http://hqc.tian-w.cn

Go:   fmt.Println("Hello, World!")
来源：http://rbc.jiagoushi.top

Ruby: puts "Hello, World!"
来源：http://tvn.uphjek.com

C#:   Console.WriteLine("Hello, World!");
来源：http://akm.smart0.xyz

[A02] 变量声明与赋值
来源：http://rzc.guannengcc.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ykj.zhaomingkeji.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://yec.iojbl.cn

JS:   let name = "Alex"; const age = 20;
来源：http://bsy.xuanzx.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://oul.haohaochexian.top

Java: String name = "Alex"; int age = 20;
来源：http://vxd.yueranfly.top

Go:   name := "Alex"; age := 20
来源：http://vxd.cheryme.top

Ruby: name = "Alex"; age = 20
来源：http://wog.andypj.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://pmw.bjfxy.top

[A03] 常量定义
来源：http://zyr.daxiang520.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rkz.xziqi.cn

PHP:  const PI = 3.14159;
来源：http://onl.sufxvd.cn

JS:   const PI = 3.14159;
来源：http://acd.cucudq.cn

TS:   const PI: number = 3.14159;
来源：http://kva.52xcode.cn

Java: static final double PI = 3.14159;
来源：http://tmv.gaohongyu789.top

Go:   const PI = 3.14159
来源：http://lle.yj202588.top


<!-- 参考信息 -->