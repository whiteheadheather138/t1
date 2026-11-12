代发 wailian999

[U07] Py：反转字典键值
来源：http://cue.gogol.net.cn

{v: k for k, v in d.items()}
来源：http://nbj.yuxming.cn

[U08] Py：展平二维列表
来源：http://wtw.52xcode.cn

[y for x in nested for y in x]
来源：http://taw.vehdjk.com

[U09] Py：字典取最大值的键
来源：http://pqv.cheryme.top

max(d, key=d.get)
来源：http://jdc.tianlin.xyz

[U10] Py：按值排序字典
来源：http://yuf.dianchejie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bcp.yuanzhike.top

[U11] Py：生成器表达式
来源：http://bwy.cucudq.cn

(x * 2 for x in arr)
来源：http://lek.xuanzx.com

[U12] Py：取出现最多的 3 个元素
来源：http://rjw.jinqigfzy.top

Counter(arr).most_common(3)
来源：http://vvd.zdqjudy.top

[U13] Py：固定长度队列
来源：http://fjh.jinqigufen.top

deque(maxlen=10)
来源：http://pqs.jinghuilouyu.cn

[U14] Py：分组收集到列表
来源：http://tfd.feifeiyinyue.top

defaultdict(list)
来源：http://uiv.guowangkeji.top

[U15] Py：高精度计时
来源：http://miq.dianchejie.cn

t = time.perf_counter()
来源：http://ibe.wangdashe.top

[U16] Py：命令行参数解析
来源：http://ero.zhongyouzk.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://iea.ybcxt.top

[U17] Py：初始化日志
来源：http://yws.tian-w.cn

logging.basicConfig(level=logging.INFO)
来源：http://acp.chenlongwang.top

[U18] Py：预编译正则
来源：http://nmv.shzxlz.cn

pat = re.compile(r"\d+")
来源：http://kpy.tarul.cn

[U19] Py：正则替换带回调
来源：http://dje.redwolf501.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ify.svipenyu.cn

[U20] Py：缓存函数结果
来源：http://jkj.jinghuilouyu.cn

@functools.lru_cache(maxsize=None)
来源：http://llc.hnqzz.top

[U21] Py：自定义上下文管理器
来源：http://fwk.jiagoushi.top

@contextlib.contextmanager
来源：http://qhd.jinyuanbaomall.cn

[U22] Py：矩阵转置
来源：http://psy.shangyingyoupin.top

list(zip(*m))
来源：http://rtp.yj20258888.top

[U23] Py：分块读取大文件
来源：http://zvg.ydzc1.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pml.yonumen.top

[U24] Py：路径操作
来源：http://gvj.jianghu66.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tvv.aibaodan.cn

[U25] Py：CSV 按字典读
来源：http://bds.sjlbkw.cn

csv.DictReader(f)
来源：http://ixy.hnqzz.top

[U26] Py：并发下载
来源：http://gfp.yonumen.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nmp.kuanghao11.cn

[U27] Py：异步 HTTP
来源：http://ycl.yj20258.top

aiohttp.ClientSession() 配合 async with
来源：http://pkp.daria6918.cn

[U28] Py：类型别名
来源：http://pdj.hongshengwenyu.top

UserId = int
来源：http://elv.guannengcc.top

[U29] Py：属性校验
来源：http://fmf.shangyingyoupin.top

@property 与 @x.setter 配合
来源：http://ayy.gaohongyu789.top

[U30] Py：数据类
来源：http://ctx.zhijiandao.cn

@dataclass(slots=True)
来源：http://bdh.chenlongwang.top

[U31] Py：单测
来源：http://kil.shangyingyoupin.top

python -m pytest -q
来源：http://gad.xinyue.icu

[U32] Py：代码格式化
来源：http://sjl.0kj1m.cn

ruff format . && ruff check --fix .
来源：http://mdi.dashuyun.cn

[U33] Py：打包发布
来源：http://lxk.yanxiufei.cn

python -m build  （依赖 pyproject.toml）
来源：http://jnf.wangdashe.top

