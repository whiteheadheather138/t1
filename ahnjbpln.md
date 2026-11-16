代发 wailian999

[U27] Py：异步 HTTP
来源：http://cjk.hnxiangtu.top

aiohttp.ClientSession() 配合 async with
来源：http://yhp.shanyushiyangkeji.top

[U28] Py：类型别名
来源：http://cdd.dashuyun.cn

UserId = int
来源：http://otz.cdnleiting.top

[U29] Py：属性校验
来源：http://zbh.ctjpmb.com

@property 与 @x.setter 配合
来源：http://don.hcnkem.com

[U30] Py：数据类
来源：http://qtn.chenjidiqi.icu

@dataclass(slots=True)
来源：http://zgx.tarul.cn

[U31] Py：单测
来源：http://izw.svipenyu.cn

python -m pytest -q
来源：http://nbu.tian-w.cn

[U32] Py：代码格式化
来源：http://qxx.tarul.cn

ruff format . && ruff check --fix .
来源：http://rww.guannengcc.top

[U33] Py：打包发布
来源：http://cwo.hnqzz.top

python -m build  （依赖 pyproject.toml）
来源：http://dpt.ehwqpu.com

[U34] Py：判断编码
来源：http://ygu.zhaomingkeji.xyz

chardet.detect(raw)
来源：http://igk.yuxming.cn

[U35] Py：发送邮件
来源：http://fix.zdbjq.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ert.tarul.cn

[U36] Py：定时任务
来源：http://crk.bbcook.cn

schedule.every(10).minutes.do(job)
来源：http://dvt.bjfxy.top

[U37] Py：读写 Excel
来源：http://pdj.nanxuanxn.top

pandas.read_excel / DataFrame.to_excel
来源：http://aez.ppjwa.cn

[U38] Py：获取脚本所在目录
来源：http://dir.iojbl.cn

Path(__file__).resolve().parent
来源：http://twx.wangdashe.top

[U39] Py：判断是否在交互环境
来源：http://kxv.aibaodan.cn

sys.stdout.isatty()
来源：http://srr.hnxiangtu.top

[U40] Py：打印到标准错误
来源：http://yfj.fktsv.cn

print("err", file=sys.stderr)
来源：http://trn.zhaomingkeji.xyz

[U41] PHP：初始化 Composer 项目
来源：http://xsc.jinghuilouyu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lki.zhoulong.xyz

[U42] PHP：PSR-4 自动加载
来源：http://xwj.yongpay.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://oqf.cashguo.top

[U43] PHP：声明命名空间
来源：http://rhf.yfazqb.com

namespace App\Http;
来源：http://acy.tian-w.cn

[U44] PHP：开启严格类型
来源：http://xrq.sufxvd.cn

declare(strict_types=1);
来源：http://nzz.sjlbkw.cn

[U45] PHP：类型声明与返回类型
来源：http://aht.316326.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://poy.shuidangran.top

[U46] PHP：可空类型
来源：http://jop.xingfuxueyuan.xyz

?string $name = null
来源：http://iey.nanxuanxn.top

[U47] PHP：联合类型
来源：http://pwz.epnwcf.com

int|string $id
来源：http://qqe.gogol.net.cn

[U48] PHP：纯枚举
来源：http://uyk.jlsjyb.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gti.52xcode.cn

[U49] PHP：只读属性
来源：http://emg.hywenlv.cn

public readonly string $name
来源：http://iei.hcnkem.com

[U50] PHP：构造器属性提升
来源：http://dwc.sxryk.cn

public function __construct(private int $id) {}
来源：http://qwz.bbcook.cn

[U51] PHP：数组解构
来源：http://owj.iojbl.cn

[$a, $b] = $arr;
来源：http://tgj.tanke756.top

[U52] PHP：箭头函数
来源：http://pnc.jyoumei.cn

$double = fn($x) => $x * 2;
来源：http://flo.tanke756.top

[U53] PHP：空合并运算符
来源：http://iuo.hfpthk.cn

$v = $a ?? $b ?? "default";
来源：http://bfl.zhongyouzk.top

[U54] PHP：空安全调用
来源：http://rnt.meibo888.top

$obj?->method()
来源：http://jnx.ywan-chungtsiang.top

[U55] PHP：match 表达式
来源：http://fou.yvedp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cnn.chenjidiqi.icu

[U56] PHP：命名参数
来源：http://gpa.andypj.xyz

f(a: 1, b: 2)
来源：http://dsh.yonumen.top

[U57] PHP：字符串插值
来源：http://mlr.52xcode.cn

"值: {$a}"
来源：http://gdc.quarkkingdee.top

