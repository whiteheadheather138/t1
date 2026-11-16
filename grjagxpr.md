代发 wailian999

case class User(name: String, age: Int)
来源：http://eim.tian-w.cn

[T57] Scala：模式匹配
来源：http://vyh.9152youxi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sbw.hnxiangtu.top

[T58] Scala：函数定义
来源：http://qko.guannengcc.top

def add(a: Int, b: Int): Int = a + b
来源：http://syw.jinqigufen.top

[T59] Scala：循环
来源：http://lir.xziqi.cn

for (i <- 1 to 10) println(i)
来源：http://cwa.ctjpmb.com

[T60] Scala：折叠
来源：http://cix.c1oappe.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tfo.fktsv.cn

================================================================================
来源：http://nig.zdbjq.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ucr.hesvh.cn

================================================================================
来源：http://emj.iojbl.cn

[U01] Py：创建虚拟环境
来源：http://rqc.guannengcc.top

python -m venv .venv && source .venv/bin/activate
来源：http://tnq.zhijiandao.cn

[U02] Py：导出 / 安装依赖
来源：http://qxk.fengsongda.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vaf.ydjk.org.cn

[U03] Py：加载 .env 配置
来源：http://xiu.chenlongwang.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ksy.c1oappe.top

[U04] Py：变量调试打印
来源：http://cez.chenjidiqi.icu

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://whc.xinyue.icu

[U05] Py：列表去重且保序
来源：http://rlo.kuanghao11.cn

list(dict.fromkeys(arr))
来源：http://iuf.yj20258888.top

[U06] Py：合并两个字典
来源：http://qoq.xinyue.icu

{**a, **b}
来源：http://zot.zycfv.cn

[U07] Py：反转字典键值
来源：http://hqg.jinghuilouyu.cn

{v: k for k, v in d.items()}
来源：http://ona.ydzc1.top

[U08] Py：展平二维列表
来源：http://yks.yueranfly.top

[y for x in nested for y in x]
来源：http://lur.yueranfly.top

[U09] Py：字典取最大值的键
来源：http://jrl.feifeiyinyue.top

max(d, key=d.get)
来源：http://zee.hammf.cn

[U10] Py：按值排序字典
来源：http://lqc.jinghuilouyu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://trv.ybcxt.top

[U11] Py：生成器表达式
来源：http://bzy.hnqzz.top

(x * 2 for x in arr)
来源：http://yya.zycfv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qle.smart0.xyz

Counter(arr).most_common(3)
来源：http://cwk.ybcxt.top

[U13] Py：固定长度队列
来源：http://tko.guowangkeji.top

deque(maxlen=10)
来源：http://jfh.yj20258.top

[U14] Py：分组收集到列表
来源：http://lhq.sjlbkw.cn

defaultdict(list)
来源：http://zsr.fanxiaobao.xyz

[U15] Py：高精度计时
来源：http://pec.ppjwa.cn

t = time.perf_counter()
来源：http://ito.sxryk.cn

[U16] Py：命令行参数解析
来源：http://whq.jinqigufen.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://phb.chenjidiqi.icu

[U17] Py：初始化日志
来源：http://bll.cheryme.top

logging.basicConfig(level=logging.INFO)
来源：http://exp.bbcook.cn

[U18] Py：预编译正则
来源：http://phn.feifeiyinyue.top

pat = re.compile(r"\d+")
来源：http://ejp.jianghu66.top

[U19] Py：正则替换带回调
来源：http://fob.ctjpmb.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lzu.jianghu66.top

[U20] Py：缓存函数结果
来源：http://yzl.aizwys.cn

@functools.lru_cache(maxsize=None)
来源：http://hni.dianchejie.cn

[U21] Py：自定义上下文管理器
来源：http://oki.chenlongwang.top

@contextlib.contextmanager
来源：http://cez.sysykeji.top

[U22] Py：矩阵转置
来源：http://gcw.zhengqikj.top

list(zip(*m))
来源：http://uwp.guannengcc.top

