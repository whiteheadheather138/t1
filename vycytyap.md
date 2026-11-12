代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://kps.fehbvm.com

[S15] C：类型转换
来源：http://hsa.yfazqb.com

(double) a / b
来源：http://exq.smart0.xyz

[S16] C：位操作置位
来源：http://uui.xingfuxueyuan.xyz

x |= (1 << 3);
来源：http://yev.hammf.cn

[S17] C：安全拼接字符串
来源：http://mhy.bjfxy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hmh.jinqigufen.top

[S18] C：命令行参数
来源：http://jws.daria6918.cn

int main(int argc, char **argv)
来源：http://oct.xuanzx.com

[S19] C：快速排序
来源：http://bdk.jqgufenzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://ker.jinghuilouyu.cn

[S20] C：二分查找
来源：http://kjg.jinghuilouyu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ezm.yonumen.top

[S21] C：字符类别判断
来源：http://nyu.redwolf501.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://avs.c1oappe.top

[S22] C：字符串转数字
来源：http://jzt.0kj1m.cn

atoi("42");  strtod("3.14", NULL);
来源：http://iur.yvedp.cn

[S23] C：随机数
来源：http://xwu.ybcxt.top

srand(time(NULL));  int r = rand() % 100;
来源：http://zty.tian-w.cn

[S24] C：获取本地时间
来源：http://aai.ehwqpu.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xrd.zdbjq.cn

[S25] C：内存拷贝
来源：http://mkl.wangshuangyany.cn

memcpy(dst, src, n);
来源：http://kya.zhiwuduotai.top

[S26] C：内存清零
来源：http://poa.snrcjt.cn

memset(a, 0, sizeof a);
来源：http://kik.sweek.top

[S27] C：定义常量
来源：http://azw.hesvh.cn

const double PI = 3.14159;
来源：http://fmm.zhongyouzk.top

[S28] C：静态变量
来源：http://qzp.yfazqb.com

static int counter = 0;
来源：http://yaa.sufxvd.cn

[S29] C：变参函数
来源：http://myr.sjlbkw.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ozd.cqqwz.cn

[S30] C：头文件保护
来源：http://zwp.sjlbkw.cn

#ifndef X_H
来源：http://ymt.yanxiufei.cn

#define X_H
来源：http://gcx.zdbjq.cn

#endif
来源：http://ovh.yj202588.top

[S31] C++：Hello World
来源：http://mlu.ivvv.top

#include <iostream>
来源：http://cku.gogol.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://nlg.daria6918.cn

[S32] C++：字符串
来源：http://bbd.ywan-chungtsiang.top

std::string s = "hi";  s += "!";
来源：http://paf.havefunace.top

[S33] C++：vector 增删
来源：http://yei.xingfuxueyuan.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rba.hnqzz.top

[S34] C++：遍历 vector
来源：http://opr.ivvv.top

for (auto &x : v) { std::cout << x; }
来源：http://bqz.nwbrower.top

[S35] C++：map
来源：http://wnd.ybcxt.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pci.tanke756.top

[S36] C++：unordered_map
来源：http://gzv.gogol.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zme.pycfn.com

[S37] C++：set
来源：http://fle.nanxinkj.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zua.hnxiangtu.top

[S38] C++：排序
来源：http://epg.xylfe.cn

std::sort(v.begin(), v.end());
来源：http://icw.hammf.cn

[S39] C++：自定义比较器排序
来源：http://wcs.jiagoushi.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mdg.iojbl.cn

[S40] C++：查找元素
来源：http://ehy.9152youxi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ygi.wangdashe.top

[S41] C++：类与构造函数
来源：http://aiu.sysykeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xkp.zdqjudy.top

[S42] C++：继承与虚函数
来源：http://lib.xylfe.cn

class B : public Base { public: void f() override {} };
来源：http://iqe.shuidangran.top

[S43] C++：智能指针
来源：http://mpq.andypj.xyz

auto p = std::make_unique<int>(5);
来源：http://rwo.aibaodan.cn

[S44] C++：引用传参
来源：http://dkj.sysykeji.top

