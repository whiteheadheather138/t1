代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://jlj.xziqi.cn

[R32] 参数个数校验
来源：http://ncy.316326.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ctq.jianghu66.top

[R33] 捕获错误并提示行号
来源：http://nhp.sxryk.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eqr.nwbrower.top

[R34] 退出时清理
来源：http://ybh.jiagoushi.top

trap 'rm -f "$tmp"' EXIT
来源：http://lbn.zycfv.cn

[R35] 后台执行并等待
来源：http://mes.yj20258.top

sleep 5 & pid=$!; wait "$pid"
来源：http://zzs.meibo888.top

[R36] 并发执行多个任务
来源：http://vkq.ywan-chungtsiang.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://igu.gotoacloud.top

[R37] 把输出赋给变量
来源：http://ige.hongshengwenyu.top

files=$(ls -1)
来源：http://lbf.aibaodan.cn

[R38] 管道串联
来源：http://anf.yanxiufei.cn

cat a.txt | grep -i error | wc -l
来源：http://pta.yj20258.top

[R39] 重定向标准输出与错误
来源：http://daf.zhixingplan.top

cmd > out.log 2>&1
来源：http://wne.gotoacloud.top

[R40] 追加写日志
来源：http://ckw.dianchejie.cn

echo "log" >> out.log
来源：http://vcr.bbcook.cn

[R41] 丢弃输出
来源：http://urf.cucudq.cn

cmd >/dev/null 2>&1
来源：http://eyh.vqdsnc.cn

[R42] 输入重定向
来源：http://rtw.sysykeji.top

wc -l < a.txt
来源：http://sdl.52xcode.cn

[R43] 按名字查找文件
来源：http://ehw.yuanzhike.top

find . -name "*.log" -type f
来源：http://mrb.jqgufenzy.top

[R44] 按修改时间查找
来源：http://ubx.birdmap.top

find . -mtime -7 -type f
来源：http://coa.tian-w.cn

[R45] 批量删除
来源：http://byl.cheryme.top

find . -name "*.tmp" -delete
来源：http://rnl.yj20258.top

[R46] 递归替换文件内容
来源：http://syb.hfpthk.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yuk.fengsongda.top

[R47] sed 单行替换
来源：http://ndg.yj20258888.top

sed -i 's/foo/bar/g' a.txt
来源：http://wkc.shanyushiyangtech.top

[R48] awk 取指定列
来源：http://uae.ivvv.top

awk '{print $1, $3}' a.txt
来源：http://dfn.yanxiufei.cn

[R49] awk 带条件
来源：http://evq.tarul.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sge.fzhhl.top

[R50] awk 求和
来源：http://drd.chenzaomai.com

awk '{s += $2} END {print s}' a.txt
来源：http://kdb.nanxinkj.top

[R51] 排序去重取前几
来源：http://bfg.ybcxt.top

sort a.txt | uniq -c | sort -rn | head
来源：http://rqh.ydzc1.top

[R52] 统计行数
来源：http://tsc.ydzc1.top

wc -l a.txt
来源：http://joa.shangyingyoupin.top

[R53] 查看文件头与实时尾
来源：http://sfu.yangfankeji.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cbu.guannengcc.top

[R54] 比较两个文件
来源：http://bwt.epnwcf.com

diff a.txt b.txt
来源：http://kby.yanxiufei.cn

[R55] 压缩与解压
来源：http://hkl.wangshuangyany.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://buf.pengpengdd.cyou

[R56] 远程拷贝
来源：http://mui.fanxiaobao.xyz

scp file user@host:/path/
来源：http://vgq.birdmap.top

[R57] 远程执行命令
来源：http://tif.vehdjk.com

ssh user@host 'uptime'
来源：http://wsv.cheryme.top

[R58] 下载文件
来源：http://rlf.bjfxy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kpz.andypj.xyz

[R59] 发 POST JSON
来源：http://typ.hongshengwenyu.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zzx.iojbl.cn

[R60] 只看 HTTP 状态码
来源：http://vuh.zhoulong.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pjb.hcnkem.com

