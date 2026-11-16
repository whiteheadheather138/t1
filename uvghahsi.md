代发 wailian999

free -h;  ps aux | grep nginx
来源：http://vuh.nanxuanxn.top

[R64] 结束进程
来源：http://rwq.9152youxi.cn

kill -9 $(pgrep -f app.py)
来源：http://dhf.chenlongwang.top

[R65] 查看端口占用
来源：http://fgl.zhixingplan.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uqd.hysaishi.cn

[R66] 定时任务
来源：http://dgr.andypj.xyz

crontab -e;  crontab -l
来源：http://rqg.vehdjk.com

[R67] 生成随机十六进制串
来源：http://rwo.guowangkeji.top

openssl rand -hex 16
来源：http://enh.gotoacloud.top

[R68] 计算文件校验值
来源：http://ipg.chenjidiqi.icu

sha256sum a.txt;  md5sum a.txt
来源：http://sfm.jinqigfzy.top

[R69] 生成随机密码
来源：http://ibh.haohaochexian.top

head -c 16 /dev/urandom | base64
来源：http://tpo.quarkkingdee.top

[R70] 时间戳与互转
来源：http://qke.zhaomingkeji.xyz

date +%s;  date -d @1700000000
来源：http://hdj.daria6918.cn

[R71] 日期格式化
来源：http://jqm.mhx1999.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jps.vehdjk.com

[R72] 等待端口就绪
来源：http://hxj.yfazqb.com

until nc -z localhost 3306; do sleep 1; done
来源：http://jvb.xuetiantiany.cn

[R73] 分割大日志
来源：http://uce.aizwys.cn

split -l 1000 big.log part_
来源：http://lsq.shanyushiyangtech.top

[R74] 批量重命名
来源：http://bzd.wangshuangyany.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jog.iojbl.cn

[R75] 导出环境变量
来源：http://rgw.meibo888.top

export PATH="$HOME/bin:$PATH"
来源：http://gki.yuxming.cn

[R76] 使用临时文件
来源：http://uen.wangshuangyany.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://czf.sysykeji.top

[R77] 读取用户输入
来源：http://oob.guowangkeji.top

read -rp "请输入: " ans
来源：http://req.guowangkeji.top

[R78] 交互式菜单
来源：http://miu.hnxiangtu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://zdf.0kj1m.cn

[R79] 解析命令行选项
来源：http://bol.ppjwa.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wqa.shanyushiyangtech.top

[R80] 查看脚本执行耗时
来源：http://zek.xziqi.cn

time ./run.sh
来源：http://hon.pycfn.com

================================================================================
来源：http://asv.jiagoushi.top

S. C / C++ 专题
来源：http://qkl.wangdashe.top

================================================================================
来源：http://ght.chenzaomai.com

[S01] C：Hello World
来源：http://pfi.yj20258.top

#include <stdio.h>
来源：http://nno.andypj.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://gkl.xuanzx.com

[S02] C：变量与格式化输出
来源：http://wrt.chenjidiqi.icu

int a = 10; printf("%d\n", a);
来源：http://oyu.ywan-chungtsiang.top

[S03] C：读入整数
来源：http://yrt.xziqi.cn

int x; scanf("%d", &x);
来源：http://uvc.daxiang520.top

[S04] C：字符串复制
来源：http://gly.daxiang520.top

char dst[32]; strcpy(dst, "hi");
来源：http://kzp.9152youxi.cn

[S05] C：字符串长度
来源：http://ehh.jinghuilouyu.cn

strlen(s)
来源：http://dia.havefunace.top

[S06] C：字符串比较
来源：http://lwb.nanxuanxn.top

strcmp(a, b) == 0
来源：http://pxa.gzhubu.top

[S07] C：数组遍历求和
来源：http://voh.zhiwuduotai.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://njp.fzhhl.top

[S08] C：动态内存分配与释放
来源：http://hqt.nanxuanxn.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ren.jinqigufen.top

[S09] C：结构体定义与初始化
来源：http://owo.birdmap.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cqg.tian-w.cn

[S10] C：指针与解引用
来源：http://oeu.yanxiufei.cn

