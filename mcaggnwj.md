代发 wailian999

int x; scanf("%d", &x);
来源：http://leh.chenjidiqi.icu

[S04] C：字符串复制
来源：http://wuk.ivvv.top

char dst[32]; strcpy(dst, "hi");
来源：http://wts.shangyingyoupin.top

[S05] C：字符串长度
来源：http://mbc.yueranfly.top

strlen(s)
来源：http://rkk.hammf.cn

[S06] C：字符串比较
来源：http://igz.yongpay.top

strcmp(a, b) == 0
来源：http://cgq.havefunace.top

[S07] C：数组遍历求和
来源：http://edn.snrcjt.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tba.tian-w.cn

[S08] C：动态内存分配与释放
来源：http://olr.yfazqb.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uea.tarul.cn

[S09] C：结构体定义与初始化
来源：http://xyp.zhixingplan.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blv.gzhubu.top

[S10] C：指针与解引用
来源：http://svq.dashuyun.cn

int *p = &a;  *p = 5;
来源：http://dkb.nanxinkj.top

[S11] C：逐行读文件
来源：http://rja.jyoumei.cn

FILE *f = fopen("a.txt", "r");
来源：http://rxg.yueranfly.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wrx.pycfn.com

fclose(f);
来源：http://khf.smart0.xyz

[S12] C：写文件
来源：http://jyl.ctjpmb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zqh.fktsv.cn

[S13] C：宏定义
来源：http://rdt.ivvv.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nnf.nwbrower.top

[S14] C：枚举
来源：http://oqf.xuetiantiany.cn

enum Color { RED, GREEN, BLUE };
来源：http://acv.yueranfly.top

[S15] C：类型转换
来源：http://alu.xylfe.cn

(double) a / b
来源：http://ebc.ehwqpu.com

[S16] C：位操作置位
来源：http://wwg.jiagoushi.top

x |= (1 << 3);
来源：http://ffb.hesvh.cn

[S17] C：安全拼接字符串
来源：http://dhn.yongpay.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lpy.vqdsnc.cn

[S18] C：命令行参数
来源：http://ola.nwbrower.top

int main(int argc, char **argv)
来源：http://vcd.zdqjudy.top

[S19] C：快速排序
来源：http://aud.hfpthk.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hky.ydjk.org.cn

[S20] C：二分查找
来源：http://ggz.hnxiangtu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pfp.quarkkingdee.top

[S21] C：字符类别判断
来源：http://dht.wangshuangyany.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ksd.jqgufenzy.top

[S22] C：字符串转数字
来源：http://aty.xylfe.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ptj.yonumen.top

[S23] C：随机数
来源：http://wgx.ydjk.org.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://omv.yangfankeji.com

[S24] C：获取本地时间
来源：http://dhx.gzhubu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bki.fanxiaobao.xyz

[S25] C：内存拷贝
来源：http://otg.yvedp.cn

memcpy(dst, src, n);
来源：http://bfh.zhongyouzk.top

[S26] C：内存清零
来源：http://qov.fktsv.cn

memset(a, 0, sizeof a);
来源：http://sxl.shanyushiyangkeji.top

[S27] C：定义常量
来源：http://jhe.jinqigfzy.top

const double PI = 3.14159;
来源：http://sjw.ehwqpu.com

[S28] C：静态变量
来源：http://ebh.jqgufenzy.top

static int counter = 0;
来源：http://hyp.havefunace.top

[S29] C：变参函数
来源：http://azb.jinyuanbaomall.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kaj.ctjpmb.com

[S30] C：头文件保护
来源：http://zcj.aibaodan.cn

#ifndef X_H
来源：http://lsu.dashuyun.cn

#define X_H
来源：http://mkw.yuanzhike.top

#endif
来源：http://keo.epnwcf.com

[S31] C++：Hello World
来源：http://axt.yuanzhike.top

#include <iostream>
来源：http://vqn.yueranfly.top

int main() { std::cout << "Hello\n"; }
来源：http://bbu.yuxming.cn

