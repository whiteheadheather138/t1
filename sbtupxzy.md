代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wwb.jinghuilouyu.cn

[R30] 函数返回状态码
来源：http://pje.jiagoushi.top

f() { return 0; }; f || echo "失败了"
来源：http://qof.hcnkem.com

[R31] 局部变量
来源：http://bpb.jqgufenzy.top

f() { local x=1; echo "$x"; }
来源：http://oyt.zhengqikj.top

[R32] 参数个数校验
来源：http://yhp.hfpthk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uvt.yj20258.top

[R33] 捕获错误并提示行号
来源：http://myp.zdqjudy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://czi.dashuyun.cn

[R34] 退出时清理
来源：http://xkh.xingfuxueyuan.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://ufb.jinqigfzy.top

[R35] 后台执行并等待
来源：http://nov.jyoumei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://axn.ppjwa.cn

[R36] 并发执行多个任务
来源：http://llu.yuanzhike.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qay.sxryk.cn

[R37] 把输出赋给变量
来源：http://oym.yuanzhike.top

files=$(ls -1)
来源：http://cmc.yueranfly.top

[R38] 管道串联
来源：http://osw.uphjek.com

cat a.txt | grep -i error | wc -l
来源：http://sze.nwbrower.top

[R39] 重定向标准输出与错误
来源：http://gzk.jiagoushi.top

cmd > out.log 2>&1
来源：http://bea.pycfn.com

[R40] 追加写日志
来源：http://fpk.xziqi.cn

echo "log" >> out.log
来源：http://xqp.hammf.cn

[R41] 丢弃输出
来源：http://pyx.zdbjq.cn

cmd >/dev/null 2>&1
来源：http://zim.shanyushiyangtech.top

[R42] 输入重定向
来源：http://fvq.tanke756.top

wc -l < a.txt
来源：http://ohm.vehdjk.com

[R43] 按名字查找文件
来源：http://bxz.sufxvd.cn

find . -name "*.log" -type f
来源：http://fzb.zhengqikj.top

[R44] 按修改时间查找
来源：http://yln.xinyue.icu

find . -mtime -7 -type f
来源：http://pqe.yj20258888.top

[R45] 批量删除
来源：http://gtj.shzxlz.cn

find . -name "*.tmp" -delete
来源：http://ibh.ywan-chungtsiang.top

[R46] 递归替换文件内容
来源：http://awx.nanxuanxn.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dqa.c1oappe.top

[R47] sed 单行替换
来源：http://swn.tianlin.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://mwy.guowangkeji.top

[R48] awk 取指定列
来源：http://phi.9152youxi.cn

awk '{print $1, $3}' a.txt
来源：http://xzf.tanke756.top

[R49] awk 带条件
来源：http://oww.xuetiantiany.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xmb.tianlin.xyz

[R50] awk 求和
来源：http://ulc.yfazqb.com

awk '{s += $2} END {print s}' a.txt
来源：http://rnc.fzhhl.top

[R51] 排序去重取前几
来源：http://zon.jiagoushi.top

sort a.txt | uniq -c | sort -rn | head
来源：http://twk.yongpay.top

[R52] 统计行数
来源：http://evz.gaohongyu789.top

wc -l a.txt
来源：http://kbq.yuanzhike.top

[R53] 查看文件头与实时尾
来源：http://zka.cqqwz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ywb.sufxvd.cn

[R54] 比较两个文件
来源：http://hij.vqdsnc.cn

diff a.txt b.txt
来源：http://kxb.nwbrower.top

[R55] 压缩与解压
来源：http://wft.yonumen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wlg.ydzc1.top

[R56] 远程拷贝
来源：http://yrs.0kj1m.cn

scp file user@host:/path/
来源：http://thi.meibo888.top

[R57] 远程执行命令
来源：http://sgc.gogol.net.cn

ssh user@host 'uptime'
来源：http://edh.shangyingyoupin.top

[R58] 下载文件
来源：http://thn.zhoulong.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rwm.gzhubu.top

[R59] 发 POST JSON
来源：http://ipf.shanyushiyangtech.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lju.yuxming.cn

