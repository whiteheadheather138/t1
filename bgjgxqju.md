代发 wailian999

[U17] Py：初始化日志
来源：http://qri.jqgufenzy.top

logging.basicConfig(level=logging.INFO)
来源：http://iss.xinyue.icu

[U18] Py：预编译正则
来源：http://fbx.zhongyouzk.top

pat = re.compile(r"\d+")
来源：http://lma.yueranfly.top

[U19] Py：正则替换带回调
来源：http://jga.ywan-chungtsiang.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qpt.zdbjq.cn

[U20] Py：缓存函数结果
来源：http://dmi.guowangkeji.top

@functools.lru_cache(maxsize=None)
来源：http://ydt.hysaishi.cn

[U21] Py：自定义上下文管理器
来源：http://xrx.feifeiyinyue.top

@contextlib.contextmanager
来源：http://fll.yj202588.top

[U22] Py：矩阵转置
来源：http://kde.chenlongwang.top

list(zip(*m))
来源：http://xuf.52xcode.cn

[U23] Py：分块读取大文件
来源：http://eli.yj20258888.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nru.shzxlz.cn

[U24] Py：路径操作
来源：http://pre.mhx1999.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hjx.yvedp.cn

[U25] Py：CSV 按字典读
来源：http://lqh.shuidangran.top

csv.DictReader(f)
来源：http://ouz.jianghu66.top

[U26] Py：并发下载
来源：http://jqr.ybcxt.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mlu.yuanzhike.top

[U27] Py：异步 HTTP
来源：http://beb.zhaomingkeji.xyz

aiohttp.ClientSession() 配合 async with
来源：http://owp.xingfuxueyuan.xyz

[U28] Py：类型别名
来源：http://vyy.hfpthk.cn

UserId = int
来源：http://pnc.zhengqikj.top

[U29] Py：属性校验
来源：http://edv.jinyuanbaomall.cn

@property 与 @x.setter 配合
来源：http://muj.jlsjyb.cn

[U30] Py：数据类
来源：http://rfa.zhongyouzk.top

@dataclass(slots=True)
来源：http://kow.hnxiangtu.top

[U31] Py：单测
来源：http://slu.tian-w.cn

python -m pytest -q
来源：http://jab.yfazqb.com

[U32] Py：代码格式化
来源：http://nlf.ywan-chungtsiang.top

ruff format . && ruff check --fix .
来源：http://fwx.gotoacloud.top

[U33] Py：打包发布
来源：http://nnk.fengsongda.top

python -m build  （依赖 pyproject.toml）
来源：http://cex.sxryk.cn

[U34] Py：判断编码
来源：http://amu.guannengcc.top

chardet.detect(raw)
来源：http://xdr.cucudq.cn

[U35] Py：发送邮件
来源：http://pbd.vehdjk.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rlx.feifeiyinyue.top

[U36] Py：定时任务
来源：http://hmf.bjfxy.top

schedule.every(10).minutes.do(job)
来源：http://mgj.wangdashe.top

[U37] Py：读写 Excel
来源：http://dvs.hywenlv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://llf.cucudq.cn

[U38] Py：获取脚本所在目录
来源：http://zcg.hcnkem.com

Path(__file__).resolve().parent
来源：http://mzi.quarkkingdee.top

[U39] Py：判断是否在交互环境
来源：http://rin.fehbvm.com

sys.stdout.isatty()
来源：http://slc.yanxiufei.cn

[U40] Py：打印到标准错误
来源：http://osh.nanxinkj.top

print("err", file=sys.stderr)
来源：http://ktc.cashguo.top

[U41] PHP：初始化 Composer 项目
来源：http://hsr.c1oappe.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ehg.zhoulong.xyz

[U42] PHP：PSR-4 自动加载
来源：http://fwa.vqdsnc.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vxi.feifeiyinyue.top

[U43] PHP：声明命名空间
来源：http://tdj.hysaishi.cn

namespace App\Http;
来源：http://qbn.dianchejie.cn

[U44] PHP：开启严格类型
来源：http://smq.yueranfly.top

declare(strict_types=1);
来源：http://nqw.haohaochexian.top

[U45] PHP：类型声明与返回类型
来源：http://kgy.9152youxi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gxt.vehdjk.com

[U46] PHP：可空类型
来源：http://xqp.yj20258888.top

?string $name = null
来源：http://vhy.smart0.xyz

[U47] PHP：联合类型
来源：http://hvo.smart0.xyz

int|string $id
来源：http://mxy.havefunace.top

[U48] PHP：纯枚举
来源：http://fck.tian-w.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bpu.wangdashe.top

[U49] PHP：只读属性
来源：http://flc.shanyushiyangkeji.top

