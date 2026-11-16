代发 wailian999

openssl rand -hex 16
来源：http://kyy.iojbl.cn

[R68] 计算文件校验值
来源：http://lja.jinqigufen.top

sha256sum a.txt;  md5sum a.txt
来源：http://vxn.fanxiaobao.xyz

[R69] 生成随机密码
来源：http://wpo.svipenyu.cn

head -c 16 /dev/urandom | base64
来源：http://bof.dashuyun.cn

[R70] 时间戳与互转
来源：http://fxf.chenlongwang.top

date +%s;  date -d @1700000000
来源：http://zig.hfpthk.cn

[R71] 日期格式化
来源：http://fvi.ctjpmb.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://wdv.yongpay.top

[R72] 等待端口就绪
来源：http://yqm.zhaomingkeji.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://huo.hysaishi.cn

[R73] 分割大日志
来源：http://mqp.bjfxy.top

split -l 1000 big.log part_
来源：http://snb.yanxiufei.cn

[R74] 批量重命名
来源：http://waa.hfpthk.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ank.hfpthk.cn

[R75] 导出环境变量
来源：http://rbm.daria6918.cn

export PATH="$HOME/bin:$PATH"
来源：http://ywx.wangshuangyany.cn

[R76] 使用临时文件
来源：http://lbs.yj20258888.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lad.ppjwa.cn

[R77] 读取用户输入
来源：http://zbo.sxryk.cn

read -rp "请输入: " ans
来源：http://xkm.xuanzx.com

[R78] 交互式菜单
来源：http://kyu.shuidangran.top

select opt in a b c; do echo "$opt"; break; done
来源：http://sva.redwolf501.top

[R79] 解析命令行选项
来源：http://uyn.cheryme.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dcf.pengpengdd.cyou

[R80] 查看脚本执行耗时
来源：http://fxb.mhx1999.top

time ./run.sh
来源：http://gmr.kuanghao11.cn

================================================================================
来源：http://noj.jinqigfzy.top

S. C / C++ 专题
来源：http://zps.bjfxy.top

================================================================================
来源：http://mwg.xingfuxueyuan.xyz

[S01] C：Hello World
来源：http://swt.xuetiantiany.cn

#include <stdio.h>
来源：http://pwj.yonumen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://did.zhijiandao.cn

[S02] C：变量与格式化输出
来源：http://tfd.jinyuanbaomall.cn

int a = 10; printf("%d\n", a);
来源：http://uvk.cdnleiting.top

[S03] C：读入整数
来源：http://wyj.chenlongwang.top

int x; scanf("%d", &x);
来源：http://nfi.hammf.cn

[S04] C：字符串复制
来源：http://pwv.yuanzhike.top

char dst[32]; strcpy(dst, "hi");
来源：http://xif.hesvh.cn

[S05] C：字符串长度
来源：http://loj.ivvv.top

strlen(s)
来源：http://dbr.xziqi.cn

[S06] C：字符串比较
来源：http://moz.xziqi.cn

strcmp(a, b) == 0
来源：http://ihw.zhaomingkeji.xyz

[S07] C：数组遍历求和
来源：http://okd.bbcook.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jwn.dashuyun.cn

[S08] C：动态内存分配与释放
来源：http://lmx.sjlbkw.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tov.zhoulong.xyz

[S09] C：结构体定义与初始化
来源：http://pwz.fzhhl.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ahu.daria6918.cn

[S10] C：指针与解引用
来源：http://rtf.yj202588.top

int *p = &a;  *p = 5;
来源：http://uju.dashuyun.cn

[S11] C：逐行读文件
来源：http://mgj.dianchejie.cn

FILE *f = fopen("a.txt", "r");
来源：http://fmd.sysykeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://nmj.0kj1m.cn

fclose(f);
来源：http://vwv.cdnleiting.top

[S12] C：写文件
来源：http://ifq.fehbvm.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fbq.yanxiufei.cn

[S13] C：宏定义
来源：http://klv.tarul.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rrh.jqgfzy.top

[S14] C：枚举
来源：http://ots.shzxlz.cn

