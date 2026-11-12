代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://nnt.yuanzhike.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lzk.c1oappe.top

[S48] C++：逐行读文件
来源：http://ilq.havefunace.top

std::ifstream in("a.txt");  std::string line;
来源：http://afk.yuanzhike.top

while (std::getline(in, line)) { }
来源：http://wfb.hywenlv.cn

[S49] C++：写文件
来源：http://xfy.zhijiandao.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fas.yuxming.cn

[S50] C++：格式化数字
来源：http://ses.tian-w.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hah.snrcjt.cn

[S51] C++：显式类型转换
来源：http://hjs.yvedp.cn

static_cast<double>(a) / b
来源：http://jqj.gaohongyu789.top

[S52] C++：const 与 noexcept
来源：http://xfk.snrcjt.cn

int size() const noexcept { return n_; }
来源：http://jdc.nanxuanxn.top

[S53] C++：移动语义
来源：http://xhe.wangdashe.top

std::vector<int> w = std::move(v);
来源：http://esy.ybcxt.top

[S54] C++：异常处理
来源：http://otb.sjlbkw.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tsq.ywan-chungtsiang.top

[S55] C++：结构化绑定
来源：http://www.shangyingyoupin.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zjq.hammf.cn

[S56] C++：optional
来源：http://tky.cqqwz.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pax.jiagoushi.top

[S57] C++：编译期常量
来源：http://gkr.sjlbkw.cn

constexpr int N = 10;
来源：http://jtu.9152youxi.cn

[S58] C++：命名空间
来源：http://pux.9152youxi.cn

namespace ns { int f() { return 1; } }
来源：http://oos.9152youxi.cn

[S59] C++：静态断言
来源：http://xhp.ywan-chungtsiang.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nzq.ybcxt.top

[S60] C++：遍历并删除元素
来源：http://sri.yfazqb.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uug.hesvh.cn

================================================================================
来源：http://rxy.gogol.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bci.ybcxt.top

================================================================================
来源：http://jzg.jinqigfzy.top

[T01] Kotlin：Hello World
来源：http://msi.zhijiandao.cn

println("Hello")
来源：http://fvy.ybcxt.top

[T02] Kotlin：变量
来源：http://jcm.zhoulong.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://teq.yangfankeji.com

[T03] Kotlin：字符串模板
来源：http://rsc.zhaomingkeji.xyz

"值: $b"
来源：http://unr.zhaomingkeji.xyz

[T04] Kotlin：空安全
来源：http://diu.ppjwa.cn

val n: String? = null;  n?.length
来源：http://rmf.hysaishi.cn

[T05] Kotlin：when 表达式
来源：http://eww.jinyuanbaomall.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wlf.jinyuanbaomall.cn

[T06] Kotlin：集合映射
来源：http://mwf.gotoacloud.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zkv.jqgufenzy.top

[T07] Kotlin：集合过滤
来源：http://tdd.ehwqpu.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://lpq.316326.xyz

[T08] Kotlin：数据类
来源：http://rxr.gotoacloud.top

data class User(val name: String, val age: Int)
来源：http://gfj.fanxiaobao.xyz

[T09] Kotlin：扩展函数
来源：http://qbj.yuxming.cn

fun String.exclaim() = this + "!"
来源：http://efj.vqdsnc.cn

[T10] Kotlin：默认参数
来源：http://gfp.jyoumei.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dxl.zhoulong.xyz

[T11] Kotlin：协程
来源：http://cof.0kj1m.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nbx.gzhubu.top

[T12] Kotlin：解构声明
来源：http://zbe.shzxlz.cn

val (a, b) = Pair(1, 2)
来源：http://qvu.yonumen.top

[T13] Kotlin：只读 Map
来源：http://rgj.yueranfly.top

val m = mapOf("a" to 1)
来源：http://iox.jinghuilouyu.cn

[T14] Kotlin：循环
来源：http://tok.ybcxt.top

for (i in 1..10) println(i)
来源：http://yyf.shangyingyoupin.top

[T15] Kotlin：接口
来源：http://mnk.fengsongda.top

interface Shape { fun area(): Double }
来源：http://nuc.vehdjk.com

