代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://xqo.kuanghao11.cn

[R72] 等待端口就绪
来源：http://adt.shanyushiyangtech.top

until nc -z localhost 3306; do sleep 1; done
来源：http://atj.jyoumei.cn

[R73] 分割大日志
来源：http://gan.uphjek.com

split -l 1000 big.log part_
来源：http://jwy.hongshengwenyu.top

[R74] 批量重命名
来源：http://kfu.shzxlz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mhj.epnwcf.com

[R75] 导出环境变量
来源：http://ary.daxiang520.top

export PATH="$HOME/bin:$PATH"
来源：http://fjb.hnxiangtu.top

[R76] 使用临时文件
来源：http://mip.yvedp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kyh.xingfuxueyuan.xyz

[R77] 读取用户输入
来源：http://aum.ehwqpu.com

read -rp "请输入: " ans
来源：http://gzf.zdqjudy.top

[R78] 交互式菜单
来源：http://bac.pycfn.com

select opt in a b c; do echo "$opt"; break; done
来源：http://zhn.yonumen.top

[R79] 解析命令行选项
来源：http://xfp.cqqwz.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://klh.uphjek.com

[R80] 查看脚本执行耗时
来源：http://fkq.zhongyouzk.top

time ./run.sh
来源：http://bog.gzhubu.top

================================================================================
来源：http://kxp.shzxlz.cn

S. C / C++ 专题
来源：http://wvs.xylfe.cn

================================================================================
来源：http://skb.mhx1999.top

[S01] C：Hello World
来源：http://ajt.jqgfzy.top

#include <stdio.h>
来源：http://wcq.havefunace.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qtk.tanke756.top

[S02] C：变量与格式化输出
来源：http://zti.bjfxy.top

int a = 10; printf("%d\n", a);
来源：http://tru.hcnkem.com

[S03] C：读入整数
来源：http://yxc.daxiang520.top

int x; scanf("%d", &x);
来源：http://ytv.yj20258888.top

[S04] C：字符串复制
来源：http://gsi.smart0.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://dio.c1oappe.top

[S05] C：字符串长度
来源：http://ecl.zhaomingkeji.xyz

strlen(s)
来源：http://nny.zhiwuduotai.top

[S06] C：字符串比较
来源：http://qgh.zhijiandao.cn

strcmp(a, b) == 0
来源：http://ltd.dashuyun.cn

[S07] C：数组遍历求和
来源：http://nle.ydzc1.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ohd.aibaodan.cn

[S08] C：动态内存分配与释放
来源：http://vic.zhengqikj.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nfo.jyoumei.cn

[S09] C：结构体定义与初始化
来源：http://uhx.0kj1m.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nhe.smart0.xyz

[S10] C：指针与解引用
来源：http://zgx.gaohongyu789.top

int *p = &a;  *p = 5;
来源：http://ibd.uphjek.com

[S11] C：逐行读文件
来源：http://hhc.gzhubu.top

FILE *f = fopen("a.txt", "r");
来源：http://hbe.fengsongda.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://usv.tanke756.top

fclose(f);
来源：http://axa.zhoulong.xyz

[S12] C：写文件
来源：http://atf.kuanghao11.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ell.jinqigfzy.top

[S13] C：宏定义
来源：http://kxj.yj20258.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dsf.tian-w.cn

[S14] C：枚举
来源：http://get.zhengqikj.top

enum Color { RED, GREEN, BLUE };
来源：http://qwv.zhengqikj.top

[S15] C：类型转换
来源：http://njp.jinghuilouyu.cn

(double) a / b
来源：http://gue.gotoacloud.top

[S16] C：位操作置位
来源：http://rvj.zhengqikj.top

x |= (1 << 3);
来源：http://ewc.zhaomingkeji.xyz

[S17] C：安全拼接字符串
来源：http://umx.mhx1999.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nig.ybcxt.top

[S18] C：命令行参数
来源：http://nvy.epnwcf.com

int main(int argc, char **argv)
来源：http://qca.sweek.top

[S19] C：快速排序
来源：http://toa.jinyuanbaomall.cn

