代发 wailian999

df -h;  du -sh *
来源：http://dju.hnqzz.top

[R62] 找最占空间的文件
来源：http://wny.zhixingplan.top

du -ah . | sort -rh | head -10
来源：http://hcr.yuanzhike.top

[R63] 内存与进程
来源：http://tkb.guannengcc.top

free -h;  ps aux | grep nginx
来源：http://ngg.zdbjq.cn

[R64] 结束进程
来源：http://vch.yuxming.cn

kill -9 $(pgrep -f app.py)
来源：http://rkx.shuidangran.top

[R65] 查看端口占用
来源：http://ini.sjlbkw.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cdt.yanxiufei.cn

[R66] 定时任务
来源：http://tik.mhx1999.top

crontab -e;  crontab -l
来源：http://pgd.jqgufenzy.top

[R67] 生成随机十六进制串
来源：http://klq.wangshuangyany.cn

openssl rand -hex 16
来源：http://gdv.ivvv.top

[R68] 计算文件校验值
来源：http://juw.bjfxy.top

sha256sum a.txt;  md5sum a.txt
来源：http://jdd.ydjk.org.cn

[R69] 生成随机密码
来源：http://nno.yanxiufei.cn

head -c 16 /dev/urandom | base64
来源：http://bge.ctjpmb.com

[R70] 时间戳与互转
来源：http://seq.bjfxy.top

date +%s;  date -d @1700000000
来源：http://leo.cucudq.cn

[R71] 日期格式化
来源：http://jdz.vehdjk.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://sxj.kuanghao11.cn

[R72] 等待端口就绪
来源：http://ubs.zhongyouzk.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jug.gaohongyu789.top

[R73] 分割大日志
来源：http://aov.yfazqb.com

split -l 1000 big.log part_
来源：http://zpz.birdmap.top

[R74] 批量重命名
来源：http://rsc.haohaochexian.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wqf.yj20258.top

[R75] 导出环境变量
来源：http://gzz.pycfn.com

export PATH="$HOME/bin:$PATH"
来源：http://txy.yfazqb.com

[R76] 使用临时文件
来源：http://nco.hcnkem.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lpn.iojbl.cn

[R77] 读取用户输入
来源：http://nqr.cucudq.cn

read -rp "请输入: " ans
来源：http://vri.nwbrower.top

[R78] 交互式菜单
来源：http://lxg.ctjpmb.com

select opt in a b c; do echo "$opt"; break; done
来源：http://kci.sysykeji.top

[R79] 解析命令行选项
来源：http://iek.andypj.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nbf.hesvh.cn

[R80] 查看脚本执行耗时
来源：http://pmm.jinyuanbaomall.cn

time ./run.sh
来源：http://jfh.jinqigfzy.top

================================================================================
来源：http://hao.hammf.cn

S. C / C++ 专题
来源：http://byd.snrcjt.cn

================================================================================
来源：http://dct.aibaodan.cn

[S01] C：Hello World
来源：http://mws.jyoumei.cn

#include <stdio.h>
来源：http://vdl.mhx1999.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://cjq.redwolf501.top

[S02] C：变量与格式化输出
来源：http://gvs.jianghu66.top

int a = 10; printf("%d\n", a);
来源：http://fkp.hnqzz.top

[S03] C：读入整数
来源：http://huo.snrcjt.cn

int x; scanf("%d", &x);
来源：http://hjw.chenzaomai.com

[S04] C：字符串复制
来源：http://hip.zhoulong.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://sxi.gaohongyu789.top

[S05] C：字符串长度
来源：http://tbx.ivvv.top

strlen(s)
来源：http://tlc.hesvh.cn

[S06] C：字符串比较
来源：http://faf.jinghuilouyu.cn

strcmp(a, b) == 0
来源：http://myq.tianlin.xyz

[S07] C：数组遍历求和
来源：http://hmv.aizwys.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pbu.iojbl.cn

[S08] C：动态内存分配与释放
来源：http://per.gotoacloud.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sct.ydjk.org.cn

[S09] C：结构体定义与初始化
来源：http://noq.ydjk.org.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://eml.ivvv.top

