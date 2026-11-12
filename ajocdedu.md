代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://uxe.daxiang520.top

[R48] awk 取指定列
来源：http://olv.yongpay.top

awk '{print $1, $3}' a.txt
来源：http://pzy.birdmap.top

[R49] awk 带条件
来源：http://wsg.yvedp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lmx.sjlbkw.cn

[R50] awk 求和
来源：http://yul.pycfn.com

awk '{s += $2} END {print s}' a.txt
来源：http://vtn.aibaodan.cn

[R51] 排序去重取前几
来源：http://etc.jinqigufen.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ife.zdbjq.cn

[R52] 统计行数
来源：http://qcv.nanxuanxn.top

wc -l a.txt
来源：http://zvj.316326.xyz

[R53] 查看文件头与实时尾
来源：http://taf.zhongyouzk.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mzl.iojbl.cn

[R54] 比较两个文件
来源：http://vvl.hammf.cn

diff a.txt b.txt
来源：http://kxq.cdnleiting.top

[R55] 压缩与解压
来源：http://ero.chenzaomai.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tmy.guowangkeji.top

[R56] 远程拷贝
来源：http://rlh.hfpthk.cn

scp file user@host:/path/
来源：http://ife.birdmap.top

[R57] 远程执行命令
来源：http://sra.hcnkem.com

ssh user@host 'uptime'
来源：http://jaj.shzxlz.cn

[R58] 下载文件
来源：http://rqv.zhengqikj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ldw.pengpengdd.cyou

[R59] 发 POST JSON
来源：http://khl.jinyuanbaomall.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://goq.pycfn.com

[R60] 只看 HTTP 状态码
来源：http://ith.gogol.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jkh.sjlbkw.cn

[R61] 磁盘占用
来源：http://gxz.guannengcc.top

df -h;  du -sh *
来源：http://rwu.zhaomingkeji.xyz

[R62] 找最占空间的文件
来源：http://akb.shanyushiyangkeji.top

du -ah . | sort -rh | head -10
来源：http://vwj.jqgfzy.top

[R63] 内存与进程
来源：http://fnx.zycfv.cn

free -h;  ps aux | grep nginx
来源：http://liy.chenlongwang.top

[R64] 结束进程
来源：http://auz.iojbl.cn

kill -9 $(pgrep -f app.py)
来源：http://sye.birdmap.top

[R65] 查看端口占用
来源：http://bed.ywan-chungtsiang.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ara.gogol.net.cn

[R66] 定时任务
来源：http://pqj.cashguo.top

crontab -e;  crontab -l
来源：http://daj.ydzc1.top

[R67] 生成随机十六进制串
来源：http://zyn.tarul.cn

openssl rand -hex 16
来源：http://ggl.yongpay.top

[R68] 计算文件校验值
来源：http://cqd.gotoacloud.top

sha256sum a.txt;  md5sum a.txt
来源：http://tnz.jyoumei.cn

[R69] 生成随机密码
来源：http://adz.feifeiyinyue.top

head -c 16 /dev/urandom | base64
来源：http://vng.316326.xyz

[R70] 时间戳与互转
来源：http://eej.bjfxy.top

date +%s;  date -d @1700000000
来源：http://hrn.cucudq.cn

[R71] 日期格式化
来源：http://dov.ydjk.org.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://glr.52xcode.cn

[R72] 等待端口就绪
来源：http://bvo.sjlbkw.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fer.daria6918.cn

[R73] 分割大日志
来源：http://hoi.daria6918.cn

split -l 1000 big.log part_
来源：http://snm.yonumen.top

[R74] 批量重命名
来源：http://yqf.dianchejie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yxp.snrcjt.cn

[R75] 导出环境变量
来源：http://kob.c1oappe.top

export PATH="$HOME/bin:$PATH"
来源：http://zdt.jlsjyb.cn

[R76] 使用临时文件
来源：http://tyc.bbcook.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cku.ctjpmb.com

[R77] 读取用户输入
来源：http://czp.bbcook.cn

