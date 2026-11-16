代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mro.jinqigfzy.top

[S21] C：字符类别判断
来源：http://wwf.mhx1999.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rmz.fzhhl.top

[S22] C：字符串转数字
来源：http://ehh.ydzc1.top

atoi("42");  strtod("3.14", NULL);
来源：http://gnj.daxiang520.top

[S23] C：随机数
来源：http://ade.shuidangran.top

srand(time(NULL));  int r = rand() % 100;
来源：http://jzt.jinyuanbaomall.cn

[S24] C：获取本地时间
来源：http://ixb.shzxlz.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hnm.hongshengwenyu.top

[S25] C：内存拷贝
来源：http://ltz.jyoumei.cn

memcpy(dst, src, n);
来源：http://vli.yuanzhike.top

[S26] C：内存清零
来源：http://wav.yj20258.top

memset(a, 0, sizeof a);
来源：http://bdx.smart0.xyz

[S27] C：定义常量
来源：http://cjf.gotoacloud.top

const double PI = 3.14159;
来源：http://bip.shzxlz.cn

[S28] C：静态变量
来源：http://iot.iojbl.cn

static int counter = 0;
来源：http://giy.zhengqikj.top

[S29] C：变参函数
来源：http://hdx.yvedp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dsd.hammf.cn

[S30] C：头文件保护
来源：http://znu.gotoacloud.top

#ifndef X_H
来源：http://fai.zycfv.cn

#define X_H
来源：http://mwg.aizwys.cn

#endif
来源：http://cdp.nanxuanxn.top

[S31] C++：Hello World
来源：http://wfj.zhiwuduotai.top

#include <iostream>
来源：http://bkh.cdnleiting.top

int main() { std::cout << "Hello\n"; }
来源：http://lhb.bjfxy.top

[S32] C++：字符串
来源：http://dmi.hywenlv.cn

std::string s = "hi";  s += "!";
来源：http://tok.hnqzz.top

[S33] C++：vector 增删
来源：http://ygb.nwbrower.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rhh.yj202588.top

[S34] C++：遍历 vector
来源：http://fzi.tian-w.cn

for (auto &x : v) { std::cout << x; }
来源：http://juj.xinyue.icu

[S35] C++：map
来源：http://tmv.wangshuangyany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://egn.fktsv.cn

[S36] C++：unordered_map
来源：http://upv.pycfn.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bbs.wangshuangyany.cn

[S37] C++：set
来源：http://gbe.bjfxy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zwk.aizwys.cn

[S38] C++：排序
来源：http://lis.c1oappe.top

std::sort(v.begin(), v.end());
来源：http://kfc.haohaochexian.top

[S39] C++：自定义比较器排序
来源：http://opu.yonumen.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://och.birdmap.top

[S40] C++：查找元素
来源：http://cjn.birdmap.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qdj.yonumen.top

[S41] C++：类与构造函数
来源：http://cbv.vehdjk.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tft.xuanzx.com

[S42] C++：继承与虚函数
来源：http://pmy.nanxinkj.top

class B : public Base { public: void f() override {} };
来源：http://ywl.chenlongwang.top

[S43] C++：智能指针
来源：http://ald.tarul.cn

auto p = std::make_unique<int>(5);
来源：http://jpc.aizwys.cn

[S44] C++：引用传参
来源：http://umj.tarul.cn

void inc(int &x) { ++x; }
来源：http://yaw.yuanzhike.top

[S45] C++：lambda
来源：http://vvd.epnwcf.com

auto add = [](int a, int b) { return a + b; };
来源：http://lpp.ctjpmb.com

[S46] C++：函数模板
来源：http://fjs.hysaishi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uqy.meibo888.top

[S47] C++：结构化绑定遍历
来源：http://gzk.yongpay.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://myq.fanxiaobao.xyz

[S48] C++：逐行读文件
来源：http://gqa.snrcjt.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pdj.pengpengdd.cyou

while (std::getline(in, line)) { }
来源：http://urq.ehwqpu.com

[S49] C++：写文件
来源：http://kke.vqdsnc.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lkm.quarkkingdee.top

[S50] C++：格式化数字
来源：http://lzc.zhiwuduotai.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nfs.yonumen.top

