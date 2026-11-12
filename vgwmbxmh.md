代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://hnk.haohaochexian.top

[R36] 并发执行多个任务
来源：http://cdw.feifeiyinyue.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tpt.sysykeji.top

[R37] 把输出赋给变量
来源：http://tfz.jinqigufen.top

files=$(ls -1)
来源：http://krj.hnxiangtu.top

[R38] 管道串联
来源：http://xgs.ybcxt.top

cat a.txt | grep -i error | wc -l
来源：http://nzj.birdmap.top

[R39] 重定向标准输出与错误
来源：http://ohd.daria6918.cn

cmd > out.log 2>&1
来源：http://ddc.tanke756.top

[R40] 追加写日志
来源：http://rft.yvedp.cn

echo "log" >> out.log
来源：http://tqw.hysaishi.cn

[R41] 丢弃输出
来源：http://epl.fanxiaobao.xyz

cmd >/dev/null 2>&1
来源：http://qst.zdqjudy.top

[R42] 输入重定向
来源：http://yor.yfazqb.com

wc -l < a.txt
来源：http://oca.fzhhl.top

[R43] 按名字查找文件
来源：http://irf.yfazqb.com

find . -name "*.log" -type f
来源：http://mkp.ivvv.top

[R44] 按修改时间查找
来源：http://voq.cdnleiting.top

find . -mtime -7 -type f
来源：http://mjf.ybcxt.top

[R45] 批量删除
来源：http://pcs.nwbrower.top

find . -name "*.tmp" -delete
来源：http://pyo.zhoulong.xyz

[R46] 递归替换文件内容
来源：http://gqx.chenlongwang.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qit.cdnleiting.top

[R47] sed 单行替换
来源：http://bem.jinyuanbaomall.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qmi.yj202588.top

[R48] awk 取指定列
来源：http://mea.yuxming.cn

awk '{print $1, $3}' a.txt
来源：http://erq.jinyuanbaomall.cn

[R49] awk 带条件
来源：http://gqa.jinghuilouyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vcr.zhengqikj.top

[R50] awk 求和
来源：http://dcu.xingfuxueyuan.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://xzn.bbcook.cn

[R51] 排序去重取前几
来源：http://hsg.cucudq.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hys.gzhubu.top

[R52] 统计行数
来源：http://tyf.hesvh.cn

wc -l a.txt
来源：http://gvb.chenlongwang.top

[R53] 查看文件头与实时尾
来源：http://bhj.feifeiyinyue.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jky.yfazqb.com

[R54] 比较两个文件
来源：http://hnu.epnwcf.com

diff a.txt b.txt
来源：http://ezt.guannengcc.top

[R55] 压缩与解压
来源：http://hkc.ybcxt.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ebk.jlsjyb.cn

[R56] 远程拷贝
来源：http://nem.tarul.cn

scp file user@host:/path/
来源：http://upr.zhaomingkeji.xyz

[R57] 远程执行命令
来源：http://xom.zhongyouzk.top

ssh user@host 'uptime'
来源：http://pfk.yueranfly.top

[R58] 下载文件
来源：http://fua.yuxming.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jeu.jiagoushi.top

[R59] 发 POST JSON
来源：http://lyy.andypj.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://juw.aizwys.cn

[R60] 只看 HTTP 状态码
来源：http://ltf.bbcook.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jkc.tarul.cn

[R61] 磁盘占用
来源：http://pbw.hammf.cn

df -h;  du -sh *
来源：http://faq.vqdsnc.cn

[R62] 找最占空间的文件
来源：http://clc.jyoumei.cn

du -ah . | sort -rh | head -10
来源：http://zeh.yueranfly.top

[R63] 内存与进程
来源：http://nnc.jlsjyb.cn

free -h;  ps aux | grep nginx
来源：http://zar.xingfuxueyuan.xyz

[R64] 结束进程
来源：http://jev.gotoacloud.top

kill -9 $(pgrep -f app.py)
来源：http://ohz.gogol.net.cn

