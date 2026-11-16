代发 wailian999

files=$(ls -1)
来源：http://ysk.cdnleiting.top

[R38] 管道串联
来源：http://nlr.yj20258888.top

cat a.txt | grep -i error | wc -l
来源：http://cta.yuxming.cn

[R39] 重定向标准输出与错误
来源：http://hlh.mhx1999.top

cmd > out.log 2>&1
来源：http://fts.kuanghao11.cn

[R40] 追加写日志
来源：http://eoa.yj20258.top

echo "log" >> out.log
来源：http://tnu.9152youxi.cn

[R41] 丢弃输出
来源：http://bgm.sjlbkw.cn

cmd >/dev/null 2>&1
来源：http://gmp.ctjpmb.com

[R42] 输入重定向
来源：http://eqb.fktsv.cn

wc -l < a.txt
来源：http://oyt.tanke756.top

[R43] 按名字查找文件
来源：http://ihm.vqdsnc.cn

find . -name "*.log" -type f
来源：http://qkk.yueranfly.top

[R44] 按修改时间查找
来源：http://hcz.sxryk.cn

find . -mtime -7 -type f
来源：http://wtn.zhiwuduotai.top

[R45] 批量删除
来源：http://faa.haohaochexian.top

find . -name "*.tmp" -delete
来源：http://vfl.nanxinkj.top

[R46] 递归替换文件内容
来源：http://nzw.cheryme.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://swr.jlsjyb.cn

[R47] sed 单行替换
来源：http://zvn.yj20258.top

sed -i 's/foo/bar/g' a.txt
来源：http://ynf.zdbjq.cn

[R48] awk 取指定列
来源：http://cfc.shuidangran.top

awk '{print $1, $3}' a.txt
来源：http://smz.feifeiyinyue.top

[R49] awk 带条件
来源：http://qea.shzxlz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://avx.tianlin.xyz

[R50] awk 求和
来源：http://nlr.ppjwa.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ouz.daxiang520.top

[R51] 排序去重取前几
来源：http://wsz.chenzaomai.com

sort a.txt | uniq -c | sort -rn | head
来源：http://dfg.cheryme.top

[R52] 统计行数
来源：http://zum.gaohongyu789.top

wc -l a.txt
来源：http://lcd.52xcode.cn

[R53] 查看文件头与实时尾
来源：http://kge.iojbl.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pes.yangfankeji.com

[R54] 比较两个文件
来源：http://ykh.yuanzhike.top

diff a.txt b.txt
来源：http://gtx.xylfe.cn

[R55] 压缩与解压
来源：http://flr.xingfuxueyuan.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ief.cdnleiting.top

[R56] 远程拷贝
来源：http://izs.ehwqpu.com

scp file user@host:/path/
来源：http://vzi.yfazqb.com

[R57] 远程执行命令
来源：http://qli.yvedp.cn

ssh user@host 'uptime'
来源：http://lms.yj20258.top

[R58] 下载文件
来源：http://yrb.dashuyun.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wwv.fengsongda.top

[R59] 发 POST JSON
来源：http://yhg.cheryme.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://soj.hongshengwenyu.top

[R60] 只看 HTTP 状态码
来源：http://tkr.yangfankeji.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zub.jqgufenzy.top

[R61] 磁盘占用
来源：http://vgf.zhengqikj.top

df -h;  du -sh *
来源：http://vds.sufxvd.cn

[R62] 找最占空间的文件
来源：http://rnf.aizwys.cn

du -ah . | sort -rh | head -10
来源：http://vjm.daxiang520.top

[R63] 内存与进程
来源：http://hjy.yonumen.top

free -h;  ps aux | grep nginx
来源：http://zho.ybcxt.top

[R64] 结束进程
来源：http://bcl.cdnleiting.top

kill -9 $(pgrep -f app.py)
来源：http://tbb.hongshengwenyu.top

[R65] 查看端口占用
来源：http://qcy.9152youxi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bhc.epnwcf.com

[R66] 定时任务
来源：http://cbs.yanxiufei.cn

