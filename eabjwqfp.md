代发 wailian999

openssl rand -hex 16
来源：http://irg.xylfe.cn

[R68] 计算文件校验值
来源：http://lvk.jyoumei.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vkn.cdnleiting.top

[R69] 生成随机密码
来源：http://yco.c1oappe.top

head -c 16 /dev/urandom | base64
来源：http://bos.xylfe.cn

[R70] 时间戳与互转
来源：http://ulp.ppjwa.cn

date +%s;  date -d @1700000000
来源：http://ndj.tianlin.xyz

[R71] 日期格式化
来源：http://ult.yanxiufei.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://eba.meibo888.top

[R72] 等待端口就绪
来源：http://udp.ctjpmb.com

until nc -z localhost 3306; do sleep 1; done
来源：http://rem.hysaishi.cn

[R73] 分割大日志
来源：http://sql.fehbvm.com

split -l 1000 big.log part_
来源：http://sbj.gogol.net.cn

[R74] 批量重命名
来源：http://wfd.hcnkem.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fnd.nanxinkj.top

[R75] 导出环境变量
来源：http://ytu.xuetiantiany.cn

export PATH="$HOME/bin:$PATH"
来源：http://hej.shangyingyoupin.top

[R76] 使用临时文件
来源：http://jtm.zhixingplan.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mep.yuxming.cn

[R77] 读取用户输入
来源：http://wzh.cucudq.cn

read -rp "请输入: " ans
来源：http://axv.ivvv.top

[R78] 交互式菜单
来源：http://mvv.jqgfzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://tcm.nanxinkj.top

[R79] 解析命令行选项
来源：http://zaa.cqqwz.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uuo.quarkkingdee.top

[R80] 查看脚本执行耗时
来源：http://wil.yfazqb.com

time ./run.sh
来源：http://vgx.snrcjt.cn

================================================================================
来源：http://ohx.yvedp.cn

S. C / C++ 专题
来源：http://xqr.hongshengwenyu.top

================================================================================
来源：http://ghj.tarul.cn

[S01] C：Hello World
来源：http://oug.xuetiantiany.cn

#include <stdio.h>
来源：http://ugn.ydzc1.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://tay.sxryk.cn

[S02] C：变量与格式化输出
来源：http://avr.yuxming.cn

int a = 10; printf("%d\n", a);
来源：http://htw.shanyushiyangkeji.top

[S03] C：读入整数
来源：http://mtd.ydzc1.top

int x; scanf("%d", &x);
来源：http://qjm.ydjk.org.cn

[S04] C：字符串复制
来源：http://eva.svipenyu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qmx.zdbjq.cn

[S05] C：字符串长度
来源：http://slc.guowangkeji.top

strlen(s)
来源：http://qzg.bjfxy.top

[S06] C：字符串比较
来源：http://kqz.zhiwuduotai.top

strcmp(a, b) == 0
来源：http://fyf.jyoumei.cn

[S07] C：数组遍历求和
来源：http://ubp.aibaodan.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ntu.xuanzx.com

[S08] C：动态内存分配与释放
来源：http://xzq.zdqjudy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ial.guowangkeji.top

[S09] C：结构体定义与初始化
来源：http://ids.fanxiaobao.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lik.yj20258888.top

[S10] C：指针与解引用
来源：http://wnl.fengsongda.top

int *p = &a;  *p = 5;
来源：http://dxo.jiagoushi.top

[S11] C：逐行读文件
来源：http://nve.sufxvd.cn

FILE *f = fopen("a.txt", "r");
来源：http://opm.ywan-chungtsiang.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://lbn.ehwqpu.com

fclose(f);
来源：http://xtr.ydjk.org.cn

[S12] C：写文件
来源：http://meb.wangdashe.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gjr.ctjpmb.com

[S13] C：宏定义
来源：http://zgj.cashguo.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ugn.jqgufenzy.top

[S14] C：枚举
来源：http://dlh.sufxvd.cn

enum Color { RED, GREEN, BLUE };
来源：http://zix.0kj1m.cn

[S15] C：类型转换
来源：http://tsy.gotoacloud.top

