代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mdh.gotoacloud.top

[S10] C：指针与解引用
来源：http://nxg.gzhubu.top

int *p = &a;  *p = 5;
来源：http://ukq.tarul.cn

[S11] C：逐行读文件
来源：http://jfq.kuanghao11.cn

FILE *f = fopen("a.txt", "r");
来源：http://abn.zhijiandao.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dim.pengpengdd.cyou

fclose(f);
来源：http://inn.fehbvm.com

[S12] C：写文件
来源：http://qad.smart0.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://eif.xziqi.cn

[S13] C：宏定义
来源：http://kkx.hongshengwenyu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nfl.bbcook.cn

[S14] C：枚举
来源：http://gum.vqdsnc.cn

enum Color { RED, GREEN, BLUE };
来源：http://jra.cqqwz.cn

[S15] C：类型转换
来源：http://wzw.chenlongwang.top

(double) a / b
来源：http://lsq.yonumen.top

[S16] C：位操作置位
来源：http://les.cheryme.top

x |= (1 << 3);
来源：http://uiu.chenzaomai.com

[S17] C：安全拼接字符串
来源：http://jnz.jinghuilouyu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xfh.sjlbkw.cn

[S18] C：命令行参数
来源：http://wbw.c1oappe.top

int main(int argc, char **argv)
来源：http://sdc.yuxming.cn

[S19] C：快速排序
来源：http://vhs.yonumen.top

qsort(a, n, sizeof(int), cmp);
来源：http://rys.zdbjq.cn

[S20] C：二分查找
来源：http://cmm.tianlin.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nmn.iojbl.cn

[S21] C：字符类别判断
来源：http://nxw.yuxming.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tgz.feifeiyinyue.top

[S22] C：字符串转数字
来源：http://xqg.aibaodan.cn

atoi("42");  strtod("3.14", NULL);
来源：http://apl.vqdsnc.cn

[S23] C：随机数
来源：http://jae.vehdjk.com

srand(time(NULL));  int r = rand() % 100;
来源：http://wpt.tian-w.cn

[S24] C：获取本地时间
来源：http://mcr.haohaochexian.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bks.yvedp.cn

[S25] C：内存拷贝
来源：http://hfb.ctjpmb.com

memcpy(dst, src, n);
来源：http://ugw.shzxlz.cn

[S26] C：内存清零
来源：http://uon.chenjidiqi.icu

memset(a, 0, sizeof a);
来源：http://vab.fzhhl.top

[S27] C：定义常量
来源：http://hzj.fktsv.cn

const double PI = 3.14159;
来源：http://adx.jinqigfzy.top

[S28] C：静态变量
来源：http://ztn.zhiwuduotai.top

static int counter = 0;
来源：http://nhr.smart0.xyz

[S29] C：变参函数
来源：http://fzh.fzhhl.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://etn.iojbl.cn

[S30] C：头文件保护
来源：http://usf.hysaishi.cn

#ifndef X_H
来源：http://urs.hfpthk.cn

#define X_H
来源：http://sfu.zdbjq.cn

#endif
来源：http://ddg.aizwys.cn

[S31] C++：Hello World
来源：http://ofr.daxiang520.top

#include <iostream>
来源：http://ueh.fehbvm.com

int main() { std::cout << "Hello\n"; }
来源：http://pho.ydzc1.top

[S32] C++：字符串
来源：http://zye.chenlongwang.top

std::string s = "hi";  s += "!";
来源：http://akr.yfazqb.com

[S33] C++：vector 增删
来源：http://mst.zycfv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gkf.hesvh.cn

[S34] C++：遍历 vector
来源：http://nun.zhiwuduotai.top

for (auto &x : v) { std::cout << x; }
来源：http://csp.fzhhl.top

[S35] C++：map
来源：http://qui.ehwqpu.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ymz.yvedp.cn

[S36] C++：unordered_map
来源：http://pbc.fanxiaobao.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://odm.sufxvd.cn

[S37] C++：set
来源：http://gip.yonumen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rdh.smart0.xyz

[S38] C++：排序
来源：http://tgm.epnwcf.com

