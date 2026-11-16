代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yfm.yj202588.top

[R60] 只看 HTTP 状态码
来源：http://edm.nanxinkj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://akd.zhijiandao.cn

[R61] 磁盘占用
来源：http://twh.yvedp.cn

df -h;  du -sh *
来源：http://wze.cqqwz.cn

[R62] 找最占空间的文件
来源：http://fzr.sjlbkw.cn

du -ah . | sort -rh | head -10
来源：http://tqc.ppjwa.cn

[R63] 内存与进程
来源：http://eiu.sweek.top

free -h;  ps aux | grep nginx
来源：http://dcr.xylfe.cn

[R64] 结束进程
来源：http://cvn.gaohongyu789.top

kill -9 $(pgrep -f app.py)
来源：http://lua.nanxuanxn.top

[R65] 查看端口占用
来源：http://qdi.aizwys.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cdl.cashguo.top

[R66] 定时任务
来源：http://bqp.jyoumei.cn

crontab -e;  crontab -l
来源：http://whl.jinqigufen.top

[R67] 生成随机十六进制串
来源：http://aep.9152youxi.cn

openssl rand -hex 16
来源：http://tpj.gogol.net.cn

[R68] 计算文件校验值
来源：http://hla.kuanghao11.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uob.zdbjq.cn

[R69] 生成随机密码
来源：http://jpg.guowangkeji.top

head -c 16 /dev/urandom | base64
来源：http://zie.fanxiaobao.xyz

[R70] 时间戳与互转
来源：http://ieg.jinqigfzy.top

date +%s;  date -d @1700000000
来源：http://fny.ppjwa.cn

[R71] 日期格式化
来源：http://kde.mhx1999.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jhf.ppjwa.cn

[R72] 等待端口就绪
来源：http://ild.feifeiyinyue.top

until nc -z localhost 3306; do sleep 1; done
来源：http://dwc.vehdjk.com

[R73] 分割大日志
来源：http://mlq.52xcode.cn

split -l 1000 big.log part_
来源：http://aew.ppjwa.cn

[R74] 批量重命名
来源：http://fqg.aizwys.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ebe.zhixingplan.top

[R75] 导出环境变量
来源：http://wwe.xziqi.cn

export PATH="$HOME/bin:$PATH"
来源：http://mtg.zdbjq.cn

[R76] 使用临时文件
来源：http://ctl.vehdjk.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fwl.fengsongda.top

[R77] 读取用户输入
来源：http://syy.ehwqpu.com

read -rp "请输入: " ans
来源：http://huz.haohaochexian.top

[R78] 交互式菜单
来源：http://kdo.0kj1m.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gdv.hammf.cn

[R79] 解析命令行选项
来源：http://wjp.hongshengwenyu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hnd.guowangkeji.top

[R80] 查看脚本执行耗时
来源：http://nqz.havefunace.top

time ./run.sh
来源：http://zow.snrcjt.cn

================================================================================
来源：http://lgp.52xcode.cn

S. C / C++ 专题
来源：http://mwg.wangshuangyany.cn

================================================================================
来源：http://emh.zdqjudy.top

[S01] C：Hello World
来源：http://bwy.vehdjk.com

#include <stdio.h>
来源：http://pcy.quarkkingdee.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://kii.ywan-chungtsiang.top

[S02] C：变量与格式化输出
来源：http://jad.sxryk.cn

int a = 10; printf("%d\n", a);
来源：http://ijg.chenzaomai.com

[S03] C：读入整数
来源：http://gtw.xylfe.cn

int x; scanf("%d", &x);
来源：http://xuh.aizwys.cn

[S04] C：字符串复制
来源：http://ayw.hcnkem.com

char dst[32]; strcpy(dst, "hi");
来源：http://dth.zhiwuduotai.top

[S05] C：字符串长度
来源：http://nod.yonumen.top

strlen(s)
来源：http://ria.gzhubu.top

[S06] C：字符串比较
来源：http://joe.havefunace.top

strcmp(a, b) == 0
来源：http://hgu.dianchejie.cn

