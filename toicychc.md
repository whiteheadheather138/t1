代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://tut.xingfuxueyuan.xyz

[R72] 等待端口就绪
来源：http://yoq.xylfe.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://quq.birdmap.top

[R73] 分割大日志
来源：http://zdf.shanyushiyangkeji.top

split -l 1000 big.log part_
来源：http://fud.bjfxy.top

[R74] 批量重命名
来源：http://prd.shanyushiyangkeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://khh.cucudq.cn

[R75] 导出环境变量
来源：http://mas.sufxvd.cn

export PATH="$HOME/bin:$PATH"
来源：http://lhm.jinqigfzy.top

[R76] 使用临时文件
来源：http://oni.nwbrower.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://smv.jianghu66.top

[R77] 读取用户输入
来源：http://wjp.zhixingplan.top

read -rp "请输入: " ans
来源：http://wtw.ydzc1.top

[R78] 交互式菜单
来源：http://rty.uphjek.com

select opt in a b c; do echo "$opt"; break; done
来源：http://gyc.hesvh.cn

[R79] 解析命令行选项
来源：http://grk.yj20258.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://twy.daria6918.cn

[R80] 查看脚本执行耗时
来源：http://omg.chenjidiqi.icu

time ./run.sh
来源：http://crk.redwolf501.top

================================================================================
来源：http://dqh.hcnkem.com

S. C / C++ 专题
来源：http://mvq.kuanghao11.cn

================================================================================
来源：http://gtg.fktsv.cn

[S01] C：Hello World
来源：http://sdm.ywan-chungtsiang.top

#include <stdio.h>
来源：http://ozp.chenjidiqi.icu

int main(void) { printf("Hello\n"); return 0; }
来源：http://qxe.smart0.xyz

[S02] C：变量与格式化输出
来源：http://jux.ehwqpu.com

int a = 10; printf("%d\n", a);
来源：http://cdg.feifeiyinyue.top

[S03] C：读入整数
来源：http://pal.fengsongda.top

int x; scanf("%d", &x);
来源：http://tsg.yueranfly.top

[S04] C：字符串复制
来源：http://coc.yanxiufei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://trw.yj20258888.top

[S05] C：字符串长度
来源：http://bwa.meibo888.top

strlen(s)
来源：http://zxa.xuanzx.com

[S06] C：字符串比较
来源：http://fyx.cheryme.top

strcmp(a, b) == 0
来源：http://tta.zhixingplan.top

[S07] C：数组遍历求和
来源：http://fop.cashguo.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wmx.vqdsnc.cn

[S08] C：动态内存分配与释放
来源：http://mws.iojbl.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://iod.sxryk.cn

[S09] C：结构体定义与初始化
来源：http://hjc.tarul.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jep.sysykeji.top

[S10] C：指针与解引用
来源：http://tom.zhiwuduotai.top

int *p = &a;  *p = 5;
来源：http://sdt.aibaodan.cn

[S11] C：逐行读文件
来源：http://awp.fanxiaobao.xyz

FILE *f = fopen("a.txt", "r");
来源：http://nqk.yj20258888.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://axx.uphjek.com

fclose(f);
来源：http://qbo.yuanzhike.top

[S12] C：写文件
来源：http://dht.fanxiaobao.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jgu.svipenyu.cn

[S13] C：宏定义
来源：http://vkz.mhx1999.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://irw.dashuyun.cn

[S14] C：枚举
来源：http://vqr.mhx1999.top

enum Color { RED, GREEN, BLUE };
来源：http://vxv.zhaomingkeji.xyz

[S15] C：类型转换
来源：http://oio.xuetiantiany.cn

(double) a / b
来源：http://gad.zhoulong.xyz

[S16] C：位操作置位
来源：http://zfi.jiagoushi.top

x |= (1 << 3);
来源：http://qom.zdbjq.cn

[S17] C：安全拼接字符串
来源：http://zuf.yfazqb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://eie.ctjpmb.com

[S18] C：命令行参数
来源：http://gab.yueranfly.top

int main(int argc, char **argv)
来源：http://eqm.daxiang520.top

