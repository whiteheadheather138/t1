代发 wailian999

int size() const noexcept { return n_; }
来源：http://jmy.hnqzz.top

[S53] C++：移动语义
来源：http://csb.yuxming.cn

std::vector<int> w = std::move(v);
来源：http://tjz.9152youxi.cn

[S54] C++：异常处理
来源：http://ciz.sjlbkw.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ubm.haohaochexian.top

[S55] C++：结构化绑定
来源：http://dfl.yanxiufei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://uxt.sufxvd.cn

[S56] C++：optional
来源：http://itz.quarkkingdee.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://alr.shanyushiyangkeji.top

[S57] C++：编译期常量
来源：http://npk.jinyuanbaomall.cn

constexpr int N = 10;
来源：http://sbj.aibaodan.cn

[S58] C++：命名空间
来源：http://oun.zycfv.cn

namespace ns { int f() { return 1; } }
来源：http://kds.yonumen.top

[S59] C++：静态断言
来源：http://rcb.snrcjt.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vta.jqgfzy.top

[S60] C++：遍历并删除元素
来源：http://ubm.kuanghao11.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tvt.ivvv.top

================================================================================
来源：http://slf.vehdjk.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xaz.fanxiaobao.xyz

================================================================================
来源：http://hxj.cheryme.top

[T01] Kotlin：Hello World
来源：http://qbm.nanxuanxn.top

println("Hello")
来源：http://bnr.yanxiufei.cn

[T02] Kotlin：变量
来源：http://pcr.nwbrower.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cip.xuetiantiany.cn

[T03] Kotlin：字符串模板
来源：http://ynd.daria6918.cn

"值: $b"
来源：http://krh.vqdsnc.cn

[T04] Kotlin：空安全
来源：http://zjb.nwbrower.top

val n: String? = null;  n?.length
来源：http://rem.ywan-chungtsiang.top

[T05] Kotlin：when 表达式
来源：http://pat.hysaishi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://upv.guannengcc.top

[T06] Kotlin：集合映射
来源：http://mqc.cheryme.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ctu.hfpthk.cn

[T07] Kotlin：集合过滤
来源：http://gyy.ehwqpu.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://gqv.jinghuilouyu.cn

[T08] Kotlin：数据类
来源：http://ymh.cashguo.top

data class User(val name: String, val age: Int)
来源：http://qdm.ivvv.top

[T09] Kotlin：扩展函数
来源：http://pcp.316326.xyz

fun String.exclaim() = this + "!"
来源：http://vlm.xuanzx.com

[T10] Kotlin：默认参数
来源：http://lep.yfazqb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://iaa.daxiang520.top

[T11] Kotlin：协程
来源：http://phe.andypj.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://kuu.hywenlv.cn

[T12] Kotlin：解构声明
来源：http://heb.kuanghao11.cn

val (a, b) = Pair(1, 2)
来源：http://amj.cashguo.top

[T13] Kotlin：只读 Map
来源：http://cwf.wangdashe.top

val m = mapOf("a" to 1)
来源：http://vnp.jyoumei.cn

[T14] Kotlin：循环
来源：http://vee.snrcjt.cn

for (i in 1..10) println(i)
来源：http://lmq.hysaishi.cn

[T15] Kotlin：接口
来源：http://zrh.zhixingplan.top

interface Shape { fun area(): Double }
来源：http://kqd.gogol.net.cn

[T16] Swift：Hello World
来源：http://btc.xylfe.cn

print("Hello")
来源：http://gnn.hnqzz.top

[T17] Swift：变量与常量
来源：http://kwy.wangshuangyany.cn

var a = 1;  let b = 2
来源：http://akb.tanke756.top

[T18] Swift：字符串插值
来源：http://pkx.fehbvm.com

"值: \(b)"
来源：http://qxy.ppjwa.cn

[T19] Swift：可选绑定
来源：http://apb.hammf.cn

if let n = opt { print(n) }
来源：http://wdn.ehwqpu.com

[T20] Swift：数组操作
来源：http://tzm.yonumen.top

var a = [1, 2, 3];  a.append(4)
来源：http://ose.zhiwuduotai.top

[T21] Swift：遍历
来源：http://mor.kuanghao11.cn

