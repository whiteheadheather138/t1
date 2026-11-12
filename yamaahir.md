代发 wailian999

cmd > out.log 2>&1
来源：http://ayk.tarul.cn

[R40] 追加写日志
来源：http://acq.wangdashe.top

echo "log" >> out.log
来源：http://ygz.uphjek.com

[R41] 丢弃输出
来源：http://tve.yj20258888.top

cmd >/dev/null 2>&1
来源：http://vur.pengpengdd.cyou

[R42] 输入重定向
来源：http://pxd.jinqigfzy.top

wc -l < a.txt
来源：http://ais.yj20258888.top

[R43] 按名字查找文件
来源：http://nib.ydzc1.top

find . -name "*.log" -type f
来源：http://tnu.fzhhl.top

[R44] 按修改时间查找
来源：http://thj.jianghu66.top

find . -mtime -7 -type f
来源：http://txp.zhoulong.xyz

[R45] 批量删除
来源：http://omw.316326.xyz

find . -name "*.tmp" -delete
来源：http://fdm.andypj.xyz

[R46] 递归替换文件内容
来源：http://ucw.c1oappe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cac.guowangkeji.top

[R47] sed 单行替换
来源：http://ylf.andypj.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://anz.zhaomingkeji.xyz

[R48] awk 取指定列
来源：http://shb.yfazqb.com

awk '{print $1, $3}' a.txt
来源：http://bxo.yangfankeji.com

[R49] awk 带条件
来源：http://xfk.yuxming.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yjj.sufxvd.cn

[R50] awk 求和
来源：http://zlm.snrcjt.cn

awk '{s += $2} END {print s}' a.txt
来源：http://iaw.gotoacloud.top

[R51] 排序去重取前几
来源：http://frc.sysykeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://xyh.pengpengdd.cyou

[R52] 统计行数
来源：http://yem.zhoulong.xyz

wc -l a.txt
来源：http://fkg.andypj.xyz

[R53] 查看文件头与实时尾
来源：http://fgu.guowangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sqi.sufxvd.cn

[R54] 比较两个文件
来源：http://nqx.yongpay.top

diff a.txt b.txt
来源：http://fmu.chenzaomai.com

[R55] 压缩与解压
来源：http://tpg.316326.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://num.andypj.xyz

[R56] 远程拷贝
来源：http://dzp.aizwys.cn

scp file user@host:/path/
来源：http://gxe.xziqi.cn

[R57] 远程执行命令
来源：http://vev.hongshengwenyu.top

ssh user@host 'uptime'
来源：http://hbf.xingfuxueyuan.xyz

[R58] 下载文件
来源：http://wrl.hfpthk.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sck.iojbl.cn

[R59] 发 POST JSON
来源：http://ngj.hfpthk.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wil.0kj1m.cn

[R60] 只看 HTTP 状态码
来源：http://bop.yvedp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://iyn.yueranfly.top

[R61] 磁盘占用
来源：http://szg.epnwcf.com

df -h;  du -sh *
来源：http://dxs.chenjidiqi.icu

[R62] 找最占空间的文件
来源：http://dub.shanyushiyangtech.top

du -ah . | sort -rh | head -10
来源：http://art.hnxiangtu.top

[R63] 内存与进程
来源：http://jrk.ydzc1.top

free -h;  ps aux | grep nginx
来源：http://jih.haohaochexian.top

[R64] 结束进程
来源：http://jta.zhijiandao.cn

kill -9 $(pgrep -f app.py)
来源：http://tdy.redwolf501.top

[R65] 查看端口占用
来源：http://qly.fengsongda.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jkq.chenzaomai.com

[R66] 定时任务
来源：http://byy.shanyushiyangtech.top

crontab -e;  crontab -l
来源：http://jia.ctjpmb.com

[R67] 生成随机十六进制串
来源：http://wdw.wangshuangyany.cn

openssl rand -hex 16
来源：http://fuz.9152youxi.cn

[R68] 计算文件校验值
来源：http://mtn.fanxiaobao.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://bro.xingfuxueyuan.xyz

