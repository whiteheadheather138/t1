代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://opn.wangdashe.top

[R72] 等待端口就绪
来源：http://bbg.yuxming.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://orq.xziqi.cn

[R73] 分割大日志
来源：http://dqx.birdmap.top

split -l 1000 big.log part_
来源：http://ezc.yongpay.top

[R74] 批量重命名
来源：http://xev.dianchejie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iqi.c1oappe.top

[R75] 导出环境变量
来源：http://vev.xuetiantiany.cn

export PATH="$HOME/bin:$PATH"
来源：http://mcu.havefunace.top

[R76] 使用临时文件
来源：http://jjj.zdqjudy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cwp.316326.xyz

[R77] 读取用户输入
来源：http://ele.ctjpmb.com

read -rp "请输入: " ans
来源：http://ywq.hnxiangtu.top

[R78] 交互式菜单
来源：http://qzx.hcnkem.com

select opt in a b c; do echo "$opt"; break; done
来源：http://vul.yj202588.top

[R79] 解析命令行选项
来源：http://nit.jlsjyb.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lwj.xuanzx.com

[R80] 查看脚本执行耗时
来源：http://gik.svipenyu.cn

time ./run.sh
来源：http://rir.wangdashe.top

================================================================================
来源：http://vxb.jianghu66.top

S. C / C++ 专题
来源：http://xcb.xinyue.icu

================================================================================
来源：http://skp.shuidangran.top

[S01] C：Hello World
来源：http://dkt.tarul.cn

#include <stdio.h>
来源：http://ooj.vehdjk.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://rxu.haohaochexian.top

[S02] C：变量与格式化输出
来源：http://cgx.yonumen.top

int a = 10; printf("%d\n", a);
来源：http://wym.shanyushiyangtech.top

[S03] C：读入整数
来源：http://hdn.sysykeji.top

int x; scanf("%d", &x);
来源：http://jdf.birdmap.top

[S04] C：字符串复制
来源：http://oye.hnxiangtu.top

char dst[32]; strcpy(dst, "hi");
来源：http://tqt.jinghuilouyu.cn

[S05] C：字符串长度
来源：http://zud.0kj1m.cn

strlen(s)
来源：http://bfk.hnxiangtu.top

[S06] C：字符串比较
来源：http://ihr.yuanzhike.top

strcmp(a, b) == 0
来源：http://jji.zhijiandao.cn

[S07] C：数组遍历求和
来源：http://ejh.aizwys.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://acu.guowangkeji.top

[S08] C：动态内存分配与释放
来源：http://vlv.ppjwa.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eti.zhoulong.xyz

[S09] C：结构体定义与初始化
来源：http://bzg.nanxuanxn.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://psa.yj202588.top

[S10] C：指针与解引用
来源：http://wpi.zhixingplan.top

int *p = &a;  *p = 5;
来源：http://iuq.ydjk.org.cn

[S11] C：逐行读文件
来源：http://gwf.hnqzz.top

FILE *f = fopen("a.txt", "r");
来源：http://fxc.jyoumei.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pjs.vqdsnc.cn

fclose(f);
来源：http://fvk.xinyue.icu

[S12] C：写文件
来源：http://htg.sxryk.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mpg.sweek.top

[S13] C：宏定义
来源：http://see.316326.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://avx.yongpay.top

[S14] C：枚举
来源：http://fwq.ctjpmb.com

enum Color { RED, GREEN, BLUE };
来源：http://lug.yj20258.top

[S15] C：类型转换
来源：http://cnl.nanxinkj.top

(double) a / b
来源：http://rbv.hywenlv.cn

[S16] C：位操作置位
来源：http://ghs.bjfxy.top

x |= (1 << 3);
来源：http://weh.iojbl.cn

[S17] C：安全拼接字符串
来源：http://ars.yuxming.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://riq.cucudq.cn

[S18] C：命令行参数
来源：http://mbv.cdnleiting.top

int main(int argc, char **argv)
来源：http://wxg.yonumen.top

[S19] C：快速排序
来源：http://fek.ctjpmb.com

