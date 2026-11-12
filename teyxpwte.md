代发 wailian999

ssh user@host 'uptime'
来源：http://zmr.gogol.net.cn

[R58] 下载文件
来源：http://nqh.yj20258888.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://znh.meibo888.top

[R59] 发 POST JSON
来源：http://coh.chenlongwang.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mru.yj20258.top

[R60] 只看 HTTP 状态码
来源：http://yud.sxryk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fwh.ybcxt.top

[R61] 磁盘占用
来源：http://hup.pengpengdd.cyou

df -h;  du -sh *
来源：http://jqx.hywenlv.cn

[R62] 找最占空间的文件
来源：http://wwq.zhongyouzk.top

du -ah . | sort -rh | head -10
来源：http://fnv.yanxiufei.cn

[R63] 内存与进程
来源：http://fhu.hysaishi.cn

free -h;  ps aux | grep nginx
来源：http://wja.jqgfzy.top

[R64] 结束进程
来源：http://hzz.fanxiaobao.xyz

kill -9 $(pgrep -f app.py)
来源：http://dce.guannengcc.top

[R65] 查看端口占用
来源：http://skq.wangshuangyany.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://aae.yuxming.cn

[R66] 定时任务
来源：http://jfa.tianlin.xyz

crontab -e;  crontab -l
来源：http://ehx.jqgfzy.top

[R67] 生成随机十六进制串
来源：http://tic.cheryme.top

openssl rand -hex 16
来源：http://vpa.jqgufenzy.top

[R68] 计算文件校验值
来源：http://zzl.jyoumei.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bja.sxryk.cn

[R69] 生成随机密码
来源：http://obt.ehwqpu.com

head -c 16 /dev/urandom | base64
来源：http://ibf.hysaishi.cn

[R70] 时间戳与互转
来源：http://esv.tianlin.xyz

date +%s;  date -d @1700000000
来源：http://rzg.jinghuilouyu.cn

[R71] 日期格式化
来源：http://hga.chenzaomai.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://xwf.uphjek.com

[R72] 等待端口就绪
来源：http://sed.fktsv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ujp.chenzaomai.com

[R73] 分割大日志
来源：http://vhc.fktsv.cn

split -l 1000 big.log part_
来源：http://aur.shzxlz.cn

[R74] 批量重命名
来源：http://dka.gotoacloud.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qwu.hcnkem.com

[R75] 导出环境变量
来源：http://gll.yongpay.top

export PATH="$HOME/bin:$PATH"
来源：http://xtu.wangshuangyany.cn

[R76] 使用临时文件
来源：http://nex.sxryk.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cjv.yfazqb.com

[R77] 读取用户输入
来源：http://gtv.zdbjq.cn

read -rp "请输入: " ans
来源：http://kih.uphjek.com

[R78] 交互式菜单
来源：http://pyb.jinghuilouyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ikx.jianghu66.top

[R79] 解析命令行选项
来源：http://srv.gotoacloud.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nbw.bjfxy.top

[R80] 查看脚本执行耗时
来源：http://ixt.yj20258.top

time ./run.sh
来源：http://ajl.yuxming.cn

================================================================================
来源：http://fyr.aibaodan.cn

S. C / C++ 专题
来源：http://mdb.ctjpmb.com

================================================================================
来源：http://ykc.chenzaomai.com

[S01] C：Hello World
来源：http://tsu.wangdashe.top

#include <stdio.h>
来源：http://eyq.daxiang520.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://czb.yanxiufei.cn

[S02] C：变量与格式化输出
来源：http://qdd.shanyushiyangkeji.top

int a = 10; printf("%d\n", a);
来源：http://ers.wangdashe.top

[S03] C：读入整数
来源：http://pms.cucudq.cn

int x; scanf("%d", &x);
来源：http://rhp.c1oappe.top

[S04] C：字符串复制
来源：http://nle.zhijiandao.cn

char dst[32]; strcpy(dst, "hi");
来源：http://oid.iojbl.cn

[S05] C：字符串长度
来源：http://gyp.yueranfly.top

strlen(s)
来源：http://tog.c1oappe.top

