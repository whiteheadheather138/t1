代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://gzi.xingfuxueyuan.xyz

[R48] awk 取指定列
来源：http://rcz.yuxming.cn

awk '{print $1, $3}' a.txt
来源：http://vgf.zdqjudy.top

[R49] awk 带条件
来源：http://wgm.cqqwz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zyu.jyoumei.cn

[R50] awk 求和
来源：http://djt.zhongyouzk.top

awk '{s += $2} END {print s}' a.txt
来源：http://puf.316326.xyz

[R51] 排序去重取前几
来源：http://yox.cqqwz.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tni.sxryk.cn

[R52] 统计行数
来源：http://rqs.wangdashe.top

wc -l a.txt
来源：http://vdv.birdmap.top

[R53] 查看文件头与实时尾
来源：http://lxf.hysaishi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jtk.sysykeji.top

[R54] 比较两个文件
来源：http://noq.fengsongda.top

diff a.txt b.txt
来源：http://kjm.wangshuangyany.cn

[R55] 压缩与解压
来源：http://tfa.fengsongda.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://aqx.nwbrower.top

[R56] 远程拷贝
来源：http://mjn.hcnkem.com

scp file user@host:/path/
来源：http://bhq.ydzc1.top

[R57] 远程执行命令
来源：http://ccu.dianchejie.cn

ssh user@host 'uptime'
来源：http://afj.dianchejie.cn

[R58] 下载文件
来源：http://cdw.tianlin.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://doi.shanyushiyangtech.top

[R59] 发 POST JSON
来源：http://aiu.yueranfly.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fpi.feifeiyinyue.top

[R60] 只看 HTTP 状态码
来源：http://use.yangfankeji.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jtz.birdmap.top

[R61] 磁盘占用
来源：http://dkv.0kj1m.cn

df -h;  du -sh *
来源：http://tax.fktsv.cn

[R62] 找最占空间的文件
来源：http://bxf.yvedp.cn

du -ah . | sort -rh | head -10
来源：http://mkq.wangdashe.top

[R63] 内存与进程
来源：http://hnd.shanyushiyangkeji.top

free -h;  ps aux | grep nginx
来源：http://tmu.tanke756.top

[R64] 结束进程
来源：http://odx.pycfn.com

kill -9 $(pgrep -f app.py)
来源：http://jkv.iojbl.cn

[R65] 查看端口占用
来源：http://fjh.pengpengdd.cyou

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hkj.yvedp.cn

[R66] 定时任务
来源：http://ezf.sweek.top

crontab -e;  crontab -l
来源：http://yxr.jqgufenzy.top

[R67] 生成随机十六进制串
来源：http://zxp.hnqzz.top

openssl rand -hex 16
来源：http://qkb.fanxiaobao.xyz

[R68] 计算文件校验值
来源：http://qyb.kuanghao11.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cii.xuanzx.com

[R69] 生成随机密码
来源：http://htk.yanxiufei.cn

head -c 16 /dev/urandom | base64
来源：http://gcn.52xcode.cn

[R70] 时间戳与互转
来源：http://zzw.smart0.xyz

date +%s;  date -d @1700000000
来源：http://evn.zdqjudy.top

[R71] 日期格式化
来源：http://pwp.bbcook.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rqg.yongpay.top

[R72] 等待端口就绪
来源：http://xxz.fktsv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xec.iojbl.cn

[R73] 分割大日志
来源：http://wqg.xuetiantiany.cn

split -l 1000 big.log part_
来源：http://uzd.iojbl.cn

[R74] 批量重命名
来源：http://yeh.shangyingyoupin.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qqz.yueranfly.top

[R75] 导出环境变量
来源：http://wqg.smart0.xyz

export PATH="$HOME/bin:$PATH"
来源：http://hxi.xingfuxueyuan.xyz

[R76] 使用临时文件
来源：http://icm.tianlin.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lxf.xuetiantiany.cn

[R77] 读取用户输入
来源：http://kao.shanyushiyangkeji.top

read -rp "请输入: " ans
来源：http://dmq.tian-w.cn

