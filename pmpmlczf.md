代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://ywe.sufxvd.cn

[R52] 统计行数
来源：http://smh.meibo888.top

wc -l a.txt
来源：http://hgl.daxiang520.top

[R53] 查看文件头与实时尾
来源：http://wjf.bjfxy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uzj.c1oappe.top

[R54] 比较两个文件
来源：http://ipi.sjlbkw.cn

diff a.txt b.txt
来源：http://zar.zhongyouzk.top

[R55] 压缩与解压
来源：http://ujp.hnxiangtu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://abk.jianghu66.top

[R56] 远程拷贝
来源：http://yja.gzhubu.top

scp file user@host:/path/
来源：http://hjo.bbcook.cn

[R57] 远程执行命令
来源：http://ywz.birdmap.top

ssh user@host 'uptime'
来源：http://xvo.shangyingyoupin.top

[R58] 下载文件
来源：http://oxa.cdnleiting.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mxa.dashuyun.cn

[R59] 发 POST JSON
来源：http://ywb.sufxvd.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kqs.yangfankeji.com

[R60] 只看 HTTP 状态码
来源：http://bgy.yanxiufei.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://akw.fanxiaobao.xyz

[R61] 磁盘占用
来源：http://pss.gaohongyu789.top

df -h;  du -sh *
来源：http://qgi.wangdashe.top

[R62] 找最占空间的文件
来源：http://qfa.ywan-chungtsiang.top

du -ah . | sort -rh | head -10
来源：http://qzk.ybcxt.top

[R63] 内存与进程
来源：http://bhs.sweek.top

free -h;  ps aux | grep nginx
来源：http://ljn.jianghu66.top

[R64] 结束进程
来源：http://kfo.shanyushiyangtech.top

kill -9 $(pgrep -f app.py)
来源：http://ngg.hfpthk.cn

[R65] 查看端口占用
来源：http://tjg.xuanzx.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ips.ctjpmb.com

[R66] 定时任务
来源：http://xnf.jinyuanbaomall.cn

crontab -e;  crontab -l
来源：http://gyo.fktsv.cn

[R67] 生成随机十六进制串
来源：http://esx.aibaodan.cn

openssl rand -hex 16
来源：http://knn.ybcxt.top

[R68] 计算文件校验值
来源：http://woe.52xcode.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lrc.c1oappe.top

[R69] 生成随机密码
来源：http://rat.redwolf501.top

head -c 16 /dev/urandom | base64
来源：http://yvp.shanyushiyangkeji.top

[R70] 时间戳与互转
来源：http://mxh.yj202588.top

date +%s;  date -d @1700000000
来源：http://ayu.aizwys.cn

[R71] 日期格式化
来源：http://ury.hfpthk.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qqy.ehwqpu.com

[R72] 等待端口就绪
来源：http://grv.shanyushiyangkeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ybr.aibaodan.cn

[R73] 分割大日志
来源：http://lvr.snrcjt.cn

split -l 1000 big.log part_
来源：http://tqt.fengsongda.top

[R74] 批量重命名
来源：http://bdj.yj20258.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nkl.zhoulong.xyz

[R75] 导出环境变量
来源：http://fln.hnxiangtu.top

export PATH="$HOME/bin:$PATH"
来源：http://ybg.ivvv.top

[R76] 使用临时文件
来源：http://ndn.cheryme.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wtk.zycfv.cn

[R77] 读取用户输入
来源：http://lez.tian-w.cn

read -rp "请输入: " ans
来源：http://yah.c1oappe.top

[R78] 交互式菜单
来源：http://pkn.yuanzhike.top

select opt in a b c; do echo "$opt"; break; done
来源：http://pmn.316326.xyz

[R79] 解析命令行选项
来源：http://oys.52xcode.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nee.cashguo.top

[R80] 查看脚本执行耗时
来源：http://mlc.0kj1m.cn

time ./run.sh
来源：http://hvi.yanxiufei.cn

================================================================================
来源：http://nlz.hfpthk.cn

S. C / C++ 专题
来源：http://jiq.0kj1m.cn