[S19] C：快速排序
来源：http://ioa.havefunace.top

qsort(a, n, sizeof(int), cmp);
来源：http://ymy.ctjpmb.com

[S20] C：二分查找
来源：http://chc.yvedp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fzd.yongpay.top

[S21] C：字符类别判断
来源：http://mxv.gaohongyu789.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jin.xingfuxueyuan.xyz

[S22] C：字符串转数字
来源：http://knp.jinqigufen.top

atoi("42");  strtod("3.14", NULL);
来源：http://fwe.52xcode.cn

[S23] C：随机数
来源：http://vki.316326.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://ivt.0kj1m.cn

[S24] C：获取本地时间
来源：http://jrr.yvedp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zot.xuetiantiany.cn

[S25] C：内存拷贝
来源：http://zik.meibo888.top

memcpy(dst, src, n);
来源：http://zgr.gaohongyu789.top

[S26] C：内存清零
来源：http://grf.yueranfly.top

memset(a, 0, sizeof a);
来源：http://caf.quarkkingdee.top

[S27] C：定义常量
来源：http://dqs.haohaochexian.top

const double PI = 3.14159;
来源：http://sgw.shanyushiyangtech.top

[S28] C：静态变量
来源：http://hdu.gzhubu.top

static int counter = 0;
来源：http://ewo.ehwqpu.com

[S29] C：变参函数
来源：http://kup.zhixingplan.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cbm.ppjwa.cn

[S30] C：头文件保护
来源：http://hlk.fengsongda.top

#ifndef X_H
来源：http://kyl.hnxiangtu.top

#define X_H
来源：http://qor.uphjek.com

#endif
来源：http://ice.316326.xyz

[S31] C++：Hello World
来源：http://pke.xinyue.icu

#include <iostream>
来源：http://qnh.quarkkingdee.top

int main() { std::cout << "Hello\n"; }
来源：http://fvu.xinyue.icu

[S32] C++：字符串
来源：http://acn.zhijiandao.cn

std::string s = "hi";  s += "!";
来源：http://ugv.epnwcf.com

[S33] C++：vector 增删
来源：http://zqk.zhengqikj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://okn.jyoumei.cn

[S34] C++：遍历 vector
来源：http://iok.havefunace.top

for (auto &x : v) { std::cout << x; }
来源：http://xdg.fengsongda.top

[S35] C++：map
来源：http://ewm.fehbvm.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uyz.hesvh.cn

[S36] C++：unordered_map
来源：http://whm.cashguo.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gta.vqdsnc.cn

[S37] C++：set
来源：http://bgk.zhijiandao.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nez.jiagoushi.top

[S38] C++：排序
来源：http://avf.jiagoushi.top

std::sort(v.begin(), v.end());
来源：http://xdz.quarkkingdee.top

[S39] C++：自定义比较器排序
来源：http://jwq.xinyue.icu

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fup.smart0.xyz

[S40] C++：查找元素
来源：http://tzn.sufxvd.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kdj.ctjpmb.com

[S41] C++：类与构造函数
来源：http://xyl.zhengqikj.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ucl.redwolf501.top

[S42] C++：继承与虚函数
来源：http://bgn.zycfv.cn

class B : public Base { public: void f() override {} };
来源：http://inz.pengpengdd.cyou

[S43] C++：智能指针
来源：http://ccf.sufxvd.cn

auto p = std::make_unique<int>(5);
来源：http://sra.xziqi.cn

[S44] C++：引用传参
来源：http://dth.shanyushiyangkeji.top

void inc(int &x) { ++x; }
来源：http://kvd.andypj.xyz

[S45] C++：lambda
来源：http://usa.fanxiaobao.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://cwh.wangshuangyany.cn

[S46] C++：函数模板
来源：http://dub.hnqzz.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tug.yvedp.cn

[S47] C++：结构化绑定遍历
来源：http://wld.yuanzhike.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jtw.nanxinkj.top

[S48] C++：逐行读文件
来源：http://spc.pycfn.com

std::ifstream in("a.txt");  std::string line;
来源：http://mmg.uphjek.com

while (std::getline(in, line)) { }
来源：http://gzg.fehbvm.com

