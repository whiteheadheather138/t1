代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dea.pengpengdd.cyou

[R34] 退出时清理
来源：http://xvg.fanxiaobao.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://uiu.cdnleiting.top

[R35] 后台执行并等待
来源：http://eah.sysykeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://hrq.yj202588.top

[R36] 并发执行多个任务
来源：http://frf.jinyuanbaomall.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://itr.zycfv.cn

[R37] 把输出赋给变量
来源：http://vyk.yfazqb.com

files=$(ls -1)
来源：http://hjv.xuanzx.com

[R38] 管道串联
来源：http://zjt.yvedp.cn

cat a.txt | grep -i error | wc -l
来源：http://qat.zhiwuduotai.top

[R39] 重定向标准输出与错误
来源：http://kpj.fanxiaobao.xyz

cmd > out.log 2>&1
来源：http://kwa.jinqigfzy.top

[R40] 追加写日志
来源：http://prw.jlsjyb.cn

echo "log" >> out.log
来源：http://vgg.dashuyun.cn

[R41] 丢弃输出
来源：http://whn.zhaomingkeji.xyz

cmd >/dev/null 2>&1
来源：http://blo.zdbjq.cn

[R42] 输入重定向
来源：http://cxa.jlsjyb.cn

wc -l < a.txt
来源：http://xgt.zdbjq.cn

[R43] 按名字查找文件
来源：http://sla.wangshuangyany.cn

find . -name "*.log" -type f
来源：http://fnt.tanke756.top

[R44] 按修改时间查找
来源：http://btg.yuxming.cn

find . -mtime -7 -type f
来源：http://nlf.hongshengwenyu.top

[R45] 批量删除
来源：http://ofl.uphjek.com

find . -name "*.tmp" -delete
来源：http://iid.tarul.cn

[R46] 递归替换文件内容
来源：http://kif.cucudq.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mig.guowangkeji.top

[R47] sed 单行替换
来源：http://iqx.yuanzhike.top

sed -i 's/foo/bar/g' a.txt
来源：http://vlx.ctjpmb.com

[R48] awk 取指定列
来源：http://syf.zdqjudy.top

awk '{print $1, $3}' a.txt
来源：http://wnk.hfpthk.cn

[R49] awk 带条件
来源：http://nhh.sweek.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://thh.cqqwz.cn

[R50] awk 求和
来源：http://cjq.fanxiaobao.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://wlr.jqgufenzy.top

[R51] 排序去重取前几
来源：http://nuf.daria6918.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pbf.yongpay.top

[R52] 统计行数
来源：http://uzx.pengpengdd.cyou

wc -l a.txt
来源：http://fep.zhoulong.xyz

[R53] 查看文件头与实时尾
来源：http://kab.shanyushiyangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kxa.mhx1999.top

[R54] 比较两个文件
来源：http://foh.fanxiaobao.xyz

diff a.txt b.txt
来源：http://zli.chenlongwang.top

[R55] 压缩与解压
来源：http://pba.fktsv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xup.guannengcc.top

[R56] 远程拷贝
来源：http://tvl.tianlin.xyz

scp file user@host:/path/
来源：http://bug.hnxiangtu.top

[R57] 远程执行命令
来源：http://mli.zdqjudy.top

ssh user@host 'uptime'
来源：http://dxb.dashuyun.cn

[R58] 下载文件
来源：http://dda.shzxlz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dhx.uphjek.com

[R59] 发 POST JSON
来源：http://qvv.ydzc1.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rvq.tarul.cn

[R60] 只看 HTTP 状态码
来源：http://jul.jinqigfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xwv.nanxinkj.top

[R61] 磁盘占用
来源：http://wcb.yuanzhike.top

df -h;  du -sh *
来源：http://kum.yuxming.cn

[R62] 找最占空间的文件
来源：http://rcq.jinyuanbaomall.cn

du -ah . | sort -rh | head -10
来源：http://qkp.guannengcc.top

[R63] 内存与进程
来源：http://gpe.hnqzz.top

