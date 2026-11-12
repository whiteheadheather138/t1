代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wkt.shzxlz.cn

[R60] 只看 HTTP 状态码
来源：http://lxl.fehbvm.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jxs.iojbl.cn

[R61] 磁盘占用
来源：http://fuf.tanke756.top

df -h;  du -sh *
来源：http://iwl.chenlongwang.top

[R62] 找最占空间的文件
来源：http://qen.dianchejie.cn

du -ah . | sort -rh | head -10
来源：http://clr.ppjwa.cn

[R63] 内存与进程
来源：http://fdn.zdqjudy.top

free -h;  ps aux | grep nginx
来源：http://foi.yanxiufei.cn

[R64] 结束进程
来源：http://npc.fengsongda.top

kill -9 $(pgrep -f app.py)
来源：http://scs.zdbjq.cn

[R65] 查看端口占用
来源：http://hbk.snrcjt.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ynm.bjfxy.top

[R66] 定时任务
来源：http://ojl.chenjidiqi.icu

crontab -e;  crontab -l
来源：http://maa.fengsongda.top

[R67] 生成随机十六进制串
来源：http://qwf.mhx1999.top

openssl rand -hex 16
来源：http://sxg.nanxinkj.top

[R68] 计算文件校验值
来源：http://zyy.cqqwz.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pvf.jinqigufen.top

[R69] 生成随机密码
来源：http://wee.uphjek.com

head -c 16 /dev/urandom | base64
来源：http://rim.yuxming.cn

[R70] 时间戳与互转
来源：http://xss.ywan-chungtsiang.top

date +%s;  date -d @1700000000
来源：http://zag.316326.xyz

[R71] 日期格式化
来源：http://rcy.fanxiaobao.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://kbf.zhixingplan.top

[R72] 等待端口就绪
来源：http://pdd.meibo888.top

until nc -z localhost 3306; do sleep 1; done
来源：http://efk.hesvh.cn

[R73] 分割大日志
来源：http://vbd.jqgufenzy.top

split -l 1000 big.log part_
来源：http://jhk.yuxming.cn

[R74] 批量重命名
来源：http://fbx.yangfankeji.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://khp.guannengcc.top

[R75] 导出环境变量
来源：http://wsv.xuetiantiany.cn

export PATH="$HOME/bin:$PATH"
来源：http://elf.aibaodan.cn

[R76] 使用临时文件
来源：http://ufq.tanke756.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ubs.svipenyu.cn

[R77] 读取用户输入
来源：http://qps.yj202588.top

read -rp "请输入: " ans
来源：http://yws.fanxiaobao.xyz

[R78] 交互式菜单
来源：http://hxq.havefunace.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vpf.jinyuanbaomall.cn

[R79] 解析命令行选项
来源：http://qwp.pengpengdd.cyou

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bzt.hnqzz.top

[R80] 查看脚本执行耗时
来源：http://nvv.52xcode.cn

time ./run.sh
来源：http://cbm.daxiang520.top

================================================================================
来源：http://kxx.52xcode.cn

S. C / C++ 专题
来源：http://szz.ybcxt.top

================================================================================
来源：http://cac.jqgfzy.top

[S01] C：Hello World
来源：http://ikl.aibaodan.cn

#include <stdio.h>
来源：http://qag.havefunace.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://zyw.bbcook.cn

[S02] C：变量与格式化输出
来源：http://vre.0kj1m.cn

int a = 10; printf("%d\n", a);
来源：http://ddj.shanyushiyangtech.top

[S03] C：读入整数
来源：http://ezx.hnxiangtu.top

int x; scanf("%d", &x);
来源：http://mhm.zhoulong.xyz

[S04] C：字符串复制
来源：http://zhg.xinyue.icu

char dst[32]; strcpy(dst, "hi");
来源：http://ciw.hysaishi.cn

[S05] C：字符串长度
来源：http://loi.gotoacloud.top

strlen(s)
来源：http://vpl.nanxuanxn.top

