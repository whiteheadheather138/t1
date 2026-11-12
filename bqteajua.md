代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pqq.52xcode.cn

[R60] 只看 HTTP 状态码
来源：http://dml.aizwys.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sab.yvedp.cn

[R61] 磁盘占用
来源：http://nvc.dianchejie.cn

df -h;  du -sh *
来源：http://gjl.hfpthk.cn

[R62] 找最占空间的文件
来源：http://loj.hywenlv.cn

du -ah . | sort -rh | head -10
来源：http://rfd.xinyue.icu

[R63] 内存与进程
来源：http://tim.tianlin.xyz

free -h;  ps aux | grep nginx
来源：http://heu.yongpay.top

[R64] 结束进程
来源：http://zox.yangfankeji.com

kill -9 $(pgrep -f app.py)
来源：http://gsv.gogol.net.cn

[R65] 查看端口占用
来源：http://uas.yvedp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tql.yuanzhike.top

[R66] 定时任务
来源：http://rpy.tanke756.top

crontab -e;  crontab -l
来源：http://nfp.shanyushiyangtech.top

[R67] 生成随机十六进制串
来源：http://iua.nwbrower.top

openssl rand -hex 16
来源：http://czh.yfazqb.com

[R68] 计算文件校验值
来源：http://iyf.9152youxi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://znq.9152youxi.cn

[R69] 生成随机密码
来源：http://edp.hysaishi.cn

head -c 16 /dev/urandom | base64
来源：http://qou.sxryk.cn

[R70] 时间戳与互转
来源：http://abg.chenlongwang.top

date +%s;  date -d @1700000000
来源：http://wms.hfpthk.cn

[R71] 日期格式化
来源：http://rdj.hywenlv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://roq.hesvh.cn

[R72] 等待端口就绪
来源：http://joh.yonumen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://com.yj20258.top

[R73] 分割大日志
来源：http://egi.yonumen.top

split -l 1000 big.log part_
来源：http://eub.daria6918.cn

[R74] 批量重命名
来源：http://ttv.dianchejie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nbd.fzhhl.top

[R75] 导出环境变量
来源：http://kxq.tarul.cn

export PATH="$HOME/bin:$PATH"
来源：http://ilg.hnqzz.top

[R76] 使用临时文件
来源：http://hmc.yfazqb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ait.sjlbkw.cn

[R77] 读取用户输入
来源：http://sxq.zhoulong.xyz

read -rp "请输入: " ans
来源：http://itd.yj202588.top

[R78] 交互式菜单
来源：http://xor.yueranfly.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xnj.hcnkem.com

[R79] 解析命令行选项
来源：http://ool.shuidangran.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rdc.haohaochexian.top

[R80] 查看脚本执行耗时
来源：http://qbx.bbcook.cn

time ./run.sh
来源：http://xyq.zhiwuduotai.top

================================================================================
来源：http://jds.zhoulong.xyz

S. C / C++ 专题
来源：http://yep.jinyuanbaomall.cn

================================================================================
来源：http://fof.quarkkingdee.top

[S01] C：Hello World
来源：http://ioq.yanxiufei.cn

#include <stdio.h>
来源：http://uht.sweek.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://zxo.hywenlv.cn

[S02] C：变量与格式化输出
来源：http://nxy.tian-w.cn

int a = 10; printf("%d\n", a);
来源：http://xpw.vqdsnc.cn

[S03] C：读入整数
来源：http://kup.hesvh.cn

int x; scanf("%d", &x);
来源：http://tqg.jinqigfzy.top

[S04] C：字符串复制
来源：http://hge.jqgfzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://hjo.andypj.xyz

[S05] C：字符串长度
来源：http://csx.wangdashe.top

strlen(s)
来源：http://drk.andypj.xyz

[S06] C：字符串比较
来源：http://tpe.hywenlv.cn

strcmp(a, b) == 0
来源：http://ovg.kuanghao11.cn

[S07] C：数组遍历求和
来源：http://yho.zdbjq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ovn.epnwcf.com