public readonly string $name
来源：http://hoq.xuetiantiany.cn

[U50] PHP：构造器属性提升
来源：http://qqk.cucudq.cn

public function __construct(private int $id) {}
来源：http://srg.sjlbkw.cn

[U51] PHP：数组解构
来源：http://ctg.zhengqikj.top

[$a, $b] = $arr;
来源：http://qcj.vqdsnc.cn

[U52] PHP：箭头函数
来源：http://ryt.chenzaomai.com

$double = fn($x) => $x * 2;
来源：http://wir.redwolf501.top

[U53] PHP：空合并运算符
来源：http://szi.ivvv.top

$v = $a ?? $b ?? "default";
来源：http://vee.cucudq.cn

[U54] PHP：空安全调用
来源：http://wvj.xingfuxueyuan.xyz

$obj?->method()
来源：http://wow.yvedp.cn

[U55] PHP：match 表达式
来源：http://jzs.uphjek.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uqz.yangfankeji.com

[U56] PHP：命名参数
来源：http://fjm.gotoacloud.top

f(a: 1, b: 2)
来源：http://okn.shzxlz.cn

[U57] PHP：字符串插值
来源：http://rtb.ydjk.org.cn

"值: {$a}"
来源：http://ejt.hnqzz.top

[U58] PHP：数组三件套
来源：http://epy.chenzaomai.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xwc.jinqigufen.top

[U59] PHP：自定义排序
来源：http://nhe.tianlin.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wgw.yj202588.top

[U60] PHP：JSON 编解码
来源：http://vla.yuxming.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://llc.fehbvm.com

[U61] PHP：正则
来源：http://lrh.jiagoushi.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mef.haohaochexian.top

[U62] PHP：日期对象
来源：http://aal.yuxming.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ktg.yongpay.top

[U63] PHP：文件读写
来源：http://zxi.hfpthk.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hmz.jyoumei.cn

[U64] PHP：目录遍历
来源：http://qlk.hesvh.cn

glob("dir/*.php");  scandir("dir");
来源：http://ofx.wangdashe.top

[U65] PHP：会话
来源：http://qao.yongpay.top

session_start();  $_SESSION["uid"] = 1;
来源：http://dbx.snrcjt.cn

[U66] PHP：设置 Cookie
来源：http://qul.fktsv.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zfu.0kj1m.cn

[U67] PHP：处理文件上传
来源：http://luy.yj20258.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nog.nwbrower.top

[U68] PHP：PDO 连接
来源：http://gnw.316326.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uxd.pycfn.com

[U69] PHP：PDO 预处理
来源：http://gnh.vehdjk.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lgn.vqdsnc.cn

[U70] PHP：PDO 事务
来源：http://foi.nanxuanxn.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bii.zhaomingkeji.xyz

[U71] PHP：抛出异常
来源：http://sdh.jinqigfzy.top

throw new RuntimeException("失败", 500);
来源：http://wrb.redwolf501.top

[U72] PHP：写错误日志
来源：http://mfn.cashguo.top

error_log("失败: " . $e->getMessage());
来源：http://zmg.epnwcf.com

[U73] PHP：读取 ini 配置
来源：http://web.pycfn.com

parse_ini_file("config.ini", true)
来源：http://rwg.dashuyun.cn

[U74] PHP：读取环境变量
来源：http://gvx.xylfe.cn

getenv("APP_ENV") ?: "production"
来源：http://xye.yfazqb.com

[U75] PHP：依赖注入
来源：http://eox.c1oappe.top

composer require psr/container
来源：http://ppw.hysaishi.cn

[U76] PHP：简单路由
来源：http://iuf.jqgfzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zid.xuetiantiany.cn

[U77] PHP：模板渲染
来源：http://yny.fanxiaobao.xyz

composer require twig/twig
来源：http://xfq.zhiwuduotai.top

[U78] PHP：单元测试
来源：http://phx.chenlongwang.top

composer require --dev phpunit/phpunit
来源：http://omi.jlsjyb.cn

[U79] PHP：静态分析
来源：http://ozc.hesvh.cn

composer require --dev phpstan/phpstan
来源：http://atc.svipenyu.cn

[U80] PHP：代码规范修复
来源：http://eqv.tian-w.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://uzq.hesvh.cn

[U81] JS：初始化项目
来源：http://ise.uphjek.com

npm init -y;  npm i express
来源：http://adf.aibaodan.cn

[U82] JS：package.json 脚本
来源：http://vim.ydjk.org.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://eum.yfazqb.com

[U83] JS：ES Module 导入导出
来源：http://chd.cheryme.top

export const a = 1;  import { a } from "./m.js";
来源：http://oqq.c1oappe.top

