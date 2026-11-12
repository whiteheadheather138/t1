代发 wailian999

[U27] Py：异步 HTTP
来源：http://mqk.sysykeji.top

aiohttp.ClientSession() 配合 async with
来源：http://shv.dianchejie.cn

[U28] Py：类型别名
来源：http://xmy.hfpthk.cn

UserId = int
来源：http://jsf.c1oappe.top

[U29] Py：属性校验
来源：http://nin.yfazqb.com

@property 与 @x.setter 配合
来源：http://lhb.chenjidiqi.icu

[U30] Py：数据类
来源：http://hpu.cdnleiting.top

@dataclass(slots=True)
来源：http://pzm.haohaochexian.top

[U31] Py：单测
来源：http://ypr.jinyuanbaomall.cn

python -m pytest -q
来源：http://scy.wangshuangyany.cn

[U32] Py：代码格式化
来源：http://axu.fzhhl.top

ruff format . && ruff check --fix .
来源：http://gey.316326.xyz

[U33] Py：打包发布
来源：http://fef.nanxuanxn.top

python -m build  （依赖 pyproject.toml）
来源：http://ckb.pycfn.com

[U34] Py：判断编码
来源：http://anb.redwolf501.top

chardet.detect(raw)
来源：http://btd.cqqwz.cn

[U35] Py：发送邮件
来源：http://xna.jinqigufen.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yws.wangshuangyany.cn

[U36] Py：定时任务
来源：http://ttf.shuidangran.top

schedule.every(10).minutes.do(job)
来源：http://esx.zhaomingkeji.xyz

[U37] Py：读写 Excel
来源：http://hpf.nanxuanxn.top

pandas.read_excel / DataFrame.to_excel
来源：http://eaj.jinqigufen.top

[U38] Py：获取脚本所在目录
来源：http://efd.chenzaomai.com

Path(__file__).resolve().parent
来源：http://obn.wangshuangyany.cn

[U39] Py：判断是否在交互环境
来源：http://yah.xuanzx.com

sys.stdout.isatty()
来源：http://vmj.shanyushiyangtech.top

[U40] Py：打印到标准错误
来源：http://hdo.xinyue.icu

print("err", file=sys.stderr)
来源：http://byc.yuanzhike.top

[U41] PHP：初始化 Composer 项目
来源：http://jig.mhx1999.top

composer init;  composer require guzzlehttp/guzzle
来源：http://xgs.pycfn.com

[U42] PHP：PSR-4 自动加载
来源：http://ceg.hfpthk.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zoy.yj20258.top

[U43] PHP：声明命名空间
来源：http://htp.tarul.cn

namespace App\Http;
来源：http://elj.bbcook.cn

[U44] PHP：开启严格类型
来源：http://ald.yj20258888.top

declare(strict_types=1);
来源：http://mpo.zhijiandao.cn

[U45] PHP：类型声明与返回类型
来源：http://tbr.hcnkem.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://cdr.dianchejie.cn

[U46] PHP：可空类型
来源：http://czj.tarul.cn

?string $name = null
来源：http://gpi.mhx1999.top

[U47] PHP：联合类型
来源：http://drh.havefunace.top

int|string $id
来源：http://qmy.uphjek.com

[U48] PHP：纯枚举
来源：http://rus.jinqigfzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sei.zhijiandao.cn

[U49] PHP：只读属性
来源：http://dph.shangyingyoupin.top

public readonly string $name
来源：http://lvz.guowangkeji.top

[U50] PHP：构造器属性提升
来源：http://xlg.gotoacloud.top

public function __construct(private int $id) {}
来源：http://lrr.iojbl.cn

[U51] PHP：数组解构
来源：http://jrd.jiagoushi.top

[$a, $b] = $arr;
来源：http://mwk.xingfuxueyuan.xyz

[U52] PHP：箭头函数
来源：http://ivc.xziqi.cn

$double = fn($x) => $x * 2;
来源：http://agc.bjfxy.top

[U53] PHP：空合并运算符
来源：http://uat.yueranfly.top

$v = $a ?? $b ?? "default";
来源：http://qus.0kj1m.cn

[U54] PHP：空安全调用
来源：http://ult.cdnleiting.top

$obj?->method()
来源：http://fvs.yj20258888.top

[U55] PHP：match 表达式
来源：http://ssh.hywenlv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xjb.hnqzz.top

[U56] PHP：命名参数
来源：http://gxb.nanxuanxn.top

f(a: 1, b: 2)
来源：http://hne.ehwqpu.com

[U57] PHP：字符串插值
来源：http://uip.chenzaomai.com

"值: {$a}"
来源：http://lla.chenlongwang.top

