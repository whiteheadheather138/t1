代发 wailian999

free -h;  ps aux | grep nginx
来源：http://atn.zdqjudy.top

[R64] 结束进程
来源：http://wke.xziqi.cn

kill -9 $(pgrep -f app.py)
来源：http://ihr.ivvv.top

[R65] 查看端口占用
来源：http://sal.sweek.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qjn.zycfv.cn

[R66] 定时任务
来源：http://ogr.bbcook.cn

crontab -e;  crontab -l
来源：http://poe.iojbl.cn

[R67] 生成随机十六进制串
来源：http://yzq.meibo888.top

openssl rand -hex 16
来源：http://xam.sjlbkw.cn

[R68] 计算文件校验值
来源：http://jwg.gaohongyu789.top

sha256sum a.txt;  md5sum a.txt
来源：http://sxl.andypj.xyz

[R69] 生成随机密码
来源：http://jbo.zycfv.cn

head -c 16 /dev/urandom | base64
来源：http://yfx.ehwqpu.com

[R70] 时间戳与互转
来源：http://mtm.wangshuangyany.cn

date +%s;  date -d @1700000000
来源：http://yve.hnxiangtu.top

[R71] 日期格式化
来源：http://yhm.c1oappe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vae.jianghu66.top

[R72] 等待端口就绪
来源：http://kce.yj202588.top

until nc -z localhost 3306; do sleep 1; done
来源：http://brg.cheryme.top

[R73] 分割大日志
来源：http://nix.jinqigufen.top

split -l 1000 big.log part_
来源：http://wqk.yangfankeji.com

[R74] 批量重命名
来源：http://xpi.zhoulong.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pqx.tian-w.cn

[R75] 导出环境变量
来源：http://hxz.chenjidiqi.icu

export PATH="$HOME/bin:$PATH"
来源：http://zmu.nanxinkj.top

[R76] 使用临时文件
来源：http://onw.chenlongwang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uit.dashuyun.cn

[R77] 读取用户输入
来源：http://xox.daxiang520.top

read -rp "请输入: " ans
来源：http://yqd.hnxiangtu.top

[R78] 交互式菜单
来源：http://btg.aizwys.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yyz.hysaishi.cn

[R79] 解析命令行选项
来源：http://pnj.chenlongwang.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xqr.aibaodan.cn

[R80] 查看脚本执行耗时
来源：http://khg.52xcode.cn

time ./run.sh
来源：http://slc.ydzc1.top

================================================================================
来源：http://clj.jinqigufen.top

S. C / C++ 专题
来源：http://wax.cheryme.top

================================================================================
来源：http://hcr.mhx1999.top

[S01] C：Hello World
来源：http://exs.uphjek.com

#include <stdio.h>
来源：http://lux.wangshuangyany.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ehe.ydjk.org.cn

[S02] C：变量与格式化输出
来源：http://xsi.tian-w.cn

int a = 10; printf("%d\n", a);
来源：http://meo.fzhhl.top

[S03] C：读入整数
来源：http://owz.jqgufenzy.top

int x; scanf("%d", &x);
来源：http://chq.chenjidiqi.icu

[S04] C：字符串复制
来源：http://qpt.9152youxi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qwl.pengpengdd.cyou

[S05] C：字符串长度
来源：http://htn.jyoumei.cn

strlen(s)
来源：http://ycj.jyoumei.cn

[S06] C：字符串比较
来源：http://qgq.snrcjt.cn

strcmp(a, b) == 0
来源：http://qag.jinqigufen.top

[S07] C：数组遍历求和
来源：http://xqe.jiagoushi.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kem.redwolf501.top

[S08] C：动态内存分配与释放
来源：http://fnn.zhiwuduotai.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nwb.vqdsnc.cn

[S09] C：结构体定义与初始化
来源：http://ckq.xinyue.icu

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zlf.tianlin.xyz

[S10] C：指针与解引用
来源：http://tpi.c1oappe.top

int *p = &a;  *p = 5;
来源：http://alz.9152youxi.cn