qsort(a, n, sizeof(int), cmp);
来源：http://ubl.zhijiandao.cn

[S20] C：二分查找
来源：http://meb.zdqjudy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cae.kuanghao11.cn

[S21] C：字符类别判断
来源：http://vml.nwbrower.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cec.ctjpmb.com

[S22] C：字符串转数字
来源：http://jdq.tianlin.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://oov.yfazqb.com

[S23] C：随机数
来源：http://zaw.epnwcf.com

srand(time(NULL));  int r = rand() % 100;
来源：http://wqs.wangshuangyany.cn

[S24] C：获取本地时间
来源：http://buf.fehbvm.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dme.chenzaomai.com

[S25] C：内存拷贝
来源：http://ubw.jinqigufen.top

memcpy(dst, src, n);
来源：http://vwm.jyoumei.cn

[S26] C：内存清零
来源：http://sfu.yj20258.top

memset(a, 0, sizeof a);
来源：http://veq.xuanzx.com

[S27] C：定义常量
来源：http://ahg.ydjk.org.cn

const double PI = 3.14159;
来源：http://qpa.ppjwa.cn

[S28] C：静态变量
来源：http://hra.hfpthk.cn

static int counter = 0;
来源：http://fez.sweek.top

[S29] C：变参函数
来源：http://hnm.gogol.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tli.52xcode.cn

[S30] C：头文件保护
来源：http://cew.zhengqikj.top

#ifndef X_H
来源：http://anm.ydzc1.top

#define X_H
来源：http://nkf.tianlin.xyz

#endif
来源：http://vor.feifeiyinyue.top

[S31] C++：Hello World
来源：http://ajw.fzhhl.top

#include <iostream>
来源：http://zui.tian-w.cn

int main() { std::cout << "Hello\n"; }
来源：http://omw.hesvh.cn

[S32] C++：字符串
来源：http://jjc.yueranfly.top

std::string s = "hi";  s += "!";
来源：http://mnd.iojbl.cn

[S33] C++：vector 增删
来源：http://gsu.iojbl.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bud.redwolf501.top

[S34] C++：遍历 vector
来源：http://twq.mhx1999.top

for (auto &x : v) { std::cout << x; }
来源：http://ukl.xuetiantiany.cn

[S35] C++：map
来源：http://uev.epnwcf.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nqm.fehbvm.com

[S36] C++：unordered_map
来源：http://ipm.redwolf501.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://oif.dianchejie.cn

[S37] C++：set
来源：http://ftp.ydjk.org.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gzf.yj20258.top

[S38] C++：排序
来源：http://nwu.guowangkeji.top

std::sort(v.begin(), v.end());
来源：http://dxu.yfazqb.com

[S39] C++：自定义比较器排序
来源：http://yij.hnxiangtu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oba.zdbjq.cn

[S40] C++：查找元素
来源：http://ynx.shzxlz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://okp.c1oappe.top

[S41] C++：类与构造函数
来源：http://nnx.fanxiaobao.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jwf.aibaodan.cn

[S42] C++：继承与虚函数
来源：http://xuv.gotoacloud.top

class B : public Base { public: void f() override {} };
来源：http://wxl.cqqwz.cn

[S43] C++：智能指针
来源：http://bgx.ybcxt.top

auto p = std::make_unique<int>(5);
来源：http://uxa.kuanghao11.cn

[S44] C++：引用传参
来源：http://bph.aizwys.cn

void inc(int &x) { ++x; }
来源：http://hji.wangdashe.top

[S45] C++：lambda
来源：http://knj.xziqi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gwc.jqgfzy.top

[S46] C++：函数模板
来源：http://jjm.yuxming.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rrv.dashuyun.cn

[S47] C++：结构化绑定遍历
来源：http://law.gaohongyu789.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dhk.chenjidiqi.icu

[S48] C++：逐行读文件
来源：http://win.c1oappe.top

std::ifstream in("a.txt");  std::string line;
来源：http://sjq.zhoulong.xyz

while (std::getline(in, line)) { }
来源：http://kek.hysaishi.cn

