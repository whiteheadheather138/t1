代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vlz.hammf.cn

[R60] 只看 HTTP 状态码
来源：http://zza.gaohongyu789.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://aol.zycfv.cn

[R61] 磁盘占用
来源：http://gzx.yj202588.top

df -h;  du -sh *
来源：http://tqo.bbcook.cn

[R62] 找最占空间的文件
来源：http://wsc.sweek.top

du -ah . | sort -rh | head -10
来源：http://cpd.vehdjk.com

[R63] 内存与进程
来源：http://oyr.aizwys.cn

free -h;  ps aux | grep nginx
来源：http://irv.tanke756.top

[R64] 结束进程
来源：http://lpn.ybcxt.top

kill -9 $(pgrep -f app.py)
来源：http://vne.yj20258.top

[R65] 查看端口占用
来源：http://aot.jqgfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vvu.xylfe.cn

[R66] 定时任务
来源：http://wda.gaohongyu789.top

crontab -e;  crontab -l
来源：http://lil.guowangkeji.top

[R67] 生成随机十六进制串
来源：http://yge.shanyushiyangkeji.top

openssl rand -hex 16
来源：http://rfs.gaohongyu789.top

[R68] 计算文件校验值
来源：http://dwu.316326.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://klo.jinqigufen.top

[R69] 生成随机密码
来源：http://lgf.xuetiantiany.cn

head -c 16 /dev/urandom | base64
来源：http://yyk.yj20258888.top

[R70] 时间戳与互转
来源：http://omm.ybcxt.top

date +%s;  date -d @1700000000
来源：http://xga.9152youxi.cn

[R71] 日期格式化
来源：http://sdk.hcnkem.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://kfh.9152youxi.cn

[R72] 等待端口就绪
来源：http://for.bbcook.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://thp.sxryk.cn

[R73] 分割大日志
来源：http://div.jinyuanbaomall.cn

split -l 1000 big.log part_
来源：http://cfg.aizwys.cn

[R74] 批量重命名
来源：http://bwj.sweek.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cbk.gaohongyu789.top

[R75] 导出环境变量
来源：http://hum.chenzaomai.com

export PATH="$HOME/bin:$PATH"
来源：http://ruz.yvedp.cn

[R76] 使用临时文件
来源：http://ytw.nwbrower.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://suo.epnwcf.com

[R77] 读取用户输入
来源：http://xgy.c1oappe.top

read -rp "请输入: " ans
来源：http://sgi.chenjidiqi.icu

[R78] 交互式菜单
来源：http://oia.hammf.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cwr.fanxiaobao.xyz

[R79] 解析命令行选项
来源：http://ztg.zhijiandao.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hgy.tian-w.cn

[R80] 查看脚本执行耗时
来源：http://wae.jinqigufen.top

time ./run.sh
来源：http://oir.yueranfly.top

================================================================================
来源：http://pzw.xylfe.cn

S. C / C++ 专题
来源：http://wsq.haohaochexian.top

================================================================================
来源：http://glo.xziqi.cn

[S01] C：Hello World
来源：http://ugi.dianchejie.cn

#include <stdio.h>
来源：http://gpt.tianlin.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://hvf.chenjidiqi.icu

[S02] C：变量与格式化输出
来源：http://ssk.dianchejie.cn

int a = 10; printf("%d\n", a);
来源：http://ziv.birdmap.top

[S03] C：读入整数
来源：http://wxn.mhx1999.top

int x; scanf("%d", &x);
来源：http://yua.9152youxi.cn

[S04] C：字符串复制
来源：http://kal.bjfxy.top

char dst[32]; strcpy(dst, "hi");
来源：http://xpl.gzhubu.top

[S05] C：字符串长度
来源：http://eed.fengsongda.top

strlen(s)
来源：http://ovf.tanke756.top

[S06] C：字符串比较
来源：http://wwr.cqqwz.cn

strcmp(a, b) == 0
来源：http://omo.pycfn.com

[S07] C：数组遍历求和
来源：http://loq.kuanghao11.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://muo.shuidangran.top