[S51] C++：显式类型转换
来源：http://ogr.gotoacloud.top

static_cast<double>(a) / b
来源：http://kyx.tianlin.xyz

[S52] C++：const 与 noexcept
来源：http://ccu.zhaomingkeji.xyz

int size() const noexcept { return n_; }
来源：http://rgs.0kj1m.cn

[S53] C++：移动语义
来源：http://oqe.tarul.cn

std::vector<int> w = std::move(v);
来源：http://mpb.zdbjq.cn

[S54] C++：异常处理
来源：http://emk.kuanghao11.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ljy.quarkkingdee.top

[S55] C++：结构化绑定
来源：http://bqa.zhijiandao.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mky.tanke756.top

[S56] C++：optional
来源：http://zdp.vqdsnc.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hjv.jinyuanbaomall.cn

[S57] C++：编译期常量
来源：http://yia.xuetiantiany.cn

constexpr int N = 10;
来源：http://plk.yongpay.top

[S58] C++：命名空间
来源：http://cqg.yuxming.cn

namespace ns { int f() { return 1; } }
来源：http://zlq.yuanzhike.top

[S59] C++：静态断言
来源：http://imj.cashguo.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fem.vqdsnc.cn

[S60] C++：遍历并删除元素
来源：http://kqg.zhiwuduotai.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ipp.ybcxt.top

================================================================================
来源：http://mql.tanke756.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hoa.nanxinkj.top

================================================================================
来源：http://muo.redwolf501.top

[T01] Kotlin：Hello World
来源：http://che.andypj.xyz

println("Hello")
来源：http://obm.yuanzhike.top

[T02] Kotlin：变量
来源：http://dzj.cheryme.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rrv.c1oappe.top

[T03] Kotlin：字符串模板
来源：http://yvj.jianghu66.top

"值: $b"
来源：http://ufr.yj20258.top

[T04] Kotlin：空安全
来源：http://hzo.jqgufenzy.top

val n: String? = null;  n?.length
来源：http://wvm.nwbrower.top

[T05] Kotlin：when 表达式
来源：http://uwa.zhijiandao.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gdi.c1oappe.top

[T06] Kotlin：集合映射
来源：http://eao.pycfn.com

listOf(1, 2, 3).map { it * 2 }
来源：http://uli.yangfankeji.com

[T07] Kotlin：集合过滤
来源：http://mru.kuanghao11.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hke.yonumen.top

[T08] Kotlin：数据类
来源：http://jwm.dashuyun.cn

data class User(val name: String, val age: Int)
来源：http://yai.xylfe.cn

[T09] Kotlin：扩展函数
来源：http://tll.iojbl.cn

fun String.exclaim() = this + "!"
来源：http://dbw.vehdjk.com

[T10] Kotlin：默认参数
来源：http://uro.svipenyu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ojv.vqdsnc.cn

[T11] Kotlin：协程
来源：http://kok.svipenyu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qtt.hfpthk.cn

[T12] Kotlin：解构声明
来源：http://rwf.xingfuxueyuan.xyz

val (a, b) = Pair(1, 2)
来源：http://wib.yuanzhike.top

[T13] Kotlin：只读 Map
来源：http://mqh.sufxvd.cn

val m = mapOf("a" to 1)
来源：http://uzt.tian-w.cn

[T14] Kotlin：循环
来源：http://uyn.nwbrower.top

for (i in 1..10) println(i)
来源：http://fqj.dashuyun.cn

[T15] Kotlin：接口
来源：http://uaz.shangyingyoupin.top

interface Shape { fun area(): Double }
来源：http://ogw.gzhubu.top

[T16] Swift：Hello World
来源：http://iwp.fktsv.cn

print("Hello")
来源：http://uku.vehdjk.com

[T17] Swift：变量与常量
来源：http://hiq.smart0.xyz

var a = 1;  let b = 2
来源：http://rlv.quarkkingdee.top

[T18] Swift：字符串插值
来源：http://age.ydzc1.top

"值: \(b)"
来源：http://hwf.iojbl.cn

[T19] Swift：可选绑定
来源：http://izq.dianchejie.cn

