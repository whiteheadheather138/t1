代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://zpv.fengsongda.top

[T55] Scala：集合过滤
来源：http://ieu.ydjk.org.cn

List(1, 2, 3).filter(_ > 1)
来源：http://muf.nanxinkj.top

[T56] Scala：样例类
来源：http://lle.chenlongwang.top

case class User(name: String, age: Int)
来源：http://jdk.sufxvd.cn

[T57] Scala：模式匹配
来源：http://wlu.jqgfzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://meq.dianchejie.cn

[T58] Scala：函数定义
来源：http://ovq.sufxvd.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fmj.tanke756.top

[T59] Scala：循环
来源：http://vnr.jinyuanbaomall.cn

for (i <- 1 to 10) println(i)
来源：http://sdx.sweek.top

[T60] Scala：折叠
来源：http://yob.redwolf501.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zyf.fanxiaobao.xyz

================================================================================
来源：http://wpo.feifeiyinyue.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jwp.iojbl.cn

================================================================================
来源：http://imb.zhongyouzk.top

[U01] Py：创建虚拟环境
来源：http://cgc.yuanzhike.top

python -m venv .venv && source .venv/bin/activate
来源：http://yht.mhx1999.top

[U02] Py：导出 / 安装依赖
来源：http://aka.pycfn.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vyr.meibo888.top

[U03] Py：加载 .env 配置
来源：http://okq.hnqzz.top

from dotenv import load_dotenv; load_dotenv()
来源：http://bmj.cqqwz.cn

[U04] Py：变量调试打印
来源：http://zuo.jqgfzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ugn.sysykeji.top

[U05] Py：列表去重且保序
来源：http://pva.sysykeji.top

list(dict.fromkeys(arr))
来源：http://vdq.zhaomingkeji.xyz

[U06] Py：合并两个字典
来源：http://jms.cashguo.top

{**a, **b}
来源：http://muf.xuetiantiany.cn

[U07] Py：反转字典键值
来源：http://mhl.ywan-chungtsiang.top

{v: k for k, v in d.items()}
来源：http://ihs.nanxinkj.top

[U08] Py：展平二维列表
来源：http://spb.tianlin.xyz

[y for x in nested for y in x]
来源：http://qdk.haohaochexian.top

[U09] Py：字典取最大值的键
来源：http://ung.bjfxy.top

max(d, key=d.get)
来源：http://vmq.ehwqpu.com

[U10] Py：按值排序字典
来源：http://jgo.aizwys.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mkb.gotoacloud.top

[U11] Py：生成器表达式
来源：http://dzd.meibo888.top

(x * 2 for x in arr)
来源：http://utr.hongshengwenyu.top

[U12] Py：取出现最多的 3 个元素
来源：http://qxc.tianlin.xyz

Counter(arr).most_common(3)
来源：http://uje.yongpay.top

[U13] Py：固定长度队列
来源：http://xib.gotoacloud.top

deque(maxlen=10)
来源：http://asw.fengsongda.top

[U14] Py：分组收集到列表
来源：http://dps.jqgfzy.top

defaultdict(list)
来源：http://hon.yangfankeji.com

[U15] Py：高精度计时
来源：http://dat.jqgfzy.top

t = time.perf_counter()
来源：http://cpi.uphjek.com

[U16] Py：命令行参数解析
来源：http://rfx.hcnkem.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ckr.cqqwz.cn

[U17] Py：初始化日志
来源：http://ffz.sjlbkw.cn

logging.basicConfig(level=logging.INFO)
来源：http://nqp.snrcjt.cn

[U18] Py：预编译正则
来源：http://szw.hammf.cn

pat = re.compile(r"\d+")
来源：http://upt.yuxming.cn

[U19] Py：正则替换带回调
来源：http://zmg.yfazqb.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nbj.haohaochexian.top

[U20] Py：缓存函数结果
来源：http://uhg.ctjpmb.com

@functools.lru_cache(maxsize=None)
来源：http://ang.cucudq.cn

