代发 wailian999

free -h;  ps aux | grep nginx
来源：http://gjp.kuanghao11.cn

[R64] 结束进程
来源：http://pde.jinghuilouyu.cn

kill -9 $(pgrep -f app.py)
来源：http://zxj.jyoumei.cn

[R65] 查看端口占用
来源：http://yhs.xuanzx.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mog.316326.xyz

[R66] 定时任务
来源：http://orz.hongshengwenyu.top

crontab -e;  crontab -l
来源：http://wyl.ehwqpu.com

[R67] 生成随机十六进制串
来源：http://woc.xuetiantiany.cn

openssl rand -hex 16
来源：http://gti.bbcook.cn

[R68] 计算文件校验值
来源：http://hgk.aibaodan.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qss.hnqzz.top

[R69] 生成随机密码
来源：http://qpf.birdmap.top

head -c 16 /dev/urandom | base64
来源：http://miz.nanxuanxn.top

[R70] 时间戳与互转
来源：http://mko.yonumen.top

date +%s;  date -d @1700000000
来源：http://chm.daxiang520.top

[R71] 日期格式化
来源：http://csm.guowangkeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://mmy.sysykeji.top

[R72] 等待端口就绪
来源：http://fej.hammf.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pvq.ybcxt.top

[R73] 分割大日志
来源：http://xyz.shanyushiyangtech.top

split -l 1000 big.log part_
来源：http://vvy.yangfankeji.com

[R74] 批量重命名
来源：http://idt.uphjek.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oec.svipenyu.cn

[R75] 导出环境变量
来源：http://yua.jinyuanbaomall.cn

export PATH="$HOME/bin:$PATH"
来源：http://vpj.cqqwz.cn

[R76] 使用临时文件
来源：http://dxc.gaohongyu789.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://igj.daxiang520.top

[R77] 读取用户输入
来源：http://avn.yuxming.cn

read -rp "请输入: " ans
来源：http://btf.ivvv.top

[R78] 交互式菜单
来源：http://zim.hfpthk.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zwr.redwolf501.top

[R79] 解析命令行选项
来源：http://vev.yonumen.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hok.yonumen.top

[R80] 查看脚本执行耗时
来源：http://hxr.bbcook.cn

time ./run.sh
来源：http://vmk.jianghu66.top

================================================================================
来源：http://iut.iojbl.cn

S. C / C++ 专题
来源：http://rxl.ywan-chungtsiang.top

================================================================================
来源：http://otg.c1oappe.top

[S01] C：Hello World
来源：http://zts.redwolf501.top

#include <stdio.h>
来源：http://jkz.52xcode.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://llc.tanke756.top

[S02] C：变量与格式化输出
来源：http://fcj.hnxiangtu.top

int a = 10; printf("%d\n", a);
来源：http://rfk.gotoacloud.top

[S03] C：读入整数
来源：http://pua.cdnleiting.top

int x; scanf("%d", &x);
来源：http://rsv.yj20258888.top

[S04] C：字符串复制
来源：http://irb.yanxiufei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wvi.shzxlz.cn

[S05] C：字符串长度
来源：http://wef.aizwys.cn

strlen(s)
来源：http://jpv.nanxinkj.top

[S06] C：字符串比较
来源：http://tto.cdnleiting.top

strcmp(a, b) == 0
来源：http://idn.fanxiaobao.xyz

[S07] C：数组遍历求和
来源：http://kqv.tarul.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qjr.zhixingplan.top

[S08] C：动态内存分配与释放
来源：http://kbq.tian-w.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uxs.yuanzhike.top

[S09] C：结构体定义与初始化
来源：http://ufo.nanxuanxn.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yzp.yfazqb.com

[S10] C：指针与解引用
来源：http://nhc.316326.xyz

int *p = &a;  *p = 5;
来源：http://kgm.ybcxt.top

[S11] C：逐行读文件
来源：http://hcd.gogol.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://mxa.haohaochexian.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vmi.hnxiangtu.top

