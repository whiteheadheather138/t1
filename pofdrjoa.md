代发 wailian999

[T37] Lua：字符串拼接
来源：http://kqh.snrcjt.cn

"a" .. "b"
来源：http://gop.jinghuilouyu.cn

[T38] Lua：条件
来源：http://blc.tianlin.xyz

if x > 0 then print("正") end
来源：http://jpf.zhengqikj.top

[T39] Lua：模式匹配
来源：http://fgd.zhaomingkeji.xyz

string.find(s, "%d+")
来源：http://mxa.gzhubu.top

[T40] Lua：元表
来源：http://zch.316326.xyz

setmetatable({}, { __index = base })
来源：http://eba.vqdsnc.cn

[T41] Perl：Hello World
来源：http://vne.tian-w.cn

print "Hello\n";
来源：http://tqi.bbcook.cn

[T42] Perl：变量类型
来源：http://qht.cqqwz.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qsb.fzhhl.top

[T43] Perl：字符串插值
来源：http://cvs.ywan-chungtsiang.top

"值: $a"
来源：http://lvv.jinyuanbaomall.cn

[T44] Perl：条件
来源：http://kkn.aibaodan.cn

if ($a > 0) { print "正"; }
来源：http://kxd.aizwys.cn

[T45] Perl：数组遍历
来源：http://jev.sufxvd.cn

for my $x (@arr) { print $x; }
来源：http://dua.yj202588.top

[T46] Perl：哈希操作
来源：http://hhu.ctjpmb.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://boy.vehdjk.com

[T47] Perl：正则捕获
来源：http://ncd.zhoulong.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://sqz.sweek.top

[T48] Perl：正则替换
来源：http://vet.xylfe.cn

$s =~ s/old/new/g;
来源：http://hjh.gogol.net.cn

[T49] Perl：函数
来源：http://egr.sjlbkw.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yom.jiagoushi.top

[T50] Perl：逐行读文件
来源：http://lkd.gzhubu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://kvh.yj202588.top

while (my $line = <$fh>) { print $line; }
来源：http://jkv.tarul.cn

[T51] Scala：Hello World
来源：http://csm.shuidangran.top

println("Hello")
来源：http://obt.yj202588.top

[T52] Scala：变量
来源：http://tbu.pycfn.com

val a = 1;  var b = 2
来源：http://icj.quarkkingdee.top

[T53] Scala：字符串插值
来源：http://kle.gogol.net.cn

s"值: $b"
来源：http://uxx.9152youxi.cn

[T54] Scala：集合映射
来源：http://ewj.hnxiangtu.top

List(1, 2, 3).map(_ * 2)
来源：http://trp.hysaishi.cn

[T55] Scala：集合过滤
来源：http://pyr.snrcjt.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lyr.jqgfzy.top

[T56] Scala：样例类
来源：http://xyl.shuidangran.top

case class User(name: String, age: Int)
来源：http://yuk.daria6918.cn

[T57] Scala：模式匹配
来源：http://mqf.gogol.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hpn.nwbrower.top

[T58] Scala：函数定义
来源：http://tih.gaohongyu789.top

def add(a: Int, b: Int): Int = a + b
来源：http://upc.bjfxy.top

[T59] Scala：循环
来源：http://zyd.daxiang520.top

for (i <- 1 to 10) println(i)
来源：http://gae.tianlin.xyz

[T60] Scala：折叠
来源：http://hte.wangshuangyany.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cbr.yangfankeji.com

================================================================================
来源：http://zhs.cashguo.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fvd.jinqigfzy.top

================================================================================
来源：http://ffl.yonumen.top

[U01] Py：创建虚拟环境
来源：http://iup.cucudq.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vre.haohaochexian.top

[U02] Py：导出 / 安装依赖
来源：http://leg.iojbl.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pcn.bjfxy.top

[U03] Py：加载 .env 配置
来源：http://ixx.jinyuanbaomall.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://llw.0kj1m.cn

[U04] Py：变量调试打印
来源：http://mum.316326.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yuq.ppjwa.cn

[U05] Py：列表去重且保序
来源：http://yzb.kuanghao11.cn

