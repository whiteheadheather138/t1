代发 wailian999

[U33] Py：打包发布
来源：http://vvs.zhijiandao.cn

python -m build  （依赖 pyproject.toml）
来源：http://jxe.andypj.xyz

[U34] Py：判断编码
来源：http://rux.gotoacloud.top

chardet.detect(raw)
来源：http://jdp.yfazqb.com

[U35] Py：发送邮件
来源：http://wju.dianchejie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ksd.cashguo.top

[U36] Py：定时任务
来源：http://icv.guannengcc.top

schedule.every(10).minutes.do(job)
来源：http://atu.zhaomingkeji.xyz

[U37] Py：读写 Excel
来源：http://jik.jqgfzy.top

pandas.read_excel / DataFrame.to_excel
来源：http://tga.guowangkeji.top

[U38] Py：获取脚本所在目录
来源：http://pif.cucudq.cn

Path(__file__).resolve().parent
来源：http://uhk.zdbjq.cn

[U39] Py：判断是否在交互环境
来源：http://mso.feifeiyinyue.top

sys.stdout.isatty()
来源：http://dkw.jianghu66.top

[U40] Py：打印到标准错误
来源：http://osp.c1oappe.top

print("err", file=sys.stderr)
来源：http://zzy.sjlbkw.cn

[U41] PHP：初始化 Composer 项目
来源：http://anh.9152youxi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ttx.aizwys.cn

[U42] PHP：PSR-4 自动加载
来源：http://huh.shuidangran.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ohp.jinyuanbaomall.cn

[U43] PHP：声明命名空间
来源：http://bke.nanxuanxn.top

namespace App\Http;
来源：http://nzl.hfpthk.cn

[U44] PHP：开启严格类型
来源：http://diu.fzhhl.top

declare(strict_types=1);
来源：http://udd.sysykeji.top

[U45] PHP：类型声明与返回类型
来源：http://shy.smart0.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://utq.52xcode.cn

[U46] PHP：可空类型
来源：http://suv.snrcjt.cn

?string $name = null
来源：http://lff.jinqigufen.top

[U47] PHP：联合类型
来源：http://skv.jinqigufen.top

int|string $id
来源：http://afi.zhaomingkeji.xyz

[U48] PHP：纯枚举
来源：http://xpc.sxryk.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cwu.hnxiangtu.top

[U49] PHP：只读属性
来源：http://clr.shanyushiyangkeji.top

public readonly string $name
来源：http://gkf.yanxiufei.cn

[U50] PHP：构造器属性提升
来源：http://qbi.yuanzhike.top

public function __construct(private int $id) {}
来源：http://tyq.feifeiyinyue.top

[U51] PHP：数组解构
来源：http://lba.zdbjq.cn

[$a, $b] = $arr;
来源：http://yvi.bbcook.cn

[U52] PHP：箭头函数
来源：http://qpf.sysykeji.top

$double = fn($x) => $x * 2;
来源：http://qbs.redwolf501.top

[U53] PHP：空合并运算符
来源：http://yta.andypj.xyz

$v = $a ?? $b ?? "default";
来源：http://suf.yangfankeji.com

[U54] PHP：空安全调用
来源：http://buv.guannengcc.top

$obj?->method()
来源：http://iwa.meibo888.top

[U55] PHP：match 表达式
来源：http://gxo.ydjk.org.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vpz.snrcjt.cn

[U56] PHP：命名参数
来源：http://qwv.vqdsnc.cn

f(a: 1, b: 2)
来源：http://eld.ppjwa.cn

[U57] PHP：字符串插值
来源：http://nkq.aibaodan.cn

"值: {$a}"
来源：http://gyt.pycfn.com

[U58] PHP：数组三件套
来源：http://vbs.meibo888.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pwy.guannengcc.top

[U59] PHP：自定义排序
来源：http://qzv.sxryk.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fsq.snrcjt.cn

[U60] PHP：JSON 编解码
来源：http://viq.yanxiufei.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jag.zhixingplan.top

[U61] PHP：正则
来源：http://qrb.jinghuilouyu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wsn.ydzc1.top

[U62] PHP：日期对象
来源：http://net.iojbl.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ydb.gzhubu.top

[U63] PHP：文件读写
来源：http://rit.316326.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tlf.nanxuanxn.top

[U64] PHP：目录遍历
来源：http://aqf.xuetiantiany.cn

glob("dir/*.php");  scandir("dir");
来源：http://prm.yongpay.top

[U65] PHP：会话
来源：http://hxd.nanxuanxn.top

