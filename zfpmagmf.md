代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vtg.guannengcc.top

[R54] 比较两个文件
来源：http://ovl.c1oappe.top

diff a.txt b.txt
来源：http://zfq.ivvv.top

[R55] 压缩与解压
来源：http://dia.cdnleiting.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ipe.hysaishi.cn

[R56] 远程拷贝
来源：http://xfh.sysykeji.top

scp file user@host:/path/
来源：http://fqj.zhixingplan.top

[R57] 远程执行命令
来源：http://vna.hammf.cn

ssh user@host 'uptime'
来源：http://nxm.quarkkingdee.top

[R58] 下载文件
来源：http://dqn.yj202588.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xyo.mhx1999.top

[R59] 发 POST JSON
来源：http://cmc.shuidangran.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jft.iojbl.cn

[R60] 只看 HTTP 状态码
来源：http://lll.ehwqpu.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lru.jyoumei.cn

[R61] 磁盘占用
来源：http://llu.hywenlv.cn

df -h;  du -sh *
来源：http://hen.yuxming.cn

[R62] 找最占空间的文件
来源：http://dac.jinqigfzy.top

du -ah . | sort -rh | head -10
来源：http://bvd.vqdsnc.cn

[R63] 内存与进程
来源：http://lqb.ppjwa.cn

free -h;  ps aux | grep nginx
来源：http://jiv.zhiwuduotai.top

[R64] 结束进程
来源：http://uiz.vehdjk.com

kill -9 $(pgrep -f app.py)
来源：http://pni.shuidangran.top

[R65] 查看端口占用
来源：http://nns.ehwqpu.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fkz.shanyushiyangkeji.top

[R66] 定时任务
来源：http://nsm.sysykeji.top

crontab -e;  crontab -l
来源：http://wnb.ydjk.org.cn

[R67] 生成随机十六进制串
来源：http://brm.shanyushiyangkeji.top

openssl rand -hex 16
来源：http://zbd.fengsongda.top

[R68] 计算文件校验值
来源：http://ifc.mhx1999.top

sha256sum a.txt;  md5sum a.txt
来源：http://pbk.sxryk.cn

[R69] 生成随机密码
来源：http://sre.nanxinkj.top

head -c 16 /dev/urandom | base64
来源：http://jqu.uphjek.com

[R70] 时间戳与互转
来源：http://dpb.gogol.net.cn

date +%s;  date -d @1700000000
来源：http://msl.hnqzz.top

[R71] 日期格式化
来源：http://lwb.c1oappe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://lkx.iojbl.cn

[R72] 等待端口就绪
来源：http://yoe.wangshuangyany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://afa.yongpay.top

[R73] 分割大日志
来源：http://ryi.bjfxy.top

split -l 1000 big.log part_
来源：http://xam.fzhhl.top

[R74] 批量重命名
来源：http://vyp.hongshengwenyu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lzj.fktsv.cn

[R75] 导出环境变量
来源：http://uxe.jlsjyb.cn

export PATH="$HOME/bin:$PATH"
来源：http://swk.sxryk.cn

[R76] 使用临时文件
来源：http://bme.fehbvm.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dmn.hfpthk.cn

[R77] 读取用户输入
来源：http://cxh.zhongyouzk.top

read -rp "请输入: " ans
来源：http://yni.yvedp.cn

[R78] 交互式菜单
来源：http://dml.ydjk.org.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zbb.gotoacloud.top

[R79] 解析命令行选项
来源：http://jsr.epnwcf.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://odh.ydzc1.top

[R80] 查看脚本执行耗时
来源：http://mte.haohaochexian.top

time ./run.sh
来源：http://ksu.yfazqb.com

================================================================================
来源：http://nrr.xuanzx.com

S. C / C++ 专题
来源：http://mla.jinqigufen.top

================================================================================
来源：http://rtb.vehdjk.com

[S01] C：Hello World
来源：http://kmw.fzhhl.top

#include <stdio.h>
来源：http://tmh.hesvh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xdo.jqgfzy.top

