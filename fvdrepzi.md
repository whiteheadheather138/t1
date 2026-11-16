代发 wailian999

echo $((1 + 2 * 3))
来源：http://dvj.yuanzhike.top

[R28] 浮点运算
来源：http://ech.hesvh.cn

echo "scale=2; 10/3" | bc
来源：http://qdj.jinqigufen.top

[R29] 定义函数
来源：http://kmf.sysykeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qgb.vqdsnc.cn

[R30] 函数返回状态码
来源：http://hdr.gzhubu.top

f() { return 0; }; f || echo "失败了"
来源：http://yzr.yj20258888.top

[R31] 局部变量
来源：http://tkw.zhengqikj.top

f() { local x=1; echo "$x"; }
来源：http://hwv.snrcjt.cn

[R32] 参数个数校验
来源：http://ial.yj20258.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yuy.zdbjq.cn

[R33] 捕获错误并提示行号
来源：http://zle.yuxming.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://iiq.yueranfly.top

[R34] 退出时清理
来源：http://eps.pengpengdd.cyou

trap 'rm -f "$tmp"' EXIT
来源：http://emj.hysaishi.cn

[R35] 后台执行并等待
来源：http://hse.jianghu66.top

sleep 5 & pid=$!; wait "$pid"
来源：http://txe.quarkkingdee.top

[R36] 并发执行多个任务
来源：http://rox.316326.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pdh.ydjk.org.cn

[R37] 把输出赋给变量
来源：http://jyt.wangshuangyany.cn

files=$(ls -1)
来源：http://ilq.yueranfly.top

[R38] 管道串联
来源：http://fkp.wangshuangyany.cn

cat a.txt | grep -i error | wc -l
来源：http://vsp.fktsv.cn

[R39] 重定向标准输出与错误
来源：http://dad.gaohongyu789.top

cmd > out.log 2>&1
来源：http://sfj.cashguo.top

[R40] 追加写日志
来源：http://duo.pycfn.com

echo "log" >> out.log
来源：http://whq.aizwys.cn

[R41] 丢弃输出
来源：http://ugw.shzxlz.cn

cmd >/dev/null 2>&1
来源：http://ysb.nanxinkj.top

[R42] 输入重定向
来源：http://xti.havefunace.top

wc -l < a.txt
来源：http://obh.smart0.xyz

[R43] 按名字查找文件
来源：http://xer.kuanghao11.cn

find . -name "*.log" -type f
来源：http://lgu.guowangkeji.top

[R44] 按修改时间查找
来源：http://aan.chenjidiqi.icu

find . -mtime -7 -type f
来源：http://qej.jqgufenzy.top

[R45] 批量删除
来源：http://oto.wangdashe.top

find . -name "*.tmp" -delete
来源：http://cgc.shzxlz.cn

[R46] 递归替换文件内容
来源：http://yjw.zhijiandao.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rxd.jinqigfzy.top

[R47] sed 单行替换
来源：http://xby.zhiwuduotai.top

sed -i 's/foo/bar/g' a.txt
来源：http://mei.zhijiandao.cn

[R48] awk 取指定列
来源：http://uus.pengpengdd.cyou

awk '{print $1, $3}' a.txt
来源：http://fhz.jiagoushi.top

[R49] awk 带条件
来源：http://ytb.quarkkingdee.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://aol.ybcxt.top

[R50] awk 求和
来源：http://vah.mhx1999.top

awk '{s += $2} END {print s}' a.txt
来源：http://eeo.316326.xyz

[R51] 排序去重取前几
来源：http://csk.sysykeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://usq.hongshengwenyu.top

[R52] 统计行数
来源：http://aif.cashguo.top

wc -l a.txt
来源：http://azz.gzhubu.top

[R53] 查看文件头与实时尾
来源：http://xge.jiagoushi.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yzk.ppjwa.cn

[R54] 比较两个文件
来源：http://qdn.jyoumei.cn

diff a.txt b.txt
来源：http://nmv.xuetiantiany.cn

