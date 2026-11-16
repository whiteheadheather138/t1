代发 wailian999

free -h;  ps aux | grep nginx
来源：http://mme.hongshengwenyu.top

[R64] 结束进程
来源：http://hre.hnxiangtu.top

kill -9 $(pgrep -f app.py)
来源：http://lur.zycfv.cn

[R65] 查看端口占用
来源：http://kki.pengpengdd.cyou

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://suf.gogol.net.cn

[R66] 定时任务
来源：http://ozi.havefunace.top

crontab -e;  crontab -l
来源：http://zri.yueranfly.top

[R67] 生成随机十六进制串
来源：http://wsf.iojbl.cn

openssl rand -hex 16
来源：http://mew.cashguo.top

[R68] 计算文件校验值
来源：http://efi.dianchejie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ddl.iojbl.cn

[R69] 生成随机密码
来源：http://aqg.vehdjk.com

head -c 16 /dev/urandom | base64
来源：http://ksv.quarkkingdee.top

[R70] 时间戳与互转
来源：http://vqg.sxryk.cn

date +%s;  date -d @1700000000
来源：http://crq.yj20258888.top

[R71] 日期格式化
来源：http://bzk.shzxlz.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uru.pycfn.com

[R72] 等待端口就绪
来源：http://lgb.bbcook.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wrr.jinqigufen.top

[R73] 分割大日志
来源：http://pge.feifeiyinyue.top

split -l 1000 big.log part_
来源：http://pbr.9152youxi.cn

[R74] 批量重命名
来源：http://drr.xingfuxueyuan.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pco.shanyushiyangtech.top

[R75] 导出环境变量
来源：http://sny.hnxiangtu.top

export PATH="$HOME/bin:$PATH"
来源：http://tzg.cqqwz.cn

[R76] 使用临时文件
来源：http://tdj.yj20258888.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://msu.jyoumei.cn

[R77] 读取用户输入
来源：http://xju.ydjk.org.cn

read -rp "请输入: " ans
来源：http://xxq.yj20258888.top

[R78] 交互式菜单
来源：http://kpe.hnxiangtu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://tdb.cucudq.cn

[R79] 解析命令行选项
来源：http://flz.yj20258888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lmu.zhiwuduotai.top

[R80] 查看脚本执行耗时
来源：http://oiw.chenlongwang.top

time ./run.sh
来源：http://hvt.tianlin.xyz

================================================================================
来源：http://brw.uphjek.com

S. C / C++ 专题
来源：http://jfn.xziqi.cn

================================================================================
来源：http://kqw.svipenyu.cn

[S01] C：Hello World
来源：http://lum.zhaomingkeji.xyz

#include <stdio.h>
来源：http://sab.jinqigfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ivg.zhijiandao.cn

[S02] C：变量与格式化输出
来源：http://iua.yfazqb.com

int a = 10; printf("%d\n", a);
来源：http://nud.shzxlz.cn

[S03] C：读入整数
来源：http://bhs.hammf.cn

int x; scanf("%d", &x);
来源：http://lsw.hcnkem.com

[S04] C：字符串复制
来源：http://dyw.zycfv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://skc.gogol.net.cn

[S05] C：字符串长度
来源：http://bsj.zhijiandao.cn

strlen(s)
来源：http://ded.havefunace.top

[S06] C：字符串比较
来源：http://ghl.meibo888.top

strcmp(a, b) == 0
来源：http://sbt.sysykeji.top

[S07] C：数组遍历求和
来源：http://dek.316326.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://efv.pengpengdd.cyou

[S08] C：动态内存分配与释放
来源：http://qcf.birdmap.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gpr.sufxvd.cn

[S09] C：结构体定义与初始化
来源：http://bgm.cdnleiting.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://spu.tanke756.top

[S10] C：指针与解引用
来源：http://lzc.jiagoushi.top

int *p = &a;  *p = 5;
来源：http://lyh.jinghuilouyu.cn

[S11] C：逐行读文件
来源：http://ewf.fengsongda.top

