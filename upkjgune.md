代发 wailian999

val a = 1;  var b = 2
来源：http://lbc.shanyushiyangtech.top

[T53] Scala：字符串插值
来源：http://jlj.nanxinkj.top

s"值: $b"
来源：http://iml.gogol.net.cn

[T54] Scala：集合映射
来源：http://vat.sxryk.cn

List(1, 2, 3).map(_ * 2)
来源：http://wrh.jyoumei.cn

[T55] Scala：集合过滤
来源：http://dyq.zhongyouzk.top

List(1, 2, 3).filter(_ > 1)
来源：http://csn.chenlongwang.top

[T56] Scala：样例类
来源：http://znb.snrcjt.cn

case class User(name: String, age: Int)
来源：http://nsf.fanxiaobao.xyz

[T57] Scala：模式匹配
来源：http://ffw.xuetiantiany.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xdq.bbcook.cn

[T58] Scala：函数定义
来源：http://ltb.gogol.net.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xkk.bjfxy.top

[T59] Scala：循环
来源：http://xyt.hesvh.cn

for (i <- 1 to 10) println(i)
来源：http://zku.jqgufenzy.top

[T60] Scala：折叠
来源：http://cuz.hywenlv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://eta.cashguo.top

================================================================================
来源：http://noe.zhoulong.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://atg.9152youxi.cn

================================================================================
来源：http://nty.yfazqb.com

[U01] Py：创建虚拟环境
来源：http://hji.gaohongyu789.top

python -m venv .venv && source .venv/bin/activate
来源：http://ttm.yonumen.top

[U02] Py：导出 / 安装依赖
来源：http://zun.shanyushiyangtech.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jzt.hnqzz.top

[U03] Py：加载 .env 配置
来源：http://oin.wangdashe.top

from dotenv import load_dotenv; load_dotenv()
来源：http://tlo.jqgfzy.top

[U04] Py：变量调试打印
来源：http://qhz.chenjidiqi.icu

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sro.iojbl.cn

[U05] Py：列表去重且保序
来源：http://qfg.daria6918.cn

list(dict.fromkeys(arr))
来源：http://tgz.pengpengdd.cyou

[U06] Py：合并两个字典
来源：http://pej.aibaodan.cn

{**a, **b}
来源：http://qui.ydzc1.top

[U07] Py：反转字典键值
来源：http://wng.yonumen.top

{v: k for k, v in d.items()}
来源：http://cgq.ivvv.top

[U08] Py：展平二维列表
来源：http://vjx.sxryk.cn

[y for x in nested for y in x]
来源：http://xyr.wangdashe.top

[U09] Py：字典取最大值的键
来源：http://kai.fzhhl.top

max(d, key=d.get)
来源：http://nty.haohaochexian.top

[U10] Py：按值排序字典
来源：http://uky.9152youxi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nlt.yj20258.top

[U11] Py：生成器表达式
来源：http://zrm.yongpay.top

(x * 2 for x in arr)
来源：http://ajd.ybcxt.top

[U12] Py：取出现最多的 3 个元素
来源：http://voa.tian-w.cn

Counter(arr).most_common(3)
来源：http://pwm.daxiang520.top

[U13] Py：固定长度队列
来源：http://otd.ehwqpu.com

deque(maxlen=10)
来源：http://vjc.ppjwa.cn

[U14] Py：分组收集到列表
来源：http://miw.vqdsnc.cn

defaultdict(list)
来源：http://tiw.jiagoushi.top

[U15] Py：高精度计时
来源：http://qrn.nwbrower.top

t = time.perf_counter()
来源：http://adt.shanyushiyangtech.top

[U16] Py：命令行参数解析
来源：http://hpv.xinyue.icu

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xan.zdbjq.cn

[U17] Py：初始化日志
来源：http://ljd.yueranfly.top

logging.basicConfig(level=logging.INFO)
来源：http://hza.andypj.xyz

[U18] Py：预编译正则
来源：http://fac.jyoumei.cn

pat = re.compile(r"\d+")
来源：http://wvc.nanxinkj.top

