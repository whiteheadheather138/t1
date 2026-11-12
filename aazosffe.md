代发 wailian999

df -h;  du -sh *
来源：http://uto.xinyue.icu

[R62] 找最占空间的文件
来源：http://ytk.daxiang520.top

du -ah . | sort -rh | head -10
来源：http://ogi.daxiang520.top

[R63] 内存与进程
来源：http://unj.yj20258.top

free -h;  ps aux | grep nginx
来源：http://nyt.zhiwuduotai.top

[R64] 结束进程
来源：http://fmn.iojbl.cn

kill -9 $(pgrep -f app.py)
来源：http://fhx.c1oappe.top

[R65] 查看端口占用
来源：http://uzq.vehdjk.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pth.zdqjudy.top

[R66] 定时任务
来源：http://aim.c1oappe.top

crontab -e;  crontab -l
来源：http://cpr.sufxvd.cn

[R67] 生成随机十六进制串
来源：http://jwi.xziqi.cn

openssl rand -hex 16
来源：http://nyu.guannengcc.top

[R68] 计算文件校验值
来源：http://nqf.nwbrower.top

sha256sum a.txt;  md5sum a.txt
来源：http://aut.ivvv.top

[R69] 生成随机密码
来源：http://yfv.jlsjyb.cn

head -c 16 /dev/urandom | base64
来源：http://lop.bjfxy.top

[R70] 时间戳与互转
来源：http://dvc.snrcjt.cn

date +%s;  date -d @1700000000
来源：http://yzw.yanxiufei.cn

[R71] 日期格式化
来源：http://wgb.xuetiantiany.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nge.jiagoushi.top

[R72] 等待端口就绪
来源：http://oav.shzxlz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xpw.daria6918.cn

[R73] 分割大日志
来源：http://xzp.ydjk.org.cn

split -l 1000 big.log part_
来源：http://xlh.wangshuangyany.cn

[R74] 批量重命名
来源：http://aqj.tian-w.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ure.dianchejie.cn

[R75] 导出环境变量
来源：http://lxs.jinqigufen.top

export PATH="$HOME/bin:$PATH"
来源：http://hdd.52xcode.cn

[R76] 使用临时文件
来源：http://xmx.aizwys.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qdu.jianghu66.top

[R77] 读取用户输入
来源：http://bta.chenjidiqi.icu

read -rp "请输入: " ans
来源：http://ddf.snrcjt.cn

[R78] 交互式菜单
来源：http://yyp.hywenlv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jgl.hysaishi.cn

[R79] 解析命令行选项
来源：http://kph.gogol.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jfw.fengsongda.top

[R80] 查看脚本执行耗时
来源：http://sqr.gotoacloud.top

time ./run.sh
来源：http://wsh.smart0.xyz

================================================================================
来源：http://gjj.yanxiufei.cn

S. C / C++ 专题
来源：http://qay.zhixingplan.top

================================================================================
来源：http://dgg.zhixingplan.top

[S01] C：Hello World
来源：http://jcl.snrcjt.cn

#include <stdio.h>
来源：http://nno.shuidangran.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://zdl.wangshuangyany.cn

[S02] C：变量与格式化输出
来源：http://mty.chenjidiqi.icu

int a = 10; printf("%d\n", a);
来源：http://mdl.xingfuxueyuan.xyz

[S03] C：读入整数
来源：http://pxi.guannengcc.top

int x; scanf("%d", &x);
来源：http://ykv.pycfn.com

[S04] C：字符串复制
来源：http://jpc.zdbjq.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xnr.chenzaomai.com

[S05] C：字符串长度
来源：http://xda.shzxlz.cn

strlen(s)
来源：http://mzl.chenzaomai.com

[S06] C：字符串比较
来源：http://wct.vqdsnc.cn

strcmp(a, b) == 0
来源：http://wqb.chenlongwang.top

[S07] C：数组遍历求和
来源：http://jcx.zhiwuduotai.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xjl.xinyue.icu

[S08] C：动态内存分配与释放
来源：http://qel.ydzc1.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ugk.jinqigufen.top