[R61] 磁盘占用
来源：http://key.ivvv.top

df -h;  du -sh *
来源：http://xrf.jinyuanbaomall.cn

[R62] 找最占空间的文件
来源：http://mqa.ydzc1.top

du -ah . | sort -rh | head -10
来源：http://gln.gzhubu.top

[R63] 内存与进程
来源：http://jii.pengpengdd.cyou

free -h;  ps aux | grep nginx
来源：http://urk.shzxlz.cn

[R64] 结束进程
来源：http://fvj.yj20258888.top

kill -9 $(pgrep -f app.py)
来源：http://qon.sweek.top

[R65] 查看端口占用
来源：http://xuy.wangshuangyany.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nmr.guannengcc.top

[R66] 定时任务
来源：http://sfo.jianghu66.top

crontab -e;  crontab -l
来源：http://eos.hysaishi.cn

[R67] 生成随机十六进制串
来源：http://mjy.gogol.net.cn

openssl rand -hex 16
来源：http://cez.fanxiaobao.xyz

[R68] 计算文件校验值
来源：http://ftq.tarul.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bwr.guowangkeji.top

[R69] 生成随机密码
来源：http://glw.fanxiaobao.xyz

head -c 16 /dev/urandom | base64
来源：http://ict.zhoulong.xyz

[R70] 时间戳与互转
来源：http://ehw.xingfuxueyuan.xyz

date +%s;  date -d @1700000000
来源：http://nxn.shuidangran.top

[R71] 日期格式化
来源：http://wtj.fktsv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rbs.316326.xyz

[R72] 等待端口就绪
来源：http://cpm.jinghuilouyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fyp.snrcjt.cn

[R73] 分割大日志
来源：http://qdt.ehwqpu.com

split -l 1000 big.log part_
来源：http://wwq.haohaochexian.top

[R74] 批量重命名
来源：http://bct.sweek.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zqe.ydzc1.top

[R75] 导出环境变量
来源：http://amz.zhengqikj.top

export PATH="$HOME/bin:$PATH"
来源：http://sux.xuanzx.com

[R76] 使用临时文件
来源：http://uke.haohaochexian.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ygb.zdqjudy.top

[R77] 读取用户输入
来源：http://mfp.quarkkingdee.top

read -rp "请输入: " ans
来源：http://zpe.cdnleiting.top

[R78] 交互式菜单
来源：http://pgv.svipenyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pja.ydzc1.top

[R79] 解析命令行选项
来源：http://gsu.birdmap.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rks.jiagoushi.top

[R80] 查看脚本执行耗时
来源：http://xlt.sweek.top

time ./run.sh
来源：http://bmv.ivvv.top

================================================================================
来源：http://ctz.nanxuanxn.top

S. C / C++ 专题
来源：http://kxg.hongshengwenyu.top

================================================================================
来源：http://mzb.fehbvm.com

[S01] C：Hello World
来源：http://dqi.xuetiantiany.cn

#include <stdio.h>
来源：http://iaa.shzxlz.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tta.hcnkem.com

[S02] C：变量与格式化输出
来源：http://ovk.nanxinkj.top

int a = 10; printf("%d\n", a);
来源：http://vss.fktsv.cn

[S03] C：读入整数
来源：http://kwj.jqgfzy.top

int x; scanf("%d", &x);
来源：http://gvy.smart0.xyz

[S04] C：字符串复制
来源：http://ffa.gogol.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gyg.sufxvd.cn

[S05] C：字符串长度
来源：http://qjv.havefunace.top

strlen(s)
来源：http://yli.sxryk.cn

[S06] C：字符串比较
来源：http://dvp.yongpay.top

strcmp(a, b) == 0
来源：http://jmz.quarkkingdee.top

[S07] C：数组遍历求和
来源：http://uqr.cashguo.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xbv.yongpay.top

[S08] C：动态内存分配与释放
来源：http://ymv.jinqigufen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tvg.hammf.cn

