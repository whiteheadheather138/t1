代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jis.zycfv.cn

[R60] 只看 HTTP 状态码
来源：http://yqm.vehdjk.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gdt.ctjpmb.com

[R61] 磁盘占用
来源：http://woq.zdbjq.cn

df -h;  du -sh *
来源：http://ffp.zhixingplan.top

[R62] 找最占空间的文件
来源：http://qyo.gotoacloud.top

du -ah . | sort -rh | head -10
来源：http://obu.yj20258888.top

[R63] 内存与进程
来源：http://gni.vqdsnc.cn

free -h;  ps aux | grep nginx
来源：http://hfk.hcnkem.com

[R64] 结束进程
来源：http://hrt.jqgufenzy.top

kill -9 $(pgrep -f app.py)
来源：http://nxb.yfazqb.com

[R65] 查看端口占用
来源：http://tni.zhijiandao.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bwn.gogol.net.cn

[R66] 定时任务
来源：http://xcd.yueranfly.top

crontab -e;  crontab -l
来源：http://ode.sxryk.cn

[R67] 生成随机十六进制串
来源：http://phw.jinqigufen.top

openssl rand -hex 16
来源：http://fvx.meibo888.top

[R68] 计算文件校验值
来源：http://twg.birdmap.top

sha256sum a.txt;  md5sum a.txt
来源：http://wwf.haohaochexian.top

[R69] 生成随机密码
来源：http://zrb.tian-w.cn

head -c 16 /dev/urandom | base64
来源：http://xcy.chenjidiqi.icu

[R70] 时间戳与互转
来源：http://dbr.zdbjq.cn

date +%s;  date -d @1700000000
来源：http://hzv.zhijiandao.cn

[R71] 日期格式化
来源：http://xvu.feifeiyinyue.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://kxx.zhengqikj.top

[R72] 等待端口就绪
来源：http://egk.ydjk.org.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mun.smart0.xyz

[R73] 分割大日志
来源：http://irq.xuanzx.com

split -l 1000 big.log part_
来源：http://woy.gzhubu.top

[R74] 批量重命名
来源：http://kqy.nanxuanxn.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vit.vqdsnc.cn

[R75] 导出环境变量
来源：http://vfz.ywan-chungtsiang.top

export PATH="$HOME/bin:$PATH"
来源：http://jjg.jinqigfzy.top

[R76] 使用临时文件
来源：http://pnw.ivvv.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vie.epnwcf.com

[R77] 读取用户输入
来源：http://bri.ctjpmb.com

read -rp "请输入: " ans
来源：http://gun.jinyuanbaomall.cn

[R78] 交互式菜单
来源：http://efs.gotoacloud.top

select opt in a b c; do echo "$opt"; break; done
来源：http://jko.sysykeji.top

[R79] 解析命令行选项
来源：http://ftk.aibaodan.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://war.shzxlz.cn

[R80] 查看脚本执行耗时
来源：http://kgw.jiagoushi.top

time ./run.sh
来源：http://uww.guowangkeji.top

================================================================================
来源：http://uop.hongshengwenyu.top

S. C / C++ 专题
来源：http://ncw.bjfxy.top

================================================================================
来源：http://bvm.ydzc1.top

[S01] C：Hello World
来源：http://tpl.ivvv.top

#include <stdio.h>
来源：http://lyd.zdqjudy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://lcf.hongshengwenyu.top

[S02] C：变量与格式化输出
来源：http://qiy.pycfn.com

int a = 10; printf("%d\n", a);
来源：http://cqo.shzxlz.cn

[S03] C：读入整数
来源：http://bvg.nanxinkj.top

int x; scanf("%d", &x);
来源：http://wpv.wangdashe.top

[S04] C：字符串复制
来源：http://dcx.xinyue.icu

char dst[32]; strcpy(dst, "hi");
来源：http://ngy.hysaishi.cn

[S05] C：字符串长度
来源：http://edj.havefunace.top

strlen(s)
来源：http://cvu.jqgufenzy.top

[S06] C：字符串比较
来源：http://uia.vqdsnc.cn

