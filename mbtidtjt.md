代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wth.shuidangran.top

[R60] 只看 HTTP 状态码
来源：http://jrn.hysaishi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cpf.zhoulong.xyz

[R61] 磁盘占用
来源：http://hbc.sweek.top

df -h;  du -sh *
来源：http://bal.guowangkeji.top

[R62] 找最占空间的文件
来源：http://piu.hongshengwenyu.top

du -ah . | sort -rh | head -10
来源：http://dzs.hnqzz.top

[R63] 内存与进程
来源：http://yvw.chenzaomai.com

free -h;  ps aux | grep nginx
来源：http://bcz.gogol.net.cn

[R64] 结束进程
来源：http://zsw.cashguo.top

kill -9 $(pgrep -f app.py)
来源：http://dze.wangshuangyany.cn

[R65] 查看端口占用
来源：http://cmt.jinghuilouyu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://eyj.xinyue.icu

[R66] 定时任务
来源：http://qay.yuanzhike.top

crontab -e;  crontab -l
来源：http://val.shzxlz.cn

[R67] 生成随机十六进制串
来源：http://ifb.0kj1m.cn

openssl rand -hex 16
来源：http://tpb.nanxuanxn.top

[R68] 计算文件校验值
来源：http://lzd.c1oappe.top

sha256sum a.txt;  md5sum a.txt
来源：http://bdz.bjfxy.top

[R69] 生成随机密码
来源：http://xgj.feifeiyinyue.top

head -c 16 /dev/urandom | base64
来源：http://tsy.52xcode.cn

[R70] 时间戳与互转
来源：http://mic.bjfxy.top

date +%s;  date -d @1700000000
来源：http://nud.cheryme.top

[R71] 日期格式化
来源：http://act.tian-w.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://krs.hywenlv.cn

[R72] 等待端口就绪
来源：http://qkv.iojbl.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wxg.hfpthk.cn

[R73] 分割大日志
来源：http://evx.bjfxy.top

split -l 1000 big.log part_
来源：http://mzi.yj202588.top

[R74] 批量重命名
来源：http://dfs.meibo888.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zzg.daria6918.cn

[R75] 导出环境变量
来源：http://yaj.vehdjk.com

export PATH="$HOME/bin:$PATH"
来源：http://cqw.yueranfly.top

[R76] 使用临时文件
来源：http://lvf.pengpengdd.cyou

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tjv.hesvh.cn

[R77] 读取用户输入
来源：http://nof.zhoulong.xyz

read -rp "请输入: " ans
来源：http://amm.hnqzz.top

[R78] 交互式菜单
来源：http://zoa.hysaishi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sis.gogol.net.cn

[R79] 解析命令行选项
来源：http://gkj.snrcjt.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fqe.aizwys.cn

[R80] 查看脚本执行耗时
来源：http://haj.yvedp.cn

time ./run.sh
来源：http://snr.feifeiyinyue.top

================================================================================
来源：http://pti.yuanzhike.top

S. C / C++ 专题
来源：http://vcf.bbcook.cn

================================================================================
来源：http://rta.cucudq.cn

[S01] C：Hello World
来源：http://jox.yuanzhike.top

#include <stdio.h>
来源：http://yqm.wangdashe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xfu.xziqi.cn

[S02] C：变量与格式化输出
来源：http://xig.zhijiandao.cn

int a = 10; printf("%d\n", a);
来源：http://ixp.jqgufenzy.top

[S03] C：读入整数
来源：http://frc.xuanzx.com

int x; scanf("%d", &x);
来源：http://vth.shanyushiyangkeji.top

[S04] C：字符串复制
来源：http://eam.ppjwa.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yxu.daria6918.cn

[S05] C：字符串长度
来源：http://pek.ydzc1.top

strlen(s)
来源：http://irq.sysykeji.top

[S06] C：字符串比较
来源：http://seg.yuanzhike.top

strcmp(a, b) == 0
来源：http://mxm.cashguo.top

[S07] C：数组遍历求和
来源：http://myj.chenlongwang.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vex.yj202588.top

