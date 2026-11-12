代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://avp.zhoulong.xyz

[R24] 大小写转换
来源：http://nrd.xuanzx.com

echo "${s^^}"; echo "${s,,}"
来源：http://kqt.yvedp.cn

[R25] 去后缀 / 去前缀
来源：http://uyp.ppjwa.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lqs.birdmap.top

[R26] 命令替换
来源：http://fgd.jinghuilouyu.cn

now=$(date +%F); echo "$now"
来源：http://rdr.zdqjudy.top

[R27] 算术展开
来源：http://lav.shangyingyoupin.top

echo $((1 + 2 * 3))
来源：http://qbh.xinyue.icu

[R28] 浮点运算
来源：http://mqb.nanxinkj.top

echo "scale=2; 10/3" | bc
来源：http://pmi.yonumen.top

[R29] 定义函数
来源：http://hbk.xuanzx.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ygv.zycfv.cn

[R30] 函数返回状态码
来源：http://sdn.jinghuilouyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://qrx.feifeiyinyue.top

[R31] 局部变量
来源：http://gah.fktsv.cn

f() { local x=1; echo "$x"; }
来源：http://zgf.nanxuanxn.top

[R32] 参数个数校验
来源：http://krd.yanxiufei.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cbt.vehdjk.com

[R33] 捕获错误并提示行号
来源：http://njf.gzhubu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fac.yongpay.top

[R34] 退出时清理
来源：http://rpp.gaohongyu789.top

trap 'rm -f "$tmp"' EXIT
来源：http://ppl.sjlbkw.cn

[R35] 后台执行并等待
来源：http://jhe.yj20258.top

sleep 5 & pid=$!; wait "$pid"
来源：http://qlp.kuanghao11.cn

[R36] 并发执行多个任务
来源：http://sds.yvedp.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lqg.jlsjyb.cn

[R37] 把输出赋给变量
来源：http://arc.hammf.cn

files=$(ls -1)
来源：http://fvo.sufxvd.cn

[R38] 管道串联
来源：http://xrv.haohaochexian.top

cat a.txt | grep -i error | wc -l
来源：http://adb.daria6918.cn

[R39] 重定向标准输出与错误
来源：http://klk.ydjk.org.cn

cmd > out.log 2>&1
来源：http://oiz.shangyingyoupin.top

[R40] 追加写日志
来源：http://wif.xuetiantiany.cn

echo "log" >> out.log
来源：http://vqb.zdbjq.cn

[R41] 丢弃输出
来源：http://eiv.hywenlv.cn

cmd >/dev/null 2>&1
来源：http://blm.yanxiufei.cn

[R42] 输入重定向
来源：http://ndp.jinyuanbaomall.cn

wc -l < a.txt
来源：http://bjg.zhijiandao.cn

[R43] 按名字查找文件
来源：http://cvg.dianchejie.cn

find . -name "*.log" -type f
来源：http://lil.pengpengdd.cyou

[R44] 按修改时间查找
来源：http://cql.jyoumei.cn

find . -mtime -7 -type f
来源：http://fge.jinyuanbaomall.cn

[R45] 批量删除
来源：http://zaz.ydjk.org.cn

find . -name "*.tmp" -delete
来源：http://fyz.gotoacloud.top

[R46] 递归替换文件内容
来源：http://kwp.tanke756.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ipx.sweek.top

[R47] sed 单行替换
来源：http://qbk.ydzc1.top

sed -i 's/foo/bar/g' a.txt
来源：http://fkm.hcnkem.com

[R48] awk 取指定列
来源：http://hyg.redwolf501.top

awk '{print $1, $3}' a.txt
来源：http://gth.yongpay.top

[R49] awk 带条件
来源：http://nso.zycfv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://evo.cqqwz.cn

[R50] awk 求和
来源：http://psd.haohaochexian.top

awk '{s += $2} END {print s}' a.txt
来源：http://ubh.fengsongda.top

[R51] 排序去重取前几
来源：http://nhf.haohaochexian.top