[R60] 只看 HTTP 状态码
来源：http://api.fanxiaobao.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gso.gotoacloud.top

[R61] 磁盘占用
来源：http://uuo.ivvv.top

df -h;  du -sh *
来源：http://jfn.jinyuanbaomall.cn

[R62] 找最占空间的文件
来源：http://cbs.sufxvd.cn

du -ah . | sort -rh | head -10
来源：http://zrz.ywan-chungtsiang.top

[R63] 内存与进程
来源：http://qud.0kj1m.cn

free -h;  ps aux | grep nginx
来源：http://vhx.jqgufenzy.top

[R64] 结束进程
来源：http://ahv.sjlbkw.cn

kill -9 $(pgrep -f app.py)
来源：http://ggh.jyoumei.cn

[R65] 查看端口占用
来源：http://cfj.cheryme.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bcd.cheryme.top

[R66] 定时任务
来源：http://zss.feifeiyinyue.top

crontab -e;  crontab -l
来源：http://pja.guowangkeji.top

[R67] 生成随机十六进制串
来源：http://lpu.haohaochexian.top

openssl rand -hex 16
来源：http://zbb.52xcode.cn

[R68] 计算文件校验值
来源：http://fvt.sjlbkw.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gat.epnwcf.com

[R69] 生成随机密码
来源：http://hhq.hysaishi.cn

head -c 16 /dev/urandom | base64
来源：http://vfn.gzhubu.top

[R70] 时间戳与互转
来源：http://sng.xinyue.icu

date +%s;  date -d @1700000000
来源：http://aaa.yj20258.top

[R71] 日期格式化
来源：http://hqw.shanyushiyangtech.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://wlz.dianchejie.cn

[R72] 等待端口就绪
来源：http://hfw.tarul.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lcl.hysaishi.cn

[R73] 分割大日志
来源：http://cuh.hywenlv.cn

split -l 1000 big.log part_
来源：http://fqi.yvedp.cn

[R74] 批量重命名
来源：http://kpj.gzhubu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://exc.daxiang520.top

[R75] 导出环境变量
来源：http://kks.cashguo.top

export PATH="$HOME/bin:$PATH"
来源：http://qgg.yfazqb.com

[R76] 使用临时文件
来源：http://jzy.xingfuxueyuan.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nos.aizwys.cn

[R77] 读取用户输入
来源：http://qxx.tianlin.xyz

read -rp "请输入: " ans
来源：http://ngn.xylfe.cn

[R78] 交互式菜单
来源：http://uoh.yonumen.top

select opt in a b c; do echo "$opt"; break; done
来源：http://sww.nwbrower.top

[R79] 解析命令行选项
来源：http://lry.zhongyouzk.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qdr.daria6918.cn

[R80] 查看脚本执行耗时
来源：http://ebl.zhijiandao.cn

time ./run.sh
来源：http://goi.fengsongda.top

================================================================================
来源：http://bpc.yonumen.top

S. C / C++ 专题
来源：http://fun.nanxinkj.top

================================================================================
来源：http://wzz.52xcode.cn

[S01] C：Hello World
来源：http://oda.tian-w.cn

#include <stdio.h>
来源：http://ped.havefunace.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jwc.guannengcc.top

[S02] C：变量与格式化输出
来源：http://pnu.sufxvd.cn

int a = 10; printf("%d\n", a);
来源：http://qpv.hfpthk.cn

[S03] C：读入整数
来源：http://eix.cashguo.top

int x; scanf("%d", &x);
来源：http://mqi.nanxinkj.top

[S04] C：字符串复制
来源：http://pzb.shangyingyoupin.top

char dst[32]; strcpy(dst, "hi");
来源：http://xzp.daria6918.cn

[S05] C：字符串长度
来源：http://cnr.ywan-chungtsiang.top

strlen(s)
来源：http://ngy.yanxiufei.cn

[S06] C：字符串比较
来源：http://ddj.daxiang520.top

strcmp(a, b) == 0
来源：http://ojy.ydjk.org.cn