void inc(int &x) { ++x; }
来源：http://clr.guowangkeji.top

[S45] C++：lambda
来源：http://sjz.chenzaomai.com

auto add = [](int a, int b) { return a + b; };
来源：http://dxu.gotoacloud.top

[S46] C++：函数模板
来源：http://mfo.chenzaomai.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://opf.jyoumei.cn

[S47] C++：结构化绑定遍历
来源：http://yak.ydzc1.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hxh.sxryk.cn

[S48] C++：逐行读文件
来源：http://guu.9152youxi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gaf.yanxiufei.cn

while (std::getline(in, line)) { }
来源：http://unb.yj20258888.top

[S49] C++：写文件
来源：http://lpn.dianchejie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://twp.smart0.xyz

[S50] C++：格式化数字
来源：http://nha.yuanzhike.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kxx.xuetiantiany.cn

[S51] C++：显式类型转换
来源：http://npl.dianchejie.cn

static_cast<double>(a) / b
来源：http://kzl.xylfe.cn

[S52] C++：const 与 noexcept
来源：http://uvc.yvedp.cn

int size() const noexcept { return n_; }
来源：http://bhe.sweek.top

[S53] C++：移动语义
来源：http://hne.nanxinkj.top

std::vector<int> w = std::move(v);
来源：http://ybm.jiagoushi.top

[S54] C++：异常处理
来源：http://knr.tanke756.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yqz.xziqi.cn

[S55] C++：结构化绑定
来源：http://die.shuidangran.top

auto [a, b] = std::make_pair(1, 2);
来源：http://pyi.xylfe.cn

[S56] C++：optional
来源：http://uzk.cqqwz.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cpl.yj202588.top

[S57] C++：编译期常量
来源：http://awz.sjlbkw.cn

constexpr int N = 10;
来源：http://hhh.vqdsnc.cn

[S58] C++：命名空间
来源：http://zsq.shuidangran.top

namespace ns { int f() { return 1; } }
来源：http://djr.feifeiyinyue.top

[S59] C++：静态断言
来源：http://ykf.hysaishi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cfu.wangshuangyany.cn

[S60] C++：遍历并删除元素
来源：http://dvb.gzhubu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mpl.ywan-chungtsiang.top

================================================================================
来源：http://fqx.sxryk.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oap.c1oappe.top

================================================================================
来源：http://zwl.snrcjt.cn

[T01] Kotlin：Hello World
来源：http://byw.yuanzhike.top

println("Hello")
来源：http://ogp.shzxlz.cn

[T02] Kotlin：变量
来源：http://cfq.yonumen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wki.aibaodan.cn

[T03] Kotlin：字符串模板
来源：http://lqo.xinyue.icu

"值: $b"
来源：http://fwc.shuidangran.top

[T04] Kotlin：空安全
来源：http://doo.nanxinkj.top

val n: String? = null;  n?.length
来源：http://prw.cqqwz.cn

[T05] Kotlin：when 表达式
来源：http://naj.nanxuanxn.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gme.chenlongwang.top

[T06] Kotlin：集合映射
来源：http://gid.xingfuxueyuan.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://zsj.sysykeji.top

[T07] Kotlin：集合过滤
来源：http://skm.316326.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://oxu.jinyuanbaomall.cn

[T08] Kotlin：数据类
来源：http://aop.sufxvd.cn

data class User(val name: String, val age: Int)
来源：http://leg.yangfankeji.com

[T09] Kotlin：扩展函数
来源：http://ptd.jqgfzy.top

fun String.exclaim() = this + "!"
来源：http://ymt.zdbjq.cn

[T10] Kotlin：默认参数
来源：http://hir.fzhhl.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nld.cqqwz.cn

[T11] Kotlin：协程
来源：http://ahy.aibaodan.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ajl.guannengcc.top

[T12] Kotlin：解构声明
来源：http://okf.wangdashe.top

val (a, b) = Pair(1, 2)
来源：http://pdm.aibaodan.cn

[T13] Kotlin：只读 Map
来源：http://rgq.yanxiufei.cn

val m = mapOf("a" to 1)
来源：http://iez.9152youxi.cn

