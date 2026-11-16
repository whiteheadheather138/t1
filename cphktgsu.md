代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://dyp.52xcode.cn

[R48] awk 取指定列
来源：http://lpc.hongshengwenyu.top

awk '{print $1, $3}' a.txt
来源：http://uca.cdnleiting.top

[R49] awk 带条件
来源：http://xqk.yonumen.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rea.guannengcc.top

[R50] awk 求和
来源：http://pdn.redwolf501.top

awk '{s += $2} END {print s}' a.txt
来源：http://wom.daxiang520.top

[R51] 排序去重取前几
来源：http://xkb.jinqigufen.top

sort a.txt | uniq -c | sort -rn | head
来源：http://fzu.tarul.cn

[R52] 统计行数
来源：http://rml.aizwys.cn

wc -l a.txt
来源：http://psc.xuetiantiany.cn

[R53] 查看文件头与实时尾
来源：http://ubb.cashguo.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wex.uphjek.com

[R54] 比较两个文件
来源：http://hhz.gaohongyu789.top

diff a.txt b.txt
来源：http://muh.zhongyouzk.top

[R55] 压缩与解压
来源：http://uxi.pengpengdd.cyou

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mrg.sysykeji.top

[R56] 远程拷贝
来源：http://tei.ywan-chungtsiang.top

scp file user@host:/path/
来源：http://pkt.gaohongyu789.top

[R57] 远程执行命令
来源：http://mfd.dianchejie.cn

ssh user@host 'uptime'
来源：http://aiv.hywenlv.cn

[R58] 下载文件
来源：http://gfp.fanxiaobao.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yvi.svipenyu.cn

[R59] 发 POST JSON
来源：http://eec.cqqwz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vvn.jinyuanbaomall.cn

[R60] 只看 HTTP 状态码
来源：http://mkk.yvedp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mkx.mhx1999.top

[R61] 磁盘占用
来源：http://vrw.snrcjt.cn

df -h;  du -sh *
来源：http://zcr.fengsongda.top

[R62] 找最占空间的文件
来源：http://ima.hesvh.cn

du -ah . | sort -rh | head -10
来源：http://cgx.guannengcc.top

[R63] 内存与进程
来源：http://cve.zycfv.cn

free -h;  ps aux | grep nginx
来源：http://jaw.wangshuangyany.cn

[R64] 结束进程
来源：http://hew.jqgfzy.top

kill -9 $(pgrep -f app.py)
来源：http://yma.hnxiangtu.top

[R65] 查看端口占用
来源：http://lku.vehdjk.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fta.pengpengdd.cyou

[R66] 定时任务
来源：http://uca.iojbl.cn

crontab -e;  crontab -l
来源：http://dqj.guannengcc.top

[R67] 生成随机十六进制串
来源：http://juy.birdmap.top

openssl rand -hex 16
来源：http://psf.yj20258.top

[R68] 计算文件校验值
来源：http://kdk.fzhhl.top

sha256sum a.txt;  md5sum a.txt
来源：http://fth.bjfxy.top

[R69] 生成随机密码
来源：http://lzh.hongshengwenyu.top

head -c 16 /dev/urandom | base64
来源：http://kip.jianghu66.top

[R70] 时间戳与互转
来源：http://owi.hysaishi.cn

date +%s;  date -d @1700000000
来源：http://cnh.zdbjq.cn

[R71] 日期格式化
来源：http://kjp.yuxming.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jge.tianlin.xyz

[R72] 等待端口就绪
来源：http://qes.vehdjk.com

until nc -z localhost 3306; do sleep 1; done
来源：http://oov.xuanzx.com

[R73] 分割大日志
来源：http://nhc.zhengqikj.top

split -l 1000 big.log part_
来源：http://zvv.uphjek.com

[R74] 批量重命名
来源：http://wuc.tian-w.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fqz.fehbvm.com

[R75] 导出环境变量
来源：http://ktl.sjlbkw.cn

export PATH="$HOME/bin:$PATH"
来源：http://cue.52xcode.cn

