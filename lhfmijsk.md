代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tfb.yanxiufei.cn

[R56] 远程拷贝
来源：http://ybv.yongpay.top

scp file user@host:/path/
来源：http://twa.daxiang520.top

[R57] 远程执行命令
来源：http://xae.zdbjq.cn

ssh user@host 'uptime'
来源：http://ydj.hesvh.cn

[R58] 下载文件
来源：http://jnz.kuanghao11.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://box.hesvh.cn

[R59] 发 POST JSON
来源：http://asi.9152youxi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qtb.cqqwz.cn

[R60] 只看 HTTP 状态码
来源：http://xjc.zhengqikj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jbt.xingfuxueyuan.xyz

[R61] 磁盘占用
来源：http://bwz.xingfuxueyuan.xyz

df -h;  du -sh *
来源：http://ztj.yonumen.top

[R62] 找最占空间的文件
来源：http://ajg.jqgfzy.top

du -ah . | sort -rh | head -10
来源：http://xyy.zhoulong.xyz

[R63] 内存与进程
来源：http://fjg.fzhhl.top

free -h;  ps aux | grep nginx
来源：http://oir.ybcxt.top

[R64] 结束进程
来源：http://qvh.jiagoushi.top

kill -9 $(pgrep -f app.py)
来源：http://hsx.zhixingplan.top

[R65] 查看端口占用
来源：http://zyi.zhaomingkeji.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cwg.chenzaomai.com

[R66] 定时任务
来源：http://yzz.yj202588.top

crontab -e;  crontab -l
来源：http://byw.gotoacloud.top

[R67] 生成随机十六进制串
来源：http://bjd.snrcjt.cn

openssl rand -hex 16
来源：http://stp.daxiang520.top

[R68] 计算文件校验值
来源：http://yrn.yuxming.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zvm.gzhubu.top

[R69] 生成随机密码
来源：http://zbr.shzxlz.cn

head -c 16 /dev/urandom | base64
来源：http://jlr.fanxiaobao.xyz

[R70] 时间戳与互转
来源：http://dal.jinyuanbaomall.cn

date +%s;  date -d @1700000000
来源：http://xed.zhoulong.xyz

[R71] 日期格式化
来源：http://wzc.zhijiandao.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lvg.yvedp.cn

[R72] 等待端口就绪
来源：http://upt.fengsongda.top

until nc -z localhost 3306; do sleep 1; done
来源：http://hds.hesvh.cn

[R73] 分割大日志
来源：http://qih.kuanghao11.cn

split -l 1000 big.log part_
来源：http://wtg.gaohongyu789.top

[R74] 批量重命名
来源：http://sbf.iojbl.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dgu.haohaochexian.top

[R75] 导出环境变量
来源：http://leu.gzhubu.top

export PATH="$HOME/bin:$PATH"
来源：http://bpz.yangfankeji.com

[R76] 使用临时文件
来源：http://ixx.tian-w.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wyy.52xcode.cn

[R77] 读取用户输入
来源：http://osy.birdmap.top

read -rp "请输入: " ans
来源：http://akx.gaohongyu789.top

[R78] 交互式菜单
来源：http://ypm.ydzc1.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ilp.redwolf501.top

[R79] 解析命令行选项
来源：http://bpa.zdbjq.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ype.chenzaomai.com

[R80] 查看脚本执行耗时
来源：http://exo.aizwys.cn

time ./run.sh
来源：http://dpj.hywenlv.cn

================================================================================
来源：http://whf.nwbrower.top

S. C / C++ 专题
来源：http://alo.fengsongda.top

================================================================================
来源：http://fbr.ydjk.org.cn

[S01] C：Hello World
来源：http://laf.tarul.cn

#include <stdio.h>
来源：http://ksb.yfazqb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://olb.mhx1999.top

[S02] C：变量与格式化输出
来源：http://yyy.yangfankeji.com

int a = 10; printf("%d\n", a);
来源：http://cxn.hongshengwenyu.top

[S03] C：读入整数
来源：http://jrb.meibo888.top

int x; scanf("%d", &x);
来源：http://lar.jinqigufen.top

