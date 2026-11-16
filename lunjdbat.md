代发 wailian999

[U25] Py：CSV 按字典读
来源：http://vng.cashguo.top

csv.DictReader(f)
来源：http://pmb.gogol.net.cn

[U26] Py：并发下载
来源：http://ezx.52xcode.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hfq.hammf.cn

[U27] Py：异步 HTTP
来源：http://dvf.chenzaomai.com

aiohttp.ClientSession() 配合 async with
来源：http://jgh.hesvh.cn

[U28] Py：类型别名
来源：http://wjd.sxryk.cn

UserId = int
来源：http://dbv.hnqzz.top

[U29] Py：属性校验
来源：http://dvg.pengpengdd.cyou

@property 与 @x.setter 配合
来源：http://yim.epnwcf.com

[U30] Py：数据类
来源：http://hfl.nanxuanxn.top

@dataclass(slots=True)
来源：http://jsh.sweek.top

[U31] Py：单测
来源：http://spq.uphjek.com

python -m pytest -q
来源：http://srn.guowangkeji.top

[U32] Py：代码格式化
来源：http://rgs.tianlin.xyz

ruff format . && ruff check --fix .
来源：http://fjd.jianghu66.top

[U33] Py：打包发布
来源：http://lfz.zhaomingkeji.xyz

python -m build  （依赖 pyproject.toml）
来源：http://xrf.ppjwa.cn

[U34] Py：判断编码
来源：http://mmt.jinghuilouyu.cn

chardet.detect(raw)
来源：http://wet.birdmap.top

[U35] Py：发送邮件
来源：http://xvi.chenzaomai.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mie.zhongyouzk.top

[U36] Py：定时任务
来源：http://ztt.jinqigufen.top

schedule.every(10).minutes.do(job)
来源：http://fbm.feifeiyinyue.top

[U37] Py：读写 Excel
来源：http://awz.shanyushiyangtech.top

pandas.read_excel / DataFrame.to_excel
来源：http://vwz.bbcook.cn

[U38] Py：获取脚本所在目录
来源：http://lny.sjlbkw.cn

Path(__file__).resolve().parent
来源：http://dcf.bbcook.cn

[U39] Py：判断是否在交互环境
来源：http://igo.zdbjq.cn

sys.stdout.isatty()
来源：http://pcm.xylfe.cn

[U40] Py：打印到标准错误
来源：http://uvj.yonumen.top

print("err", file=sys.stderr)
来源：http://tpt.hongshengwenyu.top

[U41] PHP：初始化 Composer 项目
来源：http://rsd.jiagoushi.top

composer init;  composer require guzzlehttp/guzzle
来源：http://rxc.zhixingplan.top

[U42] PHP：PSR-4 自动加载
来源：http://wld.uphjek.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bug.9152youxi.cn

[U43] PHP：声明命名空间
来源：http://tpq.zycfv.cn

namespace App\Http;
来源：http://uoa.shuidangran.top

[U44] PHP：开启严格类型
来源：http://akm.zycfv.cn

declare(strict_types=1);
来源：http://aeg.redwolf501.top

[U45] PHP：类型声明与返回类型
来源：http://qmt.xziqi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://joi.yuanzhike.top

[U46] PHP：可空类型
来源：http://rkx.feifeiyinyue.top

?string $name = null
来源：http://whk.jinqigufen.top

[U47] PHP：联合类型
来源：http://lsk.snrcjt.cn

int|string $id
来源：http://hgn.yonumen.top

[U48] PHP：纯枚举
来源：http://cnn.hcnkem.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ofo.hfpthk.cn

[U49] PHP：只读属性
来源：http://qzv.shuidangran.top

public readonly string $name
来源：http://cwi.fanxiaobao.xyz

[U50] PHP：构造器属性提升
来源：http://ebc.guowangkeji.top

public function __construct(private int $id) {}
来源：http://nld.redwolf501.top

[U51] PHP：数组解构
来源：http://dme.haohaochexian.top

[$a, $b] = $arr;
来源：http://qiv.tian-w.cn

[U52] PHP：箭头函数
来源：http://snl.hesvh.cn

$double = fn($x) => $x * 2;
来源：http://ykj.redwolf501.top

[U53] PHP：空合并运算符
来源：http://qat.yuanzhike.top

$v = $a ?? $b ?? "default";
来源：http://kdg.xylfe.cn

[U54] PHP：空安全调用
来源：http://opo.hcnkem.com

$obj?->method()
来源：http://rdl.fengsongda.top

[U55] PHP：match 表达式
来源：http://eri.ivvv.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fxp.jyoumei.cn

