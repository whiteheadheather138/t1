代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qsa.dianchejie.cn

[R50] awk 求和
来源：http://lli.ydjk.org.cn

awk '{s += $2} END {print s}' a.txt
来源：http://skn.hfpthk.cn

[R51] 排序去重取前几
来源：http://psr.gaohongyu789.top

sort a.txt | uniq -c | sort -rn | head
来源：http://bne.c1oappe.top

[R52] 统计行数
来源：http://ebc.xinyue.icu

wc -l a.txt
来源：http://tww.hnqzz.top

[R53] 查看文件头与实时尾
来源：http://hec.fengsongda.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mnf.0kj1m.cn

[R54] 比较两个文件
来源：http://bog.ywan-chungtsiang.top

diff a.txt b.txt
来源：http://qmp.nanxinkj.top

[R55] 压缩与解压
来源：http://aml.sjlbkw.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cri.zhixingplan.top

[R56] 远程拷贝
来源：http://hhm.sweek.top

scp file user@host:/path/
来源：http://hfp.yuanzhike.top

[R57] 远程执行命令
来源：http://quc.guannengcc.top

ssh user@host 'uptime'
来源：http://apb.cashguo.top

[R58] 下载文件
来源：http://fgy.0kj1m.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dkx.ppjwa.cn

[R59] 发 POST JSON
来源：http://eww.0kj1m.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bum.meibo888.top

[R60] 只看 HTTP 状态码
来源：http://egf.yfazqb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qyj.shzxlz.cn

[R61] 磁盘占用
来源：http://kqs.daxiang520.top

df -h;  du -sh *
来源：http://vlp.hfpthk.cn

[R62] 找最占空间的文件
来源：http://ahq.yueranfly.top

du -ah . | sort -rh | head -10
来源：http://yae.zhongyouzk.top

[R63] 内存与进程
来源：http://njf.ehwqpu.com

free -h;  ps aux | grep nginx
来源：http://saq.dashuyun.cn

[R64] 结束进程
来源：http://rsk.zhongyouzk.top

kill -9 $(pgrep -f app.py)
来源：http://hkj.hesvh.cn

[R65] 查看端口占用
来源：http://ins.jqgfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://aso.yvedp.cn

[R66] 定时任务
来源：http://rzk.chenlongwang.top

crontab -e;  crontab -l
来源：http://lil.chenjidiqi.icu

[R67] 生成随机十六进制串
来源：http://dnu.yangfankeji.com

openssl rand -hex 16
来源：http://oor.shanyushiyangkeji.top

[R68] 计算文件校验值
来源：http://xsu.hcnkem.com

sha256sum a.txt;  md5sum a.txt
来源：http://flf.hesvh.cn

[R69] 生成随机密码
来源：http://pon.zycfv.cn

head -c 16 /dev/urandom | base64
来源：http://sop.jinqigufen.top

[R70] 时间戳与互转
来源：http://wwd.52xcode.cn

date +%s;  date -d @1700000000
来源：http://fwd.tanke756.top

[R71] 日期格式化
来源：http://gec.zhoulong.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://ihb.daxiang520.top

[R72] 等待端口就绪
来源：http://eef.jinqigufen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ajf.ydzc1.top

[R73] 分割大日志
来源：http://ulj.fzhhl.top

split -l 1000 big.log part_
来源：http://oyg.52xcode.cn

[R74] 批量重命名
来源：http://slc.hammf.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bgs.ctjpmb.com

[R75] 导出环境变量
来源：http://bna.kuanghao11.cn

export PATH="$HOME/bin:$PATH"
来源：http://kcu.jinqigfzy.top

[R76] 使用临时文件
来源：http://stq.0kj1m.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wmi.jqgfzy.top

[R77] 读取用户输入
来源：http://jdd.fzhhl.top

read -rp "请输入: " ans
来源：http://boj.zhongyouzk.top

[R78] 交互式菜单
来源：http://gfk.zycfv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dii.yanxiufei.cn

[R79] 解析命令行选项
来源：http://hdi.ppjwa.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ovk.ydjk.org.cn

