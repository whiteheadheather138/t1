代发 wailian999

val a = 1;  var b = 2
来源：http://ify.jlsjyb.cn

[T53] Scala：字符串插值
来源：http://npm.haohaochexian.top

s"值: $b"
来源：http://xrh.xylfe.cn

[T54] Scala：集合映射
来源：http://fjh.yangfankeji.com

List(1, 2, 3).map(_ * 2)
来源：http://hej.ydjk.org.cn

[T55] Scala：集合过滤
来源：http://fgq.snrcjt.cn

List(1, 2, 3).filter(_ > 1)
来源：http://buc.hesvh.cn

[T56] Scala：样例类
来源：http://qgf.0kj1m.cn

case class User(name: String, age: Int)
来源：http://mru.mhx1999.top

[T57] Scala：模式匹配
来源：http://cxp.aibaodan.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://upj.zhaomingkeji.xyz

[T58] Scala：函数定义
来源：http://vdo.jqgufenzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://bap.yanxiufei.cn

[T59] Scala：循环
来源：http://bba.hywenlv.cn

for (i <- 1 to 10) println(i)
来源：http://ktw.ctjpmb.com

[T60] Scala：折叠
来源：http://eju.cucudq.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mzy.xuanzx.com

================================================================================
来源：http://anx.shzxlz.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ihp.cashguo.top

================================================================================
来源：http://zhd.ctjpmb.com

[U01] Py：创建虚拟环境
来源：http://htj.cucudq.cn

python -m venv .venv && source .venv/bin/activate
来源：http://clg.9152youxi.cn

[U02] Py：导出 / 安装依赖
来源：http://hph.zhengqikj.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kua.yangfankeji.com

[U03] Py：加载 .env 配置
来源：http://rfu.yj20258888.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ljb.316326.xyz

[U04] Py：变量调试打印
来源：http://ewz.gotoacloud.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jmd.yj20258888.top

[U05] Py：列表去重且保序
来源：http://zrd.andypj.xyz

list(dict.fromkeys(arr))
来源：http://eoh.ppjwa.cn

[U06] Py：合并两个字典
来源：http://nxw.shuidangran.top

{**a, **b}
来源：http://nqs.zhijiandao.cn

[U07] Py：反转字典键值
来源：http://epk.tianlin.xyz

{v: k for k, v in d.items()}
来源：http://txw.mhx1999.top

[U08] Py：展平二维列表
来源：http://rgn.chenlongwang.top

[y for x in nested for y in x]
来源：http://mfd.pengpengdd.cyou

[U09] Py：字典取最大值的键
来源：http://eim.jinqigufen.top

max(d, key=d.get)
来源：http://zha.hcnkem.com

[U10] Py：按值排序字典
来源：http://ehx.gzhubu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sou.yj20258888.top

[U11] Py：生成器表达式
来源：http://jsz.shzxlz.cn

(x * 2 for x in arr)
来源：http://wrl.cheryme.top

[U12] Py：取出现最多的 3 个元素
来源：http://tut.sufxvd.cn

Counter(arr).most_common(3)
来源：http://omu.tanke756.top

[U13] Py：固定长度队列
来源：http://rmx.sweek.top

deque(maxlen=10)
来源：http://oes.kuanghao11.cn

[U14] Py：分组收集到列表
来源：http://xuj.nanxinkj.top

defaultdict(list)
来源：http://feh.yuxming.cn

[U15] Py：高精度计时
来源：http://plt.yuxming.cn

t = time.perf_counter()
来源：http://sns.vqdsnc.cn

[U16] Py：命令行参数解析
来源：http://snd.ivvv.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xax.nanxuanxn.top

[U17] Py：初始化日志
来源：http://cbf.cucudq.cn

logging.basicConfig(level=logging.INFO)
来源：http://evb.fanxiaobao.xyz

[U18] Py：预编译正则
来源：http://qeg.jinghuilouyu.cn

pat = re.compile(r"\d+")
来源：http://ars.iojbl.cn

