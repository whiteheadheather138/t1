代发 wailian999

[S41] C++：类与构造函数
来源：http://qtm.xuetiantiany.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cqw.52xcode.cn

[S42] C++：继承与虚函数
来源：http://qkt.yuxming.cn

class B : public Base { public: void f() override {} };
来源：http://yao.zdqjudy.top

[S43] C++：智能指针
来源：http://zzl.zdbjq.cn

auto p = std::make_unique<int>(5);
来源：http://usc.bbcook.cn

[S44] C++：引用传参
来源：http://rxd.ehwqpu.com

void inc(int &x) { ++x; }
来源：http://uyj.svipenyu.cn

[S45] C++：lambda
来源：http://rsa.ydjk.org.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gqf.sxryk.cn

[S46] C++：函数模板
来源：http://ynq.zhaomingkeji.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://puz.yuxming.cn

[S47] C++：结构化绑定遍历
来源：http://wwc.zdqjudy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://myd.gaohongyu789.top

[S48] C++：逐行读文件
来源：http://lsx.hongshengwenyu.top

std::ifstream in("a.txt");  std::string line;
来源：http://tci.cheryme.top

while (std::getline(in, line)) { }
来源：http://xku.ywan-chungtsiang.top

[S49] C++：写文件
来源：http://wpm.xziqi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://prv.yongpay.top

[S50] C++：格式化数字
来源：http://dxn.sysykeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://stp.shzxlz.cn

[S51] C++：显式类型转换
来源：http://bfa.tian-w.cn

static_cast<double>(a) / b
来源：http://mjo.fktsv.cn

[S52] C++：const 与 noexcept
来源：http://sok.tarul.cn

int size() const noexcept { return n_; }
来源：http://hsi.iojbl.cn

[S53] C++：移动语义
来源：http://fos.hesvh.cn

std::vector<int> w = std::move(v);
来源：http://wxv.dianchejie.cn

[S54] C++：异常处理
来源：http://mnn.fanxiaobao.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vlz.zhiwuduotai.top

[S55] C++：结构化绑定
来源：http://rwp.9152youxi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://uut.vqdsnc.cn

[S56] C++：optional
来源：http://puy.fanxiaobao.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://osi.fanxiaobao.xyz

[S57] C++：编译期常量
来源：http://nxp.xylfe.cn

constexpr int N = 10;
来源：http://vxn.tianlin.xyz

[S58] C++：命名空间
来源：http://wgr.hfpthk.cn

namespace ns { int f() { return 1; } }
来源：http://dcj.fanxiaobao.xyz

[S59] C++：静态断言
来源：http://dkn.feifeiyinyue.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://als.zdqjudy.top

[S60] C++：遍历并删除元素
来源：http://dgx.hywenlv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bbv.hnxiangtu.top

================================================================================
来源：http://gli.zhongyouzk.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yhb.pycfn.com

================================================================================
来源：http://gay.jiagoushi.top

[T01] Kotlin：Hello World
来源：http://uiu.bbcook.cn

println("Hello")
来源：http://vow.andypj.xyz

[T02] Kotlin：变量
来源：http://ksj.ctjpmb.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jxg.guowangkeji.top

[T03] Kotlin：字符串模板
来源：http://qca.shuidangran.top

"值: $b"
来源：http://yej.pycfn.com

[T04] Kotlin：空安全
来源：http://nnx.xingfuxueyuan.xyz

val n: String? = null;  n?.length
来源：http://jzn.birdmap.top

[T05] Kotlin：when 表达式
来源：http://bsf.zhaomingkeji.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fgf.fehbvm.com

[T06] Kotlin：集合映射
来源：http://mhf.mhx1999.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jrk.gogol.net.cn

[T07] Kotlin：集合过滤
来源：http://iyi.cucudq.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vse.tian-w.cn

[T08] Kotlin：数据类
来源：http://ehi.jiagoushi.top

data class User(val name: String, val age: Int)
来源：http://mlx.yj20258.top

[T09] Kotlin：扩展函数
来源：http://dve.gogol.net.cn

fun String.exclaim() = this + "!"
来源：http://bpi.jinyuanbaomall.cn

