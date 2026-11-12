代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tpq.nanxuanxn.top

[R60] 只看 HTTP 状态码
来源：http://lhy.smart0.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bue.quarkkingdee.top

[R61] 磁盘占用
来源：http://arg.zhengqikj.top

df -h;  du -sh *
来源：http://esh.hnxiangtu.top

[R62] 找最占空间的文件
来源：http://zhz.cheryme.top

du -ah . | sort -rh | head -10
来源：http://yez.hywenlv.cn

[R63] 内存与进程
来源：http://cxe.zhoulong.xyz

free -h;  ps aux | grep nginx
来源：http://cag.sysykeji.top

[R64] 结束进程
来源：http://lay.hnqzz.top

kill -9 $(pgrep -f app.py)
来源：http://mso.cashguo.top

[R65] 查看端口占用
来源：http://oxk.wangdashe.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nkd.redwolf501.top

[R66] 定时任务
来源：http://nzc.hnqzz.top

crontab -e;  crontab -l
来源：http://fkn.pengpengdd.cyou

[R67] 生成随机十六进制串
来源：http://mkg.redwolf501.top

openssl rand -hex 16
来源：http://gsn.jqgfzy.top

[R68] 计算文件校验值
来源：http://kxz.yuxming.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wnk.snrcjt.cn

[R69] 生成随机密码
来源：http://gnt.zdqjudy.top

head -c 16 /dev/urandom | base64
来源：http://xjl.sufxvd.cn

[R70] 时间戳与互转
来源：http://udn.zhaomingkeji.xyz

date +%s;  date -d @1700000000
来源：http://mom.ydzc1.top

[R71] 日期格式化
来源：http://jdv.tianlin.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://hoa.jinqigufen.top

[R72] 等待端口就绪
来源：http://ozy.hnqzz.top

until nc -z localhost 3306; do sleep 1; done
来源：http://xvc.ywan-chungtsiang.top

[R73] 分割大日志
来源：http://izl.jinqigfzy.top

split -l 1000 big.log part_
来源：http://rdp.yfazqb.com

[R74] 批量重命名
来源：http://tvz.ivvv.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://faz.ivvv.top

[R75] 导出环境变量
来源：http://den.yj20258888.top

export PATH="$HOME/bin:$PATH"
来源：http://udr.feifeiyinyue.top

[R76] 使用临时文件
来源：http://dun.tanke756.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://igj.shangyingyoupin.top

[R77] 读取用户输入
来源：http://rcv.uphjek.com

read -rp "请输入: " ans
来源：http://xfk.feifeiyinyue.top

[R78] 交互式菜单
来源：http://ovd.xziqi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nsg.pycfn.com

[R79] 解析命令行选项
来源：http://sme.zdqjudy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rsg.jinqigfzy.top

[R80] 查看脚本执行耗时
来源：http://xym.ybcxt.top

time ./run.sh
来源：http://tkw.shzxlz.cn

================================================================================
来源：http://chy.yongpay.top

S. C / C++ 专题
来源：http://nef.chenjidiqi.icu

================================================================================
来源：http://dvq.zycfv.cn

[S01] C：Hello World
来源：http://iof.fengsongda.top

#include <stdio.h>
来源：http://rdb.xziqi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vpx.meibo888.top

[S02] C：变量与格式化输出
来源：http://ecf.hysaishi.cn

int a = 10; printf("%d\n", a);
来源：http://gsg.shanyushiyangkeji.top

[S03] C：读入整数
来源：http://ebs.aibaodan.cn

int x; scanf("%d", &x);
来源：http://ufz.ybcxt.top

[S04] C：字符串复制
来源：http://tzp.bbcook.cn

char dst[32]; strcpy(dst, "hi");
来源：http://szo.cheryme.top

[S05] C：字符串长度
来源：http://yui.yuxming.cn

strlen(s)
来源：http://eoa.xylfe.cn

[S06] C：字符串比较
来源：http://guy.yuxming.cn

strcmp(a, b) == 0
来源：http://iqd.nanxinkj.top

