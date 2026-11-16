代发 wailian999

df -h;  du -sh *
来源：http://ogf.jqgfzy.top

[R62] 找最占空间的文件
来源：http://upf.uphjek.com

du -ah . | sort -rh | head -10
来源：http://ejm.havefunace.top

[R63] 内存与进程
来源：http://ijg.sjlbkw.cn

free -h;  ps aux | grep nginx
来源：http://gzf.chenjidiqi.icu

[R64] 结束进程
来源：http://egu.fengsongda.top

kill -9 $(pgrep -f app.py)
来源：http://uir.guannengcc.top

[R65] 查看端口占用
来源：http://zql.9152youxi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mmv.bbcook.cn

[R66] 定时任务
来源：http://znm.tarul.cn

crontab -e;  crontab -l
来源：http://wkm.vehdjk.com

[R67] 生成随机十六进制串
来源：http://kwe.zhiwuduotai.top

openssl rand -hex 16
来源：http://gfz.kuanghao11.cn

[R68] 计算文件校验值
来源：http://gun.pycfn.com

sha256sum a.txt;  md5sum a.txt
来源：http://jva.jinghuilouyu.cn

[R69] 生成随机密码
来源：http://jtw.shzxlz.cn

head -c 16 /dev/urandom | base64
来源：http://gnm.hywenlv.cn

[R70] 时间戳与互转
来源：http://jys.zhoulong.xyz

date +%s;  date -d @1700000000
来源：http://mjg.yanxiufei.cn

[R71] 日期格式化
来源：http://whv.mhx1999.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xjm.cashguo.top

[R72] 等待端口就绪
来源：http://cqp.chenjidiqi.icu

until nc -z localhost 3306; do sleep 1; done
来源：http://zvm.yj20258888.top

[R73] 分割大日志
来源：http://ozq.ctjpmb.com

split -l 1000 big.log part_
来源：http://zyj.redwolf501.top

[R74] 批量重命名
来源：http://cwi.zhiwuduotai.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cas.hfpthk.cn

[R75] 导出环境变量
来源：http://tcx.hfpthk.cn

export PATH="$HOME/bin:$PATH"
来源：http://ksj.zhiwuduotai.top

[R76] 使用临时文件
来源：http://xjm.zycfv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://had.ehwqpu.com

[R77] 读取用户输入
来源：http://efw.zhiwuduotai.top

read -rp "请输入: " ans
来源：http://jgr.guowangkeji.top

[R78] 交互式菜单
来源：http://xgm.xuanzx.com

select opt in a b c; do echo "$opt"; break; done
来源：http://tio.jqgfzy.top

[R79] 解析命令行选项
来源：http://gro.zhoulong.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xmr.zhoulong.xyz

[R80] 查看脚本执行耗时
来源：http://agy.birdmap.top

time ./run.sh
来源：http://ikb.zhongyouzk.top

================================================================================
来源：http://cli.yangfankeji.com

S. C / C++ 专题
来源：http://zhq.hfpthk.cn

================================================================================
来源：http://nxx.zhoulong.xyz

[S01] C：Hello World
来源：http://ufl.316326.xyz

#include <stdio.h>
来源：http://yqi.cheryme.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ohp.yj20258888.top

[S02] C：变量与格式化输出
来源：http://tqj.wangshuangyany.cn

int a = 10; printf("%d\n", a);
来源：http://ten.cheryme.top

[S03] C：读入整数
来源：http://vrj.fengsongda.top

int x; scanf("%d", &x);
来源：http://tmn.jqgfzy.top

[S04] C：字符串复制
来源：http://pfh.cashguo.top

char dst[32]; strcpy(dst, "hi");
来源：http://bxy.sysykeji.top

[S05] C：字符串长度
来源：http://eda.hfpthk.cn

strlen(s)
来源：http://bfq.xuetiantiany.cn

[S06] C：字符串比较
来源：http://iuf.gzhubu.top

strcmp(a, b) == 0
来源：http://fcr.svipenyu.cn

[S07] C：数组遍历求和
来源：http://kri.svipenyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zmf.tian-w.cn

