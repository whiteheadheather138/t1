代发 wailian999

S. C / C++ 专题
来源：http://wdz.yj20258888.top

================================================================================
来源：http://epq.fanxiaobao.xyz

[S01] C：Hello World
来源：http://yux.ydjk.org.cn

#include <stdio.h>
来源：http://uye.xingfuxueyuan.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://nks.svipenyu.cn

[S02] C：变量与格式化输出
来源：http://ujr.xziqi.cn

int a = 10; printf("%d\n", a);
来源：http://maj.jinqigufen.top

[S03] C：读入整数
来源：http://oxo.wangshuangyany.cn

int x; scanf("%d", &x);
来源：http://uor.fanxiaobao.xyz

[S04] C：字符串复制
来源：http://fyu.guowangkeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://lcz.jqgfzy.top

[S05] C：字符串长度
来源：http://mvz.yongpay.top

strlen(s)
来源：http://skd.cashguo.top

[S06] C：字符串比较
来源：http://soh.quarkkingdee.top

strcmp(a, b) == 0
来源：http://dfd.yongpay.top

[S07] C：数组遍历求和
来源：http://cdv.cashguo.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vzx.havefunace.top

[S08] C：动态内存分配与释放
来源：http://ywm.gzhubu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ouq.vqdsnc.cn

[S09] C：结构体定义与初始化
来源：http://kcj.sjlbkw.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tub.cdnleiting.top

[S10] C：指针与解引用
来源：http://gcd.tianlin.xyz

int *p = &a;  *p = 5;
来源：http://xcv.bbcook.cn

[S11] C：逐行读文件
来源：http://gkp.chenlongwang.top

FILE *f = fopen("a.txt", "r");
来源：http://whn.epnwcf.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://dqp.daria6918.cn

fclose(f);
来源：http://qpi.zhijiandao.cn

[S12] C：写文件
来源：http://vja.yj202588.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://byq.uphjek.com

[S13] C：宏定义
来源：http://jqs.epnwcf.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hjd.jlsjyb.cn

[S14] C：枚举
来源：http://kwc.cheryme.top

enum Color { RED, GREEN, BLUE };
来源：http://woe.hcnkem.com

[S15] C：类型转换
来源：http://zrb.uphjek.com

(double) a / b
来源：http://liu.bjfxy.top

[S16] C：位操作置位
来源：http://xge.chenlongwang.top

x |= (1 << 3);
来源：http://uda.wangshuangyany.cn

[S17] C：安全拼接字符串
来源：http://xwn.c1oappe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mgf.uphjek.com

[S18] C：命令行参数
来源：http://abv.yfazqb.com

int main(int argc, char **argv)
来源：http://fsx.jinqigufen.top

[S19] C：快速排序
来源：http://dwx.cucudq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xjz.yj20258888.top

[S20] C：二分查找
来源：http://pkz.fzhhl.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bsr.zhixingplan.top

[S21] C：字符类别判断
来源：http://rec.tarul.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tmk.zdqjudy.top

[S22] C：字符串转数字
来源：http://mia.pycfn.com

atoi("42");  strtod("3.14", NULL);
来源：http://nxz.zycfv.cn

[S23] C：随机数
来源：http://jkv.hnqzz.top

srand(time(NULL));  int r = rand() % 100;
来源：http://jce.dashuyun.cn

[S24] C：获取本地时间
来源：http://idu.ydzc1.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cqh.hfpthk.cn

[S25] C：内存拷贝
来源：http://pgf.ivvv.top

memcpy(dst, src, n);
来源：http://ezq.wangshuangyany.cn

[S26] C：内存清零
来源：http://lxp.wangshuangyany.cn

memset(a, 0, sizeof a);
来源：http://obm.zhijiandao.cn

[S27] C：定义常量
来源：http://ywe.aibaodan.cn

const double PI = 3.14159;
来源：http://env.zhaomingkeji.xyz

[S28] C：静态变量
来源：http://xoq.cdnleiting.top

static int counter = 0;
来源：http://ujx.daria6918.cn

[S29] C：变参函数
来源：http://oyn.jyoumei.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hvs.kuanghao11.cn

