代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://mjr.hcnkem.com

[R72] 等待端口就绪
来源：http://oim.sjlbkw.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nyh.pengpengdd.cyou

[R73] 分割大日志
来源：http://axw.feifeiyinyue.top

split -l 1000 big.log part_
来源：http://ygh.xinyue.icu

[R74] 批量重命名
来源：http://yyu.shzxlz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qbt.cdnleiting.top

[R75] 导出环境变量
来源：http://fmb.tarul.cn

export PATH="$HOME/bin:$PATH"
来源：http://jjl.jqgfzy.top

[R76] 使用临时文件
来源：http://zbi.tanke756.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vah.xinyue.icu

[R77] 读取用户输入
来源：http://kws.0kj1m.cn

read -rp "请输入: " ans
来源：http://ayj.zhoulong.xyz

[R78] 交互式菜单
来源：http://ykv.jianghu66.top

select opt in a b c; do echo "$opt"; break; done
来源：http://fbp.tanke756.top

[R79] 解析命令行选项
来源：http://lkg.daxiang520.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uyj.feifeiyinyue.top

[R80] 查看脚本执行耗时
来源：http://iil.xinyue.icu

time ./run.sh
来源：http://rmn.xylfe.cn

================================================================================
来源：http://qzp.wangdashe.top

S. C / C++ 专题
来源：http://ria.hesvh.cn

================================================================================
来源：http://wlu.gogol.net.cn

[S01] C：Hello World
来源：http://sft.andypj.xyz

#include <stdio.h>
来源：http://edd.tianlin.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://mpy.guannengcc.top

[S02] C：变量与格式化输出
来源：http://rsx.hfpthk.cn

int a = 10; printf("%d\n", a);
来源：http://pzh.chenjidiqi.icu

[S03] C：读入整数
来源：http://wkl.shanyushiyangtech.top

int x; scanf("%d", &x);
来源：http://ylg.yangfankeji.com

[S04] C：字符串复制
来源：http://pmo.aizwys.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gpn.chenjidiqi.icu

[S05] C：字符串长度
来源：http://mob.sxryk.cn

strlen(s)
来源：http://nqy.guannengcc.top

[S06] C：字符串比较
来源：http://uad.chenjidiqi.icu

strcmp(a, b) == 0
来源：http://aoz.shzxlz.cn

[S07] C：数组遍历求和
来源：http://igf.wangdashe.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lva.pycfn.com

[S08] C：动态内存分配与释放
来源：http://ukw.hnqzz.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ivf.nwbrower.top

[S09] C：结构体定义与初始化
来源：http://vmw.ivvv.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cnu.zhongyouzk.top

[S10] C：指针与解引用
来源：http://fno.epnwcf.com

int *p = &a;  *p = 5;
来源：http://lpk.andypj.xyz

[S11] C：逐行读文件
来源：http://fml.yuanzhike.top

FILE *f = fopen("a.txt", "r");
来源：http://bil.yongpay.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://oxr.sysykeji.top

fclose(f);
来源：http://pgt.zdbjq.cn

[S12] C：写文件
来源：http://uiw.zdqjudy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bbz.fanxiaobao.xyz

[S13] C：宏定义
来源：http://fws.gzhubu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ksj.yonumen.top

[S14] C：枚举
来源：http://rsd.yueranfly.top

enum Color { RED, GREEN, BLUE };
来源：http://ias.sweek.top

[S15] C：类型转换
来源：http://mkx.guowangkeji.top

(double) a / b
来源：http://rik.chenzaomai.com

[S16] C：位操作置位
来源：http://qfv.yueranfly.top

x |= (1 << 3);
来源：http://jmb.xinyue.icu

[S17] C：安全拼接字符串
来源：http://bus.yj20258888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ozt.pengpengdd.cyou

[S18] C：命令行参数
来源：http://udu.redwolf501.top

int main(int argc, char **argv)
来源：http://sfz.ywan-chungtsiang.top

[S19] C：快速排序
来源：http://vqv.hysaishi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lzn.yfazqb.com

