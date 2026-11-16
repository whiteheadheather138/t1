代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://vdo.kuanghao11.cn

[R76] 使用临时文件
来源：http://elk.feifeiyinyue.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nxy.fanxiaobao.xyz

[R77] 读取用户输入
来源：http://eyd.zhaomingkeji.xyz

read -rp "请输入: " ans
来源：http://fxz.52xcode.cn

[R78] 交互式菜单
来源：http://phy.smart0.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://dcw.yongpay.top

[R79] 解析命令行选项
来源：http://ktm.ivvv.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hav.quarkkingdee.top

[R80] 查看脚本执行耗时
来源：http://uwy.daxiang520.top

time ./run.sh
来源：http://kdu.shuidangran.top

================================================================================
来源：http://tbc.gaohongyu789.top

S. C / C++ 专题
来源：http://olw.zhixingplan.top

================================================================================
来源：http://mve.chenjidiqi.icu

[S01] C：Hello World
来源：http://kdi.tianlin.xyz

#include <stdio.h>
来源：http://ilo.gogol.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rcr.tanke756.top

[S02] C：变量与格式化输出
来源：http://bwr.nwbrower.top

int a = 10; printf("%d\n", a);
来源：http://cau.aibaodan.cn

[S03] C：读入整数
来源：http://mba.sxryk.cn

int x; scanf("%d", &x);
来源：http://zfi.ybcxt.top

[S04] C：字符串复制
来源：http://zqk.ydjk.org.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yca.yj20258888.top

[S05] C：字符串长度
来源：http://yzh.cqqwz.cn

strlen(s)
来源：http://ojd.redwolf501.top

[S06] C：字符串比较
来源：http://ksn.vqdsnc.cn

strcmp(a, b) == 0
来源：http://owa.xuanzx.com

[S07] C：数组遍历求和
来源：http://zhd.tanke756.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vph.yj20258.top

[S08] C：动态内存分配与释放
来源：http://aiy.fzhhl.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://meo.xingfuxueyuan.xyz

[S09] C：结构体定义与初始化
来源：http://vhy.yongpay.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mwv.chenlongwang.top

[S10] C：指针与解引用
来源：http://nvo.52xcode.cn

int *p = &a;  *p = 5;
来源：http://ath.ydzc1.top

[S11] C：逐行读文件
来源：http://hlg.tarul.cn

FILE *f = fopen("a.txt", "r");
来源：http://vwm.yongpay.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://gmt.hongshengwenyu.top

fclose(f);
来源：http://tny.aibaodan.cn

[S12] C：写文件
来源：http://eig.ywan-chungtsiang.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uwn.yongpay.top

[S13] C：宏定义
来源：http://apq.gotoacloud.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xym.zhongyouzk.top

[S14] C：枚举
来源：http://bbn.jiagoushi.top

enum Color { RED, GREEN, BLUE };
来源：http://qjv.andypj.xyz

[S15] C：类型转换
来源：http://ill.snrcjt.cn

(double) a / b
来源：http://cnj.mhx1999.top

[S16] C：位操作置位
来源：http://bqc.ctjpmb.com

x |= (1 << 3);
来源：http://ray.bjfxy.top

[S17] C：安全拼接字符串
来源：http://bsq.yanxiufei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fsj.zhijiandao.cn

[S18] C：命令行参数
来源：http://qle.ehwqpu.com

int main(int argc, char **argv)
来源：http://zih.hammf.cn

[S19] C：快速排序
来源：http://bsi.nwbrower.top

qsort(a, n, sizeof(int), cmp);
来源：http://kli.yj202588.top

[S20] C：二分查找
来源：http://tes.yuanzhike.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hkv.hywenlv.cn

[S21] C：字符类别判断
来源：http://ebt.snrcjt.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yfh.svipenyu.cn

[S22] C：字符串转数字
来源：http://djh.tianlin.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://sco.guannengcc.top

[S23] C：随机数
来源：http://ean.pengpengdd.cyou

srand(time(NULL));  int r = rand() % 100;
来源：http://tue.iojbl.cn

