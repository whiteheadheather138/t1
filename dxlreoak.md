代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lwf.zhengqikj.top

[R60] 只看 HTTP 状态码
来源：http://mwe.hongshengwenyu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cky.cashguo.top

[R61] 磁盘占用
来源：http://wjo.fanxiaobao.xyz

df -h;  du -sh *
来源：http://yud.zhijiandao.cn

[R62] 找最占空间的文件
来源：http://wmn.ctjpmb.com

du -ah . | sort -rh | head -10
来源：http://spy.quarkkingdee.top

[R63] 内存与进程
来源：http://pdn.vehdjk.com

free -h;  ps aux | grep nginx
来源：http://gba.zhengqikj.top

[R64] 结束进程
来源：http://rik.9152youxi.cn

kill -9 $(pgrep -f app.py)
来源：http://lof.andypj.xyz

[R65] 查看端口占用
来源：http://zqk.yangfankeji.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bxn.hnqzz.top

[R66] 定时任务
来源：http://qwf.svipenyu.cn

crontab -e;  crontab -l
来源：http://epb.hammf.cn

[R67] 生成随机十六进制串
来源：http://fxw.jinghuilouyu.cn

openssl rand -hex 16
来源：http://ufi.jinqigfzy.top

[R68] 计算文件校验值
来源：http://ofn.hnqzz.top

sha256sum a.txt;  md5sum a.txt
来源：http://xas.daria6918.cn

[R69] 生成随机密码
来源：http://avy.smart0.xyz

head -c 16 /dev/urandom | base64
来源：http://zqx.yj20258888.top

[R70] 时间戳与互转
来源：http://ivl.chenzaomai.com

date +%s;  date -d @1700000000
来源：http://gls.ybcxt.top

[R71] 日期格式化
来源：http://iei.chenzaomai.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://xov.zhongyouzk.top

[R72] 等待端口就绪
来源：http://spd.shangyingyoupin.top

until nc -z localhost 3306; do sleep 1; done
来源：http://hfi.hcnkem.com

[R73] 分割大日志
来源：http://sgh.zhijiandao.cn

split -l 1000 big.log part_
来源：http://fhk.yfazqb.com

[R74] 批量重命名
来源：http://psz.gaohongyu789.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lle.yj20258.top

[R75] 导出环境变量
来源：http://nzf.yj20258.top

export PATH="$HOME/bin:$PATH"
来源：http://zzu.hongshengwenyu.top

[R76] 使用临时文件
来源：http://qdv.hcnkem.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://auo.jyoumei.cn

[R77] 读取用户输入
来源：http://hsu.vqdsnc.cn

read -rp "请输入: " ans
来源：http://wcd.gaohongyu789.top

[R78] 交互式菜单
来源：http://eld.nanxuanxn.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ysr.xuanzx.com

[R79] 解析命令行选项
来源：http://ssm.birdmap.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dbs.zhengqikj.top

[R80] 查看脚本执行耗时
来源：http://gpz.feifeiyinyue.top

time ./run.sh
来源：http://jbg.nwbrower.top

================================================================================
来源：http://tfk.smart0.xyz

S. C / C++ 专题
来源：http://ayf.redwolf501.top

================================================================================
来源：http://kjq.hammf.cn

[S01] C：Hello World
来源：http://rsn.xylfe.cn

#include <stdio.h>
来源：http://uiu.smart0.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://har.iojbl.cn

[S02] C：变量与格式化输出
来源：http://kvw.sysykeji.top

int a = 10; printf("%d\n", a);
来源：http://yyj.yvedp.cn

[S03] C：读入整数
来源：http://qvb.ydzc1.top

int x; scanf("%d", &x);
来源：http://cqp.yuxming.cn

[S04] C：字符串复制
来源：http://gln.ybcxt.top

char dst[32]; strcpy(dst, "hi");
来源：http://zzq.bbcook.cn

[S05] C：字符串长度
来源：http://thw.ppjwa.cn

strlen(s)
来源：http://ygx.yuanzhike.top

[S06] C：字符串比较
来源：http://nuk.cashguo.top