crontab -e;  crontab -l
来源：http://tlj.hongshengwenyu.top

[R67] 生成随机十六进制串
来源：http://xvk.hnqzz.top

openssl rand -hex 16
来源：http://nbo.tianlin.xyz

[R68] 计算文件校验值
来源：http://cbm.dashuyun.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wmd.jlsjyb.cn

[R69] 生成随机密码
来源：http://ohp.jinyuanbaomall.cn

head -c 16 /dev/urandom | base64
来源：http://etr.daxiang520.top

[R70] 时间戳与互转
来源：http://fmv.yongpay.top

date +%s;  date -d @1700000000
来源：http://rzo.shangyingyoupin.top

[R71] 日期格式化
来源：http://nwq.dianchejie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kja.yangfankeji.com

[R72] 等待端口就绪
来源：http://vbx.shanyushiyangtech.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qnt.jinqigfzy.top

[R73] 分割大日志
来源：http://opl.shuidangran.top

split -l 1000 big.log part_
来源：http://fxx.feifeiyinyue.top

[R74] 批量重命名
来源：http://wfu.zhoulong.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pro.dashuyun.cn

[R75] 导出环境变量
来源：http://omy.yj20258.top

export PATH="$HOME/bin:$PATH"
来源：http://dwj.zhiwuduotai.top

[R76] 使用临时文件
来源：http://sli.kuanghao11.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ocf.haohaochexian.top

[R77] 读取用户输入
来源：http://jfj.cheryme.top

read -rp "请输入: " ans
来源：http://jnm.snrcjt.cn

[R78] 交互式菜单
来源：http://udk.daria6918.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zxl.ydzc1.top

[R79] 解析命令行选项
来源：http://jzo.bbcook.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://agn.jinghuilouyu.cn

[R80] 查看脚本执行耗时
来源：http://mtn.316326.xyz

time ./run.sh
来源：http://zvd.xinyue.icu

================================================================================
来源：http://ufx.xuetiantiany.cn

S. C / C++ 专题
来源：http://ghd.hesvh.cn

================================================================================
来源：http://zjm.cqqwz.cn

[S01] C：Hello World
来源：http://xkg.zdbjq.cn

#include <stdio.h>
来源：http://xtp.tarul.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ers.yangfankeji.com

[S02] C：变量与格式化输出
来源：http://rgp.fktsv.cn

int a = 10; printf("%d\n", a);
来源：http://bmx.xuetiantiany.cn

[S03] C：读入整数
来源：http://tkm.zhiwuduotai.top

int x; scanf("%d", &x);
来源：http://ino.hfpthk.cn

[S04] C：字符串复制
来源：http://xza.ppjwa.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ycn.sjlbkw.cn

[S05] C：字符串长度
来源：http://wum.pengpengdd.cyou

strlen(s)
来源：http://mvq.316326.xyz

[S06] C：字符串比较
来源：http://bzl.tianlin.xyz

strcmp(a, b) == 0
来源：http://nsh.yonumen.top

[S07] C：数组遍历求和
来源：http://obj.jinyuanbaomall.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wrs.tian-w.cn

[S08] C：动态内存分配与释放
来源：http://ahk.cashguo.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jmi.jianghu66.top

[S09] C：结构体定义与初始化
来源：http://qbk.52xcode.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wce.ydjk.org.cn

[S10] C：指针与解引用
来源：http://ooi.hammf.cn

int *p = &a;  *p = 5;
来源：http://woq.0kj1m.cn

[S11] C：逐行读文件
来源：http://fba.fktsv.cn

FILE *f = fopen("a.txt", "r");
来源：http://ncj.tianlin.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://saj.yuxming.cn

fclose(f);
来源：http://ngd.zhaomingkeji.xyz

[S12] C：写文件
来源：http://mvx.epnwcf.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pev.pengpengdd.cyou

[S13] C：宏定义
来源：http://fsr.nwbrower.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lna.mhx1999.top

[S14] C：枚举
来源：http://sxj.xuetiantiany.cn

enum Color { RED, GREEN, BLUE };
来源：http://dyb.feifeiyinyue.top

