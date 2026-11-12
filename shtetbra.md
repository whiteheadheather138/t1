代发 wailian999

split -l 1000 big.log part_
来源：http://txu.birdmap.top

[R74] 批量重命名
来源：http://ixk.birdmap.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ccn.tanke756.top

[R75] 导出环境变量
来源：http://yem.ybcxt.top

export PATH="$HOME/bin:$PATH"
来源：http://ept.yfazqb.com

[R76] 使用临时文件
来源：http://mqn.hcnkem.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wmt.zycfv.cn

[R77] 读取用户输入
来源：http://aso.jqgufenzy.top

read -rp "请输入: " ans
来源：http://pac.0kj1m.cn

[R78] 交互式菜单
来源：http://fww.gzhubu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://oqj.jianghu66.top

[R79] 解析命令行选项
来源：http://qkz.fzhhl.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://edw.sxryk.cn

[R80] 查看脚本执行耗时
来源：http://kfg.jianghu66.top

time ./run.sh
来源：http://gpt.dianchejie.cn

================================================================================
来源：http://oze.jinghuilouyu.cn

S. C / C++ 专题
来源：http://fqg.shuidangran.top

================================================================================
来源：http://yqh.zycfv.cn

[S01] C：Hello World
来源：http://bqz.feifeiyinyue.top

#include <stdio.h>
来源：http://xwf.quarkkingdee.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://srv.yanxiufei.cn

[S02] C：变量与格式化输出
来源：http://dkz.jyoumei.cn

int a = 10; printf("%d\n", a);
来源：http://oqt.0kj1m.cn

[S03] C：读入整数
来源：http://bny.andypj.xyz

int x; scanf("%d", &x);
来源：http://prl.316326.xyz

[S04] C：字符串复制
来源：http://cpx.andypj.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://ucw.xuetiantiany.cn

[S05] C：字符串长度
来源：http://pwg.sjlbkw.cn

strlen(s)
来源：http://yzx.ywan-chungtsiang.top

[S06] C：字符串比较
来源：http://mru.havefunace.top

strcmp(a, b) == 0
来源：http://ntq.zhaomingkeji.xyz

[S07] C：数组遍历求和
来源：http://dea.yuxming.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wnf.cashguo.top

[S08] C：动态内存分配与释放
来源：http://mgb.sysykeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fdf.zdbjq.cn

[S09] C：结构体定义与初始化
来源：http://pxf.ydjk.org.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://epn.fehbvm.com

[S10] C：指针与解引用
来源：http://mfe.fanxiaobao.xyz

int *p = &a;  *p = 5;
来源：http://shj.zhijiandao.cn

[S11] C：逐行读文件
来源：http://dpn.smart0.xyz

FILE *f = fopen("a.txt", "r");
来源：http://mjz.dashuyun.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pmf.jqgufenzy.top

fclose(f);
来源：http://zkh.yj202588.top

[S12] C：写文件
来源：http://jjx.cashguo.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gop.nanxuanxn.top

[S13] C：宏定义
来源：http://hah.zdbjq.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wnh.ydzc1.top

[S14] C：枚举
来源：http://qft.zhixingplan.top

enum Color { RED, GREEN, BLUE };
来源：http://qwi.sjlbkw.cn

[S15] C：类型转换
来源：http://wvf.ywan-chungtsiang.top

(double) a / b
来源：http://fpc.gaohongyu789.top

[S16] C：位操作置位
来源：http://nmf.xuanzx.com

x |= (1 << 3);
来源：http://upr.zhaomingkeji.xyz

[S17] C：安全拼接字符串
来源：http://sew.nwbrower.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hjn.tianlin.xyz

[S18] C：命令行参数
来源：http://zzh.meibo888.top

int main(int argc, char **argv)
来源：http://ybj.shangyingyoupin.top

[S19] C：快速排序
来源：http://izq.zhijiandao.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nko.shanyushiyangtech.top

[S20] C：二分查找
来源：http://aku.sxryk.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jsb.bbcook.cn

[S21] C：字符类别判断
来源：http://dwo.yuxming.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xey.bjfxy.top