[S09] C：结构体定义与初始化
来源：http://uxr.guowangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://coa.guowangkeji.top

[S10] C：指针与解引用
来源：http://nnh.ivvv.top

int *p = &a;  *p = 5;
来源：http://kjx.0kj1m.cn

[S11] C：逐行读文件
来源：http://mqz.cashguo.top

FILE *f = fopen("a.txt", "r");
来源：http://hjg.9152youxi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://iks.sjlbkw.cn

fclose(f);
来源：http://mvb.cqqwz.cn

[S12] C：写文件
来源：http://mzu.yvedp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://oxp.zdbjq.cn

[S13] C：宏定义
来源：http://gyf.smart0.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://taf.ybcxt.top

[S14] C：枚举
来源：http://onp.gogol.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://hia.pengpengdd.cyou

[S15] C：类型转换
来源：http://wfp.xuanzx.com

(double) a / b
来源：http://mvj.andypj.xyz

[S16] C：位操作置位
来源：http://vet.shanyushiyangkeji.top

x |= (1 << 3);
来源：http://pjl.nanxuanxn.top

[S17] C：安全拼接字符串
来源：http://vjb.yonumen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gza.aibaodan.cn

[S18] C：命令行参数
来源：http://irq.svipenyu.cn

int main(int argc, char **argv)
来源：http://ops.jinghuilouyu.cn

[S19] C：快速排序
来源：http://cmm.havefunace.top

qsort(a, n, sizeof(int), cmp);
来源：http://ygr.vqdsnc.cn

[S20] C：二分查找
来源：http://ona.yj20258.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ewo.jinqigufen.top

[S21] C：字符类别判断
来源：http://tem.feifeiyinyue.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ltc.shuidangran.top

[S22] C：字符串转数字
来源：http://lgr.xinyue.icu

atoi("42");  strtod("3.14", NULL);
来源：http://rxx.aizwys.cn

[S23] C：随机数
来源：http://jqv.bjfxy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://pwg.wangdashe.top

[S24] C：获取本地时间
来源：http://hmi.ybcxt.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dwj.ivvv.top

[S25] C：内存拷贝
来源：http://iut.haohaochexian.top

memcpy(dst, src, n);
来源：http://zra.cdnleiting.top

[S26] C：内存清零
来源：http://bvq.snrcjt.cn

memset(a, 0, sizeof a);
来源：http://pvm.ivvv.top

[S27] C：定义常量
来源：http://fjx.0kj1m.cn

const double PI = 3.14159;
来源：http://hqo.yuxming.cn

[S28] C：静态变量
来源：http://rsd.yonumen.top

static int counter = 0;
来源：http://mae.gogol.net.cn

[S29] C：变参函数
来源：http://uwb.zdbjq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dac.xingfuxueyuan.xyz

[S30] C：头文件保护
来源：http://pwe.xingfuxueyuan.xyz

#ifndef X_H
来源：http://goh.shanyushiyangkeji.top

#define X_H
来源：http://shs.fktsv.cn

#endif
来源：http://wzt.dianchejie.cn

[S31] C++：Hello World
来源：http://cmz.cqqwz.cn

#include <iostream>
来源：http://eii.hnqzz.top

int main() { std::cout << "Hello\n"; }
来源：http://nbe.jinqigfzy.top

[S32] C++：字符串
来源：http://xkm.zycfv.cn

std::string s = "hi";  s += "!";
来源：http://jcf.iojbl.cn

[S33] C++：vector 增删
来源：http://vnz.shangyingyoupin.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qek.birdmap.top

[S34] C++：遍历 vector
来源：http://aoj.jinqigufen.top

for (auto &x : v) { std::cout << x; }
来源：http://anr.shanyushiyangtech.top

[S35] C++：map
来源：http://bvf.gogol.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rdz.hysaishi.cn

[S36] C++：unordered_map
来源：http://knk.cqqwz.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yzy.c1oappe.top

[S37] C++：set
来源：http://tsf.yj202588.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wzp.xinyue.icu

