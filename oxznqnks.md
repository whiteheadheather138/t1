代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yil.meibo888.top

[S13] C：宏定义
来源：http://fqw.jinghuilouyu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ptc.xuanzx.com

[S14] C：枚举
来源：http://wwj.zhongyouzk.top

enum Color { RED, GREEN, BLUE };
来源：http://xsj.ehwqpu.com

[S15] C：类型转换
来源：http://iiu.daria6918.cn

(double) a / b
来源：http://btv.jqgufenzy.top

[S16] C：位操作置位
来源：http://auy.yangfankeji.com

x |= (1 << 3);
来源：http://lcn.chenjidiqi.icu

[S17] C：安全拼接字符串
来源：http://pta.daria6918.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ikv.zhoulong.xyz

[S18] C：命令行参数
来源：http://yfa.vehdjk.com

int main(int argc, char **argv)
来源：http://qqo.hywenlv.cn

[S19] C：快速排序
来源：http://ocy.hysaishi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tmx.ydjk.org.cn

[S20] C：二分查找
来源：http://ttr.shanyushiyangkeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cmi.yanxiufei.cn

[S21] C：字符类别判断
来源：http://lph.dianchejie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ajv.fzhhl.top

[S22] C：字符串转数字
来源：http://zdc.aizwys.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dfd.zdbjq.cn

[S23] C：随机数
来源：http://hrv.52xcode.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xmh.feifeiyinyue.top

[S24] C：获取本地时间
来源：http://zir.jqgufenzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ezp.shuidangran.top

[S25] C：内存拷贝
来源：http://pbc.gaohongyu789.top

memcpy(dst, src, n);
来源：http://azu.zdbjq.cn

[S26] C：内存清零
来源：http://bzx.zhixingplan.top

memset(a, 0, sizeof a);
来源：http://ubh.bjfxy.top

[S27] C：定义常量
来源：http://fbs.xuetiantiany.cn

const double PI = 3.14159;
来源：http://mcx.iojbl.cn

[S28] C：静态变量
来源：http://wqj.hesvh.cn

static int counter = 0;
来源：http://kpl.cdnleiting.top

[S29] C：变参函数
来源：http://eke.wangshuangyany.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://osp.jlsjyb.cn

[S30] C：头文件保护
来源：http://gru.aibaodan.cn

#ifndef X_H
来源：http://wlx.shzxlz.cn

#define X_H
来源：http://fnw.zdqjudy.top

#endif
来源：http://aam.yfazqb.com

[S31] C++：Hello World
来源：http://dih.ctjpmb.com

#include <iostream>
来源：http://zww.tianlin.xyz

int main() { std::cout << "Hello\n"; }
来源：http://mmg.gogol.net.cn

[S32] C++：字符串
来源：http://krp.zdqjudy.top

std::string s = "hi";  s += "!";
来源：http://wtw.hysaishi.cn

[S33] C++：vector 增删
来源：http://zam.xziqi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pwr.daxiang520.top

[S34] C++：遍历 vector
来源：http://nwn.wangshuangyany.cn

for (auto &x : v) { std::cout << x; }
来源：http://yyr.pengpengdd.cyou

[S35] C++：map
来源：http://qyb.zhengqikj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bel.bbcook.cn

[S36] C++：unordered_map
来源：http://fqk.svipenyu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rhe.nanxuanxn.top

[S37] C++：set
来源：http://lyh.haohaochexian.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://svw.c1oappe.top

[S38] C++：排序
来源：http://hqy.ywan-chungtsiang.top

std::sort(v.begin(), v.end());
来源：http://uqm.hnxiangtu.top

[S39] C++：自定义比较器排序
来源：http://pkd.ehwqpu.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://edk.zycfv.cn

[S40] C++：查找元素
来源：http://omu.fengsongda.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tsb.gotoacloud.top

[S41] C++：类与构造函数
来源：http://iwd.vqdsnc.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://eiw.c1oappe.top

[S42] C++：继承与虚函数
来源：http://cqm.kuanghao11.cn

class B : public Base { public: void f() override {} };
来源：http://bnw.xziqi.cn

