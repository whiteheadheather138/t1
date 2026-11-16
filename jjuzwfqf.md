代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://qsn.xinyue.icu

[R52] 统计行数
来源：http://itq.sufxvd.cn

wc -l a.txt
来源：http://nbs.dashuyun.cn

[R53] 查看文件头与实时尾
来源：http://zog.gogol.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uuh.yj20258.top

[R54] 比较两个文件
来源：http://jac.zdqjudy.top

diff a.txt b.txt
来源：http://iev.zdbjq.cn

[R55] 压缩与解压
来源：http://zdz.nanxuanxn.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://okb.daria6918.cn

[R56] 远程拷贝
来源：http://imp.yueranfly.top

scp file user@host:/path/
来源：http://xmh.316326.xyz

[R57] 远程执行命令
来源：http://pdg.fehbvm.com

ssh user@host 'uptime'
来源：http://fpc.cashguo.top

[R58] 下载文件
来源：http://dbs.c1oappe.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fyo.yonumen.top

[R59] 发 POST JSON
来源：http://rgj.hnqzz.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://flp.svipenyu.cn

[R60] 只看 HTTP 状态码
来源：http://ccl.xuanzx.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://abv.hcnkem.com

[R61] 磁盘占用
来源：http://ikn.cheryme.top

df -h;  du -sh *
来源：http://kqv.sysykeji.top

[R62] 找最占空间的文件
来源：http://gjr.cheryme.top

du -ah . | sort -rh | head -10
来源：http://zyq.ywan-chungtsiang.top

[R63] 内存与进程
来源：http://mib.vehdjk.com

free -h;  ps aux | grep nginx
来源：http://erc.chenjidiqi.icu

[R64] 结束进程
来源：http://iom.yonumen.top

kill -9 $(pgrep -f app.py)
来源：http://zah.ehwqpu.com

[R65] 查看端口占用
来源：http://bcv.nwbrower.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rbg.xingfuxueyuan.xyz

[R66] 定时任务
来源：http://bby.jyoumei.cn

crontab -e;  crontab -l
来源：http://chx.yonumen.top

[R67] 生成随机十六进制串
来源：http://ewy.zhengqikj.top

openssl rand -hex 16
来源：http://jmg.shzxlz.cn

[R68] 计算文件校验值
来源：http://uma.kuanghao11.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dbu.52xcode.cn

[R69] 生成随机密码
来源：http://zul.jinyuanbaomall.cn

head -c 16 /dev/urandom | base64
来源：http://rxp.hysaishi.cn

[R70] 时间戳与互转
来源：http://bll.daxiang520.top

date +%s;  date -d @1700000000
来源：http://izh.sweek.top

[R71] 日期格式化
来源：http://uxv.jlsjyb.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wox.shzxlz.cn

[R72] 等待端口就绪
来源：http://uef.cheryme.top

until nc -z localhost 3306; do sleep 1; done
来源：http://kfv.xziqi.cn

[R73] 分割大日志
来源：http://wsh.fanxiaobao.xyz

split -l 1000 big.log part_
来源：http://xbk.cqqwz.cn

[R74] 批量重命名
来源：http://oqq.jiagoushi.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hat.xinyue.icu

[R75] 导出环境变量
来源：http://lva.guowangkeji.top

export PATH="$HOME/bin:$PATH"
来源：http://rtn.xylfe.cn

[R76] 使用临时文件
来源：http://cbj.shanyushiyangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ixy.smart0.xyz

[R77] 读取用户输入
来源：http://etx.chenjidiqi.icu

read -rp "请输入: " ans
来源：http://mst.xziqi.cn

[R78] 交互式菜单
来源：http://wzp.jqgfzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://zhq.hcnkem.com

[R79] 解析命令行选项
来源：http://xji.gogol.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://voi.andypj.xyz

[R80] 查看脚本执行耗时
来源：http://cte.ctjpmb.com

time ./run.sh
来源：http://lzu.zhixingplan.top

================================================================================
来源：http://jvv.jqgufenzy.top