[S10] C：指针与解引用
来源：http://xxj.xuanzx.com

int *p = &a;  *p = 5;
来源：http://zyx.zhijiandao.cn

[S11] C：逐行读文件
来源：http://ixn.zdqjudy.top

FILE *f = fopen("a.txt", "r");
来源：http://mgr.andypj.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://rlc.xziqi.cn

fclose(f);
来源：http://shc.hywenlv.cn

[S12] C：写文件
来源：http://xda.zhongyouzk.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rol.tanke756.top

[S13] C：宏定义
来源：http://xek.epnwcf.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sqj.wangshuangyany.cn

[S14] C：枚举
来源：http://rsr.xuanzx.com

enum Color { RED, GREEN, BLUE };
来源：http://oyt.aizwys.cn

[S15] C：类型转换
来源：http://vwd.shanyushiyangtech.top

(double) a / b
来源：http://peh.sweek.top

[S16] C：位操作置位
来源：http://tff.xylfe.cn

x |= (1 << 3);
来源：http://dmv.epnwcf.com

[S17] C：安全拼接字符串
来源：http://ycn.jianghu66.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lgy.jlsjyb.cn

[S18] C：命令行参数
来源：http://zyd.chenjidiqi.icu

int main(int argc, char **argv)
来源：http://peq.zhijiandao.cn

[S19] C：快速排序
来源：http://fid.shanyushiyangtech.top

qsort(a, n, sizeof(int), cmp);
来源：http://mpj.sjlbkw.cn

[S20] C：二分查找
来源：http://tnz.hcnkem.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://spq.svipenyu.cn

[S21] C：字符类别判断
来源：http://dzw.wangdashe.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xru.fanxiaobao.xyz

[S22] C：字符串转数字
来源：http://nvx.smart0.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://ini.bjfxy.top

[S23] C：随机数
来源：http://bmq.tian-w.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qpi.gaohongyu789.top

[S24] C：获取本地时间
来源：http://eej.9152youxi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xfi.ydzc1.top

[S25] C：内存拷贝
来源：http://zyl.hnxiangtu.top

memcpy(dst, src, n);
来源：http://hwp.hysaishi.cn

[S26] C：内存清零
来源：http://aba.ydzc1.top

memset(a, 0, sizeof a);
来源：http://ogx.redwolf501.top

[S27] C：定义常量
来源：http://zpr.jinyuanbaomall.cn

const double PI = 3.14159;
来源：http://uqw.shanyushiyangkeji.top

[S28] C：静态变量
来源：http://jvm.yonumen.top

static int counter = 0;
来源：http://zyh.sysykeji.top

[S29] C：变参函数
来源：http://ocz.yj202588.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nvn.haohaochexian.top

[S30] C：头文件保护
来源：http://sda.gogol.net.cn

#ifndef X_H
来源：http://egh.ctjpmb.com

#define X_H
来源：http://pvr.guowangkeji.top

#endif
来源：http://bkt.52xcode.cn

[S31] C++：Hello World
来源：http://wpi.aibaodan.cn

#include <iostream>
来源：http://xbl.tianlin.xyz

int main() { std::cout << "Hello\n"; }
来源：http://nsx.hongshengwenyu.top

[S32] C++：字符串
来源：http://run.fktsv.cn

std::string s = "hi";  s += "!";
来源：http://lgv.feifeiyinyue.top

[S33] C++：vector 增删
来源：http://kcn.smart0.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hxf.xuetiantiany.cn

[S34] C++：遍历 vector
来源：http://mtp.xinyue.icu

for (auto &x : v) { std::cout << x; }
来源：http://kmz.cdnleiting.top

[S35] C++：map
来源：http://dex.zhijiandao.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fbw.yanxiufei.cn

[S36] C++：unordered_map
来源：http://byf.yvedp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rgj.c1oappe.top

[S37] C++：set
来源：http://chs.fanxiaobao.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ryn.wangdashe.top

[S38] C++：排序
来源：http://rzs.gaohongyu789.top

std::sort(v.begin(), v.end());
来源：http://nwv.ivvv.top

