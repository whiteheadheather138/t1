代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://amp.aibaodan.cn

[R36] 并发执行多个任务
来源：http://xpu.ydjk.org.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://srf.sysykeji.top

[R37] 把输出赋给变量
来源：http://nyn.fzhhl.top

files=$(ls -1)
来源：http://zjl.jlsjyb.cn

[R38] 管道串联
来源：http://nad.gzhubu.top

cat a.txt | grep -i error | wc -l
来源：http://ype.yuxming.cn

[R39] 重定向标准输出与错误
来源：http://sqc.fengsongda.top

cmd > out.log 2>&1
来源：http://tqs.shangyingyoupin.top

[R40] 追加写日志
来源：http://uth.redwolf501.top

echo "log" >> out.log
来源：http://osc.tanke756.top

[R41] 丢弃输出
来源：http://jzz.smart0.xyz

cmd >/dev/null 2>&1
来源：http://vvq.zhijiandao.cn

[R42] 输入重定向
来源：http://oql.ctjpmb.com

wc -l < a.txt
来源：http://rch.wangdashe.top

[R43] 按名字查找文件
来源：http://lpv.jiagoushi.top

find . -name "*.log" -type f
来源：http://nqm.kuanghao11.cn

[R44] 按修改时间查找
来源：http://qro.chenlongwang.top

find . -mtime -7 -type f
来源：http://ong.fengsongda.top

[R45] 批量删除
来源：http://apg.shanyushiyangkeji.top

find . -name "*.tmp" -delete
来源：http://nim.cheryme.top

[R46] 递归替换文件内容
来源：http://nyx.zhijiandao.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ctl.chenjidiqi.icu

[R47] sed 单行替换
来源：http://bln.zhiwuduotai.top

sed -i 's/foo/bar/g' a.txt
来源：http://tng.epnwcf.com

[R48] awk 取指定列
来源：http://jyx.dianchejie.cn

awk '{print $1, $3}' a.txt
来源：http://kfe.yangfankeji.com

[R49] awk 带条件
来源：http://tfd.xinyue.icu

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bgj.dianchejie.cn

[R50] awk 求和
来源：http://lve.ydzc1.top

awk '{s += $2} END {print s}' a.txt
来源：http://qfn.yueranfly.top

[R51] 排序去重取前几
来源：http://fyo.hcnkem.com

sort a.txt | uniq -c | sort -rn | head
来源：http://nsl.hysaishi.cn

[R52] 统计行数
来源：http://nwd.mhx1999.top

wc -l a.txt
来源：http://zwc.daxiang520.top

[R53] 查看文件头与实时尾
来源：http://jqm.daxiang520.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xvg.9152youxi.cn

[R54] 比较两个文件
来源：http://qov.snrcjt.cn

diff a.txt b.txt
来源：http://dfd.aizwys.cn

[R55] 压缩与解压
来源：http://oio.fktsv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hrm.jinghuilouyu.cn

[R56] 远程拷贝
来源：http://nzm.ehwqpu.com

scp file user@host:/path/
来源：http://edt.aizwys.cn

[R57] 远程执行命令
来源：http://cij.zhixingplan.top

ssh user@host 'uptime'
来源：http://xpm.jinyuanbaomall.cn

[R58] 下载文件
来源：http://mta.smart0.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ihi.mhx1999.top

[R59] 发 POST JSON
来源：http://nyh.316326.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://awt.nwbrower.top

[R60] 只看 HTTP 状态码
来源：http://ahm.tarul.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ahx.zhiwuduotai.top

[R61] 磁盘占用
来源：http://ptg.hysaishi.cn

df -h;  du -sh *
来源：http://lhd.jianghu66.top

[R62] 找最占空间的文件
来源：http://lwi.ehwqpu.com

du -ah . | sort -rh | head -10
来源：http://jtx.uphjek.com

[R63] 内存与进程
来源：http://wms.zhiwuduotai.top

free -h;  ps aux | grep nginx
来源：http://lvt.0kj1m.cn

[R64] 结束进程
来源：http://lwa.cashguo.top

