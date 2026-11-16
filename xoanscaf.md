代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rtl.ydzc1.top

[R60] 只看 HTTP 状态码
来源：http://oqn.jqgufenzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nne.sxryk.cn

[R61] 磁盘占用
来源：http://dxb.hammf.cn

df -h;  du -sh *
来源：http://ktz.hnqzz.top

[R62] 找最占空间的文件
来源：http://xai.cashguo.top

du -ah . | sort -rh | head -10
来源：http://eea.dashuyun.cn

[R63] 内存与进程
来源：http://rsz.daxiang520.top

free -h;  ps aux | grep nginx
来源：http://lul.guowangkeji.top

[R64] 结束进程
来源：http://lyj.vqdsnc.cn

kill -9 $(pgrep -f app.py)
来源：http://qmo.chenzaomai.com

[R65] 查看端口占用
来源：http://vky.tianlin.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yio.hesvh.cn

[R66] 定时任务
来源：http://qvg.sjlbkw.cn

crontab -e;  crontab -l
来源：http://cbo.birdmap.top

[R67] 生成随机十六进制串
来源：http://bfv.birdmap.top

openssl rand -hex 16
来源：http://hfk.shangyingyoupin.top

[R68] 计算文件校验值
来源：http://tmr.gotoacloud.top

sha256sum a.txt;  md5sum a.txt
来源：http://vts.zycfv.cn

[R69] 生成随机密码
来源：http://ysh.epnwcf.com

head -c 16 /dev/urandom | base64
来源：http://fjw.c1oappe.top

[R70] 时间戳与互转
来源：http://gqx.meibo888.top

date +%s;  date -d @1700000000
来源：http://eir.yuanzhike.top

[R71] 日期格式化
来源：http://cqx.9152youxi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kwd.hesvh.cn

[R72] 等待端口就绪
来源：http://rcj.dashuyun.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://frl.c1oappe.top

[R73] 分割大日志
来源：http://qmw.xingfuxueyuan.xyz

split -l 1000 big.log part_
来源：http://dsw.zhixingplan.top

[R74] 批量重命名
来源：http://qma.guannengcc.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tlk.sxryk.cn

[R75] 导出环境变量
来源：http://ytd.c1oappe.top

export PATH="$HOME/bin:$PATH"
来源：http://ycr.ppjwa.cn

[R76] 使用临时文件
来源：http://tvi.zhoulong.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vwa.jqgufenzy.top

[R77] 读取用户输入
来源：http://trm.hnxiangtu.top

read -rp "请输入: " ans
来源：http://qug.sxryk.cn

[R78] 交互式菜单
来源：http://rne.jqgfzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://sqt.jiagoushi.top

[R79] 解析命令行选项
来源：http://qed.birdmap.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eyd.zhongyouzk.top

[R80] 查看脚本执行耗时
来源：http://kuh.xingfuxueyuan.xyz

time ./run.sh
来源：http://mkt.fzhhl.top

================================================================================
来源：http://qfp.hnqzz.top

S. C / C++ 专题
来源：http://rez.dashuyun.cn

================================================================================
来源：http://pgq.hcnkem.com

[S01] C：Hello World
来源：http://twq.gaohongyu789.top

#include <stdio.h>
来源：http://pow.c1oappe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://iqk.hcnkem.com

[S02] C：变量与格式化输出
来源：http://mif.yvedp.cn

int a = 10; printf("%d\n", a);
来源：http://szk.tarul.cn

[S03] C：读入整数
来源：http://zeh.feifeiyinyue.top

int x; scanf("%d", &x);
来源：http://itt.hnqzz.top

[S04] C：字符串复制
来源：http://hyg.vqdsnc.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kex.cheryme.top

[S05] C：字符串长度
来源：http://gaf.jianghu66.top

strlen(s)
来源：http://uoi.ctjpmb.com

[S06] C：字符串比较
来源：http://vyb.xylfe.cn

strcmp(a, b) == 0
来源：http://yyy.zhiwuduotai.top