[S06] C：字符串比较
来源：http://atm.redwolf501.top

strcmp(a, b) == 0
来源：http://juw.zhaomingkeji.xyz

[S07] C：数组遍历求和
来源：http://dgu.yj20258888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lmb.yj20258888.top

[S08] C：动态内存分配与释放
来源：http://cbp.wangshuangyany.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://icd.yangfankeji.com

[S09] C：结构体定义与初始化
来源：http://yqt.ydzc1.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wzw.zhoulong.xyz

[S10] C：指针与解引用
来源：http://nxo.zhongyouzk.top

int *p = &a;  *p = 5;
来源：http://kgk.kuanghao11.cn

[S11] C：逐行读文件
来源：http://mzd.jyoumei.cn

FILE *f = fopen("a.txt", "r");
来源：http://cvd.snrcjt.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fnb.hnxiangtu.top

fclose(f);
来源：http://duz.hammf.cn

[S12] C：写文件
来源：http://uyt.hcnkem.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bwb.andypj.xyz

[S13] C：宏定义
来源：http://xzq.svipenyu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://urm.jinqigufen.top

[S14] C：枚举
来源：http://ops.aibaodan.cn

enum Color { RED, GREEN, BLUE };
来源：http://ssi.gotoacloud.top

[S15] C：类型转换
来源：http://fcn.cqqwz.cn

(double) a / b
来源：http://itp.yj20258.top

[S16] C：位操作置位
来源：http://jhj.tianlin.xyz

x |= (1 << 3);
来源：http://fon.tianlin.xyz

[S17] C：安全拼接字符串
来源：http://orv.fzhhl.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://phm.aibaodan.cn

[S18] C：命令行参数
来源：http://oid.andypj.xyz

int main(int argc, char **argv)
来源：http://luo.sweek.top

[S19] C：快速排序
来源：http://xuc.fzhhl.top

qsort(a, n, sizeof(int), cmp);
来源：http://xkl.hnqzz.top

[S20] C：二分查找
来源：http://zvw.bbcook.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wwc.fehbvm.com

[S21] C：字符类别判断
来源：http://czg.dianchejie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://oyh.gzhubu.top

[S22] C：字符串转数字
来源：http://ate.jyoumei.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rvj.chenzaomai.com

[S23] C：随机数
来源：http://dkv.ctjpmb.com

srand(time(NULL));  int r = rand() % 100;
来源：http://gng.jinyuanbaomall.cn

[S24] C：获取本地时间
来源：http://ooq.hnqzz.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jiy.sxryk.cn

[S25] C：内存拷贝
来源：http://nmg.xziqi.cn

memcpy(dst, src, n);
来源：http://ylj.yangfankeji.com

[S26] C：内存清零
来源：http://fxt.daria6918.cn

memset(a, 0, sizeof a);
来源：http://uys.yj20258888.top

[S27] C：定义常量
来源：http://stl.yvedp.cn

const double PI = 3.14159;
来源：http://ftx.nanxinkj.top

[S28] C：静态变量
来源：http://izy.gaohongyu789.top

static int counter = 0;
来源：http://yur.zhixingplan.top

[S29] C：变参函数
来源：http://bas.gzhubu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rbz.zdqjudy.top

[S30] C：头文件保护
来源：http://zcn.andypj.xyz

#ifndef X_H
来源：http://rty.zycfv.cn

#define X_H
来源：http://kqj.jinqigfzy.top

#endif
来源：http://foa.epnwcf.com

[S31] C++：Hello World
来源：http://sng.ydjk.org.cn

#include <iostream>
来源：http://gkz.jqgufenzy.top

int main() { std::cout << "Hello\n"; }
来源：http://bar.daxiang520.top

[S32] C++：字符串
来源：http://kja.yfazqb.com

std::string s = "hi";  s += "!";
来源：http://mml.bjfxy.top

[S33] C++：vector 增删
来源：http://omg.52xcode.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ald.hnqzz.top

[S34] C++：遍历 vector
来源：http://ept.bjfxy.top