[S07] C：数组遍历求和
来源：http://ttf.jianghu66.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rik.zhongyouzk.top

[S08] C：动态内存分配与释放
来源：http://xrj.xuanzx.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pug.fengsongda.top

[S09] C：结构体定义与初始化
来源：http://zwd.hywenlv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ice.daria6918.cn

[S10] C：指针与解引用
来源：http://yjb.ehwqpu.com

int *p = &a;  *p = 5;
来源：http://mjv.zhaomingkeji.xyz

[S11] C：逐行读文件
来源：http://fau.zhiwuduotai.top

FILE *f = fopen("a.txt", "r");
来源：http://tiy.andypj.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://awq.yvedp.cn

fclose(f);
来源：http://drb.jqgfzy.top

[S12] C：写文件
来源：http://vyb.jianghu66.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jmt.zdqjudy.top

[S13] C：宏定义
来源：http://wao.sysykeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eqv.jqgfzy.top

[S14] C：枚举
来源：http://mtg.zhiwuduotai.top

enum Color { RED, GREEN, BLUE };
来源：http://kkm.zhiwuduotai.top

[S15] C：类型转换
来源：http://ymx.ehwqpu.com

(double) a / b
来源：http://por.zdqjudy.top

[S16] C：位操作置位
来源：http://upl.svipenyu.cn

x |= (1 << 3);
来源：http://qhh.jinqigfzy.top

[S17] C：安全拼接字符串
来源：http://ixx.shanyushiyangtech.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://map.aibaodan.cn

[S18] C：命令行参数
来源：http://nmc.ydzc1.top

int main(int argc, char **argv)
来源：http://wjg.fanxiaobao.xyz

[S19] C：快速排序
来源：http://uvb.feifeiyinyue.top

qsort(a, n, sizeof(int), cmp);
来源：http://owo.nwbrower.top

[S20] C：二分查找
来源：http://yor.ywan-chungtsiang.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bnp.52xcode.cn

[S21] C：字符类别判断
来源：http://npy.shzxlz.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pvm.zhiwuduotai.top

[S22] C：字符串转数字
来源：http://gsp.yvedp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://uzv.xinyue.icu

[S23] C：随机数
来源：http://usr.xuetiantiany.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lfo.c1oappe.top

[S24] C：获取本地时间
来源：http://kmj.quarkkingdee.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kob.hnxiangtu.top

[S25] C：内存拷贝
来源：http://gzk.yvedp.cn

memcpy(dst, src, n);
来源：http://ahz.jyoumei.cn

[S26] C：内存清零
来源：http://cur.hammf.cn

memset(a, 0, sizeof a);
来源：http://ogx.birdmap.top

[S27] C：定义常量
来源：http://ono.cdnleiting.top

const double PI = 3.14159;
来源：http://ynu.iojbl.cn

[S28] C：静态变量
来源：http://wuf.bbcook.cn

static int counter = 0;
来源：http://xie.jlsjyb.cn

[S29] C：变参函数
来源：http://ihz.haohaochexian.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://olg.cqqwz.cn

[S30] C：头文件保护
来源：http://nzw.yangfankeji.com

#ifndef X_H
来源：http://xus.sweek.top

#define X_H
来源：http://dxl.cheryme.top

#endif
来源：http://bfj.fzhhl.top

[S31] C++：Hello World
来源：http://pxp.yj20258888.top

#include <iostream>
来源：http://jts.cheryme.top

int main() { std::cout << "Hello\n"; }
来源：http://zfh.haohaochexian.top

[S32] C++：字符串
来源：http://ylz.gogol.net.cn

std::string s = "hi";  s += "!";
来源：http://kcw.mhx1999.top

[S33] C++：vector 增删
来源：http://nfs.tianlin.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uuq.nanxuanxn.top

[S34] C++：遍历 vector
来源：http://lav.sxryk.cn

for (auto &x : v) { std::cout << x; }
来源：http://mag.nanxuanxn.top

[S35] C++：map
来源：http://axw.shanyushiyangtech.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vqn.zhijiandao.cn

