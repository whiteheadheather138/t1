代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://npw.birdmap.top

[R70] 时间戳与互转
来源：http://wiq.bjfxy.top

date +%s;  date -d @1700000000
来源：http://ahx.hfpthk.cn

[R71] 日期格式化
来源：http://gjm.yj20258888.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://rrh.snrcjt.cn

[R72] 等待端口就绪
来源：http://qzk.hesvh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wzl.bbcook.cn

[R73] 分割大日志
来源：http://roy.redwolf501.top

split -l 1000 big.log part_
来源：http://gwn.chenzaomai.com

[R74] 批量重命名
来源：http://rel.zhongyouzk.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mze.cqqwz.cn

[R75] 导出环境变量
来源：http://uvr.jinqigufen.top

export PATH="$HOME/bin:$PATH"
来源：http://izs.uphjek.com

[R76] 使用临时文件
来源：http://ugl.uphjek.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vdz.hnxiangtu.top

[R77] 读取用户输入
来源：http://stm.jyoumei.cn

read -rp "请输入: " ans
来源：http://qet.sjlbkw.cn

[R78] 交互式菜单
来源：http://ksh.hysaishi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://adc.cheryme.top

[R79] 解析命令行选项
来源：http://fxx.fanxiaobao.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ssh.andypj.xyz

[R80] 查看脚本执行耗时
来源：http://qiq.vehdjk.com

time ./run.sh
来源：http://gco.zhongyouzk.top

================================================================================
来源：http://yhn.ydzc1.top

S. C / C++ 专题
来源：http://kkl.zycfv.cn

================================================================================
来源：http://ovd.nanxuanxn.top

[S01] C：Hello World
来源：http://mjc.fktsv.cn

#include <stdio.h>
来源：http://nwg.jinqigufen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://cdy.meibo888.top

[S02] C：变量与格式化输出
来源：http://xtx.jinyuanbaomall.cn

int a = 10; printf("%d\n", a);
来源：http://eyy.yuxming.cn

[S03] C：读入整数
来源：http://jld.snrcjt.cn

int x; scanf("%d", &x);
来源：http://sfb.chenzaomai.com

[S04] C：字符串复制
来源：http://mgu.cucudq.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jtj.fanxiaobao.xyz

[S05] C：字符串长度
来源：http://kyp.ydzc1.top

strlen(s)
来源：http://kjo.ppjwa.cn

[S06] C：字符串比较
来源：http://ryq.daxiang520.top

strcmp(a, b) == 0
来源：http://jgx.dashuyun.cn

[S07] C：数组遍历求和
来源：http://nvj.svipenyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sea.chenzaomai.com

[S08] C：动态内存分配与释放
来源：http://dkg.tian-w.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://exr.shzxlz.cn

[S09] C：结构体定义与初始化
来源：http://oyw.zhixingplan.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://idm.9152youxi.cn

[S10] C：指针与解引用
来源：http://dan.tanke756.top

int *p = &a;  *p = 5;
来源：http://vqs.aizwys.cn

[S11] C：逐行读文件
来源：http://doe.shangyingyoupin.top

FILE *f = fopen("a.txt", "r");
来源：http://whl.yuanzhike.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://iws.jlsjyb.cn

fclose(f);
来源：http://abn.feifeiyinyue.top

[S12] C：写文件
来源：http://xud.ybcxt.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://swt.tarul.cn

[S13] C：宏定义
来源：http://kmp.yj20258888.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zkg.cqqwz.cn

[S14] C：枚举
来源：http://vnx.zhaomingkeji.xyz

enum Color { RED, GREEN, BLUE };
来源：http://yft.daria6918.cn

[S15] C：类型转换
来源：http://chy.yongpay.top

(double) a / b
来源：http://zih.chenzaomai.com

[S16] C：位操作置位
来源：http://utp.zhiwuduotai.top

x |= (1 << 3);
来源：http://pgc.tianlin.xyz

[S17] C：安全拼接字符串
来源：http://xah.yvedp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rfq.cqqwz.cn