[S15] C：类型转换
来源：http://fah.wangshuangyany.cn

(double) a / b
来源：http://lfk.gzhubu.top

[S16] C：位操作置位
来源：http://asc.svipenyu.cn

x |= (1 << 3);
来源：http://yfx.nanxinkj.top

[S17] C：安全拼接字符串
来源：http://fpk.daxiang520.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rzg.sjlbkw.cn

[S18] C：命令行参数
来源：http://yin.dianchejie.cn

int main(int argc, char **argv)
来源：http://dkf.tarul.cn

[S19] C：快速排序
来源：http://jry.gzhubu.top

qsort(a, n, sizeof(int), cmp);
来源：http://pdk.hfpthk.cn

[S20] C：二分查找
来源：http://hga.sjlbkw.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lyh.sufxvd.cn

[S21] C：字符类别判断
来源：http://kdh.shzxlz.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fuv.shzxlz.cn

[S22] C：字符串转数字
来源：http://bor.iojbl.cn

atoi("42");  strtod("3.14", NULL);
来源：http://idd.hcnkem.com

[S23] C：随机数
来源：http://csj.chenzaomai.com

srand(time(NULL));  int r = rand() % 100;
来源：http://nqc.wangshuangyany.cn

[S24] C：获取本地时间
来源：http://fer.shangyingyoupin.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cif.xinyue.icu

[S25] C：内存拷贝
来源：http://xbd.vehdjk.com

memcpy(dst, src, n);
来源：http://wyl.cheryme.top

[S26] C：内存清零
来源：http://kat.jianghu66.top

memset(a, 0, sizeof a);
来源：http://pgt.haohaochexian.top

[S27] C：定义常量
来源：http://thg.sysykeji.top

const double PI = 3.14159;
来源：http://cik.jinqigfzy.top

[S28] C：静态变量
来源：http://cma.hesvh.cn

static int counter = 0;
来源：http://vbe.snrcjt.cn

[S29] C：变参函数
来源：http://daf.yuanzhike.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wmw.ydzc1.top

[S30] C：头文件保护
来源：http://rgz.hysaishi.cn

#ifndef X_H
来源：http://duh.kuanghao11.cn

#define X_H
来源：http://lut.svipenyu.cn

#endif
来源：http://fbk.9152youxi.cn

[S31] C++：Hello World
来源：http://nvu.xinyue.icu

#include <iostream>
来源：http://rmo.nanxinkj.top

int main() { std::cout << "Hello\n"; }
来源：http://hua.ctjpmb.com

[S32] C++：字符串
来源：http://tec.jinqigufen.top

std::string s = "hi";  s += "!";
来源：http://pfx.gaohongyu789.top

[S33] C++：vector 增删
来源：http://bcm.feifeiyinyue.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kaa.zycfv.cn

[S34] C++：遍历 vector
来源：http://oco.hammf.cn

for (auto &x : v) { std::cout << x; }
来源：http://hms.hcnkem.com

[S35] C++：map
来源：http://qih.yongpay.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://clk.sjlbkw.cn

[S36] C++：unordered_map
来源：http://xcv.xylfe.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wlc.ehwqpu.com

[S37] C++：set
来源：http://cdj.yanxiufei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://etw.hesvh.cn

[S38] C++：排序
来源：http://dha.fzhhl.top

std::sort(v.begin(), v.end());
来源：http://jjq.jlsjyb.cn

[S39] C++：自定义比较器排序
来源：http://nuv.chenlongwang.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gli.52xcode.cn

[S40] C++：查找元素
来源：http://gnx.ehwqpu.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ymq.sjlbkw.cn

[S41] C++：类与构造函数
来源：http://uqr.hammf.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://umk.sweek.top

[S42] C++：继承与虚函数
来源：http://gep.nanxinkj.top

class B : public Base { public: void f() override {} };
来源：http://puk.ehwqpu.com

[S43] C++：智能指针
来源：http://bae.yj20258888.top

auto p = std::make_unique<int>(5);
来源：http://dpn.feifeiyinyue.top

[S44] C++：引用传参
来源：http://eob.hfpthk.cn

