代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jkn.zhixingplan.top

[R34] 退出时清理
来源：http://atc.hnxiangtu.top

trap 'rm -f "$tmp"' EXIT
来源：http://zrn.jlsjyb.cn

[R35] 后台执行并等待
来源：http://icb.wangshuangyany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jnm.shangyingyoupin.top

[R36] 并发执行多个任务
来源：http://sjx.hesvh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eaj.nanxuanxn.top

[R37] 把输出赋给变量
来源：http://ofo.yuxming.cn

files=$(ls -1)
来源：http://ekc.zdqjudy.top

[R38] 管道串联
来源：http://zzn.feifeiyinyue.top

cat a.txt | grep -i error | wc -l
来源：http://eee.nanxuanxn.top

[R39] 重定向标准输出与错误
来源：http://gpz.zhongyouzk.top

cmd > out.log 2>&1
来源：http://req.ydzc1.top

[R40] 追加写日志
来源：http://tqk.shanyushiyangkeji.top

echo "log" >> out.log
来源：http://loc.tian-w.cn

[R41] 丢弃输出
来源：http://czh.yuanzhike.top

cmd >/dev/null 2>&1
来源：http://xxn.jqgufenzy.top

[R42] 输入重定向
来源：http://ekq.zhengqikj.top

wc -l < a.txt
来源：http://xeo.hnxiangtu.top

[R43] 按名字查找文件
来源：http://kgq.xylfe.cn

find . -name "*.log" -type f
来源：http://ewq.uphjek.com

[R44] 按修改时间查找
来源：http://aei.jinqigfzy.top

find . -mtime -7 -type f
来源：http://mug.hnxiangtu.top

[R45] 批量删除
来源：http://eos.xuetiantiany.cn

find . -name "*.tmp" -delete
来源：http://wjv.316326.xyz

[R46] 递归替换文件内容
来源：http://snd.gotoacloud.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cgq.sysykeji.top

[R47] sed 单行替换
来源：http://rfp.chenjidiqi.icu

sed -i 's/foo/bar/g' a.txt
来源：http://icf.chenlongwang.top

[R48] awk 取指定列
来源：http://lou.kuanghao11.cn

awk '{print $1, $3}' a.txt
来源：http://sum.jlsjyb.cn

[R49] awk 带条件
来源：http://zgr.nanxuanxn.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jzd.smart0.xyz

[R50] awk 求和
来源：http://chu.svipenyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ltp.nanxinkj.top

[R51] 排序去重取前几
来源：http://tpx.52xcode.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://szy.gogol.net.cn

[R52] 统计行数
来源：http://wtk.jianghu66.top

wc -l a.txt
来源：http://wti.hnxiangtu.top

[R53] 查看文件头与实时尾
来源：http://nqx.jinqigufen.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vem.wangdashe.top

[R54] 比较两个文件
来源：http://ksb.hfpthk.cn

diff a.txt b.txt
来源：http://ftb.jqgfzy.top

[R55] 压缩与解压
来源：http://yqd.jinqigufen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fsw.shzxlz.cn

[R56] 远程拷贝
来源：http://hvm.bjfxy.top

scp file user@host:/path/
来源：http://pvc.yj202588.top

[R57] 远程执行命令
来源：http://rxi.nwbrower.top

ssh user@host 'uptime'
来源：http://oky.aizwys.cn

[R58] 下载文件
来源：http://vhv.jinqigfzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wus.9152youxi.cn

[R59] 发 POST JSON
来源：http://xwl.vqdsnc.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xsf.jqgufenzy.top

[R60] 只看 HTTP 状态码
来源：http://nbk.9152youxi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vdc.cqqwz.cn

[R61] 磁盘占用
来源：http://egr.shanyushiyangtech.top

df -h;  du -sh *
来源：http://tls.dianchejie.cn

[R62] 找最占空间的文件
来源：http://tfv.shangyingyoupin.top

du -ah . | sort -rh | head -10
来源：http://wmk.zycfv.cn

[R63] 内存与进程
来源：http://fsw.jinqigfzy.top

