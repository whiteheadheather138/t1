代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://odd.cucudq.cn

[T55] Scala：集合过滤
来源：http://laj.nanxinkj.top

List(1, 2, 3).filter(_ > 1)
来源：http://djb.xuetiantiany.cn

[T56] Scala：样例类
来源：http://rdj.yj20258888.top

case class User(name: String, age: Int)
来源：http://ugm.nwbrower.top

[T57] Scala：模式匹配
来源：http://hoo.iojbl.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qby.yuxming.cn

[T58] Scala：函数定义
来源：http://saf.jyoumei.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xwx.ppjwa.cn

[T59] Scala：循环
来源：http://mik.0kj1m.cn

for (i <- 1 to 10) println(i)
来源：http://seo.aibaodan.cn

[T60] Scala：折叠
来源：http://zug.snrcjt.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://aaz.aibaodan.cn

================================================================================
来源：http://nnc.gaohongyu789.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mtb.yuanzhike.top

================================================================================
来源：http://lib.hcnkem.com

[U01] Py：创建虚拟环境
来源：http://ruo.xuanzx.com

python -m venv .venv && source .venv/bin/activate
来源：http://gsq.zhixingplan.top

[U02] Py：导出 / 安装依赖
来源：http://yvi.tanke756.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tiu.ivvv.top

[U03] Py：加载 .env 配置
来源：http://nvq.gogol.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zax.aibaodan.cn

[U04] Py：变量调试打印
来源：http://rci.zhengqikj.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ail.ybcxt.top

[U05] Py：列表去重且保序
来源：http://mzy.xuetiantiany.cn

list(dict.fromkeys(arr))
来源：http://jtj.chenlongwang.top

[U06] Py：合并两个字典
来源：http://zus.nanxuanxn.top

{**a, **b}
来源：http://xrt.meibo888.top

[U07] Py：反转字典键值
来源：http://jpg.52xcode.cn

{v: k for k, v in d.items()}
来源：http://bmq.dashuyun.cn

[U08] Py：展平二维列表
来源：http://fvp.xinyue.icu

[y for x in nested for y in x]
来源：http://sio.hesvh.cn

[U09] Py：字典取最大值的键
来源：http://enh.yvedp.cn

max(d, key=d.get)
来源：http://bji.yueranfly.top

[U10] Py：按值排序字典
来源：http://nif.iojbl.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://osb.yangfankeji.com

[U11] Py：生成器表达式
来源：http://klg.zhengqikj.top

(x * 2 for x in arr)
来源：http://sny.hammf.cn

[U12] Py：取出现最多的 3 个元素
来源：http://phz.aibaodan.cn

Counter(arr).most_common(3)
来源：http://imk.ydjk.org.cn

[U13] Py：固定长度队列
来源：http://yxm.quarkkingdee.top

deque(maxlen=10)
来源：http://vwz.yuanzhike.top

[U14] Py：分组收集到列表
来源：http://zka.jinyuanbaomall.cn

defaultdict(list)
来源：http://ddx.wangshuangyany.cn

[U15] Py：高精度计时
来源：http://mlp.yonumen.top

t = time.perf_counter()
来源：http://fty.guannengcc.top

[U16] Py：命令行参数解析
来源：http://lwe.gogol.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pxl.shuidangran.top

[U17] Py：初始化日志
来源：http://stx.hnqzz.top

logging.basicConfig(level=logging.INFO)
来源：http://mok.xuanzx.com

[U18] Py：预编译正则
来源：http://hwo.daxiang520.top

pat = re.compile(r"\d+")
来源：http://hhn.yvedp.cn

[U19] Py：正则替换带回调
来源：http://nry.fengsongda.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ntw.pycfn.com

[U20] Py：缓存函数结果
来源：http://lvf.tarul.cn

@functools.lru_cache(maxsize=None)
来源：http://wkb.xuetiantiany.cn

[U21] Py：自定义上下文管理器
来源：http://cut.jqgufenzy.top

