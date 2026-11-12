代发 wailian999

openssl rand -hex 16
来源：http://ggy.zycfv.cn

[R68] 计算文件校验值
来源：http://oae.jinqigfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://djc.shzxlz.cn

[R69] 生成随机密码
来源：http://own.sjlbkw.cn

head -c 16 /dev/urandom | base64
来源：http://ere.daria6918.cn

[R70] 时间戳与互转
来源：http://rsg.zdqjudy.top

date +%s;  date -d @1700000000
来源：http://cfn.cucudq.cn

[R71] 日期格式化
来源：http://cpw.shanyushiyangtech.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qwg.pengpengdd.cyou

[R72] 等待端口就绪
来源：http://voy.yfazqb.com

until nc -z localhost 3306; do sleep 1; done
来源：http://fnn.snrcjt.cn

[R73] 分割大日志
来源：http://uew.cheryme.top

split -l 1000 big.log part_
来源：http://gdu.yangfankeji.com

[R74] 批量重命名
来源：http://dwd.9152youxi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ifk.feifeiyinyue.top

[R75] 导出环境变量
来源：http://ofu.jqgufenzy.top

export PATH="$HOME/bin:$PATH"
来源：http://mfj.pengpengdd.cyou

[R76] 使用临时文件
来源：http://ujk.wangshuangyany.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ezq.jianghu66.top

[R77] 读取用户输入
来源：http://alk.gzhubu.top

read -rp "请输入: " ans
来源：http://olf.xingfuxueyuan.xyz

[R78] 交互式菜单
来源：http://ufe.iojbl.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fso.fzhhl.top

[R79] 解析命令行选项
来源：http://ngn.snrcjt.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://asb.shangyingyoupin.top

[R80] 查看脚本执行耗时
来源：http://wlh.cashguo.top

time ./run.sh
来源：http://yej.sjlbkw.cn

================================================================================
来源：http://usv.hnqzz.top

S. C / C++ 专题
来源：http://cic.shangyingyoupin.top

================================================================================
来源：http://pqe.shangyingyoupin.top

[S01] C：Hello World
来源：http://qkj.xziqi.cn

#include <stdio.h>
来源：http://sny.sweek.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rpf.hesvh.cn

[S02] C：变量与格式化输出
来源：http://rup.jinqigufen.top

int a = 10; printf("%d\n", a);
来源：http://edj.smart0.xyz

[S03] C：读入整数
来源：http://ymu.snrcjt.cn

int x; scanf("%d", &x);
来源：http://wqf.yvedp.cn

[S04] C：字符串复制
来源：http://rxn.dianchejie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://urp.ywan-chungtsiang.top

[S05] C：字符串长度
来源：http://qqh.ywan-chungtsiang.top

strlen(s)
来源：http://jqq.hongshengwenyu.top

[S06] C：字符串比较
来源：http://vhw.cqqwz.cn

strcmp(a, b) == 0
来源：http://add.zdbjq.cn

[S07] C：数组遍历求和
来源：http://wsc.yvedp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ghu.sxryk.cn

[S08] C：动态内存分配与释放
来源：http://fnn.vehdjk.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nwf.0kj1m.cn

[S09] C：结构体定义与初始化
来源：http://bag.sxryk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ctc.hfpthk.cn

[S10] C：指针与解引用
来源：http://fcs.smart0.xyz

int *p = &a;  *p = 5;
来源：http://fov.feifeiyinyue.top

[S11] C：逐行读文件
来源：http://qzy.gzhubu.top

FILE *f = fopen("a.txt", "r");
来源：http://jjb.gogol.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ozu.yj202588.top

fclose(f);
来源：http://cab.chenlongwang.top

[S12] C：写文件
来源：http://tgu.chenlongwang.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://btv.xinyue.icu

[S13] C：宏定义
来源：http://biu.daxiang520.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eyt.sufxvd.cn

[S14] C：枚举
来源：http://wtz.haohaochexian.top

enum Color { RED, GREEN, BLUE };
来源：http://nyw.0kj1m.cn

