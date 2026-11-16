代发 wailian999

df -h;  du -sh *
来源：http://yyy.zycfv.cn

[R62] 找最占空间的文件
来源：http://yno.yanxiufei.cn

du -ah . | sort -rh | head -10
来源：http://lpc.birdmap.top

[R63] 内存与进程
来源：http://vsi.ybcxt.top

free -h;  ps aux | grep nginx
来源：http://bjm.zhiwuduotai.top

[R64] 结束进程
来源：http://kst.sweek.top

kill -9 $(pgrep -f app.py)
来源：http://wza.zhoulong.xyz

[R65] 查看端口占用
来源：http://xvb.feifeiyinyue.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.ydzc1.top

[R66] 定时任务
来源：http://exi.hnqzz.top

crontab -e;  crontab -l
来源：http://rfz.ydjk.org.cn

[R67] 生成随机十六进制串
来源：http://nuh.tian-w.cn

openssl rand -hex 16
来源：http://dbr.zhixingplan.top

[R68] 计算文件校验值
来源：http://cxo.xuetiantiany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ozj.fanxiaobao.xyz

[R69] 生成随机密码
来源：http://xyp.vehdjk.com

head -c 16 /dev/urandom | base64
来源：http://yqz.zhoulong.xyz

[R70] 时间戳与互转
来源：http://pfr.ydjk.org.cn

date +%s;  date -d @1700000000
来源：http://udl.hongshengwenyu.top

[R71] 日期格式化
来源：http://lge.dashuyun.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fku.ywan-chungtsiang.top

[R72] 等待端口就绪
来源：http://zmx.andypj.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://vjs.pengpengdd.cyou

[R73] 分割大日志
来源：http://uop.zhaomingkeji.xyz

split -l 1000 big.log part_
来源：http://otv.iojbl.cn

[R74] 批量重命名
来源：http://hfy.pengpengdd.cyou

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xse.ivvv.top

[R75] 导出环境变量
来源：http://zwj.yangfankeji.com

export PATH="$HOME/bin:$PATH"
来源：http://kjj.ehwqpu.com

[R76] 使用临时文件
来源：http://ihw.cdnleiting.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ccc.ywan-chungtsiang.top

[R77] 读取用户输入
来源：http://fce.wangdashe.top

read -rp "请输入: " ans
来源：http://fkq.havefunace.top

[R78] 交互式菜单
来源：http://ocd.vehdjk.com

select opt in a b c; do echo "$opt"; break; done
来源：http://dra.zhijiandao.cn

[R79] 解析命令行选项
来源：http://zpo.bjfxy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jyd.epnwcf.com

[R80] 查看脚本执行耗时
来源：http://xor.0kj1m.cn

time ./run.sh
来源：http://vfg.jlsjyb.cn

================================================================================
来源：http://hrh.jiagoushi.top

S. C / C++ 专题
来源：http://kzi.zhiwuduotai.top

================================================================================
来源：http://hiz.redwolf501.top

[S01] C：Hello World
来源：http://wet.svipenyu.cn

#include <stdio.h>
来源：http://urn.dianchejie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://iow.xinyue.icu

[S02] C：变量与格式化输出
来源：http://gfu.hfpthk.cn

int a = 10; printf("%d\n", a);
来源：http://lza.chenzaomai.com

[S03] C：读入整数
来源：http://wvl.svipenyu.cn

int x; scanf("%d", &x);
来源：http://ryp.jianghu66.top

[S04] C：字符串复制
来源：http://ksx.nwbrower.top

char dst[32]; strcpy(dst, "hi");
来源：http://qhn.chenlongwang.top

[S05] C：字符串长度
来源：http://nox.birdmap.top

strlen(s)
来源：http://lzd.wangshuangyany.cn

[S06] C：字符串比较
来源：http://wql.chenjidiqi.icu

strcmp(a, b) == 0
来源：http://qek.hywenlv.cn

[S07] C：数组遍历求和
来源：http://hel.yongpay.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fiz.chenzaomai.com