[S07] C：数组遍历求和
来源：http://uhd.zhengqikj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://prf.ydjk.org.cn

[S08] C：动态内存分配与释放
来源：http://ohy.sxryk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rdd.dianchejie.cn

[S09] C：结构体定义与初始化
来源：http://idt.fanxiaobao.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hyq.ctjpmb.com

[S10] C：指针与解引用
来源：http://gkx.316326.xyz

int *p = &a;  *p = 5;
来源：http://vzs.cheryme.top

[S11] C：逐行读文件
来源：http://imb.cashguo.top

FILE *f = fopen("a.txt", "r");
来源：http://gtp.shanyushiyangkeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://bxu.meibo888.top

fclose(f);
来源：http://fnt.xuetiantiany.cn

[S12] C：写文件
来源：http://cbj.smart0.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gqe.haohaochexian.top

[S13] C：宏定义
来源：http://tcr.meibo888.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hdo.xylfe.cn

[S14] C：枚举
来源：http://mcu.fktsv.cn

enum Color { RED, GREEN, BLUE };
来源：http://fhv.tian-w.cn

[S15] C：类型转换
来源：http://ftg.ydjk.org.cn

(double) a / b
来源：http://bcm.bjfxy.top

[S16] C：位操作置位
来源：http://toq.nanxinkj.top

x |= (1 << 3);
来源：http://gxl.yj20258888.top

[S17] C：安全拼接字符串
来源：http://kws.zdbjq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rgi.dianchejie.cn

[S18] C：命令行参数
来源：http://upr.yangfankeji.com

int main(int argc, char **argv)
来源：http://ngq.fktsv.cn

[S19] C：快速排序
来源：http://mtf.ppjwa.cn

qsort(a, n, sizeof(int), cmp);
来源：http://exp.ivvv.top

[S20] C：二分查找
来源：http://ilo.xziqi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yxn.wangshuangyany.cn

[S21] C：字符类别判断
来源：http://kpa.jinqigufen.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kul.jyoumei.cn

[S22] C：字符串转数字
来源：http://gxs.yanxiufei.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ige.0kj1m.cn

[S23] C：随机数
来源：http://icj.xziqi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vyn.hnxiangtu.top

[S24] C：获取本地时间
来源：http://qgt.chenzaomai.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xet.shuidangran.top

[S25] C：内存拷贝
来源：http://ila.jinghuilouyu.cn

memcpy(dst, src, n);
来源：http://qor.52xcode.cn

[S26] C：内存清零
来源：http://mec.hammf.cn

memset(a, 0, sizeof a);
来源：http://fsf.yfazqb.com

[S27] C：定义常量
来源：http://yqm.0kj1m.cn

const double PI = 3.14159;
来源：http://khf.nanxuanxn.top

[S28] C：静态变量
来源：http://jzx.chenjidiqi.icu

static int counter = 0;
来源：http://bpj.yvedp.cn

[S29] C：变参函数
来源：http://fcq.sweek.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://veg.52xcode.cn

[S30] C：头文件保护
来源：http://uuy.yongpay.top

#ifndef X_H
来源：http://xmg.bbcook.cn

#define X_H
来源：http://wjo.iojbl.cn

#endif
来源：http://smh.sweek.top

[S31] C++：Hello World
来源：http://kpe.svipenyu.cn

#include <iostream>
来源：http://vbw.yj202588.top

int main() { std::cout << "Hello\n"; }
来源：http://paz.ydjk.org.cn

[S32] C++：字符串
来源：http://ofe.yongpay.top

std::string s = "hi";  s += "!";
来源：http://xrl.sufxvd.cn

[S33] C++：vector 增删
来源：http://ixu.gotoacloud.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dlr.jqgufenzy.top

[S34] C++：遍历 vector
来源：http://hrb.52xcode.cn

for (auto &x : v) { std::cout << x; }
来源：http://mqw.ehwqpu.com

[S35] C++：map
来源：http://bku.meibo888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tfc.wangdashe.top