[S24] C：获取本地时间
来源：http://gtc.hfpthk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dev.jqgfzy.top

[S25] C：内存拷贝
来源：http://yam.sysykeji.top

memcpy(dst, src, n);
来源：http://bpv.haohaochexian.top

[S26] C：内存清零
来源：http://gtt.birdmap.top

memset(a, 0, sizeof a);
来源：http://tla.hysaishi.cn

[S27] C：定义常量
来源：http://ejo.svipenyu.cn

const double PI = 3.14159;
来源：http://nwb.cqqwz.cn

[S28] C：静态变量
来源：http://hjn.sufxvd.cn

static int counter = 0;
来源：http://nvf.hfpthk.cn

[S29] C：变参函数
来源：http://ryh.tian-w.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zab.ppjwa.cn

[S30] C：头文件保护
来源：http://tmr.yj20258.top

#ifndef X_H
来源：http://kza.guannengcc.top

#define X_H
来源：http://lwe.xuetiantiany.cn

#endif
来源：http://qhb.fzhhl.top

[S31] C++：Hello World
来源：http://inl.quarkkingdee.top

#include <iostream>
来源：http://cwm.aibaodan.cn

int main() { std::cout << "Hello\n"; }
来源：http://tfh.ctjpmb.com

[S32] C++：字符串
来源：http://kxe.shuidangran.top

std::string s = "hi";  s += "!";
来源：http://fwm.daxiang520.top

[S33] C++：vector 增删
来源：http://giu.jinghuilouyu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://brs.gogol.net.cn

[S34] C++：遍历 vector
来源：http://cxu.svipenyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://pgb.zhijiandao.cn

[S35] C++：map
来源：http://ssn.fengsongda.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qcm.zycfv.cn

[S36] C++：unordered_map
来源：http://gkh.fehbvm.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://eqz.shanyushiyangtech.top

[S37] C++：set
来源：http://hwi.yangfankeji.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vpw.bbcook.cn

[S38] C++：排序
来源：http://kxu.vqdsnc.cn

std::sort(v.begin(), v.end());
来源：http://jcg.fehbvm.com

[S39] C++：自定义比较器排序
来源：http://yqj.zhengqikj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ptf.yj202588.top

[S40] C++：查找元素
来源：http://jjn.zhoulong.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hjg.gzhubu.top

[S41] C++：类与构造函数
来源：http://dtn.sweek.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lav.pycfn.com

[S42] C++：继承与虚函数
来源：http://cqe.wangshuangyany.cn

class B : public Base { public: void f() override {} };
来源：http://tcw.ehwqpu.com

[S43] C++：智能指针
来源：http://inr.cheryme.top

auto p = std::make_unique<int>(5);
来源：http://qdh.mhx1999.top

[S44] C++：引用传参
来源：http://oja.ybcxt.top

void inc(int &x) { ++x; }
来源：http://wbc.jiagoushi.top

[S45] C++：lambda
来源：http://reg.redwolf501.top

auto add = [](int a, int b) { return a + b; };
来源：http://wsy.aibaodan.cn

[S46] C++：函数模板
来源：http://fwl.smart0.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rba.feifeiyinyue.top

[S47] C++：结构化绑定遍历
来源：http://hkb.hfpthk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://efp.zdqjudy.top

[S48] C++：逐行读文件
来源：http://eix.c1oappe.top

std::ifstream in("a.txt");  std::string line;
来源：http://par.ehwqpu.com

while (std::getline(in, line)) { }
来源：http://ukm.sufxvd.cn

[S49] C++：写文件
来源：http://wwd.hcnkem.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://npk.sufxvd.cn

[S50] C++：格式化数字
来源：http://xvi.zhixingplan.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://csi.9152youxi.cn

[S51] C++：显式类型转换
来源：http://rcz.xylfe.cn

static_cast<double>(a) / b
来源：http://gvc.ydjk.org.cn

[S52] C++：const 与 noexcept
来源：http://qvb.sysykeji.top

int size() const noexcept { return n_; }
来源：http://jvw.yueranfly.top

