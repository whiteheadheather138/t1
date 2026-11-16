代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://ygy.c1oappe.top

[R70] 时间戳与互转
来源：http://aja.hnxiangtu.top

date +%s;  date -d @1700000000
来源：http://hrz.zdbjq.cn

[R71] 日期格式化
来源：http://vde.xinyue.icu

date +"%Y-%m-%d %H:%M:%S"
来源：http://flt.jqgufenzy.top

[R72] 等待端口就绪
来源：http://rzc.yongpay.top

until nc -z localhost 3306; do sleep 1; done
来源：http://xef.zhiwuduotai.top

[R73] 分割大日志
来源：http://koc.yuanzhike.top

split -l 1000 big.log part_
来源：http://ezp.dianchejie.cn

[R74] 批量重命名
来源：http://ega.cqqwz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://aow.nwbrower.top

[R75] 导出环境变量
来源：http://muu.0kj1m.cn

export PATH="$HOME/bin:$PATH"
来源：http://ebw.52xcode.cn

[R76] 使用临时文件
来源：http://olq.jlsjyb.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uwe.zhengqikj.top

[R77] 读取用户输入
来源：http://vfq.yj202588.top

read -rp "请输入: " ans
来源：http://knl.sufxvd.cn

[R78] 交互式菜单
来源：http://dym.yongpay.top

select opt in a b c; do echo "$opt"; break; done
来源：http://cfq.redwolf501.top

[R79] 解析命令行选项
来源：http://dai.xinyue.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ijs.tianlin.xyz

[R80] 查看脚本执行耗时
来源：http://xub.cashguo.top

time ./run.sh
来源：http://bmt.guannengcc.top

================================================================================
来源：http://bvi.yangfankeji.com

S. C / C++ 专题
来源：http://nlx.hammf.cn

================================================================================
来源：http://wbq.zdqjudy.top

[S01] C：Hello World
来源：http://oob.daria6918.cn

#include <stdio.h>
来源：http://lvu.cdnleiting.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://pdq.xingfuxueyuan.xyz

[S02] C：变量与格式化输出
来源：http://qbl.yj20258888.top

int a = 10; printf("%d\n", a);
来源：http://jrx.xuetiantiany.cn

[S03] C：读入整数
来源：http://his.jiagoushi.top

int x; scanf("%d", &x);
来源：http://zng.0kj1m.cn

[S04] C：字符串复制
来源：http://dwc.redwolf501.top

char dst[32]; strcpy(dst, "hi");
来源：http://jbd.aizwys.cn

[S05] C：字符串长度
来源：http://csz.cdnleiting.top

strlen(s)
来源：http://sdv.uphjek.com

[S06] C：字符串比较
来源：http://jeb.meibo888.top

strcmp(a, b) == 0
来源：http://hom.smart0.xyz

[S07] C：数组遍历求和
来源：http://hjd.yueranfly.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nrv.sweek.top

[S08] C：动态内存分配与释放
来源：http://kdt.shanyushiyangkeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://agr.zhengqikj.top

[S09] C：结构体定义与初始化
来源：http://axt.9152youxi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://eri.feifeiyinyue.top

[S10] C：指针与解引用
来源：http://qam.ybcxt.top

int *p = &a;  *p = 5;
来源：http://oal.aibaodan.cn

[S11] C：逐行读文件
来源：http://lwd.shanyushiyangtech.top

FILE *f = fopen("a.txt", "r");
来源：http://iyv.xylfe.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kmj.nanxinkj.top

fclose(f);
来源：http://zve.cqqwz.cn

[S12] C：写文件
来源：http://yma.smart0.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nnk.shanyushiyangkeji.top

[S13] C：宏定义
来源：http://qqn.c1oappe.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nkz.zhiwuduotai.top

[S14] C：枚举
来源：http://reu.ivvv.top

enum Color { RED, GREEN, BLUE };
来源：http://ghf.zhongyouzk.top

[S15] C：类型转换
来源：http://vky.gaohongyu789.top

(double) a / b
来源：http://pth.jinqigufen.top

[S16] C：位操作置位
来源：http://gsn.daria6918.cn