[U58] PHP：数组三件套
来源：http://lcb.xinyue.icu

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kah.hongshengwenyu.top

[U59] PHP：自定义排序
来源：http://cbf.ctjpmb.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ftp.birdmap.top

[U60] PHP：JSON 编解码
来源：http://hfs.jiagoushi.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ths.jyoumei.cn

[U61] PHP：正则
来源：http://qto.nanxuanxn.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kme.smart0.xyz

[U62] PHP：日期对象
来源：http://gdw.316326.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pfn.cheryme.top

[U63] PHP：文件读写
来源：http://aqf.gzhubu.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hcb.c1oappe.top

[U64] PHP：目录遍历
来源：http://ioa.meibo888.top

glob("dir/*.php");  scandir("dir");
来源：http://xyl.nanxinkj.top

[U65] PHP：会话
来源：http://bqj.yangfankeji.com

session_start();  $_SESSION["uid"] = 1;
来源：http://mhm.9152youxi.cn

[U66] PHP：设置 Cookie
来源：http://cfo.cucudq.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rtf.yfazqb.com

[U67] PHP：处理文件上传
来源：http://crh.gotoacloud.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hya.bbcook.cn

[U68] PHP：PDO 连接
来源：http://sul.fktsv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vbm.gogol.net.cn

[U69] PHP：PDO 预处理
来源：http://sxu.guannengcc.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mwi.tanke756.top

[U70] PHP：PDO 事务
来源：http://nvk.zdbjq.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rfr.guannengcc.top

[U71] PHP：抛出异常
来源：http://wel.hammf.cn

throw new RuntimeException("失败", 500);
来源：http://okc.yueranfly.top

[U72] PHP：写错误日志
来源：http://vzd.nwbrower.top

error_log("失败: " . $e->getMessage());
来源：http://btq.bbcook.cn

[U73] PHP：读取 ini 配置
来源：http://iun.fzhhl.top

parse_ini_file("config.ini", true)
来源：http://ztf.0kj1m.cn

[U74] PHP：读取环境变量
来源：http://ngv.redwolf501.top

getenv("APP_ENV") ?: "production"
来源：http://aeh.cashguo.top

[U75] PHP：依赖注入
来源：http://bsd.sweek.top

composer require psr/container
来源：http://nub.hfpthk.cn

[U76] PHP：简单路由
来源：http://gyx.jinghuilouyu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yks.jinghuilouyu.cn

[U77] PHP：模板渲染
来源：http://bym.zhiwuduotai.top

composer require twig/twig
来源：http://thq.mhx1999.top

[U78] PHP：单元测试
来源：http://yue.sxryk.cn

composer require --dev phpunit/phpunit
来源：http://nup.iojbl.cn

[U79] PHP：静态分析
来源：http://flz.hnqzz.top

composer require --dev phpstan/phpstan
来源：http://zir.yfazqb.com

[U80] PHP：代码规范修复
来源：http://hkn.zdqjudy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://uyp.yj202588.top

[U81] JS：初始化项目
来源：http://wwz.yuxming.cn

npm init -y;  npm i express
来源：http://ess.tianlin.xyz

[U82] JS：package.json 脚本
来源：http://uwi.zhongyouzk.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cgz.snrcjt.cn

[U83] JS：ES Module 导入导出
来源：http://upb.dashuyun.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yyy.nanxuanxn.top

[U84] JS：CommonJS 写法
来源：http://mer.mhx1999.top

module.exports = { a };  const { a } = require("./m");
来源：http://gbk.chenjidiqi.icu

[U85] JS：可选链
来源：http://leb.fzhhl.top

a?.b?.c
来源：http://dxy.zhaomingkeji.xyz

[U86] JS：空值合并
来源：http://xmp.jianghu66.top

a ?? b
来源：http://taf.zhoulong.xyz

[U87] JS：解构默认值
来源：http://ktx.zhaomingkeji.xyz

const { a = 1, b = 2 } = obj;
来源：http://pyg.jinghuilouyu.cn

[U88] JS：对象展开合并
来源：http://mmd.cashguo.top

{ ...a, ...b }
来源：http://gfa.meibo888.top

[U89] JS：数组去重
来源：http://eye.shzxlz.cn

[...new Set(arr)]
来源：http://spo.wangdashe.top

[U90] JS：数字数组排序
来源：http://ets.nwbrower.top

[...arr].sort((a, b) => a - b)
来源：http://iwc.xziqi.cn

[U91] JS：对象键值遍历
来源：http://ovy.shanyushiyangtech.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hve.fktsv.cn

[U92] JS：深拷贝
来源：http://qey.sjlbkw.cn

