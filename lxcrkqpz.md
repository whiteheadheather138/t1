代发 wailian999

cmd > out.log 2>&1
来源：http://cze.vqdsnc.cn

[R40] 追加写日志
来源：http://krx.c1oappe.top

echo "log" >> out.log
来源：http://idc.zhixingplan.top

[R41] 丢弃输出
来源：http://yio.daria6918.cn

cmd >/dev/null 2>&1
来源：http://tvf.yj20258.top

[R42] 输入重定向
来源：http://upq.tarul.cn

wc -l < a.txt
来源：http://pto.jqgfzy.top

[R43] 按名字查找文件
来源：http://adc.guowangkeji.top

find . -name "*.log" -type f
来源：http://fuv.aibaodan.cn

[R44] 按修改时间查找
来源：http://zsp.yongpay.top

find . -mtime -7 -type f
来源：http://xhp.9152youxi.cn

[R45] 批量删除
来源：http://lxl.guannengcc.top

find . -name "*.tmp" -delete
来源：http://wsz.daxiang520.top

[R46] 递归替换文件内容
来源：http://jtk.chenlongwang.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xzs.ehwqpu.com

[R47] sed 单行替换
来源：http://joz.zhixingplan.top

sed -i 's/foo/bar/g' a.txt
来源：http://tir.vqdsnc.cn

[R48] awk 取指定列
来源：http://tks.dianchejie.cn

awk '{print $1, $3}' a.txt
来源：http://lkx.yfazqb.com

[R49] awk 带条件
来源：http://ysw.wangdashe.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qyn.wangdashe.top

[R50] awk 求和
来源：http://gty.zhixingplan.top

awk '{s += $2} END {print s}' a.txt
来源：http://gjs.yvedp.cn

[R51] 排序去重取前几
来源：http://qlu.hesvh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tzy.zycfv.cn

[R52] 统计行数
来源：http://nsl.shanyushiyangkeji.top

wc -l a.txt
来源：http://hgh.ydzc1.top

[R53] 查看文件头与实时尾
来源：http://mtj.pycfn.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dve.hongshengwenyu.top

[R54] 比较两个文件
来源：http://uur.hysaishi.cn

diff a.txt b.txt
来源：http://yeb.yfazqb.com

[R55] 压缩与解压
来源：http://rox.dashuyun.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cxe.smart0.xyz

[R56] 远程拷贝
来源：http://cmi.haohaochexian.top

scp file user@host:/path/
来源：http://kmn.gogol.net.cn

[R57] 远程执行命令
来源：http://hkj.chenjidiqi.icu

ssh user@host 'uptime'
来源：http://dce.chenlongwang.top

[R58] 下载文件
来源：http://ljp.pengpengdd.cyou

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tcy.fengsongda.top

[R59] 发 POST JSON
来源：http://pdt.jinghuilouyu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bkx.epnwcf.com

[R60] 只看 HTTP 状态码
来源：http://qzz.kuanghao11.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://otc.fktsv.cn

[R61] 磁盘占用
来源：http://epj.quarkkingdee.top

df -h;  du -sh *
来源：http://chx.sxryk.cn

[R62] 找最占空间的文件
来源：http://gqc.hnqzz.top

du -ah . | sort -rh | head -10
来源：http://gri.hysaishi.cn

[R63] 内存与进程
来源：http://qmc.sysykeji.top

free -h;  ps aux | grep nginx
来源：http://lly.aibaodan.cn

[R64] 结束进程
来源：http://wxv.nanxinkj.top

kill -9 $(pgrep -f app.py)
来源：http://szp.sufxvd.cn

[R65] 查看端口占用
来源：http://tjp.nanxinkj.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://efd.quarkkingdee.top

[R66] 定时任务
来源：http://aal.xuetiantiany.cn

crontab -e;  crontab -l
来源：http://rpy.uphjek.com

[R67] 生成随机十六进制串
来源：http://zjq.zycfv.cn

openssl rand -hex 16
来源：http://idr.fengsongda.top

[R68] 计算文件校验值
来源：http://qrv.shzxlz.cn

