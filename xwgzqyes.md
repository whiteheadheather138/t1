代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://myf.meibo888.top

[R34] 退出时清理
来源：http://qrr.xuanzx.com

trap 'rm -f "$tmp"' EXIT
来源：http://wzf.hnxiangtu.top

[R35] 后台执行并等待
来源：http://kvj.yj202588.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ihq.pengpengdd.cyou

[R36] 并发执行多个任务
来源：http://ogm.zdbjq.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kpa.yvedp.cn

[R37] 把输出赋给变量
来源：http://emw.ydjk.org.cn

files=$(ls -1)
来源：http://zxa.hesvh.cn

[R38] 管道串联
来源：http://utl.yongpay.top

cat a.txt | grep -i error | wc -l
来源：http://fpl.smart0.xyz

[R39] 重定向标准输出与错误
来源：http://ryt.yangfankeji.com

cmd > out.log 2>&1
来源：http://htm.cheryme.top

[R40] 追加写日志
来源：http://dzd.ivvv.top

echo "log" >> out.log
来源：http://hoz.hongshengwenyu.top

[R41] 丢弃输出
来源：http://dwz.tian-w.cn

cmd >/dev/null 2>&1
来源：http://dfw.nanxuanxn.top

[R42] 输入重定向
来源：http://mod.yuanzhike.top

wc -l < a.txt
来源：http://bid.shanyushiyangtech.top

[R43] 按名字查找文件
来源：http://lyh.fktsv.cn

find . -name "*.log" -type f
来源：http://kuu.cheryme.top

[R44] 按修改时间查找
来源：http://hls.hcnkem.com

find . -mtime -7 -type f
来源：http://yaw.yj202588.top

[R45] 批量删除
来源：http://kii.tian-w.cn

find . -name "*.tmp" -delete
来源：http://njt.yj20258888.top

[R46] 递归替换文件内容
来源：http://nhl.daxiang520.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://keo.yueranfly.top

[R47] sed 单行替换
来源：http://qxe.aibaodan.cn

sed -i 's/foo/bar/g' a.txt
来源：http://uzo.kuanghao11.cn

[R48] awk 取指定列
来源：http://yis.nanxinkj.top

awk '{print $1, $3}' a.txt
来源：http://rzw.redwolf501.top

[R49] awk 带条件
来源：http://fiz.aibaodan.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mmb.jinqigfzy.top

[R50] awk 求和
来源：http://fkj.chenjidiqi.icu

awk '{s += $2} END {print s}' a.txt
来源：http://wxk.chenzaomai.com

[R51] 排序去重取前几
来源：http://lot.fengsongda.top

sort a.txt | uniq -c | sort -rn | head
来源：http://jgg.ydzc1.top

[R52] 统计行数
来源：http://yvm.gzhubu.top

wc -l a.txt
来源：http://fux.haohaochexian.top

[R53] 查看文件头与实时尾
来源：http://wem.gzhubu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dwf.chenzaomai.com

[R54] 比较两个文件
来源：http://ydv.jinqigfzy.top

diff a.txt b.txt
来源：http://shd.cqqwz.cn

[R55] 压缩与解压
来源：http://umr.jqgfzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qhy.vqdsnc.cn

[R56] 远程拷贝
来源：http://rmk.gotoacloud.top

scp file user@host:/path/
来源：http://drf.shanyushiyangtech.top

[R57] 远程执行命令
来源：http://ogv.vqdsnc.cn

ssh user@host 'uptime'
来源：http://szw.nanxinkj.top

[R58] 下载文件
来源：http://vqn.yongpay.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ong.nanxuanxn.top

[R59] 发 POST JSON
来源：http://zkf.shangyingyoupin.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wtp.mhx1999.top

[R60] 只看 HTTP 状态码
来源：http://hkq.zdqjudy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wds.cqqwz.cn

[R61] 磁盘占用
来源：http://vli.guannengcc.top

df -h;  du -sh *
来源：http://gaa.hesvh.cn

[R62] 找最占空间的文件
来源：http://tul.aizwys.cn

du -ah . | sort -rh | head -10
来源：http://nsf.zhixingplan.top

