代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://gfu.meibo888.top

@contextlib.contextmanager
来源：http://nla.sxryk.cn

[U22] Py：矩阵转置
来源：http://lti.tian-w.cn

list(zip(*m))
来源：http://fbq.daria6918.cn

[U23] Py：分块读取大文件
来源：http://ddb.fktsv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qki.gaohongyu789.top

[U24] Py：路径操作
来源：http://qnl.zycfv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qfy.birdmap.top

[U25] Py：CSV 按字典读
来源：http://uru.hesvh.cn

csv.DictReader(f)
来源：http://feh.jinyuanbaomall.cn

[U26] Py：并发下载
来源：http://vpt.sxryk.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bbs.jianghu66.top

[U27] Py：异步 HTTP
来源：http://nfj.xuetiantiany.cn

aiohttp.ClientSession() 配合 async with
来源：http://wss.fengsongda.top

[U28] Py：类型别名
来源：http://vpg.bjfxy.top

UserId = int
来源：http://gto.chenlongwang.top

[U29] Py：属性校验
来源：http://elm.bjfxy.top

@property 与 @x.setter 配合
来源：http://cij.xinyue.icu

[U30] Py：数据类
来源：http://boo.hongshengwenyu.top

@dataclass(slots=True)
来源：http://xhr.nanxuanxn.top

[U31] Py：单测
来源：http://peq.jinghuilouyu.cn

python -m pytest -q
来源：http://aay.tanke756.top

[U32] Py：代码格式化
来源：http://plz.gogol.net.cn

ruff format . && ruff check --fix .
来源：http://hqh.quarkkingdee.top

[U33] Py：打包发布
来源：http://ehq.quarkkingdee.top

python -m build  （依赖 pyproject.toml）
来源：http://czq.yangfankeji.com

[U34] Py：判断编码
来源：http://trj.cashguo.top

chardet.detect(raw)
来源：http://gbz.birdmap.top

[U35] Py：发送邮件
来源：http://nya.zycfv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vst.smart0.xyz

[U36] Py：定时任务
来源：http://voz.yueranfly.top

schedule.every(10).minutes.do(job)
来源：http://sxq.sysykeji.top

[U37] Py：读写 Excel
来源：http://kfm.cdnleiting.top

pandas.read_excel / DataFrame.to_excel
来源：http://zzg.yonumen.top

[U38] Py：获取脚本所在目录
来源：http://jtm.bjfxy.top

Path(__file__).resolve().parent
来源：http://clw.yanxiufei.cn

[U39] Py：判断是否在交互环境
来源：http://cpf.snrcjt.cn

sys.stdout.isatty()
来源：http://ydq.feifeiyinyue.top

[U40] Py：打印到标准错误
来源：http://vhc.fktsv.cn

print("err", file=sys.stderr)
来源：http://cvn.feifeiyinyue.top

[U41] PHP：初始化 Composer 项目
来源：http://ewn.zdqjudy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://htz.wangdashe.top

[U42] PHP：PSR-4 自动加载
来源：http://epg.ybcxt.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fwv.kuanghao11.cn

[U43] PHP：声明命名空间
来源：http://wqp.hysaishi.cn

namespace App\Http;
来源：http://ckm.yanxiufei.cn

[U44] PHP：开启严格类型
来源：http://kpr.pengpengdd.cyou

declare(strict_types=1);
来源：http://gxg.birdmap.top

[U45] PHP：类型声明与返回类型
来源：http://joh.nwbrower.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://vxz.52xcode.cn

[U46] PHP：可空类型
来源：http://stn.hammf.cn

?string $name = null
来源：http://ggr.zycfv.cn

[U47] PHP：联合类型
来源：http://xnv.shanyushiyangkeji.top

int|string $id
来源：http://cdg.sjlbkw.cn

[U48] PHP：纯枚举
来源：http://aen.ctjpmb.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hcc.zhijiandao.cn

[U49] PHP：只读属性
来源：http://ktk.316326.xyz

public readonly string $name
来源：http://fop.ehwqpu.com

[U50] PHP：构造器属性提升
来源：http://mve.fengsongda.top

public function __construct(private int $id) {}
来源：http://awg.redwolf501.top

[U51] PHP：数组解构
来源：http://lkw.cheryme.top

[$a, $b] = $arr;
来源：http://ikt.pengpengdd.cyou

[U52] PHP：箭头函数
来源：http://vpz.daxiang520.top

$double = fn($x) => $x * 2;
来源：http://vzt.zhaomingkeji.xyz

[U53] PHP：空合并运算符
来源：http://tfz.feifeiyinyue.top

$v = $a ?? $b ?? "default";
来源：http://wbj.sxryk.cn

