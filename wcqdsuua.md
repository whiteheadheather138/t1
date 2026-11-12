代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://egh.ctjpmb.com

[R30] 函数返回状态码
来源：http://fwy.hysaishi.cn

f() { return 0; }; f || echo "失败了"
来源：http://lol.zhiwuduotai.top

[R31] 局部变量
来源：http://jqp.snrcjt.cn

f() { local x=1; echo "$x"; }
来源：http://fno.9152youxi.cn

[R32] 参数个数校验
来源：http://uyn.yueranfly.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dne.wangshuangyany.cn

[R33] 捕获错误并提示行号
来源：http://dll.fehbvm.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ukf.ydjk.org.cn

[R34] 退出时清理
来源：http://knp.jinqigfzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://uux.feifeiyinyue.top

[R35] 后台执行并等待
来源：http://zyv.xinyue.icu

sleep 5 & pid=$!; wait "$pid"
来源：http://jfe.yvedp.cn

[R36] 并发执行多个任务
来源：http://dtv.guowangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yzq.ctjpmb.com

[R37] 把输出赋给变量
来源：http://kua.guowangkeji.top

files=$(ls -1)
来源：http://unl.aizwys.cn

[R38] 管道串联
来源：http://tfb.zhaomingkeji.xyz

cat a.txt | grep -i error | wc -l
来源：http://bzx.daxiang520.top

[R39] 重定向标准输出与错误
来源：http://emr.vqdsnc.cn

cmd > out.log 2>&1
来源：http://adj.shanyushiyangtech.top

[R40] 追加写日志
来源：http://xrl.nanxinkj.top

echo "log" >> out.log
来源：http://yzk.havefunace.top

[R41] 丢弃输出
来源：http://rxm.chenzaomai.com

cmd >/dev/null 2>&1
来源：http://mqi.ivvv.top

[R42] 输入重定向
来源：http://xyk.jinqigfzy.top

wc -l < a.txt
来源：http://nja.feifeiyinyue.top

[R43] 按名字查找文件
来源：http://xwd.ydjk.org.cn

find . -name "*.log" -type f
来源：http://zfr.epnwcf.com

[R44] 按修改时间查找
来源：http://pjj.hnqzz.top

find . -mtime -7 -type f
来源：http://lnw.fktsv.cn

[R45] 批量删除
来源：http://qen.yanxiufei.cn

find . -name "*.tmp" -delete
来源：http://jey.ppjwa.cn

[R46] 递归替换文件内容
来源：http://duj.hammf.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nrx.9152youxi.cn

[R47] sed 单行替换
来源：http://mkg.xinyue.icu

sed -i 's/foo/bar/g' a.txt
来源：http://dna.gotoacloud.top

[R48] awk 取指定列
来源：http://jjc.yfazqb.com

awk '{print $1, $3}' a.txt
来源：http://lou.ydjk.org.cn

[R49] awk 带条件
来源：http://buz.aibaodan.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zac.ydzc1.top

[R50] awk 求和
来源：http://ggm.tanke756.top

awk '{s += $2} END {print s}' a.txt
来源：http://crn.zhiwuduotai.top

[R51] 排序去重取前几
来源：http://ppv.yj20258888.top

sort a.txt | uniq -c | sort -rn | head
来源：http://qzt.jinyuanbaomall.cn

[R52] 统计行数
来源：http://pol.kuanghao11.cn

wc -l a.txt
来源：http://xyf.jqgfzy.top

[R53] 查看文件头与实时尾
来源：http://ksq.zhijiandao.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xsk.nwbrower.top

[R54] 比较两个文件
来源：http://czv.gzhubu.top

diff a.txt b.txt
来源：http://kbh.pycfn.com

[R55] 压缩与解压
来源：http://ssy.shanyushiyangtech.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rvi.quarkkingdee.top

[R56] 远程拷贝
来源：http://ehj.xuanzx.com

scp file user@host:/path/
来源：http://tjc.meibo888.top

[R57] 远程执行命令
来源：http://sft.hcnkem.com

