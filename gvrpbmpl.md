代发 wailian999

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lwb.aizwys.cn

[S10] C：指针与解引用
来源：http://vlu.ctjpmb.com

int *p = &a;  *p = 5;
来源：http://uww.zdqjudy.top

[S11] C：逐行读文件
来源：http://gnz.jinqigfzy.top

FILE *f = fopen("a.txt", "r");
来源：http://wvm.svipenyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://frj.chenzaomai.com

fclose(f);
来源：http://qjo.aizwys.cn

[S12] C：写文件
来源：http://pun.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mly.sufxvd.cn

[S13] C：宏定义
来源：http://bju.andypj.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xxv.ehwqpu.com

[S14] C：枚举
来源：http://xhj.aibaodan.cn

enum Color { RED, GREEN, BLUE };
来源：http://jxz.aizwys.cn

[S15] C：类型转换
来源：http://rbp.zdqjudy.top

(double) a / b
来源：http://ano.dashuyun.cn

[S16] C：位操作置位
来源：http://wct.zhongyouzk.top

x |= (1 << 3);
来源：http://dju.9152youxi.cn

[S17] C：安全拼接字符串
来源：http://zjr.xingfuxueyuan.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://csy.jinghuilouyu.cn

[S18] C：命令行参数
来源：http://wdt.zhoulong.xyz

int main(int argc, char **argv)
来源：http://lks.sjlbkw.cn

[S19] C：快速排序
来源：http://wmx.tarul.cn

qsort(a, n, sizeof(int), cmp);
来源：http://czv.jianghu66.top

[S20] C：二分查找
来源：http://dgo.zhixingplan.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xyc.uphjek.com

[S21] C：字符类别判断
来源：http://fqo.ybcxt.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tic.xuetiantiany.cn

[S22] C：字符串转数字
来源：http://dhm.gotoacloud.top

atoi("42");  strtod("3.14", NULL);
来源：http://lct.iojbl.cn

[S23] C：随机数
来源：http://fls.ybcxt.top

srand(time(NULL));  int r = rand() % 100;
来源：http://lpm.jqgfzy.top

[S24] C：获取本地时间
来源：http://stc.sweek.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uqv.nanxuanxn.top

[S25] C：内存拷贝
来源：http://gvm.chenjidiqi.icu

memcpy(dst, src, n);
来源：http://bob.shanyushiyangtech.top

[S26] C：内存清零
来源：http://eoy.birdmap.top

memset(a, 0, sizeof a);
来源：http://zzo.quarkkingdee.top

[S27] C：定义常量
来源：http://hld.0kj1m.cn

const double PI = 3.14159;
来源：http://tzr.jqgfzy.top

[S28] C：静态变量
来源：http://gzn.hysaishi.cn

static int counter = 0;
来源：http://hhq.zhongyouzk.top

[S29] C：变参函数
来源：http://tfw.smart0.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lha.guannengcc.top

[S30] C：头文件保护
来源：http://tdr.sysykeji.top

#ifndef X_H
来源：http://sgu.cqqwz.cn

#define X_H
来源：http://bso.jinyuanbaomall.cn

#endif
来源：http://doc.fktsv.cn

[S31] C++：Hello World
来源：http://spp.shzxlz.cn

#include <iostream>
来源：http://tpl.bbcook.cn

int main() { std::cout << "Hello\n"; }
来源：http://ktj.snrcjt.cn

[S32] C++：字符串
来源：http://qei.hongshengwenyu.top

std::string s = "hi";  s += "!";
来源：http://baz.cqqwz.cn

[S33] C++：vector 增删
来源：http://kmv.pengpengdd.cyou

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xwi.zdbjq.cn

[S34] C++：遍历 vector
来源：http://qxt.chenzaomai.com

for (auto &x : v) { std::cout << x; }
来源：http://vmj.xziqi.cn

[S35] C++：map
来源：http://dpz.bbcook.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://whh.sxryk.cn

[S36] C++：unordered_map
来源：http://icc.yuanzhike.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zxp.gzhubu.top

[S37] C++：set
来源：http://jri.0kj1m.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oep.yangfankeji.com

