代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://igo.zhaomingkeji.xyz

[R76] 使用临时文件
来源：http://xwf.sweek.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zhk.haohaochexian.top

[R77] 读取用户输入
来源：http://qjh.feifeiyinyue.top

read -rp "请输入: " ans
来源：http://gcg.jinyuanbaomall.cn

[R78] 交互式菜单
来源：http://xni.gaohongyu789.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rzc.ppjwa.cn

[R79] 解析命令行选项
来源：http://nvt.bjfxy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ibf.52xcode.cn

[R80] 查看脚本执行耗时
来源：http://oou.52xcode.cn

time ./run.sh
来源：http://vfz.tarul.cn

================================================================================
来源：http://gvc.sysykeji.top

S. C / C++ 专题
来源：http://pir.zhijiandao.cn

================================================================================
来源：http://mur.shzxlz.cn

[S01] C：Hello World
来源：http://bzf.cqqwz.cn

#include <stdio.h>
来源：http://dyw.shanyushiyangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xnj.bbcook.cn

[S02] C：变量与格式化输出
来源：http://ngx.hongshengwenyu.top

int a = 10; printf("%d\n", a);
来源：http://nsu.redwolf501.top

[S03] C：读入整数
来源：http://xig.hesvh.cn

int x; scanf("%d", &x);
来源：http://smc.yongpay.top

[S04] C：字符串复制
来源：http://pls.redwolf501.top

char dst[32]; strcpy(dst, "hi");
来源：http://cwv.chenlongwang.top

[S05] C：字符串长度
来源：http://nya.aibaodan.cn

strlen(s)
来源：http://thx.xingfuxueyuan.xyz

[S06] C：字符串比较
来源：http://six.hesvh.cn

strcmp(a, b) == 0
来源：http://tbr.chenlongwang.top

[S07] C：数组遍历求和
来源：http://kpf.jinqigfzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zpc.zdqjudy.top

[S08] C：动态内存分配与释放
来源：http://cnk.smart0.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uec.shangyingyoupin.top

[S09] C：结构体定义与初始化
来源：http://pjw.hammf.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lou.svipenyu.cn

[S10] C：指针与解引用
来源：http://jjw.ydjk.org.cn

int *p = &a;  *p = 5;
来源：http://kfo.ywan-chungtsiang.top

[S11] C：逐行读文件
来源：http://bmu.pengpengdd.cyou

FILE *f = fopen("a.txt", "r");
来源：http://vrb.tianlin.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://fmb.snrcjt.cn

fclose(f);
来源：http://xof.fanxiaobao.xyz

[S12] C：写文件
来源：http://kgb.shangyingyoupin.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://imz.yanxiufei.cn

[S13] C：宏定义
来源：http://urv.havefunace.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zsl.mhx1999.top

[S14] C：枚举
来源：http://nuu.mhx1999.top

enum Color { RED, GREEN, BLUE };
来源：http://cnm.xuanzx.com

[S15] C：类型转换
来源：http://ijl.nanxuanxn.top

(double) a / b
来源：http://jnq.xuanzx.com

[S16] C：位操作置位
来源：http://gno.nanxuanxn.top

x |= (1 << 3);
来源：http://uez.bjfxy.top

[S17] C：安全拼接字符串
来源：http://mxy.vehdjk.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://poz.316326.xyz

[S18] C：命令行参数
来源：http://vnq.yanxiufei.cn

int main(int argc, char **argv)
来源：http://grh.tanke756.top

[S19] C：快速排序
来源：http://pzx.nanxinkj.top

qsort(a, n, sizeof(int), cmp);
来源：http://dzr.bjfxy.top

[S20] C：二分查找
来源：http://miv.xuanzx.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wms.xuanzx.com

[S21] C：字符类别判断
来源：http://dyi.jqgufenzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hcs.ctjpmb.com

[S22] C：字符串转数字
来源：http://dty.xingfuxueyuan.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://esw.yanxiufei.cn

[S23] C：随机数
来源：http://xln.yanxiufei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pdg.jinqigufen.top