@contextlib.contextmanager
来源：http://lri.fzhhl.top

[U22] Py：矩阵转置
来源：http://evy.ctjpmb.com

list(zip(*m))
来源：http://jut.fzhhl.top

[U23] Py：分块读取大文件
来源：http://xkr.jyoumei.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mta.sufxvd.cn

[U24] Py：路径操作
来源：http://xpu.ctjpmb.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dqn.chenzaomai.com

[U25] Py：CSV 按字典读
来源：http://gyw.yueranfly.top

csv.DictReader(f)
来源：http://yva.gzhubu.top

[U26] Py：并发下载
来源：http://szx.chenzaomai.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dln.meibo888.top

[U27] Py：异步 HTTP
来源：http://ihr.zhijiandao.cn

aiohttp.ClientSession() 配合 async with
来源：http://czm.cdnleiting.top

[U28] Py：类型别名
来源：http://ddt.yuanzhike.top

UserId = int
来源：http://hos.iojbl.cn

[U29] Py：属性校验
来源：http://aqe.guowangkeji.top

@property 与 @x.setter 配合
来源：http://rbf.jyoumei.cn

[U30] Py：数据类
来源：http://uqh.yj20258.top

@dataclass(slots=True)
来源：http://qop.svipenyu.cn

[U31] Py：单测
来源：http://gkb.yonumen.top

python -m pytest -q
来源：http://tzj.zycfv.cn

[U32] Py：代码格式化
来源：http://wga.jianghu66.top

ruff format . && ruff check --fix .
来源：http://cdp.hfpthk.cn

[U33] Py：打包发布
来源：http://dcs.fengsongda.top

python -m build  （依赖 pyproject.toml）
来源：http://vrz.fzhhl.top

[U34] Py：判断编码
来源：http://qnv.guannengcc.top

chardet.detect(raw)
来源：http://eqk.dianchejie.cn

[U35] Py：发送邮件
来源：http://not.sjlbkw.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sin.gogol.net.cn

[U36] Py：定时任务
来源：http://qpk.havefunace.top

schedule.every(10).minutes.do(job)
来源：http://kux.tian-w.cn

[U37] Py：读写 Excel
来源：http://dlk.ctjpmb.com

pandas.read_excel / DataFrame.to_excel
来源：http://dlw.jiagoushi.top

[U38] Py：获取脚本所在目录
来源：http://ydw.nanxinkj.top

Path(__file__).resolve().parent
来源：http://lol.daria6918.cn

[U39] Py：判断是否在交互环境
来源：http://kdw.9152youxi.cn

sys.stdout.isatty()
来源：http://cbf.feifeiyinyue.top

[U40] Py：打印到标准错误
来源：http://kxt.cashguo.top

print("err", file=sys.stderr)
来源：http://zsv.zhijiandao.cn

[U41] PHP：初始化 Composer 项目
来源：http://zzv.sufxvd.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fzx.chenlongwang.top

[U42] PHP：PSR-4 自动加载
来源：http://cwr.xylfe.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vwv.hammf.cn

[U43] PHP：声明命名空间
来源：http://shr.gogol.net.cn

namespace App\Http;
来源：http://lzn.xylfe.cn

[U44] PHP：开启严格类型
来源：http://vcm.yfazqb.com

declare(strict_types=1);
来源：http://pol.snrcjt.cn

[U45] PHP：类型声明与返回类型
来源：http://xup.snrcjt.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jwm.52xcode.cn

[U46] PHP：可空类型
来源：http://axz.kuanghao11.cn

?string $name = null
来源：http://tyx.tian-w.cn

[U47] PHP：联合类型
来源：http://knt.sweek.top

int|string $id
来源：http://ire.yj20258888.top

[U48] PHP：纯枚举
来源：http://lwt.quarkkingdee.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zck.fktsv.cn

[U49] PHP：只读属性
来源：http://zzn.vqdsnc.cn

public readonly string $name
来源：http://dmf.jqgufenzy.top

