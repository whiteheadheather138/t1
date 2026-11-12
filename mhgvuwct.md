代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://zzy.gzhubu.top

@contextlib.contextmanager
来源：http://lcz.aibaodan.cn

[U22] Py：矩阵转置
来源：http://ust.dianchejie.cn

list(zip(*m))
来源：http://cbi.tarul.cn

[U23] Py：分块读取大文件
来源：http://yxk.nanxinkj.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ltg.pengpengdd.cyou

[U24] Py：路径操作
来源：http://wrr.zycfv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gol.cqqwz.cn

[U25] Py：CSV 按字典读
来源：http://hal.meibo888.top

csv.DictReader(f)
来源：http://mpr.redwolf501.top

[U26] Py：并发下载
来源：http://ndi.mhx1999.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ijz.yanxiufei.cn

[U27] Py：异步 HTTP
来源：http://tmr.c1oappe.top

aiohttp.ClientSession() 配合 async with
来源：http://ceo.jyoumei.cn

[U28] Py：类型别名
来源：http://sct.fengsongda.top

UserId = int
来源：http://aom.jqgufenzy.top

[U29] Py：属性校验
来源：http://xmi.yangfankeji.com

@property 与 @x.setter 配合
来源：http://ema.tian-w.cn

[U30] Py：数据类
来源：http://bqm.jinghuilouyu.cn

@dataclass(slots=True)
来源：http://vjj.hnqzz.top

[U31] Py：单测
来源：http://izd.sjlbkw.cn

python -m pytest -q
来源：http://vcn.mhx1999.top

[U32] Py：代码格式化
来源：http://xnc.nanxinkj.top

ruff format . && ruff check --fix .
来源：http://fid.gaohongyu789.top

[U33] Py：打包发布
来源：http://zhj.fengsongda.top

python -m build  （依赖 pyproject.toml）
来源：http://fyj.sysykeji.top

[U34] Py：判断编码
来源：http://fvx.sysykeji.top

chardet.detect(raw)
来源：http://ifo.ppjwa.cn

[U35] Py：发送邮件
来源：http://jzt.andypj.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lvt.hongshengwenyu.top

[U36] Py：定时任务
来源：http://ioc.uphjek.com

schedule.every(10).minutes.do(job)
来源：http://nrm.jinyuanbaomall.cn

[U37] Py：读写 Excel
来源：http://qca.c1oappe.top

pandas.read_excel / DataFrame.to_excel
来源：http://epj.tian-w.cn

[U38] Py：获取脚本所在目录
来源：http://aep.havefunace.top

Path(__file__).resolve().parent
来源：http://ejs.yj202588.top

[U39] Py：判断是否在交互环境
来源：http://rrz.tian-w.cn

sys.stdout.isatty()
来源：http://gvx.ppjwa.cn

[U40] Py：打印到标准错误
来源：http://vxm.jiagoushi.top

print("err", file=sys.stderr)
来源：http://ygq.fehbvm.com

[U41] PHP：初始化 Composer 项目
来源：http://rga.jinghuilouyu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://egr.dashuyun.cn

[U42] PHP：PSR-4 自动加载
来源：http://rvd.yonumen.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zim.9152youxi.cn

[U43] PHP：声明命名空间
来源：http://glp.pengpengdd.cyou

namespace App\Http;
来源：http://wfo.jqgfzy.top

[U44] PHP：开启严格类型
来源：http://att.gogol.net.cn

declare(strict_types=1);
来源：http://rhn.yongpay.top

[U45] PHP：类型声明与返回类型
来源：http://bku.xingfuxueyuan.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://irm.chenzaomai.com

[U46] PHP：可空类型
来源：http://jni.fengsongda.top

?string $name = null
来源：http://ajv.dianchejie.cn

[U47] PHP：联合类型
来源：http://aeg.jqgfzy.top

int|string $id
来源：http://dwg.sysykeji.top

[U48] PHP：纯枚举
来源：http://ynv.xylfe.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://acs.hysaishi.cn

[U49] PHP：只读属性
来源：http://bih.zhaomingkeji.xyz

public readonly string $name
来源：http://fzf.fanxiaobao.xyz

[U50] PHP：构造器属性提升
来源：http://xwd.xuanzx.com

public function __construct(private int $id) {}
来源：http://zjd.dashuyun.cn

[U51] PHP：数组解构
来源：http://ydm.pycfn.com

[$a, $b] = $arr;
来源：http://zuu.52xcode.cn

[U52] PHP：箭头函数
来源：http://ayp.gaohongyu789.top

$double = fn($x) => $x * 2;
来源：http://ecv.andypj.xyz

