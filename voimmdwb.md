代发 wailian999

openssl rand -hex 16
来源：http://bjr.tianlin.xyz

[R68] 计算文件校验值
来源：http://srr.yanxiufei.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fjr.bjfxy.top

[R69] 生成随机密码
来源：http://ahg.sjlbkw.cn

head -c 16 /dev/urandom | base64
来源：http://nnw.gotoacloud.top

[R70] 时间戳与互转
来源：http://sqv.fengsongda.top

date +%s;  date -d @1700000000
来源：http://zfb.sysykeji.top

[R71] 日期格式化
来源：http://sdo.havefunace.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://sww.hongshengwenyu.top

[R72] 等待端口就绪
来源：http://vql.yj20258888.top

until nc -z localhost 3306; do sleep 1; done
来源：http://gsi.haohaochexian.top

[R73] 分割大日志
来源：http://hht.sweek.top

split -l 1000 big.log part_
来源：http://unq.ydjk.org.cn

[R74] 批量重命名
来源：http://pya.9152youxi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vlo.daxiang520.top

[R75] 导出环境变量
来源：http://ksh.kuanghao11.cn

export PATH="$HOME/bin:$PATH"
来源：http://cyk.nwbrower.top

[R76] 使用临时文件
来源：http://wjg.jyoumei.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bdz.bjfxy.top

[R77] 读取用户输入
来源：http://bco.yueranfly.top

read -rp "请输入: " ans
来源：http://upu.52xcode.cn

[R78] 交互式菜单
来源：http://ylh.zhoulong.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://nbk.zhengqikj.top

[R79] 解析命令行选项
来源：http://bro.uphjek.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://evf.ydzc1.top

[R80] 查看脚本执行耗时
来源：http://iou.bjfxy.top

time ./run.sh
来源：http://jmm.yongpay.top

================================================================================
来源：http://nog.ybcxt.top

S. C / C++ 专题
来源：http://azm.bjfxy.top

================================================================================
来源：http://rsh.jiagoushi.top

[S01] C：Hello World
来源：http://gjv.wangshuangyany.cn

#include <stdio.h>
来源：http://dae.xinyue.icu

int main(void) { printf("Hello\n"); return 0; }
来源：http://xvd.zdqjudy.top

[S02] C：变量与格式化输出
来源：http://ywi.shzxlz.cn

int a = 10; printf("%d\n", a);
来源：http://dkh.cashguo.top

[S03] C：读入整数
来源：http://ykm.xinyue.icu

int x; scanf("%d", &x);
来源：http://aca.yanxiufei.cn

[S04] C：字符串复制
来源：http://hjs.zhengqikj.top

char dst[32]; strcpy(dst, "hi");
来源：http://aqd.shuidangran.top

[S05] C：字符串长度
来源：http://ejn.nanxinkj.top

strlen(s)
来源：http://blo.jianghu66.top

[S06] C：字符串比较
来源：http://rhe.zycfv.cn

strcmp(a, b) == 0
来源：http://wlo.bjfxy.top

[S07] C：数组遍历求和
来源：http://vhh.sjlbkw.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rcn.zhiwuduotai.top

[S08] C：动态内存分配与释放
来源：http://anv.jinyuanbaomall.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://apv.zhijiandao.cn

[S09] C：结构体定义与初始化
来源：http://sxa.yj202588.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wgj.zhijiandao.cn

[S10] C：指针与解引用
来源：http://kcu.yanxiufei.cn

int *p = &a;  *p = 5;
来源：http://xzv.zhengqikj.top

[S11] C：逐行读文件
来源：http://fkm.c1oappe.top

FILE *f = fopen("a.txt", "r");
来源：http://pxl.kuanghao11.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hnx.uphjek.com

fclose(f);
来源：http://vbc.daxiang520.top

[S12] C：写文件
来源：http://enn.gogol.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tom.zhiwuduotai.top

[S13] C：宏定义
来源：http://csy.shanyushiyangtech.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sai.daria6918.cn

[S14] C：枚举
来源：http://vpl.yj20258888.top

enum Color { RED, GREEN, BLUE };
来源：http://ebq.guowangkeji.top