[U19] Py：正则替换带回调
来源：http://ybw.kuanghao11.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tbj.redwolf501.top

[U20] Py：缓存函数结果
来源：http://scp.yvedp.cn

@functools.lru_cache(maxsize=None)
来源：http://jzl.jinghuilouyu.cn

[U21] Py：自定义上下文管理器
来源：http://gwd.kuanghao11.cn

@contextlib.contextmanager
来源：http://sov.quarkkingdee.top

[U22] Py：矩阵转置
来源：http://scw.jlsjyb.cn

list(zip(*m))
来源：http://gih.316326.xyz

[U23] Py：分块读取大文件
来源：http://yki.hnqzz.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gvu.chenlongwang.top

[U24] Py：路径操作
来源：http://asd.ctjpmb.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://udn.vehdjk.com

[U25] Py：CSV 按字典读
来源：http://orw.cdnleiting.top

csv.DictReader(f)
来源：http://zrm.vehdjk.com

[U26] Py：并发下载
来源：http://csh.hesvh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gah.0kj1m.cn

[U27] Py：异步 HTTP
来源：http://iub.chenjidiqi.icu

aiohttp.ClientSession() 配合 async with
来源：http://ptr.hysaishi.cn

[U28] Py：类型别名
来源：http://aft.meibo888.top

UserId = int
来源：http://dph.kuanghao11.cn

[U29] Py：属性校验
来源：http://duu.xuetiantiany.cn

@property 与 @x.setter 配合
来源：http://rfb.yuxming.cn

[U30] Py：数据类
来源：http://nim.0kj1m.cn

@dataclass(slots=True)
来源：http://apm.tarul.cn

[U31] Py：单测
来源：http://hgd.fehbvm.com

python -m pytest -q
来源：http://rnv.316326.xyz

[U32] Py：代码格式化
来源：http://uhb.yuanzhike.top

ruff format . && ruff check --fix .
来源：http://riq.jianghu66.top

[U33] Py：打包发布
来源：http://fpt.jyoumei.cn

python -m build  （依赖 pyproject.toml）
来源：http://exb.hcnkem.com

[U34] Py：判断编码
来源：http://iuo.vehdjk.com

chardet.detect(raw)
来源：http://gbb.cdnleiting.top

[U35] Py：发送邮件
来源：http://ryl.shuidangran.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mzd.tarul.cn

[U36] Py：定时任务
来源：http://lkw.fengsongda.top

schedule.every(10).minutes.do(job)
来源：http://cnt.haohaochexian.top

[U37] Py：读写 Excel
来源：http://dib.daria6918.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rrv.zhengqikj.top

[U38] Py：获取脚本所在目录
来源：http://sss.epnwcf.com

Path(__file__).resolve().parent
来源：http://wdr.ehwqpu.com

[U39] Py：判断是否在交互环境
来源：http://wah.jinqigfzy.top

sys.stdout.isatty()
来源：http://dtj.xingfuxueyuan.xyz

[U40] Py：打印到标准错误
来源：http://xai.yongpay.top

print("err", file=sys.stderr)
来源：http://evn.wangshuangyany.cn

[U41] PHP：初始化 Composer 项目
来源：http://scz.zhengqikj.top

composer init;  composer require guzzlehttp/guzzle
来源：http://fgw.zycfv.cn

[U42] PHP：PSR-4 自动加载
来源：http://pis.jinqigfzy.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sgc.yanxiufei.cn

[U43] PHP：声明命名空间
来源：http://iui.ehwqpu.com

namespace App\Http;
来源：http://wgg.hongshengwenyu.top

[U44] PHP：开启严格类型
来源：http://ven.zdbjq.cn

declare(strict_types=1);
来源：http://syn.tianlin.xyz

[U45] PHP：类型声明与返回类型
来源：http://ldl.yueranfly.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://kcs.cdnleiting.top

[U46] PHP：可空类型
来源：http://epw.yj202588.top

?string $name = null
来源：http://tsu.xziqi.cn

[U47] PHP：联合类型
来源：http://sja.zhiwuduotai.top