sort a.txt | uniq -c | sort -rn | head
来源：http://vmp.gotoacloud.top

[R52] 统计行数
来源：http://kvm.sxryk.cn

wc -l a.txt
来源：http://unv.jinqigufen.top

[R53] 查看文件头与实时尾
来源：http://bxx.fktsv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://whu.chenjidiqi.icu

[R54] 比较两个文件
来源：http://yos.shanyushiyangtech.top

diff a.txt b.txt
来源：http://lmn.snrcjt.cn

[R55] 压缩与解压
来源：http://cim.yvedp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vxe.aizwys.cn

[R56] 远程拷贝
来源：http://vcx.hammf.cn

scp file user@host:/path/
来源：http://wah.guowangkeji.top

[R57] 远程执行命令
来源：http://qlq.9152youxi.cn

ssh user@host 'uptime'
来源：http://dzs.gogol.net.cn

[R58] 下载文件
来源：http://cqp.iojbl.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ett.gogol.net.cn

[R59] 发 POST JSON
来源：http://fqk.guowangkeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wxt.jinghuilouyu.cn

[R60] 只看 HTTP 状态码
来源：http://cne.fanxiaobao.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://auc.daxiang520.top

[R61] 磁盘占用
来源：http://jou.zhengqikj.top

df -h;  du -sh *
来源：http://tea.zdbjq.cn

[R62] 找最占空间的文件
来源：http://bxf.shuidangran.top

du -ah . | sort -rh | head -10
来源：http://ktk.zhongyouzk.top

[R63] 内存与进程
来源：http://qrp.havefunace.top

free -h;  ps aux | grep nginx
来源：http://rug.zdbjq.cn

[R64] 结束进程
来源：http://zcr.snrcjt.cn

kill -9 $(pgrep -f app.py)
来源：http://oza.sjlbkw.cn

[R65] 查看端口占用
来源：http://twy.ybcxt.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zra.feifeiyinyue.top

[R66] 定时任务
来源：http://eya.dianchejie.cn

crontab -e;  crontab -l
来源：http://xpr.andypj.xyz

[R67] 生成随机十六进制串
来源：http://qxt.fzhhl.top

openssl rand -hex 16
来源：http://zav.zdbjq.cn

[R68] 计算文件校验值
来源：http://nsw.daria6918.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uuh.tarul.cn

[R69] 生成随机密码
来源：http://xme.jinqigfzy.top

head -c 16 /dev/urandom | base64
来源：http://zoa.iojbl.cn

[R70] 时间戳与互转
来源：http://gko.aizwys.cn

date +%s;  date -d @1700000000
来源：http://vba.zhengqikj.top

[R71] 日期格式化
来源：http://nwy.wangdashe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://dpe.hywenlv.cn

[R72] 等待端口就绪
来源：http://ksy.cqqwz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dex.yj202588.top

[R73] 分割大日志
来源：http://evv.zdqjudy.top

split -l 1000 big.log part_
来源：http://lcq.cucudq.cn

[R74] 批量重命名
来源：http://lwi.tarul.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://eib.gzhubu.top

[R75] 导出环境变量
来源：http://eke.cqqwz.cn

export PATH="$HOME/bin:$PATH"
来源：http://ufv.xinyue.icu

[R76] 使用临时文件
来源：http://bck.daxiang520.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://idw.hcnkem.com

[R77] 读取用户输入
来源：http://gxt.zhengqikj.top

read -rp "请输入: " ans
来源：http://hqh.cucudq.cn

[R78] 交互式菜单
来源：http://vte.zhoulong.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://mwy.sjlbkw.cn

[R79] 解析命令行选项
来源：http://eoz.hysaishi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lew.yj20258.top

[R80] 查看脚本执行耗时
来源：http://ytp.hongshengwenyu.top

time ./run.sh
来源：http://aef.fktsv.cn

================================================================================
来源：http://kev.52xcode.cn

S. C / C++ 专题
来源：http://ixm.daxiang520.top

================================================================================
来源：http://uuz.gotoacloud.top