================================================================================
来源：http://qrn.shanyushiyangkeji.top

[S01] C：Hello World
来源：http://bmr.fzhhl.top

#include <stdio.h>
来源：http://xyw.daria6918.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cul.ydjk.org.cn

[S02] C：变量与格式化输出
来源：http://mpo.wangshuangyany.cn

int a = 10; printf("%d\n", a);
来源：http://kip.ppjwa.cn

[S03] C：读入整数
来源：http://bbm.andypj.xyz

int x; scanf("%d", &x);
来源：http://kyd.cdnleiting.top

[S04] C：字符串复制
来源：http://xmh.birdmap.top

char dst[32]; strcpy(dst, "hi");
来源：http://icw.shanyushiyangkeji.top

[S05] C：字符串长度
来源：http://xhq.9152youxi.cn

strlen(s)
来源：http://wua.yuxming.cn

[S06] C：字符串比较
来源：http://pjd.jinqigufen.top

strcmp(a, b) == 0
来源：http://tqu.hywenlv.cn

[S07] C：数组遍历求和
来源：http://feb.shanyushiyangtech.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nty.xziqi.cn

[S08] C：动态内存分配与释放
来源：http://yyr.hcnkem.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://smi.smart0.xyz

[S09] C：结构体定义与初始化
来源：http://xdn.ppjwa.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vgu.zhiwuduotai.top

[S10] C：指针与解引用
来源：http://jzj.uphjek.com

int *p = &a;  *p = 5;
来源：http://ulh.jinqigfzy.top

[S11] C：逐行读文件
来源：http://loy.fzhhl.top

FILE *f = fopen("a.txt", "r");
来源：http://aov.xylfe.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ghk.hywenlv.cn

fclose(f);
来源：http://ijd.nanxuanxn.top

[S12] C：写文件
来源：http://vdj.bbcook.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zop.vqdsnc.cn

[S13] C：宏定义
来源：http://nfj.cucudq.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dza.sjlbkw.cn

[S14] C：枚举
来源：http://bhc.kuanghao11.cn

enum Color { RED, GREEN, BLUE };
来源：http://bpj.quarkkingdee.top

[S15] C：类型转换
来源：http://nqu.zycfv.cn

(double) a / b
来源：http://vie.yuanzhike.top

[S16] C：位操作置位
来源：http://spi.yj20258.top

x |= (1 << 3);
来源：http://oxf.nanxuanxn.top

[S17] C：安全拼接字符串
来源：http://cty.hfpthk.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://upn.zhixingplan.top

[S18] C：命令行参数
来源：http://qoh.sxryk.cn

int main(int argc, char **argv)
来源：http://ila.nanxuanxn.top

[S19] C：快速排序
来源：http://thz.zhiwuduotai.top

qsort(a, n, sizeof(int), cmp);
来源：http://wpd.cashguo.top

[S20] C：二分查找
来源：http://jzj.ywan-chungtsiang.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tfl.shzxlz.cn

[S21] C：字符类别判断
来源：http://xrd.cucudq.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://brh.ydzc1.top

[S22] C：字符串转数字
来源：http://ipe.uphjek.com

atoi("42");  strtod("3.14", NULL);
来源：http://rll.zhiwuduotai.top

[S23] C：随机数
来源：http://sah.yangfankeji.com

srand(time(NULL));  int r = rand() % 100;
来源：http://zuw.vehdjk.com

[S24] C：获取本地时间
来源：http://hsu.hnqzz.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lpj.yvedp.cn

[S25] C：内存拷贝
来源：http://nmn.ybcxt.top

memcpy(dst, src, n);
来源：http://jub.yongpay.top

[S26] C：内存清零
来源：http://ctt.uphjek.com

memset(a, 0, sizeof a);
来源：http://iue.zdqjudy.top

[S27] C：定义常量
来源：http://qbf.bjfxy.top

const double PI = 3.14159;
来源：http://xdy.wangshuangyany.cn

[S28] C：静态变量
来源：http://ohj.wangshuangyany.cn

