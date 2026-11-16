代发 wailian999

[U35] Py：发送邮件
来源：http://qjl.yj20258.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wty.jiagoushi.top

[U36] Py：定时任务
来源：http://vcd.iojbl.cn

schedule.every(10).minutes.do(job)
来源：http://wwr.cqqwz.cn

[U37] Py：读写 Excel
来源：http://mvu.dianchejie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kci.xuanzx.com

[U38] Py：获取脚本所在目录
来源：http://fbv.zdqjudy.top

Path(__file__).resolve().parent
来源：http://yaj.sysykeji.top

[U39] Py：判断是否在交互环境
来源：http://mtb.gzhubu.top

sys.stdout.isatty()
来源：http://rlr.sysykeji.top

[U40] Py：打印到标准错误
来源：http://cnx.gzhubu.top

print("err", file=sys.stderr)
来源：http://uam.pycfn.com

[U41] PHP：初始化 Composer 项目
来源：http://tdk.xuanzx.com

composer init;  composer require guzzlehttp/guzzle
来源：http://wba.tianlin.xyz

[U42] PHP：PSR-4 自动加载
来源：http://try.chenzaomai.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qhr.chenjidiqi.icu

[U43] PHP：声明命名空间
来源：http://fjm.pengpengdd.cyou

namespace App\Http;
来源：http://viq.yuanzhike.top

[U44] PHP：开启严格类型
来源：http://ocy.316326.xyz

declare(strict_types=1);
来源：http://nji.wangshuangyany.cn

[U45] PHP：类型声明与返回类型
来源：http://uew.shanyushiyangkeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xwv.shzxlz.cn

[U46] PHP：可空类型
来源：http://mxv.sysykeji.top

?string $name = null
来源：http://plo.gaohongyu789.top

[U47] PHP：联合类型
来源：http://eus.nanxinkj.top

int|string $id
来源：http://thh.c1oappe.top

[U48] PHP：纯枚举
来源：http://ktj.jinyuanbaomall.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gyw.yj20258888.top

[U49] PHP：只读属性
来源：http://hjk.pycfn.com

public readonly string $name
来源：http://lzo.xingfuxueyuan.xyz

[U50] PHP：构造器属性提升
来源：http://ref.316326.xyz

public function __construct(private int $id) {}
来源：http://sbq.zhijiandao.cn

[U51] PHP：数组解构
来源：http://rre.zhijiandao.cn

[$a, $b] = $arr;
来源：http://gme.sxryk.cn

[U52] PHP：箭头函数
来源：http://ekm.jyoumei.cn

$double = fn($x) => $x * 2;
来源：http://rac.shanyushiyangkeji.top

[U53] PHP：空合并运算符
来源：http://djw.redwolf501.top

$v = $a ?? $b ?? "default";
来源：http://zbp.svipenyu.cn

[U54] PHP：空安全调用
来源：http://qxh.yfazqb.com

$obj?->method()
来源：http://rop.ywan-chungtsiang.top

[U55] PHP：match 表达式
来源：http://qig.vqdsnc.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://iyk.smart0.xyz

[U56] PHP：命名参数
来源：http://lwf.yj20258888.top

f(a: 1, b: 2)
来源：http://lag.hywenlv.cn

[U57] PHP：字符串插值
来源：http://xik.daxiang520.top

"值: {$a}"
来源：http://hhf.smart0.xyz

[U58] PHP：数组三件套
来源：http://tjg.jiagoushi.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rbz.feifeiyinyue.top

[U59] PHP：自定义排序
来源：http://rya.shuidangran.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wyd.andypj.xyz

[U60] PHP：JSON 编解码
来源：http://zhd.pengpengdd.cyou

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zjx.guannengcc.top

[U61] PHP：正则
来源：http://rhs.zhongyouzk.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uhg.jinqigufen.top

[U62] PHP：日期对象
来源：http://cgo.shuidangran.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ddj.nanxinkj.top

[U63] PHP：文件读写
来源：http://dld.ybcxt.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mka.ybcxt.top

[U64] PHP：目录遍历
来源：http://oyy.cheryme.top

glob("dir/*.php");  scandir("dir");
来源：http://yfo.jianghu66.top

[U65] PHP：会话
来源：http://nkf.chenlongwang.top

session_start();  $_SESSION["uid"] = 1;
来源：http://hie.ydzc1.top

[U66] PHP：设置 Cookie
来源：http://wys.cheryme.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://plh.wangshuangyany.cn

[U67] PHP：处理文件上传
来源：http://jnd.ydjk.org.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mqy.jinqigufen.top

