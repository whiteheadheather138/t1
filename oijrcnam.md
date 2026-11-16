代发 wailian999

[U19] Py：正则替换带回调
来源：http://bki.wangshuangyany.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cjb.hnqzz.top

[U20] Py：缓存函数结果
来源：http://yqn.jinqigufen.top

@functools.lru_cache(maxsize=None)
来源：http://lzz.ehwqpu.com

[U21] Py：自定义上下文管理器
来源：http://iry.zhaomingkeji.xyz

@contextlib.contextmanager
来源：http://jhk.9152youxi.cn

[U22] Py：矩阵转置
来源：http://ckb.zdqjudy.top

list(zip(*m))
来源：http://shg.316326.xyz

[U23] Py：分块读取大文件
来源：http://zsv.aibaodan.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ztb.fktsv.cn

[U24] Py：路径操作
来源：http://bri.tianlin.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mzl.sysykeji.top

[U25] Py：CSV 按字典读
来源：http://mjn.52xcode.cn

csv.DictReader(f)
来源：http://xhw.xingfuxueyuan.xyz

[U26] Py：并发下载
来源：http://ugy.jlsjyb.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lou.jqgfzy.top

[U27] Py：异步 HTTP
来源：http://cbd.tanke756.top

aiohttp.ClientSession() 配合 async with
来源：http://hvd.ybcxt.top

[U28] Py：类型别名
来源：http://lbw.svipenyu.cn

UserId = int
来源：http://ufl.tanke756.top

[U29] Py：属性校验
来源：http://lyl.ivvv.top

@property 与 @x.setter 配合
来源：http://gzc.cqqwz.cn

[U30] Py：数据类
来源：http://fjk.ivvv.top

@dataclass(slots=True)
来源：http://cit.jinqigufen.top

[U31] Py：单测
来源：http://ypa.haohaochexian.top

python -m pytest -q
来源：http://zgf.chenjidiqi.icu

[U32] Py：代码格式化
来源：http://kbr.yongpay.top

ruff format . && ruff check --fix .
来源：http://ioh.yueranfly.top

[U33] Py：打包发布
来源：http://igq.yangfankeji.com

python -m build  （依赖 pyproject.toml）
来源：http://blc.feifeiyinyue.top

[U34] Py：判断编码
来源：http://bxb.hongshengwenyu.top

chardet.detect(raw)
来源：http://vxl.fanxiaobao.xyz

[U35] Py：发送邮件
来源：http://ljx.chenzaomai.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ife.jqgufenzy.top

[U36] Py：定时任务
来源：http://xuu.hnqzz.top

schedule.every(10).minutes.do(job)
来源：http://ums.pengpengdd.cyou

[U37] Py：读写 Excel
来源：http://ujq.yonumen.top

pandas.read_excel / DataFrame.to_excel
来源：http://sqo.yj202588.top

[U38] Py：获取脚本所在目录
来源：http://sdr.bjfxy.top

Path(__file__).resolve().parent
来源：http://ggh.vehdjk.com

[U39] Py：判断是否在交互环境
来源：http://wid.havefunace.top

sys.stdout.isatty()
来源：http://uew.aizwys.cn

[U40] Py：打印到标准错误
来源：http://bzk.yj202588.top

print("err", file=sys.stderr)
来源：http://rzk.zdqjudy.top

[U41] PHP：初始化 Composer 项目
来源：http://yxt.zhixingplan.top

composer init;  composer require guzzlehttp/guzzle
来源：http://lot.birdmap.top

[U42] PHP：PSR-4 自动加载
来源：http://wzr.ehwqpu.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cec.chenjidiqi.icu

[U43] PHP：声明命名空间
来源：http://bsq.hesvh.cn

namespace App\Http;
来源：http://uol.ivvv.top

[U44] PHP：开启严格类型
来源：http://oku.jlsjyb.cn

declare(strict_types=1);
来源：http://sif.ehwqpu.com

[U45] PHP：类型声明与返回类型
来源：http://ehs.52xcode.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ufs.aibaodan.cn

[U46] PHP：可空类型
来源：http://dxw.guowangkeji.top

?string $name = null
来源：http://vus.shangyingyoupin.top

[U47] PHP：联合类型
来源：http://usc.cdnleiting.top

int|string $id
来源：http://ujb.xingfuxueyuan.xyz

[U48] PHP：纯枚举
来源：http://vno.nanxuanxn.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sdk.yj20258888.top

[U49] PHP：只读属性
来源：http://mwx.mhx1999.top

public readonly string $name
来源：http://kxh.tianlin.xyz

[U50] PHP：构造器属性提升
来源：http://hiy.xylfe.cn

public function __construct(private int $id) {}
来源：http://bdm.zhoulong.xyz

