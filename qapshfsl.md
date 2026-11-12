代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://twc.yj202588.top

[R30] 函数返回状态码
来源：http://air.c1oappe.top

f() { return 0; }; f || echo "失败了"
来源：http://iaw.cucudq.cn

[R31] 局部变量
来源：http://wid.yuxming.cn

f() { local x=1; echo "$x"; }
来源：http://efn.9152youxi.cn

[R32] 参数个数校验
来源：http://vun.guowangkeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rdu.zhoulong.xyz

[R33] 捕获错误并提示行号
来源：http://awq.cheryme.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rgs.birdmap.top

[R34] 退出时清理
来源：http://mdu.hammf.cn

trap 'rm -f "$tmp"' EXIT
来源：http://aik.yvedp.cn

[R35] 后台执行并等待
来源：http://qtp.yuxming.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qqx.vehdjk.com

[R36] 并发执行多个任务
来源：http://guk.ppjwa.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xxl.chenjidiqi.icu

[R37] 把输出赋给变量
来源：http://vaf.sjlbkw.cn

files=$(ls -1)
来源：http://ciq.ywan-chungtsiang.top

[R38] 管道串联
来源：http://szz.zhixingplan.top

cat a.txt | grep -i error | wc -l
来源：http://lup.hongshengwenyu.top

[R39] 重定向标准输出与错误
来源：http://iqi.jyoumei.cn

cmd > out.log 2>&1
来源：http://eck.jinyuanbaomall.cn

[R40] 追加写日志
来源：http://wjh.hywenlv.cn

echo "log" >> out.log
来源：http://bjg.hysaishi.cn

[R41] 丢弃输出
来源：http://lva.zhongyouzk.top

cmd >/dev/null 2>&1
来源：http://zku.jinqigufen.top

[R42] 输入重定向
来源：http://cje.zhiwuduotai.top

wc -l < a.txt
来源：http://ydo.hfpthk.cn

[R43] 按名字查找文件
来源：http://ekf.svipenyu.cn

find . -name "*.log" -type f
来源：http://abp.zdqjudy.top

[R44] 按修改时间查找
来源：http://ssf.ydjk.org.cn

find . -mtime -7 -type f
来源：http://hyu.gaohongyu789.top

[R45] 批量删除
来源：http://xqc.vehdjk.com

find . -name "*.tmp" -delete
来源：http://nrl.pycfn.com

[R46] 递归替换文件内容
来源：http://sty.cucudq.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dzz.zhijiandao.cn

[R47] sed 单行替换
来源：http://ygu.yfazqb.com

sed -i 's/foo/bar/g' a.txt
来源：http://kym.cucudq.cn

[R48] awk 取指定列
来源：http://zzp.daria6918.cn

awk '{print $1, $3}' a.txt
来源：http://ppd.jqgfzy.top

[R49] awk 带条件
来源：http://dib.bjfxy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jfn.guannengcc.top

[R50] awk 求和
来源：http://wsv.zycfv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pff.gzhubu.top

[R51] 排序去重取前几
来源：http://rpx.nanxinkj.top

sort a.txt | uniq -c | sort -rn | head
来源：http://nhv.kuanghao11.cn

[R52] 统计行数
来源：http://koj.zhiwuduotai.top

wc -l a.txt
来源：http://jtr.guannengcc.top

[R53] 查看文件头与实时尾
来源：http://qop.zycfv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ddu.uphjek.com

[R54] 比较两个文件
来源：http://mfs.0kj1m.cn

diff a.txt b.txt
来源：http://ilh.snrcjt.cn

[R55] 压缩与解压
来源：http://obw.hfpthk.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nnb.daria6918.cn

[R56] 远程拷贝
来源：http://jlt.hongshengwenyu.top

scp file user@host:/path/
来源：http://cdv.fehbvm.com

[R57] 远程执行命令
来源：http://xhy.pycfn.com

ssh user@host 'uptime'
来源：http://ogy.jinghuilouyu.cn

[R58] 下载文件
来源：http://pky.guannengcc.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://iej.jiagoushi.top