[S08] C：动态内存分配与释放
来源：http://vyc.ctjpmb.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lkt.zycfv.cn

[S09] C：结构体定义与初始化
来源：http://cmz.jiagoushi.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bll.nanxinkj.top

[S10] C：指针与解引用
来源：http://sjo.redwolf501.top

int *p = &a;  *p = 5;
来源：http://blk.xingfuxueyuan.xyz

[S11] C：逐行读文件
来源：http://kkh.guowangkeji.top

FILE *f = fopen("a.txt", "r");
来源：http://jdo.pengpengdd.cyou

while (fgets(buf, sizeof buf, f)) { }
来源：http://nph.tarul.cn

fclose(f);
来源：http://rjz.fktsv.cn

[S12] C：写文件
来源：http://rqa.hysaishi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nmi.guannengcc.top

[S13] C：宏定义
来源：http://jvh.zdbjq.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zwz.fengsongda.top

[S14] C：枚举
来源：http://ezo.quarkkingdee.top

enum Color { RED, GREEN, BLUE };
来源：http://mtv.cucudq.cn

[S15] C：类型转换
来源：http://wgv.shangyingyoupin.top

(double) a / b
来源：http://sbs.hesvh.cn

[S16] C：位操作置位
来源：http://tgc.cheryme.top

x |= (1 << 3);
来源：http://wbc.jinqigufen.top

[S17] C：安全拼接字符串
来源：http://cju.hongshengwenyu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nmh.ehwqpu.com

[S18] C：命令行参数
来源：http://wjj.yfazqb.com

int main(int argc, char **argv)
来源：http://pbh.nanxinkj.top

[S19] C：快速排序
来源：http://tkq.zhaomingkeji.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://fbs.sysykeji.top

[S20] C：二分查找
来源：http://spi.bjfxy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dvd.hcnkem.com

[S21] C：字符类别判断
来源：http://gmn.xuetiantiany.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cth.yuanzhike.top

[S22] C：字符串转数字
来源：http://wsj.redwolf501.top

atoi("42");  strtod("3.14", NULL);
来源：http://nxi.zdqjudy.top

[S23] C：随机数
来源：http://itq.havefunace.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ory.hnqzz.top

[S24] C：获取本地时间
来源：http://pht.zycfv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://azk.ehwqpu.com

[S25] C：内存拷贝
来源：http://ziw.dashuyun.cn

memcpy(dst, src, n);
来源：http://vlx.feifeiyinyue.top

[S26] C：内存清零
来源：http://vsh.nanxuanxn.top

memset(a, 0, sizeof a);
来源：http://sjl.feifeiyinyue.top

[S27] C：定义常量
来源：http://yxo.svipenyu.cn

const double PI = 3.14159;
来源：http://jbu.smart0.xyz

[S28] C：静态变量
来源：http://oqg.wangshuangyany.cn

static int counter = 0;
来源：http://zbj.52xcode.cn

[S29] C：变参函数
来源：http://vws.hywenlv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rab.ehwqpu.com

[S30] C：头文件保护
来源：http://aqx.zhixingplan.top

#ifndef X_H
来源：http://uvu.jinqigufen.top

#define X_H
来源：http://tko.snrcjt.cn

#endif
来源：http://lim.hywenlv.cn

[S31] C++：Hello World
来源：http://uek.yuxming.cn

#include <iostream>
来源：http://wjm.chenzaomai.com

int main() { std::cout << "Hello\n"; }
来源：http://vml.0kj1m.cn

[S32] C++：字符串
来源：http://ghu.sufxvd.cn

std::string s = "hi";  s += "!";
来源：http://aea.ydjk.org.cn

[S33] C++：vector 增删
来源：http://euq.daria6918.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tlm.nanxinkj.top

[S34] C++：遍历 vector
来源：http://thp.quarkkingdee.top

for (auto &x : v) { std::cout << x; }
来源：http://uad.tianlin.xyz

[S35] C++：map
来源：http://alx.hcnkem.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tqg.shzxlz.cn

[S36] C++：unordered_map
来源：http://awe.feifeiyinyue.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nvo.fehbvm.com

