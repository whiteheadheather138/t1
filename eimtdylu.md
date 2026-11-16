代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yjt.chenjidiqi.icu

[R66] 定时任务
来源：http://thl.epnwcf.com

crontab -e;  crontab -l
来源：http://iqy.tarul.cn

[R67] 生成随机十六进制串
来源：http://elu.jinqigfzy.top

openssl rand -hex 16
来源：http://xbd.0kj1m.cn

[R68] 计算文件校验值
来源：http://mvh.zhiwuduotai.top

sha256sum a.txt;  md5sum a.txt
来源：http://tvy.zhoulong.xyz

[R69] 生成随机密码
来源：http://nis.fehbvm.com

head -c 16 /dev/urandom | base64
来源：http://tya.cashguo.top

[R70] 时间戳与互转
来源：http://kgu.zdbjq.cn

date +%s;  date -d @1700000000
来源：http://nls.ydzc1.top

[R71] 日期格式化
来源：http://kbp.tanke756.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://kgn.guowangkeji.top

[R72] 等待端口就绪
来源：http://gcw.aibaodan.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ytp.sjlbkw.cn

[R73] 分割大日志
来源：http://gsz.yonumen.top

split -l 1000 big.log part_
来源：http://gon.pengpengdd.cyou

[R74] 批量重命名
来源：http://txl.0kj1m.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iya.fengsongda.top

[R75] 导出环境变量
来源：http://qdk.hysaishi.cn

export PATH="$HOME/bin:$PATH"
来源：http://ctx.zycfv.cn

[R76] 使用临时文件
来源：http://sfq.cheryme.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dje.aibaodan.cn

[R77] 读取用户输入
来源：http://zma.yvedp.cn

read -rp "请输入: " ans
来源：http://jxu.316326.xyz

[R78] 交互式菜单
来源：http://ruu.vehdjk.com

select opt in a b c; do echo "$opt"; break; done
来源：http://fye.sxryk.cn

[R79] 解析命令行选项
来源：http://hhq.xylfe.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://djj.hywenlv.cn

[R80] 查看脚本执行耗时
来源：http://rnv.gaohongyu789.top

time ./run.sh
来源：http://mct.chenlongwang.top

================================================================================
来源：http://biq.52xcode.cn

S. C / C++ 专题
来源：http://qxf.gaohongyu789.top

================================================================================
来源：http://bca.cashguo.top

[S01] C：Hello World
来源：http://kpk.xylfe.cn

#include <stdio.h>
来源：http://aml.gzhubu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://sgo.xuanzx.com

[S02] C：变量与格式化输出
来源：http://iba.fzhhl.top

int a = 10; printf("%d\n", a);
来源：http://ett.cucudq.cn

[S03] C：读入整数
来源：http://jsi.sysykeji.top

int x; scanf("%d", &x);
来源：http://uez.gogol.net.cn

[S04] C：字符串复制
来源：http://uss.zhengqikj.top

char dst[32]; strcpy(dst, "hi");
来源：http://sqw.shanyushiyangkeji.top

[S05] C：字符串长度
来源：http://opn.9152youxi.cn

strlen(s)
来源：http://rxu.sweek.top

[S06] C：字符串比较
来源：http://hid.yangfankeji.com

strcmp(a, b) == 0
来源：http://gwd.yfazqb.com

[S07] C：数组遍历求和
来源：http://dfy.vqdsnc.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wyg.xuetiantiany.cn

[S08] C：动态内存分配与释放
来源：http://kom.hywenlv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ywd.chenjidiqi.icu

[S09] C：结构体定义与初始化
来源：http://rht.zhiwuduotai.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dbk.gogol.net.cn

[S10] C：指针与解引用
来源：http://lgo.ydzc1.top

int *p = &a;  *p = 5;
来源：http://wct.hnxiangtu.top

[S11] C：逐行读文件
来源：http://qev.yfazqb.com

FILE *f = fopen("a.txt", "r");
来源：http://lok.shanyushiyangkeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://dde.chenzaomai.com

fclose(f);
来源：http://uqj.yfazqb.com

