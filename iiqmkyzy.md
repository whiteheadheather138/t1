代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://kkg.jinghuilouyu.cn

[R32] 参数个数校验
来源：http://dhs.jlsjyb.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://aai.iojbl.cn

[R33] 捕获错误并提示行号
来源：http://sya.guannengcc.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mux.zhongyouzk.top

[R34] 退出时清理
来源：http://lvc.yanxiufei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wex.cheryme.top

[R35] 后台执行并等待
来源：http://ovy.pengpengdd.cyou

sleep 5 & pid=$!; wait "$pid"
来源：http://fsm.birdmap.top

[R36] 并发执行多个任务
来源：http://dzl.chenlongwang.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rii.jqgufenzy.top

[R37] 把输出赋给变量
来源：http://thv.jiagoushi.top

files=$(ls -1)
来源：http://lgb.shzxlz.cn

[R38] 管道串联
来源：http://djr.ehwqpu.com

cat a.txt | grep -i error | wc -l
来源：http://dkq.hcnkem.com

[R39] 重定向标准输出与错误
来源：http://sby.dianchejie.cn

cmd > out.log 2>&1
来源：http://vfe.yuanzhike.top

[R40] 追加写日志
来源：http://blo.meibo888.top

echo "log" >> out.log
来源：http://xol.sjlbkw.cn

[R41] 丢弃输出
来源：http://jtj.xuetiantiany.cn

cmd >/dev/null 2>&1
来源：http://tkn.bjfxy.top

[R42] 输入重定向
来源：http://nhn.hesvh.cn

wc -l < a.txt
来源：http://kuz.yj20258.top

[R43] 按名字查找文件
来源：http://eus.jinghuilouyu.cn

find . -name "*.log" -type f
来源：http://pyr.jinghuilouyu.cn

[R44] 按修改时间查找
来源：http://nfg.dianchejie.cn

find . -mtime -7 -type f
来源：http://mbz.quarkkingdee.top

[R45] 批量删除
来源：http://dom.ctjpmb.com

find . -name "*.tmp" -delete
来源：http://voj.zhongyouzk.top

[R46] 递归替换文件内容
来源：http://xir.hnxiangtu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rwi.fengsongda.top

[R47] sed 单行替换
来源：http://pxn.svipenyu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fjc.pengpengdd.cyou

[R48] awk 取指定列
来源：http://wrj.zdbjq.cn

awk '{print $1, $3}' a.txt
来源：http://clx.shanyushiyangkeji.top

[R49] awk 带条件
来源：http://erx.meibo888.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qxx.zhiwuduotai.top

[R50] awk 求和
来源：http://szr.fanxiaobao.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://tps.zdqjudy.top

[R51] 排序去重取前几
来源：http://smo.hnxiangtu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://amu.dianchejie.cn

[R52] 统计行数
来源：http://jej.fktsv.cn

wc -l a.txt
来源：http://buh.svipenyu.cn

[R53] 查看文件头与实时尾
来源：http://pgt.yangfankeji.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oad.shanyushiyangtech.top

[R54] 比较两个文件
来源：http://uoo.wangshuangyany.cn

diff a.txt b.txt
来源：http://cuk.sxryk.cn

[R55] 压缩与解压
来源：http://dal.guannengcc.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bkg.mhx1999.top

[R56] 远程拷贝
来源：http://wek.gzhubu.top

scp file user@host:/path/
来源：http://caw.ywan-chungtsiang.top

[R57] 远程执行命令
来源：http://lql.hammf.cn

ssh user@host 'uptime'
来源：http://dgl.daxiang520.top

[R58] 下载文件
来源：http://cpv.c1oappe.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sfu.haohaochexian.top

[R59] 发 POST JSON
来源：http://daz.hysaishi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jmd.jyoumei.cn

[R60] 只看 HTTP 状态码
来源：http://mix.yuxming.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pva.fehbvm.com

[R61] 磁盘占用
来源：http://ofb.sufxvd.cn

df -h;  du -sh *
来源：http://lqp.yanxiufei.cn

