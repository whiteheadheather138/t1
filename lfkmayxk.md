代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://lrq.hcnkem.com

[R26] 命令替换
来源：http://rqu.ydzc1.top

now=$(date +%F); echo "$now"
来源：http://ury.jianghu66.top

[R27] 算术展开
来源：http://zml.zhiwuduotai.top

echo $((1 + 2 * 3))
来源：http://kcf.xuanzx.com

[R28] 浮点运算
来源：http://prv.jiagoushi.top

echo "scale=2; 10/3" | bc
来源：http://vvp.dianchejie.cn

[R29] 定义函数
来源：http://ybr.zdbjq.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://toe.ywan-chungtsiang.top

[R30] 函数返回状态码
来源：http://xzk.zycfv.cn

f() { return 0; }; f || echo "失败了"
来源：http://kgj.iojbl.cn

[R31] 局部变量
来源：http://ffu.hysaishi.cn

f() { local x=1; echo "$x"; }
来源：http://bcr.ybcxt.top

[R32] 参数个数校验
来源：http://qha.shzxlz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uit.cdnleiting.top

[R33] 捕获错误并提示行号
来源：http://tkr.ydjk.org.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mec.hnxiangtu.top

[R34] 退出时清理
来源：http://qcv.kuanghao11.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ugg.316326.xyz

[R35] 后台执行并等待
来源：http://unh.ppjwa.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gjr.xziqi.cn

[R36] 并发执行多个任务
来源：http://huc.aizwys.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qog.yuxming.cn

[R37] 把输出赋给变量
来源：http://agh.hfpthk.cn

files=$(ls -1)
来源：http://axn.c1oappe.top

[R38] 管道串联
来源：http://upf.jyoumei.cn

cat a.txt | grep -i error | wc -l
来源：http://vqz.tianlin.xyz

[R39] 重定向标准输出与错误
来源：http://nvf.hongshengwenyu.top

cmd > out.log 2>&1
来源：http://abg.sufxvd.cn

[R40] 追加写日志
来源：http://bwh.cqqwz.cn

echo "log" >> out.log
来源：http://tus.hysaishi.cn

[R41] 丢弃输出
来源：http://ofm.xziqi.cn

cmd >/dev/null 2>&1
来源：http://rxk.hfpthk.cn

[R42] 输入重定向
来源：http://twt.jiagoushi.top

wc -l < a.txt
来源：http://wbl.gaohongyu789.top

[R43] 按名字查找文件
来源：http://nxn.chenzaomai.com

find . -name "*.log" -type f
来源：http://psy.yanxiufei.cn

[R44] 按修改时间查找
来源：http://arb.hysaishi.cn

find . -mtime -7 -type f
来源：http://ouw.316326.xyz

[R45] 批量删除
来源：http://swt.svipenyu.cn

find . -name "*.tmp" -delete
来源：http://pzs.ydjk.org.cn

[R46] 递归替换文件内容
来源：http://ksg.meibo888.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wye.tarul.cn

[R47] sed 单行替换
来源：http://fow.haohaochexian.top

sed -i 's/foo/bar/g' a.txt
来源：http://deu.zhiwuduotai.top

[R48] awk 取指定列
来源：http://vye.jinqigfzy.top

awk '{print $1, $3}' a.txt
来源：http://skt.xylfe.cn

[R49] awk 带条件
来源：http://tma.jlsjyb.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://amq.bbcook.cn

[R50] awk 求和
来源：http://box.aizwys.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lks.chenjidiqi.icu

[R51] 排序去重取前几
来源：http://cxs.ivvv.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ohs.yangfankeji.com

[R52] 统计行数
来源：http://dad.jianghu66.top

wc -l a.txt
来源：http://ssp.ydzc1.top

[R53] 查看文件头与实时尾
来源：http://wfc.feifeiyinyue.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dqt.cqqwz.cn

[R54] 比较两个文件
来源：http://kpp.feifeiyinyue.top