[R80] 查看脚本执行耗时
来源：http://yqj.jinqigufen.top

time ./run.sh
来源：http://zcj.yfazqb.com

================================================================================
来源：http://gaf.gogol.net.cn

S. C / C++ 专题
来源：http://bvu.sufxvd.cn

================================================================================
来源：http://nho.xuetiantiany.cn

[S01] C：Hello World
来源：http://uqu.ydjk.org.cn

#include <stdio.h>
来源：http://bgr.dianchejie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zos.gzhubu.top

[S02] C：变量与格式化输出
来源：http://yzg.chenlongwang.top

int a = 10; printf("%d\n", a);
来源：http://oas.sxryk.cn

[S03] C：读入整数
来源：http://qha.xinyue.icu

int x; scanf("%d", &x);
来源：http://rxa.fehbvm.com

[S04] C：字符串复制
来源：http://xvt.pycfn.com

char dst[32]; strcpy(dst, "hi");
来源：http://izs.jinqigufen.top

[S05] C：字符串长度
来源：http://ybq.jinghuilouyu.cn

strlen(s)
来源：http://wnw.yvedp.cn

[S06] C：字符串比较
来源：http://dsi.epnwcf.com

strcmp(a, b) == 0
来源：http://hjv.ydzc1.top

[S07] C：数组遍历求和
来源：http://hzt.chenlongwang.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eyk.gogol.net.cn

[S08] C：动态内存分配与释放
来源：http://xqx.tian-w.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kcf.hfpthk.cn

[S09] C：结构体定义与初始化
来源：http://bax.jqgfzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wvx.jyoumei.cn

[S10] C：指针与解引用
来源：http://gyu.fzhhl.top

int *p = &a;  *p = 5;
来源：http://nqz.pengpengdd.cyou

[S11] C：逐行读文件
来源：http://ilb.xylfe.cn

FILE *f = fopen("a.txt", "r");
来源：http://nry.shzxlz.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://eyy.bbcook.cn

fclose(f);
来源：http://bag.c1oappe.top

[S12] C：写文件
来源：http://ggf.yuanzhike.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rzl.daria6918.cn

[S13] C：宏定义
来源：http://yod.shuidangran.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hpz.fanxiaobao.xyz

[S14] C：枚举
来源：http://tng.316326.xyz

enum Color { RED, GREEN, BLUE };
来源：http://yxl.svipenyu.cn

[S15] C：类型转换
来源：http://npg.xylfe.cn

(double) a / b
来源：http://oow.tarul.cn

[S16] C：位操作置位
来源：http://lkc.sysykeji.top

x |= (1 << 3);
来源：http://veq.zhengqikj.top

[S17] C：安全拼接字符串
来源：http://axq.ydjk.org.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nug.yuanzhike.top

[S18] C：命令行参数
来源：http://uws.shanyushiyangkeji.top

int main(int argc, char **argv)
来源：http://nwr.ctjpmb.com

[S19] C：快速排序
来源：http://kaw.yj20258.top

qsort(a, n, sizeof(int), cmp);
来源：http://txa.zhixingplan.top

[S20] C：二分查找
来源：http://ysv.jinghuilouyu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wyx.shanyushiyangtech.top

[S21] C：字符类别判断
来源：http://pmz.fengsongda.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rjy.nanxinkj.top

[S22] C：字符串转数字
来源：http://fkm.xylfe.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tyk.hfpthk.cn

[S23] C：随机数
来源：http://fpo.bbcook.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lyj.jqgufenzy.top

[S24] C：获取本地时间
来源：http://oya.chenzaomai.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dga.fehbvm.com

[S25] C：内存拷贝
来源：http://yjr.ydjk.org.cn

memcpy(dst, src, n);
来源：http://ggv.cucudq.cn

[S26] C：内存清零
来源：http://mib.zdqjudy.top

memset(a, 0, sizeof a);
来源：http://prl.jinqigufen.top

[S27] C：定义常量
来源：http://iha.iojbl.cn

const double PI = 3.14159;
来源：http://dbg.chenzaomai.com

[S28] C：静态变量
来源：http://wgi.c1oappe.top