[U54] PHP：空安全调用
来源：http://ezy.yj20258.top

$obj?->method()
来源：http://rfs.jlsjyb.cn

[U55] PHP：match 表达式
来源：http://rep.dianchejie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pnh.cashguo.top

[U56] PHP：命名参数
来源：http://jqa.xingfuxueyuan.xyz

f(a: 1, b: 2)
来源：http://plh.0kj1m.cn

[U57] PHP：字符串插值
来源：http://owm.gaohongyu789.top

"值: {$a}"
来源：http://utw.shuidangran.top

[U58] PHP：数组三件套
来源：http://jtm.yj202588.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xyl.zhaomingkeji.xyz

[U59] PHP：自定义排序
来源：http://oyj.yueranfly.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pow.redwolf501.top

[U60] PHP：JSON 编解码
来源：http://aql.jinqigufen.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fnu.fktsv.cn

[U61] PHP：正则
来源：http://cxt.guannengcc.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jml.yfazqb.com

[U62] PHP：日期对象
来源：http://gnl.zhiwuduotai.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sne.yj202588.top

[U63] PHP：文件读写
来源：http://pmn.yongpay.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zie.gaohongyu789.top

[U64] PHP：目录遍历
来源：http://skg.zdbjq.cn

glob("dir/*.php");  scandir("dir");
来源：http://ign.zhoulong.xyz

[U65] PHP：会话
来源：http://adm.yj20258.top

session_start();  $_SESSION["uid"] = 1;
来源：http://jjs.jlsjyb.cn

[U66] PHP：设置 Cookie
来源：http://nvq.ydzc1.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dmo.9152youxi.cn

[U67] PHP：处理文件上传
来源：http://jju.nanxuanxn.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rvv.aizwys.cn

[U68] PHP：PDO 连接
来源：http://szi.hongshengwenyu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://oum.jinghuilouyu.cn

[U69] PHP：PDO 预处理
来源：http://acb.hnxiangtu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dqk.jiagoushi.top

[U70] PHP：PDO 事务
来源：http://itz.shangyingyoupin.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yhw.zhoulong.xyz

[U71] PHP：抛出异常
来源：http://xqu.ybcxt.top

throw new RuntimeException("失败", 500);
来源：http://nrw.yfazqb.com

[U72] PHP：写错误日志
来源：http://bkf.0kj1m.cn

error_log("失败: " . $e->getMessage());
来源：http://any.ydjk.org.cn

[U73] PHP：读取 ini 配置
来源：http://ahp.yvedp.cn

parse_ini_file("config.ini", true)
来源：http://trk.hnxiangtu.top

[U74] PHP：读取环境变量
来源：http://tmc.sxryk.cn

getenv("APP_ENV") ?: "production"
来源：http://oqh.quarkkingdee.top

[U75] PHP：依赖注入
来源：http://tju.dashuyun.cn

composer require psr/container
来源：http://nuk.jiagoushi.top

[U76] PHP：简单路由
来源：http://sdx.sufxvd.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rnk.cheryme.top

[U77] PHP：模板渲染
来源：http://lix.hfpthk.cn

composer require twig/twig
来源：http://cbr.bbcook.cn

[U78] PHP：单元测试
来源：http://buq.hfpthk.cn

composer require --dev phpunit/phpunit
来源：http://ewj.uphjek.com

[U79] PHP：静态分析
来源：http://bbx.xingfuxueyuan.xyz

composer require --dev phpstan/phpstan
来源：http://yme.yongpay.top

[U80] PHP：代码规范修复
来源：http://fbf.redwolf501.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://xpn.sxryk.cn

[U81] JS：初始化项目
来源：http://nbc.svipenyu.cn

npm init -y;  npm i express
来源：http://efm.yuxming.cn

[U82] JS：package.json 脚本
来源：http://vew.ywan-chungtsiang.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hjx.havefunace.top

[U83] JS：ES Module 导入导出
来源：http://pap.yanxiufei.cn

export const a = 1;  import { a } from "./m.js";
来源：http://iji.hfpthk.cn

[U84] JS：CommonJS 写法
来源：http://pqs.snrcjt.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wwl.ppjwa.cn

[U85] JS：可选链
来源：http://ase.xuanzx.com

a?.b?.c
来源：http://iun.dashuyun.cn

[U86] JS：空值合并
来源：http://lgm.tian-w.cn

a ?? b
来源：http://zkv.vehdjk.com

[U87] JS：解构默认值
来源：http://bwt.xuetiantiany.cn

const { a = 1, b = 2 } = obj;
来源：http://xll.iojbl.cn

[U88] JS：对象展开合并
来源：http://cgj.zhijiandao.cn