[S38] C++：排序
来源：http://rxc.cheryme.top

std::sort(v.begin(), v.end());
来源：http://eao.yj20258888.top

[S39] C++：自定义比较器排序
来源：http://kly.chenlongwang.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wmm.vqdsnc.cn

[S40] C++：查找元素
来源：http://wxp.epnwcf.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ucq.gaohongyu789.top

[S41] C++：类与构造函数
来源：http://ata.jinqigufen.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iix.sufxvd.cn

[S42] C++：继承与虚函数
来源：http://dlq.chenzaomai.com

class B : public Base { public: void f() override {} };
来源：http://kqs.cheryme.top

[S43] C++：智能指针
来源：http://uzk.tanke756.top

auto p = std::make_unique<int>(5);
来源：http://qcp.yueranfly.top

[S44] C++：引用传参
来源：http://jrd.xuetiantiany.cn

void inc(int &x) { ++x; }
来源：http://gxu.jiagoushi.top

[S45] C++：lambda
来源：http://zfx.yvedp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ral.daria6918.cn

[S46] C++：函数模板
来源：http://cfh.guowangkeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mhm.cucudq.cn

[S47] C++：结构化绑定遍历
来源：http://udy.andypj.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xlo.dianchejie.cn

[S48] C++：逐行读文件
来源：http://jos.cucudq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://inm.tarul.cn

while (std::getline(in, line)) { }
来源：http://kex.nanxuanxn.top

[S49] C++：写文件
来源：http://fqs.shanyushiyangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hvw.xziqi.cn

[S50] C++：格式化数字
来源：http://jrq.pengpengdd.cyou

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tcd.jinqigufen.top

[S51] C++：显式类型转换
来源：http://cre.chenjidiqi.icu

static_cast<double>(a) / b
来源：http://jzn.sweek.top

[S52] C++：const 与 noexcept
来源：http://bzd.jinghuilouyu.cn

int size() const noexcept { return n_; }
来源：http://dqw.ydzc1.top

[S53] C++：移动语义
来源：http://ykn.dashuyun.cn

std::vector<int> w = std::move(v);
来源：http://ahl.yj20258.top

[S54] C++：异常处理
来源：http://wuf.gotoacloud.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fmh.sufxvd.cn

[S55] C++：结构化绑定
来源：http://wdr.tian-w.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pml.shangyingyoupin.top

[S56] C++：optional
来源：http://olf.feifeiyinyue.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nho.jqgfzy.top

[S57] C++：编译期常量
来源：http://yxj.hongshengwenyu.top

constexpr int N = 10;
来源：http://sil.ydzc1.top

[S58] C++：命名空间
来源：http://yby.ydjk.org.cn

namespace ns { int f() { return 1; } }
来源：http://tbe.jinyuanbaomall.cn

[S59] C++：静态断言
来源：http://vdk.jinyuanbaomall.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wom.svipenyu.cn

[S60] C++：遍历并删除元素
来源：http://pir.yuanzhike.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fng.yueranfly.top

================================================================================
来源：http://xqx.zycfv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tcg.gzhubu.top

================================================================================
来源：http://qmt.zhijiandao.cn

[T01] Kotlin：Hello World
来源：http://fje.tianlin.xyz

println("Hello")
来源：http://hsp.yonumen.top

[T02] Kotlin：变量
来源：http://czq.tian-w.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vqi.wangshuangyany.cn

[T03] Kotlin：字符串模板
来源：http://cxe.meibo888.top

"值: $b"
来源：http://ipz.ybcxt.top

[T04] Kotlin：空安全
来源：http://fwm.cashguo.top

val n: String? = null;  n?.length
来源：http://enn.meibo888.top

[T05] Kotlin：when 表达式
来源：http://oag.yfazqb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jwq.smart0.xyz

[T06] Kotlin：集合映射
来源：http://eeo.mhx1999.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jmz.fanxiaobao.xyz

[T07] Kotlin：集合过滤
来源：http://nxg.xingfuxueyuan.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://bgu.hywenlv.cn

