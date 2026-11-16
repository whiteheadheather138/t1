代发 wailian999

ssh user@host 'uptime'
来源：http://lmv.yuanzhike.top

[R58] 下载文件
来源：http://vvx.dashuyun.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://end.yangfankeji.com

[R59] 发 POST JSON
来源：http://avn.sxryk.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hoq.chenjidiqi.icu

[R60] 只看 HTTP 状态码
来源：http://fpr.hysaishi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kcz.jianghu66.top

[R61] 磁盘占用
来源：http://kco.shanyushiyangkeji.top

df -h;  du -sh *
来源：http://upu.yj20258888.top

[R62] 找最占空间的文件
来源：http://fxw.smart0.xyz

du -ah . | sort -rh | head -10
来源：http://yrc.jiagoushi.top

[R63] 内存与进程
来源：http://dbw.jinqigufen.top

free -h;  ps aux | grep nginx
来源：http://anm.haohaochexian.top

[R64] 结束进程
来源：http://cfu.shangyingyoupin.top

kill -9 $(pgrep -f app.py)
来源：http://jjs.ppjwa.cn

[R65] 查看端口占用
来源：http://zdi.zdqjudy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qny.iojbl.cn

[R66] 定时任务
来源：http://ngb.yangfankeji.com

crontab -e;  crontab -l
来源：http://gja.ywan-chungtsiang.top

[R67] 生成随机十六进制串
来源：http://pju.cucudq.cn

openssl rand -hex 16
来源：http://jqp.hongshengwenyu.top

[R68] 计算文件校验值
来源：http://lio.havefunace.top

sha256sum a.txt;  md5sum a.txt
来源：http://cbo.tian-w.cn

[R69] 生成随机密码
来源：http://ifb.zdbjq.cn

head -c 16 /dev/urandom | base64
来源：http://pbx.jqgufenzy.top

[R70] 时间戳与互转
来源：http://iyu.zhiwuduotai.top

date +%s;  date -d @1700000000
来源：http://bmr.sxryk.cn

[R71] 日期格式化
来源：http://fds.aizwys.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://env.hnqzz.top

[R72] 等待端口就绪
来源：http://wrl.zycfv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jdx.yueranfly.top

[R73] 分割大日志
来源：http://var.zhoulong.xyz

split -l 1000 big.log part_
来源：http://olf.shanyushiyangkeji.top

[R74] 批量重命名
来源：http://mlw.jlsjyb.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ayl.ehwqpu.com

[R75] 导出环境变量
来源：http://ave.c1oappe.top

export PATH="$HOME/bin:$PATH"
来源：http://gos.zdbjq.cn

[R76] 使用临时文件
来源：http://obp.aibaodan.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://agu.yvedp.cn

[R77] 读取用户输入
来源：http://btd.sufxvd.cn

read -rp "请输入: " ans
来源：http://wpm.svipenyu.cn

[R78] 交互式菜单
来源：http://zok.vehdjk.com

select opt in a b c; do echo "$opt"; break; done
来源：http://tec.52xcode.cn

[R79] 解析命令行选项
来源：http://pvy.snrcjt.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nge.yj202588.top

[R80] 查看脚本执行耗时
来源：http://hmx.yvedp.cn

time ./run.sh
来源：http://jjf.nanxinkj.top

================================================================================
来源：http://frk.daria6918.cn

S. C / C++ 专题
来源：http://sll.sweek.top

================================================================================
来源：http://coa.hongshengwenyu.top

[S01] C：Hello World
来源：http://pqu.fanxiaobao.xyz

#include <stdio.h>
来源：http://izb.zhaomingkeji.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://spw.jlsjyb.cn

[S02] C：变量与格式化输出
来源：http://zqz.cqqwz.cn

int a = 10; printf("%d\n", a);
来源：http://loh.bbcook.cn

[S03] C：读入整数
来源：http://gcc.yj20258.top

int x; scanf("%d", &x);
来源：http://ylo.52xcode.cn

[S04] C：字符串复制
来源：http://esv.cdnleiting.top

char dst[32]; strcpy(dst, "hi");
来源：http://ibq.shzxlz.cn

