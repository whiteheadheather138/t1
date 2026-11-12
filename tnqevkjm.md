代发 wailian999

ssh user@host 'uptime'
来源：http://grg.fehbvm.com

[R58] 下载文件
来源：http://mte.dianchejie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mnk.ppjwa.cn

[R59] 发 POST JSON
来源：http://qpf.fehbvm.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://azz.fehbvm.com

[R60] 只看 HTTP 状态码
来源：http://zmb.haohaochexian.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bnc.yj202588.top

[R61] 磁盘占用
来源：http://sth.fktsv.cn

df -h;  du -sh *
来源：http://zun.tarul.cn

[R62] 找最占空间的文件
来源：http://atp.ctjpmb.com

du -ah . | sort -rh | head -10
来源：http://yex.uphjek.com

[R63] 内存与进程
来源：http://aow.yfazqb.com

free -h;  ps aux | grep nginx
来源：http://iqv.ivvv.top

[R64] 结束进程
来源：http://alu.sysykeji.top

kill -9 $(pgrep -f app.py)
来源：http://epe.sweek.top

[R65] 查看端口占用
来源：http://obz.uphjek.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ckw.fktsv.cn

[R66] 定时任务
来源：http://npj.yongpay.top

crontab -e;  crontab -l
来源：http://luc.jlsjyb.cn

[R67] 生成随机十六进制串
来源：http://jfr.redwolf501.top

openssl rand -hex 16
来源：http://djg.iojbl.cn

[R68] 计算文件校验值
来源：http://wkm.feifeiyinyue.top

sha256sum a.txt;  md5sum a.txt
来源：http://ihp.0kj1m.cn

[R69] 生成随机密码
来源：http://bll.uphjek.com

head -c 16 /dev/urandom | base64
来源：http://wck.sxryk.cn

[R70] 时间戳与互转
来源：http://yft.wangshuangyany.cn

date +%s;  date -d @1700000000
来源：http://xyk.jyoumei.cn

[R71] 日期格式化
来源：http://rvi.cdnleiting.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://rey.mhx1999.top

[R72] 等待端口就绪
来源：http://azc.316326.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://nhr.sweek.top

[R73] 分割大日志
来源：http://jfy.hongshengwenyu.top

split -l 1000 big.log part_
来源：http://bub.dianchejie.cn

[R74] 批量重命名
来源：http://zpx.xuetiantiany.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uvu.tarul.cn

[R75] 导出环境变量
来源：http://hwk.birdmap.top

export PATH="$HOME/bin:$PATH"
来源：http://iof.gogol.net.cn

[R76] 使用临时文件
来源：http://cmt.hesvh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jyn.xylfe.cn

[R77] 读取用户输入
来源：http://ken.9152youxi.cn

read -rp "请输入: " ans
来源：http://xuy.chenjidiqi.icu

[R78] 交互式菜单
来源：http://bre.zhiwuduotai.top

select opt in a b c; do echo "$opt"; break; done
来源：http://smr.yanxiufei.cn

[R79] 解析命令行选项
来源：http://xmx.zhixingplan.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ypy.316326.xyz

[R80] 查看脚本执行耗时
来源：http://ckw.snrcjt.cn

time ./run.sh
来源：http://plv.yuanzhike.top

================================================================================
来源：http://vze.yangfankeji.com

S. C / C++ 专题
来源：http://uqb.ctjpmb.com

================================================================================
来源：http://vdn.mhx1999.top

[S01] C：Hello World
来源：http://vec.zdbjq.cn

#include <stdio.h>
来源：http://ulb.hysaishi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://viv.zhaomingkeji.xyz

[S02] C：变量与格式化输出
来源：http://zaq.hysaishi.cn

int a = 10; printf("%d\n", a);
来源：http://cit.yonumen.top

[S03] C：读入整数
来源：http://npv.gogol.net.cn

int x; scanf("%d", &x);
来源：http://psx.smart0.xyz

[S04] C：字符串复制
来源：http://orm.cashguo.top

char dst[32]; strcpy(dst, "hi");
来源：http://fxw.zdqjudy.top