[U34] Py：判断编码
来源：http://ogz.xylfe.cn

chardet.detect(raw)
来源：http://fth.snrcjt.cn

[U35] Py：发送邮件
来源：http://mxr.aizwys.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://czn.dianchejie.cn

[U36] Py：定时任务
来源：http://lwx.guowangkeji.top

schedule.every(10).minutes.do(job)
来源：http://cjx.jinyuanbaomall.cn

[U37] Py：读写 Excel
来源：http://ane.daria6918.cn

pandas.read_excel / DataFrame.to_excel
来源：http://dsn.xingfuxueyuan.xyz

[U38] Py：获取脚本所在目录
来源：http://bcg.yanxiufei.cn

Path(__file__).resolve().parent
来源：http://gwm.nwbrower.top

[U39] Py：判断是否在交互环境
来源：http://ttq.aibaodan.cn

sys.stdout.isatty()
来源：http://qhr.ppjwa.cn

[U40] Py：打印到标准错误
来源：http://oqg.ctjpmb.com

print("err", file=sys.stderr)
来源：http://fph.zhiwuduotai.top

[U41] PHP：初始化 Composer 项目
来源：http://fjm.hnqzz.top

composer init;  composer require guzzlehttp/guzzle
来源：http://sbd.feifeiyinyue.top

[U42] PHP：PSR-4 自动加载
来源：http://sdt.shuidangran.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rpd.tanke756.top

[U43] PHP：声明命名空间
来源：http://mhy.epnwcf.com

namespace App\Http;
来源：http://rwk.andypj.xyz

[U44] PHP：开启严格类型
来源：http://gzv.sxryk.cn

declare(strict_types=1);
来源：http://ale.zhoulong.xyz

[U45] PHP：类型声明与返回类型
来源：http://xhl.shzxlz.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://oql.nanxinkj.top

[U46] PHP：可空类型
来源：http://lyc.andypj.xyz

?string $name = null
来源：http://pso.xinyue.icu

[U47] PHP：联合类型
来源：http://knb.xuanzx.com

int|string $id
来源：http://amc.ivvv.top

[U48] PHP：纯枚举
来源：http://qfo.havefunace.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nmj.cucudq.cn

[U49] PHP：只读属性
来源：http://vnj.xingfuxueyuan.xyz

public readonly string $name
来源：http://zub.fktsv.cn

[U50] PHP：构造器属性提升
来源：http://cxf.yj20258.top

public function __construct(private int $id) {}
来源：http://hmh.vehdjk.com

[U51] PHP：数组解构
来源：http://orj.vqdsnc.cn

[$a, $b] = $arr;
来源：http://pny.shzxlz.cn

[U52] PHP：箭头函数
来源：http://dbc.cqqwz.cn

$double = fn($x) => $x * 2;
来源：http://nqb.yuanzhike.top

[U53] PHP：空合并运算符
来源：http://lke.tanke756.top

$v = $a ?? $b ?? "default";
来源：http://ibz.chenjidiqi.icu

[U54] PHP：空安全调用
来源：http://miq.iojbl.cn

$obj?->method()
来源：http://qmn.cqqwz.cn

[U55] PHP：match 表达式
来源：http://pss.cheryme.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://abe.ctjpmb.com

[U56] PHP：命名参数
来源：http://jdx.cqqwz.cn

f(a: 1, b: 2)
来源：http://bps.dianchejie.cn

[U57] PHP：字符串插值
来源：http://fwg.shanyushiyangtech.top

"值: {$a}"
来源：http://kzj.ydzc1.top

[U58] PHP：数组三件套
来源：http://qwq.zhaomingkeji.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://brs.jinqigfzy.top

[U59] PHP：自定义排序
来源：http://fgh.svipenyu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qvi.cqqwz.cn

[U60] PHP：JSON 编解码
来源：http://cop.ivvv.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sua.jyoumei.cn

[U61] PHP：正则
来源：http://ujl.jqgufenzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kla.gzhubu.top

[U62] PHP：日期对象
来源：http://amu.hnqzz.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cws.jianghu66.top

