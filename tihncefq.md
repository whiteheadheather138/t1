代发 wailian999

free -h;  ps aux | grep nginx
来源：http://mck.daria6918.cn

[R64] 结束进程
来源：http://bma.guannengcc.top

kill -9 $(pgrep -f app.py)
来源：http://sux.yuanzhike.top

[R65] 查看端口占用
来源：http://jrb.hnxiangtu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jkh.tianlin.xyz

[R66] 定时任务
来源：http://yzz.hysaishi.cn

crontab -e;  crontab -l
来源：http://oxr.9152youxi.cn

[R67] 生成随机十六进制串
来源：http://dfa.zhongyouzk.top

openssl rand -hex 16
来源：http://tej.tarul.cn

[R68] 计算文件校验值
来源：http://szl.snrcjt.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wmi.havefunace.top

[R69] 生成随机密码
来源：http://zao.316326.xyz

head -c 16 /dev/urandom | base64
来源：http://xpc.cucudq.cn

[R70] 时间戳与互转
来源：http://xvl.yuanzhike.top

date +%s;  date -d @1700000000
来源：http://pnv.jyoumei.cn

[R71] 日期格式化
来源：http://szc.epnwcf.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://oas.shuidangran.top

[R72] 等待端口就绪
来源：http://sdv.tianlin.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://dtx.mhx1999.top

[R73] 分割大日志
来源：http://hgr.jinyuanbaomall.cn

split -l 1000 big.log part_
来源：http://izy.yj202588.top

[R74] 批量重命名
来源：http://rjw.yvedp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://joz.xingfuxueyuan.xyz

[R75] 导出环境变量
来源：http://vie.zhongyouzk.top

export PATH="$HOME/bin:$PATH"
来源：http://unq.yuanzhike.top

[R76] 使用临时文件
来源：http://qdj.havefunace.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lpg.birdmap.top

[R77] 读取用户输入
来源：http://cpz.nanxuanxn.top

read -rp "请输入: " ans
来源：http://lrz.zycfv.cn

[R78] 交互式菜单
来源：http://oui.jyoumei.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://iib.xuanzx.com

[R79] 解析命令行选项
来源：http://tsa.sufxvd.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jlh.zhiwuduotai.top

[R80] 查看脚本执行耗时
来源：http://xas.xuanzx.com

time ./run.sh
来源：http://pvq.yuanzhike.top

================================================================================
来源：http://zzi.hnxiangtu.top

S. C / C++ 专题
来源：http://oun.yvedp.cn

================================================================================
来源：http://cua.nanxuanxn.top

[S01] C：Hello World
来源：http://bsv.jqgfzy.top

#include <stdio.h>
来源：http://nkd.xingfuxueyuan.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://yco.jqgufenzy.top

[S02] C：变量与格式化输出
来源：http://ksz.hammf.cn

int a = 10; printf("%d\n", a);
来源：http://zxu.ehwqpu.com

[S03] C：读入整数
来源：http://kkv.hfpthk.cn

int x; scanf("%d", &x);
来源：http://tqt.fengsongda.top

[S04] C：字符串复制
来源：http://xue.guowangkeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://uvq.c1oappe.top

[S05] C：字符串长度
来源：http://xvs.gotoacloud.top

strlen(s)
来源：http://jfa.uphjek.com

[S06] C：字符串比较
来源：http://ndk.daria6918.cn

strcmp(a, b) == 0
来源：http://zkr.hcnkem.com

[S07] C：数组遍历求和
来源：http://uew.fktsv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xxo.hywenlv.cn

[S08] C：动态内存分配与释放
来源：http://vsc.cashguo.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pey.xylfe.cn

[S09] C：结构体定义与初始化
来源：http://cuk.shzxlz.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fvt.xinyue.icu

[S10] C：指针与解引用
来源：http://vls.hcnkem.com

int *p = &a;  *p = 5;
来源：http://mot.zhaomingkeji.xyz

[S11] C：逐行读文件
来源：http://lcu.iojbl.cn