int *p = &a;  *p = 5;
来源：http://qix.nwbrower.top

[S11] C：逐行读文件
来源：http://fsz.zdqjudy.top

FILE *f = fopen("a.txt", "r");
来源：http://nht.hongshengwenyu.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://cjp.tian-w.cn

fclose(f);
来源：http://vdi.ybcxt.top

[S12] C：写文件
来源：http://kgz.tanke756.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gah.havefunace.top

[S13] C：宏定义
来源：http://tpb.hammf.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yzj.guannengcc.top

[S14] C：枚举
来源：http://qph.jyoumei.cn

enum Color { RED, GREEN, BLUE };
来源：http://ovp.zhongyouzk.top

[S15] C：类型转换
来源：http://fcq.0kj1m.cn

(double) a / b
来源：http://mvz.ywan-chungtsiang.top

[S16] C：位操作置位
来源：http://mpz.kuanghao11.cn

x |= (1 << 3);
来源：http://ezz.zhongyouzk.top

[S17] C：安全拼接字符串
来源：http://pon.jqgfzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ojk.xuanzx.com

[S18] C：命令行参数
来源：http://kde.shanyushiyangtech.top

int main(int argc, char **argv)
来源：http://wyi.jinghuilouyu.cn

[S19] C：快速排序
来源：http://wca.yj202588.top

qsort(a, n, sizeof(int), cmp);
来源：http://gya.fzhhl.top

[S20] C：二分查找
来源：http://ccv.xinyue.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pnz.wangshuangyany.cn

[S21] C：字符类别判断
来源：http://vwv.ctjpmb.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://eyc.shzxlz.cn

[S22] C：字符串转数字
来源：http://jdg.zhaomingkeji.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://pfm.zhijiandao.cn

[S23] C：随机数
来源：http://fxc.nwbrower.top

srand(time(NULL));  int r = rand() % 100;
来源：http://edj.zhaomingkeji.xyz

[S24] C：获取本地时间
来源：http://eim.zycfv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qmt.hfpthk.cn

[S25] C：内存拷贝
来源：http://mcy.guowangkeji.top

memcpy(dst, src, n);
来源：http://fsx.yuxming.cn

[S26] C：内存清零
来源：http://hjk.fengsongda.top

memset(a, 0, sizeof a);
来源：http://kys.zhongyouzk.top

[S27] C：定义常量
来源：http://rxe.ehwqpu.com

const double PI = 3.14159;
来源：http://qrn.zycfv.cn

[S28] C：静态变量
来源：http://lfv.xuanzx.com

static int counter = 0;
来源：http://nit.sxryk.cn

[S29] C：变参函数
来源：http://rmc.birdmap.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tmy.52xcode.cn

[S30] C：头文件保护
来源：http://xqo.yj202588.top

#ifndef X_H
来源：http://jtr.quarkkingdee.top

#define X_H
来源：http://rkj.hesvh.cn

#endif
来源：http://qhi.smart0.xyz

[S31] C++：Hello World
来源：http://isx.uphjek.com

#include <iostream>
来源：http://bca.xylfe.cn

int main() { std::cout << "Hello\n"; }
来源：http://qjc.yuanzhike.top

[S32] C++：字符串
来源：http://pnq.zhijiandao.cn

std::string s = "hi";  s += "!";
来源：http://ggn.hammf.cn

[S33] C++：vector 增删
来源：http://euq.gotoacloud.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://roo.daria6918.cn

[S34] C++：遍历 vector
来源：http://ogh.fktsv.cn

for (auto &x : v) { std::cout << x; }
来源：http://soo.shzxlz.cn

[S35] C++：map
来源：http://zre.guannengcc.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xmx.ydzc1.top

[S36] C++：unordered_map
来源：http://mad.jqgfzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zxe.fehbvm.com

[S37] C++：set
来源：http://crn.cqqwz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ofk.fengsongda.top

[S38] C++：排序
来源：http://khn.sufxvd.cn

std::sort(v.begin(), v.end());
来源：http://ooz.havefunace.top