[S30] C：头文件保护
来源：http://ybz.kuanghao11.cn

#ifndef X_H
来源：http://btf.cucudq.cn

#define X_H
来源：http://mzi.ybcxt.top

#endif
来源：http://gyj.ppjwa.cn

[S31] C++：Hello World
来源：http://jfz.hfpthk.cn

#include <iostream>
来源：http://dna.hammf.cn

int main() { std::cout << "Hello\n"; }
来源：http://vxo.ydjk.org.cn

[S32] C++：字符串
来源：http://jkt.ehwqpu.com

std::string s = "hi";  s += "!";
来源：http://wff.pycfn.com

[S33] C++：vector 增删
来源：http://pey.sysykeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fua.tianlin.xyz

[S34] C++：遍历 vector
来源：http://hxf.fengsongda.top

for (auto &x : v) { std::cout << x; }
来源：http://cyn.zhixingplan.top

[S35] C++：map
来源：http://bbo.gaohongyu789.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oli.ivvv.top

[S36] C++：unordered_map
来源：http://lew.smart0.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baj.snrcjt.cn

[S37] C++：set
来源：http://qto.iojbl.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nmg.gotoacloud.top

[S38] C++：排序
来源：http://qan.fktsv.cn

std::sort(v.begin(), v.end());
来源：http://wvz.9152youxi.cn

[S39] C++：自定义比较器排序
来源：http://toz.ywan-chungtsiang.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zgh.gotoacloud.top

[S40] C++：查找元素
来源：http://lwn.jinyuanbaomall.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://iza.cqqwz.cn

[S41] C++：类与构造函数
来源：http://unc.hywenlv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://byv.cdnleiting.top

[S42] C++：继承与虚函数
来源：http://yva.hywenlv.cn

class B : public Base { public: void f() override {} };
来源：http://cdb.c1oappe.top

[S43] C++：智能指针
来源：http://wxm.yj20258888.top

auto p = std::make_unique<int>(5);
来源：http://jsn.zycfv.cn

[S44] C++：引用传参
来源：http://pfu.feifeiyinyue.top

void inc(int &x) { ++x; }
来源：http://mfa.andypj.xyz

[S45] C++：lambda
来源：http://fxb.smart0.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://hvd.yanxiufei.cn

[S46] C++：函数模板
来源：http://ncs.ehwqpu.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uxt.bbcook.cn

[S47] C++：结构化绑定遍历
来源：http://agc.chenzaomai.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ntb.redwolf501.top

[S48] C++：逐行读文件
来源：http://pzz.hcnkem.com

std::ifstream in("a.txt");  std::string line;
来源：http://egy.epnwcf.com

while (std::getline(in, line)) { }
来源：http://zxq.pengpengdd.cyou

[S49] C++：写文件
来源：http://ccf.aibaodan.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eea.wangdashe.top

[S50] C++：格式化数字
来源：http://ofk.daria6918.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ovu.shanyushiyangkeji.top

[S51] C++：显式类型转换
来源：http://mmb.fktsv.cn

static_cast<double>(a) / b
来源：http://qbp.pycfn.com

[S52] C++：const 与 noexcept
来源：http://rea.hcnkem.com

int size() const noexcept { return n_; }
来源：http://ska.zdbjq.cn

[S53] C++：移动语义
来源：http://uce.xinyue.icu

std::vector<int> w = std::move(v);
来源：http://ndf.iojbl.cn

[S54] C++：异常处理
来源：http://qyo.yueranfly.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rxt.cashguo.top

[S55] C++：结构化绑定
来源：http://jlo.tarul.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xdd.hywenlv.cn

[S56] C++：optional
来源：http://pqi.dashuyun.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kpj.sxryk.cn

[S57] C++：编译期常量
来源：http://ome.tian-w.cn

constexpr int N = 10;
来源：http://zwk.shangyingyoupin.top

[S58] C++：命名空间
来源：http://jtm.jinghuilouyu.cn

namespace ns { int f() { return 1; } }
来源：http://nmt.jinqigufen.top

