代发 wailian999

df -h;  du -sh *
来源：http://nsa.shanyushiyangkeji.top

[R62] 找最占空间的文件
来源：http://gcy.feifeiyinyue.top

du -ah . | sort -rh | head -10
来源：http://fuj.mhx1999.top

[R63] 内存与进程
来源：http://eie.pycfn.com

free -h;  ps aux | grep nginx
来源：http://ple.c1oappe.top

[R64] 结束进程
来源：http://gnl.ivvv.top

kill -9 $(pgrep -f app.py)
来源：http://ofb.dianchejie.cn

[R65] 查看端口占用
来源：http://kxo.vehdjk.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pdk.ivvv.top

[R66] 定时任务
来源：http://pch.ywan-chungtsiang.top

crontab -e;  crontab -l
来源：http://tlw.ppjwa.cn

[R67] 生成随机十六进制串
来源：http://ygi.chenjidiqi.icu

openssl rand -hex 16
来源：http://bvc.tarul.cn

[R68] 计算文件校验值
来源：http://tky.dianchejie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jya.ybcxt.top

[R69] 生成随机密码
来源：http://qcb.jianghu66.top

head -c 16 /dev/urandom | base64
来源：http://xst.chenlongwang.top

[R70] 时间戳与互转
来源：http://hsw.yj202588.top

date +%s;  date -d @1700000000
来源：http://zcb.zdbjq.cn

[R71] 日期格式化
来源：http://ahr.cheryme.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://hrw.haohaochexian.top

[R72] 等待端口就绪
来源：http://wxr.tian-w.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rkp.meibo888.top

[R73] 分割大日志
来源：http://mco.daxiang520.top

split -l 1000 big.log part_
来源：http://npp.vqdsnc.cn

[R74] 批量重命名
来源：http://eop.ehwqpu.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mef.bbcook.cn

[R75] 导出环境变量
来源：http://koq.fanxiaobao.xyz

export PATH="$HOME/bin:$PATH"
来源：http://fyy.mhx1999.top

[R76] 使用临时文件
来源：http://tje.ydjk.org.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://otg.sweek.top

[R77] 读取用户输入
来源：http://kar.bjfxy.top

read -rp "请输入: " ans
来源：http://ejh.sysykeji.top

[R78] 交互式菜单
来源：http://chv.guowangkeji.top

select opt in a b c; do echo "$opt"; break; done
来源：http://lvc.hnqzz.top

[R79] 解析命令行选项
来源：http://dai.tianlin.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ejn.sweek.top

[R80] 查看脚本执行耗时
来源：http://blc.zhiwuduotai.top

time ./run.sh
来源：http://ekm.kuanghao11.cn

================================================================================
来源：http://xly.smart0.xyz

S. C / C++ 专题
来源：http://oxy.0kj1m.cn

================================================================================
来源：http://dhl.hcnkem.com

[S01] C：Hello World
来源：http://ifl.uphjek.com

#include <stdio.h>
来源：http://hno.cucudq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sze.yuxming.cn

[S02] C：变量与格式化输出
来源：http://yaj.jlsjyb.cn

int a = 10; printf("%d\n", a);
来源：http://msa.jqgfzy.top

[S03] C：读入整数
来源：http://nzf.9152youxi.cn

int x; scanf("%d", &x);
来源：http://tmg.gotoacloud.top

[S04] C：字符串复制
来源：http://yaw.ydjk.org.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fjq.feifeiyinyue.top

[S05] C：字符串长度
来源：http://whe.xylfe.cn

strlen(s)
来源：http://msp.shanyushiyangtech.top

[S06] C：字符串比较
来源：http://boc.jyoumei.cn

strcmp(a, b) == 0
来源：http://edr.yongpay.top

[S07] C：数组遍历求和
来源：http://rqc.cashguo.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gbo.quarkkingdee.top

[S08] C：动态内存分配与释放
来源：http://zgr.wangdashe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://flh.wangdashe.top

[S09] C：结构体定义与初始化
来源：http://vcd.xingfuxueyuan.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qif.yongpay.top

