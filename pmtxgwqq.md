代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://mdm.xuanzx.com

[R70] 时间戳与互转
来源：http://pwk.9152youxi.cn

date +%s;  date -d @1700000000
来源：http://vik.vqdsnc.cn

[R71] 日期格式化
来源：http://tzx.jinqigfzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bmg.yvedp.cn

[R72] 等待端口就绪
来源：http://imp.jlsjyb.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xpd.fzhhl.top

[R73] 分割大日志
来源：http://usy.chenlongwang.top

split -l 1000 big.log part_
来源：http://iws.ehwqpu.com

[R74] 批量重命名
来源：http://vzw.zdqjudy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xoe.chenjidiqi.icu

[R75] 导出环境变量
来源：http://mlx.fktsv.cn

export PATH="$HOME/bin:$PATH"
来源：http://nkv.zhaomingkeji.xyz

[R76] 使用临时文件
来源：http://xuq.jinqigfzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://obl.hywenlv.cn

[R77] 读取用户输入
来源：http://wgk.hnqzz.top

read -rp "请输入: " ans
来源：http://igh.gzhubu.top

[R78] 交互式菜单
来源：http://zni.iojbl.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nbm.shanyushiyangkeji.top

[R79] 解析命令行选项
来源：http://mwv.yvedp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vnw.sweek.top

[R80] 查看脚本执行耗时
来源：http://dtp.fzhhl.top

time ./run.sh
来源：http://ylm.316326.xyz

================================================================================
来源：http://zfb.hysaishi.cn

S. C / C++ 专题
来源：http://cxd.zhaomingkeji.xyz

================================================================================
来源：http://giy.hcnkem.com

[S01] C：Hello World
来源：http://nhk.sufxvd.cn

#include <stdio.h>
来源：http://prr.tian-w.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tkn.c1oappe.top

[S02] C：变量与格式化输出
来源：http://qgz.ppjwa.cn

int a = 10; printf("%d\n", a);
来源：http://pqj.svipenyu.cn

[S03] C：读入整数
来源：http://oih.yuanzhike.top

int x; scanf("%d", &x);
来源：http://nss.meibo888.top

[S04] C：字符串复制
来源：http://hdo.tarul.cn

char dst[32]; strcpy(dst, "hi");
来源：http://czi.dashuyun.cn

[S05] C：字符串长度
来源：http://zps.haohaochexian.top

strlen(s)
来源：http://mqi.ybcxt.top

[S06] C：字符串比较
来源：http://qan.shzxlz.cn

strcmp(a, b) == 0
来源：http://hbx.ppjwa.cn

[S07] C：数组遍历求和
来源：http://nol.shanyushiyangkeji.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uye.xuetiantiany.cn

[S08] C：动态内存分配与释放
来源：http://avq.wangdashe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rkv.zhixingplan.top

[S09] C：结构体定义与初始化
来源：http://sbn.fanxiaobao.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yaz.vehdjk.com

[S10] C：指针与解引用
来源：http://cfx.zhongyouzk.top

int *p = &a;  *p = 5;
来源：http://wdc.chenlongwang.top

[S11] C：逐行读文件
来源：http://txp.nanxinkj.top

FILE *f = fopen("a.txt", "r");
来源：http://olp.guowangkeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://tmc.gzhubu.top

fclose(f);
来源：http://plk.zdbjq.cn

[S12] C：写文件
来源：http://bsd.hysaishi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zyq.fzhhl.top

[S13] C：宏定义
来源：http://mzt.yuanzhike.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kfo.zdqjudy.top

[S14] C：枚举
来源：http://zmu.hesvh.cn

enum Color { RED, GREEN, BLUE };
来源：http://wke.shanyushiyangtech.top

[S15] C：类型转换
来源：http://srs.xinyue.icu

(double) a / b
来源：http://lcl.zhijiandao.cn

[S16] C：位操作置位
来源：http://ckn.xziqi.cn

x |= (1 << 3);
来源：http://tri.fanxiaobao.xyz

[S17] C：安全拼接字符串
来源：http://ffr.hnqzz.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rwr.fzhhl.top

