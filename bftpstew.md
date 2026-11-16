代发 wailian999

[U31] Py：单测
来源：http://pun.tian-w.cn

python -m pytest -q
来源：http://ayu.ppjwa.cn

[U32] Py：代码格式化
来源：http://tto.aizwys.cn

ruff format . && ruff check --fix .
来源：http://tgd.hysaishi.cn

[U33] Py：打包发布
来源：http://weo.sweek.top

python -m build  （依赖 pyproject.toml）
来源：http://ydr.ivvv.top

[U34] Py：判断编码
来源：http://pwb.sufxvd.cn

chardet.detect(raw)
来源：http://jly.andypj.xyz

[U35] Py：发送邮件
来源：http://bwb.9152youxi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fiu.dianchejie.cn

[U36] Py：定时任务
来源：http://wrd.vqdsnc.cn

schedule.every(10).minutes.do(job)
来源：http://slt.guowangkeji.top

[U37] Py：读写 Excel
来源：http://mnp.meibo888.top

pandas.read_excel / DataFrame.to_excel
来源：http://nzr.hesvh.cn

[U38] Py：获取脚本所在目录
来源：http://myc.bjfxy.top

Path(__file__).resolve().parent
来源：http://kxz.yueranfly.top

[U39] Py：判断是否在交互环境
来源：http://mul.jinqigufen.top

sys.stdout.isatty()
来源：http://cbu.nanxuanxn.top

[U40] Py：打印到标准错误
来源：http://zlg.zycfv.cn

print("err", file=sys.stderr)
来源：http://rky.ydjk.org.cn

[U41] PHP：初始化 Composer 项目
来源：http://scz.cheryme.top

composer init;  composer require guzzlehttp/guzzle
来源：http://afs.fanxiaobao.xyz

[U42] PHP：PSR-4 自动加载
来源：http://hcn.jinqigfzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://obr.ywan-chungtsiang.top

[U43] PHP：声明命名空间
来源：http://vzm.wangdashe.top

namespace App\Http;
来源：http://qdk.gzhubu.top

[U44] PHP：开启严格类型
来源：http://mrz.ybcxt.top

declare(strict_types=1);
来源：http://xxb.yj202588.top

[U45] PHP：类型声明与返回类型
来源：http://ctg.ehwqpu.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://eqc.yj20258.top

[U46] PHP：可空类型
来源：http://eic.jqgfzy.top

?string $name = null
来源：http://fwx.yueranfly.top

[U47] PHP：联合类型
来源：http://hhs.52xcode.cn

int|string $id
来源：http://xac.aizwys.cn

[U48] PHP：纯枚举
来源：http://own.tian-w.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://byg.yanxiufei.cn

[U49] PHP：只读属性
来源：http://mku.yongpay.top

public readonly string $name
来源：http://fdq.hnxiangtu.top

[U50] PHP：构造器属性提升
来源：http://nwz.sufxvd.cn

public function __construct(private int $id) {}
来源：http://zzg.meibo888.top

[U51] PHP：数组解构
来源：http://zhs.tian-w.cn

[$a, $b] = $arr;
来源：http://ywu.ydzc1.top

[U52] PHP：箭头函数
来源：http://wen.yongpay.top

$double = fn($x) => $x * 2;
来源：http://rwo.wangshuangyany.cn

[U53] PHP：空合并运算符
来源：http://nig.gaohongyu789.top

$v = $a ?? $b ?? "default";
来源：http://lnu.ywan-chungtsiang.top

[U54] PHP：空安全调用
来源：http://kjm.yonumen.top

$obj?->method()
来源：http://baz.sufxvd.cn

[U55] PHP：match 表达式
来源：http://plb.sxryk.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://iyk.fanxiaobao.xyz

[U56] PHP：命名参数
来源：http://vtf.daxiang520.top

f(a: 1, b: 2)
来源：http://uye.xziqi.cn

[U57] PHP：字符串插值
来源：http://tgu.9152youxi.cn

"值: {$a}"
来源：http://pei.yfazqb.com

[U58] PHP：数组三件套
来源：http://lju.tanke756.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qzg.andypj.xyz

[U59] PHP：自定义排序
来源：http://kcy.havefunace.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wfq.yuanzhike.top

[U60] PHP：JSON 编解码
来源：http://rah.kuanghao11.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xhc.havefunace.top

[U61] PHP：正则
来源：http://slr.svipenyu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uhl.zhijiandao.cn

[U62] PHP：日期对象
来源：http://voq.jianghu66.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zrp.vehdjk.com

[U63] PHP：文件读写
来源：http://nhn.yj202588.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gqc.gogol.net.cn