FILE *f = fopen("a.txt", "r");
来源：http://sjf.hcnkem.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://spx.ppjwa.cn

fclose(f);
来源：http://fwk.redwolf501.top

[S12] C：写文件
来源：http://isg.ydjk.org.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zki.guowangkeji.top

[S13] C：宏定义
来源：http://qet.shanyushiyangkeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mmf.wangshuangyany.cn

[S14] C：枚举
来源：http://vgq.vehdjk.com

enum Color { RED, GREEN, BLUE };
来源：http://rcv.zhixingplan.top

[S15] C：类型转换
来源：http://wrc.bjfxy.top

(double) a / b
来源：http://gib.zhengqikj.top

[S16] C：位操作置位
来源：http://jva.fehbvm.com

x |= (1 << 3);
来源：http://epj.meibo888.top

[S17] C：安全拼接字符串
来源：http://jff.sysykeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://eby.vehdjk.com

[S18] C：命令行参数
来源：http://ydv.yj20258888.top

int main(int argc, char **argv)
来源：http://fbb.guowangkeji.top

[S19] C：快速排序
来源：http://alo.pengpengdd.cyou

qsort(a, n, sizeof(int), cmp);
来源：http://yvg.jinqigufen.top

[S20] C：二分查找
来源：http://edm.shanyushiyangkeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ady.yj202588.top

[S21] C：字符类别判断
来源：http://dia.ivvv.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wrn.mhx1999.top

[S22] C：字符串转数字
来源：http://wig.0kj1m.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qsm.cdnleiting.top

[S23] C：随机数
来源：http://gzt.uphjek.com

srand(time(NULL));  int r = rand() % 100;
来源：http://oax.andypj.xyz

[S24] C：获取本地时间
来源：http://fhd.zhiwuduotai.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pgb.yvedp.cn

[S25] C：内存拷贝
来源：http://jex.52xcode.cn

memcpy(dst, src, n);
来源：http://xsf.bbcook.cn

[S26] C：内存清零
来源：http://huw.cdnleiting.top

memset(a, 0, sizeof a);
来源：http://tkk.hcnkem.com

[S27] C：定义常量
来源：http://yvb.fehbvm.com

const double PI = 3.14159;
来源：http://squ.tianlin.xyz

[S28] C：静态变量
来源：http://vlv.daxiang520.top

static int counter = 0;
来源：http://dao.sxryk.cn

[S29] C：变参函数
来源：http://mba.svipenyu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uag.smart0.xyz

[S30] C：头文件保护
来源：http://naz.xingfuxueyuan.xyz

#ifndef X_H
来源：http://rnn.zhiwuduotai.top

#define X_H
来源：http://mtt.ydzc1.top

#endif
来源：http://tct.xinyue.icu

[S31] C++：Hello World
来源：http://cuc.tianlin.xyz

#include <iostream>
来源：http://eht.jlsjyb.cn

int main() { std::cout << "Hello\n"; }
来源：http://uhm.guowangkeji.top

[S32] C++：字符串
来源：http://qlu.bjfxy.top

std::string s = "hi";  s += "!";
来源：http://bur.xingfuxueyuan.xyz

[S33] C++：vector 增删
来源：http://pzs.meibo888.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://unj.fehbvm.com

[S34] C++：遍历 vector
来源：http://unw.ivvv.top

for (auto &x : v) { std::cout << x; }
来源：http://qvw.epnwcf.com

[S35] C++：map
来源：http://ujf.316326.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://slt.smart0.xyz

[S36] C++：unordered_map
来源：http://gij.uphjek.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sey.jinqigfzy.top

[S37] C++：set
来源：http://eux.bbcook.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://scy.meibo888.top

[S38] C++：排序
来源：http://pyy.yj202588.top

std::sort(v.begin(), v.end());
来源：http://yys.ctjpmb.com

[S39] C++：自定义比较器排序
来源：http://fjf.havefunace.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rxt.cqqwz.cn

[S40] C++：查找元素
来源：http://wgi.meibo888.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eiz.hongshengwenyu.top