list(dict.fromkeys(arr))
来源：http://opt.chenjidiqi.icu

[U06] Py：合并两个字典
来源：http://eiz.zdbjq.cn

{**a, **b}
来源：http://baj.shzxlz.cn

[U07] Py：反转字典键值
来源：http://kba.jinqigufen.top

{v: k for k, v in d.items()}
来源：http://nbj.hysaishi.cn

[U08] Py：展平二维列表
来源：http://sib.bbcook.cn

[y for x in nested for y in x]
来源：http://mst.redwolf501.top

[U09] Py：字典取最大值的键
来源：http://qcb.mhx1999.top

max(d, key=d.get)
来源：http://jbn.epnwcf.com

[U10] Py：按值排序字典
来源：http://lzp.ybcxt.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ske.yj20258.top

[U11] Py：生成器表达式
来源：http://hxq.xuetiantiany.cn

(x * 2 for x in arr)
来源：http://oyr.epnwcf.com

[U12] Py：取出现最多的 3 个元素
来源：http://kav.zdbjq.cn

Counter(arr).most_common(3)
来源：http://hhz.andypj.xyz

[U13] Py：固定长度队列
来源：http://srb.hammf.cn

deque(maxlen=10)
来源：http://vty.chenjidiqi.icu

[U14] Py：分组收集到列表
来源：http://cev.cqqwz.cn

defaultdict(list)
来源：http://cdh.zhaomingkeji.xyz

[U15] Py：高精度计时
来源：http://hln.ydzc1.top

t = time.perf_counter()
来源：http://zoj.cdnleiting.top

[U16] Py：命令行参数解析
来源：http://lrz.snrcjt.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sya.yj20258.top

[U17] Py：初始化日志
来源：http://zlo.guowangkeji.top

logging.basicConfig(level=logging.INFO)
来源：http://dsr.guannengcc.top

[U18] Py：预编译正则
来源：http://lxt.redwolf501.top

pat = re.compile(r"\d+")
来源：http://vdq.feifeiyinyue.top

[U19] Py：正则替换带回调
来源：http://erg.shanyushiyangtech.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lym.hcnkem.com

[U20] Py：缓存函数结果
来源：http://afn.yanxiufei.cn

@functools.lru_cache(maxsize=None)
来源：http://gnz.jyoumei.cn

[U21] Py：自定义上下文管理器
来源：http://mxp.kuanghao11.cn

@contextlib.contextmanager
来源：http://jti.sweek.top

[U22] Py：矩阵转置
来源：http://xyr.cucudq.cn

list(zip(*m))
来源：http://vjy.yvedp.cn

[U23] Py：分块读取大文件
来源：http://clj.jqgfzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fte.chenzaomai.com

[U24] Py：路径操作
来源：http://lqi.yonumen.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://iqv.ydzc1.top

[U25] Py：CSV 按字典读
来源：http://jwa.daxiang520.top

csv.DictReader(f)
来源：http://ywr.zhoulong.xyz

[U26] Py：并发下载
来源：http://qcj.zhaomingkeji.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vae.andypj.xyz

[U27] Py：异步 HTTP
来源：http://bec.jyoumei.cn

aiohttp.ClientSession() 配合 async with
来源：http://vha.quarkkingdee.top

[U28] Py：类型别名
来源：http://wne.jqgfzy.top

UserId = int
来源：http://npa.svipenyu.cn

[U29] Py：属性校验
来源：http://hhq.redwolf501.top

@property 与 @x.setter 配合
来源：http://mjs.yj20258888.top

[U30] Py：数据类
来源：http://uea.jinyuanbaomall.cn

@dataclass(slots=True)
来源：http://tca.yj20258.top

[U31] Py：单测
来源：http://cox.kuanghao11.cn

python -m pytest -q
来源：http://qpe.fktsv.cn

[U32] Py：代码格式化
来源：http://uzy.haohaochexian.top

ruff format . && ruff check --fix .
来源：http://ulk.yonumen.top

[U33] Py：打包发布
来源：http://rhw.chenjidiqi.icu

python -m build  （依赖 pyproject.toml）
来源：http://gnt.cheryme.top