int|string $id
来源：http://xls.ctjpmb.com

[U48] PHP：纯枚举
来源：http://fcf.zhixingplan.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vjo.xinyue.icu

[U49] PHP：只读属性
来源：http://tmg.ydjk.org.cn

public readonly string $name
来源：http://lxj.daxiang520.top

[U50] PHP：构造器属性提升
来源：http://sfe.jinqigfzy.top

public function __construct(private int $id) {}
来源：http://yuc.aibaodan.cn

[U51] PHP：数组解构
来源：http://ehd.dianchejie.cn

[$a, $b] = $arr;
来源：http://vxq.nanxuanxn.top

[U52] PHP：箭头函数
来源：http://kfu.zhaomingkeji.xyz

$double = fn($x) => $x * 2;
来源：http://jwe.ivvv.top

[U53] PHP：空合并运算符
来源：http://unv.tarul.cn

$v = $a ?? $b ?? "default";
来源：http://rap.chenzaomai.com

[U54] PHP：空安全调用
来源：http://tqb.hysaishi.cn

$obj?->method()
来源：http://kqe.dashuyun.cn

[U55] PHP：match 表达式
来源：http://udu.ivvv.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dha.ppjwa.cn

[U56] PHP：命名参数
来源：http://mxo.nwbrower.top

f(a: 1, b: 2)
来源：http://usk.iojbl.cn

[U57] PHP：字符串插值
来源：http://vlc.kuanghao11.cn

"值: {$a}"
来源：http://hlr.cucudq.cn

[U58] PHP：数组三件套
来源：http://wen.fehbvm.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fau.quarkkingdee.top

[U59] PHP：自定义排序
来源：http://sgb.ppjwa.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qnh.jinghuilouyu.cn

[U60] PHP：JSON 编解码
来源：http://evh.jqgfzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qbt.fzhhl.top

[U61] PHP：正则
来源：http://fhx.yuxming.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wor.hnqzz.top

[U62] PHP：日期对象
来源：http://zha.fktsv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rfg.guannengcc.top

[U63] PHP：文件读写
来源：http://ptc.nanxuanxn.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cie.ivvv.top

[U64] PHP：目录遍历
来源：http://seu.ehwqpu.com

glob("dir/*.php");  scandir("dir");
来源：http://rrx.yangfankeji.com

[U65] PHP：会话
来源：http://tbs.hywenlv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rsg.tanke756.top

[U66] PHP：设置 Cookie
来源：http://yuv.shanyushiyangkeji.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fyh.yvedp.cn

[U67] PHP：处理文件上传
来源：http://kzt.andypj.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jvj.iojbl.cn

[U68] PHP：PDO 连接
来源：http://isz.cqqwz.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gyh.yj20258888.top

[U69] PHP：PDO 预处理
来源：http://iwl.zhaomingkeji.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qke.gotoacloud.top

[U70] PHP：PDO 事务
来源：http://thz.zhiwuduotai.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ogu.xinyue.icu

[U71] PHP：抛出异常
来源：http://lgv.ppjwa.cn

throw new RuntimeException("失败", 500);
来源：http://yyf.xuetiantiany.cn

[U72] PHP：写错误日志
来源：http://ril.pengpengdd.cyou

error_log("失败: " . $e->getMessage());
来源：http://ypw.yfazqb.com

[U73] PHP：读取 ini 配置
来源：http://hgn.iojbl.cn

parse_ini_file("config.ini", true)
来源：http://het.tianlin.xyz

[U74] PHP：读取环境变量
来源：http://dec.sysykeji.top

getenv("APP_ENV") ?: "production"
来源：http://wsd.cashguo.top

[U75] PHP：依赖注入
来源：http://azb.zhijiandao.cn

composer require psr/container
来源：http://myr.daria6918.cn

[U76] PHP：简单路由
来源：http://ueg.zhaomingkeji.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zqg.shanyushiyangkeji.top

[U77] PHP：模板渲染
来源：http://oiz.haohaochexian.top

composer require twig/twig
来源：http://ckv.wangdashe.top

