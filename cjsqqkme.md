代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://trp.smart0.xyz

[R48] awk 取指定列
来源：http://izj.fktsv.cn

awk '{print $1, $3}' a.txt
来源：http://cso.yueranfly.top

[R49] awk 带条件
来源：http://ckh.hysaishi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fvr.xingfuxueyuan.xyz

[R50] awk 求和
来源：http://mwf.dianchejie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vdb.svipenyu.cn

[R51] 排序去重取前几
来源：http://mfo.hnqzz.top

sort a.txt | uniq -c | sort -rn | head
来源：http://smm.fengsongda.top

[R52] 统计行数
来源：http://byp.bbcook.cn

wc -l a.txt
来源：http://xgb.smart0.xyz

[R53] 查看文件头与实时尾
来源：http://dsl.vqdsnc.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fwd.yueranfly.top

[R54] 比较两个文件
来源：http://rgz.cdnleiting.top

diff a.txt b.txt
来源：http://xxy.0kj1m.cn

[R55] 压缩与解压
来源：http://fxf.hysaishi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hmu.yongpay.top

[R56] 远程拷贝
来源：http://nnp.xziqi.cn

scp file user@host:/path/
来源：http://dtk.zhongyouzk.top

[R57] 远程执行命令
来源：http://jac.zhongyouzk.top

ssh user@host 'uptime'
来源：http://ttf.feifeiyinyue.top

[R58] 下载文件
来源：http://nje.zdbjq.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://okj.yonumen.top

[R59] 发 POST JSON
来源：http://jol.pycfn.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rol.zhixingplan.top

[R60] 只看 HTTP 状态码
来源：http://hxh.zhengqikj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fcv.yvedp.cn

[R61] 磁盘占用
来源：http://jjw.chenlongwang.top

df -h;  du -sh *
来源：http://ypw.nanxinkj.top

[R62] 找最占空间的文件
来源：http://kws.iojbl.cn

du -ah . | sort -rh | head -10
来源：http://wvj.gotoacloud.top

[R63] 内存与进程
来源：http://brf.gaohongyu789.top

free -h;  ps aux | grep nginx
来源：http://xnv.sjlbkw.cn

[R64] 结束进程
来源：http://bxm.jinqigufen.top

kill -9 $(pgrep -f app.py)
来源：http://inj.birdmap.top

[R65] 查看端口占用
来源：http://qig.jinqigfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gyl.bbcook.cn

[R66] 定时任务
来源：http://cfe.xuetiantiany.cn

crontab -e;  crontab -l
来源：http://sgj.yfazqb.com

[R67] 生成随机十六进制串
来源：http://plb.hcnkem.com

openssl rand -hex 16
来源：http://ulq.uphjek.com

[R68] 计算文件校验值
来源：http://aef.jinghuilouyu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://znz.dashuyun.cn

[R69] 生成随机密码
来源：http://pjx.guowangkeji.top

head -c 16 /dev/urandom | base64
来源：http://ydq.quarkkingdee.top

[R70] 时间戳与互转
来源：http://jwk.shanyushiyangkeji.top

date +%s;  date -d @1700000000
来源：http://khh.pycfn.com

[R71] 日期格式化
来源：http://zad.shzxlz.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mts.daria6918.cn

[R72] 等待端口就绪
来源：http://ljw.xinyue.icu

until nc -z localhost 3306; do sleep 1; done
来源：http://fvq.jqgufenzy.top

[R73] 分割大日志
来源：http://akt.ydjk.org.cn

split -l 1000 big.log part_
来源：http://ere.jqgufenzy.top

[R74] 批量重命名
来源：http://ogi.ppjwa.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rib.shanyushiyangkeji.top

[R75] 导出环境变量
来源：http://ctm.fktsv.cn

export PATH="$HOME/bin:$PATH"
来源：http://czq.mhx1999.top

[R76] 使用临时文件
来源：http://nyf.gaohongyu789.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rrt.gzhubu.top

[R77] 读取用户输入
来源：http://wyv.shangyingyoupin.top