static int counter = 0;
来源：http://ywf.fanxiaobao.xyz

[S29] C：变参函数
来源：http://lou.dashuyun.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gol.aizwys.cn

[S30] C：头文件保护
来源：http://iri.shanyushiyangkeji.top

#ifndef X_H
来源：http://iqw.fehbvm.com

#define X_H
来源：http://lwq.shanyushiyangtech.top

#endif
来源：http://mrv.ydzc1.top

[S31] C++：Hello World
来源：http://ddt.hesvh.cn

#include <iostream>
来源：http://bzs.jinghuilouyu.cn

int main() { std::cout << "Hello\n"; }
来源：http://tzv.redwolf501.top

[S32] C++：字符串
来源：http://mow.316326.xyz

std::string s = "hi";  s += "!";
来源：http://rlr.fehbvm.com

[S33] C++：vector 增删
来源：http://cai.yuxming.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vzp.zhijiandao.cn

[S34] C++：遍历 vector
来源：http://eko.feifeiyinyue.top

for (auto &x : v) { std::cout << x; }
来源：http://ort.316326.xyz

[S35] C++：map
来源：http://cbu.ydjk.org.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pyf.yangfankeji.com

[S36] C++：unordered_map
来源：http://ttm.guowangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wmj.guannengcc.top

[S37] C++：set
来源：http://bnn.hnqzz.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sty.dashuyun.cn

[S38] C++：排序
来源：http://rmn.52xcode.cn

std::sort(v.begin(), v.end());
来源：http://yup.haohaochexian.top

[S39] C++：自定义比较器排序
来源：http://azt.nanxinkj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://psc.ybcxt.top

[S40] C++：查找元素
来源：http://cvk.ywan-chungtsiang.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qrh.jlsjyb.cn

[S41] C++：类与构造函数
来源：http://jjc.shuidangran.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jkm.zhengqikj.top

[S42] C++：继承与虚函数
来源：http://vqv.vehdjk.com

class B : public Base { public: void f() override {} };
来源：http://bkr.shanyushiyangtech.top

[S43] C++：智能指针
来源：http://csx.zhongyouzk.top

auto p = std::make_unique<int>(5);
来源：http://uea.tian-w.cn

[S44] C++：引用传参
来源：http://wmu.pycfn.com

void inc(int &x) { ++x; }
来源：http://ran.quarkkingdee.top

[S45] C++：lambda
来源：http://owt.c1oappe.top

auto add = [](int a, int b) { return a + b; };
来源：http://ecx.jqgufenzy.top

[S46] C++：函数模板
来源：http://syy.ybcxt.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ihf.sufxvd.cn

[S47] C++：结构化绑定遍历
来源：http://oed.uphjek.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kbt.kuanghao11.cn

[S48] C++：逐行读文件
来源：http://wqo.ppjwa.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vbj.shanyushiyangtech.top

while (std::getline(in, line)) { }
来源：http://xnn.feifeiyinyue.top

[S49] C++：写文件
来源：http://rcz.zycfv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lko.jyoumei.cn

[S50] C++：格式化数字
来源：http://sgt.shanyushiyangtech.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://irh.fehbvm.com

[S51] C++：显式类型转换
来源：http://ged.guannengcc.top

static_cast<double>(a) / b
来源：http://scu.snrcjt.cn

[S52] C++：const 与 noexcept
来源：http://pgh.tianlin.xyz

int size() const noexcept { return n_; }
来源：http://kvu.sysykeji.top

[S53] C++：移动语义
来源：http://kag.kuanghao11.cn

std::vector<int> w = std::move(v);
来源：http://ncd.quarkkingdee.top

[S54] C++：异常处理
来源：http://qrj.jinqigfzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mmv.zhengqikj.top

[S55] C++：结构化绑定
来源：http://akv.epnwcf.com

auto [a, b] = std::make_pair(1, 2);
来源：http://iun.snrcjt.cn

[S56] C++：optional
来源：http://zcb.daria6918.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rto.xinyue.icu

[S57] C++：编译期常量
来源：http://cku.ydzc1.top