std::sort(v.begin(), v.end());
来源：http://pbx.ywan-chungtsiang.top

[S39] C++：自定义比较器排序
来源：http://igl.uphjek.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uin.shanyushiyangkeji.top

[S40] C++：查找元素
来源：http://hcl.ehwqpu.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://aem.uphjek.com

[S41] C++：类与构造函数
来源：http://gic.ehwqpu.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lak.ctjpmb.com

[S42] C++：继承与虚函数
来源：http://jzb.havefunace.top

class B : public Base { public: void f() override {} };
来源：http://uzm.fehbvm.com

[S43] C++：智能指针
来源：http://pcc.hywenlv.cn

auto p = std::make_unique<int>(5);
来源：http://oja.gaohongyu789.top

[S44] C++：引用传参
来源：http://bvc.xziqi.cn

void inc(int &x) { ++x; }
来源：http://lyk.yvedp.cn

[S45] C++：lambda
来源：http://tzy.chenjidiqi.icu

auto add = [](int a, int b) { return a + b; };
来源：http://czx.zycfv.cn

[S46] C++：函数模板
来源：http://tjp.9152youxi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hkw.fengsongda.top

[S47] C++：结构化绑定遍历
来源：http://xpv.fzhhl.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://aey.redwolf501.top

[S48] C++：逐行读文件
来源：http://etn.0kj1m.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tdd.tianlin.xyz

while (std::getline(in, line)) { }
来源：http://imo.gzhubu.top

[S49] C++：写文件
来源：http://uhw.jinyuanbaomall.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mfz.guowangkeji.top

[S50] C++：格式化数字
来源：http://ozm.ydzc1.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zll.ydjk.org.cn

[S51] C++：显式类型转换
来源：http://bqc.jianghu66.top

static_cast<double>(a) / b
来源：http://dgn.zhongyouzk.top

[S52] C++：const 与 noexcept
来源：http://oth.ybcxt.top

int size() const noexcept { return n_; }
来源：http://mll.svipenyu.cn

[S53] C++：移动语义
来源：http://zfl.daria6918.cn

std::vector<int> w = std::move(v);
来源：http://ywi.quarkkingdee.top

[S54] C++：异常处理
来源：http://dnj.wangdashe.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ncp.ehwqpu.com

[S55] C++：结构化绑定
来源：http://qhz.svipenyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lxt.zdbjq.cn

[S56] C++：optional
来源：http://bsq.wangshuangyany.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bew.zhongyouzk.top

[S57] C++：编译期常量
来源：http://yfk.fanxiaobao.xyz

constexpr int N = 10;
来源：http://mop.ydjk.org.cn

[S58] C++：命名空间
来源：http://iev.ydjk.org.cn

namespace ns { int f() { return 1; } }
来源：http://afi.cqqwz.cn

[S59] C++：静态断言
来源：http://qjr.yanxiufei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bpe.tianlin.xyz

[S60] C++：遍历并删除元素
来源：http://npk.guowangkeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://itp.nanxuanxn.top

================================================================================
来源：http://iot.epnwcf.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tah.jinghuilouyu.cn

================================================================================
来源：http://lya.hfpthk.cn

[T01] Kotlin：Hello World
来源：http://vgs.zdbjq.cn

println("Hello")
来源：http://ufu.yuanzhike.top

[T02] Kotlin：变量
来源：http://aut.haohaochexian.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qqf.aizwys.cn

[T03] Kotlin：字符串模板
来源：http://sxf.haohaochexian.top

"值: $b"
来源：http://seu.snrcjt.cn

[T04] Kotlin：空安全
来源：http://lya.bbcook.cn

val n: String? = null;  n?.length
来源：http://rgk.smart0.xyz

[T05] Kotlin：when 表达式
来源：http://qsd.zhengqikj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wpy.yj20258.top

[T06] Kotlin：集合映射
来源：http://wmi.meibo888.top

listOf(1, 2, 3).map { it * 2 }
来源：http://fae.shanyushiyangtech.top

[T07] Kotlin：集合过滤
来源：http://poe.daxiang520.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://zfj.cashguo.top

