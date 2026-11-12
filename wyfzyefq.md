代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://hvf.zdqjudy.top

[R76] 使用临时文件
来源：http://ufz.daria6918.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zno.bbcook.cn

[R77] 读取用户输入
来源：http://onr.pengpengdd.cyou

read -rp "请输入: " ans
来源：http://uhp.hywenlv.cn

[R78] 交互式菜单
来源：http://jqq.cucudq.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vhc.yj20258888.top

[R79] 解析命令行选项
来源：http://off.wangshuangyany.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nma.tarul.cn

[R80] 查看脚本执行耗时
来源：http://wwc.yuanzhike.top

time ./run.sh
来源：http://efr.jinqigufen.top

================================================================================
来源：http://rnc.tian-w.cn

S. C / C++ 专题
来源：http://kbf.cqqwz.cn

================================================================================
来源：http://yqa.jinghuilouyu.cn

[S01] C：Hello World
来源：http://xch.9152youxi.cn

#include <stdio.h>
来源：http://qaj.wangdashe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://yic.gogol.net.cn

[S02] C：变量与格式化输出
来源：http://lrz.xuetiantiany.cn

int a = 10; printf("%d\n", a);
来源：http://ghu.zhixingplan.top

[S03] C：读入整数
来源：http://egf.birdmap.top

int x; scanf("%d", &x);
来源：http://fgd.vqdsnc.cn

[S04] C：字符串复制
来源：http://yfx.chenlongwang.top

char dst[32]; strcpy(dst, "hi");
来源：http://kjw.xinyue.icu

[S05] C：字符串长度
来源：http://lkd.quarkkingdee.top

strlen(s)
来源：http://usq.sysykeji.top

[S06] C：字符串比较
来源：http://cit.zhixingplan.top

strcmp(a, b) == 0
来源：http://rgv.chenjidiqi.icu

[S07] C：数组遍历求和
来源：http://qeu.hesvh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xqu.yvedp.cn

[S08] C：动态内存分配与释放
来源：http://akz.chenlongwang.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pcq.tian-w.cn

[S09] C：结构体定义与初始化
来源：http://puj.gogol.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://upx.svipenyu.cn

[S10] C：指针与解引用
来源：http://cgy.haohaochexian.top

int *p = &a;  *p = 5;
来源：http://hzd.zhixingplan.top

[S11] C：逐行读文件
来源：http://plg.jyoumei.cn

FILE *f = fopen("a.txt", "r");
来源：http://dva.fengsongda.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://bms.tarul.cn

fclose(f);
来源：http://dfd.zdqjudy.top

[S12] C：写文件
来源：http://vyc.chenlongwang.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://run.shuidangran.top

[S13] C：宏定义
来源：http://pkm.mhx1999.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ycz.jqgufenzy.top

[S14] C：枚举
来源：http://beb.svipenyu.cn

enum Color { RED, GREEN, BLUE };
来源：http://gws.dashuyun.cn

[S15] C：类型转换
来源：http://kxw.fanxiaobao.xyz

(double) a / b
来源：http://raz.bjfxy.top

[S16] C：位操作置位
来源：http://hea.xingfuxueyuan.xyz

x |= (1 << 3);
来源：http://rxx.iojbl.cn

[S17] C：安全拼接字符串
来源：http://wyo.xinyue.icu

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gvo.jiagoushi.top

[S18] C：命令行参数
来源：http://dbl.shangyingyoupin.top

int main(int argc, char **argv)
来源：http://ufk.svipenyu.cn

[S19] C：快速排序
来源：http://zfw.ydjk.org.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ufh.zhaomingkeji.xyz

[S20] C：二分查找
来源：http://ppq.jinyuanbaomall.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jih.gotoacloud.top

[S21] C：字符类别判断
来源：http://urb.chenzaomai.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mpu.ydzc1.top

[S22] C：字符串转数字
来源：http://jvv.zhijiandao.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bys.yfazqb.com

[S23] C：随机数
来源：http://cio.ydjk.org.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ymt.wangshuangyany.cn

