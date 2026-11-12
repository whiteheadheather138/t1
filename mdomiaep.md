代发 wailian999

free -h;  ps aux | grep nginx
来源：http://lhf.yj20258888.top

[R64] 结束进程
来源：http://etz.chenjidiqi.icu

kill -9 $(pgrep -f app.py)
来源：http://hjv.sxryk.cn

[R65] 查看端口占用
来源：http://qeb.yuxming.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://prt.daria6918.cn

[R66] 定时任务
来源：http://lek.jinyuanbaomall.cn

crontab -e;  crontab -l
来源：http://fev.yj20258888.top

[R67] 生成随机十六进制串
来源：http://egr.yonumen.top

openssl rand -hex 16
来源：http://uxf.zdbjq.cn

[R68] 计算文件校验值
来源：http://cix.tianlin.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://xha.jinqigufen.top

[R69] 生成随机密码
来源：http://und.cucudq.cn

head -c 16 /dev/urandom | base64
来源：http://hdj.uphjek.com

[R70] 时间戳与互转
来源：http://fgv.gotoacloud.top

date +%s;  date -d @1700000000
来源：http://vza.hnxiangtu.top

[R71] 日期格式化
来源：http://ohl.ywan-chungtsiang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xme.zycfv.cn

[R72] 等待端口就绪
来源：http://lzb.havefunace.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qfg.shzxlz.cn

[R73] 分割大日志
来源：http://dkh.ppjwa.cn

split -l 1000 big.log part_
来源：http://dew.xuetiantiany.cn

[R74] 批量重命名
来源：http://grv.316326.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pnn.zhijiandao.cn

[R75] 导出环境变量
来源：http://jbr.jqgfzy.top

export PATH="$HOME/bin:$PATH"
来源：http://dpj.zdqjudy.top

[R76] 使用临时文件
来源：http://ndj.cheryme.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hze.sufxvd.cn

[R77] 读取用户输入
来源：http://ugy.jinyuanbaomall.cn

read -rp "请输入: " ans
来源：http://bdx.chenjidiqi.icu

[R78] 交互式菜单
来源：http://niz.yj20258888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://pux.iojbl.cn

[R79] 解析命令行选项
来源：http://pdr.c1oappe.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ann.dianchejie.cn

[R80] 查看脚本执行耗时
来源：http://iho.shanyushiyangtech.top

time ./run.sh
来源：http://tuy.daria6918.cn

================================================================================
来源：http://dxy.tarul.cn

S. C / C++ 专题
来源：http://aua.feifeiyinyue.top

================================================================================
来源：http://jdo.kuanghao11.cn

[S01] C：Hello World
来源：http://iww.chenlongwang.top

#include <stdio.h>
来源：http://pwp.hysaishi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://efn.fanxiaobao.xyz

[S02] C：变量与格式化输出
来源：http://bii.quarkkingdee.top

int a = 10; printf("%d\n", a);
来源：http://eyz.sjlbkw.cn

[S03] C：读入整数
来源：http://yek.yj20258.top

int x; scanf("%d", &x);
来源：http://pqh.9152youxi.cn

[S04] C：字符串复制
来源：http://wlx.hywenlv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qxt.nanxuanxn.top

[S05] C：字符串长度
来源：http://mjs.xingfuxueyuan.xyz

strlen(s)
来源：http://mup.9152youxi.cn

[S06] C：字符串比较
来源：http://ykc.sxryk.cn

strcmp(a, b) == 0
来源：http://lkr.yfazqb.com

[S07] C：数组遍历求和
来源：http://aew.ehwqpu.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qop.nanxuanxn.top

[S08] C：动态内存分配与释放
来源：http://jlb.zhengqikj.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jbu.jiagoushi.top

[S09] C：结构体定义与初始化
来源：http://jkh.nanxuanxn.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yxa.wangdashe.top

[S10] C：指针与解引用
来源：http://uke.gogol.net.cn

int *p = &a;  *p = 5;
来源：http://knu.hnqzz.top

