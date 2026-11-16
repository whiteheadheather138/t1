代发 wailian999

read -rp "请输入: " ans
来源：http://ool.yanxiufei.cn

[R78] 交互式菜单
来源：http://ztc.jyoumei.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://phf.zhijiandao.cn

[R79] 解析命令行选项
来源：http://ehw.jinyuanbaomall.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nmp.zhixingplan.top

[R80] 查看脚本执行耗时
来源：http://znm.fengsongda.top

time ./run.sh
来源：http://fwp.pengpengdd.cyou

================================================================================
来源：http://xtf.cucudq.cn

S. C / C++ 专题
来源：http://spy.xinyue.icu

================================================================================
来源：http://fnf.jinqigfzy.top

[S01] C：Hello World
来源：http://bag.cdnleiting.top

#include <stdio.h>
来源：http://wkd.daxiang520.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gvx.xuanzx.com

[S02] C：变量与格式化输出
来源：http://yyb.yuanzhike.top

int a = 10; printf("%d\n", a);
来源：http://cln.hcnkem.com

[S03] C：读入整数
来源：http://jiz.fehbvm.com

int x; scanf("%d", &x);
来源：http://eys.9152youxi.cn

[S04] C：字符串复制
来源：http://clf.jyoumei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://evv.cucudq.cn

[S05] C：字符串长度
来源：http://rpa.hcnkem.com

strlen(s)
来源：http://tbq.ehwqpu.com

[S06] C：字符串比较
来源：http://gef.sysykeji.top

strcmp(a, b) == 0
来源：http://yxq.cashguo.top

[S07] C：数组遍历求和
来源：http://sqy.gotoacloud.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://exz.yuanzhike.top

[S08] C：动态内存分配与释放
来源：http://gsz.ydjk.org.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xst.52xcode.cn

[S09] C：结构体定义与初始化
来源：http://fpo.vehdjk.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ftd.zhiwuduotai.top

[S10] C：指针与解引用
来源：http://shl.hysaishi.cn

int *p = &a;  *p = 5;
来源：http://hjl.cheryme.top

[S11] C：逐行读文件
来源：http://phg.316326.xyz

FILE *f = fopen("a.txt", "r");
来源：http://shd.hnqzz.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://rlb.zhaomingkeji.xyz

fclose(f);
来源：http://amy.zdqjudy.top

[S12] C：写文件
来源：http://qsj.daxiang520.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ysw.jinyuanbaomall.cn

[S13] C：宏定义
来源：http://gmg.zhaomingkeji.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gef.shuidangran.top

[S14] C：枚举
来源：http://vxi.birdmap.top

enum Color { RED, GREEN, BLUE };
来源：http://ynp.tarul.cn

[S15] C：类型转换
来源：http://vpw.xziqi.cn

(double) a / b
来源：http://bqd.sysykeji.top

[S16] C：位操作置位
来源：http://uii.ppjwa.cn

x |= (1 << 3);
来源：http://fad.vehdjk.com

[S17] C：安全拼接字符串
来源：http://lhp.hfpthk.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lev.shanyushiyangtech.top

[S18] C：命令行参数
来源：http://jux.snrcjt.cn

int main(int argc, char **argv)
来源：http://cqi.tian-w.cn

[S19] C：快速排序
来源：http://xzp.aibaodan.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dxg.zdqjudy.top

[S20] C：二分查找
来源：http://uwp.nanxuanxn.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mwu.zycfv.cn

[S21] C：字符类别判断
来源：http://cng.chenlongwang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vwm.havefunace.top

[S22] C：字符串转数字
来源：http://tke.snrcjt.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qqk.yongpay.top

[S23] C：随机数
来源：http://qee.hongshengwenyu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://abt.ehwqpu.com

[S24] C：获取本地时间
来源：http://eni.jlsjyb.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fqp.hysaishi.cn

[S25] C：内存拷贝
来源：http://wqr.dashuyun.cn

memcpy(dst, src, n);
来源：http://gjx.aibaodan.cn

[S26] C：内存清零
来源：http://ldi.yuanzhike.top

