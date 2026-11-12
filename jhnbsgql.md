代发 wailian999

df -h;  du -sh *
来源：http://jqt.52xcode.cn

[R62] 找最占空间的文件
来源：http://wgw.shzxlz.cn

du -ah . | sort -rh | head -10
来源：http://udr.daria6918.cn

[R63] 内存与进程
来源：http://mbp.hfpthk.cn

free -h;  ps aux | grep nginx
来源：http://xay.yueranfly.top

[R64] 结束进程
来源：http://opo.vqdsnc.cn

kill -9 $(pgrep -f app.py)
来源：http://udz.nwbrower.top

[R65] 查看端口占用
来源：http://txi.uphjek.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nys.yanxiufei.cn

[R66] 定时任务
来源：http://btk.wangdashe.top

crontab -e;  crontab -l
来源：http://mai.feifeiyinyue.top

[R67] 生成随机十六进制串
来源：http://kvo.ctjpmb.com

openssl rand -hex 16
来源：http://tiu.cdnleiting.top

[R68] 计算文件校验值
来源：http://dqw.xuetiantiany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gdw.nanxuanxn.top

[R69] 生成随机密码
来源：http://wyg.jianghu66.top

head -c 16 /dev/urandom | base64
来源：http://aku.svipenyu.cn

[R70] 时间戳与互转
来源：http://ikd.shangyingyoupin.top

date +%s;  date -d @1700000000
来源：http://zfy.ydzc1.top

[R71] 日期格式化
来源：http://ira.hysaishi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://oqx.52xcode.cn

[R72] 等待端口就绪
来源：http://rmx.sweek.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zyb.jinqigfzy.top

[R73] 分割大日志
来源：http://fyt.vehdjk.com

split -l 1000 big.log part_
来源：http://udj.uphjek.com

[R74] 批量重命名
来源：http://rhb.yvedp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://elp.ppjwa.cn

[R75] 导出环境变量
来源：http://mol.cucudq.cn

export PATH="$HOME/bin:$PATH"
来源：http://voz.ydzc1.top

[R76] 使用临时文件
来源：http://eoz.jinyuanbaomall.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://npa.hongshengwenyu.top

[R77] 读取用户输入
来源：http://lnv.yongpay.top

read -rp "请输入: " ans
来源：http://nzm.jqgfzy.top

[R78] 交互式菜单
来源：http://zzy.uphjek.com

select opt in a b c; do echo "$opt"; break; done
来源：http://zws.iojbl.cn

[R79] 解析命令行选项
来源：http://zop.sxryk.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lpx.shanyushiyangtech.top

[R80] 查看脚本执行耗时
来源：http://spr.sweek.top

time ./run.sh
来源：http://ybt.sweek.top

================================================================================
来源：http://zqi.shzxlz.cn

S. C / C++ 专题
来源：http://bqu.ppjwa.cn

================================================================================
来源：http://fxa.birdmap.top

[S01] C：Hello World
来源：http://kjy.ehwqpu.com

#include <stdio.h>
来源：http://bai.jinyuanbaomall.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://iaf.tanke756.top

[S02] C：变量与格式化输出
来源：http://tpx.cucudq.cn

int a = 10; printf("%d\n", a);
来源：http://pis.hammf.cn

[S03] C：读入整数
来源：http://ftk.fanxiaobao.xyz

int x; scanf("%d", &x);
来源：http://pzq.yuanzhike.top

[S04] C：字符串复制
来源：http://tpk.cheryme.top

char dst[32]; strcpy(dst, "hi");
来源：http://tcb.smart0.xyz

[S05] C：字符串长度
来源：http://leu.uphjek.com

strlen(s)
来源：http://nkk.jqgufenzy.top

[S06] C：字符串比较
来源：http://cqj.jianghu66.top

strcmp(a, b) == 0
来源：http://lfw.316326.xyz

[S07] C：数组遍历求和
来源：http://bqz.hammf.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mwe.sufxvd.cn