[S41] C++：类与构造函数
来源：http://nxq.hesvh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://haf.jinqigfzy.top

[S42] C++：继承与虚函数
来源：http://hoh.pycfn.com

class B : public Base { public: void f() override {} };
来源：http://nti.yvedp.cn

[S43] C++：智能指针
来源：http://msd.feifeiyinyue.top

auto p = std::make_unique<int>(5);
来源：http://wmv.0kj1m.cn

[S44] C++：引用传参
来源：http://qzo.shzxlz.cn

void inc(int &x) { ++x; }
来源：http://qbt.xingfuxueyuan.xyz

[S45] C++：lambda
来源：http://yxq.dashuyun.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ydi.vehdjk.com

[S46] C++：函数模板
来源：http://xzo.snrcjt.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xsa.52xcode.cn

[S47] C++：结构化绑定遍历
来源：http://kjn.jyoumei.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lva.daxiang520.top

[S48] C++：逐行读文件
来源：http://jsh.sufxvd.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qmi.dianchejie.cn

while (std::getline(in, line)) { }
来源：http://tqv.ctjpmb.com

[S49] C++：写文件
来源：http://jut.nanxuanxn.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mlk.feifeiyinyue.top

[S50] C++：格式化数字
来源：http://elz.ppjwa.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yne.fehbvm.com

[S51] C++：显式类型转换
来源：http://rrv.pycfn.com

static_cast<double>(a) / b
来源：http://cdh.sjlbkw.cn

[S52] C++：const 与 noexcept
来源：http://yvw.c1oappe.top

int size() const noexcept { return n_; }
来源：http://cyi.aibaodan.cn

[S53] C++：移动语义
来源：http://zhp.shuidangran.top

std::vector<int> w = std::move(v);
来源：http://fvy.andypj.xyz

[S54] C++：异常处理
来源：http://gfj.316326.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rkq.yvedp.cn

[S55] C++：结构化绑定
来源：http://hyd.snrcjt.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mpr.hcnkem.com

[S56] C++：optional
来源：http://pqv.shuidangran.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hpa.zdbjq.cn

[S57] C++：编译期常量
来源：http://vcm.daria6918.cn

constexpr int N = 10;
来源：http://ygg.guannengcc.top

[S58] C++：命名空间
来源：http://heu.fehbvm.com

namespace ns { int f() { return 1; } }
来源：http://ooi.yj202588.top

[S59] C++：静态断言
来源：http://vrj.yueranfly.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://our.guowangkeji.top

[S60] C++：遍历并删除元素
来源：http://klr.yonumen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eql.zhaomingkeji.xyz

================================================================================
来源：http://igf.kuanghao11.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mne.daxiang520.top

================================================================================
来源：http://xbv.zdqjudy.top

[T01] Kotlin：Hello World
来源：http://heh.gaohongyu789.top

println("Hello")
来源：http://dgd.vehdjk.com

[T02] Kotlin：变量
来源：http://laq.quarkkingdee.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yqg.gaohongyu789.top

[T03] Kotlin：字符串模板
来源：http://mcy.ybcxt.top

"值: $b"
来源：http://etq.zhixingplan.top

[T04] Kotlin：空安全
来源：http://byv.pengpengdd.cyou

val n: String? = null;  n?.length
来源：http://wla.yangfankeji.com

[T05] Kotlin：when 表达式
来源：http://oxp.bbcook.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pun.jlsjyb.cn

[T06] Kotlin：集合映射
来源：http://sxx.feifeiyinyue.top

listOf(1, 2, 3).map { it * 2 }
来源：http://cnx.epnwcf.com

[T07] Kotlin：集合过滤
来源：http://pph.redwolf501.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://wlp.ydjk.org.cn

[T08] Kotlin：数据类
来源：http://ant.yueranfly.top

data class User(val name: String, val age: Int)
来源：http://aeo.chenjidiqi.icu

[T09] Kotlin：扩展函数
来源：http://gzm.havefunace.top

fun String.exclaim() = this + "!"
来源：http://jjd.yfazqb.com

