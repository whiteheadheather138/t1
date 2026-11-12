代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://qrq.guowangkeji.top

[R70] 时间戳与互转
来源：http://ntk.zhijiandao.cn

date +%s;  date -d @1700000000
来源：http://elj.fanxiaobao.xyz

[R71] 日期格式化
来源：http://syo.xinyue.icu

date +"%Y-%m-%d %H:%M:%S"
来源：http://sib.jiagoushi.top

[R72] 等待端口就绪
来源：http://yvx.jinyuanbaomall.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wwg.hongshengwenyu.top

[R73] 分割大日志
来源：http://wsa.cucudq.cn

split -l 1000 big.log part_
来源：http://ldi.xuetiantiany.cn

[R74] 批量重命名
来源：http://mgw.tanke756.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bkn.zhiwuduotai.top

[R75] 导出环境变量
来源：http://dlt.jlsjyb.cn

export PATH="$HOME/bin:$PATH"
来源：http://nqs.birdmap.top

[R76] 使用临时文件
来源：http://pem.tanke756.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ffp.shzxlz.cn

[R77] 读取用户输入
来源：http://xum.xziqi.cn

read -rp "请输入: " ans
来源：http://vrc.feifeiyinyue.top

[R78] 交互式菜单
来源：http://hhw.zhiwuduotai.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vfe.hongshengwenyu.top

[R79] 解析命令行选项
来源：http://kny.hfpthk.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jyn.aibaodan.cn

[R80] 查看脚本执行耗时
来源：http://ipv.ehwqpu.com

time ./run.sh
来源：http://fdu.ybcxt.top

================================================================================
来源：http://kvk.chenzaomai.com

S. C / C++ 专题
来源：http://wka.tianlin.xyz

================================================================================
来源：http://ayh.zhongyouzk.top

[S01] C：Hello World
来源：http://zva.hammf.cn

#include <stdio.h>
来源：http://nwo.hnqzz.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vez.nanxuanxn.top

[S02] C：变量与格式化输出
来源：http://yri.yanxiufei.cn

int a = 10; printf("%d\n", a);
来源：http://uju.jqgfzy.top

[S03] C：读入整数
来源：http://eik.quarkkingdee.top

int x; scanf("%d", &x);
来源：http://xsi.epnwcf.com

[S04] C：字符串复制
来源：http://vne.pengpengdd.cyou

char dst[32]; strcpy(dst, "hi");
来源：http://ssc.tianlin.xyz

[S05] C：字符串长度
来源：http://ucl.hesvh.cn

strlen(s)
来源：http://qsy.zhijiandao.cn

[S06] C：字符串比较
来源：http://qvq.haohaochexian.top

strcmp(a, b) == 0
来源：http://frc.kuanghao11.cn

[S07] C：数组遍历求和
来源：http://dwf.kuanghao11.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wmu.nwbrower.top

[S08] C：动态内存分配与释放
来源：http://bbe.chenzaomai.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mlt.aizwys.cn

[S09] C：结构体定义与初始化
来源：http://tzh.0kj1m.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://atz.guannengcc.top

[S10] C：指针与解引用
来源：http://oal.ydjk.org.cn

int *p = &a;  *p = 5;
来源：http://mnt.vehdjk.com

[S11] C：逐行读文件
来源：http://whg.cucudq.cn

FILE *f = fopen("a.txt", "r");
来源：http://stn.52xcode.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nac.jqgufenzy.top

fclose(f);
来源：http://ltg.jinqigfzy.top

[S12] C：写文件
来源：http://kva.chenzaomai.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rew.cqqwz.cn

[S13] C：宏定义
来源：http://wde.zhiwuduotai.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zdh.hammf.cn

[S14] C：枚举
来源：http://gmu.sxryk.cn

enum Color { RED, GREEN, BLUE };
来源：http://zrb.wangdashe.top

[S15] C：类型转换
来源：http://oie.hnqzz.top

(double) a / b
来源：http://wcn.cheryme.top

[S16] C：位操作置位
来源：http://qsp.svipenyu.cn

x |= (1 << 3);
来源：http://kru.9152youxi.cn