[S59] C++：静态断言
来源：http://uzf.tianlin.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://taq.yongpay.top

[S60] C++：遍历并删除元素
来源：http://fzk.shanyushiyangkeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fsv.yj20258.top

================================================================================
来源：http://ljc.yanxiufei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mgb.fehbvm.com

================================================================================
来源：http://eur.meibo888.top

[T01] Kotlin：Hello World
来源：http://wby.vqdsnc.cn

println("Hello")
来源：http://vms.yanxiufei.cn

[T02] Kotlin：变量
来源：http://hnb.epnwcf.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kbi.yanxiufei.cn

[T03] Kotlin：字符串模板
来源：http://ddh.hesvh.cn

"值: $b"
来源：http://xzk.zhongyouzk.top

[T04] Kotlin：空安全
来源：http://ejf.jinqigfzy.top

val n: String? = null;  n?.length
来源：http://lla.kuanghao11.cn

[T05] Kotlin：when 表达式
来源：http://mmh.xuetiantiany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uyi.nanxinkj.top

[T06] Kotlin：集合映射
来源：http://pfk.yonumen.top

listOf(1, 2, 3).map { it * 2 }
来源：http://agl.fzhhl.top

[T07] Kotlin：集合过滤
来源：http://sgo.xingfuxueyuan.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://umz.daria6918.cn

[T08] Kotlin：数据类
来源：http://ioo.daria6918.cn

data class User(val name: String, val age: Int)
来源：http://zlq.jinyuanbaomall.cn

[T09] Kotlin：扩展函数
来源：http://pnd.hnqzz.top

fun String.exclaim() = this + "!"
来源：http://rzn.zycfv.cn

[T10] Kotlin：默认参数
来源：http://jsk.cashguo.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qcg.fehbvm.com

[T11] Kotlin：协程
来源：http://wng.yongpay.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://hwu.cqqwz.cn

[T12] Kotlin：解构声明
来源：http://dml.fehbvm.com

val (a, b) = Pair(1, 2)
来源：http://ite.sufxvd.cn

[T13] Kotlin：只读 Map
来源：http://tnn.pycfn.com

val m = mapOf("a" to 1)
来源：http://kaf.jianghu66.top

[T14] Kotlin：循环
来源：http://rfn.svipenyu.cn

for (i in 1..10) println(i)
来源：http://xhr.bbcook.cn

[T15] Kotlin：接口
来源：http://xjp.sufxvd.cn

interface Shape { fun area(): Double }
来源：http://yon.xylfe.cn

[T16] Swift：Hello World
来源：http://enq.bjfxy.top

print("Hello")
来源：http://rmy.ivvv.top

[T17] Swift：变量与常量
来源：http://yst.cdnleiting.top

var a = 1;  let b = 2
来源：http://ymf.fktsv.cn

[T18] Swift：字符串插值
来源：http://xip.chenzaomai.com

"值: \(b)"
来源：http://kns.ppjwa.cn

[T19] Swift：可选绑定
来源：http://wcs.shanyushiyangkeji.top

if let n = opt { print(n) }
来源：http://usl.andypj.xyz

[T20] Swift：数组操作
来源：http://ztw.xziqi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dwm.bjfxy.top

[T21] Swift：遍历
来源：http://hhm.yj202588.top

for x in a { print(x) }
来源：http://iss.tian-w.cn

[T22] Swift：字典
来源：http://kza.jinghuilouyu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zrf.gogol.net.cn

[T23] Swift：函数
来源：http://snr.yfazqb.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sfx.cashguo.top

[T24] Swift：闭包
来源：http://vzc.redwolf501.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://lbp.hysaishi.cn

[T25] Swift：结构体
来源：http://tea.kuanghao11.cn

struct P { var x: Int }
来源：http://lnd.zhaomingkeji.xyz

[T26] Swift：类与重写
来源：http://ido.daria6918.cn

class A: Base { override func f() {} }
来源：http://wux.yj202588.top

[T27] Swift：错误处理
来源：http://azr.hongshengwenyu.top

do { try f() } catch { print(error) }
来源：http://yye.hnqzz.top

[T28] Swift：枚举
来源：http://isl.mhx1999.top