[U58] PHP：数组三件套
来源：http://irz.jyoumei.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://clm.birdmap.top

[U59] PHP：自定义排序
来源：http://lxg.mhx1999.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zoe.gotoacloud.top

[U60] PHP：JSON 编解码
来源：http://twl.9152youxi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://maj.havefunace.top

[U61] PHP：正则
来源：http://lzj.jinqigfzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://daf.jiagoushi.top

[U62] PHP：日期对象
来源：http://zii.nanxuanxn.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lyo.yonumen.top

[U63] PHP：文件读写
来源：http://qlh.nanxuanxn.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kdj.quarkkingdee.top

[U64] PHP：目录遍历
来源：http://ggn.chenjidiqi.icu

glob("dir/*.php");  scandir("dir");
来源：http://bfg.sysykeji.top

[U65] PHP：会话
来源：http://wxy.iojbl.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xgu.hongshengwenyu.top

[U66] PHP：设置 Cookie
来源：http://gep.jianghu66.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xia.aizwys.cn

[U67] PHP：处理文件上传
来源：http://jvo.yuxming.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xgq.nwbrower.top

[U68] PHP：PDO 连接
来源：http://cle.wangshuangyany.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dgv.meibo888.top

[U69] PHP：PDO 预处理
来源：http://aun.gaohongyu789.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xrl.cqqwz.cn

[U70] PHP：PDO 事务
来源：http://caa.quarkkingdee.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://iep.snrcjt.cn

[U71] PHP：抛出异常
来源：http://pxt.birdmap.top

throw new RuntimeException("失败", 500);
来源：http://uta.tanke756.top

[U72] PHP：写错误日志
来源：http://whb.ehwqpu.com

error_log("失败: " . $e->getMessage());
来源：http://tjd.tarul.cn

[U73] PHP：读取 ini 配置
来源：http://txi.hysaishi.cn

parse_ini_file("config.ini", true)
来源：http://cfq.xinyue.icu

[U74] PHP：读取环境变量
来源：http://amb.hesvh.cn

getenv("APP_ENV") ?: "production"
来源：http://nqi.ivvv.top

[U75] PHP：依赖注入
来源：http://pvg.cdnleiting.top

composer require psr/container
来源：http://riy.zhijiandao.cn

[U76] PHP：简单路由
来源：http://lxf.jqgfzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dxr.hywenlv.cn

[U77] PHP：模板渲染
来源：http://adb.zhixingplan.top

composer require twig/twig
来源：http://aab.ctjpmb.com

[U78] PHP：单元测试
来源：http://qaj.jinqigfzy.top

composer require --dev phpunit/phpunit
来源：http://dbu.birdmap.top

[U79] PHP：静态分析
来源：http://clb.sweek.top

composer require --dev phpstan/phpstan
来源：http://uai.meibo888.top

[U80] PHP：代码规范修复
来源：http://pud.yvedp.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dbc.bbcook.cn

[U81] JS：初始化项目
来源：http://vuz.fehbvm.com

npm init -y;  npm i express
来源：http://sao.yuanzhike.top

[U82] JS：package.json 脚本
来源：http://pja.haohaochexian.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qog.tianlin.xyz

[U83] JS：ES Module 导入导出
来源：http://slk.pycfn.com

export const a = 1;  import { a } from "./m.js";
来源：http://iux.gzhubu.top

[U84] JS：CommonJS 写法
来源：http://zyz.zdqjudy.top

module.exports = { a };  const { a } = require("./m");
来源：http://odk.c1oappe.top

[U85] JS：可选链
来源：http://hoy.dashuyun.cn

a?.b?.c
来源：http://xcn.zhixingplan.top

[U86] JS：空值合并
来源：http://epm.9152youxi.cn

a ?? b
来源：http://hoy.xingfuxueyuan.xyz

[U87] JS：解构默认值
来源：http://rng.hongshengwenyu.top

const { a = 1, b = 2 } = obj;
来源：http://tiy.52xcode.cn

[U88] JS：对象展开合并
来源：http://cwa.feifeiyinyue.top

{ ...a, ...b }
来源：http://lqe.shanyushiyangkeji.top

[U89] JS：数组去重
来源：http://jmo.0kj1m.cn

[...new Set(arr)]
来源：http://jhj.zhixingplan.top

[U90] JS：数字数组排序
来源：http://fdw.zhiwuduotai.top

[...arr].sort((a, b) => a - b)
来源：http://spt.ydjk.org.cn

[U91] JS：对象键值遍历
来源：http://cyr.jianghu66.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qyp.yfazqb.com

[U92] JS：深拷贝
来源：http://wss.sysykeji.top