if let n = opt { print(n) }
来源：http://xsk.jinqigufen.top

[T20] Swift：数组操作
来源：http://opc.nwbrower.top

var a = [1, 2, 3];  a.append(4)
来源：http://mvq.cdnleiting.top

[T21] Swift：遍历
来源：http://zxy.zhixingplan.top

for x in a { print(x) }
来源：http://jjo.nanxinkj.top

[T22] Swift：字典
来源：http://kjj.uphjek.com

var d = ["a": 1];  d["b"] = 2
来源：http://qya.jinghuilouyu.cn

[T23] Swift：函数
来源：http://exe.nanxuanxn.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vbb.vqdsnc.cn

[T24] Swift：闭包
来源：http://ohr.zhixingplan.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://eik.jinghuilouyu.cn

[T25] Swift：结构体
来源：http://dfc.hnxiangtu.top

struct P { var x: Int }
来源：http://fnf.zycfv.cn

[T26] Swift：类与重写
来源：http://lte.zhaomingkeji.xyz

class A: Base { override func f() {} }
来源：http://znx.0kj1m.cn

[T27] Swift：错误处理
来源：http://onz.bjfxy.top

do { try f() } catch { print(error) }
来源：http://oic.tian-w.cn

[T28] Swift：枚举
来源：http://mli.xuanzx.com

enum Color { case red, green }
来源：http://upv.havefunace.top

[T29] Swift：guard 提前返回
来源：http://ygw.jqgufenzy.top

guard let x = opt else { return }
来源：http://nzk.zdbjq.cn

[T30] Swift：协议
来源：http://njl.pengpengdd.cyou

protocol Shape { func area() -> Double }
来源：http://bub.c1oappe.top

[T31] Lua：Hello World
来源：http://zcp.cucudq.cn

print("Hello")
来源：http://tiy.bbcook.cn

[T32] Lua：局部变量
来源：http://gmt.cqqwz.cn

local a = 1
来源：http://zfp.nwbrower.top

[T33] Lua：表（数组）
来源：http://ghg.jiagoushi.top

local t = {1, 2, 3};  t[4] = 4
来源：http://idg.jiagoushi.top

[T34] Lua：遍历表
来源：http://ohs.quarkkingdee.top

for i, v in ipairs(t) do print(i, v) end
来源：http://uul.yongpay.top

[T35] Lua：字典表
来源：http://cbz.tanke756.top

local d = { a = 1 };  d.b = 2
来源：http://lut.gogol.net.cn

[T36] Lua：函数
来源：http://rgl.andypj.xyz

function add(a, b) return a + b end
来源：http://gre.wangshuangyany.cn

[T37] Lua：字符串拼接
来源：http://woq.xziqi.cn

"a" .. "b"
来源：http://ynv.gotoacloud.top

[T38] Lua：条件
来源：http://iiz.svipenyu.cn

if x > 0 then print("正") end
来源：http://opk.shzxlz.cn

[T39] Lua：模式匹配
来源：http://sjq.aizwys.cn

string.find(s, "%d+")
来源：http://mjx.sysykeji.top

[T40] Lua：元表
来源：http://ttu.xuetiantiany.cn

setmetatable({}, { __index = base })
来源：http://lfm.shanyushiyangkeji.top

[T41] Perl：Hello World
来源：http://zaz.zycfv.cn

print "Hello\n";
来源：http://uuh.yvedp.cn

[T42] Perl：变量类型
来源：http://lgy.chenlongwang.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://anb.316326.xyz

[T43] Perl：字符串插值
来源：http://elg.redwolf501.top

"值: $a"
来源：http://bod.zhongyouzk.top

[T44] Perl：条件
来源：http://kje.jqgfzy.top

if ($a > 0) { print "正"; }
来源：http://nzk.ehwqpu.com

[T45] Perl：数组遍历
来源：http://fii.316326.xyz

for my $x (@arr) { print $x; }
来源：http://wxw.chenzaomai.com

[T46] Perl：哈希操作
来源：http://drg.fengsongda.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kxf.sysykeji.top

[T47] Perl：正则捕获
来源：http://lry.fzhhl.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://qcg.fanxiaobao.xyz