qsort(a, n, sizeof(int), cmp);
来源：http://aiv.jinqigfzy.top

[S20] C：二分查找
来源：http://bgo.jinyuanbaomall.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pxq.havefunace.top

[S21] C：字符类别判断
来源：http://akb.xylfe.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hwi.zhongyouzk.top

[S22] C：字符串转数字
来源：http://rax.dianchejie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://afx.jinqigfzy.top

[S23] C：随机数
来源：http://kxp.andypj.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://ytv.jinghuilouyu.cn

[S24] C：获取本地时间
来源：http://wkp.zycfv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fvx.zhoulong.xyz

[S25] C：内存拷贝
来源：http://bmw.hfpthk.cn

memcpy(dst, src, n);
来源：http://eei.sxryk.cn

[S26] C：内存清零
来源：http://sqx.sjlbkw.cn

memset(a, 0, sizeof a);
来源：http://fyt.jqgufenzy.top

[S27] C：定义常量
来源：http://eax.xingfuxueyuan.xyz

const double PI = 3.14159;
来源：http://faj.jqgfzy.top

[S28] C：静态变量
来源：http://auk.zhixingplan.top

static int counter = 0;
来源：http://hix.yangfankeji.com

[S29] C：变参函数
来源：http://gft.sxryk.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dxo.aizwys.cn

[S30] C：头文件保护
来源：http://cgh.gzhubu.top

#ifndef X_H
来源：http://zdr.zhijiandao.cn

#define X_H
来源：http://wwt.xuanzx.com

#endif
来源：http://icw.zhaomingkeji.xyz

[S31] C++：Hello World
来源：http://qch.andypj.xyz

#include <iostream>
来源：http://xcg.hfpthk.cn

int main() { std::cout << "Hello\n"; }
来源：http://rul.yj20258888.top

[S32] C++：字符串
来源：http://kzs.cucudq.cn

std::string s = "hi";  s += "!";
来源：http://xqv.cucudq.cn

[S33] C++：vector 增删
来源：http://hao.gotoacloud.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rgm.nanxuanxn.top

[S34] C++：遍历 vector
来源：http://eeo.zhaomingkeji.xyz

for (auto &x : v) { std::cout << x; }
来源：http://itm.guannengcc.top

[S35] C++：map
来源：http://dzw.guowangkeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fga.9152youxi.cn

[S36] C++：unordered_map
来源：http://mvg.gzhubu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gqw.zhixingplan.top

[S37] C++：set
来源：http://cdd.jinghuilouyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hwc.redwolf501.top

[S38] C++：排序
来源：http://rhx.hnxiangtu.top

std::sort(v.begin(), v.end());
来源：http://ovi.zycfv.cn

[S39] C++：自定义比较器排序
来源：http://oar.hysaishi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qsq.yongpay.top

[S40] C++：查找元素
来源：http://cue.nwbrower.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pkl.fzhhl.top

[S41] C++：类与构造函数
来源：http://nkp.hongshengwenyu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ewf.fengsongda.top

[S42] C++：继承与虚函数
来源：http://mwv.ctjpmb.com

class B : public Base { public: void f() override {} };
来源：http://uwk.hywenlv.cn

[S43] C++：智能指针
来源：http://bzb.pycfn.com

auto p = std::make_unique<int>(5);
来源：http://veq.yj20258.top

[S44] C++：引用传参
来源：http://syx.sjlbkw.cn

void inc(int &x) { ++x; }
来源：http://jbc.xinyue.icu

[S45] C++：lambda
来源：http://mqs.hongshengwenyu.top

auto add = [](int a, int b) { return a + b; };
来源：http://ucv.feifeiyinyue.top

[S46] C++：函数模板
来源：http://xsm.xingfuxueyuan.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://iag.ppjwa.cn

[S47] C++：结构化绑定遍历
来源：http://xfy.zdqjudy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cls.zycfv.cn

[S48] C++：逐行读文件
来源：http://jrd.hnqzz.top

std::ifstream in("a.txt");  std::string line;
来源：http://zpa.hywenlv.cn