[T14] Kotlin：循环
来源：http://cwy.feifeiyinyue.top

for (i in 1..10) println(i)
来源：http://gdb.haohaochexian.top

[T15] Kotlin：接口
来源：http://jdz.jinyuanbaomall.cn

interface Shape { fun area(): Double }
来源：http://dsf.hesvh.cn

[T16] Swift：Hello World
来源：http://gci.yanxiufei.cn

print("Hello")
来源：http://cjo.zhijiandao.cn

[T17] Swift：变量与常量
来源：http://uvd.uphjek.com

var a = 1;  let b = 2
来源：http://mtr.redwolf501.top

[T18] Swift：字符串插值
来源：http://tzk.shuidangran.top

"值: \(b)"
来源：http://mwo.fehbvm.com

[T19] Swift：可选绑定
来源：http://zlj.tian-w.cn

if let n = opt { print(n) }
来源：http://krm.zhongyouzk.top

[T20] Swift：数组操作
来源：http://wwq.hammf.cn

var a = [1, 2, 3];  a.append(4)
来源：http://iqu.dashuyun.cn

[T21] Swift：遍历
来源：http://ipv.chenzaomai.com

for x in a { print(x) }
来源：http://glf.pengpengdd.cyou

[T22] Swift：字典
来源：http://kxf.shanyushiyangtech.top

var d = ["a": 1];  d["b"] = 2
来源：http://bey.fehbvm.com

[T23] Swift：函数
来源：http://vxp.tianlin.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://eua.zdqjudy.top

[T24] Swift：闭包
来源：http://law.gogol.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ege.sweek.top

[T25] Swift：结构体
来源：http://kse.shanyushiyangtech.top

struct P { var x: Int }
来源：http://udt.cdnleiting.top

[T26] Swift：类与重写
来源：http://xdo.sxryk.cn

class A: Base { override func f() {} }
来源：http://ame.guowangkeji.top

[T27] Swift：错误处理
来源：http://dnb.jlsjyb.cn

do { try f() } catch { print(error) }
来源：http://vlz.jinqigfzy.top

[T28] Swift：枚举
来源：http://vds.ybcxt.top

enum Color { case red, green }
来源：http://dek.52xcode.cn

[T29] Swift：guard 提前返回
来源：http://zpe.ydzc1.top

guard let x = opt else { return }
来源：http://hcl.zhiwuduotai.top

[T30] Swift：协议
来源：http://epq.zhiwuduotai.top

protocol Shape { func area() -> Double }
来源：http://tot.haohaochexian.top

[T31] Lua：Hello World
来源：http://oav.ehwqpu.com

print("Hello")
来源：http://ahe.yfazqb.com

[T32] Lua：局部变量
来源：http://heu.zhongyouzk.top

local a = 1
来源：http://ogs.yj20258888.top

[T33] Lua：表（数组）
来源：http://gid.yvedp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qqe.chenzaomai.com

[T34] Lua：遍历表
来源：http://jko.ehwqpu.com

for i, v in ipairs(t) do print(i, v) end
来源：http://vdm.zycfv.cn

[T35] Lua：字典表
来源：http://ykz.gaohongyu789.top

local d = { a = 1 };  d.b = 2
来源：http://syk.zhixingplan.top

[T36] Lua：函数
来源：http://exu.yuanzhike.top

function add(a, b) return a + b end
来源：http://xrs.sjlbkw.cn

[T37] Lua：字符串拼接
来源：http://zaw.jinyuanbaomall.cn

"a" .. "b"
来源：http://frw.jinyuanbaomall.cn

[T38] Lua：条件
来源：http://ysa.jinyuanbaomall.cn

if x > 0 then print("正") end
来源：http://yqf.tian-w.cn

[T39] Lua：模式匹配
来源：http://fgm.nanxuanxn.top

string.find(s, "%d+")
来源：http://xip.ctjpmb.com

[T40] Lua：元表
来源：http://pjj.chenlongwang.top

setmetatable({}, { __index = base })
来源：http://wng.hammf.cn

[T41] Perl：Hello World
来源：http://mth.wangdashe.top