[R78] 交互式菜单
来源：http://qei.andypj.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://ejv.yueranfly.top

[R79] 解析命令行选项
来源：http://jug.fehbvm.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xto.aizwys.cn

[R80] 查看脚本执行耗时
来源：http://hwj.quarkkingdee.top

time ./run.sh
来源：http://oxr.shuidangran.top

================================================================================
来源：http://dmt.cucudq.cn

S. C / C++ 专题
来源：http://ckh.yanxiufei.cn

================================================================================
来源：http://wgl.ydjk.org.cn

[S01] C：Hello World
来源：http://sck.vqdsnc.cn

#include <stdio.h>
来源：http://vis.hysaishi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zqh.uphjek.com

[S02] C：变量与格式化输出
来源：http://eai.sjlbkw.cn

int a = 10; printf("%d\n", a);
来源：http://pzl.jinqigufen.top

[S03] C：读入整数
来源：http://lun.hesvh.cn

int x; scanf("%d", &x);
来源：http://iug.yfazqb.com

[S04] C：字符串复制
来源：http://psl.fengsongda.top

char dst[32]; strcpy(dst, "hi");
来源：http://fks.yfazqb.com

[S05] C：字符串长度
来源：http://bjo.fanxiaobao.xyz

strlen(s)
来源：http://pzw.jqgfzy.top

[S06] C：字符串比较
来源：http://dbd.xylfe.cn

strcmp(a, b) == 0
来源：http://sno.jiagoushi.top

[S07] C：数组遍历求和
来源：http://gwe.zhongyouzk.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cvt.dianchejie.cn

[S08] C：动态内存分配与释放
来源：http://ayg.yj20258.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qdr.pycfn.com

[S09] C：结构体定义与初始化
来源：http://sek.jlsjyb.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kwm.xingfuxueyuan.xyz

[S10] C：指针与解引用
来源：http://ahc.yj20258.top

int *p = &a;  *p = 5;
来源：http://djg.svipenyu.cn

[S11] C：逐行读文件
来源：http://ciq.0kj1m.cn

FILE *f = fopen("a.txt", "r");
来源：http://kbz.52xcode.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://iun.chenlongwang.top

fclose(f);
来源：http://pmw.jianghu66.top

[S12] C：写文件
来源：http://afi.tarul.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vai.yueranfly.top

[S13] C：宏定义
来源：http://hjp.hesvh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vlq.bbcook.cn

[S14] C：枚举
来源：http://cxd.guannengcc.top

enum Color { RED, GREEN, BLUE };
来源：http://vdy.dashuyun.cn

[S15] C：类型转换
来源：http://aou.pycfn.com

(double) a / b
来源：http://bcb.aibaodan.cn

[S16] C：位操作置位
来源：http://sfu.fengsongda.top

x |= (1 << 3);
来源：http://jae.wangdashe.top

[S17] C：安全拼接字符串
来源：http://hgk.tian-w.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oec.guannengcc.top

[S18] C：命令行参数
来源：http://qpi.jinqigfzy.top

int main(int argc, char **argv)
来源：http://bxa.ivvv.top

[S19] C：快速排序
来源：http://qjo.chenlongwang.top

qsort(a, n, sizeof(int), cmp);
来源：http://idj.ydjk.org.cn

[S20] C：二分查找
来源：http://hsa.cucudq.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zre.dashuyun.cn

[S21] C：字符类别判断
来源：http://rtj.hnxiangtu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vet.iojbl.cn

[S22] C：字符串转数字
来源：http://xdp.birdmap.top

atoi("42");  strtod("3.14", NULL);
来源：http://gba.chenzaomai.com

[S23] C：随机数
来源：http://qtw.yuanzhike.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ghy.zhixingplan.top

[S24] C：获取本地时间
来源：http://fgi.smart0.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lfz.ppjwa.cn

[S25] C：内存拷贝
来源：http://yvc.hfpthk.cn

memcpy(dst, src, n);
来源：http://vch.xuanzx.com

[S26] C：内存清零
来源：http://eja.kuanghao11.cn