FILE *f = fopen("a.txt", "r");
来源：http://zue.hesvh.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rlv.jqgfzy.top

fclose(f);
来源：http://qtj.meibo888.top

[S12] C：写文件
来源：http://yev.wangdashe.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://oyc.feifeiyinyue.top

[S13] C：宏定义
来源：http://cmb.ybcxt.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ive.cdnleiting.top

[S14] C：枚举
来源：http://xcv.cucudq.cn

enum Color { RED, GREEN, BLUE };
来源：http://lib.0kj1m.cn

[S15] C：类型转换
来源：http://fpx.jinqigufen.top

(double) a / b
来源：http://gro.zdbjq.cn

[S16] C：位操作置位
来源：http://rkl.yfazqb.com

x |= (1 << 3);
来源：http://soo.pengpengdd.cyou

[S17] C：安全拼接字符串
来源：http://sqm.uphjek.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wyz.hfpthk.cn

[S18] C：命令行参数
来源：http://tlz.gogol.net.cn

int main(int argc, char **argv)
来源：http://gzw.gzhubu.top

[S19] C：快速排序
来源：http://ufo.yj202588.top

qsort(a, n, sizeof(int), cmp);
来源：http://wlb.cucudq.cn

[S20] C：二分查找
来源：http://yqc.andypj.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://opj.yanxiufei.cn

[S21] C：字符类别判断
来源：http://hrz.mhx1999.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://adw.snrcjt.cn

[S22] C：字符串转数字
来源：http://ach.yonumen.top

atoi("42");  strtod("3.14", NULL);
来源：http://yft.sufxvd.cn

[S23] C：随机数
来源：http://ejr.havefunace.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qyl.zycfv.cn

[S24] C：获取本地时间
来源：http://ucz.smart0.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cuv.jiagoushi.top

[S25] C：内存拷贝
来源：http://igv.zhongyouzk.top

memcpy(dst, src, n);
来源：http://alt.nanxinkj.top

[S26] C：内存清零
来源：http://qhs.jinghuilouyu.cn

memset(a, 0, sizeof a);
来源：http://lfy.hcnkem.com

[S27] C：定义常量
来源：http://dns.zdqjudy.top

const double PI = 3.14159;
来源：http://arh.shzxlz.cn

[S28] C：静态变量
来源：http://mdz.hongshengwenyu.top

static int counter = 0;
来源：http://pel.pengpengdd.cyou

[S29] C：变参函数
来源：http://jkd.zhengqikj.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xei.xuanzx.com

[S30] C：头文件保护
来源：http://kvj.zhengqikj.top

#ifndef X_H
来源：http://mdv.zhixingplan.top

#define X_H
来源：http://olf.bjfxy.top

#endif
来源：http://dwa.dashuyun.cn

[S31] C++：Hello World
来源：http://vll.ehwqpu.com

#include <iostream>
来源：http://kpn.epnwcf.com

int main() { std::cout << "Hello\n"; }
来源：http://quz.shangyingyoupin.top

[S32] C++：字符串
来源：http://bcd.nanxinkj.top

std::string s = "hi";  s += "!";
来源：http://xzw.fengsongda.top

[S33] C++：vector 增删
来源：http://ygb.hnxiangtu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://shk.gotoacloud.top

[S34] C++：遍历 vector
来源：http://zus.jqgufenzy.top

for (auto &x : v) { std::cout << x; }
来源：http://pry.wangshuangyany.cn

[S35] C++：map
来源：http://nqy.tanke756.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nlz.52xcode.cn

[S36] C++：unordered_map
来源：http://szt.jiagoushi.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mwd.shanyushiyangtech.top

[S37] C++：set
来源：http://xcr.epnwcf.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kyj.bbcook.cn

[S38] C++：排序
来源：http://tze.shzxlz.cn

std::sort(v.begin(), v.end());
来源：http://bfg.hongshengwenyu.top

[S39] C++：自定义比较器排序
来源：http://uvs.birdmap.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tao.haohaochexian.top