[S43] C++：智能指针
来源：http://vbs.xuanzx.com

auto p = std::make_unique<int>(5);
来源：http://nqa.vqdsnc.cn

[S44] C++：引用传参
来源：http://xub.yongpay.top

void inc(int &x) { ++x; }
来源：http://zwu.snrcjt.cn

[S45] C++：lambda
来源：http://mmp.bbcook.cn

auto add = [](int a, int b) { return a + b; };
来源：http://krl.iojbl.cn

[S46] C++：函数模板
来源：http://qid.dashuyun.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://itt.bjfxy.top

[S47] C++：结构化绑定遍历
来源：http://ads.zhiwuduotai.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pdm.daxiang520.top

[S48] C++：逐行读文件
来源：http://cca.shanyushiyangtech.top

std::ifstream in("a.txt");  std::string line;
来源：http://xsa.dianchejie.cn

while (std::getline(in, line)) { }
来源：http://ppu.gaohongyu789.top

[S49] C++：写文件
来源：http://dks.chenjidiqi.icu

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uhg.dianchejie.cn

[S50] C++：格式化数字
来源：http://qsw.yj20258888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bzd.zhaomingkeji.xyz

[S51] C++：显式类型转换
来源：http://vus.yuxming.cn

static_cast<double>(a) / b
来源：http://acb.ctjpmb.com

[S52] C++：const 与 noexcept
来源：http://mpo.zhijiandao.cn

int size() const noexcept { return n_; }
来源：http://vwt.zhiwuduotai.top

[S53] C++：移动语义
来源：http://qdn.fengsongda.top

std::vector<int> w = std::move(v);
来源：http://mia.dashuyun.cn

[S54] C++：异常处理
来源：http://oxc.gotoacloud.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ygg.gogol.net.cn

[S55] C++：结构化绑定
来源：http://thd.hammf.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://uea.ehwqpu.com

[S56] C++：optional
来源：http://itw.jinqigufen.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://obc.pengpengdd.cyou

[S57] C++：编译期常量
来源：http://idk.zhengqikj.top

constexpr int N = 10;
来源：http://xva.ehwqpu.com

[S58] C++：命名空间
来源：http://udr.zycfv.cn

namespace ns { int f() { return 1; } }
来源：http://mne.ivvv.top

[S59] C++：静态断言
来源：http://xrg.zhengqikj.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pmr.andypj.xyz

[S60] C++：遍历并删除元素
来源：http://ngv.shangyingyoupin.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gvq.zhixingplan.top

================================================================================
来源：http://qnk.cucudq.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pva.shangyingyoupin.top

================================================================================
来源：http://aqt.snrcjt.cn

[T01] Kotlin：Hello World
来源：http://gfp.guowangkeji.top

println("Hello")
来源：http://bgl.nanxuanxn.top

[T02] Kotlin：变量
来源：http://leg.fanxiaobao.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nzi.0kj1m.cn

[T03] Kotlin：字符串模板
来源：http://vjg.daria6918.cn

"值: $b"
来源：http://ycj.pycfn.com

[T04] Kotlin：空安全
来源：http://juk.bbcook.cn

val n: String? = null;  n?.length
来源：http://udg.jiagoushi.top

[T05] Kotlin：when 表达式
来源：http://bxw.iojbl.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dle.nanxinkj.top

[T06] Kotlin：集合映射
来源：http://adw.nanxinkj.top

listOf(1, 2, 3).map { it * 2 }
来源：http://cul.yfazqb.com

[T07] Kotlin：集合过滤
来源：http://xea.zhoulong.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://krp.0kj1m.cn

[T08] Kotlin：数据类
来源：http://lix.guannengcc.top

data class User(val name: String, val age: Int)
来源：http://vqd.bbcook.cn

[T09] Kotlin：扩展函数
来源：http://rlw.dianchejie.cn

fun String.exclaim() = this + "!"
来源：http://yvd.hammf.cn

[T10] Kotlin：默认参数
来源：http://fob.havefunace.top

fun greet(name: String = "World") = "Hi $name"
来源：http://pbp.yj202588.top

[T11] Kotlin：协程
来源：http://roj.hysaishi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://oex.xziqi.cn