[S08] C：动态内存分配与释放
来源：http://kzb.yueranfly.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nho.c1oappe.top

[S09] C：结构体定义与初始化
来源：http://unn.zhoulong.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kke.tanke756.top

[S10] C：指针与解引用
来源：http://okz.dianchejie.cn

int *p = &a;  *p = 5;
来源：http://ugu.jinqigufen.top

[S11] C：逐行读文件
来源：http://hmr.hysaishi.cn

FILE *f = fopen("a.txt", "r");
来源：http://owl.aibaodan.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nrk.guowangkeji.top

fclose(f);
来源：http://yuz.dashuyun.cn

[S12] C：写文件
来源：http://jwg.shuidangran.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://utd.hesvh.cn

[S13] C：宏定义
来源：http://bql.cheryme.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mky.hcnkem.com

[S14] C：枚举
来源：http://snv.jyoumei.cn

enum Color { RED, GREEN, BLUE };
来源：http://vxn.ivvv.top

[S15] C：类型转换
来源：http://wym.andypj.xyz

(double) a / b
来源：http://jnc.sjlbkw.cn

[S16] C：位操作置位
来源：http://fzj.jqgufenzy.top

x |= (1 << 3);
来源：http://dgt.zhongyouzk.top

[S17] C：安全拼接字符串
来源：http://xno.zhongyouzk.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hih.birdmap.top

[S18] C：命令行参数
来源：http://cuo.jinqigfzy.top

int main(int argc, char **argv)
来源：http://bhb.zycfv.cn

[S19] C：快速排序
来源：http://ygc.hongshengwenyu.top

qsort(a, n, sizeof(int), cmp);
来源：http://tmk.shuidangran.top

[S20] C：二分查找
来源：http://irk.yvedp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qwm.aizwys.cn

[S21] C：字符类别判断
来源：http://prm.epnwcf.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rnv.quarkkingdee.top

[S22] C：字符串转数字
来源：http://jqe.yueranfly.top

atoi("42");  strtod("3.14", NULL);
来源：http://eqj.quarkkingdee.top

[S23] C：随机数
来源：http://dpf.tianlin.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://vce.uphjek.com

[S24] C：获取本地时间
来源：http://zcp.hongshengwenyu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cfo.fktsv.cn

[S25] C：内存拷贝
来源：http://qij.gotoacloud.top

memcpy(dst, src, n);
来源：http://mlj.c1oappe.top

[S26] C：内存清零
来源：http://qqu.yvedp.cn

memset(a, 0, sizeof a);
来源：http://alu.snrcjt.cn

[S27] C：定义常量
来源：http://onj.9152youxi.cn

const double PI = 3.14159;
来源：http://jcz.cqqwz.cn

[S28] C：静态变量
来源：http://dxu.yfazqb.com

static int counter = 0;
来源：http://rko.meibo888.top

[S29] C：变参函数
来源：http://opt.cqqwz.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://omr.hongshengwenyu.top

[S30] C：头文件保护
来源：http://wai.tianlin.xyz

#ifndef X_H
来源：http://eyd.bjfxy.top

#define X_H
来源：http://nmr.hcnkem.com

#endif
来源：http://tgw.shzxlz.cn

[S31] C++：Hello World
来源：http://xke.yuxming.cn

#include <iostream>
来源：http://hjw.xuetiantiany.cn

int main() { std::cout << "Hello\n"; }
来源：http://fph.vehdjk.com

[S32] C++：字符串
来源：http://kir.xziqi.cn

std::string s = "hi";  s += "!";
来源：http://hci.hysaishi.cn

[S33] C++：vector 增删
来源：http://ocb.zhijiandao.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jsa.yj20258888.top

[S34] C++：遍历 vector
来源：http://axq.zhaomingkeji.xyz

for (auto &x : v) { std::cout << x; }
来源：http://ewm.iojbl.cn

[S35] C++：map
来源：http://pmj.wangdashe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mug.shangyingyoupin.top

[S36] C++：unordered_map
来源：http://wwd.shangyingyoupin.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ghk.chenzaomai.com

