代发 wailian999

free -h;  ps aux | grep nginx
来源：http://ucv.fktsv.cn

[R64] 结束进程
来源：http://kya.gaohongyu789.top

kill -9 $(pgrep -f app.py)
来源：http://uuc.nwbrower.top

[R65] 查看端口占用
来源：http://juy.daxiang520.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://onp.hammf.cn

[R66] 定时任务
来源：http://ecb.xuanzx.com

crontab -e;  crontab -l
来源：http://iyy.zycfv.cn

[R67] 生成随机十六进制串
来源：http://bpa.xuetiantiany.cn

openssl rand -hex 16
来源：http://poy.havefunace.top

[R68] 计算文件校验值
来源：http://sbl.zhaomingkeji.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://vlb.ppjwa.cn

[R69] 生成随机密码
来源：http://ulp.ehwqpu.com

head -c 16 /dev/urandom | base64
来源：http://lfa.hysaishi.cn

[R70] 时间戳与互转
来源：http://dta.ppjwa.cn

date +%s;  date -d @1700000000
来源：http://vtx.fehbvm.com

[R71] 日期格式化
来源：http://vzi.316326.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://yzu.yongpay.top

[R72] 等待端口就绪
来源：http://unf.daxiang520.top

until nc -z localhost 3306; do sleep 1; done
来源：http://mfa.snrcjt.cn

[R73] 分割大日志
来源：http://psi.jqgufenzy.top

split -l 1000 big.log part_
来源：http://erl.iojbl.cn

[R74] 批量重命名
来源：http://xsz.yangfankeji.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://igt.shanyushiyangkeji.top

[R75] 导出环境变量
来源：http://elz.shanyushiyangtech.top

export PATH="$HOME/bin:$PATH"
来源：http://hbi.yuanzhike.top

[R76] 使用临时文件
来源：http://kkn.zhongyouzk.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kox.svipenyu.cn

[R77] 读取用户输入
来源：http://tgl.birdmap.top

read -rp "请输入: " ans
来源：http://igt.fanxiaobao.xyz

[R78] 交互式菜单
来源：http://ozx.ydzc1.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ipg.guannengcc.top

[R79] 解析命令行选项
来源：http://cdr.shuidangran.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://osr.jqgfzy.top

[R80] 查看脚本执行耗时
来源：http://xfw.bbcook.cn

time ./run.sh
来源：http://unq.hcnkem.com

================================================================================
来源：http://mja.zhongyouzk.top

S. C / C++ 专题
来源：http://pvn.zhixingplan.top

================================================================================
来源：http://wqi.tarul.cn

[S01] C：Hello World
来源：http://jgc.shanyushiyangkeji.top

#include <stdio.h>
来源：http://gxa.ydzc1.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://tuw.yvedp.cn

[S02] C：变量与格式化输出
来源：http://ggo.vqdsnc.cn

int a = 10; printf("%d\n", a);
来源：http://psc.redwolf501.top

[S03] C：读入整数
来源：http://lot.zhijiandao.cn

int x; scanf("%d", &x);
来源：http://qac.zhengqikj.top

[S04] C：字符串复制
来源：http://ioz.hywenlv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wie.mhx1999.top

[S05] C：字符串长度
来源：http://fbp.yfazqb.com

strlen(s)
来源：http://evq.xuanzx.com

[S06] C：字符串比较
来源：http://hrh.tanke756.top

strcmp(a, b) == 0
来源：http://mdz.sweek.top

[S07] C：数组遍历求和
来源：http://tdl.316326.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xnu.sjlbkw.cn

[S08] C：动态内存分配与释放
来源：http://bmt.xuanzx.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dld.cheryme.top

[S09] C：结构体定义与初始化
来源：http://bfa.zhongyouzk.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lvs.iojbl.cn

[S10] C：指针与解引用
来源：http://fmk.hywenlv.cn

int *p = &a;  *p = 5;
来源：http://aby.birdmap.top

[S11] C：逐行读文件
来源：http://ljk.feifeiyinyue.top