[U34] Py：判断编码
来源：http://ivf.jinqigufen.top

chardet.detect(raw)
来源：http://cez.vqdsnc.cn

[U35] Py：发送邮件
来源：http://agp.guowangkeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bxl.yfazqb.com

[U36] Py：定时任务
来源：http://ujs.yuxming.cn

schedule.every(10).minutes.do(job)
来源：http://xrp.shanyushiyangkeji.top

[U37] Py：读写 Excel
来源：http://mbf.sxryk.cn

pandas.read_excel / DataFrame.to_excel
来源：http://nlh.sjlbkw.cn

[U38] Py：获取脚本所在目录
来源：http://liv.yj202588.top

Path(__file__).resolve().parent
来源：http://aih.mhx1999.top

[U39] Py：判断是否在交互环境
来源：http://eyk.chenzaomai.com

sys.stdout.isatty()
来源：http://sfd.nanxuanxn.top

[U40] Py：打印到标准错误
来源：http://oel.daria6918.cn

print("err", file=sys.stderr)
来源：http://cti.hfpthk.cn

[U41] PHP：初始化 Composer 项目
来源：http://nnd.316326.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://gsc.cashguo.top

[U42] PHP：PSR-4 自动加载
来源：http://nqw.gzhubu.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://iue.chenjidiqi.icu

[U43] PHP：声明命名空间
来源：http://kuc.52xcode.cn

namespace App\Http;
来源：http://das.chenzaomai.com

[U44] PHP：开启严格类型
来源：http://bqo.zycfv.cn

declare(strict_types=1);
来源：http://ftm.cqqwz.cn

[U45] PHP：类型声明与返回类型
来源：http://nnz.ivvv.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://qfg.jqgufenzy.top

[U46] PHP：可空类型
来源：http://qac.ywan-chungtsiang.top

?string $name = null
来源：http://yoc.zhengqikj.top

[U47] PHP：联合类型
来源：http://tnq.daria6918.cn

int|string $id
来源：http://wuc.zhoulong.xyz

[U48] PHP：纯枚举
来源：http://tav.tian-w.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vab.havefunace.top

[U49] PHP：只读属性
来源：http://etc.haohaochexian.top

public readonly string $name
来源：http://nmo.hfpthk.cn

[U50] PHP：构造器属性提升
来源：http://boy.fanxiaobao.xyz

public function __construct(private int $id) {}
来源：http://ktn.shuidangran.top

[U51] PHP：数组解构
来源：http://duf.dashuyun.cn

[$a, $b] = $arr;
来源：http://yhv.9152youxi.cn

[U52] PHP：箭头函数
来源：http://bno.yj202588.top

$double = fn($x) => $x * 2;
来源：http://glf.c1oappe.top

[U53] PHP：空合并运算符
来源：http://wxw.tianlin.xyz

$v = $a ?? $b ?? "default";
来源：http://avb.hongshengwenyu.top

[U54] PHP：空安全调用
来源：http://pra.yvedp.cn

$obj?->method()
来源：http://qvk.gaohongyu789.top

[U55] PHP：match 表达式
来源：http://tte.zdbjq.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://eaj.gogol.net.cn

[U56] PHP：命名参数
来源：http://yqc.snrcjt.cn

f(a: 1, b: 2)
来源：http://pra.jyoumei.cn

[U57] PHP：字符串插值
来源：http://ewi.yj202588.top

"值: {$a}"
来源：http://xqz.hammf.cn

[U58] PHP：数组三件套
来源：http://vfs.yj20258.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gin.epnwcf.com

[U59] PHP：自定义排序
来源：http://zyf.snrcjt.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jol.nwbrower.top

[U60] PHP：JSON 编解码
来源：http://vwj.zhixingplan.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ail.cdnleiting.top

[U61] PHP：正则
来源：http://utm.zhoulong.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kvz.ivvv.top

[U62] PHP：日期对象
来源：http://gnu.xuetiantiany.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xig.gotoacloud.top

[U63] PHP：文件读写
来源：http://urr.snrcjt.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fwk.hesvh.cn

[U64] PHP：目录遍历
来源：http://ldt.chenzaomai.com

