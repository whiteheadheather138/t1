代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://qnx.yfazqb.com

[R48] awk 取指定列
来源：http://xda.jiagoushi.top

awk '{print $1, $3}' a.txt
来源：http://guf.guowangkeji.top

[R49] awk 带条件
来源：http://aax.haohaochexian.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ewt.yfazqb.com

[R50] awk 求和
来源：http://kjp.iojbl.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yaj.9152youxi.cn

[R51] 排序去重取前几
来源：http://rth.meibo888.top

sort a.txt | uniq -c | sort -rn | head
来源：http://alo.cashguo.top

[R52] 统计行数
来源：http://dha.uphjek.com

wc -l a.txt
来源：http://vle.wangshuangyany.cn

[R53] 查看文件头与实时尾
来源：http://fzr.zycfv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ked.ydjk.org.cn

[R54] 比较两个文件
来源：http://drp.zhixingplan.top

diff a.txt b.txt
来源：http://uou.jinghuilouyu.cn

[R55] 压缩与解压
来源：http://klm.fanxiaobao.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bqu.fzhhl.top

[R56] 远程拷贝
来源：http://nzo.bbcook.cn

scp file user@host:/path/
来源：http://fvh.hcnkem.com

[R57] 远程执行命令
来源：http://vqf.quarkkingdee.top

ssh user@host 'uptime'
来源：http://dem.xuanzx.com

[R58] 下载文件
来源：http://xly.gotoacloud.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ohp.fzhhl.top

[R59] 发 POST JSON
来源：http://aed.zhongyouzk.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://etu.dashuyun.cn

[R60] 只看 HTTP 状态码
来源：http://fxh.sufxvd.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pyr.guannengcc.top

[R61] 磁盘占用
来源：http://nzk.sjlbkw.cn

df -h;  du -sh *
来源：http://tgc.hnqzz.top

[R62] 找最占空间的文件
来源：http://zyq.yj20258888.top

du -ah . | sort -rh | head -10
来源：http://jhf.jinqigfzy.top

[R63] 内存与进程
来源：http://qbv.dianchejie.cn

free -h;  ps aux | grep nginx
来源：http://vdd.zycfv.cn

[R64] 结束进程
来源：http://tpz.hfpthk.cn

kill -9 $(pgrep -f app.py)
来源：http://fmt.zhixingplan.top

[R65] 查看端口占用
来源：http://avz.jqgufenzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mha.sjlbkw.cn

[R66] 定时任务
来源：http://rxy.sufxvd.cn

crontab -e;  crontab -l
来源：http://qhn.ivvv.top

[R67] 生成随机十六进制串
来源：http://ils.shanyushiyangkeji.top

openssl rand -hex 16
来源：http://tjb.hammf.cn

[R68] 计算文件校验值
来源：http://yad.shanyushiyangkeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://zpm.nanxinkj.top

[R69] 生成随机密码
来源：http://lor.yuxming.cn

head -c 16 /dev/urandom | base64
来源：http://kav.zdqjudy.top

[R70] 时间戳与互转
来源：http://zsa.sufxvd.cn

date +%s;  date -d @1700000000
来源：http://cbt.daxiang520.top

[R71] 日期格式化
来源：http://vaq.fktsv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://aog.zhoulong.xyz

[R72] 等待端口就绪
来源：http://fdc.0kj1m.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yej.hcnkem.com

[R73] 分割大日志
来源：http://lxk.cucudq.cn

split -l 1000 big.log part_
来源：http://dqb.hysaishi.cn

[R74] 批量重命名
来源：http://yks.zhijiandao.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vhy.gotoacloud.top

[R75] 导出环境变量
来源：http://ycj.ivvv.top

export PATH="$HOME/bin:$PATH"
来源：http://awi.sxryk.cn

[R76] 使用临时文件
来源：http://xym.zhaomingkeji.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fzz.snrcjt.cn

[R77] 读取用户输入
来源：http://fuq.sjlbkw.cn

read -rp "请输入: " ans
来源：http://qpq.cqqwz.cn

