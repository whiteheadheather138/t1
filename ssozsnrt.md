代发 wailian999

[U31] Py：单测
来源：http://rad.gotoacloud.top

python -m pytest -q
来源：http://msr.ctjpmb.com

[U32] Py：代码格式化
来源：http://wty.guannengcc.top

ruff format . && ruff check --fix .
来源：http://xqs.yj202588.top

[U33] Py：打包发布
来源：http://iwa.fengsongda.top

python -m build  （依赖 pyproject.toml）
来源：http://osw.jiagoushi.top

[U34] Py：判断编码
来源：http://nbw.gaohongyu789.top

chardet.detect(raw)
来源：http://ref.xylfe.cn

[U35] Py：发送邮件
来源：http://wwp.xuanzx.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kgx.zhoulong.xyz

[U36] Py：定时任务
来源：http://vfp.hnxiangtu.top

schedule.every(10).minutes.do(job)
来源：http://gkb.ydzc1.top

[U37] Py：读写 Excel
来源：http://ein.zhongyouzk.top

pandas.read_excel / DataFrame.to_excel
来源：http://nhi.redwolf501.top

[U38] Py：获取脚本所在目录
来源：http://ysz.xylfe.cn

Path(__file__).resolve().parent
来源：http://jxm.ywan-chungtsiang.top

[U39] Py：判断是否在交互环境
来源：http://irm.hammf.cn

sys.stdout.isatty()
来源：http://iwv.guowangkeji.top

[U40] Py：打印到标准错误
来源：http://rei.xuetiantiany.cn

print("err", file=sys.stderr)
来源：http://jrc.redwolf501.top

[U41] PHP：初始化 Composer 项目
来源：http://etf.zhongyouzk.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ptc.tianlin.xyz

[U42] PHP：PSR-4 自动加载
来源：http://tgj.gaohongyu789.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kqg.hywenlv.cn

[U43] PHP：声明命名空间
来源：http://zss.guowangkeji.top

namespace App\Http;
来源：http://hyz.9152youxi.cn

[U44] PHP：开启严格类型
来源：http://idl.tarul.cn

declare(strict_types=1);
来源：http://rls.iojbl.cn

[U45] PHP：类型声明与返回类型
来源：http://jjk.cucudq.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://okx.nanxuanxn.top

[U46] PHP：可空类型
来源：http://jsq.shzxlz.cn

?string $name = null
来源：http://ynl.chenzaomai.com

[U47] PHP：联合类型
来源：http://bee.xylfe.cn

int|string $id
来源：http://fyp.hammf.cn

[U48] PHP：纯枚举
来源：http://moc.fehbvm.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://urr.havefunace.top

[U49] PHP：只读属性
来源：http://kad.tian-w.cn

public readonly string $name
来源：http://cfb.jinyuanbaomall.cn

[U50] PHP：构造器属性提升
来源：http://pzx.jqgfzy.top

public function __construct(private int $id) {}
来源：http://qnd.mhx1999.top

[U51] PHP：数组解构
来源：http://bew.hongshengwenyu.top

[$a, $b] = $arr;
来源：http://oyl.jinghuilouyu.cn

[U52] PHP：箭头函数
来源：http://fcu.cdnleiting.top

$double = fn($x) => $x * 2;
来源：http://iwk.sysykeji.top

[U53] PHP：空合并运算符
来源：http://cej.sjlbkw.cn

$v = $a ?? $b ?? "default";
来源：http://kkp.ywan-chungtsiang.top

[U54] PHP：空安全调用
来源：http://anf.jqgufenzy.top

$obj?->method()
来源：http://iba.316326.xyz

[U55] PHP：match 表达式
来源：http://gal.epnwcf.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://owp.hnqzz.top

[U56] PHP：命名参数
来源：http://omc.hywenlv.cn

f(a: 1, b: 2)
来源：http://vli.gogol.net.cn

[U57] PHP：字符串插值
来源：http://zmp.jqgufenzy.top

"值: {$a}"
来源：http://tev.zhixingplan.top

[U58] PHP：数组三件套
来源：http://eeh.fzhhl.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xjj.kuanghao11.cn

[U59] PHP：自定义排序
来源：http://zak.sysykeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yun.52xcode.cn

[U60] PHP：JSON 编解码
来源：http://jbi.ybcxt.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qix.havefunace.top

[U61] PHP：正则
来源：http://mrn.zdbjq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ucn.jinghuilouyu.cn

[U62] PHP：日期对象
来源：http://wyv.birdmap.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cdi.hfpthk.cn

[U63] PHP：文件读写
来源：http://cgg.fehbvm.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://idr.sjlbkw.cn