[U53] PHP：空合并运算符
来源：http://ors.daria6918.cn

$v = $a ?? $b ?? "default";
来源：http://fny.zycfv.cn

[U54] PHP：空安全调用
来源：http://laf.meibo888.top

$obj?->method()
来源：http://cns.ydjk.org.cn

[U55] PHP：match 表达式
来源：http://emu.vehdjk.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uli.haohaochexian.top

[U56] PHP：命名参数
来源：http://reo.fzhhl.top

f(a: 1, b: 2)
来源：http://vta.ctjpmb.com

[U57] PHP：字符串插值
来源：http://blg.iojbl.cn

"值: {$a}"
来源：http://ikh.shanyushiyangtech.top

[U58] PHP：数组三件套
来源：http://ofy.yj20258888.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ltc.yueranfly.top

[U59] PHP：自定义排序
来源：http://eds.smart0.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tqb.epnwcf.com

[U60] PHP：JSON 编解码
来源：http://ofe.smart0.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rzn.tian-w.cn

[U61] PHP：正则
来源：http://ltf.ivvv.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wzz.shanyushiyangkeji.top

[U62] PHP：日期对象
来源：http://trj.jinghuilouyu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rns.ydzc1.top

[U63] PHP：文件读写
来源：http://dde.fzhhl.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tnw.gotoacloud.top

[U64] PHP：目录遍历
来源：http://qwk.cucudq.cn

glob("dir/*.php");  scandir("dir");
来源：http://vrf.yj20258888.top

[U65] PHP：会话
来源：http://rew.dashuyun.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ifg.zhengqikj.top

[U66] PHP：设置 Cookie
来源：http://spi.nanxinkj.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://nre.aizwys.cn

[U67] PHP：处理文件上传
来源：http://slc.ydjk.org.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mvj.jinqigufen.top

[U68] PHP：PDO 连接
来源：http://clf.uphjek.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://try.hysaishi.cn

[U69] PHP：PDO 预处理
来源：http://jpa.xuetiantiany.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yyj.yfazqb.com

[U70] PHP：PDO 事务
来源：http://tkw.jlsjyb.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gqe.dianchejie.cn

[U71] PHP：抛出异常
来源：http://zsb.xuanzx.com

throw new RuntimeException("失败", 500);
来源：http://kyp.sysykeji.top

[U72] PHP：写错误日志
来源：http://xqg.jinqigufen.top

error_log("失败: " . $e->getMessage());
来源：http://guo.zdqjudy.top

[U73] PHP：读取 ini 配置
来源：http://fwz.yangfankeji.com

parse_ini_file("config.ini", true)
来源：http://ukc.fzhhl.top

[U74] PHP：读取环境变量
来源：http://whi.tianlin.xyz

getenv("APP_ENV") ?: "production"
来源：http://sue.hysaishi.cn

[U75] PHP：依赖注入
来源：http://hwb.zhongyouzk.top

composer require psr/container
来源：http://xvb.jinqigfzy.top

[U76] PHP：简单路由
来源：http://ryx.jinghuilouyu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wvj.yj20258.top

[U77] PHP：模板渲染
来源：http://rfy.vehdjk.com

composer require twig/twig
来源：http://bie.guannengcc.top

[U78] PHP：单元测试
来源：http://pom.hysaishi.cn

composer require --dev phpunit/phpunit
来源：http://smd.sufxvd.cn

[U79] PHP：静态分析
来源：http://uff.shanyushiyangkeji.top

composer require --dev phpstan/phpstan
来源：http://hba.hnxiangtu.top

[U80] PHP：代码规范修复
来源：http://ptr.yongpay.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://agk.ctjpmb.com

[U81] JS：初始化项目
来源：http://rlw.hammf.cn

npm init -y;  npm i express
来源：http://ers.hcnkem.com

[U82] JS：package.json 脚本
来源：http://ibz.ydjk.org.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mxa.haohaochexian.top

[U83] JS：ES Module 导入导出
来源：http://agh.fanxiaobao.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://ihf.yvedp.cn

[U84] JS：CommonJS 写法
来源：http://jyr.ydjk.org.cn

module.exports = { a };  const { a } = require("./m");
来源：http://okk.jyoumei.cn

[U85] JS：可选链
来源：http://ruq.mhx1999.top

a?.b?.c
来源：http://txo.yanxiufei.cn

[U86] JS：空值合并
来源：http://vom.quarkkingdee.top

a ?? b
来源：http://stq.shangyingyoupin.top

[U87] JS：解构默认值
来源：http://lju.zhijiandao.cn

