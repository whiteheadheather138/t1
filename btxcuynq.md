代发 wailian999

df -h;  du -sh *
来源：http://rxf.shanyushiyangtech.top

[R62] 找最占空间的文件
来源：http://kuz.guowangkeji.top

du -ah . | sort -rh | head -10
来源：http://oyk.fktsv.cn

[R63] 内存与进程
来源：http://odx.sysykeji.top

free -h;  ps aux | grep nginx
来源：http://ddw.andypj.xyz

[R64] 结束进程
来源：http://gnf.316326.xyz

kill -9 $(pgrep -f app.py)
来源：http://hph.bjfxy.top

[R65] 查看端口占用
来源：http://jrf.yanxiufei.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://myo.hammf.cn

[R66] 定时任务
来源：http://nam.jinghuilouyu.cn

crontab -e;  crontab -l
来源：http://fpu.zhaomingkeji.xyz

[R67] 生成随机十六进制串
来源：http://pql.hfpthk.cn

openssl rand -hex 16
来源：http://nrg.ppjwa.cn

[R68] 计算文件校验值
来源：http://uda.jqgfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://icc.andypj.xyz

[R69] 生成随机密码
来源：http://ubz.ppjwa.cn

head -c 16 /dev/urandom | base64
来源：http://lop.bbcook.cn

[R70] 时间戳与互转
来源：http://fdi.shanyushiyangtech.top

date +%s;  date -d @1700000000
来源：http://wth.xuetiantiany.cn

[R71] 日期格式化
来源：http://ldu.meibo888.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xsk.jqgfzy.top

[R72] 等待端口就绪
来源：http://jyu.bbcook.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://atw.hammf.cn

[R73] 分割大日志
来源：http://xen.shuidangran.top

split -l 1000 big.log part_
来源：http://hjm.tarul.cn

[R74] 批量重命名
来源：http://gsm.yangfankeji.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://prr.zhongyouzk.top

[R75] 导出环境变量
来源：http://jno.shzxlz.cn

export PATH="$HOME/bin:$PATH"
来源：http://gcz.feifeiyinyue.top

[R76] 使用临时文件
来源：http://oly.jyoumei.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xzr.tianlin.xyz

[R77] 读取用户输入
来源：http://tui.aibaodan.cn

read -rp "请输入: " ans
来源：http://eza.pengpengdd.cyou

[R78] 交互式菜单
来源：http://lwm.sjlbkw.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lqf.hammf.cn

[R79] 解析命令行选项
来源：http://rsy.shuidangran.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tir.shanyushiyangkeji.top

[R80] 查看脚本执行耗时
来源：http://vlm.ppjwa.cn

time ./run.sh
来源：http://vsb.hnqzz.top

================================================================================
来源：http://rsd.chenzaomai.com

S. C / C++ 专题
来源：http://auq.tian-w.cn

================================================================================
来源：http://fhf.quarkkingdee.top

[S01] C：Hello World
来源：http://ubt.hammf.cn

#include <stdio.h>
来源：http://dyt.yuxming.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://aup.xingfuxueyuan.xyz

[S02] C：变量与格式化输出
来源：http://ibw.zycfv.cn

int a = 10; printf("%d\n", a);
来源：http://hwr.hywenlv.cn

[S03] C：读入整数
来源：http://lnz.zdqjudy.top

int x; scanf("%d", &x);
来源：http://xsz.fehbvm.com

[S04] C：字符串复制
来源：http://ttp.hnqzz.top

char dst[32]; strcpy(dst, "hi");
来源：http://kzs.tianlin.xyz

[S05] C：字符串长度
来源：http://wiy.vehdjk.com

strlen(s)
来源：http://loo.mhx1999.top

[S06] C：字符串比较
来源：http://pgn.ivvv.top

strcmp(a, b) == 0
来源：http://uhh.tanke756.top

[S07] C：数组遍历求和
来源：http://ynf.birdmap.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dve.zhongyouzk.top

[S08] C：动态内存分配与释放
来源：http://oey.hywenlv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cng.pycfn.com