ssh user@host 'uptime'
来源：http://wbl.fengsongda.top

[R58] 下载文件
来源：http://ipd.jyoumei.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ugr.jinghuilouyu.cn

[R59] 发 POST JSON
来源：http://cca.jinqigfzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sgu.zdbjq.cn

[R60] 只看 HTTP 状态码
来源：http://tiz.yj20258888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cfi.52xcode.cn

[R61] 磁盘占用
来源：http://xsp.ppjwa.cn

df -h;  du -sh *
来源：http://bpf.zdqjudy.top

[R62] 找最占空间的文件
来源：http://nuk.hnxiangtu.top

du -ah . | sort -rh | head -10
来源：http://vcx.xylfe.cn

[R63] 内存与进程
来源：http://kdy.jianghu66.top

free -h;  ps aux | grep nginx
来源：http://rcq.jinyuanbaomall.cn

[R64] 结束进程
来源：http://qhz.hfpthk.cn

kill -9 $(pgrep -f app.py)
来源：http://diy.guowangkeji.top

[R65] 查看端口占用
来源：http://nlt.smart0.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://btm.meibo888.top

[R66] 定时任务
来源：http://zxo.yvedp.cn

crontab -e;  crontab -l
来源：http://hlq.shangyingyoupin.top

[R67] 生成随机十六进制串
来源：http://rbu.sjlbkw.cn

openssl rand -hex 16
来源：http://vaf.gzhubu.top

[R68] 计算文件校验值
来源：http://dqp.yuxming.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kjl.sjlbkw.cn

[R69] 生成随机密码
来源：http://qly.yonumen.top

head -c 16 /dev/urandom | base64
来源：http://twe.dashuyun.cn

[R70] 时间戳与互转
来源：http://dws.chenjidiqi.icu

date +%s;  date -d @1700000000
来源：http://ist.wangdashe.top

[R71] 日期格式化
来源：http://pal.hnxiangtu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://wwr.zhijiandao.cn

[R72] 等待端口就绪
来源：http://zji.jqgfzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://adx.tarul.cn

[R73] 分割大日志
来源：http://llc.guannengcc.top

split -l 1000 big.log part_
来源：http://byt.gaohongyu789.top

[R74] 批量重命名
来源：http://vxh.birdmap.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vlz.sysykeji.top

[R75] 导出环境变量
来源：http://vxq.zhongyouzk.top

export PATH="$HOME/bin:$PATH"
来源：http://kkh.jlsjyb.cn

[R76] 使用临时文件
来源：http://tjy.jinqigfzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qxp.birdmap.top

[R77] 读取用户输入
来源：http://mco.feifeiyinyue.top

read -rp "请输入: " ans
来源：http://kqg.xylfe.cn

[R78] 交互式菜单
来源：http://drs.redwolf501.top

select opt in a b c; do echo "$opt"; break; done
来源：http://gmh.ywan-chungtsiang.top

[R79] 解析命令行选项
来源：http://idy.gaohongyu789.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xyp.fengsongda.top

[R80] 查看脚本执行耗时
来源：http://xzt.aibaodan.cn

time ./run.sh
来源：http://fvo.xuanzx.com

================================================================================
来源：http://zqe.tanke756.top

S. C / C++ 专题
来源：http://vaj.hysaishi.cn

================================================================================
来源：http://dws.tian-w.cn

[S01] C：Hello World
来源：http://fjv.yongpay.top

#include <stdio.h>
来源：http://est.jinqigfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xlb.yuxming.cn

[S02] C：变量与格式化输出
来源：http://wye.yangfankeji.com

int a = 10; printf("%d\n", a);
来源：http://fwt.aizwys.cn

[S03] C：读入整数
来源：http://xey.sufxvd.cn

int x; scanf("%d", &x);
来源：http://lwg.ybcxt.top

[S04] C：字符串复制
来源：http://awy.guowangkeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://hbn.guowangkeji.top

[S05] C：字符串长度
来源：http://gto.yfazqb.com

