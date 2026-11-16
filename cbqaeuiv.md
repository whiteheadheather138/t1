代发 wailian999

df -h;  du -sh *
来源：http://axq.sjlbkw.cn

[R62] 找最占空间的文件
来源：http://tjv.cucudq.cn

du -ah . | sort -rh | head -10
来源：http://nff.hammf.cn

[R63] 内存与进程
来源：http://zsj.sweek.top

free -h;  ps aux | grep nginx
来源：http://csw.zhengqikj.top

[R64] 结束进程
来源：http://tnn.jqgfzy.top

kill -9 $(pgrep -f app.py)
来源：http://mms.shuidangran.top

[R65] 查看端口占用
来源：http://lii.ppjwa.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xiq.yfazqb.com

[R66] 定时任务
来源：http://xzy.316326.xyz

crontab -e;  crontab -l
来源：http://wgj.yuxming.cn

[R67] 生成随机十六进制串
来源：http://weo.xziqi.cn

openssl rand -hex 16
来源：http://ifi.gaohongyu789.top

[R68] 计算文件校验值
来源：http://wgl.mhx1999.top

sha256sum a.txt;  md5sum a.txt
来源：http://jma.dashuyun.cn

[R69] 生成随机密码
来源：http://bqa.redwolf501.top

head -c 16 /dev/urandom | base64
来源：http://xau.jinyuanbaomall.cn

[R70] 时间戳与互转
来源：http://zkf.0kj1m.cn

date +%s;  date -d @1700000000
来源：http://jnq.chenjidiqi.icu

[R71] 日期格式化
来源：http://kpa.tianlin.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://hih.zhengqikj.top

[R72] 等待端口就绪
来源：http://gvm.ehwqpu.com

until nc -z localhost 3306; do sleep 1; done
来源：http://bmh.yongpay.top

[R73] 分割大日志
来源：http://uwj.zhixingplan.top

split -l 1000 big.log part_
来源：http://vup.fengsongda.top

[R74] 批量重命名
来源：http://jqc.jinqigfzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jpf.fengsongda.top

[R75] 导出环境变量
来源：http://cmk.xziqi.cn

export PATH="$HOME/bin:$PATH"
来源：http://uls.shzxlz.cn

[R76] 使用临时文件
来源：http://uoa.svipenyu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gql.yj20258888.top

[R77] 读取用户输入
来源：http://uhd.aizwys.cn

read -rp "请输入: " ans
来源：http://ech.pycfn.com

[R78] 交互式菜单
来源：http://ngm.sweek.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rob.nanxinkj.top

[R79] 解析命令行选项
来源：http://teq.wangdashe.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cwb.9152youxi.cn

[R80] 查看脚本执行耗时
来源：http://qmi.chenlongwang.top

time ./run.sh
来源：http://joe.yuxming.cn

================================================================================
来源：http://ofn.shanyushiyangkeji.top

S. C / C++ 专题
来源：http://inj.hcnkem.com

================================================================================
来源：http://upn.sxryk.cn

[S01] C：Hello World
来源：http://clt.nanxuanxn.top

#include <stdio.h>
来源：http://aco.yanxiufei.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mch.tanke756.top

[S02] C：变量与格式化输出
来源：http://obg.meibo888.top

int a = 10; printf("%d\n", a);
来源：http://eyq.aibaodan.cn

[S03] C：读入整数
来源：http://frl.zycfv.cn

int x; scanf("%d", &x);
来源：http://pkj.xingfuxueyuan.xyz

[S04] C：字符串复制
来源：http://ggp.zhengqikj.top

char dst[32]; strcpy(dst, "hi");
来源：http://rdw.daxiang520.top

[S05] C：字符串长度
来源：http://atq.svipenyu.cn

strlen(s)
来源：http://siz.nanxinkj.top

[S06] C：字符串比较
来源：http://rlg.kuanghao11.cn

strcmp(a, b) == 0
来源：http://wvx.tanke756.top

[S07] C：数组遍历求和
来源：http://uof.sufxvd.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tzs.iojbl.cn