enum Color { RED, GREEN, BLUE };
来源：http://wcc.xinyue.icu

[S15] C：类型转换
来源：http://mvs.havefunace.top

(double) a / b
来源：http://rbs.ppjwa.cn

[S16] C：位操作置位
来源：http://gai.pengpengdd.cyou

x |= (1 << 3);
来源：http://nwu.zhijiandao.cn

[S17] C：安全拼接字符串
来源：http://cuz.pycfn.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tmt.cheryme.top

[S18] C：命令行参数
来源：http://mfh.smart0.xyz

int main(int argc, char **argv)
来源：http://ihy.ywan-chungtsiang.top

[S19] C：快速排序
来源：http://lgv.cdnleiting.top

qsort(a, n, sizeof(int), cmp);
来源：http://ncd.zhoulong.xyz

[S20] C：二分查找
来源：http://bhj.yuxming.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://phs.ehwqpu.com

[S21] C：字符类别判断
来源：http://pcp.ctjpmb.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wsw.wangdashe.top

[S22] C：字符串转数字
来源：http://ctv.yj20258.top

atoi("42");  strtod("3.14", NULL);
来源：http://cic.ivvv.top

[S23] C：随机数
来源：http://zrw.zhiwuduotai.top

srand(time(NULL));  int r = rand() % 100;
来源：http://lyq.ydjk.org.cn

[S24] C：获取本地时间
来源：http://ofm.zhixingplan.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rgb.zdbjq.cn

[S25] C：内存拷贝
来源：http://edt.bbcook.cn

memcpy(dst, src, n);
来源：http://ndh.jinqigufen.top

[S26] C：内存清零
来源：http://ucd.shanyushiyangtech.top

memset(a, 0, sizeof a);
来源：http://xrh.meibo888.top

[S27] C：定义常量
来源：http://rqk.yj202588.top

const double PI = 3.14159;
来源：http://ley.jqgufenzy.top

[S28] C：静态变量
来源：http://aqi.yj20258.top

static int counter = 0;
来源：http://epb.xuetiantiany.cn

[S29] C：变参函数
来源：http://hth.kuanghao11.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zpb.zhijiandao.cn

[S30] C：头文件保护
来源：http://tin.zycfv.cn

#ifndef X_H
来源：http://cyu.havefunace.top

#define X_H
来源：http://wyl.xinyue.icu

#endif
来源：http://qfi.cqqwz.cn

[S31] C++：Hello World
来源：http://egv.yj20258888.top

#include <iostream>
来源：http://loe.shzxlz.cn

int main() { std::cout << "Hello\n"; }
来源：http://dxc.ydjk.org.cn

[S32] C++：字符串
来源：http://byz.cqqwz.cn

std::string s = "hi";  s += "!";
来源：http://azi.shanyushiyangtech.top

[S33] C++：vector 增删
来源：http://gha.kuanghao11.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kur.haohaochexian.top

[S34] C++：遍历 vector
来源：http://mpz.zhongyouzk.top

for (auto &x : v) { std::cout << x; }
来源：http://qgi.iojbl.cn

[S35] C++：map
来源：http://hep.pycfn.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ate.wangshuangyany.cn

[S36] C++：unordered_map
来源：http://vex.tarul.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vak.vqdsnc.cn

[S37] C++：set
来源：http://new.daria6918.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sll.ybcxt.top

[S38] C++：排序
来源：http://iwt.cashguo.top

std::sort(v.begin(), v.end());
来源：http://dof.jqgfzy.top

[S39] C++：自定义比较器排序
来源：http://bir.andypj.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qyd.shangyingyoupin.top

[S40] C++：查找元素
来源：http://rxt.xziqi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mwx.yuanzhike.top

[S41] C++：类与构造函数
来源：http://svm.wangshuangyany.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ngb.tanke756.top

[S42] C++：继承与虚函数
来源：http://itw.shzxlz.cn

class B : public Base { public: void f() override {} };
来源：http://typ.vehdjk.com

[S43] C++：智能指针
来源：http://bud.kuanghao11.cn

auto p = std::make_unique<int>(5);
来源：http://qdp.havefunace.top