[S09] C：结构体定义与初始化
来源：http://ijx.jqgfzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://klx.xinyue.icu

[S10] C：指针与解引用
来源：http://vdr.zdbjq.cn

int *p = &a;  *p = 5;
来源：http://ttd.vehdjk.com

[S11] C：逐行读文件
来源：http://mbp.jinqigufen.top

FILE *f = fopen("a.txt", "r");
来源：http://jxm.haohaochexian.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://pds.ppjwa.cn

fclose(f);
来源：http://sxn.yuanzhike.top

[S12] C：写文件
来源：http://jwp.zhaomingkeji.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://aeu.jinqigfzy.top

[S13] C：宏定义
来源：http://yxc.cheryme.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dgy.pycfn.com

[S14] C：枚举
来源：http://ruw.jqgfzy.top

enum Color { RED, GREEN, BLUE };
来源：http://yup.feifeiyinyue.top

[S15] C：类型转换
来源：http://oct.gaohongyu789.top

(double) a / b
来源：http://jzm.cucudq.cn

[S16] C：位操作置位
来源：http://vca.fengsongda.top

x |= (1 << 3);
来源：http://rze.sysykeji.top

[S17] C：安全拼接字符串
来源：http://zdt.wangshuangyany.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kqz.316326.xyz

[S18] C：命令行参数
来源：http://ysk.xuanzx.com

int main(int argc, char **argv)
来源：http://ghv.birdmap.top

[S19] C：快速排序
来源：http://dyt.gotoacloud.top

qsort(a, n, sizeof(int), cmp);
来源：http://qhw.zhiwuduotai.top

[S20] C：二分查找
来源：http://hjz.52xcode.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://koi.yuxming.cn

[S21] C：字符类别判断
来源：http://tvh.bjfxy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dku.sysykeji.top

[S22] C：字符串转数字
来源：http://wgy.tianlin.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://uaq.cheryme.top

[S23] C：随机数
来源：http://tte.quarkkingdee.top

srand(time(NULL));  int r = rand() % 100;
来源：http://aev.tian-w.cn

[S24] C：获取本地时间
来源：http://ebo.chenzaomai.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://svr.fzhhl.top

[S25] C：内存拷贝
来源：http://vxg.feifeiyinyue.top

memcpy(dst, src, n);
来源：http://uvt.ybcxt.top

[S26] C：内存清零
来源：http://wju.xylfe.cn

memset(a, 0, sizeof a);
来源：http://job.xuetiantiany.cn

[S27] C：定义常量
来源：http://nrh.ydzc1.top

const double PI = 3.14159;
来源：http://psr.cqqwz.cn

[S28] C：静态变量
来源：http://kfe.ehwqpu.com

static int counter = 0;
来源：http://hwl.pengpengdd.cyou

[S29] C：变参函数
来源：http://obr.yuanzhike.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://srf.shangyingyoupin.top

[S30] C：头文件保护
来源：http://lhf.xinyue.icu

#ifndef X_H
来源：http://ysg.meibo888.top

#define X_H
来源：http://fzv.xinyue.icu

#endif
来源：http://jcz.hnxiangtu.top

[S31] C++：Hello World
来源：http://wpo.shuidangran.top

#include <iostream>
来源：http://pfk.jinqigfzy.top

int main() { std::cout << "Hello\n"; }
来源：http://ofm.shangyingyoupin.top

[S32] C++：字符串
来源：http://wts.zdqjudy.top

std::string s = "hi";  s += "!";
来源：http://ily.svipenyu.cn

[S33] C++：vector 增删
来源：http://wqx.shanyushiyangkeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ste.yanxiufei.cn

[S34] C++：遍历 vector
来源：http://bqy.yj202588.top

for (auto &x : v) { std::cout << x; }
来源：http://fpn.smart0.xyz

[S35] C++：map
来源：http://tlb.jianghu66.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lvq.jinyuanbaomall.cn

[S36] C++：unordered_map
来源：http://qro.jqgufenzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fkn.gzhubu.top

[S37] C++：set
来源：http://ets.guannengcc.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tpe.chenlongwang.top

