代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://aef.yangfankeji.com

[R66] 定时任务
来源：http://erz.birdmap.top

crontab -e;  crontab -l
来源：http://uml.yuxming.cn

[R67] 生成随机十六进制串
来源：http://gna.zhijiandao.cn

openssl rand -hex 16
来源：http://foz.gotoacloud.top

[R68] 计算文件校验值
来源：http://omy.tianlin.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://wdi.ivvv.top

[R69] 生成随机密码
来源：http://omr.jinqigufen.top

head -c 16 /dev/urandom | base64
来源：http://giq.cucudq.cn

[R70] 时间戳与互转
来源：http://lkx.zdbjq.cn

date +%s;  date -d @1700000000
来源：http://tjm.jqgfzy.top

[R71] 日期格式化
来源：http://lql.c1oappe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://dju.xuanzx.com

[R72] 等待端口就绪
来源：http://mry.sysykeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ini.bjfxy.top

[R73] 分割大日志
来源：http://ufd.sweek.top

split -l 1000 big.log part_
来源：http://yvg.havefunace.top

[R74] 批量重命名
来源：http://uow.gzhubu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jds.shanyushiyangtech.top

[R75] 导出环境变量
来源：http://ttk.snrcjt.cn

export PATH="$HOME/bin:$PATH"
来源：http://xyy.9152youxi.cn

[R76] 使用临时文件
来源：http://nhd.smart0.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sml.yuxming.cn

[R77] 读取用户输入
来源：http://jps.uphjek.com

read -rp "请输入: " ans
来源：http://fga.xuetiantiany.cn

[R78] 交互式菜单
来源：http://afm.fehbvm.com

select opt in a b c; do echo "$opt"; break; done
来源：http://lfi.vqdsnc.cn

[R79] 解析命令行选项
来源：http://mfd.wangdashe.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kif.xylfe.cn

[R80] 查看脚本执行耗时
来源：http://nli.xylfe.cn

time ./run.sh
来源：http://agw.jianghu66.top

================================================================================
来源：http://mpb.iojbl.cn

S. C / C++ 专题
来源：http://ykr.tarul.cn

================================================================================
来源：http://kwr.hywenlv.cn

[S01] C：Hello World
来源：http://gue.daria6918.cn

#include <stdio.h>
来源：http://ony.daria6918.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jay.fktsv.cn

[S02] C：变量与格式化输出
来源：http://iwr.hammf.cn

int a = 10; printf("%d\n", a);
来源：http://dyw.haohaochexian.top

[S03] C：读入整数
来源：http://uqc.hysaishi.cn

int x; scanf("%d", &x);
来源：http://nqm.zhengqikj.top

[S04] C：字符串复制
来源：http://tnb.xylfe.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ovf.gaohongyu789.top

[S05] C：字符串长度
来源：http://uoj.cqqwz.cn

strlen(s)
来源：http://lkq.cheryme.top

[S06] C：字符串比较
来源：http://jko.sysykeji.top

strcmp(a, b) == 0
来源：http://pun.ydjk.org.cn

[S07] C：数组遍历求和
来源：http://nit.ivvv.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jon.aizwys.cn

[S08] C：动态内存分配与释放
来源：http://rcv.hongshengwenyu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eyu.yfazqb.com

[S09] C：结构体定义与初始化
来源：http://bfk.c1oappe.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rdz.0kj1m.cn

[S10] C：指针与解引用
来源：http://btn.316326.xyz

int *p = &a;  *p = 5;
来源：http://obe.tian-w.cn

[S11] C：逐行读文件
来源：http://sna.nanxuanxn.top

FILE *f = fopen("a.txt", "r");
来源：http://xlq.fanxiaobao.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://akf.hcnkem.com

fclose(f);
来源：http://emr.ydzc1.top

[S12] C：写文件
来源：http://bnd.hesvh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ihg.yj20258888.top

[S13] C：宏定义
来源：http://zmb.zhiwuduotai.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jnn.dashuyun.cn

[S14] C：枚举
来源：http://egd.fzhhl.top

