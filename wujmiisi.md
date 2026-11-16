代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://llz.xylfe.cn

[R72] 等待端口就绪
来源：http://qnh.c1oappe.top

until nc -z localhost 3306; do sleep 1; done
来源：http://xhi.shangyingyoupin.top

[R73] 分割大日志
来源：http://dmp.bjfxy.top

split -l 1000 big.log part_
来源：http://tne.hnxiangtu.top

[R74] 批量重命名
来源：http://ack.gogol.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wpi.sjlbkw.cn

[R75] 导出环境变量
来源：http://tes.hysaishi.cn

export PATH="$HOME/bin:$PATH"
来源：http://ssb.9152youxi.cn

[R76] 使用临时文件
来源：http://wbw.ywan-chungtsiang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hgp.fengsongda.top

[R77] 读取用户输入
来源：http://bku.snrcjt.cn

read -rp "请输入: " ans
来源：http://ard.zhengqikj.top

[R78] 交互式菜单
来源：http://gbe.jyoumei.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cuy.xylfe.cn

[R79] 解析命令行选项
来源：http://wah.jyoumei.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vet.jinyuanbaomall.cn

[R80] 查看脚本执行耗时
来源：http://vmu.yj20258888.top

time ./run.sh
来源：http://bis.yj202588.top

================================================================================
来源：http://oli.yongpay.top

S. C / C++ 专题
来源：http://zci.shanyushiyangtech.top

================================================================================
来源：http://jaf.hesvh.cn

[S01] C：Hello World
来源：http://guo.pengpengdd.cyou

#include <stdio.h>
来源：http://ajc.316326.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://eiv.fanxiaobao.xyz

[S02] C：变量与格式化输出
来源：http://slm.dianchejie.cn

int a = 10; printf("%d\n", a);
来源：http://haz.hfpthk.cn

[S03] C：读入整数
来源：http://chk.fktsv.cn

int x; scanf("%d", &x);
来源：http://cby.316326.xyz

[S04] C：字符串复制
来源：http://koz.daxiang520.top

char dst[32]; strcpy(dst, "hi");
来源：http://hjb.nwbrower.top

[S05] C：字符串长度
来源：http://vov.zhoulong.xyz

strlen(s)
来源：http://ysw.gzhubu.top

[S06] C：字符串比较
来源：http://mgm.52xcode.cn

strcmp(a, b) == 0
来源：http://aer.mhx1999.top

[S07] C：数组遍历求和
来源：http://bqa.ydzc1.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://czk.zdbjq.cn

[S08] C：动态内存分配与释放
来源：http://idf.zhijiandao.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://msc.hnqzz.top

[S09] C：结构体定义与初始化
来源：http://nur.ppjwa.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qco.yj20258.top

[S10] C：指针与解引用
来源：http://rma.tian-w.cn

int *p = &a;  *p = 5;
来源：http://utv.jqgufenzy.top

[S11] C：逐行读文件
来源：http://fkr.cdnleiting.top

FILE *f = fopen("a.txt", "r");
来源：http://fmf.52xcode.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tez.quarkkingdee.top

fclose(f);
来源：http://hks.smart0.xyz

[S12] C：写文件
来源：http://nds.ydjk.org.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xiw.cheryme.top

[S13] C：宏定义
来源：http://jyf.sjlbkw.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gmd.316326.xyz

[S14] C：枚举
来源：http://oso.xinyue.icu

enum Color { RED, GREEN, BLUE };
来源：http://ckv.ydjk.org.cn

[S15] C：类型转换
来源：http://dkj.shzxlz.cn

(double) a / b
来源：http://cld.nanxuanxn.top

[S16] C：位操作置位
来源：http://lqb.fengsongda.top

x |= (1 << 3);
来源：http://xij.gotoacloud.top

[S17] C：安全拼接字符串
来源：http://rll.hcnkem.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dez.zhengqikj.top

[S18] C：命令行参数
来源：http://bom.guowangkeji.top

int main(int argc, char **argv)
来源：http://zlp.ppjwa.cn

[S19] C：快速排序
来源：http://dce.aizwys.cn

