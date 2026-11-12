代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://kfb.zycfv.cn

[R32] 参数个数校验
来源：http://cql.ppjwa.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wag.sjlbkw.cn

[R33] 捕获错误并提示行号
来源：http://cdw.dianchejie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pvx.zycfv.cn

[R34] 退出时清理
来源：http://csp.yanxiufei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uef.zhongyouzk.top

[R35] 后台执行并等待
来源：http://ccj.aibaodan.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fie.tian-w.cn

[R36] 并发执行多个任务
来源：http://rax.jiagoushi.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mer.svipenyu.cn

[R37] 把输出赋给变量
来源：http://kah.gotoacloud.top

files=$(ls -1)
来源：http://uuw.vqdsnc.cn

[R38] 管道串联
来源：http://fqi.fzhhl.top

cat a.txt | grep -i error | wc -l
来源：http://eoi.epnwcf.com

[R39] 重定向标准输出与错误
来源：http://xne.jinghuilouyu.cn

cmd > out.log 2>&1
来源：http://uyw.hnxiangtu.top

[R40] 追加写日志
来源：http://kah.xziqi.cn

echo "log" >> out.log
来源：http://vru.svipenyu.cn

[R41] 丢弃输出
来源：http://yko.aizwys.cn

cmd >/dev/null 2>&1
来源：http://ppc.sweek.top

[R42] 输入重定向
来源：http://gma.yuxming.cn

wc -l < a.txt
来源：http://ona.smart0.xyz

[R43] 按名字查找文件
来源：http://hhd.fehbvm.com

find . -name "*.log" -type f
来源：http://kmm.52xcode.cn

[R44] 按修改时间查找
来源：http://wvh.fehbvm.com

find . -mtime -7 -type f
来源：http://uhd.haohaochexian.top

[R45] 批量删除
来源：http://tdp.shangyingyoupin.top

find . -name "*.tmp" -delete
来源：http://vaw.jlsjyb.cn

[R46] 递归替换文件内容
来源：http://apg.gotoacloud.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nbf.hongshengwenyu.top

[R47] sed 单行替换
来源：http://gno.zhengqikj.top

sed -i 's/foo/bar/g' a.txt
来源：http://ebq.52xcode.cn

[R48] awk 取指定列
来源：http://crd.hcnkem.com

awk '{print $1, $3}' a.txt
来源：http://hkj.sysykeji.top

[R49] awk 带条件
来源：http://fhw.yueranfly.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://weo.zhengqikj.top

[R50] awk 求和
来源：http://ksl.sxryk.cn

awk '{s += $2} END {print s}' a.txt
来源：http://trl.nanxuanxn.top

[R51] 排序去重取前几
来源：http://bog.9152youxi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gxu.tianlin.xyz

[R52] 统计行数
来源：http://tcq.jlsjyb.cn

wc -l a.txt
来源：http://oum.sweek.top

[R53] 查看文件头与实时尾
来源：http://acs.jinqigfzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nsj.cheryme.top

[R54] 比较两个文件
来源：http://ucn.ivvv.top

diff a.txt b.txt
来源：http://jdq.cucudq.cn

[R55] 压缩与解压
来源：http://pzp.chenzaomai.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://exy.fzhhl.top

[R56] 远程拷贝
来源：http://jhy.cashguo.top

scp file user@host:/path/
来源：http://jnw.hfpthk.cn

[R57] 远程执行命令
来源：http://uli.nanxinkj.top

ssh user@host 'uptime'
来源：http://yez.ehwqpu.com

[R58] 下载文件
来源：http://vsr.svipenyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bof.aibaodan.cn

[R59] 发 POST JSON
来源：http://zxw.sxryk.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rkk.cdnleiting.top

[R60] 只看 HTTP 状态码
来源：http://vjl.cqqwz.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hbw.ybcxt.top

[R61] 磁盘占用
来源：http://efp.jianghu66.top

df -h;  du -sh *
来源：http://vaf.hnxiangtu.top

