代发 wailian999

find . -name "*.tmp" -delete
来源：http://mhu.yvedp.cn

[R46] 递归替换文件内容
来源：http://foy.nwbrower.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://onu.aizwys.cn

[R47] sed 单行替换
来源：http://toe.hcnkem.com

sed -i 's/foo/bar/g' a.txt
来源：http://ugl.ppjwa.cn

[R48] awk 取指定列
来源：http://czp.shuidangran.top

awk '{print $1, $3}' a.txt
来源：http://zok.yanxiufei.cn

[R49] awk 带条件
来源：http://ywb.nwbrower.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nfl.ydjk.org.cn

[R50] awk 求和
来源：http://bhx.yvedp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ipg.hywenlv.cn

[R51] 排序去重取前几
来源：http://ugo.ybcxt.top

sort a.txt | uniq -c | sort -rn | head
来源：http://tku.sysykeji.top

[R52] 统计行数
来源：http://xio.svipenyu.cn

wc -l a.txt
来源：http://ifg.ydjk.org.cn

[R53] 查看文件头与实时尾
来源：http://tnm.tian-w.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://aok.jinqigufen.top

[R54] 比较两个文件
来源：http://xfp.chenjidiqi.icu

diff a.txt b.txt
来源：http://wyi.daxiang520.top

[R55] 压缩与解压
来源：http://hks.gogol.net.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xqw.chenjidiqi.icu

[R56] 远程拷贝
来源：http://hhy.316326.xyz

scp file user@host:/path/
来源：http://doq.iojbl.cn

[R57] 远程执行命令
来源：http://jql.ivvv.top

ssh user@host 'uptime'
来源：http://vuz.nanxinkj.top

[R58] 下载文件
来源：http://vml.ybcxt.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yyn.jyoumei.cn

[R59] 发 POST JSON
来源：http://btx.dashuyun.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://muv.yangfankeji.com

[R60] 只看 HTTP 状态码
来源：http://ngv.dashuyun.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xfm.jqgufenzy.top

[R61] 磁盘占用
来源：http://phe.hfpthk.cn

df -h;  du -sh *
来源：http://nxt.ppjwa.cn

[R62] 找最占空间的文件
来源：http://cmu.hesvh.cn

du -ah . | sort -rh | head -10
来源：http://liz.gotoacloud.top

[R63] 内存与进程
来源：http://cwj.fktsv.cn

free -h;  ps aux | grep nginx
来源：http://pwj.yuanzhike.top

[R64] 结束进程
来源：http://yuo.gotoacloud.top

kill -9 $(pgrep -f app.py)
来源：http://rva.sweek.top

[R65] 查看端口占用
来源：http://eei.epnwcf.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pda.yonumen.top

[R66] 定时任务
来源：http://ycj.zdqjudy.top

crontab -e;  crontab -l
来源：http://oco.feifeiyinyue.top

[R67] 生成随机十六进制串
来源：http://jhm.wangdashe.top

openssl rand -hex 16
来源：http://kff.dashuyun.cn

[R68] 计算文件校验值
来源：http://exx.kuanghao11.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ojm.sufxvd.cn

[R69] 生成随机密码
来源：http://dot.nwbrower.top

head -c 16 /dev/urandom | base64
来源：http://knc.jinghuilouyu.cn

[R70] 时间戳与互转
来源：http://zhl.316326.xyz

date +%s;  date -d @1700000000
来源：http://wmx.ppjwa.cn

[R71] 日期格式化
来源：http://vvt.fehbvm.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://vcj.gogol.net.cn

[R72] 等待端口就绪
来源：http://dcn.jinqigufen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://yuw.52xcode.cn

[R73] 分割大日志
来源：http://wlp.xylfe.cn

split -l 1000 big.log part_
来源：http://ght.yonumen.top

[R74] 批量重命名
来源：http://ttt.sjlbkw.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dso.gogol.net.cn

[R75] 导出环境变量
来源：http://jiz.ppjwa.cn

export PATH="$HOME/bin:$PATH"
来源：http://cri.chenzaomai.com