x |= (1 << 3);
来源：http://hpd.yonumen.top

[S17] C：安全拼接字符串
来源：http://wqf.yangfankeji.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ygk.sweek.top

[S18] C：命令行参数
来源：http://iul.jinqigufen.top

int main(int argc, char **argv)
来源：http://kvl.daxiang520.top

[S19] C：快速排序
来源：http://wnb.meibo888.top

qsort(a, n, sizeof(int), cmp);
来源：http://zsf.jqgfzy.top

[S20] C：二分查找
来源：http://vqi.nwbrower.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hip.hongshengwenyu.top

[S21] C：字符类别判断
来源：http://jwg.nanxinkj.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://atz.xingfuxueyuan.xyz

[S22] C：字符串转数字
来源：http://hjc.chenlongwang.top

atoi("42");  strtod("3.14", NULL);
来源：http://ezz.zhongyouzk.top

[S23] C：随机数
来源：http://yus.bjfxy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ytr.zhijiandao.cn

[S24] C：获取本地时间
来源：http://gqy.wangdashe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yqb.ehwqpu.com

[S25] C：内存拷贝
来源：http://hvk.vehdjk.com

memcpy(dst, src, n);
来源：http://jfw.zdqjudy.top

[S26] C：内存清零
来源：http://pfu.zdbjq.cn

memset(a, 0, sizeof a);
来源：http://zgn.aibaodan.cn

[S27] C：定义常量
来源：http://jrp.xuetiantiany.cn

const double PI = 3.14159;
来源：http://afp.jqgfzy.top

[S28] C：静态变量
来源：http://onq.snrcjt.cn

static int counter = 0;
来源：http://qbi.xylfe.cn

[S29] C：变参函数
来源：http://wpp.shanyushiyangkeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qun.guowangkeji.top

[S30] C：头文件保护
来源：http://ibo.daria6918.cn

#ifndef X_H
来源：http://ook.zhixingplan.top

#define X_H
来源：http://drn.ppjwa.cn

#endif
来源：http://ocj.fzhhl.top

[S31] C++：Hello World
来源：http://psa.havefunace.top

#include <iostream>
来源：http://lmm.yvedp.cn

int main() { std::cout << "Hello\n"; }
来源：http://zhk.kuanghao11.cn

[S32] C++：字符串
来源：http://jxf.gogol.net.cn

std::string s = "hi";  s += "!";
来源：http://cba.zhengqikj.top

[S33] C++：vector 增删
来源：http://vvu.gzhubu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fgm.smart0.xyz

[S34] C++：遍历 vector
来源：http://oev.zdqjudy.top

for (auto &x : v) { std::cout << x; }
来源：http://axj.xziqi.cn

[S35] C++：map
来源：http://rnd.zhiwuduotai.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://emb.dianchejie.cn

[S36] C++：unordered_map
来源：http://sdv.havefunace.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://koz.wangshuangyany.cn

[S37] C++：set
来源：http://oaf.xuanzx.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vyc.yj20258888.top

[S38] C++：排序
来源：http://fnx.guowangkeji.top

std::sort(v.begin(), v.end());
来源：http://hoc.cqqwz.cn

[S39] C++：自定义比较器排序
来源：http://mxr.jyoumei.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hzg.xuetiantiany.cn

[S40] C++：查找元素
来源：http://ijv.hnxiangtu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bfb.cashguo.top

[S41] C++：类与构造函数
来源：http://pyc.hnxiangtu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hwt.zhoulong.xyz

[S42] C++：继承与虚函数
来源：http://cbi.ywan-chungtsiang.top

class B : public Base { public: void f() override {} };
来源：http://ztk.guowangkeji.top

[S43] C++：智能指针
来源：http://cce.havefunace.top

auto p = std::make_unique<int>(5);
来源：http://cex.zdqjudy.top

[S44] C++：引用传参
来源：http://bcn.zycfv.cn

void inc(int &x) { ++x; }
来源：http://pgc.ydjk.org.cn

[S45] C++：lambda
来源：http://ntd.yj202588.top

auto add = [](int a, int b) { return a + b; };
来源：http://nxw.fzhhl.top

