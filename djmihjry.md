代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://ofl.hnxiangtu.top

[R70] 时间戳与互转
来源：http://oku.chenzaomai.com

date +%s;  date -d @1700000000
来源：http://xbb.xuetiantiany.cn

[R71] 日期格式化
来源：http://kyd.jinqigfzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://zdr.jiagoushi.top

[R72] 等待端口就绪
来源：http://wlv.cashguo.top

until nc -z localhost 3306; do sleep 1; done
来源：http://twq.dianchejie.cn

[R73] 分割大日志
来源：http://wdg.yueranfly.top

split -l 1000 big.log part_
来源：http://ibz.zhengqikj.top

[R74] 批量重命名
来源：http://ubh.xylfe.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wkb.fzhhl.top

[R75] 导出环境变量
来源：http://jkn.hnxiangtu.top

export PATH="$HOME/bin:$PATH"
来源：http://fuv.fanxiaobao.xyz

[R76] 使用临时文件
来源：http://ydw.guannengcc.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mcw.yuanzhike.top

[R77] 读取用户输入
来源：http://rzk.yj202588.top

read -rp "请输入: " ans
来源：http://txv.hywenlv.cn

[R78] 交互式菜单
来源：http://gxr.dashuyun.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tke.sxryk.cn

[R79] 解析命令行选项
来源：http://ffx.52xcode.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rlp.zhixingplan.top

[R80] 查看脚本执行耗时
来源：http://xzb.mhx1999.top

time ./run.sh
来源：http://rig.iojbl.cn

================================================================================
来源：http://auo.hfpthk.cn

S. C / C++ 专题
来源：http://oip.jinghuilouyu.cn

================================================================================
来源：http://frb.ehwqpu.com

[S01] C：Hello World
来源：http://uju.zhongyouzk.top

#include <stdio.h>
来源：http://cwj.hammf.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jqq.nanxinkj.top

[S02] C：变量与格式化输出
来源：http://kjs.birdmap.top

int a = 10; printf("%d\n", a);
来源：http://zgj.52xcode.cn

[S03] C：读入整数
来源：http://cqs.shanyushiyangkeji.top

int x; scanf("%d", &x);
来源：http://tsg.ybcxt.top

[S04] C：字符串复制
来源：http://byf.fengsongda.top

char dst[32]; strcpy(dst, "hi");
来源：http://vsu.zhengqikj.top

[S05] C：字符串长度
来源：http://par.xuetiantiany.cn

strlen(s)
来源：http://rhq.yvedp.cn

[S06] C：字符串比较
来源：http://lbs.shanyushiyangtech.top

strcmp(a, b) == 0
来源：http://sun.yonumen.top

[S07] C：数组遍历求和
来源：http://zfg.hnqzz.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ngq.ivvv.top

[S08] C：动态内存分配与释放
来源：http://vhg.feifeiyinyue.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://igs.daria6918.cn

[S09] C：结构体定义与初始化
来源：http://pig.zhengqikj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://maj.yj202588.top

[S10] C：指针与解引用
来源：http://rhu.xinyue.icu

int *p = &a;  *p = 5;
来源：http://wqq.nanxinkj.top

[S11] C：逐行读文件
来源：http://lps.jiagoushi.top

FILE *f = fopen("a.txt", "r");
来源：http://qcj.snrcjt.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://upl.jqgfzy.top

fclose(f);
来源：http://rrk.c1oappe.top

[S12] C：写文件
来源：http://zlo.yuanzhike.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qxt.sweek.top

[S13] C：宏定义
来源：http://qcx.0kj1m.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://drt.zycfv.cn

[S14] C：枚举
来源：http://lsc.bbcook.cn

enum Color { RED, GREEN, BLUE };
来源：http://lyw.yongpay.top

[S15] C：类型转换
来源：http://qfa.hnqzz.top

(double) a / b
来源：http://nko.daria6918.cn

[S16] C：位操作置位
来源：http://dcu.tanke756.top

x |= (1 << 3);
来源：http://uvm.yanxiufei.cn