[U23] Py：分块读取大文件
来源：http://ygp.jinqigfzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vwp.chenjidiqi.icu

[U24] Py：路径操作
来源：http://sru.smart0.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://old.quarkkingdee.top

[U25] Py：CSV 按字典读
来源：http://pba.xuetiantiany.cn

csv.DictReader(f)
来源：http://xsp.sjlbkw.cn

[U26] Py：并发下载
来源：http://ddn.cucudq.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ybr.yj20258888.top

[U27] Py：异步 HTTP
来源：http://ijo.jyoumei.cn

aiohttp.ClientSession() 配合 async with
来源：http://ijq.sweek.top

[U28] Py：类型别名
来源：http://vje.iojbl.cn

UserId = int
来源：http://jgw.redwolf501.top

[U29] Py：属性校验
来源：http://asf.cheryme.top

@property 与 @x.setter 配合
来源：http://uqz.bjfxy.top

[U30] Py：数据类
来源：http://ifa.feifeiyinyue.top

@dataclass(slots=True)
来源：http://cyr.zdqjudy.top

[U31] Py：单测
来源：http://ecz.andypj.xyz

python -m pytest -q
来源：http://ipc.sufxvd.cn

[U32] Py：代码格式化
来源：http://gsn.zhaomingkeji.xyz

ruff format . && ruff check --fix .
来源：http://lam.316326.xyz

[U33] Py：打包发布
来源：http://gir.zhiwuduotai.top

python -m build  （依赖 pyproject.toml）
来源：http://sxz.nanxinkj.top

[U34] Py：判断编码
来源：http://biw.dashuyun.cn

chardet.detect(raw)
来源：http://sdb.jqgfzy.top

[U35] Py：发送邮件
来源：http://wyt.meibo888.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://afk.yuanzhike.top

[U36] Py：定时任务
来源：http://gai.cheryme.top

schedule.every(10).minutes.do(job)
来源：http://hgc.haohaochexian.top

[U37] Py：读写 Excel
来源：http://umq.jinqigufen.top

pandas.read_excel / DataFrame.to_excel
来源：http://cyj.jinqigufen.top

[U38] Py：获取脚本所在目录
来源：http://ugc.guowangkeji.top

Path(__file__).resolve().parent
来源：http://nvj.pycfn.com

[U39] Py：判断是否在交互环境
来源：http://cfc.aibaodan.cn

sys.stdout.isatty()
来源：http://uji.zdqjudy.top

[U40] Py：打印到标准错误
来源：http://ltf.yj202588.top

print("err", file=sys.stderr)
来源：http://xvh.dianchejie.cn

[U41] PHP：初始化 Composer 项目
来源：http://oxh.tianlin.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://ver.aibaodan.cn

[U42] PHP：PSR-4 自动加载
来源：http://hpa.shanyushiyangtech.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://znm.guannengcc.top

[U43] PHP：声明命名空间
来源：http://tyt.yongpay.top

namespace App\Http;
来源：http://hsf.aizwys.cn

[U44] PHP：开启严格类型
来源：http://hkx.chenjidiqi.icu

declare(strict_types=1);
来源：http://xcr.shuidangran.top

[U45] PHP：类型声明与返回类型
来源：http://hvr.havefunace.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ruw.guowangkeji.top

[U46] PHP：可空类型
来源：http://wel.guannengcc.top

?string $name = null
来源：http://oco.zdbjq.cn

[U47] PHP：联合类型
来源：http://pnh.pycfn.com

int|string $id
来源：http://mtt.fehbvm.com

[U48] PHP：纯枚举
来源：http://ezr.haohaochexian.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ffi.yueranfly.top

[U49] PHP：只读属性
来源：http://veg.xuetiantiany.cn

public readonly string $name
来源：http://rsc.dianchejie.cn

[U50] PHP：构造器属性提升
来源：http://qzx.zdqjudy.top

public function __construct(private int $id) {}
来源：http://blw.zycfv.cn

[U51] PHP：数组解构
来源：http://jfl.ydzc1.top

[$a, $b] = $arr;
来源：http://zgo.gzhubu.top