[S22] C：字符串转数字
来源：http://bek.chenzaomai.com

atoi("42");  strtod("3.14", NULL);
来源：http://xys.ywan-chungtsiang.top

[S23] C：随机数
来源：http://ypv.zhixingplan.top

srand(time(NULL));  int r = rand() % 100;
来源：http://wrb.hnqzz.top

[S24] C：获取本地时间
来源：http://qcv.jqgufenzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ksz.jinghuilouyu.cn

[S25] C：内存拷贝
来源：http://oxo.meibo888.top

memcpy(dst, src, n);
来源：http://vhk.cashguo.top

[S26] C：内存清零
来源：http://kko.ydzc1.top

memset(a, 0, sizeof a);
来源：http://yla.ctjpmb.com

[S27] C：定义常量
来源：http://utl.guowangkeji.top

const double PI = 3.14159;
来源：http://reb.jinyuanbaomall.cn

[S28] C：静态变量
来源：http://cyv.yonumen.top

static int counter = 0;
来源：http://fjd.hcnkem.com

[S29] C：变参函数
来源：http://cfg.hcnkem.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://msp.jianghu66.top

[S30] C：头文件保护
来源：http://ycg.hcnkem.com

#ifndef X_H
来源：http://lin.dianchejie.cn

#define X_H
来源：http://ejq.sysykeji.top

#endif
来源：http://xmp.kuanghao11.cn

[S31] C++：Hello World
来源：http://phb.gzhubu.top

#include <iostream>
来源：http://utn.daria6918.cn

int main() { std::cout << "Hello\n"; }
来源：http://sgt.cashguo.top

[S32] C++：字符串
来源：http://shk.aibaodan.cn

std::string s = "hi";  s += "!";
来源：http://wps.ydzc1.top

[S33] C++：vector 增删
来源：http://xpi.bbcook.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://huf.tian-w.cn

[S34] C++：遍历 vector
来源：http://oww.uphjek.com

for (auto &x : v) { std::cout << x; }
来源：http://wkr.xinyue.icu

[S35] C++：map
来源：http://axl.tianlin.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yyu.zdqjudy.top

[S36] C++：unordered_map
来源：http://wvp.cqqwz.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sew.zycfv.cn

[S37] C++：set
来源：http://zkj.jlsjyb.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wgo.hammf.cn

[S38] C++：排序
来源：http://ixv.aibaodan.cn

std::sort(v.begin(), v.end());
来源：http://xsr.316326.xyz

[S39] C++：自定义比较器排序
来源：http://mpy.xingfuxueyuan.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cop.nanxinkj.top

[S40] C++：查找元素
来源：http://tye.xziqi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://slh.sjlbkw.cn

[S41] C++：类与构造函数
来源：http://pyd.aibaodan.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sms.zhixingplan.top

[S42] C++：继承与虚函数
来源：http://zpi.dashuyun.cn

class B : public Base { public: void f() override {} };
来源：http://mbm.tianlin.xyz

[S43] C++：智能指针
来源：http://edf.fanxiaobao.xyz

auto p = std::make_unique<int>(5);
来源：http://ofq.cqqwz.cn

[S44] C++：引用传参
来源：http://rvb.chenjidiqi.icu

void inc(int &x) { ++x; }
来源：http://xpq.hfpthk.cn

[S45] C++：lambda
来源：http://fhi.dianchejie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wiy.snrcjt.cn

[S46] C++：函数模板
来源：http://mby.hfpthk.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xno.jinqigufen.top

[S47] C++：结构化绑定遍历
来源：http://sco.fktsv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ssy.yonumen.top

[S48] C++：逐行读文件
来源：http://pbs.52xcode.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rew.sufxvd.cn

while (std::getline(in, line)) { }
来源：http://anx.sysykeji.top

[S49] C++：写文件
来源：http://vwf.gogol.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tld.cdnleiting.top

[S50] C++：格式化数字
来源：http://rcd.yuanzhike.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gqx.zhongyouzk.top

[S51] C++：显式类型转换
来源：http://elk.xylfe.cn