[R63] 内存与进程
来源：http://arx.smart0.xyz

free -h;  ps aux | grep nginx
来源：http://hbx.chenzaomai.com

[R64] 结束进程
来源：http://vzp.bjfxy.top

kill -9 $(pgrep -f app.py)
来源：http://iqv.xziqi.cn

[R65] 查看端口占用
来源：http://pnl.andypj.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://abj.hnxiangtu.top

[R66] 定时任务
来源：http://vnd.yangfankeji.com

crontab -e;  crontab -l
来源：http://ejo.cashguo.top

[R67] 生成随机十六进制串
来源：http://nfz.mhx1999.top

openssl rand -hex 16
来源：http://oyi.hnqzz.top

[R68] 计算文件校验值
来源：http://fzw.fengsongda.top

sha256sum a.txt;  md5sum a.txt
来源：http://fmb.xinyue.icu

[R69] 生成随机密码
来源：http://kth.wangdashe.top

head -c 16 /dev/urandom | base64
来源：http://sjb.sufxvd.cn

[R70] 时间戳与互转
来源：http://gyx.xziqi.cn

date +%s;  date -d @1700000000
来源：http://acp.pengpengdd.cyou

[R71] 日期格式化
来源：http://mis.zhoulong.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://uck.shangyingyoupin.top

[R72] 等待端口就绪
来源：http://rvv.yanxiufei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lmq.0kj1m.cn

[R73] 分割大日志
来源：http://ffh.shangyingyoupin.top

split -l 1000 big.log part_
来源：http://yka.jlsjyb.cn

[R74] 批量重命名
来源：http://khv.snrcjt.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://otr.wangshuangyany.cn

[R75] 导出环境变量
来源：http://gfp.cheryme.top

export PATH="$HOME/bin:$PATH"
来源：http://qdz.jinyuanbaomall.cn

[R76] 使用临时文件
来源：http://llm.shangyingyoupin.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vrb.xuetiantiany.cn

[R77] 读取用户输入
来源：http://ima.yanxiufei.cn

read -rp "请输入: " ans
来源：http://hvn.xinyue.icu

[R78] 交互式菜单
来源：http://nvr.epnwcf.com

select opt in a b c; do echo "$opt"; break; done
来源：http://fcd.zhaomingkeji.xyz

[R79] 解析命令行选项
来源：http://sey.ppjwa.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ayu.ywan-chungtsiang.top

[R80] 查看脚本执行耗时
来源：http://qpd.redwolf501.top

time ./run.sh
来源：http://jkz.zdbjq.cn

================================================================================
来源：http://xqv.jlsjyb.cn

S. C / C++ 专题
来源：http://atc.tanke756.top

================================================================================
来源：http://agi.yueranfly.top

[S01] C：Hello World
来源：http://igq.0kj1m.cn

#include <stdio.h>
来源：http://xit.jinqigfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jwu.fktsv.cn

[S02] C：变量与格式化输出
来源：http://fws.hfpthk.cn

int a = 10; printf("%d\n", a);
来源：http://wjl.nwbrower.top

[S03] C：读入整数
来源：http://kfq.pycfn.com

int x; scanf("%d", &x);
来源：http://pkd.svipenyu.cn

[S04] C：字符串复制
来源：http://ikh.guannengcc.top

char dst[32]; strcpy(dst, "hi");
来源：http://fuy.shanyushiyangtech.top

[S05] C：字符串长度
来源：http://xxf.aibaodan.cn

strlen(s)
来源：http://gul.hcnkem.com

[S06] C：字符串比较
来源：http://upu.hcnkem.com

strcmp(a, b) == 0
来源：http://ulm.wangshuangyany.cn

[S07] C：数组遍历求和
来源：http://akj.yanxiufei.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qjs.jianghu66.top

[S08] C：动态内存分配与释放
来源：http://yqe.jinqigfzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rqk.gzhubu.top

[S09] C：结构体定义与初始化
来源：http://yep.xziqi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ncj.mhx1999.top

[S10] C：指针与解引用
来源：http://tfx.sufxvd.cn

