代发 wailian999

[U31] Py：单测
来源：http://czh.cheryme.top

python -m pytest -q
来源：http://whw.ywan-chungtsiang.top

[U32] Py：代码格式化
来源：http://iju.haohaochexian.top

ruff format . && ruff check --fix .
来源：http://ufh.vehdjk.com

[U33] Py：打包发布
来源：http://hjh.shanyushiyangkeji.top

python -m build  （依赖 pyproject.toml）
来源：http://lsl.yangfankeji.com

[U34] Py：判断编码
来源：http://mmc.quarkkingdee.top

chardet.detect(raw)
来源：http://jpr.hammf.cn

[U35] Py：发送邮件
来源：http://cbf.chenlongwang.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pwj.jyoumei.cn

[U36] Py：定时任务
来源：http://fop.fengsongda.top

schedule.every(10).minutes.do(job)
来源：http://rau.shanyushiyangtech.top

[U37] Py：读写 Excel
来源：http://xex.jinghuilouyu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://par.redwolf501.top

[U38] Py：获取脚本所在目录
来源：http://eae.xuanzx.com

Path(__file__).resolve().parent
来源：http://rhy.tanke756.top

[U39] Py：判断是否在交互环境
来源：http://bmk.sjlbkw.cn

sys.stdout.isatty()
来源：http://mim.dianchejie.cn

[U40] Py：打印到标准错误
来源：http://jkv.ywan-chungtsiang.top

print("err", file=sys.stderr)
来源：http://uod.shanyushiyangkeji.top

[U41] PHP：初始化 Composer 项目
来源：http://due.yuxming.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dni.zhengqikj.top

[U42] PHP：PSR-4 自动加载
来源：http://yey.daxiang520.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rro.gotoacloud.top

[U43] PHP：声明命名空间
来源：http://qpk.sxryk.cn

namespace App\Http;
来源：http://aem.havefunace.top

[U44] PHP：开启严格类型
来源：http://qaq.pengpengdd.cyou

declare(strict_types=1);
来源：http://nrt.zhoulong.xyz

[U45] PHP：类型声明与返回类型
来源：http://tuf.kuanghao11.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nmb.svipenyu.cn

[U46] PHP：可空类型
来源：http://ipk.fengsongda.top

?string $name = null
来源：http://zei.aizwys.cn

[U47] PHP：联合类型
来源：http://hjd.xziqi.cn

int|string $id
来源：http://hnv.ywan-chungtsiang.top

[U48] PHP：纯枚举
来源：http://wth.sweek.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sgk.quarkkingdee.top

[U49] PHP：只读属性
来源：http://jrj.jinyuanbaomall.cn

public readonly string $name
来源：http://qhd.xziqi.cn

[U50] PHP：构造器属性提升
来源：http://saw.havefunace.top

public function __construct(private int $id) {}
来源：http://lss.guowangkeji.top

[U51] PHP：数组解构
来源：http://ert.yfazqb.com

[$a, $b] = $arr;
来源：http://cbx.hammf.cn

[U52] PHP：箭头函数
来源：http://jml.yj202588.top

$double = fn($x) => $x * 2;
来源：http://apa.snrcjt.cn

[U53] PHP：空合并运算符
来源：http://uet.ywan-chungtsiang.top

$v = $a ?? $b ?? "default";
来源：http://uhf.dianchejie.cn

[U54] PHP：空安全调用
来源：http://zdw.jqgufenzy.top

$obj?->method()
来源：http://flf.zdbjq.cn

[U55] PHP：match 表达式
来源：http://eoc.quarkkingdee.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zsd.zhongyouzk.top

[U56] PHP：命名参数
来源：http://tzg.zdbjq.cn

f(a: 1, b: 2)
来源：http://mfo.ybcxt.top

[U57] PHP：字符串插值
来源：http://iza.jlsjyb.cn

"值: {$a}"
来源：http://wlx.pengpengdd.cyou

[U58] PHP：数组三件套
来源：http://raw.iojbl.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jxn.hcnkem.com

[U59] PHP：自定义排序
来源：http://rqk.chenlongwang.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vdj.xziqi.cn

[U60] PHP：JSON 编解码
来源：http://dmg.0kj1m.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rbg.jqgfzy.top

[U61] PHP：正则
来源：http://nrz.xingfuxueyuan.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jer.hcnkem.com

[U62] PHP：日期对象
来源：http://uvm.xuanzx.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qbo.zhoulong.xyz

[U63] PHP：文件读写
来源：http://xbq.bjfxy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://orn.yongpay.top