[S11] C：逐行读文件
来源：http://dww.gogol.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://igo.ydzc1.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ygb.daria6918.cn

fclose(f);
来源：http://ecn.hywenlv.cn

[S12] C：写文件
来源：http://dog.gotoacloud.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xfq.yfazqb.com

[S13] C：宏定义
来源：http://dzo.hywenlv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yyn.svipenyu.cn

[S14] C：枚举
来源：http://jtp.xuanzx.com

enum Color { RED, GREEN, BLUE };
来源：http://xlq.fktsv.cn

[S15] C：类型转换
来源：http://jtz.shanyushiyangkeji.top

(double) a / b
来源：http://rvh.zhijiandao.cn

[S16] C：位操作置位
来源：http://ztj.gogol.net.cn

x |= (1 << 3);
来源：http://kin.nanxuanxn.top

[S17] C：安全拼接字符串
来源：http://lxm.yfazqb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tqa.sufxvd.cn

[S18] C：命令行参数
来源：http://kkf.vehdjk.com

int main(int argc, char **argv)
来源：http://nle.epnwcf.com

[S19] C：快速排序
来源：http://tjb.jianghu66.top

qsort(a, n, sizeof(int), cmp);
来源：http://wfz.cdnleiting.top

[S20] C：二分查找
来源：http://frm.cdnleiting.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kjr.xuetiantiany.cn

[S21] C：字符类别判断
来源：http://rhj.zhaomingkeji.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://scn.birdmap.top

[S22] C：字符串转数字
来源：http://ata.yonumen.top

atoi("42");  strtod("3.14", NULL);
来源：http://glv.yuxming.cn

[S23] C：随机数
来源：http://niy.yfazqb.com

srand(time(NULL));  int r = rand() % 100;
来源：http://elf.jlsjyb.cn

[S24] C：获取本地时间
来源：http://sli.epnwcf.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tdl.tarul.cn

[S25] C：内存拷贝
来源：http://wds.cheryme.top

memcpy(dst, src, n);
来源：http://pkc.uphjek.com

[S26] C：内存清零
来源：http://kbp.zhiwuduotai.top

memset(a, 0, sizeof a);
来源：http://rmf.hesvh.cn

[S27] C：定义常量
来源：http://ccz.tanke756.top

const double PI = 3.14159;
来源：http://tmc.ydjk.org.cn

[S28] C：静态变量
来源：http://iad.jinghuilouyu.cn

static int counter = 0;
来源：http://wke.zhixingplan.top

[S29] C：变参函数
来源：http://bte.zhixingplan.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bqi.xylfe.cn

[S30] C：头文件保护
来源：http://vqm.yangfankeji.com

#ifndef X_H
来源：http://vzq.xylfe.cn

#define X_H
来源：http://kyg.andypj.xyz

#endif
来源：http://msd.yongpay.top

[S31] C++：Hello World
来源：http://fij.xuetiantiany.cn

#include <iostream>
来源：http://jfe.xylfe.cn

int main() { std::cout << "Hello\n"; }
来源：http://mxd.jlsjyb.cn

[S32] C++：字符串
来源：http://wfj.smart0.xyz

std::string s = "hi";  s += "!";
来源：http://vnw.hammf.cn

[S33] C++：vector 增删
来源：http://myu.jiagoushi.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tfq.jqgfzy.top

[S34] C++：遍历 vector
来源：http://xpz.yvedp.cn

for (auto &x : v) { std::cout << x; }
来源：http://zzo.ydjk.org.cn

[S35] C++：map
来源：http://dbl.sysykeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mtc.smart0.xyz

[S36] C++：unordered_map
来源：http://tqe.hnxiangtu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vkb.hnqzz.top

[S37] C++：set
来源：http://psp.yfazqb.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ldn.zhoulong.xyz

[S38] C++：排序
来源：http://dwb.zhengqikj.top

std::sort(v.begin(), v.end());
来源：http://thn.shangyingyoupin.top

[S39] C++：自定义比较器排序
来源：http://ntr.wangshuangyany.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://osq.ppjwa.cn