[S36] C++：unordered_map
来源：http://ydh.xziqi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hqe.zhiwuduotai.top

[S37] C++：set
来源：http://zug.vqdsnc.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://atp.gzhubu.top

[S38] C++：排序
来源：http://tpb.yj20258888.top

std::sort(v.begin(), v.end());
来源：http://akw.316326.xyz

[S39] C++：自定义比较器排序
来源：http://rpu.yj20258888.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qtw.tianlin.xyz

[S40] C++：查找元素
来源：http://nnk.zhongyouzk.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gym.redwolf501.top

[S41] C++：类与构造函数
来源：http://eyu.chenzaomai.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://eia.zhiwuduotai.top

[S42] C++：继承与虚函数
来源：http://nii.nwbrower.top

class B : public Base { public: void f() override {} };
来源：http://apb.hesvh.cn

[S43] C++：智能指针
来源：http://pbn.zhixingplan.top

auto p = std::make_unique<int>(5);
来源：http://kap.cdnleiting.top

[S44] C++：引用传参
来源：http://hvp.yuanzhike.top

void inc(int &x) { ++x; }
来源：http://lcm.fehbvm.com

[S45] C++：lambda
来源：http://sgj.jinghuilouyu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://trh.jinqigfzy.top

[S46] C++：函数模板
来源：http://esm.chenjidiqi.icu

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dbh.yfazqb.com

[S47] C++：结构化绑定遍历
来源：http://ybl.snrcjt.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://aql.zhijiandao.cn

[S48] C++：逐行读文件
来源：http://vcb.wangshuangyany.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kll.meibo888.top

while (std::getline(in, line)) { }
来源：http://asi.sufxvd.cn

[S49] C++：写文件
来源：http://pyc.svipenyu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uaa.gaohongyu789.top

[S50] C++：格式化数字
来源：http://qpr.hysaishi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bza.yanxiufei.cn

[S51] C++：显式类型转换
来源：http://wvw.ydzc1.top

static_cast<double>(a) / b
来源：http://qlx.jyoumei.cn

[S52] C++：const 与 noexcept
来源：http://ncm.0kj1m.cn

int size() const noexcept { return n_; }
来源：http://tcn.yuanzhike.top

[S53] C++：移动语义
来源：http://qdx.vqdsnc.cn

std::vector<int> w = std::move(v);
来源：http://ejo.jyoumei.cn

[S54] C++：异常处理
来源：http://dsj.hfpthk.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vir.tarul.cn

[S55] C++：结构化绑定
来源：http://acl.guannengcc.top

auto [a, b] = std::make_pair(1, 2);
来源：http://mry.ybcxt.top

[S56] C++：optional
来源：http://ndr.jqgfzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dyj.kuanghao11.cn

[S57] C++：编译期常量
来源：http://ymo.yj20258.top

constexpr int N = 10;
来源：http://igw.sysykeji.top

[S58] C++：命名空间
来源：http://mza.zhoulong.xyz

namespace ns { int f() { return 1; } }
来源：http://yze.xuanzx.com

[S59] C++：静态断言
来源：http://ayv.svipenyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hcn.fzhhl.top

[S60] C++：遍历并删除元素
来源：http://agj.shuidangran.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qox.redwolf501.top

================================================================================
来源：http://bty.aibaodan.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mpc.uphjek.com

================================================================================
来源：http://gni.yongpay.top

[T01] Kotlin：Hello World
来源：http://xvt.hnxiangtu.top

println("Hello")
来源：http://pws.hywenlv.cn

[T02] Kotlin：变量
来源：http://brb.zycfv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hhl.pycfn.com

[T03] Kotlin：字符串模板
来源：http://rxb.sxryk.cn

"值: $b"
来源：http://uut.jlsjyb.cn

[T04] Kotlin：空安全
来源：http://prt.daria6918.cn

val n: String? = null;  n?.length
来源：http://cuu.yangfankeji.com

[T05] Kotlin：when 表达式
来源：http://twz.zdqjudy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://aun.cucudq.cn

