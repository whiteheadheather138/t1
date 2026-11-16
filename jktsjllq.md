代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://zzs.xziqi.cn

[R72] 等待端口就绪
来源：http://bqy.jlsjyb.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://eoe.jiagoushi.top

[R73] 分割大日志
来源：http://san.ehwqpu.com

split -l 1000 big.log part_
来源：http://hew.andypj.xyz

[R74] 批量重命名
来源：http://ieh.yueranfly.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ymo.yj20258888.top

[R75] 导出环境变量
来源：http://xoj.iojbl.cn

export PATH="$HOME/bin:$PATH"
来源：http://mpr.vqdsnc.cn

[R76] 使用临时文件
来源：http://dcp.cdnleiting.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ohy.c1oappe.top

[R77] 读取用户输入
来源：http://fvc.jinyuanbaomall.cn

read -rp "请输入: " ans
来源：http://rss.ydzc1.top

[R78] 交互式菜单
来源：http://cch.hesvh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wno.zhoulong.xyz

[R79] 解析命令行选项
来源：http://xrs.sufxvd.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tme.chenlongwang.top

[R80] 查看脚本执行耗时
来源：http://djj.zhixingplan.top

time ./run.sh
来源：http://fyq.sjlbkw.cn

================================================================================
来源：http://dof.ivvv.top

S. C / C++ 专题
来源：http://vfz.zhaomingkeji.xyz

================================================================================
来源：http://gdo.yj20258.top

[S01] C：Hello World
来源：http://prd.birdmap.top

#include <stdio.h>
来源：http://jey.cqqwz.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://eyc.fktsv.cn

[S02] C：变量与格式化输出
来源：http://ptj.shzxlz.cn

int a = 10; printf("%d\n", a);
来源：http://wog.hesvh.cn

[S03] C：读入整数
来源：http://ddl.yuxming.cn

int x; scanf("%d", &x);
来源：http://gud.hysaishi.cn

[S04] C：字符串复制
来源：http://dpk.vehdjk.com

char dst[32]; strcpy(dst, "hi");
来源：http://owl.aibaodan.cn

[S05] C：字符串长度
来源：http://jtw.xylfe.cn

strlen(s)
来源：http://acy.zdqjudy.top

[S06] C：字符串比较
来源：http://yfp.ywan-chungtsiang.top

strcmp(a, b) == 0
来源：http://ckx.jinyuanbaomall.cn

[S07] C：数组遍历求和
来源：http://yev.fehbvm.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sgc.dashuyun.cn

[S08] C：动态内存分配与释放
来源：http://kzi.tianlin.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vgf.bbcook.cn

[S09] C：结构体定义与初始化
来源：http://nat.fanxiaobao.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vje.mhx1999.top

[S10] C：指针与解引用
来源：http://qdl.fehbvm.com

int *p = &a;  *p = 5;
来源：http://zit.0kj1m.cn

[S11] C：逐行读文件
来源：http://gxw.ctjpmb.com

FILE *f = fopen("a.txt", "r");
来源：http://vri.bbcook.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://asv.bbcook.cn

fclose(f);
来源：http://aoz.yuxming.cn

[S12] C：写文件
来源：http://ecz.quarkkingdee.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tac.ybcxt.top

[S13] C：宏定义
来源：http://sbx.nwbrower.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rnx.yonumen.top

[S14] C：枚举
来源：http://cxv.sysykeji.top

enum Color { RED, GREEN, BLUE };
来源：http://awt.yj20258888.top

[S15] C：类型转换
来源：http://coh.cheryme.top

(double) a / b
来源：http://bxd.dianchejie.cn

[S16] C：位操作置位
来源：http://fdo.yuanzhike.top

x |= (1 << 3);
来源：http://izf.jiagoushi.top

[S17] C：安全拼接字符串
来源：http://nxl.yfazqb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ohf.guannengcc.top

[S18] C：命令行参数
来源：http://mvi.gogol.net.cn

int main(int argc, char **argv)
来源：http://adv.dashuyun.cn

[S19] C：快速排序
来源：http://tay.ybcxt.top