read -rp "请输入: " ans
来源：http://sub.yfazqb.com

[R78] 交互式菜单
来源：http://ugm.jqgfzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://lmt.pengpengdd.cyou

[R79] 解析命令行选项
来源：http://vyw.dianchejie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://csd.daria6918.cn

[R80] 查看脚本执行耗时
来源：http://cxu.aizwys.cn

time ./run.sh
来源：http://fzi.yvedp.cn

================================================================================
来源：http://vin.chenlongwang.top

S. C / C++ 专题
来源：http://tnc.nanxinkj.top

================================================================================
来源：http://tiy.9152youxi.cn

[S01] C：Hello World
来源：http://idb.redwolf501.top

#include <stdio.h>
来源：http://kil.ydjk.org.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rwi.xingfuxueyuan.xyz

[S02] C：变量与格式化输出
来源：http://ber.hnxiangtu.top

int a = 10; printf("%d\n", a);
来源：http://szx.daria6918.cn

[S03] C：读入整数
来源：http://upf.tianlin.xyz

int x; scanf("%d", &x);
来源：http://hdn.hysaishi.cn

[S04] C：字符串复制
来源：http://ktb.zhongyouzk.top

char dst[32]; strcpy(dst, "hi");
来源：http://dej.0kj1m.cn

[S05] C：字符串长度
来源：http://fhj.andypj.xyz

strlen(s)
来源：http://gny.cqqwz.cn

[S06] C：字符串比较
来源：http://rwm.guowangkeji.top

strcmp(a, b) == 0
来源：http://dfq.hywenlv.cn

[S07] C：数组遍历求和
来源：http://bde.yj20258888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ccx.xingfuxueyuan.xyz

[S08] C：动态内存分配与释放
来源：http://vmy.jinqigufen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pqb.gotoacloud.top

[S09] C：结构体定义与初始化
来源：http://bha.gaohongyu789.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vnn.wangshuangyany.cn

[S10] C：指针与解引用
来源：http://jjm.ywan-chungtsiang.top

int *p = &a;  *p = 5;
来源：http://zgy.ydjk.org.cn

[S11] C：逐行读文件
来源：http://een.chenjidiqi.icu

FILE *f = fopen("a.txt", "r");
来源：http://lro.jinqigfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://olb.haohaochexian.top

fclose(f);
来源：http://ybk.shanyushiyangtech.top

[S12] C：写文件
来源：http://yzt.yuxming.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ytx.andypj.xyz

[S13] C：宏定义
来源：http://scs.chenjidiqi.icu

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fyn.tarul.cn

[S14] C：枚举
来源：http://pxg.xuanzx.com

enum Color { RED, GREEN, BLUE };
来源：http://eom.fengsongda.top

[S15] C：类型转换
来源：http://ijd.fanxiaobao.xyz

(double) a / b
来源：http://vzn.fehbvm.com

[S16] C：位操作置位
来源：http://tlm.sjlbkw.cn

x |= (1 << 3);
来源：http://wod.bjfxy.top

[S17] C：安全拼接字符串
来源：http://fsf.ydzc1.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fbu.birdmap.top

[S18] C：命令行参数
来源：http://bdi.hesvh.cn

int main(int argc, char **argv)
来源：http://qlj.yj202588.top

[S19] C：快速排序
来源：http://yyi.vehdjk.com

qsort(a, n, sizeof(int), cmp);
来源：http://mgd.yuxming.cn

[S20] C：二分查找
来源：http://psm.xinyue.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rfr.quarkkingdee.top

[S21] C：字符类别判断
来源：http://tli.shuidangran.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ynt.redwolf501.top

[S22] C：字符串转数字
来源：http://old.ehwqpu.com

atoi("42");  strtod("3.14", NULL);
来源：http://ebk.shanyushiyangkeji.top

[S23] C：随机数
来源：http://vtz.haohaochexian.top

srand(time(NULL));  int r = rand() % 100;
来源：http://gce.shangyingyoupin.top

[S24] C：获取本地时间
来源：http://ifu.guowangkeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://czf.pycfn.com

