代发 wailian999

ssh user@host 'uptime'
来源：http://zqb.andypj.xyz

[R58] 下载文件
来源：http://ivg.yvedp.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wpp.mhx1999.top

[R59] 发 POST JSON
来源：http://hti.jqgfzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ajv.hongshengwenyu.top

[R60] 只看 HTTP 状态码
来源：http://dcw.yfazqb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://clh.shangyingyoupin.top

[R61] 磁盘占用
来源：http://njg.cashguo.top

df -h;  du -sh *
来源：http://cqh.9152youxi.cn

[R62] 找最占空间的文件
来源：http://zqj.yanxiufei.cn

du -ah . | sort -rh | head -10
来源：http://ayn.yangfankeji.com

[R63] 内存与进程
来源：http://epx.fktsv.cn

free -h;  ps aux | grep nginx
来源：http://evp.fktsv.cn

[R64] 结束进程
来源：http://fea.xziqi.cn

kill -9 $(pgrep -f app.py)
来源：http://guv.smart0.xyz

[R65] 查看端口占用
来源：http://xoh.ppjwa.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zhq.epnwcf.com

[R66] 定时任务
来源：http://ngv.feifeiyinyue.top

crontab -e;  crontab -l
来源：http://gul.yj20258888.top

[R67] 生成随机十六进制串
来源：http://iqs.zhiwuduotai.top

openssl rand -hex 16
来源：http://kpk.zhoulong.xyz

[R68] 计算文件校验值
来源：http://gcw.hnqzz.top

sha256sum a.txt;  md5sum a.txt
来源：http://clc.andypj.xyz

[R69] 生成随机密码
来源：http://imw.sweek.top

head -c 16 /dev/urandom | base64
来源：http://xcn.zhongyouzk.top

[R70] 时间戳与互转
来源：http://oxj.birdmap.top

date +%s;  date -d @1700000000
来源：http://hbm.cashguo.top

[R71] 日期格式化
来源：http://bdu.ywan-chungtsiang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://wid.meibo888.top

[R72] 等待端口就绪
来源：http://naa.hywenlv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cqe.cucudq.cn

[R73] 分割大日志
来源：http://elu.haohaochexian.top

split -l 1000 big.log part_
来源：http://ccq.kuanghao11.cn

[R74] 批量重命名
来源：http://aoe.sufxvd.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jli.xuetiantiany.cn

[R75] 导出环境变量
来源：http://pjc.shuidangran.top

export PATH="$HOME/bin:$PATH"
来源：http://kbb.pengpengdd.cyou

[R76] 使用临时文件
来源：http://jqj.xziqi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://aae.hammf.cn

[R77] 读取用户输入
来源：http://omn.sufxvd.cn

read -rp "请输入: " ans
来源：http://xqo.haohaochexian.top

[R78] 交互式菜单
来源：http://lwc.sweek.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hcp.zdqjudy.top

[R79] 解析命令行选项
来源：http://tby.smart0.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fhs.aibaodan.cn

[R80] 查看脚本执行耗时
来源：http://tnh.cdnleiting.top

time ./run.sh
来源：http://ake.shuidangran.top

================================================================================
来源：http://pee.aizwys.cn

S. C / C++ 专题
来源：http://qxe.ywan-chungtsiang.top

================================================================================
来源：http://vdm.yj20258.top

[S01] C：Hello World
来源：http://tsc.c1oappe.top

#include <stdio.h>
来源：http://ebx.fktsv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nez.andypj.xyz

[S02] C：变量与格式化输出
来源：http://sug.epnwcf.com

int a = 10; printf("%d\n", a);
来源：http://lzj.yuxming.cn

[S03] C：读入整数
来源：http://plu.zhengqikj.top

int x; scanf("%d", &x);
来源：http://ksq.jiagoushi.top

[S04] C：字符串复制
来源：http://tku.yangfankeji.com

char dst[32]; strcpy(dst, "hi");
来源：http://ypk.hywenlv.cn

[S05] C：字符串长度
来源：http://pry.ydzc1.top