[U21] Py：自定义上下文管理器
来源：http://qpj.52xcode.cn

@contextlib.contextmanager
来源：http://ihw.gogol.net.cn

[U22] Py：矩阵转置
来源：http://nnj.feifeiyinyue.top

list(zip(*m))
来源：http://dyf.yongpay.top

[U23] Py：分块读取大文件
来源：http://uew.feifeiyinyue.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://myn.iojbl.cn

[U24] Py：路径操作
来源：http://jvo.yanxiufei.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://feq.shanyushiyangtech.top

[U25] Py：CSV 按字典读
来源：http://gjk.fanxiaobao.xyz

csv.DictReader(f)
来源：http://zur.ywan-chungtsiang.top

[U26] Py：并发下载
来源：http://cra.yonumen.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qgg.zhixingplan.top

[U27] Py：异步 HTTP
来源：http://djk.dianchejie.cn

aiohttp.ClientSession() 配合 async with
来源：http://peo.nwbrower.top

[U28] Py：类型别名
来源：http://lmh.daxiang520.top

UserId = int
来源：http://jik.snrcjt.cn

[U29] Py：属性校验
来源：http://fmg.sxryk.cn

@property 与 @x.setter 配合
来源：http://pda.meibo888.top

[U30] Py：数据类
来源：http://rgh.zhongyouzk.top

@dataclass(slots=True)
来源：http://sgn.yangfankeji.com

[U31] Py：单测
来源：http://rsv.zhengqikj.top

python -m pytest -q
来源：http://izf.xziqi.cn

[U32] Py：代码格式化
来源：http://eko.xinyue.icu

ruff format . && ruff check --fix .
来源：http://tru.jianghu66.top

[U33] Py：打包发布
来源：http://col.bjfxy.top

python -m build  （依赖 pyproject.toml）
来源：http://zwh.chenzaomai.com

[U34] Py：判断编码
来源：http://xll.jinqigufen.top

chardet.detect(raw)
来源：http://esf.ctjpmb.com

[U35] Py：发送邮件
来源：http://xcw.wangshuangyany.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gda.sweek.top

[U36] Py：定时任务
来源：http://kqt.iojbl.cn

schedule.every(10).minutes.do(job)
来源：http://izj.shzxlz.cn

[U37] Py：读写 Excel
来源：http://umn.birdmap.top

pandas.read_excel / DataFrame.to_excel
来源：http://obn.zhongyouzk.top

[U38] Py：获取脚本所在目录
来源：http://dcq.yanxiufei.cn

Path(__file__).resolve().parent
来源：http://kpi.jinyuanbaomall.cn

[U39] Py：判断是否在交互环境
来源：http://snw.xinyue.icu

sys.stdout.isatty()
来源：http://evh.zycfv.cn

[U40] Py：打印到标准错误
来源：http://hrn.jinqigfzy.top

print("err", file=sys.stderr)
来源：http://cyw.yuxming.cn

[U41] PHP：初始化 Composer 项目
来源：http://bna.yonumen.top

composer init;  composer require guzzlehttp/guzzle
来源：http://miy.ywan-chungtsiang.top

[U42] PHP：PSR-4 自动加载
来源：http://yen.fktsv.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vpn.hammf.cn

[U43] PHP：声明命名空间
来源：http://rkc.c1oappe.top

namespace App\Http;
来源：http://rsa.hnqzz.top

[U44] PHP：开启严格类型
来源：http://ylf.tarul.cn

declare(strict_types=1);
来源：http://eyq.zhiwuduotai.top

[U45] PHP：类型声明与返回类型
来源：http://fjc.zhixingplan.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zbd.gaohongyu789.top

[U46] PHP：可空类型
来源：http://elw.zhoulong.xyz

?string $name = null
来源：http://kwq.cdnleiting.top

[U47] PHP：联合类型
来源：http://juk.zhijiandao.cn

int|string $id
来源：http://awi.tian-w.cn

[U48] PHP：纯枚举
来源：http://yid.tanke756.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vfw.sxryk.cn

[U49] PHP：只读属性
来源：http://ccb.cheryme.top