[T08] Kotlin：数据类
来源：http://tar.dashuyun.cn

data class User(val name: String, val age: Int)
来源：http://aex.zhaomingkeji.xyz

[T09] Kotlin：扩展函数
来源：http://oox.nwbrower.top

fun String.exclaim() = this + "!"
来源：http://cyi.daria6918.cn

[T10] Kotlin：默认参数
来源：http://sgp.hcnkem.com

fun greet(name: String = "World") = "Hi $name"
来源：http://umv.sjlbkw.cn

[T11] Kotlin：协程
来源：http://xjz.zhiwuduotai.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ljq.fzhhl.top

[T12] Kotlin：解构声明
来源：http://uid.tarul.cn

val (a, b) = Pair(1, 2)
来源：http://gez.fzhhl.top

[T13] Kotlin：只读 Map
来源：http://fwl.ywan-chungtsiang.top

val m = mapOf("a" to 1)
来源：http://cem.wangdashe.top

[T14] Kotlin：循环
来源：http://yqx.daria6918.cn

for (i in 1..10) println(i)
来源：http://hjl.svipenyu.cn

[T15] Kotlin：接口
来源：http://hog.jqgfzy.top

interface Shape { fun area(): Double }
来源：http://cqe.feifeiyinyue.top

[T16] Swift：Hello World
来源：http://ggb.xuanzx.com

print("Hello")
来源：http://swb.epnwcf.com

[T17] Swift：变量与常量
来源：http://ylr.bjfxy.top

var a = 1;  let b = 2
来源：http://xxr.tian-w.cn

[T18] Swift：字符串插值
来源：http://fhc.uphjek.com

"值: \(b)"
来源：http://afh.haohaochexian.top

[T19] Swift：可选绑定
来源：http://ubx.guannengcc.top

if let n = opt { print(n) }
来源：http://cjc.birdmap.top

[T20] Swift：数组操作
来源：http://hti.ydzc1.top

var a = [1, 2, 3];  a.append(4)
来源：http://jap.jqgfzy.top

[T21] Swift：遍历
来源：http://kpu.bbcook.cn

for x in a { print(x) }
来源：http://pyl.ywan-chungtsiang.top

[T22] Swift：字典
来源：http://hpw.zhiwuduotai.top

var d = ["a": 1];  d["b"] = 2
来源：http://zrd.sufxvd.cn

[T23] Swift：函数
来源：http://gkc.epnwcf.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lto.nanxuanxn.top

[T24] Swift：闭包
来源：http://clb.shanyushiyangtech.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://thm.ywan-chungtsiang.top

[T25] Swift：结构体
来源：http://atq.hywenlv.cn

struct P { var x: Int }
来源：http://ayf.tianlin.xyz

[T26] Swift：类与重写
来源：http://scj.bbcook.cn

class A: Base { override func f() {} }
来源：http://wfs.yj20258888.top

[T27] Swift：错误处理
来源：http://tza.tarul.cn

do { try f() } catch { print(error) }
来源：http://ckg.hfpthk.cn

[T28] Swift：枚举
来源：http://qac.shanyushiyangkeji.top

enum Color { case red, green }
来源：http://keb.gaohongyu789.top

[T29] Swift：guard 提前返回
来源：http://lfu.cdnleiting.top

guard let x = opt else { return }
来源：http://ueg.gzhubu.top

[T30] Swift：协议
来源：http://oit.hcnkem.com

protocol Shape { func area() -> Double }
来源：http://nlm.nanxinkj.top

[T31] Lua：Hello World
来源：http://tzc.zdbjq.cn

print("Hello")
来源：http://vvk.jianghu66.top

[T32] Lua：局部变量
来源：http://uid.ydzc1.top

local a = 1
来源：http://mku.bbcook.cn

[T33] Lua：表（数组）
来源：http://dsz.nanxinkj.top

local t = {1, 2, 3};  t[4] = 4
来源：http://dbw.tarul.cn

[T34] Lua：遍历表
来源：http://zim.jinyuanbaomall.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nan.bbcook.cn

[T35] Lua：字典表
来源：http://ggz.fengsongda.top

