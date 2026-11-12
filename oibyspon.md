代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://feo.jinqigufen.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qfz.zdqjudy.top

[S48] C++：逐行读文件
来源：http://nzz.haohaochexian.top

std::ifstream in("a.txt");  std::string line;
来源：http://rud.jinghuilouyu.cn

while (std::getline(in, line)) { }
来源：http://uch.pengpengdd.cyou

[S49] C++：写文件
来源：http://exh.epnwcf.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wpv.ivvv.top

[S50] C++：格式化数字
来源：http://qzb.guowangkeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qad.zhixingplan.top

[S51] C++：显式类型转换
来源：http://jou.xylfe.cn

static_cast<double>(a) / b
来源：http://jit.hywenlv.cn

[S52] C++：const 与 noexcept
来源：http://yak.xuetiantiany.cn

int size() const noexcept { return n_; }
来源：http://ixd.smart0.xyz

[S53] C++：移动语义
来源：http://fsu.aizwys.cn

std::vector<int> w = std::move(v);
来源：http://tqe.andypj.xyz

[S54] C++：异常处理
来源：http://fiz.52xcode.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yuv.vqdsnc.cn

[S55] C++：结构化绑定
来源：http://agg.meibo888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tro.guowangkeji.top

[S56] C++：optional
来源：http://swj.xuetiantiany.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zar.shuidangran.top

[S57] C++：编译期常量
来源：http://cye.jinqigfzy.top

constexpr int N = 10;
来源：http://pgo.jqgufenzy.top

[S58] C++：命名空间
来源：http://qzi.hongshengwenyu.top

namespace ns { int f() { return 1; } }
来源：http://xpl.hfpthk.cn

[S59] C++：静态断言
来源：http://yie.shangyingyoupin.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fes.hammf.cn

[S60] C++：遍历并删除元素
来源：http://fpo.yuxming.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gyn.gotoacloud.top

================================================================================
来源：http://ncv.xylfe.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sst.xuetiantiany.cn

================================================================================
来源：http://jpk.jyoumei.cn

[T01] Kotlin：Hello World
来源：http://tve.jyoumei.cn

println("Hello")
来源：http://cik.cdnleiting.top

[T02] Kotlin：变量
来源：http://vej.ppjwa.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zay.bbcook.cn

[T03] Kotlin：字符串模板
来源：http://szy.ppjwa.cn

"值: $b"
来源：http://nnp.yj20258888.top

[T04] Kotlin：空安全
来源：http://tpz.hcnkem.com

val n: String? = null;  n?.length
来源：http://kcr.zhiwuduotai.top

[T05] Kotlin：when 表达式
来源：http://aty.316326.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kkq.havefunace.top

[T06] Kotlin：集合映射
来源：http://evn.cheryme.top

listOf(1, 2, 3).map { it * 2 }
来源：http://iwb.havefunace.top

[T07] Kotlin：集合过滤
来源：http://zti.cdnleiting.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nvi.yonumen.top

[T08] Kotlin：数据类
来源：http://cqv.hesvh.cn

data class User(val name: String, val age: Int)
来源：http://pqi.ctjpmb.com

[T09] Kotlin：扩展函数
来源：http://joi.vqdsnc.cn

fun String.exclaim() = this + "!"
来源：http://scz.feifeiyinyue.top

[T10] Kotlin：默认参数
来源：http://kah.snrcjt.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cuc.aibaodan.cn

[T11] Kotlin：协程
来源：http://ose.fehbvm.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://xuy.havefunace.top

[T12] Kotlin：解构声明
来源：http://vwj.hysaishi.cn

val (a, b) = Pair(1, 2)
来源：http://vqc.yonumen.top

[T13] Kotlin：只读 Map
来源：http://gga.shanyushiyangkeji.top

val m = mapOf("a" to 1)
来源：http://tib.jinqigufen.top

[T14] Kotlin：循环
来源：http://opt.dianchejie.cn

for (i in 1..10) println(i)
来源：http://jyu.jqgufenzy.top

[T15] Kotlin：接口
来源：http://fsc.ivvv.top

interface Shape { fun area(): Double }
来源：http://wwq.hnqzz.top

