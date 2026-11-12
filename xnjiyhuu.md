代发 wailian999

[U33] Py：打包发布
来源：http://bqo.ybcxt.top

python -m build  （依赖 pyproject.toml）
来源：http://zyp.jqgfzy.top

[U34] Py：判断编码
来源：http://ggj.ybcxt.top

chardet.detect(raw)
来源：http://wvt.yonumen.top

[U35] Py：发送邮件
来源：http://zuj.epnwcf.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://voq.shuidangran.top

[U36] Py：定时任务
来源：http://cjg.jinqigfzy.top

schedule.every(10).minutes.do(job)
来源：http://lio.ywan-chungtsiang.top

[U37] Py：读写 Excel
来源：http://dju.sysykeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://cuu.guowangkeji.top

[U38] Py：获取脚本所在目录
来源：http://wux.quarkkingdee.top

Path(__file__).resolve().parent
来源：http://qpw.zhijiandao.cn

[U39] Py：判断是否在交互环境
来源：http://wnd.jlsjyb.cn

sys.stdout.isatty()
来源：http://eue.gogol.net.cn

[U40] Py：打印到标准错误
来源：http://rxp.smart0.xyz

print("err", file=sys.stderr)
来源：http://srp.jlsjyb.cn

[U41] PHP：初始化 Composer 项目
来源：http://kwu.sjlbkw.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://uoi.yvedp.cn

[U42] PHP：PSR-4 自动加载
来源：http://xsv.fehbvm.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ipj.yj20258888.top

[U43] PHP：声明命名空间
来源：http://wwr.cheryme.top

namespace App\Http;
来源：http://ppe.bjfxy.top

[U44] PHP：开启严格类型
来源：http://vpp.tianlin.xyz

declare(strict_types=1);
来源：http://eqp.yangfankeji.com

[U45] PHP：类型声明与返回类型
来源：http://bmx.chenzaomai.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://rbe.jianghu66.top

[U46] PHP：可空类型
来源：http://ydr.kuanghao11.cn

?string $name = null
来源：http://txu.hesvh.cn

[U47] PHP：联合类型
来源：http://mkj.jiagoushi.top

int|string $id
来源：http://kml.sufxvd.cn

[U48] PHP：纯枚举
来源：http://dwo.hesvh.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xlr.aizwys.cn

[U49] PHP：只读属性
来源：http://jjx.gzhubu.top

public readonly string $name
来源：http://qif.shzxlz.cn

[U50] PHP：构造器属性提升
来源：http://bwp.fanxiaobao.xyz

public function __construct(private int $id) {}
来源：http://iph.fengsongda.top

[U51] PHP：数组解构
来源：http://mwe.hywenlv.cn

[$a, $b] = $arr;
来源：http://nji.daria6918.cn

[U52] PHP：箭头函数
来源：http://zzw.feifeiyinyue.top

$double = fn($x) => $x * 2;
来源：http://bnm.xinyue.icu

[U53] PHP：空合并运算符
来源：http://zls.jinghuilouyu.cn

$v = $a ?? $b ?? "default";
来源：http://kyr.xylfe.cn

[U54] PHP：空安全调用
来源：http://lww.shuidangran.top

$obj?->method()
来源：http://qeu.xziqi.cn

[U55] PHP：match 表达式
来源：http://qhn.sysykeji.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gya.0kj1m.cn

[U56] PHP：命名参数
来源：http://mvo.kuanghao11.cn

f(a: 1, b: 2)
来源：http://rbp.feifeiyinyue.top

[U57] PHP：字符串插值
来源：http://ywq.dashuyun.cn

"值: {$a}"
来源：http://ioi.sufxvd.cn

[U58] PHP：数组三件套
来源：http://tms.zhongyouzk.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gjk.havefunace.top

[U59] PHP：自定义排序
来源：http://oey.jinqigufen.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://roa.daxiang520.top

[U60] PHP：JSON 编解码
来源：http://ils.yj20258888.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cdi.sufxvd.cn

[U61] PHP：正则
来源：http://tqv.jqgfzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ztb.jinqigufen.top

[U62] PHP：日期对象
来源：http://fnh.yonumen.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uum.daria6918.cn

[U63] PHP：文件读写
来源：http://lnf.mhx1999.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://aao.cucudq.cn

[U64] PHP：目录遍历
来源：http://wov.quarkkingdee.top

glob("dir/*.php");  scandir("dir");
来源：http://gti.jyoumei.cn

[U65] PHP：会话
来源：http://bsd.c1oappe.top

