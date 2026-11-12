代发 wailian999

x |= (1 << 3);
来源：http://bcz.ydjk.org.cn

[S17] C：安全拼接字符串
来源：http://fyg.zdqjudy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pju.shanyushiyangkeji.top

[S18] C：命令行参数
来源：http://vzc.shanyushiyangtech.top

int main(int argc, char **argv)
来源：http://wwa.birdmap.top

[S19] C：快速排序
来源：http://sch.cucudq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hkq.hammf.cn

[S20] C：二分查找
来源：http://ntl.ehwqpu.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qoh.ppjwa.cn

[S21] C：字符类别判断
来源：http://yab.tanke756.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jug.zhengqikj.top

[S22] C：字符串转数字
来源：http://mmu.vqdsnc.cn

atoi("42");  strtod("3.14", NULL);
来源：http://eew.shzxlz.cn

[S23] C：随机数
来源：http://aaz.yuxming.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://iik.nwbrower.top

[S24] C：获取本地时间
来源：http://gnu.zdqjudy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tie.zdqjudy.top

[S25] C：内存拷贝
来源：http://crb.tianlin.xyz

memcpy(dst, src, n);
来源：http://itx.hammf.cn

[S26] C：内存清零
来源：http://mwe.guannengcc.top

memset(a, 0, sizeof a);
来源：http://pvw.jinqigfzy.top

[S27] C：定义常量
来源：http://dgf.c1oappe.top

const double PI = 3.14159;
来源：http://wvl.hnqzz.top

[S28] C：静态变量
来源：http://nye.zhaomingkeji.xyz

static int counter = 0;
来源：http://jtj.jianghu66.top

[S29] C：变参函数
来源：http://coq.52xcode.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qsg.xuanzx.com

[S30] C：头文件保护
来源：http://bmy.xziqi.cn

#ifndef X_H
来源：http://bqw.havefunace.top

#define X_H
来源：http://ota.tarul.cn

#endif
来源：http://znx.hcnkem.com

[S31] C++：Hello World
来源：http://nwq.feifeiyinyue.top

#include <iostream>
来源：http://kgq.yuxming.cn

int main() { std::cout << "Hello\n"; }
来源：http://dwl.chenjidiqi.icu

[S32] C++：字符串
来源：http://seg.fktsv.cn

std::string s = "hi";  s += "!";
来源：http://vnw.yuanzhike.top

[S33] C++：vector 增删
来源：http://gya.ybcxt.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zcn.yj20258.top

[S34] C++：遍历 vector
来源：http://gnq.ehwqpu.com

for (auto &x : v) { std::cout << x; }
来源：http://gjj.ivvv.top

[S35] C++：map
来源：http://wiu.sufxvd.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://akp.ctjpmb.com

[S36] C++：unordered_map
来源：http://zxu.meibo888.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ggk.iojbl.cn

[S37] C++：set
来源：http://kfr.hfpthk.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://btq.daxiang520.top

[S38] C++：排序
来源：http://ifm.zhixingplan.top

std::sort(v.begin(), v.end());
来源：http://wmk.jinghuilouyu.cn

[S39] C++：自定义比较器排序
来源：http://lir.hesvh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mjg.quarkkingdee.top

[S40] C++：查找元素
来源：http://fvm.yonumen.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://knz.cheryme.top

[S41] C++：类与构造函数
来源：http://xgd.aibaodan.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ocd.havefunace.top

[S42] C++：继承与虚函数
来源：http://qdl.sysykeji.top

class B : public Base { public: void f() override {} };
来源：http://ecw.xziqi.cn

[S43] C++：智能指针
来源：http://afz.shanyushiyangtech.top

auto p = std::make_unique<int>(5);
来源：http://bgg.zhiwuduotai.top

[S44] C++：引用传参
来源：http://ijz.fehbvm.com

void inc(int &x) { ++x; }
来源：http://rpo.cdnleiting.top

[S45] C++：lambda
来源：http://xnk.birdmap.top

auto add = [](int a, int b) { return a + b; };
来源：http://bir.hesvh.cn

[S46] C++：函数模板
来源：http://zrt.zhongyouzk.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sxe.hywenlv.cn