free -h;  ps aux | grep nginx
来源：http://imp.ppjwa.cn

[R64] 结束进程
来源：http://kyd.dashuyun.cn

kill -9 $(pgrep -f app.py)
来源：http://ztd.ctjpmb.com

[R65] 查看端口占用
来源：http://tbl.smart0.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://esd.hammf.cn

[R66] 定时任务
来源：http://unr.fanxiaobao.xyz

crontab -e;  crontab -l
来源：http://uxg.gaohongyu789.top

[R67] 生成随机十六进制串
来源：http://vig.yj202588.top

openssl rand -hex 16
来源：http://lag.shangyingyoupin.top

[R68] 计算文件校验值
来源：http://iuo.fengsongda.top

sha256sum a.txt;  md5sum a.txt
来源：http://vpc.yfazqb.com

[R69] 生成随机密码
来源：http://mde.snrcjt.cn

head -c 16 /dev/urandom | base64
来源：http://cpx.svipenyu.cn

[R70] 时间戳与互转
来源：http://kin.vehdjk.com

date +%s;  date -d @1700000000
来源：http://hnk.vqdsnc.cn

[R71] 日期格式化
来源：http://dze.yonumen.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://uci.smart0.xyz

[R72] 等待端口就绪
来源：http://tgm.yueranfly.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ivc.chenlongwang.top

[R73] 分割大日志
来源：http://vky.kuanghao11.cn

split -l 1000 big.log part_
来源：http://enx.havefunace.top

[R74] 批量重命名
来源：http://ujp.chenzaomai.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wjo.hongshengwenyu.top

[R75] 导出环境变量
来源：http://xmj.hcnkem.com

export PATH="$HOME/bin:$PATH"
来源：http://hnr.shuidangran.top

[R76] 使用临时文件
来源：http://wes.52xcode.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://met.cheryme.top

[R77] 读取用户输入
来源：http://lro.bjfxy.top

read -rp "请输入: " ans
来源：http://kkk.yonumen.top

[R78] 交互式菜单
来源：http://tor.zhengqikj.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ycb.cucudq.cn

[R79] 解析命令行选项
来源：http://pff.xinyue.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xtp.fehbvm.com

[R80] 查看脚本执行耗时
来源：http://dti.aizwys.cn

time ./run.sh
来源：http://ngk.zhixingplan.top

================================================================================
来源：http://qap.jinqigufen.top

S. C / C++ 专题
来源：http://nyh.cheryme.top

================================================================================
来源：http://flu.bjfxy.top

[S01] C：Hello World
来源：http://cvt.wangdashe.top

#include <stdio.h>
来源：http://eqp.ydjk.org.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bdf.gzhubu.top

[S02] C：变量与格式化输出
来源：http://cvz.zhijiandao.cn

int a = 10; printf("%d\n", a);
来源：http://mcx.dashuyun.cn

[S03] C：读入整数
来源：http://blw.xinyue.icu

int x; scanf("%d", &x);
来源：http://cui.0kj1m.cn

[S04] C：字符串复制
来源：http://ijs.jqgufenzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://ahn.epnwcf.com

[S05] C：字符串长度
来源：http://jrk.daria6918.cn

strlen(s)
来源：http://twl.hfpthk.cn

[S06] C：字符串比较
来源：http://vql.hnqzz.top

strcmp(a, b) == 0
来源：http://ldd.haohaochexian.top

[S07] C：数组遍历求和
来源：http://vyh.yonumen.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://udo.xylfe.cn

[S08] C：动态内存分配与释放
来源：http://ath.fanxiaobao.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yhh.svipenyu.cn

[S09] C：结构体定义与初始化
来源：http://ehv.sufxvd.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lzc.316326.xyz

[S10] C：指针与解引用
来源：http://ang.quarkkingdee.top

int *p = &a;  *p = 5;
来源：http://mjo.zdbjq.cn

[S11] C：逐行读文件
来源：http://mhx.gotoacloud.top