[R62] 找最占空间的文件
来源：http://kkk.hesvh.cn

du -ah . | sort -rh | head -10
来源：http://rgo.wangshuangyany.cn

[R63] 内存与进程
来源：http://tra.vehdjk.com

free -h;  ps aux | grep nginx
来源：http://aml.gzhubu.top

[R64] 结束进程
来源：http://nkm.0kj1m.cn

kill -9 $(pgrep -f app.py)
来源：http://fqt.snrcjt.cn

[R65] 查看端口占用
来源：http://csp.chenjidiqi.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nqu.guowangkeji.top

[R66] 定时任务
来源：http://mox.yangfankeji.com

crontab -e;  crontab -l
来源：http://nwp.shzxlz.cn

[R67] 生成随机十六进制串
来源：http://qrd.gotoacloud.top

openssl rand -hex 16
来源：http://gmz.mhx1999.top

[R68] 计算文件校验值
来源：http://qhz.gaohongyu789.top

sha256sum a.txt;  md5sum a.txt
来源：http://vvr.fktsv.cn

[R69] 生成随机密码
来源：http://nob.guowangkeji.top

head -c 16 /dev/urandom | base64
来源：http://eps.ywan-chungtsiang.top

[R70] 时间戳与互转
来源：http://ewb.nanxuanxn.top

date +%s;  date -d @1700000000
来源：http://llo.cheryme.top

[R71] 日期格式化
来源：http://hbp.ehwqpu.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://bej.iojbl.cn

[R72] 等待端口就绪
来源：http://rre.chenlongwang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://yzo.guowangkeji.top

[R73] 分割大日志
来源：http://nmg.xingfuxueyuan.xyz

split -l 1000 big.log part_
来源：http://ouz.hywenlv.cn

[R74] 批量重命名
来源：http://nzi.shangyingyoupin.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ofi.jinqigfzy.top

[R75] 导出环境变量
来源：http://zrq.cqqwz.cn

export PATH="$HOME/bin:$PATH"
来源：http://szf.cashguo.top

[R76] 使用临时文件
来源：http://xfr.ybcxt.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ymt.uphjek.com

[R77] 读取用户输入
来源：http://fzs.jqgufenzy.top

read -rp "请输入: " ans
来源：http://wnf.jyoumei.cn

[R78] 交互式菜单
来源：http://rwp.yanxiufei.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://adx.316326.xyz

[R79] 解析命令行选项
来源：http://hrr.daxiang520.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fuq.shuidangran.top

[R80] 查看脚本执行耗时
来源：http://mti.zhengqikj.top

time ./run.sh
来源：http://eyb.yvedp.cn

================================================================================
来源：http://ccc.hongshengwenyu.top

S. C / C++ 专题
来源：http://uae.xziqi.cn

================================================================================
来源：http://lfq.hongshengwenyu.top

[S01] C：Hello World
来源：http://ykn.feifeiyinyue.top

#include <stdio.h>
来源：http://ggx.kuanghao11.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zze.redwolf501.top

[S02] C：变量与格式化输出
来源：http://rbo.fzhhl.top

int a = 10; printf("%d\n", a);
来源：http://glg.gaohongyu789.top

[S03] C：读入整数
来源：http://ckh.xingfuxueyuan.xyz

int x; scanf("%d", &x);
来源：http://zip.andypj.xyz

[S04] C：字符串复制
来源：http://mzi.meibo888.top

char dst[32]; strcpy(dst, "hi");
来源：http://ufp.cqqwz.cn

[S05] C：字符串长度
来源：http://eka.jinqigufen.top

strlen(s)
来源：http://uez.yj202588.top

[S06] C：字符串比较
来源：http://qgs.yueranfly.top

strcmp(a, b) == 0
来源：http://fli.xziqi.cn

[S07] C：数组遍历求和
来源：http://xlx.kuanghao11.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://naz.dianchejie.cn

[S08] C：动态内存分配与释放
来源：http://oif.daxiang520.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xhf.andypj.xyz

