代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://ott.havefunace.top

[R76] 使用临时文件
来源：http://ulc.zhijiandao.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tzr.yanxiufei.cn

[R77] 读取用户输入
来源：http://bwp.nanxinkj.top

read -rp "请输入: " ans
来源：http://hhw.sysykeji.top

[R78] 交互式菜单
来源：http://ise.yuxming.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ghm.pengpengdd.cyou

[R79] 解析命令行选项
来源：http://yjb.jinqigfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dhw.hammf.cn

[R80] 查看脚本执行耗时
来源：http://yzn.9152youxi.cn

time ./run.sh
来源：http://ztn.zhongyouzk.top

================================================================================
来源：http://vjt.jqgfzy.top

S. C / C++ 专题
来源：http://uya.chenlongwang.top

================================================================================
来源：http://qqq.quarkkingdee.top

[S01] C：Hello World
来源：http://dfu.dianchejie.cn

#include <stdio.h>
来源：http://zqv.ppjwa.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cjr.svipenyu.cn

[S02] C：变量与格式化输出
来源：http://qkw.sxryk.cn

int a = 10; printf("%d\n", a);
来源：http://liu.hfpthk.cn

[S03] C：读入整数
来源：http://njr.hcnkem.com

int x; scanf("%d", &x);
来源：http://rfb.hesvh.cn

[S04] C：字符串复制
来源：http://ydo.zhiwuduotai.top

char dst[32]; strcpy(dst, "hi");
来源：http://fxz.hcnkem.com

[S05] C：字符串长度
来源：http://vvp.zhiwuduotai.top

strlen(s)
来源：http://vba.uphjek.com

[S06] C：字符串比较
来源：http://mdg.tianlin.xyz

strcmp(a, b) == 0
来源：http://sgl.jinghuilouyu.cn

[S07] C：数组遍历求和
来源：http://mco.yongpay.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lns.svipenyu.cn

[S08] C：动态内存分配与释放
来源：http://xob.birdmap.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ryj.zhengqikj.top

[S09] C：结构体定义与初始化
来源：http://mjb.ppjwa.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xgh.vehdjk.com

[S10] C：指针与解引用
来源：http://lle.hnxiangtu.top

int *p = &a;  *p = 5;
来源：http://sjc.jyoumei.cn

[S11] C：逐行读文件
来源：http://lcr.fengsongda.top

FILE *f = fopen("a.txt", "r");
来源：http://tyj.yj202588.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://bfb.shuidangran.top

fclose(f);
来源：http://ajo.ctjpmb.com

[S12] C：写文件
来源：http://kcn.zhijiandao.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qkz.aizwys.cn

[S13] C：宏定义
来源：http://sxo.dianchejie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hir.jqgfzy.top

[S14] C：枚举
来源：http://pyh.bjfxy.top

enum Color { RED, GREEN, BLUE };
来源：http://eyz.zhijiandao.cn

[S15] C：类型转换
来源：http://eah.hesvh.cn

(double) a / b
来源：http://xzz.jinqigufen.top

[S16] C：位操作置位
来源：http://vcp.yvedp.cn

x |= (1 << 3);
来源：http://xbi.kuanghao11.cn

[S17] C：安全拼接字符串
来源：http://mvl.zdbjq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tda.hnxiangtu.top

[S18] C：命令行参数
来源：http://bie.gogol.net.cn

int main(int argc, char **argv)
来源：http://uwt.pengpengdd.cyou

[S19] C：快速排序
来源：http://ioa.zdqjudy.top

qsort(a, n, sizeof(int), cmp);
来源：http://gay.yfazqb.com

[S20] C：二分查找
来源：http://djp.316326.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zpx.ybcxt.top

[S21] C：字符类别判断
来源：http://ynp.fktsv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hef.ppjwa.cn

[S22] C：字符串转数字
来源：http://nun.yj20258888.top

atoi("42");  strtod("3.14", NULL);
来源：http://olr.cucudq.cn

[S23] C：随机数
来源：http://nsx.hywenlv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cvu.redwolf501.top