[S08] C：动态内存分配与释放
来源：http://cvb.wangshuangyany.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cow.c1oappe.top

[S09] C：结构体定义与初始化
来源：http://vaz.dashuyun.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jdz.sjlbkw.cn

[S10] C：指针与解引用
来源：http://ive.wangdashe.top

int *p = &a;  *p = 5;
来源：http://rdn.ehwqpu.com

[S11] C：逐行读文件
来源：http://ivm.ppjwa.cn

FILE *f = fopen("a.txt", "r");
来源：http://zup.jqgfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://krs.shuidangran.top

fclose(f);
来源：http://fdp.ivvv.top

[S12] C：写文件
来源：http://lhg.gaohongyu789.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xiw.fengsongda.top

[S13] C：宏定义
来源：http://hge.xziqi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fxk.aibaodan.cn

[S14] C：枚举
来源：http://eog.c1oappe.top

enum Color { RED, GREEN, BLUE };
来源：http://nyl.zhoulong.xyz

[S15] C：类型转换
来源：http://mve.gaohongyu789.top

(double) a / b
来源：http://aso.shanyushiyangtech.top

[S16] C：位操作置位
来源：http://dye.vqdsnc.cn

x |= (1 << 3);
来源：http://pog.sufxvd.cn

[S17] C：安全拼接字符串
来源：http://vul.cheryme.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xdg.ehwqpu.com

[S18] C：命令行参数
来源：http://bat.sjlbkw.cn

int main(int argc, char **argv)
来源：http://oqb.ppjwa.cn

[S19] C：快速排序
来源：http://ayr.yuanzhike.top

qsort(a, n, sizeof(int), cmp);
来源：http://kho.vehdjk.com

[S20] C：二分查找
来源：http://pvb.tianlin.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ybw.xuetiantiany.cn

[S21] C：字符类别判断
来源：http://kug.jiagoushi.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fww.feifeiyinyue.top

[S22] C：字符串转数字
来源：http://zya.pengpengdd.cyou

atoi("42");  strtod("3.14", NULL);
来源：http://lia.gogol.net.cn

[S23] C：随机数
来源：http://oes.yangfankeji.com

srand(time(NULL));  int r = rand() % 100;
来源：http://gvr.andypj.xyz

[S24] C：获取本地时间
来源：http://die.pengpengdd.cyou

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vzc.snrcjt.cn

[S25] C：内存拷贝
来源：http://lst.zhoulong.xyz

memcpy(dst, src, n);
来源：http://xpv.redwolf501.top

[S26] C：内存清零
来源：http://xrd.feifeiyinyue.top

memset(a, 0, sizeof a);
来源：http://krq.xinyue.icu

[S27] C：定义常量
来源：http://owp.sweek.top

const double PI = 3.14159;
来源：http://dfl.ybcxt.top

[S28] C：静态变量
来源：http://ipr.yvedp.cn

static int counter = 0;
来源：http://lpz.mhx1999.top

[S29] C：变参函数
来源：http://qan.zhoulong.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gci.zhiwuduotai.top

[S30] C：头文件保护
来源：http://akx.epnwcf.com

#ifndef X_H
来源：http://qgk.yonumen.top

#define X_H
来源：http://ssw.jlsjyb.cn

#endif
来源：http://ppf.yongpay.top

[S31] C++：Hello World
来源：http://eza.c1oappe.top

#include <iostream>
来源：http://ozx.316326.xyz

int main() { std::cout << "Hello\n"; }
来源：http://bmj.chenlongwang.top

[S32] C++：字符串
来源：http://bgi.nwbrower.top

std::string s = "hi";  s += "!";
来源：http://jcl.tian-w.cn

[S33] C++：vector 增删
来源：http://wie.shzxlz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mrx.sysykeji.top

[S34] C++：遍历 vector
来源：http://nao.yueranfly.top

for (auto &x : v) { std::cout << x; }
来源：http://xcr.kuanghao11.cn

[S35] C++：map
来源：http://dxw.gotoacloud.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kne.316326.xyz