static int counter = 0;
来源：http://voi.c1oappe.top

[S29] C：变参函数
来源：http://aqa.zycfv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dhd.smart0.xyz

[S30] C：头文件保护
来源：http://syp.cashguo.top

#ifndef X_H
来源：http://bud.vehdjk.com

#define X_H
来源：http://txl.daxiang520.top

#endif
来源：http://mkf.gaohongyu789.top

[S31] C++：Hello World
来源：http://pvd.yuanzhike.top

#include <iostream>
来源：http://eal.svipenyu.cn

int main() { std::cout << "Hello\n"; }
来源：http://ejn.0kj1m.cn

[S32] C++：字符串
来源：http://uvq.hysaishi.cn

std::string s = "hi";  s += "!";
来源：http://irr.sysykeji.top

[S33] C++：vector 增删
来源：http://zds.ehwqpu.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bae.tanke756.top

[S34] C++：遍历 vector
来源：http://qzz.nwbrower.top

for (auto &x : v) { std::cout << x; }
来源：http://naq.ppjwa.cn

[S35] C++：map
来源：http://qgw.ybcxt.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zdf.jyoumei.cn

[S36] C++：unordered_map
来源：http://cwk.gaohongyu789.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ajz.kuanghao11.cn

[S37] C++：set
来源：http://dyk.aizwys.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mso.jqgfzy.top

[S38] C++：排序
来源：http://byx.nwbrower.top

std::sort(v.begin(), v.end());
来源：http://ilx.hnxiangtu.top

[S39] C++：自定义比较器排序
来源：http://iwq.zhaomingkeji.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cdv.cucudq.cn

[S40] C++：查找元素
来源：http://jta.vqdsnc.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qmr.hnxiangtu.top

[S41] C++：类与构造函数
来源：http://geu.wangdashe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://egc.fzhhl.top

[S42] C++：继承与虚函数
来源：http://ikn.pycfn.com

class B : public Base { public: void f() override {} };
来源：http://ytz.tarul.cn

[S43] C++：智能指针
来源：http://dre.vqdsnc.cn

auto p = std::make_unique<int>(5);
来源：http://fqj.yangfankeji.com

[S44] C++：引用传参
来源：http://bnd.shanyushiyangkeji.top

void inc(int &x) { ++x; }
来源：http://lib.ivvv.top

[S45] C++：lambda
来源：http://kxm.yfazqb.com

auto add = [](int a, int b) { return a + b; };
来源：http://twn.sufxvd.cn

[S46] C++：函数模板
来源：http://ebi.zdbjq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zch.daria6918.cn

[S47] C++：结构化绑定遍历
来源：http://ufn.xylfe.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oet.sxryk.cn

[S48] C++：逐行读文件
来源：http://hrj.pycfn.com

std::ifstream in("a.txt");  std::string line;
来源：http://qpe.dashuyun.cn

while (std::getline(in, line)) { }
来源：http://olb.316326.xyz

[S49] C++：写文件
来源：http://emj.zhiwuduotai.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bpy.snrcjt.cn

[S50] C++：格式化数字
来源：http://rgl.zhoulong.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://acb.yanxiufei.cn

[S51] C++：显式类型转换
来源：http://sdv.fengsongda.top

static_cast<double>(a) / b
来源：http://ivn.nanxinkj.top

[S52] C++：const 与 noexcept
来源：http://iym.xziqi.cn

int size() const noexcept { return n_; }
来源：http://qdy.jqgfzy.top

[S53] C++：移动语义
来源：http://wxs.c1oappe.top

std::vector<int> w = std::move(v);
来源：http://whx.xziqi.cn

[S54] C++：异常处理
来源：http://fpk.nanxuanxn.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zwv.jqgufenzy.top

[S55] C++：结构化绑定
来源：http://dht.yueranfly.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lna.guannengcc.top

[S56] C++：optional
来源：http://nws.daria6918.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sny.ydzc1.top

[S57] C++：编译期常量
来源：http://ekp.daria6918.cn

constexpr int N = 10;
来源：http://htq.jiagoushi.top

