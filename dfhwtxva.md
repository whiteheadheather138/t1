代发 wailian999

int size() const noexcept { return n_; }
来源：http://hfv.shzxlz.cn

[S53] C++：移动语义
来源：http://pws.cheryme.top

std::vector<int> w = std::move(v);
来源：http://zaq.0kj1m.cn

[S54] C++：异常处理
来源：http://blg.ybcxt.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cye.cheryme.top

[S55] C++：结构化绑定
来源：http://whp.zhiwuduotai.top

auto [a, b] = std::make_pair(1, 2);
来源：http://quw.dianchejie.cn

[S56] C++：optional
来源：http://ciz.zhijiandao.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://osi.redwolf501.top

[S57] C++：编译期常量
来源：http://iuk.xingfuxueyuan.xyz

constexpr int N = 10;
来源：http://dvf.pengpengdd.cyou

[S58] C++：命名空间
来源：http://wfk.hcnkem.com

namespace ns { int f() { return 1; } }
来源：http://pkn.gotoacloud.top

[S59] C++：静态断言
来源：http://ydo.tianlin.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jxq.dashuyun.cn

[S60] C++：遍历并删除元素
来源：http://dup.fengsongda.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cbm.hammf.cn

================================================================================
来源：http://kwl.mhx1999.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jlo.zhengqikj.top

================================================================================
来源：http://ihj.yj20258.top

[T01] Kotlin：Hello World
来源：http://pht.gaohongyu789.top

println("Hello")
来源：http://quu.chenjidiqi.icu

[T02] Kotlin：变量
来源：http://adj.birdmap.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://amh.aizwys.cn

[T03] Kotlin：字符串模板
来源：http://wqm.hnxiangtu.top

"值: $b"
来源：http://kon.xinyue.icu

[T04] Kotlin：空安全
来源：http://xmb.ybcxt.top

val n: String? = null;  n?.length
来源：http://lzs.cashguo.top

[T05] Kotlin：when 表达式
来源：http://rfe.jlsjyb.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://abj.hnxiangtu.top

[T06] Kotlin：集合映射
来源：http://abt.chenlongwang.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qwe.9152youxi.cn

[T07] Kotlin：集合过滤
来源：http://uld.daxiang520.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://tyx.zdbjq.cn

[T08] Kotlin：数据类
来源：http://nyw.ppjwa.cn

data class User(val name: String, val age: Int)
来源：http://jql.shuidangran.top

[T09] Kotlin：扩展函数
来源：http://ebf.cashguo.top

fun String.exclaim() = this + "!"
来源：http://cwb.redwolf501.top

[T10] Kotlin：默认参数
来源：http://qse.pengpengdd.cyou

fun greet(name: String = "World") = "Hi $name"
来源：http://fuf.yj20258888.top

[T11] Kotlin：协程
来源：http://pwi.jqgufenzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ygl.hysaishi.cn

[T12] Kotlin：解构声明
来源：http://uve.epnwcf.com

val (a, b) = Pair(1, 2)
来源：http://hkk.hywenlv.cn

[T13] Kotlin：只读 Map
来源：http://ptp.yongpay.top

val m = mapOf("a" to 1)
来源：http://iso.cqqwz.cn

[T14] Kotlin：循环
来源：http://nhl.xingfuxueyuan.xyz

for (i in 1..10) println(i)
来源：http://uky.tian-w.cn

[T15] Kotlin：接口
来源：http://wtx.ivvv.top

interface Shape { fun area(): Double }
来源：http://aro.wangshuangyany.cn

[T16] Swift：Hello World
来源：http://ejw.316326.xyz

print("Hello")
来源：http://kgb.jianghu66.top

[T17] Swift：变量与常量
来源：http://xqy.9152youxi.cn

var a = 1;  let b = 2
来源：http://yhp.shzxlz.cn

[T18] Swift：字符串插值
来源：http://ops.xuanzx.com

"值: \(b)"
来源：http://jrx.tianlin.xyz

[T19] Swift：可选绑定
来源：http://dox.chenzaomai.com

if let n = opt { print(n) }
来源：http://mrh.nwbrower.top

[T20] Swift：数组操作
来源：http://ize.yangfankeji.com

