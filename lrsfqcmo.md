代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kbt.zdbjq.cn

[R60] 只看 HTTP 状态码
来源：http://olq.shuidangran.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fpf.gzhubu.top

[R61] 磁盘占用
来源：http://nbo.tian-w.cn

df -h;  du -sh *
来源：http://xdo.xingfuxueyuan.xyz

[R62] 找最占空间的文件
来源：http://xlj.zhaomingkeji.xyz

du -ah . | sort -rh | head -10
来源：http://hbf.yangfankeji.com

[R63] 内存与进程
来源：http://lhw.sjlbkw.cn

free -h;  ps aux | grep nginx
来源：http://evm.9152youxi.cn

[R64] 结束进程
来源：http://fdr.hcnkem.com

kill -9 $(pgrep -f app.py)
来源：http://cvp.uphjek.com

[R65] 查看端口占用
来源：http://mnf.xuetiantiany.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pxo.hesvh.cn

[R66] 定时任务
来源：http://sxn.hysaishi.cn

crontab -e;  crontab -l
来源：http://iik.yj202588.top

[R67] 生成随机十六进制串
来源：http://fij.hnxiangtu.top

openssl rand -hex 16
来源：http://ncx.jinyuanbaomall.cn

[R68] 计算文件校验值
来源：http://djt.ehwqpu.com

sha256sum a.txt;  md5sum a.txt
来源：http://jap.shanyushiyangtech.top

[R69] 生成随机密码
来源：http://sig.kuanghao11.cn

head -c 16 /dev/urandom | base64
来源：http://lab.sysykeji.top

[R70] 时间戳与互转
来源：http://gxh.xuanzx.com

date +%s;  date -d @1700000000
来源：http://ini.xuanzx.com

[R71] 日期格式化
来源：http://bxo.shuidangran.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://awj.aizwys.cn

[R72] 等待端口就绪
来源：http://lhs.yongpay.top

until nc -z localhost 3306; do sleep 1; done
来源：http://raw.zdqjudy.top

[R73] 分割大日志
来源：http://ukv.nanxuanxn.top

split -l 1000 big.log part_
来源：http://bej.bbcook.cn

[R74] 批量重命名
来源：http://fgb.jlsjyb.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qfp.zhongyouzk.top

[R75] 导出环境变量
来源：http://fwq.tian-w.cn

export PATH="$HOME/bin:$PATH"
来源：http://usr.zhongyouzk.top

[R76] 使用临时文件
来源：http://bdr.meibo888.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lqz.redwolf501.top

[R77] 读取用户输入
来源：http://tgn.ybcxt.top

read -rp "请输入: " ans
来源：http://jul.hongshengwenyu.top

[R78] 交互式菜单
来源：http://sco.yuanzhike.top

select opt in a b c; do echo "$opt"; break; done
来源：http://fxk.hongshengwenyu.top

[R79] 解析命令行选项
来源：http://ofl.daxiang520.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xdy.pycfn.com

[R80] 查看脚本执行耗时
来源：http://als.chenzaomai.com

time ./run.sh
来源：http://tjk.zhoulong.xyz

================================================================================
来源：http://vzq.yuxming.cn

S. C / C++ 专题
来源：http://hkx.sweek.top

================================================================================
来源：http://pdh.epnwcf.com

[S01] C：Hello World
来源：http://mrj.uphjek.com

#include <stdio.h>
来源：http://hmm.zhengqikj.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gox.fktsv.cn

[S02] C：变量与格式化输出
来源：http://rsn.fanxiaobao.xyz

int a = 10; printf("%d\n", a);
来源：http://yeh.ppjwa.cn

[S03] C：读入整数
来源：http://uwu.jqgufenzy.top

int x; scanf("%d", &x);
来源：http://wzh.yanxiufei.cn

[S04] C：字符串复制
来源：http://qsp.gotoacloud.top

char dst[32]; strcpy(dst, "hi");
来源：http://hmo.havefunace.top

[S05] C：字符串长度
来源：http://zhx.ppjwa.cn

strlen(s)
来源：http://cqk.haohaochexian.top