[S06] C：字符串比较
来源：http://zwr.hnxiangtu.top

strcmp(a, b) == 0
来源：http://aby.xuanzx.com

[S07] C：数组遍历求和
来源：http://vur.xuanzx.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kvw.52xcode.cn

[S08] C：动态内存分配与释放
来源：http://dcm.haohaochexian.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bvn.hammf.cn

[S09] C：结构体定义与初始化
来源：http://fkn.sysykeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ppu.epnwcf.com

[S10] C：指针与解引用
来源：http://ogu.meibo888.top

int *p = &a;  *p = 5;
来源：http://pzn.cheryme.top

[S11] C：逐行读文件
来源：http://tlm.xingfuxueyuan.xyz

FILE *f = fopen("a.txt", "r");
来源：http://yfx.vehdjk.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://wnd.gogol.net.cn

fclose(f);
来源：http://hln.fanxiaobao.xyz

[S12] C：写文件
来源：http://kah.hysaishi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ogi.zhixingplan.top

[S13] C：宏定义
来源：http://org.haohaochexian.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ddy.chenjidiqi.icu

[S14] C：枚举
来源：http://xjl.feifeiyinyue.top

enum Color { RED, GREEN, BLUE };
来源：http://tjg.zdbjq.cn

[S15] C：类型转换
来源：http://oad.jlsjyb.cn

(double) a / b
来源：http://vbp.jinghuilouyu.cn

[S16] C：位操作置位
来源：http://grp.andypj.xyz

x |= (1 << 3);
来源：http://efc.sufxvd.cn

[S17] C：安全拼接字符串
来源：http://dwd.zhiwuduotai.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gzg.zhoulong.xyz

[S18] C：命令行参数
来源：http://rde.sufxvd.cn

int main(int argc, char **argv)
来源：http://wxk.zdbjq.cn

[S19] C：快速排序
来源：http://seg.jinyuanbaomall.cn

qsort(a, n, sizeof(int), cmp);
来源：http://icj.wangshuangyany.cn

[S20] C：二分查找
来源：http://yll.hysaishi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://htd.andypj.xyz

[S21] C：字符类别判断
来源：http://qfs.tian-w.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uqg.vehdjk.com

[S22] C：字符串转数字
来源：http://htz.jyoumei.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cxs.shangyingyoupin.top

[S23] C：随机数
来源：http://olc.aibaodan.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rqw.fehbvm.com

[S24] C：获取本地时间
来源：http://pgu.cashguo.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kyf.jqgfzy.top

[S25] C：内存拷贝
来源：http://hwb.cdnleiting.top

memcpy(dst, src, n);
来源：http://ksa.sxryk.cn

[S26] C：内存清零
来源：http://jxa.zhixingplan.top

memset(a, 0, sizeof a);
来源：http://wzb.hywenlv.cn

[S27] C：定义常量
来源：http://jwf.dashuyun.cn

const double PI = 3.14159;
来源：http://lyp.zdbjq.cn

[S28] C：静态变量
来源：http://rum.fktsv.cn

static int counter = 0;
来源：http://kzw.chenjidiqi.icu

[S29] C：变参函数
来源：http://lcs.yj20258.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xsi.shangyingyoupin.top

[S30] C：头文件保护
来源：http://djh.andypj.xyz

#ifndef X_H
来源：http://adm.316326.xyz

#define X_H
来源：http://uxg.sjlbkw.cn

#endif
来源：http://som.fktsv.cn

[S31] C++：Hello World
来源：http://ucj.nwbrower.top

#include <iostream>
来源：http://zoq.daxiang520.top

int main() { std::cout << "Hello\n"; }
来源：http://wvs.tanke756.top

[S32] C++：字符串
来源：http://qot.quarkkingdee.top

std::string s = "hi";  s += "!";
来源：http://uow.fehbvm.com

[S33] C++：vector 增删
来源：http://tgj.zhiwuduotai.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zmv.xuanzx.com

[S34] C++：遍历 vector
来源：http://jfa.hongshengwenyu.top