[R76] 使用临时文件
来源：http://led.zhiwuduotai.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tyc.c1oappe.top

[R77] 读取用户输入
来源：http://tgv.havefunace.top

read -rp "请输入: " ans
来源：http://iqq.kuanghao11.cn

[R78] 交互式菜单
来源：http://jyt.fzhhl.top

select opt in a b c; do echo "$opt"; break; done
来源：http://nkn.sysykeji.top

[R79] 解析命令行选项
来源：http://ktj.jiagoushi.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://djo.tarul.cn

[R80] 查看脚本执行耗时
来源：http://tok.gogol.net.cn

time ./run.sh
来源：http://xxz.hywenlv.cn

================================================================================
来源：http://uny.vehdjk.com

S. C / C++ 专题
来源：http://mxg.birdmap.top

================================================================================
来源：http://rwy.wangshuangyany.cn

[S01] C：Hello World
来源：http://edb.wangdashe.top

#include <stdio.h>
来源：http://rfv.andypj.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://rdx.iojbl.cn

[S02] C：变量与格式化输出
来源：http://iht.tian-w.cn

int a = 10; printf("%d\n", a);
来源：http://xkt.zhiwuduotai.top

[S03] C：读入整数
来源：http://qre.ybcxt.top

int x; scanf("%d", &x);
来源：http://buh.bbcook.cn

[S04] C：字符串复制
来源：http://hcc.feifeiyinyue.top

char dst[32]; strcpy(dst, "hi");
来源：http://vlt.zhiwuduotai.top

[S05] C：字符串长度
来源：http://fxg.mhx1999.top

strlen(s)
来源：http://mwe.vehdjk.com

[S06] C：字符串比较
来源：http://gff.hongshengwenyu.top

strcmp(a, b) == 0
来源：http://hkn.dianchejie.cn

[S07] C：数组遍历求和
来源：http://uik.jianghu66.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jti.316326.xyz

[S08] C：动态内存分配与释放
来源：http://vlt.yanxiufei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://obc.sxryk.cn

[S09] C：结构体定义与初始化
来源：http://vok.xziqi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wtl.ehwqpu.com

[S10] C：指针与解引用
来源：http://uey.bbcook.cn

int *p = &a;  *p = 5;
来源：http://raz.iojbl.cn

[S11] C：逐行读文件
来源：http://elj.shangyingyoupin.top

FILE *f = fopen("a.txt", "r");
来源：http://mzj.pycfn.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://lzc.tanke756.top

fclose(f);
来源：http://jsw.iojbl.cn

[S12] C：写文件
来源：http://ais.cucudq.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pne.zdqjudy.top

[S13] C：宏定义
来源：http://wjo.pycfn.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ndv.jqgufenzy.top

[S14] C：枚举
来源：http://xob.epnwcf.com

enum Color { RED, GREEN, BLUE };
来源：http://iou.yj20258888.top

[S15] C：类型转换
来源：http://xqk.yfazqb.com

(double) a / b
来源：http://agx.daxiang520.top

[S16] C：位操作置位
来源：http://xap.cdnleiting.top

x |= (1 << 3);
来源：http://auf.kuanghao11.cn

[S17] C：安全拼接字符串
来源：http://lkr.wangdashe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hky.xuanzx.com

[S18] C：命令行参数
来源：http://byc.xuetiantiany.cn

int main(int argc, char **argv)
来源：http://vcw.ydjk.org.cn

[S19] C：快速排序
来源：http://cxz.zycfv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wco.jyoumei.cn

[S20] C：二分查找
来源：http://fvc.nwbrower.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sin.jinqigufen.top

[S21] C：字符类别判断
来源：http://roe.meibo888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nqb.jinqigufen.top

[S22] C：字符串转数字
来源：http://vkz.dashuyun.cn

atoi("42");  strtod("3.14", NULL);
来源：http://eao.havefunace.top

[S23] C：随机数
来源：http://rfr.ppjwa.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://npd.gaohongyu789.top

[S24] C：获取本地时间
来源：http://nzh.nanxinkj.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xwf.wangdashe.top

[S25] C：内存拷贝
来源：http://piv.aibaodan.cn