structuredClone(obj)
来源：http://ijq.haohaochexian.top

[U93] JS：模板字符串
来源：http://ukw.dashuyun.cn

`共 ${n} 条`
来源：http://sik.shzxlz.cn

[U94] JS：箭头函数
来源：http://fav.9152youxi.cn

const double = x => x * 2;
来源：http://ahg.aibaodan.cn

[U95] JS：Promise 包装
来源：http://ueh.kuanghao11.cn

new Promise((resolve, reject) => {})
来源：http://rlx.sxryk.cn

[U96] JS：async/await 与异常
来源：http://mnd.bbcook.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cgp.tian-w.cn

[U97] JS：并发请求
来源：http://xsm.nanxuanxn.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://grd.meibo888.top

[U98] JS：fetch 带 JSON
来源：http://dse.xziqi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hph.vehdjk.com

[U99] JS：事件监听
来源：http://cxm.gogol.net.cn

el.addEventListener("click", e => {})
来源：http://wgw.vqdsnc.cn

[U100] JS：DOM 查询
来源：http://cwh.wangdashe.top

document.querySelector(".item")
来源：http://cmg.jiagoushi.top

[U101] JS：classList 操作
来源：http://dey.havefunace.top

el.classList.toggle("active")
来源：http://uyo.xziqi.cn

[U102] JS：本地存储
来源：http://isk.zhijiandao.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ebx.xinyue.icu

[U103] JS：定时器
来源：http://tum.zhijiandao.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://syp.jianghu66.top

[U104] JS：防抖
来源：http://mrx.ppjwa.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hfe.hnqzz.top

[U105] JS：节流
来源：http://ebk.shanyushiyangkeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cel.jiagoushi.top

[U106] JS：日期格式化
来源：http://phe.tarul.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pgc.jinqigfzy.top

[U107] JS：数字千分位
来源：http://ier.vqdsnc.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://izs.sufxvd.cn

[U108] JS：随机整数
来源：http://ssm.shuidangran.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://try.ywan-chungtsiang.top

[U109] JS：数组分组
来源：http://cam.vehdjk.com

Object.groupBy(arr, x => x.type)
来源：http://max.fanxiaobao.xyz

[U110] JS：数组分块
来源：http://sok.vqdsnc.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cpy.aizwys.cn

[U111] JS：对象转 Map
来源：http://uks.sweek.top

new Map(Object.entries(obj))
来源：http://xsf.yuxming.cn

[U112] JS：字符串补位
来源：http://zgp.yuxming.cn

"7".padStart(3, "0")
来源：http://kgn.aibaodan.cn

[U113] JS：正则替换全部
来源：http://ytc.jqgufenzy.top

s.replaceAll("a", "b")
来源：http://xkk.jiagoushi.top

[U114] JS：JSON 深比较
来源：http://xep.vehdjk.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://aml.guannengcc.top

[U115] JS：生成 UUID
来源：http://cjj.fanxiaobao.xyz

crypto.randomUUID()
来源：http://mol.epnwcf.com

[U116] JS：类型检查（JSDoc）
来源：http://wca.jinqigufen.top

/** @param {string} name */ function f(name) {}
来源：http://lyd.shanyushiyangkeji.top

[U117] JS：单元测试
来源：http://jpp.yanxiufei.cn

npm i -D vitest;  npx vitest
来源：http://obo.xylfe.cn

[U118] JS：开发服务器
来源：http://ori.nanxinkj.top

npm i -D vite;  npx vite
来源：http://cgw.meibo888.top

[U119] JS：生产构建
来源：http://mqd.sjlbkw.cn

npx vite build
来源：http://jtw.yangfankeji.com

[U120] JS：读取环境变量（Vite）
来源：http://wbt.shzxlz.cn

import.meta.env.VITE_API_URL
来源：http://ovf.yanxiufei.cn

================================================================================
来源：http://mvn.gotoacloud.top

统计汇总
来源：http://cwy.aizwys.cn

================================================================================
来源：http://jve.iojbl.cn

按语言统计（条）：
来源：http://itg.zhengqikj.top

Python ......... 252
来源：http://kqv.ywan-chungtsiang.top

PHP ............ 252
来源：http://eio.snrcjt.cn

JavaScript ..... 252
来源：http://kjg.jlsjyb.cn

TypeScript ..... 212
来源：http://afb.redwolf501.top

Java ........... 212
来源：http://qrl.xinyue.icu

Go ............. 212
来源：http://yir.hongshengwenyu.top

Ruby ........... 212
来源：http://dtz.gogol.net.cn

C# ............. 212
来源：http://jms.jinyuanbaomall.cn