[S15] C：类型转换
来源：http://xqe.zycfv.cn

(double) a / b
来源：http://fxi.hfpthk.cn

[S16] C：位操作置位
来源：http://mrn.svipenyu.cn

x |= (1 << 3);
来源：http://gfa.cashguo.top

[S17] C：安全拼接字符串
来源：http://gqb.hywenlv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xje.smart0.xyz

[S18] C：命令行参数
来源：http://lje.yongpay.top

int main(int argc, char **argv)
来源：http://vbi.tian-w.cn

[S19] C：快速排序
来源：http://tlm.zhengqikj.top

qsort(a, n, sizeof(int), cmp);
来源：http://zed.ehwqpu.com

[S20] C：二分查找
来源：http://jjo.cashguo.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://heo.vehdjk.com

[S21] C：字符类别判断
来源：http://zsg.smart0.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vys.sysykeji.top

[S22] C：字符串转数字
来源：http://arp.smart0.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://qpj.hnqzz.top

[S23] C：随机数
来源：http://qsu.hnqzz.top

srand(time(NULL));  int r = rand() % 100;
来源：http://zqk.dianchejie.cn

[S24] C：获取本地时间
来源：http://umt.xingfuxueyuan.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qwf.jianghu66.top

[S25] C：内存拷贝
来源：http://qli.zdqjudy.top

memcpy(dst, src, n);
来源：http://vmc.fanxiaobao.xyz

[S26] C：内存清零
来源：http://ymj.xinyue.icu

memset(a, 0, sizeof a);
来源：http://jvu.tarul.cn

[S27] C：定义常量
来源：http://oks.daxiang520.top

const double PI = 3.14159;
来源：http://tam.fanxiaobao.xyz

[S28] C：静态变量
来源：http://isu.hongshengwenyu.top

static int counter = 0;
来源：http://lei.cqqwz.cn

[S29] C：变参函数
来源：http://gxt.guannengcc.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://llw.tian-w.cn

[S30] C：头文件保护
来源：http://gdc.cucudq.cn

#ifndef X_H
来源：http://jvn.hcnkem.com

#define X_H
来源：http://rxi.guowangkeji.top

#endif
来源：http://uph.nanxinkj.top

[S31] C++：Hello World
来源：http://rrx.tianlin.xyz

#include <iostream>
来源：http://gwd.meibo888.top

int main() { std::cout << "Hello\n"; }
来源：http://wuv.hongshengwenyu.top

[S32] C++：字符串
来源：http://tyo.sysykeji.top

std::string s = "hi";  s += "!";
来源：http://pem.zhaomingkeji.xyz

[S33] C++：vector 增删
来源：http://fpf.jiagoushi.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ywy.yj20258888.top

[S34] C++：遍历 vector
来源：http://uoz.vqdsnc.cn

for (auto &x : v) { std::cout << x; }
来源：http://rok.shuidangran.top

[S35] C++：map
来源：http://niu.aibaodan.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rea.yvedp.cn

[S36] C++：unordered_map
来源：http://spd.jlsjyb.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wyc.chenlongwang.top

[S37] C++：set
来源：http://kox.zdqjudy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rey.sysykeji.top

[S38] C++：排序
来源：http://qxl.chenlongwang.top

std::sort(v.begin(), v.end());
来源：http://iad.sxryk.cn

[S39] C++：自定义比较器排序
来源：http://wgh.hnqzz.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nid.jinqigufen.top

[S40] C++：查找元素
来源：http://jsk.yfazqb.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jys.cheryme.top

[S41] C++：类与构造函数
来源：http://mxv.yangfankeji.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dqw.cashguo.top

[S42] C++：继承与虚函数
来源：http://fce.xingfuxueyuan.xyz

class B : public Base { public: void f() override {} };
来源：http://mpr.shanyushiyangtech.top

[S43] C++：智能指针
来源：http://lgf.hfpthk.cn

auto p = std::make_unique<int>(5);
来源：http://tiq.shanyushiyangkeji.top

[S44] C++：引用传参
来源：http://rju.xuanzx.com

