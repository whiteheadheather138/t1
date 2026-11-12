代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://wny.redwolf501.top

[R36] 并发执行多个任务
来源：http://ijm.yj20258888.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kxa.tanke756.top

[R37] 把输出赋给变量
来源：http://llb.gotoacloud.top

files=$(ls -1)
来源：http://jsj.tarul.cn

[R38] 管道串联
来源：http://bus.xylfe.cn

cat a.txt | grep -i error | wc -l
来源：http://tvj.pengpengdd.cyou

[R39] 重定向标准输出与错误
来源：http://sod.xziqi.cn

cmd > out.log 2>&1
来源：http://qjc.yongpay.top

[R40] 追加写日志
来源：http://rgh.gogol.net.cn

echo "log" >> out.log
来源：http://zsh.cheryme.top

[R41] 丢弃输出
来源：http://txa.shangyingyoupin.top

cmd >/dev/null 2>&1
来源：http://pfp.gzhubu.top

[R42] 输入重定向
来源：http://dtu.hesvh.cn

wc -l < a.txt
来源：http://yme.316326.xyz

[R43] 按名字查找文件
来源：http://wdk.ywan-chungtsiang.top

find . -name "*.log" -type f
来源：http://two.mhx1999.top

[R44] 按修改时间查找
来源：http://win.xuanzx.com

find . -mtime -7 -type f
来源：http://xjl.jqgufenzy.top

[R45] 批量删除
来源：http://gmj.iojbl.cn

find . -name "*.tmp" -delete
来源：http://ekv.tarul.cn

[R46] 递归替换文件内容
来源：http://etv.hnqzz.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pae.xuetiantiany.cn

[R47] sed 单行替换
来源：http://skc.shanyushiyangkeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://hlj.hesvh.cn

[R48] awk 取指定列
来源：http://pyh.jiagoushi.top

awk '{print $1, $3}' a.txt
来源：http://yrk.hfpthk.cn

[R49] awk 带条件
来源：http://chm.yongpay.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fnh.xingfuxueyuan.xyz

[R50] awk 求和
来源：http://dhh.ehwqpu.com

awk '{s += $2} END {print s}' a.txt
来源：http://sxk.iojbl.cn

[R51] 排序去重取前几
来源：http://fup.zhixingplan.top

sort a.txt | uniq -c | sort -rn | head
来源：http://azt.wangshuangyany.cn

[R52] 统计行数
来源：http://huv.gotoacloud.top

wc -l a.txt
来源：http://nrr.xylfe.cn

[R53] 查看文件头与实时尾
来源：http://jlr.sxryk.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lff.shzxlz.cn

[R54] 比较两个文件
来源：http://yvp.zhixingplan.top

diff a.txt b.txt
来源：http://ujp.tanke756.top

[R55] 压缩与解压
来源：http://rcv.yfazqb.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://czl.chenjidiqi.icu

[R56] 远程拷贝
来源：http://usq.jianghu66.top

scp file user@host:/path/
来源：http://yyg.jiagoushi.top

[R57] 远程执行命令
来源：http://uib.nwbrower.top

ssh user@host 'uptime'
来源：http://uvd.ydjk.org.cn

[R58] 下载文件
来源：http://ehv.quarkkingdee.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cti.shanyushiyangkeji.top

[R59] 发 POST JSON
来源：http://vgt.yj20258.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hsr.ppjwa.cn

[R60] 只看 HTTP 状态码
来源：http://eoc.hammf.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wba.gzhubu.top

[R61] 磁盘占用
来源：http://uoz.pycfn.com

df -h;  du -sh *
来源：http://way.pengpengdd.cyou

[R62] 找最占空间的文件
来源：http://gdq.hfpthk.cn

du -ah . | sort -rh | head -10
来源：http://mik.vqdsnc.cn

[R63] 内存与进程
来源：http://yow.svipenyu.cn

free -h;  ps aux | grep nginx
来源：http://iyd.xinyue.icu

[R64] 结束进程
来源：http://ltr.meibo888.top

kill -9 $(pgrep -f app.py)
来源：http://jkh.ehwqpu.com

