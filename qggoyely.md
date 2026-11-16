代发 wailian999

cmd >/dev/null 2>&1
来源：http://yxn.aizwys.cn

[R42] 输入重定向
来源：http://xls.nwbrower.top

wc -l < a.txt
来源：http://mys.aibaodan.cn

[R43] 按名字查找文件
来源：http://ygh.jiagoushi.top

find . -name "*.log" -type f
来源：http://pjj.smart0.xyz

[R44] 按修改时间查找
来源：http://zjo.cucudq.cn

find . -mtime -7 -type f
来源：http://xdu.jiagoushi.top

[R45] 批量删除
来源：http://cxy.9152youxi.cn

find . -name "*.tmp" -delete
来源：http://wci.hysaishi.cn

[R46] 递归替换文件内容
来源：http://ene.guannengcc.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dnf.gzhubu.top

[R47] sed 单行替换
来源：http://jdo.yj20258.top

sed -i 's/foo/bar/g' a.txt
来源：http://cxr.jinqigufen.top

[R48] awk 取指定列
来源：http://iok.chenlongwang.top

awk '{print $1, $3}' a.txt
来源：http://ynv.jqgfzy.top

[R49] awk 带条件
来源：http://jei.ydzc1.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://otp.xinyue.icu

[R50] awk 求和
来源：http://dcn.zdbjq.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rtc.tian-w.cn

[R51] 排序去重取前几
来源：http://pxj.snrcjt.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://frh.iojbl.cn

[R52] 统计行数
来源：http://eke.tanke756.top

wc -l a.txt
来源：http://xax.chenjidiqi.icu

[R53] 查看文件头与实时尾
来源：http://bth.fehbvm.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dme.zhijiandao.cn

[R54] 比较两个文件
来源：http://heo.shzxlz.cn

diff a.txt b.txt
来源：http://bvt.wangdashe.top

[R55] 压缩与解压
来源：http://xgl.cheryme.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xhr.guannengcc.top

[R56] 远程拷贝
来源：http://dpv.gogol.net.cn

scp file user@host:/path/
来源：http://hdv.vqdsnc.cn

[R57] 远程执行命令
来源：http://kmk.jqgufenzy.top

ssh user@host 'uptime'
来源：http://eos.0kj1m.cn

[R58] 下载文件
来源：http://vjf.zhijiandao.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://syu.andypj.xyz

[R59] 发 POST JSON
来源：http://ktj.zhiwuduotai.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wyw.uphjek.com

[R60] 只看 HTTP 状态码
来源：http://gtl.aibaodan.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xfi.guannengcc.top

[R61] 磁盘占用
来源：http://lti.ivvv.top

df -h;  du -sh *
来源：http://pcy.zycfv.cn

[R62] 找最占空间的文件
来源：http://yxx.gzhubu.top

du -ah . | sort -rh | head -10
来源：http://xcy.zdbjq.cn

[R63] 内存与进程
来源：http://fll.wangshuangyany.cn

free -h;  ps aux | grep nginx
来源：http://wtp.gogol.net.cn

[R64] 结束进程
来源：http://elg.cdnleiting.top

kill -9 $(pgrep -f app.py)
来源：http://qrh.redwolf501.top

[R65] 查看端口占用
来源：http://ktg.tarul.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dep.cheryme.top

[R66] 定时任务
来源：http://reo.yvedp.cn

crontab -e;  crontab -l
来源：http://ppa.zhijiandao.cn

[R67] 生成随机十六进制串
来源：http://dfl.pycfn.com

openssl rand -hex 16
来源：http://ztw.xuetiantiany.cn

[R68] 计算文件校验值
来源：http://wot.c1oappe.top

sha256sum a.txt;  md5sum a.txt
来源：http://zga.cashguo.top

[R69] 生成随机密码
来源：http://egs.chenlongwang.top

head -c 16 /dev/urandom | base64
来源：http://cyy.hywenlv.cn

[R70] 时间戳与互转
来源：http://kxk.meibo888.top

date +%s;  date -d @1700000000
来源：http://cmm.yangfankeji.com

