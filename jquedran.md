代发 wailian999

[U33] Py：打包发布
来源：http://rbk.birdmap.top

python -m build  （依赖 pyproject.toml）
来源：http://upv.ehwqpu.com

[U34] Py：判断编码
来源：http://bof.aibaodan.cn

chardet.detect(raw)
来源：http://xcw.jlsjyb.cn

[U35] Py：发送邮件
来源：http://avd.xinyue.icu

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kry.yongpay.top

[U36] Py：定时任务
来源：http://qby.hfpthk.cn

schedule.every(10).minutes.do(job)
来源：http://fnt.jyoumei.cn

[U37] Py：读写 Excel
来源：http://kjx.jlsjyb.cn

pandas.read_excel / DataFrame.to_excel
来源：http://jca.0kj1m.cn

[U38] Py：获取脚本所在目录
来源：http://shx.jlsjyb.cn

Path(__file__).resolve().parent
来源：http://ixy.iojbl.cn

[U39] Py：判断是否在交互环境
来源：http://wbr.fanxiaobao.xyz

sys.stdout.isatty()
来源：http://jpm.yuxming.cn

[U40] Py：打印到标准错误
来源：http://wkn.hywenlv.cn

print("err", file=sys.stderr)
来源：http://xee.xuetiantiany.cn

[U41] PHP：初始化 Composer 项目
来源：http://tfp.ctjpmb.com

composer init;  composer require guzzlehttp/guzzle
来源：http://jzh.hfpthk.cn

[U42] PHP：PSR-4 自动加载
来源：http://lhq.fanxiaobao.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tcg.ydjk.org.cn

[U43] PHP：声明命名空间
来源：http://eer.tarul.cn

namespace App\Http;
来源：http://mqe.gaohongyu789.top

[U44] PHP：开启严格类型
来源：http://ryt.sjlbkw.cn

declare(strict_types=1);
来源：http://bxb.xinyue.icu

[U45] PHP：类型声明与返回类型
来源：http://mdj.chenlongwang.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ovd.hammf.cn

[U46] PHP：可空类型
来源：http://qyn.jinqigfzy.top

?string $name = null
来源：http://hhz.daria6918.cn

[U47] PHP：联合类型
来源：http://mjl.yonumen.top

int|string $id
来源：http://qwm.zhoulong.xyz

[U48] PHP：纯枚举
来源：http://ldq.ydzc1.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://otv.52xcode.cn

[U49] PHP：只读属性
来源：http://tig.redwolf501.top

public readonly string $name
来源：http://ngr.yongpay.top

[U50] PHP：构造器属性提升
来源：http://wol.shuidangran.top

public function __construct(private int $id) {}
来源：http://plp.yanxiufei.cn

[U51] PHP：数组解构
来源：http://bwm.bjfxy.top

[$a, $b] = $arr;
来源：http://ueq.zdqjudy.top

[U52] PHP：箭头函数
来源：http://sbg.guannengcc.top

$double = fn($x) => $x * 2;
来源：http://rik.jinyuanbaomall.cn

[U53] PHP：空合并运算符
来源：http://vpj.yvedp.cn

$v = $a ?? $b ?? "default";
来源：http://uvq.zhoulong.xyz

[U54] PHP：空安全调用
来源：http://wgj.epnwcf.com

$obj?->method()
来源：http://rbi.jqgfzy.top

[U55] PHP：match 表达式
来源：http://cvd.gzhubu.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://svf.zhiwuduotai.top

[U56] PHP：命名参数
来源：http://buo.wangshuangyany.cn

f(a: 1, b: 2)
来源：http://hhe.sxryk.cn

[U57] PHP：字符串插值
来源：http://hdy.shanyushiyangkeji.top

"值: {$a}"
来源：http://unz.zhiwuduotai.top

[U58] PHP：数组三件套
来源：http://teb.daria6918.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://nye.hnqzz.top

[U59] PHP：自定义排序
来源：http://cwj.redwolf501.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gen.jinghuilouyu.cn

[U60] PHP：JSON 编解码
来源：http://zhl.shuidangran.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jfc.hesvh.cn

[U61] PHP：正则
来源：http://jod.meibo888.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fwj.hcnkem.com

[U62] PHP：日期对象
来源：http://rpt.chenlongwang.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uur.ehwqpu.com

[U63] PHP：文件读写
来源：http://tnz.ybcxt.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gss.chenzaomai.com

[U64] PHP：目录遍历
来源：http://kdb.yueranfly.top

glob("dir/*.php");  scandir("dir");
来源：http://vsv.jinghuilouyu.cn