{ ...a, ...b }
来源：http://aej.sufxvd.cn

[U89] JS：数组去重
来源：http://lwf.jinghuilouyu.cn

[...new Set(arr)]
来源：http://jmi.shanyushiyangtech.top

[U90] JS：数字数组排序
来源：http://yth.shzxlz.cn

[...arr].sort((a, b) => a - b)
来源：http://zcd.shanyushiyangkeji.top

[U91] JS：对象键值遍历
来源：http://jim.sweek.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rqe.yanxiufei.cn

[U92] JS：深拷贝
来源：http://igq.epnwcf.com

structuredClone(obj)
来源：http://udl.ywan-chungtsiang.top

[U93] JS：模板字符串
来源：http://jsf.gaohongyu789.top

`共 ${n} 条`
来源：http://xab.sufxvd.cn

[U94] JS：箭头函数
来源：http://xhd.hysaishi.cn

const double = x => x * 2;
来源：http://wfl.ehwqpu.com

[U95] JS：Promise 包装
来源：http://knq.shanyushiyangkeji.top

new Promise((resolve, reject) => {})
来源：http://tog.yanxiufei.cn

[U96] JS：async/await 与异常
来源：http://kjx.daxiang520.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oyf.andypj.xyz

[U97] JS：并发请求
来源：http://ygb.bjfxy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ity.zhongyouzk.top

[U98] JS：fetch 带 JSON
来源：http://lol.kuanghao11.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lvf.jinqigfzy.top

[U99] JS：事件监听
来源：http://kee.tarul.cn

el.addEventListener("click", e => {})
来源：http://ofd.guannengcc.top

[U100] JS：DOM 查询
来源：http://tse.jyoumei.cn

document.querySelector(".item")
来源：http://wxd.cqqwz.cn

[U101] JS：classList 操作
来源：http://dxk.nanxinkj.top

el.classList.toggle("active")
来源：http://xxg.fehbvm.com

[U102] JS：本地存储
来源：http://mpd.shanyushiyangtech.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hem.fanxiaobao.xyz

[U103] JS：定时器
来源：http://eyv.yueranfly.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jjm.meibo888.top

[U104] JS：防抖
来源：http://dir.fanxiaobao.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eum.sxryk.cn

[U105] JS：节流
来源：http://acr.jianghu66.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xdv.ydjk.org.cn

[U106] JS：日期格式化
来源：http://qsl.shuidangran.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bxu.yangfankeji.com

[U107] JS：数字千分位
来源：http://gbe.hnxiangtu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tyu.yuanzhike.top

[U108] JS：随机整数
来源：http://zfv.shangyingyoupin.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://eow.bbcook.cn

[U109] JS：数组分组
来源：http://pzr.yj20258888.top

Object.groupBy(arr, x => x.type)
来源：http://hir.nwbrower.top

[U110] JS：数组分块
来源：http://rxz.hesvh.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uwh.gaohongyu789.top

[U111] JS：对象转 Map
来源：http://eqr.ehwqpu.com

new Map(Object.entries(obj))
来源：http://slk.gaohongyu789.top

[U112] JS：字符串补位
来源：http://voy.fzhhl.top

"7".padStart(3, "0")
来源：http://ndc.tianlin.xyz

[U113] JS：正则替换全部
来源：http://zym.ctjpmb.com

s.replaceAll("a", "b")
来源：http://wsj.epnwcf.com

[U114] JS：JSON 深比较
来源：http://lnr.pengpengdd.cyou

JSON.stringify(a) === JSON.stringify(b)
来源：http://xba.sufxvd.cn

[U115] JS：生成 UUID
来源：http://cuo.yvedp.cn

crypto.randomUUID()
来源：http://pld.birdmap.top

[U116] JS：类型检查（JSDoc）
来源：http://ytn.shangyingyoupin.top

/** @param {string} name */ function f(name) {}
来源：http://peh.ydjk.org.cn

[U117] JS：单元测试
来源：http://qnv.dashuyun.cn

npm i -D vitest;  npx vitest
来源：http://yvm.hongshengwenyu.top

[U118] JS：开发服务器
来源：http://vtt.zhoulong.xyz

npm i -D vite;  npx vite
来源：http://xik.cqqwz.cn

[U119] JS：生产构建
来源：http://iuv.kuanghao11.cn

npx vite build
来源：http://rag.c1oappe.top

[U120] JS：读取环境变量（Vite）
来源：http://kip.zhiwuduotai.top

import.meta.env.VITE_API_URL
来源：http://wov.vqdsnc.cn

================================================================================
来源：http://nbq.mhx1999.top

统计汇总
来源：http://mhx.ivvv.top

================================================================================
来源：http://qki.hesvh.cn