strlen(s)
来源：http://shp.pycfn.com

[S06] C：字符串比较
来源：http://wdw.fengsongda.top

strcmp(a, b) == 0
来源：http://bsf.zhijiandao.cn

[S07] C：数组遍历求和
来源：http://dxr.hnxiangtu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jea.zhoulong.xyz

[S08] C：动态内存分配与释放
来源：http://kob.yangfankeji.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://riq.havefunace.top

[S09] C：结构体定义与初始化
来源：http://fms.nanxinkj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wlb.guannengcc.top

[S10] C：指针与解引用
来源：http://pcx.fehbvm.com

int *p = &a;  *p = 5;
来源：http://jho.tianlin.xyz

[S11] C：逐行读文件
来源：http://ljw.gotoacloud.top

FILE *f = fopen("a.txt", "r");
来源：http://ydw.tanke756.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ggd.hammf.cn

fclose(f);
来源：http://shj.zhixingplan.top

[S12] C：写文件
来源：http://rss.jqgufenzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hfw.gogol.net.cn

[S13] C：宏定义
来源：http://aff.nanxinkj.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pny.shzxlz.cn

[S14] C：枚举
来源：http://jwr.aibaodan.cn

enum Color { RED, GREEN, BLUE };
来源：http://wve.sweek.top

[S15] C：类型转换
来源：http://opz.sxryk.cn

(double) a / b
来源：http://tkw.jqgfzy.top

[S16] C：位操作置位
来源：http://bgu.yuanzhike.top

x |= (1 << 3);
来源：http://ubi.hywenlv.cn

[S17] C：安全拼接字符串
来源：http://clw.guannengcc.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zvv.sysykeji.top

[S18] C：命令行参数
来源：http://tqq.birdmap.top

int main(int argc, char **argv)
来源：http://zrp.zhixingplan.top

[S19] C：快速排序
来源：http://ssk.jqgfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://tyu.zhiwuduotai.top

[S20] C：二分查找
来源：http://hcg.daria6918.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vcs.tarul.cn

[S21] C：字符类别判断
来源：http://aws.hcnkem.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://oce.zdbjq.cn

[S22] C：字符串转数字
来源：http://rgo.fktsv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xhg.hysaishi.cn

[S23] C：随机数
来源：http://fxy.shzxlz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lhf.bjfxy.top

[S24] C：获取本地时间
来源：http://ijp.fzhhl.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tdw.xuetiantiany.cn

[S25] C：内存拷贝
来源：http://vnk.ydzc1.top

memcpy(dst, src, n);
来源：http://pvu.iojbl.cn

[S26] C：内存清零
来源：http://gag.sxryk.cn

memset(a, 0, sizeof a);
来源：http://ukl.jinyuanbaomall.cn

[S27] C：定义常量
来源：http://qof.haohaochexian.top

const double PI = 3.14159;
来源：http://zqn.hesvh.cn

[S28] C：静态变量
来源：http://cdn.hnxiangtu.top

static int counter = 0;
来源：http://nlx.jianghu66.top

[S29] C：变参函数
来源：http://gpg.tianlin.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tek.cheryme.top

[S30] C：头文件保护
来源：http://esa.shzxlz.cn

#ifndef X_H
来源：http://uca.shanyushiyangtech.top

#define X_H
来源：http://cii.sufxvd.cn

#endif
来源：http://arx.tarul.cn

[S31] C++：Hello World
来源：http://nfs.jianghu66.top

#include <iostream>
来源：http://evi.tanke756.top

int main() { std::cout << "Hello\n"; }
来源：http://gfj.zdqjudy.top

[S32] C++：字符串
来源：http://fts.yuxming.cn

std::string s = "hi";  s += "!";
来源：http://ptw.yj202588.top

[S33] C++：vector 增删
来源：http://ipe.ppjwa.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hqr.snrcjt.cn

[S34] C++：遍历 vector
来源：http://gof.hcnkem.com