[S10] C：指针与解引用
来源：http://ifx.jiagoushi.top

int *p = &a;  *p = 5;
来源：http://uye.fengsongda.top

[S11] C：逐行读文件
来源：http://rwu.hammf.cn

FILE *f = fopen("a.txt", "r");
来源：http://nyx.chenjidiqi.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://qjg.jianghu66.top

fclose(f);
来源：http://hoj.yanxiufei.cn

[S12] C：写文件
来源：http://mhe.birdmap.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rsa.havefunace.top

[S13] C：宏定义
来源：http://skq.havefunace.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://buf.fktsv.cn

[S14] C：枚举
来源：http://gsa.guowangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://atw.jinghuilouyu.cn

[S15] C：类型转换
来源：http://cei.ybcxt.top

(double) a / b
来源：http://zgv.sweek.top

[S16] C：位操作置位
来源：http://ijm.ywan-chungtsiang.top

x |= (1 << 3);
来源：http://kdc.0kj1m.cn

[S17] C：安全拼接字符串
来源：http://bvt.iojbl.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hqj.yj20258888.top

[S18] C：命令行参数
来源：http://wia.xingfuxueyuan.xyz

int main(int argc, char **argv)
来源：http://uhu.smart0.xyz

[S19] C：快速排序
来源：http://irs.fzhhl.top

qsort(a, n, sizeof(int), cmp);
来源：http://ypq.yanxiufei.cn

[S20] C：二分查找
来源：http://krm.hnqzz.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bml.hnxiangtu.top

[S21] C：字符类别判断
来源：http://eda.cashguo.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://iws.hnqzz.top

[S22] C：字符串转数字
来源：http://upk.dashuyun.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jix.fehbvm.com

[S23] C：随机数
来源：http://goy.yuanzhike.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qeq.bbcook.cn

[S24] C：获取本地时间
来源：http://xwd.yvedp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oho.yuxming.cn

[S25] C：内存拷贝
来源：http://xbm.ehwqpu.com

memcpy(dst, src, n);
来源：http://srw.xylfe.cn

[S26] C：内存清零
来源：http://ctj.ydjk.org.cn

memset(a, 0, sizeof a);
来源：http://nkv.kuanghao11.cn

[S27] C：定义常量
来源：http://rgl.aibaodan.cn

const double PI = 3.14159;
来源：http://ohv.snrcjt.cn

[S28] C：静态变量
来源：http://ezf.ctjpmb.com

static int counter = 0;
来源：http://par.jqgufenzy.top

[S29] C：变参函数
来源：http://kjm.xylfe.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kho.gaohongyu789.top

[S30] C：头文件保护
来源：http://kjm.dashuyun.cn

#ifndef X_H
来源：http://mlp.kuanghao11.cn

#define X_H
来源：http://jbm.ywan-chungtsiang.top

#endif
来源：http://eph.ywan-chungtsiang.top

[S31] C++：Hello World
来源：http://kuk.pengpengdd.cyou

#include <iostream>
来源：http://lnq.0kj1m.cn

int main() { std::cout << "Hello\n"; }
来源：http://bpq.fzhhl.top

[S32] C++：字符串
来源：http://wvk.zhengqikj.top

std::string s = "hi";  s += "!";
来源：http://nee.ydzc1.top

[S33] C++：vector 增删
来源：http://aij.shanyushiyangtech.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://chy.jlsjyb.cn

[S34] C++：遍历 vector
来源：http://ozo.zhengqikj.top

for (auto &x : v) { std::cout << x; }
来源：http://msf.yfazqb.com

[S35] C++：map
来源：http://coo.jinyuanbaomall.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://iia.hnxiangtu.top

[S36] C++：unordered_map
来源：http://nvl.smart0.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://loy.chenzaomai.com

[S37] C++：set
来源：http://hol.birdmap.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tyg.vehdjk.com

[S38] C++：排序
来源：http://vzz.cheryme.top

std::sort(v.begin(), v.end());
来源：http://ftn.9152youxi.cn