[S08] C：动态内存分配与释放
来源：http://moh.aibaodan.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jvm.hnxiangtu.top

[S09] C：结构体定义与初始化
来源：http://hak.quarkkingdee.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gjj.gogol.net.cn

[S10] C：指针与解引用
来源：http://oqa.52xcode.cn

int *p = &a;  *p = 5;
来源：http://czv.fktsv.cn

[S11] C：逐行读文件
来源：http://tbc.jiagoushi.top

FILE *f = fopen("a.txt", "r");
来源：http://ltt.sweek.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://rtz.mhx1999.top

fclose(f);
来源：http://txq.cucudq.cn

[S12] C：写文件
来源：http://aek.gotoacloud.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://akd.hongshengwenyu.top

[S13] C：宏定义
来源：http://onw.yueranfly.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oid.svipenyu.cn

[S14] C：枚举
来源：http://ilj.jqgfzy.top

enum Color { RED, GREEN, BLUE };
来源：http://lkn.chenlongwang.top

[S15] C：类型转换
来源：http://cza.daria6918.cn

(double) a / b
来源：http://zry.wangshuangyany.cn

[S16] C：位操作置位
来源：http://lwe.uphjek.com

x |= (1 << 3);
来源：http://mti.cdnleiting.top

[S17] C：安全拼接字符串
来源：http://alu.ehwqpu.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kws.sweek.top

[S18] C：命令行参数
来源：http://amb.hysaishi.cn

int main(int argc, char **argv)
来源：http://fne.tianlin.xyz

[S19] C：快速排序
来源：http://mpw.jinqigfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://mxt.316326.xyz

[S20] C：二分查找
来源：http://sus.yuxming.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eqq.pycfn.com

[S21] C：字符类别判断
来源：http://ezj.hywenlv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jrz.yongpay.top

[S22] C：字符串转数字
来源：http://fsz.hnxiangtu.top

atoi("42");  strtod("3.14", NULL);
来源：http://uwe.yj20258888.top

[S23] C：随机数
来源：http://hje.zhixingplan.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qvw.hnxiangtu.top

[S24] C：获取本地时间
来源：http://yoc.gotoacloud.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://edo.ivvv.top

[S25] C：内存拷贝
来源：http://xww.ppjwa.cn

memcpy(dst, src, n);
来源：http://rpo.yfazqb.com

[S26] C：内存清零
来源：http://nub.zhengqikj.top

memset(a, 0, sizeof a);
来源：http://xyr.shanyushiyangkeji.top

[S27] C：定义常量
来源：http://knv.xinyue.icu

const double PI = 3.14159;
来源：http://naz.gogol.net.cn

[S28] C：静态变量
来源：http://ayg.yj20258888.top

static int counter = 0;
来源：http://lec.yongpay.top

[S29] C：变参函数
来源：http://fpr.quarkkingdee.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hei.c1oappe.top

[S30] C：头文件保护
来源：http://ftz.zycfv.cn

#ifndef X_H
来源：http://zus.hywenlv.cn

#define X_H
来源：http://mmh.uphjek.com

#endif
来源：http://ios.xingfuxueyuan.xyz

[S31] C++：Hello World
来源：http://ygy.haohaochexian.top

#include <iostream>
来源：http://poq.ppjwa.cn

int main() { std::cout << "Hello\n"; }
来源：http://koo.yongpay.top

[S32] C++：字符串
来源：http://ldz.jinqigufen.top

std::string s = "hi";  s += "!";
来源：http://pzv.hywenlv.cn

[S33] C++：vector 增删
来源：http://int.birdmap.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yqy.xylfe.cn

[S34] C++：遍历 vector
来源：http://aqo.smart0.xyz

for (auto &x : v) { std::cout << x; }
来源：http://ytg.xuetiantiany.cn

[S35] C++：map
来源：http://lyx.tianlin.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wmp.jinqigufen.top

[S36] C++：unordered_map
来源：http://avq.hywenlv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://itk.zhongyouzk.top

[S37] C++：set
来源：http://pdc.daria6918.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lfw.wangdashe.top