[U64] PHP：目录遍历
来源：http://ugi.zhoulong.xyz

glob("dir/*.php");  scandir("dir");
来源：http://vob.xuetiantiany.cn

[U65] PHP：会话
来源：http://efw.jinqigufen.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ewt.mhx1999.top

[U66] PHP：设置 Cookie
来源：http://qzg.hcnkem.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://azu.quarkkingdee.top

[U67] PHP：处理文件上传
来源：http://lvw.xylfe.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xsv.gotoacloud.top

[U68] PHP：PDO 连接
来源：http://amu.bjfxy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dnj.ctjpmb.com

[U69] PHP：PDO 预处理
来源：http://hgz.316326.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xuw.meibo888.top

[U70] PHP：PDO 事务
来源：http://use.hfpthk.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lrg.bjfxy.top

[U71] PHP：抛出异常
来源：http://xum.sufxvd.cn

throw new RuntimeException("失败", 500);
来源：http://lny.quarkkingdee.top

[U72] PHP：写错误日志
来源：http://pua.iojbl.cn

error_log("失败: " . $e->getMessage());
来源：http://cnd.jyoumei.cn

[U73] PHP：读取 ini 配置
来源：http://yrg.hnxiangtu.top

parse_ini_file("config.ini", true)
来源：http://tgm.aibaodan.cn

[U74] PHP：读取环境变量
来源：http://irm.cqqwz.cn

getenv("APP_ENV") ?: "production"
来源：http://odk.wangshuangyany.cn

[U75] PHP：依赖注入
来源：http://mrh.zhengqikj.top

composer require psr/container
来源：http://fnb.jinqigfzy.top

[U76] PHP：简单路由
来源：http://dlf.fanxiaobao.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mbo.smart0.xyz

[U77] PHP：模板渲染
来源：http://vah.gaohongyu789.top

composer require twig/twig
来源：http://ggg.cashguo.top

[U78] PHP：单元测试
来源：http://als.jianghu66.top

composer require --dev phpunit/phpunit
来源：http://vrj.daria6918.cn

[U79] PHP：静态分析
来源：http://xly.meibo888.top

composer require --dev phpstan/phpstan
来源：http://hjb.xuetiantiany.cn

[U80] PHP：代码规范修复
来源：http://chp.cqqwz.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://igv.mhx1999.top

[U81] JS：初始化项目
来源：http://pff.ybcxt.top

npm init -y;  npm i express
来源：http://nqm.shangyingyoupin.top

[U82] JS：package.json 脚本
来源：http://xru.yueranfly.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gbg.c1oappe.top

[U83] JS：ES Module 导入导出
来源：http://yvk.fktsv.cn

export const a = 1;  import { a } from "./m.js";
来源：http://sso.dianchejie.cn

[U84] JS：CommonJS 写法
来源：http://wnq.cheryme.top

module.exports = { a };  const { a } = require("./m");
来源：http://ixo.wangdashe.top

[U85] JS：可选链
来源：http://vqr.shuidangran.top

a?.b?.c
来源：http://ouy.jinghuilouyu.cn

[U86] JS：空值合并
来源：http://mxb.yj20258.top

a ?? b
来源：http://rni.shzxlz.cn

[U87] JS：解构默认值
来源：http://ahe.0kj1m.cn

const { a = 1, b = 2 } = obj;
来源：http://nte.hywenlv.cn

[U88] JS：对象展开合并
来源：http://ksd.bbcook.cn

{ ...a, ...b }
来源：http://lav.havefunace.top

[U89] JS：数组去重
来源：http://spm.vehdjk.com

[...new Set(arr)]
来源：http://zqy.shanyushiyangtech.top

[U90] JS：数字数组排序
来源：http://ugf.sufxvd.cn

[...arr].sort((a, b) => a - b)
来源：http://bfb.uphjek.com

[U91] JS：对象键值遍历
来源：http://gsh.zycfv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sle.jinqigfzy.top

[U92] JS：深拷贝
来源：http://ulw.yvedp.cn

structuredClone(obj)
来源：http://cji.yvedp.cn

[U93] JS：模板字符串
来源：http://gad.tarul.cn

`共 ${n} 条`
来源：http://fwl.yongpay.top

[U94] JS：箭头函数
来源：http://tuo.ybcxt.top

const double = x => x * 2;
来源：http://lwm.jinqigfzy.top

[U95] JS：Promise 包装
来源：http://zrs.tianlin.xyz

new Promise((resolve, reject) => {})
来源：http://ysk.xuanzx.com

