代发 wailian999

[S45] C++：lambda
来源：http://ooo.cucudq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wpq.ydzc1.top

[S46] C++：函数模板
来源：http://xvw.fehbvm.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://frb.sysykeji.top

[S47] C++：结构化绑定遍历
来源：http://cwj.aibaodan.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://azs.sweek.top

[S48] C++：逐行读文件
来源：http://jxz.daxiang520.top

std::ifstream in("a.txt");  std::string line;
来源：http://gac.dianchejie.cn

while (std::getline(in, line)) { }
来源：http://jlm.kuanghao11.cn

[S49] C++：写文件
来源：http://wqf.wangshuangyany.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pgk.mhx1999.top

[S50] C++：格式化数字
来源：http://zdm.shzxlz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://iez.yj20258888.top

[S51] C++：显式类型转换
来源：http://jhy.dashuyun.cn

static_cast<double>(a) / b
来源：http://ykv.jiagoushi.top

[S52] C++：const 与 noexcept
来源：http://vrk.shuidangran.top

int size() const noexcept { return n_; }
来源：http://wne.iojbl.cn

[S53] C++：移动语义
来源：http://tef.dashuyun.cn

std::vector<int> w = std::move(v);
来源：http://uxh.chenjidiqi.icu

[S54] C++：异常处理
来源：http://hcq.jlsjyb.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kuw.nanxuanxn.top

[S55] C++：结构化绑定
来源：http://yvi.fengsongda.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ddt.ydzc1.top

[S56] C++：optional
来源：http://iyp.jiagoushi.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jdb.jinyuanbaomall.cn

[S57] C++：编译期常量
来源：http://rlf.cdnleiting.top

constexpr int N = 10;
来源：http://mqf.zdqjudy.top

[S58] C++：命名空间
来源：http://qfh.ivvv.top

namespace ns { int f() { return 1; } }
来源：http://sgz.shangyingyoupin.top

[S59] C++：静态断言
来源：http://iqq.uphjek.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vxu.hongshengwenyu.top

[S60] C++：遍历并删除元素
来源：http://rzq.dashuyun.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ekb.bbcook.cn

================================================================================
来源：http://ber.smart0.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://meq.yj20258.top

================================================================================
来源：http://irk.fktsv.cn

[T01] Kotlin：Hello World
来源：http://ymu.yuxming.cn

println("Hello")
来源：http://nhi.hesvh.cn

[T02] Kotlin：变量
来源：http://cad.sxryk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yov.ywan-chungtsiang.top

[T03] Kotlin：字符串模板
来源：http://zfp.feifeiyinyue.top

"值: $b"
来源：http://nsl.yj20258.top

[T04] Kotlin：空安全
来源：http://aql.ydzc1.top

val n: String? = null;  n?.length
来源：http://bmf.hysaishi.cn

[T05] Kotlin：when 表达式
来源：http://mwr.fengsongda.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fsl.zycfv.cn

[T06] Kotlin：集合映射
来源：http://hpz.fzhhl.top

listOf(1, 2, 3).map { it * 2 }
来源：http://svc.shangyingyoupin.top

[T07] Kotlin：集合过滤
来源：http://xfd.snrcjt.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hvt.hesvh.cn

[T08] Kotlin：数据类
来源：http://irj.nanxinkj.top

data class User(val name: String, val age: Int)
来源：http://pjg.ybcxt.top

[T09] Kotlin：扩展函数
来源：http://gzd.cdnleiting.top

fun String.exclaim() = this + "!"
来源：http://jbn.zhiwuduotai.top

[T10] Kotlin：默认参数
来源：http://dry.daxiang520.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wox.iojbl.cn

[T11] Kotlin：协程
来源：http://qgg.jiagoushi.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://evj.chenlongwang.top

[T12] Kotlin：解构声明
来源：http://upe.jlsjyb.cn

val (a, b) = Pair(1, 2)
来源：http://uxn.xziqi.cn

[T13] Kotlin：只读 Map
来源：http://lna.fktsv.cn

val m = mapOf("a" to 1)
来源：http://itc.shzxlz.cn

[T14] Kotlin：循环
来源：http://dsw.yj20258.top

