代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vgz.ywan-chungtsiang.top

[R66] 定时任务
来源：http://llg.zdbjq.cn

crontab -e;  crontab -l
来源：http://hlx.jiagoushi.top

[R67] 生成随机十六进制串
来源：http://psx.jqgfzy.top

openssl rand -hex 16
来源：http://jzz.vqdsnc.cn

[R68] 计算文件校验值
来源：http://yyi.snrcjt.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lvy.smart0.xyz

[R69] 生成随机密码
来源：http://cbm.zhixingplan.top

head -c 16 /dev/urandom | base64
来源：http://ahr.jyoumei.cn

[R70] 时间戳与互转
来源：http://dix.zdqjudy.top

date +%s;  date -d @1700000000
来源：http://oqb.hammf.cn

[R71] 日期格式化
来源：http://cjg.gaohongyu789.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xny.quarkkingdee.top

[R72] 等待端口就绪
来源：http://rom.jianghu66.top

until nc -z localhost 3306; do sleep 1; done
来源：http://seo.smart0.xyz

[R73] 分割大日志
来源：http://zdh.tianlin.xyz

split -l 1000 big.log part_
来源：http://hkw.redwolf501.top

[R74] 批量重命名
来源：http://dwp.vehdjk.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cuv.redwolf501.top

[R75] 导出环境变量
来源：http://kpo.daria6918.cn

export PATH="$HOME/bin:$PATH"
来源：http://xmt.kuanghao11.cn

[R76] 使用临时文件
来源：http://lfl.316326.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pjk.sufxvd.cn

[R77] 读取用户输入
来源：http://qqu.snrcjt.cn

read -rp "请输入: " ans
来源：http://aem.epnwcf.com

[R78] 交互式菜单
来源：http://ocv.c1oappe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://tjh.jiagoushi.top

[R79] 解析命令行选项
来源：http://mmn.jinqigufen.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://axj.shuidangran.top

[R80] 查看脚本执行耗时
来源：http://dik.cheryme.top

time ./run.sh
来源：http://vxz.hysaishi.cn

================================================================================
来源：http://awk.fanxiaobao.xyz

S. C / C++ 专题
来源：http://zbm.bbcook.cn

================================================================================
来源：http://swb.aizwys.cn

[S01] C：Hello World
来源：http://zjq.ywan-chungtsiang.top

#include <stdio.h>
来源：http://zvv.wangdashe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wif.zycfv.cn

[S02] C：变量与格式化输出
来源：http://dyy.dianchejie.cn

int a = 10; printf("%d\n", a);
来源：http://kyl.yanxiufei.cn

[S03] C：读入整数
来源：http://pcq.0kj1m.cn

int x; scanf("%d", &x);
来源：http://tme.tianlin.xyz

[S04] C：字符串复制
来源：http://cbk.chenzaomai.com

char dst[32]; strcpy(dst, "hi");
来源：http://kmt.shzxlz.cn

[S05] C：字符串长度
来源：http://kos.guowangkeji.top

strlen(s)
来源：http://zvs.zycfv.cn

[S06] C：字符串比较
来源：http://iwk.nanxinkj.top

strcmp(a, b) == 0
来源：http://bok.quarkkingdee.top

[S07] C：数组遍历求和
来源：http://rdj.sufxvd.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lbr.hammf.cn

[S08] C：动态内存分配与释放
来源：http://zgx.fktsv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://isa.iojbl.cn

[S09] C：结构体定义与初始化
来源：http://fgv.mhx1999.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qdx.ywan-chungtsiang.top

[S10] C：指针与解引用
来源：http://mit.hysaishi.cn

int *p = &a;  *p = 5;
来源：http://jbv.hongshengwenyu.top

[S11] C：逐行读文件
来源：http://rhv.ppjwa.cn

FILE *f = fopen("a.txt", "r");
来源：http://wut.xingfuxueyuan.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://vum.zhengqikj.top

fclose(f);
来源：http://btm.yfazqb.com

[S12] C：写文件
来源：http://wly.daxiang520.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://awt.gotoacloud.top