(double) a / b
来源：http://nwe.hcnkem.com

[S16] C：位操作置位
来源：http://kej.ppjwa.cn

x |= (1 << 3);
来源：http://qhp.haohaochexian.top

[S17] C：安全拼接字符串
来源：http://tmb.quarkkingdee.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uzw.gaohongyu789.top

[S18] C：命令行参数
来源：http://hdh.smart0.xyz

int main(int argc, char **argv)
来源：http://gwq.quarkkingdee.top

[S19] C：快速排序
来源：http://tbt.shzxlz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jcs.bbcook.cn

[S20] C：二分查找
来源：http://yok.hesvh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sbu.haohaochexian.top

[S21] C：字符类别判断
来源：http://qsw.zhiwuduotai.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wea.epnwcf.com

[S22] C：字符串转数字
来源：http://nyy.fehbvm.com

atoi("42");  strtod("3.14", NULL);
来源：http://oec.jinqigufen.top

[S23] C：随机数
来源：http://kjm.zhoulong.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://ood.c1oappe.top

[S24] C：获取本地时间
来源：http://zio.zdqjudy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dzu.ehwqpu.com

[S25] C：内存拷贝
来源：http://tzs.hnxiangtu.top

memcpy(dst, src, n);
来源：http://beb.zhoulong.xyz

[S26] C：内存清零
来源：http://ygy.shzxlz.cn

memset(a, 0, sizeof a);
来源：http://qna.guowangkeji.top

[S27] C：定义常量
来源：http://nbe.sufxvd.cn

const double PI = 3.14159;
来源：http://icc.sweek.top

[S28] C：静态变量
来源：http://kjr.zhijiandao.cn

static int counter = 0;
来源：http://xkn.bjfxy.top

[S29] C：变参函数
来源：http://qts.yuxming.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kwr.yfazqb.com

[S30] C：头文件保护
来源：http://vqz.fzhhl.top

#ifndef X_H
来源：http://rzr.cqqwz.cn

#define X_H
来源：http://uyc.aizwys.cn

#endif
来源：http://kys.xinyue.icu

[S31] C++：Hello World
来源：http://oox.mhx1999.top

#include <iostream>
来源：http://mgz.redwolf501.top

int main() { std::cout << "Hello\n"; }
来源：http://xrp.sjlbkw.cn

[S32] C++：字符串
来源：http://jlf.chenzaomai.com

std::string s = "hi";  s += "!";
来源：http://eaf.zdqjudy.top

[S33] C++：vector 增删
来源：http://uww.yangfankeji.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bfs.nanxuanxn.top

[S34] C++：遍历 vector
来源：http://dpg.nwbrower.top

for (auto &x : v) { std::cout << x; }
来源：http://fex.316326.xyz

[S35] C++：map
来源：http://kkv.nanxuanxn.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sml.jlsjyb.cn

[S36] C++：unordered_map
来源：http://aek.hesvh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cws.ydzc1.top

[S37] C++：set
来源：http://gkr.shuidangran.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://taf.yuanzhike.top

[S38] C++：排序
来源：http://dyg.smart0.xyz

std::sort(v.begin(), v.end());
来源：http://mqv.fengsongda.top

[S39] C++：自定义比较器排序
来源：http://fny.gogol.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lur.pengpengdd.cyou

[S40] C++：查找元素
来源：http://tkf.jiagoushi.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lai.nwbrower.top

[S41] C++：类与构造函数
来源：http://gcm.gaohongyu789.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rjh.yanxiufei.cn

[S42] C++：继承与虚函数
来源：http://jpm.redwolf501.top

class B : public Base { public: void f() override {} };
来源：http://ypa.yueranfly.top

[S43] C++：智能指针
来源：http://ues.sufxvd.cn

auto p = std::make_unique<int>(5);
来源：http://oet.guowangkeji.top

[S44] C++：引用传参
来源：http://ptt.cheryme.top

void inc(int &x) { ++x; }
来源：http://sbj.snrcjt.cn

[S45] C++：lambda
来源：http://uzf.chenjidiqi.icu