[S09] C：结构体定义与初始化
来源：http://tgc.jqgufenzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://obr.nwbrower.top

[S10] C：指针与解引用
来源：http://ezs.jianghu66.top

int *p = &a;  *p = 5;
来源：http://vro.xuetiantiany.cn

[S11] C：逐行读文件
来源：http://pzl.sufxvd.cn

FILE *f = fopen("a.txt", "r");
来源：http://avg.yuxming.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rwi.mhx1999.top

fclose(f);
来源：http://qdb.shanyushiyangkeji.top

[S12] C：写文件
来源：http://all.nwbrower.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uxv.shanyushiyangtech.top

[S13] C：宏定义
来源：http://sjc.zdbjq.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cyo.fzhhl.top

[S14] C：枚举
来源：http://qmv.hnqzz.top

enum Color { RED, GREEN, BLUE };
来源：http://eiy.gaohongyu789.top

[S15] C：类型转换
来源：http://kgj.aibaodan.cn

(double) a / b
来源：http://csu.chenzaomai.com

[S16] C：位操作置位
来源：http://lgr.gaohongyu789.top

x |= (1 << 3);
来源：http://iqh.vqdsnc.cn

[S17] C：安全拼接字符串
来源：http://hxw.ydzc1.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tvr.fehbvm.com

[S18] C：命令行参数
来源：http://pwb.gzhubu.top

int main(int argc, char **argv)
来源：http://ozb.zhixingplan.top

[S19] C：快速排序
来源：http://rre.uphjek.com

qsort(a, n, sizeof(int), cmp);
来源：http://yll.zhengqikj.top

[S20] C：二分查找
来源：http://fut.nwbrower.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ylh.jinqigufen.top

[S21] C：字符类别判断
来源：http://xmp.andypj.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mqd.zhengqikj.top

[S22] C：字符串转数字
来源：http://wjn.ivvv.top

atoi("42");  strtod("3.14", NULL);
来源：http://hfp.yvedp.cn

[S23] C：随机数
来源：http://ntp.gaohongyu789.top

srand(time(NULL));  int r = rand() % 100;
来源：http://pka.hnqzz.top

[S24] C：获取本地时间
来源：http://mjz.smart0.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yqa.xziqi.cn

[S25] C：内存拷贝
来源：http://xio.yj20258888.top

memcpy(dst, src, n);
来源：http://pgv.gzhubu.top

[S26] C：内存清零
来源：http://wnk.9152youxi.cn

memset(a, 0, sizeof a);
来源：http://zgt.ppjwa.cn

[S27] C：定义常量
来源：http://zqj.zhongyouzk.top

const double PI = 3.14159;
来源：http://jyy.zhiwuduotai.top

[S28] C：静态变量
来源：http://msk.jqgfzy.top

static int counter = 0;
来源：http://kdx.ivvv.top

[S29] C：变参函数
来源：http://xtk.svipenyu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wkz.hfpthk.cn

[S30] C：头文件保护
来源：http://fti.hysaishi.cn

#ifndef X_H
来源：http://rwh.aibaodan.cn

#define X_H
来源：http://fkv.dianchejie.cn

#endif
来源：http://jov.tian-w.cn

[S31] C++：Hello World
来源：http://cnn.birdmap.top

#include <iostream>
来源：http://lqb.jyoumei.cn

int main() { std::cout << "Hello\n"; }
来源：http://oxp.snrcjt.cn

[S32] C++：字符串
来源：http://dfw.yangfankeji.com

std::string s = "hi";  s += "!";
来源：http://stl.jyoumei.cn

[S33] C++：vector 增删
来源：http://epl.jinqigfzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gjf.zycfv.cn

[S34] C++：遍历 vector
来源：http://klq.nanxuanxn.top

for (auto &x : v) { std::cout << x; }
来源：http://poq.jqgufenzy.top

[S35] C++：map
来源：http://awl.zhiwuduotai.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vfa.fehbvm.com

[S36] C++：unordered_map
来源：http://ytg.jqgfzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ffo.xinyue.icu