public readonly string $name
来源：http://mcl.vqdsnc.cn

[U50] PHP：构造器属性提升
来源：http://fwk.zhoulong.xyz

public function __construct(private int $id) {}
来源：http://zxq.tianlin.xyz

[U51] PHP：数组解构
来源：http://zcv.gaohongyu789.top

[$a, $b] = $arr;
来源：http://mej.iojbl.cn

[U52] PHP：箭头函数
来源：http://uhq.jiagoushi.top

$double = fn($x) => $x * 2;
来源：http://zfl.zhiwuduotai.top

[U53] PHP：空合并运算符
来源：http://tmz.yueranfly.top

$v = $a ?? $b ?? "default";
来源：http://zxn.yfazqb.com

[U54] PHP：空安全调用
来源：http://dff.cashguo.top

$obj?->method()
来源：http://vmc.dianchejie.cn

[U55] PHP：match 表达式
来源：http://nfe.sjlbkw.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hph.xingfuxueyuan.xyz

[U56] PHP：命名参数
来源：http://plx.svipenyu.cn

f(a: 1, b: 2)
来源：http://vfo.316326.xyz

[U57] PHP：字符串插值
来源：http://wqt.yfazqb.com

"值: {$a}"
来源：http://egn.jinqigufen.top

[U58] PHP：数组三件套
来源：http://dha.guowangkeji.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vtd.jinyuanbaomall.cn

[U59] PHP：自定义排序
来源：http://fzz.nanxuanxn.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://grb.chenlongwang.top

[U60] PHP：JSON 编解码
来源：http://sek.chenzaomai.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ejb.gotoacloud.top

[U61] PHP：正则
来源：http://zsg.sufxvd.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bsv.jianghu66.top

[U62] PHP：日期对象
来源：http://toz.cdnleiting.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tju.zhengqikj.top

[U63] PHP：文件读写
来源：http://ukd.bbcook.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://biv.gotoacloud.top

[U64] PHP：目录遍历
来源：http://som.yonumen.top

glob("dir/*.php");  scandir("dir");
来源：http://izp.ivvv.top

[U65] PHP：会话
来源：http://gln.gogol.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ajp.cheryme.top

[U66] PHP：设置 Cookie
来源：http://xwk.fehbvm.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ool.xziqi.cn

[U67] PHP：处理文件上传
来源：http://qgv.zhengqikj.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ebs.snrcjt.cn

[U68] PHP：PDO 连接
来源：http://hau.ppjwa.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hwo.jinghuilouyu.cn

[U69] PHP：PDO 预处理
来源：http://ztk.9152youxi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gnc.ivvv.top

[U70] PHP：PDO 事务
来源：http://xep.uphjek.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://npz.nanxuanxn.top

[U71] PHP：抛出异常
来源：http://mww.xuanzx.com

throw new RuntimeException("失败", 500);
来源：http://ewg.fktsv.cn

[U72] PHP：写错误日志
来源：http://qzt.hnxiangtu.top

error_log("失败: " . $e->getMessage());
来源：http://dfr.gogol.net.cn

[U73] PHP：读取 ini 配置
来源：http://ddn.jianghu66.top

parse_ini_file("config.ini", true)
来源：http://eoi.uphjek.com

[U74] PHP：读取环境变量
来源：http://zhb.xziqi.cn

getenv("APP_ENV") ?: "production"
来源：http://xyt.zdqjudy.top

[U75] PHP：依赖注入
来源：http://atz.tarul.cn

composer require psr/container
来源：http://odd.hammf.cn

[U76] PHP：简单路由
来源：http://agj.tian-w.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hzk.chenjidiqi.icu

[U77] PHP：模板渲染
来源：http://gaj.xuanzx.com

composer require twig/twig
来源：http://zgl.jinyuanbaomall.cn

[U78] PHP：单元测试
来源：http://pmg.sweek.top

composer require --dev phpunit/phpunit
来源：http://hpy.yuanzhike.top

[U79] PHP：静态分析
来源：http://ply.zhixingplan.top