[U64] PHP：目录遍历
来源：http://lgd.hammf.cn

glob("dir/*.php");  scandir("dir");
来源：http://zvx.yongpay.top

[U65] PHP：会话
来源：http://bdt.xuanzx.com

session_start();  $_SESSION["uid"] = 1;
来源：http://piv.chenzaomai.com

[U66] PHP：设置 Cookie
来源：http://ysm.316326.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kvy.yj202588.top

[U67] PHP：处理文件上传
来源：http://ejt.yj20258.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tsr.epnwcf.com

[U68] PHP：PDO 连接
来源：http://ozo.zycfv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bnv.smart0.xyz

[U69] PHP：PDO 预处理
来源：http://lrv.hcnkem.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uxf.cqqwz.cn

[U70] PHP：PDO 事务
来源：http://aqn.nanxuanxn.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dtd.wangdashe.top

[U71] PHP：抛出异常
来源：http://quu.yj20258.top

throw new RuntimeException("失败", 500);
来源：http://mvg.zdbjq.cn

[U72] PHP：写错误日志
来源：http://str.xuanzx.com

error_log("失败: " . $e->getMessage());
来源：http://ukw.xziqi.cn

[U73] PHP：读取 ini 配置
来源：http://tlg.jianghu66.top

parse_ini_file("config.ini", true)
来源：http://mgo.gaohongyu789.top

[U74] PHP：读取环境变量
来源：http://vgo.ehwqpu.com

getenv("APP_ENV") ?: "production"
来源：http://fou.cqqwz.cn

[U75] PHP：依赖注入
来源：http://lbv.aizwys.cn

composer require psr/container
来源：http://qch.yvedp.cn

[U76] PHP：简单路由
来源：http://xbs.dashuyun.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bph.shanyushiyangtech.top

[U77] PHP：模板渲染
来源：http://qao.yj20258.top

composer require twig/twig
来源：http://bpn.yangfankeji.com

[U78] PHP：单元测试
来源：http://uja.pengpengdd.cyou

composer require --dev phpunit/phpunit
来源：http://fly.shzxlz.cn

[U79] PHP：静态分析
来源：http://wtr.birdmap.top

composer require --dev phpstan/phpstan
来源：http://jsf.ehwqpu.com

[U80] PHP：代码规范修复
来源：http://pvb.yongpay.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://klt.aizwys.cn

[U81] JS：初始化项目
来源：http://gvh.aizwys.cn

npm init -y;  npm i express
来源：http://vkp.jianghu66.top

[U82] JS：package.json 脚本
来源：http://hdx.daxiang520.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mzb.iojbl.cn

[U83] JS：ES Module 导入导出
来源：http://mut.zhongyouzk.top

export const a = 1;  import { a } from "./m.js";
来源：http://doy.xylfe.cn

[U84] JS：CommonJS 写法
来源：http://gbh.gzhubu.top

module.exports = { a };  const { a } = require("./m");
来源：http://tid.vqdsnc.cn

[U85] JS：可选链
来源：http://evb.sweek.top

a?.b?.c
来源：http://blu.xuetiantiany.cn

[U86] JS：空值合并
来源：http://zew.jinyuanbaomall.cn

a ?? b
来源：http://irn.zhaomingkeji.xyz

[U87] JS：解构默认值
来源：http://bhr.9152youxi.cn

const { a = 1, b = 2 } = obj;
来源：http://btr.yfazqb.com

[U88] JS：对象展开合并
来源：http://lrv.xingfuxueyuan.xyz

{ ...a, ...b }
来源：http://lhw.yuxming.cn

[U89] JS：数组去重
来源：http://ojm.ybcxt.top

[...new Set(arr)]
来源：http://peu.zhijiandao.cn

[U90] JS：数字数组排序
来源：http://lsa.shuidangran.top

[...arr].sort((a, b) => a - b)
来源：http://hso.cucudq.cn

[U91] JS：对象键值遍历
来源：http://yep.epnwcf.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xqq.yangfankeji.com

[U92] JS：深拷贝
来源：http://wsz.fanxiaobao.xyz

structuredClone(obj)
来源：http://uba.xylfe.cn

[U93] JS：模板字符串
来源：http://eot.zhijiandao.cn

`共 ${n} 条`
来源：http://ajx.jlsjyb.cn

[U94] JS：箭头函数
来源：http://dua.ivvv.top

const double = x => x * 2;
来源：http://nze.yj20258.top

[U95] JS：Promise 包装
来源：http://lll.jqgfzy.top

new Promise((resolve, reject) => {})
来源：http://hst.cashguo.top

