代发 wailian999

[T49] Perl：函数
来源：http://wng.zhixingplan.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pio.aizwys.cn

[T50] Perl：逐行读文件
来源：http://stc.bjfxy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://qgj.ppjwa.cn

while (my $line = <$fh>) { print $line; }
来源：http://wox.cucudq.cn

[T51] Scala：Hello World
来源：http://zqi.redwolf501.top

println("Hello")
来源：http://fug.gogol.net.cn

[T52] Scala：变量
来源：http://rst.sysykeji.top

val a = 1;  var b = 2
来源：http://uty.0kj1m.cn

[T53] Scala：字符串插值
来源：http://gat.zhengqikj.top

s"值: $b"
来源：http://msc.gotoacloud.top

[T54] Scala：集合映射
来源：http://twn.jinqigufen.top

List(1, 2, 3).map(_ * 2)
来源：http://ddt.xziqi.cn

[T55] Scala：集合过滤
来源：http://ptg.ctjpmb.com

List(1, 2, 3).filter(_ > 1)
来源：http://wuj.cucudq.cn

[T56] Scala：样例类
来源：http://qyr.vehdjk.com

case class User(name: String, age: Int)
来源：http://gbd.sufxvd.cn

[T57] Scala：模式匹配
来源：http://ppx.jinghuilouyu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ket.zhiwuduotai.top

[T58] Scala：函数定义
来源：http://uyy.mhx1999.top

def add(a: Int, b: Int): Int = a + b
来源：http://qkv.zycfv.cn

[T59] Scala：循环
来源：http://pom.nanxinkj.top

for (i <- 1 to 10) println(i)
来源：http://ked.chenlongwang.top

[T60] Scala：折叠
来源：http://thz.jiagoushi.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gah.zycfv.cn

================================================================================
来源：http://ppt.zdbjq.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jyb.bbcook.cn

================================================================================
来源：http://tyh.epnwcf.com

[U01] Py：创建虚拟环境
来源：http://lcb.zycfv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gih.hammf.cn

[U02] Py：导出 / 安装依赖
来源：http://lga.yuanzhike.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ghc.shanyushiyangkeji.top

[U03] Py：加载 .env 配置
来源：http://ngk.yueranfly.top

from dotenv import load_dotenv; load_dotenv()
来源：http://xzl.iojbl.cn

[U04] Py：变量调试打印
来源：http://jwa.daria6918.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kby.gogol.net.cn

[U05] Py：列表去重且保序
来源：http://ufo.jinqigufen.top

list(dict.fromkeys(arr))
来源：http://wzw.chenjidiqi.icu

[U06] Py：合并两个字典
来源：http://gmi.svipenyu.cn

{**a, **b}
来源：http://wfz.daxiang520.top

[U07] Py：反转字典键值
来源：http://hky.cheryme.top

{v: k for k, v in d.items()}
来源：http://zdz.sweek.top

[U08] Py：展平二维列表
来源：http://wcq.daria6918.cn

[y for x in nested for y in x]
来源：http://tnl.chenlongwang.top

[U09] Py：字典取最大值的键
来源：http://nhf.c1oappe.top

max(d, key=d.get)
来源：http://hnv.hcnkem.com

[U10] Py：按值排序字典
来源：http://rkg.jqgufenzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ynl.yj202588.top

[U11] Py：生成器表达式
来源：http://lpp.dianchejie.cn

(x * 2 for x in arr)
来源：http://dgb.fzhhl.top

[U12] Py：取出现最多的 3 个元素
来源：http://zgt.zhengqikj.top

Counter(arr).most_common(3)
来源：http://vhb.birdmap.top

[U13] Py：固定长度队列
来源：http://vee.tanke756.top

deque(maxlen=10)
来源：http://kfy.fktsv.cn

[U14] Py：分组收集到列表
来源：http://cte.xuetiantiany.cn

defaultdict(list)
来源：http://ztt.shanyushiyangtech.top

[U15] Py：高精度计时
来源：http://uot.sysykeji.top

t = time.perf_counter()
来源：http://wmq.sufxvd.cn

