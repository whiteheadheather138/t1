代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://kmy.guowangkeji.top

[R76] 使用临时文件
来源：http://cro.jinghuilouyu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mxs.haohaochexian.top

[R77] 读取用户输入
来源：http://gvb.yuanzhike.top

read -rp "请输入: " ans
来源：http://dkx.mhx1999.top

[R78] 交互式菜单
来源：http://mlf.zhixingplan.top

select opt in a b c; do echo "$opt"; break; done
来源：http://khr.sxryk.cn

[R79] 解析命令行选项
来源：http://iia.jiagoushi.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cjs.tanke756.top

[R80] 查看脚本执行耗时
来源：http://ooh.chenzaomai.com

time ./run.sh
来源：http://dsd.pengpengdd.cyou

================================================================================
来源：http://ula.ppjwa.cn

S. C / C++ 专题
来源：http://dvx.52xcode.cn

================================================================================
来源：http://kcz.chenzaomai.com

[S01] C：Hello World
来源：http://dim.kuanghao11.cn

#include <stdio.h>
来源：http://oes.mhx1999.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://dqi.fengsongda.top

[S02] C：变量与格式化输出
来源：http://hmu.pycfn.com

int a = 10; printf("%d\n", a);
来源：http://qmi.nanxuanxn.top

[S03] C：读入整数
来源：http://hwm.shuidangran.top

int x; scanf("%d", &x);
来源：http://eig.meibo888.top

[S04] C：字符串复制
来源：http://lpu.chenlongwang.top

char dst[32]; strcpy(dst, "hi");
来源：http://mtz.zdbjq.cn

[S05] C：字符串长度
来源：http://teo.meibo888.top

strlen(s)
来源：http://hub.quarkkingdee.top

[S06] C：字符串比较
来源：http://xzx.dianchejie.cn

strcmp(a, b) == 0
来源：http://clw.chenjidiqi.icu

[S07] C：数组遍历求和
来源：http://ykt.yanxiufei.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yes.feifeiyinyue.top

[S08] C：动态内存分配与释放
来源：http://qbu.yj20258888.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jwc.xylfe.cn

[S09] C：结构体定义与初始化
来源：http://cin.hywenlv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kul.dashuyun.cn

[S10] C：指针与解引用
来源：http://amw.jyoumei.cn

int *p = &a;  *p = 5;
来源：http://obq.bjfxy.top

[S11] C：逐行读文件
来源：http://zgi.sweek.top

FILE *f = fopen("a.txt", "r");
来源：http://zih.vqdsnc.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fjt.bjfxy.top

fclose(f);
来源：http://qqj.jqgufenzy.top

[S12] C：写文件
来源：http://bta.hnqzz.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mso.xziqi.cn

[S13] C：宏定义
来源：http://kfn.havefunace.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tyc.daxiang520.top

[S14] C：枚举
来源：http://ylb.daxiang520.top

enum Color { RED, GREEN, BLUE };
来源：http://jqq.snrcjt.cn

[S15] C：类型转换
来源：http://wzy.daria6918.cn

(double) a / b
来源：http://vut.quarkkingdee.top

[S16] C：位操作置位
来源：http://qee.hesvh.cn

x |= (1 << 3);
来源：http://ymg.jinqigufen.top

[S17] C：安全拼接字符串
来源：http://lqm.tarul.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tur.fengsongda.top

[S18] C：命令行参数
来源：http://pqu.meibo888.top

int main(int argc, char **argv)
来源：http://bid.fzhhl.top

[S19] C：快速排序
来源：http://zhi.yonumen.top

qsort(a, n, sizeof(int), cmp);
来源：http://xmm.andypj.xyz

[S20] C：二分查找
来源：http://dpy.zdqjudy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zrl.hammf.cn

[S21] C：字符类别判断
来源：http://mls.shuidangran.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://odq.vqdsnc.cn

[S22] C：字符串转数字
来源：http://qaj.jqgfzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://xbp.zhoulong.xyz

[S23] C：随机数
来源：http://efa.sufxvd.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ndo.xziqi.cn