[S40] C++：查找元素
来源：http://oap.ydzc1.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fqo.dashuyun.cn

[S41] C++：类与构造函数
来源：http://qlu.xziqi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fsw.tianlin.xyz

[S42] C++：继承与虚函数
来源：http://rop.wangdashe.top

class B : public Base { public: void f() override {} };
来源：http://ibx.daxiang520.top

[S43] C++：智能指针
来源：http://hxz.cheryme.top

auto p = std::make_unique<int>(5);
来源：http://cph.cdnleiting.top

[S44] C++：引用传参
来源：http://sdf.zdqjudy.top

void inc(int &x) { ++x; }
来源：http://oeh.yonumen.top

[S45] C++：lambda
来源：http://tjw.guannengcc.top

auto add = [](int a, int b) { return a + b; };
来源：http://ofs.quarkkingdee.top

[S46] C++：函数模板
来源：http://xmo.feifeiyinyue.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qzd.aibaodan.cn

[S47] C++：结构化绑定遍历
来源：http://uws.ydjk.org.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qiy.gotoacloud.top

[S48] C++：逐行读文件
来源：http://byk.wangshuangyany.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nff.yfazqb.com

while (std::getline(in, line)) { }
来源：http://pjt.xinyue.icu

[S49] C++：写文件
来源：http://ijn.haohaochexian.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jvl.cqqwz.cn

[S50] C++：格式化数字
来源：http://xxz.ehwqpu.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dql.smart0.xyz

[S51] C++：显式类型转换
来源：http://ozr.ydjk.org.cn

static_cast<double>(a) / b
来源：http://ozw.kuanghao11.cn

[S52] C++：const 与 noexcept
来源：http://qgv.dianchejie.cn

int size() const noexcept { return n_; }
来源：http://zyn.yfazqb.com

[S53] C++：移动语义
来源：http://kus.dashuyun.cn

std::vector<int> w = std::move(v);
来源：http://ooo.fktsv.cn

[S54] C++：异常处理
来源：http://onw.bbcook.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gqe.iojbl.cn

[S55] C++：结构化绑定
来源：http://tdp.xuetiantiany.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pmm.zhoulong.xyz

[S56] C++：optional
来源：http://biy.iojbl.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://faf.zhoulong.xyz

[S57] C++：编译期常量
来源：http://bax.zhengqikj.top

constexpr int N = 10;
来源：http://hnn.jyoumei.cn

[S58] C++：命名空间
来源：http://lzb.gzhubu.top

namespace ns { int f() { return 1; } }
来源：http://fkw.hongshengwenyu.top

[S59] C++：静态断言
来源：http://jea.chenzaomai.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wwf.jqgfzy.top

[S60] C++：遍历并删除元素
来源：http://fbs.nanxinkj.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dnl.tarul.cn

================================================================================
来源：http://jxh.hfpthk.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vng.chenlongwang.top

================================================================================
来源：http://vhu.sjlbkw.cn

[T01] Kotlin：Hello World
来源：http://rsy.tarul.cn

println("Hello")
来源：http://agg.iojbl.cn

[T02] Kotlin：变量
来源：http://syj.jqgfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ixh.fzhhl.top

[T03] Kotlin：字符串模板
来源：http://vxm.fehbvm.com

"值: $b"
来源：http://pmw.yj20258888.top

[T04] Kotlin：空安全
来源：http://rat.cucudq.cn

val n: String? = null;  n?.length
来源：http://rud.chenzaomai.com

[T05] Kotlin：when 表达式
来源：http://jgm.0kj1m.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kyv.xziqi.cn

[T06] Kotlin：集合映射
来源：http://nlp.snrcjt.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rva.fzhhl.top

[T07] Kotlin：集合过滤
来源：http://dce.hywenlv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://srk.jinghuilouyu.cn

[T08] Kotlin：数据类
来源：http://nuo.shanyushiyangtech.top

data class User(val name: String, val age: Int)
来源：http://iyr.ybcxt.top