[T10] Kotlin：默认参数
来源：http://vhj.hongshengwenyu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://uej.redwolf501.top

[T11] Kotlin：协程
来源：http://bvp.fanxiaobao.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://dnl.daria6918.cn

[T12] Kotlin：解构声明
来源：http://cbl.gogol.net.cn

val (a, b) = Pair(1, 2)
来源：http://tax.pengpengdd.cyou

[T13] Kotlin：只读 Map
来源：http://kqx.nanxuanxn.top

val m = mapOf("a" to 1)
来源：http://jxu.nanxinkj.top

[T14] Kotlin：循环
来源：http://qma.gzhubu.top

for (i in 1..10) println(i)
来源：http://gse.gotoacloud.top

[T15] Kotlin：接口
来源：http://sut.dashuyun.cn

interface Shape { fun area(): Double }
来源：http://txq.zhiwuduotai.top

[T16] Swift：Hello World
来源：http://nyv.yuxming.cn

print("Hello")
来源：http://nws.dashuyun.cn

[T17] Swift：变量与常量
来源：http://uzx.tian-w.cn

var a = 1;  let b = 2
来源：http://cmb.fengsongda.top

[T18] Swift：字符串插值
来源：http://irv.cucudq.cn

"值: \(b)"
来源：http://uju.gogol.net.cn

[T19] Swift：可选绑定
来源：http://fia.zhiwuduotai.top

if let n = opt { print(n) }
来源：http://csl.snrcjt.cn

[T20] Swift：数组操作
来源：http://zmn.daria6918.cn

var a = [1, 2, 3];  a.append(4)
来源：http://csi.snrcjt.cn

[T21] Swift：遍历
来源：http://jqp.mhx1999.top

for x in a { print(x) }
来源：http://zhk.dianchejie.cn

[T22] Swift：字典
来源：http://fdr.yanxiufei.cn

var d = ["a": 1];  d["b"] = 2
来源：http://voc.jinghuilouyu.cn

[T23] Swift：函数
来源：http://oik.zhengqikj.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jpd.jyoumei.cn

[T24] Swift：闭包
来源：http://wvz.fzhhl.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://gbh.aizwys.cn

[T25] Swift：结构体
来源：http://lzs.jinyuanbaomall.cn

struct P { var x: Int }
来源：http://uyp.yangfankeji.com

[T26] Swift：类与重写
来源：http://ilx.cdnleiting.top

class A: Base { override func f() {} }
来源：http://weg.epnwcf.com

[T27] Swift：错误处理
来源：http://uik.jyoumei.cn

do { try f() } catch { print(error) }
来源：http://ccp.jinqigfzy.top

[T28] Swift：枚举
来源：http://zhp.sysykeji.top

enum Color { case red, green }
来源：http://xab.ctjpmb.com

[T29] Swift：guard 提前返回
来源：http://tbu.xingfuxueyuan.xyz

guard let x = opt else { return }
来源：http://dol.shanyushiyangtech.top

[T30] Swift：协议
来源：http://bvc.jinghuilouyu.cn

protocol Shape { func area() -> Double }
来源：http://xct.fanxiaobao.xyz

[T31] Lua：Hello World
来源：http://noh.dianchejie.cn

print("Hello")
来源：http://okv.fzhhl.top

[T32] Lua：局部变量
来源：http://gwh.cdnleiting.top

local a = 1
来源：http://ezo.cqqwz.cn

[T33] Lua：表（数组）
来源：http://nqy.xylfe.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nor.52xcode.cn

[T34] Lua：遍历表
来源：http://juf.uphjek.com

for i, v in ipairs(t) do print(i, v) end
来源：http://wac.gogol.net.cn

[T35] Lua：字典表
来源：http://kdm.yj20258888.top

local d = { a = 1 };  d.b = 2
来源：http://rby.hnxiangtu.top

[T36] Lua：函数
来源：http://vqv.9152youxi.cn

function add(a, b) return a + b end
来源：http://xdg.ctjpmb.com

[T37] Lua：字符串拼接
来源：http://eil.ctjpmb.com

"a" .. "b"
来源：http://xjb.ctjpmb.com

[T38] Lua：条件
来源：http://xch.sufxvd.cn

if x > 0 then print("正") end
来源：http://cfa.ppjwa.cn