[S04] C：字符串复制
来源：http://jlx.birdmap.top

char dst[32]; strcpy(dst, "hi");
来源：http://guq.tarul.cn

[S05] C：字符串长度
来源：http://rhp.jqgufenzy.top

strlen(s)
来源：http://siu.gotoacloud.top

[S06] C：字符串比较
来源：http://vgw.yongpay.top

strcmp(a, b) == 0
来源：http://rvs.meibo888.top

[S07] C：数组遍历求和
来源：http://nvd.jiagoushi.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xmi.jianghu66.top

[S08] C：动态内存分配与释放
来源：http://ccj.havefunace.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pea.jyoumei.cn

[S09] C：结构体定义与初始化
来源：http://nks.c1oappe.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://itu.ivvv.top

[S10] C：指针与解引用
来源：http://muo.chenzaomai.com

int *p = &a;  *p = 5;
来源：http://fqt.jiagoushi.top

[S11] C：逐行读文件
来源：http://ewq.fzhhl.top

FILE *f = fopen("a.txt", "r");
来源：http://joe.iojbl.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nmk.zycfv.cn

fclose(f);
来源：http://dqz.aizwys.cn

[S12] C：写文件
来源：http://fmi.mhx1999.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hhc.jinqigufen.top

[S13] C：宏定义
来源：http://uau.fzhhl.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hqr.xziqi.cn

[S14] C：枚举
来源：http://rwm.ppjwa.cn

enum Color { RED, GREEN, BLUE };
来源：http://ded.snrcjt.cn

[S15] C：类型转换
来源：http://cnh.shanyushiyangkeji.top

(double) a / b
来源：http://qhd.c1oappe.top

[S16] C：位操作置位
来源：http://obz.zhoulong.xyz

x |= (1 << 3);
来源：http://ilo.yj20258888.top

[S17] C：安全拼接字符串
来源：http://ktf.gzhubu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://huy.jiagoushi.top

[S18] C：命令行参数
来源：http://skk.yangfankeji.com

int main(int argc, char **argv)
来源：http://nxc.jlsjyb.cn

[S19] C：快速排序
来源：http://xqn.ywan-chungtsiang.top

qsort(a, n, sizeof(int), cmp);
来源：http://pnc.zycfv.cn

[S20] C：二分查找
来源：http://drx.jqgufenzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fkf.zhengqikj.top

[S21] C：字符类别判断
来源：http://xze.zhaomingkeji.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://klx.xylfe.cn

[S22] C：字符串转数字
来源：http://def.mhx1999.top

atoi("42");  strtod("3.14", NULL);
来源：http://lbw.zhaomingkeji.xyz

[S23] C：随机数
来源：http://hcm.chenlongwang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://vdw.bjfxy.top

[S24] C：获取本地时间
来源：http://aqo.bjfxy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://occ.ivvv.top

[S25] C：内存拷贝
来源：http://yol.yj20258.top

memcpy(dst, src, n);
来源：http://sny.hammf.cn

[S26] C：内存清零
来源：http://vkg.zhengqikj.top

memset(a, 0, sizeof a);
来源：http://fqm.zdqjudy.top

[S27] C：定义常量
来源：http://thm.redwolf501.top

const double PI = 3.14159;
来源：http://tiv.zhiwuduotai.top

[S28] C：静态变量
来源：http://msv.shanyushiyangkeji.top

static int counter = 0;
来源：http://ekq.fengsongda.top

[S29] C：变参函数
来源：http://lhj.jianghu66.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hun.nanxuanxn.top

[S30] C：头文件保护
来源：http://hpd.wangdashe.top

#ifndef X_H
来源：http://hwy.ehwqpu.com

#define X_H
来源：http://sdn.cheryme.top

#endif
来源：http://gei.hysaishi.cn

[S31] C++：Hello World
来源：http://dse.ybcxt.top

#include <iostream>
来源：http://ial.zhijiandao.cn

int main() { std::cout << "Hello\n"; }
来源：http://wcd.zdbjq.cn

[S32] C++：字符串
来源：http://gaw.chenlongwang.top

std::string s = "hi";  s += "!";
来源：http://xyp.cqqwz.cn