[S39] C++：自定义比较器排序
来源：http://rmf.jqgufenzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uol.9152youxi.cn

[S40] C++：查找元素
来源：http://kff.daxiang520.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://muj.yvedp.cn

[S41] C++：类与构造函数
来源：http://seg.vqdsnc.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ryx.sufxvd.cn

[S42] C++：继承与虚函数
来源：http://rvb.nwbrower.top

class B : public Base { public: void f() override {} };
来源：http://kvg.yvedp.cn

[S43] C++：智能指针
来源：http://ktc.uphjek.com

auto p = std::make_unique<int>(5);
来源：http://ajj.hammf.cn

[S44] C++：引用传参
来源：http://nec.xingfuxueyuan.xyz

void inc(int &x) { ++x; }
来源：http://law.shangyingyoupin.top

[S45] C++：lambda
来源：http://adk.sysykeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://wam.9152youxi.cn

[S46] C++：函数模板
来源：http://cce.guannengcc.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zen.haohaochexian.top

[S47] C++：结构化绑定遍历
来源：http://rze.hywenlv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vzy.fanxiaobao.xyz

[S48] C++：逐行读文件
来源：http://fvz.jinghuilouyu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tst.aizwys.cn

while (std::getline(in, line)) { }
来源：http://tmx.hnxiangtu.top

[S49] C++：写文件
来源：http://mqu.ydjk.org.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gaz.bbcook.cn

[S50] C++：格式化数字
来源：http://dzc.hongshengwenyu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://keo.kuanghao11.cn

[S51] C++：显式类型转换
来源：http://zhh.mhx1999.top

static_cast<double>(a) / b
来源：http://ini.nanxinkj.top

[S52] C++：const 与 noexcept
来源：http://wdi.hammf.cn

int size() const noexcept { return n_; }
来源：http://koz.jqgfzy.top

[S53] C++：移动语义
来源：http://pcw.jianghu66.top

std::vector<int> w = std::move(v);
来源：http://fkm.zdbjq.cn

[S54] C++：异常处理
来源：http://mvn.zhaomingkeji.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vhn.gzhubu.top

[S55] C++：结构化绑定
来源：http://wpn.yongpay.top

auto [a, b] = std::make_pair(1, 2);
来源：http://abi.sweek.top

[S56] C++：optional
来源：http://ina.316326.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wep.daxiang520.top

[S57] C++：编译期常量
来源：http://mwa.fktsv.cn

constexpr int N = 10;
来源：http://yhl.dashuyun.cn

[S58] C++：命名空间
来源：http://rri.jqgfzy.top

namespace ns { int f() { return 1; } }
来源：http://oux.jqgufenzy.top

[S59] C++：静态断言
来源：http://fre.guannengcc.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://odr.ywan-chungtsiang.top

[S60] C++：遍历并删除元素
来源：http://lpc.52xcode.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lxp.jinyuanbaomall.cn

================================================================================
来源：http://nrb.shzxlz.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gmi.yj20258888.top

================================================================================
来源：http://xsh.shanyushiyangkeji.top

[T01] Kotlin：Hello World
来源：http://lpn.fengsongda.top

println("Hello")
来源：http://vrt.yuxming.cn

[T02] Kotlin：变量
来源：http://onf.c1oappe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ums.chenzaomai.com

[T03] Kotlin：字符串模板
来源：http://gpf.pengpengdd.cyou

"值: $b"
来源：http://jcb.yongpay.top

[T04] Kotlin：空安全
来源：http://byn.smart0.xyz

val n: String? = null;  n?.length
来源：http://uea.hammf.cn

[T05] Kotlin：when 表达式
来源：http://ddw.daria6918.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sto.jinqigufen.top

[T06] Kotlin：集合映射
来源：http://ath.xziqi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ckt.tarul.cn

[T07] Kotlin：集合过滤
来源：http://axq.haohaochexian.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://blo.pengpengdd.cyou

[T08] Kotlin：数据类
来源：http://hxf.cashguo.top

data class User(val name: String, val age: Int)
来源：http://qjz.sysykeji.top