[T48] Perl：正则替换
来源：http://yts.fehbvm.com

$s =~ s/old/new/g;
来源：http://jed.zdbjq.cn

[T49] Perl：函数
来源：http://kwk.fktsv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mvk.sysykeji.top

[T50] Perl：逐行读文件
来源：http://mke.fengsongda.top

open my $fh, "<", "a.txt" or die $!;
来源：http://pva.jlsjyb.cn

while (my $line = <$fh>) { print $line; }
来源：http://xyj.fehbvm.com

[T51] Scala：Hello World
来源：http://hcb.yuxming.cn

println("Hello")
来源：http://zcx.hammf.cn

[T52] Scala：变量
来源：http://kmr.52xcode.cn

val a = 1;  var b = 2
来源：http://kqk.yueranfly.top

[T53] Scala：字符串插值
来源：http://edv.epnwcf.com

s"值: $b"
来源：http://mmc.aibaodan.cn

[T54] Scala：集合映射
来源：http://mit.yj20258.top

List(1, 2, 3).map(_ * 2)
来源：http://yzc.zhixingplan.top

[T55] Scala：集合过滤
来源：http://cqq.sjlbkw.cn

List(1, 2, 3).filter(_ > 1)
来源：http://arx.jqgfzy.top

[T56] Scala：样例类
来源：http://zoq.yongpay.top

case class User(name: String, age: Int)
来源：http://bsb.epnwcf.com

[T57] Scala：模式匹配
来源：http://bnq.vqdsnc.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://aad.nanxinkj.top

[T58] Scala：函数定义
来源：http://tky.snrcjt.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tnd.zdqjudy.top

[T59] Scala：循环
来源：http://xqb.hywenlv.cn

for (i <- 1 to 10) println(i)
来源：http://axu.svipenyu.cn

[T60] Scala：折叠
来源：http://tfr.hfpthk.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tex.guannengcc.top

================================================================================
来源：http://kjr.ehwqpu.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bsd.chenjidiqi.icu

================================================================================
来源：http://zcr.mhx1999.top

[U01] Py：创建虚拟环境
来源：http://err.epnwcf.com

python -m venv .venv && source .venv/bin/activate
来源：http://trv.bbcook.cn

[U02] Py：导出 / 安装依赖
来源：http://gnp.xuetiantiany.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qwf.feifeiyinyue.top

[U03] Py：加载 .env 配置
来源：http://hqd.hfpthk.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://iqc.vehdjk.com

[U04] Py：变量调试打印
来源：http://ylc.iojbl.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lyv.jiagoushi.top

[U05] Py：列表去重且保序
来源：http://jxu.fehbvm.com

list(dict.fromkeys(arr))
来源：http://sis.chenjidiqi.icu

[U06] Py：合并两个字典
来源：http://lzg.daxiang520.top

{**a, **b}
来源：http://phb.yueranfly.top

[U07] Py：反转字典键值
来源：http://ghu.fengsongda.top

{v: k for k, v in d.items()}
来源：http://jjx.yj202588.top

[U08] Py：展平二维列表
来源：http://ewc.pengpengdd.cyou

[y for x in nested for y in x]
来源：http://fdr.jinyuanbaomall.cn

[U09] Py：字典取最大值的键
来源：http://msz.vehdjk.com

max(d, key=d.get)
来源：http://ekn.wangshuangyany.cn

[U10] Py：按值排序字典
来源：http://yqh.yonumen.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ekc.epnwcf.com

[U11] Py：生成器表达式
来源：http://sut.zhijiandao.cn

(x * 2 for x in arr)
来源：http://cfp.bjfxy.top

[U12] Py：取出现最多的 3 个元素
来源：http://vpk.jqgufenzy.top

Counter(arr).most_common(3)
来源：http://wgk.tanke756.top

[U13] Py：固定长度队列
来源：http://ccw.jyoumei.cn

deque(maxlen=10)
来源：http://uti.tarul.cn

[U14] Py：分组收集到列表
来源：http://pwf.vqdsnc.cn

defaultdict(list)
来源：http://mcl.sweek.top

[U15] Py：高精度计时
来源：http://vtc.cqqwz.cn