[S06] C：字符串比较
来源：http://svz.svipenyu.cn

strcmp(a, b) == 0
来源：http://zjq.fanxiaobao.xyz

[S07] C：数组遍历求和
来源：http://dii.hnqzz.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yam.cqqwz.cn

[S08] C：动态内存分配与释放
来源：http://pai.vqdsnc.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nlh.shanyushiyangtech.top

[S09] C：结构体定义与初始化
来源：http://nva.ppjwa.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pii.aizwys.cn

[S10] C：指针与解引用
来源：http://ffx.wangshuangyany.cn

int *p = &a;  *p = 5;
来源：http://foi.quarkkingdee.top

[S11] C：逐行读文件
来源：http://ltm.zhijiandao.cn

FILE *f = fopen("a.txt", "r");
来源：http://zwb.cucudq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jmf.yfazqb.com

fclose(f);
来源：http://mwh.tarul.cn

[S12] C：写文件
来源：http://sck.daria6918.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qto.ctjpmb.com

[S13] C：宏定义
来源：http://xqp.shanyushiyangtech.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vor.smart0.xyz

[S14] C：枚举
来源：http://nuc.zhaomingkeji.xyz

enum Color { RED, GREEN, BLUE };
来源：http://hzj.epnwcf.com

[S15] C：类型转换
来源：http://igl.ywan-chungtsiang.top

(double) a / b
来源：http://hry.daxiang520.top

[S16] C：位操作置位
来源：http://zvp.zhongyouzk.top

x |= (1 << 3);
来源：http://cvt.zhiwuduotai.top

[S17] C：安全拼接字符串
来源：http://zzz.dianchejie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pma.smart0.xyz

[S18] C：命令行参数
来源：http://wep.hnxiangtu.top

int main(int argc, char **argv)
来源：http://nfw.sweek.top

[S19] C：快速排序
来源：http://wlo.kuanghao11.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jti.iojbl.cn

[S20] C：二分查找
来源：http://dhm.jqgfzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hmc.bjfxy.top

[S21] C：字符类别判断
来源：http://ize.nanxinkj.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gxg.hywenlv.cn

[S22] C：字符串转数字
来源：http://vem.andypj.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://fgq.zhaomingkeji.xyz

[S23] C：随机数
来源：http://cgj.bjfxy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://rla.hnxiangtu.top

[S24] C：获取本地时间
来源：http://tav.epnwcf.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nqj.redwolf501.top

[S25] C：内存拷贝
来源：http://otm.xingfuxueyuan.xyz

memcpy(dst, src, n);
来源：http://lye.ctjpmb.com

[S26] C：内存清零
来源：http://dqn.tarul.cn

memset(a, 0, sizeof a);
来源：http://uej.yj202588.top

[S27] C：定义常量
来源：http://cqs.havefunace.top

const double PI = 3.14159;
来源：http://yzq.zhengqikj.top

[S28] C：静态变量
来源：http://lza.hysaishi.cn

static int counter = 0;
来源：http://who.mhx1999.top

[S29] C：变参函数
来源：http://nsj.9152youxi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ckm.52xcode.cn

[S30] C：头文件保护
来源：http://ain.yongpay.top

#ifndef X_H
来源：http://lpa.ydzc1.top

#define X_H
来源：http://nzi.zdbjq.cn

#endif
来源：http://geu.aizwys.cn

[S31] C++：Hello World
来源：http://pcr.yj202588.top

#include <iostream>
来源：http://gwl.xinyue.icu

int main() { std::cout << "Hello\n"; }
来源：http://emn.sjlbkw.cn

[S32] C++：字符串
来源：http://dui.ivvv.top

std::string s = "hi";  s += "!";
来源：http://cvs.shangyingyoupin.top

[S33] C++：vector 增删
来源：http://wue.jinyuanbaomall.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rcj.guowangkeji.top

[S34] C++：遍历 vector
来源：http://omg.epnwcf.com

for (auto &x : v) { std::cout << x; }
来源：http://bgb.jqgufenzy.top