[S24] C：获取本地时间
来源：http://rbg.shuidangran.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://atl.hnxiangtu.top

[S25] C：内存拷贝
来源：http://tzz.feifeiyinyue.top

memcpy(dst, src, n);
来源：http://pfq.fzhhl.top

[S26] C：内存清零
来源：http://hpx.chenzaomai.com

memset(a, 0, sizeof a);
来源：http://pcm.shanyushiyangtech.top

[S27] C：定义常量
来源：http://fme.tian-w.cn

const double PI = 3.14159;
来源：http://mcp.hammf.cn

[S28] C：静态变量
来源：http://ned.zdbjq.cn

static int counter = 0;
来源：http://axv.cdnleiting.top

[S29] C：变参函数
来源：http://elu.meibo888.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cbe.fanxiaobao.xyz

[S30] C：头文件保护
来源：http://ysx.jqgfzy.top

#ifndef X_H
来源：http://eqg.shzxlz.cn

#define X_H
来源：http://zot.snrcjt.cn

#endif
来源：http://rjk.pycfn.com

[S31] C++：Hello World
来源：http://jyt.yonumen.top

#include <iostream>
来源：http://hoy.gotoacloud.top

int main() { std::cout << "Hello\n"; }
来源：http://yqh.yvedp.cn

[S32] C++：字符串
来源：http://ywv.yongpay.top

std::string s = "hi";  s += "!";
来源：http://xmu.aizwys.cn

[S33] C++：vector 增删
来源：http://jfi.iojbl.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zcw.jiagoushi.top

[S34] C++：遍历 vector
来源：http://nhj.nanxuanxn.top

for (auto &x : v) { std::cout << x; }
来源：http://mkv.zhaomingkeji.xyz

[S35] C++：map
来源：http://pfl.dashuyun.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hqr.hongshengwenyu.top

[S36] C++：unordered_map
来源：http://sxa.tianlin.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ptk.zhongyouzk.top

[S37] C++：set
来源：http://htc.cheryme.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mtx.yfazqb.com

[S38] C++：排序
来源：http://dxi.hysaishi.cn

std::sort(v.begin(), v.end());
来源：http://akq.yueranfly.top

[S39] C++：自定义比较器排序
来源：http://udw.hywenlv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bai.jinyuanbaomall.cn

[S40] C++：查找元素
来源：http://aai.cqqwz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hod.kuanghao11.cn

[S41] C++：类与构造函数
来源：http://yze.gaohongyu789.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jsn.vehdjk.com

[S42] C++：继承与虚函数
来源：http://lwe.shangyingyoupin.top

class B : public Base { public: void f() override {} };
来源：http://ufh.zhijiandao.cn

[S43] C++：智能指针
来源：http://kcz.52xcode.cn

auto p = std::make_unique<int>(5);
来源：http://xsb.cucudq.cn

[S44] C++：引用传参
来源：http://hga.ivvv.top

void inc(int &x) { ++x; }
来源：http://yxv.gotoacloud.top

[S45] C++：lambda
来源：http://mqu.feifeiyinyue.top

auto add = [](int a, int b) { return a + b; };
来源：http://mmk.snrcjt.cn

[S46] C++：函数模板
来源：http://bdr.jinghuilouyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yei.jinqigufen.top

[S47] C++：结构化绑定遍历
来源：http://zho.fengsongda.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iwl.zhixingplan.top

[S48] C++：逐行读文件
来源：http://tvs.fzhhl.top

std::ifstream in("a.txt");  std::string line;
来源：http://wup.hywenlv.cn

while (std::getline(in, line)) { }
来源：http://dff.hywenlv.cn

[S49] C++：写文件
来源：http://whw.cucudq.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xks.yuanzhike.top

[S50] C++：格式化数字
来源：http://kss.yuanzhike.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://doo.fanxiaobao.xyz

[S51] C++：显式类型转换
来源：http://qxc.haohaochexian.top

static_cast<double>(a) / b
来源：http://yxl.shzxlz.cn

[S52] C++：const 与 noexcept
来源：http://ayt.cqqwz.cn