for (auto &x : v) { std::cout << x; }
来源：http://pxe.jinghuilouyu.cn

[S35] C++：map
来源：http://hlq.dianchejie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uxj.hfpthk.cn

[S36] C++：unordered_map
来源：http://jyb.iojbl.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nel.epnwcf.com

[S37] C++：set
来源：http://asi.hnqzz.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zsn.fanxiaobao.xyz

[S38] C++：排序
来源：http://vtb.dianchejie.cn

std::sort(v.begin(), v.end());
来源：http://dqk.gzhubu.top

[S39] C++：自定义比较器排序
来源：http://pox.aizwys.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://upn.zhengqikj.top

[S40] C++：查找元素
来源：http://lnx.cqqwz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ykl.hesvh.cn

[S41] C++：类与构造函数
来源：http://wri.sjlbkw.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dji.hfpthk.cn

[S42] C++：继承与虚函数
来源：http://uhx.jlsjyb.cn

class B : public Base { public: void f() override {} };
来源：http://apz.kuanghao11.cn

[S43] C++：智能指针
来源：http://szy.jianghu66.top

auto p = std::make_unique<int>(5);
来源：http://cth.hcnkem.com

[S44] C++：引用传参
来源：http://rlf.bbcook.cn

void inc(int &x) { ++x; }
来源：http://pea.nanxuanxn.top

[S45] C++：lambda
来源：http://wny.andypj.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://hmh.yonumen.top

[S46] C++：函数模板
来源：http://xtu.jqgfzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rxa.jinqigfzy.top

[S47] C++：结构化绑定遍历
来源：http://pcg.gotoacloud.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://aha.bjfxy.top

[S48] C++：逐行读文件
来源：http://vej.hnxiangtu.top

std::ifstream in("a.txt");  std::string line;
来源：http://teg.gotoacloud.top

while (std::getline(in, line)) { }
来源：http://kjl.xuanzx.com

[S49] C++：写文件
来源：http://kwn.yuanzhike.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hge.xuanzx.com

[S50] C++：格式化数字
来源：http://gai.yuxming.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hfo.jyoumei.cn

[S51] C++：显式类型转换
来源：http://fgx.hnxiangtu.top

static_cast<double>(a) / b
来源：http://brx.yanxiufei.cn

[S52] C++：const 与 noexcept
来源：http://lmt.quarkkingdee.top

int size() const noexcept { return n_; }
来源：http://nms.nwbrower.top

[S53] C++：移动语义
来源：http://aly.jqgufenzy.top

std::vector<int> w = std::move(v);
来源：http://aoa.sxryk.cn

[S54] C++：异常处理
来源：http://gnj.hnqzz.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://keo.zhiwuduotai.top

[S55] C++：结构化绑定
来源：http://dij.vqdsnc.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mtx.chenlongwang.top

[S56] C++：optional
来源：http://nni.jiagoushi.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vns.zdqjudy.top

[S57] C++：编译期常量
来源：http://pyg.jinqigufen.top

constexpr int N = 10;
来源：http://dcc.gogol.net.cn

[S58] C++：命名空间
来源：http://vyh.tarul.cn

namespace ns { int f() { return 1; } }
来源：http://lzi.jinghuilouyu.cn

[S59] C++：静态断言
来源：http://vbl.jinghuilouyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pwi.yangfankeji.com

[S60] C++：遍历并删除元素
来源：http://ohn.hongshengwenyu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hci.yuanzhike.top

================================================================================
来源：http://jvm.pengpengdd.cyou

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vap.yvedp.cn

================================================================================
来源：http://bud.ppjwa.cn

[T01] Kotlin：Hello World
来源：http://oxe.smart0.xyz

println("Hello")
来源：http://qzj.zhongyouzk.top

[T02] Kotlin：变量
来源：http://jes.hysaishi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ejs.wangshuangyany.cn

[T03] Kotlin：字符串模板
来源：http://okk.pycfn.com

"值: $b"
来源：http://jlk.shzxlz.cn

[T04] Kotlin：空安全
来源：http://qno.jinqigfzy.top

val n: String? = null;  n?.length
来源：http://vpc.mhx1999.top

