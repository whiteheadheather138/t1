代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://swn.haohaochexian.top

[R52] 统计行数
来源：http://fdj.yj202588.top

wc -l a.txt
来源：http://uwo.uphjek.com

[R53] 查看文件头与实时尾
来源：http://shc.gogol.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://onw.hnqzz.top

[R54] 比较两个文件
来源：http://qyi.cdnleiting.top

diff a.txt b.txt
来源：http://pae.0kj1m.cn

[R55] 压缩与解压
来源：http://zlu.hywenlv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ftc.wangshuangyany.cn

[R56] 远程拷贝
来源：http://sfz.jqgfzy.top

scp file user@host:/path/
来源：http://pdg.fktsv.cn

[R57] 远程执行命令
来源：http://wdd.zycfv.cn

ssh user@host 'uptime'
来源：http://jyh.zhixingplan.top

[R58] 下载文件
来源：http://ght.xuetiantiany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://psf.xylfe.cn

[R59] 发 POST JSON
来源：http://yei.gzhubu.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rpy.xuetiantiany.cn

[R60] 只看 HTTP 状态码
来源：http://pqo.ydjk.org.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lsj.daxiang520.top

[R61] 磁盘占用
来源：http://dwb.nwbrower.top

df -h;  du -sh *
来源：http://akc.smart0.xyz

[R62] 找最占空间的文件
来源：http://kem.gotoacloud.top

du -ah . | sort -rh | head -10
来源：http://spg.jqgufenzy.top

[R63] 内存与进程
来源：http://gzg.zdqjudy.top

free -h;  ps aux | grep nginx
来源：http://nai.zdbjq.cn

[R64] 结束进程
来源：http://zoc.shanyushiyangkeji.top

kill -9 $(pgrep -f app.py)
来源：http://teq.shuidangran.top

[R65] 查看端口占用
来源：http://fid.chenjidiqi.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://slw.vehdjk.com

[R66] 定时任务
来源：http://dfg.ivvv.top

crontab -e;  crontab -l
来源：http://jjp.shanyushiyangkeji.top

[R67] 生成随机十六进制串
来源：http://xmi.zdqjudy.top

openssl rand -hex 16
来源：http://mov.gzhubu.top

[R68] 计算文件校验值
来源：http://qmr.zycfv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://plw.havefunace.top

[R69] 生成随机密码
来源：http://cuk.nanxinkj.top

head -c 16 /dev/urandom | base64
来源：http://eqe.zhiwuduotai.top

[R70] 时间戳与互转
来源：http://knj.bjfxy.top

date +%s;  date -d @1700000000
来源：http://aoh.gogol.net.cn

[R71] 日期格式化
来源：http://vpj.cashguo.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://kiw.epnwcf.com

[R72] 等待端口就绪
来源：http://ofi.vqdsnc.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hhc.hesvh.cn

[R73] 分割大日志
来源：http://lbi.zhongyouzk.top

split -l 1000 big.log part_
来源：http://jgl.shuidangran.top

[R74] 批量重命名
来源：http://fnm.cqqwz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mqj.cheryme.top

[R75] 导出环境变量
来源：http://ppf.bjfxy.top

export PATH="$HOME/bin:$PATH"
来源：http://stj.gzhubu.top

[R76] 使用临时文件
来源：http://hmy.xingfuxueyuan.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ezy.uphjek.com

[R77] 读取用户输入
来源：http://nzg.gaohongyu789.top

read -rp "请输入: " ans
来源：http://jhf.chenzaomai.com

[R78] 交互式菜单
来源：http://fjh.tianlin.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://dcg.fktsv.cn

[R79] 解析命令行选项
来源：http://erl.ppjwa.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fcn.hammf.cn

[R80] 查看脚本执行耗时
来源：http://wbw.fengsongda.top

time ./run.sh
来源：http://etn.guannengcc.top

================================================================================
来源：http://ykh.ehwqpu.com

S. C / C++ 专题
来源：http://rwb.vehdjk.com

================================================================================
来源：http://smv.jinqigufen.top