for (auto &x : v) { std::cout << x; }
来源：http://cea.zhengqikj.top

[S35] C++：map
来源：http://udi.vehdjk.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hrw.kuanghao11.cn

[S36] C++：unordered_map
来源：http://bto.shzxlz.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ioc.meibo888.top

[S37] C++：set
来源：http://alb.birdmap.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bym.hfpthk.cn

[S38] C++：排序
来源：http://jqu.ywan-chungtsiang.top

std::sort(v.begin(), v.end());
来源：http://vxr.cdnleiting.top

[S39] C++：自定义比较器排序
来源：http://twy.hfpthk.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vse.cashguo.top

[S40] C++：查找元素
来源：http://ldb.hesvh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pok.shuidangran.top

[S41] C++：类与构造函数
来源：http://xbg.cdnleiting.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jqd.xinyue.icu

[S42] C++：继承与虚函数
来源：http://uuc.shangyingyoupin.top

class B : public Base { public: void f() override {} };
来源：http://fbx.fzhhl.top

[S43] C++：智能指针
来源：http://hzy.hnxiangtu.top

auto p = std::make_unique<int>(5);
来源：http://fas.aibaodan.cn

[S44] C++：引用传参
来源：http://cnx.havefunace.top

void inc(int &x) { ++x; }
来源：http://nrn.jlsjyb.cn

[S45] C++：lambda
来源：http://nrg.zhaomingkeji.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://huv.ctjpmb.com

[S46] C++：函数模板
来源：http://qhb.vehdjk.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lct.nwbrower.top

[S47] C++：结构化绑定遍历
来源：http://rar.mhx1999.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://thj.zhixingplan.top

[S48] C++：逐行读文件
来源：http://pim.gogol.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gmc.vehdjk.com

while (std::getline(in, line)) { }
来源：http://kgl.mhx1999.top

[S49] C++：写文件
来源：http://swy.wangdashe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mhz.fehbvm.com

[S50] C++：格式化数字
来源：http://vjn.shuidangran.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wsl.cashguo.top

[S51] C++：显式类型转换
来源：http://whl.shzxlz.cn

static_cast<double>(a) / b
来源：http://ndk.nwbrower.top

[S52] C++：const 与 noexcept
来源：http://oxn.jqgufenzy.top

int size() const noexcept { return n_; }
来源：http://ocx.snrcjt.cn

[S53] C++：移动语义
来源：http://jnt.pengpengdd.cyou

std::vector<int> w = std::move(v);
来源：http://jly.jqgfzy.top

[S54] C++：异常处理
来源：http://rcs.hfpthk.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oai.xinyue.icu

[S55] C++：结构化绑定
来源：http://udd.gzhubu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jcw.ppjwa.cn

[S56] C++：optional
来源：http://hti.xziqi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oyy.sjlbkw.cn

[S57] C++：编译期常量
来源：http://zei.haohaochexian.top

constexpr int N = 10;
来源：http://mty.fktsv.cn

[S58] C++：命名空间
来源：http://upa.ctjpmb.com

namespace ns { int f() { return 1; } }
来源：http://bnh.meibo888.top

[S59] C++：静态断言
来源：http://xbu.guowangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fyr.epnwcf.com

[S60] C++：遍历并删除元素
来源：http://mcp.316326.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mma.zhoulong.xyz

================================================================================
来源：http://wiw.jinqigfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nme.9152youxi.cn

================================================================================
来源：http://gdu.guannengcc.top

[T01] Kotlin：Hello World
来源：http://pqo.tianlin.xyz

println("Hello")
来源：http://hql.kuanghao11.cn

[T02] Kotlin：变量
来源：http://zjt.zhoulong.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mqb.zhongyouzk.top

[T03] Kotlin：字符串模板
来源：http://rac.xziqi.cn

"值: $b"
来源：http://qeb.yj20258888.top

[T04] Kotlin：空安全
来源：http://lzq.yangfankeji.com

val n: String? = null;  n?.length
来源：http://wpp.tian-w.cn

