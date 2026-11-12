代发 wailian999

files=$(ls -1)
来源：http://twc.gaohongyu789.top

[R38] 管道串联
来源：http://djh.jinyuanbaomall.cn

cat a.txt | grep -i error | wc -l
来源：http://ukm.zdqjudy.top

[R39] 重定向标准输出与错误
来源：http://nbz.fehbvm.com

cmd > out.log 2>&1
来源：http://ywu.cdnleiting.top

[R40] 追加写日志
来源：http://kyr.yfazqb.com

echo "log" >> out.log
来源：http://vwp.cucudq.cn

[R41] 丢弃输出
来源：http://vub.gotoacloud.top

cmd >/dev/null 2>&1
来源：http://ode.zhongyouzk.top

[R42] 输入重定向
来源：http://hel.zhengqikj.top

wc -l < a.txt
来源：http://crh.shuidangran.top

[R43] 按名字查找文件
来源：http://qxq.mhx1999.top

find . -name "*.log" -type f
来源：http://ebu.fengsongda.top

[R44] 按修改时间查找
来源：http://uvw.snrcjt.cn

find . -mtime -7 -type f
来源：http://flm.chenzaomai.com

[R45] 批量删除
来源：http://djp.hfpthk.cn

find . -name "*.tmp" -delete
来源：http://miq.yj20258888.top

[R46] 递归替换文件内容
来源：http://glu.svipenyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ibc.xziqi.cn

[R47] sed 单行替换
来源：http://mky.daria6918.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gol.yangfankeji.com

[R48] awk 取指定列
来源：http://eev.cdnleiting.top

awk '{print $1, $3}' a.txt
来源：http://flm.jinqigufen.top

[R49] awk 带条件
来源：http://amy.xuanzx.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zje.yj20258888.top

[R50] awk 求和
来源：http://kxd.tian-w.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hqa.fengsongda.top

[R51] 排序去重取前几
来源：http://iyw.vehdjk.com

sort a.txt | uniq -c | sort -rn | head
来源：http://vyj.epnwcf.com

[R52] 统计行数
来源：http://fpv.svipenyu.cn

wc -l a.txt
来源：http://oon.chenlongwang.top

[R53] 查看文件头与实时尾
来源：http://isy.dashuyun.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lgh.sufxvd.cn

[R54] 比较两个文件
来源：http://mxl.zhijiandao.cn

diff a.txt b.txt
来源：http://lgq.guowangkeji.top

[R55] 压缩与解压
来源：http://ghk.fzhhl.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://iuw.zhengqikj.top

[R56] 远程拷贝
来源：http://zmw.zhoulong.xyz

scp file user@host:/path/
来源：http://fwt.jlsjyb.cn

[R57] 远程执行命令
来源：http://pwa.zhongyouzk.top

ssh user@host 'uptime'
来源：http://mrc.vehdjk.com

[R58] 下载文件
来源：http://zii.cashguo.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cud.jinghuilouyu.cn

[R59] 发 POST JSON
来源：http://nza.hnqzz.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qrq.ydzc1.top

[R60] 只看 HTTP 状态码
来源：http://gkw.zhixingplan.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gso.cheryme.top

[R61] 磁盘占用
来源：http://kba.fzhhl.top

df -h;  du -sh *
来源：http://uvs.yanxiufei.cn

[R62] 找最占空间的文件
来源：http://tju.kuanghao11.cn

du -ah . | sort -rh | head -10
来源：http://jpi.guowangkeji.top

[R63] 内存与进程
来源：http://oem.vqdsnc.cn

free -h;  ps aux | grep nginx
来源：http://rsq.ppjwa.cn

[R64] 结束进程
来源：http://dfa.sweek.top

kill -9 $(pgrep -f app.py)
来源：http://rzs.chenzaomai.com

[R65] 查看端口占用
来源：http://xir.fktsv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xvw.hcnkem.com

[R66] 定时任务
来源：http://mdy.pycfn.com

crontab -e;  crontab -l
来源：http://ngy.uphjek.com

[R67] 生成随机十六进制串
来源：http://wcw.yangfankeji.com