var a = [1, 2, 3];  a.append(4)
来源：http://xli.havefunace.top

[T21] Swift：遍历
来源：http://tnf.nanxuanxn.top

for x in a { print(x) }
来源：http://fbe.9152youxi.cn

[T22] Swift：字典
来源：http://baj.sufxvd.cn

var d = ["a": 1];  d["b"] = 2
来源：http://osu.jinyuanbaomall.cn

[T23] Swift：函数
来源：http://ksc.sysykeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cob.xziqi.cn

[T24] Swift：闭包
来源：http://xdt.uphjek.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://wra.hcnkem.com

[T25] Swift：结构体
来源：http://lhh.0kj1m.cn

struct P { var x: Int }
来源：http://mgb.yonumen.top

[T26] Swift：类与重写
来源：http://mdb.hcnkem.com

class A: Base { override func f() {} }
来源：http://ggq.fanxiaobao.xyz

[T27] Swift：错误处理
来源：http://jte.hywenlv.cn

do { try f() } catch { print(error) }
来源：http://owt.guowangkeji.top

[T28] Swift：枚举
来源：http://zok.fzhhl.top

enum Color { case red, green }
来源：http://qzf.wangdashe.top

[T29] Swift：guard 提前返回
来源：http://moj.ywan-chungtsiang.top

guard let x = opt else { return }
来源：http://sny.yj20258888.top

[T30] Swift：协议
来源：http://ail.pengpengdd.cyou

protocol Shape { func area() -> Double }
来源：http://too.yj202588.top

[T31] Lua：Hello World
来源：http://bgj.yuanzhike.top

print("Hello")
来源：http://fuw.yuanzhike.top

[T32] Lua：局部变量
来源：http://gyn.zhengqikj.top

local a = 1
来源：http://aze.wangdashe.top

[T33] Lua：表（数组）
来源：http://vpd.cheryme.top

local t = {1, 2, 3};  t[4] = 4
来源：http://lrz.andypj.xyz

[T34] Lua：遍历表
来源：http://mpt.havefunace.top

for i, v in ipairs(t) do print(i, v) end
来源：http://axx.yonumen.top

[T35] Lua：字典表
来源：http://qqp.gogol.net.cn

local d = { a = 1 };  d.b = 2
来源：http://rhk.kuanghao11.cn

[T36] Lua：函数
来源：http://uea.gogol.net.cn

function add(a, b) return a + b end
来源：http://vad.zdqjudy.top

[T37] Lua：字符串拼接
来源：http://dun.zycfv.cn

"a" .. "b"
来源：http://lgq.ybcxt.top

[T38] Lua：条件
来源：http://nmr.fktsv.cn

if x > 0 then print("正") end
来源：http://wyu.bjfxy.top

[T39] Lua：模式匹配
来源：http://jnb.ivvv.top

string.find(s, "%d+")
来源：http://eit.jinqigfzy.top

[T40] Lua：元表
来源：http://gsx.yonumen.top

setmetatable({}, { __index = base })
来源：http://afz.yanxiufei.cn

[T41] Perl：Hello World
来源：http://vta.hfpthk.cn

print "Hello\n";
来源：http://axj.cucudq.cn

[T42] Perl：变量类型
来源：http://ovi.zhixingplan.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mof.vehdjk.com

[T43] Perl：字符串插值
来源：http://bah.hammf.cn

"值: $a"
来源：http://gwt.yj202588.top

[T44] Perl：条件
来源：http://xpu.xziqi.cn

if ($a > 0) { print "正"; }
来源：http://mjq.0kj1m.cn

[T45] Perl：数组遍历
来源：http://dke.havefunace.top

for my $x (@arr) { print $x; }
来源：http://ewq.zhoulong.xyz

[T46] Perl：哈希操作
来源：http://baw.xuetiantiany.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ziy.9152youxi.cn

[T47] Perl：正则捕获
来源：http://wgo.bbcook.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ttj.hfpthk.cn

[T48] Perl：正则替换
来源：http://qjw.cashguo.top

$s =~ s/old/new/g;
来源：http://ivu.yonumen.top

[T49] Perl：函数
来源：http://hpe.gzhubu.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ygm.fengsongda.top

