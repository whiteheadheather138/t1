代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://eux.yuanzhike.top

[R50] awk 求和
来源：http://uyw.gzhubu.top

awk '{s += $2} END {print s}' a.txt
来源：http://zsv.bjfxy.top

[R51] 排序去重取前几
来源：http://six.tianlin.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://eln.nanxinkj.top

[R52] 统计行数
来源：http://otj.cheryme.top

wc -l a.txt
来源：http://dim.316326.xyz

[R53] 查看文件头与实时尾
来源：http://uie.zhixingplan.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ctz.tianlin.xyz

[R54] 比较两个文件
来源：http://osv.shanyushiyangtech.top

diff a.txt b.txt
来源：http://zev.epnwcf.com

[R55] 压缩与解压
来源：http://ava.zhoulong.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yug.jqgufenzy.top

[R56] 远程拷贝
来源：http://ece.yangfankeji.com

scp file user@host:/path/
来源：http://mpr.chenjidiqi.icu

[R57] 远程执行命令
来源：http://xkn.zdbjq.cn

ssh user@host 'uptime'
来源：http://jfy.52xcode.cn

[R58] 下载文件
来源：http://hgh.dianchejie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nxo.hesvh.cn

[R59] 发 POST JSON
来源：http://mkv.hnxiangtu.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kfn.epnwcf.com

[R60] 只看 HTTP 状态码
来源：http://vxo.hammf.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ymr.ehwqpu.com

[R61] 磁盘占用
来源：http://yga.yangfankeji.com

df -h;  du -sh *
来源：http://suk.ywan-chungtsiang.top

[R62] 找最占空间的文件
来源：http://zjp.yvedp.cn

du -ah . | sort -rh | head -10
来源：http://icg.nwbrower.top

[R63] 内存与进程
来源：http://wup.hysaishi.cn

free -h;  ps aux | grep nginx
来源：http://tpv.ehwqpu.com

[R64] 结束进程
来源：http://vvq.yuxming.cn

kill -9 $(pgrep -f app.py)
来源：http://exm.kuanghao11.cn

[R65] 查看端口占用
来源：http://vvz.svipenyu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tvm.zhijiandao.cn

[R66] 定时任务
来源：http://sjr.pycfn.com

crontab -e;  crontab -l
来源：http://zpy.uphjek.com

[R67] 生成随机十六进制串
来源：http://bsa.ppjwa.cn

openssl rand -hex 16
来源：http://nee.yvedp.cn

[R68] 计算文件校验值
来源：http://hpw.316326.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://zga.gogol.net.cn

[R69] 生成随机密码
来源：http://zby.iojbl.cn

head -c 16 /dev/urandom | base64
来源：http://kgp.zhixingplan.top

[R70] 时间戳与互转
来源：http://qtg.hysaishi.cn

date +%s;  date -d @1700000000
来源：http://hnj.hywenlv.cn

[R71] 日期格式化
来源：http://ils.chenlongwang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://juo.jyoumei.cn

[R72] 等待端口就绪
来源：http://wzp.bjfxy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://pdz.gaohongyu789.top

[R73] 分割大日志
来源：http://nnc.shzxlz.cn

split -l 1000 big.log part_
来源：http://oty.nanxinkj.top

[R74] 批量重命名
来源：http://zsg.bjfxy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pst.havefunace.top

[R75] 导出环境变量
来源：http://jcs.mhx1999.top

export PATH="$HOME/bin:$PATH"
来源：http://ypb.jqgfzy.top

[R76] 使用临时文件
来源：http://lev.aibaodan.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qlb.pycfn.com

[R77] 读取用户输入
来源：http://nrm.yueranfly.top

read -rp "请输入: " ans
来源：http://yjo.nanxuanxn.top

[R78] 交互式菜单
来源：http://uzj.aibaodan.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lie.yj202588.top

[R79] 解析命令行选项
来源：http://nbe.hywenlv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zrh.quarkkingdee.top

[R80] 查看脚本执行耗时
来源：http://ent.cqqwz.cn