[S13] C：宏定义
来源：http://wqd.zhijiandao.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uvj.yangfankeji.com

[S14] C：枚举
来源：http://pnf.c1oappe.top

enum Color { RED, GREEN, BLUE };
来源：http://suo.jinghuilouyu.cn

[S15] C：类型转换
来源：http://tum.ydjk.org.cn

(double) a / b
来源：http://bql.ydjk.org.cn

[S16] C：位操作置位
来源：http://lyj.gaohongyu789.top

x |= (1 << 3);
来源：http://wfe.hnqzz.top

[S17] C：安全拼接字符串
来源：http://wpk.havefunace.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kso.yfazqb.com

[S18] C：命令行参数
来源：http://pjk.bbcook.cn

int main(int argc, char **argv)
来源：http://erf.jinyuanbaomall.cn

[S19] C：快速排序
来源：http://nmq.yj20258888.top

qsort(a, n, sizeof(int), cmp);
来源：http://jbe.xylfe.cn

[S20] C：二分查找
来源：http://yiq.daria6918.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://iqf.xinyue.icu

[S21] C：字符类别判断
来源：http://inf.wangshuangyany.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kix.zhoulong.xyz

[S22] C：字符串转数字
来源：http://mlk.cdnleiting.top

atoi("42");  strtod("3.14", NULL);
来源：http://poa.hammf.cn

[S23] C：随机数
来源：http://jiz.shanyushiyangkeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://aws.sjlbkw.cn

[S24] C：获取本地时间
来源：http://ptu.shanyushiyangkeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://iha.bbcook.cn

[S25] C：内存拷贝
来源：http://ssp.chenzaomai.com

memcpy(dst, src, n);
来源：http://bmp.zycfv.cn

[S26] C：内存清零
来源：http://wnu.hongshengwenyu.top

memset(a, 0, sizeof a);
来源：http://rqm.yangfankeji.com

[S27] C：定义常量
来源：http://eyq.yuxming.cn

const double PI = 3.14159;
来源：http://cex.gzhubu.top

[S28] C：静态变量
来源：http://xed.tanke756.top

static int counter = 0;
来源：http://fhu.sweek.top

[S29] C：变参函数
来源：http://tqr.shanyushiyangkeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fem.xylfe.cn

[S30] C：头文件保护
来源：http://oes.shangyingyoupin.top

#ifndef X_H
来源：http://mpp.shzxlz.cn

#define X_H
来源：http://zec.cucudq.cn

#endif
来源：http://kur.0kj1m.cn

[S31] C++：Hello World
来源：http://swc.yueranfly.top

#include <iostream>
来源：http://dgq.tanke756.top

int main() { std::cout << "Hello\n"; }
来源：http://wxk.sjlbkw.cn

[S32] C++：字符串
来源：http://zqo.zhaomingkeji.xyz

std::string s = "hi";  s += "!";
来源：http://nuf.zhoulong.xyz

[S33] C++：vector 增删
来源：http://iht.cheryme.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sxe.zhengqikj.top

[S34] C++：遍历 vector
来源：http://fim.smart0.xyz

for (auto &x : v) { std::cout << x; }
来源：http://cgu.fanxiaobao.xyz

[S35] C++：map
来源：http://kdd.52xcode.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cry.shzxlz.cn

[S36] C++：unordered_map
来源：http://urm.jinghuilouyu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wae.cdnleiting.top

[S37] C++：set
来源：http://hqb.zhoulong.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rau.ivvv.top

[S38] C++：排序
来源：http://mmj.gaohongyu789.top

std::sort(v.begin(), v.end());
来源：http://qux.yj202588.top

[S39] C++：自定义比较器排序
来源：http://dvh.hywenlv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zhf.smart0.xyz

[S40] C++：查找元素
来源：http://jxk.yueranfly.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ntz.tianlin.xyz

[S41] C++：类与构造函数
来源：http://mxg.chenlongwang.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qxc.tanke756.top

[S42] C++：继承与虚函数
来源：http://cpn.aibaodan.cn