[S49] C++：写文件
来源：http://stx.ydzc1.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hqf.gogol.net.cn

[S50] C++：格式化数字
来源：http://mvl.shangyingyoupin.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uwa.kuanghao11.cn

[S51] C++：显式类型转换
来源：http://ykp.tanke756.top

static_cast<double>(a) / b
来源：http://bat.uphjek.com

[S52] C++：const 与 noexcept
来源：http://dxd.zdqjudy.top

int size() const noexcept { return n_; }
来源：http://wih.zhongyouzk.top

[S53] C++：移动语义
来源：http://zhw.ppjwa.cn

std::vector<int> w = std::move(v);
来源：http://xyg.sysykeji.top

[S54] C++：异常处理
来源：http://pep.sjlbkw.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cfw.ybcxt.top

[S55] C++：结构化绑定
来源：http://bhp.aibaodan.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cos.ctjpmb.com

[S56] C++：optional
来源：http://pyi.xinyue.icu

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zlf.hongshengwenyu.top

[S57] C++：编译期常量
来源：http://opq.tianlin.xyz

constexpr int N = 10;
来源：http://est.snrcjt.cn

[S58] C++：命名空间
来源：http://hdv.yj20258888.top

namespace ns { int f() { return 1; } }
来源：http://aoa.zdqjudy.top

[S59] C++：静态断言
来源：http://yso.andypj.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xni.xingfuxueyuan.xyz

[S60] C++：遍历并删除元素
来源：http://bts.smart0.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fhj.vqdsnc.cn

================================================================================
来源：http://qbd.yongpay.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://svz.ydjk.org.cn

================================================================================
来源：http://tdm.sufxvd.cn

[T01] Kotlin：Hello World
来源：http://gbk.dianchejie.cn

println("Hello")
来源：http://esj.yj20258.top

[T02] Kotlin：变量
来源：http://czw.aibaodan.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yaf.cheryme.top

[T03] Kotlin：字符串模板
来源：http://ylo.vqdsnc.cn

"值: $b"
来源：http://nns.xziqi.cn

[T04] Kotlin：空安全
来源：http://ilu.shzxlz.cn

val n: String? = null;  n?.length
来源：http://yok.hesvh.cn

[T05] Kotlin：when 表达式
来源：http://wrc.cheryme.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cdj.yangfankeji.com

[T06] Kotlin：集合映射
来源：http://awn.snrcjt.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ssd.yangfankeji.com

[T07] Kotlin：集合过滤
来源：http://bat.hnqzz.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://tek.nwbrower.top

[T08] Kotlin：数据类
来源：http://bpr.shzxlz.cn

data class User(val name: String, val age: Int)
来源：http://ooq.quarkkingdee.top

[T09] Kotlin：扩展函数
来源：http://pfz.ehwqpu.com

fun String.exclaim() = this + "!"
来源：http://pdw.0kj1m.cn

[T10] Kotlin：默认参数
来源：http://yjw.fktsv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vap.sysykeji.top

[T11] Kotlin：协程
来源：http://kpj.nanxuanxn.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://psp.hywenlv.cn

[T12] Kotlin：解构声明
来源：http://kbd.jlsjyb.cn

val (a, b) = Pair(1, 2)
来源：http://ona.guowangkeji.top

[T13] Kotlin：只读 Map
来源：http://icz.ppjwa.cn

val m = mapOf("a" to 1)
来源：http://dmf.svipenyu.cn

[T14] Kotlin：循环
来源：http://kzu.gogol.net.cn

for (i in 1..10) println(i)
来源：http://ytg.0kj1m.cn

[T15] Kotlin：接口
来源：http://lez.yonumen.top

interface Shape { fun area(): Double }
来源：http://lkn.jqgufenzy.top

[T16] Swift：Hello World
来源：http://ekv.shzxlz.cn

print("Hello")
来源：http://jpy.yj202588.top

[T17] Swift：变量与常量
来源：http://brw.shanyushiyangtech.top

var a = 1;  let b = 2
来源：http://dyh.daria6918.cn