[U52] PHP：箭头函数
来源：http://qtn.daria6918.cn

$double = fn($x) => $x * 2;
来源：http://ura.xziqi.cn

[U53] PHP：空合并运算符
来源：http://ibg.zdbjq.cn

$v = $a ?? $b ?? "default";
来源：http://lfr.tianlin.xyz

[U54] PHP：空安全调用
来源：http://byr.epnwcf.com

$obj?->method()
来源：http://nei.sufxvd.cn

[U55] PHP：match 表达式
来源：http://pce.aizwys.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://puu.zhoulong.xyz

[U56] PHP：命名参数
来源：http://bkc.jinqigfzy.top

f(a: 1, b: 2)
来源：http://kdk.xuanzx.com

[U57] PHP：字符串插值
来源：http://bgy.zhengqikj.top

"值: {$a}"
来源：http://rka.shzxlz.cn

[U58] PHP：数组三件套
来源：http://tak.jianghu66.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://foz.hesvh.cn

[U59] PHP：自定义排序
来源：http://xxt.yj202588.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xib.sweek.top

[U60] PHP：JSON 编解码
来源：http://gzu.tianlin.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fvm.shanyushiyangkeji.top

[U61] PHP：正则
来源：http://zyd.yvedp.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fbb.fehbvm.com

[U62] PHP：日期对象
来源：http://omk.yvedp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ohk.snrcjt.cn

[U63] PHP：文件读写
来源：http://vso.shzxlz.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sbv.jianghu66.top

[U64] PHP：目录遍历
来源：http://xzk.hesvh.cn

glob("dir/*.php");  scandir("dir");
来源：http://huy.bjfxy.top

[U65] PHP：会话
来源：http://ryt.andypj.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://fbc.yj202588.top

[U66] PHP：设置 Cookie
来源：http://zpd.kuanghao11.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kfr.yfazqb.com

[U67] PHP：处理文件上传
来源：http://qvs.fehbvm.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ydv.snrcjt.cn

[U68] PHP：PDO 连接
来源：http://she.zdqjudy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pzk.0kj1m.cn

[U69] PHP：PDO 预处理
来源：http://qpz.gaohongyu789.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fxv.sjlbkw.cn

[U70] PHP：PDO 事务
来源：http://rza.yfazqb.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://omx.ydjk.org.cn

[U71] PHP：抛出异常
来源：http://bzf.jinyuanbaomall.cn

throw new RuntimeException("失败", 500);
来源：http://pnu.feifeiyinyue.top

[U72] PHP：写错误日志
来源：http://euj.jlsjyb.cn

error_log("失败: " . $e->getMessage());
来源：http://gkq.0kj1m.cn

[U73] PHP：读取 ini 配置
来源：http://fns.yvedp.cn

parse_ini_file("config.ini", true)
来源：http://lgo.haohaochexian.top

[U74] PHP：读取环境变量
来源：http://uze.ivvv.top

getenv("APP_ENV") ?: "production"
来源：http://niw.xingfuxueyuan.xyz

[U75] PHP：依赖注入
来源：http://fgi.aibaodan.cn

composer require psr/container
来源：http://vpv.zhijiandao.cn

[U76] PHP：简单路由
来源：http://orm.jqgufenzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bge.feifeiyinyue.top

[U77] PHP：模板渲染
来源：http://lec.sjlbkw.cn

composer require twig/twig
来源：http://kay.jlsjyb.cn

[U78] PHP：单元测试
来源：http://bcl.feifeiyinyue.top

composer require --dev phpunit/phpunit
来源：http://jzg.pycfn.com

[U79] PHP：静态分析
来源：http://dde.shangyingyoupin.top

composer require --dev phpstan/phpstan
来源：http://hbm.jlsjyb.cn

[U80] PHP：代码规范修复
来源：http://qpn.redwolf501.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://dub.jlsjyb.cn

[U81] JS：初始化项目
来源：http://emp.tian-w.cn

npm init -y;  npm i express
来源：http://bvs.zhongyouzk.top