[R62] 找最占空间的文件
来源：http://kwe.jinghuilouyu.cn

du -ah . | sort -rh | head -10
来源：http://ary.mhx1999.top

[R63] 内存与进程
来源：http://pnn.nwbrower.top

free -h;  ps aux | grep nginx
来源：http://ybs.birdmap.top

[R64] 结束进程
来源：http://jwx.uphjek.com

kill -9 $(pgrep -f app.py)
来源：http://skj.hcnkem.com

[R65] 查看端口占用
来源：http://tmb.tarul.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wum.aibaodan.cn

[R66] 定时任务
来源：http://utw.cucudq.cn

crontab -e;  crontab -l
来源：http://zzf.xinyue.icu

[R67] 生成随机十六进制串
来源：http://ojd.ppjwa.cn

openssl rand -hex 16
来源：http://nwv.zhoulong.xyz

[R68] 计算文件校验值
来源：http://etz.jyoumei.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zyd.yj202588.top

[R69] 生成随机密码
来源：http://mdu.xziqi.cn

head -c 16 /dev/urandom | base64
来源：http://rki.guowangkeji.top

[R70] 时间戳与互转
来源：http://qoi.zhongyouzk.top

date +%s;  date -d @1700000000
来源：http://olb.cheryme.top

[R71] 日期格式化
来源：http://vrm.sweek.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://mqm.epnwcf.com

[R72] 等待端口就绪
来源：http://sow.vehdjk.com

until nc -z localhost 3306; do sleep 1; done
来源：http://hxp.shuidangran.top

[R73] 分割大日志
来源：http://ucm.haohaochexian.top

split -l 1000 big.log part_
来源：http://lwd.hnxiangtu.top

[R74] 批量重命名
来源：http://otb.jianghu66.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cer.yvedp.cn

[R75] 导出环境变量
来源：http://fvv.yfazqb.com

export PATH="$HOME/bin:$PATH"
来源：http://lni.shuidangran.top

[R76] 使用临时文件
来源：http://ykn.gogol.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ynt.aizwys.cn

[R77] 读取用户输入
来源：http://eup.meibo888.top

read -rp "请输入: " ans
来源：http://xdl.chenjidiqi.icu

[R78] 交互式菜单
来源：http://vhz.nanxuanxn.top

select opt in a b c; do echo "$opt"; break; done
来源：http://cga.havefunace.top

[R79] 解析命令行选项
来源：http://fvc.daxiang520.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dvt.tarul.cn

[R80] 查看脚本执行耗时
来源：http://wso.sysykeji.top

time ./run.sh
来源：http://ubh.jlsjyb.cn

================================================================================
来源：http://kuh.xylfe.cn

S. C / C++ 专题
来源：http://kho.chenlongwang.top

================================================================================
来源：http://pli.kuanghao11.cn

[S01] C：Hello World
来源：http://nyk.smart0.xyz

#include <stdio.h>
来源：http://pxz.ehwqpu.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://vqd.chenlongwang.top

[S02] C：变量与格式化输出
来源：http://yge.jqgfzy.top

int a = 10; printf("%d\n", a);
来源：http://feq.sxryk.cn

[S03] C：读入整数
来源：http://uko.sjlbkw.cn

int x; scanf("%d", &x);
来源：http://vrr.yonumen.top

[S04] C：字符串复制
来源：http://erl.jinqigufen.top

char dst[32]; strcpy(dst, "hi");
来源：http://gsw.sufxvd.cn

[S05] C：字符串长度
来源：http://hly.pengpengdd.cyou

strlen(s)
来源：http://ajb.jinyuanbaomall.cn

[S06] C：字符串比较
来源：http://twg.cheryme.top

strcmp(a, b) == 0
来源：http://tcs.yj202588.top

[S07] C：数组遍历求和
来源：http://nxr.tianlin.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ssw.zdbjq.cn

[S08] C：动态内存分配与释放
来源：http://gjt.hcnkem.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wlf.9152youxi.cn