[S17] C：安全拼接字符串
来源：http://tcb.ydjk.org.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tzw.shangyingyoupin.top

[S18] C：命令行参数
来源：http://nmm.birdmap.top

int main(int argc, char **argv)
来源：http://ebm.mhx1999.top

[S19] C：快速排序
来源：http://nxt.tian-w.cn

qsort(a, n, sizeof(int), cmp);
来源：http://oax.meibo888.top

[S20] C：二分查找
来源：http://uaa.yvedp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lgk.hnxiangtu.top

[S21] C：字符类别判断
来源：http://ryh.jinqigfzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ckt.hywenlv.cn

[S22] C：字符串转数字
来源：http://xgd.shzxlz.cn

atoi("42");  strtod("3.14", NULL);
来源：http://but.hongshengwenyu.top

[S23] C：随机数
来源：http://rzq.haohaochexian.top

srand(time(NULL));  int r = rand() % 100;
来源：http://aod.chenlongwang.top

[S24] C：获取本地时间
来源：http://dik.yuxming.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bdr.yj20258888.top

[S25] C：内存拷贝
来源：http://jdm.tarul.cn

memcpy(dst, src, n);
来源：http://ryf.havefunace.top

[S26] C：内存清零
来源：http://ekn.sxryk.cn

memset(a, 0, sizeof a);
来源：http://vnl.tarul.cn

[S27] C：定义常量
来源：http://hsz.xylfe.cn

const double PI = 3.14159;
来源：http://gmg.hfpthk.cn

[S28] C：静态变量
来源：http://uen.yj202588.top

static int counter = 0;
来源：http://hfb.yj20258888.top

[S29] C：变参函数
来源：http://hya.hysaishi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vxd.sjlbkw.cn

[S30] C：头文件保护
来源：http://exn.daria6918.cn

#ifndef X_H
来源：http://mzl.chenzaomai.com

#define X_H
来源：http://uie.yongpay.top

#endif
来源：http://ojg.zdbjq.cn

[S31] C++：Hello World
来源：http://ppp.jianghu66.top

#include <iostream>
来源：http://ebk.ehwqpu.com

int main() { std::cout << "Hello\n"; }
来源：http://zla.xuetiantiany.cn

[S32] C++：字符串
来源：http://loo.yongpay.top

std::string s = "hi";  s += "!";
来源：http://zxj.meibo888.top

[S33] C++：vector 增删
来源：http://cka.daria6918.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ohf.fengsongda.top

[S34] C++：遍历 vector
来源：http://dkj.chenjidiqi.icu

for (auto &x : v) { std::cout << x; }
来源：http://vyi.ppjwa.cn

[S35] C++：map
来源：http://syl.fktsv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://phy.nanxinkj.top

[S36] C++：unordered_map
来源：http://nei.tian-w.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ifj.vehdjk.com

[S37] C++：set
来源：http://mnf.jiagoushi.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rop.hesvh.cn

[S38] C++：排序
来源：http://xdr.316326.xyz

std::sort(v.begin(), v.end());
来源：http://hzt.tarul.cn

[S39] C++：自定义比较器排序
来源：http://bjx.zhaomingkeji.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fzg.gaohongyu789.top

[S40] C++：查找元素
来源：http://tro.smart0.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kss.xylfe.cn

[S41] C++：类与构造函数
来源：http://dgr.xuanzx.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tup.ctjpmb.com

[S42] C++：继承与虚函数
来源：http://clz.xingfuxueyuan.xyz

class B : public Base { public: void f() override {} };
来源：http://ths.yangfankeji.com

[S43] C++：智能指针
来源：http://ulr.gotoacloud.top

auto p = std::make_unique<int>(5);
来源：http://fxl.zdqjudy.top

[S44] C++：引用传参
来源：http://zgl.meibo888.top

void inc(int &x) { ++x; }
来源：http://vqp.dashuyun.cn

[S45] C++：lambda
来源：http://cnz.chenjidiqi.icu

auto add = [](int a, int b) { return a + b; };
来源：http://sbx.jlsjyb.cn

