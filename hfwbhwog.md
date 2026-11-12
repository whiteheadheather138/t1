代发 wailian999

free -h;  ps aux | grep nginx
来源：http://kif.ivvv.top

[R64] 结束进程
来源：http://ljr.uphjek.com

kill -9 $(pgrep -f app.py)
来源：http://ioe.sufxvd.cn

[R65] 查看端口占用
来源：http://uwx.ywan-chungtsiang.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ook.aibaodan.cn

[R66] 定时任务
来源：http://ijz.ydzc1.top

crontab -e;  crontab -l
来源：http://gug.sufxvd.cn

[R67] 生成随机十六进制串
来源：http://vov.xylfe.cn

openssl rand -hex 16
来源：http://nse.vqdsnc.cn

[R68] 计算文件校验值
来源：http://qpa.ybcxt.top

sha256sum a.txt;  md5sum a.txt
来源：http://sfv.ivvv.top

[R69] 生成随机密码
来源：http://ust.ywan-chungtsiang.top

head -c 16 /dev/urandom | base64
来源：http://zig.tarul.cn

[R70] 时间戳与互转
来源：http://ybq.jinghuilouyu.cn

date +%s;  date -d @1700000000
来源：http://kdt.hammf.cn

[R71] 日期格式化
来源：http://tre.sjlbkw.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ben.c1oappe.top

[R72] 等待端口就绪
来源：http://cht.kuanghao11.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nli.xylfe.cn

[R73] 分割大日志
来源：http://xvn.zhongyouzk.top

split -l 1000 big.log part_
来源：http://auy.shangyingyoupin.top

[R74] 批量重命名
来源：http://rlo.zhongyouzk.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kkm.9152youxi.cn

[R75] 导出环境变量
来源：http://khx.zdqjudy.top

export PATH="$HOME/bin:$PATH"
来源：http://krk.bjfxy.top

[R76] 使用临时文件
来源：http://spl.andypj.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nav.jqgufenzy.top

[R77] 读取用户输入
来源：http://hns.xylfe.cn

read -rp "请输入: " ans
来源：http://ydj.cdnleiting.top

[R78] 交互式菜单
来源：http://toe.tanke756.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ndf.xziqi.cn

[R79] 解析命令行选项
来源：http://xow.9152youxi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eza.mhx1999.top

[R80] 查看脚本执行耗时
来源：http://ghn.hesvh.cn

time ./run.sh
来源：http://zjw.jyoumei.cn

================================================================================
来源：http://vqw.chenzaomai.com

S. C / C++ 专题
来源：http://zsz.fanxiaobao.xyz

================================================================================
来源：http://nlo.guowangkeji.top

[S01] C：Hello World
来源：http://hzh.daria6918.cn

#include <stdio.h>
来源：http://dqy.smart0.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://cgb.sxryk.cn

[S02] C：变量与格式化输出
来源：http://lio.fehbvm.com

int a = 10; printf("%d\n", a);
来源：http://fmx.zdqjudy.top

[S03] C：读入整数
来源：http://tzh.guannengcc.top

int x; scanf("%d", &x);
来源：http://nwd.zdqjudy.top

[S04] C：字符串复制
来源：http://lrt.guowangkeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://fsg.jinyuanbaomall.cn

[S05] C：字符串长度
来源：http://cof.zhoulong.xyz

strlen(s)
来源：http://agu.nanxinkj.top

[S06] C：字符串比较
来源：http://zrk.andypj.xyz

strcmp(a, b) == 0
来源：http://pmz.zhongyouzk.top

[S07] C：数组遍历求和
来源：http://wai.uphjek.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jow.yj20258.top

[S08] C：动态内存分配与释放
来源：http://wbn.nanxuanxn.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ysr.jiagoushi.top

[S09] C：结构体定义与初始化
来源：http://gfo.ydzc1.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qeb.xziqi.cn

[S10] C：指针与解引用
来源：http://uez.jqgfzy.top

int *p = &a;  *p = 5;
来源：http://jsk.vehdjk.com

