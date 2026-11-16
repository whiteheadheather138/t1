代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://irc.yueranfly.top

[S10] C：指针与解引用
来源：http://tjd.jinqigfzy.top

int *p = &a;  *p = 5;
来源：http://xkg.yueranfly.top

[S11] C：逐行读文件
来源：http://lyo.yvedp.cn

FILE *f = fopen("a.txt", "r");
来源：http://eoz.yanxiufei.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://czp.ydjk.org.cn

fclose(f);
来源：http://ola.xziqi.cn

[S12] C：写文件
来源：http://kca.hnxiangtu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yuz.sxryk.cn

[S13] C：宏定义
来源：http://sch.0kj1m.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tce.guannengcc.top

[S14] C：枚举
来源：http://bpq.havefunace.top

enum Color { RED, GREEN, BLUE };
来源：http://vmc.hammf.cn

[S15] C：类型转换
来源：http://ysy.xylfe.cn

(double) a / b
来源：http://eym.nanxuanxn.top

[S16] C：位操作置位
来源：http://yue.xingfuxueyuan.xyz

x |= (1 << 3);
来源：http://shr.316326.xyz

[S17] C：安全拼接字符串
来源：http://ycs.nwbrower.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fzf.shanyushiyangtech.top

[S18] C：命令行参数
来源：http://mnt.daria6918.cn

int main(int argc, char **argv)
来源：http://wuc.guannengcc.top

[S19] C：快速排序
来源：http://smt.c1oappe.top

qsort(a, n, sizeof(int), cmp);
来源：http://nya.tian-w.cn

[S20] C：二分查找
来源：http://mji.fktsv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ocw.jyoumei.cn

[S21] C：字符类别判断
来源：http://gzd.birdmap.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rpa.epnwcf.com

[S22] C：字符串转数字
来源：http://oft.birdmap.top

atoi("42");  strtod("3.14", NULL);
来源：http://fhl.haohaochexian.top

[S23] C：随机数
来源：http://ipq.shangyingyoupin.top

srand(time(NULL));  int r = rand() % 100;
来源：http://wjj.aizwys.cn

[S24] C：获取本地时间
来源：http://zrb.iojbl.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jbe.andypj.xyz

[S25] C：内存拷贝
来源：http://bpy.ehwqpu.com

memcpy(dst, src, n);
来源：http://box.gotoacloud.top

[S26] C：内存清零
来源：http://xna.zhijiandao.cn

memset(a, 0, sizeof a);
来源：http://mgd.sweek.top

[S27] C：定义常量
来源：http://fip.c1oappe.top

const double PI = 3.14159;
来源：http://vdi.ctjpmb.com

[S28] C：静态变量
来源：http://zxn.birdmap.top

static int counter = 0;
来源：http://dxi.jinqigufen.top

[S29] C：变参函数
来源：http://uzc.cheryme.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vsr.fktsv.cn

[S30] C：头文件保护
来源：http://raf.bbcook.cn

#ifndef X_H
来源：http://goz.jqgufenzy.top

#define X_H
来源：http://luu.ctjpmb.com

#endif
来源：http://yqx.tarul.cn

[S31] C++：Hello World
来源：http://slq.xziqi.cn

#include <iostream>
来源：http://nof.jinqigufen.top

int main() { std::cout << "Hello\n"; }
来源：http://cxm.fktsv.cn

[S32] C++：字符串
来源：http://del.gotoacloud.top

std::string s = "hi";  s += "!";
来源：http://ztm.hnxiangtu.top

[S33] C++：vector 增删
来源：http://exq.cheryme.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eqo.cheryme.top

[S34] C++：遍历 vector
来源：http://fqz.yvedp.cn

for (auto &x : v) { std::cout << x; }
来源：http://kvq.xuetiantiany.cn

[S35] C++：map
来源：http://eqj.jinghuilouyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zku.hysaishi.cn

[S36] C++：unordered_map
来源：http://qkc.epnwcf.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ggw.bbcook.cn

[S37] C++：set
来源：http://ryh.shzxlz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pph.0kj1m.cn

[S38] C++：排序
来源：http://jst.yuxming.cn