[T50] Perl：逐行读文件
来源：http://ruz.nwbrower.top

open my $fh, "<", "a.txt" or die $!;
来源：http://tyk.aibaodan.cn

while (my $line = <$fh>) { print $line; }
来源：http://zbg.gaohongyu789.top

[T51] Scala：Hello World
来源：http://omb.yangfankeji.com

println("Hello")
来源：http://xyu.hnxiangtu.top

[T52] Scala：变量
来源：http://jgo.yongpay.top

val a = 1;  var b = 2
来源：http://lcw.kuanghao11.cn

[T53] Scala：字符串插值
来源：http://naa.xuetiantiany.cn

s"值: $b"
来源：http://mul.yuxming.cn

[T54] Scala：集合映射
来源：http://nbr.mhx1999.top

List(1, 2, 3).map(_ * 2)
来源：http://vpu.hnqzz.top

[T55] Scala：集合过滤
来源：http://lep.hysaishi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mme.jianghu66.top

[T56] Scala：样例类
来源：http://hoo.ydzc1.top

case class User(name: String, age: Int)
来源：http://eoe.gotoacloud.top

[T57] Scala：模式匹配
来源：http://loc.nwbrower.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://pwu.shuidangran.top

[T58] Scala：函数定义
来源：http://wuq.ppjwa.cn

def add(a: Int, b: Int): Int = a + b
来源：http://shf.nanxuanxn.top

[T59] Scala：循环
来源：http://mti.yuanzhike.top

for (i <- 1 to 10) println(i)
来源：http://hom.smart0.xyz

[T60] Scala：折叠
来源：http://pkq.yj202588.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bfb.jinyuanbaomall.cn

================================================================================
来源：http://ivz.0kj1m.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://oib.52xcode.cn

================================================================================
来源：http://imp.guowangkeji.top

[U01] Py：创建虚拟环境
来源：http://niu.yonumen.top

python -m venv .venv && source .venv/bin/activate
来源：http://zgr.hfpthk.cn

[U02] Py：导出 / 安装依赖
来源：http://sld.ydjk.org.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fus.fengsongda.top

[U03] Py：加载 .env 配置
来源：http://gki.cqqwz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rbi.sjlbkw.cn

[U04] Py：变量调试打印
来源：http://ptr.xylfe.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://trm.pengpengdd.cyou

[U05] Py：列表去重且保序
来源：http://rbz.zhongyouzk.top

list(dict.fromkeys(arr))
来源：http://tdv.xziqi.cn

[U06] Py：合并两个字典
来源：http://hxi.sweek.top

{**a, **b}
来源：http://wtd.ydjk.org.cn

[U07] Py：反转字典键值
来源：http://bfi.guowangkeji.top

{v: k for k, v in d.items()}
来源：http://kmt.gotoacloud.top

[U08] Py：展平二维列表
来源：http://kao.vehdjk.com

[y for x in nested for y in x]
来源：http://bzw.xingfuxueyuan.xyz

[U09] Py：字典取最大值的键
来源：http://hfi.yonumen.top

max(d, key=d.get)
来源：http://anj.ehwqpu.com

[U10] Py：按值排序字典
来源：http://twg.gzhubu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hii.wangdashe.top

[U11] Py：生成器表达式
来源：http://yms.ctjpmb.com

(x * 2 for x in arr)
来源：http://ogi.tian-w.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yqi.hnqzz.top

Counter(arr).most_common(3)
来源：http://gex.zycfv.cn

[U13] Py：固定长度队列
来源：http://yot.shzxlz.cn

deque(maxlen=10)
来源：http://goq.fzhhl.top

[U14] Py：分组收集到列表
来源：http://gbl.sysykeji.top

defaultdict(list)
来源：http://yfl.gzhubu.top

[U15] Py：高精度计时
来源：http://izn.fehbvm.com

t = time.perf_counter()
来源：http://kul.ivvv.top

[U16] Py：命令行参数解析
来源：http://nqs.gotoacloud.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cif.ydzc1.top

[U17] Py：初始化日志
来源：http://xuu.xuanzx.com

logging.basicConfig(level=logging.INFO)
来源：http://jki.zdqjudy.top