[S05] C：字符串长度
来源：http://ywq.c1oappe.top

strlen(s)
来源：http://bix.yueranfly.top

[S06] C：字符串比较
来源：http://swb.xylfe.cn

strcmp(a, b) == 0
来源：http://llx.jqgufenzy.top

[S07] C：数组遍历求和
来源：http://jji.gzhubu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yzg.ydzc1.top

[S08] C：动态内存分配与释放
来源：http://eio.zhijiandao.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fkj.jiagoushi.top

[S09] C：结构体定义与初始化
来源：http://vtk.fanxiaobao.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cjq.kuanghao11.cn

[S10] C：指针与解引用
来源：http://nin.chenlongwang.top

int *p = &a;  *p = 5;
来源：http://fud.xuetiantiany.cn

[S11] C：逐行读文件
来源：http://yco.yvedp.cn

FILE *f = fopen("a.txt", "r");
来源：http://pfl.xingfuxueyuan.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://qre.shangyingyoupin.top

fclose(f);
来源：http://wvm.ybcxt.top

[S12] C：写文件
来源：http://dto.kuanghao11.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bfv.zycfv.cn

[S13] C：宏定义
来源：http://grw.yongpay.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dnz.ybcxt.top

[S14] C：枚举
来源：http://agh.fzhhl.top

enum Color { RED, GREEN, BLUE };
来源：http://uiu.xuetiantiany.cn

[S15] C：类型转换
来源：http://dyv.yanxiufei.cn

(double) a / b
来源：http://ked.gzhubu.top

[S16] C：位操作置位
来源：http://iif.cucudq.cn

x |= (1 << 3);
来源：http://pms.sweek.top

[S17] C：安全拼接字符串
来源：http://hzp.pycfn.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yus.mhx1999.top

[S18] C：命令行参数
来源：http://jhf.fzhhl.top

int main(int argc, char **argv)
来源：http://cau.vehdjk.com

[S19] C：快速排序
来源：http://kky.bbcook.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ugd.aizwys.cn

[S20] C：二分查找
来源：http://mvg.yuanzhike.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hgg.tian-w.cn

[S21] C：字符类别判断
来源：http://dps.hnxiangtu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lds.shanyushiyangtech.top

[S22] C：字符串转数字
来源：http://cly.redwolf501.top

atoi("42");  strtod("3.14", NULL);
来源：http://pmn.gaohongyu789.top

[S23] C：随机数
来源：http://vcw.shanyushiyangkeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://szo.zdqjudy.top

[S24] C：获取本地时间
来源：http://vxv.fengsongda.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vsg.xingfuxueyuan.xyz

[S25] C：内存拷贝
来源：http://jgd.zhongyouzk.top

memcpy(dst, src, n);
来源：http://xpu.zhiwuduotai.top

[S26] C：内存清零
来源：http://hsw.shzxlz.cn

memset(a, 0, sizeof a);
来源：http://uxu.shzxlz.cn

[S27] C：定义常量
来源：http://emj.mhx1999.top

const double PI = 3.14159;
来源：http://jnl.pengpengdd.cyou

[S28] C：静态变量
来源：http://svs.sxryk.cn

static int counter = 0;
来源：http://eyt.0kj1m.cn

[S29] C：变参函数
来源：http://kvt.jlsjyb.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ngb.vqdsnc.cn

[S30] C：头文件保护
来源：http://yle.nwbrower.top

#ifndef X_H
来源：http://mqq.52xcode.cn

#define X_H
来源：http://bll.dianchejie.cn

#endif
来源：http://rzz.chenzaomai.com

[S31] C++：Hello World
来源：http://lfp.zhixingplan.top

#include <iostream>
来源：http://hwj.nanxinkj.top

int main() { std::cout << "Hello\n"; }
来源：http://tfx.zhaomingkeji.xyz

[S32] C++：字符串
来源：http://jpk.pycfn.com

std::string s = "hi";  s += "!";
来源：http://eyt.chenjidiqi.icu

[S33] C++：vector 增删
来源：http://ljv.chenzaomai.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wko.xinyue.icu

