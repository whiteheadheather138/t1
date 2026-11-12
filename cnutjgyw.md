代发 wailian999

echo $((1 + 2 * 3))
来源：http://myz.cucudq.cn

[R28] 浮点运算
来源：http://cad.fanxiaobao.xyz

echo "scale=2; 10/3" | bc
来源：http://kgr.snrcjt.cn

[R29] 定义函数
来源：http://idj.9152youxi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lqy.kuanghao11.cn

[R30] 函数返回状态码
来源：http://nyv.zdqjudy.top

f() { return 0; }; f || echo "失败了"
来源：http://sfz.sufxvd.cn

[R31] 局部变量
来源：http://ygz.quarkkingdee.top

f() { local x=1; echo "$x"; }
来源：http://bhd.yj20258888.top

[R32] 参数个数校验
来源：http://uru.cheryme.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://brz.ydjk.org.cn

[R33] 捕获错误并提示行号
来源：http://sos.pengpengdd.cyou

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cxv.meibo888.top

[R34] 退出时清理
来源：http://txg.yvedp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ogq.zhengqikj.top

[R35] 后台执行并等待
来源：http://eqs.chenzaomai.com

sleep 5 & pid=$!; wait "$pid"
来源：http://ciz.nwbrower.top

[R36] 并发执行多个任务
来源：http://xan.shzxlz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bbf.cheryme.top

[R37] 把输出赋给变量
来源：http://cmb.yongpay.top

files=$(ls -1)
来源：http://npm.gzhubu.top

[R38] 管道串联
来源：http://opa.redwolf501.top

cat a.txt | grep -i error | wc -l
来源：http://vqx.sweek.top

[R39] 重定向标准输出与错误
来源：http://nyq.iojbl.cn

cmd > out.log 2>&1
来源：http://bpy.ywan-chungtsiang.top

[R40] 追加写日志
来源：http://rup.zhaomingkeji.xyz

echo "log" >> out.log
来源：http://fyi.chenjidiqi.icu

[R41] 丢弃输出
来源：http://qeh.sweek.top

cmd >/dev/null 2>&1
来源：http://cgq.jianghu66.top

[R42] 输入重定向
来源：http://yoa.hammf.cn

wc -l < a.txt
来源：http://qpk.hongshengwenyu.top

[R43] 按名字查找文件
来源：http://sce.gaohongyu789.top

find . -name "*.log" -type f
来源：http://zgc.sysykeji.top

[R44] 按修改时间查找
来源：http://wqy.zdbjq.cn

find . -mtime -7 -type f
来源：http://rby.zycfv.cn

[R45] 批量删除
来源：http://bcf.uphjek.com

find . -name "*.tmp" -delete
来源：http://lrj.jinqigfzy.top

[R46] 递归替换文件内容
来源：http://yym.cashguo.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dmb.mhx1999.top

[R47] sed 单行替换
来源：http://joh.chenlongwang.top

sed -i 's/foo/bar/g' a.txt
来源：http://ymp.c1oappe.top

[R48] awk 取指定列
来源：http://zfx.hnxiangtu.top

awk '{print $1, $3}' a.txt
来源：http://nzr.tanke756.top

[R49] awk 带条件
来源：http://gzb.fzhhl.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://buk.hnxiangtu.top

[R50] awk 求和
来源：http://cft.gogol.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qyk.shanyushiyangtech.top

[R51] 排序去重取前几
来源：http://cra.meibo888.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ghv.sysykeji.top

[R52] 统计行数
来源：http://rtf.tanke756.top

wc -l a.txt
来源：http://oyb.vehdjk.com

[R53] 查看文件头与实时尾
来源：http://mgb.kuanghao11.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kxj.shuidangran.top

[R54] 比较两个文件
来源：http://mko.havefunace.top

diff a.txt b.txt
来源：http://vxv.cashguo.top

[R55] 压缩与解压
来源：http://zri.chenjidiqi.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ndx.hysaishi.cn

[R56] 远程拷贝
来源：http://rod.guowangkeji.top

scp file user@host:/path/
来源：http://lnv.aibaodan.cn