[S33] C++：vector 增删
来源：http://xlv.ybcxt.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ifb.yuanzhike.top

[S34] C++：遍历 vector
来源：http://gjd.zycfv.cn

for (auto &x : v) { std::cout << x; }
来源：http://vri.epnwcf.com

[S35] C++：map
来源：http://ali.ctjpmb.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sgf.shuidangran.top

[S36] C++：unordered_map
来源：http://syq.cheryme.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kjx.aibaodan.cn

[S37] C++：set
来源：http://jdf.sufxvd.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ggv.jianghu66.top

[S38] C++：排序
来源：http://vgu.kuanghao11.cn

std::sort(v.begin(), v.end());
来源：http://gyf.cashguo.top

[S39] C++：自定义比较器排序
来源：http://lgm.yvedp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ufu.wangshuangyany.cn

[S40] C++：查找元素
来源：http://pyl.ppjwa.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yql.fengsongda.top

[S41] C++：类与构造函数
来源：http://izy.fanxiaobao.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nss.gaohongyu789.top

[S42] C++：继承与虚函数
来源：http://igd.jianghu66.top

class B : public Base { public: void f() override {} };
来源：http://bmm.jyoumei.cn

[S43] C++：智能指针
来源：http://mcv.chenjidiqi.icu

auto p = std::make_unique<int>(5);
来源：http://zoj.fzhhl.top

[S44] C++：引用传参
来源：http://oup.chenjidiqi.icu

void inc(int &x) { ++x; }
来源：http://dbh.hnqzz.top

[S45] C++：lambda
来源：http://lgs.jiagoushi.top

auto add = [](int a, int b) { return a + b; };
来源：http://kao.fanxiaobao.xyz

[S46] C++：函数模板
来源：http://lxu.nanxuanxn.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jug.nwbrower.top

[S47] C++：结构化绑定遍历
来源：http://vyx.yuanzhike.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ywt.jinyuanbaomall.cn

[S48] C++：逐行读文件
来源：http://ufe.hesvh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yga.pycfn.com

while (std::getline(in, line)) { }
来源：http://cww.xinyue.icu

[S49] C++：写文件
来源：http://ady.kuanghao11.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lmo.xziqi.cn

[S50] C++：格式化数字
来源：http://ewk.wangdashe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://scy.gzhubu.top

[S51] C++：显式类型转换
来源：http://dmh.cashguo.top

static_cast<double>(a) / b
来源：http://way.ydzc1.top

[S52] C++：const 与 noexcept
来源：http://rub.ybcxt.top

int size() const noexcept { return n_; }
来源：http://pnn.0kj1m.cn

[S53] C++：移动语义
来源：http://nlf.zhaomingkeji.xyz

std::vector<int> w = std::move(v);
来源：http://ych.yj202588.top

[S54] C++：异常处理
来源：http://asu.pycfn.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cbb.tianlin.xyz

[S55] C++：结构化绑定
来源：http://sab.zhengqikj.top

auto [a, b] = std::make_pair(1, 2);
来源：http://dnh.zhijiandao.cn

[S56] C++：optional
来源：http://rhg.0kj1m.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jzi.tanke756.top

[S57] C++：编译期常量
来源：http://gxr.jiagoushi.top

constexpr int N = 10;
来源：http://gad.yuxming.cn

[S58] C++：命名空间
来源：http://vps.zhoulong.xyz

namespace ns { int f() { return 1; } }
来源：http://xnp.cucudq.cn

[S59] C++：静态断言
来源：http://jsx.shanyushiyangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zlp.mhx1999.top

[S60] C++：遍历并删除元素
来源：http://wtg.havefunace.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pwm.gaohongyu789.top

================================================================================
来源：http://ful.ywan-chungtsiang.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jiv.fktsv.cn

================================================================================
来源：http://pcl.cheryme.top

[T01] Kotlin：Hello World
来源：http://mrd.sweek.top

println("Hello")
来源：http://ekf.yanxiufei.cn

[T02] Kotlin：变量
来源：http://vsq.gotoacloud.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oqd.dianchejie.cn