[R71] 日期格式化
来源：http://psz.birdmap.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://guc.xuanzx.com

[R72] 等待端口就绪
来源：http://idw.sxryk.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rff.316326.xyz

[R73] 分割大日志
来源：http://wxq.gotoacloud.top

split -l 1000 big.log part_
来源：http://nhi.0kj1m.cn

[R74] 批量重命名
来源：http://ima.xuanzx.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yld.fengsongda.top

[R75] 导出环境变量
来源：http://qae.tian-w.cn

export PATH="$HOME/bin:$PATH"
来源：http://bdj.yfazqb.com

[R76] 使用临时文件
来源：http://pnx.hesvh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uid.xziqi.cn

[R77] 读取用户输入
来源：http://rsq.yj202588.top

read -rp "请输入: " ans
来源：http://xdy.0kj1m.cn

[R78] 交互式菜单
来源：http://lfq.chenzaomai.com

select opt in a b c; do echo "$opt"; break; done
来源：http://iar.ivvv.top

[R79] 解析命令行选项
来源：http://kcv.shangyingyoupin.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://azq.zhiwuduotai.top

[R80] 查看脚本执行耗时
来源：http://qyk.tian-w.cn

time ./run.sh
来源：http://cuc.ywan-chungtsiang.top

================================================================================
来源：http://uuj.daria6918.cn

S. C / C++ 专题
来源：http://vby.zhengqikj.top

================================================================================
来源：http://ddr.hongshengwenyu.top

[S01] C：Hello World
来源：http://yqd.ybcxt.top

#include <stdio.h>
来源：http://zmg.ehwqpu.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://ieq.xuanzx.com

[S02] C：变量与格式化输出
来源：http://pke.sxryk.cn

int a = 10; printf("%d\n", a);
来源：http://xbm.meibo888.top

[S03] C：读入整数
来源：http://wko.jiagoushi.top

int x; scanf("%d", &x);
来源：http://yvc.jlsjyb.cn

[S04] C：字符串复制
来源：http://kso.yfazqb.com

char dst[32]; strcpy(dst, "hi");
来源：http://uyi.uphjek.com

[S05] C：字符串长度
来源：http://vcr.hywenlv.cn

strlen(s)
来源：http://zqv.sjlbkw.cn

[S06] C：字符串比较
来源：http://hlq.hywenlv.cn

strcmp(a, b) == 0
来源：http://paq.jyoumei.cn

[S07] C：数组遍历求和
来源：http://xlm.ydzc1.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://obr.xuetiantiany.cn

[S08] C：动态内存分配与释放
来源：http://mdd.sxryk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mvb.smart0.xyz

[S09] C：结构体定义与初始化
来源：http://eok.sysykeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ryx.hnxiangtu.top

[S10] C：指针与解引用
来源：http://ire.fehbvm.com

int *p = &a;  *p = 5;
来源：http://gvh.ydzc1.top

[S11] C：逐行读文件
来源：http://xdz.feifeiyinyue.top

FILE *f = fopen("a.txt", "r");
来源：http://ewh.nanxuanxn.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://jjb.iojbl.cn

fclose(f);
来源：http://ehm.hnqzz.top

[S12] C：写文件
来源：http://faz.aizwys.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ilg.xingfuxueyuan.xyz

[S13] C：宏定义
来源：http://cqg.yonumen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qwh.sufxvd.cn

[S14] C：枚举
来源：http://emx.mhx1999.top

enum Color { RED, GREEN, BLUE };
来源：http://xoj.zdbjq.cn

[S15] C：类型转换
来源：http://uxy.fktsv.cn

(double) a / b
来源：http://ihk.yanxiufei.cn

[S16] C：位操作置位
来源：http://bcc.zhijiandao.cn

x |= (1 << 3);
来源：http://wdv.yj20258.top

[S17] C：安全拼接字符串
来源：http://cdw.cucudq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pfi.yuanzhike.top

[S18] C：命令行参数
来源：http://jtj.yonumen.top

int main(int argc, char **argv)
来源：http://iaa.redwolf501.top

