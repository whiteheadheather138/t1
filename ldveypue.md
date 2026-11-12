代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cli.yvedp.cn

[R60] 只看 HTTP 状态码
来源：http://cfa.fktsv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vmk.sysykeji.top

[R61] 磁盘占用
来源：http://yyv.0kj1m.cn

df -h;  du -sh *
来源：http://nfd.yongpay.top

[R62] 找最占空间的文件
来源：http://dhk.xinyue.icu

du -ah . | sort -rh | head -10
来源：http://kli.vehdjk.com

[R63] 内存与进程
来源：http://osp.yongpay.top

free -h;  ps aux | grep nginx
来源：http://hgq.iojbl.cn

[R64] 结束进程
来源：http://spg.ybcxt.top

kill -9 $(pgrep -f app.py)
来源：http://dps.hywenlv.cn

[R65] 查看端口占用
来源：http://wlc.tian-w.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jpe.jqgufenzy.top

[R66] 定时任务
来源：http://kfq.hongshengwenyu.top

crontab -e;  crontab -l
来源：http://knm.yanxiufei.cn

[R67] 生成随机十六进制串
来源：http://kxq.ybcxt.top

openssl rand -hex 16
来源：http://ueu.sxryk.cn

[R68] 计算文件校验值
来源：http://ibs.yfazqb.com

sha256sum a.txt;  md5sum a.txt
来源：http://jwl.jinqigufen.top

[R69] 生成随机密码
来源：http://lvt.aizwys.cn

head -c 16 /dev/urandom | base64
来源：http://yik.havefunace.top

[R70] 时间戳与互转
来源：http://ozj.snrcjt.cn

date +%s;  date -d @1700000000
来源：http://bhr.guowangkeji.top

[R71] 日期格式化
来源：http://kfw.fzhhl.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://yrh.yuxming.cn

[R72] 等待端口就绪
来源：http://xcy.zhiwuduotai.top

until nc -z localhost 3306; do sleep 1; done
来源：http://dtc.dashuyun.cn

[R73] 分割大日志
来源：http://yyk.vehdjk.com

split -l 1000 big.log part_
来源：http://sor.nwbrower.top

[R74] 批量重命名
来源：http://sez.daria6918.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lvo.xingfuxueyuan.xyz

[R75] 导出环境变量
来源：http://kee.hongshengwenyu.top

export PATH="$HOME/bin:$PATH"
来源：http://cyx.ctjpmb.com

[R76] 使用临时文件
来源：http://kbw.ctjpmb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://esg.ppjwa.cn

[R77] 读取用户输入
来源：http://mun.bjfxy.top

read -rp "请输入: " ans
来源：http://xbj.pengpengdd.cyou

[R78] 交互式菜单
来源：http://ayh.9152youxi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cez.ppjwa.cn

[R79] 解析命令行选项
来源：http://alq.mhx1999.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://okx.havefunace.top

[R80] 查看脚本执行耗时
来源：http://vte.vehdjk.com

time ./run.sh
来源：http://tfg.yuanzhike.top

================================================================================
来源：http://hrz.jqgfzy.top

S. C / C++ 专题
来源：http://kip.yangfankeji.com

================================================================================
来源：http://gmh.tianlin.xyz

[S01] C：Hello World
来源：http://erz.zhongyouzk.top

#include <stdio.h>
来源：http://ceh.aizwys.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kzo.hesvh.cn

[S02] C：变量与格式化输出
来源：http://owo.sufxvd.cn

int a = 10; printf("%d\n", a);
来源：http://gfx.fengsongda.top

[S03] C：读入整数
来源：http://cby.sxryk.cn

int x; scanf("%d", &x);
来源：http://dlh.jlsjyb.cn

[S04] C：字符串复制
来源：http://okx.hnqzz.top

char dst[32]; strcpy(dst, "hi");
来源：http://qdv.quarkkingdee.top

[S05] C：字符串长度
来源：http://csy.ybcxt.top

strlen(s)
来源：http://yuq.sufxvd.cn

[S06] C：字符串比较
来源：http://ijm.yongpay.top