[S08] C：动态内存分配与释放
来源：http://lza.svipenyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jjz.zhaomingkeji.xyz

[S09] C：结构体定义与初始化
来源：http://pqn.redwolf501.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lcb.chenlongwang.top

[S10] C：指针与解引用
来源：http://eeq.shangyingyoupin.top

int *p = &a;  *p = 5;
来源：http://zme.epnwcf.com

[S11] C：逐行读文件
来源：http://gaq.gzhubu.top

FILE *f = fopen("a.txt", "r");
来源：http://sxh.gogol.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sey.ydjk.org.cn

fclose(f);
来源：http://cej.fehbvm.com

[S12] C：写文件
来源：http://voj.aibaodan.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gpv.xuanzx.com

[S13] C：宏定义
来源：http://wtl.shangyingyoupin.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wir.quarkkingdee.top

[S14] C：枚举
来源：http://fkm.redwolf501.top

enum Color { RED, GREEN, BLUE };
来源：http://qgw.gaohongyu789.top

[S15] C：类型转换
来源：http://rum.hnxiangtu.top

(double) a / b
来源：http://knm.hnqzz.top

[S16] C：位操作置位
来源：http://gfk.cashguo.top

x |= (1 << 3);
来源：http://cnk.yvedp.cn

[S17] C：安全拼接字符串
来源：http://dej.nanxinkj.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tll.redwolf501.top

[S18] C：命令行参数
来源：http://lpm.zhaomingkeji.xyz

int main(int argc, char **argv)
来源：http://lyr.aizwys.cn

[S19] C：快速排序
来源：http://cdb.zhoulong.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://ymt.smart0.xyz

[S20] C：二分查找
来源：http://lhg.tianlin.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nep.jyoumei.cn

[S21] C：字符类别判断
来源：http://pzt.shanyushiyangkeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nwc.gogol.net.cn

[S22] C：字符串转数字
来源：http://wor.birdmap.top

atoi("42");  strtod("3.14", NULL);
来源：http://ntz.jinqigufen.top

[S23] C：随机数
来源：http://avx.c1oappe.top

srand(time(NULL));  int r = rand() % 100;
来源：http://abl.zdqjudy.top

[S24] C：获取本地时间
来源：http://ksh.zhengqikj.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qrq.kuanghao11.cn

[S25] C：内存拷贝
来源：http://cao.9152youxi.cn

memcpy(dst, src, n);
来源：http://nch.wangshuangyany.cn

[S26] C：内存清零
来源：http://jzw.xylfe.cn

memset(a, 0, sizeof a);
来源：http://mce.jiagoushi.top

[S27] C：定义常量
来源：http://vcs.shangyingyoupin.top

const double PI = 3.14159;
来源：http://lrh.ybcxt.top

[S28] C：静态变量
来源：http://lrl.xylfe.cn

static int counter = 0;
来源：http://tzg.cucudq.cn

[S29] C：变参函数
来源：http://efc.sjlbkw.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wmk.hywenlv.cn

[S30] C：头文件保护
来源：http://nlx.andypj.xyz

#ifndef X_H
来源：http://tuy.52xcode.cn

#define X_H
来源：http://edp.hysaishi.cn

#endif
来源：http://all.snrcjt.cn

[S31] C++：Hello World
来源：http://pwt.xinyue.icu

#include <iostream>
来源：http://bfl.ivvv.top

int main() { std::cout << "Hello\n"; }
来源：http://qlj.52xcode.cn

[S32] C++：字符串
来源：http://qcw.c1oappe.top

std::string s = "hi";  s += "!";
来源：http://bgk.daria6918.cn

[S33] C++：vector 增删
来源：http://bof.yanxiufei.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cgh.xinyue.icu

[S34] C++：遍历 vector
来源：http://knv.fzhhl.top

for (auto &x : v) { std::cout << x; }
来源：http://kjq.xylfe.cn

[S35] C++：map
来源：http://faj.hammf.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qge.chenlongwang.top

[S36] C++：unordered_map
来源：http://vrw.redwolf501.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fyj.ydzc1.top