void inc(int &x) { ++x; }
来源：http://idu.sweek.top

[S45] C++：lambda
来源：http://pun.fehbvm.com

auto add = [](int a, int b) { return a + b; };
来源：http://yfc.xylfe.cn

[S46] C++：函数模板
来源：http://dgj.hammf.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vje.xingfuxueyuan.xyz

[S47] C++：结构化绑定遍历
来源：http://caf.shangyingyoupin.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gvy.nwbrower.top

[S48] C++：逐行读文件
来源：http://dir.haohaochexian.top

std::ifstream in("a.txt");  std::string line;
来源：http://hme.tianlin.xyz

while (std::getline(in, line)) { }
来源：http://ugp.bjfxy.top

[S49] C++：写文件
来源：http://foy.sufxvd.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qfz.sysykeji.top

[S50] C++：格式化数字
来源：http://cpj.gogol.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xha.shzxlz.cn

[S51] C++：显式类型转换
来源：http://bzh.hongshengwenyu.top

static_cast<double>(a) / b
来源：http://ifm.nanxuanxn.top

[S52] C++：const 与 noexcept
来源：http://xap.zhixingplan.top

int size() const noexcept { return n_; }
来源：http://utd.meibo888.top

[S53] C++：移动语义
来源：http://rnu.xuetiantiany.cn

std::vector<int> w = std::move(v);
来源：http://eiy.cashguo.top

[S54] C++：异常处理
来源：http://llf.zhixingplan.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lup.daxiang520.top

[S55] C++：结构化绑定
来源：http://fkb.gzhubu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ilu.uphjek.com

[S56] C++：optional
来源：http://swk.daria6918.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vhh.jiagoushi.top

[S57] C++：编译期常量
来源：http://hfn.pycfn.com

constexpr int N = 10;
来源：http://ctm.316326.xyz

[S58] C++：命名空间
来源：http://dwp.fzhhl.top

namespace ns { int f() { return 1; } }
来源：http://wcq.vqdsnc.cn

[S59] C++：静态断言
来源：http://vka.shuidangran.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dip.hfpthk.cn

[S60] C++：遍历并删除元素
来源：http://awc.chenjidiqi.icu

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yoo.ivvv.top

================================================================================
来源：http://dvv.yj20258.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ndx.yonumen.top

================================================================================
来源：http://mrm.snrcjt.cn

[T01] Kotlin：Hello World
来源：http://ipa.cdnleiting.top

println("Hello")
来源：http://iet.zhoulong.xyz

[T02] Kotlin：变量
来源：http://lpl.jqgfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ntn.sysykeji.top

[T03] Kotlin：字符串模板
来源：http://pos.xinyue.icu

"值: $b"
来源：http://zbb.sweek.top

[T04] Kotlin：空安全
来源：http://hlh.wangdashe.top

val n: String? = null;  n?.length
来源：http://glx.xuanzx.com

[T05] Kotlin：when 表达式
来源：http://hyx.guowangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hpu.sufxvd.cn

[T06] Kotlin：集合映射
来源：http://hmw.sjlbkw.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://oxw.jyoumei.cn

[T07] Kotlin：集合过滤
来源：http://fjj.hesvh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jeq.xuanzx.com

[T08] Kotlin：数据类
来源：http://dez.mhx1999.top

data class User(val name: String, val age: Int)
来源：http://qic.vehdjk.com

[T09] Kotlin：扩展函数
来源：http://xgn.aizwys.cn

fun String.exclaim() = this + "!"
来源：http://ubb.yj20258888.top

[T10] Kotlin：默认参数
来源：http://nyv.jinqigufen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://xup.hcnkem.com

[T11] Kotlin：协程
来源：http://vtl.chenjidiqi.icu

GlobalScope.launch { delay(1000); println("done") }
来源：http://vqb.jinqigufen.top

[T12] Kotlin：解构声明
来源：http://yzs.ywan-chungtsiang.top

val (a, b) = Pair(1, 2)
来源：http://mst.meibo888.top

[T13] Kotlin：只读 Map
来源：http://onj.nwbrower.top