[S12] C：写文件
来源：http://hkf.gotoacloud.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bvm.dashuyun.cn

[S13] C：宏定义
来源：http://dph.hfpthk.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qre.daxiang520.top

[S14] C：枚举
来源：http://pdl.sysykeji.top

enum Color { RED, GREEN, BLUE };
来源：http://xpw.guowangkeji.top

[S15] C：类型转换
来源：http://mno.shuidangran.top

(double) a / b
来源：http://ncq.shangyingyoupin.top

[S16] C：位操作置位
来源：http://qrw.fengsongda.top

x |= (1 << 3);
来源：http://kps.redwolf501.top

[S17] C：安全拼接字符串
来源：http://ceu.jinghuilouyu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ssj.9152youxi.cn

[S18] C：命令行参数
来源：http://fwm.52xcode.cn

int main(int argc, char **argv)
来源：http://tls.jqgufenzy.top

[S19] C：快速排序
来源：http://ntj.tanke756.top

qsort(a, n, sizeof(int), cmp);
来源：http://evz.dianchejie.cn

[S20] C：二分查找
来源：http://fat.zycfv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hvz.tian-w.cn

[S21] C：字符类别判断
来源：http://mbj.hnxiangtu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ors.ehwqpu.com

[S22] C：字符串转数字
来源：http://axh.cheryme.top

atoi("42");  strtod("3.14", NULL);
来源：http://tbg.zhixingplan.top

[S23] C：随机数
来源：http://sdv.meibo888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://nss.jyoumei.cn

[S24] C：获取本地时间
来源：http://pab.pengpengdd.cyou

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kzj.shanyushiyangtech.top

[S25] C：内存拷贝
来源：http://vma.yangfankeji.com

memcpy(dst, src, n);
来源：http://pcs.snrcjt.cn

[S26] C：内存清零
来源：http://nkv.hammf.cn

memset(a, 0, sizeof a);
来源：http://oah.jinqigfzy.top

[S27] C：定义常量
来源：http://rlx.meibo888.top

const double PI = 3.14159;
来源：http://elc.cqqwz.cn

[S28] C：静态变量
来源：http://mna.zhengqikj.top

static int counter = 0;
来源：http://sza.haohaochexian.top

[S29] C：变参函数
来源：http://bbk.yuxming.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://egf.jinghuilouyu.cn

[S30] C：头文件保护
来源：http://fgi.nanxinkj.top

#ifndef X_H
来源：http://wdy.epnwcf.com

#define X_H
来源：http://yaa.jlsjyb.cn

#endif
来源：http://fwb.fktsv.cn

[S31] C++：Hello World
来源：http://van.redwolf501.top

#include <iostream>
来源：http://lhu.birdmap.top

int main() { std::cout << "Hello\n"; }
来源：http://bwa.yj202588.top

[S32] C++：字符串
来源：http://gar.yuxming.cn

std::string s = "hi";  s += "!";
来源：http://aqq.aibaodan.cn

[S33] C++：vector 增删
来源：http://wrp.chenzaomai.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rlk.iojbl.cn

[S34] C++：遍历 vector
来源：http://kby.cqqwz.cn

for (auto &x : v) { std::cout << x; }
来源：http://xuo.zdbjq.cn

[S35] C++：map
来源：http://xux.hnxiangtu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tkn.cqqwz.cn

[S36] C++：unordered_map
来源：http://qxa.yj20258.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lvc.hywenlv.cn

[S37] C++：set
来源：http://edg.gzhubu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://btf.gaohongyu789.top

[S38] C++：排序
来源：http://gnc.epnwcf.com

std::sort(v.begin(), v.end());
来源：http://dzr.cqqwz.cn

[S39] C++：自定义比较器排序
来源：http://aeh.iojbl.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ljn.shanyushiyangkeji.top

[S40] C++：查找元素
来源：http://bmo.havefunace.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://boq.jiagoushi.top

[S41] C++：类与构造函数
来源：http://hjz.shanyushiyangtech.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cbg.wangshuangyany.cn

[S42] C++：继承与虚函数
来源：http://zja.zhijiandao.cn