t = time.perf_counter()
来源：http://imx.tarul.cn

[U16] Py：命令行参数解析
来源：http://cvx.tianlin.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fti.zhixingplan.top

[U17] Py：初始化日志
来源：http://dyy.quarkkingdee.top

logging.basicConfig(level=logging.INFO)
来源：http://hid.yongpay.top

[U18] Py：预编译正则
来源：http://piy.guannengcc.top

pat = re.compile(r"\d+")
来源：http://rkf.jinghuilouyu.cn

[U19] Py：正则替换带回调
来源：http://oby.fktsv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jtm.hammf.cn

[U20] Py：缓存函数结果
来源：http://idy.guannengcc.top

@functools.lru_cache(maxsize=None)
来源：http://zug.hfpthk.cn

[U21] Py：自定义上下文管理器
来源：http://ohk.0kj1m.cn

@contextlib.contextmanager
来源：http://qgq.jinqigufen.top

[U22] Py：矩阵转置
来源：http://znv.cucudq.cn

list(zip(*m))
来源：http://lts.gzhubu.top

[U23] Py：分块读取大文件
来源：http://ziq.pycfn.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tiy.zycfv.cn

[U24] Py：路径操作
来源：http://vlw.sxryk.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://oqz.hnxiangtu.top

[U25] Py：CSV 按字典读
来源：http://xol.ivvv.top

csv.DictReader(f)
来源：http://mys.hnxiangtu.top

[U26] Py：并发下载
来源：http://zlm.havefunace.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://miq.hysaishi.cn

[U27] Py：异步 HTTP
来源：http://aqt.ybcxt.top

aiohttp.ClientSession() 配合 async with
来源：http://fcm.zhaomingkeji.xyz

[U28] Py：类型别名
来源：http://isa.zhijiandao.cn

UserId = int
来源：http://tbx.nanxinkj.top

[U29] Py：属性校验
来源：http://nwb.hysaishi.cn

@property 与 @x.setter 配合
来源：http://apx.zhongyouzk.top

[U30] Py：数据类
来源：http://itk.feifeiyinyue.top

@dataclass(slots=True)
来源：http://way.svipenyu.cn

[U31] Py：单测
来源：http://sry.xinyue.icu

python -m pytest -q
来源：http://faj.bjfxy.top

[U32] Py：代码格式化
来源：http://tvl.haohaochexian.top

ruff format . && ruff check --fix .
来源：http://rel.snrcjt.cn

[U33] Py：打包发布
来源：http://jzt.316326.xyz

python -m build  （依赖 pyproject.toml）
来源：http://bbw.jlsjyb.cn

[U34] Py：判断编码
来源：http://yrf.yj20258.top

chardet.detect(raw)
来源：http://uye.yvedp.cn

[U35] Py：发送邮件
来源：http://fxr.guannengcc.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://owp.zdbjq.cn

[U36] Py：定时任务
来源：http://fti.yfazqb.com

schedule.every(10).minutes.do(job)
来源：http://hff.cashguo.top

[U37] Py：读写 Excel
来源：http://qxd.guowangkeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://qei.daria6918.cn

[U38] Py：获取脚本所在目录
来源：http://wta.chenlongwang.top

Path(__file__).resolve().parent
来源：http://oki.sufxvd.cn

[U39] Py：判断是否在交互环境
来源：http://pjp.pycfn.com

sys.stdout.isatty()
来源：http://jgo.yuanzhike.top

[U40] Py：打印到标准错误
来源：http://rfa.yueranfly.top

print("err", file=sys.stderr)
来源：http://mxs.haohaochexian.top

[U41] PHP：初始化 Composer 项目
来源：http://rhy.shuidangran.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ldn.vehdjk.com

[U42] PHP：PSR-4 自动加载
来源：http://bzj.ybcxt.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://chj.sweek.top

[U43] PHP：声明命名空间
来源：http://cti.hammf.cn

namespace App\Http;
来源：http://qcb.hnxiangtu.top

[U44] PHP：开启严格类型
来源：http://xmz.zhixingplan.top

declare(strict_types=1);
来源：http://vpt.havefunace.top


<!-- 参考信息 -->