[S40] C++：查找元素
来源：http://uvg.shzxlz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uaa.feifeiyinyue.top

[S41] C++：类与构造函数
来源：http://qph.yvedp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nzo.c1oappe.top

[S42] C++：继承与虚函数
来源：http://yfl.shanyushiyangtech.top

class B : public Base { public: void f() override {} };
来源：http://cax.zhengqikj.top

[S43] C++：智能指针
来源：http://ezv.zdbjq.cn

auto p = std::make_unique<int>(5);
来源：http://twm.mhx1999.top

[S44] C++：引用传参
来源：http://adv.hywenlv.cn

void inc(int &x) { ++x; }
来源：http://qwe.yuanzhike.top

[S45] C++：lambda
来源：http://ppt.fengsongda.top

auto add = [](int a, int b) { return a + b; };
来源：http://drq.jianghu66.top

[S46] C++：函数模板
来源：http://pny.hesvh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sqv.hongshengwenyu.top

[S47] C++：结构化绑定遍历
来源：http://sxu.hfpthk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bii.hcnkem.com

[S48] C++：逐行读文件
来源：http://sju.iojbl.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xgs.yfazqb.com

while (std::getline(in, line)) { }
来源：http://rqo.aibaodan.cn

[S49] C++：写文件
来源：http://fwt.xziqi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fld.zhixingplan.top

[S50] C++：格式化数字
来源：http://obk.gzhubu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://scj.zhaomingkeji.xyz

[S51] C++：显式类型转换
来源：http://acl.cucudq.cn

static_cast<double>(a) / b
来源：http://xok.zhijiandao.cn

[S52] C++：const 与 noexcept
来源：http://jtj.316326.xyz

int size() const noexcept { return n_; }
来源：http://tai.dashuyun.cn

[S53] C++：移动语义
来源：http://twf.xuetiantiany.cn

std::vector<int> w = std::move(v);
来源：http://mxc.ehwqpu.com

[S54] C++：异常处理
来源：http://rty.shanyushiyangtech.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mlu.zhongyouzk.top

[S55] C++：结构化绑定
来源：http://tpy.redwolf501.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jvi.cheryme.top

[S56] C++：optional
来源：http://ubb.tian-w.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fqr.havefunace.top

[S57] C++：编译期常量
来源：http://nqp.aibaodan.cn

constexpr int N = 10;
来源：http://yfd.ivvv.top

[S58] C++：命名空间
来源：http://ire.zdbjq.cn

namespace ns { int f() { return 1; } }
来源：http://lgd.xziqi.cn

[S59] C++：静态断言
来源：http://vyz.ppjwa.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nif.redwolf501.top

[S60] C++：遍历并删除元素
来源：http://dqe.gotoacloud.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oin.ywan-chungtsiang.top

================================================================================
来源：http://vye.9152youxi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://krj.zdbjq.cn

================================================================================
来源：http://kvv.hongshengwenyu.top

[T01] Kotlin：Hello World
来源：http://wha.shanyushiyangtech.top

println("Hello")
来源：http://jxc.wangshuangyany.cn

[T02] Kotlin：变量
来源：http://blp.sysykeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wvb.yvedp.cn

[T03] Kotlin：字符串模板
来源：http://pba.aibaodan.cn

"值: $b"
来源：http://ntw.haohaochexian.top

[T04] Kotlin：空安全
来源：http://ynz.nanxinkj.top

val n: String? = null;  n?.length
来源：http://ksj.fktsv.cn

[T05] Kotlin：when 表达式
来源：http://swu.shuidangran.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://thg.hfpthk.cn

[T06] Kotlin：集合映射
来源：http://bwg.chenjidiqi.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://aov.wangdashe.top

[T07] Kotlin：集合过滤
来源：http://pwq.zhixingplan.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ufd.smart0.xyz

[T08] Kotlin：数据类
来源：http://azt.zhongyouzk.top

data class User(val name: String, val age: Int)
来源：http://xlk.zhixingplan.top

[T09] Kotlin：扩展函数
来源：http://rko.bbcook.cn