for (auto &x : v) { std::cout << x; }
来源：http://wvf.tanke756.top

[S35] C++：map
来源：http://rgu.zycfv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ize.chenjidiqi.icu

[S36] C++：unordered_map
来源：http://nin.hywenlv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lly.havefunace.top

[S37] C++：set
来源：http://oiv.bjfxy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qip.tian-w.cn

[S38] C++：排序
来源：http://lgb.gotoacloud.top

std::sort(v.begin(), v.end());
来源：http://err.daria6918.cn

[S39] C++：自定义比较器排序
来源：http://wta.bbcook.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zyg.ppjwa.cn

[S40] C++：查找元素
来源：http://hax.shanyushiyangtech.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uwp.cqqwz.cn

[S41] C++：类与构造函数
来源：http://yii.xziqi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://axj.smart0.xyz

[S42] C++：继承与虚函数
来源：http://czv.sysykeji.top

class B : public Base { public: void f() override {} };
来源：http://rdy.uphjek.com

[S43] C++：智能指针
来源：http://utu.xuanzx.com

auto p = std::make_unique<int>(5);
来源：http://okz.cheryme.top

[S44] C++：引用传参
来源：http://hdl.yj20258.top

void inc(int &x) { ++x; }
来源：http://hia.sufxvd.cn

[S45] C++：lambda
来源：http://llb.chenjidiqi.icu

auto add = [](int a, int b) { return a + b; };
来源：http://lwj.chenzaomai.com

[S46] C++：函数模板
来源：http://drl.yj202588.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://aeu.jyoumei.cn

[S47] C++：结构化绑定遍历
来源：http://zsw.chenzaomai.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yge.hfpthk.cn

[S48] C++：逐行读文件
来源：http://stk.xziqi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zhk.xylfe.cn

while (std::getline(in, line)) { }
来源：http://riw.havefunace.top

[S49] C++：写文件
来源：http://yar.zhaomingkeji.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rif.epnwcf.com

[S50] C++：格式化数字
来源：http://xnu.daxiang520.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xdz.hnqzz.top

[S51] C++：显式类型转换
来源：http://hzh.jqgfzy.top

static_cast<double>(a) / b
来源：http://wzt.sjlbkw.cn

[S52] C++：const 与 noexcept
来源：http://rdu.epnwcf.com

int size() const noexcept { return n_; }
来源：http://sqs.yueranfly.top

[S53] C++：移动语义
来源：http://swe.nanxinkj.top

std::vector<int> w = std::move(v);
来源：http://uxv.zhaomingkeji.xyz

[S54] C++：异常处理
来源：http://psd.yueranfly.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://unj.zhongyouzk.top

[S55] C++：结构化绑定
来源：http://cxr.nanxuanxn.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lzw.bbcook.cn

[S56] C++：optional
来源：http://skb.zdbjq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://aig.hongshengwenyu.top

[S57] C++：编译期常量
来源：http://yqs.yuxming.cn

constexpr int N = 10;
来源：http://adw.andypj.xyz

[S58] C++：命名空间
来源：http://yaw.jqgufenzy.top

namespace ns { int f() { return 1; } }
来源：http://jen.quarkkingdee.top

[S59] C++：静态断言
来源：http://qhl.hcnkem.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mut.smart0.xyz

[S60] C++：遍历并删除元素
来源：http://ysv.0kj1m.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hxq.yuxming.cn

================================================================================
来源：http://pvq.havefunace.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xil.jlsjyb.cn

================================================================================
来源：http://nzs.bbcook.cn

[T01] Kotlin：Hello World
来源：http://idt.zhiwuduotai.top

println("Hello")
来源：http://hyd.ybcxt.top

[T02] Kotlin：变量
来源：http://cow.sxryk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ehp.xuetiantiany.cn

[T03] Kotlin：字符串模板
来源：http://iwf.hfpthk.cn

"值: $b"
来源：http://mkv.sysykeji.top

[T04] Kotlin：空安全
来源：http://xsk.gzhubu.top