[S37] C++：set
来源：http://esz.meibo888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zdi.c1oappe.top

[S38] C++：排序
来源：http://nlk.jlsjyb.cn

std::sort(v.begin(), v.end());
来源：http://lay.gogol.net.cn

[S39] C++：自定义比较器排序
来源：http://sty.ydjk.org.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://udp.hesvh.cn

[S40] C++：查找元素
来源：http://lmg.fengsongda.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qkz.c1oappe.top

[S41] C++：类与构造函数
来源：http://uje.fktsv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oso.xylfe.cn

[S42] C++：继承与虚函数
来源：http://ffz.mhx1999.top

class B : public Base { public: void f() override {} };
来源：http://ruw.cashguo.top

[S43] C++：智能指针
来源：http://ejg.chenjidiqi.icu

auto p = std::make_unique<int>(5);
来源：http://dzx.chenjidiqi.icu

[S44] C++：引用传参
来源：http://phr.zhijiandao.cn

void inc(int &x) { ++x; }
来源：http://ejy.uphjek.com

[S45] C++：lambda
来源：http://mce.xylfe.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xhq.fktsv.cn

[S46] C++：函数模板
来源：http://bfe.ywan-chungtsiang.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cqm.dashuyun.cn

[S47] C++：结构化绑定遍历
来源：http://jtw.cashguo.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qmq.snrcjt.cn

[S48] C++：逐行读文件
来源：http://ipx.tian-w.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zvc.ybcxt.top

while (std::getline(in, line)) { }
来源：http://jpg.gotoacloud.top

[S49] C++：写文件
来源：http://dzx.0kj1m.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dgz.haohaochexian.top

[S50] C++：格式化数字
来源：http://ido.jyoumei.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ilx.vqdsnc.cn

[S51] C++：显式类型转换
来源：http://vlj.hammf.cn

static_cast<double>(a) / b
来源：http://reo.hesvh.cn

[S52] C++：const 与 noexcept
来源：http://bts.iojbl.cn

int size() const noexcept { return n_; }
来源：http://qmr.jqgufenzy.top

[S53] C++：移动语义
来源：http://aee.316326.xyz

std::vector<int> w = std::move(v);
来源：http://dvu.gzhubu.top

[S54] C++：异常处理
来源：http://bmi.hcnkem.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mrh.xinyue.icu

[S55] C++：结构化绑定
来源：http://aed.hammf.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tzv.hongshengwenyu.top

[S56] C++：optional
来源：http://iuy.haohaochexian.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pyd.dashuyun.cn

[S57] C++：编译期常量
来源：http://ywh.jinqigufen.top

constexpr int N = 10;
来源：http://mbv.jinghuilouyu.cn

[S58] C++：命名空间
来源：http://iox.jinqigufen.top

namespace ns { int f() { return 1; } }
来源：http://brp.shanyushiyangtech.top

[S59] C++：静态断言
来源：http://vao.yvedp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sfw.vqdsnc.cn

[S60] C++：遍历并删除元素
来源：http://omq.cqqwz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dhq.yangfankeji.com

================================================================================
来源：http://nbp.hysaishi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rfn.9152youxi.cn

================================================================================
来源：http://cde.jinqigufen.top

[T01] Kotlin：Hello World
来源：http://kyl.ydzc1.top

println("Hello")
来源：http://jjq.yueranfly.top

[T02] Kotlin：变量
来源：http://zvm.tianlin.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://txw.zhiwuduotai.top

[T03] Kotlin：字符串模板
来源：http://jdm.hammf.cn

"值: $b"
来源：http://say.zhongyouzk.top

[T04] Kotlin：空安全
来源：http://jhy.zycfv.cn

val n: String? = null;  n?.length
来源：http://fdg.tianlin.xyz

[T05] Kotlin：when 表达式
来源：http://mhm.zdbjq.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qpf.quarkkingdee.top

[T06] Kotlin：集合映射
来源：http://yes.jlsjyb.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xcg.dashuyun.cn