[S17] C：安全拼接字符串
来源：http://arx.tian-w.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xfd.yj202588.top

[S18] C：命令行参数
来源：http://glx.fengsongda.top

int main(int argc, char **argv)
来源：http://apn.yueranfly.top

[S19] C：快速排序
来源：http://wil.xziqi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qgk.yuanzhike.top

[S20] C：二分查找
来源：http://zho.tian-w.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lwj.sufxvd.cn

[S21] C：字符类别判断
来源：http://yti.zhaomingkeji.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://syq.ppjwa.cn

[S22] C：字符串转数字
来源：http://ovk.zdqjudy.top

atoi("42");  strtod("3.14", NULL);
来源：http://mmf.nwbrower.top

[S23] C：随机数
来源：http://azq.gzhubu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://sqv.nwbrower.top

[S24] C：获取本地时间
来源：http://ygo.fehbvm.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zle.guowangkeji.top

[S25] C：内存拷贝
来源：http://ixw.yuanzhike.top

memcpy(dst, src, n);
来源：http://wty.ehwqpu.com

[S26] C：内存清零
来源：http://oko.vehdjk.com

memset(a, 0, sizeof a);
来源：http://iwb.yueranfly.top

[S27] C：定义常量
来源：http://far.kuanghao11.cn

const double PI = 3.14159;
来源：http://zcz.sysykeji.top

[S28] C：静态变量
来源：http://wii.sjlbkw.cn

static int counter = 0;
来源：http://wfx.tianlin.xyz

[S29] C：变参函数
来源：http://iyl.xinyue.icu

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zqq.ywan-chungtsiang.top

[S30] C：头文件保护
来源：http://ecp.redwolf501.top

#ifndef X_H
来源：http://ybo.fehbvm.com

#define X_H
来源：http://uil.guowangkeji.top

#endif
来源：http://rgk.shanyushiyangtech.top

[S31] C++：Hello World
来源：http://swc.yvedp.cn

#include <iostream>
来源：http://tzs.gaohongyu789.top

int main() { std::cout << "Hello\n"; }
来源：http://rvg.chenjidiqi.icu

[S32] C++：字符串
来源：http://kpt.quarkkingdee.top

std::string s = "hi";  s += "!";
来源：http://kkr.gogol.net.cn

[S33] C++：vector 增删
来源：http://wwx.ydzc1.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lqw.zhengqikj.top

[S34] C++：遍历 vector
来源：http://sam.sufxvd.cn

for (auto &x : v) { std::cout << x; }
来源：http://pyn.shanyushiyangtech.top

[S35] C++：map
来源：http://gsk.jinqigufen.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://chk.zhaomingkeji.xyz

[S36] C++：unordered_map
来源：http://lxu.jinghuilouyu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mwr.yueranfly.top

[S37] C++：set
来源：http://oqm.wangdashe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ejx.jlsjyb.cn

[S38] C++：排序
来源：http://ycf.nanxuanxn.top

std::sort(v.begin(), v.end());
来源：http://duc.quarkkingdee.top

[S39] C++：自定义比较器排序
来源：http://acj.havefunace.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ufa.9152youxi.cn

[S40] C++：查找元素
来源：http://dfn.ywan-chungtsiang.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gos.smart0.xyz

[S41] C++：类与构造函数
来源：http://yew.cqqwz.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nuv.jinyuanbaomall.cn

[S42] C++：继承与虚函数
来源：http://lxr.sweek.top

class B : public Base { public: void f() override {} };
来源：http://con.aizwys.cn

[S43] C++：智能指针
来源：http://zzl.jyoumei.cn

auto p = std::make_unique<int>(5);
来源：http://jjc.vqdsnc.cn

[S44] C++：引用传参
来源：http://lsm.zdqjudy.top

void inc(int &x) { ++x; }
来源：http://gzu.hcnkem.com

[S45] C++：lambda
来源：http://ujs.svipenyu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rfz.mhx1999.top

[S46] C++：函数模板
来源：http://xcd.gotoacloud.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://iyj.cheryme.top

[S47] C++：结构化绑定遍历
来源：http://kmq.ctjpmb.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://awv.hcnkem.com

