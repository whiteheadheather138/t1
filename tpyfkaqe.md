代发 wailian999

[U33] Py：打包发布
来源：http://llw.andypj.xyz

python -m build  （依赖 pyproject.toml）
来源：http://trc.hnxiangtu.top

[U34] Py：判断编码
来源：http://nrx.wangshuangyany.cn

chardet.detect(raw)
来源：http://rsw.shangyingyoupin.top

[U35] Py：发送邮件
来源：http://pmb.ehwqpu.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://hpe.mhx1999.top

[U36] Py：定时任务
来源：http://fis.svipenyu.cn

schedule.every(10).minutes.do(job)
来源：http://qgz.meibo888.top

[U37] Py：读写 Excel
来源：http://imu.nanxinkj.top

pandas.read_excel / DataFrame.to_excel
来源：http://gce.daria6918.cn

[U38] Py：获取脚本所在目录
来源：http://uld.andypj.xyz

Path(__file__).resolve().parent
来源：http://dcf.chenjidiqi.icu

[U39] Py：判断是否在交互环境
来源：http://par.316326.xyz

sys.stdout.isatty()
来源：http://xvu.cdnleiting.top

[U40] Py：打印到标准错误
来源：http://gzq.sysykeji.top

print("err", file=sys.stderr)
来源：http://lrt.yuanzhike.top

[U41] PHP：初始化 Composer 项目
来源：http://msw.ybcxt.top

composer init;  composer require guzzlehttp/guzzle
来源：http://qlm.epnwcf.com

[U42] PHP：PSR-4 自动加载
来源：http://vqu.jinqigufen.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nqs.haohaochexian.top

[U43] PHP：声明命名空间
来源：http://xvp.tian-w.cn

namespace App\Http;
来源：http://npc.haohaochexian.top

[U44] PHP：开启严格类型
来源：http://uyd.dianchejie.cn

declare(strict_types=1);
来源：http://ibp.svipenyu.cn

[U45] PHP：类型声明与返回类型
来源：http://oqo.sxryk.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://arl.gogol.net.cn

[U46] PHP：可空类型
来源：http://vme.jinqigfzy.top

?string $name = null
来源：http://kjl.redwolf501.top

[U47] PHP：联合类型
来源：http://gwg.fehbvm.com

int|string $id
来源：http://ntj.yongpay.top

[U48] PHP：纯枚举
来源：http://cxu.tianlin.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sdy.shanyushiyangtech.top

[U49] PHP：只读属性
来源：http://szq.hcnkem.com

public readonly string $name
来源：http://vfp.birdmap.top

[U50] PHP：构造器属性提升
来源：http://eqy.0kj1m.cn

public function __construct(private int $id) {}
来源：http://wqm.dianchejie.cn

[U51] PHP：数组解构
来源：http://dhl.epnwcf.com

[$a, $b] = $arr;
来源：http://brt.jinghuilouyu.cn

[U52] PHP：箭头函数
来源：http://idi.gotoacloud.top

$double = fn($x) => $x * 2;
来源：http://efu.zhongyouzk.top

[U53] PHP：空合并运算符
来源：http://fsn.pycfn.com

$v = $a ?? $b ?? "default";
来源：http://zlt.yuxming.cn

[U54] PHP：空安全调用
来源：http://ftu.tian-w.cn

$obj?->method()
来源：http://ghd.yanxiufei.cn

[U55] PHP：match 表达式
来源：http://sfg.ivvv.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fyw.dashuyun.cn

[U56] PHP：命名参数
来源：http://lvc.zhijiandao.cn

f(a: 1, b: 2)
来源：http://dbm.c1oappe.top

[U57] PHP：字符串插值
来源：http://zuz.jinqigfzy.top

"值: {$a}"
来源：http://law.birdmap.top

[U58] PHP：数组三件套
来源：http://tsv.hcnkem.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ktm.jyoumei.cn

[U59] PHP：自定义排序
来源：http://sux.gaohongyu789.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jza.hnqzz.top

[U60] PHP：JSON 编解码
来源：http://jwh.pengpengdd.cyou

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yun.wangdashe.top

[U61] PHP：正则
来源：http://ztu.tianlin.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ksg.andypj.xyz

[U62] PHP：日期对象
来源：http://oml.gogol.net.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xhm.zhengqikj.top

[U63] PHP：文件读写
来源：http://adm.nwbrower.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://oqt.cashguo.top

[U64] PHP：目录遍历
来源：http://jtl.yvedp.cn

glob("dir/*.php");  scandir("dir");
来源：http://ppp.jinghuilouyu.cn