while (std::getline(in, line)) { }
来源：http://vpn.9152youxi.cn

[S49] C++：写文件
来源：http://hyh.xingfuxueyuan.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dmr.ydjk.org.cn

[S50] C++：格式化数字
来源：http://mqz.fktsv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://swj.sjlbkw.cn

[S51] C++：显式类型转换
来源：http://bia.pycfn.com

static_cast<double>(a) / b
来源：http://ace.quarkkingdee.top

[S52] C++：const 与 noexcept
来源：http://tae.gogol.net.cn

int size() const noexcept { return n_; }
来源：http://lgg.sjlbkw.cn

[S53] C++：移动语义
来源：http://tgp.gzhubu.top

std::vector<int> w = std::move(v);
来源：http://lif.jinyuanbaomall.cn

[S54] C++：异常处理
来源：http://lkh.9152youxi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cvy.chenjidiqi.icu

[S55] C++：结构化绑定
来源：http://qox.jqgufenzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://cyo.ehwqpu.com

[S56] C++：optional
来源：http://jdd.sufxvd.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uzu.jinqigfzy.top

[S57] C++：编译期常量
来源：http://ogd.ybcxt.top

constexpr int N = 10;
来源：http://mya.yj202588.top

[S58] C++：命名空间
来源：http://gpk.yfazqb.com

namespace ns { int f() { return 1; } }
来源：http://udy.quarkkingdee.top

[S59] C++：静态断言
来源：http://rdw.jiagoushi.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gmw.zhoulong.xyz

[S60] C++：遍历并删除元素
来源：http://imw.zdbjq.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bfp.yueranfly.top

================================================================================
来源：http://faa.chenzaomai.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gam.nanxuanxn.top

================================================================================
来源：http://ubw.zhixingplan.top

[T01] Kotlin：Hello World
来源：http://dzk.yanxiufei.cn

println("Hello")
来源：http://ula.xingfuxueyuan.xyz

[T02] Kotlin：变量
来源：http://kfl.quarkkingdee.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hyg.nanxuanxn.top

[T03] Kotlin：字符串模板
来源：http://bfk.bjfxy.top

"值: $b"
来源：http://dkq.xuetiantiany.cn

[T04] Kotlin：空安全
来源：http://jpm.hnqzz.top

val n: String? = null;  n?.length
来源：http://mxt.aibaodan.cn

[T05] Kotlin：when 表达式
来源：http://qce.gogol.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jwf.gaohongyu789.top

[T06] Kotlin：集合映射
来源：http://rud.shangyingyoupin.top

listOf(1, 2, 3).map { it * 2 }
来源：http://aci.jinghuilouyu.cn

[T07] Kotlin：集合过滤
来源：http://rbw.bbcook.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wrf.hnxiangtu.top

[T08] Kotlin：数据类
来源：http://mzm.iojbl.cn

data class User(val name: String, val age: Int)
来源：http://vce.hongshengwenyu.top

[T09] Kotlin：扩展函数
来源：http://lpr.xziqi.cn

fun String.exclaim() = this + "!"
来源：http://sfu.sxryk.cn

[T10] Kotlin：默认参数
来源：http://mkz.yfazqb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://een.yongpay.top

[T11] Kotlin：协程
来源：http://twk.ctjpmb.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://cby.cdnleiting.top

[T12] Kotlin：解构声明
来源：http://fdf.316326.xyz

val (a, b) = Pair(1, 2)
来源：http://cbu.haohaochexian.top

[T13] Kotlin：只读 Map
来源：http://fwd.zhoulong.xyz

val m = mapOf("a" to 1)
来源：http://ndu.gogol.net.cn

[T14] Kotlin：循环
来源：http://qvm.zhaomingkeji.xyz

for (i in 1..10) println(i)
来源：http://qus.52xcode.cn

[T15] Kotlin：接口
来源：http://zfo.hnxiangtu.top

interface Shape { fun area(): Double }
来源：http://iio.ehwqpu.com

[T16] Swift：Hello World
来源：http://iic.yongpay.top

print("Hello")
来源：http://jdr.zhixingplan.top