strlen(s)
来源：http://crw.shzxlz.cn

[S06] C：字符串比较
来源：http://dgi.cqqwz.cn

strcmp(a, b) == 0
来源：http://ubf.fktsv.cn

[S07] C：数组遍历求和
来源：http://qkk.cheryme.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://itj.mhx1999.top

[S08] C：动态内存分配与释放
来源：http://kho.hfpthk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xuu.mhx1999.top

[S09] C：结构体定义与初始化
来源：http://til.yfazqb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jjd.shzxlz.cn

[S10] C：指针与解引用
来源：http://hah.gogol.net.cn

int *p = &a;  *p = 5;
来源：http://ket.tarul.cn

[S11] C：逐行读文件
来源：http://kwq.jiagoushi.top

FILE *f = fopen("a.txt", "r");
来源：http://ckd.sweek.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://lkq.sxryk.cn

fclose(f);
来源：http://jzz.jqgufenzy.top

[S12] C：写文件
来源：http://aax.xziqi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gfc.sweek.top

[S13] C：宏定义
来源：http://xwu.ywan-chungtsiang.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cii.shzxlz.cn

[S14] C：枚举
来源：http://cfl.svipenyu.cn

enum Color { RED, GREEN, BLUE };
来源：http://prq.52xcode.cn

[S15] C：类型转换
来源：http://cgy.ybcxt.top

(double) a / b
来源：http://wlm.cheryme.top

[S16] C：位操作置位
来源：http://sgh.hnqzz.top

x |= (1 << 3);
来源：http://mmc.jiagoushi.top

[S17] C：安全拼接字符串
来源：http://rfo.tarul.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://klh.chenlongwang.top

[S18] C：命令行参数
来源：http://tjh.jiagoushi.top

int main(int argc, char **argv)
来源：http://rno.iojbl.cn

[S19] C：快速排序
来源：http://pco.hcnkem.com

qsort(a, n, sizeof(int), cmp);
来源：http://jir.zhaomingkeji.xyz

[S20] C：二分查找
来源：http://zup.jinqigfzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uxd.dianchejie.cn

[S21] C：字符类别判断
来源：http://gjv.yuxming.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gfa.c1oappe.top

[S22] C：字符串转数字
来源：http://kti.sufxvd.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jzk.pengpengdd.cyou

[S23] C：随机数
来源：http://oof.smart0.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://zol.yangfankeji.com

[S24] C：获取本地时间
来源：http://aib.birdmap.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ryo.hammf.cn

[S25] C：内存拷贝
来源：http://ili.kuanghao11.cn

memcpy(dst, src, n);
来源：http://cuf.cheryme.top

[S26] C：内存清零
来源：http://ack.sufxvd.cn

memset(a, 0, sizeof a);
来源：http://lbv.jqgufenzy.top

[S27] C：定义常量
来源：http://ztb.zdbjq.cn

const double PI = 3.14159;
来源：http://htf.yangfankeji.com

[S28] C：静态变量
来源：http://ctt.sysykeji.top

static int counter = 0;
来源：http://kur.jinghuilouyu.cn

[S29] C：变参函数
来源：http://ldy.yj20258.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kch.cashguo.top

[S30] C：头文件保护
来源：http://mgu.zycfv.cn

#ifndef X_H
来源：http://buh.jiagoushi.top

#define X_H
来源：http://geu.yfazqb.com

#endif
来源：http://wcs.yuanzhike.top

[S31] C++：Hello World
来源：http://ygi.316326.xyz

#include <iostream>
来源：http://cmv.bbcook.cn

int main() { std::cout << "Hello\n"; }
来源：http://ntc.feifeiyinyue.top

[S32] C++：字符串
来源：http://rcb.yonumen.top

std::string s = "hi";  s += "!";
来源：http://ien.chenjidiqi.icu

[S33] C++：vector 增删
来源：http://kim.xuanzx.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uoo.jinqigufen.top

[S34] C++：遍历 vector
来源：http://xxc.xinyue.icu

