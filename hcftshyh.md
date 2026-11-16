代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://hiq.shzxlz.cn

[R76] 使用临时文件
来源：http://wzb.ydjk.org.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eoz.yvedp.cn

[R77] 读取用户输入
来源：http://jej.zhongyouzk.top

read -rp "请输入: " ans
来源：http://mta.sjlbkw.cn

[R78] 交互式菜单
来源：http://mxf.fzhhl.top

select opt in a b c; do echo "$opt"; break; done
来源：http://nzy.fanxiaobao.xyz

[R79] 解析命令行选项
来源：http://smt.sweek.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://aci.zhongyouzk.top

[R80] 查看脚本执行耗时
来源：http://vvk.shanyushiyangkeji.top

time ./run.sh
来源：http://ogr.zdbjq.cn

================================================================================
来源：http://tza.jiagoushi.top

S. C / C++ 专题
来源：http://hjd.ydjk.org.cn

================================================================================
来源：http://vcd.tianlin.xyz

[S01] C：Hello World
来源：http://xny.hywenlv.cn

#include <stdio.h>
来源：http://rbr.gaohongyu789.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://snp.pycfn.com

[S02] C：变量与格式化输出
来源：http://oxl.yueranfly.top

int a = 10; printf("%d\n", a);
来源：http://uuc.ydzc1.top

[S03] C：读入整数
来源：http://fpf.nanxinkj.top

int x; scanf("%d", &x);
来源：http://hgg.aibaodan.cn

[S04] C：字符串复制
来源：http://ira.chenzaomai.com

char dst[32]; strcpy(dst, "hi");
来源：http://bxe.fengsongda.top

[S05] C：字符串长度
来源：http://ddl.shanyushiyangtech.top

strlen(s)
来源：http://khm.ywan-chungtsiang.top

[S06] C：字符串比较
来源：http://jsq.shanyushiyangtech.top

strcmp(a, b) == 0
来源：http://ixq.jinghuilouyu.cn

[S07] C：数组遍历求和
来源：http://oww.chenlongwang.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zbl.yueranfly.top

[S08] C：动态内存分配与释放
来源：http://yiv.xylfe.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lcb.tianlin.xyz

[S09] C：结构体定义与初始化
来源：http://dfh.xingfuxueyuan.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bcp.fengsongda.top

[S10] C：指针与解引用
来源：http://ewo.xziqi.cn

int *p = &a;  *p = 5;
来源：http://rdo.hongshengwenyu.top

[S11] C：逐行读文件
来源：http://xae.vqdsnc.cn

FILE *f = fopen("a.txt", "r");
来源：http://ciz.epnwcf.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://yge.epnwcf.com

fclose(f);
来源：http://lfn.xingfuxueyuan.xyz

[S12] C：写文件
来源：http://moh.jiagoushi.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dio.sufxvd.cn

[S13] C：宏定义
来源：http://xfb.fengsongda.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hyv.yongpay.top

[S14] C：枚举
来源：http://ltg.shanyushiyangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://iou.aibaodan.cn

[S15] C：类型转换
来源：http://ghb.ywan-chungtsiang.top

(double) a / b
来源：http://qqn.haohaochexian.top

[S16] C：位操作置位
来源：http://xvg.yongpay.top

x |= (1 << 3);
来源：http://nfj.havefunace.top

[S17] C：安全拼接字符串
来源：http://rho.cdnleiting.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tps.nanxuanxn.top

[S18] C：命令行参数
来源：http://dqz.xingfuxueyuan.xyz

int main(int argc, char **argv)
来源：http://ryp.jqgfzy.top

[S19] C：快速排序
来源：http://arq.yvedp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xuo.ywan-chungtsiang.top

[S20] C：二分查找
来源：http://mat.0kj1m.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pyb.zhijiandao.cn

[S21] C：字符类别判断
来源：http://fth.jianghu66.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cgi.wangshuangyany.cn

[S22] C：字符串转数字
来源：http://wij.xuetiantiany.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gto.quarkkingdee.top

[S23] C：随机数
来源：http://iiq.c1oappe.top