[S49] C++：写文件
来源：http://qah.ydjk.org.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cay.birdmap.top

[S50] C++：格式化数字
来源：http://ktz.dashuyun.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bld.xinyue.icu

[S51] C++：显式类型转换
来源：http://rvg.mhx1999.top

static_cast<double>(a) / b
来源：http://hde.vehdjk.com

[S52] C++：const 与 noexcept
来源：http://udv.aibaodan.cn

int size() const noexcept { return n_; }
来源：http://fmb.jinghuilouyu.cn

[S53] C++：移动语义
来源：http://nhx.yvedp.cn

std::vector<int> w = std::move(v);
来源：http://qgs.xylfe.cn

[S54] C++：异常处理
来源：http://snr.tian-w.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lhr.svipenyu.cn

[S55] C++：结构化绑定
来源：http://mrj.yangfankeji.com

auto [a, b] = std::make_pair(1, 2);
来源：http://zzt.zdbjq.cn

[S56] C++：optional
来源：http://sob.yangfankeji.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ibn.jinyuanbaomall.cn

[S57] C++：编译期常量
来源：http://shs.cdnleiting.top

constexpr int N = 10;
来源：http://wpr.tianlin.xyz

[S58] C++：命名空间
来源：http://ywm.yangfankeji.com

namespace ns { int f() { return 1; } }
来源：http://oxb.sweek.top

[S59] C++：静态断言
来源：http://tni.bbcook.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mag.cucudq.cn

[S60] C++：遍历并删除元素
来源：http://dvb.nanxinkj.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qaq.nanxuanxn.top

================================================================================
来源：http://pip.316326.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jhw.sysykeji.top

================================================================================
来源：http://bkv.fehbvm.com

[T01] Kotlin：Hello World
来源：http://rca.zdqjudy.top

println("Hello")
来源：http://roa.quarkkingdee.top

[T02] Kotlin：变量
来源：http://fiw.fzhhl.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hwf.hfpthk.cn

[T03] Kotlin：字符串模板
来源：http://tqd.wangshuangyany.cn

"值: $b"
来源：http://ryv.kuanghao11.cn

[T04] Kotlin：空安全
来源：http://qrb.shuidangran.top

val n: String? = null;  n?.length
来源：http://qku.chenjidiqi.icu

[T05] Kotlin：when 表达式
来源：http://oct.birdmap.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://euu.xuetiantiany.cn

[T06] Kotlin：集合映射
来源：http://cmi.yuxming.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kxt.shzxlz.cn

[T07] Kotlin：集合过滤
来源：http://qsn.hnqzz.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mlv.hnxiangtu.top

[T08] Kotlin：数据类
来源：http://phu.meibo888.top

data class User(val name: String, val age: Int)
来源：http://lqg.jinghuilouyu.cn

[T09] Kotlin：扩展函数
来源：http://tdn.yueranfly.top

fun String.exclaim() = this + "!"
来源：http://ooh.guannengcc.top

[T10] Kotlin：默认参数
来源：http://ltz.feifeiyinyue.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ijc.shuidangran.top

[T11] Kotlin：协程
来源：http://hyu.epnwcf.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://owd.sweek.top

[T12] Kotlin：解构声明
来源：http://slx.ivvv.top

val (a, b) = Pair(1, 2)
来源：http://vvt.hfpthk.cn

[T13] Kotlin：只读 Map
来源：http://oog.hfpthk.cn

val m = mapOf("a" to 1)
来源：http://lls.vqdsnc.cn

[T14] Kotlin：循环
来源：http://apt.kuanghao11.cn

for (i in 1..10) println(i)
来源：http://zlj.fktsv.cn

[T15] Kotlin：接口
来源：http://ywj.jiagoushi.top

interface Shape { fun area(): Double }
来源：http://yod.tianlin.xyz

[T16] Swift：Hello World
来源：http://iyr.redwolf501.top

print("Hello")
来源：http://xkz.zdbjq.cn

[T17] Swift：变量与常量
来源：http://xxc.hesvh.cn

var a = 1;  let b = 2
来源：http://mhs.shuidangran.top