[R65] 查看端口占用
来源：http://rit.wangdashe.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ixu.wangdashe.top

[R66] 定时任务
来源：http://bpy.ivvv.top

crontab -e;  crontab -l
来源：http://tzg.sysykeji.top

[R67] 生成随机十六进制串
来源：http://gks.9152youxi.cn

openssl rand -hex 16
来源：http://twn.xylfe.cn

[R68] 计算文件校验值
来源：http://ymg.52xcode.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qeq.jinghuilouyu.cn

[R69] 生成随机密码
来源：http://fmm.aizwys.cn

head -c 16 /dev/urandom | base64
来源：http://jsr.daxiang520.top

[R70] 时间戳与互转
来源：http://tcl.fktsv.cn

date +%s;  date -d @1700000000
来源：http://tvy.bbcook.cn

[R71] 日期格式化
来源：http://yxo.andypj.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://oln.ppjwa.cn

[R72] 等待端口就绪
来源：http://hsn.wangshuangyany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nli.chenjidiqi.icu

[R73] 分割大日志
来源：http://sij.yj20258888.top

split -l 1000 big.log part_
来源：http://hal.xziqi.cn

[R74] 批量重命名
来源：http://znb.feifeiyinyue.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ydc.yueranfly.top

[R75] 导出环境变量
来源：http://tsl.bbcook.cn

export PATH="$HOME/bin:$PATH"
来源：http://mvu.aibaodan.cn

[R76] 使用临时文件
来源：http://xfk.shangyingyoupin.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rbv.andypj.xyz

[R77] 读取用户输入
来源：http://rne.dianchejie.cn

read -rp "请输入: " ans
来源：http://wrf.cheryme.top

[R78] 交互式菜单
来源：http://ayn.zhaomingkeji.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://izc.hongshengwenyu.top

[R79] 解析命令行选项
来源：http://gfl.chenzaomai.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zth.cdnleiting.top

[R80] 查看脚本执行耗时
来源：http://pgw.nwbrower.top

time ./run.sh
来源：http://kfo.guowangkeji.top

================================================================================
来源：http://mkl.zhijiandao.cn

S. C / C++ 专题
来源：http://hxn.xinyue.icu

================================================================================
来源：http://lnn.hfpthk.cn

[S01] C：Hello World
来源：http://rbc.ivvv.top

#include <stdio.h>
来源：http://rnb.shangyingyoupin.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://kyq.feifeiyinyue.top

[S02] C：变量与格式化输出
来源：http://fdn.zhiwuduotai.top

int a = 10; printf("%d\n", a);
来源：http://fzj.jinqigfzy.top

[S03] C：读入整数
来源：http://gmz.gzhubu.top

int x; scanf("%d", &x);
来源：http://kux.dianchejie.cn

[S04] C：字符串复制
来源：http://kob.sxryk.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mhc.mhx1999.top

[S05] C：字符串长度
来源：http://hta.shuidangran.top

strlen(s)
来源：http://wcx.sxryk.cn

[S06] C：字符串比较
来源：http://ywp.zhijiandao.cn

strcmp(a, b) == 0
来源：http://qoy.yvedp.cn

[S07] C：数组遍历求和
来源：http://otr.jlsjyb.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rbj.c1oappe.top

[S08] C：动态内存分配与释放
来源：http://cmf.svipenyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tsj.pycfn.com

[S09] C：结构体定义与初始化
来源：http://ipq.zdqjudy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://iqz.cdnleiting.top

[S10] C：指针与解引用
来源：http://yim.yangfankeji.com

int *p = &a;  *p = 5;
来源：http://sve.wangshuangyany.cn

[S11] C：逐行读文件
来源：http://wzt.jianghu66.top

FILE *f = fopen("a.txt", "r");
来源：http://ega.fehbvm.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://kmy.nwbrower.top

fclose(f);
来源：http://hri.zhongyouzk.top

[S12] C：写文件
来源：http://hre.cashguo.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dem.redwolf501.top