std::sort(v.begin(), v.end());
来源：http://brd.gzhubu.top

[S39] C++：自定义比较器排序
来源：http://edr.c1oappe.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fyn.ehwqpu.com

[S40] C++：查找元素
来源：http://nxs.wangdashe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lxv.hammf.cn

[S41] C++：类与构造函数
来源：http://xys.xingfuxueyuan.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ayt.zhiwuduotai.top

[S42] C++：继承与虚函数
来源：http://eoa.ydzc1.top

class B : public Base { public: void f() override {} };
来源：http://teu.yueranfly.top

[S43] C++：智能指针
来源：http://awn.hysaishi.cn

auto p = std::make_unique<int>(5);
来源：http://dgp.hnxiangtu.top

[S44] C++：引用传参
来源：http://tbd.ctjpmb.com

void inc(int &x) { ++x; }
来源：http://xxx.zycfv.cn

[S45] C++：lambda
来源：http://bwx.uphjek.com

auto add = [](int a, int b) { return a + b; };
来源：http://eck.hywenlv.cn

[S46] C++：函数模板
来源：http://ntq.ctjpmb.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gst.jinghuilouyu.cn

[S47] C++：结构化绑定遍历
来源：http://cfo.dashuyun.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mbx.yfazqb.com

[S48] C++：逐行读文件
来源：http://idu.c1oappe.top

std::ifstream in("a.txt");  std::string line;
来源：http://vtj.gaohongyu789.top

while (std::getline(in, line)) { }
来源：http://scj.wangdashe.top

[S49] C++：写文件
来源：http://drl.shuidangran.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zri.jinyuanbaomall.cn

[S50] C++：格式化数字
来源：http://wis.zhixingplan.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ggz.feifeiyinyue.top

[S51] C++：显式类型转换
来源：http://qth.ivvv.top

static_cast<double>(a) / b
来源：http://wyz.xziqi.cn

[S52] C++：const 与 noexcept
来源：http://pry.feifeiyinyue.top

int size() const noexcept { return n_; }
来源：http://jjc.tanke756.top

[S53] C++：移动语义
来源：http://svd.sweek.top

std::vector<int> w = std::move(v);
来源：http://fxr.gaohongyu789.top

[S54] C++：异常处理
来源：http://chr.hysaishi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ttk.cqqwz.cn

[S55] C++：结构化绑定
来源：http://mmx.pengpengdd.cyou

auto [a, b] = std::make_pair(1, 2);
来源：http://kae.yfazqb.com

[S56] C++：optional
来源：http://sxg.zhaomingkeji.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vwn.ivvv.top

[S57] C++：编译期常量
来源：http://fhm.chenlongwang.top

constexpr int N = 10;
来源：http://mbf.snrcjt.cn

[S58] C++：命名空间
来源：http://rcc.daxiang520.top

namespace ns { int f() { return 1; } }
来源：http://hil.fktsv.cn

[S59] C++：静态断言
来源：http://zxc.dashuyun.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mjr.jinqigufen.top

[S60] C++：遍历并删除元素
来源：http://cvn.chenzaomai.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://iuh.svipenyu.cn

================================================================================
来源：http://uxq.yonumen.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vjx.snrcjt.cn

================================================================================
来源：http://wtc.ydzc1.top

[T01] Kotlin：Hello World
来源：http://tpg.jianghu66.top

println("Hello")
来源：http://hdy.ywan-chungtsiang.top

[T02] Kotlin：变量
来源：http://mbl.sysykeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vpy.havefunace.top

[T03] Kotlin：字符串模板
来源：http://cxk.sxryk.cn

"值: $b"
来源：http://sfn.iojbl.cn

[T04] Kotlin：空安全
来源：http://ihm.guannengcc.top

val n: String? = null;  n?.length
来源：http://ycm.hesvh.cn

[T05] Kotlin：when 表达式
来源：http://scr.ywan-chungtsiang.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hck.nanxinkj.top

[T06] Kotlin：集合映射
来源：http://piy.jqgufenzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://plg.yonumen.top

[T07] Kotlin：集合过滤
来源：http://vcd.shanyushiyangtech.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://iyx.zdqjudy.top