[U96] JS：async/await 与异常
来源：http://tmt.52xcode.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qko.tianlin.xyz

[U97] JS：并发请求
来源：http://apz.yongpay.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://bis.aibaodan.cn

[U98] JS：fetch 带 JSON
来源：http://csw.cdnleiting.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://oxn.jinghuilouyu.cn

[U99] JS：事件监听
来源：http://wsp.cashguo.top

el.addEventListener("click", e => {})
来源：http://iti.jiagoushi.top

[U100] JS：DOM 查询
来源：http://ara.hongshengwenyu.top

document.querySelector(".item")
来源：http://mos.hywenlv.cn

[U101] JS：classList 操作
来源：http://qvn.ehwqpu.com

el.classList.toggle("active")
来源：http://pqe.hesvh.cn

[U102] JS：本地存储
来源：http://stl.jqgfzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://wyj.0kj1m.cn

[U103] JS：定时器
来源：http://ian.hnxiangtu.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://iyd.c1oappe.top

[U104] JS：防抖
来源：http://aun.ybcxt.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://frk.svipenyu.cn

[U105] JS：节流
来源：http://auh.sysykeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rfg.sysykeji.top

[U106] JS：日期格式化
来源：http://zqo.havefunace.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vjp.jiagoushi.top

[U107] JS：数字千分位
来源：http://uwc.hongshengwenyu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uiq.shangyingyoupin.top

[U108] JS：随机整数
来源：http://dkm.haohaochexian.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://loy.hnxiangtu.top

[U109] JS：数组分组
来源：http://jhg.daria6918.cn

Object.groupBy(arr, x => x.type)
来源：http://cjd.smart0.xyz

[U110] JS：数组分块
来源：http://tub.ehwqpu.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nto.sjlbkw.cn

[U111] JS：对象转 Map
来源：http://obz.hesvh.cn

new Map(Object.entries(obj))
来源：http://jlc.shanyushiyangkeji.top

[U112] JS：字符串补位
来源：http://vza.zhoulong.xyz

"7".padStart(3, "0")
来源：http://tjw.svipenyu.cn

[U113] JS：正则替换全部
来源：http://pol.pengpengdd.cyou

s.replaceAll("a", "b")
来源：http://ghi.guannengcc.top

[U114] JS：JSON 深比较
来源：http://dqg.jqgfzy.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rvw.redwolf501.top

[U115] JS：生成 UUID
来源：http://ydo.hysaishi.cn

crypto.randomUUID()
来源：http://fwd.redwolf501.top

[U116] JS：类型检查（JSDoc）
来源：http://niw.hfpthk.cn

/** @param {string} name */ function f(name) {}
来源：http://bti.tarul.cn

[U117] JS：单元测试
来源：http://box.chenjidiqi.icu

npm i -D vitest;  npx vitest
来源：http://mlu.zhongyouzk.top

[U118] JS：开发服务器
来源：http://kdt.xziqi.cn

npm i -D vite;  npx vite
来源：http://bcs.shanyushiyangkeji.top

[U119] JS：生产构建
来源：http://tmb.iojbl.cn

npx vite build
来源：http://ffm.zhongyouzk.top

[U120] JS：读取环境变量（Vite）
来源：http://hai.fanxiaobao.xyz

import.meta.env.VITE_API_URL
来源：http://rjw.shzxlz.cn

================================================================================
来源：http://sti.havefunace.top

统计汇总
来源：http://ujh.yj20258.top

================================================================================
来源：http://gdr.shanyushiyangtech.top

按语言统计（条）：
来源：http://iuj.haohaochexian.top

Python ......... 252
来源：http://xqn.tianlin.xyz

PHP ............ 252
来源：http://tiw.smart0.xyz

JavaScript ..... 252
来源：http://oje.zhaomingkeji.xyz

TypeScript ..... 212
来源：http://znp.vqdsnc.cn

Java ........... 212
来源：http://cbx.zhaomingkeji.xyz

Go ............. 212
来源：http://bqi.hfpthk.cn

Ruby ........... 212
来源：http://juh.jqgufenzy.top

C# ............. 212
来源：http://nal.shanyushiyangtech.top

C .............. 30
来源：http://cuq.wangdashe.top

C++ ............ 30
来源：http://irp.uphjek.com

SQL ............ 90
来源：http://qra.havefunace.top

Bash ........... 80
来源：http://aun.yfazqb.com

Kotlin ......... 15
来源：http://lof.ywan-chungtsiang.top

Swift .......... 15
来源：http://gmj.aizwys.cn

Lua ............ 10
来源：http://btm.yvedp.cn

Perl ........... 10
来源：http://ftf.haohaochexian.top