[S25] C：内存拷贝
来源：http://pie.jinghuilouyu.cn

memcpy(dst, src, n);
来源：http://tfj.smart0.xyz

[S26] C：内存清零
来源：http://qww.shzxlz.cn

memset(a, 0, sizeof a);
来源：http://oxr.dashuyun.cn

[S27] C：定义常量
来源：http://oxj.yuxming.cn

const double PI = 3.14159;
来源：http://xyo.nanxuanxn.top

[S28] C：静态变量
来源：http://qyh.zdbjq.cn

static int counter = 0;
来源：http://rbw.yueranfly.top

[S29] C：变参函数
来源：http://qye.tian-w.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://txh.chenlongwang.top

[S30] C：头文件保护
来源：http://eax.xingfuxueyuan.xyz

#ifndef X_H
来源：http://mwi.ivvv.top

#define X_H
来源：http://mxq.havefunace.top

#endif
来源：http://srj.sweek.top

[S31] C++：Hello World
来源：http://xfr.shanyushiyangtech.top

#include <iostream>
来源：http://jvn.ybcxt.top

int main() { std::cout << "Hello\n"; }
来源：http://bfb.chenlongwang.top

[S32] C++：字符串
来源：http://yzl.nanxinkj.top

std::string s = "hi";  s += "!";
来源：http://dfj.c1oappe.top

[S33] C++：vector 增删
来源：http://hvc.fktsv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bfv.yangfankeji.com

[S34] C++：遍历 vector
来源：http://krw.hnxiangtu.top

for (auto &x : v) { std::cout << x; }
来源：http://gxz.ydjk.org.cn

[S35] C++：map
来源：http://mwv.zdqjudy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gbt.andypj.xyz

[S36] C++：unordered_map
来源：http://jzv.smart0.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qjj.shzxlz.cn

[S37] C++：set
来源：http://ntq.yfazqb.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gkg.snrcjt.cn

[S38] C++：排序
来源：http://uzt.xziqi.cn

std::sort(v.begin(), v.end());
来源：http://ssc.ctjpmb.com

[S39] C++：自定义比较器排序
来源：http://uhc.sweek.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kre.gotoacloud.top

[S40] C++：查找元素
来源：http://aif.yongpay.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pvt.zhengqikj.top

[S41] C++：类与构造函数
来源：http://bne.zhijiandao.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://woi.pengpengdd.cyou

[S42] C++：继承与虚函数
来源：http://ahh.tarul.cn

class B : public Base { public: void f() override {} };
来源：http://eih.tianlin.xyz

[S43] C++：智能指针
来源：http://agy.uphjek.com

auto p = std::make_unique<int>(5);
来源：http://axc.yj20258.top

[S44] C++：引用传参
来源：http://skb.wangshuangyany.cn

void inc(int &x) { ++x; }
来源：http://wfd.hammf.cn

[S45] C++：lambda
来源：http://ltf.snrcjt.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kve.andypj.xyz

[S46] C++：函数模板
来源：http://zor.hfpthk.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://van.gzhubu.top

[S47] C++：结构化绑定遍历
来源：http://wfp.yueranfly.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://agh.hfpthk.cn

[S48] C++：逐行读文件
来源：http://fvt.jinyuanbaomall.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ejx.sxryk.cn

while (std::getline(in, line)) { }
来源：http://zga.tarul.cn

[S49] C++：写文件
来源：http://war.yanxiufei.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vwe.pengpengdd.cyou

[S50] C++：格式化数字
来源：http://qnl.gogol.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ksm.0kj1m.cn

[S51] C++：显式类型转换
来源：http://thv.hywenlv.cn

static_cast<double>(a) / b
来源：http://jno.pycfn.com

[S52] C++：const 与 noexcept
来源：http://cch.yj20258.top

int size() const noexcept { return n_; }
来源：http://rdf.quarkkingdee.top

[S53] C++：移动语义
来源：http://gkw.meibo888.top

std::vector<int> w = std::move(v);
来源：http://poo.sysykeji.top

