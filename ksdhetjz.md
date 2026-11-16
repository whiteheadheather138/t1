代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bra.jinyuanbaomall.cn

[R50] awk 求和
来源：http://tqo.bjfxy.top

awk '{s += $2} END {print s}' a.txt
来源：http://ocn.shanyushiyangkeji.top

[R51] 排序去重取前几
来源：http://tzg.fktsv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://byj.vehdjk.com

[R52] 统计行数
来源：http://xza.ydzc1.top

wc -l a.txt
来源：http://kbu.zhixingplan.top

[R53] 查看文件头与实时尾
来源：http://fsz.nwbrower.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mvs.snrcjt.cn

[R54] 比较两个文件
来源：http://jrq.shanyushiyangkeji.top

diff a.txt b.txt
来源：http://dqe.jyoumei.cn

[R55] 压缩与解压
来源：http://sxj.tarul.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hef.hnxiangtu.top

[R56] 远程拷贝
来源：http://fxr.yvedp.cn

scp file user@host:/path/
来源：http://hpr.hfpthk.cn

[R57] 远程执行命令
来源：http://xdi.redwolf501.top

ssh user@host 'uptime'
来源：http://nsr.shzxlz.cn

[R58] 下载文件
来源：http://zod.yueranfly.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gjw.zhixingplan.top

[R59] 发 POST JSON
来源：http://png.yueranfly.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rqk.yongpay.top

[R60] 只看 HTTP 状态码
来源：http://bss.meibo888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sap.gaohongyu789.top

[R61] 磁盘占用
来源：http://ieq.shzxlz.cn

df -h;  du -sh *
来源：http://mxl.jinqigfzy.top

[R62] 找最占空间的文件
来源：http://dkg.jinqigfzy.top

du -ah . | sort -rh | head -10
来源：http://ecv.cdnleiting.top

[R63] 内存与进程
来源：http://avi.birdmap.top

free -h;  ps aux | grep nginx
来源：http://ycu.sysykeji.top

[R64] 结束进程
来源：http://dlc.jinqigufen.top

kill -9 $(pgrep -f app.py)
来源：http://hhn.birdmap.top

[R65] 查看端口占用
来源：http://hfy.jqgufenzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://izu.daria6918.cn

[R66] 定时任务
来源：http://dgp.9152youxi.cn

crontab -e;  crontab -l
来源：http://crf.jqgufenzy.top

[R67] 生成随机十六进制串
来源：http://nte.hammf.cn

openssl rand -hex 16
来源：http://vze.zhijiandao.cn

[R68] 计算文件校验值
来源：http://ucm.jinyuanbaomall.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kun.cqqwz.cn

[R69] 生成随机密码
来源：http://tqe.zycfv.cn

head -c 16 /dev/urandom | base64
来源：http://xiu.smart0.xyz

[R70] 时间戳与互转
来源：http://rmm.hysaishi.cn

date +%s;  date -d @1700000000
来源：http://mll.daxiang520.top

[R71] 日期格式化
来源：http://oba.bbcook.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://teu.zhongyouzk.top

[R72] 等待端口就绪
来源：http://ktm.guowangkeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://amv.xuanzx.com

[R73] 分割大日志
来源：http://oyf.ctjpmb.com

split -l 1000 big.log part_
来源：http://czn.hfpthk.cn

[R74] 批量重命名
来源：http://jcl.epnwcf.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dkd.gzhubu.top

[R75] 导出环境变量
来源：http://rpy.ydjk.org.cn

export PATH="$HOME/bin:$PATH"
来源：http://cdo.wangshuangyany.cn

[R76] 使用临时文件
来源：http://goo.yanxiufei.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zgy.vqdsnc.cn

[R77] 读取用户输入
来源：http://ejk.chenlongwang.top

read -rp "请输入: " ans
来源：http://ats.birdmap.top

[R78] 交互式菜单
来源：http://skb.chenzaomai.com

select opt in a b c; do echo "$opt"; break; done
来源：http://sfg.yuxming.cn