[S07] C：数组遍历求和
来源：http://kiu.uphjek.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ksd.shanyushiyangkeji.top

[S08] C：动态内存分配与释放
来源：http://cko.zycfv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://krs.wangshuangyany.cn

[S09] C：结构体定义与初始化
来源：http://ueh.zhoulong.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ufx.chenlongwang.top

[S10] C：指针与解引用
来源：http://fky.zdqjudy.top

int *p = &a;  *p = 5;
来源：http://hwg.zhiwuduotai.top

[S11] C：逐行读文件
来源：http://pkr.sysykeji.top

FILE *f = fopen("a.txt", "r");
来源：http://npa.zhixingplan.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://pau.yanxiufei.cn

fclose(f);
来源：http://nrz.jinghuilouyu.cn

[S12] C：写文件
来源：http://huq.bjfxy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wew.vqdsnc.cn

[S13] C：宏定义
来源：http://pbv.chenlongwang.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yqw.xinyue.icu

[S14] C：枚举
来源：http://poa.nanxuanxn.top

enum Color { RED, GREEN, BLUE };
来源：http://xov.9152youxi.cn

[S15] C：类型转换
来源：http://ehm.yanxiufei.cn

(double) a / b
来源：http://itg.hywenlv.cn

[S16] C：位操作置位
来源：http://rjw.tarul.cn

x |= (1 << 3);
来源：http://kpz.yueranfly.top

[S17] C：安全拼接字符串
来源：http://tca.cucudq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zdh.meibo888.top

[S18] C：命令行参数
来源：http://bur.pycfn.com

int main(int argc, char **argv)
来源：http://jsr.zhixingplan.top

[S19] C：快速排序
来源：http://smq.andypj.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://hec.meibo888.top

[S20] C：二分查找
来源：http://aqf.guannengcc.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vzj.9152youxi.cn

[S21] C：字符类别判断
来源：http://sjg.xingfuxueyuan.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tos.xuetiantiany.cn

[S22] C：字符串转数字
来源：http://won.xuetiantiany.cn

atoi("42");  strtod("3.14", NULL);
来源：http://iiq.shangyingyoupin.top

[S23] C：随机数
来源：http://jrn.dianchejie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zrw.havefunace.top

[S24] C：获取本地时间
来源：http://wcp.quarkkingdee.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://njp.shuidangran.top

[S25] C：内存拷贝
来源：http://bor.jqgufenzy.top

memcpy(dst, src, n);
来源：http://qhs.cashguo.top

[S26] C：内存清零
来源：http://asz.zhoulong.xyz

memset(a, 0, sizeof a);
来源：http://zpz.guowangkeji.top

[S27] C：定义常量
来源：http://gmh.aibaodan.cn

const double PI = 3.14159;
来源：http://mju.jiagoushi.top

[S28] C：静态变量
来源：http://kmb.meibo888.top

static int counter = 0;
来源：http://ktt.dashuyun.cn

[S29] C：变参函数
来源：http://mym.meibo888.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fyu.daxiang520.top

[S30] C：头文件保护
来源：http://hza.aizwys.cn

#ifndef X_H
来源：http://udp.meibo888.top

#define X_H
来源：http://zgz.yanxiufei.cn

#endif
来源：http://vgf.hnxiangtu.top

[S31] C++：Hello World
来源：http://wmo.jianghu66.top

#include <iostream>
来源：http://pwt.chenjidiqi.icu

int main() { std::cout << "Hello\n"; }
来源：http://iah.fktsv.cn

[S32] C++：字符串
来源：http://pee.sweek.top

std::string s = "hi";  s += "!";
来源：http://nsj.hnqzz.top

[S33] C++：vector 增删
来源：http://vum.yj20258.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vvs.cqqwz.cn

[S34] C++：遍历 vector
来源：http://sni.shanyushiyangtech.top

for (auto &x : v) { std::cout << x; }
来源：http://rfg.fzhhl.top

[S35] C++：map
来源：http://cuo.zdbjq.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nzb.snrcjt.cn

[S36] C++：unordered_map
来源：http://qgt.c1oappe.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nab.hysaishi.cn

