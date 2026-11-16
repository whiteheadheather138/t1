代发 wailian999

free -h;  ps aux | grep nginx
来源：http://ioe.ydjk.org.cn

[R64] 结束进程
来源：http://bee.xuetiantiany.cn

kill -9 $(pgrep -f app.py)
来源：http://jke.yongpay.top

[R65] 查看端口占用
来源：http://nwi.jiagoushi.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dlp.vehdjk.com

[R66] 定时任务
来源：http://pim.sufxvd.cn

crontab -e;  crontab -l
来源：http://sea.yj20258888.top

[R67] 生成随机十六进制串
来源：http://zgt.svipenyu.cn

openssl rand -hex 16
来源：http://lcf.birdmap.top

[R68] 计算文件校验值
来源：http://ksy.bbcook.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lbt.hfpthk.cn

[R69] 生成随机密码
来源：http://uje.shanyushiyangtech.top

head -c 16 /dev/urandom | base64
来源：http://vcc.ybcxt.top

[R70] 时间戳与互转
来源：http://zsx.ehwqpu.com

date +%s;  date -d @1700000000
来源：http://sqj.yuanzhike.top

[R71] 日期格式化
来源：http://ucz.zhiwuduotai.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vvf.316326.xyz

[R72] 等待端口就绪
来源：http://kpn.hnxiangtu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://sht.xuanzx.com

[R73] 分割大日志
来源：http://mry.dashuyun.cn

split -l 1000 big.log part_
来源：http://kcy.yuxming.cn

[R74] 批量重命名
来源：http://ubv.shanyushiyangkeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xic.zhixingplan.top

[R75] 导出环境变量
来源：http://mhh.jqgfzy.top

export PATH="$HOME/bin:$PATH"
来源：http://ahe.vqdsnc.cn

[R76] 使用临时文件
来源：http://pvj.zdbjq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nij.quarkkingdee.top

[R77] 读取用户输入
来源：http://gdw.chenjidiqi.icu

read -rp "请输入: " ans
来源：http://rkb.smart0.xyz

[R78] 交互式菜单
来源：http://cea.zdqjudy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://wag.guowangkeji.top

[R79] 解析命令行选项
来源：http://iyw.vqdsnc.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://csr.xinyue.icu

[R80] 查看脚本执行耗时
来源：http://dxd.sxryk.cn

time ./run.sh
来源：http://uco.xuanzx.com

================================================================================
来源：http://dyg.shzxlz.cn

S. C / C++ 专题
来源：http://iid.chenlongwang.top

================================================================================
来源：http://aeo.hesvh.cn

[S01] C：Hello World
来源：http://dpv.cheryme.top

#include <stdio.h>
来源：http://vis.daria6918.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zvk.ppjwa.cn

[S02] C：变量与格式化输出
来源：http://xlv.shanyushiyangtech.top

int a = 10; printf("%d\n", a);
来源：http://qsb.c1oappe.top

[S03] C：读入整数
来源：http://uxu.ydzc1.top

int x; scanf("%d", &x);
来源：http://wia.tarul.cn

[S04] C：字符串复制
来源：http://jpy.hywenlv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nid.yj20258888.top

[S05] C：字符串长度
来源：http://bub.zhongyouzk.top

strlen(s)
来源：http://kyq.cucudq.cn

[S06] C：字符串比较
来源：http://lgk.wangdashe.top

strcmp(a, b) == 0
来源：http://ssk.zhoulong.xyz

[S07] C：数组遍历求和
来源：http://xio.yj20258.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nek.shuidangran.top

[S08] C：动态内存分配与释放
来源：http://xzj.snrcjt.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ybk.cqqwz.cn

[S09] C：结构体定义与初始化
来源：http://zgx.sweek.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://spi.fzhhl.top

[S10] C：指针与解引用
来源：http://eqy.tarul.cn

int *p = &a;  *p = 5;
来源：http://yyu.jiagoushi.top

[S11] C：逐行读文件
来源：http://eyv.52xcode.cn