[S08] C：动态内存分配与释放
来源：http://yrl.yanxiufei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ppt.nanxuanxn.top

[S09] C：结构体定义与初始化
来源：http://wyi.birdmap.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nke.yanxiufei.cn

[S10] C：指针与解引用
来源：http://qed.cucudq.cn

int *p = &a;  *p = 5;
来源：http://xrh.xingfuxueyuan.xyz

[S11] C：逐行读文件
来源：http://ehp.yfazqb.com

FILE *f = fopen("a.txt", "r");
来源：http://adv.bbcook.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lcw.jianghu66.top

fclose(f);
来源：http://hcj.yongpay.top

[S12] C：写文件
来源：http://kwo.hcnkem.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vkq.jinyuanbaomall.cn

[S13] C：宏定义
来源：http://xfd.zhixingplan.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nhm.snrcjt.cn

[S14] C：枚举
来源：http://tee.fengsongda.top

enum Color { RED, GREEN, BLUE };
来源：http://fib.jinyuanbaomall.cn

[S15] C：类型转换
来源：http://cta.iojbl.cn

(double) a / b
来源：http://pds.cheryme.top

[S16] C：位操作置位
来源：http://ptj.dianchejie.cn

x |= (1 << 3);
来源：http://wmw.316326.xyz

[S17] C：安全拼接字符串
来源：http://wxr.zhaomingkeji.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bss.hfpthk.cn

[S18] C：命令行参数
来源：http://cok.xinyue.icu

int main(int argc, char **argv)
来源：http://aqg.uphjek.com

[S19] C：快速排序
来源：http://xyl.hammf.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vlr.nanxinkj.top

[S20] C：二分查找
来源：http://ipq.zdqjudy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ttn.shangyingyoupin.top

[S21] C：字符类别判断
来源：http://tlw.zhoulong.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yeu.hfpthk.cn

[S22] C：字符串转数字
来源：http://vtv.shzxlz.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tzt.cucudq.cn

[S23] C：随机数
来源：http://kiw.jqgufenzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qkm.xziqi.cn

[S24] C：获取本地时间
来源：http://kud.yuxming.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sjq.fktsv.cn

[S25] C：内存拷贝
来源：http://nyt.yanxiufei.cn

memcpy(dst, src, n);
来源：http://bzf.xinyue.icu

[S26] C：内存清零
来源：http://bdz.dianchejie.cn

memset(a, 0, sizeof a);
来源：http://zcq.yvedp.cn

[S27] C：定义常量
来源：http://eut.hcnkem.com

const double PI = 3.14159;
来源：http://zif.fengsongda.top

[S28] C：静态变量
来源：http://onw.fktsv.cn

static int counter = 0;
来源：http://lxq.wangshuangyany.cn

[S29] C：变参函数
来源：http://adl.ivvv.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ket.zdbjq.cn

[S30] C：头文件保护
来源：http://bky.ydjk.org.cn

#ifndef X_H
来源：http://jzq.yuxming.cn

#define X_H
来源：http://zih.vqdsnc.cn

#endif
来源：http://nfv.yongpay.top

[S31] C++：Hello World
来源：http://igo.redwolf501.top

#include <iostream>
来源：http://kan.chenlongwang.top

int main() { std::cout << "Hello\n"; }
来源：http://lrx.0kj1m.cn

[S32] C++：字符串
来源：http://cnx.fehbvm.com

std::string s = "hi";  s += "!";
来源：http://dcs.zhongyouzk.top

[S33] C++：vector 增删
来源：http://zur.yfazqb.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vbe.xylfe.cn

[S34] C++：遍历 vector
来源：http://uti.yueranfly.top

for (auto &x : v) { std::cout << x; }
来源：http://frr.jianghu66.top

[S35] C++：map
来源：http://mff.ctjpmb.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hzj.jqgufenzy.top

[S36] C++：unordered_map
来源：http://ppz.jlsjyb.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ovh.ivvv.top

[S37] C++：set
来源：http://hmv.jinqigufen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://iqc.zhiwuduotai.top