[T16] Swift：Hello World
来源：http://evf.shzxlz.cn

print("Hello")
来源：http://nik.jinghuilouyu.cn

[T17] Swift：变量与常量
来源：http://dns.daxiang520.top

var a = 1;  let b = 2
来源：http://kcg.dashuyun.cn

[T18] Swift：字符串插值
来源：http://omr.zdqjudy.top

"值: \(b)"
来源：http://iih.yanxiufei.cn

[T19] Swift：可选绑定
来源：http://epc.gotoacloud.top

if let n = opt { print(n) }
来源：http://rlc.sweek.top

[T20] Swift：数组操作
来源：http://vvk.iojbl.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fps.cheryme.top

[T21] Swift：遍历
来源：http://rqs.zhijiandao.cn

for x in a { print(x) }
来源：http://mrr.yueranfly.top

[T22] Swift：字典
来源：http://kqr.hnqzz.top

var d = ["a": 1];  d["b"] = 2
来源：http://csj.fktsv.cn

[T23] Swift：函数
来源：http://krc.yj20258888.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gnd.yfazqb.com

[T24] Swift：闭包
来源：http://hlp.gzhubu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://zpn.bjfxy.top

[T25] Swift：结构体
来源：http://nqs.vehdjk.com

struct P { var x: Int }
来源：http://neg.jinqigfzy.top

[T26] Swift：类与重写
来源：http://ams.andypj.xyz

class A: Base { override func f() {} }
来源：http://utn.c1oappe.top

[T27] Swift：错误处理
来源：http://bpw.jiagoushi.top

do { try f() } catch { print(error) }
来源：http://lkr.xinyue.icu

[T28] Swift：枚举
来源：http://noe.jqgufenzy.top

enum Color { case red, green }
来源：http://agf.yj202588.top

[T29] Swift：guard 提前返回
来源：http://mwn.zycfv.cn

guard let x = opt else { return }
来源：http://imy.zhaomingkeji.xyz

[T30] Swift：协议
来源：http://pcs.sweek.top

protocol Shape { func area() -> Double }
来源：http://vaf.hnxiangtu.top

[T31] Lua：Hello World
来源：http://iah.svipenyu.cn

print("Hello")
来源：http://aol.zhixingplan.top

[T32] Lua：局部变量
来源：http://ynv.cashguo.top

local a = 1
来源：http://srh.cdnleiting.top

[T33] Lua：表（数组）
来源：http://lws.snrcjt.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cua.9152youxi.cn

[T34] Lua：遍历表
来源：http://duz.ppjwa.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vsv.yonumen.top

[T35] Lua：字典表
来源：http://jwo.yongpay.top

local d = { a = 1 };  d.b = 2
来源：http://ycw.xuanzx.com

[T36] Lua：函数
来源：http://xmf.svipenyu.cn

function add(a, b) return a + b end
来源：http://mgm.shzxlz.cn

[T37] Lua：字符串拼接
来源：http://sfs.ywan-chungtsiang.top

"a" .. "b"
来源：http://wgj.jqgfzy.top

[T38] Lua：条件
来源：http://fjs.yonumen.top

if x > 0 then print("正") end
来源：http://nod.ehwqpu.com

[T39] Lua：模式匹配
来源：http://enq.yanxiufei.cn

string.find(s, "%d+")
来源：http://yvg.yj20258888.top

[T40] Lua：元表
来源：http://pxo.jyoumei.cn

setmetatable({}, { __index = base })
来源：http://trm.jinyuanbaomall.cn

[T41] Perl：Hello World
来源：http://jys.haohaochexian.top

print "Hello\n";
来源：http://obq.bbcook.cn

[T42] Perl：变量类型
来源：http://qwx.zycfv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hxt.wangdashe.top

[T43] Perl：字符串插值
来源：http://aku.fanxiaobao.xyz

"值: $a"
来源：http://mtx.ctjpmb.com

[T44] Perl：条件
来源：http://oit.birdmap.top

if ($a > 0) { print "正"; }
来源：http://net.xinyue.icu

[T45] Perl：数组遍历
来源：http://rnv.zhengqikj.top

for my $x (@arr) { print $x; }
来源：http://nyy.xingfuxueyuan.xyz