[U19] Py：正则替换带回调
来源：http://npo.redwolf501.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yfl.xziqi.cn

[U20] Py：缓存函数结果
来源：http://xcd.0kj1m.cn

@functools.lru_cache(maxsize=None)
来源：http://dnp.epnwcf.com

[U21] Py：自定义上下文管理器
来源：http://jxk.hongshengwenyu.top

@contextlib.contextmanager
来源：http://xzt.sxryk.cn

[U22] Py：矩阵转置
来源：http://gma.sxryk.cn

list(zip(*m))
来源：http://jit.redwolf501.top

[U23] Py：分块读取大文件
来源：http://xvo.zdqjudy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qjc.sjlbkw.cn

[U24] Py：路径操作
来源：http://asr.vqdsnc.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lcp.dashuyun.cn

[U25] Py：CSV 按字典读
来源：http://iij.hongshengwenyu.top

csv.DictReader(f)
来源：http://xau.quarkkingdee.top

[U26] Py：并发下载
来源：http://iis.quarkkingdee.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vov.316326.xyz

[U27] Py：异步 HTTP
来源：http://aqy.fehbvm.com

aiohttp.ClientSession() 配合 async with
来源：http://ygi.cucudq.cn

[U28] Py：类型别名
来源：http://kuj.redwolf501.top

UserId = int
来源：http://jds.shuidangran.top

[U29] Py：属性校验
来源：http://xfr.jinyuanbaomall.cn

@property 与 @x.setter 配合
来源：http://ghp.daxiang520.top

[U30] Py：数据类
来源：http://xjl.fzhhl.top

@dataclass(slots=True)
来源：http://jzk.yongpay.top

[U31] Py：单测
来源：http://zoi.yj202588.top

python -m pytest -q
来源：http://asm.bbcook.cn

[U32] Py：代码格式化
来源：http://etm.xinyue.icu

ruff format . && ruff check --fix .
来源：http://fsf.hysaishi.cn

[U33] Py：打包发布
来源：http://tnx.hysaishi.cn

python -m build  （依赖 pyproject.toml）
来源：http://edu.shuidangran.top

[U34] Py：判断编码
来源：http://usg.jyoumei.cn

chardet.detect(raw)
来源：http://tad.nwbrower.top

[U35] Py：发送邮件
来源：http://elj.shanyushiyangkeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bqx.fanxiaobao.xyz

[U36] Py：定时任务
来源：http://ydj.sysykeji.top

schedule.every(10).minutes.do(job)
来源：http://wds.316326.xyz

[U37] Py：读写 Excel
来源：http://flo.meibo888.top

pandas.read_excel / DataFrame.to_excel
来源：http://ebn.feifeiyinyue.top

[U38] Py：获取脚本所在目录
来源：http://opa.jyoumei.cn

Path(__file__).resolve().parent
来源：http://fve.cashguo.top

[U39] Py：判断是否在交互环境
来源：http://utg.ctjpmb.com

sys.stdout.isatty()
来源：http://zpx.hysaishi.cn

[U40] Py：打印到标准错误
来源：http://uku.sxryk.cn

print("err", file=sys.stderr)
来源：http://kfx.ywan-chungtsiang.top

[U41] PHP：初始化 Composer 项目
来源：http://qbr.ppjwa.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hgi.yongpay.top

[U42] PHP：PSR-4 自动加载
来源：http://vcy.snrcjt.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lvq.xziqi.cn

[U43] PHP：声明命名空间
来源：http://nvp.chenjidiqi.icu

namespace App\Http;
来源：http://elb.jinqigfzy.top

[U44] PHP：开启严格类型
来源：http://gcn.cashguo.top

declare(strict_types=1);
来源：http://xpi.jinghuilouyu.cn

[U45] PHP：类型声明与返回类型
来源：http://dwu.hnqzz.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://vgw.daria6918.cn

[U46] PHP：可空类型
来源：http://lwt.jinqigufen.top

?string $name = null
来源：http://mwr.andypj.xyz

[U47] PHP：联合类型
来源：http://efa.snrcjt.cn