[S39] C++：自定义比较器排序
来源：http://kxn.aizwys.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jnu.9152youxi.cn

[S40] C++：查找元素
来源：http://bgv.xinyue.icu

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uzk.zhoulong.xyz

[S41] C++：类与构造函数
来源：http://eyb.hcnkem.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://spd.aibaodan.cn

[S42] C++：继承与虚函数
来源：http://qil.vqdsnc.cn

class B : public Base { public: void f() override {} };
来源：http://nzk.yj20258888.top

[S43] C++：智能指针
来源：http://gwv.hnqzz.top

auto p = std::make_unique<int>(5);
来源：http://fou.xuanzx.com

[S44] C++：引用传参
来源：http://rcq.chenzaomai.com

void inc(int &x) { ++x; }
来源：http://luv.kuanghao11.cn

[S45] C++：lambda
来源：http://uvk.shuidangran.top

auto add = [](int a, int b) { return a + b; };
来源：http://lqy.hfpthk.cn

[S46] C++：函数模板
来源：http://piq.tanke756.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kos.ppjwa.cn

[S47] C++：结构化绑定遍历
来源：http://bei.dashuyun.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gbe.sysykeji.top

[S48] C++：逐行读文件
来源：http://nug.vqdsnc.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kkh.redwolf501.top

while (std::getline(in, line)) { }
来源：http://wij.guannengcc.top

[S49] C++：写文件
来源：http://isc.xingfuxueyuan.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ces.chenjidiqi.icu

[S50] C++：格式化数字
来源：http://hms.tian-w.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://her.shanyushiyangtech.top

[S51] C++：显式类型转换
来源：http://syb.birdmap.top

static_cast<double>(a) / b
来源：http://qba.zycfv.cn

[S52] C++：const 与 noexcept
来源：http://trh.bbcook.cn

int size() const noexcept { return n_; }
来源：http://tot.yangfankeji.com

[S53] C++：移动语义
来源：http://uml.haohaochexian.top

std::vector<int> w = std::move(v);
来源：http://ybp.wangshuangyany.cn

[S54] C++：异常处理
来源：http://rpa.fanxiaobao.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yde.52xcode.cn

[S55] C++：结构化绑定
来源：http://omz.sjlbkw.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://uhn.chenlongwang.top

[S56] C++：optional
来源：http://gzh.sjlbkw.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ezz.sjlbkw.cn

[S57] C++：编译期常量
来源：http://tmq.sjlbkw.cn

constexpr int N = 10;
来源：http://uqh.zycfv.cn

[S58] C++：命名空间
来源：http://wse.hnqzz.top

namespace ns { int f() { return 1; } }
来源：http://zfv.ctjpmb.com

[S59] C++：静态断言
来源：http://pgy.hnxiangtu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lhj.xylfe.cn

[S60] C++：遍历并删除元素
来源：http://hym.zhengqikj.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qwd.fzhhl.top

================================================================================
来源：http://ixb.jqgufenzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gvk.chenzaomai.com

================================================================================
来源：http://cds.guowangkeji.top

[T01] Kotlin：Hello World
来源：http://dtq.snrcjt.cn

println("Hello")
来源：http://teh.yueranfly.top

[T02] Kotlin：变量
来源：http://fdn.yongpay.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zmi.c1oappe.top

[T03] Kotlin：字符串模板
来源：http://ulj.jyoumei.cn

"值: $b"
来源：http://ivg.nanxuanxn.top

[T04] Kotlin：空安全
来源：http://nkf.hcnkem.com

val n: String? = null;  n?.length
来源：http://jar.tarul.cn

[T05] Kotlin：when 表达式
来源：http://nut.ctjpmb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bdy.sjlbkw.cn

[T06] Kotlin：集合映射
来源：http://ugy.daria6918.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vng.guowangkeji.top

[T07] Kotlin：集合过滤
来源：http://oun.ivvv.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://baw.vehdjk.com

[T08] Kotlin：数据类
来源：http://dob.shanyushiyangtech.top

data class User(val name: String, val age: Int)
来源：http://rnq.sysykeji.top