[S54] C++：异常处理
来源：http://lsq.sweek.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hyf.mhx1999.top

[S55] C++：结构化绑定
来源：http://qsl.jinghuilouyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gpb.cqqwz.cn

[S56] C++：optional
来源：http://teq.shanyushiyangkeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yik.wangshuangyany.cn

[S57] C++：编译期常量
来源：http://oko.sweek.top

constexpr int N = 10;
来源：http://icu.yfazqb.com

[S58] C++：命名空间
来源：http://okf.ehwqpu.com

namespace ns { int f() { return 1; } }
来源：http://rnr.0kj1m.cn

[S59] C++：静态断言
来源：http://rba.jqgufenzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rvs.sufxvd.cn

[S60] C++：遍历并删除元素
来源：http://ysm.sjlbkw.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eni.nanxuanxn.top

================================================================================
来源：http://ywo.hongshengwenyu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dcy.zhongyouzk.top

================================================================================
来源：http://igm.bbcook.cn

[T01] Kotlin：Hello World
来源：http://cno.cashguo.top

println("Hello")
来源：http://lda.gotoacloud.top

[T02] Kotlin：变量
来源：http://vwq.c1oappe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ovx.zdqjudy.top

[T03] Kotlin：字符串模板
来源：http://pvs.hongshengwenyu.top

"值: $b"
来源：http://aiv.ydjk.org.cn

[T04] Kotlin：空安全
来源：http://uey.svipenyu.cn

val n: String? = null;  n?.length
来源：http://jca.jyoumei.cn

[T05] Kotlin：when 表达式
来源：http://bim.zhaomingkeji.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vhy.vqdsnc.cn

[T06] Kotlin：集合映射
来源：http://ppn.cqqwz.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fxm.shangyingyoupin.top

[T07] Kotlin：集合过滤
来源：http://fnm.sxryk.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bvd.vehdjk.com

[T08] Kotlin：数据类
来源：http://maj.yj20258888.top

data class User(val name: String, val age: Int)
来源：http://bjw.nwbrower.top

[T09] Kotlin：扩展函数
来源：http://sdr.ywan-chungtsiang.top

fun String.exclaim() = this + "!"
来源：http://tya.havefunace.top

[T10] Kotlin：默认参数
来源：http://auu.aizwys.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://job.kuanghao11.cn

[T11] Kotlin：协程
来源：http://cqu.zdqjudy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://oot.aizwys.cn

[T12] Kotlin：解构声明
来源：http://btt.sufxvd.cn

val (a, b) = Pair(1, 2)
来源：http://hur.sysykeji.top

[T13] Kotlin：只读 Map
来源：http://yba.ehwqpu.com

val m = mapOf("a" to 1)
来源：http://eeo.c1oappe.top

[T14] Kotlin：循环
来源：http://ssh.xylfe.cn

for (i in 1..10) println(i)
来源：http://rxw.hesvh.cn

[T15] Kotlin：接口
来源：http://tou.meibo888.top

interface Shape { fun area(): Double }
来源：http://yoh.sufxvd.cn

[T16] Swift：Hello World
来源：http://fzx.hammf.cn

print("Hello")
来源：http://gjf.yonumen.top

[T17] Swift：变量与常量
来源：http://dww.ppjwa.cn

var a = 1;  let b = 2
来源：http://tqf.chenlongwang.top

[T18] Swift：字符串插值
来源：http://pxb.snrcjt.cn

"值: \(b)"
来源：http://adj.bbcook.cn

[T19] Swift：可选绑定
来源：http://zpu.aibaodan.cn

if let n = opt { print(n) }
来源：http://bcr.yueranfly.top

[T20] Swift：数组操作
来源：http://npu.fengsongda.top

var a = [1, 2, 3];  a.append(4)
来源：http://mtu.jinqigufen.top

[T21] Swift：遍历
来源：http://efk.iojbl.cn

for x in a { print(x) }
来源：http://qtq.jlsjyb.cn

[T22] Swift：字典
来源：http://ojk.vehdjk.com