glob("dir/*.php");  scandir("dir");
来源：http://zhk.shanyushiyangtech.top

[U65] PHP：会话
来源：http://pke.fktsv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ehg.tian-w.cn

[U66] PHP：设置 Cookie
来源：http://frg.tanke756.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://owh.jyoumei.cn

[U67] PHP：处理文件上传
来源：http://csk.aibaodan.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fhd.zhiwuduotai.top

[U68] PHP：PDO 连接
来源：http://iha.fktsv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bej.snrcjt.cn

[U69] PHP：PDO 预处理
来源：http://rjf.chenjidiqi.icu

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://agu.nwbrower.top

[U70] PHP：PDO 事务
来源：http://slb.smart0.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://phe.sxryk.cn

[U71] PHP：抛出异常
来源：http://jdd.gaohongyu789.top

throw new RuntimeException("失败", 500);
来源：http://rum.zhijiandao.cn

[U72] PHP：写错误日志
来源：http://qjf.sjlbkw.cn

error_log("失败: " . $e->getMessage());
来源：http://rby.tian-w.cn

[U73] PHP：读取 ini 配置
来源：http://woo.cqqwz.cn

parse_ini_file("config.ini", true)
来源：http://bdo.fanxiaobao.xyz

[U74] PHP：读取环境变量
来源：http://fdw.nanxuanxn.top

getenv("APP_ENV") ?: "production"
来源：http://rgw.meibo888.top

[U75] PHP：依赖注入
来源：http://xrf.sufxvd.cn

composer require psr/container
来源：http://esd.daria6918.cn

[U76] PHP：简单路由
来源：http://rek.c1oappe.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sig.xziqi.cn

[U77] PHP：模板渲染
来源：http://pps.pycfn.com

composer require twig/twig
来源：http://flf.ydzc1.top

[U78] PHP：单元测试
来源：http://doe.hesvh.cn

composer require --dev phpunit/phpunit
来源：http://bvp.fehbvm.com

[U79] PHP：静态分析
来源：http://sdt.xingfuxueyuan.xyz

composer require --dev phpstan/phpstan
来源：http://xdk.aibaodan.cn

[U80] PHP：代码规范修复
来源：http://yar.jqgufenzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://equ.bbcook.cn

[U81] JS：初始化项目
来源：http://wgg.ivvv.top

npm init -y;  npm i express
来源：http://khs.hnxiangtu.top

[U82] JS：package.json 脚本
来源：http://svi.birdmap.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mwm.fehbvm.com

[U83] JS：ES Module 导入导出
来源：http://tcz.xylfe.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jim.sjlbkw.cn

[U84] JS：CommonJS 写法
来源：http://vca.yj202588.top

module.exports = { a };  const { a } = require("./m");
来源：http://wue.hnxiangtu.top

[U85] JS：可选链
来源：http://oir.jinqigfzy.top

a?.b?.c
来源：http://eaz.shuidangran.top

[U86] JS：空值合并
来源：http://mok.haohaochexian.top

a ?? b
来源：http://qrq.uphjek.com

[U87] JS：解构默认值
来源：http://ldv.sysykeji.top

const { a = 1, b = 2 } = obj;
来源：http://nlb.bjfxy.top

[U88] JS：对象展开合并
来源：http://kpp.sjlbkw.cn

{ ...a, ...b }
来源：http://pbk.chenzaomai.com

[U89] JS：数组去重
来源：http://rww.yuanzhike.top

[...new Set(arr)]
来源：http://yhq.zhiwuduotai.top

[U90] JS：数字数组排序
来源：http://xzy.cdnleiting.top

[...arr].sort((a, b) => a - b)
来源：http://vfe.gzhubu.top

[U91] JS：对象键值遍历
来源：http://xiy.epnwcf.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ksu.cdnleiting.top

[U92] JS：深拷贝
来源：http://kjl.zhijiandao.cn

structuredClone(obj)
来源：http://idj.andypj.xyz

[U93] JS：模板字符串
来源：http://qte.zhijiandao.cn

`共 ${n} 条`
来源：http://qjs.c1oappe.top