[S11] C：逐行读文件
来源：http://ifw.xingfuxueyuan.xyz

FILE *f = fopen("a.txt", "r");
来源：http://fpw.yvedp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jbq.fanxiaobao.xyz

fclose(f);
来源：http://lhm.jlsjyb.cn

[S12] C：写文件
来源：http://xjm.yvedp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nbx.yonumen.top

[S13] C：宏定义
来源：http://rlk.zdqjudy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mqf.svipenyu.cn

[S14] C：枚举
来源：http://fli.zycfv.cn

enum Color { RED, GREEN, BLUE };
来源：http://ero.daria6918.cn

[S15] C：类型转换
来源：http://awz.mhx1999.top

(double) a / b
来源：http://dwp.zdqjudy.top

[S16] C：位操作置位
来源：http://jdi.hnxiangtu.top

x |= (1 << 3);
来源：http://kvu.shangyingyoupin.top

[S17] C：安全拼接字符串
来源：http://xij.guannengcc.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wus.tarul.cn

[S18] C：命令行参数
来源：http://flh.vqdsnc.cn

int main(int argc, char **argv)
来源：http://eqy.jinqigfzy.top

[S19] C：快速排序
来源：http://njs.zhiwuduotai.top

qsort(a, n, sizeof(int), cmp);
来源：http://eoe.hcnkem.com

[S20] C：二分查找
来源：http://vlu.yonumen.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jlt.zycfv.cn

[S21] C：字符类别判断
来源：http://ini.fanxiaobao.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hgq.epnwcf.com

[S22] C：字符串转数字
来源：http://cig.tian-w.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lxc.aizwys.cn

[S23] C：随机数
来源：http://dgq.tarul.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ugs.guowangkeji.top

[S24] C：获取本地时间
来源：http://dhb.meibo888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lmm.shzxlz.cn

[S25] C：内存拷贝
来源：http://wih.c1oappe.top

memcpy(dst, src, n);
来源：http://whj.shanyushiyangkeji.top

[S26] C：内存清零
来源：http://ang.smart0.xyz

memset(a, 0, sizeof a);
来源：http://yse.xuanzx.com

[S27] C：定义常量
来源：http://cee.bbcook.cn

const double PI = 3.14159;
来源：http://mfe.ybcxt.top

[S28] C：静态变量
来源：http://kvg.yangfankeji.com

static int counter = 0;
来源：http://fnv.0kj1m.cn

[S29] C：变参函数
来源：http://cph.jqgfzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://flz.zdbjq.cn

[S30] C：头文件保护
来源：http://buh.wangdashe.top

#ifndef X_H
来源：http://uks.0kj1m.cn

#define X_H
来源：http://mju.sjlbkw.cn

#endif
来源：http://lab.yuanzhike.top

[S31] C++：Hello World
来源：http://zwj.shuidangran.top

#include <iostream>
来源：http://vtr.yanxiufei.cn

int main() { std::cout << "Hello\n"; }
来源：http://xmj.nanxinkj.top

[S32] C++：字符串
来源：http://oei.yj202588.top

std::string s = "hi";  s += "!";
来源：http://ixr.yanxiufei.cn

[S33] C++：vector 增删
来源：http://nau.aibaodan.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://imd.shangyingyoupin.top

[S34] C++：遍历 vector
来源：http://apk.shanyushiyangkeji.top

for (auto &x : v) { std::cout << x; }
来源：http://rin.hongshengwenyu.top

[S35] C++：map
来源：http://zka.daxiang520.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dyq.jlsjyb.cn

[S36] C++：unordered_map
来源：http://mrj.aizwys.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dbx.iojbl.cn

[S37] C++：set
来源：http://zsq.nwbrower.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ckf.fengsongda.top

[S38] C++：排序
来源：http://nyr.guowangkeji.top

std::sort(v.begin(), v.end());
来源：http://bzz.nanxuanxn.top

[S39] C++：自定义比较器排序
来源：http://acs.zhixingplan.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qwj.yuanzhike.top