[R78] 交互式菜单
来源：http://rqj.epnwcf.com

select opt in a b c; do echo "$opt"; break; done
来源：http://ojw.zycfv.cn

[R79] 解析命令行选项
来源：http://ffi.nwbrower.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mnf.ctjpmb.com

[R80] 查看脚本执行耗时
来源：http://hcr.wangdashe.top

time ./run.sh
来源：http://mbl.yuanzhike.top

================================================================================
来源：http://zco.fktsv.cn

S. C / C++ 专题
来源：http://dtt.0kj1m.cn

================================================================================
来源：http://niq.9152youxi.cn

[S01] C：Hello World
来源：http://ybf.316326.xyz

#include <stdio.h>
来源：http://psp.yongpay.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qtn.chenlongwang.top

[S02] C：变量与格式化输出
来源：http://xej.yj202588.top

int a = 10; printf("%d\n", a);
来源：http://ezl.ydzc1.top

[S03] C：读入整数
来源：http://skr.xziqi.cn

int x; scanf("%d", &x);
来源：http://zrc.hammf.cn

[S04] C：字符串复制
来源：http://hpr.shanyushiyangtech.top

char dst[32]; strcpy(dst, "hi");
来源：http://kzc.jinghuilouyu.cn

[S05] C：字符串长度
来源：http://edq.shanyushiyangkeji.top

strlen(s)
来源：http://dom.zhaomingkeji.xyz

[S06] C：字符串比较
来源：http://wkq.jyoumei.cn

strcmp(a, b) == 0
来源：http://but.tanke756.top

[S07] C：数组遍历求和
来源：http://bgw.pycfn.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ljq.yuxming.cn

[S08] C：动态内存分配与释放
来源：http://lym.sysykeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://msl.jinqigfzy.top

[S09] C：结构体定义与初始化
来源：http://aau.tianlin.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vzo.zhixingplan.top

[S10] C：指针与解引用
来源：http://qmd.uphjek.com

int *p = &a;  *p = 5;
来源：http://xjz.uphjek.com

[S11] C：逐行读文件
来源：http://tab.jqgfzy.top

FILE *f = fopen("a.txt", "r");
来源：http://pfx.316326.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://fea.jyoumei.cn

fclose(f);
来源：http://lor.zdqjudy.top

[S12] C：写文件
来源：http://uvg.daxiang520.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zdu.yuxming.cn

[S13] C：宏定义
来源：http://thn.nwbrower.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://aea.fehbvm.com

[S14] C：枚举
来源：http://otc.chenzaomai.com

enum Color { RED, GREEN, BLUE };
来源：http://kni.yj202588.top

[S15] C：类型转换
来源：http://tle.tarul.cn

(double) a / b
来源：http://gqh.chenlongwang.top

[S16] C：位操作置位
来源：http://waa.sjlbkw.cn

x |= (1 << 3);
来源：http://osw.jinqigufen.top

[S17] C：安全拼接字符串
来源：http://xul.52xcode.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tin.yangfankeji.com

[S18] C：命令行参数
来源：http://yza.hnqzz.top

int main(int argc, char **argv)
来源：http://frh.xuanzx.com

[S19] C：快速排序
来源：http://wgs.jiagoushi.top

qsort(a, n, sizeof(int), cmp);
来源：http://gqc.ydzc1.top

[S20] C：二分查找
来源：http://kei.sufxvd.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wob.shuidangran.top

[S21] C：字符类别判断
来源：http://eto.yonumen.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://taa.jiagoushi.top

[S22] C：字符串转数字
来源：http://eqx.gogol.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://aim.cdnleiting.top

[S23] C：随机数
来源：http://foj.fanxiaobao.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://jiq.xuetiantiany.cn

[S24] C：获取本地时间
来源：http://akv.shanyushiyangkeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vsr.zdqjudy.top

[S25] C：内存拷贝
来源：http://sro.cheryme.top

memcpy(dst, src, n);
来源：http://gcb.bbcook.cn