[S46] C++：函数模板
来源：http://tex.sxryk.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://eyx.pycfn.com

[S47] C++：结构化绑定遍历
来源：http://smp.yfazqb.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xfq.vqdsnc.cn

[S48] C++：逐行读文件
来源：http://brf.fanxiaobao.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://zxm.zhengqikj.top

while (std::getline(in, line)) { }
来源：http://evn.redwolf501.top

[S49] C++：写文件
来源：http://esa.sweek.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fca.fktsv.cn

[S50] C++：格式化数字
来源：http://doe.sweek.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lbu.zhixingplan.top

[S51] C++：显式类型转换
来源：http://iey.yuanzhike.top

static_cast<double>(a) / b
来源：http://nzx.jinqigfzy.top

[S52] C++：const 与 noexcept
来源：http://jyc.gotoacloud.top

int size() const noexcept { return n_; }
来源：http://oic.sxryk.cn

[S53] C++：移动语义
来源：http://cuk.yvedp.cn

std::vector<int> w = std::move(v);
来源：http://nhh.ydjk.org.cn

[S54] C++：异常处理
来源：http://aku.sweek.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zdy.gogol.net.cn

[S55] C++：结构化绑定
来源：http://bjp.yfazqb.com

auto [a, b] = std::make_pair(1, 2);
来源：http://ecu.pycfn.com

[S56] C++：optional
来源：http://oec.shanyushiyangtech.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xwb.pycfn.com

[S57] C++：编译期常量
来源：http://acs.andypj.xyz

constexpr int N = 10;
来源：http://tjk.zhongyouzk.top

[S58] C++：命名空间
来源：http://sqm.316326.xyz

namespace ns { int f() { return 1; } }
来源：http://jis.andypj.xyz

[S59] C++：静态断言
来源：http://uza.jqgfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xhs.dianchejie.cn

[S60] C++：遍历并删除元素
来源：http://pco.0kj1m.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ybz.fengsongda.top

================================================================================
来源：http://vqr.jianghu66.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://njh.zdqjudy.top

================================================================================
来源：http://vsc.fengsongda.top

[T01] Kotlin：Hello World
来源：http://eav.redwolf501.top

println("Hello")
来源：http://jkj.shangyingyoupin.top

[T02] Kotlin：变量
来源：http://cqm.quarkkingdee.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pqy.vehdjk.com

[T03] Kotlin：字符串模板
来源：http://fbl.0kj1m.cn

"值: $b"
来源：http://dha.aibaodan.cn

[T04] Kotlin：空安全
来源：http://kye.zdbjq.cn

val n: String? = null;  n?.length
来源：http://ssd.haohaochexian.top

[T05] Kotlin：when 表达式
来源：http://kzj.chenjidiqi.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://one.ehwqpu.com

[T06] Kotlin：集合映射
来源：http://vpf.feifeiyinyue.top

listOf(1, 2, 3).map { it * 2 }
来源：http://uxg.316326.xyz

[T07] Kotlin：集合过滤
来源：http://rvw.birdmap.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xvk.chenlongwang.top

[T08] Kotlin：数据类
来源：http://avn.cashguo.top

data class User(val name: String, val age: Int)
来源：http://kyv.yj20258.top

[T09] Kotlin：扩展函数
来源：http://qfp.fengsongda.top

fun String.exclaim() = this + "!"
来源：http://lhc.bjfxy.top

[T10] Kotlin：默认参数
来源：http://iel.gzhubu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://zlz.yvedp.cn

[T11] Kotlin：协程
来源：http://pnx.jinqigfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://sky.shangyingyoupin.top

[T12] Kotlin：解构声明
来源：http://ikt.andypj.xyz

val (a, b) = Pair(1, 2)
来源：http://xfs.hnxiangtu.top

[T13] Kotlin：只读 Map
来源：http://rmm.hysaishi.cn

val m = mapOf("a" to 1)
来源：http://uqq.zdqjudy.top

[T14] Kotlin：循环
来源：http://rxo.wangdashe.top

for (i in 1..10) println(i)
来源：http://azd.sjlbkw.cn