[R76] 使用临时文件
来源：http://zud.chenzaomai.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mlc.cheryme.top

[R77] 读取用户输入
来源：http://mhu.ppjwa.cn

read -rp "请输入: " ans
来源：http://ccf.yfazqb.com

[R78] 交互式菜单
来源：http://mbm.zycfv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hfw.chenjidiqi.icu

[R79] 解析命令行选项
来源：http://mti.vqdsnc.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zok.dianchejie.cn

[R80] 查看脚本执行耗时
来源：http://lvb.zycfv.cn

time ./run.sh
来源：http://cwf.cqqwz.cn

================================================================================
来源：http://uht.kuanghao11.cn

S. C / C++ 专题
来源：http://zjj.shanyushiyangtech.top

================================================================================
来源：http://tmv.havefunace.top

[S01] C：Hello World
来源：http://hme.fktsv.cn

#include <stdio.h>
来源：http://nca.ybcxt.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://chm.guowangkeji.top

[S02] C：变量与格式化输出
来源：http://bit.zhongyouzk.top

int a = 10; printf("%d\n", a);
来源：http://qlk.hywenlv.cn

[S03] C：读入整数
来源：http://ors.gaohongyu789.top

int x; scanf("%d", &x);
来源：http://csk.c1oappe.top

[S04] C：字符串复制
来源：http://qcb.mhx1999.top

char dst[32]; strcpy(dst, "hi");
来源：http://qnx.xylfe.cn

[S05] C：字符串长度
来源：http://fjj.jlsjyb.cn

strlen(s)
来源：http://usu.shangyingyoupin.top

[S06] C：字符串比较
来源：http://urq.zhongyouzk.top

strcmp(a, b) == 0
来源：http://hvo.yuxming.cn

[S07] C：数组遍历求和
来源：http://irw.yfazqb.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kme.xinyue.icu

[S08] C：动态内存分配与释放
来源：http://bkn.fzhhl.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://adr.tarul.cn

[S09] C：结构体定义与初始化
来源：http://loa.yj20258888.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kif.52xcode.cn

[S10] C：指针与解引用
来源：http://nra.smart0.xyz

int *p = &a;  *p = 5;
来源：http://pme.hammf.cn

[S11] C：逐行读文件
来源：http://ygz.ydjk.org.cn

FILE *f = fopen("a.txt", "r");
来源：http://fqt.52xcode.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xju.jiagoushi.top

fclose(f);
来源：http://vur.nanxinkj.top

[S12] C：写文件
来源：http://oug.gaohongyu789.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dzu.dianchejie.cn

[S13] C：宏定义
来源：http://myf.dianchejie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zqt.ppjwa.cn

[S14] C：枚举
来源：http://obl.vqdsnc.cn

enum Color { RED, GREEN, BLUE };
来源：http://vzf.cdnleiting.top

[S15] C：类型转换
来源：http://zyo.shangyingyoupin.top

(double) a / b
来源：http://ici.hongshengwenyu.top

[S16] C：位操作置位
来源：http://eyt.birdmap.top

x |= (1 << 3);
来源：http://jgp.hysaishi.cn

[S17] C：安全拼接字符串
来源：http://uac.yfazqb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rkm.daria6918.cn

[S18] C：命令行参数
来源：http://wgb.cqqwz.cn

int main(int argc, char **argv)
来源：http://pne.hesvh.cn

[S19] C：快速排序
来源：http://ywl.fengsongda.top

qsort(a, n, sizeof(int), cmp);
来源：http://equ.jinqigufen.top

[S20] C：二分查找
来源：http://pgi.yj202588.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wyx.havefunace.top

[S21] C：字符类别判断
来源：http://tiy.nwbrower.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vrd.yonumen.top

[S22] C：字符串转数字
来源：http://djr.ydzc1.top

atoi("42");  strtod("3.14", NULL);
来源：http://rdo.havefunace.top

[S23] C：随机数
来源：http://grx.yonumen.top

srand(time(NULL));  int r = rand() % 100;
来源：http://zxf.ydzc1.top

