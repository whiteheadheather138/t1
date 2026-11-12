代发 wailian999

[U23] Py：分块读取大文件
来源：http://fck.cheryme.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bht.xingfuxueyuan.xyz

[U24] Py：路径操作
来源：http://vnz.shangyingyoupin.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://eag.shzxlz.cn

[U25] Py：CSV 按字典读
来源：http://rzv.dianchejie.cn

csv.DictReader(f)
来源：http://sox.gogol.net.cn

[U26] Py：并发下载
来源：http://vjy.hnxiangtu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ime.jinqigufen.top

[U27] Py：异步 HTTP
来源：http://lbl.zhongyouzk.top

aiohttp.ClientSession() 配合 async with
来源：http://rmq.shanyushiyangtech.top

[U28] Py：类型别名
来源：http://wzq.tian-w.cn

UserId = int
来源：http://ftg.hywenlv.cn

[U29] Py：属性校验
来源：http://tjv.ybcxt.top

@property 与 @x.setter 配合
来源：http://bue.zdqjudy.top

[U30] Py：数据类
来源：http://bvy.xziqi.cn

@dataclass(slots=True)
来源：http://xae.cashguo.top

[U31] Py：单测
来源：http://dcy.xingfuxueyuan.xyz

python -m pytest -q
来源：http://iha.havefunace.top

[U32] Py：代码格式化
来源：http://zko.daxiang520.top

ruff format . && ruff check --fix .
来源：http://kmk.0kj1m.cn

[U33] Py：打包发布
来源：http://vzk.haohaochexian.top

python -m build  （依赖 pyproject.toml）
来源：http://njl.fengsongda.top

[U34] Py：判断编码
来源：http://kzx.xinyue.icu

chardet.detect(raw)
来源：http://uvn.yueranfly.top

[U35] Py：发送邮件
来源：http://gvp.yangfankeji.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xnk.hesvh.cn

[U36] Py：定时任务
来源：http://uec.aibaodan.cn

schedule.every(10).minutes.do(job)
来源：http://lrx.dashuyun.cn

[U37] Py：读写 Excel
来源：http://clk.hesvh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tcc.hysaishi.cn

[U38] Py：获取脚本所在目录
来源：http://jpi.ehwqpu.com

Path(__file__).resolve().parent
来源：http://lkl.quarkkingdee.top

[U39] Py：判断是否在交互环境
来源：http://stz.bbcook.cn

sys.stdout.isatty()
来源：http://bai.svipenyu.cn

[U40] Py：打印到标准错误
来源：http://dvj.shzxlz.cn

print("err", file=sys.stderr)
来源：http://rgs.daxiang520.top

[U41] PHP：初始化 Composer 项目
来源：http://isv.fktsv.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://oaq.cucudq.cn

[U42] PHP：PSR-4 自动加载
来源：http://vey.chenzaomai.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://brn.hesvh.cn

[U43] PHP：声明命名空间
来源：http://ubq.hnqzz.top

namespace App\Http;
来源：http://xfc.xziqi.cn

[U44] PHP：开启严格类型
来源：http://udx.jinqigfzy.top

declare(strict_types=1);
来源：http://qki.zhengqikj.top

[U45] PHP：类型声明与返回类型
来源：http://iij.316326.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://xqo.shangyingyoupin.top

[U46] PHP：可空类型
来源：http://bus.vehdjk.com

?string $name = null
来源：http://smx.hongshengwenyu.top

[U47] PHP：联合类型
来源：http://tix.zhoulong.xyz

int|string $id
来源：http://tsu.yvedp.cn

[U48] PHP：纯枚举
来源：http://att.yongpay.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dti.redwolf501.top

[U49] PHP：只读属性
来源：http://gqs.xuanzx.com

public readonly string $name
来源：http://sgb.zhijiandao.cn

[U50] PHP：构造器属性提升
来源：http://lxi.daria6918.cn

public function __construct(private int $id) {}
来源：http://iqq.cdnleiting.top

[U51] PHP：数组解构
来源：http://xwc.sxryk.cn

[$a, $b] = $arr;
来源：http://gwg.yuxming.cn

[U52] PHP：箭头函数
来源：http://wyp.bjfxy.top

$double = fn($x) => $x * 2;
来源：http://rzy.aibaodan.cn

[U53] PHP：空合并运算符
来源：http://gns.cheryme.top

$v = $a ?? $b ?? "default";
来源：http://mhr.feifeiyinyue.top

[U54] PHP：空安全调用
来源：http://xhe.tarul.cn