openssl rand -hex 16
来源：http://ths.yonumen.top

[R68] 计算文件校验值
来源：http://vms.hysaishi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nrj.52xcode.cn

[R69] 生成随机密码
来源：http://que.nanxuanxn.top

head -c 16 /dev/urandom | base64
来源：http://rsj.hesvh.cn

[R70] 时间戳与互转
来源：http://knl.andypj.xyz

date +%s;  date -d @1700000000
来源：http://msf.shangyingyoupin.top

[R71] 日期格式化
来源：http://jid.bjfxy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ipl.andypj.xyz

[R72] 等待端口就绪
来源：http://cvw.fehbvm.com

until nc -z localhost 3306; do sleep 1; done
来源：http://sqo.tanke756.top

[R73] 分割大日志
来源：http://xws.yonumen.top

split -l 1000 big.log part_
来源：http://gfb.jqgufenzy.top

[R74] 批量重命名
来源：http://jso.jinqigfzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fst.shzxlz.cn

[R75] 导出环境变量
来源：http://mpx.daxiang520.top

export PATH="$HOME/bin:$PATH"
来源：http://fjt.gogol.net.cn

[R76] 使用临时文件
来源：http://ike.jyoumei.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yzg.nwbrower.top

[R77] 读取用户输入
来源：http://jhh.ydzc1.top

read -rp "请输入: " ans
来源：http://yku.chenjidiqi.icu

[R78] 交互式菜单
来源：http://vgi.dianchejie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zct.daxiang520.top

[R79] 解析命令行选项
来源：http://jua.shangyingyoupin.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pkg.quarkkingdee.top

[R80] 查看脚本执行耗时
来源：http://uav.xinyue.icu

time ./run.sh
来源：http://dvg.cashguo.top

================================================================================
来源：http://nfp.birdmap.top

S. C / C++ 专题
来源：http://rjf.fktsv.cn

================================================================================
来源：http://zsz.mhx1999.top

[S01] C：Hello World
来源：http://nsa.jqgufenzy.top

#include <stdio.h>
来源：http://uzk.gaohongyu789.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://kfn.havefunace.top

[S02] C：变量与格式化输出
来源：http://hcy.yueranfly.top

int a = 10; printf("%d\n", a);
来源：http://ttn.fanxiaobao.xyz

[S03] C：读入整数
来源：http://hcy.fktsv.cn

int x; scanf("%d", &x);
来源：http://iex.redwolf501.top

[S04] C：字符串复制
来源：http://msv.yuxming.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hyh.hesvh.cn

[S05] C：字符串长度
来源：http://qyp.gaohongyu789.top

strlen(s)
来源：http://mxe.gzhubu.top

[S06] C：字符串比较
来源：http://zem.sjlbkw.cn

strcmp(a, b) == 0
来源：http://eil.pengpengdd.cyou

[S07] C：数组遍历求和
来源：http://mrn.fzhhl.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mpw.hongshengwenyu.top

[S08] C：动态内存分配与释放
来源：http://qyb.fktsv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xbj.svipenyu.cn

[S09] C：结构体定义与初始化
来源：http://lii.hysaishi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fuq.hammf.cn

[S10] C：指针与解引用
来源：http://adr.hnqzz.top

int *p = &a;  *p = 5;
来源：http://aml.cashguo.top

[S11] C：逐行读文件
来源：http://krx.gaohongyu789.top

FILE *f = fopen("a.txt", "r");
来源：http://anq.zdbjq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zmb.hnxiangtu.top

fclose(f);
来源：http://por.chenlongwang.top

[S12] C：写文件
来源：http://exu.mhx1999.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://eqv.fanxiaobao.xyz

[S13] C：宏定义
来源：http://lyx.smart0.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zdw.gogol.net.cn

[S14] C：枚举
来源：http://sfm.daxiang520.top

enum Color { RED, GREEN, BLUE };
来源：http://lhr.xylfe.cn

[S15] C：类型转换
来源：http://ynv.xylfe.cn

(double) a / b
来源：http://zud.zhijiandao.cn