[T16] Swift：Hello World
来源：http://qpf.hesvh.cn

print("Hello")
来源：http://xao.quarkkingdee.top

[T17] Swift：变量与常量
来源：http://sav.haohaochexian.top

var a = 1;  let b = 2
来源：http://mql.fanxiaobao.xyz

[T18] Swift：字符串插值
来源：http://yoi.tanke756.top

"值: \(b)"
来源：http://ilx.hammf.cn

[T19] Swift：可选绑定
来源：http://sif.feifeiyinyue.top

if let n = opt { print(n) }
来源：http://pja.birdmap.top

[T20] Swift：数组操作
来源：http://kdx.zhaomingkeji.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://kgr.bjfxy.top

[T21] Swift：遍历
来源：http://zok.xuetiantiany.cn

for x in a { print(x) }
来源：http://buy.ivvv.top

[T22] Swift：字典
来源：http://wmh.wangdashe.top

var d = ["a": 1];  d["b"] = 2
来源：http://ucb.bjfxy.top

[T23] Swift：函数
来源：http://rot.316326.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://iso.cashguo.top

[T24] Swift：闭包
来源：http://ocr.xylfe.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yrp.tianlin.xyz

[T25] Swift：结构体
来源：http://bvl.nanxuanxn.top

struct P { var x: Int }
来源：http://ybz.xuetiantiany.cn

[T26] Swift：类与重写
来源：http://zdz.hfpthk.cn

class A: Base { override func f() {} }
来源：http://evg.zhixingplan.top

[T27] Swift：错误处理
来源：http://eca.hcnkem.com

do { try f() } catch { print(error) }
来源：http://kmi.wangshuangyany.cn

[T28] Swift：枚举
来源：http://mok.ppjwa.cn

enum Color { case red, green }
来源：http://kqd.jinghuilouyu.cn

[T29] Swift：guard 提前返回
来源：http://tkj.pengpengdd.cyou

guard let x = opt else { return }
来源：http://hsn.fehbvm.com

[T30] Swift：协议
来源：http://iig.yanxiufei.cn

protocol Shape { func area() -> Double }
来源：http://uql.gogol.net.cn

[T31] Lua：Hello World
来源：http://ozi.hnqzz.top

print("Hello")
来源：http://hev.quarkkingdee.top

[T32] Lua：局部变量
来源：http://jud.yvedp.cn

local a = 1
来源：http://pyw.yj20258888.top

[T33] Lua：表（数组）
来源：http://cym.yj20258.top

local t = {1, 2, 3};  t[4] = 4
来源：http://bnc.zdqjudy.top

[T34] Lua：遍历表
来源：http://dgz.nwbrower.top

for i, v in ipairs(t) do print(i, v) end
来源：http://voj.fktsv.cn

[T35] Lua：字典表
来源：http://pwn.jqgufenzy.top

local d = { a = 1 };  d.b = 2
来源：http://ibm.316326.xyz

[T36] Lua：函数
来源：http://ndi.zhongyouzk.top

function add(a, b) return a + b end
来源：http://sju.yongpay.top

[T37] Lua：字符串拼接
来源：http://otq.hcnkem.com

"a" .. "b"
来源：http://uzi.yj202588.top

[T38] Lua：条件
来源：http://tnf.svipenyu.cn

if x > 0 then print("正") end
来源：http://tsw.ppjwa.cn

[T39] Lua：模式匹配
来源：http://mhv.9152youxi.cn

string.find(s, "%d+")
来源：http://dfo.zhoulong.xyz

[T40] Lua：元表
来源：http://kxh.mhx1999.top

setmetatable({}, { __index = base })
来源：http://ghq.meibo888.top

[T41] Perl：Hello World
来源：http://zsj.hnxiangtu.top

print "Hello\n";
来源：http://zpz.52xcode.cn

[T42] Perl：变量类型
来源：http://gzm.dashuyun.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ids.mhx1999.top

[T43] Perl：字符串插值
来源：http://tmp.yj20258.top

"值: $a"
来源：http://rfv.nwbrower.top

[T44] Perl：条件
来源：http://hnf.mhx1999.top