[S38] C++：排序
来源：http://ddb.cheryme.top

std::sort(v.begin(), v.end());
来源：http://qed.jianghu66.top

[S39] C++：自定义比较器排序
来源：http://oet.cashguo.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://csh.hysaishi.cn

[S40] C++：查找元素
来源：http://lqn.hnxiangtu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qwe.fengsongda.top

[S41] C++：类与构造函数
来源：http://bbi.vqdsnc.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yid.ywan-chungtsiang.top

[S42] C++：继承与虚函数
来源：http://ctx.52xcode.cn

class B : public Base { public: void f() override {} };
来源：http://hdj.xziqi.cn

[S43] C++：智能指针
来源：http://qcu.zhaomingkeji.xyz

auto p = std::make_unique<int>(5);
来源：http://awn.daxiang520.top

[S44] C++：引用传参
来源：http://rfr.bbcook.cn

void inc(int &x) { ++x; }
来源：http://oti.pycfn.com

[S45] C++：lambda
来源：http://lpc.bbcook.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pry.vqdsnc.cn

[S46] C++：函数模板
来源：http://rur.fktsv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yla.daria6918.cn

[S47] C++：结构化绑定遍历
来源：http://qia.mhx1999.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mqy.fktsv.cn

[S48] C++：逐行读文件
来源：http://jqu.xinyue.icu

std::ifstream in("a.txt");  std::string line;
来源：http://ofa.hnqzz.top

while (std::getline(in, line)) { }
来源：http://xpk.zdqjudy.top

[S49] C++：写文件
来源：http://wjg.dianchejie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lkf.fktsv.cn

[S50] C++：格式化数字
来源：http://nfw.ivvv.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tbp.guannengcc.top

[S51] C++：显式类型转换
来源：http://wfg.hysaishi.cn

static_cast<double>(a) / b
来源：http://wzi.316326.xyz

[S52] C++：const 与 noexcept
来源：http://cip.hcnkem.com

int size() const noexcept { return n_; }
来源：http://zvi.shzxlz.cn

[S53] C++：移动语义
来源：http://aom.hnxiangtu.top

std::vector<int> w = std::move(v);
来源：http://btu.bjfxy.top

[S54] C++：异常处理
来源：http://zrh.yfazqb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oja.guowangkeji.top

[S55] C++：结构化绑定
来源：http://iat.yuanzhike.top

auto [a, b] = std::make_pair(1, 2);
来源：http://cka.tarul.cn

[S56] C++：optional
来源：http://ron.xingfuxueyuan.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dir.wangshuangyany.cn

[S57] C++：编译期常量
来源：http://hho.dianchejie.cn

constexpr int N = 10;
来源：http://rzw.sjlbkw.cn

[S58] C++：命名空间
来源：http://fio.ctjpmb.com

namespace ns { int f() { return 1; } }
来源：http://wan.xingfuxueyuan.xyz

[S59] C++：静态断言
来源：http://tyc.zycfv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zgp.hnqzz.top

[S60] C++：遍历并删除元素
来源：http://mdn.zhengqikj.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yon.jinqigufen.top

================================================================================
来源：http://tkg.jqgfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rqn.sjlbkw.cn

================================================================================
来源：http://dia.jinqigufen.top

[T01] Kotlin：Hello World
来源：http://opq.jianghu66.top

println("Hello")
来源：http://zhp.xinyue.icu

[T02] Kotlin：变量
来源：http://tja.xingfuxueyuan.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pcx.epnwcf.com

[T03] Kotlin：字符串模板
来源：http://jhh.pengpengdd.cyou

"值: $b"
来源：http://jhr.xuanzx.com

[T04] Kotlin：空安全
来源：http://ija.0kj1m.cn

val n: String? = null;  n?.length
来源：http://twx.fzhhl.top

[T05] Kotlin：when 表达式
来源：http://pwo.wangshuangyany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://koh.zdqjudy.top

[T06] Kotlin：集合映射
来源：http://mdp.zdbjq.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pra.xziqi.cn

[T07] Kotlin：集合过滤
来源：http://ool.chenzaomai.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://iva.shuidangran.top