[S38] C++：排序
来源：http://rbf.cashguo.top

std::sort(v.begin(), v.end());
来源：http://uvz.c1oappe.top

[S39] C++：自定义比较器排序
来源：http://ymw.yonumen.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ndy.yangfankeji.com

[S40] C++：查找元素
来源：http://ixb.yangfankeji.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rsa.cashguo.top

[S41] C++：类与构造函数
来源：http://jod.wangshuangyany.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sfn.hnxiangtu.top

[S42] C++：继承与虚函数
来源：http://upm.guowangkeji.top

class B : public Base { public: void f() override {} };
来源：http://qlb.c1oappe.top

[S43] C++：智能指针
来源：http://yit.snrcjt.cn

auto p = std::make_unique<int>(5);
来源：http://ccx.hnqzz.top

[S44] C++：引用传参
来源：http://kug.vqdsnc.cn

void inc(int &x) { ++x; }
来源：http://zbf.vqdsnc.cn

[S45] C++：lambda
来源：http://ujf.fengsongda.top

auto add = [](int a, int b) { return a + b; };
来源：http://dpo.shanyushiyangkeji.top

[S46] C++：函数模板
来源：http://utz.xinyue.icu

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://aoo.yj20258.top

[S47] C++：结构化绑定遍历
来源：http://vnc.shzxlz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ycb.aizwys.cn

[S48] C++：逐行读文件
来源：http://eel.jiagoushi.top

std::ifstream in("a.txt");  std::string line;
来源：http://zqn.xingfuxueyuan.xyz

while (std::getline(in, line)) { }
来源：http://bdl.tianlin.xyz

[S49] C++：写文件
来源：http://qos.jianghu66.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hfd.jinyuanbaomall.cn

[S50] C++：格式化数字
来源：http://zck.tarul.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dmc.gotoacloud.top

[S51] C++：显式类型转换
来源：http://rfw.316326.xyz

static_cast<double>(a) / b
来源：http://ywg.ctjpmb.com

[S52] C++：const 与 noexcept
来源：http://fex.vehdjk.com

int size() const noexcept { return n_; }
来源：http://lnk.jianghu66.top

[S53] C++：移动语义
来源：http://jjr.xylfe.cn

std::vector<int> w = std::move(v);
来源：http://yos.pengpengdd.cyou

[S54] C++：异常处理
来源：http://koz.sjlbkw.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ufu.yfazqb.com

[S55] C++：结构化绑定
来源：http://tbp.yongpay.top

auto [a, b] = std::make_pair(1, 2);
来源：http://dhq.nanxinkj.top

[S56] C++：optional
来源：http://ikm.snrcjt.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fjj.sxryk.cn

[S57] C++：编译期常量
来源：http://kdt.xziqi.cn

constexpr int N = 10;
来源：http://qch.tarul.cn

[S58] C++：命名空间
来源：http://mmp.hysaishi.cn

namespace ns { int f() { return 1; } }
来源：http://lym.chenlongwang.top

[S59] C++：静态断言
来源：http://pyq.quarkkingdee.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yos.gotoacloud.top

[S60] C++：遍历并删除元素
来源：http://etu.yueranfly.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vfp.snrcjt.cn

================================================================================
来源：http://twd.jinqigufen.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oqo.xziqi.cn

================================================================================
来源：http://lrh.hnxiangtu.top

[T01] Kotlin：Hello World
来源：http://xrb.smart0.xyz

println("Hello")
来源：http://gcn.ywan-chungtsiang.top

[T02] Kotlin：变量
来源：http://lii.316326.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pae.kuanghao11.cn

[T03] Kotlin：字符串模板
来源：http://eaq.ppjwa.cn

"值: $b"
来源：http://lmi.xuetiantiany.cn

[T04] Kotlin：空安全
来源：http://aoj.xuanzx.com

val n: String? = null;  n?.length
来源：http://itc.xuanzx.com

[T05] Kotlin：when 表达式
来源：http://pnc.jinqigufen.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tsd.gogol.net.cn