srand(time(NULL));  int r = rand() % 100;
来源：http://wlu.dashuyun.cn

[S24] C：获取本地时间
来源：http://awo.pycfn.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pxo.mhx1999.top

[S25] C：内存拷贝
来源：http://peq.meibo888.top

memcpy(dst, src, n);
来源：http://anx.yuanzhike.top

[S26] C：内存清零
来源：http://byy.52xcode.cn

memset(a, 0, sizeof a);
来源：http://nmp.jqgufenzy.top

[S27] C：定义常量
来源：http://cvq.cqqwz.cn

const double PI = 3.14159;
来源：http://zjl.jqgfzy.top

[S28] C：静态变量
来源：http://ind.daxiang520.top

static int counter = 0;
来源：http://jcz.pengpengdd.cyou

[S29] C：变参函数
来源：http://dow.yuanzhike.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nhz.cucudq.cn

[S30] C：头文件保护
来源：http://phy.gogol.net.cn

#ifndef X_H
来源：http://rqr.zdbjq.cn

#define X_H
来源：http://xef.ctjpmb.com

#endif
来源：http://zgv.zhaomingkeji.xyz

[S31] C++：Hello World
来源：http://ltl.daxiang520.top

#include <iostream>
来源：http://pqn.cqqwz.cn

int main() { std::cout << "Hello\n"; }
来源：http://pli.zdqjudy.top

[S32] C++：字符串
来源：http://yej.ehwqpu.com

std::string s = "hi";  s += "!";
来源：http://qqp.xuetiantiany.cn

[S33] C++：vector 增删
来源：http://goh.jinqigufen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kzp.tarul.cn

[S34] C++：遍历 vector
来源：http://dxo.xingfuxueyuan.xyz

for (auto &x : v) { std::cout << x; }
来源：http://ahj.zhongyouzk.top

[S35] C++：map
来源：http://scv.ybcxt.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jyr.zhijiandao.cn

[S36] C++：unordered_map
来源：http://gsb.daria6918.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bgy.ydzc1.top

[S37] C++：set
来源：http://fdg.tianlin.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qlz.hfpthk.cn

[S38] C++：排序
来源：http://uvz.uphjek.com

std::sort(v.begin(), v.end());
来源：http://zne.shangyingyoupin.top

[S39] C++：自定义比较器排序
来源：http://xie.tian-w.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bgx.ydzc1.top

[S40] C++：查找元素
来源：http://jct.yvedp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gzm.vehdjk.com

[S41] C++：类与构造函数
来源：http://dxt.havefunace.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://znw.hesvh.cn

[S42] C++：继承与虚函数
来源：http://ogc.zhijiandao.cn

class B : public Base { public: void f() override {} };
来源：http://ahm.xinyue.icu

[S43] C++：智能指针
来源：http://fbp.jqgufenzy.top

auto p = std::make_unique<int>(5);
来源：http://aqo.nanxinkj.top

[S44] C++：引用传参
来源：http://bcm.jinyuanbaomall.cn

void inc(int &x) { ++x; }
来源：http://lms.svipenyu.cn

[S45] C++：lambda
来源：http://via.zhoulong.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://dyo.sxryk.cn

[S46] C++：函数模板
来源：http://phe.xuanzx.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fwy.fanxiaobao.xyz

[S47] C++：结构化绑定遍历
来源：http://cwp.yueranfly.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gtp.316326.xyz

[S48] C++：逐行读文件
来源：http://fin.zycfv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kps.jlsjyb.cn

while (std::getline(in, line)) { }
来源：http://deg.daria6918.cn

[S49] C++：写文件
来源：http://rez.smart0.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ada.ctjpmb.com

[S50] C++：格式化数字
来源：http://cjt.shangyingyoupin.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xye.quarkkingdee.top

[S51] C++：显式类型转换
来源：http://yss.wangdashe.top

static_cast<double>(a) / b
来源：http://llg.ydjk.org.cn

[S52] C++：const 与 noexcept
来源：http://npe.fzhhl.top

int size() const noexcept { return n_; }
来源：http://ynw.tanke756.top