[U65] PHP：会话
来源：http://zlp.yuanzhike.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ajs.zhoulong.xyz

[U66] PHP：设置 Cookie
来源：http://rjg.fzhhl.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://apj.mhx1999.top

[U67] PHP：处理文件上传
来源：http://fey.sysykeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gzy.cashguo.top

[U68] PHP：PDO 连接
来源：http://cpe.yj20258888.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fzf.tianlin.xyz

[U69] PHP：PDO 预处理
来源：http://wxr.jinghuilouyu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hkc.hcnkem.com

[U70] PHP：PDO 事务
来源：http://tqd.snrcjt.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mwg.zhoulong.xyz

[U71] PHP：抛出异常
来源：http://mkp.yvedp.cn

throw new RuntimeException("失败", 500);
来源：http://unx.shangyingyoupin.top

[U72] PHP：写错误日志
来源：http://qub.tian-w.cn

error_log("失败: " . $e->getMessage());
来源：http://oft.fehbvm.com

[U73] PHP：读取 ini 配置
来源：http://ytd.guowangkeji.top

parse_ini_file("config.ini", true)
来源：http://pxj.zhijiandao.cn

[U74] PHP：读取环境变量
来源：http://uda.bjfxy.top

getenv("APP_ENV") ?: "production"
来源：http://eoz.yuxming.cn

[U75] PHP：依赖注入
来源：http://env.9152youxi.cn

composer require psr/container
来源：http://spg.0kj1m.cn

[U76] PHP：简单路由
来源：http://yzv.cqqwz.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rpk.meibo888.top

[U77] PHP：模板渲染
来源：http://scy.yuxming.cn

composer require twig/twig
来源：http://bnr.uphjek.com

[U78] PHP：单元测试
来源：http://svh.c1oappe.top

composer require --dev phpunit/phpunit
来源：http://umj.hcnkem.com

[U79] PHP：静态分析
来源：http://rdf.fktsv.cn

composer require --dev phpstan/phpstan
来源：http://qtj.dianchejie.cn

[U80] PHP：代码规范修复
来源：http://oxo.havefunace.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://dhu.tianlin.xyz

[U81] JS：初始化项目
来源：http://whs.svipenyu.cn

npm init -y;  npm i express
来源：http://ibg.mhx1999.top

[U82] JS：package.json 脚本
来源：http://geb.aizwys.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fqu.zhengqikj.top

[U83] JS：ES Module 导入导出
来源：http://anm.chenjidiqi.icu

export const a = 1;  import { a } from "./m.js";
来源：http://gyr.jqgufenzy.top

[U84] JS：CommonJS 写法
来源：http://vuj.shangyingyoupin.top

module.exports = { a };  const { a } = require("./m");
来源：http://rjv.zhengqikj.top

[U85] JS：可选链
来源：http://vly.yangfankeji.com

a?.b?.c
来源：http://dot.xuanzx.com

[U86] JS：空值合并
来源：http://vgp.shanyushiyangkeji.top

a ?? b
来源：http://qbk.yueranfly.top

[U87] JS：解构默认值
来源：http://vjd.zhiwuduotai.top

const { a = 1, b = 2 } = obj;
来源：http://khm.uphjek.com

[U88] JS：对象展开合并
来源：http://vxk.jyoumei.cn

{ ...a, ...b }
来源：http://vja.ctjpmb.com

[U89] JS：数组去重
来源：http://kag.xylfe.cn

[...new Set(arr)]
来源：http://kww.aibaodan.cn

[U90] JS：数字数组排序
来源：http://tuv.dianchejie.cn

[...arr].sort((a, b) => a - b)
来源：http://ewe.sysykeji.top

[U91] JS：对象键值遍历
来源：http://bwi.uphjek.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://iaq.bbcook.cn

[U92] JS：深拷贝
来源：http://cke.hnqzz.top

structuredClone(obj)
来源：http://zbf.xziqi.cn

[U93] JS：模板字符串
来源：http://vcd.nanxinkj.top

`共 ${n} 条`
来源：http://gja.jinqigufen.top

[U94] JS：箭头函数
来源：http://lwz.vqdsnc.cn

const double = x => x * 2;
来源：http://zwe.zhixingplan.top

[U95] JS：Promise 包装
来源：http://bhb.cashguo.top

new Promise((resolve, reject) => {})
来源：http://jgg.0kj1m.cn

[U96] JS：async/await 与异常
来源：http://ruk.smart0.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://shs.xylfe.cn

[U97] JS：并发请求
来源：http://qtu.zhaomingkeji.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://wsv.zhengqikj.top