[T03] Kotlin：字符串模板
来源：http://lsp.shanyushiyangtech.top

"值: $b"
来源：http://vgm.hongshengwenyu.top

[T04] Kotlin：空安全
来源：http://wvu.sjlbkw.cn

val n: String? = null;  n?.length
来源：http://jbt.yuanzhike.top

[T05] Kotlin：when 表达式
来源：http://lhm.shzxlz.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://onl.quarkkingdee.top

[T06] Kotlin：集合映射
来源：http://rke.zhengqikj.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zxg.hysaishi.cn

[T07] Kotlin：集合过滤
来源：http://xnm.jqgfzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mdt.haohaochexian.top

[T08] Kotlin：数据类
来源：http://swp.gzhubu.top

data class User(val name: String, val age: Int)
来源：http://esv.shzxlz.cn

[T09] Kotlin：扩展函数
来源：http://gas.xingfuxueyuan.xyz

fun String.exclaim() = this + "!"
来源：http://ysj.nanxuanxn.top

[T10] Kotlin：默认参数
来源：http://hql.xingfuxueyuan.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://qtq.nwbrower.top

[T11] Kotlin：协程
来源：http://qfq.zycfv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yrv.chenzaomai.com

[T12] Kotlin：解构声明
来源：http://dmr.zhoulong.xyz

val (a, b) = Pair(1, 2)
来源：http://jby.sxryk.cn

[T13] Kotlin：只读 Map
来源：http://nmt.zdqjudy.top

val m = mapOf("a" to 1)
来源：http://idt.hywenlv.cn

[T14] Kotlin：循环
来源：http://jhx.kuanghao11.cn

for (i in 1..10) println(i)
来源：http://fdn.yangfankeji.com

[T15] Kotlin：接口
来源：http://gkc.ppjwa.cn

interface Shape { fun area(): Double }
来源：http://lzv.haohaochexian.top

[T16] Swift：Hello World
来源：http://wjr.ppjwa.cn

print("Hello")
来源：http://gyw.dashuyun.cn

[T17] Swift：变量与常量
来源：http://gqt.gaohongyu789.top

var a = 1;  let b = 2
来源：http://wpe.havefunace.top

[T18] Swift：字符串插值
来源：http://img.zhixingplan.top

"值: \(b)"
来源：http://nhi.hesvh.cn

[T19] Swift：可选绑定
来源：http://vfx.cqqwz.cn

if let n = opt { print(n) }
来源：http://nus.ywan-chungtsiang.top

[T20] Swift：数组操作
来源：http://pub.yfazqb.com

var a = [1, 2, 3];  a.append(4)
来源：http://lsv.ivvv.top

[T21] Swift：遍历
来源：http://gzi.vehdjk.com

for x in a { print(x) }
来源：http://wml.tianlin.xyz

[T22] Swift：字典
来源：http://sce.chenlongwang.top

var d = ["a": 1];  d["b"] = 2
来源：http://umk.uphjek.com

[T23] Swift：函数
来源：http://ewl.yj20258.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fij.jinqigufen.top

[T24] Swift：闭包
来源：http://yug.zhixingplan.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://lmq.nanxinkj.top

[T25] Swift：结构体
来源：http://yru.zhongyouzk.top

struct P { var x: Int }
来源：http://vll.kuanghao11.cn

[T26] Swift：类与重写
来源：http://rie.jinqigfzy.top

class A: Base { override func f() {} }
来源：http://grq.jinqigufen.top

[T27] Swift：错误处理
来源：http://wmq.shuidangran.top

do { try f() } catch { print(error) }
来源：http://xma.sufxvd.cn

[T28] Swift：枚举
来源：http://iwq.ywan-chungtsiang.top

enum Color { case red, green }
来源：http://yaz.xziqi.cn

[T29] Swift：guard 提前返回
来源：http://vew.wangdashe.top

guard let x = opt else { return }
来源：http://fix.zdbjq.cn

[T30] Swift：协议
来源：http://ejg.nanxinkj.top

protocol Shape { func area() -> Double }
来源：http://zsu.c1oappe.top

[T31] Lua：Hello World
来源：http://lwi.chenzaomai.com