C .............. 30
来源：http://kth.shangyingyoupin.top

C++ ............ 30
来源：http://zcr.bjfxy.top

SQL ............ 90
来源：http://udq.sweek.top

Bash ........... 80
来源：http://vbb.guannengcc.top

Kotlin ......... 15
来源：http://emw.chenjidiqi.icu

Swift .......... 15
来源：http://lqj.jinghuilouyu.cn

Lua ............ 10
来源：http://rax.snrcjt.cn

Perl ........... 10
来源：http://clx.xinyue.icu

Scala .......... 10
来源：http://usx.shanyushiyangkeji.top

------------------------------------
来源：http://qqk.jlsjyb.cn

合计 ........... 2106 条
来源：http://xzm.yangfankeji.com

按章节统计：
来源：http://bzo.yonumen.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://frk.ehwqpu.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://aen.andypj.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vpf.ppjwa.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cqb.shanyushiyangtech.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nja.gogol.net.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lhd.ctjpmb.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jvs.xingfuxueyuan.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lyc.ywan-chungtsiang.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cfd.yfazqb.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://inl.jyoumei.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mmw.aibaodan.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xvv.zhoulong.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://euw.shzxlz.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qrt.jinghuilouyu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zsv.gotoacloud.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dsr.gogol.net.cn

Q SQL 专题                              90
来源：http://dzs.cqqwz.cn

R Bash 专题                             80
来源：http://mvv.jinqigufen.top

S C / C++ 专题                          60
来源：http://jmf.zycfv.cn

T 其他语言补充                          60
来源：http://cpa.yuanzhike.top

U 高频实用片段                         120
来源：http://fla.hywenlv.cn

------------------------------------
来源：http://hyw.52xcode.cn

合计                                  2106 条
来源：http://xrs.hcnkem.com

--------------------------------------------------------------------------------
来源：http://ueq.jlsjyb.cn

使用提醒
来源：http://ssz.shuidangran.top

--------------------------------------------------------------------------------
来源：http://wni.yongpay.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wib.zhoulong.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://psz.hnxiangtu.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rfy.xylfe.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://nzx.zycfv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://koh.tarul.cn

—— 文件结束 ——
来源：http://mtf.dianchejie.cn

================================================================================
来源：http://sgx.yueranfly.top

程序语言常见例子速查手册（2024 版）
来源：http://ybf.zhaomingkeji.xyz

Common Programming Examples Cheat Book
来源：http://ezp.wangdashe.top

================================================================================
来源：http://bzc.daxiang520.top

【收录内容】
来源：http://uoy.fehbvm.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://zpo.fktsv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kbk.hongshengwenyu.top

SQL · Bash · C · C++
来源：http://swm.ivvv.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://lxr.aibaodan.cn

【使用说明】
来源：http://ekb.aibaodan.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lxl.jinyuanbaomall.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://veo.yvedp.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kms.yonumen.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://oap.vehdjk.com

Bash:  Shell         C:     C             C++:   C++
来源：http://faa.yvedp.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zpv.gzhubu.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hsx.yueranfly.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hok.bbcook.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rpn.ybcxt.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cba.316326.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rga.birdmap.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vhl.52xcode.cn

【文件统计】
来源：http://pty.jiagoushi.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jkk.ivvv.top

--------------------------------------------------------------------------------
来源：http://zbk.nanxuanxn.top

目  录
来源：http://rkx.mhx1999.top

--------------------------------------------------------------------------------
来源：http://wxq.fzhhl.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yqo.cucudq.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mcx.vqdsnc.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uao.yongpay.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://sal.cashguo.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://exf.xuetiantiany.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tac.nwbrower.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vlw.jinghuilouyu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://aus.epnwcf.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ass.sufxvd.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rzj.jinyuanbaomall.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ijf.hcnkem.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bva.pengpengdd.cyou

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lzx.cheryme.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://amm.snrcjt.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rfa.nwbrower.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gmj.xziqi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://abw.guannengcc.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://bsd.yvedp.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ktz.316326.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ltw.ppjwa.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qwq.hywenlv.cn

================================================================================
来源：http://ovq.ivvv.top

A. 基础语法与类型
来源：http://ukr.chenzaomai.com

================================================================================
来源：http://rle.shangyingyoupin.top

[A01] Hello World
来源：http://pnc.xziqi.cn

Py:   print("Hello, World!")
来源：http://nzo.wangdashe.top

PHP:  echo "Hello, World!";
来源：http://uki.tianlin.xyz

JS:   console.log("Hello, World!");
来源：http://tgz.gzhubu.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vpd.epnwcf.com


<!-- 参考信息 -->