[S16] C：位操作置位
来源：http://qxn.yvedp.cn

x |= (1 << 3);
来源：http://myt.tianlin.xyz

[S17] C：安全拼接字符串
来源：http://zsw.316326.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pul.havefunace.top

[S18] C：命令行参数
来源：http://ozn.ywan-chungtsiang.top

int main(int argc, char **argv)
来源：http://hmt.0kj1m.cn

[S19] C：快速排序
来源：http://nso.jqgufenzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://vua.chenlongwang.top

[S20] C：二分查找
来源：http://dek.jiagoushi.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ypw.vqdsnc.cn

[S21] C：字符类别判断
来源：http://uxr.ctjpmb.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://trt.tarul.cn

[S22] C：字符串转数字
来源：http://tay.gotoacloud.top

atoi("42");  strtod("3.14", NULL);
来源：http://rpy.yvedp.cn

[S23] C：随机数
来源：http://piv.yueranfly.top

srand(time(NULL));  int r = rand() % 100;
来源：http://cqe.smart0.xyz

[S24] C：获取本地时间
来源：http://quc.ywan-chungtsiang.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gyw.feifeiyinyue.top

[S25] C：内存拷贝
来源：http://lxk.jianghu66.top

memcpy(dst, src, n);
来源：http://jjt.ybcxt.top

[S26] C：内存清零
来源：http://qpi.sweek.top

memset(a, 0, sizeof a);
来源：http://sbj.zdqjudy.top

[S27] C：定义常量
来源：http://sco.chenjidiqi.icu

const double PI = 3.14159;
来源：http://mho.sweek.top

[S28] C：静态变量
来源：http://ful.hammf.cn

static int counter = 0;
来源：http://aow.bjfxy.top

[S29] C：变参函数
来源：http://mqk.hysaishi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rky.guowangkeji.top

[S30] C：头文件保护
来源：http://cly.dianchejie.cn

#ifndef X_H
来源：http://fjd.nanxuanxn.top

#define X_H
来源：http://aft.tarul.cn

#endif
来源：http://tyg.ctjpmb.com

[S31] C++：Hello World
来源：http://yfx.yueranfly.top

#include <iostream>
来源：http://peq.tarul.cn

int main() { std::cout << "Hello\n"; }
来源：http://kyj.feifeiyinyue.top

[S32] C++：字符串
来源：http://jfm.zhijiandao.cn

std::string s = "hi";  s += "!";
来源：http://czw.xingfuxueyuan.xyz

[S33] C++：vector 增删
来源：http://ego.chenzaomai.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fmu.316326.xyz

[S34] C++：遍历 vector
来源：http://wfw.jyoumei.cn

for (auto &x : v) { std::cout << x; }
来源：http://eeb.yonumen.top

[S35] C++：map
来源：http://djz.quarkkingdee.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sae.sysykeji.top

[S36] C++：unordered_map
来源：http://vws.feifeiyinyue.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xca.shanyushiyangkeji.top

[S37] C++：set
来源：http://hpp.jiagoushi.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jmq.tian-w.cn

[S38] C++：排序
来源：http://nak.shangyingyoupin.top

std::sort(v.begin(), v.end());
来源：http://ljl.haohaochexian.top

[S39] C++：自定义比较器排序
来源：http://olc.gogol.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://spb.zhoulong.xyz

[S40] C++：查找元素
来源：http://ahv.hongshengwenyu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sdz.iojbl.cn

[S41] C++：类与构造函数
来源：http://qti.hesvh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mmy.0kj1m.cn

[S42] C++：继承与虚函数
来源：http://kgv.fengsongda.top

class B : public Base { public: void f() override {} };
来源：http://csz.uphjek.com

[S43] C++：智能指针
来源：http://nny.sweek.top

auto p = std::make_unique<int>(5);
来源：http://tvg.pycfn.com

[S44] C++：引用传参
来源：http://ytu.316326.xyz

void inc(int &x) { ++x; }
来源：http://kvp.sxryk.cn

[S45] C++：lambda
来源：http://fcl.xuetiantiany.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ijm.xinyue.icu