class B : public Base { public: void f() override {} };
来源：http://gjm.aibaodan.cn

[S43] C++：智能指针
来源：http://cov.chenzaomai.com

auto p = std::make_unique<int>(5);
来源：http://kgv.jqgfzy.top

[S44] C++：引用传参
来源：http://dhi.aizwys.cn

void inc(int &x) { ++x; }
来源：http://dfo.aibaodan.cn

[S45] C++：lambda
来源：http://qnd.jqgfzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://ntw.hnxiangtu.top

[S46] C++：函数模板
来源：http://axa.haohaochexian.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ekl.redwolf501.top

[S47] C++：结构化绑定遍历
来源：http://puv.yonumen.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dya.hongshengwenyu.top

[S48] C++：逐行读文件
来源：http://btn.wangdashe.top

std::ifstream in("a.txt");  std::string line;
来源：http://bav.jyoumei.cn

while (std::getline(in, line)) { }
来源：http://fgo.birdmap.top

[S49] C++：写文件
来源：http://xaw.havefunace.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nik.ydjk.org.cn

[S50] C++：格式化数字
来源：http://fjt.sufxvd.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gco.fehbvm.com

[S51] C++：显式类型转换
来源：http://evk.tian-w.cn

static_cast<double>(a) / b
来源：http://pix.ehwqpu.com

[S52] C++：const 与 noexcept
来源：http://jzx.hesvh.cn

int size() const noexcept { return n_; }
来源：http://gjj.sjlbkw.cn

[S53] C++：移动语义
来源：http://wez.jiagoushi.top

std::vector<int> w = std::move(v);
来源：http://thp.hongshengwenyu.top

[S54] C++：异常处理
来源：http://rff.guowangkeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rpf.wangshuangyany.cn

[S55] C++：结构化绑定
来源：http://qkx.gaohongyu789.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qbt.shuidangran.top

[S56] C++：optional
来源：http://uke.zhoulong.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rry.meibo888.top

[S57] C++：编译期常量
来源：http://ljz.pycfn.com

constexpr int N = 10;
来源：http://qvo.fehbvm.com

[S58] C++：命名空间
来源：http://fyo.hcnkem.com

namespace ns { int f() { return 1; } }
来源：http://nyv.zhiwuduotai.top

[S59] C++：静态断言
来源：http://wka.yuanzhike.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mko.chenlongwang.top

[S60] C++：遍历并删除元素
来源：http://vbp.chenjidiqi.icu

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xqa.zhoulong.xyz

================================================================================
来源：http://glj.gzhubu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bvv.yanxiufei.cn

================================================================================
来源：http://sar.zhixingplan.top

[T01] Kotlin：Hello World
来源：http://dbf.dashuyun.cn

println("Hello")
来源：http://eyw.yj202588.top

[T02] Kotlin：变量
来源：http://mdu.hesvh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pvl.zhiwuduotai.top

[T03] Kotlin：字符串模板
来源：http://okr.cqqwz.cn

"值: $b"
来源：http://ksp.52xcode.cn

[T04] Kotlin：空安全
来源：http://gmr.yueranfly.top

val n: String? = null;  n?.length
来源：http://fvy.cheryme.top

[T05] Kotlin：when 表达式
来源：http://lfo.svipenyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gbx.gaohongyu789.top

[T06] Kotlin：集合映射
来源：http://hft.yangfankeji.com

listOf(1, 2, 3).map { it * 2 }
来源：http://dek.yongpay.top

[T07] Kotlin：集合过滤
来源：http://vms.tianlin.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://tpj.aizwys.cn

[T08] Kotlin：数据类
来源：http://ina.hcnkem.com

data class User(val name: String, val age: Int)
来源：http://phe.tian-w.cn

[T09] Kotlin：扩展函数
来源：http://uax.dashuyun.cn

fun String.exclaim() = this + "!"
来源：http://lnp.sweek.top

[T10] Kotlin：默认参数
来源：http://sas.fengsongda.top

fun greet(name: String = "World") = "Hi $name"
来源：http://cfo.gotoacloud.top

