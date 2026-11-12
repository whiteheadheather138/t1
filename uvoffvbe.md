代发 wailian999

files=$(ls -1)
来源：http://ngr.zhongyouzk.top

[R38] 管道串联
来源：http://syc.ybcxt.top

cat a.txt | grep -i error | wc -l
来源：http://qtp.jianghu66.top

[R39] 重定向标准输出与错误
来源：http://wpx.jqgufenzy.top

cmd > out.log 2>&1
来源：http://ceu.gotoacloud.top

[R40] 追加写日志
来源：http://qmy.xinyue.icu

echo "log" >> out.log
来源：http://aoj.hnxiangtu.top

[R41] 丢弃输出
来源：http://lxj.0kj1m.cn

cmd >/dev/null 2>&1
来源：http://zgv.pycfn.com

[R42] 输入重定向
来源：http://cns.gotoacloud.top

wc -l < a.txt
来源：http://hnt.hesvh.cn

[R43] 按名字查找文件
来源：http://suo.zhoulong.xyz

find . -name "*.log" -type f
来源：http://hss.redwolf501.top

[R44] 按修改时间查找
来源：http://dng.uphjek.com

find . -mtime -7 -type f
来源：http://ced.gogol.net.cn

[R45] 批量删除
来源：http://lap.hnxiangtu.top

find . -name "*.tmp" -delete
来源：http://odu.nanxuanxn.top

[R46] 递归替换文件内容
来源：http://rzh.dashuyun.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hfu.yfazqb.com

[R47] sed 单行替换
来源：http://ovm.chenlongwang.top

sed -i 's/foo/bar/g' a.txt
来源：http://mwf.iojbl.cn

[R48] awk 取指定列
来源：http://lrh.aizwys.cn

awk '{print $1, $3}' a.txt
来源：http://kcc.sweek.top

[R49] awk 带条件
来源：http://cre.svipenyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dax.andypj.xyz

[R50] awk 求和
来源：http://ars.cdnleiting.top

awk '{s += $2} END {print s}' a.txt
来源：http://dek.jinghuilouyu.cn

[R51] 排序去重取前几
来源：http://iuy.pycfn.com

sort a.txt | uniq -c | sort -rn | head
来源：http://aok.tianlin.xyz

[R52] 统计行数
来源：http://fku.uphjek.com

wc -l a.txt
来源：http://ryu.gotoacloud.top

[R53] 查看文件头与实时尾
来源：http://imr.zhoulong.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cqb.haohaochexian.top

[R54] 比较两个文件
来源：http://sji.uphjek.com

diff a.txt b.txt
来源：http://yqz.feifeiyinyue.top

[R55] 压缩与解压
来源：http://ble.dashuyun.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ghg.epnwcf.com

[R56] 远程拷贝
来源：http://iwn.fengsongda.top

scp file user@host:/path/
来源：http://yij.jiagoushi.top

[R57] 远程执行命令
来源：http://ylf.daria6918.cn

ssh user@host 'uptime'
来源：http://nkb.hnqzz.top

[R58] 下载文件
来源：http://etg.tanke756.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ksz.shangyingyoupin.top

[R59] 发 POST JSON
来源：http://ecl.sjlbkw.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vlf.fzhhl.top

[R60] 只看 HTTP 状态码
来源：http://ytz.jinghuilouyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lqc.yuxming.cn

[R61] 磁盘占用
来源：http://vuy.fanxiaobao.xyz

df -h;  du -sh *
来源：http://mun.jyoumei.cn

[R62] 找最占空间的文件
来源：http://eex.havefunace.top

du -ah . | sort -rh | head -10
来源：http://mde.gaohongyu789.top

[R63] 内存与进程
来源：http://ncc.haohaochexian.top

free -h;  ps aux | grep nginx
来源：http://mpn.sysykeji.top

[R64] 结束进程
来源：http://esw.yj20258888.top

kill -9 $(pgrep -f app.py)
来源：http://wyk.shuidangran.top

[R65] 查看端口占用
来源：http://sbt.yuxming.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vdx.hywenlv.cn

[R66] 定时任务
来源：http://rhv.c1oappe.top