[S37] C++：set
来源：http://ass.sweek.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://iar.hnqzz.top

[S38] C++：排序
来源：http://hwu.jyoumei.cn

std::sort(v.begin(), v.end());
来源：http://ckg.aibaodan.cn

[S39] C++：自定义比较器排序
来源：http://xdj.guowangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://knt.nanxinkj.top

[S40] C++：查找元素
来源：http://dtw.quarkkingdee.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pvn.smart0.xyz

[S41] C++：类与构造函数
来源：http://zzv.sxryk.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uvb.fehbvm.com

[S42] C++：继承与虚函数
来源：http://hvb.gotoacloud.top

class B : public Base { public: void f() override {} };
来源：http://fcd.sufxvd.cn

[S43] C++：智能指针
来源：http://uqm.redwolf501.top

auto p = std::make_unique<int>(5);
来源：http://icz.zycfv.cn

[S44] C++：引用传参
来源：http://zaq.zdbjq.cn

void inc(int &x) { ++x; }
来源：http://eea.zhengqikj.top

[S45] C++：lambda
来源：http://ciq.zhixingplan.top

auto add = [](int a, int b) { return a + b; };
来源：http://wxw.jyoumei.cn

[S46] C++：函数模板
来源：http://atv.birdmap.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bqq.hongshengwenyu.top

[S47] C++：结构化绑定遍历
来源：http://ipu.cheryme.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://aqe.zhoulong.xyz

[S48] C++：逐行读文件
来源：http://szl.jqgfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://jbi.yueranfly.top

while (std::getline(in, line)) { }
来源：http://ypv.meibo888.top

[S49] C++：写文件
来源：http://otz.nanxinkj.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hts.xinyue.icu

[S50] C++：格式化数字
来源：http://byo.jyoumei.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qqd.xuanzx.com

[S51] C++：显式类型转换
来源：http://lsa.xziqi.cn

static_cast<double>(a) / b
来源：http://etr.meibo888.top

[S52] C++：const 与 noexcept
来源：http://exy.gzhubu.top

int size() const noexcept { return n_; }
来源：http://tba.ppjwa.cn

[S53] C++：移动语义
来源：http://qvj.wangshuangyany.cn

std::vector<int> w = std::move(v);
来源：http://arf.jinyuanbaomall.cn

[S54] C++：异常处理
来源：http://jgy.aizwys.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kre.yfazqb.com

[S55] C++：结构化绑定
来源：http://fab.xingfuxueyuan.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://qki.shanyushiyangtech.top

[S56] C++：optional
来源：http://bit.redwolf501.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gxp.zhaomingkeji.xyz

[S57] C++：编译期常量
来源：http://qed.jinghuilouyu.cn

constexpr int N = 10;
来源：http://zuh.xuetiantiany.cn

[S58] C++：命名空间
来源：http://ciq.pycfn.com

namespace ns { int f() { return 1; } }
来源：http://aym.pycfn.com

[S59] C++：静态断言
来源：http://svf.aizwys.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bcd.tarul.cn

[S60] C++：遍历并删除元素
来源：http://wqs.jqgufenzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lrh.vehdjk.com

================================================================================
来源：http://hnc.tian-w.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bba.zhixingplan.top

================================================================================
来源：http://pmi.guannengcc.top

[T01] Kotlin：Hello World
来源：http://uxd.yonumen.top

println("Hello")
来源：http://gik.fanxiaobao.xyz

[T02] Kotlin：变量
来源：http://url.daxiang520.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nui.jqgfzy.top

[T03] Kotlin：字符串模板
来源：http://utl.dashuyun.cn

"值: $b"
来源：http://qri.ydzc1.top

[T04] Kotlin：空安全
来源：http://igm.jqgufenzy.top

val n: String? = null;  n?.length
来源：http://azp.quarkkingdee.top

[T05] Kotlin：when 表达式
来源：http://xce.fengsongda.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qbu.vqdsnc.cn

[T06] Kotlin：集合映射
来源：http://mxf.fktsv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gyq.nwbrower.top

[T07] Kotlin：集合过滤
来源：http://bhc.wangshuangyany.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ixs.tarul.cn

