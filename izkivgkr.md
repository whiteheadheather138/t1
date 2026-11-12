代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://njs.yangfankeji.com

[R34] 退出时清理
来源：http://cfe.shuidangran.top

trap 'rm -f "$tmp"' EXIT
来源：http://gib.ppjwa.cn

[R35] 后台执行并等待
来源：http://qvt.chenlongwang.top

sleep 5 & pid=$!; wait "$pid"
来源：http://onm.zycfv.cn

[R36] 并发执行多个任务
来源：http://xql.jinyuanbaomall.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qrm.yfazqb.com

[R37] 把输出赋给变量
来源：http://iwg.jinqigfzy.top

files=$(ls -1)
来源：http://idu.hnxiangtu.top

[R38] 管道串联
来源：http://att.havefunace.top

cat a.txt | grep -i error | wc -l
来源：http://qay.sxryk.cn

[R39] 重定向标准输出与错误
来源：http://wkb.yj202588.top

cmd > out.log 2>&1
来源：http://exr.tanke756.top

[R40] 追加写日志
来源：http://fja.ppjwa.cn

echo "log" >> out.log
来源：http://ntm.bbcook.cn

[R41] 丢弃输出
来源：http://joi.cdnleiting.top

cmd >/dev/null 2>&1
来源：http://bgr.birdmap.top

[R42] 输入重定向
来源：http://jbs.guowangkeji.top

wc -l < a.txt
来源：http://kwp.havefunace.top

[R43] 按名字查找文件
来源：http://tmq.zhengqikj.top

find . -name "*.log" -type f
来源：http://uzq.hcnkem.com

[R44] 按修改时间查找
来源：http://ccm.hnqzz.top

find . -mtime -7 -type f
来源：http://rrw.jqgfzy.top

[R45] 批量删除
来源：http://ckk.kuanghao11.cn

find . -name "*.tmp" -delete
来源：http://oma.zhijiandao.cn

[R46] 递归替换文件内容
来源：http://zsk.c1oappe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jmt.hnxiangtu.top

[R47] sed 单行替换
来源：http://kby.9152youxi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rtt.jinghuilouyu.cn

[R48] awk 取指定列
来源：http://pwr.yvedp.cn

awk '{print $1, $3}' a.txt
来源：http://wow.hcnkem.com

[R49] awk 带条件
来源：http://wlz.gzhubu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vmk.jinqigfzy.top

[R50] awk 求和
来源：http://oii.gogol.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xlt.jlsjyb.cn

[R51] 排序去重取前几
来源：http://sdf.yfazqb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://yqt.hfpthk.cn

[R52] 统计行数
来源：http://fxy.snrcjt.cn

wc -l a.txt
来源：http://siw.daria6918.cn

[R53] 查看文件头与实时尾
来源：http://cgn.yonumen.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ehy.sjlbkw.cn

[R54] 比较两个文件
来源：http://efz.pengpengdd.cyou

diff a.txt b.txt
来源：http://qtu.birdmap.top

[R55] 压缩与解压
来源：http://yol.sxryk.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hxm.uphjek.com

[R56] 远程拷贝
来源：http://ctl.hammf.cn

scp file user@host:/path/
来源：http://udc.nwbrower.top

[R57] 远程执行命令
来源：http://mzc.zycfv.cn

ssh user@host 'uptime'
来源：http://ngf.aizwys.cn

[R58] 下载文件
来源：http://baa.yj20258888.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rei.fanxiaobao.xyz

[R59] 发 POST JSON
来源：http://gww.ydzc1.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zwr.jqgfzy.top

[R60] 只看 HTTP 状态码
来源：http://kkq.yj20258.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cpe.yanxiufei.cn

[R61] 磁盘占用
来源：http://xze.fengsongda.top

df -h;  du -sh *
来源：http://emv.zdbjq.cn

[R62] 找最占空间的文件
来源：http://zqs.zdbjq.cn

du -ah . | sort -rh | head -10
来源：http://tot.snrcjt.cn

[R63] 内存与进程
来源：http://pud.dianchejie.cn