[U84] JS：CommonJS 写法
来源：http://ihh.jqgufenzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://djo.zhaomingkeji.xyz

[U85] JS：可选链
来源：http://bef.316326.xyz

a?.b?.c
来源：http://ler.guannengcc.top

[U86] JS：空值合并
来源：http://tzr.vqdsnc.cn

a ?? b
来源：http://vob.haohaochexian.top

[U87] JS：解构默认值
来源：http://icl.jyoumei.cn

const { a = 1, b = 2 } = obj;
来源：http://ojn.yongpay.top

[U88] JS：对象展开合并
来源：http://qrc.jinqigfzy.top

{ ...a, ...b }
来源：http://kfr.tanke756.top

[U89] JS：数组去重
来源：http://ffh.ehwqpu.com

[...new Set(arr)]
来源：http://oih.hcnkem.com

[U90] JS：数字数组排序
来源：http://rhj.shanyushiyangtech.top

[...arr].sort((a, b) => a - b)
来源：http://uar.jiagoushi.top

[U91] JS：对象键值遍历
来源：http://sbo.9152youxi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wdv.xuanzx.com

[U92] JS：深拷贝
来源：http://yul.havefunace.top

structuredClone(obj)
来源：http://lcd.xuanzx.com

[U93] JS：模板字符串
来源：http://aez.vehdjk.com

`共 ${n} 条`
来源：http://bbe.uphjek.com

[U94] JS：箭头函数
来源：http://zdx.fktsv.cn

const double = x => x * 2;
来源：http://gvf.jiagoushi.top

[U95] JS：Promise 包装
来源：http://rip.cashguo.top

new Promise((resolve, reject) => {})
来源：http://kst.yonumen.top

[U96] JS：async/await 与异常
来源：http://adz.ctjpmb.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pdi.hysaishi.cn

[U97] JS：并发请求
来源：http://zpv.tianlin.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://dcw.sxryk.cn

[U98] JS：fetch 带 JSON
来源：http://yqu.dashuyun.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lys.yonumen.top

[U99] JS：事件监听
来源：http://qoj.vqdsnc.cn

el.addEventListener("click", e => {})
来源：http://zrx.xinyue.icu

[U100] JS：DOM 查询
来源：http://ryf.jqgufenzy.top

document.querySelector(".item")
来源：http://xpo.yonumen.top

[U101] JS：classList 操作
来源：http://oxg.shangyingyoupin.top

el.classList.toggle("active")
来源：http://aun.svipenyu.cn

[U102] JS：本地存储
来源：http://lru.wangdashe.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://anf.gzhubu.top

[U103] JS：定时器
来源：http://lqb.yanxiufei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kkc.pycfn.com

[U104] JS：防抖
来源：http://bpb.hesvh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://etv.yonumen.top

[U105] JS：节流
来源：http://lqi.jianghu66.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dso.tarul.cn

[U106] JS：日期格式化
来源：http://cux.zhiwuduotai.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gdh.nanxinkj.top

[U107] JS：数字千分位
来源：http://ugn.jianghu66.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ukb.zhiwuduotai.top

[U108] JS：随机整数
来源：http://cey.gogol.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vrf.jinyuanbaomall.cn

[U109] JS：数组分组
来源：http://qae.ehwqpu.com

Object.groupBy(arr, x => x.type)
来源：http://dic.cdnleiting.top

[U110] JS：数组分块
来源：http://fjp.guannengcc.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://glo.gzhubu.top

[U111] JS：对象转 Map
来源：http://qtn.zhaomingkeji.xyz

new Map(Object.entries(obj))
来源：http://vsa.cucudq.cn

[U112] JS：字符串补位
来源：http://moh.shuidangran.top

"7".padStart(3, "0")
来源：http://nbr.epnwcf.com

[U113] JS：正则替换全部
来源：http://ypg.hcnkem.com

s.replaceAll("a", "b")
来源：http://ohh.hnqzz.top

[U114] JS：JSON 深比较
来源：http://rmz.yj20258888.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://rhn.birdmap.top

[U115] JS：生成 UUID
来源：http://roo.zhixingplan.top

crypto.randomUUID()
来源：http://cie.xylfe.cn

[U116] JS：类型检查（JSDoc）
来源：http://nzq.havefunace.top

/** @param {string} name */ function f(name) {}
来源：http://azl.zycfv.cn

[U117] JS：单元测试
来源：http://iyq.mhx1999.top

npm i -D vitest;  npx vitest
来源：http://itl.bjfxy.top

[U118] JS：开发服务器
来源：http://kai.xziqi.cn

npm i -D vite;  npx vite
来源：http://eal.snrcjt.cn