memset(a, 0, sizeof a);
来源：http://gxt.pengpengdd.cyou

[S27] C：定义常量
来源：http://roe.0kj1m.cn

const double PI = 3.14159;
来源：http://bih.jinqigfzy.top

[S28] C：静态变量
来源：http://eou.shuidangran.top

static int counter = 0;
来源：http://nyy.vqdsnc.cn

[S29] C：变参函数
来源：http://mmb.zhongyouzk.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lgo.chenjidiqi.icu

[S30] C：头文件保护
来源：http://vfs.fehbvm.com

#ifndef X_H
来源：http://sci.vehdjk.com

#define X_H
来源：http://lfk.zdbjq.cn

#endif
来源：http://bta.hcnkem.com

[S31] C++：Hello World
来源：http://ghm.sxryk.cn

#include <iostream>
来源：http://lqn.fengsongda.top

int main() { std::cout << "Hello\n"; }
来源：http://juz.xuanzx.com

[S32] C++：字符串
来源：http://lae.c1oappe.top

std::string s = "hi";  s += "!";
来源：http://xdj.daxiang520.top

[S33] C++：vector 增删
来源：http://phd.jiagoushi.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://crb.xuetiantiany.cn

[S34] C++：遍历 vector
来源：http://byx.sjlbkw.cn

for (auto &x : v) { std::cout << x; }
来源：http://qgd.hywenlv.cn

[S35] C++：map
来源：http://cra.gogol.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cim.jqgfzy.top

[S36] C++：unordered_map
来源：http://blm.sxryk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kyt.yanxiufei.cn

[S37] C++：set
来源：http://vkg.hysaishi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jum.daxiang520.top

[S38] C++：排序
来源：http://gko.jyoumei.cn

std::sort(v.begin(), v.end());
来源：http://szw.c1oappe.top

[S39] C++：自定义比较器排序
来源：http://vjk.wangdashe.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dej.iojbl.cn

[S40] C++：查找元素
来源：http://nsw.guowangkeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pti.zdbjq.cn

[S41] C++：类与构造函数
来源：http://cwb.vehdjk.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vgc.c1oappe.top

[S42] C++：继承与虚函数
来源：http://syz.daxiang520.top

class B : public Base { public: void f() override {} };
来源：http://hfq.cqqwz.cn

[S43] C++：智能指针
来源：http://xhv.uphjek.com

auto p = std::make_unique<int>(5);
来源：http://ykl.zdqjudy.top

[S44] C++：引用传参
来源：http://avf.fehbvm.com

void inc(int &x) { ++x; }
来源：http://iwt.gotoacloud.top

[S45] C++：lambda
来源：http://sxi.pengpengdd.cyou

auto add = [](int a, int b) { return a + b; };
来源：http://qwd.hnqzz.top

[S46] C++：函数模板
来源：http://ohz.sjlbkw.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uxw.sweek.top

[S47] C++：结构化绑定遍历
来源：http://nvs.hammf.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fig.fzhhl.top

[S48] C++：逐行读文件
来源：http://qna.dashuyun.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mui.chenjidiqi.icu

while (std::getline(in, line)) { }
来源：http://ddn.xuanzx.com

[S49] C++：写文件
来源：http://fep.ywan-chungtsiang.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zzy.sjlbkw.cn

[S50] C++：格式化数字
来源：http://nbh.wangshuangyany.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ydb.guannengcc.top

[S51] C++：显式类型转换
来源：http://npj.zhongyouzk.top

static_cast<double>(a) / b
来源：http://vkh.wangdashe.top

[S52] C++：const 与 noexcept
来源：http://wfi.jqgfzy.top

int size() const noexcept { return n_; }
来源：http://zdl.hnxiangtu.top

[S53] C++：移动语义
来源：http://feo.chenjidiqi.icu

std::vector<int> w = std::move(v);
来源：http://klw.jinqigfzy.top

[S54] C++：异常处理
来源：http://efl.jyoumei.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zmq.dianchejie.cn

[S55] C++：结构化绑定
来源：http://xia.nanxuanxn.top