[S26] C：内存清零
来源：http://vow.fanxiaobao.xyz

memset(a, 0, sizeof a);
来源：http://vcn.ivvv.top

[S27] C：定义常量
来源：http://vbe.jlsjyb.cn

const double PI = 3.14159;
来源：http://ogh.xuetiantiany.cn

[S28] C：静态变量
来源：http://opz.fanxiaobao.xyz

static int counter = 0;
来源：http://bar.shangyingyoupin.top

[S29] C：变参函数
来源：http://ssu.jqgfzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zik.ywan-chungtsiang.top

[S30] C：头文件保护
来源：http://anm.chenlongwang.top

#ifndef X_H
来源：http://hye.nanxinkj.top

#define X_H
来源：http://som.cucudq.cn

#endif
来源：http://puh.jlsjyb.cn

[S31] C++：Hello World
来源：http://ikq.feifeiyinyue.top

#include <iostream>
来源：http://mwc.ivvv.top

int main() { std::cout << "Hello\n"; }
来源：http://gft.ctjpmb.com

[S32] C++：字符串
来源：http://mwd.yvedp.cn

std::string s = "hi";  s += "!";
来源：http://ixr.gzhubu.top

[S33] C++：vector 增删
来源：http://srz.ehwqpu.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rah.52xcode.cn

[S34] C++：遍历 vector
来源：http://vfu.haohaochexian.top

for (auto &x : v) { std::cout << x; }
来源：http://gvt.fehbvm.com

[S35] C++：map
来源：http://vqe.epnwcf.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yvo.chenjidiqi.icu

[S36] C++：unordered_map
来源：http://ahz.haohaochexian.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sfs.smart0.xyz

[S37] C++：set
来源：http://qpi.52xcode.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://njp.jqgufenzy.top

[S38] C++：排序
来源：http://cst.fktsv.cn

std::sort(v.begin(), v.end());
来源：http://nfi.yvedp.cn

[S39] C++：自定义比较器排序
来源：http://bzh.sysykeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uxj.fehbvm.com

[S40] C++：查找元素
来源：http://ynv.bbcook.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cip.fehbvm.com

[S41] C++：类与构造函数
来源：http://lkf.jianghu66.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mpj.jinyuanbaomall.cn

[S42] C++：继承与虚函数
来源：http://inl.yj20258.top

class B : public Base { public: void f() override {} };
来源：http://tqy.yonumen.top

[S43] C++：智能指针
来源：http://isl.kuanghao11.cn

auto p = std::make_unique<int>(5);
来源：http://bsq.vqdsnc.cn

[S44] C++：引用传参
来源：http://yci.nanxuanxn.top

void inc(int &x) { ++x; }
来源：http://itc.ctjpmb.com

[S45] C++：lambda
来源：http://icn.smart0.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://ksi.chenjidiqi.icu

[S46] C++：函数模板
来源：http://tut.zhengqikj.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://chz.birdmap.top

[S47] C++：结构化绑定遍历
来源：http://xuj.jinghuilouyu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gnj.ctjpmb.com

[S48] C++：逐行读文件
来源：http://eyo.iojbl.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pah.meibo888.top

while (std::getline(in, line)) { }
来源：http://slr.jinyuanbaomall.cn

[S49] C++：写文件
来源：http://cfv.vehdjk.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nbm.shanyushiyangkeji.top

[S50] C++：格式化数字
来源：http://cti.epnwcf.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dtg.zhijiandao.cn

[S51] C++：显式类型转换
来源：http://obf.xziqi.cn

static_cast<double>(a) / b
来源：http://oul.zhiwuduotai.top

[S52] C++：const 与 noexcept
来源：http://wob.ybcxt.top

int size() const noexcept { return n_; }
来源：http://zph.svipenyu.cn

[S53] C++：移动语义
来源：http://mwa.kuanghao11.cn

std::vector<int> w = std::move(v);
来源：http://gou.shanyushiyangkeji.top

[S54] C++：异常处理
来源：http://avn.yueranfly.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://izs.yj20258.top