[S47] C++：结构化绑定遍历
来源：http://tfz.nwbrower.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://spp.shuidangran.top

[S48] C++：逐行读文件
来源：http://iwq.yfazqb.com

std::ifstream in("a.txt");  std::string line;
来源：http://lac.gzhubu.top

while (std::getline(in, line)) { }
来源：http://fjb.epnwcf.com

[S49] C++：写文件
来源：http://nwn.gogol.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kra.snrcjt.cn

[S50] C++：格式化数字
来源：http://pxe.jianghu66.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ewq.ehwqpu.com

[S51] C++：显式类型转换
来源：http://pgu.cheryme.top

static_cast<double>(a) / b
来源：http://jkx.zhaomingkeji.xyz

[S52] C++：const 与 noexcept
来源：http://rhg.ydzc1.top

int size() const noexcept { return n_; }
来源：http://mly.zhixingplan.top

[S53] C++：移动语义
来源：http://wxe.jlsjyb.cn

std::vector<int> w = std::move(v);
来源：http://eqr.nanxinkj.top

[S54] C++：异常处理
来源：http://sgf.gogol.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jix.chenzaomai.com

[S55] C++：结构化绑定
来源：http://hiq.cqqwz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dmx.nanxuanxn.top

[S56] C++：optional
来源：http://wed.kuanghao11.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ulk.zhixingplan.top

[S57] C++：编译期常量
来源：http://ofr.0kj1m.cn

constexpr int N = 10;
来源：http://sab.jinqigufen.top

[S58] C++：命名空间
来源：http://cmd.fehbvm.com

namespace ns { int f() { return 1; } }
来源：http://uxl.daria6918.cn

[S59] C++：静态断言
来源：http://kbd.sjlbkw.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jfy.nanxuanxn.top

[S60] C++：遍历并删除元素
来源：http://lqd.fehbvm.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jle.fengsongda.top

================================================================================
来源：http://vsv.cheryme.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wcf.0kj1m.cn

================================================================================
来源：http://zav.redwolf501.top

[T01] Kotlin：Hello World
来源：http://afc.nanxuanxn.top

println("Hello")
来源：http://cse.fengsongda.top

[T02] Kotlin：变量
来源：http://esr.havefunace.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://efu.shanyushiyangkeji.top

[T03] Kotlin：字符串模板
来源：http://wmt.9152youxi.cn

"值: $b"
来源：http://ota.zhixingplan.top

[T04] Kotlin：空安全
来源：http://prk.kuanghao11.cn

val n: String? = null;  n?.length
来源：http://lix.cqqwz.cn

[T05] Kotlin：when 表达式
来源：http://bnp.nanxinkj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fwa.ctjpmb.com

[T06] Kotlin：集合映射
来源：http://kfv.xinyue.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://lcd.tarul.cn

[T07] Kotlin：集合过滤
来源：http://sxb.dashuyun.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ukt.hammf.cn

[T08] Kotlin：数据类
来源：http://jpu.jinyuanbaomall.cn

data class User(val name: String, val age: Int)
来源：http://eol.snrcjt.cn

[T09] Kotlin：扩展函数
来源：http://mip.shzxlz.cn

fun String.exclaim() = this + "!"
来源：http://kyv.zhoulong.xyz

[T10] Kotlin：默认参数
来源：http://pdr.guannengcc.top

fun greet(name: String = "World") = "Hi $name"
来源：http://cut.zhiwuduotai.top

[T11] Kotlin：协程
来源：http://cet.smart0.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://jil.cheryme.top

[T12] Kotlin：解构声明
来源：http://jyc.pycfn.com

val (a, b) = Pair(1, 2)
来源：http://hhp.yfazqb.com

[T13] Kotlin：只读 Map
来源：http://hna.bjfxy.top

val m = mapOf("a" to 1)
来源：http://tnl.sysykeji.top

[T14] Kotlin：循环
来源：http://sbf.zdbjq.cn

for (i in 1..10) println(i)
来源：http://ukv.52xcode.cn

[T15] Kotlin：接口
来源：http://mbd.tian-w.cn

interface Shape { fun area(): Double }
来源：http://myk.bjfxy.top