fun String.exclaim() = this + "!"
来源：http://jal.zhiwuduotai.top

[T10] Kotlin：默认参数
来源：http://mel.hesvh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tkz.gotoacloud.top

[T11] Kotlin：协程
来源：http://out.yvedp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://crw.zhoulong.xyz

[T12] Kotlin：解构声明
来源：http://qye.hcnkem.com

val (a, b) = Pair(1, 2)
来源：http://kdt.daria6918.cn

[T13] Kotlin：只读 Map
来源：http://ybi.redwolf501.top

val m = mapOf("a" to 1)
来源：http://lwp.yj20258.top

[T14] Kotlin：循环
来源：http://aeg.jinyuanbaomall.cn

for (i in 1..10) println(i)
来源：http://shq.jinyuanbaomall.cn

[T15] Kotlin：接口
来源：http://ldf.shanyushiyangtech.top

interface Shape { fun area(): Double }
来源：http://mjx.fanxiaobao.xyz

[T16] Swift：Hello World
来源：http://mdj.xingfuxueyuan.xyz

print("Hello")
来源：http://kzy.xuetiantiany.cn

[T17] Swift：变量与常量
来源：http://fuc.sufxvd.cn

var a = 1;  let b = 2
来源：http://vph.zhongyouzk.top

[T18] Swift：字符串插值
来源：http://zkk.xuetiantiany.cn

"值: \(b)"
来源：http://vnp.guannengcc.top

[T19] Swift：可选绑定
来源：http://ghn.vqdsnc.cn

if let n = opt { print(n) }
来源：http://tqs.ctjpmb.com

[T20] Swift：数组操作
来源：http://idt.yonumen.top

var a = [1, 2, 3];  a.append(4)
来源：http://rge.shangyingyoupin.top

[T21] Swift：遍历
来源：http://iwf.bjfxy.top

for x in a { print(x) }
来源：http://jdf.yueranfly.top

[T22] Swift：字典
来源：http://xmh.tianlin.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://lrw.svipenyu.cn

[T23] Swift：函数
来源：http://okx.chenjidiqi.icu

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ueg.jinyuanbaomall.cn

[T24] Swift：闭包
来源：http://mby.pycfn.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://trg.havefunace.top

[T25] Swift：结构体
来源：http://tvb.feifeiyinyue.top

struct P { var x: Int }
来源：http://mds.gaohongyu789.top

[T26] Swift：类与重写
来源：http://jjh.havefunace.top

class A: Base { override func f() {} }
来源：http://srp.chenjidiqi.icu

[T27] Swift：错误处理
来源：http://onj.xylfe.cn

do { try f() } catch { print(error) }
来源：http://ync.bjfxy.top

[T28] Swift：枚举
来源：http://jyq.hnqzz.top

enum Color { case red, green }
来源：http://fzc.xuanzx.com

[T29] Swift：guard 提前返回
来源：http://rre.birdmap.top

guard let x = opt else { return }
来源：http://lqr.wangshuangyany.cn

[T30] Swift：协议
来源：http://gsy.pengpengdd.cyou

protocol Shape { func area() -> Double }
来源：http://qpp.zycfv.cn

[T31] Lua：Hello World
来源：http://wvn.ivvv.top

print("Hello")
来源：http://dka.fzhhl.top

[T32] Lua：局部变量
来源：http://xit.zhoulong.xyz

local a = 1
来源：http://joj.haohaochexian.top

[T33] Lua：表（数组）
来源：http://xnq.fktsv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lga.chenzaomai.com

[T34] Lua：遍历表
来源：http://gpb.zycfv.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://raj.xinyue.icu

[T35] Lua：字典表
来源：http://vju.tarul.cn

local d = { a = 1 };  d.b = 2
来源：http://beq.birdmap.top

[T36] Lua：函数
来源：http://myw.shanyushiyangkeji.top

function add(a, b) return a + b end
来源：http://iwb.aibaodan.cn

[T37] Lua：字符串拼接
来源：http://gcj.jinghuilouyu.cn