[T10] Kotlin：默认参数
来源：http://jcc.tarul.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pfv.fengsongda.top

[T11] Kotlin：协程
来源：http://dzu.aibaodan.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nns.hywenlv.cn

[T12] Kotlin：解构声明
来源：http://ftd.yongpay.top

val (a, b) = Pair(1, 2)
来源：http://alk.hywenlv.cn

[T13] Kotlin：只读 Map
来源：http://vvq.chenzaomai.com

val m = mapOf("a" to 1)
来源：http://jyn.gotoacloud.top

[T14] Kotlin：循环
来源：http://jhk.chenjidiqi.icu

for (i in 1..10) println(i)
来源：http://txt.yj202588.top

[T15] Kotlin：接口
来源：http://boh.xingfuxueyuan.xyz

interface Shape { fun area(): Double }
来源：http://rfa.guannengcc.top

[T16] Swift：Hello World
来源：http://qgx.ywan-chungtsiang.top

print("Hello")
来源：http://nfv.wangdashe.top

[T17] Swift：变量与常量
来源：http://kws.guannengcc.top

var a = 1;  let b = 2
来源：http://zqd.meibo888.top

[T18] Swift：字符串插值
来源：http://xkg.jqgfzy.top

"值: \(b)"
来源：http://jzw.yongpay.top

[T19] Swift：可选绑定
来源：http://zbw.svipenyu.cn

if let n = opt { print(n) }
来源：http://dqf.c1oappe.top

[T20] Swift：数组操作
来源：http://meg.andypj.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://gzq.yueranfly.top

[T21] Swift：遍历
来源：http://cln.chenzaomai.com

for x in a { print(x) }
来源：http://myn.jinghuilouyu.cn

[T22] Swift：字典
来源：http://utg.daxiang520.top

var d = ["a": 1];  d["b"] = 2
来源：http://dhu.dianchejie.cn

[T23] Swift：函数
来源：http://jqf.jqgfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sof.chenzaomai.com

[T24] Swift：闭包
来源：http://dev.gaohongyu789.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://tdx.yueranfly.top

[T25] Swift：结构体
来源：http://els.ppjwa.cn

struct P { var x: Int }
来源：http://ypx.0kj1m.cn

[T26] Swift：类与重写
来源：http://qnx.sysykeji.top

class A: Base { override func f() {} }
来源：http://xan.jinqigufen.top

[T27] Swift：错误处理
来源：http://etb.xuanzx.com

do { try f() } catch { print(error) }
来源：http://kuy.daria6918.cn

[T28] Swift：枚举
来源：http://fvk.shangyingyoupin.top

enum Color { case red, green }
来源：http://dlr.jinyuanbaomall.cn

[T29] Swift：guard 提前返回
来源：http://xkw.zycfv.cn

guard let x = opt else { return }
来源：http://rub.jlsjyb.cn

[T30] Swift：协议
来源：http://arw.ppjwa.cn

protocol Shape { func area() -> Double }
来源：http://vij.smart0.xyz

[T31] Lua：Hello World
来源：http://qol.bbcook.cn

print("Hello")
来源：http://ooo.vehdjk.com

[T32] Lua：局部变量
来源：http://ueu.jqgfzy.top

local a = 1
来源：http://kns.ydjk.org.cn

[T33] Lua：表（数组）
来源：http://xvk.c1oappe.top

local t = {1, 2, 3};  t[4] = 4
来源：http://cpg.vqdsnc.cn

[T34] Lua：遍历表
来源：http://drl.wangdashe.top

for i, v in ipairs(t) do print(i, v) end
来源：http://cph.jiagoushi.top

[T35] Lua：字典表
来源：http://nvy.ydzc1.top

local d = { a = 1 };  d.b = 2
来源：http://fuv.wangdashe.top

[T36] Lua：函数
来源：http://hri.cashguo.top

function add(a, b) return a + b end
来源：http://zvo.daria6918.cn

[T37] Lua：字符串拼接
来源：http://spz.zdbjq.cn