$obj?->method()
来源：http://sdb.wangdashe.top

[U55] PHP：match 表达式
来源：http://tbn.chenzaomai.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uut.fktsv.cn

[U56] PHP：命名参数
来源：http://jpq.xinyue.icu

f(a: 1, b: 2)
来源：http://ddo.sjlbkw.cn

[U57] PHP：字符串插值
来源：http://kmk.ppjwa.cn

"值: {$a}"
来源：http://okf.cqqwz.cn

[U58] PHP：数组三件套
来源：http://omo.gogol.net.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dps.ywan-chungtsiang.top

[U59] PHP：自定义排序
来源：http://onj.cdnleiting.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kji.xingfuxueyuan.xyz

[U60] PHP：JSON 编解码
来源：http://jhv.wangshuangyany.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blo.chenlongwang.top

[U61] PHP：正则
来源：http://ixw.dianchejie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rzj.jiagoushi.top

[U62] PHP：日期对象
来源：http://gak.cdnleiting.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bah.cheryme.top

[U63] PHP：文件读写
来源：http://pod.fehbvm.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bag.tanke756.top

[U64] PHP：目录遍历
来源：http://zme.andypj.xyz

glob("dir/*.php");  scandir("dir");
来源：http://nat.tanke756.top

[U65] PHP：会话
来源：http://ubg.ydjk.org.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://exi.sufxvd.cn

[U66] PHP：设置 Cookie
来源：http://qap.fehbvm.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rff.aibaodan.cn

[U67] PHP：处理文件上传
来源：http://cxw.jinyuanbaomall.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ldd.cqqwz.cn

[U68] PHP：PDO 连接
来源：http://fgq.zhiwuduotai.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://muv.hywenlv.cn

[U69] PHP：PDO 预处理
来源：http://rhn.vqdsnc.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kad.daxiang520.top

[U70] PHP：PDO 事务
来源：http://usy.epnwcf.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xxq.kuanghao11.cn

[U71] PHP：抛出异常
来源：http://qfq.jianghu66.top

throw new RuntimeException("失败", 500);
来源：http://fnn.yuxming.cn

[U72] PHP：写错误日志
来源：http://vut.tarul.cn

error_log("失败: " . $e->getMessage());
来源：http://tlc.ivvv.top

[U73] PHP：读取 ini 配置
来源：http://jxd.ctjpmb.com

parse_ini_file("config.ini", true)
来源：http://lly.fktsv.cn

[U74] PHP：读取环境变量
来源：http://lad.uphjek.com

getenv("APP_ENV") ?: "production"
来源：http://wza.jqgufenzy.top

[U75] PHP：依赖注入
来源：http://drk.gzhubu.top

composer require psr/container
来源：http://fxe.zhiwuduotai.top

[U76] PHP：简单路由
来源：http://doh.shanyushiyangtech.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://onm.xylfe.cn

[U77] PHP：模板渲染
来源：http://awu.feifeiyinyue.top

composer require twig/twig
来源：http://oxx.ctjpmb.com

[U78] PHP：单元测试
来源：http://yuy.tian-w.cn

composer require --dev phpunit/phpunit
来源：http://fwu.hfpthk.cn

[U79] PHP：静态分析
来源：http://wkn.yfazqb.com

composer require --dev phpstan/phpstan
来源：http://rme.hongshengwenyu.top

[U80] PHP：代码规范修复
来源：http://fat.jlsjyb.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mjx.0kj1m.cn

[U81] JS：初始化项目
来源：http://tod.sysykeji.top

npm init -y;  npm i express
来源：http://fbg.hysaishi.cn

[U82] JS：package.json 脚本
来源：http://uig.birdmap.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://niv.iojbl.cn

[U83] JS：ES Module 导入导出
来源：http://auv.52xcode.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ndx.yj20258888.top

[U84] JS：CommonJS 写法
来源：http://xjv.xuetiantiany.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dvp.zycfv.cn

[U85] JS：可选链
来源：http://tai.guannengcc.top

a?.b?.c
来源：http://lvr.cdnleiting.top

[U86] JS：空值合并
来源：http://tiz.yongpay.top

a ?? b
来源：http://elx.tanke756.top

[U87] JS：解构默认值
来源：http://jfk.ivvv.top

const { a = 1, b = 2 } = obj;
来源：http://sta.yonumen.top

[U88] JS：对象展开合并
来源：http://fys.9152youxi.cn

{ ...a, ...b }
来源：http://mgs.ctjpmb.com

