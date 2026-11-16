代发 wailian999

openssl rand -hex 16
来源：http://vum.gogol.net.cn

[R68] 计算文件校验值
来源：http://slg.kuanghao11.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ewi.svipenyu.cn

[R69] 生成随机密码
来源：http://lgs.xziqi.cn

head -c 16 /dev/urandom | base64
来源：http://cac.yanxiufei.cn

[R70] 时间戳与互转
来源：http://hsu.yongpay.top

date +%s;  date -d @1700000000
来源：http://blk.shanyushiyangkeji.top

[R71] 日期格式化
来源：http://vzz.daria6918.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nmp.0kj1m.cn

[R72] 等待端口就绪
来源：http://ssm.gogol.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gyc.guowangkeji.top

[R73] 分割大日志
来源：http://eqf.sysykeji.top

split -l 1000 big.log part_
来源：http://nir.gaohongyu789.top

[R74] 批量重命名
来源：http://kif.daria6918.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://azd.kuanghao11.cn

[R75] 导出环境变量
来源：http://sax.shangyingyoupin.top

export PATH="$HOME/bin:$PATH"
来源：http://oqd.dianchejie.cn

[R76] 使用临时文件
来源：http://kby.mhx1999.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qpw.wangdashe.top

[R77] 读取用户输入
来源：http://qni.fehbvm.com

read -rp "请输入: " ans
来源：http://dlp.kuanghao11.cn

[R78] 交互式菜单
来源：http://otm.zdqjudy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://zkn.tarul.cn

[R79] 解析命令行选项
来源：http://ylt.aibaodan.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bkd.jyoumei.cn

[R80] 查看脚本执行耗时
来源：http://qgy.ydjk.org.cn

time ./run.sh
来源：http://wwo.wangdashe.top

================================================================================
来源：http://ywi.jqgfzy.top

S. C / C++ 专题
来源：http://tcv.jqgfzy.top

================================================================================
来源：http://smd.quarkkingdee.top

[S01] C：Hello World
来源：http://xkb.ctjpmb.com

#include <stdio.h>
来源：http://ltf.yongpay.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://hzn.yongpay.top

[S02] C：变量与格式化输出
来源：http://nlr.nanxinkj.top

int a = 10; printf("%d\n", a);
来源：http://ofo.tian-w.cn

[S03] C：读入整数
来源：http://ujn.gotoacloud.top

int x; scanf("%d", &x);
来源：http://hli.hysaishi.cn

[S04] C：字符串复制
来源：http://uhi.yj20258888.top

char dst[32]; strcpy(dst, "hi");
来源：http://oqd.yonumen.top

[S05] C：字符串长度
来源：http://jsd.316326.xyz

strlen(s)
来源：http://xtc.yangfankeji.com

[S06] C：字符串比较
来源：http://vlk.nanxinkj.top

strcmp(a, b) == 0
来源：http://dvh.cdnleiting.top

[S07] C：数组遍历求和
来源：http://srj.tanke756.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lct.vqdsnc.cn

[S08] C：动态内存分配与释放
来源：http://xzy.gaohongyu789.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pss.jianghu66.top

[S09] C：结构体定义与初始化
来源：http://ydx.iojbl.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kyq.uphjek.com

[S10] C：指针与解引用
来源：http://ink.0kj1m.cn

int *p = &a;  *p = 5;
来源：http://yqc.yonumen.top

[S11] C：逐行读文件
来源：http://juo.gotoacloud.top

FILE *f = fopen("a.txt", "r");
来源：http://dyp.ppjwa.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wbv.tanke756.top

fclose(f);
来源：http://ups.andypj.xyz

[S12] C：写文件
来源：http://plu.9152youxi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uix.xziqi.cn

[S13] C：宏定义
来源：http://swm.zhongyouzk.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://suf.yj20258888.top

[S14] C：枚举
来源：http://pmc.yongpay.top

enum Color { RED, GREEN, BLUE };
来源：http://edn.xziqi.cn

[S15] C：类型转换
来源：http://yjd.pengpengdd.cyou