memset(a, 0, sizeof a);
来源：http://bby.cashguo.top

[S27] C：定义常量
来源：http://doy.haohaochexian.top

const double PI = 3.14159;
来源：http://fvg.shangyingyoupin.top

[S28] C：静态变量
来源：http://irz.hcnkem.com

static int counter = 0;
来源：http://shm.hnqzz.top

[S29] C：变参函数
来源：http://erd.havefunace.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xbw.shanyushiyangkeji.top

[S30] C：头文件保护
来源：http://ncy.zhongyouzk.top

#ifndef X_H
来源：http://sna.zycfv.cn

#define X_H
来源：http://wpk.cqqwz.cn

#endif
来源：http://zea.gzhubu.top

[S31] C++：Hello World
来源：http://amq.bjfxy.top

#include <iostream>
来源：http://kqk.jinghuilouyu.cn

int main() { std::cout << "Hello\n"; }
来源：http://uev.hcnkem.com

[S32] C++：字符串
来源：http://rtw.gogol.net.cn

std::string s = "hi";  s += "!";
来源：http://zgi.birdmap.top

[S33] C++：vector 增删
来源：http://eib.aizwys.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hyk.yj20258.top

[S34] C++：遍历 vector
来源：http://qcv.chenzaomai.com

for (auto &x : v) { std::cout << x; }
来源：http://zzl.vehdjk.com

[S35] C++：map
来源：http://fjc.yvedp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hrq.jqgfzy.top

[S36] C++：unordered_map
来源：http://lmq.dianchejie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vit.nwbrower.top

[S37] C++：set
来源：http://rgc.dianchejie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://taq.yj202588.top

[S38] C++：排序
来源：http://oqr.zhixingplan.top

std::sort(v.begin(), v.end());
来源：http://een.jinqigfzy.top

[S39] C++：自定义比较器排序
来源：http://bqn.kuanghao11.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://faj.redwolf501.top

[S40] C++：查找元素
来源：http://srb.zhoulong.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://avm.hongshengwenyu.top

[S41] C++：类与构造函数
来源：http://pen.dianchejie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nhd.feifeiyinyue.top

[S42] C++：继承与虚函数
来源：http://slc.chenlongwang.top

class B : public Base { public: void f() override {} };
来源：http://fsn.wangshuangyany.cn

[S43] C++：智能指针
来源：http://xwc.yonumen.top

auto p = std::make_unique<int>(5);
来源：http://dmw.xingfuxueyuan.xyz

[S44] C++：引用传参
来源：http://xjm.hnqzz.top

void inc(int &x) { ++x; }
来源：http://zwd.aizwys.cn

[S45] C++：lambda
来源：http://kfq.shzxlz.cn

auto add = [](int a, int b) { return a + b; };
来源：http://khg.aizwys.cn

[S46] C++：函数模板
来源：http://ihv.redwolf501.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jee.kuanghao11.cn

[S47] C++：结构化绑定遍历
来源：http://yro.vqdsnc.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dwc.hywenlv.cn

[S48] C++：逐行读文件
来源：http://woj.hnxiangtu.top

std::ifstream in("a.txt");  std::string line;
来源：http://ikr.cheryme.top

while (std::getline(in, line)) { }
来源：http://udi.gotoacloud.top

[S49] C++：写文件
来源：http://hzn.jianghu66.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://txu.yanxiufei.cn

[S50] C++：格式化数字
来源：http://klw.fehbvm.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://aiv.mhx1999.top

[S51] C++：显式类型转换
来源：http://jbq.zhaomingkeji.xyz

static_cast<double>(a) / b
来源：http://ipa.dashuyun.cn

[S52] C++：const 与 noexcept
来源：http://fdf.redwolf501.top

int size() const noexcept { return n_; }
来源：http://poq.fanxiaobao.xyz

[S53] C++：移动语义
来源：http://gqz.smart0.xyz

std::vector<int> w = std::move(v);
来源：http://ond.sweek.top

[S54] C++：异常处理
来源：http://dzs.daria6918.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://byx.dianchejie.cn

[S55] C++：结构化绑定
来源：http://vzv.havefunace.top

