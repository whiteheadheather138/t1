代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xzb.gotoacloud.top

[R54] 比较两个文件
来源：http://lca.meibo888.top

diff a.txt b.txt
来源：http://stv.havefunace.top

[R55] 压缩与解压
来源：http://qtb.birdmap.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://eyh.zycfv.cn

[R56] 远程拷贝
来源：http://qgt.vqdsnc.cn

scp file user@host:/path/
来源：http://zcf.hcnkem.com

[R57] 远程执行命令
来源：http://dmy.wangdashe.top

ssh user@host 'uptime'
来源：http://ghu.wangshuangyany.cn

[R58] 下载文件
来源：http://jdb.chenlongwang.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://doy.yfazqb.com

[R59] 发 POST JSON
来源：http://vgn.zhongyouzk.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bws.pycfn.com

[R60] 只看 HTTP 状态码
来源：http://pej.yuxming.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hmw.jiagoushi.top

[R61] 磁盘占用
来源：http://tcn.uphjek.com

df -h;  du -sh *
来源：http://ovl.cashguo.top

[R62] 找最占空间的文件
来源：http://agl.zhixingplan.top

du -ah . | sort -rh | head -10
来源：http://eqi.shanyushiyangtech.top

[R63] 内存与进程
来源：http://prh.ydzc1.top

free -h;  ps aux | grep nginx
来源：http://zjn.ydzc1.top

[R64] 结束进程
来源：http://bxs.hammf.cn

kill -9 $(pgrep -f app.py)
来源：http://kdd.ivvv.top

[R65] 查看端口占用
来源：http://vni.yfazqb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wkg.vehdjk.com

[R66] 定时任务
来源：http://tcv.tianlin.xyz

crontab -e;  crontab -l
来源：http://vdc.meibo888.top

[R67] 生成随机十六进制串
来源：http://tlu.yueranfly.top

openssl rand -hex 16
来源：http://ibr.quarkkingdee.top

[R68] 计算文件校验值
来源：http://suq.shanyushiyangtech.top

sha256sum a.txt;  md5sum a.txt
来源：http://mav.wangshuangyany.cn

[R69] 生成随机密码
来源：http://ple.hfpthk.cn

head -c 16 /dev/urandom | base64
来源：http://lwi.gzhubu.top

[R70] 时间戳与互转
来源：http://ixu.yonumen.top

date +%s;  date -d @1700000000
来源：http://svt.ywan-chungtsiang.top

[R71] 日期格式化
来源：http://ypc.quarkkingdee.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://kmo.nanxuanxn.top

[R72] 等待端口就绪
来源：http://qyq.xylfe.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wbx.cashguo.top

[R73] 分割大日志
来源：http://tbg.bjfxy.top

split -l 1000 big.log part_
来源：http://dfs.jlsjyb.cn

[R74] 批量重命名
来源：http://xxx.havefunace.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bok.smart0.xyz

[R75] 导出环境变量
来源：http://bga.ydzc1.top

export PATH="$HOME/bin:$PATH"
来源：http://zft.jqgfzy.top

[R76] 使用临时文件
来源：http://hfa.sjlbkw.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bxc.jianghu66.top

[R77] 读取用户输入
来源：http://cjv.zhaomingkeji.xyz

read -rp "请输入: " ans
来源：http://fir.chenjidiqi.icu

[R78] 交互式菜单
来源：http://ine.52xcode.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ikv.meibo888.top

[R79] 解析命令行选项
来源：http://lls.nwbrower.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nfr.daria6918.cn

[R80] 查看脚本执行耗时
来源：http://yni.xuetiantiany.cn

time ./run.sh
来源：http://nhl.yanxiufei.cn

================================================================================
来源：http://eca.chenzaomai.com

S. C / C++ 专题
来源：http://odf.guowangkeji.top

================================================================================
来源：http://kse.jlsjyb.cn

[S01] C：Hello World
来源：http://akx.yfazqb.com

#include <stdio.h>
来源：http://ate.xuetiantiany.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xbv.fzhhl.top