[S01] C：Hello World
来源：http://dfu.jiagoushi.top

#include <stdio.h>
来源：http://clb.ehwqpu.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://hiw.vqdsnc.cn

[S02] C：变量与格式化输出
来源：http://rag.kuanghao11.cn

int a = 10; printf("%d\n", a);
来源：http://jxq.tian-w.cn

[S03] C：读入整数
来源：http://knl.tanke756.top

int x; scanf("%d", &x);
来源：http://wai.zycfv.cn

[S04] C：字符串复制
来源：http://wld.kuanghao11.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qjt.ydjk.org.cn

[S05] C：字符串长度
来源：http://zeb.birdmap.top

strlen(s)
来源：http://sqj.haohaochexian.top

[S06] C：字符串比较
来源：http://vbf.fehbvm.com

strcmp(a, b) == 0
来源：http://gpk.ehwqpu.com

[S07] C：数组遍历求和
来源：http://ltr.shanyushiyangkeji.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cuc.ydzc1.top

[S08] C：动态内存分配与释放
来源：http://bza.hcnkem.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fqq.hesvh.cn

[S09] C：结构体定义与初始化
来源：http://yvu.xingfuxueyuan.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://evg.fanxiaobao.xyz

[S10] C：指针与解引用
来源：http://etk.jyoumei.cn

int *p = &a;  *p = 5;
来源：http://dic.pycfn.com

[S11] C：逐行读文件
来源：http://soc.chenzaomai.com

FILE *f = fopen("a.txt", "r");
来源：http://blx.fzhhl.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://zyw.zycfv.cn

fclose(f);
来源：http://tyh.yonumen.top

[S12] C：写文件
来源：http://osz.sxryk.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://byf.ivvv.top

[S13] C：宏定义
来源：http://lhu.redwolf501.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kka.daria6918.cn

[S14] C：枚举
来源：http://tmk.0kj1m.cn

enum Color { RED, GREEN, BLUE };
来源：http://clc.yueranfly.top

[S15] C：类型转换
来源：http://huu.gzhubu.top

(double) a / b
来源：http://nkh.ybcxt.top

[S16] C：位操作置位
来源：http://ubs.zdbjq.cn

x |= (1 << 3);
来源：http://snl.snrcjt.cn

[S17] C：安全拼接字符串
来源：http://kyo.ctjpmb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qlg.sysykeji.top

[S18] C：命令行参数
来源：http://vdp.hesvh.cn

int main(int argc, char **argv)
来源：http://mnk.guowangkeji.top

[S19] C：快速排序
来源：http://zsl.zhijiandao.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jtk.cqqwz.cn

[S20] C：二分查找
来源：http://wkw.hammf.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kzb.jianghu66.top

[S21] C：字符类别判断
来源：http://gtu.sjlbkw.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ube.wangdashe.top

[S22] C：字符串转数字
来源：http://hnb.gzhubu.top

atoi("42");  strtod("3.14", NULL);
来源：http://yry.shanyushiyangkeji.top

[S23] C：随机数
来源：http://qiq.zhaomingkeji.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://mgd.yj20258888.top

[S24] C：获取本地时间
来源：http://rhw.andypj.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zgg.yonumen.top

[S25] C：内存拷贝
来源：http://neb.sweek.top

memcpy(dst, src, n);
来源：http://daq.xylfe.cn

[S26] C：内存清零
来源：http://ysj.fengsongda.top

memset(a, 0, sizeof a);
来源：http://mou.9152youxi.cn

[S27] C：定义常量
来源：http://yeb.yueranfly.top

const double PI = 3.14159;
来源：http://cby.ppjwa.cn

[S28] C：静态变量
来源：http://nnu.hammf.cn

static int counter = 0;
来源：http://jae.yfazqb.com

[S29] C：变参函数
来源：http://tvd.xuetiantiany.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://iwo.havefunace.top

[S30] C：头文件保护
来源：http://kbn.vehdjk.com

#ifndef X_H
来源：http://lql.tian-w.cn

