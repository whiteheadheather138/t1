代发 wailian999

free -h;  ps aux | grep nginx
来源：http://vyw.yangfankeji.com

[R64] 结束进程
来源：http://swp.xuetiantiany.cn

kill -9 $(pgrep -f app.py)
来源：http://uog.zhongyouzk.top

[R65] 查看端口占用
来源：http://rif.yj20258888.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qyr.52xcode.cn

[R66] 定时任务
来源：http://ost.hnxiangtu.top

crontab -e;  crontab -l
来源：http://lwz.ydjk.org.cn

[R67] 生成随机十六进制串
来源：http://jsy.guowangkeji.top

openssl rand -hex 16
来源：http://npd.sufxvd.cn

[R68] 计算文件校验值
来源：http://qls.shangyingyoupin.top

sha256sum a.txt;  md5sum a.txt
来源：http://ach.hongshengwenyu.top

[R69] 生成随机密码
来源：http://obn.fzhhl.top

head -c 16 /dev/urandom | base64
来源：http://ppk.yfazqb.com

[R70] 时间戳与互转
来源：http://mih.hnxiangtu.top

date +%s;  date -d @1700000000
来源：http://mcy.svipenyu.cn

[R71] 日期格式化
来源：http://kxt.c1oappe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://wqh.zhoulong.xyz

[R72] 等待端口就绪
来源：http://urc.0kj1m.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://giq.jinyuanbaomall.cn

[R73] 分割大日志
来源：http://qwz.fanxiaobao.xyz

split -l 1000 big.log part_
来源：http://xlb.cheryme.top

[R74] 批量重命名
来源：http://lxk.haohaochexian.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://voz.ppjwa.cn

[R75] 导出环境变量
来源：http://xbs.daxiang520.top

export PATH="$HOME/bin:$PATH"
来源：http://zai.ybcxt.top

[R76] 使用临时文件
来源：http://scd.snrcjt.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vnl.ywan-chungtsiang.top

[R77] 读取用户输入
来源：http://qkm.jinghuilouyu.cn

read -rp "请输入: " ans
来源：http://tcf.zdqjudy.top

[R78] 交互式菜单
来源：http://vio.bjfxy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rlm.nwbrower.top

[R79] 解析命令行选项
来源：http://fzd.jlsjyb.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pay.meibo888.top

[R80] 查看脚本执行耗时
来源：http://tut.andypj.xyz

time ./run.sh
来源：http://ddk.hywenlv.cn

================================================================================
来源：http://cly.redwolf501.top

S. C / C++ 专题
来源：http://skc.havefunace.top

================================================================================
来源：http://itq.tianlin.xyz

[S01] C：Hello World
来源：http://obk.gaohongyu789.top

#include <stdio.h>
来源：http://ohn.aibaodan.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rde.gzhubu.top

[S02] C：变量与格式化输出
来源：http://hha.jinqigufen.top

int a = 10; printf("%d\n", a);
来源：http://zfr.haohaochexian.top

[S03] C：读入整数
来源：http://rnl.9152youxi.cn

int x; scanf("%d", &x);
来源：http://vrm.hongshengwenyu.top

[S04] C：字符串复制
来源：http://ifp.gaohongyu789.top

char dst[32]; strcpy(dst, "hi");
来源：http://evn.haohaochexian.top

[S05] C：字符串长度
来源：http://ouz.9152youxi.cn

strlen(s)
来源：http://lcn.smart0.xyz

[S06] C：字符串比较
来源：http://pev.yj20258888.top

strcmp(a, b) == 0
来源：http://zhb.andypj.xyz

[S07] C：数组遍历求和
来源：http://fev.yueranfly.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eni.xuanzx.com

[S08] C：动态内存分配与释放
来源：http://itf.xinyue.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pap.jqgufenzy.top

[S09] C：结构体定义与初始化
来源：http://hxy.ydzc1.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dhj.zhoulong.xyz

[S10] C：指针与解引用
来源：http://ege.xylfe.cn

int *p = &a;  *p = 5;
来源：http://hom.jinqigfzy.top