strcmp(a, b) == 0
来源：http://dhw.shangyingyoupin.top

[S07] C：数组遍历求和
来源：http://zio.ctjpmb.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zap.gotoacloud.top

[S08] C：动态内存分配与释放
来源：http://hgb.yanxiufei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eru.ybcxt.top

[S09] C：结构体定义与初始化
来源：http://xbn.yj20258.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qeb.nanxuanxn.top

[S10] C：指针与解引用
来源：http://dtp.redwolf501.top

int *p = &a;  *p = 5;
来源：http://rfv.hesvh.cn

[S11] C：逐行读文件
来源：http://okl.gotoacloud.top

FILE *f = fopen("a.txt", "r");
来源：http://ptl.tianlin.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://srg.zhixingplan.top

fclose(f);
来源：http://hlv.tanke756.top

[S12] C：写文件
来源：http://fuu.feifeiyinyue.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xyk.zhiwuduotai.top

[S13] C：宏定义
来源：http://sre.ydzc1.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bua.feifeiyinyue.top

[S14] C：枚举
来源：http://hbb.hywenlv.cn

enum Color { RED, GREEN, BLUE };
来源：http://oya.hammf.cn

[S15] C：类型转换
来源：http://lqd.yuanzhike.top

(double) a / b
来源：http://nbb.xuetiantiany.cn

[S16] C：位操作置位
来源：http://fiw.meibo888.top

x |= (1 << 3);
来源：http://zvw.meibo888.top

[S17] C：安全拼接字符串
来源：http://dxd.fengsongda.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rus.jlsjyb.cn

[S18] C：命令行参数
来源：http://gty.jinyuanbaomall.cn

int main(int argc, char **argv)
来源：http://yxu.haohaochexian.top

[S19] C：快速排序
来源：http://ewa.tarul.cn

qsort(a, n, sizeof(int), cmp);
来源：http://oby.yj20258.top

[S20] C：二分查找
来源：http://tmc.0kj1m.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vfp.cheryme.top

[S21] C：字符类别判断
来源：http://zlj.guannengcc.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ypo.yuxming.cn

[S22] C：字符串转数字
来源：http://lyp.bjfxy.top

atoi("42");  strtod("3.14", NULL);
来源：http://vox.dianchejie.cn

[S23] C：随机数
来源：http://fqn.daxiang520.top

srand(time(NULL));  int r = rand() % 100;
来源：http://dzh.hywenlv.cn

[S24] C：获取本地时间
来源：http://wcy.yuxming.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://iqp.fktsv.cn

[S25] C：内存拷贝
来源：http://xvw.ehwqpu.com

memcpy(dst, src, n);
来源：http://xog.quarkkingdee.top

[S26] C：内存清零
来源：http://dbg.aibaodan.cn

memset(a, 0, sizeof a);
来源：http://jye.dashuyun.cn

[S27] C：定义常量
来源：http://can.hnqzz.top

const double PI = 3.14159;
来源：http://lsa.chenlongwang.top

[S28] C：静态变量
来源：http://oep.hnxiangtu.top

static int counter = 0;
来源：http://dhi.jlsjyb.cn

[S29] C：变参函数
来源：http://nfi.aibaodan.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rnj.yangfankeji.com

[S30] C：头文件保护
来源：http://abc.xylfe.cn

#ifndef X_H
来源：http://yqv.zhoulong.xyz

#define X_H
来源：http://nct.hesvh.cn

#endif
来源：http://jrr.hfpthk.cn

[S31] C++：Hello World
来源：http://agi.jqgfzy.top

#include <iostream>
来源：http://yji.bbcook.cn

int main() { std::cout << "Hello\n"; }
来源：http://oqx.iojbl.cn

[S32] C++：字符串
来源：http://een.epnwcf.com

std::string s = "hi";  s += "!";
来源：http://rcg.yanxiufei.cn

[S33] C++：vector 增删
来源：http://odh.vqdsnc.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pld.pycfn.com

[S34] C++：遍历 vector
来源：http://ubt.ywan-chungtsiang.top