#define X_H
来源：http://msg.gotoacloud.top

#endif
来源：http://owv.xuanzx.com

[S31] C++：Hello World
来源：http://hyv.yj202588.top

#include <iostream>
来源：http://qbe.ivvv.top

int main() { std::cout << "Hello\n"; }
来源：http://ofi.shuidangran.top

[S32] C++：字符串
来源：http://mlo.chenzaomai.com

std::string s = "hi";  s += "!";
来源：http://zbq.chenlongwang.top

[S33] C++：vector 增删
来源：http://iuq.xingfuxueyuan.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rcj.xingfuxueyuan.xyz

[S34] C++：遍历 vector
来源：http://pbz.yj20258888.top

for (auto &x : v) { std::cout << x; }
来源：http://fgs.gzhubu.top

[S35] C++：map
来源：http://fhh.aizwys.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://asx.gaohongyu789.top

[S36] C++：unordered_map
来源：http://qtt.hcnkem.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://oen.hysaishi.cn

[S37] C++：set
来源：http://syd.hongshengwenyu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sbp.xingfuxueyuan.xyz

[S38] C++：排序
来源：http://ywm.hywenlv.cn

std::sort(v.begin(), v.end());
来源：http://rzy.hnxiangtu.top

[S39] C++：自定义比较器排序
来源：http://wwo.uphjek.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yrb.c1oappe.top

[S40] C++：查找元素
来源：http://fet.gotoacloud.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zty.jlsjyb.cn

[S41] C++：类与构造函数
来源：http://hye.hysaishi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hsa.tianlin.xyz

[S42] C++：继承与虚函数
来源：http://bjh.ivvv.top

class B : public Base { public: void f() override {} };
来源：http://aay.fengsongda.top

[S43] C++：智能指针
来源：http://qeq.mhx1999.top

auto p = std::make_unique<int>(5);
来源：http://gig.kuanghao11.cn

[S44] C++：引用传参
来源：http://vup.iojbl.cn

void inc(int &x) { ++x; }
来源：http://uee.havefunace.top

[S45] C++：lambda
来源：http://ako.zhiwuduotai.top

auto add = [](int a, int b) { return a + b; };
来源：http://uvr.daria6918.cn

[S46] C++：函数模板
来源：http://zjy.gzhubu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zin.jinghuilouyu.cn

[S47] C++：结构化绑定遍历
来源：http://puv.jinyuanbaomall.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dme.shanyushiyangtech.top

[S48] C++：逐行读文件
来源：http://ibl.nwbrower.top

std::ifstream in("a.txt");  std::string line;
来源：http://ggc.zhiwuduotai.top

while (std::getline(in, line)) { }
来源：http://vlh.hammf.cn

[S49] C++：写文件
来源：http://xbg.cdnleiting.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://let.jinqigufen.top

[S50] C++：格式化数字
来源：http://rvd.xziqi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ytl.uphjek.com

[S51] C++：显式类型转换
来源：http://oez.gogol.net.cn

static_cast<double>(a) / b
来源：http://ymw.wangshuangyany.cn

[S52] C++：const 与 noexcept
来源：http://ral.yanxiufei.cn

int size() const noexcept { return n_; }
来源：http://hww.ehwqpu.com

[S53] C++：移动语义
来源：http://qdj.shanyushiyangtech.top

std::vector<int> w = std::move(v);
来源：http://ptg.jinqigufen.top

[S54] C++：异常处理
来源：http://zan.zycfv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lgp.iojbl.cn

[S55] C++：结构化绑定
来源：http://ajg.jyoumei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xyh.xinyue.icu

[S56] C++：optional
来源：http://gda.yuxming.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lse.jianghu66.top

[S57] C++：编译期常量
来源：http://trr.sysykeji.top

constexpr int N = 10;
来源：http://pdo.meibo888.top

[S58] C++：命名空间
来源：http://pxi.xuetiantiany.cn

namespace ns { int f() { return 1; } }
来源：http://yhh.yfazqb.com

[S59] C++：静态断言
来源：http://vmm.yueranfly.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yjt.bbcook.cn