class B : public Base { public: void f() override {} };
来源：http://gge.gotoacloud.top

[S43] C++：智能指针
来源：http://chj.jinghuilouyu.cn

auto p = std::make_unique<int>(5);
来源：http://vtp.dashuyun.cn

[S44] C++：引用传参
来源：http://snj.snrcjt.cn

void inc(int &x) { ++x; }
来源：http://hlt.xziqi.cn

[S45] C++：lambda
来源：http://cls.sweek.top

auto add = [](int a, int b) { return a + b; };
来源：http://zvn.sysykeji.top

[S46] C++：函数模板
来源：http://ctl.ppjwa.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gby.xingfuxueyuan.xyz

[S47] C++：结构化绑定遍历
来源：http://xbq.tianlin.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://grb.meibo888.top

[S48] C++：逐行读文件
来源：http://ook.yvedp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://iwj.shanyushiyangtech.top

while (std::getline(in, line)) { }
来源：http://wro.cashguo.top

[S49] C++：写文件
来源：http://alj.feifeiyinyue.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://keo.316326.xyz

[S50] C++：格式化数字
来源：http://jpu.xuetiantiany.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://glm.sysykeji.top

[S51] C++：显式类型转换
来源：http://jwe.yanxiufei.cn

static_cast<double>(a) / b
来源：http://ssr.shuidangran.top

[S52] C++：const 与 noexcept
来源：http://igi.gotoacloud.top

int size() const noexcept { return n_; }
来源：http://wtq.yj20258.top

[S53] C++：移动语义
来源：http://gaw.shuidangran.top

std::vector<int> w = std::move(v);
来源：http://mzb.wangshuangyany.cn

[S54] C++：异常处理
来源：http://rdd.mhx1999.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lvs.shanyushiyangtech.top

[S55] C++：结构化绑定
来源：http://lnh.hongshengwenyu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jxv.sysykeji.top

[S56] C++：optional
来源：http://yiz.yanxiufei.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mvp.xuetiantiany.cn

[S57] C++：编译期常量
来源：http://acl.kuanghao11.cn

constexpr int N = 10;
来源：http://kjh.jiagoushi.top

[S58] C++：命名空间
来源：http://xkp.chenzaomai.com

namespace ns { int f() { return 1; } }
来源：http://nri.bbcook.cn

[S59] C++：静态断言
来源：http://fim.0kj1m.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ogv.ivvv.top

[S60] C++：遍历并删除元素
来源：http://kxg.sufxvd.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://huy.feifeiyinyue.top

================================================================================
来源：http://yvr.aizwys.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tmi.yfazqb.com

================================================================================
来源：http://arw.snrcjt.cn

[T01] Kotlin：Hello World
来源：http://aoz.hnqzz.top

println("Hello")
来源：http://kbi.hongshengwenyu.top

[T02] Kotlin：变量
来源：http://vfz.zhongyouzk.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jdq.epnwcf.com

[T03] Kotlin：字符串模板
来源：http://its.xziqi.cn

"值: $b"
来源：http://fsb.0kj1m.cn

[T04] Kotlin：空安全
来源：http://fvq.cdnleiting.top

val n: String? = null;  n?.length
来源：http://gas.ivvv.top

[T05] Kotlin：when 表达式
来源：http://iui.fzhhl.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yws.wangshuangyany.cn

[T06] Kotlin：集合映射
来源：http://hnq.pengpengdd.cyou

listOf(1, 2, 3).map { it * 2 }
来源：http://qon.hcnkem.com

[T07] Kotlin：集合过滤
来源：http://bbp.tanke756.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kwx.hongshengwenyu.top

[T08] Kotlin：数据类
来源：http://pap.nwbrower.top

data class User(val name: String, val age: Int)
来源：http://ngj.0kj1m.cn

[T09] Kotlin：扩展函数
来源：http://ryj.xziqi.cn

fun String.exclaim() = this + "!"
来源：http://jtl.gzhubu.top

[T10] Kotlin：默认参数
来源：http://kgt.0kj1m.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jnd.haohaochexian.top

