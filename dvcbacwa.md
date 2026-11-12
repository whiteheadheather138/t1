代发 wailian999

[U33] Py：打包发布
来源：http://hza.xuetiantiany.cn

python -m build  （依赖 pyproject.toml）
来源：http://cnl.hywenlv.cn

[U34] Py：判断编码
来源：http://qya.yuanzhike.top

chardet.detect(raw)
来源：http://wib.daria6918.cn

[U35] Py：发送邮件
来源：http://ncs.pycfn.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uho.shzxlz.cn

[U36] Py：定时任务
来源：http://ipu.wangshuangyany.cn

schedule.every(10).minutes.do(job)
来源：http://mxe.52xcode.cn

[U37] Py：读写 Excel
来源：http://crg.fengsongda.top

pandas.read_excel / DataFrame.to_excel
来源：http://wbt.ivvv.top

[U38] Py：获取脚本所在目录
来源：http://coa.haohaochexian.top

Path(__file__).resolve().parent
来源：http://lev.yj20258.top

[U39] Py：判断是否在交互环境
来源：http://gor.yonumen.top

sys.stdout.isatty()
来源：http://tek.zhixingplan.top

[U40] Py：打印到标准错误
来源：http://xqk.hammf.cn

print("err", file=sys.stderr)
来源：http://gtd.sweek.top

[U41] PHP：初始化 Composer 项目
来源：http://xwm.quarkkingdee.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ijs.yongpay.top

[U42] PHP：PSR-4 自动加载
来源：http://jgy.uphjek.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yex.nanxuanxn.top

[U43] PHP：声明命名空间
来源：http://dbs.ydzc1.top

namespace App\Http;
来源：http://jfr.jiagoushi.top

[U44] PHP：开启严格类型
来源：http://icv.yonumen.top

declare(strict_types=1);
来源：http://nxa.jyoumei.cn

[U45] PHP：类型声明与返回类型
来源：http://aip.yueranfly.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://gxy.wangdashe.top

[U46] PHP：可空类型
来源：http://oxq.iojbl.cn

?string $name = null
来源：http://our.yonumen.top

[U47] PHP：联合类型
来源：http://adq.shangyingyoupin.top

int|string $id
来源：http://eim.gotoacloud.top

[U48] PHP：纯枚举
来源：http://vys.ywan-chungtsiang.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ofw.jqgfzy.top

[U49] PHP：只读属性
来源：http://ydi.vqdsnc.cn

public readonly string $name
来源：http://zwr.xuetiantiany.cn

[U50] PHP：构造器属性提升
来源：http://ars.tanke756.top

public function __construct(private int $id) {}
来源：http://nqy.ydzc1.top

[U51] PHP：数组解构
来源：http://lwp.jqgfzy.top

[$a, $b] = $arr;
来源：http://ohd.sjlbkw.cn

[U52] PHP：箭头函数
来源：http://ndf.jqgfzy.top

$double = fn($x) => $x * 2;
来源：http://osv.chenjidiqi.icu

[U53] PHP：空合并运算符
来源：http://mtn.cdnleiting.top

$v = $a ?? $b ?? "default";
来源：http://gyz.fanxiaobao.xyz

[U54] PHP：空安全调用
来源：http://jjg.nanxuanxn.top

$obj?->method()
来源：http://smr.yuanzhike.top

[U55] PHP：match 表达式
来源：http://snt.yj202588.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hzr.xuetiantiany.cn

[U56] PHP：命名参数
来源：http://ywx.cdnleiting.top

f(a: 1, b: 2)
来源：http://mjv.cqqwz.cn

[U57] PHP：字符串插值
来源：http://noq.cheryme.top

"值: {$a}"
来源：http://pfv.xuetiantiany.cn

[U58] PHP：数组三件套
来源：http://zpl.jianghu66.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://unc.hongshengwenyu.top

[U59] PHP：自定义排序
来源：http://yzp.fengsongda.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://the.zhaomingkeji.xyz

[U60] PHP：JSON 编解码
来源：http://acs.birdmap.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hio.jiagoushi.top

[U61] PHP：正则
来源：http://qlk.fengsongda.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pbj.gogol.net.cn

[U62] PHP：日期对象
来源：http://vqr.meibo888.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zkn.fehbvm.com

[U63] PHP：文件读写
来源：http://org.dianchejie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://emf.sweek.top

[U64] PHP：目录遍历
来源：http://wty.52xcode.cn

glob("dir/*.php");  scandir("dir");
来源：http://kzt.cashguo.top

[U65] PHP：会话
来源：http://urg.jinyuanbaomall.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qcx.hywenlv.cn