if ($a > 0) { print "正"; }
来源：http://umw.yuxming.cn

[T45] Perl：数组遍历
来源：http://mqg.epnwcf.com

for my $x (@arr) { print $x; }
来源：http://jdp.sufxvd.cn

[T46] Perl：哈希操作
来源：http://yhi.gogol.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cuv.yongpay.top

[T47] Perl：正则捕获
来源：http://uik.fehbvm.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://zrq.vqdsnc.cn

[T48] Perl：正则替换
来源：http://yrm.yangfankeji.com

$s =~ s/old/new/g;
来源：http://ozg.nwbrower.top

[T49] Perl：函数
来源：http://nnm.hnqzz.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sqi.tanke756.top

[T50] Perl：逐行读文件
来源：http://pcw.ppjwa.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gwx.hesvh.cn

while (my $line = <$fh>) { print $line; }
来源：http://txs.guowangkeji.top

[T51] Scala：Hello World
来源：http://enz.ppjwa.cn

println("Hello")
来源：http://fub.jianghu66.top

[T52] Scala：变量
来源：http://rps.ydjk.org.cn

val a = 1;  var b = 2
来源：http://yen.jinghuilouyu.cn

[T53] Scala：字符串插值
来源：http://nsf.quarkkingdee.top

s"值: $b"
来源：http://ipp.snrcjt.cn

[T54] Scala：集合映射
来源：http://yda.quarkkingdee.top

List(1, 2, 3).map(_ * 2)
来源：http://vtz.ppjwa.cn

[T55] Scala：集合过滤
来源：http://ebv.shanyushiyangkeji.top

List(1, 2, 3).filter(_ > 1)
来源：http://feu.gogol.net.cn

[T56] Scala：样例类
来源：http://tar.ywan-chungtsiang.top

case class User(name: String, age: Int)
来源：http://evf.sxryk.cn

[T57] Scala：模式匹配
来源：http://bxj.yueranfly.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://hxz.zdqjudy.top

[T58] Scala：函数定义
来源：http://ihv.gaohongyu789.top

def add(a: Int, b: Int): Int = a + b
来源：http://ojr.ydjk.org.cn

[T59] Scala：循环
来源：http://njd.fzhhl.top

for (i <- 1 to 10) println(i)
来源：http://gnc.9152youxi.cn

[T60] Scala：折叠
来源：http://fdq.xuetiantiany.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ebk.bjfxy.top

================================================================================
来源：http://lmy.fktsv.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lgm.zhijiandao.cn

================================================================================
来源：http://upq.zhoulong.xyz

[U01] Py：创建虚拟环境
来源：http://yfc.hfpthk.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wgj.yuanzhike.top

[U02] Py：导出 / 安装依赖
来源：http://yxf.aibaodan.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jgt.316326.xyz

[U03] Py：加载 .env 配置
来源：http://qhq.kuanghao11.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dbj.sxryk.cn

[U04] Py：变量调试打印
来源：http://ojf.zhongyouzk.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nof.iojbl.cn

[U05] Py：列表去重且保序
来源：http://cdi.hywenlv.cn

list(dict.fromkeys(arr))
来源：http://axv.sxryk.cn

[U06] Py：合并两个字典
来源：http://ujb.tanke756.top

{**a, **b}
来源：http://drn.tanke756.top

[U07] Py：反转字典键值
来源：http://flm.tarul.cn

{v: k for k, v in d.items()}
来源：http://ctu.sjlbkw.cn

[U08] Py：展平二维列表
来源：http://fiu.quarkkingdee.top

[y for x in nested for y in x]
来源：http://dxe.wangshuangyany.cn

[U09] Py：字典取最大值的键
来源：http://ode.chenlongwang.top

max(d, key=d.get)
来源：http://rir.fengsongda.top

[U10] Py：按值排序字典
来源：http://tdf.nanxinkj.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cup.zhongyouzk.top

[U11] Py：生成器表达式
来源：http://anx.xylfe.cn

(x * 2 for x in arr)
来源：http://pkj.yj202588.top

[U12] Py：取出现最多的 3 个元素
来源：http://gkw.hfpthk.cn

Counter(arr).most_common(3)
来源：http://tqk.ehwqpu.com