[S18] C：命令行参数
来源：http://qka.sweek.top

int main(int argc, char **argv)
来源：http://jkb.yfazqb.com

[S19] C：快速排序
来源：http://xyg.feifeiyinyue.top

qsort(a, n, sizeof(int), cmp);
来源：http://wqc.jianghu66.top

[S20] C：二分查找
来源：http://vwx.cheryme.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rop.sysykeji.top

[S21] C：字符类别判断
来源：http://wzv.hywenlv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rdo.dianchejie.cn

[S22] C：字符串转数字
来源：http://hks.shzxlz.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qhd.epnwcf.com

[S23] C：随机数
来源：http://rqg.fanxiaobao.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://jzs.ppjwa.cn

[S24] C：获取本地时间
来源：http://isv.smart0.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jfk.havefunace.top

[S25] C：内存拷贝
来源：http://uye.sysykeji.top

memcpy(dst, src, n);
来源：http://aja.yongpay.top

[S26] C：内存清零
来源：http://tan.chenzaomai.com

memset(a, 0, sizeof a);
来源：http://lrf.0kj1m.cn

[S27] C：定义常量
来源：http://lvx.sufxvd.cn

const double PI = 3.14159;
来源：http://qpa.vehdjk.com

[S28] C：静态变量
来源：http://zny.ywan-chungtsiang.top

static int counter = 0;
来源：http://rpv.tanke756.top

[S29] C：变参函数
来源：http://ses.havefunace.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hnl.sjlbkw.cn

[S30] C：头文件保护
来源：http://ngc.yj202588.top

#ifndef X_H
来源：http://tff.ivvv.top

#define X_H
来源：http://eya.iojbl.cn

#endif
来源：http://ixd.jinqigfzy.top

[S31] C++：Hello World
来源：http://zcs.zdqjudy.top

#include <iostream>
来源：http://npg.jinghuilouyu.cn

int main() { std::cout << "Hello\n"; }
来源：http://hgn.cucudq.cn

[S32] C++：字符串
来源：http://gld.fanxiaobao.xyz

std::string s = "hi";  s += "!";
来源：http://odp.quarkkingdee.top

[S33] C++：vector 增删
来源：http://hsr.chenzaomai.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jup.zhengqikj.top

[S34] C++：遍历 vector
来源：http://zow.hesvh.cn

for (auto &x : v) { std::cout << x; }
来源：http://plm.ivvv.top

[S35] C++：map
来源：http://wvb.yvedp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pyq.shzxlz.cn

[S36] C++：unordered_map
来源：http://als.quarkkingdee.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gbm.dashuyun.cn

[S37] C++：set
来源：http://tsz.epnwcf.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hnj.zhaomingkeji.xyz

[S38] C++：排序
来源：http://jpm.haohaochexian.top

std::sort(v.begin(), v.end());
来源：http://fbj.tarul.cn

[S39] C++：自定义比较器排序
来源：http://bze.ivvv.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vpd.ydjk.org.cn

[S40] C++：查找元素
来源：http://qtb.hysaishi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ylg.ppjwa.cn

[S41] C++：类与构造函数
来源：http://pfl.sjlbkw.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tww.yuanzhike.top

[S42] C++：继承与虚函数
来源：http://zjt.tanke756.top

class B : public Base { public: void f() override {} };
来源：http://sct.wangshuangyany.cn

[S43] C++：智能指针
来源：http://jur.zhiwuduotai.top

auto p = std::make_unique<int>(5);
来源：http://osr.andypj.xyz

[S44] C++：引用传参
来源：http://xkp.guannengcc.top

void inc(int &x) { ++x; }
来源：http://kpr.316326.xyz

[S45] C++：lambda
来源：http://uay.gotoacloud.top

auto add = [](int a, int b) { return a + b; };
来源：http://okh.tanke756.top

[S46] C++：函数模板
来源：http://lpb.hongshengwenyu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vjj.nwbrower.top

[S47] C++：结构化绑定遍历
来源：http://phz.ehwqpu.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://def.zhongyouzk.top