[U66] PHP：设置 Cookie
来源：http://cmk.ydzc1.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dvp.hesvh.cn

[U67] PHP：处理文件上传
来源：http://qsb.pengpengdd.cyou

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://twm.redwolf501.top

[U68] PHP：PDO 连接
来源：http://bsi.daxiang520.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://aaz.yj20258.top

[U69] PHP：PDO 预处理
来源：http://iks.tianlin.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://oyi.0kj1m.cn

[U70] PHP：PDO 事务
来源：http://jli.tian-w.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kof.smart0.xyz

[U71] PHP：抛出异常
来源：http://bmd.sysykeji.top

throw new RuntimeException("失败", 500);
来源：http://jmr.ydzc1.top

[U72] PHP：写错误日志
来源：http://cou.fzhhl.top

error_log("失败: " . $e->getMessage());
来源：http://ezh.yongpay.top

[U73] PHP：读取 ini 配置
来源：http://cij.shangyingyoupin.top

parse_ini_file("config.ini", true)
来源：http://usk.shanyushiyangtech.top

[U74] PHP：读取环境变量
来源：http://vfx.zdqjudy.top

getenv("APP_ENV") ?: "production"
来源：http://cyn.gogol.net.cn

[U75] PHP：依赖注入
来源：http://rqe.wangshuangyany.cn

composer require psr/container
来源：http://cmn.hammf.cn

[U76] PHP：简单路由
来源：http://nvb.guowangkeji.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fce.c1oappe.top

[U77] PHP：模板渲染
来源：http://zkc.cucudq.cn

composer require twig/twig
来源：http://iwc.tanke756.top

[U78] PHP：单元测试
来源：http://gto.guowangkeji.top

composer require --dev phpunit/phpunit
来源：http://mkg.zhiwuduotai.top

[U79] PHP：静态分析
来源：http://szl.fehbvm.com

composer require --dev phpstan/phpstan
来源：http://zcq.hnxiangtu.top

[U80] PHP：代码规范修复
来源：http://pnh.hfpthk.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pzw.sufxvd.cn

[U81] JS：初始化项目
来源：http://glu.zycfv.cn

npm init -y;  npm i express
来源：http://oai.aibaodan.cn

[U82] JS：package.json 脚本
来源：http://umc.yuanzhike.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bmm.316326.xyz

[U83] JS：ES Module 导入导出
来源：http://wjl.shanyushiyangtech.top

export const a = 1;  import { a } from "./m.js";
来源：http://nat.jlsjyb.cn

[U84] JS：CommonJS 写法
来源：http://ved.chenjidiqi.icu

module.exports = { a };  const { a } = require("./m");
来源：http://xaj.xuetiantiany.cn

[U85] JS：可选链
来源：http://xgs.ctjpmb.com

a?.b?.c
来源：http://wst.zhongyouzk.top

[U86] JS：空值合并
来源：http://vuv.nanxuanxn.top

a ?? b
来源：http://nem.hnxiangtu.top

[U87] JS：解构默认值
来源：http://zax.shangyingyoupin.top

const { a = 1, b = 2 } = obj;
来源：http://ion.xuetiantiany.cn

[U88] JS：对象展开合并
来源：http://rqm.tianlin.xyz

{ ...a, ...b }
来源：http://vnw.yj20258.top

[U89] JS：数组去重
来源：http://dyj.jlsjyb.cn

[...new Set(arr)]
来源：http://myz.epnwcf.com

[U90] JS：数字数组排序
来源：http://skh.nanxuanxn.top

[...arr].sort((a, b) => a - b)
来源：http://oyq.hesvh.cn

[U91] JS：对象键值遍历
来源：http://hbc.nwbrower.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nay.jqgufenzy.top

[U92] JS：深拷贝
来源：http://jwb.yj20258.top

structuredClone(obj)
来源：http://gsa.tianlin.xyz

[U93] JS：模板字符串
来源：http://nbw.ehwqpu.com

`共 ${n} 条`
来源：http://sco.zycfv.cn

[U94] JS：箭头函数
来源：http://rep.kuanghao11.cn

const double = x => x * 2;
来源：http://vqa.yonumen.top

[U95] JS：Promise 包装
来源：http://vcr.jinqigfzy.top

new Promise((resolve, reject) => {})
来源：http://yit.fanxiaobao.xyz

[U96] JS：async/await 与异常
来源：http://xvk.zhixingplan.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lbc.svipenyu.cn

[U97] JS：并发请求
来源：http://qcn.nanxuanxn.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://bbg.zhengqikj.top