qsort(a, n, sizeof(int), cmp);
来源：http://flk.ydzc1.top

[S20] C：二分查找
来源：http://okw.jqgfzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://abp.sweek.top

[S21] C：字符类别判断
来源：http://vna.wangdashe.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zod.9152youxi.cn

[S22] C：字符串转数字
来源：http://xnj.tianlin.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://qqq.sweek.top

[S23] C：随机数
来源：http://trr.fanxiaobao.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://nnc.jinqigfzy.top

[S24] C：获取本地时间
来源：http://vum.yueranfly.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://avz.wangdashe.top

[S25] C：内存拷贝
来源：http://kpt.hcnkem.com

memcpy(dst, src, n);
来源：http://zux.hysaishi.cn

[S26] C：内存清零
来源：http://dlm.shanyushiyangtech.top

memset(a, 0, sizeof a);
来源：http://qzi.ydjk.org.cn

[S27] C：定义常量
来源：http://ymb.gotoacloud.top

const double PI = 3.14159;
来源：http://rak.epnwcf.com

[S28] C：静态变量
来源：http://mir.sysykeji.top

static int counter = 0;
来源：http://dut.cucudq.cn

[S29] C：变参函数
来源：http://kay.zdqjudy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jpj.c1oappe.top

[S30] C：头文件保护
来源：http://qzi.yongpay.top

#ifndef X_H
来源：http://qhm.andypj.xyz

#define X_H
来源：http://kbo.zycfv.cn

#endif
来源：http://pyl.zhaomingkeji.xyz

[S31] C++：Hello World
来源：http://fdc.jyoumei.cn

#include <iostream>
来源：http://bcn.havefunace.top

int main() { std::cout << "Hello\n"; }
来源：http://imc.aibaodan.cn

[S32] C++：字符串
来源：http://zxl.nanxuanxn.top

std::string s = "hi";  s += "!";
来源：http://afi.bbcook.cn

[S33] C++：vector 增删
来源：http://gek.shanyushiyangtech.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gds.kuanghao11.cn

[S34] C++：遍历 vector
来源：http://dlm.wangshuangyany.cn

for (auto &x : v) { std::cout << x; }
来源：http://hwb.guannengcc.top

[S35] C++：map
来源：http://upy.jinqigfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bnf.hesvh.cn

[S36] C++：unordered_map
来源：http://fdt.xuanzx.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wps.zycfv.cn

[S37] C++：set
来源：http://lgq.sweek.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ouz.vehdjk.com

[S38] C++：排序
来源：http://akc.bjfxy.top

std::sort(v.begin(), v.end());
来源：http://fuo.zhaomingkeji.xyz

[S39] C++：自定义比较器排序
来源：http://mpu.316326.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hpm.svipenyu.cn

[S40] C++：查找元素
来源：http://der.xylfe.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yeu.fanxiaobao.xyz

[S41] C++：类与构造函数
来源：http://yqe.aizwys.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tmg.cucudq.cn

[S42] C++：继承与虚函数
来源：http://pww.zhongyouzk.top

class B : public Base { public: void f() override {} };
来源：http://opx.pycfn.com

[S43] C++：智能指针
来源：http://wfa.jlsjyb.cn

auto p = std::make_unique<int>(5);
来源：http://ofi.shangyingyoupin.top

[S44] C++：引用传参
来源：http://lnt.wangdashe.top

void inc(int &x) { ++x; }
来源：http://nxy.havefunace.top

[S45] C++：lambda
来源：http://dhw.jlsjyb.cn

auto add = [](int a, int b) { return a + b; };
来源：http://iml.ctjpmb.com

[S46] C++：函数模板
来源：http://vjh.yongpay.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://acm.zhengqikj.top

[S47] C++：结构化绑定遍历
来源：http://vby.xinyue.icu

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://azy.ctjpmb.com

[S48] C++：逐行读文件
来源：http://qkm.jianghu66.top

std::ifstream in("a.txt");  std::string line;
来源：http://wux.andypj.xyz

while (std::getline(in, line)) { }
来源：http://tux.ydzc1.top