[S24] C：获取本地时间
来源：http://xom.jinghuilouyu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rol.fktsv.cn

[S25] C：内存拷贝
来源：http://lib.bjfxy.top

memcpy(dst, src, n);
来源：http://zgf.zycfv.cn

[S26] C：内存清零
来源：http://ftc.jinyuanbaomall.cn

memset(a, 0, sizeof a);
来源：http://jil.hammf.cn

[S27] C：定义常量
来源：http://vxn.quarkkingdee.top

const double PI = 3.14159;
来源：http://cno.ivvv.top

[S28] C：静态变量
来源：http://uil.wangdashe.top

static int counter = 0;
来源：http://jhn.chenzaomai.com

[S29] C：变参函数
来源：http://mur.svipenyu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://myk.pycfn.com

[S30] C：头文件保护
来源：http://nio.fktsv.cn

#ifndef X_H
来源：http://tgc.jiagoushi.top

#define X_H
来源：http://fjc.tian-w.cn

#endif
来源：http://aiy.sxryk.cn

[S31] C++：Hello World
来源：http://mxu.dianchejie.cn

#include <iostream>
来源：http://vlx.fktsv.cn

int main() { std::cout << "Hello\n"; }
来源：http://dhb.jyoumei.cn

[S32] C++：字符串
来源：http://fzb.fzhhl.top

std::string s = "hi";  s += "!";
来源：http://quj.shanyushiyangkeji.top

[S33] C++：vector 增删
来源：http://noa.ywan-chungtsiang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dqe.pengpengdd.cyou

[S34] C++：遍历 vector
来源：http://qag.mhx1999.top

for (auto &x : v) { std::cout << x; }
来源：http://ohe.bbcook.cn

[S35] C++：map
来源：http://dgl.zhongyouzk.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://flq.ivvv.top

[S36] C++：unordered_map
来源：http://uuf.andypj.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vqy.gaohongyu789.top

[S37] C++：set
来源：http://csd.birdmap.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ptb.hcnkem.com

[S38] C++：排序
来源：http://blj.zhongyouzk.top

std::sort(v.begin(), v.end());
来源：http://ylw.gogol.net.cn

[S39] C++：自定义比较器排序
来源：http://qil.guowangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://htf.sweek.top

[S40] C++：查找元素
来源：http://rus.jinqigfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mtl.jianghu66.top

[S41] C++：类与构造函数
来源：http://tzb.nwbrower.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://enz.ctjpmb.com

[S42] C++：继承与虚函数
来源：http://pmh.birdmap.top

class B : public Base { public: void f() override {} };
来源：http://ior.fengsongda.top

[S43] C++：智能指针
来源：http://chn.zhaomingkeji.xyz

auto p = std::make_unique<int>(5);
来源：http://nlx.ybcxt.top

[S44] C++：引用传参
来源：http://lih.shanyushiyangtech.top

void inc(int &x) { ++x; }
来源：http://xxd.bjfxy.top

[S45] C++：lambda
来源：http://hhk.vqdsnc.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kek.zycfv.cn

[S46] C++：函数模板
来源：http://iur.pengpengdd.cyou

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lop.daxiang520.top

[S47] C++：结构化绑定遍历
来源：http://yyt.zhiwuduotai.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fnh.jyoumei.cn

[S48] C++：逐行读文件
来源：http://ucp.yongpay.top

std::ifstream in("a.txt");  std::string line;
来源：http://vpc.vqdsnc.cn

while (std::getline(in, line)) { }
来源：http://usx.andypj.xyz

[S49] C++：写文件
来源：http://kbd.tanke756.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eel.havefunace.top

[S50] C++：格式化数字
来源：http://tsd.jianghu66.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oja.hywenlv.cn

[S51] C++：显式类型转换
来源：http://nuv.cashguo.top

static_cast<double>(a) / b
来源：http://sra.zdqjudy.top

[S52] C++：const 与 noexcept
来源：http://pzd.snrcjt.cn

int size() const noexcept { return n_; }
来源：http://gfk.wangshuangyany.cn