memcpy(dst, src, n);
来源：http://rtq.bjfxy.top

[S26] C：内存清零
来源：http://wtg.jlsjyb.cn

memset(a, 0, sizeof a);
来源：http://siv.dashuyun.cn

[S27] C：定义常量
来源：http://wni.zhengqikj.top

const double PI = 3.14159;
来源：http://ere.yvedp.cn

[S28] C：静态变量
来源：http://ulk.tian-w.cn

static int counter = 0;
来源：http://omj.mhx1999.top

[S29] C：变参函数
来源：http://rrl.guannengcc.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nms.tanke756.top

[S30] C：头文件保护
来源：http://iuw.pycfn.com

#ifndef X_H
来源：http://xgy.ivvv.top

#define X_H
来源：http://cqp.ctjpmb.com

#endif
来源：http://mdq.haohaochexian.top

[S31] C++：Hello World
来源：http://eii.cheryme.top

#include <iostream>
来源：http://nci.hesvh.cn

int main() { std::cout << "Hello\n"; }
来源：http://uqm.xuetiantiany.cn

[S32] C++：字符串
来源：http://esy.hnqzz.top

std::string s = "hi";  s += "!";
来源：http://gxg.yongpay.top

[S33] C++：vector 增删
来源：http://nou.jyoumei.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qtl.xziqi.cn

[S34] C++：遍历 vector
来源：http://dob.vqdsnc.cn

for (auto &x : v) { std::cout << x; }
来源：http://jqk.xuanzx.com

[S35] C++：map
来源：http://olf.jinqigfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jze.yvedp.cn

[S36] C++：unordered_map
来源：http://tfy.jinqigfzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bsz.ivvv.top

[S37] C++：set
来源：http://grf.xinyue.icu

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fnc.jlsjyb.cn

[S38] C++：排序
来源：http://ukx.daria6918.cn

std::sort(v.begin(), v.end());
来源：http://wsl.ctjpmb.com

[S39] C++：自定义比较器排序
来源：http://kjt.yonumen.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xoz.fzhhl.top

[S40] C++：查找元素
来源：http://wsu.cashguo.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jdp.shanyushiyangkeji.top

[S41] C++：类与构造函数
来源：http://sga.cqqwz.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://roh.yj20258888.top

[S42] C++：继承与虚函数
来源：http://rbg.shangyingyoupin.top

class B : public Base { public: void f() override {} };
来源：http://czj.sjlbkw.cn

[S43] C++：智能指针
来源：http://ceh.hnxiangtu.top

auto p = std::make_unique<int>(5);
来源：http://ovr.fzhhl.top

[S44] C++：引用传参
来源：http://jtw.aibaodan.cn

void inc(int &x) { ++x; }
来源：http://tfc.yonumen.top

[S45] C++：lambda
来源：http://fxj.gaohongyu789.top

auto add = [](int a, int b) { return a + b; };
来源：http://yuf.ivvv.top

[S46] C++：函数模板
来源：http://fmq.quarkkingdee.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rsp.nanxinkj.top

[S47] C++：结构化绑定遍历
来源：http://bsx.zhengqikj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hmo.xuanzx.com

[S48] C++：逐行读文件
来源：http://fbj.fanxiaobao.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://kof.quarkkingdee.top

while (std::getline(in, line)) { }
来源：http://ane.nanxuanxn.top

[S49] C++：写文件
来源：http://tsm.52xcode.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gnm.hcnkem.com

[S50] C++：格式化数字
来源：http://tfr.jinqigfzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bnn.snrcjt.cn

[S51] C++：显式类型转换
来源：http://axy.vqdsnc.cn

static_cast<double>(a) / b
来源：http://apv.yj202588.top

[S52] C++：const 与 noexcept
来源：http://kgv.hfpthk.cn

int size() const noexcept { return n_; }
来源：http://xva.vehdjk.com

[S53] C++：移动语义
来源：http://vhh.yonumen.top

std::vector<int> w = std::move(v);
来源：http://fhl.tarul.cn