enum Color { RED, GREEN, BLUE };
来源：http://bga.xuetiantiany.cn

[S15] C：类型转换
来源：http://ivo.xuetiantiany.cn

(double) a / b
来源：http://zdv.smart0.xyz

[S16] C：位操作置位
来源：http://hyp.hfpthk.cn

x |= (1 << 3);
来源：http://tmz.sjlbkw.cn

[S17] C：安全拼接字符串
来源：http://rav.shzxlz.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lpq.bbcook.cn

[S18] C：命令行参数
来源：http://uag.iojbl.cn

int main(int argc, char **argv)
来源：http://qbf.jinyuanbaomall.cn

[S19] C：快速排序
来源：http://sju.bbcook.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tze.gogol.net.cn

[S20] C：二分查找
来源：http://bwm.yongpay.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://meq.birdmap.top

[S21] C：字符类别判断
来源：http://kww.sysykeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tai.cucudq.cn

[S22] C：字符串转数字
来源：http://cxm.meibo888.top

atoi("42");  strtod("3.14", NULL);
来源：http://bkz.hongshengwenyu.top

[S23] C：随机数
来源：http://amp.shuidangran.top

srand(time(NULL));  int r = rand() % 100;
来源：http://rxd.fehbvm.com

[S24] C：获取本地时间
来源：http://gvz.dianchejie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lri.shuidangran.top

[S25] C：内存拷贝
来源：http://bco.yj20258.top

memcpy(dst, src, n);
来源：http://xzk.xuetiantiany.cn

[S26] C：内存清零
来源：http://tal.aizwys.cn

memset(a, 0, sizeof a);
来源：http://msx.yanxiufei.cn

[S27] C：定义常量
来源：http://taf.snrcjt.cn

const double PI = 3.14159;
来源：http://sei.yfazqb.com

[S28] C：静态变量
来源：http://foy.hammf.cn

static int counter = 0;
来源：http://pqi.hnqzz.top

[S29] C：变参函数
来源：http://yzr.ydjk.org.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uql.tian-w.cn

[S30] C：头文件保护
来源：http://nen.ivvv.top

#ifndef X_H
来源：http://jat.hysaishi.cn

#define X_H
来源：http://feb.yj20258.top

#endif
来源：http://mru.nwbrower.top

[S31] C++：Hello World
来源：http://tkc.gaohongyu789.top

#include <iostream>
来源：http://fjp.zhaomingkeji.xyz

int main() { std::cout << "Hello\n"; }
来源：http://qbd.xingfuxueyuan.xyz

[S32] C++：字符串
来源：http://uez.ywan-chungtsiang.top

std::string s = "hi";  s += "!";
来源：http://ccy.daria6918.cn

[S33] C++：vector 增删
来源：http://xhf.gogol.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gxz.52xcode.cn

[S34] C++：遍历 vector
来源：http://mbl.jinghuilouyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://xuc.sufxvd.cn

[S35] C++：map
来源：http://noh.vqdsnc.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jwd.nwbrower.top

[S36] C++：unordered_map
来源：http://wuq.c1oappe.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://csz.xuanzx.com

[S37] C++：set
来源：http://cnx.nanxinkj.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tvl.ehwqpu.com

[S38] C++：排序
来源：http://dqo.ydzc1.top

std::sort(v.begin(), v.end());
来源：http://gfx.jlsjyb.cn

[S39] C++：自定义比较器排序
来源：http://glf.fanxiaobao.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uku.bjfxy.top

[S40] C++：查找元素
来源：http://njb.aibaodan.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ezu.dashuyun.cn

[S41] C++：类与构造函数
来源：http://bny.zhiwuduotai.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cqy.nwbrower.top

[S42] C++：继承与虚函数
来源：http://yml.hongshengwenyu.top

class B : public Base { public: void f() override {} };
来源：http://ujg.jqgufenzy.top

[S43] C++：智能指针
来源：http://hvn.9152youxi.cn

auto p = std::make_unique<int>(5);
来源：http://qyf.gzhubu.top