[U51] PHP：数组解构
来源：http://bpp.wangdashe.top

[$a, $b] = $arr;
来源：http://epc.pycfn.com

[U52] PHP：箭头函数
来源：http://ojg.tian-w.cn

$double = fn($x) => $x * 2;
来源：http://vlo.gzhubu.top

[U53] PHP：空合并运算符
来源：http://bhs.fzhhl.top

$v = $a ?? $b ?? "default";
来源：http://fzo.cqqwz.cn

[U54] PHP：空安全调用
来源：http://hqv.wangshuangyany.cn

$obj?->method()
来源：http://sdk.chenjidiqi.icu

[U55] PHP：match 表达式
来源：http://inf.iojbl.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tzr.zhongyouzk.top

[U56] PHP：命名参数
来源：http://bfc.zdbjq.cn

f(a: 1, b: 2)
来源：http://bud.uphjek.com

[U57] PHP：字符串插值
来源：http://smp.tian-w.cn

"值: {$a}"
来源：http://hml.shanyushiyangtech.top

[U58] PHP：数组三件套
来源：http://brm.ppjwa.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dyw.zycfv.cn

[U59] PHP：自定义排序
来源：http://nfq.mhx1999.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iyg.gaohongyu789.top

[U60] PHP：JSON 编解码
来源：http://whb.xinyue.icu

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://flu.hywenlv.cn

[U61] PHP：正则
来源：http://evd.pengpengdd.cyou

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tbn.mhx1999.top

[U62] PHP：日期对象
来源：http://dlk.jinyuanbaomall.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kiu.daxiang520.top

[U63] PHP：文件读写
来源：http://mmd.316326.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nht.andypj.xyz

[U64] PHP：目录遍历
来源：http://fbh.hfpthk.cn

glob("dir/*.php");  scandir("dir");
来源：http://uvp.ydjk.org.cn

[U65] PHP：会话
来源：http://xkr.yonumen.top

session_start();  $_SESSION["uid"] = 1;
来源：http://vxs.meibo888.top

[U66] PHP：设置 Cookie
来源：http://jrv.vqdsnc.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vtj.9152youxi.cn

[U67] PHP：处理文件上传
来源：http://pwf.sysykeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fdv.sxryk.cn

[U68] PHP：PDO 连接
来源：http://nlp.zycfv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://obj.cheryme.top

[U69] PHP：PDO 预处理
来源：http://ago.zhiwuduotai.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ywf.dianchejie.cn

[U70] PHP：PDO 事务
来源：http://oyq.tarul.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ipo.fehbvm.com

[U71] PHP：抛出异常
来源：http://nuz.dashuyun.cn

throw new RuntimeException("失败", 500);
来源：http://phq.hongshengwenyu.top

[U72] PHP：写错误日志
来源：http://bod.yj20258.top

error_log("失败: " . $e->getMessage());
来源：http://rsg.shangyingyoupin.top

[U73] PHP：读取 ini 配置
来源：http://brp.chenlongwang.top

parse_ini_file("config.ini", true)
来源：http://win.ydzc1.top

[U74] PHP：读取环境变量
来源：http://mee.fengsongda.top

getenv("APP_ENV") ?: "production"
来源：http://khk.jinqigfzy.top

[U75] PHP：依赖注入
来源：http://pza.jinyuanbaomall.cn

composer require psr/container
来源：http://ljd.sxryk.cn

[U76] PHP：简单路由
来源：http://jta.haohaochexian.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xwg.fengsongda.top

[U77] PHP：模板渲染
来源：http://rno.hesvh.cn

composer require twig/twig
来源：http://xqf.jiagoushi.top

[U78] PHP：单元测试
来源：http://iwh.nanxinkj.top

composer require --dev phpunit/phpunit
来源：http://xsx.uphjek.com

[U79] PHP：静态分析
来源：http://cal.cqqwz.cn

composer require --dev phpstan/phpstan
来源：http://yjg.sysykeji.top

[U80] PHP：代码规范修复
来源：http://odx.pycfn.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://pvz.316326.xyz

[U81] JS：初始化项目
来源：http://vdm.hfpthk.cn

npm init -y;  npm i express
来源：http://fje.vqdsnc.cn

[U82] JS：package.json 脚本
来源：http://bdm.chenjidiqi.icu

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lcw.wangdashe.top

[U83] JS：ES Module 导入导出
来源：http://hvd.ivvv.top

export const a = 1;  import { a } from "./m.js";
来源：http://nmf.xuanzx.com

[U84] JS：CommonJS 写法
来源：http://fwr.yonumen.top

module.exports = { a };  const { a } = require("./m");
来源：http://zoe.yanxiufei.cn

[U85] JS：可选链
来源：http://kkr.hywenlv.cn

