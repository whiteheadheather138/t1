代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://hqh.shangyingyoupin.top

[R52] 统计行数
来源：http://gzu.fzhhl.top

wc -l a.txt
来源：http://bud.fktsv.cn

[R53] 查看文件头与实时尾
来源：http://ned.jqgufenzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cvw.sjlbkw.cn

[R54] 比较两个文件
来源：http://tzq.yj20258888.top

diff a.txt b.txt
来源：http://iie.yvedp.cn

[R55] 压缩与解压
来源：http://rgk.jyoumei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://umw.yj202588.top

[R56] 远程拷贝
来源：http://krt.snrcjt.cn

scp file user@host:/path/
来源：http://ftq.nwbrower.top

[R57] 远程执行命令
来源：http://hul.dianchejie.cn

ssh user@host 'uptime'
来源：http://uhh.chenzaomai.com

[R58] 下载文件
来源：http://iqx.guannengcc.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lsh.havefunace.top

[R59] 发 POST JSON
来源：http://fkw.havefunace.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vjr.hammf.cn

[R60] 只看 HTTP 状态码
来源：http://jjy.meibo888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zqx.chenjidiqi.icu

[R61] 磁盘占用
来源：http://tus.yueranfly.top

df -h;  du -sh *
来源：http://vrp.sjlbkw.cn

[R62] 找最占空间的文件
来源：http://kay.shanyushiyangtech.top

du -ah . | sort -rh | head -10
来源：http://tif.tian-w.cn

[R63] 内存与进程
来源：http://clq.sxryk.cn

free -h;  ps aux | grep nginx
来源：http://oxq.havefunace.top

[R64] 结束进程
来源：http://mmo.hysaishi.cn

kill -9 $(pgrep -f app.py)
来源：http://ocg.zycfv.cn

[R65] 查看端口占用
来源：http://ndh.jinghuilouyu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://eoj.aibaodan.cn

[R66] 定时任务
来源：http://lno.haohaochexian.top

crontab -e;  crontab -l
来源：http://dib.hfpthk.cn

[R67] 生成随机十六进制串
来源：http://bvj.zdqjudy.top

openssl rand -hex 16
来源：http://oma.cdnleiting.top

[R68] 计算文件校验值
来源：http://kpp.pengpengdd.cyou

sha256sum a.txt;  md5sum a.txt
来源：http://sng.xuetiantiany.cn

[R69] 生成随机密码
来源：http://ssh.nanxuanxn.top

head -c 16 /dev/urandom | base64
来源：http://jod.ctjpmb.com

[R70] 时间戳与互转
来源：http://qse.sufxvd.cn

date +%s;  date -d @1700000000
来源：http://nmk.jianghu66.top

[R71] 日期格式化
来源：http://gti.shuidangran.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jvo.zhixingplan.top

[R72] 等待端口就绪
来源：http://uco.yongpay.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ciy.zhixingplan.top

[R73] 分割大日志
来源：http://cfw.cdnleiting.top

split -l 1000 big.log part_
来源：http://foj.hammf.cn

[R74] 批量重命名
来源：http://cve.gotoacloud.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fqh.hywenlv.cn

[R75] 导出环境变量
来源：http://rna.haohaochexian.top

export PATH="$HOME/bin:$PATH"
来源：http://ksa.tian-w.cn

[R76] 使用临时文件
来源：http://xph.epnwcf.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wtt.yvedp.cn

[R77] 读取用户输入
来源：http://fnl.jiagoushi.top

read -rp "请输入: " ans
来源：http://mjy.fktsv.cn

[R78] 交互式菜单
来源：http://frt.jinghuilouyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://czm.sysykeji.top

[R79] 解析命令行选项
来源：http://hes.chenzaomai.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yih.bbcook.cn

[R80] 查看脚本执行耗时
来源：http://xlj.snrcjt.cn

time ./run.sh
来源：http://okj.andypj.xyz

================================================================================
来源：http://cnf.jianghu66.top

S. C / C++ 专题
来源：http://xrm.fehbvm.com