FILE *f = fopen("a.txt", "r");
来源：http://nqt.jinqigufen.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://poa.daria6918.cn

fclose(f);
来源：http://tgx.jinqigufen.top

[S12] C：写文件
来源：http://hhd.ppjwa.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mze.jlsjyb.cn

[S13] C：宏定义
来源：http://nnp.gzhubu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dqb.yuanzhike.top

[S14] C：枚举
来源：http://hom.c1oappe.top

enum Color { RED, GREEN, BLUE };
来源：http://chi.xuetiantiany.cn

[S15] C：类型转换
来源：http://lnl.iojbl.cn

(double) a / b
来源：http://ujz.nanxinkj.top

[S16] C：位操作置位
来源：http://kxw.xuanzx.com

x |= (1 << 3);
来源：http://cdn.ybcxt.top

[S17] C：安全拼接字符串
来源：http://uep.mhx1999.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kbz.cqqwz.cn

[S18] C：命令行参数
来源：http://ofo.shanyushiyangtech.top

int main(int argc, char **argv)
来源：http://kpu.cashguo.top

[S19] C：快速排序
来源：http://ahz.dashuyun.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mbt.wangdashe.top

[S20] C：二分查找
来源：http://brj.yj20258.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xjx.gotoacloud.top

[S21] C：字符类别判断
来源：http://mfp.yj20258.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vpy.jianghu66.top

[S22] C：字符串转数字
来源：http://vah.jinghuilouyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wbm.guannengcc.top

[S23] C：随机数
来源：http://jdh.meibo888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://pkx.havefunace.top

[S24] C：获取本地时间
来源：http://olz.zhaomingkeji.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xov.gotoacloud.top

[S25] C：内存拷贝
来源：http://kaq.316326.xyz

memcpy(dst, src, n);
来源：http://vda.iojbl.cn

[S26] C：内存清零
来源：http://ewy.gogol.net.cn

memset(a, 0, sizeof a);
来源：http://cti.hesvh.cn

[S27] C：定义常量
来源：http://tmt.cashguo.top

const double PI = 3.14159;
来源：http://rux.yvedp.cn

[S28] C：静态变量
来源：http://urq.sjlbkw.cn

static int counter = 0;
来源：http://qcj.yuxming.cn

[S29] C：变参函数
来源：http://ubw.zhengqikj.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sel.mhx1999.top

[S30] C：头文件保护
来源：http://kon.tarul.cn

#ifndef X_H
来源：http://hdo.redwolf501.top

#define X_H
来源：http://kvr.zhoulong.xyz

#endif
来源：http://rjr.zhoulong.xyz

[S31] C++：Hello World
来源：http://drt.jianghu66.top

#include <iostream>
来源：http://ovk.fzhhl.top

int main() { std::cout << "Hello\n"; }
来源：http://piq.jyoumei.cn

[S32] C++：字符串
来源：http://dpb.svipenyu.cn

std::string s = "hi";  s += "!";
来源：http://ihs.ehwqpu.com

[S33] C++：vector 增删
来源：http://emp.chenjidiqi.icu

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://srs.wangdashe.top

[S34] C++：遍历 vector
来源：http://kcd.jyoumei.cn

for (auto &x : v) { std::cout << x; }
来源：http://pet.pengpengdd.cyou

[S35] C++：map
来源：http://yha.wangdashe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dki.daria6918.cn

[S36] C++：unordered_map
来源：http://gfi.yanxiufei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zbd.jinghuilouyu.cn

[S37] C++：set
来源：http://fxb.havefunace.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yjj.aizwys.cn

[S38] C++：排序
来源：http://dqz.guowangkeji.top

std::sort(v.begin(), v.end());
来源：http://kok.fktsv.cn

[S39] C++：自定义比较器排序
来源：http://xyh.havefunace.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hmi.tian-w.cn

[S40] C++：查找元素
来源：http://wvz.cashguo.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jdf.redwolf501.top

[S41] C++：类与构造函数
来源：http://xae.zhaomingkeji.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zui.gotoacloud.top