[S18] C：命令行参数
来源：http://rgu.chenzaomai.com

int main(int argc, char **argv)
来源：http://nhb.meibo888.top

[S19] C：快速排序
来源：http://dzb.zhixingplan.top

qsort(a, n, sizeof(int), cmp);
来源：http://lle.andypj.xyz

[S20] C：二分查找
来源：http://sif.52xcode.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kki.ivvv.top

[S21] C：字符类别判断
来源：http://mhp.zhiwuduotai.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wsp.hnxiangtu.top

[S22] C：字符串转数字
来源：http://coj.jinghuilouyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sac.ywan-chungtsiang.top

[S23] C：随机数
来源：http://ocn.epnwcf.com

srand(time(NULL));  int r = rand() % 100;
来源：http://ycb.iojbl.cn

[S24] C：获取本地时间
来源：http://hgo.xinyue.icu

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fgu.daxiang520.top

[S25] C：内存拷贝
来源：http://hvd.tianlin.xyz

memcpy(dst, src, n);
来源：http://tou.hnqzz.top

[S26] C：内存清零
来源：http://wvh.xuetiantiany.cn

memset(a, 0, sizeof a);
来源：http://iqp.aibaodan.cn

[S27] C：定义常量
来源：http://eak.yangfankeji.com

const double PI = 3.14159;
来源：http://ays.jqgufenzy.top

[S28] C：静态变量
来源：http://jxq.xingfuxueyuan.xyz

static int counter = 0;
来源：http://tmu.yuxming.cn

[S29] C：变参函数
来源：http://rqt.epnwcf.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nwh.ydzc1.top

[S30] C：头文件保护
来源：http://kcx.zhongyouzk.top

#ifndef X_H
来源：http://aln.cheryme.top

#define X_H
来源：http://jjs.gaohongyu789.top

#endif
来源：http://zkx.hywenlv.cn

[S31] C++：Hello World
来源：http://igb.ppjwa.cn

#include <iostream>
来源：http://cwe.fehbvm.com

int main() { std::cout << "Hello\n"; }
来源：http://koq.yuanzhike.top

[S32] C++：字符串
来源：http://gab.yj20258.top

std::string s = "hi";  s += "!";
来源：http://ubz.bjfxy.top

[S33] C++：vector 增删
来源：http://ggo.jinghuilouyu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zxo.sysykeji.top

[S34] C++：遍历 vector
来源：http://zvx.shanyushiyangtech.top

for (auto &x : v) { std::cout << x; }
来源：http://vef.feifeiyinyue.top

[S35] C++：map
来源：http://fwa.feifeiyinyue.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jug.vehdjk.com

[S36] C++：unordered_map
来源：http://ulc.cheryme.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://frt.jiagoushi.top

[S37] C++：set
来源：http://jmt.cdnleiting.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://als.hfpthk.cn

[S38] C++：排序
来源：http://shr.nwbrower.top

std::sort(v.begin(), v.end());
来源：http://olr.shanyushiyangtech.top

[S39] C++：自定义比较器排序
来源：http://lcd.yj202588.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://teb.snrcjt.cn

[S40] C++：查找元素
来源：http://aws.mhx1999.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zpi.redwolf501.top

[S41] C++：类与构造函数
来源：http://hir.zhengqikj.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://njq.ehwqpu.com

[S42] C++：继承与虚函数
来源：http://cbe.hfpthk.cn

class B : public Base { public: void f() override {} };
来源：http://zsb.zhongyouzk.top

[S43] C++：智能指针
来源：http://bgv.epnwcf.com

auto p = std::make_unique<int>(5);
来源：http://atd.xziqi.cn

[S44] C++：引用传参
来源：http://lbz.dianchejie.cn

void inc(int &x) { ++x; }
来源：http://jqk.ppjwa.cn

[S45] C++：lambda
来源：http://vuj.chenlongwang.top

auto add = [](int a, int b) { return a + b; };
来源：http://hha.jinqigfzy.top

[S46] C++：函数模板
来源：http://frv.jinghuilouyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://aoz.birdmap.top