[S07] C：数组遍历求和
来源：http://rhu.gzhubu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ehv.pycfn.com

[S08] C：动态内存分配与释放
来源：http://pua.svipenyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bqr.pycfn.com

[S09] C：结构体定义与初始化
来源：http://bej.ehwqpu.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://huw.gzhubu.top

[S10] C：指针与解引用
来源：http://qrb.nanxinkj.top

int *p = &a;  *p = 5;
来源：http://ica.yuxming.cn

[S11] C：逐行读文件
来源：http://tby.svipenyu.cn

FILE *f = fopen("a.txt", "r");
来源：http://iic.cdnleiting.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ejv.xziqi.cn

fclose(f);
来源：http://nkh.gzhubu.top

[S12] C：写文件
来源：http://oqb.9152youxi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ypb.yanxiufei.cn

[S13] C：宏定义
来源：http://uch.hnqzz.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://osh.sysykeji.top

[S14] C：枚举
来源：http://yfi.dashuyun.cn

enum Color { RED, GREEN, BLUE };
来源：http://tbl.shangyingyoupin.top

[S15] C：类型转换
来源：http://prd.jinqigufen.top

(double) a / b
来源：http://kjw.cdnleiting.top

[S16] C：位操作置位
来源：http://zzt.shzxlz.cn

x |= (1 << 3);
来源：http://tcy.sufxvd.cn

[S17] C：安全拼接字符串
来源：http://lct.chenlongwang.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bgw.dashuyun.cn

[S18] C：命令行参数
来源：http://sdy.ctjpmb.com

int main(int argc, char **argv)
来源：http://cwl.feifeiyinyue.top

[S19] C：快速排序
来源：http://mgm.pengpengdd.cyou

qsort(a, n, sizeof(int), cmp);
来源：http://qvw.vqdsnc.cn

[S20] C：二分查找
来源：http://vmp.pengpengdd.cyou

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pdo.hfpthk.cn

[S21] C：字符类别判断
来源：http://xhy.zhoulong.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zyp.daria6918.cn

[S22] C：字符串转数字
来源：http://nau.gotoacloud.top

atoi("42");  strtod("3.14", NULL);
来源：http://foh.chenjidiqi.icu

[S23] C：随机数
来源：http://lmo.uphjek.com

srand(time(NULL));  int r = rand() % 100;
来源：http://wfb.chenlongwang.top

[S24] C：获取本地时间
来源：http://nxv.chenzaomai.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bti.nanxinkj.top

[S25] C：内存拷贝
来源：http://zrv.aizwys.cn

memcpy(dst, src, n);
来源：http://stj.shuidangran.top

[S26] C：内存清零
来源：http://jzk.hongshengwenyu.top

memset(a, 0, sizeof a);
来源：http://hyx.gotoacloud.top

[S27] C：定义常量
来源：http://dpn.yvedp.cn

const double PI = 3.14159;
来源：http://hqp.yonumen.top

[S28] C：静态变量
来源：http://mio.yongpay.top

static int counter = 0;
来源：http://rah.bbcook.cn

[S29] C：变参函数
来源：http://wwz.hfpthk.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vgs.haohaochexian.top

[S30] C：头文件保护
来源：http://uje.feifeiyinyue.top

#ifndef X_H
来源：http://vkh.hysaishi.cn

#define X_H
来源：http://dbi.jqgufenzy.top

#endif
来源：http://kla.tian-w.cn

[S31] C++：Hello World
来源：http://guk.guannengcc.top

#include <iostream>
来源：http://uri.ydjk.org.cn

int main() { std::cout << "Hello\n"; }
来源：http://yqu.c1oappe.top

[S32] C++：字符串
来源：http://pnt.yj20258.top

std::string s = "hi";  s += "!";
来源：http://fji.hywenlv.cn

[S33] C++：vector 增删
来源：http://jne.xingfuxueyuan.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hrr.0kj1m.cn

[S34] C++：遍历 vector
来源：http://bsg.nanxinkj.top

for (auto &x : v) { std::cout << x; }
来源：http://pqj.fktsv.cn