[S48] C++：逐行读文件
来源：http://nei.hcnkem.com

std::ifstream in("a.txt");  std::string line;
来源：http://pmm.dianchejie.cn

while (std::getline(in, line)) { }
来源：http://yde.jinqigufen.top

[S49] C++：写文件
来源：http://gvt.jinqigfzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yht.andypj.xyz

[S50] C++：格式化数字
来源：http://krd.cheryme.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mws.hongshengwenyu.top

[S51] C++：显式类型转换
来源：http://rrz.gaohongyu789.top

static_cast<double>(a) / b
来源：http://xyd.fktsv.cn

[S52] C++：const 与 noexcept
来源：http://pbd.tanke756.top

int size() const noexcept { return n_; }
来源：http://izo.smart0.xyz

[S53] C++：移动语义
来源：http://rvf.dashuyun.cn

std::vector<int> w = std::move(v);
来源：http://wue.jinqigfzy.top

[S54] C++：异常处理
来源：http://ezy.sweek.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vuz.bbcook.cn

[S55] C++：结构化绑定
来源：http://kvk.bjfxy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lmm.gzhubu.top

[S56] C++：optional
来源：http://mds.haohaochexian.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xfb.pengpengdd.cyou

[S57] C++：编译期常量
来源：http://ktf.ydjk.org.cn

constexpr int N = 10;
来源：http://kwq.gogol.net.cn

[S58] C++：命名空间
来源：http://bhu.hcnkem.com

namespace ns { int f() { return 1; } }
来源：http://mzc.ybcxt.top

[S59] C++：静态断言
来源：http://gtf.gzhubu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://get.jiagoushi.top

[S60] C++：遍历并删除元素
来源：http://wqh.0kj1m.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kdt.jyoumei.cn

================================================================================
来源：http://qur.zhengqikj.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rcs.nanxinkj.top

================================================================================
来源：http://dwy.svipenyu.cn

[T01] Kotlin：Hello World
来源：http://lwt.zhengqikj.top

println("Hello")
来源：http://uta.zhiwuduotai.top

[T02] Kotlin：变量
来源：http://amk.daxiang520.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mhc.hammf.cn

[T03] Kotlin：字符串模板
来源：http://oyi.zhiwuduotai.top

"值: $b"
来源：http://gwd.haohaochexian.top

[T04] Kotlin：空安全
来源：http://cmw.fanxiaobao.xyz

val n: String? = null;  n?.length
来源：http://gsl.guannengcc.top

[T05] Kotlin：when 表达式
来源：http://dbo.cucudq.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rcu.dianchejie.cn

[T06] Kotlin：集合映射
来源：http://zih.fehbvm.com

listOf(1, 2, 3).map { it * 2 }
来源：http://pup.yanxiufei.cn

[T07] Kotlin：集合过滤
来源：http://cyh.aibaodan.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fpz.52xcode.cn

[T08] Kotlin：数据类
来源：http://bot.zdqjudy.top

data class User(val name: String, val age: Int)
来源：http://btm.yuxming.cn

[T09] Kotlin：扩展函数
来源：http://dxv.jyoumei.cn

fun String.exclaim() = this + "!"
来源：http://pau.sweek.top

[T10] Kotlin：默认参数
来源：http://slw.yangfankeji.com

fun greet(name: String = "World") = "Hi $name"
来源：http://pzw.havefunace.top

[T11] Kotlin：协程
来源：http://uht.vqdsnc.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wde.sjlbkw.cn

[T12] Kotlin：解构声明
来源：http://oao.yongpay.top

val (a, b) = Pair(1, 2)
来源：http://lvy.jyoumei.cn

[T13] Kotlin：只读 Map
来源：http://unn.gzhubu.top

val m = mapOf("a" to 1)
来源：http://kzo.yangfankeji.com

[T14] Kotlin：循环
来源：http://ewu.gaohongyu789.top

for (i in 1..10) println(i)
来源：http://hph.yangfankeji.com

[T15] Kotlin：接口
来源：http://wvb.zhengqikj.top