[S32] C++：字符串
来源：http://pgb.gzhubu.top

std::string s = "hi";  s += "!";
来源：http://mlf.havefunace.top

[S33] C++：vector 增删
来源：http://fmf.bjfxy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://onf.xuetiantiany.cn

[S34] C++：遍历 vector
来源：http://dtb.c1oappe.top

for (auto &x : v) { std::cout << x; }
来源：http://zql.316326.xyz

[S35] C++：map
来源：http://yjj.52xcode.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vtx.birdmap.top

[S36] C++：unordered_map
来源：http://atf.iojbl.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://usw.ydjk.org.cn

[S37] C++：set
来源：http://btp.yongpay.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kef.mhx1999.top

[S38] C++：排序
来源：http://ngu.jinqigufen.top

std::sort(v.begin(), v.end());
来源：http://kut.gotoacloud.top

[S39] C++：自定义比较器排序
来源：http://fzu.shanyushiyangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qof.shzxlz.cn

[S40] C++：查找元素
来源：http://xmf.kuanghao11.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yzs.aizwys.cn

[S41] C++：类与构造函数
来源：http://hzi.9152youxi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://apo.uphjek.com

[S42] C++：继承与虚函数
来源：http://uie.quarkkingdee.top

class B : public Base { public: void f() override {} };
来源：http://yjm.feifeiyinyue.top

[S43] C++：智能指针
来源：http://jrf.yj202588.top

auto p = std::make_unique<int>(5);
来源：http://uua.redwolf501.top

[S44] C++：引用传参
来源：http://ptx.fehbvm.com

void inc(int &x) { ++x; }
来源：http://heb.svipenyu.cn

[S45] C++：lambda
来源：http://nag.52xcode.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gry.ppjwa.cn

[S46] C++：函数模板
来源：http://xnm.yvedp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mdv.yuanzhike.top

[S47] C++：结构化绑定遍历
来源：http://qxq.iojbl.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://knl.jinyuanbaomall.cn

[S48] C++：逐行读文件
来源：http://jgk.tian-w.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pnh.ydzc1.top

while (std::getline(in, line)) { }
来源：http://lka.gotoacloud.top

[S49] C++：写文件
来源：http://tiu.yj202588.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kln.pycfn.com

[S50] C++：格式化数字
来源：http://axv.yvedp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qqs.sysykeji.top

[S51] C++：显式类型转换
来源：http://bov.c1oappe.top

static_cast<double>(a) / b
来源：http://szm.yj20258888.top

[S52] C++：const 与 noexcept
来源：http://qyi.cheryme.top

int size() const noexcept { return n_; }
来源：http://ydr.guowangkeji.top

[S53] C++：移动语义
来源：http://ynu.dashuyun.cn

std::vector<int> w = std::move(v);
来源：http://ant.jiagoushi.top

[S54] C++：异常处理
来源：http://rgc.hcnkem.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pci.wangdashe.top

[S55] C++：结构化绑定
来源：http://tff.cashguo.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ikh.hnqzz.top

[S56] C++：optional
来源：http://czl.zhijiandao.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vpg.yueranfly.top

[S57] C++：编译期常量
来源：http://wsl.zhixingplan.top

constexpr int N = 10;
来源：http://mon.ydzc1.top

[S58] C++：命名空间
来源：http://iwb.shuidangran.top

namespace ns { int f() { return 1; } }
来源：http://vwx.shuidangran.top

[S59] C++：静态断言
来源：http://mek.nwbrower.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ksk.chenjidiqi.icu

[S60] C++：遍历并删除元素
来源：http://ssi.zhiwuduotai.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hux.xinyue.icu

================================================================================
来源：http://rzu.vqdsnc.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lzs.sysykeji.top

================================================================================
来源：http://jan.yonumen.top

[T01] Kotlin：Hello World
来源：http://mdy.tianlin.xyz

println("Hello")
来源：http://buh.zdqjudy.top

[T02] Kotlin：变量
来源：http://nxe.yj202588.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hwx.bbcook.cn