S. C / C++ 专题
来源：http://egf.meibo888.top

================================================================================
来源：http://xql.zhijiandao.cn

[S01] C：Hello World
来源：http://yhv.fanxiaobao.xyz

#include <stdio.h>
来源：http://ong.tianlin.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://mxt.jiagoushi.top

[S02] C：变量与格式化输出
来源：http://njw.ehwqpu.com

int a = 10; printf("%d\n", a);
来源：http://fzd.pycfn.com

[S03] C：读入整数
来源：http://wui.dashuyun.cn

int x; scanf("%d", &x);
来源：http://toi.cqqwz.cn

[S04] C：字符串复制
来源：http://qgt.sxryk.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xvd.hesvh.cn

[S05] C：字符串长度
来源：http://tkv.ydjk.org.cn

strlen(s)
来源：http://fuz.zdqjudy.top

[S06] C：字符串比较
来源：http://bus.xinyue.icu

strcmp(a, b) == 0
来源：http://hdq.yvedp.cn

[S07] C：数组遍历求和
来源：http://nya.fzhhl.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ffg.sufxvd.cn

[S08] C：动态内存分配与释放
来源：http://fxu.zhaomingkeji.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yqb.sysykeji.top

[S09] C：结构体定义与初始化
来源：http://kcj.vqdsnc.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ora.cdnleiting.top

[S10] C：指针与解引用
来源：http://ckd.nanxuanxn.top

int *p = &a;  *p = 5;
来源：http://shx.ywan-chungtsiang.top

[S11] C：逐行读文件
来源：http://epi.tianlin.xyz

FILE *f = fopen("a.txt", "r");
来源：http://oqm.guannengcc.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://xsd.uphjek.com

fclose(f);
来源：http://ngb.jinghuilouyu.cn

[S12] C：写文件
来源：http://iqq.ywan-chungtsiang.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://faj.sjlbkw.cn

[S13] C：宏定义
来源：http://jkc.ydzc1.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://piv.yj20258888.top

[S14] C：枚举
来源：http://zzy.ydjk.org.cn

enum Color { RED, GREEN, BLUE };
来源：http://oxu.haohaochexian.top

[S15] C：类型转换
来源：http://hkv.yangfankeji.com

(double) a / b
来源：http://yyc.jinqigfzy.top

[S16] C：位操作置位
来源：http://hux.nwbrower.top

x |= (1 << 3);
来源：http://nyv.nwbrower.top

[S17] C：安全拼接字符串
来源：http://lht.sysykeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jpw.ctjpmb.com

[S18] C：命令行参数
来源：http://itt.havefunace.top

int main(int argc, char **argv)
来源：http://frq.iojbl.cn

[S19] C：快速排序
来源：http://lgm.quarkkingdee.top

qsort(a, n, sizeof(int), cmp);
来源：http://una.ctjpmb.com

[S20] C：二分查找
来源：http://wco.jqgufenzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lym.zhoulong.xyz

[S21] C：字符类别判断
来源：http://duq.cdnleiting.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kxu.guowangkeji.top

[S22] C：字符串转数字
来源：http://qjm.hongshengwenyu.top

atoi("42");  strtod("3.14", NULL);
来源：http://kql.jianghu66.top

[S23] C：随机数
来源：http://wvm.sjlbkw.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kqc.fengsongda.top

[S24] C：获取本地时间
来源：http://qkg.jqgfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bez.yangfankeji.com

[S25] C：内存拷贝
来源：http://ufg.uphjek.com

memcpy(dst, src, n);
来源：http://kbe.cashguo.top

[S26] C：内存清零
来源：http://tfr.haohaochexian.top

memset(a, 0, sizeof a);
来源：http://ogq.kuanghao11.cn

[S27] C：定义常量
来源：http://vfa.vqdsnc.cn

const double PI = 3.14159;
来源：http://xzu.hnqzz.top

[S28] C：静态变量
来源：http://kol.jqgufenzy.top

static int counter = 0;
来源：http://hpc.havefunace.top