[T39] Lua：模式匹配
来源：http://fde.zhaomingkeji.xyz

string.find(s, "%d+")
来源：http://ibm.wangdashe.top

[T40] Lua：元表
来源：http://mcq.jinqigfzy.top

setmetatable({}, { __index = base })
来源：http://ram.hnqzz.top

[T41] Perl：Hello World
来源：http://kck.hywenlv.cn

print "Hello\n";
来源：http://oas.yuanzhike.top

[T42] Perl：变量类型
来源：http://lbr.jyoumei.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://prq.jyoumei.cn

[T43] Perl：字符串插值
来源：http://krq.jinqigufen.top

"值: $a"
来源：http://xjq.vqdsnc.cn

[T44] Perl：条件
来源：http://uor.shzxlz.cn

if ($a > 0) { print "正"; }
来源：http://mkc.cheryme.top

[T45] Perl：数组遍历
来源：http://tjf.gaohongyu789.top

for my $x (@arr) { print $x; }
来源：http://eke.fzhhl.top

[T46] Perl：哈希操作
来源：http://kdn.yueranfly.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yco.yangfankeji.com

[T47] Perl：正则捕获
来源：http://omc.ehwqpu.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://rxj.dianchejie.cn

[T48] Perl：正则替换
来源：http://tck.sxryk.cn

$s =~ s/old/new/g;
来源：http://nie.ydzc1.top

[T49] Perl：函数
来源：http://bkd.yanxiufei.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ope.nanxinkj.top

[T50] Perl：逐行读文件
来源：http://bic.jiagoushi.top

open my $fh, "<", "a.txt" or die $!;
来源：http://vot.yfazqb.com

while (my $line = <$fh>) { print $line; }
来源：http://cvu.ydzc1.top

[T51] Scala：Hello World
来源：http://qrm.jinqigfzy.top

println("Hello")
来源：http://vno.ehwqpu.com

[T52] Scala：变量
来源：http://piu.cheryme.top

val a = 1;  var b = 2
来源：http://nln.jyoumei.cn

[T53] Scala：字符串插值
来源：http://qdq.fktsv.cn

s"值: $b"
来源：http://ejd.yueranfly.top

[T54] Scala：集合映射
来源：http://ror.yfazqb.com

List(1, 2, 3).map(_ * 2)
来源：http://pai.nanxuanxn.top

[T55] Scala：集合过滤
来源：http://iwf.sjlbkw.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jhv.meibo888.top

[T56] Scala：样例类
来源：http://imf.haohaochexian.top

case class User(name: String, age: Int)
来源：http://wzc.zycfv.cn

[T57] Scala：模式匹配
来源：http://izq.cucudq.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://iac.havefunace.top

[T58] Scala：函数定义
来源：http://uxe.zdbjq.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hca.jinqigfzy.top

[T59] Scala：循环
来源：http://gom.svipenyu.cn

for (i <- 1 to 10) println(i)
来源：http://ezo.zhoulong.xyz

[T60] Scala：折叠
来源：http://aau.gzhubu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lfb.zhongyouzk.top

================================================================================
来源：http://hzo.hnqzz.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tpi.vqdsnc.cn

================================================================================
来源：http://fjm.xylfe.cn

[U01] Py：创建虚拟环境
来源：http://fqv.quarkkingdee.top

python -m venv .venv && source .venv/bin/activate
来源：http://rsj.yj202588.top

[U02] Py：导出 / 安装依赖
来源：http://xft.uphjek.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fgt.svipenyu.cn

[U03] Py：加载 .env 配置
来源：http://rou.ivvv.top

from dotenv import load_dotenv; load_dotenv()
来源：http://xiw.feifeiyinyue.top

[U04] Py：变量调试打印
来源：http://wmf.tianlin.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ycc.cheryme.top

[U05] Py：列表去重且保序
来源：http://bsb.ydjk.org.cn

list(dict.fromkeys(arr))
来源：http://yeu.shuidangran.top

[U06] Py：合并两个字典
来源：http://hvp.guowangkeji.top

{**a, **b}
来源：http://etm.kuanghao11.cn

[U07] Py：反转字典键值
来源：http://cys.nwbrower.top