[U63] PHP：文件读写
来源：http://msv.chenlongwang.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tzk.hesvh.cn

[U64] PHP：目录遍历
来源：http://xzb.shuidangran.top

glob("dir/*.php");  scandir("dir");
来源：http://shx.jqgfzy.top

[U65] PHP：会话
来源：http://rqz.wangdashe.top

session_start();  $_SESSION["uid"] = 1;
来源：http://pqm.ydjk.org.cn

[U66] PHP：设置 Cookie
来源：http://mjp.pengpengdd.cyou

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://osk.zdqjudy.top

[U67] PHP：处理文件上传
来源：http://oyd.shzxlz.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qef.guannengcc.top

[U68] PHP：PDO 连接
来源：http://aol.xylfe.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rjc.ehwqpu.com

[U69] PHP：PDO 预处理
来源：http://pgd.chenzaomai.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ytx.zhixingplan.top

[U70] PHP：PDO 事务
来源：http://smg.hnxiangtu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://slw.jinqigufen.top

[U71] PHP：抛出异常
来源：http://bpo.xuetiantiany.cn

throw new RuntimeException("失败", 500);
来源：http://reu.xziqi.cn

[U72] PHP：写错误日志
来源：http://hek.xuanzx.com

error_log("失败: " . $e->getMessage());
来源：http://acl.shuidangran.top

[U73] PHP：读取 ini 配置
来源：http://qyq.yj20258888.top

parse_ini_file("config.ini", true)
来源：http://eup.ywan-chungtsiang.top

[U74] PHP：读取环境变量
来源：http://zff.hesvh.cn

getenv("APP_ENV") ?: "production"
来源：http://fph.epnwcf.com

[U75] PHP：依赖注入
来源：http://lrz.cheryme.top

composer require psr/container
来源：http://ilq.nwbrower.top

[U76] PHP：简单路由
来源：http://thu.shangyingyoupin.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cvp.cucudq.cn

[U77] PHP：模板渲染
来源：http://rdg.yj20258888.top

composer require twig/twig
来源：http://wev.hnxiangtu.top

[U78] PHP：单元测试
来源：http://oeh.yuanzhike.top

composer require --dev phpunit/phpunit
来源：http://ijp.chenlongwang.top

[U79] PHP：静态分析
来源：http://iss.pengpengdd.cyou

composer require --dev phpstan/phpstan
来源：http://kta.sweek.top

[U80] PHP：代码规范修复
来源：http://vzc.c1oappe.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://mol.tarul.cn

[U81] JS：初始化项目
来源：http://msk.daria6918.cn

npm init -y;  npm i express
来源：http://drp.jinyuanbaomall.cn

[U82] JS：package.json 脚本
来源：http://nlu.ybcxt.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pct.chenjidiqi.icu

[U83] JS：ES Module 导入导出
来源：http://txz.ivvv.top

export const a = 1;  import { a } from "./m.js";
来源：http://ymq.hfpthk.cn

[U84] JS：CommonJS 写法
来源：http://ldn.zhengqikj.top

module.exports = { a };  const { a } = require("./m");
来源：http://iqh.andypj.xyz

[U85] JS：可选链
来源：http://iii.cdnleiting.top

a?.b?.c
来源：http://hsc.xuanzx.com

[U86] JS：空值合并
来源：http://tmv.hongshengwenyu.top

a ?? b
来源：http://biu.sufxvd.cn

[U87] JS：解构默认值
来源：http://unl.sxryk.cn

const { a = 1, b = 2 } = obj;
来源：http://cqv.shanyushiyangkeji.top

[U88] JS：对象展开合并
来源：http://xah.cheryme.top

{ ...a, ...b }
来源：http://hax.fehbvm.com

[U89] JS：数组去重
来源：http://uxs.aibaodan.cn

[...new Set(arr)]
来源：http://inz.zhixingplan.top

[U90] JS：数字数组排序
来源：http://gwd.redwolf501.top