FILE *f = fopen("a.txt", "r");
来源：http://ekl.yangfankeji.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://neh.hongshengwenyu.top

fclose(f);
来源：http://svy.ywan-chungtsiang.top

[S12] C：写文件
来源：http://txz.ppjwa.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fyo.wangdashe.top

[S13] C：宏定义
来源：http://bbj.mhx1999.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qxm.hnqzz.top

[S14] C：枚举
来源：http://esw.yanxiufei.cn

enum Color { RED, GREEN, BLUE };
来源：http://ppy.vehdjk.com

[S15] C：类型转换
来源：http://cyn.hywenlv.cn

(double) a / b
来源：http://mbv.cqqwz.cn

[S16] C：位操作置位
来源：http://bie.zhengqikj.top

x |= (1 << 3);
来源：http://qdy.gogol.net.cn

[S17] C：安全拼接字符串
来源：http://koo.jiagoushi.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://smv.hnqzz.top

[S18] C：命令行参数
来源：http://bhk.nanxuanxn.top

int main(int argc, char **argv)
来源：http://qkr.gotoacloud.top

[S19] C：快速排序
来源：http://mxs.ydjk.org.cn

qsort(a, n, sizeof(int), cmp);
来源：http://elu.hysaishi.cn

[S20] C：二分查找
来源：http://ror.shuidangran.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bfa.sweek.top

[S21] C：字符类别判断
来源：http://wjb.zycfv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://myp.aibaodan.cn

[S22] C：字符串转数字
来源：http://abq.ydjk.org.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sro.andypj.xyz

[S23] C：随机数
来源：http://qxp.jinghuilouyu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mqb.jqgufenzy.top

[S24] C：获取本地时间
来源：http://jtz.gogol.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fol.shuidangran.top

[S25] C：内存拷贝
来源：http://pbh.kuanghao11.cn

memcpy(dst, src, n);
来源：http://ele.tian-w.cn

[S26] C：内存清零
来源：http://pac.aibaodan.cn

memset(a, 0, sizeof a);
来源：http://pxk.jqgufenzy.top

[S27] C：定义常量
来源：http://bci.shzxlz.cn

const double PI = 3.14159;
来源：http://dcj.pycfn.com

[S28] C：静态变量
来源：http://soi.zhongyouzk.top

static int counter = 0;
来源：http://ugr.birdmap.top

[S29] C：变参函数
来源：http://iwv.hcnkem.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bwc.yonumen.top

[S30] C：头文件保护
来源：http://mci.hnxiangtu.top

#ifndef X_H
来源：http://srj.sysykeji.top

#define X_H
来源：http://gbr.jlsjyb.cn

#endif
来源：http://zgw.daria6918.cn

[S31] C++：Hello World
来源：http://zil.wangdashe.top

#include <iostream>
来源：http://zlm.xingfuxueyuan.xyz

int main() { std::cout << "Hello\n"; }
来源：http://vay.nanxuanxn.top

[S32] C++：字符串
来源：http://ihp.zhiwuduotai.top

std::string s = "hi";  s += "!";
来源：http://oia.redwolf501.top

[S33] C++：vector 增删
来源：http://okb.hysaishi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ghk.yj20258888.top

[S34] C++：遍历 vector
来源：http://wbd.cucudq.cn

for (auto &x : v) { std::cout << x; }
来源：http://hkr.gogol.net.cn

[S35] C++：map
来源：http://bkw.sjlbkw.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sgd.zhijiandao.cn

[S36] C++：unordered_map
来源：http://fbf.cucudq.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ykl.gaohongyu789.top

[S37] C++：set
来源：http://jhw.gzhubu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ihx.gogol.net.cn

[S38] C++：排序
来源：http://zvw.shanyushiyangkeji.top

std::sort(v.begin(), v.end());
来源：http://mqx.chenlongwang.top

[S39] C++：自定义比较器排序
来源：http://osq.yanxiufei.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tmz.xingfuxueyuan.xyz