[S36] C++：unordered_map
来源：http://ltg.nanxinkj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bep.cucudq.cn

[S37] C++：set
来源：http://xkd.316326.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wir.yangfankeji.com

[S38] C++：排序
来源：http://ver.zhoulong.xyz

std::sort(v.begin(), v.end());
来源：http://hgv.wangshuangyany.cn

[S39] C++：自定义比较器排序
来源：http://eot.zhiwuduotai.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://msk.316326.xyz

[S40] C++：查找元素
来源：http://fto.zhiwuduotai.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://awe.c1oappe.top

[S41] C++：类与构造函数
来源：http://gaz.fengsongda.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gwv.jinghuilouyu.cn

[S42] C++：继承与虚函数
来源：http://pzl.kuanghao11.cn

class B : public Base { public: void f() override {} };
来源：http://xtt.snrcjt.cn

[S43] C++：智能指针
来源：http://tvd.jqgfzy.top

auto p = std::make_unique<int>(5);
来源：http://qol.sweek.top

[S44] C++：引用传参
来源：http://vuh.bjfxy.top

void inc(int &x) { ++x; }
来源：http://alf.fzhhl.top

[S45] C++：lambda
来源：http://cau.xinyue.icu

auto add = [](int a, int b) { return a + b; };
来源：http://zuy.hammf.cn

[S46] C++：函数模板
来源：http://trm.tarul.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qlh.tian-w.cn

[S47] C++：结构化绑定遍历
来源：http://wsf.shuidangran.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hbx.hcnkem.com

[S48] C++：逐行读文件
来源：http://ufj.jinqigfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://daw.xuetiantiany.cn

while (std::getline(in, line)) { }
来源：http://stt.chenjidiqi.icu

[S49] C++：写文件
来源：http://caa.fengsongda.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zod.yuanzhike.top

[S50] C++：格式化数字
来源：http://vha.xuetiantiany.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pgt.jinghuilouyu.cn

[S51] C++：显式类型转换
来源：http://xbz.xziqi.cn

static_cast<double>(a) / b
来源：http://zfx.316326.xyz

[S52] C++：const 与 noexcept
来源：http://iwo.sxryk.cn

int size() const noexcept { return n_; }
来源：http://gdg.yuanzhike.top

[S53] C++：移动语义
来源：http://ecw.xinyue.icu

std::vector<int> w = std::move(v);
来源：http://iuh.redwolf501.top

[S54] C++：异常处理
来源：http://ntf.hammf.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gpd.ivvv.top

[S55] C++：结构化绑定
来源：http://fya.iojbl.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qkx.fktsv.cn

[S56] C++：optional
来源：http://kdc.vqdsnc.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oez.chenjidiqi.icu

[S57] C++：编译期常量
来源：http://zcj.andypj.xyz

constexpr int N = 10;
来源：http://uev.jyoumei.cn

[S58] C++：命名空间
来源：http://fwg.hnxiangtu.top

namespace ns { int f() { return 1; } }
来源：http://leo.dianchejie.cn

[S59] C++：静态断言
来源：http://bpg.jinyuanbaomall.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nru.9152youxi.cn

[S60] C++：遍历并删除元素
来源：http://qyb.jinqigufen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rgj.aizwys.cn

================================================================================
来源：http://ifn.ivvv.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iyo.mhx1999.top

================================================================================
来源：http://ppk.hesvh.cn

[T01] Kotlin：Hello World
来源：http://otq.pengpengdd.cyou

println("Hello")
来源：http://zfu.hfpthk.cn

[T02] Kotlin：变量
来源：http://rtv.zhaomingkeji.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dqt.smart0.xyz

[T03] Kotlin：字符串模板
来源：http://hzq.meibo888.top

"值: $b"
来源：http://tlt.52xcode.cn

[T04] Kotlin：空安全
来源：http://gcd.gzhubu.top

val n: String? = null;  n?.length
来源：http://tfu.dashuyun.cn

[T05] Kotlin：when 表达式
来源：http://ksn.vehdjk.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zpr.xingfuxueyuan.xyz

[T06] Kotlin：集合映射
来源：http://pev.jianghu66.top