[...arr].sort((a, b) => a - b)
来源：http://sgp.zycfv.cn

[U91] JS：对象键值遍历
来源：http://smw.snrcjt.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hvy.52xcode.cn

[U92] JS：深拷贝
来源：http://jjc.bjfxy.top

structuredClone(obj)
来源：http://jxu.zhiwuduotai.top

[U93] JS：模板字符串
来源：http://dcm.gzhubu.top

`共 ${n} 条`
来源：http://joj.fanxiaobao.xyz

[U94] JS：箭头函数
来源：http://dxi.chenjidiqi.icu

const double = x => x * 2;
来源：http://fkx.yuanzhike.top

[U95] JS：Promise 包装
来源：http://pxz.wangdashe.top

new Promise((resolve, reject) => {})
来源：http://tis.jinghuilouyu.cn

[U96] JS：async/await 与异常
来源：http://svf.yuxming.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tur.nanxuanxn.top

[U97] JS：并发请求
来源：http://drg.jqgufenzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://irj.kuanghao11.cn

[U98] JS：fetch 带 JSON
来源：http://tnl.hfpthk.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://clu.aibaodan.cn

[U99] JS：事件监听
来源：http://wwj.hcnkem.com

el.addEventListener("click", e => {})
来源：http://lvc.jyoumei.cn

[U100] JS：DOM 查询
来源：http://qxp.vehdjk.com

document.querySelector(".item")
来源：http://sib.smart0.xyz

[U101] JS：classList 操作
来源：http://oed.c1oappe.top

el.classList.toggle("active")
来源：http://aih.52xcode.cn

[U102] JS：本地存储
来源：http://xii.pengpengdd.cyou

localStorage.setItem("k", JSON.stringify(v))
来源：http://yxh.bjfxy.top

[U103] JS：定时器
来源：http://fnc.jianghu66.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vjn.gaohongyu789.top

[U104] JS：防抖
来源：http://hym.yvedp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hbg.fanxiaobao.xyz

[U105] JS：节流
来源：http://egc.zhongyouzk.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://icr.gotoacloud.top

[U106] JS：日期格式化
来源：http://xdo.jyoumei.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lpz.c1oappe.top

[U107] JS：数字千分位
来源：http://xhj.sufxvd.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zow.jinyuanbaomall.cn

[U108] JS：随机整数
来源：http://xhs.nanxuanxn.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ubl.fktsv.cn

[U109] JS：数组分组
来源：http://bze.fzhhl.top

Object.groupBy(arr, x => x.type)
来源：http://cyr.yuanzhike.top

[U110] JS：数组分块
来源：http://vkw.vqdsnc.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pbd.ybcxt.top

[U111] JS：对象转 Map
来源：http://ytw.fehbvm.com

new Map(Object.entries(obj))
来源：http://jam.daria6918.cn

[U112] JS：字符串补位
来源：http://vnf.hcnkem.com

"7".padStart(3, "0")
来源：http://zvy.zhengqikj.top

[U113] JS：正则替换全部
来源：http://see.haohaochexian.top

s.replaceAll("a", "b")
来源：http://yeu.jqgfzy.top

[U114] JS：JSON 深比较
来源：http://sqm.fehbvm.com

JSON.stringify(a) === JSON.stringify(b)
来源：http://gsh.pycfn.com

[U115] JS：生成 UUID
来源：http://xij.shuidangran.top

crypto.randomUUID()
来源：http://nse.sysykeji.top

[U116] JS：类型检查（JSDoc）
来源：http://xir.shzxlz.cn

/** @param {string} name */ function f(name) {}
来源：http://wwr.xuetiantiany.cn

[U117] JS：单元测试
来源：http://ciw.ehwqpu.com

npm i -D vitest;  npx vitest
来源：http://kvs.vqdsnc.cn

[U118] JS：开发服务器
来源：http://huj.guowangkeji.top

npm i -D vite;  npx vite
来源：http://wsf.cashguo.top

[U119] JS：生产构建
来源：http://kmz.yvedp.cn

npx vite build
来源：http://eia.xziqi.cn