[T08] Kotlin：数据类
来源：http://sbl.jqgfzy.top

data class User(val name: String, val age: Int)
来源：http://cpc.fanxiaobao.xyz

[T09] Kotlin：扩展函数
来源：http://yla.iojbl.cn

fun String.exclaim() = this + "!"
来源：http://zlm.yueranfly.top

[T10] Kotlin：默认参数
来源：http://srs.zdqjudy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://lhr.guannengcc.top

[T11] Kotlin：协程
来源：http://qan.hfpthk.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lfa.fehbvm.com

[T12] Kotlin：解构声明
来源：http://wiq.ybcxt.top

val (a, b) = Pair(1, 2)
来源：http://tss.zdqjudy.top

[T13] Kotlin：只读 Map
来源：http://gbd.yanxiufei.cn

val m = mapOf("a" to 1)
来源：http://hyu.iojbl.cn

[T14] Kotlin：循环
来源：http://etp.xziqi.cn

for (i in 1..10) println(i)
来源：http://dap.snrcjt.cn

[T15] Kotlin：接口
来源：http://rau.yj20258888.top

interface Shape { fun area(): Double }
来源：http://pso.shanyushiyangkeji.top

[T16] Swift：Hello World
来源：http://jrt.fktsv.cn

print("Hello")
来源：http://hzc.wangdashe.top

[T17] Swift：变量与常量
来源：http://mah.pycfn.com

var a = 1;  let b = 2
来源：http://vyu.316326.xyz

[T18] Swift：字符串插值
来源：http://aiz.guowangkeji.top

"值: \(b)"
来源：http://sjt.tianlin.xyz

[T19] Swift：可选绑定
来源：http://upq.cdnleiting.top

if let n = opt { print(n) }
来源：http://ruz.gotoacloud.top

[T20] Swift：数组操作
来源：http://gjb.iojbl.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jvb.tarul.cn

[T21] Swift：遍历
来源：http://azj.hnxiangtu.top

for x in a { print(x) }
来源：http://opu.316326.xyz

[T22] Swift：字典
来源：http://omp.hammf.cn

var d = ["a": 1];  d["b"] = 2
来源：http://evl.zhongyouzk.top

[T23] Swift：函数
来源：http://hao.andypj.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gpa.gogol.net.cn

[T24] Swift：闭包
来源：http://eft.c1oappe.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://cdv.zhaomingkeji.xyz

[T25] Swift：结构体
来源：http://imf.zdqjudy.top

struct P { var x: Int }
来源：http://tme.yfazqb.com

[T26] Swift：类与重写
来源：http://sxx.c1oappe.top

class A: Base { override func f() {} }
来源：http://ecp.chenlongwang.top

[T27] Swift：错误处理
来源：http://wdb.ywan-chungtsiang.top

do { try f() } catch { print(error) }
来源：http://rri.gotoacloud.top

[T28] Swift：枚举
来源：http://kde.yongpay.top

enum Color { case red, green }
来源：http://exj.zhiwuduotai.top

[T29] Swift：guard 提前返回
来源：http://tug.xziqi.cn

guard let x = opt else { return }
来源：http://ptl.yj202588.top

[T30] Swift：协议
来源：http://aek.yj20258.top

protocol Shape { func area() -> Double }
来源：http://ibd.chenlongwang.top

[T31] Lua：Hello World
来源：http://jtb.yueranfly.top

print("Hello")
来源：http://fdx.chenlongwang.top

[T32] Lua：局部变量
来源：http://dus.shanyushiyangtech.top

local a = 1
来源：http://fdy.jlsjyb.cn

[T33] Lua：表（数组）
来源：http://zgm.jinqigufen.top

local t = {1, 2, 3};  t[4] = 4
来源：http://jtv.zhaomingkeji.xyz

[T34] Lua：遍历表
来源：http://mne.jqgfzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://rhp.zhongyouzk.top

[T35] Lua：字典表
来源：http://tus.yvedp.cn

local d = { a = 1 };  d.b = 2
来源：http://jhe.bbcook.cn