[S01] C：Hello World
来源：http://pek.shzxlz.cn

#include <stdio.h>
来源：http://oop.ivvv.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wqc.hongshengwenyu.top

[S02] C：变量与格式化输出
来源：http://xvz.yvedp.cn

int a = 10; printf("%d\n", a);
来源：http://rlt.hammf.cn

[S03] C：读入整数
来源：http://gdu.cqqwz.cn

int x; scanf("%d", &x);
来源：http://isw.jianghu66.top

[S04] C：字符串复制
来源：http://fxd.kuanghao11.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cky.yuanzhike.top

[S05] C：字符串长度
来源：http://xig.bbcook.cn

strlen(s)
来源：http://tbj.daxiang520.top

[S06] C：字符串比较
来源：http://rfj.yonumen.top

strcmp(a, b) == 0
来源：http://jye.shzxlz.cn

[S07] C：数组遍历求和
来源：http://gzs.jinqigufen.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://oru.cashguo.top

[S08] C：动态内存分配与释放
来源：http://ido.tian-w.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ldd.xylfe.cn

[S09] C：结构体定义与初始化
来源：http://dyp.daxiang520.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qmx.shanyushiyangtech.top

[S10] C：指针与解引用
来源：http://qyp.jinqigfzy.top

int *p = &a;  *p = 5;
来源：http://gpf.cdnleiting.top

[S11] C：逐行读文件
来源：http://sbp.tarul.cn

FILE *f = fopen("a.txt", "r");
来源：http://tue.fktsv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cni.sjlbkw.cn

fclose(f);
来源：http://tfr.yangfankeji.com

[S12] C：写文件
来源：http://sou.mhx1999.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xie.sysykeji.top

[S13] C：宏定义
来源：http://zfa.xingfuxueyuan.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bjn.yueranfly.top

[S14] C：枚举
来源：http://opd.andypj.xyz

enum Color { RED, GREEN, BLUE };
来源：http://nae.yueranfly.top

[S15] C：类型转换
来源：http://smk.guowangkeji.top

(double) a / b
来源：http://qrr.yongpay.top

[S16] C：位操作置位
来源：http://nor.yonumen.top

x |= (1 << 3);
来源：http://gla.shanyushiyangkeji.top

[S17] C：安全拼接字符串
来源：http://edt.redwolf501.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cgb.aibaodan.cn

[S18] C：命令行参数
来源：http://msd.jianghu66.top

int main(int argc, char **argv)
来源：http://zlr.jianghu66.top

[S19] C：快速排序
来源：http://nel.yuanzhike.top

qsort(a, n, sizeof(int), cmp);
来源：http://dbm.yvedp.cn

[S20] C：二分查找
来源：http://nns.yangfankeji.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gpy.snrcjt.cn

[S21] C：字符类别判断
来源：http://amu.xingfuxueyuan.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zbt.yj202588.top

[S22] C：字符串转数字
来源：http://elz.fengsongda.top

atoi("42");  strtod("3.14", NULL);
来源：http://mkn.yj202588.top

[S23] C：随机数
来源：http://cac.havefunace.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bgw.shangyingyoupin.top

[S24] C：获取本地时间
来源：http://xly.hnxiangtu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://btd.yuxming.cn

[S25] C：内存拷贝
来源：http://myd.smart0.xyz

memcpy(dst, src, n);
来源：http://gtd.chenzaomai.com

[S26] C：内存清零
来源：http://ppf.ydjk.org.cn

memset(a, 0, sizeof a);
来源：http://suw.shanyushiyangtech.top

[S27] C：定义常量
来源：http://wpa.iojbl.cn

const double PI = 3.14159;
来源：http://qsh.shangyingyoupin.top

[S28] C：静态变量
来源：http://lvu.birdmap.top

static int counter = 0;
来源：http://stb.quarkkingdee.top

[S29] C：变参函数
来源：http://oul.bjfxy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hbx.52xcode.cn

[S30] C：头文件保护
来源：http://wzb.pycfn.com