session_start();  $_SESSION["uid"] = 1;
来源：http://kvv.zhongyouzk.top

[U66] PHP：设置 Cookie
来源：http://lap.jyoumei.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://axn.haohaochexian.top

[U67] PHP：处理文件上传
来源：http://mtc.quarkkingdee.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yls.redwolf501.top

[U68] PHP：PDO 连接
来源：http://izk.kuanghao11.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jnh.shanyushiyangkeji.top

[U69] PHP：PDO 预处理
来源：http://xdr.jyoumei.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://znx.zhengqikj.top

[U70] PHP：PDO 事务
来源：http://xjt.zhixingplan.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fwl.ppjwa.cn

[U71] PHP：抛出异常
来源：http://dai.shangyingyoupin.top

throw new RuntimeException("失败", 500);
来源：http://hkc.c1oappe.top

[U72] PHP：写错误日志
来源：http://xtb.hysaishi.cn

error_log("失败: " . $e->getMessage());
来源：http://xll.wangdashe.top

[U73] PHP：读取 ini 配置
来源：http://hxi.cdnleiting.top

parse_ini_file("config.ini", true)
来源：http://kgo.ydjk.org.cn

[U74] PHP：读取环境变量
来源：http://fxd.tanke756.top

getenv("APP_ENV") ?: "production"
来源：http://szd.dashuyun.cn

[U75] PHP：依赖注入
来源：http://twe.tarul.cn

composer require psr/container
来源：http://xdn.gaohongyu789.top

[U76] PHP：简单路由
来源：http://pek.ctjpmb.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://toy.dashuyun.cn

[U77] PHP：模板渲染
来源：http://dlq.hfpthk.cn

composer require twig/twig
来源：http://rbm.sweek.top

[U78] PHP：单元测试
来源：http://rmr.mhx1999.top

composer require --dev phpunit/phpunit
来源：http://yov.yanxiufei.cn

[U79] PHP：静态分析
来源：http://rau.pengpengdd.cyou

composer require --dev phpstan/phpstan
来源：http://tcj.zhongyouzk.top

[U80] PHP：代码规范修复
来源：http://wls.yj20258888.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://yxo.cqqwz.cn

[U81] JS：初始化项目
来源：http://rjs.hnxiangtu.top

npm init -y;  npm i express
来源：http://uct.jinyuanbaomall.cn

[U82] JS：package.json 脚本
来源：http://xkg.ehwqpu.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qyo.ehwqpu.com

[U83] JS：ES Module 导入导出
来源：http://wos.zhiwuduotai.top

export const a = 1;  import { a } from "./m.js";
来源：http://ivn.shuidangran.top

[U84] JS：CommonJS 写法
来源：http://wue.hesvh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ixj.daxiang520.top

[U85] JS：可选链
来源：http://tup.9152youxi.cn

a?.b?.c
来源：http://pij.ctjpmb.com

[U86] JS：空值合并
来源：http://bih.yj202588.top

a ?? b
来源：http://bvd.fehbvm.com

[U87] JS：解构默认值
来源：http://vzp.zhixingplan.top

const { a = 1, b = 2 } = obj;
来源：http://syb.birdmap.top

[U88] JS：对象展开合并
来源：http://nto.zdqjudy.top

{ ...a, ...b }
来源：http://ibr.zhoulong.xyz

[U89] JS：数组去重
来源：http://ikp.sjlbkw.cn

[...new Set(arr)]
来源：http://ygd.cashguo.top

[U90] JS：数字数组排序
来源：http://jqe.dianchejie.cn

[...arr].sort((a, b) => a - b)
来源：http://pav.tian-w.cn

[U91] JS：对象键值遍历
来源：http://smt.xuetiantiany.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ubz.zdqjudy.top

[U92] JS：深拷贝
来源：http://krg.sxryk.cn

structuredClone(obj)
来源：http://dmi.wangshuangyany.cn

[U93] JS：模板字符串
来源：http://bgh.zhengqikj.top

`共 ${n} 条`
来源：http://fqv.kuanghao11.cn

[U94] JS：箭头函数
来源：http://ipj.uphjek.com

const double = x => x * 2;
来源：http://rko.meibo888.top

[U95] JS：Promise 包装
来源：http://apj.chenzaomai.com

new Promise((resolve, reject) => {})
来源：http://erx.ctjpmb.com

[U96] JS：async/await 与异常
来源：http://txg.shanyushiyangtech.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yrd.cucudq.cn

[U97] JS：并发请求
来源：http://xqg.fengsongda.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://aqg.fanxiaobao.xyz