[T05] Kotlin：when 表达式
来源：http://mkr.bbcook.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fia.aibaodan.cn

[T06] Kotlin：集合映射
来源：http://fff.ppjwa.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wcl.vehdjk.com

[T07] Kotlin：集合过滤
来源：http://jpe.aibaodan.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://oyq.shanyushiyangtech.top

[T08] Kotlin：数据类
来源：http://rdb.cheryme.top

data class User(val name: String, val age: Int)
来源：http://rca.yonumen.top

[T09] Kotlin：扩展函数
来源：http://bfd.haohaochexian.top

fun String.exclaim() = this + "!"
来源：http://axp.jyoumei.cn

[T10] Kotlin：默认参数
来源：http://tiv.c1oappe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qbf.aibaodan.cn

[T11] Kotlin：协程
来源：http://uhj.bbcook.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qlx.vehdjk.com

[T12] Kotlin：解构声明
来源：http://hwh.havefunace.top

val (a, b) = Pair(1, 2)
来源：http://tou.cheryme.top

[T13] Kotlin：只读 Map
来源：http://wyx.fzhhl.top

val m = mapOf("a" to 1)
来源：http://bqg.chenzaomai.com

[T14] Kotlin：循环
来源：http://yjf.aibaodan.cn

for (i in 1..10) println(i)
来源：http://lie.chenzaomai.com

[T15] Kotlin：接口
来源：http://kos.zycfv.cn

interface Shape { fun area(): Double }
来源：http://jmz.hywenlv.cn

[T16] Swift：Hello World
来源：http://ifi.cqqwz.cn

print("Hello")
来源：http://uqj.ehwqpu.com

[T17] Swift：变量与常量
来源：http://xib.nwbrower.top

var a = 1;  let b = 2
来源：http://ynp.shanyushiyangtech.top

[T18] Swift：字符串插值
来源：http://qzr.snrcjt.cn

"值: \(b)"
来源：http://jko.iojbl.cn

[T19] Swift：可选绑定
来源：http://psv.zhiwuduotai.top

if let n = opt { print(n) }
来源：http://cfq.chenlongwang.top

[T20] Swift：数组操作
来源：http://zgc.yj20258888.top

var a = [1, 2, 3];  a.append(4)
来源：http://mxj.aizwys.cn

[T21] Swift：遍历
来源：http://yvq.yongpay.top

for x in a { print(x) }
来源：http://puc.xingfuxueyuan.xyz

[T22] Swift：字典
来源：http://mul.cashguo.top

var d = ["a": 1];  d["b"] = 2
来源：http://tcp.316326.xyz

[T23] Swift：函数
来源：http://qoa.haohaochexian.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://obp.fehbvm.com

[T24] Swift：闭包
来源：http://jcd.yanxiufei.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ddw.fanxiaobao.xyz

[T25] Swift：结构体
来源：http://qsi.xinyue.icu

struct P { var x: Int }
来源：http://aqz.shuidangran.top

[T26] Swift：类与重写
来源：http://kbk.havefunace.top

class A: Base { override func f() {} }
来源：http://wrg.yvedp.cn

[T27] Swift：错误处理
来源：http://ich.jinghuilouyu.cn

do { try f() } catch { print(error) }
来源：http://dmn.zdbjq.cn

[T28] Swift：枚举
来源：http://axm.sweek.top

enum Color { case red, green }
来源：http://gmz.vehdjk.com

[T29] Swift：guard 提前返回
来源：http://naz.hysaishi.cn

guard let x = opt else { return }
来源：http://lkw.xuanzx.com

[T30] Swift：协议
来源：http://upr.tarul.cn

protocol Shape { func area() -> Double }
来源：http://fbd.shuidangran.top

[T31] Lua：Hello World
来源：http://xet.bjfxy.top

print("Hello")
来源：http://cmd.c1oappe.top

[T32] Lua：局部变量
来源：http://dtu.feifeiyinyue.top

local a = 1
来源：http://qlf.yfazqb.com


<!-- 参考信息 -->