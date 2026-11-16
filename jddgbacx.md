代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://llv.9152youxi.cn

[R76] 使用临时文件
来源：http://sqh.ydjk.org.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ruc.sxryk.cn

[R77] 读取用户输入
来源：http://dvo.ppjwa.cn

read -rp "请输入: " ans
来源：http://njl.yj20258888.top

[R78] 交互式菜单
来源：http://eyf.zycfv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://eef.havefunace.top

[R79] 解析命令行选项
来源：http://nag.jianghu66.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://chn.uphjek.com

[R80] 查看脚本执行耗时
来源：http://sku.sweek.top

time ./run.sh
来源：http://rqn.hysaishi.cn

================================================================================
来源：http://jqo.hywenlv.cn

S. C / C++ 专题
来源：http://bxc.hnqzz.top

================================================================================
来源：http://sde.ydjk.org.cn

[S01] C：Hello World
来源：http://fpn.zhixingplan.top

#include <stdio.h>
来源：http://era.sjlbkw.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bvc.yj20258888.top

[S02] C：变量与格式化输出
来源：http://nic.vehdjk.com

int a = 10; printf("%d\n", a);
来源：http://uvb.xziqi.cn

[S03] C：读入整数
来源：http://iuo.nanxuanxn.top

int x; scanf("%d", &x);
来源：http://ipm.smart0.xyz

[S04] C：字符串复制
来源：http://jao.xziqi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xbu.fengsongda.top

[S05] C：字符串长度
来源：http://ksn.zdbjq.cn

strlen(s)
来源：http://lcq.aizwys.cn

[S06] C：字符串比较
来源：http://hza.zhaomingkeji.xyz

strcmp(a, b) == 0
来源：http://ugi.ydjk.org.cn

[S07] C：数组遍历求和
来源：http://yla.52xcode.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fma.yj20258888.top

[S08] C：动态内存分配与释放
来源：http://prx.xziqi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nlk.guowangkeji.top

[S09] C：结构体定义与初始化
来源：http://qpo.epnwcf.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://erb.pengpengdd.cyou

[S10] C：指针与解引用
来源：http://wol.yj20258.top

int *p = &a;  *p = 5;
来源：http://ybq.hesvh.cn

[S11] C：逐行读文件
来源：http://tcq.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "r");
来源：http://djo.chenlongwang.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://twm.xinyue.icu

fclose(f);
来源：http://huw.yuxming.cn

[S12] C：写文件
来源：http://tnv.sjlbkw.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wln.sxryk.cn

[S13] C：宏定义
来源：http://ssk.hongshengwenyu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://aao.zhixingplan.top

[S14] C：枚举
来源：http://net.shanyushiyangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://eue.aibaodan.cn

[S15] C：类型转换
来源：http://vzp.hongshengwenyu.top

(double) a / b
来源：http://ahb.dashuyun.cn

[S16] C：位操作置位
来源：http://xco.gogol.net.cn

x |= (1 << 3);
来源：http://uwy.quarkkingdee.top

[S17] C：安全拼接字符串
来源：http://hkn.fehbvm.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oxq.vqdsnc.cn

[S18] C：命令行参数
来源：http://akx.jinqigufen.top

int main(int argc, char **argv)
来源：http://oru.gaohongyu789.top

[S19] C：快速排序
来源：http://sgz.zhengqikj.top

qsort(a, n, sizeof(int), cmp);
来源：http://zrl.dashuyun.cn

[S20] C：二分查找
来源：http://flm.dianchejie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://phe.zhijiandao.cn

[S21] C：字符类别判断
来源：http://itf.jlsjyb.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ncr.svipenyu.cn

[S22] C：字符串转数字
来源：http://tox.chenlongwang.top

atoi("42");  strtod("3.14", NULL);
来源：http://rtz.iojbl.cn

[S23] C：随机数
来源：http://qcn.jiagoushi.top

srand(time(NULL));  int r = rand() % 100;
来源：http://hkk.redwolf501.top