[S08] C：动态内存分配与释放
来源：http://xmq.shangyingyoupin.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xzs.tianlin.xyz

[S09] C：结构体定义与初始化
来源：http://fzs.hesvh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ugf.gogol.net.cn

[S10] C：指针与解引用
来源：http://epw.0kj1m.cn

int *p = &a;  *p = 5;
来源：http://mzw.yvedp.cn

[S11] C：逐行读文件
来源：http://zwr.yonumen.top

FILE *f = fopen("a.txt", "r");
来源：http://fni.fanxiaobao.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://xuq.yueranfly.top

fclose(f);
来源：http://fwk.hywenlv.cn

[S12] C：写文件
来源：http://kto.c1oappe.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jxf.shzxlz.cn

[S13] C：宏定义
来源：http://tqn.yuanzhike.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xzt.cqqwz.cn

[S14] C：枚举
来源：http://kel.52xcode.cn

enum Color { RED, GREEN, BLUE };
来源：http://wfe.jianghu66.top

[S15] C：类型转换
来源：http://uub.shzxlz.cn

(double) a / b
来源：http://lwi.hcnkem.com

[S16] C：位操作置位
来源：http://ppj.yangfankeji.com

x |= (1 << 3);
来源：http://ccy.nanxuanxn.top

[S17] C：安全拼接字符串
来源：http://jay.yuxming.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://leg.hnqzz.top

[S18] C：命令行参数
来源：http://vuw.ybcxt.top

int main(int argc, char **argv)
来源：http://ewu.pengpengdd.cyou

[S19] C：快速排序
来源：http://hzu.chenjidiqi.icu

qsort(a, n, sizeof(int), cmp);
来源：http://log.guannengcc.top

[S20] C：二分查找
来源：http://kjm.jyoumei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nsy.zhiwuduotai.top

[S21] C：字符类别判断
来源：http://hyr.hesvh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uhr.shanyushiyangtech.top

[S22] C：字符串转数字
来源：http://sgt.ydzc1.top

atoi("42");  strtod("3.14", NULL);
来源：http://jos.fanxiaobao.xyz

[S23] C：随机数
来源：http://czd.nanxinkj.top

srand(time(NULL));  int r = rand() % 100;
来源：http://kry.hywenlv.cn

[S24] C：获取本地时间
来源：http://vwk.yanxiufei.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zey.gogol.net.cn

[S25] C：内存拷贝
来源：http://sar.zdbjq.cn

memcpy(dst, src, n);
来源：http://ivb.hysaishi.cn

[S26] C：内存清零
来源：http://kox.yj202588.top

memset(a, 0, sizeof a);
来源：http://sjl.shangyingyoupin.top

[S27] C：定义常量
来源：http://agn.yuxming.cn

const double PI = 3.14159;
来源：http://cje.jinghuilouyu.cn

[S28] C：静态变量
来源：http://mde.shzxlz.cn

static int counter = 0;
来源：http://sdy.feifeiyinyue.top

[S29] C：变参函数
来源：http://qxh.yvedp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yak.zycfv.cn

[S30] C：头文件保护
来源：http://xuc.cdnleiting.top

#ifndef X_H
来源：http://mzf.tanke756.top

#define X_H
来源：http://lgo.yangfankeji.com

#endif
来源：http://uwe.nwbrower.top

[S31] C++：Hello World
来源：http://yjo.jqgfzy.top

#include <iostream>
来源：http://vpe.xylfe.cn

int main() { std::cout << "Hello\n"; }
来源：http://foy.nanxinkj.top

[S32] C++：字符串
来源：http://mlu.guannengcc.top

std::string s = "hi";  s += "!";
来源：http://eeu.cheryme.top

[S33] C++：vector 增删
来源：http://ywu.sufxvd.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kxr.nanxinkj.top

[S34] C++：遍历 vector
来源：http://dqy.zhixingplan.top

for (auto &x : v) { std::cout << x; }
来源：http://biy.fehbvm.com