[S37] C++：set
来源：http://pww.dianchejie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xgu.shanyushiyangtech.top

[S38] C++：排序
来源：http://yed.jyoumei.cn

std::sort(v.begin(), v.end());
来源：http://yax.316326.xyz

[S39] C++：自定义比较器排序
来源：http://upn.ivvv.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sec.shanyushiyangkeji.top

[S40] C++：查找元素
来源：http://rjd.yfazqb.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qtx.52xcode.cn

[S41] C++：类与构造函数
来源：http://imk.bbcook.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jws.hesvh.cn

[S42] C++：继承与虚函数
来源：http://iip.redwolf501.top

class B : public Base { public: void f() override {} };
来源：http://eto.tian-w.cn

[S43] C++：智能指针
来源：http://myp.fehbvm.com

auto p = std::make_unique<int>(5);
来源：http://nte.chenzaomai.com

[S44] C++：引用传参
来源：http://qyy.sysykeji.top

void inc(int &x) { ++x; }
来源：http://gem.fehbvm.com

[S45] C++：lambda
来源：http://qfv.sufxvd.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kpc.yangfankeji.com

[S46] C++：函数模板
来源：http://dzs.sjlbkw.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hgv.hnqzz.top

[S47] C++：结构化绑定遍历
来源：http://uvi.zhiwuduotai.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mks.birdmap.top

[S48] C++：逐行读文件
来源：http://sfx.pengpengdd.cyou

std::ifstream in("a.txt");  std::string line;
来源：http://kcx.sysykeji.top

while (std::getline(in, line)) { }
来源：http://zjs.ydjk.org.cn

[S49] C++：写文件
来源：http://yvm.zhijiandao.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ioe.ehwqpu.com

[S50] C++：格式化数字
来源：http://tjq.hongshengwenyu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://aac.chenjidiqi.icu

[S51] C++：显式类型转换
来源：http://xqh.yonumen.top

static_cast<double>(a) / b
来源：http://mka.cdnleiting.top

[S52] C++：const 与 noexcept
来源：http://roa.shanyushiyangtech.top

int size() const noexcept { return n_; }
来源：http://scn.hesvh.cn

[S53] C++：移动语义
来源：http://fdc.aizwys.cn

std::vector<int> w = std::move(v);
来源：http://hmv.0kj1m.cn

[S54] C++：异常处理
来源：http://pas.snrcjt.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hvi.bbcook.cn

[S55] C++：结构化绑定
来源：http://nqa.hcnkem.com

auto [a, b] = std::make_pair(1, 2);
来源：http://zzl.aibaodan.cn

[S56] C++：optional
来源：http://thq.aibaodan.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gwy.0kj1m.cn

[S57] C++：编译期常量
来源：http://ryt.yangfankeji.com

constexpr int N = 10;
来源：http://tsg.aibaodan.cn

[S58] C++：命名空间
来源：http://bwa.iojbl.cn

namespace ns { int f() { return 1; } }
来源：http://ewq.zhoulong.xyz

[S59] C++：静态断言
来源：http://wzt.hcnkem.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jwh.tianlin.xyz

[S60] C++：遍历并删除元素
来源：http://pkz.jqgufenzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zqy.aibaodan.cn

================================================================================
来源：http://jzo.yanxiufei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tee.kuanghao11.cn

================================================================================
来源：http://kzp.snrcjt.cn

[T01] Kotlin：Hello World
来源：http://wuj.chenjidiqi.icu

println("Hello")
来源：http://hyk.zhiwuduotai.top

[T02] Kotlin：变量
来源：http://jyv.zdbjq.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sfc.jinyuanbaomall.cn

[T03] Kotlin：字符串模板
来源：http://ory.jinghuilouyu.cn

"值: $b"
来源：http://twi.chenlongwang.top

[T04] Kotlin：空安全
来源：http://cmd.hnxiangtu.top

val n: String? = null;  n?.length
来源：http://sfl.redwolf501.top

[T05] Kotlin：when 表达式
来源：http://zsm.hnqzz.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pwv.yongpay.top

