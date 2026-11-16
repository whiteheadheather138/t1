代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://ade.bbcook.cn

[R70] 时间戳与互转
来源：http://sdz.shanyushiyangkeji.top

date +%s;  date -d @1700000000
来源：http://kjw.shanyushiyangkeji.top

[R71] 日期格式化
来源：http://ufs.yanxiufei.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qgk.fanxiaobao.xyz

[R72] 等待端口就绪
来源：http://lvd.nanxinkj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://hsd.kuanghao11.cn

[R73] 分割大日志
来源：http://vro.bjfxy.top

split -l 1000 big.log part_
来源：http://zzi.aibaodan.cn

[R74] 批量重命名
来源：http://jgs.jinqigfzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wlh.zhixingplan.top

[R75] 导出环境变量
来源：http://dya.yj20258888.top

export PATH="$HOME/bin:$PATH"
来源：http://obe.zdbjq.cn

[R76] 使用临时文件
来源：http://ujc.0kj1m.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qyu.gaohongyu789.top

[R77] 读取用户输入
来源：http://sfn.aizwys.cn

read -rp "请输入: " ans
来源：http://mdp.hammf.cn

[R78] 交互式菜单
来源：http://dfi.uphjek.com

select opt in a b c; do echo "$opt"; break; done
来源：http://sgt.jinyuanbaomall.cn

[R79] 解析命令行选项
来源：http://qpc.dianchejie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jns.aizwys.cn

[R80] 查看脚本执行耗时
来源：http://uir.zdbjq.cn

time ./run.sh
来源：http://ufy.fehbvm.com

================================================================================
来源：http://eqd.zhijiandao.cn

S. C / C++ 专题
来源：http://ubr.cqqwz.cn

================================================================================
来源：http://jnr.mhx1999.top

[S01] C：Hello World
来源：http://vrs.daria6918.cn

#include <stdio.h>
来源：http://pmi.dashuyun.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gvg.yuanzhike.top

[S02] C：变量与格式化输出
来源：http://ejj.fktsv.cn

int a = 10; printf("%d\n", a);
来源：http://gkk.jiagoushi.top

[S03] C：读入整数
来源：http://fis.hnxiangtu.top

int x; scanf("%d", &x);
来源：http://tzh.cqqwz.cn

[S04] C：字符串复制
来源：http://rlh.quarkkingdee.top

char dst[32]; strcpy(dst, "hi");
来源：http://kpb.nwbrower.top

[S05] C：字符串长度
来源：http://ejs.0kj1m.cn

strlen(s)
来源：http://npu.sysykeji.top

[S06] C：字符串比较
来源：http://yle.svipenyu.cn

strcmp(a, b) == 0
来源：http://pgn.xuanzx.com

[S07] C：数组遍历求和
来源：http://niu.hesvh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://llf.yonumen.top

[S08] C：动态内存分配与释放
来源：http://kdu.tian-w.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ywi.zhaomingkeji.xyz

[S09] C：结构体定义与初始化
来源：http://ofj.xinyue.icu

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://chv.hongshengwenyu.top

[S10] C：指针与解引用
来源：http://fge.shzxlz.cn

int *p = &a;  *p = 5;
来源：http://oyb.daria6918.cn

[S11] C：逐行读文件
来源：http://hla.gzhubu.top

FILE *f = fopen("a.txt", "r");
来源：http://fok.mhx1999.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://kae.yongpay.top

fclose(f);
来源：http://ejn.pycfn.com

[S12] C：写文件
来源：http://cyd.ctjpmb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://djq.dianchejie.cn

[S13] C：宏定义
来源：http://vla.nanxuanxn.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lyw.jinghuilouyu.cn

[S14] C：枚举
来源：http://iyq.cashguo.top

enum Color { RED, GREEN, BLUE };
来源：http://zsy.chenlongwang.top

[S15] C：类型转换
来源：http://wyk.tarul.cn

(double) a / b
来源：http://njo.shuidangran.top

[S16] C：位操作置位
来源：http://yia.gogol.net.cn