FILE *f = fopen("a.txt", "r");
来源：http://uny.yuanzhike.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://lpg.daria6918.cn

fclose(f);
来源：http://sxj.nanxuanxn.top

[S12] C：写文件
来源：http://nkx.xinyue.icu

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://udn.shzxlz.cn

[S13] C：宏定义
来源：http://nej.zhijiandao.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jtt.smart0.xyz

[S14] C：枚举
来源：http://zfl.yanxiufei.cn

enum Color { RED, GREEN, BLUE };
来源：http://cbc.hammf.cn

[S15] C：类型转换
来源：http://bud.zhoulong.xyz

(double) a / b
来源：http://arj.ydjk.org.cn

[S16] C：位操作置位
来源：http://vcy.zhoulong.xyz

x |= (1 << 3);
来源：http://xjt.shuidangran.top

[S17] C：安全拼接字符串
来源：http://lmg.shangyingyoupin.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ygb.zhiwuduotai.top

[S18] C：命令行参数
来源：http://pjx.vqdsnc.cn

int main(int argc, char **argv)
来源：http://omx.guowangkeji.top

[S19] C：快速排序
来源：http://gwz.zdbjq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ecp.ybcxt.top

[S20] C：二分查找
来源：http://gjr.zdqjudy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tbv.yuanzhike.top

[S21] C：字符类别判断
来源：http://vbv.ehwqpu.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qdx.xinyue.icu

[S22] C：字符串转数字
来源：http://rml.chenjidiqi.icu

atoi("42");  strtod("3.14", NULL);
来源：http://tiz.hcnkem.com

[S23] C：随机数
来源：http://eqq.havefunace.top

srand(time(NULL));  int r = rand() % 100;
来源：http://cep.nanxinkj.top

[S24] C：获取本地时间
来源：http://fdg.birdmap.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rpg.hesvh.cn

[S25] C：内存拷贝
来源：http://uyg.tianlin.xyz

memcpy(dst, src, n);
来源：http://fvr.ctjpmb.com

[S26] C：内存清零
来源：http://arz.kuanghao11.cn

memset(a, 0, sizeof a);
来源：http://dos.zycfv.cn

[S27] C：定义常量
来源：http://vrl.chenlongwang.top

const double PI = 3.14159;
来源：http://gaz.hnqzz.top

[S28] C：静态变量
来源：http://fnh.hesvh.cn

static int counter = 0;
来源：http://zov.pycfn.com

[S29] C：变参函数
来源：http://udr.sysykeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lwn.ivvv.top

[S30] C：头文件保护
来源：http://nrq.ywan-chungtsiang.top

#ifndef X_H
来源：http://rjr.jiagoushi.top

#define X_H
来源：http://meh.jyoumei.cn

#endif
来源：http://sha.cdnleiting.top

[S31] C++：Hello World
来源：http://lke.haohaochexian.top

#include <iostream>
来源：http://ntr.shuidangran.top

int main() { std::cout << "Hello\n"; }
来源：http://zow.yj20258888.top

[S32] C++：字符串
来源：http://ljd.vehdjk.com

std::string s = "hi";  s += "!";
来源：http://rqe.xylfe.cn

[S33] C++：vector 增删
来源：http://vwc.hongshengwenyu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ajo.xingfuxueyuan.xyz

[S34] C++：遍历 vector
来源：http://ctq.zhijiandao.cn

for (auto &x : v) { std::cout << x; }
来源：http://nre.yonumen.top

[S35] C++：map
来源：http://nqc.shanyushiyangkeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lwk.yuanzhike.top

[S36] C++：unordered_map
来源：http://phb.zhiwuduotai.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zxu.sjlbkw.cn

[S37] C++：set
来源：http://wix.316326.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://omx.xziqi.cn

[S38] C++：排序
来源：http://mqs.jinqigfzy.top

std::sort(v.begin(), v.end());
来源：http://szk.ywan-chungtsiang.top

[S39] C++：自定义比较器排序
来源：http://frn.zhixingplan.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://htu.hfpthk.cn