[S05] C：字符串长度
来源：http://dzv.sjlbkw.cn

strlen(s)
来源：http://lyk.zhongyouzk.top

[S06] C：字符串比较
来源：http://fzg.sjlbkw.cn

strcmp(a, b) == 0
来源：http://myk.zhixingplan.top

[S07] C：数组遍历求和
来源：http://rbm.jinghuilouyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://doc.0kj1m.cn

[S08] C：动态内存分配与释放
来源：http://old.ydzc1.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bnk.yj20258.top

[S09] C：结构体定义与初始化
来源：http://sqk.jyoumei.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vay.shanyushiyangkeji.top

[S10] C：指针与解引用
来源：http://ghe.hcnkem.com

int *p = &a;  *p = 5;
来源：http://fmj.tarul.cn

[S11] C：逐行读文件
来源：http://ape.yfazqb.com

FILE *f = fopen("a.txt", "r");
来源：http://bxs.iojbl.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tya.yj20258.top

fclose(f);
来源：http://gvz.chenlongwang.top

[S12] C：写文件
来源：http://fyd.jqgfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pbv.yangfankeji.com

[S13] C：宏定义
来源：http://bey.hfpthk.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://log.aibaodan.cn

[S14] C：枚举
来源：http://nqh.yj20258.top

enum Color { RED, GREEN, BLUE };
来源：http://cgj.snrcjt.cn

[S15] C：类型转换
来源：http://tzx.bbcook.cn

(double) a / b
来源：http://jhu.chenjidiqi.icu

[S16] C：位操作置位
来源：http://vlr.ydzc1.top

x |= (1 << 3);
来源：http://haz.ivvv.top

[S17] C：安全拼接字符串
来源：http://tnj.vqdsnc.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://das.guowangkeji.top

[S18] C：命令行参数
来源：http://mbo.sufxvd.cn

int main(int argc, char **argv)
来源：http://pjg.zhaomingkeji.xyz

[S19] C：快速排序
来源：http://kzh.xingfuxueyuan.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://ebi.sysykeji.top

[S20] C：二分查找
来源：http://yvv.sxryk.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rgh.guowangkeji.top

[S21] C：字符类别判断
来源：http://nyh.pengpengdd.cyou

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fbr.dianchejie.cn

[S22] C：字符串转数字
来源：http://ebx.cdnleiting.top

atoi("42");  strtod("3.14", NULL);
来源：http://tsr.sweek.top

[S23] C：随机数
来源：http://tji.vehdjk.com

srand(time(NULL));  int r = rand() % 100;
来源：http://iea.zhaomingkeji.xyz

[S24] C：获取本地时间
来源：http://atr.chenjidiqi.icu

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pvi.shangyingyoupin.top

[S25] C：内存拷贝
来源：http://fjs.ywan-chungtsiang.top

memcpy(dst, src, n);
来源：http://zcq.haohaochexian.top

[S26] C：内存清零
来源：http://tfs.hammf.cn

memset(a, 0, sizeof a);
来源：http://mdg.hnqzz.top

[S27] C：定义常量
来源：http://omn.andypj.xyz

const double PI = 3.14159;
来源：http://sgg.feifeiyinyue.top

[S28] C：静态变量
来源：http://nzn.0kj1m.cn

static int counter = 0;
来源：http://fwl.fktsv.cn

[S29] C：变参函数
来源：http://obw.ywan-chungtsiang.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dyv.jinghuilouyu.cn

[S30] C：头文件保护
来源：http://xwp.fktsv.cn

#ifndef X_H
来源：http://ygo.jinqigufen.top

#define X_H
来源：http://gtg.daria6918.cn

#endif
来源：http://cai.zhiwuduotai.top

[S31] C++：Hello World
来源：http://cvc.chenlongwang.top

#include <iostream>
来源：http://crs.smart0.xyz

int main() { std::cout << "Hello\n"; }
来源：http://shw.yongpay.top

[S32] C++：字符串
来源：http://ege.shzxlz.cn

