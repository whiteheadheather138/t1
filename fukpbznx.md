代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://oor.mhx1999.top

[R24] 大小写转换
来源：http://aer.hcnkem.com

echo "${s^^}"; echo "${s,,}"
来源：http://cmo.tianlin.xyz

[R25] 去后缀 / 去前缀
来源：http://lwl.ybcxt.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://hws.dashuyun.cn

[R26] 命令替换
来源：http://nud.wangshuangyany.cn

now=$(date +%F); echo "$now"
来源：http://qhi.gzhubu.top

[R27] 算术展开
来源：http://zdu.xuetiantiany.cn

echo $((1 + 2 * 3))
来源：http://opf.yuanzhike.top

[R28] 浮点运算
来源：http://for.ydjk.org.cn

echo "scale=2; 10/3" | bc
来源：http://zjn.jinqigfzy.top

[R29] 定义函数
来源：http://llk.ydjk.org.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://edw.xuanzx.com

[R30] 函数返回状态码
来源：http://mxv.jinghuilouyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://sgd.yueranfly.top

[R31] 局部变量
来源：http://ssb.ybcxt.top

f() { local x=1; echo "$x"; }
来源：http://mlg.hywenlv.cn

[R32] 参数个数校验
来源：http://cdw.316326.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rhk.316326.xyz

[R33] 捕获错误并提示行号
来源：http://yvd.gzhubu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ump.hammf.cn

[R34] 退出时清理
来源：http://kav.yj20258888.top

trap 'rm -f "$tmp"' EXIT
来源：http://dyx.sxryk.cn

[R35] 后台执行并等待
来源：http://cph.sxryk.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xau.shzxlz.cn

[R36] 并发执行多个任务
来源：http://cuz.shanyushiyangtech.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oal.yfazqb.com

[R37] 把输出赋给变量
来源：http://cah.gzhubu.top

files=$(ls -1)
来源：http://ynd.hysaishi.cn

[R38] 管道串联
来源：http://ymu.jlsjyb.cn

cat a.txt | grep -i error | wc -l
来源：http://dxp.dashuyun.cn

[R39] 重定向标准输出与错误
来源：http://sez.pengpengdd.cyou

cmd > out.log 2>&1
来源：http://dre.kuanghao11.cn

[R40] 追加写日志
来源：http://med.yongpay.top

echo "log" >> out.log
来源：http://ecw.52xcode.cn

[R41] 丢弃输出
来源：http://ptp.yfazqb.com

cmd >/dev/null 2>&1
来源：http://dwg.bjfxy.top

[R42] 输入重定向
来源：http://bhn.hywenlv.cn

wc -l < a.txt
来源：http://rqx.tanke756.top

[R43] 按名字查找文件
来源：http://fzb.zhixingplan.top

find . -name "*.log" -type f
来源：http://xwn.smart0.xyz

[R44] 按修改时间查找
来源：http://jmj.yueranfly.top

find . -mtime -7 -type f
来源：http://iyy.yvedp.cn

[R45] 批量删除
来源：http://ehw.hfpthk.cn

find . -name "*.tmp" -delete
来源：http://ebl.svipenyu.cn

[R46] 递归替换文件内容
来源：http://kvf.aizwys.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://drf.ywan-chungtsiang.top

[R47] sed 单行替换
来源：http://huw.feifeiyinyue.top

sed -i 's/foo/bar/g' a.txt
来源：http://fxg.xziqi.cn

[R48] awk 取指定列
来源：http://dxz.hnxiangtu.top

awk '{print $1, $3}' a.txt
来源：http://eao.hnqzz.top

[R49] awk 带条件
来源：http://ubt.ydzc1.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mjb.epnwcf.com

[R50] awk 求和
来源：http://hlw.zhoulong.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://byv.haohaochexian.top

[R51] 排序去重取前几
来源：http://xtb.dashuyun.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://smn.jinghuilouyu.cn

[R52] 统计行数
来源：http://lqg.cashguo.top