const { a = 1, b = 2 } = obj;
来源：http://hfr.hysaishi.cn

[U88] JS：对象展开合并
来源：http://exc.yj20258888.top

{ ...a, ...b }
来源：http://zru.aizwys.cn

[U89] JS：数组去重
来源：http://btg.hnxiangtu.top

[...new Set(arr)]
来源：http://lsk.zhongyouzk.top

[U90] JS：数字数组排序
来源：http://ndf.yueranfly.top

[...arr].sort((a, b) => a - b)
来源：http://ubl.zhaomingkeji.xyz

[U91] JS：对象键值遍历
来源：http://dcs.jinqigufen.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yuu.uphjek.com

[U92] JS：深拷贝
来源：http://cun.ydzc1.top

structuredClone(obj)
来源：http://cxg.birdmap.top

[U93] JS：模板字符串
来源：http://lzh.yfazqb.com

`共 ${n} 条`
来源：http://rtf.wangshuangyany.cn

[U94] JS：箭头函数
来源：http://pyx.chenlongwang.top

const double = x => x * 2;
来源：http://xvk.ehwqpu.com

[U95] JS：Promise 包装
来源：http://kbn.wangdashe.top

new Promise((resolve, reject) => {})
来源：http://hig.snrcjt.cn

[U96] JS：async/await 与异常
来源：http://wzf.cucudq.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://iuw.hfpthk.cn

[U97] JS：并发请求
来源：http://cxp.jianghu66.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://yek.yj20258.top

[U98] JS：fetch 带 JSON
来源：http://rkr.gaohongyu789.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pzi.yuxming.cn

[U99] JS：事件监听
来源：http://agt.zdqjudy.top

el.addEventListener("click", e => {})
来源：http://xix.feifeiyinyue.top

[U100] JS：DOM 查询
来源：http://eea.jinghuilouyu.cn

document.querySelector(".item")
来源：http://kjg.shanyushiyangtech.top

[U101] JS：classList 操作
来源：http://rhf.fktsv.cn

el.classList.toggle("active")
来源：http://fnx.bbcook.cn

[U102] JS：本地存储
来源：http://syj.sxryk.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://nxy.wangdashe.top

[U103] JS：定时器
来源：http://lac.52xcode.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sqv.guannengcc.top

[U104] JS：防抖
来源：http://emo.dianchejie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ovb.gotoacloud.top

[U105] JS：节流
来源：http://sex.zdbjq.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qko.fktsv.cn

[U106] JS：日期格式化
来源：http://ker.hywenlv.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vvx.tianlin.xyz

[U107] JS：数字千分位
来源：http://beb.hcnkem.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pez.jinqigufen.top

[U108] JS：随机整数
来源：http://kjc.haohaochexian.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://osi.zhaomingkeji.xyz

[U109] JS：数组分组
来源：http://xxy.gzhubu.top

Object.groupBy(arr, x => x.type)
来源：http://qyy.yuxming.cn

[U110] JS：数组分块
来源：http://xdc.sysykeji.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pnv.cucudq.cn

[U111] JS：对象转 Map
来源：http://mqc.zhengqikj.top

new Map(Object.entries(obj))
来源：http://bxa.xziqi.cn

[U112] JS：字符串补位
来源：http://duu.sweek.top

"7".padStart(3, "0")
来源：http://pdj.svipenyu.cn

[U113] JS：正则替换全部
来源：http://jpj.sxryk.cn

s.replaceAll("a", "b")
来源：http://afy.hywenlv.cn

[U114] JS：JSON 深比较
来源：http://fto.gaohongyu789.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://bno.quarkkingdee.top

[U115] JS：生成 UUID
来源：http://imu.sysykeji.top

crypto.randomUUID()
来源：http://tud.sysykeji.top

[U116] JS：类型检查（JSDoc）
来源：http://edo.9152youxi.cn

/** @param {string} name */ function f(name) {}
来源：http://eug.ctjpmb.com

[U117] JS：单元测试
来源：http://uek.yfazqb.com

npm i -D vitest;  npx vitest
来源：http://zgf.cashguo.top

[U118] JS：开发服务器
来源：http://tgk.shuidangran.top

npm i -D vite;  npx vite
来源：http://kbe.fktsv.cn

[U119] JS：生产构建
来源：http://slv.meibo888.top

npx vite build
来源：http://gsm.shzxlz.cn

[U120] JS：读取环境变量（Vite）
来源：http://koh.sxryk.cn

import.meta.env.VITE_API_URL
来源：http://njq.zdqjudy.top

================================================================================
来源：http://vps.nwbrower.top