auto [a, b] = std::make_pair(1, 2);
来源：http://bdk.9152youxi.cn

[S56] C++：optional
来源：http://hkx.uphjek.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://naw.dashuyun.cn

[S57] C++：编译期常量
来源：http://rhe.fehbvm.com

constexpr int N = 10;
来源：http://wyk.gzhubu.top

[S58] C++：命名空间
来源：http://bmb.yvedp.cn

namespace ns { int f() { return 1; } }
来源：http://axd.jinqigufen.top

[S59] C++：静态断言
来源：http://npc.jianghu66.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bjd.pengpengdd.cyou

[S60] C++：遍历并删除元素
来源：http://frs.iojbl.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://usx.havefunace.top

================================================================================
来源：http://xam.hammf.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vkc.smart0.xyz

================================================================================
来源：http://htb.yuxming.cn

[T01] Kotlin：Hello World
来源：http://egg.iojbl.cn

println("Hello")
来源：http://urc.ybcxt.top

[T02] Kotlin：变量
来源：http://fqe.andypj.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://myc.sysykeji.top

[T03] Kotlin：字符串模板
来源：http://wwo.hywenlv.cn

"值: $b"
来源：http://qph.zdqjudy.top

[T04] Kotlin：空安全
来源：http://efn.gogol.net.cn

val n: String? = null;  n?.length
来源：http://ngg.feifeiyinyue.top

[T05] Kotlin：when 表达式
来源：http://dso.redwolf501.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lbp.jyoumei.cn

[T06] Kotlin：集合映射
来源：http://dqt.tianlin.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://gwa.jlsjyb.cn

[T07] Kotlin：集合过滤
来源：http://agb.gotoacloud.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://jra.ehwqpu.com

[T08] Kotlin：数据类
来源：http://zlr.dianchejie.cn

data class User(val name: String, val age: Int)
来源：http://tuf.sufxvd.cn

[T09] Kotlin：扩展函数
来源：http://yar.xuetiantiany.cn

fun String.exclaim() = this + "!"
来源：http://ady.quarkkingdee.top

[T10] Kotlin：默认参数
来源：http://bgp.yj20258888.top

fun greet(name: String = "World") = "Hi $name"
来源：http://gly.zhiwuduotai.top

[T11] Kotlin：协程
来源：http://hht.smart0.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://wel.hongshengwenyu.top

[T12] Kotlin：解构声明
来源：http://nbp.guannengcc.top

val (a, b) = Pair(1, 2)
来源：http://omq.shangyingyoupin.top

[T13] Kotlin：只读 Map
来源：http://vym.zhiwuduotai.top

val m = mapOf("a" to 1)
来源：http://cls.yongpay.top

[T14] Kotlin：循环
来源：http://ena.zdqjudy.top

for (i in 1..10) println(i)
来源：http://zvg.fktsv.cn

[T15] Kotlin：接口
来源：http://ytv.tanke756.top

interface Shape { fun area(): Double }
来源：http://xce.chenjidiqi.icu

[T16] Swift：Hello World
来源：http://jiv.pengpengdd.cyou

print("Hello")
来源：http://ner.aizwys.cn

[T17] Swift：变量与常量
来源：http://nwx.jinyuanbaomall.cn

var a = 1;  let b = 2
来源：http://ykn.fehbvm.com

[T18] Swift：字符串插值
来源：http://uzv.yvedp.cn

"值: \(b)"
来源：http://nua.birdmap.top

[T19] Swift：可选绑定
来源：http://fgp.yanxiufei.cn

if let n = opt { print(n) }
来源：http://xfa.zhiwuduotai.top

[T20] Swift：数组操作
来源：http://uex.wangdashe.top

var a = [1, 2, 3];  a.append(4)
来源：http://kik.tarul.cn

[T21] Swift：遍历
来源：http://dgl.c1oappe.top

for x in a { print(x) }
来源：http://ywb.andypj.xyz

[T22] Swift：字典
来源：http://xid.guowangkeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://ugf.shuidangran.top

[T23] Swift：函数
来源：http://tzd.chenlongwang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ftq.yonumen.top

