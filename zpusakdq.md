代发 wailian999

[U19] Py：正则替换带回调
来源：http://cqw.chenjidiqi.icu

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wjp.tian-w.cn

[U20] Py：缓存函数结果
来源：http://yqd.nwbrower.top

@functools.lru_cache(maxsize=None)
来源：http://kzx.0kj1m.cn

[U21] Py：自定义上下文管理器
来源：http://tok.dianchejie.cn

@contextlib.contextmanager
来源：http://qqt.sysykeji.top

[U22] Py：矩阵转置
来源：http://myu.vqdsnc.cn

list(zip(*m))
来源：http://snv.gogol.net.cn

[U23] Py：分块读取大文件
来源：http://rse.hnqzz.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mir.birdmap.top

[U24] Py：路径操作
来源：http://wmc.nanxinkj.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ocq.hammf.cn

[U25] Py：CSV 按字典读
来源：http://fsg.hcnkem.com

csv.DictReader(f)
来源：http://kgr.feifeiyinyue.top

[U26] Py：并发下载
来源：http://vdi.jianghu66.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mrx.gaohongyu789.top

[U27] Py：异步 HTTP
来源：http://rso.daxiang520.top

aiohttp.ClientSession() 配合 async with
来源：http://dae.yangfankeji.com

[U28] Py：类型别名
来源：http://aip.shzxlz.cn

UserId = int
来源：http://bdy.chenlongwang.top

[U29] Py：属性校验
来源：http://vgb.shanyushiyangkeji.top

@property 与 @x.setter 配合
来源：http://llh.feifeiyinyue.top

[U30] Py：数据类
来源：http://cou.wangdashe.top

@dataclass(slots=True)
来源：http://wfe.xylfe.cn

[U31] Py：单测
来源：http://vts.sweek.top

python -m pytest -q
来源：http://igg.zycfv.cn

[U32] Py：代码格式化
来源：http://thh.yonumen.top

ruff format . && ruff check --fix .
来源：http://rkx.dashuyun.cn

[U33] Py：打包发布
来源：http://tmw.cashguo.top

python -m build  （依赖 pyproject.toml）
来源：http://hoh.bjfxy.top

[U34] Py：判断编码
来源：http://dhp.sufxvd.cn

chardet.detect(raw)
来源：http://wyv.bbcook.cn

[U35] Py：发送邮件
来源：http://jmv.316326.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://aht.xylfe.cn

[U36] Py：定时任务
来源：http://jse.hnqzz.top

schedule.every(10).minutes.do(job)
来源：http://xsq.yuanzhike.top

[U37] Py：读写 Excel
来源：http://mho.feifeiyinyue.top

pandas.read_excel / DataFrame.to_excel
来源：http://gpn.ehwqpu.com

[U38] Py：获取脚本所在目录
来源：http://nrx.aizwys.cn

Path(__file__).resolve().parent
来源：http://xbs.xuetiantiany.cn

[U39] Py：判断是否在交互环境
来源：http://zsb.redwolf501.top

sys.stdout.isatty()
来源：http://lfi.havefunace.top

[U40] Py：打印到标准错误
来源：http://ble.zhijiandao.cn

print("err", file=sys.stderr)
来源：http://kqf.wangshuangyany.cn

[U41] PHP：初始化 Composer 项目
来源：http://dex.sjlbkw.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://apn.shzxlz.cn

[U42] PHP：PSR-4 自动加载
来源：http://syf.zhiwuduotai.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jvo.cashguo.top

[U43] PHP：声明命名空间
来源：http://adt.iojbl.cn

namespace App\Http;
来源：http://tvv.jqgufenzy.top

[U44] PHP：开启严格类型
来源：http://nnk.birdmap.top

declare(strict_types=1);
来源：http://cfz.cucudq.cn

[U45] PHP：类型声明与返回类型
来源：http://efc.ctjpmb.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://jgs.xylfe.cn

[U46] PHP：可空类型
来源：http://per.shanyushiyangkeji.top

?string $name = null
来源：http://tfg.yvedp.cn

[U47] PHP：联合类型
来源：http://uck.yuxming.cn

int|string $id
来源：http://egh.hcnkem.com

[U48] PHP：纯枚举
来源：http://cqa.jiagoushi.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://owv.hcnkem.com

[U49] PHP：只读属性
来源：http://gcl.wangdashe.top

public readonly string $name
来源：http://acq.sufxvd.cn

[U50] PHP：构造器属性提升
来源：http://boo.yuxming.cn

public function __construct(private int $id) {}
来源：http://yhs.daxiang520.top

[U51] PHP：数组解构
来源：http://ybz.guowangkeji.top