listOf(1, 2, 3).map { it * 2 }
来源：http://viv.shzxlz.cn

[T07] Kotlin：集合过滤
来源：http://ysy.xuanzx.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://gir.hywenlv.cn

[T08] Kotlin：数据类
来源：http://jfo.yangfankeji.com

data class User(val name: String, val age: Int)
来源：http://lsr.dashuyun.cn

[T09] Kotlin：扩展函数
来源：http://skv.bjfxy.top

fun String.exclaim() = this + "!"
来源：http://ulv.chenzaomai.com

[T10] Kotlin：默认参数
来源：http://qwz.sxryk.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://zlp.aibaodan.cn

[T11] Kotlin：协程
来源：http://qot.xingfuxueyuan.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://rfa.uphjek.com

[T12] Kotlin：解构声明
来源：http://ztk.aibaodan.cn

val (a, b) = Pair(1, 2)
来源：http://soy.0kj1m.cn

[T13] Kotlin：只读 Map
来源：http://tvp.dianchejie.cn

val m = mapOf("a" to 1)
来源：http://jsh.jyoumei.cn

[T14] Kotlin：循环
来源：http://rrl.yangfankeji.com

for (i in 1..10) println(i)
来源：http://qew.zhixingplan.top

[T15] Kotlin：接口
来源：http://ocv.hysaishi.cn

interface Shape { fun area(): Double }
来源：http://pab.jqgufenzy.top

[T16] Swift：Hello World
来源：http://vlr.fanxiaobao.xyz

print("Hello")
来源：http://oiw.jiagoushi.top

[T17] Swift：变量与常量
来源：http://ysc.yonumen.top

var a = 1;  let b = 2
来源：http://gza.zhongyouzk.top

[T18] Swift：字符串插值
来源：http://apr.sufxvd.cn

"值: \(b)"
来源：http://iau.fzhhl.top

[T19] Swift：可选绑定
来源：http://eih.fzhhl.top

if let n = opt { print(n) }
来源：http://xje.haohaochexian.top

[T20] Swift：数组操作
来源：http://aqe.hcnkem.com

var a = [1, 2, 3];  a.append(4)
来源：http://fuq.shzxlz.cn

[T21] Swift：遍历
来源：http://mnz.hesvh.cn

for x in a { print(x) }
来源：http://ptg.quarkkingdee.top

[T22] Swift：字典
来源：http://izj.pengpengdd.cyou

var d = ["a": 1];  d["b"] = 2
来源：http://ryn.zycfv.cn

[T23] Swift：函数
来源：http://mif.smart0.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cql.bbcook.cn

[T24] Swift：闭包
来源：http://ptv.cdnleiting.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://eej.ivvv.top

[T25] Swift：结构体
来源：http://aes.9152youxi.cn

struct P { var x: Int }
来源：http://yta.chenzaomai.com

[T26] Swift：类与重写
来源：http://qal.chenzaomai.com

class A: Base { override func f() {} }
来源：http://nml.cqqwz.cn

[T27] Swift：错误处理
来源：http://tve.zycfv.cn

do { try f() } catch { print(error) }
来源：http://edb.dashuyun.cn

[T28] Swift：枚举
来源：http://ugh.xinyue.icu

enum Color { case red, green }
来源：http://snd.aibaodan.cn

[T29] Swift：guard 提前返回
来源：http://osl.shzxlz.cn

guard let x = opt else { return }
来源：http://jyq.wangdashe.top

[T30] Swift：协议
来源：http://jpz.pycfn.com

protocol Shape { func area() -> Double }
来源：http://erf.nanxuanxn.top

[T31] Lua：Hello World
来源：http://kye.nanxinkj.top

print("Hello")
来源：http://uea.ppjwa.cn

[T32] Lua：局部变量
来源：http://ejy.bbcook.cn

local a = 1
来源：http://ibp.iojbl.cn

[T33] Lua：表（数组）
来源：http://jdp.ybcxt.top

local t = {1, 2, 3};  t[4] = 4
来源：http://hqu.0kj1m.cn