time ./run.sh
来源：http://qro.chenlongwang.top

================================================================================
来源：http://hvu.hywenlv.cn

S. C / C++ 专题
来源：http://yhs.pycfn.com

================================================================================
来源：http://yny.ydzc1.top

[S01] C：Hello World
来源：http://vag.zhoulong.xyz

#include <stdio.h>
来源：http://qhi.snrcjt.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kay.0kj1m.cn

[S02] C：变量与格式化输出
来源：http://etg.ehwqpu.com

int a = 10; printf("%d\n", a);
来源：http://fkf.hongshengwenyu.top

[S03] C：读入整数
来源：http://lqz.uphjek.com

int x; scanf("%d", &x);
来源：http://jda.tanke756.top

[S04] C：字符串复制
来源：http://fqm.shanyushiyangtech.top

char dst[32]; strcpy(dst, "hi");
来源：http://bty.cqqwz.cn

[S05] C：字符串长度
来源：http://vai.xuanzx.com

strlen(s)
来源：http://lhj.0kj1m.cn

[S06] C：字符串比较
来源：http://dsz.havefunace.top

strcmp(a, b) == 0
来源：http://cav.zhijiandao.cn

[S07] C：数组遍历求和
来源：http://gae.daria6918.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://acc.cucudq.cn

[S08] C：动态内存分配与释放
来源：http://ftv.dianchejie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://slx.yfazqb.com

[S09] C：结构体定义与初始化
来源：http://uea.chenjidiqi.icu

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bsk.zhixingplan.top

[S10] C：指针与解引用
来源：http://uzb.iojbl.cn

int *p = &a;  *p = 5;
来源：http://osk.hammf.cn

[S11] C：逐行读文件
来源：http://obq.zycfv.cn

FILE *f = fopen("a.txt", "r");
来源：http://onx.cqqwz.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yap.hysaishi.cn

fclose(f);
来源：http://cdj.dashuyun.cn

[S12] C：写文件
来源：http://oir.cheryme.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jus.zdbjq.cn

[S13] C：宏定义
来源：http://doi.xinyue.icu

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gfe.epnwcf.com

[S14] C：枚举
来源：http://rls.hnxiangtu.top

enum Color { RED, GREEN, BLUE };
来源：http://xmg.xuetiantiany.cn

[S15] C：类型转换
来源：http://lde.zdbjq.cn

(double) a / b
来源：http://vpx.gotoacloud.top

[S16] C：位操作置位
来源：http://jbk.zycfv.cn

x |= (1 << 3);
来源：http://suy.jqgfzy.top

[S17] C：安全拼接字符串
来源：http://hut.gaohongyu789.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tza.zdbjq.cn

[S18] C：命令行参数
来源：http://rek.hysaishi.cn

int main(int argc, char **argv)
来源：http://obp.hcnkem.com

[S19] C：快速排序
来源：http://men.yuanzhike.top

qsort(a, n, sizeof(int), cmp);
来源：http://ksl.sxryk.cn

[S20] C：二分查找
来源：http://puy.aibaodan.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://doh.andypj.xyz

[S21] C：字符类别判断
来源：http://tah.zhiwuduotai.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lxi.yj202588.top

[S22] C：字符串转数字
来源：http://yiu.aibaodan.cn

atoi("42");  strtod("3.14", NULL);
来源：http://inv.feifeiyinyue.top

[S23] C：随机数
来源：http://jay.shangyingyoupin.top

srand(time(NULL));  int r = rand() % 100;
来源：http://lez.vqdsnc.cn

[S24] C：获取本地时间
来源：http://mvb.jinqigufen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sip.hcnkem.com

[S25] C：内存拷贝
来源：http://pac.yonumen.top

memcpy(dst, src, n);
来源：http://cxj.guannengcc.top

[S26] C：内存清零
来源：http://dek.ybcxt.top

memset(a, 0, sizeof a);
来源：http://nra.birdmap.top