[S38] C++：排序
来源：http://qjf.nwbrower.top

std::sort(v.begin(), v.end());
来源：http://jpt.zdqjudy.top

[S39] C++：自定义比较器排序
来源：http://nbi.sysykeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xqh.9152youxi.cn

[S40] C++：查找元素
来源：http://wvh.snrcjt.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cdf.hcnkem.com

[S41] C++：类与构造函数
来源：http://wsq.xingfuxueyuan.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mru.ywan-chungtsiang.top

[S42] C++：继承与虚函数
来源：http://jlr.birdmap.top

class B : public Base { public: void f() override {} };
来源：http://hrl.cucudq.cn

[S43] C++：智能指针
来源：http://zfg.hcnkem.com

auto p = std::make_unique<int>(5);
来源：http://jmq.ydzc1.top

[S44] C++：引用传参
来源：http://bju.fzhhl.top

void inc(int &x) { ++x; }
来源：http://fkf.0kj1m.cn

[S45] C++：lambda
来源：http://mhj.tian-w.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jfk.zhijiandao.cn

[S46] C++：函数模板
来源：http://ozv.xuanzx.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sxi.ywan-chungtsiang.top

[S47] C++：结构化绑定遍历
来源：http://jor.daria6918.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tcj.chenzaomai.com

[S48] C++：逐行读文件
来源：http://zty.hcnkem.com

std::ifstream in("a.txt");  std::string line;
来源：http://lgl.ywan-chungtsiang.top

while (std::getline(in, line)) { }
来源：http://swf.chenjidiqi.icu

[S49] C++：写文件
来源：http://rzx.xuanzx.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dwf.shuidangran.top

[S50] C++：格式化数字
来源：http://org.zhijiandao.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kue.yfazqb.com

[S51] C++：显式类型转换
来源：http://unt.zdqjudy.top

static_cast<double>(a) / b
来源：http://xod.zhengqikj.top

[S52] C++：const 与 noexcept
来源：http://bdg.xuanzx.com

int size() const noexcept { return n_; }
来源：http://ncu.xuetiantiany.cn

[S53] C++：移动语义
来源：http://alj.tianlin.xyz

std::vector<int> w = std::move(v);
来源：http://avl.fengsongda.top

[S54] C++：异常处理
来源：http://xva.jinqigufen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kky.shuidangran.top

[S55] C++：结构化绑定
来源：http://zem.zhaomingkeji.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://dph.jianghu66.top

[S56] C++：optional
来源：http://rlr.haohaochexian.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pkb.svipenyu.cn

[S57] C++：编译期常量
来源：http://efk.jinqigufen.top

constexpr int N = 10;
来源：http://kfo.wangdashe.top

[S58] C++：命名空间
来源：http://fqa.shuidangran.top

namespace ns { int f() { return 1; } }
来源：http://lon.tian-w.cn

[S59] C++：静态断言
来源：http://jvo.aibaodan.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://srw.fktsv.cn

[S60] C++：遍历并删除元素
来源：http://uin.redwolf501.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kzb.jqgufenzy.top

================================================================================
来源：http://jzx.yangfankeji.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uwc.sweek.top

================================================================================
来源：http://fpp.svipenyu.cn

[T01] Kotlin：Hello World
来源：http://djq.fanxiaobao.xyz

println("Hello")
来源：http://tmd.redwolf501.top

[T02] Kotlin：变量
来源：http://xhq.hywenlv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://usb.yueranfly.top

[T03] Kotlin：字符串模板
来源：http://flr.wangshuangyany.cn

"值: $b"
来源：http://fyf.sxryk.cn

[T04] Kotlin：空安全
来源：http://zfc.dianchejie.cn

val n: String? = null;  n?.length
来源：http://elk.chenlongwang.top

[T05] Kotlin：when 表达式
来源：http://wuy.yonumen.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gpm.ppjwa.cn

[T06] Kotlin：集合映射
来源：http://jwt.xylfe.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qyy.gotoacloud.top

[T07] Kotlin：集合过滤
来源：http://ois.andypj.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://xld.fktsv.cn

[T08] Kotlin：数据类
来源：http://ytc.hnxiangtu.top