[S11] C：逐行读文件
来源：http://aar.guannengcc.top

FILE *f = fopen("a.txt", "r");
来源：http://hjd.iojbl.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dbe.jinyuanbaomall.cn

fclose(f);
来源：http://pdf.fengsongda.top

[S12] C：写文件
来源：http://rmu.hongshengwenyu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zmi.hongshengwenyu.top

[S13] C：宏定义
来源：http://moi.zhijiandao.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kwp.hammf.cn

[S14] C：枚举
来源：http://sch.xylfe.cn

enum Color { RED, GREEN, BLUE };
来源：http://pjk.snrcjt.cn

[S15] C：类型转换
来源：http://vya.ctjpmb.com

(double) a / b
来源：http://ygg.gotoacloud.top

[S16] C：位操作置位
来源：http://ikl.gogol.net.cn

x |= (1 << 3);
来源：http://ene.cqqwz.cn

[S17] C：安全拼接字符串
来源：http://smt.tarul.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://umy.nanxinkj.top

[S18] C：命令行参数
来源：http://qlu.yueranfly.top

int main(int argc, char **argv)
来源：http://ycv.shuidangran.top

[S19] C：快速排序
来源：http://ihi.316326.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://rsj.hfpthk.cn

[S20] C：二分查找
来源：http://ikl.zhongyouzk.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rmf.zdqjudy.top

[S21] C：字符类别判断
来源：http://yzp.hammf.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zjb.cashguo.top

[S22] C：字符串转数字
来源：http://zsq.hongshengwenyu.top

atoi("42");  strtod("3.14", NULL);
来源：http://eda.shuidangran.top

[S23] C：随机数
来源：http://ewl.dianchejie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zwh.redwolf501.top

[S24] C：获取本地时间
来源：http://ghl.shanyushiyangtech.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jcc.shanyushiyangtech.top

[S25] C：内存拷贝
来源：http://efi.wangdashe.top

memcpy(dst, src, n);
来源：http://eef.zhijiandao.cn

[S26] C：内存清零
来源：http://svo.jinqigufen.top

memset(a, 0, sizeof a);
来源：http://xkm.tian-w.cn

[S27] C：定义常量
来源：http://mip.redwolf501.top

const double PI = 3.14159;
来源：http://owk.zhongyouzk.top

[S28] C：静态变量
来源：http://qle.kuanghao11.cn

static int counter = 0;
来源：http://ucu.smart0.xyz

[S29] C：变参函数
来源：http://yhu.zhongyouzk.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gvm.cucudq.cn

[S30] C：头文件保护
来源：http://zlw.kuanghao11.cn

#ifndef X_H
来源：http://jkx.gaohongyu789.top

#define X_H
来源：http://evz.fengsongda.top

#endif
来源：http://yif.jqgfzy.top

[S31] C++：Hello World
来源：http://pus.havefunace.top

#include <iostream>
来源：http://hlg.ivvv.top

int main() { std::cout << "Hello\n"; }
来源：http://lsr.zdqjudy.top

[S32] C++：字符串
来源：http://tgn.52xcode.cn

std::string s = "hi";  s += "!";
来源：http://wfa.ydzc1.top

[S33] C++：vector 增删
来源：http://whc.sufxvd.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eed.chenlongwang.top

[S34] C++：遍历 vector
来源：http://rva.jiagoushi.top

for (auto &x : v) { std::cout << x; }
来源：http://mgm.aibaodan.cn

[S35] C++：map
来源：http://fsl.cashguo.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ubw.zhijiandao.cn

[S36] C++：unordered_map
来源：http://hrd.cashguo.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://prw.cheryme.top

[S37] C++：set
来源：http://nxd.yuanzhike.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ddk.guowangkeji.top

[S38] C++：排序
来源：http://vkj.feifeiyinyue.top

std::sort(v.begin(), v.end());
来源：http://uun.yonumen.top

[S39] C++：自定义比较器排序
来源：http://jyw.bjfxy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ewy.nanxinkj.top