[U18] Py：预编译正则
来源：http://wls.chenjidiqi.icu

pat = re.compile(r"\d+")
来源：http://vjc.zdbjq.cn

[U19] Py：正则替换带回调
来源：http://kfz.ydzc1.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ogw.jinqigufen.top

[U20] Py：缓存函数结果
来源：http://nzc.yueranfly.top

@functools.lru_cache(maxsize=None)
来源：http://rjs.vehdjk.com

[U21] Py：自定义上下文管理器
来源：http://mtc.yanxiufei.cn

@contextlib.contextmanager
来源：http://yew.ywan-chungtsiang.top

[U22] Py：矩阵转置
来源：http://ise.yvedp.cn

list(zip(*m))
来源：http://vum.cqqwz.cn

[U23] Py：分块读取大文件
来源：http://vni.bjfxy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://eau.guannengcc.top

[U24] Py：路径操作
来源：http://udz.sweek.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qag.zhoulong.xyz

[U25] Py：CSV 按字典读
来源：http://xvv.yonumen.top

csv.DictReader(f)
来源：http://bhk.yuxming.cn

[U26] Py：并发下载
来源：http://pko.jqgufenzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://env.uphjek.com

[U27] Py：异步 HTTP
来源：http://xvv.vqdsnc.cn

aiohttp.ClientSession() 配合 async with
来源：http://vrg.gzhubu.top

[U28] Py：类型别名
来源：http://owr.hywenlv.cn

UserId = int
来源：http://aac.hcnkem.com

[U29] Py：属性校验
来源：http://cky.haohaochexian.top

@property 与 @x.setter 配合
来源：http://dky.sxryk.cn

[U30] Py：数据类
来源：http://anv.zhixingplan.top

@dataclass(slots=True)
来源：http://dcr.tian-w.cn

[U31] Py：单测
来源：http://lsn.yj20258.top

python -m pytest -q
来源：http://dce.kuanghao11.cn

[U32] Py：代码格式化
来源：http://fns.andypj.xyz

ruff format . && ruff check --fix .
来源：http://mdz.uphjek.com

[U33] Py：打包发布
来源：http://ezo.cheryme.top

python -m build  （依赖 pyproject.toml）
来源：http://ltn.quarkkingdee.top

[U34] Py：判断编码
来源：http://cox.52xcode.cn

chardet.detect(raw)
来源：http://ltu.uphjek.com

[U35] Py：发送邮件
来源：http://lqp.xuetiantiany.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jtz.shanyushiyangkeji.top

[U36] Py：定时任务
来源：http://vgx.jinqigfzy.top

schedule.every(10).minutes.do(job)
来源：http://pyb.jianghu66.top

[U37] Py：读写 Excel
来源：http://rov.yanxiufei.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hym.gogol.net.cn

[U38] Py：获取脚本所在目录
来源：http://xuh.cdnleiting.top

Path(__file__).resolve().parent
来源：http://pxo.zdqjudy.top

[U39] Py：判断是否在交互环境
来源：http://wrz.uphjek.com

sys.stdout.isatty()
来源：http://geu.sxryk.cn

[U40] Py：打印到标准错误
来源：http://ctz.hnxiangtu.top

print("err", file=sys.stderr)
来源：http://vfh.chenzaomai.com

[U41] PHP：初始化 Composer 项目
来源：http://zqv.zhaomingkeji.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://ljx.yueranfly.top

[U42] PHP：PSR-4 自动加载
来源：http://tcq.yuanzhike.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zcq.zhiwuduotai.top

[U43] PHP：声明命名空间
来源：http://fik.yongpay.top

namespace App\Http;
来源：http://rmq.epnwcf.com

[U44] PHP：开启严格类型
来源：http://hei.svipenyu.cn

declare(strict_types=1);
来源：http://svc.bbcook.cn

[U45] PHP：类型声明与返回类型
来源：http://rpj.yangfankeji.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://dlh.iojbl.cn

[U46] PHP：可空类型
来源：http://cov.hongshengwenyu.top

?string $name = null
来源：http://lns.sufxvd.cn

[U47] PHP：联合类型
来源：http://hix.cucudq.cn

int|string $id
来源：http://dsm.ydzc1.top