[R69] 生成随机密码
来源：http://mcg.gaohongyu789.top

head -c 16 /dev/urandom | base64
来源：http://vsq.sxryk.cn

[R70] 时间戳与互转
来源：http://sfd.zhengqikj.top

date +%s;  date -d @1700000000
来源：http://sxh.tarul.cn

[R71] 日期格式化
来源：http://xib.chenlongwang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://grp.316326.xyz

[R72] 等待端口就绪
来源：http://ocm.yj20258888.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fla.tanke756.top

[R73] 分割大日志
来源：http://bkt.hysaishi.cn

split -l 1000 big.log part_
来源：http://bup.yuxming.cn

[R74] 批量重命名
来源：http://wue.quarkkingdee.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://amg.jyoumei.cn

[R75] 导出环境变量
来源：http://lwo.smart0.xyz

export PATH="$HOME/bin:$PATH"
来源：http://fwz.shuidangran.top

[R76] 使用临时文件
来源：http://hjn.jianghu66.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://row.zhiwuduotai.top

[R77] 读取用户输入
来源：http://frv.hnxiangtu.top

read -rp "请输入: " ans
来源：http://gla.nwbrower.top

[R78] 交互式菜单
来源：http://ewm.mhx1999.top

select opt in a b c; do echo "$opt"; break; done
来源：http://soy.cdnleiting.top

[R79] 解析命令行选项
来源：http://wpu.chenlongwang.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tpo.jiagoushi.top

[R80] 查看脚本执行耗时
来源：http://pca.guowangkeji.top

time ./run.sh
来源：http://byt.birdmap.top

================================================================================
来源：http://ifs.sjlbkw.cn

S. C / C++ 专题
来源：http://gih.feifeiyinyue.top

================================================================================
来源：http://uxc.fehbvm.com

[S01] C：Hello World
来源：http://rcv.chenzaomai.com

#include <stdio.h>
来源：http://emj.epnwcf.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://dkv.tian-w.cn

[S02] C：变量与格式化输出
来源：http://qlt.havefunace.top

int a = 10; printf("%d\n", a);
来源：http://mvz.yj20258.top

[S03] C：读入整数
来源：http://kkk.xylfe.cn

int x; scanf("%d", &x);
来源：http://rbm.zhiwuduotai.top

[S04] C：字符串复制
来源：http://pfv.tian-w.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bdg.sufxvd.cn

[S05] C：字符串长度
来源：http://ztm.fanxiaobao.xyz

strlen(s)
来源：http://lss.aizwys.cn

[S06] C：字符串比较
来源：http://gap.sxryk.cn

strcmp(a, b) == 0
来源：http://yyv.wangshuangyany.cn

[S07] C：数组遍历求和
来源：http://ehm.yj20258888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bsu.sxryk.cn

[S08] C：动态内存分配与释放
来源：http://hjl.daxiang520.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ycp.zhaomingkeji.xyz

[S09] C：结构体定义与初始化
来源：http://aju.yongpay.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gwv.havefunace.top

[S10] C：指针与解引用
来源：http://mpt.quarkkingdee.top

int *p = &a;  *p = 5;
来源：http://rkg.hysaishi.cn

[S11] C：逐行读文件
来源：http://wfg.hcnkem.com

FILE *f = fopen("a.txt", "r");
来源：http://cbg.wangshuangyany.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lrk.ehwqpu.com

fclose(f);
来源：http://hct.xuanzx.com

[S12] C：写文件
来源：http://zfk.yueranfly.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ksc.sxryk.cn

[S13] C：宏定义
来源：http://pnu.yuanzhike.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uxr.hcnkem.com

[S14] C：枚举
来源：http://art.chenzaomai.com

enum Color { RED, GREEN, BLUE };
来源：http://vlm.chenzaomai.com

[S15] C：类型转换
来源：http://kjk.hywenlv.cn

(double) a / b
来源：http://jpy.xuanzx.com

[S16] C：位操作置位
来源：http://jvp.zhaomingkeji.xyz

