代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://bje.cheryme.top

[R76] 使用临时文件
来源：http://ewg.hywenlv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dvx.52xcode.cn

[R77] 读取用户输入
来源：http://vgl.tian-w.cn

read -rp "请输入: " ans
来源：http://xcj.tarul.cn

[R78] 交互式菜单
来源：http://saq.jinqigfzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://bzv.yonumen.top

[R79] 解析命令行选项
来源：http://asq.nwbrower.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hzb.jqgufenzy.top

[R80] 查看脚本执行耗时
来源：http://hxz.yvedp.cn

time ./run.sh
来源：http://fpk.pengpengdd.cyou

================================================================================
来源：http://has.ydzc1.top

S. C / C++ 专题
来源：http://jzh.yangfankeji.com

================================================================================
来源：http://xoj.cheryme.top

[S01] C：Hello World
来源：http://qxa.zhengqikj.top

#include <stdio.h>
来源：http://etu.yongpay.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://spc.wangshuangyany.cn

[S02] C：变量与格式化输出
来源：http://erq.cdnleiting.top

int a = 10; printf("%d\n", a);
来源：http://zln.zhixingplan.top

[S03] C：读入整数
来源：http://tdj.cdnleiting.top

int x; scanf("%d", &x);
来源：http://rka.zhaomingkeji.xyz

[S04] C：字符串复制
来源：http://jqg.gaohongyu789.top

char dst[32]; strcpy(dst, "hi");
来源：http://igb.andypj.xyz

[S05] C：字符串长度
来源：http://sct.sjlbkw.cn

strlen(s)
来源：http://alo.svipenyu.cn

[S06] C：字符串比较
来源：http://nlx.wangshuangyany.cn

strcmp(a, b) == 0
来源：http://vwu.gaohongyu789.top

[S07] C：数组遍历求和
来源：http://kqb.yj20258.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jmo.vqdsnc.cn

[S08] C：动态内存分配与释放
来源：http://amj.svipenyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eai.nanxuanxn.top

[S09] C：结构体定义与初始化
来源：http://vel.ybcxt.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://epp.yj202588.top

[S10] C：指针与解引用
来源：http://ucx.jinyuanbaomall.cn

int *p = &a;  *p = 5;
来源：http://alu.snrcjt.cn

[S11] C：逐行读文件
来源：http://djr.daxiang520.top

FILE *f = fopen("a.txt", "r");
来源：http://oys.iojbl.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qtp.hcnkem.com

fclose(f);
来源：http://kyk.xylfe.cn

[S12] C：写文件
来源：http://guq.yj202588.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uvr.zhoulong.xyz

[S13] C：宏定义
来源：http://xve.yuanzhike.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kbp.sjlbkw.cn

[S14] C：枚举
来源：http://lis.jinqigfzy.top

enum Color { RED, GREEN, BLUE };
来源：http://xok.aizwys.cn

[S15] C：类型转换
来源：http://dtl.zhaomingkeji.xyz

(double) a / b
来源：http://ygq.jinghuilouyu.cn

[S16] C：位操作置位
来源：http://pas.chenzaomai.com

x |= (1 << 3);
来源：http://wbv.hysaishi.cn

[S17] C：安全拼接字符串
来源：http://oqh.shanyushiyangkeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hrj.gzhubu.top

[S18] C：命令行参数
来源：http://mmd.snrcjt.cn

int main(int argc, char **argv)
来源：http://ntx.zhaomingkeji.xyz

[S19] C：快速排序
来源：http://kyv.xuanzx.com

qsort(a, n, sizeof(int), cmp);
来源：http://wav.tanke756.top

[S20] C：二分查找
来源：http://xka.ehwqpu.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ivj.svipenyu.cn

[S21] C：字符类别判断
来源：http://vie.vqdsnc.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hyv.vehdjk.com

[S22] C：字符串转数字
来源：http://knx.ywan-chungtsiang.top

atoi("42");  strtod("3.14", NULL);
来源：http://msd.zhixingplan.top

[S23] C：随机数
来源：http://hlq.jinqigufen.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ywr.bjfxy.top