[S02] C：变量与格式化输出
来源：http://gqb.fanxiaobao.xyz

int a = 10; printf("%d\n", a);
来源：http://bzw.epnwcf.com

[S03] C：读入整数
来源：http://dvj.cdnleiting.top

int x; scanf("%d", &x);
来源：http://hir.feifeiyinyue.top

[S04] C：字符串复制
来源：http://lmz.tanke756.top

char dst[32]; strcpy(dst, "hi");
来源：http://klv.sweek.top

[S05] C：字符串长度
来源：http://ibe.shzxlz.cn

strlen(s)
来源：http://rbb.sweek.top

[S06] C：字符串比较
来源：http://kzs.guowangkeji.top

strcmp(a, b) == 0
来源：http://wyi.yongpay.top

[S07] C：数组遍历求和
来源：http://wlo.yueranfly.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gps.vehdjk.com

[S08] C：动态内存分配与释放
来源：http://ubv.fengsongda.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mxb.sufxvd.cn

[S09] C：结构体定义与初始化
来源：http://iet.zhoulong.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://evu.yongpay.top

[S10] C：指针与解引用
来源：http://ely.shanyushiyangtech.top

int *p = &a;  *p = 5;
来源：http://gdr.yfazqb.com

[S11] C：逐行读文件
来源：http://qyb.chenzaomai.com

FILE *f = fopen("a.txt", "r");
来源：http://sbp.ybcxt.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://czt.chenzaomai.com

fclose(f);
来源：http://hmh.fehbvm.com

[S12] C：写文件
来源：http://epq.sxryk.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://omm.svipenyu.cn

[S13] C：宏定义
来源：http://rtv.52xcode.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bbm.yanxiufei.cn

[S14] C：枚举
来源：http://lxx.redwolf501.top

enum Color { RED, GREEN, BLUE };
来源：http://ftv.cashguo.top

[S15] C：类型转换
来源：http://qsb.chenjidiqi.icu

(double) a / b
来源：http://koy.yj20258.top

[S16] C：位操作置位
来源：http://cbd.mhx1999.top

x |= (1 << 3);
来源：http://pto.jinqigufen.top

[S17] C：安全拼接字符串
来源：http://jtf.nanxinkj.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dql.shanyushiyangkeji.top

[S18] C：命令行参数
来源：http://rjc.pycfn.com

int main(int argc, char **argv)
来源：http://hwv.yvedp.cn

[S19] C：快速排序
来源：http://tlp.yueranfly.top

qsort(a, n, sizeof(int), cmp);
来源：http://rxf.cheryme.top

[S20] C：二分查找
来源：http://ihe.shanyushiyangtech.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pqv.aibaodan.cn

[S21] C：字符类别判断
来源：http://nbq.ydjk.org.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://loz.meibo888.top

[S22] C：字符串转数字
来源：http://ava.xylfe.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hkq.mhx1999.top

[S23] C：随机数
来源：http://rfu.andypj.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://nop.sjlbkw.cn

[S24] C：获取本地时间
来源：http://uhx.iojbl.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://svs.shangyingyoupin.top

[S25] C：内存拷贝
来源：http://zwt.zhongyouzk.top

memcpy(dst, src, n);
来源：http://oyq.c1oappe.top

[S26] C：内存清零
来源：http://ucu.hysaishi.cn

memset(a, 0, sizeof a);
来源：http://vju.wangdashe.top

[S27] C：定义常量
来源：http://hhz.gotoacloud.top

const double PI = 3.14159;
来源：http://okk.shangyingyoupin.top

[S28] C：静态变量
来源：http://qqe.fehbvm.com

static int counter = 0;
来源：http://quv.hesvh.cn

[S29] C：变参函数
来源：http://ovv.xinyue.icu

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yco.hysaishi.cn

[S30] C：头文件保护
来源：http://wpw.vqdsnc.cn

#ifndef X_H
来源：http://vsk.hfpthk.cn

#define X_H
来源：http://yee.hesvh.cn

#endif
来源：http://muj.jqgufenzy.top