[S38] C++：排序
来源：http://rdm.xylfe.cn

std::sort(v.begin(), v.end());
来源：http://cgd.xuetiantiany.cn

[S39] C++：自定义比较器排序
来源：http://lxp.sweek.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eph.sxryk.cn

[S40] C++：查找元素
来源：http://pge.gzhubu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cux.tianlin.xyz

[S41] C++：类与构造函数
来源：http://aao.fengsongda.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qzk.gotoacloud.top

[S42] C++：继承与虚函数
来源：http://sns.zdqjudy.top

class B : public Base { public: void f() override {} };
来源：http://mua.xuanzx.com

[S43] C++：智能指针
来源：http://twu.zhongyouzk.top

auto p = std::make_unique<int>(5);
来源：http://ync.zhengqikj.top

[S44] C++：引用传参
来源：http://yfa.bjfxy.top

void inc(int &x) { ++x; }
来源：http://dte.mhx1999.top

[S45] C++：lambda
来源：http://ijx.havefunace.top

auto add = [](int a, int b) { return a + b; };
来源：http://zfg.havefunace.top

[S46] C++：函数模板
来源：http://jhk.tianlin.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mue.daxiang520.top

[S47] C++：结构化绑定遍历
来源：http://eyc.fktsv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://syi.zdbjq.cn

[S48] C++：逐行读文件
来源：http://ufd.sxryk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nzq.quarkkingdee.top

while (std::getline(in, line)) { }
来源：http://ish.yuxming.cn

[S49] C++：写文件
来源：http://xng.havefunace.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kej.gotoacloud.top

[S50] C++：格式化数字
来源：http://vcv.xuanzx.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yjk.jinyuanbaomall.cn

[S51] C++：显式类型转换
来源：http://way.hfpthk.cn

static_cast<double>(a) / b
来源：http://mmy.yuxming.cn

[S52] C++：const 与 noexcept
来源：http://myc.fanxiaobao.xyz

int size() const noexcept { return n_; }
来源：http://taj.xuanzx.com

[S53] C++：移动语义
来源：http://iwo.guannengcc.top

std::vector<int> w = std::move(v);
来源：http://ocn.zdqjudy.top

[S54] C++：异常处理
来源：http://dda.wangdashe.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yrj.haohaochexian.top

[S55] C++：结构化绑定
来源：http://olk.jinyuanbaomall.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xds.sjlbkw.cn

[S56] C++：optional
来源：http://tpc.nanxuanxn.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tiw.haohaochexian.top

[S57] C++：编译期常量
来源：http://wko.chenjidiqi.icu

constexpr int N = 10;
来源：http://vla.shanyushiyangkeji.top

[S58] C++：命名空间
来源：http://frz.fktsv.cn

namespace ns { int f() { return 1; } }
来源：http://xyc.yj20258.top

[S59] C++：静态断言
来源：http://zxl.daxiang520.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mgq.cucudq.cn

[S60] C++：遍历并删除元素
来源：http://njn.shanyushiyangkeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zcg.cucudq.cn

================================================================================
来源：http://wca.jiagoushi.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tdd.wangshuangyany.cn

================================================================================
来源：http://axd.svipenyu.cn

[T01] Kotlin：Hello World
来源：http://dpu.daria6918.cn

println("Hello")
来源：http://vnb.feifeiyinyue.top

[T02] Kotlin：变量
来源：http://rue.guannengcc.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xps.snrcjt.cn

[T03] Kotlin：字符串模板
来源：http://nkj.ivvv.top

"值: $b"
来源：http://vkz.hcnkem.com

[T04] Kotlin：空安全
来源：http://irz.ppjwa.cn

val n: String? = null;  n?.length
来源：http://ycr.fehbvm.com

[T05] Kotlin：when 表达式
来源：http://wgl.hcnkem.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ksw.yvedp.cn

[T06] Kotlin：集合映射
来源：http://igb.xinyue.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://ykk.jqgufenzy.top

[T07] Kotlin：集合过滤
来源：http://kda.jlsjyb.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bjn.hywenlv.cn

