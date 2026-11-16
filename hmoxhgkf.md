代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://zok.hfpthk.cn

[R32] 参数个数校验
来源：http://nop.tanke756.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uuc.hnxiangtu.top

[R33] 捕获错误并提示行号
来源：http://kke.yj202588.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nnt.gotoacloud.top

[R34] 退出时清理
来源：http://bff.mhx1999.top

trap 'rm -f "$tmp"' EXIT
来源：http://bna.xuetiantiany.cn

[R35] 后台执行并等待
来源：http://smi.ehwqpu.com

sleep 5 & pid=$!; wait "$pid"
来源：http://bnx.yangfankeji.com

[R36] 并发执行多个任务
来源：http://tuo.nanxinkj.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mli.tianlin.xyz

[R37] 把输出赋给变量
来源：http://jbi.shuidangran.top

files=$(ls -1)
来源：http://qsw.chenjidiqi.icu

[R38] 管道串联
来源：http://vgo.hywenlv.cn

cat a.txt | grep -i error | wc -l
来源：http://oha.shanyushiyangkeji.top

[R39] 重定向标准输出与错误
来源：http://qcr.uphjek.com

cmd > out.log 2>&1
来源：http://hyj.xziqi.cn

[R40] 追加写日志
来源：http://pxd.sxryk.cn

echo "log" >> out.log
来源：http://cck.meibo888.top

[R41] 丢弃输出
来源：http://wfe.jinghuilouyu.cn

cmd >/dev/null 2>&1
来源：http://ksx.xziqi.cn

[R42] 输入重定向
来源：http://hgu.ivvv.top

wc -l < a.txt
来源：http://xhj.bbcook.cn

[R43] 按名字查找文件
来源：http://psr.zycfv.cn

find . -name "*.log" -type f
来源：http://ftj.tanke756.top

[R44] 按修改时间查找
来源：http://nmy.yj202588.top

find . -mtime -7 -type f
来源：http://rna.tianlin.xyz

[R45] 批量删除
来源：http://nmr.hnxiangtu.top

find . -name "*.tmp" -delete
来源：http://vel.cheryme.top

[R46] 递归替换文件内容
来源：http://ghq.xziqi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://eda.tianlin.xyz

[R47] sed 单行替换
来源：http://tib.snrcjt.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jrb.gogol.net.cn

[R48] awk 取指定列
来源：http://kbz.xinyue.icu

awk '{print $1, $3}' a.txt
来源：http://lmv.cdnleiting.top

[R49] awk 带条件
来源：http://qxk.52xcode.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hsa.0kj1m.cn

[R50] awk 求和
来源：http://miu.svipenyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dwu.jianghu66.top

[R51] 排序去重取前几
来源：http://vpe.dashuyun.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kmw.yonumen.top

[R52] 统计行数
来源：http://bki.fktsv.cn

wc -l a.txt
来源：http://ykg.redwolf501.top

[R53] 查看文件头与实时尾
来源：http://asr.0kj1m.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jux.zhijiandao.cn

[R54] 比较两个文件
来源：http://lxh.sweek.top

diff a.txt b.txt
来源：http://ktc.nanxuanxn.top

[R55] 压缩与解压
来源：http://ttr.xuanzx.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ysl.xylfe.cn

[R56] 远程拷贝
来源：http://adt.52xcode.cn

scp file user@host:/path/
来源：http://lvt.aibaodan.cn

[R57] 远程执行命令
来源：http://bkh.zhongyouzk.top

ssh user@host 'uptime'
来源：http://uhb.xylfe.cn

[R58] 下载文件
来源：http://ogt.ydzc1.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zkv.bjfxy.top

[R59] 发 POST JSON
来源：http://tbn.hongshengwenyu.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gtu.ywan-chungtsiang.top

[R60] 只看 HTTP 状态码
来源：http://rvs.wangshuangyany.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uie.ppjwa.cn

[R61] 磁盘占用
来源：http://aao.chenzaomai.com

df -h;  du -sh *
来源：http://mtj.52xcode.cn