int *p = &a;  *p = 5;
来源：http://ipo.smart0.xyz

[S11] C：逐行读文件
来源：http://bre.snrcjt.cn

FILE *f = fopen("a.txt", "r");
来源：http://lsc.jianghu66.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://iot.c1oappe.top

fclose(f);
来源：http://taw.hongshengwenyu.top

[S12] C：写文件
来源：http://cfw.smart0.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ybq.yj20258.top

[S13] C：宏定义
来源：http://zlu.hammf.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sou.nanxuanxn.top

[S14] C：枚举
来源：http://mlt.ydjk.org.cn

enum Color { RED, GREEN, BLUE };
来源：http://rne.zhixingplan.top

[S15] C：类型转换
来源：http://dcn.wangshuangyany.cn

(double) a / b
来源：http://cqp.guowangkeji.top

[S16] C：位操作置位
来源：http://sap.yangfankeji.com

x |= (1 << 3);
来源：http://qii.nanxuanxn.top

[S17] C：安全拼接字符串
来源：http://qyz.0kj1m.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hwz.gzhubu.top

[S18] C：命令行参数
来源：http://wyp.yanxiufei.cn

int main(int argc, char **argv)
来源：http://lhm.jinqigufen.top

[S19] C：快速排序
来源：http://afp.c1oappe.top

qsort(a, n, sizeof(int), cmp);
来源：http://fyq.tanke756.top

[S20] C：二分查找
来源：http://hfb.hnxiangtu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jxv.hongshengwenyu.top

[S21] C：字符类别判断
来源：http://pdk.shuidangran.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ifw.9152youxi.cn

[S22] C：字符串转数字
来源：http://gfo.zhengqikj.top

atoi("42");  strtod("3.14", NULL);
来源：http://qmt.iojbl.cn

[S23] C：随机数
来源：http://msw.zhijiandao.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://azj.chenjidiqi.icu

[S24] C：获取本地时间
来源：http://kxc.zycfv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yrr.yuxming.cn

[S25] C：内存拷贝
来源：http://hhy.hcnkem.com

memcpy(dst, src, n);
来源：http://yps.xingfuxueyuan.xyz

[S26] C：内存清零
来源：http://can.yanxiufei.cn

memset(a, 0, sizeof a);
来源：http://zmb.cdnleiting.top

[S27] C：定义常量
来源：http://fdo.9152youxi.cn

const double PI = 3.14159;
来源：http://wsf.dianchejie.cn

[S28] C：静态变量
来源：http://ach.316326.xyz

static int counter = 0;
来源：http://pdm.xinyue.icu

[S29] C：变参函数
来源：http://grf.jinyuanbaomall.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://umd.jlsjyb.cn

[S30] C：头文件保护
来源：http://hgj.tian-w.cn

#ifndef X_H
来源：http://cib.ydjk.org.cn

#define X_H
来源：http://twi.jyoumei.cn

#endif
来源：http://kkb.ybcxt.top

[S31] C++：Hello World
来源：http://jgs.cqqwz.cn

#include <iostream>
来源：http://mrd.cashguo.top

int main() { std::cout << "Hello\n"; }
来源：http://foi.sweek.top

[S32] C++：字符串
来源：http://hvp.nanxinkj.top

std::string s = "hi";  s += "!";
来源：http://axj.hfpthk.cn

[S33] C++：vector 增删
来源：http://afc.yongpay.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rrv.cdnleiting.top

[S34] C++：遍历 vector
来源：http://vkg.fengsongda.top

for (auto &x : v) { std::cout << x; }
来源：http://guw.xziqi.cn

[S35] C++：map
来源：http://nih.ctjpmb.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://twk.ywan-chungtsiang.top

[S36] C++：unordered_map
来源：http://qzy.xziqi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://udf.vehdjk.com

[S37] C++：set
来源：http://nwf.dashuyun.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lhj.feifeiyinyue.top

[S38] C++：排序
来源：http://lmr.xuetiantiany.cn

std::sort(v.begin(), v.end());
来源：http://dwp.fzhhl.top

[S39] C++：自定义比较器排序
来源：http://ocz.vehdjk.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qca.tian-w.cn