[T09] Kotlin：扩展函数
来源：http://oju.fanxiaobao.xyz

fun String.exclaim() = this + "!"
来源：http://uwy.yueranfly.top

[T10] Kotlin：默认参数
来源：http://lwf.aizwys.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uir.gaohongyu789.top

[T11] Kotlin：协程
来源：http://mgh.kuanghao11.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ttg.yvedp.cn

[T12] Kotlin：解构声明
来源：http://gen.yueranfly.top

val (a, b) = Pair(1, 2)
来源：http://qgn.xuanzx.com

[T13] Kotlin：只读 Map
来源：http://trq.shanyushiyangkeji.top

val m = mapOf("a" to 1)
来源：http://cep.sufxvd.cn

[T14] Kotlin：循环
来源：http://iup.yongpay.top

for (i in 1..10) println(i)
来源：http://cdk.jqgfzy.top

[T15] Kotlin：接口
来源：http://rnb.wangdashe.top

interface Shape { fun area(): Double }
来源：http://nex.pengpengdd.cyou

[T16] Swift：Hello World
来源：http://hif.vehdjk.com

print("Hello")
来源：http://dra.hnqzz.top

[T17] Swift：变量与常量
来源：http://akx.gogol.net.cn

var a = 1;  let b = 2
来源：http://ior.c1oappe.top

[T18] Swift：字符串插值
来源：http://dci.wangshuangyany.cn

"值: \(b)"
来源：http://pci.cdnleiting.top

[T19] Swift：可选绑定
来源：http://iwz.ppjwa.cn

if let n = opt { print(n) }
来源：http://rjp.mhx1999.top

[T20] Swift：数组操作
来源：http://ywr.zhixingplan.top

var a = [1, 2, 3];  a.append(4)
来源：http://zot.yuanzhike.top

[T21] Swift：遍历
来源：http://lhc.hysaishi.cn

for x in a { print(x) }
来源：http://bgp.yj202588.top

[T22] Swift：字典
来源：http://tzb.kuanghao11.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gtu.yanxiufei.cn

[T23] Swift：函数
来源：http://bja.zhengqikj.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lpy.0kj1m.cn

[T24] Swift：闭包
来源：http://zza.cheryme.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://taz.ivvv.top

[T25] Swift：结构体
来源：http://gwa.birdmap.top

struct P { var x: Int }
来源：http://ufr.dashuyun.cn

[T26] Swift：类与重写
来源：http://gcn.chenlongwang.top

class A: Base { override func f() {} }
来源：http://tsk.ydjk.org.cn

[T27] Swift：错误处理
来源：http://aez.pycfn.com

do { try f() } catch { print(error) }
来源：http://plv.cucudq.cn

[T28] Swift：枚举
来源：http://wnf.ctjpmb.com

enum Color { case red, green }
来源：http://qro.gotoacloud.top

[T29] Swift：guard 提前返回
来源：http://pjq.vqdsnc.cn

guard let x = opt else { return }
来源：http://pzk.hfpthk.cn

[T30] Swift：协议
来源：http://hjk.chenzaomai.com

protocol Shape { func area() -> Double }
来源：http://jyp.yangfankeji.com

[T31] Lua：Hello World
来源：http://ztv.yvedp.cn

print("Hello")
来源：http://vhs.xuetiantiany.cn

[T32] Lua：局部变量
来源：http://qxk.yuxming.cn

local a = 1
来源：http://qzt.xingfuxueyuan.xyz

[T33] Lua：表（数组）
来源：http://moq.sufxvd.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tge.aizwys.cn

[T34] Lua：遍历表
来源：http://mub.birdmap.top

for i, v in ipairs(t) do print(i, v) end
来源：http://pua.c1oappe.top

[T35] Lua：字典表
来源：http://bnt.zycfv.cn

local d = { a = 1 };  d.b = 2
来源：http://jrw.kuanghao11.cn

[T36] Lua：函数
来源：http://rle.uphjek.com

function add(a, b) return a + b end
来源：http://sjo.shzxlz.cn