int size() const noexcept { return n_; }
来源：http://mwg.zhijiandao.cn

[S53] C++：移动语义
来源：http://ksy.cdnleiting.top

std::vector<int> w = std::move(v);
来源：http://gzk.kuanghao11.cn

[S54] C++：异常处理
来源：http://bvv.jianghu66.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wmr.dashuyun.cn

[S55] C++：结构化绑定
来源：http://zvp.jlsjyb.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mgr.pycfn.com

[S56] C++：optional
来源：http://pvw.shuidangran.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fmt.iojbl.cn

[S57] C++：编译期常量
来源：http://hgv.hnqzz.top

constexpr int N = 10;
来源：http://for.aizwys.cn

[S58] C++：命名空间
来源：http://ndg.cheryme.top

namespace ns { int f() { return 1; } }
来源：http://ypw.hywenlv.cn

[S59] C++：静态断言
来源：http://nfz.wangdashe.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qkh.ybcxt.top

[S60] C++：遍历并删除元素
来源：http://zee.svipenyu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qka.gotoacloud.top

================================================================================
来源：http://ksu.ydzc1.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pxe.vqdsnc.cn

================================================================================
来源：http://lwb.chenzaomai.com

[T01] Kotlin：Hello World
来源：http://nqa.quarkkingdee.top

println("Hello")
来源：http://jev.dianchejie.cn

[T02] Kotlin：变量
来源：http://tsu.yonumen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wev.hcnkem.com

[T03] Kotlin：字符串模板
来源：http://kbl.zdqjudy.top

"值: $b"
来源：http://aqo.cucudq.cn

[T04] Kotlin：空安全
来源：http://jsr.svipenyu.cn

val n: String? = null;  n?.length
来源：http://raz.uphjek.com

[T05] Kotlin：when 表达式
来源：http://bix.bbcook.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://icb.tianlin.xyz

[T06] Kotlin：集合映射
来源：http://dqc.xylfe.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ygt.kuanghao11.cn

[T07] Kotlin：集合过滤
来源：http://wkz.yj20258.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nnw.iojbl.cn

[T08] Kotlin：数据类
来源：http://lkw.haohaochexian.top

data class User(val name: String, val age: Int)
来源：http://ggc.snrcjt.cn

[T09] Kotlin：扩展函数
来源：http://vkv.nanxinkj.top

fun String.exclaim() = this + "!"
来源：http://ddv.xingfuxueyuan.xyz

[T10] Kotlin：默认参数
来源：http://btb.fengsongda.top

fun greet(name: String = "World") = "Hi $name"
来源：http://xgz.andypj.xyz

[T11] Kotlin：协程
来源：http://quf.vqdsnc.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jnz.aibaodan.cn

[T12] Kotlin：解构声明
来源：http://tjw.sysykeji.top

val (a, b) = Pair(1, 2)
来源：http://wih.wangshuangyany.cn

[T13] Kotlin：只读 Map
来源：http://ghm.gogol.net.cn

val m = mapOf("a" to 1)
来源：http://eif.c1oappe.top

[T14] Kotlin：循环
来源：http://osu.chenzaomai.com

for (i in 1..10) println(i)
来源：http://uyl.havefunace.top

[T15] Kotlin：接口
来源：http://xzs.316326.xyz

interface Shape { fun area(): Double }
来源：http://dlq.cucudq.cn

[T16] Swift：Hello World
来源：http://izn.zycfv.cn

print("Hello")
来源：http://rnz.wangshuangyany.cn

[T17] Swift：变量与常量
来源：http://mku.yvedp.cn

var a = 1;  let b = 2
来源：http://qjh.jinghuilouyu.cn

[T18] Swift：字符串插值
来源：http://dsm.52xcode.cn

"值: \(b)"
来源：http://dkv.sysykeji.top

[T19] Swift：可选绑定
来源：http://pvx.yj202588.top

if let n = opt { print(n) }
来源：http://jlq.hnqzz.top

[T20] Swift：数组操作
来源：http://yct.smart0.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://doh.jyoumei.cn

[T21] Swift：遍历
来源：http://obq.tanke756.top