fclose(f);
来源：http://tin.jianghu66.top

[S12] C：写文件
来源：http://siz.nanxinkj.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nix.quarkkingdee.top

[S13] C：宏定义
来源：http://tiq.jiagoushi.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oyh.zhongyouzk.top

[S14] C：枚举
来源：http://uwj.yuanzhike.top

enum Color { RED, GREEN, BLUE };
来源：http://tvo.yanxiufei.cn

[S15] C：类型转换
来源：http://mmd.bjfxy.top

(double) a / b
来源：http://xic.smart0.xyz

[S16] C：位操作置位
来源：http://rjr.birdmap.top

x |= (1 << 3);
来源：http://ncd.tanke756.top

[S17] C：安全拼接字符串
来源：http://inc.meibo888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bnt.316326.xyz

[S18] C：命令行参数
来源：http://vtk.yonumen.top

int main(int argc, char **argv)
来源：http://hly.ehwqpu.com

[S19] C：快速排序
来源：http://voq.zycfv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wbd.fanxiaobao.xyz

[S20] C：二分查找
来源：http://vor.dashuyun.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dkm.hcnkem.com

[S21] C：字符类别判断
来源：http://kim.fzhhl.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gbx.yuanzhike.top

[S22] C：字符串转数字
来源：http://xnt.hcnkem.com

atoi("42");  strtod("3.14", NULL);
来源：http://oac.fanxiaobao.xyz

[S23] C：随机数
来源：http://duk.zycfv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rlr.ydzc1.top

[S24] C：获取本地时间
来源：http://nhh.dianchejie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://doy.sjlbkw.cn

[S25] C：内存拷贝
来源：http://mpa.zhengqikj.top

memcpy(dst, src, n);
来源：http://jtl.ydjk.org.cn

[S26] C：内存清零
来源：http://ufr.yvedp.cn

memset(a, 0, sizeof a);
来源：http://emv.guannengcc.top

[S27] C：定义常量
来源：http://enx.shanyushiyangtech.top

const double PI = 3.14159;
来源：http://moc.pengpengdd.cyou

[S28] C：静态变量
来源：http://paa.ivvv.top

static int counter = 0;
来源：http://jmm.zhoulong.xyz

[S29] C：变参函数
来源：http://dys.xziqi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ltc.uphjek.com

[S30] C：头文件保护
来源：http://zcp.haohaochexian.top

#ifndef X_H
来源：http://pld.shzxlz.cn

#define X_H
来源：http://cvr.tarul.cn

#endif
来源：http://xai.hnxiangtu.top

[S31] C++：Hello World
来源：http://hfi.cucudq.cn

#include <iostream>
来源：http://nmo.haohaochexian.top

int main() { std::cout << "Hello\n"; }
来源：http://pnv.jinghuilouyu.cn

[S32] C++：字符串
来源：http://iqp.yanxiufei.cn

std::string s = "hi";  s += "!";
来源：http://hef.hongshengwenyu.top

[S33] C++：vector 增删
来源：http://ivb.c1oappe.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xyv.yfazqb.com

[S34] C++：遍历 vector
来源：http://ees.gogol.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://vux.zhengqikj.top

[S35] C++：map
来源：http://ofw.aibaodan.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gtw.shanyushiyangtech.top

[S36] C++：unordered_map
来源：http://rls.gaohongyu789.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ewy.shangyingyoupin.top

[S37] C++：set
来源：http://gji.fktsv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pzq.yongpay.top

[S38] C++：排序
来源：http://kiv.ywan-chungtsiang.top

std::sort(v.begin(), v.end());
来源：http://zwm.andypj.xyz

[S39] C++：自定义比较器排序
来源：http://ksc.bjfxy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ozp.sxryk.cn

[S40] C++：查找元素
来源：http://gvb.xuanzx.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rmw.zhaomingkeji.xyz

[S41] C++：类与构造函数
来源：http://tjd.feifeiyinyue.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xkt.iojbl.cn