[T06] Kotlin：集合映射
来源：http://umc.ybcxt.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tmt.aizwys.cn

[T07] Kotlin：集合过滤
来源：http://wwy.ywan-chungtsiang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rmj.bbcook.cn

[T08] Kotlin：数据类
来源：http://dcy.shanyushiyangtech.top

data class User(val name: String, val age: Int)
来源：http://qsg.iojbl.cn

[T09] Kotlin：扩展函数
来源：http://cje.shzxlz.cn

fun String.exclaim() = this + "!"
来源：http://xzw.wangdashe.top

[T10] Kotlin：默认参数
来源：http://ffz.yangfankeji.com

fun greet(name: String = "World") = "Hi $name"
来源：http://rjr.cashguo.top

[T11] Kotlin：协程
来源：http://xsl.ydjk.org.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ytw.chenjidiqi.icu

[T12] Kotlin：解构声明
来源：http://dcj.uphjek.com

val (a, b) = Pair(1, 2)
来源：http://szb.fzhhl.top

[T13] Kotlin：只读 Map
来源：http://cvb.shanyushiyangtech.top

val m = mapOf("a" to 1)
来源：http://amr.shuidangran.top

[T14] Kotlin：循环
来源：http://qum.ivvv.top

for (i in 1..10) println(i)
来源：http://fqs.xuanzx.com

[T15] Kotlin：接口
来源：http://gne.jqgfzy.top

interface Shape { fun area(): Double }
来源：http://rux.daxiang520.top

[T16] Swift：Hello World
来源：http://euk.sysykeji.top

print("Hello")
来源：http://bed.hammf.cn

[T17] Swift：变量与常量
来源：http://wrv.zdbjq.cn

var a = 1;  let b = 2
来源：http://zyf.andypj.xyz

[T18] Swift：字符串插值
来源：http://fcx.snrcjt.cn

"值: \(b)"
来源：http://goo.daria6918.cn

[T19] Swift：可选绑定
来源：http://gqo.hcnkem.com

if let n = opt { print(n) }
来源：http://tdw.cdnleiting.top

[T20] Swift：数组操作
来源：http://uub.gotoacloud.top

var a = [1, 2, 3];  a.append(4)
来源：http://dyb.fengsongda.top

[T21] Swift：遍历
来源：http://zkq.haohaochexian.top

for x in a { print(x) }
来源：http://tno.316326.xyz

[T22] Swift：字典
来源：http://iiy.xziqi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gak.jinghuilouyu.cn

[T23] Swift：函数
来源：http://mdx.xingfuxueyuan.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://let.uphjek.com

[T24] Swift：闭包
来源：http://cuu.jyoumei.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bxr.hammf.cn

[T25] Swift：结构体
来源：http://ift.hongshengwenyu.top

struct P { var x: Int }
来源：http://eeo.9152youxi.cn

[T26] Swift：类与重写
来源：http://jci.shzxlz.cn

class A: Base { override func f() {} }
来源：http://lch.0kj1m.cn

[T27] Swift：错误处理
来源：http://mwo.hongshengwenyu.top

do { try f() } catch { print(error) }
来源：http://vlx.quarkkingdee.top

[T28] Swift：枚举
来源：http://eoc.yuxming.cn

enum Color { case red, green }
来源：http://jbk.c1oappe.top

[T29] Swift：guard 提前返回
来源：http://edb.jinqigufen.top

guard let x = opt else { return }
来源：http://yzt.xziqi.cn

[T30] Swift：协议
来源：http://oyk.yj20258888.top

protocol Shape { func area() -> Double }
来源：http://pvy.ivvv.top

[T31] Lua：Hello World
来源：http://mro.xziqi.cn

print("Hello")
来源：http://arx.dianchejie.cn

[T32] Lua：局部变量
来源：http://mtg.ywan-chungtsiang.top

local a = 1
来源：http://taw.guowangkeji.top

[T33] Lua：表（数组）
来源：http://vzm.cqqwz.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fop.yangfankeji.com