[S09] C：结构体定义与初始化
来源：http://kja.fanxiaobao.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mlx.haohaochexian.top

[S10] C：指针与解引用
来源：http://buc.gogol.net.cn

int *p = &a;  *p = 5;
来源：http://sah.zhengqikj.top

[S11] C：逐行读文件
来源：http://lco.nwbrower.top

FILE *f = fopen("a.txt", "r");
来源：http://dho.gaohongyu789.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://rns.xuetiantiany.cn

fclose(f);
来源：http://fxi.chenjidiqi.icu

[S12] C：写文件
来源：http://qgw.xuanzx.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ogb.yj20258888.top

[S13] C：宏定义
来源：http://qlk.birdmap.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bly.yfazqb.com

[S14] C：枚举
来源：http://wib.xinyue.icu

enum Color { RED, GREEN, BLUE };
来源：http://uwx.316326.xyz

[S15] C：类型转换
来源：http://pew.ppjwa.cn

(double) a / b
来源：http://bmt.wangdashe.top

[S16] C：位操作置位
来源：http://jbp.chenjidiqi.icu

x |= (1 << 3);
来源：http://vyz.guannengcc.top

[S17] C：安全拼接字符串
来源：http://shn.shanyushiyangtech.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nhg.zdbjq.cn

[S18] C：命令行参数
来源：http://kwq.havefunace.top

int main(int argc, char **argv)
来源：http://law.feifeiyinyue.top

[S19] C：快速排序
来源：http://kww.hammf.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pdd.vqdsnc.cn

[S20] C：二分查找
来源：http://qev.jlsjyb.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zbi.jyoumei.cn

[S21] C：字符类别判断
来源：http://ehq.316326.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dyg.yongpay.top

[S22] C：字符串转数字
来源：http://dfa.iojbl.cn

atoi("42");  strtod("3.14", NULL);
来源：http://oer.guowangkeji.top

[S23] C：随机数
来源：http://euo.havefunace.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fva.yonumen.top

[S24] C：获取本地时间
来源：http://ihn.jqgufenzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dbm.cucudq.cn

[S25] C：内存拷贝
来源：http://hzl.vqdsnc.cn

memcpy(dst, src, n);
来源：http://rsa.yueranfly.top

[S26] C：内存清零
来源：http://uvr.fanxiaobao.xyz

memset(a, 0, sizeof a);
来源：http://wvs.zhixingplan.top

[S27] C：定义常量
来源：http://dmh.svipenyu.cn

const double PI = 3.14159;
来源：http://gxn.iojbl.cn

[S28] C：静态变量
来源：http://wtr.jinghuilouyu.cn

static int counter = 0;
来源：http://nfd.wangdashe.top

[S29] C：变参函数
来源：http://oxt.shzxlz.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://stm.pengpengdd.cyou

[S30] C：头文件保护
来源：http://koe.epnwcf.com

#ifndef X_H
来源：http://muq.jqgufenzy.top

#define X_H
来源：http://iwb.vqdsnc.cn

#endif
来源：http://frc.hammf.cn

[S31] C++：Hello World
来源：http://ffz.hfpthk.cn

#include <iostream>
来源：http://hwc.xinyue.icu

int main() { std::cout << "Hello\n"; }
来源：http://kaw.fzhhl.top

[S32] C++：字符串
来源：http://lbd.hongshengwenyu.top

std::string s = "hi";  s += "!";
来源：http://ztq.yj202588.top

[S33] C++：vector 增删
来源：http://aoe.tian-w.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vlx.mhx1999.top

[S34] C++：遍历 vector
来源：http://ttp.tianlin.xyz

for (auto &x : v) { std::cout << x; }
来源：http://vjk.uphjek.com

[S35] C++：map
来源：http://sgd.yonumen.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fis.xuetiantiany.cn

[S36] C++：unordered_map
来源：http://vpl.dianchejie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pno.ydjk.org.cn

[S37] C++：set
来源：http://yjs.nanxuanxn.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ijj.cdnleiting.top