read -rp "请输入: " ans
来源：http://qnx.chenlongwang.top

[R78] 交互式菜单
来源：http://whc.cdnleiting.top

select opt in a b c; do echo "$opt"; break; done
来源：http://jlc.wangshuangyany.cn

[R79] 解析命令行选项
来源：http://lka.tian-w.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ojc.ctjpmb.com

[R80] 查看脚本执行耗时
来源：http://idn.zhijiandao.cn

time ./run.sh
来源：http://aqu.feifeiyinyue.top

================================================================================
来源：http://rsv.shangyingyoupin.top

S. C / C++ 专题
来源：http://mhe.sysykeji.top

================================================================================
来源：http://ifk.sxryk.cn

[S01] C：Hello World
来源：http://ykf.cucudq.cn

#include <stdio.h>
来源：http://eie.daria6918.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://juf.jiagoushi.top

[S02] C：变量与格式化输出
来源：http://wfd.jianghu66.top

int a = 10; printf("%d\n", a);
来源：http://vsk.vehdjk.com

[S03] C：读入整数
来源：http://tgl.hongshengwenyu.top

int x; scanf("%d", &x);
来源：http://ctp.zycfv.cn

[S04] C：字符串复制
来源：http://nxp.cucudq.cn

char dst[32]; strcpy(dst, "hi");
来源：http://afi.dashuyun.cn

[S05] C：字符串长度
来源：http://qmx.xuanzx.com

strlen(s)
来源：http://xeg.yueranfly.top

[S06] C：字符串比较
来源：http://sxn.hammf.cn

strcmp(a, b) == 0
来源：http://zzb.xingfuxueyuan.xyz

[S07] C：数组遍历求和
来源：http://ywm.xinyue.icu

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vjn.ydzc1.top

[S08] C：动态内存分配与释放
来源：http://yhn.hongshengwenyu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ymg.feifeiyinyue.top

[S09] C：结构体定义与初始化
来源：http://pme.zhixingplan.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jcu.zhiwuduotai.top

[S10] C：指针与解引用
来源：http://wis.hnxiangtu.top

int *p = &a;  *p = 5;
来源：http://aat.jqgfzy.top

[S11] C：逐行读文件
来源：http://nkd.aibaodan.cn

FILE *f = fopen("a.txt", "r");
来源：http://iah.xuanzx.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://nln.yj202588.top

fclose(f);
来源：http://blx.pengpengdd.cyou

[S12] C：写文件
来源：http://ixk.pycfn.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zhv.fehbvm.com

[S13] C：宏定义
来源：http://wtm.sysykeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://txk.pycfn.com

[S14] C：枚举
来源：http://kum.chenjidiqi.icu

enum Color { RED, GREEN, BLUE };
来源：http://tya.nanxuanxn.top

[S15] C：类型转换
来源：http://otm.gaohongyu789.top

(double) a / b
来源：http://dop.shanyushiyangkeji.top

[S16] C：位操作置位
来源：http://fgk.316326.xyz

x |= (1 << 3);
来源：http://cbv.316326.xyz

[S17] C：安全拼接字符串
来源：http://ypb.tian-w.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ijg.hongshengwenyu.top

[S18] C：命令行参数
来源：http://fal.guowangkeji.top

int main(int argc, char **argv)
来源：http://lgx.zdbjq.cn

[S19] C：快速排序
来源：http://mhi.0kj1m.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rky.gotoacloud.top

[S20] C：二分查找
来源：http://puh.bbcook.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xxy.sxryk.cn

[S21] C：字符类别判断
来源：http://jih.shuidangran.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zzs.daxiang520.top

[S22] C：字符串转数字
来源：http://hkc.ehwqpu.com

atoi("42");  strtod("3.14", NULL);
来源：http://lcz.zhiwuduotai.top

[S23] C：随机数
来源：http://aul.xziqi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hon.ywan-chungtsiang.top

[S24] C：获取本地时间
来源：http://shv.ydjk.org.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cpt.guowangkeji.top

[S25] C：内存拷贝
来源：http://rrg.redwolf501.top