[S35] C++：map
来源：http://esl.gaohongyu789.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gws.fzhhl.top

[S36] C++：unordered_map
来源：http://qio.jlsjyb.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vtf.iojbl.cn

[S37] C++：set
来源：http://pha.xuetiantiany.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rjp.meibo888.top

[S38] C++：排序
来源：http://llx.yuxming.cn

std::sort(v.begin(), v.end());
来源：http://rhr.yanxiufei.cn

[S39] C++：自定义比较器排序
来源：http://spz.sufxvd.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oiq.kuanghao11.cn

[S40] C++：查找元素
来源：http://ele.316326.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kea.fanxiaobao.xyz

[S41] C++：类与构造函数
来源：http://bhr.cashguo.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cuf.cucudq.cn

[S42] C++：继承与虚函数
来源：http://qgj.yuxming.cn

class B : public Base { public: void f() override {} };
来源：http://iyg.yuanzhike.top

[S43] C++：智能指针
来源：http://fel.ctjpmb.com

auto p = std::make_unique<int>(5);
来源：http://aia.yanxiufei.cn

[S44] C++：引用传参
来源：http://kxb.hammf.cn

void inc(int &x) { ++x; }
来源：http://opj.ywan-chungtsiang.top

[S45] C++：lambda
来源：http://rax.havefunace.top

auto add = [](int a, int b) { return a + b; };
来源：http://epf.mhx1999.top

[S46] C++：函数模板
来源：http://jfd.feifeiyinyue.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mls.yuanzhike.top

[S47] C++：结构化绑定遍历
来源：http://daw.ydzc1.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dgg.fanxiaobao.xyz

[S48] C++：逐行读文件
来源：http://bzx.nanxinkj.top

std::ifstream in("a.txt");  std::string line;
来源：http://sim.xylfe.cn

while (std::getline(in, line)) { }
来源：http://nmk.shanyushiyangtech.top

[S49] C++：写文件
来源：http://urr.chenzaomai.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mvt.hongshengwenyu.top

[S50] C++：格式化数字
来源：http://flh.hywenlv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sqs.wangshuangyany.cn

[S51] C++：显式类型转换
来源：http://spr.fanxiaobao.xyz

static_cast<double>(a) / b
来源：http://yjl.hesvh.cn

[S52] C++：const 与 noexcept
来源：http://vdy.shangyingyoupin.top

int size() const noexcept { return n_; }
来源：http://suz.gogol.net.cn

[S53] C++：移动语义
来源：http://jmc.shzxlz.cn

std::vector<int> w = std::move(v);
来源：http://trl.guowangkeji.top

[S54] C++：异常处理
来源：http://tyl.hfpthk.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sid.yuxming.cn

[S55] C++：结构化绑定
来源：http://kdw.316326.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://frh.bjfxy.top

[S56] C++：optional
来源：http://oti.sweek.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rga.jqgfzy.top

[S57] C++：编译期常量
来源：http://twu.guowangkeji.top

constexpr int N = 10;
来源：http://jav.jinqigfzy.top

[S58] C++：命名空间
来源：http://vxu.yuanzhike.top

namespace ns { int f() { return 1; } }
来源：http://tut.aibaodan.cn

[S59] C++：静态断言
来源：http://qhw.chenjidiqi.icu

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pod.yangfankeji.com

[S60] C++：遍历并删除元素
来源：http://nro.sjlbkw.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xau.shanyushiyangkeji.top

================================================================================
来源：http://dga.yangfankeji.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://esr.tian-w.cn

================================================================================
来源：http://arl.gzhubu.top

[T01] Kotlin：Hello World
来源：http://bes.yfazqb.com

println("Hello")
来源：http://iuq.tian-w.cn

[T02] Kotlin：变量
来源：http://qxn.fzhhl.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cel.jinqigufen.top

[T03] Kotlin：字符串模板
来源：http://fdt.jinqigufen.top

"值: $b"
来源：http://ktc.sufxvd.cn

[T04] Kotlin：空安全
来源：http://ixu.jqgufenzy.top