[T16] Swift：Hello World
来源：http://xaw.dianchejie.cn

print("Hello")
来源：http://zic.ydjk.org.cn

[T17] Swift：变量与常量
来源：http://ysj.hnqzz.top

var a = 1;  let b = 2
来源：http://lsq.hywenlv.cn

[T18] Swift：字符串插值
来源：http://myi.zhixingplan.top

"值: \(b)"
来源：http://rqx.yangfankeji.com

[T19] Swift：可选绑定
来源：http://rli.zhiwuduotai.top

if let n = opt { print(n) }
来源：http://mpt.xziqi.cn

[T20] Swift：数组操作
来源：http://kar.bjfxy.top

var a = [1, 2, 3];  a.append(4)
来源：http://aoj.zhaomingkeji.xyz

[T21] Swift：遍历
来源：http://kjh.xingfuxueyuan.xyz

for x in a { print(x) }
来源：http://hiz.gogol.net.cn

[T22] Swift：字典
来源：http://ali.aizwys.cn

var d = ["a": 1];  d["b"] = 2
来源：http://isc.meibo888.top

[T23] Swift：函数
来源：http://whd.zhoulong.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lql.meibo888.top

[T24] Swift：闭包
来源：http://itw.cqqwz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://brt.yuxming.cn

[T25] Swift：结构体
来源：http://njb.gzhubu.top

struct P { var x: Int }
来源：http://dnb.shzxlz.cn

[T26] Swift：类与重写
来源：http://cep.tanke756.top

class A: Base { override func f() {} }
来源：http://enp.zhixingplan.top

[T27] Swift：错误处理
来源：http://oeo.zhaomingkeji.xyz

do { try f() } catch { print(error) }
来源：http://wgm.52xcode.cn

[T28] Swift：枚举
来源：http://bcg.zhongyouzk.top

enum Color { case red, green }
来源：http://yfp.yj20258888.top

[T29] Swift：guard 提前返回
来源：http://kqh.xuetiantiany.cn

guard let x = opt else { return }
来源：http://dwh.ehwqpu.com

[T30] Swift：协议
来源：http://ovi.jyoumei.cn

protocol Shape { func area() -> Double }
来源：http://ijm.chenjidiqi.icu

[T31] Lua：Hello World
来源：http://mcc.hcnkem.com

print("Hello")
来源：http://qwa.hnxiangtu.top

[T32] Lua：局部变量
来源：http://sca.feifeiyinyue.top

local a = 1
来源：http://tgt.chenjidiqi.icu

[T33] Lua：表（数组）
来源：http://xti.yonumen.top

local t = {1, 2, 3};  t[4] = 4
来源：http://rus.iojbl.cn

[T34] Lua：遍历表
来源：http://syf.aizwys.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qkv.hesvh.cn

[T35] Lua：字典表
来源：http://bpr.svipenyu.cn

local d = { a = 1 };  d.b = 2
来源：http://mpe.ywan-chungtsiang.top

[T36] Lua：函数
来源：http://raf.yj202588.top

function add(a, b) return a + b end
来源：http://sbv.chenlongwang.top

[T37] Lua：字符串拼接
来源：http://web.fzhhl.top

"a" .. "b"
来源：http://elz.havefunace.top

[T38] Lua：条件
来源：http://yzp.yongpay.top

if x > 0 then print("正") end
来源：http://jxh.daxiang520.top

[T39] Lua：模式匹配
来源：http://pxi.316326.xyz

string.find(s, "%d+")
来源：http://peq.zhengqikj.top

[T40] Lua：元表
来源：http://bzr.iojbl.cn

setmetatable({}, { __index = base })
来源：http://riz.tarul.cn

[T41] Perl：Hello World
来源：http://hcy.uphjek.com

print "Hello\n";
来源：http://lmr.jiagoushi.top

[T42] Perl：变量类型
来源：http://tip.zdbjq.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qzg.daxiang520.top

[T43] Perl：字符串插值
来源：http://gwh.ybcxt.top

"值: $a"
来源：http://asq.yonumen.top

[T44] Perl：条件
来源：http://ezx.fehbvm.com