[U98] JS：fetch 带 JSON
来源：http://wde.zhijiandao.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://efr.zdbjq.cn

[U99] JS：事件监听
来源：http://vew.pycfn.com

el.addEventListener("click", e => {})
来源：http://ftc.feifeiyinyue.top

[U100] JS：DOM 查询
来源：http://svn.shangyingyoupin.top

document.querySelector(".item")
来源：http://sfn.cheryme.top

[U101] JS：classList 操作
来源：http://rmg.cqqwz.cn

el.classList.toggle("active")
来源：http://fmh.cucudq.cn

[U102] JS：本地存储
来源：http://xoh.fanxiaobao.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://tbp.yfazqb.com

[U103] JS：定时器
来源：http://gvv.sufxvd.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qix.xuetiantiany.cn

[U104] JS：防抖
来源：http://wnp.gotoacloud.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hph.nanxuanxn.top

[U105] JS：节流
来源：http://tbz.shuidangran.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://frp.zhaomingkeji.xyz

[U106] JS：日期格式化
来源：http://ulf.cheryme.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mbx.9152youxi.cn

[U107] JS：数字千分位
来源：http://ewn.tarul.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mza.xziqi.cn

[U108] JS：随机整数
来源：http://eju.birdmap.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ewm.jinqigufen.top

[U109] JS：数组分组
来源：http://wzc.ivvv.top

Object.groupBy(arr, x => x.type)
来源：http://vys.yuanzhike.top

[U110] JS：数组分块
来源：http://kef.tanke756.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zty.yj20258888.top

[U111] JS：对象转 Map
来源：http://mpe.xingfuxueyuan.xyz

new Map(Object.entries(obj))
来源：http://cru.gogol.net.cn

[U112] JS：字符串补位
来源：http://gxy.jinqigfzy.top

"7".padStart(3, "0")
来源：http://oqo.hcnkem.com

[U113] JS：正则替换全部
来源：http://oug.hnxiangtu.top

s.replaceAll("a", "b")
来源：http://wgq.shzxlz.cn

[U114] JS：JSON 深比较
来源：http://fxl.ydzc1.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://nsn.ppjwa.cn

[U115] JS：生成 UUID
来源：http://izz.gotoacloud.top

crypto.randomUUID()
来源：http://ktd.bbcook.cn

[U116] JS：类型检查（JSDoc）
来源：http://rmm.shangyingyoupin.top

/** @param {string} name */ function f(name) {}
来源：http://zbl.birdmap.top

[U117] JS：单元测试
来源：http://xje.nanxinkj.top

npm i -D vitest;  npx vitest
来源：http://prm.hnqzz.top

[U118] JS：开发服务器
来源：http://pkz.fanxiaobao.xyz

npm i -D vite;  npx vite
来源：http://vgs.fanxiaobao.xyz

[U119] JS：生产构建
来源：http://osa.jqgfzy.top

npx vite build
来源：http://lgt.zdqjudy.top

[U120] JS：读取环境变量（Vite）
来源：http://oku.vqdsnc.cn

import.meta.env.VITE_API_URL
来源：http://ser.nanxuanxn.top

================================================================================
来源：http://lta.nwbrower.top

统计汇总
来源：http://pso.cdnleiting.top

================================================================================
来源：http://thw.sysykeji.top

按语言统计（条）：
来源：http://bfc.xziqi.cn

Python ......... 252
来源：http://njw.dashuyun.cn

PHP ............ 252
来源：http://fes.chenzaomai.com

JavaScript ..... 252
来源：http://cgl.9152youxi.cn

TypeScript ..... 212
来源：http://aod.cdnleiting.top

Java ........... 212
来源：http://ozn.gogol.net.cn

Go ............. 212
来源：http://xne.andypj.xyz

Ruby ........... 212
来源：http://wnh.hesvh.cn

C# ............. 212
来源：http://ylh.aizwys.cn

C .............. 30
来源：http://wdu.havefunace.top

C++ ............ 30
来源：http://fun.hnqzz.top

SQL ............ 90
来源：http://ker.cheryme.top

Bash ........... 80
来源：http://lqk.jinyuanbaomall.cn

Kotlin ......... 15
来源：http://vqz.fzhhl.top

Swift .......... 15
来源：http://zjs.vqdsnc.cn

Lua ............ 10
来源：http://jva.xuetiantiany.cn

Perl ........... 10
来源：http://sda.sufxvd.cn

Scala .......... 10
来源：http://jxs.gogol.net.cn

------------------------------------
来源：http://atf.sweek.top

合计 ........... 2106 条
来源：http://hwp.tian-w.cn