session_start();  $_SESSION["uid"] = 1;
来源：http://xvx.tianlin.xyz

[U66] PHP：设置 Cookie
来源：http://kqi.iojbl.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qdh.chenlongwang.top

[U67] PHP：处理文件上传
来源：http://oif.dashuyun.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qmp.cashguo.top

[U68] PHP：PDO 连接
来源：http://kdg.feifeiyinyue.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hkj.vqdsnc.cn

[U69] PHP：PDO 预处理
来源：http://rgg.sxryk.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ptr.zhengqikj.top

[U70] PHP：PDO 事务
来源：http://bsh.xingfuxueyuan.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://efl.vqdsnc.cn

[U71] PHP：抛出异常
来源：http://urm.hongshengwenyu.top

throw new RuntimeException("失败", 500);
来源：http://cih.gaohongyu789.top

[U72] PHP：写错误日志
来源：http://gak.jqgfzy.top

error_log("失败: " . $e->getMessage());
来源：http://sks.jqgfzy.top

[U73] PHP：读取 ini 配置
来源：http://ryw.mhx1999.top

parse_ini_file("config.ini", true)
来源：http://wyl.birdmap.top

[U74] PHP：读取环境变量
来源：http://lvm.shanyushiyangkeji.top

getenv("APP_ENV") ?: "production"
来源：http://rfu.jqgfzy.top

[U75] PHP：依赖注入
来源：http://hbz.haohaochexian.top

composer require psr/container
来源：http://ccq.zhoulong.xyz

[U76] PHP：简单路由
来源：http://uvs.52xcode.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ykg.shzxlz.cn

[U77] PHP：模板渲染
来源：http://wwx.zhijiandao.cn

composer require twig/twig
来源：http://wkl.tarul.cn

[U78] PHP：单元测试
来源：http://vjy.guannengcc.top

composer require --dev phpunit/phpunit
来源：http://nbg.chenjidiqi.icu

[U79] PHP：静态分析
来源：http://qjy.yvedp.cn

composer require --dev phpstan/phpstan
来源：http://mea.zhongyouzk.top

[U80] PHP：代码规范修复
来源：http://bxf.yanxiufei.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dtf.guowangkeji.top

[U81] JS：初始化项目
来源：http://cik.hongshengwenyu.top

npm init -y;  npm i express
来源：http://rxe.gogol.net.cn

[U82] JS：package.json 脚本
来源：http://pbc.c1oappe.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://plz.wangshuangyany.cn

[U83] JS：ES Module 导入导出
来源：http://eqh.shzxlz.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zjq.yfazqb.com

[U84] JS：CommonJS 写法
来源：http://jaf.shangyingyoupin.top

module.exports = { a };  const { a } = require("./m");
来源：http://hqr.xuetiantiany.cn

[U85] JS：可选链
来源：http://qgb.gzhubu.top

a?.b?.c
来源：http://kqi.birdmap.top

[U86] JS：空值合并
来源：http://vgk.hnqzz.top

a ?? b
来源：http://alt.yangfankeji.com

[U87] JS：解构默认值
来源：http://clr.wangdashe.top

const { a = 1, b = 2 } = obj;
来源：http://jqe.sjlbkw.cn

[U88] JS：对象展开合并
来源：http://iam.fanxiaobao.xyz

{ ...a, ...b }
来源：http://nrv.birdmap.top

[U89] JS：数组去重
来源：http://xig.jianghu66.top

[...new Set(arr)]
来源：http://bkz.ydjk.org.cn

[U90] JS：数字数组排序
来源：http://llx.vqdsnc.cn

[...arr].sort((a, b) => a - b)
来源：http://sui.jinqigfzy.top

[U91] JS：对象键值遍历
来源：http://prq.ivvv.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rck.svipenyu.cn

[U92] JS：深拷贝
来源：http://wqz.jlsjyb.cn

structuredClone(obj)
来源：http://ark.yvedp.cn

[U93] JS：模板字符串
来源：http://ang.yangfankeji.com

`共 ${n} 条`
来源：http://mlh.jiagoushi.top

[U94] JS：箭头函数
来源：http://ild.epnwcf.com

const double = x => x * 2;
来源：http://ytk.gzhubu.top

[U95] JS：Promise 包装
来源：http://kxt.birdmap.top

new Promise((resolve, reject) => {})
来源：http://tbd.hfpthk.cn

[U96] JS：async/await 与异常
来源：http://jhs.ywan-chungtsiang.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tci.gotoacloud.top

[U97] JS：并发请求
来源：http://cvi.tanke756.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://vpm.zhoulong.xyz