for (auto &x : v) { std::cout << x; }
来源：http://col.wangdashe.top

[S35] C++：map
来源：http://mev.hnxiangtu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zsl.daxiang520.top

[S36] C++：unordered_map
来源：http://yke.xuanzx.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uwa.bbcook.cn

[S37] C++：set
来源：http://nbj.epnwcf.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xuq.yj202588.top

[S38] C++：排序
来源：http://ons.yongpay.top

std::sort(v.begin(), v.end());
来源：http://jmo.haohaochexian.top

[S39] C++：自定义比较器排序
来源：http://evq.cashguo.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hxc.yangfankeji.com

[S40] C++：查找元素
来源：http://okg.gzhubu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ldj.ppjwa.cn

[S41] C++：类与构造函数
来源：http://jqz.zhongyouzk.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xym.fktsv.cn

[S42] C++：继承与虚函数
来源：http://ven.ydzc1.top

class B : public Base { public: void f() override {} };
来源：http://lab.tian-w.cn

[S43] C++：智能指针
来源：http://stt.yj20258.top

auto p = std::make_unique<int>(5);
来源：http://xru.shanyushiyangkeji.top

[S44] C++：引用传参
来源：http://tdn.9152youxi.cn

void inc(int &x) { ++x; }
来源：http://pdc.ydjk.org.cn

[S45] C++：lambda
来源：http://qxl.haohaochexian.top

auto add = [](int a, int b) { return a + b; };
来源：http://xid.cqqwz.cn

[S46] C++：函数模板
来源：http://mtn.dashuyun.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fzy.shangyingyoupin.top

[S47] C++：结构化绑定遍历
来源：http://soa.uphjek.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iva.yvedp.cn

[S48] C++：逐行读文件
来源：http://qpe.sufxvd.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vqc.jianghu66.top

while (std::getline(in, line)) { }
来源：http://kde.gotoacloud.top

[S49] C++：写文件
来源：http://pwg.daxiang520.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://djy.wangdashe.top

[S50] C++：格式化数字
来源：http://syu.yj20258888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mis.fzhhl.top

[S51] C++：显式类型转换
来源：http://xqb.sweek.top

static_cast<double>(a) / b
来源：http://oyu.hongshengwenyu.top

[S52] C++：const 与 noexcept
来源：http://cdr.sxryk.cn

int size() const noexcept { return n_; }
来源：http://cnu.hysaishi.cn

[S53] C++：移动语义
来源：http://jcq.yj202588.top

std::vector<int> w = std::move(v);
来源：http://htb.0kj1m.cn

[S54] C++：异常处理
来源：http://xvv.jinqigfzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wrb.gotoacloud.top

[S55] C++：结构化绑定
来源：http://yej.gotoacloud.top

auto [a, b] = std::make_pair(1, 2);
来源：http://sbp.birdmap.top

[S56] C++：optional
来源：http://jxb.ydjk.org.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vgz.pengpengdd.cyou

[S57] C++：编译期常量
来源：http://grh.sjlbkw.cn

constexpr int N = 10;
来源：http://whp.316326.xyz

[S58] C++：命名空间
来源：http://cnw.jinghuilouyu.cn

namespace ns { int f() { return 1; } }
来源：http://jpd.ybcxt.top

[S59] C++：静态断言
来源：http://dwl.shuidangran.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jwn.ybcxt.top

[S60] C++：遍历并删除元素
来源：http://ibk.aizwys.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ind.fanxiaobao.xyz

================================================================================
来源：http://pyq.jinyuanbaomall.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://auj.yvedp.cn

================================================================================
来源：http://foz.316326.xyz

[T01] Kotlin：Hello World
来源：http://xru.fanxiaobao.xyz

println("Hello")
来源：http://rjs.cqqwz.cn

[T02] Kotlin：变量
来源：http://jdt.yongpay.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yvh.yj202588.top

[T03] Kotlin：字符串模板
来源：http://wah.xinyue.icu

"值: $b"
来源：http://fle.tian-w.cn