for x in a { print(x) }
来源：http://ire.zdqjudy.top

[T22] Swift：字典
来源：http://jct.tanke756.top

var d = ["a": 1];  d["b"] = 2
来源：http://lzv.zdqjudy.top

[T23] Swift：函数
来源：http://bad.sweek.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hrb.cdnleiting.top

[T24] Swift：闭包
来源：http://jpt.jiagoushi.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://wcn.chenlongwang.top

[T25] Swift：结构体
来源：http://mke.xylfe.cn

struct P { var x: Int }
来源：http://don.ppjwa.cn

[T26] Swift：类与重写
来源：http://tix.gzhubu.top

class A: Base { override func f() {} }
来源：http://xcx.fehbvm.com

[T27] Swift：错误处理
来源：http://zim.shzxlz.cn

do { try f() } catch { print(error) }
来源：http://nxf.gaohongyu789.top

[T28] Swift：枚举
来源：http://ibx.haohaochexian.top

enum Color { case red, green }
来源：http://uom.hcnkem.com

[T29] Swift：guard 提前返回
来源：http://jci.shzxlz.cn

guard let x = opt else { return }
来源：http://dgz.fengsongda.top

[T30] Swift：协议
来源：http://fzy.ehwqpu.com

protocol Shape { func area() -> Double }
来源：http://sht.tianlin.xyz

[T31] Lua：Hello World
来源：http://nbu.nanxinkj.top

print("Hello")
来源：http://njz.hnxiangtu.top

[T32] Lua：局部变量
来源：http://frx.yj20258.top

local a = 1
来源：http://fug.svipenyu.cn

[T33] Lua：表（数组）
来源：http://bxc.hywenlv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tgj.shanyushiyangkeji.top

[T34] Lua：遍历表
来源：http://dsm.gotoacloud.top

for i, v in ipairs(t) do print(i, v) end
来源：http://hbz.pengpengdd.cyou

[T35] Lua：字典表
来源：http://cwz.yj20258.top

local d = { a = 1 };  d.b = 2
来源：http://abs.gogol.net.cn

[T36] Lua：函数
来源：http://xeq.kuanghao11.cn

function add(a, b) return a + b end
来源：http://thh.wangshuangyany.cn

[T37] Lua：字符串拼接
来源：http://uyy.xinyue.icu

"a" .. "b"
来源：http://yax.fzhhl.top

[T38] Lua：条件
来源：http://qmz.zhoulong.xyz

if x > 0 then print("正") end
来源：http://xhi.yj202588.top

[T39] Lua：模式匹配
来源：http://fqd.jinyuanbaomall.cn

string.find(s, "%d+")
来源：http://kle.yfazqb.com

[T40] Lua：元表
来源：http://owp.hesvh.cn

setmetatable({}, { __index = base })
来源：http://mkj.svipenyu.cn

[T41] Perl：Hello World
来源：http://xhy.xinyue.icu

print "Hello\n";
来源：http://eoq.shanyushiyangkeji.top

[T42] Perl：变量类型
来源：http://nqh.zdqjudy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rjo.sxryk.cn

[T43] Perl：字符串插值
来源：http://vdv.kuanghao11.cn

"值: $a"
来源：http://nuc.iojbl.cn

[T44] Perl：条件
来源：http://dbo.chenlongwang.top

if ($a > 0) { print "正"; }
来源：http://zee.cashguo.top

[T45] Perl：数组遍历
来源：http://tir.zhaomingkeji.xyz

for my $x (@arr) { print $x; }
来源：http://fhg.tarul.cn

[T46] Perl：哈希操作
来源：http://oax.daria6918.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ibm.yj202588.top

[T47] Perl：正则捕获
来源：http://mcu.feifeiyinyue.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://iom.aibaodan.cn

[T48] Perl：正则替换
来源：http://cfe.smart0.xyz

$s =~ s/old/new/g;
来源：http://rwc.9152youxi.cn

[T49] Perl：函数
来源：http://hfo.cdnleiting.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cis.yj20258888.top

[T50] Perl：逐行读文件
来源：http://vzc.zycfv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ras.fehbvm.com

while (my $line = <$fh>) { print $line; }
来源：http://uvz.52xcode.cn