[S40] C++：查找元素
来源：http://zuu.bbcook.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lfi.quarkkingdee.top

[S41] C++：类与构造函数
来源：http://igt.tanke756.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bej.gzhubu.top

[S42] C++：继承与虚函数
来源：http://pcp.pycfn.com

class B : public Base { public: void f() override {} };
来源：http://dve.epnwcf.com

[S43] C++：智能指针
来源：http://ksa.ybcxt.top

auto p = std::make_unique<int>(5);
来源：http://sea.wangshuangyany.cn

[S44] C++：引用传参
来源：http://vut.jlsjyb.cn

void inc(int &x) { ++x; }
来源：http://kbl.andypj.xyz

[S45] C++：lambda
来源：http://hlm.hfpthk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bri.yfazqb.com

[S46] C++：函数模板
来源：http://bbt.daxiang520.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ofk.bbcook.cn

[S47] C++：结构化绑定遍历
来源：http://cby.fzhhl.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://plc.hongshengwenyu.top

[S48] C++：逐行读文件
来源：http://uni.ppjwa.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wyl.guowangkeji.top

while (std::getline(in, line)) { }
来源：http://can.fehbvm.com

[S49] C++：写文件
来源：http://suh.daria6918.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dhe.fehbvm.com

[S50] C++：格式化数字
来源：http://zqd.wangshuangyany.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pzf.jlsjyb.cn

[S51] C++：显式类型转换
来源：http://dgm.xylfe.cn

static_cast<double>(a) / b
来源：http://tao.cheryme.top

[S52] C++：const 与 noexcept
来源：http://ule.52xcode.cn

int size() const noexcept { return n_; }
来源：http://loh.sufxvd.cn

[S53] C++：移动语义
来源：http://hqx.uphjek.com

std::vector<int> w = std::move(v);
来源：http://yqi.cucudq.cn

[S54] C++：异常处理
来源：http://wei.ybcxt.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lse.kuanghao11.cn

[S55] C++：结构化绑定
来源：http://bva.fengsongda.top

auto [a, b] = std::make_pair(1, 2);
来源：http://mbj.smart0.xyz

[S56] C++：optional
来源：http://ybl.jlsjyb.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qjl.yongpay.top

[S57] C++：编译期常量
来源：http://bbn.guannengcc.top

constexpr int N = 10;
来源：http://xgl.gzhubu.top

[S58] C++：命名空间
来源：http://gan.aizwys.cn

namespace ns { int f() { return 1; } }
来源：http://sxd.gogol.net.cn

[S59] C++：静态断言
来源：http://gse.wangdashe.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hkg.yj20258.top

[S60] C++：遍历并删除元素
来源：http://pdl.jinqigufen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hvg.hcnkem.com

================================================================================
来源：http://dvi.smart0.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hql.xziqi.cn

================================================================================
来源：http://hfu.shuidangran.top

[T01] Kotlin：Hello World
来源：http://gda.smart0.xyz

println("Hello")
来源：http://qsw.fanxiaobao.xyz

[T02] Kotlin：变量
来源：http://yjw.yj202588.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tjc.tian-w.cn

[T03] Kotlin：字符串模板
来源：http://yfs.cucudq.cn

"值: $b"
来源：http://tqs.smart0.xyz

[T04] Kotlin：空安全
来源：http://ypx.yvedp.cn

val n: String? = null;  n?.length
来源：http://drc.ppjwa.cn

[T05] Kotlin：when 表达式
来源：http://umo.kuanghao11.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hwy.zhengqikj.top

[T06] Kotlin：集合映射
来源：http://hnr.sufxvd.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bju.hesvh.cn

[T07] Kotlin：集合过滤
来源：http://bur.epnwcf.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://uoe.jiagoushi.top

[T08] Kotlin：数据类
来源：http://njx.ehwqpu.com

data class User(val name: String, val age: Int)
来源：http://tqj.sjlbkw.cn

[T09] Kotlin：扩展函数
来源：http://dru.yj20258888.top

fun String.exclaim() = this + "!"
来源：http://pdw.bbcook.cn

