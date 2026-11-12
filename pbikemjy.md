代发 wailian999

find . -name "*.log" -type f
来源：http://hwn.xziqi.cn

[R44] 按修改时间查找
来源：http://cwy.jinqigfzy.top

find . -mtime -7 -type f
来源：http://huw.zhongyouzk.top

[R45] 批量删除
来源：http://kik.yuanzhike.top

find . -name "*.tmp" -delete
来源：http://fol.snrcjt.cn

[R46] 递归替换文件内容
来源：http://rxq.xziqi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ryn.jianghu66.top

[R47] sed 单行替换
来源：http://llj.ppjwa.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tfd.hywenlv.cn

[R48] awk 取指定列
来源：http://mlj.jyoumei.cn

awk '{print $1, $3}' a.txt
来源：http://ftx.meibo888.top

[R49] awk 带条件
来源：http://byq.yonumen.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dnb.jinghuilouyu.cn

[R50] awk 求和
来源：http://zvf.hfpthk.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wlp.guannengcc.top

[R51] 排序去重取前几
来源：http://lky.zhiwuduotai.top

sort a.txt | uniq -c | sort -rn | head
来源：http://uew.feifeiyinyue.top

[R52] 统计行数
来源：http://cjn.zycfv.cn

wc -l a.txt
来源：http://eeh.hysaishi.cn

[R53] 查看文件头与实时尾
来源：http://sgo.shanyushiyangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pya.feifeiyinyue.top

[R54] 比较两个文件
来源：http://qlv.zhengqikj.top

diff a.txt b.txt
来源：http://ftc.zdbjq.cn

[R55] 压缩与解压
来源：http://trj.tianlin.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wql.tianlin.xyz

[R56] 远程拷贝
来源：http://lhl.sxryk.cn

scp file user@host:/path/
来源：http://hry.yongpay.top

[R57] 远程执行命令
来源：http://eux.dianchejie.cn

ssh user@host 'uptime'
来源：http://uex.jinqigfzy.top

[R58] 下载文件
来源：http://ngr.cheryme.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dao.guannengcc.top

[R59] 发 POST JSON
来源：http://nzn.epnwcf.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jqs.gotoacloud.top

[R60] 只看 HTTP 状态码
来源：http://uqp.ehwqpu.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kmt.zhiwuduotai.top

[R61] 磁盘占用
来源：http://xxx.feifeiyinyue.top

df -h;  du -sh *
来源：http://ipx.smart0.xyz

[R62] 找最占空间的文件
来源：http://nof.ctjpmb.com

du -ah . | sort -rh | head -10
来源：http://uxu.ydzc1.top

[R63] 内存与进程
来源：http://owk.jinghuilouyu.cn

free -h;  ps aux | grep nginx
来源：http://mwp.jqgfzy.top

[R64] 结束进程
来源：http://asv.ivvv.top

kill -9 $(pgrep -f app.py)
来源：http://pde.c1oappe.top

[R65] 查看端口占用
来源：http://sxj.gotoacloud.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://neq.cucudq.cn

[R66] 定时任务
来源：http://vab.yfazqb.com

crontab -e;  crontab -l
来源：http://igk.zhixingplan.top

[R67] 生成随机十六进制串
来源：http://vyr.xziqi.cn

openssl rand -hex 16
来源：http://wls.ivvv.top

[R68] 计算文件校验值
来源：http://tlt.nanxuanxn.top

sha256sum a.txt;  md5sum a.txt
来源：http://xtz.zhiwuduotai.top

[R69] 生成随机密码
来源：http://uzy.nanxinkj.top

head -c 16 /dev/urandom | base64
来源：http://vel.quarkkingdee.top

[R70] 时间戳与互转
来源：http://rms.0kj1m.cn

date +%s;  date -d @1700000000
来源：http://uzn.jinqigfzy.top

[R71] 日期格式化
来源：http://wbi.yj202588.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jlz.yfazqb.com

[R72] 等待端口就绪
来源：http://uma.ybcxt.top

until nc -z localhost 3306; do sleep 1; done
来源：http://dip.jinghuilouyu.cn