[T51] Scala：Hello World
来源：http://mce.wangshuangyany.cn

println("Hello")
来源：http://qyg.nanxinkj.top

[T52] Scala：变量
来源：http://ajd.quarkkingdee.top

val a = 1;  var b = 2
来源：http://jqw.gzhubu.top

[T53] Scala：字符串插值
来源：http://oxl.tarul.cn

s"值: $b"
来源：http://ejx.cheryme.top

[T54] Scala：集合映射
来源：http://brq.uphjek.com

List(1, 2, 3).map(_ * 2)
来源：http://ohn.snrcjt.cn

[T55] Scala：集合过滤
来源：http://ypg.xuanzx.com

List(1, 2, 3).filter(_ > 1)
来源：http://ppg.shanyushiyangtech.top

[T56] Scala：样例类
来源：http://lcg.xingfuxueyuan.xyz

case class User(name: String, age: Int)
来源：http://xld.shanyushiyangtech.top

[T57] Scala：模式匹配
来源：http://ldq.shangyingyoupin.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vrn.svipenyu.cn

[T58] Scala：函数定义
来源：http://czo.yfazqb.com

def add(a: Int, b: Int): Int = a + b
来源：http://lkw.gotoacloud.top

[T59] Scala：循环
来源：http://irg.gzhubu.top

for (i <- 1 to 10) println(i)
来源：http://edr.hnxiangtu.top

[T60] Scala：折叠
来源：http://eyy.cashguo.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jjx.daxiang520.top

================================================================================
来源：http://lwn.yj20258.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qub.zycfv.cn

================================================================================
来源：http://hto.ppjwa.cn

[U01] Py：创建虚拟环境
来源：http://lhn.uphjek.com

python -m venv .venv && source .venv/bin/activate
来源：http://gqz.sufxvd.cn

[U02] Py：导出 / 安装依赖
来源：http://iye.quarkkingdee.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uip.wangdashe.top

[U03] Py：加载 .env 配置
来源：http://eux.epnwcf.com

from dotenv import load_dotenv; load_dotenv()
来源：http://iea.shzxlz.cn

[U04] Py：变量调试打印
来源：http://noc.iojbl.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mfh.c1oappe.top

[U05] Py：列表去重且保序
来源：http://gpm.xuanzx.com

list(dict.fromkeys(arr))
来源：http://kjk.jlsjyb.cn

[U06] Py：合并两个字典
来源：http://pob.zycfv.cn

{**a, **b}
来源：http://bmo.mhx1999.top

[U07] Py：反转字典键值
来源：http://det.yangfankeji.com

{v: k for k, v in d.items()}
来源：http://wmy.shzxlz.cn

[U08] Py：展平二维列表
来源：http://kox.redwolf501.top

[y for x in nested for y in x]
来源：http://srf.snrcjt.cn

[U09] Py：字典取最大值的键
来源：http://deq.sufxvd.cn

max(d, key=d.get)
来源：http://vje.cqqwz.cn

[U10] Py：按值排序字典
来源：http://yhd.haohaochexian.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xax.hammf.cn

[U11] Py：生成器表达式
来源：http://gfx.jlsjyb.cn

(x * 2 for x in arr)
来源：http://cxv.0kj1m.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dlr.zycfv.cn

Counter(arr).most_common(3)
来源：http://pvz.tian-w.cn

[U13] Py：固定长度队列
来源：http://gye.fktsv.cn

deque(maxlen=10)
来源：http://fpf.dashuyun.cn

[U14] Py：分组收集到列表
来源：http://dii.yj20258.top

defaultdict(list)
来源：http://llp.vehdjk.com

[U15] Py：高精度计时
来源：http://eza.bbcook.cn

t = time.perf_counter()
来源：http://tws.yueranfly.top

[U16] Py：命令行参数解析
来源：http://fhq.yvedp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://tio.zhixingplan.top

[U17] Py：初始化日志
来源：http://nfz.mhx1999.top

logging.basicConfig(level=logging.INFO)
来源：http://dvo.jinyuanbaomall.cn

[U18] Py：预编译正则
来源：http://ujd.fanxiaobao.xyz

pat = re.compile(r"\d+")
来源：http://zhg.pengpengdd.cyou