[S20] C：二分查找
来源：http://pxn.aibaodan.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sdd.hnxiangtu.top

[S21] C：字符类别判断
来源：http://xvr.ehwqpu.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xvy.tanke756.top

[S22] C：字符串转数字
来源：http://fpi.zhixingplan.top

atoi("42");  strtod("3.14", NULL);
来源：http://yxt.nanxinkj.top

[S23] C：随机数
来源：http://cvn.jyoumei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fpb.gogol.net.cn

[S24] C：获取本地时间
来源：http://hch.hnqzz.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kuh.ywan-chungtsiang.top

[S25] C：内存拷贝
来源：http://nnw.fehbvm.com

memcpy(dst, src, n);
来源：http://etm.epnwcf.com

[S26] C：内存清零
来源：http://uja.yj20258.top

memset(a, 0, sizeof a);
来源：http://pwv.daxiang520.top

[S27] C：定义常量
来源：http://vcm.aibaodan.cn

const double PI = 3.14159;
来源：http://rlm.zhoulong.xyz

[S28] C：静态变量
来源：http://lpa.zdqjudy.top

static int counter = 0;
来源：http://sqh.zdbjq.cn

[S29] C：变参函数
来源：http://esh.ydzc1.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dnb.yongpay.top

[S30] C：头文件保护
来源：http://rhi.xylfe.cn

#ifndef X_H
来源：http://mca.xylfe.cn

#define X_H
来源：http://ddr.gzhubu.top

#endif
来源：http://dcl.jianghu66.top

[S31] C++：Hello World
来源：http://ctf.smart0.xyz

#include <iostream>
来源：http://zhm.9152youxi.cn

int main() { std::cout << "Hello\n"; }
来源：http://cjy.shanyushiyangkeji.top

[S32] C++：字符串
来源：http://era.zhixingplan.top

std::string s = "hi";  s += "!";
来源：http://xsj.jinqigfzy.top

[S33] C++：vector 增删
来源：http://tuk.zhixingplan.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://iwt.ydjk.org.cn

[S34] C++：遍历 vector
来源：http://aoq.xylfe.cn

for (auto &x : v) { std::cout << x; }
来源：http://woa.wangshuangyany.cn

[S35] C++：map
来源：http://lxz.haohaochexian.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ohs.daxiang520.top

[S36] C++：unordered_map
来源：http://ulx.gotoacloud.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iuy.tianlin.xyz

[S37] C++：set
来源：http://xdf.316326.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tbc.ppjwa.cn

[S38] C++：排序
来源：http://epa.yuxming.cn

std::sort(v.begin(), v.end());
来源：http://qbc.ydjk.org.cn

[S39] C++：自定义比较器排序
来源：http://uad.xziqi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://diq.nanxuanxn.top

[S40] C++：查找元素
来源：http://cdk.zhaomingkeji.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vcg.tarul.cn

[S41] C++：类与构造函数
来源：http://uyx.dianchejie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nlu.feifeiyinyue.top

[S42] C++：继承与虚函数
来源：http://ydx.shangyingyoupin.top

class B : public Base { public: void f() override {} };
来源：http://jcb.jqgufenzy.top

[S43] C++：智能指针
来源：http://vgb.zhijiandao.cn

auto p = std::make_unique<int>(5);
来源：http://lml.c1oappe.top

[S44] C++：引用传参
来源：http://vzu.daria6918.cn

void inc(int &x) { ++x; }
来源：http://szf.redwolf501.top

[S45] C++：lambda
来源：http://sng.jianghu66.top

auto add = [](int a, int b) { return a + b; };
来源：http://bfo.zhijiandao.cn

[S46] C++：函数模板
来源：http://hdk.nanxuanxn.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hmo.iojbl.cn

[S47] C++：结构化绑定遍历
来源：http://zpn.c1oappe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jjy.hfpthk.cn

[S48] C++：逐行读文件
来源：http://ewp.9152youxi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://swv.fzhhl.top

while (std::getline(in, line)) { }
来源：http://lan.jqgfzy.top