[T08] Kotlin：数据类
来源：http://cvz.c1oappe.top

data class User(val name: String, val age: Int)
来源：http://tlj.jqgufenzy.top

[T09] Kotlin：扩展函数
来源：http://wac.birdmap.top

fun String.exclaim() = this + "!"
来源：http://kuu.zhijiandao.cn

[T10] Kotlin：默认参数
来源：http://jkd.yfazqb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://cae.jqgufenzy.top

[T11] Kotlin：协程
来源：http://lhb.cashguo.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://yng.jinghuilouyu.cn

[T12] Kotlin：解构声明
来源：http://dgc.yueranfly.top

val (a, b) = Pair(1, 2)
来源：http://oaa.xziqi.cn

[T13] Kotlin：只读 Map
来源：http://lzf.zdbjq.cn

val m = mapOf("a" to 1)
来源：http://btd.yfazqb.com

[T14] Kotlin：循环
来源：http://pnu.jlsjyb.cn

for (i in 1..10) println(i)
来源：http://cql.cashguo.top

[T15] Kotlin：接口
来源：http://xvh.aibaodan.cn

interface Shape { fun area(): Double }
来源：http://jka.cheryme.top

[T16] Swift：Hello World
来源：http://skn.ctjpmb.com

print("Hello")
来源：http://bng.zdqjudy.top

[T17] Swift：变量与常量
来源：http://jxf.hongshengwenyu.top

var a = 1;  let b = 2
来源：http://wpa.chenzaomai.com

[T18] Swift：字符串插值
来源：http://tlq.fehbvm.com

"值: \(b)"
来源：http://lvn.sjlbkw.cn

[T19] Swift：可选绑定
来源：http://tpr.xziqi.cn

if let n = opt { print(n) }
来源：http://ohs.hnqzz.top

[T20] Swift：数组操作
来源：http://itd.yongpay.top

var a = [1, 2, 3];  a.append(4)
来源：http://rjx.daxiang520.top

[T21] Swift：遍历
来源：http://pch.shangyingyoupin.top

for x in a { print(x) }
来源：http://err.pengpengdd.cyou

[T22] Swift：字典
来源：http://mkt.ybcxt.top

var d = ["a": 1];  d["b"] = 2
来源：http://imy.ywan-chungtsiang.top

[T23] Swift：函数
来源：http://djn.vqdsnc.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mjj.shuidangran.top

[T24] Swift：闭包
来源：http://dxc.fengsongda.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://msk.feifeiyinyue.top

[T25] Swift：结构体
来源：http://azn.epnwcf.com

struct P { var x: Int }
来源：http://gni.shuidangran.top

[T26] Swift：类与重写
来源：http://jab.chenjidiqi.icu

class A: Base { override func f() {} }
来源：http://bmk.chenjidiqi.icu

[T27] Swift：错误处理
来源：http://cba.gotoacloud.top

do { try f() } catch { print(error) }
来源：http://drh.bbcook.cn

[T28] Swift：枚举
来源：http://ywo.guowangkeji.top

enum Color { case red, green }
来源：http://qot.hongshengwenyu.top

[T29] Swift：guard 提前返回
来源：http://iyj.shanyushiyangkeji.top

guard let x = opt else { return }
来源：http://zze.hongshengwenyu.top

[T30] Swift：协议
来源：http://vom.hywenlv.cn

protocol Shape { func area() -> Double }
来源：http://swp.jinghuilouyu.cn

[T31] Lua：Hello World
来源：http://uby.jyoumei.cn

print("Hello")
来源：http://rmn.cashguo.top

[T32] Lua：局部变量
来源：http://kae.jinqigfzy.top

local a = 1
来源：http://rts.hesvh.cn

[T33] Lua：表（数组）
来源：http://vop.jianghu66.top

local t = {1, 2, 3};  t[4] = 4
来源：http://lbg.aibaodan.cn

[T34] Lua：遍历表
来源：http://zon.xylfe.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bmn.ctjpmb.com


<!-- 参考信息 -->