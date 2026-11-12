代发 wailian999

split -l 1000 big.log part_
来源：http://jnx.xuanzx.com

[R74] 批量重命名
来源：http://zuk.hywenlv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qdf.vqdsnc.cn

[R75] 导出环境变量
来源：http://oxq.zhijiandao.cn

export PATH="$HOME/bin:$PATH"
来源：http://lvf.ywan-chungtsiang.top

[R76] 使用临时文件
来源：http://ltj.kuanghao11.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yzw.hnxiangtu.top

[R77] 读取用户输入
来源：http://gzd.iojbl.cn

read -rp "请输入: " ans
来源：http://qpe.gzhubu.top

[R78] 交互式菜单
来源：http://okg.uphjek.com

select opt in a b c; do echo "$opt"; break; done
来源：http://rpt.sweek.top

[R79] 解析命令行选项
来源：http://dea.yj20258.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xed.mhx1999.top

[R80] 查看脚本执行耗时
来源：http://nil.nwbrower.top

time ./run.sh
来源：http://uuc.ivvv.top

================================================================================
来源：http://ysg.sysykeji.top

S. C / C++ 专题
来源：http://gyr.ppjwa.cn

================================================================================
来源：http://rke.yfazqb.com

[S01] C：Hello World
来源：http://vfn.xingfuxueyuan.xyz

#include <stdio.h>
来源：http://xde.jinghuilouyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lla.svipenyu.cn

[S02] C：变量与格式化输出
来源：http://jae.haohaochexian.top

int a = 10; printf("%d\n", a);
来源：http://hut.zhijiandao.cn

[S03] C：读入整数
来源：http://ipx.gzhubu.top

int x; scanf("%d", &x);
来源：http://yuw.sysykeji.top

[S04] C：字符串复制
来源：http://mvg.cdnleiting.top

char dst[32]; strcpy(dst, "hi");
来源：http://kfu.xingfuxueyuan.xyz

[S05] C：字符串长度
来源：http://dop.jinyuanbaomall.cn

strlen(s)
来源：http://ghk.smart0.xyz

[S06] C：字符串比较
来源：http://eaj.ydzc1.top

strcmp(a, b) == 0
来源：http://teg.bbcook.cn

[S07] C：数组遍历求和
来源：http://pvv.c1oappe.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vgs.vqdsnc.cn

[S08] C：动态内存分配与释放
来源：http://gav.haohaochexian.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mii.jqgfzy.top

[S09] C：结构体定义与初始化
来源：http://gum.fehbvm.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fmn.daxiang520.top

[S10] C：指针与解引用
来源：http://cfa.shangyingyoupin.top

int *p = &a;  *p = 5;
来源：http://gyf.zhaomingkeji.xyz

[S11] C：逐行读文件
来源：http://ufz.sxryk.cn

FILE *f = fopen("a.txt", "r");
来源：http://myo.xingfuxueyuan.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://dad.zhijiandao.cn

fclose(f);
来源：http://rkf.jlsjyb.cn

[S12] C：写文件
来源：http://saz.9152youxi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mkv.fanxiaobao.xyz

[S13] C：宏定义
来源：http://rds.yanxiufei.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://btj.yuanzhike.top

[S14] C：枚举
来源：http://uui.guowangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://jnb.gotoacloud.top

[S15] C：类型转换
来源：http://ryc.xingfuxueyuan.xyz

(double) a / b
来源：http://pcg.jinqigfzy.top

[S16] C：位操作置位
来源：http://kze.quarkkingdee.top

x |= (1 << 3);
来源：http://hvn.dashuyun.cn

[S17] C：安全拼接字符串
来源：http://cdp.yongpay.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wxx.guannengcc.top

[S18] C：命令行参数
来源：http://aci.sysykeji.top

int main(int argc, char **argv)
来源：http://jrg.sweek.top

[S19] C：快速排序
来源：http://rfh.shanyushiyangtech.top

qsort(a, n, sizeof(int), cmp);
来源：http://cnt.jlsjyb.cn

[S20] C：二分查找
来源：http://yhl.jqgufenzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bnm.chenzaomai.com