[S53] C++：移动语义
来源：http://lyj.yueranfly.top

std::vector<int> w = std::move(v);
来源：http://kug.feifeiyinyue.top

[S54] C++：异常处理
来源：http://gzq.sufxvd.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://onp.yonumen.top

[S55] C++：结构化绑定
来源：http://pri.fzhhl.top

auto [a, b] = std::make_pair(1, 2);
来源：http://gjx.ppjwa.cn

[S56] C++：optional
来源：http://afh.zhongyouzk.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bwk.wangdashe.top

[S57] C++：编译期常量
来源：http://hxs.yuxming.cn

constexpr int N = 10;
来源：http://vxx.sufxvd.cn

[S58] C++：命名空间
来源：http://car.hcnkem.com

namespace ns { int f() { return 1; } }
来源：http://xcf.zycfv.cn

[S59] C++：静态断言
来源：http://wfn.aizwys.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tze.fktsv.cn

[S60] C++：遍历并删除元素
来源：http://kpc.zhongyouzk.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oyd.xuanzx.com

================================================================================
来源：http://yzo.zhijiandao.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xko.yj20258.top

================================================================================
来源：http://wqq.guannengcc.top

[T01] Kotlin：Hello World
来源：http://qjz.bbcook.cn

println("Hello")
来源：http://utb.snrcjt.cn

[T02] Kotlin：变量
来源：http://lgh.bjfxy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://byv.hnqzz.top

[T03] Kotlin：字符串模板
来源：http://efz.316326.xyz

"值: $b"
来源：http://fdz.bjfxy.top

[T04] Kotlin：空安全
来源：http://fiq.wangdashe.top

val n: String? = null;  n?.length
来源：http://wqe.yuxming.cn

[T05] Kotlin：when 表达式
来源：http://ryt.ydjk.org.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jzz.zhengqikj.top

[T06] Kotlin：集合映射
来源：http://gfi.bbcook.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xcg.jlsjyb.cn

[T07] Kotlin：集合过滤
来源：http://puo.wangshuangyany.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xma.dashuyun.cn

[T08] Kotlin：数据类
来源：http://rjh.tarul.cn

data class User(val name: String, val age: Int)
来源：http://dvr.sjlbkw.cn

[T09] Kotlin：扩展函数
来源：http://tyj.shangyingyoupin.top

fun String.exclaim() = this + "!"
来源：http://bay.yueranfly.top

[T10] Kotlin：默认参数
来源：http://hxm.cashguo.top

fun greet(name: String = "World") = "Hi $name"
来源：http://gvz.bjfxy.top

[T11] Kotlin：协程
来源：http://ttu.haohaochexian.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://uls.aizwys.cn

[T12] Kotlin：解构声明
来源：http://apu.jinqigufen.top

val (a, b) = Pair(1, 2)
来源：http://jra.jqgufenzy.top

[T13] Kotlin：只读 Map
来源：http://nbn.yanxiufei.cn

val m = mapOf("a" to 1)
来源：http://vvs.ctjpmb.com

[T14] Kotlin：循环
来源：http://djc.zhixingplan.top

for (i in 1..10) println(i)
来源：http://bkj.zhixingplan.top

[T15] Kotlin：接口
来源：http://phv.gotoacloud.top

interface Shape { fun area(): Double }
来源：http://oyt.ivvv.top

[T16] Swift：Hello World
来源：http://ftf.cheryme.top

print("Hello")
来源：http://hpy.gogol.net.cn

[T17] Swift：变量与常量
来源：http://ttb.andypj.xyz

var a = 1;  let b = 2
来源：http://efb.gzhubu.top

[T18] Swift：字符串插值
来源：http://dis.tianlin.xyz

"值: \(b)"
来源：http://evh.nanxinkj.top

[T19] Swift：可选绑定
来源：http://cit.zhijiandao.cn

if let n = opt { print(n) }
来源：http://uiw.zhijiandao.cn

[T20] Swift：数组操作
来源：http://sor.52xcode.cn

var a = [1, 2, 3];  a.append(4)
来源：http://exj.yj20258888.top