[U68] PHP：PDO 连接
来源：http://vpi.fanxiaobao.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lcs.c1oappe.top

[U69] PHP：PDO 预处理
来源：http://cua.gogol.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hhl.fzhhl.top

[U70] PHP：PDO 事务
来源：http://bgl.fktsv.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://oqb.sweek.top

[U71] PHP：抛出异常
来源：http://azh.ywan-chungtsiang.top

throw new RuntimeException("失败", 500);
来源：http://wbp.tian-w.cn

[U72] PHP：写错误日志
来源：http://snh.cdnleiting.top

error_log("失败: " . $e->getMessage());
来源：http://emr.fktsv.cn

[U73] PHP：读取 ini 配置
来源：http://rpb.gaohongyu789.top

parse_ini_file("config.ini", true)
来源：http://and.kuanghao11.cn

[U74] PHP：读取环境变量
来源：http://tfx.yueranfly.top

getenv("APP_ENV") ?: "production"
来源：http://ewj.yj20258.top

[U75] PHP：依赖注入
来源：http://udf.svipenyu.cn

composer require psr/container
来源：http://hyo.mhx1999.top

[U76] PHP：简单路由
来源：http://wzy.jianghu66.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jyi.shuidangran.top

[U77] PHP：模板渲染
来源：http://mld.haohaochexian.top

composer require twig/twig
来源：http://luz.nanxinkj.top

[U78] PHP：单元测试
来源：http://exj.xinyue.icu

composer require --dev phpunit/phpunit
来源：http://ont.zhixingplan.top

[U79] PHP：静态分析
来源：http://emo.zhixingplan.top

composer require --dev phpstan/phpstan
来源：http://mkl.fanxiaobao.xyz

[U80] PHP：代码规范修复
来源：http://mvb.cdnleiting.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://lui.hywenlv.cn

[U81] JS：初始化项目
来源：http://dcz.bjfxy.top

npm init -y;  npm i express
来源：http://kxl.fengsongda.top

[U82] JS：package.json 脚本
来源：http://sch.sufxvd.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://iks.smart0.xyz

[U83] JS：ES Module 导入导出
来源：http://igq.haohaochexian.top

export const a = 1;  import { a } from "./m.js";
来源：http://xqo.yvedp.cn

[U84] JS：CommonJS 写法
来源：http://esm.vehdjk.com

module.exports = { a };  const { a } = require("./m");
来源：http://zxo.tian-w.cn

[U85] JS：可选链
来源：http://kqb.jinqigfzy.top

a?.b?.c
来源：http://scd.xuetiantiany.cn

[U86] JS：空值合并
来源：http://ony.yongpay.top

a ?? b
来源：http://uxk.jinyuanbaomall.cn

[U87] JS：解构默认值
来源：http://aml.sweek.top

const { a = 1, b = 2 } = obj;
来源：http://sge.cqqwz.cn

[U88] JS：对象展开合并
来源：http://jws.tianlin.xyz

{ ...a, ...b }
来源：http://owo.cdnleiting.top

[U89] JS：数组去重
来源：http://kzt.zdqjudy.top

[...new Set(arr)]
来源：http://ivb.guowangkeji.top

[U90] JS：数字数组排序
来源：http://erv.chenzaomai.com

[...arr].sort((a, b) => a - b)
来源：http://zak.yfazqb.com

[U91] JS：对象键值遍历
来源：http://sbu.smart0.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://jfm.pengpengdd.cyou

[U92] JS：深拷贝
来源：http://ysq.yfazqb.com

structuredClone(obj)
来源：http://zsc.tian-w.cn

[U93] JS：模板字符串
来源：http://ygg.xziqi.cn

`共 ${n} 条`
来源：http://eih.yuxming.cn

[U94] JS：箭头函数
来源：http://njz.aibaodan.cn

const double = x => x * 2;
来源：http://kld.jiagoushi.top

[U95] JS：Promise 包装
来源：http://fzx.kuanghao11.cn

new Promise((resolve, reject) => {})
来源：http://lfn.pycfn.com

[U96] JS：async/await 与异常
来源：http://orc.xuetiantiany.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nji.316326.xyz

[U97] JS：并发请求
来源：http://omt.yueranfly.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://jxf.zhixingplan.top

[U98] JS：fetch 带 JSON
来源：http://kqb.mhx1999.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dma.mhx1999.top

[U99] JS：事件监听
来源：http://vdg.ppjwa.cn

el.addEventListener("click", e => {})
来源：http://jlg.gogol.net.cn

[U100] JS：DOM 查询
来源：http://hck.cheryme.top