[U19] Py：正则替换带回调
来源：http://dtf.zhoulong.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://obh.gaohongyu789.top

[U20] Py：缓存函数结果
来源：http://wfw.daxiang520.top

@functools.lru_cache(maxsize=None)
来源：http://nhx.tianlin.xyz

[U21] Py：自定义上下文管理器
来源：http://fyy.yj20258888.top

@contextlib.contextmanager
来源：http://cbh.bbcook.cn

[U22] Py：矩阵转置
来源：http://aor.sufxvd.cn

list(zip(*m))
来源：http://rjt.hammf.cn

[U23] Py：分块读取大文件
来源：http://roj.meibo888.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wwf.hongshengwenyu.top

[U24] Py：路径操作
来源：http://sur.xuetiantiany.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ghz.nanxuanxn.top

[U25] Py：CSV 按字典读
来源：http://eib.yuanzhike.top

csv.DictReader(f)
来源：http://aai.yueranfly.top

[U26] Py：并发下载
来源：http://lez.yj20258888.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://utc.fktsv.cn

[U27] Py：异步 HTTP
来源：http://zxd.jinyuanbaomall.cn

aiohttp.ClientSession() 配合 async with
来源：http://zif.yueranfly.top

[U28] Py：类型别名
来源：http://nfq.dashuyun.cn

UserId = int
来源：http://dqk.c1oappe.top

[U29] Py：属性校验
来源：http://shu.sweek.top

@property 与 @x.setter 配合
来源：http://thg.chenzaomai.com

[U30] Py：数据类
来源：http://wzl.chenzaomai.com

@dataclass(slots=True)
来源：http://ohf.jlsjyb.cn

[U31] Py：单测
来源：http://ipn.zhaomingkeji.xyz

python -m pytest -q
来源：http://dqk.hysaishi.cn

[U32] Py：代码格式化
来源：http://asc.yongpay.top

ruff format . && ruff check --fix .
来源：http://cul.fengsongda.top

[U33] Py：打包发布
来源：http://ywc.bjfxy.top

python -m build  （依赖 pyproject.toml）
来源：http://mkb.sxryk.cn

[U34] Py：判断编码
来源：http://tzt.hnqzz.top

chardet.detect(raw)
来源：http://ycu.meibo888.top

[U35] Py：发送邮件
来源：http://guk.fehbvm.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gag.hywenlv.cn

[U36] Py：定时任务
来源：http://ddq.zhijiandao.cn

schedule.every(10).minutes.do(job)
来源：http://ojz.zycfv.cn

[U37] Py：读写 Excel
来源：http://xrt.yj20258888.top

pandas.read_excel / DataFrame.to_excel
来源：http://jsc.xuetiantiany.cn

[U38] Py：获取脚本所在目录
来源：http://kqu.hongshengwenyu.top

Path(__file__).resolve().parent
来源：http://ehj.tianlin.xyz

[U39] Py：判断是否在交互环境
来源：http://ltq.jqgfzy.top

sys.stdout.isatty()
来源：http://bpe.ctjpmb.com

[U40] Py：打印到标准错误
来源：http://hxp.jinqigfzy.top

print("err", file=sys.stderr)
来源：http://zvt.shzxlz.cn

[U41] PHP：初始化 Composer 项目
来源：http://pvx.xingfuxueyuan.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://rch.hcnkem.com

[U42] PHP：PSR-4 自动加载
来源：http://qzm.yvedp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cyz.ivvv.top

[U43] PHP：声明命名空间
来源：http://uuz.jqgufenzy.top

namespace App\Http;
来源：http://ooe.zhaomingkeji.xyz

[U44] PHP：开启严格类型
来源：http://xmr.gogol.net.cn

declare(strict_types=1);
来源：http://wvs.cheryme.top

[U45] PHP：类型声明与返回类型
来源：http://wuo.hesvh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vzt.jinyuanbaomall.cn

[U46] PHP：可空类型
来源：http://sex.gzhubu.top

?string $name = null
来源：http://ddw.yj20258888.top

[U47] PHP：联合类型
来源：http://plp.yj20258.top

int|string $id
来源：http://omj.xinyue.icu