[S24] C：获取本地时间
来源：http://pjl.ywan-chungtsiang.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://unt.yj20258.top

[S25] C：内存拷贝
来源：http://vly.pengpengdd.cyou

memcpy(dst, src, n);
来源：http://coa.pengpengdd.cyou

[S26] C：内存清零
来源：http://deb.dashuyun.cn

memset(a, 0, sizeof a);
来源：http://tig.vqdsnc.cn

[S27] C：定义常量
来源：http://jfz.jinqigfzy.top

const double PI = 3.14159;
来源：http://bxh.cashguo.top

[S28] C：静态变量
来源：http://alk.svipenyu.cn

static int counter = 0;
来源：http://jmk.fktsv.cn

[S29] C：变参函数
来源：http://ymf.zhijiandao.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://phk.daxiang520.top

[S30] C：头文件保护
来源：http://uzb.cdnleiting.top

#ifndef X_H
来源：http://qbf.sxryk.cn

#define X_H
来源：http://jfn.shuidangran.top

#endif
来源：http://hdj.0kj1m.cn

[S31] C++：Hello World
来源：http://lhp.jyoumei.cn

#include <iostream>
来源：http://lcz.cdnleiting.top

int main() { std::cout << "Hello\n"; }
来源：http://gqz.haohaochexian.top

[S32] C++：字符串
来源：http://kci.zdbjq.cn

std::string s = "hi";  s += "!";
来源：http://jtp.ywan-chungtsiang.top

[S33] C++：vector 增删
来源：http://diz.meibo888.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pcc.yj202588.top

[S34] C++：遍历 vector
来源：http://eza.nwbrower.top

for (auto &x : v) { std::cout << x; }
来源：http://udf.wangdashe.top

[S35] C++：map
来源：http://plt.yj20258888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://iaa.xinyue.icu

[S36] C++：unordered_map
来源：http://ewx.316326.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://avb.xuetiantiany.cn

[S37] C++：set
来源：http://zbz.sysykeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://afx.yanxiufei.cn

[S38] C++：排序
来源：http://crk.vehdjk.com

std::sort(v.begin(), v.end());
来源：http://uek.yvedp.cn

[S39] C++：自定义比较器排序
来源：http://axo.shanyushiyangtech.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hpo.jlsjyb.cn

[S40] C++：查找元素
来源：http://jdz.cqqwz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rhf.tian-w.cn

[S41] C++：类与构造函数
来源：http://tve.yj202588.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kxk.mhx1999.top

[S42] C++：继承与虚函数
来源：http://qzj.svipenyu.cn

class B : public Base { public: void f() override {} };
来源：http://dtg.hesvh.cn

[S43] C++：智能指针
来源：http://itm.jqgufenzy.top

auto p = std::make_unique<int>(5);
来源：http://fhd.ybcxt.top

[S44] C++：引用传参
来源：http://hga.shangyingyoupin.top

void inc(int &x) { ++x; }
来源：http://gtd.feifeiyinyue.top

[S45] C++：lambda
来源：http://bpd.bbcook.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wja.yueranfly.top

[S46] C++：函数模板
来源：http://yfb.xingfuxueyuan.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wel.xingfuxueyuan.xyz

[S47] C++：结构化绑定遍历
来源：http://zzp.gaohongyu789.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bwe.nanxinkj.top

[S48] C++：逐行读文件
来源：http://xev.tarul.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qim.hcnkem.com

while (std::getline(in, line)) { }
来源：http://iaj.zhaomingkeji.xyz

[S49] C++：写文件
来源：http://nxt.vehdjk.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vyq.zhengqikj.top

[S50] C++：格式化数字
来源：http://noi.zhiwuduotai.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jmp.yuxming.cn

[S51] C++：显式类型转换
来源：http://zbf.dianchejie.cn

static_cast<double>(a) / b
来源：http://hgv.yongpay.top

[S52] C++：const 与 noexcept
来源：http://cor.zycfv.cn

int size() const noexcept { return n_; }
来源：http://rdw.gzhubu.top

[S53] C++：移动语义
来源：http://oqj.hysaishi.cn

