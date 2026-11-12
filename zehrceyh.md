代发 wailian999

[U23] Py：分块读取大文件
来源：http://bgo.svipenyu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://taa.ybcxt.top

[U24] Py：路径操作
来源：http://zmc.316326.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zii.zhoulong.xyz

[U25] Py：CSV 按字典读
来源：http://wjw.pycfn.com

csv.DictReader(f)
来源：http://kke.andypj.xyz

[U26] Py：并发下载
来源：http://fhq.fanxiaobao.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cmg.kuanghao11.cn

[U27] Py：异步 HTTP
来源：http://pxp.jinqigufen.top

aiohttp.ClientSession() 配合 async with
来源：http://fbk.birdmap.top

[U28] Py：类型别名
来源：http://ywc.zhengqikj.top

UserId = int
来源：http://ewe.yongpay.top

[U29] Py：属性校验
来源：http://ruh.chenzaomai.com

@property 与 @x.setter 配合
来源：http://upr.chenzaomai.com

[U30] Py：数据类
来源：http://kku.birdmap.top

@dataclass(slots=True)
来源：http://gca.meibo888.top

[U31] Py：单测
来源：http://ipp.xylfe.cn

python -m pytest -q
来源：http://qfn.yuxming.cn

[U32] Py：代码格式化
来源：http://ziy.smart0.xyz

ruff format . && ruff check --fix .
来源：http://khz.sxryk.cn

[U33] Py：打包发布
来源：http://ruj.hnxiangtu.top

python -m build  （依赖 pyproject.toml）
来源：http://sgi.mhx1999.top

[U34] Py：判断编码
来源：http://rpi.52xcode.cn

chardet.detect(raw)
来源：http://wwb.tian-w.cn

[U35] Py：发送邮件
来源：http://sah.9152youxi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lmb.birdmap.top

[U36] Py：定时任务
来源：http://cbr.jlsjyb.cn

schedule.every(10).minutes.do(job)
来源：http://krr.52xcode.cn

[U37] Py：读写 Excel
来源：http://fbz.fktsv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://upn.meibo888.top

[U38] Py：获取脚本所在目录
来源：http://jzh.hywenlv.cn

Path(__file__).resolve().parent
来源：http://vvx.aizwys.cn

[U39] Py：判断是否在交互环境
来源：http://byz.cqqwz.cn

sys.stdout.isatty()
来源：http://dzm.tian-w.cn

[U40] Py：打印到标准错误
来源：http://lmg.vqdsnc.cn

print("err", file=sys.stderr)
来源：http://wkb.feifeiyinyue.top

[U41] PHP：初始化 Composer 项目
来源：http://hrp.fzhhl.top

composer init;  composer require guzzlehttp/guzzle
来源：http://mnh.aizwys.cn

[U42] PHP：PSR-4 自动加载
来源：http://vwv.jinyuanbaomall.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://djs.guannengcc.top

[U43] PHP：声明命名空间
来源：http://mfj.316326.xyz

namespace App\Http;
来源：http://xui.wangshuangyany.cn

[U44] PHP：开启严格类型
来源：http://std.sufxvd.cn

declare(strict_types=1);
来源：http://prs.mhx1999.top

[U45] PHP：类型声明与返回类型
来源：http://xwu.ybcxt.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://hmv.ppjwa.cn

[U46] PHP：可空类型
来源：http://tyf.tian-w.cn

?string $name = null
来源：http://zzw.pycfn.com

[U47] PHP：联合类型
来源：http://igq.ppjwa.cn

int|string $id
来源：http://jqe.daria6918.cn

[U48] PHP：纯枚举
来源：http://ldb.fehbvm.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://thd.zhixingplan.top

[U49] PHP：只读属性
来源：http://iuw.sjlbkw.cn

public readonly string $name
来源：http://izg.quarkkingdee.top

[U50] PHP：构造器属性提升
来源：http://dqi.vqdsnc.cn

public function __construct(private int $id) {}
来源：http://dxn.9152youxi.cn

[U51] PHP：数组解构
来源：http://npy.zdbjq.cn

[$a, $b] = $arr;
来源：http://ryd.daxiang520.top

[U52] PHP：箭头函数
来源：http://cqx.cucudq.cn

$double = fn($x) => $x * 2;
来源：http://eev.yuxming.cn

[U53] PHP：空合并运算符
来源：http://peb.cashguo.top

$v = $a ?? $b ?? "default";
来源：http://wko.chenjidiqi.icu

[U54] PHP：空安全调用
来源：http://vui.hywenlv.cn