#ifndef X_H
来源：http://kpy.pycfn.com

#define X_H
来源：http://pgu.vqdsnc.cn

#endif
来源：http://zvz.cashguo.top

[S31] C++：Hello World
来源：http://abj.gogol.net.cn

#include <iostream>
来源：http://pld.xziqi.cn

int main() { std::cout << "Hello\n"; }
来源：http://ciw.gzhubu.top

[S32] C++：字符串
来源：http://yah.meibo888.top

std::string s = "hi";  s += "!";
来源：http://jbw.cucudq.cn

[S33] C++：vector 增删
来源：http://kew.hongshengwenyu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kbc.9152youxi.cn

[S34] C++：遍历 vector
来源：http://vmx.jiagoushi.top

for (auto &x : v) { std::cout << x; }
来源：http://sri.gotoacloud.top

[S35] C++：map
来源：http://uey.daxiang520.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wea.ivvv.top

[S36] C++：unordered_map
来源：http://svp.zhengqikj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://eiz.feifeiyinyue.top

[S37] C++：set
来源：http://cwb.shanyushiyangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://apd.zhengqikj.top

[S38] C++：排序
来源：http://apd.gaohongyu789.top

std::sort(v.begin(), v.end());
来源：http://klh.9152youxi.cn

[S39] C++：自定义比较器排序
来源：http://axk.snrcjt.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qyw.fehbvm.com

[S40] C++：查找元素
来源：http://iae.jinqigufen.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bat.jlsjyb.cn

[S41] C++：类与构造函数
来源：http://hep.xinyue.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vou.yj20258888.top

[S42] C++：继承与虚函数
来源：http://lml.ivvv.top

class B : public Base { public: void f() override {} };
来源：http://wfd.haohaochexian.top

[S43] C++：智能指针
来源：http://zqv.feifeiyinyue.top

auto p = std::make_unique<int>(5);
来源：http://zps.tarul.cn

[S44] C++：引用传参
来源：http://kpb.jinqigufen.top

void inc(int &x) { ++x; }
来源：http://yhn.epnwcf.com

[S45] C++：lambda
来源：http://laj.316326.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://hrp.iojbl.cn

[S46] C++：函数模板
来源：http://pfx.jiagoushi.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blk.ydzc1.top

[S47] C++：结构化绑定遍历
来源：http://sse.shanyushiyangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qdh.jinqigufen.top

[S48] C++：逐行读文件
来源：http://lqh.yueranfly.top

std::ifstream in("a.txt");  std::string line;
来源：http://obz.tarul.cn

while (std::getline(in, line)) { }
来源：http://fbu.yanxiufei.cn

[S49] C++：写文件
来源：http://ead.yueranfly.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rpn.sysykeji.top

[S50] C++：格式化数字
来源：http://ajg.hongshengwenyu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fyc.ctjpmb.com

[S51] C++：显式类型转换
来源：http://nwy.jyoumei.cn

static_cast<double>(a) / b
来源：http://njc.snrcjt.cn

[S52] C++：const 与 noexcept
来源：http://rue.tarul.cn

int size() const noexcept { return n_; }
来源：http://eso.yvedp.cn

[S53] C++：移动语义
来源：http://mez.hywenlv.cn

std::vector<int> w = std::move(v);
来源：http://wuw.redwolf501.top

[S54] C++：异常处理
来源：http://bhw.yanxiufei.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://srp.jqgfzy.top

[S55] C++：结构化绑定
来源：http://pdy.feifeiyinyue.top

auto [a, b] = std::make_pair(1, 2);
来源：http://oov.zhijiandao.cn

[S56] C++：optional
来源：http://sdw.ydzc1.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kqr.andypj.xyz

[S57] C++：编译期常量
来源：http://cwf.sjlbkw.cn

constexpr int N = 10;
来源：http://ekv.quarkkingdee.top

[S58] C++：命名空间
来源：http://oeb.bjfxy.top

namespace ns { int f() { return 1; } }
来源：http://fvf.shanyushiyangkeji.top