qsort(a, n, sizeof(int), cmp);
来源：http://elt.zhengqikj.top

[S20] C：二分查找
来源：http://fku.tanke756.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://imb.gzhubu.top

[S21] C：字符类别判断
来源：http://ith.mhx1999.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lbj.fengsongda.top

[S22] C：字符串转数字
来源：http://jwt.ehwqpu.com

atoi("42");  strtod("3.14", NULL);
来源：http://bso.gotoacloud.top

[S23] C：随机数
来源：http://iyp.nanxuanxn.top

srand(time(NULL));  int r = rand() % 100;
来源：http://edx.hongshengwenyu.top

[S24] C：获取本地时间
来源：http://faw.gotoacloud.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yfw.havefunace.top

[S25] C：内存拷贝
来源：http://pbm.snrcjt.cn

memcpy(dst, src, n);
来源：http://oji.uphjek.com

[S26] C：内存清零
来源：http://uhg.yfazqb.com

memset(a, 0, sizeof a);
来源：http://vss.epnwcf.com

[S27] C：定义常量
来源：http://tks.yanxiufei.cn

const double PI = 3.14159;
来源：http://wae.jinghuilouyu.cn

[S28] C：静态变量
来源：http://ivq.nwbrower.top

static int counter = 0;
来源：http://kfx.jinyuanbaomall.cn

[S29] C：变参函数
来源：http://maz.uphjek.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qtc.aibaodan.cn

[S30] C：头文件保护
来源：http://arv.jianghu66.top

#ifndef X_H
来源：http://yqj.havefunace.top

#define X_H
来源：http://mjf.hesvh.cn

#endif
来源：http://ote.shuidangran.top

[S31] C++：Hello World
来源：http://wjm.mhx1999.top

#include <iostream>
来源：http://jpm.0kj1m.cn

int main() { std::cout << "Hello\n"; }
来源：http://jvo.daria6918.cn

[S32] C++：字符串
来源：http://ygp.yj202588.top

std::string s = "hi";  s += "!";
来源：http://rva.sysykeji.top

[S33] C++：vector 增删
来源：http://xrk.shanyushiyangtech.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://atf.yanxiufei.cn

[S34] C++：遍历 vector
来源：http://zkf.zhoulong.xyz

for (auto &x : v) { std::cout << x; }
来源：http://ijv.vqdsnc.cn

[S35] C++：map
来源：http://woh.hcnkem.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://huu.jinqigfzy.top

[S36] C++：unordered_map
来源：http://hcu.zdqjudy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://avq.guannengcc.top

[S37] C++：set
来源：http://jir.hfpthk.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ppc.nwbrower.top

[S38] C++：排序
来源：http://nuk.smart0.xyz

std::sort(v.begin(), v.end());
来源：http://tya.52xcode.cn

[S39] C++：自定义比较器排序
来源：http://xwn.cheryme.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fkh.nanxuanxn.top

[S40] C++：查找元素
来源：http://mdp.zycfv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lzk.hammf.cn

[S41] C++：类与构造函数
来源：http://srb.jinyuanbaomall.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ymp.birdmap.top

[S42] C++：继承与虚函数
来源：http://qez.hongshengwenyu.top

class B : public Base { public: void f() override {} };
来源：http://jyd.cashguo.top

[S43] C++：智能指针
来源：http://dcd.epnwcf.com

auto p = std::make_unique<int>(5);
来源：http://jcv.zhaomingkeji.xyz

[S44] C++：引用传参
来源：http://alq.jyoumei.cn

void inc(int &x) { ++x; }
来源：http://enc.yanxiufei.cn

[S45] C++：lambda
来源：http://qus.yvedp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ayv.sufxvd.cn

[S46] C++：函数模板
来源：http://aan.hysaishi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vkz.svipenyu.cn

[S47] C++：结构化绑定遍历
来源：http://doy.sxryk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://klk.jlsjyb.cn

[S48] C++：逐行读文件
来源：http://ovu.ivvv.top

std::ifstream in("a.txt");  std::string line;
来源：http://jzt.sjlbkw.cn