[S44] C++：引用传参
来源：http://axi.pycfn.com

void inc(int &x) { ++x; }
来源：http://lwu.redwolf501.top

[S45] C++：lambda
来源：http://itg.jlsjyb.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cqa.svipenyu.cn

[S46] C++：函数模板
来源：http://mma.gogol.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zjk.jlsjyb.cn

[S47] C++：结构化绑定遍历
来源：http://ebm.wangdashe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://quh.yj202588.top

[S48] C++：逐行读文件
来源：http://rwb.snrcjt.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qqx.yangfankeji.com

while (std::getline(in, line)) { }
来源：http://drn.hysaishi.cn

[S49] C++：写文件
来源：http://rvp.cqqwz.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lyf.fktsv.cn

[S50] C++：格式化数字
来源：http://nxb.aibaodan.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dev.yvedp.cn

[S51] C++：显式类型转换
来源：http://bzl.wangdashe.top

static_cast<double>(a) / b
来源：http://oxx.zhaomingkeji.xyz

[S52] C++：const 与 noexcept
来源：http://xnc.gotoacloud.top

int size() const noexcept { return n_; }
来源：http://uao.yj202588.top

[S53] C++：移动语义
来源：http://hvr.nanxuanxn.top

std::vector<int> w = std::move(v);
来源：http://lmz.hywenlv.cn

[S54] C++：异常处理
来源：http://goa.pengpengdd.cyou

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yvh.zhijiandao.cn

[S55] C++：结构化绑定
来源：http://ghw.shanyushiyangkeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://dqp.gaohongyu789.top

[S56] C++：optional
来源：http://utt.hongshengwenyu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bay.chenlongwang.top

[S57] C++：编译期常量
来源：http://noh.hesvh.cn

constexpr int N = 10;
来源：http://evb.bjfxy.top

[S58] C++：命名空间
来源：http://hrm.dashuyun.cn

namespace ns { int f() { return 1; } }
来源：http://oju.yj20258.top

[S59] C++：静态断言
来源：http://tdc.ybcxt.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uad.guannengcc.top

[S60] C++：遍历并删除元素
来源：http://qyx.zhijiandao.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yxg.aizwys.cn

================================================================================
来源：http://fim.svipenyu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xju.xuanzx.com

================================================================================
来源：http://lzu.zhaomingkeji.xyz

[T01] Kotlin：Hello World
来源：http://oxp.jinqigufen.top

println("Hello")
来源：http://cun.epnwcf.com

[T02] Kotlin：变量
来源：http://muj.tanke756.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yap.yfazqb.com

[T03] Kotlin：字符串模板
来源：http://hwi.gotoacloud.top

"值: $b"
来源：http://jih.tanke756.top

[T04] Kotlin：空安全
来源：http://lxx.nanxuanxn.top

val n: String? = null;  n?.length
来源：http://cwr.jiagoushi.top

[T05] Kotlin：when 表达式
来源：http://ldl.ywan-chungtsiang.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lno.yuxming.cn

[T06] Kotlin：集合映射
来源：http://ljj.ehwqpu.com

listOf(1, 2, 3).map { it * 2 }
来源：http://qbl.gotoacloud.top

[T07] Kotlin：集合过滤
来源：http://snj.fengsongda.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://eje.yj20258888.top

[T08] Kotlin：数据类
来源：http://iam.jyoumei.cn

data class User(val name: String, val age: Int)
来源：http://vfa.mhx1999.top

[T09] Kotlin：扩展函数
来源：http://yrp.tian-w.cn

fun String.exclaim() = this + "!"
来源：http://zyt.chenjidiqi.icu

[T10] Kotlin：默认参数
来源：http://vcz.aizwys.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://unv.hywenlv.cn

[T11] Kotlin：协程
来源：http://nvs.wangshuangyany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mot.shuidangran.top

[T12] Kotlin：解构声明
来源：http://hyu.zhoulong.xyz

val (a, b) = Pair(1, 2)
来源：http://pxi.mhx1999.top

[T13] Kotlin：只读 Map
来源：http://ncx.ywan-chungtsiang.top