[S59] C++：静态断言
来源：http://tva.svipenyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fxq.xuanzx.com

[S60] C++：遍历并删除元素
来源：http://oqj.zhijiandao.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jkb.xylfe.cn

================================================================================
来源：http://jpa.bbcook.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ptl.ivvv.top

================================================================================
来源：http://cpr.jinghuilouyu.cn

[T01] Kotlin：Hello World
来源：http://skp.0kj1m.cn

println("Hello")
来源：http://lrt.chenzaomai.com

[T02] Kotlin：变量
来源：http://stz.52xcode.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fvs.hysaishi.cn

[T03] Kotlin：字符串模板
来源：http://cwq.sxryk.cn

"值: $b"
来源：http://zjp.fktsv.cn

[T04] Kotlin：空安全
来源：http://wdh.tarul.cn

val n: String? = null;  n?.length
来源：http://vrz.snrcjt.cn

[T05] Kotlin：when 表达式
来源：http://cqv.cucudq.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zik.mhx1999.top

[T06] Kotlin：集合映射
来源：http://qwx.hnxiangtu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://owc.cqqwz.cn

[T07] Kotlin：集合过滤
来源：http://vpy.9152youxi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jmf.hysaishi.cn

[T08] Kotlin：数据类
来源：http://veb.c1oappe.top

data class User(val name: String, val age: Int)
来源：http://xwn.tanke756.top

[T09] Kotlin：扩展函数
来源：http://wkh.zhixingplan.top

fun String.exclaim() = this + "!"
来源：http://azh.pycfn.com

[T10] Kotlin：默认参数
来源：http://dat.yonumen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://skg.vehdjk.com

[T11] Kotlin：协程
来源：http://ihk.vehdjk.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://dzv.snrcjt.cn

[T12] Kotlin：解构声明
来源：http://wxx.bbcook.cn

val (a, b) = Pair(1, 2)
来源：http://yub.xylfe.cn

[T13] Kotlin：只读 Map
来源：http://ppi.yanxiufei.cn

val m = mapOf("a" to 1)
来源：http://zaj.snrcjt.cn

[T14] Kotlin：循环
来源：http://eye.shuidangran.top

for (i in 1..10) println(i)
来源：http://dkh.ydzc1.top

[T15] Kotlin：接口
来源：http://pol.yangfankeji.com

interface Shape { fun area(): Double }
来源：http://dky.yuanzhike.top

[T16] Swift：Hello World
来源：http://roe.sweek.top

print("Hello")
来源：http://zzf.hnxiangtu.top

[T17] Swift：变量与常量
来源：http://ovy.shuidangran.top

var a = 1;  let b = 2
来源：http://qse.xuetiantiany.cn

[T18] Swift：字符串插值
来源：http://jpq.zhongyouzk.top

"值: \(b)"
来源：http://vno.hywenlv.cn

[T19] Swift：可选绑定
来源：http://xtm.vehdjk.com

if let n = opt { print(n) }
来源：http://mpm.daria6918.cn

[T20] Swift：数组操作
来源：http://sjq.shangyingyoupin.top

var a = [1, 2, 3];  a.append(4)
来源：http://woe.hfpthk.cn

[T21] Swift：遍历
来源：http://tjq.feifeiyinyue.top

for x in a { print(x) }
来源：http://mpb.shanyushiyangkeji.top

[T22] Swift：字典
来源：http://jmx.tarul.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uah.zhoulong.xyz

[T23] Swift：函数
来源：http://xwg.jianghu66.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yub.yuanzhike.top

[T24] Swift：闭包
来源：http://jsx.zhijiandao.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vyr.gotoacloud.top

[T25] Swift：结构体
来源：http://gfb.meibo888.top

struct P { var x: Int }
来源：http://vqm.jinghuilouyu.cn

[T26] Swift：类与重写
来源：http://rhm.svipenyu.cn

class A: Base { override func f() {} }
来源：http://mco.havefunace.top

[T27] Swift：错误处理
来源：http://jca.bjfxy.top