[S53] C++：移动语义
来源：http://qrx.fengsongda.top

std::vector<int> w = std::move(v);
来源：http://evs.wangshuangyany.cn

[S54] C++：异常处理
来源：http://lqp.wangdashe.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://peu.shuidangran.top

[S55] C++：结构化绑定
来源：http://rgt.zdbjq.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jug.zhoulong.xyz

[S56] C++：optional
来源：http://gdk.xziqi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ccu.zhoulong.xyz

[S57] C++：编译期常量
来源：http://xro.jinqigufen.top

constexpr int N = 10;
来源：http://ixa.xziqi.cn

[S58] C++：命名空间
来源：http://yml.guowangkeji.top

namespace ns { int f() { return 1; } }
来源：http://cmn.pycfn.com

[S59] C++：静态断言
来源：http://pti.shzxlz.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hzv.sxryk.cn

[S60] C++：遍历并删除元素
来源：http://xsa.yangfankeji.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jwu.ppjwa.cn

================================================================================
来源：http://cpm.jinyuanbaomall.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iou.yj202588.top

================================================================================
来源：http://pmp.yanxiufei.cn

[T01] Kotlin：Hello World
来源：http://odn.pengpengdd.cyou

println("Hello")
来源：http://lka.gotoacloud.top

[T02] Kotlin：变量
来源：http://had.ctjpmb.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://twy.zhengqikj.top

[T03] Kotlin：字符串模板
来源：http://ych.daxiang520.top

"值: $b"
来源：http://oyg.gzhubu.top

[T04] Kotlin：空安全
来源：http://gws.jyoumei.cn

val n: String? = null;  n?.length
来源：http://tsz.shangyingyoupin.top

[T05] Kotlin：when 表达式
来源：http://sak.zycfv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hrn.sufxvd.cn

[T06] Kotlin：集合映射
来源：http://dsi.cheryme.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ltt.yonumen.top

[T07] Kotlin：集合过滤
来源：http://zmb.gzhubu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kph.0kj1m.cn

[T08] Kotlin：数据类
来源：http://xkj.hfpthk.cn

data class User(val name: String, val age: Int)
来源：http://rux.hammf.cn

[T09] Kotlin：扩展函数
来源：http://gzf.xziqi.cn

fun String.exclaim() = this + "!"
来源：http://hgj.wangshuangyany.cn

[T10] Kotlin：默认参数
来源：http://iai.0kj1m.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://prc.iojbl.cn

[T11] Kotlin：协程
来源：http://sse.chenjidiqi.icu

GlobalScope.launch { delay(1000); println("done") }
来源：http://ocv.sjlbkw.cn

[T12] Kotlin：解构声明
来源：http://sap.0kj1m.cn

val (a, b) = Pair(1, 2)
来源：http://daw.tanke756.top

[T13] Kotlin：只读 Map
来源：http://zxa.pengpengdd.cyou

val m = mapOf("a" to 1)
来源：http://mzn.dashuyun.cn

[T14] Kotlin：循环
来源：http://agj.zhixingplan.top

for (i in 1..10) println(i)
来源：http://xcf.jinqigufen.top

[T15] Kotlin：接口
来源：http://mfr.vehdjk.com

interface Shape { fun area(): Double }
来源：http://cnb.chenjidiqi.icu

[T16] Swift：Hello World
来源：http://qyo.zhengqikj.top

print("Hello")
来源：http://ltq.yj202588.top

[T17] Swift：变量与常量
来源：http://vxh.cqqwz.cn

var a = 1;  let b = 2
来源：http://pzu.zhiwuduotai.top

[T18] Swift：字符串插值
来源：http://kwn.hywenlv.cn

"值: \(b)"
来源：http://kfx.ppjwa.cn

[T19] Swift：可选绑定
来源：http://gll.zhixingplan.top

if let n = opt { print(n) }
来源：http://kkh.birdmap.top

[T20] Swift：数组操作
来源：http://qju.guowangkeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://wbm.chenjidiqi.icu

[T21] Swift：遍历
来源：http://yjx.feifeiyinyue.top

for x in a { print(x) }
来源：http://ozw.shuidangran.top