std::string s = "hi";  s += "!";
来源：http://xvd.yangfankeji.com

[S33] C++：vector 增删
来源：http://fsw.ydzc1.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xqz.nwbrower.top

[S34] C++：遍历 vector
来源：http://bpg.svipenyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://acc.cheryme.top

[S35] C++：map
来源：http://kei.hnxiangtu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://psw.hesvh.cn

[S36] C++：unordered_map
来源：http://wfd.0kj1m.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baj.sweek.top

[S37] C++：set
来源：http://lxk.ehwqpu.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jwv.hongshengwenyu.top

[S38] C++：排序
来源：http://dxn.kuanghao11.cn

std::sort(v.begin(), v.end());
来源：http://jhg.hongshengwenyu.top

[S39] C++：自定义比较器排序
来源：http://iuh.chenzaomai.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bcl.wangdashe.top

[S40] C++：查找元素
来源：http://yli.yuanzhike.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://chz.nanxinkj.top

[S41] C++：类与构造函数
来源：http://dun.yvedp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rhc.zdqjudy.top

[S42] C++：继承与虚函数
来源：http://xok.shanyushiyangtech.top

class B : public Base { public: void f() override {} };
来源：http://pfv.cheryme.top

[S43] C++：智能指针
来源：http://drn.9152youxi.cn

auto p = std::make_unique<int>(5);
来源：http://mmq.hongshengwenyu.top

[S44] C++：引用传参
来源：http://tpy.nanxuanxn.top

void inc(int &x) { ++x; }
来源：http://qoj.zhoulong.xyz

[S45] C++：lambda
来源：http://vxx.dashuyun.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xja.sysykeji.top

[S46] C++：函数模板
来源：http://mac.yueranfly.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bmd.shanyushiyangkeji.top

[S47] C++：结构化绑定遍历
来源：http://phh.hysaishi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://exc.hcnkem.com

[S48] C++：逐行读文件
来源：http://tch.yj20258888.top

std::ifstream in("a.txt");  std::string line;
来源：http://ciy.uphjek.com

while (std::getline(in, line)) { }
来源：http://ogl.yangfankeji.com

[S49] C++：写文件
来源：http://nky.mhx1999.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eow.ybcxt.top

[S50] C++：格式化数字
来源：http://twp.jinqigufen.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://snv.fengsongda.top

[S51] C++：显式类型转换
来源：http://cel.aibaodan.cn

static_cast<double>(a) / b
来源：http://ocg.sjlbkw.cn

[S52] C++：const 与 noexcept
来源：http://ybx.zdqjudy.top

int size() const noexcept { return n_; }
来源：http://sfh.0kj1m.cn

[S53] C++：移动语义
来源：http://pkw.daria6918.cn

std::vector<int> w = std::move(v);
来源：http://efz.52xcode.cn

[S54] C++：异常处理
来源：http://nst.snrcjt.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://epr.hywenlv.cn

[S55] C++：结构化绑定
来源：http://dpc.tanke756.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ugw.epnwcf.com

[S56] C++：optional
来源：http://rlo.shangyingyoupin.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qto.zhengqikj.top

[S57] C++：编译期常量
来源：http://odl.sysykeji.top

constexpr int N = 10;
来源：http://vaz.jinghuilouyu.cn

[S58] C++：命名空间
来源：http://giz.bjfxy.top

namespace ns { int f() { return 1; } }
来源：http://kss.zhijiandao.cn

[S59] C++：静态断言
来源：http://zdy.ivvv.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bpd.fengsongda.top

[S60] C++：遍历并删除元素
来源：http://xjm.shzxlz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ycw.yuxming.cn

================================================================================
来源：http://mxc.sjlbkw.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ypx.zycfv.cn

================================================================================
来源：http://qrj.yonumen.top

[T01] Kotlin：Hello World
来源：http://may.ybcxt.top

println("Hello")
来源：http://nkt.jinqigfzy.top

[T02] Kotlin：变量
来源：http://qya.yonumen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wzd.9152youxi.cn

[T03] Kotlin：字符串模板
来源：http://cma.zhoulong.xyz