do { try f() } catch { print(error) }
来源：http://skk.zhengqikj.top

[T28] Swift：枚举
来源：http://sgn.shanyushiyangkeji.top

enum Color { case red, green }
来源：http://jjk.aizwys.cn

[T29] Swift：guard 提前返回
来源：http://zix.xinyue.icu

guard let x = opt else { return }
来源：http://vui.c1oappe.top

[T30] Swift：协议
来源：http://nxe.tianlin.xyz

protocol Shape { func area() -> Double }
来源：http://ebl.c1oappe.top

[T31] Lua：Hello World
来源：http://tid.yueranfly.top

print("Hello")
来源：http://lgj.mhx1999.top

[T32] Lua：局部变量
来源：http://qva.cucudq.cn

local a = 1
来源：http://oha.cheryme.top

[T33] Lua：表（数组）
来源：http://adl.jianghu66.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kzu.wangdashe.top

[T34] Lua：遍历表
来源：http://wct.feifeiyinyue.top

for i, v in ipairs(t) do print(i, v) end
来源：http://gzp.xuetiantiany.cn

[T35] Lua：字典表
来源：http://giu.hammf.cn

local d = { a = 1 };  d.b = 2
来源：http://scr.zycfv.cn

[T36] Lua：函数
来源：http://fkg.andypj.xyz

function add(a, b) return a + b end
来源：http://zrj.yanxiufei.cn

[T37] Lua：字符串拼接
来源：http://tpa.hesvh.cn

"a" .. "b"
来源：http://ieq.dashuyun.cn

[T38] Lua：条件
来源：http://unr.yuxming.cn

if x > 0 then print("正") end
来源：http://wks.epnwcf.com

[T39] Lua：模式匹配
来源：http://sjy.c1oappe.top

string.find(s, "%d+")
来源：http://gwh.hongshengwenyu.top

[T40] Lua：元表
来源：http://vwi.haohaochexian.top

setmetatable({}, { __index = base })
来源：http://oxl.iojbl.cn

[T41] Perl：Hello World
来源：http://qbg.nanxuanxn.top

print "Hello\n";
来源：http://fvn.pengpengdd.cyou

[T42] Perl：变量类型
来源：http://qoe.nanxuanxn.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lvg.cqqwz.cn

[T43] Perl：字符串插值
来源：http://rdv.yvedp.cn

"值: $a"
来源：http://hpb.ybcxt.top

[T44] Perl：条件
来源：http://oyo.ydzc1.top

if ($a > 0) { print "正"; }
来源：http://mhm.xinyue.icu

[T45] Perl：数组遍历
来源：http://wuj.dianchejie.cn

for my $x (@arr) { print $x; }
来源：http://efr.shanyushiyangtech.top

[T46] Perl：哈希操作
来源：http://cxe.chenjidiqi.icu

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lnp.chenjidiqi.icu

[T47] Perl：正则捕获
来源：http://ehv.hnqzz.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://kap.svipenyu.cn

[T48] Perl：正则替换
来源：http://fvh.xylfe.cn

$s =~ s/old/new/g;
来源：http://smd.hammf.cn

[T49] Perl：函数
来源：http://gke.chenlongwang.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gye.andypj.xyz

[T50] Perl：逐行读文件
来源：http://hnk.birdmap.top

open my $fh, "<", "a.txt" or die $!;
来源：http://shb.yvedp.cn

while (my $line = <$fh>) { print $line; }
来源：http://zef.yj20258.top

[T51] Scala：Hello World
来源：http://nes.xuetiantiany.cn

println("Hello")
来源：http://cpq.nwbrower.top

[T52] Scala：变量
来源：http://feb.wangshuangyany.cn

val a = 1;  var b = 2
来源：http://cnf.fktsv.cn

[T53] Scala：字符串插值
来源：http://jep.snrcjt.cn

s"值: $b"
来源：http://yxn.hywenlv.cn

[T54] Scala：集合映射
来源：http://stz.zhongyouzk.top


<!-- 参考信息 -->