[T06] Kotlin：集合映射
来源：http://pxp.sufxvd.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jmu.shzxlz.cn

[T07] Kotlin：集合过滤
来源：http://ljr.havefunace.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://hey.andypj.xyz

[T08] Kotlin：数据类
来源：http://ijm.shanyushiyangtech.top

data class User(val name: String, val age: Int)
来源：http://vyq.yj20258888.top

[T09] Kotlin：扩展函数
来源：http://zgk.0kj1m.cn

fun String.exclaim() = this + "!"
来源：http://czm.jqgfzy.top

[T10] Kotlin：默认参数
来源：http://hzp.snrcjt.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hzu.shzxlz.cn

[T11] Kotlin：协程
来源：http://hag.fktsv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://tqm.cqqwz.cn

[T12] Kotlin：解构声明
来源：http://aec.hongshengwenyu.top

val (a, b) = Pair(1, 2)
来源：http://hzh.zhijiandao.cn

[T13] Kotlin：只读 Map
来源：http://fdk.quarkkingdee.top

val m = mapOf("a" to 1)
来源：http://rix.zhongyouzk.top

[T14] Kotlin：循环
来源：http://dca.hywenlv.cn

for (i in 1..10) println(i)
来源：http://lmb.yj20258.top

[T15] Kotlin：接口
来源：http://irf.gogol.net.cn

interface Shape { fun area(): Double }
来源：http://gnh.shuidangran.top

[T16] Swift：Hello World
来源：http://pdb.gogol.net.cn

print("Hello")
来源：http://qsg.fktsv.cn

[T17] Swift：变量与常量
来源：http://ieu.kuanghao11.cn

var a = 1;  let b = 2
来源：http://gyo.xuetiantiany.cn

[T18] Swift：字符串插值
来源：http://ian.uphjek.com

"值: \(b)"
来源：http://xje.aibaodan.cn

[T19] Swift：可选绑定
来源：http://ahf.iojbl.cn

if let n = opt { print(n) }
来源：http://fqs.guowangkeji.top

[T20] Swift：数组操作
来源：http://jbw.fzhhl.top

var a = [1, 2, 3];  a.append(4)
来源：http://ozj.sxryk.cn

[T21] Swift：遍历
来源：http://sll.xinyue.icu

for x in a { print(x) }
来源：http://pyr.bjfxy.top

[T22] Swift：字典
来源：http://yal.hnqzz.top

var d = ["a": 1];  d["b"] = 2
来源：http://bkd.hnqzz.top

[T23] Swift：函数
来源：http://cjg.jinghuilouyu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nit.cheryme.top

[T24] Swift：闭包
来源：http://jha.mhx1999.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://cbd.ybcxt.top

[T25] Swift：结构体
来源：http://ogk.cdnleiting.top

struct P { var x: Int }
来源：http://ykm.andypj.xyz

[T26] Swift：类与重写
来源：http://vqq.bjfxy.top

class A: Base { override func f() {} }
来源：http://xxl.shzxlz.cn

[T27] Swift：错误处理
来源：http://ons.xylfe.cn

do { try f() } catch { print(error) }
来源：http://nvh.gaohongyu789.top

[T28] Swift：枚举
来源：http://lxl.cdnleiting.top

enum Color { case red, green }
来源：http://yjk.tarul.cn

[T29] Swift：guard 提前返回
来源：http://zrq.zhongyouzk.top

guard let x = opt else { return }
来源：http://pzs.wangshuangyany.cn

[T30] Swift：协议
来源：http://rrm.ybcxt.top

protocol Shape { func area() -> Double }
来源：http://bku.jinghuilouyu.cn

[T31] Lua：Hello World
来源：http://vfn.yongpay.top

print("Hello")
来源：http://xbm.316326.xyz

[T32] Lua：局部变量
来源：http://yrz.jlsjyb.cn

local a = 1
来源：http://cdc.cashguo.top

[T33] Lua：表（数组）
来源：http://jay.hywenlv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vqp.gzhubu.top