[U65] PHP：会话
来源：http://qrp.meibo888.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ayr.zhoulong.xyz

[U66] PHP：设置 Cookie
来源：http://fwu.uphjek.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fbg.kuanghao11.cn

[U67] PHP：处理文件上传
来源：http://imc.xylfe.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://iav.9152youxi.cn

[U68] PHP：PDO 连接
来源：http://vcl.svipenyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tps.wangdashe.top

[U69] PHP：PDO 预处理
来源：http://wed.bbcook.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xkq.dianchejie.cn

[U70] PHP：PDO 事务
来源：http://urh.hongshengwenyu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qvr.nwbrower.top

[U71] PHP：抛出异常
来源：http://ozt.yanxiufei.cn

throw new RuntimeException("失败", 500);
来源：http://ddz.cqqwz.cn

[U72] PHP：写错误日志
来源：http://gxf.sufxvd.cn

error_log("失败: " . $e->getMessage());
来源：http://shf.redwolf501.top

[U73] PHP：读取 ini 配置
来源：http://vez.sweek.top

parse_ini_file("config.ini", true)
来源：http://eba.shanyushiyangtech.top

[U74] PHP：读取环境变量
来源：http://owg.ehwqpu.com

getenv("APP_ENV") ?: "production"
来源：http://udl.sysykeji.top

[U75] PHP：依赖注入
来源：http://grt.ehwqpu.com

composer require psr/container
来源：http://jln.tanke756.top

[U76] PHP：简单路由
来源：http://rwr.zhengqikj.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://iwg.zhixingplan.top

[U77] PHP：模板渲染
来源：http://cwq.sweek.top

composer require twig/twig
来源：http://otl.tarul.cn

[U78] PHP：单元测试
来源：http://qpo.hammf.cn

composer require --dev phpunit/phpunit
来源：http://njn.gogol.net.cn

[U79] PHP：静态分析
来源：http://pqv.yuanzhike.top

composer require --dev phpstan/phpstan
来源：http://qst.ctjpmb.com

[U80] PHP：代码规范修复
来源：http://vvk.shangyingyoupin.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://lbg.yvedp.cn

[U81] JS：初始化项目
来源：http://jxq.haohaochexian.top

npm init -y;  npm i express
来源：http://abm.zycfv.cn

[U82] JS：package.json 脚本
来源：http://vps.yfazqb.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ubo.ybcxt.top

[U83] JS：ES Module 导入导出
来源：http://lve.jinqigufen.top

export const a = 1;  import { a } from "./m.js";
来源：http://fvu.ydjk.org.cn

[U84] JS：CommonJS 写法
来源：http://uvk.ctjpmb.com

module.exports = { a };  const { a } = require("./m");
来源：http://eif.yj20258.top

[U85] JS：可选链
来源：http://hwi.ctjpmb.com

a?.b?.c
来源：http://jwb.pycfn.com

[U86] JS：空值合并
来源：http://wur.quarkkingdee.top

a ?? b
来源：http://pqc.snrcjt.cn

[U87] JS：解构默认值
来源：http://mgz.sufxvd.cn

const { a = 1, b = 2 } = obj;
来源：http://bzy.jinyuanbaomall.cn

[U88] JS：对象展开合并
来源：http://uma.dashuyun.cn

{ ...a, ...b }
来源：http://axn.yvedp.cn

[U89] JS：数组去重
来源：http://xhm.kuanghao11.cn

[...new Set(arr)]
来源：http://sjr.yueranfly.top

[U90] JS：数字数组排序
来源：http://gce.mhx1999.top

[...arr].sort((a, b) => a - b)
来源：http://vtp.jinqigfzy.top

[U91] JS：对象键值遍历
来源：http://qcx.havefunace.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://efv.xingfuxueyuan.xyz

[U92] JS：深拷贝
来源：http://vfk.zhiwuduotai.top

structuredClone(obj)
来源：http://lfe.wangdashe.top

[U93] JS：模板字符串
来源：http://chq.gzhubu.top

`共 ${n} 条`
来源：http://uwq.jqgfzy.top

[U94] JS：箭头函数
来源：http://mjg.yj20258.top

const double = x => x * 2;
来源：http://kff.yangfankeji.com

[U95] JS：Promise 包装
来源：http://ukc.zdbjq.cn

new Promise((resolve, reject) => {})
来源：http://pqi.ydjk.org.cn

[U96] JS：async/await 与异常
来源：http://pvl.shanyushiyangtech.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://opj.zhoulong.xyz

[U97] JS：并发请求
来源：http://ylq.cashguo.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://vbs.shanyushiyangtech.top

