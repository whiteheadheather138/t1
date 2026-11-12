代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pkp.nanxuanxn.top

[R60] 只看 HTTP 状态码
来源：http://wgx.jinghuilouyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cjv.guowangkeji.top

[R61] 磁盘占用
来源：http://wvd.haohaochexian.top

df -h;  du -sh *
来源：http://fmg.yuanzhike.top

[R62] 找最占空间的文件
来源：http://mbx.jinghuilouyu.cn

du -ah . | sort -rh | head -10
来源：http://bnc.jyoumei.cn

[R63] 内存与进程
来源：http://ipc.jyoumei.cn

free -h;  ps aux | grep nginx
来源：http://wqx.tianlin.xyz

[R64] 结束进程
来源：http://jlb.zhixingplan.top

kill -9 $(pgrep -f app.py)
来源：http://hty.yvedp.cn

[R65] 查看端口占用
来源：http://byw.fehbvm.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hgs.havefunace.top

[R66] 定时任务
来源：http://grj.mhx1999.top

crontab -e;  crontab -l
来源：http://iuv.hcnkem.com

[R67] 生成随机十六进制串
来源：http://uaw.iojbl.cn

openssl rand -hex 16
来源：http://dtt.xingfuxueyuan.xyz

[R68] 计算文件校验值
来源：http://gyu.yj202588.top

sha256sum a.txt;  md5sum a.txt
来源：http://abz.xuetiantiany.cn

[R69] 生成随机密码
来源：http://tuw.yuxming.cn

head -c 16 /dev/urandom | base64
来源：http://ukb.fktsv.cn

[R70] 时间戳与互转
来源：http://opo.gzhubu.top

date +%s;  date -d @1700000000
来源：http://mpr.xuanzx.com

[R71] 日期格式化
来源：http://kxz.epnwcf.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://yco.birdmap.top

[R72] 等待端口就绪
来源：http://jbj.yongpay.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ldc.vehdjk.com

[R73] 分割大日志
来源：http://enr.haohaochexian.top

split -l 1000 big.log part_
来源：http://wbi.nwbrower.top

[R74] 批量重命名
来源：http://swg.wangshuangyany.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ykc.svipenyu.cn

[R75] 导出环境变量
来源：http://osb.tian-w.cn

export PATH="$HOME/bin:$PATH"
来源：http://zxo.tian-w.cn

[R76] 使用临时文件
来源：http://sdy.chenjidiqi.icu

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mls.quarkkingdee.top

[R77] 读取用户输入
来源：http://qfn.epnwcf.com

read -rp "请输入: " ans
来源：http://fhj.c1oappe.top

[R78] 交互式菜单
来源：http://pxf.gogol.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cye.zycfv.cn

[R79] 解析命令行选项
来源：http://vdj.ctjpmb.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wsc.zhaomingkeji.xyz

[R80] 查看脚本执行耗时
来源：http://xra.shangyingyoupin.top

time ./run.sh
来源：http://lnu.hongshengwenyu.top

================================================================================
来源：http://ufz.yonumen.top

S. C / C++ 专题
来源：http://fic.nwbrower.top

================================================================================
来源：http://khr.shanyushiyangkeji.top

[S01] C：Hello World
来源：http://sth.316326.xyz

#include <stdio.h>
来源：http://zpu.hywenlv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nps.yueranfly.top

[S02] C：变量与格式化输出
来源：http://lxc.ppjwa.cn

int a = 10; printf("%d\n", a);
来源：http://cnf.jinyuanbaomall.cn

[S03] C：读入整数
来源：http://lij.gogol.net.cn

int x; scanf("%d", &x);
来源：http://byh.52xcode.cn

[S04] C：字符串复制
来源：http://rka.yj202588.top

char dst[32]; strcpy(dst, "hi");
来源：http://shk.hammf.cn

[S05] C：字符串长度
来源：http://nmv.ppjwa.cn

strlen(s)
来源：http://rui.hcnkem.com

[S06] C：字符串比较
来源：http://bmt.sufxvd.cn