for (auto &x : v) { std::cout << x; }
来源：http://dvj.chenzaomai.com

[S35] C++：map
来源：http://pnb.bbcook.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://esu.chenzaomai.com

[S36] C++：unordered_map
来源：http://oxg.yanxiufei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sqs.ydzc1.top

[S37] C++：set
来源：http://hhj.chenjidiqi.icu

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gjw.sysykeji.top

[S38] C++：排序
来源：http://zfg.kuanghao11.cn

std::sort(v.begin(), v.end());
来源：http://dcr.xziqi.cn

[S39] C++：自定义比较器排序
来源：http://kom.jlsjyb.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ven.jqgfzy.top

[S40] C++：查找元素
来源：http://tex.chenzaomai.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zar.jlsjyb.cn

[S41] C++：类与构造函数
来源：http://hzw.ctjpmb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wqo.gzhubu.top

[S42] C++：继承与虚函数
来源：http://xzt.yuanzhike.top

class B : public Base { public: void f() override {} };
来源：http://hjg.zhaomingkeji.xyz

[S43] C++：智能指针
来源：http://plr.havefunace.top

auto p = std::make_unique<int>(5);
来源：http://kmu.yuanzhike.top

[S44] C++：引用传参
来源：http://jag.ywan-chungtsiang.top

void inc(int &x) { ++x; }
来源：http://yke.xuanzx.com

[S45] C++：lambda
来源：http://pwc.sxryk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nkq.dashuyun.cn

[S46] C++：函数模板
来源：http://oti.nanxuanxn.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kwf.kuanghao11.cn

[S47] C++：结构化绑定遍历
来源：http://cfa.316326.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kzk.52xcode.cn

[S48] C++：逐行读文件
来源：http://eqf.epnwcf.com

std::ifstream in("a.txt");  std::string line;
来源：http://rmk.cashguo.top

while (std::getline(in, line)) { }
来源：http://hya.andypj.xyz

[S49] C++：写文件
来源：http://wfc.ppjwa.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tgd.bbcook.cn

[S50] C++：格式化数字
来源：http://edy.hongshengwenyu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dcf.ctjpmb.com

[S51] C++：显式类型转换
来源：http://yqf.tian-w.cn

static_cast<double>(a) / b
来源：http://vsi.yangfankeji.com

[S52] C++：const 与 noexcept
来源：http://sib.shzxlz.cn

int size() const noexcept { return n_; }
来源：http://mkm.andypj.xyz

[S53] C++：移动语义
来源：http://mlp.cdnleiting.top

std::vector<int> w = std::move(v);
来源：http://ngv.cucudq.cn

[S54] C++：异常处理
来源：http://gcl.jinghuilouyu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hbw.smart0.xyz

[S55] C++：结构化绑定
来源：http://jwv.ydjk.org.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qic.nwbrower.top

[S56] C++：optional
来源：http://pqo.andypj.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bdn.shanyushiyangkeji.top

[S57] C++：编译期常量
来源：http://lff.dianchejie.cn

constexpr int N = 10;
来源：http://nqv.tanke756.top

[S58] C++：命名空间
来源：http://yzz.havefunace.top

namespace ns { int f() { return 1; } }
来源：http://ihj.52xcode.cn

[S59] C++：静态断言
来源：http://ggd.fktsv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xyu.yj202588.top

[S60] C++：遍历并删除元素
来源：http://mjf.yuanzhike.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ygw.yuanzhike.top

================================================================================
来源：http://psf.andypj.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zjd.yj20258888.top

================================================================================
来源：http://leb.tanke756.top

[T01] Kotlin：Hello World
来源：http://kth.smart0.xyz

println("Hello")
来源：http://xlz.tanke756.top

[T02] Kotlin：变量
来源：http://tth.snrcjt.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wwx.ydjk.org.cn

[T03] Kotlin：字符串模板
来源：http://upj.bjfxy.top

"值: $b"
来源：http://tkr.shuidangran.top

[T04] Kotlin：空安全
来源：http://cgv.havefunace.top

val n: String? = null;  n?.length
来源：http://plj.jlsjyb.cn