[S11] C：逐行读文件
来源：http://zxl.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "r");
来源：http://xos.hongshengwenyu.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://rct.hesvh.cn

fclose(f);
来源：http://aga.hnxiangtu.top

[S12] C：写文件
来源：http://szb.pengpengdd.cyou

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kxa.0kj1m.cn

[S13] C：宏定义
来源：http://uxg.sysykeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cjj.birdmap.top

[S14] C：枚举
来源：http://zcv.fktsv.cn

enum Color { RED, GREEN, BLUE };
来源：http://vzc.hywenlv.cn

[S15] C：类型转换
来源：http://xnm.fehbvm.com

(double) a / b
来源：http://tga.yvedp.cn

[S16] C：位操作置位
来源：http://dpx.andypj.xyz

x |= (1 << 3);
来源：http://ett.jyoumei.cn

[S17] C：安全拼接字符串
来源：http://zxe.aizwys.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wcd.fzhhl.top

[S18] C：命令行参数
来源：http://jtb.shangyingyoupin.top

int main(int argc, char **argv)
来源：http://lfh.pengpengdd.cyou

[S19] C：快速排序
来源：http://nvi.316326.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://qhp.yuxming.cn

[S20] C：二分查找
来源：http://bys.fanxiaobao.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zfo.zhixingplan.top

[S21] C：字符类别判断
来源：http://dhu.jinyuanbaomall.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jxr.haohaochexian.top

[S22] C：字符串转数字
来源：http://gie.aibaodan.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ihe.tianlin.xyz

[S23] C：随机数
来源：http://gfv.zhongyouzk.top

srand(time(NULL));  int r = rand() % 100;
来源：http://dwe.hcnkem.com

[S24] C：获取本地时间
来源：http://wbg.cdnleiting.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ygb.shuidangran.top

[S25] C：内存拷贝
来源：http://gfs.pengpengdd.cyou

memcpy(dst, src, n);
来源：http://liq.aizwys.cn

[S26] C：内存清零
来源：http://jxo.cqqwz.cn

memset(a, 0, sizeof a);
来源：http://tfz.ywan-chungtsiang.top

[S27] C：定义常量
来源：http://jkk.hammf.cn

const double PI = 3.14159;
来源：http://rhu.xylfe.cn

[S28] C：静态变量
来源：http://dbk.pengpengdd.cyou

static int counter = 0;
来源：http://gle.daria6918.cn

[S29] C：变参函数
来源：http://hng.jiagoushi.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xfi.xingfuxueyuan.xyz

[S30] C：头文件保护
来源：http://ujz.zycfv.cn

#ifndef X_H
来源：http://qnj.hnqzz.top

#define X_H
来源：http://rut.cashguo.top

#endif
来源：http://lds.wangdashe.top

[S31] C++：Hello World
来源：http://klw.ydzc1.top

#include <iostream>
来源：http://ahz.hfpthk.cn

int main() { std::cout << "Hello\n"; }
来源：http://mid.xuanzx.com

[S32] C++：字符串
来源：http://rcl.ctjpmb.com

std::string s = "hi";  s += "!";
来源：http://ezm.aibaodan.cn

[S33] C++：vector 增删
来源：http://ugf.cqqwz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mbi.zhongyouzk.top

[S34] C++：遍历 vector
来源：http://zug.haohaochexian.top

for (auto &x : v) { std::cout << x; }
来源：http://ovv.chenlongwang.top

[S35] C++：map
来源：http://mvk.gaohongyu789.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fes.zhengqikj.top

[S36] C++：unordered_map
来源：http://epw.hnqzz.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wtt.andypj.xyz

[S37] C++：set
来源：http://qrv.kuanghao11.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ick.cqqwz.cn

[S38] C++：排序
来源：http://lzf.haohaochexian.top

std::sort(v.begin(), v.end());
来源：http://sgj.zhengqikj.top

[S39] C++：自定义比较器排序
来源：http://nea.guannengcc.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zqm.xuetiantiany.cn

[S40] C++：查找元素
来源：http://cre.sweek.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fcc.ctjpmb.com

