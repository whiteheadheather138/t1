代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://tss.zhaomingkeji.xyz

[R32] 参数个数校验
来源：http://wrt.guannengcc.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baz.ydzc1.top

[R33] 捕获错误并提示行号
来源：http://gfg.kuanghao11.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ujg.daxiang520.top

[R34] 退出时清理
来源：http://hfv.yj202588.top

trap 'rm -f "$tmp"' EXIT
来源：http://ebh.tanke756.top

[R35] 后台执行并等待
来源：http://fcz.tarul.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://isj.0kj1m.cn

[R36] 并发执行多个任务
来源：http://nrt.xuetiantiany.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gsf.bbcook.cn

[R37] 把输出赋给变量
来源：http://cap.tianlin.xyz

files=$(ls -1)
来源：http://alz.316326.xyz

[R38] 管道串联
来源：http://cpu.52xcode.cn

cat a.txt | grep -i error | wc -l
来源：http://lcl.nanxinkj.top

[R39] 重定向标准输出与错误
来源：http://ope.shanyushiyangkeji.top

cmd > out.log 2>&1
来源：http://ayt.hongshengwenyu.top

[R40] 追加写日志
来源：http://cus.uphjek.com

echo "log" >> out.log
来源：http://bjh.iojbl.cn

[R41] 丢弃输出
来源：http://wci.nwbrower.top

cmd >/dev/null 2>&1
来源：http://olw.tianlin.xyz

[R42] 输入重定向
来源：http://fla.jlsjyb.cn

wc -l < a.txt
来源：http://uhp.ydjk.org.cn

[R43] 按名字查找文件
来源：http://icy.chenjidiqi.icu

find . -name "*.log" -type f
来源：http://bno.wangdashe.top

[R44] 按修改时间查找
来源：http://jrd.fktsv.cn

find . -mtime -7 -type f
来源：http://bix.gogol.net.cn

[R45] 批量删除
来源：http://xao.xuanzx.com

find . -name "*.tmp" -delete
来源：http://xlk.vqdsnc.cn

[R46] 递归替换文件内容
来源：http://igy.xingfuxueyuan.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lzi.jqgfzy.top

[R47] sed 单行替换
来源：http://fpx.sjlbkw.cn

sed -i 's/foo/bar/g' a.txt
来源：http://blh.52xcode.cn

[R48] awk 取指定列
来源：http://nou.cucudq.cn

awk '{print $1, $3}' a.txt
来源：http://dho.hnqzz.top

[R49] awk 带条件
来源：http://lzn.zhixingplan.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://svf.hesvh.cn

[R50] awk 求和
来源：http://pby.mhx1999.top

awk '{s += $2} END {print s}' a.txt
来源：http://err.sysykeji.top

[R51] 排序去重取前几
来源：http://uce.redwolf501.top

sort a.txt | uniq -c | sort -rn | head
来源：http://hyz.hysaishi.cn

[R52] 统计行数
来源：http://mkm.ydjk.org.cn

wc -l a.txt
来源：http://ozu.0kj1m.cn

[R53] 查看文件头与实时尾
来源：http://rli.ehwqpu.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mhc.c1oappe.top

[R54] 比较两个文件
来源：http://cgd.feifeiyinyue.top

diff a.txt b.txt
来源：http://nup.sufxvd.cn

[R55] 压缩与解压
来源：http://car.ydjk.org.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uri.daxiang520.top

[R56] 远程拷贝
来源：http://mnn.hongshengwenyu.top

scp file user@host:/path/
来源：http://kxu.mhx1999.top

[R57] 远程执行命令
来源：http://mzn.pengpengdd.cyou

ssh user@host 'uptime'
来源：http://ysq.sufxvd.cn

[R58] 下载文件
来源：http://ayw.sxryk.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ldz.zdbjq.cn

[R59] 发 POST JSON
来源：http://jmd.jinqigfzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nri.mhx1999.top

[R60] 只看 HTTP 状态码
来源：http://gni.zhoulong.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ssa.smart0.xyz

[R61] 磁盘占用
来源：http://oar.shuidangran.top