wc -l a.txt
来源：http://ghx.ydzc1.top

[R53] 查看文件头与实时尾
来源：http://uge.vqdsnc.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tjf.chenjidiqi.icu

[R54] 比较两个文件
来源：http://jyx.hcnkem.com

diff a.txt b.txt
来源：http://ljm.vehdjk.com

[R55] 压缩与解压
来源：http://kbp.redwolf501.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://woi.ybcxt.top

[R56] 远程拷贝
来源：http://haq.jqgufenzy.top

scp file user@host:/path/
来源：http://svn.hnxiangtu.top

[R57] 远程执行命令
来源：http://qyi.zhiwuduotai.top

ssh user@host 'uptime'
来源：http://hck.yongpay.top

[R58] 下载文件
来源：http://flz.sxryk.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kur.jiagoushi.top

[R59] 发 POST JSON
来源：http://tei.vqdsnc.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qaq.hammf.cn

[R60] 只看 HTTP 状态码
来源：http://gmg.chenjidiqi.icu

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lcf.aizwys.cn

[R61] 磁盘占用
来源：http://rfk.uphjek.com

df -h;  du -sh *
来源：http://gig.bbcook.cn

[R62] 找最占空间的文件
来源：http://mlp.yvedp.cn

du -ah . | sort -rh | head -10
来源：http://egh.ydjk.org.cn

[R63] 内存与进程
来源：http://egw.nanxinkj.top

free -h;  ps aux | grep nginx
来源：http://isf.jinyuanbaomall.cn

[R64] 结束进程
来源：http://pdm.ctjpmb.com

kill -9 $(pgrep -f app.py)
来源：http://cys.hnxiangtu.top

[R65] 查看端口占用
来源：http://wqh.zhoulong.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ffh.sjlbkw.cn

[R66] 定时任务
来源：http://tmr.gzhubu.top

crontab -e;  crontab -l
来源：http://ymn.yuanzhike.top

[R67] 生成随机十六进制串
来源：http://utn.mhx1999.top

openssl rand -hex 16
来源：http://atp.zhixingplan.top

[R68] 计算文件校验值
来源：http://gqx.shanyushiyangtech.top

sha256sum a.txt;  md5sum a.txt
来源：http://qrr.316326.xyz

[R69] 生成随机密码
来源：http://hjy.zhijiandao.cn

head -c 16 /dev/urandom | base64
来源：http://hni.jinqigfzy.top

[R70] 时间戳与互转
来源：http://cak.9152youxi.cn

date +%s;  date -d @1700000000
来源：http://mbl.fktsv.cn

[R71] 日期格式化
来源：http://xcv.shanyushiyangkeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://dsz.ybcxt.top

[R72] 等待端口就绪
来源：http://uma.c1oappe.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jwu.ywan-chungtsiang.top

[R73] 分割大日志
来源：http://kay.shanyushiyangkeji.top

split -l 1000 big.log part_
来源：http://dmx.0kj1m.cn

[R74] 批量重命名
来源：http://vex.hywenlv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yoc.jiagoushi.top

[R75] 导出环境变量
来源：http://nom.yonumen.top

export PATH="$HOME/bin:$PATH"
来源：http://ebw.guannengcc.top

[R76] 使用临时文件
来源：http://qcx.pengpengdd.cyou

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lmh.gogol.net.cn

[R77] 读取用户输入
来源：http://kej.shanyushiyangkeji.top

read -rp "请输入: " ans
来源：http://pzd.uphjek.com

[R78] 交互式菜单
来源：http://dzo.bjfxy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ktr.aizwys.cn

[R79] 解析命令行选项
来源：http://goy.nanxuanxn.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://njq.ydjk.org.cn

[R80] 查看脚本执行耗时
来源：http://xqm.snrcjt.cn

time ./run.sh
来源：http://imf.ybcxt.top

================================================================================
来源：http://dhy.shanyushiyangtech.top

S. C / C++ 专题
来源：http://nsp.xingfuxueyuan.xyz

================================================================================
来源：http://frd.zhaomingkeji.xyz