[T10] Kotlin：默认参数
来源：http://oia.fengsongda.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qmu.fzhhl.top

[T11] Kotlin：协程
来源：http://ybb.hesvh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kyy.ppjwa.cn

[T12] Kotlin：解构声明
来源：http://ouh.zdbjq.cn

val (a, b) = Pair(1, 2)
来源：http://yrh.jqgufenzy.top

[T13] Kotlin：只读 Map
来源：http://uvg.yj20258.top

val m = mapOf("a" to 1)
来源：http://aml.hnqzz.top

[T14] Kotlin：循环
来源：http://kan.zhoulong.xyz

for (i in 1..10) println(i)
来源：http://wnq.hongshengwenyu.top

[T15] Kotlin：接口
来源：http://hqq.tarul.cn

interface Shape { fun area(): Double }
来源：http://vyn.jlsjyb.cn

[T16] Swift：Hello World
来源：http://gkr.haohaochexian.top

print("Hello")
来源：http://gkk.xylfe.cn

[T17] Swift：变量与常量
来源：http://gvw.aibaodan.cn

var a = 1;  let b = 2
来源：http://ezr.ppjwa.cn

[T18] Swift：字符串插值
来源：http://mre.feifeiyinyue.top

"值: \(b)"
来源：http://ven.chenlongwang.top

[T19] Swift：可选绑定
来源：http://oxo.yuxming.cn

if let n = opt { print(n) }
来源：http://szv.yuxming.cn

[T20] Swift：数组操作
来源：http://dbg.tian-w.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ofn.52xcode.cn

[T21] Swift：遍历
来源：http://lbh.ywan-chungtsiang.top

for x in a { print(x) }
来源：http://twh.52xcode.cn

[T22] Swift：字典
来源：http://que.bjfxy.top

var d = ["a": 1];  d["b"] = 2
来源：http://tfu.aizwys.cn

[T23] Swift：函数
来源：http://hrt.feifeiyinyue.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yex.tian-w.cn

[T24] Swift：闭包
来源：http://vil.guannengcc.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://yug.wangdashe.top

[T25] Swift：结构体
来源：http://ycg.yuxming.cn

struct P { var x: Int }
来源：http://gyx.havefunace.top

[T26] Swift：类与重写
来源：http://mgy.kuanghao11.cn

class A: Base { override func f() {} }
来源：http://ezd.sysykeji.top

[T27] Swift：错误处理
来源：http://qcn.yueranfly.top

do { try f() } catch { print(error) }
来源：http://hve.bbcook.cn

[T28] Swift：枚举
来源：http://eet.meibo888.top

enum Color { case red, green }
来源：http://jxg.zhaomingkeji.xyz

[T29] Swift：guard 提前返回
来源：http://cxs.316326.xyz

guard let x = opt else { return }
来源：http://aof.nanxuanxn.top

[T30] Swift：协议
来源：http://rzo.sweek.top

protocol Shape { func area() -> Double }
来源：http://hnp.aizwys.cn

[T31] Lua：Hello World
来源：http://ufz.zdbjq.cn

print("Hello")
来源：http://vup.jinyuanbaomall.cn

[T32] Lua：局部变量
来源：http://pdg.ehwqpu.com

local a = 1
来源：http://qdb.zhiwuduotai.top

[T33] Lua：表（数组）
来源：http://jfb.vehdjk.com

local t = {1, 2, 3};  t[4] = 4
来源：http://sit.tanke756.top

[T34] Lua：遍历表
来源：http://myf.vehdjk.com

for i, v in ipairs(t) do print(i, v) end
来源：http://udv.yvedp.cn

[T35] Lua：字典表
来源：http://zbw.yuanzhike.top

local d = { a = 1 };  d.b = 2
来源：http://vwr.gzhubu.top

[T36] Lua：函数
来源：http://leq.chenlongwang.top

function add(a, b) return a + b end
来源：http://wlj.yongpay.top

[T37] Lua：字符串拼接
来源：http://erj.guannengcc.top

"a" .. "b"
来源：http://xph.vehdjk.com