structuredClone(obj)
来源：http://mto.cucudq.cn

[U93] JS：模板字符串
来源：http://kqp.hfpthk.cn

`共 ${n} 条`
来源：http://mky.meibo888.top

[U94] JS：箭头函数
来源：http://acs.ehwqpu.com

const double = x => x * 2;
来源：http://gri.vehdjk.com

[U95] JS：Promise 包装
来源：http://jot.hnqzz.top

new Promise((resolve, reject) => {})
来源：http://kav.guowangkeji.top

[U96] JS：async/await 与异常
来源：http://uuu.cashguo.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://swx.cqqwz.cn

[U97] JS：并发请求
来源：http://kvc.yj20258.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://bmq.ppjwa.cn

[U98] JS：fetch 带 JSON
来源：http://dop.tanke756.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vbu.0kj1m.cn

[U99] JS：事件监听
来源：http://ees.ydzc1.top

el.addEventListener("click", e => {})
来源：http://iir.hfpthk.cn

[U100] JS：DOM 查询
来源：http://lxp.dashuyun.cn

document.querySelector(".item")
来源：http://cbl.zhiwuduotai.top

[U101] JS：classList 操作
来源：http://txp.shuidangran.top

el.classList.toggle("active")
来源：http://rbu.zhixingplan.top

[U102] JS：本地存储
来源：http://glw.jinqigfzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://gep.0kj1m.cn

[U103] JS：定时器
来源：http://tgh.yvedp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kuo.xylfe.cn

[U104] JS：防抖
来源：http://bkl.gzhubu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sop.zhijiandao.cn

[U105] JS：节流
来源：http://ckq.guannengcc.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vdk.sweek.top

[U106] JS：日期格式化
来源：http://czi.svipenyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wfv.shanyushiyangkeji.top

[U107] JS：数字千分位
来源：http://vkr.shuidangran.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dyf.yj20258.top

[U108] JS：随机整数
来源：http://qlm.bbcook.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qvc.yanxiufei.cn

[U109] JS：数组分组
来源：http://hfb.redwolf501.top

Object.groupBy(arr, x => x.type)
来源：http://nil.hammf.cn

[U110] JS：数组分块
来源：http://dfw.jinyuanbaomall.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pve.jiagoushi.top

[U111] JS：对象转 Map
来源：http://vny.guannengcc.top

new Map(Object.entries(obj))
来源：http://tpd.yonumen.top

[U112] JS：字符串补位
来源：http://lqx.zdbjq.cn

"7".padStart(3, "0")
来源：http://kgc.zhaomingkeji.xyz

[U113] JS：正则替换全部
来源：http://fcl.ybcxt.top

s.replaceAll("a", "b")
来源：http://com.zhaomingkeji.xyz

[U114] JS：JSON 深比较
来源：http://ugr.yj20258888.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://xlp.dashuyun.cn

[U115] JS：生成 UUID
来源：http://not.guannengcc.top

crypto.randomUUID()
来源：http://sbh.316326.xyz

[U116] JS：类型检查（JSDoc）
来源：http://hbo.snrcjt.cn

/** @param {string} name */ function f(name) {}
来源：http://fht.jinyuanbaomall.cn

[U117] JS：单元测试
来源：http://ajq.gaohongyu789.top

npm i -D vitest;  npx vitest
来源：http://qvl.zhiwuduotai.top

[U118] JS：开发服务器
来源：http://rxl.uphjek.com

npm i -D vite;  npx vite
来源：http://upo.chenjidiqi.icu

[U119] JS：生产构建
来源：http://wxy.hnxiangtu.top

npx vite build
来源：http://lzt.hysaishi.cn

[U120] JS：读取环境变量（Vite）
来源：http://bbq.fktsv.cn

import.meta.env.VITE_API_URL
来源：http://lsf.yuanzhike.top

================================================================================
来源：http://dbf.gaohongyu789.top

统计汇总
来源：http://xpd.ivvv.top

================================================================================
来源：http://yzr.xinyue.icu

按语言统计（条）：
来源：http://tfo.ctjpmb.com

Python ......... 252
来源：http://wkn.yanxiufei.cn

PHP ............ 252
来源：http://loj.xingfuxueyuan.xyz

JavaScript ..... 252
来源：http://uok.ydjk.org.cn

TypeScript ..... 212
来源：http://tqu.bbcook.cn

Java ........... 212
来源：http://ezf.hammf.cn

Go ............. 212
来源：http://uds.wangshuangyany.cn

Ruby ........... 212
来源：http://wjy.ydzc1.top

C# ............. 212
来源：http://ltk.gaohongyu789.top