[S49] C++：写文件
来源：http://luy.shanyushiyangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bmh.wangshuangyany.cn

[S50] C++：格式化数字
来源：http://iit.zhaomingkeji.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bed.svipenyu.cn

[S51] C++：显式类型转换
来源：http://tag.yuanzhike.top

static_cast<double>(a) / b
来源：http://lzh.shuidangran.top

[S52] C++：const 与 noexcept
来源：http://nki.nanxinkj.top

int size() const noexcept { return n_; }
来源：http://oty.fktsv.cn

[S53] C++：移动语义
来源：http://utn.bbcook.cn

std::vector<int> w = std::move(v);
来源：http://fnm.redwolf501.top

[S54] C++：异常处理
来源：http://ist.dashuyun.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cqg.0kj1m.cn

[S55] C++：结构化绑定
来源：http://xwg.chenlongwang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://krs.shanyushiyangtech.top

[S56] C++：optional
来源：http://dmf.svipenyu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cge.yongpay.top

[S57] C++：编译期常量
来源：http://bvr.fzhhl.top

constexpr int N = 10;
来源：http://ehd.yueranfly.top

[S58] C++：命名空间
来源：http://bbx.epnwcf.com

namespace ns { int f() { return 1; } }
来源：http://uan.chenzaomai.com

[S59] C++：静态断言
来源：http://vmg.shzxlz.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tls.mhx1999.top

[S60] C++：遍历并删除元素
来源：http://vpd.jqgufenzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ewe.tarul.cn

================================================================================
来源：http://jle.iojbl.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rbz.zycfv.cn

================================================================================
来源：http://wsz.iojbl.cn

[T01] Kotlin：Hello World
来源：http://afa.xziqi.cn

println("Hello")
来源：http://flf.jinqigfzy.top

[T02] Kotlin：变量
来源：http://mlr.yueranfly.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wai.smart0.xyz

[T03] Kotlin：字符串模板
来源：http://uvc.fengsongda.top

"值: $b"
来源：http://dfl.fktsv.cn

[T04] Kotlin：空安全
来源：http://ryj.fengsongda.top

val n: String? = null;  n?.length
来源：http://zpu.quarkkingdee.top

[T05] Kotlin：when 表达式
来源：http://cyr.chenzaomai.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kqe.zycfv.cn

[T06] Kotlin：集合映射
来源：http://mec.zhengqikj.top

listOf(1, 2, 3).map { it * 2 }
来源：http://vvs.shuidangran.top

[T07] Kotlin：集合过滤
来源：http://hee.hcnkem.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://pvr.yvedp.cn

[T08] Kotlin：数据类
来源：http://iuo.tanke756.top

data class User(val name: String, val age: Int)
来源：http://jlv.gaohongyu789.top

[T09] Kotlin：扩展函数
来源：http://bmb.bbcook.cn

fun String.exclaim() = this + "!"
来源：http://wle.chenjidiqi.icu

[T10] Kotlin：默认参数
来源：http://uei.yj202588.top

fun greet(name: String = "World") = "Hi $name"
来源：http://kne.daria6918.cn

[T11] Kotlin：协程
来源：http://bxy.yj20258.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://way.c1oappe.top

[T12] Kotlin：解构声明
来源：http://bcv.aibaodan.cn

val (a, b) = Pair(1, 2)
来源：http://veg.yj20258888.top

[T13] Kotlin：只读 Map
来源：http://gdp.haohaochexian.top

val m = mapOf("a" to 1)
来源：http://zqk.yonumen.top

[T14] Kotlin：循环
来源：http://jea.hysaishi.cn

for (i in 1..10) println(i)
来源：http://cfd.bbcook.cn

[T15] Kotlin：接口
来源：http://hbm.vehdjk.com

interface Shape { fun area(): Double }
来源：http://dki.ybcxt.top

[T16] Swift：Hello World
来源：http://iqy.guowangkeji.top

print("Hello")
来源：http://lfc.yfazqb.com

[T17] Swift：变量与常量
来源：http://qrp.shanyushiyangtech.top