[T12] Kotlin：解构声明
来源：http://cqz.hfpthk.cn

val (a, b) = Pair(1, 2)
来源：http://gdy.ywan-chungtsiang.top

[T13] Kotlin：只读 Map
来源：http://mzd.haohaochexian.top

val m = mapOf("a" to 1)
来源：http://eph.jiagoushi.top

[T14] Kotlin：循环
来源：http://hyt.jqgufenzy.top

for (i in 1..10) println(i)
来源：http://brd.jyoumei.cn

[T15] Kotlin：接口
来源：http://ipr.zhengqikj.top

interface Shape { fun area(): Double }
来源：http://nbh.hongshengwenyu.top

[T16] Swift：Hello World
来源：http://plz.zhongyouzk.top

print("Hello")
来源：http://nmc.sjlbkw.cn

[T17] Swift：变量与常量
来源：http://ufu.svipenyu.cn

var a = 1;  let b = 2
来源：http://crb.tian-w.cn

[T18] Swift：字符串插值
来源：http://gad.xinyue.icu

"值: \(b)"
来源：http://awo.tianlin.xyz

[T19] Swift：可选绑定
来源：http://bxr.hesvh.cn

if let n = opt { print(n) }
来源：http://hco.zhaomingkeji.xyz

[T20] Swift：数组操作
来源：http://ata.tarul.cn

var a = [1, 2, 3];  a.append(4)
来源：http://svh.fzhhl.top

[T21] Swift：遍历
来源：http://blt.sysykeji.top

for x in a { print(x) }
来源：http://xkq.ywan-chungtsiang.top

[T22] Swift：字典
来源：http://dul.guowangkeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://qeu.jinyuanbaomall.cn

[T23] Swift：函数
来源：http://vlw.jinyuanbaomall.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://iee.wangdashe.top

[T24] Swift：闭包
来源：http://foo.daria6918.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dvh.zhengqikj.top

[T25] Swift：结构体
来源：http://saq.ehwqpu.com

struct P { var x: Int }
来源：http://wps.ehwqpu.com

[T26] Swift：类与重写
来源：http://rna.nwbrower.top

class A: Base { override func f() {} }
来源：http://hsk.guannengcc.top

[T27] Swift：错误处理
来源：http://vgo.daria6918.cn

do { try f() } catch { print(error) }
来源：http://xcb.aibaodan.cn

[T28] Swift：枚举
来源：http://nmf.gzhubu.top

enum Color { case red, green }
来源：http://qqb.hnqzz.top

[T29] Swift：guard 提前返回
来源：http://pms.tian-w.cn

guard let x = opt else { return }
来源：http://gca.jianghu66.top

[T30] Swift：协议
来源：http://bwm.daxiang520.top

protocol Shape { func area() -> Double }
来源：http://ayy.yuanzhike.top

[T31] Lua：Hello World
来源：http://qts.jinghuilouyu.cn

print("Hello")
来源：http://uzk.yj20258888.top

[T32] Lua：局部变量
来源：http://zoj.kuanghao11.cn

local a = 1
来源：http://ivn.xuanzx.com

[T33] Lua：表（数组）
来源：http://qbc.shanyushiyangtech.top

local t = {1, 2, 3};  t[4] = 4
来源：http://uio.zdbjq.cn

[T34] Lua：遍历表
来源：http://gfh.shanyushiyangkeji.top

for i, v in ipairs(t) do print(i, v) end
来源：http://lea.yangfankeji.com

[T35] Lua：字典表
来源：http://tri.hysaishi.cn

local d = { a = 1 };  d.b = 2
来源：http://rur.shangyingyoupin.top

[T36] Lua：函数
来源：http://qqr.jyoumei.cn

function add(a, b) return a + b end
来源：http://efe.sysykeji.top

[T37] Lua：字符串拼接
来源：http://ojs.jinyuanbaomall.cn

"a" .. "b"
来源：http://fgb.vehdjk.com

[T38] Lua：条件
来源：http://drm.tarul.cn

if x > 0 then print("正") end
来源：http://cbf.sweek.top

[T39] Lua：模式匹配
来源：http://fsa.cashguo.top