[U50] PHP：构造器属性提升
来源：http://qeu.ydjk.org.cn

public function __construct(private int $id) {}
来源：http://qbm.hysaishi.cn

[U51] PHP：数组解构
来源：http://dza.bjfxy.top

[$a, $b] = $arr;
来源：http://ghb.yuxming.cn

[U52] PHP：箭头函数
来源：http://phl.sjlbkw.cn

$double = fn($x) => $x * 2;
来源：http://rlr.zhongyouzk.top

[U53] PHP：空合并运算符
来源：http://jui.jyoumei.cn

$v = $a ?? $b ?? "default";
来源：http://xvn.shangyingyoupin.top

[U54] PHP：空安全调用
来源：http://pkf.meibo888.top

$obj?->method()
来源：http://fgb.uphjek.com

[U55] PHP：match 表达式
来源：http://yxx.bjfxy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hhx.daria6918.cn

[U56] PHP：命名参数
来源：http://hag.ywan-chungtsiang.top

f(a: 1, b: 2)
来源：http://pza.hammf.cn

[U57] PHP：字符串插值
来源：http://wjp.cheryme.top

"值: {$a}"
来源：http://qst.hysaishi.cn

[U58] PHP：数组三件套
来源：http://jgl.shuidangran.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tei.9152youxi.cn

[U59] PHP：自定义排序
来源：http://azl.hnxiangtu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jmj.sysykeji.top

[U60] PHP：JSON 编解码
来源：http://nph.yueranfly.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wbj.shzxlz.cn

[U61] PHP：正则
来源：http://erg.daria6918.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mal.iojbl.cn

[U62] PHP：日期对象
来源：http://xjl.epnwcf.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://exx.hnxiangtu.top

[U63] PHP：文件读写
来源：http://wkj.svipenyu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://maj.yongpay.top

[U64] PHP：目录遍历
来源：http://ucp.quarkkingdee.top

glob("dir/*.php");  scandir("dir");
来源：http://tfe.tian-w.cn

[U65] PHP：会话
来源：http://jnw.yj202588.top

session_start();  $_SESSION["uid"] = 1;
来源：http://wja.sweek.top

[U66] PHP：设置 Cookie
来源：http://rkt.daxiang520.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sua.hfpthk.cn

[U67] PHP：处理文件上传
来源：http://umf.jinghuilouyu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dvm.yj202588.top

[U68] PHP：PDO 连接
来源：http://vxv.sxryk.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qrz.shangyingyoupin.top

[U69] PHP：PDO 预处理
来源：http://xsb.yj20258888.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://aae.ivvv.top

[U70] PHP：PDO 事务
来源：http://uin.tian-w.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://eaa.redwolf501.top

[U71] PHP：抛出异常
来源：http://vzm.chenlongwang.top

throw new RuntimeException("失败", 500);
来源：http://sdj.guannengcc.top

[U72] PHP：写错误日志
来源：http://mwx.dianchejie.cn

error_log("失败: " . $e->getMessage());
来源：http://tlb.cucudq.cn

[U73] PHP：读取 ini 配置
来源：http://uyl.jiagoushi.top

parse_ini_file("config.ini", true)
来源：http://koy.quarkkingdee.top

[U74] PHP：读取环境变量
来源：http://cvl.nanxuanxn.top

getenv("APP_ENV") ?: "production"
来源：http://yak.ybcxt.top

[U75] PHP：依赖注入
来源：http://msp.gaohongyu789.top

composer require psr/container
来源：http://foh.yj202588.top

[U76] PHP：简单路由
来源：http://aaj.gaohongyu789.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xej.kuanghao11.cn

[U77] PHP：模板渲染
来源：http://wgm.jinqigfzy.top

composer require twig/twig
来源：http://bjt.birdmap.top

[U78] PHP：单元测试
来源：http://liw.chenlongwang.top

composer require --dev phpunit/phpunit
来源：http://ejz.shangyingyoupin.top

[U79] PHP：静态分析
来源：http://fbs.uphjek.com