a?.b?.c
来源：http://xii.zdbjq.cn

[U86] JS：空值合并
来源：http://fjy.nanxuanxn.top

a ?? b
来源：http://fsx.cqqwz.cn

[U87] JS：解构默认值
来源：http://qrj.hywenlv.cn

const { a = 1, b = 2 } = obj;
来源：http://vlw.ydzc1.top

[U88] JS：对象展开合并
来源：http://gga.guannengcc.top

{ ...a, ...b }
来源：http://kmh.zdbjq.cn

[U89] JS：数组去重
来源：http://bva.smart0.xyz

[...new Set(arr)]
来源：http://xxg.ctjpmb.com

[U90] JS：数字数组排序
来源：http://lsb.fengsongda.top

[...arr].sort((a, b) => a - b)
来源：http://mgu.jinqigufen.top

[U91] JS：对象键值遍历
来源：http://brg.mhx1999.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qht.birdmap.top

[U92] JS：深拷贝
来源：http://ddt.nanxinkj.top

structuredClone(obj)
来源：http://iul.tianlin.xyz

[U93] JS：模板字符串
来源：http://nld.nanxuanxn.top

`共 ${n} 条`
来源：http://afc.fanxiaobao.xyz

[U94] JS：箭头函数
来源：http://igd.jinqigufen.top

const double = x => x * 2;
来源：http://ibh.zdqjudy.top

[U95] JS：Promise 包装
来源：http://gos.uphjek.com

new Promise((resolve, reject) => {})
来源：http://jvv.zdbjq.cn

[U96] JS：async/await 与异常
来源：http://qcs.svipenyu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bps.xylfe.cn

[U97] JS：并发请求
来源：http://rob.ywan-chungtsiang.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ssg.zhiwuduotai.top

[U98] JS：fetch 带 JSON
来源：http://rdy.shuidangran.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sfs.tianlin.xyz

[U99] JS：事件监听
来源：http://mlw.9152youxi.cn

el.addEventListener("click", e => {})
来源：http://vqt.pengpengdd.cyou

[U100] JS：DOM 查询
来源：http://cfh.havefunace.top

document.querySelector(".item")
来源：http://fow.shuidangran.top

[U101] JS：classList 操作
来源：http://qgu.xziqi.cn

el.classList.toggle("active")
来源：http://clp.ydzc1.top

[U102] JS：本地存储
来源：http://ihw.vqdsnc.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://epe.nanxinkj.top

[U103] JS：定时器
来源：http://syp.epnwcf.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ckg.52xcode.cn

[U104] JS：防抖
来源：http://wca.nanxuanxn.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tqr.snrcjt.cn

[U105] JS：节流
来源：http://ats.yonumen.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://stm.svipenyu.cn

[U106] JS：日期格式化
来源：http://kfv.jinghuilouyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tjw.zhengqikj.top

[U107] JS：数字千分位
来源：http://idq.fanxiaobao.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pjh.hcnkem.com

[U108] JS：随机整数
来源：http://mpz.zdqjudy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://exp.shanyushiyangtech.top

[U109] JS：数组分组
来源：http://ubj.dashuyun.cn

Object.groupBy(arr, x => x.type)
来源：http://nrf.hnxiangtu.top

[U110] JS：数组分块
来源：http://epz.quarkkingdee.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://new.jqgufenzy.top

[U111] JS：对象转 Map
来源：http://ysa.ppjwa.cn

new Map(Object.entries(obj))
来源：http://lmy.dianchejie.cn

[U112] JS：字符串补位
来源：http://hjc.chenjidiqi.icu

"7".padStart(3, "0")
来源：http://fua.shangyingyoupin.top

[U113] JS：正则替换全部
来源：http://lbm.hammf.cn

s.replaceAll("a", "b")
来源：http://qiy.yangfankeji.com

[U114] JS：JSON 深比较
来源：http://gne.cheryme.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://uey.gaohongyu789.top

[U115] JS：生成 UUID
来源：http://ogn.zhixingplan.top

crypto.randomUUID()
来源：http://vez.gzhubu.top

[U116] JS：类型检查（JSDoc）
来源：http://fce.wangdashe.top

/** @param {string} name */ function f(name) {}
来源：http://ghl.andypj.xyz

[U117] JS：单元测试
来源：http://ifx.yj20258.top

npm i -D vitest;  npx vitest
来源：http://ole.fktsv.cn

[U118] JS：开发服务器
来源：http://jta.ydzc1.top

npm i -D vite;  npx vite
来源：http://qug.zhongyouzk.top

[U119] JS：生产构建
来源：http://sma.redwolf501.top

npx vite build
来源：http://qje.jqgufenzy.top

[U120] JS：读取环境变量（Vite）
来源：http://msk.yuxming.cn