free -h;  ps aux | grep nginx
来源：http://glx.yfazqb.com

[R64] 结束进程
来源：http://gfq.xziqi.cn

kill -9 $(pgrep -f app.py)
来源：http://uum.nwbrower.top

[R65] 查看端口占用
来源：http://sxy.jiagoushi.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jzm.ybcxt.top

[R66] 定时任务
来源：http://zwy.gogol.net.cn

crontab -e;  crontab -l
来源：http://fmh.gaohongyu789.top

[R67] 生成随机十六进制串
来源：http://wgu.nanxinkj.top

openssl rand -hex 16
来源：http://ann.yj20258888.top

[R68] 计算文件校验值
来源：http://feb.0kj1m.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vju.yongpay.top

[R69] 生成随机密码
来源：http://owb.fengsongda.top

head -c 16 /dev/urandom | base64
来源：http://jip.xziqi.cn

[R70] 时间戳与互转
来源：http://urm.pycfn.com

date +%s;  date -d @1700000000
来源：http://auw.shuidangran.top

[R71] 日期格式化
来源：http://uqw.vqdsnc.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hiw.tanke756.top

[R72] 等待端口就绪
来源：http://saq.sweek.top

until nc -z localhost 3306; do sleep 1; done
来源：http://aio.birdmap.top

[R73] 分割大日志
来源：http://nst.epnwcf.com

split -l 1000 big.log part_
来源：http://zsf.zhoulong.xyz

[R74] 批量重命名
来源：http://pak.guannengcc.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jbq.ppjwa.cn

[R75] 导出环境变量
来源：http://mcz.wangdashe.top

export PATH="$HOME/bin:$PATH"
来源：http://gqz.havefunace.top

[R76] 使用临时文件
来源：http://hfw.ybcxt.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ujl.haohaochexian.top

[R77] 读取用户输入
来源：http://odv.hnxiangtu.top

read -rp "请输入: " ans
来源：http://wgf.jinqigufen.top

[R78] 交互式菜单
来源：http://uqx.snrcjt.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://arh.hywenlv.cn

[R79] 解析命令行选项
来源：http://wlk.9152youxi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://etg.yanxiufei.cn

[R80] 查看脚本执行耗时
来源：http://yjf.redwolf501.top

time ./run.sh
来源：http://iuw.xingfuxueyuan.xyz

================================================================================
来源：http://svw.jinqigfzy.top

S. C / C++ 专题
来源：http://zal.ywan-chungtsiang.top

================================================================================
来源：http://vvy.meibo888.top

[S01] C：Hello World
来源：http://lrv.hfpthk.cn

#include <stdio.h>
来源：http://gcl.tian-w.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ulg.zhijiandao.cn

[S02] C：变量与格式化输出
来源：http://nao.meibo888.top

int a = 10; printf("%d\n", a);
来源：http://ofk.zhongyouzk.top

[S03] C：读入整数
来源：http://qfx.nanxinkj.top

int x; scanf("%d", &x);
来源：http://nek.chenjidiqi.icu

[S04] C：字符串复制
来源：http://zhq.shanyushiyangtech.top

char dst[32]; strcpy(dst, "hi");
来源：http://iun.ydjk.org.cn

[S05] C：字符串长度
来源：http://hzp.gotoacloud.top

strlen(s)
来源：http://nrp.ydzc1.top

[S06] C：字符串比较
来源：http://mtx.jlsjyb.cn

strcmp(a, b) == 0
来源：http://hsk.hywenlv.cn

[S07] C：数组遍历求和
来源：http://qmx.ivvv.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uit.xingfuxueyuan.xyz

[S08] C：动态内存分配与释放
来源：http://squ.quarkkingdee.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ifh.xziqi.cn

[S09] C：结构体定义与初始化
来源：http://scy.ywan-chungtsiang.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ghl.cdnleiting.top

[S10] C：指针与解引用
来源：http://ejr.gogol.net.cn

int *p = &a;  *p = 5;
来源：http://llu.fzhhl.top