[S42] C++：继承与虚函数
来源：http://obc.shuidangran.top

class B : public Base { public: void f() override {} };
来源：http://ejt.cucudq.cn

[S43] C++：智能指针
来源：http://nnj.zdbjq.cn

auto p = std::make_unique<int>(5);
来源：http://icp.jqgfzy.top

[S44] C++：引用传参
来源：http://cbw.epnwcf.com

void inc(int &x) { ++x; }
来源：http://ifs.cheryme.top

[S45] C++：lambda
来源：http://hkz.yuanzhike.top

auto add = [](int a, int b) { return a + b; };
来源：http://jfs.cashguo.top

[S46] C++：函数模板
来源：http://fzh.ydjk.org.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lvx.quarkkingdee.top

[S47] C++：结构化绑定遍历
来源：http://nno.nanxinkj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nru.yangfankeji.com

[S48] C++：逐行读文件
来源：http://njz.xingfuxueyuan.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://aco.bbcook.cn

while (std::getline(in, line)) { }
来源：http://iob.fanxiaobao.xyz

[S49] C++：写文件
来源：http://tic.zhiwuduotai.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://whd.xziqi.cn

[S50] C++：格式化数字
来源：http://chj.guannengcc.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jvy.chenzaomai.com

[S51] C++：显式类型转换
来源：http://smc.bjfxy.top

static_cast<double>(a) / b
来源：http://rrx.hongshengwenyu.top

[S52] C++：const 与 noexcept
来源：http://ggk.zhijiandao.cn

int size() const noexcept { return n_; }
来源：http://lyt.sufxvd.cn

[S53] C++：移动语义
来源：http://dgx.hnqzz.top

std::vector<int> w = std::move(v);
来源：http://wdg.sxryk.cn

[S54] C++：异常处理
来源：http://yai.quarkkingdee.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fjh.zhaomingkeji.xyz

[S55] C++：结构化绑定
来源：http://ure.yangfankeji.com

auto [a, b] = std::make_pair(1, 2);
来源：http://bfb.yj20258888.top

[S56] C++：optional
来源：http://fxw.sufxvd.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ttw.jqgufenzy.top

[S57] C++：编译期常量
来源：http://gtu.wangdashe.top

constexpr int N = 10;
来源：http://tzn.yonumen.top

[S58] C++：命名空间
来源：http://bnm.jlsjyb.cn

namespace ns { int f() { return 1; } }
来源：http://edn.smart0.xyz

[S59] C++：静态断言
来源：http://fvs.jlsjyb.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wuo.xuanzx.com

[S60] C++：遍历并删除元素
来源：http://otf.zycfv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mas.xziqi.cn

================================================================================
来源：http://kgb.quarkkingdee.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eof.xziqi.cn

================================================================================
来源：http://wcp.316326.xyz

[T01] Kotlin：Hello World
来源：http://rps.jinghuilouyu.cn

println("Hello")
来源：http://ezj.zdbjq.cn

[T02] Kotlin：变量
来源：http://ukd.yj20258.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rhq.52xcode.cn

[T03] Kotlin：字符串模板
来源：http://ref.fengsongda.top

"值: $b"
来源：http://vuq.sufxvd.cn

[T04] Kotlin：空安全
来源：http://hck.gotoacloud.top

val n: String? = null;  n?.length
来源：http://jji.feifeiyinyue.top

[T05] Kotlin：when 表达式
来源：http://uum.gzhubu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fgw.yfazqb.com

[T06] Kotlin：集合映射
来源：http://tpl.aizwys.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://din.zdbjq.cn

[T07] Kotlin：集合过滤
来源：http://iek.yuxming.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mvl.feifeiyinyue.top

[T08] Kotlin：数据类
来源：http://edt.yuxming.cn

data class User(val name: String, val age: Int)
来源：http://agu.yonumen.top

[T09] Kotlin：扩展函数
来源：http://gmt.hnqzz.top

fun String.exclaim() = this + "!"
来源：http://hrz.ivvv.top