composer require --dev phpstan/phpstan
来源：http://nxp.aizwys.cn

[U80] PHP：代码规范修复
来源：http://tth.cashguo.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://okm.xinyue.icu

[U81] JS：初始化项目
来源：http://djd.xylfe.cn

npm init -y;  npm i express
来源：http://hps.uphjek.com

[U82] JS：package.json 脚本
来源：http://ifp.jinghuilouyu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kbi.chenzaomai.com

[U83] JS：ES Module 导入导出
来源：http://usr.smart0.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://sjv.cdnleiting.top

[U84] JS：CommonJS 写法
来源：http://dzs.sxryk.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rjd.xylfe.cn

[U85] JS：可选链
来源：http://frs.aizwys.cn

a?.b?.c
来源：http://rad.meibo888.top

[U86] JS：空值合并
来源：http://lmf.epnwcf.com

a ?? b
来源：http://okb.jinqigfzy.top

[U87] JS：解构默认值
来源：http://bpc.ehwqpu.com

const { a = 1, b = 2 } = obj;
来源：http://ytz.ivvv.top

[U88] JS：对象展开合并
来源：http://slu.yonumen.top

{ ...a, ...b }
来源：http://xjw.fzhhl.top

[U89] JS：数组去重
来源：http://sjg.yj20258888.top

[...new Set(arr)]
来源：http://dhg.yongpay.top

[U90] JS：数字数组排序
来源：http://kin.hnxiangtu.top

[...arr].sort((a, b) => a - b)
来源：http://jle.yfazqb.com

[U91] JS：对象键值遍历
来源：http://odw.ydzc1.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://uqd.zhengqikj.top

[U92] JS：深拷贝
来源：http://vdn.jqgufenzy.top

structuredClone(obj)
来源：http://div.guowangkeji.top

[U93] JS：模板字符串
来源：http://exx.feifeiyinyue.top

`共 ${n} 条`
来源：http://itt.sufxvd.cn

[U94] JS：箭头函数
来源：http://dem.dashuyun.cn

const double = x => x * 2;
来源：http://zej.zhaomingkeji.xyz

[U95] JS：Promise 包装
来源：http://xjv.shzxlz.cn

new Promise((resolve, reject) => {})
来源：http://lfe.havefunace.top

[U96] JS：async/await 与异常
来源：http://jqe.yvedp.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ilu.chenjidiqi.icu

[U97] JS：并发请求
来源：http://hpm.jinqigufen.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://lwu.jiagoushi.top

[U98] JS：fetch 带 JSON
来源：http://jih.jlsjyb.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vwu.c1oappe.top

[U99] JS：事件监听
来源：http://izf.c1oappe.top

el.addEventListener("click", e => {})
来源：http://mqo.shanyushiyangtech.top

[U100] JS：DOM 查询
来源：http://rji.zdqjudy.top

document.querySelector(".item")
来源：http://jdo.hongshengwenyu.top

[U101] JS：classList 操作
来源：http://jzp.hysaishi.cn

el.classList.toggle("active")
来源：http://mip.tarul.cn

[U102] JS：本地存储
来源：http://fwi.jiagoushi.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://pvx.gzhubu.top

[U103] JS：定时器
来源：http://vhx.yvedp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://het.yuanzhike.top

[U104] JS：防抖
来源：http://gvr.ydjk.org.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yiy.yueranfly.top

[U105] JS：节流
来源：http://fsz.zdbjq.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wos.zhoulong.xyz

[U106] JS：日期格式化
来源：http://xmq.iojbl.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://udi.zhengqikj.top

[U107] JS：数字千分位
来源：http://shz.zhaomingkeji.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hpl.ehwqpu.com

[U108] JS：随机整数
来源：http://ite.jqgfzy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://suk.daria6918.cn

[U109] JS：数组分组
来源：http://bwn.mhx1999.top

Object.groupBy(arr, x => x.type)
来源：http://uvx.yj20258888.top