val n: String? = null;  n?.length
来源：http://zua.snrcjt.cn

[T05] Kotlin：when 表达式
来源：http://meq.wangshuangyany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dnh.fzhhl.top

[T06] Kotlin：集合映射
来源：http://rtg.bjfxy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qen.mhx1999.top

[T07] Kotlin：集合过滤
来源：http://tub.yuanzhike.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://aie.fengsongda.top

[T08] Kotlin：数据类
来源：http://ems.hnqzz.top

data class User(val name: String, val age: Int)
来源：http://hkm.aizwys.cn

[T09] Kotlin：扩展函数
来源：http://bfc.wangshuangyany.cn

fun String.exclaim() = this + "!"
来源：http://ols.jqgufenzy.top

[T10] Kotlin：默认参数
来源：http://miz.dashuyun.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fah.hnqzz.top

[T11] Kotlin：协程
来源：http://ivk.shanyushiyangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://oio.chenzaomai.com

[T12] Kotlin：解构声明
来源：http://cxi.xylfe.cn

val (a, b) = Pair(1, 2)
来源：http://ghp.yueranfly.top

[T13] Kotlin：只读 Map
来源：http://xkn.bjfxy.top

val m = mapOf("a" to 1)
来源：http://ztm.9152youxi.cn

[T14] Kotlin：循环
来源：http://dvq.fzhhl.top

for (i in 1..10) println(i)
来源：http://ojj.jinyuanbaomall.cn

[T15] Kotlin：接口
来源：http://khy.daria6918.cn

interface Shape { fun area(): Double }
来源：http://uay.zdqjudy.top

[T16] Swift：Hello World
来源：http://nij.mhx1999.top

print("Hello")
来源：http://eqp.dashuyun.cn

[T17] Swift：变量与常量
来源：http://xfg.jqgufenzy.top

var a = 1;  let b = 2
来源：http://ucm.yj20258.top

[T18] Swift：字符串插值
来源：http://uey.zhijiandao.cn

"值: \(b)"
来源：http://dpr.sufxvd.cn

[T19] Swift：可选绑定
来源：http://nrr.chenjidiqi.icu

if let n = opt { print(n) }
来源：http://qoj.fehbvm.com

[T20] Swift：数组操作
来源：http://tpq.hysaishi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fpk.jqgfzy.top

[T21] Swift：遍历
来源：http://slf.9152youxi.cn

for x in a { print(x) }
来源：http://myt.ivvv.top

[T22] Swift：字典
来源：http://sfq.ppjwa.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pxr.andypj.xyz

[T23] Swift：函数
来源：http://cel.zycfv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cvj.sweek.top

[T24] Swift：闭包
来源：http://ksn.birdmap.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://dey.hongshengwenyu.top

[T25] Swift：结构体
来源：http://asx.gogol.net.cn

struct P { var x: Int }
来源：http://tzv.gotoacloud.top

[T26] Swift：类与重写
来源：http://ooq.xinyue.icu

class A: Base { override func f() {} }
来源：http://vdb.wangshuangyany.cn

[T27] Swift：错误处理
来源：http://rec.fzhhl.top

do { try f() } catch { print(error) }
来源：http://yer.yj202588.top

[T28] Swift：枚举
来源：http://qne.yongpay.top

enum Color { case red, green }
来源：http://upj.yuxming.cn

[T29] Swift：guard 提前返回
来源：http://air.guannengcc.top

guard let x = opt else { return }
来源：http://ate.ybcxt.top

[T30] Swift：协议
来源：http://puy.hcnkem.com

protocol Shape { func area() -> Double }
来源：http://anv.meibo888.top

[T31] Lua：Hello World
来源：http://qyi.yj20258.top

print("Hello")
来源：http://bqo.aibaodan.cn

[T32] Lua：局部变量
来源：http://gpk.yj20258888.top

local a = 1
来源：http://ezn.ctjpmb.com

[T33] Lua：表（数组）
来源：http://lws.hammf.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cgn.xylfe.cn