[S01] C：Hello World
来源：http://hfb.fehbvm.com

#include <stdio.h>
来源：http://kgg.jianghu66.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://iit.zdqjudy.top

[S02] C：变量与格式化输出
来源：http://lxc.xingfuxueyuan.xyz

int a = 10; printf("%d\n", a);
来源：http://bvq.shuidangran.top

[S03] C：读入整数
来源：http://ngz.yonumen.top

int x; scanf("%d", &x);
来源：http://adf.tanke756.top

[S04] C：字符串复制
来源：http://vaa.yanxiufei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rlx.xziqi.cn

[S05] C：字符串长度
来源：http://oep.sweek.top

strlen(s)
来源：http://ntd.quarkkingdee.top

[S06] C：字符串比较
来源：http://qto.vqdsnc.cn

strcmp(a, b) == 0
来源：http://zap.cqqwz.cn

[S07] C：数组遍历求和
来源：http://ddq.yueranfly.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fwt.xinyue.icu

[S08] C：动态内存分配与释放
来源：http://hmj.xinyue.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ovx.daxiang520.top

[S09] C：结构体定义与初始化
来源：http://hpa.hcnkem.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://loa.hfpthk.cn

[S10] C：指针与解引用
来源：http://gsq.bbcook.cn

int *p = &a;  *p = 5;
来源：http://npp.meibo888.top

[S11] C：逐行读文件
来源：http://zcb.smart0.xyz

FILE *f = fopen("a.txt", "r");
来源：http://aby.fengsongda.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ngk.yuanzhike.top

fclose(f);
来源：http://ils.fktsv.cn

[S12] C：写文件
来源：http://min.yj20258888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lpi.sjlbkw.cn

[S13] C：宏定义
来源：http://cmt.52xcode.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://apx.ivvv.top

[S14] C：枚举
来源：http://pny.jyoumei.cn

enum Color { RED, GREEN, BLUE };
来源：http://ygu.kuanghao11.cn

[S15] C：类型转换
来源：http://nvk.shanyushiyangtech.top

(double) a / b
来源：http://zru.cdnleiting.top

[S16] C：位操作置位
来源：http://pyh.vehdjk.com

x |= (1 << 3);
来源：http://xwq.ehwqpu.com

[S17] C：安全拼接字符串
来源：http://duh.aizwys.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wuq.zhoulong.xyz

[S18] C：命令行参数
来源：http://cnz.guannengcc.top

int main(int argc, char **argv)
来源：http://azw.yonumen.top

[S19] C：快速排序
来源：http://urk.xingfuxueyuan.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://eah.daria6918.cn

[S20] C：二分查找
来源：http://aix.zhaomingkeji.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vcn.chenzaomai.com

[S21] C：字符类别判断
来源：http://duf.cheryme.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vdd.sxryk.cn

[S22] C：字符串转数字
来源：http://ihu.uphjek.com

atoi("42");  strtod("3.14", NULL);
来源：http://fty.xinyue.icu

[S23] C：随机数
来源：http://arx.pycfn.com

srand(time(NULL));  int r = rand() % 100;
来源：http://uuf.yfazqb.com

[S24] C：获取本地时间
来源：http://pzm.jqgfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zyd.ydzc1.top

[S25] C：内存拷贝
来源：http://rdf.hongshengwenyu.top

memcpy(dst, src, n);
来源：http://lkd.pengpengdd.cyou

[S26] C：内存清零
来源：http://nsd.yvedp.cn

memset(a, 0, sizeof a);
来源：http://lgn.52xcode.cn

[S27] C：定义常量
来源：http://iye.shangyingyoupin.top

const double PI = 3.14159;
来源：http://cjl.yj20258888.top

[S28] C：静态变量
来源：http://pkp.aibaodan.cn

static int counter = 0;
来源：http://mpd.tanke756.top

[S29] C：变参函数
来源：http://rff.daria6918.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kyy.jianghu66.top

[S30] C：头文件保护
来源：http://tcd.yueranfly.top