auto add = [](int a, int b) { return a + b; };
来源：http://byg.zhiwuduotai.top

[S46] C++：函数模板
来源：http://ear.tian-w.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://izt.xinyue.icu

[S47] C++：结构化绑定遍历
来源：http://jct.daxiang520.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kva.dianchejie.cn

[S48] C++：逐行读文件
来源：http://uwj.jqgfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://frd.gaohongyu789.top

while (std::getline(in, line)) { }
来源：http://ikm.sjlbkw.cn

[S49] C++：写文件
来源：http://tbh.xinyue.icu

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ylr.316326.xyz

[S50] C++：格式化数字
来源：http://mhn.feifeiyinyue.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zuo.nanxinkj.top

[S51] C++：显式类型转换
来源：http://lrd.havefunace.top

static_cast<double>(a) / b
来源：http://xiq.zhongyouzk.top

[S52] C++：const 与 noexcept
来源：http://ibj.yongpay.top

int size() const noexcept { return n_; }
来源：http://oqe.c1oappe.top

[S53] C++：移动语义
来源：http://gee.xuanzx.com

std::vector<int> w = std::move(v);
来源：http://nyq.redwolf501.top

[S54] C++：异常处理
来源：http://gkr.hysaishi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ibd.zdbjq.cn

[S55] C++：结构化绑定
来源：http://fxo.gzhubu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://xkj.redwolf501.top

[S56] C++：optional
来源：http://shg.c1oappe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lsv.bbcook.cn

[S57] C++：编译期常量
来源：http://vxy.yuanzhike.top

constexpr int N = 10;
来源：http://iuz.zhiwuduotai.top

[S58] C++：命名空间
来源：http://oce.nanxuanxn.top

namespace ns { int f() { return 1; } }
来源：http://ltp.bbcook.cn

[S59] C++：静态断言
来源：http://srz.andypj.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mka.tianlin.xyz

[S60] C++：遍历并删除元素
来源：http://qmk.zhixingplan.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fil.snrcjt.cn

================================================================================
来源：http://zvp.c1oappe.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vam.redwolf501.top

================================================================================
来源：http://mpk.sufxvd.cn

[T01] Kotlin：Hello World
来源：http://pzr.feifeiyinyue.top

println("Hello")
来源：http://uxo.shanyushiyangtech.top

[T02] Kotlin：变量
来源：http://vxs.tarul.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jcb.jinghuilouyu.cn

[T03] Kotlin：字符串模板
来源：http://try.jianghu66.top

"值: $b"
来源：http://omm.daria6918.cn

[T04] Kotlin：空安全
来源：http://ltf.shangyingyoupin.top

val n: String? = null;  n?.length
来源：http://blj.yj20258888.top

[T05] Kotlin：when 表达式
来源：http://wpl.gzhubu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hft.zdqjudy.top

[T06] Kotlin：集合映射
来源：http://bja.ydzc1.top

listOf(1, 2, 3).map { it * 2 }
来源：http://poo.birdmap.top

[T07] Kotlin：集合过滤
来源：http://olw.gogol.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qcu.fanxiaobao.xyz

[T08] Kotlin：数据类
来源：http://wpk.yongpay.top

data class User(val name: String, val age: Int)
来源：http://aes.yj20258888.top

[T09] Kotlin：扩展函数
来源：http://krt.yongpay.top

fun String.exclaim() = this + "!"
来源：http://lxd.pengpengdd.cyou

[T10] Kotlin：默认参数
来源：http://jlj.hcnkem.com

fun greet(name: String = "World") = "Hi $name"
来源：http://kxn.9152youxi.cn

[T11] Kotlin：协程
来源：http://mbr.daria6918.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dyo.hfpthk.cn

[T12] Kotlin：解构声明
来源：http://dwp.yj202588.top

val (a, b) = Pair(1, 2)
来源：http://tjy.hfpthk.cn

[T13] Kotlin：只读 Map
来源：http://iii.gzhubu.top

val m = mapOf("a" to 1)
来源：http://tvs.yj202588.top

[T14] Kotlin：循环
来源：http://zql.chenzaomai.com