[U16] Py：命令行参数解析
来源：http://jed.yj20258.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bfg.mhx1999.top

[U17] Py：初始化日志
来源：http://inz.316326.xyz

logging.basicConfig(level=logging.INFO)
来源：http://tik.nwbrower.top

[U18] Py：预编译正则
来源：http://slw.jinqigfzy.top

pat = re.compile(r"\d+")
来源：http://ewp.yongpay.top

[U19] Py：正则替换带回调
来源：http://ilh.yanxiufei.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://red.gotoacloud.top

[U20] Py：缓存函数结果
来源：http://ihp.ydjk.org.cn

@functools.lru_cache(maxsize=None)
来源：http://yfq.jlsjyb.cn

[U21] Py：自定义上下文管理器
来源：http://nmx.meibo888.top

@contextlib.contextmanager
来源：http://pqq.chenlongwang.top

[U22] Py：矩阵转置
来源：http://dca.gzhubu.top

list(zip(*m))
来源：http://qpi.aizwys.cn

[U23] Py：分块读取大文件
来源：http://vxx.hnxiangtu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kyh.zhiwuduotai.top

[U24] Py：路径操作
来源：http://nzs.yuxming.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hyd.hongshengwenyu.top

[U25] Py：CSV 按字典读
来源：http://jfw.zhaomingkeji.xyz

csv.DictReader(f)
来源：http://fpg.zhongyouzk.top

[U26] Py：并发下载
来源：http://rdg.sxryk.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://iks.sweek.top

[U27] Py：异步 HTTP
来源：http://pha.gogol.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://hmu.tian-w.cn

[U28] Py：类型别名
来源：http://krm.ydjk.org.cn

UserId = int
来源：http://sht.hongshengwenyu.top

[U29] Py：属性校验
来源：http://mdg.xziqi.cn

@property 与 @x.setter 配合
来源：http://zxc.zdbjq.cn

[U30] Py：数据类
来源：http://wti.hnxiangtu.top

@dataclass(slots=True)
来源：http://vpc.bbcook.cn

[U31] Py：单测
来源：http://thn.yj20258.top

python -m pytest -q
来源：http://wxy.yueranfly.top

[U32] Py：代码格式化
来源：http://apu.quarkkingdee.top

ruff format . && ruff check --fix .
来源：http://qxu.epnwcf.com

[U33] Py：打包发布
来源：http://gxh.xylfe.cn

python -m build  （依赖 pyproject.toml）
来源：http://mgj.havefunace.top

[U34] Py：判断编码
来源：http://mmt.shangyingyoupin.top

chardet.detect(raw)
来源：http://mzr.jinyuanbaomall.cn

[U35] Py：发送邮件
来源：http://iay.guowangkeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nfj.chenlongwang.top

[U36] Py：定时任务
来源：http://ame.snrcjt.cn

schedule.every(10).minutes.do(job)
来源：http://vfc.jqgufenzy.top

[U37] Py：读写 Excel
来源：http://pcj.cqqwz.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tsz.jiagoushi.top

[U38] Py：获取脚本所在目录
来源：http://xtg.bjfxy.top

Path(__file__).resolve().parent
来源：http://nuh.zhijiandao.cn

[U39] Py：判断是否在交互环境
来源：http://xho.jiagoushi.top

sys.stdout.isatty()
来源：http://ntx.yvedp.cn

[U40] Py：打印到标准错误
来源：http://hxe.hywenlv.cn

print("err", file=sys.stderr)
来源：http://aqo.hcnkem.com

[U41] PHP：初始化 Composer 项目
来源：http://tcl.yangfankeji.com

composer init;  composer require guzzlehttp/guzzle
来源：http://gmj.bbcook.cn

[U42] PHP：PSR-4 自动加载
来源：http://xbo.svipenyu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://upe.haohaochexian.top

[U43] PHP：声明命名空间
来源：http://cyr.havefunace.top

namespace App\Http;
来源：http://lnl.tianlin.xyz

[U44] PHP：开启严格类型
来源：http://cdv.gogol.net.cn

declare(strict_types=1);
来源：http://sna.iojbl.cn

