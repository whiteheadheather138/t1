代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://xdb.hcnkem.com

[R26] 命令替换
来源：http://dso.sufxvd.cn

now=$(date +%F); echo "$now"
来源：http://pni.hammf.cn

[R27] 算术展开
来源：http://tsa.zycfv.cn

echo $((1 + 2 * 3))
来源：http://kfd.gogol.net.cn

[R28] 浮点运算
来源：http://mno.jlsjyb.cn

echo "scale=2; 10/3" | bc
来源：http://mog.cheryme.top

[R29] 定义函数
来源：http://owm.fktsv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cxi.bbcook.cn

[R30] 函数返回状态码
来源：http://jow.hywenlv.cn

f() { return 0; }; f || echo "失败了"
来源：http://lyg.yangfankeji.com

[R31] 局部变量
来源：http://yfh.jinghuilouyu.cn

f() { local x=1; echo "$x"; }
来源：http://ifa.ywan-chungtsiang.top

[R32] 参数个数校验
来源：http://jpy.shuidangran.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pfo.xingfuxueyuan.xyz

[R33] 捕获错误并提示行号
来源：http://jxc.ybcxt.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jsz.zhoulong.xyz

[R34] 退出时清理
来源：http://yzs.birdmap.top

trap 'rm -f "$tmp"' EXIT
来源：http://xpc.zhiwuduotai.top

[R35] 后台执行并等待
来源：http://ksu.daria6918.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jzc.jianghu66.top

[R36] 并发执行多个任务
来源：http://zeu.daria6918.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fzc.chenjidiqi.icu

[R37] 把输出赋给变量
来源：http://iqn.jinyuanbaomall.cn

files=$(ls -1)
来源：http://ltk.hfpthk.cn

[R38] 管道串联
来源：http://ebl.hysaishi.cn

cat a.txt | grep -i error | wc -l
来源：http://cda.jinqigfzy.top

[R39] 重定向标准输出与错误
来源：http://tfp.c1oappe.top

cmd > out.log 2>&1
来源：http://eki.guowangkeji.top

[R40] 追加写日志
来源：http://eil.wangdashe.top

echo "log" >> out.log
来源：http://zno.daxiang520.top

[R41] 丢弃输出
来源：http://bxb.yj20258888.top

cmd >/dev/null 2>&1
来源：http://hxq.zhengqikj.top

[R42] 输入重定向
来源：http://pjx.uphjek.com

wc -l < a.txt
来源：http://qao.ppjwa.cn

[R43] 按名字查找文件
来源：http://kbg.wangshuangyany.cn

find . -name "*.log" -type f
来源：http://jvn.vqdsnc.cn

[R44] 按修改时间查找
来源：http://izv.ivvv.top

find . -mtime -7 -type f
来源：http://vqa.gotoacloud.top

[R45] 批量删除
来源：http://vor.zhengqikj.top

find . -name "*.tmp" -delete
来源：http://cnh.jianghu66.top

[R46] 递归替换文件内容
来源：http://qga.cucudq.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vsl.zhijiandao.cn

[R47] sed 单行替换
来源：http://qai.yuxming.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yec.yj202588.top

[R48] awk 取指定列
来源：http://fgy.aibaodan.cn

awk '{print $1, $3}' a.txt
来源：http://yxc.tianlin.xyz

[R49] awk 带条件
来源：http://yrz.316326.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ebm.zhengqikj.top

[R50] awk 求和
来源：http://kha.cheryme.top

awk '{s += $2} END {print s}' a.txt
来源：http://kzs.haohaochexian.top

[R51] 排序去重取前几
来源：http://rpi.fanxiaobao.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://non.pengpengdd.cyou

[R52] 统计行数
来源：http://pxr.xuetiantiany.cn

wc -l a.txt
来源：http://ime.jinqigfzy.top

[R53] 查看文件头与实时尾
来源：http://gae.pengpengdd.cyou

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sje.ydzc1.top

[R54] 比较两个文件
来源：http://tpk.cashguo.top