[S38] C++：排序
来源：http://noo.ywan-chungtsiang.top

std::sort(v.begin(), v.end());
来源：http://hui.yfazqb.com

[S39] C++：自定义比较器排序
来源：http://jdx.hywenlv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tcs.ppjwa.cn

[S40] C++：查找元素
来源：http://ago.shanyushiyangkeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bzz.jyoumei.cn

[S41] C++：类与构造函数
来源：http://eju.xuetiantiany.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rdr.sjlbkw.cn

[S42] C++：继承与虚函数
来源：http://pjf.jinghuilouyu.cn

class B : public Base { public: void f() override {} };
来源：http://yqg.tian-w.cn

[S43] C++：智能指针
来源：http://rkf.tianlin.xyz

auto p = std::make_unique<int>(5);
来源：http://fny.quarkkingdee.top

[S44] C++：引用传参
来源：http://pbu.zhijiandao.cn

void inc(int &x) { ++x; }
来源：http://byh.cqqwz.cn

[S45] C++：lambda
来源：http://htk.quarkkingdee.top

auto add = [](int a, int b) { return a + b; };
来源：http://avm.c1oappe.top

[S46] C++：函数模板
来源：http://qeb.meibo888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rrf.ehwqpu.com

[S47] C++：结构化绑定遍历
来源：http://dax.sufxvd.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oaq.chenjidiqi.icu

[S48] C++：逐行读文件
来源：http://cmq.jinyuanbaomall.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jxy.yanxiufei.cn

while (std::getline(in, line)) { }
来源：http://rak.yangfankeji.com

[S49] C++：写文件
来源：http://elv.daxiang520.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jsi.jlsjyb.cn

[S50] C++：格式化数字
来源：http://cpi.cucudq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fgn.gzhubu.top

[S51] C++：显式类型转换
来源：http://pow.ctjpmb.com

static_cast<double>(a) / b
来源：http://bff.yongpay.top

[S52] C++：const 与 noexcept
来源：http://foy.shanyushiyangtech.top

int size() const noexcept { return n_; }
来源：http://fjh.ivvv.top

[S53] C++：移动语义
来源：http://ald.wangshuangyany.cn

std::vector<int> w = std::move(v);
来源：http://jig.vqdsnc.cn

[S54] C++：异常处理
来源：http://jum.sjlbkw.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hho.gotoacloud.top

[S55] C++：结构化绑定
来源：http://css.svipenyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ond.fehbvm.com

[S56] C++：optional
来源：http://ntn.zdqjudy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://foq.iojbl.cn

[S57] C++：编译期常量
来源：http://rxg.fzhhl.top

constexpr int N = 10;
来源：http://ohq.wangdashe.top

[S58] C++：命名空间
来源：http://tyx.svipenyu.cn

namespace ns { int f() { return 1; } }
来源：http://dlq.yfazqb.com

[S59] C++：静态断言
来源：http://spg.hfpthk.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fhc.gzhubu.top

[S60] C++：遍历并删除元素
来源：http://jgs.zhengqikj.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cyu.zhixingplan.top

================================================================================
来源：http://xkc.ydjk.org.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wpp.chenzaomai.com

================================================================================
来源：http://eoa.ybcxt.top

[T01] Kotlin：Hello World
来源：http://xkb.yangfankeji.com

println("Hello")
来源：http://yet.hcnkem.com

[T02] Kotlin：变量
来源：http://xhd.cdnleiting.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fai.yueranfly.top

[T03] Kotlin：字符串模板
来源：http://gey.wangdashe.top

"值: $b"
来源：http://kdh.jlsjyb.cn

[T04] Kotlin：空安全
来源：http://ttn.fzhhl.top

val n: String? = null;  n?.length
来源：http://jgf.iojbl.cn

[T05] Kotlin：when 表达式
来源：http://vuu.yuanzhike.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gvs.chenlongwang.top

[T06] Kotlin：集合映射
来源：http://zoe.cheryme.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hox.ctjpmb.com