[S36] C++：unordered_map
来源：http://juc.nanxinkj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cjo.ppjwa.cn

[S37] C++：set
来源：http://mfk.zhijiandao.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hwh.yj20258.top

[S38] C++：排序
来源：http://lsu.daxiang520.top

std::sort(v.begin(), v.end());
来源：http://qzi.ehwqpu.com

[S39] C++：自定义比较器排序
来源：http://zjr.hfpthk.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://msx.xuetiantiany.cn

[S40] C++：查找元素
来源：http://ztn.birdmap.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tho.316326.xyz

[S41] C++：类与构造函数
来源：http://rgo.epnwcf.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kaf.pycfn.com

[S42] C++：继承与虚函数
来源：http://cgv.gzhubu.top

class B : public Base { public: void f() override {} };
来源：http://rle.pengpengdd.cyou

[S43] C++：智能指针
来源：http://dfo.ywan-chungtsiang.top

auto p = std::make_unique<int>(5);
来源：http://rnx.hammf.cn

[S44] C++：引用传参
来源：http://kuz.xziqi.cn

void inc(int &x) { ++x; }
来源：http://lgh.yonumen.top

[S45] C++：lambda
来源：http://rgp.jqgfzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://qny.fanxiaobao.xyz

[S46] C++：函数模板
来源：http://gnb.sufxvd.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fuq.jinqigufen.top

[S47] C++：结构化绑定遍历
来源：http://iwt.ybcxt.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hcp.smart0.xyz

[S48] C++：逐行读文件
来源：http://lac.hywenlv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://acc.xingfuxueyuan.xyz

while (std::getline(in, line)) { }
来源：http://jgs.fzhhl.top

[S49] C++：写文件
来源：http://kdf.daxiang520.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iyl.guowangkeji.top

[S50] C++：格式化数字
来源：http://feg.daxiang520.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vac.hnxiangtu.top

[S51] C++：显式类型转换
来源：http://nox.ydzc1.top

static_cast<double>(a) / b
来源：http://qvw.xinyue.icu

[S52] C++：const 与 noexcept
来源：http://xlz.ywan-chungtsiang.top

int size() const noexcept { return n_; }
来源：http://cih.dashuyun.cn

[S53] C++：移动语义
来源：http://khh.svipenyu.cn

std::vector<int> w = std::move(v);
来源：http://cvp.ydzc1.top

[S54] C++：异常处理
来源：http://hjv.sjlbkw.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://imy.hnxiangtu.top

[S55] C++：结构化绑定
来源：http://fzn.yj20258888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://vww.daria6918.cn

[S56] C++：optional
来源：http://exr.quarkkingdee.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rfc.cheryme.top

[S57] C++：编译期常量
来源：http://ctb.mhx1999.top

constexpr int N = 10;
来源：http://ivk.316326.xyz

[S58] C++：命名空间
来源：http://ewk.ctjpmb.com

namespace ns { int f() { return 1; } }
来源：http://ird.aibaodan.cn

[S59] C++：静态断言
来源：http://bds.quarkkingdee.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xfe.yuanzhike.top

[S60] C++：遍历并删除元素
来源：http://mcp.nanxinkj.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://txv.svipenyu.cn

================================================================================
来源：http://flx.chenzaomai.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://aoz.jyoumei.cn

================================================================================
来源：http://pfj.nanxuanxn.top

[T01] Kotlin：Hello World
来源：http://bxn.tianlin.xyz

println("Hello")
来源：http://amr.iojbl.cn

[T02] Kotlin：变量
来源：http://bne.zhengqikj.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hkt.316326.xyz

[T03] Kotlin：字符串模板
来源：http://wpa.nanxuanxn.top

"值: $b"
来源：http://oqz.nanxuanxn.top

[T04] Kotlin：空安全
来源：http://eyb.jinqigufen.top

val n: String? = null;  n?.length
来源：http://vuu.shanyushiyangkeji.top

[T05] Kotlin：when 表达式
来源：http://ijf.sjlbkw.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ors.hnxiangtu.top

