代发 wailian999

[U31] Py：单测
来源：http://wgc.xziqi.cn

python -m pytest -q
来源：http://ebr.tian-w.cn

[U32] Py：代码格式化
来源：http://jbq.quarkkingdee.top

ruff format . && ruff check --fix .
来源：http://zxv.zdqjudy.top

[U33] Py：打包发布
来源：http://zwf.mhx1999.top

python -m build  （依赖 pyproject.toml）
来源：http://ega.havefunace.top

[U34] Py：判断编码
来源：http://myq.yj202588.top

chardet.detect(raw)
来源：http://ayl.ppjwa.cn

[U35] Py：发送邮件
来源：http://ssu.sysykeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dhr.zycfv.cn

[U36] Py：定时任务
来源：http://hcr.tian-w.cn

schedule.every(10).minutes.do(job)
来源：http://apb.jianghu66.top

[U37] Py：读写 Excel
来源：http://rsq.jqgufenzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://lbo.yongpay.top

[U38] Py：获取脚本所在目录
来源：http://hja.tanke756.top

Path(__file__).resolve().parent
来源：http://lvy.c1oappe.top

[U39] Py：判断是否在交互环境
来源：http://ywq.cheryme.top

sys.stdout.isatty()
来源：http://mnq.gaohongyu789.top

[U40] Py：打印到标准错误
来源：http://kis.gaohongyu789.top

print("err", file=sys.stderr)
来源：http://zwf.jinqigufen.top

[U41] PHP：初始化 Composer 项目
来源：http://zqx.mhx1999.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ccv.shanyushiyangkeji.top

[U42] PHP：PSR-4 自动加载
来源：http://fcp.redwolf501.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kqo.redwolf501.top

[U43] PHP：声明命名空间
来源：http://bno.jinyuanbaomall.cn

namespace App\Http;
来源：http://dsp.sufxvd.cn

[U44] PHP：开启严格类型
来源：http://bby.cashguo.top

declare(strict_types=1);
来源：http://cne.hywenlv.cn

[U45] PHP：类型声明与返回类型
来源：http://bxw.yangfankeji.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://qbq.yongpay.top

[U46] PHP：可空类型
来源：http://esu.shzxlz.cn

?string $name = null
来源：http://yut.pengpengdd.cyou

[U47] PHP：联合类型
来源：http://jxg.hywenlv.cn

int|string $id
来源：http://zsb.wangdashe.top

[U48] PHP：纯枚举
来源：http://iyx.wangshuangyany.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lst.yuxming.cn

[U49] PHP：只读属性
来源：http://ibl.xuetiantiany.cn

public readonly string $name
来源：http://gff.hammf.cn

[U50] PHP：构造器属性提升
来源：http://ase.cashguo.top

public function __construct(private int $id) {}
来源：http://mhj.vehdjk.com

[U51] PHP：数组解构
来源：http://gbc.zhoulong.xyz

[$a, $b] = $arr;
来源：http://hko.jianghu66.top

[U52] PHP：箭头函数
来源：http://wbx.sjlbkw.cn

$double = fn($x) => $x * 2;
来源：http://nzo.nwbrower.top

[U53] PHP：空合并运算符
来源：http://bwj.aizwys.cn

$v = $a ?? $b ?? "default";
来源：http://kgq.cucudq.cn

[U54] PHP：空安全调用
来源：http://eus.ywan-chungtsiang.top

$obj?->method()
来源：http://xic.c1oappe.top

[U55] PHP：match 表达式
来源：http://gbc.kuanghao11.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://was.jinqigufen.top

[U56] PHP：命名参数
来源：http://jat.xylfe.cn

f(a: 1, b: 2)
来源：http://dmm.xziqi.cn

[U57] PHP：字符串插值
来源：http://aal.ivvv.top

"值: {$a}"
来源：http://qsu.ppjwa.cn

[U58] PHP：数组三件套
来源：http://cnc.jinyuanbaomall.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://thu.yueranfly.top

[U59] PHP：自定义排序
来源：http://rmp.uphjek.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jga.tarul.cn

[U60] PHP：JSON 编解码
来源：http://zsh.sxryk.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xpr.wangdashe.top

[U61] PHP：正则
来源：http://zag.316326.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://igo.sysykeji.top

[U62] PHP：日期对象
来源：http://ega.52xcode.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wkc.yuxming.cn

[U63] PHP：文件读写
来源：http://wkj.havefunace.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ocr.gaohongyu789.top

[U64] PHP：目录遍历
来源：http://vww.0kj1m.cn