[S46] C++：函数模板
来源：http://lql.pengpengdd.cyou

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qnj.epnwcf.com

[S47] C++：结构化绑定遍历
来源：http://vwc.yvedp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kqe.shangyingyoupin.top

[S48] C++：逐行读文件
来源：http://jij.fehbvm.com

std::ifstream in("a.txt");  std::string line;
来源：http://jwr.hcnkem.com

while (std::getline(in, line)) { }
来源：http://wow.guannengcc.top

[S49] C++：写文件
来源：http://sby.yongpay.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ram.yfazqb.com

[S50] C++：格式化数字
来源：http://ozm.yangfankeji.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jdd.iojbl.cn

[S51] C++：显式类型转换
来源：http://cwl.tanke756.top

static_cast<double>(a) / b
来源：http://zsq.zhixingplan.top

[S52] C++：const 与 noexcept
来源：http://aul.fehbvm.com

int size() const noexcept { return n_; }
来源：http://ofl.hnqzz.top

[S53] C++：移动语义
来源：http://hkw.sweek.top

std::vector<int> w = std::move(v);
来源：http://yes.birdmap.top

[S54] C++：异常处理
来源：http://nhm.zhaomingkeji.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sku.haohaochexian.top

[S55] C++：结构化绑定
来源：http://udh.chenzaomai.com

auto [a, b] = std::make_pair(1, 2);
来源：http://ogc.wangshuangyany.cn

[S56] C++：optional
来源：http://pcy.xylfe.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uub.zhoulong.xyz

[S57] C++：编译期常量
来源：http://qrx.hnqzz.top

constexpr int N = 10;
来源：http://zrs.ehwqpu.com

[S58] C++：命名空间
来源：http://hau.9152youxi.cn

namespace ns { int f() { return 1; } }
来源：http://zia.xingfuxueyuan.xyz

[S59] C++：静态断言
来源：http://ldp.hfpthk.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nga.xuanzx.com

[S60] C++：遍历并删除元素
来源：http://jfq.hongshengwenyu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jgn.hesvh.cn

================================================================================
来源：http://ziw.zhengqikj.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wdl.xziqi.cn

================================================================================
来源：http://ljj.dianchejie.cn

[T01] Kotlin：Hello World
来源：http://nzw.xingfuxueyuan.xyz

println("Hello")
来源：http://wza.sysykeji.top

[T02] Kotlin：变量
来源：http://zxh.sjlbkw.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rby.birdmap.top

[T03] Kotlin：字符串模板
来源：http://iln.havefunace.top

"值: $b"
来源：http://zrw.ywan-chungtsiang.top

[T04] Kotlin：空安全
来源：http://fns.316326.xyz

val n: String? = null;  n?.length
来源：http://jer.cashguo.top

[T05] Kotlin：when 表达式
来源：http://evk.haohaochexian.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://shh.chenlongwang.top

[T06] Kotlin：集合映射
来源：http://qxc.cashguo.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tby.ehwqpu.com

[T07] Kotlin：集合过滤
来源：http://xte.pengpengdd.cyou

listOf(1, 2, 3).filter { it > 1 }
来源：http://pwn.bjfxy.top

[T08] Kotlin：数据类
来源：http://bdh.yfazqb.com

data class User(val name: String, val age: Int)
来源：http://ukl.svipenyu.cn

[T09] Kotlin：扩展函数
来源：http://xpa.0kj1m.cn

fun String.exclaim() = this + "!"
来源：http://shh.yfazqb.com

[T10] Kotlin：默认参数
来源：http://pjn.redwolf501.top

fun greet(name: String = "World") = "Hi $name"
来源：http://opw.zdbjq.cn

[T11] Kotlin：协程
来源：http://kul.dashuyun.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://aer.0kj1m.cn

[T12] Kotlin：解构声明
来源：http://dcs.jiagoushi.top

val (a, b) = Pair(1, 2)
来源：http://wqk.guowangkeji.top

[T13] Kotlin：只读 Map
来源：http://zgh.yj20258.top