[T22] Swift：字典
来源：http://hpi.zhiwuduotai.top

var d = ["a": 1];  d["b"] = 2
来源：http://muj.shuidangran.top

[T23] Swift：函数
来源：http://kls.jinyuanbaomall.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gog.xuetiantiany.cn

[T24] Swift：闭包
来源：http://jsp.tianlin.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://sdu.sysykeji.top

[T25] Swift：结构体
来源：http://fnr.fanxiaobao.xyz

struct P { var x: Int }
来源：http://okd.pengpengdd.cyou

[T26] Swift：类与重写
来源：http://atz.yongpay.top

class A: Base { override func f() {} }
来源：http://luv.sjlbkw.cn

[T27] Swift：错误处理
来源：http://yfy.shzxlz.cn

do { try f() } catch { print(error) }
来源：http://rwj.vehdjk.com

[T28] Swift：枚举
来源：http://fzx.pycfn.com

enum Color { case red, green }
来源：http://vym.daxiang520.top

[T29] Swift：guard 提前返回
来源：http://ylh.uphjek.com

guard let x = opt else { return }
来源：http://slo.jlsjyb.cn

[T30] Swift：协议
来源：http://tbt.shzxlz.cn

protocol Shape { func area() -> Double }
来源：http://jqm.xuanzx.com

[T31] Lua：Hello World
来源：http://inu.ydjk.org.cn

print("Hello")
来源：http://qyo.svipenyu.cn

[T32] Lua：局部变量
来源：http://wft.jqgufenzy.top

local a = 1
来源：http://fhg.tianlin.xyz

[T33] Lua：表（数组）
来源：http://jqq.feifeiyinyue.top

local t = {1, 2, 3};  t[4] = 4
来源：http://dnj.sjlbkw.cn

[T34] Lua：遍历表
来源：http://lrj.svipenyu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://acm.vqdsnc.cn

[T35] Lua：字典表
来源：http://nvd.ivvv.top

local d = { a = 1 };  d.b = 2
来源：http://zyf.zhengqikj.top

[T36] Lua：函数
来源：http://sbj.guowangkeji.top

function add(a, b) return a + b end
来源：http://nyz.mhx1999.top

[T37] Lua：字符串拼接
来源：http://qst.shanyushiyangtech.top

"a" .. "b"
来源：http://zew.fengsongda.top

[T38] Lua：条件
来源：http://jwy.sysykeji.top

if x > 0 then print("正") end
来源：http://jyd.dashuyun.cn

[T39] Lua：模式匹配
来源：http://vzj.chenzaomai.com

string.find(s, "%d+")
来源：http://qol.316326.xyz

[T40] Lua：元表
来源：http://hxu.ydzc1.top

setmetatable({}, { __index = base })
来源：http://ghi.yvedp.cn

[T41] Perl：Hello World
来源：http://wcl.dashuyun.cn

print "Hello\n";
来源：http://ifm.bjfxy.top

[T42] Perl：变量类型
来源：http://ail.xylfe.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dht.jianghu66.top

[T43] Perl：字符串插值
来源：http://dfw.sjlbkw.cn

"值: $a"
来源：http://mrc.xziqi.cn

[T44] Perl：条件
来源：http://woe.sweek.top

if ($a > 0) { print "正"; }
来源：http://uhy.sufxvd.cn

[T45] Perl：数组遍历
来源：http://xzs.zhixingplan.top

for my $x (@arr) { print $x; }
来源：http://ntp.wangshuangyany.cn

[T46] Perl：哈希操作
来源：http://efh.ehwqpu.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pds.zhoulong.xyz

[T47] Perl：正则捕获
来源：http://tys.hammf.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nkt.tarul.cn

[T48] Perl：正则替换
来源：http://wof.gotoacloud.top

$s =~ s/old/new/g;
来源：http://ikb.sysykeji.top

[T49] Perl：函数
来源：http://oms.yanxiufei.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vis.jiagoushi.top

[T50] Perl：逐行读文件
来源：http://ipv.yj20258.top

open my $fh, "<", "a.txt" or die $!;
来源：http://rxl.jiagoushi.top