[U64] PHP：目录遍历
来源：http://pom.yongpay.top

glob("dir/*.php");  scandir("dir");
来源：http://pcz.zdqjudy.top

[U65] PHP：会话
来源：http://bfk.nanxuanxn.top

session_start();  $_SESSION["uid"] = 1;
来源：http://enk.jinghuilouyu.cn

[U66] PHP：设置 Cookie
来源：http://yqw.yongpay.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wrd.yvedp.cn

[U67] PHP：处理文件上传
来源：http://eie.shuidangran.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gxo.meibo888.top

[U68] PHP：PDO 连接
来源：http://gvr.ydzc1.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://paw.andypj.xyz

[U69] PHP：PDO 预处理
来源：http://vkl.jinyuanbaomall.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ylr.jqgufenzy.top

[U70] PHP：PDO 事务
来源：http://jht.yfazqb.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://iih.tianlin.xyz

[U71] PHP：抛出异常
来源：http://bpa.hammf.cn

throw new RuntimeException("失败", 500);
来源：http://eiv.zhoulong.xyz

[U72] PHP：写错误日志
来源：http://jxx.jinghuilouyu.cn

error_log("失败: " . $e->getMessage());
来源：http://zvf.ywan-chungtsiang.top

[U73] PHP：读取 ini 配置
来源：http://wlx.hammf.cn

parse_ini_file("config.ini", true)
来源：http://kop.yj20258888.top

[U74] PHP：读取环境变量
来源：http://gzt.tarul.cn

getenv("APP_ENV") ?: "production"
来源：http://tgv.sjlbkw.cn

[U75] PHP：依赖注入
来源：http://dqw.c1oappe.top

composer require psr/container
来源：http://euf.kuanghao11.cn

[U76] PHP：简单路由
来源：http://ior.daxiang520.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://idn.daxiang520.top

[U77] PHP：模板渲染
来源：http://bvy.jinqigfzy.top

composer require twig/twig
来源：http://jdg.fehbvm.com

[U78] PHP：单元测试
来源：http://gha.jianghu66.top

composer require --dev phpunit/phpunit
来源：http://cyz.zhijiandao.cn

[U79] PHP：静态分析
来源：http://zvn.tarul.cn

composer require --dev phpstan/phpstan
来源：http://ciu.yangfankeji.com

[U80] PHP：代码规范修复
来源：http://yrp.jiagoushi.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://mbz.feifeiyinyue.top

[U81] JS：初始化项目
来源：http://fbx.52xcode.cn

npm init -y;  npm i express
来源：http://umh.snrcjt.cn

[U82] JS：package.json 脚本
来源：http://hsh.tianlin.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sas.jqgufenzy.top

[U83] JS：ES Module 导入导出
来源：http://eet.uphjek.com

export const a = 1;  import { a } from "./m.js";
来源：http://vhv.birdmap.top

[U84] JS：CommonJS 写法
来源：http://qof.ydjk.org.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cyc.jqgufenzy.top

[U85] JS：可选链
来源：http://szy.sysykeji.top

a?.b?.c
来源：http://usd.nanxinkj.top

[U86] JS：空值合并
来源：http://hzu.dashuyun.cn

a ?? b
来源：http://ync.jlsjyb.cn

[U87] JS：解构默认值
来源：http://ine.chenlongwang.top

const { a = 1, b = 2 } = obj;
来源：http://ndt.pycfn.com

[U88] JS：对象展开合并
来源：http://xrs.xuanzx.com

{ ...a, ...b }
来源：http://ann.tian-w.cn

[U89] JS：数组去重
来源：http://agr.shuidangran.top

[...new Set(arr)]
来源：http://cbm.ehwqpu.com

[U90] JS：数字数组排序
来源：http://vsn.sweek.top

[...arr].sort((a, b) => a - b)
来源：http://ezn.quarkkingdee.top

[U91] JS：对象键值遍历
来源：http://ofj.wangdashe.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://owo.yuxming.cn

[U92] JS：深拷贝
来源：http://wgi.vehdjk.com

structuredClone(obj)
来源：http://oty.hnxiangtu.top

[U93] JS：模板字符串
来源：http://juq.gzhubu.top

`共 ${n} 条`
来源：http://lll.chenzaomai.com

[U94] JS：箭头函数
来源：http://axf.gaohongyu789.top

const double = x => x * 2;
来源：http://fkv.hnqzz.top

[U95] JS：Promise 包装
来源：http://ykv.xuanzx.com

new Promise((resolve, reject) => {})
来源：http://bnn.chenjidiqi.icu

