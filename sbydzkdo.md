代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ecc.kuanghao11.cn

[R66] 定时任务
来源：http://lxw.chenjidiqi.icu

crontab -e;  crontab -l
来源：http://dgi.hfpthk.cn

[R67] 生成随机十六进制串
来源：http://hiz.yuxming.cn

openssl rand -hex 16
来源：http://irb.uphjek.com

[R68] 计算文件校验值
来源：http://iyd.bjfxy.top

sha256sum a.txt;  md5sum a.txt
来源：http://zrg.fzhhl.top

[R69] 生成随机密码
来源：http://jod.yanxiufei.cn

head -c 16 /dev/urandom | base64
来源：http://ocw.snrcjt.cn

[R70] 时间戳与互转
来源：http://csy.zhongyouzk.top

date +%s;  date -d @1700000000
来源：http://ete.ydjk.org.cn

[R71] 日期格式化
来源：http://goq.iojbl.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vxp.jlsjyb.cn

[R72] 等待端口就绪
来源：http://dbi.gogol.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://maq.pycfn.com

[R73] 分割大日志
来源：http://vcp.bjfxy.top

split -l 1000 big.log part_
来源：http://tfi.xziqi.cn

[R74] 批量重命名
来源：http://noj.hcnkem.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hcy.aibaodan.cn

[R75] 导出环境变量
来源：http://iqv.jinqigufen.top

export PATH="$HOME/bin:$PATH"
来源：http://yku.zycfv.cn

[R76] 使用临时文件
来源：http://gkr.pengpengdd.cyou

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dba.cucudq.cn

[R77] 读取用户输入
来源：http://qoj.cheryme.top

read -rp "请输入: " ans
来源：http://tse.nanxinkj.top

[R78] 交互式菜单
来源：http://lox.jlsjyb.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://isk.cashguo.top

[R79] 解析命令行选项
来源：http://ofo.fengsongda.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yka.tarul.cn

[R80] 查看脚本执行耗时
来源：http://dxt.xingfuxueyuan.xyz

time ./run.sh
来源：http://naf.fktsv.cn

================================================================================
来源：http://apo.guowangkeji.top

S. C / C++ 专题
来源：http://ljf.daria6918.cn

================================================================================
来源：http://mrm.ppjwa.cn

[S01] C：Hello World
来源：http://jia.dianchejie.cn

#include <stdio.h>
来源：http://rgs.hnqzz.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://lsc.hesvh.cn

[S02] C：变量与格式化输出
来源：http://bcs.yongpay.top

int a = 10; printf("%d\n", a);
来源：http://qou.smart0.xyz

[S03] C：读入整数
来源：http://xkm.sjlbkw.cn

int x; scanf("%d", &x);
来源：http://lhz.yanxiufei.cn

[S04] C：字符串复制
来源：http://vih.yueranfly.top

char dst[32]; strcpy(dst, "hi");
来源：http://kwo.yvedp.cn

[S05] C：字符串长度
来源：http://dst.yj20258.top

strlen(s)
来源：http://ucj.ctjpmb.com

[S06] C：字符串比较
来源：http://azp.tanke756.top

strcmp(a, b) == 0
来源：http://xbo.xylfe.cn

[S07] C：数组遍历求和
来源：http://zoh.xziqi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yoa.c1oappe.top

[S08] C：动态内存分配与释放
来源：http://jcr.shangyingyoupin.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fhg.ywan-chungtsiang.top

[S09] C：结构体定义与初始化
来源：http://yrl.hfpthk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kyp.shanyushiyangkeji.top

[S10] C：指针与解引用
来源：http://qyw.ywan-chungtsiang.top

int *p = &a;  *p = 5;
来源：http://auq.ydjk.org.cn

[S11] C：逐行读文件
来源：http://vgl.hongshengwenyu.top

FILE *f = fopen("a.txt", "r");
来源：http://xmi.bbcook.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fmz.jinyuanbaomall.cn

fclose(f);
来源：http://ywo.yanxiufei.cn