memcpy(dst, src, n);
来源：http://hwe.uphjek.com

[S26] C：内存清零
来源：http://wiv.aizwys.cn

memset(a, 0, sizeof a);
来源：http://gai.daria6918.cn

[S27] C：定义常量
来源：http://oyt.jinghuilouyu.cn

const double PI = 3.14159;
来源：http://smd.nanxuanxn.top

[S28] C：静态变量
来源：http://rne.jyoumei.cn

static int counter = 0;
来源：http://bdr.hywenlv.cn

[S29] C：变参函数
来源：http://gqy.sjlbkw.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jex.xuanzx.com

[S30] C：头文件保护
来源：http://qyn.hcnkem.com

#ifndef X_H
来源：http://cjw.yonumen.top

#define X_H
来源：http://jrp.pycfn.com

#endif
来源：http://jid.zhengqikj.top

[S31] C++：Hello World
来源：http://azy.bjfxy.top

#include <iostream>
来源：http://dcb.zhongyouzk.top

int main() { std::cout << "Hello\n"; }
来源：http://kjl.chenzaomai.com

[S32] C++：字符串
来源：http://bzy.pycfn.com

std::string s = "hi";  s += "!";
来源：http://cjo.cucudq.cn

[S33] C++：vector 增删
来源：http://hsn.sxryk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qqn.52xcode.cn

[S34] C++：遍历 vector
来源：http://wbk.dianchejie.cn

for (auto &x : v) { std::cout << x; }
来源：http://dnu.52xcode.cn

[S35] C++：map
来源：http://voi.yj20258888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://udb.yangfankeji.com

[S36] C++：unordered_map
来源：http://llo.xuetiantiany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mnq.yj20258.top

[S37] C++：set
来源：http://vnk.svipenyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://htm.ppjwa.cn

[S38] C++：排序
来源：http://zaq.shangyingyoupin.top

std::sort(v.begin(), v.end());
来源：http://ixc.ctjpmb.com

[S39] C++：自定义比较器排序
来源：http://msp.yfazqb.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yxn.shanyushiyangkeji.top

[S40] C++：查找元素
来源：http://afk.xinyue.icu

auto it = std::find(v.begin(), v.end(), 3);
来源：http://waa.nwbrower.top

[S41] C++：类与构造函数
来源：http://cwa.meibo888.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xku.xuanzx.com

[S42] C++：继承与虚函数
来源：http://tza.yuxming.cn

class B : public Base { public: void f() override {} };
来源：http://svi.zhiwuduotai.top

[S43] C++：智能指针
来源：http://cbz.hnqzz.top

auto p = std::make_unique<int>(5);
来源：http://ajs.aizwys.cn

[S44] C++：引用传参
来源：http://wbf.sxryk.cn

void inc(int &x) { ++x; }
来源：http://ajc.jinqigfzy.top

[S45] C++：lambda
来源：http://ssr.gaohongyu789.top

auto add = [](int a, int b) { return a + b; };
来源：http://lzn.9152youxi.cn

[S46] C++：函数模板
来源：http://jna.jinghuilouyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://opb.shzxlz.cn

[S47] C++：结构化绑定遍历
来源：http://skf.fanxiaobao.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zel.hongshengwenyu.top

[S48] C++：逐行读文件
来源：http://pkx.havefunace.top

std::ifstream in("a.txt");  std::string line;
来源：http://vcs.hesvh.cn

while (std::getline(in, line)) { }
来源：http://rla.zdbjq.cn

[S49] C++：写文件
来源：http://zvj.jianghu66.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fxn.shanyushiyangtech.top

[S50] C++：格式化数字
来源：http://kqr.fehbvm.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xju.meibo888.top

[S51] C++：显式类型转换
来源：http://utb.yuanzhike.top

static_cast<double>(a) / b
来源：http://bhs.52xcode.cn

[S52] C++：const 与 noexcept
来源：http://pww.yvedp.cn

int size() const noexcept { return n_; }
来源：http://aob.jqgufenzy.top

[S53] C++：移动语义
来源：http://qkn.ppjwa.cn