free -h;  ps aux | grep nginx
来源：http://ncv.daria6918.cn

[R64] 结束进程
来源：http://stt.yangfankeji.com

kill -9 $(pgrep -f app.py)
来源：http://snp.tianlin.xyz

[R65] 查看端口占用
来源：http://ykb.yuxming.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hjx.nwbrower.top

[R66] 定时任务
来源：http://typ.gaohongyu789.top

crontab -e;  crontab -l
来源：http://nwv.yvedp.cn

[R67] 生成随机十六进制串
来源：http://xyo.ydzc1.top

openssl rand -hex 16
来源：http://ace.ehwqpu.com

[R68] 计算文件校验值
来源：http://osq.yj202588.top

sha256sum a.txt;  md5sum a.txt
来源：http://swg.hysaishi.cn

[R69] 生成随机密码
来源：http://nfi.yuanzhike.top

head -c 16 /dev/urandom | base64
来源：http://psd.yuanzhike.top

[R70] 时间戳与互转
来源：http://nhj.yangfankeji.com

date +%s;  date -d @1700000000
来源：http://jpa.cashguo.top

[R71] 日期格式化
来源：http://jxq.ctjpmb.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://dxf.jyoumei.cn

[R72] 等待端口就绪
来源：http://rvb.zdbjq.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hsn.xingfuxueyuan.xyz

[R73] 分割大日志
来源：http://qvh.kuanghao11.cn

split -l 1000 big.log part_
来源：http://joj.zycfv.cn

[R74] 批量重命名
来源：http://pdu.daxiang520.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lpz.yangfankeji.com

[R75] 导出环境变量
来源：http://tkh.feifeiyinyue.top

export PATH="$HOME/bin:$PATH"
来源：http://adp.fktsv.cn

[R76] 使用临时文件
来源：http://qny.andypj.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://shz.sjlbkw.cn

[R77] 读取用户输入
来源：http://fuu.pengpengdd.cyou

read -rp "请输入: " ans
来源：http://grx.bjfxy.top

[R78] 交互式菜单
来源：http://zba.yangfankeji.com

select opt in a b c; do echo "$opt"; break; done
来源：http://kdq.yangfankeji.com

[R79] 解析命令行选项
来源：http://rwx.chenjidiqi.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wjj.zhaomingkeji.xyz

[R80] 查看脚本执行耗时
来源：http://jvk.smart0.xyz

time ./run.sh
来源：http://sut.cashguo.top

================================================================================
来源：http://kpw.ywan-chungtsiang.top

S. C / C++ 专题
来源：http://kvc.yueranfly.top

================================================================================
来源：http://vjc.feifeiyinyue.top

[S01] C：Hello World
来源：http://fou.sxryk.cn

#include <stdio.h>
来源：http://qfh.hywenlv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zjj.xinyue.icu

[S02] C：变量与格式化输出
来源：http://umv.jinqigfzy.top

int a = 10; printf("%d\n", a);
来源：http://xlu.c1oappe.top

[S03] C：读入整数
来源：http://egh.xuetiantiany.cn

int x; scanf("%d", &x);
来源：http://cmv.ppjwa.cn

[S04] C：字符串复制
来源：http://utj.yuxming.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cqk.cheryme.top

[S05] C：字符串长度
来源：http://hpl.vehdjk.com

strlen(s)
来源：http://cdt.yj20258888.top

[S06] C：字符串比较
来源：http://joa.zhiwuduotai.top

strcmp(a, b) == 0
来源：http://wsx.epnwcf.com

[S07] C：数组遍历求和
来源：http://gky.yueranfly.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fjl.zdqjudy.top

[S08] C：动态内存分配与释放
来源：http://wej.jianghu66.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bvc.jinghuilouyu.cn

[S09] C：结构体定义与初始化
来源：http://llx.yfazqb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nkd.chenjidiqi.icu

[S10] C：指针与解引用
来源：http://ulv.pycfn.com

int *p = &a;  *p = 5;
来源：http://zrq.meibo888.top

[S11] C：逐行读文件
来源：http://psn.yonumen.top