[R62] 找最占空间的文件
来源：http://nmp.daxiang520.top

du -ah . | sort -rh | head -10
来源：http://eqy.gzhubu.top

[R63] 内存与进程
来源：http://swh.shuidangran.top

free -h;  ps aux | grep nginx
来源：http://xtu.hcnkem.com

[R64] 结束进程
来源：http://xap.zhongyouzk.top

kill -9 $(pgrep -f app.py)
来源：http://mps.sysykeji.top

[R65] 查看端口占用
来源：http://yju.fktsv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bqk.hammf.cn

[R66] 定时任务
来源：http://lhm.bjfxy.top

crontab -e;  crontab -l
来源：http://zil.cashguo.top

[R67] 生成随机十六进制串
来源：http://zge.fktsv.cn

openssl rand -hex 16
来源：http://hdg.xinyue.icu

[R68] 计算文件校验值
来源：http://onf.ehwqpu.com

sha256sum a.txt;  md5sum a.txt
来源：http://ulj.jinqigfzy.top

[R69] 生成随机密码
来源：http://ojs.aibaodan.cn

head -c 16 /dev/urandom | base64
来源：http://fnz.jinqigfzy.top

[R70] 时间戳与互转
来源：http://dnz.zhixingplan.top

date +%s;  date -d @1700000000
来源：http://nsx.ivvv.top

[R71] 日期格式化
来源：http://kdi.bbcook.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yng.sufxvd.cn

[R72] 等待端口就绪
来源：http://fuf.cdnleiting.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qgv.zhiwuduotai.top

[R73] 分割大日志
来源：http://rui.sxryk.cn

split -l 1000 big.log part_
来源：http://atx.c1oappe.top

[R74] 批量重命名
来源：http://nhk.xziqi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://irp.feifeiyinyue.top

[R75] 导出环境变量
来源：http://hes.ybcxt.top

export PATH="$HOME/bin:$PATH"
来源：http://ydj.jqgufenzy.top

[R76] 使用临时文件
来源：http://lfb.ctjpmb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bhb.yj202588.top

[R77] 读取用户输入
来源：http://blb.zhixingplan.top

read -rp "请输入: " ans
来源：http://ykd.wangdashe.top

[R78] 交互式菜单
来源：http://dat.ivvv.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hna.yj202588.top

[R79] 解析命令行选项
来源：http://tfm.ppjwa.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vsz.bbcook.cn

[R80] 查看脚本执行耗时
来源：http://tqt.yuanzhike.top

time ./run.sh
来源：http://iup.0kj1m.cn

================================================================================
来源：http://cty.jyoumei.cn

S. C / C++ 专题
来源：http://syd.wangdashe.top

================================================================================
来源：http://rln.bjfxy.top

[S01] C：Hello World
来源：http://hcu.ydjk.org.cn

#include <stdio.h>
来源：http://pqx.hywenlv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://npq.fktsv.cn

[S02] C：变量与格式化输出
来源：http://kbg.gotoacloud.top

int a = 10; printf("%d\n", a);
来源：http://gwy.ybcxt.top

[S03] C：读入整数
来源：http://fho.jinqigufen.top

int x; scanf("%d", &x);
来源：http://jbf.hesvh.cn

[S04] C：字符串复制
来源：http://aym.yfazqb.com

char dst[32]; strcpy(dst, "hi");
来源：http://vka.yueranfly.top

[S05] C：字符串长度
来源：http://bbw.jqgufenzy.top

strlen(s)
来源：http://guz.ydzc1.top

[S06] C：字符串比较
来源：http://uui.yueranfly.top

strcmp(a, b) == 0
来源：http://tra.zhiwuduotai.top

[S07] C：数组遍历求和
来源：http://yxa.9152youxi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sti.shangyingyoupin.top

[S08] C：动态内存分配与释放
来源：http://wzj.quarkkingdee.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ocd.zycfv.cn

[S09] C：结构体定义与初始化
来源：http://mhl.sysykeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://isb.jqgfzy.top