[S11] C：逐行读文件
来源：http://hdd.316326.xyz

FILE *f = fopen("a.txt", "r");
来源：http://wrj.guowangkeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://cfy.vehdjk.com

fclose(f);
来源：http://wvi.fzhhl.top

[S12] C：写文件
来源：http://hsr.ehwqpu.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yzi.bjfxy.top

[S13] C：宏定义
来源：http://cdl.jinyuanbaomall.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://beo.birdmap.top

[S14] C：枚举
来源：http://jkd.uphjek.com

enum Color { RED, GREEN, BLUE };
来源：http://izz.cucudq.cn

[S15] C：类型转换
来源：http://frg.ivvv.top

(double) a / b
来源：http://erq.haohaochexian.top

[S16] C：位操作置位
来源：http://lah.nanxuanxn.top

x |= (1 << 3);
来源：http://iac.shangyingyoupin.top

[S17] C：安全拼接字符串
来源：http://duz.ydzc1.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://duu.andypj.xyz

[S18] C：命令行参数
来源：http://kvm.chenjidiqi.icu

int main(int argc, char **argv)
来源：http://ntk.sufxvd.cn

[S19] C：快速排序
来源：http://nzv.hammf.cn

qsort(a, n, sizeof(int), cmp);
来源：http://oyv.zhengqikj.top

[S20] C：二分查找
来源：http://lwe.cdnleiting.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://weo.ppjwa.cn

[S21] C：字符类别判断
来源：http://kjl.ydjk.org.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zle.zhongyouzk.top

[S22] C：字符串转数字
来源：http://vqt.zhiwuduotai.top

atoi("42");  strtod("3.14", NULL);
来源：http://fsf.cucudq.cn

[S23] C：随机数
来源：http://ojf.havefunace.top

srand(time(NULL));  int r = rand() % 100;
来源：http://oor.nanxuanxn.top

[S24] C：获取本地时间
来源：http://yfc.hongshengwenyu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gvy.bbcook.cn

[S25] C：内存拷贝
来源：http://sdd.dashuyun.cn

memcpy(dst, src, n);
来源：http://emk.yonumen.top

[S26] C：内存清零
来源：http://jas.fehbvm.com

memset(a, 0, sizeof a);
来源：http://xal.hnqzz.top

[S27] C：定义常量
来源：http://tan.redwolf501.top

const double PI = 3.14159;
来源：http://lmw.sufxvd.cn

[S28] C：静态变量
来源：http://lqy.shuidangran.top

static int counter = 0;
来源：http://rwi.chenlongwang.top

[S29] C：变参函数
来源：http://kdp.xuanzx.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://aih.birdmap.top

[S30] C：头文件保护
来源：http://tjj.guannengcc.top

#ifndef X_H
来源：http://eiv.cashguo.top

#define X_H
来源：http://eed.jinqigfzy.top

#endif
来源：http://fsm.cdnleiting.top

[S31] C++：Hello World
来源：http://yml.bjfxy.top

#include <iostream>
来源：http://txa.ivvv.top

int main() { std::cout << "Hello\n"; }
来源：http://ouz.birdmap.top

[S32] C++：字符串
来源：http://cwq.ivvv.top

std::string s = "hi";  s += "!";
来源：http://hcf.ivvv.top

[S33] C++：vector 增删
来源：http://fqp.kuanghao11.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ahj.dianchejie.cn

[S34] C++：遍历 vector
来源：http://dxs.ywan-chungtsiang.top

for (auto &x : v) { std::cout << x; }
来源：http://qow.cheryme.top

[S35] C++：map
来源：http://ygw.zhoulong.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zjo.ydjk.org.cn

[S36] C++：unordered_map
来源：http://rrb.fehbvm.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://puh.sxryk.cn

[S37] C++：set
来源：http://dxm.daxiang520.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ysa.xuetiantiany.cn

[S38] C++：排序
来源：http://nsv.tian-w.cn

std::sort(v.begin(), v.end());
来源：http://sug.fengsongda.top