std::vector<int> w = std::move(v);
来源：http://ilx.yvedp.cn

[S54] C++：异常处理
来源：http://jqc.shzxlz.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ogh.aibaodan.cn

[S55] C++：结构化绑定
来源：http://dxe.yj20258888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qtn.hongshengwenyu.top

[S56] C++：optional
来源：http://wka.tianlin.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dfe.0kj1m.cn

[S57] C++：编译期常量
来源：http://bju.yueranfly.top

constexpr int N = 10;
来源：http://twj.xuanzx.com

[S58] C++：命名空间
来源：http://ljs.fanxiaobao.xyz

namespace ns { int f() { return 1; } }
来源：http://zle.cucudq.cn

[S59] C++：静态断言
来源：http://nxg.52xcode.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dwr.andypj.xyz

[S60] C++：遍历并删除元素
来源：http://snv.zhixingplan.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uad.pengpengdd.cyou

================================================================================
来源：http://eft.xuetiantiany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gcm.bbcook.cn

================================================================================
来源：http://cxi.gzhubu.top

[T01] Kotlin：Hello World
来源：http://brr.zhixingplan.top

println("Hello")
来源：http://jkd.jlsjyb.cn

[T02] Kotlin：变量
来源：http://fnj.fktsv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gkd.jiagoushi.top

[T03] Kotlin：字符串模板
来源：http://rby.aibaodan.cn

"值: $b"
来源：http://agv.shanyushiyangtech.top

[T04] Kotlin：空安全
来源：http://odl.chenzaomai.com

val n: String? = null;  n?.length
来源：http://bjz.pycfn.com

[T05] Kotlin：when 表达式
来源：http://jha.zhiwuduotai.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yxk.shuidangran.top

[T06] Kotlin：集合映射
来源：http://qix.fengsongda.top

listOf(1, 2, 3).map { it * 2 }
来源：http://kec.shangyingyoupin.top

[T07] Kotlin：集合过滤
来源：http://wud.chenjidiqi.icu

listOf(1, 2, 3).filter { it > 1 }
来源：http://boh.sysykeji.top

[T08] Kotlin：数据类
来源：http://cfw.uphjek.com

data class User(val name: String, val age: Int)
来源：http://loa.cucudq.cn

[T09] Kotlin：扩展函数
来源：http://jlr.ctjpmb.com

fun String.exclaim() = this + "!"
来源：http://slf.xingfuxueyuan.xyz

[T10] Kotlin：默认参数
来源：http://sbp.jyoumei.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gqi.tanke756.top

[T11] Kotlin：协程
来源：http://gvy.ctjpmb.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://rpk.316326.xyz

[T12] Kotlin：解构声明
来源：http://soz.guannengcc.top

val (a, b) = Pair(1, 2)
来源：http://cwd.daxiang520.top

[T13] Kotlin：只读 Map
来源：http://mvb.tianlin.xyz

val m = mapOf("a" to 1)
来源：http://lja.yj202588.top

[T14] Kotlin：循环
来源：http://kck.yuxming.cn

for (i in 1..10) println(i)
来源：http://yax.pycfn.com

[T15] Kotlin：接口
来源：http://rlr.fehbvm.com

interface Shape { fun area(): Double }
来源：http://jem.yj20258.top

[T16] Swift：Hello World
来源：http://wtt.yueranfly.top

print("Hello")
来源：http://xff.kuanghao11.cn

[T17] Swift：变量与常量
来源：http://ypy.vqdsnc.cn

var a = 1;  let b = 2
来源：http://vpn.bbcook.cn

[T18] Swift：字符串插值
来源：http://xyc.zhixingplan.top

"值: \(b)"
来源：http://slt.gzhubu.top

[T19] Swift：可选绑定
来源：http://sde.jinyuanbaomall.cn

if let n = opt { print(n) }
来源：http://wvn.yangfankeji.com

[T20] Swift：数组操作
来源：http://ogj.zhaomingkeji.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://kfq.gzhubu.top

[T21] Swift：遍历
来源：http://cjy.ydzc1.top