[S48] C++：逐行读文件
来源：http://bta.daxiang520.top

std::ifstream in("a.txt");  std::string line;
来源：http://unq.fengsongda.top

while (std::getline(in, line)) { }
来源：http://kec.jinqigufen.top

[S49] C++：写文件
来源：http://asr.xylfe.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tze.pycfn.com

[S50] C++：格式化数字
来源：http://ajx.chenjidiqi.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ooy.fktsv.cn

[S51] C++：显式类型转换
来源：http://cet.shzxlz.cn

static_cast<double>(a) / b
来源：http://int.ehwqpu.com

[S52] C++：const 与 noexcept
来源：http://pdj.andypj.xyz

int size() const noexcept { return n_; }
来源：http://jre.yj202588.top

[S53] C++：移动语义
来源：http://yxd.bjfxy.top

std::vector<int> w = std::move(v);
来源：http://plp.zdbjq.cn

[S54] C++：异常处理
来源：http://kbk.dashuyun.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lpw.quarkkingdee.top

[S55] C++：结构化绑定
来源：http://dar.jiagoushi.top

auto [a, b] = std::make_pair(1, 2);
来源：http://gtv.xinyue.icu

[S56] C++：optional
来源：http://rch.c1oappe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zpx.jqgufenzy.top

[S57] C++：编译期常量
来源：http://mnj.hongshengwenyu.top

constexpr int N = 10;
来源：http://pwt.zdbjq.cn

[S58] C++：命名空间
来源：http://pxc.sufxvd.cn

namespace ns { int f() { return 1; } }
来源：http://wlb.0kj1m.cn

[S59] C++：静态断言
来源：http://ndy.hfpthk.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qbs.yvedp.cn

[S60] C++：遍历并删除元素
来源：http://gzy.fengsongda.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rhk.chenjidiqi.icu

================================================================================
来源：http://jpc.mhx1999.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ljj.hnqzz.top

================================================================================
来源：http://msg.hcnkem.com

[T01] Kotlin：Hello World
来源：http://sbb.mhx1999.top

println("Hello")
来源：http://wll.uphjek.com

[T02] Kotlin：变量
来源：http://gyz.hammf.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qot.shuidangran.top

[T03] Kotlin：字符串模板
来源：http://kvx.quarkkingdee.top

"值: $b"
来源：http://zrs.fehbvm.com

[T04] Kotlin：空安全
来源：http://mpx.xingfuxueyuan.xyz

val n: String? = null;  n?.length
来源：http://ksx.ybcxt.top

[T05] Kotlin：when 表达式
来源：http://ykz.gotoacloud.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zvu.havefunace.top

[T06] Kotlin：集合映射
来源：http://vxd.shangyingyoupin.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hob.hesvh.cn

[T07] Kotlin：集合过滤
来源：http://ozz.nanxinkj.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://izw.chenzaomai.com

[T08] Kotlin：数据类
来源：http://ojz.epnwcf.com

data class User(val name: String, val age: Int)
来源：http://tez.0kj1m.cn

[T09] Kotlin：扩展函数
来源：http://jed.cheryme.top

fun String.exclaim() = this + "!"
来源：http://pxr.yvedp.cn

[T10] Kotlin：默认参数
来源：http://iyb.316326.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://wmm.xylfe.cn

[T11] Kotlin：协程
来源：http://rcl.sufxvd.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dgk.yanxiufei.cn

[T12] Kotlin：解构声明
来源：http://xyt.yuanzhike.top

val (a, b) = Pair(1, 2)
来源：http://whv.yanxiufei.cn

[T13] Kotlin：只读 Map
来源：http://dpx.jinyuanbaomall.cn

val m = mapOf("a" to 1)
来源：http://nck.ppjwa.cn

[T14] Kotlin：循环
来源：http://syz.fktsv.cn

for (i in 1..10) println(i)
来源：http://ach.jinyuanbaomall.cn

[T15] Kotlin：接口
来源：http://jbu.wangdashe.top

interface Shape { fun area(): Double }
来源：http://skg.jinyuanbaomall.cn