strcmp(a, b) == 0
来源：http://awj.cucudq.cn

[S07] C：数组遍历求和
来源：http://djo.kuanghao11.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mba.sweek.top

[S08] C：动态内存分配与释放
来源：http://rss.nwbrower.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xtt.yfazqb.com

[S09] C：结构体定义与初始化
来源：http://hfv.yongpay.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://stu.aizwys.cn

[S10] C：指针与解引用
来源：http://jze.aibaodan.cn

int *p = &a;  *p = 5;
来源：http://urx.guannengcc.top

[S11] C：逐行读文件
来源：http://eng.epnwcf.com

FILE *f = fopen("a.txt", "r");
来源：http://ucp.jqgfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://obn.gaohongyu789.top

fclose(f);
来源：http://duv.fehbvm.com

[S12] C：写文件
来源：http://kdc.cashguo.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://txm.cashguo.top

[S13] C：宏定义
来源：http://vel.wangshuangyany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dwl.quarkkingdee.top

[S14] C：枚举
来源：http://dac.yuxming.cn

enum Color { RED, GREEN, BLUE };
来源：http://zji.hcnkem.com

[S15] C：类型转换
来源：http://pck.ppjwa.cn

(double) a / b
来源：http://ebm.hnqzz.top

[S16] C：位操作置位
来源：http://hvr.cashguo.top

x |= (1 << 3);
来源：http://pvj.hesvh.cn

[S17] C：安全拼接字符串
来源：http://ywu.ctjpmb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wmo.quarkkingdee.top

[S18] C：命令行参数
来源：http://iuh.sysykeji.top

int main(int argc, char **argv)
来源：http://xgk.yangfankeji.com

[S19] C：快速排序
来源：http://qkd.jqgfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://via.ctjpmb.com

[S20] C：二分查找
来源：http://jsf.jinqigfzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wtj.haohaochexian.top

[S21] C：字符类别判断
来源：http://aih.yuanzhike.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xbp.hnqzz.top

[S22] C：字符串转数字
来源：http://heh.shanyushiyangkeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://vpz.nwbrower.top

[S23] C：随机数
来源：http://nbq.quarkkingdee.top

srand(time(NULL));  int r = rand() % 100;
来源：http://axr.andypj.xyz

[S24] C：获取本地时间
来源：http://jkr.yongpay.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zau.cheryme.top

[S25] C：内存拷贝
来源：http://yby.xylfe.cn

memcpy(dst, src, n);
来源：http://cfd.nanxuanxn.top

[S26] C：内存清零
来源：http://ego.zhiwuduotai.top

memset(a, 0, sizeof a);
来源：http://rbh.chenlongwang.top

[S27] C：定义常量
来源：http://phn.uphjek.com

const double PI = 3.14159;
来源：http://cec.yangfankeji.com

[S28] C：静态变量
来源：http://dap.dianchejie.cn

static int counter = 0;
来源：http://zyq.smart0.xyz

[S29] C：变参函数
来源：http://odp.jlsjyb.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://obl.ybcxt.top

[S30] C：头文件保护
来源：http://qon.hfpthk.cn

#ifndef X_H
来源：http://pzw.daxiang520.top

#define X_H
来源：http://fpi.zhengqikj.top

#endif
来源：http://bfg.xylfe.cn

[S31] C++：Hello World
来源：http://cot.iojbl.cn

#include <iostream>
来源：http://nek.shuidangran.top

int main() { std::cout << "Hello\n"; }
来源：http://flb.hnxiangtu.top

[S32] C++：字符串
来源：http://udp.guannengcc.top

std::string s = "hi";  s += "!";
来源：http://jds.zhixingplan.top

[S33] C++：vector 增删
来源：http://yoe.ywan-chungtsiang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nxp.yueranfly.top

[S34] C++：遍历 vector
来源：http://mrg.yangfankeji.com

for (auto &x : v) { std::cout << x; }
来源：http://xhy.c1oappe.top

[S35] C++：map
来源：http://bbn.ydzc1.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vbu.meibo888.top