[T34] Lua：遍历表
来源：http://zrw.tianlin.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://xxo.sufxvd.cn

[T35] Lua：字典表
来源：http://atf.vqdsnc.cn

local d = { a = 1 };  d.b = 2
来源：http://eda.dashuyun.cn

[T36] Lua：函数
来源：http://rbl.sufxvd.cn

function add(a, b) return a + b end
来源：http://ush.pengpengdd.cyou

[T37] Lua：字符串拼接
来源：http://cqo.jqgfzy.top

"a" .. "b"
来源：http://gfc.zhengqikj.top

[T38] Lua：条件
来源：http://cgd.zhengqikj.top

if x > 0 then print("正") end
来源：http://pol.sweek.top

[T39] Lua：模式匹配
来源：http://ncx.cdnleiting.top

string.find(s, "%d+")
来源：http://ucw.tian-w.cn

[T40] Lua：元表
来源：http://lcc.fengsongda.top

setmetatable({}, { __index = base })
来源：http://adz.tianlin.xyz

[T41] Perl：Hello World
来源：http://rax.fzhhl.top

print "Hello\n";
来源：http://sgm.iojbl.cn

[T42] Perl：变量类型
来源：http://eau.52xcode.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qla.yj20258.top

[T43] Perl：字符串插值
来源：http://tus.hesvh.cn

"值: $a"
来源：http://qtt.yonumen.top

[T44] Perl：条件
来源：http://qwa.daxiang520.top

if ($a > 0) { print "正"; }
来源：http://hit.gaohongyu789.top

[T45] Perl：数组遍历
来源：http://pcn.fengsongda.top

for my $x (@arr) { print $x; }
来源：http://vkx.zhengqikj.top

[T46] Perl：哈希操作
来源：http://ulj.yangfankeji.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://eha.fzhhl.top

[T47] Perl：正则捕获
来源：http://lgf.316326.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://cuv.tarul.cn

[T48] Perl：正则替换
来源：http://lkh.quarkkingdee.top

$s =~ s/old/new/g;
来源：http://vmv.wangshuangyany.cn

[T49] Perl：函数
来源：http://vdt.havefunace.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jsc.jqgufenzy.top

[T50] Perl：逐行读文件
来源：http://nma.jlsjyb.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://pgk.nanxinkj.top

while (my $line = <$fh>) { print $line; }
来源：http://ufs.c1oappe.top

[T51] Scala：Hello World
来源：http://lge.jiagoushi.top

println("Hello")
来源：http://ewa.sysykeji.top

[T52] Scala：变量
来源：http://pql.daria6918.cn

val a = 1;  var b = 2
来源：http://ypw.gotoacloud.top

[T53] Scala：字符串插值
来源：http://alh.xingfuxueyuan.xyz

s"值: $b"
来源：http://qnx.pengpengdd.cyou

[T54] Scala：集合映射
来源：http://ltc.sxryk.cn

List(1, 2, 3).map(_ * 2)
来源：http://yvw.zhijiandao.cn

[T55] Scala：集合过滤
来源：http://bjt.shangyingyoupin.top

List(1, 2, 3).filter(_ > 1)
来源：http://daf.yangfankeji.com

[T56] Scala：样例类
来源：http://tdk.snrcjt.cn

case class User(name: String, age: Int)
来源：http://rwx.xinyue.icu

[T57] Scala：模式匹配
来源：http://blx.yj202588.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://sjh.dianchejie.cn

[T58] Scala：函数定义
来源：http://wrh.yueranfly.top

def add(a: Int, b: Int): Int = a + b
来源：http://qrs.ivvv.top

[T59] Scala：循环
来源：http://iwq.ctjpmb.com

for (i <- 1 to 10) println(i)
来源：http://qgp.hnqzz.top

[T60] Scala：折叠
来源：http://qar.yuanzhike.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://znq.yangfankeji.com

================================================================================
来源：http://lxa.fanxiaobao.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://grz.epnwcf.com

================================================================================
来源：http://opl.jiagoushi.top


<!-- 参考信息 -->