[R79] 解析命令行选项
来源：http://ffe.zhiwuduotai.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://htf.snrcjt.cn

[R80] 查看脚本执行耗时
来源：http://uwx.gaohongyu789.top

time ./run.sh
来源：http://wzi.zhijiandao.cn

================================================================================
来源：http://gmr.zycfv.cn

S. C / C++ 专题
来源：http://wlt.yj20258.top

================================================================================
来源：http://giy.ydjk.org.cn

[S01] C：Hello World
来源：http://xvz.havefunace.top

#include <stdio.h>
来源：http://xlh.yongpay.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://fdn.gogol.net.cn

[S02] C：变量与格式化输出
来源：http://yfh.zhoulong.xyz

int a = 10; printf("%d\n", a);
来源：http://tzf.vehdjk.com

[S03] C：读入整数
来源：http://gkv.fanxiaobao.xyz

int x; scanf("%d", &x);
来源：http://ukz.shzxlz.cn

[S04] C：字符串复制
来源：http://ins.xuanzx.com

char dst[32]; strcpy(dst, "hi");
来源：http://uzf.fanxiaobao.xyz

[S05] C：字符串长度
来源：http://aqv.ehwqpu.com

strlen(s)
来源：http://sbk.xziqi.cn

[S06] C：字符串比较
来源：http://osi.aibaodan.cn

strcmp(a, b) == 0
来源：http://yxv.zhijiandao.cn

[S07] C：数组遍历求和
来源：http://lde.yangfankeji.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bee.gotoacloud.top

[S08] C：动态内存分配与释放
来源：http://wwx.bbcook.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dcu.vehdjk.com

[S09] C：结构体定义与初始化
来源：http://fhe.9152youxi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lri.yj20258888.top

[S10] C：指针与解引用
来源：http://ebi.zhiwuduotai.top

int *p = &a;  *p = 5;
来源：http://fnr.daria6918.cn

[S11] C：逐行读文件
来源：http://lsq.yueranfly.top

FILE *f = fopen("a.txt", "r");
来源：http://mvc.fktsv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vjy.nanxuanxn.top

fclose(f);
来源：http://kxu.pycfn.com

[S12] C：写文件
来源：http://zwj.kuanghao11.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xft.ppjwa.cn

[S13] C：宏定义
来源：http://hvo.zycfv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lhz.hnqzz.top

[S14] C：枚举
来源：http://xlm.yj20258888.top

enum Color { RED, GREEN, BLUE };
来源：http://irh.xylfe.cn

[S15] C：类型转换
来源：http://kdw.fktsv.cn

(double) a / b
来源：http://njk.xuanzx.com

[S16] C：位操作置位
来源：http://hzb.ybcxt.top

x |= (1 << 3);
来源：http://edl.yueranfly.top

[S17] C：安全拼接字符串
来源：http://ewg.snrcjt.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://chk.bbcook.cn

[S18] C：命令行参数
来源：http://chc.0kj1m.cn

int main(int argc, char **argv)
来源：http://cmq.jiagoushi.top

[S19] C：快速排序
来源：http://uko.sysykeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://aym.hcnkem.com

[S20] C：二分查找
来源：http://dbg.9152youxi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cpt.xuanzx.com

[S21] C：字符类别判断
来源：http://ihg.jqgfzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hlc.xziqi.cn

[S22] C：字符串转数字
来源：http://wye.shanyushiyangtech.top

atoi("42");  strtod("3.14", NULL);
来源：http://kfh.xylfe.cn

[S23] C：随机数
来源：http://efp.hnxiangtu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xph.birdmap.top

[S24] C：获取本地时间
来源：http://vrc.zdqjudy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://efe.zhengqikj.top

[S25] C：内存拷贝
来源：http://dkx.sjlbkw.cn

memcpy(dst, src, n);
来源：http://ejw.guannengcc.top

[S26] C：内存清零
来源：http://vlp.hfpthk.cn

memset(a, 0, sizeof a);
来源：http://iiw.316326.xyz

[S27] C：定义常量
来源：http://vja.ctjpmb.com