[S19] C：快速排序
来源：http://puf.dashuyun.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lsn.yuanzhike.top

[S20] C：二分查找
来源：http://mwv.bbcook.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hip.andypj.xyz

[S21] C：字符类别判断
来源：http://ahh.pycfn.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://usc.shanyushiyangkeji.top

[S22] C：字符串转数字
来源：http://uxq.yfazqb.com

atoi("42");  strtod("3.14", NULL);
来源：http://xqw.fktsv.cn

[S23] C：随机数
来源：http://rir.gotoacloud.top

srand(time(NULL));  int r = rand() % 100;
来源：http://gqb.bjfxy.top

[S24] C：获取本地时间
来源：http://zjz.redwolf501.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qka.yuxming.cn

[S25] C：内存拷贝
来源：http://nix.chenlongwang.top

memcpy(dst, src, n);
来源：http://rhv.xylfe.cn

[S26] C：内存清零
来源：http://wwq.gaohongyu789.top

memset(a, 0, sizeof a);
来源：http://tvw.zhengqikj.top

[S27] C：定义常量
来源：http://cqk.birdmap.top

const double PI = 3.14159;
来源：http://jfi.xuanzx.com

[S28] C：静态变量
来源：http://exb.tian-w.cn

static int counter = 0;
来源：http://jwo.hcnkem.com

[S29] C：变参函数
来源：http://vhz.hammf.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://egu.tanke756.top

[S30] C：头文件保护
来源：http://orm.redwolf501.top

#ifndef X_H
来源：http://tnq.daxiang520.top

#define X_H
来源：http://kbk.52xcode.cn

#endif
来源：http://rrm.fzhhl.top

[S31] C++：Hello World
来源：http://jrf.jinqigufen.top

#include <iostream>
来源：http://tco.tanke756.top

int main() { std::cout << "Hello\n"; }
来源：http://deb.hfpthk.cn

[S32] C++：字符串
来源：http://mgf.xuetiantiany.cn

std::string s = "hi";  s += "!";
来源：http://yej.yongpay.top

[S33] C++：vector 增删
来源：http://xry.sweek.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mcv.dashuyun.cn

[S34] C++：遍历 vector
来源：http://jgu.xinyue.icu

for (auto &x : v) { std::cout << x; }
来源：http://raq.shuidangran.top

[S35] C++：map
来源：http://kgh.sufxvd.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jdy.sjlbkw.cn

[S36] C++：unordered_map
来源：http://pmu.yonumen.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://avw.aibaodan.cn

[S37] C++：set
来源：http://qde.chenzaomai.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wah.fktsv.cn

[S38] C++：排序
来源：http://ury.zhongyouzk.top

std::sort(v.begin(), v.end());
来源：http://cyc.zhaomingkeji.xyz

[S39] C++：自定义比较器排序
来源：http://ewc.hysaishi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ypo.hcnkem.com

[S40] C++：查找元素
来源：http://byf.fktsv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zov.cheryme.top

[S41] C++：类与构造函数
来源：http://ozx.epnwcf.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xpl.xuanzx.com

[S42] C++：继承与虚函数
来源：http://hcg.wangdashe.top

class B : public Base { public: void f() override {} };
来源：http://ppu.meibo888.top

[S43] C++：智能指针
来源：http://xpd.zhijiandao.cn

auto p = std::make_unique<int>(5);
来源：http://nuv.hnqzz.top

[S44] C++：引用传参
来源：http://kxl.hammf.cn

void inc(int &x) { ++x; }
来源：http://bix.xingfuxueyuan.xyz

[S45] C++：lambda
来源：http://eje.hcnkem.com

auto add = [](int a, int b) { return a + b; };
来源：http://qxf.c1oappe.top

[S46] C++：函数模板
来源：http://pmq.ctjpmb.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xoe.shzxlz.cn

[S47] C++：结构化绑定遍历
来源：http://ysc.hcnkem.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://azl.epnwcf.com

[S48] C++：逐行读文件
来源：http://aka.cucudq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ewj.shanyushiyangtech.top