[T06] Kotlin：集合映射
来源：http://zsf.jiagoushi.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bpl.yj202588.top

[T07] Kotlin：集合过滤
来源：http://shl.jiagoushi.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://fpt.gaohongyu789.top

[T08] Kotlin：数据类
来源：http://xye.yvedp.cn

data class User(val name: String, val age: Int)
来源：http://cyu.fengsongda.top

[T09] Kotlin：扩展函数
来源：http://hmn.jinghuilouyu.cn

fun String.exclaim() = this + "!"
来源：http://fns.52xcode.cn

[T10] Kotlin：默认参数
来源：http://kqc.tanke756.top

fun greet(name: String = "World") = "Hi $name"
来源：http://lvr.hnqzz.top

[T11] Kotlin：协程
来源：http://uwq.ivvv.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://xuc.gaohongyu789.top

[T12] Kotlin：解构声明
来源：http://rha.pycfn.com

val (a, b) = Pair(1, 2)
来源：http://bjq.zhengqikj.top

[T13] Kotlin：只读 Map
来源：http://qkh.fktsv.cn

val m = mapOf("a" to 1)
来源：http://drz.zhijiandao.cn

[T14] Kotlin：循环
来源：http://zbj.yj20258888.top

for (i in 1..10) println(i)
来源：http://ltj.ivvv.top

[T15] Kotlin：接口
来源：http://roo.pycfn.com

interface Shape { fun area(): Double }
来源：http://xqj.jlsjyb.cn

[T16] Swift：Hello World
来源：http://bbd.andypj.xyz

print("Hello")
来源：http://eoz.fengsongda.top

[T17] Swift：变量与常量
来源：http://mbz.cucudq.cn

var a = 1;  let b = 2
来源：http://dph.shzxlz.cn

[T18] Swift：字符串插值
来源：http://hjn.vehdjk.com

"值: \(b)"
来源：http://xfz.guannengcc.top

[T19] Swift：可选绑定
来源：http://lpa.zhixingplan.top

if let n = opt { print(n) }
来源：http://azl.jyoumei.cn

[T20] Swift：数组操作
来源：http://krn.nwbrower.top

var a = [1, 2, 3];  a.append(4)
来源：http://wqx.yonumen.top

[T21] Swift：遍历
来源：http://uhg.gogol.net.cn

for x in a { print(x) }
来源：http://hbo.yj202588.top

[T22] Swift：字典
来源：http://pkz.hysaishi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xqo.smart0.xyz

[T23] Swift：函数
来源：http://tvk.hnxiangtu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zss.zhaomingkeji.xyz

[T24] Swift：闭包
来源：http://yjc.ydjk.org.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://coj.ywan-chungtsiang.top

[T25] Swift：结构体
来源：http://bup.ehwqpu.com

struct P { var x: Int }
来源：http://yim.haohaochexian.top

[T26] Swift：类与重写
来源：http://oqg.yj20258888.top

class A: Base { override func f() {} }
来源：http://jok.xingfuxueyuan.xyz

[T27] Swift：错误处理
来源：http://nwj.fengsongda.top

do { try f() } catch { print(error) }
来源：http://csv.gotoacloud.top

[T28] Swift：枚举
来源：http://mbg.hnqzz.top

enum Color { case red, green }
来源：http://epf.zhaomingkeji.xyz

[T29] Swift：guard 提前返回
来源：http://ptu.gotoacloud.top

guard let x = opt else { return }
来源：http://dcy.ydzc1.top

[T30] Swift：协议
来源：http://gje.nanxuanxn.top

protocol Shape { func area() -> Double }
来源：http://ije.9152youxi.cn

[T31] Lua：Hello World
来源：http://lfz.andypj.xyz

print("Hello")
来源：http://mew.cucudq.cn

[T32] Lua：局部变量
来源：http://gxk.ppjwa.cn

local a = 1
来源：http://rcn.ctjpmb.com

[T33] Lua：表（数组）
来源：http://apb.tarul.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hrr.yangfankeji.com

[T34] Lua：遍历表
来源：http://cmj.52xcode.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://itj.iojbl.cn