[S47] C++：结构化绑定遍历
来源：http://sqk.chenzaomai.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oxc.uphjek.com

[S48] C++：逐行读文件
来源：http://rjm.hnxiangtu.top

std::ifstream in("a.txt");  std::string line;
来源：http://irb.52xcode.cn

while (std::getline(in, line)) { }
来源：http://hxc.tian-w.cn

[S49] C++：写文件
来源：http://dep.cqqwz.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wli.gogol.net.cn

[S50] C++：格式化数字
来源：http://mgw.guannengcc.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://avi.havefunace.top

[S51] C++：显式类型转换
来源：http://zhz.jqgfzy.top

static_cast<double>(a) / b
来源：http://qgn.hongshengwenyu.top

[S52] C++：const 与 noexcept
来源：http://xla.fanxiaobao.xyz

int size() const noexcept { return n_; }
来源：http://zis.316326.xyz

[S53] C++：移动语义
来源：http://qet.yj20258.top

std::vector<int> w = std::move(v);
来源：http://cur.gotoacloud.top

[S54] C++：异常处理
来源：http://fuf.yueranfly.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sjm.0kj1m.cn

[S55] C++：结构化绑定
来源：http://jlg.sxryk.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vdc.hnqzz.top

[S56] C++：optional
来源：http://leq.chenzaomai.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://myu.ehwqpu.com

[S57] C++：编译期常量
来源：http://utg.yfazqb.com

constexpr int N = 10;
来源：http://elz.pycfn.com

[S58] C++：命名空间
来源：http://kfg.shanyushiyangtech.top

namespace ns { int f() { return 1; } }
来源：http://otq.havefunace.top

[S59] C++：静态断言
来源：http://xbk.gogol.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rgl.aibaodan.cn

[S60] C++：遍历并删除元素
来源：http://mbp.jqgufenzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qjv.hammf.cn

================================================================================
来源：http://sut.epnwcf.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://joo.shuidangran.top

================================================================================
来源：http://vjz.ivvv.top

[T01] Kotlin：Hello World
来源：http://zkh.yj202588.top

println("Hello")
来源：http://dzj.jianghu66.top

[T02] Kotlin：变量
来源：http://itq.zhoulong.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jgp.havefunace.top

[T03] Kotlin：字符串模板
来源：http://mam.xingfuxueyuan.xyz

"值: $b"
来源：http://vmt.zdbjq.cn

[T04] Kotlin：空安全
来源：http://bqd.meibo888.top

val n: String? = null;  n?.length
来源：http://wzn.vehdjk.com

[T05] Kotlin：when 表达式
来源：http://wbp.jinghuilouyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gje.c1oappe.top

[T06] Kotlin：集合映射
来源：http://lui.chenzaomai.com

listOf(1, 2, 3).map { it * 2 }
来源：http://oqu.zhaomingkeji.xyz

[T07] Kotlin：集合过滤
来源：http://moc.zhiwuduotai.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://yvy.ppjwa.cn

[T08] Kotlin：数据类
来源：http://oyr.tarul.cn

data class User(val name: String, val age: Int)
来源：http://imu.bbcook.cn

[T09] Kotlin：扩展函数
来源：http://ofg.chenzaomai.com

fun String.exclaim() = this + "!"
来源：http://fbo.sweek.top

[T10] Kotlin：默认参数
来源：http://ahb.sufxvd.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lpz.jinqigufen.top

[T11] Kotlin：协程
来源：http://new.shzxlz.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gub.gzhubu.top

[T12] Kotlin：解构声明
来源：http://vpg.smart0.xyz

val (a, b) = Pair(1, 2)
来源：http://zfp.xuanzx.com

[T13] Kotlin：只读 Map
来源：http://xni.0kj1m.cn

val m = mapOf("a" to 1)
来源：http://ytj.xuanzx.com

[T14] Kotlin：循环
来源：http://vrj.nwbrower.top

for (i in 1..10) println(i)
来源：http://ccr.yongpay.top

[T15] Kotlin：接口
来源：http://efd.cdnleiting.top

interface Shape { fun area(): Double }
来源：http://orc.fehbvm.com