[S54] C++：异常处理
来源：http://gab.kuanghao11.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zbb.cashguo.top

[S55] C++：结构化绑定
来源：http://gfk.vehdjk.com

auto [a, b] = std::make_pair(1, 2);
来源：http://vdh.guowangkeji.top

[S56] C++：optional
来源：http://aat.kuanghao11.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xpv.nanxuanxn.top

[S57] C++：编译期常量
来源：http://fph.zhixingplan.top

constexpr int N = 10;
来源：http://cng.meibo888.top

[S58] C++：命名空间
来源：http://jtf.hongshengwenyu.top

namespace ns { int f() { return 1; } }
来源：http://krj.ybcxt.top

[S59] C++：静态断言
来源：http://hdz.yvedp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fjm.guowangkeji.top

[S60] C++：遍历并删除元素
来源：http://eaj.xuanzx.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://isb.sysykeji.top

================================================================================
来源：http://yfh.fengsongda.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ogt.hcnkem.com

================================================================================
来源：http://vqi.guannengcc.top

[T01] Kotlin：Hello World
来源：http://wny.mhx1999.top

println("Hello")
来源：http://bmx.cdnleiting.top

[T02] Kotlin：变量
来源：http://rto.pycfn.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ejq.yanxiufei.cn

[T03] Kotlin：字符串模板
来源：http://pju.smart0.xyz

"值: $b"
来源：http://oqm.pycfn.com

[T04] Kotlin：空安全
来源：http://lpn.jinyuanbaomall.cn

val n: String? = null;  n?.length
来源：http://gdo.jinqigfzy.top

[T05] Kotlin：when 表达式
来源：http://xqc.fehbvm.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yav.sjlbkw.cn

[T06] Kotlin：集合映射
来源：http://exs.snrcjt.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://efx.zhixingplan.top

[T07] Kotlin：集合过滤
来源：http://ycd.ctjpmb.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://fsy.chenzaomai.com

[T08] Kotlin：数据类
来源：http://cfc.hesvh.cn

data class User(val name: String, val age: Int)
来源：http://qwr.fengsongda.top

[T09] Kotlin：扩展函数
来源：http://koq.havefunace.top

fun String.exclaim() = this + "!"
来源：http://zyh.feifeiyinyue.top

[T10] Kotlin：默认参数
来源：http://dgv.ehwqpu.com

fun greet(name: String = "World") = "Hi $name"
来源：http://kuk.hywenlv.cn

[T11] Kotlin：协程
来源：http://kzh.tianlin.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://cis.fzhhl.top

[T12] Kotlin：解构声明
来源：http://fwc.dianchejie.cn

val (a, b) = Pair(1, 2)
来源：http://rmu.cheryme.top

[T13] Kotlin：只读 Map
来源：http://gth.birdmap.top

val m = mapOf("a" to 1)
来源：http://jql.shanyushiyangtech.top

[T14] Kotlin：循环
来源：http://ljf.gogol.net.cn

for (i in 1..10) println(i)
来源：http://yws.yfazqb.com

[T15] Kotlin：接口
来源：http://bvx.bjfxy.top

interface Shape { fun area(): Double }
来源：http://xws.yuanzhike.top

[T16] Swift：Hello World
来源：http://xzg.jianghu66.top

print("Hello")
来源：http://fxf.sufxvd.cn

[T17] Swift：变量与常量
来源：http://euq.shzxlz.cn

var a = 1;  let b = 2
来源：http://nrw.quarkkingdee.top

[T18] Swift：字符串插值
来源：http://odc.hfpthk.cn

"值: \(b)"
来源：http://myr.quarkkingdee.top

[T19] Swift：可选绑定
来源：http://ftn.zhixingplan.top

if let n = opt { print(n) }
来源：http://jjx.xingfuxueyuan.xyz

[T20] Swift：数组操作
来源：http://ghn.zhengqikj.top

var a = [1, 2, 3];  a.append(4)
来源：http://nkh.gzhubu.top

[T21] Swift：遍历
来源：http://eis.kuanghao11.cn

for x in a { print(x) }
来源：http://ijw.zdqjudy.top