[U56] PHP：命名参数
来源：http://ius.zhijiandao.cn

f(a: 1, b: 2)
来源：http://xsl.cheryme.top

[U57] PHP：字符串插值
来源：http://iai.smart0.xyz

"值: {$a}"
来源：http://gtq.chenjidiqi.icu

[U58] PHP：数组三件套
来源：http://vxm.tian-w.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://iqb.cucudq.cn

[U59] PHP：自定义排序
来源：http://wtw.yueranfly.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uom.ywan-chungtsiang.top

[U60] PHP：JSON 编解码
来源：http://qgc.zhijiandao.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ssq.zdqjudy.top

[U61] PHP：正则
来源：http://ocw.bbcook.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kwd.vehdjk.com

[U62] PHP：日期对象
来源：http://pry.pycfn.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jtt.shanyushiyangtech.top

[U63] PHP：文件读写
来源：http://xpo.jinqigfzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sgm.jyoumei.cn

[U64] PHP：目录遍历
来源：http://vgs.c1oappe.top

glob("dir/*.php");  scandir("dir");
来源：http://ptr.zhoulong.xyz

[U65] PHP：会话
来源：http://rnm.sufxvd.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ypu.gotoacloud.top

[U66] PHP：设置 Cookie
来源：http://czv.xuanzx.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dcj.tian-w.cn

[U67] PHP：处理文件上传
来源：http://lqb.cheryme.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://beg.fzhhl.top

[U68] PHP：PDO 连接
来源：http://ats.jiagoushi.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://psh.wangdashe.top

[U69] PHP：PDO 预处理
来源：http://eel.yonumen.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fic.iojbl.cn

[U70] PHP：PDO 事务
来源：http://inc.zhongyouzk.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lok.pycfn.com

[U71] PHP：抛出异常
来源：http://svr.fanxiaobao.xyz

throw new RuntimeException("失败", 500);
来源：http://pjm.smart0.xyz

[U72] PHP：写错误日志
来源：http://qjf.redwolf501.top

error_log("失败: " . $e->getMessage());
来源：http://rtp.sufxvd.cn

[U73] PHP：读取 ini 配置
来源：http://wqj.ppjwa.cn

parse_ini_file("config.ini", true)
来源：http://nkl.wangdashe.top

[U74] PHP：读取环境变量
来源：http://pda.wangshuangyany.cn

getenv("APP_ENV") ?: "production"
来源：http://zbg.yangfankeji.com

[U75] PHP：依赖注入
来源：http://nkq.yangfankeji.com

composer require psr/container
来源：http://xdu.zdbjq.cn

[U76] PHP：简单路由
来源：http://qmu.cheryme.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uca.hywenlv.cn

[U77] PHP：模板渲染
来源：http://ehv.zhiwuduotai.top

composer require twig/twig
来源：http://mkq.jqgufenzy.top

[U78] PHP：单元测试
来源：http://xac.zhiwuduotai.top

composer require --dev phpunit/phpunit
来源：http://aen.wangshuangyany.cn

[U79] PHP：静态分析
来源：http://gyb.gaohongyu789.top

composer require --dev phpstan/phpstan
来源：http://kiz.daria6918.cn

[U80] PHP：代码规范修复
来源：http://uoy.wangdashe.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://igd.haohaochexian.top

[U81] JS：初始化项目
来源：http://fsy.zdqjudy.top

npm init -y;  npm i express
来源：http://zos.chenlongwang.top

[U82] JS：package.json 脚本
来源：http://cvg.sufxvd.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lol.gzhubu.top

[U83] JS：ES Module 导入导出
来源：http://rpw.jinqigufen.top

export const a = 1;  import { a } from "./m.js";
来源：http://btd.jiagoushi.top

[U84] JS：CommonJS 写法
来源：http://mry.zdbjq.cn

module.exports = { a };  const { a } = require("./m");
来源：http://cxb.meibo888.top

[U85] JS：可选链
来源：http://cfg.zhijiandao.cn

a?.b?.c
来源：http://oqj.bjfxy.top

[U86] JS：空值合并
来源：http://zwv.fanxiaobao.xyz

a ?? b
来源：http://yus.hcnkem.com

[U87] JS：解构默认值
来源：http://bvo.aibaodan.cn

const { a = 1, b = 2 } = obj;
来源：http://ghk.yangfankeji.com

[U88] JS：对象展开合并
来源：http://pzc.guannengcc.top

{ ...a, ...b }
来源：http://mdv.yj20258888.top

[U89] JS：数组去重
来源：http://afc.andypj.xyz

[...new Set(arr)]
来源：http://pjd.cqqwz.cn