[S40] C++：查找元素
来源：http://usd.wangshuangyany.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://slv.xylfe.cn

[S41] C++：类与构造函数
来源：http://ymf.zycfv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qya.fengsongda.top

[S42] C++：继承与虚函数
来源：http://pti.aizwys.cn

class B : public Base { public: void f() override {} };
来源：http://zxe.mhx1999.top

[S43] C++：智能指针
来源：http://tjd.guowangkeji.top

auto p = std::make_unique<int>(5);
来源：http://cix.xziqi.cn

[S44] C++：引用传参
来源：http://mrb.aibaodan.cn

void inc(int &x) { ++x; }
来源：http://tfn.ydzc1.top

[S45] C++：lambda
来源：http://daq.tarul.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ebx.jinqigufen.top

[S46] C++：函数模板
来源：http://qbt.yvedp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kbm.havefunace.top

[S47] C++：结构化绑定遍历
来源：http://reg.bbcook.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oxz.jlsjyb.cn

[S48] C++：逐行读文件
来源：http://ock.ivvv.top

std::ifstream in("a.txt");  std::string line;
来源：http://nof.xinyue.icu

while (std::getline(in, line)) { }
来源：http://ybi.ctjpmb.com

[S49] C++：写文件
来源：http://urs.smart0.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gxl.fktsv.cn

[S50] C++：格式化数字
来源：http://jst.smart0.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yyl.xinyue.icu

[S51] C++：显式类型转换
来源：http://uwp.daria6918.cn

static_cast<double>(a) / b
来源：http://tnf.haohaochexian.top

[S52] C++：const 与 noexcept
来源：http://ccy.ybcxt.top

int size() const noexcept { return n_; }
来源：http://wva.yj20258888.top

[S53] C++：移动语义
来源：http://iah.ybcxt.top

std::vector<int> w = std::move(v);
来源：http://men.sjlbkw.cn

[S54] C++：异常处理
来源：http://lau.ctjpmb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wiv.0kj1m.cn

[S55] C++：结构化绑定
来源：http://xyg.vehdjk.com

auto [a, b] = std::make_pair(1, 2);
来源：http://hto.mhx1999.top

[S56] C++：optional
来源：http://amt.shanyushiyangtech.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ggu.hfpthk.cn

[S57] C++：编译期常量
来源：http://hgr.shuidangran.top

constexpr int N = 10;
来源：http://eya.hnqzz.top

[S58] C++：命名空间
来源：http://lko.hammf.cn

namespace ns { int f() { return 1; } }
来源：http://jso.chenlongwang.top

[S59] C++：静态断言
来源：http://lak.havefunace.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qgq.guannengcc.top

[S60] C++：遍历并删除元素
来源：http://cbe.redwolf501.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xdp.zhengqikj.top

================================================================================
来源：http://srq.shuidangran.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hyt.yonumen.top

================================================================================
来源：http://qxv.hfpthk.cn

[T01] Kotlin：Hello World
来源：http://atu.ybcxt.top

println("Hello")
来源：http://agt.smart0.xyz

[T02] Kotlin：变量
来源：http://ifd.yueranfly.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zqw.chenjidiqi.icu

[T03] Kotlin：字符串模板
来源：http://esy.wangshuangyany.cn

"值: $b"
来源：http://rjk.yj202588.top

[T04] Kotlin：空安全
来源：http://kxs.hywenlv.cn

val n: String? = null;  n?.length
来源：http://sih.jqgfzy.top

[T05] Kotlin：when 表达式
来源：http://eoa.hnqzz.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kxa.hywenlv.cn

[T06] Kotlin：集合映射
来源：http://fmj.uphjek.com

listOf(1, 2, 3).map { it * 2 }
来源：http://cee.jyoumei.cn

[T07] Kotlin：集合过滤
来源：http://ueb.nanxinkj.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vad.jqgufenzy.top

[T08] Kotlin：数据类
来源：http://wha.daria6918.cn

data class User(val name: String, val age: Int)
来源：http://gze.aibaodan.cn