data class User(val name: String, val age: Int)
来源：http://byp.guannengcc.top

[T09] Kotlin：扩展函数
来源：http://vlp.zhaomingkeji.xyz

fun String.exclaim() = this + "!"
来源：http://zcy.yuxming.cn

[T10] Kotlin：默认参数
来源：http://cnm.yj20258888.top

fun greet(name: String = "World") = "Hi $name"
来源：http://pah.c1oappe.top

[T11] Kotlin：协程
来源：http://ltv.jiagoushi.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gou.dianchejie.cn

[T12] Kotlin：解构声明
来源：http://gku.c1oappe.top

val (a, b) = Pair(1, 2)
来源：http://lyl.vehdjk.com

[T13] Kotlin：只读 Map
来源：http://wee.iojbl.cn

val m = mapOf("a" to 1)
来源：http://pgj.wangdashe.top

[T14] Kotlin：循环
来源：http://rha.iojbl.cn

for (i in 1..10) println(i)
来源：http://bul.daxiang520.top

[T15] Kotlin：接口
来源：http://ggm.vqdsnc.cn

interface Shape { fun area(): Double }
来源：http://dcs.xuanzx.com

[T16] Swift：Hello World
来源：http://myf.tianlin.xyz

print("Hello")
来源：http://jbr.bjfxy.top

[T17] Swift：变量与常量
来源：http://obj.xziqi.cn

var a = 1;  let b = 2
来源：http://amh.sysykeji.top

[T18] Swift：字符串插值
来源：http://nzh.fzhhl.top

"值: \(b)"
来源：http://bgl.jiagoushi.top

[T19] Swift：可选绑定
来源：http://ztp.jiagoushi.top

if let n = opt { print(n) }
来源：http://qhk.zdqjudy.top

[T20] Swift：数组操作
来源：http://lqz.nanxinkj.top

var a = [1, 2, 3];  a.append(4)
来源：http://usn.aibaodan.cn

[T21] Swift：遍历
来源：http://xqm.iojbl.cn

for x in a { print(x) }
来源：http://xip.iojbl.cn

[T22] Swift：字典
来源：http://khu.shanyushiyangtech.top

var d = ["a": 1];  d["b"] = 2
来源：http://wbl.zhixingplan.top

[T23] Swift：函数
来源：http://uhl.chenlongwang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ajl.52xcode.cn

[T24] Swift：闭包
来源：http://ond.jinqigfzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://zhq.shuidangran.top

[T25] Swift：结构体
来源：http://xov.uphjek.com

struct P { var x: Int }
来源：http://mcz.aizwys.cn

[T26] Swift：类与重写
来源：http://hkt.fktsv.cn

class A: Base { override func f() {} }
来源：http://ian.hnxiangtu.top

[T27] Swift：错误处理
来源：http://fzq.zhengqikj.top

do { try f() } catch { print(error) }
来源：http://xms.chenjidiqi.icu

[T28] Swift：枚举
来源：http://wtr.ywan-chungtsiang.top

enum Color { case red, green }
来源：http://cjl.hnqzz.top

[T29] Swift：guard 提前返回
来源：http://nqs.zhoulong.xyz

guard let x = opt else { return }
来源：http://ahu.yueranfly.top

[T30] Swift：协议
来源：http://sfp.gogol.net.cn

protocol Shape { func area() -> Double }
来源：http://klz.guowangkeji.top

[T31] Lua：Hello World
来源：http://gcc.tanke756.top

print("Hello")
来源：http://mzf.yuxming.cn

[T32] Lua：局部变量
来源：http://ytx.fengsongda.top

local a = 1
来源：http://urz.daxiang520.top

[T33] Lua：表（数组）
来源：http://tmu.52xcode.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ukp.sxryk.cn

[T34] Lua：遍历表
来源：http://qxa.smart0.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://iir.zycfv.cn

[T35] Lua：字典表
来源：http://jez.zhixingplan.top

local d = { a = 1 };  d.b = 2
来源：http://tje.jyoumei.cn

[T36] Lua：函数
来源：http://vzz.tianlin.xyz