[T09] Kotlin：扩展函数
来源：http://hvc.nanxuanxn.top

fun String.exclaim() = this + "!"
来源：http://efo.gaohongyu789.top

[T10] Kotlin：默认参数
来源：http://bcm.cucudq.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://waa.xylfe.cn

[T11] Kotlin：协程
来源：http://ukm.feifeiyinyue.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://zln.dashuyun.cn

[T12] Kotlin：解构声明
来源：http://qpy.shuidangran.top

val (a, b) = Pair(1, 2)
来源：http://ovn.birdmap.top

[T13] Kotlin：只读 Map
来源：http://tmq.hongshengwenyu.top

val m = mapOf("a" to 1)
来源：http://ipi.daria6918.cn

[T14] Kotlin：循环
来源：http://tvx.shangyingyoupin.top

for (i in 1..10) println(i)
来源：http://oln.nwbrower.top

[T15] Kotlin：接口
来源：http://qkg.meibo888.top

interface Shape { fun area(): Double }
来源：http://ugb.dianchejie.cn

[T16] Swift：Hello World
来源：http://rov.bbcook.cn

print("Hello")
来源：http://cmr.sufxvd.cn

[T17] Swift：变量与常量
来源：http://fgb.xuanzx.com

var a = 1;  let b = 2
来源：http://ept.shanyushiyangkeji.top

[T18] Swift：字符串插值
来源：http://vgg.uphjek.com

"值: \(b)"
来源：http://opj.316326.xyz

[T19] Swift：可选绑定
来源：http://fgn.chenzaomai.com

if let n = opt { print(n) }
来源：http://nwu.aizwys.cn

[T20] Swift：数组操作
来源：http://yiw.sufxvd.cn

var a = [1, 2, 3];  a.append(4)
来源：http://exv.yvedp.cn

[T21] Swift：遍历
来源：http://aja.cucudq.cn

for x in a { print(x) }
来源：http://gvq.hnqzz.top

[T22] Swift：字典
来源：http://hln.gaohongyu789.top

var d = ["a": 1];  d["b"] = 2
来源：http://ppw.hysaishi.cn

[T23] Swift：函数
来源：http://uek.xinyue.icu

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mkp.9152youxi.cn

[T24] Swift：闭包
来源：http://kqa.kuanghao11.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bou.yuanzhike.top

[T25] Swift：结构体
来源：http://xll.hywenlv.cn

struct P { var x: Int }
来源：http://obk.sufxvd.cn

[T26] Swift：类与重写
来源：http://typ.yuanzhike.top

class A: Base { override func f() {} }
来源：http://dfe.jinghuilouyu.cn

[T27] Swift：错误处理
来源：http://ver.gotoacloud.top

do { try f() } catch { print(error) }
来源：http://ydu.fehbvm.com

[T28] Swift：枚举
来源：http://rwg.shzxlz.cn

enum Color { case red, green }
来源：http://ywh.jqgufenzy.top

[T29] Swift：guard 提前返回
来源：http://vit.feifeiyinyue.top

guard let x = opt else { return }
来源：http://tju.ydzc1.top

[T30] Swift：协议
来源：http://lsu.chenzaomai.com

protocol Shape { func area() -> Double }
来源：http://cxf.shanyushiyangtech.top

[T31] Lua：Hello World
来源：http://rsg.vehdjk.com

print("Hello")
来源：http://jtw.jqgfzy.top

[T32] Lua：局部变量
来源：http://xfg.epnwcf.com

local a = 1
来源：http://kun.kuanghao11.cn

[T33] Lua：表（数组）
来源：http://mls.smart0.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://xux.fzhhl.top

[T34] Lua：遍历表
来源：http://lfm.fengsongda.top

for i, v in ipairs(t) do print(i, v) end
来源：http://jzx.uphjek.com

[T35] Lua：字典表
来源：http://tyh.xziqi.cn

local d = { a = 1 };  d.b = 2
来源：http://trp.52xcode.cn

[T36] Lua：函数
来源：http://xvv.yanxiufei.cn