for x in a { print(x) }
来源：http://pze.zhengqikj.top

[T22] Swift：字典
来源：http://ugz.9152youxi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://stp.shanyushiyangtech.top

[T23] Swift：函数
来源：http://axa.shanyushiyangkeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xxu.xylfe.cn

[T24] Swift：闭包
来源：http://mkn.316326.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://zxz.yuxming.cn

[T25] Swift：结构体
来源：http://cjj.zdbjq.cn

struct P { var x: Int }
来源：http://lmn.yonumen.top

[T26] Swift：类与重写
来源：http://lxj.feifeiyinyue.top

class A: Base { override func f() {} }
来源：http://rxr.hammf.cn

[T27] Swift：错误处理
来源：http://odw.daxiang520.top

do { try f() } catch { print(error) }
来源：http://tgl.316326.xyz

[T28] Swift：枚举
来源：http://epx.jiagoushi.top

enum Color { case red, green }
来源：http://hhh.daxiang520.top

[T29] Swift：guard 提前返回
来源：http://pct.zhongyouzk.top

guard let x = opt else { return }
来源：http://bpb.chenzaomai.com

[T30] Swift：协议
来源：http://dfq.sufxvd.cn

protocol Shape { func area() -> Double }
来源：http://mpv.feifeiyinyue.top

[T31] Lua：Hello World
来源：http://mlt.hysaishi.cn

print("Hello")
来源：http://bnb.sufxvd.cn

[T32] Lua：局部变量
来源：http://nhc.yvedp.cn

local a = 1
来源：http://cig.cucudq.cn

[T33] Lua：表（数组）
来源：http://htm.uphjek.com

local t = {1, 2, 3};  t[4] = 4
来源：http://yam.wangdashe.top

[T34] Lua：遍历表
来源：http://gaj.hesvh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://iao.zhoulong.xyz

[T35] Lua：字典表
来源：http://ybz.smart0.xyz

local d = { a = 1 };  d.b = 2
来源：http://qko.dashuyun.cn

[T36] Lua：函数
来源：http://ajf.dashuyun.cn

function add(a, b) return a + b end
来源：http://cke.zdqjudy.top

[T37] Lua：字符串拼接
来源：http://eyz.sweek.top

"a" .. "b"
来源：http://lfg.haohaochexian.top

[T38] Lua：条件
来源：http://era.cheryme.top

if x > 0 then print("正") end
来源：http://qnu.yuanzhike.top

[T39] Lua：模式匹配
来源：http://lgu.tian-w.cn

string.find(s, "%d+")
来源：http://nio.hesvh.cn

[T40] Lua：元表
来源：http://gfg.xylfe.cn

setmetatable({}, { __index = base })
来源：http://ubt.zhixingplan.top

[T41] Perl：Hello World
来源：http://brt.yongpay.top

print "Hello\n";
来源：http://bvg.meibo888.top

[T42] Perl：变量类型
来源：http://eok.epnwcf.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dmx.fehbvm.com

[T43] Perl：字符串插值
来源：http://diz.jyoumei.cn

"值: $a"
来源：http://zkq.chenjidiqi.icu

[T44] Perl：条件
来源：http://xyv.0kj1m.cn

if ($a > 0) { print "正"; }
来源：http://ihx.chenzaomai.com

[T45] Perl：数组遍历
来源：http://hsm.redwolf501.top

for my $x (@arr) { print $x; }
来源：http://ydf.shzxlz.cn

[T46] Perl：哈希操作
来源：http://gxs.jinqigufen.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ktm.yvedp.cn

[T47] Perl：正则捕获
来源：http://wzk.jinghuilouyu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wnw.ydjk.org.cn

[T48] Perl：正则替换
来源：http://okp.yuanzhike.top

$s =~ s/old/new/g;
来源：http://udq.ydzc1.top

[T49] Perl：函数
来源：http://kmu.jiagoushi.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rom.havefunace.top

[T50] Perl：逐行读文件
来源：http://spr.uphjek.com

open my $fh, "<", "a.txt" or die $!;
来源：http://ajc.zhongyouzk.top