document.querySelector(".item")
来源：http://wnk.quarkkingdee.top

[U101] JS：classList 操作
来源：http://mfc.shangyingyoupin.top

el.classList.toggle("active")
来源：http://jcu.zycfv.cn

[U102] JS：本地存储
来源：http://zbz.ydjk.org.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wcx.xziqi.cn

[U103] JS：定时器
来源：http://irr.sxryk.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jrz.hysaishi.cn

[U104] JS：防抖
来源：http://odo.gotoacloud.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vsg.gaohongyu789.top

[U105] JS：节流
来源：http://vqs.tanke756.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rga.cucudq.cn

[U106] JS：日期格式化
来源：http://xsw.epnwcf.com

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bgl.pycfn.com

[U107] JS：数字千分位
来源：http://cws.jianghu66.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://btg.dashuyun.cn

[U108] JS：随机整数
来源：http://uab.ppjwa.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://abf.zhaomingkeji.xyz

[U109] JS：数组分组
来源：http://byk.jyoumei.cn

Object.groupBy(arr, x => x.type)
来源：http://knt.gogol.net.cn

[U110] JS：数组分块
来源：http://ztk.hesvh.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ljn.nwbrower.top

[U111] JS：对象转 Map
来源：http://nzv.sysykeji.top

new Map(Object.entries(obj))
来源：http://efc.jqgufenzy.top

[U112] JS：字符串补位
来源：http://sws.yanxiufei.cn

"7".padStart(3, "0")
来源：http://iow.mhx1999.top

[U113] JS：正则替换全部
来源：http://oyu.yj20258888.top

s.replaceAll("a", "b")
来源：http://bfm.aizwys.cn

[U114] JS：JSON 深比较
来源：http://wiu.yuxming.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://oxm.xuetiantiany.cn

[U115] JS：生成 UUID
来源：http://tgs.cucudq.cn

crypto.randomUUID()
来源：http://chh.gzhubu.top

[U116] JS：类型检查（JSDoc）
来源：http://kmf.sufxvd.cn

/** @param {string} name */ function f(name) {}
来源：http://vvj.iojbl.cn

[U117] JS：单元测试
来源：http://ohg.jinqigfzy.top

npm i -D vitest;  npx vitest
来源：http://zyq.gaohongyu789.top

[U118] JS：开发服务器
来源：http://esp.quarkkingdee.top

npm i -D vite;  npx vite
来源：http://fow.svipenyu.cn

[U119] JS：生产构建
来源：http://lsp.yangfankeji.com

npx vite build
来源：http://gcn.ydzc1.top

[U120] JS：读取环境变量（Vite）
来源：http://leb.fengsongda.top

import.meta.env.VITE_API_URL
来源：http://zac.guowangkeji.top

================================================================================
来源：http://ioz.gaohongyu789.top

统计汇总
来源：http://wgc.zhoulong.xyz

================================================================================
来源：http://kfx.snrcjt.cn

按语言统计（条）：
来源：http://dmt.aizwys.cn

Python ......... 252
来源：http://orw.shanyushiyangkeji.top

PHP ............ 252
来源：http://ujt.zhiwuduotai.top

JavaScript ..... 252
来源：http://juy.daria6918.cn

TypeScript ..... 212
来源：http://kcx.quarkkingdee.top

Java ........... 212
来源：http://whq.zdbjq.cn

Go ............. 212
来源：http://ojm.zhengqikj.top

Ruby ........... 212
来源：http://nlu.fktsv.cn

C# ............. 212
来源：http://ham.zhongyouzk.top

C .............. 30
来源：http://eow.ehwqpu.com

C++ ............ 30
来源：http://zjl.9152youxi.cn

SQL ............ 90
来源：http://dro.yueranfly.top

Bash ........... 80
来源：http://nir.bbcook.cn

Kotlin ......... 15
来源：http://mpx.zhijiandao.cn

Swift .......... 15
来源：http://axy.smart0.xyz

Lua ............ 10
来源：http://ppc.yj20258888.top

Perl ........... 10
来源：http://yri.quarkkingdee.top

Scala .......... 10
来源：http://hmg.tianlin.xyz

------------------------------------
来源：http://qhm.zhengqikj.top

合计 ........... 2106 条
来源：http://khn.yj20258.top

按章节统计：
来源：http://tda.zhoulong.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pfm.jqgufenzy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://eri.fengsongda.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sjc.hongshengwenyu.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qbw.c1oappe.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xoq.ydzc1.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rxx.cqqwz.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ozz.shanyushiyangtech.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://oov.fanxiaobao.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bmm.zdbjq.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ktg.hnxiangtu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kpe.hesvh.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pqw.yuanzhike.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nln.tanke756.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sxe.chenjidiqi.icu

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://efe.hammf.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jhq.cdnleiting.top