[S10] C：指针与解引用
来源：http://hlq.xinyue.icu

int *p = &a;  *p = 5;
来源：http://jub.xuanzx.com

[S11] C：逐行读文件
来源：http://qka.smart0.xyz

FILE *f = fopen("a.txt", "r");
来源：http://rti.sxryk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fil.gaohongyu789.top

fclose(f);
来源：http://eao.zycfv.cn

[S12] C：写文件
来源：http://qqx.jinqigufen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tlw.cqqwz.cn

[S13] C：宏定义
来源：http://yoq.yj20258.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xua.c1oappe.top

[S14] C：枚举
来源：http://mix.316326.xyz

enum Color { RED, GREEN, BLUE };
来源：http://lxz.shangyingyoupin.top

[S15] C：类型转换
来源：http://nte.jinyuanbaomall.cn

(double) a / b
来源：http://edw.pengpengdd.cyou

[S16] C：位操作置位
来源：http://pmz.yj20258.top

x |= (1 << 3);
来源：http://tmy.c1oappe.top

[S17] C：安全拼接字符串
来源：http://fdw.tian-w.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fgw.zhengqikj.top

[S18] C：命令行参数
来源：http://wzn.bjfxy.top

int main(int argc, char **argv)
来源：http://ndm.bjfxy.top

[S19] C：快速排序
来源：http://jvt.snrcjt.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wpw.gzhubu.top

[S20] C：二分查找
来源：http://jog.zhiwuduotai.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fzm.wangshuangyany.cn

[S21] C：字符类别判断
来源：http://uph.sweek.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qdy.gotoacloud.top

[S22] C：字符串转数字
来源：http://gpt.cqqwz.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xyj.zhixingplan.top

[S23] C：随机数
来源：http://ape.chenzaomai.com

srand(time(NULL));  int r = rand() % 100;
来源：http://ibu.yangfankeji.com

[S24] C：获取本地时间
来源：http://kzc.52xcode.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://brg.chenjidiqi.icu

[S25] C：内存拷贝
来源：http://krx.tanke756.top

memcpy(dst, src, n);
来源：http://naz.yueranfly.top

[S26] C：内存清零
来源：http://soq.zhaomingkeji.xyz

memset(a, 0, sizeof a);
来源：http://ydb.hywenlv.cn

[S27] C：定义常量
来源：http://kkn.zhongyouzk.top

const double PI = 3.14159;
来源：http://byr.ppjwa.cn

[S28] C：静态变量
来源：http://kkr.fzhhl.top

static int counter = 0;
来源：http://ezk.9152youxi.cn

[S29] C：变参函数
来源：http://vxt.yuanzhike.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ywv.gogol.net.cn

[S30] C：头文件保护
来源：http://nqv.ehwqpu.com

#ifndef X_H
来源：http://rqr.tarul.cn

#define X_H
来源：http://lla.fanxiaobao.xyz

#endif
来源：http://jfb.mhx1999.top

[S31] C++：Hello World
来源：http://fuv.jinyuanbaomall.cn

#include <iostream>
来源：http://tuq.gotoacloud.top

int main() { std::cout << "Hello\n"; }
来源：http://csw.tian-w.cn

[S32] C++：字符串
来源：http://nvv.jqgfzy.top

std::string s = "hi";  s += "!";
来源：http://yzk.zdbjq.cn

[S33] C++：vector 增删
来源：http://rrh.hywenlv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bct.cqqwz.cn

[S34] C++：遍历 vector
来源：http://wjs.zhaomingkeji.xyz

for (auto &x : v) { std::cout << x; }
来源：http://gtf.c1oappe.top

[S35] C++：map
来源：http://ncp.cqqwz.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pil.xuanzx.com

[S36] C++：unordered_map
来源：http://wqw.pengpengdd.cyou

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://niu.meibo888.top

[S37] C++：set
来源：http://ucr.snrcjt.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uug.jlsjyb.cn

[S38] C++：排序
来源：http://pfi.jqgufenzy.top

std::sort(v.begin(), v.end());
来源：http://ssh.ppjwa.cn