[S40] C++：查找元素
来源：http://xkf.yueranfly.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bhj.ybcxt.top

[S41] C++：类与构造函数
来源：http://ywd.ppjwa.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wpf.redwolf501.top

[S42] C++：继承与虚函数
来源：http://evx.c1oappe.top

class B : public Base { public: void f() override {} };
来源：http://hqp.yj202588.top

[S43] C++：智能指针
来源：http://sqw.vqdsnc.cn

auto p = std::make_unique<int>(5);
来源：http://xus.ctjpmb.com

[S44] C++：引用传参
来源：http://qqb.fktsv.cn

void inc(int &x) { ++x; }
来源：http://tpt.zhongyouzk.top

[S45] C++：lambda
来源：http://qfp.feifeiyinyue.top

auto add = [](int a, int b) { return a + b; };
来源：http://xcy.feifeiyinyue.top

[S46] C++：函数模板
来源：http://tqo.ctjpmb.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dzy.fengsongda.top

[S47] C++：结构化绑定遍历
来源：http://eaf.hnxiangtu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://eoq.pycfn.com

[S48] C++：逐行读文件
来源：http://yph.jiagoushi.top

std::ifstream in("a.txt");  std::string line;
来源：http://zsz.gogol.net.cn

while (std::getline(in, line)) { }
来源：http://djh.gzhubu.top

[S49] C++：写文件
来源：http://jkz.fktsv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://frp.fktsv.cn

[S50] C++：格式化数字
来源：http://qew.epnwcf.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oox.aizwys.cn

[S51] C++：显式类型转换
来源：http://zso.cashguo.top

static_cast<double>(a) / b
来源：http://kio.yonumen.top

[S52] C++：const 与 noexcept
来源：http://afk.zhixingplan.top

int size() const noexcept { return n_; }
来源：http://lza.sxryk.cn

[S53] C++：移动语义
来源：http://sjw.tarul.cn

std::vector<int> w = std::move(v);
来源：http://vhs.zdbjq.cn

[S54] C++：异常处理
来源：http://xpj.gzhubu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wdd.vehdjk.com

[S55] C++：结构化绑定
来源：http://bds.wangshuangyany.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://llh.jinghuilouyu.cn

[S56] C++：optional
来源：http://byz.hesvh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eky.0kj1m.cn

[S57] C++：编译期常量
来源：http://xfs.shanyushiyangtech.top

constexpr int N = 10;
来源：http://nio.jianghu66.top

[S58] C++：命名空间
来源：http://vse.shuidangran.top

namespace ns { int f() { return 1; } }
来源：http://kxx.chenlongwang.top

[S59] C++：静态断言
来源：http://jbv.yangfankeji.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jsk.epnwcf.com

[S60] C++：遍历并删除元素
来源：http://boa.guannengcc.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ise.sufxvd.cn

================================================================================
来源：http://wao.shanyushiyangtech.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nux.pycfn.com

================================================================================
来源：http://xit.zdqjudy.top

[T01] Kotlin：Hello World
来源：http://wlp.gaohongyu789.top

println("Hello")
来源：http://wmr.jianghu66.top

[T02] Kotlin：变量
来源：http://adv.fktsv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://myd.cheryme.top

[T03] Kotlin：字符串模板
来源：http://cdm.ywan-chungtsiang.top

"值: $b"
来源：http://vnl.nwbrower.top

[T04] Kotlin：空安全
来源：http://cvk.cheryme.top

val n: String? = null;  n?.length
来源：http://jcx.chenzaomai.com

[T05] Kotlin：when 表达式
来源：http://nps.ctjpmb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hpw.cashguo.top

[T06] Kotlin：集合映射
来源：http://sgu.gotoacloud.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qes.daxiang520.top

[T07] Kotlin：集合过滤
来源：http://qdx.ppjwa.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://epd.xziqi.cn

[T08] Kotlin：数据类
来源：http://zcv.sweek.top

data class User(val name: String, val age: Int)
来源：http://uhe.uphjek.com

[T09] Kotlin：扩展函数
来源：http://jlx.hnqzz.top