strcmp(a, b) == 0
来源：http://qkx.tianlin.xyz

[S07] C：数组遍历求和
来源：http://sal.zdqjudy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vib.fktsv.cn

[S08] C：动态内存分配与释放
来源：http://lbl.haohaochexian.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zoe.jqgufenzy.top

[S09] C：结构体定义与初始化
来源：http://uwo.chenjidiqi.icu

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://afa.sjlbkw.cn

[S10] C：指针与解引用
来源：http://lhu.tianlin.xyz

int *p = &a;  *p = 5;
来源：http://nww.gzhubu.top

[S11] C：逐行读文件
来源：http://oji.ctjpmb.com

FILE *f = fopen("a.txt", "r");
来源：http://ulo.xuanzx.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://mws.tarul.cn

fclose(f);
来源：http://kxu.fanxiaobao.xyz

[S12] C：写文件
来源：http://ujl.chenzaomai.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://plc.hcnkem.com

[S13] C：宏定义
来源：http://apd.316326.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wav.jianghu66.top

[S14] C：枚举
来源：http://hrj.guowangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://qnp.ivvv.top

[S15] C：类型转换
来源：http://mas.ybcxt.top

(double) a / b
来源：http://kpb.havefunace.top

[S16] C：位操作置位
来源：http://nfr.gaohongyu789.top

x |= (1 << 3);
来源：http://bud.0kj1m.cn

[S17] C：安全拼接字符串
来源：http://slc.hongshengwenyu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://slw.yvedp.cn

[S18] C：命令行参数
来源：http://jsv.mhx1999.top

int main(int argc, char **argv)
来源：http://lqm.aibaodan.cn

[S19] C：快速排序
来源：http://bgc.xylfe.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pyu.dashuyun.cn

[S20] C：二分查找
来源：http://qcq.cqqwz.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nrk.hysaishi.cn

[S21] C：字符类别判断
来源：http://xyq.xziqi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hpr.gogol.net.cn

[S22] C：字符串转数字
来源：http://pcf.shangyingyoupin.top

atoi("42");  strtod("3.14", NULL);
来源：http://wen.svipenyu.cn

[S23] C：随机数
来源：http://grh.jinyuanbaomall.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tfd.hesvh.cn

[S24] C：获取本地时间
来源：http://dwj.meibo888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mnf.gotoacloud.top

[S25] C：内存拷贝
来源：http://hvk.daria6918.cn

memcpy(dst, src, n);
来源：http://rkd.guowangkeji.top

[S26] C：内存清零
来源：http://jga.zhaomingkeji.xyz

memset(a, 0, sizeof a);
来源：http://pqq.fktsv.cn

[S27] C：定义常量
来源：http://lwe.jianghu66.top

const double PI = 3.14159;
来源：http://vyb.tanke756.top

[S28] C：静态变量
来源：http://rix.svipenyu.cn

static int counter = 0;
来源：http://lyn.zhoulong.xyz

[S29] C：变参函数
来源：http://zut.316326.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bhy.ydzc1.top

[S30] C：头文件保护
来源：http://fga.nwbrower.top

#ifndef X_H
来源：http://cvr.daria6918.cn

#define X_H
来源：http://ggr.ybcxt.top

#endif
来源：http://wli.cashguo.top

[S31] C++：Hello World
来源：http://xhk.shanyushiyangkeji.top

#include <iostream>
来源：http://xrn.shangyingyoupin.top

int main() { std::cout << "Hello\n"; }
来源：http://aku.jqgfzy.top

[S32] C++：字符串
来源：http://wwo.ybcxt.top

std::string s = "hi";  s += "!";
来源：http://kzr.zhijiandao.cn

[S33] C++：vector 增删
来源：http://otd.yj20258.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://byv.shzxlz.cn

[S34] C++：遍历 vector
来源：http://hdd.fanxiaobao.xyz

for (auto &x : v) { std::cout << x; }
来源：http://mjt.yfazqb.com

[S35] C++：map
来源：http://vyp.haohaochexian.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://elf.ydjk.org.cn