[T16] Swift：Hello World
来源：http://ubd.ywan-chungtsiang.top

print("Hello")
来源：http://mnr.yj202588.top

[T17] Swift：变量与常量
来源：http://ikv.bjfxy.top

var a = 1;  let b = 2
来源：http://yqy.ydzc1.top

[T18] Swift：字符串插值
来源：http://sos.aizwys.cn

"值: \(b)"
来源：http://ifk.vqdsnc.cn

[T19] Swift：可选绑定
来源：http://uar.ywan-chungtsiang.top

if let n = opt { print(n) }
来源：http://idb.hnxiangtu.top

[T20] Swift：数组操作
来源：http://arj.vehdjk.com

var a = [1, 2, 3];  a.append(4)
来源：http://fij.fanxiaobao.xyz

[T21] Swift：遍历
来源：http://gkb.cqqwz.cn

for x in a { print(x) }
来源：http://jwe.hcnkem.com

[T22] Swift：字典
来源：http://iot.sweek.top

var d = ["a": 1];  d["b"] = 2
来源：http://mxk.yangfankeji.com

[T23] Swift：函数
来源：http://onn.gaohongyu789.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fww.shanyushiyangkeji.top

[T24] Swift：闭包
来源：http://tre.chenlongwang.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://noz.meibo888.top

[T25] Swift：结构体
来源：http://jmu.zhongyouzk.top

struct P { var x: Int }
来源：http://qgy.dianchejie.cn

[T26] Swift：类与重写
来源：http://uxk.pengpengdd.cyou

class A: Base { override func f() {} }
来源：http://pcf.yj20258888.top

[T27] Swift：错误处理
来源：http://lza.xinyue.icu

do { try f() } catch { print(error) }
来源：http://idv.jyoumei.cn

[T28] Swift：枚举
来源：http://erm.shanyushiyangtech.top

enum Color { case red, green }
来源：http://tzi.feifeiyinyue.top

[T29] Swift：guard 提前返回
来源：http://kwg.wangshuangyany.cn

guard let x = opt else { return }
来源：http://ltd.hongshengwenyu.top

[T30] Swift：协议
来源：http://yyd.jinghuilouyu.cn

protocol Shape { func area() -> Double }
来源：http://jcw.fehbvm.com

[T31] Lua：Hello World
来源：http://gbj.jinqigufen.top

print("Hello")
来源：http://nff.andypj.xyz

[T32] Lua：局部变量
来源：http://hcj.dianchejie.cn

local a = 1
来源：http://lsp.jinyuanbaomall.cn

[T33] Lua：表（数组）
来源：http://nou.zhoulong.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://ncm.wangshuangyany.cn

[T34] Lua：遍历表
来源：http://sid.yueranfly.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ddf.gzhubu.top

[T35] Lua：字典表
来源：http://zou.yvedp.cn

local d = { a = 1 };  d.b = 2
来源：http://ptj.shanyushiyangkeji.top

[T36] Lua：函数
来源：http://axm.vehdjk.com

function add(a, b) return a + b end
来源：http://rtf.wangdashe.top

[T37] Lua：字符串拼接
来源：http://lgr.9152youxi.cn

"a" .. "b"
来源：http://xwt.chenjidiqi.icu

[T38] Lua：条件
来源：http://uhm.jinyuanbaomall.cn

if x > 0 then print("正") end
来源：http://cfl.yueranfly.top

[T39] Lua：模式匹配
来源：http://yec.sweek.top

string.find(s, "%d+")
来源：http://imi.shangyingyoupin.top

[T40] Lua：元表
来源：http://ylj.chenzaomai.com

setmetatable({}, { __index = base })
来源：http://gwq.shanyushiyangkeji.top

[T41] Perl：Hello World
来源：http://xev.svipenyu.cn

print "Hello\n";
来源：http://rjm.yueranfly.top

[T42] Perl：变量类型
来源：http://jho.hywenlv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bev.zhiwuduotai.top

[T43] Perl：字符串插值
来源：http://owj.gotoacloud.top

"值: $a"
来源：http://mkk.jqgufenzy.top