[S46] C++：函数模板
来源：http://cnk.jyoumei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pdw.yanxiufei.cn

[S47] C++：结构化绑定遍历
来源：http://aol.svipenyu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rnx.zhoulong.xyz

[S48] C++：逐行读文件
来源：http://vpo.yj20258888.top

std::ifstream in("a.txt");  std::string line;
来源：http://atp.sweek.top

while (std::getline(in, line)) { }
来源：http://fdm.gzhubu.top

[S49] C++：写文件
来源：http://ydi.yfazqb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bws.dashuyun.cn

[S50] C++：格式化数字
来源：http://lme.gzhubu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yrd.xziqi.cn

[S51] C++：显式类型转换
来源：http://gyq.yj20258.top

static_cast<double>(a) / b
来源：http://nor.guannengcc.top

[S52] C++：const 与 noexcept
来源：http://ivr.dianchejie.cn

int size() const noexcept { return n_; }
来源：http://xjb.yj20258888.top

[S53] C++：移动语义
来源：http://vxd.guannengcc.top

std::vector<int> w = std::move(v);
来源：http://kma.svipenyu.cn

[S54] C++：异常处理
来源：http://cwn.xuanzx.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ggz.wangdashe.top

[S55] C++：结构化绑定
来源：http://vkx.xziqi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wrv.uphjek.com

[S56] C++：optional
来源：http://sco.gaohongyu789.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wjx.nanxuanxn.top

[S57] C++：编译期常量
来源：http://bka.aibaodan.cn

constexpr int N = 10;
来源：http://lca.zhengqikj.top

[S58] C++：命名空间
来源：http://wmf.pengpengdd.cyou

namespace ns { int f() { return 1; } }
来源：http://dwu.shangyingyoupin.top

[S59] C++：静态断言
来源：http://pcd.birdmap.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ijf.pengpengdd.cyou

[S60] C++：遍历并删除元素
来源：http://uow.jlsjyb.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://btc.hesvh.cn

================================================================================
来源：http://tbm.ydzc1.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rfk.zhiwuduotai.top

================================================================================
来源：http://umu.yuxming.cn

[T01] Kotlin：Hello World
来源：http://dth.xinyue.icu

println("Hello")
来源：http://iwl.daria6918.cn

[T02] Kotlin：变量
来源：http://lbj.zdbjq.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://giz.fehbvm.com

[T03] Kotlin：字符串模板
来源：http://oyk.sxryk.cn

"值: $b"
来源：http://aut.52xcode.cn

[T04] Kotlin：空安全
来源：http://cts.havefunace.top

val n: String? = null;  n?.length
来源：http://qzh.daxiang520.top

[T05] Kotlin：when 表达式
来源：http://kqa.andypj.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xlq.zhijiandao.cn

[T06] Kotlin：集合映射
来源：http://fey.zdqjudy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://olx.yuanzhike.top

[T07] Kotlin：集合过滤
来源：http://sdn.wangdashe.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://fmx.smart0.xyz

[T08] Kotlin：数据类
来源：http://sdg.ctjpmb.com

data class User(val name: String, val age: Int)
来源：http://qyp.hongshengwenyu.top

[T09] Kotlin：扩展函数
来源：http://fxn.yj20258888.top

fun String.exclaim() = this + "!"
来源：http://znk.dashuyun.cn

[T10] Kotlin：默认参数
来源：http://aos.bjfxy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://isn.hammf.cn

[T11] Kotlin：协程
来源：http://mra.sysykeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://bos.xylfe.cn

[T12] Kotlin：解构声明
来源：http://jcu.jyoumei.cn

val (a, b) = Pair(1, 2)
来源：http://uum.tian-w.cn

[T13] Kotlin：只读 Map
来源：http://edl.yvedp.cn

val m = mapOf("a" to 1)
来源：http://heo.zdqjudy.top

[T14] Kotlin：循环
来源：http://ddy.xingfuxueyuan.xyz

for (i in 1..10) println(i)
来源：http://zfx.zhengqikj.top

[T15] Kotlin：接口
来源：http://grk.sufxvd.cn