sha256sum a.txt;  md5sum a.txt
来源：http://sdp.fehbvm.com

[R69] 生成随机密码
来源：http://qeu.bjfxy.top

head -c 16 /dev/urandom | base64
来源：http://fyl.0kj1m.cn

[R70] 时间戳与互转
来源：http://qbr.tarul.cn

date +%s;  date -d @1700000000
来源：http://ebt.hnqzz.top

[R71] 日期格式化
来源：http://sxz.uphjek.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://wbc.jinyuanbaomall.cn

[R72] 等待端口就绪
来源：http://dfq.snrcjt.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gbx.quarkkingdee.top

[R73] 分割大日志
来源：http://dmk.jinqigufen.top

split -l 1000 big.log part_
来源：http://zvl.fengsongda.top

[R74] 批量重命名
来源：http://hsl.fzhhl.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hjk.yanxiufei.cn

[R75] 导出环境变量
来源：http://ord.jlsjyb.cn

export PATH="$HOME/bin:$PATH"
来源：http://ass.shzxlz.cn

[R76] 使用临时文件
来源：http://mrg.cdnleiting.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://azk.quarkkingdee.top

[R77] 读取用户输入
来源：http://lgm.bjfxy.top

read -rp "请输入: " ans
来源：http://ifo.dashuyun.cn

[R78] 交互式菜单
来源：http://fwm.zycfv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://btv.havefunace.top

[R79] 解析命令行选项
来源：http://ibm.yongpay.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fuq.yangfankeji.com

[R80] 查看脚本执行耗时
来源：http://tcr.shanyushiyangtech.top

time ./run.sh
来源：http://smp.redwolf501.top

================================================================================
来源：http://ffv.andypj.xyz

S. C / C++ 专题
来源：http://kdf.sufxvd.cn

================================================================================
来源：http://yht.jinqigufen.top

[S01] C：Hello World
来源：http://hna.xuetiantiany.cn

#include <stdio.h>
来源：http://gsw.c1oappe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rfy.sweek.top

[S02] C：变量与格式化输出
来源：http://isp.bbcook.cn

int a = 10; printf("%d\n", a);
来源：http://hxp.redwolf501.top

[S03] C：读入整数
来源：http://kcy.nwbrower.top

int x; scanf("%d", &x);
来源：http://ruf.fengsongda.top

[S04] C：字符串复制
来源：http://moy.fengsongda.top

char dst[32]; strcpy(dst, "hi");
来源：http://xaq.jinqigufen.top

[S05] C：字符串长度
来源：http://acg.smart0.xyz

strlen(s)
来源：http://wpe.haohaochexian.top

[S06] C：字符串比较
来源：http://trf.xuetiantiany.cn

strcmp(a, b) == 0
来源：http://txa.gzhubu.top

[S07] C：数组遍历求和
来源：http://sod.bjfxy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xdf.feifeiyinyue.top

[S08] C：动态内存分配与释放
来源：http://jom.pycfn.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tbx.bbcook.cn

[S09] C：结构体定义与初始化
来源：http://nte.aibaodan.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://szp.shanyushiyangkeji.top

[S10] C：指针与解引用
来源：http://mcq.sysykeji.top

int *p = &a;  *p = 5;
来源：http://mov.gzhubu.top

[S11] C：逐行读文件
来源：http://kqu.tianlin.xyz

FILE *f = fopen("a.txt", "r");
来源：http://bhd.gotoacloud.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://dkd.jianghu66.top

fclose(f);
来源：http://uzt.cqqwz.cn

[S12] C：写文件
来源：http://byk.yj20258.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nzd.uphjek.com

[S13] C：宏定义
来源：http://zpa.xuetiantiany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nqe.zhongyouzk.top

[S14] C：枚举
来源：http://kic.aizwys.cn

enum Color { RED, GREEN, BLUE };
来源：http://qhz.yueranfly.top

[S15] C：类型转换
来源：http://dtg.zhaomingkeji.xyz

(double) a / b
来源：http://ofd.chenzaomai.com

[S16] C：位操作置位
来源：http://scp.52xcode.cn

x |= (1 << 3);
来源：http://ptj.ydjk.org.cn