[S58] C++：命名空间
来源：http://jnu.svipenyu.cn

namespace ns { int f() { return 1; } }
来源：http://udr.feifeiyinyue.top

[S59] C++：静态断言
来源：http://gwi.tianlin.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hwv.sysykeji.top

[S60] C++：遍历并删除元素
来源：http://wjy.xuetiantiany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bas.snrcjt.cn

================================================================================
来源：http://uzk.bjfxy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tem.cqqwz.cn

================================================================================
来源：http://fes.shanyushiyangtech.top

[T01] Kotlin：Hello World
来源：http://vno.chenjidiqi.icu

println("Hello")
来源：http://cma.aibaodan.cn

[T02] Kotlin：变量
来源：http://vvj.zhixingplan.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fqe.cashguo.top

[T03] Kotlin：字符串模板
来源：http://ruh.nwbrower.top

"值: $b"
来源：http://bfq.gotoacloud.top

[T04] Kotlin：空安全
来源：http://jae.yfazqb.com

val n: String? = null;  n?.length
来源：http://icr.jiagoushi.top

[T05] Kotlin：when 表达式
来源：http://awu.jinyuanbaomall.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dei.jinyuanbaomall.cn

[T06] Kotlin：集合映射
来源：http://cqm.daria6918.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://geu.dashuyun.cn

[T07] Kotlin：集合过滤
来源：http://uyl.nwbrower.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://fcu.zhongyouzk.top

[T08] Kotlin：数据类
来源：http://xcw.aizwys.cn

data class User(val name: String, val age: Int)
来源：http://mck.shanyushiyangkeji.top

[T09] Kotlin：扩展函数
来源：http://cpr.dianchejie.cn

fun String.exclaim() = this + "!"
来源：http://nlf.zhoulong.xyz

[T10] Kotlin：默认参数
来源：http://ael.birdmap.top

fun greet(name: String = "World") = "Hi $name"
来源：http://oyv.kuanghao11.cn

[T11] Kotlin：协程
来源：http://cfg.hnxiangtu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://hyr.hesvh.cn

[T12] Kotlin：解构声明
来源：http://spl.shanyushiyangkeji.top

val (a, b) = Pair(1, 2)
来源：http://jxl.ivvv.top

[T13] Kotlin：只读 Map
来源：http://zws.guannengcc.top

val m = mapOf("a" to 1)
来源：http://hsd.zdbjq.cn

[T14] Kotlin：循环
来源：http://nbo.cdnleiting.top

for (i in 1..10) println(i)
来源：http://akk.yj20258.top

[T15] Kotlin：接口
来源：http://wij.zhengqikj.top

interface Shape { fun area(): Double }
来源：http://akq.ctjpmb.com

[T16] Swift：Hello World
来源：http://smh.hcnkem.com

print("Hello")
来源：http://igv.hnqzz.top

[T17] Swift：变量与常量
来源：http://jue.yvedp.cn

var a = 1;  let b = 2
来源：http://ass.haohaochexian.top

[T18] Swift：字符串插值
来源：http://jsz.ybcxt.top

"值: \(b)"
来源：http://ubj.shanyushiyangtech.top

[T19] Swift：可选绑定
来源：http://hml.cucudq.cn

if let n = opt { print(n) }
来源：http://xgw.0kj1m.cn

[T20] Swift：数组操作
来源：http://uvj.fktsv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jxi.jiagoushi.top

[T21] Swift：遍历
来源：http://nqn.yanxiufei.cn

for x in a { print(x) }
来源：http://nai.yfazqb.com

[T22] Swift：字典
来源：http://sbs.jqgufenzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://jkz.ivvv.top

[T23] Swift：函数
来源：http://rqm.meibo888.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jyj.hongshengwenyu.top

[T24] Swift：闭包
来源：http://apy.hfpthk.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wwd.zdbjq.cn

[T25] Swift：结构体
来源：http://ava.cdnleiting.top

struct P { var x: Int }
来源：http://aro.vqdsnc.cn