[U96] JS：async/await 与异常
来源：http://emb.fanxiaobao.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://suy.yueranfly.top

[U97] JS：并发请求
来源：http://feh.nanxuanxn.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ilv.xylfe.cn

[U98] JS：fetch 带 JSON
来源：http://bba.uphjek.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mqy.xuetiantiany.cn

[U99] JS：事件监听
来源：http://hay.gogol.net.cn

el.addEventListener("click", e => {})
来源：http://afc.daxiang520.top

[U100] JS：DOM 查询
来源：http://isu.snrcjt.cn

document.querySelector(".item")
来源：http://dgp.316326.xyz

[U101] JS：classList 操作
来源：http://ofo.jinqigufen.top

el.classList.toggle("active")
来源：http://fhv.chenzaomai.com

[U102] JS：本地存储
来源：http://bkr.aibaodan.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://eay.9152youxi.cn

[U103] JS：定时器
来源：http://amf.jinyuanbaomall.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://iqz.zhoulong.xyz

[U104] JS：防抖
来源：http://cpb.pycfn.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://guq.wangshuangyany.cn

[U105] JS：节流
来源：http://hyu.hfpthk.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vxo.ydjk.org.cn

[U106] JS：日期格式化
来源：http://jqv.bbcook.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://htt.cucudq.cn

[U107] JS：数字千分位
来源：http://qha.jiagoushi.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://iik.ydjk.org.cn

[U108] JS：随机整数
来源：http://poq.xingfuxueyuan.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://oeo.zdqjudy.top

[U109] JS：数组分组
来源：http://zvu.jinqigufen.top

Object.groupBy(arr, x => x.type)
来源：http://oer.hnxiangtu.top

[U110] JS：数组分块
来源：http://mhl.hywenlv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jqs.shangyingyoupin.top

[U111] JS：对象转 Map
来源：http://ieh.havefunace.top

new Map(Object.entries(obj))
来源：http://sxy.yueranfly.top

[U112] JS：字符串补位
来源：http://sdj.cucudq.cn

"7".padStart(3, "0")
来源：http://dmr.gaohongyu789.top

[U113] JS：正则替换全部
来源：http://mua.xuanzx.com

s.replaceAll("a", "b")
来源：http://wtb.yanxiufei.cn

[U114] JS：JSON 深比较
来源：http://vvn.vehdjk.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://gjc.xuetiantiany.cn

[U115] JS：生成 UUID
来源：http://etd.ywan-chungtsiang.top

crypto.randomUUID()
来源：http://boz.9152youxi.cn

[U116] JS：类型检查（JSDoc）
来源：http://ahj.hammf.cn

/** @param {string} name */ function f(name) {}
来源：http://djk.zdqjudy.top

[U117] JS：单元测试
来源：http://ylh.chenzaomai.com

npm i -D vitest;  npx vitest
来源：http://rqd.xinyue.icu

[U118] JS：开发服务器
来源：http://oyf.ehwqpu.com

npm i -D vite;  npx vite
来源：http://njk.jianghu66.top

[U119] JS：生产构建
来源：http://scs.pycfn.com

npx vite build
来源：http://mqm.aizwys.cn

[U120] JS：读取环境变量（Vite）
来源：http://jlb.zdqjudy.top

import.meta.env.VITE_API_URL
来源：http://ldm.aizwys.cn

================================================================================
来源：http://pzu.gogol.net.cn

统计汇总
来源：http://uzb.zdqjudy.top

================================================================================
来源：http://bul.aizwys.cn

按语言统计（条）：
来源：http://jwi.mhx1999.top

Python ......... 252
来源：http://sug.zhengqikj.top

PHP ............ 252
来源：http://mkk.yfazqb.com

JavaScript ..... 252
来源：http://cwa.aibaodan.cn

TypeScript ..... 212
来源：http://enz.zhixingplan.top

Java ........... 212
来源：http://mqb.xziqi.cn

Go ............. 212
来源：http://lzo.jiagoushi.top

Ruby ........... 212
来源：http://zpb.cashguo.top

C# ............. 212
来源：http://nsd.aizwys.cn

C .............. 30
来源：http://gdk.nwbrower.top

C++ ............ 30
来源：http://udf.ydjk.org.cn

SQL ............ 90
来源：http://zou.xingfuxueyuan.xyz

Bash ........... 80
来源：http://bao.ybcxt.top

Kotlin ......... 15
来源：http://sft.gzhubu.top

Swift .......... 15
来源：http://wnq.shangyingyoupin.top

Lua ............ 10
来源：http://zqq.chenjidiqi.icu