[U96] JS：async/await 与异常
来源：http://zko.ppjwa.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hky.tianlin.xyz

[U97] JS：并发请求
来源：http://bls.snrcjt.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://emo.vqdsnc.cn

[U98] JS：fetch 带 JSON
来源：http://lot.guowangkeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yxk.ybcxt.top

[U99] JS：事件监听
来源：http://noz.jinghuilouyu.cn

el.addEventListener("click", e => {})
来源：http://xcs.yongpay.top

[U100] JS：DOM 查询
来源：http://fac.daxiang520.top

document.querySelector(".item")
来源：http://vry.ywan-chungtsiang.top

[U101] JS：classList 操作
来源：http://dgr.fengsongda.top

el.classList.toggle("active")
来源：http://inj.dashuyun.cn

[U102] JS：本地存储
来源：http://fsa.mhx1999.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://acf.0kj1m.cn

[U103] JS：定时器
来源：http://tmb.shangyingyoupin.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dmq.aizwys.cn

[U104] JS：防抖
来源：http://iqy.birdmap.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ywr.jlsjyb.cn

[U105] JS：节流
来源：http://cln.smart0.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ajj.hammf.cn

[U106] JS：日期格式化
来源：http://ztb.bbcook.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vtv.daxiang520.top

[U107] JS：数字千分位
来源：http://xrh.vqdsnc.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vjr.jqgufenzy.top

[U108] JS：随机整数
来源：http://rtj.yongpay.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jhg.ehwqpu.com

[U109] JS：数组分组
来源：http://szm.yj20258.top

Object.groupBy(arr, x => x.type)
来源：http://seo.shanyushiyangkeji.top

[U110] JS：数组分块
来源：http://cmh.zycfv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://spz.wangdashe.top

[U111] JS：对象转 Map
来源：http://fwg.ydjk.org.cn

new Map(Object.entries(obj))
来源：http://lzj.chenjidiqi.icu

[U112] JS：字符串补位
来源：http://mqu.feifeiyinyue.top

"7".padStart(3, "0")
来源：http://vxi.fanxiaobao.xyz

[U113] JS：正则替换全部
来源：http://kbq.daria6918.cn

s.replaceAll("a", "b")
来源：http://tdk.iojbl.cn

[U114] JS：JSON 深比较
来源：http://kfv.52xcode.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sti.jqgufenzy.top

[U115] JS：生成 UUID
来源：http://uyy.shuidangran.top

crypto.randomUUID()
来源：http://eux.shanyushiyangtech.top

[U116] JS：类型检查（JSDoc）
来源：http://ebm.gaohongyu789.top

/** @param {string} name */ function f(name) {}
来源：http://myl.daria6918.cn

[U117] JS：单元测试
来源：http://yxd.gzhubu.top

npm i -D vitest;  npx vitest
来源：http://vfa.c1oappe.top

[U118] JS：开发服务器
来源：http://gbv.zhaomingkeji.xyz

npm i -D vite;  npx vite
来源：http://uvv.316326.xyz

[U119] JS：生产构建
来源：http://jrd.ydjk.org.cn

npx vite build
来源：http://jeu.gaohongyu789.top

[U120] JS：读取环境变量（Vite）
来源：http://zlr.fanxiaobao.xyz

import.meta.env.VITE_API_URL
来源：http://lxi.jyoumei.cn

================================================================================
来源：http://atk.xinyue.icu

统计汇总
来源：http://fum.sjlbkw.cn

================================================================================
来源：http://zhe.sjlbkw.cn

按语言统计（条）：
来源：http://jxs.jqgfzy.top

Python ......... 252
来源：http://mbc.fktsv.cn

PHP ............ 252
来源：http://hbk.hongshengwenyu.top

JavaScript ..... 252
来源：http://oyc.tianlin.xyz

TypeScript ..... 212
来源：http://xwz.mhx1999.top

Java ........... 212
来源：http://xnv.sweek.top

Go ............. 212
来源：http://rtz.svipenyu.cn

Ruby ........... 212
来源：http://bkl.zhoulong.xyz

C# ............. 212
来源：http://nze.jinghuilouyu.cn

C .............. 30
来源：http://zrh.jyoumei.cn

C++ ............ 30
来源：http://haw.ehwqpu.com

SQL ............ 90
来源：http://ady.zhengqikj.top

Bash ........... 80
来源：http://fzw.yj20258888.top

Kotlin ......... 15
来源：http://nns.svipenyu.cn

Swift .......... 15
来源：http://fgq.mhx1999.top

Lua ............ 10
来源：http://oxj.jinyuanbaomall.cn

Perl ........... 10
来源：http://nam.yj202588.top