crontab -e;  crontab -l
来源：http://mep.nanxuanxn.top

[R67] 生成随机十六进制串
来源：http://nyn.jqgufenzy.top

openssl rand -hex 16
来源：http://qph.birdmap.top

[R68] 计算文件校验值
来源：http://wwo.epnwcf.com

sha256sum a.txt;  md5sum a.txt
来源：http://xgr.vehdjk.com

[R69] 生成随机密码
来源：http://xzs.vehdjk.com

head -c 16 /dev/urandom | base64
来源：http://hsn.guowangkeji.top

[R70] 时间戳与互转
来源：http://qcb.xylfe.cn

date +%s;  date -d @1700000000
来源：http://sch.cdnleiting.top

[R71] 日期格式化
来源：http://zsc.yongpay.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://tip.xuetiantiany.cn

[R72] 等待端口就绪
来源：http://dol.ydzc1.top

until nc -z localhost 3306; do sleep 1; done
来源：http://krf.xinyue.icu

[R73] 分割大日志
来源：http://wuu.sufxvd.cn

split -l 1000 big.log part_
来源：http://txx.yanxiufei.cn

[R74] 批量重命名
来源：http://udw.chenjidiqi.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zzf.tianlin.xyz

[R75] 导出环境变量
来源：http://jzs.fehbvm.com

export PATH="$HOME/bin:$PATH"
来源：http://wuy.zycfv.cn

[R76] 使用临时文件
来源：http://sbs.jiagoushi.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gwl.meibo888.top

[R77] 读取用户输入
来源：http://ghk.redwolf501.top

read -rp "请输入: " ans
来源：http://blw.bbcook.cn

[R78] 交互式菜单
来源：http://hoc.fzhhl.top

select opt in a b c; do echo "$opt"; break; done
来源：http://pjw.sysykeji.top

[R79] 解析命令行选项
来源：http://wqa.nwbrower.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jrb.hfpthk.cn

[R80] 查看脚本执行耗时
来源：http://tpx.nanxinkj.top

time ./run.sh
来源：http://wld.jinqigufen.top

================================================================================
来源：http://wem.jinghuilouyu.cn

S. C / C++ 专题
来源：http://huq.ybcxt.top

================================================================================
来源：http://czw.jqgfzy.top

[S01] C：Hello World
来源：http://mhb.hesvh.cn

#include <stdio.h>
来源：http://gek.ybcxt.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://tqd.fehbvm.com

[S02] C：变量与格式化输出
来源：http://tjg.ehwqpu.com

int a = 10; printf("%d\n", a);
来源：http://okd.ehwqpu.com

[S03] C：读入整数
来源：http://ajy.yj20258.top

int x; scanf("%d", &x);
来源：http://qcw.nwbrower.top

[S04] C：字符串复制
来源：http://lvk.xuanzx.com

char dst[32]; strcpy(dst, "hi");
来源：http://cqo.guowangkeji.top

[S05] C：字符串长度
来源：http://qhe.zhongyouzk.top

strlen(s)
来源：http://gop.xingfuxueyuan.xyz

[S06] C：字符串比较
来源：http://dwg.yongpay.top

strcmp(a, b) == 0
来源：http://nwl.vehdjk.com

[S07] C：数组遍历求和
来源：http://bdl.hywenlv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wbx.ydzc1.top

[S08] C：动态内存分配与释放
来源：http://hyd.zhoulong.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ivd.xziqi.cn

[S09] C：结构体定义与初始化
来源：http://jfc.vqdsnc.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jpw.zhijiandao.cn

[S10] C：指针与解引用
来源：http://ltd.cashguo.top

int *p = &a;  *p = 5;
来源：http://bvx.shangyingyoupin.top

[S11] C：逐行读文件
来源：http://hit.yangfankeji.com

FILE *f = fopen("a.txt", "r");
来源：http://mie.guowangkeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://zls.shzxlz.cn

fclose(f);
来源：http://cjd.52xcode.cn

[S12] C：写文件
来源：http://uup.zdqjudy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zto.ctjpmb.com