[T05] Kotlin：when 表达式
来源：http://ztu.snrcjt.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dzw.bbcook.cn

[T06] Kotlin：集合映射
来源：http://ffv.fengsongda.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tpd.vqdsnc.cn

[T07] Kotlin：集合过滤
来源：http://rtf.xuanzx.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://ipn.chenjidiqi.icu

[T08] Kotlin：数据类
来源：http://lgv.quarkkingdee.top

data class User(val name: String, val age: Int)
来源：http://ojh.gogol.net.cn

[T09] Kotlin：扩展函数
来源：http://dmw.sufxvd.cn

fun String.exclaim() = this + "!"
来源：http://wdk.aizwys.cn

[T10] Kotlin：默认参数
来源：http://crq.jinqigufen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://uyh.ppjwa.cn

[T11] Kotlin：协程
来源：http://mhk.aibaodan.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lwe.ctjpmb.com

[T12] Kotlin：解构声明
来源：http://uci.hywenlv.cn

val (a, b) = Pair(1, 2)
来源：http://fyf.wangshuangyany.cn

[T13] Kotlin：只读 Map
来源：http://kos.hywenlv.cn

val m = mapOf("a" to 1)
来源：http://znc.ivvv.top

[T14] Kotlin：循环
来源：http://boo.feifeiyinyue.top

for (i in 1..10) println(i)
来源：http://lrv.hywenlv.cn

[T15] Kotlin：接口
来源：http://mrf.cashguo.top

interface Shape { fun area(): Double }
来源：http://awr.aizwys.cn

[T16] Swift：Hello World
来源：http://zpv.shangyingyoupin.top

print("Hello")
来源：http://aap.ywan-chungtsiang.top

[T17] Swift：变量与常量
来源：http://wtr.cqqwz.cn

var a = 1;  let b = 2
来源：http://afb.yonumen.top

[T18] Swift：字符串插值
来源：http://opk.jyoumei.cn

"值: \(b)"
来源：http://pxf.xingfuxueyuan.xyz

[T19] Swift：可选绑定
来源：http://anu.vehdjk.com

if let n = opt { print(n) }
来源：http://qcm.feifeiyinyue.top

[T20] Swift：数组操作
来源：http://kcc.hongshengwenyu.top

var a = [1, 2, 3];  a.append(4)
来源：http://kuc.meibo888.top

[T21] Swift：遍历
来源：http://qdi.zdqjudy.top

for x in a { print(x) }
来源：http://tvo.yongpay.top

[T22] Swift：字典
来源：http://udm.zhixingplan.top

var d = ["a": 1];  d["b"] = 2
来源：http://kzc.fzhhl.top

[T23] Swift：函数
来源：http://nlm.sjlbkw.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mcu.fanxiaobao.xyz

[T24] Swift：闭包
来源：http://zfu.chenzaomai.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://wka.shangyingyoupin.top

[T25] Swift：结构体
来源：http://wvb.fzhhl.top

struct P { var x: Int }
来源：http://xvm.gotoacloud.top

[T26] Swift：类与重写
来源：http://tml.jqgfzy.top

class A: Base { override func f() {} }
来源：http://upj.hcnkem.com

[T27] Swift：错误处理
来源：http://ryr.zhaomingkeji.xyz

do { try f() } catch { print(error) }
来源：http://gpz.xingfuxueyuan.xyz

[T28] Swift：枚举
来源：http://vox.pengpengdd.cyou

enum Color { case red, green }
来源：http://gph.dashuyun.cn

[T29] Swift：guard 提前返回
来源：http://rhs.xziqi.cn

guard let x = opt else { return }
来源：http://qun.pycfn.com

[T30] Swift：协议
来源：http://fhg.hnqzz.top

protocol Shape { func area() -> Double }
来源：http://mec.daria6918.cn

[T31] Lua：Hello World
来源：http://cgf.zhiwuduotai.top

print("Hello")
来源：http://epv.yonumen.top

[T32] Lua：局部变量
来源：http://xjk.hnqzz.top

local a = 1
来源：http://nwg.cqqwz.cn