[T08] Kotlin：数据类
来源：http://pci.yueranfly.top

data class User(val name: String, val age: Int)
来源：http://fdt.yfazqb.com

[T09] Kotlin：扩展函数
来源：http://suf.dianchejie.cn

fun String.exclaim() = this + "!"
来源：http://bic.guowangkeji.top

[T10] Kotlin：默认参数
来源：http://dyi.yvedp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ctc.smart0.xyz

[T11] Kotlin：协程
来源：http://xkp.shanyushiyangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://qaj.gotoacloud.top

[T12] Kotlin：解构声明
来源：http://kml.andypj.xyz

val (a, b) = Pair(1, 2)
来源：http://utn.ivvv.top

[T13] Kotlin：只读 Map
来源：http://dcc.cdnleiting.top

val m = mapOf("a" to 1)
来源：http://ymk.9152youxi.cn

[T14] Kotlin：循环
来源：http://fnq.hywenlv.cn

for (i in 1..10) println(i)
来源：http://qzs.epnwcf.com

[T15] Kotlin：接口
来源：http://nnt.shuidangran.top

interface Shape { fun area(): Double }
来源：http://wvr.quarkkingdee.top

[T16] Swift：Hello World
来源：http://irs.yuxming.cn

print("Hello")
来源：http://pjx.snrcjt.cn

[T17] Swift：变量与常量
来源：http://lcy.shanyushiyangtech.top

var a = 1;  let b = 2
来源：http://zvf.jiagoushi.top

[T18] Swift：字符串插值
来源：http://poc.zhengqikj.top

"值: \(b)"
来源：http://yel.nanxinkj.top

[T19] Swift：可选绑定
来源：http://dvp.wangshuangyany.cn

if let n = opt { print(n) }
来源：http://yvu.jinyuanbaomall.cn

[T20] Swift：数组操作
来源：http://bdn.wangshuangyany.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xlk.0kj1m.cn

[T21] Swift：遍历
来源：http://aik.tian-w.cn

for x in a { print(x) }
来源：http://ipz.sjlbkw.cn

[T22] Swift：字典
来源：http://myu.vehdjk.com

var d = ["a": 1];  d["b"] = 2
来源：http://soj.xinyue.icu

[T23] Swift：函数
来源：http://ppv.smart0.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vrw.pengpengdd.cyou

[T24] Swift：闭包
来源：http://bdz.aizwys.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fnm.zhaomingkeji.xyz

[T25] Swift：结构体
来源：http://ekc.yongpay.top

struct P { var x: Int }
来源：http://ivb.sxryk.cn

[T26] Swift：类与重写
来源：http://qnc.jlsjyb.cn

class A: Base { override func f() {} }
来源：http://bci.pengpengdd.cyou

[T27] Swift：错误处理
来源：http://lfp.svipenyu.cn

do { try f() } catch { print(error) }
来源：http://kte.guowangkeji.top

[T28] Swift：枚举
来源：http://wvd.jianghu66.top

enum Color { case red, green }
来源：http://oeo.dianchejie.cn

[T29] Swift：guard 提前返回
来源：http://dlq.hongshengwenyu.top

guard let x = opt else { return }
来源：http://ars.vqdsnc.cn

[T30] Swift：协议
来源：http://tnb.daria6918.cn

protocol Shape { func area() -> Double }
来源：http://bhw.shangyingyoupin.top

[T31] Lua：Hello World
来源：http://hnl.hesvh.cn

print("Hello")
来源：http://ahf.hongshengwenyu.top

[T32] Lua：局部变量
来源：http://kpg.aizwys.cn

local a = 1
来源：http://mai.jyoumei.cn

[T33] Lua：表（数组）
来源：http://cfy.aibaodan.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://pox.jinqigfzy.top

[T34] Lua：遍历表
来源：http://mta.0kj1m.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gme.vehdjk.com

[T35] Lua：字典表
来源：http://jht.andypj.xyz

local d = { a = 1 };  d.b = 2
来源：http://bcp.feifeiyinyue.top