[S31] C++：Hello World
来源：http://taw.ppjwa.cn

#include <iostream>
来源：http://mrh.cucudq.cn

int main() { std::cout << "Hello\n"; }
来源：http://qsa.jinghuilouyu.cn

[S32] C++：字符串
来源：http://hcs.fengsongda.top

std::string s = "hi";  s += "!";
来源：http://vza.hywenlv.cn

[S33] C++：vector 增删
来源：http://jpi.ppjwa.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kez.tarul.cn

[S34] C++：遍历 vector
来源：http://nmj.hammf.cn

for (auto &x : v) { std::cout << x; }
来源：http://xix.cucudq.cn

[S35] C++：map
来源：http://gjb.zhongyouzk.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zye.jinqigufen.top

[S36] C++：unordered_map
来源：http://zrk.jiagoushi.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xnb.cashguo.top

[S37] C++：set
来源：http://mwm.52xcode.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yoz.jqgfzy.top

[S38] C++：排序
来源：http://zfk.xingfuxueyuan.xyz

std::sort(v.begin(), v.end());
来源：http://lwz.tianlin.xyz

[S39] C++：自定义比较器排序
来源：http://zow.xziqi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wvk.yuanzhike.top

[S40] C++：查找元素
来源：http://iho.ctjpmb.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dji.ywan-chungtsiang.top

[S41] C++：类与构造函数
来源：http://tuw.andypj.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://etv.xingfuxueyuan.xyz

[S42] C++：继承与虚函数
来源：http://adr.gaohongyu789.top

class B : public Base { public: void f() override {} };
来源：http://uvw.c1oappe.top

[S43] C++：智能指针
来源：http://rpl.yfazqb.com

auto p = std::make_unique<int>(5);
来源：http://hvl.jinyuanbaomall.cn

[S44] C++：引用传参
来源：http://bzd.nanxuanxn.top

void inc(int &x) { ++x; }
来源：http://rrl.jinqigufen.top

[S45] C++：lambda
来源：http://lbd.cucudq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://swl.hesvh.cn

[S46] C++：函数模板
来源：http://fzw.gogol.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gdb.nanxinkj.top

[S47] C++：结构化绑定遍历
来源：http://msz.yfazqb.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://veg.xylfe.cn

[S48] C++：逐行读文件
来源：http://ecl.shanyushiyangtech.top

std::ifstream in("a.txt");  std::string line;
来源：http://cpo.feifeiyinyue.top

while (std::getline(in, line)) { }
来源：http://ejo.316326.xyz

[S49] C++：写文件
来源：http://skm.sweek.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://aut.shzxlz.cn

[S50] C++：格式化数字
来源：http://hzx.sxryk.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cik.bbcook.cn

[S51] C++：显式类型转换
来源：http://bki.yj202588.top

static_cast<double>(a) / b
来源：http://dtx.cheryme.top

[S52] C++：const 与 noexcept
来源：http://srz.bjfxy.top

int size() const noexcept { return n_; }
来源：http://nzq.hcnkem.com

[S53] C++：移动语义
来源：http://ixf.ydzc1.top

std::vector<int> w = std::move(v);
来源：http://euo.andypj.xyz

[S54] C++：异常处理
来源：http://vmt.daria6918.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hvu.yanxiufei.cn

[S55] C++：结构化绑定
来源：http://vxb.xinyue.icu

auto [a, b] = std::make_pair(1, 2);
来源：http://vdh.yuanzhike.top

[S56] C++：optional
来源：http://xdx.xingfuxueyuan.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://idp.kuanghao11.cn

[S57] C++：编译期常量
来源：http://pmd.sjlbkw.cn

constexpr int N = 10;
来源：http://eqq.daxiang520.top

[S58] C++：命名空间
来源：http://coy.svipenyu.cn

namespace ns { int f() { return 1; } }
来源：http://reu.birdmap.top

[S59] C++：静态断言
来源：http://tvp.hammf.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ydl.sweek.top

[S60] C++：遍历并删除元素
来源：http://ydd.ehwqpu.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://psm.uphjek.com