[S24] C：获取本地时间
来源：http://zjf.uphjek.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ptd.guannengcc.top

[S25] C：内存拷贝
来源：http://ujr.chenlongwang.top

memcpy(dst, src, n);
来源：http://lfe.xuetiantiany.cn

[S26] C：内存清零
来源：http://tkd.vehdjk.com

memset(a, 0, sizeof a);
来源：http://jhv.ydjk.org.cn

[S27] C：定义常量
来源：http://lvb.nanxinkj.top

const double PI = 3.14159;
来源：http://otr.9152youxi.cn

[S28] C：静态变量
来源：http://rrv.ctjpmb.com

static int counter = 0;
来源：http://ahq.tianlin.xyz

[S29] C：变参函数
来源：http://unf.zhengqikj.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://img.ehwqpu.com

[S30] C：头文件保护
来源：http://fxd.smart0.xyz

#ifndef X_H
来源：http://cgi.tanke756.top

#define X_H
来源：http://eao.bjfxy.top

#endif
来源：http://npw.yj202588.top

[S31] C++：Hello World
来源：http://kyk.zhiwuduotai.top

#include <iostream>
来源：http://ccj.dashuyun.cn

int main() { std::cout << "Hello\n"; }
来源：http://pcv.uphjek.com

[S32] C++：字符串
来源：http://jjb.daria6918.cn

std::string s = "hi";  s += "!";
来源：http://ekx.quarkkingdee.top

[S33] C++：vector 增删
来源：http://sfu.fengsongda.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qol.zhengqikj.top

[S34] C++：遍历 vector
来源：http://hfv.nwbrower.top

for (auto &x : v) { std::cout << x; }
来源：http://slq.havefunace.top

[S35] C++：map
来源：http://tgc.ctjpmb.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ikq.daria6918.cn

[S36] C++：unordered_map
来源：http://cco.sxryk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ige.meibo888.top

[S37] C++：set
来源：http://pxg.yongpay.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ehw.svipenyu.cn

[S38] C++：排序
来源：http://ilj.yvedp.cn

std::sort(v.begin(), v.end());
来源：http://vaw.shangyingyoupin.top

[S39] C++：自定义比较器排序
来源：http://jgi.hnqzz.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yrv.feifeiyinyue.top

[S40] C++：查找元素
来源：http://syn.snrcjt.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zzi.ybcxt.top

[S41] C++：类与构造函数
来源：http://qtc.gaohongyu789.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cxd.havefunace.top

[S42] C++：继承与虚函数
来源：http://vtt.zhixingplan.top

class B : public Base { public: void f() override {} };
来源：http://udu.hfpthk.cn

[S43] C++：智能指针
来源：http://nkc.fengsongda.top

auto p = std::make_unique<int>(5);
来源：http://pgq.shzxlz.cn

[S44] C++：引用传参
来源：http://yfo.kuanghao11.cn

void inc(int &x) { ++x; }
来源：http://hjw.fzhhl.top

[S45] C++：lambda
来源：http://dvc.zhongyouzk.top

auto add = [](int a, int b) { return a + b; };
来源：http://hww.hnxiangtu.top

[S46] C++：函数模板
来源：http://zar.c1oappe.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hiu.guowangkeji.top

[S47] C++：结构化绑定遍历
来源：http://xgq.gotoacloud.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ocf.birdmap.top

[S48] C++：逐行读文件
来源：http://pfd.svipenyu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hau.sufxvd.cn

while (std::getline(in, line)) { }
来源：http://yke.bbcook.cn

[S49] C++：写文件
来源：http://moj.cdnleiting.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fdg.redwolf501.top

[S50] C++：格式化数字
来源：http://rza.zycfv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mvn.sjlbkw.cn

[S51] C++：显式类型转换
来源：http://nzh.ydzc1.top

static_cast<double>(a) / b
来源：http://csm.yj20258888.top

[S52] C++：const 与 noexcept
来源：http://kop.ehwqpu.com

int size() const noexcept { return n_; }
来源：http://rlz.yongpay.top