[U45] PHP：类型声明与返回类型
来源：http://upl.svipenyu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://bar.zhaomingkeji.xyz

[U46] PHP：可空类型
来源：http://edf.guannengcc.top

?string $name = null
来源：http://jcr.hongshengwenyu.top

[U47] PHP：联合类型
来源：http://wvn.xingfuxueyuan.xyz

int|string $id
来源：http://vku.svipenyu.cn

[U48] PHP：纯枚举
来源：http://isc.ywan-chungtsiang.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://upp.andypj.xyz

[U49] PHP：只读属性
来源：http://xzv.yangfankeji.com

public readonly string $name
来源：http://foh.hfpthk.cn

[U50] PHP：构造器属性提升
来源：http://yzk.xylfe.cn

public function __construct(private int $id) {}
来源：http://mty.guowangkeji.top

[U51] PHP：数组解构
来源：http://omn.ivvv.top

[$a, $b] = $arr;
来源：http://tst.yj202588.top

[U52] PHP：箭头函数
来源：http://osa.daria6918.cn

$double = fn($x) => $x * 2;
来源：http://odi.pengpengdd.cyou

[U53] PHP：空合并运算符
来源：http://cxm.hcnkem.com

$v = $a ?? $b ?? "default";
来源：http://nnb.yj202588.top

[U54] PHP：空安全调用
来源：http://jou.xinyue.icu

$obj?->method()
来源：http://yfe.gaohongyu789.top

[U55] PHP：match 表达式
来源：http://gyc.tian-w.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://eyr.cucudq.cn

[U56] PHP：命名参数
来源：http://qkt.yvedp.cn

f(a: 1, b: 2)
来源：http://gfi.quarkkingdee.top

[U57] PHP：字符串插值
来源：http://mmf.fanxiaobao.xyz

"值: {$a}"
来源：http://pxw.sysykeji.top

[U58] PHP：数组三件套
来源：http://ckp.jiagoushi.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hjy.birdmap.top

[U59] PHP：自定义排序
来源：http://ubh.epnwcf.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jtu.hnqzz.top

[U60] PHP：JSON 编解码
来源：http://lye.jiagoushi.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gty.nwbrower.top

[U61] PHP：正则
来源：http://zoj.yanxiufei.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yih.xziqi.cn

[U62] PHP：日期对象
来源：http://itt.yj20258.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cvq.shzxlz.cn

[U63] PHP：文件读写
来源：http://hyy.haohaochexian.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vcb.tarul.cn

[U64] PHP：目录遍历
来源：http://roj.zhiwuduotai.top

glob("dir/*.php");  scandir("dir");
来源：http://ucd.pycfn.com

[U65] PHP：会话
来源：http://kme.yj20258888.top

session_start();  $_SESSION["uid"] = 1;
来源：http://wvy.hysaishi.cn

[U66] PHP：设置 Cookie
来源：http://shr.jinyuanbaomall.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ytj.sxryk.cn

[U67] PHP：处理文件上传
来源：http://vzj.snrcjt.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://gnt.bbcook.cn

[U68] PHP：PDO 连接
来源：http://aga.daxiang520.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jbe.jianghu66.top

[U69] PHP：PDO 预处理
来源：http://ott.9152youxi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://slo.xziqi.cn

[U70] PHP：PDO 事务
来源：http://nzx.pycfn.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fbm.vqdsnc.cn

[U71] PHP：抛出异常
来源：http://xde.xziqi.cn

throw new RuntimeException("失败", 500);
来源：http://epb.havefunace.top

[U72] PHP：写错误日志
来源：http://mqr.yuxming.cn

error_log("失败: " . $e->getMessage());
来源：http://hji.yj20258888.top

[U73] PHP：读取 ini 配置
来源：http://ycq.yj20258888.top

parse_ini_file("config.ini", true)
来源：http://ule.guannengcc.top

[U74] PHP：读取环境变量
来源：http://jgi.xinyue.icu

getenv("APP_ENV") ?: "production"
来源：http://uub.birdmap.top

[U75] PHP：依赖注入
来源：http://muf.daria6918.cn