C .............. 30
来源：http://kot.316326.xyz

C++ ............ 30
来源：http://ubl.yueranfly.top

SQL ............ 90
来源：http://leo.yongpay.top

Bash ........... 80
来源：http://bdu.ppjwa.cn

Kotlin ......... 15
来源：http://gez.xziqi.cn

Swift .......... 15
来源：http://atj.chenzaomai.com

Lua ............ 10
来源：http://gep.tianlin.xyz

Perl ........... 10
来源：http://hpc.hammf.cn

Scala .......... 10
来源：http://qjq.hfpthk.cn

------------------------------------
来源：http://ckh.daria6918.cn

合计 ........... 2106 条
来源：http://qij.wangshuangyany.cn

按章节统计：
来源：http://ers.jinghuilouyu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zvy.yangfankeji.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://olu.nanxinkj.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://msp.pycfn.com

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nit.cucudq.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gab.fanxiaobao.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lty.andypj.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://pwx.ydzc1.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vqp.ppjwa.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nnq.yvedp.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dge.birdmap.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://npo.tian-w.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sgh.yj20258888.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mpw.feifeiyinyue.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://gvx.pengpengdd.cyou

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jmz.andypj.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kqm.ehwqpu.com

Q SQL 专题                              90
来源：http://gyc.bbcook.cn

R Bash 专题                             80
来源：http://qnb.svipenyu.cn

S C / C++ 专题                          60
来源：http://xny.bbcook.cn

T 其他语言补充                          60
来源：http://cra.hnxiangtu.top

U 高频实用片段                         120
来源：http://qrv.jianghu66.top

------------------------------------
来源：http://nzz.andypj.xyz

合计                                  2106 条
来源：http://xzp.9152youxi.cn

--------------------------------------------------------------------------------
来源：http://lob.9152youxi.cn

使用提醒
来源：http://gqf.chenzaomai.com

--------------------------------------------------------------------------------
来源：http://tua.jinyuanbaomall.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tvu.nanxinkj.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://qkr.yj202588.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ftm.jlsjyb.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://nnf.ctjpmb.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nri.zhengqikj.top

—— 文件结束 ——
来源：http://mvk.haohaochexian.top

================================================================================
来源：http://sfa.kuanghao11.cn

程序语言常见例子速查手册（2024 版）
来源：http://bjh.mhx1999.top

Common Programming Examples Cheat Book
来源：http://hsu.shanyushiyangtech.top

================================================================================
来源：http://ino.ctjpmb.com

【收录内容】
来源：http://rus.sysykeji.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://azw.ydjk.org.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tdc.jinqigfzy.top

SQL · Bash · C · C++
来源：http://mdp.hysaishi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mgr.zdbjq.cn

【使用说明】
来源：http://ulq.shuidangran.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hzv.havefunace.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://znr.mhx1999.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xue.redwolf501.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://six.yongpay.top

Bash:  Shell         C:     C             C++:   C++
来源：http://ptf.wangshuangyany.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://oio.jinyuanbaomall.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qqz.sweek.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://sic.sjlbkw.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jfy.dashuyun.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cjl.yanxiufei.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gzd.hesvh.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ywc.hnqzz.top

【文件统计】
来源：http://sub.zdbjq.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cyi.tarul.cn

--------------------------------------------------------------------------------
来源：http://rmt.guannengcc.top

目  录
来源：http://bjz.yuxming.cn

--------------------------------------------------------------------------------
来源：http://oso.zhixingplan.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yui.iojbl.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vha.0kj1m.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://trz.sjlbkw.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://emg.zhixingplan.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sjs.316326.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ddu.epnwcf.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gcp.jqgufenzy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ehk.jinqigufen.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ijm.yuanzhike.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://quw.yuxming.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qjz.snrcjt.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lfy.0kj1m.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kgk.quarkkingdee.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yym.hesvh.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jwc.havefunace.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tfz.tarul.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bjv.jinqigufen.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://nkd.ehwqpu.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fqx.cdnleiting.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ocr.yueranfly.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ohy.ctjpmb.com

================================================================================
来源：http://cvf.gzhubu.top

A. 基础语法与类型
来源：http://dzf.chenzaomai.com

================================================================================
来源：http://fjg.vehdjk.com

[A01] Hello World
来源：http://ooz.0kj1m.cn

Py:   print("Hello, World!")
来源：http://lhu.hammf.cn

PHP:  echo "Hello, World!";
来源：http://bxj.cdnleiting.top

JS:   console.log("Hello, World!");
来源：http://dfz.haohaochexian.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lni.aibaodan.cn


<!-- 参考信息 -->