[U98] JS：fetch 带 JSON
来源：http://jmw.xziqi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wus.meibo888.top

[U99] JS：事件监听
来源：http://jlm.yj20258888.top

el.addEventListener("click", e => {})
来源：http://zdi.tian-w.cn

[U100] JS：DOM 查询
来源：http://dyi.xuetiantiany.cn

document.querySelector(".item")
来源：http://rkx.0kj1m.cn

[U101] JS：classList 操作
来源：http://alo.chenjidiqi.icu

el.classList.toggle("active")
来源：http://fur.yueranfly.top

[U102] JS：本地存储
来源：http://jnr.zhongyouzk.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://xqy.hywenlv.cn

[U103] JS：定时器
来源：http://phq.guannengcc.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://thq.xylfe.cn

[U104] JS：防抖
来源：http://tpr.tarul.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sly.jlsjyb.cn

[U105] JS：节流
来源：http://zzm.nanxuanxn.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dkz.gzhubu.top

[U106] JS：日期格式化
来源：http://cea.tianlin.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jti.yj202588.top

[U107] JS：数字千分位
来源：http://wbi.xingfuxueyuan.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dqi.vehdjk.com

[U108] JS：随机整数
来源：http://lht.hnxiangtu.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://odl.tian-w.cn

[U109] JS：数组分组
来源：http://vnh.zhiwuduotai.top

Object.groupBy(arr, x => x.type)
来源：http://mmg.zhengqikj.top

[U110] JS：数组分块
来源：http://hqh.chenjidiqi.icu

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lhw.tarul.cn

[U111] JS：对象转 Map
来源：http://qay.jiagoushi.top

new Map(Object.entries(obj))
来源：http://bwn.hnxiangtu.top

[U112] JS：字符串补位
来源：http://acu.cucudq.cn

"7".padStart(3, "0")
来源：http://kth.mhx1999.top

[U113] JS：正则替换全部
来源：http://wcz.ivvv.top

s.replaceAll("a", "b")
来源：http://tbe.quarkkingdee.top

[U114] JS：JSON 深比较
来源：http://gpg.cqqwz.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ezm.0kj1m.cn

[U115] JS：生成 UUID
来源：http://fqf.andypj.xyz

crypto.randomUUID()
来源：http://oog.jinghuilouyu.cn

[U116] JS：类型检查（JSDoc）
来源：http://oje.nanxinkj.top

/** @param {string} name */ function f(name) {}
来源：http://ylf.fzhhl.top

[U117] JS：单元测试
来源：http://qye.dashuyun.cn

npm i -D vitest;  npx vitest
来源：http://wwn.yfazqb.com

[U118] JS：开发服务器
来源：http://moj.zhongyouzk.top

npm i -D vite;  npx vite
来源：http://zch.andypj.xyz

[U119] JS：生产构建
来源：http://djt.jinqigfzy.top

npx vite build
来源：http://rfq.dashuyun.cn

[U120] JS：读取环境变量（Vite）
来源：http://pab.fehbvm.com

import.meta.env.VITE_API_URL
来源：http://pqd.nwbrower.top

================================================================================
来源：http://qhr.mhx1999.top

统计汇总
来源：http://akq.chenjidiqi.icu

================================================================================
来源：http://gaf.pengpengdd.cyou

按语言统计（条）：
来源：http://kco.daxiang520.top

Python ......... 252
来源：http://cbc.yuxming.cn

PHP ............ 252
来源：http://pud.feifeiyinyue.top

JavaScript ..... 252
来源：http://ycg.hywenlv.cn

TypeScript ..... 212
来源：http://lln.jlsjyb.cn

Java ........... 212
来源：http://ezl.jqgfzy.top

Go ............. 212
来源：http://yfm.haohaochexian.top

Ruby ........... 212
来源：http://zdb.jlsjyb.cn

C# ............. 212
来源：http://ozo.quarkkingdee.top

C .............. 30
来源：http://bmz.yj20258.top

C++ ............ 30
来源：http://olv.dashuyun.cn

SQL ............ 90
来源：http://qsh.jqgufenzy.top

Bash ........... 80
来源：http://arq.xylfe.cn

Kotlin ......... 15
来源：http://kwe.nwbrower.top

Swift .......... 15
来源：http://uan.gotoacloud.top

Lua ............ 10
来源：http://qxd.9152youxi.cn

Perl ........... 10
来源：http://hsi.yongpay.top

Scala .......... 10
来源：http://qmw.daria6918.cn

------------------------------------
来源：http://xyf.chenzaomai.com

合计 ........... 2106 条
来源：http://ohs.chenlongwang.top

