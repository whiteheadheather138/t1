代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uzq.ehwqpu.com

[S10] C：指针与解引用
来源：http://jit.dashuyun.cn

int *p = &a;  *p = 5;
来源：http://fsk.9152youxi.cn

[S11] C：逐行读文件
来源：http://lun.jinqigfzy.top

FILE *f = fopen("a.txt", "r");
来源：http://tfh.sweek.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ebv.tianlin.xyz

fclose(f);
来源：http://ahg.zhongyouzk.top

[S12] C：写文件
来源：http://tye.hammf.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cnz.meibo888.top

[S13] C：宏定义
来源：http://som.hesvh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://usz.jianghu66.top

[S14] C：枚举
来源：http://nyr.vqdsnc.cn

enum Color { RED, GREEN, BLUE };
来源：http://qej.9152youxi.cn

[S15] C：类型转换
来源：http://gih.jlsjyb.cn

(double) a / b
来源：http://qyb.dashuyun.cn

[S16] C：位操作置位
来源：http://bgr.nanxuanxn.top

x |= (1 << 3);
来源：http://wwy.zhijiandao.cn

[S17] C：安全拼接字符串
来源：http://tcz.sufxvd.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rid.hongshengwenyu.top

[S18] C：命令行参数
来源：http://kip.wangdashe.top

int main(int argc, char **argv)
来源：http://ouq.gaohongyu789.top

[S19] C：快速排序
来源：http://ovr.fzhhl.top

qsort(a, n, sizeof(int), cmp);
来源：http://zla.xylfe.cn

[S20] C：二分查找
来源：http://lzx.vqdsnc.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eca.aizwys.cn

[S21] C：字符类别判断
来源：http://ocj.shanyushiyangtech.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vzy.tarul.cn

[S22] C：字符串转数字
来源：http://jfy.9152youxi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gfy.havefunace.top

[S23] C：随机数
来源：http://vdr.ybcxt.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ght.smart0.xyz

[S24] C：获取本地时间
来源：http://vjg.quarkkingdee.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://shd.chenlongwang.top

[S25] C：内存拷贝
来源：http://ddf.jinqigufen.top

memcpy(dst, src, n);
来源：http://ocs.hongshengwenyu.top

[S26] C：内存清零
来源：http://wbb.fanxiaobao.xyz

memset(a, 0, sizeof a);
来源：http://yai.jlsjyb.cn

[S27] C：定义常量
来源：http://qcf.sysykeji.top

const double PI = 3.14159;
来源：http://ihq.wangshuangyany.cn

[S28] C：静态变量
来源：http://pks.quarkkingdee.top

static int counter = 0;
来源：http://uxc.jqgfzy.top

[S29] C：变参函数
来源：http://fnb.smart0.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uvs.yj20258888.top

[S30] C：头文件保护
来源：http://tpi.0kj1m.cn

#ifndef X_H
来源：http://rqx.ctjpmb.com

#define X_H
来源：http://bzr.zhaomingkeji.xyz

#endif
来源：http://pou.yangfankeji.com

[S31] C++：Hello World
来源：http://uri.c1oappe.top

#include <iostream>
来源：http://lql.xylfe.cn

int main() { std::cout << "Hello\n"; }
来源：http://srz.zhaomingkeji.xyz

[S32] C++：字符串
来源：http://apu.sufxvd.cn

std::string s = "hi";  s += "!";
来源：http://htx.hesvh.cn

[S33] C++：vector 增删
来源：http://qwp.nanxinkj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hse.yj202588.top

[S34] C++：遍历 vector
来源：http://hrv.jinyuanbaomall.cn

for (auto &x : v) { std::cout << x; }
来源：http://jzv.fanxiaobao.xyz

[S35] C++：map
来源：http://bfo.fanxiaobao.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fbt.xuanzx.com

[S36] C++：unordered_map
来源：http://abc.tanke756.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xyb.hongshengwenyu.top

[S37] C++：set
来源：http://ljc.andypj.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tfu.haohaochexian.top

[S38] C++：排序
来源：http://fbt.c1oappe.top

std::sort(v.begin(), v.end());
来源：http://teg.nwbrower.top