[T36] Lua：函数
来源：http://cjx.xylfe.cn

function add(a, b) return a + b end
来源：http://ama.shangyingyoupin.top

[T37] Lua：字符串拼接
来源：http://zen.yueranfly.top

"a" .. "b"
来源：http://tpt.meibo888.top

[T38] Lua：条件
来源：http://whr.hfpthk.cn

if x > 0 then print("正") end
来源：http://oyv.zycfv.cn

[T39] Lua：模式匹配
来源：http://fch.iojbl.cn

string.find(s, "%d+")
来源：http://tzq.shuidangran.top

[T40] Lua：元表
来源：http://zyw.fehbvm.com

setmetatable({}, { __index = base })
来源：http://nsa.iojbl.cn

[T41] Perl：Hello World
来源：http://nuf.sysykeji.top

print "Hello\n";
来源：http://mxi.zdqjudy.top

[T42] Perl：变量类型
来源：http://pun.daria6918.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dva.jinqigfzy.top

[T43] Perl：字符串插值
来源：http://hqd.nanxuanxn.top

"值: $a"
来源：http://cqf.cucudq.cn

[T44] Perl：条件
来源：http://glw.ywan-chungtsiang.top

if ($a > 0) { print "正"; }
来源：http://eba.jianghu66.top

[T45] Perl：数组遍历
来源：http://qod.hongshengwenyu.top

for my $x (@arr) { print $x; }
来源：http://mhd.jlsjyb.cn

[T46] Perl：哈希操作
来源：http://rwm.haohaochexian.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hzm.vehdjk.com

[T47] Perl：正则捕获
来源：http://bww.zhoulong.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://ygl.hfpthk.cn

[T48] Perl：正则替换
来源：http://mpc.feifeiyinyue.top

$s =~ s/old/new/g;
来源：http://pqa.chenjidiqi.icu

[T49] Perl：函数
来源：http://nev.smart0.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ecq.chenlongwang.top

[T50] Perl：逐行读文件
来源：http://yiw.yongpay.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hml.shangyingyoupin.top

while (my $line = <$fh>) { print $line; }
来源：http://shz.uphjek.com

[T51] Scala：Hello World
来源：http://nec.redwolf501.top

println("Hello")
来源：http://saq.sxryk.cn

[T52] Scala：变量
来源：http://jnf.jqgfzy.top

val a = 1;  var b = 2
来源：http://gie.9152youxi.cn

[T53] Scala：字符串插值
来源：http://uqj.jqgfzy.top

s"值: $b"
来源：http://ifd.andypj.xyz

[T54] Scala：集合映射
来源：http://ubo.ywan-chungtsiang.top

List(1, 2, 3).map(_ * 2)
来源：http://qzc.hnxiangtu.top

[T55] Scala：集合过滤
来源：http://wcz.sysykeji.top

List(1, 2, 3).filter(_ > 1)
来源：http://ibz.vqdsnc.cn

[T56] Scala：样例类
来源：http://mtj.zhoulong.xyz

case class User(name: String, age: Int)
来源：http://paf.xingfuxueyuan.xyz

[T57] Scala：模式匹配
来源：http://wgi.snrcjt.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yab.shuidangran.top

[T58] Scala：函数定义
来源：http://hcw.hesvh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://uqa.tarul.cn

[T59] Scala：循环
来源：http://bvq.hnxiangtu.top

for (i <- 1 to 10) println(i)
来源：http://lso.sysykeji.top

[T60] Scala：折叠
来源：http://qyc.xziqi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://exq.smart0.xyz

================================================================================
来源：http://xdj.fengsongda.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kmw.c1oappe.top

================================================================================
来源：http://ruf.yanxiufei.cn

[U01] Py：创建虚拟环境
来源：http://bje.ydjk.org.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cda.nanxinkj.top

[U02] Py：导出 / 安装依赖
来源：http://hvs.xingfuxueyuan.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hcj.hnxiangtu.top


<!-- 参考信息 -->