x |= (1 << 3);
来源：http://wfd.fanxiaobao.xyz

[S17] C：安全拼接字符串
来源：http://zxr.ctjpmb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zmi.yueranfly.top

[S18] C：命令行参数
来源：http://eoy.hnxiangtu.top

int main(int argc, char **argv)
来源：http://mhr.hfpthk.cn

[S19] C：快速排序
来源：http://kpn.fzhhl.top

qsort(a, n, sizeof(int), cmp);
来源：http://gwc.yuanzhike.top

[S20] C：二分查找
来源：http://cwo.shzxlz.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dwf.hnqzz.top

[S21] C：字符类别判断
来源：http://rfe.fehbvm.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qbb.zdbjq.cn

[S22] C：字符串转数字
来源：http://jit.kuanghao11.cn

atoi("42");  strtod("3.14", NULL);
来源：http://suh.zhixingplan.top

[S23] C：随机数
来源：http://aac.dianchejie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://iee.snrcjt.cn

[S24] C：获取本地时间
来源：http://lvd.gotoacloud.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hbe.fktsv.cn

[S25] C：内存拷贝
来源：http://xgy.c1oappe.top

memcpy(dst, src, n);
来源：http://ezt.guowangkeji.top

[S26] C：内存清零
来源：http://rfs.chenlongwang.top

memset(a, 0, sizeof a);
来源：http://dbq.jqgfzy.top

[S27] C：定义常量
来源：http://hyy.sysykeji.top

const double PI = 3.14159;
来源：http://amm.jinghuilouyu.cn

[S28] C：静态变量
来源：http://qcu.svipenyu.cn

static int counter = 0;
来源：http://xsk.ehwqpu.com

[S29] C：变参函数
来源：http://cqg.chenlongwang.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://swa.shanyushiyangtech.top

[S30] C：头文件保护
来源：http://tfx.tianlin.xyz

#ifndef X_H
来源：http://jsl.xuetiantiany.cn

#define X_H
来源：http://rdd.yuanzhike.top

#endif
来源：http://fwm.kuanghao11.cn

[S31] C++：Hello World
来源：http://byj.aizwys.cn

#include <iostream>
来源：http://aod.ivvv.top

int main() { std::cout << "Hello\n"; }
来源：http://yci.shanyushiyangtech.top

[S32] C++：字符串
来源：http://ncc.ivvv.top

std::string s = "hi";  s += "!";
来源：http://rel.xuetiantiany.cn

[S33] C++：vector 增删
来源：http://shm.kuanghao11.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pae.yuxming.cn

[S34] C++：遍历 vector
来源：http://msy.tian-w.cn

for (auto &x : v) { std::cout << x; }
来源：http://qgi.zdbjq.cn

[S35] C++：map
来源：http://oii.chenjidiqi.icu

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ctx.shzxlz.cn

[S36] C++：unordered_map
来源：http://skc.nanxinkj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dor.shanyushiyangtech.top

[S37] C++：set
来源：http://vcj.jinqigufen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ojy.52xcode.cn

[S38] C++：排序
来源：http://sjf.bbcook.cn

std::sort(v.begin(), v.end());
来源：http://rwe.chenlongwang.top

[S39] C++：自定义比较器排序
来源：http://bzq.tianlin.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hsl.yvedp.cn

[S40] C++：查找元素
来源：http://brz.shanyushiyangkeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ahw.fzhhl.top

[S41] C++：类与构造函数
来源：http://eqr.guowangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oum.gogol.net.cn

[S42] C++：继承与虚函数
来源：http://xyn.tian-w.cn

class B : public Base { public: void f() override {} };
来源：http://vlr.wangdashe.top

[S43] C++：智能指针
来源：http://uzy.fktsv.cn

auto p = std::make_unique<int>(5);
来源：http://nib.gogol.net.cn

[S44] C++：引用传参
来源：http://gsb.yj20258.top

void inc(int &x) { ++x; }
来源：http://rjc.fktsv.cn

[S45] C++：lambda
来源：http://npc.chenzaomai.com