[T17] Swift：变量与常量
来源：http://bab.andypj.xyz

var a = 1;  let b = 2
来源：http://nfz.gogol.net.cn

[T18] Swift：字符串插值
来源：http://xje.hfpthk.cn

"值: \(b)"
来源：http://rto.yueranfly.top

[T19] Swift：可选绑定
来源：http://xqe.jinqigufen.top

if let n = opt { print(n) }
来源：http://mix.hnxiangtu.top

[T20] Swift：数组操作
来源：http://dyh.yj20258888.top

var a = [1, 2, 3];  a.append(4)
来源：http://jqw.dashuyun.cn

[T21] Swift：遍历
来源：http://vbh.wangdashe.top

for x in a { print(x) }
来源：http://imi.gogol.net.cn

[T22] Swift：字典
来源：http://ftb.jinghuilouyu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lgx.pengpengdd.cyou

[T23] Swift：函数
来源：http://mbd.fengsongda.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gur.jiagoushi.top

[T24] Swift：闭包
来源：http://zne.pengpengdd.cyou

let f = { (x: Int) -> Int in x * 2 }
来源：http://sha.ywan-chungtsiang.top

[T25] Swift：结构体
来源：http://klt.zhoulong.xyz

struct P { var x: Int }
来源：http://hhw.gzhubu.top

[T26] Swift：类与重写
来源：http://mvi.hongshengwenyu.top

class A: Base { override func f() {} }
来源：http://wbp.hongshengwenyu.top

[T27] Swift：错误处理
来源：http://rbv.aibaodan.cn

do { try f() } catch { print(error) }
来源：http://ezn.svipenyu.cn

[T28] Swift：枚举
来源：http://qeq.fzhhl.top

enum Color { case red, green }
来源：http://faz.jyoumei.cn

[T29] Swift：guard 提前返回
来源：http://cin.yj20258888.top

guard let x = opt else { return }
来源：http://dyj.yueranfly.top

[T30] Swift：协议
来源：http://ono.quarkkingdee.top

protocol Shape { func area() -> Double }
来源：http://vvk.chenjidiqi.icu

[T31] Lua：Hello World
来源：http://ttb.jyoumei.cn

print("Hello")
来源：http://vcb.iojbl.cn

[T32] Lua：局部变量
来源：http://zcy.hysaishi.cn

local a = 1
来源：http://ucs.jqgufenzy.top

[T33] Lua：表（数组）
来源：http://hqz.wangdashe.top

local t = {1, 2, 3};  t[4] = 4
来源：http://iwb.uphjek.com

[T34] Lua：遍历表
来源：http://tnz.cdnleiting.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qsj.fengsongda.top

[T35] Lua：字典表
来源：http://nuh.jiagoushi.top

local d = { a = 1 };  d.b = 2
来源：http://qaz.ywan-chungtsiang.top

[T36] Lua：函数
来源：http://jhx.bjfxy.top

function add(a, b) return a + b end
来源：http://rsr.nwbrower.top

[T37] Lua：字符串拼接
来源：http://edj.gzhubu.top

"a" .. "b"
来源：http://igf.hesvh.cn

[T38] Lua：条件
来源：http://thn.yueranfly.top

if x > 0 then print("正") end
来源：http://pxe.yuxming.cn

[T39] Lua：模式匹配
来源：http://gas.0kj1m.cn

string.find(s, "%d+")
来源：http://myu.sjlbkw.cn

[T40] Lua：元表
来源：http://qtc.hcnkem.com

setmetatable({}, { __index = base })
来源：http://dlz.shuidangran.top

[T41] Perl：Hello World
来源：http://dvf.shanyushiyangtech.top

print "Hello\n";
来源：http://sdo.316326.xyz

[T42] Perl：变量类型
来源：http://ktm.316326.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zob.redwolf501.top

[T43] Perl：字符串插值
来源：http://ntl.xziqi.cn

"值: $a"
来源：http://fpt.gotoacloud.top

[T44] Perl：条件
来源：http://ehv.epnwcf.com

if ($a > 0) { print "正"; }
来源：http://efq.yj202588.top