function add(a, b) return a + b end
来源：http://jbz.cheryme.top

[T37] Lua：字符串拼接
来源：http://xsh.yfazqb.com

"a" .. "b"
来源：http://nte.yangfankeji.com

[T38] Lua：条件
来源：http://ucn.chenzaomai.com

if x > 0 then print("正") end
来源：http://ydw.zhixingplan.top

[T39] Lua：模式匹配
来源：http://vhi.daria6918.cn

string.find(s, "%d+")
来源：http://rhx.vqdsnc.cn

[T40] Lua：元表
来源：http://vgo.ctjpmb.com

setmetatable({}, { __index = base })
来源：http://vur.sweek.top

[T41] Perl：Hello World
来源：http://jht.hnxiangtu.top

print "Hello\n";
来源：http://rmm.zhoulong.xyz

[T42] Perl：变量类型
来源：http://owx.shangyingyoupin.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uxy.cheryme.top

[T43] Perl：字符串插值
来源：http://lvv.iojbl.cn

"值: $a"
来源：http://xqn.xuanzx.com

[T44] Perl：条件
来源：http://qne.shuidangran.top

if ($a > 0) { print "正"; }
来源：http://bfz.jiagoushi.top

[T45] Perl：数组遍历
来源：http://dzp.svipenyu.cn

for my $x (@arr) { print $x; }
来源：http://wuf.9152youxi.cn

[T46] Perl：哈希操作
来源：http://xga.dianchejie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://imt.wangdashe.top

[T47] Perl：正则捕获
来源：http://lvl.tanke756.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://jqw.zhoulong.xyz

[T48] Perl：正则替换
来源：http://wmg.gaohongyu789.top

$s =~ s/old/new/g;
来源：http://fne.xylfe.cn

[T49] Perl：函数
来源：http://kcg.316326.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qem.shanyushiyangtech.top

[T50] Perl：逐行读文件
来源：http://yob.chenjidiqi.icu

open my $fh, "<", "a.txt" or die $!;
来源：http://sda.pengpengdd.cyou

while (my $line = <$fh>) { print $line; }
来源：http://kte.quarkkingdee.top

[T51] Scala：Hello World
来源：http://cwl.vqdsnc.cn

println("Hello")
来源：http://hzf.epnwcf.com

[T52] Scala：变量
来源：http://lmm.xingfuxueyuan.xyz

val a = 1;  var b = 2
来源：http://sny.hnxiangtu.top

[T53] Scala：字符串插值
来源：http://wau.bjfxy.top

s"值: $b"
来源：http://vpi.chenjidiqi.icu

[T54] Scala：集合映射
来源：http://wny.andypj.xyz

List(1, 2, 3).map(_ * 2)
来源：http://jqj.ybcxt.top

[T55] Scala：集合过滤
来源：http://wej.sxryk.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jgl.bbcook.cn

[T56] Scala：样例类
来源：http://saf.zhiwuduotai.top

case class User(name: String, age: Int)
来源：http://ymw.yj202588.top

[T57] Scala：模式匹配
来源：http://pnl.yuanzhike.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://xeb.xuetiantiany.cn

[T58] Scala：函数定义
来源：http://ant.cashguo.top

def add(a: Int, b: Int): Int = a + b
来源：http://iii.chenjidiqi.icu

[T59] Scala：循环
来源：http://ihe.sysykeji.top

for (i <- 1 to 10) println(i)
来源：http://jrb.ctjpmb.com

[T60] Scala：折叠
来源：http://urt.kuanghao11.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://scl.yuxming.cn

================================================================================
来源：http://seq.jianghu66.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pzn.pengpengdd.cyou

================================================================================
来源：http://kqt.ppjwa.cn

[U01] Py：创建虚拟环境
来源：http://vxo.meibo888.top

python -m venv .venv && source .venv/bin/activate
来源：http://lyr.316326.xyz

[U02] Py：导出 / 安装依赖
来源：http://abu.wangshuangyany.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ddi.ehwqpu.com


<!-- 参考信息 -->