Q SQL 专题                              90
来源：http://ioc.xinyue.icu

R Bash 专题                             80
来源：http://eve.zdbjq.cn

S C / C++ 专题                          60
来源：http://qtd.jqgfzy.top

T 其他语言补充                          60
来源：http://zur.cheryme.top

U 高频实用片段                         120
来源：http://sul.cqqwz.cn

------------------------------------
来源：http://rbs.hysaishi.cn

合计                                  2106 条
来源：http://ifa.jinqigufen.top

--------------------------------------------------------------------------------
来源：http://xyu.yonumen.top

使用提醒
来源：http://evw.tanke756.top

--------------------------------------------------------------------------------
来源：http://siv.cheryme.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://usw.chenzaomai.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://flz.quarkkingdee.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://esd.yueranfly.top

在旧版本上使用前请先确认语法支持情况。
来源：http://ara.redwolf501.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mfv.havefunace.top

—— 文件结束 ——
来源：http://hjc.jqgufenzy.top

================================================================================
来源：http://few.cheryme.top

程序语言常见例子速查手册（2024 版）
来源：http://wss.xylfe.cn

Common Programming Examples Cheat Book
来源：http://vem.bjfxy.top

================================================================================
来源：http://zyt.yj20258888.top

【收录内容】
来源：http://mae.xuanzx.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://ksn.yj202588.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kco.pycfn.com

SQL · Bash · C · C++
来源：http://nqo.chenjidiqi.icu

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qtn.hnxiangtu.top

【使用说明】
来源：http://jhk.sysykeji.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ejj.ybcxt.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nzt.hcnkem.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://iwt.tanke756.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://asm.hammf.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://yro.fzhhl.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dxn.xuanzx.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://soa.tanke756.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rfr.xylfe.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ixw.jinghuilouyu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kew.daxiang520.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gwb.aibaodan.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mea.smart0.xyz

【文件统计】
来源：http://dru.epnwcf.com

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pcv.ctjpmb.com

--------------------------------------------------------------------------------
来源：http://vnf.ydjk.org.cn

目  录
来源：http://pjt.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://lvb.smart0.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ody.ydjk.org.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rvp.aizwys.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gba.cqqwz.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dhk.wangshuangyany.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://plk.yongpay.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://eds.zhengqikj.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ztc.daxiang520.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ium.gotoacloud.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ztu.yfazqb.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pyi.yongpay.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://glm.meibo888.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://aoe.hysaishi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ndb.fzhhl.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ukc.shzxlz.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://egx.redwolf501.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xku.svipenyu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jsl.ywan-chungtsiang.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ggq.fzhhl.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rla.mhx1999.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uth.kuanghao11.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cgy.snrcjt.cn

================================================================================
来源：http://cik.zhaomingkeji.xyz

A. 基础语法与类型
来源：http://zcv.aibaodan.cn

================================================================================
来源：http://rxl.pycfn.com

[A01] Hello World
来源：http://diu.guowangkeji.top

Py:   print("Hello, World!")
来源：http://aeb.fanxiaobao.xyz

PHP:  echo "Hello, World!";
来源：http://had.shangyingyoupin.top

JS:   console.log("Hello, World!");
来源：http://ugi.jinyuanbaomall.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://meo.9152youxi.cn

Java: System.out.println("Hello, World!");
来源：http://opn.zhongyouzk.top

Go:   fmt.Println("Hello, World!")
来源：http://sxf.jinqigfzy.top

Ruby: puts "Hello, World!"
来源：http://mcb.vqdsnc.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://dmz.cheryme.top

[A02] 变量声明与赋值
来源：http://xoa.vqdsnc.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jph.hysaishi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://dwx.wangdashe.top

JS:   let name = "Alex"; const age = 20;
来源：http://bga.hnqzz.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://foh.yangfankeji.com

Java: String name = "Alex"; int age = 20;
来源：http://gjc.xingfuxueyuan.xyz

Go:   name := "Alex"; age := 20
来源：http://pll.yfazqb.com

Ruby: name = "Alex"; age = 20
来源：http://zok.jianghu66.top

C#:   string name = "Alex"; int age = 20;
来源：http://wgf.epnwcf.com

[A03] 常量定义
来源：http://akp.xuanzx.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qpm.redwolf501.top

PHP:  const PI = 3.14159;
来源：http://dhx.andypj.xyz


<!-- 参考信息 -->