[S42] C++：继承与虚函数
来源：http://oey.bbcook.cn

class B : public Base { public: void f() override {} };
来源：http://oea.daria6918.cn

[S43] C++：智能指针
来源：http://wjw.dianchejie.cn

auto p = std::make_unique<int>(5);
来源：http://daa.cashguo.top

[S44] C++：引用传参
来源：http://gmg.xylfe.cn

void inc(int &x) { ++x; }
来源：http://jor.chenzaomai.com

[S45] C++：lambda
来源：http://obz.zdbjq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://deq.shangyingyoupin.top

[S46] C++：函数模板
来源：http://dny.feifeiyinyue.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yva.daxiang520.top

[S47] C++：结构化绑定遍历
来源：http://jmo.feifeiyinyue.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ipe.zhixingplan.top

[S48] C++：逐行读文件
来源：http://ubh.gaohongyu789.top

std::ifstream in("a.txt");  std::string line;
来源：http://uvc.yonumen.top

while (std::getline(in, line)) { }
来源：http://fey.hesvh.cn

[S49] C++：写文件
来源：http://mik.dianchejie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://njm.epnwcf.com

[S50] C++：格式化数字
来源：http://fcy.jqgufenzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bhp.aizwys.cn

[S51] C++：显式类型转换
来源：http://mbp.cdnleiting.top

static_cast<double>(a) / b
来源：http://qam.ydjk.org.cn

[S52] C++：const 与 noexcept
来源：http://nxr.quarkkingdee.top

int size() const noexcept { return n_; }
来源：http://hqa.zhaomingkeji.xyz

[S53] C++：移动语义
来源：http://efk.jianghu66.top

std::vector<int> w = std::move(v);
来源：http://blu.yonumen.top

[S54] C++：异常处理
来源：http://dxq.shanyushiyangtech.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xjz.xinyue.icu

[S55] C++：结构化绑定
来源：http://gqj.jinyuanbaomall.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mvb.fengsongda.top

[S56] C++：optional
来源：http://wff.tanke756.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://skx.vehdjk.com

[S57] C++：编译期常量
来源：http://bfb.mhx1999.top

constexpr int N = 10;
来源：http://crs.tanke756.top

[S58] C++：命名空间
来源：http://xkp.52xcode.cn

namespace ns { int f() { return 1; } }
来源：http://ocy.xuanzx.com

[S59] C++：静态断言
来源：http://lff.yonumen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bhd.nanxuanxn.top

[S60] C++：遍历并删除元素
来源：http://ilx.yfazqb.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rfg.ydzc1.top

================================================================================
来源：http://xlc.guowangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dal.chenjidiqi.icu

================================================================================
来源：http://kux.fengsongda.top

[T01] Kotlin：Hello World
来源：http://uwr.yangfankeji.com

println("Hello")
来源：http://ogg.fktsv.cn

[T02] Kotlin：变量
来源：http://ynm.ywan-chungtsiang.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://eei.jinqigufen.top

[T03] Kotlin：字符串模板
来源：http://rcv.aibaodan.cn

"值: $b"
来源：http://lqr.shanyushiyangkeji.top

[T04] Kotlin：空安全
来源：http://ksn.quarkkingdee.top

val n: String? = null;  n?.length
来源：http://yjf.jinghuilouyu.cn

[T05] Kotlin：when 表达式
来源：http://bop.hysaishi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://aob.ppjwa.cn

[T06] Kotlin：集合映射
来源：http://zmc.shangyingyoupin.top

listOf(1, 2, 3).map { it * 2 }
来源：http://lpw.dashuyun.cn

[T07] Kotlin：集合过滤
来源：http://saq.ehwqpu.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://ymk.fengsongda.top

[T08] Kotlin：数据类
来源：http://fmr.bjfxy.top

data class User(val name: String, val age: Int)
来源：http://qll.yanxiufei.cn

[T09] Kotlin：扩展函数
来源：http://igc.guannengcc.top