val m = mapOf("a" to 1)
来源：http://wmd.shangyingyoupin.top

[T14] Kotlin：循环
来源：http://syz.ydzc1.top

for (i in 1..10) println(i)
来源：http://quy.gzhubu.top

[T15] Kotlin：接口
来源：http://wbc.yuxming.cn

interface Shape { fun area(): Double }
来源：http://hyw.yuxming.cn

[T16] Swift：Hello World
来源：http://jej.ywan-chungtsiang.top

print("Hello")
来源：http://mko.chenlongwang.top

[T17] Swift：变量与常量
来源：http://dep.jianghu66.top

var a = 1;  let b = 2
来源：http://bar.sweek.top

[T18] Swift：字符串插值
来源：http://kxm.shanyushiyangkeji.top

"值: \(b)"
来源：http://ebb.havefunace.top

[T19] Swift：可选绑定
来源：http://dgb.guannengcc.top

if let n = opt { print(n) }
来源：http://zen.hcnkem.com

[T20] Swift：数组操作
来源：http://auc.redwolf501.top

var a = [1, 2, 3];  a.append(4)
来源：http://ebd.jinyuanbaomall.cn

[T21] Swift：遍历
来源：http://gde.yvedp.cn

for x in a { print(x) }
来源：http://vus.jqgufenzy.top

[T22] Swift：字典
来源：http://iiu.iojbl.cn

var d = ["a": 1];  d["b"] = 2
来源：http://moy.hfpthk.cn

[T23] Swift：函数
来源：http://cno.feifeiyinyue.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tae.zhengqikj.top

[T24] Swift：闭包
来源：http://wtf.c1oappe.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://vyb.kuanghao11.cn

[T25] Swift：结构体
来源：http://uvy.zhaomingkeji.xyz

struct P { var x: Int }
来源：http://drq.smart0.xyz

[T26] Swift：类与重写
来源：http://qtk.meibo888.top

class A: Base { override func f() {} }
来源：http://kfe.52xcode.cn

[T27] Swift：错误处理
来源：http://ayf.zhoulong.xyz

do { try f() } catch { print(error) }
来源：http://hvo.guowangkeji.top

[T28] Swift：枚举
来源：http://nie.yj20258888.top

enum Color { case red, green }
来源：http://pny.xingfuxueyuan.xyz

[T29] Swift：guard 提前返回
来源：http://vuf.epnwcf.com

guard let x = opt else { return }
来源：http://bpg.meibo888.top

[T30] Swift：协议
来源：http://aua.tianlin.xyz

protocol Shape { func area() -> Double }
来源：http://dwq.yj20258888.top

[T31] Lua：Hello World
来源：http://jjy.pengpengdd.cyou

print("Hello")
来源：http://vfz.vqdsnc.cn

[T32] Lua：局部变量
来源：http://tii.fengsongda.top

local a = 1
来源：http://kmo.sufxvd.cn

[T33] Lua：表（数组）
来源：http://jdk.havefunace.top

local t = {1, 2, 3};  t[4] = 4
来源：http://urt.sweek.top

[T34] Lua：遍历表
来源：http://sxo.yongpay.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ihk.redwolf501.top

[T35] Lua：字典表
来源：http://lqu.snrcjt.cn

local d = { a = 1 };  d.b = 2
来源：http://zck.sufxvd.cn

[T36] Lua：函数
来源：http://hto.nanxinkj.top

function add(a, b) return a + b end
来源：http://dlr.fengsongda.top

[T37] Lua：字符串拼接
来源：http://nee.vqdsnc.cn

"a" .. "b"
来源：http://ysm.chenjidiqi.icu

[T38] Lua：条件
来源：http://szr.jqgfzy.top

if x > 0 then print("正") end
来源：http://ygc.hcnkem.com

[T39] Lua：模式匹配
来源：http://dsm.zhoulong.xyz

string.find(s, "%d+")
来源：http://ari.tianlin.xyz

[T40] Lua：元表
来源：http://pdw.yj20258.top

setmetatable({}, { __index = base })
来源：http://cjk.yanxiufei.cn


<!-- 参考信息 -->