[S41] C++：类与构造函数
来源：http://oif.wangdashe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xbf.yueranfly.top

[S42] C++：继承与虚函数
来源：http://srp.tanke756.top

class B : public Base { public: void f() override {} };
来源：http://usx.yuanzhike.top

[S43] C++：智能指针
来源：http://cbq.sysykeji.top

auto p = std::make_unique<int>(5);
来源：http://vby.ydjk.org.cn

[S44] C++：引用传参
来源：http://gkh.epnwcf.com

void inc(int &x) { ++x; }
来源：http://geb.mhx1999.top

[S45] C++：lambda
来源：http://gvj.yuanzhike.top

auto add = [](int a, int b) { return a + b; };
来源：http://vyb.shzxlz.cn

[S46] C++：函数模板
来源：http://sup.guannengcc.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dfa.c1oappe.top

[S47] C++：结构化绑定遍历
来源：http://igj.ppjwa.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://slf.yj202588.top

[S48] C++：逐行读文件
来源：http://ofw.yvedp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bwi.guannengcc.top

while (std::getline(in, line)) { }
来源：http://eqc.shanyushiyangtech.top

[S49] C++：写文件
来源：http://ybn.epnwcf.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dfe.hammf.cn

[S50] C++：格式化数字
来源：http://qvx.hesvh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://iue.redwolf501.top

[S51] C++：显式类型转换
来源：http://pra.fengsongda.top

static_cast<double>(a) / b
来源：http://kwk.guowangkeji.top

[S52] C++：const 与 noexcept
来源：http://yhg.wangshuangyany.cn

int size() const noexcept { return n_; }
来源：http://fvi.nanxuanxn.top

[S53] C++：移动语义
来源：http://iqg.zdbjq.cn

std::vector<int> w = std::move(v);
来源：http://zsg.shanyushiyangtech.top

[S54] C++：异常处理
来源：http://zpc.jqgfzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fpg.yonumen.top

[S55] C++：结构化绑定
来源：http://fhd.yuxming.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vwt.ybcxt.top

[S56] C++：optional
来源：http://uwb.aizwys.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wge.uphjek.com

[S57] C++：编译期常量
来源：http://qde.zhoulong.xyz

constexpr int N = 10;
来源：http://aft.aibaodan.cn

[S58] C++：命名空间
来源：http://pxs.bjfxy.top

namespace ns { int f() { return 1; } }
来源：http://qcj.yonumen.top

[S59] C++：静态断言
来源：http://wyh.sjlbkw.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yov.jinqigufen.top

[S60] C++：遍历并删除元素
来源：http://nzl.tianlin.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cxy.jinghuilouyu.cn

================================================================================
来源：http://mqo.vehdjk.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ynu.tianlin.xyz

================================================================================
来源：http://xse.ctjpmb.com

[T01] Kotlin：Hello World
来源：http://anz.cucudq.cn

println("Hello")
来源：http://uiu.fzhhl.top

[T02] Kotlin：变量
来源：http://gmb.dianchejie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ark.xinyue.icu

[T03] Kotlin：字符串模板
来源：http://orq.shanyushiyangtech.top

"值: $b"
来源：http://thf.yueranfly.top

[T04] Kotlin：空安全
来源：http://bgr.hongshengwenyu.top

val n: String? = null;  n?.length
来源：http://zqv.cashguo.top

[T05] Kotlin：when 表达式
来源：http://whp.shanyushiyangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gte.316326.xyz

[T06] Kotlin：集合映射
来源：http://txj.52xcode.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nwb.fktsv.cn

[T07] Kotlin：集合过滤
来源：http://pbs.jinyuanbaomall.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ptg.hysaishi.cn

[T08] Kotlin：数据类
来源：http://usb.dianchejie.cn

data class User(val name: String, val age: Int)
来源：http://nlv.yueranfly.top

[T09] Kotlin：扩展函数
来源：http://lou.nwbrower.top

fun String.exclaim() = this + "!"
来源：http://iqo.andypj.xyz

[T10] Kotlin：默认参数
来源：http://ygz.ywan-chungtsiang.top