df -h;  du -sh *
来源：http://zpm.yj20258888.top

[R62] 找最占空间的文件
来源：http://shd.jqgfzy.top

du -ah . | sort -rh | head -10
来源：http://psk.zdbjq.cn

[R63] 内存与进程
来源：http://spi.hysaishi.cn

free -h;  ps aux | grep nginx
来源：http://bmn.sufxvd.cn

[R64] 结束进程
来源：http://nyp.zdbjq.cn

kill -9 $(pgrep -f app.py)
来源：http://tkq.shuidangran.top

[R65] 查看端口占用
来源：http://koi.xylfe.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lwa.redwolf501.top

[R66] 定时任务
来源：http://edv.yangfankeji.com

crontab -e;  crontab -l
来源：http://bof.ctjpmb.com

[R67] 生成随机十六进制串
来源：http://pxl.feifeiyinyue.top

openssl rand -hex 16
来源：http://bjx.zhoulong.xyz

[R68] 计算文件校验值
来源：http://enq.nwbrower.top

sha256sum a.txt;  md5sum a.txt
来源：http://tmq.daxiang520.top

[R69] 生成随机密码
来源：http://rjw.chenzaomai.com

head -c 16 /dev/urandom | base64
来源：http://tux.zhongyouzk.top

[R70] 时间戳与互转
来源：http://dxg.zhixingplan.top

date +%s;  date -d @1700000000
来源：http://ytc.hnqzz.top

[R71] 日期格式化
来源：http://jbq.uphjek.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://qon.fengsongda.top

[R72] 等待端口就绪
来源：http://cfb.gogol.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tec.jinqigfzy.top

[R73] 分割大日志
来源：http://udv.sjlbkw.cn

split -l 1000 big.log part_
来源：http://zka.svipenyu.cn

[R74] 批量重命名
来源：http://lju.ywan-chungtsiang.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qtc.iojbl.cn

[R75] 导出环境变量
来源：http://tqs.jianghu66.top

export PATH="$HOME/bin:$PATH"
来源：http://uvx.daria6918.cn

[R76] 使用临时文件
来源：http://rth.pengpengdd.cyou

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tuz.smart0.xyz

[R77] 读取用户输入
来源：http://duw.shzxlz.cn

read -rp "请输入: " ans
来源：http://erj.yonumen.top

[R78] 交互式菜单
来源：http://quf.jqgufenzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rkn.yj20258.top

[R79] 解析命令行选项
来源：http://cxe.gzhubu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qon.ctjpmb.com

[R80] 查看脚本执行耗时
来源：http://haj.xuetiantiany.cn

time ./run.sh
来源：http://slj.hnqzz.top

================================================================================
来源：http://mlp.gotoacloud.top

S. C / C++ 专题
来源：http://jnq.hywenlv.cn

================================================================================
来源：http://qzu.sweek.top

[S01] C：Hello World
来源：http://fjh.yongpay.top

#include <stdio.h>
来源：http://yig.316326.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://cod.gaohongyu789.top

[S02] C：变量与格式化输出
来源：http://wzz.sysykeji.top

int a = 10; printf("%d\n", a);
来源：http://ove.uphjek.com

[S03] C：读入整数
来源：http://aov.9152youxi.cn

int x; scanf("%d", &x);
来源：http://jii.bjfxy.top

[S04] C：字符串复制
来源：http://wos.ydzc1.top

char dst[32]; strcpy(dst, "hi");
来源：http://wag.feifeiyinyue.top

[S05] C：字符串长度
来源：http://sgd.birdmap.top

strlen(s)
来源：http://uaa.bbcook.cn

[S06] C：字符串比较
来源：http://vkf.aibaodan.cn

strcmp(a, b) == 0
来源：http://cij.sysykeji.top

[S07] C：数组遍历求和
来源：http://cpn.cucudq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fwh.cucudq.cn

[S08] C：动态内存分配与释放
来源：http://kdu.jqgfzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mnd.ctjpmb.com

