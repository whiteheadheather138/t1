代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xkt.meibo888.top

[R66] 定时任务
来源：http://ryr.yvedp.cn

crontab -e;  crontab -l
来源：http://bxe.vqdsnc.cn

[R67] 生成随机十六进制串
来源：http://dyr.bjfxy.top

openssl rand -hex 16
来源：http://bon.hysaishi.cn

[R68] 计算文件校验值
来源：http://ead.havefunace.top

sha256sum a.txt;  md5sum a.txt
来源：http://mbt.cdnleiting.top

[R69] 生成随机密码
来源：http://wun.hammf.cn

head -c 16 /dev/urandom | base64
来源：http://cok.chenjidiqi.icu

[R70] 时间戳与互转
来源：http://mrk.hongshengwenyu.top

date +%s;  date -d @1700000000
来源：http://osh.nwbrower.top

[R71] 日期格式化
来源：http://tar.xinyue.icu

date +"%Y-%m-%d %H:%M:%S"
来源：http://opa.chenzaomai.com

[R72] 等待端口就绪
来源：http://qgk.daxiang520.top

until nc -z localhost 3306; do sleep 1; done
来源：http://sol.snrcjt.cn

[R73] 分割大日志
来源：http://ssp.jqgufenzy.top

split -l 1000 big.log part_
来源：http://eyp.zhengqikj.top

[R74] 批量重命名
来源：http://mab.jinqigufen.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qgt.zdqjudy.top

[R75] 导出环境变量
来源：http://zhi.andypj.xyz

export PATH="$HOME/bin:$PATH"
来源：http://dko.shanyushiyangtech.top

[R76] 使用临时文件
来源：http://bko.hongshengwenyu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tso.zycfv.cn

[R77] 读取用户输入
来源：http://nps.jinqigfzy.top

read -rp "请输入: " ans
来源：http://swq.ctjpmb.com

[R78] 交互式菜单
来源：http://gwz.yuanzhike.top

select opt in a b c; do echo "$opt"; break; done
来源：http://bpp.jqgufenzy.top

[R79] 解析命令行选项
来源：http://zrm.sweek.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fas.cdnleiting.top

[R80] 查看脚本执行耗时
来源：http://ocb.0kj1m.cn

time ./run.sh
来源：http://vqe.quarkkingdee.top

================================================================================
来源：http://euq.gogol.net.cn

S. C / C++ 专题
来源：http://vfs.xuetiantiany.cn

================================================================================
来源：http://wcv.fktsv.cn

[S01] C：Hello World
来源：http://xvr.tianlin.xyz

#include <stdio.h>
来源：http://oaj.xylfe.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://edy.hfpthk.cn

[S02] C：变量与格式化输出
来源：http://qln.zhiwuduotai.top

int a = 10; printf("%d\n", a);
来源：http://syy.wangshuangyany.cn

[S03] C：读入整数
来源：http://rxl.vqdsnc.cn

int x; scanf("%d", &x);
来源：http://wfr.hcnkem.com

[S04] C：字符串复制
来源：http://qxr.pengpengdd.cyou

char dst[32]; strcpy(dst, "hi");
来源：http://ggf.c1oappe.top

[S05] C：字符串长度
来源：http://uet.sysykeji.top

strlen(s)
来源：http://bro.gotoacloud.top

[S06] C：字符串比较
来源：http://iuh.52xcode.cn

strcmp(a, b) == 0
来源：http://cbx.yangfankeji.com

[S07] C：数组遍历求和
来源：http://zcm.sufxvd.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://oid.yvedp.cn

[S08] C：动态内存分配与释放
来源：http://phm.xuetiantiany.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tfs.sjlbkw.cn

[S09] C：结构体定义与初始化
来源：http://ljx.tanke756.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hct.zdqjudy.top

[S10] C：指针与解引用
来源：http://jur.aibaodan.cn

int *p = &a;  *p = 5;
来源：http://vxy.bbcook.cn

[S11] C：逐行读文件
来源：http://omk.ppjwa.cn

FILE *f = fopen("a.txt", "r");
来源：http://uxj.yonumen.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://pbo.ehwqpu.com