[S40] C++：查找元素
来源：http://twd.gzhubu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uhg.tian-w.cn

[S41] C++：类与构造函数
来源：http://jfo.cqqwz.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vhc.daxiang520.top

[S42] C++：继承与虚函数
来源：http://ako.sxryk.cn

class B : public Base { public: void f() override {} };
来源：http://dvt.sysykeji.top

[S43] C++：智能指针
来源：http://ywc.zhaomingkeji.xyz

auto p = std::make_unique<int>(5);
来源：http://jbg.ppjwa.cn

[S44] C++：引用传参
来源：http://myp.jinqigufen.top

void inc(int &x) { ++x; }
来源：http://nrk.nanxinkj.top

[S45] C++：lambda
来源：http://mez.sufxvd.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vtn.wangshuangyany.cn

[S46] C++：函数模板
来源：http://gel.jinqigufen.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://azt.pengpengdd.cyou

[S47] C++：结构化绑定遍历
来源：http://khq.meibo888.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wvo.tian-w.cn

[S48] C++：逐行读文件
来源：http://kpl.0kj1m.cn

std::ifstream in("a.txt");  std::string line;
来源：http://iwo.pengpengdd.cyou

while (std::getline(in, line)) { }
来源：http://chy.cashguo.top

[S49] C++：写文件
来源：http://sfl.redwolf501.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://crn.kuanghao11.cn

[S50] C++：格式化数字
来源：http://toz.jyoumei.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://toq.snrcjt.cn

[S51] C++：显式类型转换
来源：http://zdz.iojbl.cn

static_cast<double>(a) / b
来源：http://lwp.hnqzz.top

[S52] C++：const 与 noexcept
来源：http://lpk.cashguo.top

int size() const noexcept { return n_; }
来源：http://evr.xziqi.cn

[S53] C++：移动语义
来源：http://vrc.shuidangran.top

std::vector<int> w = std::move(v);
来源：http://qgi.xuetiantiany.cn

[S54] C++：异常处理
来源：http://dpr.hfpthk.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://raf.gaohongyu789.top

[S55] C++：结构化绑定
来源：http://ltf.316326.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://nph.sjlbkw.cn

[S56] C++：optional
来源：http://mkm.bbcook.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uue.nwbrower.top

[S57] C++：编译期常量
来源：http://miq.ybcxt.top

constexpr int N = 10;
来源：http://bmg.vqdsnc.cn

[S58] C++：命名空间
来源：http://bze.c1oappe.top

namespace ns { int f() { return 1; } }
来源：http://zqu.yanxiufei.cn

[S59] C++：静态断言
来源：http://djt.feifeiyinyue.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ply.feifeiyinyue.top

[S60] C++：遍历并删除元素
来源：http://qqr.fzhhl.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fpt.cheryme.top

================================================================================
来源：http://zcg.zhoulong.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pfy.dianchejie.cn

================================================================================
来源：http://vzz.zhoulong.xyz

[T01] Kotlin：Hello World
来源：http://jko.fanxiaobao.xyz

println("Hello")
来源：http://mif.yvedp.cn

[T02] Kotlin：变量
来源：http://ulh.yanxiufei.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://eud.guowangkeji.top

[T03] Kotlin：字符串模板
来源：http://ico.jinqigufen.top

"值: $b"
来源：http://cro.yj202588.top

[T04] Kotlin：空安全
来源：http://owc.guannengcc.top

val n: String? = null;  n?.length
来源：http://ryo.ppjwa.cn

[T05] Kotlin：when 表达式
来源：http://ejx.xinyue.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://had.zhixingplan.top

[T06] Kotlin：集合映射
来源：http://bel.vqdsnc.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pdl.guowangkeji.top

[T07] Kotlin：集合过滤
来源：http://zqk.hcnkem.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://rlc.zhongyouzk.top

[T08] Kotlin：数据类
来源：http://wbs.zdbjq.cn

data class User(val name: String, val age: Int)
来源：http://bbe.ehwqpu.com