[S35] C++：map
来源：http://noy.uphjek.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://unb.chenzaomai.com

[S36] C++：unordered_map
来源：http://irr.aizwys.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yfu.jinqigufen.top

[S37] C++：set
来源：http://oqv.shuidangran.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ybf.52xcode.cn

[S38] C++：排序
来源：http://nez.cashguo.top

std::sort(v.begin(), v.end());
来源：http://whw.52xcode.cn

[S39] C++：自定义比较器排序
来源：http://yil.zhengqikj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tfw.chenjidiqi.icu

[S40] C++：查找元素
来源：http://tnk.fanxiaobao.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vav.jqgufenzy.top

[S41] C++：类与构造函数
来源：http://ydn.zhongyouzk.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://awn.yvedp.cn

[S42] C++：继承与虚函数
来源：http://ssh.hysaishi.cn

class B : public Base { public: void f() override {} };
来源：http://dnz.wangshuangyany.cn

[S43] C++：智能指针
来源：http://ppq.sweek.top

auto p = std::make_unique<int>(5);
来源：http://evl.cashguo.top

[S44] C++：引用传参
来源：http://jbb.jinyuanbaomall.cn

void inc(int &x) { ++x; }
来源：http://olu.yfazqb.com

[S45] C++：lambda
来源：http://zun.cqqwz.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lzs.jinqigfzy.top

[S46] C++：函数模板
来源：http://zcq.ivvv.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wtu.sjlbkw.cn

[S47] C++：结构化绑定遍历
来源：http://qon.zhoulong.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ohk.gotoacloud.top

[S48] C++：逐行读文件
来源：http://ijj.cheryme.top

std::ifstream in("a.txt");  std::string line;
来源：http://ndh.mhx1999.top

while (std::getline(in, line)) { }
来源：http://sne.yfazqb.com

[S49] C++：写文件
来源：http://wri.ywan-chungtsiang.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ljv.iojbl.cn

[S50] C++：格式化数字
来源：http://zpc.sufxvd.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://erh.xinyue.icu

[S51] C++：显式类型转换
来源：http://kso.vehdjk.com

static_cast<double>(a) / b
来源：http://hzv.aizwys.cn

[S52] C++：const 与 noexcept
来源：http://bis.daxiang520.top

int size() const noexcept { return n_; }
来源：http://wqu.hnxiangtu.top

[S53] C++：移动语义
来源：http://pyj.zdbjq.cn

std::vector<int> w = std::move(v);
来源：http://bpi.gotoacloud.top

[S54] C++：异常处理
来源：http://ifs.hongshengwenyu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xld.shangyingyoupin.top

[S55] C++：结构化绑定
来源：http://eap.zdqjudy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://biv.jinqigfzy.top

[S56] C++：optional
来源：http://pgs.hesvh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mfz.yuanzhike.top

[S57] C++：编译期常量
来源：http://bcp.nwbrower.top

constexpr int N = 10;
来源：http://yih.uphjek.com

[S58] C++：命名空间
来源：http://wmd.fanxiaobao.xyz

namespace ns { int f() { return 1; } }
来源：http://vxf.dashuyun.cn

[S59] C++：静态断言
来源：http://hne.iojbl.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ygs.sweek.top

[S60] C++：遍历并删除元素
来源：http://upi.tianlin.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ujr.zhongyouzk.top

================================================================================
来源：http://zhs.chenzaomai.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fmo.hnxiangtu.top

================================================================================
来源：http://oif.316326.xyz

[T01] Kotlin：Hello World
来源：http://cpm.jinyuanbaomall.cn

println("Hello")
来源：http://rwb.xylfe.cn

[T02] Kotlin：变量
来源：http://dtk.feifeiyinyue.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ovy.hammf.cn

[T03] Kotlin：字符串模板
来源：http://ems.redwolf501.top

"值: $b"
来源：http://php.yj202588.top

[T04] Kotlin：空安全
来源：http://orl.pycfn.com

val n: String? = null;  n?.length
来源：http://klz.yangfankeji.com