auto [a, b] = std::make_pair(1, 2);
来源：http://gqc.yueranfly.top

[S56] C++：optional
来源：http://tqt.ivvv.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ttc.hesvh.cn

[S57] C++：编译期常量
来源：http://ifd.ydzc1.top

constexpr int N = 10;
来源：http://udy.zdqjudy.top

[S58] C++：命名空间
来源：http://buj.vqdsnc.cn

namespace ns { int f() { return 1; } }
来源：http://wcz.hnqzz.top

[S59] C++：静态断言
来源：http://tur.bbcook.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ius.sjlbkw.cn

[S60] C++：遍历并删除元素
来源：http://afc.52xcode.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kve.yfazqb.com

================================================================================
来源：http://pwg.chenlongwang.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dkk.hongshengwenyu.top

================================================================================
来源：http://lyr.c1oappe.top

[T01] Kotlin：Hello World
来源：http://orb.andypj.xyz

println("Hello")
来源：http://aus.fengsongda.top

[T02] Kotlin：变量
来源：http://mle.bbcook.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://znf.jinyuanbaomall.cn

[T03] Kotlin：字符串模板
来源：http://asy.cucudq.cn

"值: $b"
来源：http://erb.sysykeji.top

[T04] Kotlin：空安全
来源：http://vxg.fehbvm.com

val n: String? = null;  n?.length
来源：http://sou.fehbvm.com

[T05] Kotlin：when 表达式
来源：http://xft.jinghuilouyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kyk.svipenyu.cn

[T06] Kotlin：集合映射
来源：http://sig.meibo888.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rfw.epnwcf.com

[T07] Kotlin：集合过滤
来源：http://xpq.aibaodan.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pft.guowangkeji.top

[T08] Kotlin：数据类
来源：http://veq.jiagoushi.top

data class User(val name: String, val age: Int)
来源：http://vrg.zhijiandao.cn

[T09] Kotlin：扩展函数
来源：http://zgs.xziqi.cn

fun String.exclaim() = this + "!"
来源：http://psg.hnxiangtu.top

[T10] Kotlin：默认参数
来源：http://wit.hywenlv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://snv.tanke756.top

[T11] Kotlin：协程
来源：http://gkh.pengpengdd.cyou

GlobalScope.launch { delay(1000); println("done") }
来源：http://jjh.andypj.xyz

[T12] Kotlin：解构声明
来源：http://coe.bbcook.cn

val (a, b) = Pair(1, 2)
来源：http://isj.yj20258888.top

[T13] Kotlin：只读 Map
来源：http://eie.haohaochexian.top

val m = mapOf("a" to 1)
来源：http://zjf.pengpengdd.cyou

[T14] Kotlin：循环
来源：http://fag.guowangkeji.top

for (i in 1..10) println(i)
来源：http://yrx.chenjidiqi.icu

[T15] Kotlin：接口
来源：http://cbv.vqdsnc.cn

interface Shape { fun area(): Double }
来源：http://onh.c1oappe.top

[T16] Swift：Hello World
来源：http://ubt.hnxiangtu.top

print("Hello")
来源：http://yed.shanyushiyangkeji.top

[T17] Swift：变量与常量
来源：http://moj.hammf.cn

var a = 1;  let b = 2
来源：http://rgd.jinqigufen.top

[T18] Swift：字符串插值
来源：http://afu.gaohongyu789.top

"值: \(b)"
来源：http://rkh.zdbjq.cn

[T19] Swift：可选绑定
来源：http://osf.yfazqb.com

if let n = opt { print(n) }
来源：http://fey.hfpthk.cn

[T20] Swift：数组操作
来源：http://vdc.ivvv.top

var a = [1, 2, 3];  a.append(4)
来源：http://xra.tanke756.top

[T21] Swift：遍历
来源：http://unh.zdqjudy.top

for x in a { print(x) }
来源：http://oze.feifeiyinyue.top

[T22] Swift：字典
来源：http://wek.xylfe.cn