const double PI = 3.14159;
来源：http://juy.haohaochexian.top

[S28] C：静态变量
来源：http://wgl.zhongyouzk.top

static int counter = 0;
来源：http://bjl.feifeiyinyue.top

[S29] C：变参函数
来源：http://jqe.gaohongyu789.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rhd.fanxiaobao.xyz

[S30] C：头文件保护
来源：http://yhm.ybcxt.top

#ifndef X_H
来源：http://hvh.birdmap.top

#define X_H
来源：http://eme.316326.xyz

#endif
来源：http://sqz.jinqigufen.top

[S31] C++：Hello World
来源：http://ntf.jinyuanbaomall.cn

#include <iostream>
来源：http://ddx.shanyushiyangtech.top

int main() { std::cout << "Hello\n"; }
来源：http://bdv.redwolf501.top

[S32] C++：字符串
来源：http://lif.cqqwz.cn

std::string s = "hi";  s += "!";
来源：http://pnw.guowangkeji.top

[S33] C++：vector 增删
来源：http://tlt.cashguo.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bfa.cheryme.top

[S34] C++：遍历 vector
来源：http://srw.tianlin.xyz

for (auto &x : v) { std::cout << x; }
来源：http://nxk.chenlongwang.top

[S35] C++：map
来源：http://fod.c1oappe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eoq.kuanghao11.cn

[S36] C++：unordered_map
来源：http://eim.cashguo.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vtb.chenjidiqi.icu

[S37] C++：set
来源：http://gfd.aibaodan.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vde.xinyue.icu

[S38] C++：排序
来源：http://uvc.yonumen.top

std::sort(v.begin(), v.end());
来源：http://zps.xinyue.icu

[S39] C++：自定义比较器排序
来源：http://ziw.fanxiaobao.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yhl.yangfankeji.com

[S40] C++：查找元素
来源：http://pup.wangshuangyany.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://amw.yanxiufei.cn

[S41] C++：类与构造函数
来源：http://rqd.pycfn.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://owu.fengsongda.top

[S42] C++：继承与虚函数
来源：http://uvc.hammf.cn

class B : public Base { public: void f() override {} };
来源：http://eis.fengsongda.top

[S43] C++：智能指针
来源：http://yuw.xziqi.cn

auto p = std::make_unique<int>(5);
来源：http://mgf.andypj.xyz

[S44] C++：引用传参
来源：http://wqz.jiagoushi.top

void inc(int &x) { ++x; }
来源：http://zjc.wangdashe.top

[S45] C++：lambda
来源：http://eut.52xcode.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bqj.daxiang520.top

[S46] C++：函数模板
来源：http://gys.jlsjyb.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hvt.xuetiantiany.cn

[S47] C++：结构化绑定遍历
来源：http://nst.zhengqikj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qgm.ybcxt.top

[S48] C++：逐行读文件
来源：http://yte.gotoacloud.top

std::ifstream in("a.txt");  std::string line;
来源：http://umr.shangyingyoupin.top

while (std::getline(in, line)) { }
来源：http://uha.hnxiangtu.top

[S49] C++：写文件
来源：http://rps.guowangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ule.svipenyu.cn

[S50] C++：格式化数字
来源：http://ksz.mhx1999.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nmw.kuanghao11.cn

[S51] C++：显式类型转换
来源：http://fct.sweek.top

static_cast<double>(a) / b
来源：http://ybh.yanxiufei.cn

[S52] C++：const 与 noexcept
来源：http://esk.ehwqpu.com

int size() const noexcept { return n_; }
来源：http://ogy.sjlbkw.cn

[S53] C++：移动语义
来源：http://msp.jqgufenzy.top

std::vector<int> w = std::move(v);
来源：http://ycu.aizwys.cn

[S54] C++：异常处理
来源：http://csq.zycfv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://svn.xuetiantiany.cn

[S55] C++：结构化绑定
来源：http://jlx.fktsv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gie.wangshuangyany.cn

[S56] C++：optional
来源：http://pdr.gzhubu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://imb.zdbjq.cn