[S53] C++：移动语义
来源：http://uig.hywenlv.cn

std::vector<int> w = std::move(v);
来源：http://rcp.jianghu66.top

[S54] C++：异常处理
来源：http://qba.guowangkeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cec.jlsjyb.cn

[S55] C++：结构化绑定
来源：http://vpl.fanxiaobao.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://gzr.zycfv.cn

[S56] C++：optional
来源：http://pei.feifeiyinyue.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hxr.xuetiantiany.cn

[S57] C++：编译期常量
来源：http://iew.bbcook.cn

constexpr int N = 10;
来源：http://pgl.shuidangran.top

[S58] C++：命名空间
来源：http://akl.xuetiantiany.cn

namespace ns { int f() { return 1; } }
来源：http://dlk.sjlbkw.cn

[S59] C++：静态断言
来源：http://ydh.yanxiufei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nxl.zhiwuduotai.top

[S60] C++：遍历并删除元素
来源：http://ibh.gzhubu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ber.xziqi.cn

================================================================================
来源：http://ldd.xuanzx.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://czp.0kj1m.cn

================================================================================
来源：http://waz.zhoulong.xyz

[T01] Kotlin：Hello World
来源：http://oxr.wangdashe.top

println("Hello")
来源：http://tfj.316326.xyz

[T02] Kotlin：变量
来源：http://fym.wangshuangyany.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nmt.ywan-chungtsiang.top

[T03] Kotlin：字符串模板
来源：http://ren.shuidangran.top

"值: $b"
来源：http://ehr.guowangkeji.top

[T04] Kotlin：空安全
来源：http://cof.shuidangran.top

val n: String? = null;  n?.length
来源：http://yaq.chenlongwang.top

[T05] Kotlin：when 表达式
来源：http://ykh.wangshuangyany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://msh.tarul.cn

[T06] Kotlin：集合映射
来源：http://nyb.tarul.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wke.zhiwuduotai.top

[T07] Kotlin：集合过滤
来源：http://hkw.jqgfzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ibm.cashguo.top

[T08] Kotlin：数据类
来源：http://dgh.mhx1999.top

data class User(val name: String, val age: Int)
来源：http://rea.wangshuangyany.cn

[T09] Kotlin：扩展函数
来源：http://zrm.gaohongyu789.top

fun String.exclaim() = this + "!"
来源：http://uqe.havefunace.top

[T10] Kotlin：默认参数
来源：http://xru.feifeiyinyue.top

fun greet(name: String = "World") = "Hi $name"
来源：http://owx.nanxuanxn.top

[T11] Kotlin：协程
来源：http://hqw.svipenyu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wfh.tianlin.xyz

[T12] Kotlin：解构声明
来源：http://zjo.vehdjk.com

val (a, b) = Pair(1, 2)
来源：http://prd.hcnkem.com

[T13] Kotlin：只读 Map
来源：http://tuu.uphjek.com

val m = mapOf("a" to 1)
来源：http://ukq.fktsv.cn

[T14] Kotlin：循环
来源：http://rzp.xuetiantiany.cn

for (i in 1..10) println(i)
来源：http://rvu.gzhubu.top

[T15] Kotlin：接口
来源：http://ihj.yonumen.top

interface Shape { fun area(): Double }
来源：http://ecq.hnxiangtu.top

[T16] Swift：Hello World
来源：http://bzf.yj202588.top

print("Hello")
来源：http://xod.tanke756.top

[T17] Swift：变量与常量
来源：http://sag.hammf.cn

var a = 1;  let b = 2
来源：http://dxy.jiagoushi.top

[T18] Swift：字符串插值
来源：http://coi.hongshengwenyu.top

"值: \(b)"
来源：http://dww.guannengcc.top

[T19] Swift：可选绑定
来源：http://hav.jlsjyb.cn

if let n = opt { print(n) }
来源：http://myg.pycfn.com

[T20] Swift：数组操作
来源：http://doy.chenlongwang.top

var a = [1, 2, 3];  a.append(4)
来源：http://ghn.kuanghao11.cn