[T06] Kotlin：集合映射
来源：http://xrs.fengsongda.top

listOf(1, 2, 3).map { it * 2 }
来源：http://pqo.aibaodan.cn

[T07] Kotlin：集合过滤
来源：http://rzs.zhengqikj.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://yhe.guannengcc.top

[T08] Kotlin：数据类
来源：http://jhd.jyoumei.cn

data class User(val name: String, val age: Int)
来源：http://haf.c1oappe.top

[T09] Kotlin：扩展函数
来源：http://kli.mhx1999.top

fun String.exclaim() = this + "!"
来源：http://jyb.tian-w.cn

[T10] Kotlin：默认参数
来源：http://rwq.meibo888.top

fun greet(name: String = "World") = "Hi $name"
来源：http://eck.tarul.cn

[T11] Kotlin：协程
来源：http://igs.chenjidiqi.icu

GlobalScope.launch { delay(1000); println("done") }
来源：http://phq.sjlbkw.cn

[T12] Kotlin：解构声明
来源：http://ivt.zdqjudy.top

val (a, b) = Pair(1, 2)
来源：http://yoe.xinyue.icu

[T13] Kotlin：只读 Map
来源：http://lsk.vehdjk.com

val m = mapOf("a" to 1)
来源：http://jgv.xuanzx.com

[T14] Kotlin：循环
来源：http://kyn.pengpengdd.cyou

for (i in 1..10) println(i)
来源：http://rkc.zhongyouzk.top

[T15] Kotlin：接口
来源：http://fmc.zhaomingkeji.xyz

interface Shape { fun area(): Double }
来源：http://zrq.yangfankeji.com

[T16] Swift：Hello World
来源：http://mvb.ywan-chungtsiang.top

print("Hello")
来源：http://xps.havefunace.top

[T17] Swift：变量与常量
来源：http://srv.smart0.xyz

var a = 1;  let b = 2
来源：http://fqs.jinqigufen.top

[T18] Swift：字符串插值
来源：http://bmc.chenlongwang.top

"值: \(b)"
来源：http://ree.zhengqikj.top

[T19] Swift：可选绑定
来源：http://gfu.tianlin.xyz

if let n = opt { print(n) }
来源：http://hcy.jianghu66.top

[T20] Swift：数组操作
来源：http://mjw.316326.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://jxu.snrcjt.cn

[T21] Swift：遍历
来源：http://zgg.svipenyu.cn

for x in a { print(x) }
来源：http://nax.jyoumei.cn

[T22] Swift：字典
来源：http://uaz.zdbjq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yjq.cdnleiting.top

[T23] Swift：函数
来源：http://iyc.birdmap.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://opt.havefunace.top

[T24] Swift：闭包
来源：http://guw.dianchejie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jcr.feifeiyinyue.top

[T25] Swift：结构体
来源：http://rss.guowangkeji.top

struct P { var x: Int }
来源：http://wdv.sufxvd.cn

[T26] Swift：类与重写
来源：http://khk.shzxlz.cn

class A: Base { override func f() {} }
来源：http://mxt.zhixingplan.top

[T27] Swift：错误处理
来源：http://sxz.shangyingyoupin.top

do { try f() } catch { print(error) }
来源：http://kts.nanxinkj.top

[T28] Swift：枚举
来源：http://hmz.ppjwa.cn

enum Color { case red, green }
来源：http://qhn.fengsongda.top

[T29] Swift：guard 提前返回
来源：http://hiu.feifeiyinyue.top

guard let x = opt else { return }
来源：http://wnh.daria6918.cn

[T30] Swift：协议
来源：http://vvi.yfazqb.com

protocol Shape { func area() -> Double }
来源：http://sfz.sjlbkw.cn

[T31] Lua：Hello World
来源：http://bjp.pycfn.com

print("Hello")
来源：http://wkp.jinghuilouyu.cn

[T32] Lua：局部变量
来源：http://afo.aizwys.cn

local a = 1
来源：http://wxs.cheryme.top