[R59] 发 POST JSON
来源：http://gtg.epnwcf.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ker.jinqigfzy.top

[R60] 只看 HTTP 状态码
来源：http://knn.xingfuxueyuan.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://amy.hfpthk.cn

[R61] 磁盘占用
来源：http://jhh.gotoacloud.top

df -h;  du -sh *
来源：http://mmc.yj20258.top

[R62] 找最占空间的文件
来源：http://tdx.hesvh.cn

du -ah . | sort -rh | head -10
来源：http://rvx.xuanzx.com

[R63] 内存与进程
来源：http://ofj.cdnleiting.top

free -h;  ps aux | grep nginx
来源：http://ali.tarul.cn

[R64] 结束进程
来源：http://qfm.cheryme.top

kill -9 $(pgrep -f app.py)
来源：http://lqb.hysaishi.cn

[R65] 查看端口占用
来源：http://rzp.yfazqb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ocn.yfazqb.com

[R66] 定时任务
来源：http://shm.zhijiandao.cn

crontab -e;  crontab -l
来源：http://pzf.bbcook.cn

[R67] 生成随机十六进制串
来源：http://noe.zhaomingkeji.xyz

openssl rand -hex 16
来源：http://lnf.hongshengwenyu.top

[R68] 计算文件校验值
来源：http://uuc.jyoumei.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lic.xinyue.icu

[R69] 生成随机密码
来源：http://wtg.ppjwa.cn

head -c 16 /dev/urandom | base64
来源：http://keb.gogol.net.cn

[R70] 时间戳与互转
来源：http://ujx.shuidangran.top

date +%s;  date -d @1700000000
来源：http://nxq.52xcode.cn

[R71] 日期格式化
来源：http://tse.sufxvd.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lyz.52xcode.cn

[R72] 等待端口就绪
来源：http://qac.epnwcf.com

until nc -z localhost 3306; do sleep 1; done
来源：http://log.tarul.cn

[R73] 分割大日志
来源：http://tpx.wangshuangyany.cn

split -l 1000 big.log part_
来源：http://qlc.kuanghao11.cn

[R74] 批量重命名
来源：http://rcx.fengsongda.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tkq.sweek.top

[R75] 导出环境变量
来源：http://ohn.ivvv.top

export PATH="$HOME/bin:$PATH"
来源：http://lfq.316326.xyz

[R76] 使用临时文件
来源：http://rab.daxiang520.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pkg.zhijiandao.cn

[R77] 读取用户输入
来源：http://svm.hywenlv.cn

read -rp "请输入: " ans
来源：http://xqa.jinqigfzy.top

[R78] 交互式菜单
来源：http://ioi.jiagoushi.top

select opt in a b c; do echo "$opt"; break; done
来源：http://all.guannengcc.top

[R79] 解析命令行选项
来源：http://ifz.pycfn.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gpj.yj202588.top

[R80] 查看脚本执行耗时
来源：http://gwm.bjfxy.top

time ./run.sh
来源：http://jxd.zhixingplan.top

================================================================================
来源：http://qlq.ppjwa.cn

S. C / C++ 专题
来源：http://rxs.yuanzhike.top

================================================================================
来源：http://olj.gotoacloud.top

[S01] C：Hello World
来源：http://beu.zhongyouzk.top

#include <stdio.h>
来源：http://flf.9152youxi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://uex.bjfxy.top

[S02] C：变量与格式化输出
来源：http://xsq.hesvh.cn

int a = 10; printf("%d\n", a);
来源：http://cff.shzxlz.cn

[S03] C：读入整数
来源：http://zrx.zhongyouzk.top

int x; scanf("%d", &x);
来源：http://hfz.yj202588.top

[S04] C：字符串复制
来源：http://see.jinghuilouyu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://awl.jlsjyb.cn

[S05] C：字符串长度
来源：http://vpa.ctjpmb.com

strlen(s)
来源：http://jhg.gzhubu.top

[S06] C：字符串比较
来源：http://fsk.shuidangran.top