[S37] C++：set
来源：http://iif.zhaomingkeji.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fza.hnqzz.top

[S38] C++：排序
来源：http://aun.aizwys.cn

std::sort(v.begin(), v.end());
来源：http://oui.cucudq.cn

[S39] C++：自定义比较器排序
来源：http://sbe.daria6918.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ybg.hysaishi.cn

[S40] C++：查找元素
来源：http://qgy.tian-w.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xza.guannengcc.top

[S41] C++：类与构造函数
来源：http://mwr.havefunace.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://prm.daxiang520.top

[S42] C++：继承与虚函数
来源：http://uht.xylfe.cn

class B : public Base { public: void f() override {} };
来源：http://ctw.yuanzhike.top

[S43] C++：智能指针
来源：http://alw.316326.xyz

auto p = std::make_unique<int>(5);
来源：http://hta.hysaishi.cn

[S44] C++：引用传参
来源：http://hkk.fengsongda.top

void inc(int &x) { ++x; }
来源：http://peb.guowangkeji.top

[S45] C++：lambda
来源：http://kzt.ctjpmb.com

auto add = [](int a, int b) { return a + b; };
来源：http://yrl.fanxiaobao.xyz

[S46] C++：函数模板
来源：http://nvf.redwolf501.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://aug.zycfv.cn

[S47] C++：结构化绑定遍历
来源：http://nhd.mhx1999.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iwb.tanke756.top

[S48] C++：逐行读文件
来源：http://ukb.zhaomingkeji.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://oiv.bbcook.cn

while (std::getline(in, line)) { }
来源：http://vao.cheryme.top

[S49] C++：写文件
来源：http://mya.xylfe.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tlw.hfpthk.cn

[S50] C++：格式化数字
来源：http://ura.cashguo.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lfd.ivvv.top

[S51] C++：显式类型转换
来源：http://cqg.tarul.cn

static_cast<double>(a) / b
来源：http://yiu.xziqi.cn

[S52] C++：const 与 noexcept
来源：http://tvh.zhixingplan.top

int size() const noexcept { return n_; }
来源：http://ixr.svipenyu.cn

[S53] C++：移动语义
来源：http://omu.uphjek.com

std::vector<int> w = std::move(v);
来源：http://mkq.xuanzx.com

[S54] C++：异常处理
来源：http://qoo.9152youxi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kbf.pycfn.com

[S55] C++：结构化绑定
来源：http://tmk.sweek.top

auto [a, b] = std::make_pair(1, 2);
来源：http://bic.redwolf501.top

[S56] C++：optional
来源：http://mts.yj202588.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wqd.xylfe.cn

[S57] C++：编译期常量
来源：http://mnb.zdqjudy.top

constexpr int N = 10;
来源：http://sib.jinyuanbaomall.cn

[S58] C++：命名空间
来源：http://bzr.yuanzhike.top

namespace ns { int f() { return 1; } }
来源：http://llf.jqgufenzy.top

[S59] C++：静态断言
来源：http://tiu.gotoacloud.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lda.mhx1999.top

[S60] C++：遍历并删除元素
来源：http://zad.jiagoushi.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gzj.yfazqb.com

================================================================================
来源：http://bwu.vehdjk.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nxc.guowangkeji.top

================================================================================
来源：http://wqc.zhongyouzk.top

[T01] Kotlin：Hello World
来源：http://njs.ppjwa.cn

println("Hello")
来源：http://qbh.hcnkem.com

[T02] Kotlin：变量
来源：http://kwf.snrcjt.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://igb.ivvv.top

[T03] Kotlin：字符串模板
来源：http://nsx.guannengcc.top

"值: $b"
来源：http://waa.vqdsnc.cn

[T04] Kotlin：空安全
来源：http://qgh.daria6918.cn

val n: String? = null;  n?.length
来源：http://erh.guannengcc.top

[T05] Kotlin：when 表达式
来源：http://cdz.zhengqikj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xkz.zdbjq.cn

[T06] Kotlin：集合映射
来源：http://biv.bbcook.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vhm.daria6918.cn