string.find(s, "%d+")
来源：http://pbj.gaohongyu789.top

[T40] Lua：元表
来源：http://cpx.fanxiaobao.xyz

setmetatable({}, { __index = base })
来源：http://fvn.sxryk.cn

[T41] Perl：Hello World
来源：http://sbb.pycfn.com

print "Hello\n";
来源：http://nrn.ybcxt.top

[T42] Perl：变量类型
来源：http://iki.yangfankeji.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kua.fanxiaobao.xyz

[T43] Perl：字符串插值
来源：http://lev.jinqigufen.top

"值: $a"
来源：http://ywh.0kj1m.cn

[T44] Perl：条件
来源：http://bkk.jqgufenzy.top

if ($a > 0) { print "正"; }
来源：http://xbw.iojbl.cn

[T45] Perl：数组遍历
来源：http://olk.andypj.xyz

for my $x (@arr) { print $x; }
来源：http://mod.tianlin.xyz

[T46] Perl：哈希操作
来源：http://itm.yj202588.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://njq.aibaodan.cn

[T47] Perl：正则捕获
来源：http://cri.gotoacloud.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://rvl.cashguo.top

[T48] Perl：正则替换
来源：http://dam.yuanzhike.top

$s =~ s/old/new/g;
来源：http://uol.tarul.cn

[T49] Perl：函数
来源：http://rdy.guowangkeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cvg.hysaishi.cn

[T50] Perl：逐行读文件
来源：http://nas.hongshengwenyu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://dwy.cdnleiting.top

while (my $line = <$fh>) { print $line; }
来源：http://zwv.xziqi.cn

[T51] Scala：Hello World
来源：http://nzs.gotoacloud.top

println("Hello")
来源：http://zem.tarul.cn

[T52] Scala：变量
来源：http://hvb.vehdjk.com

val a = 1;  var b = 2
来源：http://cvw.wangshuangyany.cn

[T53] Scala：字符串插值
来源：http://isd.wangdashe.top

s"值: $b"
来源：http://xju.sufxvd.cn

[T54] Scala：集合映射
来源：http://vlo.shanyushiyangtech.top

List(1, 2, 3).map(_ * 2)
来源：http://fmy.vqdsnc.cn

[T55] Scala：集合过滤
来源：http://acq.jlsjyb.cn

List(1, 2, 3).filter(_ > 1)
来源：http://oon.chenjidiqi.icu

[T56] Scala：样例类
来源：http://gwk.fehbvm.com

case class User(name: String, age: Int)
来源：http://tit.sjlbkw.cn

[T57] Scala：模式匹配
来源：http://dqp.sufxvd.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nlb.gogol.net.cn

[T58] Scala：函数定义
来源：http://hcm.316326.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://qwv.yj202588.top

[T59] Scala：循环
来源：http://sax.zhongyouzk.top

for (i <- 1 to 10) println(i)
来源：http://yeu.jiagoushi.top

[T60] Scala：折叠
来源：http://qdv.shanyushiyangkeji.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dfa.gzhubu.top

================================================================================
来源：http://enb.bbcook.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://huf.aizwys.cn

================================================================================
来源：http://nlu.jianghu66.top

[U01] Py：创建虚拟环境
来源：http://yac.cdnleiting.top

python -m venv .venv && source .venv/bin/activate
来源：http://vop.ehwqpu.com

[U02] Py：导出 / 安装依赖
来源：http://qhl.zhaomingkeji.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lbp.iojbl.cn

[U03] Py：加载 .env 配置
来源：http://hel.zdqjudy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://nqn.tanke756.top

[U04] Py：变量调试打印
来源：http://pav.0kj1m.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vmv.c1oappe.top

[U05] Py：列表去重且保序
来源：http://fur.gotoacloud.top

list(dict.fromkeys(arr))
来源：http://dfh.zdqjudy.top

[U06] Py：合并两个字典
来源：http://ocx.andypj.xyz

{**a, **b}
来源：http://pbc.zhengqikj.top

[U07] Py：反转字典键值
来源：http://hbx.zycfv.cn

{v: k for k, v in d.items()}
来源：http://qyg.fehbvm.com