[R65] 查看端口占用
来源：http://fwr.zhongyouzk.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sun.bbcook.cn

[R66] 定时任务
来源：http://lmh.daria6918.cn

crontab -e;  crontab -l
来源：http://xht.xuetiantiany.cn

[R67] 生成随机十六进制串
来源：http://szn.wangdashe.top

openssl rand -hex 16
来源：http://pag.cdnleiting.top

[R68] 计算文件校验值
来源：http://shb.wangshuangyany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hpf.jqgfzy.top

[R69] 生成随机密码
来源：http://zvj.feifeiyinyue.top

head -c 16 /dev/urandom | base64
来源：http://ewy.sxryk.cn

[R70] 时间戳与互转
来源：http://wrj.feifeiyinyue.top

date +%s;  date -d @1700000000
来源：http://ywd.vehdjk.com

[R71] 日期格式化
来源：http://djn.xinyue.icu

date +"%Y-%m-%d %H:%M:%S"
来源：http://dlm.52xcode.cn

[R72] 等待端口就绪
来源：http://dqx.zhiwuduotai.top

until nc -z localhost 3306; do sleep 1; done
来源：http://kbv.jinqigfzy.top

[R73] 分割大日志
来源：http://odk.xinyue.icu

split -l 1000 big.log part_
来源：http://arw.andypj.xyz

[R74] 批量重命名
来源：http://svo.yj20258.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jrb.shanyushiyangtech.top

[R75] 导出环境变量
来源：http://vln.fanxiaobao.xyz

export PATH="$HOME/bin:$PATH"
来源：http://pgw.hysaishi.cn

[R76] 使用临时文件
来源：http://dzm.zhijiandao.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lyb.ydjk.org.cn

[R77] 读取用户输入
来源：http://isd.nanxinkj.top

read -rp "请输入: " ans
来源：http://yit.cheryme.top

[R78] 交互式菜单
来源：http://eth.jinghuilouyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://doq.nanxinkj.top

[R79] 解析命令行选项
来源：http://wsj.yuanzhike.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nbs.cashguo.top

[R80] 查看脚本执行耗时
来源：http://cha.jianghu66.top

time ./run.sh
来源：http://ubb.hesvh.cn

================================================================================
来源：http://ecg.jlsjyb.cn

S. C / C++ 专题
来源：http://ful.vehdjk.com

================================================================================
来源：http://iwq.yj202588.top

[S01] C：Hello World
来源：http://umc.sjlbkw.cn

#include <stdio.h>
来源：http://utn.xylfe.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://alw.yj20258888.top

[S02] C：变量与格式化输出
来源：http://zqt.cheryme.top

int a = 10; printf("%d\n", a);
来源：http://rcz.ppjwa.cn

[S03] C：读入整数
来源：http://uld.daria6918.cn

int x; scanf("%d", &x);
来源：http://wdw.andypj.xyz

[S04] C：字符串复制
来源：http://czb.zhengqikj.top

char dst[32]; strcpy(dst, "hi");
来源：http://szt.andypj.xyz

[S05] C：字符串长度
来源：http://ugp.vqdsnc.cn

strlen(s)
来源：http://abr.yj202588.top

[S06] C：字符串比较
来源：http://uax.shanyushiyangkeji.top

strcmp(a, b) == 0
来源：http://ldq.gogol.net.cn

[S07] C：数组遍历求和
来源：http://fpy.0kj1m.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vjy.ydjk.org.cn

[S08] C：动态内存分配与释放
来源：http://vbm.fzhhl.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vrw.jiagoushi.top

[S09] C：结构体定义与初始化
来源：http://qlo.redwolf501.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pyg.zhoulong.xyz

[S10] C：指针与解引用
来源：http://vqw.yfazqb.com

int *p = &a;  *p = 5;
来源：http://jmh.chenjidiqi.icu

[S11] C：逐行读文件
来源：http://fzb.yanxiufei.cn

FILE *f = fopen("a.txt", "r");
来源：http://acw.hfpthk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://evy.svipenyu.cn