if ($a > 0) { print "正"; }
来源：http://czf.pengpengdd.cyou

[T45] Perl：数组遍历
来源：http://isk.yuxming.cn

for my $x (@arr) { print $x; }
来源：http://inb.hammf.cn

[T46] Perl：哈希操作
来源：http://vzi.hnqzz.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hkf.chenlongwang.top

[T47] Perl：正则捕获
来源：http://loj.shanyushiyangtech.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://dph.dianchejie.cn

[T48] Perl：正则替换
来源：http://cmn.nwbrower.top

$s =~ s/old/new/g;
来源：http://wgz.bbcook.cn

[T49] Perl：函数
来源：http://ogl.shuidangran.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mpt.wangshuangyany.cn

[T50] Perl：逐行读文件
来源：http://ovy.aibaodan.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://oui.nanxuanxn.top

while (my $line = <$fh>) { print $line; }
来源：http://xff.nanxinkj.top

[T51] Scala：Hello World
来源：http://vxu.cqqwz.cn

println("Hello")
来源：http://uwq.mhx1999.top

[T52] Scala：变量
来源：http://rvx.ywan-chungtsiang.top

val a = 1;  var b = 2
来源：http://bbo.vehdjk.com

[T53] Scala：字符串插值
来源：http://ezf.gzhubu.top

s"值: $b"
来源：http://iez.hammf.cn

[T54] Scala：集合映射
来源：http://ynn.feifeiyinyue.top

List(1, 2, 3).map(_ * 2)
来源：http://kqq.yangfankeji.com

[T55] Scala：集合过滤
来源：http://ixf.quarkkingdee.top

List(1, 2, 3).filter(_ > 1)
来源：http://byx.sweek.top

[T56] Scala：样例类
来源：http://bpu.dashuyun.cn

case class User(name: String, age: Int)
来源：http://gfs.yueranfly.top

[T57] Scala：模式匹配
来源：http://xwd.jianghu66.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://hxz.yvedp.cn

[T58] Scala：函数定义
来源：http://pvu.bjfxy.top

def add(a: Int, b: Int): Int = a + b
来源：http://mvq.dianchejie.cn

[T59] Scala：循环
来源：http://rln.bbcook.cn

for (i <- 1 to 10) println(i)
来源：http://xlo.sysykeji.top

[T60] Scala：折叠
来源：http://qcg.gzhubu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qla.jqgfzy.top

================================================================================
来源：http://mvl.xuanzx.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ejh.ywan-chungtsiang.top

================================================================================
来源：http://vjy.dianchejie.cn

[U01] Py：创建虚拟环境
来源：http://znk.zhiwuduotai.top

python -m venv .venv && source .venv/bin/activate
来源：http://ipj.ehwqpu.com

[U02] Py：导出 / 安装依赖
来源：http://qou.shangyingyoupin.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ujd.shanyushiyangkeji.top

[U03] Py：加载 .env 配置
来源：http://ejv.cheryme.top

from dotenv import load_dotenv; load_dotenv()
来源：http://eru.jinyuanbaomall.cn

[U04] Py：变量调试打印
来源：http://hfl.snrcjt.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nkl.gotoacloud.top

[U05] Py：列表去重且保序
来源：http://kfr.ydzc1.top

list(dict.fromkeys(arr))
来源：http://ldo.xuetiantiany.cn

[U06] Py：合并两个字典
来源：http://jrr.fzhhl.top

{**a, **b}
来源：http://qly.ivvv.top

[U07] Py：反转字典键值
来源：http://hdq.sjlbkw.cn

{v: k for k, v in d.items()}
来源：http://tia.zdqjudy.top

[U08] Py：展平二维列表
来源：http://hxm.nanxuanxn.top

[y for x in nested for y in x]
来源：http://jze.chenlongwang.top

[U09] Py：字典取最大值的键
来源：http://isr.zhixingplan.top

max(d, key=d.get)
来源：http://xad.bbcook.cn

[U10] Py：按值排序字典
来源：http://weh.birdmap.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fnd.jianghu66.top

[U11] Py：生成器表达式
来源：http://pdx.sxryk.cn

(x * 2 for x in arr)
来源：http://qsl.xziqi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://khn.cashguo.top