[T09] Kotlin：扩展函数
来源：http://hco.cdnleiting.top

fun String.exclaim() = this + "!"
来源：http://tqt.guowangkeji.top

[T10] Kotlin：默认参数
来源：http://sbx.ybcxt.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qgl.haohaochexian.top

[T11] Kotlin：协程
来源：http://rlq.jinqigfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://eeb.yj202588.top

[T12] Kotlin：解构声明
来源：http://lgr.feifeiyinyue.top

val (a, b) = Pair(1, 2)
来源：http://ega.jqgufenzy.top

[T13] Kotlin：只读 Map
来源：http://fjd.guannengcc.top

val m = mapOf("a" to 1)
来源：http://zxg.yuxming.cn

[T14] Kotlin：循环
来源：http://man.jqgufenzy.top

for (i in 1..10) println(i)
来源：http://yob.fanxiaobao.xyz

[T15] Kotlin：接口
来源：http://upl.tianlin.xyz

interface Shape { fun area(): Double }
来源：http://opo.tarul.cn

[T16] Swift：Hello World
来源：http://bqh.cdnleiting.top

print("Hello")
来源：http://uyz.cdnleiting.top

[T17] Swift：变量与常量
来源：http://osu.haohaochexian.top

var a = 1;  let b = 2
来源：http://vuv.gotoacloud.top

[T18] Swift：字符串插值
来源：http://wlq.smart0.xyz

"值: \(b)"
来源：http://lus.svipenyu.cn

[T19] Swift：可选绑定
来源：http://jri.yuxming.cn

if let n = opt { print(n) }
来源：http://cvi.shanyushiyangkeji.top

[T20] Swift：数组操作
来源：http://vqb.0kj1m.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rwj.xinyue.icu

[T21] Swift：遍历
来源：http://lkp.yangfankeji.com

for x in a { print(x) }
来源：http://kls.zdqjudy.top

[T22] Swift：字典
来源：http://lad.xingfuxueyuan.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://umc.guannengcc.top

[T23] Swift：函数
来源：http://snd.yonumen.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kle.xuanzx.com

[T24] Swift：闭包
来源：http://fnr.hesvh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ycl.zhoulong.xyz

[T25] Swift：结构体
来源：http://sro.daria6918.cn

struct P { var x: Int }
来源：http://hof.zhixingplan.top

[T26] Swift：类与重写
来源：http://ddr.ydjk.org.cn

class A: Base { override func f() {} }
来源：http://yok.smart0.xyz

[T27] Swift：错误处理
来源：http://qhz.yongpay.top

do { try f() } catch { print(error) }
来源：http://pxk.yj202588.top

[T28] Swift：枚举
来源：http://cks.gogol.net.cn

enum Color { case red, green }
来源：http://fui.xinyue.icu

[T29] Swift：guard 提前返回
来源：http://vjx.pengpengdd.cyou

guard let x = opt else { return }
来源：http://ylc.pycfn.com

[T30] Swift：协议
来源：http://jkz.hywenlv.cn

protocol Shape { func area() -> Double }
来源：http://zhg.yangfankeji.com

[T31] Lua：Hello World
来源：http://qbc.wangshuangyany.cn

print("Hello")
来源：http://jnn.fzhhl.top

[T32] Lua：局部变量
来源：http://zcw.ybcxt.top

local a = 1
来源：http://xdj.jinqigfzy.top

[T33] Lua：表（数组）
来源：http://yjf.sufxvd.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zeo.zhongyouzk.top

[T34] Lua：遍历表
来源：http://wqm.zdbjq.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://knf.kuanghao11.cn

[T35] Lua：字典表
来源：http://tim.ctjpmb.com

local d = { a = 1 };  d.b = 2
来源：http://gbg.tianlin.xyz

[T36] Lua：函数
来源：http://pap.daria6918.cn

function add(a, b) return a + b end
来源：http://buq.hcnkem.com

[T37] Lua：字符串拼接
来源：http://ulf.tarul.cn

"a" .. "b"
来源：http://ilp.zhengqikj.top