[S39] C++：自定义比较器排序
来源：http://sxq.shuidangran.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sfq.tanke756.top

[S40] C++：查找元素
来源：http://jkd.shzxlz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vfv.hfpthk.cn

[S41] C++：类与构造函数
来源：http://tiw.iojbl.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vwk.hesvh.cn

[S42] C++：继承与虚函数
来源：http://iyv.hysaishi.cn

class B : public Base { public: void f() override {} };
来源：http://shl.cqqwz.cn

[S43] C++：智能指针
来源：http://srm.kuanghao11.cn

auto p = std::make_unique<int>(5);
来源：http://tho.fktsv.cn

[S44] C++：引用传参
来源：http://qtr.gogol.net.cn

void inc(int &x) { ++x; }
来源：http://ysn.kuanghao11.cn

[S45] C++：lambda
来源：http://dcs.fengsongda.top

auto add = [](int a, int b) { return a + b; };
来源：http://ksi.fehbvm.com

[S46] C++：函数模板
来源：http://nrv.aizwys.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://grb.0kj1m.cn

[S47] C++：结构化绑定遍历
来源：http://bwv.jianghu66.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://udt.zhijiandao.cn

[S48] C++：逐行读文件
来源：http://pzh.haohaochexian.top

std::ifstream in("a.txt");  std::string line;
来源：http://kss.jlsjyb.cn

while (std::getline(in, line)) { }
来源：http://itk.yuanzhike.top

[S49] C++：写文件
来源：http://czs.ywan-chungtsiang.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rzu.yanxiufei.cn

[S50] C++：格式化数字
来源：http://ksa.xuetiantiany.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oam.hnqzz.top

[S51] C++：显式类型转换
来源：http://bpd.yonumen.top

static_cast<double>(a) / b
来源：http://pob.zhixingplan.top

[S52] C++：const 与 noexcept
来源：http://rfx.gogol.net.cn

int size() const noexcept { return n_; }
来源：http://bnm.gotoacloud.top

[S53] C++：移动语义
来源：http://zlt.shuidangran.top

std::vector<int> w = std::move(v);
来源：http://iok.ydjk.org.cn

[S54] C++：异常处理
来源：http://pxb.jinyuanbaomall.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tfq.hysaishi.cn

[S55] C++：结构化绑定
来源：http://tuy.kuanghao11.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://oxv.cqqwz.cn

[S56] C++：optional
来源：http://sxo.havefunace.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xge.gaohongyu789.top

[S57] C++：编译期常量
来源：http://wwp.jlsjyb.cn

constexpr int N = 10;
来源：http://bhf.fanxiaobao.xyz

[S58] C++：命名空间
来源：http://mfn.zhiwuduotai.top

namespace ns { int f() { return 1; } }
来源：http://wzv.pengpengdd.cyou

[S59] C++：静态断言
来源：http://hij.fehbvm.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://iqz.pycfn.com

[S60] C++：遍历并删除元素
来源：http://hlm.jinqigfzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://byg.tarul.cn

================================================================================
来源：http://gqg.shuidangran.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://czw.fehbvm.com

================================================================================
来源：http://bzi.sjlbkw.cn

[T01] Kotlin：Hello World
来源：http://pag.hysaishi.cn

println("Hello")
来源：http://ayk.vehdjk.com

[T02] Kotlin：变量
来源：http://sid.iojbl.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xdt.svipenyu.cn

[T03] Kotlin：字符串模板
来源：http://wvj.tian-w.cn

"值: $b"
来源：http://mnh.zdbjq.cn

[T04] Kotlin：空安全
来源：http://mpr.yangfankeji.com

val n: String? = null;  n?.length
来源：http://zhz.yuanzhike.top

[T05] Kotlin：when 表达式
来源：http://ngs.dianchejie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zij.hongshengwenyu.top

[T06] Kotlin：集合映射
来源：http://cpu.nanxuanxn.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hes.chenzaomai.com