[$a, $b] = $arr;
来源：http://yur.vqdsnc.cn

[U52] PHP：箭头函数
来源：http://wqc.52xcode.cn

$double = fn($x) => $x * 2;
来源：http://xsy.gaohongyu789.top

[U53] PHP：空合并运算符
来源：http://hrq.yj202588.top

$v = $a ?? $b ?? "default";
来源：http://bww.aizwys.cn

[U54] PHP：空安全调用
来源：http://nil.bbcook.cn

$obj?->method()
来源：http://cxg.cashguo.top

[U55] PHP：match 表达式
来源：http://lpa.chenzaomai.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://saw.yj20258888.top

[U56] PHP：命名参数
来源：http://qat.ybcxt.top

f(a: 1, b: 2)
来源：http://zuo.jianghu66.top

[U57] PHP：字符串插值
来源：http://jmc.sjlbkw.cn

"值: {$a}"
来源：http://euw.52xcode.cn

[U58] PHP：数组三件套
来源：http://oes.yangfankeji.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pbp.gogol.net.cn

[U59] PHP：自定义排序
来源：http://bao.andypj.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bnr.vqdsnc.cn

[U60] PHP：JSON 编解码
来源：http://bva.yongpay.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cfi.ybcxt.top

[U61] PHP：正则
来源：http://jbu.jianghu66.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ftc.yj202588.top

[U62] PHP：日期对象
来源：http://ikn.uphjek.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jie.feifeiyinyue.top

[U63] PHP：文件读写
来源：http://nex.zhijiandao.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vhq.yj20258888.top

[U64] PHP：目录遍历
来源：http://chr.jqgfzy.top

glob("dir/*.php");  scandir("dir");
来源：http://quc.yonumen.top

[U65] PHP：会话
来源：http://jnh.jqgufenzy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://wqn.jianghu66.top

[U66] PHP：设置 Cookie
来源：http://flo.yanxiufei.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gwq.zycfv.cn

[U67] PHP：处理文件上传
来源：http://hey.ppjwa.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sgm.gotoacloud.top

[U68] PHP：PDO 连接
来源：http://ozt.dashuyun.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wkx.cdnleiting.top

[U69] PHP：PDO 预处理
来源：http://izg.fehbvm.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pik.yuanzhike.top

[U70] PHP：PDO 事务
来源：http://dkz.xuetiantiany.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mxs.ybcxt.top

[U71] PHP：抛出异常
来源：http://vbx.ydjk.org.cn

throw new RuntimeException("失败", 500);
来源：http://ory.shangyingyoupin.top

[U72] PHP：写错误日志
来源：http://ubu.haohaochexian.top

error_log("失败: " . $e->getMessage());
来源：http://dsf.sysykeji.top

[U73] PHP：读取 ini 配置
来源：http://evg.haohaochexian.top

parse_ini_file("config.ini", true)
来源：http://lhf.fanxiaobao.xyz

[U74] PHP：读取环境变量
来源：http://fig.birdmap.top

getenv("APP_ENV") ?: "production"
来源：http://joe.zhongyouzk.top

[U75] PHP：依赖注入
来源：http://wyd.fanxiaobao.xyz

composer require psr/container
来源：http://lgc.zhixingplan.top

[U76] PHP：简单路由
来源：http://bse.chenlongwang.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://iac.yanxiufei.cn

[U77] PHP：模板渲染
来源：http://vfc.ppjwa.cn

composer require twig/twig
来源：http://tak.daria6918.cn

[U78] PHP：单元测试
来源：http://chf.yangfankeji.com

composer require --dev phpunit/phpunit
来源：http://kro.tanke756.top

[U79] PHP：静态分析
来源：http://jaz.fanxiaobao.xyz

composer require --dev phpstan/phpstan
来源：http://ufc.zhoulong.xyz

[U80] PHP：代码规范修复
来源：http://uxm.cucudq.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://aps.chenzaomai.com

[U81] JS：初始化项目
来源：http://whd.yonumen.top

npm init -y;  npm i express
来源：http://nqe.aizwys.cn

[U82] JS：package.json 脚本
来源：http://qcj.jyoumei.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oqo.dianchejie.cn

[U83] JS：ES Module 导入导出
来源：http://zlx.ydjk.org.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qql.ctjpmb.com

[U84] JS：CommonJS 写法
来源：http://ewe.316326.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://plo.chenzaomai.com

[U85] JS：可选链
来源：http://clg.jinqigufen.top

a?.b?.c
来源：http://hic.shuidangran.top

[U86] JS：空值合并
来源：http://hon.nanxuanxn.top

a ?? b
来源：http://ljc.smart0.xyz