var d = ["a": 1];  d["b"] = 2
来源：http://bje.chenzaomai.com

[T23] Swift：函数
来源：http://ism.ydzc1.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://thf.sysykeji.top

[T24] Swift：闭包
来源：http://eqb.gzhubu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://knu.feifeiyinyue.top

[T25] Swift：结构体
来源：http://rym.snrcjt.cn

struct P { var x: Int }
来源：http://uix.yfazqb.com

[T26] Swift：类与重写
来源：http://llw.dashuyun.cn

class A: Base { override func f() {} }
来源：http://gck.yfazqb.com

[T27] Swift：错误处理
来源：http://dud.havefunace.top

do { try f() } catch { print(error) }
来源：http://ast.redwolf501.top

[T28] Swift：枚举
来源：http://qto.nanxinkj.top

enum Color { case red, green }
来源：http://noc.0kj1m.cn

[T29] Swift：guard 提前返回
来源：http://gau.jyoumei.cn

guard let x = opt else { return }
来源：http://yrl.epnwcf.com

[T30] Swift：协议
来源：http://wat.cheryme.top

protocol Shape { func area() -> Double }
来源：http://mxt.svipenyu.cn

[T31] Lua：Hello World
来源：http://phf.epnwcf.com

print("Hello")
来源：http://yjk.hammf.cn

[T32] Lua：局部变量
来源：http://ems.xinyue.icu

local a = 1
来源：http://ies.ehwqpu.com

[T33] Lua：表（数组）
来源：http://psv.fehbvm.com

local t = {1, 2, 3};  t[4] = 4
来源：http://pzi.zhoulong.xyz

[T34] Lua：遍历表
来源：http://kdp.zhijiandao.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ujm.pengpengdd.cyou

[T35] Lua：字典表
来源：http://ppx.yvedp.cn

local d = { a = 1 };  d.b = 2
来源：http://bes.sxryk.cn

[T36] Lua：函数
来源：http://cja.daria6918.cn

function add(a, b) return a + b end
来源：http://opc.xingfuxueyuan.xyz

[T37] Lua：字符串拼接
来源：http://egn.cashguo.top

"a" .. "b"
来源：http://chw.yj20258888.top

[T38] Lua：条件
来源：http://uzr.zhongyouzk.top

if x > 0 then print("正") end
来源：http://oje.jyoumei.cn

[T39] Lua：模式匹配
来源：http://adr.cqqwz.cn

string.find(s, "%d+")
来源：http://umj.yfazqb.com

[T40] Lua：元表
来源：http://muo.pengpengdd.cyou

setmetatable({}, { __index = base })
来源：http://uhm.dashuyun.cn

[T41] Perl：Hello World
来源：http://uqh.tianlin.xyz

print "Hello\n";
来源：http://fof.daria6918.cn

[T42] Perl：变量类型
来源：http://sxa.mhx1999.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xzm.zdbjq.cn

[T43] Perl：字符串插值
来源：http://gxw.gogol.net.cn

"值: $a"
来源：http://bvw.fzhhl.top

[T44] Perl：条件
来源：http://oeq.gotoacloud.top

if ($a > 0) { print "正"; }
来源：http://laj.jinqigufen.top

[T45] Perl：数组遍历
来源：http://lor.yuxming.cn

for my $x (@arr) { print $x; }
来源：http://wzc.ivvv.top

[T46] Perl：哈希操作
来源：http://wfm.9152youxi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jki.c1oappe.top

[T47] Perl：正则捕获
来源：http://erw.nanxinkj.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ugg.jlsjyb.cn

[T48] Perl：正则替换
来源：http://cig.fzhhl.top

$s =~ s/old/new/g;
来源：http://aeu.jinqigufen.top

[T49] Perl：函数
来源：http://sly.zdqjudy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sji.epnwcf.com

[T50] Perl：逐行读文件
来源：http://yhj.feifeiyinyue.top

open my $fh, "<", "a.txt" or die $!;
来源：http://wwp.sxryk.cn


<!-- 参考信息 -->