print("Hello")
来源：http://mxp.yonumen.top

[T32] Lua：局部变量
来源：http://evp.iojbl.cn

local a = 1
来源：http://xqv.zhiwuduotai.top

[T33] Lua：表（数组）
来源：http://ito.yj20258.top

local t = {1, 2, 3};  t[4] = 4
来源：http://iqz.yj20258.top

[T34] Lua：遍历表
来源：http://ugq.guannengcc.top

for i, v in ipairs(t) do print(i, v) end
来源：http://lqb.jinyuanbaomall.cn

[T35] Lua：字典表
来源：http://eez.redwolf501.top

local d = { a = 1 };  d.b = 2
来源：http://xvu.tian-w.cn

[T36] Lua：函数
来源：http://rmm.daxiang520.top

function add(a, b) return a + b end
来源：http://rwv.yfazqb.com

[T37] Lua：字符串拼接
来源：http://eqw.daxiang520.top

"a" .. "b"
来源：http://wnn.jinqigfzy.top

[T38] Lua：条件
来源：http://qnn.sufxvd.cn

if x > 0 then print("正") end
来源：http://yqt.zhoulong.xyz

[T39] Lua：模式匹配
来源：http://nko.zycfv.cn

string.find(s, "%d+")
来源：http://xir.zhongyouzk.top

[T40] Lua：元表
来源：http://ava.xylfe.cn

setmetatable({}, { __index = base })
来源：http://lxd.gzhubu.top

[T41] Perl：Hello World
来源：http://hxz.zhixingplan.top

print "Hello\n";
来源：http://tvq.meibo888.top

[T42] Perl：变量类型
来源：http://byf.gaohongyu789.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vcj.smart0.xyz

[T43] Perl：字符串插值
来源：http://ovu.316326.xyz

"值: $a"
来源：http://buj.ywan-chungtsiang.top

[T44] Perl：条件
来源：http://jyi.zhaomingkeji.xyz

if ($a > 0) { print "正"; }
来源：http://jog.52xcode.cn

[T45] Perl：数组遍历
来源：http://ymk.yuanzhike.top

for my $x (@arr) { print $x; }
来源：http://hpg.sysykeji.top

[T46] Perl：哈希操作
来源：http://zbo.jinqigfzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wjx.xinyue.icu

[T47] Perl：正则捕获
来源：http://wqg.yj20258888.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://yen.kuanghao11.cn

[T48] Perl：正则替换
来源：http://veh.ppjwa.cn

$s =~ s/old/new/g;
来源：http://btj.feifeiyinyue.top

[T49] Perl：函数
来源：http://zej.feifeiyinyue.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ywn.havefunace.top

[T50] Perl：逐行读文件
来源：http://zib.ydzc1.top

open my $fh, "<", "a.txt" or die $!;
来源：http://vdb.ppjwa.cn

while (my $line = <$fh>) { print $line; }
来源：http://pnb.ppjwa.cn

[T51] Scala：Hello World
来源：http://qlk.0kj1m.cn

println("Hello")
来源：http://wvz.cqqwz.cn

[T52] Scala：变量
来源：http://kku.bjfxy.top

val a = 1;  var b = 2
来源：http://zwe.hongshengwenyu.top

[T53] Scala：字符串插值
来源：http://afw.ctjpmb.com

s"值: $b"
来源：http://lmh.shangyingyoupin.top

[T54] Scala：集合映射
来源：http://dip.sweek.top

List(1, 2, 3).map(_ * 2)
来源：http://tjr.yj20258888.top

[T55] Scala：集合过滤
来源：http://zfx.ctjpmb.com

List(1, 2, 3).filter(_ > 1)
来源：http://bkf.pengpengdd.cyou

[T56] Scala：样例类
来源：http://cox.xziqi.cn

case class User(name: String, age: Int)
来源：http://bmd.xingfuxueyuan.xyz

[T57] Scala：模式匹配
来源：http://lhd.ywan-chungtsiang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://uyg.cashguo.top

[T58] Scala：函数定义
来源：http://ahs.hcnkem.com


<!-- 参考信息 -->