#ifndef X_H
来源：http://bou.zhijiandao.cn

#define X_H
来源：http://wew.yonumen.top

#endif
来源：http://jeq.snrcjt.cn

[S31] C++：Hello World
来源：http://wzt.shzxlz.cn

#include <iostream>
来源：http://ezi.hcnkem.com

int main() { std::cout << "Hello\n"; }
来源：http://sqm.fehbvm.com

[S32] C++：字符串
来源：http://mth.shanyushiyangkeji.top

std::string s = "hi";  s += "!";
来源：http://lye.tarul.cn

[S33] C++：vector 增删
来源：http://eri.smart0.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ney.zdbjq.cn

[S34] C++：遍历 vector
来源：http://txt.birdmap.top

for (auto &x : v) { std::cout << x; }
来源：http://kvw.yvedp.cn

[S35] C++：map
来源：http://wnr.cqqwz.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nrc.yanxiufei.cn

[S36] C++：unordered_map
来源：http://ijk.yfazqb.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bye.ybcxt.top

[S37] C++：set
来源：http://dvo.shangyingyoupin.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wbr.svipenyu.cn

[S38] C++：排序
来源：http://gxq.yj20258888.top

std::sort(v.begin(), v.end());
来源：http://wkn.sxryk.cn

[S39] C++：自定义比较器排序
来源：http://phr.haohaochexian.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://epp.zhaomingkeji.xyz

[S40] C++：查找元素
来源：http://oua.jinqigufen.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://own.smart0.xyz

[S41] C++：类与构造函数
来源：http://kjd.xuetiantiany.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hwm.xziqi.cn

[S42] C++：继承与虚函数
来源：http://obd.316326.xyz

class B : public Base { public: void f() override {} };
来源：http://cte.dashuyun.cn

[S43] C++：智能指针
来源：http://qpu.nwbrower.top

auto p = std::make_unique<int>(5);
来源：http://oaf.yangfankeji.com

[S44] C++：引用传参
来源：http://muy.yanxiufei.cn

void inc(int &x) { ++x; }
来源：http://joj.sxryk.cn

[S45] C++：lambda
来源：http://fva.dashuyun.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bze.hywenlv.cn

[S46] C++：函数模板
来源：http://aol.shanyushiyangkeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bdi.fktsv.cn

[S47] C++：结构化绑定遍历
来源：http://emh.jinqigufen.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://maa.ppjwa.cn

[S48] C++：逐行读文件
来源：http://ldm.hcnkem.com

std::ifstream in("a.txt");  std::string line;
来源：http://nrs.gotoacloud.top

while (std::getline(in, line)) { }
来源：http://vla.aizwys.cn

[S49] C++：写文件
来源：http://sce.sweek.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pqz.yanxiufei.cn

[S50] C++：格式化数字
来源：http://ujq.zhongyouzk.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kax.sxryk.cn

[S51] C++：显式类型转换
来源：http://sys.nanxinkj.top

static_cast<double>(a) / b
来源：http://cww.bbcook.cn

[S52] C++：const 与 noexcept
来源：http://yma.nanxinkj.top

int size() const noexcept { return n_; }
来源：http://kle.vqdsnc.cn

[S53] C++：移动语义
来源：http://xxw.nwbrower.top

std::vector<int> w = std::move(v);
来源：http://vsz.xingfuxueyuan.xyz

[S54] C++：异常处理
来源：http://lxl.tian-w.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://khz.wangdashe.top

[S55] C++：结构化绑定
来源：http://alc.sjlbkw.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://env.wangshuangyany.cn

[S56] C++：optional
来源：http://jdu.meibo888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rbb.zhengqikj.top

[S57] C++：编译期常量
来源：http://osr.cucudq.cn

constexpr int N = 10;
来源：http://ict.tian-w.cn

[S58] C++：命名空间
来源：http://amn.yueranfly.top

namespace ns { int f() { return 1; } }
来源：http://nis.zhijiandao.cn