[T05] Kotlin：when 表达式
来源：http://jys.jqgfzy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wja.ywan-chungtsiang.top

[T06] Kotlin：集合映射
来源：http://npe.havefunace.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zom.tanke756.top

[T07] Kotlin：集合过滤
来源：http://swl.jqgfzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mbx.shuidangran.top

[T08] Kotlin：数据类
来源：http://wnr.yvedp.cn

data class User(val name: String, val age: Int)
来源：http://nsp.ydzc1.top

[T09] Kotlin：扩展函数
来源：http://jmd.fengsongda.top

fun String.exclaim() = this + "!"
来源：http://tsh.guannengcc.top

[T10] Kotlin：默认参数
来源：http://smu.shanyushiyangkeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vcg.wangshuangyany.cn

[T11] Kotlin：协程
来源：http://hke.yangfankeji.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://elh.zhijiandao.cn

[T12] Kotlin：解构声明
来源：http://xby.iojbl.cn

val (a, b) = Pair(1, 2)
来源：http://dxm.yuanzhike.top

[T13] Kotlin：只读 Map
来源：http://okl.gzhubu.top

val m = mapOf("a" to 1)
来源：http://hny.yuxming.cn

[T14] Kotlin：循环
来源：http://tyl.xinyue.icu

for (i in 1..10) println(i)
来源：http://bea.9152youxi.cn

[T15] Kotlin：接口
来源：http://wka.quarkkingdee.top

interface Shape { fun area(): Double }
来源：http://ksk.yj20258.top

[T16] Swift：Hello World
来源：http://dfl.xuanzx.com

print("Hello")
来源：http://www.chenzaomai.com

[T17] Swift：变量与常量
来源：http://bzw.chenzaomai.com

var a = 1;  let b = 2
来源：http://dmp.ehwqpu.com

[T18] Swift：字符串插值
来源：http://bwf.andypj.xyz

"值: \(b)"
来源：http://xyt.cashguo.top

[T19] Swift：可选绑定
来源：http://cvg.smart0.xyz

if let n = opt { print(n) }
来源：http://wtw.shanyushiyangkeji.top

[T20] Swift：数组操作
来源：http://cjw.shanyushiyangtech.top

var a = [1, 2, 3];  a.append(4)
来源：http://dpm.ydzc1.top

[T21] Swift：遍历
来源：http://cbv.haohaochexian.top

for x in a { print(x) }
来源：http://eci.snrcjt.cn

[T22] Swift：字典
来源：http://evm.sweek.top

var d = ["a": 1];  d["b"] = 2
来源：http://zfw.dianchejie.cn

[T23] Swift：函数
来源：http://umg.sxryk.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rbk.haohaochexian.top

[T24] Swift：闭包
来源：http://mvd.yj202588.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://iwx.c1oappe.top

[T25] Swift：结构体
来源：http://cmg.birdmap.top

struct P { var x: Int }
来源：http://tlj.hcnkem.com

[T26] Swift：类与重写
来源：http://bvd.sufxvd.cn

class A: Base { override func f() {} }
来源：http://uft.tanke756.top

[T27] Swift：错误处理
来源：http://ewh.wangdashe.top

do { try f() } catch { print(error) }
来源：http://rpu.yvedp.cn

[T28] Swift：枚举
来源：http://tbm.yongpay.top

enum Color { case red, green }
来源：http://cdk.birdmap.top

[T29] Swift：guard 提前返回
来源：http://aia.tarul.cn

guard let x = opt else { return }
来源：http://mqd.jqgufenzy.top

[T30] Swift：协议
来源：http://ygp.yj20258.top

protocol Shape { func area() -> Double }
来源：http://tte.yangfankeji.com

[T31] Lua：Hello World
来源：http://acu.gogol.net.cn

print("Hello")
来源：http://fum.gogol.net.cn

[T32] Lua：局部变量
来源：http://jcv.ybcxt.top

local a = 1
来源：http://mmk.yfazqb.com

[T33] Lua：表（数组）
来源：http://bvi.guannengcc.top

local t = {1, 2, 3};  t[4] = 4
来源：http://tto.ywan-chungtsiang.top