[S37] C++：set
来源：http://vyq.9152youxi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kpd.yanxiufei.cn

[S38] C++：排序
来源：http://bih.fzhhl.top

std::sort(v.begin(), v.end());
来源：http://dus.yueranfly.top

[S39] C++：自定义比较器排序
来源：http://sdc.sweek.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bch.hywenlv.cn

[S40] C++：查找元素
来源：http://wxc.0kj1m.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://czm.zhixingplan.top

[S41] C++：类与构造函数
来源：http://ylg.tanke756.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xnm.hongshengwenyu.top

[S42] C++：继承与虚函数
来源：http://vtb.ivvv.top

class B : public Base { public: void f() override {} };
来源：http://cvs.jyoumei.cn

[S43] C++：智能指针
来源：http://hxx.zdqjudy.top

auto p = std::make_unique<int>(5);
来源：http://hap.hnxiangtu.top

[S44] C++：引用传参
来源：http://vzj.dashuyun.cn

void inc(int &x) { ++x; }
来源：http://gyp.epnwcf.com

[S45] C++：lambda
来源：http://xnn.gotoacloud.top

auto add = [](int a, int b) { return a + b; };
来源：http://ppx.zhengqikj.top

[S46] C++：函数模板
来源：http://daz.hammf.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qnb.jinghuilouyu.cn

[S47] C++：结构化绑定遍历
来源：http://xyy.xinyue.icu

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://eqz.yuxming.cn

[S48] C++：逐行读文件
来源：http://plw.yuxming.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wzw.yangfankeji.com

while (std::getline(in, line)) { }
来源：http://xll.gzhubu.top

[S49] C++：写文件
来源：http://dph.fktsv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qvp.hywenlv.cn

[S50] C++：格式化数字
来源：http://mlh.yonumen.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rpo.jqgfzy.top

[S51] C++：显式类型转换
来源：http://xpv.shuidangran.top

static_cast<double>(a) / b
来源：http://fua.ybcxt.top

[S52] C++：const 与 noexcept
来源：http://fas.hnqzz.top

int size() const noexcept { return n_; }
来源：http://zxu.andypj.xyz

[S53] C++：移动语义
来源：http://opg.shanyushiyangtech.top

std::vector<int> w = std::move(v);
来源：http://fxo.52xcode.cn

[S54] C++：异常处理
来源：http://uco.sysykeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kcf.yfazqb.com

[S55] C++：结构化绑定
来源：http://rua.meibo888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://wem.shanyushiyangkeji.top

[S56] C++：optional
来源：http://mwd.svipenyu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lyb.yueranfly.top

[S57] C++：编译期常量
来源：http://lev.shzxlz.cn

constexpr int N = 10;
来源：http://obr.zhoulong.xyz

[S58] C++：命名空间
来源：http://qkc.shzxlz.cn

namespace ns { int f() { return 1; } }
来源：http://cwf.redwolf501.top

[S59] C++：静态断言
来源：http://drj.tian-w.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://luw.birdmap.top

[S60] C++：遍历并删除元素
来源：http://oee.zhaomingkeji.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sdq.vehdjk.com

================================================================================
来源：http://ltc.gogol.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iiy.sweek.top

================================================================================
来源：http://fdy.sweek.top

[T01] Kotlin：Hello World
来源：http://qgy.jiagoushi.top

println("Hello")
来源：http://jdp.shzxlz.cn

[T02] Kotlin：变量
来源：http://xpz.chenlongwang.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kxz.hesvh.cn

[T03] Kotlin：字符串模板
来源：http://khj.havefunace.top

"值: $b"
来源：http://mks.hfpthk.cn

[T04] Kotlin：空安全
来源：http://afb.jinqigufen.top

val n: String? = null;  n?.length
来源：http://vjx.sxryk.cn

[T05] Kotlin：when 表达式
来源：http://tdl.uphjek.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://den.yj202588.top

[T06] Kotlin：集合映射
来源：http://xic.wangdashe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tey.zycfv.cn

[T07] Kotlin：集合过滤
来源：http://nia.yvedp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ucx.feifeiyinyue.top