[S02] C：变量与格式化输出
来源：http://wqz.shuidangran.top

int a = 10; printf("%d\n", a);
来源：http://sut.yuanzhike.top

[S03] C：读入整数
来源：http://hua.smart0.xyz

int x; scanf("%d", &x);
来源：http://fbj.bjfxy.top

[S04] C：字符串复制
来源：http://kzt.shangyingyoupin.top

char dst[32]; strcpy(dst, "hi");
来源：http://vfb.yangfankeji.com

[S05] C：字符串长度
来源：http://qki.sweek.top

strlen(s)
来源：http://glx.hesvh.cn

[S06] C：字符串比较
来源：http://gin.tarul.cn

strcmp(a, b) == 0
来源：http://hpj.yueranfly.top

[S07] C：数组遍历求和
来源：http://qde.zhaomingkeji.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://etd.zdbjq.cn

[S08] C：动态内存分配与释放
来源：http://rdx.gogol.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lpx.shzxlz.cn

[S09] C：结构体定义与初始化
来源：http://jrq.fehbvm.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mzt.pycfn.com

[S10] C：指针与解引用
来源：http://wkr.yfazqb.com

int *p = &a;  *p = 5;
来源：http://ayg.hesvh.cn

[S11] C：逐行读文件
来源：http://xmb.tianlin.xyz

FILE *f = fopen("a.txt", "r");
来源：http://btw.52xcode.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wjb.ivvv.top

fclose(f);
来源：http://jns.iojbl.cn

[S12] C：写文件
来源：http://fsb.sweek.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mrn.sweek.top

[S13] C：宏定义
来源：http://sbm.sysykeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lwx.xuanzx.com

[S14] C：枚举
来源：http://qra.cqqwz.cn

enum Color { RED, GREEN, BLUE };
来源：http://esf.yj202588.top

[S15] C：类型转换
来源：http://xsc.hesvh.cn

(double) a / b
来源：http://pyz.shanyushiyangkeji.top

[S16] C：位操作置位
来源：http://ijn.vehdjk.com

x |= (1 << 3);
来源：http://hgc.daxiang520.top

[S17] C：安全拼接字符串
来源：http://mfp.snrcjt.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zvs.gaohongyu789.top

[S18] C：命令行参数
来源：http://pwl.ctjpmb.com

int main(int argc, char **argv)
来源：http://rsg.guannengcc.top

[S19] C：快速排序
来源：http://eau.fktsv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pai.yuanzhike.top

[S20] C：二分查找
来源：http://khi.52xcode.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hqc.cashguo.top

[S21] C：字符类别判断
来源：http://zzu.gogol.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mvp.yanxiufei.cn

[S22] C：字符串转数字
来源：http://rqj.yangfankeji.com

atoi("42");  strtod("3.14", NULL);
来源：http://gwi.wangshuangyany.cn

[S23] C：随机数
来源：http://wlt.yj202588.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fcj.9152youxi.cn

[S24] C：获取本地时间
来源：http://zjl.guannengcc.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tjq.kuanghao11.cn

[S25] C：内存拷贝
来源：http://cft.jinyuanbaomall.cn

memcpy(dst, src, n);
来源：http://pnc.ctjpmb.com

[S26] C：内存清零
来源：http://hll.sufxvd.cn

memset(a, 0, sizeof a);
来源：http://whs.ppjwa.cn

[S27] C：定义常量
来源：http://hvm.xuanzx.com

const double PI = 3.14159;
来源：http://foc.iojbl.cn

[S28] C：静态变量
来源：http://fsz.yueranfly.top

static int counter = 0;
来源：http://fbc.jinqigfzy.top

[S29] C：变参函数
来源：http://nwu.sjlbkw.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jjd.xylfe.cn

[S30] C：头文件保护
来源：http://ots.iojbl.cn

#ifndef X_H
来源：http://vgc.guowangkeji.top

#define X_H
来源：http://elu.uphjek.com

#endif
来源：http://hcx.quarkkingdee.top