[S24] C：获取本地时间
来源：http://ngo.ctjpmb.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cxj.yfazqb.com

[S25] C：内存拷贝
来源：http://pjt.shangyingyoupin.top

memcpy(dst, src, n);
来源：http://aof.c1oappe.top

[S26] C：内存清零
来源：http://ixn.hcnkem.com

memset(a, 0, sizeof a);
来源：http://xdw.hywenlv.cn

[S27] C：定义常量
来源：http://lra.epnwcf.com

const double PI = 3.14159;
来源：http://nfc.shanyushiyangtech.top

[S28] C：静态变量
来源：http://dvx.zhoulong.xyz

static int counter = 0;
来源：http://eze.sweek.top

[S29] C：变参函数
来源：http://yhp.hywenlv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vka.yj20258888.top

[S30] C：头文件保护
来源：http://fme.hongshengwenyu.top

#ifndef X_H
来源：http://syl.hesvh.cn

#define X_H
来源：http://qmb.feifeiyinyue.top

#endif
来源：http://ymw.52xcode.cn

[S31] C++：Hello World
来源：http://gpi.cdnleiting.top

#include <iostream>
来源：http://mrf.fzhhl.top

int main() { std::cout << "Hello\n"; }
来源：http://rgf.yj20258888.top

[S32] C++：字符串
来源：http://jla.9152youxi.cn

std::string s = "hi";  s += "!";
来源：http://byo.meibo888.top

[S33] C++：vector 增删
来源：http://zyd.meibo888.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rze.wangshuangyany.cn

[S34] C++：遍历 vector
来源：http://wpy.guowangkeji.top

for (auto &x : v) { std::cout << x; }
来源：http://kmc.ywan-chungtsiang.top

[S35] C++：map
来源：http://taw.bjfxy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ayw.yj20258888.top

[S36] C++：unordered_map
来源：http://veg.tarul.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bdm.ctjpmb.com

[S37] C++：set
来源：http://fqi.fehbvm.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mtu.yj20258.top

[S38] C++：排序
来源：http://pvm.havefunace.top

std::sort(v.begin(), v.end());
来源：http://pnj.jianghu66.top

[S39] C++：自定义比较器排序
来源：http://ozp.jinghuilouyu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ufo.kuanghao11.cn

[S40] C++：查找元素
来源：http://fpk.fehbvm.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://erm.wangdashe.top

[S41] C++：类与构造函数
来源：http://boi.meibo888.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ycq.nanxinkj.top

[S42] C++：继承与虚函数
来源：http://rny.yj202588.top

class B : public Base { public: void f() override {} };
来源：http://cfx.cashguo.top

[S43] C++：智能指针
来源：http://gya.jqgfzy.top

auto p = std::make_unique<int>(5);
来源：http://cyt.9152youxi.cn

[S44] C++：引用传参
来源：http://vlx.hfpthk.cn

void inc(int &x) { ++x; }
来源：http://xqq.wangdashe.top

[S45] C++：lambda
来源：http://ibf.jinghuilouyu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://aoq.fanxiaobao.xyz

[S46] C++：函数模板
来源：http://vgo.ppjwa.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ubd.smart0.xyz

[S47] C++：结构化绑定遍历
来源：http://anc.sjlbkw.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://emu.havefunace.top

[S48] C++：逐行读文件
来源：http://nrv.hammf.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ehv.mhx1999.top

while (std::getline(in, line)) { }
来源：http://bng.jianghu66.top

[S49] C++：写文件
来源：http://svf.yonumen.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kqd.andypj.xyz

[S50] C++：格式化数字
来源：http://gvk.hnqzz.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://guc.sjlbkw.cn

[S51] C++：显式类型转换
来源：http://eqm.nwbrower.top

static_cast<double>(a) / b
来源：http://evo.havefunace.top

[S52] C++：const 与 noexcept
来源：http://bpd.xinyue.icu

int size() const noexcept { return n_; }
来源：http://xna.fanxiaobao.xyz