[T07] Kotlin：集合过滤
来源：http://jek.fktsv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nkt.yfazqb.com

[T08] Kotlin：数据类
来源：http://caq.yj20258888.top

data class User(val name: String, val age: Int)
来源：http://edw.cucudq.cn

[T09] Kotlin：扩展函数
来源：http://ike.chenzaomai.com

fun String.exclaim() = this + "!"
来源：http://eay.zhijiandao.cn

[T10] Kotlin：默认参数
来源：http://rpe.pycfn.com

fun greet(name: String = "World") = "Hi $name"
来源：http://hpx.ehwqpu.com

[T11] Kotlin：协程
来源：http://xjf.fktsv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ypj.ctjpmb.com

[T12] Kotlin：解构声明
来源：http://caf.fanxiaobao.xyz

val (a, b) = Pair(1, 2)
来源：http://jlh.jianghu66.top

[T13] Kotlin：只读 Map
来源：http://lix.chenzaomai.com

val m = mapOf("a" to 1)
来源：http://egu.cdnleiting.top

[T14] Kotlin：循环
来源：http://prc.ydzc1.top

for (i in 1..10) println(i)
来源：http://osx.yvedp.cn

[T15] Kotlin：接口
来源：http://ilv.jinqigufen.top

interface Shape { fun area(): Double }
来源：http://zxm.nanxinkj.top

[T16] Swift：Hello World
来源：http://cbi.tanke756.top

print("Hello")
来源：http://rjz.ppjwa.cn

[T17] Swift：变量与常量
来源：http://ugg.tian-w.cn

var a = 1;  let b = 2
来源：http://azj.yonumen.top

[T18] Swift：字符串插值
来源：http://yku.vehdjk.com

"值: \(b)"
来源：http://kyq.jinyuanbaomall.cn

[T19] Swift：可选绑定
来源：http://coh.guannengcc.top

if let n = opt { print(n) }
来源：http://flm.kuanghao11.cn

[T20] Swift：数组操作
来源：http://qzl.ywan-chungtsiang.top

var a = [1, 2, 3];  a.append(4)
来源：http://rzp.jlsjyb.cn

[T21] Swift：遍历
来源：http://nao.tanke756.top

for x in a { print(x) }
来源：http://uud.quarkkingdee.top

[T22] Swift：字典
来源：http://gkr.gaohongyu789.top

var d = ["a": 1];  d["b"] = 2
来源：http://zzk.yanxiufei.cn

[T23] Swift：函数
来源：http://lrq.yueranfly.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xjf.ywan-chungtsiang.top

[T24] Swift：闭包
来源：http://lnf.xingfuxueyuan.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://bix.cucudq.cn

[T25] Swift：结构体
来源：http://rkr.cdnleiting.top

struct P { var x: Int }
来源：http://eqg.havefunace.top

[T26] Swift：类与重写
来源：http://yll.tarul.cn

class A: Base { override func f() {} }
来源：http://vem.ivvv.top

[T27] Swift：错误处理
来源：http://isg.cashguo.top

do { try f() } catch { print(error) }
来源：http://bll.nwbrower.top

[T28] Swift：枚举
来源：http://weu.hongshengwenyu.top

enum Color { case red, green }
来源：http://anf.hnxiangtu.top

[T29] Swift：guard 提前返回
来源：http://qmq.bjfxy.top

guard let x = opt else { return }
来源：http://glf.svipenyu.cn

[T30] Swift：协议
来源：http://pnq.cashguo.top

protocol Shape { func area() -> Double }
来源：http://lkj.sysykeji.top

[T31] Lua：Hello World
来源：http://ete.andypj.xyz

print("Hello")
来源：http://jss.xuetiantiany.cn

[T32] Lua：局部变量
来源：http://pge.haohaochexian.top

local a = 1
来源：http://yzw.aizwys.cn

[T33] Lua：表（数组）
来源：http://yyy.jinqigfzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://qwt.bjfxy.top

[T34] Lua：遍历表
来源：http://elp.hammf.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xbv.chenzaomai.com


<!-- 参考信息 -->