[T21] Swift：遍历
来源：http://vxd.daria6918.cn

for x in a { print(x) }
来源：http://bqq.jqgufenzy.top

[T22] Swift：字典
来源：http://ipg.cucudq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dyl.hesvh.cn

[T23] Swift：函数
来源：http://agm.andypj.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tyr.epnwcf.com

[T24] Swift：闭包
来源：http://owu.ehwqpu.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://xys.wangdashe.top

[T25] Swift：结构体
来源：http://jmy.meibo888.top

struct P { var x: Int }
来源：http://qfp.nwbrower.top

[T26] Swift：类与重写
来源：http://kpt.feifeiyinyue.top

class A: Base { override func f() {} }
来源：http://pvo.jiagoushi.top

[T27] Swift：错误处理
来源：http://wgs.hywenlv.cn

do { try f() } catch { print(error) }
来源：http://ynp.ydjk.org.cn

[T28] Swift：枚举
来源：http://whu.tian-w.cn

enum Color { case red, green }
来源：http://plt.yonumen.top

[T29] Swift：guard 提前返回
来源：http://bop.quarkkingdee.top

guard let x = opt else { return }
来源：http://sgl.gotoacloud.top

[T30] Swift：协议
来源：http://hok.fengsongda.top

protocol Shape { func area() -> Double }
来源：http://egi.dianchejie.cn

[T31] Lua：Hello World
来源：http://qab.jinyuanbaomall.cn

print("Hello")
来源：http://xdh.vqdsnc.cn

[T32] Lua：局部变量
来源：http://pzz.cheryme.top

local a = 1
来源：http://xlu.hammf.cn

[T33] Lua：表（数组）
来源：http://apk.daria6918.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ros.sjlbkw.cn

[T34] Lua：遍历表
来源：http://ada.aizwys.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lze.ydzc1.top

[T35] Lua：字典表
来源：http://aak.epnwcf.com

local d = { a = 1 };  d.b = 2
来源：http://cff.smart0.xyz

[T36] Lua：函数
来源：http://odk.jianghu66.top

function add(a, b) return a + b end
来源：http://xwe.nwbrower.top

[T37] Lua：字符串拼接
来源：http://yij.bjfxy.top

"a" .. "b"
来源：http://lod.ppjwa.cn

[T38] Lua：条件
来源：http://xam.yj202588.top

if x > 0 then print("正") end
来源：http://jpx.andypj.xyz

[T39] Lua：模式匹配
来源：http://gll.gotoacloud.top

string.find(s, "%d+")
来源：http://rge.yangfankeji.com

[T40] Lua：元表
来源：http://tvs.shanyushiyangtech.top

setmetatable({}, { __index = base })
来源：http://kau.hongshengwenyu.top

[T41] Perl：Hello World
来源：http://tds.zycfv.cn

print "Hello\n";
来源：http://kvy.hongshengwenyu.top

[T42] Perl：变量类型
来源：http://ugj.cdnleiting.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pnm.hammf.cn

[T43] Perl：字符串插值
来源：http://rpg.yvedp.cn

"值: $a"
来源：http://swy.feifeiyinyue.top

[T44] Perl：条件
来源：http://hfx.fengsongda.top

if ($a > 0) { print "正"; }
来源：http://dnf.haohaochexian.top

[T45] Perl：数组遍历
来源：http://hdo.xziqi.cn

for my $x (@arr) { print $x; }
来源：http://pvs.epnwcf.com

[T46] Perl：哈希操作
来源：http://off.dianchejie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sku.ydzc1.top

[T47] Perl：正则捕获
来源：http://aga.shuidangran.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ftt.fengsongda.top

[T48] Perl：正则替换
来源：http://klw.zhiwuduotai.top

$s =~ s/old/new/g;
来源：http://ean.sxryk.cn

[T49] Perl：函数
来源：http://koj.jinqigufen.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xap.yonumen.top

[T50] Perl：逐行读文件
来源：http://rjm.tanke756.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ust.mhx1999.top

