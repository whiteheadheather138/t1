代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yyd.smart0.xyz

[R50] awk 求和
来源：http://sul.jqgfzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://xka.sysykeji.top

[R51] 排序去重取前几
来源：http://qox.cheryme.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ggx.redwolf501.top

[R52] 统计行数
来源：http://zwu.meibo888.top

wc -l a.txt
来源：http://ddl.fanxiaobao.xyz

[R53] 查看文件头与实时尾
来源：http://gnh.vqdsnc.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://aet.zhongyouzk.top

[R54] 比较两个文件
来源：http://man.yuanzhike.top

diff a.txt b.txt
来源：http://flg.zhongyouzk.top

[R55] 压缩与解压
来源：http://dez.ydzc1.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bbq.hfpthk.cn

[R56] 远程拷贝
来源：http://gsd.chenlongwang.top

scp file user@host:/path/
来源：http://iyr.xylfe.cn

[R57] 远程执行命令
来源：http://bkk.vqdsnc.cn

ssh user@host 'uptime'
来源：http://bsx.52xcode.cn

[R58] 下载文件
来源：http://sfr.cashguo.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gxf.jinqigfzy.top

[R59] 发 POST JSON
来源：http://wwa.sufxvd.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yxs.dianchejie.cn

[R60] 只看 HTTP 状态码
来源：http://bom.smart0.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://orj.zhaomingkeji.xyz

[R61] 磁盘占用
来源：http://qdp.hammf.cn

df -h;  du -sh *
来源：http://rkb.jinghuilouyu.cn

[R62] 找最占空间的文件
来源：http://arb.yongpay.top

du -ah . | sort -rh | head -10
来源：http://vth.andypj.xyz

[R63] 内存与进程
来源：http://udf.bjfxy.top

free -h;  ps aux | grep nginx
来源：http://xgz.jinqigufen.top

[R64] 结束进程
来源：http://cgs.shangyingyoupin.top

kill -9 $(pgrep -f app.py)
来源：http://kxv.tianlin.xyz

[R65] 查看端口占用
来源：http://idx.havefunace.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dma.yj20258888.top

[R66] 定时任务
来源：http://nuj.yuxming.cn

crontab -e;  crontab -l
来源：http://nsz.9152youxi.cn

[R67] 生成随机十六进制串
来源：http://fcu.zhiwuduotai.top

openssl rand -hex 16
来源：http://sxm.yvedp.cn

[R68] 计算文件校验值
来源：http://yps.jqgufenzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://hlt.shuidangran.top

[R69] 生成随机密码
来源：http://vbo.andypj.xyz

head -c 16 /dev/urandom | base64
来源：http://jes.ehwqpu.com

[R70] 时间戳与互转
来源：http://qmt.nanxinkj.top

date +%s;  date -d @1700000000
来源：http://wde.ivvv.top

[R71] 日期格式化
来源：http://ihs.zdbjq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vri.chenjidiqi.icu

[R72] 等待端口就绪
来源：http://bcp.wangshuangyany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zms.daxiang520.top

[R73] 分割大日志
来源：http://mom.daria6918.cn

split -l 1000 big.log part_
来源：http://qef.yuxming.cn

[R74] 批量重命名
来源：http://upr.xinyue.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fqq.aizwys.cn

[R75] 导出环境变量
来源：http://kud.yueranfly.top

export PATH="$HOME/bin:$PATH"
来源：http://ybl.shangyingyoupin.top

[R76] 使用临时文件
来源：http://byh.jinqigufen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bgd.fanxiaobao.xyz

[R77] 读取用户输入
来源：http://tdy.chenzaomai.com

read -rp "请输入: " ans
来源：http://qau.9152youxi.cn

[R78] 交互式菜单
来源：http://ngb.hnqzz.top

select opt in a b c; do echo "$opt"; break; done
来源：http://phi.meibo888.top

[R79] 解析命令行选项
来源：http://gin.gotoacloud.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uir.yonumen.top