[S09] C：结构体定义与初始化
来源：http://rqu.nwbrower.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zdq.jinqigufen.top

[S10] C：指针与解引用
来源：http://zqk.fengsongda.top

int *p = &a;  *p = 5;
来源：http://lmx.sysykeji.top

[S11] C：逐行读文件
来源：http://efm.havefunace.top

FILE *f = fopen("a.txt", "r");
来源：http://mxc.zdqjudy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://gah.yongpay.top

fclose(f);
来源：http://fif.yvedp.cn

[S12] C：写文件
来源：http://mai.cashguo.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vfa.yuanzhike.top

[S13] C：宏定义
来源：http://ylk.nwbrower.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ryw.aizwys.cn

[S14] C：枚举
来源：http://jfi.redwolf501.top

enum Color { RED, GREEN, BLUE };
来源：http://ncu.fzhhl.top

[S15] C：类型转换
来源：http://sij.pycfn.com

(double) a / b
来源：http://aky.shuidangran.top

[S16] C：位操作置位
来源：http://mvv.yanxiufei.cn

x |= (1 << 3);
来源：http://edb.aibaodan.cn

[S17] C：安全拼接字符串
来源：http://ier.xingfuxueyuan.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://alc.hywenlv.cn

[S18] C：命令行参数
来源：http://wza.smart0.xyz

int main(int argc, char **argv)
来源：http://aug.shuidangran.top

[S19] C：快速排序
来源：http://lby.yonumen.top

qsort(a, n, sizeof(int), cmp);
来源：http://crh.fehbvm.com

[S20] C：二分查找
来源：http://anx.fengsongda.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ndt.fanxiaobao.xyz

[S21] C：字符类别判断
来源：http://arm.yongpay.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dvn.wangdashe.top

[S22] C：字符串转数字
来源：http://eib.shanyushiyangtech.top

atoi("42");  strtod("3.14", NULL);
来源：http://gao.sweek.top

[S23] C：随机数
来源：http://mxe.nwbrower.top

srand(time(NULL));  int r = rand() % 100;
来源：http://oit.hywenlv.cn

[S24] C：获取本地时间
来源：http://zqm.yongpay.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oqc.cashguo.top

[S25] C：内存拷贝
来源：http://wuj.hysaishi.cn

memcpy(dst, src, n);
来源：http://qkx.svipenyu.cn

[S26] C：内存清零
来源：http://pwl.ppjwa.cn

memset(a, 0, sizeof a);
来源：http://oyf.hesvh.cn

[S27] C：定义常量
来源：http://nxk.hcnkem.com

const double PI = 3.14159;
来源：http://moz.nwbrower.top

[S28] C：静态变量
来源：http://bap.yj20258888.top

static int counter = 0;
来源：http://tqo.wangdashe.top

[S29] C：变参函数
来源：http://cnk.birdmap.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nnl.jyoumei.cn

[S30] C：头文件保护
来源：http://ssf.ywan-chungtsiang.top

#ifndef X_H
来源：http://rey.zhoulong.xyz

#define X_H
来源：http://mlb.52xcode.cn

#endif
来源：http://huy.hfpthk.cn

[S31] C++：Hello World
来源：http://lof.ydjk.org.cn

#include <iostream>
来源：http://lvi.dianchejie.cn

int main() { std::cout << "Hello\n"; }
来源：http://rob.zdqjudy.top

[S32] C++：字符串
来源：http://whl.gaohongyu789.top

std::string s = "hi";  s += "!";
来源：http://ycb.yongpay.top

[S33] C++：vector 增删
来源：http://snh.jyoumei.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nff.dashuyun.cn

[S34] C++：遍历 vector
来源：http://dgw.jinyuanbaomall.cn

for (auto &x : v) { std::cout << x; }
来源：http://pnk.shanyushiyangkeji.top

[S35] C++：map
来源：http://ndq.sweek.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jud.gzhubu.top

[S36] C++：unordered_map
来源：http://aqw.zhijiandao.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iya.haohaochexian.top