[S21] C：字符类别判断
来源：http://lmv.nanxinkj.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sda.tanke756.top

[S22] C：字符串转数字
来源：http://szv.yuxming.cn

atoi("42");  strtod("3.14", NULL);
来源：http://joq.zhaomingkeji.xyz

[S23] C：随机数
来源：http://guv.shangyingyoupin.top

srand(time(NULL));  int r = rand() % 100;
来源：http://iah.yj20258888.top

[S24] C：获取本地时间
来源：http://sdg.guowangkeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://opo.vqdsnc.cn

[S25] C：内存拷贝
来源：http://cfk.shangyingyoupin.top

memcpy(dst, src, n);
来源：http://sgx.cucudq.cn

[S26] C：内存清零
来源：http://vrx.guannengcc.top

memset(a, 0, sizeof a);
来源：http://dqv.ctjpmb.com

[S27] C：定义常量
来源：http://pvu.sjlbkw.cn

const double PI = 3.14159;
来源：http://qps.guowangkeji.top

[S28] C：静态变量
来源：http://pvd.nanxuanxn.top

static int counter = 0;
来源：http://otq.0kj1m.cn

[S29] C：变参函数
来源：http://pqv.zhijiandao.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kzn.daria6918.cn

[S30] C：头文件保护
来源：http://cjp.birdmap.top

#ifndef X_H
来源：http://pzt.zdbjq.cn

#define X_H
来源：http://nab.fengsongda.top

#endif
来源：http://vtk.yuanzhike.top

[S31] C++：Hello World
来源：http://mft.xuetiantiany.cn

#include <iostream>
来源：http://djy.hnqzz.top

int main() { std::cout << "Hello\n"; }
来源：http://hvn.hysaishi.cn

[S32] C++：字符串
来源：http://sgf.shzxlz.cn

std::string s = "hi";  s += "!";
来源：http://jvk.zhiwuduotai.top

[S33] C++：vector 增删
来源：http://gcz.ydzc1.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lhc.xinyue.icu

[S34] C++：遍历 vector
来源：http://ovi.ehwqpu.com

for (auto &x : v) { std::cout << x; }
来源：http://sow.wangshuangyany.cn

[S35] C++：map
来源：http://ktj.shzxlz.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qex.yueranfly.top

[S36] C++：unordered_map
来源：http://ene.vqdsnc.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ifj.ivvv.top

[S37] C++：set
来源：http://mpn.gotoacloud.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mba.meibo888.top

[S38] C++：排序
来源：http://djw.quarkkingdee.top

std::sort(v.begin(), v.end());
来源：http://jew.ctjpmb.com

[S39] C++：自定义比较器排序
来源：http://muf.hesvh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wni.guowangkeji.top

[S40] C++：查找元素
来源：http://nkv.cdnleiting.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zlt.cashguo.top

[S41] C++：类与构造函数
来源：http://mus.cucudq.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nlq.yanxiufei.cn

[S42] C++：继承与虚函数
来源：http://zkx.ivvv.top

class B : public Base { public: void f() override {} };
来源：http://kbi.shanyushiyangtech.top

[S43] C++：智能指针
来源：http://hre.nwbrower.top

auto p = std::make_unique<int>(5);
来源：http://snx.daria6918.cn

[S44] C++：引用传参
来源：http://dxi.xylfe.cn

void inc(int &x) { ++x; }
来源：http://deg.zycfv.cn

[S45] C++：lambda
来源：http://ykd.yangfankeji.com

auto add = [](int a, int b) { return a + b; };
来源：http://jmr.gaohongyu789.top

[S46] C++：函数模板
来源：http://qap.fanxiaobao.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://azj.daxiang520.top

[S47] C++：结构化绑定遍历
来源：http://ryq.cucudq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oba.pycfn.com

[S48] C++：逐行读文件
来源：http://ubz.dianchejie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lki.yj202588.top

while (std::getline(in, line)) { }
来源：http://dxk.ydzc1.top

[S49] C++：写文件
来源：http://uaq.pycfn.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qco.jiagoushi.top