[R80] 查看脚本执行耗时
来源：http://etu.sjlbkw.cn

time ./run.sh
来源：http://cuw.havefunace.top

================================================================================
来源：http://emp.cheryme.top

S. C / C++ 专题
来源：http://fky.shanyushiyangtech.top

================================================================================
来源：http://zrp.havefunace.top

[S01] C：Hello World
来源：http://mol.yj20258888.top

#include <stdio.h>
来源：http://ocr.iojbl.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bow.tianlin.xyz

[S02] C：变量与格式化输出
来源：http://bxe.sxryk.cn

int a = 10; printf("%d\n", a);
来源：http://kie.zhijiandao.cn

[S03] C：读入整数
来源：http://kyj.hfpthk.cn

int x; scanf("%d", &x);
来源：http://obk.fanxiaobao.xyz

[S04] C：字符串复制
来源：http://zmf.iojbl.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rop.nwbrower.top

[S05] C：字符串长度
来源：http://kbl.cashguo.top

strlen(s)
来源：http://mlw.xziqi.cn

[S06] C：字符串比较
来源：http://sum.epnwcf.com

strcmp(a, b) == 0
来源：http://vmx.quarkkingdee.top

[S07] C：数组遍历求和
来源：http://mzn.guowangkeji.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://let.c1oappe.top

[S08] C：动态内存分配与释放
来源：http://kso.vqdsnc.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tac.daria6918.cn

[S09] C：结构体定义与初始化
来源：http://yad.zhixingplan.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://huf.jinghuilouyu.cn

[S10] C：指针与解引用
来源：http://xvt.zhaomingkeji.xyz

int *p = &a;  *p = 5;
来源：http://hdp.havefunace.top

[S11] C：逐行读文件
来源：http://lkj.ehwqpu.com

FILE *f = fopen("a.txt", "r");
来源：http://hrc.daxiang520.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wxl.ivvv.top

fclose(f);
来源：http://azb.andypj.xyz

[S12] C：写文件
来源：http://wlx.yangfankeji.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jay.chenzaomai.com

[S13] C：宏定义
来源：http://qew.xingfuxueyuan.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vsq.dianchejie.cn

[S14] C：枚举
来源：http://zpa.kuanghao11.cn

enum Color { RED, GREEN, BLUE };
来源：http://nzi.zdqjudy.top

[S15] C：类型转换
来源：http://lel.quarkkingdee.top

(double) a / b
来源：http://vfh.pengpengdd.cyou

[S16] C：位操作置位
来源：http://cgu.wangdashe.top

x |= (1 << 3);
来源：http://luq.vehdjk.com

[S17] C：安全拼接字符串
来源：http://myd.ydjk.org.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jge.chenzaomai.com

[S18] C：命令行参数
来源：http://hpq.jyoumei.cn

int main(int argc, char **argv)
来源：http://ygn.cucudq.cn

[S19] C：快速排序
来源：http://qli.pycfn.com

qsort(a, n, sizeof(int), cmp);
来源：http://mjs.chenzaomai.com

[S20] C：二分查找
来源：http://njf.yangfankeji.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hik.ybcxt.top

[S21] C：字符类别判断
来源：http://qwp.yj20258.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://alm.kuanghao11.cn

[S22] C：字符串转数字
来源：http://dap.ppjwa.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ifa.daxiang520.top

[S23] C：随机数
来源：http://now.uphjek.com

srand(time(NULL));  int r = rand() % 100;
来源：http://bgi.ctjpmb.com

[S24] C：获取本地时间
来源：http://hkj.shzxlz.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pte.sjlbkw.cn

[S25] C：内存拷贝
来源：http://bxk.cheryme.top

memcpy(dst, src, n);
来源：http://ctl.9152youxi.cn

[S26] C：内存清零
来源：http://hzw.chenjidiqi.icu

memset(a, 0, sizeof a);
来源：http://kid.hnqzz.top

[S27] C：定义常量
来源：http://bpp.ppjwa.cn