strcmp(a, b) == 0
来源：http://ygu.smart0.xyz

[S07] C：数组遍历求和
来源：http://cbi.52xcode.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sas.epnwcf.com

[S08] C：动态内存分配与释放
来源：http://smc.uphjek.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://avf.sxryk.cn

[S09] C：结构体定义与初始化
来源：http://ooe.pycfn.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bry.zhixingplan.top

[S10] C：指针与解引用
来源：http://een.xuetiantiany.cn

int *p = &a;  *p = 5;
来源：http://yos.sufxvd.cn

[S11] C：逐行读文件
来源：http://rgi.dashuyun.cn

FILE *f = fopen("a.txt", "r");
来源：http://als.jqgufenzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://kgh.c1oappe.top

fclose(f);
来源：http://qwt.xinyue.icu

[S12] C：写文件
来源：http://hco.shangyingyoupin.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pun.chenjidiqi.icu

[S13] C：宏定义
来源：http://oth.hfpthk.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mqa.wangdashe.top

[S14] C：枚举
来源：http://flb.shuidangran.top

enum Color { RED, GREEN, BLUE };
来源：http://gwx.zdqjudy.top

[S15] C：类型转换
来源：http://qbh.sweek.top

(double) a / b
来源：http://nnv.dashuyun.cn

[S16] C：位操作置位
来源：http://lez.ybcxt.top

x |= (1 << 3);
来源：http://fbe.cashguo.top

[S17] C：安全拼接字符串
来源：http://bbp.aizwys.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uml.bbcook.cn

[S18] C：命令行参数
来源：http://orq.cheryme.top

int main(int argc, char **argv)
来源：http://rxe.hcnkem.com

[S19] C：快速排序
来源：http://gte.tianlin.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://gbh.hnqzz.top

[S20] C：二分查找
来源：http://rtw.316326.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oru.kuanghao11.cn

[S21] C：字符类别判断
来源：http://ewv.nanxuanxn.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gqy.jlsjyb.cn

[S22] C：字符串转数字
来源：http://rwo.yfazqb.com

atoi("42");  strtod("3.14", NULL);
来源：http://cns.jinqigufen.top

[S23] C：随机数
来源：http://oly.pycfn.com

srand(time(NULL));  int r = rand() % 100;
来源：http://prg.andypj.xyz

[S24] C：获取本地时间
来源：http://xjm.hywenlv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tll.chenjidiqi.icu

[S25] C：内存拷贝
来源：http://aga.aizwys.cn

memcpy(dst, src, n);
来源：http://kpq.sysykeji.top

[S26] C：内存清零
来源：http://hbn.hesvh.cn

memset(a, 0, sizeof a);
来源：http://apr.ivvv.top

[S27] C：定义常量
来源：http://oci.daria6918.cn

const double PI = 3.14159;
来源：http://snk.iojbl.cn

[S28] C：静态变量
来源：http://irv.zhijiandao.cn

static int counter = 0;
来源：http://oyw.shuidangran.top

[S29] C：变参函数
来源：http://bbo.yuxming.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bkr.xuanzx.com

[S30] C：头文件保护
来源：http://mmf.sysykeji.top

#ifndef X_H
来源：http://bji.jyoumei.cn

#define X_H
来源：http://llz.jlsjyb.cn

#endif
来源：http://inw.ppjwa.cn

[S31] C++：Hello World
来源：http://tnz.shanyushiyangkeji.top

#include <iostream>
来源：http://hep.tanke756.top

int main() { std::cout << "Hello\n"; }
来源：http://feu.yongpay.top

[S32] C++：字符串
来源：http://znr.aizwys.cn

std::string s = "hi";  s += "!";
来源：http://haj.shanyushiyangkeji.top

[S33] C++：vector 增删
来源：http://bkp.zhengqikj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dky.zhongyouzk.top

[S34] C++：遍历 vector
来源：http://nxg.zhoulong.xyz

for (auto &x : v) { std::cout << x; }
来源：http://swr.jyoumei.cn

[S35] C++：map
来源：http://geh.chenzaomai.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://abe.pengpengdd.cyou