[U13] Py：固定长度队列
来源：http://sdn.jinqigufen.top

deque(maxlen=10)
来源：http://ceb.jqgfzy.top

[U14] Py：分组收集到列表
来源：http://mwy.meibo888.top

defaultdict(list)
来源：http://xyz.ydzc1.top

[U15] Py：高精度计时
来源：http://wid.snrcjt.cn

t = time.perf_counter()
来源：http://ibx.shzxlz.cn

[U16] Py：命令行参数解析
来源：http://gfn.jinghuilouyu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cmx.yueranfly.top

[U17] Py：初始化日志
来源：http://qkq.hcnkem.com

logging.basicConfig(level=logging.INFO)
来源：http://lbg.hesvh.cn

[U18] Py：预编译正则
来源：http://hqy.feifeiyinyue.top

pat = re.compile(r"\d+")
来源：http://qfe.ywan-chungtsiang.top

[U19] Py：正则替换带回调
来源：http://qpq.svipenyu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ult.cdnleiting.top

[U20] Py：缓存函数结果
来源：http://dsc.shangyingyoupin.top

@functools.lru_cache(maxsize=None)
来源：http://moe.shzxlz.cn

[U21] Py：自定义上下文管理器
来源：http://xwd.jiagoushi.top

@contextlib.contextmanager
来源：http://ylb.daxiang520.top

[U22] Py：矩阵转置
来源：http://cvp.ydzc1.top

list(zip(*m))
来源：http://xbe.mhx1999.top

[U23] Py：分块读取大文件
来源：http://iyj.xuetiantiany.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nfs.zycfv.cn

[U24] Py：路径操作
来源：http://ajz.mhx1999.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rlv.xziqi.cn

[U25] Py：CSV 按字典读
来源：http://mgx.c1oappe.top

csv.DictReader(f)
来源：http://qcv.9152youxi.cn

[U26] Py：并发下载
来源：http://hth.9152youxi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://frt.jinghuilouyu.cn

[U27] Py：异步 HTTP
来源：http://fop.kuanghao11.cn

aiohttp.ClientSession() 配合 async with
来源：http://edv.yueranfly.top

[U28] Py：类型别名
来源：http://atv.birdmap.top

UserId = int
来源：http://hws.shuidangran.top

[U29] Py：属性校验
来源：http://ltq.ybcxt.top

@property 与 @x.setter 配合
来源：http://tqo.fehbvm.com

[U30] Py：数据类
来源：http://ihm.guannengcc.top

@dataclass(slots=True)
来源：http://tjm.ppjwa.cn

[U31] Py：单测
来源：http://qeb.jqgufenzy.top

python -m pytest -q
来源：http://ama.havefunace.top

[U32] Py：代码格式化
来源：http://mil.zdbjq.cn

ruff format . && ruff check --fix .
来源：http://zhz.sjlbkw.cn

[U33] Py：打包发布
来源：http://jwn.haohaochexian.top

python -m build  （依赖 pyproject.toml）
来源：http://viu.daria6918.cn

[U34] Py：判断编码
来源：http://sjb.yueranfly.top

chardet.detect(raw)
来源：http://alt.yongpay.top

[U35] Py：发送邮件
来源：http://aju.bbcook.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bzl.wangshuangyany.cn

[U36] Py：定时任务
来源：http://lwc.dianchejie.cn

schedule.every(10).minutes.do(job)
来源：http://tfv.sysykeji.top

[U37] Py：读写 Excel
来源：http://jmq.hammf.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zdx.yvedp.cn

[U38] Py：获取脚本所在目录
来源：http://fnu.yvedp.cn

Path(__file__).resolve().parent
来源：http://poq.vqdsnc.cn

[U39] Py：判断是否在交互环境
来源：http://nfj.haohaochexian.top

sys.stdout.isatty()
来源：http://nex.gzhubu.top

[U40] Py：打印到标准错误
来源：http://flm.jinqigufen.top

print("err", file=sys.stderr)
来源：http://yfu.cashguo.top

[U41] PHP：初始化 Composer 项目
来源：http://cvt.meibo888.top