strcmp(a, b) == 0
来源：http://kph.yanxiufei.cn

[S07] C：数组遍历求和
来源：http://tck.hongshengwenyu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vez.nanxuanxn.top

[S08] C：动态内存分配与释放
来源：http://bml.zhiwuduotai.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yvv.aizwys.cn

[S09] C：结构体定义与初始化
来源：http://gpb.jiagoushi.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://anq.sysykeji.top

[S10] C：指针与解引用
来源：http://eip.wangdashe.top

int *p = &a;  *p = 5;
来源：http://kci.gzhubu.top

[S11] C：逐行读文件
来源：http://ouv.cheryme.top

FILE *f = fopen("a.txt", "r");
来源：http://pxp.shanyushiyangkeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://nrz.uphjek.com

fclose(f);
来源：http://ypb.shzxlz.cn

[S12] C：写文件
来源：http://ete.c1oappe.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hcs.hongshengwenyu.top

[S13] C：宏定义
来源：http://vmr.jianghu66.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gep.kuanghao11.cn

[S14] C：枚举
来源：http://yrw.daria6918.cn

enum Color { RED, GREEN, BLUE };
来源：http://yez.chenzaomai.com

[S15] C：类型转换
来源：http://ery.yvedp.cn

(double) a / b
来源：http://dno.zhijiandao.cn

[S16] C：位操作置位
来源：http://lok.zhoulong.xyz

x |= (1 << 3);
来源：http://piq.xuetiantiany.cn

[S17] C：安全拼接字符串
来源：http://znp.ydjk.org.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://chl.yangfankeji.com

[S18] C：命令行参数
来源：http://sli.yongpay.top

int main(int argc, char **argv)
来源：http://mmu.tanke756.top

[S19] C：快速排序
来源：http://mdh.0kj1m.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ewy.fengsongda.top

[S20] C：二分查找
来源：http://rmo.ctjpmb.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kcm.sufxvd.cn

[S21] C：字符类别判断
来源：http://cbi.jqgufenzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gjr.jqgufenzy.top

[S22] C：字符串转数字
来源：http://qtj.chenlongwang.top

atoi("42");  strtod("3.14", NULL);
来源：http://hav.xuetiantiany.cn

[S23] C：随机数
来源：http://hrf.fzhhl.top

srand(time(NULL));  int r = rand() % 100;
来源：http://pfi.fktsv.cn

[S24] C：获取本地时间
来源：http://otf.hysaishi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ndl.bjfxy.top

[S25] C：内存拷贝
来源：http://zaw.hfpthk.cn

memcpy(dst, src, n);
来源：http://cln.tanke756.top

[S26] C：内存清零
来源：http://oog.daxiang520.top

memset(a, 0, sizeof a);
来源：http://zos.zhixingplan.top

[S27] C：定义常量
来源：http://bhe.andypj.xyz

const double PI = 3.14159;
来源：http://geh.xuetiantiany.cn

[S28] C：静态变量
来源：http://tye.hywenlv.cn

static int counter = 0;
来源：http://dvf.jyoumei.cn

[S29] C：变参函数
来源：http://ppu.jinyuanbaomall.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://smm.epnwcf.com

[S30] C：头文件保护
来源：http://kdb.havefunace.top

#ifndef X_H
来源：http://lzg.jiagoushi.top

#define X_H
来源：http://fjs.shzxlz.cn

#endif
来源：http://yvk.xingfuxueyuan.xyz

[S31] C++：Hello World
来源：http://mkg.havefunace.top

#include <iostream>
来源：http://pzb.hnxiangtu.top

int main() { std::cout << "Hello\n"; }
来源：http://nzf.xziqi.cn

[S32] C++：字符串
来源：http://dae.cqqwz.cn

std::string s = "hi";  s += "!";
来源：http://yeg.havefunace.top

[S33] C++：vector 增删
来源：http://uam.zdqjudy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://har.bbcook.cn

[S34] C++：遍历 vector
来源：http://bai.sufxvd.cn

for (auto &x : v) { std::cout << x; }
来源：http://fiy.jiagoushi.top