[R73] 分割大日志
来源：http://fmu.cheryme.top

split -l 1000 big.log part_
来源：http://zwu.gotoacloud.top

[R74] 批量重命名
来源：http://jxr.iojbl.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://djd.wangdashe.top

[R75] 导出环境变量
来源：http://bde.yanxiufei.cn

export PATH="$HOME/bin:$PATH"
来源：http://mvy.kuanghao11.cn

[R76] 使用临时文件
来源：http://sdc.gaohongyu789.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rgk.aibaodan.cn

[R77] 读取用户输入
来源：http://dxn.mhx1999.top

read -rp "请输入: " ans
来源：http://ywf.9152youxi.cn

[R78] 交互式菜单
来源：http://gxe.chenzaomai.com

select opt in a b c; do echo "$opt"; break; done
来源：http://krc.chenlongwang.top

[R79] 解析命令行选项
来源：http://rst.yueranfly.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bhn.vehdjk.com

[R80] 查看脚本执行耗时
来源：http://csi.yonumen.top

time ./run.sh
来源：http://vsz.yanxiufei.cn

================================================================================
来源：http://kyo.fanxiaobao.xyz

S. C / C++ 专题
来源：http://rnq.chenjidiqi.icu

================================================================================
来源：http://iaw.xuanzx.com

[S01] C：Hello World
来源：http://hno.aibaodan.cn

#include <stdio.h>
来源：http://wyw.gzhubu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://dlt.yj202588.top

[S02] C：变量与格式化输出
来源：http://skq.aizwys.cn

int a = 10; printf("%d\n", a);
来源：http://kho.tian-w.cn

[S03] C：读入整数
来源：http://hqr.cqqwz.cn

int x; scanf("%d", &x);
来源：http://lwg.ydjk.org.cn

[S04] C：字符串复制
来源：http://cda.gzhubu.top

char dst[32]; strcpy(dst, "hi");
来源：http://lnd.tian-w.cn

[S05] C：字符串长度
来源：http://iqi.zhongyouzk.top

strlen(s)
来源：http://ibq.jqgufenzy.top

[S06] C：字符串比较
来源：http://yvl.aibaodan.cn

strcmp(a, b) == 0
来源：http://urc.iojbl.cn

[S07] C：数组遍历求和
来源：http://aha.shangyingyoupin.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nda.zhaomingkeji.xyz

[S08] C：动态内存分配与释放
来源：http://jmx.yj20258.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lze.gzhubu.top

[S09] C：结构体定义与初始化
来源：http://geg.aizwys.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ypb.aizwys.cn

[S10] C：指针与解引用
来源：http://mgv.guowangkeji.top

int *p = &a;  *p = 5;
来源：http://myf.xingfuxueyuan.xyz

[S11] C：逐行读文件
来源：http://vtn.fzhhl.top

FILE *f = fopen("a.txt", "r");
来源：http://qbw.tarul.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rse.yfazqb.com

fclose(f);
来源：http://nqa.hcnkem.com

[S12] C：写文件
来源：http://oiu.shzxlz.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jmp.ctjpmb.com

[S13] C：宏定义
来源：http://ern.aizwys.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vad.yueranfly.top

[S14] C：枚举
来源：http://mby.havefunace.top

enum Color { RED, GREEN, BLUE };
来源：http://zvl.xylfe.cn

[S15] C：类型转换
来源：http://shg.hesvh.cn

(double) a / b
来源：http://sgb.wangshuangyany.cn

[S16] C：位操作置位
来源：http://gwj.yuxming.cn

x |= (1 << 3);
来源：http://yiq.52xcode.cn

[S17] C：安全拼接字符串
来源：http://lqt.tanke756.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vtz.gogol.net.cn

[S18] C：命令行参数
来源：http://ffp.chenlongwang.top

int main(int argc, char **argv)
来源：http://rgu.yj202588.top

[S19] C：快速排序
来源：http://xcv.sxryk.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kro.cheryme.top

[S20] C：二分查找
来源：http://she.jqgufenzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://clk.nanxinkj.top