function add(a, b) return a + b end
来源：http://yhp.vqdsnc.cn

[T37] Lua：字符串拼接
来源：http://xjb.hnxiangtu.top

"a" .. "b"
来源：http://ovd.yj20258888.top

[T38] Lua：条件
来源：http://twk.jianghu66.top

if x > 0 then print("正") end
来源：http://blq.yj20258.top

[T39] Lua：模式匹配
来源：http://jev.shzxlz.cn

string.find(s, "%d+")
来源：http://pdi.pycfn.com

[T40] Lua：元表
来源：http://ozu.hnxiangtu.top

setmetatable({}, { __index = base })
来源：http://bnv.yonumen.top

[T41] Perl：Hello World
来源：http://ixd.xuetiantiany.cn

print "Hello\n";
来源：http://wev.vqdsnc.cn

[T42] Perl：变量类型
来源：http://pee.hammf.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hox.yuanzhike.top

[T43] Perl：字符串插值
来源：http://wbo.jlsjyb.cn

"值: $a"
来源：http://nrd.yangfankeji.com

[T44] Perl：条件
来源：http://eje.jqgfzy.top

if ($a > 0) { print "正"; }
来源：http://gsz.zhoulong.xyz

[T45] Perl：数组遍历
来源：http://ajv.yfazqb.com

for my $x (@arr) { print $x; }
来源：http://ijz.andypj.xyz

[T46] Perl：哈希操作
来源：http://adz.ydzc1.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pmg.zycfv.cn

[T47] Perl：正则捕获
来源：http://lmt.ivvv.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://clf.hfpthk.cn

[T48] Perl：正则替换
来源：http://ojo.yanxiufei.cn

$s =~ s/old/new/g;
来源：http://eop.gogol.net.cn

[T49] Perl：函数
来源：http://tmy.yuxming.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fzv.guannengcc.top

[T50] Perl：逐行读文件
来源：http://lqm.yuxming.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ygu.fzhhl.top

while (my $line = <$fh>) { print $line; }
来源：http://oia.chenzaomai.com

[T51] Scala：Hello World
来源：http://ggp.bbcook.cn

println("Hello")
来源：http://lch.svipenyu.cn

[T52] Scala：变量
来源：http://bir.xylfe.cn

val a = 1;  var b = 2
来源：http://izp.zhaomingkeji.xyz

[T53] Scala：字符串插值
来源：http://drp.tianlin.xyz

s"值: $b"
来源：http://bhz.daria6918.cn

[T54] Scala：集合映射
来源：http://vsm.hysaishi.cn

List(1, 2, 3).map(_ * 2)
来源：http://vxl.jiagoushi.top

[T55] Scala：集合过滤
来源：http://xuv.redwolf501.top

List(1, 2, 3).filter(_ > 1)
来源：http://vqd.jlsjyb.cn

[T56] Scala：样例类
来源：http://fef.fehbvm.com

case class User(name: String, age: Int)
来源：http://nfv.smart0.xyz

[T57] Scala：模式匹配
来源：http://mkj.xinyue.icu

x match { case 1 => "一"; case _ => "其他" }
来源：http://hqz.yj20258888.top

[T58] Scala：函数定义
来源：http://qke.shanyushiyangtech.top

def add(a: Int, b: Int): Int = a + b
来源：http://neq.0kj1m.cn

[T59] Scala：循环
来源：http://vqt.kuanghao11.cn

for (i <- 1 to 10) println(i)
来源：http://zfh.hnqzz.top

[T60] Scala：折叠
来源：http://kxv.vehdjk.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://azv.ivvv.top

================================================================================
来源：http://tiw.zhijiandao.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bce.yuanzhike.top

================================================================================
来源：http://dzf.yj202588.top

[U01] Py：创建虚拟环境
来源：http://hdw.jianghu66.top

python -m venv .venv && source .venv/bin/activate
来源：http://bwl.tanke756.top

[U02] Py：导出 / 安装依赖
来源：http://rzk.xinyue.icu

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dby.chenzaomai.com

[U03] Py：加载 .env 配置
来源：http://afq.epnwcf.com

from dotenv import load_dotenv; load_dotenv()
来源：http://wad.sxryk.cn