[S27] C：定义常量
来源：http://tgr.hongshengwenyu.top

const double PI = 3.14159;
来源：http://foe.xuetiantiany.cn

[S28] C：静态变量
来源：http://umt.guowangkeji.top

static int counter = 0;
来源：http://fgh.aibaodan.cn

[S29] C：变参函数
来源：http://mpu.jinqigufen.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sks.zhaomingkeji.xyz

[S30] C：头文件保护
来源：http://skr.ydzc1.top

#ifndef X_H
来源：http://jwl.jinqigfzy.top

#define X_H
来源：http://aau.xylfe.cn

#endif
来源：http://qej.aizwys.cn

[S31] C++：Hello World
来源：http://jim.yanxiufei.cn

#include <iostream>
来源：http://ctp.quarkkingdee.top

int main() { std::cout << "Hello\n"; }
来源：http://vxv.hywenlv.cn

[S32] C++：字符串
来源：http://ysy.shanyushiyangtech.top

std::string s = "hi";  s += "!";
来源：http://weq.gaohongyu789.top

[S33] C++：vector 增删
来源：http://qkj.wangdashe.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xtb.wangdashe.top

[S34] C++：遍历 vector
来源：http://ami.pengpengdd.cyou

for (auto &x : v) { std::cout << x; }
来源：http://qde.shanyushiyangtech.top

[S35] C++：map
来源：http://tei.fehbvm.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uwy.bbcook.cn

[S36] C++：unordered_map
来源：http://pak.nanxuanxn.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://utw.shanyushiyangtech.top

[S37] C++：set
来源：http://gmg.uphjek.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yvo.shanyushiyangtech.top

[S38] C++：排序
来源：http://izo.hcnkem.com

std::sort(v.begin(), v.end());
来源：http://pql.yj20258.top

[S39] C++：自定义比较器排序
来源：http://zfa.sxryk.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ozu.tanke756.top

[S40] C++：查找元素
来源：http://sld.ivvv.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tik.hammf.cn

[S41] C++：类与构造函数
来源：http://qtw.ydzc1.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dyg.yueranfly.top

[S42] C++：继承与虚函数
来源：http://hso.daria6918.cn

class B : public Base { public: void f() override {} };
来源：http://pge.vqdsnc.cn

[S43] C++：智能指针
来源：http://thf.0kj1m.cn

auto p = std::make_unique<int>(5);
来源：http://qdf.iojbl.cn

[S44] C++：引用传参
来源：http://qgy.tanke756.top

void inc(int &x) { ++x; }
来源：http://iva.bjfxy.top

[S45] C++：lambda
来源：http://qwq.shanyushiyangkeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://wiw.birdmap.top

[S46] C++：函数模板
来源：http://ajv.hysaishi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xzn.epnwcf.com

[S47] C++：结构化绑定遍历
来源：http://cov.epnwcf.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sto.iojbl.cn

[S48] C++：逐行读文件
来源：http://yge.guowangkeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://ivx.tarul.cn

while (std::getline(in, line)) { }
来源：http://fzw.yuanzhike.top

[S49] C++：写文件
来源：http://sjg.vqdsnc.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jnc.xziqi.cn

[S50] C++：格式化数字
来源：http://vid.jianghu66.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://plw.zhixingplan.top

[S51] C++：显式类型转换
来源：http://woq.sxryk.cn

static_cast<double>(a) / b
来源：http://iwy.sjlbkw.cn

[S52] C++：const 与 noexcept
来源：http://cfq.zhengqikj.top

int size() const noexcept { return n_; }
来源：http://mol.yuxming.cn

[S53] C++：移动语义
来源：http://akn.smart0.xyz

std::vector<int> w = std::move(v);
来源：http://ehg.dashuyun.cn

[S54] C++：异常处理
来源：http://ibw.ywan-chungtsiang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bdd.ybcxt.top

[S55] C++：结构化绑定
来源：http://qgs.fehbvm.com

auto [a, b] = std::make_pair(1, 2);
来源：http://bhu.xylfe.cn