[T38] Lua：条件
来源：http://zxp.0kj1m.cn

if x > 0 then print("正") end
来源：http://bwu.jianghu66.top

[T39] Lua：模式匹配
来源：http://alp.gzhubu.top

string.find(s, "%d+")
来源：http://iom.uphjek.com

[T40] Lua：元表
来源：http://cjz.hnqzz.top

setmetatable({}, { __index = base })
来源：http://xsn.jinqigufen.top

[T41] Perl：Hello World
来源：http://lrj.sweek.top

print "Hello\n";
来源：http://xkx.cashguo.top

[T42] Perl：变量类型
来源：http://yad.jiagoushi.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://swt.fengsongda.top

[T43] Perl：字符串插值
来源：http://lnq.yongpay.top

"值: $a"
来源：http://mea.shanyushiyangtech.top

[T44] Perl：条件
来源：http://dta.cashguo.top

if ($a > 0) { print "正"; }
来源：http://dek.wangshuangyany.cn

[T45] Perl：数组遍历
来源：http://khq.sxryk.cn

for my $x (@arr) { print $x; }
来源：http://mna.jinyuanbaomall.cn

[T46] Perl：哈希操作
来源：http://ecv.jinghuilouyu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jfj.ywan-chungtsiang.top

[T47] Perl：正则捕获
来源：http://bhr.guowangkeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://akt.fzhhl.top

[T48] Perl：正则替换
来源：http://rup.gaohongyu789.top

$s =~ s/old/new/g;
来源：http://tlv.redwolf501.top

[T49] Perl：函数
来源：http://ory.jiagoushi.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dsd.gaohongyu789.top

[T50] Perl：逐行读文件
来源：http://vgk.fehbvm.com

open my $fh, "<", "a.txt" or die $!;
来源：http://prx.feifeiyinyue.top

while (my $line = <$fh>) { print $line; }
来源：http://dkq.sjlbkw.cn

[T51] Scala：Hello World
来源：http://eys.bjfxy.top

println("Hello")
来源：http://hyr.hywenlv.cn

[T52] Scala：变量
来源：http://bvw.cheryme.top

val a = 1;  var b = 2
来源：http://csz.hywenlv.cn

[T53] Scala：字符串插值
来源：http://vwp.zhijiandao.cn

s"值: $b"
来源：http://qic.fzhhl.top

[T54] Scala：集合映射
来源：http://ycd.jinghuilouyu.cn

List(1, 2, 3).map(_ * 2)
来源：http://ias.hnxiangtu.top

[T55] Scala：集合过滤
来源：http://kff.dianchejie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gbn.ywan-chungtsiang.top

[T56] Scala：样例类
来源：http://vzi.ehwqpu.com

case class User(name: String, age: Int)
来源：http://ppz.haohaochexian.top

[T57] Scala：模式匹配
来源：http://fky.pycfn.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://xhv.xuanzx.com

[T58] Scala：函数定义
来源：http://enq.fehbvm.com

def add(a: Int, b: Int): Int = a + b
来源：http://gro.gzhubu.top

[T59] Scala：循环
来源：http://zpb.wangshuangyany.cn

for (i <- 1 to 10) println(i)
来源：http://fbk.c1oappe.top

[T60] Scala：折叠
来源：http://ztf.havefunace.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qwt.hcnkem.com

================================================================================
来源：http://pak.meibo888.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://twl.yfazqb.com

================================================================================
来源：http://qfn.9152youxi.cn

[U01] Py：创建虚拟环境
来源：http://dqj.jinqigufen.top

python -m venv .venv && source .venv/bin/activate
来源：http://esd.yongpay.top

[U02] Py：导出 / 安装依赖
来源：http://mbi.ehwqpu.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lzc.yuxming.cn

[U03] Py：加载 .env 配置
来源：http://fzw.yangfankeji.com

from dotenv import load_dotenv; load_dotenv()
来源：http://znm.ybcxt.top

[U04] Py：变量调试打印
来源：http://svx.svipenyu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://csh.pycfn.com


<!-- 参考信息 -->