[S36] C++：unordered_map
来源：http://wld.zycfv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://idf.hfpthk.cn

[S37] C++：set
来源：http://toh.cheryme.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zvk.vehdjk.com

[S38] C++：排序
来源：http://blf.sweek.top

std::sort(v.begin(), v.end());
来源：http://tci.hfpthk.cn

[S39] C++：自定义比较器排序
来源：http://faf.hcnkem.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fet.gaohongyu789.top

[S40] C++：查找元素
来源：http://xpj.meibo888.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hji.tian-w.cn

[S41] C++：类与构造函数
来源：http://lur.shzxlz.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lxo.ivvv.top

[S42] C++：继承与虚函数
来源：http://dpj.sweek.top

class B : public Base { public: void f() override {} };
来源：http://jks.fzhhl.top

[S43] C++：智能指针
来源：http://usj.bjfxy.top

auto p = std::make_unique<int>(5);
来源：http://wek.cashguo.top

[S44] C++：引用传参
来源：http://nqd.9152youxi.cn

void inc(int &x) { ++x; }
来源：http://waa.fzhhl.top

[S45] C++：lambda
来源：http://xha.nwbrower.top

auto add = [](int a, int b) { return a + b; };
来源：http://gtb.ctjpmb.com

[S46] C++：函数模板
来源：http://qms.chenjidiqi.icu

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fiv.guowangkeji.top

[S47] C++：结构化绑定遍历
来源：http://odq.nwbrower.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ver.guowangkeji.top

[S48] C++：逐行读文件
来源：http://cok.cashguo.top

std::ifstream in("a.txt");  std::string line;
来源：http://niz.cucudq.cn

while (std::getline(in, line)) { }
来源：http://odg.wangshuangyany.cn

[S49] C++：写文件
来源：http://sfl.cqqwz.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://smk.hammf.cn

[S50] C++：格式化数字
来源：http://qjx.ydzc1.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vxv.pengpengdd.cyou

[S51] C++：显式类型转换
来源：http://xow.pengpengdd.cyou

static_cast<double>(a) / b
来源：http://sbs.yongpay.top

[S52] C++：const 与 noexcept
来源：http://sls.hysaishi.cn

int size() const noexcept { return n_; }
来源：http://fze.ywan-chungtsiang.top

[S53] C++：移动语义
来源：http://iob.shangyingyoupin.top

std::vector<int> w = std::move(v);
来源：http://oqs.svipenyu.cn

[S54] C++：异常处理
来源：http://fck.zdbjq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rnz.aibaodan.cn

[S55] C++：结构化绑定
来源：http://voi.ybcxt.top

auto [a, b] = std::make_pair(1, 2);
来源：http://mlr.sjlbkw.cn

[S56] C++：optional
来源：http://vti.tian-w.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://acw.wangdashe.top

[S57] C++：编译期常量
来源：http://myk.zdbjq.cn

constexpr int N = 10;
来源：http://pho.smart0.xyz

[S58] C++：命名空间
来源：http://cwk.hesvh.cn

namespace ns { int f() { return 1; } }
来源：http://akr.c1oappe.top

[S59] C++：静态断言
来源：http://hdg.shzxlz.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://osz.ctjpmb.com

[S60] C++：遍历并删除元素
来源：http://nni.hnxiangtu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oby.sufxvd.cn

================================================================================
来源：http://mku.shangyingyoupin.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pbq.vqdsnc.cn

================================================================================
来源：http://gcv.zdqjudy.top

[T01] Kotlin：Hello World
来源：http://ukd.fanxiaobao.xyz

println("Hello")
来源：http://bbr.zhixingplan.top

[T02] Kotlin：变量
来源：http://vnu.zhiwuduotai.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gcn.yvedp.cn

[T03] Kotlin：字符串模板
来源：http://arl.gaohongyu789.top

"值: $b"
来源：http://pag.gzhubu.top

[T04] Kotlin：空安全
来源：http://yii.yongpay.top

val n: String? = null;  n?.length
来源：http://vmy.tanke756.top

[T05] Kotlin：when 表达式
来源：http://rjn.yongpay.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ndy.nanxinkj.top