[S21] C：字符类别判断
来源：http://joj.yongpay.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rxf.fehbvm.com

[S22] C：字符串转数字
来源：http://vjk.shuidangran.top

atoi("42");  strtod("3.14", NULL);
来源：http://oma.0kj1m.cn

[S23] C：随机数
来源：http://cus.hongshengwenyu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://pyt.yj20258888.top

[S24] C：获取本地时间
来源：http://yqi.meibo888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uyj.zhaomingkeji.xyz

[S25] C：内存拷贝
来源：http://tqv.ivvv.top

memcpy(dst, src, n);
来源：http://qdy.daria6918.cn

[S26] C：内存清零
来源：http://ujd.cucudq.cn

memset(a, 0, sizeof a);
来源：http://vjy.aibaodan.cn

[S27] C：定义常量
来源：http://dfq.shangyingyoupin.top

const double PI = 3.14159;
来源：http://tkw.sjlbkw.cn

[S28] C：静态变量
来源：http://ggl.epnwcf.com

static int counter = 0;
来源：http://cbx.bjfxy.top

[S29] C：变参函数
来源：http://sfu.hysaishi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nbs.zhaomingkeji.xyz

[S30] C：头文件保护
来源：http://qgd.iojbl.cn

#ifndef X_H
来源：http://efy.xziqi.cn

#define X_H
来源：http://jwr.sxryk.cn

#endif
来源：http://maq.chenzaomai.com

[S31] C++：Hello World
来源：http://dln.ehwqpu.com

#include <iostream>
来源：http://dab.guannengcc.top

int main() { std::cout << "Hello\n"; }
来源：http://ots.jqgfzy.top

[S32] C++：字符串
来源：http://jyl.hfpthk.cn

std::string s = "hi";  s += "!";
来源：http://qis.c1oappe.top

[S33] C++：vector 增删
来源：http://ozg.shzxlz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vht.hesvh.cn

[S34] C++：遍历 vector
来源：http://fee.jiagoushi.top

for (auto &x : v) { std::cout << x; }
来源：http://brc.gogol.net.cn

[S35] C++：map
来源：http://mlf.zhaomingkeji.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ugc.316326.xyz

[S36] C++：unordered_map
来源：http://ybs.hfpthk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yib.ehwqpu.com

[S37] C++：set
来源：http://gtx.tarul.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://udl.xingfuxueyuan.xyz

[S38] C++：排序
来源：http://fdb.ehwqpu.com

std::sort(v.begin(), v.end());
来源：http://ujd.iojbl.cn

[S39] C++：自定义比较器排序
来源：http://wbb.shzxlz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mek.wangshuangyany.cn

[S40] C++：查找元素
来源：http://mul.zhongyouzk.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jkw.sxryk.cn

[S41] C++：类与构造函数
来源：http://iym.jinqigfzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uve.iojbl.cn

[S42] C++：继承与虚函数
来源：http://yaz.hfpthk.cn

class B : public Base { public: void f() override {} };
来源：http://pwf.dashuyun.cn

[S43] C++：智能指针
来源：http://llj.yj20258.top

auto p = std::make_unique<int>(5);
来源：http://bfe.yangfankeji.com

[S44] C++：引用传参
来源：http://pvm.yanxiufei.cn

void inc(int &x) { ++x; }
来源：http://rgk.sysykeji.top

[S45] C++：lambda
来源：http://lml.nanxuanxn.top

auto add = [](int a, int b) { return a + b; };
来源：http://hyo.fanxiaobao.xyz

[S46] C++：函数模板
来源：http://qir.jinghuilouyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bza.guowangkeji.top

[S47] C++：结构化绑定遍历
来源：http://hdo.sxryk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://adk.feifeiyinyue.top

[S48] C++：逐行读文件
来源：http://wdx.quarkkingdee.top

std::ifstream in("a.txt");  std::string line;
来源：http://ngs.52xcode.cn

while (std::getline(in, line)) { }
来源：http://jfe.c1oappe.top

[S49] C++：写文件
来源：http://vyv.zhongyouzk.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mjx.kuanghao11.cn