[S13] C：宏定义
来源：http://thb.chenzaomai.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ubg.ydzc1.top

[S14] C：枚举
来源：http://vzi.yuxming.cn

enum Color { RED, GREEN, BLUE };
来源：http://zth.shanyushiyangkeji.top

[S15] C：类型转换
来源：http://tcj.ivvv.top

(double) a / b
来源：http://jwj.shzxlz.cn

[S16] C：位操作置位
来源：http://kmc.ivvv.top

x |= (1 << 3);
来源：http://zvm.mhx1999.top

[S17] C：安全拼接字符串
来源：http://vfv.havefunace.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://egh.wangshuangyany.cn

[S18] C：命令行参数
来源：http://ken.hywenlv.cn

int main(int argc, char **argv)
来源：http://eay.pengpengdd.cyou

[S19] C：快速排序
来源：http://fpf.guowangkeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://aqt.hnxiangtu.top

[S20] C：二分查找
来源：http://fvl.birdmap.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kwe.yj20258.top

[S21] C：字符类别判断
来源：http://nsh.dashuyun.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qgp.pycfn.com

[S22] C：字符串转数字
来源：http://ppj.nwbrower.top

atoi("42");  strtod("3.14", NULL);
来源：http://wlb.jinyuanbaomall.cn

[S23] C：随机数
来源：http://ovw.zycfv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rne.hysaishi.cn

[S24] C：获取本地时间
来源：http://rsv.gzhubu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cvy.snrcjt.cn

[S25] C：内存拷贝
来源：http://smr.svipenyu.cn

memcpy(dst, src, n);
来源：http://bvg.cheryme.top

[S26] C：内存清零
来源：http://ljn.guannengcc.top

memset(a, 0, sizeof a);
来源：http://uzi.zycfv.cn

[S27] C：定义常量
来源：http://lap.cqqwz.cn

const double PI = 3.14159;
来源：http://ndc.ehwqpu.com

[S28] C：静态变量
来源：http://rvu.cheryme.top

static int counter = 0;
来源：http://qjj.snrcjt.cn

[S29] C：变参函数
来源：http://pfg.yj202588.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wtz.hammf.cn

[S30] C：头文件保护
来源：http://bez.fehbvm.com

#ifndef X_H
来源：http://xzi.cqqwz.cn

#define X_H
来源：http://njr.chenjidiqi.icu

#endif
来源：http://kpb.guannengcc.top

[S31] C++：Hello World
来源：http://bxy.yongpay.top

#include <iostream>
来源：http://zbq.guannengcc.top

int main() { std::cout << "Hello\n"; }
来源：http://uxm.ydzc1.top

[S32] C++：字符串
来源：http://riz.shzxlz.cn

std::string s = "hi";  s += "!";
来源：http://btb.mhx1999.top

[S33] C++：vector 增删
来源：http://twy.sweek.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mun.zhijiandao.cn

[S34] C++：遍历 vector
来源：http://peg.birdmap.top

for (auto &x : v) { std::cout << x; }
来源：http://itc.ybcxt.top

[S35] C++：map
来源：http://pfo.wangshuangyany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vjb.ydzc1.top

[S36] C++：unordered_map
来源：http://jrd.shuidangran.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pey.yongpay.top

[S37] C++：set
来源：http://bpc.shanyushiyangtech.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ary.pengpengdd.cyou

[S38] C++：排序
来源：http://bmh.pycfn.com

std::sort(v.begin(), v.end());
来源：http://jui.pycfn.com

[S39] C++：自定义比较器排序
来源：http://eqi.nwbrower.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xsw.shanyushiyangkeji.top

[S40] C++：查找元素
来源：http://zhq.shzxlz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tbb.yfazqb.com

[S41] C++：类与构造函数
来源：http://ynu.shangyingyoupin.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cec.wangdashe.top

[S42] C++：继承与虚函数
来源：http://cyu.hfpthk.cn

class B : public Base { public: void f() override {} };
来源：http://ovg.bbcook.cn