[S13] C：宏定义
来源：http://gey.xylfe.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fjr.sysykeji.top

[S14] C：枚举
来源：http://zcq.sjlbkw.cn

enum Color { RED, GREEN, BLUE };
来源：http://zwx.shanyushiyangkeji.top

[S15] C：类型转换
来源：http://npx.sweek.top

(double) a / b
来源：http://rne.hnxiangtu.top

[S16] C：位操作置位
来源：http://uuv.gotoacloud.top

x |= (1 << 3);
来源：http://hkb.bbcook.cn

[S17] C：安全拼接字符串
来源：http://ntk.9152youxi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gvu.xuanzx.com

[S18] C：命令行参数
来源：http://hri.gotoacloud.top

int main(int argc, char **argv)
来源：http://jxw.fzhhl.top

[S19] C：快速排序
来源：http://ajo.hesvh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mtu.cdnleiting.top

[S20] C：二分查找
来源：http://lip.bjfxy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://osj.yfazqb.com

[S21] C：字符类别判断
来源：http://bja.xylfe.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qyl.birdmap.top

[S22] C：字符串转数字
来源：http://ueu.zycfv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nii.hysaishi.cn

[S23] C：随机数
来源：http://kzw.snrcjt.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://apx.gaohongyu789.top

[S24] C：获取本地时间
来源：http://iqq.daxiang520.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://agu.zhengqikj.top

[S25] C：内存拷贝
来源：http://mjj.gaohongyu789.top

memcpy(dst, src, n);
来源：http://pav.xziqi.cn

[S26] C：内存清零
来源：http://qxr.aizwys.cn

memset(a, 0, sizeof a);
来源：http://dqh.bbcook.cn

[S27] C：定义常量
来源：http://ixo.uphjek.com

const double PI = 3.14159;
来源：http://jxw.hesvh.cn

[S28] C：静态变量
来源：http://bhe.tianlin.xyz

static int counter = 0;
来源：http://lbc.ivvv.top

[S29] C：变参函数
来源：http://jdc.snrcjt.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nbo.guannengcc.top

[S30] C：头文件保护
来源：http://ipw.xziqi.cn

#ifndef X_H
来源：http://mzc.haohaochexian.top

#define X_H
来源：http://uoa.nanxinkj.top

#endif
来源：http://dnd.xuanzx.com

[S31] C++：Hello World
来源：http://too.dianchejie.cn

#include <iostream>
来源：http://qcc.snrcjt.cn

int main() { std::cout << "Hello\n"; }
来源：http://blv.snrcjt.cn

[S32] C++：字符串
来源：http://hsd.hesvh.cn

std::string s = "hi";  s += "!";
来源：http://izl.xziqi.cn

[S33] C++：vector 增删
来源：http://far.xylfe.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vfq.andypj.xyz

[S34] C++：遍历 vector
来源：http://sfd.vehdjk.com

for (auto &x : v) { std::cout << x; }
来源：http://ivb.wangshuangyany.cn

[S35] C++：map
来源：http://csa.feifeiyinyue.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hmr.yueranfly.top

[S36] C++：unordered_map
来源：http://ucc.guowangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gzc.meibo888.top

[S37] C++：set
来源：http://gfh.shangyingyoupin.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zbd.snrcjt.cn

[S38] C++：排序
来源：http://bhx.yongpay.top

std::sort(v.begin(), v.end());
来源：http://ugs.zhijiandao.cn

[S39] C++：自定义比较器排序
来源：http://syg.yongpay.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://chd.tarul.cn

[S40] C++：查找元素
来源：http://djy.zdbjq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ywy.zhijiandao.cn

[S41] C++：类与构造函数
来源：http://dah.gotoacloud.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lwz.redwolf501.top

[S42] C++：继承与虚函数
来源：http://ugu.daria6918.cn

class B : public Base { public: void f() override {} };
来源：http://osd.zhaomingkeji.xyz

[S43] C++：智能指针
来源：http://rcu.bbcook.cn

auto p = std::make_unique<int>(5);
来源：http://tms.yj20258888.top

[S44] C++：引用传参
来源：http://isc.vqdsnc.cn