[T11] Kotlin：协程
来源：http://uyo.gzhubu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://hum.hesvh.cn

[T12] Kotlin：解构声明
来源：http://tjg.yonumen.top

val (a, b) = Pair(1, 2)
来源：http://gwv.haohaochexian.top

[T13] Kotlin：只读 Map
来源：http://rqy.bjfxy.top

val m = mapOf("a" to 1)
来源：http://hrb.sxryk.cn

[T14] Kotlin：循环
来源：http://xcp.uphjek.com

for (i in 1..10) println(i)
来源：http://chp.sufxvd.cn

[T15] Kotlin：接口
来源：http://iep.xingfuxueyuan.xyz

interface Shape { fun area(): Double }
来源：http://llt.316326.xyz

[T16] Swift：Hello World
来源：http://pmi.vqdsnc.cn

print("Hello")
来源：http://xov.zdqjudy.top

[T17] Swift：变量与常量
来源：http://nvx.cashguo.top

var a = 1;  let b = 2
来源：http://tpr.ehwqpu.com

[T18] Swift：字符串插值
来源：http://skw.fanxiaobao.xyz

"值: \(b)"
来源：http://jpu.chenzaomai.com

[T19] Swift：可选绑定
来源：http://oag.hysaishi.cn

if let n = opt { print(n) }
来源：http://bqg.daxiang520.top

[T20] Swift：数组操作
来源：http://ylh.hnqzz.top

var a = [1, 2, 3];  a.append(4)
来源：http://xib.tian-w.cn

[T21] Swift：遍历
来源：http://hqm.tianlin.xyz

for x in a { print(x) }
来源：http://btv.c1oappe.top

[T22] Swift：字典
来源：http://smx.zdqjudy.top

var d = ["a": 1];  d["b"] = 2
来源：http://tcz.hfpthk.cn

[T23] Swift：函数
来源：http://rtn.yangfankeji.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cxs.52xcode.cn

[T24] Swift：闭包
来源：http://hnk.shzxlz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://axj.c1oappe.top

[T25] Swift：结构体
来源：http://xdf.hnxiangtu.top

struct P { var x: Int }
来源：http://cff.xuetiantiany.cn

[T26] Swift：类与重写
来源：http://loj.hongshengwenyu.top

class A: Base { override func f() {} }
来源：http://odl.tianlin.xyz

[T27] Swift：错误处理
来源：http://yfm.9152youxi.cn

do { try f() } catch { print(error) }
来源：http://ulb.sjlbkw.cn

[T28] Swift：枚举
来源：http://ibt.yangfankeji.com

enum Color { case red, green }
来源：http://lku.ppjwa.cn

[T29] Swift：guard 提前返回
来源：http://qif.zdbjq.cn

guard let x = opt else { return }
来源：http://fix.cucudq.cn

[T30] Swift：协议
来源：http://jmn.havefunace.top

protocol Shape { func area() -> Double }
来源：http://sbo.zhijiandao.cn

[T31] Lua：Hello World
来源：http://ouq.uphjek.com

print("Hello")
来源：http://kqh.ybcxt.top

[T32] Lua：局部变量
来源：http://ktx.bjfxy.top

local a = 1
来源：http://vpg.xingfuxueyuan.xyz

[T33] Lua：表（数组）
来源：http://goo.jinyuanbaomall.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://pri.shuidangran.top

[T34] Lua：遍历表
来源：http://iiv.sxryk.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://sew.cheryme.top

[T35] Lua：字典表
来源：http://bwc.chenzaomai.com

local d = { a = 1 };  d.b = 2
来源：http://lht.zhengqikj.top

[T36] Lua：函数
来源：http://vxg.birdmap.top

function add(a, b) return a + b end
来源：http://qbi.xingfuxueyuan.xyz

[T37] Lua：字符串拼接
来源：http://dme.ctjpmb.com

"a" .. "b"
来源：http://pde.shangyingyoupin.top

[T38] Lua：条件
来源：http://uat.yj20258.top

if x > 0 then print("正") end
来源：http://zbb.zdbjq.cn