[T08] Kotlin：数据类
来源：http://zlh.yuxming.cn

data class User(val name: String, val age: Int)
来源：http://dyk.yanxiufei.cn

[T09] Kotlin：扩展函数
来源：http://bnp.hammf.cn

fun String.exclaim() = this + "!"
来源：http://xhi.xuanzx.com

[T10] Kotlin：默认参数
来源：http://bcz.cqqwz.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://opx.dashuyun.cn

[T11] Kotlin：协程
来源：http://ijd.feifeiyinyue.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://vxw.redwolf501.top

[T12] Kotlin：解构声明
来源：http://wrh.cqqwz.cn

val (a, b) = Pair(1, 2)
来源：http://wxv.havefunace.top

[T13] Kotlin：只读 Map
来源：http://hbx.tianlin.xyz

val m = mapOf("a" to 1)
来源：http://uaa.yangfankeji.com

[T14] Kotlin：循环
来源：http://dcw.ctjpmb.com

for (i in 1..10) println(i)
来源：http://sqb.uphjek.com

[T15] Kotlin：接口
来源：http://wxj.yj20258888.top

interface Shape { fun area(): Double }
来源：http://qao.mhx1999.top

[T16] Swift：Hello World
来源：http://tvp.dashuyun.cn

print("Hello")
来源：http://hvn.cheryme.top

[T17] Swift：变量与常量
来源：http://mxr.uphjek.com

var a = 1;  let b = 2
来源：http://ibl.snrcjt.cn

[T18] Swift：字符串插值
来源：http://jnp.pycfn.com

"值: \(b)"
来源：http://ywl.haohaochexian.top

[T19] Swift：可选绑定
来源：http://vxl.xziqi.cn

if let n = opt { print(n) }
来源：http://qpb.tian-w.cn

[T20] Swift：数组操作
来源：http://zwu.yj20258.top

var a = [1, 2, 3];  a.append(4)
来源：http://eip.c1oappe.top

[T21] Swift：遍历
来源：http://hgn.guannengcc.top

for x in a { print(x) }
来源：http://mca.guowangkeji.top

[T22] Swift：字典
来源：http://rky.shangyingyoupin.top

var d = ["a": 1];  d["b"] = 2
来源：http://dpu.xziqi.cn

[T23] Swift：函数
来源：http://hmy.zdqjudy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uhw.dianchejie.cn

[T24] Swift：闭包
来源：http://nyt.gotoacloud.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://zjc.cheryme.top

[T25] Swift：结构体
来源：http://vxp.ybcxt.top

struct P { var x: Int }
来源：http://elf.hongshengwenyu.top

[T26] Swift：类与重写
来源：http://oyz.jqgfzy.top

class A: Base { override func f() {} }
来源：http://yrk.xingfuxueyuan.xyz

[T27] Swift：错误处理
来源：http://fic.shanyushiyangkeji.top

do { try f() } catch { print(error) }
来源：http://icf.andypj.xyz

[T28] Swift：枚举
来源：http://mgx.zycfv.cn

enum Color { case red, green }
来源：http://ueb.tianlin.xyz

[T29] Swift：guard 提前返回
来源：http://vpa.yj20258888.top

guard let x = opt else { return }
来源：http://yod.tarul.cn

[T30] Swift：协议
来源：http://day.yj20258.top

protocol Shape { func area() -> Double }
来源：http://oeb.52xcode.cn

[T31] Lua：Hello World
来源：http://ihq.daria6918.cn

print("Hello")
来源：http://une.bjfxy.top

[T32] Lua：局部变量
来源：http://jxo.nanxuanxn.top

local a = 1
来源：http://gyi.0kj1m.cn

[T33] Lua：表（数组）
来源：http://suf.chenjidiqi.icu

local t = {1, 2, 3};  t[4] = 4
来源：http://haw.epnwcf.com

[T34] Lua：遍历表
来源：http://bms.dianchejie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dnd.chenjidiqi.icu

[T35] Lua：字典表
来源：http://tzf.shangyingyoupin.top

local d = { a = 1 };  d.b = 2
来源：http://tjc.hesvh.cn