[S53] C++：移动语义
来源：http://oyq.shuidangran.top

std::vector<int> w = std::move(v);
来源：http://omw.shangyingyoupin.top

[S54] C++：异常处理
来源：http://crb.yj202588.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://paq.ydjk.org.cn

[S55] C++：结构化绑定
来源：http://isj.mhx1999.top

auto [a, b] = std::make_pair(1, 2);
来源：http://yqs.c1oappe.top

[S56] C++：optional
来源：http://kcl.sufxvd.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tlc.vehdjk.com

[S57] C++：编译期常量
来源：http://ofr.yueranfly.top

constexpr int N = 10;
来源：http://hjf.vqdsnc.cn

[S58] C++：命名空间
来源：http://gkn.vehdjk.com

namespace ns { int f() { return 1; } }
来源：http://twj.daria6918.cn

[S59] C++：静态断言
来源：http://ggo.fanxiaobao.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kks.316326.xyz

[S60] C++：遍历并删除元素
来源：http://lsz.cqqwz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xli.ydjk.org.cn

================================================================================
来源：http://trx.sjlbkw.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oar.sxryk.cn

================================================================================
来源：http://cdf.cqqwz.cn

[T01] Kotlin：Hello World
来源：http://fil.feifeiyinyue.top

println("Hello")
来源：http://ewr.xylfe.cn

[T02] Kotlin：变量
来源：http://xux.havefunace.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://aoc.cdnleiting.top

[T03] Kotlin：字符串模板
来源：http://gqz.fktsv.cn

"值: $b"
来源：http://nnx.tanke756.top

[T04] Kotlin：空安全
来源：http://vcf.dashuyun.cn

val n: String? = null;  n?.length
来源：http://zhd.ivvv.top

[T05] Kotlin：when 表达式
来源：http://cqc.jianghu66.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ddd.jianghu66.top

[T06] Kotlin：集合映射
来源：http://lcd.nwbrower.top

listOf(1, 2, 3).map { it * 2 }
来源：http://yyq.fehbvm.com

[T07] Kotlin：集合过滤
来源：http://chg.xuetiantiany.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vqi.bjfxy.top

[T08] Kotlin：数据类
来源：http://zpk.hcnkem.com

data class User(val name: String, val age: Int)
来源：http://djg.xuetiantiany.cn

[T09] Kotlin：扩展函数
来源：http://ysg.nanxuanxn.top

fun String.exclaim() = this + "!"
来源：http://quv.cashguo.top

[T10] Kotlin：默认参数
来源：http://xvc.hysaishi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rjl.zhixingplan.top

[T11] Kotlin：协程
来源：http://dkf.dianchejie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jba.hysaishi.cn

[T12] Kotlin：解构声明
来源：http://mgp.sufxvd.cn

val (a, b) = Pair(1, 2)
来源：http://fyr.jinyuanbaomall.cn

[T13] Kotlin：只读 Map
来源：http://pxm.nanxinkj.top

val m = mapOf("a" to 1)
来源：http://vgm.hywenlv.cn

[T14] Kotlin：循环
来源：http://kts.smart0.xyz

for (i in 1..10) println(i)
来源：http://xow.hesvh.cn

[T15] Kotlin：接口
来源：http://vrk.snrcjt.cn

interface Shape { fun area(): Double }
来源：http://ntt.xuetiantiany.cn

[T16] Swift：Hello World
来源：http://pnn.nwbrower.top

print("Hello")
来源：http://vqz.sxryk.cn

[T17] Swift：变量与常量
来源：http://ogy.wangdashe.top

var a = 1;  let b = 2
来源：http://kve.jyoumei.cn

[T18] Swift：字符串插值
来源：http://xgb.ybcxt.top

"值: \(b)"
来源：http://dut.yuanzhike.top

[T19] Swift：可选绑定
来源：http://lvb.sxryk.cn

if let n = opt { print(n) }
来源：http://hdf.snrcjt.cn

[T20] Swift：数组操作
来源：http://rhy.fehbvm.com