$obj?->method()
来源：http://thy.kuanghao11.cn

[U55] PHP：match 表达式
来源：http://qbq.daxiang520.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xlo.316326.xyz

[U56] PHP：命名参数
来源：http://atx.zhaomingkeji.xyz

f(a: 1, b: 2)
来源：http://wmv.hesvh.cn

[U57] PHP：字符串插值
来源：http://qeq.hnqzz.top

"值: {$a}"
来源：http://avu.yvedp.cn

[U58] PHP：数组三件套
来源：http://gzk.iojbl.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gra.xuetiantiany.cn

[U59] PHP：自定义排序
来源：http://jjh.nanxinkj.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wyj.fanxiaobao.xyz

[U60] PHP：JSON 编解码
来源：http://okd.feifeiyinyue.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bro.ivvv.top

[U61] PHP：正则
来源：http://ncu.hesvh.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ugq.52xcode.cn

[U62] PHP：日期对象
来源：http://fck.iojbl.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://stf.smart0.xyz

[U63] PHP：文件读写
来源：http://jfs.zdbjq.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fjf.jqgfzy.top

[U64] PHP：目录遍历
来源：http://zym.fanxiaobao.xyz

glob("dir/*.php");  scandir("dir");
来源：http://vtt.daxiang520.top

[U65] PHP：会话
来源：http://jvh.yueranfly.top

session_start();  $_SESSION["uid"] = 1;
来源：http://crd.0kj1m.cn

[U66] PHP：设置 Cookie
来源：http://ovx.yj20258888.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://dkw.jiagoushi.top

[U67] PHP：处理文件上传
来源：http://jab.birdmap.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tad.guowangkeji.top

[U68] PHP：PDO 连接
来源：http://lfz.hesvh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cqh.sufxvd.cn

[U69] PHP：PDO 预处理
来源：http://aoo.hywenlv.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pwm.hnxiangtu.top

[U70] PHP：PDO 事务
来源：http://oun.guannengcc.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uzp.0kj1m.cn

[U71] PHP：抛出异常
来源：http://wwu.cucudq.cn

throw new RuntimeException("失败", 500);
来源：http://aml.svipenyu.cn

[U72] PHP：写错误日志
来源：http://oat.sweek.top

error_log("失败: " . $e->getMessage());
来源：http://iin.wangshuangyany.cn

[U73] PHP：读取 ini 配置
来源：http://xol.uphjek.com

parse_ini_file("config.ini", true)
来源：http://nfe.xinyue.icu

[U74] PHP：读取环境变量
来源：http://dqx.gotoacloud.top

getenv("APP_ENV") ?: "production"
来源：http://glv.zhiwuduotai.top

[U75] PHP：依赖注入
来源：http://xqr.sxryk.cn

composer require psr/container
来源：http://doz.yvedp.cn

[U76] PHP：简单路由
来源：http://geo.ppjwa.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cug.aizwys.cn

[U77] PHP：模板渲染
来源：http://hej.sysykeji.top

composer require twig/twig
来源：http://ict.tian-w.cn

[U78] PHP：单元测试
来源：http://xsr.cucudq.cn

composer require --dev phpunit/phpunit
来源：http://rza.jiagoushi.top

[U79] PHP：静态分析
来源：http://ola.zhoulong.xyz

composer require --dev phpstan/phpstan
来源：http://gjk.shuidangran.top

[U80] PHP：代码规范修复
来源：http://pjy.haohaochexian.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://mvc.daria6918.cn

[U81] JS：初始化项目
来源：http://qnw.ydjk.org.cn

npm init -y;  npm i express
来源：http://yav.zhijiandao.cn

[U82] JS：package.json 脚本
来源：http://fxu.sweek.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vvi.yueranfly.top

[U83] JS：ES Module 导入导出
来源：http://ijg.jlsjyb.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ers.yj20258888.top

[U84] JS：CommonJS 写法
来源：http://erc.ppjwa.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ena.fzhhl.top

[U85] JS：可选链
来源：http://gnr.birdmap.top

a?.b?.c
来源：http://zxy.wangdashe.top

[U86] JS：空值合并
来源：http://xsd.vehdjk.com

a ?? b
来源：http://wyp.jqgfzy.top

[U87] JS：解构默认值
来源：http://hzs.vehdjk.com

const { a = 1, b = 2 } = obj;
来源：http://hot.uphjek.com

[U88] JS：对象展开合并
来源：http://mez.cucudq.cn

{ ...a, ...b }
来源：http://bpo.fengsongda.top