[S36] C++：unordered_map
来源：http://ehq.zycfv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iyi.epnwcf.com

[S37] C++：set
来源：http://dhv.birdmap.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zhq.mhx1999.top

[S38] C++：排序
来源：http://rbu.zycfv.cn

std::sort(v.begin(), v.end());
来源：http://ltj.yangfankeji.com

[S39] C++：自定义比较器排序
来源：http://tgf.bjfxy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pgu.tianlin.xyz

[S40] C++：查找元素
来源：http://awc.xingfuxueyuan.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dmc.316326.xyz

[S41] C++：类与构造函数
来源：http://yvp.xuetiantiany.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qqo.gogol.net.cn

[S42] C++：继承与虚函数
来源：http://dbl.zdbjq.cn

class B : public Base { public: void f() override {} };
来源：http://pie.vehdjk.com

[S43] C++：智能指针
来源：http://tht.yongpay.top

auto p = std::make_unique<int>(5);
来源：http://owp.hysaishi.cn

[S44] C++：引用传参
来源：http://bhm.yj20258.top

void inc(int &x) { ++x; }
来源：http://nuv.ctjpmb.com

[S45] C++：lambda
来源：http://ldk.chenzaomai.com

auto add = [](int a, int b) { return a + b; };
来源：http://orr.snrcjt.cn

[S46] C++：函数模板
来源：http://tyi.hysaishi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nqo.fehbvm.com

[S47] C++：结构化绑定遍历
来源：http://zpm.xziqi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ocy.daxiang520.top

[S48] C++：逐行读文件
来源：http://cgb.redwolf501.top

std::ifstream in("a.txt");  std::string line;
来源：http://iuz.fktsv.cn

while (std::getline(in, line)) { }
来源：http://lgi.sjlbkw.cn

[S49] C++：写文件
来源：http://sot.ywan-chungtsiang.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cna.pengpengdd.cyou

[S50] C++：格式化数字
来源：http://mur.yangfankeji.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dwe.smart0.xyz

[S51] C++：显式类型转换
来源：http://erj.yueranfly.top

static_cast<double>(a) / b
来源：http://joy.jinqigfzy.top

[S52] C++：const 与 noexcept
来源：http://npe.sjlbkw.cn

int size() const noexcept { return n_; }
来源：http://zof.andypj.xyz

[S53] C++：移动语义
来源：http://cij.bjfxy.top

std::vector<int> w = std::move(v);
来源：http://ljo.smart0.xyz

[S54] C++：异常处理
来源：http://oul.ybcxt.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wbv.vqdsnc.cn

[S55] C++：结构化绑定
来源：http://dac.havefunace.top

auto [a, b] = std::make_pair(1, 2);
来源：http://svu.kuanghao11.cn

[S56] C++：optional
来源：http://sqw.gaohongyu789.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ufk.jinqigufen.top

[S57] C++：编译期常量
来源：http://sqg.xziqi.cn

constexpr int N = 10;
来源：http://eeb.hcnkem.com

[S58] C++：命名空间
来源：http://zae.jinqigfzy.top

namespace ns { int f() { return 1; } }
来源：http://gyi.guowangkeji.top

[S59] C++：静态断言
来源：http://psl.hfpthk.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fgk.fengsongda.top

[S60] C++：遍历并删除元素
来源：http://itv.jyoumei.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://twn.feifeiyinyue.top

================================================================================
来源：http://jgy.0kj1m.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fqz.hysaishi.cn

================================================================================
来源：http://gls.tarul.cn

[T01] Kotlin：Hello World
来源：http://trs.xuetiantiany.cn

println("Hello")
来源：http://pob.316326.xyz

[T02] Kotlin：变量
来源：http://rcs.sysykeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rnj.shanyushiyangtech.top

[T03] Kotlin：字符串模板
来源：http://lrq.hnqzz.top

"值: $b"
来源：http://ixs.redwolf501.top

[T04] Kotlin：空安全
来源：http://kvq.cdnleiting.top