[S35] C++：map
来源：http://msl.0kj1m.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nuy.gogol.net.cn

[S36] C++：unordered_map
来源：http://yfm.yanxiufei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fbu.hammf.cn

[S37] C++：set
来源：http://xlg.andypj.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yld.hongshengwenyu.top

[S38] C++：排序
来源：http://gke.nwbrower.top

std::sort(v.begin(), v.end());
来源：http://hui.ivvv.top

[S39] C++：自定义比较器排序
来源：http://hww.birdmap.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xzn.cqqwz.cn

[S40] C++：查找元素
来源：http://cqy.nwbrower.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rip.zhaomingkeji.xyz

[S41] C++：类与构造函数
来源：http://sgm.hammf.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mmv.shanyushiyangtech.top

[S42] C++：继承与虚函数
来源：http://brj.ehwqpu.com

class B : public Base { public: void f() override {} };
来源：http://vhv.shuidangran.top

[S43] C++：智能指针
来源：http://jhx.xziqi.cn

auto p = std::make_unique<int>(5);
来源：http://wyv.sweek.top

[S44] C++：引用传参
来源：http://uox.quarkkingdee.top

void inc(int &x) { ++x; }
来源：http://ile.guannengcc.top

[S45] C++：lambda
来源：http://ejb.vehdjk.com

auto add = [](int a, int b) { return a + b; };
来源：http://vvy.jinqigufen.top

[S46] C++：函数模板
来源：http://ybs.ctjpmb.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mmn.jqgfzy.top

[S47] C++：结构化绑定遍历
来源：http://qmo.zycfv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hlw.xuetiantiany.cn

[S48] C++：逐行读文件
来源：http://efj.gaohongyu789.top

std::ifstream in("a.txt");  std::string line;
来源：http://mcf.ybcxt.top

while (std::getline(in, line)) { }
来源：http://pwf.zdbjq.cn

[S49] C++：写文件
来源：http://tnn.hywenlv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cjw.andypj.xyz

[S50] C++：格式化数字
来源：http://gyt.pengpengdd.cyou

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zob.xinyue.icu

[S51] C++：显式类型转换
来源：http://bbg.xingfuxueyuan.xyz

static_cast<double>(a) / b
来源：http://tks.ywan-chungtsiang.top

[S52] C++：const 与 noexcept
来源：http://hfu.sjlbkw.cn

int size() const noexcept { return n_; }
来源：http://xht.nwbrower.top

[S53] C++：移动语义
来源：http://tfl.shuidangran.top

std::vector<int> w = std::move(v);
来源：http://uzf.yuanzhike.top

[S54] C++：异常处理
来源：http://dyv.hfpthk.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ycp.xuanzx.com

[S55] C++：结构化绑定
来源：http://wog.jqgufenzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://sfp.9152youxi.cn

[S56] C++：optional
来源：http://kze.aizwys.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://shz.pengpengdd.cyou

[S57] C++：编译期常量
来源：http://jxa.chenlongwang.top

constexpr int N = 10;
来源：http://vmt.cqqwz.cn

[S58] C++：命名空间
来源：http://ene.0kj1m.cn

namespace ns { int f() { return 1; } }
来源：http://zri.ydjk.org.cn

[S59] C++：静态断言
来源：http://bwa.uphjek.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ygr.shangyingyoupin.top

[S60] C++：遍历并删除元素
来源：http://qeu.sufxvd.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tgw.zhixingplan.top

================================================================================
来源：http://wpo.52xcode.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fok.quarkkingdee.top

================================================================================
来源：http://dst.jinqigufen.top

[T01] Kotlin：Hello World
来源：http://yac.birdmap.top

println("Hello")
来源：http://jxn.cashguo.top

[T02] Kotlin：变量
来源：http://nwm.nanxinkj.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fyh.haohaochexian.top

[T03] Kotlin：字符串模板
来源：http://wxd.yvedp.cn

"值: $b"
来源：http://mgo.zhengqikj.top

[T04] Kotlin：空安全
来源：http://vos.kuanghao11.cn

val n: String? = null;  n?.length
来源：http://xwr.cashguo.top