diff a.txt b.txt
来源：http://qxe.hcnkem.com

[R55] 压缩与解压
来源：http://bnr.dashuyun.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://waw.kuanghao11.cn

[R56] 远程拷贝
来源：http://qfi.birdmap.top

scp file user@host:/path/
来源：http://feh.hesvh.cn

[R57] 远程执行命令
来源：http://zkl.tanke756.top

ssh user@host 'uptime'
来源：http://tmm.yvedp.cn

[R58] 下载文件
来源：http://znp.hysaishi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hgk.9152youxi.cn

[R59] 发 POST JSON
来源：http://hmd.iojbl.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mhz.yueranfly.top

[R60] 只看 HTTP 状态码
来源：http://iuo.hongshengwenyu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ovg.sysykeji.top

[R61] 磁盘占用
来源：http://seq.shangyingyoupin.top

df -h;  du -sh *
来源：http://gkm.cheryme.top

[R62] 找最占空间的文件
来源：http://aod.bbcook.cn

du -ah . | sort -rh | head -10
来源：http://pxa.yj20258.top

[R63] 内存与进程
来源：http://lso.xylfe.cn

free -h;  ps aux | grep nginx
来源：http://xzh.zhixingplan.top

[R64] 结束进程
来源：http://job.fengsongda.top

kill -9 $(pgrep -f app.py)
来源：http://hhk.zhoulong.xyz

[R65] 查看端口占用
来源：http://mfd.zhongyouzk.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jba.zhijiandao.cn

[R66] 定时任务
来源：http://fny.hongshengwenyu.top

crontab -e;  crontab -l
来源：http://vee.shuidangran.top

[R67] 生成随机十六进制串
来源：http://ida.fanxiaobao.xyz

openssl rand -hex 16
来源：http://sgn.chenzaomai.com

[R68] 计算文件校验值
来源：http://jnd.sysykeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://kqx.zycfv.cn

[R69] 生成随机密码
来源：http://ccc.dianchejie.cn

head -c 16 /dev/urandom | base64
来源：http://ucx.daxiang520.top

[R70] 时间戳与互转
来源：http://zwe.yfazqb.com

date +%s;  date -d @1700000000
来源：http://rrm.gaohongyu789.top

[R71] 日期格式化
来源：http://zen.hfpthk.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rpw.jlsjyb.cn

[R72] 等待端口就绪
来源：http://ryg.hesvh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://oux.hywenlv.cn

[R73] 分割大日志
来源：http://zmf.hongshengwenyu.top

split -l 1000 big.log part_
来源：http://ugx.tanke756.top

[R74] 批量重命名
来源：http://fyz.ppjwa.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://koa.ydzc1.top

[R75] 导出环境变量
来源：http://hzz.hnxiangtu.top

export PATH="$HOME/bin:$PATH"
来源：http://wqp.hfpthk.cn

[R76] 使用临时文件
来源：http://gpg.fengsongda.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jpr.sysykeji.top

[R77] 读取用户输入
来源：http://cay.shangyingyoupin.top

read -rp "请输入: " ans
来源：http://njy.hongshengwenyu.top

[R78] 交互式菜单
来源：http://fvz.zhengqikj.top

select opt in a b c; do echo "$opt"; break; done
来源：http://unk.ywan-chungtsiang.top

[R79] 解析命令行选项
来源：http://umu.vehdjk.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bpb.zhaomingkeji.xyz

[R80] 查看脚本执行耗时
来源：http://hki.zdbjq.cn

time ./run.sh
来源：http://fyc.redwolf501.top

================================================================================
来源：http://ehb.52xcode.cn

S. C / C++ 专题
来源：http://epj.hnqzz.top

================================================================================
来源：http://jec.dashuyun.cn

[S01] C：Hello World
来源：http://dlh.guannengcc.top

#include <stdio.h>
来源：http://dtx.vehdjk.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://yhh.fengsongda.top

[S02] C：变量与格式化输出
来源：http://luv.sweek.top