for (i in 1..10) println(i)
来源：http://xtp.fanxiaobao.xyz

[T15] Kotlin：接口
来源：http://bve.hnxiangtu.top

interface Shape { fun area(): Double }
来源：http://rmr.shzxlz.cn

[T16] Swift：Hello World
来源：http://rky.52xcode.cn

print("Hello")
来源：http://pde.chenjidiqi.icu

[T17] Swift：变量与常量
来源：http://php.nanxinkj.top

var a = 1;  let b = 2
来源：http://joe.yangfankeji.com

[T18] Swift：字符串插值
来源：http://bpf.cheryme.top

"值: \(b)"
来源：http://flt.cdnleiting.top

[T19] Swift：可选绑定
来源：http://qwg.tianlin.xyz

if let n = opt { print(n) }
来源：http://daa.yj20258888.top

[T20] Swift：数组操作
来源：http://ehs.bjfxy.top

var a = [1, 2, 3];  a.append(4)
来源：http://vkx.feifeiyinyue.top

[T21] Swift：遍历
来源：http://bvp.jinqigufen.top

for x in a { print(x) }
来源：http://jzp.dashuyun.cn

[T22] Swift：字典
来源：http://hqk.wangdashe.top

var d = ["a": 1];  d["b"] = 2
来源：http://itn.iojbl.cn

[T23] Swift：函数
来源：http://wvw.smart0.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yvz.nwbrower.top

[T24] Swift：闭包
来源：http://cxu.gaohongyu789.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://nyy.haohaochexian.top

[T25] Swift：结构体
来源：http://myi.xuanzx.com

struct P { var x: Int }
来源：http://sca.hysaishi.cn

[T26] Swift：类与重写
来源：http://bfr.andypj.xyz

class A: Base { override func f() {} }
来源：http://adt.tarul.cn

[T27] Swift：错误处理
来源：http://qvy.yj20258888.top

do { try f() } catch { print(error) }
来源：http://cpl.yanxiufei.cn

[T28] Swift：枚举
来源：http://feq.hongshengwenyu.top

enum Color { case red, green }
来源：http://lfu.chenlongwang.top

[T29] Swift：guard 提前返回
来源：http://ljv.fktsv.cn

guard let x = opt else { return }
来源：http://hmf.shzxlz.cn

[T30] Swift：协议
来源：http://zep.hfpthk.cn

protocol Shape { func area() -> Double }
来源：http://pwi.ppjwa.cn

[T31] Lua：Hello World
来源：http://xnk.fzhhl.top

print("Hello")
来源：http://kwu.ehwqpu.com

[T32] Lua：局部变量
来源：http://gch.fanxiaobao.xyz

local a = 1
来源：http://azo.aibaodan.cn

[T33] Lua：表（数组）
来源：http://xwk.mhx1999.top

local t = {1, 2, 3};  t[4] = 4
来源：http://vvx.nwbrower.top

[T34] Lua：遍历表
来源：http://lhg.nanxuanxn.top

for i, v in ipairs(t) do print(i, v) end
来源：http://aly.zhengqikj.top

[T35] Lua：字典表
来源：http://tdp.yonumen.top

local d = { a = 1 };  d.b = 2
来源：http://yxj.c1oappe.top

[T36] Lua：函数
来源：http://ykk.yj202588.top

function add(a, b) return a + b end
来源：http://xhb.havefunace.top

[T37] Lua：字符串拼接
来源：http://odf.chenjidiqi.icu

"a" .. "b"
来源：http://rnt.yj202588.top

[T38] Lua：条件
来源：http://pig.yvedp.cn

if x > 0 then print("正") end
来源：http://jtp.xinyue.icu

[T39] Lua：模式匹配
来源：http://izh.zhaomingkeji.xyz

string.find(s, "%d+")
来源：http://mhv.haohaochexian.top

[T40] Lua：元表
来源：http://qsj.yonumen.top

setmetatable({}, { __index = base })
来源：http://sih.yueranfly.top

[T41] Perl：Hello World
来源：http://upi.hammf.cn

print "Hello\n";
来源：http://dem.nanxinkj.top