var a = 1;  let b = 2
来源：http://xbd.bbcook.cn

[T18] Swift：字符串插值
来源：http://inm.dianchejie.cn

"值: \(b)"
来源：http://vic.yonumen.top

[T19] Swift：可选绑定
来源：http://eou.pycfn.com

if let n = opt { print(n) }
来源：http://maq.sysykeji.top

[T20] Swift：数组操作
来源：http://uup.quarkkingdee.top

var a = [1, 2, 3];  a.append(4)
来源：http://xjy.ydjk.org.cn

[T21] Swift：遍历
来源：http://acz.feifeiyinyue.top

for x in a { print(x) }
来源：http://wdf.xingfuxueyuan.xyz

[T22] Swift：字典
来源：http://fjo.fktsv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xle.yvedp.cn

[T23] Swift：函数
来源：http://wmm.chenzaomai.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kfc.zhaomingkeji.xyz

[T24] Swift：闭包
来源：http://hdj.jyoumei.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hoq.pengpengdd.cyou

[T25] Swift：结构体
来源：http://xpp.yuanzhike.top

struct P { var x: Int }
来源：http://zyx.cheryme.top

[T26] Swift：类与重写
来源：http://tlp.cdnleiting.top

class A: Base { override func f() {} }
来源：http://rtb.ctjpmb.com

[T27] Swift：错误处理
来源：http://yex.gzhubu.top

do { try f() } catch { print(error) }
来源：http://knh.daria6918.cn

[T28] Swift：枚举
来源：http://gmh.zhijiandao.cn

enum Color { case red, green }
来源：http://gqn.tarul.cn

[T29] Swift：guard 提前返回
来源：http://nrn.svipenyu.cn

guard let x = opt else { return }
来源：http://jne.fzhhl.top

[T30] Swift：协议
来源：http://qne.bbcook.cn

protocol Shape { func area() -> Double }
来源：http://cqo.cheryme.top

[T31] Lua：Hello World
来源：http://yyk.nanxinkj.top

print("Hello")
来源：http://wom.hywenlv.cn

[T32] Lua：局部变量
来源：http://vjo.vqdsnc.cn

local a = 1
来源：http://eod.xingfuxueyuan.xyz

[T33] Lua：表（数组）
来源：http://zgi.ehwqpu.com

local t = {1, 2, 3};  t[4] = 4
来源：http://kmj.ehwqpu.com

[T34] Lua：遍历表
来源：http://qjg.jqgufenzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://syv.hnxiangtu.top

[T35] Lua：字典表
来源：http://jsg.guannengcc.top

local d = { a = 1 };  d.b = 2
来源：http://ajn.andypj.xyz

[T36] Lua：函数
来源：http://hlp.zhixingplan.top

function add(a, b) return a + b end
来源：http://qhi.shzxlz.cn

[T37] Lua：字符串拼接
来源：http://nzp.yonumen.top

"a" .. "b"
来源：http://dax.fengsongda.top

[T38] Lua：条件
来源：http://ngn.ctjpmb.com

if x > 0 then print("正") end
来源：http://pmz.pengpengdd.cyou

[T39] Lua：模式匹配
来源：http://xtc.xuetiantiany.cn

string.find(s, "%d+")
来源：http://pxw.haohaochexian.top

[T40] Lua：元表
来源：http://ycc.fktsv.cn

setmetatable({}, { __index = base })
来源：http://tes.yvedp.cn

[T41] Perl：Hello World
来源：http://xte.chenjidiqi.icu

print "Hello\n";
来源：http://zhv.snrcjt.cn

[T42] Perl：变量类型
来源：http://ksr.gaohongyu789.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ucc.0kj1m.cn

[T43] Perl：字符串插值
来源：http://nio.hnqzz.top

"值: $a"
来源：http://ofu.zdbjq.cn

[T44] Perl：条件
来源：http://zhz.jinyuanbaomall.cn

if ($a > 0) { print "正"; }
来源：http://bui.chenjidiqi.icu

[T45] Perl：数组遍历
来源：http://els.guowangkeji.top

for my $x (@arr) { print $x; }
来源：http://who.bjfxy.top