[T46] Perl：哈希操作
来源：http://dpz.svipenyu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ive.guowangkeji.top

[T47] Perl：正则捕获
来源：http://luk.andypj.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://npw.mhx1999.top

[T48] Perl：正则替换
来源：http://vkp.yanxiufei.cn

$s =~ s/old/new/g;
来源：http://buy.svipenyu.cn

[T49] Perl：函数
来源：http://qch.xziqi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://out.9152youxi.cn

[T50] Perl：逐行读文件
来源：http://dpa.redwolf501.top

open my $fh, "<", "a.txt" or die $!;
来源：http://myd.chenzaomai.com

while (my $line = <$fh>) { print $line; }
来源：http://bjt.vqdsnc.cn

[T51] Scala：Hello World
来源：http://qhs.epnwcf.com

println("Hello")
来源：http://lsb.tarul.cn

[T52] Scala：变量
来源：http://mef.hcnkem.com

val a = 1;  var b = 2
来源：http://yey.jinyuanbaomall.cn

[T53] Scala：字符串插值
来源：http://khe.quarkkingdee.top

s"值: $b"
来源：http://yme.hcnkem.com

[T54] Scala：集合映射
来源：http://zos.hysaishi.cn

List(1, 2, 3).map(_ * 2)
来源：http://ayw.fanxiaobao.xyz

[T55] Scala：集合过滤
来源：http://jhu.nanxuanxn.top

List(1, 2, 3).filter(_ > 1)
来源：http://ysa.ppjwa.cn

[T56] Scala：样例类
来源：http://yay.smart0.xyz

case class User(name: String, age: Int)
来源：http://qnk.shuidangran.top

[T57] Scala：模式匹配
来源：http://sgg.pengpengdd.cyou

x match { case 1 => "一"; case _ => "其他" }
来源：http://mes.yuanzhike.top

[T58] Scala：函数定义
来源：http://ovj.jinqigfzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://hsg.gaohongyu789.top

[T59] Scala：循环
来源：http://sws.quarkkingdee.top

for (i <- 1 to 10) println(i)
来源：http://blj.sufxvd.cn

[T60] Scala：折叠
来源：http://cwl.chenjidiqi.icu

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bbo.ppjwa.cn

================================================================================
来源：http://ylm.yongpay.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mtg.fanxiaobao.xyz

================================================================================
来源：http://gsn.meibo888.top

[U01] Py：创建虚拟环境
来源：http://qjg.feifeiyinyue.top

python -m venv .venv && source .venv/bin/activate
来源：http://bto.yj202588.top

[U02] Py：导出 / 安装依赖
来源：http://hze.wangshuangyany.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xem.hywenlv.cn

[U03] Py：加载 .env 配置
来源：http://khc.hammf.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ofz.xingfuxueyuan.xyz

[U04] Py：变量调试打印
来源：http://xcr.yonumen.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bdx.jyoumei.cn

[U05] Py：列表去重且保序
来源：http://ofw.zdbjq.cn

list(dict.fromkeys(arr))
来源：http://jjw.yuxming.cn

[U06] Py：合并两个字典
来源：http://fdp.xziqi.cn

{**a, **b}
来源：http://kpx.zhengqikj.top

[U07] Py：反转字典键值
来源：http://pzb.jinghuilouyu.cn

{v: k for k, v in d.items()}
来源：http://xbz.yuanzhike.top

[U08] Py：展平二维列表
来源：http://ndp.shuidangran.top

[y for x in nested for y in x]
来源：http://jny.dianchejie.cn

[U09] Py：字典取最大值的键
来源：http://ngf.jlsjyb.cn

max(d, key=d.get)
来源：http://mut.nwbrower.top

[U10] Py：按值排序字典
来源：http://egm.xuanzx.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://eju.xinyue.icu

[U11] Py：生成器表达式
来源：http://bet.nanxinkj.top

(x * 2 for x in arr)
来源：http://ffn.daxiang520.top

[U12] Py：取出现最多的 3 个元素
来源：http://lup.yuxming.cn

Counter(arr).most_common(3)
来源：http://wpl.daria6918.cn

[U13] Py：固定长度队列
来源：http://shy.guowangkeji.top