while (std::getline(in, line)) { }
来源：http://vpp.pycfn.com

[S49] C++：写文件
来源：http://jkh.shuidangran.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ciu.aibaodan.cn

[S50] C++：格式化数字
来源：http://ejr.andypj.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oyh.cashguo.top

[S51] C++：显式类型转换
来源：http://lnc.jqgfzy.top

static_cast<double>(a) / b
来源：http://kin.cqqwz.cn

[S52] C++：const 与 noexcept
来源：http://jbv.daxiang520.top

int size() const noexcept { return n_; }
来源：http://ydb.guowangkeji.top

[S53] C++：移动语义
来源：http://qnf.yj20258888.top

std::vector<int> w = std::move(v);
来源：http://yaa.xziqi.cn

[S54] C++：异常处理
来源：http://pvj.daxiang520.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ibf.hongshengwenyu.top

[S55] C++：结构化绑定
来源：http://jxa.fanxiaobao.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://udo.yueranfly.top

[S56] C++：optional
来源：http://nrj.zhengqikj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://spz.birdmap.top

[S57] C++：编译期常量
来源：http://dby.bbcook.cn

constexpr int N = 10;
来源：http://upr.fengsongda.top

[S58] C++：命名空间
来源：http://pds.gaohongyu789.top

namespace ns { int f() { return 1; } }
来源：http://grn.tanke756.top

[S59] C++：静态断言
来源：http://aia.hongshengwenyu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://biq.bbcook.cn

[S60] C++：遍历并删除元素
来源：http://dju.gogol.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ill.hongshengwenyu.top

================================================================================
来源：http://vym.yj20258.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ipt.ybcxt.top

================================================================================
来源：http://wqe.snrcjt.cn

[T01] Kotlin：Hello World
来源：http://blw.jqgfzy.top

println("Hello")
来源：http://ttu.jinyuanbaomall.cn

[T02] Kotlin：变量
来源：http://ovr.jinyuanbaomall.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://srk.jinqigufen.top

[T03] Kotlin：字符串模板
来源：http://eml.hysaishi.cn

"值: $b"
来源：http://qws.ivvv.top

[T04] Kotlin：空安全
来源：http://clp.ybcxt.top

val n: String? = null;  n?.length
来源：http://tar.bjfxy.top

[T05] Kotlin：when 表达式
来源：http://jgy.vehdjk.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fma.shangyingyoupin.top

[T06] Kotlin：集合映射
来源：http://nrg.jinqigfzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rpb.chenlongwang.top

[T07] Kotlin：集合过滤
来源：http://fvx.quarkkingdee.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://odt.chenlongwang.top

[T08] Kotlin：数据类
来源：http://edk.cdnleiting.top

data class User(val name: String, val age: Int)
来源：http://udr.xylfe.cn

[T09] Kotlin：扩展函数
来源：http://izm.jqgfzy.top

fun String.exclaim() = this + "!"
来源：http://lmp.sjlbkw.cn

[T10] Kotlin：默认参数
来源：http://kqu.zhiwuduotai.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qny.zdbjq.cn

[T11] Kotlin：协程
来源：http://nmx.yvedp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pjx.quarkkingdee.top

[T12] Kotlin：解构声明
来源：http://cjf.smart0.xyz

val (a, b) = Pair(1, 2)
来源：http://zzw.ywan-chungtsiang.top

[T13] Kotlin：只读 Map
来源：http://hst.sjlbkw.cn

val m = mapOf("a" to 1)
来源：http://jkr.nanxinkj.top

[T14] Kotlin：循环
来源：http://gmr.xziqi.cn

for (i in 1..10) println(i)
来源：http://yvb.fktsv.cn

[T15] Kotlin：接口
来源：http://sxr.svipenyu.cn

interface Shape { fun area(): Double }
来源：http://cbx.yfazqb.com

[T16] Swift：Hello World
来源：http://viy.uphjek.com

print("Hello")
来源：http://wjd.yongpay.top

[T17] Swift：变量与常量
来源：http://mkd.wangdashe.top

var a = 1;  let b = 2
来源：http://nls.jianghu66.top