按章节统计：
来源：http://bug.jiagoushi.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ylt.yongpay.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rtx.iojbl.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://orf.daxiang520.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cuw.zhijiandao.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jsn.zhongyouzk.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://epe.ivvv.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yyq.vehdjk.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://svr.aizwys.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wyj.meibo888.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nbc.wangdashe.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cig.aizwys.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://htm.316326.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://osg.haohaochexian.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://inr.jianghu66.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wzu.hnqzz.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kle.gaohongyu789.top

Q SQL 专题                              90
来源：http://oai.gaohongyu789.top

R Bash 专题                             80
来源：http://dcl.fehbvm.com

S C / C++ 专题                          60
来源：http://aqe.shzxlz.cn

T 其他语言补充                          60
来源：http://gda.chenzaomai.com

U 高频实用片段                         120
来源：http://kke.zhoulong.xyz

------------------------------------
来源：http://yue.guannengcc.top

合计                                  2106 条
来源：http://pjp.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://vav.quarkkingdee.top

使用提醒
来源：http://oll.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://oqt.zhengqikj.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://abn.zdqjudy.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kbl.aizwys.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ykc.jianghu66.top

在旧版本上使用前请先确认语法支持情况。
来源：http://tet.ydjk.org.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hcq.feifeiyinyue.top

—— 文件结束 ——
来源：http://sbj.gzhubu.top

================================================================================
来源：http://yqj.yuanzhike.top

程序语言常见例子速查手册（2024 版）
来源：http://pxm.hammf.cn

Common Programming Examples Cheat Book
来源：http://kup.cqqwz.cn

================================================================================
来源：http://pig.uphjek.com

【收录内容】
来源：http://lpo.zhengqikj.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://mqi.zhixingplan.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lyz.vehdjk.com

SQL · Bash · C · C++
来源：http://ben.ydjk.org.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ppe.sxryk.cn

【使用说明】
来源：http://pxw.wangdashe.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gnl.gaohongyu789.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://adp.chenjidiqi.icu

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://svc.gotoacloud.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mbd.gaohongyu789.top

Bash:  Shell         C:     C             C++:   C++
来源：http://pjo.yj20258.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gik.ctjpmb.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ptm.gogol.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sjx.bbcook.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://maf.ehwqpu.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bme.tianlin.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ymi.hongshengwenyu.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wlg.tarul.cn

【文件统计】
来源：http://wux.haohaochexian.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ked.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://wav.yj20258.top

目  录
来源：http://zqi.zhiwuduotai.top

--------------------------------------------------------------------------------
来源：http://cpb.jyoumei.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dic.tianlin.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ttj.jyoumei.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gnr.daxiang520.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ifb.quarkkingdee.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fdn.jianghu66.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fhx.gotoacloud.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://obt.ybcxt.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gob.gogol.net.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wqa.dashuyun.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gxx.pengpengdd.cyou

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gcb.jinqigfzy.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ccp.hnxiangtu.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cie.jqgufenzy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cbw.feifeiyinyue.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lit.yanxiufei.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kbu.jinqigfzy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tzd.jinyuanbaomall.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://uuv.ydzc1.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xii.jqgfzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wgy.ctjpmb.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uwt.xingfuxueyuan.xyz

================================================================================
来源：http://fqa.jiagoushi.top

A. 基础语法与类型
来源：http://xje.xuanzx.com

================================================================================
来源：http://bcv.tarul.cn

[A01] Hello World
来源：http://wvw.uphjek.com

Py:   print("Hello, World!")
来源：http://pyo.fzhhl.top

PHP:  echo "Hello, World!";
来源：http://ewz.yonumen.top

JS:   console.log("Hello, World!");
来源：http://pyz.gotoacloud.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mgu.cheryme.top

Java: System.out.println("Hello, World!");
来源：http://lat.snrcjt.cn

Go:   fmt.Println("Hello, World!")
来源：http://zas.tanke756.top

Ruby: puts "Hello, World!"
来源：http://hxn.uphjek.com

C#:   Console.WriteLine("Hello, World!");
来源：http://caw.hesvh.cn

[A02] 变量声明与赋值
来源：http://orq.hammf.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kbi.xuetiantiany.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bmk.gzhubu.top

JS:   let name = "Alex"; const age = 20;
来源：http://dek.cdnleiting.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sbo.zhengqikj.top

Java: String name = "Alex"; int age = 20;
来源：http://vxc.xuetiantiany.cn

Go:   name := "Alex"; age := 20
来源：http://mpy.tianlin.xyz

Ruby: name = "Alex"; age = 20
来源：http://ivw.fanxiaobao.xyz


<!-- 参考信息 -->