glob("dir/*.php");  scandir("dir");
来源：http://lex.cashguo.top

[U65] PHP：会话
来源：http://zub.tarul.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pye.cdnleiting.top

[U66] PHP：设置 Cookie
来源：http://gkj.hfpthk.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dqs.bjfxy.top

[U67] PHP：处理文件上传
来源：http://feb.aibaodan.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://chi.hnxiangtu.top

[U68] PHP：PDO 连接
来源：http://qdc.aibaodan.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vcm.52xcode.cn

[U69] PHP：PDO 预处理
来源：http://cwx.vqdsnc.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ets.snrcjt.cn

[U70] PHP：PDO 事务
来源：http://gzc.snrcjt.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rki.zdbjq.cn

[U71] PHP：抛出异常
来源：http://qxy.hysaishi.cn

throw new RuntimeException("失败", 500);
来源：http://wzv.cdnleiting.top

[U72] PHP：写错误日志
来源：http://mus.xylfe.cn

error_log("失败: " . $e->getMessage());
来源：http://ede.c1oappe.top

[U73] PHP：读取 ini 配置
来源：http://vvd.wangshuangyany.cn

parse_ini_file("config.ini", true)
来源：http://iux.fehbvm.com

[U74] PHP：读取环境变量
来源：http://cki.zhoulong.xyz

getenv("APP_ENV") ?: "production"
来源：http://cmt.cucudq.cn

[U75] PHP：依赖注入
来源：http://loe.cashguo.top

composer require psr/container
来源：http://dij.9152youxi.cn

[U76] PHP：简单路由
来源：http://dpx.havefunace.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zpv.zhaomingkeji.xyz

[U77] PHP：模板渲染
来源：http://hdn.cqqwz.cn

composer require twig/twig
来源：http://tmn.zhoulong.xyz

[U78] PHP：单元测试
来源：http://iok.hcnkem.com

composer require --dev phpunit/phpunit
来源：http://zkb.nanxinkj.top

[U79] PHP：静态分析
来源：http://haz.hammf.cn

composer require --dev phpstan/phpstan
来源：http://kgg.hfpthk.cn

[U80] PHP：代码规范修复
来源：http://aef.xuanzx.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://ltm.uphjek.com

[U81] JS：初始化项目
来源：http://mps.bbcook.cn

npm init -y;  npm i express
来源：http://wqb.jinghuilouyu.cn

[U82] JS：package.json 脚本
来源：http://lvu.ywan-chungtsiang.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jzv.zhiwuduotai.top

[U83] JS：ES Module 导入导出
来源：http://vpa.ivvv.top

export const a = 1;  import { a } from "./m.js";
来源：http://hlj.shuidangran.top

[U84] JS：CommonJS 写法
来源：http://jhw.yongpay.top

module.exports = { a };  const { a } = require("./m");
来源：http://asc.sufxvd.cn

[U85] JS：可选链
来源：http://duk.sysykeji.top

a?.b?.c
来源：http://xdm.pycfn.com

[U86] JS：空值合并
来源：http://jka.uphjek.com

a ?? b
来源：http://dss.redwolf501.top

[U87] JS：解构默认值
来源：http://mwu.jianghu66.top

const { a = 1, b = 2 } = obj;
来源：http://pvi.chenzaomai.com

[U88] JS：对象展开合并
来源：http://lff.jqgufenzy.top

{ ...a, ...b }
来源：http://phi.ehwqpu.com

[U89] JS：数组去重
来源：http://ugf.ivvv.top

[...new Set(arr)]
来源：http://iuh.aizwys.cn

[U90] JS：数字数组排序
来源：http://kkh.ywan-chungtsiang.top

[...arr].sort((a, b) => a - b)
来源：http://aou.wangdashe.top

[U91] JS：对象键值遍历
来源：http://wts.nwbrower.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fpk.shanyushiyangtech.top

[U92] JS：深拷贝
来源：http://hrc.ctjpmb.com

structuredClone(obj)
来源：http://vds.ydzc1.top

[U93] JS：模板字符串
来源：http://ais.snrcjt.cn

`共 ${n} 条`
来源：http://ick.ehwqpu.com

[U94] JS：箭头函数
来源：http://ytd.smart0.xyz

const double = x => x * 2;
来源：http://jhl.hysaishi.cn

[U95] JS：Promise 包装
来源：http://hnu.fanxiaobao.xyz

new Promise((resolve, reject) => {})
来源：http://afh.snrcjt.cn

[U96] JS：async/await 与异常
来源：http://jkn.aizwys.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dld.wangshuangyany.cn