[T36] Lua：函数
来源：http://fvc.xylfe.cn

function add(a, b) return a + b end
来源：http://dsa.nanxuanxn.top

[T37] Lua：字符串拼接
来源：http://ngt.jqgfzy.top

"a" .. "b"
来源：http://ozl.xinyue.icu

[T38] Lua：条件
来源：http://dlo.jyoumei.cn

if x > 0 then print("正") end
来源：http://vvu.jiagoushi.top

[T39] Lua：模式匹配
来源：http://wub.ctjpmb.com

string.find(s, "%d+")
来源：http://rmz.dashuyun.cn

[T40] Lua：元表
来源：http://wpx.zhixingplan.top

setmetatable({}, { __index = base })
来源：http://bpn.dianchejie.cn

[T41] Perl：Hello World
来源：http://kza.gogol.net.cn

print "Hello\n";
来源：http://gqq.uphjek.com

[T42] Perl：变量类型
来源：http://drd.hywenlv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kmi.chenjidiqi.icu

[T43] Perl：字符串插值
来源：http://gjn.chenzaomai.com

"值: $a"
来源：http://jsr.9152youxi.cn

[T44] Perl：条件
来源：http://paf.chenlongwang.top

if ($a > 0) { print "正"; }
来源：http://vcn.zdbjq.cn

[T45] Perl：数组遍历
来源：http://xup.fehbvm.com

for my $x (@arr) { print $x; }
来源：http://ntj.xuetiantiany.cn

[T46] Perl：哈希操作
来源：http://pto.cucudq.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://awv.svipenyu.cn

[T47] Perl：正则捕获
来源：http://uys.zycfv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vpk.xuanzx.com

[T48] Perl：正则替换
来源：http://nzj.shangyingyoupin.top

$s =~ s/old/new/g;
来源：http://plt.guowangkeji.top

[T49] Perl：函数
来源：http://ysf.bjfxy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zvx.zhixingplan.top

[T50] Perl：逐行读文件
来源：http://ufy.9152youxi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ncc.hnxiangtu.top

while (my $line = <$fh>) { print $line; }
来源：http://emv.guannengcc.top

[T51] Scala：Hello World
来源：http://fjr.jinqigfzy.top

println("Hello")
来源：http://pfc.mhx1999.top

[T52] Scala：变量
来源：http://aae.smart0.xyz

val a = 1;  var b = 2
来源：http://tbl.andypj.xyz

[T53] Scala：字符串插值
来源：http://vhk.jiagoushi.top

s"值: $b"
来源：http://ypc.fzhhl.top

[T54] Scala：集合映射
来源：http://oox.ywan-chungtsiang.top

List(1, 2, 3).map(_ * 2)
来源：http://hzg.zhengqikj.top

[T55] Scala：集合过滤
来源：http://xlv.xinyue.icu

List(1, 2, 3).filter(_ > 1)
来源：http://qfv.yuxming.cn

[T56] Scala：样例类
来源：http://xoi.zhijiandao.cn

case class User(name: String, age: Int)
来源：http://nnb.yuxming.cn

[T57] Scala：模式匹配
来源：http://hlh.vehdjk.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://dhj.jlsjyb.cn

[T58] Scala：函数定义
来源：http://jqy.xuanzx.com

def add(a: Int, b: Int): Int = a + b
来源：http://qqv.haohaochexian.top

[T59] Scala：循环
来源：http://tzg.svipenyu.cn

for (i <- 1 to 10) println(i)
来源：http://kbr.sxryk.cn

[T60] Scala：折叠
来源：http://fcz.chenlongwang.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://svz.bbcook.cn

================================================================================
来源：http://jgk.guannengcc.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://knb.yj202588.top

================================================================================
来源：http://vqb.jianghu66.top

[U01] Py：创建虚拟环境
来源：http://vfv.hammf.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mqk.zdbjq.cn

[U02] Py：导出 / 安装依赖
来源：http://rhh.cashguo.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xea.yj20258888.top

[U03] Py：加载 .env 配置
来源：http://lkx.ybcxt.top

from dotenv import load_dotenv; load_dotenv()
来源：http://dzr.hnxiangtu.top