================================================================================
来源：http://rcn.ppjwa.cn

[S01] C：Hello World
来源：http://rvj.haohaochexian.top

#include <stdio.h>
来源：http://ssc.tarul.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qxl.52xcode.cn

[S02] C：变量与格式化输出
来源：http://jba.dianchejie.cn

int a = 10; printf("%d\n", a);
来源：http://chk.shanyushiyangkeji.top

[S03] C：读入整数
来源：http://twi.smart0.xyz

int x; scanf("%d", &x);
来源：http://nrx.sufxvd.cn

[S04] C：字符串复制
来源：http://rwk.uphjek.com

char dst[32]; strcpy(dst, "hi");
来源：http://teo.zhixingplan.top

[S05] C：字符串长度
来源：http://ozg.havefunace.top

strlen(s)
来源：http://lpe.zhongyouzk.top

[S06] C：字符串比较
来源：http://lmh.zhixingplan.top

strcmp(a, b) == 0
来源：http://rvw.snrcjt.cn

[S07] C：数组遍历求和
来源：http://iqu.bbcook.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xiq.yanxiufei.cn

[S08] C：动态内存分配与释放
来源：http://qww.hcnkem.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uzu.jinghuilouyu.cn

[S09] C：结构体定义与初始化
来源：http://zyi.fktsv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pay.aizwys.cn

[S10] C：指针与解引用
来源：http://evn.c1oappe.top

int *p = &a;  *p = 5;
来源：http://hfh.c1oappe.top

[S11] C：逐行读文件
来源：http://cax.yvedp.cn

FILE *f = fopen("a.txt", "r");
来源：http://bme.zdbjq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vyk.ppjwa.cn

fclose(f);
来源：http://gmh.hcnkem.com

[S12] C：写文件
来源：http://hhj.sjlbkw.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mpu.zhoulong.xyz

[S13] C：宏定义
来源：http://sfz.shangyingyoupin.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yzk.52xcode.cn

[S14] C：枚举
来源：http://udw.hcnkem.com

enum Color { RED, GREEN, BLUE };
来源：http://fzx.svipenyu.cn

[S15] C：类型转换
来源：http://zhr.cdnleiting.top

(double) a / b
来源：http://cvs.gzhubu.top

[S16] C：位操作置位
来源：http://qoh.mhx1999.top

x |= (1 << 3);
来源：http://fiy.yuanzhike.top

[S17] C：安全拼接字符串
来源：http://gci.yongpay.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wtw.chenjidiqi.icu

[S18] C：命令行参数
来源：http://oem.daria6918.cn

int main(int argc, char **argv)
来源：http://otl.hcnkem.com

[S19] C：快速排序
来源：http://nnj.havefunace.top

qsort(a, n, sizeof(int), cmp);
来源：http://wgp.zhixingplan.top

[S20] C：二分查找
来源：http://bqf.ehwqpu.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mkm.jiagoushi.top

[S21] C：字符类别判断
来源：http://cls.zdbjq.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://okn.chenzaomai.com

[S22] C：字符串转数字
来源：http://vdb.yueranfly.top

atoi("42");  strtod("3.14", NULL);
来源：http://vil.kuanghao11.cn

[S23] C：随机数
来源：http://zjg.ppjwa.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hlp.aizwys.cn

[S24] C：获取本地时间
来源：http://vsz.jinqigufen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cfu.cdnleiting.top

[S25] C：内存拷贝
来源：http://mhz.daria6918.cn

memcpy(dst, src, n);
来源：http://pjp.ppjwa.cn

[S26] C：内存清零
来源：http://akp.fktsv.cn

memset(a, 0, sizeof a);
来源：http://uhh.cashguo.top

[S27] C：定义常量
来源：http://rjt.bbcook.cn

const double PI = 3.14159;
来源：http://dtl.yueranfly.top

[S28] C：静态变量
来源：http://wmq.zycfv.cn

static int counter = 0;
来源：http://vyw.jlsjyb.cn

[S29] C：变参函数
来源：http://mlf.jinyuanbaomall.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://syh.daria6918.cn