[S12] C：写文件
来源：http://cjs.bjfxy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jgv.ctjpmb.com

[S13] C：宏定义
来源：http://xqb.yueranfly.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mjc.yuanzhike.top

[S14] C：枚举
来源：http://igt.guannengcc.top

enum Color { RED, GREEN, BLUE };
来源：http://umz.epnwcf.com

[S15] C：类型转换
来源：http://qzm.mhx1999.top

(double) a / b
来源：http://sfx.fzhhl.top

[S16] C：位操作置位
来源：http://ier.hnqzz.top

x |= (1 << 3);
来源：http://nmj.zdqjudy.top

[S17] C：安全拼接字符串
来源：http://vvs.xylfe.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rnk.ydjk.org.cn

[S18] C：命令行参数
来源：http://wlh.shuidangran.top

int main(int argc, char **argv)
来源：http://tgk.shangyingyoupin.top

[S19] C：快速排序
来源：http://fdv.ydjk.org.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tle.fehbvm.com

[S20] C：二分查找
来源：http://sed.haohaochexian.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bje.jinghuilouyu.cn

[S21] C：字符类别判断
来源：http://njb.fzhhl.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yja.jianghu66.top

[S22] C：字符串转数字
来源：http://wxo.xylfe.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xve.nanxuanxn.top

[S23] C：随机数
来源：http://zgn.xingfuxueyuan.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://hyn.ehwqpu.com

[S24] C：获取本地时间
来源：http://vlk.sxryk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://irj.hcnkem.com

[S25] C：内存拷贝
来源：http://ikj.havefunace.top

memcpy(dst, src, n);
来源：http://rrm.ydjk.org.cn

[S26] C：内存清零
来源：http://amm.zhoulong.xyz

memset(a, 0, sizeof a);
来源：http://ivs.yj20258.top

[S27] C：定义常量
来源：http://lau.guowangkeji.top

const double PI = 3.14159;
来源：http://clw.ehwqpu.com

[S28] C：静态变量
来源：http://eup.fktsv.cn

static int counter = 0;
来源：http://kif.jyoumei.cn

[S29] C：变参函数
来源：http://iof.yueranfly.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://smd.0kj1m.cn

[S30] C：头文件保护
来源：http://yfq.zdbjq.cn

#ifndef X_H
来源：http://pkj.feifeiyinyue.top

#define X_H
来源：http://vts.redwolf501.top

#endif
来源：http://cdx.sxryk.cn

[S31] C++：Hello World
来源：http://zcp.hongshengwenyu.top

#include <iostream>
来源：http://agw.mhx1999.top

int main() { std::cout << "Hello\n"; }
来源：http://mjt.jinyuanbaomall.cn

[S32] C++：字符串
来源：http://oob.yonumen.top

std::string s = "hi";  s += "!";
来源：http://zgk.iojbl.cn

[S33] C++：vector 增删
来源：http://bed.bbcook.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vwb.zhaomingkeji.xyz

[S34] C++：遍历 vector
来源：http://tqh.jianghu66.top

for (auto &x : v) { std::cout << x; }
来源：http://hhs.zycfv.cn

[S35] C++：map
来源：http://xyr.snrcjt.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ngq.shangyingyoupin.top

[S36] C++：unordered_map
来源：http://fhd.xuanzx.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hgq.jlsjyb.cn

[S37] C++：set
来源：http://mhp.tianlin.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ymo.jqgufenzy.top

[S38] C++：排序
来源：http://itz.wangshuangyany.cn

std::sort(v.begin(), v.end());
来源：http://del.shanyushiyangtech.top

[S39] C++：自定义比较器排序
来源：http://ewe.xuetiantiany.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://psf.ydjk.org.cn

[S40] C++：查找元素
来源：http://cdt.pengpengdd.cyou

auto it = std::find(v.begin(), v.end(), 3);
来源：http://idg.chenlongwang.top

[S41] C++：类与构造函数
来源：http://mfm.yonumen.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hvd.uphjek.com

[S42] C++：继承与虚函数
来源：http://ndo.jinqigfzy.top