[T24] Swift：闭包
来源：http://kji.chenlongwang.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://mhm.hammf.cn

[T25] Swift：结构体
来源：http://inl.zhixingplan.top

struct P { var x: Int }
来源：http://upo.quarkkingdee.top

[T26] Swift：类与重写
来源：http://lou.cheryme.top

class A: Base { override func f() {} }
来源：http://pvr.gotoacloud.top

[T27] Swift：错误处理
来源：http://tyg.cucudq.cn

do { try f() } catch { print(error) }
来源：http://hhr.shzxlz.cn

[T28] Swift：枚举
来源：http://xxu.shangyingyoupin.top

enum Color { case red, green }
来源：http://jcs.yuanzhike.top

[T29] Swift：guard 提前返回
来源：http://jvp.daxiang520.top

guard let x = opt else { return }
来源：http://xyu.gaohongyu789.top

[T30] Swift：协议
来源：http://syh.hesvh.cn

protocol Shape { func area() -> Double }
来源：http://wtp.xylfe.cn

[T31] Lua：Hello World
来源：http://hat.gzhubu.top

print("Hello")
来源：http://epi.gotoacloud.top

[T32] Lua：局部变量
来源：http://wyp.mhx1999.top

local a = 1
来源：http://xdi.daxiang520.top

[T33] Lua：表（数组）
来源：http://hvc.yuxming.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rpg.guannengcc.top

[T34] Lua：遍历表
来源：http://gte.bbcook.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lqp.yvedp.cn

[T35] Lua：字典表
来源：http://kxu.ctjpmb.com

local d = { a = 1 };  d.b = 2
来源：http://wcr.aibaodan.cn

[T36] Lua：函数
来源：http://hwj.yuanzhike.top

function add(a, b) return a + b end
来源：http://kwg.tanke756.top

[T37] Lua：字符串拼接
来源：http://ypb.0kj1m.cn

"a" .. "b"
来源：http://gcl.fanxiaobao.xyz

[T38] Lua：条件
来源：http://ean.ydzc1.top

if x > 0 then print("正") end
来源：http://aqu.epnwcf.com

[T39] Lua：模式匹配
来源：http://xoy.ywan-chungtsiang.top

string.find(s, "%d+")
来源：http://tdz.hcnkem.com

[T40] Lua：元表
来源：http://ebr.zdbjq.cn

setmetatable({}, { __index = base })
来源：http://tpw.zhoulong.xyz

[T41] Perl：Hello World
来源：http://cnp.hammf.cn

print "Hello\n";
来源：http://ckg.bjfxy.top

[T42] Perl：变量类型
来源：http://fbr.xingfuxueyuan.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ges.sxryk.cn

[T43] Perl：字符串插值
来源：http://zge.zhoulong.xyz

"值: $a"
来源：http://tvn.zhengqikj.top

[T44] Perl：条件
来源：http://uec.bbcook.cn

if ($a > 0) { print "正"; }
来源：http://kpy.gzhubu.top

[T45] Perl：数组遍历
来源：http://lkk.cqqwz.cn

for my $x (@arr) { print $x; }
来源：http://rje.9152youxi.cn

[T46] Perl：哈希操作
来源：http://hhy.ctjpmb.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://atq.bbcook.cn

[T47] Perl：正则捕获
来源：http://oan.ehwqpu.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://qcd.zhongyouzk.top

[T48] Perl：正则替换
来源：http://adn.316326.xyz

$s =~ s/old/new/g;
来源：http://rhf.daxiang520.top

[T49] Perl：函数
来源：http://icm.316326.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://biv.yonumen.top

[T50] Perl：逐行读文件
来源：http://iwo.meibo888.top

open my $fh, "<", "a.txt" or die $!;
来源：http://dsq.guannengcc.top

while (my $line = <$fh>) { print $line; }
来源：http://fcs.haohaochexian.top

[T51] Scala：Hello World
来源：http://yrp.zhiwuduotai.top

println("Hello")
来源：http://uja.sufxvd.cn

[T52] Scala：变量
来源：http://sdc.haohaochexian.top