[S09] C：结构体定义与初始化
来源：http://pyc.9152youxi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sgg.hesvh.cn

[S10] C：指针与解引用
来源：http://tmu.gaohongyu789.top

int *p = &a;  *p = 5;
来源：http://vtu.yj20258888.top

[S11] C：逐行读文件
来源：http://pym.sysykeji.top

FILE *f = fopen("a.txt", "r");
来源：http://lmh.cdnleiting.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://war.hfpthk.cn

fclose(f);
来源：http://ami.daria6918.cn

[S12] C：写文件
来源：http://olg.sjlbkw.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://obf.sjlbkw.cn

[S13] C：宏定义
来源：http://twv.cashguo.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://euo.cucudq.cn

[S14] C：枚举
来源：http://pmq.jlsjyb.cn

enum Color { RED, GREEN, BLUE };
来源：http://vmj.cqqwz.cn

[S15] C：类型转换
来源：http://xmg.cucudq.cn

(double) a / b
来源：http://yvn.bbcook.cn

[S16] C：位操作置位
来源：http://pva.wangshuangyany.cn

x |= (1 << 3);
来源：http://rsb.nanxinkj.top

[S17] C：安全拼接字符串
来源：http://blj.tarul.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://aws.tian-w.cn

[S18] C：命令行参数
来源：http://wsr.guowangkeji.top

int main(int argc, char **argv)
来源：http://prs.meibo888.top

[S19] C：快速排序
来源：http://blq.guowangkeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://pcd.nanxinkj.top

[S20] C：二分查找
来源：http://zhw.cashguo.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yye.fzhhl.top

[S21] C：字符类别判断
来源：http://ujs.bbcook.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://oiw.pengpengdd.cyou

[S22] C：字符串转数字
来源：http://dra.nwbrower.top

atoi("42");  strtod("3.14", NULL);
来源：http://pgu.vqdsnc.cn

[S23] C：随机数
来源：http://ukx.vehdjk.com

srand(time(NULL));  int r = rand() % 100;
来源：http://xrn.zhixingplan.top

[S24] C：获取本地时间
来源：http://iqs.meibo888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bst.pengpengdd.cyou

[S25] C：内存拷贝
来源：http://amw.yj20258.top

memcpy(dst, src, n);
来源：http://zxc.hammf.cn

[S26] C：内存清零
来源：http://yvh.cheryme.top

memset(a, 0, sizeof a);
来源：http://qzx.ppjwa.cn

[S27] C：定义常量
来源：http://jzt.yueranfly.top

const double PI = 3.14159;
来源：http://mll.nwbrower.top

[S28] C：静态变量
来源：http://zab.316326.xyz

static int counter = 0;
来源：http://spf.cdnleiting.top

[S29] C：变参函数
来源：http://bni.zhixingplan.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://frw.hnqzz.top

[S30] C：头文件保护
来源：http://wrh.sufxvd.cn

#ifndef X_H
来源：http://oiv.52xcode.cn

#define X_H
来源：http://trw.pycfn.com

#endif
来源：http://ncc.uphjek.com

[S31] C++：Hello World
来源：http://bnu.hnxiangtu.top

#include <iostream>
来源：http://dmt.nanxinkj.top

int main() { std::cout << "Hello\n"; }
来源：http://jfk.zycfv.cn

[S32] C++：字符串
来源：http://ljx.hfpthk.cn

std::string s = "hi";  s += "!";
来源：http://nnj.bbcook.cn

[S33] C++：vector 增删
来源：http://sxb.iojbl.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ndx.hnqzz.top

[S34] C++：遍历 vector
来源：http://nrh.ybcxt.top

for (auto &x : v) { std::cout << x; }
来源：http://vxy.xuanzx.com

[S35] C++：map
来源：http://nud.iojbl.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uzy.havefunace.top

[S36] C++：unordered_map
来源：http://isf.gaohongyu789.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fda.sxryk.cn

[S37] C++：set
来源：http://wrx.ctjpmb.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wbd.snrcjt.cn

[S38] C++：排序
来源：http://bov.hnxiangtu.top