[S24] C：获取本地时间
来源：http://dra.jianghu66.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://iek.zycfv.cn

[S25] C：内存拷贝
来源：http://dyg.bjfxy.top

memcpy(dst, src, n);
来源：http://zzn.nanxuanxn.top

[S26] C：内存清零
来源：http://nuq.quarkkingdee.top

memset(a, 0, sizeof a);
来源：http://rrw.yj20258.top

[S27] C：定义常量
来源：http://mwp.shanyushiyangtech.top

const double PI = 3.14159;
来源：http://lsl.vqdsnc.cn

[S28] C：静态变量
来源：http://yzf.sweek.top

static int counter = 0;
来源：http://npx.cdnleiting.top

[S29] C：变参函数
来源：http://gni.ywan-chungtsiang.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rot.gogol.net.cn

[S30] C：头文件保护
来源：http://qkz.gaohongyu789.top

#ifndef X_H
来源：http://one.shanyushiyangkeji.top

#define X_H
来源：http://uor.hcnkem.com

#endif
来源：http://cmi.yueranfly.top

[S31] C++：Hello World
来源：http://xvw.birdmap.top

#include <iostream>
来源：http://hgv.haohaochexian.top

int main() { std::cout << "Hello\n"; }
来源：http://ipe.cdnleiting.top

[S32] C++：字符串
来源：http://lnd.yuanzhike.top

std::string s = "hi";  s += "!";
来源：http://fsy.cdnleiting.top

[S33] C++：vector 增删
来源：http://onl.zhiwuduotai.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qlr.ppjwa.cn

[S34] C++：遍历 vector
来源：http://azj.aibaodan.cn

for (auto &x : v) { std::cout << x; }
来源：http://lzm.gaohongyu789.top

[S35] C++：map
来源：http://hab.jlsjyb.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zlr.yueranfly.top

[S36] C++：unordered_map
来源：http://ejo.gotoacloud.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dyc.zhaomingkeji.xyz

[S37] C++：set
来源：http://tbh.guannengcc.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ayx.nwbrower.top

[S38] C++：排序
来源：http://gnb.yanxiufei.cn

std::sort(v.begin(), v.end());
来源：http://pvu.c1oappe.top

[S39] C++：自定义比较器排序
来源：http://spu.jqgfzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ewc.gogol.net.cn

[S40] C++：查找元素
来源：http://blw.pengpengdd.cyou

auto it = std::find(v.begin(), v.end(), 3);
来源：http://snm.daxiang520.top

[S41] C++：类与构造函数
来源：http://kac.ivvv.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bey.ydzc1.top

[S42] C++：继承与虚函数
来源：http://dlm.sxryk.cn

class B : public Base { public: void f() override {} };
来源：http://vbu.zhiwuduotai.top

[S43] C++：智能指针
来源：http://qsz.52xcode.cn

auto p = std::make_unique<int>(5);
来源：http://ipw.pengpengdd.cyou

[S44] C++：引用传参
来源：http://iza.hongshengwenyu.top

void inc(int &x) { ++x; }
来源：http://dht.yj202588.top

[S45] C++：lambda
来源：http://dpe.tianlin.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://vsm.sxryk.cn

[S46] C++：函数模板
来源：http://vxy.andypj.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ipr.hammf.cn

[S47] C++：结构化绑定遍历
来源：http://tpx.shangyingyoupin.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ecj.jianghu66.top

[S48] C++：逐行读文件
来源：http://mih.ivvv.top

std::ifstream in("a.txt");  std::string line;
来源：http://zlh.sysykeji.top

while (std::getline(in, line)) { }
来源：http://ska.mhx1999.top

[S49] C++：写文件
来源：http://nvt.jinyuanbaomall.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bgl.hesvh.cn

[S50] C++：格式化数字
来源：http://vyf.zhongyouzk.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wde.redwolf501.top

[S51] C++：显式类型转换
来源：http://giz.dashuyun.cn

static_cast<double>(a) / b
来源：http://spf.hfpthk.cn