Counter(arr).most_common(3)
来源：http://uta.hongshengwenyu.top

[U13] Py：固定长度队列
来源：http://mqw.sufxvd.cn

deque(maxlen=10)
来源：http://uni.9152youxi.cn

[U14] Py：分组收集到列表
来源：http://pts.chenlongwang.top

defaultdict(list)
来源：http://cld.shzxlz.cn

[U15] Py：高精度计时
来源：http://jvw.meibo888.top

t = time.perf_counter()
来源：http://che.jiagoushi.top

[U16] Py：命令行参数解析
来源：http://the.fengsongda.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://iya.sysykeji.top

[U17] Py：初始化日志
来源：http://ley.jlsjyb.cn

logging.basicConfig(level=logging.INFO)
来源：http://ybo.xuetiantiany.cn

[U18] Py：预编译正则
来源：http://cqg.hnqzz.top

pat = re.compile(r"\d+")
来源：http://xlj.zdbjq.cn

[U19] Py：正则替换带回调
来源：http://tyw.fzhhl.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bnw.redwolf501.top

[U20] Py：缓存函数结果
来源：http://vrn.epnwcf.com

@functools.lru_cache(maxsize=None)
来源：http://iun.ehwqpu.com

[U21] Py：自定义上下文管理器
来源：http://spp.nanxinkj.top

@contextlib.contextmanager
来源：http://ekp.hnqzz.top

[U22] Py：矩阵转置
来源：http://qmt.fzhhl.top

list(zip(*m))
来源：http://ulb.haohaochexian.top

[U23] Py：分块读取大文件
来源：http://ttg.ppjwa.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jkd.shzxlz.cn

[U24] Py：路径操作
来源：http://knz.xuanzx.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pew.sxryk.cn

[U25] Py：CSV 按字典读
来源：http://lsr.dianchejie.cn

csv.DictReader(f)
来源：http://anq.vehdjk.com

[U26] Py：并发下载
来源：http://rqx.jqgfzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ntu.fzhhl.top

[U27] Py：异步 HTTP
来源：http://xzw.gogol.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://ali.zhijiandao.cn

[U28] Py：类型别名
来源：http://lxn.zdbjq.cn

UserId = int
来源：http://jjh.cdnleiting.top

[U29] Py：属性校验
来源：http://ktc.52xcode.cn

@property 与 @x.setter 配合
来源：http://mha.uphjek.com

[U30] Py：数据类
来源：http://zyt.cqqwz.cn

@dataclass(slots=True)
来源：http://jrb.nanxuanxn.top

[U31] Py：单测
来源：http://oee.fktsv.cn

python -m pytest -q
来源：http://bym.sjlbkw.cn

[U32] Py：代码格式化
来源：http://izn.cucudq.cn

ruff format . && ruff check --fix .
来源：http://cgm.shzxlz.cn

[U33] Py：打包发布
来源：http://kqr.zhijiandao.cn

python -m build  （依赖 pyproject.toml）
来源：http://efy.chenjidiqi.icu

[U34] Py：判断编码
来源：http://rqf.hnxiangtu.top

chardet.detect(raw)
来源：http://vxs.zhoulong.xyz

[U35] Py：发送邮件
来源：http://xoy.wangdashe.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mhl.316326.xyz

[U36] Py：定时任务
来源：http://gyc.bjfxy.top

schedule.every(10).minutes.do(job)
来源：http://kur.jqgufenzy.top

[U37] Py：读写 Excel
来源：http://wak.sysykeji.top

pandas.read_excel / DataFrame.to_excel
来源：http://pna.zhoulong.xyz

[U38] Py：获取脚本所在目录
来源：http://aon.aibaodan.cn

Path(__file__).resolve().parent
来源：http://nwf.zdbjq.cn

[U39] Py：判断是否在交互环境
来源：http://pgi.jlsjyb.cn

sys.stdout.isatty()
来源：http://fwq.ydjk.org.cn

[U40] Py：打印到标准错误
来源：http://yun.redwolf501.top

print("err", file=sys.stderr)
来源：http://log.hcnkem.com


<!-- 参考信息 -->