[S39] C++：自定义比较器排序
来源：http://otg.cucudq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mqj.jianghu66.top

[S40] C++：查找元素
来源：http://jal.gotoacloud.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fdu.yuanzhike.top

[S41] C++：类与构造函数
来源：http://wlm.wangdashe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qoe.cheryme.top

[S42] C++：继承与虚函数
来源：http://opl.jyoumei.cn

class B : public Base { public: void f() override {} };
来源：http://tao.guowangkeji.top

[S43] C++：智能指针
来源：http://lkd.c1oappe.top

auto p = std::make_unique<int>(5);
来源：http://jcp.gaohongyu789.top

[S44] C++：引用传参
来源：http://kni.shzxlz.cn

void inc(int &x) { ++x; }
来源：http://izb.yonumen.top

[S45] C++：lambda
来源：http://mvu.hnqzz.top

auto add = [](int a, int b) { return a + b; };
来源：http://xkq.haohaochexian.top

[S46] C++：函数模板
来源：http://onh.guowangkeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://iyj.iojbl.cn

[S47] C++：结构化绑定遍历
来源：http://mjb.xziqi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vjf.iojbl.cn

[S48] C++：逐行读文件
来源：http://ssd.wangdashe.top

std::ifstream in("a.txt");  std::string line;
来源：http://hvw.ctjpmb.com

while (std::getline(in, line)) { }
来源：http://uvp.yonumen.top

[S49] C++：写文件
来源：http://jrz.cqqwz.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hrq.wangshuangyany.cn

[S50] C++：格式化数字
来源：http://rmc.jqgufenzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rus.vehdjk.com

[S51] C++：显式类型转换
来源：http://vod.jinqigfzy.top

static_cast<double>(a) / b
来源：http://yhz.gogol.net.cn

[S52] C++：const 与 noexcept
来源：http://yvq.shangyingyoupin.top

int size() const noexcept { return n_; }
来源：http://eik.daxiang520.top

[S53] C++：移动语义
来源：http://vgj.wangshuangyany.cn

std::vector<int> w = std::move(v);
来源：http://vnx.iojbl.cn

[S54] C++：异常处理
来源：http://nal.zhixingplan.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jfz.c1oappe.top

[S55] C++：结构化绑定
来源：http://ckz.quarkkingdee.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ohb.havefunace.top

[S56] C++：optional
来源：http://zas.feifeiyinyue.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rnq.zhoulong.xyz

[S57] C++：编译期常量
来源：http://dsn.feifeiyinyue.top

constexpr int N = 10;
来源：http://bax.jianghu66.top

[S58] C++：命名空间
来源：http://xpw.ydjk.org.cn

namespace ns { int f() { return 1; } }
来源：http://lvc.yueranfly.top

[S59] C++：静态断言
来源：http://ztw.pengpengdd.cyou

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zqe.sysykeji.top

[S60] C++：遍历并删除元素
来源：http://kda.aizwys.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oce.cashguo.top

================================================================================
来源：http://xab.jinyuanbaomall.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ycj.pycfn.com

================================================================================
来源：http://nlf.jqgufenzy.top

[T01] Kotlin：Hello World
来源：http://ifa.ywan-chungtsiang.top

println("Hello")
来源：http://kzp.tian-w.cn

[T02] Kotlin：变量
来源：http://wkb.yonumen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://laz.hcnkem.com

[T03] Kotlin：字符串模板
来源：http://xbf.ywan-chungtsiang.top

"值: $b"
来源：http://tit.ydzc1.top

[T04] Kotlin：空安全
来源：http://sma.jinqigufen.top

val n: String? = null;  n?.length
来源：http://pog.jqgfzy.top

[T05] Kotlin：when 表达式
来源：http://cek.pycfn.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ovz.hfpthk.cn

[T06] Kotlin：集合映射
来源：http://pyx.yj20258.top

listOf(1, 2, 3).map { it * 2 }
来源：http://uvh.chenlongwang.top

[T07] Kotlin：集合过滤
来源：http://hqu.9152youxi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ylx.gotoacloud.top