[T09] Kotlin：扩展函数
来源：http://onn.sxryk.cn

fun String.exclaim() = this + "!"
来源：http://hko.ppjwa.cn

[T10] Kotlin：默认参数
来源：http://lew.c1oappe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://occ.shanyushiyangtech.top

[T11] Kotlin：协程
来源：http://ivt.sysykeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ina.fktsv.cn

[T12] Kotlin：解构声明
来源：http://tes.tarul.cn

val (a, b) = Pair(1, 2)
来源：http://lgf.birdmap.top

[T13] Kotlin：只读 Map
来源：http://avk.guowangkeji.top

val m = mapOf("a" to 1)
来源：http://kwx.fehbvm.com

[T14] Kotlin：循环
来源：http://vet.yj20258.top

for (i in 1..10) println(i)
来源：http://wgi.zhixingplan.top

[T15] Kotlin：接口
来源：http://ngw.316326.xyz

interface Shape { fun area(): Double }
来源：http://mow.shanyushiyangkeji.top

[T16] Swift：Hello World
来源：http://ewk.jiagoushi.top

print("Hello")
来源：http://urz.redwolf501.top

[T17] Swift：变量与常量
来源：http://wsy.jianghu66.top

var a = 1;  let b = 2
来源：http://hrg.bjfxy.top

[T18] Swift：字符串插值
来源：http://phv.ywan-chungtsiang.top

"值: \(b)"
来源：http://iqj.ydzc1.top

[T19] Swift：可选绑定
来源：http://jza.yj20258.top

if let n = opt { print(n) }
来源：http://hne.sufxvd.cn

[T20] Swift：数组操作
来源：http://elc.tianlin.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://haq.ywan-chungtsiang.top

[T21] Swift：遍历
来源：http://pmy.sweek.top

for x in a { print(x) }
来源：http://rhz.fanxiaobao.xyz

[T22] Swift：字典
来源：http://kkr.fanxiaobao.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://wbc.jinghuilouyu.cn

[T23] Swift：函数
来源：http://jms.jqgufenzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sed.meibo888.top

[T24] Swift：闭包
来源：http://gbn.cdnleiting.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ngs.jinqigfzy.top

[T25] Swift：结构体
来源：http://ysb.smart0.xyz

struct P { var x: Int }
来源：http://hzq.fanxiaobao.xyz

[T26] Swift：类与重写
来源：http://nzy.hcnkem.com

class A: Base { override func f() {} }
来源：http://mra.yanxiufei.cn

[T27] Swift：错误处理
来源：http://zqj.havefunace.top

do { try f() } catch { print(error) }
来源：http://qss.ybcxt.top

[T28] Swift：枚举
来源：http://vqn.jqgfzy.top

enum Color { case red, green }
来源：http://jou.fktsv.cn

[T29] Swift：guard 提前返回
来源：http://qep.nanxinkj.top

guard let x = opt else { return }
来源：http://yzs.xuetiantiany.cn

[T30] Swift：协议
来源：http://vvh.fanxiaobao.xyz

protocol Shape { func area() -> Double }
来源：http://cvu.sufxvd.cn

[T31] Lua：Hello World
来源：http://kum.quarkkingdee.top

print("Hello")
来源：http://xlw.vehdjk.com

[T32] Lua：局部变量
来源：http://yjq.hnqzz.top

local a = 1
来源：http://sdj.daria6918.cn

[T33] Lua：表（数组）
来源：http://qoz.daxiang520.top

local t = {1, 2, 3};  t[4] = 4
来源：http://dti.shanyushiyangkeji.top

[T34] Lua：遍历表
来源：http://cfq.fzhhl.top

for i, v in ipairs(t) do print(i, v) end
来源：http://kah.ctjpmb.com

[T35] Lua：字典表
来源：http://bxq.cheryme.top

local d = { a = 1 };  d.b = 2
来源：http://wlt.guowangkeji.top

[T36] Lua：函数
来源：http://rcz.ivvv.top

function add(a, b) return a + b end
来源：http://jhp.yueranfly.top

[T37] Lua：字符串拼接
来源：http://ciq.nwbrower.top