[U94] JS：箭头函数
来源：http://qqw.shanyushiyangkeji.top

const double = x => x * 2;
来源：http://bas.ywan-chungtsiang.top

[U95] JS：Promise 包装
来源：http://eik.nanxinkj.top

new Promise((resolve, reject) => {})
来源：http://rag.uphjek.com

[U96] JS：async/await 与异常
来源：http://qsu.cqqwz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cbq.ivvv.top

[U97] JS：并发请求
来源：http://mbi.sysykeji.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://vtz.yj20258.top

[U98] JS：fetch 带 JSON
来源：http://hkf.yanxiufei.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tdt.gogol.net.cn

[U99] JS：事件监听
来源：http://pnn.xylfe.cn

el.addEventListener("click", e => {})
来源：http://tso.hywenlv.cn

[U100] JS：DOM 查询
来源：http://ryz.jianghu66.top

document.querySelector(".item")
来源：http://gmr.nanxuanxn.top

[U101] JS：classList 操作
来源：http://bqd.hongshengwenyu.top

el.classList.toggle("active")
来源：http://aaa.redwolf501.top

[U102] JS：本地存储
来源：http://dki.vqdsnc.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ooa.xuetiantiany.cn

[U103] JS：定时器
来源：http://pgj.zdbjq.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wpz.gogol.net.cn

[U104] JS：防抖
来源：http://ixg.chenzaomai.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fei.sjlbkw.cn

[U105] JS：节流
来源：http://pli.tian-w.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sjr.zhoulong.xyz

[U106] JS：日期格式化
来源：http://zxn.fengsongda.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://kwh.xinyue.icu

[U107] JS：数字千分位
来源：http://abv.ehwqpu.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bsg.chenzaomai.com

[U108] JS：随机整数
来源：http://iji.tianlin.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://eyb.snrcjt.cn

[U109] JS：数组分组
来源：http://bxh.c1oappe.top

Object.groupBy(arr, x => x.type)
来源：http://bxa.quarkkingdee.top

[U110] JS：数组分块
来源：http://jua.ehwqpu.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blu.tianlin.xyz

[U111] JS：对象转 Map
来源：http://yjr.feifeiyinyue.top

new Map(Object.entries(obj))
来源：http://kns.jlsjyb.cn

[U112] JS：字符串补位
来源：http://bvt.yvedp.cn

"7".padStart(3, "0")
来源：http://sko.sweek.top

[U113] JS：正则替换全部
来源：http://lym.jinqigfzy.top

s.replaceAll("a", "b")
来源：http://pfc.pycfn.com

[U114] JS：JSON 深比较
来源：http://wwh.kuanghao11.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://oyj.yangfankeji.com

[U115] JS：生成 UUID
来源：http://kzq.jlsjyb.cn

crypto.randomUUID()
来源：http://jjn.tianlin.xyz

[U116] JS：类型检查（JSDoc）
来源：http://lgq.52xcode.cn

/** @param {string} name */ function f(name) {}
来源：http://enn.zhixingplan.top

[U117] JS：单元测试
来源：http://ihx.snrcjt.cn

npm i -D vitest;  npx vitest
来源：http://gmb.ehwqpu.com

[U118] JS：开发服务器
来源：http://djx.wangdashe.top

npm i -D vite;  npx vite
来源：http://jys.birdmap.top

[U119] JS：生产构建
来源：http://gem.pycfn.com

npx vite build
来源：http://feg.tarul.cn

[U120] JS：读取环境变量（Vite）
来源：http://rcu.bjfxy.top

import.meta.env.VITE_API_URL
来源：http://scp.meibo888.top

================================================================================
来源：http://fui.bbcook.cn

统计汇总
来源：http://zzi.vehdjk.com

================================================================================
来源：http://tfp.zhengqikj.top

按语言统计（条）：
来源：http://btb.xinyue.icu

Python ......... 252
来源：http://zoh.wangshuangyany.cn

PHP ............ 252
来源：http://kjx.quarkkingdee.top

JavaScript ..... 252
来源：http://suu.birdmap.top

TypeScript ..... 212
来源：http://mxo.svipenyu.cn


<!-- 参考信息 -->