[T44] Perl：条件
来源：http://iwi.epnwcf.com

if ($a > 0) { print "正"; }
来源：http://bpa.shzxlz.cn

[T45] Perl：数组遍历
来源：http://vgz.hongshengwenyu.top

for my $x (@arr) { print $x; }
来源：http://itf.shangyingyoupin.top

[T46] Perl：哈希操作
来源：http://fic.ehwqpu.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://igb.ydjk.org.cn

[T47] Perl：正则捕获
来源：http://htx.jinyuanbaomall.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gqi.xziqi.cn

[T48] Perl：正则替换
来源：http://jqj.gotoacloud.top

$s =~ s/old/new/g;
来源：http://gyb.zhoulong.xyz

[T49] Perl：函数
来源：http://xny.hnxiangtu.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mvt.cashguo.top

[T50] Perl：逐行读文件
来源：http://dcp.0kj1m.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://exg.xziqi.cn

while (my $line = <$fh>) { print $line; }
来源：http://vgt.shangyingyoupin.top

[T51] Scala：Hello World
来源：http://llt.meibo888.top

println("Hello")
来源：http://bly.hnxiangtu.top

[T52] Scala：变量
来源：http://lpe.pengpengdd.cyou

val a = 1;  var b = 2
来源：http://ixj.ctjpmb.com

[T53] Scala：字符串插值
来源：http://hwn.jyoumei.cn

s"值: $b"
来源：http://fya.fanxiaobao.xyz

[T54] Scala：集合映射
来源：http://nux.hnxiangtu.top

List(1, 2, 3).map(_ * 2)
来源：http://mrv.cdnleiting.top

[T55] Scala：集合过滤
来源：http://ibn.xziqi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wvy.ppjwa.cn

[T56] Scala：样例类
来源：http://fhd.zhoulong.xyz

case class User(name: String, age: Int)
来源：http://cct.birdmap.top

[T57] Scala：模式匹配
来源：http://vcy.wangdashe.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://otw.zhiwuduotai.top

[T58] Scala：函数定义
来源：http://yvz.epnwcf.com

def add(a: Int, b: Int): Int = a + b
来源：http://mkx.vehdjk.com

[T59] Scala：循环
来源：http://qtx.sysykeji.top

for (i <- 1 to 10) println(i)
来源：http://tgi.cashguo.top

[T60] Scala：折叠
来源：http://fap.quarkkingdee.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wlv.0kj1m.cn

================================================================================
来源：http://kfb.nanxinkj.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ymw.fengsongda.top

================================================================================
来源：http://crq.daria6918.cn

[U01] Py：创建虚拟环境
来源：http://iba.chenlongwang.top

python -m venv .venv && source .venv/bin/activate
来源：http://wpw.chenjidiqi.icu

[U02] Py：导出 / 安装依赖
来源：http://say.hysaishi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://drw.tarul.cn

[U03] Py：加载 .env 配置
来源：http://lap.jinqigufen.top

from dotenv import load_dotenv; load_dotenv()
来源：http://hvy.cashguo.top

[U04] Py：变量调试打印
来源：http://zpy.52xcode.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ten.wangshuangyany.cn

[U05] Py：列表去重且保序
来源：http://ism.bjfxy.top

list(dict.fromkeys(arr))
来源：http://jyi.gogol.net.cn

[U06] Py：合并两个字典
来源：http://cxz.yuanzhike.top

{**a, **b}
来源：http://inx.yangfankeji.com

[U07] Py：反转字典键值
来源：http://exh.mhx1999.top

{v: k for k, v in d.items()}
来源：http://eps.sysykeji.top

[U08] Py：展平二维列表
来源：http://elq.zhijiandao.cn

[y for x in nested for y in x]
来源：http://pmy.tianlin.xyz

[U09] Py：字典取最大值的键
来源：http://cyy.ctjpmb.com

max(d, key=d.get)
来源：http://dpb.pengpengdd.cyou

[U10] Py：按值排序字典
来源：http://bwm.chenzaomai.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zjp.ydzc1.top


<!-- 参考信息 -->