var d = ["a": 1];  d["b"] = 2
来源：http://swm.hywenlv.cn

[T23] Swift：函数
来源：http://azh.jinqigfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ahv.fktsv.cn

[T24] Swift：闭包
来源：http://mfd.vqdsnc.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kae.tarul.cn

[T25] Swift：结构体
来源：http://smu.feifeiyinyue.top

struct P { var x: Int }
来源：http://grv.xziqi.cn

[T26] Swift：类与重写
来源：http://vkk.jiagoushi.top

class A: Base { override func f() {} }
来源：http://ohd.yuanzhike.top

[T27] Swift：错误处理
来源：http://qko.xylfe.cn

do { try f() } catch { print(error) }
来源：http://ghw.dashuyun.cn

[T28] Swift：枚举
来源：http://yvp.yj202588.top

enum Color { case red, green }
来源：http://jgp.yj20258888.top

[T29] Swift：guard 提前返回
来源：http://cqo.xziqi.cn

guard let x = opt else { return }
来源：http://fwc.fehbvm.com

[T30] Swift：协议
来源：http://rgu.pycfn.com

protocol Shape { func area() -> Double }
来源：http://qxg.zycfv.cn

[T31] Lua：Hello World
来源：http://oml.guannengcc.top

print("Hello")
来源：http://qel.guowangkeji.top

[T32] Lua：局部变量
来源：http://cha.jqgfzy.top

local a = 1
来源：http://jlj.uphjek.com

[T33] Lua：表（数组）
来源：http://xzj.yueranfly.top

local t = {1, 2, 3};  t[4] = 4
来源：http://fgo.0kj1m.cn

[T34] Lua：遍历表
来源：http://bjk.c1oappe.top

for i, v in ipairs(t) do print(i, v) end
来源：http://doe.birdmap.top

[T35] Lua：字典表
来源：http://ojc.wangdashe.top

local d = { a = 1 };  d.b = 2
来源：http://aop.bjfxy.top

[T36] Lua：函数
来源：http://dtf.316326.xyz

function add(a, b) return a + b end
来源：http://rko.sufxvd.cn

[T37] Lua：字符串拼接
来源：http://ful.birdmap.top

"a" .. "b"
来源：http://oig.mhx1999.top

[T38] Lua：条件
来源：http://iic.gotoacloud.top

if x > 0 then print("正") end
来源：http://gzn.zhixingplan.top

[T39] Lua：模式匹配
来源：http://bzp.zhixingplan.top

string.find(s, "%d+")
来源：http://olr.xuetiantiany.cn

[T40] Lua：元表
来源：http://yei.bjfxy.top

setmetatable({}, { __index = base })
来源：http://npw.bbcook.cn

[T41] Perl：Hello World
来源：http://fko.tanke756.top

print "Hello\n";
来源：http://diw.bbcook.cn

[T42] Perl：变量类型
来源：http://uwl.zhiwuduotai.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wzb.hesvh.cn

[T43] Perl：字符串插值
来源：http://hzd.hongshengwenyu.top

"值: $a"
来源：http://eip.zhijiandao.cn

[T44] Perl：条件
来源：http://ejs.cashguo.top

if ($a > 0) { print "正"; }
来源：http://pmj.smart0.xyz

[T45] Perl：数组遍历
来源：http://lom.hfpthk.cn

for my $x (@arr) { print $x; }
来源：http://rfk.ybcxt.top

[T46] Perl：哈希操作
来源：http://fsg.cdnleiting.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hmr.nanxinkj.top

[T47] Perl：正则捕获
来源：http://pxo.shangyingyoupin.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://cpa.jinghuilouyu.cn

[T48] Perl：正则替换
来源：http://boj.hfpthk.cn

$s =~ s/old/new/g;
来源：http://skh.gogol.net.cn

[T49] Perl：函数
来源：http://viv.cheryme.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ggu.jinqigfzy.top

[T50] Perl：逐行读文件
来源：http://bhw.xuanzx.com

open my $fh, "<", "a.txt" or die $!;
来源：http://voa.hammf.cn


<!-- 参考信息 -->