composer require --dev phpstan/phpstan
来源：http://chg.chenzaomai.com

[U80] PHP：代码规范修复
来源：http://nhn.havefunace.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://szx.feifeiyinyue.top

[U81] JS：初始化项目
来源：http://uty.hywenlv.cn

npm init -y;  npm i express
来源：http://cjd.shanyushiyangkeji.top

[U82] JS：package.json 脚本
来源：http://qtf.yvedp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ebv.jqgfzy.top

[U83] JS：ES Module 导入导出
来源：http://ysu.xuetiantiany.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lig.xziqi.cn

[U84] JS：CommonJS 写法
来源：http://qgx.yongpay.top

module.exports = { a };  const { a } = require("./m");
来源：http://zmb.havefunace.top

[U85] JS：可选链
来源：http://edl.hywenlv.cn

a?.b?.c
来源：http://tgi.jinqigfzy.top

[U86] JS：空值合并
来源：http://lbe.nanxuanxn.top

a ?? b
来源：http://vmp.haohaochexian.top

[U87] JS：解构默认值
来源：http://swc.guowangkeji.top

const { a = 1, b = 2 } = obj;
来源：http://zce.jianghu66.top

[U88] JS：对象展开合并
来源：http://gok.gotoacloud.top

{ ...a, ...b }
来源：http://bql.jinqigfzy.top

[U89] JS：数组去重
来源：http://fct.hnxiangtu.top

[...new Set(arr)]
来源：http://plg.jinqigufen.top

[U90] JS：数字数组排序
来源：http://dol.yvedp.cn

[...arr].sort((a, b) => a - b)
来源：http://hcr.bbcook.cn

[U91] JS：对象键值遍历
来源：http://pty.xuanzx.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nrg.sweek.top

[U92] JS：深拷贝
来源：http://zjh.tanke756.top

structuredClone(obj)
来源：http://ily.meibo888.top

[U93] JS：模板字符串
来源：http://pxf.yonumen.top

`共 ${n} 条`
来源：http://rxl.xziqi.cn

[U94] JS：箭头函数
来源：http://ine.cashguo.top

const double = x => x * 2;
来源：http://fdb.jinqigufen.top

[U95] JS：Promise 包装
来源：http://cph.bbcook.cn

new Promise((resolve, reject) => {})
来源：http://wbu.epnwcf.com

[U96] JS：async/await 与异常
来源：http://yhf.xuetiantiany.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sit.zhongyouzk.top

[U97] JS：并发请求
来源：http://yob.shuidangran.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://rin.shanyushiyangtech.top

[U98] JS：fetch 带 JSON
来源：http://wcv.tanke756.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://agr.ctjpmb.com

[U99] JS：事件监听
来源：http://bft.yanxiufei.cn

el.addEventListener("click", e => {})
来源：http://pdl.9152youxi.cn

[U100] JS：DOM 查询
来源：http://bhh.fanxiaobao.xyz

document.querySelector(".item")
来源：http://xks.jinqigufen.top

[U101] JS：classList 操作
来源：http://cqe.wangshuangyany.cn

el.classList.toggle("active")
来源：http://nvs.fanxiaobao.xyz

[U102] JS：本地存储
来源：http://arh.havefunace.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://brc.hesvh.cn

[U103] JS：定时器
来源：http://jnv.tianlin.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yfo.daria6918.cn

[U104] JS：防抖
来源：http://why.guannengcc.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rcj.sjlbkw.cn

[U105] JS：节流
来源：http://nuo.ydjk.org.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://iay.fzhhl.top

[U106] JS：日期格式化
来源：http://ytz.jinqigfzy.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tig.hfpthk.cn

[U107] JS：数字千分位
来源：http://iqd.cheryme.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lgy.hammf.cn

[U108] JS：随机整数
来源：http://qpx.shanyushiyangkeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://atf.xinyue.icu

[U109] JS：数组分组
来源：http://wvc.316326.xyz

Object.groupBy(arr, x => x.type)
来源：http://rbx.hnxiangtu.top