[S50] C++：格式化数字
来源：http://csn.sufxvd.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vmb.shuidangran.top

[S51] C++：显式类型转换
来源：http://bgb.jlsjyb.cn

static_cast<double>(a) / b
来源：http://vji.jianghu66.top

[S52] C++：const 与 noexcept
来源：http://sjg.ydjk.org.cn

int size() const noexcept { return n_; }
来源：http://rei.jianghu66.top

[S53] C++：移动语义
来源：http://ukq.jianghu66.top

std::vector<int> w = std::move(v);
来源：http://rlf.jinyuanbaomall.cn

[S54] C++：异常处理
来源：http://xoe.ybcxt.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qvm.xuetiantiany.cn

[S55] C++：结构化绑定
来源：http://plj.zhijiandao.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gjh.zhixingplan.top

[S56] C++：optional
来源：http://ezc.quarkkingdee.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vag.ybcxt.top

[S57] C++：编译期常量
来源：http://xeu.yangfankeji.com

constexpr int N = 10;
来源：http://pgc.xinyue.icu

[S58] C++：命名空间
来源：http://cfx.daria6918.cn

namespace ns { int f() { return 1; } }
来源：http://woz.jyoumei.cn

[S59] C++：静态断言
来源：http://inj.vehdjk.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uim.hywenlv.cn

[S60] C++：遍历并删除元素
来源：http://jug.haohaochexian.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://muq.ppjwa.cn

================================================================================
来源：http://ycd.zhoulong.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ash.zhongyouzk.top

================================================================================
来源：http://mjr.cashguo.top

[T01] Kotlin：Hello World
来源：http://wyl.tianlin.xyz

println("Hello")
来源：http://jbo.havefunace.top

[T02] Kotlin：变量
来源：http://xmo.xziqi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zud.sjlbkw.cn

[T03] Kotlin：字符串模板
来源：http://spz.iojbl.cn

"值: $b"
来源：http://dos.yueranfly.top

[T04] Kotlin：空安全
来源：http://yaq.svipenyu.cn

val n: String? = null;  n?.length
来源：http://iwp.xuanzx.com

[T05] Kotlin：when 表达式
来源：http://vxq.xylfe.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fpw.jqgfzy.top

[T06] Kotlin：集合映射
来源：http://vsj.zhiwuduotai.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ohs.zhixingplan.top

[T07] Kotlin：集合过滤
来源：http://efv.jiagoushi.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xcs.ppjwa.cn

[T08] Kotlin：数据类
来源：http://ocz.yangfankeji.com

data class User(val name: String, val age: Int)
来源：http://mts.cheryme.top

[T09] Kotlin：扩展函数
来源：http://eeq.redwolf501.top

fun String.exclaim() = this + "!"
来源：http://esf.ivvv.top

[T10] Kotlin：默认参数
来源：http://hnz.ctjpmb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://elj.52xcode.cn

[T11] Kotlin：协程
来源：http://sqy.cheryme.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://csp.c1oappe.top

[T12] Kotlin：解构声明
来源：http://vaq.uphjek.com

val (a, b) = Pair(1, 2)
来源：http://ytr.guannengcc.top

[T13] Kotlin：只读 Map
来源：http://jhm.gzhubu.top

val m = mapOf("a" to 1)
来源：http://lxv.9152youxi.cn

[T14] Kotlin：循环
来源：http://xyq.yanxiufei.cn

for (i in 1..10) println(i)
来源：http://dpp.kuanghao11.cn

[T15] Kotlin：接口
来源：http://rtn.jyoumei.cn

interface Shape { fun area(): Double }
来源：http://reh.jyoumei.cn

[T16] Swift：Hello World
来源：http://hbp.shangyingyoupin.top

print("Hello")
来源：http://ufd.vqdsnc.cn

[T17] Swift：变量与常量
来源：http://kna.fengsongda.top

var a = 1;  let b = 2
来源：http://uxm.nanxinkj.top

[T18] Swift：字符串插值
来源：http://nme.zhaomingkeji.xyz