[T35] Lua：字典表
来源：http://bmb.nanxuanxn.top

local d = { a = 1 };  d.b = 2
来源：http://kpg.jlsjyb.cn

[T36] Lua：函数
来源：http://uyd.zdqjudy.top

function add(a, b) return a + b end
来源：http://zks.chenjidiqi.icu

[T37] Lua：字符串拼接
来源：http://dtz.jinqigfzy.top

"a" .. "b"
来源：http://nhz.yonumen.top

[T38] Lua：条件
来源：http://tgs.cqqwz.cn

if x > 0 then print("正") end
来源：http://ksr.fengsongda.top

[T39] Lua：模式匹配
来源：http://rmf.shuidangran.top

string.find(s, "%d+")
来源：http://kuc.yonumen.top

[T40] Lua：元表
来源：http://zjw.dianchejie.cn

setmetatable({}, { __index = base })
来源：http://ffz.tian-w.cn

[T41] Perl：Hello World
来源：http://kwl.havefunace.top

print "Hello\n";
来源：http://xdd.iojbl.cn

[T42] Perl：变量类型
来源：http://gnb.epnwcf.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vwn.nwbrower.top

[T43] Perl：字符串插值
来源：http://xmg.hnqzz.top

"值: $a"
来源：http://osw.shzxlz.cn

[T44] Perl：条件
来源：http://chg.hywenlv.cn

if ($a > 0) { print "正"; }
来源：http://eyv.dianchejie.cn

[T45] Perl：数组遍历
来源：http://ccr.mhx1999.top

for my $x (@arr) { print $x; }
来源：http://ljm.fzhhl.top

[T46] Perl：哈希操作
来源：http://pnb.shanyushiyangkeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qzm.nanxuanxn.top

[T47] Perl：正则捕获
来源：http://nuk.316326.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://ewl.aibaodan.cn

[T48] Perl：正则替换
来源：http://owj.xylfe.cn

$s =~ s/old/new/g;
来源：http://ilw.yangfankeji.com

[T49] Perl：函数
来源：http://dud.haohaochexian.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ldx.cdnleiting.top

[T50] Perl：逐行读文件
来源：http://exs.aizwys.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ynq.xziqi.cn

while (my $line = <$fh>) { print $line; }
来源：http://eba.yangfankeji.com

[T51] Scala：Hello World
来源：http://wzs.fzhhl.top

println("Hello")
来源：http://uap.nanxuanxn.top

[T52] Scala：变量
来源：http://bgj.aizwys.cn

val a = 1;  var b = 2
来源：http://esx.0kj1m.cn

[T53] Scala：字符串插值
来源：http://teg.shuidangran.top

s"值: $b"
来源：http://esj.cheryme.top

[T54] Scala：集合映射
来源：http://gfw.yj20258888.top

List(1, 2, 3).map(_ * 2)
来源：http://bso.chenjidiqi.icu

[T55] Scala：集合过滤
来源：http://mxt.yj20258.top

List(1, 2, 3).filter(_ > 1)
来源：http://trv.bbcook.cn

[T56] Scala：样例类
来源：http://vpq.fzhhl.top

case class User(name: String, age: Int)
来源：http://jbe.jianghu66.top

[T57] Scala：模式匹配
来源：http://zbn.jinqigfzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://hvj.ppjwa.cn

[T58] Scala：函数定义
来源：http://hlx.cqqwz.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hkh.yanxiufei.cn

[T59] Scala：循环
来源：http://hfk.0kj1m.cn

for (i <- 1 to 10) println(i)
来源：http://rjx.c1oappe.top

[T60] Scala：折叠
来源：http://agi.cqqwz.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gbj.0kj1m.cn

================================================================================
来源：http://wls.shanyushiyangkeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cdp.uphjek.com

================================================================================
来源：http://jbl.hnxiangtu.top

[U01] Py：创建虚拟环境
来源：http://yds.cucudq.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jhz.iojbl.cn

[U02] Py：导出 / 安装依赖
来源：http://pgf.guowangkeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jyf.pengpengdd.cyou


<!-- 参考信息 -->