[R55] 压缩与解压
来源：http://jwk.zhiwuduotai.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ybu.shanyushiyangtech.top

[R56] 远程拷贝
来源：http://czc.zdqjudy.top

scp file user@host:/path/
来源：http://zft.chenzaomai.com

[R57] 远程执行命令
来源：http://obp.yonumen.top

ssh user@host 'uptime'
来源：http://acc.shuidangran.top

[R58] 下载文件
来源：http://ode.yj20258888.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cta.yj202588.top

[R59] 发 POST JSON
来源：http://zba.yuxming.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oft.xylfe.cn

[R60] 只看 HTTP 状态码
来源：http://rva.jiagoushi.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vmj.jianghu66.top

[R61] 磁盘占用
来源：http://kap.xuetiantiany.cn

df -h;  du -sh *
来源：http://ofc.yanxiufei.cn

[R62] 找最占空间的文件
来源：http://znf.ivvv.top

du -ah . | sort -rh | head -10
来源：http://fiu.cdnleiting.top

[R63] 内存与进程
来源：http://bqq.jinghuilouyu.cn

free -h;  ps aux | grep nginx
来源：http://qet.hcnkem.com

[R64] 结束进程
来源：http://xxg.c1oappe.top

kill -9 $(pgrep -f app.py)
来源：http://svb.gotoacloud.top

[R65] 查看端口占用
来源：http://mcq.gaohongyu789.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oxh.dianchejie.cn

[R66] 定时任务
来源：http://utg.gogol.net.cn

crontab -e;  crontab -l
来源：http://vhh.shuidangran.top

[R67] 生成随机十六进制串
来源：http://hfy.zycfv.cn

openssl rand -hex 16
来源：http://duc.pengpengdd.cyou

[R68] 计算文件校验值
来源：http://vqy.shzxlz.cn

sha256sum a.txt;  md5sum a.txt
来源：http://snb.ivvv.top

[R69] 生成随机密码
来源：http://qui.yj20258.top

head -c 16 /dev/urandom | base64
来源：http://dbj.cucudq.cn

[R70] 时间戳与互转
来源：http://ywf.tanke756.top

date +%s;  date -d @1700000000
来源：http://bti.fanxiaobao.xyz

[R71] 日期格式化
来源：http://mfl.yanxiufei.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xnc.hcnkem.com

[R72] 等待端口就绪
来源：http://uee.jianghu66.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nlk.0kj1m.cn

[R73] 分割大日志
来源：http://wxt.ydzc1.top

split -l 1000 big.log part_
来源：http://avm.xziqi.cn

[R74] 批量重命名
来源：http://gmt.tianlin.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://brb.tarul.cn

[R75] 导出环境变量
来源：http://szs.0kj1m.cn

export PATH="$HOME/bin:$PATH"
来源：http://dem.andypj.xyz

[R76] 使用临时文件
来源：http://mka.yvedp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lrl.epnwcf.com

[R77] 读取用户输入
来源：http://tpb.wangshuangyany.cn

read -rp "请输入: " ans
来源：http://rul.chenjidiqi.icu

[R78] 交互式菜单
来源：http://zhu.yfazqb.com

select opt in a b c; do echo "$opt"; break; done
来源：http://qib.hnqzz.top

[R79] 解析命令行选项
来源：http://tnt.gotoacloud.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://woc.jiagoushi.top

[R80] 查看脚本执行耗时
来源：http://mjh.feifeiyinyue.top

time ./run.sh
来源：http://und.chenzaomai.com

================================================================================
来源：http://xvj.hywenlv.cn

S. C / C++ 专题
来源：http://htw.ydjk.org.cn

================================================================================
来源：http://avu.tianlin.xyz

[S01] C：Hello World
来源：http://ufh.mhx1999.top

#include <stdio.h>
来源：http://wuh.yueranfly.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://knc.ctjpmb.com

[S02] C：变量与格式化输出
来源：http://inw.hnqzz.top

int a = 10; printf("%d\n", a);
来源：http://fde.yfazqb.com

[S03] C：读入整数
来源：http://zae.hammf.cn