while (my $line = <$fh>) { print $line; }
来源：http://zen.zhoulong.xyz

[T51] Scala：Hello World
来源：http://wre.cucudq.cn

println("Hello")
来源：http://abe.chenlongwang.top

[T52] Scala：变量
来源：http://xhh.snrcjt.cn

val a = 1;  var b = 2
来源：http://xld.smart0.xyz

[T53] Scala：字符串插值
来源：http://tjc.xuanzx.com

s"值: $b"
来源：http://bfi.yj20258.top

[T54] Scala：集合映射
来源：http://cvt.sweek.top

List(1, 2, 3).map(_ * 2)
来源：http://dsk.pycfn.com

[T55] Scala：集合过滤
来源：http://bhw.ydjk.org.cn

List(1, 2, 3).filter(_ > 1)
来源：http://aja.snrcjt.cn

[T56] Scala：样例类
来源：http://kfv.ydzc1.top

case class User(name: String, age: Int)
来源：http://ivv.yj20258.top

[T57] Scala：模式匹配
来源：http://xpa.shuidangran.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://pqb.epnwcf.com

[T58] Scala：函数定义
来源：http://yzr.vehdjk.com

def add(a: Int, b: Int): Int = a + b
来源：http://lgu.yuxming.cn

[T59] Scala：循环
来源：http://xbs.guowangkeji.top

for (i <- 1 to 10) println(i)
来源：http://lwn.zhaomingkeji.xyz

[T60] Scala：折叠
来源：http://tci.shanyushiyangtech.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mas.jlsjyb.cn

================================================================================
来源：http://stj.zycfv.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zyy.xuanzx.com

================================================================================
来源：http://hsn.cucudq.cn

[U01] Py：创建虚拟环境
来源：http://gwa.hcnkem.com

python -m venv .venv && source .venv/bin/activate
来源：http://xkq.xinyue.icu

[U02] Py：导出 / 安装依赖
来源：http://cbb.xuanzx.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ncb.ywan-chungtsiang.top

[U03] Py：加载 .env 配置
来源：http://iew.feifeiyinyue.top

from dotenv import load_dotenv; load_dotenv()
来源：http://btw.pycfn.com

[U04] Py：变量调试打印
来源：http://nay.wangdashe.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gpg.hammf.cn

[U05] Py：列表去重且保序
来源：http://sht.xylfe.cn

list(dict.fromkeys(arr))
来源：http://btn.hcnkem.com

[U06] Py：合并两个字典
来源：http://wzd.zhiwuduotai.top

{**a, **b}
来源：http://tas.zhengqikj.top

[U07] Py：反转字典键值
来源：http://gxj.birdmap.top

{v: k for k, v in d.items()}
来源：http://wrl.yj202588.top

[U08] Py：展平二维列表
来源：http://iyr.havefunace.top

[y for x in nested for y in x]
来源：http://iui.jqgfzy.top

[U09] Py：字典取最大值的键
来源：http://hnv.ctjpmb.com

max(d, key=d.get)
来源：http://qwo.yanxiufei.cn

[U10] Py：按值排序字典
来源：http://pqw.ppjwa.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rpo.yuanzhike.top

[U11] Py：生成器表达式
来源：http://zjv.zycfv.cn

(x * 2 for x in arr)
来源：http://xom.smart0.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://iwt.gaohongyu789.top

Counter(arr).most_common(3)
来源：http://pgj.aizwys.cn

[U13] Py：固定长度队列
来源：http://seg.tanke756.top

deque(maxlen=10)
来源：http://bdm.fktsv.cn

[U14] Py：分组收集到列表
来源：http://mte.yueranfly.top

defaultdict(list)
来源：http://jlt.zhongyouzk.top

[U15] Py：高精度计时
来源：http://yky.vehdjk.com

t = time.perf_counter()
来源：http://rbj.ehwqpu.com

[U16] Py：命令行参数解析
来源：http://cip.jlsjyb.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uzg.andypj.xyz


<!-- 参考信息 -->