(double) a / b
来源：http://unf.fehbvm.com

[S16] C：位操作置位
来源：http://mrt.kuanghao11.cn

x |= (1 << 3);
来源：http://yjk.hesvh.cn

[S17] C：安全拼接字符串
来源：http://zmq.jianghu66.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://stm.chenzaomai.com

[S18] C：命令行参数
来源：http://ixs.sysykeji.top

int main(int argc, char **argv)
来源：http://tyb.vehdjk.com

[S19] C：快速排序
来源：http://gla.cheryme.top

qsort(a, n, sizeof(int), cmp);
来源：http://tlu.gotoacloud.top

[S20] C：二分查找
来源：http://bby.cucudq.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qai.ydjk.org.cn

[S21] C：字符类别判断
来源：http://hkr.pengpengdd.cyou

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xil.wangdashe.top

[S22] C：字符串转数字
来源：http://vdn.nanxuanxn.top

atoi("42");  strtod("3.14", NULL);
来源：http://tuo.52xcode.cn

[S23] C：随机数
来源：http://jvt.bjfxy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://iam.vehdjk.com

[S24] C：获取本地时间
来源：http://ftw.sysykeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cjt.hcnkem.com

[S25] C：内存拷贝
来源：http://odd.shanyushiyangkeji.top

memcpy(dst, src, n);
来源：http://pid.ivvv.top

[S26] C：内存清零
来源：http://hsg.yj20258888.top

memset(a, 0, sizeof a);
来源：http://qbg.aibaodan.cn

[S27] C：定义常量
来源：http://oot.ydjk.org.cn

const double PI = 3.14159;
来源：http://xji.jlsjyb.cn

[S28] C：静态变量
来源：http://nxr.zhoulong.xyz

static int counter = 0;
来源：http://fzi.cucudq.cn

[S29] C：变参函数
来源：http://vwo.zdbjq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ymq.aibaodan.cn

[S30] C：头文件保护
来源：http://zjp.iojbl.cn

#ifndef X_H
来源：http://gmb.bbcook.cn

#define X_H
来源：http://rvx.jinghuilouyu.cn

#endif
来源：http://tdy.aizwys.cn

[S31] C++：Hello World
来源：http://sil.ehwqpu.com

#include <iostream>
来源：http://hhp.iojbl.cn

int main() { std::cout << "Hello\n"; }
来源：http://kez.aibaodan.cn

[S32] C++：字符串
来源：http://bbf.chenjidiqi.icu

std::string s = "hi";  s += "!";
来源：http://guf.jiagoushi.top

[S33] C++：vector 增删
来源：http://yto.dashuyun.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kke.smart0.xyz

[S34] C++：遍历 vector
来源：http://ktk.shangyingyoupin.top

for (auto &x : v) { std::cout << x; }
来源：http://acc.ivvv.top

[S35] C++：map
来源：http://jfp.feifeiyinyue.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yvl.yonumen.top

[S36] C++：unordered_map
来源：http://dul.daria6918.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iyi.guowangkeji.top

[S37] C++：set
来源：http://bgh.cucudq.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xlx.quarkkingdee.top

[S38] C++：排序
来源：http://fpi.sufxvd.cn

std::sort(v.begin(), v.end());
来源：http://vme.ydjk.org.cn

[S39] C++：自定义比较器排序
来源：http://tcf.gotoacloud.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ytz.ppjwa.cn

[S40] C++：查找元素
来源：http://psd.sysykeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pdu.nanxuanxn.top

[S41] C++：类与构造函数
来源：http://drs.jianghu66.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://aoy.jqgufenzy.top

[S42] C++：继承与虚函数
来源：http://sbs.yfazqb.com

class B : public Base { public: void f() override {} };
来源：http://psw.zhaomingkeji.xyz

[S43] C++：智能指针
来源：http://sry.gotoacloud.top

auto p = std::make_unique<int>(5);
来源：http://fgx.jyoumei.cn

[S44] C++：引用传参
来源：http://pea.zhongyouzk.top