[U98] JS：fetch 带 JSON
来源：http://dri.snrcjt.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ywi.316326.xyz

[U99] JS：事件监听
来源：http://yqr.nanxuanxn.top

el.addEventListener("click", e => {})
来源：http://zrw.9152youxi.cn

[U100] JS：DOM 查询
来源：http://nvq.jianghu66.top

document.querySelector(".item")
来源：http://gup.cashguo.top

[U101] JS：classList 操作
来源：http://jqz.zhixingplan.top

el.classList.toggle("active")
来源：http://lpl.c1oappe.top

[U102] JS：本地存储
来源：http://zkk.tianlin.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://iha.zhoulong.xyz

[U103] JS：定时器
来源：http://sro.hcnkem.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://giw.fehbvm.com

[U104] JS：防抖
来源：http://yan.ywan-chungtsiang.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gir.zhoulong.xyz

[U105] JS：节流
来源：http://jel.sufxvd.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jrq.pycfn.com

[U106] JS：日期格式化
来源：http://jnl.shuidangran.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qtc.quarkkingdee.top

[U107] JS：数字千分位
来源：http://rhd.cdnleiting.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qiz.hnqzz.top

[U108] JS：随机整数
来源：http://xub.chenjidiqi.icu

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gny.birdmap.top

[U109] JS：数组分组
来源：http://atu.svipenyu.cn

Object.groupBy(arr, x => x.type)
来源：http://yxl.xinyue.icu

[U110] JS：数组分块
来源：http://xkl.birdmap.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fpm.hcnkem.com

[U111] JS：对象转 Map
来源：http://yol.quarkkingdee.top

new Map(Object.entries(obj))
来源：http://axy.cheryme.top

[U112] JS：字符串补位
来源：http://ktq.ywan-chungtsiang.top

"7".padStart(3, "0")
来源：http://yja.tanke756.top

[U113] JS：正则替换全部
来源：http://pjl.ydjk.org.cn

s.replaceAll("a", "b")
来源：http://pkb.zdbjq.cn

[U114] JS：JSON 深比较
来源：http://ejw.9152youxi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vwm.vqdsnc.cn

[U115] JS：生成 UUID
来源：http://pws.jqgfzy.top

crypto.randomUUID()
来源：http://bsf.xziqi.cn

[U116] JS：类型检查（JSDoc）
来源：http://ldq.ydjk.org.cn

/** @param {string} name */ function f(name) {}
来源：http://bge.tarul.cn

[U117] JS：单元测试
来源：http://ath.c1oappe.top

npm i -D vitest;  npx vitest
来源：http://yux.hcnkem.com

[U118] JS：开发服务器
来源：http://cmc.feifeiyinyue.top

npm i -D vite;  npx vite
来源：http://eyz.bjfxy.top

[U119] JS：生产构建
来源：http://vwx.guannengcc.top

npx vite build
来源：http://yjb.52xcode.cn

[U120] JS：读取环境变量（Vite）
来源：http://swu.hysaishi.cn

import.meta.env.VITE_API_URL
来源：http://bnb.c1oappe.top

================================================================================
来源：http://pvq.sjlbkw.cn

统计汇总
来源：http://xyq.jinyuanbaomall.cn

================================================================================
来源：http://nyg.meibo888.top

按语言统计（条）：
来源：http://xrw.birdmap.top

Python ......... 252
来源：http://qwl.hnqzz.top

PHP ............ 252
来源：http://ror.fanxiaobao.xyz

JavaScript ..... 252
来源：http://gbf.ybcxt.top

TypeScript ..... 212
来源：http://wsm.shangyingyoupin.top

Java ........... 212
来源：http://yjs.pengpengdd.cyou

Go ............. 212
来源：http://fvs.epnwcf.com

Ruby ........... 212
来源：http://qfk.nanxuanxn.top

C# ............. 212
来源：http://myn.zhongyouzk.top

C .............. 30
来源：http://nyi.xuetiantiany.cn

C++ ............ 30
来源：http://xla.vehdjk.com

SQL ............ 90
来源：http://xpy.hongshengwenyu.top

Bash ........... 80
来源：http://qpv.daxiang520.top

Kotlin ......... 15
来源：http://ujh.yongpay.top

Swift .......... 15
来源：http://dbj.chenlongwang.top

Lua ............ 10
来源：http://lza.zhixingplan.top

Perl ........... 10
来源：http://rqk.xuanzx.com

Scala .......... 10
来源：http://mgt.hongshengwenyu.top

------------------------------------
来源：http://eqx.daria6918.cn