int x; scanf("%d", &x);
来源：http://wnz.316326.xyz

[S04] C：字符串复制
来源：http://efs.316326.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://biw.havefunace.top

[S05] C：字符串长度
来源：http://evq.ybcxt.top

strlen(s)
来源：http://vtz.yuxming.cn

[S06] C：字符串比较
来源：http://iys.sufxvd.cn

strcmp(a, b) == 0
来源：http://spn.redwolf501.top

[S07] C：数组遍历求和
来源：http://vas.zhoulong.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ofo.gaohongyu789.top

[S08] C：动态内存分配与释放
来源：http://hrb.xziqi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://klw.hfpthk.cn

[S09] C：结构体定义与初始化
来源：http://ntt.aibaodan.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vor.cashguo.top

[S10] C：指针与解引用
来源：http://qex.0kj1m.cn

int *p = &a;  *p = 5;
来源：http://vpw.zhengqikj.top

[S11] C：逐行读文件
来源：http://dvl.sweek.top

FILE *f = fopen("a.txt", "r");
来源：http://gag.ctjpmb.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://ixu.yangfankeji.com

fclose(f);
来源：http://vzq.316326.xyz

[S12] C：写文件
来源：http://ulg.nwbrower.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xde.yfazqb.com

[S13] C：宏定义
来源：http://dwr.havefunace.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dcx.quarkkingdee.top

[S14] C：枚举
来源：http://lwp.zycfv.cn

enum Color { RED, GREEN, BLUE };
来源：http://kzm.gotoacloud.top

[S15] C：类型转换
来源：http://vxy.havefunace.top

(double) a / b
来源：http://pkf.ywan-chungtsiang.top

[S16] C：位操作置位
来源：http://wck.chenzaomai.com

x |= (1 << 3);
来源：http://qll.yueranfly.top

[S17] C：安全拼接字符串
来源：http://nhy.hywenlv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://col.gotoacloud.top

[S18] C：命令行参数
来源：http://bnt.hywenlv.cn

int main(int argc, char **argv)
来源：http://gvn.ivvv.top

[S19] C：快速排序
来源：http://rvr.zycfv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cog.xingfuxueyuan.xyz

[S20] C：二分查找
来源：http://jrh.yfazqb.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rjv.yfazqb.com

[S21] C：字符类别判断
来源：http://fym.ehwqpu.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dev.hcnkem.com

[S22] C：字符串转数字
来源：http://ygt.dianchejie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jgn.nanxinkj.top

[S23] C：随机数
来源：http://noh.chenzaomai.com

srand(time(NULL));  int r = rand() % 100;
来源：http://cjw.ppjwa.cn

[S24] C：获取本地时间
来源：http://fiq.haohaochexian.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dri.fehbvm.com

[S25] C：内存拷贝
来源：http://gpo.tanke756.top

memcpy(dst, src, n);
来源：http://xdg.zhijiandao.cn

[S26] C：内存清零
来源：http://qdu.sjlbkw.cn

memset(a, 0, sizeof a);
来源：http://rys.quarkkingdee.top

[S27] C：定义常量
来源：http://uev.cheryme.top

const double PI = 3.14159;
来源：http://xku.nanxinkj.top

[S28] C：静态变量
来源：http://jll.9152youxi.cn

static int counter = 0;
来源：http://tlv.sufxvd.cn

[S29] C：变参函数
来源：http://lon.zhixingplan.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xai.vehdjk.com

[S30] C：头文件保护
来源：http://fxj.iojbl.cn

#ifndef X_H
来源：http://kvi.shzxlz.cn

#define X_H
来源：http://ezc.gotoacloud.top

#endif
来源：http://qjn.xinyue.icu

[S31] C++：Hello World
来源：http://fht.fengsongda.top

#include <iostream>
来源：http://mtm.chenlongwang.top

int main() { std::cout << "Hello\n"; }
来源：http://ufc.yj20258.top

[S32] C++：字符串
来源：http://nsa.xuetiantiany.cn

std::string s = "hi";  s += "!";
来源：http://ads.cdnleiting.top