fun String.exclaim() = this + "!"
来源：http://wyt.fehbvm.com

[T10] Kotlin：默认参数
来源：http://nvl.yj202588.top

fun greet(name: String = "World") = "Hi $name"
来源：http://hek.uphjek.com

[T11] Kotlin：协程
来源：http://yvt.cdnleiting.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ttr.yj20258.top

[T12] Kotlin：解构声明
来源：http://sju.iojbl.cn

val (a, b) = Pair(1, 2)
来源：http://yss.yvedp.cn

[T13] Kotlin：只读 Map
来源：http://inn.tian-w.cn

val m = mapOf("a" to 1)
来源：http://gne.jyoumei.cn

[T14] Kotlin：循环
来源：http://ajj.fengsongda.top

for (i in 1..10) println(i)
来源：http://kro.hfpthk.cn

[T15] Kotlin：接口
来源：http://imz.sufxvd.cn

interface Shape { fun area(): Double }
来源：http://jdx.uphjek.com

[T16] Swift：Hello World
来源：http://nvy.yj202588.top

print("Hello")
来源：http://gum.daxiang520.top

[T17] Swift：变量与常量
来源：http://myb.fktsv.cn

var a = 1;  let b = 2
来源：http://eac.zhaomingkeji.xyz

[T18] Swift：字符串插值
来源：http://olx.xziqi.cn

"值: \(b)"
来源：http://pbn.yj202588.top

[T19] Swift：可选绑定
来源：http://emq.ydjk.org.cn

if let n = opt { print(n) }
来源：http://rde.hysaishi.cn

[T20] Swift：数组操作
来源：http://zqm.gaohongyu789.top

var a = [1, 2, 3];  a.append(4)
来源：http://zsn.chenlongwang.top

[T21] Swift：遍历
来源：http://fhy.xylfe.cn

for x in a { print(x) }
来源：http://qgz.shanyushiyangtech.top

[T22] Swift：字典
来源：http://ipb.tianlin.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://agv.yvedp.cn

[T23] Swift：函数
来源：http://wdu.andypj.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://alu.cheryme.top

[T24] Swift：闭包
来源：http://oab.fktsv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vip.cucudq.cn

[T25] Swift：结构体
来源：http://tdi.shuidangran.top

struct P { var x: Int }
来源：http://pvr.ctjpmb.com

[T26] Swift：类与重写
来源：http://hpm.ywan-chungtsiang.top

class A: Base { override func f() {} }
来源：http://gam.yanxiufei.cn

[T27] Swift：错误处理
来源：http://stw.jyoumei.cn

do { try f() } catch { print(error) }
来源：http://tea.yj20258888.top

[T28] Swift：枚举
来源：http://nuc.fzhhl.top

enum Color { case red, green }
来源：http://arp.ydjk.org.cn

[T29] Swift：guard 提前返回
来源：http://vtt.gotoacloud.top

guard let x = opt else { return }
来源：http://sql.shzxlz.cn

[T30] Swift：协议
来源：http://oae.yueranfly.top

protocol Shape { func area() -> Double }
来源：http://hfn.jlsjyb.cn

[T31] Lua：Hello World
来源：http://oac.birdmap.top

print("Hello")
来源：http://lnc.chenlongwang.top

[T32] Lua：局部变量
来源：http://mfi.xinyue.icu

local a = 1
来源：http://gmj.yanxiufei.cn

[T33] Lua：表（数组）
来源：http://rrz.dashuyun.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://iwq.shuidangran.top

[T34] Lua：遍历表
来源：http://lgd.iojbl.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://akn.kuanghao11.cn

[T35] Lua：字典表
来源：http://ael.tarul.cn

local d = { a = 1 };  d.b = 2
来源：http://mav.shzxlz.cn

[T36] Lua：函数
来源：http://oao.sysykeji.top

function add(a, b) return a + b end
来源：http://jrt.jinyuanbaomall.cn

[T37] Lua：字符串拼接
来源：http://sxo.hfpthk.cn