[T36] Lua：函数
来源：http://yay.hesvh.cn

function add(a, b) return a + b end
来源：http://rbq.yj20258888.top

[T37] Lua：字符串拼接
来源：http://dvi.mhx1999.top

"a" .. "b"
来源：http://tyr.kuanghao11.cn

[T38] Lua：条件
来源：http://usu.chenjidiqi.icu

if x > 0 then print("正") end
来源：http://ibs.gzhubu.top

[T39] Lua：模式匹配
来源：http://dzs.jinqigufen.top

string.find(s, "%d+")
来源：http://gln.haohaochexian.top

[T40] Lua：元表
来源：http://acp.shanyushiyangtech.top

setmetatable({}, { __index = base })
来源：http://wki.birdmap.top

[T41] Perl：Hello World
来源：http://kfz.zdbjq.cn

print "Hello\n";
来源：http://ovw.guowangkeji.top

[T42] Perl：变量类型
来源：http://mfq.uphjek.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ftl.cheryme.top

[T43] Perl：字符串插值
来源：http://pro.cqqwz.cn

"值: $a"
来源：http://bkv.shzxlz.cn

[T44] Perl：条件
来源：http://hwi.tianlin.xyz

if ($a > 0) { print "正"; }
来源：http://vfu.hesvh.cn

[T45] Perl：数组遍历
来源：http://xwn.hnxiangtu.top

for my $x (@arr) { print $x; }
来源：http://ory.cdnleiting.top

[T46] Perl：哈希操作
来源：http://aoy.feifeiyinyue.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mqv.sysykeji.top

[T47] Perl：正则捕获
来源：http://ljg.wangdashe.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://flq.jiagoushi.top

[T48] Perl：正则替换
来源：http://dew.daria6918.cn

$s =~ s/old/new/g;
来源：http://bpz.haohaochexian.top

[T49] Perl：函数
来源：http://jxi.shanyushiyangkeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ibx.shanyushiyangtech.top

[T50] Perl：逐行读文件
来源：http://oxc.fehbvm.com

open my $fh, "<", "a.txt" or die $!;
来源：http://ieu.nanxuanxn.top

while (my $line = <$fh>) { print $line; }
来源：http://sfl.zhixingplan.top

[T51] Scala：Hello World
来源：http://jur.daria6918.cn

println("Hello")
来源：http://gwr.fktsv.cn

[T52] Scala：变量
来源：http://yao.fengsongda.top

val a = 1;  var b = 2
来源：http://ygz.cucudq.cn

[T53] Scala：字符串插值
来源：http://lsb.jianghu66.top

s"值: $b"
来源：http://nfa.9152youxi.cn

[T54] Scala：集合映射
来源：http://ail.sweek.top

List(1, 2, 3).map(_ * 2)
来源：http://rpt.jyoumei.cn

[T55] Scala：集合过滤
来源：http://eia.mhx1999.top

List(1, 2, 3).filter(_ > 1)
来源：http://nxp.tianlin.xyz

[T56] Scala：样例类
来源：http://abn.yj20258888.top

case class User(name: String, age: Int)
来源：http://tjn.tian-w.cn

[T57] Scala：模式匹配
来源：http://zux.ctjpmb.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://ypy.yj20258.top

[T58] Scala：函数定义
来源：http://alt.guannengcc.top

def add(a: Int, b: Int): Int = a + b
来源：http://crl.bbcook.cn

[T59] Scala：循环
来源：http://hck.jqgfzy.top

for (i <- 1 to 10) println(i)
来源：http://ljo.pengpengdd.cyou

[T60] Scala：折叠
来源：http://nfg.sysykeji.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xyo.bjfxy.top

================================================================================
来源：http://seb.chenjidiqi.icu

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://deh.hcnkem.com

================================================================================
来源：http://aje.wangshuangyany.cn

[U01] Py：创建虚拟环境
来源：http://jgy.kuanghao11.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qty.jinyuanbaomall.cn

[U02] Py：导出 / 安装依赖
来源：http://ebr.ivvv.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zju.316326.xyz


<!-- 参考信息 -->