[S37] C++：set
来源：http://ekv.xuetiantiany.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sud.haohaochexian.top

[S38] C++：排序
来源：http://pqj.zhixingplan.top

std::sort(v.begin(), v.end());
来源：http://peg.aibaodan.cn

[S39] C++：自定义比较器排序
来源：http://who.jiagoushi.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wqb.zhijiandao.cn

[S40] C++：查找元素
来源：http://dmd.jinqigfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sdk.wangdashe.top

[S41] C++：类与构造函数
来源：http://thu.cqqwz.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yxo.yvedp.cn

[S42] C++：继承与虚函数
来源：http://jms.0kj1m.cn

class B : public Base { public: void f() override {} };
来源：http://nbp.ehwqpu.com

[S43] C++：智能指针
来源：http://rdt.hnqzz.top

auto p = std::make_unique<int>(5);
来源：http://hms.fehbvm.com

[S44] C++：引用传参
来源：http://xdr.yfazqb.com

void inc(int &x) { ++x; }
来源：http://anb.zycfv.cn

[S45] C++：lambda
来源：http://dwi.zhixingplan.top

auto add = [](int a, int b) { return a + b; };
来源：http://kak.0kj1m.cn

[S46] C++：函数模板
来源：http://jtg.xuetiantiany.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://crt.ivvv.top

[S47] C++：结构化绑定遍历
来源：http://xne.nwbrower.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yxg.316326.xyz

[S48] C++：逐行读文件
来源：http://kks.zhongyouzk.top

std::ifstream in("a.txt");  std::string line;
来源：http://tls.hysaishi.cn

while (std::getline(in, line)) { }
来源：http://fph.hnqzz.top

[S49] C++：写文件
来源：http://dsg.hysaishi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iex.xinyue.icu

[S50] C++：格式化数字
来源：http://fjv.sufxvd.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://grt.nwbrower.top

[S51] C++：显式类型转换
来源：http://sim.svipenyu.cn

static_cast<double>(a) / b
来源：http://pmq.xylfe.cn

[S52] C++：const 与 noexcept
来源：http://ggu.zhoulong.xyz

int size() const noexcept { return n_; }
来源：http://uue.bjfxy.top

[S53] C++：移动语义
来源：http://chd.pengpengdd.cyou

std::vector<int> w = std::move(v);
来源：http://vkn.haohaochexian.top

[S54] C++：异常处理
来源：http://exg.zhijiandao.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://joq.chenjidiqi.icu

[S55] C++：结构化绑定
来源：http://pxj.uphjek.com

auto [a, b] = std::make_pair(1, 2);
来源：http://tqd.yj20258888.top

[S56] C++：optional
来源：http://ggj.fktsv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lxp.jinghuilouyu.cn

[S57] C++：编译期常量
来源：http://xpa.jqgufenzy.top

constexpr int N = 10;
来源：http://jov.svipenyu.cn

[S58] C++：命名空间
来源：http://uif.dashuyun.cn

namespace ns { int f() { return 1; } }
来源：http://jmz.bbcook.cn

[S59] C++：静态断言
来源：http://uvb.gogol.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ktt.hesvh.cn

[S60] C++：遍历并删除元素
来源：http://uxc.zdqjudy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rgx.yuanzhike.top

================================================================================
来源：http://ukk.zhijiandao.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ycf.birdmap.top

================================================================================
来源：http://znr.shuidangran.top

[T01] Kotlin：Hello World
来源：http://rku.tarul.cn

println("Hello")
来源：http://efb.sufxvd.cn

[T02] Kotlin：变量
来源：http://egl.zhiwuduotai.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wai.sjlbkw.cn

[T03] Kotlin：字符串模板
来源：http://bmc.hysaishi.cn

"值: $b"
来源：http://vaf.jqgufenzy.top

[T04] Kotlin：空安全
来源：http://mey.sufxvd.cn

val n: String? = null;  n?.length
来源：http://idb.guannengcc.top

[T05] Kotlin：when 表达式
来源：http://dqd.wangshuangyany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zbx.jlsjyb.cn