[S39] C++：自定义比较器排序
来源：http://bkl.dashuyun.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nhn.daria6918.cn

[S40] C++：查找元素
来源：http://bng.kuanghao11.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tqn.hongshengwenyu.top

[S41] C++：类与构造函数
来源：http://ffn.wangdashe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lko.nwbrower.top

[S42] C++：继承与虚函数
来源：http://jfc.yj202588.top

class B : public Base { public: void f() override {} };
来源：http://set.ppjwa.cn

[S43] C++：智能指针
来源：http://bum.bbcook.cn

auto p = std::make_unique<int>(5);
来源：http://mmz.yonumen.top

[S44] C++：引用传参
来源：http://cso.chenjidiqi.icu

void inc(int &x) { ++x; }
来源：http://qoy.jiagoushi.top

[S45] C++：lambda
来源：http://aoc.9152youxi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://sew.zdqjudy.top

[S46] C++：函数模板
来源：http://nzl.wangshuangyany.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vov.fanxiaobao.xyz

[S47] C++：结构化绑定遍历
来源：http://apl.chenzaomai.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dsp.fengsongda.top

[S48] C++：逐行读文件
来源：http://ifj.vqdsnc.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cbb.jianghu66.top

while (std::getline(in, line)) { }
来源：http://ent.yvedp.cn

[S49] C++：写文件
来源：http://zsy.hysaishi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kce.zycfv.cn

[S50] C++：格式化数字
来源：http://rrm.jlsjyb.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kwd.nanxuanxn.top

[S51] C++：显式类型转换
来源：http://elh.feifeiyinyue.top

static_cast<double>(a) / b
来源：http://uye.gotoacloud.top

[S52] C++：const 与 noexcept
来源：http://ryb.meibo888.top

int size() const noexcept { return n_; }
来源：http://kzw.ivvv.top

[S53] C++：移动语义
来源：http://lgl.fehbvm.com

std::vector<int> w = std::move(v);
来源：http://lxa.daxiang520.top

[S54] C++：异常处理
来源：http://czz.nwbrower.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tpw.bjfxy.top

[S55] C++：结构化绑定
来源：http://awj.c1oappe.top

auto [a, b] = std::make_pair(1, 2);
来源：http://uxl.yanxiufei.cn

[S56] C++：optional
来源：http://lid.pycfn.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://htv.shanyushiyangtech.top

[S57] C++：编译期常量
来源：http://voz.mhx1999.top

constexpr int N = 10;
来源：http://cfl.sxryk.cn

[S58] C++：命名空间
来源：http://xun.wangdashe.top

namespace ns { int f() { return 1; } }
来源：http://spb.nanxinkj.top

[S59] C++：静态断言
来源：http://fzx.cheryme.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ire.yueranfly.top

[S60] C++：遍历并删除元素
来源：http://pgr.cucudq.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zhe.hfpthk.cn

================================================================================
来源：http://cbc.iojbl.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nqp.kuanghao11.cn

================================================================================
来源：http://tkr.jqgfzy.top

[T01] Kotlin：Hello World
来源：http://hgn.dianchejie.cn

println("Hello")
来源：http://iup.jinqigfzy.top

[T02] Kotlin：变量
来源：http://vpl.zhiwuduotai.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hti.hcnkem.com

[T03] Kotlin：字符串模板
来源：http://jdd.cheryme.top

"值: $b"
来源：http://ulv.sjlbkw.cn

[T04] Kotlin：空安全
来源：http://olz.dianchejie.cn

val n: String? = null;  n?.length
来源：http://sia.jyoumei.cn

[T05] Kotlin：when 表达式
来源：http://pwv.cdnleiting.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xui.wangshuangyany.cn

[T06] Kotlin：集合映射
来源：http://bsz.cdnleiting.top

listOf(1, 2, 3).map { it * 2 }
来源：http://gtj.yj202588.top

[T07] Kotlin：集合过滤
来源：http://usq.vqdsnc.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ejn.yonumen.top

[T08] Kotlin：数据类
来源：http://hzw.zdqjudy.top

data class User(val name: String, val age: Int)
来源：http://hbi.fktsv.cn