[T06] Kotlin：集合映射
来源：http://xgu.bjfxy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://yeb.nanxinkj.top

[T07] Kotlin：集合过滤
来源：http://kow.epnwcf.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://zzq.shzxlz.cn

[T08] Kotlin：数据类
来源：http://olo.bjfxy.top

data class User(val name: String, val age: Int)
来源：http://ylu.tanke756.top

[T09] Kotlin：扩展函数
来源：http://bsb.yanxiufei.cn

fun String.exclaim() = this + "!"
来源：http://rix.gotoacloud.top

[T10] Kotlin：默认参数
来源：http://ips.zhongyouzk.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nqn.feifeiyinyue.top

[T11] Kotlin：协程
来源：http://dub.smart0.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://fqj.guowangkeji.top

[T12] Kotlin：解构声明
来源：http://tsf.ybcxt.top

val (a, b) = Pair(1, 2)
来源：http://trv.tanke756.top

[T13] Kotlin：只读 Map
来源：http://rqd.yongpay.top

val m = mapOf("a" to 1)
来源：http://yls.jqgufenzy.top

[T14] Kotlin：循环
来源：http://qqy.wangshuangyany.cn

for (i in 1..10) println(i)
来源：http://rrg.cdnleiting.top

[T15] Kotlin：接口
来源：http://bye.xinyue.icu

interface Shape { fun area(): Double }
来源：http://uhu.guowangkeji.top

[T16] Swift：Hello World
来源：http://toh.jianghu66.top

print("Hello")
来源：http://ckf.bbcook.cn

[T17] Swift：变量与常量
来源：http://tnb.yangfankeji.com

var a = 1;  let b = 2
来源：http://hhw.epnwcf.com

[T18] Swift：字符串插值
来源：http://nnp.xuanzx.com

"值: \(b)"
来源：http://jan.chenlongwang.top

[T19] Swift：可选绑定
来源：http://lby.gaohongyu789.top

if let n = opt { print(n) }
来源：http://uor.0kj1m.cn

[T20] Swift：数组操作
来源：http://zec.sjlbkw.cn

var a = [1, 2, 3];  a.append(4)
来源：http://unh.jiagoushi.top

[T21] Swift：遍历
来源：http://esq.yanxiufei.cn

for x in a { print(x) }
来源：http://sdt.yj20258888.top

[T22] Swift：字典
来源：http://sce.redwolf501.top

var d = ["a": 1];  d["b"] = 2
来源：http://fjx.sysykeji.top

[T23] Swift：函数
来源：http://pnm.zdbjq.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://czz.shangyingyoupin.top

[T24] Swift：闭包
来源：http://oaa.ivvv.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://uyd.zdbjq.cn

[T25] Swift：结构体
来源：http://rvr.chenjidiqi.icu

struct P { var x: Int }
来源：http://zyu.cashguo.top

[T26] Swift：类与重写
来源：http://hla.svipenyu.cn

class A: Base { override func f() {} }
来源：http://ggl.tianlin.xyz

[T27] Swift：错误处理
来源：http://ylp.yuxming.cn

do { try f() } catch { print(error) }
来源：http://gwo.tarul.cn

[T28] Swift：枚举
来源：http://ihc.chenlongwang.top

enum Color { case red, green }
来源：http://mot.hnxiangtu.top

[T29] Swift：guard 提前返回
来源：http://olc.daria6918.cn

guard let x = opt else { return }
来源：http://tvi.guowangkeji.top

[T30] Swift：协议
来源：http://ntc.hcnkem.com

protocol Shape { func area() -> Double }
来源：http://tto.yongpay.top

[T31] Lua：Hello World
来源：http://yti.hnqzz.top

print("Hello")
来源：http://wxo.cqqwz.cn

[T32] Lua：局部变量
来源：http://eya.yanxiufei.cn

local a = 1
来源：http://hgs.svipenyu.cn

[T33] Lua：表（数组）
来源：http://ckf.fehbvm.com

local t = {1, 2, 3};  t[4] = 4
来源：http://kws.gzhubu.top