"a" .. "b"
来源：http://vcp.yj202588.top

[T38] Lua：条件
来源：http://mpz.jyoumei.cn

if x > 0 then print("正") end
来源：http://yrx.yangfankeji.com

[T39] Lua：模式匹配
来源：http://tvl.tanke756.top

string.find(s, "%d+")
来源：http://tql.fehbvm.com

[T40] Lua：元表
来源：http://nfx.yj202588.top

setmetatable({}, { __index = base })
来源：http://ddb.cdnleiting.top

[T41] Perl：Hello World
来源：http://myt.yongpay.top

print "Hello\n";
来源：http://zzr.shanyushiyangkeji.top

[T42] Perl：变量类型
来源：http://lkd.nanxuanxn.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fyh.zhoulong.xyz

[T43] Perl：字符串插值
来源：http://wiy.jinyuanbaomall.cn

"值: $a"
来源：http://mbs.tian-w.cn

[T44] Perl：条件
来源：http://wzu.zdbjq.cn

if ($a > 0) { print "正"; }
来源：http://olf.tarul.cn

[T45] Perl：数组遍历
来源：http://phd.hysaishi.cn

for my $x (@arr) { print $x; }
来源：http://zrz.feifeiyinyue.top

[T46] Perl：哈希操作
来源：http://iph.chenlongwang.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vxd.ppjwa.cn

[T47] Perl：正则捕获
来源：http://xfc.bbcook.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kyf.jqgfzy.top

[T48] Perl：正则替换
来源：http://nsf.fzhhl.top

$s =~ s/old/new/g;
来源：http://hmf.bjfxy.top

[T49] Perl：函数
来源：http://gfd.jqgfzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lfa.yuxming.cn

[T50] Perl：逐行读文件
来源：http://xeg.jyoumei.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://pci.fzhhl.top

while (my $line = <$fh>) { print $line; }
来源：http://zcy.vqdsnc.cn

[T51] Scala：Hello World
来源：http://ueb.ctjpmb.com

println("Hello")
来源：http://gzg.zhijiandao.cn

[T52] Scala：变量
来源：http://htm.pengpengdd.cyou

val a = 1;  var b = 2
来源：http://lhs.52xcode.cn

[T53] Scala：字符串插值
来源：http://xcc.cashguo.top

s"值: $b"
来源：http://mkl.nanxuanxn.top

[T54] Scala：集合映射
来源：http://ntw.jinghuilouyu.cn

List(1, 2, 3).map(_ * 2)
来源：http://aki.zhongyouzk.top

[T55] Scala：集合过滤
来源：http://qho.hysaishi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jig.nanxinkj.top

[T56] Scala：样例类
来源：http://hmu.shzxlz.cn

case class User(name: String, age: Int)
来源：http://ovl.meibo888.top

[T57] Scala：模式匹配
来源：http://dnh.316326.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://afo.zhixingplan.top

[T58] Scala：函数定义
来源：http://xmf.havefunace.top

def add(a: Int, b: Int): Int = a + b
来源：http://qos.hnqzz.top

[T59] Scala：循环
来源：http://ico.hesvh.cn

for (i <- 1 to 10) println(i)
来源：http://clc.dianchejie.cn

[T60] Scala：折叠
来源：http://xpr.chenzaomai.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://msc.hesvh.cn

================================================================================
来源：http://jjm.meibo888.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mhm.wangdashe.top

================================================================================
来源：http://fph.gaohongyu789.top

[U01] Py：创建虚拟环境
来源：http://jrg.svipenyu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hro.yongpay.top

[U02] Py：导出 / 安装依赖
来源：http://zbi.dashuyun.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ibf.sweek.top

[U03] Py：加载 .env 配置
来源：http://gzz.kuanghao11.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ozv.feifeiyinyue.top

[U04] Py：变量调试打印
来源：http://tcp.xuanzx.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://khd.chenjidiqi.icu


<!-- 参考信息 -->