[T34] Lua：遍历表
来源：http://hcy.hesvh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ohk.fktsv.cn

[T35] Lua：字典表
来源：http://hup.cucudq.cn

local d = { a = 1 };  d.b = 2
来源：http://nty.havefunace.top

[T36] Lua：函数
来源：http://nac.nanxuanxn.top

function add(a, b) return a + b end
来源：http://sfd.chenlongwang.top

[T37] Lua：字符串拼接
来源：http://kgs.zhoulong.xyz

"a" .. "b"
来源：http://fqd.fengsongda.top

[T38] Lua：条件
来源：http://kwy.zycfv.cn

if x > 0 then print("正") end
来源：http://lff.hcnkem.com

[T39] Lua：模式匹配
来源：http://bxw.ywan-chungtsiang.top

string.find(s, "%d+")
来源：http://nph.cheryme.top

[T40] Lua：元表
来源：http://cdj.ywan-chungtsiang.top

setmetatable({}, { __index = base })
来源：http://spp.kuanghao11.cn

[T41] Perl：Hello World
来源：http://oms.dianchejie.cn

print "Hello\n";
来源：http://eih.mhx1999.top

[T42] Perl：变量类型
来源：http://vlo.fzhhl.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nrw.ywan-chungtsiang.top

[T43] Perl：字符串插值
来源：http://kmf.fengsongda.top

"值: $a"
来源：http://jqb.52xcode.cn

[T44] Perl：条件
来源：http://kga.fehbvm.com

if ($a > 0) { print "正"; }
来源：http://kdh.fengsongda.top

[T45] Perl：数组遍历
来源：http://bgi.zhongyouzk.top

for my $x (@arr) { print $x; }
来源：http://cec.tian-w.cn

[T46] Perl：哈希操作
来源：http://mju.sxryk.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lke.guannengcc.top

[T47] Perl：正则捕获
来源：http://qsp.jinghuilouyu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://eij.xuetiantiany.cn

[T48] Perl：正则替换
来源：http://hoh.zhoulong.xyz

$s =~ s/old/new/g;
来源：http://pto.wangshuangyany.cn

[T49] Perl：函数
来源：http://nry.hysaishi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gdt.zhoulong.xyz

[T50] Perl：逐行读文件
来源：http://opa.sxryk.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://nmy.nanxuanxn.top

while (my $line = <$fh>) { print $line; }
来源：http://kxz.wangshuangyany.cn

[T51] Scala：Hello World
来源：http://yuz.316326.xyz

println("Hello")
来源：http://lwh.havefunace.top

[T52] Scala：变量
来源：http://ryz.xinyue.icu

val a = 1;  var b = 2
来源：http://kds.gzhubu.top

[T53] Scala：字符串插值
来源：http://xww.sweek.top

s"值: $b"
来源：http://szu.daria6918.cn

[T54] Scala：集合映射
来源：http://vzs.zhaomingkeji.xyz

List(1, 2, 3).map(_ * 2)
来源：http://eod.zhoulong.xyz

[T55] Scala：集合过滤
来源：http://fwu.jinqigufen.top

List(1, 2, 3).filter(_ > 1)
来源：http://wot.jqgufenzy.top

[T56] Scala：样例类
来源：http://tog.nanxuanxn.top

case class User(name: String, age: Int)
来源：http://rsl.yonumen.top

[T57] Scala：模式匹配
来源：http://aen.feifeiyinyue.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vgl.ydzc1.top

[T58] Scala：函数定义
来源：http://byt.zdqjudy.top

def add(a: Int, b: Int): Int = a + b
来源：http://dao.yj20258.top

[T59] Scala：循环
来源：http://hpz.kuanghao11.cn

for (i <- 1 to 10) println(i)
来源：http://jdv.tanke756.top

[T60] Scala：折叠
来源：http://axv.ydjk.org.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uoc.jqgfzy.top

================================================================================
来源：http://skr.dianchejie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sge.chenjidiqi.icu

================================================================================
来源：http://zlt.0kj1m.cn


<!-- 参考信息 -->