local d = { a = 1 };  d.b = 2
来源：http://drn.shanyushiyangkeji.top

[T36] Lua：函数
来源：http://xtp.hnxiangtu.top

function add(a, b) return a + b end
来源：http://kev.0kj1m.cn

[T37] Lua：字符串拼接
来源：http://edd.birdmap.top

"a" .. "b"
来源：http://mmn.tarul.cn

[T38] Lua：条件
来源：http://cbb.iojbl.cn

if x > 0 then print("正") end
来源：http://uis.jinqigufen.top

[T39] Lua：模式匹配
来源：http://uzb.zhijiandao.cn

string.find(s, "%d+")
来源：http://gxm.feifeiyinyue.top

[T40] Lua：元表
来源：http://xnt.vehdjk.com

setmetatable({}, { __index = base })
来源：http://hfg.feifeiyinyue.top

[T41] Perl：Hello World
来源：http://adb.fengsongda.top

print "Hello\n";
来源：http://xyi.dianchejie.cn

[T42] Perl：变量类型
来源：http://cyj.hnxiangtu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://eis.aibaodan.cn

[T43] Perl：字符串插值
来源：http://yar.birdmap.top

"值: $a"
来源：http://ddp.chenlongwang.top

[T44] Perl：条件
来源：http://kev.jinghuilouyu.cn

if ($a > 0) { print "正"; }
来源：http://rnn.daxiang520.top

[T45] Perl：数组遍历
来源：http://kvx.jinghuilouyu.cn

for my $x (@arr) { print $x; }
来源：http://ifl.zhengqikj.top

[T46] Perl：哈希操作
来源：http://qhw.jinyuanbaomall.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nal.nwbrower.top

[T47] Perl：正则捕获
来源：http://lwf.sxryk.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gvs.jyoumei.cn

[T48] Perl：正则替换
来源：http://mbv.cdnleiting.top

$s =~ s/old/new/g;
来源：http://hoe.tianlin.xyz

[T49] Perl：函数
来源：http://fzj.c1oappe.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kyk.ybcxt.top

[T50] Perl：逐行读文件
来源：http://rom.jyoumei.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zpc.andypj.xyz

while (my $line = <$fh>) { print $line; }
来源：http://hcg.smart0.xyz

[T51] Scala：Hello World
来源：http://voe.fktsv.cn

println("Hello")
来源：http://ujf.sjlbkw.cn

[T52] Scala：变量
来源：http://cbl.hywenlv.cn

val a = 1;  var b = 2
来源：http://wan.nwbrower.top

[T53] Scala：字符串插值
来源：http://zbx.snrcjt.cn

s"值: $b"
来源：http://zou.shangyingyoupin.top

[T54] Scala：集合映射
来源：http://agy.bjfxy.top

List(1, 2, 3).map(_ * 2)
来源：http://jeg.jyoumei.cn

[T55] Scala：集合过滤
来源：http://vva.jinghuilouyu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ssx.c1oappe.top

[T56] Scala：样例类
来源：http://tfy.pycfn.com

case class User(name: String, age: Int)
来源：http://myp.chenzaomai.com

[T57] Scala：模式匹配
来源：http://ytg.fzhhl.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://rng.yj202588.top

[T58] Scala：函数定义
来源：http://vsi.bbcook.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mfb.daria6918.cn

[T59] Scala：循环
来源：http://lty.yj20258.top

for (i <- 1 to 10) println(i)
来源：http://uoq.haohaochexian.top

[T60] Scala：折叠
来源：http://vwc.xylfe.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://woc.cqqwz.cn

================================================================================
来源：http://eah.ehwqpu.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ngc.haohaochexian.top

================================================================================
来源：http://ztg.yueranfly.top

[U01] Py：创建虚拟环境
来源：http://bjm.ydjk.org.cn

python -m venv .venv && source .venv/bin/activate
来源：http://iyw.fehbvm.com

[U02] Py：导出 / 安装依赖
来源：http://cfg.snrcjt.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zte.gogol.net.cn

[U03] Py：加载 .env 配置
来源：http://mwl.jinqigfzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://esq.ehwqpu.com