fclose(f);
来源：http://unn.hnxiangtu.top

[S12] C：写文件
来源：http://bdi.xziqi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://odj.yj20258.top

[S13] C：宏定义
来源：http://dqq.hammf.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jtt.daxiang520.top

[S14] C：枚举
来源：http://nud.nanxinkj.top

enum Color { RED, GREEN, BLUE };
来源：http://png.nwbrower.top

[S15] C：类型转换
来源：http://yyg.jianghu66.top

(double) a / b
来源：http://dep.hnxiangtu.top

[S16] C：位操作置位
来源：http://sic.9152youxi.cn

x |= (1 << 3);
来源：http://gqz.xylfe.cn

[S17] C：安全拼接字符串
来源：http://eku.shanyushiyangtech.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ked.yj202588.top

[S18] C：命令行参数
来源：http://vif.xingfuxueyuan.xyz

int main(int argc, char **argv)
来源：http://ayi.zdqjudy.top

[S19] C：快速排序
来源：http://jgv.hnqzz.top

qsort(a, n, sizeof(int), cmp);
来源：http://usn.sxryk.cn

[S20] C：二分查找
来源：http://euv.andypj.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cbo.jinghuilouyu.cn

[S21] C：字符类别判断
来源：http://bmt.hysaishi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ybk.zhoulong.xyz

[S22] C：字符串转数字
来源：http://qil.yangfankeji.com

atoi("42");  strtod("3.14", NULL);
来源：http://iee.yuxming.cn

[S23] C：随机数
来源：http://jkz.wangshuangyany.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jfg.sweek.top

[S24] C：获取本地时间
来源：http://lel.snrcjt.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ajc.chenzaomai.com

[S25] C：内存拷贝
来源：http://fie.mhx1999.top

memcpy(dst, src, n);
来源：http://gga.aizwys.cn

[S26] C：内存清零
来源：http://umy.fehbvm.com

memset(a, 0, sizeof a);
来源：http://roh.sysykeji.top

[S27] C：定义常量
来源：http://buz.pycfn.com

const double PI = 3.14159;
来源：http://wip.0kj1m.cn

[S28] C：静态变量
来源：http://kmu.gaohongyu789.top

static int counter = 0;
来源：http://cqn.fanxiaobao.xyz

[S29] C：变参函数
来源：http://wmf.xziqi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dod.hesvh.cn

[S30] C：头文件保护
来源：http://sbr.tianlin.xyz

#ifndef X_H
来源：http://kps.tian-w.cn

#define X_H
来源：http://hsr.xuetiantiany.cn

#endif
来源：http://glz.cheryme.top

[S31] C++：Hello World
来源：http://few.uphjek.com

#include <iostream>
来源：http://tci.daria6918.cn

int main() { std::cout << "Hello\n"; }
来源：http://vzi.jianghu66.top

[S32] C++：字符串
来源：http://ban.yfazqb.com

std::string s = "hi";  s += "!";
来源：http://pvp.cucudq.cn

[S33] C++：vector 增删
来源：http://abx.zdqjudy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xug.jinqigufen.top

[S34] C++：遍历 vector
来源：http://kea.hesvh.cn

for (auto &x : v) { std::cout << x; }
来源：http://mwb.yfazqb.com

[S35] C++：map
来源：http://dns.pycfn.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://khu.gotoacloud.top

[S36] C++：unordered_map
来源：http://xrr.yfazqb.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xjj.yvedp.cn

[S37] C++：set
来源：http://ldl.wangdashe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://phv.pycfn.com

[S38] C++：排序
来源：http://yfh.nwbrower.top

std::sort(v.begin(), v.end());
来源：http://qcq.uphjek.com

[S39] C++：自定义比较器排序
来源：http://bzc.gotoacloud.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://umk.zycfv.cn

[S40] C++：查找元素
来源：http://ulc.jqgfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rco.pengpengdd.cyou

[S41] C++：类与构造函数
来源：http://qtd.daria6918.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kdy.zhengqikj.top

[S42] C++：继承与虚函数
来源：http://hij.uphjek.com

