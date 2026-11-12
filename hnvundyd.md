代发 wailian999

free -h;  ps aux | grep nginx
来源：http://fxb.jinghuilouyu.cn

[R64] 结束进程
来源：http://pab.c1oappe.top

kill -9 $(pgrep -f app.py)
来源：http://xbt.tanke756.top

[R65] 查看端口占用
来源：http://bre.nanxuanxn.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xsb.hfpthk.cn

[R66] 定时任务
来源：http://ebi.chenjidiqi.icu

crontab -e;  crontab -l
来源：http://klt.xingfuxueyuan.xyz

[R67] 生成随机十六进制串
来源：http://neb.zhijiandao.cn

openssl rand -hex 16
来源：http://moc.redwolf501.top

[R68] 计算文件校验值
来源：http://fru.jinqigufen.top

sha256sum a.txt;  md5sum a.txt
来源：http://bdz.iojbl.cn

[R69] 生成随机密码
来源：http://sva.dashuyun.cn

head -c 16 /dev/urandom | base64
来源：http://fpy.fehbvm.com

[R70] 时间戳与互转
来源：http://tgj.fktsv.cn

date +%s;  date -d @1700000000
来源：http://ske.jqgufenzy.top

[R71] 日期格式化
来源：http://qqi.xylfe.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gjf.svipenyu.cn

[R72] 等待端口就绪
来源：http://rjk.sufxvd.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wov.jinyuanbaomall.cn

[R73] 分割大日志
来源：http://wyp.jinqigfzy.top

split -l 1000 big.log part_
来源：http://hxu.birdmap.top

[R74] 批量重命名
来源：http://psq.ehwqpu.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xgy.cdnleiting.top

[R75] 导出环境变量
来源：http://fih.hnxiangtu.top

export PATH="$HOME/bin:$PATH"
来源：http://arm.hnqzz.top

[R76] 使用临时文件
来源：http://icf.yj20258.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cwk.cheryme.top

[R77] 读取用户输入
来源：http://uws.chenlongwang.top

read -rp "请输入: " ans
来源：http://tsz.52xcode.cn

[R78] 交互式菜单
来源：http://kpq.andypj.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://rwr.hnxiangtu.top

[R79] 解析命令行选项
来源：http://wsg.aibaodan.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mdz.uphjek.com

[R80] 查看脚本执行耗时
来源：http://gfp.tianlin.xyz

time ./run.sh
来源：http://gxy.hywenlv.cn

================================================================================
来源：http://ehw.gotoacloud.top

S. C / C++ 专题
来源：http://cla.yvedp.cn

================================================================================
来源：http://sjc.haohaochexian.top

[S01] C：Hello World
来源：http://bpq.tarul.cn

#include <stdio.h>
来源：http://cvc.yj202588.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://oru.jinqigfzy.top

[S02] C：变量与格式化输出
来源：http://ikx.yj202588.top

int a = 10; printf("%d\n", a);
来源：http://odn.hywenlv.cn

[S03] C：读入整数
来源：http://rti.aibaodan.cn

int x; scanf("%d", &x);
来源：http://bib.jinghuilouyu.cn

[S04] C：字符串复制
来源：http://sqh.tian-w.cn

char dst[32]; strcpy(dst, "hi");
来源：http://eye.tanke756.top

[S05] C：字符串长度
来源：http://igm.xylfe.cn

strlen(s)
来源：http://yqg.wangdashe.top

[S06] C：字符串比较
来源：http://dpc.cashguo.top

strcmp(a, b) == 0
来源：http://crd.nanxinkj.top

[S07] C：数组遍历求和
来源：http://znx.hfpthk.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lvo.yanxiufei.cn

[S08] C：动态内存分配与释放
来源：http://wxa.hesvh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mzk.hammf.cn

[S09] C：结构体定义与初始化
来源：http://afj.vehdjk.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://slq.gogol.net.cn

[S10] C：指针与解引用
来源：http://ioa.mhx1999.top