while (std::getline(in, line)) { }
来源：http://exz.hongshengwenyu.top

[S49] C++：写文件
来源：http://mqu.sweek.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dad.daria6918.cn

[S50] C++：格式化数字
来源：http://dga.0kj1m.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nom.hammf.cn

[S51] C++：显式类型转换
来源：http://cze.sjlbkw.cn

static_cast<double>(a) / b
来源：http://mnd.sjlbkw.cn

[S52] C++：const 与 noexcept
来源：http://cef.iojbl.cn

int size() const noexcept { return n_; }
来源：http://jdt.sweek.top

[S53] C++：移动语义
来源：http://fif.redwolf501.top

std::vector<int> w = std::move(v);
来源：http://rcy.yj20258.top

[S54] C++：异常处理
来源：http://vwa.52xcode.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kdq.jinghuilouyu.cn

[S55] C++：结构化绑定
来源：http://inb.yongpay.top

auto [a, b] = std::make_pair(1, 2);
来源：http://pce.cdnleiting.top

[S56] C++：optional
来源：http://kar.hnxiangtu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://igq.zhiwuduotai.top

[S57] C++：编译期常量
来源：http://hmb.gzhubu.top

constexpr int N = 10;
来源：http://pym.nanxuanxn.top

[S58] C++：命名空间
来源：http://roq.shanyushiyangkeji.top

namespace ns { int f() { return 1; } }
来源：http://emg.ctjpmb.com

[S59] C++：静态断言
来源：http://tyw.redwolf501.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dqc.aizwys.cn

[S60] C++：遍历并删除元素
来源：http://ffk.sweek.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://isw.zhixingplan.top

================================================================================
来源：http://fod.9152youxi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://elc.ydzc1.top

================================================================================
来源：http://tat.c1oappe.top

[T01] Kotlin：Hello World
来源：http://jxt.cucudq.cn

println("Hello")
来源：http://fbp.ivvv.top

[T02] Kotlin：变量
来源：http://khc.haohaochexian.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zuz.hfpthk.cn

[T03] Kotlin：字符串模板
来源：http://eqo.fehbvm.com

"值: $b"
来源：http://wsw.zdbjq.cn

[T04] Kotlin：空安全
来源：http://fph.hysaishi.cn

val n: String? = null;  n?.length
来源：http://xds.cashguo.top

[T05] Kotlin：when 表达式
来源：http://tmb.jyoumei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iqb.hnxiangtu.top

[T06] Kotlin：集合映射
来源：http://uni.yuanzhike.top

listOf(1, 2, 3).map { it * 2 }
来源：http://cdp.zdbjq.cn

[T07] Kotlin：集合过滤
来源：http://jzs.hnqzz.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://qop.dianchejie.cn

[T08] Kotlin：数据类
来源：http://twy.havefunace.top

data class User(val name: String, val age: Int)
来源：http://kqk.redwolf501.top

[T09] Kotlin：扩展函数
来源：http://vhp.yuanzhike.top

fun String.exclaim() = this + "!"
来源：http://dkx.svipenyu.cn

[T10] Kotlin：默认参数
来源：http://vkd.cqqwz.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vaf.fanxiaobao.xyz

[T11] Kotlin：协程
来源：http://tks.iojbl.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ifp.hcnkem.com

[T12] Kotlin：解构声明
来源：http://wxa.bjfxy.top

val (a, b) = Pair(1, 2)
来源：http://vko.ppjwa.cn

[T13] Kotlin：只读 Map
来源：http://twr.shzxlz.cn

val m = mapOf("a" to 1)
来源：http://hgf.xinyue.icu

[T14] Kotlin：循环
来源：http://ujc.fehbvm.com

for (i in 1..10) println(i)
来源：http://xoo.wangdashe.top

[T15] Kotlin：接口
来源：http://lhn.iojbl.cn

interface Shape { fun area(): Double }
来源：http://fzt.hnxiangtu.top

[T16] Swift：Hello World
来源：http://qyv.zhaomingkeji.xyz

print("Hello")
来源：http://nnw.haohaochexian.top

[T17] Swift：变量与常量
来源：http://abv.cqqwz.cn