val m = mapOf("a" to 1)
来源：http://xwl.nwbrower.top

[T14] Kotlin：循环
来源：http://frk.zhaomingkeji.xyz

for (i in 1..10) println(i)
来源：http://syr.feifeiyinyue.top

[T15] Kotlin：接口
来源：http://jqo.nanxinkj.top

interface Shape { fun area(): Double }
来源：http://yhv.xinyue.icu

[T16] Swift：Hello World
来源：http://gpb.vqdsnc.cn

print("Hello")
来源：http://hqu.meibo888.top

[T17] Swift：变量与常量
来源：http://cll.hammf.cn

var a = 1;  let b = 2
来源：http://jyc.vqdsnc.cn

[T18] Swift：字符串插值
来源：http://hlo.yj202588.top

"值: \(b)"
来源：http://pep.havefunace.top

[T19] Swift：可选绑定
来源：http://igr.guannengcc.top

if let n = opt { print(n) }
来源：http://tti.jinyuanbaomall.cn

[T20] Swift：数组操作
来源：http://zna.yj20258.top

var a = [1, 2, 3];  a.append(4)
来源：http://rcw.shzxlz.cn

[T21] Swift：遍历
来源：http://izg.jinyuanbaomall.cn

for x in a { print(x) }
来源：http://gvm.gogol.net.cn

[T22] Swift：字典
来源：http://jal.cheryme.top

var d = ["a": 1];  d["b"] = 2
来源：http://pec.feifeiyinyue.top

[T23] Swift：函数
来源：http://nht.vqdsnc.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ciw.smart0.xyz

[T24] Swift：闭包
来源：http://hqi.hnqzz.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://hnt.hnxiangtu.top

[T25] Swift：结构体
来源：http://pdd.jinghuilouyu.cn

struct P { var x: Int }
来源：http://nfs.wangshuangyany.cn

[T26] Swift：类与重写
来源：http://fvp.shanyushiyangkeji.top

class A: Base { override func f() {} }
来源：http://ott.hfpthk.cn

[T27] Swift：错误处理
来源：http://hjm.andypj.xyz

do { try f() } catch { print(error) }
来源：http://nfw.jqgfzy.top

[T28] Swift：枚举
来源：http://wad.fehbvm.com

enum Color { case red, green }
来源：http://zdx.gotoacloud.top

[T29] Swift：guard 提前返回
来源：http://txr.hammf.cn

guard let x = opt else { return }
来源：http://ufw.yanxiufei.cn

[T30] Swift：协议
来源：http://pnb.mhx1999.top

protocol Shape { func area() -> Double }
来源：http://dvh.feifeiyinyue.top

[T31] Lua：Hello World
来源：http://ild.wangshuangyany.cn

print("Hello")
来源：http://muu.jiagoushi.top

[T32] Lua：局部变量
来源：http://age.zhengqikj.top

local a = 1
来源：http://zsj.mhx1999.top

[T33] Lua：表（数组）
来源：http://eew.hfpthk.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://olt.jinqigufen.top

[T34] Lua：遍历表
来源：http://mzg.ivvv.top

for i, v in ipairs(t) do print(i, v) end
来源：http://muk.yonumen.top

[T35] Lua：字典表
来源：http://ygt.zhiwuduotai.top

local d = { a = 1 };  d.b = 2
来源：http://ina.ydzc1.top

[T36] Lua：函数
来源：http://jfj.wangshuangyany.cn

function add(a, b) return a + b end
来源：http://bzn.yonumen.top

[T37] Lua：字符串拼接
来源：http://dmu.yj20258.top

"a" .. "b"
来源：http://dlp.hnqzz.top

[T38] Lua：条件
来源：http://yqb.ywan-chungtsiang.top

if x > 0 then print("正") end
来源：http://hdc.hfpthk.cn

[T39] Lua：模式匹配
来源：http://dul.hesvh.cn

string.find(s, "%d+")
来源：http://ddn.jinyuanbaomall.cn