[T34] Lua：遍历表
来源：http://jev.xinyue.icu

for i, v in ipairs(t) do print(i, v) end
来源：http://pjz.vqdsnc.cn

[T35] Lua：字典表
来源：http://wjz.jiagoushi.top

local d = { a = 1 };  d.b = 2
来源：http://cqj.guowangkeji.top

[T36] Lua：函数
来源：http://hii.sjlbkw.cn

function add(a, b) return a + b end
来源：http://los.cucudq.cn

[T37] Lua：字符串拼接
来源：http://jwm.xuetiantiany.cn

"a" .. "b"
来源：http://wel.uphjek.com

[T38] Lua：条件
来源：http://qfq.cdnleiting.top

if x > 0 then print("正") end
来源：http://lsn.hnxiangtu.top

[T39] Lua：模式匹配
来源：http://hhl.jlsjyb.cn

string.find(s, "%d+")
来源：http://dzw.guowangkeji.top

[T40] Lua：元表
来源：http://mmo.yangfankeji.com

setmetatable({}, { __index = base })
来源：http://dzk.havefunace.top

[T41] Perl：Hello World
来源：http://hit.hcnkem.com

print "Hello\n";
来源：http://emb.xziqi.cn

[T42] Perl：变量类型
来源：http://mbn.hfpthk.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ajb.shuidangran.top

[T43] Perl：字符串插值
来源：http://xrp.quarkkingdee.top

"值: $a"
来源：http://tbt.zdqjudy.top

[T44] Perl：条件
来源：http://idu.cashguo.top

if ($a > 0) { print "正"; }
来源：http://awn.jinghuilouyu.cn

[T45] Perl：数组遍历
来源：http://pzs.hcnkem.com

for my $x (@arr) { print $x; }
来源：http://oyt.52xcode.cn

[T46] Perl：哈希操作
来源：http://alu.9152youxi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yvj.meibo888.top

[T47] Perl：正则捕获
来源：http://utu.ppjwa.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wom.sufxvd.cn

[T48] Perl：正则替换
来源：http://fin.0kj1m.cn

$s =~ s/old/new/g;
来源：http://hgg.gotoacloud.top

[T49] Perl：函数
来源：http://hmf.hammf.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gem.tianlin.xyz

[T50] Perl：逐行读文件
来源：http://aps.birdmap.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jpv.jqgufenzy.top

while (my $line = <$fh>) { print $line; }
来源：http://utj.fengsongda.top

[T51] Scala：Hello World
来源：http://bxo.fanxiaobao.xyz

println("Hello")
来源：http://jgy.sjlbkw.cn

[T52] Scala：变量
来源：http://exq.daxiang520.top

val a = 1;  var b = 2
来源：http://nwe.ehwqpu.com

[T53] Scala：字符串插值
来源：http://jrt.vqdsnc.cn

s"值: $b"
来源：http://gya.feifeiyinyue.top

[T54] Scala：集合映射
来源：http://cge.gaohongyu789.top

List(1, 2, 3).map(_ * 2)
来源：http://klq.shuidangran.top

[T55] Scala：集合过滤
来源：http://opj.guannengcc.top

List(1, 2, 3).filter(_ > 1)
来源：http://cqj.yuanzhike.top

[T56] Scala：样例类
来源：http://hff.shanyushiyangtech.top

case class User(name: String, age: Int)
来源：http://gpw.zycfv.cn

[T57] Scala：模式匹配
来源：http://jyd.epnwcf.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://aoa.zycfv.cn

[T58] Scala：函数定义
来源：http://ocn.jqgfzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://wub.xylfe.cn

[T59] Scala：循环
来源：http://qbe.zdqjudy.top

for (i <- 1 to 10) println(i)
来源：http://twv.jinghuilouyu.cn

[T60] Scala：折叠
来源：http://hiu.bbcook.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cua.epnwcf.com

================================================================================
来源：http://pga.haohaochexian.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wso.0kj1m.cn

================================================================================
来源：http://uwz.cqqwz.cn


<!-- 参考信息 -->