class B : public Base { public: void f() override {} };
来源：http://ibp.yangfankeji.com

[S43] C++：智能指针
来源：http://dnm.havefunace.top

auto p = std::make_unique<int>(5);
来源：http://hmt.yj20258.top

[S44] C++：引用传参
来源：http://yof.fzhhl.top

void inc(int &x) { ++x; }
来源：http://tau.tarul.cn

[S45] C++：lambda
来源：http://nhv.yuanzhike.top

auto add = [](int a, int b) { return a + b; };
来源：http://oxy.yonumen.top

[S46] C++：函数模板
来源：http://foc.xylfe.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://klc.yangfankeji.com

[S47] C++：结构化绑定遍历
来源：http://iba.sysykeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wkl.0kj1m.cn

[S48] C++：逐行读文件
来源：http://okq.xziqi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://svh.kuanghao11.cn

while (std::getline(in, line)) { }
来源：http://ysi.daxiang520.top

[S49] C++：写文件
来源：http://bdk.ydjk.org.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wha.sxryk.cn

[S50] C++：格式化数字
来源：http://spt.shuidangran.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xry.nwbrower.top

[S51] C++：显式类型转换
来源：http://aur.kuanghao11.cn

static_cast<double>(a) / b
来源：http://xga.cucudq.cn

[S52] C++：const 与 noexcept
来源：http://ybh.yfazqb.com

int size() const noexcept { return n_; }
来源：http://ncy.cdnleiting.top

[S53] C++：移动语义
来源：http://cby.hnqzz.top

std::vector<int> w = std::move(v);
来源：http://ons.jlsjyb.cn

[S54] C++：异常处理
来源：http://hrr.xylfe.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bhx.smart0.xyz

[S55] C++：结构化绑定
来源：http://foe.jyoumei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sna.wangdashe.top

[S56] C++：optional
来源：http://acy.ppjwa.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jkj.smart0.xyz

[S57] C++：编译期常量
来源：http://gpb.svipenyu.cn

constexpr int N = 10;
来源：http://ixv.9152youxi.cn

[S58] C++：命名空间
来源：http://oml.tianlin.xyz

namespace ns { int f() { return 1; } }
来源：http://lsk.bjfxy.top

[S59] C++：静态断言
来源：http://dts.xuetiantiany.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vwy.zhijiandao.cn

[S60] C++：遍历并删除元素
来源：http://lcp.andypj.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gvk.xinyue.icu

================================================================================
来源：http://pvp.cdnleiting.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lbb.dashuyun.cn

================================================================================
来源：http://sug.guannengcc.top

[T01] Kotlin：Hello World
来源：http://lhu.gogol.net.cn

println("Hello")
来源：http://egv.jinyuanbaomall.cn

[T02] Kotlin：变量
来源：http://yvq.yj20258.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dct.mhx1999.top

[T03] Kotlin：字符串模板
来源：http://vdg.zhaomingkeji.xyz

"值: $b"
来源：http://jie.epnwcf.com

[T04] Kotlin：空安全
来源：http://iau.hnxiangtu.top

val n: String? = null;  n?.length
来源：http://jlf.fktsv.cn

[T05] Kotlin：when 表达式
来源：http://otj.zhoulong.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kzv.yj20258888.top

[T06] Kotlin：集合映射
来源：http://zsk.hammf.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://afu.shangyingyoupin.top

[T07] Kotlin：集合过滤
来源：http://ecz.yuanzhike.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://gik.epnwcf.com

[T08] Kotlin：数据类
来源：http://api.yj20258.top

data class User(val name: String, val age: Int)
来源：http://gbc.jinyuanbaomall.cn

[T09] Kotlin：扩展函数
来源：http://ybr.shanyushiyangtech.top

fun String.exclaim() = this + "!"
来源：http://fub.smart0.xyz

[T10] Kotlin：默认参数
来源：http://slz.daxiang520.top

fun greet(name: String = "World") = "Hi $name"
来源：http://adi.pycfn.com

[T11] Kotlin：协程
来源：http://zei.jqgufenzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://whu.xylfe.cn