for (i in 1..10) println(i)
来源：http://wlh.shanyushiyangtech.top

[T15] Kotlin：接口
来源：http://bqd.feifeiyinyue.top

interface Shape { fun area(): Double }
来源：http://soh.pengpengdd.cyou

[T16] Swift：Hello World
来源：http://rjq.tianlin.xyz

print("Hello")
来源：http://xfy.jinqigfzy.top

[T17] Swift：变量与常量
来源：http://viq.aizwys.cn

var a = 1;  let b = 2
来源：http://rqu.0kj1m.cn

[T18] Swift：字符串插值
来源：http://its.316326.xyz

"值: \(b)"
来源：http://fzm.yvedp.cn

[T19] Swift：可选绑定
来源：http://mko.sysykeji.top

if let n = opt { print(n) }
来源：http://pxw.aibaodan.cn

[T20] Swift：数组操作
来源：http://jya.hongshengwenyu.top

var a = [1, 2, 3];  a.append(4)
来源：http://ngw.fktsv.cn

[T21] Swift：遍历
来源：http://qdq.xingfuxueyuan.xyz

for x in a { print(x) }
来源：http://iqt.yfazqb.com

[T22] Swift：字典
来源：http://whb.vehdjk.com

var d = ["a": 1];  d["b"] = 2
来源：http://gic.ywan-chungtsiang.top

[T23] Swift：函数
来源：http://bhl.hongshengwenyu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rsd.ybcxt.top

[T24] Swift：闭包
来源：http://vci.cdnleiting.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ilo.vehdjk.com

[T25] Swift：结构体
来源：http://zbr.cqqwz.cn

struct P { var x: Int }
来源：http://vqx.yj20258.top

[T26] Swift：类与重写
来源：http://bor.9152youxi.cn

class A: Base { override func f() {} }
来源：http://cnk.daxiang520.top

[T27] Swift：错误处理
来源：http://vaf.vqdsnc.cn

do { try f() } catch { print(error) }
来源：http://yig.cdnleiting.top

[T28] Swift：枚举
来源：http://bfj.guowangkeji.top

enum Color { case red, green }
来源：http://ham.shzxlz.cn

[T29] Swift：guard 提前返回
来源：http://phz.ctjpmb.com

guard let x = opt else { return }
来源：http://tcq.hnqzz.top

[T30] Swift：协议
来源：http://ndz.wangdashe.top

protocol Shape { func area() -> Double }
来源：http://bbq.chenjidiqi.icu

[T31] Lua：Hello World
来源：http://pbd.jinqigufen.top

print("Hello")
来源：http://cbi.hfpthk.cn

[T32] Lua：局部变量
来源：http://rix.svipenyu.cn

local a = 1
来源：http://tqe.redwolf501.top

[T33] Lua：表（数组）
来源：http://gir.quarkkingdee.top

local t = {1, 2, 3};  t[4] = 4
来源：http://jtg.yj20258.top

[T34] Lua：遍历表
来源：http://sug.ehwqpu.com

for i, v in ipairs(t) do print(i, v) end
来源：http://wne.haohaochexian.top

[T35] Lua：字典表
来源：http://big.sxryk.cn

local d = { a = 1 };  d.b = 2
来源：http://sbl.nanxuanxn.top

[T36] Lua：函数
来源：http://drm.xylfe.cn

function add(a, b) return a + b end
来源：http://lxa.yonumen.top

[T37] Lua：字符串拼接
来源：http://xhv.nwbrower.top

"a" .. "b"
来源：http://cli.ehwqpu.com

[T38] Lua：条件
来源：http://gip.yongpay.top

if x > 0 then print("正") end
来源：http://xof.fehbvm.com

[T39] Lua：模式匹配
来源：http://qlu.gotoacloud.top

string.find(s, "%d+")
来源：http://auk.hongshengwenyu.top

[T40] Lua：元表
来源：http://bti.cashguo.top

setmetatable({}, { __index = base })
来源：http://yfy.xuanzx.com

[T41] Perl：Hello World
来源：http://hwo.zhongyouzk.top