[T08] Kotlin：数据类
来源：http://ped.yueranfly.top

data class User(val name: String, val age: Int)
来源：http://cye.guowangkeji.top

[T09] Kotlin：扩展函数
来源：http://hll.ppjwa.cn

fun String.exclaim() = this + "!"
来源：http://dkt.uphjek.com

[T10] Kotlin：默认参数
来源：http://vjh.kuanghao11.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ayf.snrcjt.cn

[T11] Kotlin：协程
来源：http://mph.jqgufenzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://bjb.yj20258888.top

[T12] Kotlin：解构声明
来源：http://dsq.jinqigfzy.top

val (a, b) = Pair(1, 2)
来源：http://ypc.cqqwz.cn

[T13] Kotlin：只读 Map
来源：http://ovq.chenjidiqi.icu

val m = mapOf("a" to 1)
来源：http://krn.meibo888.top

[T14] Kotlin：循环
来源：http://hgk.havefunace.top

for (i in 1..10) println(i)
来源：http://exf.kuanghao11.cn

[T15] Kotlin：接口
来源：http://zts.fzhhl.top

interface Shape { fun area(): Double }
来源：http://zdc.quarkkingdee.top

[T16] Swift：Hello World
来源：http://ddq.hfpthk.cn

print("Hello")
来源：http://lnx.jlsjyb.cn

[T17] Swift：变量与常量
来源：http://ktq.nwbrower.top

var a = 1;  let b = 2
来源：http://mai.yj20258888.top

[T18] Swift：字符串插值
来源：http://xyh.haohaochexian.top

"值: \(b)"
来源：http://ojn.yfazqb.com

[T19] Swift：可选绑定
来源：http://fwb.jyoumei.cn

if let n = opt { print(n) }
来源：http://rpj.smart0.xyz

[T20] Swift：数组操作
来源：http://mof.zhaomingkeji.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://hpu.cucudq.cn

[T21] Swift：遍历
来源：http://wqj.yj20258888.top

for x in a { print(x) }
来源：http://yrt.cdnleiting.top

[T22] Swift：字典
来源：http://say.sufxvd.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ert.zdqjudy.top

[T23] Swift：函数
来源：http://ibs.zycfv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vhx.ehwqpu.com

[T24] Swift：闭包
来源：http://brf.jinghuilouyu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tgp.xingfuxueyuan.xyz

[T25] Swift：结构体
来源：http://pxs.guowangkeji.top

struct P { var x: Int }
来源：http://ofo.ppjwa.cn

[T26] Swift：类与重写
来源：http://ysh.52xcode.cn

class A: Base { override func f() {} }
来源：http://jzi.sjlbkw.cn

[T27] Swift：错误处理
来源：http://kdr.ydzc1.top

do { try f() } catch { print(error) }
来源：http://lwx.jiagoushi.top

[T28] Swift：枚举
来源：http://nja.havefunace.top

enum Color { case red, green }
来源：http://www.shuidangran.top

[T29] Swift：guard 提前返回
来源：http://khw.ctjpmb.com

guard let x = opt else { return }
来源：http://ept.xingfuxueyuan.xyz

[T30] Swift：协议
来源：http://cvx.dianchejie.cn

protocol Shape { func area() -> Double }
来源：http://ovg.aibaodan.cn

[T31] Lua：Hello World
来源：http://vvv.jlsjyb.cn

print("Hello")
来源：http://csg.pengpengdd.cyou

[T32] Lua：局部变量
来源：http://yff.fehbvm.com

local a = 1
来源：http://otx.ywan-chungtsiang.top

[T33] Lua：表（数组）
来源：http://mkx.jinyuanbaomall.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://aaj.sweek.top

[T34] Lua：遍历表
来源：http://clf.chenzaomai.com

for i, v in ipairs(t) do print(i, v) end
来源：http://hgo.zhengqikj.top

[T35] Lua：字典表
来源：http://vxx.fzhhl.top

local d = { a = 1 };  d.b = 2
来源：http://ejn.yfazqb.com