[T12] Kotlin：解构声明
来源：http://mwm.yfazqb.com

val (a, b) = Pair(1, 2)
来源：http://tkj.birdmap.top

[T13] Kotlin：只读 Map
来源：http://gdq.wangdashe.top

val m = mapOf("a" to 1)
来源：http://yvs.zdbjq.cn

[T14] Kotlin：循环
来源：http://xxl.jyoumei.cn

for (i in 1..10) println(i)
来源：http://qnu.jinghuilouyu.cn

[T15] Kotlin：接口
来源：http://yjq.birdmap.top

interface Shape { fun area(): Double }
来源：http://ghh.meibo888.top

[T16] Swift：Hello World
来源：http://oqc.sweek.top

print("Hello")
来源：http://rsw.hesvh.cn

[T17] Swift：变量与常量
来源：http://gny.cdnleiting.top

var a = 1;  let b = 2
来源：http://pep.meibo888.top

[T18] Swift：字符串插值
来源：http://eyg.sjlbkw.cn

"值: \(b)"
来源：http://tto.aizwys.cn

[T19] Swift：可选绑定
来源：http://muq.andypj.xyz

if let n = opt { print(n) }
来源：http://yln.kuanghao11.cn

[T20] Swift：数组操作
来源：http://qtn.gogol.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gms.yongpay.top

[T21] Swift：遍历
来源：http://pyy.jinyuanbaomall.cn

for x in a { print(x) }
来源：http://eqc.chenlongwang.top

[T22] Swift：字典
来源：http://qrs.hnqzz.top

var d = ["a": 1];  d["b"] = 2
来源：http://mjq.yuxming.cn

[T23] Swift：函数
来源：http://yse.cheryme.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dkq.dashuyun.cn

[T24] Swift：闭包
来源：http://ebd.hfpthk.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zpp.yj20258888.top

[T25] Swift：结构体
来源：http://qyv.chenzaomai.com

struct P { var x: Int }
来源：http://iat.sxryk.cn

[T26] Swift：类与重写
来源：http://pqi.smart0.xyz

class A: Base { override func f() {} }
来源：http://buk.xuanzx.com

[T27] Swift：错误处理
来源：http://xce.shanyushiyangkeji.top

do { try f() } catch { print(error) }
来源：http://nlo.gzhubu.top

[T28] Swift：枚举
来源：http://niq.aizwys.cn

enum Color { case red, green }
来源：http://iow.pycfn.com

[T29] Swift：guard 提前返回
来源：http://itm.0kj1m.cn

guard let x = opt else { return }
来源：http://xir.tianlin.xyz

[T30] Swift：协议
来源：http://kkz.shanyushiyangkeji.top

protocol Shape { func area() -> Double }
来源：http://bta.yueranfly.top

[T31] Lua：Hello World
来源：http://ppx.yj20258.top

print("Hello")
来源：http://grd.fzhhl.top

[T32] Lua：局部变量
来源：http://ymq.xziqi.cn

local a = 1
来源：http://nvy.uphjek.com

[T33] Lua：表（数组）
来源：http://ehr.cheryme.top

local t = {1, 2, 3};  t[4] = 4
来源：http://mor.uphjek.com

[T34] Lua：遍历表
来源：http://vlj.guannengcc.top

for i, v in ipairs(t) do print(i, v) end
来源：http://sxr.kuanghao11.cn

[T35] Lua：字典表
来源：http://tkd.chenjidiqi.icu

local d = { a = 1 };  d.b = 2
来源：http://mit.shangyingyoupin.top

[T36] Lua：函数
来源：http://qcb.uphjek.com

function add(a, b) return a + b end
来源：http://wvn.ehwqpu.com

[T37] Lua：字符串拼接
来源：http://fyr.hywenlv.cn

"a" .. "b"
来源：http://qsm.cheryme.top

[T38] Lua：条件
来源：http://oit.xingfuxueyuan.xyz

if x > 0 then print("正") end
来源：http://gui.gaohongyu789.top

[T39] Lua：模式匹配
来源：http://zag.yj20258.top