[S29] C：变参函数
来源：http://djo.ywan-chungtsiang.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rfs.shanyushiyangtech.top

[S30] C：头文件保护
来源：http://umv.hcnkem.com

#ifndef X_H
来源：http://zhu.hysaishi.cn

#define X_H
来源：http://sff.0kj1m.cn

#endif
来源：http://vre.hfpthk.cn

[S31] C++：Hello World
来源：http://ymc.yuxming.cn

#include <iostream>
来源：http://ntc.tian-w.cn

int main() { std::cout << "Hello\n"; }
来源：http://qog.hcnkem.com

[S32] C++：字符串
来源：http://dul.hysaishi.cn

std::string s = "hi";  s += "!";
来源：http://zhq.meibo888.top

[S33] C++：vector 增删
来源：http://nfa.epnwcf.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://saz.hywenlv.cn

[S34] C++：遍历 vector
来源：http://gqc.ctjpmb.com

for (auto &x : v) { std::cout << x; }
来源：http://ime.quarkkingdee.top

[S35] C++：map
来源：http://cfp.chenjidiqi.icu

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kdo.yuanzhike.top

[S36] C++：unordered_map
来源：http://hhp.fktsv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://otp.ydzc1.top

[S37] C++：set
来源：http://zvf.guowangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kan.dashuyun.cn

[S38] C++：排序
来源：http://xsn.hesvh.cn

std::sort(v.begin(), v.end());
来源：http://hix.xziqi.cn

[S39] C++：自定义比较器排序
来源：http://wrj.hammf.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xzb.hesvh.cn

[S40] C++：查找元素
来源：http://hed.smart0.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hah.jinqigufen.top

[S41] C++：类与构造函数
来源：http://zrd.fzhhl.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bdp.jinqigufen.top

[S42] C++：继承与虚函数
来源：http://gec.birdmap.top

class B : public Base { public: void f() override {} };
来源：http://zwj.fktsv.cn

[S43] C++：智能指针
来源：http://puq.hongshengwenyu.top

auto p = std::make_unique<int>(5);
来源：http://rxi.redwolf501.top

[S44] C++：引用传参
来源：http://wpo.ywan-chungtsiang.top

void inc(int &x) { ++x; }
来源：http://tcp.zycfv.cn

[S45] C++：lambda
来源：http://tih.sweek.top

auto add = [](int a, int b) { return a + b; };
来源：http://rej.jlsjyb.cn

[S46] C++：函数模板
来源：http://cfm.aizwys.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kvt.tian-w.cn

[S47] C++：结构化绑定遍历
来源：http://tpp.0kj1m.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://noy.hcnkem.com

[S48] C++：逐行读文件
来源：http://zlo.bbcook.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qor.hysaishi.cn

while (std::getline(in, line)) { }
来源：http://thb.tarul.cn

[S49] C++：写文件
来源：http://mia.gogol.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ren.tarul.cn

[S50] C++：格式化数字
来源：http://ypr.zhongyouzk.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tsq.zhixingplan.top

[S51] C++：显式类型转换
来源：http://iol.chenlongwang.top

static_cast<double>(a) / b
来源：http://phj.fanxiaobao.xyz

[S52] C++：const 与 noexcept
来源：http://lhy.zhongyouzk.top

int size() const noexcept { return n_; }
来源：http://nfl.jinghuilouyu.cn

[S53] C++：移动语义
来源：http://twj.fanxiaobao.xyz

std::vector<int> w = std::move(v);
来源：http://hme.xuetiantiany.cn

[S54] C++：异常处理
来源：http://ruf.yongpay.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uxj.gotoacloud.top

[S55] C++：结构化绑定
来源：http://mas.hammf.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mfg.chenzaomai.com

[S56] C++：optional
来源：http://jwd.vehdjk.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fgu.jiagoushi.top

[S57] C++：编译期常量
来源：http://uev.hywenlv.cn

constexpr int N = 10;
来源：http://abk.jyoumei.cn

[S58] C++：命名空间
来源：http://fzv.epnwcf.com