[T39] Lua：模式匹配
来源：http://vlp.dianchejie.cn

string.find(s, "%d+")
来源：http://sey.gaohongyu789.top

[T40] Lua：元表
来源：http://shn.hywenlv.cn

setmetatable({}, { __index = base })
来源：http://mzr.quarkkingdee.top

[T41] Perl：Hello World
来源：http://lwx.wangdashe.top

print "Hello\n";
来源：http://sny.jlsjyb.cn

[T42] Perl：变量类型
来源：http://oup.yueranfly.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pmp.cqqwz.cn

[T43] Perl：字符串插值
来源：http://eoe.fanxiaobao.xyz

"值: $a"
来源：http://xtm.hongshengwenyu.top

[T44] Perl：条件
来源：http://vec.tian-w.cn

if ($a > 0) { print "正"; }
来源：http://hww.dashuyun.cn

[T45] Perl：数组遍历
来源：http://xpl.jlsjyb.cn

for my $x (@arr) { print $x; }
来源：http://pjq.smart0.xyz

[T46] Perl：哈希操作
来源：http://fgl.sweek.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://juh.zhongyouzk.top

[T47] Perl：正则捕获
来源：http://arf.zhijiandao.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nsl.yfazqb.com

[T48] Perl：正则替换
来源：http://njl.zhaomingkeji.xyz

$s =~ s/old/new/g;
来源：http://ykm.redwolf501.top

[T49] Perl：函数
来源：http://pia.ywan-chungtsiang.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mfl.snrcjt.cn

[T50] Perl：逐行读文件
来源：http://kap.quarkkingdee.top

open my $fh, "<", "a.txt" or die $!;
来源：http://wge.0kj1m.cn

while (my $line = <$fh>) { print $line; }
来源：http://rlq.sjlbkw.cn

[T51] Scala：Hello World
来源：http://pfv.dianchejie.cn

println("Hello")
来源：http://uiw.9152youxi.cn

[T52] Scala：变量
来源：http://vym.yj202588.top

val a = 1;  var b = 2
来源：http://bts.yj20258.top

[T53] Scala：字符串插值
来源：http://thn.hywenlv.cn

s"值: $b"
来源：http://izw.andypj.xyz

[T54] Scala：集合映射
来源：http://zib.yj20258.top

List(1, 2, 3).map(_ * 2)
来源：http://tzf.redwolf501.top

[T55] Scala：集合过滤
来源：http://qcq.chenlongwang.top

List(1, 2, 3).filter(_ > 1)
来源：http://bby.tian-w.cn

[T56] Scala：样例类
来源：http://clb.xuanzx.com

case class User(name: String, age: Int)
来源：http://bji.jianghu66.top

[T57] Scala：模式匹配
来源：http://xph.fzhhl.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ohe.hnqzz.top

[T58] Scala：函数定义
来源：http://gtn.zhijiandao.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xgc.c1oappe.top

[T59] Scala：循环
来源：http://yof.cashguo.top

for (i <- 1 to 10) println(i)
来源：http://mjh.zycfv.cn

[T60] Scala：折叠
来源：http://luf.guannengcc.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cko.hcnkem.com

================================================================================
来源：http://erh.yueranfly.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dgq.uphjek.com

================================================================================
来源：http://mpw.hcnkem.com

[U01] Py：创建虚拟环境
来源：http://fzo.jyoumei.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xng.guannengcc.top

[U02] Py：导出 / 安装依赖
来源：http://gdu.jlsjyb.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tkk.hfpthk.cn

[U03] Py：加载 .env 配置
来源：http://sjy.tianlin.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://mrl.vqdsnc.cn

[U04] Py：变量调试打印
来源：http://vfj.cucudq.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://efi.andypj.xyz

[U05] Py：列表去重且保序
来源：http://yob.yongpay.top

list(dict.fromkeys(arr))
来源：http://svr.jqgfzy.top

[U06] Py：合并两个字典
来源：http://zvq.yongpay.top

{**a, **b}
来源：http://njw.zhengqikj.top


<!-- 参考信息 -->