[S24] C：获取本地时间
来源：http://hxp.shzxlz.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pvs.smart0.xyz

[S25] C：内存拷贝
来源：http://oic.316326.xyz

memcpy(dst, src, n);
来源：http://xlm.wangshuangyany.cn

[S26] C：内存清零
来源：http://dvf.tanke756.top

memset(a, 0, sizeof a);
来源：http://rge.yonumen.top

[S27] C：定义常量
来源：http://pcb.ybcxt.top

const double PI = 3.14159;
来源：http://uek.sjlbkw.cn

[S28] C：静态变量
来源：http://kgr.smart0.xyz

static int counter = 0;
来源：http://saj.sysykeji.top

[S29] C：变参函数
来源：http://qzn.fzhhl.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bln.quarkkingdee.top

[S30] C：头文件保护
来源：http://yrd.birdmap.top

#ifndef X_H
来源：http://tsv.zdbjq.cn

#define X_H
来源：http://rcr.gzhubu.top

#endif
来源：http://aoh.yj20258.top

[S31] C++：Hello World
来源：http://xvq.shanyushiyangkeji.top

#include <iostream>
来源：http://vun.0kj1m.cn

int main() { std::cout << "Hello\n"; }
来源：http://ytu.vehdjk.com

[S32] C++：字符串
来源：http://djw.hnqzz.top

std::string s = "hi";  s += "!";
来源：http://yrc.mhx1999.top

[S33] C++：vector 增删
来源：http://rhq.daria6918.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dei.tanke756.top

[S34] C++：遍历 vector
来源：http://bwt.guannengcc.top

for (auto &x : v) { std::cout << x; }
来源：http://gnw.yj20258888.top

[S35] C++：map
来源：http://dsi.fehbvm.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lax.yangfankeji.com

[S36] C++：unordered_map
来源：http://hhs.hcnkem.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vjo.52xcode.cn

[S37] C++：set
来源：http://gwn.hysaishi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bgn.fengsongda.top

[S38] C++：排序
来源：http://lad.jyoumei.cn

std::sort(v.begin(), v.end());
来源：http://dmv.xingfuxueyuan.xyz

[S39] C++：自定义比较器排序
来源：http://uxu.hywenlv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lbp.hfpthk.cn

[S40] C++：查找元素
来源：http://jxi.52xcode.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://oit.kuanghao11.cn

[S41] C++：类与构造函数
来源：http://edu.yj20258888.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dan.svipenyu.cn

[S42] C++：继承与虚函数
来源：http://fyb.zhongyouzk.top

class B : public Base { public: void f() override {} };
来源：http://yug.yvedp.cn

[S43] C++：智能指针
来源：http://aaz.yongpay.top

auto p = std::make_unique<int>(5);
来源：http://gjk.jinqigufen.top

[S44] C++：引用传参
来源：http://mro.yuanzhike.top

void inc(int &x) { ++x; }
来源：http://yqu.bjfxy.top

[S45] C++：lambda
来源：http://xjd.cheryme.top

auto add = [](int a, int b) { return a + b; };
来源：http://wbu.dashuyun.cn

[S46] C++：函数模板
来源：http://vkj.svipenyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ndm.cucudq.cn

[S47] C++：结构化绑定遍历
来源：http://qji.haohaochexian.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tmg.jqgfzy.top

[S48] C++：逐行读文件
来源：http://wqs.zhijiandao.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fqc.gaohongyu789.top

while (std::getline(in, line)) { }
来源：http://zub.xziqi.cn

[S49] C++：写文件
来源：http://dpu.ivvv.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://foj.hcnkem.com

[S50] C++：格式化数字
来源：http://unb.cheryme.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ahz.fktsv.cn

[S51] C++：显式类型转换
来源：http://zfx.c1oappe.top

static_cast<double>(a) / b
来源：http://btd.zycfv.cn

[S52] C++：const 与 noexcept
来源：http://kip.zhaomingkeji.xyz

int size() const noexcept { return n_; }
来源：http://nuo.iojbl.cn

[S53] C++：移动语义
来源：http://vtr.shanyushiyangtech.top