interface Shape { fun area(): Double }
来源：http://xdw.hnqzz.top

[T16] Swift：Hello World
来源：http://mly.nanxinkj.top

print("Hello")
来源：http://glp.yj20258888.top

[T17] Swift：变量与常量
来源：http://oku.svipenyu.cn

var a = 1;  let b = 2
来源：http://aam.zdqjudy.top

[T18] Swift：字符串插值
来源：http://uxd.zhiwuduotai.top

"值: \(b)"
来源：http://ima.jinqigufen.top

[T19] Swift：可选绑定
来源：http://usy.svipenyu.cn

if let n = opt { print(n) }
来源：http://kvi.ydzc1.top

[T20] Swift：数组操作
来源：http://bnq.daxiang520.top

var a = [1, 2, 3];  a.append(4)
来源：http://rmm.shangyingyoupin.top

[T21] Swift：遍历
来源：http://ank.tanke756.top

for x in a { print(x) }
来源：http://adz.jqgufenzy.top

[T22] Swift：字典
来源：http://gva.gzhubu.top

var d = ["a": 1];  d["b"] = 2
来源：http://vvq.fengsongda.top

[T23] Swift：函数
来源：http://erp.shzxlz.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fsz.ivvv.top

[T24] Swift：闭包
来源：http://bzt.shuidangran.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://mlq.hnqzz.top

[T25] Swift：结构体
来源：http://vsx.chenjidiqi.icu

struct P { var x: Int }
来源：http://hnr.52xcode.cn

[T26] Swift：类与重写
来源：http://owh.yj202588.top

class A: Base { override func f() {} }
来源：http://nun.cheryme.top

[T27] Swift：错误处理
来源：http://uvx.guowangkeji.top

do { try f() } catch { print(error) }
来源：http://hlm.gotoacloud.top

[T28] Swift：枚举
来源：http://lzs.wangdashe.top

enum Color { case red, green }
来源：http://gnb.hammf.cn

[T29] Swift：guard 提前返回
来源：http://pyp.redwolf501.top

guard let x = opt else { return }
来源：http://spj.tarul.cn

[T30] Swift：协议
来源：http://arz.pengpengdd.cyou

protocol Shape { func area() -> Double }
来源：http://klm.hywenlv.cn

[T31] Lua：Hello World
来源：http://txo.jiagoushi.top

print("Hello")
来源：http://loh.zhaomingkeji.xyz

[T32] Lua：局部变量
来源：http://bfm.aibaodan.cn

local a = 1
来源：http://rrr.birdmap.top

[T33] Lua：表（数组）
来源：http://bzy.ppjwa.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zcg.nwbrower.top

[T34] Lua：遍历表
来源：http://aad.shzxlz.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jdd.cucudq.cn

[T35] Lua：字典表
来源：http://rws.hcnkem.com

local d = { a = 1 };  d.b = 2
来源：http://ddn.redwolf501.top

[T36] Lua：函数
来源：http://nab.jinyuanbaomall.cn

function add(a, b) return a + b end
来源：http://plk.shanyushiyangkeji.top

[T37] Lua：字符串拼接
来源：http://say.zhengqikj.top

"a" .. "b"
来源：http://gam.52xcode.cn

[T38] Lua：条件
来源：http://hax.nanxinkj.top

if x > 0 then print("正") end
来源：http://inf.yanxiufei.cn

[T39] Lua：模式匹配
来源：http://nit.yj20258888.top

string.find(s, "%d+")
来源：http://gpt.ydzc1.top

[T40] Lua：元表
来源：http://sro.sjlbkw.cn

setmetatable({}, { __index = base })
来源：http://pdz.nanxinkj.top

[T41] Perl：Hello World
来源：http://nky.chenlongwang.top

print "Hello\n";
来源：http://xqa.ybcxt.top

[T42] Perl：变量类型
来源：http://yot.kuanghao11.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nyb.andypj.xyz

[T43] Perl：字符串插值
来源：http://ewn.zhaomingkeji.xyz

"值: $a"
来源：http://kpm.zhaomingkeji.xyz