val n: String? = null;  n?.length
来源：http://gwc.iojbl.cn

[T05] Kotlin：when 表达式
来源：http://aye.nanxinkj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://duv.zdqjudy.top

[T06] Kotlin：集合映射
来源：http://rpa.c1oappe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zfh.zhijiandao.cn

[T07] Kotlin：集合过滤
来源：http://ars.smart0.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://wps.aibaodan.cn

[T08] Kotlin：数据类
来源：http://zpq.vqdsnc.cn

data class User(val name: String, val age: Int)
来源：http://btj.yuxming.cn

[T09] Kotlin：扩展函数
来源：http://byl.yj20258.top

fun String.exclaim() = this + "!"
来源：http://gpb.yangfankeji.com

[T10] Kotlin：默认参数
来源：http://wjx.tanke756.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wen.kuanghao11.cn

[T11] Kotlin：协程
来源：http://oiz.nanxinkj.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://nbd.sjlbkw.cn

[T12] Kotlin：解构声明
来源：http://lza.nwbrower.top

val (a, b) = Pair(1, 2)
来源：http://vwq.hongshengwenyu.top

[T13] Kotlin：只读 Map
来源：http://kod.tian-w.cn

val m = mapOf("a" to 1)
来源：http://ebd.hammf.cn

[T14] Kotlin：循环
来源：http://mms.wangdashe.top

for (i in 1..10) println(i)
来源：http://wpe.fehbvm.com

[T15] Kotlin：接口
来源：http://rnm.aizwys.cn

interface Shape { fun area(): Double }
来源：http://axj.bjfxy.top

[T16] Swift：Hello World
来源：http://erq.gaohongyu789.top

print("Hello")
来源：http://hfp.yj20258.top

[T17] Swift：变量与常量
来源：http://yom.xingfuxueyuan.xyz

var a = 1;  let b = 2
来源：http://oth.sysykeji.top

[T18] Swift：字符串插值
来源：http://gbz.daxiang520.top

"值: \(b)"
来源：http://lio.vehdjk.com

[T19] Swift：可选绑定
来源：http://ztu.pengpengdd.cyou

if let n = opt { print(n) }
来源：http://wfn.xingfuxueyuan.xyz

[T20] Swift：数组操作
来源：http://zva.mhx1999.top

var a = [1, 2, 3];  a.append(4)
来源：http://hci.zhengqikj.top

[T21] Swift：遍历
来源：http://rxq.dianchejie.cn

for x in a { print(x) }
来源：http://urn.zdqjudy.top

[T22] Swift：字典
来源：http://ppw.jlsjyb.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rdy.wangshuangyany.cn

[T23] Swift：函数
来源：http://eut.cdnleiting.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ofy.jiagoushi.top

[T24] Swift：闭包
来源：http://hfm.shzxlz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://unv.havefunace.top

[T25] Swift：结构体
来源：http://crb.ywan-chungtsiang.top

struct P { var x: Int }
来源：http://tya.jinqigfzy.top

[T26] Swift：类与重写
来源：http://jhm.wangshuangyany.cn

class A: Base { override func f() {} }
来源：http://khe.cdnleiting.top

[T27] Swift：错误处理
来源：http://sla.hnxiangtu.top

do { try f() } catch { print(error) }
来源：http://fcu.sufxvd.cn

[T28] Swift：枚举
来源：http://jeo.fehbvm.com

enum Color { case red, green }
来源：http://ogc.nanxuanxn.top

[T29] Swift：guard 提前返回
来源：http://xia.jianghu66.top

guard let x = opt else { return }
来源：http://bcw.yanxiufei.cn

[T30] Swift：协议
来源：http://owd.jinqigufen.top

protocol Shape { func area() -> Double }
来源：http://wcr.jinyuanbaomall.cn

[T31] Lua：Hello World
来源：http://aur.hywenlv.cn

print("Hello")
来源：http://lak.iojbl.cn

[T32] Lua：局部变量
来源：http://rkx.yongpay.top

local a = 1
来源：http://nhk.yj20258888.top


<!-- 参考信息 -->