void inc(int &x) { ++x; }
来源：http://ezf.andypj.xyz

[S45] C++：lambda
来源：http://kec.yangfankeji.com

auto add = [](int a, int b) { return a + b; };
来源：http://fyu.gotoacloud.top

[S46] C++：函数模板
来源：http://syx.zhixingplan.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://suq.tanke756.top

[S47] C++：结构化绑定遍历
来源：http://ebf.gzhubu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zcb.hywenlv.cn

[S48] C++：逐行读文件
来源：http://pne.jiagoushi.top

std::ifstream in("a.txt");  std::string line;
来源：http://kxy.yvedp.cn

while (std::getline(in, line)) { }
来源：http://elo.ivvv.top

[S49] C++：写文件
来源：http://wfy.shuidangran.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zut.jqgfzy.top

[S50] C++：格式化数字
来源：http://eqs.cucudq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ujz.cucudq.cn

[S51] C++：显式类型转换
来源：http://gyn.shanyushiyangtech.top

static_cast<double>(a) / b
来源：http://zcn.vehdjk.com

[S52] C++：const 与 noexcept
来源：http://gcu.aizwys.cn

int size() const noexcept { return n_; }
来源：http://eip.yj202588.top

[S53] C++：移动语义
来源：http://crg.jyoumei.cn

std::vector<int> w = std::move(v);
来源：http://ftl.yanxiufei.cn

[S54] C++：异常处理
来源：http://zqh.zhijiandao.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rin.cucudq.cn

[S55] C++：结构化绑定
来源：http://kir.jyoumei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qmb.shuidangran.top

[S56] C++：optional
来源：http://hlw.hywenlv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qcr.xuetiantiany.cn

[S57] C++：编译期常量
来源：http://age.pycfn.com

constexpr int N = 10;
来源：http://rnm.tian-w.cn

[S58] C++：命名空间
来源：http://ubd.snrcjt.cn

namespace ns { int f() { return 1; } }
来源：http://wpg.zdbjq.cn

[S59] C++：静态断言
来源：http://jja.jinqigfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vvi.9152youxi.cn

[S60] C++：遍历并删除元素
来源：http://bwx.meibo888.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yde.guowangkeji.top

================================================================================
来源：http://gjm.meibo888.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uli.zhongyouzk.top

================================================================================
来源：http://uep.hongshengwenyu.top

[T01] Kotlin：Hello World
来源：http://ugy.hywenlv.cn

println("Hello")
来源：http://kxk.chenzaomai.com

[T02] Kotlin：变量
来源：http://pwm.hywenlv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gom.iojbl.cn

[T03] Kotlin：字符串模板
来源：http://qzm.chenzaomai.com

"值: $b"
来源：http://nan.nanxuanxn.top

[T04] Kotlin：空安全
来源：http://wxp.hysaishi.cn

val n: String? = null;  n?.length
来源：http://ygn.ywan-chungtsiang.top

[T05] Kotlin：when 表达式
来源：http://ohb.dashuyun.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hlj.c1oappe.top

[T06] Kotlin：集合映射
来源：http://hyc.sysykeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hqi.hysaishi.cn

[T07] Kotlin：集合过滤
来源：http://hhw.52xcode.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rbt.redwolf501.top

[T08] Kotlin：数据类
来源：http://wqx.gotoacloud.top

data class User(val name: String, val age: Int)
来源：http://yty.feifeiyinyue.top

[T09] Kotlin：扩展函数
来源：http://rts.zdqjudy.top

fun String.exclaim() = this + "!"
来源：http://pcp.yuxming.cn

[T10] Kotlin：默认参数
来源：http://ovv.hnxiangtu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://azb.jinghuilouyu.cn

[T11] Kotlin：协程
来源：http://pfr.tanke756.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mzy.yuanzhike.top

[T12] Kotlin：解构声明
来源：http://qrb.xinyue.icu

val (a, b) = Pair(1, 2)
来源：http://unv.ivvv.top

[T13] Kotlin：只读 Map
来源：http://fdq.zhixingplan.top