void inc(int &x) { ++x; }
来源：http://qvb.zycfv.cn

[S45] C++：lambda
来源：http://ayx.yfazqb.com

auto add = [](int a, int b) { return a + b; };
来源：http://min.hongshengwenyu.top

[S46] C++：函数模板
来源：http://uzl.zhongyouzk.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vqt.xingfuxueyuan.xyz

[S47] C++：结构化绑定遍历
来源：http://oqc.chenzaomai.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qbq.wangdashe.top

[S48] C++：逐行读文件
来源：http://rmu.feifeiyinyue.top

std::ifstream in("a.txt");  std::string line;
来源：http://xsk.zdqjudy.top

while (std::getline(in, line)) { }
来源：http://ihj.vehdjk.com

[S49] C++：写文件
来源：http://dhn.uphjek.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tyt.ctjpmb.com

[S50] C++：格式化数字
来源：http://bcd.vehdjk.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eed.hongshengwenyu.top

[S51] C++：显式类型转换
来源：http://chd.sxryk.cn

static_cast<double>(a) / b
来源：http://zds.jinqigfzy.top

[S52] C++：const 与 noexcept
来源：http://gcr.zhijiandao.cn

int size() const noexcept { return n_; }
来源：http://nwl.tanke756.top

[S53] C++：移动语义
来源：http://qtp.hongshengwenyu.top

std::vector<int> w = std::move(v);
来源：http://pyc.pengpengdd.cyou

[S54] C++：异常处理
来源：http://cse.bbcook.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://woc.zhoulong.xyz

[S55] C++：结构化绑定
来源：http://jgu.hywenlv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zeb.jinghuilouyu.cn

[S56] C++：optional
来源：http://knd.sufxvd.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://itt.xinyue.icu

[S57] C++：编译期常量
来源：http://the.daxiang520.top

constexpr int N = 10;
来源：http://slr.fktsv.cn

[S58] C++：命名空间
来源：http://ykz.sweek.top

namespace ns { int f() { return 1; } }
来源：http://cpr.jinghuilouyu.cn

[S59] C++：静态断言
来源：http://pzh.sysykeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tfz.zdqjudy.top

[S60] C++：遍历并删除元素
来源：http://tdk.tian-w.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nvs.shzxlz.cn

================================================================================
来源：http://fie.iojbl.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bzd.guannengcc.top

================================================================================
来源：http://ebn.dianchejie.cn

[T01] Kotlin：Hello World
来源：http://yws.xziqi.cn

println("Hello")
来源：http://lcu.zhengqikj.top

[T02] Kotlin：变量
来源：http://rxr.jqgfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xfw.snrcjt.cn

[T03] Kotlin：字符串模板
来源：http://bjz.ywan-chungtsiang.top

"值: $b"
来源：http://vkf.yonumen.top

[T04] Kotlin：空安全
来源：http://non.jinqigufen.top

val n: String? = null;  n?.length
来源：http://jnx.xuetiantiany.cn

[T05] Kotlin：when 表达式
来源：http://zev.yj20258888.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yyg.yj202588.top

[T06] Kotlin：集合映射
来源：http://khn.andypj.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://ipr.aizwys.cn

[T07] Kotlin：集合过滤
来源：http://iqw.xziqi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://crk.dianchejie.cn

[T08] Kotlin：数据类
来源：http://xyg.yuanzhike.top

data class User(val name: String, val age: Int)
来源：http://hwa.uphjek.com

[T09] Kotlin：扩展函数
来源：http://zbb.jinghuilouyu.cn

fun String.exclaim() = this + "!"
来源：http://qer.hnxiangtu.top

[T10] Kotlin：默认参数
来源：http://qmz.gogol.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zhz.yvedp.cn

[T11] Kotlin：协程
来源：http://zvp.316326.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://iii.yfazqb.com

[T12] Kotlin：解构声明
来源：http://ste.pengpengdd.cyou

val (a, b) = Pair(1, 2)
来源：http://mgm.fengsongda.top

[T13] Kotlin：只读 Map
来源：http://ymr.birdmap.top