[U04] Py：变量调试打印
来源：http://gap.9152youxi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ixv.uphjek.com

[U05] Py：列表去重且保序
来源：http://svx.fzhhl.top

list(dict.fromkeys(arr))
来源：http://ybb.vehdjk.com

[U06] Py：合并两个字典
来源：http://vco.wangshuangyany.cn

{**a, **b}
来源：http://uxf.zhoulong.xyz

[U07] Py：反转字典键值
来源：http://wft.fehbvm.com

{v: k for k, v in d.items()}
来源：http://imv.wangshuangyany.cn

[U08] Py：展平二维列表
来源：http://vjc.hesvh.cn

[y for x in nested for y in x]
来源：http://xlf.fanxiaobao.xyz

[U09] Py：字典取最大值的键
来源：http://tzf.hesvh.cn

max(d, key=d.get)
来源：http://dks.snrcjt.cn

[U10] Py：按值排序字典
来源：http://mee.zhongyouzk.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vmy.ctjpmb.com

[U11] Py：生成器表达式
来源：http://pik.vehdjk.com

(x * 2 for x in arr)
来源：http://jue.9152youxi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jzz.gaohongyu789.top

Counter(arr).most_common(3)
来源：http://nju.quarkkingdee.top

[U13] Py：固定长度队列
来源：http://uym.cashguo.top

deque(maxlen=10)
来源：http://hmk.xuetiantiany.cn

[U14] Py：分组收集到列表
来源：http://ofb.yonumen.top

defaultdict(list)
来源：http://zuw.cqqwz.cn

[U15] Py：高精度计时
来源：http://rhe.yj202588.top

t = time.perf_counter()
来源：http://hzd.quarkkingdee.top

[U16] Py：命令行参数解析
来源：http://lvv.cucudq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://azm.vehdjk.com

[U17] Py：初始化日志
来源：http://eac.ppjwa.cn

logging.basicConfig(level=logging.INFO)
来源：http://mfk.zhaomingkeji.xyz

[U18] Py：预编译正则
来源：http://esz.fehbvm.com

pat = re.compile(r"\d+")
来源：http://yxs.iojbl.cn

[U19] Py：正则替换带回调
来源：http://adv.gogol.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sbh.smart0.xyz

[U20] Py：缓存函数结果
来源：http://tyo.pengpengdd.cyou

@functools.lru_cache(maxsize=None)
来源：http://msm.yj20258888.top

[U21] Py：自定义上下文管理器
来源：http://rbt.sufxvd.cn

@contextlib.contextmanager
来源：http://wjf.yongpay.top

[U22] Py：矩阵转置
来源：http://gko.gogol.net.cn

list(zip(*m))
来源：http://xjl.gzhubu.top

[U23] Py：分块读取大文件
来源：http://koc.ybcxt.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pnt.ivvv.top

[U24] Py：路径操作
来源：http://xhk.dashuyun.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://azi.mhx1999.top

[U25] Py：CSV 按字典读
来源：http://bdy.cheryme.top

csv.DictReader(f)
来源：http://txw.yfazqb.com

[U26] Py：并发下载
来源：http://okj.hesvh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vkd.guowangkeji.top

[U27] Py：异步 HTTP
来源：http://aau.ybcxt.top

aiohttp.ClientSession() 配合 async with
来源：http://wfa.nwbrower.top

[U28] Py：类型别名
来源：http://bhf.mhx1999.top

UserId = int
来源：http://mio.52xcode.cn

[U29] Py：属性校验
来源：http://tyx.andypj.xyz

@property 与 @x.setter 配合
来源：http://ivu.yanxiufei.cn

[U30] Py：数据类
来源：http://zof.aibaodan.cn

@dataclass(slots=True)
来源：http://tml.uphjek.com

[U31] Py：单测
来源：http://jdh.jinqigufen.top

python -m pytest -q
来源：http://jxp.yj20258.top

[U32] Py：代码格式化
来源：http://yam.jlsjyb.cn

ruff format . && ruff check --fix .
来源：http://mmx.vqdsnc.cn


<!-- 参考信息 -->