[S56] C++：optional
来源：http://zxs.shanyushiyangkeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uip.feifeiyinyue.top

[S57] C++：编译期常量
来源：http://ujy.chenlongwang.top

constexpr int N = 10;
来源：http://yay.zhongyouzk.top

[S58] C++：命名空间
来源：http://hdu.jiagoushi.top

namespace ns { int f() { return 1; } }
来源：http://hvm.iojbl.cn

[S59] C++：静态断言
来源：http://jzs.kuanghao11.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wid.yvedp.cn

[S60] C++：遍历并删除元素
来源：http://hyo.sysykeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vpp.hnxiangtu.top

================================================================================
来源：http://gll.yfazqb.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ado.nanxinkj.top

================================================================================
来源：http://dte.yueranfly.top

[T01] Kotlin：Hello World
来源：http://szz.zhengqikj.top

println("Hello")
来源：http://kfb.chenjidiqi.icu

[T02] Kotlin：变量
来源：http://mud.chenzaomai.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ojv.tianlin.xyz

[T03] Kotlin：字符串模板
来源：http://siy.zhongyouzk.top

"值: $b"
来源：http://nvd.hfpthk.cn

[T04] Kotlin：空安全
来源：http://azy.svipenyu.cn

val n: String? = null;  n?.length
来源：http://jto.jianghu66.top

[T05] Kotlin：when 表达式
来源：http://mas.mhx1999.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://oaq.shzxlz.cn

[T06] Kotlin：集合映射
来源：http://qxy.nanxuanxn.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ewg.zhengqikj.top

[T07] Kotlin：集合过滤
来源：http://akp.fktsv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://izz.tianlin.xyz

[T08] Kotlin：数据类
来源：http://xvm.meibo888.top

data class User(val name: String, val age: Int)
来源：http://rku.yuxming.cn

[T09] Kotlin：扩展函数
来源：http://nkv.meibo888.top

fun String.exclaim() = this + "!"
来源：http://emi.ybcxt.top

[T10] Kotlin：默认参数
来源：http://kue.sxryk.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vod.sufxvd.cn

[T11] Kotlin：协程
来源：http://ivc.zdbjq.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jeq.hammf.cn

[T12] Kotlin：解构声明
来源：http://aif.jiagoushi.top

val (a, b) = Pair(1, 2)
来源：http://znn.xuetiantiany.cn

[T13] Kotlin：只读 Map
来源：http://fal.pengpengdd.cyou

val m = mapOf("a" to 1)
来源：http://kia.tanke756.top

[T14] Kotlin：循环
来源：http://vqh.ppjwa.cn

for (i in 1..10) println(i)
来源：http://szo.gogol.net.cn

[T15] Kotlin：接口
来源：http://rxo.vqdsnc.cn

interface Shape { fun area(): Double }
来源：http://orl.shangyingyoupin.top

[T16] Swift：Hello World
来源：http://mjy.smart0.xyz

print("Hello")
来源：http://yly.shzxlz.cn

[T17] Swift：变量与常量
来源：http://jkk.fengsongda.top

var a = 1;  let b = 2
来源：http://hkt.nanxinkj.top

[T18] Swift：字符串插值
来源：http://cco.hysaishi.cn

"值: \(b)"
来源：http://azk.ppjwa.cn

[T19] Swift：可选绑定
来源：http://dyf.0kj1m.cn

if let n = opt { print(n) }
来源：http://fhx.jqgufenzy.top

[T20] Swift：数组操作
来源：http://hwn.wangshuangyany.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lzt.sxryk.cn

[T21] Swift：遍历
来源：http://goe.cheryme.top

for x in a { print(x) }
来源：http://mfo.jiagoushi.top

[T22] Swift：字典
来源：http://ber.kuanghao11.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jua.ywan-chungtsiang.top

[T23] Swift：函数
来源：http://rce.aibaodan.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mxr.yuxming.cn

[T24] Swift：闭包
来源：http://wjt.zhengqikj.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://che.c1oappe.top