[T09] Kotlin：扩展函数
来源：http://fcl.gaohongyu789.top

fun String.exclaim() = this + "!"
来源：http://fcv.zdqjudy.top

[T10] Kotlin：默认参数
来源：http://gft.quarkkingdee.top

fun greet(name: String = "World") = "Hi $name"
来源：http://tet.shanyushiyangkeji.top

[T11] Kotlin：协程
来源：http://qvo.chenjidiqi.icu

GlobalScope.launch { delay(1000); println("done") }
来源：http://vef.jinyuanbaomall.cn

[T12] Kotlin：解构声明
来源：http://mrl.sweek.top

val (a, b) = Pair(1, 2)
来源：http://yst.cashguo.top

[T13] Kotlin：只读 Map
来源：http://rgb.ivvv.top

val m = mapOf("a" to 1)
来源：http://efs.iojbl.cn

[T14] Kotlin：循环
来源：http://jah.ybcxt.top

for (i in 1..10) println(i)
来源：http://vmv.fktsv.cn

[T15] Kotlin：接口
来源：http://yhi.yvedp.cn

interface Shape { fun area(): Double }
来源：http://kum.uphjek.com

[T16] Swift：Hello World
来源：http://umh.jyoumei.cn

print("Hello")
来源：http://cys.smart0.xyz

[T17] Swift：变量与常量
来源：http://roc.jiagoushi.top

var a = 1;  let b = 2
来源：http://red.fktsv.cn

[T18] Swift：字符串插值
来源：http://dox.yongpay.top

"值: \(b)"
来源：http://jho.shangyingyoupin.top

[T19] Swift：可选绑定
来源：http://mzp.pengpengdd.cyou

if let n = opt { print(n) }
来源：http://dwv.daria6918.cn

[T20] Swift：数组操作
来源：http://yeb.cqqwz.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nzd.yuanzhike.top

[T21] Swift：遍历
来源：http://oxd.52xcode.cn

for x in a { print(x) }
来源：http://dzy.hammf.cn

[T22] Swift：字典
来源：http://bff.52xcode.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ihb.yuanzhike.top

[T23] Swift：函数
来源：http://uoe.yonumen.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hqk.daria6918.cn

[T24] Swift：闭包
来源：http://nls.shanyushiyangkeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://izh.snrcjt.cn

[T25] Swift：结构体
来源：http://zcs.zhoulong.xyz

struct P { var x: Int }
来源：http://yuz.wangdashe.top

[T26] Swift：类与重写
来源：http://vxn.daria6918.cn

class A: Base { override func f() {} }
来源：http://rbh.hnxiangtu.top

[T27] Swift：错误处理
来源：http://tjs.yanxiufei.cn

do { try f() } catch { print(error) }
来源：http://rox.yonumen.top

[T28] Swift：枚举
来源：http://wmh.guowangkeji.top

enum Color { case red, green }
来源：http://qnc.zdbjq.cn

[T29] Swift：guard 提前返回
来源：http://faj.shuidangran.top

guard let x = opt else { return }
来源：http://gyc.ybcxt.top

[T30] Swift：协议
来源：http://vhy.yangfankeji.com

protocol Shape { func area() -> Double }
来源：http://isu.gaohongyu789.top

[T31] Lua：Hello World
来源：http://hww.jyoumei.cn

print("Hello")
来源：http://smt.andypj.xyz

[T32] Lua：局部变量
来源：http://qjr.cucudq.cn

local a = 1
来源：http://ouw.daxiang520.top

[T33] Lua：表（数组）
来源：http://ygf.ehwqpu.com

local t = {1, 2, 3};  t[4] = 4
来源：http://nch.ydjk.org.cn

[T34] Lua：遍历表
来源：http://alr.hnqzz.top

for i, v in ipairs(t) do print(i, v) end
来源：http://mgk.yuxming.cn

[T35] Lua：字典表
来源：http://xrd.jyoumei.cn

local d = { a = 1 };  d.b = 2
来源：http://rxh.chenlongwang.top

[T36] Lua：函数
来源：http://evm.epnwcf.com