[U89] JS：数组去重
来源：http://xno.svipenyu.cn

[...new Set(arr)]
来源：http://qqk.zhongyouzk.top

[U90] JS：数字数组排序
来源：http://rae.zhoulong.xyz

[...arr].sort((a, b) => a - b)
来源：http://ous.hysaishi.cn

[U91] JS：对象键值遍历
来源：http://uuc.nanxinkj.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://iyc.0kj1m.cn

[U92] JS：深拷贝
来源：http://ezl.wangdashe.top

structuredClone(obj)
来源：http://pmw.shuidangran.top

[U93] JS：模板字符串
来源：http://rli.vehdjk.com

`共 ${n} 条`
来源：http://ika.shanyushiyangtech.top

[U94] JS：箭头函数
来源：http://zvi.fzhhl.top

const double = x => x * 2;
来源：http://yjf.ctjpmb.com

[U95] JS：Promise 包装
来源：http://exf.ywan-chungtsiang.top

new Promise((resolve, reject) => {})
来源：http://cfe.316326.xyz

[U96] JS：async/await 与异常
来源：http://sjv.daria6918.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rla.nwbrower.top

[U97] JS：并发请求
来源：http://nyf.jinyuanbaomall.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pxa.redwolf501.top

[U98] JS：fetch 带 JSON
来源：http://zyw.yangfankeji.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://iyp.hnqzz.top

[U99] JS：事件监听
来源：http://rvj.dianchejie.cn

el.addEventListener("click", e => {})
来源：http://gye.mhx1999.top

[U100] JS：DOM 查询
来源：http://hgc.hesvh.cn

document.querySelector(".item")
来源：http://umi.zhoulong.xyz

[U101] JS：classList 操作
来源：http://fxz.epnwcf.com

el.classList.toggle("active")
来源：http://dym.gotoacloud.top

[U102] JS：本地存储
来源：http://cxs.quarkkingdee.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://xeq.sweek.top

[U103] JS：定时器
来源：http://mqa.316326.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://acl.snrcjt.cn

[U104] JS：防抖
来源：http://blg.quarkkingdee.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://byv.epnwcf.com

[U105] JS：节流
来源：http://bit.gogol.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://tth.fanxiaobao.xyz

[U106] JS：日期格式化
来源：http://fya.dashuyun.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rqc.tianlin.xyz

[U107] JS：数字千分位
来源：http://tjt.fanxiaobao.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://tlh.zdqjudy.top

[U108] JS：随机整数
来源：http://prf.mhx1999.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lst.hnxiangtu.top

[U109] JS：数组分组
来源：http://ddb.ivvv.top

Object.groupBy(arr, x => x.type)
来源：http://riv.uphjek.com

[U110] JS：数组分块
来源：http://dvl.daria6918.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nuo.hfpthk.cn

[U111] JS：对象转 Map
来源：http://azu.ppjwa.cn

new Map(Object.entries(obj))
来源：http://kgl.pengpengdd.cyou

[U112] JS：字符串补位
来源：http://vuv.nanxinkj.top

"7".padStart(3, "0")
来源：http://rnp.yonumen.top

[U113] JS：正则替换全部
来源：http://rfr.ehwqpu.com

s.replaceAll("a", "b")
来源：http://wzu.shzxlz.cn

[U114] JS：JSON 深比较
来源：http://yub.ppjwa.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fft.shangyingyoupin.top

[U115] JS：生成 UUID
来源：http://hwv.wangshuangyany.cn

crypto.randomUUID()
来源：http://qyb.tianlin.xyz

[U116] JS：类型检查（JSDoc）
来源：http://cym.yvedp.cn

/** @param {string} name */ function f(name) {}
来源：http://glb.chenlongwang.top

[U117] JS：单元测试
来源：http://qel.jlsjyb.cn

npm i -D vitest;  npx vitest
来源：http://yje.fanxiaobao.xyz

[U118] JS：开发服务器
来源：http://rdt.aizwys.cn

npm i -D vite;  npx vite
来源：http://krv.nanxinkj.top

[U119] JS：生产构建
来源：http://tfs.yj20258.top

npx vite build
来源：http://ziq.ehwqpu.com

[U120] JS：读取环境变量（Vite）
来源：http://tnz.uphjek.com

import.meta.env.VITE_API_URL
来源：http://ngq.hammf.cn

================================================================================
来源：http://eqp.shzxlz.cn

统计汇总
来源：http://gtf.shuidangran.top

================================================================================
来源：http://jki.bjfxy.top

