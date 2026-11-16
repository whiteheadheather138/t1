代发 wailian999

[U33] Py：打包发布
来源：http://zvx.tian-w.cn

python -m build  （依赖 pyproject.toml）
来源：http://hur.cqqwz.cn

[U34] Py：判断编码
来源：http://vrn.nanxinkj.top

chardet.detect(raw)
来源：http://vgr.nanxinkj.top

[U35] Py：发送邮件
来源：http://wmg.gaohongyu789.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ucd.nwbrower.top

[U36] Py：定时任务
来源：http://qkt.zhoulong.xyz

schedule.every(10).minutes.do(job)
来源：http://gmu.nanxinkj.top

[U37] Py：读写 Excel
来源：http://eut.chenzaomai.com

pandas.read_excel / DataFrame.to_excel
来源：http://dpz.gzhubu.top

[U38] Py：获取脚本所在目录
来源：http://eiu.shanyushiyangkeji.top

Path(__file__).resolve().parent
来源：http://lop.sysykeji.top

[U39] Py：判断是否在交互环境
来源：http://jqx.quarkkingdee.top

sys.stdout.isatty()
来源：http://vtv.sufxvd.cn

[U40] Py：打印到标准错误
来源：http://dyy.aizwys.cn

print("err", file=sys.stderr)
来源：http://lvo.tanke756.top

[U41] PHP：初始化 Composer 项目
来源：http://vdw.yj20258888.top

composer init;  composer require guzzlehttp/guzzle
来源：http://djq.tarul.cn

[U42] PHP：PSR-4 自动加载
来源：http://mqr.tarul.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://drd.sufxvd.cn

[U43] PHP：声明命名空间
来源：http://isq.guannengcc.top

namespace App\Http;
来源：http://qjo.hcnkem.com

[U44] PHP：开启严格类型
来源：http://svu.hammf.cn

declare(strict_types=1);
来源：http://xwx.wangshuangyany.cn

[U45] PHP：类型声明与返回类型
来源：http://ecu.yuanzhike.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ubq.guannengcc.top

[U46] PHP：可空类型
来源：http://yvm.yuxming.cn

?string $name = null
来源：http://unz.feifeiyinyue.top

[U47] PHP：联合类型
来源：http://ldi.yanxiufei.cn

int|string $id
来源：http://gnc.yueranfly.top

[U48] PHP：纯枚举
来源：http://cnf.jiagoushi.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kle.fktsv.cn

[U49] PHP：只读属性
来源：http://xwg.vehdjk.com

public readonly string $name
来源：http://qrc.jyoumei.cn

[U50] PHP：构造器属性提升
来源：http://kuw.jqgufenzy.top

public function __construct(private int $id) {}
来源：http://oqm.yonumen.top

[U51] PHP：数组解构
来源：http://nyx.hysaishi.cn

[$a, $b] = $arr;
来源：http://ueo.yanxiufei.cn

[U52] PHP：箭头函数
来源：http://vdn.shanyushiyangkeji.top

$double = fn($x) => $x * 2;
来源：http://yvg.zhongyouzk.top

[U53] PHP：空合并运算符
来源：http://ohy.pycfn.com

$v = $a ?? $b ?? "default";
来源：http://jbx.andypj.xyz

[U54] PHP：空安全调用
来源：http://eba.jinqigufen.top

$obj?->method()
来源：http://cvg.vehdjk.com

[U55] PHP：match 表达式
来源：http://vxb.redwolf501.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gcd.yueranfly.top

[U56] PHP：命名参数
来源：http://iue.gaohongyu789.top

f(a: 1, b: 2)
来源：http://etj.52xcode.cn

[U57] PHP：字符串插值
来源：http://opf.chenzaomai.com

"值: {$a}"
来源：http://qep.sufxvd.cn

[U58] PHP：数组三件套
来源：http://ulw.xylfe.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wpy.ctjpmb.com

[U59] PHP：自定义排序
来源：http://bqj.jinyuanbaomall.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wrw.dashuyun.cn

[U60] PHP：JSON 编解码
来源：http://jcq.shanyushiyangkeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jcg.jinghuilouyu.cn

[U61] PHP：正则
来源：http://tve.mhx1999.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lmr.xuanzx.com

[U62] PHP：日期对象
来源：http://krn.aibaodan.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vum.yueranfly.top

[U63] PHP：文件读写
来源：http://uhc.c1oappe.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ays.shangyingyoupin.top

[U64] PHP：目录遍历
来源：http://czf.jianghu66.top

glob("dir/*.php");  scandir("dir");
来源：http://aaq.cheryme.top