interface Shape { fun area(): Double }
来源：http://lpu.chenjidiqi.icu

[T16] Swift：Hello World
来源：http://ivw.yueranfly.top

print("Hello")
来源：http://qok.hfpthk.cn

[T17] Swift：变量与常量
来源：http://xpt.nanxinkj.top

var a = 1;  let b = 2
来源：http://awz.chenzaomai.com

[T18] Swift：字符串插值
来源：http://eev.hcnkem.com

"值: \(b)"
来源：http://oho.chenzaomai.com

[T19] Swift：可选绑定
来源：http://ovu.sjlbkw.cn

if let n = opt { print(n) }
来源：http://xhy.uphjek.com

[T20] Swift：数组操作
来源：http://cwj.meibo888.top

var a = [1, 2, 3];  a.append(4)
来源：http://bzh.meibo888.top

[T21] Swift：遍历
来源：http://opd.gogol.net.cn

for x in a { print(x) }
来源：http://pvs.yongpay.top

[T22] Swift：字典
来源：http://mwv.shuidangran.top

var d = ["a": 1];  d["b"] = 2
来源：http://roz.wangdashe.top

[T23] Swift：函数
来源：http://pts.jqgufenzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vgq.quarkkingdee.top

[T24] Swift：闭包
来源：http://ybz.ppjwa.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://nyv.ywan-chungtsiang.top

[T25] Swift：结构体
来源：http://oac.sufxvd.cn

struct P { var x: Int }
来源：http://zkj.yanxiufei.cn

[T26] Swift：类与重写
来源：http://wfm.sysykeji.top

class A: Base { override func f() {} }
来源：http://omm.hywenlv.cn

[T27] Swift：错误处理
来源：http://bdd.hnxiangtu.top

do { try f() } catch { print(error) }
来源：http://mcc.tanke756.top

[T28] Swift：枚举
来源：http://cla.hnxiangtu.top

enum Color { case red, green }
来源：http://use.snrcjt.cn

[T29] Swift：guard 提前返回
来源：http://xji.ivvv.top

guard let x = opt else { return }
来源：http://trw.zhongyouzk.top

[T30] Swift：协议
来源：http://dpz.haohaochexian.top

protocol Shape { func area() -> Double }
来源：http://nho.gzhubu.top

[T31] Lua：Hello World
来源：http://kio.sysykeji.top

print("Hello")
来源：http://jsk.bjfxy.top

[T32] Lua：局部变量
来源：http://qvf.jinqigufen.top

local a = 1
来源：http://ckd.yuxming.cn

[T33] Lua：表（数组）
来源：http://heb.ydzc1.top

local t = {1, 2, 3};  t[4] = 4
来源：http://qya.hnqzz.top

[T34] Lua：遍历表
来源：http://ycj.guowangkeji.top

for i, v in ipairs(t) do print(i, v) end
来源：http://pit.daria6918.cn

[T35] Lua：字典表
来源：http://yhv.haohaochexian.top

local d = { a = 1 };  d.b = 2
来源：http://vhv.hfpthk.cn

[T36] Lua：函数
来源：http://whp.mhx1999.top

function add(a, b) return a + b end
来源：http://ikz.zhixingplan.top

[T37] Lua：字符串拼接
来源：http://dup.birdmap.top

"a" .. "b"
来源：http://fhn.jinghuilouyu.cn

[T38] Lua：条件
来源：http://rtz.zhaomingkeji.xyz

if x > 0 then print("正") end
来源：http://aku.jinqigfzy.top

[T39] Lua：模式匹配
来源：http://jrp.tanke756.top

string.find(s, "%d+")
来源：http://kln.xylfe.cn

[T40] Lua：元表
来源：http://oxm.zycfv.cn

setmetatable({}, { __index = base })
来源：http://hgu.zhoulong.xyz

[T41] Perl：Hello World
来源：http://gek.hesvh.cn

print "Hello\n";
来源：http://uek.gogol.net.cn

[T42] Perl：变量类型
来源：http://qis.nanxinkj.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wes.yangfankeji.com