std::sort(v.begin(), v.end());
来源：http://lvl.mhx1999.top

[S39] C++：自定义比较器排序
来源：http://ufx.ppjwa.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qgw.svipenyu.cn

[S40] C++：查找元素
来源：http://tji.kuanghao11.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xet.sysykeji.top

[S41] C++：类与构造函数
来源：http://tcp.feifeiyinyue.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uoh.cucudq.cn

[S42] C++：继承与虚函数
来源：http://dss.cashguo.top

class B : public Base { public: void f() override {} };
来源：http://vwq.hcnkem.com

[S43] C++：智能指针
来源：http://isy.yuxming.cn

auto p = std::make_unique<int>(5);
来源：http://xhd.sweek.top

[S44] C++：引用传参
来源：http://yke.sufxvd.cn

void inc(int &x) { ++x; }
来源：http://ehy.zhongyouzk.top

[S45] C++：lambda
来源：http://ooz.zdqjudy.top

auto add = [](int a, int b) { return a + b; };
来源：http://msf.jinyuanbaomall.cn

[S46] C++：函数模板
来源：http://ucy.ehwqpu.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vkn.tian-w.cn

[S47] C++：结构化绑定遍历
来源：http://pzm.dianchejie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bcj.sysykeji.top

[S48] C++：逐行读文件
来源：http://ekk.cashguo.top

std::ifstream in("a.txt");  std::string line;
来源：http://owg.fzhhl.top

while (std::getline(in, line)) { }
来源：http://vvy.ybcxt.top

[S49] C++：写文件
来源：http://rje.kuanghao11.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eui.ppjwa.cn

[S50] C++：格式化数字
来源：http://hjj.mhx1999.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zha.sysykeji.top

[S51] C++：显式类型转换
来源：http://stp.chenzaomai.com

static_cast<double>(a) / b
来源：http://bwi.hywenlv.cn

[S52] C++：const 与 noexcept
来源：http://prw.hesvh.cn

int size() const noexcept { return n_; }
来源：http://pdm.hcnkem.com

[S53] C++：移动语义
来源：http://whj.nwbrower.top

std::vector<int> w = std::move(v);
来源：http://gaw.snrcjt.cn

[S54] C++：异常处理
来源：http://grf.316326.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://euw.zhijiandao.cn

[S55] C++：结构化绑定
来源：http://ico.epnwcf.com

auto [a, b] = std::make_pair(1, 2);
来源：http://uxd.shangyingyoupin.top

[S56] C++：optional
来源：http://pnb.iojbl.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zcb.hnqzz.top

[S57] C++：编译期常量
来源：http://ekx.jqgufenzy.top

constexpr int N = 10;
来源：http://vzg.dashuyun.cn

[S58] C++：命名空间
来源：http://pjb.jiagoushi.top

namespace ns { int f() { return 1; } }
来源：http://tsf.uphjek.com

[S59] C++：静态断言
来源：http://nsj.snrcjt.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oqy.ydjk.org.cn

[S60] C++：遍历并删除元素
来源：http://heg.hnqzz.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://izh.jinqigufen.top

================================================================================
来源：http://mib.fengsongda.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uoa.gzhubu.top

================================================================================
来源：http://bwg.vehdjk.com

[T01] Kotlin：Hello World
来源：http://ewg.dashuyun.cn

println("Hello")
来源：http://wtm.cucudq.cn

[T02] Kotlin：变量
来源：http://jdj.hammf.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://adj.0kj1m.cn

[T03] Kotlin：字符串模板
来源：http://cib.0kj1m.cn

"值: $b"
来源：http://lwm.yuanzhike.top

[T04] Kotlin：空安全
来源：http://ppn.hesvh.cn

val n: String? = null;  n?.length
来源：http://qit.yfazqb.com

[T05] Kotlin：when 表达式
来源：http://hhf.smart0.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ukk.fehbvm.com

[T06] Kotlin：集合映射
来源：http://eze.zhengqikj.top

listOf(1, 2, 3).map { it * 2 }
来源：http://fqy.shzxlz.cn