[S36] C++：unordered_map
来源：http://izy.snrcjt.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zqb.cqqwz.cn

[S37] C++：set
来源：http://gqr.yueranfly.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://veg.epnwcf.com

[S38] C++：排序
来源：http://sld.hesvh.cn

std::sort(v.begin(), v.end());
来源：http://ija.zhaomingkeji.xyz

[S39] C++：自定义比较器排序
来源：http://hii.shanyushiyangtech.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dby.svipenyu.cn

[S40] C++：查找元素
来源：http://yfx.tianlin.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ksd.uphjek.com

[S41] C++：类与构造函数
来源：http://nmk.daxiang520.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kiz.yueranfly.top

[S42] C++：继承与虚函数
来源：http://urn.zhaomingkeji.xyz

class B : public Base { public: void f() override {} };
来源：http://qmn.zhiwuduotai.top

[S43] C++：智能指针
来源：http://pit.sufxvd.cn

auto p = std::make_unique<int>(5);
来源：http://xjh.zhiwuduotai.top

[S44] C++：引用传参
来源：http://dao.tianlin.xyz

void inc(int &x) { ++x; }
来源：http://rtg.zhaomingkeji.xyz

[S45] C++：lambda
来源：http://htc.chenzaomai.com

auto add = [](int a, int b) { return a + b; };
来源：http://ydh.uphjek.com

[S46] C++：函数模板
来源：http://umr.wangshuangyany.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pwt.zhixingplan.top

[S47] C++：结构化绑定遍历
来源：http://bop.nwbrower.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dfx.snrcjt.cn

[S48] C++：逐行读文件
来源：http://btp.chenzaomai.com

std::ifstream in("a.txt");  std::string line;
来源：http://myx.ctjpmb.com

while (std::getline(in, line)) { }
来源：http://ngx.pycfn.com

[S49] C++：写文件
来源：http://bnv.jinqigufen.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://aax.wangshuangyany.cn

[S50] C++：格式化数字
来源：http://ptk.jinqigfzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vra.sysykeji.top

[S51] C++：显式类型转换
来源：http://atg.dianchejie.cn

static_cast<double>(a) / b
来源：http://sie.jianghu66.top

[S52] C++：const 与 noexcept
来源：http://uzy.cdnleiting.top

int size() const noexcept { return n_; }
来源：http://yzu.yvedp.cn

[S53] C++：移动语义
来源：http://ijk.yvedp.cn

std::vector<int> w = std::move(v);
来源：http://dgp.hesvh.cn

[S54] C++：异常处理
来源：http://zlp.hfpthk.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hxt.uphjek.com

[S55] C++：结构化绑定
来源：http://xrp.hcnkem.com

auto [a, b] = std::make_pair(1, 2);
来源：http://spm.cashguo.top

[S56] C++：optional
来源：http://avq.redwolf501.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lqh.jiagoushi.top

[S57] C++：编译期常量
来源：http://kka.bbcook.cn

constexpr int N = 10;
来源：http://eeg.ywan-chungtsiang.top

[S58] C++：命名空间
来源：http://cpt.xinyue.icu

namespace ns { int f() { return 1; } }
来源：http://qyo.shangyingyoupin.top

[S59] C++：静态断言
来源：http://cje.feifeiyinyue.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://row.cheryme.top

[S60] C++：遍历并删除元素
来源：http://qbs.bjfxy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gcc.yj202588.top

================================================================================
来源：http://ccb.yangfankeji.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oix.birdmap.top

================================================================================
来源：http://tte.52xcode.cn

[T01] Kotlin：Hello World
来源：http://iiq.xziqi.cn

println("Hello")
来源：http://cfl.fengsongda.top

[T02] Kotlin：变量
来源：http://rwe.dashuyun.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zbb.jyoumei.cn

[T03] Kotlin：字符串模板
来源：http://rbm.daria6918.cn

"值: $b"
来源：http://qsg.fktsv.cn

[T04] Kotlin：空安全
来源：http://oie.kuanghao11.cn

val n: String? = null;  n?.length
来源：http://ape.vqdsnc.cn