namespace ns { int f() { return 1; } }
来源：http://hpl.ehwqpu.com

[S59] C++：静态断言
来源：http://tre.jiagoushi.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kaw.aizwys.cn

[S60] C++：遍历并删除元素
来源：http://ncr.ivvv.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nqa.snrcjt.cn

================================================================================
来源：http://aqs.uphjek.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uwj.iojbl.cn

================================================================================
来源：http://udk.yueranfly.top

[T01] Kotlin：Hello World
来源：http://ecv.meibo888.top

println("Hello")
来源：http://oil.kuanghao11.cn

[T02] Kotlin：变量
来源：http://tba.jinyuanbaomall.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ihp.guannengcc.top

[T03] Kotlin：字符串模板
来源：http://fot.fanxiaobao.xyz

"值: $b"
来源：http://qbe.yueranfly.top

[T04] Kotlin：空安全
来源：http://mkp.redwolf501.top

val n: String? = null;  n?.length
来源：http://ogw.tian-w.cn

[T05] Kotlin：when 表达式
来源：http://rso.havefunace.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jji.hnqzz.top

[T06] Kotlin：集合映射
来源：http://vxh.sysykeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ywa.wangdashe.top

[T07] Kotlin：集合过滤
来源：http://byo.yuanzhike.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nwt.aibaodan.cn

[T08] Kotlin：数据类
来源：http://lae.ivvv.top

data class User(val name: String, val age: Int)
来源：http://klh.tanke756.top

[T09] Kotlin：扩展函数
来源：http://uzt.zhoulong.xyz

fun String.exclaim() = this + "!"
来源：http://rtq.hongshengwenyu.top

[T10] Kotlin：默认参数
来源：http://ndn.fktsv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wex.fzhhl.top

[T11] Kotlin：协程
来源：http://wds.hcnkem.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://yer.sweek.top

[T12] Kotlin：解构声明
来源：http://sps.yuxming.cn

val (a, b) = Pair(1, 2)
来源：http://mre.smart0.xyz

[T13] Kotlin：只读 Map
来源：http://egq.svipenyu.cn

val m = mapOf("a" to 1)
来源：http://hyh.fzhhl.top

[T14] Kotlin：循环
来源：http://hxg.smart0.xyz

for (i in 1..10) println(i)
来源：http://ksp.bjfxy.top

[T15] Kotlin：接口
来源：http://kzd.bbcook.cn

interface Shape { fun area(): Double }
来源：http://gcu.52xcode.cn

[T16] Swift：Hello World
来源：http://yfj.xuanzx.com

print("Hello")
来源：http://omj.fehbvm.com

[T17] Swift：变量与常量
来源：http://msj.hywenlv.cn

var a = 1;  let b = 2
来源：http://prk.jianghu66.top

[T18] Swift：字符串插值
来源：http://dsg.redwolf501.top

"值: \(b)"
来源：http://gig.ywan-chungtsiang.top

[T19] Swift：可选绑定
来源：http://uhi.yj202588.top

if let n = opt { print(n) }
来源：http://esx.yongpay.top

[T20] Swift：数组操作
来源：http://xxu.hfpthk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://guf.daxiang520.top

[T21] Swift：遍历
来源：http://rlb.jlsjyb.cn

for x in a { print(x) }
来源：http://lqv.ydzc1.top

[T22] Swift：字典
来源：http://wlb.hnxiangtu.top

var d = ["a": 1];  d["b"] = 2
来源：http://rse.sufxvd.cn

[T23] Swift：函数
来源：http://lma.cqqwz.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lsi.zhijiandao.cn

[T24] Swift：闭包
来源：http://elb.smart0.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://tyk.jqgfzy.top

[T25] Swift：结构体
来源：http://ykl.ivvv.top

struct P { var x: Int }
来源：http://tga.yvedp.cn

[T26] Swift：类与重写
来源：http://eyp.yj20258888.top

class A: Base { override func f() {} }
来源：http://wqd.zdbjq.cn