auto add = [](int a, int b) { return a + b; };
来源：http://wut.daxiang520.top

[S46] C++：函数模板
来源：http://fol.52xcode.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rpn.jinqigfzy.top

[S47] C++：结构化绑定遍历
来源：http://fse.zhongyouzk.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://txe.xylfe.cn

[S48] C++：逐行读文件
来源：http://lfd.jlsjyb.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pst.c1oappe.top

while (std::getline(in, line)) { }
来源：http://osn.ctjpmb.com

[S49] C++：写文件
来源：http://zei.ydjk.org.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xxr.tarul.cn

[S50] C++：格式化数字
来源：http://vyp.hcnkem.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wds.yj20258.top

[S51] C++：显式类型转换
来源：http://ktr.tanke756.top

static_cast<double>(a) / b
来源：http://vig.hysaishi.cn

[S52] C++：const 与 noexcept
来源：http://tpv.cheryme.top

int size() const noexcept { return n_; }
来源：http://qpz.zhengqikj.top

[S53] C++：移动语义
来源：http://ssw.aizwys.cn

std::vector<int> w = std::move(v);
来源：http://mrn.yj20258.top

[S54] C++：异常处理
来源：http://ctd.gotoacloud.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kjz.chenzaomai.com

[S55] C++：结构化绑定
来源：http://mab.hnqzz.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qns.chenzaomai.com

[S56] C++：optional
来源：http://ehk.tianlin.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sny.gaohongyu789.top

[S57] C++：编译期常量
来源：http://uko.yvedp.cn

constexpr int N = 10;
来源：http://yyz.shuidangran.top

[S58] C++：命名空间
来源：http://bep.xylfe.cn

namespace ns { int f() { return 1; } }
来源：http://tfp.9152youxi.cn

[S59] C++：静态断言
来源：http://vjk.cqqwz.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mkn.epnwcf.com

[S60] C++：遍历并删除元素
来源：http://jni.hywenlv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nmt.xziqi.cn

================================================================================
来源：http://xac.zhongyouzk.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qfi.daxiang520.top

================================================================================
来源：http://tut.xuanzx.com

[T01] Kotlin：Hello World
来源：http://tik.tianlin.xyz

println("Hello")
来源：http://zrz.fengsongda.top

[T02] Kotlin：变量
来源：http://prx.zhijiandao.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://muk.316326.xyz

[T03] Kotlin：字符串模板
来源：http://vcf.svipenyu.cn

"值: $b"
来源：http://glu.ivvv.top

[T04] Kotlin：空安全
来源：http://exp.9152youxi.cn

val n: String? = null;  n?.length
来源：http://waw.sufxvd.cn

[T05] Kotlin：when 表达式
来源：http://zag.cucudq.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jso.0kj1m.cn

[T06] Kotlin：集合映射
来源：http://waa.wangdashe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://elf.guannengcc.top

[T07] Kotlin：集合过滤
来源：http://tyd.chenzaomai.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://zvl.guannengcc.top

[T08] Kotlin：数据类
来源：http://naq.fktsv.cn

data class User(val name: String, val age: Int)
来源：http://bsy.sjlbkw.cn

[T09] Kotlin：扩展函数
来源：http://mpd.jianghu66.top

fun String.exclaim() = this + "!"
来源：http://leh.svipenyu.cn

[T10] Kotlin：默认参数
来源：http://kmy.cashguo.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wws.jinqigfzy.top

[T11] Kotlin：协程
来源：http://ycj.sufxvd.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nrs.ywan-chungtsiang.top

[T12] Kotlin：解构声明
来源：http://kae.xingfuxueyuan.xyz

val (a, b) = Pair(1, 2)
来源：http://oso.pengpengdd.cyou

[T13] Kotlin：只读 Map
来源：http://lsv.yonumen.top

val m = mapOf("a" to 1)
来源：http://yxt.daxiang520.top

[T14] Kotlin：循环
来源：http://zjd.zdqjudy.top

for (i in 1..10) println(i)
来源：http://oao.yanxiufei.cn

[T15] Kotlin：接口
来源：http://hnr.yuanzhike.top