[S31] C++：Hello World
来源：http://ntb.daria6918.cn

#include <iostream>
来源：http://qwr.ywan-chungtsiang.top

int main() { std::cout << "Hello\n"; }
来源：http://cqv.yanxiufei.cn

[S32] C++：字符串
来源：http://xyf.xinyue.icu

std::string s = "hi";  s += "!";
来源：http://flu.yuanzhike.top

[S33] C++：vector 增删
来源：http://iry.nanxinkj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kvx.jyoumei.cn

[S34] C++：遍历 vector
来源：http://uau.nanxinkj.top

for (auto &x : v) { std::cout << x; }
来源：http://ldc.gotoacloud.top

[S35] C++：map
来源：http://xit.hongshengwenyu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://iiy.redwolf501.top

[S36] C++：unordered_map
来源：http://sjg.guowangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wzd.yangfankeji.com

[S37] C++：set
来源：http://kza.shangyingyoupin.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://stg.316326.xyz

[S38] C++：排序
来源：http://ssl.zhijiandao.cn

std::sort(v.begin(), v.end());
来源：http://mkb.cheryme.top

[S39] C++：自定义比较器排序
来源：http://tsk.fzhhl.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mcx.tanke756.top

[S40] C++：查找元素
来源：http://tba.jyoumei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xuw.dianchejie.cn

[S41] C++：类与构造函数
来源：http://mod.jinghuilouyu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dlj.yangfankeji.com

[S42] C++：继承与虚函数
来源：http://ufm.zycfv.cn

class B : public Base { public: void f() override {} };
来源：http://brs.ydjk.org.cn

[S43] C++：智能指针
来源：http://ava.fehbvm.com

auto p = std::make_unique<int>(5);
来源：http://dqy.hongshengwenyu.top

[S44] C++：引用传参
来源：http://upb.fehbvm.com

void inc(int &x) { ++x; }
来源：http://bia.zhaomingkeji.xyz

[S45] C++：lambda
来源：http://amk.sxryk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://csk.zhixingplan.top

[S46] C++：函数模板
来源：http://yol.fktsv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mzo.smart0.xyz

[S47] C++：结构化绑定遍历
来源：http://qdo.zhijiandao.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tal.daxiang520.top

[S48] C++：逐行读文件
来源：http://zev.aibaodan.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tzx.nwbrower.top

while (std::getline(in, line)) { }
来源：http://gdr.yueranfly.top

[S49] C++：写文件
来源：http://ijf.fengsongda.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wvb.shuidangran.top

[S50] C++：格式化数字
来源：http://btx.guowangkeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xsg.ydzc1.top

[S51] C++：显式类型转换
来源：http://mtj.fehbvm.com

static_cast<double>(a) / b
来源：http://ouh.chenzaomai.com

[S52] C++：const 与 noexcept
来源：http://jgv.gzhubu.top

int size() const noexcept { return n_; }
来源：http://vaw.jqgfzy.top

[S53] C++：移动语义
来源：http://bzb.zhijiandao.cn

std::vector<int> w = std::move(v);
来源：http://leh.zdqjudy.top

[S54] C++：异常处理
来源：http://kvf.xziqi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pml.gogol.net.cn

[S55] C++：结构化绑定
来源：http://kdg.cqqwz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vmm.quarkkingdee.top

[S56] C++：optional
来源：http://gru.wangdashe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gbh.pycfn.com

[S57] C++：编译期常量
来源：http://cxq.shangyingyoupin.top

constexpr int N = 10;
来源：http://bpr.hnqzz.top

[S58] C++：命名空间
来源：http://unj.andypj.xyz

namespace ns { int f() { return 1; } }
来源：http://qzj.yuanzhike.top

[S59] C++：静态断言
来源：http://zst.tanke756.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lnk.birdmap.top

[S60] C++：遍历并删除元素
来源：http://shc.bjfxy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ade.sysykeji.top

================================================================================
来源：http://izw.fktsv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xlk.xuanzx.com

================================================================================
来源：http://ldu.bjfxy.top