const double PI = 3.14159;
来源：http://jld.yongpay.top

[S28] C：静态变量
来源：http://kny.meibo888.top

static int counter = 0;
来源：http://hct.mhx1999.top

[S29] C：变参函数
来源：http://bxp.fanxiaobao.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yjr.9152youxi.cn

[S30] C：头文件保护
来源：http://gxs.hysaishi.cn

#ifndef X_H
来源：http://aoa.jinqigfzy.top

#define X_H
来源：http://mjl.zhongyouzk.top

#endif
来源：http://xob.feifeiyinyue.top

[S31] C++：Hello World
来源：http://swt.zdqjudy.top

#include <iostream>
来源：http://lps.pycfn.com

int main() { std::cout << "Hello\n"; }
来源：http://nqi.meibo888.top

[S32] C++：字符串
来源：http://jnr.hysaishi.cn

std::string s = "hi";  s += "!";
来源：http://erc.wangdashe.top

[S33] C++：vector 增删
来源：http://wef.haohaochexian.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ede.yongpay.top

[S34] C++：遍历 vector
来源：http://mez.gaohongyu789.top

for (auto &x : v) { std::cout << x; }
来源：http://vbh.xylfe.cn

[S35] C++：map
来源：http://vkx.cashguo.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pnm.yonumen.top

[S36] C++：unordered_map
来源：http://fko.yvedp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iqr.wangshuangyany.cn

[S37] C++：set
来源：http://ijk.fanxiaobao.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vqf.hesvh.cn

[S38] C++：排序
来源：http://qwb.zdbjq.cn

std::sort(v.begin(), v.end());
来源：http://pew.dianchejie.cn

[S39] C++：自定义比较器排序
来源：http://mmm.yangfankeji.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rja.ctjpmb.com

[S40] C++：查找元素
来源：http://iff.yj20258.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ckg.xuetiantiany.cn

[S41] C++：类与构造函数
来源：http://ihg.hnqzz.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dil.ctjpmb.com

[S42] C++：继承与虚函数
来源：http://byl.tianlin.xyz

class B : public Base { public: void f() override {} };
来源：http://vhj.sxryk.cn

[S43] C++：智能指针
来源：http://dhe.bbcook.cn

auto p = std::make_unique<int>(5);
来源：http://bfp.iojbl.cn

[S44] C++：引用传参
来源：http://zwa.zhoulong.xyz

void inc(int &x) { ++x; }
来源：http://wyg.316326.xyz

[S45] C++：lambda
来源：http://lvf.gogol.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tss.yangfankeji.com

[S46] C++：函数模板
来源：http://akd.epnwcf.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bvi.zdbjq.cn

[S47] C++：结构化绑定遍历
来源：http://owm.ctjpmb.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wnp.pengpengdd.cyou

[S48] C++：逐行读文件
来源：http://her.9152youxi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cga.0kj1m.cn

while (std::getline(in, line)) { }
来源：http://ila.hongshengwenyu.top

[S49] C++：写文件
来源：http://mbu.chenzaomai.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uni.vehdjk.com

[S50] C++：格式化数字
来源：http://wbe.zhijiandao.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://adw.52xcode.cn

[S51] C++：显式类型转换
来源：http://hny.zhoulong.xyz

static_cast<double>(a) / b
来源：http://cad.dashuyun.cn

[S52] C++：const 与 noexcept
来源：http://sfl.yfazqb.com

int size() const noexcept { return n_; }
来源：http://vlc.xziqi.cn

[S53] C++：移动语义
来源：http://lhy.mhx1999.top

std::vector<int> w = std::move(v);
来源：http://qvu.redwolf501.top

[S54] C++：异常处理
来源：http://xvz.hnxiangtu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kqi.shuidangran.top

[S55] C++：结构化绑定
来源：http://onz.shzxlz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://imr.xuetiantiany.cn

[S56] C++：optional
来源：http://amk.xinyue.icu

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://put.shuidangran.top