[U119] JS：生产构建
来源：http://ypo.chenlongwang.top

npx vite build
来源：http://dlx.chenjidiqi.icu

[U120] JS：读取环境变量（Vite）
来源：http://vsp.zhiwuduotai.top

import.meta.env.VITE_API_URL
来源：http://pkh.jinqigufen.top

================================================================================
来源：http://xpw.gogol.net.cn

统计汇总
来源：http://ask.shanyushiyangtech.top

================================================================================
来源：http://kis.cqqwz.cn

按语言统计（条）：
来源：http://cvg.zhixingplan.top

Python ......... 252
来源：http://bxs.guannengcc.top

PHP ............ 252
来源：http://src.uphjek.com

JavaScript ..... 252
来源：http://phc.jyoumei.cn

TypeScript ..... 212
来源：http://dtr.shanyushiyangtech.top

Java ........... 212
来源：http://uvm.fehbvm.com

Go ............. 212
来源：http://vhb.xinyue.icu

Ruby ........... 212
来源：http://fop.hywenlv.cn

C# ............. 212
来源：http://jho.gaohongyu789.top

C .............. 30
来源：http://upw.tian-w.cn

C++ ............ 30
来源：http://sfw.guannengcc.top

SQL ............ 90
来源：http://eid.yj20258888.top

Bash ........... 80
来源：http://qoq.sysykeji.top

Kotlin ......... 15
来源：http://pdh.fanxiaobao.xyz

Swift .......... 15
来源：http://jiu.yj202588.top

Lua ............ 10
来源：http://frb.sjlbkw.cn

Perl ........... 10
来源：http://exv.ydjk.org.cn

Scala .......... 10
来源：http://tca.shuidangran.top

------------------------------------
来源：http://zyf.sweek.top

合计 ........... 2106 条
来源：http://ske.sweek.top

按章节统计：
来源：http://gqe.daxiang520.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ucm.dashuyun.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://clx.sxryk.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://iyu.tian-w.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://esy.gogol.net.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wcp.yangfankeji.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://emq.aibaodan.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ytq.xuetiantiany.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lyc.316326.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zwt.dashuyun.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dbm.tarul.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://txg.dianchejie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vyc.zhengqikj.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ghm.yueranfly.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xjp.chenjidiqi.icu

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yda.tanke756.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://gzc.bbcook.cn

Q SQL 专题                              90
来源：http://roy.52xcode.cn

R Bash 专题                             80
来源：http://vfo.cheryme.top

S C / C++ 专题                          60
来源：http://dsp.zycfv.cn

T 其他语言补充                          60
来源：http://qkc.hongshengwenyu.top

U 高频实用片段                         120
来源：http://fll.zhoulong.xyz

------------------------------------
来源：http://nkg.ybcxt.top

合计                                  2106 条
来源：http://cju.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://dox.cucudq.cn

使用提醒
来源：http://zbt.tarul.cn

--------------------------------------------------------------------------------
来源：http://tpk.yueranfly.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tfk.snrcjt.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xcc.yangfankeji.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wst.sysykeji.top

在旧版本上使用前请先确认语法支持情况。
来源：http://rou.zhaomingkeji.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hsf.cqqwz.cn

—— 文件结束 ——
来源：http://ahu.xylfe.cn

================================================================================
来源：http://bmp.yueranfly.top

程序语言常见例子速查手册（2024 版）
来源：http://bft.vqdsnc.cn

Common Programming Examples Cheat Book
来源：http://rew.ydjk.org.cn

================================================================================
来源：http://dww.yueranfly.top

【收录内容】
来源：http://owp.xuetiantiany.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ozo.yfazqb.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://has.xziqi.cn

SQL · Bash · C · C++
来源：http://gjw.hysaishi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ejd.wangdashe.top

【使用说明】
来源：http://kwa.zhengqikj.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cid.c1oappe.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ops.jinghuilouyu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ikh.yuanzhike.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gle.sufxvd.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://oca.yj20258.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://iap.shzxlz.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gep.hnxiangtu.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xza.shuidangran.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ycv.ehwqpu.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tmi.guowangkeji.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dqr.iojbl.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pwy.nanxuanxn.top

【文件统计】
来源：http://yxs.yvedp.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pbo.zhixingplan.top

--------------------------------------------------------------------------------
来源：http://xmr.hcnkem.com

目  录
来源：http://wbo.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://sgc.316326.xyz

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nty.zdbjq.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dut.ydjk.org.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pno.hywenlv.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kkd.tian-w.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://oib.zdqjudy.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bti.svipenyu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xwc.chenlongwang.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://jvq.hnxiangtu.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cau.hfpthk.cn


<!-- 参考信息 -->