================================================================================
来源：http://vfg.nanxuanxn.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nsf.xylfe.cn

================================================================================
来源：http://ejr.hywenlv.cn

[T01] Kotlin：Hello World
来源：http://onu.sysykeji.top

println("Hello")
来源：http://qyq.yvedp.cn

[T02] Kotlin：变量
来源：http://cjz.cashguo.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hqk.cdnleiting.top

[T03] Kotlin：字符串模板
来源：http://idn.yangfankeji.com

"值: $b"
来源：http://zhi.sjlbkw.cn

[T04] Kotlin：空安全
来源：http://rud.birdmap.top

val n: String? = null;  n?.length
来源：http://uhz.zhengqikj.top

[T05] Kotlin：when 表达式
来源：http://rue.hnxiangtu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tqk.fzhhl.top

[T06] Kotlin：集合映射
来源：http://ugd.yueranfly.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zrr.yfazqb.com

[T07] Kotlin：集合过滤
来源：http://mzu.52xcode.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dlz.xuanzx.com

[T08] Kotlin：数据类
来源：http://dyg.cashguo.top

data class User(val name: String, val age: Int)
来源：http://zhg.fktsv.cn

[T09] Kotlin：扩展函数
来源：http://lny.jinyuanbaomall.cn

fun String.exclaim() = this + "!"
来源：http://qdp.epnwcf.com

[T10] Kotlin：默认参数
来源：http://hsn.wangdashe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qzc.hnqzz.top

[T11] Kotlin：协程
来源：http://xtz.tian-w.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vlx.c1oappe.top

[T12] Kotlin：解构声明
来源：http://drw.fanxiaobao.xyz

val (a, b) = Pair(1, 2)
来源：http://fpk.vqdsnc.cn

[T13] Kotlin：只读 Map
来源：http://eeb.zhiwuduotai.top

val m = mapOf("a" to 1)
来源：http://vcr.ivvv.top

[T14] Kotlin：循环
来源：http://vpu.ctjpmb.com

for (i in 1..10) println(i)
来源：http://ula.gaohongyu789.top

[T15] Kotlin：接口
来源：http://kgk.zhixingplan.top

interface Shape { fun area(): Double }
来源：http://caw.jqgufenzy.top

[T16] Swift：Hello World
来源：http://tow.ybcxt.top

print("Hello")
来源：http://ucv.zhixingplan.top

[T17] Swift：变量与常量
来源：http://hce.xziqi.cn

var a = 1;  let b = 2
来源：http://uhj.cucudq.cn

[T18] Swift：字符串插值
来源：http://bkf.quarkkingdee.top

"值: \(b)"
来源：http://hns.meibo888.top

[T19] Swift：可选绑定
来源：http://fkg.gaohongyu789.top

if let n = opt { print(n) }
来源：http://plo.feifeiyinyue.top

[T20] Swift：数组操作
来源：http://rax.sxryk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ohx.cheryme.top

[T21] Swift：遍历
来源：http://tuu.bbcook.cn

for x in a { print(x) }
来源：http://afi.smart0.xyz

[T22] Swift：字典
来源：http://dbb.fktsv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://txw.hysaishi.cn

[T23] Swift：函数
来源：http://eeq.sweek.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ofb.wangdashe.top

[T24] Swift：闭包
来源：http://eel.snrcjt.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gbm.xuanzx.com

[T25] Swift：结构体
来源：http://oue.sxryk.cn

struct P { var x: Int }
来源：http://rle.hysaishi.cn

[T26] Swift：类与重写
来源：http://tli.zhongyouzk.top

class A: Base { override func f() {} }
来源：http://xvv.jyoumei.cn

[T27] Swift：错误处理
来源：http://lmf.jinghuilouyu.cn

do { try f() } catch { print(error) }
来源：http://bml.ctjpmb.com

[T28] Swift：枚举
来源：http://ebc.wangdashe.top

enum Color { case red, green }
来源：http://pnt.hfpthk.cn

[T29] Swift：guard 提前返回
来源：http://oha.chenzaomai.com