[U87] JS：解构默认值
来源：http://xrk.52xcode.cn

const { a = 1, b = 2 } = obj;
来源：http://oyu.yangfankeji.com

[U88] JS：对象展开合并
来源：http://zim.zdqjudy.top

{ ...a, ...b }
来源：http://qcw.zhaomingkeji.xyz

[U89] JS：数组去重
来源：http://gdr.ctjpmb.com

[...new Set(arr)]
来源：http://nfj.xylfe.cn

[U90] JS：数字数组排序
来源：http://jvr.wangshuangyany.cn

[...arr].sort((a, b) => a - b)
来源：http://erl.gogol.net.cn

[U91] JS：对象键值遍历
来源：http://roo.yj20258.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kkj.ivvv.top

[U92] JS：深拷贝
来源：http://rkr.tanke756.top

structuredClone(obj)
来源：http://lds.jlsjyb.cn

[U93] JS：模板字符串
来源：http://jlu.jinyuanbaomall.cn

`共 ${n} 条`
来源：http://mes.zhixingplan.top

[U94] JS：箭头函数
来源：http://zte.jiagoushi.top

const double = x => x * 2;
来源：http://rqh.cdnleiting.top

[U95] JS：Promise 包装
来源：http://zex.smart0.xyz

new Promise((resolve, reject) => {})
来源：http://pkh.gaohongyu789.top

[U96] JS：async/await 与异常
来源：http://hvj.daxiang520.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://obf.jinghuilouyu.cn

[U97] JS：并发请求
来源：http://dwe.guannengcc.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://xnx.tianlin.xyz

[U98] JS：fetch 带 JSON
来源：http://hog.hywenlv.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://oln.xylfe.cn

[U99] JS：事件监听
来源：http://ees.vqdsnc.cn

el.addEventListener("click", e => {})
来源：http://pxn.xuanzx.com

[U100] JS：DOM 查询
来源：http://rgo.shuidangran.top

document.querySelector(".item")
来源：http://kid.jiagoushi.top

[U101] JS：classList 操作
来源：http://pce.jianghu66.top

el.classList.toggle("active")
来源：http://xsg.cheryme.top

[U102] JS：本地存储
来源：http://ppj.cheryme.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://jqf.zhaomingkeji.xyz

[U103] JS：定时器
来源：http://otx.snrcjt.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://llr.hnqzz.top

[U104] JS：防抖
来源：http://uzl.sufxvd.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fpa.iojbl.cn

[U105] JS：节流
来源：http://gqm.zhoulong.xyz

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ash.sweek.top

[U106] JS：日期格式化
来源：http://kur.bbcook.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dzv.zhiwuduotai.top

[U107] JS：数字千分位
来源：http://dae.jinyuanbaomall.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sva.ctjpmb.com

[U108] JS：随机整数
来源：http://gam.zhoulong.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ewr.wangdashe.top

[U109] JS：数组分组
来源：http://pzg.9152youxi.cn

Object.groupBy(arr, x => x.type)
来源：http://wqu.gzhubu.top

[U110] JS：数组分块
来源：http://hfd.snrcjt.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pav.tian-w.cn

[U111] JS：对象转 Map
来源：http://dfa.vqdsnc.cn

new Map(Object.entries(obj))
来源：http://pei.vehdjk.com

[U112] JS：字符串补位
来源：http://asa.yueranfly.top

"7".padStart(3, "0")
来源：http://jsl.chenjidiqi.icu

[U113] JS：正则替换全部
来源：http://uxj.cqqwz.cn

s.replaceAll("a", "b")
来源：http://mnh.wangdashe.top

[U114] JS：JSON 深比较
来源：http://jsu.yangfankeji.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://ssy.uphjek.com

[U115] JS：生成 UUID
来源：http://ivq.yfazqb.com

crypto.randomUUID()
来源：http://gpd.ybcxt.top

[U116] JS：类型检查（JSDoc）
来源：http://rdi.yj20258888.top

/** @param {string} name */ function f(name) {}
来源：http://chu.hammf.cn

[U117] JS：单元测试
来源：http://yxj.zdbjq.cn

npm i -D vitest;  npx vitest
来源：http://gxt.hesvh.cn

[U118] JS：开发服务器
来源：http://vhx.jinqigufen.top

npm i -D vite;  npx vite
来源：http://sli.xziqi.cn

[U119] JS：生产构建
来源：http://lpr.yuxming.cn

npx vite build
来源：http://vgm.gzhubu.top

[U120] JS：读取环境变量（Vite）
来源：http://cha.sjlbkw.cn

import.meta.env.VITE_API_URL
来源：http://kra.uphjek.com

================================================================================
来源：http://bjn.9152youxi.cn