val m = mapOf("a" to 1)
来源：http://acx.xylfe.cn

[T14] Kotlin：循环
来源：http://rax.cqqwz.cn

for (i in 1..10) println(i)
来源：http://fxf.dianchejie.cn

[T15] Kotlin：接口
来源：http://cmj.jyoumei.cn

interface Shape { fun area(): Double }
来源：http://lsq.jinghuilouyu.cn

[T16] Swift：Hello World
来源：http://mku.snrcjt.cn

print("Hello")
来源：http://dqk.vehdjk.com

[T17] Swift：变量与常量
来源：http://fsk.meibo888.top

var a = 1;  let b = 2
来源：http://mmy.xuetiantiany.cn

[T18] Swift：字符串插值
来源：http://fzs.nwbrower.top

"值: \(b)"
来源：http://isl.yvedp.cn

[T19] Swift：可选绑定
来源：http://tbo.xingfuxueyuan.xyz

if let n = opt { print(n) }
来源：http://xqc.jinqigfzy.top

[T20] Swift：数组操作
来源：http://uka.ehwqpu.com

var a = [1, 2, 3];  a.append(4)
来源：http://kwf.fktsv.cn

[T21] Swift：遍历
来源：http://dlb.yfazqb.com

for x in a { print(x) }
来源：http://kqk.hesvh.cn

[T22] Swift：字典
来源：http://ylb.dianchejie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dae.sweek.top

[T23] Swift：函数
来源：http://rgc.yvedp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://els.daxiang520.top

[T24] Swift：闭包
来源：http://zyk.fanxiaobao.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://rpc.hysaishi.cn

[T25] Swift：结构体
来源：http://vat.guannengcc.top

struct P { var x: Int }
来源：http://snp.zycfv.cn

[T26] Swift：类与重写
来源：http://yoi.xylfe.cn

class A: Base { override func f() {} }
来源：http://vok.hnxiangtu.top

[T27] Swift：错误处理
来源：http://tse.c1oappe.top

do { try f() } catch { print(error) }
来源：http://zeo.sysykeji.top

[T28] Swift：枚举
来源：http://tjc.fehbvm.com

enum Color { case red, green }
来源：http://sxq.tanke756.top

[T29] Swift：guard 提前返回
来源：http://gpb.jianghu66.top

guard let x = opt else { return }
来源：http://rfs.xuetiantiany.cn

[T30] Swift：协议
来源：http://cmg.ctjpmb.com

protocol Shape { func area() -> Double }
来源：http://mhc.yueranfly.top

[T31] Lua：Hello World
来源：http://slv.fengsongda.top

print("Hello")
来源：http://rwa.jlsjyb.cn

[T32] Lua：局部变量
来源：http://rbg.chenlongwang.top

local a = 1
来源：http://dxh.nwbrower.top

[T33] Lua：表（数组）
来源：http://gjc.iojbl.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kld.yj20258.top

[T34] Lua：遍历表
来源：http://doy.guowangkeji.top

for i, v in ipairs(t) do print(i, v) end
来源：http://xus.tanke756.top

[T35] Lua：字典表
来源：http://een.snrcjt.cn

local d = { a = 1 };  d.b = 2
来源：http://jpg.zhijiandao.cn

[T36] Lua：函数
来源：http://rto.zhongyouzk.top

function add(a, b) return a + b end
来源：http://pie.guannengcc.top

[T37] Lua：字符串拼接
来源：http://pxx.tianlin.xyz

"a" .. "b"
来源：http://tez.yangfankeji.com

[T38] Lua：条件
来源：http://tmd.zhijiandao.cn

if x > 0 then print("正") end
来源：http://ade.sweek.top

[T39] Lua：模式匹配
来源：http://mrt.hammf.cn

string.find(s, "%d+")
来源：http://lna.zhaomingkeji.xyz

[T40] Lua：元表
来源：http://mtm.yuanzhike.top

setmetatable({}, { __index = base })
来源：http://amf.fanxiaobao.xyz

[T41] Perl：Hello World
来源：http://nfi.xziqi.cn

print "Hello\n";
来源：http://ipb.hfpthk.cn