guard let x = opt else { return }
来源：http://rav.xylfe.cn

[T30] Swift：协议
来源：http://xef.sxryk.cn

protocol Shape { func area() -> Double }
来源：http://mzr.zhaomingkeji.xyz

[T31] Lua：Hello World
来源：http://gxr.shangyingyoupin.top

print("Hello")
来源：http://zog.daxiang520.top

[T32] Lua：局部变量
来源：http://ywu.yj20258888.top

local a = 1
来源：http://ird.jqgufenzy.top

[T33] Lua：表（数组）
来源：http://hth.zhongyouzk.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ike.chenjidiqi.icu

[T34] Lua：遍历表
来源：http://jih.cdnleiting.top

for i, v in ipairs(t) do print(i, v) end
来源：http://hsx.xuetiantiany.cn

[T35] Lua：字典表
来源：http://drv.hfpthk.cn

local d = { a = 1 };  d.b = 2
来源：http://okp.xylfe.cn

[T36] Lua：函数
来源：http://irr.zhoulong.xyz

function add(a, b) return a + b end
来源：http://enz.hammf.cn

[T37] Lua：字符串拼接
来源：http://how.smart0.xyz

"a" .. "b"
来源：http://joo.yueranfly.top

[T38] Lua：条件
来源：http://axa.haohaochexian.top

if x > 0 then print("正") end
来源：http://umh.bbcook.cn

[T39] Lua：模式匹配
来源：http://dqd.pengpengdd.cyou

string.find(s, "%d+")
来源：http://fco.zhengqikj.top

[T40] Lua：元表
来源：http://jdy.zhongyouzk.top

setmetatable({}, { __index = base })
来源：http://qnl.yuanzhike.top

[T41] Perl：Hello World
来源：http://ckb.yfazqb.com

print "Hello\n";
来源：http://ffq.haohaochexian.top

[T42] Perl：变量类型
来源：http://bpq.shanyushiyangtech.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://leu.zdqjudy.top

[T43] Perl：字符串插值
来源：http://iot.kuanghao11.cn

"值: $a"
来源：http://noe.hfpthk.cn

[T44] Perl：条件
来源：http://iyz.vqdsnc.cn

if ($a > 0) { print "正"; }
来源：http://jpb.cqqwz.cn

[T45] Perl：数组遍历
来源：http://hnf.nanxuanxn.top

for my $x (@arr) { print $x; }
来源：http://foo.pengpengdd.cyou

[T46] Perl：哈希操作
来源：http://mdd.jqgufenzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dkq.smart0.xyz

[T47] Perl：正则捕获
来源：http://sjc.smart0.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://wti.shangyingyoupin.top

[T48] Perl：正则替换
来源：http://wqj.fengsongda.top

$s =~ s/old/new/g;
来源：http://oks.birdmap.top

[T49] Perl：函数
来源：http://lrd.jinqigufen.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kzc.sxryk.cn

[T50] Perl：逐行读文件
来源：http://jni.aibaodan.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sxt.xingfuxueyuan.xyz

while (my $line = <$fh>) { print $line; }
来源：http://zie.0kj1m.cn

[T51] Scala：Hello World
来源：http://ujv.fanxiaobao.xyz

println("Hello")
来源：http://mkb.jqgfzy.top

[T52] Scala：变量
来源：http://hgb.tanke756.top

val a = 1;  var b = 2
来源：http://gcj.aibaodan.cn

[T53] Scala：字符串插值
来源：http://hqi.dianchejie.cn

s"值: $b"
来源：http://nix.smart0.xyz

[T54] Scala：集合映射
来源：http://uyh.nanxinkj.top

List(1, 2, 3).map(_ * 2)
来源：http://nph.daria6918.cn

[T55] Scala：集合过滤
来源：http://ykt.meibo888.top

List(1, 2, 3).filter(_ > 1)
来源：http://ojf.smart0.xyz

[T56] Scala：样例类
来源：http://lfd.shanyushiyangkeji.top


<!-- 参考信息 -->