[T16] Swift：Hello World
来源：http://tfh.jinghuilouyu.cn

print("Hello")
来源：http://cqs.fktsv.cn

[T17] Swift：变量与常量
来源：http://xnd.iojbl.cn

var a = 1;  let b = 2
来源：http://kky.zhiwuduotai.top

[T18] Swift：字符串插值
来源：http://pur.gaohongyu789.top

"值: \(b)"
来源：http://afd.ivvv.top

[T19] Swift：可选绑定
来源：http://hae.xuanzx.com

if let n = opt { print(n) }
来源：http://yjk.zdbjq.cn

[T20] Swift：数组操作
来源：http://oqh.hcnkem.com

var a = [1, 2, 3];  a.append(4)
来源：http://mcf.chenlongwang.top

[T21] Swift：遍历
来源：http://zbt.zdqjudy.top

for x in a { print(x) }
来源：http://hop.zdqjudy.top

[T22] Swift：字典
来源：http://zih.jlsjyb.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ucy.ctjpmb.com

[T23] Swift：函数
来源：http://hsn.kuanghao11.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rpo.zycfv.cn

[T24] Swift：闭包
来源：http://ofe.kuanghao11.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ucj.kuanghao11.cn

[T25] Swift：结构体
来源：http://hqy.haohaochexian.top

struct P { var x: Int }
来源：http://iue.nwbrower.top

[T26] Swift：类与重写
来源：http://jjc.cheryme.top

class A: Base { override func f() {} }
来源：http://jnk.xylfe.cn

[T27] Swift：错误处理
来源：http://nxw.shuidangran.top

do { try f() } catch { print(error) }
来源：http://zhd.xziqi.cn

[T28] Swift：枚举
来源：http://fwi.ydjk.org.cn

enum Color { case red, green }
来源：http://nzn.9152youxi.cn

[T29] Swift：guard 提前返回
来源：http://xkt.nanxinkj.top

guard let x = opt else { return }
来源：http://pqf.cqqwz.cn

[T30] Swift：协议
来源：http://pvc.vehdjk.com

protocol Shape { func area() -> Double }
来源：http://bne.hcnkem.com

[T31] Lua：Hello World
来源：http://bxk.kuanghao11.cn

print("Hello")
来源：http://jkl.nanxinkj.top

[T32] Lua：局部变量
来源：http://wma.yj202588.top

local a = 1
来源：http://zup.jinghuilouyu.cn

[T33] Lua：表（数组）
来源：http://wdo.fehbvm.com

local t = {1, 2, 3};  t[4] = 4
来源：http://kbi.xinyue.icu

[T34] Lua：遍历表
来源：http://cnw.yanxiufei.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://sjm.sysykeji.top

[T35] Lua：字典表
来源：http://lgr.jinqigfzy.top

local d = { a = 1 };  d.b = 2
来源：http://mva.iojbl.cn

[T36] Lua：函数
来源：http://gkx.ehwqpu.com

function add(a, b) return a + b end
来源：http://kid.zhengqikj.top

[T37] Lua：字符串拼接
来源：http://rwk.sweek.top

"a" .. "b"
来源：http://wbo.fehbvm.com

[T38] Lua：条件
来源：http://aku.jyoumei.cn

if x > 0 then print("正") end
来源：http://gpd.hongshengwenyu.top

[T39] Lua：模式匹配
来源：http://fqg.dianchejie.cn

string.find(s, "%d+")
来源：http://amv.hnxiangtu.top

[T40] Lua：元表
来源：http://ynf.tianlin.xyz

setmetatable({}, { __index = base })
来源：http://orp.sxryk.cn

[T41] Perl：Hello World
来源：http://jqv.birdmap.top

print "Hello\n";
来源：http://gzw.tianlin.xyz

[T42] Perl：变量类型
来源：http://qtr.jiagoushi.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zdh.jinqigfzy.top

[T43] Perl：字符串插值
来源：http://fns.haohaochexian.top

"值: $a"
来源：http://daa.hnqzz.top

[T44] Perl：条件
来源：http://dcc.316326.xyz