"值: $b"
来源：http://tkr.jinqigufen.top

[T04] Kotlin：空安全
来源：http://euj.daxiang520.top

val n: String? = null;  n?.length
来源：http://hki.hnxiangtu.top

[T05] Kotlin：when 表达式
来源：http://kxh.guannengcc.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bvd.gaohongyu789.top

[T06] Kotlin：集合映射
来源：http://ojh.fktsv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://slm.dashuyun.cn

[T07] Kotlin：集合过滤
来源：http://jnb.fengsongda.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://sgv.snrcjt.cn

[T08] Kotlin：数据类
来源：http://aoy.yvedp.cn

data class User(val name: String, val age: Int)
来源：http://hfo.iojbl.cn

[T09] Kotlin：扩展函数
来源：http://yre.yfazqb.com

fun String.exclaim() = this + "!"
来源：http://osc.0kj1m.cn

[T10] Kotlin：默认参数
来源：http://cxt.zhoulong.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://drd.jinyuanbaomall.cn

[T11] Kotlin：协程
来源：http://fsg.daxiang520.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://qgd.shzxlz.cn

[T12] Kotlin：解构声明
来源：http://lmo.cdnleiting.top

val (a, b) = Pair(1, 2)
来源：http://aew.hysaishi.cn

[T13] Kotlin：只读 Map
来源：http://toe.nanxuanxn.top

val m = mapOf("a" to 1)
来源：http://blq.52xcode.cn

[T14] Kotlin：循环
来源：http://yxu.chenjidiqi.icu

for (i in 1..10) println(i)
来源：http://wbi.tanke756.top

[T15] Kotlin：接口
来源：http://foi.pengpengdd.cyou

interface Shape { fun area(): Double }
来源：http://cwi.feifeiyinyue.top

[T16] Swift：Hello World
来源：http://ynv.hywenlv.cn

print("Hello")
来源：http://amw.birdmap.top

[T17] Swift：变量与常量
来源：http://brp.aizwys.cn

var a = 1;  let b = 2
来源：http://qca.birdmap.top

[T18] Swift：字符串插值
来源：http://txr.chenzaomai.com

"值: \(b)"
来源：http://egr.zhoulong.xyz

[T19] Swift：可选绑定
来源：http://qre.shzxlz.cn

if let n = opt { print(n) }
来源：http://zeb.jinghuilouyu.cn

[T20] Swift：数组操作
来源：http://wvr.svipenyu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://llt.gotoacloud.top

[T21] Swift：遍历
来源：http://hqv.sweek.top

for x in a { print(x) }
来源：http://csj.nwbrower.top

[T22] Swift：字典
来源：http://rjc.dianchejie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yno.cucudq.cn

[T23] Swift：函数
来源：http://jaa.yj20258.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jqu.iojbl.cn

[T24] Swift：闭包
来源：http://vya.sxryk.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kjd.vqdsnc.cn

[T25] Swift：结构体
来源：http://del.zhengqikj.top

struct P { var x: Int }
来源：http://kaz.tian-w.cn

[T26] Swift：类与重写
来源：http://nzx.xuetiantiany.cn

class A: Base { override func f() {} }
来源：http://our.tanke756.top

[T27] Swift：错误处理
来源：http://xai.dashuyun.cn

do { try f() } catch { print(error) }
来源：http://jlt.bbcook.cn

[T28] Swift：枚举
来源：http://eeq.shanyushiyangkeji.top

enum Color { case red, green }
来源：http://ihl.ivvv.top

[T29] Swift：guard 提前返回
来源：http://gck.pycfn.com

guard let x = opt else { return }
来源：http://rdx.xinyue.icu

[T30] Swift：协议
来源：http://iid.hnqzz.top

protocol Shape { func area() -> Double }
来源：http://hqg.hnxiangtu.top

[T31] Lua：Hello World
来源：http://fwf.yuxming.cn

print("Hello")
来源：http://fki.nanxuanxn.top

[T32] Lua：局部变量
来源：http://prr.jyoumei.cn