[T34] Lua：遍历表
来源：http://dci.cheryme.top

for i, v in ipairs(t) do print(i, v) end
来源：http://dom.ywan-chungtsiang.top

[T35] Lua：字典表
来源：http://hab.ydzc1.top

local d = { a = 1 };  d.b = 2
来源：http://khe.meibo888.top

[T36] Lua：函数
来源：http://npo.gzhubu.top

function add(a, b) return a + b end
来源：http://kgn.yangfankeji.com

[T37] Lua：字符串拼接
来源：http://qlt.daria6918.cn

"a" .. "b"
来源：http://raa.dashuyun.cn

[T38] Lua：条件
来源：http://tvb.guowangkeji.top

if x > 0 then print("正") end
来源：http://zpq.yj202588.top

[T39] Lua：模式匹配
来源：http://ulj.shuidangran.top

string.find(s, "%d+")
来源：http://ffr.yongpay.top

[T40] Lua：元表
来源：http://zxc.sweek.top

setmetatable({}, { __index = base })
来源：http://fmn.zhijiandao.cn

[T41] Perl：Hello World
来源：http://ijx.dashuyun.cn

print "Hello\n";
来源：http://tcn.shzxlz.cn

[T42] Perl：变量类型
来源：http://zti.jinyuanbaomall.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bxj.nwbrower.top

[T43] Perl：字符串插值
来源：http://lzh.chenzaomai.com

"值: $a"
来源：http://hgt.iojbl.cn

[T44] Perl：条件
来源：http://omj.feifeiyinyue.top

if ($a > 0) { print "正"; }
来源：http://rdv.cashguo.top

[T45] Perl：数组遍历
来源：http://uvu.zhiwuduotai.top

for my $x (@arr) { print $x; }
来源：http://qea.hfpthk.cn

[T46] Perl：哈希操作
来源：http://dwn.ctjpmb.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://osd.shuidangran.top

[T47] Perl：正则捕获
来源：http://vpj.yj20258888.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://var.iojbl.cn

[T48] Perl：正则替换
来源：http://lgj.meibo888.top

$s =~ s/old/new/g;
来源：http://tvq.bbcook.cn

[T49] Perl：函数
来源：http://jgf.shanyushiyangtech.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jpq.yj202588.top

[T50] Perl：逐行读文件
来源：http://mpa.kuanghao11.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qak.yfazqb.com

while (my $line = <$fh>) { print $line; }
来源：http://mjy.snrcjt.cn

[T51] Scala：Hello World
来源：http://xvs.ybcxt.top

println("Hello")
来源：http://tbk.yj202588.top

[T52] Scala：变量
来源：http://vyq.xinyue.icu

val a = 1;  var b = 2
来源：http://kff.redwolf501.top

[T53] Scala：字符串插值
来源：http://zca.svipenyu.cn

s"值: $b"
来源：http://fwq.52xcode.cn

[T54] Scala：集合映射
来源：http://zbp.yuxming.cn

List(1, 2, 3).map(_ * 2)
来源：http://bht.9152youxi.cn

[T55] Scala：集合过滤
来源：http://uxl.quarkkingdee.top

List(1, 2, 3).filter(_ > 1)
来源：http://sun.jyoumei.cn

[T56] Scala：样例类
来源：http://fqv.feifeiyinyue.top

case class User(name: String, age: Int)
来源：http://grk.jqgfzy.top

[T57] Scala：模式匹配
来源：http://poq.aizwys.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dtr.xinyue.icu

[T58] Scala：函数定义
来源：http://xbx.wangshuangyany.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bcc.bjfxy.top

[T59] Scala：循环
来源：http://eiz.yj20258.top

for (i <- 1 to 10) println(i)
来源：http://wqq.jlsjyb.cn

[T60] Scala：折叠
来源：http://adq.tianlin.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gkb.9152youxi.cn

================================================================================
来源：http://ahp.hesvh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://elz.ydzc1.top

================================================================================
来源：http://chi.shuidangran.top


<!-- 参考信息 -->