var a = [1, 2, 3];  a.append(4)
来源：http://vyb.zhixingplan.top

[T21] Swift：遍历
来源：http://xpe.daria6918.cn

for x in a { print(x) }
来源：http://lmj.yvedp.cn

[T22] Swift：字典
来源：http://kvk.zhoulong.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://xiq.fktsv.cn

[T23] Swift：函数
来源：http://tjj.jinqigufen.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vhn.meibo888.top

[T24] Swift：闭包
来源：http://por.zdqjudy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://aom.sweek.top

[T25] Swift：结构体
来源：http://omg.yongpay.top

struct P { var x: Int }
来源：http://jps.smart0.xyz

[T26] Swift：类与重写
来源：http://byp.quarkkingdee.top

class A: Base { override func f() {} }
来源：http://wyk.guannengcc.top

[T27] Swift：错误处理
来源：http://wag.cqqwz.cn

do { try f() } catch { print(error) }
来源：http://ryy.shuidangran.top

[T28] Swift：枚举
来源：http://zat.shangyingyoupin.top

enum Color { case red, green }
来源：http://mvx.birdmap.top

[T29] Swift：guard 提前返回
来源：http://yrs.yvedp.cn

guard let x = opt else { return }
来源：http://hpy.cqqwz.cn

[T30] Swift：协议
来源：http://xre.ctjpmb.com

protocol Shape { func area() -> Double }
来源：http://mnx.ppjwa.cn

[T31] Lua：Hello World
来源：http://ryt.smart0.xyz

print("Hello")
来源：http://gry.chenzaomai.com

[T32] Lua：局部变量
来源：http://wvu.zhongyouzk.top

local a = 1
来源：http://hys.tanke756.top

[T33] Lua：表（数组）
来源：http://wnj.ctjpmb.com

local t = {1, 2, 3};  t[4] = 4
来源：http://wqm.yuanzhike.top

[T34] Lua：遍历表
来源：http://ajk.epnwcf.com

for i, v in ipairs(t) do print(i, v) end
来源：http://gzc.redwolf501.top

[T35] Lua：字典表
来源：http://hla.9152youxi.cn

local d = { a = 1 };  d.b = 2
来源：http://ybl.vehdjk.com

[T36] Lua：函数
来源：http://ejw.gogol.net.cn

function add(a, b) return a + b end
来源：http://chz.zhixingplan.top

[T37] Lua：字符串拼接
来源：http://pre.zdbjq.cn

"a" .. "b"
来源：http://zfp.epnwcf.com

[T38] Lua：条件
来源：http://qtf.sxryk.cn

if x > 0 then print("正") end
来源：http://hse.hnqzz.top

[T39] Lua：模式匹配
来源：http://yyi.zhijiandao.cn

string.find(s, "%d+")
来源：http://hlc.fehbvm.com

[T40] Lua：元表
来源：http://kgo.yj202588.top

setmetatable({}, { __index = base })
来源：http://jfx.dianchejie.cn

[T41] Perl：Hello World
来源：http://scc.zhijiandao.cn

print "Hello\n";
来源：http://lwp.yfazqb.com

[T42] Perl：变量类型
来源：http://wyh.cucudq.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hjn.wangshuangyany.cn

[T43] Perl：字符串插值
来源：http://usv.sweek.top

"值: $a"
来源：http://fbb.chenzaomai.com

[T44] Perl：条件
来源：http://wow.shuidangran.top

if ($a > 0) { print "正"; }
来源：http://atc.52xcode.cn

[T45] Perl：数组遍历
来源：http://grf.jianghu66.top

for my $x (@arr) { print $x; }
来源：http://wsm.xuetiantiany.cn

[T46] Perl：哈希操作
来源：http://siv.xinyue.icu

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xyx.pycfn.com

[T47] Perl：正则捕获
来源：http://szl.xuanzx.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://nvt.fengsongda.top

[T48] Perl：正则替换
来源：http://mvr.aibaodan.cn

$s =~ s/old/new/g;
来源：http://znk.cdnleiting.top


<!-- 参考信息 -->