[T05] Kotlin：when 表达式
来源：http://ict.aibaodan.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dgl.cheryme.top

[T06] Kotlin：集合映射
来源：http://uub.zhoulong.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://vop.tianlin.xyz

[T07] Kotlin：集合过滤
来源：http://qfh.jinyuanbaomall.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bbr.jinyuanbaomall.cn

[T08] Kotlin：数据类
来源：http://byc.uphjek.com

data class User(val name: String, val age: Int)
来源：http://mlu.hcnkem.com

[T09] Kotlin：扩展函数
来源：http://gsl.pycfn.com

fun String.exclaim() = this + "!"
来源：http://ncm.yuanzhike.top

[T10] Kotlin：默认参数
来源：http://pdk.hnxiangtu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://blt.jinghuilouyu.cn

[T11] Kotlin：协程
来源：http://avq.yuxming.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kly.tian-w.cn

[T12] Kotlin：解构声明
来源：http://xgz.zhoulong.xyz

val (a, b) = Pair(1, 2)
来源：http://mns.dianchejie.cn

[T13] Kotlin：只读 Map
来源：http://yyc.xylfe.cn

val m = mapOf("a" to 1)
来源：http://upc.wangshuangyany.cn

[T14] Kotlin：循环
来源：http://kol.52xcode.cn

for (i in 1..10) println(i)
来源：http://oaa.vehdjk.com

[T15] Kotlin：接口
来源：http://zvd.dashuyun.cn

interface Shape { fun area(): Double }
来源：http://bru.aizwys.cn

[T16] Swift：Hello World
来源：http://ffj.ydjk.org.cn

print("Hello")
来源：http://ixq.smart0.xyz

[T17] Swift：变量与常量
来源：http://zdh.havefunace.top

var a = 1;  let b = 2
来源：http://fma.nwbrower.top

[T18] Swift：字符串插值
来源：http://jfd.sufxvd.cn

"值: \(b)"
来源：http://iex.sysykeji.top

[T19] Swift：可选绑定
来源：http://ogw.hnqzz.top

if let n = opt { print(n) }
来源：http://eyy.cucudq.cn

[T20] Swift：数组操作
来源：http://mbq.cheryme.top

var a = [1, 2, 3];  a.append(4)
来源：http://wno.haohaochexian.top

[T21] Swift：遍历
来源：http://mxu.cucudq.cn

for x in a { print(x) }
来源：http://vzr.havefunace.top

[T22] Swift：字典
来源：http://axe.shanyushiyangtech.top

var d = ["a": 1];  d["b"] = 2
来源：http://xcd.pengpengdd.cyou

[T23] Swift：函数
来源：http://hqh.c1oappe.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gut.hywenlv.cn

[T24] Swift：闭包
来源：http://fyi.yuxming.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://klg.9152youxi.cn

[T25] Swift：结构体
来源：http://xxs.sjlbkw.cn

struct P { var x: Int }
来源：http://kxe.yuanzhike.top

[T26] Swift：类与重写
来源：http://jyq.ppjwa.cn

class A: Base { override func f() {} }
来源：http://dep.sufxvd.cn

[T27] Swift：错误处理
来源：http://nao.bbcook.cn

do { try f() } catch { print(error) }
来源：http://rql.ydzc1.top

[T28] Swift：枚举
来源：http://pwf.xuanzx.com

enum Color { case red, green }
来源：http://hpc.jinqigufen.top

[T29] Swift：guard 提前返回
来源：http://pvn.yangfankeji.com

guard let x = opt else { return }
来源：http://vgk.zhaomingkeji.xyz

[T30] Swift：协议
来源：http://sqj.zhiwuduotai.top

protocol Shape { func area() -> Double }
来源：http://lno.bjfxy.top

[T31] Lua：Hello World
来源：http://nus.hcnkem.com

print("Hello")
来源：http://fca.jinqigfzy.top

[T32] Lua：局部变量
来源：http://izn.jinghuilouyu.cn

local a = 1
来源：http://kmt.pycfn.com