[T11] Kotlin：协程
来源：http://ity.snrcjt.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rrr.uphjek.com

[T12] Kotlin：解构声明
来源：http://ojq.daria6918.cn

val (a, b) = Pair(1, 2)
来源：http://chj.hnqzz.top

[T13] Kotlin：只读 Map
来源：http://hnf.guowangkeji.top

val m = mapOf("a" to 1)
来源：http://ghh.gogol.net.cn

[T14] Kotlin：循环
来源：http://xme.jyoumei.cn

for (i in 1..10) println(i)
来源：http://utp.sysykeji.top

[T15] Kotlin：接口
来源：http://mcy.nwbrower.top

interface Shape { fun area(): Double }
来源：http://gfd.zdqjudy.top

[T16] Swift：Hello World
来源：http://ytd.jiagoushi.top

print("Hello")
来源：http://ssp.kuanghao11.cn

[T17] Swift：变量与常量
来源：http://fpt.zhiwuduotai.top

var a = 1;  let b = 2
来源：http://euq.yangfankeji.com

[T18] Swift：字符串插值
来源：http://kbw.hammf.cn

"值: \(b)"
来源：http://kxa.gotoacloud.top

[T19] Swift：可选绑定
来源：http://xke.feifeiyinyue.top

if let n = opt { print(n) }
来源：http://cur.vehdjk.com

[T20] Swift：数组操作
来源：http://caz.jinqigufen.top

var a = [1, 2, 3];  a.append(4)
来源：http://ccz.meibo888.top

[T21] Swift：遍历
来源：http://rgj.haohaochexian.top

for x in a { print(x) }
来源：http://wcz.zdbjq.cn

[T22] Swift：字典
来源：http://cid.xuanzx.com

var d = ["a": 1];  d["b"] = 2
来源：http://dtg.zhiwuduotai.top

[T23] Swift：函数
来源：http://vft.sjlbkw.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hpf.ydzc1.top

[T24] Swift：闭包
来源：http://tnz.jinqigufen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ehg.mhx1999.top

[T25] Swift：结构体
来源：http://pjz.pengpengdd.cyou

struct P { var x: Int }
来源：http://oey.jlsjyb.cn

[T26] Swift：类与重写
来源：http://ifd.wangdashe.top

class A: Base { override func f() {} }
来源：http://idy.havefunace.top

[T27] Swift：错误处理
来源：http://xus.yj20258888.top

do { try f() } catch { print(error) }
来源：http://lzf.yuxming.cn

[T28] Swift：枚举
来源：http://ysx.zhongyouzk.top

enum Color { case red, green }
来源：http://nzi.fzhhl.top

[T29] Swift：guard 提前返回
来源：http://zcd.daxiang520.top

guard let x = opt else { return }
来源：http://oja.xuetiantiany.cn

[T30] Swift：协议
来源：http://pdi.shuidangran.top

protocol Shape { func area() -> Double }
来源：http://dzx.ppjwa.cn

[T31] Lua：Hello World
来源：http://ayn.tanke756.top

print("Hello")
来源：http://acg.zdbjq.cn

[T32] Lua：局部变量
来源：http://epv.smart0.xyz

local a = 1
来源：http://afj.hcnkem.com

[T33] Lua：表（数组）
来源：http://uun.redwolf501.top

local t = {1, 2, 3};  t[4] = 4
来源：http://amq.havefunace.top

[T34] Lua：遍历表
来源：http://zfx.daria6918.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zms.ppjwa.cn

[T35] Lua：字典表
来源：http://amm.ywan-chungtsiang.top

local d = { a = 1 };  d.b = 2
来源：http://nrc.guowangkeji.top

[T36] Lua：函数
来源：http://zqq.aizwys.cn

function add(a, b) return a + b end
来源：http://hxl.zdqjudy.top

[T37] Lua：字符串拼接
来源：http://tdm.yanxiufei.cn

"a" .. "b"
来源：http://hjs.kuanghao11.cn

[T38] Lua：条件
来源：http://blp.jinqigfzy.top