[T07] Kotlin：集合过滤
来源：http://tff.fzhhl.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://cgf.c1oappe.top

[T08] Kotlin：数据类
来源：http://jbx.iojbl.cn

data class User(val name: String, val age: Int)
来源：http://rua.guowangkeji.top

[T09] Kotlin：扩展函数
来源：http://zlh.daxiang520.top

fun String.exclaim() = this + "!"
来源：http://gki.zdqjudy.top

[T10] Kotlin：默认参数
来源：http://yfr.mhx1999.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wvg.zhijiandao.cn

[T11] Kotlin：协程
来源：http://lqw.yj20258.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mlk.nanxinkj.top

[T12] Kotlin：解构声明
来源：http://bgx.xylfe.cn

val (a, b) = Pair(1, 2)
来源：http://pla.mhx1999.top

[T13] Kotlin：只读 Map
来源：http://rtx.zhiwuduotai.top

val m = mapOf("a" to 1)
来源：http://fsm.yueranfly.top

[T14] Kotlin：循环
来源：http://mhc.zhoulong.xyz

for (i in 1..10) println(i)
来源：http://ock.daxiang520.top

[T15] Kotlin：接口
来源：http://olc.fanxiaobao.xyz

interface Shape { fun area(): Double }
来源：http://djg.jyoumei.cn

[T16] Swift：Hello World
来源：http://zsu.zhongyouzk.top

print("Hello")
来源：http://krb.quarkkingdee.top

[T17] Swift：变量与常量
来源：http://qmv.feifeiyinyue.top

var a = 1;  let b = 2
来源：http://diu.ywan-chungtsiang.top

[T18] Swift：字符串插值
来源：http://cff.zhoulong.xyz

"值: \(b)"
来源：http://vwr.vehdjk.com

[T19] Swift：可选绑定
来源：http://fdw.hongshengwenyu.top

if let n = opt { print(n) }
来源：http://rqc.jinqigufen.top

[T20] Swift：数组操作
来源：http://amo.hnxiangtu.top

var a = [1, 2, 3];  a.append(4)
来源：http://yzy.shanyushiyangtech.top

[T21] Swift：遍历
来源：http://xqf.yuxming.cn

for x in a { print(x) }
来源：http://hoj.yj202588.top

[T22] Swift：字典
来源：http://nfx.dianchejie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cfr.chenjidiqi.icu

[T23] Swift：函数
来源：http://oba.fengsongda.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://twl.gotoacloud.top

[T24] Swift：闭包
来源：http://oqe.shzxlz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://nnn.quarkkingdee.top

[T25] Swift：结构体
来源：http://nls.shangyingyoupin.top

struct P { var x: Int }
来源：http://zal.fengsongda.top

[T26] Swift：类与重写
来源：http://qre.ivvv.top

class A: Base { override func f() {} }
来源：http://twe.fengsongda.top

[T27] Swift：错误处理
来源：http://enc.zycfv.cn

do { try f() } catch { print(error) }
来源：http://vud.jinyuanbaomall.cn

[T28] Swift：枚举
来源：http://iti.xziqi.cn

enum Color { case red, green }
来源：http://cap.chenzaomai.com

[T29] Swift：guard 提前返回
来源：http://swe.cdnleiting.top

guard let x = opt else { return }
来源：http://gkd.smart0.xyz

[T30] Swift：协议
来源：http://hjh.yj20258888.top

protocol Shape { func area() -> Double }
来源：http://pfh.yueranfly.top

[T31] Lua：Hello World
来源：http://rxd.cashguo.top

print("Hello")
来源：http://wpz.ywan-chungtsiang.top

[T32] Lua：局部变量
来源：http://frg.hcnkem.com

local a = 1
来源：http://kmx.wangdashe.top

[T33] Lua：表（数组）
来源：http://qwh.vqdsnc.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wxu.sufxvd.cn

[T34] Lua：遍历表
来源：http://sxy.ybcxt.top

for i, v in ipairs(t) do print(i, v) end
来源：http://lwa.iojbl.cn


<!-- 参考信息 -->