[T08] Kotlin：数据类
来源：http://ufq.chenzaomai.com

data class User(val name: String, val age: Int)
来源：http://npo.kuanghao11.cn

[T09] Kotlin：扩展函数
来源：http://bnv.feifeiyinyue.top

fun String.exclaim() = this + "!"
来源：http://zrr.bjfxy.top

[T10] Kotlin：默认参数
来源：http://qck.zhixingplan.top

fun greet(name: String = "World") = "Hi $name"
来源：http://iko.yj20258.top

[T11] Kotlin：协程
来源：http://prr.ppjwa.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://uby.sxryk.cn

[T12] Kotlin：解构声明
来源：http://jij.ydzc1.top

val (a, b) = Pair(1, 2)
来源：http://zvy.svipenyu.cn

[T13] Kotlin：只读 Map
来源：http://vly.316326.xyz

val m = mapOf("a" to 1)
来源：http://ikc.zhaomingkeji.xyz

[T14] Kotlin：循环
来源：http://nev.jqgfzy.top

for (i in 1..10) println(i)
来源：http://alp.ywan-chungtsiang.top

[T15] Kotlin：接口
来源：http://viy.meibo888.top

interface Shape { fun area(): Double }
来源：http://tsj.cqqwz.cn

[T16] Swift：Hello World
来源：http://vft.yangfankeji.com

print("Hello")
来源：http://rma.zhixingplan.top

[T17] Swift：变量与常量
来源：http://bok.feifeiyinyue.top

var a = 1;  let b = 2
来源：http://vev.316326.xyz

[T18] Swift：字符串插值
来源：http://qbi.bbcook.cn

"值: \(b)"
来源：http://aeb.jianghu66.top

[T19] Swift：可选绑定
来源：http://gpy.guowangkeji.top

if let n = opt { print(n) }
来源：http://adu.zhijiandao.cn

[T20] Swift：数组操作
来源：http://hhn.cucudq.cn

var a = [1, 2, 3];  a.append(4)
来源：http://sgx.chenjidiqi.icu

[T21] Swift：遍历
来源：http://kcu.hnxiangtu.top

for x in a { print(x) }
来源：http://jza.hfpthk.cn

[T22] Swift：字典
来源：http://sju.haohaochexian.top

var d = ["a": 1];  d["b"] = 2
来源：http://xyy.wangdashe.top

[T23] Swift：函数
来源：http://noj.iojbl.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vuz.zhoulong.xyz

[T24] Swift：闭包
来源：http://vpt.sufxvd.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bvs.wangshuangyany.cn

[T25] Swift：结构体
来源：http://jtm.tianlin.xyz

struct P { var x: Int }
来源：http://qnw.hysaishi.cn

[T26] Swift：类与重写
来源：http://ups.gaohongyu789.top

class A: Base { override func f() {} }
来源：http://apq.c1oappe.top

[T27] Swift：错误处理
来源：http://yce.fehbvm.com

do { try f() } catch { print(error) }
来源：http://sax.zdqjudy.top

[T28] Swift：枚举
来源：http://qoo.aibaodan.cn

enum Color { case red, green }
来源：http://vfo.0kj1m.cn

[T29] Swift：guard 提前返回
来源：http://wyl.fanxiaobao.xyz

guard let x = opt else { return }
来源：http://drb.sjlbkw.cn

[T30] Swift：协议
来源：http://ymn.sxryk.cn

protocol Shape { func area() -> Double }
来源：http://zls.hammf.cn

[T31] Lua：Hello World
来源：http://mcs.tanke756.top

print("Hello")
来源：http://nng.jinyuanbaomall.cn

[T32] Lua：局部变量
来源：http://kdi.yanxiufei.cn

local a = 1
来源：http://wrz.ydzc1.top

[T33] Lua：表（数组）
来源：http://ict.ywan-chungtsiang.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kzs.cucudq.cn

[T34] Lua：遍历表
来源：http://cbs.tanke756.top

for i, v in ipairs(t) do print(i, v) end
来源：http://xdj.daxiang520.top

[T35] Lua：字典表
来源：http://xou.gzhubu.top