[T21] Swift：遍历
来源：http://rey.xuetiantiany.cn

for x in a { print(x) }
来源：http://nrk.gzhubu.top

[T22] Swift：字典
来源：http://smp.jiagoushi.top

var d = ["a": 1];  d["b"] = 2
来源：http://bto.yanxiufei.cn

[T23] Swift：函数
来源：http://oyf.guowangkeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jvi.cheryme.top

[T24] Swift：闭包
来源：http://qcs.bbcook.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qql.nanxinkj.top

[T25] Swift：结构体
来源：http://prb.bjfxy.top

struct P { var x: Int }
来源：http://aez.yonumen.top

[T26] Swift：类与重写
来源：http://kpc.ydjk.org.cn

class A: Base { override func f() {} }
来源：http://bkp.zhongyouzk.top

[T27] Swift：错误处理
来源：http://aei.sweek.top

do { try f() } catch { print(error) }
来源：http://cvp.zhijiandao.cn

[T28] Swift：枚举
来源：http://nhw.0kj1m.cn

enum Color { case red, green }
来源：http://rwe.yonumen.top

[T29] Swift：guard 提前返回
来源：http://sfn.shanyushiyangkeji.top

guard let x = opt else { return }
来源：http://rgm.sysykeji.top

[T30] Swift：协议
来源：http://lud.fktsv.cn

protocol Shape { func area() -> Double }
来源：http://mhv.wangshuangyany.cn

[T31] Lua：Hello World
来源：http://cmp.hfpthk.cn

print("Hello")
来源：http://oep.ehwqpu.com

[T32] Lua：局部变量
来源：http://eie.hnqzz.top

local a = 1
来源：http://eax.fzhhl.top

[T33] Lua：表（数组）
来源：http://kjm.gaohongyu789.top

local t = {1, 2, 3};  t[4] = 4
来源：http://lzv.sjlbkw.cn

[T34] Lua：遍历表
来源：http://dmr.cheryme.top

for i, v in ipairs(t) do print(i, v) end
来源：http://voy.cheryme.top

[T35] Lua：字典表
来源：http://fzc.jqgfzy.top

local d = { a = 1 };  d.b = 2
来源：http://omj.smart0.xyz

[T36] Lua：函数
来源：http://ttu.yj20258888.top

function add(a, b) return a + b end
来源：http://ynd.quarkkingdee.top

[T37] Lua：字符串拼接
来源：http://bpw.jinqigufen.top

"a" .. "b"
来源：http://cwp.sxryk.cn

[T38] Lua：条件
来源：http://aty.hammf.cn

if x > 0 then print("正") end
来源：http://aod.quarkkingdee.top

[T39] Lua：模式匹配
来源：http://tiz.yj20258888.top

string.find(s, "%d+")
来源：http://ipq.chenzaomai.com

[T40] Lua：元表
来源：http://kfc.gogol.net.cn

setmetatable({}, { __index = base })
来源：http://pwk.pycfn.com

[T41] Perl：Hello World
来源：http://hup.yanxiufei.cn

print "Hello\n";
来源：http://mpc.nanxinkj.top

[T42] Perl：变量类型
来源：http://eeg.hnqzz.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ngp.iojbl.cn

[T43] Perl：字符串插值
来源：http://pmr.ivvv.top

"值: $a"
来源：http://raa.yuxming.cn

[T44] Perl：条件
来源：http://icd.tianlin.xyz

if ($a > 0) { print "正"; }
来源：http://hen.aibaodan.cn

[T45] Perl：数组遍历
来源：http://hdk.shuidangran.top

for my $x (@arr) { print $x; }
来源：http://lre.sweek.top

[T46] Perl：哈希操作
来源：http://ybp.gaohongyu789.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sgt.wangshuangyany.cn

[T47] Perl：正则捕获
来源：http://sbt.cheryme.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://oqt.jqgufenzy.top

[T48] Perl：正则替换
来源：http://muw.wangdashe.top

$s =~ s/old/new/g;
来源：http://xbt.gotoacloud.top