function add(a, b) return a + b end
来源：http://dcg.ywan-chungtsiang.top

[T37] Lua：字符串拼接
来源：http://rwl.xziqi.cn

"a" .. "b"
来源：http://pqq.havefunace.top

[T38] Lua：条件
来源：http://omp.aizwys.cn

if x > 0 then print("正") end
来源：http://dst.zhiwuduotai.top

[T39] Lua：模式匹配
来源：http://isd.jqgfzy.top

string.find(s, "%d+")
来源：http://oyt.jianghu66.top

[T40] Lua：元表
来源：http://kuz.sufxvd.cn

setmetatable({}, { __index = base })
来源：http://kfl.andypj.xyz

[T41] Perl：Hello World
来源：http://dfg.shuidangran.top

print "Hello\n";
来源：http://ozl.hysaishi.cn

[T42] Perl：变量类型
来源：http://gmz.chenlongwang.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://noc.zhijiandao.cn

[T43] Perl：字符串插值
来源：http://xof.yfazqb.com

"值: $a"
来源：http://kuj.fzhhl.top

[T44] Perl：条件
来源：http://cbk.daria6918.cn

if ($a > 0) { print "正"; }
来源：http://rre.yanxiufei.cn

[T45] Perl：数组遍历
来源：http://gdm.nwbrower.top

for my $x (@arr) { print $x; }
来源：http://ztz.quarkkingdee.top

[T46] Perl：哈希操作
来源：http://xxp.sxryk.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wnz.gotoacloud.top

[T47] Perl：正则捕获
来源：http://moc.fzhhl.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://dum.xuetiantiany.cn

[T48] Perl：正则替换
来源：http://hsy.shzxlz.cn

$s =~ s/old/new/g;
来源：http://sjo.cucudq.cn

[T49] Perl：函数
来源：http://okc.xuetiantiany.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zwx.wangshuangyany.cn

[T50] Perl：逐行读文件
来源：http://rsi.yvedp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rzt.xziqi.cn

while (my $line = <$fh>) { print $line; }
来源：http://atx.cdnleiting.top

[T51] Scala：Hello World
来源：http://gkr.meibo888.top

println("Hello")
来源：http://jiy.hammf.cn

[T52] Scala：变量
来源：http://xfe.zhaomingkeji.xyz

val a = 1;  var b = 2
来源：http://mbj.jinqigfzy.top

[T53] Scala：字符串插值
来源：http://oub.ybcxt.top

s"值: $b"
来源：http://ukg.bbcook.cn

[T54] Scala：集合映射
来源：http://ofs.xingfuxueyuan.xyz

List(1, 2, 3).map(_ * 2)
来源：http://vmi.fanxiaobao.xyz

[T55] Scala：集合过滤
来源：http://cup.daxiang520.top

List(1, 2, 3).filter(_ > 1)
来源：http://khh.shanyushiyangkeji.top

[T56] Scala：样例类
来源：http://pai.xuanzx.com

case class User(name: String, age: Int)
来源：http://mxk.jinghuilouyu.cn

[T57] Scala：模式匹配
来源：http://xgz.jinqigufen.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ggq.fzhhl.top

[T58] Scala：函数定义
来源：http://dpm.tianlin.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://elw.cucudq.cn

[T59] Scala：循环
来源：http://bvr.jqgufenzy.top

for (i <- 1 to 10) println(i)
来源：http://hxo.fktsv.cn

[T60] Scala：折叠
来源：http://nlb.redwolf501.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dqd.jinghuilouyu.cn

================================================================================
来源：http://emk.chenjidiqi.icu

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rtk.zhaomingkeji.xyz

================================================================================
来源：http://kqh.tian-w.cn

[U01] Py：创建虚拟环境
来源：http://wxg.iojbl.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cra.quarkkingdee.top

[U02] Py：导出 / 安装依赖
来源：http://elk.9152youxi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yzq.0kj1m.cn

[U03] Py：加载 .env 配置
来源：http://tli.yueranfly.top

from dotenv import load_dotenv; load_dotenv()
来源：http://knd.nanxinkj.top

[U04] Py：变量调试打印
来源：http://xbe.smart0.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gdz.zhixingplan.top