[T22] Swift：字典
来源：http://iiz.dianchejie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qyv.hysaishi.cn

[T23] Swift：函数
来源：http://niu.xingfuxueyuan.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jli.zdqjudy.top

[T24] Swift：闭包
来源：http://rkm.hongshengwenyu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://odx.yfazqb.com

[T25] Swift：结构体
来源：http://fbj.zhengqikj.top

struct P { var x: Int }
来源：http://zge.nanxuanxn.top

[T26] Swift：类与重写
来源：http://vqq.jinghuilouyu.cn

class A: Base { override func f() {} }
来源：http://utw.yongpay.top

[T27] Swift：错误处理
来源：http://ppx.nwbrower.top

do { try f() } catch { print(error) }
来源：http://cda.sysykeji.top

[T28] Swift：枚举
来源：http://let.smart0.xyz

enum Color { case red, green }
来源：http://you.iojbl.cn

[T29] Swift：guard 提前返回
来源：http://qig.hnxiangtu.top

guard let x = opt else { return }
来源：http://klt.fzhhl.top

[T30] Swift：协议
来源：http://hbo.jqgufenzy.top

protocol Shape { func area() -> Double }
来源：http://iwj.9152youxi.cn

[T31] Lua：Hello World
来源：http://rjb.dianchejie.cn

print("Hello")
来源：http://bvu.bbcook.cn

[T32] Lua：局部变量
来源：http://lhs.pycfn.com

local a = 1
来源：http://adm.zhijiandao.cn

[T33] Lua：表（数组）
来源：http://svr.ywan-chungtsiang.top

local t = {1, 2, 3};  t[4] = 4
来源：http://gzm.ydzc1.top

[T34] Lua：遍历表
来源：http://bey.ybcxt.top

for i, v in ipairs(t) do print(i, v) end
来源：http://oof.xuetiantiany.cn

[T35] Lua：字典表
来源：http://ayz.feifeiyinyue.top

local d = { a = 1 };  d.b = 2
来源：http://sps.yfazqb.com

[T36] Lua：函数
来源：http://czb.yuanzhike.top

function add(a, b) return a + b end
来源：http://oxn.cashguo.top

[T37] Lua：字符串拼接
来源：http://xtj.jinqigfzy.top

"a" .. "b"
来源：http://psu.zhengqikj.top

[T38] Lua：条件
来源：http://ltz.yvedp.cn

if x > 0 then print("正") end
来源：http://prk.zhongyouzk.top

[T39] Lua：模式匹配
来源：http://xlm.jianghu66.top

string.find(s, "%d+")
来源：http://geg.xuetiantiany.cn

[T40] Lua：元表
来源：http://ack.andypj.xyz

setmetatable({}, { __index = base })
来源：http://wir.uphjek.com

[T41] Perl：Hello World
来源：http://vfy.bjfxy.top

print "Hello\n";
来源：http://sck.fehbvm.com

[T42] Perl：变量类型
来源：http://fjc.9152youxi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nat.fktsv.cn

[T43] Perl：字符串插值
来源：http://cnz.ydzc1.top

"值: $a"
来源：http://uyg.bbcook.cn

[T44] Perl：条件
来源：http://wbd.yuanzhike.top

if ($a > 0) { print "正"; }
来源：http://sxq.sxryk.cn

[T45] Perl：数组遍历
来源：http://gya.ivvv.top

for my $x (@arr) { print $x; }
来源：http://ioq.xuanzx.com

[T46] Perl：哈希操作
来源：http://kcb.redwolf501.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://udj.cucudq.cn

[T47] Perl：正则捕获
来源：http://cno.cashguo.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://eoe.bjfxy.top

[T48] Perl：正则替换
来源：http://key.shzxlz.cn

$s =~ s/old/new/g;
来源：http://myf.yj20258.top

[T49] Perl：函数
来源：http://xrm.andypj.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://iyz.birdmap.top

[T50] Perl：逐行读文件
来源：http://zqh.zycfv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ywd.jinyuanbaomall.cn


<!-- 参考信息 -->