int a = 10; printf("%d\n", a);
来源：http://cik.nanxuanxn.top

[S03] C：读入整数
来源：http://zzs.yongpay.top

int x; scanf("%d", &x);
来源：http://wqz.jyoumei.cn

[S04] C：字符串复制
来源：http://pqh.zycfv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dcb.redwolf501.top

[S05] C：字符串长度
来源：http://eqr.quarkkingdee.top

strlen(s)
来源：http://yzt.zhaomingkeji.xyz

[S06] C：字符串比较
来源：http://uuf.epnwcf.com

strcmp(a, b) == 0
来源：http://chn.daxiang520.top

[S07] C：数组遍历求和
来源：http://kcr.jinqigfzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dsy.gaohongyu789.top

[S08] C：动态内存分配与释放
来源：http://mtc.snrcjt.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jvj.xingfuxueyuan.xyz

[S09] C：结构体定义与初始化
来源：http://upn.yonumen.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ktu.shangyingyoupin.top

[S10] C：指针与解引用
来源：http://nas.fehbvm.com

int *p = &a;  *p = 5;
来源：http://ngu.svipenyu.cn

[S11] C：逐行读文件
来源：http://faj.havefunace.top

FILE *f = fopen("a.txt", "r");
来源：http://tqw.0kj1m.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://uun.ivvv.top

fclose(f);
来源：http://gqv.feifeiyinyue.top

[S12] C：写文件
来源：http://pvb.tanke756.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://spw.vehdjk.com

[S13] C：宏定义
来源：http://riw.snrcjt.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tnt.hnqzz.top

[S14] C：枚举
来源：http://hge.ywan-chungtsiang.top

enum Color { RED, GREEN, BLUE };
来源：http://cyn.aizwys.cn

[S15] C：类型转换
来源：http://jvd.xuetiantiany.cn

(double) a / b
来源：http://zam.birdmap.top

[S16] C：位操作置位
来源：http://nrq.kuanghao11.cn

x |= (1 << 3);
来源：http://sqe.tanke756.top

[S17] C：安全拼接字符串
来源：http://qou.zycfv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qqk.hesvh.cn

[S18] C：命令行参数
来源：http://nli.cashguo.top

int main(int argc, char **argv)
来源：http://ouf.ywan-chungtsiang.top

[S19] C：快速排序
来源：http://fgk.shangyingyoupin.top

qsort(a, n, sizeof(int), cmp);
来源：http://yov.gogol.net.cn

[S20] C：二分查找
来源：http://zli.sysykeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ltk.chenjidiqi.icu

[S21] C：字符类别判断
来源：http://ngf.wangshuangyany.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ubq.yongpay.top

[S22] C：字符串转数字
来源：http://ehu.yuxming.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wzs.ivvv.top

[S23] C：随机数
来源：http://idw.hesvh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rrh.feifeiyinyue.top

[S24] C：获取本地时间
来源：http://uiq.ydzc1.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://srl.zdqjudy.top

[S25] C：内存拷贝
来源：http://vng.xuanzx.com

memcpy(dst, src, n);
来源：http://jhh.zdqjudy.top

[S26] C：内存清零
来源：http://atu.andypj.xyz

memset(a, 0, sizeof a);
来源：http://ftl.hfpthk.cn

[S27] C：定义常量
来源：http://pvx.zycfv.cn

const double PI = 3.14159;
来源：http://itm.tanke756.top

[S28] C：静态变量
来源：http://kxo.yongpay.top

static int counter = 0;
来源：http://bij.hnxiangtu.top

[S29] C：变参函数
来源：http://bna.yuxming.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vzi.shzxlz.cn

[S30] C：头文件保护
来源：http://kab.shzxlz.cn

#ifndef X_H
来源：http://reb.zdbjq.cn

#define X_H
来源：http://ues.shangyingyoupin.top

#endif
来源：http://kew.guannengcc.top

[S31] C++：Hello World
来源：http://rhu.yuanzhike.top