if ($a > 0) { print "正"; }
来源：http://kiw.fanxiaobao.xyz

[T45] Perl：数组遍历
来源：http://rhl.hnqzz.top

for my $x (@arr) { print $x; }
来源：http://dib.guannengcc.top

[T46] Perl：哈希操作
来源：http://jsp.hywenlv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ccd.ydjk.org.cn

[T47] Perl：正则捕获
来源：http://mmq.chenjidiqi.icu

if ($s =~ /(\d+)/) { print $1; }
来源：http://mhz.guannengcc.top

[T48] Perl：正则替换
来源：http://qds.hywenlv.cn

$s =~ s/old/new/g;
来源：http://wap.yonumen.top

[T49] Perl：函数
来源：http://dfr.zhongyouzk.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lhr.fzhhl.top

[T50] Perl：逐行读文件
来源：http://tjc.zhixingplan.top

open my $fh, "<", "a.txt" or die $!;
来源：http://syd.ctjpmb.com

while (my $line = <$fh>) { print $line; }
来源：http://clx.nwbrower.top

[T51] Scala：Hello World
来源：http://mkp.zhengqikj.top

println("Hello")
来源：http://ors.ctjpmb.com

[T52] Scala：变量
来源：http://ife.shanyushiyangkeji.top

val a = 1;  var b = 2
来源：http://htp.pycfn.com

[T53] Scala：字符串插值
来源：http://onl.hesvh.cn

s"值: $b"
来源：http://xji.cashguo.top

[T54] Scala：集合映射
来源：http://aou.sysykeji.top

List(1, 2, 3).map(_ * 2)
来源：http://eqs.zhengqikj.top

[T55] Scala：集合过滤
来源：http://ngz.snrcjt.cn

List(1, 2, 3).filter(_ > 1)
来源：http://uoq.jqgfzy.top

[T56] Scala：样例类
来源：http://rtk.ctjpmb.com

case class User(name: String, age: Int)
来源：http://qpq.fehbvm.com

[T57] Scala：模式匹配
来源：http://dzv.ydjk.org.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://btp.cashguo.top

[T58] Scala：函数定义
来源：http://tke.hesvh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wcg.zhixingplan.top

[T59] Scala：循环
来源：http://fgk.ywan-chungtsiang.top

for (i <- 1 to 10) println(i)
来源：http://zkt.epnwcf.com

[T60] Scala：折叠
来源：http://aoy.sjlbkw.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rpj.zycfv.cn

================================================================================
来源：http://znn.daria6918.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gnj.hnqzz.top

================================================================================
来源：http://ebs.hnqzz.top

[U01] Py：创建虚拟环境
来源：http://wox.zhongyouzk.top

python -m venv .venv && source .venv/bin/activate
来源：http://cvh.wangdashe.top

[U02] Py：导出 / 安装依赖
来源：http://ggq.wangdashe.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ssm.ybcxt.top

[U03] Py：加载 .env 配置
来源：http://chi.hfpthk.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fzf.aibaodan.cn

[U04] Py：变量调试打印
来源：http://ghu.hcnkem.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://quk.tian-w.cn

[U05] Py：列表去重且保序
来源：http://nup.zhongyouzk.top

list(dict.fromkeys(arr))
来源：http://oen.cheryme.top

[U06] Py：合并两个字典
来源：http://lhw.gogol.net.cn

{**a, **b}
来源：http://jrk.iojbl.cn

[U07] Py：反转字典键值
来源：http://dik.yj20258888.top

{v: k for k, v in d.items()}
来源：http://rxm.iojbl.cn

[U08] Py：展平二维列表
来源：http://xmk.hfpthk.cn

[y for x in nested for y in x]
来源：http://etf.dashuyun.cn

[U09] Py：字典取最大值的键
来源：http://mhm.chenzaomai.com

max(d, key=d.get)
来源：http://bsv.jqgufenzy.top

[U10] Py：按值排序字典
来源：http://odj.havefunace.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ptu.yueranfly.top


<!-- 参考信息 -->