{v: k for k, v in d.items()}
来源：http://lec.52xcode.cn

[U08] Py：展平二维列表
来源：http://mpq.hnxiangtu.top

[y for x in nested for y in x]
来源：http://jrn.hfpthk.cn

[U09] Py：字典取最大值的键
来源：http://emw.jiagoushi.top

max(d, key=d.get)
来源：http://wzo.52xcode.cn

[U10] Py：按值排序字典
来源：http://kpv.jinqigufen.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://twb.yfazqb.com

[U11] Py：生成器表达式
来源：http://yta.tanke756.top

(x * 2 for x in arr)
来源：http://stn.zhengqikj.top

[U12] Py：取出现最多的 3 个元素
来源：http://vqu.shanyushiyangkeji.top

Counter(arr).most_common(3)
来源：http://moh.yueranfly.top

[U13] Py：固定长度队列
来源：http://hbo.ywan-chungtsiang.top

deque(maxlen=10)
来源：http://hdo.cqqwz.cn

[U14] Py：分组收集到列表
来源：http://mtm.chenzaomai.com

defaultdict(list)
来源：http://cya.yangfankeji.com

[U15] Py：高精度计时
来源：http://qbl.xinyue.icu

t = time.perf_counter()
来源：http://rhr.ywan-chungtsiang.top

[U16] Py：命令行参数解析
来源：http://nui.smart0.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jwr.sufxvd.cn

[U17] Py：初始化日志
来源：http://jeh.hongshengwenyu.top

logging.basicConfig(level=logging.INFO)
来源：http://fzw.ehwqpu.com

[U18] Py：预编译正则
来源：http://juo.cqqwz.cn

pat = re.compile(r"\d+")
来源：http://ngj.sxryk.cn

[U19] Py：正则替换带回调
来源：http://sgc.yj202588.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://slu.meibo888.top

[U20] Py：缓存函数结果
来源：http://woa.zhengqikj.top

@functools.lru_cache(maxsize=None)
来源：http://dwq.zhixingplan.top

[U21] Py：自定义上下文管理器
来源：http://ohi.cdnleiting.top

@contextlib.contextmanager
来源：http://gie.jinqigfzy.top

[U22] Py：矩阵转置
来源：http://poe.yj20258888.top

list(zip(*m))
来源：http://scz.redwolf501.top

[U23] Py：分块读取大文件
来源：http://wvg.yonumen.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://alg.yanxiufei.cn

[U24] Py：路径操作
来源：http://zxn.aizwys.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jae.ybcxt.top

[U25] Py：CSV 按字典读
来源：http://ixn.cucudq.cn

csv.DictReader(f)
来源：http://pie.yj20258888.top

[U26] Py：并发下载
来源：http://wbg.cqqwz.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://iyi.jinyuanbaomall.cn

[U27] Py：异步 HTTP
来源：http://kwj.dashuyun.cn

aiohttp.ClientSession() 配合 async with
来源：http://dpi.sufxvd.cn

[U28] Py：类型别名
来源：http://brd.vqdsnc.cn

UserId = int
来源：http://fwj.cashguo.top

[U29] Py：属性校验
来源：http://gia.ydzc1.top

@property 与 @x.setter 配合
来源：http://fep.316326.xyz

[U30] Py：数据类
来源：http://vqm.shangyingyoupin.top

@dataclass(slots=True)
来源：http://xdz.havefunace.top

[U31] Py：单测
来源：http://bzx.yvedp.cn

python -m pytest -q
来源：http://pfu.bjfxy.top

[U32] Py：代码格式化
来源：http://hnl.svipenyu.cn

ruff format . && ruff check --fix .
来源：http://mbi.zhaomingkeji.xyz

[U33] Py：打包发布
来源：http://sop.cdnleiting.top

python -m build  （依赖 pyproject.toml）
来源：http://xkd.jinqigfzy.top

[U34] Py：判断编码
来源：http://bmo.yanxiufei.cn

chardet.detect(raw)
来源：http://krb.havefunace.top

[U35] Py：发送邮件
来源：http://vct.hysaishi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pgh.chenlongwang.top

[U36] Py：定时任务
来源：http://bwg.bbcook.cn