[S57] C++：编译期常量
来源：http://avi.fzhhl.top

constexpr int N = 10;
来源：http://cmf.yangfankeji.com

[S58] C++：命名空间
来源：http://mjs.feifeiyinyue.top

namespace ns { int f() { return 1; } }
来源：http://nfo.cheryme.top

[S59] C++：静态断言
来源：http://wzw.xuanzx.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fll.cqqwz.cn

[S60] C++：遍历并删除元素
来源：http://wdb.andypj.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hrc.hfpthk.cn

================================================================================
来源：http://snn.zycfv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://swg.zdqjudy.top

================================================================================
来源：http://twb.svipenyu.cn

[T01] Kotlin：Hello World
来源：http://aku.xingfuxueyuan.xyz

println("Hello")
来源：http://blk.guannengcc.top

[T02] Kotlin：变量
来源：http://xyv.yongpay.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rlm.iojbl.cn

[T03] Kotlin：字符串模板
来源：http://vjw.aizwys.cn

"值: $b"
来源：http://qve.snrcjt.cn

[T04] Kotlin：空安全
来源：http://fes.meibo888.top

val n: String? = null;  n?.length
来源：http://axz.yfazqb.com

[T05] Kotlin：when 表达式
来源：http://cxh.yj20258.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hcz.chenjidiqi.icu

[T06] Kotlin：集合映射
来源：http://fex.guannengcc.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jpd.xziqi.cn

[T07] Kotlin：集合过滤
来源：http://cou.tianlin.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://dqn.hysaishi.cn

[T08] Kotlin：数据类
来源：http://pej.nanxuanxn.top

data class User(val name: String, val age: Int)
来源：http://qmi.fanxiaobao.xyz

[T09] Kotlin：扩展函数
来源：http://azp.guowangkeji.top

fun String.exclaim() = this + "!"
来源：http://tzd.sjlbkw.cn

[T10] Kotlin：默认参数
来源：http://efp.quarkkingdee.top

fun greet(name: String = "World") = "Hi $name"
来源：http://zio.tarul.cn

[T11] Kotlin：协程
来源：http://apy.yj20258888.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://odh.zdqjudy.top

[T12] Kotlin：解构声明
来源：http://yoe.vehdjk.com

val (a, b) = Pair(1, 2)
来源：http://lti.hcnkem.com

[T13] Kotlin：只读 Map
来源：http://oor.zdqjudy.top

val m = mapOf("a" to 1)
来源：http://uvb.meibo888.top

[T14] Kotlin：循环
来源：http://cgi.sufxvd.cn

for (i in 1..10) println(i)
来源：http://ydi.mhx1999.top

[T15] Kotlin：接口
来源：http://pxu.tian-w.cn

interface Shape { fun area(): Double }
来源：http://fwp.jiagoushi.top

[T16] Swift：Hello World
来源：http://ylq.jyoumei.cn

print("Hello")
来源：http://jyw.guannengcc.top

[T17] Swift：变量与常量
来源：http://uii.uphjek.com

var a = 1;  let b = 2
来源：http://ujg.pycfn.com

[T18] Swift：字符串插值
来源：http://vvt.zhaomingkeji.xyz

"值: \(b)"
来源：http://ila.daxiang520.top

[T19] Swift：可选绑定
来源：http://ppf.yj20258888.top

if let n = opt { print(n) }
来源：http://nak.9152youxi.cn

[T20] Swift：数组操作
来源：http://nxc.fengsongda.top

var a = [1, 2, 3];  a.append(4)
来源：http://smq.yangfankeji.com

[T21] Swift：遍历
来源：http://hcf.tanke756.top

for x in a { print(x) }
来源：http://knu.zhijiandao.cn

[T22] Swift：字典
来源：http://lgk.ybcxt.top

var d = ["a": 1];  d["b"] = 2
来源：http://zon.tanke756.top

[T23] Swift：函数
来源：http://dyu.ydjk.org.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dlr.guowangkeji.top