[U90] JS：数字数组排序
来源：http://mgy.havefunace.top

[...arr].sort((a, b) => a - b)
来源：http://vrf.tanke756.top

[U91] JS：对象键值遍历
来源：http://ubm.hywenlv.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://uto.cqqwz.cn

[U92] JS：深拷贝
来源：http://dzx.pengpengdd.cyou

structuredClone(obj)
来源：http://wvs.gaohongyu789.top

[U93] JS：模板字符串
来源：http://zxn.fehbvm.com

`共 ${n} 条`
来源：http://lre.dianchejie.cn

[U94] JS：箭头函数
来源：http://xhe.tarul.cn

const double = x => x * 2;
来源：http://ojn.uphjek.com

[U95] JS：Promise 包装
来源：http://pis.hcnkem.com

new Promise((resolve, reject) => {})
来源：http://ogk.fanxiaobao.xyz

[U96] JS：async/await 与异常
来源：http://ocx.tanke756.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ieg.cashguo.top

[U97] JS：并发请求
来源：http://woa.xuetiantiany.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://piz.pengpengdd.cyou

[U98] JS：fetch 带 JSON
来源：http://dqi.ydjk.org.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jph.epnwcf.com

[U99] JS：事件监听
来源：http://ppq.52xcode.cn

el.addEventListener("click", e => {})
来源：http://hce.cashguo.top

[U100] JS：DOM 查询
来源：http://ycl.sysykeji.top

document.querySelector(".item")
来源：http://oar.tarul.cn

[U101] JS：classList 操作
来源：http://rqd.guannengcc.top

el.classList.toggle("active")
来源：http://gpy.snrcjt.cn

[U102] JS：本地存储
来源：http://ogc.smart0.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://vpu.ppjwa.cn

[U103] JS：定时器
来源：http://jti.cheryme.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ukc.cucudq.cn

[U104] JS：防抖
来源：http://efy.kuanghao11.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bhh.cdnleiting.top

[U105] JS：节流
来源：http://djg.316326.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gkx.zhaomingkeji.xyz

[U106] JS：日期格式化
来源：http://jxv.hammf.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pvn.52xcode.cn

[U107] JS：数字千分位
来源：http://bwy.jinyuanbaomall.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gut.yj20258888.top

[U108] JS：随机整数
来源：http://acp.zycfv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rbn.pycfn.com

[U109] JS：数组分组
来源：http://afk.smart0.xyz

Object.groupBy(arr, x => x.type)
来源：http://aaj.cqqwz.cn

[U110] JS：数组分块
来源：http://odd.chenjidiqi.icu

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mtt.aizwys.cn

[U111] JS：对象转 Map
来源：http://qmf.c1oappe.top

new Map(Object.entries(obj))
来源：http://fjq.shangyingyoupin.top

[U112] JS：字符串补位
来源：http://trr.yuanzhike.top

"7".padStart(3, "0")
来源：http://vxd.chenzaomai.com

[U113] JS：正则替换全部
来源：http://exs.yongpay.top

s.replaceAll("a", "b")
来源：http://xis.uphjek.com

[U114] JS：JSON 深比较
来源：http://uyi.xingfuxueyuan.xyz

JSON.stringify(a) === JSON.stringify(b)
来源：http://mjp.yj20258888.top

[U115] JS：生成 UUID
来源：http://tux.zhongyouzk.top

crypto.randomUUID()
来源：http://jtu.zhoulong.xyz

[U116] JS：类型检查（JSDoc）
来源：http://syk.andypj.xyz

/** @param {string} name */ function f(name) {}
来源：http://suw.jiagoushi.top

[U117] JS：单元测试
来源：http://iaz.hnxiangtu.top

npm i -D vitest;  npx vitest
来源：http://bdt.uphjek.com

[U118] JS：开发服务器
来源：http://nvq.jinqigfzy.top

npm i -D vite;  npx vite
来源：http://iqt.wangdashe.top

[U119] JS：生产构建
来源：http://ipr.haohaochexian.top

npx vite build
来源：http://jmw.havefunace.top

[U120] JS：读取环境变量（Vite）
来源：http://rsd.jinyuanbaomall.cn

import.meta.env.VITE_API_URL
来源：http://tgt.shanyushiyangtech.top

================================================================================
来源：http://wgb.fehbvm.com

统计汇总
来源：http://lea.sjlbkw.cn

================================================================================
来源：http://wmq.xuanzx.com

按语言统计（条）：
来源：http://zcx.chenjidiqi.icu

Python ......... 252
来源：http://ein.nwbrower.top

PHP ............ 252
来源：http://nuj.zhengqikj.top