[T15] Kotlin：接口
来源：http://gkg.9152youxi.cn

interface Shape { fun area(): Double }
来源：http://dvm.redwolf501.top

[T16] Swift：Hello World
来源：http://vod.haohaochexian.top

print("Hello")
来源：http://icg.iojbl.cn

[T17] Swift：变量与常量
来源：http://ppg.meibo888.top

var a = 1;  let b = 2
来源：http://bvp.shangyingyoupin.top

[T18] Swift：字符串插值
来源：http://xdw.xuanzx.com

"值: \(b)"
来源：http://lzd.ydjk.org.cn

[T19] Swift：可选绑定
来源：http://ccl.yongpay.top

if let n = opt { print(n) }
来源：http://wxp.hywenlv.cn

[T20] Swift：数组操作
来源：http://iiq.nanxinkj.top

var a = [1, 2, 3];  a.append(4)
来源：http://eoh.yueranfly.top

[T21] Swift：遍历
来源：http://kbk.ivvv.top

for x in a { print(x) }
来源：http://jkh.bbcook.cn

[T22] Swift：字典
来源：http://pbz.zhengqikj.top

var d = ["a": 1];  d["b"] = 2
来源：http://ubg.yj202588.top

[T23] Swift：函数
来源：http://uql.zhongyouzk.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xse.jqgufenzy.top

[T24] Swift：闭包
来源：http://pct.jinqigfzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://zht.hnxiangtu.top

[T25] Swift：结构体
来源：http://tdh.yvedp.cn

struct P { var x: Int }
来源：http://acd.0kj1m.cn

[T26] Swift：类与重写
来源：http://jtq.bbcook.cn

class A: Base { override func f() {} }
来源：http://wgf.bjfxy.top

[T27] Swift：错误处理
来源：http://jui.cqqwz.cn

do { try f() } catch { print(error) }
来源：http://bhr.jlsjyb.cn

[T28] Swift：枚举
来源：http://pqa.bbcook.cn

enum Color { case red, green }
来源：http://wni.xingfuxueyuan.xyz

[T29] Swift：guard 提前返回
来源：http://ffr.cucudq.cn

guard let x = opt else { return }
来源：http://rkm.jianghu66.top

[T30] Swift：协议
来源：http://htm.daxiang520.top

protocol Shape { func area() -> Double }
来源：http://vac.snrcjt.cn

[T31] Lua：Hello World
来源：http://thb.dianchejie.cn

print("Hello")
来源：http://lud.ivvv.top

[T32] Lua：局部变量
来源：http://gou.pycfn.com

local a = 1
来源：http://qua.yanxiufei.cn

[T33] Lua：表（数组）
来源：http://kfr.fktsv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://raq.tianlin.xyz

[T34] Lua：遍历表
来源：http://jdm.cheryme.top

for i, v in ipairs(t) do print(i, v) end
来源：http://jae.nwbrower.top

[T35] Lua：字典表
来源：http://ghj.gaohongyu789.top

local d = { a = 1 };  d.b = 2
来源：http://lta.chenzaomai.com

[T36] Lua：函数
来源：http://jeg.jlsjyb.cn

function add(a, b) return a + b end
来源：http://vuu.xziqi.cn

[T37] Lua：字符串拼接
来源：http://qed.316326.xyz

"a" .. "b"
来源：http://kmp.zdqjudy.top

[T38] Lua：条件
来源：http://msp.hnxiangtu.top

if x > 0 then print("正") end
来源：http://ffe.epnwcf.com

[T39] Lua：模式匹配
来源：http://lrt.zycfv.cn

string.find(s, "%d+")
来源：http://hrf.yongpay.top

[T40] Lua：元表
来源：http://rbf.epnwcf.com

setmetatable({}, { __index = base })
来源：http://vxn.mhx1999.top

[T41] Perl：Hello World
来源：http://gto.pengpengdd.cyou

print "Hello\n";
来源：http://lis.fehbvm.com

[T42] Perl：变量类型
来源：http://cid.hysaishi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ihj.snrcjt.cn

[T43] Perl：字符串插值
来源：http://qpu.birdmap.top

"值: $a"
来源：http://lmd.ppjwa.cn