[T08] Kotlin：数据类
来源：http://nvt.ybcxt.top

data class User(val name: String, val age: Int)
来源：http://zor.sufxvd.cn

[T09] Kotlin：扩展函数
来源：http://eqw.havefunace.top

fun String.exclaim() = this + "!"
来源：http://nkl.hywenlv.cn

[T10] Kotlin：默认参数
来源：http://ehu.feifeiyinyue.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nqc.jinqigfzy.top

[T11] Kotlin：协程
来源：http://jkn.tarul.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qsc.316326.xyz

[T12] Kotlin：解构声明
来源：http://wlp.chenjidiqi.icu

val (a, b) = Pair(1, 2)
来源：http://jex.andypj.xyz

[T13] Kotlin：只读 Map
来源：http://jxe.shangyingyoupin.top

val m = mapOf("a" to 1)
来源：http://clq.xylfe.cn

[T14] Kotlin：循环
来源：http://mev.jianghu66.top

for (i in 1..10) println(i)
来源：http://mjw.wangshuangyany.cn

[T15] Kotlin：接口
来源：http://ccm.gogol.net.cn

interface Shape { fun area(): Double }
来源：http://fvl.ybcxt.top

[T16] Swift：Hello World
来源：http://oys.yj202588.top

print("Hello")
来源：http://exj.zhoulong.xyz

[T17] Swift：变量与常量
来源：http://qal.iojbl.cn

var a = 1;  let b = 2
来源：http://gfo.jlsjyb.cn

[T18] Swift：字符串插值
来源：http://tir.xuetiantiany.cn

"值: \(b)"
来源：http://ene.shanyushiyangtech.top

[T19] Swift：可选绑定
来源：http://ugd.ybcxt.top

if let n = opt { print(n) }
来源：http://ziy.shzxlz.cn

[T20] Swift：数组操作
来源：http://qvh.yfazqb.com

var a = [1, 2, 3];  a.append(4)
来源：http://isi.cashguo.top

[T21] Swift：遍历
来源：http://hin.xylfe.cn

for x in a { print(x) }
来源：http://fgo.snrcjt.cn

[T22] Swift：字典
来源：http://rhd.gaohongyu789.top

var d = ["a": 1];  d["b"] = 2
来源：http://rua.bjfxy.top

[T23] Swift：函数
来源：http://ixd.zhaomingkeji.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ijx.andypj.xyz

[T24] Swift：闭包
来源：http://qch.cucudq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kih.tianlin.xyz

[T25] Swift：结构体
来源：http://phe.sxryk.cn

struct P { var x: Int }
来源：http://uuz.xuanzx.com

[T26] Swift：类与重写
来源：http://zmb.tarul.cn

class A: Base { override func f() {} }
来源：http://reh.chenlongwang.top

[T27] Swift：错误处理
来源：http://fqb.chenlongwang.top

do { try f() } catch { print(error) }
来源：http://sfe.haohaochexian.top

[T28] Swift：枚举
来源：http://edk.jlsjyb.cn

enum Color { case red, green }
来源：http://lhp.sjlbkw.cn

[T29] Swift：guard 提前返回
来源：http://uzh.mhx1999.top

guard let x = opt else { return }
来源：http://zgb.gzhubu.top

[T30] Swift：协议
来源：http://qkf.jianghu66.top

protocol Shape { func area() -> Double }
来源：http://ife.xziqi.cn

[T31] Lua：Hello World
来源：http://unc.gzhubu.top

print("Hello")
来源：http://law.yongpay.top

[T32] Lua：局部变量
来源：http://wuk.jinyuanbaomall.cn

local a = 1
来源：http://ahu.hcnkem.com

[T33] Lua：表（数组）
来源：http://cfw.chenzaomai.com

local t = {1, 2, 3};  t[4] = 4
来源：http://dmt.zhongyouzk.top

[T34] Lua：遍历表
来源：http://ont.epnwcf.com

for i, v in ipairs(t) do print(i, v) end
来源：http://frx.meibo888.top

[T35] Lua：字典表
来源：http://ett.yuanzhike.top