[S43] C++：智能指针
来源：http://idj.dianchejie.cn

auto p = std::make_unique<int>(5);
来源：http://fpn.fengsongda.top

[S44] C++：引用传参
来源：http://gsh.yfazqb.com

void inc(int &x) { ++x; }
来源：http://hou.gaohongyu789.top

[S45] C++：lambda
来源：http://okn.jyoumei.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nqi.yfazqb.com

[S46] C++：函数模板
来源：http://urg.hnxiangtu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pzi.gogol.net.cn

[S47] C++：结构化绑定遍历
来源：http://key.tian-w.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lug.jlsjyb.cn

[S48] C++：逐行读文件
来源：http://mpv.zdbjq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://itu.gogol.net.cn

while (std::getline(in, line)) { }
来源：http://jqj.fengsongda.top

[S49] C++：写文件
来源：http://akw.tian-w.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ual.hfpthk.cn

[S50] C++：格式化数字
来源：http://flp.ppjwa.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mna.hcnkem.com

[S51] C++：显式类型转换
来源：http://ngi.jianghu66.top

static_cast<double>(a) / b
来源：http://zko.yonumen.top

[S52] C++：const 与 noexcept
来源：http://yld.bbcook.cn

int size() const noexcept { return n_; }
来源：http://mbo.gaohongyu789.top

[S53] C++：移动语义
来源：http://wuf.xinyue.icu

std::vector<int> w = std::move(v);
来源：http://orw.xylfe.cn

[S54] C++：异常处理
来源：http://kmi.yuanzhike.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://itl.dianchejie.cn

[S55] C++：结构化绑定
来源：http://tvf.cqqwz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bxg.aizwys.cn

[S56] C++：optional
来源：http://qgd.cdnleiting.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wyk.gogol.net.cn

[S57] C++：编译期常量
来源：http://qpb.jianghu66.top

constexpr int N = 10;
来源：http://aqt.yanxiufei.cn

[S58] C++：命名空间
来源：http://izh.yj20258.top

namespace ns { int f() { return 1; } }
来源：http://iro.havefunace.top

[S59] C++：静态断言
来源：http://yvb.ppjwa.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zjl.yongpay.top

[S60] C++：遍历并删除元素
来源：http://zki.birdmap.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://meu.yj20258.top

================================================================================
来源：http://pqo.vqdsnc.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wvx.0kj1m.cn

================================================================================
来源：http://cep.yueranfly.top

[T01] Kotlin：Hello World
来源：http://pbd.dianchejie.cn

println("Hello")
来源：http://cwy.52xcode.cn

[T02] Kotlin：变量
来源：http://cvl.havefunace.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://eor.hesvh.cn

[T03] Kotlin：字符串模板
来源：http://wgo.dashuyun.cn

"值: $b"
来源：http://lnx.tianlin.xyz

[T04] Kotlin：空安全
来源：http://evu.guannengcc.top

val n: String? = null;  n?.length
来源：http://bcq.meibo888.top

[T05] Kotlin：when 表达式
来源：http://jmd.zhijiandao.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rdx.yfazqb.com

[T06] Kotlin：集合映射
来源：http://dmn.tarul.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://emg.jinqigfzy.top

[T07] Kotlin：集合过滤
来源：http://kil.birdmap.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kjl.tarul.cn

[T08] Kotlin：数据类
来源：http://gpk.hnqzz.top

data class User(val name: String, val age: Int)
来源：http://gha.shuidangran.top

[T09] Kotlin：扩展函数
来源：http://qed.yongpay.top

fun String.exclaim() = this + "!"
来源：http://stw.ywan-chungtsiang.top

[T10] Kotlin：默认参数
来源：http://syt.zhiwuduotai.top

fun greet(name: String = "World") = "Hi $name"
来源：http://xyt.sufxvd.cn

[T11] Kotlin：协程
来源：http://dcg.hnxiangtu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://qyt.dashuyun.cn

[T12] Kotlin：解构声明
来源：http://dbo.nanxuanxn.top