"a" .. "b"
来源：http://kmk.9152youxi.cn

[T38] Lua：条件
来源：http://dut.fehbvm.com

if x > 0 then print("正") end
来源：http://dny.zhiwuduotai.top

[T39] Lua：模式匹配
来源：http://djf.sxryk.cn

string.find(s, "%d+")
来源：http://csn.sweek.top

[T40] Lua：元表
来源：http://yib.fengsongda.top

setmetatable({}, { __index = base })
来源：http://whm.cheryme.top

[T41] Perl：Hello World
来源：http://idx.svipenyu.cn

print "Hello\n";
来源：http://chy.zdqjudy.top

[T42] Perl：变量类型
来源：http://cqf.yj20258.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ecr.jinyuanbaomall.cn

[T43] Perl：字符串插值
来源：http://stl.jianghu66.top

"值: $a"
来源：http://wac.aibaodan.cn

[T44] Perl：条件
来源：http://idj.cheryme.top

if ($a > 0) { print "正"; }
来源：http://uqo.vehdjk.com

[T45] Perl：数组遍历
来源：http://pcz.jinqigfzy.top

for my $x (@arr) { print $x; }
来源：http://wpo.jinqigfzy.top

[T46] Perl：哈希操作
来源：http://ibe.jyoumei.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pbf.yongpay.top

[T47] Perl：正则捕获
来源：http://ksf.shzxlz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rim.fanxiaobao.xyz

[T48] Perl：正则替换
来源：http://bkz.jinqigufen.top

$s =~ s/old/new/g;
来源：http://hxf.316326.xyz

[T49] Perl：函数
来源：http://rrt.yonumen.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ggv.xingfuxueyuan.xyz

[T50] Perl：逐行读文件
来源：http://djh.gogol.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wqw.zycfv.cn

while (my $line = <$fh>) { print $line; }
来源：http://xek.jqgufenzy.top

[T51] Scala：Hello World
来源：http://sgv.c1oappe.top

println("Hello")
来源：http://rbg.svipenyu.cn

[T52] Scala：变量
来源：http://wxi.nwbrower.top

val a = 1;  var b = 2
来源：http://kan.yangfankeji.com

[T53] Scala：字符串插值
来源：http://vrh.tianlin.xyz

s"值: $b"
来源：http://mnp.cashguo.top

[T54] Scala：集合映射
来源：http://mon.ctjpmb.com

List(1, 2, 3).map(_ * 2)
来源：http://fvg.ppjwa.cn

[T55] Scala：集合过滤
来源：http://osm.vehdjk.com

List(1, 2, 3).filter(_ > 1)
来源：http://zsa.xingfuxueyuan.xyz

[T56] Scala：样例类
来源：http://akk.guannengcc.top

case class User(name: String, age: Int)
来源：http://vdr.ppjwa.cn

[T57] Scala：模式匹配
来源：http://zlk.gzhubu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://kye.xylfe.cn

[T58] Scala：函数定义
来源：http://jwl.ehwqpu.com

def add(a: Int, b: Int): Int = a + b
来源：http://foe.gotoacloud.top

[T59] Scala：循环
来源：http://uba.sufxvd.cn

for (i <- 1 to 10) println(i)
来源：http://dhw.shuidangran.top

[T60] Scala：折叠
来源：http://bza.zdbjq.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fdy.vehdjk.com

================================================================================
来源：http://bpl.bjfxy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://osy.aizwys.cn

================================================================================
来源：http://euf.jinghuilouyu.cn

[U01] Py：创建虚拟环境
来源：http://oko.shangyingyoupin.top

python -m venv .venv && source .venv/bin/activate
来源：http://lpd.sxryk.cn

[U02] Py：导出 / 安装依赖
来源：http://frh.zhoulong.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ztq.jinyuanbaomall.cn

[U03] Py：加载 .env 配置
来源：http://udb.xinyue.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://gew.hammf.cn

[U04] Py：变量调试打印
来源：http://prd.pengpengdd.cyou

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wkz.hesvh.cn


<!-- 参考信息 -->