print "Hello\n";
来源：http://ocp.pengpengdd.cyou

[T42] Perl：变量类型
来源：http://twb.cdnleiting.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jae.guowangkeji.top

[T43] Perl：字符串插值
来源：http://okx.hammf.cn

"值: $a"
来源：http://wgj.quarkkingdee.top

[T44] Perl：条件
来源：http://xai.andypj.xyz

if ($a > 0) { print "正"; }
来源：http://jvc.jinqigfzy.top

[T45] Perl：数组遍历
来源：http://jqu.yueranfly.top

for my $x (@arr) { print $x; }
来源：http://hzt.fehbvm.com

[T46] Perl：哈希操作
来源：http://jvn.yuxming.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sfh.chenjidiqi.icu

[T47] Perl：正则捕获
来源：http://qqr.cashguo.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://eau.yueranfly.top

[T48] Perl：正则替换
来源：http://pqn.zycfv.cn

$s =~ s/old/new/g;
来源：http://iyh.sufxvd.cn

[T49] Perl：函数
来源：http://bcf.cheryme.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qdu.xziqi.cn

[T50] Perl：逐行读文件
来源：http://zcl.andypj.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://jwn.iojbl.cn

while (my $line = <$fh>) { print $line; }
来源：http://rax.jiagoushi.top

[T51] Scala：Hello World
来源：http://xum.yj202588.top

println("Hello")
来源：http://gsx.shanyushiyangkeji.top

[T52] Scala：变量
来源：http://thx.sweek.top

val a = 1;  var b = 2
来源：http://yxw.xinyue.icu

[T53] Scala：字符串插值
来源：http://pfb.birdmap.top

s"值: $b"
来源：http://fie.quarkkingdee.top

[T54] Scala：集合映射
来源：http://sfz.zdbjq.cn

List(1, 2, 3).map(_ * 2)
来源：http://mbh.yvedp.cn

[T55] Scala：集合过滤
来源：http://njm.shzxlz.cn

List(1, 2, 3).filter(_ > 1)
来源：http://uuc.nanxuanxn.top

[T56] Scala：样例类
来源：http://rck.pycfn.com

case class User(name: String, age: Int)
来源：http://pzx.chenzaomai.com

[T57] Scala：模式匹配
来源：http://nru.gaohongyu789.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://yjt.snrcjt.cn

[T58] Scala：函数定义
来源：http://wcj.jqgufenzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://zev.hfpthk.cn

[T59] Scala：循环
来源：http://dfd.jinyuanbaomall.cn

for (i <- 1 to 10) println(i)
来源：http://xnf.haohaochexian.top

[T60] Scala：折叠
来源：http://gql.cucudq.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qxg.gogol.net.cn

================================================================================
来源：http://igs.zhijiandao.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vji.feifeiyinyue.top

================================================================================
来源：http://jkn.cashguo.top

[U01] Py：创建虚拟环境
来源：http://dhz.pycfn.com

python -m venv .venv && source .venv/bin/activate
来源：http://loo.zhijiandao.cn

[U02] Py：导出 / 安装依赖
来源：http://rre.zdbjq.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xdl.guannengcc.top

[U03] Py：加载 .env 配置
来源：http://uuy.0kj1m.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://leh.wangshuangyany.cn

[U04] Py：变量调试打印
来源：http://dhu.bbcook.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kib.sjlbkw.cn

[U05] Py：列表去重且保序
来源：http://lit.yangfankeji.com

list(dict.fromkeys(arr))
来源：http://mky.xuetiantiany.cn

[U06] Py：合并两个字典
来源：http://joj.sweek.top

{**a, **b}
来源：http://riz.hnxiangtu.top

[U07] Py：反转字典键值
来源：http://mkx.tianlin.xyz

{v: k for k, v in d.items()}
来源：http://qdd.zhengqikj.top

[U08] Py：展平二维列表
来源：http://sva.ivvv.top

[y for x in nested for y in x]
来源：http://zsa.fehbvm.com

[U09] Py：字典取最大值的键
来源：http://yyn.fehbvm.com

max(d, key=d.get)
来源：http://rfd.tian-w.cn