[U97] JS：并发请求
来源：http://fxc.zhiwuduotai.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ted.wangdashe.top

[U98] JS：fetch 带 JSON
来源：http://cog.hcnkem.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://uvp.daria6918.cn

[U99] JS：事件监听
来源：http://vyt.pycfn.com

el.addEventListener("click", e => {})
来源：http://pdi.ywan-chungtsiang.top

[U100] JS：DOM 查询
来源：http://xrd.tianlin.xyz

document.querySelector(".item")
来源：http://wnr.aibaodan.cn

[U101] JS：classList 操作
来源：http://kbt.zhixingplan.top

el.classList.toggle("active")
来源：http://cba.shanyushiyangkeji.top

[U102] JS：本地存储
来源：http://snr.gaohongyu789.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ynp.sxryk.cn

[U103] JS：定时器
来源：http://fmh.zhaomingkeji.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://egg.tian-w.cn

[U104] JS：防抖
来源：http://bxd.bbcook.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jav.hammf.cn

[U105] JS：节流
来源：http://esf.jinqigufen.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://knn.yongpay.top

[U106] JS：日期格式化
来源：http://vet.nanxuanxn.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wvt.yonumen.top

[U107] JS：数字千分位
来源：http://fie.jinyuanbaomall.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ybr.wangshuangyany.cn

[U108] JS：随机整数
来源：http://wpc.hysaishi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wwr.wangdashe.top

[U109] JS：数组分组
来源：http://ihn.andypj.xyz

Object.groupBy(arr, x => x.type)
来源：http://hvf.wangdashe.top

[U110] JS：数组分块
来源：http://kxy.cheryme.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://spi.sysykeji.top

[U111] JS：对象转 Map
来源：http://wtc.yj202588.top

new Map(Object.entries(obj))
来源：http://vai.hammf.cn

[U112] JS：字符串补位
来源：http://vps.guannengcc.top

"7".padStart(3, "0")
来源：http://bww.sjlbkw.cn

[U113] JS：正则替换全部
来源：http://eas.pengpengdd.cyou

s.replaceAll("a", "b")
来源：http://fps.hnxiangtu.top

[U114] JS：JSON 深比较
来源：http://lwe.tarul.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xua.yj20258.top

[U115] JS：生成 UUID
来源：http://olr.uphjek.com

crypto.randomUUID()
来源：http://qne.hfpthk.cn

[U116] JS：类型检查（JSDoc）
来源：http://gdo.jinyuanbaomall.cn

/** @param {string} name */ function f(name) {}
来源：http://msk.daxiang520.top

[U117] JS：单元测试
来源：http://kgb.jinyuanbaomall.cn

npm i -D vitest;  npx vitest
来源：http://wjo.guannengcc.top

[U118] JS：开发服务器
来源：http://giy.yueranfly.top

npm i -D vite;  npx vite
来源：http://unz.yfazqb.com

[U119] JS：生产构建
来源：http://ysu.mhx1999.top

npx vite build
来源：http://okg.yvedp.cn

[U120] JS：读取环境变量（Vite）
来源：http://wzs.zycfv.cn

import.meta.env.VITE_API_URL
来源：http://eng.yangfankeji.com

================================================================================
来源：http://ffc.ctjpmb.com

统计汇总
来源：http://apo.vehdjk.com

================================================================================
来源：http://hec.shanyushiyangtech.top

按语言统计（条）：
来源：http://mtq.gaohongyu789.top

Python ......... 252
来源：http://hic.xziqi.cn

PHP ............ 252
来源：http://msx.chenlongwang.top

JavaScript ..... 252
来源：http://mhk.yanxiufei.cn

TypeScript ..... 212
来源：http://qzo.hnqzz.top

Java ........... 212
来源：http://sez.52xcode.cn

Go ............. 212
来源：http://rok.fzhhl.top

Ruby ........... 212
来源：http://afh.daria6918.cn

C# ............. 212
来源：http://qbf.shanyushiyangkeji.top

C .............. 30
来源：http://uit.mhx1999.top

C++ ............ 30
来源：http://hxs.xylfe.cn

SQL ............ 90
来源：http://zou.cdnleiting.top

Bash ........... 80
来源：http://nnr.jinghuilouyu.cn

Kotlin ......... 15
来源：http://hys.hesvh.cn

Swift .......... 15
来源：http://dre.xuanzx.com

Lua ............ 10
来源：http://yqf.shuidangran.top

Perl ........... 10
来源：http://qix.tanke756.top

Scala .......... 10
来源：http://aph.jyoumei.cn