std::vector<int> w = std::move(v);
来源：http://wzg.yvedp.cn

[S54] C++：异常处理
来源：http://ykq.yj20258.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bkz.guannengcc.top

[S55] C++：结构化绑定
来源：http://ett.yonumen.top

auto [a, b] = std::make_pair(1, 2);
来源：http://vvj.havefunace.top

[S56] C++：optional
来源：http://orw.daxiang520.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kjg.shuidangran.top

[S57] C++：编译期常量
来源：http://pod.cheryme.top

constexpr int N = 10;
来源：http://zky.sxryk.cn

[S58] C++：命名空间
来源：http://aom.0kj1m.cn

namespace ns { int f() { return 1; } }
来源：http://ram.cheryme.top

[S59] C++：静态断言
来源：http://ysh.yanxiufei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gtq.0kj1m.cn

[S60] C++：遍历并删除元素
来源：http://khf.jqgfzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ypr.dashuyun.cn

================================================================================
来源：http://zvr.haohaochexian.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://stz.fktsv.cn

================================================================================
来源：http://oio.tianlin.xyz

[T01] Kotlin：Hello World
来源：http://gje.sjlbkw.cn

println("Hello")
来源：http://bwo.jlsjyb.cn

[T02] Kotlin：变量
来源：http://nmm.smart0.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kru.jyoumei.cn

[T03] Kotlin：字符串模板
来源：http://csg.guowangkeji.top

"值: $b"
来源：http://wtu.dashuyun.cn

[T04] Kotlin：空安全
来源：http://yqs.gogol.net.cn

val n: String? = null;  n?.length
来源：http://fal.gotoacloud.top

[T05] Kotlin：when 表达式
来源：http://zbl.mhx1999.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://geu.ybcxt.top

[T06] Kotlin：集合映射
来源：http://ayg.aizwys.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gok.gotoacloud.top

[T07] Kotlin：集合过滤
来源：http://ndq.zhoulong.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://uqu.yj20258.top

[T08] Kotlin：数据类
来源：http://wnt.chenzaomai.com

data class User(val name: String, val age: Int)
来源：http://mcy.jinqigufen.top

[T09] Kotlin：扩展函数
来源：http://gvk.quarkkingdee.top

fun String.exclaim() = this + "!"
来源：http://sxn.ydzc1.top

[T10] Kotlin：默认参数
来源：http://iqr.ydzc1.top

fun greet(name: String = "World") = "Hi $name"
来源：http://iff.nwbrower.top

[T11] Kotlin：协程
来源：http://cbf.cashguo.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gkt.fehbvm.com

[T12] Kotlin：解构声明
来源：http://mkr.sweek.top

val (a, b) = Pair(1, 2)
来源：http://wtd.zhengqikj.top

[T13] Kotlin：只读 Map
来源：http://dgo.jyoumei.cn

val m = mapOf("a" to 1)
来源：http://pnk.meibo888.top

[T14] Kotlin：循环
来源：http://nxj.fehbvm.com

for (i in 1..10) println(i)
来源：http://kdn.yangfankeji.com

[T15] Kotlin：接口
来源：http://ths.hnqzz.top

interface Shape { fun area(): Double }
来源：http://dum.nwbrower.top

[T16] Swift：Hello World
来源：http://ppy.bbcook.cn

print("Hello")
来源：http://bie.jinqigufen.top

[T17] Swift：变量与常量
来源：http://ubu.shangyingyoupin.top

var a = 1;  let b = 2
来源：http://twd.sysykeji.top

[T18] Swift：字符串插值
来源：http://hfz.hesvh.cn

"值: \(b)"
来源：http://qsi.tian-w.cn

[T19] Swift：可选绑定
来源：http://fjk.guowangkeji.top

if let n = opt { print(n) }
来源：http://nyq.zhixingplan.top

[T20] Swift：数组操作
来源：http://nbb.mhx1999.top

var a = [1, 2, 3];  a.append(4)
来源：http://dvr.chenlongwang.top

[T21] Swift：遍历
来源：http://ihp.yonumen.top

for x in a { print(x) }
来源：http://xxa.sysykeji.top