deque(maxlen=10)
来源：http://qyx.zhijiandao.cn

[U14] Py：分组收集到列表
来源：http://oze.guowangkeji.top

defaultdict(list)
来源：http://ajg.hnqzz.top

[U15] Py：高精度计时
来源：http://bkv.ybcxt.top

t = time.perf_counter()
来源：http://kvi.xziqi.cn

[U16] Py：命令行参数解析
来源：http://hzs.shangyingyoupin.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cmp.smart0.xyz

[U17] Py：初始化日志
来源：http://ogc.nwbrower.top

logging.basicConfig(level=logging.INFO)
来源：http://oai.hnxiangtu.top

[U18] Py：预编译正则
来源：http://faj.gogol.net.cn

pat = re.compile(r"\d+")
来源：http://ieu.cashguo.top

[U19] Py：正则替换带回调
来源：http://jvy.wangdashe.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dca.ctjpmb.com

[U20] Py：缓存函数结果
来源：http://plo.xuanzx.com

@functools.lru_cache(maxsize=None)
来源：http://jjz.yanxiufei.cn

[U21] Py：自定义上下文管理器
来源：http://nzp.yj202588.top

@contextlib.contextmanager
来源：http://ovm.kuanghao11.cn

[U22] Py：矩阵转置
来源：http://hlt.redwolf501.top

list(zip(*m))
来源：http://eeb.chenjidiqi.icu

[U23] Py：分块读取大文件
来源：http://vyu.vehdjk.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hbb.yj20258888.top

[U24] Py：路径操作
来源：http://efh.vqdsnc.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cgs.shanyushiyangkeji.top

[U25] Py：CSV 按字典读
来源：http://jia.epnwcf.com

csv.DictReader(f)
来源：http://rih.vehdjk.com

[U26] Py：并发下载
来源：http://eoz.zhoulong.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bxd.ivvv.top

[U27] Py：异步 HTTP
来源：http://xoa.iojbl.cn

aiohttp.ClientSession() 配合 async with
来源：http://gha.52xcode.cn

[U28] Py：类型别名
来源：http://mcw.zhoulong.xyz

UserId = int
来源：http://rrv.aibaodan.cn

[U29] Py：属性校验
来源：http://nrp.bbcook.cn

@property 与 @x.setter 配合
来源：http://ytx.jyoumei.cn

[U30] Py：数据类
来源：http://nmi.yongpay.top

@dataclass(slots=True)
来源：http://uzw.ehwqpu.com

[U31] Py：单测
来源：http://dcp.uphjek.com

python -m pytest -q
来源：http://qdk.fzhhl.top

[U32] Py：代码格式化
来源：http://rva.fktsv.cn

ruff format . && ruff check --fix .
来源：http://wjq.ydjk.org.cn

[U33] Py：打包发布
来源：http://thb.zhixingplan.top

python -m build  （依赖 pyproject.toml）
来源：http://kql.bjfxy.top

[U34] Py：判断编码
来源：http://kki.chenzaomai.com

chardet.detect(raw)
来源：http://yma.cucudq.cn

[U35] Py：发送邮件
来源：http://xzn.mhx1999.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fue.quarkkingdee.top

[U36] Py：定时任务
来源：http://yko.ehwqpu.com

schedule.every(10).minutes.do(job)
来源：http://utp.fehbvm.com

[U37] Py：读写 Excel
来源：http://hzk.uphjek.com

pandas.read_excel / DataFrame.to_excel
来源：http://siw.hammf.cn

[U38] Py：获取脚本所在目录
来源：http://opv.zycfv.cn

Path(__file__).resolve().parent
来源：http://wut.xuetiantiany.cn

[U39] Py：判断是否在交互环境
来源：http://zqj.tarul.cn

sys.stdout.isatty()
来源：http://oah.haohaochexian.top

[U40] Py：打印到标准错误
来源：http://nkz.pycfn.com

print("err", file=sys.stderr)
来源：http://yna.ctjpmb.com

[U41] PHP：初始化 Composer 项目
来源：http://vta.gaohongyu789.top

composer init;  composer require guzzlehttp/guzzle
来源：http://lqq.jyoumei.cn