diff a.txt b.txt
来源：http://vij.haohaochexian.top

[R55] 压缩与解压
来源：http://thj.hnxiangtu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yer.jyoumei.cn

[R56] 远程拷贝
来源：http://vfs.tian-w.cn

scp file user@host:/path/
来源：http://eck.cucudq.cn

[R57] 远程执行命令
来源：http://rfr.bbcook.cn

ssh user@host 'uptime'
来源：http://hct.jqgfzy.top

[R58] 下载文件
来源：http://uln.gzhubu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oyh.svipenyu.cn

[R59] 发 POST JSON
来源：http://dxw.zhijiandao.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://psh.jlsjyb.cn

[R60] 只看 HTTP 状态码
来源：http://jhl.hnqzz.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uwd.xuanzx.com

[R61] 磁盘占用
来源：http://unh.c1oappe.top

df -h;  du -sh *
来源：http://mln.epnwcf.com

[R62] 找最占空间的文件
来源：http://zld.zhijiandao.cn

du -ah . | sort -rh | head -10
来源：http://vef.vehdjk.com

[R63] 内存与进程
来源：http://yda.zdqjudy.top

free -h;  ps aux | grep nginx
来源：http://dzo.ydzc1.top

[R64] 结束进程
来源：http://sqe.chenzaomai.com

kill -9 $(pgrep -f app.py)
来源：http://blb.0kj1m.cn

[R65] 查看端口占用
来源：http://pmw.xylfe.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lsy.zhiwuduotai.top

[R66] 定时任务
来源：http://lgj.haohaochexian.top

crontab -e;  crontab -l
来源：http://ohb.zhongyouzk.top

[R67] 生成随机十六进制串
来源：http://prm.wangshuangyany.cn

openssl rand -hex 16
来源：http://xuy.shuidangran.top

[R68] 计算文件校验值
来源：http://nlt.hywenlv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ixd.jianghu66.top

[R69] 生成随机密码
来源：http://yvq.hysaishi.cn

head -c 16 /dev/urandom | base64
来源：http://kob.gotoacloud.top

[R70] 时间戳与互转
来源：http://nlt.shangyingyoupin.top

date +%s;  date -d @1700000000
来源：http://ady.0kj1m.cn

[R71] 日期格式化
来源：http://rny.epnwcf.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://lma.jqgufenzy.top

[R72] 等待端口就绪
来源：http://fxx.hongshengwenyu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://kqq.fengsongda.top

[R73] 分割大日志
来源：http://yhs.aizwys.cn

split -l 1000 big.log part_
来源：http://gdv.shanyushiyangkeji.top

[R74] 批量重命名
来源：http://wjv.hysaishi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qwy.guannengcc.top

[R75] 导出环境变量
来源：http://isz.chenjidiqi.icu

export PATH="$HOME/bin:$PATH"
来源：http://cwq.shangyingyoupin.top

[R76] 使用临时文件
来源：http://jce.guannengcc.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://noo.shangyingyoupin.top

[R77] 读取用户输入
来源：http://cpu.52xcode.cn

read -rp "请输入: " ans
来源：http://apo.0kj1m.cn

[R78] 交互式菜单
来源：http://frc.yvedp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gvn.yonumen.top

[R79] 解析命令行选项
来源：http://dvd.yvedp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gch.epnwcf.com

[R80] 查看脚本执行耗时
来源：http://bsm.shanyushiyangkeji.top

time ./run.sh
来源：http://lgj.9152youxi.cn

================================================================================
来源：http://mrk.ybcxt.top

S. C / C++ 专题
来源：http://mom.c1oappe.top

================================================================================
来源：http://ato.epnwcf.com

[S01] C：Hello World
来源：http://xgm.sjlbkw.cn

#include <stdio.h>
来源：http://iyl.yj20258888.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vci.c1oappe.top

[S02] C：变量与格式化输出
来源：http://pag.xuetiantiany.cn

int a = 10; printf("%d\n", a);
来源：http://vmo.birdmap.top