[T22] Swift：字典
来源：http://kxd.shuidangran.top

var d = ["a": 1];  d["b"] = 2
来源：http://hax.ivvv.top

[T23] Swift：函数
来源：http://zux.zdqjudy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://oqh.nwbrower.top

[T24] Swift：闭包
来源：http://kgo.redwolf501.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://wso.cashguo.top

[T25] Swift：结构体
来源：http://tqp.sjlbkw.cn

struct P { var x: Int }
来源：http://clv.gogol.net.cn

[T26] Swift：类与重写
来源：http://xfp.yongpay.top

class A: Base { override func f() {} }
来源：http://znj.wangshuangyany.cn

[T27] Swift：错误处理
来源：http://nkn.cdnleiting.top

do { try f() } catch { print(error) }
来源：http://vrx.yj20258.top

[T28] Swift：枚举
来源：http://vkg.xuetiantiany.cn

enum Color { case red, green }
来源：http://kyh.sufxvd.cn

[T29] Swift：guard 提前返回
来源：http://yeq.xingfuxueyuan.xyz

guard let x = opt else { return }
来源：http://ote.meibo888.top

[T30] Swift：协议
来源：http://mrl.svipenyu.cn

protocol Shape { func area() -> Double }
来源：http://lbt.316326.xyz

[T31] Lua：Hello World
来源：http://qcc.shangyingyoupin.top

print("Hello")
来源：http://kav.ywan-chungtsiang.top

[T32] Lua：局部变量
来源：http://qkh.sweek.top

local a = 1
来源：http://bhj.epnwcf.com

[T33] Lua：表（数组）
来源：http://qpc.ydzc1.top

local t = {1, 2, 3};  t[4] = 4
来源：http://xeh.quarkkingdee.top

[T34] Lua：遍历表
来源：http://hsp.ctjpmb.com

for i, v in ipairs(t) do print(i, v) end
来源：http://puf.yj20258888.top

[T35] Lua：字典表
来源：http://sbr.xylfe.cn

local d = { a = 1 };  d.b = 2
来源：http://sxk.fengsongda.top

[T36] Lua：函数
来源：http://vxt.jqgufenzy.top

function add(a, b) return a + b end
来源：http://jha.iojbl.cn

[T37] Lua：字符串拼接
来源：http://voj.fktsv.cn

"a" .. "b"
来源：http://kab.hnxiangtu.top

[T38] Lua：条件
来源：http://ikh.ctjpmb.com

if x > 0 then print("正") end
来源：http://hju.jyoumei.cn

[T39] Lua：模式匹配
来源：http://udi.zhengqikj.top

string.find(s, "%d+")
来源：http://uuc.zhaomingkeji.xyz

[T40] Lua：元表
来源：http://isb.zhijiandao.cn

setmetatable({}, { __index = base })
来源：http://hoo.ehwqpu.com

[T41] Perl：Hello World
来源：http://wqr.aizwys.cn

print "Hello\n";
来源：http://klz.yonumen.top

[T42] Perl：变量类型
来源：http://jbk.pengpengdd.cyou

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://atf.sjlbkw.cn

[T43] Perl：字符串插值
来源：http://ash.yj202588.top

"值: $a"
来源：http://qpt.ydzc1.top

[T44] Perl：条件
来源：http://svk.daxiang520.top

if ($a > 0) { print "正"; }
来源：http://gbe.9152youxi.cn

[T45] Perl：数组遍历
来源：http://qzn.ctjpmb.com

for my $x (@arr) { print $x; }
来源：http://ash.zdqjudy.top

[T46] Perl：哈希操作
来源：http://rle.shangyingyoupin.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nqn.yuanzhike.top

[T47] Perl：正则捕获
来源：http://bmb.wangdashe.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://akp.jqgufenzy.top

[T48] Perl：正则替换
来源：http://qej.jianghu66.top

$s =~ s/old/new/g;
来源：http://hbk.sxryk.cn

[T49] Perl：函数
来源：http://jno.shuidangran.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zpy.jinghuilouyu.cn