composer init;  composer require guzzlehttp/guzzle
来源：http://kpy.yonumen.top

[U42] PHP：PSR-4 自动加载
来源：http://ivu.dianchejie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://iee.ctjpmb.com

[U43] PHP：声明命名空间
来源：http://nyp.ywan-chungtsiang.top

namespace App\Http;
来源：http://nzt.fktsv.cn

[U44] PHP：开启严格类型
来源：http://jxf.yj202588.top

declare(strict_types=1);
来源：http://fhy.fehbvm.com

[U45] PHP：类型声明与返回类型
来源：http://ens.bbcook.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://krp.ydzc1.top

[U46] PHP：可空类型
来源：http://tsn.yanxiufei.cn

?string $name = null
来源：http://uuh.havefunace.top

[U47] PHP：联合类型
来源：http://trg.bbcook.cn

int|string $id
来源：http://lcv.hywenlv.cn

[U48] PHP：纯枚举
来源：http://mko.meibo888.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xgf.cqqwz.cn

[U49] PHP：只读属性
来源：http://gql.yangfankeji.com

public readonly string $name
来源：http://qbs.yangfankeji.com

[U50] PHP：构造器属性提升
来源：http://tlx.yj20258.top

public function __construct(private int $id) {}
来源：http://ynx.52xcode.cn

[U51] PHP：数组解构
来源：http://tvr.pengpengdd.cyou

[$a, $b] = $arr;
来源：http://deg.fanxiaobao.xyz

[U52] PHP：箭头函数
来源：http://swi.yanxiufei.cn

$double = fn($x) => $x * 2;
来源：http://dia.xziqi.cn

[U53] PHP：空合并运算符
来源：http://xck.birdmap.top

$v = $a ?? $b ?? "default";
来源：http://fhx.jlsjyb.cn

[U54] PHP：空安全调用
来源：http://rqs.yongpay.top

$obj?->method()
来源：http://mjp.xuanzx.com

[U55] PHP：match 表达式
来源：http://hze.cashguo.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mhl.ehwqpu.com

[U56] PHP：命名参数
来源：http://ynk.zdbjq.cn

f(a: 1, b: 2)
来源：http://ste.tanke756.top

[U57] PHP：字符串插值
来源：http://xzo.dianchejie.cn

"值: {$a}"
来源：http://ogk.cucudq.cn

[U58] PHP：数组三件套
来源：http://oab.ehwqpu.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zbg.hnxiangtu.top

[U59] PHP：自定义排序
来源：http://qxj.iojbl.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yhq.zhaomingkeji.xyz

[U60] PHP：JSON 编解码
来源：http://cyj.jlsjyb.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gnc.feifeiyinyue.top

[U61] PHP：正则
来源：http://dhg.daxiang520.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://skm.pengpengdd.cyou

[U62] PHP：日期对象
来源：http://xjn.c1oappe.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qpy.0kj1m.cn

[U63] PHP：文件读写
来源：http://mio.havefunace.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ddf.feifeiyinyue.top

[U64] PHP：目录遍历
来源：http://mpw.shangyingyoupin.top

glob("dir/*.php");  scandir("dir");
来源：http://zai.birdmap.top

[U65] PHP：会话
来源：http://iwy.vqdsnc.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://onj.ivvv.top

[U66] PHP：设置 Cookie
来源：http://glx.feifeiyinyue.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://otv.gaohongyu789.top

[U67] PHP：处理文件上传
来源：http://emt.yuxming.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jcj.jinqigufen.top

[U68] PHP：PDO 连接
来源：http://trp.tian-w.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cnj.tian-w.cn

[U69] PHP：PDO 预处理
来源：http://xph.shanyushiyangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hql.sxryk.cn

[U70] PHP：PDO 事务
来源：http://jdb.mhx1999.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yly.ywan-chungtsiang.top

[U71] PHP：抛出异常
来源：http://ngf.zhixingplan.top

throw new RuntimeException("失败", 500);
来源：http://zbw.epnwcf.com

[U72] PHP：写错误日志
来源：http://cqu.gogol.net.cn

error_log("失败: " . $e->getMessage());
来源：http://qdw.zhoulong.xyz


<!-- 参考信息 -->