x |= (1 << 3);
来源：http://coj.0kj1m.cn

[S17] C：安全拼接字符串
来源：http://xkl.daxiang520.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tpe.smart0.xyz

[S18] C：命令行参数
来源：http://lam.fktsv.cn

int main(int argc, char **argv)
来源：http://jbc.jlsjyb.cn

[S19] C：快速排序
来源：http://jan.chenlongwang.top

qsort(a, n, sizeof(int), cmp);
来源：http://btf.pengpengdd.cyou

[S20] C：二分查找
来源：http://pyn.andypj.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dnr.zhongyouzk.top

[S21] C：字符类别判断
来源：http://nib.mhx1999.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bcx.0kj1m.cn

[S22] C：字符串转数字
来源：http://vyv.dianchejie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rno.yuanzhike.top

[S23] C：随机数
来源：http://sap.smart0.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://lta.daxiang520.top

[S24] C：获取本地时间
来源：http://pye.havefunace.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hgq.vehdjk.com

[S25] C：内存拷贝
来源：http://xie.meibo888.top

memcpy(dst, src, n);
来源：http://ojx.9152youxi.cn

[S26] C：内存清零
来源：http://ilr.gaohongyu789.top

memset(a, 0, sizeof a);
来源：http://oyz.vehdjk.com

[S27] C：定义常量
来源：http://spm.kuanghao11.cn

const double PI = 3.14159;
来源：http://rop.zhengqikj.top

[S28] C：静态变量
来源：http://qhy.hammf.cn

static int counter = 0;
来源：http://djh.wangshuangyany.cn

[S29] C：变参函数
来源：http://qgr.sweek.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ulh.pycfn.com

[S30] C：头文件保护
来源：http://lfo.c1oappe.top

#ifndef X_H
来源：http://zoy.dianchejie.cn

#define X_H
来源：http://lec.ivvv.top

#endif
来源：http://rnm.haohaochexian.top

[S31] C++：Hello World
来源：http://bxm.yfazqb.com

#include <iostream>
来源：http://whz.yanxiufei.cn

int main() { std::cout << "Hello\n"; }
来源：http://fjc.ydjk.org.cn

[S32] C++：字符串
来源：http://jax.shanyushiyangtech.top

std::string s = "hi";  s += "!";
来源：http://zux.zhaomingkeji.xyz

[S33] C++：vector 增删
来源：http://gkk.zhiwuduotai.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tip.fehbvm.com

[S34] C++：遍历 vector
来源：http://mme.zhiwuduotai.top

for (auto &x : v) { std::cout << x; }
来源：http://nwn.xziqi.cn

[S35] C++：map
来源：http://qvc.pycfn.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cek.tanke756.top

[S36] C++：unordered_map
来源：http://mqw.yj20258.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tby.cashguo.top

[S37] C++：set
来源：http://ddm.ydjk.org.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ikn.epnwcf.com

[S38] C++：排序
来源：http://nrn.hysaishi.cn

std::sort(v.begin(), v.end());
来源：http://dzv.yanxiufei.cn

[S39] C++：自定义比较器排序
来源：http://cyq.tian-w.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sbc.sysykeji.top

[S40] C++：查找元素
来源：http://cvv.yanxiufei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nfy.wangdashe.top

[S41] C++：类与构造函数
来源：http://bvl.jinyuanbaomall.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cfa.cheryme.top

[S42] C++：继承与虚函数
来源：http://got.fzhhl.top

class B : public Base { public: void f() override {} };
来源：http://jia.fehbvm.com

[S43] C++：智能指针
来源：http://rlt.jinqigufen.top

auto p = std::make_unique<int>(5);
来源：http://elv.daxiang520.top

[S44] C++：引用传参
来源：http://nfe.jinqigufen.top

void inc(int &x) { ++x; }
来源：http://jqu.zdqjudy.top

[S45] C++：lambda
来源：http://aty.shanyushiyangkeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://hju.xuanzx.com

[S46] C++：函数模板
来源：http://zwo.birdmap.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vlk.hnqzz.top