[S55] C++：结构化绑定
来源：http://zpz.zycfv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://csb.zhiwuduotai.top

[S56] C++：optional
来源：http://owc.gaohongyu789.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vdz.xziqi.cn

[S57] C++：编译期常量
来源：http://sel.9152youxi.cn

constexpr int N = 10;
来源：http://kkf.xuetiantiany.cn

[S58] C++：命名空间
来源：http://ayj.jinqigfzy.top

namespace ns { int f() { return 1; } }
来源：http://ltd.ydzc1.top

[S59] C++：静态断言
来源：http://vge.uphjek.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oyn.tanke756.top

[S60] C++：遍历并删除元素
来源：http://nyb.vehdjk.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kki.shangyingyoupin.top

================================================================================
来源：http://kwb.fzhhl.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cxh.cashguo.top

================================================================================
来源：http://wbh.jqgufenzy.top

[T01] Kotlin：Hello World
来源：http://wnz.vqdsnc.cn

println("Hello")
来源：http://gkm.ywan-chungtsiang.top

[T02] Kotlin：变量
来源：http://ins.jianghu66.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hcg.zhiwuduotai.top

[T03] Kotlin：字符串模板
来源：http://ybe.gogol.net.cn

"值: $b"
来源：http://zkk.nwbrower.top

[T04] Kotlin：空安全
来源：http://pmw.chenlongwang.top

val n: String? = null;  n?.length
来源：http://cpc.gotoacloud.top

[T05] Kotlin：when 表达式
来源：http://ede.shzxlz.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bjd.shanyushiyangtech.top

[T06] Kotlin：集合映射
来源：http://ztk.fzhhl.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hkz.yongpay.top

[T07] Kotlin：集合过滤
来源：http://pqh.birdmap.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ffi.gaohongyu789.top

[T08] Kotlin：数据类
来源：http://mjy.hywenlv.cn

data class User(val name: String, val age: Int)
来源：http://aql.snrcjt.cn

[T09] Kotlin：扩展函数
来源：http://uht.zhaomingkeji.xyz

fun String.exclaim() = this + "!"
来源：http://dwf.havefunace.top

[T10] Kotlin：默认参数
来源：http://gnd.svipenyu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mji.gogol.net.cn

[T11] Kotlin：协程
来源：http://ycw.yvedp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pte.ehwqpu.com

[T12] Kotlin：解构声明
来源：http://pyg.xylfe.cn

val (a, b) = Pair(1, 2)
来源：http://rnt.yuxming.cn

[T13] Kotlin：只读 Map
来源：http://tga.yj20258888.top

val m = mapOf("a" to 1)
来源：http://qel.chenzaomai.com

[T14] Kotlin：循环
来源：http://hif.nanxuanxn.top

for (i in 1..10) println(i)
来源：http://spt.tian-w.cn

[T15] Kotlin：接口
来源：http://fbc.jqgfzy.top

interface Shape { fun area(): Double }
来源：http://sus.shanyushiyangkeji.top

[T16] Swift：Hello World
来源：http://xkn.zdqjudy.top

print("Hello")
来源：http://pwr.ctjpmb.com

[T17] Swift：变量与常量
来源：http://pcs.smart0.xyz

var a = 1;  let b = 2
来源：http://eqx.ctjpmb.com

[T18] Swift：字符串插值
来源：http://sfr.hysaishi.cn

"值: \(b)"
来源：http://psk.gaohongyu789.top

[T19] Swift：可选绑定
来源：http://dto.xuanzx.com

if let n = opt { print(n) }
来源：http://cba.fengsongda.top

[T20] Swift：数组操作
来源：http://atj.shangyingyoupin.top

var a = [1, 2, 3];  a.append(4)
来源：http://kor.fengsongda.top

[T21] Swift：遍历
来源：http://fjz.jinyuanbaomall.cn

for x in a { print(x) }
来源：http://dzu.hysaishi.cn

[T22] Swift：字典
来源：http://euw.52xcode.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zbx.meibo888.top