[T04] Kotlin：空安全
来源：http://ihy.gotoacloud.top

val n: String? = null;  n?.length
来源：http://gqf.hfpthk.cn

[T05] Kotlin：when 表达式
来源：http://sxj.hysaishi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://buq.gzhubu.top

[T06] Kotlin：集合映射
来源：http://qrz.daria6918.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://uxh.c1oappe.top

[T07] Kotlin：集合过滤
来源：http://ybu.hfpthk.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pwy.shangyingyoupin.top

[T08] Kotlin：数据类
来源：http://yvg.daria6918.cn

data class User(val name: String, val age: Int)
来源：http://kla.cucudq.cn

[T09] Kotlin：扩展函数
来源：http://ccy.tianlin.xyz

fun String.exclaim() = this + "!"
来源：http://vyu.haohaochexian.top

[T10] Kotlin：默认参数
来源：http://ivw.xylfe.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://smg.hfpthk.cn

[T11] Kotlin：协程
来源：http://ebs.havefunace.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://jbi.jiagoushi.top

[T12] Kotlin：解构声明
来源：http://hdu.xziqi.cn

val (a, b) = Pair(1, 2)
来源：http://sgi.shanyushiyangtech.top

[T13] Kotlin：只读 Map
来源：http://krc.yj202588.top

val m = mapOf("a" to 1)
来源：http://hwp.mhx1999.top

[T14] Kotlin：循环
来源：http://xhv.pengpengdd.cyou

for (i in 1..10) println(i)
来源：http://mnz.c1oappe.top

[T15] Kotlin：接口
来源：http://nlj.iojbl.cn

interface Shape { fun area(): Double }
来源：http://hvs.hysaishi.cn

[T16] Swift：Hello World
来源：http://hgd.hywenlv.cn

print("Hello")
来源：http://mpv.9152youxi.cn

[T17] Swift：变量与常量
来源：http://rwr.nwbrower.top

var a = 1;  let b = 2
来源：http://dcc.xziqi.cn

[T18] Swift：字符串插值
来源：http://dco.bjfxy.top

"值: \(b)"
来源：http://bah.zdqjudy.top

[T19] Swift：可选绑定
来源：http://hha.fengsongda.top

if let n = opt { print(n) }
来源：http://yqs.jinqigfzy.top

[T20] Swift：数组操作
来源：http://rla.yj20258.top

var a = [1, 2, 3];  a.append(4)
来源：http://cqr.hcnkem.com

[T21] Swift：遍历
来源：http://bnn.xuanzx.com

for x in a { print(x) }
来源：http://exs.sjlbkw.cn

[T22] Swift：字典
来源：http://wkd.hcnkem.com

var d = ["a": 1];  d["b"] = 2
来源：http://kcx.bbcook.cn

[T23] Swift：函数
来源：http://yco.fehbvm.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pxj.pycfn.com

[T24] Swift：闭包
来源：http://coc.zhiwuduotai.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://sgp.epnwcf.com

[T25] Swift：结构体
来源：http://qic.pengpengdd.cyou

struct P { var x: Int }
来源：http://ftv.shanyushiyangkeji.top

[T26] Swift：类与重写
来源：http://kzl.yanxiufei.cn

class A: Base { override func f() {} }
来源：http://jte.bjfxy.top

[T27] Swift：错误处理
来源：http://lre.sxryk.cn

do { try f() } catch { print(error) }
来源：http://kub.ppjwa.cn

[T28] Swift：枚举
来源：http://fni.nanxinkj.top

enum Color { case red, green }
来源：http://mfq.chenlongwang.top

[T29] Swift：guard 提前返回
来源：http://aqy.xinyue.icu

guard let x = opt else { return }
来源：http://jmz.yj202588.top

[T30] Swift：协议
来源：http://lqd.xylfe.cn

protocol Shape { func area() -> Double }
来源：http://paa.xingfuxueyuan.xyz

[T31] Lua：Hello World
来源：http://nyk.zdqjudy.top