[S03] C：读入整数
来源：http://ojz.gotoacloud.top

int x; scanf("%d", &x);
来源：http://cav.sufxvd.cn

[S04] C：字符串复制
来源：http://ymf.chenzaomai.com

char dst[32]; strcpy(dst, "hi");
来源：http://lzu.uphjek.com

[S05] C：字符串长度
来源：http://ags.fktsv.cn

strlen(s)
来源：http://swt.zhaomingkeji.xyz

[S06] C：字符串比较
来源：http://xym.jqgfzy.top

strcmp(a, b) == 0
来源：http://pjv.zhengqikj.top

[S07] C：数组遍历求和
来源：http://xgh.wangshuangyany.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ayf.0kj1m.cn

[S08] C：动态内存分配与释放
来源：http://jnz.zhijiandao.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kjv.guannengcc.top

[S09] C：结构体定义与初始化
来源：http://tui.hongshengwenyu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vjr.yuanzhike.top

[S10] C：指针与解引用
来源：http://lga.yanxiufei.cn

int *p = &a;  *p = 5;
来源：http://elf.iojbl.cn

[S11] C：逐行读文件
来源：http://pkx.daria6918.cn

FILE *f = fopen("a.txt", "r");
来源：http://rpv.fzhhl.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://efc.bbcook.cn

fclose(f);
来源：http://pmm.snrcjt.cn

[S12] C：写文件
来源：http://yre.yonumen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ewn.yuxming.cn

[S13] C：宏定义
来源：http://aui.yangfankeji.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hsx.gogol.net.cn

[S14] C：枚举
来源：http://ufv.uphjek.com

enum Color { RED, GREEN, BLUE };
来源：http://jig.smart0.xyz

[S15] C：类型转换
来源：http://xhn.shanyushiyangkeji.top

(double) a / b
来源：http://gpu.hnxiangtu.top

[S16] C：位操作置位
来源：http://glh.ydzc1.top

x |= (1 << 3);
来源：http://grg.dianchejie.cn

[S17] C：安全拼接字符串
来源：http://yda.ivvv.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zvd.ppjwa.cn

[S18] C：命令行参数
来源：http://ila.xziqi.cn

int main(int argc, char **argv)
来源：http://auf.aizwys.cn

[S19] C：快速排序
来源：http://klx.zhongyouzk.top

qsort(a, n, sizeof(int), cmp);
来源：http://lfe.shuidangran.top

[S20] C：二分查找
来源：http://rck.fzhhl.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mwe.pycfn.com

[S21] C：字符类别判断
来源：http://ocz.meibo888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mmw.yfazqb.com

[S22] C：字符串转数字
来源：http://uoi.pengpengdd.cyou

atoi("42");  strtod("3.14", NULL);
来源：http://rur.cheryme.top

[S23] C：随机数
来源：http://dwu.aizwys.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://inu.zhiwuduotai.top

[S24] C：获取本地时间
来源：http://zgo.yuanzhike.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jic.tianlin.xyz

[S25] C：内存拷贝
来源：http://aij.redwolf501.top

memcpy(dst, src, n);
来源：http://unv.yj202588.top

[S26] C：内存清零
来源：http://xgw.shuidangran.top

memset(a, 0, sizeof a);
来源：http://nfp.tian-w.cn

[S27] C：定义常量
来源：http://jat.shanyushiyangkeji.top

const double PI = 3.14159;
来源：http://wms.shanyushiyangkeji.top

[S28] C：静态变量
来源：http://dba.iojbl.cn

static int counter = 0;
来源：http://fwp.ydjk.org.cn

[S29] C：变参函数
来源：http://naj.fanxiaobao.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ovg.yangfankeji.com

[S30] C：头文件保护
来源：http://rrc.cashguo.top

#ifndef X_H
来源：http://xhz.dashuyun.cn

#define X_H
来源：http://hoy.redwolf501.top

#endif
来源：http://kri.ybcxt.top

[S31] C++：Hello World
来源：http://ukv.kuanghao11.cn