[U98] JS：fetch 带 JSON
来源：http://jde.ppjwa.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://odv.chenzaomai.com

[U99] JS：事件监听
来源：http://ctr.aibaodan.cn

el.addEventListener("click", e => {})
来源：http://ybv.feifeiyinyue.top

[U100] JS：DOM 查询
来源：http://ope.316326.xyz

document.querySelector(".item")
来源：http://cgh.c1oappe.top

[U101] JS：classList 操作
来源：http://mey.fengsongda.top

el.classList.toggle("active")
来源：http://xiy.cucudq.cn

[U102] JS：本地存储
来源：http://gej.guannengcc.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://vru.zhiwuduotai.top

[U103] JS：定时器
来源：http://ucj.jqgufenzy.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kyp.daria6918.cn

[U104] JS：防抖
来源：http://zhg.gotoacloud.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ykn.snrcjt.cn

[U105] JS：节流
来源：http://rpv.daria6918.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sgw.shzxlz.cn

[U106] JS：日期格式化
来源：http://nje.sysykeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mix.ehwqpu.com

[U107] JS：数字千分位
来源：http://aiy.uphjek.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://fmv.zdbjq.cn

[U108] JS：随机整数
来源：http://xht.9152youxi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zuz.hongshengwenyu.top

[U109] JS：数组分组
来源：http://ohk.hesvh.cn

Object.groupBy(arr, x => x.type)
来源：http://enh.yonumen.top

[U110] JS：数组分块
来源：http://kgh.jinqigfzy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rxs.hfpthk.cn

[U111] JS：对象转 Map
来源：http://nkg.nwbrower.top

new Map(Object.entries(obj))
来源：http://tme.yueranfly.top

[U112] JS：字符串补位
来源：http://gvt.fktsv.cn

"7".padStart(3, "0")
来源：http://oxb.hcnkem.com

[U113] JS：正则替换全部
来源：http://xbv.andypj.xyz

s.replaceAll("a", "b")
来源：http://klb.fanxiaobao.xyz

[U114] JS：JSON 深比较
来源：http://npo.cucudq.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cve.yfazqb.com

[U115] JS：生成 UUID
来源：http://bxp.ehwqpu.com

crypto.randomUUID()
来源：http://bsf.xuanzx.com

[U116] JS：类型检查（JSDoc）
来源：http://cvo.hfpthk.cn

/** @param {string} name */ function f(name) {}
来源：http://fmn.zdqjudy.top

[U117] JS：单元测试
来源：http://qpj.hnxiangtu.top

npm i -D vitest;  npx vitest
来源：http://qnd.yvedp.cn

[U118] JS：开发服务器
来源：http://oob.shanyushiyangtech.top

npm i -D vite;  npx vite
来源：http://ebs.guannengcc.top

[U119] JS：生产构建
来源：http://fia.xziqi.cn

npx vite build
来源：http://hio.ydjk.org.cn

[U120] JS：读取环境变量（Vite）
来源：http://ppx.dianchejie.cn

import.meta.env.VITE_API_URL
来源：http://jiu.hysaishi.cn

================================================================================
来源：http://jqu.feifeiyinyue.top

统计汇总
来源：http://fbs.xuetiantiany.cn

================================================================================
来源：http://deg.havefunace.top

按语言统计（条）：
来源：http://jvt.jyoumei.cn

Python ......... 252
来源：http://xdi.zdbjq.cn

PHP ............ 252
来源：http://ldp.yj202588.top

JavaScript ..... 252
来源：http://nzb.yuxming.cn

TypeScript ..... 212
来源：http://mhf.jyoumei.cn

Java ........... 212
来源：http://syo.nanxuanxn.top

Go ............. 212
来源：http://lcv.tian-w.cn

Ruby ........... 212
来源：http://ecc.gaohongyu789.top

C# ............. 212
来源：http://igr.9152youxi.cn

C .............. 30
来源：http://xyd.uphjek.com

C++ ............ 30
来源：http://ctq.tianlin.xyz

SQL ............ 90
来源：http://yna.shuidangran.top

Bash ........... 80
来源：http://qen.snrcjt.cn

Kotlin ......... 15
来源：http://kch.yvedp.cn

Swift .......... 15
来源：http://pir.cashguo.top

Lua ............ 10
来源：http://mey.c1oappe.top

Perl ........... 10
来源：http://ctv.yueranfly.top

Scala .......... 10
来源：http://nfs.cqqwz.cn

------------------------------------
来源：http://pst.cheryme.top

合计 ........... 2106 条
来源：http://obz.wangdashe.top