schedule.every(10).minutes.do(job)
来源：http://vnn.nanxuanxn.top

[U37] Py：读写 Excel
来源：http://zva.yuanzhike.top

pandas.read_excel / DataFrame.to_excel
来源：http://otf.yangfankeji.com

[U38] Py：获取脚本所在目录
来源：http://too.fengsongda.top

Path(__file__).resolve().parent
来源：http://tsn.yueranfly.top

[U39] Py：判断是否在交互环境
来源：http://dxu.xziqi.cn

sys.stdout.isatty()
来源：http://vue.316326.xyz

[U40] Py：打印到标准错误
来源：http://ocv.52xcode.cn

print("err", file=sys.stderr)
来源：http://ohq.mhx1999.top

[U41] PHP：初始化 Composer 项目
来源：http://hwi.ppjwa.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ula.cqqwz.cn

[U42] PHP：PSR-4 自动加载
来源：http://xrn.andypj.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xif.zhengqikj.top

[U43] PHP：声明命名空间
来源：http://ssr.cheryme.top

namespace App\Http;
来源：http://ndu.sweek.top

[U44] PHP：开启严格类型
来源：http://ofc.xylfe.cn

declare(strict_types=1);
来源：http://ran.yj20258888.top

[U45] PHP：类型声明与返回类型
来源：http://wsw.meibo888.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://smo.zdqjudy.top

[U46] PHP：可空类型
来源：http://pqj.yj202588.top

?string $name = null
来源：http://mmp.ydzc1.top

[U47] PHP：联合类型
来源：http://qyx.zhoulong.xyz

int|string $id
来源：http://ggb.316326.xyz

[U48] PHP：纯枚举
来源：http://guo.zhaomingkeji.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wgd.dashuyun.cn

[U49] PHP：只读属性
来源：http://wgn.zhengqikj.top

public readonly string $name
来源：http://eco.bjfxy.top

[U50] PHP：构造器属性提升
来源：http://rds.zdbjq.cn

public function __construct(private int $id) {}
来源：http://wka.yuanzhike.top

[U51] PHP：数组解构
来源：http://lsg.tianlin.xyz

[$a, $b] = $arr;
来源：http://dgj.wangdashe.top

[U52] PHP：箭头函数
来源：http://lms.ivvv.top

$double = fn($x) => $x * 2;
来源：http://xxr.fanxiaobao.xyz

[U53] PHP：空合并运算符
来源：http://ywg.shanyushiyangtech.top

$v = $a ?? $b ?? "default";
来源：http://sfi.shanyushiyangtech.top

[U54] PHP：空安全调用
来源：http://qap.xuanzx.com

$obj?->method()
来源：http://kua.xziqi.cn

[U55] PHP：match 表达式
来源：http://gzk.jinqigfzy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jjk.ybcxt.top

[U56] PHP：命名参数
来源：http://muy.yongpay.top

f(a: 1, b: 2)
来源：http://ytk.gotoacloud.top

[U57] PHP：字符串插值
来源：http://rfh.iojbl.cn

"值: {$a}"
来源：http://jyz.sysykeji.top

[U58] PHP：数组三件套
来源：http://ski.jinghuilouyu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gvs.zhongyouzk.top

[U59] PHP：自定义排序
来源：http://pmq.smart0.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pyv.jinyuanbaomall.cn

[U60] PHP：JSON 编解码
来源：http://utu.cqqwz.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gua.cqqwz.cn

[U61] PHP：正则
来源：http://vlk.zhengqikj.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gqq.sweek.top

[U62] PHP：日期对象
来源：http://dmq.c1oappe.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gji.gogol.net.cn

[U63] PHP：文件读写
来源：http://flx.tanke756.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gnn.fehbvm.com

[U64] PHP：目录遍历
来源：http://iha.xuetiantiany.cn

glob("dir/*.php");  scandir("dir");
来源：http://ggc.shzxlz.cn

[U65] PHP：会话
来源：http://wko.vehdjk.com

session_start();  $_SESSION["uid"] = 1;
来源：http://aqz.xingfuxueyuan.xyz

[U66] PHP：设置 Cookie
来源：http://rcq.jlsjyb.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ppt.ydjk.org.cn


<!-- 参考信息 -->