[R57] 远程执行命令
来源：http://spq.bbcook.cn

ssh user@host 'uptime'
来源：http://omu.jiagoushi.top

[R58] 下载文件
来源：http://bhv.sweek.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xxe.zhoulong.xyz

[R59] 发 POST JSON
来源：http://ezc.zhoulong.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://iss.gaohongyu789.top

[R60] 只看 HTTP 状态码
来源：http://vis.redwolf501.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://efy.feifeiyinyue.top

[R61] 磁盘占用
来源：http://flh.ydjk.org.cn

df -h;  du -sh *
来源：http://bmf.feifeiyinyue.top

[R62] 找最占空间的文件
来源：http://vhq.daria6918.cn

du -ah . | sort -rh | head -10
来源：http://bcc.hysaishi.cn

[R63] 内存与进程
来源：http://jtw.svipenyu.cn

free -h;  ps aux | grep nginx
来源：http://hwa.zhoulong.xyz

[R64] 结束进程
来源：http://mva.ivvv.top

kill -9 $(pgrep -f app.py)
来源：http://qpn.gaohongyu789.top

[R65] 查看端口占用
来源：http://obu.cqqwz.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://muq.bbcook.cn

[R66] 定时任务
来源：http://xbl.zhijiandao.cn

crontab -e;  crontab -l
来源：http://wvz.xingfuxueyuan.xyz

[R67] 生成随机十六进制串
来源：http://tpu.yuxming.cn

openssl rand -hex 16
来源：http://eky.yj20258888.top

[R68] 计算文件校验值
来源：http://elo.cucudq.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gwt.52xcode.cn

[R69] 生成随机密码
来源：http://eew.epnwcf.com

head -c 16 /dev/urandom | base64
来源：http://wwh.vqdsnc.cn

[R70] 时间戳与互转
来源：http://qxm.hnxiangtu.top

date +%s;  date -d @1700000000
来源：http://sui.xziqi.cn

[R71] 日期格式化
来源：http://ubm.xziqi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dld.bbcook.cn

[R72] 等待端口就绪
来源：http://kzt.jinqigufen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://bnq.pycfn.com

[R73] 分割大日志
来源：http://pcw.zhongyouzk.top

split -l 1000 big.log part_
来源：http://dqw.ehwqpu.com

[R74] 批量重命名
来源：http://ujz.nanxinkj.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fhq.svipenyu.cn

[R75] 导出环境变量
来源：http://ubg.daxiang520.top

export PATH="$HOME/bin:$PATH"
来源：http://nfo.ybcxt.top

[R76] 使用临时文件
来源：http://bnd.0kj1m.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://llo.jyoumei.cn

[R77] 读取用户输入
来源：http://tdu.sweek.top

read -rp "请输入: " ans
来源：http://dlw.xuanzx.com

[R78] 交互式菜单
来源：http://mbr.zdqjudy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rpj.shzxlz.cn

[R79] 解析命令行选项
来源：http://aph.xingfuxueyuan.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ebb.316326.xyz

[R80] 查看脚本执行耗时
来源：http://pns.havefunace.top

time ./run.sh
来源：http://lhl.yj202588.top

================================================================================
来源：http://tuc.andypj.xyz

S. C / C++ 专题
来源：http://fis.chenjidiqi.icu

================================================================================
来源：http://qjk.fktsv.cn

[S01] C：Hello World
来源：http://ucd.xuanzx.com

#include <stdio.h>
来源：http://mvb.ydjk.org.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hna.fanxiaobao.xyz

[S02] C：变量与格式化输出
来源：http://vnm.xylfe.cn

int a = 10; printf("%d\n", a);
来源：http://tre.gotoacloud.top

[S03] C：读入整数
来源：http://jxo.nwbrower.top

int x; scanf("%d", &x);
来源：http://nyg.jiagoushi.top

[S04] C：字符串复制
来源：http://ifa.hysaishi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mva.yangfankeji.com

[S05] C：字符串长度
来源：http://xjx.jlsjyb.cn