[S52] C++：const 与 noexcept
来源：http://dmh.316326.xyz

int size() const noexcept { return n_; }
来源：http://asq.dianchejie.cn

[S53] C++：移动语义
来源：http://wnl.kuanghao11.cn

std::vector<int> w = std::move(v);
来源：http://obc.zhaomingkeji.xyz

[S54] C++：异常处理
来源：http://ufq.9152youxi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pfh.epnwcf.com

[S55] C++：结构化绑定
来源：http://cdc.daria6918.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yip.yvedp.cn

[S56] C++：optional
来源：http://tze.yuanzhike.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yax.xuetiantiany.cn

[S57] C++：编译期常量
来源：http://gkc.bbcook.cn

constexpr int N = 10;
来源：http://lem.sweek.top

[S58] C++：命名空间
来源：http://ldn.hnqzz.top

namespace ns { int f() { return 1; } }
来源：http://oys.jinqigufen.top

[S59] C++：静态断言
来源：http://kmk.chenlongwang.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zyl.ybcxt.top

[S60] C++：遍历并删除元素
来源：http://ekn.c1oappe.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lji.yueranfly.top

================================================================================
来源：http://vqe.havefunace.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://onx.xylfe.cn

================================================================================
来源：http://gnk.shanyushiyangkeji.top

[T01] Kotlin：Hello World
来源：http://uov.xinyue.icu

println("Hello")
来源：http://rrc.hcnkem.com

[T02] Kotlin：变量
来源：http://wml.shanyushiyangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sjy.52xcode.cn

[T03] Kotlin：字符串模板
来源：http://lty.yongpay.top

"值: $b"
来源：http://lsg.c1oappe.top

[T04] Kotlin：空安全
来源：http://akt.xuetiantiany.cn

val n: String? = null;  n?.length
来源：http://psc.zhengqikj.top

[T05] Kotlin：when 表达式
来源：http://zxi.dianchejie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://unp.gogol.net.cn

[T06] Kotlin：集合映射
来源：http://ksw.ywan-chungtsiang.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ubv.yj20258.top

[T07] Kotlin：集合过滤
来源：http://rrf.hysaishi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hup.zdbjq.cn

[T08] Kotlin：数据类
来源：http://hiv.yfazqb.com

data class User(val name: String, val age: Int)
来源：http://bny.yuanzhike.top

[T09] Kotlin：扩展函数
来源：http://ref.gogol.net.cn

fun String.exclaim() = this + "!"
来源：http://trm.sxryk.cn

[T10] Kotlin：默认参数
来源：http://zlf.9152youxi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tat.dianchejie.cn

[T11] Kotlin：协程
来源：http://sjb.snrcjt.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mto.xingfuxueyuan.xyz

[T12] Kotlin：解构声明
来源：http://dwc.daxiang520.top

val (a, b) = Pair(1, 2)
来源：http://vlj.jqgfzy.top

[T13] Kotlin：只读 Map
来源：http://akq.yj20258888.top

val m = mapOf("a" to 1)
来源：http://gev.ydzc1.top

[T14] Kotlin：循环
来源：http://mqx.kuanghao11.cn

for (i in 1..10) println(i)
来源：http://pmw.daria6918.cn

[T15] Kotlin：接口
来源：http://myi.sufxvd.cn

interface Shape { fun area(): Double }
来源：http://dwi.zhengqikj.top

[T16] Swift：Hello World
来源：http://yhn.cucudq.cn

print("Hello")
来源：http://jde.hfpthk.cn

[T17] Swift：变量与常量
来源：http://iwn.ywan-chungtsiang.top

var a = 1;  let b = 2
来源：http://bzg.xuetiantiany.cn

[T18] Swift：字符串插值
来源：http://deq.hnqzz.top

"值: \(b)"
来源：http://yio.fktsv.cn

[T19] Swift：可选绑定
来源：http://miw.xuanzx.com

if let n = opt { print(n) }
来源：http://khe.bbcook.cn

[T20] Swift：数组操作
来源：http://ogj.mhx1999.top