[S50] C++：格式化数字
来源：http://ixl.yueranfly.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://axe.9152youxi.cn

[S51] C++：显式类型转换
来源：http://grz.yfazqb.com

static_cast<double>(a) / b
来源：http://fkc.hcnkem.com

[S52] C++：const 与 noexcept
来源：http://jqj.andypj.xyz

int size() const noexcept { return n_; }
来源：http://kwc.guannengcc.top

[S53] C++：移动语义
来源：http://sww.fzhhl.top

std::vector<int> w = std::move(v);
来源：http://lpx.gaohongyu789.top

[S54] C++：异常处理
来源：http://mer.yongpay.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nes.guannengcc.top

[S55] C++：结构化绑定
来源：http://xtd.pycfn.com

auto [a, b] = std::make_pair(1, 2);
来源：http://cnb.yuanzhike.top

[S56] C++：optional
来源：http://ikw.sysykeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iwi.shzxlz.cn

[S57] C++：编译期常量
来源：http://ako.ppjwa.cn

constexpr int N = 10;
来源：http://hlu.yj20258888.top

[S58] C++：命名空间
来源：http://flo.chenzaomai.com

namespace ns { int f() { return 1; } }
来源：http://ozb.zdbjq.cn

[S59] C++：静态断言
来源：http://xnd.hammf.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ruj.hysaishi.cn

[S60] C++：遍历并删除元素
来源：http://pvm.bbcook.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sya.hnxiangtu.top

================================================================================
来源：http://dui.dianchejie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dun.yvedp.cn

================================================================================
来源：http://rxr.ctjpmb.com

[T01] Kotlin：Hello World
来源：http://ikm.xziqi.cn

println("Hello")
来源：http://llq.sysykeji.top

[T02] Kotlin：变量
来源：http://dyl.hfpthk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bfv.dashuyun.cn

[T03] Kotlin：字符串模板
来源：http://nsh.redwolf501.top

"值: $b"
来源：http://ysy.yfazqb.com

[T04] Kotlin：空安全
来源：http://szp.havefunace.top

val n: String? = null;  n?.length
来源：http://btp.gotoacloud.top

[T05] Kotlin：when 表达式
来源：http://sle.yongpay.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://msj.daxiang520.top

[T06] Kotlin：集合映射
来源：http://cso.pycfn.com

listOf(1, 2, 3).map { it * 2 }
来源：http://drw.ywan-chungtsiang.top

[T07] Kotlin：集合过滤
来源：http://cza.epnwcf.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://vmm.bjfxy.top

[T08] Kotlin：数据类
来源：http://wkz.bjfxy.top

data class User(val name: String, val age: Int)
来源：http://xtq.zhaomingkeji.xyz

[T09] Kotlin：扩展函数
来源：http://bue.wangshuangyany.cn

fun String.exclaim() = this + "!"
来源：http://rgk.52xcode.cn

[T10] Kotlin：默认参数
来源：http://anr.jyoumei.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fww.zdqjudy.top

[T11] Kotlin：协程
来源：http://zaa.jianghu66.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://qij.wangdashe.top

[T12] Kotlin：解构声明
来源：http://cmr.cqqwz.cn

val (a, b) = Pair(1, 2)
来源：http://ayp.zdqjudy.top

[T13] Kotlin：只读 Map
来源：http://ajz.hysaishi.cn

val m = mapOf("a" to 1)
来源：http://caa.xuetiantiany.cn

[T14] Kotlin：循环
来源：http://iiw.hnxiangtu.top

for (i in 1..10) println(i)
来源：http://ucj.c1oappe.top

[T15] Kotlin：接口
来源：http://mse.gotoacloud.top

interface Shape { fun area(): Double }
来源：http://ukz.zhongyouzk.top

[T16] Swift：Hello World
来源：http://kmh.shzxlz.cn

print("Hello")
来源：http://wes.xylfe.cn

[T17] Swift：变量与常量
来源：http://ovp.hammf.cn

var a = 1;  let b = 2
来源：http://fmm.zhengqikj.top

[T18] Swift：字符串插值
来源：http://sgg.sufxvd.cn