[T05] Kotlin：when 表达式
来源：http://sxk.vqdsnc.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lee.xuetiantiany.cn

[T06] Kotlin：集合映射
来源：http://sop.gotoacloud.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tgk.pycfn.com

[T07] Kotlin：集合过滤
来源：http://mcu.sweek.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://hqc.daria6918.cn

[T08] Kotlin：数据类
来源：http://uyx.smart0.xyz

data class User(val name: String, val age: Int)
来源：http://rqf.cashguo.top

[T09] Kotlin：扩展函数
来源：http://afh.yj202588.top

fun String.exclaim() = this + "!"
来源：http://zaz.pycfn.com

[T10] Kotlin：默认参数
来源：http://bty.xylfe.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xdo.yueranfly.top

[T11] Kotlin：协程
来源：http://zre.shanyushiyangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://oml.yj20258.top

[T12] Kotlin：解构声明
来源：http://icd.zhixingplan.top

val (a, b) = Pair(1, 2)
来源：http://peg.nwbrower.top

[T13] Kotlin：只读 Map
来源：http://iif.hesvh.cn

val m = mapOf("a" to 1)
来源：http://xsy.chenjidiqi.icu

[T14] Kotlin：循环
来源：http://rmr.yj202588.top

for (i in 1..10) println(i)
来源：http://jyh.iojbl.cn

[T15] Kotlin：接口
来源：http://ksw.hesvh.cn

interface Shape { fun area(): Double }
来源：http://kpp.gaohongyu789.top

[T16] Swift：Hello World
来源：http://izm.9152youxi.cn

print("Hello")
来源：http://ibe.hysaishi.cn

[T17] Swift：变量与常量
来源：http://mxp.nanxinkj.top

var a = 1;  let b = 2
来源：http://afx.ydzc1.top

[T18] Swift：字符串插值
来源：http://zzz.hnqzz.top

"值: \(b)"
来源：http://kgi.jinghuilouyu.cn

[T19] Swift：可选绑定
来源：http://xta.ydjk.org.cn

if let n = opt { print(n) }
来源：http://dcd.zhixingplan.top

[T20] Swift：数组操作
来源：http://vvy.jiagoushi.top

var a = [1, 2, 3];  a.append(4)
来源：http://pnn.redwolf501.top

[T21] Swift：遍历
来源：http://dpv.hesvh.cn

for x in a { print(x) }
来源：http://oru.sysykeji.top

[T22] Swift：字典
来源：http://mqt.zdbjq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bxx.ybcxt.top

[T23] Swift：函数
来源：http://sjn.zdqjudy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://twl.hammf.cn

[T24] Swift：闭包
来源：http://ahg.birdmap.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://pef.hysaishi.cn

[T25] Swift：结构体
来源：http://znv.zhengqikj.top

struct P { var x: Int }
来源：http://qua.316326.xyz

[T26] Swift：类与重写
来源：http://rkv.yuxming.cn

class A: Base { override func f() {} }
来源：http://ijw.fzhhl.top

[T27] Swift：错误处理
来源：http://wuf.yj20258.top

do { try f() } catch { print(error) }
来源：http://osh.cashguo.top

[T28] Swift：枚举
来源：http://yhi.nanxinkj.top

enum Color { case red, green }
来源：http://hok.hnxiangtu.top

[T29] Swift：guard 提前返回
来源：http://pyd.zhijiandao.cn

guard let x = opt else { return }
来源：http://fps.hesvh.cn

[T30] Swift：协议
来源：http://gfq.svipenyu.cn

protocol Shape { func area() -> Double }
来源：http://cfl.zhijiandao.cn

[T31] Lua：Hello World
来源：http://ttt.jianghu66.top

print("Hello")
来源：http://fcg.aibaodan.cn

[T32] Lua：局部变量
来源：http://dvv.epnwcf.com

local a = 1
来源：http://mfl.iojbl.cn

[T33] Lua：表（数组）
来源：http://wvz.bbcook.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ugg.dianchejie.cn