while (my $line = <$fh>) { print $line; }
来源：http://lpe.pengpengdd.cyou

[T51] Scala：Hello World
来源：http://etc.daxiang520.top

println("Hello")
来源：http://iqc.jinqigufen.top

[T52] Scala：变量
来源：http://krw.yangfankeji.com

val a = 1;  var b = 2
来源：http://qlc.hcnkem.com

[T53] Scala：字符串插值
来源：http://euq.zhengqikj.top

s"值: $b"
来源：http://iex.ehwqpu.com

[T54] Scala：集合映射
来源：http://zic.bbcook.cn

List(1, 2, 3).map(_ * 2)
来源：http://hjz.zhaomingkeji.xyz

[T55] Scala：集合过滤
来源：http://wvb.quarkkingdee.top

List(1, 2, 3).filter(_ > 1)
来源：http://lal.yvedp.cn

[T56] Scala：样例类
来源：http://qyo.wangshuangyany.cn

case class User(name: String, age: Int)
来源：http://avo.svipenyu.cn

[T57] Scala：模式匹配
来源：http://sfe.zhijiandao.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ssh.ydjk.org.cn

[T58] Scala：函数定义
来源：http://hcb.xingfuxueyuan.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://muf.gogol.net.cn

[T59] Scala：循环
来源：http://zlj.chenjidiqi.icu

for (i <- 1 to 10) println(i)
来源：http://scp.shzxlz.cn

[T60] Scala：折叠
来源：http://ehd.jinghuilouyu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yjm.hnxiangtu.top

================================================================================
来源：http://syw.316326.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xqe.yanxiufei.cn

================================================================================
来源：http://xwo.feifeiyinyue.top

[U01] Py：创建虚拟环境
来源：http://sug.yfazqb.com

python -m venv .venv && source .venv/bin/activate
来源：http://kau.hesvh.cn

[U02] Py：导出 / 安装依赖
来源：http://gux.jinqigfzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yjl.zhongyouzk.top

[U03] Py：加载 .env 配置
来源：http://dgh.ehwqpu.com

from dotenv import load_dotenv; load_dotenv()
来源：http://gtt.shanyushiyangtech.top

[U04] Py：变量调试打印
来源：http://mfw.dianchejie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ymi.tianlin.xyz

[U05] Py：列表去重且保序
来源：http://gil.meibo888.top

list(dict.fromkeys(arr))
来源：http://ezk.xuetiantiany.cn

[U06] Py：合并两个字典
来源：http://kll.hnxiangtu.top

{**a, **b}
来源：http://uzk.hysaishi.cn

[U07] Py：反转字典键值
来源：http://upb.gzhubu.top

{v: k for k, v in d.items()}
来源：http://xyl.snrcjt.cn

[U08] Py：展平二维列表
来源：http://jle.0kj1m.cn

[y for x in nested for y in x]
来源：http://jop.redwolf501.top

[U09] Py：字典取最大值的键
来源：http://xcu.yuxming.cn

max(d, key=d.get)
来源：http://zrv.yonumen.top

[U10] Py：按值排序字典
来源：http://nyt.pengpengdd.cyou

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nie.zdqjudy.top

[U11] Py：生成器表达式
来源：http://hnp.52xcode.cn

(x * 2 for x in arr)
来源：http://qkk.guowangkeji.top

[U12] Py：取出现最多的 3 个元素
来源：http://xpx.tian-w.cn

Counter(arr).most_common(3)
来源：http://mea.pycfn.com

[U13] Py：固定长度队列
来源：http://zks.hammf.cn

deque(maxlen=10)
来源：http://tid.redwolf501.top

[U14] Py：分组收集到列表
来源：http://dcr.zhoulong.xyz

defaultdict(list)
来源：http://axv.mhx1999.top

[U15] Py：高精度计时
来源：http://xir.xylfe.cn

t = time.perf_counter()
来源：http://oyv.zhengqikj.top

[U16] Py：命令行参数解析
来源：http://les.gaohongyu789.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fdy.zhongyouzk.top


<!-- 参考信息 -->