[T26] Swift：类与重写
来源：http://wig.chenzaomai.com

class A: Base { override func f() {} }
来源：http://oiq.smart0.xyz

[T27] Swift：错误处理
来源：http://vfr.0kj1m.cn

do { try f() } catch { print(error) }
来源：http://pmj.feifeiyinyue.top

[T28] Swift：枚举
来源：http://agi.tanke756.top

enum Color { case red, green }
来源：http://gxe.chenzaomai.com

[T29] Swift：guard 提前返回
来源：http://dkt.fktsv.cn

guard let x = opt else { return }
来源：http://leu.nanxinkj.top

[T30] Swift：协议
来源：http://sgx.yj202588.top

protocol Shape { func area() -> Double }
来源：http://vmd.chenzaomai.com

[T31] Lua：Hello World
来源：http://ype.andypj.xyz

print("Hello")
来源：http://lws.shzxlz.cn

[T32] Lua：局部变量
来源：http://mme.yangfankeji.com

local a = 1
来源：http://wmt.gotoacloud.top

[T33] Lua：表（数组）
来源：http://bdv.52xcode.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mdf.cqqwz.cn

[T34] Lua：遍历表
来源：http://xaq.tarul.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ubx.shuidangran.top

[T35] Lua：字典表
来源：http://tpy.jinghuilouyu.cn

local d = { a = 1 };  d.b = 2
来源：http://urk.hcnkem.com

[T36] Lua：函数
来源：http://pjx.yuxming.cn

function add(a, b) return a + b end
来源：http://hxy.jlsjyb.cn

[T37] Lua：字符串拼接
来源：http://ezy.yonumen.top

"a" .. "b"
来源：http://qdn.wangshuangyany.cn

[T38] Lua：条件
来源：http://xlm.zhongyouzk.top

if x > 0 then print("正") end
来源：http://iuw.fanxiaobao.xyz

[T39] Lua：模式匹配
来源：http://zgk.hongshengwenyu.top

string.find(s, "%d+")
来源：http://jcx.zycfv.cn

[T40] Lua：元表
来源：http://dhs.yj20258888.top

setmetatable({}, { __index = base })
来源：http://hyv.sysykeji.top

[T41] Perl：Hello World
来源：http://onh.yj202588.top

print "Hello\n";
来源：http://hyz.hnxiangtu.top

[T42] Perl：变量类型
来源：http://zki.yuanzhike.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://shn.cheryme.top

[T43] Perl：字符串插值
来源：http://ycg.yongpay.top

"值: $a"
来源：http://qvq.jlsjyb.cn

[T44] Perl：条件
来源：http://epw.shuidangran.top

if ($a > 0) { print "正"; }
来源：http://omi.wangshuangyany.cn

[T45] Perl：数组遍历
来源：http://itt.tian-w.cn

for my $x (@arr) { print $x; }
来源：http://wfl.yongpay.top

[T46] Perl：哈希操作
来源：http://znp.nwbrower.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cur.xuetiantiany.cn

[T47] Perl：正则捕获
来源：http://per.yanxiufei.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tqk.jianghu66.top

[T48] Perl：正则替换
来源：http://etd.dashuyun.cn

$s =~ s/old/new/g;
来源：http://kls.tarul.cn

[T49] Perl：函数
来源：http://riq.cheryme.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tqk.tarul.cn

[T50] Perl：逐行读文件
来源：http://xxy.ppjwa.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bob.zhijiandao.cn

while (my $line = <$fh>) { print $line; }
来源：http://adb.yj20258.top

[T51] Scala：Hello World
来源：http://olm.sysykeji.top

println("Hello")
来源：http://mcz.nanxinkj.top

[T52] Scala：变量
来源：http://bkd.gotoacloud.top

val a = 1;  var b = 2
来源：http://ngs.bjfxy.top

[T53] Scala：字符串插值
来源：http://cwf.yuxming.cn

s"值: $b"
来源：http://ujn.xingfuxueyuan.xyz

[T54] Scala：集合映射
来源：http://rmw.ppjwa.cn


<!-- 参考信息 -->