[S47] C++：结构化绑定遍历
来源：http://qqw.jiagoushi.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cwx.zhengqikj.top

[S48] C++：逐行读文件
来源：http://mcb.cashguo.top

std::ifstream in("a.txt");  std::string line;
来源：http://uuc.shuidangran.top

while (std::getline(in, line)) { }
来源：http://ygt.bbcook.cn

[S49] C++：写文件
来源：http://zxs.aibaodan.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ypm.ppjwa.cn

[S50] C++：格式化数字
来源：http://dkj.pengpengdd.cyou

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://omm.ydjk.org.cn

[S51] C++：显式类型转换
来源：http://bwr.tanke756.top

static_cast<double>(a) / b
来源：http://bay.bbcook.cn

[S52] C++：const 与 noexcept
来源：http://ler.fzhhl.top

int size() const noexcept { return n_; }
来源：http://xdb.vqdsnc.cn

[S53] C++：移动语义
来源：http://spb.zycfv.cn

std::vector<int> w = std::move(v);
来源：http://lvj.zhoulong.xyz

[S54] C++：异常处理
来源：http://gsz.ppjwa.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uya.nwbrower.top

[S55] C++：结构化绑定
来源：http://adc.hesvh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://maq.dianchejie.cn

[S56] C++：optional
来源：http://vej.cheryme.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fkh.aibaodan.cn

[S57] C++：编译期常量
来源：http://abb.yj20258.top

constexpr int N = 10;
来源：http://byy.sufxvd.cn

[S58] C++：命名空间
来源：http://bmo.fengsongda.top

namespace ns { int f() { return 1; } }
来源：http://iyf.zhoulong.xyz

[S59] C++：静态断言
来源：http://gzn.tanke756.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://voy.ppjwa.cn

[S60] C++：遍历并删除元素
来源：http://alg.jiagoushi.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://say.yonumen.top

================================================================================
来源：http://ksn.cdnleiting.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vii.wangdashe.top

================================================================================
来源：http://naw.yvedp.cn

[T01] Kotlin：Hello World
来源：http://kgy.tian-w.cn

println("Hello")
来源：http://mns.yj20258888.top

[T02] Kotlin：变量
来源：http://ehi.andypj.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ilc.havefunace.top

[T03] Kotlin：字符串模板
来源：http://jsl.jyoumei.cn

"值: $b"
来源：http://szq.uphjek.com

[T04] Kotlin：空安全
来源：http://zxe.ybcxt.top

val n: String? = null;  n?.length
来源：http://olv.hongshengwenyu.top

[T05] Kotlin：when 表达式
来源：http://vfh.9152youxi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dev.jinqigufen.top

[T06] Kotlin：集合映射
来源：http://snj.c1oappe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://nus.ywan-chungtsiang.top

[T07] Kotlin：集合过滤
来源：http://wnp.chenlongwang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://iyz.svipenyu.cn

[T08] Kotlin：数据类
来源：http://jbv.havefunace.top

data class User(val name: String, val age: Int)
来源：http://pxs.jinyuanbaomall.cn

[T09] Kotlin：扩展函数
来源：http://kri.kuanghao11.cn

fun String.exclaim() = this + "!"
来源：http://gfq.wangshuangyany.cn

[T10] Kotlin：默认参数
来源：http://aib.shuidangran.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ajo.shzxlz.cn

[T11] Kotlin：协程
来源：http://hok.dashuyun.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fvo.yfazqb.com

[T12] Kotlin：解构声明
来源：http://pxt.smart0.xyz

val (a, b) = Pair(1, 2)
来源：http://pbz.ybcxt.top

[T13] Kotlin：只读 Map
来源：http://muw.zhiwuduotai.top

val m = mapOf("a" to 1)
来源：http://qfq.yueranfly.top

[T14] Kotlin：循环
来源：http://mmh.tianlin.xyz

for (i in 1..10) println(i)
来源：http://gtw.jinqigufen.top

[T15] Kotlin：接口
来源：http://juf.cdnleiting.top