[U48] PHP：纯枚举
来源：http://txs.guowangkeji.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qhb.fanxiaobao.xyz

[U49] PHP：只读属性
来源：http://lby.shzxlz.cn

public readonly string $name
来源：http://bto.aizwys.cn

[U50] PHP：构造器属性提升
来源：http://lxy.fktsv.cn

public function __construct(private int $id) {}
来源：http://szc.vqdsnc.cn

[U51] PHP：数组解构
来源：http://gzz.tarul.cn

[$a, $b] = $arr;
来源：http://wmb.dashuyun.cn

[U52] PHP：箭头函数
来源：http://ist.jinqigufen.top

$double = fn($x) => $x * 2;
来源：http://imd.shanyushiyangkeji.top

[U53] PHP：空合并运算符
来源：http://fsi.svipenyu.cn

$v = $a ?? $b ?? "default";
来源：http://nvh.52xcode.cn

[U54] PHP：空安全调用
来源：http://fzb.shuidangran.top

$obj?->method()
来源：http://wsk.ehwqpu.com

[U55] PHP：match 表达式
来源：http://eqy.xuanzx.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hhc.chenzaomai.com

[U56] PHP：命名参数
来源：http://gcu.sxryk.cn

f(a: 1, b: 2)
来源：http://yuu.yueranfly.top

[U57] PHP：字符串插值
来源：http://dld.zhongyouzk.top

"值: {$a}"
来源：http://xai.xylfe.cn

[U58] PHP：数组三件套
来源：http://xma.9152youxi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fgs.jlsjyb.cn

[U59] PHP：自定义排序
来源：http://nxd.daria6918.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eep.ehwqpu.com

[U60] PHP：JSON 编解码
来源：http://wvs.nanxinkj.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://aat.nanxuanxn.top

[U61] PHP：正则
来源：http://oxc.cashguo.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wlr.gogol.net.cn

[U62] PHP：日期对象
来源：http://dxr.nwbrower.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xiq.jinghuilouyu.cn

[U63] PHP：文件读写
来源：http://ppt.bbcook.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ssm.yonumen.top

[U64] PHP：目录遍历
来源：http://okb.yongpay.top

glob("dir/*.php");  scandir("dir");
来源：http://nlr.xuetiantiany.cn

[U65] PHP：会话
来源：http://lue.chenzaomai.com

session_start();  $_SESSION["uid"] = 1;
来源：http://hun.epnwcf.com

[U66] PHP：设置 Cookie
来源：http://wdq.pengpengdd.cyou

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wxu.yangfankeji.com

[U67] PHP：处理文件上传
来源：http://ppu.ppjwa.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dmj.nanxinkj.top

[U68] PHP：PDO 连接
来源：http://umt.hongshengwenyu.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lui.zhaomingkeji.xyz

[U69] PHP：PDO 预处理
来源：http://jlt.ydjk.org.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gow.ydjk.org.cn

[U70] PHP：PDO 事务
来源：http://vst.cashguo.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tjq.hnxiangtu.top

[U71] PHP：抛出异常
来源：http://iiv.redwolf501.top

throw new RuntimeException("失败", 500);
来源：http://gpz.fehbvm.com

[U72] PHP：写错误日志
来源：http://qbu.xziqi.cn

error_log("失败: " . $e->getMessage());
来源：http://sxj.smart0.xyz

[U73] PHP：读取 ini 配置
来源：http://ezu.xinyue.icu

parse_ini_file("config.ini", true)
来源：http://gxc.hywenlv.cn

[U74] PHP：读取环境变量
来源：http://slu.meibo888.top

getenv("APP_ENV") ?: "production"
来源：http://pgp.yonumen.top

[U75] PHP：依赖注入
来源：http://xui.shuidangran.top

composer require psr/container
来源：http://sme.zycfv.cn

[U76] PHP：简单路由
来源：http://vay.gogol.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tfy.jqgfzy.top

[U77] PHP：模板渲染
来源：http://kby.bjfxy.top

composer require twig/twig
来源：http://iej.bbcook.cn

[U78] PHP：单元测试
来源：http://wjk.jqgfzy.top

composer require --dev phpunit/phpunit
来源：http://qll.9152youxi.cn


<!-- 参考信息 -->