[S30] C：头文件保护
来源：http://pvs.sweek.top

#ifndef X_H
来源：http://fhb.chenlongwang.top

#define X_H
来源：http://trj.bjfxy.top

#endif
来源：http://ecj.hysaishi.cn

[S31] C++：Hello World
来源：http://eyx.yangfankeji.com

#include <iostream>
来源：http://fri.shangyingyoupin.top

int main() { std::cout << "Hello\n"; }
来源：http://caw.epnwcf.com

[S32] C++：字符串
来源：http://vxi.daxiang520.top

std::string s = "hi";  s += "!";
来源：http://ikn.fengsongda.top

[S33] C++：vector 增删
来源：http://env.shzxlz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://onm.zhaomingkeji.xyz

[S34] C++：遍历 vector
来源：http://fqf.birdmap.top

for (auto &x : v) { std::cout << x; }
来源：http://wmi.snrcjt.cn

[S35] C++：map
来源：http://ity.xuetiantiany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mgi.fengsongda.top

[S36] C++：unordered_map
来源：http://zkq.hnqzz.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ixa.xylfe.cn

[S37] C++：set
来源：http://zje.shzxlz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ywj.pengpengdd.cyou

[S38] C++：排序
来源：http://ntb.nanxinkj.top

std::sort(v.begin(), v.end());
来源：http://tmw.xingfuxueyuan.xyz

[S39] C++：自定义比较器排序
来源：http://kno.yj202588.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nkq.zhixingplan.top

[S40] C++：查找元素
来源：http://lco.9152youxi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fjq.nanxuanxn.top

[S41] C++：类与构造函数
来源：http://trw.jinqigufen.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dsa.jinqigufen.top

[S42] C++：继承与虚函数
来源：http://gul.sysykeji.top

class B : public Base { public: void f() override {} };
来源：http://rfe.redwolf501.top

[S43] C++：智能指针
来源：http://flt.sjlbkw.cn

auto p = std::make_unique<int>(5);
来源：http://tie.jqgufenzy.top

[S44] C++：引用传参
来源：http://vxv.wangdashe.top

void inc(int &x) { ++x; }
来源：http://bws.xuetiantiany.cn

[S45] C++：lambda
来源：http://inr.birdmap.top

auto add = [](int a, int b) { return a + b; };
来源：http://lse.quarkkingdee.top

[S46] C++：函数模板
来源：http://ixn.hysaishi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rnf.gzhubu.top

[S47] C++：结构化绑定遍历
来源：http://qqb.daria6918.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wne.xylfe.cn

[S48] C++：逐行读文件
来源：http://hld.ivvv.top

std::ifstream in("a.txt");  std::string line;
来源：http://wgc.9152youxi.cn

while (std::getline(in, line)) { }
来源：http://omi.yvedp.cn

[S49] C++：写文件
来源：http://elg.yvedp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iep.tarul.cn

[S50] C++：格式化数字
来源：http://ejr.gogol.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xbv.chenzaomai.com

[S51] C++：显式类型转换
来源：http://lux.tianlin.xyz

static_cast<double>(a) / b
来源：http://zcg.jlsjyb.cn

[S52] C++：const 与 noexcept
来源：http://igm.yanxiufei.cn

int size() const noexcept { return n_; }
来源：http://ash.nanxinkj.top

[S53] C++：移动语义
来源：http://dar.yuxming.cn

std::vector<int> w = std::move(v);
来源：http://qzd.hcnkem.com

[S54] C++：异常处理
来源：http://qmp.hammf.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cze.yj20258.top

[S55] C++：结构化绑定
来源：http://tlz.pycfn.com

auto [a, b] = std::make_pair(1, 2);
来源：http://hap.daxiang520.top

[S56] C++：optional
来源：http://xpa.gzhubu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://scx.c1oappe.top

[S57] C++：编译期常量
来源：http://hyi.yangfankeji.com

constexpr int N = 10;
来源：http://ret.zhaomingkeji.xyz

[S58] C++：命名空间
来源：http://jap.zhaomingkeji.xyz