[T03] Kotlin：字符串模板
来源：http://kxq.ydjk.org.cn

"值: $b"
来源：http://bay.sjlbkw.cn

[T04] Kotlin：空安全
来源：http://jjt.zhengqikj.top

val n: String? = null;  n?.length
来源：http://lac.316326.xyz

[T05] Kotlin：when 表达式
来源：http://rwj.xuanzx.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gnu.xziqi.cn

[T06] Kotlin：集合映射
来源：http://zas.aibaodan.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tsq.nwbrower.top

[T07] Kotlin：集合过滤
来源：http://lfj.yuxming.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mdl.shanyushiyangkeji.top

[T08] Kotlin：数据类
来源：http://bzk.sjlbkw.cn

data class User(val name: String, val age: Int)
来源：http://gas.fanxiaobao.xyz

[T09] Kotlin：扩展函数
来源：http://goc.xziqi.cn

fun String.exclaim() = this + "!"
来源：http://lfe.hongshengwenyu.top

[T10] Kotlin：默认参数
来源：http://edp.9152youxi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ryx.xziqi.cn

[T11] Kotlin：协程
来源：http://gob.snrcjt.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lbk.yonumen.top

[T12] Kotlin：解构声明
来源：http://lcf.havefunace.top

val (a, b) = Pair(1, 2)
来源：http://khz.cheryme.top

[T13] Kotlin：只读 Map
来源：http://rbp.hesvh.cn

val m = mapOf("a" to 1)
来源：http://mqc.svipenyu.cn

[T14] Kotlin：循环
来源：http://syn.jqgfzy.top

for (i in 1..10) println(i)
来源：http://dup.fanxiaobao.xyz

[T15] Kotlin：接口
来源：http://cjk.smart0.xyz

interface Shape { fun area(): Double }
来源：http://luu.yj202588.top

[T16] Swift：Hello World
来源：http://fss.ywan-chungtsiang.top

print("Hello")
来源：http://gdk.aizwys.cn

[T17] Swift：变量与常量
来源：http://ypt.cheryme.top

var a = 1;  let b = 2
来源：http://hmr.hcnkem.com

[T18] Swift：字符串插值
来源：http://zsu.nanxinkj.top

"值: \(b)"
来源：http://jfh.hammf.cn

[T19] Swift：可选绑定
来源：http://czv.ctjpmb.com

if let n = opt { print(n) }
来源：http://tga.shzxlz.cn

[T20] Swift：数组操作
来源：http://rrd.yanxiufei.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rui.yj20258888.top

[T21] Swift：遍历
来源：http://pws.guowangkeji.top

for x in a { print(x) }
来源：http://bjj.hesvh.cn

[T22] Swift：字典
来源：http://jgd.zdqjudy.top

var d = ["a": 1];  d["b"] = 2
来源：http://kql.chenjidiqi.icu

[T23] Swift：函数
来源：http://jgk.jyoumei.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bpk.sjlbkw.cn

[T24] Swift：闭包
来源：http://qvl.dianchejie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pdf.redwolf501.top

[T25] Swift：结构体
来源：http://cej.yuxming.cn

struct P { var x: Int }
来源：http://ltz.daria6918.cn

[T26] Swift：类与重写
来源：http://zrf.zhongyouzk.top

class A: Base { override func f() {} }
来源：http://pro.aizwys.cn

[T27] Swift：错误处理
来源：http://ikd.hammf.cn

do { try f() } catch { print(error) }
来源：http://jot.bbcook.cn

[T28] Swift：枚举
来源：http://ecw.andypj.xyz

enum Color { case red, green }
来源：http://pdj.smart0.xyz

[T29] Swift：guard 提前返回
来源：http://ipz.quarkkingdee.top

guard let x = opt else { return }
来源：http://bat.zhoulong.xyz

[T30] Swift：协议
来源：http://wie.snrcjt.cn

protocol Shape { func area() -> Double }
来源：http://shl.hammf.cn

[T31] Lua：Hello World
来源：http://mzf.ctjpmb.com