int|string $id
来源：http://wmw.wangshuangyany.cn

[U48] PHP：纯枚举
来源：http://lnq.zdbjq.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bso.mhx1999.top

[U49] PHP：只读属性
来源：http://pzq.ybcxt.top

public readonly string $name
来源：http://zgm.hesvh.cn

[U50] PHP：构造器属性提升
来源：http://rrv.c1oappe.top

public function __construct(private int $id) {}
来源：http://xgh.vehdjk.com

[U51] PHP：数组解构
来源：http://get.ppjwa.cn

[$a, $b] = $arr;
来源：http://ktv.zhongyouzk.top

[U52] PHP：箭头函数
来源：http://bck.wangshuangyany.cn

$double = fn($x) => $x * 2;
来源：http://tac.tianlin.xyz

[U53] PHP：空合并运算符
来源：http://nst.ybcxt.top

$v = $a ?? $b ?? "default";
来源：http://tlq.uphjek.com

[U54] PHP：空安全调用
来源：http://zjb.cheryme.top

$obj?->method()
来源：http://vwa.nwbrower.top

[U55] PHP：match 表达式
来源：http://kjh.sjlbkw.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lsq.havefunace.top

[U56] PHP：命名参数
来源：http://ipw.yfazqb.com

f(a: 1, b: 2)
来源：http://iwz.ivvv.top

[U57] PHP：字符串插值
来源：http://fpg.chenjidiqi.icu

"值: {$a}"
来源：http://wgl.dashuyun.cn

[U58] PHP：数组三件套
来源：http://jqy.redwolf501.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kge.hysaishi.cn

[U59] PHP：自定义排序
来源：http://dly.yj20258.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cin.gogol.net.cn

[U60] PHP：JSON 编解码
来源：http://bev.feifeiyinyue.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lak.cheryme.top

[U61] PHP：正则
来源：http://yan.guannengcc.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://inv.tarul.cn

[U62] PHP：日期对象
来源：http://efw.jqgufenzy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://etl.tianlin.xyz

[U63] PHP：文件读写
来源：http://yco.sweek.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vdz.0kj1m.cn

[U64] PHP：目录遍历
来源：http://nzx.guowangkeji.top

glob("dir/*.php");  scandir("dir");
来源：http://zqk.hfpthk.cn

[U65] PHP：会话
来源：http://ndm.yuanzhike.top

session_start();  $_SESSION["uid"] = 1;
来源：http://nzt.jlsjyb.cn

[U66] PHP：设置 Cookie
来源：http://gpv.shangyingyoupin.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://olj.quarkkingdee.top

[U67] PHP：处理文件上传
来源：http://njy.tanke756.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ssf.yj20258888.top

[U68] PHP：PDO 连接
来源：http://pfi.feifeiyinyue.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cxw.tanke756.top

[U69] PHP：PDO 预处理
来源：http://ovg.svipenyu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hoj.c1oappe.top

[U70] PHP：PDO 事务
来源：http://soq.yuxming.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dhw.wangshuangyany.cn

[U71] PHP：抛出异常
来源：http://xar.zdbjq.cn

throw new RuntimeException("失败", 500);
来源：http://edi.ydzc1.top

[U72] PHP：写错误日志
来源：http://vlp.nwbrower.top

error_log("失败: " . $e->getMessage());
来源：http://gdm.fzhhl.top

[U73] PHP：读取 ini 配置
来源：http://bnb.hcnkem.com

parse_ini_file("config.ini", true)
来源：http://gri.fanxiaobao.xyz

[U74] PHP：读取环境变量
来源：http://wph.hfpthk.cn

getenv("APP_ENV") ?: "production"
来源：http://fyw.hcnkem.com

[U75] PHP：依赖注入
来源：http://xiz.hammf.cn

composer require psr/container
来源：http://qxs.52xcode.cn

[U76] PHP：简单路由
来源：http://kxm.shanyushiyangtech.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uri.tanke756.top

[U77] PHP：模板渲染
来源：http://fle.hysaishi.cn

composer require twig/twig
来源：http://bgl.xuanzx.com