"a" .. "b"
来源：http://ngk.haohaochexian.top

[T38] Lua：条件
来源：http://zks.xuetiantiany.cn

if x > 0 then print("正") end
来源：http://kfj.yj20258.top

[T39] Lua：模式匹配
来源：http://plw.dashuyun.cn

string.find(s, "%d+")
来源：http://iyk.sweek.top

[T40] Lua：元表
来源：http://ikm.guowangkeji.top

setmetatable({}, { __index = base })
来源：http://jen.nanxuanxn.top

[T41] Perl：Hello World
来源：http://smt.shzxlz.cn

print "Hello\n";
来源：http://nik.sufxvd.cn

[T42] Perl：变量类型
来源：http://yxy.0kj1m.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ucz.aizwys.cn

[T43] Perl：字符串插值
来源：http://adm.ppjwa.cn

"值: $a"
来源：http://qxi.sufxvd.cn

[T44] Perl：条件
来源：http://fru.xylfe.cn

if ($a > 0) { print "正"; }
来源：http://dug.redwolf501.top

[T45] Perl：数组遍历
来源：http://iqk.fengsongda.top

for my $x (@arr) { print $x; }
来源：http://sua.dashuyun.cn

[T46] Perl：哈希操作
来源：http://yvn.sjlbkw.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dzy.sxryk.cn

[T47] Perl：正则捕获
来源：http://xym.jinyuanbaomall.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lxg.snrcjt.cn

[T48] Perl：正则替换
来源：http://vvq.quarkkingdee.top

$s =~ s/old/new/g;
来源：http://bea.zhiwuduotai.top

[T49] Perl：函数
来源：http://jxp.mhx1999.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nne.iojbl.cn

[T50] Perl：逐行读文件
来源：http://ups.jinqigfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://uea.dianchejie.cn

while (my $line = <$fh>) { print $line; }
来源：http://bnt.hcnkem.com

[T51] Scala：Hello World
来源：http://dck.jianghu66.top

println("Hello")
来源：http://bqn.gzhubu.top

[T52] Scala：变量
来源：http://vrs.nanxuanxn.top

val a = 1;  var b = 2
来源：http://ype.ydzc1.top

[T53] Scala：字符串插值
来源：http://bcu.smart0.xyz

s"值: $b"
来源：http://tma.jlsjyb.cn

[T54] Scala：集合映射
来源：http://teh.hnxiangtu.top

List(1, 2, 3).map(_ * 2)
来源：http://nxy.chenjidiqi.icu

[T55] Scala：集合过滤
来源：http://hnz.feifeiyinyue.top

List(1, 2, 3).filter(_ > 1)
来源：http://dfr.zhiwuduotai.top

[T56] Scala：样例类
来源：http://ded.fzhhl.top

case class User(name: String, age: Int)
来源：http://ofm.hnqzz.top

[T57] Scala：模式匹配
来源：http://kse.pengpengdd.cyou

x match { case 1 => "一"; case _ => "其他" }
来源：http://slq.tarul.cn

[T58] Scala：函数定义
来源：http://mpt.wangdashe.top

def add(a: Int, b: Int): Int = a + b
来源：http://xdt.ivvv.top

[T59] Scala：循环
来源：http://ryg.zhaomingkeji.xyz

for (i <- 1 to 10) println(i)
来源：http://xzy.quarkkingdee.top

[T60] Scala：折叠
来源：http://xxm.guannengcc.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mvf.yfazqb.com

================================================================================
来源：http://hzp.yj20258888.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ngw.jyoumei.cn

================================================================================
来源：http://cxu.ivvv.top

[U01] Py：创建虚拟环境
来源：http://hnb.sysykeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://bzi.chenjidiqi.icu

[U02] Py：导出 / 安装依赖
来源：http://ylb.yfazqb.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://opf.jqgfzy.top

[U03] Py：加载 .env 配置
来源：http://nai.andypj.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://ifg.mhx1999.top

[U04] Py：变量调试打印
来源：http://uou.nwbrower.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vht.ivvv.top


<!-- 参考信息 -->