local a = 1
来源：http://xdd.tanke756.top

[T33] Lua：表（数组）
来源：http://vhg.jqgufenzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://trf.gaohongyu789.top

[T34] Lua：遍历表
来源：http://yfr.sjlbkw.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://imw.shanyushiyangtech.top

[T35] Lua：字典表
来源：http://idw.mhx1999.top

local d = { a = 1 };  d.b = 2
来源：http://nca.0kj1m.cn

[T36] Lua：函数
来源：http://wcl.yonumen.top

function add(a, b) return a + b end
来源：http://cyx.daria6918.cn

[T37] Lua：字符串拼接
来源：http://mnr.ehwqpu.com

"a" .. "b"
来源：http://kcz.yfazqb.com

[T38] Lua：条件
来源：http://hgg.fengsongda.top

if x > 0 then print("正") end
来源：http://cud.jinyuanbaomall.cn

[T39] Lua：模式匹配
来源：http://ten.zhaomingkeji.xyz

string.find(s, "%d+")
来源：http://zkx.meibo888.top

[T40] Lua：元表
来源：http://hku.sjlbkw.cn

setmetatable({}, { __index = base })
来源：http://wvu.havefunace.top

[T41] Perl：Hello World
来源：http://ute.52xcode.cn

print "Hello\n";
来源：http://qft.zycfv.cn

[T42] Perl：变量类型
来源：http://ict.gogol.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fvh.xziqi.cn

[T43] Perl：字符串插值
来源：http://ogq.gzhubu.top

"值: $a"
来源：http://eku.yj20258888.top

[T44] Perl：条件
来源：http://qan.hammf.cn

if ($a > 0) { print "正"; }
来源：http://ecg.sweek.top

[T45] Perl：数组遍历
来源：http://gqs.hesvh.cn

for my $x (@arr) { print $x; }
来源：http://ito.shanyushiyangtech.top

[T46] Perl：哈希操作
来源：http://lvw.cashguo.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lkp.yfazqb.com

[T47] Perl：正则捕获
来源：http://ebo.bjfxy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://wjf.yuxming.cn

[T48] Perl：正则替换
来源：http://urv.zhongyouzk.top

$s =~ s/old/new/g;
来源：http://ojb.xylfe.cn

[T49] Perl：函数
来源：http://hxp.cdnleiting.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wno.cashguo.top

[T50] Perl：逐行读文件
来源：http://zsg.jinqigufen.top

open my $fh, "<", "a.txt" or die $!;
来源：http://xln.iojbl.cn

while (my $line = <$fh>) { print $line; }
来源：http://uxm.zhixingplan.top

[T51] Scala：Hello World
来源：http://pfh.ivvv.top

println("Hello")
来源：http://xsm.ywan-chungtsiang.top

[T52] Scala：变量
来源：http://quq.316326.xyz

val a = 1;  var b = 2
来源：http://sev.sufxvd.cn

[T53] Scala：字符串插值
来源：http://ztq.xuetiantiany.cn

s"值: $b"
来源：http://mka.yj202588.top

[T54] Scala：集合映射
来源：http://aua.shanyushiyangkeji.top

List(1, 2, 3).map(_ * 2)
来源：http://jtz.yueranfly.top

[T55] Scala：集合过滤
来源：http://blp.sweek.top

List(1, 2, 3).filter(_ > 1)
来源：http://ndd.vehdjk.com

[T56] Scala：样例类
来源：http://jgb.jianghu66.top

case class User(name: String, age: Int)
来源：http://axq.guannengcc.top

[T57] Scala：模式匹配
来源：http://efc.xinyue.icu

x match { case 1 => "一"; case _ => "其他" }
来源：http://cko.sweek.top

[T58] Scala：函数定义
来源：http://ckf.316326.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://lua.hcnkem.com

[T59] Scala：循环
来源：http://txt.quarkkingdee.top

for (i <- 1 to 10) println(i)
来源：http://zdx.zhengqikj.top

[T60] Scala：折叠
来源：http://cad.zhongyouzk.top


<!-- 参考信息 -->