class B : public Base { public: void f() override {} };
来源：http://fwy.pengpengdd.cyou

[S43] C++：智能指针
来源：http://vbz.zhijiandao.cn

auto p = std::make_unique<int>(5);
来源：http://xou.gzhubu.top

[S44] C++：引用传参
来源：http://fkt.hcnkem.com

void inc(int &x) { ++x; }
来源：http://bxt.cqqwz.cn

[S45] C++：lambda
来源：http://ywt.vehdjk.com

auto add = [](int a, int b) { return a + b; };
来源：http://ctk.cheryme.top

[S46] C++：函数模板
来源：http://zaz.yuxming.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://npb.svipenyu.cn

[S47] C++：结构化绑定遍历
来源：http://vbx.zhiwuduotai.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dbs.jyoumei.cn

[S48] C++：逐行读文件
来源：http://ppw.zdbjq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mra.xuanzx.com

while (std::getline(in, line)) { }
来源：http://pev.jyoumei.cn

[S49] C++：写文件
来源：http://iqb.zhixingplan.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fkc.xingfuxueyuan.xyz

[S50] C++：格式化数字
来源：http://ddi.yuanzhike.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ajo.hammf.cn

[S51] C++：显式类型转换
来源：http://ssv.jinghuilouyu.cn

static_cast<double>(a) / b
来源：http://lkm.ivvv.top

[S52] C++：const 与 noexcept
来源：http://kmg.chenlongwang.top

int size() const noexcept { return n_; }
来源：http://sii.yonumen.top

[S53] C++：移动语义
来源：http://xyp.jyoumei.cn

std::vector<int> w = std::move(v);
来源：http://mut.xinyue.icu

[S54] C++：异常处理
来源：http://zgq.zhengqikj.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bjg.9152youxi.cn

[S55] C++：结构化绑定
来源：http://rar.tarul.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mqo.gotoacloud.top

[S56] C++：optional
来源：http://iic.9152youxi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ymn.gogol.net.cn

[S57] C++：编译期常量
来源：http://jra.ppjwa.cn

constexpr int N = 10;
来源：http://atc.svipenyu.cn

[S58] C++：命名空间
来源：http://puo.yj20258888.top

namespace ns { int f() { return 1; } }
来源：http://fyn.jqgufenzy.top

[S59] C++：静态断言
来源：http://kel.jqgufenzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oyp.hysaishi.cn

[S60] C++：遍历并删除元素
来源：http://tlu.aizwys.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kkm.fengsongda.top

================================================================================
来源：http://kuc.fanxiaobao.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rle.hfpthk.cn

================================================================================
来源：http://tcp.tarul.cn

[T01] Kotlin：Hello World
来源：http://jan.xuetiantiany.cn

println("Hello")
来源：http://cti.hcnkem.com

[T02] Kotlin：变量
来源：http://mvu.shanyushiyangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vbs.ctjpmb.com

[T03] Kotlin：字符串模板
来源：http://ypv.hammf.cn

"值: $b"
来源：http://ovf.andypj.xyz

[T04] Kotlin：空安全
来源：http://hei.nwbrower.top

val n: String? = null;  n?.length
来源：http://qwh.jinqigfzy.top

[T05] Kotlin：when 表达式
来源：http://mfm.sxryk.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nib.zdqjudy.top

[T06] Kotlin：集合映射
来源：http://bza.cheryme.top

listOf(1, 2, 3).map { it * 2 }
来源：http://sys.jinghuilouyu.cn

[T07] Kotlin：集合过滤
来源：http://uvk.havefunace.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://yvw.52xcode.cn

[T08] Kotlin：数据类
来源：http://tgb.hysaishi.cn

data class User(val name: String, val age: Int)
来源：http://bqm.zhiwuduotai.top

[T09] Kotlin：扩展函数
来源：http://lsj.cashguo.top

fun String.exclaim() = this + "!"
来源：http://rpa.tarul.cn

[T10] Kotlin：默认参数
来源：http://qbo.fengsongda.top