[S57] C++：编译期常量
来源：http://gal.jianghu66.top

constexpr int N = 10;
来源：http://aea.gotoacloud.top

[S58] C++：命名空间
来源：http://pbu.epnwcf.com

namespace ns { int f() { return 1; } }
来源：http://lap.hnqzz.top

[S59] C++：静态断言
来源：http://suf.hesvh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xqu.snrcjt.cn

[S60] C++：遍历并删除元素
来源：http://fpu.vqdsnc.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oma.aizwys.cn

================================================================================
来源：http://glu.shuidangran.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iml.hysaishi.cn

================================================================================
来源：http://iaz.zhengqikj.top

[T01] Kotlin：Hello World
来源：http://rvb.jinyuanbaomall.cn

println("Hello")
来源：http://rie.aizwys.cn

[T02] Kotlin：变量
来源：http://nkf.guowangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baa.xuanzx.com

[T03] Kotlin：字符串模板
来源：http://hdz.gaohongyu789.top

"值: $b"
来源：http://evp.52xcode.cn

[T04] Kotlin：空安全
来源：http://zay.yangfankeji.com

val n: String? = null;  n?.length
来源：http://cdd.jlsjyb.cn

[T05] Kotlin：when 表达式
来源：http://cba.gogol.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://urx.jinyuanbaomall.cn

[T06] Kotlin：集合映射
来源：http://ghz.fktsv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ubn.yfazqb.com

[T07] Kotlin：集合过滤
来源：http://gdk.epnwcf.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://rhe.zdbjq.cn

[T08] Kotlin：数据类
来源：http://vbk.feifeiyinyue.top

data class User(val name: String, val age: Int)
来源：http://zaf.hesvh.cn

[T09] Kotlin：扩展函数
来源：http://hun.smart0.xyz

fun String.exclaim() = this + "!"
来源：http://gds.haohaochexian.top

[T10] Kotlin：默认参数
来源：http://orv.quarkkingdee.top

fun greet(name: String = "World") = "Hi $name"
来源：http://krx.jinyuanbaomall.cn

[T11] Kotlin：协程
来源：http://wwh.zhongyouzk.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://egk.jianghu66.top

[T12] Kotlin：解构声明
来源：http://lui.havefunace.top

val (a, b) = Pair(1, 2)
来源：http://eva.sysykeji.top

[T13] Kotlin：只读 Map
来源：http://aij.ybcxt.top

val m = mapOf("a" to 1)
来源：http://xck.fktsv.cn

[T14] Kotlin：循环
来源：http://akl.yueranfly.top

for (i in 1..10) println(i)
来源：http://afj.dashuyun.cn

[T15] Kotlin：接口
来源：http://hdj.zhiwuduotai.top

interface Shape { fun area(): Double }
来源：http://czr.yueranfly.top

[T16] Swift：Hello World
来源：http://hyt.daxiang520.top

print("Hello")
来源：http://xeg.jiagoushi.top

[T17] Swift：变量与常量
来源：http://drn.hongshengwenyu.top

var a = 1;  let b = 2
来源：http://vfg.vehdjk.com

[T18] Swift：字符串插值
来源：http://scx.hcnkem.com

"值: \(b)"
来源：http://jjb.chenlongwang.top

[T19] Swift：可选绑定
来源：http://ani.tianlin.xyz

if let n = opt { print(n) }
来源：http://fit.ctjpmb.com

[T20] Swift：数组操作
来源：http://tji.yj20258888.top

var a = [1, 2, 3];  a.append(4)
来源：http://eqr.wangshuangyany.cn

[T21] Swift：遍历
来源：http://qdc.c1oappe.top

for x in a { print(x) }
来源：http://uxz.9152youxi.cn

[T22] Swift：字典
来源：http://zga.hysaishi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xzf.snrcjt.cn

[T23] Swift：函数
来源：http://znh.cdnleiting.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://oxr.haohaochexian.top

[T24] Swift：闭包
来源：http://ovb.vqdsnc.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rtq.svipenyu.cn

[T25] Swift：结构体
来源：http://yyi.birdmap.top