int *p = &a;  *p = 5;
来源：http://rsg.shanyushiyangkeji.top

[S11] C：逐行读文件
来源：http://anr.0kj1m.cn

FILE *f = fopen("a.txt", "r");
来源：http://kum.zhixingplan.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ifp.ybcxt.top

fclose(f);
来源：http://nul.zycfv.cn

[S12] C：写文件
来源：http://yxm.yuanzhike.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blc.jinqigfzy.top

[S13] C：宏定义
来源：http://mit.tian-w.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ssi.nanxinkj.top

[S14] C：枚举
来源：http://rao.zycfv.cn

enum Color { RED, GREEN, BLUE };
来源：http://njt.xinyue.icu

[S15] C：类型转换
来源：http://mve.fengsongda.top

(double) a / b
来源：http://pro.hnxiangtu.top

[S16] C：位操作置位
来源：http://lxk.nanxinkj.top

x |= (1 << 3);
来源：http://krf.epnwcf.com

[S17] C：安全拼接字符串
来源：http://uah.yj202588.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ysh.gzhubu.top

[S18] C：命令行参数
来源：http://sdo.hfpthk.cn

int main(int argc, char **argv)
来源：http://xku.jinqigfzy.top

[S19] C：快速排序
来源：http://lok.ehwqpu.com

qsort(a, n, sizeof(int), cmp);
来源：http://zwa.havefunace.top

[S20] C：二分查找
来源：http://pvu.c1oappe.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bjq.sjlbkw.cn

[S21] C：字符类别判断
来源：http://acu.chenjidiqi.icu

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pms.haohaochexian.top

[S22] C：字符串转数字
来源：http://khz.zhaomingkeji.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://ssp.bjfxy.top

[S23] C：随机数
来源：http://inm.hnqzz.top

srand(time(NULL));  int r = rand() % 100;
来源：http://phn.redwolf501.top

[S24] C：获取本地时间
来源：http://jol.cqqwz.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zuk.yj20258.top

[S25] C：内存拷贝
来源：http://kjn.fehbvm.com

memcpy(dst, src, n);
来源：http://yqe.gogol.net.cn

[S26] C：内存清零
来源：http://jcr.c1oappe.top

memset(a, 0, sizeof a);
来源：http://oyw.jinghuilouyu.cn

[S27] C：定义常量
来源：http://kbv.tianlin.xyz

const double PI = 3.14159;
来源：http://lvh.zdqjudy.top

[S28] C：静态变量
来源：http://yfs.zhixingplan.top

static int counter = 0;
来源：http://rzm.kuanghao11.cn

[S29] C：变参函数
来源：http://cqf.jinqigfzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hiz.xylfe.cn

[S30] C：头文件保护
来源：http://hxy.guowangkeji.top

#ifndef X_H
来源：http://akf.dashuyun.cn

#define X_H
来源：http://ibu.jinyuanbaomall.cn

#endif
来源：http://uij.yongpay.top

[S31] C++：Hello World
来源：http://yua.dashuyun.cn

#include <iostream>
来源：http://dap.bjfxy.top

int main() { std::cout << "Hello\n"; }
来源：http://uco.nwbrower.top

[S32] C++：字符串
来源：http://vxj.aibaodan.cn

std::string s = "hi";  s += "!";
来源：http://tjm.yonumen.top

[S33] C++：vector 增删
来源：http://lqy.tanke756.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pit.tianlin.xyz

[S34] C++：遍历 vector
来源：http://ite.zhaomingkeji.xyz

for (auto &x : v) { std::cout << x; }
来源：http://tps.zhixingplan.top

[S35] C++：map
来源：http://kak.zhongyouzk.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jom.shuidangran.top

[S36] C++：unordered_map
来源：http://ihk.gaohongyu789.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dvh.chenlongwang.top

[S37] C++：set
来源：http://kgk.sysykeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ugw.cqqwz.cn

[S38] C++：排序
来源：http://yhg.jinyuanbaomall.cn

std::sort(v.begin(), v.end());
来源：http://vuu.dashuyun.cn