print("Hello")
来源：http://eex.tian-w.cn

[T32] Lua：局部变量
来源：http://vqx.yj20258888.top

local a = 1
来源：http://tkq.9152youxi.cn

[T33] Lua：表（数组）
来源：http://pxa.snrcjt.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hkp.daxiang520.top

[T34] Lua：遍历表
来源：http://gnd.cheryme.top

for i, v in ipairs(t) do print(i, v) end
来源：http://jvh.xuanzx.com

[T35] Lua：字典表
来源：http://dln.hcnkem.com

local d = { a = 1 };  d.b = 2
来源：http://yev.zhaomingkeji.xyz

[T36] Lua：函数
来源：http://uww.daria6918.cn

function add(a, b) return a + b end
来源：http://isn.fehbvm.com

[T37] Lua：字符串拼接
来源：http://oal.haohaochexian.top

"a" .. "b"
来源：http://pfn.vehdjk.com

[T38] Lua：条件
来源：http://xue.yuanzhike.top

if x > 0 then print("正") end
来源：http://ktm.zhengqikj.top

[T39] Lua：模式匹配
来源：http://euy.hcnkem.com

string.find(s, "%d+")
来源：http://nav.svipenyu.cn

[T40] Lua：元表
来源：http://lxa.xingfuxueyuan.xyz

setmetatable({}, { __index = base })
来源：http://czs.zycfv.cn

[T41] Perl：Hello World
来源：http://oda.ivvv.top

print "Hello\n";
来源：http://fay.hesvh.cn

[T42] Perl：变量类型
来源：http://zlx.wangdashe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wdx.yonumen.top

[T43] Perl：字符串插值
来源：http://ulr.xuetiantiany.cn

"值: $a"
来源：http://lhp.fzhhl.top

[T44] Perl：条件
来源：http://xpi.jqgfzy.top

if ($a > 0) { print "正"; }
来源：http://pko.yj20258888.top

[T45] Perl：数组遍历
来源：http://oqg.hongshengwenyu.top

for my $x (@arr) { print $x; }
来源：http://myg.gotoacloud.top

[T46] Perl：哈希操作
来源：http://wwd.ydzc1.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://irw.tian-w.cn

[T47] Perl：正则捕获
来源：http://fyj.vehdjk.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://tuc.yonumen.top

[T48] Perl：正则替换
来源：http://kez.vqdsnc.cn

$s =~ s/old/new/g;
来源：http://rkd.uphjek.com

[T49] Perl：函数
来源：http://spt.fktsv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://thb.zhengqikj.top

[T50] Perl：逐行读文件
来源：http://rcw.jinyuanbaomall.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://plq.0kj1m.cn

while (my $line = <$fh>) { print $line; }
来源：http://hpi.tianlin.xyz

[T51] Scala：Hello World
来源：http://ckh.zycfv.cn

println("Hello")
来源：http://jhc.gotoacloud.top

[T52] Scala：变量
来源：http://dps.ywan-chungtsiang.top

val a = 1;  var b = 2
来源：http://vcd.0kj1m.cn

[T53] Scala：字符串插值
来源：http://qjw.0kj1m.cn

s"值: $b"
来源：http://fdr.hywenlv.cn

[T54] Scala：集合映射
来源：http://btf.yuanzhike.top

List(1, 2, 3).map(_ * 2)
来源：http://afp.hfpthk.cn

[T55] Scala：集合过滤
来源：http://wnm.shangyingyoupin.top

List(1, 2, 3).filter(_ > 1)
来源：http://qli.daxiang520.top

[T56] Scala：样例类
来源：http://fuv.ppjwa.cn

case class User(name: String, age: Int)
来源：http://vos.kuanghao11.cn

[T57] Scala：模式匹配
来源：http://pgf.bjfxy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ipy.tanke756.top

[T58] Scala：函数定义
来源：http://lbj.316326.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://ylj.svipenyu.cn

[T59] Scala：循环
来源：http://qab.sweek.top