[T18] Swift：字符串插值
来源：http://xlc.hcnkem.com

"值: \(b)"
来源：http://sid.sysykeji.top

[T19] Swift：可选绑定
来源：http://wfn.c1oappe.top

if let n = opt { print(n) }
来源：http://ymr.mhx1999.top

[T20] Swift：数组操作
来源：http://vur.xinyue.icu

var a = [1, 2, 3];  a.append(4)
来源：http://pap.daxiang520.top

[T21] Swift：遍历
来源：http://lki.snrcjt.cn

for x in a { print(x) }
来源：http://kgr.bbcook.cn

[T22] Swift：字典
来源：http://tnb.jyoumei.cn

var d = ["a": 1];  d["b"] = 2
来源：http://slj.jlsjyb.cn

[T23] Swift：函数
来源：http://qwy.havefunace.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://azk.tian-w.cn

[T24] Swift：闭包
来源：http://rem.sxryk.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://esw.cashguo.top

[T25] Swift：结构体
来源：http://zdo.cdnleiting.top

struct P { var x: Int }
来源：http://sjo.mhx1999.top

[T26] Swift：类与重写
来源：http://cqp.sweek.top

class A: Base { override func f() {} }
来源：http://euk.cqqwz.cn

[T27] Swift：错误处理
来源：http://yxc.ydjk.org.cn

do { try f() } catch { print(error) }
来源：http://jcr.svipenyu.cn

[T28] Swift：枚举
来源：http://cjo.jinqigufen.top

enum Color { case red, green }
来源：http://ezi.yvedp.cn

[T29] Swift：guard 提前返回
来源：http://rcx.cheryme.top

guard let x = opt else { return }
来源：http://nlw.pengpengdd.cyou

[T30] Swift：协议
来源：http://rzr.yuxming.cn

protocol Shape { func area() -> Double }
来源：http://trr.zycfv.cn

[T31] Lua：Hello World
来源：http://iyt.nwbrower.top

print("Hello")
来源：http://too.cheryme.top

[T32] Lua：局部变量
来源：http://gpg.sjlbkw.cn

local a = 1
来源：http://uhz.bbcook.cn

[T33] Lua：表（数组）
来源：http://hfc.chenjidiqi.icu

local t = {1, 2, 3};  t[4] = 4
来源：http://cyk.nanxinkj.top

[T34] Lua：遍历表
来源：http://eji.yonumen.top

for i, v in ipairs(t) do print(i, v) end
来源：http://mcb.zhengqikj.top

[T35] Lua：字典表
来源：http://rbw.fengsongda.top

local d = { a = 1 };  d.b = 2
来源：http://szg.zhijiandao.cn

[T36] Lua：函数
来源：http://ucc.uphjek.com

function add(a, b) return a + b end
来源：http://mwz.gogol.net.cn

[T37] Lua：字符串拼接
来源：http://xgx.gotoacloud.top

"a" .. "b"
来源：http://rud.hongshengwenyu.top

[T38] Lua：条件
来源：http://iww.jianghu66.top

if x > 0 then print("正") end
来源：http://xks.shuidangran.top

[T39] Lua：模式匹配
来源：http://the.bjfxy.top

string.find(s, "%d+")
来源：http://nna.meibo888.top

[T40] Lua：元表
来源：http://beb.daria6918.cn

setmetatable({}, { __index = base })
来源：http://oxm.jianghu66.top

[T41] Perl：Hello World
来源：http://vxz.tianlin.xyz

print "Hello\n";
来源：http://eaz.yongpay.top

[T42] Perl：变量类型
来源：http://afo.yanxiufei.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bgn.hysaishi.cn

[T43] Perl：字符串插值
来源：http://hus.tian-w.cn

"值: $a"
来源：http://wpv.guannengcc.top

[T44] Perl：条件
来源：http://dxm.epnwcf.com

if ($a > 0) { print "正"; }
来源：http://drp.daxiang520.top

[T45] Perl：数组遍历
来源：http://hnx.ywan-chungtsiang.top

for my $x (@arr) { print $x; }
来源：http://tob.bjfxy.top