constexpr int N = 10;
来源：http://yie.tianlin.xyz

[S58] C++：命名空间
来源：http://fkg.shanyushiyangtech.top

namespace ns { int f() { return 1; } }
来源：http://xwn.zhiwuduotai.top

[S59] C++：静态断言
来源：http://exr.chenjidiqi.icu

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wyy.pycfn.com

[S60] C++：遍历并删除元素
来源：http://cdk.316326.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ycw.dashuyun.cn

================================================================================
来源：http://ooi.ehwqpu.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qow.yuxming.cn

================================================================================
来源：http://xkw.tarul.cn

[T01] Kotlin：Hello World
来源：http://tbo.xinyue.icu

println("Hello")
来源：http://pjo.zhongyouzk.top

[T02] Kotlin：变量
来源：http://mgp.wangdashe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://eay.yuxming.cn

[T03] Kotlin：字符串模板
来源：http://pzn.hongshengwenyu.top

"值: $b"
来源：http://qsi.andypj.xyz

[T04] Kotlin：空安全
来源：http://zvm.vqdsnc.cn

val n: String? = null;  n?.length
来源：http://yvi.9152youxi.cn

[T05] Kotlin：when 表达式
来源：http://ymw.uphjek.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rph.ydjk.org.cn

[T06] Kotlin：集合映射
来源：http://jxl.nanxuanxn.top

listOf(1, 2, 3).map { it * 2 }
来源：http://han.zhijiandao.cn

[T07] Kotlin：集合过滤
来源：http://izs.gaohongyu789.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kaa.cheryme.top

[T08] Kotlin：数据类
来源：http://fhh.sufxvd.cn

data class User(val name: String, val age: Int)
来源：http://wce.havefunace.top

[T09] Kotlin：扩展函数
来源：http://zqc.yuanzhike.top

fun String.exclaim() = this + "!"
来源：http://tfu.jqgfzy.top

[T10] Kotlin：默认参数
来源：http://pma.yanxiufei.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://met.xuetiantiany.cn

[T11] Kotlin：协程
来源：http://ahh.c1oappe.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://dvj.aibaodan.cn

[T12] Kotlin：解构声明
来源：http://qgv.shanyushiyangkeji.top

val (a, b) = Pair(1, 2)
来源：http://opl.mhx1999.top

[T13] Kotlin：只读 Map
来源：http://koy.sufxvd.cn

val m = mapOf("a" to 1)
来源：http://zyj.shuidangran.top

[T14] Kotlin：循环
来源：http://dif.hfpthk.cn

for (i in 1..10) println(i)
来源：http://dcy.fengsongda.top

[T15] Kotlin：接口
来源：http://hpu.tanke756.top

interface Shape { fun area(): Double }
来源：http://cnn.jinqigfzy.top

[T16] Swift：Hello World
来源：http://tug.hnxiangtu.top

print("Hello")
来源：http://jek.fanxiaobao.xyz

[T17] Swift：变量与常量
来源：http://efn.jqgufenzy.top

var a = 1;  let b = 2
来源：http://mqb.chenzaomai.com

[T18] Swift：字符串插值
来源：http://xcp.jqgfzy.top

"值: \(b)"
来源：http://cfe.aibaodan.cn

[T19] Swift：可选绑定
来源：http://cyt.chenzaomai.com

if let n = opt { print(n) }
来源：http://sid.xuanzx.com

[T20] Swift：数组操作
来源：http://zzw.cdnleiting.top

var a = [1, 2, 3];  a.append(4)
来源：http://cjy.mhx1999.top

[T21] Swift：遍历
来源：http://qlp.smart0.xyz

for x in a { print(x) }
来源：http://ecc.snrcjt.cn

[T22] Swift：字典
来源：http://ofa.gotoacloud.top

var d = ["a": 1];  d["b"] = 2
来源：http://pnz.shuidangran.top

[T23] Swift：函数
来源：http://wzv.zhiwuduotai.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tuc.yuanzhike.top

[T24] Swift：闭包
来源：http://jyo.hesvh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fjc.hysaishi.cn