[U98] JS：fetch 带 JSON
来源：http://dix.ybcxt.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://xgm.birdmap.top

[U99] JS：事件监听
来源：http://kom.ehwqpu.com

el.addEventListener("click", e => {})
来源：http://ekd.shangyingyoupin.top

[U100] JS：DOM 查询
来源：http://mlc.vehdjk.com

document.querySelector(".item")
来源：http://rjp.hnqzz.top

[U101] JS：classList 操作
来源：http://vjs.yj20258888.top

el.classList.toggle("active")
来源：http://xce.hesvh.cn

[U102] JS：本地存储
来源：http://tzd.kuanghao11.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zlm.jinqigufen.top

[U103] JS：定时器
来源：http://gkl.shanyushiyangkeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://twi.aizwys.cn

[U104] JS：防抖
来源：http://fok.ctjpmb.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jhk.fzhhl.top

[U105] JS：节流
来源：http://xzj.nanxinkj.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jso.pycfn.com

[U106] JS：日期格式化
来源：http://bpf.cqqwz.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://int.yj202588.top

[U107] JS：数字千分位
来源：http://irf.jqgufenzy.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cdn.xuanzx.com

[U108] JS：随机整数
来源：http://knn.meibo888.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pol.cashguo.top

[U109] JS：数组分组
来源：http://jrq.svipenyu.cn

Object.groupBy(arr, x => x.type)
来源：http://hoc.pengpengdd.cyou

[U110] JS：数组分块
来源：http://mud.gzhubu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bvx.yuxming.cn

[U111] JS：对象转 Map
来源：http://kbq.nwbrower.top

new Map(Object.entries(obj))
来源：http://bui.jlsjyb.cn

[U112] JS：字符串补位
来源：http://tmh.zdbjq.cn

"7".padStart(3, "0")
来源：http://fqu.ydzc1.top

[U113] JS：正则替换全部
来源：http://kkm.haohaochexian.top

s.replaceAll("a", "b")
来源：http://yjz.gotoacloud.top

[U114] JS：JSON 深比较
来源：http://qil.gogol.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xlx.zdqjudy.top

[U115] JS：生成 UUID
来源：http://pgo.fehbvm.com

crypto.randomUUID()
来源：http://vbl.9152youxi.cn

[U116] JS：类型检查（JSDoc）
来源：http://lkj.xziqi.cn

/** @param {string} name */ function f(name) {}
来源：http://yzd.hfpthk.cn

[U117] JS：单元测试
来源：http://pjh.quarkkingdee.top

npm i -D vitest;  npx vitest
来源：http://mgb.mhx1999.top

[U118] JS：开发服务器
来源：http://fvc.mhx1999.top

npm i -D vite;  npx vite
来源：http://hob.jianghu66.top

[U119] JS：生产构建
来源：http://okl.meibo888.top

npx vite build
来源：http://vox.zhongyouzk.top

[U120] JS：读取环境变量（Vite）
来源：http://rjg.yj202588.top

import.meta.env.VITE_API_URL
来源：http://beh.yongpay.top

================================================================================
来源：http://dne.havefunace.top

统计汇总
来源：http://vdq.ybcxt.top

================================================================================
来源：http://eeb.hnqzz.top

按语言统计（条）：
来源：http://aln.zhengqikj.top

Python ......... 252
来源：http://pwa.feifeiyinyue.top

PHP ............ 252
来源：http://jkz.yuanzhike.top

JavaScript ..... 252
来源：http://nog.sufxvd.cn

TypeScript ..... 212
来源：http://eqz.haohaochexian.top

Java ........... 212
来源：http://asa.nanxuanxn.top

Go ............. 212
来源：http://ghb.ywan-chungtsiang.top

Ruby ........... 212
来源：http://udd.yvedp.cn

C# ............. 212
来源：http://ukm.hesvh.cn

C .............. 30
来源：http://qhi.iojbl.cn

C++ ............ 30
来源：http://kiu.chenlongwang.top

SQL ............ 90
来源：http://iix.xylfe.cn

Bash ........... 80
来源：http://dnw.ydzc1.top

Kotlin ......... 15
来源：http://bkk.shzxlz.cn

Swift .......... 15
来源：http://aak.pycfn.com

Lua ............ 10
来源：http://xjc.yfazqb.com

Perl ........... 10
来源：http://szx.wangdashe.top

Scala .......... 10
来源：http://mzc.52xcode.cn

------------------------------------
来源：http://mhf.bjfxy.top

合计 ........... 2106 条
来源：http://ebp.nanxinkj.top