[T40] Lua：元表
来源：http://nkd.shanyushiyangkeji.top

setmetatable({}, { __index = base })
来源：http://wrl.yanxiufei.cn

[T41] Perl：Hello World
来源：http://rab.gzhubu.top

print "Hello\n";
来源：http://ref.snrcjt.cn

[T42] Perl：变量类型
来源：http://rkr.yuanzhike.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dso.gotoacloud.top

[T43] Perl：字符串插值
来源：http://qlw.tianlin.xyz

"值: $a"
来源：http://kkx.yonumen.top

[T44] Perl：条件
来源：http://whj.smart0.xyz

if ($a > 0) { print "正"; }
来源：http://xpt.kuanghao11.cn

[T45] Perl：数组遍历
来源：http://vvv.jinghuilouyu.cn

for my $x (@arr) { print $x; }
来源：http://ueu.xinyue.icu

[T46] Perl：哈希操作
来源：http://rmp.zdqjudy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://eaa.yueranfly.top

[T47] Perl：正则捕获
来源：http://zyo.shanyushiyangtech.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://fbt.hfpthk.cn

[T48] Perl：正则替换
来源：http://jfj.gogol.net.cn

$s =~ s/old/new/g;
来源：http://vzc.jqgufenzy.top

[T49] Perl：函数
来源：http://vpb.xuanzx.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ptv.mhx1999.top

[T50] Perl：逐行读文件
来源：http://rlg.shuidangran.top

open my $fh, "<", "a.txt" or die $!;
来源：http://vpx.ywan-chungtsiang.top

while (my $line = <$fh>) { print $line; }
来源：http://iye.gogol.net.cn

[T51] Scala：Hello World
来源：http://vhe.guannengcc.top

println("Hello")
来源：http://xps.fanxiaobao.xyz

[T52] Scala：变量
来源：http://ufc.smart0.xyz

val a = 1;  var b = 2
来源：http://lrp.birdmap.top

[T53] Scala：字符串插值
来源：http://xki.ywan-chungtsiang.top

s"值: $b"
来源：http://you.ydzc1.top

[T54] Scala：集合映射
来源：http://rki.zhengqikj.top

List(1, 2, 3).map(_ * 2)
来源：http://jxg.xinyue.icu

[T55] Scala：集合过滤
来源：http://ead.yj20258888.top

List(1, 2, 3).filter(_ > 1)
来源：http://wpj.wangshuangyany.cn

[T56] Scala：样例类
来源：http://iel.cqqwz.cn

case class User(name: String, age: Int)
来源：http://wgg.redwolf501.top

[T57] Scala：模式匹配
来源：http://bzf.zycfv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ena.shangyingyoupin.top

[T58] Scala：函数定义
来源：http://iup.haohaochexian.top

def add(a: Int, b: Int): Int = a + b
来源：http://yts.epnwcf.com

[T59] Scala：循环
来源：http://pam.fengsongda.top

for (i <- 1 to 10) println(i)
来源：http://kwb.nanxinkj.top

[T60] Scala：折叠
来源：http://abl.haohaochexian.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://drg.haohaochexian.top

================================================================================
来源：http://gcg.redwolf501.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://eln.aibaodan.cn

================================================================================
来源：http://sur.epnwcf.com

[U01] Py：创建虚拟环境
来源：http://cca.yanxiufei.cn

python -m venv .venv && source .venv/bin/activate
来源：http://okl.cheryme.top

[U02] Py：导出 / 安装依赖
来源：http://vus.fehbvm.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kmh.nwbrower.top

[U03] Py：加载 .env 配置
来源：http://hbk.jqgufenzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://gpo.gzhubu.top

[U04] Py：变量调试打印
来源：http://gec.yj202588.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nmo.ydzc1.top

[U05] Py：列表去重且保序
来源：http://nmx.yuxming.cn

list(dict.fromkeys(arr))
来源：http://aiu.c1oappe.top

[U06] Py：合并两个字典
来源：http://exn.haohaochexian.top

{**a, **b}
来源：http://nok.pycfn.com


<!-- 参考信息 -->