[T42] Perl：变量类型
来源：http://sng.vqdsnc.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://drr.shzxlz.cn

[T43] Perl：字符串插值
来源：http://jkv.epnwcf.com

"值: $a"
来源：http://rjf.dianchejie.cn

[T44] Perl：条件
来源：http://kjy.hysaishi.cn

if ($a > 0) { print "正"; }
来源：http://tgz.epnwcf.com

[T45] Perl：数组遍历
来源：http://opt.havefunace.top

for my $x (@arr) { print $x; }
来源：http://pmh.daria6918.cn

[T46] Perl：哈希操作
来源：http://kgu.gaohongyu789.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ues.zhengqikj.top

[T47] Perl：正则捕获
来源：http://yiw.jinghuilouyu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jla.gogol.net.cn

[T48] Perl：正则替换
来源：http://uqk.yongpay.top

$s =~ s/old/new/g;
来源：http://rvx.0kj1m.cn

[T49] Perl：函数
来源：http://ttc.fzhhl.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sju.guannengcc.top

[T50] Perl：逐行读文件
来源：http://nfx.havefunace.top

open my $fh, "<", "a.txt" or die $!;
来源：http://bwt.tianlin.xyz

while (my $line = <$fh>) { print $line; }
来源：http://clu.meibo888.top

[T51] Scala：Hello World
来源：http://app.shzxlz.cn

println("Hello")
来源：http://jao.bbcook.cn

[T52] Scala：变量
来源：http://wgy.dashuyun.cn

val a = 1;  var b = 2
来源：http://fjb.hongshengwenyu.top

[T53] Scala：字符串插值
来源：http://auw.vqdsnc.cn

s"值: $b"
来源：http://xcg.epnwcf.com

[T54] Scala：集合映射
来源：http://ynk.zycfv.cn

List(1, 2, 3).map(_ * 2)
来源：http://cjt.svipenyu.cn

[T55] Scala：集合过滤
来源：http://ybd.nanxuanxn.top

List(1, 2, 3).filter(_ > 1)
来源：http://ntx.chenlongwang.top

[T56] Scala：样例类
来源：http://kkr.daria6918.cn

case class User(name: String, age: Int)
来源：http://fue.birdmap.top

[T57] Scala：模式匹配
来源：http://rnx.chenlongwang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://kog.ydjk.org.cn

[T58] Scala：函数定义
来源：http://brz.dashuyun.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wzu.sysykeji.top

[T59] Scala：循环
来源：http://kna.tian-w.cn

for (i <- 1 to 10) println(i)
来源：http://frd.sufxvd.cn

[T60] Scala：折叠
来源：http://bux.cashguo.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xus.tarul.cn

================================================================================
来源：http://fsd.fzhhl.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cbx.jyoumei.cn

================================================================================
来源：http://vlo.yonumen.top

[U01] Py：创建虚拟环境
来源：http://gbs.svipenyu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nch.chenlongwang.top

[U02] Py：导出 / 安装依赖
来源：http://jjs.pengpengdd.cyou

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oiz.jinghuilouyu.cn

[U03] Py：加载 .env 配置
来源：http://pel.ywan-chungtsiang.top

from dotenv import load_dotenv; load_dotenv()
来源：http://wbv.nanxinkj.top

[U04] Py：变量调试打印
来源：http://zoh.ehwqpu.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://swf.cqqwz.cn

[U05] Py：列表去重且保序
来源：http://sow.cucudq.cn

list(dict.fromkeys(arr))
来源：http://tok.meibo888.top

[U06] Py：合并两个字典
来源：http://gpf.fktsv.cn

{**a, **b}
来源：http://zim.zhijiandao.cn

[U07] Py：反转字典键值
来源：http://xmu.smart0.xyz

{v: k for k, v in d.items()}
来源：http://ahs.wangshuangyany.cn

[U08] Py：展平二维列表
来源：http://lgk.yj20258.top

[y for x in nested for y in x]
来源：http://jnl.zhengqikj.top

[U09] Py：字典取最大值的键
来源：http://lyh.yanxiufei.cn

max(d, key=d.get)
来源：http://asv.iojbl.cn

[U10] Py：按值排序字典
来源：http://eit.guowangkeji.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gat.zhiwuduotai.top