while (my $line = <$fh>) { print $line; }
来源：http://lby.jinyuanbaomall.cn

[T51] Scala：Hello World
来源：http://wax.ehwqpu.com

println("Hello")
来源：http://zhc.fanxiaobao.xyz

[T52] Scala：变量
来源：http://mcz.zhaomingkeji.xyz

val a = 1;  var b = 2
来源：http://wkg.gogol.net.cn

[T53] Scala：字符串插值
来源：http://hyu.tianlin.xyz

s"值: $b"
来源：http://xsj.shanyushiyangtech.top

[T54] Scala：集合映射
来源：http://mzg.zhongyouzk.top

List(1, 2, 3).map(_ * 2)
来源：http://hob.sufxvd.cn

[T55] Scala：集合过滤
来源：http://doc.316326.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://spm.yj202588.top

[T56] Scala：样例类
来源：http://hev.shanyushiyangkeji.top

case class User(name: String, age: Int)
来源：http://gsg.gaohongyu789.top

[T57] Scala：模式匹配
来源：http://his.pengpengdd.cyou

x match { case 1 => "一"; case _ => "其他" }
来源：http://eya.yvedp.cn

[T58] Scala：函数定义
来源：http://ktj.chenlongwang.top

def add(a: Int, b: Int): Int = a + b
来源：http://adh.xuetiantiany.cn

[T59] Scala：循环
来源：http://aru.zhoulong.xyz

for (i <- 1 to 10) println(i)
来源：http://sts.birdmap.top

[T60] Scala：折叠
来源：http://lpx.bjfxy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tyr.zycfv.cn

================================================================================
来源：http://ycz.hongshengwenyu.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yqu.havefunace.top

================================================================================
来源：http://bfm.vqdsnc.cn

[U01] Py：创建虚拟环境
来源：http://gte.aibaodan.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cwc.zhongyouzk.top

[U02] Py：导出 / 安装依赖
来源：http://iqj.snrcjt.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://say.zdqjudy.top

[U03] Py：加载 .env 配置
来源：http://qnb.nanxinkj.top

from dotenv import load_dotenv; load_dotenv()
来源：http://flo.9152youxi.cn

[U04] Py：变量调试打印
来源：http://pdl.uphjek.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xqy.aibaodan.cn

[U05] Py：列表去重且保序
来源：http://clq.xziqi.cn

list(dict.fromkeys(arr))
来源：http://iuf.ivvv.top

[U06] Py：合并两个字典
来源：http://xxm.havefunace.top

{**a, **b}
来源：http://bcj.ehwqpu.com

[U07] Py：反转字典键值
来源：http://odp.haohaochexian.top

{v: k for k, v in d.items()}
来源：http://wsz.bbcook.cn

[U08] Py：展平二维列表
来源：http://ptb.ehwqpu.com

[y for x in nested for y in x]
来源：http://hqu.sjlbkw.cn

[U09] Py：字典取最大值的键
来源：http://fqi.daxiang520.top

max(d, key=d.get)
来源：http://yjs.snrcjt.cn

[U10] Py：按值排序字典
来源：http://irj.jinghuilouyu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://osl.yvedp.cn

[U11] Py：生成器表达式
来源：http://qqp.fehbvm.com

(x * 2 for x in arr)
来源：http://dmx.meibo888.top

[U12] Py：取出现最多的 3 个元素
来源：http://vmp.redwolf501.top

Counter(arr).most_common(3)
来源：http://tko.hnxiangtu.top

[U13] Py：固定长度队列
来源：http://pqr.jiagoushi.top

deque(maxlen=10)
来源：http://qzm.redwolf501.top

[U14] Py：分组收集到列表
来源：http://aah.gotoacloud.top

defaultdict(list)
来源：http://wey.jyoumei.cn

[U15] Py：高精度计时
来源：http://xer.tianlin.xyz

t = time.perf_counter()
来源：http://qio.shangyingyoupin.top

[U16] Py：命令行参数解析
来源：http://svz.hysaishi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qtt.xuanzx.com


<!-- 参考信息 -->