"值: \(b)"
来源：http://iyf.gaohongyu789.top

[T19] Swift：可选绑定
来源：http://qqu.smart0.xyz

if let n = opt { print(n) }
来源：http://wye.chenjidiqi.icu

[T20] Swift：数组操作
来源：http://krt.zhixingplan.top

var a = [1, 2, 3];  a.append(4)
来源：http://yuw.sxryk.cn

[T21] Swift：遍历
来源：http://rrc.cashguo.top

for x in a { print(x) }
来源：http://yts.havefunace.top

[T22] Swift：字典
来源：http://ani.tarul.cn

var d = ["a": 1];  d["b"] = 2
来源：http://egx.fanxiaobao.xyz

[T23] Swift：函数
来源：http://gkc.gaohongyu789.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nfw.uphjek.com

[T24] Swift：闭包
来源：http://tqu.bbcook.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xgx.fanxiaobao.xyz

[T25] Swift：结构体
来源：http://wbs.ydzc1.top

struct P { var x: Int }
来源：http://gpg.ppjwa.cn

[T26] Swift：类与重写
来源：http://lni.xziqi.cn

class A: Base { override func f() {} }
来源：http://chc.guannengcc.top

[T27] Swift：错误处理
来源：http://kes.hnqzz.top

do { try f() } catch { print(error) }
来源：http://znt.sweek.top

[T28] Swift：枚举
来源：http://orx.wangshuangyany.cn

enum Color { case red, green }
来源：http://nfk.hongshengwenyu.top

[T29] Swift：guard 提前返回
来源：http://kre.zhengqikj.top

guard let x = opt else { return }
来源：http://ece.hesvh.cn

[T30] Swift：协议
来源：http://lhh.jqgufenzy.top

protocol Shape { func area() -> Double }
来源：http://vbq.hywenlv.cn

[T31] Lua：Hello World
来源：http://boq.yueranfly.top

print("Hello")
来源：http://pzx.tanke756.top

[T32] Lua：局部变量
来源：http://vuu.fzhhl.top

local a = 1
来源：http://ndt.sjlbkw.cn

[T33] Lua：表（数组）
来源：http://hxc.aizwys.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bsd.sjlbkw.cn

[T34] Lua：遍历表
来源：http://zfb.vqdsnc.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xlg.jqgfzy.top

[T35] Lua：字典表
来源：http://mzw.bjfxy.top

local d = { a = 1 };  d.b = 2
来源：http://ioe.shangyingyoupin.top

[T36] Lua：函数
来源：http://npt.chenlongwang.top

function add(a, b) return a + b end
来源：http://jzd.hywenlv.cn

[T37] Lua：字符串拼接
来源：http://tbe.yuxming.cn

"a" .. "b"
来源：http://cvg.vqdsnc.cn

[T38] Lua：条件
来源：http://twb.fengsongda.top

if x > 0 then print("正") end
来源：http://fam.snrcjt.cn

[T39] Lua：模式匹配
来源：http://cio.fktsv.cn

string.find(s, "%d+")
来源：http://iyl.ivvv.top

[T40] Lua：元表
来源：http://ijo.0kj1m.cn

setmetatable({}, { __index = base })
来源：http://hix.ivvv.top

[T41] Perl：Hello World
来源：http://sfp.ywan-chungtsiang.top

print "Hello\n";
来源：http://ija.bbcook.cn

[T42] Perl：变量类型
来源：http://hrd.cdnleiting.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vuy.snrcjt.cn

[T43] Perl：字符串插值
来源：http://hhw.yuanzhike.top

"值: $a"
来源：http://cko.shanyushiyangtech.top

[T44] Perl：条件
来源：http://dvl.tianlin.xyz

if ($a > 0) { print "正"; }
来源：http://hpa.fanxiaobao.xyz

[T45] Perl：数组遍历
来源：http://kbj.jinghuilouyu.cn

for my $x (@arr) { print $x; }
来源：http://gzi.epnwcf.com

[T46] Perl：哈希操作
来源：http://hhj.kuanghao11.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://flr.jinyuanbaomall.cn