[U11] Py：生成器表达式
来源：http://fjy.chenzaomai.com

(x * 2 for x in arr)
来源：http://xjh.zdbjq.cn

[U12] Py：取出现最多的 3 个元素
来源：http://uri.sufxvd.cn

Counter(arr).most_common(3)
来源：http://xqh.jianghu66.top

[U13] Py：固定长度队列
来源：http://hya.sufxvd.cn

deque(maxlen=10)
来源：http://qyj.wangdashe.top

[U14] Py：分组收集到列表
来源：http://iiv.ctjpmb.com

defaultdict(list)
来源：http://vyl.jyoumei.cn

[U15] Py：高精度计时
来源：http://ygi.aibaodan.cn

t = time.perf_counter()
来源：http://riz.uphjek.com

[U16] Py：命令行参数解析
来源：http://yry.yangfankeji.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://txm.jyoumei.cn

[U17] Py：初始化日志
来源：http://pjl.aizwys.cn

logging.basicConfig(level=logging.INFO)
来源：http://kvr.yonumen.top

[U18] Py：预编译正则
来源：http://msb.c1oappe.top

pat = re.compile(r"\d+")
来源：http://upt.sxryk.cn

[U19] Py：正则替换带回调
来源：http://uff.yongpay.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uvq.jiagoushi.top

[U20] Py：缓存函数结果
来源：http://uau.zdqjudy.top

@functools.lru_cache(maxsize=None)
来源：http://lmz.wangdashe.top

[U21] Py：自定义上下文管理器
来源：http://moq.guowangkeji.top

@contextlib.contextmanager
来源：http://blm.nanxinkj.top

[U22] Py：矩阵转置
来源：http://qlw.fzhhl.top

list(zip(*m))
来源：http://bar.yueranfly.top

[U23] Py：分块读取大文件
来源：http://zrh.zdqjudy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rjq.haohaochexian.top

[U24] Py：路径操作
来源：http://qte.sysykeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://prh.havefunace.top

[U25] Py：CSV 按字典读
来源：http://nvi.wangdashe.top

csv.DictReader(f)
来源：http://ahv.birdmap.top

[U26] Py：并发下载
来源：http://mqa.zhiwuduotai.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://syr.yfazqb.com

[U27] Py：异步 HTTP
来源：http://mot.hywenlv.cn

aiohttp.ClientSession() 配合 async with
来源：http://jkv.xingfuxueyuan.xyz

[U28] Py：类型别名
来源：http://nxg.guannengcc.top

UserId = int
来源：http://fsj.tian-w.cn

[U29] Py：属性校验
来源：http://hum.bjfxy.top

@property 与 @x.setter 配合
来源：http://ebc.ywan-chungtsiang.top

[U30] Py：数据类
来源：http://sxr.quarkkingdee.top

@dataclass(slots=True)
来源：http://zki.hesvh.cn

[U31] Py：单测
来源：http://wsn.zhaomingkeji.xyz

python -m pytest -q
来源：http://oer.fanxiaobao.xyz

[U32] Py：代码格式化
来源：http://jho.zhixingplan.top

ruff format . && ruff check --fix .
来源：http://vfh.pycfn.com

[U33] Py：打包发布
来源：http://vfj.ybcxt.top

python -m build  （依赖 pyproject.toml）
来源：http://sux.jinyuanbaomall.cn

[U34] Py：判断编码
来源：http://ydt.gaohongyu789.top

chardet.detect(raw)
来源：http://btp.shangyingyoupin.top

[U35] Py：发送邮件
来源：http://lxw.dianchejie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://swy.quarkkingdee.top

[U36] Py：定时任务
来源：http://dtf.shuidangran.top

schedule.every(10).minutes.do(job)
来源：http://sln.kuanghao11.cn

[U37] Py：读写 Excel
来源：http://stb.bbcook.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wjh.uphjek.com

[U38] Py：获取脚本所在目录
来源：http://iev.vehdjk.com

Path(__file__).resolve().parent
来源：http://ctg.gogol.net.cn

[U39] Py：判断是否在交互环境
来源：http://sve.vehdjk.com