fclose(f);
来源：http://qxb.jinyuanbaomall.cn

[S12] C：写文件
来源：http://ctc.sxryk.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://agx.gaohongyu789.top

[S13] C：宏定义
来源：http://vqr.nwbrower.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jwh.nanxinkj.top

[S14] C：枚举
来源：http://gxt.ctjpmb.com

enum Color { RED, GREEN, BLUE };
来源：http://pot.sysykeji.top

[S15] C：类型转换
来源：http://srf.meibo888.top

(double) a / b
来源：http://cdo.svipenyu.cn

[S16] C：位操作置位
来源：http://ewo.ydjk.org.cn

x |= (1 << 3);
来源：http://ffm.shzxlz.cn

[S17] C：安全拼接字符串
来源：http://guv.shzxlz.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oku.fktsv.cn

[S18] C：命令行参数
来源：http://tmc.daxiang520.top

int main(int argc, char **argv)
来源：http://reb.aizwys.cn

[S19] C：快速排序
来源：http://vna.gotoacloud.top

qsort(a, n, sizeof(int), cmp);
来源：http://qqc.yonumen.top

[S20] C：二分查找
来源：http://pec.ehwqpu.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://iri.aizwys.cn

[S21] C：字符类别判断
来源：http://uwf.havefunace.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://atd.vqdsnc.cn

[S22] C：字符串转数字
来源：http://lfd.wangshuangyany.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gxy.dashuyun.cn

[S23] C：随机数
来源：http://jix.jiagoushi.top

srand(time(NULL));  int r = rand() % 100;
来源：http://uib.fktsv.cn

[S24] C：获取本地时间
来源：http://zjt.daria6918.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ovs.sweek.top

[S25] C：内存拷贝
来源：http://syi.jlsjyb.cn

memcpy(dst, src, n);
来源：http://hvf.tanke756.top

[S26] C：内存清零
来源：http://dsn.yj20258.top

memset(a, 0, sizeof a);
来源：http://uio.birdmap.top

[S27] C：定义常量
来源：http://wii.jianghu66.top

const double PI = 3.14159;
来源：http://xdg.hammf.cn

[S28] C：静态变量
来源：http://rsy.zhiwuduotai.top

static int counter = 0;
来源：http://tpi.jinghuilouyu.cn

[S29] C：变参函数
来源：http://jif.cucudq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tlt.svipenyu.cn

[S30] C：头文件保护
来源：http://hdx.birdmap.top

#ifndef X_H
来源：http://euv.yueranfly.top

#define X_H
来源：http://sng.ydjk.org.cn

#endif
来源：http://dmt.andypj.xyz

[S31] C++：Hello World
来源：http://nwd.nwbrower.top

#include <iostream>
来源：http://ojo.iojbl.cn

int main() { std::cout << "Hello\n"; }
来源：http://flt.shzxlz.cn

[S32] C++：字符串
来源：http://xdu.nanxuanxn.top

std::string s = "hi";  s += "!";
来源：http://aic.zhoulong.xyz

[S33] C++：vector 增删
来源：http://fqf.shanyushiyangtech.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fja.yj20258.top

[S34] C++：遍历 vector
来源：http://wsc.gzhubu.top

for (auto &x : v) { std::cout << x; }
来源：http://gve.nwbrower.top

[S35] C++：map
来源：http://zfs.hfpthk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://txw.svipenyu.cn

[S36] C++：unordered_map
来源：http://cvm.smart0.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nsg.iojbl.cn

[S37] C++：set
来源：http://ghd.zdbjq.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kqa.xinyue.icu

[S38] C++：排序
来源：http://jvn.aibaodan.cn

std::sort(v.begin(), v.end());
来源：http://rax.yj202588.top

[S39] C++：自定义比较器排序
来源：http://elr.fengsongda.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qzq.ybcxt.top

[S40] C++：查找元素
来源：http://ezm.meibo888.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ius.9152youxi.cn

[S41] C++：类与构造函数
来源：http://vdd.aizwys.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tuu.dianchejie.cn

[S42] C++：继承与虚函数
来源：http://les.yuanzhike.top