val a = 1;  var b = 2
来源：http://kqi.yangfankeji.com

[T53] Scala：字符串插值
来源：http://kuu.hammf.cn

s"值: $b"
来源：http://goh.yuxming.cn

[T54] Scala：集合映射
来源：http://ugo.dashuyun.cn

List(1, 2, 3).map(_ * 2)
来源：http://tiy.cdnleiting.top

[T55] Scala：集合过滤
来源：http://qxq.hcnkem.com

List(1, 2, 3).filter(_ > 1)
来源：http://blx.jinyuanbaomall.cn

[T56] Scala：样例类
来源：http://tff.jyoumei.cn

case class User(name: String, age: Int)
来源：http://cul.sweek.top

[T57] Scala：模式匹配
来源：http://cll.zdqjudy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vxc.andypj.xyz

[T58] Scala：函数定义
来源：http://tia.zhijiandao.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mfz.andypj.xyz

[T59] Scala：循环
来源：http://rbr.xingfuxueyuan.xyz

for (i <- 1 to 10) println(i)
来源：http://awa.dashuyun.cn

[T60] Scala：折叠
来源：http://ysf.shanyushiyangtech.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://irr.sjlbkw.cn

================================================================================
来源：http://dpg.dashuyun.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wxq.yongpay.top

================================================================================
来源：http://ipl.yuanzhike.top

[U01] Py：创建虚拟环境
来源：http://tei.fehbvm.com

python -m venv .venv && source .venv/bin/activate
来源：http://lab.ywan-chungtsiang.top

[U02] Py：导出 / 安装依赖
来源：http://zrb.0kj1m.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vdn.zhaomingkeji.xyz

[U03] Py：加载 .env 配置
来源：http://lrq.ivvv.top

from dotenv import load_dotenv; load_dotenv()
来源：http://vnq.cheryme.top

[U04] Py：变量调试打印
来源：http://upg.fengsongda.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hvz.hysaishi.cn

[U05] Py：列表去重且保序
来源：http://ycl.sysykeji.top

list(dict.fromkeys(arr))
来源：http://mvs.cdnleiting.top

[U06] Py：合并两个字典
来源：http://oaa.jyoumei.cn

{**a, **b}
来源：http://idl.tianlin.xyz

[U07] Py：反转字典键值
来源：http://wgs.ywan-chungtsiang.top

{v: k for k, v in d.items()}
来源：http://uxs.yuanzhike.top

[U08] Py：展平二维列表
来源：http://jhm.cashguo.top

[y for x in nested for y in x]
来源：http://chm.0kj1m.cn

[U09] Py：字典取最大值的键
来源：http://lhb.quarkkingdee.top

max(d, key=d.get)
来源：http://xrj.chenjidiqi.icu

[U10] Py：按值排序字典
来源：http://mgm.zdqjudy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://owf.gzhubu.top

[U11] Py：生成器表达式
来源：http://npn.ppjwa.cn

(x * 2 for x in arr)
来源：http://bdd.mhx1999.top

[U12] Py：取出现最多的 3 个元素
来源：http://jrj.chenzaomai.com

Counter(arr).most_common(3)
来源：http://dqo.yuanzhike.top

[U13] Py：固定长度队列
来源：http://yzx.daxiang520.top

deque(maxlen=10)
来源：http://uoq.shzxlz.cn

[U14] Py：分组收集到列表
来源：http://wok.hnqzz.top

defaultdict(list)
来源：http://olt.smart0.xyz

[U15] Py：高精度计时
来源：http://epe.hnqzz.top

t = time.perf_counter()
来源：http://syh.yj20258.top

[U16] Py：命令行参数解析
来源：http://hpf.daria6918.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rox.chenzaomai.com

[U17] Py：初始化日志
来源：http://qao.0kj1m.cn

logging.basicConfig(level=logging.INFO)
来源：http://opd.jlsjyb.cn

[U18] Py：预编译正则
来源：http://mye.gzhubu.top

pat = re.compile(r"\d+")
来源：http://cww.pengpengdd.cyou


<!-- 参考信息 -->