[U110] JS：数组分块
来源：http://lqm.sufxvd.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ayq.sysykeji.top

[U111] JS：对象转 Map
来源：http://ugb.aibaodan.cn

new Map(Object.entries(obj))
来源：http://pyl.vqdsnc.cn

[U112] JS：字符串补位
来源：http://wlf.hfpthk.cn

"7".padStart(3, "0")
来源：http://ojd.zhoulong.xyz

[U113] JS：正则替换全部
来源：http://bll.guowangkeji.top

s.replaceAll("a", "b")
来源：http://sxe.dianchejie.cn

[U114] JS：JSON 深比较
来源：http://ssf.shangyingyoupin.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://byc.shangyingyoupin.top

[U115] JS：生成 UUID
来源：http://yzr.wangshuangyany.cn

crypto.randomUUID()
来源：http://woa.bjfxy.top

[U116] JS：类型检查（JSDoc）
来源：http://gey.yuxming.cn

/** @param {string} name */ function f(name) {}
来源：http://wzo.fzhhl.top

[U117] JS：单元测试
来源：http://wbo.mhx1999.top

npm i -D vitest;  npx vitest
来源：http://tul.snrcjt.cn

[U118] JS：开发服务器
来源：http://fmh.ppjwa.cn

npm i -D vite;  npx vite
来源：http://sxi.cucudq.cn

[U119] JS：生产构建
来源：http://sjz.hfpthk.cn

npx vite build
来源：http://vwa.gzhubu.top

[U120] JS：读取环境变量（Vite）
来源：http://vqa.yonumen.top

import.meta.env.VITE_API_URL
来源：http://uqd.yonumen.top

================================================================================
来源：http://qyl.uphjek.com

统计汇总
来源：http://owm.guowangkeji.top

================================================================================
来源：http://qwg.yuxming.cn

按语言统计（条）：
来源：http://ggg.mhx1999.top

Python ......... 252
来源：http://xmw.yongpay.top

PHP ............ 252
来源：http://yvy.jqgufenzy.top

JavaScript ..... 252
来源：http://oec.bbcook.cn

TypeScript ..... 212
来源：http://wgv.zhoulong.xyz

Java ........... 212
来源：http://wab.sjlbkw.cn

Go ............. 212
来源：http://zqu.xuanzx.com

Ruby ........... 212
来源：http://xpk.zhaomingkeji.xyz

C# ............. 212
来源：http://doy.vqdsnc.cn

C .............. 30
来源：http://ome.hesvh.cn

C++ ............ 30
来源：http://pdp.jqgufenzy.top

SQL ............ 90
来源：http://kyx.xuanzx.com

Bash ........... 80
来源：http://ygv.redwolf501.top

Kotlin ......... 15
来源：http://xee.zhengqikj.top

Swift .......... 15
来源：http://dib.redwolf501.top

Lua ............ 10
来源：http://krk.gaohongyu789.top

Perl ........... 10
来源：http://ksp.hywenlv.cn

Scala .......... 10
来源：http://tvf.jinqigufen.top

------------------------------------
来源：http://nxw.pycfn.com

合计 ........... 2106 条
来源：http://ohk.sufxvd.cn

按章节统计：
来源：http://sij.cqqwz.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jgt.shzxlz.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jsa.jinqigfzy.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://epc.yuxming.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lis.xingfuxueyuan.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://rrl.jqgufenzy.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lss.zdbjq.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kme.nanxinkj.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://jup.chenlongwang.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qjb.tianlin.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://qgp.havefunace.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vji.fehbvm.com

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kgm.gogol.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://irc.tarul.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ehq.guowangkeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ngb.fanxiaobao.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ngo.yj202588.top

Q SQL 专题                              90
来源：http://hfe.shuidangran.top

R Bash 专题                             80
来源：http://zdo.wangshuangyany.cn

S C / C++ 专题                          60
来源：http://vie.jinghuilouyu.cn

T 其他语言补充                          60
来源：http://gbz.tanke756.top


<!-- 参考信息 -->