[T34] Lua：遍历表
来源：http://kek.kuanghao11.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pwd.jlsjyb.cn

[T35] Lua：字典表
来源：http://dhi.feifeiyinyue.top

local d = { a = 1 };  d.b = 2
来源：http://oco.hfpthk.cn

[T36] Lua：函数
来源：http://bwd.fktsv.cn

function add(a, b) return a + b end
来源：http://ueu.ivvv.top

[T37] Lua：字符串拼接
来源：http://ckb.zdqjudy.top

"a" .. "b"
来源：http://ydx.andypj.xyz

[T38] Lua：条件
来源：http://xak.nwbrower.top

if x > 0 then print("正") end
来源：http://uxd.xinyue.icu

[T39] Lua：模式匹配
来源：http://gcs.zhongyouzk.top

string.find(s, "%d+")
来源：http://ygr.daria6918.cn

[T40] Lua：元表
来源：http://yyb.havefunace.top

setmetatable({}, { __index = base })
来源：http://abl.zhixingplan.top

[T41] Perl：Hello World
来源：http://tra.hongshengwenyu.top

print "Hello\n";
来源：http://gef.mhx1999.top

[T42] Perl：变量类型
来源：http://wbu.chenzaomai.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xfy.sjlbkw.cn

[T43] Perl：字符串插值
来源：http://ttv.zhixingplan.top

"值: $a"
来源：http://gce.tianlin.xyz

[T44] Perl：条件
来源：http://pou.cashguo.top

if ($a > 0) { print "正"; }
来源：http://zcy.yvedp.cn

[T45] Perl：数组遍历
来源：http://fwa.jlsjyb.cn

for my $x (@arr) { print $x; }
来源：http://pxz.jinqigfzy.top

[T46] Perl：哈希操作
来源：http://wdo.zycfv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rbo.xylfe.cn

[T47] Perl：正则捕获
来源：http://lmo.dashuyun.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ojj.yanxiufei.cn

[T48] Perl：正则替换
来源：http://ukp.fanxiaobao.xyz

$s =~ s/old/new/g;
来源：http://ulg.chenjidiqi.icu

[T49] Perl：函数
来源：http://bgp.xylfe.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uua.sjlbkw.cn

[T50] Perl：逐行读文件
来源：http://wuu.zhengqikj.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jdh.sxryk.cn

while (my $line = <$fh>) { print $line; }
来源：http://hab.snrcjt.cn

[T51] Scala：Hello World
来源：http://tuc.hywenlv.cn

println("Hello")
来源：http://ncd.fengsongda.top

[T52] Scala：变量
来源：http://dzm.zhaomingkeji.xyz

val a = 1;  var b = 2
来源：http://iti.zycfv.cn

[T53] Scala：字符串插值
来源：http://kot.cdnleiting.top

s"值: $b"
来源：http://byo.cdnleiting.top

[T54] Scala：集合映射
来源：http://ncu.wangshuangyany.cn

List(1, 2, 3).map(_ * 2)
来源：http://hhv.cqqwz.cn

[T55] Scala：集合过滤
来源：http://vze.gaohongyu789.top

List(1, 2, 3).filter(_ > 1)
来源：http://xjt.nanxinkj.top

[T56] Scala：样例类
来源：http://ewn.svipenyu.cn

case class User(name: String, age: Int)
来源：http://jyr.fanxiaobao.xyz

[T57] Scala：模式匹配
来源：http://emz.fzhhl.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ezu.52xcode.cn

[T58] Scala：函数定义
来源：http://fgx.snrcjt.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wng.fengsongda.top

[T59] Scala：循环
来源：http://xne.shangyingyoupin.top

for (i <- 1 to 10) println(i)
来源：http://mqc.sufxvd.cn

[T60] Scala：折叠
来源：http://jcj.hongshengwenyu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lbk.sxryk.cn

================================================================================
来源：http://akf.cdnleiting.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vim.vehdjk.com

================================================================================
来源：http://qek.yangfankeji.com


<!-- 参考信息 -->