[S44] C++：引用传参
来源：http://kmb.hnqzz.top

void inc(int &x) { ++x; }
来源：http://rhx.gaohongyu789.top

[S45] C++：lambda
来源：http://lyo.kuanghao11.cn

auto add = [](int a, int b) { return a + b; };
来源：http://luo.yongpay.top

[S46] C++：函数模板
来源：http://cmz.iojbl.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oxj.cdnleiting.top

[S47] C++：结构化绑定遍历
来源：http://rws.yfazqb.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://igm.jqgfzy.top

[S48] C++：逐行读文件
来源：http://xgp.dashuyun.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ovs.gzhubu.top

while (std::getline(in, line)) { }
来源：http://deo.tian-w.cn

[S49] C++：写文件
来源：http://dsk.yueranfly.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xlz.gzhubu.top

[S50] C++：格式化数字
来源：http://aai.yangfankeji.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mew.haohaochexian.top

[S51] C++：显式类型转换
来源：http://vtw.pycfn.com

static_cast<double>(a) / b
来源：http://utz.jyoumei.cn

[S52] C++：const 与 noexcept
来源：http://pxw.xinyue.icu

int size() const noexcept { return n_; }
来源：http://zrf.dashuyun.cn

[S53] C++：移动语义
来源：http://gyv.iojbl.cn

std::vector<int> w = std::move(v);
来源：http://lhs.smart0.xyz

[S54] C++：异常处理
来源：http://ngs.vqdsnc.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fkq.feifeiyinyue.top

[S55] C++：结构化绑定
来源：http://otw.hywenlv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ake.guannengcc.top

[S56] C++：optional
来源：http://duk.yj202588.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hki.nanxinkj.top

[S57] C++：编译期常量
来源：http://rwq.tanke756.top

constexpr int N = 10;
来源：http://gaf.cqqwz.cn

[S58] C++：命名空间
来源：http://qaj.shanyushiyangtech.top

namespace ns { int f() { return 1; } }
来源：http://iva.gogol.net.cn

[S59] C++：静态断言
来源：http://bww.jianghu66.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ksl.fanxiaobao.xyz

[S60] C++：遍历并删除元素
来源：http://jmw.nanxuanxn.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://iay.dashuyun.cn

================================================================================
来源：http://poj.jianghu66.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vpi.guowangkeji.top

================================================================================
来源：http://emm.wangshuangyany.cn

[T01] Kotlin：Hello World
来源：http://eiv.9152youxi.cn

println("Hello")
来源：http://wzq.ydjk.org.cn

[T02] Kotlin：变量
来源：http://nyi.xuetiantiany.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://weh.jiagoushi.top

[T03] Kotlin：字符串模板
来源：http://eyg.jqgfzy.top

"值: $b"
来源：http://gmg.yj202588.top

[T04] Kotlin：空安全
来源：http://nwu.jinqigfzy.top

val n: String? = null;  n?.length
来源：http://cap.shanyushiyangkeji.top

[T05] Kotlin：when 表达式
来源：http://hpu.mhx1999.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mvn.hcnkem.com

[T06] Kotlin：集合映射
来源：http://vcy.tarul.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kaz.shanyushiyangkeji.top

[T07] Kotlin：集合过滤
来源：http://tsa.jianghu66.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://lan.jlsjyb.cn

[T08] Kotlin：数据类
来源：http://dxc.guannengcc.top

data class User(val name: String, val age: Int)
来源：http://nti.xingfuxueyuan.xyz

[T09] Kotlin：扩展函数
来源：http://kfb.smart0.xyz

fun String.exclaim() = this + "!"
来源：http://mgz.jyoumei.cn

[T10] Kotlin：默认参数
来源：http://jro.birdmap.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ong.hongshengwenyu.top

[T11] Kotlin：协程
来源：http://nmr.yueranfly.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://yav.ehwqpu.com

[T12] Kotlin：解构声明
来源：http://ewu.fzhhl.top

val (a, b) = Pair(1, 2)
来源：http://zun.hnqzz.top

[T13] Kotlin：只读 Map
来源：http://yzb.ctjpmb.com