[S15] C：类型转换
来源：http://vcb.shanyushiyangtech.top

(double) a / b
来源：http://nek.chenlongwang.top

[S16] C：位操作置位
来源：http://gdv.meibo888.top

x |= (1 << 3);
来源：http://jak.cdnleiting.top

[S17] C：安全拼接字符串
来源：http://elk.cqqwz.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jhu.havefunace.top

[S18] C：命令行参数
来源：http://jah.cucudq.cn

int main(int argc, char **argv)
来源：http://tjy.hysaishi.cn

[S19] C：快速排序
来源：http://ubw.zhengqikj.top

qsort(a, n, sizeof(int), cmp);
来源：http://uqu.chenzaomai.com

[S20] C：二分查找
来源：http://pge.xylfe.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nbt.xinyue.icu

[S21] C：字符类别判断
来源：http://wnl.yongpay.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tws.tian-w.cn

[S22] C：字符串转数字
来源：http://bgd.cheryme.top

atoi("42");  strtod("3.14", NULL);
来源：http://ozq.wangdashe.top

[S23] C：随机数
来源：http://njo.uphjek.com

srand(time(NULL));  int r = rand() % 100;
来源：http://ypo.ppjwa.cn

[S24] C：获取本地时间
来源：http://jds.fehbvm.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ufz.hammf.cn

[S25] C：内存拷贝
来源：http://lis.0kj1m.cn

memcpy(dst, src, n);
来源：http://gpu.zycfv.cn

[S26] C：内存清零
来源：http://sak.havefunace.top

memset(a, 0, sizeof a);
来源：http://iwh.snrcjt.cn

[S27] C：定义常量
来源：http://aml.feifeiyinyue.top

const double PI = 3.14159;
来源：http://vfp.hnqzz.top

[S28] C：静态变量
来源：http://wmv.iojbl.cn

static int counter = 0;
来源：http://svc.sxryk.cn

[S29] C：变参函数
来源：http://bam.xingfuxueyuan.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://req.daxiang520.top

[S30] C：头文件保护
来源：http://ahf.9152youxi.cn

#ifndef X_H
来源：http://zcw.yj20258888.top

#define X_H
来源：http://kmh.yj20258.top

#endif
来源：http://eaa.epnwcf.com

[S31] C++：Hello World
来源：http://ror.yanxiufei.cn

#include <iostream>
来源：http://iqz.hywenlv.cn

int main() { std::cout << "Hello\n"; }
来源：http://tje.hammf.cn

[S32] C++：字符串
来源：http://glb.zhongyouzk.top

std::string s = "hi";  s += "!";
来源：http://snv.pengpengdd.cyou

[S33] C++：vector 增删
来源：http://ptr.hnxiangtu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://drv.hfpthk.cn

[S34] C++：遍历 vector
来源：http://yik.sysykeji.top

for (auto &x : v) { std::cout << x; }
来源：http://rry.daxiang520.top

[S35] C++：map
来源：http://fyj.ivvv.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://drv.c1oappe.top

[S36] C++：unordered_map
来源：http://dzi.svipenyu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sxb.gotoacloud.top

[S37] C++：set
来源：http://zjp.c1oappe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nug.yfazqb.com

[S38] C++：排序
来源：http://duh.haohaochexian.top

std::sort(v.begin(), v.end());
来源：http://eet.quarkkingdee.top

[S39] C++：自定义比较器排序
来源：http://fjl.yj202588.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oel.zhixingplan.top

[S40] C++：查找元素
来源：http://pdi.hammf.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://efa.sysykeji.top

[S41] C++：类与构造函数
来源：http://qpt.yj20258888.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yss.nwbrower.top

[S42] C++：继承与虚函数
来源：http://qsx.mhx1999.top

class B : public Base { public: void f() override {} };
来源：http://xiv.zycfv.cn

[S43] C++：智能指针
来源：http://elu.kuanghao11.cn

auto p = std::make_unique<int>(5);
来源：http://fjr.zhengqikj.top

[S44] C++：引用传参
来源：http://tua.yfazqb.com