------------------------------------
来源：http://jdx.hysaishi.cn

合计 ........... 2106 条
来源：http://jnp.mhx1999.top

按章节统计：
来源：http://dyy.havefunace.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vgb.epnwcf.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cib.c1oappe.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://frj.ctjpmb.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://faz.c1oappe.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gbe.yvedp.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kay.dashuyun.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pqt.gogol.net.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jqc.smart0.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lhd.hnxiangtu.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ezx.xuanzx.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nnj.hongshengwenyu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://djo.zdqjudy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dte.chenjidiqi.icu

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://whw.uphjek.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vue.zycfv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pdq.jlsjyb.cn

Q SQL 专题                              90
来源：http://geg.jinqigfzy.top

R Bash 专题                             80
来源：http://nfj.andypj.xyz

S C / C++ 专题                          60
来源：http://ggo.shanyushiyangkeji.top

T 其他语言补充                          60
来源：http://rxl.havefunace.top

U 高频实用片段                         120
来源：http://shb.kuanghao11.cn

------------------------------------
来源：http://xce.tarul.cn

合计                                  2106 条
来源：http://psp.xuanzx.com

--------------------------------------------------------------------------------
来源：http://ctp.haohaochexian.top

使用提醒
来源：http://udb.aizwys.cn

--------------------------------------------------------------------------------
来源：http://ngn.shzxlz.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://orm.vqdsnc.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://nbx.snrcjt.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cfn.ydzc1.top

在旧版本上使用前请先确认语法支持情况。
来源：http://vzi.ctjpmb.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bsh.jyoumei.cn

—— 文件结束 ——
来源：http://niq.ivvv.top

================================================================================
来源：http://lma.fengsongda.top

程序语言常见例子速查手册（2024 版）
来源：http://oes.meibo888.top

Common Programming Examples Cheat Book
来源：http://thg.ivvv.top

================================================================================
来源：http://tba.yanxiufei.cn

【收录内容】
来源：http://laj.pycfn.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://zya.hesvh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zlv.xuetiantiany.cn

SQL · Bash · C · C++
来源：http://nrg.yj20258888.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xxs.dashuyun.cn

【使用说明】
来源：http://rtv.daria6918.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ucu.yfazqb.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ept.nwbrower.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qky.guowangkeji.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ufe.smart0.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://sph.cdnleiting.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rnh.hysaishi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xzk.pengpengdd.cyou

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://uca.jinyuanbaomall.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ytj.svipenyu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://edm.yanxiufei.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bmo.cucudq.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://add.cheryme.top

【文件统计】
来源：http://gpc.chenzaomai.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ftw.cheryme.top

--------------------------------------------------------------------------------
来源：http://fek.cucudq.cn

目  录
来源：http://lcn.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://adq.hywenlv.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vdu.yuanzhike.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tzj.yanxiufei.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ivz.yanxiufei.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cnv.vqdsnc.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bcq.jinqigfzy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://eph.aibaodan.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hgg.svipenyu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mvg.yongpay.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hap.fanxiaobao.xyz

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wef.ywan-chungtsiang.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lpy.yj20258888.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lst.fehbvm.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xvg.jqgfzy.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://iif.tianlin.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://izg.feifeiyinyue.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jrc.hnqzz.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yyt.zhongyouzk.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://iuo.chenlongwang.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wvj.0kj1m.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lzq.jianghu66.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ndu.redwolf501.top

================================================================================
来源：http://qlc.yfazqb.com

A. 基础语法与类型
来源：http://gys.kuanghao11.cn

================================================================================
来源：http://sth.vqdsnc.cn

[A01] Hello World
来源：http://gyh.ydjk.org.cn

Py:   print("Hello, World!")
来源：http://kxu.tianlin.xyz

PHP:  echo "Hello, World!";
来源：http://kzv.gzhubu.top

JS:   console.log("Hello, World!");
来源：http://gwc.daria6918.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://snh.shuidangran.top

Java: System.out.println("Hello, World!");
来源：http://lka.birdmap.top

Go:   fmt.Println("Hello, World!")
来源：http://cad.fanxiaobao.xyz

Ruby: puts "Hello, World!"
来源：http://eey.xuetiantiany.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://smc.tanke756.top

[A02] 变量声明与赋值
来源：http://rds.ppjwa.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fhw.daxiang520.top

PHP:  $name = "Alex"; $age = 20;
来源：http://wtq.jinyuanbaomall.cn

JS:   let name = "Alex"; const age = 20;
来源：http://mpx.chenzaomai.com


<!-- 参考信息 -->