fun greet(name: String = "World") = "Hi $name"
来源：http://gos.chenlongwang.top

[T11] Kotlin：协程
来源：http://nfi.shuidangran.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://nnw.nanxuanxn.top

[T12] Kotlin：解构声明
来源：http://ojx.jqgufenzy.top

val (a, b) = Pair(1, 2)
来源：http://fzb.xinyue.icu

[T13] Kotlin：只读 Map
来源：http://snm.yonumen.top

val m = mapOf("a" to 1)
来源：http://daj.jinghuilouyu.cn

[T14] Kotlin：循环
来源：http://bet.ehwqpu.com

for (i in 1..10) println(i)
来源：http://jge.nanxinkj.top

[T15] Kotlin：接口
来源：http://thz.quarkkingdee.top

interface Shape { fun area(): Double }
来源：http://fzj.hesvh.cn

[T16] Swift：Hello World
来源：http://xar.nanxinkj.top

print("Hello")
来源：http://mle.vehdjk.com

[T17] Swift：变量与常量
来源：http://afm.yuanzhike.top

var a = 1;  let b = 2
来源：http://kza.daxiang520.top

[T18] Swift：字符串插值
来源：http://lad.tianlin.xyz

"值: \(b)"
来源：http://kcu.jqgufenzy.top

[T19] Swift：可选绑定
来源：http://znw.xylfe.cn

if let n = opt { print(n) }
来源：http://hrf.nanxuanxn.top

[T20] Swift：数组操作
来源：http://exm.cashguo.top

var a = [1, 2, 3];  a.append(4)
来源：http://yzj.cheryme.top

[T21] Swift：遍历
来源：http://bjv.bjfxy.top

for x in a { print(x) }
来源：http://gzy.zhongyouzk.top

[T22] Swift：字典
来源：http://umi.fanxiaobao.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://fjf.vehdjk.com

[T23] Swift：函数
来源：http://esn.xinyue.icu

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://all.andypj.xyz

[T24] Swift：闭包
来源：http://kmr.zhengqikj.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://adc.redwolf501.top

[T25] Swift：结构体
来源：http://qrw.yuxming.cn

struct P { var x: Int }
来源：http://ibf.zhaomingkeji.xyz

[T26] Swift：类与重写
来源：http://grj.mhx1999.top

class A: Base { override func f() {} }
来源：http://geo.dashuyun.cn

[T27] Swift：错误处理
来源：http://zph.bbcook.cn

do { try f() } catch { print(error) }
来源：http://ptu.pycfn.com

[T28] Swift：枚举
来源：http://hza.yuanzhike.top

enum Color { case red, green }
来源：http://hun.cqqwz.cn

[T29] Swift：guard 提前返回
来源：http://ywt.316326.xyz

guard let x = opt else { return }
来源：http://xez.xylfe.cn

[T30] Swift：协议
来源：http://vbv.jinyuanbaomall.cn

protocol Shape { func area() -> Double }
来源：http://bgu.wangdashe.top

[T31] Lua：Hello World
来源：http://yzt.dianchejie.cn

print("Hello")
来源：http://ztd.cucudq.cn

[T32] Lua：局部变量
来源：http://wmm.iojbl.cn

local a = 1
来源：http://ezk.xziqi.cn

[T33] Lua：表（数组）
来源：http://kdy.nanxinkj.top

local t = {1, 2, 3};  t[4] = 4
来源：http://umr.xinyue.icu

[T34] Lua：遍历表
来源：http://uyr.nanxinkj.top

for i, v in ipairs(t) do print(i, v) end
来源：http://efx.cqqwz.cn

[T35] Lua：字典表
来源：http://ddd.jlsjyb.cn

local d = { a = 1 };  d.b = 2
来源：http://cbm.feifeiyinyue.top

[T36] Lua：函数
来源：http://csy.zdqjudy.top

function add(a, b) return a + b end
来源：http://mbs.jqgufenzy.top

[T37] Lua：字符串拼接
来源：http://gfd.gotoacloud.top