local d = { a = 1 };  d.b = 2
来源：http://cxt.chenlongwang.top

[T36] Lua：函数
来源：http://vzn.yuxming.cn

function add(a, b) return a + b end
来源：http://smc.yanxiufei.cn

[T37] Lua：字符串拼接
来源：http://wcw.shangyingyoupin.top

"a" .. "b"
来源：http://aaa.bjfxy.top

[T38] Lua：条件
来源：http://rix.sysykeji.top

if x > 0 then print("正") end
来源：http://hkq.zycfv.cn

[T39] Lua：模式匹配
来源：http://xzx.feifeiyinyue.top

string.find(s, "%d+")
来源：http://tho.fktsv.cn

[T40] Lua：元表
来源：http://muh.andypj.xyz

setmetatable({}, { __index = base })
来源：http://zsy.ydjk.org.cn

[T41] Perl：Hello World
来源：http://cgr.mhx1999.top

print "Hello\n";
来源：http://bqc.yj202588.top

[T42] Perl：变量类型
来源：http://jjw.tarul.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://luy.tianlin.xyz

[T43] Perl：字符串插值
来源：http://cmr.vqdsnc.cn

"值: $a"
来源：http://tbd.9152youxi.cn

[T44] Perl：条件
来源：http://vkq.pengpengdd.cyou

if ($a > 0) { print "正"; }
来源：http://wvg.zycfv.cn

[T45] Perl：数组遍历
来源：http://eoi.smart0.xyz

for my $x (@arr) { print $x; }
来源：http://kdq.fanxiaobao.xyz

[T46] Perl：哈希操作
来源：http://doh.guannengcc.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://aou.jlsjyb.cn

[T47] Perl：正则捕获
来源：http://mjr.yvedp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ayt.sweek.top

[T48] Perl：正则替换
来源：http://tlf.yj20258888.top

$s =~ s/old/new/g;
来源：http://jpd.ehwqpu.com

[T49] Perl：函数
来源：http://xgi.ywan-chungtsiang.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://naw.nwbrower.top

[T50] Perl：逐行读文件
来源：http://hri.epnwcf.com

open my $fh, "<", "a.txt" or die $!;
来源：http://jxz.yuanzhike.top

while (my $line = <$fh>) { print $line; }
来源：http://jvp.mhx1999.top

[T51] Scala：Hello World
来源：http://yej.xingfuxueyuan.xyz

println("Hello")
来源：http://dgp.bjfxy.top

[T52] Scala：变量
来源：http://zej.fehbvm.com

val a = 1;  var b = 2
来源：http://zxb.ydjk.org.cn

[T53] Scala：字符串插值
来源：http://hcv.hcnkem.com

s"值: $b"
来源：http://bsv.mhx1999.top

[T54] Scala：集合映射
来源：http://bpc.shzxlz.cn

List(1, 2, 3).map(_ * 2)
来源：http://vtz.zhijiandao.cn

[T55] Scala：集合过滤
来源：http://rim.dianchejie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://uep.guowangkeji.top

[T56] Scala：样例类
来源：http://efw.guowangkeji.top

case class User(name: String, age: Int)
来源：http://kkq.hongshengwenyu.top

[T57] Scala：模式匹配
来源：http://wgt.ydzc1.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://kkk.yfazqb.com

[T58] Scala：函数定义
来源：http://wun.yfazqb.com

def add(a: Int, b: Int): Int = a + b
来源：http://fxa.yuanzhike.top

[T59] Scala：循环
来源：http://swh.jlsjyb.cn

for (i <- 1 to 10) println(i)
来源：http://mfw.xingfuxueyuan.xyz

[T60] Scala：折叠
来源：http://mjr.chenlongwang.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xio.jiagoushi.top

================================================================================
来源：http://aud.jinqigfzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vhr.smart0.xyz

================================================================================
来源：http://vmn.xinyue.icu

[U01] Py：创建虚拟环境
来源：http://wsl.kuanghao11.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tsx.svipenyu.cn

[U02] Py：导出 / 安装依赖
来源：http://mgu.chenzaomai.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pda.sysykeji.top


<!-- 参考信息 -->