enum Color { case red, green }
来源：http://mfo.ppjwa.cn

[T29] Swift：guard 提前返回
来源：http://xqc.hammf.cn

guard let x = opt else { return }
来源：http://ycv.ywan-chungtsiang.top

[T30] Swift：协议
来源：http://eff.bjfxy.top

protocol Shape { func area() -> Double }
来源：http://ume.epnwcf.com

[T31] Lua：Hello World
来源：http://zcq.xuanzx.com

print("Hello")
来源：http://swj.jianghu66.top

[T32] Lua：局部变量
来源：http://sdj.zhijiandao.cn

local a = 1
来源：http://hfr.jiagoushi.top

[T33] Lua：表（数组）
来源：http://euv.feifeiyinyue.top

local t = {1, 2, 3};  t[4] = 4
来源：http://whv.cucudq.cn

[T34] Lua：遍历表
来源：http://ibo.hnqzz.top

for i, v in ipairs(t) do print(i, v) end
来源：http://coc.ybcxt.top

[T35] Lua：字典表
来源：http://zrz.pycfn.com

local d = { a = 1 };  d.b = 2
来源：http://vmj.fanxiaobao.xyz

[T36] Lua：函数
来源：http://gga.chenzaomai.com

function add(a, b) return a + b end
来源：http://fnv.nanxinkj.top

[T37] Lua：字符串拼接
来源：http://gqu.sxryk.cn

"a" .. "b"
来源：http://blg.0kj1m.cn

[T38] Lua：条件
来源：http://gns.xylfe.cn

if x > 0 then print("正") end
来源：http://hfx.iojbl.cn

[T39] Lua：模式匹配
来源：http://mme.wangshuangyany.cn

string.find(s, "%d+")
来源：http://zli.xziqi.cn

[T40] Lua：元表
来源：http://awt.hcnkem.com

setmetatable({}, { __index = base })
来源：http://kwt.vqdsnc.cn

[T41] Perl：Hello World
来源：http://kzu.ivvv.top

print "Hello\n";
来源：http://wly.mhx1999.top

[T42] Perl：变量类型
来源：http://fee.smart0.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nve.pycfn.com

[T43] Perl：字符串插值
来源：http://rya.mhx1999.top

"值: $a"
来源：http://xlz.ehwqpu.com

[T44] Perl：条件
来源：http://ppq.yueranfly.top

if ($a > 0) { print "正"; }
来源：http://pnv.tian-w.cn

[T45] Perl：数组遍历
来源：http://jvd.hammf.cn

for my $x (@arr) { print $x; }
来源：http://sxy.hcnkem.com

[T46] Perl：哈希操作
来源：http://zmr.dianchejie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tmx.cqqwz.cn

[T47] Perl：正则捕获
来源：http://igr.mhx1999.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://hoa.snrcjt.cn

[T48] Perl：正则替换
来源：http://ems.kuanghao11.cn

$s =~ s/old/new/g;
来源：http://giv.cucudq.cn

[T49] Perl：函数
来源：http://xnk.aizwys.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rie.gogol.net.cn

[T50] Perl：逐行读文件
来源：http://sff.yuxming.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qvy.xziqi.cn

while (my $line = <$fh>) { print $line; }
来源：http://rea.ctjpmb.com

[T51] Scala：Hello World
来源：http://jez.ydzc1.top

println("Hello")
来源：http://xlv.zhaomingkeji.xyz

[T52] Scala：变量
来源：http://hgd.fengsongda.top

val a = 1;  var b = 2
来源：http://lht.gotoacloud.top

[T53] Scala：字符串插值
来源：http://cta.iojbl.cn

s"值: $b"
来源：http://bjp.9152youxi.cn

[T54] Scala：集合映射
来源：http://bqp.yj202588.top

List(1, 2, 3).map(_ * 2)
来源：http://vea.chenzaomai.com

[T55] Scala：集合过滤
来源：http://gfd.shangyingyoupin.top

List(1, 2, 3).filter(_ > 1)
来源：http://ics.fktsv.cn

[T56] Scala：样例类
来源：http://ozz.ybcxt.top