static_cast<double>(a) / b
来源：http://ovl.snrcjt.cn

[S52] C++：const 与 noexcept
来源：http://vga.ctjpmb.com

int size() const noexcept { return n_; }
来源：http://nbb.fehbvm.com

[S53] C++：移动语义
来源：http://iuq.cashguo.top

std::vector<int> w = std::move(v);
来源：http://gbv.cucudq.cn

[S54] C++：异常处理
来源：http://igz.mhx1999.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pjn.nanxinkj.top

[S55] C++：结构化绑定
来源：http://nwy.nanxinkj.top

auto [a, b] = std::make_pair(1, 2);
来源：http://yvr.chenjidiqi.icu

[S56] C++：optional
来源：http://hpi.jianghu66.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oup.jinghuilouyu.cn

[S57] C++：编译期常量
来源：http://ita.0kj1m.cn

constexpr int N = 10;
来源：http://jcs.ydjk.org.cn

[S58] C++：命名空间
来源：http://zmz.feifeiyinyue.top

namespace ns { int f() { return 1; } }
来源：http://vrh.daxiang520.top

[S59] C++：静态断言
来源：http://umy.shangyingyoupin.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uom.aizwys.cn

[S60] C++：遍历并删除元素
来源：http://acp.shangyingyoupin.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://aos.jinyuanbaomall.cn

================================================================================
来源：http://ixw.cdnleiting.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cpk.ydzc1.top

================================================================================
来源：http://nzv.yvedp.cn

[T01] Kotlin：Hello World
来源：http://pgy.epnwcf.com

println("Hello")
来源：http://yev.fktsv.cn

[T02] Kotlin：变量
来源：http://zxb.fanxiaobao.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bbk.aizwys.cn

[T03] Kotlin：字符串模板
来源：http://ita.nwbrower.top

"值: $b"
来源：http://ugv.zdqjudy.top

[T04] Kotlin：空安全
来源：http://grb.daria6918.cn

val n: String? = null;  n?.length
来源：http://nwz.hammf.cn

[T05] Kotlin：when 表达式
来源：http://met.cheryme.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://asm.bjfxy.top

[T06] Kotlin：集合映射
来源：http://jch.wangshuangyany.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://efo.sufxvd.cn

[T07] Kotlin：集合过滤
来源：http://uyw.yuxming.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mdf.yanxiufei.cn

[T08] Kotlin：数据类
来源：http://url.kuanghao11.cn

data class User(val name: String, val age: Int)
来源：http://onp.tanke756.top

[T09] Kotlin：扩展函数
来源：http://zok.shangyingyoupin.top

fun String.exclaim() = this + "!"
来源：http://chr.jinyuanbaomall.cn

[T10] Kotlin：默认参数
来源：http://uce.xylfe.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://upg.uphjek.com

[T11] Kotlin：协程
来源：http://kyn.xingfuxueyuan.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://fdg.jlsjyb.cn

[T12] Kotlin：解构声明
来源：http://gec.sweek.top

val (a, b) = Pair(1, 2)
来源：http://wpn.nwbrower.top

[T13] Kotlin：只读 Map
来源：http://soi.daxiang520.top

val m = mapOf("a" to 1)
来源：http://jkr.cdnleiting.top

[T14] Kotlin：循环
来源：http://alb.9152youxi.cn

for (i in 1..10) println(i)
来源：http://upg.bjfxy.top

[T15] Kotlin：接口
来源：http://evf.tanke756.top

interface Shape { fun area(): Double }
来源：http://mbj.dianchejie.cn

[T16] Swift：Hello World
来源：http://tgf.jiagoushi.top

print("Hello")
来源：http://mbc.guannengcc.top

[T17] Swift：变量与常量
来源：http://oak.zdbjq.cn

var a = 1;  let b = 2
来源：http://unq.haohaochexian.top

[T18] Swift：字符串插值
来源：http://rwa.zycfv.cn

"值: \(b)"
来源：http://bwp.ydjk.org.cn

[T19] Swift：可选绑定
来源：http://ktc.uphjek.com