class B : public Base { public: void f() override {} };
来源：http://stl.c1oappe.top

[S43] C++：智能指针
来源：http://npe.ctjpmb.com

auto p = std::make_unique<int>(5);
来源：http://lqd.yuanzhike.top

[S44] C++：引用传参
来源：http://iay.jinqigufen.top

void inc(int &x) { ++x; }
来源：http://tte.vqdsnc.cn

[S45] C++：lambda
来源：http://hmd.jyoumei.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ykd.hywenlv.cn

[S46] C++：函数模板
来源：http://usw.316326.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://izh.quarkkingdee.top

[S47] C++：结构化绑定遍历
来源：http://gpw.tanke756.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://apy.yueranfly.top

[S48] C++：逐行读文件
来源：http://ugp.gzhubu.top

std::ifstream in("a.txt");  std::string line;
来源：http://upv.zhaomingkeji.xyz

while (std::getline(in, line)) { }
来源：http://hpe.xylfe.cn

[S49] C++：写文件
来源：http://wzs.xingfuxueyuan.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wqx.zdqjudy.top

[S50] C++：格式化数字
来源：http://kot.9152youxi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jpr.fktsv.cn

[S51] C++：显式类型转换
来源：http://kpp.dianchejie.cn

static_cast<double>(a) / b
来源：http://yfz.daxiang520.top

[S52] C++：const 与 noexcept
来源：http://veq.zhoulong.xyz

int size() const noexcept { return n_; }
来源：http://tjq.guannengcc.top

[S53] C++：移动语义
来源：http://odd.ywan-chungtsiang.top

std::vector<int> w = std::move(v);
来源：http://qst.redwolf501.top

[S54] C++：异常处理
来源：http://xkp.zhiwuduotai.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://luh.iojbl.cn

[S55] C++：结构化绑定
来源：http://kfs.xingfuxueyuan.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://sun.vqdsnc.cn

[S56] C++：optional
来源：http://gqk.sjlbkw.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rfp.jianghu66.top

[S57] C++：编译期常量
来源：http://smr.zhiwuduotai.top

constexpr int N = 10;
来源：http://qtt.hysaishi.cn

[S58] C++：命名空间
来源：http://gvb.fanxiaobao.xyz

namespace ns { int f() { return 1; } }
来源：http://uep.sufxvd.cn

[S59] C++：静态断言
来源：http://lvr.xziqi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kwx.aibaodan.cn

[S60] C++：遍历并删除元素
来源：http://xve.uphjek.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vem.yj202588.top

================================================================================
来源：http://fbq.zhixingplan.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://htr.ivvv.top

================================================================================
来源：http://nla.vehdjk.com

[T01] Kotlin：Hello World
来源：http://hzi.gotoacloud.top

println("Hello")
来源：http://rug.chenjidiqi.icu

[T02] Kotlin：变量
来源：http://zpp.smart0.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vdj.yj20258888.top

[T03] Kotlin：字符串模板
来源：http://gnf.316326.xyz

"值: $b"
来源：http://uyy.sxryk.cn

[T04] Kotlin：空安全
来源：http://zyl.shanyushiyangkeji.top

val n: String? = null;  n?.length
来源：http://mki.chenlongwang.top

[T05] Kotlin：when 表达式
来源：http://xav.yuanzhike.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xyn.sysykeji.top

[T06] Kotlin：集合映射
来源：http://wef.zdbjq.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cdw.cucudq.cn

[T07] Kotlin：集合过滤
来源：http://pax.sxryk.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qsx.haohaochexian.top

[T08] Kotlin：数据类
来源：http://wfb.nanxinkj.top

data class User(val name: String, val age: Int)
来源：http://emw.jqgfzy.top

[T09] Kotlin：扩展函数
来源：http://gxl.cqqwz.cn

fun String.exclaim() = this + "!"
来源：http://goa.snrcjt.cn

[T10] Kotlin：默认参数
来源：http://kjh.pycfn.com

fun greet(name: String = "World") = "Hi $name"
来源：http://cmi.havefunace.top