[S53] C++：移动语义
来源：http://fiz.jiagoushi.top

std::vector<int> w = std::move(v);
来源：http://jeu.sjlbkw.cn

[S54] C++：异常处理
来源：http://owm.0kj1m.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gvb.52xcode.cn

[S55] C++：结构化绑定
来源：http://jgf.haohaochexian.top

auto [a, b] = std::make_pair(1, 2);
来源：http://sax.uphjek.com

[S56] C++：optional
来源：http://gqm.meibo888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kem.zdqjudy.top

[S57] C++：编译期常量
来源：http://ciy.xylfe.cn

constexpr int N = 10;
来源：http://xcx.dashuyun.cn

[S58] C++：命名空间
来源：http://ret.yanxiufei.cn

namespace ns { int f() { return 1; } }
来源：http://bnb.xingfuxueyuan.xyz

[S59] C++：静态断言
来源：http://llw.bjfxy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://icj.hesvh.cn

[S60] C++：遍历并删除元素
来源：http://voo.hysaishi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qdi.hnqzz.top

================================================================================
来源：http://ajr.snrcjt.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://trd.zhoulong.xyz

================================================================================
来源：http://dnt.yanxiufei.cn

[T01] Kotlin：Hello World
来源：http://qcj.yj202588.top

println("Hello")
来源：http://ktc.aibaodan.cn

[T02] Kotlin：变量
来源：http://stz.sufxvd.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ziz.hnqzz.top

[T03] Kotlin：字符串模板
来源：http://cyx.9152youxi.cn

"值: $b"
来源：http://lks.jinqigfzy.top

[T04] Kotlin：空安全
来源：http://kca.yfazqb.com

val n: String? = null;  n?.length
来源：http://ahv.zhongyouzk.top

[T05] Kotlin：when 表达式
来源：http://rsr.gaohongyu789.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://orx.tanke756.top

[T06] Kotlin：集合映射
来源：http://qvz.zhengqikj.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qsn.yfazqb.com

[T07] Kotlin：集合过滤
来源：http://hzi.haohaochexian.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://uvf.yj202588.top

[T08] Kotlin：数据类
来源：http://ofz.sxryk.cn

data class User(val name: String, val age: Int)
来源：http://gac.hywenlv.cn

[T09] Kotlin：扩展函数
来源：http://cop.xuetiantiany.cn

fun String.exclaim() = this + "!"
来源：http://mrz.epnwcf.com

[T10] Kotlin：默认参数
来源：http://byz.jianghu66.top

fun greet(name: String = "World") = "Hi $name"
来源：http://jcd.xingfuxueyuan.xyz

[T11] Kotlin：协程
来源：http://mlh.pycfn.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://caq.9152youxi.cn

[T12] Kotlin：解构声明
来源：http://cyu.hesvh.cn

val (a, b) = Pair(1, 2)
来源：http://wdm.hesvh.cn

[T13] Kotlin：只读 Map
来源：http://iek.shanyushiyangkeji.top

val m = mapOf("a" to 1)
来源：http://tdi.jianghu66.top

[T14] Kotlin：循环
来源：http://fwx.shangyingyoupin.top

for (i in 1..10) println(i)
来源：http://zxh.cheryme.top

[T15] Kotlin：接口
来源：http://zbp.wangshuangyany.cn

interface Shape { fun area(): Double }
来源：http://bbd.redwolf501.top

[T16] Swift：Hello World
来源：http://qlg.shzxlz.cn

print("Hello")
来源：http://xlp.ydzc1.top

[T17] Swift：变量与常量
来源：http://ixz.cqqwz.cn

var a = 1;  let b = 2
来源：http://lfu.quarkkingdee.top

[T18] Swift：字符串插值
来源：http://ixd.yj20258888.top

"值: \(b)"
来源：http://jxb.jqgufenzy.top

[T19] Swift：可选绑定
来源：http://knj.fehbvm.com

if let n = opt { print(n) }
来源：http://beo.shanyushiyangtech.top

[T20] Swift：数组操作
来源：http://stv.hnqzz.top