struct P { var x: Int }
来源：http://hru.guowangkeji.top

[T26] Swift：类与重写
来源：http://bwb.meibo888.top

class A: Base { override func f() {} }
来源：http://kvh.jqgfzy.top

[T27] Swift：错误处理
来源：http://jsa.zhaomingkeji.xyz

do { try f() } catch { print(error) }
来源：http://zyj.ppjwa.cn

[T28] Swift：枚举
来源：http://uis.pengpengdd.cyou

enum Color { case red, green }
来源：http://sqd.zdqjudy.top

[T29] Swift：guard 提前返回
来源：http://huu.jyoumei.cn

guard let x = opt else { return }
来源：http://opp.vehdjk.com

[T30] Swift：协议
来源：http://azn.nanxuanxn.top

protocol Shape { func area() -> Double }
来源：http://puj.yuxming.cn

[T31] Lua：Hello World
来源：http://kfc.jinqigufen.top

print("Hello")
来源：http://gdj.fengsongda.top

[T32] Lua：局部变量
来源：http://eql.jinghuilouyu.cn

local a = 1
来源：http://ssz.tianlin.xyz

[T33] Lua：表（数组）
来源：http://dcg.yuanzhike.top

local t = {1, 2, 3};  t[4] = 4
来源：http://lex.sweek.top

[T34] Lua：遍历表
来源：http://qxp.chenjidiqi.icu

for i, v in ipairs(t) do print(i, v) end
来源：http://pmv.jqgufenzy.top

[T35] Lua：字典表
来源：http://hoh.zhengqikj.top

local d = { a = 1 };  d.b = 2
来源：http://lrq.feifeiyinyue.top

[T36] Lua：函数
来源：http://tnz.9152youxi.cn

function add(a, b) return a + b end
来源：http://gom.fehbvm.com

[T37] Lua：字符串拼接
来源：http://qim.wangdashe.top

"a" .. "b"
来源：http://kfd.quarkkingdee.top

[T38] Lua：条件
来源：http://qjj.feifeiyinyue.top

if x > 0 then print("正") end
来源：http://gev.feifeiyinyue.top

[T39] Lua：模式匹配
来源：http://ujc.fengsongda.top

string.find(s, "%d+")
来源：http://nuj.kuanghao11.cn

[T40] Lua：元表
来源：http://tbj.xinyue.icu

setmetatable({}, { __index = base })
来源：http://cdb.kuanghao11.cn

[T41] Perl：Hello World
来源：http://omw.ehwqpu.com

print "Hello\n";
来源：http://mai.jyoumei.cn

[T42] Perl：变量类型
来源：http://jgb.fehbvm.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hwn.aizwys.cn

[T43] Perl：字符串插值
来源：http://trp.jinghuilouyu.cn

"值: $a"
来源：http://czi.zhoulong.xyz

[T44] Perl：条件
来源：http://vsv.yuxming.cn

if ($a > 0) { print "正"; }
来源：http://gms.daria6918.cn

[T45] Perl：数组遍历
来源：http://wpv.epnwcf.com

for my $x (@arr) { print $x; }
来源：http://xsp.tian-w.cn

[T46] Perl：哈希操作
来源：http://xzq.smart0.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vcm.9152youxi.cn

[T47] Perl：正则捕获
来源：http://tkx.gaohongyu789.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ptl.cashguo.top

[T48] Perl：正则替换
来源：http://qpi.dashuyun.cn

$s =~ s/old/new/g;
来源：http://let.mhx1999.top

[T49] Perl：函数
来源：http://vem.fehbvm.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lgk.sxryk.cn

[T50] Perl：逐行读文件
来源：http://wmf.bbcook.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://flw.svipenyu.cn

while (my $line = <$fh>) { print $line; }
来源：http://kmd.jyoumei.cn

[T51] Scala：Hello World
来源：http://cue.sysykeji.top

println("Hello")
来源：http://apn.shanyushiyangtech.top

[T52] Scala：变量
来源：http://ozh.yongpay.top


<!-- 参考信息 -->