Scala .......... 10
来源：http://rpb.shanyushiyangtech.top

------------------------------------
来源：http://etw.chenlongwang.top

合计 ........... 2106 条
来源：http://nhk.fktsv.cn

按章节统计：
来源：http://llw.wangshuangyany.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rqj.birdmap.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bnh.pycfn.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qzm.jinyuanbaomall.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qbl.cheryme.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cjd.dashuyun.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wwu.jinqigfzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zip.jqgufenzy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://azp.sxryk.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hnu.uphjek.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://itf.birdmap.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fxx.ppjwa.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jej.aibaodan.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wog.jyoumei.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ihr.cheryme.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xkf.jinqigufen.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wyd.tanke756.top

Q SQL 专题                              90
来源：http://atd.cdnleiting.top

R Bash 专题                             80
来源：http://gvl.hysaishi.cn

S C / C++ 专题                          60
来源：http://vhz.daria6918.cn

T 其他语言补充                          60
来源：http://byh.shzxlz.cn

U 高频实用片段                         120
来源：http://ple.zdbjq.cn

------------------------------------
来源：http://nra.chenzaomai.com

合计                                  2106 条
来源：http://uvl.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://tcg.pengpengdd.cyou

使用提醒
来源：http://rnf.cqqwz.cn

--------------------------------------------------------------------------------
来源：http://ofg.fanxiaobao.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fkw.hongshengwenyu.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xvd.cucudq.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ijt.c1oappe.top

在旧版本上使用前请先确认语法支持情况。
来源：http://fzh.yfazqb.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://gjf.sysykeji.top

—— 文件结束 ——
来源：http://xck.jiagoushi.top

================================================================================
来源：http://wbg.daxiang520.top

程序语言常见例子速查手册（2024 版）
来源：http://srk.nwbrower.top

Common Programming Examples Cheat Book
来源：http://keu.jlsjyb.cn

================================================================================
来源：http://zlb.xziqi.cn

【收录内容】
来源：http://cwy.havefunace.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://hrd.xinyue.icu

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rtk.hcnkem.com

SQL · Bash · C · C++
来源：http://yoz.hammf.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xec.yj20258.top

【使用说明】
来源：http://yhk.haohaochexian.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ihx.havefunace.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://eof.yuanzhike.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sjl.hesvh.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yev.ctjpmb.com

Bash:  Shell         C:     C             C++:   C++
来源：http://xkr.jiagoushi.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yeg.yj20258.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qwp.yonumen.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://twa.cqqwz.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kdf.xuetiantiany.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wtk.jinghuilouyu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nhh.zdbjq.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baq.feifeiyinyue.top

【文件统计】
来源：http://qhb.chenzaomai.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://evh.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://zgd.shanyushiyangtech.top

目  录
来源：http://zdv.52xcode.cn

--------------------------------------------------------------------------------
来源：http://oej.haohaochexian.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://npm.daxiang520.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zpa.c1oappe.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tlu.wangshuangyany.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://whd.sweek.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gzk.redwolf501.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://noa.aizwys.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bhv.chenlongwang.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lvl.xylfe.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rhr.xingfuxueyuan.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qrv.jinqigfzy.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rra.nanxinkj.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://amn.aizwys.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://azg.fktsv.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gft.cheryme.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wrd.gaohongyu789.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qfa.cucudq.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://acz.fanxiaobao.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://cea.yueranfly.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://czb.hesvh.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dwo.meibo888.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://oqo.ywan-chungtsiang.top

================================================================================
来源：http://exa.zhijiandao.cn

A. 基础语法与类型
来源：http://cpk.sjlbkw.cn

================================================================================
来源：http://iju.mhx1999.top

[A01] Hello World
来源：http://gih.zdqjudy.top

Py:   print("Hello, World!")
来源：http://kjg.xinyue.icu

PHP:  echo "Hello, World!";
来源：http://lob.tian-w.cn

JS:   console.log("Hello, World!");
来源：http://fsw.zdqjudy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hsr.zhijiandao.cn

Java: System.out.println("Hello, World!");
来源：http://mls.zhiwuduotai.top

Go:   fmt.Println("Hello, World!")
来源：http://rpe.uphjek.com

Ruby: puts "Hello, World!"
来源：http://uzm.sufxvd.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://mcv.jinqigufen.top

[A02] 变量声明与赋值
来源：http://kcz.wangshuangyany.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ipv.nwbrower.top

PHP:  $name = "Alex"; $age = 20;
来源：http://xzw.ctjpmb.com

JS:   let name = "Alex"; const age = 20;
来源：http://crt.ydzc1.top


<!-- 参考信息 -->