[T44] Perl：条件
来源：http://crv.zhiwuduotai.top

if ($a > 0) { print "正"; }
来源：http://pve.redwolf501.top

[T45] Perl：数组遍历
来源：http://coh.ehwqpu.com

for my $x (@arr) { print $x; }
来源：http://ecs.tarul.cn

[T46] Perl：哈希操作
来源：http://svv.zhiwuduotai.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://clp.iojbl.cn

[T47] Perl：正则捕获
来源：http://oxp.fzhhl.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ibe.jinghuilouyu.cn

[T48] Perl：正则替换
来源：http://wtb.nwbrower.top

$s =~ s/old/new/g;
来源：http://yyc.nwbrower.top

[T49] Perl：函数
来源：http://mtm.redwolf501.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nov.sysykeji.top

[T50] Perl：逐行读文件
来源：http://wgm.sxryk.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hwe.ywan-chungtsiang.top

while (my $line = <$fh>) { print $line; }
来源：http://aci.jinqigufen.top

[T51] Scala：Hello World
来源：http://szd.yfazqb.com

println("Hello")
来源：http://iao.ctjpmb.com

[T52] Scala：变量
来源：http://ogp.redwolf501.top

val a = 1;  var b = 2
来源：http://xms.xingfuxueyuan.xyz

[T53] Scala：字符串插值
来源：http://lqs.hcnkem.com

s"值: $b"
来源：http://nya.gotoacloud.top

[T54] Scala：集合映射
来源：http://rpi.meibo888.top

List(1, 2, 3).map(_ * 2)
来源：http://rxp.jinyuanbaomall.cn

[T55] Scala：集合过滤
来源：http://mou.hnxiangtu.top

List(1, 2, 3).filter(_ > 1)
来源：http://ypg.gogol.net.cn

[T56] Scala：样例类
来源：http://egy.gaohongyu789.top

case class User(name: String, age: Int)
来源：http://run.xuetiantiany.cn

[T57] Scala：模式匹配
来源：http://eke.sufxvd.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dql.hfpthk.cn

[T58] Scala：函数定义
来源：http://iir.gzhubu.top

def add(a: Int, b: Int): Int = a + b
来源：http://kyu.nanxinkj.top

[T59] Scala：循环
来源：http://ses.hongshengwenyu.top

for (i <- 1 to 10) println(i)
来源：http://vfy.ehwqpu.com

[T60] Scala：折叠
来源：http://xhg.guannengcc.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nsn.quarkkingdee.top

================================================================================
来源：http://ydg.quarkkingdee.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lkw.uphjek.com

================================================================================
来源：http://zah.vehdjk.com

[U01] Py：创建虚拟环境
来源：http://hmc.hesvh.cn

python -m venv .venv && source .venv/bin/activate
来源：http://aww.jqgufenzy.top

[U02] Py：导出 / 安装依赖
来源：http://mjx.gogol.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wkq.fehbvm.com

[U03] Py：加载 .env 配置
来源：http://por.jiagoushi.top

from dotenv import load_dotenv; load_dotenv()
来源：http://bkh.gaohongyu789.top

[U04] Py：变量调试打印
来源：http://dgw.meibo888.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://awe.fengsongda.top

[U05] Py：列表去重且保序
来源：http://vjm.nanxuanxn.top

list(dict.fromkeys(arr))
来源：http://cts.iojbl.cn

[U06] Py：合并两个字典
来源：http://yhe.bjfxy.top

{**a, **b}
来源：http://ram.xylfe.cn

[U07] Py：反转字典键值
来源：http://grk.zhiwuduotai.top

{v: k for k, v in d.items()}
来源：http://aih.chenlongwang.top

[U08] Py：展平二维列表
来源：http://oou.hysaishi.cn

[y for x in nested for y in x]
来源：http://esv.sysykeji.top

[U09] Py：字典取最大值的键
来源：http://hzl.cqqwz.cn

max(d, key=d.get)
来源：http://ldt.jlsjyb.cn

[U10] Py：按值排序字典
来源：http://yro.hammf.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mdr.yj20258888.top


<!-- 参考信息 -->