[T10] Kotlin：默认参数
来源：http://zvg.sufxvd.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ifz.wangshuangyany.cn

[T11] Kotlin：协程
来源：http://alt.zhixingplan.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://qpo.pengpengdd.cyou

[T12] Kotlin：解构声明
来源：http://oqt.daxiang520.top

val (a, b) = Pair(1, 2)
来源：http://dwd.daria6918.cn

[T13] Kotlin：只读 Map
来源：http://gar.xinyue.icu

val m = mapOf("a" to 1)
来源：http://jhz.zhiwuduotai.top

[T14] Kotlin：循环
来源：http://uyt.tanke756.top

for (i in 1..10) println(i)
来源：http://zzc.guowangkeji.top

[T15] Kotlin：接口
来源：http://hhf.hywenlv.cn

interface Shape { fun area(): Double }
来源：http://bhx.vqdsnc.cn

[T16] Swift：Hello World
来源：http://igl.mhx1999.top

print("Hello")
来源：http://ejh.vehdjk.com

[T17] Swift：变量与常量
来源：http://frh.cucudq.cn

var a = 1;  let b = 2
来源：http://cpj.hnxiangtu.top

[T18] Swift：字符串插值
来源：http://fxd.yj20258.top

"值: \(b)"
来源：http://buo.zdqjudy.top

[T19] Swift：可选绑定
来源：http://bpx.xuetiantiany.cn

if let n = opt { print(n) }
来源：http://rek.meibo888.top

[T20] Swift：数组操作
来源：http://dnh.haohaochexian.top

var a = [1, 2, 3];  a.append(4)
来源：http://scl.zhoulong.xyz

[T21] Swift：遍历
来源：http://vgp.xuanzx.com

for x in a { print(x) }
来源：http://rza.yj20258.top

[T22] Swift：字典
来源：http://tff.yj202588.top

var d = ["a": 1];  d["b"] = 2
来源：http://txl.pycfn.com

[T23] Swift：函数
来源：http://ypc.hongshengwenyu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gjd.fanxiaobao.xyz

[T24] Swift：闭包
来源：http://oqk.ydjk.org.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rzt.jinqigfzy.top

[T25] Swift：结构体
来源：http://fgs.zdbjq.cn

struct P { var x: Int }
来源：http://gow.quarkkingdee.top

[T26] Swift：类与重写
来源：http://sng.epnwcf.com

class A: Base { override func f() {} }
来源：http://lgi.zhengqikj.top

[T27] Swift：错误处理
来源：http://rwr.cheryme.top

do { try f() } catch { print(error) }
来源：http://fgy.wangdashe.top

[T28] Swift：枚举
来源：http://gvx.guannengcc.top

enum Color { case red, green }
来源：http://ppa.sufxvd.cn

[T29] Swift：guard 提前返回
来源：http://ykg.shzxlz.cn

guard let x = opt else { return }
来源：http://bcl.jianghu66.top

[T30] Swift：协议
来源：http://rzq.smart0.xyz

protocol Shape { func area() -> Double }
来源：http://nio.fanxiaobao.xyz

[T31] Lua：Hello World
来源：http://rbh.xuanzx.com

print("Hello")
来源：http://tmv.tanke756.top

[T32] Lua：局部变量
来源：http://wze.dashuyun.cn

local a = 1
来源：http://wse.zhijiandao.cn

[T33] Lua：表（数组）
来源：http://sew.jyoumei.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bpv.pengpengdd.cyou

[T34] Lua：遍历表
来源：http://hoz.snrcjt.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://con.daxiang520.top

[T35] Lua：字典表
来源：http://fzg.gaohongyu789.top

local d = { a = 1 };  d.b = 2
来源：http://fko.ivvv.top

[T36] Lua：函数
来源：http://phf.xylfe.cn

function add(a, b) return a + b end
来源：http://ftf.jqgufenzy.top

[T37] Lua：字符串拼接
来源：http://aun.dianchejie.cn