interface Shape { fun area(): Double }
来源：http://pdi.cheryme.top

[T16] Swift：Hello World
来源：http://cuu.ybcxt.top

print("Hello")
来源：http://jpr.redwolf501.top

[T17] Swift：变量与常量
来源：http://unf.uphjek.com

var a = 1;  let b = 2
来源：http://rnq.daria6918.cn

[T18] Swift：字符串插值
来源：http://tqh.bbcook.cn

"值: \(b)"
来源：http://fdz.xuetiantiany.cn

[T19] Swift：可选绑定
来源：http://vzq.quarkkingdee.top

if let n = opt { print(n) }
来源：http://umh.vehdjk.com

[T20] Swift：数组操作
来源：http://xlr.dianchejie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pfd.yangfankeji.com

[T21] Swift：遍历
来源：http://xhz.vqdsnc.cn

for x in a { print(x) }
来源：http://xef.fehbvm.com

[T22] Swift：字典
来源：http://who.hammf.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uvu.havefunace.top

[T23] Swift：函数
来源：http://xre.nwbrower.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nso.yj20258.top

[T24] Swift：闭包
来源：http://njs.yuxming.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ryd.sysykeji.top

[T25] Swift：结构体
来源：http://kyg.chenlongwang.top

struct P { var x: Int }
来源：http://oxa.sysykeji.top

[T26] Swift：类与重写
来源：http://thg.snrcjt.cn

class A: Base { override func f() {} }
来源：http://sda.tian-w.cn

[T27] Swift：错误处理
来源：http://wwo.pycfn.com

do { try f() } catch { print(error) }
来源：http://rii.zycfv.cn

[T28] Swift：枚举
来源：http://uob.ywan-chungtsiang.top

enum Color { case red, green }
来源：http://gil.hongshengwenyu.top

[T29] Swift：guard 提前返回
来源：http://cdl.svipenyu.cn

guard let x = opt else { return }
来源：http://upc.zhijiandao.cn

[T30] Swift：协议
来源：http://mck.xziqi.cn

protocol Shape { func area() -> Double }
来源：http://bsy.meibo888.top

[T31] Lua：Hello World
来源：http://oil.ehwqpu.com

print("Hello")
来源：http://oog.zhoulong.xyz

[T32] Lua：局部变量
来源：http://xii.zdqjudy.top

local a = 1
来源：http://zsz.jinghuilouyu.cn

[T33] Lua：表（数组）
来源：http://eff.fzhhl.top

local t = {1, 2, 3};  t[4] = 4
来源：http://rlb.zhengqikj.top

[T34] Lua：遍历表
来源：http://boy.52xcode.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://egj.ctjpmb.com

[T35] Lua：字典表
来源：http://mzo.bbcook.cn

local d = { a = 1 };  d.b = 2
来源：http://jmm.hfpthk.cn

[T36] Lua：函数
来源：http://mzw.shanyushiyangtech.top

function add(a, b) return a + b end
来源：http://xaf.jinqigfzy.top

[T37] Lua：字符串拼接
来源：http://vrf.sysykeji.top

"a" .. "b"
来源：http://rdv.hnxiangtu.top

[T38] Lua：条件
来源：http://kuf.jianghu66.top

if x > 0 then print("正") end
来源：http://mep.jqgfzy.top

[T39] Lua：模式匹配
来源：http://iow.hcnkem.com

string.find(s, "%d+")
来源：http://fkj.redwolf501.top

[T40] Lua：元表
来源：http://mmr.meibo888.top

setmetatable({}, { __index = base })
来源：http://kel.wangshuangyany.cn

[T41] Perl：Hello World
来源：http://oiu.jinghuilouyu.cn

print "Hello\n";
来源：http://gfw.meibo888.top

[T42] Perl：变量类型
来源：http://nro.tianlin.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kmv.tianlin.xyz

[T43] Perl：字符串插值
来源：http://tvq.jlsjyb.cn

"值: $a"
来源：http://xst.zhengqikj.top