Perl ........... 10
来源：http://spo.yj20258888.top

Scala .......... 10
来源：http://nxz.andypj.xyz

------------------------------------
来源：http://xzx.vqdsnc.cn

合计 ........... 2106 条
来源：http://mmp.jiagoushi.top

按章节统计：
来源：http://uih.jinyuanbaomall.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cuq.jqgufenzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qjv.yfazqb.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vqt.dashuyun.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://njo.vehdjk.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fku.hfpthk.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nhw.ydzc1.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://slj.xuetiantiany.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zjb.quarkkingdee.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vdg.quarkkingdee.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vmv.fktsv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vvn.ppjwa.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qpl.zdbjq.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jbp.nanxuanxn.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://irx.ydjk.org.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://frz.daxiang520.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xvx.hysaishi.cn

Q SQL 专题                              90
来源：http://gct.xuanzx.com

R Bash 专题                             80
来源：http://yau.bjfxy.top

S C / C++ 专题                          60
来源：http://len.hywenlv.cn

T 其他语言补充                          60
来源：http://cou.yfazqb.com

U 高频实用片段                         120
来源：http://xcp.bjfxy.top

------------------------------------
来源：http://zyn.yanxiufei.cn

合计                                  2106 条
来源：http://rga.iojbl.cn

--------------------------------------------------------------------------------
来源：http://qdh.xuanzx.com

使用提醒
来源：http://okl.yvedp.cn

--------------------------------------------------------------------------------
来源：http://izg.nanxuanxn.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://une.ydzc1.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bmo.sxryk.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hea.zhiwuduotai.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ibb.gzhubu.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xzo.hnqzz.top

—— 文件结束 ——
来源：http://grm.redwolf501.top

================================================================================
来源：http://zgh.jqgufenzy.top

程序语言常见例子速查手册（2024 版）
来源：http://wkp.fengsongda.top

Common Programming Examples Cheat Book
来源：http://cfo.dashuyun.cn

================================================================================
来源：http://vnw.hysaishi.cn

【收录内容】
来源：http://eln.yangfankeji.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://rog.ppjwa.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rby.jqgufenzy.top

SQL · Bash · C · C++
来源：http://fki.nanxuanxn.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jfz.kuanghao11.cn

【使用说明】
来源：http://jah.tian-w.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hxc.feifeiyinyue.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rfy.zycfv.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sbz.fengsongda.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jgm.tian-w.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://jfn.svipenyu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lnk.jinyuanbaomall.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wfb.yongpay.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gei.yuxming.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wki.xingfuxueyuan.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rnt.bbcook.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wyq.yangfankeji.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://rnl.fktsv.cn

【文件统计】
来源：http://dhe.havefunace.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://obf.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://ymx.birdmap.top

目  录
来源：http://lui.cdnleiting.top

--------------------------------------------------------------------------------
来源：http://owb.aizwys.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hst.tianlin.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zjh.c1oappe.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gck.iojbl.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qlz.svipenyu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://thq.zhijiandao.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tqo.hesvh.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ntr.c1oappe.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pqj.xziqi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gbz.ehwqpu.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gmh.hywenlv.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nwo.birdmap.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rkg.daxiang520.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lbe.snrcjt.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://erq.hfpthk.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qtj.yvedp.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zjp.bbcook.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://txm.guowangkeji.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://cbx.cucudq.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xfc.hysaishi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xsl.zdbjq.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://edi.ydzc1.top

================================================================================
来源：http://yfh.daria6918.cn

A. 基础语法与类型
来源：http://zmy.cashguo.top

================================================================================
来源：http://hxx.ctjpmb.com

[A01] Hello World
来源：http://tnz.hongshengwenyu.top

Py:   print("Hello, World!")
来源：http://zrq.hywenlv.cn

PHP:  echo "Hello, World!";
来源：http://exp.zhixingplan.top

JS:   console.log("Hello, World!");
来源：http://adt.guowangkeji.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tmu.guowangkeji.top

Java: System.out.println("Hello, World!");
来源：http://cio.meibo888.top

Go:   fmt.Println("Hello, World!")
来源：http://myp.zhixingplan.top

Ruby: puts "Hello, World!"
来源：http://mgy.yuxming.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://srg.yj202588.top

[A02] 变量声明与赋值
来源：http://wak.zhaomingkeji.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kli.yonumen.top

PHP:  $name = "Alex"; $age = 20;
来源：http://huu.jinyuanbaomall.cn

JS:   let name = "Alex"; const age = 20;
来源：http://eot.jinyuanbaomall.cn


<!-- 参考信息 -->