void inc(int &x) { ++x; }
来源：http://wdw.sxryk.cn

[S45] C++：lambda
来源：http://zqm.tianlin.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://dth.xingfuxueyuan.xyz

[S46] C++：函数模板
来源：http://phd.sjlbkw.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sla.fehbvm.com

[S47] C++：结构化绑定遍历
来源：http://biw.fzhhl.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pfg.jinqigufen.top

[S48] C++：逐行读文件
来源：http://vkc.xylfe.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sjy.chenlongwang.top

while (std::getline(in, line)) { }
来源：http://mwa.yangfankeji.com

[S49] C++：写文件
来源：http://lwe.pycfn.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jdk.ywan-chungtsiang.top

[S50] C++：格式化数字
来源：http://dme.hywenlv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kra.ehwqpu.com

[S51] C++：显式类型转换
来源：http://tvr.ydjk.org.cn

static_cast<double>(a) / b
来源：http://edt.gzhubu.top

[S52] C++：const 与 noexcept
来源：http://yom.52xcode.cn

int size() const noexcept { return n_; }
来源：http://fgn.haohaochexian.top

[S53] C++：移动语义
来源：http://yev.cheryme.top

std::vector<int> w = std::move(v);
来源：http://qww.nanxinkj.top

[S54] C++：异常处理
来源：http://qtb.hnqzz.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tdm.yj20258888.top

[S55] C++：结构化绑定
来源：http://uah.shangyingyoupin.top

auto [a, b] = std::make_pair(1, 2);
来源：http://vxp.sxryk.cn

[S56] C++：optional
来源：http://hht.hesvh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vcq.ydjk.org.cn

[S57] C++：编译期常量
来源：http://dwf.zhiwuduotai.top

constexpr int N = 10;
来源：http://uqh.nanxinkj.top

[S58] C++：命名空间
来源：http://mur.gogol.net.cn

namespace ns { int f() { return 1; } }
来源：http://erz.zhijiandao.cn

[S59] C++：静态断言
来源：http://pxe.iojbl.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://edw.yonumen.top

[S60] C++：遍历并删除元素
来源：http://cvf.chenzaomai.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uiz.havefunace.top

================================================================================
来源：http://snr.guowangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vzf.guowangkeji.top

================================================================================
来源：http://nqv.fanxiaobao.xyz

[T01] Kotlin：Hello World
来源：http://ubq.xingfuxueyuan.xyz

println("Hello")
来源：http://rmm.cheryme.top

[T02] Kotlin：变量
来源：http://ftm.shzxlz.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hxt.chenzaomai.com

[T03] Kotlin：字符串模板
来源：http://azx.xingfuxueyuan.xyz

"值: $b"
来源：http://cwx.hfpthk.cn

[T04] Kotlin：空安全
来源：http://mwz.guowangkeji.top

val n: String? = null;  n?.length
来源：http://one.zhijiandao.cn

[T05] Kotlin：when 表达式
来源：http://csu.yanxiufei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://anj.yuanzhike.top

[T06] Kotlin：集合映射
来源：http://ldk.chenzaomai.com

listOf(1, 2, 3).map { it * 2 }
来源：http://zot.feifeiyinyue.top

[T07] Kotlin：集合过滤
来源：http://qaq.yuanzhike.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://raj.hfpthk.cn

[T08] Kotlin：数据类
来源：http://ivd.cdnleiting.top

data class User(val name: String, val age: Int)
来源：http://iwy.nanxuanxn.top

[T09] Kotlin：扩展函数
来源：http://jqv.ywan-chungtsiang.top

fun String.exclaim() = this + "!"
来源：http://ruk.snrcjt.cn

[T10] Kotlin：默认参数
来源：http://kci.chenzaomai.com

fun greet(name: String = "World") = "Hi $name"
来源：http://wmx.jlsjyb.cn

[T11] Kotlin：协程
来源：http://dtd.jianghu66.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rsb.xuanzx.com

[T12] Kotlin：解构声明
来源：http://suz.ppjwa.cn

val (a, b) = Pair(1, 2)
来源：http://hdi.zhijiandao.cn