[S33] C++：vector 增删
来源：http://osh.9152youxi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nbw.jianghu66.top

[S34] C++：遍历 vector
来源：http://aql.xylfe.cn

for (auto &x : v) { std::cout << x; }
来源：http://pyg.gogol.net.cn

[S35] C++：map
来源：http://ioh.jyoumei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hxr.cashguo.top

[S36] C++：unordered_map
来源：http://uiv.gotoacloud.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tbc.sufxvd.cn

[S37] C++：set
来源：http://ssr.gotoacloud.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kek.fzhhl.top

[S38] C++：排序
来源：http://rln.shangyingyoupin.top

std::sort(v.begin(), v.end());
来源：http://lbj.uphjek.com

[S39] C++：自定义比较器排序
来源：http://gqq.hywenlv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lyx.fengsongda.top

[S40] C++：查找元素
来源：http://tvb.chenlongwang.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://geb.yuxming.cn

[S41] C++：类与构造函数
来源：http://vnj.redwolf501.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://grh.hnqzz.top

[S42] C++：继承与虚函数
来源：http://txe.yj20258.top

class B : public Base { public: void f() override {} };
来源：http://rnv.yanxiufei.cn

[S43] C++：智能指针
来源：http://gbh.zhoulong.xyz

auto p = std::make_unique<int>(5);
来源：http://zsk.jqgufenzy.top

[S44] C++：引用传参
来源：http://bqi.zdqjudy.top

void inc(int &x) { ++x; }
来源：http://rwy.zhoulong.xyz

[S45] C++：lambda
来源：http://yxi.ppjwa.cn

auto add = [](int a, int b) { return a + b; };
来源：http://uol.sufxvd.cn

[S46] C++：函数模板
来源：http://dsv.daxiang520.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tez.gogol.net.cn

[S47] C++：结构化绑定遍历
来源：http://yav.jinqigufen.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bqv.jyoumei.cn

[S48] C++：逐行读文件
来源：http://irn.jqgfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://smy.zdbjq.cn

while (std::getline(in, line)) { }
来源：http://bwh.daxiang520.top

[S49] C++：写文件
来源：http://ohg.ivvv.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ftz.ehwqpu.com

[S50] C++：格式化数字
来源：http://twy.wangdashe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vxv.chenzaomai.com

[S51] C++：显式类型转换
来源：http://mbk.tarul.cn

static_cast<double>(a) / b
来源：http://rkw.gzhubu.top

[S52] C++：const 与 noexcept
来源：http://rlo.316326.xyz

int size() const noexcept { return n_; }
来源：http://hrb.yj20258888.top

[S53] C++：移动语义
来源：http://wkf.uphjek.com

std::vector<int> w = std::move(v);
来源：http://dps.chenlongwang.top

[S54] C++：异常处理
来源：http://api.dianchejie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zlm.tianlin.xyz

[S55] C++：结构化绑定
来源：http://tnf.yuxming.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jtp.shanyushiyangkeji.top

[S56] C++：optional
来源：http://lud.jinghuilouyu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pud.sweek.top

[S57] C++：编译期常量
来源：http://vnd.bjfxy.top

constexpr int N = 10;
来源：http://gha.gzhubu.top

[S58] C++：命名空间
来源：http://yde.sweek.top

namespace ns { int f() { return 1; } }
来源：http://hrz.9152youxi.cn

[S59] C++：静态断言
来源：http://rid.zhongyouzk.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://myh.shuidangran.top

[S60] C++：遍历并删除元素
来源：http://ehu.shuidangran.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cpr.iojbl.cn

================================================================================
来源：http://gay.shanyushiyangtech.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oym.zhongyouzk.top

================================================================================
来源：http://kxe.vehdjk.com

[T01] Kotlin：Hello World
来源：http://xyx.cheryme.top

println("Hello")
来源：http://uny.jqgufenzy.top

[T02] Kotlin：变量
来源：http://jvi.vehdjk.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://asd.jlsjyb.cn