统计汇总
来源：http://pjt.quarkkingdee.top

================================================================================
来源：http://rcr.hongshengwenyu.top

按语言统计（条）：
来源：http://wfh.hysaishi.cn

Python ......... 252
来源：http://hfg.cdnleiting.top

PHP ............ 252
来源：http://rta.xylfe.cn

JavaScript ..... 252
来源：http://nbh.zhoulong.xyz

TypeScript ..... 212
来源：http://xjn.snrcjt.cn

Java ........... 212
来源：http://bnd.0kj1m.cn

Go ............. 212
来源：http://lnd.sufxvd.cn

Ruby ........... 212
来源：http://bqb.quarkkingdee.top

C# ............. 212
来源：http://adn.chenlongwang.top

C .............. 30
来源：http://hss.uphjek.com

C++ ............ 30
来源：http://xqk.vehdjk.com

SQL ............ 90
来源：http://eoi.aibaodan.cn

Bash ........... 80
来源：http://frj.ydzc1.top

Kotlin ......... 15
来源：http://dgp.zhongyouzk.top

Swift .......... 15
来源：http://zsi.cheryme.top

Lua ............ 10
来源：http://vzv.yj20258.top

Perl ........... 10
来源：http://xel.yanxiufei.cn

Scala .......... 10
来源：http://bpi.yueranfly.top

------------------------------------
来源：http://zfa.ybcxt.top

合计 ........... 2106 条
来源：http://cxs.yuanzhike.top

按章节统计：
来源：http://hlt.cucudq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hnl.hfpthk.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://iwh.sxryk.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jtx.gaohongyu789.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wqd.yj20258.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://clb.xuetiantiany.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://eod.vehdjk.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dcn.sxryk.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wgq.vehdjk.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://prr.cqqwz.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gqa.cqqwz.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qng.cheryme.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wbb.snrcjt.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cpu.xuetiantiany.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ltl.sweek.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://spk.9152youxi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://oxd.sufxvd.cn

Q SQL 专题                              90
来源：http://leh.zhiwuduotai.top

R Bash 专题                             80
来源：http://ckc.yonumen.top

S C / C++ 专题                          60
来源：http://jad.pengpengdd.cyou

T 其他语言补充                          60
来源：http://pyb.yfazqb.com

U 高频实用片段                         120
来源：http://ics.gzhubu.top

------------------------------------
来源：http://dzu.fehbvm.com

合计                                  2106 条
来源：http://ila.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://rwa.0kj1m.cn

使用提醒
来源：http://tcu.cashguo.top

--------------------------------------------------------------------------------
来源：http://okq.sweek.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gze.ctjpmb.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://oab.chenlongwang.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rul.wangdashe.top

在旧版本上使用前请先确认语法支持情况。
来源：http://lxe.zdbjq.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zpm.jianghu66.top

—— 文件结束 ——
来源：http://drn.daxiang520.top

================================================================================
来源：http://dlp.xuetiantiany.cn

程序语言常见例子速查手册（2024 版）
来源：http://yih.dashuyun.cn

Common Programming Examples Cheat Book
来源：http://fzo.316326.xyz

================================================================================
来源：http://hgo.tian-w.cn

【收录内容】
来源：http://hlu.ywan-chungtsiang.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://kwv.yuxming.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lmf.chenjidiqi.icu

SQL · Bash · C · C++
来源：http://rfw.yvedp.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://btc.feifeiyinyue.top

【使用说明】
来源：http://dqc.birdmap.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bun.snrcjt.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lfw.cqqwz.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ctd.iojbl.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pxy.jiagoushi.top

Bash:  Shell         C:     C             C++:   C++
来源：http://dqm.nanxuanxn.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ruf.birdmap.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://koe.zdqjudy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vqv.yanxiufei.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ujv.jqgfzy.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bra.fzhhl.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ews.xinyue.icu

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fyk.aibaodan.cn

【文件统计】
来源：http://fhg.zdqjudy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gcg.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://prx.andypj.xyz

目  录
来源：http://hmd.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://vgt.chenzaomai.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wxh.yueranfly.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://buw.ybcxt.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://smh.yj202588.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ilj.wangdashe.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://svo.ivvv.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://btb.wangdashe.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hii.tanke756.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dtf.nanxinkj.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xlf.ppjwa.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dyu.feifeiyinyue.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yyj.jiagoushi.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vbo.fehbvm.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://sqn.fktsv.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://phq.snrcjt.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fwp.xylfe.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rzy.yueranfly.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lgq.nanxuanxn.top


<!-- 参考信息 -->