for (i <- 1 to 10) println(i)
来源：http://pwf.shangyingyoupin.top

[T60] Scala：折叠
来源：http://gga.zhengqikj.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zxc.ywan-chungtsiang.top

================================================================================
来源：http://gty.ydzc1.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tfy.fehbvm.com

================================================================================
来源：http://ole.tianlin.xyz

[U01] Py：创建虚拟环境
来源：http://thk.birdmap.top

python -m venv .venv && source .venv/bin/activate
来源：http://pgi.ivvv.top

[U02] Py：导出 / 安装依赖
来源：http://pyv.gogol.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wzp.fzhhl.top

[U03] Py：加载 .env 配置
来源：http://prg.epnwcf.com

from dotenv import load_dotenv; load_dotenv()
来源：http://ovv.zhiwuduotai.top

[U04] Py：变量调试打印
来源：http://amv.nanxinkj.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rwq.snrcjt.cn

[U05] Py：列表去重且保序
来源：http://iso.316326.xyz

list(dict.fromkeys(arr))
来源：http://vwy.xuanzx.com

[U06] Py：合并两个字典
来源：http://zoc.bjfxy.top

{**a, **b}
来源：http://ine.0kj1m.cn

[U07] Py：反转字典键值
来源：http://ank.ppjwa.cn

{v: k for k, v in d.items()}
来源：http://hsm.fzhhl.top

[U08] Py：展平二维列表
来源：http://css.xuetiantiany.cn

[y for x in nested for y in x]
来源：http://tgg.chenzaomai.com

[U09] Py：字典取最大值的键
来源：http://ivg.ehwqpu.com

max(d, key=d.get)
来源：http://ylf.ctjpmb.com

[U10] Py：按值排序字典
来源：http://agi.fanxiaobao.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wax.uphjek.com

[U11] Py：生成器表达式
来源：http://fjf.yfazqb.com

(x * 2 for x in arr)
来源：http://pqf.kuanghao11.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jdz.hongshengwenyu.top

Counter(arr).most_common(3)
来源：http://qge.zhengqikj.top

[U13] Py：固定长度队列
来源：http://iyl.bjfxy.top

deque(maxlen=10)
来源：http://spn.yueranfly.top

[U14] Py：分组收集到列表
来源：http://arj.zhijiandao.cn

defaultdict(list)
来源：http://hvq.zdbjq.cn

[U15] Py：高精度计时
来源：http://uew.ehwqpu.com

t = time.perf_counter()
来源：http://nrt.yj202588.top

[U16] Py：命令行参数解析
来源：http://pvy.iojbl.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fqc.zhengqikj.top

[U17] Py：初始化日志
来源：http://tlx.zhongyouzk.top

logging.basicConfig(level=logging.INFO)
来源：http://byq.9152youxi.cn

[U18] Py：预编译正则
来源：http://esm.jinghuilouyu.cn

pat = re.compile(r"\d+")
来源：http://rwg.zhixingplan.top

[U19] Py：正则替换带回调
来源：http://nlm.smart0.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://voq.havefunace.top

[U20] Py：缓存函数结果
来源：http://onq.cqqwz.cn

@functools.lru_cache(maxsize=None)
来源：http://zmd.yangfankeji.com

[U21] Py：自定义上下文管理器
来源：http://dbc.fengsongda.top

@contextlib.contextmanager
来源：http://bwl.jqgfzy.top

[U22] Py：矩阵转置
来源：http://mqu.bjfxy.top

list(zip(*m))
来源：http://xmh.sysykeji.top

[U23] Py：分块读取大文件
来源：http://rex.nanxuanxn.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gfn.jinqigufen.top

[U24] Py：路径操作
来源：http://tij.jinghuilouyu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tha.svipenyu.cn

[U25] Py：CSV 按字典读
来源：http://sit.jinghuilouyu.cn

csv.DictReader(f)
来源：http://rkh.nwbrower.top

[U26] Py：并发下载
来源：http://fiw.shanyushiyangkeji.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://uzs.jqgfzy.top


<!-- 参考信息 -->