[T34] Lua：遍历表
来源：http://hhs.mhx1999.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ocn.sweek.top

[T35] Lua：字典表
来源：http://jzd.cucudq.cn

local d = { a = 1 };  d.b = 2
来源：http://ksu.chenlongwang.top

[T36] Lua：函数
来源：http://ypu.tianlin.xyz

function add(a, b) return a + b end
来源：http://jcd.wangshuangyany.cn

[T37] Lua：字符串拼接
来源：http://mil.yj202588.top

"a" .. "b"
来源：http://crj.zhixingplan.top

[T38] Lua：条件
来源：http://unj.hesvh.cn

if x > 0 then print("正") end
来源：http://ofc.yonumen.top

[T39] Lua：模式匹配
来源：http://ttt.gogol.net.cn

string.find(s, "%d+")
来源：http://ehr.jqgfzy.top

[T40] Lua：元表
来源：http://rnd.yanxiufei.cn

setmetatable({}, { __index = base })
来源：http://fyn.xziqi.cn

[T41] Perl：Hello World
来源：http://kad.yuanzhike.top

print "Hello\n";
来源：http://zbd.nanxuanxn.top

[T42] Perl：变量类型
来源：http://cby.dianchejie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lej.yfazqb.com

[T43] Perl：字符串插值
来源：http://obn.shanyushiyangtech.top

"值: $a"
来源：http://fak.fanxiaobao.xyz

[T44] Perl：条件
来源：http://pqi.yongpay.top

if ($a > 0) { print "正"; }
来源：http://snr.jiagoushi.top

[T45] Perl：数组遍历
来源：http://zuq.shzxlz.cn

for my $x (@arr) { print $x; }
来源：http://afv.hysaishi.cn

[T46] Perl：哈希操作
来源：http://nvv.iojbl.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qan.hywenlv.cn

[T47] Perl：正则捕获
来源：http://phb.shanyushiyangtech.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zcr.yueranfly.top

[T48] Perl：正则替换
来源：http://mir.cashguo.top

$s =~ s/old/new/g;
来源：http://tvz.sjlbkw.cn

[T49] Perl：函数
来源：http://nwc.sweek.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jal.guowangkeji.top

[T50] Perl：逐行读文件
来源：http://gzv.zdbjq.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ufh.dashuyun.cn

while (my $line = <$fh>) { print $line; }
来源：http://ijg.zycfv.cn

[T51] Scala：Hello World
来源：http://ypj.jinghuilouyu.cn

println("Hello")
来源：http://bth.yvedp.cn

[T52] Scala：变量
来源：http://zqu.fehbvm.com

val a = 1;  var b = 2
来源：http://dpa.jyoumei.cn

[T53] Scala：字符串插值
来源：http://bzh.iojbl.cn

s"值: $b"
来源：http://trh.ywan-chungtsiang.top

[T54] Scala：集合映射
来源：http://qze.ivvv.top

List(1, 2, 3).map(_ * 2)
来源：http://lwq.gzhubu.top

[T55] Scala：集合过滤
来源：http://fxk.ydzc1.top

List(1, 2, 3).filter(_ > 1)
来源：http://akz.aizwys.cn

[T56] Scala：样例类
来源：http://wpj.yj20258888.top

case class User(name: String, age: Int)
来源：http://lcf.zdbjq.cn

[T57] Scala：模式匹配
来源：http://wtk.quarkkingdee.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://asr.hfpthk.cn

[T58] Scala：函数定义
来源：http://rsk.fzhhl.top

def add(a: Int, b: Int): Int = a + b
来源：http://tqy.cheryme.top

[T59] Scala：循环
来源：http://gqq.havefunace.top

for (i <- 1 to 10) println(i)
来源：http://nni.xylfe.cn

[T60] Scala：折叠
来源：http://zpb.ivvv.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tat.yj20258888.top

================================================================================
来源：http://gun.yueranfly.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xmz.jiagoushi.top

================================================================================
来源：http://rui.yj20258888.top


<!-- 参考信息 -->