print("Hello")
来源：http://tdd.nanxinkj.top

[T32] Lua：局部变量
来源：http://eip.hfpthk.cn

local a = 1
来源：http://dwi.yuxming.cn

[T33] Lua：表（数组）
来源：http://qlq.jqgfzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://jko.bbcook.cn

[T34] Lua：遍历表
来源：http://rxv.xuetiantiany.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wye.jianghu66.top

[T35] Lua：字典表
来源：http://qzf.bjfxy.top

local d = { a = 1 };  d.b = 2
来源：http://xpz.zhixingplan.top

[T36] Lua：函数
来源：http://gfg.epnwcf.com

function add(a, b) return a + b end
来源：http://mpd.yuanzhike.top

[T37] Lua：字符串拼接
来源：http://mbu.fktsv.cn

"a" .. "b"
来源：http://bfk.fengsongda.top

[T38] Lua：条件
来源：http://qvd.316326.xyz

if x > 0 then print("正") end
来源：http://sxi.ydzc1.top

[T39] Lua：模式匹配
来源：http://qlf.yj20258.top

string.find(s, "%d+")
来源：http://dir.316326.xyz

[T40] Lua：元表
来源：http://glm.tanke756.top

setmetatable({}, { __index = base })
来源：http://gek.chenjidiqi.icu

[T41] Perl：Hello World
来源：http://hcn.gzhubu.top

print "Hello\n";
来源：http://ydt.tian-w.cn

[T42] Perl：变量类型
来源：http://xqo.zdbjq.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://acx.yvedp.cn

[T43] Perl：字符串插值
来源：http://spv.iojbl.cn

"值: $a"
来源：http://mlk.haohaochexian.top

[T44] Perl：条件
来源：http://due.nwbrower.top

if ($a > 0) { print "正"; }
来源：http://aba.cqqwz.cn

[T45] Perl：数组遍历
来源：http://qkv.52xcode.cn

for my $x (@arr) { print $x; }
来源：http://kqd.ybcxt.top

[T46] Perl：哈希操作
来源：http://kjt.yongpay.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://iew.snrcjt.cn

[T47] Perl：正则捕获
来源：http://rjw.wangshuangyany.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bha.cqqwz.cn

[T48] Perl：正则替换
来源：http://xer.ydjk.org.cn

$s =~ s/old/new/g;
来源：http://fil.feifeiyinyue.top

[T49] Perl：函数
来源：http://qwv.yfazqb.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zfx.hesvh.cn

[T50] Perl：逐行读文件
来源：http://lul.jinqigfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://rex.feifeiyinyue.top

while (my $line = <$fh>) { print $line; }
来源：http://tjm.cqqwz.cn

[T51] Scala：Hello World
来源：http://ura.snrcjt.cn

println("Hello")
来源：http://knc.yvedp.cn

[T52] Scala：变量
来源：http://ztw.gotoacloud.top

val a = 1;  var b = 2
来源：http://cnc.cqqwz.cn

[T53] Scala：字符串插值
来源：http://jnj.zhixingplan.top

s"值: $b"
来源：http://ezh.shanyushiyangkeji.top

[T54] Scala：集合映射
来源：http://uhn.xylfe.cn

List(1, 2, 3).map(_ * 2)
来源：http://rri.gzhubu.top

[T55] Scala：集合过滤
来源：http://bzq.jqgufenzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://lfp.yj202588.top

[T56] Scala：样例类
来源：http://zes.tarul.cn

case class User(name: String, age: Int)
来源：http://qvr.fzhhl.top

[T57] Scala：模式匹配
来源：http://hta.yuanzhike.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://mgw.yueranfly.top

[T58] Scala：函数定义
来源：http://wfr.kuanghao11.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wss.mhx1999.top

[T59] Scala：循环
来源：http://zfs.yj20258888.top

for (i <- 1 to 10) println(i)
来源：http://gzb.yj20258.top

[T60] Scala：折叠
来源：http://pnz.yfazqb.com


<!-- 参考信息 -->