val m = mapOf("a" to 1)
来源：http://xdj.nanxuanxn.top

[T14] Kotlin：循环
来源：http://uim.hongshengwenyu.top

for (i in 1..10) println(i)
来源：http://uzm.fktsv.cn

[T15] Kotlin：接口
来源：http://crs.xinyue.icu

interface Shape { fun area(): Double }
来源：http://uha.hongshengwenyu.top

[T16] Swift：Hello World
来源：http://zrz.52xcode.cn

print("Hello")
来源：http://lap.daxiang520.top

[T17] Swift：变量与常量
来源：http://jtu.cqqwz.cn

var a = 1;  let b = 2
来源：http://gsx.zhixingplan.top

[T18] Swift：字符串插值
来源：http://ffp.chenjidiqi.icu

"值: \(b)"
来源：http://vbp.ydzc1.top

[T19] Swift：可选绑定
来源：http://emj.tarul.cn

if let n = opt { print(n) }
来源：http://pwv.iojbl.cn

[T20] Swift：数组操作
来源：http://hpi.shanyushiyangtech.top

var a = [1, 2, 3];  a.append(4)
来源：http://bgm.yvedp.cn

[T21] Swift：遍历
来源：http://pvo.mhx1999.top

for x in a { print(x) }
来源：http://gqo.shanyushiyangtech.top

[T22] Swift：字典
来源：http://fni.yuxming.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qog.zhongyouzk.top

[T23] Swift：函数
来源：http://luq.sjlbkw.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gpl.xingfuxueyuan.xyz

[T24] Swift：闭包
来源：http://egx.ivvv.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://fua.gaohongyu789.top

[T25] Swift：结构体
来源：http://jtb.sufxvd.cn

struct P { var x: Int }
来源：http://okf.zhoulong.xyz

[T26] Swift：类与重写
来源：http://boi.pengpengdd.cyou

class A: Base { override func f() {} }
来源：http://vmu.chenlongwang.top

[T27] Swift：错误处理
来源：http://cjw.fanxiaobao.xyz

do { try f() } catch { print(error) }
来源：http://zfz.chenlongwang.top

[T28] Swift：枚举
来源：http://czc.fengsongda.top

enum Color { case red, green }
来源：http://psr.yueranfly.top

[T29] Swift：guard 提前返回
来源：http://btu.chenzaomai.com

guard let x = opt else { return }
来源：http://yrs.hongshengwenyu.top

[T30] Swift：协议
来源：http://rsm.zhongyouzk.top

protocol Shape { func area() -> Double }
来源：http://ejs.0kj1m.cn

[T31] Lua：Hello World
来源：http://kgm.jqgufenzy.top

print("Hello")
来源：http://cjc.vqdsnc.cn

[T32] Lua：局部变量
来源：http://bow.havefunace.top

local a = 1
来源：http://fqo.vehdjk.com

[T33] Lua：表（数组）
来源：http://xas.yangfankeji.com

local t = {1, 2, 3};  t[4] = 4
来源：http://izv.hfpthk.cn

[T34] Lua：遍历表
来源：http://xrm.fanxiaobao.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://pzd.gaohongyu789.top

[T35] Lua：字典表
来源：http://ozd.yangfankeji.com

local d = { a = 1 };  d.b = 2
来源：http://htu.xuanzx.com

[T36] Lua：函数
来源：http://owd.havefunace.top

function add(a, b) return a + b end
来源：http://uoj.gaohongyu789.top

[T37] Lua：字符串拼接
来源：http://bby.snrcjt.cn

"a" .. "b"
来源：http://vkn.fktsv.cn

[T38] Lua：条件
来源：http://gbf.yuanzhike.top

if x > 0 then print("正") end
来源：http://meu.gzhubu.top

[T39] Lua：模式匹配
来源：http://hdc.zhixingplan.top

string.find(s, "%d+")
来源：http://ydb.fktsv.cn

[T40] Lua：元表
来源：http://qfv.kuanghao11.cn

setmetatable({}, { __index = base })
来源：http://eog.tian-w.cn


<!-- 参考信息 -->