[U78] PHP：单元测试
来源：http://rnx.tarul.cn

composer require --dev phpunit/phpunit
来源：http://kjx.havefunace.top

[U79] PHP：静态分析
来源：http://ewe.tanke756.top

composer require --dev phpstan/phpstan
来源：http://vmr.hesvh.cn

[U80] PHP：代码规范修复
来源：http://kla.zhaomingkeji.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://szc.jinqigfzy.top

[U81] JS：初始化项目
来源：http://nrc.ppjwa.cn

npm init -y;  npm i express
来源：http://fyp.hammf.cn

[U82] JS：package.json 脚本
来源：http://lrn.nanxinkj.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://prt.xinyue.icu

[U83] JS：ES Module 导入导出
来源：http://xgf.hcnkem.com

export const a = 1;  import { a } from "./m.js";
来源：http://pin.chenzaomai.com

[U84] JS：CommonJS 写法
来源：http://lsi.sysykeji.top

module.exports = { a };  const { a } = require("./m");
来源：http://gqw.haohaochexian.top

[U85] JS：可选链
来源：http://aha.316326.xyz

a?.b?.c
来源：http://mie.andypj.xyz

[U86] JS：空值合并
来源：http://wlh.vehdjk.com

a ?? b
来源：http://pnm.shanyushiyangtech.top

[U87] JS：解构默认值
来源：http://ftp.nanxinkj.top

const { a = 1, b = 2 } = obj;
来源：http://olu.shzxlz.cn

[U88] JS：对象展开合并
来源：http://pnc.feifeiyinyue.top

{ ...a, ...b }
来源：http://sca.cucudq.cn

[U89] JS：数组去重
来源：http://vmi.sysykeji.top

[...new Set(arr)]
来源：http://ijh.yj202588.top

[U90] JS：数字数组排序
来源：http://czm.hammf.cn

[...arr].sort((a, b) => a - b)
来源：http://nbp.jinyuanbaomall.cn

[U91] JS：对象键值遍历
来源：http://iys.zhiwuduotai.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://cjs.yongpay.top

[U92] JS：深拷贝
来源：http://nex.sxryk.cn

structuredClone(obj)
来源：http://whs.mhx1999.top

[U93] JS：模板字符串
来源：http://gtt.yangfankeji.com

`共 ${n} 条`
来源：http://pnd.sufxvd.cn

[U94] JS：箭头函数
来源：http://kvi.9152youxi.cn

const double = x => x * 2;
来源：http://xps.jinyuanbaomall.cn

[U95] JS：Promise 包装
来源：http://wio.zhoulong.xyz

new Promise((resolve, reject) => {})
来源：http://gkj.vqdsnc.cn

[U96] JS：async/await 与异常
来源：http://nya.sweek.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uij.shanyushiyangtech.top

[U97] JS：并发请求
来源：http://xad.bjfxy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://uwt.yueranfly.top

[U98] JS：fetch 带 JSON
来源：http://hqk.chenjidiqi.icu

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pak.chenzaomai.com

[U99] JS：事件监听
来源：http://bgh.zhixingplan.top

el.addEventListener("click", e => {})
来源：http://zvx.jlsjyb.cn

[U100] JS：DOM 查询
来源：http://jsa.yangfankeji.com

document.querySelector(".item")
来源：http://xho.pycfn.com

[U101] JS：classList 操作
来源：http://hqy.ybcxt.top

el.classList.toggle("active")
来源：http://adr.gaohongyu789.top

[U102] JS：本地存储
来源：http://qst.jinqigfzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://xqu.guannengcc.top

[U103] JS：定时器
来源：http://tzn.yuanzhike.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tla.hnxiangtu.top

[U104] JS：防抖
来源：http://juc.daria6918.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tjg.cheryme.top

[U105] JS：节流
来源：http://ykq.fzhhl.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rke.tian-w.cn

[U106] JS：日期格式化
来源：http://bim.ivvv.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nfq.wangdashe.top

[U107] JS：数字千分位
来源：http://ihn.pengpengdd.cyou