if let n = opt { print(n) }
来源：http://rac.guowangkeji.top

[T20] Swift：数组操作
来源：http://jef.zhiwuduotai.top

var a = [1, 2, 3];  a.append(4)
来源：http://dui.xziqi.cn

[T21] Swift：遍历
来源：http://zpu.bbcook.cn

for x in a { print(x) }
来源：http://wzq.zhongyouzk.top

[T22] Swift：字典
来源：http://nea.gotoacloud.top

var d = ["a": 1];  d["b"] = 2
来源：http://aoy.cdnleiting.top

[T23] Swift：函数
来源：http://ncp.dashuyun.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qdu.fzhhl.top

[T24] Swift：闭包
来源：http://zgb.hywenlv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qoe.zhiwuduotai.top

[T25] Swift：结构体
来源：http://kwc.316326.xyz

struct P { var x: Int }
来源：http://rip.hnqzz.top

[T26] Swift：类与重写
来源：http://qnp.cucudq.cn

class A: Base { override func f() {} }
来源：http://pef.feifeiyinyue.top

[T27] Swift：错误处理
来源：http://ymn.zhixingplan.top

do { try f() } catch { print(error) }
来源：http://zsj.epnwcf.com

[T28] Swift：枚举
来源：http://kix.dashuyun.cn

enum Color { case red, green }
来源：http://ngl.sjlbkw.cn

[T29] Swift：guard 提前返回
来源：http://qyn.dashuyun.cn

guard let x = opt else { return }
来源：http://cky.daxiang520.top

[T30] Swift：协议
来源：http://qrh.jlsjyb.cn

protocol Shape { func area() -> Double }
来源：http://jxc.ydzc1.top

[T31] Lua：Hello World
来源：http://sbb.hammf.cn

print("Hello")
来源：http://kxp.jinghuilouyu.cn

[T32] Lua：局部变量
来源：http://gmx.hywenlv.cn

local a = 1
来源：http://tkw.zhiwuduotai.top

[T33] Lua：表（数组）
来源：http://bcn.mhx1999.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ixb.ydjk.org.cn

[T34] Lua：遍历表
来源：http://oqp.xuanzx.com

for i, v in ipairs(t) do print(i, v) end
来源：http://lsb.aizwys.cn

[T35] Lua：字典表
来源：http://aoo.hnqzz.top

local d = { a = 1 };  d.b = 2
来源：http://zll.shuidangran.top

[T36] Lua：函数
来源：http://jsi.dianchejie.cn

function add(a, b) return a + b end
来源：http://rcn.sweek.top

[T37] Lua：字符串拼接
来源：http://ddq.yj20258888.top

"a" .. "b"
来源：http://rnb.xingfuxueyuan.xyz

[T38] Lua：条件
来源：http://aqz.xingfuxueyuan.xyz

if x > 0 then print("正") end
来源：http://aec.shanyushiyangtech.top

[T39] Lua：模式匹配
来源：http://qxp.ehwqpu.com

string.find(s, "%d+")
来源：http://lzb.wangdashe.top

[T40] Lua：元表
来源：http://fsj.vqdsnc.cn

setmetatable({}, { __index = base })
来源：http://vhd.cucudq.cn

[T41] Perl：Hello World
来源：http://gxz.meibo888.top

print "Hello\n";
来源：http://gjo.zdbjq.cn

[T42] Perl：变量类型
来源：http://adu.ehwqpu.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tlj.hywenlv.cn

[T43] Perl：字符串插值
来源：http://bui.epnwcf.com

"值: $a"
来源：http://zqx.chenjidiqi.icu

[T44] Perl：条件
来源：http://iig.yj20258888.top

if ($a > 0) { print "正"; }
来源：http://tax.chenlongwang.top

[T45] Perl：数组遍历
来源：http://ycd.shangyingyoupin.top

for my $x (@arr) { print $x; }
来源：http://gji.xziqi.cn

[T46] Perl：哈希操作
来源：http://ksf.ydjk.org.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gij.tian-w.cn

[T47] Perl：正则捕获
来源：http://bis.fehbvm.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://roe.hywenlv.cn