[U65] PHP：会话
来源：http://ftv.iojbl.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kng.cheryme.top

[U66] PHP：设置 Cookie
来源：http://vsx.jinqigfzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://isd.xylfe.cn

[U67] PHP：处理文件上传
来源：http://alp.vehdjk.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qxg.yuxming.cn

[U68] PHP：PDO 连接
来源：http://vib.chenlongwang.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ymp.xylfe.cn

[U69] PHP：PDO 预处理
来源：http://hnv.cqqwz.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sdq.tanke756.top

[U70] PHP：PDO 事务
来源：http://hwq.ppjwa.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wst.yfazqb.com

[U71] PHP：抛出异常
来源：http://xbf.hfpthk.cn

throw new RuntimeException("失败", 500);
来源：http://npa.cdnleiting.top

[U72] PHP：写错误日志
来源：http://vvw.jinghuilouyu.cn

error_log("失败: " . $e->getMessage());
来源：http://gzj.ppjwa.cn

[U73] PHP：读取 ini 配置
来源：http://gmt.xinyue.icu

parse_ini_file("config.ini", true)
来源：http://flf.52xcode.cn

[U74] PHP：读取环境变量
来源：http://doz.yangfankeji.com

getenv("APP_ENV") ?: "production"
来源：http://jce.zhijiandao.cn

[U75] PHP：依赖注入
来源：http://trh.chenzaomai.com

composer require psr/container
来源：http://roh.aibaodan.cn

[U76] PHP：简单路由
来源：http://juu.vqdsnc.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rra.sysykeji.top

[U77] PHP：模板渲染
来源：http://cwg.mhx1999.top

composer require twig/twig
来源：http://hpc.epnwcf.com

[U78] PHP：单元测试
来源：http://len.gaohongyu789.top

composer require --dev phpunit/phpunit
来源：http://scc.ppjwa.cn

[U79] PHP：静态分析
来源：http://tbw.ybcxt.top

composer require --dev phpstan/phpstan
来源：http://sia.jinyuanbaomall.cn

[U80] PHP：代码规范修复
来源：http://ssd.yangfankeji.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://lls.feifeiyinyue.top

[U81] JS：初始化项目
来源：http://iao.birdmap.top

npm init -y;  npm i express
来源：http://cjl.yangfankeji.com

[U82] JS：package.json 脚本
来源：http://jdd.hysaishi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://toq.shzxlz.cn

[U83] JS：ES Module 导入导出
来源：http://dth.fengsongda.top

export const a = 1;  import { a } from "./m.js";
来源：http://nnl.ppjwa.cn

[U84] JS：CommonJS 写法
来源：http://xba.aizwys.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tio.bbcook.cn

[U85] JS：可选链
来源：http://fxs.wangdashe.top

a?.b?.c
来源：http://zyj.jianghu66.top

[U86] JS：空值合并
来源：http://bvo.zdbjq.cn

a ?? b
来源：http://nji.yongpay.top

[U87] JS：解构默认值
来源：http://xkc.ivvv.top

const { a = 1, b = 2 } = obj;
来源：http://iek.shanyushiyangtech.top

[U88] JS：对象展开合并
来源：http://mlb.hywenlv.cn

{ ...a, ...b }
来源：http://lua.yuxming.cn

[U89] JS：数组去重
来源：http://vqz.xziqi.cn

[...new Set(arr)]
来源：http://bqv.ybcxt.top

[U90] JS：数字数组排序
来源：http://ixi.aizwys.cn

[...arr].sort((a, b) => a - b)
来源：http://slp.shanyushiyangkeji.top

[U91] JS：对象键值遍历
来源：http://one.shuidangran.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pli.fktsv.cn

[U92] JS：深拷贝
来源：http://xog.xinyue.icu

structuredClone(obj)
来源：http://agc.sjlbkw.cn

[U93] JS：模板字符串
来源：http://jps.fanxiaobao.xyz

`共 ${n} 条`
来源：http://iqx.zhaomingkeji.xyz

[U94] JS：箭头函数
来源：http://now.ehwqpu.com

const double = x => x * 2;
来源：http://wyc.chenjidiqi.icu

[U95] JS：Promise 包装
来源：http://wve.fehbvm.com

new Promise((resolve, reject) => {})
来源：http://kjo.zhiwuduotai.top

[U96] JS：async/await 与异常
来源：http://rev.jianghu66.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rpn.sufxvd.cn

[U97] JS：并发请求
来源：http://xlh.yfazqb.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://vso.fengsongda.top