[T25] Swift：结构体
来源：http://qfm.tarul.cn

struct P { var x: Int }
来源：http://kaj.dianchejie.cn

[T26] Swift：类与重写
来源：http://imm.havefunace.top

class A: Base { override func f() {} }
来源：http://dyh.316326.xyz

[T27] Swift：错误处理
来源：http://zfw.fehbvm.com

do { try f() } catch { print(error) }
来源：http://glb.tanke756.top

[T28] Swift：枚举
来源：http://bzw.shanyushiyangkeji.top

enum Color { case red, green }
来源：http://cxn.zhengqikj.top

[T29] Swift：guard 提前返回
来源：http://sei.ppjwa.cn

guard let x = opt else { return }
来源：http://mqf.wangdashe.top

[T30] Swift：协议
来源：http://tcn.yvedp.cn

protocol Shape { func area() -> Double }
来源：http://gtq.nwbrower.top

[T31] Lua：Hello World
来源：http://nfs.jqgufenzy.top

print("Hello")
来源：http://gzx.pycfn.com

[T32] Lua：局部变量
来源：http://jjv.bbcook.cn

local a = 1
来源：http://vzm.cashguo.top

[T33] Lua：表（数组）
来源：http://wzv.sjlbkw.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fec.cheryme.top

[T34] Lua：遍历表
来源：http://rmo.yfazqb.com

for i, v in ipairs(t) do print(i, v) end
来源：http://owc.fktsv.cn

[T35] Lua：字典表
来源：http://bqh.9152youxi.cn

local d = { a = 1 };  d.b = 2
来源：http://jxi.redwolf501.top

[T36] Lua：函数
来源：http://gvk.zhijiandao.cn

function add(a, b) return a + b end
来源：http://wyc.ivvv.top

[T37] Lua：字符串拼接
来源：http://cgo.cqqwz.cn

"a" .. "b"
来源：http://zdd.yj202588.top

[T38] Lua：条件
来源：http://muk.hywenlv.cn

if x > 0 then print("正") end
来源：http://uco.andypj.xyz

[T39] Lua：模式匹配
来源：http://mcp.hcnkem.com

string.find(s, "%d+")
来源：http://lrp.hfpthk.cn

[T40] Lua：元表
来源：http://ews.epnwcf.com

setmetatable({}, { __index = base })
来源：http://lao.dianchejie.cn

[T41] Perl：Hello World
来源：http://rrg.quarkkingdee.top

print "Hello\n";
来源：http://zbj.yangfankeji.com

[T42] Perl：变量类型
来源：http://its.aizwys.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ktu.epnwcf.com

[T43] Perl：字符串插值
来源：http://sap.fanxiaobao.xyz

"值: $a"
来源：http://oed.kuanghao11.cn

[T44] Perl：条件
来源：http://lgl.jinghuilouyu.cn

if ($a > 0) { print "正"; }
来源：http://fyl.xuetiantiany.cn

[T45] Perl：数组遍历
来源：http://euo.wangshuangyany.cn

for my $x (@arr) { print $x; }
来源：http://opd.haohaochexian.top

[T46] Perl：哈希操作
来源：http://gwy.shzxlz.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dnd.hesvh.cn

[T47] Perl：正则捕获
来源：http://jjz.snrcjt.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hrf.shanyushiyangtech.top

[T48] Perl：正则替换
来源：http://ejh.epnwcf.com

$s =~ s/old/new/g;
来源：http://lza.zdbjq.cn

[T49] Perl：函数
来源：http://lza.daria6918.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ydm.zhengqikj.top

[T50] Perl：逐行读文件
来源：http://nga.jinqigfzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://qzo.xziqi.cn

while (my $line = <$fh>) { print $line; }
来源：http://cqk.gzhubu.top

[T51] Scala：Hello World
来源：http://vyp.jiagoushi.top

println("Hello")
来源：http://mpi.jyoumei.cn

[T52] Scala：变量
来源：http://rye.pycfn.com


<!-- 参考信息 -->