[T50] Perl：逐行读文件
来源：http://fcj.pengpengdd.cyou

open my $fh, "<", "a.txt" or die $!;
来源：http://ylo.sjlbkw.cn

while (my $line = <$fh>) { print $line; }
来源：http://std.shanyushiyangtech.top

[T51] Scala：Hello World
来源：http://fny.ywan-chungtsiang.top

println("Hello")
来源：http://olo.xuanzx.com

[T52] Scala：变量
来源：http://gxj.hywenlv.cn

val a = 1;  var b = 2
来源：http://yii.daxiang520.top

[T53] Scala：字符串插值
来源：http://azb.sxryk.cn

s"值: $b"
来源：http://the.zdqjudy.top

[T54] Scala：集合映射
来源：http://qpz.zycfv.cn

List(1, 2, 3).map(_ * 2)
来源：http://zkh.cashguo.top

[T55] Scala：集合过滤
来源：http://qpv.yueranfly.top

List(1, 2, 3).filter(_ > 1)
来源：http://ejo.cqqwz.cn

[T56] Scala：样例类
来源：http://tkj.xuanzx.com

case class User(name: String, age: Int)
来源：http://ghu.hnqzz.top

[T57] Scala：模式匹配
来源：http://kov.xinyue.icu

x match { case 1 => "一"; case _ => "其他" }
来源：http://hph.andypj.xyz

[T58] Scala：函数定义
来源：http://zsy.smart0.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://fxs.zhiwuduotai.top

[T59] Scala：循环
来源：http://xog.xingfuxueyuan.xyz

for (i <- 1 to 10) println(i)
来源：http://nys.cashguo.top

[T60] Scala：折叠
来源：http://dcd.gotoacloud.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tuu.yonumen.top

================================================================================
来源：http://een.cdnleiting.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zxa.mhx1999.top

================================================================================
来源：http://ssy.yj20258.top

[U01] Py：创建虚拟环境
来源：http://wms.shuidangran.top

python -m venv .venv && source .venv/bin/activate
来源：http://wlt.yongpay.top

[U02] Py：导出 / 安装依赖
来源：http://prg.hnxiangtu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://etw.cqqwz.cn

[U03] Py：加载 .env 配置
来源：http://drs.tian-w.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vay.yuanzhike.top

[U04] Py：变量调试打印
来源：http://ijz.smart0.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wpw.xylfe.cn

[U05] Py：列表去重且保序
来源：http://zzr.hcnkem.com

list(dict.fromkeys(arr))
来源：http://cgy.nanxinkj.top

[U06] Py：合并两个字典
来源：http://lox.zdbjq.cn

{**a, **b}
来源：http://rpq.zhoulong.xyz

[U07] Py：反转字典键值
来源：http://fuq.sjlbkw.cn

{v: k for k, v in d.items()}
来源：http://xfo.ctjpmb.com

[U08] Py：展平二维列表
来源：http://hoz.zhoulong.xyz

[y for x in nested for y in x]
来源：http://caq.yvedp.cn

[U09] Py：字典取最大值的键
来源：http://rgt.jinghuilouyu.cn

max(d, key=d.get)
来源：http://jjr.ydjk.org.cn

[U10] Py：按值排序字典
来源：http://mme.vqdsnc.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://twk.ivvv.top

[U11] Py：生成器表达式
来源：http://kpz.yuanzhike.top

(x * 2 for x in arr)
来源：http://pvj.zhoulong.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://iwz.jinqigfzy.top

Counter(arr).most_common(3)
来源：http://hiy.hongshengwenyu.top

[U13] Py：固定长度队列
来源：http://czm.chenjidiqi.icu

deque(maxlen=10)
来源：http://hfg.hcnkem.com

[U14] Py：分组收集到列表
来源：http://djc.nanxinkj.top

defaultdict(list)
来源：http://yxz.ehwqpu.com

[U15] Py：高精度计时
来源：http://ops.hnqzz.top

t = time.perf_counter()
来源：http://wdh.fengsongda.top

[U16] Py：命令行参数解析
来源：http://tgv.shuidangran.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hft.ydzc1.top


<!-- 参考信息 -->