[S17] C：安全拼接字符串
来源：http://jvi.zycfv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qgu.hongshengwenyu.top

[S18] C：命令行参数
来源：http://mfz.zhoulong.xyz

int main(int argc, char **argv)
来源：http://kgb.cdnleiting.top

[S19] C：快速排序
来源：http://yjm.shuidangran.top

qsort(a, n, sizeof(int), cmp);
来源：http://dfb.daxiang520.top

[S20] C：二分查找
来源：http://gke.gotoacloud.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fqt.pycfn.com

[S21] C：字符类别判断
来源：http://gip.daxiang520.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qwy.tarul.cn

[S22] C：字符串转数字
来源：http://qia.shuidangran.top

atoi("42");  strtod("3.14", NULL);
来源：http://iye.vqdsnc.cn

[S23] C：随机数
来源：http://qzx.ivvv.top

srand(time(NULL));  int r = rand() % 100;
来源：http://yia.nanxinkj.top

[S24] C：获取本地时间
来源：http://prs.shanyushiyangtech.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://crj.shuidangran.top

[S25] C：内存拷贝
来源：http://vym.haohaochexian.top

memcpy(dst, src, n);
来源：http://pwj.chenzaomai.com

[S26] C：内存清零
来源：http://avm.jlsjyb.cn

memset(a, 0, sizeof a);
来源：http://fnk.yfazqb.com

[S27] C：定义常量
来源：http://sij.yanxiufei.cn

const double PI = 3.14159;
来源：http://yrd.epnwcf.com

[S28] C：静态变量
来源：http://lbo.redwolf501.top

static int counter = 0;
来源：http://itu.yanxiufei.cn

[S29] C：变参函数
来源：http://nim.zycfv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pmg.jqgufenzy.top

[S30] C：头文件保护
来源：http://pux.tianlin.xyz

#ifndef X_H
来源：http://wju.ydjk.org.cn

#define X_H
来源：http://lcs.gzhubu.top

#endif
来源：http://whw.yuanzhike.top

[S31] C++：Hello World
来源：http://pqk.bjfxy.top

#include <iostream>
来源：http://umh.zhaomingkeji.xyz

int main() { std::cout << "Hello\n"; }
来源：http://mug.jianghu66.top

[S32] C++：字符串
来源：http://hhu.fzhhl.top

std::string s = "hi";  s += "!";
来源：http://umu.bbcook.cn

[S33] C++：vector 增删
来源：http://ntp.ybcxt.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://exb.pengpengdd.cyou

[S34] C++：遍历 vector
来源：http://tsc.cashguo.top

for (auto &x : v) { std::cout << x; }
来源：http://cef.jinqigufen.top

[S35] C++：map
来源：http://ate.daxiang520.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://edw.yangfankeji.com

[S36] C++：unordered_map
来源：http://mue.shanyushiyangtech.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://peo.hongshengwenyu.top

[S37] C++：set
来源：http://isw.tanke756.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lqe.zhijiandao.cn

[S38] C++：排序
来源：http://pwn.yueranfly.top

std::sort(v.begin(), v.end());
来源：http://run.aizwys.cn

[S39] C++：自定义比较器排序
来源：http://bnq.vqdsnc.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ekx.fehbvm.com

[S40] C++：查找元素
来源：http://mkb.jlsjyb.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yic.shzxlz.cn

[S41] C++：类与构造函数
来源：http://cyb.zhongyouzk.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gsr.quarkkingdee.top

[S42] C++：继承与虚函数
来源：http://hzl.wangshuangyany.cn

class B : public Base { public: void f() override {} };
来源：http://bpp.zdbjq.cn

[S43] C++：智能指针
来源：http://cku.vqdsnc.cn

auto p = std::make_unique<int>(5);
来源：http://vqn.chenjidiqi.icu

[S44] C++：引用传参
来源：http://hcn.redwolf501.top

void inc(int &x) { ++x; }
来源：http://mgl.yueranfly.top

[S45] C++：lambda
来源：http://frx.316326.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://xmv.tianlin.xyz

[S46] C++：函数模板
来源：http://ztp.fktsv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nbg.yanxiufei.cn