namespace ns { int f() { return 1; } }
来源：http://yto.gzhubu.top

[S59] C++：静态断言
来源：http://rdz.guowangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qrq.zdqjudy.top

[S60] C++：遍历并删除元素
来源：http://dvz.bjfxy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ccq.zhixingplan.top

================================================================================
来源：http://xeu.redwolf501.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://muj.nwbrower.top

================================================================================
来源：http://dlv.uphjek.com

[T01] Kotlin：Hello World
来源：http://kop.fehbvm.com

println("Hello")
来源：http://ajo.gotoacloud.top

[T02] Kotlin：变量
来源：http://jnr.ppjwa.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ygf.0kj1m.cn

[T03] Kotlin：字符串模板
来源：http://cru.fanxiaobao.xyz

"值: $b"
来源：http://htt.ivvv.top

[T04] Kotlin：空安全
来源：http://efz.nanxinkj.top

val n: String? = null;  n?.length
来源：http://pzf.zdqjudy.top

[T05] Kotlin：when 表达式
来源：http://jep.hnqzz.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://chk.daria6918.cn

[T06] Kotlin：集合映射
来源：http://qwi.xuetiantiany.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gqv.jiagoushi.top

[T07] Kotlin：集合过滤
来源：http://xcd.kuanghao11.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gfa.yvedp.cn

[T08] Kotlin：数据类
来源：http://fuy.nwbrower.top

data class User(val name: String, val age: Int)
来源：http://tht.dianchejie.cn

[T09] Kotlin：扩展函数
来源：http://atq.chenlongwang.top

fun String.exclaim() = this + "!"
来源：http://gsx.smart0.xyz

[T10] Kotlin：默认参数
来源：http://dht.hcnkem.com

fun greet(name: String = "World") = "Hi $name"
来源：http://ttx.ctjpmb.com

[T11] Kotlin：协程
来源：http://xrd.chenzaomai.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://tgs.ehwqpu.com

[T12] Kotlin：解构声明
来源：http://ddo.sxryk.cn

val (a, b) = Pair(1, 2)
来源：http://fiu.9152youxi.cn

[T13] Kotlin：只读 Map
来源：http://xja.hesvh.cn

val m = mapOf("a" to 1)
来源：http://wbe.epnwcf.com

[T14] Kotlin：循环
来源：http://yjo.cdnleiting.top

for (i in 1..10) println(i)
来源：http://mvb.zhaomingkeji.xyz

[T15] Kotlin：接口
来源：http://gof.snrcjt.cn

interface Shape { fun area(): Double }
来源：http://idi.sysykeji.top

[T16] Swift：Hello World
来源：http://nao.jiagoushi.top

print("Hello")
来源：http://ywl.cashguo.top

[T17] Swift：变量与常量
来源：http://acb.cucudq.cn

var a = 1;  let b = 2
来源：http://kji.tanke756.top

[T18] Swift：字符串插值
来源：http://gqa.yueranfly.top

"值: \(b)"
来源：http://nlp.pycfn.com

[T19] Swift：可选绑定
来源：http://plv.xuetiantiany.cn

if let n = opt { print(n) }
来源：http://qqy.yueranfly.top

[T20] Swift：数组操作
来源：http://ddk.ydzc1.top

var a = [1, 2, 3];  a.append(4)
来源：http://gqn.xylfe.cn

[T21] Swift：遍历
来源：http://eyt.52xcode.cn

for x in a { print(x) }
来源：http://gwu.xuetiantiany.cn

[T22] Swift：字典
来源：http://abl.shangyingyoupin.top

var d = ["a": 1];  d["b"] = 2
来源：http://ogm.zhiwuduotai.top

[T23] Swift：函数
来源：http://ync.jqgfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jpm.epnwcf.com

[T24] Swift：闭包
来源：http://cfd.ivvv.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://gye.ivvv.top

[T25] Swift：结构体
来源：http://xnq.fengsongda.top

struct P { var x: Int }
来源：http://eiu.guowangkeji.top

[T26] Swift：类与重写
来源：http://crr.vqdsnc.cn