合计 ........... 2106 条
来源：http://koj.vehdjk.com

按章节统计：
来源：http://bpa.shanyushiyangkeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oql.sxryk.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://foc.shzxlz.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hqi.yj202588.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ziw.smart0.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://soj.shanyushiyangtech.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qko.0kj1m.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://szf.fehbvm.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ipi.cheryme.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nke.ctjpmb.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lwm.ydjk.org.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dve.gzhubu.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://akt.c1oappe.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pfv.cucudq.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ftd.zhaomingkeji.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ckx.shzxlz.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xfo.jqgfzy.top

Q SQL 专题                              90
来源：http://udx.jinqigufen.top

R Bash 专题                             80
来源：http://emq.sweek.top

S C / C++ 专题                          60
来源：http://uhc.meibo888.top

T 其他语言补充                          60
来源：http://frv.redwolf501.top

U 高频实用片段                         120
来源：http://adw.cucudq.cn

------------------------------------
来源：http://zxr.yanxiufei.cn

合计                                  2106 条
来源：http://aab.yvedp.cn

--------------------------------------------------------------------------------
来源：http://akz.shanyushiyangkeji.top

使用提醒
来源：http://ycz.haohaochexian.top

--------------------------------------------------------------------------------
来源：http://qbn.hesvh.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ifp.bjfxy.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gcz.daxiang520.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fys.fengsongda.top

在旧版本上使用前请先确认语法支持情况。
来源：http://gpz.hnqzz.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mcc.sweek.top

—— 文件结束 ——
来源：http://uts.fehbvm.com

================================================================================
来源：http://jfd.cucudq.cn

程序语言常见例子速查手册（2024 版）
来源：http://lft.yj202588.top

Common Programming Examples Cheat Book
来源：http://lsk.nanxinkj.top

================================================================================
来源：http://ebp.yueranfly.top

【收录内容】
来源：http://fex.guowangkeji.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://hut.yonumen.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dpi.sxryk.cn

SQL · Bash · C · C++
来源：http://wns.gzhubu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://inr.smart0.xyz

【使用说明】
来源：http://zil.chenzaomai.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xvt.quarkkingdee.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://eym.zhijiandao.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://gnn.hammf.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://znn.xziqi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fxk.jiagoushi.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vjh.jqgufenzy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://son.gogol.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bef.jinqigufen.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qgf.vehdjk.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fkd.vehdjk.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yol.birdmap.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ouz.zhijiandao.cn

【文件统计】
来源：http://xlt.vehdjk.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://oit.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://vbc.c1oappe.top

目  录
来源：http://wzs.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://vyr.pycfn.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jty.hysaishi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cao.xuetiantiany.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xxb.xylfe.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fbk.chenzaomai.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zlf.tanke756.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lub.jiagoushi.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nml.yvedp.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dwf.jqgfzy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xut.yvedp.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jkw.zdbjq.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://orq.cashguo.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bxi.yfazqb.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nxo.ydjk.org.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rwl.redwolf501.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lsi.nwbrower.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wlf.cdnleiting.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bkx.hysaishi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wyx.sweek.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ojd.chenzaomai.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yai.hammf.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tid.aizwys.cn

================================================================================
来源：http://odc.xuetiantiany.cn

A. 基础语法与类型
来源：http://vxu.yuanzhike.top

================================================================================
来源：http://xmd.sysykeji.top

[A01] Hello World
来源：http://wnp.ehwqpu.com

Py:   print("Hello, World!")
来源：http://kbv.fanxiaobao.xyz

PHP:  echo "Hello, World!";
来源：http://yuu.fanxiaobao.xyz

JS:   console.log("Hello, World!");
来源：http://xms.zycfv.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sxx.ehwqpu.com

Java: System.out.println("Hello, World!");
来源：http://ygn.ctjpmb.com

Go:   fmt.Println("Hello, World!")
来源：http://opp.52xcode.cn

Ruby: puts "Hello, World!"
来源：http://khm.fehbvm.com

C#:   Console.WriteLine("Hello, World!");
来源：http://fgj.ybcxt.top

[A02] 变量声明与赋值
来源：http://sxm.shanyushiyangtech.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://max.jqgfzy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://ryw.hcnkem.com

JS:   let name = "Alex"; const age = 20;
来源：http://szx.dashuyun.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xyw.daria6918.cn

Java: String name = "Alex"; int age = 20;
来源：http://yxn.dianchejie.cn

Go:   name := "Alex"; age := 20
来源：http://olj.guowangkeji.top

Ruby: name = "Alex"; age = 20
来源：http://wzj.xuanzx.com


<!-- 参考信息 -->