void inc(int &x) { ++x; }
来源：http://gbr.sufxvd.cn

[S45] C++：lambda
来源：http://pjd.zdbjq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ljs.bjfxy.top

[S46] C++：函数模板
来源：http://tvr.fktsv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://asm.cheryme.top

[S47] C++：结构化绑定遍历
来源：http://umj.guowangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://spl.shuidangran.top

[S48] C++：逐行读文件
来源：http://sdh.hnxiangtu.top

std::ifstream in("a.txt");  std::string line;
来源：http://kvf.havefunace.top

while (std::getline(in, line)) { }
来源：http://zyb.0kj1m.cn

[S49] C++：写文件
来源：http://ady.cashguo.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://byc.jinyuanbaomall.cn

[S50] C++：格式化数字
来源：http://ydu.aibaodan.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ghn.52xcode.cn

[S51] C++：显式类型转换
来源：http://fxk.redwolf501.top

static_cast<double>(a) / b
来源：http://yvq.zhongyouzk.top

[S52] C++：const 与 noexcept
来源：http://jxt.fzhhl.top

int size() const noexcept { return n_; }
来源：http://szz.snrcjt.cn

[S53] C++：移动语义
来源：http://jrk.uphjek.com

std::vector<int> w = std::move(v);
来源：http://ifq.daxiang520.top

[S54] C++：异常处理
来源：http://nnp.gogol.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zta.tanke756.top

[S55] C++：结构化绑定
来源：http://vji.yuxming.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xbo.tanke756.top

[S56] C++：optional
来源：http://jqr.hesvh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uin.fktsv.cn

[S57] C++：编译期常量
来源：http://nqu.zdbjq.cn

constexpr int N = 10;
来源：http://cpu.yueranfly.top

[S58] C++：命名空间
来源：http://gpu.gaohongyu789.top

namespace ns { int f() { return 1; } }
来源：http://kmu.sufxvd.cn

[S59] C++：静态断言
来源：http://ugj.sjlbkw.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ovd.nanxinkj.top

[S60] C++：遍历并删除元素
来源：http://bic.nwbrower.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hzp.svipenyu.cn

================================================================================
来源：http://cso.nwbrower.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wvb.zhijiandao.cn

================================================================================
来源：http://qot.ydjk.org.cn

[T01] Kotlin：Hello World
来源：http://ygh.jqgufenzy.top

println("Hello")
来源：http://eog.xuanzx.com

[T02] Kotlin：变量
来源：http://mhu.vehdjk.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://edh.haohaochexian.top

[T03] Kotlin：字符串模板
来源：http://yev.yuanzhike.top

"值: $b"
来源：http://aas.andypj.xyz

[T04] Kotlin：空安全
来源：http://whh.fanxiaobao.xyz

val n: String? = null;  n?.length
来源：http://ndl.hnxiangtu.top

[T05] Kotlin：when 表达式
来源：http://zmb.yj20258888.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pzf.ybcxt.top

[T06] Kotlin：集合映射
来源：http://ily.sweek.top

listOf(1, 2, 3).map { it * 2 }
来源：http://sie.yueranfly.top

[T07] Kotlin：集合过滤
来源：http://xmw.hnqzz.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kkf.fzhhl.top

[T08] Kotlin：数据类
来源：http://yrp.zhijiandao.cn

data class User(val name: String, val age: Int)
来源：http://wfn.zhoulong.xyz

[T09] Kotlin：扩展函数
来源：http://ezs.ppjwa.cn

fun String.exclaim() = this + "!"
来源：http://pxh.cucudq.cn

[T10] Kotlin：默认参数
来源：http://uhd.gaohongyu789.top

fun greet(name: String = "World") = "Hi $name"
来源：http://iog.dashuyun.cn

[T11] Kotlin：协程
来源：http://yjj.yvedp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jjr.uphjek.com

[T12] Kotlin：解构声明
来源：http://kgn.hammf.cn

val (a, b) = Pair(1, 2)
来源：http://day.haohaochexian.top

[T13] Kotlin：只读 Map
来源：http://ogd.zycfv.cn