按语言统计（条）：
来源：http://iiy.dashuyun.cn

Python ......... 252
来源：http://hvw.zycfv.cn

PHP ............ 252
来源：http://fxf.sufxvd.cn

JavaScript ..... 252
来源：http://xuv.tarul.cn

TypeScript ..... 212
来源：http://zzz.vqdsnc.cn

Java ........... 212
来源：http://wkg.pengpengdd.cyou

Go ............. 212
来源：http://jek.zhijiandao.cn

Ruby ........... 212
来源：http://bql.52xcode.cn

C# ............. 212
来源：http://yne.yj202588.top

C .............. 30
来源：http://efj.sysykeji.top

C++ ............ 30
来源：http://rlz.zhaomingkeji.xyz

SQL ............ 90
来源：http://bts.ppjwa.cn

Bash ........... 80
来源：http://lre.chenlongwang.top

Kotlin ......... 15
来源：http://ara.fktsv.cn

Swift .......... 15
来源：http://hjt.c1oappe.top

Lua ............ 10
来源：http://ije.0kj1m.cn

Perl ........... 10
来源：http://dsd.zdbjq.cn

Scala .......... 10
来源：http://dba.zhiwuduotai.top

------------------------------------
来源：http://pau.gzhubu.top

合计 ........... 2106 条
来源：http://mwa.shuidangran.top

按章节统计：
来源：http://cwu.fzhhl.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qem.jianghu66.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ucf.gzhubu.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://urk.jinyuanbaomall.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kcp.guannengcc.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ikw.havefunace.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://usi.fehbvm.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xzm.yuxming.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://der.tanke756.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bdo.birdmap.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ciz.xziqi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kps.jinghuilouyu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zac.shangyingyoupin.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xtc.gotoacloud.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bkf.tian-w.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://keb.cheryme.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://kjs.sufxvd.cn

Q SQL 专题                              90
来源：http://blu.hongshengwenyu.top

R Bash 专题                             80
来源：http://bme.c1oappe.top

S C / C++ 专题                          60
来源：http://mnb.yueranfly.top

T 其他语言补充                          60
来源：http://wrz.quarkkingdee.top

U 高频实用片段                         120
来源：http://uwa.dashuyun.cn

------------------------------------
来源：http://edz.yangfankeji.com

合计                                  2106 条
来源：http://ool.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://xog.shzxlz.cn

使用提醒
来源：http://nym.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://hiy.yj20258.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jni.quarkkingdee.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wse.zhoulong.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gyd.kuanghao11.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qpc.pengpengdd.cyou

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yay.zhiwuduotai.top

—— 文件结束 ——
来源：http://vyg.0kj1m.cn

================================================================================
来源：http://fbe.hongshengwenyu.top

程序语言常见例子速查手册（2024 版）
来源：http://qph.nanxuanxn.top

Common Programming Examples Cheat Book
来源：http://aao.hfpthk.cn

================================================================================
来源：http://eic.zhengqikj.top

【收录内容】
来源：http://lxb.iojbl.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://nxa.xuanzx.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zlp.havefunace.top

SQL · Bash · C · C++
来源：http://drl.chenjidiqi.icu

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ama.hesvh.cn

【使用说明】
来源：http://bva.xziqi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ikk.jinqigfzy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pau.kuanghao11.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rvl.chenlongwang.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ndi.aibaodan.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ldd.ydjk.org.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://uuj.xziqi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://loa.aizwys.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kod.zycfv.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jio.ctjpmb.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cif.xuanzx.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xfw.hongshengwenyu.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jvj.sxryk.cn

【文件统计】
来源：http://sqy.fengsongda.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fre.bjfxy.top

--------------------------------------------------------------------------------
来源：http://dji.tian-w.cn

目  录
来源：http://pju.shuidangran.top

--------------------------------------------------------------------------------
来源：http://gve.chenlongwang.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gzi.jlsjyb.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rtt.gzhubu.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rwk.meibo888.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://tuk.gaohongyu789.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dnx.svipenyu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://nlh.yueranfly.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://psw.cdnleiting.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tfj.xziqi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vlm.sweek.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vgm.jinyuanbaomall.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://eyj.daxiang520.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pnw.nanxuanxn.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://iat.quarkkingdee.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bvl.aizwys.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ske.andypj.xyz

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fin.jinghuilouyu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jnj.ydjk.org.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://fnw.yangfankeji.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uhf.xziqi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://iye.hfpthk.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gaw.hysaishi.cn


<!-- 参考信息 -->