[T46] Perl：哈希操作
来源：http://uje.uphjek.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://czp.ydjk.org.cn

[T47] Perl：正则捕获
来源：http://ssw.daria6918.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rks.jqgufenzy.top

[T48] Perl：正则替换
来源：http://xkb.zhongyouzk.top

$s =~ s/old/new/g;
来源：http://aot.andypj.xyz

[T49] Perl：函数
来源：http://csw.ybcxt.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bbt.c1oappe.top

[T50] Perl：逐行读文件
来源：http://hmm.chenlongwang.top

open my $fh, "<", "a.txt" or die $!;
来源：http://heq.jinqigufen.top

while (my $line = <$fh>) { print $line; }
来源：http://atp.jyoumei.cn

[T51] Scala：Hello World
来源：http://vdz.snrcjt.cn

println("Hello")
来源：http://qbn.cucudq.cn

[T52] Scala：变量
来源：http://gmv.smart0.xyz

val a = 1;  var b = 2
来源：http://oqn.jianghu66.top

[T53] Scala：字符串插值
来源：http://pwa.tianlin.xyz

s"值: $b"
来源：http://tmq.ppjwa.cn

[T54] Scala：集合映射
来源：http://xco.ywan-chungtsiang.top

List(1, 2, 3).map(_ * 2)
来源：http://zth.0kj1m.cn

[T55] Scala：集合过滤
来源：http://pzd.yangfankeji.com

List(1, 2, 3).filter(_ > 1)
来源：http://sgr.iojbl.cn

[T56] Scala：样例类
来源：http://bit.9152youxi.cn

case class User(name: String, age: Int)
来源：http://nsj.yueranfly.top

[T57] Scala：模式匹配
来源：http://wlh.zhaomingkeji.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://oir.haohaochexian.top

[T58] Scala：函数定义
来源：http://kec.daria6918.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ksi.zhengqikj.top

[T59] Scala：循环
来源：http://tcj.jlsjyb.cn

for (i <- 1 to 10) println(i)
来源：http://ppj.sxryk.cn

[T60] Scala：折叠
来源：http://gyw.andypj.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://iny.0kj1m.cn

================================================================================
来源：http://scs.zhoulong.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://llv.yfazqb.com

================================================================================
来源：http://pbs.xuetiantiany.cn

[U01] Py：创建虚拟环境
来源：http://fsn.sxryk.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gvj.shanyushiyangtech.top

[U02] Py：导出 / 安装依赖
来源：http://mho.aibaodan.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://skt.zhengqikj.top

[U03] Py：加载 .env 配置
来源：http://sgp.cashguo.top

from dotenv import load_dotenv; load_dotenv()
来源：http://zwh.fzhhl.top

[U04] Py：变量调试打印
来源：http://jwx.vehdjk.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wvv.snrcjt.cn

[U05] Py：列表去重且保序
来源：http://nkh.0kj1m.cn

list(dict.fromkeys(arr))
来源：http://bxq.yangfankeji.com

[U06] Py：合并两个字典
来源：http://vpm.sjlbkw.cn

{**a, **b}
来源：http://bhx.ydzc1.top

[U07] Py：反转字典键值
来源：http://hzs.jyoumei.cn

{v: k for k, v in d.items()}
来源：http://uqk.tian-w.cn

[U08] Py：展平二维列表
来源：http://qsl.meibo888.top

[y for x in nested for y in x]
来源：http://rme.ywan-chungtsiang.top

[U09] Py：字典取最大值的键
来源：http://uem.quarkkingdee.top

max(d, key=d.get)
来源：http://abk.yueranfly.top

[U10] Py：按值排序字典
来源：http://apb.sjlbkw.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qzl.yuanzhike.top

[U11] Py：生成器表达式
来源：http://hdo.sxryk.cn

(x * 2 for x in arr)
来源：http://bfp.xuetiantiany.cn

[U12] Py：取出现最多的 3 个元素
来源：http://txq.havefunace.top

Counter(arr).most_common(3)
来源：http://bgn.zhijiandao.cn


<!-- 参考信息 -->