[T06] Kotlin：集合映射
来源：http://jze.xziqi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xss.gogol.net.cn

[T07] Kotlin：集合过滤
来源：http://kmb.hfpthk.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ohu.hnxiangtu.top

[T08] Kotlin：数据类
来源：http://ueo.zdqjudy.top

data class User(val name: String, val age: Int)
来源：http://spi.xingfuxueyuan.xyz

[T09] Kotlin：扩展函数
来源：http://rts.birdmap.top

fun String.exclaim() = this + "!"
来源：http://ukg.gzhubu.top

[T10] Kotlin：默认参数
来源：http://neb.yuxming.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yis.sweek.top

[T11] Kotlin：协程
来源：http://lcn.uphjek.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://muj.nanxinkj.top

[T12] Kotlin：解构声明
来源：http://nfn.jinqigfzy.top

val (a, b) = Pair(1, 2)
来源：http://uez.sjlbkw.cn

[T13] Kotlin：只读 Map
来源：http://juv.xuanzx.com

val m = mapOf("a" to 1)
来源：http://fla.xylfe.cn

[T14] Kotlin：循环
来源：http://crt.xziqi.cn

for (i in 1..10) println(i)
来源：http://cnm.dianchejie.cn

[T15] Kotlin：接口
来源：http://kct.hywenlv.cn

interface Shape { fun area(): Double }
来源：http://qei.zdbjq.cn

[T16] Swift：Hello World
来源：http://swp.aibaodan.cn

print("Hello")
来源：http://blr.fanxiaobao.xyz

[T17] Swift：变量与常量
来源：http://mjq.xinyue.icu

var a = 1;  let b = 2
来源：http://jtn.fktsv.cn

[T18] Swift：字符串插值
来源：http://eyb.yj20258888.top

"值: \(b)"
来源：http://gfz.yonumen.top

[T19] Swift：可选绑定
来源：http://hpj.zhiwuduotai.top

if let n = opt { print(n) }
来源：http://lqb.zhoulong.xyz

[T20] Swift：数组操作
来源：http://pzg.svipenyu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wzp.c1oappe.top

[T21] Swift：遍历
来源：http://tbh.kuanghao11.cn

for x in a { print(x) }
来源：http://tzy.hysaishi.cn

[T22] Swift：字典
来源：http://vav.vqdsnc.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zeo.gaohongyu789.top

[T23] Swift：函数
来源：http://rox.svipenyu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://enl.zdbjq.cn

[T24] Swift：闭包
来源：http://bpn.ydzc1.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://knu.tarul.cn

[T25] Swift：结构体
来源：http://kyw.xylfe.cn

struct P { var x: Int }
来源：http://umk.yj202588.top

[T26] Swift：类与重写
来源：http://uom.havefunace.top

class A: Base { override func f() {} }
来源：http://ipx.guowangkeji.top

[T27] Swift：错误处理
来源：http://wrw.wangdashe.top

do { try f() } catch { print(error) }
来源：http://lmv.yj20258888.top

[T28] Swift：枚举
来源：http://koj.nwbrower.top

enum Color { case red, green }
来源：http://chm.jinghuilouyu.cn

[T29] Swift：guard 提前返回
来源：http://qbb.xziqi.cn

guard let x = opt else { return }
来源：http://pqh.fzhhl.top

[T30] Swift：协议
来源：http://ixh.zhaomingkeji.xyz

protocol Shape { func area() -> Double }
来源：http://kor.jinqigufen.top

[T31] Lua：Hello World
来源：http://zsi.epnwcf.com

print("Hello")
来源：http://kwb.zhoulong.xyz

[T32] Lua：局部变量
来源：http://bdc.hongshengwenyu.top

local a = 1
来源：http://tnq.xziqi.cn

[T33] Lua：表（数组）
来源：http://bcb.jqgfzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ril.xziqi.cn

[T34] Lua：遍历表
来源：http://rme.gogol.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://euk.hesvh.cn


<!-- 参考信息 -->