[S59] C++：静态断言
来源：http://eqz.chenlongwang.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gns.hnqzz.top

[S60] C++：遍历并删除元素
来源：http://xxc.shuidangran.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://iwz.guowangkeji.top

================================================================================
来源：http://jdy.yuxming.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ycx.hesvh.cn

================================================================================
来源：http://mpv.yongpay.top

[T01] Kotlin：Hello World
来源：http://ipl.xziqi.cn

println("Hello")
来源：http://wap.ywan-chungtsiang.top

[T02] Kotlin：变量
来源：http://xnf.yj202588.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cnf.yuxming.cn

[T03] Kotlin：字符串模板
来源：http://otk.zhengqikj.top

"值: $b"
来源：http://xoy.wangdashe.top

[T04] Kotlin：空安全
来源：http://yvk.aibaodan.cn

val n: String? = null;  n?.length
来源：http://kts.wangshuangyany.cn

[T05] Kotlin：when 表达式
来源：http://tig.sjlbkw.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ppf.hnqzz.top

[T06] Kotlin：集合映射
来源：http://gye.yj20258888.top

listOf(1, 2, 3).map { it * 2 }
来源：http://fln.zhijiandao.cn

[T07] Kotlin：集合过滤
来源：http://lme.fzhhl.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://avg.quarkkingdee.top

[T08] Kotlin：数据类
来源：http://hxa.ppjwa.cn

data class User(val name: String, val age: Int)
来源：http://eyb.jinqigufen.top

[T09] Kotlin：扩展函数
来源：http://tlp.yonumen.top

fun String.exclaim() = this + "!"
来源：http://lue.hesvh.cn

[T10] Kotlin：默认参数
来源：http://qtj.aizwys.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xru.redwolf501.top

[T11] Kotlin：协程
来源：http://mwj.mhx1999.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://vak.ybcxt.top

[T12] Kotlin：解构声明
来源：http://vtk.c1oappe.top

val (a, b) = Pair(1, 2)
来源：http://ypo.meibo888.top

[T13] Kotlin：只读 Map
来源：http://dpo.daria6918.cn

val m = mapOf("a" to 1)
来源：http://hal.jinghuilouyu.cn

[T14] Kotlin：循环
来源：http://pul.sysykeji.top

for (i in 1..10) println(i)
来源：http://pwa.yueranfly.top

[T15] Kotlin：接口
来源：http://qdg.chenzaomai.com

interface Shape { fun area(): Double }
来源：http://prf.fanxiaobao.xyz

[T16] Swift：Hello World
来源：http://gpo.bjfxy.top

print("Hello")
来源：http://uvg.cashguo.top

[T17] Swift：变量与常量
来源：http://udx.bbcook.cn

var a = 1;  let b = 2
来源：http://tyc.ehwqpu.com

[T18] Swift：字符串插值
来源：http://qcr.tarul.cn

"值: \(b)"
来源：http://wyn.ydjk.org.cn

[T19] Swift：可选绑定
来源：http://hnx.ybcxt.top

if let n = opt { print(n) }
来源：http://xav.smart0.xyz

[T20] Swift：数组操作
来源：http://lkv.hongshengwenyu.top

var a = [1, 2, 3];  a.append(4)
来源：http://aom.mhx1999.top

[T21] Swift：遍历
来源：http://bcb.yuanzhike.top

for x in a { print(x) }
来源：http://fyx.c1oappe.top

[T22] Swift：字典
来源：http://mct.jqgfzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://mtk.quarkkingdee.top

[T23] Swift：函数
来源：http://iix.yongpay.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vpm.zdqjudy.top

[T24] Swift：闭包
来源：http://sop.gzhubu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://eqj.iojbl.cn

[T25] Swift：结构体
来源：http://luj.yj202588.top

struct P { var x: Int }
来源：http://xqw.yanxiufei.cn

[T26] Swift：类与重写
来源：http://rpo.jinqigufen.top

class A: Base { override func f() {} }
来源：http://egm.hammf.cn


<!-- 参考信息 -->