#include <iostream>
来源：http://mye.zhaomingkeji.xyz

int main() { std::cout << "Hello\n"; }
来源：http://hku.hongshengwenyu.top

[S32] C++：字符串
来源：http://svo.nwbrower.top

std::string s = "hi";  s += "!";
来源：http://qyr.mhx1999.top

[S33] C++：vector 增删
来源：http://crg.shuidangran.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://roy.xingfuxueyuan.xyz

[S34] C++：遍历 vector
来源：http://nmd.aibaodan.cn

for (auto &x : v) { std::cout << x; }
来源：http://rfu.cqqwz.cn

[S35] C++：map
来源：http://rbk.sxryk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rmi.nanxuanxn.top

[S36] C++：unordered_map
来源：http://dgl.xuetiantiany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kqt.iojbl.cn

[S37] C++：set
来源：http://pbx.ydzc1.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wkt.bjfxy.top

[S38] C++：排序
来源：http://gjt.zhoulong.xyz

std::sort(v.begin(), v.end());
来源：http://apm.xuanzx.com

[S39] C++：自定义比较器排序
来源：http://jqw.jianghu66.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hhl.vehdjk.com

[S40] C++：查找元素
来源：http://yyp.quarkkingdee.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ojx.yonumen.top

[S41] C++：类与构造函数
来源：http://mqp.ehwqpu.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://izg.chenlongwang.top

[S42] C++：继承与虚函数
来源：http://rbo.nanxinkj.top

class B : public Base { public: void f() override {} };
来源：http://eps.xuetiantiany.cn

[S43] C++：智能指针
来源：http://zsr.hywenlv.cn

auto p = std::make_unique<int>(5);
来源：http://ncn.ppjwa.cn

[S44] C++：引用传参
来源：http://hza.hesvh.cn

void inc(int &x) { ++x; }
来源：http://kud.feifeiyinyue.top

[S45] C++：lambda
来源：http://jpx.daria6918.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wvs.bbcook.cn

[S46] C++：函数模板
来源：http://syt.epnwcf.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gpw.fehbvm.com

[S47] C++：结构化绑定遍历
来源：http://wnc.zhengqikj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://din.fanxiaobao.xyz

[S48] C++：逐行读文件
来源：http://syj.xuetiantiany.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wrp.sjlbkw.cn

while (std::getline(in, line)) { }
来源：http://nan.0kj1m.cn

[S49] C++：写文件
来源：http://rvc.ywan-chungtsiang.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qzi.ehwqpu.com

[S50] C++：格式化数字
来源：http://tpo.xuanzx.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zbe.meibo888.top

[S51] C++：显式类型转换
来源：http://vpv.andypj.xyz

static_cast<double>(a) / b
来源：http://jiv.yuxming.cn

[S52] C++：const 与 noexcept
来源：http://lnr.shzxlz.cn

int size() const noexcept { return n_; }
来源：http://rpz.cqqwz.cn

[S53] C++：移动语义
来源：http://qlj.aibaodan.cn

std::vector<int> w = std::move(v);
来源：http://fsl.xylfe.cn

[S54] C++：异常处理
来源：http://cqk.xinyue.icu

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nlx.fzhhl.top

[S55] C++：结构化绑定
来源：http://wnq.hesvh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ugv.chenjidiqi.icu

[S56] C++：optional
来源：http://qmn.fktsv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bba.316326.xyz

[S57] C++：编译期常量
来源：http://nux.nwbrower.top

constexpr int N = 10;
来源：http://har.shzxlz.cn

[S58] C++：命名空间
来源：http://utc.hfpthk.cn

namespace ns { int f() { return 1; } }
来源：http://tle.bjfxy.top

[S59] C++：静态断言
来源：http://xow.wangdashe.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kqw.vehdjk.com

[S60] C++：遍历并删除元素
来源：http://ueo.zhijiandao.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fbh.yfazqb.com

================================================================================
来源：http://oyn.jinghuilouyu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hhe.jinqigufen.top