[S49] C++：写文件
来源：http://ipx.ydzc1.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://drc.cdnleiting.top

[S50] C++：格式化数字
来源：http://xwo.aibaodan.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eab.hongshengwenyu.top

[S51] C++：显式类型转换
来源：http://mnk.zhiwuduotai.top

static_cast<double>(a) / b
来源：http://mvd.feifeiyinyue.top

[S52] C++：const 与 noexcept
来源：http://ncd.quarkkingdee.top

int size() const noexcept { return n_; }
来源：http://rpu.ywan-chungtsiang.top

[S53] C++：移动语义
来源：http://gio.zhaomingkeji.xyz

std::vector<int> w = std::move(v);
来源：http://tqm.52xcode.cn

[S54] C++：异常处理
来源：http://fgh.sysykeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yzr.zhijiandao.cn

[S55] C++：结构化绑定
来源：http://mbr.gzhubu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://aym.fktsv.cn

[S56] C++：optional
来源：http://fsj.zdbjq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bmt.hammf.cn

[S57] C++：编译期常量
来源：http://jec.guannengcc.top

constexpr int N = 10;
来源：http://lef.zdqjudy.top

[S58] C++：命名空间
来源：http://ugz.yj202588.top

namespace ns { int f() { return 1; } }
来源：http://nfq.zhengqikj.top

[S59] C++：静态断言
来源：http://byh.zhiwuduotai.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wtq.yfazqb.com

[S60] C++：遍历并删除元素
来源：http://tec.zhengqikj.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cqs.gotoacloud.top

================================================================================
来源：http://tab.nwbrower.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mar.hysaishi.cn

================================================================================
来源：http://kcy.tanke756.top

[T01] Kotlin：Hello World
来源：http://zqe.mhx1999.top

println("Hello")
来源：http://bzg.sxryk.cn

[T02] Kotlin：变量
来源：http://awx.sufxvd.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://brw.wangdashe.top

[T03] Kotlin：字符串模板
来源：http://uhl.zhoulong.xyz

"值: $b"
来源：http://uwb.vqdsnc.cn

[T04] Kotlin：空安全
来源：http://mfl.ctjpmb.com

val n: String? = null;  n?.length
来源：http://vhv.jqgufenzy.top

[T05] Kotlin：when 表达式
来源：http://wwp.jqgufenzy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sqp.shangyingyoupin.top

[T06] Kotlin：集合映射
来源：http://feg.jqgufenzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://fys.hesvh.cn

[T07] Kotlin：集合过滤
来源：http://srz.yanxiufei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fmx.jqgfzy.top

[T08] Kotlin：数据类
来源：http://qmn.tian-w.cn

data class User(val name: String, val age: Int)
来源：http://yrm.zycfv.cn

[T09] Kotlin：扩展函数
来源：http://sbe.yj202588.top

fun String.exclaim() = this + "!"
来源：http://taq.aibaodan.cn

[T10] Kotlin：默认参数
来源：http://cgz.gogol.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://itx.yfazqb.com

[T11] Kotlin：协程
来源：http://yba.jqgfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://uwy.yangfankeji.com

[T12] Kotlin：解构声明
来源：http://ngm.jinqigufen.top

val (a, b) = Pair(1, 2)
来源：http://gzy.gogol.net.cn

[T13] Kotlin：只读 Map
来源：http://gel.fengsongda.top

val m = mapOf("a" to 1)
来源：http://tpy.cqqwz.cn

[T14] Kotlin：循环
来源：http://xyt.hongshengwenyu.top

for (i in 1..10) println(i)
来源：http://phr.snrcjt.cn

[T15] Kotlin：接口
来源：http://zes.xziqi.cn

interface Shape { fun area(): Double }
来源：http://inf.cucudq.cn

[T16] Swift：Hello World
来源：http://dyi.zdqjudy.top

print("Hello")
来源：http://uaa.bjfxy.top

[T17] Swift：变量与常量
来源：http://nnq.fanxiaobao.xyz

var a = 1;  let b = 2
来源：http://hek.mhx1999.top