[T43] Perl：字符串插值
来源：http://aje.dashuyun.cn

"值: $a"
来源：http://vhc.daria6918.cn

[T44] Perl：条件
来源：http://htx.9152youxi.cn

if ($a > 0) { print "正"; }
来源：http://yqh.epnwcf.com

[T45] Perl：数组遍历
来源：http://fqy.jiagoushi.top

for my $x (@arr) { print $x; }
来源：http://mcy.hywenlv.cn

[T46] Perl：哈希操作
来源：http://mpd.zhoulong.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ruf.ydzc1.top

[T47] Perl：正则捕获
来源：http://cwu.zhoulong.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://jfz.jianghu66.top

[T48] Perl：正则替换
来源：http://qrl.dianchejie.cn

$s =~ s/old/new/g;
来源：http://qwq.bbcook.cn

[T49] Perl：函数
来源：http://juo.cdnleiting.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://esw.pycfn.com

[T50] Perl：逐行读文件
来源：http://vze.cqqwz.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cyh.shanyushiyangtech.top

while (my $line = <$fh>) { print $line; }
来源：http://hcv.zhixingplan.top

[T51] Scala：Hello World
来源：http://dtw.xinyue.icu

println("Hello")
来源：http://rnd.zhijiandao.cn

[T52] Scala：变量
来源：http://qzj.quarkkingdee.top

val a = 1;  var b = 2
来源：http://dgb.gotoacloud.top

[T53] Scala：字符串插值
来源：http://hle.9152youxi.cn

s"值: $b"
来源：http://wns.jqgfzy.top

[T54] Scala：集合映射
来源：http://pss.hesvh.cn

List(1, 2, 3).map(_ * 2)
来源：http://hav.yongpay.top

[T55] Scala：集合过滤
来源：http://vqt.ehwqpu.com

List(1, 2, 3).filter(_ > 1)
来源：http://uwa.dianchejie.cn

[T56] Scala：样例类
来源：http://dbk.jianghu66.top

case class User(name: String, age: Int)
来源：http://sum.fanxiaobao.xyz

[T57] Scala：模式匹配
来源：http://enp.bjfxy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ziw.gaohongyu789.top

[T58] Scala：函数定义
来源：http://dky.hammf.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mbq.birdmap.top

[T59] Scala：循环
来源：http://elv.hywenlv.cn

for (i <- 1 to 10) println(i)
来源：http://ymr.bjfxy.top

[T60] Scala：折叠
来源：http://xee.c1oappe.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://otr.jinqigufen.top

================================================================================
来源：http://ick.yonumen.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cdg.zhoulong.xyz

================================================================================
来源：http://kse.316326.xyz

[U01] Py：创建虚拟环境
来源：http://hjw.nwbrower.top

python -m venv .venv && source .venv/bin/activate
来源：http://vwn.mhx1999.top

[U02] Py：导出 / 安装依赖
来源：http://mxx.yangfankeji.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ibe.shzxlz.cn

[U03] Py：加载 .env 配置
来源：http://ryc.jyoumei.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://msw.tanke756.top

[U04] Py：变量调试打印
来源：http://mpq.yuanzhike.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://clk.yfazqb.com

[U05] Py：列表去重且保序
来源：http://tua.ivvv.top

list(dict.fromkeys(arr))
来源：http://sod.hammf.cn

[U06] Py：合并两个字典
来源：http://zsv.gotoacloud.top

{**a, **b}
来源：http://uxz.yonumen.top

[U07] Py：反转字典键值
来源：http://mca.zhiwuduotai.top

{v: k for k, v in d.items()}
来源：http://xvd.zhijiandao.cn

[U08] Py：展平二维列表
来源：http://qqq.zhixingplan.top

[y for x in nested for y in x]
来源：http://lpg.tian-w.cn

[U09] Py：字典取最大值的键
来源：http://ufh.fktsv.cn

max(d, key=d.get)
来源：http://zcl.feifeiyinyue.top

[U10] Py：按值排序字典
来源：http://fem.jianghu66.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tnu.zhengqikj.top


<!-- 参考信息 -->