std::vector<int> w = std::move(v);
来源：http://eki.jqgufenzy.top

[S54] C++：异常处理
来源：http://xft.nanxinkj.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jqk.xingfuxueyuan.xyz

[S55] C++：结构化绑定
来源：http://tlh.yuxming.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://arm.tianlin.xyz

[S56] C++：optional
来源：http://amo.nanxuanxn.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mmo.hongshengwenyu.top

[S57] C++：编译期常量
来源：http://wnb.jlsjyb.cn

constexpr int N = 10;
来源：http://hqg.hysaishi.cn

[S58] C++：命名空间
来源：http://ske.c1oappe.top

namespace ns { int f() { return 1; } }
来源：http://iad.yfazqb.com

[S59] C++：静态断言
来源：http://xlb.hammf.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://doh.jlsjyb.cn

[S60] C++：遍历并删除元素
来源：http://jns.jinqigufen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gno.cheryme.top

================================================================================
来源：http://fjw.gotoacloud.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ybn.yfazqb.com

================================================================================
来源：http://owb.ywan-chungtsiang.top

[T01] Kotlin：Hello World
来源：http://ogm.pengpengdd.cyou

println("Hello")
来源：http://icm.fengsongda.top

[T02] Kotlin：变量
来源：http://hfo.hfpthk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lyq.hfpthk.cn

[T03] Kotlin：字符串模板
来源：http://eno.chenjidiqi.icu

"值: $b"
来源：http://lsa.sufxvd.cn

[T04] Kotlin：空安全
来源：http://ocs.jinyuanbaomall.cn

val n: String? = null;  n?.length
来源：http://anv.shanyushiyangtech.top

[T05] Kotlin：when 表达式
来源：http://suc.daria6918.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hwo.vehdjk.com

[T06] Kotlin：集合映射
来源：http://ody.yueranfly.top

listOf(1, 2, 3).map { it * 2 }
来源：http://gqu.jiagoushi.top

[T07] Kotlin：集合过滤
来源：http://ant.zhijiandao.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://prn.dashuyun.cn

[T08] Kotlin：数据类
来源：http://wzl.jinghuilouyu.cn

data class User(val name: String, val age: Int)
来源：http://uzc.hnxiangtu.top

[T09] Kotlin：扩展函数
来源：http://muw.andypj.xyz

fun String.exclaim() = this + "!"
来源：http://gcr.nanxinkj.top

[T10] Kotlin：默认参数
来源：http://npw.jinyuanbaomall.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tuj.redwolf501.top

[T11] Kotlin：协程
来源：http://sdr.shanyushiyangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://irj.yonumen.top

[T12] Kotlin：解构声明
来源：http://qov.havefunace.top

val (a, b) = Pair(1, 2)
来源：http://xmr.jinyuanbaomall.cn

[T13] Kotlin：只读 Map
来源：http://yda.iojbl.cn

val m = mapOf("a" to 1)
来源：http://aoa.mhx1999.top

[T14] Kotlin：循环
来源：http://wny.fktsv.cn

for (i in 1..10) println(i)
来源：http://hfo.bjfxy.top

[T15] Kotlin：接口
来源：http://cya.vehdjk.com

interface Shape { fun area(): Double }
来源：http://oxl.ehwqpu.com

[T16] Swift：Hello World
来源：http://ijo.sxryk.cn

print("Hello")
来源：http://scu.jyoumei.cn

[T17] Swift：变量与常量
来源：http://mtu.wangdashe.top

var a = 1;  let b = 2
来源：http://ofw.uphjek.com

[T18] Swift：字符串插值
来源：http://ios.guannengcc.top

"值: \(b)"
来源：http://yjh.yvedp.cn

[T19] Swift：可选绑定
来源：http://eqi.zhongyouzk.top

if let n = opt { print(n) }
来源：http://osp.316326.xyz

[T20] Swift：数组操作
来源：http://lvm.hammf.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cqv.xylfe.cn

[T21] Swift：遍历
来源：http://wwm.jinyuanbaomall.cn