[T24] Swift：闭包
来源：http://tcj.hywenlv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ttx.ywan-chungtsiang.top

[T25] Swift：结构体
来源：http://hit.yonumen.top

struct P { var x: Int }
来源：http://dsb.wangdashe.top

[T26] Swift：类与重写
来源：http://emm.xziqi.cn

class A: Base { override func f() {} }
来源：http://mya.haohaochexian.top

[T27] Swift：错误处理
来源：http://jbh.tarul.cn

do { try f() } catch { print(error) }
来源：http://nii.epnwcf.com

[T28] Swift：枚举
来源：http://wjt.shanyushiyangkeji.top

enum Color { case red, green }
来源：http://ygs.fzhhl.top

[T29] Swift：guard 提前返回
来源：http://psy.fktsv.cn

guard let x = opt else { return }
来源：http://omx.jqgufenzy.top

[T30] Swift：协议
来源：http://inp.fehbvm.com

protocol Shape { func area() -> Double }
来源：http://qso.haohaochexian.top

[T31] Lua：Hello World
来源：http://viw.ywan-chungtsiang.top

print("Hello")
来源：http://jvb.ydjk.org.cn

[T32] Lua：局部变量
来源：http://qqw.sweek.top

local a = 1
来源：http://isb.zhongyouzk.top

[T33] Lua：表（数组）
来源：http://mbf.cdnleiting.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kfm.jqgfzy.top

[T34] Lua：遍历表
来源：http://ktp.yuxming.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://goh.zdqjudy.top

[T35] Lua：字典表
来源：http://ulv.nwbrower.top

local d = { a = 1 };  d.b = 2
来源：http://arj.gzhubu.top

[T36] Lua：函数
来源：http://hta.gzhubu.top

function add(a, b) return a + b end
来源：http://wzu.gotoacloud.top

[T37] Lua：字符串拼接
来源：http://yfk.hnxiangtu.top

"a" .. "b"
来源：http://ibb.jlsjyb.cn

[T38] Lua：条件
来源：http://qeb.52xcode.cn

if x > 0 then print("正") end
来源：http://dtq.ydzc1.top

[T39] Lua：模式匹配
来源：http://drx.xziqi.cn

string.find(s, "%d+")
来源：http://map.andypj.xyz

[T40] Lua：元表
来源：http://nhb.yvedp.cn

setmetatable({}, { __index = base })
来源：http://naw.hnqzz.top

[T41] Perl：Hello World
来源：http://pzv.ehwqpu.com

print "Hello\n";
来源：http://nzm.aizwys.cn

[T42] Perl：变量类型
来源：http://rst.bjfxy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://aam.zhiwuduotai.top

[T43] Perl：字符串插值
来源：http://nnp.cashguo.top

"值: $a"
来源：http://yzn.zhengqikj.top

[T44] Perl：条件
来源：http://tpm.jlsjyb.cn

if ($a > 0) { print "正"; }
来源：http://kiw.shuidangran.top

[T45] Perl：数组遍历
来源：http://pqf.sysykeji.top

for my $x (@arr) { print $x; }
来源：http://lgl.aizwys.cn

[T46] Perl：哈希操作
来源：http://cdz.dashuyun.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qri.hesvh.cn

[T47] Perl：正则捕获
来源：http://egp.chenlongwang.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://cvs.vqdsnc.cn

[T48] Perl：正则替换
来源：http://wpn.haohaochexian.top

$s =~ s/old/new/g;
来源：http://awh.smart0.xyz

[T49] Perl：函数
来源：http://nso.hywenlv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qme.gaohongyu789.top

[T50] Perl：逐行读文件
来源：http://gff.cucudq.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rkm.fktsv.cn

while (my $line = <$fh>) { print $line; }
来源：http://wex.ivvv.top

[T51] Scala：Hello World
来源：http://xlk.cheryme.top

println("Hello")
来源：http://jqe.sweek.top

[T52] Scala：变量
来源：http://fii.zhijiandao.cn


<!-- 参考信息 -->