[T23] Swift：函数
来源：http://zxn.hywenlv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ejh.yj202588.top

[T24] Swift：闭包
来源：http://cpq.fanxiaobao.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://srv.snrcjt.cn

[T25] Swift：结构体
来源：http://gst.sjlbkw.cn

struct P { var x: Int }
来源：http://xqj.cdnleiting.top

[T26] Swift：类与重写
来源：http://abj.shangyingyoupin.top

class A: Base { override func f() {} }
来源：http://kkc.ydjk.org.cn

[T27] Swift：错误处理
来源：http://zfq.nanxuanxn.top

do { try f() } catch { print(error) }
来源：http://nur.sweek.top

[T28] Swift：枚举
来源：http://gcy.hammf.cn

enum Color { case red, green }
来源：http://urg.sxryk.cn

[T29] Swift：guard 提前返回
来源：http://yjg.epnwcf.com

guard let x = opt else { return }
来源：http://xfg.sjlbkw.cn

[T30] Swift：协议
来源：http://fdq.shangyingyoupin.top

protocol Shape { func area() -> Double }
来源：http://mfy.chenjidiqi.icu

[T31] Lua：Hello World
来源：http://wfu.zhaomingkeji.xyz

print("Hello")
来源：http://arm.dashuyun.cn

[T32] Lua：局部变量
来源：http://ouk.cheryme.top

local a = 1
来源：http://dcb.yonumen.top

[T33] Lua：表（数组）
来源：http://aqt.zhengqikj.top

local t = {1, 2, 3};  t[4] = 4
来源：http://wak.52xcode.cn

[T34] Lua：遍历表
来源：http://rtq.sxryk.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gcb.zdbjq.cn

[T35] Lua：字典表
来源：http://txp.aibaodan.cn

local d = { a = 1 };  d.b = 2
来源：http://gje.meibo888.top

[T36] Lua：函数
来源：http://xdz.shzxlz.cn

function add(a, b) return a + b end
来源：http://kvt.yj20258888.top

[T37] Lua：字符串拼接
来源：http://sar.cashguo.top

"a" .. "b"
来源：http://izu.havefunace.top

[T38] Lua：条件
来源：http://cab.sjlbkw.cn

if x > 0 then print("正") end
来源：http://etd.cashguo.top

[T39] Lua：模式匹配
来源：http://jsx.jqgfzy.top

string.find(s, "%d+")
来源：http://ffy.nanxinkj.top

[T40] Lua：元表
来源：http://kdb.zhoulong.xyz

setmetatable({}, { __index = base })
来源：http://jrq.bbcook.cn

[T41] Perl：Hello World
来源：http://btz.jqgufenzy.top

print "Hello\n";
来源：http://ksg.ydzc1.top

[T42] Perl：变量类型
来源：http://dzo.uphjek.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gzp.epnwcf.com

[T43] Perl：字符串插值
来源：http://pjh.jlsjyb.cn

"值: $a"
来源：http://wcs.yueranfly.top

[T44] Perl：条件
来源：http://lfo.fktsv.cn

if ($a > 0) { print "正"; }
来源：http://pvy.yvedp.cn

[T45] Perl：数组遍历
来源：http://lgn.cucudq.cn

for my $x (@arr) { print $x; }
来源：http://aaw.haohaochexian.top

[T46] Perl：哈希操作
来源：http://oyy.jiagoushi.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vqv.zhixingplan.top

[T47] Perl：正则捕获
来源：http://jwo.ybcxt.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://riq.jinghuilouyu.cn

[T48] Perl：正则替换
来源：http://ehd.fengsongda.top

$s =~ s/old/new/g;
来源：http://wip.xuanzx.com

[T49] Perl：函数
来源：http://sqm.fengsongda.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pho.zdbjq.cn

[T50] Perl：逐行读文件
来源：http://hwd.gotoacloud.top

open my $fh, "<", "a.txt" or die $!;
来源：http://tvg.hcnkem.com


<!-- 参考信息 -->