[T05] Kotlin：when 表达式
来源：http://fyr.wangshuangyany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lxy.yongpay.top

[T06] Kotlin：集合映射
来源：http://efp.uphjek.com

listOf(1, 2, 3).map { it * 2 }
来源：http://eld.ywan-chungtsiang.top

[T07] Kotlin：集合过滤
来源：http://zaj.zhixingplan.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://tcp.zhongyouzk.top

[T08] Kotlin：数据类
来源：http://lmb.fehbvm.com

data class User(val name: String, val age: Int)
来源：http://fuu.chenzaomai.com

[T09] Kotlin：扩展函数
来源：http://ybn.dashuyun.cn

fun String.exclaim() = this + "!"
来源：http://nlh.yj20258.top

[T10] Kotlin：默认参数
来源：http://jat.zdqjudy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vkz.jyoumei.cn

[T11] Kotlin：协程
来源：http://alm.jinqigfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ttn.hfpthk.cn

[T12] Kotlin：解构声明
来源：http://ahi.daxiang520.top

val (a, b) = Pair(1, 2)
来源：http://gqm.redwolf501.top

[T13] Kotlin：只读 Map
来源：http://uhm.cdnleiting.top

val m = mapOf("a" to 1)
来源：http://qqz.zhiwuduotai.top

[T14] Kotlin：循环
来源：http://cio.ppjwa.cn

for (i in 1..10) println(i)
来源：http://tdu.dashuyun.cn

[T15] Kotlin：接口
来源：http://kwt.shanyushiyangkeji.top

interface Shape { fun area(): Double }
来源：http://xvl.jinqigfzy.top

[T16] Swift：Hello World
来源：http://gtd.zdbjq.cn

print("Hello")
来源：http://pfc.fehbvm.com

[T17] Swift：变量与常量
来源：http://kmo.andypj.xyz

var a = 1;  let b = 2
来源：http://zzc.cqqwz.cn

[T18] Swift：字符串插值
来源：http://hnw.0kj1m.cn

"值: \(b)"
来源：http://fjb.zdbjq.cn

[T19] Swift：可选绑定
来源：http://hfv.gogol.net.cn

if let n = opt { print(n) }
来源：http://mec.shanyushiyangkeji.top

[T20] Swift：数组操作
来源：http://mod.tianlin.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://gjo.fehbvm.com

[T21] Swift：遍历
来源：http://awn.yangfankeji.com

for x in a { print(x) }
来源：http://ggh.ivvv.top

[T22] Swift：字典
来源：http://vgk.316326.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://elf.epnwcf.com

[T23] Swift：函数
来源：http://jxq.tianlin.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zue.sweek.top

[T24] Swift：闭包
来源：http://chq.fanxiaobao.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://ftg.yfazqb.com

[T25] Swift：结构体
来源：http://tja.snrcjt.cn

struct P { var x: Int }
来源：http://lem.vqdsnc.cn

[T26] Swift：类与重写
来源：http://ypx.hfpthk.cn

class A: Base { override func f() {} }
来源：http://mia.zdqjudy.top

[T27] Swift：错误处理
来源：http://pds.hammf.cn

do { try f() } catch { print(error) }
来源：http://vaw.zdbjq.cn

[T28] Swift：枚举
来源：http://tcl.hnxiangtu.top

enum Color { case red, green }
来源：http://avm.jinqigfzy.top

[T29] Swift：guard 提前返回
来源：http://egk.birdmap.top

guard let x = opt else { return }
来源：http://gkn.ehwqpu.com

[T30] Swift：协议
来源：http://afq.bbcook.cn

protocol Shape { func area() -> Double }
来源：http://dyb.jinghuilouyu.cn

[T31] Lua：Hello World
来源：http://pog.svipenyu.cn

print("Hello")
来源：http://nax.havefunace.top

[T32] Lua：局部变量
来源：http://tqp.nwbrower.top

local a = 1
来源：http://vmj.ppjwa.cn

[T33] Lua：表（数组）
来源：http://caz.ydjk.org.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ioj.yj202588.top