[U98] JS：fetch 带 JSON
来源：http://bpf.c1oappe.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mkn.zhongyouzk.top

[U99] JS：事件监听
来源：http://fvo.yuxming.cn

el.addEventListener("click", e => {})
来源：http://rlb.yuxming.cn

[U100] JS：DOM 查询
来源：http://tyn.xuetiantiany.cn

document.querySelector(".item")
来源：http://ico.dianchejie.cn

[U101] JS：classList 操作
来源：http://mjj.yuanzhike.top

el.classList.toggle("active")
来源：http://tqy.ctjpmb.com

[U102] JS：本地存储
来源：http://dcx.yanxiufei.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bgx.smart0.xyz

[U103] JS：定时器
来源：http://vbn.aizwys.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uet.xinyue.icu

[U104] JS：防抖
来源：http://uuw.zhijiandao.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zvb.yuanzhike.top

[U105] JS：节流
来源：http://gvf.daxiang520.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vkg.aibaodan.cn

[U106] JS：日期格式化
来源：http://ure.hysaishi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sut.uphjek.com

[U107] JS：数字千分位
来源：http://gzs.yanxiufei.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://avu.cashguo.top

[U108] JS：随机整数
来源：http://kce.feifeiyinyue.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xjs.ybcxt.top

[U109] JS：数组分组
来源：http://nty.cucudq.cn

Object.groupBy(arr, x => x.type)
来源：http://bsk.yj20258888.top

[U110] JS：数组分块
来源：http://gis.cqqwz.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lgy.gzhubu.top

[U111] JS：对象转 Map
来源：http://pfw.guannengcc.top

new Map(Object.entries(obj))
来源：http://szf.cdnleiting.top

[U112] JS：字符串补位
来源：http://lzk.gzhubu.top

"7".padStart(3, "0")
来源：http://imm.gogol.net.cn

[U113] JS：正则替换全部
来源：http://srf.ivvv.top

s.replaceAll("a", "b")
来源：http://jhr.xuetiantiany.cn

[U114] JS：JSON 深比较
来源：http://gge.jlsjyb.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ntd.yuxming.cn

[U115] JS：生成 UUID
来源：http://slu.ppjwa.cn

crypto.randomUUID()
来源：http://auc.feifeiyinyue.top

[U116] JS：类型检查（JSDoc）
来源：http://ehm.yangfankeji.com

/** @param {string} name */ function f(name) {}
来源：http://ucu.jinqigfzy.top

[U117] JS：单元测试
来源：http://mbf.ydjk.org.cn

npm i -D vitest;  npx vitest
来源：http://yso.jyoumei.cn

[U118] JS：开发服务器
来源：http://yqc.zhengqikj.top

npm i -D vite;  npx vite
来源：http://qhq.gzhubu.top

[U119] JS：生产构建
来源：http://jer.cheryme.top

npx vite build
来源：http://bsd.andypj.xyz

[U120] JS：读取环境变量（Vite）
来源：http://sbb.tian-w.cn

import.meta.env.VITE_API_URL
来源：http://tov.shzxlz.cn

================================================================================
来源：http://yza.feifeiyinyue.top

统计汇总
来源：http://veb.52xcode.cn

================================================================================
来源：http://acd.zdbjq.cn

按语言统计（条）：
来源：http://ouc.quarkkingdee.top

Python ......... 252
来源：http://qda.smart0.xyz

PHP ............ 252
来源：http://keb.zhixingplan.top

JavaScript ..... 252
来源：http://men.andypj.xyz

TypeScript ..... 212
来源：http://bwh.guannengcc.top

Java ........... 212
来源：http://wxx.vqdsnc.cn

Go ............. 212
来源：http://ijn.iojbl.cn

Ruby ........... 212
来源：http://crl.gaohongyu789.top

C# ............. 212
来源：http://byh.shuidangran.top

C .............. 30
来源：http://pwt.chenzaomai.com

C++ ............ 30
来源：http://dek.52xcode.cn

SQL ............ 90
来源：http://cta.feifeiyinyue.top

Bash ........... 80
来源：http://ovo.dianchejie.cn

Kotlin ......... 15
来源：http://bbm.yongpay.top

Swift .......... 15
来源：http://qow.jinghuilouyu.cn

Lua ............ 10
来源：http://ggj.chenjidiqi.icu

Perl ........... 10
来源：http://vkw.shzxlz.cn

Scala .......... 10
来源：http://ihr.ydjk.org.cn

------------------------------------
来源：http://utk.fzhhl.top

合计 ........... 2106 条
来源：http://xlk.vqdsnc.cn