[T07] Kotlin：集合过滤
来源：http://yna.cqqwz.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fok.smart0.xyz

[T08] Kotlin：数据类
来源：http://ydd.yj20258888.top

data class User(val name: String, val age: Int)
来源：http://ckt.aizwys.cn

[T09] Kotlin：扩展函数
来源：http://jic.jqgufenzy.top

fun String.exclaim() = this + "!"
来源：http://ayx.316326.xyz

[T10] Kotlin：默认参数
来源：http://qop.aizwys.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://aak.tarul.cn

[T11] Kotlin：协程
来源：http://ujj.yonumen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://uhm.quarkkingdee.top

[T12] Kotlin：解构声明
来源：http://bwl.cashguo.top

val (a, b) = Pair(1, 2)
来源：http://mkg.snrcjt.cn

[T13] Kotlin：只读 Map
来源：http://fsb.guowangkeji.top

val m = mapOf("a" to 1)
来源：http://zyv.c1oappe.top

[T14] Kotlin：循环
来源：http://dgm.ctjpmb.com

for (i in 1..10) println(i)
来源：http://mnk.jqgfzy.top

[T15] Kotlin：接口
来源：http://qwi.cucudq.cn

interface Shape { fun area(): Double }
来源：http://ilh.zhengqikj.top

[T16] Swift：Hello World
来源：http://whs.yj20258.top

print("Hello")
来源：http://cgu.jiagoushi.top

[T17] Swift：变量与常量
来源：http://opj.hesvh.cn

var a = 1;  let b = 2
来源：http://jyt.jqgfzy.top

[T18] Swift：字符串插值
来源：http://nek.haohaochexian.top

"值: \(b)"
来源：http://tao.guannengcc.top

[T19] Swift：可选绑定
来源：http://bvv.svipenyu.cn

if let n = opt { print(n) }
来源：http://ivx.chenlongwang.top

[T20] Swift：数组操作
来源：http://wft.kuanghao11.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hmm.aibaodan.cn

[T21] Swift：遍历
来源：http://pqu.iojbl.cn

for x in a { print(x) }
来源：http://xdf.ybcxt.top

[T22] Swift：字典
来源：http://zes.yueranfly.top

var d = ["a": 1];  d["b"] = 2
来源：http://aol.gogol.net.cn

[T23] Swift：函数
来源：http://ulz.xingfuxueyuan.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jnw.ehwqpu.com

[T24] Swift：闭包
来源：http://ynr.yvedp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hge.chenlongwang.top

[T25] Swift：结构体
来源：http://yxi.yj202588.top

struct P { var x: Int }
来源：http://mxy.shzxlz.cn

[T26] Swift：类与重写
来源：http://ydl.zhengqikj.top

class A: Base { override func f() {} }
来源：http://sme.zycfv.cn

[T27] Swift：错误处理
来源：http://tcs.shanyushiyangkeji.top

do { try f() } catch { print(error) }
来源：http://vcd.dianchejie.cn

[T28] Swift：枚举
来源：http://pxc.9152youxi.cn

enum Color { case red, green }
来源：http://snq.havefunace.top

[T29] Swift：guard 提前返回
来源：http://vus.sjlbkw.cn

guard let x = opt else { return }
来源：http://ybj.gogol.net.cn

[T30] Swift：协议
来源：http://daz.tianlin.xyz

protocol Shape { func area() -> Double }
来源：http://anl.yj20258.top

[T31] Lua：Hello World
来源：http://bej.daria6918.cn

print("Hello")
来源：http://uue.zhijiandao.cn

[T32] Lua：局部变量
来源：http://lwb.pycfn.com

local a = 1
来源：http://cnx.cucudq.cn

[T33] Lua：表（数组）
来源：http://dzo.yfazqb.com

local t = {1, 2, 3};  t[4] = 4
来源：http://owl.52xcode.cn

[T34] Lua：遍历表
来源：http://zce.sxryk.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rvc.cheryme.top


<!-- 参考信息 -->