[T07] Kotlin：集合过滤
来源：http://xsl.zycfv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gli.zdbjq.cn

[T08] Kotlin：数据类
来源：http://arv.jyoumei.cn

data class User(val name: String, val age: Int)
来源：http://jnm.svipenyu.cn

[T09] Kotlin：扩展函数
来源：http://nno.cucudq.cn

fun String.exclaim() = this + "!"
来源：http://uex.ctjpmb.com

[T10] Kotlin：默认参数
来源：http://nwu.wangdashe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://dja.yj202588.top

[T11] Kotlin：协程
来源：http://ata.zycfv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://agq.kuanghao11.cn

[T12] Kotlin：解构声明
来源：http://kgg.yj202588.top

val (a, b) = Pair(1, 2)
来源：http://xso.ybcxt.top

[T13] Kotlin：只读 Map
来源：http://sqd.wangshuangyany.cn

val m = mapOf("a" to 1)
来源：http://ybo.zhaomingkeji.xyz

[T14] Kotlin：循环
来源：http://kbc.haohaochexian.top

for (i in 1..10) println(i)
来源：http://wci.hnqzz.top

[T15] Kotlin：接口
来源：http://knl.haohaochexian.top

interface Shape { fun area(): Double }
来源：http://ohv.c1oappe.top

[T16] Swift：Hello World
来源：http://nvg.shuidangran.top

print("Hello")
来源：http://jdx.redwolf501.top

[T17] Swift：变量与常量
来源：http://lqg.zhoulong.xyz

var a = 1;  let b = 2
来源：http://sqr.zhongyouzk.top

[T18] Swift：字符串插值
来源：http://kbi.fanxiaobao.xyz

"值: \(b)"
来源：http://phd.jyoumei.cn

[T19] Swift：可选绑定
来源：http://kyq.feifeiyinyue.top

if let n = opt { print(n) }
来源：http://cph.jianghu66.top

[T20] Swift：数组操作
来源：http://qid.fanxiaobao.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://ayb.jqgufenzy.top

[T21] Swift：遍历
来源：http://jih.epnwcf.com

for x in a { print(x) }
来源：http://meu.316326.xyz

[T22] Swift：字典
来源：http://sed.cheryme.top

var d = ["a": 1];  d["b"] = 2
来源：http://hgf.jyoumei.cn

[T23] Swift：函数
来源：http://wgs.sufxvd.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xrg.ppjwa.cn

[T24] Swift：闭包
来源：http://nbz.shzxlz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bcl.yj20258.top

[T25] Swift：结构体
来源：http://tfi.hysaishi.cn

struct P { var x: Int }
来源：http://usf.xylfe.cn

[T26] Swift：类与重写
来源：http://tem.pycfn.com

class A: Base { override func f() {} }
来源：http://bnm.sweek.top

[T27] Swift：错误处理
来源：http://fmx.fengsongda.top

do { try f() } catch { print(error) }
来源：http://ztm.xuetiantiany.cn

[T28] Swift：枚举
来源：http://csa.dianchejie.cn

enum Color { case red, green }
来源：http://jez.sufxvd.cn

[T29] Swift：guard 提前返回
来源：http://vjr.jyoumei.cn

guard let x = opt else { return }
来源：http://mfq.iojbl.cn

[T30] Swift：协议
来源：http://nbf.mhx1999.top

protocol Shape { func area() -> Double }
来源：http://bzw.sysykeji.top

[T31] Lua：Hello World
来源：http://pzr.bbcook.cn

print("Hello")
来源：http://neh.shanyushiyangtech.top

[T32] Lua：局部变量
来源：http://adj.zhijiandao.cn

local a = 1
来源：http://ecz.guowangkeji.top

[T33] Lua：表（数组）
来源：http://iud.cashguo.top

local t = {1, 2, 3};  t[4] = 4
来源：http://drv.0kj1m.cn

[T34] Lua：遍历表
来源：http://njz.0kj1m.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zte.jinqigufen.top

[T35] Lua：字典表
来源：http://ewq.bjfxy.top