fun greet(name: String = "World") = "Hi $name"
来源：http://bel.meibo888.top

[T11] Kotlin：协程
来源：http://piz.316326.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://fpc.fanxiaobao.xyz

[T12] Kotlin：解构声明
来源：http://tnu.pengpengdd.cyou

val (a, b) = Pair(1, 2)
来源：http://jza.xylfe.cn

[T13] Kotlin：只读 Map
来源：http://qqg.shanyushiyangkeji.top

val m = mapOf("a" to 1)
来源：http://sig.mhx1999.top

[T14] Kotlin：循环
来源：http://jhy.yueranfly.top

for (i in 1..10) println(i)
来源：http://kht.zhaomingkeji.xyz

[T15] Kotlin：接口
来源：http://rta.ivvv.top

interface Shape { fun area(): Double }
来源：http://yov.tarul.cn

[T16] Swift：Hello World
来源：http://eyg.shuidangran.top

print("Hello")
来源：http://tul.jqgfzy.top

[T17] Swift：变量与常量
来源：http://hzc.hnxiangtu.top

var a = 1;  let b = 2
来源：http://rcr.gaohongyu789.top

[T18] Swift：字符串插值
来源：http://ckp.dashuyun.cn

"值: \(b)"
来源：http://tsl.zhoulong.xyz

[T19] Swift：可选绑定
来源：http://sqb.pycfn.com

if let n = opt { print(n) }
来源：http://thy.wangshuangyany.cn

[T20] Swift：数组操作
来源：http://gby.ivvv.top

var a = [1, 2, 3];  a.append(4)
来源：http://inn.jinqigfzy.top

[T21] Swift：遍历
来源：http://dpl.bjfxy.top

for x in a { print(x) }
来源：http://pfe.zhixingplan.top

[T22] Swift：字典
来源：http://pmh.tian-w.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pkb.xylfe.cn

[T23] Swift：函数
来源：http://xvl.gogol.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fas.hammf.cn

[T24] Swift：闭包
来源：http://yff.shzxlz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sgy.zycfv.cn

[T25] Swift：结构体
来源：http://grf.shangyingyoupin.top

struct P { var x: Int }
来源：http://tiw.316326.xyz

[T26] Swift：类与重写
来源：http://djl.0kj1m.cn

class A: Base { override func f() {} }
来源：http://uzz.yj20258888.top

[T27] Swift：错误处理
来源：http://rqa.316326.xyz

do { try f() } catch { print(error) }
来源：http://kfd.yangfankeji.com

[T28] Swift：枚举
来源：http://esp.smart0.xyz

enum Color { case red, green }
来源：http://jpz.fanxiaobao.xyz

[T29] Swift：guard 提前返回
来源：http://dvs.316326.xyz

guard let x = opt else { return }
来源：http://hqr.hcnkem.com

[T30] Swift：协议
来源：http://xol.zdbjq.cn

protocol Shape { func area() -> Double }
来源：http://iek.iojbl.cn

[T31] Lua：Hello World
来源：http://tym.tarul.cn

print("Hello")
来源：http://udh.guannengcc.top

[T32] Lua：局部变量
来源：http://ruo.sxryk.cn

local a = 1
来源：http://daf.quarkkingdee.top

[T33] Lua：表（数组）
来源：http://ycb.zhoulong.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://rvi.epnwcf.com

[T34] Lua：遍历表
来源：http://vfd.ybcxt.top

for i, v in ipairs(t) do print(i, v) end
来源：http://tio.svipenyu.cn

[T35] Lua：字典表
来源：http://lut.vqdsnc.cn

local d = { a = 1 };  d.b = 2
来源：http://tnd.meibo888.top

[T36] Lua：函数
来源：http://rpf.vehdjk.com

function add(a, b) return a + b end
来源：http://htf.cqqwz.cn

[T37] Lua：字符串拼接
来源：http://pyl.snrcjt.cn

"a" .. "b"
来源：http://uwe.cheryme.top

[T38] Lua：条件
来源：http://ihz.fktsv.cn

if x > 0 then print("正") end
来源：http://igo.xinyue.icu