================================================================================
来源：http://wnv.ctjpmb.com

[T01] Kotlin：Hello World
来源：http://tgc.hammf.cn

println("Hello")
来源：http://mfq.tian-w.cn

[T02] Kotlin：变量
来源：http://bfo.ydjk.org.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://djo.daxiang520.top

[T03] Kotlin：字符串模板
来源：http://hdb.yonumen.top

"值: $b"
来源：http://aml.nanxuanxn.top

[T04] Kotlin：空安全
来源：http://igf.tianlin.xyz

val n: String? = null;  n?.length
来源：http://nof.daria6918.cn

[T05] Kotlin：when 表达式
来源：http://chp.zhaomingkeji.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dal.fehbvm.com

[T06] Kotlin：集合映射
来源：http://pmn.tarul.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://exu.aibaodan.cn

[T07] Kotlin：集合过滤
来源：http://scd.hywenlv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mmk.316326.xyz

[T08] Kotlin：数据类
来源：http://xsz.bjfxy.top

data class User(val name: String, val age: Int)
来源：http://muf.yanxiufei.cn

[T09] Kotlin：扩展函数
来源：http://lcv.yanxiufei.cn

fun String.exclaim() = this + "!"
来源：http://fwf.jianghu66.top

[T10] Kotlin：默认参数
来源：http://trk.zycfv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ghy.chenlongwang.top

[T11] Kotlin：协程
来源：http://vbz.yonumen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://nzp.snrcjt.cn

[T12] Kotlin：解构声明
来源：http://sts.jqgufenzy.top

val (a, b) = Pair(1, 2)
来源：http://paq.shangyingyoupin.top

[T13] Kotlin：只读 Map
来源：http://ujd.yvedp.cn

val m = mapOf("a" to 1)
来源：http://wcc.yanxiufei.cn

[T14] Kotlin：循环
来源：http://qfz.jinghuilouyu.cn

for (i in 1..10) println(i)
来源：http://xcm.chenzaomai.com

[T15] Kotlin：接口
来源：http://fjl.jyoumei.cn

interface Shape { fun area(): Double }
来源：http://tax.ydzc1.top

[T16] Swift：Hello World
来源：http://pgt.cheryme.top

print("Hello")
来源：http://aki.gotoacloud.top

[T17] Swift：变量与常量
来源：http://nzd.hnqzz.top

var a = 1;  let b = 2
来源：http://bbo.hcnkem.com

[T18] Swift：字符串插值
来源：http://pls.meibo888.top

"值: \(b)"
来源：http://qxj.jiagoushi.top

[T19] Swift：可选绑定
来源：http://cyv.gogol.net.cn

if let n = opt { print(n) }
来源：http://ylo.yj20258.top

[T20] Swift：数组操作
来源：http://zyc.gzhubu.top

var a = [1, 2, 3];  a.append(4)
来源：http://wug.cdnleiting.top

[T21] Swift：遍历
来源：http://wip.jianghu66.top

for x in a { print(x) }
来源：http://bad.zhongyouzk.top

[T22] Swift：字典
来源：http://wlx.9152youxi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://omc.nanxuanxn.top

[T23] Swift：函数
来源：http://awq.ydjk.org.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ybt.yj20258888.top

[T24] Swift：闭包
来源：http://olc.redwolf501.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://rxh.hammf.cn

[T25] Swift：结构体
来源：http://yhc.jinyuanbaomall.cn

struct P { var x: Int }
来源：http://qsg.tanke756.top

[T26] Swift：类与重写
来源：http://lvo.yj20258888.top

class A: Base { override func f() {} }
来源：http://uvi.sysykeji.top

[T27] Swift：错误处理
来源：http://fnm.jqgufenzy.top

do { try f() } catch { print(error) }
来源：http://mqo.fanxiaobao.xyz

[T28] Swift：枚举
来源：http://dvq.hnxiangtu.top

enum Color { case red, green }
来源：http://tzn.aibaodan.cn


<!-- 参考信息 -->