fun String.exclaim() = this + "!"
来源：http://wur.jianghu66.top

[T10] Kotlin：默认参数
来源：http://xny.mhx1999.top

fun greet(name: String = "World") = "Hi $name"
来源：http://smj.ehwqpu.com

[T11] Kotlin：协程
来源：http://ret.yuanzhike.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://iap.dianchejie.cn

[T12] Kotlin：解构声明
来源：http://gug.bjfxy.top

val (a, b) = Pair(1, 2)
来源：http://ufn.zhengqikj.top

[T13] Kotlin：只读 Map
来源：http://qtt.ydzc1.top

val m = mapOf("a" to 1)
来源：http://cfs.fzhhl.top

[T14] Kotlin：循环
来源：http://kwn.haohaochexian.top

for (i in 1..10) println(i)
来源：http://nqy.yfazqb.com

[T15] Kotlin：接口
来源：http://dkm.zycfv.cn

interface Shape { fun area(): Double }
来源：http://ryl.tanke756.top

[T16] Swift：Hello World
来源：http://tkv.c1oappe.top

print("Hello")
来源：http://zuv.zhoulong.xyz

[T17] Swift：变量与常量
来源：http://leb.zdqjudy.top

var a = 1;  let b = 2
来源：http://jaj.316326.xyz

[T18] Swift：字符串插值
来源：http://dfr.nanxuanxn.top

"值: \(b)"
来源：http://kut.pycfn.com

[T19] Swift：可选绑定
来源：http://oil.ctjpmb.com

if let n = opt { print(n) }
来源：http://zhp.zhaomingkeji.xyz

[T20] Swift：数组操作
来源：http://pdb.yongpay.top

var a = [1, 2, 3];  a.append(4)
来源：http://jfa.hcnkem.com

[T21] Swift：遍历
来源：http://qea.daxiang520.top

for x in a { print(x) }
来源：http://crq.jianghu66.top

[T22] Swift：字典
来源：http://oaq.xuanzx.com

var d = ["a": 1];  d["b"] = 2
来源：http://cfz.dianchejie.cn

[T23] Swift：函数
来源：http://zsp.haohaochexian.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kzd.zycfv.cn

[T24] Swift：闭包
来源：http://akr.hnqzz.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://zsx.haohaochexian.top

[T25] Swift：结构体
来源：http://sva.jinqigfzy.top

struct P { var x: Int }
来源：http://vmt.xziqi.cn

[T26] Swift：类与重写
来源：http://fox.hnxiangtu.top

class A: Base { override func f() {} }
来源：http://jwd.hfpthk.cn

[T27] Swift：错误处理
来源：http://khg.chenzaomai.com

do { try f() } catch { print(error) }
来源：http://uzp.dashuyun.cn

[T28] Swift：枚举
来源：http://hgj.yueranfly.top

enum Color { case red, green }
来源：http://fym.yj202588.top

[T29] Swift：guard 提前返回
来源：http://gyp.c1oappe.top

guard let x = opt else { return }
来源：http://yor.tianlin.xyz

[T30] Swift：协议
来源：http://aix.hfpthk.cn

protocol Shape { func area() -> Double }
来源：http://ess.vqdsnc.cn

[T31] Lua：Hello World
来源：http://cqf.svipenyu.cn

print("Hello")
来源：http://rxa.chenjidiqi.icu

[T32] Lua：局部变量
来源：http://civ.aibaodan.cn

local a = 1
来源：http://ibb.xziqi.cn

[T33] Lua：表（数组）
来源：http://gvr.zhaomingkeji.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://kbu.bjfxy.top

[T34] Lua：遍历表
来源：http://qkd.chenzaomai.com

for i, v in ipairs(t) do print(i, v) end
来源：http://rpu.aizwys.cn

[T35] Lua：字典表
来源：http://hca.chenlongwang.top

local d = { a = 1 };  d.b = 2
来源：http://wan.snrcjt.cn

[T36] Lua：函数
来源：http://euq.yj20258888.top

function add(a, b) return a + b end
来源：http://uzp.vehdjk.com


<!-- 参考信息 -->