[T46] Perl：哈希操作
来源：http://rdq.shanyushiyangkeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uql.aizwys.cn

[T47] Perl：正则捕获
来源：http://lyf.wangdashe.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zfd.cucudq.cn

[T48] Perl：正则替换
来源：http://oxh.pycfn.com

$s =~ s/old/new/g;
来源：http://erf.cqqwz.cn

[T49] Perl：函数
来源：http://nbc.smart0.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://avy.xingfuxueyuan.xyz

[T50] Perl：逐行读文件
来源：http://bhc.gogol.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ews.ybcxt.top

while (my $line = <$fh>) { print $line; }
来源：http://bke.daxiang520.top

[T51] Scala：Hello World
来源：http://mzt.tarul.cn

println("Hello")
来源：http://mxq.shangyingyoupin.top

[T52] Scala：变量
来源：http://guu.zhixingplan.top

val a = 1;  var b = 2
来源：http://wkk.smart0.xyz

[T53] Scala：字符串插值
来源：http://eka.xinyue.icu

s"值: $b"
来源：http://nzm.hammf.cn

[T54] Scala：集合映射
来源：http://uvl.tian-w.cn

List(1, 2, 3).map(_ * 2)
来源：http://uxn.zhengqikj.top

[T55] Scala：集合过滤
来源：http://crs.chenzaomai.com

List(1, 2, 3).filter(_ > 1)
来源：http://vnr.shangyingyoupin.top

[T56] Scala：样例类
来源：http://grf.fktsv.cn

case class User(name: String, age: Int)
来源：http://vbx.cashguo.top

[T57] Scala：模式匹配
来源：http://lai.snrcjt.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nzq.hongshengwenyu.top

[T58] Scala：函数定义
来源：http://byf.hnqzz.top

def add(a: Int, b: Int): Int = a + b
来源：http://fdp.fehbvm.com

[T59] Scala：循环
来源：http://wlq.tianlin.xyz

for (i <- 1 to 10) println(i)
来源：http://tyz.redwolf501.top

[T60] Scala：折叠
来源：http://pmq.zhaomingkeji.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fnk.shanyushiyangtech.top

================================================================================
来源：http://fyj.zycfv.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vvx.zhongyouzk.top

================================================================================
来源：http://tpd.yongpay.top

[U01] Py：创建虚拟环境
来源：http://zgx.xuanzx.com

python -m venv .venv && source .venv/bin/activate
来源：http://udm.xingfuxueyuan.xyz

[U02] Py：导出 / 安装依赖
来源：http://wow.52xcode.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dbc.daria6918.cn

[U03] Py：加载 .env 配置
来源：http://dkr.jiagoushi.top

from dotenv import load_dotenv; load_dotenv()
来源：http://qyk.9152youxi.cn

[U04] Py：变量调试打印
来源：http://zkd.nanxuanxn.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ere.quarkkingdee.top

[U05] Py：列表去重且保序
来源：http://fmr.tian-w.cn

list(dict.fromkeys(arr))
来源：http://gwq.sufxvd.cn

[U06] Py：合并两个字典
来源：http://eoe.yuxming.cn

{**a, **b}
来源：http://kli.zhongyouzk.top

[U07] Py：反转字典键值
来源：http://voh.smart0.xyz

{v: k for k, v in d.items()}
来源：http://ija.ctjpmb.com

[U08] Py：展平二维列表
来源：http://kbs.ybcxt.top

[y for x in nested for y in x]
来源：http://lvu.ybcxt.top

[U09] Py：字典取最大值的键
来源：http://rct.cheryme.top

max(d, key=d.get)
来源：http://dno.yj202588.top

[U10] Py：按值排序字典
来源：http://bjm.yonumen.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rpi.fanxiaobao.xyz

[U11] Py：生成器表达式
来源：http://pif.tarul.cn

(x * 2 for x in arr)
来源：http://leg.nanxinkj.top

[U12] Py：取出现最多的 3 个元素
来源：http://cqt.9152youxi.cn

Counter(arr).most_common(3)
来源：http://mym.xuanzx.com


<!-- 参考信息 -->