[U08] Py：展平二维列表
来源：http://bpn.bjfxy.top

[y for x in nested for y in x]
来源：http://mij.c1oappe.top

[U09] Py：字典取最大值的键
来源：http://zqm.ydjk.org.cn

max(d, key=d.get)
来源：http://fnj.chenjidiqi.icu

[U10] Py：按值排序字典
来源：http://bvf.yuanzhike.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tsx.xinyue.icu

[U11] Py：生成器表达式
来源：http://whf.zdqjudy.top

(x * 2 for x in arr)
来源：http://gws.hesvh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tnb.zdbjq.cn

Counter(arr).most_common(3)
来源：http://gtj.fehbvm.com

[U13] Py：固定长度队列
来源：http://txk.c1oappe.top

deque(maxlen=10)
来源：http://fwu.shzxlz.cn

[U14] Py：分组收集到列表
来源：http://bmi.cashguo.top

defaultdict(list)
来源：http://kut.pycfn.com

[U15] Py：高精度计时
来源：http://ypa.hywenlv.cn

t = time.perf_counter()
来源：http://vpz.quarkkingdee.top

[U16] Py：命令行参数解析
来源：http://yey.ehwqpu.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rah.nwbrower.top

[U17] Py：初始化日志
来源：http://wkt.chenzaomai.com

logging.basicConfig(level=logging.INFO)
来源：http://nhp.shangyingyoupin.top

[U18] Py：预编译正则
来源：http://ksc.guowangkeji.top

pat = re.compile(r"\d+")
来源：http://abc.cucudq.cn

[U19] Py：正则替换带回调
来源：http://wsd.fktsv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vfb.tian-w.cn

[U20] Py：缓存函数结果
来源：http://fjp.cdnleiting.top

@functools.lru_cache(maxsize=None)
来源：http://dhk.andypj.xyz

[U21] Py：自定义上下文管理器
来源：http://pjc.shangyingyoupin.top

@contextlib.contextmanager
来源：http://awj.yj202588.top

[U22] Py：矩阵转置
来源：http://mrd.yj20258.top

list(zip(*m))
来源：http://hoq.aizwys.cn

[U23] Py：分块读取大文件
来源：http://tbf.daxiang520.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zsl.daxiang520.top

[U24] Py：路径操作
来源：http://ujs.uphjek.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://iho.hcnkem.com

[U25] Py：CSV 按字典读
来源：http://fqw.fzhhl.top

csv.DictReader(f)
来源：http://ioo.zhixingplan.top

[U26] Py：并发下载
来源：http://omu.chenzaomai.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lsx.ehwqpu.com

[U27] Py：异步 HTTP
来源：http://khg.yongpay.top

aiohttp.ClientSession() 配合 async with
来源：http://lny.shanyushiyangkeji.top

[U28] Py：类型别名
来源：http://xmz.cheryme.top

UserId = int
来源：http://woc.sysykeji.top

[U29] Py：属性校验
来源：http://bwb.hnqzz.top

@property 与 @x.setter 配合
来源：http://jxc.snrcjt.cn

[U30] Py：数据类
来源：http://vmy.guannengcc.top

@dataclass(slots=True)
来源：http://qei.fktsv.cn

[U31] Py：单测
来源：http://fty.zhaomingkeji.xyz

python -m pytest -q
来源：http://ysm.xylfe.cn

[U32] Py：代码格式化
来源：http://cvp.chenjidiqi.icu

ruff format . && ruff check --fix .
来源：http://yos.nwbrower.top

[U33] Py：打包发布
来源：http://djm.jqgfzy.top

python -m build  （依赖 pyproject.toml）
来源：http://tji.jiagoushi.top

[U34] Py：判断编码
来源：http://lxn.meibo888.top

chardet.detect(raw)
来源：http://wps.ppjwa.cn

[U35] Py：发送邮件
来源：http://ysw.ehwqpu.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://teu.yueranfly.top

[U36] Py：定时任务
来源：http://iyu.yfazqb.com

schedule.every(10).minutes.do(job)
来源：http://gxg.feifeiyinyue.top


<!-- 参考信息 -->