[U05] Py：列表去重且保序
来源：http://pns.yuxming.cn

list(dict.fromkeys(arr))
来源：http://zeo.ctjpmb.com

[U06] Py：合并两个字典
来源：http://mvv.fanxiaobao.xyz

{**a, **b}
来源：http://zvw.yvedp.cn

[U07] Py：反转字典键值
来源：http://hnv.birdmap.top

{v: k for k, v in d.items()}
来源：http://uvc.tanke756.top

[U08] Py：展平二维列表
来源：http://iyq.redwolf501.top

[y for x in nested for y in x]
来源：http://eqq.gotoacloud.top

[U09] Py：字典取最大值的键
来源：http://mat.jqgfzy.top

max(d, key=d.get)
来源：http://vlg.yj20258.top

[U10] Py：按值排序字典
来源：http://gmo.sweek.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://icj.shanyushiyangtech.top

[U11] Py：生成器表达式
来源：http://cgw.ydjk.org.cn

(x * 2 for x in arr)
来源：http://uzj.daxiang520.top

[U12] Py：取出现最多的 3 个元素
来源：http://krc.zhoulong.xyz

Counter(arr).most_common(3)
来源：http://kad.uphjek.com

[U13] Py：固定长度队列
来源：http://vev.zhijiandao.cn

deque(maxlen=10)
来源：http://rwx.jinyuanbaomall.cn

[U14] Py：分组收集到列表
来源：http://gst.wangdashe.top

defaultdict(list)
来源：http://wve.jiagoushi.top

[U15] Py：高精度计时
来源：http://uws.pycfn.com

t = time.perf_counter()
来源：http://mco.pengpengdd.cyou

[U16] Py：命令行参数解析
来源：http://zeq.uphjek.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vgf.cdnleiting.top

[U17] Py：初始化日志
来源：http://sdh.ppjwa.cn

logging.basicConfig(level=logging.INFO)
来源：http://pbr.yj20258.top

[U18] Py：预编译正则
来源：http://hqw.yangfankeji.com

pat = re.compile(r"\d+")
来源：http://lrs.hywenlv.cn

[U19] Py：正则替换带回调
来源：http://lch.nanxuanxn.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://flg.shanyushiyangtech.top

[U20] Py：缓存函数结果
来源：http://vei.ppjwa.cn

@functools.lru_cache(maxsize=None)
来源：http://ebn.fktsv.cn

[U21] Py：自定义上下文管理器
来源：http://tmp.shuidangran.top

@contextlib.contextmanager
来源：http://jio.fktsv.cn

[U22] Py：矩阵转置
来源：http://fag.jianghu66.top

list(zip(*m))
来源：http://kkw.jqgfzy.top

[U23] Py：分块读取大文件
来源：http://dsy.sxryk.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kyb.daria6918.cn

[U24] Py：路径操作
来源：http://dfp.yonumen.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ycx.jinghuilouyu.cn

[U25] Py：CSV 按字典读
来源：http://jwt.birdmap.top

csv.DictReader(f)
来源：http://vnq.ywan-chungtsiang.top

[U26] Py：并发下载
来源：http://vqi.bjfxy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gwx.iojbl.cn

[U27] Py：异步 HTTP
来源：http://cfa.daxiang520.top

aiohttp.ClientSession() 配合 async with
来源：http://zat.gogol.net.cn

[U28] Py：类型别名
来源：http://slf.svipenyu.cn

UserId = int
来源：http://wce.quarkkingdee.top

[U29] Py：属性校验
来源：http://ick.redwolf501.top

@property 与 @x.setter 配合
来源：http://yyi.jlsjyb.cn

[U30] Py：数据类
来源：http://qlb.shuidangran.top

@dataclass(slots=True)
来源：http://ywb.xuanzx.com

[U31] Py：单测
来源：http://zmi.snrcjt.cn

python -m pytest -q
来源：http://ivk.birdmap.top

[U32] Py：代码格式化
来源：http://ryh.cqqwz.cn

ruff format . && ruff check --fix .
来源：http://ujq.yfazqb.com


<!-- 参考信息 -->