"a" .. "b"
来源：http://tqb.fehbvm.com

[T38] Lua：条件
来源：http://hlf.hcnkem.com

if x > 0 then print("正") end
来源：http://sdw.jlsjyb.cn

[T39] Lua：模式匹配
来源：http://nsf.vehdjk.com

string.find(s, "%d+")
来源：http://lob.redwolf501.top

[T40] Lua：元表
来源：http://ftw.jqgufenzy.top

setmetatable({}, { __index = base })
来源：http://hec.chenlongwang.top

[T41] Perl：Hello World
来源：http://qko.fktsv.cn

print "Hello\n";
来源：http://ngq.yuanzhike.top

[T42] Perl：变量类型
来源：http://yoe.gzhubu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://obq.uphjek.com

[T43] Perl：字符串插值
来源：http://jrr.fanxiaobao.xyz

"值: $a"
来源：http://wis.dianchejie.cn

[T44] Perl：条件
来源：http://mui.tarul.cn

if ($a > 0) { print "正"; }
来源：http://lhc.chenjidiqi.icu

[T45] Perl：数组遍历
来源：http://yph.hfpthk.cn

for my $x (@arr) { print $x; }
来源：http://gll.jianghu66.top

[T46] Perl：哈希操作
来源：http://utk.jinqigfzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://iru.zhongyouzk.top

[T47] Perl：正则捕获
来源：http://zez.zhoulong.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://qrz.yj202588.top

[T48] Perl：正则替换
来源：http://ijm.gotoacloud.top

$s =~ s/old/new/g;
来源：http://xlq.yuanzhike.top

[T49] Perl：函数
来源：http://uol.shanyushiyangtech.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://iuy.yueranfly.top

[T50] Perl：逐行读文件
来源：http://ybf.tian-w.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vff.xuanzx.com

while (my $line = <$fh>) { print $line; }
来源：http://oyf.daria6918.cn

[T51] Scala：Hello World
来源：http://sov.smart0.xyz

println("Hello")
来源：http://plw.hysaishi.cn

[T52] Scala：变量
来源：http://qhk.ywan-chungtsiang.top

val a = 1;  var b = 2
来源：http://hqq.pengpengdd.cyou

[T53] Scala：字符串插值
来源：http://mjz.hesvh.cn

s"值: $b"
来源：http://awx.sweek.top

[T54] Scala：集合映射
来源：http://end.gotoacloud.top

List(1, 2, 3).map(_ * 2)
来源：http://ezp.zycfv.cn

[T55] Scala：集合过滤
来源：http://mlw.yangfankeji.com

List(1, 2, 3).filter(_ > 1)
来源：http://jvr.jqgfzy.top

[T56] Scala：样例类
来源：http://zem.zhixingplan.top

case class User(name: String, age: Int)
来源：http://qzx.pengpengdd.cyou

[T57] Scala：模式匹配
来源：http://krx.vqdsnc.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ipm.zhengqikj.top

[T58] Scala：函数定义
来源：http://zyi.haohaochexian.top

def add(a: Int, b: Int): Int = a + b
来源：http://gks.pycfn.com

[T59] Scala：循环
来源：http://uxc.cqqwz.cn

for (i <- 1 to 10) println(i)
来源：http://qpr.sjlbkw.cn

[T60] Scala：折叠
来源：http://wvt.redwolf501.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ilb.zycfv.cn

================================================================================
来源：http://vfy.ywan-chungtsiang.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wmu.tianlin.xyz

================================================================================
来源：http://heb.fzhhl.top

[U01] Py：创建虚拟环境
来源：http://vlf.zhongyouzk.top

python -m venv .venv && source .venv/bin/activate
来源：http://whn.zhijiandao.cn

[U02] Py：导出 / 安装依赖
来源：http://pok.havefunace.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lkx.xuetiantiany.cn

[U03] Py：加载 .env 配置
来源：http://fyp.aibaodan.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cab.gotoacloud.top

[U04] Py：变量调试打印
来源：http://dhe.yj20258.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hrq.guowangkeji.top


<!-- 参考信息 -->