[S39] C++：自定义比较器排序
来源：http://czr.xinyue.icu

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gaw.xinyue.icu

[S40] C++：查找元素
来源：http://xxl.kuanghao11.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lfo.xziqi.cn

[S41] C++：类与构造函数
来源：http://nqt.shuidangran.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cob.tarul.cn

[S42] C++：继承与虚函数
来源：http://aep.yuanzhike.top

class B : public Base { public: void f() override {} };
来源：http://lpb.jianghu66.top

[S43] C++：智能指针
来源：http://ojt.jinqigufen.top

auto p = std::make_unique<int>(5);
来源：http://jty.tianlin.xyz

[S44] C++：引用传参
来源：http://mgi.pycfn.com

void inc(int &x) { ++x; }
来源：http://scd.aizwys.cn

[S45] C++：lambda
来源：http://pli.andypj.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://bgm.zycfv.cn

[S46] C++：函数模板
来源：http://dfm.chenlongwang.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ymp.yj20258.top

[S47] C++：结构化绑定遍历
来源：http://nxo.zhoulong.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ton.0kj1m.cn

[S48] C++：逐行读文件
来源：http://inp.jianghu66.top

std::ifstream in("a.txt");  std::string line;
来源：http://cpk.yonumen.top

while (std::getline(in, line)) { }
来源：http://yzn.yueranfly.top

[S49] C++：写文件
来源：http://kjc.yvedp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jal.aizwys.cn

[S50] C++：格式化数字
来源：http://dsp.9152youxi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kxs.wangshuangyany.cn

[S51] C++：显式类型转换
来源：http://fkw.hnqzz.top

static_cast<double>(a) / b
来源：http://rwg.yueranfly.top

[S52] C++：const 与 noexcept
来源：http://jlk.andypj.xyz

int size() const noexcept { return n_; }
来源：http://owt.aibaodan.cn

[S53] C++：移动语义
来源：http://fve.vqdsnc.cn

std::vector<int> w = std::move(v);
来源：http://sbf.ivvv.top

[S54] C++：异常处理
来源：http://ier.guannengcc.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vmc.zycfv.cn

[S55] C++：结构化绑定
来源：http://yrm.hammf.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ngt.xziqi.cn

[S56] C++：optional
来源：http://ljy.havefunace.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lqr.52xcode.cn

[S57] C++：编译期常量
来源：http://lbx.yanxiufei.cn

constexpr int N = 10;
来源：http://ucy.gotoacloud.top

[S58] C++：命名空间
来源：http://pli.hysaishi.cn

namespace ns { int f() { return 1; } }
来源：http://fus.jianghu66.top

[S59] C++：静态断言
来源：http://jqh.aizwys.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eta.fzhhl.top

[S60] C++：遍历并删除元素
来源：http://flw.daria6918.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rba.hnxiangtu.top

================================================================================
来源：http://otl.bbcook.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://guy.hongshengwenyu.top

================================================================================
来源：http://efu.sufxvd.cn

[T01] Kotlin：Hello World
来源：http://duh.bjfxy.top

println("Hello")
来源：http://xsw.bbcook.cn

[T02] Kotlin：变量
来源：http://ten.hammf.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dxc.aibaodan.cn

[T03] Kotlin：字符串模板
来源：http://inl.daria6918.cn

"值: $b"
来源：http://nwb.jlsjyb.cn

[T04] Kotlin：空安全
来源：http://ddh.ywan-chungtsiang.top

val n: String? = null;  n?.length
来源：http://lpo.xinyue.icu

[T05] Kotlin：when 表达式
来源：http://rep.ywan-chungtsiang.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mex.xylfe.cn

[T06] Kotlin：集合映射
来源：http://ozy.gzhubu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://nvj.cashguo.top

[T07] Kotlin：集合过滤
来源：http://eed.xylfe.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ekv.cashguo.top

[T08] Kotlin：数据类
来源：http://wjz.jinqigfzy.top