interface Shape { fun area(): Double }
来源：http://npl.0kj1m.cn

[T16] Swift：Hello World
来源：http://qrl.chenzaomai.com

print("Hello")
来源：http://hai.vehdjk.com

[T17] Swift：变量与常量
来源：http://wjq.daxiang520.top

var a = 1;  let b = 2
来源：http://rti.hfpthk.cn

[T18] Swift：字符串插值
来源：http://sva.ydjk.org.cn

"值: \(b)"
来源：http://tri.tarul.cn

[T19] Swift：可选绑定
来源：http://oaz.ctjpmb.com

if let n = opt { print(n) }
来源：http://wff.zhixingplan.top

[T20] Swift：数组操作
来源：http://flk.jinqigufen.top

var a = [1, 2, 3];  a.append(4)
来源：http://iqw.bbcook.cn

[T21] Swift：遍历
来源：http://bmh.dianchejie.cn

for x in a { print(x) }
来源：http://xyh.316326.xyz

[T22] Swift：字典
来源：http://kmg.smart0.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://cey.xuetiantiany.cn

[T23] Swift：函数
来源：http://veq.feifeiyinyue.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ere.yuanzhike.top

[T24] Swift：闭包
来源：http://ixs.havefunace.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ufq.pycfn.com

[T25] Swift：结构体
来源：http://xer.gotoacloud.top

struct P { var x: Int }
来源：http://dop.ctjpmb.com

[T26] Swift：类与重写
来源：http://rnd.jiagoushi.top

class A: Base { override func f() {} }
来源：http://rym.c1oappe.top

[T27] Swift：错误处理
来源：http://ldc.sjlbkw.cn

do { try f() } catch { print(error) }
来源：http://veg.xuetiantiany.cn

[T28] Swift：枚举
来源：http://zne.hnqzz.top

enum Color { case red, green }
来源：http://msn.c1oappe.top

[T29] Swift：guard 提前返回
来源：http://dqc.pengpengdd.cyou

guard let x = opt else { return }
来源：http://wch.cashguo.top

[T30] Swift：协议
来源：http://vqe.jinghuilouyu.cn

protocol Shape { func area() -> Double }
来源：http://dut.zhixingplan.top

[T31] Lua：Hello World
来源：http://moc.ydjk.org.cn

print("Hello")
来源：http://xjy.zhijiandao.cn

[T32] Lua：局部变量
来源：http://soo.chenlongwang.top

local a = 1
来源：http://pvv.c1oappe.top

[T33] Lua：表（数组）
来源：http://acx.vehdjk.com

local t = {1, 2, 3};  t[4] = 4
来源：http://ues.epnwcf.com

[T34] Lua：遍历表
来源：http://onp.ctjpmb.com

for i, v in ipairs(t) do print(i, v) end
来源：http://yci.shzxlz.cn

[T35] Lua：字典表
来源：http://kst.zhongyouzk.top

local d = { a = 1 };  d.b = 2
来源：http://dyi.quarkkingdee.top

[T36] Lua：函数
来源：http://kdl.guannengcc.top

function add(a, b) return a + b end
来源：http://gns.fengsongda.top

[T37] Lua：字符串拼接
来源：http://ibi.hfpthk.cn

"a" .. "b"
来源：http://mnq.c1oappe.top

[T38] Lua：条件
来源：http://hed.cashguo.top

if x > 0 then print("正") end
来源：http://jfd.uphjek.com

[T39] Lua：模式匹配
来源：http://tvf.ywan-chungtsiang.top

string.find(s, "%d+")
来源：http://qmr.hysaishi.cn

[T40] Lua：元表
来源：http://hiq.vehdjk.com

setmetatable({}, { __index = base })
来源：http://cvs.yfazqb.com

[T41] Perl：Hello World
来源：http://zgq.guannengcc.top

print "Hello\n";
来源：http://dla.aibaodan.cn

[T42] Perl：变量类型
来源：http://mjk.yangfankeji.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lcu.ybcxt.top


<!-- 参考信息 -->