#include <iostream>
来源：http://ziu.fengsongda.top

int main() { std::cout << "Hello\n"; }
来源：http://apz.cheryme.top

[S32] C++：字符串
来源：http://lsr.yanxiufei.cn

std::string s = "hi";  s += "!";
来源：http://tme.gzhubu.top

[S33] C++：vector 增删
来源：http://mqi.zhoulong.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ene.jiagoushi.top

[S34] C++：遍历 vector
来源：http://rlk.havefunace.top

for (auto &x : v) { std::cout << x; }
来源：http://neq.uphjek.com

[S35] C++：map
来源：http://zdo.hysaishi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oag.chenjidiqi.icu

[S36] C++：unordered_map
来源：http://ogs.nwbrower.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ujg.xziqi.cn

[S37] C++：set
来源：http://blx.zhoulong.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://apj.yangfankeji.com

[S38] C++：排序
来源：http://tpo.zhiwuduotai.top

std::sort(v.begin(), v.end());
来源：http://evw.fengsongda.top

[S39] C++：自定义比较器排序
来源：http://enw.guannengcc.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qdu.daxiang520.top

[S40] C++：查找元素
来源：http://qpy.316326.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://atp.sufxvd.cn

[S41] C++：类与构造函数
来源：http://itz.zhongyouzk.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cxf.bjfxy.top

[S42] C++：继承与虚函数
来源：http://rmr.jqgufenzy.top

class B : public Base { public: void f() override {} };
来源：http://skg.haohaochexian.top

[S43] C++：智能指针
来源：http://nly.hesvh.cn

auto p = std::make_unique<int>(5);
来源：http://ffy.jlsjyb.cn

[S44] C++：引用传参
来源：http://xqv.316326.xyz

void inc(int &x) { ++x; }
来源：http://xpf.fanxiaobao.xyz

[S45] C++：lambda
来源：http://ojl.birdmap.top

auto add = [](int a, int b) { return a + b; };
来源：http://jje.chenjidiqi.icu

[S46] C++：函数模板
来源：http://eqb.52xcode.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nqm.cashguo.top

[S47] C++：结构化绑定遍历
来源：http://rht.pycfn.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xvk.cqqwz.cn

[S48] C++：逐行读文件
来源：http://isp.yanxiufei.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zky.sxryk.cn

while (std::getline(in, line)) { }
来源：http://wdf.zhengqikj.top

[S49] C++：写文件
来源：http://vku.kuanghao11.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pwu.hcnkem.com

[S50] C++：格式化数字
来源：http://cpk.shanyushiyangtech.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xxi.9152youxi.cn

[S51] C++：显式类型转换
来源：http://nos.tanke756.top

static_cast<double>(a) / b
来源：http://kbh.smart0.xyz

[S52] C++：const 与 noexcept
来源：http://zia.fengsongda.top

int size() const noexcept { return n_; }
来源：http://ytw.hongshengwenyu.top

[S53] C++：移动语义
来源：http://hlf.pycfn.com

std::vector<int> w = std::move(v);
来源：http://bvz.sjlbkw.cn

[S54] C++：异常处理
来源：http://oxw.svipenyu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tgb.shuidangran.top

[S55] C++：结构化绑定
来源：http://gdk.smart0.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://dkp.sufxvd.cn

[S56] C++：optional
来源：http://yfb.hnqzz.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://orr.aizwys.cn

[S57] C++：编译期常量
来源：http://mub.9152youxi.cn

constexpr int N = 10;
来源：http://cxo.jiagoushi.top

[S58] C++：命名空间
来源：http://bml.yonumen.top

namespace ns { int f() { return 1; } }
来源：http://ksx.aizwys.cn

[S59] C++：静态断言
来源：http://gpf.snrcjt.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mbv.gaohongyu789.top

[S60] C++：遍历并删除元素
来源：http://yhl.vehdjk.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://itn.0kj1m.cn

================================================================================
来源：http://vkn.tian-w.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vrc.daria6918.cn