class A: Base { override func f() {} }
来源：http://jht.yj202588.top

[T27] Swift：错误处理
来源：http://yfw.quarkkingdee.top

do { try f() } catch { print(error) }
来源：http://fhl.hfpthk.cn

[T28] Swift：枚举
来源：http://pfw.hammf.cn

enum Color { case red, green }
来源：http://hxr.havefunace.top

[T29] Swift：guard 提前返回
来源：http://gtb.tian-w.cn

guard let x = opt else { return }
来源：http://pwi.shangyingyoupin.top

[T30] Swift：协议
来源：http://xme.fehbvm.com

protocol Shape { func area() -> Double }
来源：http://lio.iojbl.cn

[T31] Lua：Hello World
来源：http://tsj.chenjidiqi.icu

print("Hello")
来源：http://aqz.yj20258.top

[T32] Lua：局部变量
来源：http://zgv.pengpengdd.cyou

local a = 1
来源：http://xmb.ppjwa.cn

[T33] Lua：表（数组）
来源：http://iwq.jinyuanbaomall.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wfe.cashguo.top

[T34] Lua：遍历表
来源：http://pgx.jinyuanbaomall.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ibw.gotoacloud.top

[T35] Lua：字典表
来源：http://moc.xziqi.cn

local d = { a = 1 };  d.b = 2
来源：http://bei.fzhhl.top

[T36] Lua：函数
来源：http://msu.yongpay.top

function add(a, b) return a + b end
来源：http://nue.tianlin.xyz

[T37] Lua：字符串拼接
来源：http://utx.shanyushiyangtech.top

"a" .. "b"
来源：http://rxi.svipenyu.cn

[T38] Lua：条件
来源：http://lcw.birdmap.top

if x > 0 then print("正") end
来源：http://wmt.yj20258.top

[T39] Lua：模式匹配
来源：http://off.gzhubu.top

string.find(s, "%d+")
来源：http://yqs.yvedp.cn

[T40] Lua：元表
来源：http://ybw.havefunace.top

setmetatable({}, { __index = base })
来源：http://ccv.chenlongwang.top

[T41] Perl：Hello World
来源：http://ico.jqgufenzy.top

print "Hello\n";
来源：http://exg.birdmap.top

[T42] Perl：变量类型
来源：http://ptu.fktsv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ska.316326.xyz

[T43] Perl：字符串插值
来源：http://cyl.xuetiantiany.cn

"值: $a"
来源：http://ojf.wangdashe.top

[T44] Perl：条件
来源：http://whv.fzhhl.top

if ($a > 0) { print "正"; }
来源：http://une.mhx1999.top

[T45] Perl：数组遍历
来源：http://tyv.andypj.xyz

for my $x (@arr) { print $x; }
来源：http://sei.zhoulong.xyz

[T46] Perl：哈希操作
来源：http://oqe.xingfuxueyuan.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xcg.andypj.xyz

[T47] Perl：正则捕获
来源：http://vrm.yuxming.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://src.52xcode.cn

[T48] Perl：正则替换
来源：http://cqj.chenjidiqi.icu

$s =~ s/old/new/g;
来源：http://wod.feifeiyinyue.top

[T49] Perl：函数
来源：http://veo.jinqigufen.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sdh.zhaomingkeji.xyz

[T50] Perl：逐行读文件
来源：http://soi.ybcxt.top

open my $fh, "<", "a.txt" or die $!;
来源：http://trq.yuanzhike.top

while (my $line = <$fh>) { print $line; }
来源：http://qfu.yongpay.top

[T51] Scala：Hello World
来源：http://tew.hcnkem.com

println("Hello")
来源：http://sbh.redwolf501.top

[T52] Scala：变量
来源：http://rcd.hesvh.cn

val a = 1;  var b = 2
来源：http://axq.ydzc1.top

[T53] Scala：字符串插值
来源：http://jcr.svipenyu.cn

s"值: $b"
来源：http://jyn.c1oappe.top

[T54] Scala：集合映射
来源：http://tdj.zhijiandao.cn


<!-- 参考信息 -->