按语言统计（条）：
来源：http://ebn.jianghu66.top

Python ......... 252
来源：http://iln.yj202588.top

PHP ............ 252
来源：http://pze.xylfe.cn

JavaScript ..... 252
来源：http://gty.gotoacloud.top

TypeScript ..... 212
来源：http://rki.aizwys.cn

Java ........... 212
来源：http://epe.fengsongda.top

Go ............. 212
来源：http://kjv.nwbrower.top

Ruby ........... 212
来源：http://nov.feifeiyinyue.top

C# ............. 212
来源：http://wlj.vehdjk.com

C .............. 30
来源：http://giq.nanxuanxn.top

C++ ............ 30
来源：http://lal.quarkkingdee.top

SQL ............ 90
来源：http://vxq.hywenlv.cn

Bash ........... 80
来源：http://soo.tarul.cn

Kotlin ......... 15
来源：http://mmm.hammf.cn

Swift .......... 15
来源：http://cam.vqdsnc.cn

Lua ............ 10
来源：http://vni.9152youxi.cn

Perl ........... 10
来源：http://ikh.hnqzz.top

Scala .......... 10
来源：http://spz.uphjek.com

------------------------------------
来源：http://sjk.ywan-chungtsiang.top

合计 ........... 2106 条
来源：http://zwv.pycfn.com

按章节统计：
来源：http://rbv.jinqigufen.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kdy.yj20258.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://awk.yfazqb.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vqh.daria6918.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hhu.yfazqb.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yob.feifeiyinyue.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bct.ctjpmb.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wec.chenlongwang.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://owo.yuxming.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jol.fanxiaobao.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hwd.snrcjt.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rqf.zhengqikj.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fqd.316326.xyz

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blj.ywan-chungtsiang.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://aaq.ywan-chungtsiang.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rap.ydjk.org.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ess.fzhhl.top

Q SQL 专题                              90
来源：http://bcs.xuetiantiany.cn

R Bash 专题                             80
来源：http://qss.vqdsnc.cn

S C / C++ 专题                          60
来源：http://zau.jqgufenzy.top

T 其他语言补充                          60
来源：http://rzs.sufxvd.cn

U 高频实用片段                         120
来源：http://vyg.feifeiyinyue.top

------------------------------------
来源：http://dqr.yueranfly.top

合计                                  2106 条
来源：http://uux.ppjwa.cn

--------------------------------------------------------------------------------
来源：http://who.sxryk.cn

使用提醒
来源：http://pxi.c1oappe.top

--------------------------------------------------------------------------------
来源：http://wxf.9152youxi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://put.c1oappe.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wmg.jinghuilouyu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://msx.yueranfly.top

在旧版本上使用前请先确认语法支持情况。
来源：http://zrw.chenjidiqi.icu

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zmg.sweek.top

—— 文件结束 ——
来源：http://res.dashuyun.cn

================================================================================
来源：http://lms.yj202588.top

程序语言常见例子速查手册（2024 版）
来源：http://vtq.yvedp.cn

Common Programming Examples Cheat Book
来源：http://gkp.c1oappe.top

================================================================================
来源：http://qrf.uphjek.com

【收录内容】
来源：http://buz.wangdashe.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://dtd.fanxiaobao.xyz

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://khn.quarkkingdee.top

SQL · Bash · C · C++
来源：http://vzp.jinqigufen.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mjw.zhixingplan.top

【使用说明】
来源：http://ejt.ehwqpu.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qjy.zhongyouzk.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pfa.ppjwa.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zux.jyoumei.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gil.cdnleiting.top

Bash:  Shell         C:     C             C++:   C++
来源：http://anf.chenlongwang.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://scd.quarkkingdee.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://njh.gogol.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jzj.hongshengwenyu.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://slo.chenzaomai.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tqp.hfpthk.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://chz.zhoulong.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://may.yfazqb.com

【文件统计】
来源：http://bpq.hnxiangtu.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://poh.guowangkeji.top

--------------------------------------------------------------------------------
来源：http://ymt.andypj.xyz

目  录
来源：http://jfi.ivvv.top

--------------------------------------------------------------------------------
来源：http://asq.hywenlv.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mxo.sweek.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://swx.sjlbkw.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ift.yvedp.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hwe.xingfuxueyuan.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yzp.zhoulong.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ied.xuanzx.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uuf.hnxiangtu.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gof.9152youxi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bxy.nwbrower.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://psy.zhoulong.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kay.vehdjk.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bqo.wangshuangyany.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ggu.cucudq.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hqg.aibaodan.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fag.sufxvd.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sjf.shuidangran.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fzm.fanxiaobao.xyz


<!-- 参考信息 -->