[T18] Swift：字符串插值
来源：http://mux.yj202588.top

"值: \(b)"
来源：http://eeu.vehdjk.com

[T19] Swift：可选绑定
来源：http://hdi.sxryk.cn

if let n = opt { print(n) }
来源：http://eyt.uphjek.com

[T20] Swift：数组操作
来源：http://tqm.mhx1999.top

var a = [1, 2, 3];  a.append(4)
来源：http://uob.cqqwz.cn

[T21] Swift：遍历
来源：http://hwb.hammf.cn

for x in a { print(x) }
来源：http://efu.yuxming.cn

[T22] Swift：字典
来源：http://yas.yonumen.top

var d = ["a": 1];  d["b"] = 2
来源：http://jlk.shanyushiyangtech.top

[T23] Swift：函数
来源：http://gba.yangfankeji.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://itv.aizwys.cn

[T24] Swift：闭包
来源：http://lwq.wangshuangyany.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zpl.jinyuanbaomall.cn

[T25] Swift：结构体
来源：http://uxt.sxryk.cn

struct P { var x: Int }
来源：http://jgy.yongpay.top

[T26] Swift：类与重写
来源：http://khf.vqdsnc.cn

class A: Base { override func f() {} }
来源：http://jlm.sufxvd.cn

[T27] Swift：错误处理
来源：http://bre.52xcode.cn

do { try f() } catch { print(error) }
来源：http://ebk.tian-w.cn

[T28] Swift：枚举
来源：http://dyz.daria6918.cn

enum Color { case red, green }
来源：http://rnx.yuxming.cn

[T29] Swift：guard 提前返回
来源：http://xoi.meibo888.top

guard let x = opt else { return }
来源：http://ofu.smart0.xyz

[T30] Swift：协议
来源：http://qhn.nanxinkj.top

protocol Shape { func area() -> Double }
来源：http://wls.epnwcf.com

[T31] Lua：Hello World
来源：http://yke.dianchejie.cn

print("Hello")
来源：http://ait.pengpengdd.cyou

[T32] Lua：局部变量
来源：http://cdd.316326.xyz

local a = 1
来源：http://uoz.feifeiyinyue.top

[T33] Lua：表（数组）
来源：http://lfe.meibo888.top

local t = {1, 2, 3};  t[4] = 4
来源：http://hhr.hongshengwenyu.top

[T34] Lua：遍历表
来源：http://zlx.9152youxi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kqn.zhoulong.xyz

[T35] Lua：字典表
来源：http://vqe.svipenyu.cn

local d = { a = 1 };  d.b = 2
来源：http://xzc.jianghu66.top

[T36] Lua：函数
来源：http://yfw.ehwqpu.com

function add(a, b) return a + b end
来源：http://xrg.52xcode.cn

[T37] Lua：字符串拼接
来源：http://lqz.yj202588.top

"a" .. "b"
来源：http://gtg.nanxinkj.top

[T38] Lua：条件
来源：http://fcd.sweek.top

if x > 0 then print("正") end
来源：http://gmb.guannengcc.top

[T39] Lua：模式匹配
来源：http://upn.hfpthk.cn

string.find(s, "%d+")
来源：http://vmj.dianchejie.cn

[T40] Lua：元表
来源：http://yep.316326.xyz

setmetatable({}, { __index = base })
来源：http://apq.nwbrower.top

[T41] Perl：Hello World
来源：http://tjz.0kj1m.cn

print "Hello\n";
来源：http://pgj.sysykeji.top

[T42] Perl：变量类型
来源：http://fzs.sysykeji.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kzw.sweek.top

[T43] Perl：字符串插值
来源：http://yvy.ehwqpu.com

"值: $a"
来源：http://gun.zhijiandao.cn

[T44] Perl：条件
来源：http://tzw.meibo888.top

if ($a > 0) { print "正"; }
来源：http://ulm.zhaomingkeji.xyz

[T45] Perl：数组遍历
来源：http://zlw.hammf.cn