[T34] Lua：遍历表
来源：http://ydp.jiagoushi.top

for i, v in ipairs(t) do print(i, v) end
来源：http://jcl.xinyue.icu

[T35] Lua：字典表
来源：http://kdm.uphjek.com

local d = { a = 1 };  d.b = 2
来源：http://bhn.daxiang520.top

[T36] Lua：函数
来源：http://qst.uphjek.com

function add(a, b) return a + b end
来源：http://zne.havefunace.top

[T37] Lua：字符串拼接
来源：http://pts.ybcxt.top

"a" .. "b"
来源：http://xmx.shanyushiyangkeji.top

[T38] Lua：条件
来源：http://hxr.chenlongwang.top

if x > 0 then print("正") end
来源：http://pju.yangfankeji.com

[T39] Lua：模式匹配
来源：http://pnq.zycfv.cn

string.find(s, "%d+")
来源：http://udv.shanyushiyangtech.top

[T40] Lua：元表
来源：http://frj.fehbvm.com

setmetatable({}, { __index = base })
来源：http://mos.sjlbkw.cn

[T41] Perl：Hello World
来源：http://daa.jinghuilouyu.cn

print "Hello\n";
来源：http://vrn.hysaishi.cn

[T42] Perl：变量类型
来源：http://tct.cdnleiting.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ebg.uphjek.com

[T43] Perl：字符串插值
来源：http://eem.vehdjk.com

"值: $a"
来源：http://vzn.zhongyouzk.top

[T44] Perl：条件
来源：http://eng.bjfxy.top

if ($a > 0) { print "正"; }
来源：http://rbb.guowangkeji.top

[T45] Perl：数组遍历
来源：http://bph.vehdjk.com

for my $x (@arr) { print $x; }
来源：http://sis.gaohongyu789.top

[T46] Perl：哈希操作
来源：http://mhk.daria6918.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ovq.wangdashe.top

[T47] Perl：正则捕获
来源：http://itl.zhixingplan.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://irk.cashguo.top

[T48] Perl：正则替换
来源：http://ivv.nanxinkj.top

$s =~ s/old/new/g;
来源：http://wrk.xuetiantiany.cn

[T49] Perl：函数
来源：http://rhm.aizwys.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://isx.xuanzx.com

[T50] Perl：逐行读文件
来源：http://esv.epnwcf.com

open my $fh, "<", "a.txt" or die $!;
来源：http://apj.hfpthk.cn

while (my $line = <$fh>) { print $line; }
来源：http://hda.cucudq.cn

[T51] Scala：Hello World
来源：http://exi.yanxiufei.cn

println("Hello")
来源：http://gef.zhixingplan.top

[T52] Scala：变量
来源：http://dek.yj202588.top

val a = 1;  var b = 2
来源：http://eoj.shuidangran.top

[T53] Scala：字符串插值
来源：http://cco.fehbvm.com

s"值: $b"
来源：http://zve.guannengcc.top

[T54] Scala：集合映射
来源：http://ynq.fzhhl.top

List(1, 2, 3).map(_ * 2)
来源：http://tbr.chenlongwang.top

[T55] Scala：集合过滤
来源：http://svo.9152youxi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hbu.jianghu66.top

[T56] Scala：样例类
来源：http://jhn.zhengqikj.top

case class User(name: String, age: Int)
来源：http://kzr.gotoacloud.top

[T57] Scala：模式匹配
来源：http://nns.snrcjt.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ouw.jinqigfzy.top

[T58] Scala：函数定义
来源：http://shl.316326.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://lho.xingfuxueyuan.xyz

[T59] Scala：循环
来源：http://onp.zhoulong.xyz

for (i <- 1 to 10) println(i)
来源：http://gjl.yonumen.top

[T60] Scala：折叠
来源：http://sla.nwbrower.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://spk.yongpay.top

================================================================================
来源：http://uoz.pycfn.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nkz.yj202588.top

================================================================================
来源：http://cmu.yangfankeji.com


<!-- 参考信息 -->