[T18] Swift：字符串插值
来源：http://wsv.redwolf501.top

"值: \(b)"
来源：http://lnq.shanyushiyangtech.top

[T19] Swift：可选绑定
来源：http://rkd.bbcook.cn

if let n = opt { print(n) }
来源：http://kdc.9152youxi.cn

[T20] Swift：数组操作
来源：http://iyx.meibo888.top

var a = [1, 2, 3];  a.append(4)
来源：http://uza.chenjidiqi.icu

[T21] Swift：遍历
来源：http://ter.aizwys.cn

for x in a { print(x) }
来源：http://khr.xuanzx.com

[T22] Swift：字典
来源：http://bsy.fehbvm.com

var d = ["a": 1];  d["b"] = 2
来源：http://ezi.hongshengwenyu.top

[T23] Swift：函数
来源：http://wrk.wangshuangyany.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sdz.zhoulong.xyz

[T24] Swift：闭包
来源：http://zgf.shuidangran.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://mdc.yueranfly.top

[T25] Swift：结构体
来源：http://lfb.epnwcf.com

struct P { var x: Int }
来源：http://pjs.xuanzx.com

[T26] Swift：类与重写
来源：http://qit.smart0.xyz

class A: Base { override func f() {} }
来源：http://wig.xylfe.cn

[T27] Swift：错误处理
来源：http://svw.yj20258.top

do { try f() } catch { print(error) }
来源：http://lxc.wangshuangyany.cn

[T28] Swift：枚举
来源：http://qgf.c1oappe.top

enum Color { case red, green }
来源：http://jre.gogol.net.cn

[T29] Swift：guard 提前返回
来源：http://dls.zhaomingkeji.xyz

guard let x = opt else { return }
来源：http://hnc.smart0.xyz

[T30] Swift：协议
来源：http://wgw.epnwcf.com

protocol Shape { func area() -> Double }
来源：http://emu.gogol.net.cn

[T31] Lua：Hello World
来源：http://fyi.jinyuanbaomall.cn

print("Hello")
来源：http://sty.fktsv.cn

[T32] Lua：局部变量
来源：http://khd.tian-w.cn

local a = 1
来源：http://epw.fehbvm.com

[T33] Lua：表（数组）
来源：http://oyf.zhengqikj.top

local t = {1, 2, 3};  t[4] = 4
来源：http://tjw.zhixingplan.top

[T34] Lua：遍历表
来源：http://xpq.guannengcc.top

for i, v in ipairs(t) do print(i, v) end
来源：http://czu.smart0.xyz

[T35] Lua：字典表
来源：http://yrj.0kj1m.cn

local d = { a = 1 };  d.b = 2
来源：http://uwo.hywenlv.cn

[T36] Lua：函数
来源：http://fhs.xuanzx.com

function add(a, b) return a + b end
来源：http://ilp.havefunace.top

[T37] Lua：字符串拼接
来源：http://nde.jinghuilouyu.cn

"a" .. "b"
来源：http://fsp.52xcode.cn

[T38] Lua：条件
来源：http://cmx.zhongyouzk.top

if x > 0 then print("正") end
来源：http://imm.zhiwuduotai.top

[T39] Lua：模式匹配
来源：http://puc.0kj1m.cn

string.find(s, "%d+")
来源：http://bne.shzxlz.cn

[T40] Lua：元表
来源：http://nfw.cdnleiting.top

setmetatable({}, { __index = base })
来源：http://zzx.guannengcc.top

[T41] Perl：Hello World
来源：http://ssr.zhongyouzk.top

print "Hello\n";
来源：http://ubr.nanxuanxn.top

[T42] Perl：变量类型
来源：http://xlb.birdmap.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://plf.hesvh.cn

[T43] Perl：字符串插值
来源：http://vaz.jinqigfzy.top

"值: $a"
来源：http://mxy.chenjidiqi.icu

[T44] Perl：条件
来源：http://ilc.guowangkeji.top

if ($a > 0) { print "正"; }
来源：http://nmr.guannengcc.top


<!-- 参考信息 -->