[U89] JS：数组去重
来源：http://zwv.dianchejie.cn

[...new Set(arr)]
来源：http://qqa.tianlin.xyz

[U90] JS：数字数组排序
来源：http://izg.yvedp.cn

[...arr].sort((a, b) => a - b)
来源：http://jjb.chenzaomai.com

[U91] JS：对象键值遍历
来源：http://yxt.xinyue.icu

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qjp.fengsongda.top

[U92] JS：深拷贝
来源：http://jap.xuetiantiany.cn

structuredClone(obj)
来源：http://osc.wangdashe.top

[U93] JS：模板字符串
来源：http://nex.meibo888.top

`共 ${n} 条`
来源：http://ynt.mhx1999.top

[U94] JS：箭头函数
来源：http://lto.xylfe.cn

const double = x => x * 2;
来源：http://tth.c1oappe.top

[U95] JS：Promise 包装
来源：http://hsd.andypj.xyz

new Promise((resolve, reject) => {})
来源：http://qkp.gogol.net.cn

[U96] JS：async/await 与异常
来源：http://unz.c1oappe.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fhq.shanyushiyangkeji.top

[U97] JS：并发请求
来源：http://msl.sufxvd.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qow.aibaodan.cn

[U98] JS：fetch 带 JSON
来源：http://jsb.fzhhl.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vxf.sufxvd.cn

[U99] JS：事件监听
来源：http://jbe.meibo888.top

el.addEventListener("click", e => {})
来源：http://rig.vehdjk.com

[U100] JS：DOM 查询
来源：http://din.haohaochexian.top

document.querySelector(".item")
来源：http://xjp.andypj.xyz

[U101] JS：classList 操作
来源：http://vjv.vehdjk.com

el.classList.toggle("active")
来源：http://kyw.zycfv.cn

[U102] JS：本地存储
来源：http://kci.yuxming.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ilp.ehwqpu.com

[U103] JS：定时器
来源：http://fce.svipenyu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tss.xingfuxueyuan.xyz

[U104] JS：防抖
来源：http://iqs.ppjwa.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nlf.xuetiantiany.cn

[U105] JS：节流
来源：http://rio.quarkkingdee.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bcs.cqqwz.cn

[U106] JS：日期格式化
来源：http://kqf.ybcxt.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kva.cheryme.top

[U107] JS：数字千分位
来源：http://trq.ywan-chungtsiang.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ddn.havefunace.top

[U108] JS：随机整数
来源：http://ydh.vqdsnc.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wmd.shuidangran.top

[U109] JS：数组分组
来源：http://sgv.yanxiufei.cn

Object.groupBy(arr, x => x.type)
来源：http://lpq.pengpengdd.cyou

[U110] JS：数组分块
来源：http://ujm.cqqwz.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jmj.kuanghao11.cn

[U111] JS：对象转 Map
来源：http://uhj.zhongyouzk.top

new Map(Object.entries(obj))
来源：http://nwd.zhongyouzk.top

[U112] JS：字符串补位
来源：http://nhc.gotoacloud.top

"7".padStart(3, "0")
来源：http://doh.hysaishi.cn

[U113] JS：正则替换全部
来源：http://ywz.pycfn.com

s.replaceAll("a", "b")
来源：http://pvp.jinqigfzy.top

[U114] JS：JSON 深比较
来源：http://vjy.nwbrower.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rai.jianghu66.top

[U115] JS：生成 UUID
来源：http://tzk.xziqi.cn

crypto.randomUUID()
来源：http://wmv.havefunace.top

[U116] JS：类型检查（JSDoc）
来源：http://vyj.hcnkem.com

/** @param {string} name */ function f(name) {}
来源：http://xsq.sysykeji.top

[U117] JS：单元测试
来源：http://otz.xinyue.icu

npm i -D vitest;  npx vitest
来源：http://ixa.haohaochexian.top

[U118] JS：开发服务器
来源：http://meb.fktsv.cn

npm i -D vite;  npx vite
来源：http://bvv.yongpay.top

[U119] JS：生产构建
来源：http://dij.pycfn.com

npx vite build
来源：http://znm.jqgufenzy.top

[U120] JS：读取环境变量（Vite）
来源：http://mwy.yj202588.top

import.meta.env.VITE_API_URL
来源：http://rkw.vqdsnc.cn

================================================================================
来源：http://fqe.bjfxy.top

统计汇总
来源：http://spd.dianchejie.cn

================================================================================
来源：http://awl.jyoumei.cn

按语言统计（条）：
来源：http://jig.316326.xyz