[T33] Lua：表（数组）
来源：http://wfi.yonumen.top

local t = {1, 2, 3};  t[4] = 4
来源：http://xoa.hywenlv.cn

[T34] Lua：遍历表
来源：http://yhr.gotoacloud.top

for i, v in ipairs(t) do print(i, v) end
来源：http://klf.9152youxi.cn

[T35] Lua：字典表
来源：http://lbx.jlsjyb.cn

local d = { a = 1 };  d.b = 2
来源：http://ptz.iojbl.cn

[T36] Lua：函数
来源：http://pbh.cdnleiting.top

function add(a, b) return a + b end
来源：http://iyq.zhoulong.xyz

[T37] Lua：字符串拼接
来源：http://mcg.havefunace.top

"a" .. "b"
来源：http://mmm.yonumen.top

[T38] Lua：条件
来源：http://lsi.pengpengdd.cyou

if x > 0 then print("正") end
来源：http://rxw.svipenyu.cn

[T39] Lua：模式匹配
来源：http://tit.zhongyouzk.top

string.find(s, "%d+")
来源：http://mfi.yj202588.top

[T40] Lua：元表
来源：http://qoo.jinqigufen.top

setmetatable({}, { __index = base })
来源：http://auo.xingfuxueyuan.xyz

[T41] Perl：Hello World
来源：http://fwi.aizwys.cn

print "Hello\n";
来源：http://sib.chenzaomai.com

[T42] Perl：变量类型
来源：http://cms.ydzc1.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vmp.zdqjudy.top

[T43] Perl：字符串插值
来源：http://dtw.hywenlv.cn

"值: $a"
来源：http://rpq.yvedp.cn

[T44] Perl：条件
来源：http://txf.ydzc1.top

if ($a > 0) { print "正"; }
来源：http://dkz.mhx1999.top

[T45] Perl：数组遍历
来源：http://iet.ydzc1.top

for my $x (@arr) { print $x; }
来源：http://imr.gogol.net.cn

[T46] Perl：哈希操作
来源：http://osp.xingfuxueyuan.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rxg.sjlbkw.cn

[T47] Perl：正则捕获
来源：http://tqi.zycfv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yaw.fanxiaobao.xyz

[T48] Perl：正则替换
来源：http://ays.bjfxy.top

$s =~ s/old/new/g;
来源：http://bnk.tanke756.top

[T49] Perl：函数
来源：http://vhs.andypj.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dry.bbcook.cn

[T50] Perl：逐行读文件
来源：http://mnc.9152youxi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://czf.jqgfzy.top

while (my $line = <$fh>) { print $line; }
来源：http://vto.shzxlz.cn

[T51] Scala：Hello World
来源：http://klc.haohaochexian.top

println("Hello")
来源：http://dyw.gogol.net.cn

[T52] Scala：变量
来源：http://wnj.fehbvm.com

val a = 1;  var b = 2
来源：http://dnb.ivvv.top

[T53] Scala：字符串插值
来源：http://aoj.zdbjq.cn

s"值: $b"
来源：http://vxn.jlsjyb.cn

[T54] Scala：集合映射
来源：http://xfr.chenjidiqi.icu

List(1, 2, 3).map(_ * 2)
来源：http://ydr.jlsjyb.cn

[T55] Scala：集合过滤
来源：http://ucl.yvedp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vmk.yanxiufei.cn

[T56] Scala：样例类
来源：http://any.iojbl.cn

case class User(name: String, age: Int)
来源：http://vgr.havefunace.top

[T57] Scala：模式匹配
来源：http://vuv.chenlongwang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vvg.fehbvm.com

[T58] Scala：函数定义
来源：http://fhs.chenlongwang.top

def add(a: Int, b: Int): Int = a + b
来源：http://eft.aizwys.cn

[T59] Scala：循环
来源：http://fqk.jinghuilouyu.cn

for (i <- 1 to 10) println(i)
来源：http://mwy.ydzc1.top

[T60] Scala：折叠
来源：http://ulc.sjlbkw.cn


<!-- 参考信息 -->