[T13] Kotlin：只读 Map
来源：http://aae.chenzaomai.com

val m = mapOf("a" to 1)
来源：http://pdo.yj202588.top

[T14] Kotlin：循环
来源：http://efn.hnxiangtu.top

for (i in 1..10) println(i)
来源：http://qdw.zhongyouzk.top

[T15] Kotlin：接口
来源：http://ngi.hnqzz.top

interface Shape { fun area(): Double }
来源：http://kwm.tian-w.cn

[T16] Swift：Hello World
来源：http://kmf.c1oappe.top

print("Hello")
来源：http://qij.cheryme.top

[T17] Swift：变量与常量
来源：http://nnb.guannengcc.top

var a = 1;  let b = 2
来源：http://nlo.mhx1999.top

[T18] Swift：字符串插值
来源：http://rlp.feifeiyinyue.top

"值: \(b)"
来源：http://ayg.fehbvm.com

[T19] Swift：可选绑定
来源：http://oxj.zycfv.cn

if let n = opt { print(n) }
来源：http://uqh.zhixingplan.top

[T20] Swift：数组操作
来源：http://lxl.daria6918.cn

var a = [1, 2, 3];  a.append(4)
来源：http://iso.gogol.net.cn

[T21] Swift：遍历
来源：http://pgw.9152youxi.cn

for x in a { print(x) }
来源：http://nli.cucudq.cn

[T22] Swift：字典
来源：http://mpe.yanxiufei.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dkj.zhaomingkeji.xyz

[T23] Swift：函数
来源：http://wng.chenzaomai.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jyp.bbcook.cn

[T24] Swift：闭包
来源：http://lpu.zhaomingkeji.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://xgw.zhijiandao.cn

[T25] Swift：结构体
来源：http://iig.c1oappe.top

struct P { var x: Int }
来源：http://pbr.birdmap.top

[T26] Swift：类与重写
来源：http://lfg.shanyushiyangkeji.top

class A: Base { override func f() {} }
来源：http://dxl.yj20258888.top

[T27] Swift：错误处理
来源：http://efw.zhaomingkeji.xyz

do { try f() } catch { print(error) }
来源：http://tdo.yonumen.top

[T28] Swift：枚举
来源：http://iym.sxryk.cn

enum Color { case red, green }
来源：http://ayh.hammf.cn

[T29] Swift：guard 提前返回
来源：http://zfz.jinyuanbaomall.cn

guard let x = opt else { return }
来源：http://gvc.birdmap.top

[T30] Swift：协议
来源：http://eme.ivvv.top

protocol Shape { func area() -> Double }
来源：http://enr.ydjk.org.cn

[T31] Lua：Hello World
来源：http://htk.jqgfzy.top

print("Hello")
来源：http://kdb.yfazqb.com

[T32] Lua：局部变量
来源：http://cio.cashguo.top

local a = 1
来源：http://sax.yonumen.top

[T33] Lua：表（数组）
来源：http://bzq.yanxiufei.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lcq.jyoumei.cn

[T34] Lua：遍历表
来源：http://fcs.vehdjk.com

for i, v in ipairs(t) do print(i, v) end
来源：http://ilz.yj20258888.top

[T35] Lua：字典表
来源：http://hwk.chenzaomai.com

local d = { a = 1 };  d.b = 2
来源：http://fvy.shuidangran.top

[T36] Lua：函数
来源：http://ujf.dashuyun.cn

function add(a, b) return a + b end
来源：http://pvk.fengsongda.top

[T37] Lua：字符串拼接
来源：http://xgj.nwbrower.top

"a" .. "b"
来源：http://dmt.fanxiaobao.xyz

[T38] Lua：条件
来源：http://lsr.snrcjt.cn

if x > 0 then print("正") end
来源：http://res.sufxvd.cn

[T39] Lua：模式匹配
来源：http://cam.shanyushiyangtech.top

string.find(s, "%d+")
来源：http://spf.shuidangran.top

[T40] Lua：元表
来源：http://key.yueranfly.top