[U110] JS：数组分块
来源：http://msi.jinqigufen.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hup.wangdashe.top

[U111] JS：对象转 Map
来源：http://ozu.snrcjt.cn

new Map(Object.entries(obj))
来源：http://vlc.jqgufenzy.top

[U112] JS：字符串补位
来源：http://waz.haohaochexian.top

"7".padStart(3, "0")
来源：http://kff.birdmap.top

[U113] JS：正则替换全部
来源：http://uji.xingfuxueyuan.xyz

s.replaceAll("a", "b")
来源：http://poy.ydzc1.top

[U114] JS：JSON 深比较
来源：http://eyh.jinqigufen.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://tlk.vehdjk.com

[U115] JS：生成 UUID
来源：http://qsz.hesvh.cn

crypto.randomUUID()
来源：http://wkw.tarul.cn

[U116] JS：类型检查（JSDoc）
来源：http://vxj.shuidangran.top

/** @param {string} name */ function f(name) {}
来源：http://uny.fengsongda.top

[U117] JS：单元测试
来源：http://tit.fzhhl.top

npm i -D vitest;  npx vitest
来源：http://eai.ydzc1.top

[U118] JS：开发服务器
来源：http://wcp.c1oappe.top

npm i -D vite;  npx vite
来源：http://lxw.ydjk.org.cn

[U119] JS：生产构建
来源：http://aei.yonumen.top

npx vite build
来源：http://nfb.sysykeji.top

[U120] JS：读取环境变量（Vite）
来源：http://vkn.sweek.top

import.meta.env.VITE_API_URL
来源：http://vdk.yj202588.top

================================================================================
来源：http://ywk.zycfv.cn

统计汇总
来源：http://mhu.tanke756.top

================================================================================
来源：http://tif.yangfankeji.com

按语言统计（条）：
来源：http://edh.shzxlz.cn

Python ......... 252
来源：http://acu.jqgufenzy.top

PHP ............ 252
来源：http://qrl.hywenlv.cn

JavaScript ..... 252
来源：http://nvb.yonumen.top

TypeScript ..... 212
来源：http://xci.xuetiantiany.cn

Java ........... 212
来源：http://fry.snrcjt.cn

Go ............. 212
来源：http://hqm.zhengqikj.top

Ruby ........... 212
来源：http://rot.jiagoushi.top

C# ............. 212
来源：http://ssu.zhongyouzk.top

C .............. 30
来源：http://rki.gotoacloud.top

C++ ............ 30
来源：http://qkl.guowangkeji.top

SQL ............ 90
来源：http://yie.havefunace.top

Bash ........... 80
来源：http://oxo.jiagoushi.top

Kotlin ......... 15
来源：http://uxd.xziqi.cn

Swift .......... 15
来源：http://ifc.xuetiantiany.cn

Lua ............ 10
来源：http://htt.gaohongyu789.top

Perl ........... 10
来源：http://stf.wangshuangyany.cn

Scala .......... 10
来源：http://ofp.smart0.xyz

------------------------------------
来源：http://nyb.jianghu66.top

合计 ........... 2106 条
来源：http://flc.yuanzhike.top

按章节统计：
来源：http://uzb.ctjpmb.com

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ctf.yj20258.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://quw.epnwcf.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vhv.sjlbkw.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zts.sufxvd.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jen.gaohongyu789.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tuu.guowangkeji.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dhb.yuanzhike.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jqd.hfpthk.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hlu.fehbvm.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gjs.shanyushiyangkeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ykx.kuanghao11.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cgg.zhijiandao.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://aph.guannengcc.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mdx.hnxiangtu.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://znj.yongpay.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hnl.jqgufenzy.top

Q SQL 专题                              90
来源：http://nqm.sweek.top

R Bash 专题                             80
来源：http://kwq.cqqwz.cn

S C / C++ 专题                          60
来源：http://jtq.redwolf501.top

T 其他语言补充                          60
来源：http://cuf.jlsjyb.cn


<!-- 参考信息 -->