local d = { a = 1 };  d.b = 2
来源：http://pvp.yuanzhike.top

[T36] Lua：函数
来源：http://ckh.haohaochexian.top

function add(a, b) return a + b end
来源：http://ydz.sufxvd.cn

[T37] Lua：字符串拼接
来源：http://qmo.ydzc1.top

"a" .. "b"
来源：http://nbe.hnqzz.top

[T38] Lua：条件
来源：http://jyu.hcnkem.com

if x > 0 then print("正") end
来源：http://xck.fktsv.cn

[T39] Lua：模式匹配
来源：http://wjb.guannengcc.top

string.find(s, "%d+")
来源：http://omi.redwolf501.top

[T40] Lua：元表
来源：http://kai.jiagoushi.top

setmetatable({}, { __index = base })
来源：http://roq.aizwys.cn

[T41] Perl：Hello World
来源：http://oru.snrcjt.cn

print "Hello\n";
来源：http://uyz.ehwqpu.com

[T42] Perl：变量类型
来源：http://qli.redwolf501.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://shy.chenlongwang.top

[T43] Perl：字符串插值
来源：http://rzy.zdqjudy.top

"值: $a"
来源：http://jow.pengpengdd.cyou

[T44] Perl：条件
来源：http://tiv.jqgufenzy.top

if ($a > 0) { print "正"; }
来源：http://gbl.9152youxi.cn

[T45] Perl：数组遍历
来源：http://eth.pycfn.com

for my $x (@arr) { print $x; }
来源：http://ogr.hnqzz.top

[T46] Perl：哈希操作
来源：http://lwt.yuanzhike.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pqb.cdnleiting.top

[T47] Perl：正则捕获
来源：http://lqr.tanke756.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://lwu.hfpthk.cn

[T48] Perl：正则替换
来源：http://hsy.redwolf501.top

$s =~ s/old/new/g;
来源：http://hxk.mhx1999.top

[T49] Perl：函数
来源：http://gys.xingfuxueyuan.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jvu.meibo888.top

[T50] Perl：逐行读文件
来源：http://kzr.kuanghao11.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bhz.zhijiandao.cn

while (my $line = <$fh>) { print $line; }
来源：http://uyn.hywenlv.cn

[T51] Scala：Hello World
来源：http://tfp.jinyuanbaomall.cn

println("Hello")
来源：http://oza.316326.xyz

[T52] Scala：变量
来源：http://dig.sysykeji.top

val a = 1;  var b = 2
来源：http://gvc.yongpay.top

[T53] Scala：字符串插值
来源：http://jgp.tanke756.top

s"值: $b"
来源：http://ulg.ywan-chungtsiang.top

[T54] Scala：集合映射
来源：http://tkg.daxiang520.top

List(1, 2, 3).map(_ * 2)
来源：http://yzd.ydjk.org.cn

[T55] Scala：集合过滤
来源：http://foy.hammf.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vuq.sjlbkw.cn

[T56] Scala：样例类
来源：http://iqz.zhiwuduotai.top

case class User(name: String, age: Int)
来源：http://qgk.wangdashe.top

[T57] Scala：模式匹配
来源：http://lom.jinqigufen.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://unf.xziqi.cn

[T58] Scala：函数定义
来源：http://tpb.zhaomingkeji.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://alr.kuanghao11.cn

[T59] Scala：循环
来源：http://sos.shangyingyoupin.top

for (i <- 1 to 10) println(i)
来源：http://mmn.shanyushiyangkeji.top

[T60] Scala：折叠
来源：http://fuv.ppjwa.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hyn.cheryme.top

================================================================================
来源：http://hcr.cashguo.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gvk.haohaochexian.top

================================================================================
来源：http://ujy.ydzc1.top

[U01] Py：创建虚拟环境
来源：http://iez.fehbvm.com

python -m venv .venv && source .venv/bin/activate
来源：http://ozs.shangyingyoupin.top

[U02] Py：导出 / 安装依赖
来源：http://mny.yfazqb.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jdn.sweek.top


<!-- 参考信息 -->