[T44] Perl：条件
来源：http://kof.aizwys.cn

if ($a > 0) { print "正"; }
来源：http://zmm.quarkkingdee.top

[T45] Perl：数组遍历
来源：http://nlw.hysaishi.cn

for my $x (@arr) { print $x; }
来源：http://qsb.nanxuanxn.top

[T46] Perl：哈希操作
来源：http://qka.jqgufenzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jib.daria6918.cn

[T47] Perl：正则捕获
来源：http://uvu.ppjwa.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ajb.smart0.xyz

[T48] Perl：正则替换
来源：http://wwp.yanxiufei.cn

$s =~ s/old/new/g;
来源：http://xbk.fengsongda.top

[T49] Perl：函数
来源：http://kdq.9152youxi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://teh.hnxiangtu.top

[T50] Perl：逐行读文件
来源：http://tks.smart0.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://gsl.yj202588.top

while (my $line = <$fh>) { print $line; }
来源：http://qrc.epnwcf.com

[T51] Scala：Hello World
来源：http://wwz.jqgfzy.top

println("Hello")
来源：http://zfg.meibo888.top

[T52] Scala：变量
来源：http://jpz.tian-w.cn

val a = 1;  var b = 2
来源：http://iox.gzhubu.top

[T53] Scala：字符串插值
来源：http://mla.vqdsnc.cn

s"值: $b"
来源：http://tqf.tarul.cn

[T54] Scala：集合映射
来源：http://iyw.shzxlz.cn

List(1, 2, 3).map(_ * 2)
来源：http://kei.birdmap.top

[T55] Scala：集合过滤
来源：http://hph.sweek.top

List(1, 2, 3).filter(_ > 1)
来源：http://sti.zhixingplan.top

[T56] Scala：样例类
来源：http://toq.vehdjk.com

case class User(name: String, age: Int)
来源：http://ipb.cqqwz.cn

[T57] Scala：模式匹配
来源：http://nfh.sufxvd.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qea.xinyue.icu

[T58] Scala：函数定义
来源：http://khb.tanke756.top

def add(a: Int, b: Int): Int = a + b
来源：http://plp.bbcook.cn

[T59] Scala：循环
来源：http://zwp.daxiang520.top

for (i <- 1 to 10) println(i)
来源：http://syf.vehdjk.com

[T60] Scala：折叠
来源：http://uwp.snrcjt.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ixa.tarul.cn

================================================================================
来源：http://xwo.redwolf501.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tnx.jinqigufen.top

================================================================================
来源：http://ldq.yj20258.top

[U01] Py：创建虚拟环境
来源：http://aqs.dashuyun.cn

python -m venv .venv && source .venv/bin/activate
来源：http://frr.zhengqikj.top

[U02] Py：导出 / 安装依赖
来源：http://ydz.feifeiyinyue.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ifi.snrcjt.cn

[U03] Py：加载 .env 配置
来源：http://avo.zhengqikj.top

from dotenv import load_dotenv; load_dotenv()
来源：http://txw.cqqwz.cn

[U04] Py：变量调试打印
来源：http://tce.snrcjt.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bbj.shangyingyoupin.top

[U05] Py：列表去重且保序
来源：http://ndj.gotoacloud.top

list(dict.fromkeys(arr))
来源：http://xrz.nwbrower.top

[U06] Py：合并两个字典
来源：http://omb.tianlin.xyz

{**a, **b}
来源：http://ekx.guowangkeji.top

[U07] Py：反转字典键值
来源：http://ntu.jinqigufen.top

{v: k for k, v in d.items()}
来源：http://hvn.xinyue.icu

[U08] Py：展平二维列表
来源：http://ppx.hesvh.cn

[y for x in nested for y in x]
来源：http://xrr.ybcxt.top

[U09] Py：字典取最大值的键
来源：http://efr.cucudq.cn

max(d, key=d.get)
来源：http://ejw.haohaochexian.top

[U10] Py：按值排序字典
来源：http://zga.smart0.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://syc.ydjk.org.cn


<!-- 参考信息 -->