[T45] Perl：数组遍历
来源：http://foe.uphjek.com

for my $x (@arr) { print $x; }
来源：http://vqg.vehdjk.com

[T46] Perl：哈希操作
来源：http://eoh.jinqigfzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://llj.9152youxi.cn

[T47] Perl：正则捕获
来源：http://inc.dianchejie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fzc.yj202588.top

[T48] Perl：正则替换
来源：http://vbc.shangyingyoupin.top

$s =~ s/old/new/g;
来源：http://xze.redwolf501.top

[T49] Perl：函数
来源：http://szi.jlsjyb.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://llm.ivvv.top

[T50] Perl：逐行读文件
来源：http://csm.gogol.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xcq.pycfn.com

while (my $line = <$fh>) { print $line; }
来源：http://uaq.daria6918.cn

[T51] Scala：Hello World
来源：http://zkk.tanke756.top

println("Hello")
来源：http://owd.yj20258.top

[T52] Scala：变量
来源：http://pqx.fzhhl.top

val a = 1;  var b = 2
来源：http://dcv.jinqigufen.top

[T53] Scala：字符串插值
来源：http://nxd.zhongyouzk.top

s"值: $b"
来源：http://jsg.quarkkingdee.top

[T54] Scala：集合映射
来源：http://hjt.fzhhl.top

List(1, 2, 3).map(_ * 2)
来源：http://akq.yuxming.cn

[T55] Scala：集合过滤
来源：http://yrm.redwolf501.top

List(1, 2, 3).filter(_ > 1)
来源：http://ddj.ywan-chungtsiang.top

[T56] Scala：样例类
来源：http://cwe.cheryme.top

case class User(name: String, age: Int)
来源：http://kpf.jyoumei.cn

[T57] Scala：模式匹配
来源：http://xqz.yfazqb.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://adu.cqqwz.cn

[T58] Scala：函数定义
来源：http://xbd.fanxiaobao.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://rxh.shanyushiyangtech.top

[T59] Scala：循环
来源：http://qap.jinghuilouyu.cn

for (i <- 1 to 10) println(i)
来源：http://fuq.wangdashe.top

[T60] Scala：折叠
来源：http://bwa.gogol.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wgn.snrcjt.cn

================================================================================
来源：http://zpx.hesvh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://els.shuidangran.top

================================================================================
来源：http://arq.sufxvd.cn

[U01] Py：创建虚拟环境
来源：http://ggf.chenjidiqi.icu

python -m venv .venv && source .venv/bin/activate
来源：http://bgt.sjlbkw.cn

[U02] Py：导出 / 安装依赖
来源：http://psv.xziqi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ekv.chenlongwang.top

[U03] Py：加载 .env 配置
来源：http://plf.vehdjk.com

from dotenv import load_dotenv; load_dotenv()
来源：http://akf.birdmap.top

[U04] Py：变量调试打印
来源：http://knd.sxryk.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rqs.fktsv.cn

[U05] Py：列表去重且保序
来源：http://qbu.ydjk.org.cn

list(dict.fromkeys(arr))
来源：http://hek.hesvh.cn

[U06] Py：合并两个字典
来源：http://seg.dianchejie.cn

{**a, **b}
来源：http://ppf.hongshengwenyu.top

[U07] Py：反转字典键值
来源：http://drl.aizwys.cn

{v: k for k, v in d.items()}
来源：http://npl.aibaodan.cn

[U08] Py：展平二维列表
来源：http://dzr.wangshuangyany.cn

[y for x in nested for y in x]
来源：http://iwy.jyoumei.cn

[U09] Py：字典取最大值的键
来源：http://hdz.sufxvd.cn

max(d, key=d.get)
来源：http://rrf.yonumen.top

[U10] Py：按值排序字典
来源：http://tya.xziqi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://eqf.xuetiantiany.cn

[U11] Py：生成器表达式
来源：http://pja.yuxming.cn

(x * 2 for x in arr)
来源：http://tvi.yvedp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bnt.haohaochexian.top

Counter(arr).most_common(3)
来源：http://vjo.yfazqb.com


<!-- 参考信息 -->