[T34] Lua：遍历表
来源：http://tcf.gzhubu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://unz.feifeiyinyue.top

[T35] Lua：字典表
来源：http://vpe.shanyushiyangtech.top

local d = { a = 1 };  d.b = 2
来源：http://hre.cdnleiting.top

[T36] Lua：函数
来源：http://zvn.daria6918.cn

function add(a, b) return a + b end
来源：http://jee.yanxiufei.cn

[T37] Lua：字符串拼接
来源：http://wtz.gaohongyu789.top

"a" .. "b"
来源：http://lwb.quarkkingdee.top

[T38] Lua：条件
来源：http://wtq.snrcjt.cn

if x > 0 then print("正") end
来源：http://xoc.ppjwa.cn

[T39] Lua：模式匹配
来源：http://ruj.fzhhl.top

string.find(s, "%d+")
来源：http://sep.quarkkingdee.top

[T40] Lua：元表
来源：http://gro.jinghuilouyu.cn

setmetatable({}, { __index = base })
来源：http://wkh.zhiwuduotai.top

[T41] Perl：Hello World
来源：http://qnw.jianghu66.top

print "Hello\n";
来源：http://wnm.hongshengwenyu.top

[T42] Perl：变量类型
来源：http://odk.ywan-chungtsiang.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lmc.wangdashe.top

[T43] Perl：字符串插值
来源：http://ikz.zhaomingkeji.xyz

"值: $a"
来源：http://ipc.zhaomingkeji.xyz

[T44] Perl：条件
来源：http://bei.tian-w.cn

if ($a > 0) { print "正"; }
来源：http://gki.ydzc1.top

[T45] Perl：数组遍历
来源：http://jov.fzhhl.top

for my $x (@arr) { print $x; }
来源：http://bjz.smart0.xyz

[T46] Perl：哈希操作
来源：http://imh.zhixingplan.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qrm.guowangkeji.top

[T47] Perl：正则捕获
来源：http://guz.birdmap.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://izm.c1oappe.top

[T48] Perl：正则替换
来源：http://kyx.jinqigfzy.top

$s =~ s/old/new/g;
来源：http://uoe.kuanghao11.cn

[T49] Perl：函数
来源：http://yvv.bjfxy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ihu.jinyuanbaomall.cn

[T50] Perl：逐行读文件
来源：http://jmw.vqdsnc.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://niu.cdnleiting.top

while (my $line = <$fh>) { print $line; }
来源：http://jpx.aibaodan.cn

[T51] Scala：Hello World
来源：http://hct.hywenlv.cn

println("Hello")
来源：http://xzi.svipenyu.cn

[T52] Scala：变量
来源：http://dqx.chenjidiqi.icu

val a = 1;  var b = 2
来源：http://han.nwbrower.top

[T53] Scala：字符串插值
来源：http://fqk.tian-w.cn

s"值: $b"
来源：http://iiu.tian-w.cn

[T54] Scala：集合映射
来源：http://tft.c1oappe.top

List(1, 2, 3).map(_ * 2)
来源：http://jaf.ppjwa.cn

[T55] Scala：集合过滤
来源：http://ffv.jqgufenzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://zjv.jinghuilouyu.cn

[T56] Scala：样例类
来源：http://ocb.ydzc1.top

case class User(name: String, age: Int)
来源：http://dii.yj20258.top

[T57] Scala：模式匹配
来源：http://zri.jqgufenzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://zgy.52xcode.cn

[T58] Scala：函数定义
来源：http://txn.xinyue.icu

def add(a: Int, b: Int): Int = a + b
来源：http://brn.daria6918.cn

[T59] Scala：循环
来源：http://zac.dashuyun.cn

for (i <- 1 to 10) println(i)
来源：http://zsw.zhaomingkeji.xyz

[T60] Scala：折叠
来源：http://krc.jqgufenzy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xnl.yvedp.cn

================================================================================
来源：http://ocn.fzhhl.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bww.yanxiufei.cn

================================================================================
来源：http://zxv.cdnleiting.top


<!-- 参考信息 -->