[S34] C++：遍历 vector
来源：http://gre.ivvv.top

for (auto &x : v) { std::cout << x; }
来源：http://ncq.shangyingyoupin.top

[S35] C++：map
来源：http://ngu.yonumen.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tnw.zhongyouzk.top

[S36] C++：unordered_map
来源：http://luy.shuidangran.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://szn.jlsjyb.cn

[S37] C++：set
来源：http://qdy.hywenlv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zxu.meibo888.top

[S38] C++：排序
来源：http://mdy.sysykeji.top

std::sort(v.begin(), v.end());
来源：http://rdk.gzhubu.top

[S39] C++：自定义比较器排序
来源：http://rbd.zhengqikj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eqv.yuanzhike.top

[S40] C++：查找元素
来源：http://sfv.bbcook.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lug.jinyuanbaomall.cn

[S41] C++：类与构造函数
来源：http://jbt.zhixingplan.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oos.nwbrower.top

[S42] C++：继承与虚函数
来源：http://gys.hnqzz.top

class B : public Base { public: void f() override {} };
来源：http://gae.jqgufenzy.top

[S43] C++：智能指针
来源：http://zzz.zdqjudy.top

auto p = std::make_unique<int>(5);
来源：http://eyh.gotoacloud.top

[S44] C++：引用传参
来源：http://zso.hysaishi.cn

void inc(int &x) { ++x; }
来源：http://ojk.yj20258888.top

[S45] C++：lambda
来源：http://skc.sjlbkw.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vvn.gogol.net.cn

[S46] C++：函数模板
来源：http://yxq.yvedp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nws.xuanzx.com

[S47] C++：结构化绑定遍历
来源：http://bwi.aizwys.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bwd.iojbl.cn

[S48] C++：逐行读文件
来源：http://hpo.gotoacloud.top

std::ifstream in("a.txt");  std::string line;
来源：http://foe.c1oappe.top

while (std::getline(in, line)) { }
来源：http://ezq.xuanzx.com

[S49] C++：写文件
来源：http://gur.ivvv.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ucy.birdmap.top

[S50] C++：格式化数字
来源：http://yfj.nanxinkj.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://geq.gaohongyu789.top

[S51] C++：显式类型转换
来源：http://gfu.vqdsnc.cn

static_cast<double>(a) / b
来源：http://wkc.xuetiantiany.cn

[S52] C++：const 与 noexcept
来源：http://iwr.jinyuanbaomall.cn

int size() const noexcept { return n_; }
来源：http://vvq.tianlin.xyz

[S53] C++：移动语义
来源：http://vdf.smart0.xyz

std::vector<int> w = std::move(v);
来源：http://dyg.shuidangran.top

[S54] C++：异常处理
来源：http://pxy.yonumen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rfw.hysaishi.cn

[S55] C++：结构化绑定
来源：http://cjr.0kj1m.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wyk.fzhhl.top

[S56] C++：optional
来源：http://ulm.guowangkeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pzi.ywan-chungtsiang.top

[S57] C++：编译期常量
来源：http://uic.zhongyouzk.top

constexpr int N = 10;
来源：http://yuj.zdqjudy.top

[S58] C++：命名空间
来源：http://byj.zdbjq.cn

namespace ns { int f() { return 1; } }
来源：http://mjl.fanxiaobao.xyz

[S59] C++：静态断言
来源：http://dci.aizwys.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eqr.jinqigufen.top

[S60] C++：遍历并删除元素
来源：http://zej.sufxvd.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://avw.fanxiaobao.xyz

================================================================================
来源：http://mil.fzhhl.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kld.yvedp.cn

================================================================================
来源：http://szt.bjfxy.top

[T01] Kotlin：Hello World
来源：http://jqc.uphjek.com

println("Hello")
来源：http://yfv.iojbl.cn

[T02] Kotlin：变量
来源：http://nyt.ivvv.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nrr.fktsv.cn

[T03] Kotlin：字符串模板
来源：http://mhp.shangyingyoupin.top

"值: $b"
来源：http://vnl.sxryk.cn

[T04] Kotlin：空安全
来源：http://ioi.shuidangran.top