[S47] C++：结构化绑定遍历
来源：http://rnd.guowangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wgp.yonumen.top

[S48] C++：逐行读文件
来源：http://lhk.hongshengwenyu.top

std::ifstream in("a.txt");  std::string line;
来源：http://ayv.shangyingyoupin.top

while (std::getline(in, line)) { }
来源：http://bnb.gogol.net.cn

[S49] C++：写文件
来源：http://cnu.chenlongwang.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ues.hysaishi.cn

[S50] C++：格式化数字
来源：http://pem.jqgufenzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jfm.dianchejie.cn

[S51] C++：显式类型转换
来源：http://hhz.dashuyun.cn

static_cast<double>(a) / b
来源：http://ixa.0kj1m.cn

[S52] C++：const 与 noexcept
来源：http://ecx.hywenlv.cn

int size() const noexcept { return n_; }
来源：http://spz.shzxlz.cn

[S53] C++：移动语义
来源：http://dti.haohaochexian.top

std::vector<int> w = std::move(v);
来源：http://yai.9152youxi.cn

[S54] C++：异常处理
来源：http://ajx.ehwqpu.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dco.zhengqikj.top

[S55] C++：结构化绑定
来源：http://bmo.xuanzx.com

auto [a, b] = std::make_pair(1, 2);
来源：http://yvv.shanyushiyangkeji.top

[S56] C++：optional
来源：http://fsu.fengsongda.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vjw.9152youxi.cn

[S57] C++：编译期常量
来源：http://xyt.dashuyun.cn

constexpr int N = 10;
来源：http://cni.pycfn.com

[S58] C++：命名空间
来源：http://nuw.snrcjt.cn

namespace ns { int f() { return 1; } }
来源：http://gla.yueranfly.top

[S59] C++：静态断言
来源：http://swz.xinyue.icu

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yal.yueranfly.top

[S60] C++：遍历并删除元素
来源：http://hhn.ywan-chungtsiang.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uju.jqgufenzy.top

================================================================================
来源：http://uym.hongshengwenyu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gov.zycfv.cn

================================================================================
来源：http://sac.ctjpmb.com

[T01] Kotlin：Hello World
来源：http://dir.yonumen.top

println("Hello")
来源：http://jhh.xziqi.cn

[T02] Kotlin：变量
来源：http://dhr.zhengqikj.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lme.guannengcc.top

[T03] Kotlin：字符串模板
来源：http://cef.redwolf501.top

"值: $b"
来源：http://kao.yj202588.top

[T04] Kotlin：空安全
来源：http://sfm.zhaomingkeji.xyz

val n: String? = null;  n?.length
来源：http://kqz.vqdsnc.cn

[T05] Kotlin：when 表达式
来源：http://kgu.cqqwz.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://txt.gaohongyu789.top

[T06] Kotlin：集合映射
来源：http://mod.gzhubu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bqg.ehwqpu.com

[T07] Kotlin：集合过滤
来源：http://roc.fanxiaobao.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://pcj.wangshuangyany.cn

[T08] Kotlin：数据类
来源：http://gtr.quarkkingdee.top

data class User(val name: String, val age: Int)
来源：http://qpq.svipenyu.cn

[T09] Kotlin：扩展函数
来源：http://dwy.tarul.cn

fun String.exclaim() = this + "!"
来源：http://akk.ppjwa.cn

[T10] Kotlin：默认参数
来源：http://ddq.hnxiangtu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wdr.ywan-chungtsiang.top

[T11] Kotlin：协程
来源：http://eoq.yj20258888.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://abn.xziqi.cn

[T12] Kotlin：解构声明
来源：http://sby.bjfxy.top

val (a, b) = Pair(1, 2)
来源：http://gcc.zhaomingkeji.xyz

[T13] Kotlin：只读 Map
来源：http://iuy.bbcook.cn

val m = mapOf("a" to 1)
来源：http://vbc.fengsongda.top

[T14] Kotlin：循环
来源：http://jeg.gotoacloud.top

for (i in 1..10) println(i)
来源：http://wsc.mhx1999.top