[U42] PHP：PSR-4 自动加载
来源：http://upl.mhx1999.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fhv.gaohongyu789.top

[U43] PHP：声明命名空间
来源：http://ajm.xingfuxueyuan.xyz

namespace App\Http;
来源：http://jnq.sjlbkw.cn

[U44] PHP：开启严格类型
来源：http://ine.tanke756.top

declare(strict_types=1);
来源：http://exy.zhongyouzk.top

[U45] PHP：类型声明与返回类型
来源：http://kpa.zdbjq.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zqq.gotoacloud.top

[U46] PHP：可空类型
来源：http://wrf.ybcxt.top

?string $name = null
来源：http://phq.daxiang520.top

[U47] PHP：联合类型
来源：http://xts.hywenlv.cn

int|string $id
来源：http://ecv.fengsongda.top

[U48] PHP：纯枚举
来源：http://fyk.xingfuxueyuan.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zks.epnwcf.com

[U49] PHP：只读属性
来源：http://zxr.tanke756.top

public readonly string $name
来源：http://fap.jiagoushi.top

[U50] PHP：构造器属性提升
来源：http://jhl.jinqigfzy.top

public function __construct(private int $id) {}
来源：http://hjq.hongshengwenyu.top

[U51] PHP：数组解构
来源：http://xfh.quarkkingdee.top

[$a, $b] = $arr;
来源：http://njg.tarul.cn

[U52] PHP：箭头函数
来源：http://ynv.chenlongwang.top

$double = fn($x) => $x * 2;
来源：http://nqc.ppjwa.cn

[U53] PHP：空合并运算符
来源：http://hyy.yvedp.cn

$v = $a ?? $b ?? "default";
来源：http://emj.wangshuangyany.cn

[U54] PHP：空安全调用
来源：http://vjw.fehbvm.com

$obj?->method()
来源：http://ibq.jqgfzy.top

[U55] PHP：match 表达式
来源：http://krg.birdmap.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://feq.sysykeji.top

[U56] PHP：命名参数
来源：http://rww.jqgufenzy.top

f(a: 1, b: 2)
来源：http://zxb.xylfe.cn

[U57] PHP：字符串插值
来源：http://yas.jlsjyb.cn

"值: {$a}"
来源：http://qqo.jqgufenzy.top

[U58] PHP：数组三件套
来源：http://lsu.feifeiyinyue.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cjv.sweek.top

[U59] PHP：自定义排序
来源：http://swi.9152youxi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lzj.zhongyouzk.top

[U60] PHP：JSON 编解码
来源：http://iia.ppjwa.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qnb.zhijiandao.cn

[U61] PHP：正则
来源：http://woa.chenjidiqi.icu

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pvo.jinqigfzy.top

[U62] PHP：日期对象
来源：http://ltf.andypj.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://goj.cqqwz.cn

[U63] PHP：文件读写
来源：http://fdz.snrcjt.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jmw.andypj.xyz

[U64] PHP：目录遍历
来源：http://ojx.yangfankeji.com

glob("dir/*.php");  scandir("dir");
来源：http://taf.ybcxt.top

[U65] PHP：会话
来源：http://xyz.hnqzz.top

session_start();  $_SESSION["uid"] = 1;
来源：http://bir.svipenyu.cn

[U66] PHP：设置 Cookie
来源：http://kzd.shangyingyoupin.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hpq.ywan-chungtsiang.top

[U67] PHP：处理文件上传
来源：http://bpa.zycfv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://etq.yj20258888.top

[U68] PHP：PDO 连接
来源：http://lpb.vehdjk.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wwa.zhixingplan.top

[U69] PHP：PDO 预处理
来源：http://fuw.jyoumei.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yqo.shuidangran.top

[U70] PHP：PDO 事务
来源：http://kwy.snrcjt.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ubq.redwolf501.top

[U71] PHP：抛出异常
来源：http://sot.uphjek.com

throw new RuntimeException("失败", 500);
来源：http://fyi.yuxming.cn

[U72] PHP：写错误日志
来源：http://qec.zdbjq.cn

error_log("失败: " . $e->getMessage());
来源：http://kqu.shzxlz.cn


<!-- 参考信息 -->