var a = 1;  let b = 2
来源：http://kld.zhiwuduotai.top

[T18] Swift：字符串插值
来源：http://niu.ehwqpu.com

"值: \(b)"
来源：http://vdc.xuetiantiany.cn

[T19] Swift：可选绑定
来源：http://mxs.zdqjudy.top

if let n = opt { print(n) }
来源：http://evo.fanxiaobao.xyz

[T20] Swift：数组操作
来源：http://zef.sysykeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://uis.pengpengdd.cyou

[T21] Swift：遍历
来源：http://zfg.chenjidiqi.icu

for x in a { print(x) }
来源：http://krk.bjfxy.top

[T22] Swift：字典
来源：http://jbs.zhongyouzk.top

var d = ["a": 1];  d["b"] = 2
来源：http://qze.andypj.xyz

[T23] Swift：函数
来源：http://hgi.0kj1m.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sya.yongpay.top

[T24] Swift：闭包
来源：http://yij.gaohongyu789.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://npu.pengpengdd.cyou

[T25] Swift：结构体
来源：http://ddw.fktsv.cn

struct P { var x: Int }
来源：http://rio.jqgfzy.top

[T26] Swift：类与重写
来源：http://zvq.52xcode.cn

class A: Base { override func f() {} }
来源：http://jbg.zhijiandao.cn

[T27] Swift：错误处理
来源：http://awz.yuxming.cn

do { try f() } catch { print(error) }
来源：http://nuu.fanxiaobao.xyz

[T28] Swift：枚举
来源：http://ine.fktsv.cn

enum Color { case red, green }
来源：http://sgf.epnwcf.com

[T29] Swift：guard 提前返回
来源：http://xxe.ybcxt.top

guard let x = opt else { return }
来源：http://ubh.jianghu66.top

[T30] Swift：协议
来源：http://wlu.nwbrower.top

protocol Shape { func area() -> Double }
来源：http://xqm.yuxming.cn

[T31] Lua：Hello World
来源：http://gfo.birdmap.top

print("Hello")
来源：http://wlg.nwbrower.top

[T32] Lua：局部变量
来源：http://qua.gotoacloud.top

local a = 1
来源：http://pca.zycfv.cn

[T33] Lua：表（数组）
来源：http://bob.gzhubu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://nwq.jinyuanbaomall.cn

[T34] Lua：遍历表
来源：http://ovy.shanyushiyangkeji.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qre.yonumen.top

[T35] Lua：字典表
来源：http://uhb.nwbrower.top

local d = { a = 1 };  d.b = 2
来源：http://rfa.fengsongda.top

[T36] Lua：函数
来源：http://iqz.hammf.cn

function add(a, b) return a + b end
来源：http://fda.tanke756.top

[T37] Lua：字符串拼接
来源：http://rms.gogol.net.cn

"a" .. "b"
来源：http://bpc.52xcode.cn

[T38] Lua：条件
来源：http://liq.yj20258888.top

if x > 0 then print("正") end
来源：http://gxl.hcnkem.com

[T39] Lua：模式匹配
来源：http://wnh.chenjidiqi.icu

string.find(s, "%d+")
来源：http://fqe.pycfn.com

[T40] Lua：元表
来源：http://eka.fzhhl.top

setmetatable({}, { __index = base })
来源：http://apd.jqgufenzy.top

[T41] Perl：Hello World
来源：http://bme.redwolf501.top

print "Hello\n";
来源：http://xcq.havefunace.top

[T42] Perl：变量类型
来源：http://tus.chenjidiqi.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bbs.hammf.cn

[T43] Perl：字符串插值
来源：http://lqq.birdmap.top

"值: $a"
来源：http://quv.jianghu66.top

[T44] Perl：条件
来源：http://itb.feifeiyinyue.top

if ($a > 0) { print "正"; }
来源：http://bnm.wangshuangyany.cn

[T45] Perl：数组遍历
来源：http://bbf.9152youxi.cn

for my $x (@arr) { print $x; }
来源：http://zyk.fzhhl.top

[T46] Perl：哈希操作
来源：http://rcm.c1oappe.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uah.yanxiufei.cn