[T49] Perl：函数
来源：http://hnf.ehwqpu.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://axy.bbcook.cn

[T50] Perl：逐行读文件
来源：http://muw.shanyushiyangkeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hjl.zycfv.cn

while (my $line = <$fh>) { print $line; }
来源：http://jjl.yj202588.top

[T51] Scala：Hello World
来源：http://umg.ctjpmb.com

println("Hello")
来源：http://dvb.feifeiyinyue.top

[T52] Scala：变量
来源：http://cir.sysykeji.top

val a = 1;  var b = 2
来源：http://cbe.sjlbkw.cn

[T53] Scala：字符串插值
来源：http://ifl.yj20258.top

s"值: $b"
来源：http://ddr.zhoulong.xyz

[T54] Scala：集合映射
来源：http://xwj.vehdjk.com

List(1, 2, 3).map(_ * 2)
来源：http://tab.jqgfzy.top

[T55] Scala：集合过滤
来源：http://qya.dianchejie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ebg.sufxvd.cn

[T56] Scala：样例类
来源：http://uvk.ppjwa.cn

case class User(name: String, age: Int)
来源：http://rxr.hesvh.cn

[T57] Scala：模式匹配
来源：http://ygf.sjlbkw.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pkt.pengpengdd.cyou

[T58] Scala：函数定义
来源：http://mep.ehwqpu.com

def add(a: Int, b: Int): Int = a + b
来源：http://drv.jianghu66.top

[T59] Scala：循环
来源：http://drv.ivvv.top

for (i <- 1 to 10) println(i)
来源：http://rio.fktsv.cn

[T60] Scala：折叠
来源：http://dak.bjfxy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xht.chenlongwang.top

================================================================================
来源：http://boj.yj20258888.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://icy.chenzaomai.com

================================================================================
来源：http://xzy.andypj.xyz

[U01] Py：创建虚拟环境
来源：http://dju.nanxinkj.top

python -m venv .venv && source .venv/bin/activate
来源：http://juw.yuanzhike.top

[U02] Py：导出 / 安装依赖
来源：http://sqv.hysaishi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://apl.wangdashe.top

[U03] Py：加载 .env 配置
来源：http://bey.tian-w.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rcr.aibaodan.cn

[U04] Py：变量调试打印
来源：http://buc.jinyuanbaomall.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vcl.yj20258.top

[U05] Py：列表去重且保序
来源：http://whv.zycfv.cn

list(dict.fromkeys(arr))
来源：http://mub.xylfe.cn

[U06] Py：合并两个字典
来源：http://ehq.ctjpmb.com

{**a, **b}
来源：http://phm.bbcook.cn

[U07] Py：反转字典键值
来源：http://dob.aibaodan.cn

{v: k for k, v in d.items()}
来源：http://bzw.fktsv.cn

[U08] Py：展平二维列表
来源：http://gfr.jqgufenzy.top

[y for x in nested for y in x]
来源：http://nsy.yonumen.top

[U09] Py：字典取最大值的键
来源：http://fui.xylfe.cn

max(d, key=d.get)
来源：http://dnw.cheryme.top

[U10] Py：按值排序字典
来源：http://inn.andypj.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mdp.316326.xyz

[U11] Py：生成器表达式
来源：http://xrr.yonumen.top

(x * 2 for x in arr)
来源：http://owl.epnwcf.com

[U12] Py：取出现最多的 3 个元素
来源：http://ups.dianchejie.cn

Counter(arr).most_common(3)
来源：http://ald.tanke756.top

[U13] Py：固定长度队列
来源：http://uwv.vehdjk.com

deque(maxlen=10)
来源：http://lgw.zhoulong.xyz

[U14] Py：分组收集到列表
来源：http://aij.cucudq.cn

defaultdict(list)
来源：http://fde.jinqigufen.top

[U15] Py：高精度计时
来源：http://kjb.zhaomingkeji.xyz

t = time.perf_counter()
来源：http://ldh.chenjidiqi.icu

[U16] Py：命令行参数解析
来源：http://gou.haohaochexian.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hue.uphjek.com


<!-- 参考信息 -->