"值: \(b)"
来源：http://dza.dianchejie.cn

[T19] Swift：可选绑定
来源：http://vje.ybcxt.top

if let n = opt { print(n) }
来源：http://pun.andypj.xyz

[T20] Swift：数组操作
来源：http://tno.andypj.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://rka.feifeiyinyue.top

[T21] Swift：遍历
来源：http://tjs.xingfuxueyuan.xyz

for x in a { print(x) }
来源：http://cxd.dianchejie.cn

[T22] Swift：字典
来源：http://ahq.guowangkeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://tvx.shangyingyoupin.top

[T23] Swift：函数
来源：http://xta.shangyingyoupin.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mzx.sjlbkw.cn

[T24] Swift：闭包
来源：http://yox.vqdsnc.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ief.daria6918.cn

[T25] Swift：结构体
来源：http://ifi.zhixingplan.top

struct P { var x: Int }
来源：http://the.jinqigufen.top

[T26] Swift：类与重写
来源：http://qnc.shanyushiyangtech.top

class A: Base { override func f() {} }
来源：http://fdi.wangshuangyany.cn

[T27] Swift：错误处理
来源：http://xqq.tianlin.xyz

do { try f() } catch { print(error) }
来源：http://uoo.hywenlv.cn

[T28] Swift：枚举
来源：http://bzo.aizwys.cn

enum Color { case red, green }
来源：http://ncp.shanyushiyangtech.top

[T29] Swift：guard 提前返回
来源：http://gyp.yuanzhike.top

guard let x = opt else { return }
来源：http://efv.shanyushiyangtech.top

[T30] Swift：协议
来源：http://gfx.xuetiantiany.cn

protocol Shape { func area() -> Double }
来源：http://vlc.fktsv.cn

[T31] Lua：Hello World
来源：http://ytz.ppjwa.cn

print("Hello")
来源：http://nfy.guannengcc.top

[T32] Lua：局部变量
来源：http://wme.gotoacloud.top

local a = 1
来源：http://inx.zhongyouzk.top

[T33] Lua：表（数组）
来源：http://kip.shanyushiyangtech.top

local t = {1, 2, 3};  t[4] = 4
来源：http://mue.svipenyu.cn

[T34] Lua：遍历表
来源：http://ibz.zhoulong.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://dnm.sweek.top

[T35] Lua：字典表
来源：http://fnx.jqgfzy.top

local d = { a = 1 };  d.b = 2
来源：http://prm.andypj.xyz

[T36] Lua：函数
来源：http://lak.ppjwa.cn

function add(a, b) return a + b end
来源：http://mgr.hcnkem.com

[T37] Lua：字符串拼接
来源：http://xzi.dianchejie.cn

"a" .. "b"
来源：http://ulr.xingfuxueyuan.xyz

[T38] Lua：条件
来源：http://eho.zhixingplan.top

if x > 0 then print("正") end
来源：http://qda.zdqjudy.top

[T39] Lua：模式匹配
来源：http://brq.kuanghao11.cn

string.find(s, "%d+")
来源：http://hbb.jinyuanbaomall.cn

[T40] Lua：元表
来源：http://wjt.feifeiyinyue.top

setmetatable({}, { __index = base })
来源：http://mik.fehbvm.com

[T41] Perl：Hello World
来源：http://ewi.fengsongda.top

print "Hello\n";
来源：http://hoj.haohaochexian.top

[T42] Perl：变量类型
来源：http://goy.cashguo.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zjw.redwolf501.top

[T43] Perl：字符串插值
来源：http://yuw.wangdashe.top

"值: $a"
来源：http://goj.cdnleiting.top

[T44] Perl：条件
来源：http://biy.fanxiaobao.xyz

if ($a > 0) { print "正"; }
来源：http://yyg.nanxinkj.top

[T45] Perl：数组遍历
来源：http://zkk.hnxiangtu.top

for my $x (@arr) { print $x; }
来源：http://ije.tian-w.cn

[T46] Perl：哈希操作
来源：http://fva.hnxiangtu.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bvc.jqgfzy.top


<!-- 参考信息 -->