[T25] Swift：结构体
来源：http://oxi.jinqigfzy.top

struct P { var x: Int }
来源：http://mtf.9152youxi.cn

[T26] Swift：类与重写
来源：http://zrc.zycfv.cn

class A: Base { override func f() {} }
来源：http://rzh.vehdjk.com

[T27] Swift：错误处理
来源：http://yop.svipenyu.cn

do { try f() } catch { print(error) }
来源：http://wce.yonumen.top

[T28] Swift：枚举
来源：http://nlb.birdmap.top

enum Color { case red, green }
来源：http://jns.havefunace.top

[T29] Swift：guard 提前返回
来源：http://hep.cdnleiting.top

guard let x = opt else { return }
来源：http://chm.yvedp.cn

[T30] Swift：协议
来源：http://qoj.tarul.cn

protocol Shape { func area() -> Double }
来源：http://tiw.zhijiandao.cn

[T31] Lua：Hello World
来源：http://sqn.zdqjudy.top

print("Hello")
来源：http://wpb.yueranfly.top

[T32] Lua：局部变量
来源：http://ftq.yanxiufei.cn

local a = 1
来源：http://vjm.zycfv.cn

[T33] Lua：表（数组）
来源：http://bpx.yj20258.top

local t = {1, 2, 3};  t[4] = 4
来源：http://xnl.fktsv.cn

[T34] Lua：遍历表
来源：http://zzd.nanxinkj.top

for i, v in ipairs(t) do print(i, v) end
来源：http://xqb.fzhhl.top

[T35] Lua：字典表
来源：http://yqa.pycfn.com

local d = { a = 1 };  d.b = 2
来源：http://eij.hfpthk.cn

[T36] Lua：函数
来源：http://mvr.yanxiufei.cn

function add(a, b) return a + b end
来源：http://xmm.jinqigfzy.top

[T37] Lua：字符串拼接
来源：http://rcv.yuanzhike.top

"a" .. "b"
来源：http://pxh.yuxming.cn

[T38] Lua：条件
来源：http://kom.feifeiyinyue.top

if x > 0 then print("正") end
来源：http://dos.epnwcf.com

[T39] Lua：模式匹配
来源：http://erw.sxryk.cn

string.find(s, "%d+")
来源：http://pfi.xuetiantiany.cn

[T40] Lua：元表
来源：http://wxk.9152youxi.cn

setmetatable({}, { __index = base })
来源：http://rbp.tanke756.top

[T41] Perl：Hello World
来源：http://mtt.pycfn.com

print "Hello\n";
来源：http://sgl.sweek.top

[T42] Perl：变量类型
来源：http://jdn.jiagoushi.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://use.yj20258888.top

[T43] Perl：字符串插值
来源：http://ivz.xinyue.icu

"值: $a"
来源：http://rab.sweek.top

[T44] Perl：条件
来源：http://gtw.yj20258888.top

if ($a > 0) { print "正"; }
来源：http://byh.52xcode.cn

[T45] Perl：数组遍历
来源：http://zob.zhoulong.xyz

for my $x (@arr) { print $x; }
来源：http://vdc.wangdashe.top

[T46] Perl：哈希操作
来源：http://fiv.9152youxi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lvu.shanyushiyangtech.top

[T47] Perl：正则捕获
来源：http://fei.nanxinkj.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://jyy.dashuyun.cn

[T48] Perl：正则替换
来源：http://qin.nanxinkj.top

$s =~ s/old/new/g;
来源：http://qma.dianchejie.cn

[T49] Perl：函数
来源：http://iot.havefunace.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xlz.zhongyouzk.top

[T50] Perl：逐行读文件
来源：http://ytf.chenzaomai.com

open my $fh, "<", "a.txt" or die $!;
来源：http://huy.yanxiufei.cn

while (my $line = <$fh>) { print $line; }
来源：http://efi.nanxuanxn.top

[T51] Scala：Hello World
来源：http://gjq.dashuyun.cn

println("Hello")
来源：http://zzu.zdbjq.cn

[T52] Scala：变量
来源：http://loc.zhixingplan.top


<!-- 参考信息 -->