[S40] C++：查找元素
来源：http://ois.jinghuilouyu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nga.yangfankeji.com

[S41] C++：类与构造函数
来源：http://php.ivvv.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hqo.hfpthk.cn

[S42] C++：继承与虚函数
来源：http://dlt.sweek.top

class B : public Base { public: void f() override {} };
来源：http://twq.fengsongda.top

[S43] C++：智能指针
来源：http://iae.ivvv.top

auto p = std::make_unique<int>(5);
来源：http://ren.hfpthk.cn

[S44] C++：引用传参
来源：http://mds.chenjidiqi.icu

void inc(int &x) { ++x; }
来源：http://nce.yonumen.top

[S45] C++：lambda
来源：http://kss.jinqigufen.top

auto add = [](int a, int b) { return a + b; };
来源：http://uuy.52xcode.cn

[S46] C++：函数模板
来源：http://mqv.shanyushiyangkeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ssa.jinqigfzy.top

[S47] C++：结构化绑定遍历
来源：http://duo.xylfe.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://svw.yonumen.top

[S48] C++：逐行读文件
来源：http://qnz.wangshuangyany.cn

std::ifstream in("a.txt");  std::string line;
来源：http://aeu.sjlbkw.cn

while (std::getline(in, line)) { }
来源：http://awf.daxiang520.top

[S49] C++：写文件
来源：http://sej.epnwcf.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zxi.sysykeji.top

[S50] C++：格式化数字
来源：http://qen.yuxming.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tjj.wangshuangyany.cn

[S51] C++：显式类型转换
来源：http://qkd.fzhhl.top

static_cast<double>(a) / b
来源：http://idi.52xcode.cn

[S52] C++：const 与 noexcept
来源：http://lzo.hnqzz.top

int size() const noexcept { return n_; }
来源：http://abb.xziqi.cn

[S53] C++：移动语义
来源：http://tyc.sysykeji.top

std::vector<int> w = std::move(v);
来源：http://fcc.hnqzz.top

[S54] C++：异常处理
来源：http://szg.aizwys.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://obl.fanxiaobao.xyz

[S55] C++：结构化绑定
来源：http://pqs.zycfv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://grt.ehwqpu.com

[S56] C++：optional
来源：http://oic.jinqigufen.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pgt.fzhhl.top

[S57] C++：编译期常量
来源：http://qti.zhiwuduotai.top

constexpr int N = 10;
来源：http://mkm.sweek.top

[S58] C++：命名空间
来源：http://ynp.redwolf501.top

namespace ns { int f() { return 1; } }
来源：http://nuv.fanxiaobao.xyz

[S59] C++：静态断言
来源：http://lhk.zhongyouzk.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ijw.havefunace.top

[S60] C++：遍历并删除元素
来源：http://kcg.quarkkingdee.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gtk.epnwcf.com

================================================================================
来源：http://erw.hysaishi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ovz.xziqi.cn

================================================================================
来源：http://bxm.yuanzhike.top

[T01] Kotlin：Hello World
来源：http://dkl.zhongyouzk.top

println("Hello")
来源：http://prk.iojbl.cn

[T02] Kotlin：变量
来源：http://gxj.yanxiufei.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yyu.havefunace.top

[T03] Kotlin：字符串模板
来源：http://ddd.316326.xyz

"值: $b"
来源：http://lhv.xingfuxueyuan.xyz

[T04] Kotlin：空安全
来源：http://mlf.xziqi.cn

val n: String? = null;  n?.length
来源：http://gby.zhengqikj.top

[T05] Kotlin：when 表达式
来源：http://ima.jiagoushi.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tsf.fengsongda.top

[T06] Kotlin：集合映射
来源：http://dlu.shanyushiyangkeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://fwp.iojbl.cn

[T07] Kotlin：集合过滤
来源：http://dkh.hfpthk.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://irx.sysykeji.top

[T08] Kotlin：数据类
来源：http://cll.52xcode.cn

data class User(val name: String, val age: Int)
来源：http://set.jqgufenzy.top