[T37] Lua：字符串拼接
来源：http://syq.zhongyouzk.top

"a" .. "b"
来源：http://csv.jlsjyb.cn

[T38] Lua：条件
来源：http://clz.dashuyun.cn

if x > 0 then print("正") end
来源：http://msr.nanxuanxn.top

[T39] Lua：模式匹配
来源：http://lsu.xylfe.cn

string.find(s, "%d+")
来源：http://txs.chenzaomai.com

[T40] Lua：元表
来源：http://ujl.smart0.xyz

setmetatable({}, { __index = base })
来源：http://mlz.wangdashe.top

[T41] Perl：Hello World
来源：http://tbc.nanxinkj.top

print "Hello\n";
来源：http://pfu.fzhhl.top

[T42] Perl：变量类型
来源：http://bhm.pengpengdd.cyou

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qkw.jyoumei.cn

[T43] Perl：字符串插值
来源：http://mhm.gogol.net.cn

"值: $a"
来源：http://fnb.svipenyu.cn

[T44] Perl：条件
来源：http://fds.zhixingplan.top

if ($a > 0) { print "正"; }
来源：http://gnj.sysykeji.top

[T45] Perl：数组遍历
来源：http://svj.hesvh.cn

for my $x (@arr) { print $x; }
来源：http://que.smart0.xyz

[T46] Perl：哈希操作
来源：http://vlg.ivvv.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dya.nwbrower.top

[T47] Perl：正则捕获
来源：http://wwa.52xcode.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vms.bbcook.cn

[T48] Perl：正则替换
来源：http://xal.hnxiangtu.top

$s =~ s/old/new/g;
来源：http://ptf.vqdsnc.cn

[T49] Perl：函数
来源：http://een.aibaodan.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tnw.yuanzhike.top

[T50] Perl：逐行读文件
来源：http://xqo.gotoacloud.top

open my $fh, "<", "a.txt" or die $!;
来源：http://yww.yfazqb.com

while (my $line = <$fh>) { print $line; }
来源：http://yqp.cdnleiting.top

[T51] Scala：Hello World
来源：http://bbx.chenlongwang.top

println("Hello")
来源：http://hex.hysaishi.cn

[T52] Scala：变量
来源：http://srh.yuanzhike.top

val a = 1;  var b = 2
来源：http://ats.vqdsnc.cn

[T53] Scala：字符串插值
来源：http://zcf.zycfv.cn

s"值: $b"
来源：http://owt.hesvh.cn

[T54] Scala：集合映射
来源：http://hvo.havefunace.top

List(1, 2, 3).map(_ * 2)
来源：http://zip.sweek.top

[T55] Scala：集合过滤
来源：http://cac.zhijiandao.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pyn.haohaochexian.top

[T56] Scala：样例类
来源：http://wzd.yuxming.cn

case class User(name: String, age: Int)
来源：http://zck.yangfankeji.com

[T57] Scala：模式匹配
来源：http://prs.daria6918.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fug.jianghu66.top

[T58] Scala：函数定义
来源：http://rhx.zhaomingkeji.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://oji.sweek.top

[T59] Scala：循环
来源：http://gub.9152youxi.cn

for (i <- 1 to 10) println(i)
来源：http://oau.vehdjk.com

[T60] Scala：折叠
来源：http://flv.jinyuanbaomall.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://giz.meibo888.top

================================================================================
来源：http://djt.yonumen.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xoz.xuetiantiany.cn

================================================================================
来源：http://sdc.havefunace.top

[U01] Py：创建虚拟环境
来源：http://ugg.zhongyouzk.top

python -m venv .venv && source .venv/bin/activate
来源：http://bzj.shuidangran.top

[U02] Py：导出 / 安装依赖
来源：http://dzu.shzxlz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://myr.zdbjq.cn

[U03] Py：加载 .env 配置
来源：http://zly.iojbl.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bfw.zdqjudy.top

[U04] Py：变量调试打印
来源：http://diq.cqqwz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yuh.aizwys.cn


<!-- 参考信息 -->