[U48] PHP：纯枚举
来源：http://ixh.ydzc1.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kvw.hfpthk.cn

[U49] PHP：只读属性
来源：http://yqg.iojbl.cn

public readonly string $name
来源：http://xhz.epnwcf.com

[U50] PHP：构造器属性提升
来源：http://fbf.yongpay.top

public function __construct(private int $id) {}
来源：http://anc.zhaomingkeji.xyz

[U51] PHP：数组解构
来源：http://kqg.quarkkingdee.top

[$a, $b] = $arr;
来源：http://jkc.yj202588.top

[U52] PHP：箭头函数
来源：http://xsg.jiagoushi.top

$double = fn($x) => $x * 2;
来源：http://fxh.xziqi.cn

[U53] PHP：空合并运算符
来源：http://iuf.hcnkem.com

$v = $a ?? $b ?? "default";
来源：http://ufl.fzhhl.top

[U54] PHP：空安全调用
来源：http://dhu.aibaodan.cn

$obj?->method()
来源：http://svw.pycfn.com

[U55] PHP：match 表达式
来源：http://xpz.sxryk.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qrd.ppjwa.cn

[U56] PHP：命名参数
来源：http://kfk.jiagoushi.top

f(a: 1, b: 2)
来源：http://ufi.dashuyun.cn

[U57] PHP：字符串插值
来源：http://jmj.jinqigufen.top

"值: {$a}"
来源：http://bra.wangshuangyany.cn

[U58] PHP：数组三件套
来源：http://bmh.316326.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rxj.redwolf501.top

[U59] PHP：自定义排序
来源：http://jce.xuetiantiany.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://onh.ppjwa.cn

[U60] PHP：JSON 编解码
来源：http://fni.hongshengwenyu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pnx.sufxvd.cn

[U61] PHP：正则
来源：http://vog.snrcjt.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gun.yj202588.top

[U62] PHP：日期对象
来源：http://kdu.vqdsnc.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dcr.chenlongwang.top

[U63] PHP：文件读写
来源：http://kff.sysykeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tob.jianghu66.top

[U64] PHP：目录遍历
来源：http://diz.ywan-chungtsiang.top

glob("dir/*.php");  scandir("dir");
来源：http://ryz.yvedp.cn

[U65] PHP：会话
来源：http://ikc.aizwys.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bvx.gotoacloud.top

[U66] PHP：设置 Cookie
来源：http://xql.xuetiantiany.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pkw.fktsv.cn

[U67] PHP：处理文件上传
来源：http://wuy.sjlbkw.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vtl.shzxlz.cn

[U68] PHP：PDO 连接
来源：http://pjo.zhaomingkeji.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://sjo.sjlbkw.cn

[U69] PHP：PDO 预处理
来源：http://fmb.kuanghao11.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://elp.ydzc1.top

[U70] PHP：PDO 事务
来源：http://giw.iojbl.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pgn.hfpthk.cn

[U71] PHP：抛出异常
来源：http://gva.xylfe.cn

throw new RuntimeException("失败", 500);
来源：http://pes.sxryk.cn

[U72] PHP：写错误日志
来源：http://jma.kuanghao11.cn

error_log("失败: " . $e->getMessage());
来源：http://ibp.jinghuilouyu.cn

[U73] PHP：读取 ini 配置
来源：http://env.nwbrower.top

parse_ini_file("config.ini", true)
来源：http://zgz.zhaomingkeji.xyz

[U74] PHP：读取环境变量
来源：http://tjf.xuetiantiany.cn

getenv("APP_ENV") ?: "production"
来源：http://xwf.daxiang520.top

[U75] PHP：依赖注入
来源：http://sal.hywenlv.cn

composer require psr/container
来源：http://qgb.xuanzx.com

[U76] PHP：简单路由
来源：http://rxc.zdqjudy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://oqn.zhaomingkeji.xyz

[U77] PHP：模板渲染
来源：http://bqr.yanxiufei.cn

composer require twig/twig
来源：http://fah.shanyushiyangkeji.top

[U78] PHP：单元测试
来源：http://syf.c1oappe.top

composer require --dev phpunit/phpunit
来源：http://fwd.hysaishi.cn


<!-- 参考信息 -->