[T09] Kotlin：扩展函数
来源：http://mdr.zhaomingkeji.xyz

fun String.exclaim() = this + "!"
来源：http://qsg.sweek.top

[T10] Kotlin：默认参数
来源：http://fwa.mhx1999.top

fun greet(name: String = "World") = "Hi $name"
来源：http://cgt.aizwys.cn

[T11] Kotlin：协程
来源：http://mvh.xuetiantiany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://umr.ctjpmb.com

[T12] Kotlin：解构声明
来源：http://ato.hnqzz.top

val (a, b) = Pair(1, 2)
来源：http://uzg.fengsongda.top

[T13] Kotlin：只读 Map
来源：http://gqr.meibo888.top

val m = mapOf("a" to 1)
来源：http://vod.jqgufenzy.top

[T14] Kotlin：循环
来源：http://kdo.xuetiantiany.cn

for (i in 1..10) println(i)
来源：http://nzm.shanyushiyangtech.top

[T15] Kotlin：接口
来源：http://hto.dashuyun.cn

interface Shape { fun area(): Double }
来源：http://gux.sysykeji.top

[T16] Swift：Hello World
来源：http://eet.vqdsnc.cn

print("Hello")
来源：http://btt.jianghu66.top

[T17] Swift：变量与常量
来源：http://bqj.ydjk.org.cn

var a = 1;  let b = 2
来源：http://bnd.ctjpmb.com

[T18] Swift：字符串插值
来源：http://umh.jianghu66.top

"值: \(b)"
来源：http://erj.zhaomingkeji.xyz

[T19] Swift：可选绑定
来源：http://otp.xziqi.cn

if let n = opt { print(n) }
来源：http://bff.zhengqikj.top

[T20] Swift：数组操作
来源：http://hhx.xingfuxueyuan.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://fqo.hnqzz.top

[T21] Swift：遍历
来源：http://foo.nanxuanxn.top

for x in a { print(x) }
来源：http://nek.tian-w.cn

[T22] Swift：字典
来源：http://atj.bbcook.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jxa.jianghu66.top

[T23] Swift：函数
来源：http://jcr.daxiang520.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jcc.yuxming.cn

[T24] Swift：闭包
来源：http://gdx.yuxming.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://nls.yj202588.top

[T25] Swift：结构体
来源：http://akw.zycfv.cn

struct P { var x: Int }
来源：http://qwf.sufxvd.cn

[T26] Swift：类与重写
来源：http://jap.wangshuangyany.cn

class A: Base { override func f() {} }
来源：http://swz.wangdashe.top

[T27] Swift：错误处理
来源：http://wgs.jlsjyb.cn

do { try f() } catch { print(error) }
来源：http://jpd.uphjek.com

[T28] Swift：枚举
来源：http://abu.fanxiaobao.xyz

enum Color { case red, green }
来源：http://gfb.cqqwz.cn

[T29] Swift：guard 提前返回
来源：http://ovj.dianchejie.cn

guard let x = opt else { return }
来源：http://nzm.ctjpmb.com

[T30] Swift：协议
来源：http://tkt.xinyue.icu

protocol Shape { func area() -> Double }
来源：http://bxe.xziqi.cn

[T31] Lua：Hello World
来源：http://ips.cheryme.top

print("Hello")
来源：http://xzk.0kj1m.cn

[T32] Lua：局部变量
来源：http://soo.0kj1m.cn

local a = 1
来源：http://yya.yangfankeji.com

[T33] Lua：表（数组）
来源：http://sad.xingfuxueyuan.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://hlm.daxiang520.top

[T34] Lua：遍历表
来源：http://hyt.birdmap.top

for i, v in ipairs(t) do print(i, v) end
来源：http://tzk.hnqzz.top

[T35] Lua：字典表
来源：http://nlw.shanyushiyangtech.top

local d = { a = 1 };  d.b = 2
来源：http://xga.hammf.cn

[T36] Lua：函数
来源：http://nio.ctjpmb.com

function add(a, b) return a + b end
来源：http://ceb.cucudq.cn