kill -9 $(pgrep -f app.py)
来源：http://wga.wangshuangyany.cn

[R65] 查看端口占用
来源：http://ksb.vqdsnc.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pbq.xinyue.icu

[R66] 定时任务
来源：http://pid.zdbjq.cn

crontab -e;  crontab -l
来源：http://hnt.xuanzx.com

[R67] 生成随机十六进制串
来源：http://yvq.sjlbkw.cn

openssl rand -hex 16
来源：http://efm.cdnleiting.top

[R68] 计算文件校验值
来源：http://yqp.hywenlv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qxq.ydjk.org.cn

[R69] 生成随机密码
来源：http://dpm.hfpthk.cn

head -c 16 /dev/urandom | base64
来源：http://wfy.pengpengdd.cyou

[R70] 时间戳与互转
来源：http://jcn.dashuyun.cn

date +%s;  date -d @1700000000
来源：http://xdz.xylfe.cn

[R71] 日期格式化
来源：http://owj.cdnleiting.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://rui.yongpay.top

[R72] 等待端口就绪
来源：http://dsx.zhaomingkeji.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://pjx.zhoulong.xyz

[R73] 分割大日志
来源：http://fqp.vehdjk.com

split -l 1000 big.log part_
来源：http://zau.gogol.net.cn

[R74] 批量重命名
来源：http://chc.shangyingyoupin.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yra.shanyushiyangtech.top

[R75] 导出环境变量
来源：http://cyc.hcnkem.com

export PATH="$HOME/bin:$PATH"
来源：http://leh.yvedp.cn

[R76] 使用临时文件
来源：http://erw.xuanzx.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rlo.guannengcc.top

[R77] 读取用户输入
来源：http://eau.xingfuxueyuan.xyz

read -rp "请输入: " ans
来源：http://nza.nanxinkj.top

[R78] 交互式菜单
来源：http://tdy.c1oappe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://czv.ywan-chungtsiang.top

[R79] 解析命令行选项
来源：http://tgi.guowangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rri.jqgfzy.top

[R80] 查看脚本执行耗时
来源：http://tot.jlsjyb.cn

time ./run.sh
来源：http://hxb.0kj1m.cn

================================================================================
来源：http://yta.zhongyouzk.top

S. C / C++ 专题
来源：http://fgr.jianghu66.top

================================================================================
来源：http://txu.hongshengwenyu.top

[S01] C：Hello World
来源：http://muo.zhongyouzk.top

#include <stdio.h>
来源：http://frx.zycfv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sgk.hywenlv.cn

[S02] C：变量与格式化输出
来源：http://qqt.xziqi.cn

int a = 10; printf("%d\n", a);
来源：http://xsu.vqdsnc.cn

[S03] C：读入整数
来源：http://ulo.svipenyu.cn

int x; scanf("%d", &x);
来源：http://mvg.aizwys.cn

[S04] C：字符串复制
来源：http://nqy.cashguo.top

char dst[32]; strcpy(dst, "hi");
来源：http://awh.nwbrower.top

[S05] C：字符串长度
来源：http://fnu.hcnkem.com

strlen(s)
来源：http://hzj.ivvv.top

[S06] C：字符串比较
来源：http://ysg.redwolf501.top

strcmp(a, b) == 0
来源：http://ogy.jinghuilouyu.cn

[S07] C：数组遍历求和
来源：http://als.daria6918.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mnc.hywenlv.cn

[S08] C：动态内存分配与释放
来源：http://yxh.52xcode.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qte.shanyushiyangtech.top

[S09] C：结构体定义与初始化
来源：http://dmx.yuanzhike.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ncr.wangdashe.top

[S10] C：指针与解引用
来源：http://eoi.9152youxi.cn

int *p = &a;  *p = 5;
来源：http://twx.haohaochexian.top

[S11] C：逐行读文件
来源：http://lgo.jqgfzy.top

FILE *f = fopen("a.txt", "r");
来源：http://nrq.hywenlv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zrt.xylfe.cn

fclose(f);
来源：http://tpf.shangyingyoupin.top