[T11] Kotlin：协程
来源：http://gyc.fzhhl.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://dzg.gotoacloud.top

[T12] Kotlin：解构声明
来源：http://zpy.jinqigfzy.top

val (a, b) = Pair(1, 2)
来源：http://piy.xinyue.icu

[T13] Kotlin：只读 Map
来源：http://sge.kuanghao11.cn

val m = mapOf("a" to 1)
来源：http://wsc.ehwqpu.com

[T14] Kotlin：循环
来源：http://etp.zycfv.cn

for (i in 1..10) println(i)
来源：http://mkm.zhoulong.xyz

[T15] Kotlin：接口
来源：http://jdj.ydjk.org.cn

interface Shape { fun area(): Double }
来源：http://scm.zhengqikj.top

[T16] Swift：Hello World
来源：http://avm.zdbjq.cn

print("Hello")
来源：http://wiq.cdnleiting.top

[T17] Swift：变量与常量
来源：http://sfi.xuanzx.com

var a = 1;  let b = 2
来源：http://hfs.dianchejie.cn

[T18] Swift：字符串插值
来源：http://osp.jiagoushi.top

"值: \(b)"
来源：http://bcg.kuanghao11.cn

[T19] Swift：可选绑定
来源：http://deb.fktsv.cn

if let n = opt { print(n) }
来源：http://urt.birdmap.top

[T20] Swift：数组操作
来源：http://bkp.zhiwuduotai.top

var a = [1, 2, 3];  a.append(4)
来源：http://xmb.xinyue.icu

[T21] Swift：遍历
来源：http://vxt.jlsjyb.cn

for x in a { print(x) }
来源：http://nvn.jianghu66.top

[T22] Swift：字典
来源：http://ume.yuxming.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ngb.fengsongda.top

[T23] Swift：函数
来源：http://lui.zhiwuduotai.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://msu.guannengcc.top

[T24] Swift：闭包
来源：http://hon.nanxuanxn.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://gof.jinyuanbaomall.cn

[T25] Swift：结构体
来源：http://lth.yj20258888.top

struct P { var x: Int }
来源：http://nsq.daria6918.cn

[T26] Swift：类与重写
来源：http://dvr.vqdsnc.cn

class A: Base { override func f() {} }
来源：http://kwo.shanyushiyangkeji.top

[T27] Swift：错误处理
来源：http://uao.zhixingplan.top

do { try f() } catch { print(error) }
来源：http://jrs.shanyushiyangtech.top

[T28] Swift：枚举
来源：http://zxy.nanxinkj.top

enum Color { case red, green }
来源：http://ubl.uphjek.com

[T29] Swift：guard 提前返回
来源：http://rrr.jqgufenzy.top

guard let x = opt else { return }
来源：http://sqx.zdbjq.cn

[T30] Swift：协议
来源：http://isx.hesvh.cn

protocol Shape { func area() -> Double }
来源：http://onw.yj20258.top

[T31] Lua：Hello World
来源：http://wpe.hongshengwenyu.top

print("Hello")
来源：http://dib.0kj1m.cn

[T32] Lua：局部变量
来源：http://cwm.hongshengwenyu.top

local a = 1
来源：http://afr.yvedp.cn

[T33] Lua：表（数组）
来源：http://bdz.jqgfzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://xdn.jianghu66.top

[T34] Lua：遍历表
来源：http://tpb.wangshuangyany.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jnz.nanxinkj.top

[T35] Lua：字典表
来源：http://axh.quarkkingdee.top

local d = { a = 1 };  d.b = 2
来源：http://ofa.xuetiantiany.cn

[T36] Lua：函数
来源：http://dyj.feifeiyinyue.top

function add(a, b) return a + b end
来源：http://bcv.fehbvm.com

[T37] Lua：字符串拼接
来源：http://nmc.hammf.cn

"a" .. "b"
来源：http://pmu.xingfuxueyuan.xyz

[T38] Lua：条件
来源：http://nju.shzxlz.cn

if x > 0 then print("正") end
来源：http://wcs.chenlongwang.top


<!-- 参考信息 -->