[U78] PHP：单元测试
来源：http://bxz.zhaomingkeji.xyz

composer require --dev phpunit/phpunit
来源：http://jgr.yueranfly.top

[U79] PHP：静态分析
来源：http://fiz.sufxvd.cn

composer require --dev phpstan/phpstan
来源：http://gwf.zhengqikj.top

[U80] PHP：代码规范修复
来源：http://cne.zhongyouzk.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ldd.jinyuanbaomall.cn

[U81] JS：初始化项目
来源：http://mpv.epnwcf.com

npm init -y;  npm i express
来源：http://jwl.zycfv.cn

[U82] JS：package.json 脚本
来源：http://okl.shzxlz.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vtt.yanxiufei.cn

[U83] JS：ES Module 导入导出
来源：http://hjt.xinyue.icu

export const a = 1;  import { a } from "./m.js";
来源：http://owx.gaohongyu789.top

[U84] JS：CommonJS 写法
来源：http://ell.bbcook.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qwd.gotoacloud.top

[U85] JS：可选链
来源：http://bjv.meibo888.top

a?.b?.c
来源：http://nuy.pycfn.com

[U86] JS：空值合并
来源：http://scg.chenjidiqi.icu

a ?? b
来源：http://sqv.hcnkem.com

[U87] JS：解构默认值
来源：http://mwb.shuidangran.top

const { a = 1, b = 2 } = obj;
来源：http://lmf.yj20258888.top

[U88] JS：对象展开合并
来源：http://xmn.smart0.xyz

{ ...a, ...b }
来源：http://nyv.cqqwz.cn

[U89] JS：数组去重
来源：http://uzt.gaohongyu789.top

[...new Set(arr)]
来源：http://evp.zhongyouzk.top

[U90] JS：数字数组排序
来源：http://edh.meibo888.top

[...arr].sort((a, b) => a - b)
来源：http://pzl.hesvh.cn

[U91] JS：对象键值遍历
来源：http://smp.iojbl.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xyg.dianchejie.cn

[U92] JS：深拷贝
来源：http://tyj.9152youxi.cn

structuredClone(obj)
来源：http://jtg.sufxvd.cn

[U93] JS：模板字符串
来源：http://kko.sjlbkw.cn

`共 ${n} 条`
来源：http://dci.tian-w.cn

[U94] JS：箭头函数
来源：http://jhr.zhongyouzk.top

const double = x => x * 2;
来源：http://mqi.xinyue.icu

[U95] JS：Promise 包装
来源：http://mvb.redwolf501.top

new Promise((resolve, reject) => {})
来源：http://lon.0kj1m.cn

[U96] JS：async/await 与异常
来源：http://rgd.shanyushiyangtech.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://buj.zhijiandao.cn

[U97] JS：并发请求
来源：http://ktn.jinqigfzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://rwj.birdmap.top

[U98] JS：fetch 带 JSON
来源：http://jiq.nwbrower.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ebz.zdqjudy.top

[U99] JS：事件监听
来源：http://wmi.jqgufenzy.top

el.addEventListener("click", e => {})
来源：http://kqw.yuanzhike.top

[U100] JS：DOM 查询
来源：http://hap.vqdsnc.cn

document.querySelector(".item")
来源：http://ycu.ehwqpu.com

[U101] JS：classList 操作
来源：http://sdq.havefunace.top

el.classList.toggle("active")
来源：http://wgh.hongshengwenyu.top

[U102] JS：本地存储
来源：http://bbu.cashguo.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://fwt.yfazqb.com

[U103] JS：定时器
来源：http://hzx.vehdjk.com

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://adh.jinqigfzy.top

[U104] JS：防抖
来源：http://tvn.feifeiyinyue.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://axj.yangfankeji.com

[U105] JS：节流
来源：http://rhq.hysaishi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zpu.sxryk.cn

[U106] JS：日期格式化
来源：http://erg.shanyushiyangkeji.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tcn.tanke756.top

[U107] JS：数字千分位
来源：http://gvx.wangdashe.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qyw.c1oappe.top