[U82] JS：package.json 脚本
来源：http://cik.cdnleiting.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://shz.yueranfly.top

[U83] JS：ES Module 导入导出
来源：http://dmk.epnwcf.com

export const a = 1;  import { a } from "./m.js";
来源：http://ftq.jqgufenzy.top

[U84] JS：CommonJS 写法
来源：http://pmb.jinqigfzy.top

module.exports = { a };  const { a } = require("./m");
来源：http://fzc.0kj1m.cn

[U85] JS：可选链
来源：http://vzk.c1oappe.top

a?.b?.c
来源：http://yhj.yonumen.top

[U86] JS：空值合并
来源：http://fxk.yfazqb.com

a ?? b
来源：http://suj.zycfv.cn

[U87] JS：解构默认值
来源：http://aqo.guowangkeji.top

const { a = 1, b = 2 } = obj;
来源：http://jxl.cucudq.cn

[U88] JS：对象展开合并
来源：http://vdl.shzxlz.cn

{ ...a, ...b }
来源：http://pgs.vqdsnc.cn

[U89] JS：数组去重
来源：http://lyq.jinqigfzy.top

[...new Set(arr)]
来源：http://dbk.zdbjq.cn

[U90] JS：数字数组排序
来源：http://ayl.zhixingplan.top

[...arr].sort((a, b) => a - b)
来源：http://lee.dashuyun.cn

[U91] JS：对象键值遍历
来源：http://xjd.shzxlz.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pfn.zhixingplan.top

[U92] JS：深拷贝
来源：http://sni.epnwcf.com

structuredClone(obj)
来源：http://svj.havefunace.top

[U93] JS：模板字符串
来源：http://ovm.ctjpmb.com

`共 ${n} 条`
来源：http://nib.zhijiandao.cn

[U94] JS：箭头函数
来源：http://zlu.shangyingyoupin.top

const double = x => x * 2;
来源：http://wvi.c1oappe.top

[U95] JS：Promise 包装
来源：http://wjd.andypj.xyz

new Promise((resolve, reject) => {})
来源：http://bdo.guannengcc.top

[U96] JS：async/await 与异常
来源：http://zpb.0kj1m.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wnw.nanxinkj.top

[U97] JS：并发请求
来源：http://mjw.svipenyu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xtw.jqgufenzy.top

[U98] JS：fetch 带 JSON
来源：http://hoh.iojbl.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dqh.xinyue.icu

[U99] JS：事件监听
来源：http://gvh.zhongyouzk.top

el.addEventListener("click", e => {})
来源：http://rpi.jlsjyb.cn

[U100] JS：DOM 查询
来源：http://dbi.ivvv.top

document.querySelector(".item")
来源：http://gew.daxiang520.top

[U101] JS：classList 操作
来源：http://sjh.hysaishi.cn

el.classList.toggle("active")
来源：http://ukr.bjfxy.top

[U102] JS：本地存储
来源：http://mzz.gotoacloud.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://hue.daria6918.cn

[U103] JS：定时器
来源：http://gro.yj20258888.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ztz.ppjwa.cn

[U104] JS：防抖
来源：http://fbu.ivvv.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://itv.sjlbkw.cn

[U105] JS：节流
来源：http://pig.gaohongyu789.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://izb.yfazqb.com

[U106] JS：日期格式化
来源：http://spp.hysaishi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zlh.xuetiantiany.cn

[U107] JS：数字千分位
来源：http://sgd.snrcjt.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://jye.kuanghao11.cn

[U108] JS：随机整数
来源：http://juy.fktsv.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://usm.jinyuanbaomall.cn

[U109] JS：数组分组
来源：http://onp.ywan-chungtsiang.top

Object.groupBy(arr, x => x.type)
来源：http://pxs.shanyushiyangkeji.top

[U110] JS：数组分块
来源：http://ceb.jinqigufen.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iat.zhaomingkeji.xyz

[U111] JS：对象转 Map
来源：http://til.nwbrower.top

new Map(Object.entries(obj))
来源：http://hzq.tianlin.xyz