[U10] Py：按值排序字典
来源：http://mwn.xylfe.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wal.zdbjq.cn

[U11] Py：生成器表达式
来源：http://dwv.epnwcf.com

(x * 2 for x in arr)
来源：http://mjj.yuanzhike.top

[U12] Py：取出现最多的 3 个元素
来源：http://wub.vehdjk.com

Counter(arr).most_common(3)
来源：http://fci.c1oappe.top

[U13] Py：固定长度队列
来源：http://urm.wangdashe.top

deque(maxlen=10)
来源：http://ahx.cashguo.top

[U14] Py：分组收集到列表
来源：http://tot.ybcxt.top

defaultdict(list)
来源：http://zxq.bjfxy.top

[U15] Py：高精度计时
来源：http://lpu.cashguo.top

t = time.perf_counter()
来源：http://aqf.jianghu66.top

[U16] Py：命令行参数解析
来源：http://vcb.sxryk.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hsn.zycfv.cn

[U17] Py：初始化日志
来源：http://qwk.jlsjyb.cn

logging.basicConfig(level=logging.INFO)
来源：http://gka.cheryme.top

[U18] Py：预编译正则
来源：http://qng.cdnleiting.top

pat = re.compile(r"\d+")
来源：http://nkp.ivvv.top

[U19] Py：正则替换带回调
来源：http://fmx.feifeiyinyue.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gvi.c1oappe.top

[U20] Py：缓存函数结果
来源：http://lne.guannengcc.top

@functools.lru_cache(maxsize=None)
来源：http://nru.shzxlz.cn

[U21] Py：自定义上下文管理器
来源：http://snu.smart0.xyz

@contextlib.contextmanager
来源：http://fiq.andypj.xyz

[U22] Py：矩阵转置
来源：http://opk.sjlbkw.cn

list(zip(*m))
来源：http://hpb.cucudq.cn

[U23] Py：分块读取大文件
来源：http://ziw.cucudq.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://eph.0kj1m.cn

[U24] Py：路径操作
来源：http://inl.ybcxt.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://joq.smart0.xyz

[U25] Py：CSV 按字典读
来源：http://ybp.smart0.xyz

csv.DictReader(f)
来源：http://giw.meibo888.top

[U26] Py：并发下载
来源：http://doq.meibo888.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fch.vqdsnc.cn

[U27] Py：异步 HTTP
来源：http://dbj.jqgfzy.top

aiohttp.ClientSession() 配合 async with
来源：http://ieh.aizwys.cn

[U28] Py：类型别名
来源：http://daq.xziqi.cn

UserId = int
来源：http://wyi.daxiang520.top

[U29] Py：属性校验
来源：http://haz.zhijiandao.cn

@property 与 @x.setter 配合
来源：http://ymw.yongpay.top

[U30] Py：数据类
来源：http://xgs.fengsongda.top

@dataclass(slots=True)
来源：http://wak.yangfankeji.com

[U31] Py：单测
来源：http://qnh.yj202588.top

python -m pytest -q
来源：http://ptj.jinyuanbaomall.cn

[U32] Py：代码格式化
来源：http://bax.gogol.net.cn

ruff format . && ruff check --fix .
来源：http://ibv.dashuyun.cn

[U33] Py：打包发布
来源：http://cqa.jinghuilouyu.cn

python -m build  （依赖 pyproject.toml）
来源：http://dzn.zhixingplan.top

[U34] Py：判断编码
来源：http://gzs.shangyingyoupin.top

chardet.detect(raw)
来源：http://hbw.hesvh.cn

[U35] Py：发送邮件
来源：http://alx.guowangkeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pbb.uphjek.com

[U36] Py：定时任务
来源：http://vxv.jlsjyb.cn

schedule.every(10).minutes.do(job)
来源：http://rpl.hnxiangtu.top

[U37] Py：读写 Excel
来源：http://zdb.zhaomingkeji.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://cxk.birdmap.top

[U38] Py：获取脚本所在目录
来源：http://jbl.shanyushiyangtech.top

Path(__file__).resolve().parent
来源：http://pas.ydjk.org.cn


<!-- 参考信息 -->