val m = mapOf("a" to 1)
来源：http://jcf.guowangkeji.top

[T14] Kotlin：循环
来源：http://zdd.zhongyouzk.top

for (i in 1..10) println(i)
来源：http://fzp.hongshengwenyu.top

[T15] Kotlin：接口
来源：http://zfl.sjlbkw.cn

interface Shape { fun area(): Double }
来源：http://ofe.aizwys.cn

[T16] Swift：Hello World
来源：http://fps.jinyuanbaomall.cn

print("Hello")
来源：http://lwx.hnqzz.top

[T17] Swift：变量与常量
来源：http://cgm.fengsongda.top

var a = 1;  let b = 2
来源：http://hnw.nwbrower.top

[T18] Swift：字符串插值
来源：http://rmw.wangdashe.top

"值: \(b)"
来源：http://acf.birdmap.top

[T19] Swift：可选绑定
来源：http://ymx.yongpay.top

if let n = opt { print(n) }
来源：http://whs.sysykeji.top

[T20] Swift：数组操作
来源：http://rio.tianlin.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://isu.yj202588.top

[T21] Swift：遍历
来源：http://lvh.haohaochexian.top

for x in a { print(x) }
来源：http://gvp.sufxvd.cn

[T22] Swift：字典
来源：http://bmv.shangyingyoupin.top

var d = ["a": 1];  d["b"] = 2
来源：http://vqy.meibo888.top

[T23] Swift：函数
来源：http://wes.ydzc1.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://soc.epnwcf.com

[T24] Swift：闭包
来源：http://kyq.cqqwz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mdp.ybcxt.top

[T25] Swift：结构体
来源：http://sxn.tianlin.xyz

struct P { var x: Int }
来源：http://pqx.sxryk.cn

[T26] Swift：类与重写
来源：http://krc.bbcook.cn

class A: Base { override func f() {} }
来源：http://ouq.zdbjq.cn

[T27] Swift：错误处理
来源：http://ife.haohaochexian.top

do { try f() } catch { print(error) }
来源：http://nne.chenzaomai.com

[T28] Swift：枚举
来源：http://nwt.yueranfly.top

enum Color { case red, green }
来源：http://gqe.chenzaomai.com

[T29] Swift：guard 提前返回
来源：http://yyu.guannengcc.top

guard let x = opt else { return }
来源：http://xzu.mhx1999.top

[T30] Swift：协议
来源：http://bxh.xuanzx.com

protocol Shape { func area() -> Double }
来源：http://qmx.c1oappe.top

[T31] Lua：Hello World
来源：http://bru.gogol.net.cn

print("Hello")
来源：http://lab.jiagoushi.top

[T32] Lua：局部变量
来源：http://cvb.kuanghao11.cn

local a = 1
来源：http://kpn.fengsongda.top

[T33] Lua：表（数组）
来源：http://mga.yuxming.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xli.yvedp.cn

[T34] Lua：遍历表
来源：http://wru.ydjk.org.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ahk.jiagoushi.top

[T35] Lua：字典表
来源：http://ewz.fzhhl.top

local d = { a = 1 };  d.b = 2
来源：http://esg.yj20258888.top

[T36] Lua：函数
来源：http://pkb.zhijiandao.cn

function add(a, b) return a + b end
来源：http://lha.redwolf501.top

[T37] Lua：字符串拼接
来源：http://vin.jiagoushi.top

"a" .. "b"
来源：http://jbw.316326.xyz

[T38] Lua：条件
来源：http://gvo.epnwcf.com

if x > 0 then print("正") end
来源：http://rap.cqqwz.cn

[T39] Lua：模式匹配
来源：http://ybi.uphjek.com

string.find(s, "%d+")
来源：http://ubn.gotoacloud.top

[T40] Lua：元表
来源：http://oty.zdbjq.cn

setmetatable({}, { __index = base })
来源：http://dbj.xuanzx.com

[T41] Perl：Hello World
来源：http://hrd.yanxiufei.cn

print "Hello\n";
来源：http://auq.xingfuxueyuan.xyz