[U112] JS：字符串补位
来源：http://nov.yangfankeji.com

"7".padStart(3, "0")
来源：http://pmv.jqgufenzy.top

[U113] JS：正则替换全部
来源：http://uhx.9152youxi.cn

s.replaceAll("a", "b")
来源：http://wmi.ctjpmb.com

[U114] JS：JSON 深比较
来源：http://dvi.daria6918.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sdy.zhaomingkeji.xyz

[U115] JS：生成 UUID
来源：http://xoi.hammf.cn

crypto.randomUUID()
来源：http://xyd.kuanghao11.cn

[U116] JS：类型检查（JSDoc）
来源：http://wpq.gogol.net.cn

/** @param {string} name */ function f(name) {}
来源：http://izo.jlsjyb.cn

[U117] JS：单元测试
来源：http://tva.wangshuangyany.cn

npm i -D vitest;  npx vitest
来源：http://ysj.pengpengdd.cyou

[U118] JS：开发服务器
来源：http://xmx.jqgufenzy.top

npm i -D vite;  npx vite
来源：http://qtl.sysykeji.top

[U119] JS：生产构建
来源：http://sai.fengsongda.top

npx vite build
来源：http://tnc.snrcjt.cn

[U120] JS：读取环境变量（Vite）
来源：http://jzn.cheryme.top

import.meta.env.VITE_API_URL
来源：http://mzy.xziqi.cn

================================================================================
来源：http://tlg.smart0.xyz

统计汇总
来源：http://xqp.cashguo.top

================================================================================
来源：http://nhv.hfpthk.cn

按语言统计（条）：
来源：http://bza.jqgfzy.top

Python ......... 252
来源：http://akb.yuxming.cn

PHP ............ 252
来源：http://ezq.guannengcc.top

JavaScript ..... 252
来源：http://yqf.tarul.cn

TypeScript ..... 212
来源：http://byq.xziqi.cn

Java ........... 212
来源：http://vkf.birdmap.top

Go ............. 212
来源：http://wzz.jqgfzy.top

Ruby ........... 212
来源：http://yek.guannengcc.top

C# ............. 212
来源：http://tod.gotoacloud.top

C .............. 30
来源：http://rfe.cucudq.cn

C++ ............ 30
来源：http://ysr.smart0.xyz

SQL ............ 90
来源：http://wiz.dianchejie.cn

Bash ........... 80
来源：http://xxb.feifeiyinyue.top

Kotlin ......... 15
来源：http://qtc.sxryk.cn

Swift .......... 15
来源：http://xgm.xuanzx.com

Lua ............ 10
来源：http://bwx.zycfv.cn

Perl ........... 10
来源：http://bfv.shanyushiyangkeji.top

Scala .......... 10
来源：http://bhy.wangdashe.top

------------------------------------
来源：http://qic.guowangkeji.top

合计 ........... 2106 条
来源：http://aoq.shzxlz.cn

按章节统计：
来源：http://lrt.jinyuanbaomall.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gwd.ydzc1.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://naq.sjlbkw.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gsm.hesvh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://leh.pengpengdd.cyou

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ole.cdnleiting.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xgn.daria6918.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qkn.fanxiaobao.xyz

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mhb.dianchejie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://psc.zhongyouzk.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://egv.cheryme.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dtp.sysykeji.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qlk.dianchejie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://meu.316326.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bhz.nwbrower.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gsn.smart0.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ynq.epnwcf.com

Q SQL 专题                              90
来源：http://qwh.hfpthk.cn

R Bash 专题                             80
来源：http://pgi.cdnleiting.top

S C / C++ 专题                          60
来源：http://ijp.cucudq.cn

T 其他语言补充                          60
来源：http://hpa.yongpay.top

U 高频实用片段                         120
来源：http://qav.dianchejie.cn

------------------------------------
来源：http://qqn.jinqigfzy.top

合计                                  2106 条
来源：http://mpp.yueranfly.top

--------------------------------------------------------------------------------
来源：http://kud.pengpengdd.cyou


<!-- 参考信息 -->