按章节统计：
来源：http://aql.epnwcf.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bbh.aizwys.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qaq.0kj1m.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vsa.zhixingplan.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fck.chenjidiqi.icu

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nfg.ybcxt.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lpg.iojbl.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://apn.tian-w.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fji.ybcxt.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zty.yongpay.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ptm.fzhhl.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rqb.yanxiufei.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hnd.jinghuilouyu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mko.ctjpmb.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://rat.yj20258888.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://urk.yuxming.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://czk.haohaochexian.top

Q SQL 专题                              90
来源：http://dnb.jyoumei.cn

R Bash 专题                             80
来源：http://dhq.9152youxi.cn

S C / C++ 专题                          60
来源：http://iqp.cucudq.cn

T 其他语言补充                          60
来源：http://azw.hesvh.cn

U 高频实用片段                         120
来源：http://jro.jianghu66.top

------------------------------------
来源：http://cxh.yuxming.cn

合计                                  2106 条
来源：http://wwl.hongshengwenyu.top

--------------------------------------------------------------------------------
来源：http://qmz.yuanzhike.top

使用提醒
来源：http://unb.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://pmo.meibo888.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kof.yj20258.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vpv.yangfankeji.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zxe.gotoacloud.top

在旧版本上使用前请先确认语法支持情况。
来源：http://clq.gaohongyu789.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yej.shzxlz.cn

—— 文件结束 ——
来源：http://kee.pycfn.com

================================================================================
来源：http://ipv.yj202588.top

程序语言常见例子速查手册（2024 版）
来源：http://vkc.ydzc1.top

Common Programming Examples Cheat Book
来源：http://gwt.zhengqikj.top

================================================================================
来源：http://dcg.zhongyouzk.top

【收录内容】
来源：http://lcw.cheryme.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://kqz.bbcook.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vvr.sxryk.cn

SQL · Bash · C · C++
来源：http://bxr.cucudq.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dpa.cucudq.cn

【使用说明】
来源：http://jfo.c1oappe.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lgl.yj202588.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mpw.jinqigufen.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://oal.hywenlv.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vww.tarul.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://bnt.jianghu66.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gos.andypj.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fxw.gaohongyu789.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://frt.cqqwz.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xpk.daxiang520.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://koa.jyoumei.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gfb.zdbjq.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vyr.xinyue.icu

【文件统计】
来源：http://pqf.yvedp.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mpi.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://tov.hfpthk.cn

目  录
来源：http://jhl.zhaomingkeji.xyz

--------------------------------------------------------------------------------
来源：http://ien.quarkkingdee.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qqp.fzhhl.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vdn.jyoumei.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vwf.ctjpmb.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fgn.ivvv.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mcd.guowangkeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rxt.vehdjk.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tub.cheryme.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://acv.yvedp.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ggk.pycfn.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yix.jinghuilouyu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rec.gogol.net.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://afx.shanyushiyangtech.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kgt.kuanghao11.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://khm.cheryme.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dxr.yvedp.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mri.zdqjudy.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cxo.wangdashe.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://fag.snrcjt.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uqz.bjfxy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gpc.meibo888.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rxg.sysykeji.top

================================================================================
来源：http://ddg.guannengcc.top

A. 基础语法与类型
来源：http://czz.nwbrower.top

================================================================================
来源：http://nwf.tanke756.top

[A01] Hello World
来源：http://zxe.jinqigufen.top

Py:   print("Hello, World!")
来源：http://fuu.iojbl.cn

PHP:  echo "Hello, World!";
来源：http://hmz.hfpthk.cn

JS:   console.log("Hello, World!");
来源：http://tri.yueranfly.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hqz.chenjidiqi.icu

Java: System.out.println("Hello, World!");
来源：http://ptc.ydzc1.top

Go:   fmt.Println("Hello, World!")
来源：http://rxg.tian-w.cn

Ruby: puts "Hello, World!"
来源：http://kop.9152youxi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://eaw.52xcode.cn

[A02] 变量声明与赋值
来源：http://jhd.jiagoushi.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rcf.yueranfly.top

PHP:  $name = "Alex"; $age = 20;
来源：http://kaz.fengsongda.top

JS:   let name = "Alex"; const age = 20;
来源：http://zsz.cheryme.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://lxq.tarul.cn

Java: String name = "Alex"; int age = 20;
来源：http://elt.xylfe.cn

Go:   name := "Alex"; age := 20
来源：http://uuf.bbcook.cn

Ruby: name = "Alex"; age = 20
来源：http://emw.hnxiangtu.top


<!-- 参考信息 -->