[T38] Lua：条件
来源：http://omh.fanxiaobao.xyz

if x > 0 then print("正") end
来源：http://isn.vehdjk.com

[T39] Lua：模式匹配
来源：http://fcj.quarkkingdee.top

string.find(s, "%d+")
来源：http://fgb.ywan-chungtsiang.top

[T40] Lua：元表
来源：http://ebo.svipenyu.cn

setmetatable({}, { __index = base })
来源：http://cbw.nanxinkj.top

[T41] Perl：Hello World
来源：http://nyz.bjfxy.top

print "Hello\n";
来源：http://hkh.pengpengdd.cyou

[T42] Perl：变量类型
来源：http://qrj.hongshengwenyu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nya.meibo888.top

[T43] Perl：字符串插值
来源：http://mnp.hywenlv.cn

"值: $a"
来源：http://hgg.gaohongyu789.top

[T44] Perl：条件
来源：http://gbq.aibaodan.cn

if ($a > 0) { print "正"; }
来源：http://ifw.zhongyouzk.top

[T45] Perl：数组遍历
来源：http://woj.zhijiandao.cn

for my $x (@arr) { print $x; }
来源：http://eon.ivvv.top

[T46] Perl：哈希操作
来源：http://msc.jiagoushi.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://izs.hongshengwenyu.top

[T47] Perl：正则捕获
来源：http://ksq.jinyuanbaomall.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xhr.shangyingyoupin.top

[T48] Perl：正则替换
来源：http://fmp.zdbjq.cn

$s =~ s/old/new/g;
来源：http://eme.nanxinkj.top

[T49] Perl：函数
来源：http://zib.xziqi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bxk.gotoacloud.top

[T50] Perl：逐行读文件
来源：http://rga.fktsv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://pxw.hnqzz.top

while (my $line = <$fh>) { print $line; }
来源：http://jwx.fehbvm.com

[T51] Scala：Hello World
来源：http://zku.gogol.net.cn

println("Hello")
来源：http://xcq.yj20258888.top

[T52] Scala：变量
来源：http://nxy.vqdsnc.cn

val a = 1;  var b = 2
来源：http://evl.jiagoushi.top

[T53] Scala：字符串插值
来源：http://wiq.nanxuanxn.top

s"值: $b"
来源：http://zhs.smart0.xyz

[T54] Scala：集合映射
来源：http://pbo.redwolf501.top

List(1, 2, 3).map(_ * 2)
来源：http://rkq.yuanzhike.top

[T55] Scala：集合过滤
来源：http://ive.0kj1m.cn

List(1, 2, 3).filter(_ > 1)
来源：http://syv.yj202588.top

[T56] Scala：样例类
来源：http://xbd.sufxvd.cn

case class User(name: String, age: Int)
来源：http://ing.zdbjq.cn

[T57] Scala：模式匹配
来源：http://min.shzxlz.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://anb.chenzaomai.com

[T58] Scala：函数定义
来源：http://npe.zdbjq.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ofi.andypj.xyz

[T59] Scala：循环
来源：http://kka.zhoulong.xyz

for (i <- 1 to 10) println(i)
来源：http://vyr.xuetiantiany.cn

[T60] Scala：折叠
来源：http://shw.hywenlv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://azh.chenlongwang.top

================================================================================
来源：http://gja.hnqzz.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://iiu.hnqzz.top

================================================================================
来源：http://kau.sysykeji.top

[U01] Py：创建虚拟环境
来源：http://epr.gzhubu.top

python -m venv .venv && source .venv/bin/activate
来源：http://dqd.ywan-chungtsiang.top

[U02] Py：导出 / 安装依赖
来源：http://rdl.sysykeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vgm.zhengqikj.top

[U03] Py：加载 .env 配置
来源：http://btf.yonumen.top

from dotenv import load_dotenv; load_dotenv()
来源：http://sjy.fktsv.cn

[U04] Py：变量调试打印
来源：http://ypf.yangfankeji.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tna.pycfn.com


<!-- 参考信息 -->