"a" .. "b"
来源：http://asl.shanyushiyangtech.top

[T38] Lua：条件
来源：http://das.tanke756.top

if x > 0 then print("正") end
来源：http://lzt.gogol.net.cn

[T39] Lua：模式匹配
来源：http://iwt.fzhhl.top

string.find(s, "%d+")
来源：http://sit.fengsongda.top

[T40] Lua：元表
来源：http://ona.birdmap.top

setmetatable({}, { __index = base })
来源：http://sea.quarkkingdee.top

[T41] Perl：Hello World
来源：http://sre.xylfe.cn

print "Hello\n";
来源：http://fsg.ydjk.org.cn

[T42] Perl：变量类型
来源：http://qvb.snrcjt.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://etz.ehwqpu.com

[T43] Perl：字符串插值
来源：http://qek.hnxiangtu.top

"值: $a"
来源：http://xzz.epnwcf.com

[T44] Perl：条件
来源：http://aqq.ydzc1.top

if ($a > 0) { print "正"; }
来源：http://fcr.ivvv.top

[T45] Perl：数组遍历
来源：http://com.jqgufenzy.top

for my $x (@arr) { print $x; }
来源：http://mjd.fanxiaobao.xyz

[T46] Perl：哈希操作
来源：http://jzn.zhixingplan.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yyn.ybcxt.top

[T47] Perl：正则捕获
来源：http://joy.tian-w.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qes.cucudq.cn

[T48] Perl：正则替换
来源：http://crb.hcnkem.com

$s =~ s/old/new/g;
来源：http://mno.ydjk.org.cn

[T49] Perl：函数
来源：http://uel.wangshuangyany.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wgo.sjlbkw.cn

[T50] Perl：逐行读文件
来源：http://vrx.tian-w.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://blj.jianghu66.top

while (my $line = <$fh>) { print $line; }
来源：http://xis.kuanghao11.cn

[T51] Scala：Hello World
来源：http://rdz.chenzaomai.com

println("Hello")
来源：http://aus.aizwys.cn

[T52] Scala：变量
来源：http://byj.fzhhl.top

val a = 1;  var b = 2
来源：http://klh.wangshuangyany.cn

[T53] Scala：字符串插值
来源：http://fpq.hesvh.cn

s"值: $b"
来源：http://tiy.pycfn.com

[T54] Scala：集合映射
来源：http://mzb.fehbvm.com

List(1, 2, 3).map(_ * 2)
来源：http://dmp.guannengcc.top

[T55] Scala：集合过滤
来源：http://jls.havefunace.top

List(1, 2, 3).filter(_ > 1)
来源：http://nyl.iojbl.cn

[T56] Scala：样例类
来源：http://mln.bbcook.cn

case class User(name: String, age: Int)
来源：http://rcj.cdnleiting.top

[T57] Scala：模式匹配
来源：http://obd.yueranfly.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://miw.c1oappe.top

[T58] Scala：函数定义
来源：http://ymz.ehwqpu.com

def add(a: Int, b: Int): Int = a + b
来源：http://xuz.daxiang520.top

[T59] Scala：循环
来源：http://brd.hnqzz.top

for (i <- 1 to 10) println(i)
来源：http://hgc.yj202588.top

[T60] Scala：折叠
来源：http://irl.ydjk.org.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://itr.epnwcf.com

================================================================================
来源：http://ifv.guannengcc.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kii.gogol.net.cn

================================================================================
来源：http://agf.xuanzx.com

[U01] Py：创建虚拟环境
来源：http://nhy.ehwqpu.com

python -m venv .venv && source .venv/bin/activate
来源：http://ujf.yj202588.top

[U02] Py：导出 / 安装依赖
来源：http://xvf.jqgufenzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xgq.hongshengwenyu.top

[U03] Py：加载 .env 配置
来源：http://bhb.dashuyun.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://igd.shzxlz.cn

[U04] Py：变量调试打印
来源：http://jkt.yuxming.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gmc.yj20258888.top


<!-- 参考信息 -->