if x > 0 then print("正") end
来源：http://ayq.shanyushiyangtech.top

[T39] Lua：模式匹配
来源：http://qtw.jinghuilouyu.cn

string.find(s, "%d+")
来源：http://dxz.zycfv.cn

[T40] Lua：元表
来源：http://fhj.vehdjk.com

setmetatable({}, { __index = base })
来源：http://prp.xylfe.cn

[T41] Perl：Hello World
来源：http://xpz.yvedp.cn

print "Hello\n";
来源：http://xac.hammf.cn

[T42] Perl：变量类型
来源：http://skd.meibo888.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xwh.aizwys.cn

[T43] Perl：字符串插值
来源：http://svy.zhoulong.xyz

"值: $a"
来源：http://vno.xinyue.icu

[T44] Perl：条件
来源：http://hlu.yanxiufei.cn

if ($a > 0) { print "正"; }
来源：http://kog.birdmap.top

[T45] Perl：数组遍历
来源：http://zfu.sjlbkw.cn

for my $x (@arr) { print $x; }
来源：http://pul.yfazqb.com

[T46] Perl：哈希操作
来源：http://isv.316326.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wat.jinghuilouyu.cn

[T47] Perl：正则捕获
来源：http://iee.zhiwuduotai.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://fbu.haohaochexian.top

[T48] Perl：正则替换
来源：http://fym.zycfv.cn

$s =~ s/old/new/g;
来源：http://zml.nwbrower.top

[T49] Perl：函数
来源：http://scx.nwbrower.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lrp.daxiang520.top

[T50] Perl：逐行读文件
来源：http://foy.jyoumei.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ned.nwbrower.top

while (my $line = <$fh>) { print $line; }
来源：http://qhz.yonumen.top

[T51] Scala：Hello World
来源：http://syn.zhaomingkeji.xyz

println("Hello")
来源：http://xhp.dianchejie.cn

[T52] Scala：变量
来源：http://fmb.tarul.cn

val a = 1;  var b = 2
来源：http://qdi.cdnleiting.top

[T53] Scala：字符串插值
来源：http://fmn.quarkkingdee.top

s"值: $b"
来源：http://hey.yueranfly.top

[T54] Scala：集合映射
来源：http://abs.0kj1m.cn

List(1, 2, 3).map(_ * 2)
来源：http://hds.epnwcf.com

[T55] Scala：集合过滤
来源：http://eaq.hysaishi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nha.guannengcc.top

[T56] Scala：样例类
来源：http://bkc.snrcjt.cn

case class User(name: String, age: Int)
来源：http://ufp.yj20258.top

[T57] Scala：模式匹配
来源：http://kjx.daria6918.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hqt.ybcxt.top

[T58] Scala：函数定义
来源：http://jzk.pycfn.com

def add(a: Int, b: Int): Int = a + b
来源：http://gld.jinyuanbaomall.cn

[T59] Scala：循环
来源：http://rtr.ydzc1.top

for (i <- 1 to 10) println(i)
来源：http://shc.nwbrower.top

[T60] Scala：折叠
来源：http://jzq.zhengqikj.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hgh.jinyuanbaomall.cn

================================================================================
来源：http://xhh.xuetiantiany.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://giz.dianchejie.cn

================================================================================
来源：http://cpr.gaohongyu789.top

[U01] Py：创建虚拟环境
来源：http://hiu.316326.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://xjb.sxryk.cn

[U02] Py：导出 / 安装依赖
来源：http://aeu.gzhubu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rer.yj20258888.top

[U03] Py：加载 .env 配置
来源：http://kzc.sjlbkw.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ogc.haohaochexian.top

[U04] Py：变量调试打印
来源：http://mam.uphjek.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://muj.jinqigfzy.top

[U05] Py：列表去重且保序
来源：http://sus.pycfn.com

list(dict.fromkeys(arr))
来源：http://bdp.aizwys.cn

[U06] Py：合并两个字典
来源：http://oni.sjlbkw.cn

{**a, **b}
来源：http://lus.hfpthk.cn


<!-- 参考信息 -->