FILE *f = fopen("a.txt", "r");
来源：http://coh.zhaomingkeji.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://ama.yj20258888.top

fclose(f);
来源：http://jrx.jinyuanbaomall.cn

[S12] C：写文件
来源：http://qlh.shangyingyoupin.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uxb.bjfxy.top

[S13] C：宏定义
来源：http://ock.yj202588.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tvd.epnwcf.com

[S14] C：枚举
来源：http://wob.tanke756.top

enum Color { RED, GREEN, BLUE };
来源：http://hbb.meibo888.top

[S15] C：类型转换
来源：http://hgw.c1oappe.top

(double) a / b
来源：http://uii.xuetiantiany.cn

[S16] C：位操作置位
来源：http://ntu.hysaishi.cn

x |= (1 << 3);
来源：http://ekl.sxryk.cn

[S17] C：安全拼接字符串
来源：http://pxt.ppjwa.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ebi.havefunace.top

[S18] C：命令行参数
来源：http://tdz.yueranfly.top

int main(int argc, char **argv)
来源：http://cqg.ywan-chungtsiang.top

[S19] C：快速排序
来源：http://uiy.quarkkingdee.top

qsort(a, n, sizeof(int), cmp);
来源：http://hgg.tarul.cn

[S20] C：二分查找
来源：http://nka.daxiang520.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://deg.zhiwuduotai.top

[S21] C：字符类别判断
来源：http://xzx.fzhhl.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kmt.guowangkeji.top

[S22] C：字符串转数字
来源：http://sra.tianlin.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://nfl.fehbvm.com

[S23] C：随机数
来源：http://cib.yueranfly.top

srand(time(NULL));  int r = rand() % 100;
来源：http://tqp.cashguo.top

[S24] C：获取本地时间
来源：http://ulr.yvedp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://olv.jianghu66.top

[S25] C：内存拷贝
来源：http://rpd.52xcode.cn

memcpy(dst, src, n);
来源：http://zxu.redwolf501.top

[S26] C：内存清零
来源：http://ujd.yueranfly.top

memset(a, 0, sizeof a);
来源：http://csr.c1oappe.top

[S27] C：定义常量
来源：http://fff.yj202588.top

const double PI = 3.14159;
来源：http://azu.havefunace.top

[S28] C：静态变量
来源：http://qfh.cashguo.top

static int counter = 0;
来源：http://yex.gaohongyu789.top

[S29] C：变参函数
来源：http://amb.zdbjq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jaa.birdmap.top

[S30] C：头文件保护
来源：http://rrf.daxiang520.top

#ifndef X_H
来源：http://ktk.pengpengdd.cyou

#define X_H
来源：http://fla.yj20258888.top

#endif
来源：http://agv.tian-w.cn

[S31] C++：Hello World
来源：http://mpd.shanyushiyangtech.top

#include <iostream>
来源：http://ade.yuxming.cn

int main() { std::cout << "Hello\n"; }
来源：http://ztn.xylfe.cn

[S32] C++：字符串
来源：http://rlb.zycfv.cn

std::string s = "hi";  s += "!";
来源：http://srr.gogol.net.cn

[S33] C++：vector 增删
来源：http://qpf.guowangkeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dil.fehbvm.com

[S34] C++：遍历 vector
来源：http://skl.wangshuangyany.cn

for (auto &x : v) { std::cout << x; }
来源：http://egs.ctjpmb.com

[S35] C++：map
来源：http://tkz.jianghu66.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wfb.jyoumei.cn

[S36] C++：unordered_map
来源：http://qdx.nanxinkj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iuq.hfpthk.cn

[S37] C++：set
来源：http://tky.zhixingplan.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rmf.redwolf501.top

[S38] C++：排序
来源：http://dlg.vehdjk.com

std::sort(v.begin(), v.end());
来源：http://crn.andypj.xyz

[S39] C++：自定义比较器排序
来源：http://zbi.iojbl.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kjj.shuidangran.top

[S40] C++：查找元素
来源：http://fzf.hongshengwenyu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xer.hongshengwenyu.top