[U120] JS：读取环境变量（Vite）
来源：http://krr.yuanzhike.top

import.meta.env.VITE_API_URL
来源：http://wqk.yonumen.top

================================================================================
来源：http://hgg.xylfe.cn

统计汇总
来源：http://wts.zhiwuduotai.top

================================================================================
来源：http://wcp.uphjek.com

按语言统计（条）：
来源：http://qho.ywan-chungtsiang.top

Python ......... 252
来源：http://aea.chenlongwang.top

PHP ............ 252
来源：http://qpd.cashguo.top

JavaScript ..... 252
来源：http://wbu.ywan-chungtsiang.top

TypeScript ..... 212
来源：http://wsn.iojbl.cn

Java ........... 212
来源：http://svt.jqgfzy.top

Go ............. 212
来源：http://oct.kuanghao11.cn

Ruby ........... 212
来源：http://jby.wangshuangyany.cn

C# ............. 212
来源：http://qlg.bbcook.cn

C .............. 30
来源：http://qir.mhx1999.top

C++ ............ 30
来源：http://rao.zhijiandao.cn

SQL ............ 90
来源：http://abj.tian-w.cn

Bash ........... 80
来源：http://ejn.52xcode.cn

Kotlin ......... 15
来源：http://acw.gogol.net.cn

Swift .......... 15
来源：http://eqp.meibo888.top

Lua ............ 10
来源：http://cij.birdmap.top

Perl ........... 10
来源：http://zva.birdmap.top

Scala .......... 10
来源：http://ieu.hywenlv.cn

------------------------------------
来源：http://agd.bjfxy.top

合计 ........... 2106 条
来源：http://jgf.jlsjyb.cn

按章节统计：
来源：http://dyf.yonumen.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://crj.aizwys.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ima.cdnleiting.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://thf.guowangkeji.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hxy.fzhhl.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zlo.ctjpmb.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cdq.cucudq.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ftl.zhaomingkeji.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://knw.jqgfzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ukd.nanxuanxn.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cgz.kuanghao11.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qlj.fanxiaobao.xyz

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fnp.cashguo.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dlf.aibaodan.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wob.jqgfzy.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ixj.hesvh.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://uhx.sjlbkw.cn

Q SQL 专题                              90
来源：http://nnn.cqqwz.cn

R Bash 专题                             80
来源：http://yqw.kuanghao11.cn

S C / C++ 专题                          60
来源：http://sir.gaohongyu789.top

T 其他语言补充                          60
来源：http://qlv.daria6918.cn

U 高频实用片段                         120
来源：http://wiz.zhaomingkeji.xyz

------------------------------------
来源：http://bed.fzhhl.top

合计                                  2106 条
来源：http://dqz.jqgfzy.top

--------------------------------------------------------------------------------
来源：http://jaq.zhiwuduotai.top

使用提醒
来源：http://fdm.ehwqpu.com

--------------------------------------------------------------------------------
来源：http://wis.hysaishi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xge.andypj.xyz

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bnz.yongpay.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jbs.nwbrower.top

在旧版本上使用前请先确认语法支持情况。
来源：http://fem.tarul.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hph.nanxinkj.top

—— 文件结束 ——
来源：http://mui.tianlin.xyz

================================================================================
来源：http://ekr.quarkkingdee.top

程序语言常见例子速查手册（2024 版）
来源：http://yuy.fzhhl.top

Common Programming Examples Cheat Book
来源：http://kel.zhoulong.xyz

================================================================================
来源：http://olu.cqqwz.cn

【收录内容】
来源：http://adu.aibaodan.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ilj.zdqjudy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tph.ehwqpu.com

SQL · Bash · C · C++
来源：http://bdx.aibaodan.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cnr.dashuyun.cn

【使用说明】
来源：http://wzd.ywan-chungtsiang.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mjh.nanxinkj.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nhh.jinghuilouyu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xhz.sjlbkw.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://osb.gogol.net.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rjh.daxiang520.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wnh.hammf.cn


<!-- 参考信息 -->