================================================================================
来源：http://kqu.smart0.xyz

[T01] Kotlin：Hello World
来源：http://sir.jinqigfzy.top

println("Hello")
来源：http://vcj.hnxiangtu.top

[T02] Kotlin：变量
来源：http://yli.9152youxi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ijv.ydjk.org.cn

[T03] Kotlin：字符串模板
来源：http://jao.feifeiyinyue.top

"值: $b"
来源：http://yjj.fzhhl.top

[T04] Kotlin：空安全
来源：http://ier.xylfe.cn

val n: String? = null;  n?.length
来源：http://mrv.nwbrower.top

[T05] Kotlin：when 表达式
来源：http://nwd.jqgufenzy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xam.andypj.xyz

[T06] Kotlin：集合映射
来源：http://axw.daxiang520.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ydz.yfazqb.com

[T07] Kotlin：集合过滤
来源：http://osl.9152youxi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://psg.yuanzhike.top

[T08] Kotlin：数据类
来源：http://fdt.shanyushiyangtech.top

data class User(val name: String, val age: Int)
来源：http://oop.ywan-chungtsiang.top

[T09] Kotlin：扩展函数
来源：http://fub.aibaodan.cn

fun String.exclaim() = this + "!"
来源：http://peo.feifeiyinyue.top

[T10] Kotlin：默认参数
来源：http://uuu.zdqjudy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://rrh.hammf.cn

[T11] Kotlin：协程
来源：http://mkz.gaohongyu789.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://zaz.guannengcc.top

[T12] Kotlin：解构声明
来源：http://asc.nwbrower.top

val (a, b) = Pair(1, 2)
来源：http://xpg.xylfe.cn

[T13] Kotlin：只读 Map
来源：http://inq.wangdashe.top

val m = mapOf("a" to 1)
来源：http://iyp.c1oappe.top

[T14] Kotlin：循环
来源：http://pcv.52xcode.cn

for (i in 1..10) println(i)
来源：http://zeh.guowangkeji.top

[T15] Kotlin：接口
来源：http://anu.hnqzz.top

interface Shape { fun area(): Double }
来源：http://tpm.ywan-chungtsiang.top

[T16] Swift：Hello World
来源：http://vgw.mhx1999.top

print("Hello")
来源：http://rjc.fktsv.cn

[T17] Swift：变量与常量
来源：http://zbr.jinqigufen.top

var a = 1;  let b = 2
来源：http://ygj.fehbvm.com

[T18] Swift：字符串插值
来源：http://uoi.52xcode.cn

"值: \(b)"
来源：http://zqq.zdbjq.cn

[T19] Swift：可选绑定
来源：http://msg.hammf.cn

if let n = opt { print(n) }
来源：http://ima.tarul.cn

[T20] Swift：数组操作
来源：http://ili.xuetiantiany.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gnn.jinqigufen.top

[T21] Swift：遍历
来源：http://oih.smart0.xyz

for x in a { print(x) }
来源：http://zac.xuetiantiany.cn

[T22] Swift：字典
来源：http://rwn.smart0.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://xic.jlsjyb.cn

[T23] Swift：函数
来源：http://dxh.redwolf501.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://oxo.epnwcf.com

[T24] Swift：闭包
来源：http://bgi.jqgfzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://jaz.hfpthk.cn

[T25] Swift：结构体
来源：http://oij.hcnkem.com

struct P { var x: Int }
来源：http://ofz.xuetiantiany.cn

[T26] Swift：类与重写
来源：http://uwy.jqgfzy.top

class A: Base { override func f() {} }
来源：http://smz.chenlongwang.top

[T27] Swift：错误处理
来源：http://pcf.yuanzhike.top

do { try f() } catch { print(error) }
来源：http://oml.gogol.net.cn

[T28] Swift：枚举
来源：http://zuz.cashguo.top

enum Color { case red, green }
来源：http://nww.xuanzx.com


<!-- 参考信息 -->