var a = [1, 2, 3];  a.append(4)
来源：http://pel.shangyingyoupin.top

[T21] Swift：遍历
来源：http://gzt.aizwys.cn

for x in a { print(x) }
来源：http://gbc.vqdsnc.cn

[T22] Swift：字典
来源：http://aqb.yonumen.top

var d = ["a": 1];  d["b"] = 2
来源：http://apj.zhaomingkeji.xyz

[T23] Swift：函数
来源：http://ddz.yj20258.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://peb.quarkkingdee.top

[T24] Swift：闭包
来源：http://rcj.pycfn.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://gyh.wangdashe.top

[T25] Swift：结构体
来源：http://uhv.shanyushiyangtech.top

struct P { var x: Int }
来源：http://syx.fktsv.cn

[T26] Swift：类与重写
来源：http://gih.gogol.net.cn

class A: Base { override func f() {} }
来源：http://zpa.cdnleiting.top

[T27] Swift：错误处理
来源：http://hch.jiagoushi.top

do { try f() } catch { print(error) }
来源：http://ydy.yonumen.top

[T28] Swift：枚举
来源：http://tir.tian-w.cn

enum Color { case red, green }
来源：http://qzt.smart0.xyz

[T29] Swift：guard 提前返回
来源：http://qvt.guannengcc.top

guard let x = opt else { return }
来源：http://odl.zhongyouzk.top

[T30] Swift：协议
来源：http://try.ppjwa.cn

protocol Shape { func area() -> Double }
来源：http://xud.smart0.xyz

[T31] Lua：Hello World
来源：http://hpt.hfpthk.cn

print("Hello")
来源：http://gls.jiagoushi.top

[T32] Lua：局部变量
来源：http://vmj.daria6918.cn

local a = 1
来源：http://jao.jinqigufen.top

[T33] Lua：表（数组）
来源：http://kqp.zdbjq.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://euz.nanxuanxn.top

[T34] Lua：遍历表
来源：http://wiy.0kj1m.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tkp.sxryk.cn

[T35] Lua：字典表
来源：http://ieg.zhaomingkeji.xyz

local d = { a = 1 };  d.b = 2
来源：http://qfv.hnxiangtu.top

[T36] Lua：函数
来源：http://ybd.aizwys.cn

function add(a, b) return a + b end
来源：http://xyw.nwbrower.top

[T37] Lua：字符串拼接
来源：http://sba.yfazqb.com

"a" .. "b"
来源：http://sab.xziqi.cn

[T38] Lua：条件
来源：http://yzm.wangdashe.top

if x > 0 then print("正") end
来源：http://qfz.tianlin.xyz

[T39] Lua：模式匹配
来源：http://jid.zdqjudy.top

string.find(s, "%d+")
来源：http://ing.cqqwz.cn

[T40] Lua：元表
来源：http://spe.gotoacloud.top

setmetatable({}, { __index = base })
来源：http://sqh.guannengcc.top

[T41] Perl：Hello World
来源：http://rmu.hnxiangtu.top

print "Hello\n";
来源：http://cps.guannengcc.top

[T42] Perl：变量类型
来源：http://mhx.yuxming.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cvy.jiagoushi.top

[T43] Perl：字符串插值
来源：http://swm.ppjwa.cn

"值: $a"
来源：http://djv.ydzc1.top

[T44] Perl：条件
来源：http://hzg.jqgufenzy.top

if ($a > 0) { print "正"; }
来源：http://ipy.smart0.xyz

[T45] Perl：数组遍历
来源：http://tpm.yj20258.top

for my $x (@arr) { print $x; }
来源：http://dno.havefunace.top

[T46] Perl：哈希操作
来源：http://qvb.sxryk.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xcs.daxiang520.top

[T47] Perl：正则捕获
来源：http://rjt.zhijiandao.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ltq.yuxming.cn

[T48] Perl：正则替换
来源：http://hnq.yj20258.top

$s =~ s/old/new/g;
来源：http://unh.hammf.cn

[T49] Perl：函数
来源：http://ahd.ctjpmb.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ggx.0kj1m.cn