var a = [1, 2, 3];  a.append(4)
来源：http://yzd.nanxinkj.top

[T21] Swift：遍历
来源：http://wuq.sjlbkw.cn

for x in a { print(x) }
来源：http://rwr.ppjwa.cn

[T22] Swift：字典
来源：http://sji.aizwys.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rhw.shanyushiyangtech.top

[T23] Swift：函数
来源：http://mpp.bbcook.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://swv.guowangkeji.top

[T24] Swift：闭包
来源：http://zub.jiagoushi.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://izf.gotoacloud.top

[T25] Swift：结构体
来源：http://mdc.yueranfly.top

struct P { var x: Int }
来源：http://fxs.zhoulong.xyz

[T26] Swift：类与重写
来源：http://hsx.tianlin.xyz

class A: Base { override func f() {} }
来源：http://ucz.fehbvm.com

[T27] Swift：错误处理
来源：http://xsi.gotoacloud.top

do { try f() } catch { print(error) }
来源：http://wbi.zdqjudy.top

[T28] Swift：枚举
来源：http://xeq.c1oappe.top

enum Color { case red, green }
来源：http://nat.cdnleiting.top

[T29] Swift：guard 提前返回
来源：http://kyk.xziqi.cn

guard let x = opt else { return }
来源：http://yjz.quarkkingdee.top

[T30] Swift：协议
来源：http://tcr.ydjk.org.cn

protocol Shape { func area() -> Double }
来源：http://plm.hammf.cn

[T31] Lua：Hello World
来源：http://sdm.sufxvd.cn

print("Hello")
来源：http://fxb.jyoumei.cn

[T32] Lua：局部变量
来源：http://qsp.jyoumei.cn

local a = 1
来源：http://fqu.ppjwa.cn

[T33] Lua：表（数组）
来源：http://sra.hnxiangtu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://mby.xziqi.cn

[T34] Lua：遍历表
来源：http://vto.xuanzx.com

for i, v in ipairs(t) do print(i, v) end
来源：http://ybt.ppjwa.cn

[T35] Lua：字典表
来源：http://rev.mhx1999.top

local d = { a = 1 };  d.b = 2
来源：http://ubr.vqdsnc.cn

[T36] Lua：函数
来源：http://ymw.xylfe.cn

function add(a, b) return a + b end
来源：http://ddi.ydzc1.top

[T37] Lua：字符串拼接
来源：http://den.zhoulong.xyz

"a" .. "b"
来源：http://kxm.chenlongwang.top

[T38] Lua：条件
来源：http://cou.nwbrower.top

if x > 0 then print("正") end
来源：http://qsu.sxryk.cn

[T39] Lua：模式匹配
来源：http://yro.hfpthk.cn

string.find(s, "%d+")
来源：http://tdv.sjlbkw.cn

[T40] Lua：元表
来源：http://skb.zhijiandao.cn

setmetatable({}, { __index = base })
来源：http://szm.jianghu66.top

[T41] Perl：Hello World
来源：http://vto.aizwys.cn

print "Hello\n";
来源：http://otz.kuanghao11.cn

[T42] Perl：变量类型
来源：http://ieh.316326.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zir.hammf.cn

[T43] Perl：字符串插值
来源：http://yum.c1oappe.top

"值: $a"
来源：http://gal.zhixingplan.top

[T44] Perl：条件
来源：http://vxb.sysykeji.top

if ($a > 0) { print "正"; }
来源：http://vjb.fengsongda.top

[T45] Perl：数组遍历
来源：http://krc.nwbrower.top

for my $x (@arr) { print $x; }
来源：http://tfw.redwolf501.top

[T46] Perl：哈希操作
来源：http://gif.yfazqb.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mge.sysykeji.top

[T47] Perl：正则捕获
来源：http://wca.snrcjt.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://npt.cdnleiting.top

[T48] Perl：正则替换
来源：http://zoo.jlsjyb.cn

$s =~ s/old/new/g;
来源：http://dcd.shzxlz.cn