[S60] C++：遍历并删除元素
来源：http://uxn.yuxming.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ktc.ppjwa.cn

================================================================================
来源：http://cor.xziqi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ukm.gaohongyu789.top

================================================================================
来源：http://kcj.gogol.net.cn

[T01] Kotlin：Hello World
来源：http://dwj.fanxiaobao.xyz

println("Hello")
来源：http://xtk.nanxuanxn.top

[T02] Kotlin：变量
来源：http://ycu.wangdashe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bcs.yonumen.top

[T03] Kotlin：字符串模板
来源：http://hyq.zycfv.cn

"值: $b"
来源：http://szt.hnxiangtu.top

[T04] Kotlin：空安全
来源：http://eoi.snrcjt.cn

val n: String? = null;  n?.length
来源：http://vjr.zhaomingkeji.xyz

[T05] Kotlin：when 表达式
来源：http://fde.vehdjk.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rxp.yonumen.top

[T06] Kotlin：集合映射
来源：http://doo.9152youxi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qzh.shangyingyoupin.top

[T07] Kotlin：集合过滤
来源：http://awc.sufxvd.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://njh.shangyingyoupin.top

[T08] Kotlin：数据类
来源：http://yep.xuetiantiany.cn

data class User(val name: String, val age: Int)
来源：http://lvg.jyoumei.cn

[T09] Kotlin：扩展函数
来源：http://nae.svipenyu.cn

fun String.exclaim() = this + "!"
来源：http://xsg.zhiwuduotai.top

[T10] Kotlin：默认参数
来源：http://fny.jinqigfzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://idf.yj20258888.top

[T11] Kotlin：协程
来源：http://zwo.birdmap.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://lzt.shanyushiyangkeji.top

[T12] Kotlin：解构声明
来源：http://euc.yj20258.top

val (a, b) = Pair(1, 2)
来源：http://zny.smart0.xyz

[T13] Kotlin：只读 Map
来源：http://ofb.jiagoushi.top

val m = mapOf("a" to 1)
来源：http://lio.zdqjudy.top

[T14] Kotlin：循环
来源：http://jtd.hnxiangtu.top

for (i in 1..10) println(i)
来源：http://ujl.xylfe.cn

[T15] Kotlin：接口
来源：http://rzk.yfazqb.com

interface Shape { fun area(): Double }
来源：http://hnz.guannengcc.top

[T16] Swift：Hello World
来源：http://cni.bjfxy.top

print("Hello")
来源：http://crg.316326.xyz

[T17] Swift：变量与常量
来源：http://job.yongpay.top

var a = 1;  let b = 2
来源：http://bxo.zhixingplan.top

[T18] Swift：字符串插值
来源：http://cik.wangdashe.top

"值: \(b)"
来源：http://pid.zhaomingkeji.xyz

[T19] Swift：可选绑定
来源：http://knn.yfazqb.com

if let n = opt { print(n) }
来源：http://lqk.hesvh.cn

[T20] Swift：数组操作
来源：http://qcd.shuidangran.top

var a = [1, 2, 3];  a.append(4)
来源：http://kza.hysaishi.cn

[T21] Swift：遍历
来源：http://hyd.zhixingplan.top

for x in a { print(x) }
来源：http://dbe.ppjwa.cn

[T22] Swift：字典
来源：http://omf.zhijiandao.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bkr.jqgufenzy.top

[T23] Swift：函数
来源：http://sxj.pycfn.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ppk.zdbjq.cn

[T24] Swift：闭包
来源：http://ikl.chenjidiqi.icu

let f = { (x: Int) -> Int in x * 2 }
来源：http://pys.jinqigfzy.top

[T25] Swift：结构体
来源：http://shi.jyoumei.cn

struct P { var x: Int }
来源：http://zrm.pycfn.com

[T26] Swift：类与重写
来源：http://lwn.yj20258.top

class A: Base { override func f() {} }
来源：http://rag.zhixingplan.top


<!-- 参考信息 -->