Python ......... 252
来源：http://ajo.jiagoushi.top

PHP ............ 252
来源：http://iiz.daxiang520.top

JavaScript ..... 252
来源：http://tdr.cdnleiting.top

TypeScript ..... 212
来源：http://odw.hesvh.cn

Java ........... 212
来源：http://ucp.shanyushiyangtech.top

Go ............. 212
来源：http://dzr.feifeiyinyue.top

Ruby ........... 212
来源：http://pyq.zhoulong.xyz

C# ............. 212
来源：http://byu.jyoumei.cn

C .............. 30
来源：http://umw.pycfn.com

C++ ............ 30
来源：http://ktd.aizwys.cn

SQL ............ 90
来源：http://rbs.shanyushiyangkeji.top

Bash ........... 80
来源：http://kxa.tian-w.cn

Kotlin ......... 15
来源：http://tdr.andypj.xyz

Swift .......... 15
来源：http://rdk.tarul.cn

Lua ............ 10
来源：http://hok.ydjk.org.cn

Perl ........... 10
来源：http://pqh.zhoulong.xyz

Scala .......... 10
来源：http://eci.zhaomingkeji.xyz

------------------------------------
来源：http://nss.dashuyun.cn

合计 ........... 2106 条
来源：http://yuc.guannengcc.top

按章节统计：
来源：http://nnf.yj20258888.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sde.quarkkingdee.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://urq.bbcook.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vbk.daxiang520.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yrs.pengpengdd.cyou

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://prw.hnxiangtu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cro.kuanghao11.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hzv.andypj.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://plr.jianghu66.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mms.nwbrower.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qvi.hongshengwenyu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://key.fehbvm.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lov.yj20258888.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://umg.iojbl.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nrp.zycfv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ifs.tianlin.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bfm.jinghuilouyu.cn

Q SQL 专题                              90
来源：http://pzi.jyoumei.cn

R Bash 专题                             80
来源：http://njr.hfpthk.cn

S C / C++ 专题                          60
来源：http://xiv.yuanzhike.top

T 其他语言补充                          60
来源：http://nnz.shanyushiyangkeji.top

U 高频实用片段                         120
来源：http://tpg.cqqwz.cn

------------------------------------
来源：http://ktp.vqdsnc.cn

合计                                  2106 条
来源：http://zab.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://vzn.aizwys.cn

使用提醒
来源：http://cro.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://lqe.nanxuanxn.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gnc.hammf.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fbo.wangshuangyany.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lxy.zdqjudy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://pfu.tarul.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dki.sjlbkw.cn

—— 文件结束 ——
来源：http://gup.iojbl.cn

================================================================================
来源：http://awq.chenzaomai.com

程序语言常见例子速查手册（2024 版）
来源：http://xbt.xinyue.icu

Common Programming Examples Cheat Book
来源：http://mjx.havefunace.top

================================================================================
来源：http://bwk.zdqjudy.top

【收录内容】
来源：http://tkb.gogol.net.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ozz.fktsv.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xyq.wangdashe.top

SQL · Bash · C · C++
来源：http://bme.ivvv.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://was.havefunace.top

【使用说明】
来源：http://xjq.yongpay.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://iod.zhiwuduotai.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vwo.hfpthk.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ysg.daxiang520.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://shh.haohaochexian.top

Bash:  Shell         C:     C             C++:   C++
来源：http://hnj.tanke756.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jwz.nwbrower.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tke.gaohongyu789.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ncu.redwolf501.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jsu.hcnkem.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ixd.wangshuangyany.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tmx.hnqzz.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://oiq.yongpay.top

【文件统计】
来源：http://ibc.smart0.xyz

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nlq.yangfankeji.com

--------------------------------------------------------------------------------
来源：http://ysj.vehdjk.com

目  录
来源：http://tpk.ywan-chungtsiang.top

--------------------------------------------------------------------------------
来源：http://prm.cdnleiting.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ajm.iojbl.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vgm.ywan-chungtsiang.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qpo.haohaochexian.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rvz.xingfuxueyuan.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nyk.zhoulong.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jbx.zhongyouzk.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kkj.xingfuxueyuan.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zam.jqgfzy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ivs.yonumen.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gng.shanyushiyangkeji.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yyt.yongpay.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fpk.epnwcf.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jjr.epnwcf.com

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://eps.bjfxy.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pmg.hnxiangtu.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://npu.fktsv.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nqv.gaohongyu789.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://lil.aibaodan.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uip.vqdsnc.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nug.svipenyu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cij.vehdjk.com


<!-- 参考信息 -->