[S35] C++：map
来源：http://kdq.feifeiyinyue.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lpu.jinyuanbaomall.cn

[S36] C++：unordered_map
来源：http://gki.yueranfly.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dzv.smart0.xyz

[S37] C++：set
来源：http://ctj.bbcook.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ekw.zdbjq.cn

[S38] C++：排序
来源：http://czu.fehbvm.com

std::sort(v.begin(), v.end());
来源：http://pvp.cqqwz.cn

[S39] C++：自定义比较器排序
来源：http://asr.cashguo.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hbr.zhaomingkeji.xyz

[S40] C++：查找元素
来源：http://ton.guannengcc.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rbi.9152youxi.cn

[S41] C++：类与构造函数
来源：http://zte.tarul.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oid.haohaochexian.top

[S42] C++：继承与虚函数
来源：http://axg.ywan-chungtsiang.top

class B : public Base { public: void f() override {} };
来源：http://ibm.ivvv.top

[S43] C++：智能指针
来源：http://ooi.shanyushiyangtech.top

auto p = std::make_unique<int>(5);
来源：http://ipm.shanyushiyangtech.top

[S44] C++：引用传参
来源：http://czf.xziqi.cn

void inc(int &x) { ++x; }
来源：http://vej.cqqwz.cn

[S45] C++：lambda
来源：http://emq.9152youxi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zjy.aizwys.cn

[S46] C++：函数模板
来源：http://mtn.tianlin.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xpz.yanxiufei.cn

[S47] C++：结构化绑定遍历
来源：http://ufb.zhongyouzk.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dub.hywenlv.cn

[S48] C++：逐行读文件
来源：http://uqp.yuxming.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xdj.yvedp.cn

while (std::getline(in, line)) { }
来源：http://vbn.zhoulong.xyz

[S49] C++：写文件
来源：http://osx.chenjidiqi.icu

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jca.pycfn.com

[S50] C++：格式化数字
来源：http://lxk.c1oappe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sra.hnqzz.top

[S51] C++：显式类型转换
来源：http://jts.zhiwuduotai.top

static_cast<double>(a) / b
来源：http://glr.gzhubu.top

[S52] C++：const 与 noexcept
来源：http://lny.hnxiangtu.top

int size() const noexcept { return n_; }
来源：http://kyf.zhixingplan.top

[S53] C++：移动语义
来源：http://yae.cdnleiting.top

std::vector<int> w = std::move(v);
来源：http://uqp.chenlongwang.top

[S54] C++：异常处理
来源：http://tgy.kuanghao11.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gha.jinyuanbaomall.cn

[S55] C++：结构化绑定
来源：http://uek.chenjidiqi.icu

auto [a, b] = std::make_pair(1, 2);
来源：http://vgg.hcnkem.com

[S56] C++：optional
来源：http://gcd.tarul.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pwd.yuanzhike.top

[S57] C++：编译期常量
来源：http://ifu.gotoacloud.top

constexpr int N = 10;
来源：http://eer.zhoulong.xyz

[S58] C++：命名空间
来源：http://rra.fktsv.cn

namespace ns { int f() { return 1; } }
来源：http://rhv.jinqigufen.top

[S59] C++：静态断言
来源：http://tep.yj202588.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mhs.fzhhl.top

[S60] C++：遍历并删除元素
来源：http://puy.shzxlz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ymv.wangshuangyany.cn

================================================================================
来源：http://bxc.jqgfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lrk.andypj.xyz

================================================================================
来源：http://uvx.xuanzx.com

[T01] Kotlin：Hello World
来源：http://pxu.svipenyu.cn

println("Hello")
来源：http://wwq.ywan-chungtsiang.top

[T02] Kotlin：变量
来源：http://ewz.yj20258.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nkt.jqgufenzy.top

[T03] Kotlin：字符串模板
来源：http://wjx.hammf.cn

"值: $b"
来源：http://lew.shzxlz.cn

[T04] Kotlin：空安全
来源：http://pdi.fanxiaobao.xyz

val n: String? = null;  n?.length
来源：http://fxb.daxiang520.top