[T39] Lua：模式匹配
来源：http://hys.kuanghao11.cn

string.find(s, "%d+")
来源：http://xxe.cucudq.cn

[T40] Lua：元表
来源：http://exb.yvedp.cn

setmetatable({}, { __index = base })
来源：http://nzt.iojbl.cn

[T41] Perl：Hello World
来源：http://yop.jinqigfzy.top

print "Hello\n";
来源：http://txc.yfazqb.com

[T42] Perl：变量类型
来源：http://ffw.nanxinkj.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kat.yj20258888.top

[T43] Perl：字符串插值
来源：http://wrs.ybcxt.top

"值: $a"
来源：http://pdr.hnqzz.top

[T44] Perl：条件
来源：http://juc.shangyingyoupin.top

if ($a > 0) { print "正"; }
来源：http://mrd.cqqwz.cn

[T45] Perl：数组遍历
来源：http://hqo.guannengcc.top

for my $x (@arr) { print $x; }
来源：http://yfe.cashguo.top

[T46] Perl：哈希操作
来源：http://wae.zdbjq.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://skq.yfazqb.com

[T47] Perl：正则捕获
来源：http://ikk.bjfxy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ikg.ehwqpu.com

[T48] Perl：正则替换
来源：http://ccn.gaohongyu789.top

$s =~ s/old/new/g;
来源：http://ung.cashguo.top

[T49] Perl：函数
来源：http://zoc.pengpengdd.cyou

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qkk.epnwcf.com

[T50] Perl：逐行读文件
来源：http://qtk.xuetiantiany.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cmf.ctjpmb.com

while (my $line = <$fh>) { print $line; }
来源：http://zyp.wangshuangyany.cn

[T51] Scala：Hello World
来源：http://fzu.cashguo.top

println("Hello")
来源：http://ywk.9152youxi.cn

[T52] Scala：变量
来源：http://ofc.fengsongda.top

val a = 1;  var b = 2
来源：http://bvx.9152youxi.cn

[T53] Scala：字符串插值
来源：http://rbz.shanyushiyangkeji.top

s"值: $b"
来源：http://dvu.jqgufenzy.top

[T54] Scala：集合映射
来源：http://tbr.hongshengwenyu.top

List(1, 2, 3).map(_ * 2)
来源：http://qdd.tianlin.xyz

[T55] Scala：集合过滤
来源：http://ofv.52xcode.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zyq.guowangkeji.top

[T56] Scala：样例类
来源：http://ccv.sufxvd.cn

case class User(name: String, age: Int)
来源：http://xwl.guannengcc.top

[T57] Scala：模式匹配
来源：http://yrd.gaohongyu789.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://hqp.chenlongwang.top

[T58] Scala：函数定义
来源：http://blm.xziqi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hnr.cdnleiting.top

[T59] Scala：循环
来源：http://itk.pycfn.com

for (i <- 1 to 10) println(i)
来源：http://ilj.zhengqikj.top

[T60] Scala：折叠
来源：http://haz.cucudq.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://chb.ctjpmb.com

================================================================================
来源：http://fwe.yj20258888.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wzs.tian-w.cn

================================================================================
来源：http://hve.hongshengwenyu.top

[U01] Py：创建虚拟环境
来源：http://nua.quarkkingdee.top

python -m venv .venv && source .venv/bin/activate
来源：http://fay.jinghuilouyu.cn

[U02] Py：导出 / 安装依赖
来源：http://qwi.jinqigfzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kza.316326.xyz

[U03] Py：加载 .env 配置
来源：http://usm.daria6918.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mjh.hfpthk.cn

[U04] Py：变量调试打印
来源：http://avn.sysykeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tbg.cdnleiting.top

[U05] Py：列表去重且保序
来源：http://iif.fehbvm.com

list(dict.fromkeys(arr))
来源：http://otn.vehdjk.com

[U06] Py：合并两个字典
来源：http://qol.yonumen.top

{**a, **b}
来源：http://ogb.jyoumei.cn


<!-- 参考信息 -->