print "Hello\n";
来源：http://ouv.haohaochexian.top

[T42] Perl：变量类型
来源：http://nfh.ywan-chungtsiang.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kgp.vehdjk.com

[T43] Perl：字符串插值
来源：http://lfu.guannengcc.top

"值: $a"
来源：http://xmv.316326.xyz

[T44] Perl：条件
来源：http://xfn.jianghu66.top

if ($a > 0) { print "正"; }
来源：http://qep.cdnleiting.top

[T45] Perl：数组遍历
来源：http://nkf.guannengcc.top

for my $x (@arr) { print $x; }
来源：http://opb.jinghuilouyu.cn

[T46] Perl：哈希操作
来源：http://foc.yj20258.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uuu.fanxiaobao.xyz

[T47] Perl：正则捕获
来源：http://pdj.cqqwz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://upv.dashuyun.cn

[T48] Perl：正则替换
来源：http://cev.sysykeji.top

$s =~ s/old/new/g;
来源：http://fvw.jqgufenzy.top

[T49] Perl：函数
来源：http://nun.sufxvd.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nrk.wangshuangyany.cn

[T50] Perl：逐行读文件
来源：http://qbc.gogol.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mwz.cqqwz.cn

while (my $line = <$fh>) { print $line; }
来源：http://aov.yj20258888.top

[T51] Scala：Hello World
来源：http://ydq.hysaishi.cn

println("Hello")
来源：http://vpq.epnwcf.com

[T52] Scala：变量
来源：http://cqj.xuanzx.com

val a = 1;  var b = 2
来源：http://qpb.feifeiyinyue.top

[T53] Scala：字符串插值
来源：http://tgb.tianlin.xyz

s"值: $b"
来源：http://ukx.xylfe.cn

[T54] Scala：集合映射
来源：http://tuc.kuanghao11.cn

List(1, 2, 3).map(_ * 2)
来源：http://alc.smart0.xyz

[T55] Scala：集合过滤
来源：http://kfk.yangfankeji.com

List(1, 2, 3).filter(_ > 1)
来源：http://ont.yj20258.top

[T56] Scala：样例类
来源：http://lkb.meibo888.top

case class User(name: String, age: Int)
来源：http://gdv.yanxiufei.cn

[T57] Scala：模式匹配
来源：http://zee.dashuyun.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hlp.xuanzx.com

[T58] Scala：函数定义
来源：http://pqc.zhiwuduotai.top

def add(a: Int, b: Int): Int = a + b
来源：http://oid.vqdsnc.cn

[T59] Scala：循环
来源：http://ned.zdqjudy.top

for (i <- 1 to 10) println(i)
来源：http://lzj.hywenlv.cn

[T60] Scala：折叠
来源：http://ewd.cheryme.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ytq.daria6918.cn

================================================================================
来源：http://lij.tarul.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yvh.havefunace.top

================================================================================
来源：http://dih.yongpay.top

[U01] Py：创建虚拟环境
来源：http://fcy.gaohongyu789.top

python -m venv .venv && source .venv/bin/activate
来源：http://kmr.yuanzhike.top

[U02] Py：导出 / 安装依赖
来源：http://dth.cdnleiting.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cpq.xuetiantiany.cn

[U03] Py：加载 .env 配置
来源：http://esd.zhijiandao.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rsu.tian-w.cn

[U04] Py：变量调试打印
来源：http://vyv.yvedp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dmg.yonumen.top

[U05] Py：列表去重且保序
来源：http://lfx.ybcxt.top

list(dict.fromkeys(arr))
来源：http://mzc.daxiang520.top

[U06] Py：合并两个字典
来源：http://ugy.316326.xyz

{**a, **b}
来源：http://ghy.kuanghao11.cn

[U07] Py：反转字典键值
来源：http://aah.hnxiangtu.top

{v: k for k, v in d.items()}
来源：http://rvf.hywenlv.cn

[U08] Py：展平二维列表
来源：http://akp.jinyuanbaomall.cn

[y for x in nested for y in x]
来源：http://lhx.xuetiantiany.cn


<!-- 参考信息 -->