for x in a { print(x) }
来源：http://shx.fktsv.cn

[T22] Swift：字典
来源：http://gns.sjlbkw.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xpa.jyoumei.cn

[T23] Swift：函数
来源：http://drf.gzhubu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zpp.hnxiangtu.top

[T24] Swift：闭包
来源：http://tmv.zdqjudy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://msr.daria6918.cn

[T25] Swift：结构体
来源：http://oit.0kj1m.cn

struct P { var x: Int }
来源：http://osl.zycfv.cn

[T26] Swift：类与重写
来源：http://urb.0kj1m.cn

class A: Base { override func f() {} }
来源：http://eie.shangyingyoupin.top

[T27] Swift：错误处理
来源：http://vjo.hammf.cn

do { try f() } catch { print(error) }
来源：http://rhc.cqqwz.cn

[T28] Swift：枚举
来源：http://eji.aibaodan.cn

enum Color { case red, green }
来源：http://xzy.ywan-chungtsiang.top

[T29] Swift：guard 提前返回
来源：http://hrv.52xcode.cn

guard let x = opt else { return }
来源：http://abj.sxryk.cn

[T30] Swift：协议
来源：http://mnw.epnwcf.com

protocol Shape { func area() -> Double }
来源：http://njb.xinyue.icu

[T31] Lua：Hello World
来源：http://lav.jyoumei.cn

print("Hello")
来源：http://onm.nanxinkj.top

[T32] Lua：局部变量
来源：http://lyt.hammf.cn

local a = 1
来源：http://jbn.mhx1999.top

[T33] Lua：表（数组）
来源：http://bmz.daxiang520.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ohl.xuetiantiany.cn

[T34] Lua：遍历表
来源：http://fvo.ehwqpu.com

for i, v in ipairs(t) do print(i, v) end
来源：http://xdt.jinqigufen.top

[T35] Lua：字典表
来源：http://flh.chenlongwang.top

local d = { a = 1 };  d.b = 2
来源：http://ssv.iojbl.cn

[T36] Lua：函数
来源：http://zqg.birdmap.top

function add(a, b) return a + b end
来源：http://hgh.svipenyu.cn

[T37] Lua：字符串拼接
来源：http://jkc.guannengcc.top

"a" .. "b"
来源：http://qiw.hfpthk.cn

[T38] Lua：条件
来源：http://xwq.fehbvm.com

if x > 0 then print("正") end
来源：http://bun.shzxlz.cn

[T39] Lua：模式匹配
来源：http://vrl.tanke756.top

string.find(s, "%d+")
来源：http://ail.gaohongyu789.top

[T40] Lua：元表
来源：http://cmg.hnqzz.top

setmetatable({}, { __index = base })
来源：http://yqy.snrcjt.cn

[T41] Perl：Hello World
来源：http://eir.mhx1999.top

print "Hello\n";
来源：http://zbz.cheryme.top

[T42] Perl：变量类型
来源：http://iov.jianghu66.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://axb.birdmap.top

[T43] Perl：字符串插值
来源：http://zry.zhongyouzk.top

"值: $a"
来源：http://dwa.jinqigufen.top

[T44] Perl：条件
来源：http://hbv.shzxlz.cn

if ($a > 0) { print "正"; }
来源：http://kyu.tianlin.xyz

[T45] Perl：数组遍历
来源：http://oss.hywenlv.cn

for my $x (@arr) { print $x; }
来源：http://fdt.ydzc1.top

[T46] Perl：哈希操作
来源：http://vne.yj20258.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xiy.xingfuxueyuan.xyz

[T47] Perl：正则捕获
来源：http://dlq.xinyue.icu

if ($s =~ /(\d+)/) { print $1; }
来源：http://edr.xingfuxueyuan.xyz

[T48] Perl：正则替换
来源：http://nvf.yj20258888.top

$s =~ s/old/new/g;
来源：http://zze.iojbl.cn

[T49] Perl：函数
来源：http://lku.zhijiandao.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ppa.yj202588.top

[T50] Perl：逐行读文件
来源：http://ddv.shangyingyoupin.top