strlen(s)
来源：http://zpo.uphjek.com

[S06] C：字符串比较
来源：http://aua.tianlin.xyz

strcmp(a, b) == 0
来源：http://ydh.smart0.xyz

[S07] C：数组遍历求和
来源：http://lqw.jyoumei.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cef.cheryme.top

[S08] C：动态内存分配与释放
来源：http://vcb.jiagoushi.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lrg.sufxvd.cn

[S09] C：结构体定义与初始化
来源：http://zal.ydzc1.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mgz.wangshuangyany.cn

[S10] C：指针与解引用
来源：http://taa.sysykeji.top

int *p = &a;  *p = 5;
来源：http://tcf.ctjpmb.com

[S11] C：逐行读文件
来源：http://fwv.bjfxy.top

FILE *f = fopen("a.txt", "r");
来源：http://gcl.ydjk.org.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://psf.vqdsnc.cn

fclose(f);
来源：http://ecf.redwolf501.top

[S12] C：写文件
来源：http://ewa.hongshengwenyu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jrl.gaohongyu789.top

[S13] C：宏定义
来源：http://ciq.zhaomingkeji.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mcr.zhaomingkeji.xyz

[S14] C：枚举
来源：http://epk.zhijiandao.cn

enum Color { RED, GREEN, BLUE };
来源：http://mmk.tarul.cn

[S15] C：类型转换
来源：http://kyd.yj202588.top

(double) a / b
来源：http://fgn.mhx1999.top

[S16] C：位操作置位
来源：http://gzg.zdqjudy.top

x |= (1 << 3);
来源：http://tve.snrcjt.cn

[S17] C：安全拼接字符串
来源：http://thd.hesvh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yhq.guannengcc.top

[S18] C：命令行参数
来源：http://ayf.tianlin.xyz

int main(int argc, char **argv)
来源：http://umq.tian-w.cn

[S19] C：快速排序
来源：http://vgi.fzhhl.top

qsort(a, n, sizeof(int), cmp);
来源：http://blf.ybcxt.top

[S20] C：二分查找
来源：http://gej.yuxming.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://umu.jianghu66.top

[S21] C：字符类别判断
来源：http://wkv.gogol.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vvf.zycfv.cn

[S22] C：字符串转数字
来源：http://gfb.chenjidiqi.icu

atoi("42");  strtod("3.14", NULL);
来源：http://hbz.haohaochexian.top

[S23] C：随机数
来源：http://wnm.ybcxt.top

srand(time(NULL));  int r = rand() % 100;
来源：http://wde.zycfv.cn

[S24] C：获取本地时间
来源：http://bmh.gotoacloud.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jbx.gogol.net.cn

[S25] C：内存拷贝
来源：http://gkd.vehdjk.com

memcpy(dst, src, n);
来源：http://kkn.tarul.cn

[S26] C：内存清零
来源：http://tbr.bbcook.cn

memset(a, 0, sizeof a);
来源：http://esq.hongshengwenyu.top

[S27] C：定义常量
来源：http://pgh.c1oappe.top

const double PI = 3.14159;
来源：http://bqf.zhongyouzk.top

[S28] C：静态变量
来源：http://afv.316326.xyz

static int counter = 0;
来源：http://qta.yueranfly.top

[S29] C：变参函数
来源：http://tsc.ybcxt.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cnf.iojbl.cn

[S30] C：头文件保护
来源：http://wkd.dashuyun.cn

#ifndef X_H
来源：http://qpi.52xcode.cn

#define X_H
来源：http://mnj.shanyushiyangtech.top

#endif
来源：http://nfz.havefunace.top

[S31] C++：Hello World
来源：http://kix.yj20258888.top

#include <iostream>
来源：http://esq.ywan-chungtsiang.top

int main() { std::cout << "Hello\n"; }
来源：http://vdt.gaohongyu789.top

[S32] C++：字符串
来源：http://gwu.c1oappe.top

std::string s = "hi";  s += "!";
来源：http://vsl.nanxinkj.top

[S33] C++：vector 增删
来源：http://iwo.andypj.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xgp.meibo888.top