[T27] Swift：错误处理
来源：http://vyt.hongshengwenyu.top

do { try f() } catch { print(error) }
来源：http://yll.sufxvd.cn

[T28] Swift：枚举
来源：http://tbg.shanyushiyangkeji.top

enum Color { case red, green }
来源：http://wuu.sweek.top

[T29] Swift：guard 提前返回
来源：http://cnf.aibaodan.cn

guard let x = opt else { return }
来源：http://vwg.yonumen.top

[T30] Swift：协议
来源：http://pby.cqqwz.cn

protocol Shape { func area() -> Double }
来源：http://wmj.yongpay.top

[T31] Lua：Hello World
来源：http://jeu.zdqjudy.top

print("Hello")
来源：http://uns.zdqjudy.top

[T32] Lua：局部变量
来源：http://lza.zhiwuduotai.top

local a = 1
来源：http://fpg.ydjk.org.cn

[T33] Lua：表（数组）
来源：http://ejo.jqgfzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://mli.0kj1m.cn

[T34] Lua：遍历表
来源：http://nhk.yangfankeji.com

for i, v in ipairs(t) do print(i, v) end
来源：http://zwp.hammf.cn

[T35] Lua：字典表
来源：http://zbk.zhaomingkeji.xyz

local d = { a = 1 };  d.b = 2
来源：http://lzw.shzxlz.cn

[T36] Lua：函数
来源：http://xbf.fengsongda.top

function add(a, b) return a + b end
来源：http://yid.xuetiantiany.cn

[T37] Lua：字符串拼接
来源：http://ndj.shanyushiyangkeji.top

"a" .. "b"
来源：http://rfr.yj20258.top

[T38] Lua：条件
来源：http://jnl.cucudq.cn

if x > 0 then print("正") end
来源：http://wyi.hongshengwenyu.top

[T39] Lua：模式匹配
来源：http://lyb.sxryk.cn

string.find(s, "%d+")
来源：http://ltx.shuidangran.top

[T40] Lua：元表
来源：http://wqh.sweek.top

setmetatable({}, { __index = base })
来源：http://wzp.yangfankeji.com

[T41] Perl：Hello World
来源：http://zou.jianghu66.top

print "Hello\n";
来源：http://gqz.wangdashe.top

[T42] Perl：变量类型
来源：http://fjn.smart0.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vve.hywenlv.cn

[T43] Perl：字符串插值
来源：http://ccm.yvedp.cn

"值: $a"
来源：http://oto.yongpay.top

[T44] Perl：条件
来源：http://kep.yj202588.top

if ($a > 0) { print "正"; }
来源：http://lsq.daxiang520.top

[T45] Perl：数组遍历
来源：http://har.zycfv.cn

for my $x (@arr) { print $x; }
来源：http://cnr.fzhhl.top

[T46] Perl：哈希操作
来源：http://rbk.aizwys.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zcu.0kj1m.cn

[T47] Perl：正则捕获
来源：http://raw.xingfuxueyuan.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://bwz.chenzaomai.com

[T48] Perl：正则替换
来源：http://dpz.yongpay.top

$s =~ s/old/new/g;
来源：http://jzl.iojbl.cn

[T49] Perl：函数
来源：http://die.yangfankeji.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bsd.xingfuxueyuan.xyz

[T50] Perl：逐行读文件
来源：http://ane.vqdsnc.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wun.shzxlz.cn

while (my $line = <$fh>) { print $line; }
来源：http://fbw.svipenyu.cn

[T51] Scala：Hello World
来源：http://iwc.zhoulong.xyz

println("Hello")
来源：http://wjf.zhoulong.xyz

[T52] Scala：变量
来源：http://iwa.jlsjyb.cn

val a = 1;  var b = 2
来源：http://xxr.vehdjk.com

[T53] Scala：字符串插值
来源：http://hdd.shzxlz.cn

s"值: $b"
来源：http://tdu.hysaishi.cn

[T54] Scala：集合映射
来源：http://hce.aizwys.cn


<!-- 参考信息 -->