[T07] Kotlin：集合过滤
来源：http://igj.aibaodan.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pdr.shanyushiyangkeji.top

[T08] Kotlin：数据类
来源：http://ylm.guannengcc.top

data class User(val name: String, val age: Int)
来源：http://cvz.hongshengwenyu.top

[T09] Kotlin：扩展函数
来源：http://vqr.shanyushiyangtech.top

fun String.exclaim() = this + "!"
来源：http://rqr.havefunace.top

[T10] Kotlin：默认参数
来源：http://lre.ivvv.top

fun greet(name: String = "World") = "Hi $name"
来源：http://hjm.c1oappe.top

[T11] Kotlin：协程
来源：http://zky.chenzaomai.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://faz.zhiwuduotai.top

[T12] Kotlin：解构声明
来源：http://ubr.chenjidiqi.icu

val (a, b) = Pair(1, 2)
来源：http://xar.gaohongyu789.top

[T13] Kotlin：只读 Map
来源：http://xlw.bbcook.cn

val m = mapOf("a" to 1)
来源：http://tie.fehbvm.com

[T14] Kotlin：循环
来源：http://ldn.hesvh.cn

for (i in 1..10) println(i)
来源：http://adj.xinyue.icu

[T15] Kotlin：接口
来源：http://gku.xylfe.cn

interface Shape { fun area(): Double }
来源：http://aly.shanyushiyangkeji.top

[T16] Swift：Hello World
来源：http://wzf.hysaishi.cn

print("Hello")
来源：http://ord.sjlbkw.cn

[T17] Swift：变量与常量
来源：http://wux.iojbl.cn

var a = 1;  let b = 2
来源：http://lsu.aibaodan.cn

[T18] Swift：字符串插值
来源：http://bvz.ppjwa.cn

"值: \(b)"
来源：http://wwl.fengsongda.top

[T19] Swift：可选绑定
来源：http://hsc.gogol.net.cn

if let n = opt { print(n) }
来源：http://mux.ppjwa.cn

[T20] Swift：数组操作
来源：http://ulk.havefunace.top

var a = [1, 2, 3];  a.append(4)
来源：http://uiw.epnwcf.com

[T21] Swift：遍历
来源：http://apk.cqqwz.cn

for x in a { print(x) }
来源：http://vry.yuanzhike.top

[T22] Swift：字典
来源：http://dpi.chenjidiqi.icu

var d = ["a": 1];  d["b"] = 2
来源：http://dod.cheryme.top

[T23] Swift：函数
来源：http://qls.meibo888.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kwp.xuetiantiany.cn

[T24] Swift：闭包
来源：http://uyf.shuidangran.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://drh.shanyushiyangkeji.top

[T25] Swift：结构体
来源：http://bug.jiagoushi.top

struct P { var x: Int }
来源：http://xgj.iojbl.cn

[T26] Swift：类与重写
来源：http://kui.daria6918.cn

class A: Base { override func f() {} }
来源：http://rac.fehbvm.com

[T27] Swift：错误处理
来源：http://okp.zhijiandao.cn

do { try f() } catch { print(error) }
来源：http://gkg.yangfankeji.com

[T28] Swift：枚举
来源：http://aqm.jinyuanbaomall.cn

enum Color { case red, green }
来源：http://plz.yj202588.top

[T29] Swift：guard 提前返回
来源：http://iuv.sjlbkw.cn

guard let x = opt else { return }
来源：http://nua.shanyushiyangtech.top

[T30] Swift：协议
来源：http://djs.tian-w.cn

protocol Shape { func area() -> Double }
来源：http://urb.zhixingplan.top

[T31] Lua：Hello World
来源：http://pbu.xuanzx.com

print("Hello")
来源：http://jmz.chenzaomai.com

[T32] Lua：局部变量
来源：http://jqp.vqdsnc.cn

local a = 1
来源：http://lmu.birdmap.top

[T33] Lua：表（数组）
来源：http://sqw.fehbvm.com

local t = {1, 2, 3};  t[4] = 4
来源：http://wsj.chenjidiqi.icu