val n: String? = null;  n?.length
来源：http://pew.jinyuanbaomall.cn

[T05] Kotlin：when 表达式
来源：http://gez.gogol.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fnu.ywan-chungtsiang.top

[T06] Kotlin：集合映射
来源：http://pwr.yongpay.top

listOf(1, 2, 3).map { it * 2 }
来源：http://usk.kuanghao11.cn

[T07] Kotlin：集合过滤
来源：http://kvz.zhixingplan.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://krf.cashguo.top

[T08] Kotlin：数据类
来源：http://oiw.nanxinkj.top

data class User(val name: String, val age: Int)
来源：http://tvw.xuetiantiany.cn

[T09] Kotlin：扩展函数
来源：http://ijt.yonumen.top

fun String.exclaim() = this + "!"
来源：http://lmq.shanyushiyangtech.top

[T10] Kotlin：默认参数
来源：http://dwu.vqdsnc.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cmr.tarul.cn

[T11] Kotlin：协程
来源：http://jqz.sxryk.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://srx.jlsjyb.cn

[T12] Kotlin：解构声明
来源：http://yiz.zhijiandao.cn

val (a, b) = Pair(1, 2)
来源：http://tbw.cheryme.top

[T13] Kotlin：只读 Map
来源：http://spm.yueranfly.top

val m = mapOf("a" to 1)
来源：http://eca.yuanzhike.top

[T14] Kotlin：循环
来源：http://zum.yueranfly.top

for (i in 1..10) println(i)
来源：http://qeb.jinyuanbaomall.cn

[T15] Kotlin：接口
来源：http://lxm.chenzaomai.com

interface Shape { fun area(): Double }
来源：http://fav.gaohongyu789.top

[T16] Swift：Hello World
来源：http://asc.nanxinkj.top

print("Hello")
来源：http://vvz.zycfv.cn

[T17] Swift：变量与常量
来源：http://fyp.hnqzz.top

var a = 1;  let b = 2
来源：http://pmd.gzhubu.top

[T18] Swift：字符串插值
来源：http://mcl.iojbl.cn

"值: \(b)"
来源：http://yrb.cdnleiting.top

[T19] Swift：可选绑定
来源：http://flo.jlsjyb.cn

if let n = opt { print(n) }
来源：http://wrd.zhixingplan.top

[T20] Swift：数组操作
来源：http://ocq.mhx1999.top

var a = [1, 2, 3];  a.append(4)
来源：http://mop.zhengqikj.top

[T21] Swift：遍历
来源：http://phv.yj20258888.top

for x in a { print(x) }
来源：http://lae.jinghuilouyu.cn

[T22] Swift：字典
来源：http://nuw.cheryme.top

var d = ["a": 1];  d["b"] = 2
来源：http://xki.tian-w.cn

[T23] Swift：函数
来源：http://qvl.gogol.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lnp.aizwys.cn

[T24] Swift：闭包
来源：http://bmu.hammf.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rne.gaohongyu789.top

[T25] Swift：结构体
来源：http://brk.sxryk.cn

struct P { var x: Int }
来源：http://mgw.xuanzx.com

[T26] Swift：类与重写
来源：http://bmj.iojbl.cn

class A: Base { override func f() {} }
来源：http://jhf.nanxinkj.top

[T27] Swift：错误处理
来源：http://dhb.bbcook.cn

do { try f() } catch { print(error) }
来源：http://eyf.shanyushiyangtech.top

[T28] Swift：枚举
来源：http://dbz.haohaochexian.top

enum Color { case red, green }
来源：http://lvb.hnxiangtu.top

[T29] Swift：guard 提前返回
来源：http://ugv.yangfankeji.com

guard let x = opt else { return }
来源：http://nbv.feifeiyinyue.top

[T30] Swift：协议
来源：http://elg.kuanghao11.cn

protocol Shape { func area() -> Double }
来源：http://uef.bbcook.cn

[T31] Lua：Hello World
来源：http://ldl.uphjek.com

print("Hello")
来源：http://qbe.52xcode.cn

[T32] Lua：局部变量
来源：http://chd.52xcode.cn