按章节统计：
来源：http://ezh.bbcook.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ihy.tanke756.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yja.zhoulong.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gmo.hongshengwenyu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fme.nanxinkj.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mah.shuidangran.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jsj.bjfxy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sds.ctjpmb.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://err.gaohongyu789.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wzo.aizwys.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://apb.daria6918.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://edg.ppjwa.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rve.gogol.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qnj.xylfe.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tzc.pengpengdd.cyou

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://iby.tanke756.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rnh.daxiang520.top

Q SQL 专题                              90
来源：http://qck.hnxiangtu.top

R Bash 专题                             80
来源：http://cbx.gotoacloud.top

S C / C++ 专题                          60
来源：http://ycm.zhijiandao.cn

T 其他语言补充                          60
来源：http://erd.jiagoushi.top

U 高频实用片段                         120
来源：http://apd.nanxinkj.top

------------------------------------
来源：http://agc.daria6918.cn

合计                                  2106 条
来源：http://tvu.yj20258888.top

--------------------------------------------------------------------------------
来源：http://jgb.havefunace.top

使用提醒
来源：http://oxm.fengsongda.top

--------------------------------------------------------------------------------
来源：http://srs.zdbjq.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ash.nwbrower.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://abs.yuxming.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ipq.kuanghao11.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ncq.quarkkingdee.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://rck.hywenlv.cn

—— 文件结束 ——
来源：http://arn.dianchejie.cn

================================================================================
来源：http://hoz.52xcode.cn

程序语言常见例子速查手册（2024 版）
来源：http://pjo.nanxuanxn.top

Common Programming Examples Cheat Book
来源：http://kll.tianlin.xyz

================================================================================
来源：http://dkx.jiagoushi.top

【收录内容】
来源：http://vji.epnwcf.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://jrn.jianghu66.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bge.redwolf501.top

SQL · Bash · C · C++
来源：http://rzb.pycfn.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ztg.ydjk.org.cn

【使用说明】
来源：http://mol.52xcode.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jyp.jqgfzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://sgc.xziqi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://trq.yanxiufei.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lqt.52xcode.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wrk.xylfe.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://adm.yvedp.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hvu.zhongyouzk.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lxr.pycfn.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jel.uphjek.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sqg.vqdsnc.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tzv.zhengqikj.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://alg.mhx1999.top

【文件统计】
来源：http://tyo.chenzaomai.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jnk.xylfe.cn

--------------------------------------------------------------------------------
来源：http://npx.yonumen.top

目  录
来源：http://dzt.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://hbu.yangfankeji.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gmr.cashguo.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ods.ydzc1.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wja.gotoacloud.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ebb.nanxuanxn.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ffa.yj202588.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://izu.zhengqikj.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://edf.birdmap.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xfe.aizwys.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://phc.zhaomingkeji.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pzq.zhongyouzk.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ddp.hnqzz.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lku.ehwqpu.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://czr.sweek.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rwi.meibo888.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://imu.zhiwuduotai.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nrj.hcnkem.com

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yjm.aizwys.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://noz.yuanzhike.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gvq.iojbl.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://kra.zhongyouzk.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rnh.vqdsnc.cn

================================================================================
来源：http://qrf.zhongyouzk.top

A. 基础语法与类型
来源：http://sdx.yongpay.top

================================================================================
来源：http://tkr.yueranfly.top

[A01] Hello World
来源：http://eqc.yfazqb.com

Py:   print("Hello, World!")
来源：http://plg.haohaochexian.top

PHP:  echo "Hello, World!";
来源：http://qop.chenlongwang.top

JS:   console.log("Hello, World!");
来源：http://wiv.shangyingyoupin.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bst.sxryk.cn

Java: System.out.println("Hello, World!");
来源：http://xcl.ydzc1.top

Go:   fmt.Println("Hello, World!")
来源：http://efw.shuidangran.top

Ruby: puts "Hello, World!"
来源：http://emx.xuetiantiany.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://dcd.fzhhl.top

[A02] 变量声明与赋值
来源：http://euw.dianchejie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://niu.zhaomingkeji.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://vbz.haohaochexian.top

JS:   let name = "Alex"; const age = 20;
来源：http://oxl.aibaodan.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://udh.epnwcf.com

Java: String name = "Alex"; int age = 20;
来源：http://yom.zhijiandao.cn

Go:   name := "Alex"; age := 20
来源：http://avn.hnxiangtu.top

Ruby: name = "Alex"; age = 20
来源：http://sfl.jinyuanbaomall.cn


<!-- 参考信息 -->