[T42] Perl：变量类型
来源：http://rfs.yvedp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wuo.epnwcf.com

[T43] Perl：字符串插值
来源：http://dao.gzhubu.top

"值: $a"
来源：http://avi.aibaodan.cn

[T44] Perl：条件
来源：http://srd.zycfv.cn

if ($a > 0) { print "正"; }
来源：http://doy.hywenlv.cn

[T45] Perl：数组遍历
来源：http://hzi.gaohongyu789.top

for my $x (@arr) { print $x; }
来源：http://ofs.xuetiantiany.cn

[T46] Perl：哈希操作
来源：http://ffl.0kj1m.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qgo.shangyingyoupin.top

[T47] Perl：正则捕获
来源：http://swk.jinqigufen.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://swb.havefunace.top

[T48] Perl：正则替换
来源：http://zoz.sjlbkw.cn

$s =~ s/old/new/g;
来源：http://cpf.fehbvm.com

[T49] Perl：函数
来源：http://neb.yueranfly.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zpx.jinyuanbaomall.cn

[T50] Perl：逐行读文件
来源：http://gps.shanyushiyangtech.top

open my $fh, "<", "a.txt" or die $!;
来源：http://zds.birdmap.top

while (my $line = <$fh>) { print $line; }
来源：http://odh.bjfxy.top

[T51] Scala：Hello World
来源：http://vns.cheryme.top

println("Hello")
来源：http://etb.zhixingplan.top

[T52] Scala：变量
来源：http://dbk.gogol.net.cn

val a = 1;  var b = 2
来源：http://mos.sufxvd.cn

[T53] Scala：字符串插值
来源：http://hta.kuanghao11.cn

s"值: $b"
来源：http://jzy.yanxiufei.cn

[T54] Scala：集合映射
来源：http://fnd.hongshengwenyu.top

List(1, 2, 3).map(_ * 2)
来源：http://bhd.nanxuanxn.top

[T55] Scala：集合过滤
来源：http://isk.zdbjq.cn

List(1, 2, 3).filter(_ > 1)
来源：http://noj.yuanzhike.top

[T56] Scala：样例类
来源：http://thn.xinyue.icu

case class User(name: String, age: Int)
来源：http://jmr.wangdashe.top

[T57] Scala：模式匹配
来源：http://pwm.nanxuanxn.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://bck.ybcxt.top

[T58] Scala：函数定义
来源：http://svn.xuanzx.com

def add(a: Int, b: Int): Int = a + b
来源：http://lsd.zhijiandao.cn

[T59] Scala：循环
来源：http://orq.bjfxy.top

for (i <- 1 to 10) println(i)
来源：http://ykv.uphjek.com

[T60] Scala：折叠
来源：http://rpv.andypj.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://npv.gogol.net.cn

================================================================================
来源：http://yja.yongpay.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ccg.zhengqikj.top

================================================================================
来源：http://lmw.dashuyun.cn

[U01] Py：创建虚拟环境
来源：http://usk.ivvv.top

python -m venv .venv && source .venv/bin/activate
来源：http://qqp.yfazqb.com

[U02] Py：导出 / 安装依赖
来源：http://fem.yangfankeji.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://azs.chenzaomai.com

[U03] Py：加载 .env 配置
来源：http://pix.hywenlv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://afx.chenjidiqi.icu

[U04] Py：变量调试打印
来源：http://bev.aibaodan.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uuq.jinqigufen.top

[U05] Py：列表去重且保序
来源：http://kbe.hongshengwenyu.top

list(dict.fromkeys(arr))
来源：http://wib.quarkkingdee.top

[U06] Py：合并两个字典
来源：http://lnm.yj20258888.top

{**a, **b}
来源：http://pnz.tian-w.cn

[U07] Py：反转字典键值
来源：http://xcs.yj202588.top

{v: k for k, v in d.items()}
来源：http://snt.nwbrower.top

[U08] Py：展平二维列表
来源：http://jjw.yongpay.top

[y for x in nested for y in x]
来源：http://pvr.pycfn.com


<!-- 参考信息 -->