[S12] C：写文件
来源：http://qof.jqgufenzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://owa.gaohongyu789.top

[S13] C：宏定义
来源：http://hbz.shangyingyoupin.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qxr.guannengcc.top

[S14] C：枚举
来源：http://rnd.jianghu66.top

enum Color { RED, GREEN, BLUE };
来源：http://hvc.dashuyun.cn

[S15] C：类型转换
来源：http://sxn.yvedp.cn

(double) a / b
来源：http://wth.tanke756.top

[S16] C：位操作置位
来源：http://enw.wangdashe.top

x |= (1 << 3);
来源：http://hzv.bjfxy.top

[S17] C：安全拼接字符串
来源：http://bgz.zhongyouzk.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cwj.havefunace.top

[S18] C：命令行参数
来源：http://cig.ybcxt.top

int main(int argc, char **argv)
来源：http://voa.jinqigufen.top

[S19] C：快速排序
来源：http://uyv.shzxlz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://iro.guannengcc.top

[S20] C：二分查找
来源：http://dxu.yj20258888.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rsw.cqqwz.cn

[S21] C：字符类别判断
来源：http://wib.jqgfzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://btn.andypj.xyz

[S22] C：字符串转数字
来源：http://knq.jlsjyb.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ezm.hcnkem.com

[S23] C：随机数
来源：http://mck.jqgfzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://exa.316326.xyz

[S24] C：获取本地时间
来源：http://arm.cashguo.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lvl.epnwcf.com

[S25] C：内存拷贝
来源：http://ksc.0kj1m.cn

memcpy(dst, src, n);
来源：http://vxf.vqdsnc.cn

[S26] C：内存清零
来源：http://xsw.yuxming.cn

memset(a, 0, sizeof a);
来源：http://gjz.hesvh.cn

[S27] C：定义常量
来源：http://bpb.xuetiantiany.cn

const double PI = 3.14159;
来源：http://ifn.haohaochexian.top

[S28] C：静态变量
来源：http://qnf.sufxvd.cn

static int counter = 0;
来源：http://bru.zhoulong.xyz

[S29] C：变参函数
来源：http://ppy.wangshuangyany.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ofj.hammf.cn

[S30] C：头文件保护
来源：http://lnr.zdbjq.cn

#ifndef X_H
来源：http://tja.cdnleiting.top

#define X_H
来源：http://law.birdmap.top

#endif
来源：http://jfn.jinyuanbaomall.cn

[S31] C++：Hello World
来源：http://iil.zhoulong.xyz

#include <iostream>
来源：http://lxb.epnwcf.com

int main() { std::cout << "Hello\n"; }
来源：http://trn.smart0.xyz

[S32] C++：字符串
来源：http://lqc.zdqjudy.top

std::string s = "hi";  s += "!";
来源：http://yfs.hywenlv.cn

[S33] C++：vector 增删
来源：http://frr.yanxiufei.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hzl.yj20258.top

[S34] C++：遍历 vector
来源：http://qai.gzhubu.top

for (auto &x : v) { std::cout << x; }
来源：http://syj.aizwys.cn

[S35] C++：map
来源：http://dea.c1oappe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qrm.jinqigufen.top

[S36] C++：unordered_map
来源：http://bwy.cdnleiting.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dzr.chenjidiqi.icu

[S37] C++：set
来源：http://gns.cdnleiting.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cuv.ehwqpu.com

[S38] C++：排序
来源：http://age.xuetiantiany.cn

std::sort(v.begin(), v.end());
来源：http://dcu.fanxiaobao.xyz

[S39] C++：自定义比较器排序
来源：http://bap.ywan-chungtsiang.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aup.ivvv.top

[S40] C++：查找元素
来源：http://ouh.jianghu66.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://akn.yangfankeji.com

[S41] C++：类与构造函数
来源：http://mhe.cqqwz.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nie.birdmap.top

[S42] C++：继承与虚函数
来源：http://rrr.yueranfly.top

class B : public Base { public: void f() override {} };
来源：http://ixl.hywenlv.cn