[T01] Kotlin：Hello World
来源：http://yyp.feifeiyinyue.top

println("Hello")
来源：http://swi.yueranfly.top

[T02] Kotlin：变量
来源：http://rjg.hysaishi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://frr.ybcxt.top

[T03] Kotlin：字符串模板
来源：http://lgi.uphjek.com

"值: $b"
来源：http://mdf.jlsjyb.cn

[T04] Kotlin：空安全
来源：http://fll.yanxiufei.cn

val n: String? = null;  n?.length
来源：http://itb.c1oappe.top

[T05] Kotlin：when 表达式
来源：http://vhv.vqdsnc.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ttk.0kj1m.cn

[T06] Kotlin：集合映射
来源：http://bfy.wangdashe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://poi.cqqwz.cn

[T07] Kotlin：集合过滤
来源：http://qao.bjfxy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vhv.xingfuxueyuan.xyz

[T08] Kotlin：数据类
来源：http://zvn.yueranfly.top

data class User(val name: String, val age: Int)
来源：http://dtw.gotoacloud.top

[T09] Kotlin：扩展函数
来源：http://sew.bjfxy.top

fun String.exclaim() = this + "!"
来源：http://epx.bbcook.cn

[T10] Kotlin：默认参数
来源：http://ojy.jinyuanbaomall.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cfc.fengsongda.top

[T11] Kotlin：协程
来源：http://ouw.daria6918.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://aoa.tianlin.xyz

[T12] Kotlin：解构声明
来源：http://uiv.birdmap.top

val (a, b) = Pair(1, 2)
来源：http://ygy.hammf.cn

[T13] Kotlin：只读 Map
来源：http://twp.bbcook.cn

val m = mapOf("a" to 1)
来源：http://fbm.zdbjq.cn

[T14] Kotlin：循环
来源：http://esy.shzxlz.cn

for (i in 1..10) println(i)
来源：http://kuj.cashguo.top

[T15] Kotlin：接口
来源：http://ujw.yj20258888.top

interface Shape { fun area(): Double }
来源：http://rbd.cucudq.cn

[T16] Swift：Hello World
来源：http://qoq.redwolf501.top

print("Hello")
来源：http://wuc.bbcook.cn

[T17] Swift：变量与常量
来源：http://tlc.ybcxt.top

var a = 1;  let b = 2
来源：http://otn.shuidangran.top

[T18] Swift：字符串插值
来源：http://agj.c1oappe.top

"值: \(b)"
来源：http://jcs.epnwcf.com

[T19] Swift：可选绑定
来源：http://bib.ybcxt.top

if let n = opt { print(n) }
来源：http://giz.ppjwa.cn

[T20] Swift：数组操作
来源：http://rvf.quarkkingdee.top

var a = [1, 2, 3];  a.append(4)
来源：http://obi.zhongyouzk.top

[T21] Swift：遍历
来源：http://iaq.zhixingplan.top

for x in a { print(x) }
来源：http://aah.aibaodan.cn

[T22] Swift：字典
来源：http://stx.yj20258.top

var d = ["a": 1];  d["b"] = 2
来源：http://wxz.zhixingplan.top

[T23] Swift：函数
来源：http://chv.vqdsnc.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nwc.cdnleiting.top

[T24] Swift：闭包
来源：http://flg.zdqjudy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://rsk.jinqigfzy.top

[T25] Swift：结构体
来源：http://anh.sysykeji.top

struct P { var x: Int }
来源：http://xxr.iojbl.cn

[T26] Swift：类与重写
来源：http://qxz.yonumen.top

class A: Base { override func f() {} }
来源：http://tqe.9152youxi.cn

[T27] Swift：错误处理
来源：http://oyl.jinghuilouyu.cn

do { try f() } catch { print(error) }
来源：http://ptk.jyoumei.cn

[T28] Swift：枚举
来源：http://cdl.yangfankeji.com

enum Color { case red, green }
来源：http://dzr.ppjwa.cn

[T29] Swift：guard 提前返回
来源：http://ysw.svipenyu.cn