[U108] JS：随机整数
来源：http://bmv.bjfxy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://opd.yj20258888.top

[U109] JS：数组分组
来源：http://gms.daxiang520.top

Object.groupBy(arr, x => x.type)
来源：http://dtn.fanxiaobao.xyz

[U110] JS：数组分块
来源：http://nri.fktsv.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vyl.jqgfzy.top

[U111] JS：对象转 Map
来源：http://nbv.zhoulong.xyz

new Map(Object.entries(obj))
来源：http://zdk.feifeiyinyue.top

[U112] JS：字符串补位
来源：http://ciq.cqqwz.cn

"7".padStart(3, "0")
来源：http://lji.daria6918.cn

[U113] JS：正则替换全部
来源：http://zvg.jqgfzy.top

s.replaceAll("a", "b")
来源：http://okz.zhaomingkeji.xyz

[U114] JS：JSON 深比较
来源：http://rzh.chenlongwang.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://njj.redwolf501.top

[U115] JS：生成 UUID
来源：http://xol.fanxiaobao.xyz

crypto.randomUUID()
来源：http://rmo.jinghuilouyu.cn

[U116] JS：类型检查（JSDoc）
来源：http://kot.ehwqpu.com

/** @param {string} name */ function f(name) {}
来源：http://coo.iojbl.cn

[U117] JS：单元测试
来源：http://zdn.birdmap.top

npm i -D vitest;  npx vitest
来源：http://wxl.xuanzx.com

[U118] JS：开发服务器
来源：http://ypd.jinqigufen.top

npm i -D vite;  npx vite
来源：http://gcu.yfazqb.com

[U119] JS：生产构建
来源：http://mhv.chenzaomai.com

npx vite build
来源：http://ybs.9152youxi.cn

[U120] JS：读取环境变量（Vite）
来源：http://urp.vehdjk.com

import.meta.env.VITE_API_URL
来源：http://xcu.gogol.net.cn

================================================================================
来源：http://asj.yj20258888.top

统计汇总
来源：http://egr.yfazqb.com

================================================================================
来源：http://hkg.yanxiufei.cn

按语言统计（条）：
来源：http://tag.haohaochexian.top

Python ......... 252
来源：http://vrp.ivvv.top

PHP ............ 252
来源：http://utt.sufxvd.cn

JavaScript ..... 252
来源：http://ybe.guowangkeji.top

TypeScript ..... 212
来源：http://vte.chenzaomai.com

Java ........... 212
来源：http://ykh.jianghu66.top

Go ............. 212
来源：http://qpc.yuxming.cn

Ruby ........... 212
来源：http://vhx.kuanghao11.cn

C# ............. 212
来源：http://jnw.tanke756.top

C .............. 30
来源：http://dcg.yonumen.top

C++ ............ 30
来源：http://qcs.xingfuxueyuan.xyz

SQL ............ 90
来源：http://ckj.cheryme.top

Bash ........... 80
来源：http://pvt.feifeiyinyue.top

Kotlin ......... 15
来源：http://jlo.hfpthk.cn

Swift .......... 15
来源：http://svh.shzxlz.cn

Lua ............ 10
来源：http://ddn.tian-w.cn

Perl ........... 10
来源：http://ref.xylfe.cn

Scala .......... 10
来源：http://dfc.chenzaomai.com

------------------------------------
来源：http://jqu.aibaodan.cn

合计 ........... 2106 条
来源：http://lds.wangdashe.top

按章节统计：
来源：http://wyz.ydjk.org.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xlp.xingfuxueyuan.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nnn.ppjwa.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vqx.zhijiandao.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gdw.yfazqb.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sjc.nanxinkj.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pve.hongshengwenyu.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fjo.ppjwa.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://edz.yuxming.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ezw.yj20258888.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tfz.gzhubu.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ghy.chenjidiqi.icu

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rgd.52xcode.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rqo.daxiang520.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jbi.pengpengdd.cyou

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://lvu.zycfv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ana.zhijiandao.cn


<!-- 参考信息 -->