[T37] Lua：字符串拼接
来源：http://dlo.hesvh.cn

"a" .. "b"
来源：http://hmn.jinqigfzy.top

[T38] Lua：条件
来源：http://pxt.yj20258.top

if x > 0 then print("正") end
来源：http://uen.tian-w.cn

[T39] Lua：模式匹配
来源：http://wmb.gotoacloud.top

string.find(s, "%d+")
来源：http://xkq.ppjwa.cn

[T40] Lua：元表
来源：http://ijl.nanxuanxn.top

setmetatable({}, { __index = base })
来源：http://zez.xylfe.cn

[T41] Perl：Hello World
来源：http://zln.quarkkingdee.top

print "Hello\n";
来源：http://yhw.daxiang520.top

[T42] Perl：变量类型
来源：http://dnc.zhijiandao.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tab.sufxvd.cn

[T43] Perl：字符串插值
来源：http://ifx.bbcook.cn

"值: $a"
来源：http://aud.sysykeji.top

[T44] Perl：条件
来源：http://tzr.shzxlz.cn

if ($a > 0) { print "正"; }
来源：http://csg.hnqzz.top

[T45] Perl：数组遍历
来源：http://noy.jinqigufen.top

for my $x (@arr) { print $x; }
来源：http://foq.nwbrower.top

[T46] Perl：哈希操作
来源：http://bgh.yfazqb.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wne.hysaishi.cn

[T47] Perl：正则捕获
来源：http://wjg.fehbvm.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://zxb.iojbl.cn

[T48] Perl：正则替换
来源：http://xru.svipenyu.cn

$s =~ s/old/new/g;
来源：http://ccj.nwbrower.top

[T49] Perl：函数
来源：http://hro.chenlongwang.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://awa.yj20258.top

[T50] Perl：逐行读文件
来源：http://jtg.gogol.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hdc.cqqwz.cn

while (my $line = <$fh>) { print $line; }
来源：http://hvj.kuanghao11.cn

[T51] Scala：Hello World
来源：http://wza.cheryme.top

println("Hello")
来源：http://int.pengpengdd.cyou

[T52] Scala：变量
来源：http://dst.zdbjq.cn

val a = 1;  var b = 2
来源：http://ddx.nanxinkj.top

[T53] Scala：字符串插值
来源：http://elp.tanke756.top

s"值: $b"
来源：http://lmn.hysaishi.cn

[T54] Scala：集合映射
来源：http://qdy.zycfv.cn

List(1, 2, 3).map(_ * 2)
来源：http://mqe.daria6918.cn

[T55] Scala：集合过滤
来源：http://sit.jinqigfzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://kna.shzxlz.cn

[T56] Scala：样例类
来源：http://zkj.sxryk.cn

case class User(name: String, age: Int)
来源：http://wmi.dianchejie.cn

[T57] Scala：模式匹配
来源：http://bkm.jianghu66.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://bwm.jqgfzy.top

[T58] Scala：函数定义
来源：http://dyt.hysaishi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pnw.sweek.top

[T59] Scala：循环
来源：http://dlt.fanxiaobao.xyz

for (i <- 1 to 10) println(i)
来源：http://izx.shanyushiyangkeji.top

[T60] Scala：折叠
来源：http://rmq.bbcook.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hec.pycfn.com

================================================================================
来源：http://hqc.svipenyu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mgk.wangshuangyany.cn

================================================================================
来源：http://xbg.hesvh.cn

[U01] Py：创建虚拟环境
来源：http://spj.gzhubu.top

python -m venv .venv && source .venv/bin/activate
来源：http://rhn.sysykeji.top

[U02] Py：导出 / 安装依赖
来源：http://ckv.hongshengwenyu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kpq.dianchejie.cn

[U03] Py：加载 .env 配置
来源：http://tfp.fanxiaobao.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://xxg.fktsv.cn

[U04] Py：变量调试打印
来源：http://ntu.pycfn.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://egn.zhaomingkeji.xyz


<!-- 参考信息 -->