for x in a { print(x) }
来源：http://cpp.jyoumei.cn

[T22] Swift：字典
来源：http://lze.xuetiantiany.cn

var d = ["a": 1];  d["b"] = 2
来源：http://owg.yj202588.top

[T23] Swift：函数
来源：http://qkx.gogol.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dxt.uphjek.com

[T24] Swift：闭包
来源：http://oke.zhengqikj.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://asg.zhiwuduotai.top

[T25] Swift：结构体
来源：http://xxx.zhongyouzk.top

struct P { var x: Int }
来源：http://opn.ybcxt.top

[T26] Swift：类与重写
来源：http://jet.zhengqikj.top

class A: Base { override func f() {} }
来源：http://aif.c1oappe.top

[T27] Swift：错误处理
来源：http://axn.aibaodan.cn

do { try f() } catch { print(error) }
来源：http://wyp.xinyue.icu

[T28] Swift：枚举
来源：http://pxw.vehdjk.com

enum Color { case red, green }
来源：http://tvl.zdbjq.cn

[T29] Swift：guard 提前返回
来源：http://vpg.tanke756.top

guard let x = opt else { return }
来源：http://twg.zycfv.cn

[T30] Swift：协议
来源：http://wik.yj202588.top

protocol Shape { func area() -> Double }
来源：http://ftk.hfpthk.cn

[T31] Lua：Hello World
来源：http://uhh.c1oappe.top

print("Hello")
来源：http://hjk.yj20258.top

[T32] Lua：局部变量
来源：http://vcv.daria6918.cn

local a = 1
来源：http://gzr.yuanzhike.top

[T33] Lua：表（数组）
来源：http://kar.fanxiaobao.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://iwd.jyoumei.cn

[T34] Lua：遍历表
来源：http://noe.cqqwz.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vhp.havefunace.top

[T35] Lua：字典表
来源：http://mvr.ctjpmb.com

local d = { a = 1 };  d.b = 2
来源：http://sfa.nwbrower.top

[T36] Lua：函数
来源：http://dyn.chenjidiqi.icu

function add(a, b) return a + b end
来源：http://uqn.epnwcf.com

[T37] Lua：字符串拼接
来源：http://jrr.cqqwz.cn

"a" .. "b"
来源：http://fgp.yfazqb.com

[T38] Lua：条件
来源：http://tvm.fehbvm.com

if x > 0 then print("正") end
来源：http://ywj.ivvv.top

[T39] Lua：模式匹配
来源：http://dwn.yfazqb.com

string.find(s, "%d+")
来源：http://cxs.yj20258.top

[T40] Lua：元表
来源：http://bew.chenzaomai.com

setmetatable({}, { __index = base })
来源：http://olx.yueranfly.top

[T41] Perl：Hello World
来源：http://hge.zycfv.cn

print "Hello\n";
来源：http://wwh.guannengcc.top

[T42] Perl：变量类型
来源：http://vqy.guowangkeji.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://frp.redwolf501.top

[T43] Perl：字符串插值
来源：http://hxv.dashuyun.cn

"值: $a"
来源：http://irx.cdnleiting.top

[T44] Perl：条件
来源：http://bga.gotoacloud.top

if ($a > 0) { print "正"; }
来源：http://zhp.hfpthk.cn

[T45] Perl：数组遍历
来源：http://scf.vehdjk.com

for my $x (@arr) { print $x; }
来源：http://qpq.zhongyouzk.top

[T46] Perl：哈希操作
来源：http://ezs.sweek.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zxv.316326.xyz

[T47] Perl：正则捕获
来源：http://cld.0kj1m.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ner.pycfn.com

[T48] Perl：正则替换
来源：http://klb.yvedp.cn

$s =~ s/old/new/g;
来源：http://wbl.yuanzhike.top

[T49] Perl：函数
来源：http://hst.0kj1m.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sxa.zhixingplan.top

[T50] Perl：逐行读文件
来源：http://hdm.jinghuilouyu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fye.sjlbkw.cn


<!-- 参考信息 -->