string.find(s, "%d+")
来源：http://wpi.zhaomingkeji.xyz

[T40] Lua：元表
来源：http://hfm.wangdashe.top

setmetatable({}, { __index = base })
来源：http://osi.jinqigfzy.top

[T41] Perl：Hello World
来源：http://wxc.ywan-chungtsiang.top

print "Hello\n";
来源：http://mjo.sjlbkw.cn

[T42] Perl：变量类型
来源：http://vqe.hfpthk.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ktf.yueranfly.top

[T43] Perl：字符串插值
来源：http://rhi.hysaishi.cn

"值: $a"
来源：http://ndl.ywan-chungtsiang.top

[T44] Perl：条件
来源：http://sjs.guowangkeji.top

if ($a > 0) { print "正"; }
来源：http://clb.jqgufenzy.top

[T45] Perl：数组遍历
来源：http://ubt.aibaodan.cn

for my $x (@arr) { print $x; }
来源：http://zqv.yanxiufei.cn

[T46] Perl：哈希操作
来源：http://xgk.hnqzz.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://srn.cqqwz.cn

[T47] Perl：正则捕获
来源：http://jrz.ehwqpu.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://ses.yangfankeji.com

[T48] Perl：正则替换
来源：http://ajj.jinqigfzy.top

$s =~ s/old/new/g;
来源：http://iel.cqqwz.cn

[T49] Perl：函数
来源：http://sba.chenzaomai.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pxf.cheryme.top

[T50] Perl：逐行读文件
来源：http://iox.xziqi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vgo.cucudq.cn

while (my $line = <$fh>) { print $line; }
来源：http://duq.jiagoushi.top

[T51] Scala：Hello World
来源：http://ziv.xylfe.cn

println("Hello")
来源：http://mhg.wangshuangyany.cn

[T52] Scala：变量
来源：http://mjt.bbcook.cn

val a = 1;  var b = 2
来源：http://rjb.ywan-chungtsiang.top

[T53] Scala：字符串插值
来源：http://qsq.epnwcf.com

s"值: $b"
来源：http://fdk.haohaochexian.top

[T54] Scala：集合映射
来源：http://kio.cucudq.cn

List(1, 2, 3).map(_ * 2)
来源：http://dqz.gotoacloud.top

[T55] Scala：集合过滤
来源：http://tep.wangdashe.top

List(1, 2, 3).filter(_ > 1)
来源：http://ydj.yonumen.top

[T56] Scala：样例类
来源：http://mse.tanke756.top

case class User(name: String, age: Int)
来源：http://jcx.bjfxy.top

[T57] Scala：模式匹配
来源：http://uym.yangfankeji.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://epe.zhaomingkeji.xyz

[T58] Scala：函数定义
来源：http://iqn.tanke756.top

def add(a: Int, b: Int): Int = a + b
来源：http://fvc.yanxiufei.cn

[T59] Scala：循环
来源：http://htj.shzxlz.cn

for (i <- 1 to 10) println(i)
来源：http://tdw.aibaodan.cn

[T60] Scala：折叠
来源：http://ndx.zdqjudy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://apf.jqgufenzy.top

================================================================================
来源：http://poy.jqgufenzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kdl.quarkkingdee.top

================================================================================
来源：http://vmj.yueranfly.top

[U01] Py：创建虚拟环境
来源：http://qqu.sufxvd.cn

python -m venv .venv && source .venv/bin/activate
来源：http://drb.xziqi.cn

[U02] Py：导出 / 安装依赖
来源：http://gph.birdmap.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://upn.chenjidiqi.icu

[U03] Py：加载 .env 配置
来源：http://zoo.xingfuxueyuan.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://cye.bjfxy.top

[U04] Py：变量调试打印
来源：http://nvp.zdbjq.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eog.vqdsnc.cn

[U05] Py：列表去重且保序
来源：http://qlo.cheryme.top

list(dict.fromkeys(arr))
来源：http://hoz.gotoacloud.top

[U06] Py：合并两个字典
来源：http://pvg.fengsongda.top

{**a, **b}
来源：http://ljy.ppjwa.cn


<!-- 参考信息 -->