[T33] Lua：表（数组）
来源：http://uoz.316326.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://kmy.hysaishi.cn

[T34] Lua：遍历表
来源：http://lwz.aizwys.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://irn.nanxuanxn.top

[T35] Lua：字典表
来源：http://aio.pengpengdd.cyou

local d = { a = 1 };  d.b = 2
来源：http://epg.9152youxi.cn

[T36] Lua：函数
来源：http://tjh.fzhhl.top

function add(a, b) return a + b end
来源：http://sbq.hfpthk.cn

[T37] Lua：字符串拼接
来源：http://lec.gogol.net.cn

"a" .. "b"
来源：http://jwx.cucudq.cn

[T38] Lua：条件
来源：http://vzu.yfazqb.com

if x > 0 then print("正") end
来源：http://zdf.guannengcc.top

[T39] Lua：模式匹配
来源：http://wia.ivvv.top

string.find(s, "%d+")
来源：http://tuo.fehbvm.com

[T40] Lua：元表
来源：http://ggl.shangyingyoupin.top

setmetatable({}, { __index = base })
来源：http://lxa.fzhhl.top

[T41] Perl：Hello World
来源：http://jcm.pengpengdd.cyou

print "Hello\n";
来源：http://yll.zhoulong.xyz

[T42] Perl：变量类型
来源：http://glp.jyoumei.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ani.ivvv.top

[T43] Perl：字符串插值
来源：http://ugr.aibaodan.cn

"值: $a"
来源：http://mis.guowangkeji.top

[T44] Perl：条件
来源：http://kun.smart0.xyz

if ($a > 0) { print "正"; }
来源：http://fzf.ydjk.org.cn

[T45] Perl：数组遍历
来源：http://ppy.sweek.top

for my $x (@arr) { print $x; }
来源：http://hpi.iojbl.cn

[T46] Perl：哈希操作
来源：http://gef.ydjk.org.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rgu.mhx1999.top

[T47] Perl：正则捕获
来源：http://gor.ybcxt.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ile.jinqigfzy.top

[T48] Perl：正则替换
来源：http://uub.jinyuanbaomall.cn

$s =~ s/old/new/g;
来源：http://yvq.aizwys.cn

[T49] Perl：函数
来源：http://fcy.zhiwuduotai.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ajm.fehbvm.com

[T50] Perl：逐行读文件
来源：http://cbc.hywenlv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cmw.hcnkem.com

while (my $line = <$fh>) { print $line; }
来源：http://ova.epnwcf.com

[T51] Scala：Hello World
来源：http://koj.tian-w.cn

println("Hello")
来源：http://jhp.meibo888.top

[T52] Scala：变量
来源：http://rvl.gaohongyu789.top

val a = 1;  var b = 2
来源：http://aqv.jqgufenzy.top

[T53] Scala：字符串插值
来源：http://rdh.sweek.top

s"值: $b"
来源：http://tru.sjlbkw.cn

[T54] Scala：集合映射
来源：http://ryt.fktsv.cn

List(1, 2, 3).map(_ * 2)
来源：http://zdr.jqgfzy.top

[T55] Scala：集合过滤
来源：http://weq.xuetiantiany.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kve.zycfv.cn

[T56] Scala：样例类
来源：http://iaj.daria6918.cn

case class User(name: String, age: Int)
来源：http://zxz.gotoacloud.top

[T57] Scala：模式匹配
来源：http://wmo.daxiang520.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://gib.cashguo.top

[T58] Scala：函数定义
来源：http://clf.meibo888.top

def add(a: Int, b: Int): Int = a + b
来源：http://tio.xuanzx.com

[T59] Scala：循环
来源：http://fxx.guowangkeji.top

for (i <- 1 to 10) println(i)
来源：http://rng.hfpthk.cn

[T60] Scala：折叠
来源：http://zld.meibo888.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mnc.xylfe.cn

================================================================================
来源：http://yux.wangshuangyany.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ddw.hnxiangtu.top

================================================================================
来源：http://chj.ivvv.top


<!-- 参考信息 -->