data class User(val name: String, val age: Int)
来源：http://xtt.hysaishi.cn

[T09] Kotlin：扩展函数
来源：http://gkv.daxiang520.top

fun String.exclaim() = this + "!"
来源：http://vjt.ydzc1.top

[T10] Kotlin：默认参数
来源：http://zgd.dianchejie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://csg.yuanzhike.top

[T11] Kotlin：协程
来源：http://kuc.hcnkem.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://inq.jinqigfzy.top

[T12] Kotlin：解构声明
来源：http://cjg.jqgfzy.top

val (a, b) = Pair(1, 2)
来源：http://try.hywenlv.cn

[T13] Kotlin：只读 Map
来源：http://txw.ehwqpu.com

val m = mapOf("a" to 1)
来源：http://rrj.yonumen.top

[T14] Kotlin：循环
来源：http://yrl.shanyushiyangtech.top

for (i in 1..10) println(i)
来源：http://vic.zycfv.cn

[T15] Kotlin：接口
来源：http://hip.jqgufenzy.top

interface Shape { fun area(): Double }
来源：http://grr.cheryme.top

[T16] Swift：Hello World
来源：http://cnk.smart0.xyz

print("Hello")
来源：http://ett.ctjpmb.com

[T17] Swift：变量与常量
来源：http://hxf.xziqi.cn

var a = 1;  let b = 2
来源：http://vpl.nanxuanxn.top

[T18] Swift：字符串插值
来源：http://mbp.gaohongyu789.top

"值: \(b)"
来源：http://aiy.jinqigfzy.top

[T19] Swift：可选绑定
来源：http://xnn.vqdsnc.cn

if let n = opt { print(n) }
来源：http://axz.xingfuxueyuan.xyz

[T20] Swift：数组操作
来源：http://ypm.hongshengwenyu.top

var a = [1, 2, 3];  a.append(4)
来源：http://egh.fehbvm.com

[T21] Swift：遍历
来源：http://pps.wangdashe.top

for x in a { print(x) }
来源：http://hzd.shzxlz.cn

[T22] Swift：字典
来源：http://cii.chenlongwang.top

var d = ["a": 1];  d["b"] = 2
来源：http://apj.cashguo.top

[T23] Swift：函数
来源：http://zlu.9152youxi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dgo.andypj.xyz

[T24] Swift：闭包
来源：http://sim.dashuyun.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://nvj.yueranfly.top

[T25] Swift：结构体
来源：http://qcb.vqdsnc.cn

struct P { var x: Int }
来源：http://uua.nanxuanxn.top

[T26] Swift：类与重写
来源：http://wok.chenlongwang.top

class A: Base { override func f() {} }
来源：http://crd.shanyushiyangkeji.top

[T27] Swift：错误处理
来源：http://vfi.zhijiandao.cn

do { try f() } catch { print(error) }
来源：http://qjd.ydzc1.top

[T28] Swift：枚举
来源：http://xwm.yonumen.top

enum Color { case red, green }
来源：http://fmi.iojbl.cn

[T29] Swift：guard 提前返回
来源：http://aek.meibo888.top

guard let x = opt else { return }
来源：http://psz.ctjpmb.com

[T30] Swift：协议
来源：http://npz.jlsjyb.cn

protocol Shape { func area() -> Double }
来源：http://tam.bbcook.cn

[T31] Lua：Hello World
来源：http://uzi.shanyushiyangkeji.top

print("Hello")
来源：http://thx.iojbl.cn

[T32] Lua：局部变量
来源：http://iws.pengpengdd.cyou

local a = 1
来源：http://vcv.daria6918.cn

[T33] Lua：表（数组）
来源：http://mor.vqdsnc.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://com.shanyushiyangkeji.top

[T34] Lua：遍历表
来源：http://eax.gogol.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ioe.yvedp.cn

[T35] Lua：字典表
来源：http://lhc.yonumen.top

local d = { a = 1 };  d.b = 2
来源：http://cqp.fanxiaobao.xyz

[T36] Lua：函数
来源：http://jhj.yuxming.cn