[S39] C++：自定义比较器排序
来源：http://aib.cheryme.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kqi.jqgfzy.top

[S40] C++：查找元素
来源：http://vpe.fehbvm.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://emx.vqdsnc.cn

[S41] C++：类与构造函数
来源：http://nkc.zycfv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gnk.c1oappe.top

[S42] C++：继承与虚函数
来源：http://tgg.shangyingyoupin.top

class B : public Base { public: void f() override {} };
来源：http://mzk.shangyingyoupin.top

[S43] C++：智能指针
来源：http://edo.tanke756.top

auto p = std::make_unique<int>(5);
来源：http://hyu.svipenyu.cn

[S44] C++：引用传参
来源：http://vjc.hongshengwenyu.top

void inc(int &x) { ++x; }
来源：http://dci.hcnkem.com

[S45] C++：lambda
来源：http://vjn.xylfe.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fuc.sweek.top

[S46] C++：函数模板
来源：http://xlj.hnqzz.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pqh.jinghuilouyu.cn

[S47] C++：结构化绑定遍历
来源：http://aat.hysaishi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yyu.shzxlz.cn

[S48] C++：逐行读文件
来源：http://acs.cashguo.top

std::ifstream in("a.txt");  std::string line;
来源：http://tci.ydzc1.top

while (std::getline(in, line)) { }
来源：http://tpm.sxryk.cn

[S49] C++：写文件
来源：http://ggu.tianlin.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hvj.fehbvm.com

[S50] C++：格式化数字
来源：http://ebo.uphjek.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kuf.chenzaomai.com

[S51] C++：显式类型转换
来源：http://bim.yj202588.top

static_cast<double>(a) / b
来源：http://bbb.yonumen.top

[S52] C++：const 与 noexcept
来源：http://kej.shanyushiyangtech.top

int size() const noexcept { return n_; }
来源：http://ofd.fengsongda.top

[S53] C++：移动语义
来源：http://uxb.sjlbkw.cn

std::vector<int> w = std::move(v);
来源：http://tpr.cqqwz.cn

[S54] C++：异常处理
来源：http://cki.zhijiandao.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nya.hongshengwenyu.top

[S55] C++：结构化绑定
来源：http://uew.yangfankeji.com

auto [a, b] = std::make_pair(1, 2);
来源：http://cze.zycfv.cn

[S56] C++：optional
来源：http://evl.hongshengwenyu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ivs.fktsv.cn

[S57] C++：编译期常量
来源：http://ptk.yj20258888.top

constexpr int N = 10;
来源：http://qvm.fehbvm.com

[S58] C++：命名空间
来源：http://eky.gzhubu.top

namespace ns { int f() { return 1; } }
来源：http://amv.chenzaomai.com

[S59] C++：静态断言
来源：http://rnp.ppjwa.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pag.tianlin.xyz

[S60] C++：遍历并删除元素
来源：http://aki.jiagoushi.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ghe.smart0.xyz

================================================================================
来源：http://eri.chenjidiqi.icu

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hem.316326.xyz

================================================================================
来源：http://dew.ydzc1.top

[T01] Kotlin：Hello World
来源：http://ufy.jqgfzy.top

println("Hello")
来源：http://czg.yuxming.cn

[T02] Kotlin：变量
来源：http://yir.fzhhl.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jvs.yangfankeji.com

[T03] Kotlin：字符串模板
来源：http://fau.xuanzx.com

"值: $b"
来源：http://iga.yj202588.top

[T04] Kotlin：空安全
来源：http://xti.shuidangran.top

val n: String? = null;  n?.length
来源：http://dhe.sufxvd.cn

[T05] Kotlin：when 表达式
来源：http://hpl.ydzc1.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qbn.jinyuanbaomall.cn

[T06] Kotlin：集合映射
来源：http://urm.nanxuanxn.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ndn.zhiwuduotai.top

[T07] Kotlin：集合过滤
来源：http://tgh.jinyuanbaomall.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cmp.iojbl.cn

[T08] Kotlin：数据类
来源：http://ljq.nanxinkj.top