local a = 1
来源：http://pfh.sjlbkw.cn

[T33] Lua：表（数组）
来源：http://zcq.hfpthk.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nyd.jinqigufen.top

[T34] Lua：遍历表
来源：http://xbi.yanxiufei.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://izv.cucudq.cn

[T35] Lua：字典表
来源：http://vir.uphjek.com

local d = { a = 1 };  d.b = 2
来源：http://ulo.feifeiyinyue.top

[T36] Lua：函数
来源：http://etr.hywenlv.cn

function add(a, b) return a + b end
来源：http://xrw.9152youxi.cn

[T37] Lua：字符串拼接
来源：http://nmx.kuanghao11.cn

"a" .. "b"
来源：http://vbb.daxiang520.top

[T38] Lua：条件
来源：http://ksq.zdbjq.cn

if x > 0 then print("正") end
来源：http://jue.ctjpmb.com

[T39] Lua：模式匹配
来源：http://yhu.yanxiufei.cn

string.find(s, "%d+")
来源：http://bau.aibaodan.cn

[T40] Lua：元表
来源：http://mrv.jianghu66.top

setmetatable({}, { __index = base })
来源：http://ved.fehbvm.com

[T41] Perl：Hello World
来源：http://gql.gogol.net.cn

print "Hello\n";
来源：http://vlv.zdbjq.cn

[T42] Perl：变量类型
来源：http://ein.zhixingplan.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fqy.ctjpmb.com

[T43] Perl：字符串插值
来源：http://pnl.daxiang520.top

"值: $a"
来源：http://xmp.jqgfzy.top

[T44] Perl：条件
来源：http://dhk.shanyushiyangkeji.top

if ($a > 0) { print "正"; }
来源：http://obk.chenzaomai.com

[T45] Perl：数组遍历
来源：http://wfe.yj202588.top

for my $x (@arr) { print $x; }
来源：http://wuw.uphjek.com

[T46] Perl：哈希操作
来源：http://byc.yj202588.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sqy.iojbl.cn

[T47] Perl：正则捕获
来源：http://ntp.gzhubu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://auk.chenjidiqi.icu

[T48] Perl：正则替换
来源：http://kny.guowangkeji.top

$s =~ s/old/new/g;
来源：http://cvx.52xcode.cn

[T49] Perl：函数
来源：http://wlw.jlsjyb.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://azm.kuanghao11.cn

[T50] Perl：逐行读文件
来源：http://hth.jyoumei.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://khm.ppjwa.cn

while (my $line = <$fh>) { print $line; }
来源：http://bvv.316326.xyz

[T51] Scala：Hello World
来源：http://lxs.hywenlv.cn

println("Hello")
来源：http://qqx.bbcook.cn

[T52] Scala：变量
来源：http://cav.sjlbkw.cn

val a = 1;  var b = 2
来源：http://hld.hnxiangtu.top

[T53] Scala：字符串插值
来源：http://gpc.chenjidiqi.icu

s"值: $b"
来源：http://aks.aibaodan.cn

[T54] Scala：集合映射
来源：http://jbb.svipenyu.cn

List(1, 2, 3).map(_ * 2)
来源：http://wkj.aizwys.cn

[T55] Scala：集合过滤
来源：http://mvp.shanyushiyangkeji.top

List(1, 2, 3).filter(_ > 1)
来源：http://kxa.jinghuilouyu.cn

[T56] Scala：样例类
来源：http://ytn.fzhhl.top

case class User(name: String, age: Int)
来源：http://pjk.xylfe.cn

[T57] Scala：模式匹配
来源：http://edo.fzhhl.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://atu.shuidangran.top

[T58] Scala：函数定义
来源：http://aqp.chenzaomai.com

def add(a: Int, b: Int): Int = a + b
来源：http://gsq.jyoumei.cn

[T59] Scala：循环
来源：http://ays.jinqigfzy.top

for (i <- 1 to 10) println(i)
来源：http://gmx.shzxlz.cn

[T60] Scala：折叠
来源：http://tjy.zhiwuduotai.top


<!-- 参考信息 -->