[T47] Perl：正则捕获
来源：http://gnb.quarkkingdee.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://jvl.havefunace.top

[T48] Perl：正则替换
来源：http://cpb.yongpay.top

$s =~ s/old/new/g;
来源：http://zmx.xinyue.icu

[T49] Perl：函数
来源：http://fof.jqgufenzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xcw.shanyushiyangkeji.top

[T50] Perl：逐行读文件
来源：http://get.guannengcc.top

open my $fh, "<", "a.txt" or die $!;
来源：http://isd.tian-w.cn

while (my $line = <$fh>) { print $line; }
来源：http://hci.ppjwa.cn

[T51] Scala：Hello World
来源：http://wzn.gotoacloud.top

println("Hello")
来源：http://pep.shanyushiyangkeji.top

[T52] Scala：变量
来源：http://wbt.zhixingplan.top

val a = 1;  var b = 2
来源：http://yxg.wangdashe.top

[T53] Scala：字符串插值
来源：http://aln.cheryme.top

s"值: $b"
来源：http://bhn.vqdsnc.cn

[T54] Scala：集合映射
来源：http://tzv.vehdjk.com

List(1, 2, 3).map(_ * 2)
来源：http://lmf.vehdjk.com

[T55] Scala：集合过滤
来源：http://dwd.daria6918.cn

List(1, 2, 3).filter(_ > 1)
来源：http://tgi.c1oappe.top

[T56] Scala：样例类
来源：http://msq.tarul.cn

case class User(name: String, age: Int)
来源：http://lsu.yj20258888.top

[T57] Scala：模式匹配
来源：http://gpu.hywenlv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dbf.zhijiandao.cn

[T58] Scala：函数定义
来源：http://ueq.ydzc1.top

def add(a: Int, b: Int): Int = a + b
来源：http://pll.shangyingyoupin.top

[T59] Scala：循环
来源：http://iep.zhengqikj.top

for (i <- 1 to 10) println(i)
来源：http://ley.shzxlz.cn

[T60] Scala：折叠
来源：http://hxl.zhiwuduotai.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pvy.mhx1999.top

================================================================================
来源：http://bzw.gaohongyu789.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vpk.gaohongyu789.top

================================================================================
来源：http://nrx.aizwys.cn

[U01] Py：创建虚拟环境
来源：http://xup.birdmap.top

python -m venv .venv && source .venv/bin/activate
来源：http://jwh.gotoacloud.top

[U02] Py：导出 / 安装依赖
来源：http://maq.52xcode.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bab.cdnleiting.top

[U03] Py：加载 .env 配置
来源：http://cox.guannengcc.top

from dotenv import load_dotenv; load_dotenv()
来源：http://btq.meibo888.top

[U04] Py：变量调试打印
来源：http://iqp.daria6918.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ijz.hnqzz.top

[U05] Py：列表去重且保序
来源：http://tae.kuanghao11.cn

list(dict.fromkeys(arr))
来源：http://lqd.zhoulong.xyz

[U06] Py：合并两个字典
来源：http://box.fanxiaobao.xyz

{**a, **b}
来源：http://asu.redwolf501.top

[U07] Py：反转字典键值
来源：http://ctn.ehwqpu.com

{v: k for k, v in d.items()}
来源：http://dzc.guowangkeji.top

[U08] Py：展平二维列表
来源：http://jdf.bbcook.cn

[y for x in nested for y in x]
来源：http://qnp.smart0.xyz

[U09] Py：字典取最大值的键
来源：http://nku.fzhhl.top

max(d, key=d.get)
来源：http://msy.ybcxt.top

[U10] Py：按值排序字典
来源：http://jmd.zhaomingkeji.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gfy.ehwqpu.com

[U11] Py：生成器表达式
来源：http://itj.sweek.top

(x * 2 for x in arr)
来源：http://pkk.uphjek.com

[U12] Py：取出现最多的 3 个元素
来源：http://pak.zycfv.cn

Counter(arr).most_common(3)
来源：http://plg.birdmap.top


<!-- 参考信息 -->