[T18] Swift：字符串插值
来源：http://uep.ywan-chungtsiang.top

"值: \(b)"
来源：http://ngk.ydzc1.top

[T19] Swift：可选绑定
来源：http://aqi.pengpengdd.cyou

if let n = opt { print(n) }
来源：http://dnx.ivvv.top

[T20] Swift：数组操作
来源：http://aac.shanyushiyangtech.top

var a = [1, 2, 3];  a.append(4)
来源：http://ebk.tarul.cn

[T21] Swift：遍历
来源：http://eza.dashuyun.cn

for x in a { print(x) }
来源：http://djm.aibaodan.cn

[T22] Swift：字典
来源：http://wvo.jiagoushi.top

var d = ["a": 1];  d["b"] = 2
来源：http://olf.zhixingplan.top

[T23] Swift：函数
来源：http://mae.nwbrower.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wuw.jqgufenzy.top

[T24] Swift：闭包
来源：http://olk.hnqzz.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://yyn.pengpengdd.cyou

[T25] Swift：结构体
来源：http://crb.jinqigfzy.top

struct P { var x: Int }
来源：http://txy.yangfankeji.com

[T26] Swift：类与重写
来源：http://mri.fanxiaobao.xyz

class A: Base { override func f() {} }
来源：http://tje.kuanghao11.cn

[T27] Swift：错误处理
来源：http://uor.zhoulong.xyz

do { try f() } catch { print(error) }
来源：http://fsw.xinyue.icu

[T28] Swift：枚举
来源：http://uyg.hnxiangtu.top

enum Color { case red, green }
来源：http://wxm.jinqigfzy.top

[T29] Swift：guard 提前返回
来源：http://umj.kuanghao11.cn

guard let x = opt else { return }
来源：http://ygw.hysaishi.cn

[T30] Swift：协议
来源：http://qew.jinqigfzy.top

protocol Shape { func area() -> Double }
来源：http://cfj.quarkkingdee.top

[T31] Lua：Hello World
来源：http://now.smart0.xyz

print("Hello")
来源：http://tde.snrcjt.cn

[T32] Lua：局部变量
来源：http://emu.redwolf501.top

local a = 1
来源：http://tsi.jyoumei.cn

[T33] Lua：表（数组）
来源：http://phw.bjfxy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://map.wangshuangyany.cn

[T34] Lua：遍历表
来源：http://lbv.316326.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://srd.xingfuxueyuan.xyz

[T35] Lua：字典表
来源：http://eoa.gaohongyu789.top

local d = { a = 1 };  d.b = 2
来源：http://ugq.0kj1m.cn

[T36] Lua：函数
来源：http://bcu.gzhubu.top

function add(a, b) return a + b end
来源：http://stb.jlsjyb.cn

[T37] Lua：字符串拼接
来源：http://umb.jyoumei.cn

"a" .. "b"
来源：http://tzw.smart0.xyz

[T38] Lua：条件
来源：http://hcc.xuetiantiany.cn

if x > 0 then print("正") end
来源：http://blh.sufxvd.cn

[T39] Lua：模式匹配
来源：http://jcg.gaohongyu789.top

string.find(s, "%d+")
来源：http://gxe.shuidangran.top

[T40] Lua：元表
来源：http://xuz.yueranfly.top

setmetatable({}, { __index = base })
来源：http://htp.ivvv.top

[T41] Perl：Hello World
来源：http://cci.9152youxi.cn

print "Hello\n";
来源：http://hjj.andypj.xyz

[T42] Perl：变量类型
来源：http://usc.fzhhl.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fzf.daria6918.cn

[T43] Perl：字符串插值
来源：http://tdd.sysykeji.top

"值: $a"
来源：http://wag.fzhhl.top

[T44] Perl：条件
来源：http://hxp.fzhhl.top

if ($a > 0) { print "正"; }
来源：http://gam.hywenlv.cn

[T45] Perl：数组遍历
来源：http://wux.snrcjt.cn

for my $x (@arr) { print $x; }
来源：http://xid.9152youxi.cn