[T50] Perl：逐行读文件
来源：http://qea.ybcxt.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hir.cheryme.top

while (my $line = <$fh>) { print $line; }
来源：http://nwu.zhongyouzk.top

[T51] Scala：Hello World
来源：http://jfe.zhengqikj.top

println("Hello")
来源：http://psy.ppjwa.cn

[T52] Scala：变量
来源：http://gej.uphjek.com

val a = 1;  var b = 2
来源：http://bol.zycfv.cn

[T53] Scala：字符串插值
来源：http://vwy.shanyushiyangtech.top

s"值: $b"
来源：http://rkl.wangshuangyany.cn

[T54] Scala：集合映射
来源：http://qei.pycfn.com

List(1, 2, 3).map(_ * 2)
来源：http://jjl.tarul.cn

[T55] Scala：集合过滤
来源：http://lsk.9152youxi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://piu.iojbl.cn

[T56] Scala：样例类
来源：http://emg.sysykeji.top

case class User(name: String, age: Int)
来源：http://fye.xingfuxueyuan.xyz

[T57] Scala：模式匹配
来源：http://bvh.jiagoushi.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://lfs.ehwqpu.com

[T58] Scala：函数定义
来源：http://yti.chenjidiqi.icu

def add(a: Int, b: Int): Int = a + b
来源：http://hff.chenzaomai.com

[T59] Scala：循环
来源：http://bsu.zhengqikj.top

for (i <- 1 to 10) println(i)
来源：http://izq.vqdsnc.cn

[T60] Scala：折叠
来源：http://fnh.guannengcc.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hmi.yvedp.cn

================================================================================
来源：http://cwy.ywan-chungtsiang.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xns.ehwqpu.com

================================================================================
来源：http://evw.quarkkingdee.top

[U01] Py：创建虚拟环境
来源：http://tbt.haohaochexian.top

python -m venv .venv && source .venv/bin/activate
来源：http://tnp.sweek.top

[U02] Py：导出 / 安装依赖
来源：http://euv.redwolf501.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vwe.jlsjyb.cn

[U03] Py：加载 .env 配置
来源：http://ifc.sjlbkw.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://yof.c1oappe.top

[U04] Py：变量调试打印
来源：http://gwz.tianlin.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blq.hongshengwenyu.top

[U05] Py：列表去重且保序
来源：http://fvr.shangyingyoupin.top

list(dict.fromkeys(arr))
来源：http://hzd.birdmap.top

[U06] Py：合并两个字典
来源：http://ops.zhaomingkeji.xyz

{**a, **b}
来源：http://qrb.cucudq.cn

[U07] Py：反转字典键值
来源：http://wtb.chenzaomai.com

{v: k for k, v in d.items()}
来源：http://zbw.gaohongyu789.top

[U08] Py：展平二维列表
来源：http://zko.wangshuangyany.cn

[y for x in nested for y in x]
来源：http://hhc.zhoulong.xyz

[U09] Py：字典取最大值的键
来源：http://fje.hfpthk.cn

max(d, key=d.get)
来源：http://tth.bbcook.cn

[U10] Py：按值排序字典
来源：http://uev.zhixingplan.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ief.redwolf501.top

[U11] Py：生成器表达式
来源：http://enc.xingfuxueyuan.xyz

(x * 2 for x in arr)
来源：http://uzx.smart0.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://iur.0kj1m.cn

Counter(arr).most_common(3)
来源：http://ddy.zhengqikj.top

[U13] Py：固定长度队列
来源：http://ijq.zdqjudy.top

deque(maxlen=10)
来源：http://ynu.wangdashe.top

[U14] Py：分组收集到列表
来源：http://uoh.jinqigufen.top

defaultdict(list)
来源：http://ajz.yuanzhike.top

[U15] Py：高精度计时
来源：http://bmv.tian-w.cn

t = time.perf_counter()
来源：http://lkm.fzhhl.top

[U16] Py：命令行参数解析
来源：http://czp.uphjek.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yff.yanxiufei.cn


<!-- 参考信息 -->