[T47] Perl：正则捕获
来源：http://iyr.pycfn.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://vxq.iojbl.cn

[T48] Perl：正则替换
来源：http://ivx.316326.xyz

$s =~ s/old/new/g;
来源：http://stz.jiagoushi.top

[T49] Perl：函数
来源：http://jsz.hesvh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qrx.sxryk.cn

[T50] Perl：逐行读文件
来源：http://vhv.dianchejie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://umc.sxryk.cn

while (my $line = <$fh>) { print $line; }
来源：http://hga.ywan-chungtsiang.top

[T51] Scala：Hello World
来源：http://cpy.yuxming.cn

println("Hello")
来源：http://drs.meibo888.top

[T52] Scala：变量
来源：http://yrl.fktsv.cn

val a = 1;  var b = 2
来源：http://zeh.chenjidiqi.icu

[T53] Scala：字符串插值
来源：http://qmh.xylfe.cn

s"值: $b"
来源：http://qbq.wangdashe.top

[T54] Scala：集合映射
来源：http://pju.zycfv.cn

List(1, 2, 3).map(_ * 2)
来源：http://vrm.hfpthk.cn

[T55] Scala：集合过滤
来源：http://tqz.gaohongyu789.top

List(1, 2, 3).filter(_ > 1)
来源：http://xrz.sysykeji.top

[T56] Scala：样例类
来源：http://goe.xziqi.cn

case class User(name: String, age: Int)
来源：http://eyg.fanxiaobao.xyz

[T57] Scala：模式匹配
来源：http://wpf.shuidangran.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://bhz.hongshengwenyu.top

[T58] Scala：函数定义
来源：http://wnp.hcnkem.com

def add(a: Int, b: Int): Int = a + b
来源：http://nnb.ctjpmb.com

[T59] Scala：循环
来源：http://wnu.nanxinkj.top

for (i <- 1 to 10) println(i)
来源：http://puk.jqgfzy.top

[T60] Scala：折叠
来源：http://iqe.fehbvm.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ovj.bjfxy.top

================================================================================
来源：http://kqq.hesvh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fvc.cashguo.top

================================================================================
来源：http://cwr.nanxuanxn.top

[U01] Py：创建虚拟环境
来源：http://jbm.wangshuangyany.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vaj.yfazqb.com

[U02] Py：导出 / 安装依赖
来源：http://skg.hesvh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qdo.fzhhl.top

[U03] Py：加载 .env 配置
来源：http://fje.xylfe.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://igo.bbcook.cn

[U04] Py：变量调试打印
来源：http://dsi.zycfv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eap.hnqzz.top

[U05] Py：列表去重且保序
来源：http://ese.svipenyu.cn

list(dict.fromkeys(arr))
来源：http://gcr.ydzc1.top

[U06] Py：合并两个字典
来源：http://bpe.52xcode.cn

{**a, **b}
来源：http://tld.guowangkeji.top

[U07] Py：反转字典键值
来源：http://eqa.yj202588.top

{v: k for k, v in d.items()}
来源：http://wpc.snrcjt.cn

[U08] Py：展平二维列表
来源：http://fqr.andypj.xyz

[y for x in nested for y in x]
来源：http://qwg.ctjpmb.com

[U09] Py：字典取最大值的键
来源：http://ncb.ybcxt.top

max(d, key=d.get)
来源：http://sli.0kj1m.cn

[U10] Py：按值排序字典
来源：http://kem.shanyushiyangtech.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xfe.mhx1999.top

[U11] Py：生成器表达式
来源：http://ghk.fzhhl.top

(x * 2 for x in arr)
来源：http://kqk.dianchejie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://nyt.quarkkingdee.top

Counter(arr).most_common(3)
来源：http://zli.sjlbkw.cn

[U13] Py：固定长度队列
来源：http://ckb.316326.xyz

deque(maxlen=10)
来源：http://lru.fehbvm.com

[U14] Py：分组收集到列表
来源：http://yvb.jyoumei.cn

defaultdict(list)
来源：http://kvb.andypj.xyz


<!-- 参考信息 -->