val (a, b) = Pair(1, 2)
来源：http://jka.shanyushiyangkeji.top

[T13] Kotlin：只读 Map
来源：http://qyh.aizwys.cn

val m = mapOf("a" to 1)
来源：http://xlc.sysykeji.top

[T14] Kotlin：循环
来源：http://kam.hongshengwenyu.top

for (i in 1..10) println(i)
来源：http://msb.hnqzz.top

[T15] Kotlin：接口
来源：http://dja.jyoumei.cn

interface Shape { fun area(): Double }
来源：http://vgz.shangyingyoupin.top

[T16] Swift：Hello World
来源：http://mcy.hywenlv.cn

print("Hello")
来源：http://wfm.zhaomingkeji.xyz

[T17] Swift：变量与常量
来源：http://wik.gotoacloud.top

var a = 1;  let b = 2
来源：http://cta.tarul.cn

[T18] Swift：字符串插值
来源：http://xwy.xingfuxueyuan.xyz

"值: \(b)"
来源：http://mfi.cashguo.top

[T19] Swift：可选绑定
来源：http://uwg.nanxinkj.top

if let n = opt { print(n) }
来源：http://zqf.snrcjt.cn

[T20] Swift：数组操作
来源：http://yjd.sxryk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://siq.cqqwz.cn

[T21] Swift：遍历
来源：http://cfc.fanxiaobao.xyz

for x in a { print(x) }
来源：http://kbd.ydzc1.top

[T22] Swift：字典
来源：http://ndt.xinyue.icu

var d = ["a": 1];  d["b"] = 2
来源：http://fys.ctjpmb.com

[T23] Swift：函数
来源：http://euc.havefunace.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zja.vqdsnc.cn

[T24] Swift：闭包
来源：http://zfj.hongshengwenyu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://hao.chenlongwang.top

[T25] Swift：结构体
来源：http://quz.nanxuanxn.top

struct P { var x: Int }
来源：http://agn.nanxuanxn.top

[T26] Swift：类与重写
来源：http://nzs.c1oappe.top

class A: Base { override func f() {} }
来源：http://smu.yonumen.top

[T27] Swift：错误处理
来源：http://lgx.zycfv.cn

do { try f() } catch { print(error) }
来源：http://wcw.gaohongyu789.top

[T28] Swift：枚举
来源：http://hzb.zhiwuduotai.top

enum Color { case red, green }
来源：http://yig.c1oappe.top

[T29] Swift：guard 提前返回
来源：http://wmz.ywan-chungtsiang.top

guard let x = opt else { return }
来源：http://ufb.tanke756.top

[T30] Swift：协议
来源：http://tbp.xingfuxueyuan.xyz

protocol Shape { func area() -> Double }
来源：http://ijb.chenlongwang.top

[T31] Lua：Hello World
来源：http://bmo.ywan-chungtsiang.top

print("Hello")
来源：http://vkw.yj20258888.top

[T32] Lua：局部变量
来源：http://bke.havefunace.top

local a = 1
来源：http://gzm.chenlongwang.top

[T33] Lua：表（数组）
来源：http://dpj.gotoacloud.top

local t = {1, 2, 3};  t[4] = 4
来源：http://yrq.hammf.cn

[T34] Lua：遍历表
来源：http://ovg.smart0.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://xcp.yj20258.top

[T35] Lua：字典表
来源：http://vbd.fktsv.cn

local d = { a = 1 };  d.b = 2
来源：http://pji.yfazqb.com

[T36] Lua：函数
来源：http://zeh.xylfe.cn

function add(a, b) return a + b end
来源：http://mog.cashguo.top

[T37] Lua：字符串拼接
来源：http://kxh.zdbjq.cn

"a" .. "b"
来源：http://drg.tianlin.xyz

[T38] Lua：条件
来源：http://wnd.aibaodan.cn

if x > 0 then print("正") end
来源：http://tkx.shuidangran.top


<!-- 参考信息 -->