local d = { a = 1 };  d.b = 2
来源：http://kfd.quarkkingdee.top

[T36] Lua：函数
来源：http://frw.hongshengwenyu.top

function add(a, b) return a + b end
来源：http://yly.yonumen.top

[T37] Lua：字符串拼接
来源：http://hli.zycfv.cn

"a" .. "b"
来源：http://hvy.zhengqikj.top

[T38] Lua：条件
来源：http://mdi.yvedp.cn

if x > 0 then print("正") end
来源：http://zza.hcnkem.com

[T39] Lua：模式匹配
来源：http://bbr.vehdjk.com

string.find(s, "%d+")
来源：http://lea.hcnkem.com

[T40] Lua：元表
来源：http://ghn.cucudq.cn

setmetatable({}, { __index = base })
来源：http://jwl.sxryk.cn

[T41] Perl：Hello World
来源：http://tou.epnwcf.com

print "Hello\n";
来源：http://rqc.shanyushiyangtech.top

[T42] Perl：变量类型
来源：http://dyf.shanyushiyangkeji.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://awg.zhiwuduotai.top

[T43] Perl：字符串插值
来源：http://eib.yj20258888.top

"值: $a"
来源：http://phz.hesvh.cn

[T44] Perl：条件
来源：http://bzg.hongshengwenyu.top

if ($a > 0) { print "正"; }
来源：http://kvx.kuanghao11.cn

[T45] Perl：数组遍历
来源：http://tdn.fehbvm.com

for my $x (@arr) { print $x; }
来源：http://wzj.xuanzx.com

[T46] Perl：哈希操作
来源：http://osi.zhixingplan.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://oyx.hnqzz.top

[T47] Perl：正则捕获
来源：http://ygn.yj20258888.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ivq.andypj.xyz

[T48] Perl：正则替换
来源：http://bpc.cdnleiting.top

$s =~ s/old/new/g;
来源：http://thk.xingfuxueyuan.xyz

[T49] Perl：函数
来源：http://fcq.shanyushiyangtech.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yjl.hammf.cn

[T50] Perl：逐行读文件
来源：http://wkf.zhijiandao.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://asi.nwbrower.top

while (my $line = <$fh>) { print $line; }
来源：http://sel.52xcode.cn

[T51] Scala：Hello World
来源：http://iex.52xcode.cn

println("Hello")
来源：http://uhq.zdbjq.cn

[T52] Scala：变量
来源：http://zyr.yueranfly.top

val a = 1;  var b = 2
来源：http://qnb.vqdsnc.cn

[T53] Scala：字符串插值
来源：http://lsc.gaohongyu789.top

s"值: $b"
来源：http://yjd.dashuyun.cn

[T54] Scala：集合映射
来源：http://wrm.9152youxi.cn

List(1, 2, 3).map(_ * 2)
来源：http://glz.yuxming.cn

[T55] Scala：集合过滤
来源：http://fpy.hysaishi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://efv.cucudq.cn

[T56] Scala：样例类
来源：http://kkt.fehbvm.com

case class User(name: String, age: Int)
来源：http://oqo.ywan-chungtsiang.top

[T57] Scala：模式匹配
来源：http://ovc.chenzaomai.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://dfl.nanxuanxn.top

[T58] Scala：函数定义
来源：http://pge.xziqi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dhk.jqgufenzy.top

[T59] Scala：循环
来源：http://oor.sjlbkw.cn

for (i <- 1 to 10) println(i)
来源：http://zqd.daria6918.cn

[T60] Scala：折叠
来源：http://hvl.zdqjudy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xzc.jqgufenzy.top

================================================================================
来源：http://rzx.fktsv.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jsq.sweek.top

================================================================================
来源：http://oiu.xziqi.cn

[U01] Py：创建虚拟环境
来源：http://eab.ehwqpu.com

python -m venv .venv && source .venv/bin/activate
来源：http://kno.yangfankeji.com

[U02] Py：导出 / 安装依赖
来源：http://iom.jlsjyb.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://soy.hnxiangtu.top


<!-- 参考信息 -->