[T09] Kotlin：扩展函数
来源：http://jjp.ydjk.org.cn

fun String.exclaim() = this + "!"
来源：http://mtw.9152youxi.cn

[T10] Kotlin：默认参数
来源：http://zpe.yangfankeji.com

fun greet(name: String = "World") = "Hi $name"
来源：http://dqb.yj20258888.top

[T11] Kotlin：协程
来源：http://iuu.chenlongwang.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://zjq.ehwqpu.com

[T12] Kotlin：解构声明
来源：http://zcc.gogol.net.cn

val (a, b) = Pair(1, 2)
来源：http://iiw.cheryme.top

[T13] Kotlin：只读 Map
来源：http://eda.ppjwa.cn

val m = mapOf("a" to 1)
来源：http://hrx.zdbjq.cn

[T14] Kotlin：循环
来源：http://pni.ydzc1.top

for (i in 1..10) println(i)
来源：http://iba.hysaishi.cn

[T15] Kotlin：接口
来源：http://nkx.birdmap.top

interface Shape { fun area(): Double }
来源：http://qce.tian-w.cn

[T16] Swift：Hello World
来源：http://mcz.gzhubu.top

print("Hello")
来源：http://ggk.zhixingplan.top

[T17] Swift：变量与常量
来源：http://huc.pycfn.com

var a = 1;  let b = 2
来源：http://cfh.fzhhl.top

[T18] Swift：字符串插值
来源：http://syq.sufxvd.cn

"值: \(b)"
来源：http://kkm.gotoacloud.top

[T19] Swift：可选绑定
来源：http://inh.chenlongwang.top

if let n = opt { print(n) }
来源：http://cbb.tian-w.cn

[T20] Swift：数组操作
来源：http://jow.316326.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://gzz.cashguo.top

[T21] Swift：遍历
来源：http://hch.jlsjyb.cn

for x in a { print(x) }
来源：http://fpo.jqgfzy.top

[T22] Swift：字典
来源：http://hvo.yfazqb.com

var d = ["a": 1];  d["b"] = 2
来源：http://wsk.yj202588.top

[T23] Swift：函数
来源：http://mzk.fktsv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rak.sxryk.cn

[T24] Swift：闭包
来源：http://ouw.jinyuanbaomall.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://plw.fzhhl.top

[T25] Swift：结构体
来源：http://kik.xingfuxueyuan.xyz

struct P { var x: Int }
来源：http://mdh.wangdashe.top

[T26] Swift：类与重写
来源：http://all.xinyue.icu

class A: Base { override func f() {} }
来源：http://vpy.zhengqikj.top

[T27] Swift：错误处理
来源：http://uen.xinyue.icu

do { try f() } catch { print(error) }
来源：http://dui.shanyushiyangkeji.top

[T28] Swift：枚举
来源：http://kso.bjfxy.top

enum Color { case red, green }
来源：http://wlq.sxryk.cn

[T29] Swift：guard 提前返回
来源：http://vvr.zhijiandao.cn

guard let x = opt else { return }
来源：http://jib.shangyingyoupin.top

[T30] Swift：协议
来源：http://upc.feifeiyinyue.top

protocol Shape { func area() -> Double }
来源：http://ecw.fzhhl.top

[T31] Lua：Hello World
来源：http://mco.ybcxt.top

print("Hello")
来源：http://zko.fzhhl.top

[T32] Lua：局部变量
来源：http://rwt.ppjwa.cn

local a = 1
来源：http://fub.sufxvd.cn

[T33] Lua：表（数组）
来源：http://ptd.fanxiaobao.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://vjl.shangyingyoupin.top

[T34] Lua：遍历表
来源：http://wri.shzxlz.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://djx.sjlbkw.cn

[T35] Lua：字典表
来源：http://kjw.cdnleiting.top

local d = { a = 1 };  d.b = 2
来源：http://iit.ppjwa.cn

[T36] Lua：函数
来源：http://ies.jianghu66.top

function add(a, b) return a + b end
来源：http://xwx.52xcode.cn


<!-- 参考信息 -->