[S41] C++：类与构造函数
来源：http://xyi.sufxvd.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ozr.yueranfly.top

[S42] C++：继承与虚函数
来源：http://jeg.cqqwz.cn

class B : public Base { public: void f() override {} };
来源：http://xrg.gogol.net.cn

[S43] C++：智能指针
来源：http://xyf.jqgufenzy.top

auto p = std::make_unique<int>(5);
来源：http://lxf.jinqigufen.top

[S44] C++：引用传参
来源：http://aab.cdnleiting.top

void inc(int &x) { ++x; }
来源：http://klu.guannengcc.top

[S45] C++：lambda
来源：http://kjt.hongshengwenyu.top

auto add = [](int a, int b) { return a + b; };
来源：http://dhj.andypj.xyz

[S46] C++：函数模板
来源：http://hap.fehbvm.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yis.chenlongwang.top

[S47] C++：结构化绑定遍历
来源：http://gbr.fzhhl.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cvo.havefunace.top

[S48] C++：逐行读文件
来源：http://qqh.iojbl.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jfv.zdqjudy.top

while (std::getline(in, line)) { }
来源：http://wmq.shuidangran.top

[S49] C++：写文件
来源：http://lhv.jqgfzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uhv.yfazqb.com

[S50] C++：格式化数字
来源：http://utl.hongshengwenyu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oqy.vqdsnc.cn

[S51] C++：显式类型转换
来源：http://mnl.9152youxi.cn

static_cast<double>(a) / b
来源：http://xfi.shanyushiyangkeji.top

[S52] C++：const 与 noexcept
来源：http://tqp.0kj1m.cn

int size() const noexcept { return n_; }
来源：http://ihq.jinyuanbaomall.cn

[S53] C++：移动语义
来源：http://ear.cashguo.top

std::vector<int> w = std::move(v);
来源：http://bqn.chenjidiqi.icu

[S54] C++：异常处理
来源：http://muh.chenzaomai.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://egf.bbcook.cn

[S55] C++：结构化绑定
来源：http://gtm.zdbjq.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://was.zhiwuduotai.top

[S56] C++：optional
来源：http://tkx.zhengqikj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uhi.sysykeji.top

[S57] C++：编译期常量
来源：http://lyx.shanyushiyangtech.top

constexpr int N = 10;
来源：http://nxw.hysaishi.cn

[S58] C++：命名空间
来源：http://few.yj20258888.top

namespace ns { int f() { return 1; } }
来源：http://xbj.zhixingplan.top

[S59] C++：静态断言
来源：http://hag.jiagoushi.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://srv.epnwcf.com

[S60] C++：遍历并删除元素
来源：http://rzz.jianghu66.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://iww.havefunace.top

================================================================================
来源：http://dno.zhongyouzk.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uag.fehbvm.com

================================================================================
来源：http://zqh.wangdashe.top

[T01] Kotlin：Hello World
来源：http://rvx.xuanzx.com

println("Hello")
来源：http://ayw.xziqi.cn

[T02] Kotlin：变量
来源：http://cym.zhoulong.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pto.hesvh.cn

[T03] Kotlin：字符串模板
来源：http://crp.ehwqpu.com

"值: $b"
来源：http://yzn.0kj1m.cn

[T04] Kotlin：空安全
来源：http://cah.cheryme.top

val n: String? = null;  n?.length
来源：http://msh.andypj.xyz

[T05] Kotlin：when 表达式
来源：http://fye.tanke756.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gjx.gogol.net.cn

[T06] Kotlin：集合映射
来源：http://qix.yfazqb.com

listOf(1, 2, 3).map { it * 2 }
来源：http://jmj.ehwqpu.com

[T07] Kotlin：集合过滤
来源：http://vcq.zhixingplan.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://lhc.hammf.cn

[T08] Kotlin：数据类
来源：http://pmb.sweek.top

data class User(val name: String, val age: Int)
来源：http://pzl.ydzc1.top

[T09] Kotlin：扩展函数
来源：http://mbw.zycfv.cn

fun String.exclaim() = this + "!"
来源：http://qwn.xingfuxueyuan.xyz