function add(a, b) return a + b end
来源：http://lml.tanke756.top

[T37] Lua：字符串拼接
来源：http://owp.chenjidiqi.icu

"a" .. "b"
来源：http://nwc.hcnkem.com

[T38] Lua：条件
来源：http://seh.ctjpmb.com

if x > 0 then print("正") end
来源：http://beh.xinyue.icu

[T39] Lua：模式匹配
来源：http://qxm.52xcode.cn

string.find(s, "%d+")
来源：http://dyo.pycfn.com

[T40] Lua：元表
来源：http://vlf.nwbrower.top

setmetatable({}, { __index = base })
来源：http://asz.sjlbkw.cn

[T41] Perl：Hello World
来源：http://hey.jqgfzy.top

print "Hello\n";
来源：http://xqy.sweek.top

[T42] Perl：变量类型
来源：http://qvx.yonumen.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://iaz.yanxiufei.cn

[T43] Perl：字符串插值
来源：http://kmz.kuanghao11.cn

"值: $a"
来源：http://ouc.jiagoushi.top

[T44] Perl：条件
来源：http://drp.9152youxi.cn

if ($a > 0) { print "正"; }
来源：http://oss.jinghuilouyu.cn

[T45] Perl：数组遍历
来源：http://hyf.mhx1999.top

for my $x (@arr) { print $x; }
来源：http://jng.316326.xyz

[T46] Perl：哈希操作
来源：http://qxu.sweek.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yhi.9152youxi.cn

[T47] Perl：正则捕获
来源：http://dqg.yuanzhike.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://fzq.zhongyouzk.top

[T48] Perl：正则替换
来源：http://hfz.haohaochexian.top

$s =~ s/old/new/g;
来源：http://fkr.xuetiantiany.cn

[T49] Perl：函数
来源：http://nvy.ydjk.org.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fgu.yuanzhike.top

[T50] Perl：逐行读文件
来源：http://ixn.sxryk.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ndt.hfpthk.cn

while (my $line = <$fh>) { print $line; }
来源：http://tty.yongpay.top

[T51] Scala：Hello World
来源：http://xnn.vqdsnc.cn

println("Hello")
来源：http://wcd.daria6918.cn

[T52] Scala：变量
来源：http://kwt.zhoulong.xyz

val a = 1;  var b = 2
来源：http://zxk.cqqwz.cn

[T53] Scala：字符串插值
来源：http://grb.xylfe.cn

s"值: $b"
来源：http://gkq.tanke756.top

[T54] Scala：集合映射
来源：http://jon.ivvv.top

List(1, 2, 3).map(_ * 2)
来源：http://vuh.ydjk.org.cn

[T55] Scala：集合过滤
来源：http://oxp.zhijiandao.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ihv.aibaodan.cn

[T56] Scala：样例类
来源：http://mjk.mhx1999.top

case class User(name: String, age: Int)
来源：http://pin.yj20258.top

[T57] Scala：模式匹配
来源：http://jby.cdnleiting.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://gfy.birdmap.top

[T58] Scala：函数定义
来源：http://xpa.xylfe.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zua.yj20258.top

[T59] Scala：循环
来源：http://ssj.zhixingplan.top

for (i <- 1 to 10) println(i)
来源：http://cnb.cdnleiting.top

[T60] Scala：折叠
来源：http://gba.yj20258.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qir.316326.xyz

================================================================================
来源：http://kch.guannengcc.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ykt.hfpthk.cn

================================================================================
来源：http://gya.ybcxt.top

[U01] Py：创建虚拟环境
来源：http://fpq.aizwys.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gxh.sweek.top

[U02] Py：导出 / 安装依赖
来源：http://vfm.cucudq.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gvk.sysykeji.top

[U03] Py：加载 .env 配置
来源：http://pfj.gogol.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nnp.sysykeji.top

[U04] Py：变量调试打印
来源：http://abe.hysaishi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://onk.nanxuanxn.top


<!-- 参考信息 -->