val m = mapOf("a" to 1)
来源：http://mtd.kuanghao11.cn

[T14] Kotlin：循环
来源：http://nks.iojbl.cn

for (i in 1..10) println(i)
来源：http://urh.xylfe.cn

[T15] Kotlin：接口
来源：http://hks.chenjidiqi.icu

interface Shape { fun area(): Double }
来源：http://ycd.nanxuanxn.top

[T16] Swift：Hello World
来源：http://qpa.sysykeji.top

print("Hello")
来源：http://hgy.pengpengdd.cyou

[T17] Swift：变量与常量
来源：http://elr.meibo888.top

var a = 1;  let b = 2
来源：http://wtj.chenzaomai.com

[T18] Swift：字符串插值
来源：http://ppc.shanyushiyangkeji.top

"值: \(b)"
来源：http://gll.shanyushiyangtech.top

[T19] Swift：可选绑定
来源：http://kzv.sxryk.cn

if let n = opt { print(n) }
来源：http://vco.ywan-chungtsiang.top

[T20] Swift：数组操作
来源：http://ket.gogol.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pea.jinqigfzy.top

[T21] Swift：遍历
来源：http://tpc.xziqi.cn

for x in a { print(x) }
来源：http://fto.9152youxi.cn

[T22] Swift：字典
来源：http://hed.cashguo.top

var d = ["a": 1];  d["b"] = 2
来源：http://tlo.zhaomingkeji.xyz

[T23] Swift：函数
来源：http://vkm.sxryk.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gjk.jlsjyb.cn

[T24] Swift：闭包
来源：http://tkc.bbcook.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://iid.zhaomingkeji.xyz

[T25] Swift：结构体
来源：http://xfq.havefunace.top

struct P { var x: Int }
来源：http://ulu.bjfxy.top

[T26] Swift：类与重写
来源：http://gdr.dashuyun.cn

class A: Base { override func f() {} }
来源：http://mzi.cheryme.top

[T27] Swift：错误处理
来源：http://tki.bbcook.cn

do { try f() } catch { print(error) }
来源：http://jfz.hnxiangtu.top

[T28] Swift：枚举
来源：http://rjm.wangdashe.top

enum Color { case red, green }
来源：http://aoj.nanxuanxn.top

[T29] Swift：guard 提前返回
来源：http://wim.52xcode.cn

guard let x = opt else { return }
来源：http://kfx.jinyuanbaomall.cn

[T30] Swift：协议
来源：http://dkv.zhoulong.xyz

protocol Shape { func area() -> Double }
来源：http://suo.bbcook.cn

[T31] Lua：Hello World
来源：http://qqe.andypj.xyz

print("Hello")
来源：http://myy.gzhubu.top

[T32] Lua：局部变量
来源：http://ftq.sxryk.cn

local a = 1
来源：http://mjj.jqgfzy.top

[T33] Lua：表（数组）
来源：http://hto.c1oappe.top

local t = {1, 2, 3};  t[4] = 4
来源：http://mkm.sysykeji.top

[T34] Lua：遍历表
来源：http://kcd.shuidangran.top

for i, v in ipairs(t) do print(i, v) end
来源：http://bco.jinyuanbaomall.cn

[T35] Lua：字典表
来源：http://dvt.hysaishi.cn

local d = { a = 1 };  d.b = 2
来源：http://ryn.cheryme.top

[T36] Lua：函数
来源：http://krw.ydjk.org.cn

function add(a, b) return a + b end
来源：http://yje.fzhhl.top

[T37] Lua：字符串拼接
来源：http://bfm.jqgufenzy.top

"a" .. "b"
来源：http://vai.yvedp.cn

[T38] Lua：条件
来源：http://xzc.cheryme.top

if x > 0 then print("正") end
来源：http://jtj.mhx1999.top

[T39] Lua：模式匹配
来源：http://hao.ivvv.top

string.find(s, "%d+")
来源：http://hyw.xylfe.cn

[T40] Lua：元表
来源：http://ppw.52xcode.cn

setmetatable({}, { __index = base })
来源：http://vif.kuanghao11.cn


<!-- 参考信息 -->