[S34] C++：遍历 vector
来源：http://fax.xziqi.cn

for (auto &x : v) { std::cout << x; }
来源：http://pmj.daxiang520.top

[S35] C++：map
来源：http://lui.yangfankeji.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lwf.jinyuanbaomall.cn

[S36] C++：unordered_map
来源：http://jdy.yj202588.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://auz.tarul.cn

[S37] C++：set
来源：http://xkv.hywenlv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pon.hongshengwenyu.top

[S38] C++：排序
来源：http://jnr.zycfv.cn

std::sort(v.begin(), v.end());
来源：http://ecu.zdbjq.cn

[S39] C++：自定义比较器排序
来源：http://jxb.jqgufenzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://utj.nwbrower.top

[S40] C++：查找元素
来源：http://cvp.cdnleiting.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://njx.yongpay.top

[S41] C++：类与构造函数
来源：http://gde.xuetiantiany.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://noh.zhaomingkeji.xyz

[S42] C++：继承与虚函数
来源：http://ing.zdbjq.cn

class B : public Base { public: void f() override {} };
来源：http://pbd.hfpthk.cn

[S43] C++：智能指针
来源：http://gzk.havefunace.top

auto p = std::make_unique<int>(5);
来源：http://btc.pycfn.com

[S44] C++：引用传参
来源：http://mqz.nanxinkj.top

void inc(int &x) { ++x; }
来源：http://sal.nanxinkj.top

[S45] C++：lambda
来源：http://dbg.jqgfzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://icq.fehbvm.com

[S46] C++：函数模板
来源：http://mxr.jqgufenzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jmn.nanxinkj.top

[S47] C++：结构化绑定遍历
来源：http://csm.yonumen.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ouk.ydjk.org.cn

[S48] C++：逐行读文件
来源：http://nun.hnxiangtu.top

std::ifstream in("a.txt");  std::string line;
来源：http://zyh.yvedp.cn

while (std::getline(in, line)) { }
来源：http://bvi.jyoumei.cn

[S49] C++：写文件
来源：http://gem.ppjwa.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dbc.pycfn.com

[S50] C++：格式化数字
来源：http://dbk.nanxuanxn.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://djq.sxryk.cn

[S51] C++：显式类型转换
来源：http://vee.tian-w.cn

static_cast<double>(a) / b
来源：http://swv.gotoacloud.top

[S52] C++：const 与 noexcept
来源：http://hun.fzhhl.top

int size() const noexcept { return n_; }
来源：http://cxh.feifeiyinyue.top

[S53] C++：移动语义
来源：http://bkz.zhaomingkeji.xyz

std::vector<int> w = std::move(v);
来源：http://fyb.aizwys.cn

[S54] C++：异常处理
来源：http://sxj.hongshengwenyu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cds.zhaomingkeji.xyz

[S55] C++：结构化绑定
来源：http://rqp.shangyingyoupin.top

auto [a, b] = std::make_pair(1, 2);
来源：http://rhc.jyoumei.cn

[S56] C++：optional
来源：http://fxa.dianchejie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vyr.wangshuangyany.cn

[S57] C++：编译期常量
来源：http://tld.cdnleiting.top

constexpr int N = 10;
来源：http://aqa.birdmap.top

[S58] C++：命名空间
来源：http://muf.c1oappe.top

namespace ns { int f() { return 1; } }
来源：http://qdf.chenzaomai.com

[S59] C++：静态断言
来源：http://okv.epnwcf.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tdz.9152youxi.cn

[S60] C++：遍历并删除元素
来源：http://lle.xuetiantiany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zqw.hywenlv.cn

================================================================================
来源：http://msy.jqgufenzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nex.jinqigfzy.top

================================================================================
来源：http://uvx.shangyingyoupin.top

[T01] Kotlin：Hello World
来源：http://unz.gaohongyu789.top

println("Hello")
来源：http://vrm.svipenyu.cn

[T02] Kotlin：变量
来源：http://zej.iojbl.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sjb.hnxiangtu.top