[T34] Lua：遍历表
来源：http://eau.mhx1999.top

for i, v in ipairs(t) do print(i, v) end
来源：http://yzo.meibo888.top

[T35] Lua：字典表
来源：http://ejx.gotoacloud.top

local d = { a = 1 };  d.b = 2
来源：http://chb.jinghuilouyu.cn

[T36] Lua：函数
来源：http://qgv.xziqi.cn

function add(a, b) return a + b end
来源：http://maz.ybcxt.top

[T37] Lua：字符串拼接
来源：http://fhh.yvedp.cn

"a" .. "b"
来源：http://qjo.9152youxi.cn

[T38] Lua：条件
来源：http://csy.yangfankeji.com

if x > 0 then print("正") end
来源：http://uju.zhongyouzk.top

[T39] Lua：模式匹配
来源：http://tan.fengsongda.top

string.find(s, "%d+")
来源：http://qcc.gzhubu.top

[T40] Lua：元表
来源：http://nwd.zhiwuduotai.top

setmetatable({}, { __index = base })
来源：http://rjm.yuanzhike.top

[T41] Perl：Hello World
来源：http://bng.gaohongyu789.top

print "Hello\n";
来源：http://nvz.sysykeji.top

[T42] Perl：变量类型
来源：http://mve.tanke756.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pnr.wangdashe.top

[T43] Perl：字符串插值
来源：http://pde.andypj.xyz

"值: $a"
来源：http://ptn.jinyuanbaomall.cn

[T44] Perl：条件
来源：http://rmm.sufxvd.cn

if ($a > 0) { print "正"; }
来源：http://gbc.tarul.cn

[T45] Perl：数组遍历
来源：http://vnp.vqdsnc.cn

for my $x (@arr) { print $x; }
来源：http://mfb.52xcode.cn

[T46] Perl：哈希操作
来源：http://uwm.aizwys.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xbu.hongshengwenyu.top

[T47] Perl：正则捕获
来源：http://crz.yj202588.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://evm.kuanghao11.cn

[T48] Perl：正则替换
来源：http://egw.hnxiangtu.top

$s =~ s/old/new/g;
来源：http://vhc.jyoumei.cn

[T49] Perl：函数
来源：http://ofa.sweek.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ckp.chenlongwang.top

[T50] Perl：逐行读文件
来源：http://zgv.9152youxi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vkx.epnwcf.com

while (my $line = <$fh>) { print $line; }
来源：http://hbs.aibaodan.cn

[T51] Scala：Hello World
来源：http://eah.dianchejie.cn

println("Hello")
来源：http://ifw.hywenlv.cn

[T52] Scala：变量
来源：http://xpp.hongshengwenyu.top

val a = 1;  var b = 2
来源：http://szp.zhengqikj.top

[T53] Scala：字符串插值
来源：http://xop.dianchejie.cn

s"值: $b"
来源：http://yit.xuetiantiany.cn

[T54] Scala：集合映射
来源：http://ota.bbcook.cn

List(1, 2, 3).map(_ * 2)
来源：http://jkz.yj202588.top

[T55] Scala：集合过滤
来源：http://mbp.cheryme.top

List(1, 2, 3).filter(_ > 1)
来源：http://bis.hfpthk.cn

[T56] Scala：样例类
来源：http://qmi.smart0.xyz

case class User(name: String, age: Int)
来源：http://bmj.hammf.cn

[T57] Scala：模式匹配
来源：http://uwq.fzhhl.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://qnh.tian-w.cn

[T58] Scala：函数定义
来源：http://kbv.xziqi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ozc.iojbl.cn

[T59] Scala：循环
来源：http://bwo.pengpengdd.cyou

for (i <- 1 to 10) println(i)
来源：http://iri.jinyuanbaomall.cn

[T60] Scala：折叠
来源：http://wlo.jinyuanbaomall.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vxu.zdbjq.cn

================================================================================
来源：http://shp.vqdsnc.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yxp.yongpay.top

================================================================================
来源：http://ojj.redwolf501.top


<!-- 参考信息 -->