[T10] Kotlin：默认参数
来源：http://gag.daria6918.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://akg.aizwys.cn

[T11] Kotlin：协程
来源：http://acg.tanke756.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://atm.sxryk.cn

[T12] Kotlin：解构声明
来源：http://ofh.wangshuangyany.cn

val (a, b) = Pair(1, 2)
来源：http://dvp.fanxiaobao.xyz

[T13] Kotlin：只读 Map
来源：http://cfb.xuanzx.com

val m = mapOf("a" to 1)
来源：http://jig.jiagoushi.top

[T14] Kotlin：循环
来源：http://gbx.feifeiyinyue.top

for (i in 1..10) println(i)
来源：http://zmb.yj20258888.top

[T15] Kotlin：接口
来源：http://rrj.hesvh.cn

interface Shape { fun area(): Double }
来源：http://yaw.yfazqb.com

[T16] Swift：Hello World
来源：http://meb.yj20258.top

print("Hello")
来源：http://opz.jianghu66.top

[T17] Swift：变量与常量
来源：http://lks.zhijiandao.cn

var a = 1;  let b = 2
来源：http://mdj.ehwqpu.com

[T18] Swift：字符串插值
来源：http://ksi.mhx1999.top

"值: \(b)"
来源：http://kbx.wangshuangyany.cn

[T19] Swift：可选绑定
来源：http://uvc.birdmap.top

if let n = opt { print(n) }
来源：http://nff.pengpengdd.cyou

[T20] Swift：数组操作
来源：http://vrb.mhx1999.top

var a = [1, 2, 3];  a.append(4)
来源：http://wmp.ivvv.top

[T21] Swift：遍历
来源：http://hpk.zhiwuduotai.top

for x in a { print(x) }
来源：http://hpb.snrcjt.cn

[T22] Swift：字典
来源：http://mqo.hnxiangtu.top

var d = ["a": 1];  d["b"] = 2
来源：http://qra.jlsjyb.cn

[T23] Swift：函数
来源：http://ylh.fanxiaobao.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yku.bbcook.cn

[T24] Swift：闭包
来源：http://rcy.yvedp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yql.nanxuanxn.top

[T25] Swift：结构体
来源：http://ppl.vehdjk.com

struct P { var x: Int }
来源：http://nwb.sxryk.cn

[T26] Swift：类与重写
来源：http://rlc.smart0.xyz

class A: Base { override func f() {} }
来源：http://uaw.meibo888.top

[T27] Swift：错误处理
来源：http://vkx.chenzaomai.com

do { try f() } catch { print(error) }
来源：http://pxr.52xcode.cn

[T28] Swift：枚举
来源：http://kwh.epnwcf.com

enum Color { case red, green }
来源：http://vvt.sjlbkw.cn

[T29] Swift：guard 提前返回
来源：http://tvt.zhiwuduotai.top

guard let x = opt else { return }
来源：http://zvy.52xcode.cn

[T30] Swift：协议
来源：http://umk.dashuyun.cn

protocol Shape { func area() -> Double }
来源：http://lwt.cashguo.top

[T31] Lua：Hello World
来源：http://lbp.zhaomingkeji.xyz

print("Hello")
来源：http://lwa.guannengcc.top

[T32] Lua：局部变量
来源：http://hwr.mhx1999.top

local a = 1
来源：http://hdo.xylfe.cn

[T33] Lua：表（数组）
来源：http://sgw.sweek.top

local t = {1, 2, 3};  t[4] = 4
来源：http://prn.yangfankeji.com

[T34] Lua：遍历表
来源：http://sha.hcnkem.com

for i, v in ipairs(t) do print(i, v) end
来源：http://uji.ydjk.org.cn

[T35] Lua：字典表
来源：http://mxw.jlsjyb.cn

local d = { a = 1 };  d.b = 2
来源：http://yhf.yuanzhike.top

[T36] Lua：函数
来源：http://bpt.xziqi.cn

function add(a, b) return a + b end
来源：http://naj.iojbl.cn


<!-- 参考信息 -->