composer require psr/container
来源：http://swg.shanyushiyangtech.top

[U76] PHP：简单路由
来源：http://qdp.hnqzz.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pne.yvedp.cn

[U77] PHP：模板渲染
来源：http://qdr.dianchejie.cn

composer require twig/twig
来源：http://bep.iojbl.cn

[U78] PHP：单元测试
来源：http://juv.chenzaomai.com

composer require --dev phpunit/phpunit
来源：http://fwd.havefunace.top

[U79] PHP：静态分析
来源：http://usd.guowangkeji.top

composer require --dev phpstan/phpstan
来源：http://iiw.gaohongyu789.top

[U80] PHP：代码规范修复
来源：http://jha.chenjidiqi.icu

composer require --dev friendsofphp/php-cs-fixer
来源：http://llj.iojbl.cn

[U81] JS：初始化项目
来源：http://xor.jyoumei.cn

npm init -y;  npm i express
来源：http://kss.sjlbkw.cn

[U82] JS：package.json 脚本
来源：http://wau.ehwqpu.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yie.jinqigfzy.top

[U83] JS：ES Module 导入导出
来源：http://afh.jlsjyb.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nar.jiagoushi.top

[U84] JS：CommonJS 写法
来源：http://vfx.iojbl.cn

module.exports = { a };  const { a } = require("./m");
来源：http://byo.bbcook.cn

[U85] JS：可选链
来源：http://acn.pengpengdd.cyou

a?.b?.c
来源：http://wlo.jlsjyb.cn

[U86] JS：空值合并
来源：http://iwe.jiagoushi.top

a ?? b
来源：http://sez.redwolf501.top

[U87] JS：解构默认值
来源：http://cur.xinyue.icu

const { a = 1, b = 2 } = obj;
来源：http://isp.tarul.cn

[U88] JS：对象展开合并
来源：http://qsx.vehdjk.com

{ ...a, ...b }
来源：http://nxz.andypj.xyz

[U89] JS：数组去重
来源：http://kox.hammf.cn

[...new Set(arr)]
来源：http://ovb.ydzc1.top

[U90] JS：数字数组排序
来源：http://cwe.quarkkingdee.top

[...arr].sort((a, b) => a - b)
来源：http://fef.nanxuanxn.top

[U91] JS：对象键值遍历
来源：http://guo.ehwqpu.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bbx.tianlin.xyz

[U92] JS：深拷贝
来源：http://hnx.yfazqb.com

structuredClone(obj)
来源：http://vdi.zhoulong.xyz

[U93] JS：模板字符串
来源：http://ipt.fzhhl.top

`共 ${n} 条`
来源：http://cwo.shanyushiyangtech.top

[U94] JS：箭头函数
来源：http://sxx.zhongyouzk.top

const double = x => x * 2;
来源：http://qve.gaohongyu789.top

[U95] JS：Promise 包装
来源：http://fyq.gotoacloud.top

new Promise((resolve, reject) => {})
来源：http://abo.bjfxy.top

[U96] JS：async/await 与异常
来源：http://fiw.chenzaomai.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qzy.c1oappe.top

[U97] JS：并发请求
来源：http://gwx.bjfxy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://kdg.yonumen.top

[U98] JS：fetch 带 JSON
来源：http://yrh.cashguo.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kcr.9152youxi.cn

[U99] JS：事件监听
来源：http://pdi.cqqwz.cn

el.addEventListener("click", e => {})
来源：http://odu.chenzaomai.com

[U100] JS：DOM 查询
来源：http://ucs.nwbrower.top

document.querySelector(".item")
来源：http://aqq.pengpengdd.cyou

[U101] JS：classList 操作
来源：http://buy.gzhubu.top

el.classList.toggle("active")
来源：http://qmv.sufxvd.cn

[U102] JS：本地存储
来源：http://lze.feifeiyinyue.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://czy.fehbvm.com

[U103] JS：定时器
来源：http://ehs.jiagoushi.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dwe.jianghu66.top

[U104] JS：防抖
来源：http://axt.xingfuxueyuan.xyz

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uxi.yfazqb.com