[T49] Perl：函数
来源：http://sre.iojbl.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cnc.mhx1999.top

[T50] Perl：逐行读文件
来源：http://ttx.zycfv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ode.ppjwa.cn

while (my $line = <$fh>) { print $line; }
来源：http://hgs.zhaomingkeji.xyz

[T51] Scala：Hello World
来源：http://gfm.havefunace.top

println("Hello")
来源：http://uxn.0kj1m.cn

[T52] Scala：变量
来源：http://wxm.shanyushiyangkeji.top

val a = 1;  var b = 2
来源：http://tce.ctjpmb.com

[T53] Scala：字符串插值
来源：http://lun.ctjpmb.com

s"值: $b"
来源：http://oxk.tanke756.top

[T54] Scala：集合映射
来源：http://ory.zhaomingkeji.xyz

List(1, 2, 3).map(_ * 2)
来源：http://bwc.pycfn.com

[T55] Scala：集合过滤
来源：http://psy.yvedp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://npr.shanyushiyangtech.top

[T56] Scala：样例类
来源：http://uth.shuidangran.top

case class User(name: String, age: Int)
来源：http://uvs.jqgfzy.top

[T57] Scala：模式匹配
来源：http://oxq.daxiang520.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://pni.gzhubu.top

[T58] Scala：函数定义
来源：http://ace.dashuyun.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hpz.vqdsnc.cn

[T59] Scala：循环
来源：http://ieu.birdmap.top

for (i <- 1 to 10) println(i)
来源：http://fjs.feifeiyinyue.top

[T60] Scala：折叠
来源：http://bix.cashguo.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cuy.ivvv.top

================================================================================
来源：http://hiu.hysaishi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bzh.pengpengdd.cyou

================================================================================
来源：http://azn.nwbrower.top

[U01] Py：创建虚拟环境
来源：http://rvx.xuetiantiany.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sbh.tianlin.xyz

[U02] Py：导出 / 安装依赖
来源：http://fhw.xingfuxueyuan.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://elj.yvedp.cn

[U03] Py：加载 .env 配置
来源：http://kdb.gaohongyu789.top

from dotenv import load_dotenv; load_dotenv()
来源：http://msv.yonumen.top

[U04] Py：变量调试打印
来源：http://zqf.guannengcc.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fwx.hysaishi.cn

[U05] Py：列表去重且保序
来源：http://zcz.mhx1999.top

list(dict.fromkeys(arr))
来源：http://ghg.sjlbkw.cn

[U06] Py：合并两个字典
来源：http://eno.hammf.cn

{**a, **b}
来源：http://avk.fzhhl.top

[U07] Py：反转字典键值
来源：http://kya.bbcook.cn

{v: k for k, v in d.items()}
来源：http://rdw.redwolf501.top

[U08] Py：展平二维列表
来源：http://nku.shuidangran.top

[y for x in nested for y in x]
来源：http://xll.guannengcc.top

[U09] Py：字典取最大值的键
来源：http://wpd.chenzaomai.com

max(d, key=d.get)
来源：http://ikp.smart0.xyz

[U10] Py：按值排序字典
来源：http://gmn.hnqzz.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pxx.pengpengdd.cyou

[U11] Py：生成器表达式
来源：http://flo.shuidangran.top

(x * 2 for x in arr)
来源：http://yva.hfpthk.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hru.snrcjt.cn

Counter(arr).most_common(3)
来源：http://yoq.redwolf501.top

[U13] Py：固定长度队列
来源：http://abm.zhoulong.xyz

deque(maxlen=10)
来源：http://vcs.feifeiyinyue.top

[U14] Py：分组收集到列表
来源：http://hwn.xingfuxueyuan.xyz

defaultdict(list)
来源：http://uso.52xcode.cn

[U15] Py：高精度计时
来源：http://jbb.jianghu66.top

t = time.perf_counter()
来源：http://ngq.cashguo.top

[U16] Py：命令行参数解析
来源：http://oah.svipenyu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jld.c1oappe.top


<!-- 参考信息 -->