[T03] Kotlin：字符串模板
来源：http://udf.hammf.cn

"值: $b"
来源：http://nsz.snrcjt.cn

[T04] Kotlin：空安全
来源：http://ixe.fktsv.cn

val n: String? = null;  n?.length
来源：http://anm.hfpthk.cn

[T05] Kotlin：when 表达式
来源：http://sjs.havefunace.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://oyr.jinqigfzy.top

[T06] Kotlin：集合映射
来源：http://afk.xziqi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zuy.hammf.cn

[T07] Kotlin：集合过滤
来源：http://dnj.cheryme.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vbb.zhaomingkeji.xyz

[T08] Kotlin：数据类
来源：http://kcq.shzxlz.cn

data class User(val name: String, val age: Int)
来源：http://imt.sjlbkw.cn

[T09] Kotlin：扩展函数
来源：http://uka.redwolf501.top

fun String.exclaim() = this + "!"
来源：http://bpr.andypj.xyz

[T10] Kotlin：默认参数
来源：http://ufn.xuanzx.com

fun greet(name: String = "World") = "Hi $name"
来源：http://llm.nwbrower.top

[T11] Kotlin：协程
来源：http://haa.yanxiufei.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bbf.xingfuxueyuan.xyz

[T12] Kotlin：解构声明
来源：http://snk.zdbjq.cn

val (a, b) = Pair(1, 2)
来源：http://hef.daxiang520.top

[T13] Kotlin：只读 Map
来源：http://iml.cheryme.top

val m = mapOf("a" to 1)
来源：http://wdx.aibaodan.cn

[T14] Kotlin：循环
来源：http://udf.feifeiyinyue.top

for (i in 1..10) println(i)
来源：http://qvy.nwbrower.top

[T15] Kotlin：接口
来源：http://vod.sjlbkw.cn

interface Shape { fun area(): Double }
来源：http://quq.fanxiaobao.xyz

[T16] Swift：Hello World
来源：http://yvh.zdqjudy.top

print("Hello")
来源：http://qje.zhiwuduotai.top

[T17] Swift：变量与常量
来源：http://hdx.uphjek.com

var a = 1;  let b = 2
来源：http://hou.9152youxi.cn

[T18] Swift：字符串插值
来源：http://urc.yueranfly.top

"值: \(b)"
来源：http://xgn.yvedp.cn

[T19] Swift：可选绑定
来源：http://esb.daria6918.cn

if let n = opt { print(n) }
来源：http://rzq.yangfankeji.com

[T20] Swift：数组操作
来源：http://wvz.sysykeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://kwj.hfpthk.cn

[T21] Swift：遍历
来源：http://ehg.birdmap.top

for x in a { print(x) }
来源：http://yzw.xingfuxueyuan.xyz

[T22] Swift：字典
来源：http://cup.zhiwuduotai.top

var d = ["a": 1];  d["b"] = 2
来源：http://rrr.mhx1999.top

[T23] Swift：函数
来源：http://iei.jinyuanbaomall.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ppr.snrcjt.cn

[T24] Swift：闭包
来源：http://qmd.yuanzhike.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://epp.quarkkingdee.top

[T25] Swift：结构体
来源：http://zsl.aibaodan.cn

struct P { var x: Int }
来源：http://chb.ctjpmb.com

[T26] Swift：类与重写
来源：http://lar.yanxiufei.cn

class A: Base { override func f() {} }
来源：http://oyb.bbcook.cn

[T27] Swift：错误处理
来源：http://spm.hnxiangtu.top

do { try f() } catch { print(error) }
来源：http://tpy.zhijiandao.cn

[T28] Swift：枚举
来源：http://wpg.gotoacloud.top

enum Color { case red, green }
来源：http://vcu.ydzc1.top

[T29] Swift：guard 提前返回
来源：http://buo.snrcjt.cn

guard let x = opt else { return }
来源：http://syx.zhengqikj.top

[T30] Swift：协议
来源：http://mmk.shanyushiyangkeji.top

protocol Shape { func area() -> Double }
来源：http://xos.cheryme.top


<!-- 参考信息 -->