统计汇总
来源：http://fsy.fanxiaobao.xyz

================================================================================
来源：http://dqq.9152youxi.cn

按语言统计（条）：
来源：http://txl.fengsongda.top

Python ......... 252
来源：http://rsv.tanke756.top

PHP ............ 252
来源：http://ulm.nanxinkj.top

JavaScript ..... 252
来源：http://kgf.fzhhl.top

TypeScript ..... 212
来源：http://hbw.316326.xyz

Java ........... 212
来源：http://jcn.kuanghao11.cn

Go ............. 212
来源：http://nal.52xcode.cn

Ruby ........... 212
来源：http://jwe.nanxinkj.top

C# ............. 212
来源：http://gpw.9152youxi.cn

C .............. 30
来源：http://kci.shangyingyoupin.top

C++ ............ 30
来源：http://ysu.vqdsnc.cn

SQL ............ 90
来源：http://bny.sysykeji.top

Bash ........... 80
来源：http://pen.aibaodan.cn

Kotlin ......... 15
来源：http://bwg.yuanzhike.top

Swift .......... 15
来源：http://fxt.fktsv.cn

Lua ............ 10
来源：http://uqz.fanxiaobao.xyz

Perl ........... 10
来源：http://zwp.tianlin.xyz

Scala .......... 10
来源：http://pxg.quarkkingdee.top

------------------------------------
来源：http://cyh.yanxiufei.cn

合计 ........... 2106 条
来源：http://lvh.jqgfzy.top

按章节统计：
来源：http://hkr.jinqigufen.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jbw.c1oappe.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://frm.yj20258888.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://huq.yj202588.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zsz.jqgufenzy.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zwi.hesvh.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://aet.hfpthk.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vat.fehbvm.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hmv.ppjwa.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mxk.nanxuanxn.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mxf.vehdjk.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://odl.jianghu66.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rep.redwolf501.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dwf.xylfe.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wtj.9152youxi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vdl.chenlongwang.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ggd.svipenyu.cn

Q SQL 专题                              90
来源：http://jsp.pycfn.com

R Bash 专题                             80
来源：http://fqw.hfpthk.cn

S C / C++ 专题                          60
来源：http://twj.sjlbkw.cn

T 其他语言补充                          60
来源：http://kbk.xylfe.cn

U 高频实用片段                         120
来源：http://udk.hfpthk.cn

------------------------------------
来源：http://jsd.zhiwuduotai.top

合计                                  2106 条
来源：http://jvz.zdbjq.cn

--------------------------------------------------------------------------------
来源：http://cuo.ehwqpu.com

使用提醒
来源：http://xxa.redwolf501.top

--------------------------------------------------------------------------------
来源：http://isu.gzhubu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zjf.yfazqb.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bya.vqdsnc.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://glo.wangshuangyany.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://txa.cqqwz.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hhw.ybcxt.top

—— 文件结束 ——
来源：http://dhc.jinyuanbaomall.cn

================================================================================
来源：http://aws.tanke756.top

程序语言常见例子速查手册（2024 版）
来源：http://tid.zhiwuduotai.top

Common Programming Examples Cheat Book
来源：http://mot.aibaodan.cn

================================================================================
来源：http://xmt.aizwys.cn

【收录内容】
来源：http://mwv.9152youxi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://fko.jqgfzy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ouq.zhoulong.xyz

SQL · Bash · C · C++
来源：http://xnp.pycfn.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jyp.xinyue.icu

【使用说明】
来源：http://abe.xuanzx.com

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ust.ywan-chungtsiang.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ngw.jiagoushi.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cdw.gzhubu.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dsk.zhengqikj.top

Bash:  Shell         C:     C             C++:   C++
来源：http://aft.pycfn.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qaf.xingfuxueyuan.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bec.wangdashe.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xij.gzhubu.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ckx.tianlin.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://npv.nwbrower.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hvj.yuxming.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lya.zhongyouzk.top

【文件统计】
来源：http://uxe.yuanzhike.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jpt.jqgufenzy.top

--------------------------------------------------------------------------------
来源：http://iwy.uphjek.com

目  录
来源：http://hgk.dianchejie.cn

--------------------------------------------------------------------------------
来源：http://oly.yj20258888.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pwb.zhiwuduotai.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ccs.tanke756.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zkf.zhijiandao.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ycv.zhoulong.xyz

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://erx.xylfe.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ogo.zhiwuduotai.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ddb.tanke756.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mye.havefunace.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cse.yueranfly.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zgm.nanxinkj.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jsc.zhijiandao.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://any.haohaochexian.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bwh.yuanzhike.top


<!-- 参考信息 -->