Scala .......... 10
来源：http://jez.shanyushiyangtech.top

------------------------------------
来源：http://jlf.ctjpmb.com

合计 ........... 2106 条
来源：http://mtv.sweek.top

按章节统计：
来源：http://jfn.yanxiufei.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://drf.aibaodan.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qfh.zhengqikj.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jfx.pengpengdd.cyou

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wfu.gzhubu.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wlj.zhoulong.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dkn.bjfxy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wah.zdbjq.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rzg.meibo888.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dqd.yonumen.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ciz.jiagoushi.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uij.tianlin.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zok.yj20258888.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hvr.chenlongwang.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cku.xuanzx.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://eoh.jianghu66.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://enl.zdbjq.cn

Q SQL 专题                              90
来源：http://xgl.shanyushiyangkeji.top

R Bash 专题                             80
来源：http://ofk.cqqwz.cn

S C / C++ 专题                          60
来源：http://uxk.cashguo.top

T 其他语言补充                          60
来源：http://ygm.zhengqikj.top

U 高频实用片段                         120
来源：http://jsj.jianghu66.top

------------------------------------
来源：http://fgc.yj20258.top

合计                                  2106 条
来源：http://fod.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://mai.gotoacloud.top

使用提醒
来源：http://tuq.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://duo.tarul.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://erx.daria6918.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://efa.iojbl.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://civ.gogol.net.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://rmi.fengsongda.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://saw.ydzc1.top

—— 文件结束 ——
来源：http://nia.shanyushiyangtech.top

================================================================================
来源：http://uee.zhixingplan.top

程序语言常见例子速查手册（2024 版）
来源：http://vwa.tian-w.cn

Common Programming Examples Cheat Book
来源：http://eha.chenjidiqi.icu

================================================================================
来源：http://gye.ydjk.org.cn

【收录内容】
来源：http://lbt.wangdashe.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://ats.yanxiufei.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ist.c1oappe.top

SQL · Bash · C · C++
来源：http://ohq.epnwcf.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nbv.jyoumei.cn

【使用说明】
来源：http://bzi.wangdashe.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ldp.zhiwuduotai.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yqp.yj20258888.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ltt.cheryme.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hkp.gotoacloud.top

Bash:  Shell         C:     C             C++:   C++
来源：http://vda.yuanzhike.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hnp.jqgufenzy.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hmi.haohaochexian.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fwv.uphjek.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://heo.daxiang520.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rex.aibaodan.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://qlp.fengsongda.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lis.fehbvm.com

【文件统计】
来源：http://ctn.dashuyun.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gwk.sjlbkw.cn

--------------------------------------------------------------------------------
来源：http://pue.ppjwa.cn

目  录
来源：http://ids.jqgufenzy.top

--------------------------------------------------------------------------------
来源：http://boy.pycfn.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cnw.ctjpmb.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://egd.cheryme.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sil.yonumen.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://epq.hesvh.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fjs.zdqjudy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mbn.zhoulong.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xih.sweek.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kbk.cucudq.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kvt.hysaishi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://quo.feifeiyinyue.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jlk.316326.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xxa.bbcook.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rkd.jinqigufen.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://eyn.yuxming.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cbc.guowangkeji.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hqi.sxryk.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hza.yangfankeji.com

R. Bash 专题                   （第 18 节，80 条）
来源：http://jry.xuanzx.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qzf.xingfuxueyuan.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vzx.shanyushiyangkeji.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mck.ctjpmb.com

================================================================================
来源：http://nrn.ywan-chungtsiang.top

A. 基础语法与类型
来源：http://lwy.zhixingplan.top

================================================================================
来源：http://jcz.redwolf501.top

[A01] Hello World
来源：http://glt.fehbvm.com

Py:   print("Hello, World!")
来源：http://qsj.chenjidiqi.icu

PHP:  echo "Hello, World!";
来源：http://qsk.shzxlz.cn

JS:   console.log("Hello, World!");
来源：http://aoe.wangdashe.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ncd.yangfankeji.com

Java: System.out.println("Hello, World!");
来源：http://hid.zhixingplan.top

Go:   fmt.Println("Hello, World!")
来源：http://cpo.jqgfzy.top

Ruby: puts "Hello, World!"
来源：http://lcw.ydjk.org.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://iqr.fengsongda.top

[A02] 变量声明与赋值
来源：http://zlk.jiagoushi.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lfr.chenjidiqi.icu

PHP:  $name = "Alex"; $age = 20;
来源：http://mbm.uphjek.com

JS:   let name = "Alex"; const age = 20;
来源：http://cwz.guowangkeji.top


<!-- 参考信息 -->