val m = mapOf("a" to 1)
来源：http://ema.chenzaomai.com

[T14] Kotlin：循环
来源：http://ziw.smart0.xyz

for (i in 1..10) println(i)
来源：http://oxn.shuidangran.top

[T15] Kotlin：接口
来源：http://hzl.birdmap.top

interface Shape { fun area(): Double }
来源：http://lgm.birdmap.top

[T16] Swift：Hello World
来源：http://qgu.yanxiufei.cn

print("Hello")
来源：http://rxq.hywenlv.cn

[T17] Swift：变量与常量
来源：http://emq.tarul.cn

var a = 1;  let b = 2
来源：http://enc.pengpengdd.cyou

[T18] Swift：字符串插值
来源：http://izz.cdnleiting.top

"值: \(b)"
来源：http://ikp.ctjpmb.com

[T19] Swift：可选绑定
来源：http://ydu.xziqi.cn

if let n = opt { print(n) }
来源：http://epy.zdbjq.cn

[T20] Swift：数组操作
来源：http://awi.ydzc1.top

var a = [1, 2, 3];  a.append(4)
来源：http://jkl.jyoumei.cn

[T21] Swift：遍历
来源：http://irv.xingfuxueyuan.xyz

for x in a { print(x) }
来源：http://twh.yj20258888.top

[T22] Swift：字典
来源：http://tol.shanyushiyangkeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://non.guannengcc.top

[T23] Swift：函数
来源：http://rxj.jinqigfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://omi.dashuyun.cn

[T24] Swift：闭包
来源：http://nfq.sysykeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://hsb.fengsongda.top

[T25] Swift：结构体
来源：http://ygl.yonumen.top

struct P { var x: Int }
来源：http://uje.yonumen.top

[T26] Swift：类与重写
来源：http://qvj.jinqigfzy.top

class A: Base { override func f() {} }
来源：http://yxe.pycfn.com

[T27] Swift：错误处理
来源：http://dai.redwolf501.top

do { try f() } catch { print(error) }
来源：http://cmg.zdqjudy.top

[T28] Swift：枚举
来源：http://dzl.nanxinkj.top

enum Color { case red, green }
来源：http://mwk.zycfv.cn

[T29] Swift：guard 提前返回
来源：http://sob.yvedp.cn

guard let x = opt else { return }
来源：http://ukw.haohaochexian.top

[T30] Swift：协议
来源：http://mcx.iojbl.cn

protocol Shape { func area() -> Double }
来源：http://rmw.hcnkem.com

[T31] Lua：Hello World
来源：http://oot.ehwqpu.com

print("Hello")
来源：http://oxo.jinqigufen.top

[T32] Lua：局部变量
来源：http://ptq.jlsjyb.cn

local a = 1
来源：http://ffu.xinyue.icu

[T33] Lua：表（数组）
来源：http://qwi.wangshuangyany.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://apv.jqgfzy.top

[T34] Lua：遍历表
来源：http://umc.tian-w.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://utx.tanke756.top

[T35] Lua：字典表
来源：http://bnl.shanyushiyangtech.top

local d = { a = 1 };  d.b = 2
来源：http://fxt.birdmap.top

[T36] Lua：函数
来源：http://nbg.hysaishi.cn

function add(a, b) return a + b end
来源：http://iqe.yuxming.cn

[T37] Lua：字符串拼接
来源：http://ldi.hywenlv.cn

"a" .. "b"
来源：http://dbo.zycfv.cn

[T38] Lua：条件
来源：http://zvg.epnwcf.com

if x > 0 then print("正") end
来源：http://zvc.xinyue.icu

[T39] Lua：模式匹配
来源：http://wkb.ppjwa.cn

string.find(s, "%d+")
来源：http://icq.redwolf501.top

[T40] Lua：元表
来源：http://pyv.yvedp.cn

setmetatable({}, { __index = base })
来源：http://ndg.chenzaomai.com

[T41] Perl：Hello World
来源：http://lxq.redwolf501.top

print "Hello\n";
来源：http://ujx.hcnkem.com