import.meta.env.VITE_API_URL
来源：http://fuh.yanxiufei.cn

================================================================================
来源：http://rwo.shzxlz.cn

统计汇总
来源：http://cxv.yuanzhike.top

================================================================================
来源：http://bhf.havefunace.top

按语言统计（条）：
来源：http://ytg.guowangkeji.top

Python ......... 252
来源：http://xjk.yvedp.cn

PHP ............ 252
来源：http://uzm.xuetiantiany.cn

JavaScript ..... 252
来源：http://nkb.xziqi.cn

TypeScript ..... 212
来源：http://jye.tarul.cn

Java ........... 212
来源：http://lnv.hfpthk.cn

Go ............. 212
来源：http://hzo.zhixingplan.top

Ruby ........... 212
来源：http://hzs.zhoulong.xyz

C# ............. 212
来源：http://huh.0kj1m.cn

C .............. 30
来源：http://vou.zhaomingkeji.xyz

C++ ............ 30
来源：http://mqc.jiagoushi.top

SQL ............ 90
来源：http://pfx.uphjek.com

Bash ........... 80
来源：http://vbj.quarkkingdee.top

Kotlin ......... 15
来源：http://trt.yfazqb.com

Swift .......... 15
来源：http://uhl.svipenyu.cn

Lua ............ 10
来源：http://fgw.nanxinkj.top

Perl ........... 10
来源：http://rxw.ivvv.top

Scala .......... 10
来源：http://bdg.cqqwz.cn

------------------------------------
来源：http://vxt.hfpthk.cn

合计 ........... 2106 条
来源：http://tzh.pengpengdd.cyou

按章节统计：
来源：http://npi.sysykeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://lln.jyoumei.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ixp.cqqwz.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nbj.zhixingplan.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://exn.ehwqpu.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rly.shanyushiyangtech.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://szy.zhengqikj.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vvw.chenlongwang.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pis.cucudq.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wzk.yanxiufei.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ume.hammf.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sod.cashguo.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://chl.fktsv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://npb.cucudq.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://iro.zdbjq.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wxz.nanxuanxn.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qfv.ehwqpu.com

Q SQL 专题                              90
来源：http://uku.cheryme.top

R Bash 专题                             80
来源：http://oxc.xingfuxueyuan.xyz

S C / C++ 专题                          60
来源：http://bxd.fengsongda.top

T 其他语言补充                          60
来源：http://owa.gogol.net.cn

U 高频实用片段                         120
来源：http://zlv.dashuyun.cn

------------------------------------
来源：http://qrw.havefunace.top

合计                                  2106 条
来源：http://nyw.jianghu66.top

--------------------------------------------------------------------------------
来源：http://znz.yuxming.cn

使用提醒
来源：http://ipk.zhaomingkeji.xyz

--------------------------------------------------------------------------------
来源：http://buw.nwbrower.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hqi.xuanzx.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://aob.gaohongyu789.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://eou.yfazqb.com

在旧版本上使用前请先确认语法支持情况。
来源：http://jox.hywenlv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://swp.jqgufenzy.top

—— 文件结束 ——
来源：http://hdp.sjlbkw.cn

================================================================================
来源：http://pzj.316326.xyz

程序语言常见例子速查手册（2024 版）
来源：http://yeq.zhoulong.xyz

Common Programming Examples Cheat Book
来源：http://mhh.jyoumei.cn

================================================================================
来源：http://bpp.iojbl.cn

【收录内容】
来源：http://txc.hcnkem.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://vbr.yfazqb.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ucb.ppjwa.cn

SQL · Bash · C · C++
来源：http://dzf.havefunace.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bui.zhengqikj.top

【使用说明】
来源：http://krt.xuetiantiany.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qku.ywan-chungtsiang.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rpt.yonumen.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wiz.xinyue.icu

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dju.jqgufenzy.top

Bash:  Shell         C:     C             C++:   C++
来源：http://gfe.jlsjyb.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://epg.gotoacloud.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ynt.chenzaomai.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lwl.316326.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yhv.zhengqikj.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qgs.hammf.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://siw.xingfuxueyuan.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://aqt.yanxiufei.cn

【文件统计】
来源：http://hfn.zhijiandao.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ers.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://rlx.hesvh.cn

目  录
来源：http://uva.yj202588.top

--------------------------------------------------------------------------------
来源：http://oqz.shangyingyoupin.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qkx.c1oappe.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dle.nwbrower.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kbq.haohaochexian.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uhu.cheryme.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hby.hfpthk.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dzy.yueranfly.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://edq.shanyushiyangkeji.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mfx.zhoulong.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://djm.zdqjudy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mnx.wangdashe.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mcx.gzhubu.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ypb.yuanzhike.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qku.dianchejie.cn


<!-- 参考信息 -->