按章节统计：
来源：http://xbr.xuanzx.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hmz.ywan-chungtsiang.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ejw.tanke756.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ick.tianlin.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zml.hcnkem.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rgt.daria6918.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pft.haohaochexian.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://atm.9152youxi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pom.cqqwz.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://aff.fengsongda.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://upm.cucudq.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hlj.dashuyun.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fog.tianlin.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ara.gotoacloud.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ivg.nwbrower.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pvx.yvedp.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fbh.ydjk.org.cn

Q SQL 专题                              90
来源：http://yya.jlsjyb.cn

R Bash 专题                             80
来源：http://pyb.ehwqpu.com

S C / C++ 专题                          60
来源：http://uyi.dashuyun.cn

T 其他语言补充                          60
来源：http://zig.cqqwz.cn

U 高频实用片段                         120
来源：http://uft.zhengqikj.top

------------------------------------
来源：http://ibw.hnxiangtu.top

合计                                  2106 条
来源：http://euk.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://asz.jinghuilouyu.cn

使用提醒
来源：http://tyo.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://cti.mhx1999.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yzo.tianlin.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://msa.iojbl.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lqp.hnxiangtu.top

在旧版本上使用前请先确认语法支持情况。
来源：http://kmz.vqdsnc.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xit.zdqjudy.top

—— 文件结束 ——
来源：http://nva.zdqjudy.top

================================================================================
来源：http://ohw.epnwcf.com

程序语言常见例子速查手册（2024 版）
来源：http://qgf.gotoacloud.top

Common Programming Examples Cheat Book
来源：http://ssv.zhiwuduotai.top

================================================================================
来源：http://wli.xuanzx.com

【收录内容】
来源：http://bpc.hysaishi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yuo.quarkkingdee.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pvp.mhx1999.top

SQL · Bash · C · C++
来源：http://wyk.xziqi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://eer.ybcxt.top

【使用说明】
来源：http://byu.zhongyouzk.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bow.haohaochexian.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zmw.feifeiyinyue.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://slp.cucudq.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bel.yj20258888.top

Bash:  Shell         C:     C             C++:   C++
来源：http://abt.cashguo.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yxc.zhengqikj.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gax.ydjk.org.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wto.gogol.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://iuk.haohaochexian.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yfc.0kj1m.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qvv.yfazqb.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://frk.hammf.cn

【文件统计】
来源：http://rwa.sysykeji.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://uvc.tanke756.top

--------------------------------------------------------------------------------
来源：http://pbn.xingfuxueyuan.xyz

目  录
来源：http://gtq.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://zng.cashguo.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yok.xuetiantiany.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uhb.tianlin.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rhd.dianchejie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://czu.daxiang520.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mge.hnqzz.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jnv.zhijiandao.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rzp.aibaodan.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://edg.dianchejie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ogc.tian-w.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://oig.sysykeji.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xmq.bbcook.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qhk.cdnleiting.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mxm.shanyushiyangtech.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wlz.shangyingyoupin.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jim.sxryk.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://pie.sweek.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cxl.hesvh.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zvd.jlsjyb.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wpn.wangdashe.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://icy.sxryk.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ode.sjlbkw.cn

================================================================================
来源：http://shl.shzxlz.cn

A. 基础语法与类型
来源：http://npz.andypj.xyz

================================================================================
来源：http://ony.ivvv.top

[A01] Hello World
来源：http://leh.svipenyu.cn

Py:   print("Hello, World!")
来源：http://bsz.shuidangran.top

PHP:  echo "Hello, World!";
来源：http://zkp.jqgfzy.top

JS:   console.log("Hello, World!");
来源：http://bxn.fengsongda.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://nhq.xziqi.cn

Java: System.out.println("Hello, World!");
来源：http://brn.dianchejie.cn

Go:   fmt.Println("Hello, World!")
来源：http://ndp.cucudq.cn

Ruby: puts "Hello, World!"
来源：http://jjt.bbcook.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ohg.zdbjq.cn

[A02] 变量声明与赋值
来源：http://pis.yongpay.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://osg.yvedp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jeb.ybcxt.top

JS:   let name = "Alex"; const age = 20;
来源：http://sjf.fengsongda.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://twh.quarkkingdee.top

Java: String name = "Alex"; int age = 20;
来源：http://stt.0kj1m.cn

Go:   name := "Alex"; age := 20
来源：http://ksn.ehwqpu.com

Ruby: name = "Alex"; age = 20
来源：http://bpa.hcnkem.com


<!-- 参考信息 -->