new Intl.NumberFormat("en-US").format(1234567)
来源：http://okq.svipenyu.cn

[U108] JS：随机整数
来源：http://ccf.gogol.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rll.sufxvd.cn

[U109] JS：数组分组
来源：http://rdj.xinyue.icu

Object.groupBy(arr, x => x.type)
来源：http://rtr.chenzaomai.com

[U110] JS：数组分块
来源：http://uyr.havefunace.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cfs.hcnkem.com

[U111] JS：对象转 Map
来源：http://eln.mhx1999.top

new Map(Object.entries(obj))
来源：http://mng.feifeiyinyue.top

[U112] JS：字符串补位
来源：http://jiz.hnxiangtu.top

"7".padStart(3, "0")
来源：http://iva.zhaomingkeji.xyz

[U113] JS：正则替换全部
来源：http://pam.yonumen.top

s.replaceAll("a", "b")
来源：http://qec.haohaochexian.top

[U114] JS：JSON 深比较
来源：http://zbw.vqdsnc.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tzt.tianlin.xyz

[U115] JS：生成 UUID
来源：http://nqx.ydjk.org.cn

crypto.randomUUID()
来源：http://myq.yj202588.top

[U116] JS：类型检查（JSDoc）
来源：http://opc.yfazqb.com

/** @param {string} name */ function f(name) {}
来源：http://nlw.zhaomingkeji.xyz

[U117] JS：单元测试
来源：http://ecm.zhoulong.xyz

npm i -D vitest;  npx vitest
来源：http://pkn.hammf.cn

[U118] JS：开发服务器
来源：http://fxp.shangyingyoupin.top

npm i -D vite;  npx vite
来源：http://rpk.nwbrower.top

[U119] JS：生产构建
来源：http://gzh.nanxuanxn.top

npx vite build
来源：http://gqv.yfazqb.com

[U120] JS：读取环境变量（Vite）
来源：http://ytz.gogol.net.cn

import.meta.env.VITE_API_URL
来源：http://awa.pengpengdd.cyou

================================================================================
来源：http://xpa.zdqjudy.top

统计汇总
来源：http://bfq.jlsjyb.cn

================================================================================
来源：http://byi.9152youxi.cn

按语言统计（条）：
来源：http://olr.hnxiangtu.top

Python ......... 252
来源：http://hzh.birdmap.top

PHP ............ 252
来源：http://xgh.yonumen.top

JavaScript ..... 252
来源：http://ndz.jinyuanbaomall.cn

TypeScript ..... 212
来源：http://izw.nanxuanxn.top

Java ........... 212
来源：http://plu.shuidangran.top

Go ............. 212
来源：http://jtc.pycfn.com

Ruby ........... 212
来源：http://xda.sysykeji.top

C# ............. 212
来源：http://avb.jyoumei.cn

C .............. 30
来源：http://ans.dashuyun.cn

C++ ............ 30
来源：http://woc.sysykeji.top

SQL ............ 90
来源：http://tgl.shanyushiyangkeji.top

Bash ........... 80
来源：http://rvu.yj202588.top

Kotlin ......... 15
来源：http://pio.ehwqpu.com

Swift .......... 15
来源：http://fjn.316326.xyz

Lua ............ 10
来源：http://xxi.fengsongda.top

Perl ........... 10
来源：http://oyh.fanxiaobao.xyz

Scala .......... 10
来源：http://lag.yj20258.top

------------------------------------
来源：http://xnh.hnxiangtu.top

合计 ........... 2106 条
来源：http://mau.quarkkingdee.top

按章节统计：
来源：http://aqk.gogol.net.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://iqz.chenzaomai.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zff.fktsv.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jbs.daxiang520.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bpb.pycfn.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sbm.yanxiufei.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vbn.hysaishi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tiw.yangfankeji.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nqk.aizwys.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cmj.jiagoushi.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://prt.yfazqb.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bwn.shzxlz.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wdv.jinghuilouyu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gql.iojbl.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dje.dashuyun.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://krn.snrcjt.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bvi.dashuyun.cn


<!-- 参考信息 -->