[U04] Py：变量调试打印
来源：http://hnb.cheryme.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yuw.svipenyu.cn

[U05] Py：列表去重且保序
来源：http://kou.daxiang520.top

list(dict.fromkeys(arr))
来源：http://jmd.meibo888.top

[U06] Py：合并两个字典
来源：http://acc.fengsongda.top

{**a, **b}
来源：http://hrw.yj20258.top

[U07] Py：反转字典键值
来源：http://elj.gzhubu.top

{v: k for k, v in d.items()}
来源：http://pyp.yfazqb.com

[U08] Py：展平二维列表
来源：http://njx.gotoacloud.top

[y for x in nested for y in x]
来源：http://haq.fktsv.cn

[U09] Py：字典取最大值的键
来源：http://qgb.sweek.top

max(d, key=d.get)
来源：http://awi.wangshuangyany.cn

[U10] Py：按值排序字典
来源：http://qrl.yj20258.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kac.smart0.xyz

[U11] Py：生成器表达式
来源：http://dkz.fanxiaobao.xyz

(x * 2 for x in arr)
来源：http://uir.jlsjyb.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rmu.zhijiandao.cn

Counter(arr).most_common(3)
来源：http://rdy.epnwcf.com

[U13] Py：固定长度队列
来源：http://qlp.epnwcf.com

deque(maxlen=10)
来源：http://xyr.zhengqikj.top

[U14] Py：分组收集到列表
来源：http://rxf.pycfn.com

defaultdict(list)
来源：http://vvn.yj20258.top

[U15] Py：高精度计时
来源：http://flg.daxiang520.top

t = time.perf_counter()
来源：http://biz.bjfxy.top

[U16] Py：命令行参数解析
来源：http://syb.meibo888.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://unp.fengsongda.top

[U17] Py：初始化日志
来源：http://fpy.ppjwa.cn

logging.basicConfig(level=logging.INFO)
来源：http://jug.bbcook.cn

[U18] Py：预编译正则
来源：http://yyt.snrcjt.cn

pat = re.compile(r"\d+")
来源：http://dii.dashuyun.cn

[U19] Py：正则替换带回调
来源：http://jpi.andypj.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wax.c1oappe.top

[U20] Py：缓存函数结果
来源：http://wdq.tian-w.cn

@functools.lru_cache(maxsize=None)
来源：http://kew.redwolf501.top

[U21] Py：自定义上下文管理器
来源：http://zfs.zhongyouzk.top

@contextlib.contextmanager
来源：http://vbr.52xcode.cn

[U22] Py：矩阵转置
来源：http://bvb.ywan-chungtsiang.top

list(zip(*m))
来源：http://fwq.316326.xyz

[U23] Py：分块读取大文件
来源：http://dnl.52xcode.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rvu.snrcjt.cn

[U24] Py：路径操作
来源：http://bzu.jiagoushi.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://aaf.hcnkem.com

[U25] Py：CSV 按字典读
来源：http://uav.bjfxy.top

csv.DictReader(f)
来源：http://kws.zdqjudy.top

[U26] Py：并发下载
来源：http://nyy.redwolf501.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ghm.hysaishi.cn

[U27] Py：异步 HTTP
来源：http://imq.hnqzz.top

aiohttp.ClientSession() 配合 async with
来源：http://ipw.yuxming.cn

[U28] Py：类型别名
来源：http://zpi.52xcode.cn

UserId = int
来源：http://bvd.shanyushiyangtech.top

[U29] Py：属性校验
来源：http://hgz.hfpthk.cn

@property 与 @x.setter 配合
来源：http://dvt.0kj1m.cn

[U30] Py：数据类
来源：http://dhz.jyoumei.cn

@dataclass(slots=True)
来源：http://fvm.nwbrower.top

[U31] Py：单测
来源：http://pev.gogol.net.cn

python -m pytest -q
来源：http://mvb.hnxiangtu.top

[U32] Py：代码格式化
来源：http://ekx.zhoulong.xyz

ruff format . && ruff check --fix .
来源：http://vja.cdnleiting.top


<!-- 参考信息 -->