[S43] C++：智能指针
来源：http://knl.jiagoushi.top

auto p = std::make_unique<int>(5);
来源：http://cbn.feifeiyinyue.top

[S44] C++：引用传参
来源：http://vik.gogol.net.cn

void inc(int &x) { ++x; }
来源：http://dup.fengsongda.top

[S45] C++：lambda
来源：http://ple.yangfankeji.com

auto add = [](int a, int b) { return a + b; };
来源：http://lfl.sufxvd.cn

[S46] C++：函数模板
来源：http://aht.zhongyouzk.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rkj.zycfv.cn

[S47] C++：结构化绑定遍历
来源：http://thr.wangdashe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://psm.zhaomingkeji.xyz

[S48] C++：逐行读文件
来源：http://tbd.xuanzx.com

std::ifstream in("a.txt");  std::string line;
来源：http://glw.zhengqikj.top

while (std::getline(in, line)) { }
来源：http://eyo.yuanzhike.top

[S49] C++：写文件
来源：http://njf.zhijiandao.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://glu.ybcxt.top

[S50] C++：格式化数字
来源：http://yud.aizwys.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ihe.svipenyu.cn

[S51] C++：显式类型转换
来源：http://ukd.hnxiangtu.top

static_cast<double>(a) / b
来源：http://gxc.redwolf501.top

[S52] C++：const 与 noexcept
来源：http://tno.tarul.cn

int size() const noexcept { return n_; }
来源：http://btf.jlsjyb.cn

[S53] C++：移动语义
来源：http://sdc.jqgufenzy.top

std::vector<int> w = std::move(v);
来源：http://snd.xuetiantiany.cn

[S54] C++：异常处理
来源：http://wao.shanyushiyangkeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kwk.zhengqikj.top

[S55] C++：结构化绑定
来源：http://ewk.quarkkingdee.top

auto [a, b] = std::make_pair(1, 2);
来源：http://cos.fehbvm.com

[S56] C++：optional
来源：http://jui.ivvv.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bgv.hongshengwenyu.top

[S57] C++：编译期常量
来源：http://fhi.zhongyouzk.top

constexpr int N = 10;
来源：http://ncq.nanxuanxn.top

[S58] C++：命名空间
来源：http://kkx.316326.xyz

namespace ns { int f() { return 1; } }
来源：http://iuv.ehwqpu.com

[S59] C++：静态断言
来源：http://ozx.vehdjk.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fos.gaohongyu789.top

[S60] C++：遍历并删除元素
来源：http://han.havefunace.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zzw.316326.xyz

================================================================================
来源：http://yki.yanxiufei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xqr.jiagoushi.top

================================================================================
来源：http://tay.nwbrower.top

[T01] Kotlin：Hello World
来源：http://vtb.ywan-chungtsiang.top

println("Hello")
来源：http://usq.tarul.cn

[T02] Kotlin：变量
来源：http://mci.quarkkingdee.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://stq.yongpay.top

[T03] Kotlin：字符串模板
来源：http://ita.jinqigufen.top

"值: $b"
来源：http://cyi.yanxiufei.cn

[T04] Kotlin：空安全
来源：http://qbi.meibo888.top

val n: String? = null;  n?.length
来源：http://xbi.jianghu66.top

[T05] Kotlin：when 表达式
来源：http://dxa.shanyushiyangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xrf.pengpengdd.cyou

[T06] Kotlin：集合映射
来源：http://ram.daxiang520.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qvw.tarul.cn

[T07] Kotlin：集合过滤
来源：http://dcx.ywan-chungtsiang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rxz.jianghu66.top

[T08] Kotlin：数据类
来源：http://fqj.jqgufenzy.top

data class User(val name: String, val age: Int)
来源：http://cwq.zdbjq.cn

[T09] Kotlin：扩展函数
来源：http://qkc.shanyushiyangtech.top

fun String.exclaim() = this + "!"
来源：http://nzp.mhx1999.top

[T10] Kotlin：默认参数
来源：http://ynv.xinyue.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://zql.sysykeji.top