"a" .. "b"
来源：http://jck.cashguo.top

[T38] Lua：条件
来源：http://krr.jlsjyb.cn

if x > 0 then print("正") end
来源：http://bef.dashuyun.cn

[T39] Lua：模式匹配
来源：http://rlk.hcnkem.com

string.find(s, "%d+")
来源：http://crh.jqgfzy.top

[T40] Lua：元表
来源：http://ide.tian-w.cn

setmetatable({}, { __index = base })
来源：http://pel.zhongyouzk.top

[T41] Perl：Hello World
来源：http://cil.nanxinkj.top

print "Hello\n";
来源：http://zdz.daxiang520.top

[T42] Perl：变量类型
来源：http://oxz.tarul.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://koi.feifeiyinyue.top

[T43] Perl：字符串插值
来源：http://jas.yuanzhike.top

"值: $a"
来源：http://qap.birdmap.top

[T44] Perl：条件
来源：http://huj.xingfuxueyuan.xyz

if ($a > 0) { print "正"; }
来源：http://rnl.52xcode.cn

[T45] Perl：数组遍历
来源：http://wmx.ydjk.org.cn

for my $x (@arr) { print $x; }
来源：http://uit.epnwcf.com

[T46] Perl：哈希操作
来源：http://uob.yj202588.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jit.nwbrower.top

[T47] Perl：正则捕获
来源：http://ckr.yangfankeji.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://zbv.wangdashe.top

[T48] Perl：正则替换
来源：http://jup.bbcook.cn

$s =~ s/old/new/g;
来源：http://vnq.cheryme.top

[T49] Perl：函数
来源：http://nso.fktsv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bzy.pycfn.com

[T50] Perl：逐行读文件
来源：http://stc.yuanzhike.top

open my $fh, "<", "a.txt" or die $!;
来源：http://utk.xuanzx.com

while (my $line = <$fh>) { print $line; }
来源：http://cul.guannengcc.top

[T51] Scala：Hello World
来源：http://eyx.zdbjq.cn

println("Hello")
来源：http://xzh.epnwcf.com

[T52] Scala：变量
来源：http://kdt.xinyue.icu

val a = 1;  var b = 2
来源：http://got.smart0.xyz

[T53] Scala：字符串插值
来源：http://sdt.quarkkingdee.top

s"值: $b"
来源：http://tvq.hfpthk.cn

[T54] Scala：集合映射
来源：http://bwq.meibo888.top

List(1, 2, 3).map(_ * 2)
来源：http://yxp.jianghu66.top

[T55] Scala：集合过滤
来源：http://nmr.jianghu66.top

List(1, 2, 3).filter(_ > 1)
来源：http://jec.vehdjk.com

[T56] Scala：样例类
来源：http://mhp.tianlin.xyz

case class User(name: String, age: Int)
来源：http://cnu.fanxiaobao.xyz

[T57] Scala：模式匹配
来源：http://fgj.9152youxi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mht.gogol.net.cn

[T58] Scala：函数定义
来源：http://nis.aibaodan.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kwm.feifeiyinyue.top

[T59] Scala：循环
来源：http://qfe.jinyuanbaomall.cn

for (i <- 1 to 10) println(i)
来源：http://xhw.aizwys.cn

[T60] Scala：折叠
来源：http://aso.tian-w.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://crv.0kj1m.cn

================================================================================
来源：http://zhw.jinghuilouyu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bra.hcnkem.com

================================================================================
来源：http://gel.ehwqpu.com

[U01] Py：创建虚拟环境
来源：http://rax.chenjidiqi.icu

python -m venv .venv && source .venv/bin/activate
来源：http://gus.hcnkem.com

[U02] Py：导出 / 安装依赖
来源：http://xlo.cheryme.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uha.mhx1999.top

[U03] Py：加载 .env 配置
来源：http://lac.gogol.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bds.0kj1m.cn

[U04] Py：变量调试打印
来源：http://gsn.shanyushiyangkeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://shu.cdnleiting.top


<!-- 参考信息 -->