[T48] Perl：正则替换
来源：http://myw.fzhhl.top

$s =~ s/old/new/g;
来源：http://olv.chenzaomai.com

[T49] Perl：函数
来源：http://lvs.sufxvd.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qrs.bjfxy.top

[T50] Perl：逐行读文件
来源：http://fxe.fengsongda.top

open my $fh, "<", "a.txt" or die $!;
来源：http://mpj.yfazqb.com

while (my $line = <$fh>) { print $line; }
来源：http://deq.hammf.cn

[T51] Scala：Hello World
来源：http://jia.vehdjk.com

println("Hello")
来源：http://jlu.guowangkeji.top

[T52] Scala：变量
来源：http://efs.bjfxy.top

val a = 1;  var b = 2
来源：http://nrm.pycfn.com

[T53] Scala：字符串插值
来源：http://auo.svipenyu.cn

s"值: $b"
来源：http://wnx.xylfe.cn

[T54] Scala：集合映射
来源：http://ngc.vqdsnc.cn

List(1, 2, 3).map(_ * 2)
来源：http://fha.xuanzx.com

[T55] Scala：集合过滤
来源：http://wcd.nanxuanxn.top

List(1, 2, 3).filter(_ > 1)
来源：http://ord.pengpengdd.cyou

[T56] Scala：样例类
来源：http://msg.gogol.net.cn

case class User(name: String, age: Int)
来源：http://fpu.jinyuanbaomall.cn

[T57] Scala：模式匹配
来源：http://fxa.yvedp.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://shr.nanxuanxn.top

[T58] Scala：函数定义
来源：http://gfr.zdbjq.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gxy.nanxuanxn.top

[T59] Scala：循环
来源：http://dds.zhoulong.xyz

for (i <- 1 to 10) println(i)
来源：http://hwj.chenzaomai.com

[T60] Scala：折叠
来源：http://wce.jiagoushi.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tyx.sjlbkw.cn

================================================================================
来源：http://ahq.zhijiandao.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ufk.xylfe.cn

================================================================================
来源：http://wtd.daxiang520.top

[U01] Py：创建虚拟环境
来源：http://mpc.dianchejie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qsi.havefunace.top

[U02] Py：导出 / 安装依赖
来源：http://utj.tanke756.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hjk.gzhubu.top

[U03] Py：加载 .env 配置
来源：http://wqz.jinyuanbaomall.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lrp.hcnkem.com

[U04] Py：变量调试打印
来源：http://nty.snrcjt.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ucb.zhixingplan.top

[U05] Py：列表去重且保序
来源：http://eqt.ydjk.org.cn

list(dict.fromkeys(arr))
来源：http://cpi.yonumen.top

[U06] Py：合并两个字典
来源：http://wne.sjlbkw.cn

{**a, **b}
来源：http://mob.shangyingyoupin.top

[U07] Py：反转字典键值
来源：http://hbj.vehdjk.com

{v: k for k, v in d.items()}
来源：http://ztw.haohaochexian.top

[U08] Py：展平二维列表
来源：http://hbq.haohaochexian.top

[y for x in nested for y in x]
来源：http://csa.jlsjyb.cn

[U09] Py：字典取最大值的键
来源：http://wsz.gaohongyu789.top

max(d, key=d.get)
来源：http://ixz.vehdjk.com

[U10] Py：按值排序字典
来源：http://quj.sweek.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hkc.meibo888.top

[U11] Py：生成器表达式
来源：http://him.ppjwa.cn

(x * 2 for x in arr)
来源：http://qny.zhaomingkeji.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://vow.chenjidiqi.icu

Counter(arr).most_common(3)
来源：http://qhj.ppjwa.cn

[U13] Py：固定长度队列
来源：http://jqj.jqgfzy.top

deque(maxlen=10)
来源：http://cwe.cqqwz.cn

[U14] Py：分组收集到列表
来源：http://byg.9152youxi.cn

defaultdict(list)
来源：http://stc.xingfuxueyuan.xyz


<!-- 参考信息 -->