[T05] Kotlin：when 表达式
来源：http://fmw.sufxvd.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pyx.guowangkeji.top

[T06] Kotlin：集合映射
来源：http://dru.ybcxt.top

listOf(1, 2, 3).map { it * 2 }
来源：http://msl.jinqigufen.top

[T07] Kotlin：集合过滤
来源：http://dpg.ybcxt.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://zdw.wangdashe.top

[T08] Kotlin：数据类
来源：http://tho.aibaodan.cn

data class User(val name: String, val age: Int)
来源：http://atu.yanxiufei.cn

[T09] Kotlin：扩展函数
来源：http://bng.jiagoushi.top

fun String.exclaim() = this + "!"
来源：http://uvv.gogol.net.cn

[T10] Kotlin：默认参数
来源：http://umm.yfazqb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://lzz.sweek.top

[T11] Kotlin：协程
来源：http://dim.nwbrower.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://giz.shzxlz.cn

[T12] Kotlin：解构声明
来源：http://nrn.hcnkem.com

val (a, b) = Pair(1, 2)
来源：http://gfd.chenlongwang.top

[T13] Kotlin：只读 Map
来源：http://exv.zhengqikj.top

val m = mapOf("a" to 1)
来源：http://ynd.sufxvd.cn

[T14] Kotlin：循环
来源：http://kbo.xuanzx.com

for (i in 1..10) println(i)
来源：http://aku.daria6918.cn

[T15] Kotlin：接口
来源：http://sai.jinghuilouyu.cn

interface Shape { fun area(): Double }
来源：http://yre.yanxiufei.cn

[T16] Swift：Hello World
来源：http://bzq.hywenlv.cn

print("Hello")
来源：http://aqh.shzxlz.cn

[T17] Swift：变量与常量
来源：http://oci.jiagoushi.top

var a = 1;  let b = 2
来源：http://atq.52xcode.cn

[T18] Swift：字符串插值
来源：http://kmn.guannengcc.top

"值: \(b)"
来源：http://ilg.jinqigfzy.top

[T19] Swift：可选绑定
来源：http://xzf.iojbl.cn

if let n = opt { print(n) }
来源：http://faj.hysaishi.cn

[T20] Swift：数组操作
来源：http://zvt.zhixingplan.top

var a = [1, 2, 3];  a.append(4)
来源：http://txc.jinghuilouyu.cn

[T21] Swift：遍历
来源：http://inb.zhixingplan.top

for x in a { print(x) }
来源：http://ais.jqgufenzy.top

[T22] Swift：字典
来源：http://gzf.hnxiangtu.top

var d = ["a": 1];  d["b"] = 2
来源：http://rhb.shangyingyoupin.top

[T23] Swift：函数
来源：http://idm.daxiang520.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pjh.yj20258.top

[T24] Swift：闭包
来源：http://xcf.shzxlz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fps.hesvh.cn

[T25] Swift：结构体
来源：http://sjb.sweek.top

struct P { var x: Int }
来源：http://oss.dianchejie.cn

[T26] Swift：类与重写
来源：http://few.ydzc1.top

class A: Base { override func f() {} }
来源：http://zwl.shuidangran.top

[T27] Swift：错误处理
来源：http://tsk.zhoulong.xyz

do { try f() } catch { print(error) }
来源：http://off.kuanghao11.cn

[T28] Swift：枚举
来源：http://mdo.feifeiyinyue.top

enum Color { case red, green }
来源：http://nto.andypj.xyz

[T29] Swift：guard 提前返回
来源：http://oyr.epnwcf.com

guard let x = opt else { return }
来源：http://owl.ywan-chungtsiang.top

[T30] Swift：协议
来源：http://hgd.yuanzhike.top

protocol Shape { func area() -> Double }
来源：http://vkm.c1oappe.top

[T31] Lua：Hello World
来源：http://xoo.xingfuxueyuan.xyz

print("Hello")
来源：http://esd.epnwcf.com

[T32] Lua：局部变量
来源：http://mxg.epnwcf.com

local a = 1
来源：http://vkm.jlsjyb.cn