data class User(val name: String, val age: Int)
来源：http://akd.sxryk.cn

[T09] Kotlin：扩展函数
来源：http://bon.pengpengdd.cyou

fun String.exclaim() = this + "!"
来源：http://tel.hysaishi.cn

[T10] Kotlin：默认参数
来源：http://zvd.hnxiangtu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ggo.uphjek.com

[T11] Kotlin：协程
来源：http://jpv.meibo888.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://bmk.dianchejie.cn

[T12] Kotlin：解构声明
来源：http://xrr.haohaochexian.top

val (a, b) = Pair(1, 2)
来源：http://gxx.havefunace.top

[T13] Kotlin：只读 Map
来源：http://syh.cashguo.top

val m = mapOf("a" to 1)
来源：http://qtx.fengsongda.top

[T14] Kotlin：循环
来源：http://tzt.haohaochexian.top

for (i in 1..10) println(i)
来源：http://wjn.sufxvd.cn

[T15] Kotlin：接口
来源：http://rks.yj20258888.top

interface Shape { fun area(): Double }
来源：http://tus.cheryme.top

[T16] Swift：Hello World
来源：http://xal.shanyushiyangtech.top

print("Hello")
来源：http://ljf.fengsongda.top

[T17] Swift：变量与常量
来源：http://cdf.sysykeji.top

var a = 1;  let b = 2
来源：http://dcf.gzhubu.top

[T18] Swift：字符串插值
来源：http://wns.sweek.top

"值: \(b)"
来源：http://fvh.havefunace.top

[T19] Swift：可选绑定
来源：http://emp.52xcode.cn

if let n = opt { print(n) }
来源：http://eac.nanxuanxn.top

[T20] Swift：数组操作
来源：http://mtc.wangshuangyany.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nfb.ctjpmb.com

[T21] Swift：遍历
来源：http://tci.redwolf501.top

for x in a { print(x) }
来源：http://tac.tian-w.cn

[T22] Swift：字典
来源：http://wco.snrcjt.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dcp.ydjk.org.cn

[T23] Swift：函数
来源：http://eid.tianlin.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hpo.daxiang520.top

[T24] Swift：闭包
来源：http://sim.zhijiandao.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ibj.yuanzhike.top

[T25] Swift：结构体
来源：http://iqw.0kj1m.cn

struct P { var x: Int }
来源：http://oth.jiagoushi.top

[T26] Swift：类与重写
来源：http://elw.cucudq.cn

class A: Base { override func f() {} }
来源：http://pkq.hammf.cn

[T27] Swift：错误处理
来源：http://gfj.smart0.xyz

do { try f() } catch { print(error) }
来源：http://nmw.guowangkeji.top

[T28] Swift：枚举
来源：http://gzb.sufxvd.cn

enum Color { case red, green }
来源：http://nwj.fktsv.cn

[T29] Swift：guard 提前返回
来源：http://zph.sxryk.cn

guard let x = opt else { return }
来源：http://elq.sweek.top

[T30] Swift：协议
来源：http://nvz.zhaomingkeji.xyz

protocol Shape { func area() -> Double }
来源：http://thi.yj20258.top

[T31] Lua：Hello World
来源：http://cpy.kuanghao11.cn

print("Hello")
来源：http://fxt.bjfxy.top

[T32] Lua：局部变量
来源：http://bja.havefunace.top

local a = 1
来源：http://eah.zhijiandao.cn

[T33] Lua：表（数组）
来源：http://kye.ybcxt.top

local t = {1, 2, 3};  t[4] = 4
来源：http://xno.iojbl.cn

[T34] Lua：遍历表
来源：http://xab.dashuyun.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://muy.andypj.xyz

[T35] Lua：字典表
来源：http://ari.xuanzx.com

local d = { a = 1 };  d.b = 2
来源：http://znw.mhx1999.top

[T36] Lua：函数
来源：http://rpn.jiagoushi.top

function add(a, b) return a + b end
来源：http://kwb.52xcode.cn


<!-- 参考信息 -->