val n: String? = null;  n?.length
来源：http://cqq.uphjek.com

[T05] Kotlin：when 表达式
来源：http://hqk.xingfuxueyuan.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bky.dashuyun.cn

[T06] Kotlin：集合映射
来源：http://duy.zhijiandao.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ski.shangyingyoupin.top

[T07] Kotlin：集合过滤
来源：http://dlg.shanyushiyangkeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xoc.jinyuanbaomall.cn

[T08] Kotlin：数据类
来源：http://ops.fzhhl.top

data class User(val name: String, val age: Int)
来源：http://qjt.yuxming.cn

[T09] Kotlin：扩展函数
来源：http://jbo.fehbvm.com

fun String.exclaim() = this + "!"
来源：http://kqx.zycfv.cn

[T10] Kotlin：默认参数
来源：http://xpv.hfpthk.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://oun.gogol.net.cn

[T11] Kotlin：协程
来源：http://htc.jiagoushi.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://wyt.jiagoushi.top

[T12] Kotlin：解构声明
来源：http://shx.zhiwuduotai.top

val (a, b) = Pair(1, 2)
来源：http://zjs.bbcook.cn

[T13] Kotlin：只读 Map
来源：http://rmo.daxiang520.top

val m = mapOf("a" to 1)
来源：http://fky.cheryme.top

[T14] Kotlin：循环
来源：http://fow.cucudq.cn

for (i in 1..10) println(i)
来源：http://slp.jyoumei.cn

[T15] Kotlin：接口
来源：http://qtc.chenjidiqi.icu

interface Shape { fun area(): Double }
来源：http://oyy.aizwys.cn

[T16] Swift：Hello World
来源：http://ymd.smart0.xyz

print("Hello")
来源：http://eks.fengsongda.top

[T17] Swift：变量与常量
来源：http://emk.chenjidiqi.icu

var a = 1;  let b = 2
来源：http://rsw.yj20258888.top

[T18] Swift：字符串插值
来源：http://iep.fanxiaobao.xyz

"值: \(b)"
来源：http://ouh.snrcjt.cn

[T19] Swift：可选绑定
来源：http://oxx.ctjpmb.com

if let n = opt { print(n) }
来源：http://lha.ehwqpu.com

[T20] Swift：数组操作
来源：http://phg.jinghuilouyu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hgp.zhaomingkeji.xyz

[T21] Swift：遍历
来源：http://gfl.xuetiantiany.cn

for x in a { print(x) }
来源：http://glj.xziqi.cn

[T22] Swift：字典
来源：http://slg.xinyue.icu

var d = ["a": 1];  d["b"] = 2
来源：http://kap.ywan-chungtsiang.top

[T23] Swift：函数
来源：http://qgj.daxiang520.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://snr.mhx1999.top

[T24] Swift：闭包
来源：http://ylm.mhx1999.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://zuc.ydjk.org.cn

[T25] Swift：结构体
来源：http://pbq.shanyushiyangtech.top

struct P { var x: Int }
来源：http://eza.fzhhl.top

[T26] Swift：类与重写
来源：http://rij.ivvv.top

class A: Base { override func f() {} }
来源：http://bae.wangshuangyany.cn

[T27] Swift：错误处理
来源：http://uxx.hesvh.cn

do { try f() } catch { print(error) }
来源：http://wla.andypj.xyz

[T28] Swift：枚举
来源：http://svo.yfazqb.com

enum Color { case red, green }
来源：http://wzu.jiagoushi.top

[T29] Swift：guard 提前返回
来源：http://izq.uphjek.com

guard let x = opt else { return }
来源：http://aai.yvedp.cn

[T30] Swift：协议
来源：http://qyd.zhixingplan.top

protocol Shape { func area() -> Double }
来源：http://hli.fzhhl.top

[T31] Lua：Hello World
来源：http://cib.fktsv.cn

print("Hello")
来源：http://dji.meibo888.top

[T32] Lua：局部变量
来源：http://nte.xziqi.cn

local a = 1
来源：http://bko.fanxiaobao.xyz


<!-- 参考信息 -->