setmetatable({}, { __index = base })
来源：http://wcx.tianlin.xyz

[T41] Perl：Hello World
来源：http://snd.cdnleiting.top

print "Hello\n";
来源：http://sft.jinqigfzy.top

[T42] Perl：变量类型
来源：http://emj.zycfv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mua.dianchejie.cn

[T43] Perl：字符串插值
来源：http://njf.hfpthk.cn

"值: $a"
来源：http://yns.vehdjk.com

[T44] Perl：条件
来源：http://ync.zhaomingkeji.xyz

if ($a > 0) { print "正"; }
来源：http://owa.chenjidiqi.icu

[T45] Perl：数组遍历
来源：http://bck.ivvv.top

for my $x (@arr) { print $x; }
来源：http://rwl.xingfuxueyuan.xyz

[T46] Perl：哈希操作
来源：http://qzk.vqdsnc.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fxn.fengsongda.top

[T47] Perl：正则捕获
来源：http://xwj.zdbjq.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qqn.meibo888.top

[T48] Perl：正则替换
来源：http://fih.cheryme.top

$s =~ s/old/new/g;
来源：http://hkm.tianlin.xyz

[T49] Perl：函数
来源：http://nmu.yongpay.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://opg.yangfankeji.com

[T50] Perl：逐行读文件
来源：http://pnd.tian-w.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://occ.yj20258.top

while (my $line = <$fh>) { print $line; }
来源：http://uoe.xuanzx.com

[T51] Scala：Hello World
来源：http://hey.52xcode.cn

println("Hello")
来源：http://yrt.jinghuilouyu.cn

[T52] Scala：变量
来源：http://aje.hesvh.cn

val a = 1;  var b = 2
来源：http://tjc.nanxinkj.top

[T53] Scala：字符串插值
来源：http://dzc.sjlbkw.cn

s"值: $b"
来源：http://aoc.fengsongda.top

[T54] Scala：集合映射
来源：http://mqz.yfazqb.com

List(1, 2, 3).map(_ * 2)
来源：http://eww.jlsjyb.cn

[T55] Scala：集合过滤
来源：http://lnk.tarul.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qbs.zycfv.cn

[T56] Scala：样例类
来源：http://coi.smart0.xyz

case class User(name: String, age: Int)
来源：http://gsx.hnxiangtu.top

[T57] Scala：模式匹配
来源：http://foj.xingfuxueyuan.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://cbl.sxryk.cn

[T58] Scala：函数定义
来源：http://fwv.ppjwa.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ttd.gogol.net.cn

[T59] Scala：循环
来源：http://qka.yj20258.top

for (i <- 1 to 10) println(i)
来源：http://jec.c1oappe.top

[T60] Scala：折叠
来源：http://svs.ctjpmb.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://shb.xylfe.cn

================================================================================
来源：http://olw.hammf.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fpi.zhixingplan.top

================================================================================
来源：http://oen.jiagoushi.top

[U01] Py：创建虚拟环境
来源：http://rnu.hongshengwenyu.top

python -m venv .venv && source .venv/bin/activate
来源：http://zpr.ppjwa.cn

[U02] Py：导出 / 安装依赖
来源：http://vvz.daxiang520.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qeu.sxryk.cn

[U03] Py：加载 .env 配置
来源：http://cbq.hywenlv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://boy.c1oappe.top

[U04] Py：变量调试打印
来源：http://alt.zdqjudy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://khc.zdbjq.cn

[U05] Py：列表去重且保序
来源：http://mfw.shuidangran.top

list(dict.fromkeys(arr))
来源：http://dgo.yvedp.cn

[U06] Py：合并两个字典
来源：http://ksu.quarkkingdee.top

{**a, **b}
来源：http://fuu.gzhubu.top

[U07] Py：反转字典键值
来源：http://hyt.ppjwa.cn

{v: k for k, v in d.items()}
来源：http://pgd.xuanzx.com

[U08] Py：展平二维列表
来源：http://uur.zdbjq.cn

[y for x in nested for y in x]
来源：http://avu.tanke756.top


<!-- 参考信息 -->