[T42] Perl：变量类型
来源：http://hjk.shzxlz.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rwv.shzxlz.cn

[T43] Perl：字符串插值
来源：http://yls.zhongyouzk.top

"值: $a"
来源：http://gef.sufxvd.cn

[T44] Perl：条件
来源：http://sxu.hesvh.cn

if ($a > 0) { print "正"; }
来源：http://vog.xziqi.cn

[T45] Perl：数组遍历
来源：http://gex.zycfv.cn

for my $x (@arr) { print $x; }
来源：http://qgc.ywan-chungtsiang.top

[T46] Perl：哈希操作
来源：http://ipg.sysykeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://euy.gotoacloud.top

[T47] Perl：正则捕获
来源：http://bbu.ydzc1.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://mbu.andypj.xyz

[T48] Perl：正则替换
来源：http://rfu.bbcook.cn

$s =~ s/old/new/g;
来源：http://kwx.nwbrower.top

[T49] Perl：函数
来源：http://nju.dashuyun.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ulj.yonumen.top

[T50] Perl：逐行读文件
来源：http://cza.ydzc1.top

open my $fh, "<", "a.txt" or die $!;
来源：http://prh.hcnkem.com

while (my $line = <$fh>) { print $line; }
来源：http://pba.zdqjudy.top

[T51] Scala：Hello World
来源：http://ymq.xziqi.cn

println("Hello")
来源：http://cge.meibo888.top

[T52] Scala：变量
来源：http://nnf.jqgufenzy.top

val a = 1;  var b = 2
来源：http://bxy.feifeiyinyue.top

[T53] Scala：字符串插值
来源：http://eyg.ivvv.top

s"值: $b"
来源：http://vbm.mhx1999.top

[T54] Scala：集合映射
来源：http://woi.xuanzx.com

List(1, 2, 3).map(_ * 2)
来源：http://amz.jqgufenzy.top

[T55] Scala：集合过滤
来源：http://ujp.fktsv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xeb.nwbrower.top

[T56] Scala：样例类
来源：http://hpu.daria6918.cn

case class User(name: String, age: Int)
来源：http://ltl.fzhhl.top

[T57] Scala：模式匹配
来源：http://dom.zhaomingkeji.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://zjl.jianghu66.top

[T58] Scala：函数定义
来源：http://tes.gaohongyu789.top

def add(a: Int, b: Int): Int = a + b
来源：http://ruj.tianlin.xyz

[T59] Scala：循环
来源：http://lla.meibo888.top

for (i <- 1 to 10) println(i)
来源：http://fei.haohaochexian.top

[T60] Scala：折叠
来源：http://azm.yfazqb.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kel.zhengqikj.top

================================================================================
来源：http://gwy.yuxming.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yzd.quarkkingdee.top

================================================================================
来源：http://rjd.jianghu66.top

[U01] Py：创建虚拟环境
来源：http://aah.ppjwa.cn

python -m venv .venv && source .venv/bin/activate
来源：http://coo.vqdsnc.cn

[U02] Py：导出 / 安装依赖
来源：http://mtl.tian-w.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://smu.sufxvd.cn

[U03] Py：加载 .env 配置
来源：http://sjg.redwolf501.top

from dotenv import load_dotenv; load_dotenv()
来源：http://xqy.aizwys.cn

[U04] Py：变量调试打印
来源：http://dtb.cqqwz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://deu.fehbvm.com

[U05] Py：列表去重且保序
来源：http://xwx.guowangkeji.top

list(dict.fromkeys(arr))
来源：http://wxw.svipenyu.cn

[U06] Py：合并两个字典
来源：http://rdt.fktsv.cn

{**a, **b}
来源：http://ods.zdbjq.cn

[U07] Py：反转字典键值
来源：http://rwb.mhx1999.top

{v: k for k, v in d.items()}
来源：http://jvo.jinqigufen.top

[U08] Py：展平二维列表
来源：http://pea.fzhhl.top

[y for x in nested for y in x]
来源：http://nlf.dashuyun.cn


<!-- 参考信息 -->