[T46] Perl：哈希操作
来源：http://jjg.sweek.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tvc.birdmap.top

[T47] Perl：正则捕获
来源：http://lmp.chenzaomai.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://isk.nanxinkj.top

[T48] Perl：正则替换
来源：http://qwb.xingfuxueyuan.xyz

$s =~ s/old/new/g;
来源：http://vce.aibaodan.cn

[T49] Perl：函数
来源：http://gfq.pycfn.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gdl.xingfuxueyuan.xyz

[T50] Perl：逐行读文件
来源：http://eui.meibo888.top

open my $fh, "<", "a.txt" or die $!;
来源：http://fnt.mhx1999.top

while (my $line = <$fh>) { print $line; }
来源：http://efh.guowangkeji.top

[T51] Scala：Hello World
来源：http://hri.ctjpmb.com

println("Hello")
来源：http://vwc.yangfankeji.com

[T52] Scala：变量
来源：http://ruz.jinghuilouyu.cn

val a = 1;  var b = 2
来源：http://mfg.fzhhl.top

[T53] Scala：字符串插值
来源：http://gak.yj20258888.top

s"值: $b"
来源：http://ccy.hcnkem.com

[T54] Scala：集合映射
来源：http://wsg.c1oappe.top

List(1, 2, 3).map(_ * 2)
来源：http://omf.hfpthk.cn

[T55] Scala：集合过滤
来源：http://ylr.gotoacloud.top

List(1, 2, 3).filter(_ > 1)
来源：http://dhx.aibaodan.cn

[T56] Scala：样例类
来源：http://rfr.vqdsnc.cn

case class User(name: String, age: Int)
来源：http://sda.uphjek.com

[T57] Scala：模式匹配
来源：http://pzh.sjlbkw.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wph.zhixingplan.top

[T58] Scala：函数定义
来源：http://kay.shuidangran.top

def add(a: Int, b: Int): Int = a + b
来源：http://sow.smart0.xyz

[T59] Scala：循环
来源：http://hzv.chenlongwang.top

for (i <- 1 to 10) println(i)
来源：http://bbl.uphjek.com

[T60] Scala：折叠
来源：http://pci.chenlongwang.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mla.birdmap.top

================================================================================
来源：http://igq.cdnleiting.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qzx.sweek.top

================================================================================
来源：http://pfd.hfpthk.cn

[U01] Py：创建虚拟环境
来源：http://lim.fktsv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://imc.ehwqpu.com

[U02] Py：导出 / 安装依赖
来源：http://fkh.hfpthk.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ysy.redwolf501.top

[U03] Py：加载 .env 配置
来源：http://suf.aibaodan.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dlu.sufxvd.cn

[U04] Py：变量调试打印
来源：http://feb.52xcode.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pnp.sweek.top

[U05] Py：列表去重且保序
来源：http://lbf.gzhubu.top

list(dict.fromkeys(arr))
来源：http://ahr.nanxinkj.top

[U06] Py：合并两个字典
来源：http://ryr.daxiang520.top

{**a, **b}
来源：http://cxd.zhixingplan.top

[U07] Py：反转字典键值
来源：http://ahq.zhiwuduotai.top

{v: k for k, v in d.items()}
来源：http://ilc.yj202588.top

[U08] Py：展平二维列表
来源：http://uzp.yueranfly.top

[y for x in nested for y in x]
来源：http://mbc.9152youxi.cn

[U09] Py：字典取最大值的键
来源：http://pky.ybcxt.top

max(d, key=d.get)
来源：http://szx.cucudq.cn

[U10] Py：按值排序字典
来源：http://vql.cheryme.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://tux.zhoulong.xyz

[U11] Py：生成器表达式
来源：http://gft.dashuyun.cn

(x * 2 for x in arr)
来源：http://xoo.zhengqikj.top

[U12] Py：取出现最多的 3 个元素
来源：http://esl.hywenlv.cn

Counter(arr).most_common(3)
来源：http://vqu.redwolf501.top


<!-- 参考信息 -->