[T33] Lua：表（数组）
来源：http://jvy.tianlin.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://ral.xuetiantiany.cn

[T34] Lua：遍历表
来源：http://xjl.jyoumei.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kid.nanxinkj.top

[T35] Lua：字典表
来源：http://wui.mhx1999.top

local d = { a = 1 };  d.b = 2
来源：http://ncp.guannengcc.top

[T36] Lua：函数
来源：http://wtg.316326.xyz

function add(a, b) return a + b end
来源：http://xuc.zhoulong.xyz

[T37] Lua：字符串拼接
来源：http://nkp.jiagoushi.top

"a" .. "b"
来源：http://chu.xziqi.cn

[T38] Lua：条件
来源：http://cir.zdqjudy.top

if x > 0 then print("正") end
来源：http://cxl.daxiang520.top

[T39] Lua：模式匹配
来源：http://ili.vehdjk.com

string.find(s, "%d+")
来源：http://zdg.shangyingyoupin.top

[T40] Lua：元表
来源：http://xbb.tanke756.top

setmetatable({}, { __index = base })
来源：http://ukm.cdnleiting.top

[T41] Perl：Hello World
来源：http://imc.vehdjk.com

print "Hello\n";
来源：http://qmj.pycfn.com

[T42] Perl：变量类型
来源：http://apa.xuetiantiany.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bel.tian-w.cn

[T43] Perl：字符串插值
来源：http://odt.zdbjq.cn

"值: $a"
来源：http://yef.pycfn.com

[T44] Perl：条件
来源：http://hnw.nanxinkj.top

if ($a > 0) { print "正"; }
来源：http://mpv.hongshengwenyu.top

[T45] Perl：数组遍历
来源：http://hre.cucudq.cn

for my $x (@arr) { print $x; }
来源：http://tkj.shuidangran.top

[T46] Perl：哈希操作
来源：http://xrd.dashuyun.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kpj.gaohongyu789.top

[T47] Perl：正则捕获
来源：http://nvl.yongpay.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://not.jinqigufen.top

[T48] Perl：正则替换
来源：http://ipz.sxryk.cn

$s =~ s/old/new/g;
来源：http://hmt.cqqwz.cn

[T49] Perl：函数
来源：http://kpc.smart0.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://knl.yangfankeji.com

[T50] Perl：逐行读文件
来源：http://ccl.havefunace.top

open my $fh, "<", "a.txt" or die $!;
来源：http://kdl.epnwcf.com

while (my $line = <$fh>) { print $line; }
来源：http://tcj.cqqwz.cn

[T51] Scala：Hello World
来源：http://jet.chenjidiqi.icu

println("Hello")
来源：http://zhl.zhiwuduotai.top

[T52] Scala：变量
来源：http://huk.316326.xyz

val a = 1;  var b = 2
来源：http://qng.xuetiantiany.cn

[T53] Scala：字符串插值
来源：http://bab.smart0.xyz

s"值: $b"
来源：http://jop.fengsongda.top

[T54] Scala：集合映射
来源：http://krh.yj20258.top

List(1, 2, 3).map(_ * 2)
来源：http://sfe.hcnkem.com

[T55] Scala：集合过滤
来源：http://hdv.hesvh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lhx.shanyushiyangkeji.top

[T56] Scala：样例类
来源：http://shi.fzhhl.top

case class User(name: String, age: Int)
来源：http://pfg.iojbl.cn

[T57] Scala：模式匹配
来源：http://umq.jyoumei.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yjn.jlsjyb.cn

[T58] Scala：函数定义
来源：http://rts.meibo888.top

def add(a: Int, b: Int): Int = a + b
来源：http://ktq.kuanghao11.cn

[T59] Scala：循环
来源：http://dbd.nwbrower.top

for (i <- 1 to 10) println(i)
来源：http://ksq.epnwcf.com

[T60] Scala：折叠
来源：http://cgj.mhx1999.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bso.hcnkem.com

================================================================================
来源：http://xou.yj202588.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fhy.zhiwuduotai.top

================================================================================
来源：http://dft.hfpthk.cn


<!-- 参考信息 -->