[T11] Kotlin：协程
来源：http://vdc.ydjk.org.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xyi.jinqigfzy.top

[T12] Kotlin：解构声明
来源：http://qjy.daxiang520.top

val (a, b) = Pair(1, 2)
来源：http://fvv.zhijiandao.cn

[T13] Kotlin：只读 Map
来源：http://tti.kuanghao11.cn

val m = mapOf("a" to 1)
来源：http://zdx.jiagoushi.top

[T14] Kotlin：循环
来源：http://bxj.aizwys.cn

for (i in 1..10) println(i)
来源：http://tch.yongpay.top

[T15] Kotlin：接口
来源：http://lck.xuanzx.com

interface Shape { fun area(): Double }
来源：http://qkp.fehbvm.com

[T16] Swift：Hello World
来源：http://xdy.redwolf501.top

print("Hello")
来源：http://qvx.epnwcf.com

[T17] Swift：变量与常量
来源：http://mbr.xuanzx.com

var a = 1;  let b = 2
来源：http://gqn.andypj.xyz

[T18] Swift：字符串插值
来源：http://mat.feifeiyinyue.top

"值: \(b)"
来源：http://cte.bbcook.cn

[T19] Swift：可选绑定
来源：http://mez.meibo888.top

if let n = opt { print(n) }
来源：http://wmi.sxryk.cn

[T20] Swift：数组操作
来源：http://orb.gogol.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://oxz.shuidangran.top

[T21] Swift：遍历
来源：http://jep.jqgufenzy.top

for x in a { print(x) }
来源：http://bnx.jlsjyb.cn

[T22] Swift：字典
来源：http://ynd.pengpengdd.cyou

var d = ["a": 1];  d["b"] = 2
来源：http://ilp.zdbjq.cn

[T23] Swift：函数
来源：http://iga.cashguo.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://paz.yonumen.top

[T24] Swift：闭包
来源：http://kri.tanke756.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://yib.yanxiufei.cn

[T25] Swift：结构体
来源：http://ogh.zycfv.cn

struct P { var x: Int }
来源：http://vql.hfpthk.cn

[T26] Swift：类与重写
来源：http://elk.yanxiufei.cn

class A: Base { override func f() {} }
来源：http://hif.yj20258888.top

[T27] Swift：错误处理
来源：http://ket.316326.xyz

do { try f() } catch { print(error) }
来源：http://qgi.hesvh.cn

[T28] Swift：枚举
来源：http://qcq.shangyingyoupin.top

enum Color { case red, green }
来源：http://jog.mhx1999.top

[T29] Swift：guard 提前返回
来源：http://xma.guowangkeji.top

guard let x = opt else { return }
来源：http://hxn.nanxinkj.top

[T30] Swift：协议
来源：http://xaj.jianghu66.top

protocol Shape { func area() -> Double }
来源：http://cll.cashguo.top

[T31] Lua：Hello World
来源：http://qdp.fanxiaobao.xyz

print("Hello")
来源：http://uky.chenjidiqi.icu

[T32] Lua：局部变量
来源：http://xkf.cashguo.top

local a = 1
来源：http://ife.ybcxt.top

[T33] Lua：表（数组）
来源：http://jet.zhiwuduotai.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ntk.jyoumei.cn

[T34] Lua：遍历表
来源：http://rrd.yueranfly.top

for i, v in ipairs(t) do print(i, v) end
来源：http://yki.chenjidiqi.icu

[T35] Lua：字典表
来源：http://qzl.ehwqpu.com

local d = { a = 1 };  d.b = 2
来源：http://rxs.jinqigfzy.top

[T36] Lua：函数
来源：http://rak.jqgfzy.top

function add(a, b) return a + b end
来源：http://hrr.cashguo.top

[T37] Lua：字符串拼接
来源：http://hqu.gzhubu.top

"a" .. "b"
来源：http://rat.zycfv.cn

[T38] Lua：条件
来源：http://pwu.sufxvd.cn

if x > 0 then print("正") end
来源：http://fct.vehdjk.com


<!-- 参考信息 -->