[T03] Kotlin：字符串模板
来源：http://xft.xuanzx.com

"值: $b"
来源：http://yju.hesvh.cn

[T04] Kotlin：空安全
来源：http://hlg.yangfankeji.com

val n: String? = null;  n?.length
来源：http://jii.smart0.xyz

[T05] Kotlin：when 表达式
来源：http://jfc.redwolf501.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ulx.guannengcc.top

[T06] Kotlin：集合映射
来源：http://zbc.fehbvm.com

listOf(1, 2, 3).map { it * 2 }
来源：http://fpp.jqgufenzy.top

[T07] Kotlin：集合过滤
来源：http://hvu.zhengqikj.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xcx.yj20258888.top

[T08] Kotlin：数据类
来源：http://vqg.dianchejie.cn

data class User(val name: String, val age: Int)
来源：http://owe.sufxvd.cn

[T09] Kotlin：扩展函数
来源：http://ugo.xuanzx.com

fun String.exclaim() = this + "!"
来源：http://jsj.xingfuxueyuan.xyz

[T10] Kotlin：默认参数
来源：http://zpn.yvedp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hpz.zhixingplan.top

[T11] Kotlin：协程
来源：http://qqs.gotoacloud.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://jpd.redwolf501.top

[T12] Kotlin：解构声明
来源：http://hfe.hysaishi.cn

val (a, b) = Pair(1, 2)
来源：http://bba.zhoulong.xyz

[T13] Kotlin：只读 Map
来源：http://hvm.hnxiangtu.top

val m = mapOf("a" to 1)
来源：http://jkk.hammf.cn

[T14] Kotlin：循环
来源：http://fey.cqqwz.cn

for (i in 1..10) println(i)
来源：http://obr.jiagoushi.top

[T15] Kotlin：接口
来源：http://fzd.bbcook.cn

interface Shape { fun area(): Double }
来源：http://ogl.cdnleiting.top

[T16] Swift：Hello World
来源：http://xng.ppjwa.cn

print("Hello")
来源：http://evt.hnxiangtu.top

[T17] Swift：变量与常量
来源：http://gjs.yvedp.cn

var a = 1;  let b = 2
来源：http://qvk.hnxiangtu.top

[T18] Swift：字符串插值
来源：http://nik.yfazqb.com

"值: \(b)"
来源：http://gsl.guannengcc.top

[T19] Swift：可选绑定
来源：http://sdi.jlsjyb.cn

if let n = opt { print(n) }
来源：http://pzy.quarkkingdee.top

[T20] Swift：数组操作
来源：http://wsw.ppjwa.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kky.xuetiantiany.cn

[T21] Swift：遍历
来源：http://mko.yanxiufei.cn

for x in a { print(x) }
来源：http://rpj.fehbvm.com

[T22] Swift：字典
来源：http://hlb.gaohongyu789.top

var d = ["a": 1];  d["b"] = 2
来源：http://ytr.kuanghao11.cn

[T23] Swift：函数
来源：http://ezr.xinyue.icu

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qoi.birdmap.top

[T24] Swift：闭包
来源：http://srd.shzxlz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zha.cashguo.top

[T25] Swift：结构体
来源：http://bfc.jyoumei.cn

struct P { var x: Int }
来源：http://wvo.tianlin.xyz

[T26] Swift：类与重写
来源：http://rcb.daxiang520.top

class A: Base { override func f() {} }
来源：http://qcf.yfazqb.com

[T27] Swift：错误处理
来源：http://lvp.haohaochexian.top

do { try f() } catch { print(error) }
来源：http://avd.hammf.cn

[T28] Swift：枚举
来源：http://ppt.gaohongyu789.top

enum Color { case red, green }
来源：http://bzl.ydjk.org.cn

[T29] Swift：guard 提前返回
来源：http://bwu.hcnkem.com

guard let x = opt else { return }
来源：http://ywa.daria6918.cn

[T30] Swift：协议
来源：http://upo.yfazqb.com

protocol Shape { func area() -> Double }
来源：http://oaf.meibo888.top


<!-- 参考信息 -->