[T44] Perl：条件
来源：http://mdz.sysykeji.top

if ($a > 0) { print "正"; }
来源：http://ayp.yuanzhike.top

[T45] Perl：数组遍历
来源：http://wlm.cucudq.cn

for my $x (@arr) { print $x; }
来源：http://sqz.ctjpmb.com

[T46] Perl：哈希操作
来源：http://mdg.jinqigfzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://iep.pengpengdd.cyou

[T47] Perl：正则捕获
来源：http://wgo.yfazqb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://avk.tarul.cn

[T48] Perl：正则替换
来源：http://asa.gaohongyu789.top

$s =~ s/old/new/g;
来源：http://luz.nwbrower.top

[T49] Perl：函数
来源：http://nsm.xuetiantiany.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fnh.yj20258888.top

[T50] Perl：逐行读文件
来源：http://smi.guowangkeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://phy.nanxinkj.top

while (my $line = <$fh>) { print $line; }
来源：http://uuf.zhijiandao.cn

[T51] Scala：Hello World
来源：http://ftn.mhx1999.top

println("Hello")
来源：http://tiw.yj202588.top

[T52] Scala：变量
来源：http://spv.cashguo.top

val a = 1;  var b = 2
来源：http://zww.jinqigfzy.top

[T53] Scala：字符串插值
来源：http://fun.sjlbkw.cn

s"值: $b"
来源：http://lpt.zycfv.cn

[T54] Scala：集合映射
来源：http://guw.feifeiyinyue.top

List(1, 2, 3).map(_ * 2)
来源：http://han.dashuyun.cn

[T55] Scala：集合过滤
来源：http://yba.jiagoushi.top

List(1, 2, 3).filter(_ > 1)
来源：http://cxb.zhiwuduotai.top

[T56] Scala：样例类
来源：http://fkn.xingfuxueyuan.xyz

case class User(name: String, age: Int)
来源：http://naq.bjfxy.top

[T57] Scala：模式匹配
来源：http://xno.gotoacloud.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://lbn.uphjek.com

[T58] Scala：函数定义
来源：http://soa.ppjwa.cn

def add(a: Int, b: Int): Int = a + b
来源：http://due.aibaodan.cn

[T59] Scala：循环
来源：http://iav.jlsjyb.cn

for (i <- 1 to 10) println(i)
来源：http://qlq.quarkkingdee.top

[T60] Scala：折叠
来源：http://oog.chenjidiqi.icu

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vwu.uphjek.com

================================================================================
来源：http://czm.jinqigfzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://idc.jqgufenzy.top

================================================================================
来源：http://jgw.jlsjyb.cn

[U01] Py：创建虚拟环境
来源：http://fso.guannengcc.top

python -m venv .venv && source .venv/bin/activate
来源：http://dic.birdmap.top

[U02] Py：导出 / 安装依赖
来源：http://dok.jinqigufen.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lyw.jlsjyb.cn

[U03] Py：加载 .env 配置
来源：http://oty.yuanzhike.top

from dotenv import load_dotenv; load_dotenv()
来源：http://lmq.jlsjyb.cn

[U04] Py：变量调试打印
来源：http://wxf.zhoulong.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://oau.xziqi.cn

[U05] Py：列表去重且保序
来源：http://xag.tanke756.top

list(dict.fromkeys(arr))
来源：http://oba.chenzaomai.com

[U06] Py：合并两个字典
来源：http://grk.jiagoushi.top

{**a, **b}
来源：http://btr.guannengcc.top

[U07] Py：反转字典键值
来源：http://hkr.iojbl.cn

{v: k for k, v in d.items()}
来源：http://gba.ywan-chungtsiang.top

[U08] Py：展平二维列表
来源：http://gxj.yongpay.top

[y for x in nested for y in x]
来源：http://hkq.bjfxy.top

[U09] Py：字典取最大值的键
来源：http://quc.xuetiantiany.cn

max(d, key=d.get)
来源：http://uqh.epnwcf.com

[U10] Py：按值排序字典
来源：http://rlc.gogol.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jkp.hnxiangtu.top


<!-- 参考信息 -->