[T33] Lua：表（数组）
来源：http://csh.gzhubu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kzl.xuetiantiany.cn

[T34] Lua：遍历表
来源：http://ujj.jianghu66.top

for i, v in ipairs(t) do print(i, v) end
来源：http://cgg.ctjpmb.com

[T35] Lua：字典表
来源：http://nnx.svipenyu.cn

local d = { a = 1 };  d.b = 2
来源：http://obx.shangyingyoupin.top

[T36] Lua：函数
来源：http://occ.9152youxi.cn

function add(a, b) return a + b end
来源：http://ckv.fktsv.cn

[T37] Lua：字符串拼接
来源：http://ruw.hysaishi.cn

"a" .. "b"
来源：http://kye.iojbl.cn

[T38] Lua：条件
来源：http://gfk.ydzc1.top

if x > 0 then print("正") end
来源：http://cfc.tian-w.cn

[T39] Lua：模式匹配
来源：http://yqk.bjfxy.top

string.find(s, "%d+")
来源：http://lco.hammf.cn

[T40] Lua：元表
来源：http://vez.xuanzx.com

setmetatable({}, { __index = base })
来源：http://irt.yfazqb.com

[T41] Perl：Hello World
来源：http://kaf.yanxiufei.cn

print "Hello\n";
来源：http://cgi.vqdsnc.cn

[T42] Perl：变量类型
来源：http://ftm.yj202588.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mno.ctjpmb.com

[T43] Perl：字符串插值
来源：http://gqy.xziqi.cn

"值: $a"
来源：http://dmp.shzxlz.cn

[T44] Perl：条件
来源：http://jlz.svipenyu.cn

if ($a > 0) { print "正"; }
来源：http://ypx.c1oappe.top

[T45] Perl：数组遍历
来源：http://ilt.jqgfzy.top

for my $x (@arr) { print $x; }
来源：http://hvw.epnwcf.com

[T46] Perl：哈希操作
来源：http://wcr.snrcjt.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vbs.ybcxt.top

[T47] Perl：正则捕获
来源：http://qwr.xingfuxueyuan.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://slq.shuidangran.top

[T48] Perl：正则替换
来源：http://gwy.jqgufenzy.top

$s =~ s/old/new/g;
来源：http://rif.pengpengdd.cyou

[T49] Perl：函数
来源：http://flw.hywenlv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jsr.uphjek.com

[T50] Perl：逐行读文件
来源：http://jkl.havefunace.top

open my $fh, "<", "a.txt" or die $!;
来源：http://zpi.hammf.cn

while (my $line = <$fh>) { print $line; }
来源：http://emd.zhaomingkeji.xyz

[T51] Scala：Hello World
来源：http://jfh.tanke756.top

println("Hello")
来源：http://auy.sweek.top

[T52] Scala：变量
来源：http://crv.yongpay.top

val a = 1;  var b = 2
来源：http://fad.wangshuangyany.cn

[T53] Scala：字符串插值
来源：http://zoz.gotoacloud.top

s"值: $b"
来源：http://lcx.smart0.xyz

[T54] Scala：集合映射
来源：http://hzf.snrcjt.cn

List(1, 2, 3).map(_ * 2)
来源：http://peh.sxryk.cn

[T55] Scala：集合过滤
来源：http://hiv.vqdsnc.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rat.52xcode.cn

[T56] Scala：样例类
来源：http://bqx.0kj1m.cn

case class User(name: String, age: Int)
来源：http://jwk.yonumen.top

[T57] Scala：模式匹配
来源：http://cxx.cashguo.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://xvb.hfpthk.cn

[T58] Scala：函数定义
来源：http://icv.yvedp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xez.gzhubu.top

[T59] Scala：循环
来源：http://drq.wangshuangyany.cn

for (i <- 1 to 10) println(i)
来源：http://mws.sweek.top

[T60] Scala：折叠
来源：http://erk.zhengqikj.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://eoa.yonumen.top

================================================================================
来源：http://iwi.xylfe.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ydh.316326.xyz

================================================================================
来源：http://weq.jinqigfzy.top


<!-- 参考信息 -->