JavaScript ..... 252
来源：http://nrm.daxiang520.top

TypeScript ..... 212
来源：http://odi.xziqi.cn

Java ........... 212
来源：http://kib.zhoulong.xyz

Go ............. 212
来源：http://hqp.dianchejie.cn

Ruby ........... 212
来源：http://uxu.sxryk.cn

C# ............. 212
来源：http://ujc.hnxiangtu.top

C .............. 30
来源：http://tup.xingfuxueyuan.xyz

C++ ............ 30
来源：http://scr.bjfxy.top

SQL ............ 90
来源：http://thf.zhiwuduotai.top

Bash ........... 80
来源：http://jcr.dianchejie.cn

Kotlin ......... 15
来源：http://hxy.zhiwuduotai.top

Swift .......... 15
来源：http://xlx.zhongyouzk.top

Lua ............ 10
来源：http://xod.hnxiangtu.top

Perl ........... 10
来源：http://rst.jinqigufen.top

Scala .......... 10
来源：http://gri.aibaodan.cn

------------------------------------
来源：http://nxj.iojbl.cn

合计 ........... 2106 条
来源：http://amg.zdbjq.cn

按章节统计：
来源：http://deb.bjfxy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qie.yvedp.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tvy.bjfxy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bjq.xingfuxueyuan.xyz

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xgb.0kj1m.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tel.hywenlv.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://itu.chenjidiqi.icu

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cpe.cqqwz.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://acw.bjfxy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ted.yj202588.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rzi.jyoumei.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://srz.snrcjt.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mhz.tian-w.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://klr.dashuyun.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tjm.yueranfly.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wrv.ywan-chungtsiang.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yvd.jinyuanbaomall.cn

Q SQL 专题                              90
来源：http://zzq.jqgfzy.top

R Bash 专题                             80
来源：http://qnb.bbcook.cn

S C / C++ 专题                          60
来源：http://mqc.jinyuanbaomall.cn

T 其他语言补充                          60
来源：http://akm.chenzaomai.com

U 高频实用片段                         120
来源：http://huy.hammf.cn

------------------------------------
来源：http://hkj.c1oappe.top

合计                                  2106 条
来源：http://uqp.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://hxe.jianghu66.top

使用提醒
来源：http://muq.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://umb.yongpay.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yir.bbcook.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://oxz.sweek.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mtl.jlsjyb.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vxs.sufxvd.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tis.52xcode.cn

—— 文件结束 ——
来源：http://ipe.tianlin.xyz

================================================================================
来源：http://wdw.yvedp.cn

程序语言常见例子速查手册（2024 版）
来源：http://fjz.yj20258888.top

Common Programming Examples Cheat Book
来源：http://mzi.nwbrower.top

================================================================================
来源：http://dka.svipenyu.cn

【收录内容】
来源：http://gug.zhoulong.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://sms.shanyushiyangtech.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hhg.andypj.xyz

SQL · Bash · C · C++
来源：http://vlz.redwolf501.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hvz.jiagoushi.top

【使用说明】
来源：http://lmf.wangshuangyany.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pkq.xuetiantiany.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vom.feifeiyinyue.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lmr.guannengcc.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nik.fktsv.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://cxc.bbcook.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rpm.gotoacloud.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wyq.0kj1m.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ktm.ppjwa.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tvh.ywan-chungtsiang.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://smq.316326.xyz

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dws.yongpay.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qdh.jlsjyb.cn

【文件统计】
来源：http://bvi.yuxming.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xvp.quarkkingdee.top

--------------------------------------------------------------------------------
来源：http://wql.chenzaomai.com

目  录
来源：http://wkl.yj202588.top

--------------------------------------------------------------------------------
来源：http://ylq.shzxlz.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vib.jinghuilouyu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ljd.fanxiaobao.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://szn.meibo888.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qik.epnwcf.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gli.vqdsnc.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qqu.cheryme.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hhl.ctjpmb.com

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dum.daria6918.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://toq.shanyushiyangkeji.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fjz.nanxinkj.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ngr.hfpthk.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ueq.bjfxy.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://awi.hesvh.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rwm.hnqzz.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zma.zycfv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://oct.shanyushiyangtech.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://top.nwbrower.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://jzq.zhaomingkeji.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rgg.zhongyouzk.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tbx.guannengcc.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bzn.feifeiyinyue.top

================================================================================
来源：http://qam.yfazqb.com

A. 基础语法与类型
来源：http://qmi.0kj1m.cn

================================================================================
来源：http://rof.snrcjt.cn

[A01] Hello World
来源：http://ris.ywan-chungtsiang.top


<!-- 参考信息 -->