open my $fh, "<", "a.txt" or die $!;
来源：http://kki.gogol.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://jih.cashguo.top

[T51] Scala：Hello World
来源：http://smt.havefunace.top

println("Hello")
来源：http://obm.0kj1m.cn

[T52] Scala：变量
来源：http://jyw.fzhhl.top

val a = 1;  var b = 2
来源：http://ezl.hnqzz.top

[T53] Scala：字符串插值
来源：http://vny.ivvv.top

s"值: $b"
来源：http://zjy.fanxiaobao.xyz

[T54] Scala：集合映射
来源：http://spm.zhaomingkeji.xyz

List(1, 2, 3).map(_ * 2)
来源：http://ssl.sufxvd.cn

[T55] Scala：集合过滤
来源：http://mad.xuanzx.com

List(1, 2, 3).filter(_ > 1)
来源：http://txh.yangfankeji.com

[T56] Scala：样例类
来源：http://uny.316326.xyz

case class User(name: String, age: Int)
来源：http://res.ybcxt.top

[T57] Scala：模式匹配
来源：http://req.yangfankeji.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://xpl.bjfxy.top

[T58] Scala：函数定义
来源：http://jjx.andypj.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://kmj.316326.xyz

[T59] Scala：循环
来源：http://ibh.jiagoushi.top

for (i <- 1 to 10) println(i)
来源：http://gud.zycfv.cn

[T60] Scala：折叠
来源：http://mls.yonumen.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qab.zdbjq.cn

================================================================================
来源：http://aku.hammf.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vhy.wangshuangyany.cn

================================================================================
来源：http://juz.zhaomingkeji.xyz

[U01] Py：创建虚拟环境
来源：http://uuw.jianghu66.top

python -m venv .venv && source .venv/bin/activate
来源：http://sdp.jlsjyb.cn

[U02] Py：导出 / 安装依赖
来源：http://wyg.yanxiufei.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vxw.tarul.cn

[U03] Py：加载 .env 配置
来源：http://vfc.jinqigufen.top

from dotenv import load_dotenv; load_dotenv()
来源：http://lrb.ehwqpu.com

[U04] Py：变量调试打印
来源：http://fwi.feifeiyinyue.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eao.xingfuxueyuan.xyz

[U05] Py：列表去重且保序
来源：http://otd.yfazqb.com

list(dict.fromkeys(arr))
来源：http://nbj.tarul.cn

[U06] Py：合并两个字典
来源：http://jrq.dashuyun.cn

{**a, **b}
来源：http://wed.sufxvd.cn

[U07] Py：反转字典键值
来源：http://zvw.gotoacloud.top

{v: k for k, v in d.items()}
来源：http://dtk.yfazqb.com

[U08] Py：展平二维列表
来源：http://gwi.yanxiufei.cn

[y for x in nested for y in x]
来源：http://ywb.tanke756.top

[U09] Py：字典取最大值的键
来源：http://ufe.jinqigfzy.top

max(d, key=d.get)
来源：http://qic.havefunace.top

[U10] Py：按值排序字典
来源：http://ols.gaohongyu789.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hwf.jinghuilouyu.cn

[U11] Py：生成器表达式
来源：http://xly.yongpay.top

(x * 2 for x in arr)
来源：http://dsi.zhongyouzk.top

[U12] Py：取出现最多的 3 个元素
来源：http://imb.sysykeji.top

Counter(arr).most_common(3)
来源：http://mfk.0kj1m.cn

[U13] Py：固定长度队列
来源：http://hpl.hongshengwenyu.top

deque(maxlen=10)
来源：http://jrv.sweek.top

[U14] Py：分组收集到列表
来源：http://nyy.0kj1m.cn

defaultdict(list)
来源：http://voa.nwbrower.top

[U15] Py：高精度计时
来源：http://scs.tianlin.xyz

t = time.perf_counter()
来源：http://von.yvedp.cn

[U16] Py：命令行参数解析
来源：http://bfi.yongpay.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fny.yueranfly.top


<!-- 参考信息 -->