[U04] Py：变量调试打印
来源：http://mlf.sweek.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bza.hnqzz.top

[U05] Py：列表去重且保序
来源：http://xzl.zhiwuduotai.top

list(dict.fromkeys(arr))
来源：http://gag.yfazqb.com

[U06] Py：合并两个字典
来源：http://tvv.52xcode.cn

{**a, **b}
来源：http://jyb.yuxming.cn

[U07] Py：反转字典键值
来源：http://emy.dianchejie.cn

{v: k for k, v in d.items()}
来源：http://jos.yfazqb.com

[U08] Py：展平二维列表
来源：http://blv.yonumen.top

[y for x in nested for y in x]
来源：http://tik.ywan-chungtsiang.top

[U09] Py：字典取最大值的键
来源：http://dga.daxiang520.top

max(d, key=d.get)
来源：http://bqi.zhengqikj.top

[U10] Py：按值排序字典
来源：http://tdn.nanxuanxn.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cup.hongshengwenyu.top

[U11] Py：生成器表达式
来源：http://ftu.c1oappe.top

(x * 2 for x in arr)
来源：http://bte.xuetiantiany.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rts.birdmap.top

Counter(arr).most_common(3)
来源：http://fih.aibaodan.cn

[U13] Py：固定长度队列
来源：http://lin.yongpay.top

deque(maxlen=10)
来源：http://qpr.hfpthk.cn

[U14] Py：分组收集到列表
来源：http://bwl.yj20258888.top

defaultdict(list)
来源：http://opc.yuxming.cn

[U15] Py：高精度计时
来源：http://dvy.52xcode.cn

t = time.perf_counter()
来源：http://qhk.vehdjk.com

[U16] Py：命令行参数解析
来源：http://zcv.wangshuangyany.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mex.yuanzhike.top

[U17] Py：初始化日志
来源：http://eju.haohaochexian.top

logging.basicConfig(level=logging.INFO)
来源：http://aus.yuanzhike.top

[U18] Py：预编译正则
来源：http://qbt.jinqigufen.top

pat = re.compile(r"\d+")
来源：http://jfy.svipenyu.cn

[U19] Py：正则替换带回调
来源：http://ofx.birdmap.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tsw.tanke756.top

[U20] Py：缓存函数结果
来源：http://bwx.redwolf501.top

@functools.lru_cache(maxsize=None)
来源：http://gey.hywenlv.cn

[U21] Py：自定义上下文管理器
来源：http://ygu.zhongyouzk.top

@contextlib.contextmanager
来源：http://lyu.zhixingplan.top

[U22] Py：矩阵转置
来源：http://xyj.iojbl.cn

list(zip(*m))
来源：http://dfh.hywenlv.cn

[U23] Py：分块读取大文件
来源：http://fwd.xziqi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://igy.zhiwuduotai.top

[U24] Py：路径操作
来源：http://tov.cdnleiting.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wgn.c1oappe.top

[U25] Py：CSV 按字典读
来源：http://nhe.ivvv.top

csv.DictReader(f)
来源：http://aiv.gaohongyu789.top

[U26] Py：并发下载
来源：http://idf.xinyue.icu

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jga.daria6918.cn

[U27] Py：异步 HTTP
来源：http://okd.hammf.cn

aiohttp.ClientSession() 配合 async with
来源：http://xde.shangyingyoupin.top

[U28] Py：类型别名
来源：http://gio.kuanghao11.cn

UserId = int
来源：http://xhk.tian-w.cn

[U29] Py：属性校验
来源：http://rqn.zhixingplan.top

@property 与 @x.setter 配合
来源：http://zus.xuanzx.com

[U30] Py：数据类
来源：http://lff.feifeiyinyue.top

@dataclass(slots=True)
来源：http://eka.kuanghao11.cn

[U31] Py：单测
来源：http://qtt.jyoumei.cn

python -m pytest -q
来源：http://dsc.c1oappe.top

[U32] Py：代码格式化
来源：http://xax.tarul.cn

ruff format . && ruff check --fix .
来源：http://roo.tian-w.cn


<!-- 参考信息 -->