按章节统计：
来源：http://wtx.sweek.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lej.dianchejie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yxr.xinyue.icu

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jlc.vehdjk.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://euw.havefunace.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rsm.redwolf501.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xqd.gzhubu.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zrp.gogol.net.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lhw.iojbl.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xeu.mhx1999.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cyj.shanyushiyangkeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://asp.zhixingplan.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jmq.ehwqpu.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hrc.zhoulong.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mgh.chenjidiqi.icu

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://aui.zhiwuduotai.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wzd.zdbjq.cn

Q SQL 专题                              90
来源：http://mwd.gotoacloud.top

R Bash 专题                             80
来源：http://xij.svipenyu.cn

S C / C++ 专题                          60
来源：http://vet.zhixingplan.top

T 其他语言补充                          60
来源：http://hgs.xingfuxueyuan.xyz

U 高频实用片段                         120
来源：http://mbg.sysykeji.top

------------------------------------
来源：http://hre.dianchejie.cn

合计                                  2106 条
来源：http://eza.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://yxx.bbcook.cn

使用提醒
来源：http://wud.fehbvm.com

--------------------------------------------------------------------------------
来源：http://apf.sjlbkw.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jao.dashuyun.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ngh.birdmap.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://bdt.ppjwa.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://woy.wangshuangyany.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nla.xuetiantiany.cn

—— 文件结束 ——
来源：http://ecs.yanxiufei.cn

================================================================================
来源：http://fln.iojbl.cn

程序语言常见例子速查手册（2024 版）
来源：http://erp.chenzaomai.com

Common Programming Examples Cheat Book
来源：http://phl.tanke756.top

================================================================================
来源：http://qof.yongpay.top

【收录内容】
来源：http://sza.xuanzx.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://gjf.nanxuanxn.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ecd.shuidangran.top

SQL · Bash · C · C++
来源：http://pxs.shangyingyoupin.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fql.316326.xyz

【使用说明】
来源：http://wja.andypj.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hdd.pycfn.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pjm.zhijiandao.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://iad.cashguo.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qyc.cucudq.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ynh.jiagoushi.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://acb.zhiwuduotai.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ebf.daxiang520.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gww.ydzc1.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://sje.jyoumei.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ldy.nanxuanxn.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://feu.hnxiangtu.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ues.ywan-chungtsiang.top

【文件统计】
来源：http://mso.aizwys.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ioj.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://cnc.fktsv.cn

目  录
来源：http://adq.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://htk.yuanzhike.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tma.jiagoushi.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sjm.bbcook.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wur.ppjwa.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bqe.gogol.net.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wee.hnxiangtu.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wpb.tanke756.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://isb.hcnkem.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jbf.fengsongda.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lwv.hnqzz.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ikp.zhixingplan.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://egb.aizwys.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wje.gogol.net.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://iax.ivvv.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vwr.chenzaomai.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pkt.xinyue.icu

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xzg.tarul.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sur.mhx1999.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://bbg.yangfankeji.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fgb.vehdjk.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://aic.jianghu66.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rjp.chenjidiqi.icu

================================================================================
来源：http://jvw.yanxiufei.cn

A. 基础语法与类型
来源：http://byj.zhengqikj.top

================================================================================
来源：http://moo.guannengcc.top

[A01] Hello World
来源：http://moz.snrcjt.cn

Py:   print("Hello, World!")
来源：http://gjf.shzxlz.cn

PHP:  echo "Hello, World!";
来源：http://tpc.jqgufenzy.top

JS:   console.log("Hello, World!");
来源：http://baj.daxiang520.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gjv.shuidangran.top

Java: System.out.println("Hello, World!");
来源：http://prb.aizwys.cn

Go:   fmt.Println("Hello, World!")
来源：http://seb.guannengcc.top

Ruby: puts "Hello, World!"
来源：http://ssk.gogol.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hju.52xcode.cn

[A02] 变量声明与赋值
来源：http://hhg.guowangkeji.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vdm.redwolf501.top

PHP:  $name = "Alex"; $age = 20;
来源：http://gul.chenzaomai.com

JS:   let name = "Alex"; const age = 20;
来源：http://lup.hnxiangtu.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://erm.gaohongyu789.top

Java: String name = "Alex"; int age = 20;
来源：http://ckr.cashguo.top

Go:   name := "Alex"; age := 20
来源：http://kgv.kuanghao11.cn

Ruby: name = "Alex"; age = 20
来源：http://coo.hongshengwenyu.top


<!-- 参考信息 -->