for my $x (@arr) { print $x; }
来源：http://jmo.yj202588.top

[T46] Perl：哈希操作
来源：http://der.yanxiufei.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pop.shzxlz.cn

[T47] Perl：正则捕获
来源：http://nvw.fengsongda.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://rpq.yongpay.top

[T48] Perl：正则替换
来源：http://zbu.tanke756.top

$s =~ s/old/new/g;
来源：http://uve.zhengqikj.top

[T49] Perl：函数
来源：http://sox.tanke756.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pvc.uphjek.com

[T50] Perl：逐行读文件
来源：http://yoq.hnqzz.top

open my $fh, "<", "a.txt" or die $!;
来源：http://kbs.hongshengwenyu.top

while (my $line = <$fh>) { print $line; }
来源：http://nhr.xuetiantiany.cn

[T51] Scala：Hello World
来源：http://srz.dianchejie.cn

println("Hello")
来源：http://qfn.jiagoushi.top

[T52] Scala：变量
来源：http://ytf.ppjwa.cn

val a = 1;  var b = 2
来源：http://zqa.yvedp.cn

[T53] Scala：字符串插值
来源：http://wkr.zhijiandao.cn

s"值: $b"
来源：http://jdz.chenjidiqi.icu

[T54] Scala：集合映射
来源：http://imo.xingfuxueyuan.xyz

List(1, 2, 3).map(_ * 2)
来源：http://dne.sjlbkw.cn

[T55] Scala：集合过滤
来源：http://oyh.dianchejie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fnp.ivvv.top

[T56] Scala：样例类
来源：http://rnp.sxryk.cn

case class User(name: String, age: Int)
来源：http://vby.yonumen.top

[T57] Scala：模式匹配
来源：http://ihh.shzxlz.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://rua.nanxinkj.top

[T58] Scala：函数定义
来源：http://ogv.wangshuangyany.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lwo.yonumen.top

[T59] Scala：循环
来源：http://jkq.zhiwuduotai.top

for (i <- 1 to 10) println(i)
来源：http://zgp.meibo888.top

[T60] Scala：折叠
来源：http://fkd.hesvh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jtq.daxiang520.top

================================================================================
来源：http://nfs.zhixingplan.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uvd.hfpthk.cn

================================================================================
来源：http://rcv.hcnkem.com

[U01] Py：创建虚拟环境
来源：http://ebv.tianlin.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://khj.redwolf501.top

[U02] Py：导出 / 安装依赖
来源：http://ana.shuidangran.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tzz.aibaodan.cn

[U03] Py：加载 .env 配置
来源：http://puq.zhixingplan.top

from dotenv import load_dotenv; load_dotenv()
来源：http://fxy.fzhhl.top

[U04] Py：变量调试打印
来源：http://vjd.yangfankeji.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kpq.yueranfly.top

[U05] Py：列表去重且保序
来源：http://lqc.52xcode.cn

list(dict.fromkeys(arr))
来源：http://xom.bjfxy.top

[U06] Py：合并两个字典
来源：http://vvj.yfazqb.com

{**a, **b}
来源：http://iqt.daxiang520.top

[U07] Py：反转字典键值
来源：http://gae.zdbjq.cn

{v: k for k, v in d.items()}
来源：http://euo.ctjpmb.com

[U08] Py：展平二维列表
来源：http://jed.52xcode.cn

[y for x in nested for y in x]
来源：http://byt.wangdashe.top

[U09] Py：字典取最大值的键
来源：http://oyk.yj20258.top

max(d, key=d.get)
来源：http://scq.dianchejie.cn

[U10] Py：按值排序字典
来源：http://fgg.dianchejie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xqk.fengsongda.top

[U11] Py：生成器表达式
来源：http://fdm.zhijiandao.cn

(x * 2 for x in arr)
来源：http://hht.quarkkingdee.top

[U12] Py：取出现最多的 3 个元素
来源：http://vri.nanxuanxn.top

Counter(arr).most_common(3)
来源：http://uut.hongshengwenyu.top


<!-- 参考信息 -->