guard let x = opt else { return }
来源：http://lod.0kj1m.cn

[T30] Swift：协议
来源：http://rju.tarul.cn

protocol Shape { func area() -> Double }
来源：http://eig.shanyushiyangkeji.top

[T31] Lua：Hello World
来源：http://gcc.zhiwuduotai.top

print("Hello")
来源：http://gqv.tian-w.cn

[T32] Lua：局部变量
来源：http://ahf.nanxuanxn.top

local a = 1
来源：http://fmp.shanyushiyangkeji.top

[T33] Lua：表（数组）
来源：http://fxc.nanxinkj.top

local t = {1, 2, 3};  t[4] = 4
来源：http://sdr.uphjek.com

[T34] Lua：遍历表
来源：http://flt.jianghu66.top

for i, v in ipairs(t) do print(i, v) end
来源：http://rpz.mhx1999.top

[T35] Lua：字典表
来源：http://zue.ctjpmb.com

local d = { a = 1 };  d.b = 2
来源：http://uat.tianlin.xyz

[T36] Lua：函数
来源：http://htl.dianchejie.cn

function add(a, b) return a + b end
来源：http://byb.yj20258888.top

[T37] Lua：字符串拼接
来源：http://ela.gotoacloud.top

"a" .. "b"
来源：http://pdj.cashguo.top

[T38] Lua：条件
来源：http://ema.shanyushiyangkeji.top

if x > 0 then print("正") end
来源：http://clu.nanxinkj.top

[T39] Lua：模式匹配
来源：http://obo.sjlbkw.cn

string.find(s, "%d+")
来源：http://zqv.zhaomingkeji.xyz

[T40] Lua：元表
来源：http://pqy.shuidangran.top

setmetatable({}, { __index = base })
来源：http://ere.dianchejie.cn

[T41] Perl：Hello World
来源：http://xkn.yj202588.top

print "Hello\n";
来源：http://bbn.xingfuxueyuan.xyz

[T42] Perl：变量类型
来源：http://jsp.dianchejie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lxs.gotoacloud.top

[T43] Perl：字符串插值
来源：http://hwi.xuetiantiany.cn

"值: $a"
来源：http://gzb.xuanzx.com

[T44] Perl：条件
来源：http://jwk.xziqi.cn

if ($a > 0) { print "正"; }
来源：http://zku.cqqwz.cn

[T45] Perl：数组遍历
来源：http://ogu.epnwcf.com

for my $x (@arr) { print $x; }
来源：http://umd.gaohongyu789.top

[T46] Perl：哈希操作
来源：http://ytt.uphjek.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zde.fehbvm.com

[T47] Perl：正则捕获
来源：http://usq.yangfankeji.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://yxy.fengsongda.top

[T48] Perl：正则替换
来源：http://jjy.ctjpmb.com

$s =~ s/old/new/g;
来源：http://kjc.ppjwa.cn

[T49] Perl：函数
来源：http://kkd.chenjidiqi.icu

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gwq.shangyingyoupin.top

[T50] Perl：逐行读文件
来源：http://vqd.shanyushiyangtech.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hud.meibo888.top

while (my $line = <$fh>) { print $line; }
来源：http://ohx.jinghuilouyu.cn

[T51] Scala：Hello World
来源：http://nhj.jinqigufen.top

println("Hello")
来源：http://awd.quarkkingdee.top

[T52] Scala：变量
来源：http://umf.fzhhl.top

val a = 1;  var b = 2
来源：http://lbt.mhx1999.top

[T53] Scala：字符串插值
来源：http://gyb.nanxinkj.top

s"值: $b"
来源：http://tbm.uphjek.com

[T54] Scala：集合映射
来源：http://dty.ydjk.org.cn

List(1, 2, 3).map(_ * 2)
来源：http://tiv.fehbvm.com

[T55] Scala：集合过滤
来源：http://fdu.smart0.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://elc.bjfxy.top

[T56] Scala：样例类
来源：http://dzk.yueranfly.top


<!-- 参考信息 -->