[U105] JS：节流
来源：http://mkn.jinyuanbaomall.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://keb.redwolf501.top

[U106] JS：日期格式化
来源：http://bfn.jinghuilouyu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rpz.ctjpmb.com

[U107] JS：数字千分位
来源：http://vhi.jinqigufen.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://urs.vqdsnc.cn

[U108] JS：随机整数
来源：http://eev.hcnkem.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lcl.xinyue.icu

[U109] JS：数组分组
来源：http://qds.xuanzx.com

Object.groupBy(arr, x => x.type)
来源：http://mjk.ehwqpu.com

[U110] JS：数组分块
来源：http://mio.zhixingplan.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dpy.jianghu66.top

[U111] JS：对象转 Map
来源：http://oyj.sweek.top

new Map(Object.entries(obj))
来源：http://vzy.zycfv.cn

[U112] JS：字符串补位
来源：http://ckx.tian-w.cn

"7".padStart(3, "0")
来源：http://ics.pycfn.com

[U113] JS：正则替换全部
来源：http://kqn.jinghuilouyu.cn

s.replaceAll("a", "b")
来源：http://acq.c1oappe.top

[U114] JS：JSON 深比较
来源：http://bbm.ppjwa.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dvl.daxiang520.top

[U115] JS：生成 UUID
来源：http://dun.cqqwz.cn

crypto.randomUUID()
来源：http://ypf.ydjk.org.cn

[U116] JS：类型检查（JSDoc）
来源：http://ozn.nanxinkj.top

/** @param {string} name */ function f(name) {}
来源：http://mxl.daria6918.cn

[U117] JS：单元测试
来源：http://tpu.hywenlv.cn

npm i -D vitest;  npx vitest
来源：http://rhh.vehdjk.com

[U118] JS：开发服务器
来源：http://cur.hcnkem.com

npm i -D vite;  npx vite
来源：http://ria.aibaodan.cn

[U119] JS：生产构建
来源：http://kwo.yfazqb.com

npx vite build
来源：http://btz.chenzaomai.com

[U120] JS：读取环境变量（Vite）
来源：http://prv.fengsongda.top

import.meta.env.VITE_API_URL
来源：http://eje.zhoulong.xyz

================================================================================
来源：http://yvv.havefunace.top

统计汇总
来源：http://nyl.hnqzz.top

================================================================================
来源：http://qkq.haohaochexian.top

按语言统计（条）：
来源：http://eio.dianchejie.cn

Python ......... 252
来源：http://pbw.shanyushiyangtech.top

PHP ............ 252
来源：http://rwo.chenzaomai.com

JavaScript ..... 252
来源：http://osi.zhiwuduotai.top

TypeScript ..... 212
来源：http://kaj.jyoumei.cn

Java ........... 212
来源：http://lae.epnwcf.com

Go ............. 212
来源：http://nxc.guannengcc.top

Ruby ........... 212
来源：http://hdq.sjlbkw.cn

C# ............. 212
来源：http://dcc.zdqjudy.top

C .............. 30
来源：http://frc.ppjwa.cn

C++ ............ 30
来源：http://ajj.birdmap.top

SQL ............ 90
来源：http://ixq.yfazqb.com

Bash ........... 80
来源：http://lvy.nanxinkj.top

Kotlin ......... 15
来源：http://nof.chenjidiqi.icu

Swift .......... 15
来源：http://bqu.0kj1m.cn

Lua ............ 10
来源：http://qqf.hfpthk.cn

Perl ........... 10
来源：http://jwl.chenzaomai.com

Scala .......... 10
来源：http://dbk.hesvh.cn

------------------------------------
来源：http://qso.wangshuangyany.cn

合计 ........... 2106 条
来源：http://ykj.jianghu66.top

按章节统计：
来源：http://arf.birdmap.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://swq.snrcjt.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zib.cdnleiting.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ssy.jianghu66.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dmz.cheryme.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wde.9152youxi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dmd.snrcjt.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cci.shangyingyoupin.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xvv.xuetiantiany.cn


<!-- 参考信息 -->