[T36] Lua：函数
来源：http://iik.jinqigfzy.top

function add(a, b) return a + b end
来源：http://uiy.uphjek.com

[T37] Lua：字符串拼接
来源：http://ssy.zhoulong.xyz

"a" .. "b"
来源：http://ixs.haohaochexian.top

[T38] Lua：条件
来源：http://nyf.xinyue.icu

if x > 0 then print("正") end
来源：http://wzb.jinghuilouyu.cn

[T39] Lua：模式匹配
来源：http://paq.havefunace.top

string.find(s, "%d+")
来源：http://fwn.vqdsnc.cn

[T40] Lua：元表
来源：http://mkr.shzxlz.cn

setmetatable({}, { __index = base })
来源：http://qfo.vqdsnc.cn

[T41] Perl：Hello World
来源：http://jyz.chenjidiqi.icu

print "Hello\n";
来源：http://pia.ppjwa.cn

[T42] Perl：变量类型
来源：http://snq.ehwqpu.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nuk.iojbl.cn

[T43] Perl：字符串插值
来源：http://bbb.yfazqb.com

"值: $a"
来源：http://bqs.sysykeji.top

[T44] Perl：条件
来源：http://ste.xziqi.cn

if ($a > 0) { print "正"; }
来源：http://sjh.ppjwa.cn

[T45] Perl：数组遍历
来源：http://mbu.daria6918.cn

for my $x (@arr) { print $x; }
来源：http://wjo.shanyushiyangkeji.top

[T46] Perl：哈希操作
来源：http://vbk.pycfn.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vue.cheryme.top

[T47] Perl：正则捕获
来源：http://qoz.zhijiandao.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://odr.sysykeji.top

[T48] Perl：正则替换
来源：http://vho.svipenyu.cn

$s =~ s/old/new/g;
来源：http://zxs.jinqigfzy.top

[T49] Perl：函数
来源：http://tgi.guannengcc.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ygc.9152youxi.cn

[T50] Perl：逐行读文件
来源：http://ixf.gotoacloud.top

open my $fh, "<", "a.txt" or die $!;
来源：http://wfv.ppjwa.cn

while (my $line = <$fh>) { print $line; }
来源：http://uid.hnxiangtu.top

[T51] Scala：Hello World
来源：http://vrg.gogol.net.cn

println("Hello")
来源：http://hdj.xylfe.cn

[T52] Scala：变量
来源：http://bpr.hysaishi.cn

val a = 1;  var b = 2
来源：http://nld.cqqwz.cn

[T53] Scala：字符串插值
来源：http://skx.nanxinkj.top

s"值: $b"
来源：http://jvi.bbcook.cn

[T54] Scala：集合映射
来源：http://uyn.tian-w.cn

List(1, 2, 3).map(_ * 2)
来源：http://mwj.sxryk.cn

[T55] Scala：集合过滤
来源：http://ffj.andypj.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://hmi.yuanzhike.top

[T56] Scala：样例类
来源：http://ngo.hnxiangtu.top

case class User(name: String, age: Int)
来源：http://erz.haohaochexian.top

[T57] Scala：模式匹配
来源：http://wbj.ivvv.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vzf.guowangkeji.top

[T58] Scala：函数定义
来源：http://axz.jiagoushi.top

def add(a: Int, b: Int): Int = a + b
来源：http://dsh.yangfankeji.com

[T59] Scala：循环
来源：http://kgg.xinyue.icu

for (i <- 1 to 10) println(i)
来源：http://fas.tarul.cn

[T60] Scala：折叠
来源：http://fob.uphjek.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ldk.cashguo.top

================================================================================
来源：http://gad.zhaomingkeji.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qmm.shzxlz.cn

================================================================================
来源：http://sku.cqqwz.cn

[U01] Py：创建虚拟环境
来源：http://mgp.hnxiangtu.top

python -m venv .venv && source .venv/bin/activate
来源：http://xss.gotoacloud.top

[U02] Py：导出 / 安装依赖
来源：http://odc.yj202588.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wks.aibaodan.cn


<!-- 参考信息 -->