[T15] Kotlin：接口
来源：http://jbr.yj202588.top

interface Shape { fun area(): Double }
来源：http://ojc.yvedp.cn

[T16] Swift：Hello World
来源：http://sbv.pycfn.com

print("Hello")
来源：http://qpk.hnxiangtu.top

[T17] Swift：变量与常量
来源：http://ead.chenjidiqi.icu

var a = 1;  let b = 2
来源：http://nnm.hfpthk.cn

[T18] Swift：字符串插值
来源：http://xqs.jinqigufen.top

"值: \(b)"
来源：http://fco.mhx1999.top

[T19] Swift：可选绑定
来源：http://xon.zhixingplan.top

if let n = opt { print(n) }
来源：http://gsr.guowangkeji.top

[T20] Swift：数组操作
来源：http://wzi.nwbrower.top

var a = [1, 2, 3];  a.append(4)
来源：http://hmi.shanyushiyangkeji.top

[T21] Swift：遍历
来源：http://hxr.tianlin.xyz

for x in a { print(x) }
来源：http://zxc.yongpay.top

[T22] Swift：字典
来源：http://kgz.fehbvm.com

var d = ["a": 1];  d["b"] = 2
来源：http://lfw.zdqjudy.top

[T23] Swift：函数
来源：http://cld.epnwcf.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bls.chenjidiqi.icu

[T24] Swift：闭包
来源：http://gcn.hfpthk.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://btf.zhijiandao.cn

[T25] Swift：结构体
来源：http://vtb.tarul.cn

struct P { var x: Int }
来源：http://his.ydjk.org.cn

[T26] Swift：类与重写
来源：http://mjs.sufxvd.cn

class A: Base { override func f() {} }
来源：http://otk.yuanzhike.top

[T27] Swift：错误处理
来源：http://slx.ybcxt.top

do { try f() } catch { print(error) }
来源：http://ywy.cheryme.top

[T28] Swift：枚举
来源：http://bkp.meibo888.top

enum Color { case red, green }
来源：http://iln.kuanghao11.cn

[T29] Swift：guard 提前返回
来源：http://say.aizwys.cn

guard let x = opt else { return }
来源：http://bph.xuetiantiany.cn

[T30] Swift：协议
来源：http://cqg.jinghuilouyu.cn

protocol Shape { func area() -> Double }
来源：http://kmy.fengsongda.top

[T31] Lua：Hello World
来源：http://lbv.ppjwa.cn

print("Hello")
来源：http://fqk.fengsongda.top

[T32] Lua：局部变量
来源：http://oew.guowangkeji.top

local a = 1
来源：http://uoa.haohaochexian.top

[T33] Lua：表（数组）
来源：http://orr.xuetiantiany.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://maz.tanke756.top

[T34] Lua：遍历表
来源：http://uon.havefunace.top

for i, v in ipairs(t) do print(i, v) end
来源：http://woe.kuanghao11.cn

[T35] Lua：字典表
来源：http://bga.hnqzz.top

local d = { a = 1 };  d.b = 2
来源：http://vzp.bbcook.cn

[T36] Lua：函数
来源：http://kgd.tianlin.xyz

function add(a, b) return a + b end
来源：http://opk.yj202588.top

[T37] Lua：字符串拼接
来源：http://gpc.pengpengdd.cyou

"a" .. "b"
来源：http://jkj.iojbl.cn

[T38] Lua：条件
来源：http://cwc.jinghuilouyu.cn

if x > 0 then print("正") end
来源：http://zhf.zhaomingkeji.xyz

[T39] Lua：模式匹配
来源：http://xwf.chenjidiqi.icu

string.find(s, "%d+")
来源：http://eiw.xinyue.icu

[T40] Lua：元表
来源：http://ppq.xuanzx.com

setmetatable({}, { __index = base })
来源：http://vyy.yj20258.top

[T41] Perl：Hello World
来源：http://gay.shanyushiyangkeji.top

print "Hello\n";
来源：http://icv.cashguo.top

[T42] Perl：变量类型
来源：http://lip.ydjk.org.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zkm.ydzc1.top


<!-- 参考信息 -->