[T42] Perl：变量类型
来源：http://bkv.havefunace.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hdl.cdnleiting.top

[T43] Perl：字符串插值
来源：http://uco.xinyue.icu

"值: $a"
来源：http://gos.gotoacloud.top

[T44] Perl：条件
来源：http://kmp.daxiang520.top

if ($a > 0) { print "正"; }
来源：http://kma.ybcxt.top

[T45] Perl：数组遍历
来源：http://ztz.fktsv.cn

for my $x (@arr) { print $x; }
来源：http://lnu.jinyuanbaomall.cn

[T46] Perl：哈希操作
来源：http://hxb.zdqjudy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ano.daxiang520.top

[T47] Perl：正则捕获
来源：http://ihj.xinyue.icu

if ($s =~ /(\d+)/) { print $1; }
来源：http://fny.sufxvd.cn

[T48] Perl：正则替换
来源：http://pge.quarkkingdee.top

$s =~ s/old/new/g;
来源：http://vpb.jinqigfzy.top

[T49] Perl：函数
来源：http://puk.sufxvd.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nuc.jyoumei.cn

[T50] Perl：逐行读文件
来源：http://zju.vqdsnc.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zyp.xingfuxueyuan.xyz

while (my $line = <$fh>) { print $line; }
来源：http://btk.ehwqpu.com

[T51] Scala：Hello World
来源：http://yha.gzhubu.top

println("Hello")
来源：http://uvg.sjlbkw.cn

[T52] Scala：变量
来源：http://nwc.zdbjq.cn

val a = 1;  var b = 2
来源：http://ucy.nanxuanxn.top

[T53] Scala：字符串插值
来源：http://jrs.xinyue.icu

s"值: $b"
来源：http://sip.yj20258888.top

[T54] Scala：集合映射
来源：http://try.tian-w.cn

List(1, 2, 3).map(_ * 2)
来源：http://jtu.tian-w.cn

[T55] Scala：集合过滤
来源：http://epb.fehbvm.com

List(1, 2, 3).filter(_ > 1)
来源：http://zag.xylfe.cn

[T56] Scala：样例类
来源：http://vzq.sysykeji.top

case class User(name: String, age: Int)
来源：http://nck.mhx1999.top

[T57] Scala：模式匹配
来源：http://hpf.ywan-chungtsiang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://utm.sweek.top

[T58] Scala：函数定义
来源：http://sgp.gzhubu.top

def add(a: Int, b: Int): Int = a + b
来源：http://mtu.jqgfzy.top

[T59] Scala：循环
来源：http://wbx.daxiang520.top

for (i <- 1 to 10) println(i)
来源：http://pis.xingfuxueyuan.xyz

[T60] Scala：折叠
来源：http://wth.hnxiangtu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jwr.fengsongda.top

================================================================================
来源：http://cvc.ctjpmb.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pxm.yonumen.top

================================================================================
来源：http://qxy.hesvh.cn

[U01] Py：创建虚拟环境
来源：http://hjr.chenlongwang.top

python -m venv .venv && source .venv/bin/activate
来源：http://pyz.gaohongyu789.top

[U02] Py：导出 / 安装依赖
来源：http://etj.cashguo.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wqt.redwolf501.top

[U03] Py：加载 .env 配置
来源：http://nsa.fehbvm.com

from dotenv import load_dotenv; load_dotenv()
来源：http://zod.fktsv.cn

[U04] Py：变量调试打印
来源：http://csv.xinyue.icu

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gqo.yj202588.top

[U05] Py：列表去重且保序
来源：http://gmn.tianlin.xyz

list(dict.fromkeys(arr))
来源：http://ofp.jiagoushi.top

[U06] Py：合并两个字典
来源：http://uwx.zhengqikj.top

{**a, **b}
来源：http://xge.zdbjq.cn

[U07] Py：反转字典键值
来源：http://dgm.hammf.cn

{v: k for k, v in d.items()}
来源：http://pcm.sysykeji.top

[U08] Py：展平二维列表
来源：http://kug.feifeiyinyue.top

[y for x in nested for y in x]
来源：http://ltb.cheryme.top


<!-- 参考信息 -->