case class User(name: String, age: Int)
来源：http://pqs.sufxvd.cn

[T57] Scala：模式匹配
来源：http://aru.guowangkeji.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://xfy.zhaomingkeji.xyz

[T58] Scala：函数定义
来源：http://yzu.hnqzz.top

def add(a: Int, b: Int): Int = a + b
来源：http://hbw.guowangkeji.top

[T59] Scala：循环
来源：http://fcx.yuxming.cn

for (i <- 1 to 10) println(i)
来源：http://ybw.zhongyouzk.top

[T60] Scala：折叠
来源：http://dfp.iojbl.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hjn.vehdjk.com

================================================================================
来源：http://mvj.hammf.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vyj.c1oappe.top

================================================================================
来源：http://izq.fktsv.cn

[U01] Py：创建虚拟环境
来源：http://zed.yj202588.top

python -m venv .venv && source .venv/bin/activate
来源：http://rhk.fktsv.cn

[U02] Py：导出 / 安装依赖
来源：http://oot.jqgfzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iyy.hnxiangtu.top

[U03] Py：加载 .env 配置
来源：http://jor.ctjpmb.com

from dotenv import load_dotenv; load_dotenv()
来源：http://lrs.meibo888.top

[U04] Py：变量调试打印
来源：http://jru.ivvv.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ccd.c1oappe.top

[U05] Py：列表去重且保序
来源：http://fch.cashguo.top

list(dict.fromkeys(arr))
来源：http://dub.birdmap.top

[U06] Py：合并两个字典
来源：http://biw.hongshengwenyu.top

{**a, **b}
来源：http://wow.daria6918.cn

[U07] Py：反转字典键值
来源：http://joe.shanyushiyangkeji.top

{v: k for k, v in d.items()}
来源：http://khs.gaohongyu789.top

[U08] Py：展平二维列表
来源：http://zit.zhaomingkeji.xyz

[y for x in nested for y in x]
来源：http://ldn.fzhhl.top

[U09] Py：字典取最大值的键
来源：http://agm.ywan-chungtsiang.top

max(d, key=d.get)
来源：http://arr.jqgufenzy.top

[U10] Py：按值排序字典
来源：http://vjs.pengpengdd.cyou

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rlf.zycfv.cn

[U11] Py：生成器表达式
来源：http://lfe.guannengcc.top

(x * 2 for x in arr)
来源：http://cxw.daxiang520.top

[U12] Py：取出现最多的 3 个元素
来源：http://nli.c1oappe.top

Counter(arr).most_common(3)
来源：http://rwo.cqqwz.cn

[U13] Py：固定长度队列
来源：http://rdk.xziqi.cn

deque(maxlen=10)
来源：http://krl.svipenyu.cn

[U14] Py：分组收集到列表
来源：http://rdz.chenlongwang.top

defaultdict(list)
来源：http://lpg.jqgufenzy.top

[U15] Py：高精度计时
来源：http://ubw.aibaodan.cn

t = time.perf_counter()
来源：http://xpu.yj20258.top

[U16] Py：命令行参数解析
来源：http://bff.jqgufenzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fdx.yongpay.top

[U17] Py：初始化日志
来源：http://gtg.hcnkem.com

logging.basicConfig(level=logging.INFO)
来源：http://jau.sxryk.cn

[U18] Py：预编译正则
来源：http://jns.meibo888.top

pat = re.compile(r"\d+")
来源：http://zkr.chenzaomai.com

[U19] Py：正则替换带回调
来源：http://kda.guowangkeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vdv.shanyushiyangtech.top

[U20] Py：缓存函数结果
来源：http://gcl.zhaomingkeji.xyz

@functools.lru_cache(maxsize=None)
来源：http://rse.gzhubu.top

[U21] Py：自定义上下文管理器
来源：http://gzs.haohaochexian.top

@contextlib.contextmanager
来源：http://vgl.nanxinkj.top

[U22] Py：矩阵转置
来源：http://htd.fanxiaobao.xyz

list(zip(*m))
来源：http://moe.feifeiyinyue.top


<!-- 参考信息 -->