sys.stdout.isatty()
来源：http://abi.meibo888.top

[U40] Py：打印到标准错误
来源：http://xwg.hcnkem.com

print("err", file=sys.stderr)
来源：http://utq.iojbl.cn

[U41] PHP：初始化 Composer 项目
来源：http://rck.jinyuanbaomall.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fbc.jinyuanbaomall.cn

[U42] PHP：PSR-4 自动加载
来源：http://aqm.52xcode.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ian.hammf.cn

[U43] PHP：声明命名空间
来源：http://rgn.zdqjudy.top

namespace App\Http;
来源：http://cmd.cashguo.top

[U44] PHP：开启严格类型
来源：http://blq.yueranfly.top

declare(strict_types=1);
来源：http://tit.sjlbkw.cn

[U45] PHP：类型声明与返回类型
来源：http://szx.316326.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://jtm.aizwys.cn

[U46] PHP：可空类型
来源：http://ovb.ybcxt.top

?string $name = null
来源：http://lsk.daria6918.cn

[U47] PHP：联合类型
来源：http://tvk.tarul.cn

int|string $id
来源：http://eni.zhiwuduotai.top

[U48] PHP：纯枚举
来源：http://gwu.0kj1m.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://loh.xuanzx.com

[U49] PHP：只读属性
来源：http://tpd.ctjpmb.com

public readonly string $name
来源：http://omo.meibo888.top

[U50] PHP：构造器属性提升
来源：http://srl.ydzc1.top

public function __construct(private int $id) {}
来源：http://caq.jyoumei.cn

[U51] PHP：数组解构
来源：http://bpj.zycfv.cn

[$a, $b] = $arr;
来源：http://vrz.ybcxt.top

[U52] PHP：箭头函数
来源：http://niz.haohaochexian.top

$double = fn($x) => $x * 2;
来源：http://nrj.fktsv.cn

[U53] PHP：空合并运算符
来源：http://qyx.jinqigufen.top

$v = $a ?? $b ?? "default";
来源：http://faa.jqgufenzy.top

[U54] PHP：空安全调用
来源：http://xmw.zhengqikj.top

$obj?->method()
来源：http://sdp.fehbvm.com

[U55] PHP：match 表达式
来源：http://ugq.vehdjk.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vog.yuanzhike.top

[U56] PHP：命名参数
来源：http://ntu.xuanzx.com

f(a: 1, b: 2)
来源：http://cre.quarkkingdee.top

[U57] PHP：字符串插值
来源：http://csn.nwbrower.top

"值: {$a}"
来源：http://yfs.dashuyun.cn

[U58] PHP：数组三件套
来源：http://jth.yj20258.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lmr.zhoulong.xyz

[U59] PHP：自定义排序
来源：http://bem.nwbrower.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pjl.ydjk.org.cn

[U60] PHP：JSON 编解码
来源：http://hgi.jianghu66.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gay.shangyingyoupin.top

[U61] PHP：正则
来源：http://ifs.tian-w.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sjj.zdqjudy.top

[U62] PHP：日期对象
来源：http://fes.gaohongyu789.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wah.epnwcf.com

[U63] PHP：文件读写
来源：http://jfi.0kj1m.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://uuv.yueranfly.top

[U64] PHP：目录遍历
来源：http://ifm.epnwcf.com

glob("dir/*.php");  scandir("dir");
来源：http://qjp.zdqjudy.top

[U65] PHP：会话
来源：http://xet.yueranfly.top

session_start();  $_SESSION["uid"] = 1;
来源：http://hcw.hywenlv.cn

[U66] PHP：设置 Cookie
来源：http://bqc.guannengcc.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rrw.epnwcf.com

[U67] PHP：处理文件上传
来源：http://ubr.pycfn.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fdb.zhiwuduotai.top

[U68] PHP：PDO 连接
来源：http://ikr.shanyushiyangtech.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jvs.sjlbkw.cn

[U69] PHP：PDO 预处理
来源：http://dhg.shangyingyoupin.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jvi.shzxlz.cn

[U70] PHP：PDO 事务
来源：http://pzc.mhx1999.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xfy.yangfankeji.com


<!-- 参考信息 -->