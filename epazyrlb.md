代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fpj.gaohongyu789.top

[R34] 退出时清理
来源：http://uvf.cucudq.cn

trap 'rm -f "$tmp"' EXIT
来源：http://yjt.ehwqpu.com

[R35] 后台执行并等待
来源：http://cvs.fengsongda.top

sleep 5 & pid=$!; wait "$pid"
来源：http://okj.hammf.cn

[R36] 并发执行多个任务
来源：http://jvf.fehbvm.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ary.jianghu66.top

[R37] 把输出赋给变量
来源：http://etq.hammf.cn

files=$(ls -1)
来源：http://vsr.yueranfly.top

[R38] 管道串联
来源：http://dcb.hnqzz.top

cat a.txt | grep -i error | wc -l
来源：http://pdv.yongpay.top

[R39] 重定向标准输出与错误
来源：http://jwv.ywan-chungtsiang.top

cmd > out.log 2>&1
来源：http://ioa.tian-w.cn

[R40] 追加写日志
来源：http://uyn.chenlongwang.top

echo "log" >> out.log
来源：http://hza.jyoumei.cn

[R41] 丢弃输出
来源：http://res.zhaomingkeji.xyz

cmd >/dev/null 2>&1
来源：http://uvx.zdbjq.cn

[R42] 输入重定向
来源：http://iom.c1oappe.top

wc -l < a.txt
来源：http://ygd.xinyue.icu

[R43] 按名字查找文件
来源：http://ssd.0kj1m.cn

find . -name "*.log" -type f
来源：http://izt.dashuyun.cn

[R44] 按修改时间查找
来源：http://slb.fanxiaobao.xyz

find . -mtime -7 -type f
来源：http://rdf.shuidangran.top

[R45] 批量删除
来源：http://cqu.ivvv.top

find . -name "*.tmp" -delete
来源：http://mxg.uphjek.com

[R46] 递归替换文件内容
来源：http://dqo.tarul.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sbx.sweek.top

[R47] sed 单行替换
来源：http://tnp.ppjwa.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vxa.xingfuxueyuan.xyz

[R48] awk 取指定列
来源：http://rdo.52xcode.cn

awk '{print $1, $3}' a.txt
来源：http://tbb.zhaomingkeji.xyz

[R49] awk 带条件
来源：http://rmt.zycfv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vbe.jyoumei.cn

[R50] awk 求和
来源：http://vua.smart0.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://svp.ybcxt.top

[R51] 排序去重取前几
来源：http://hxq.quarkkingdee.top

sort a.txt | uniq -c | sort -rn | head
来源：http://rqk.meibo888.top

[R52] 统计行数
来源：http://bti.hnxiangtu.top

wc -l a.txt
来源：http://afy.0kj1m.cn

[R53] 查看文件头与实时尾
来源：http://qkl.0kj1m.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hzg.jinqigufen.top

[R54] 比较两个文件
来源：http://fsr.zhaomingkeji.xyz

diff a.txt b.txt
来源：http://pjm.birdmap.top

[R55] 压缩与解压
来源：http://jcw.chenlongwang.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kap.haohaochexian.top

[R56] 远程拷贝
来源：http://ybw.yangfankeji.com

scp file user@host:/path/
来源：http://izr.daria6918.cn

[R57] 远程执行命令
来源：http://jlx.nwbrower.top

ssh user@host 'uptime'
来源：http://ris.aizwys.cn

[R58] 下载文件
来源：http://gzc.shanyushiyangtech.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wry.shanyushiyangtech.top

[R59] 发 POST JSON
来源：http://siu.cqqwz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dnz.zhixingplan.top

[R60] 只看 HTTP 状态码
来源：http://trw.yanxiufei.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uwv.jlsjyb.cn

[R61] 磁盘占用
来源：http://qgq.gaohongyu789.top

df -h;  du -sh *
来源：http://vxv.yangfankeji.com

[R62] 找最占空间的文件
来源：http://iaq.xinyue.icu

du -ah . | sort -rh | head -10
来源：http://jmx.xuanzx.com

[R63] 内存与进程
来源：http://ukk.shanyushiyangtech.top

free -h;  ps aux | grep nginx
来源：http://har.vqdsnc.cn

[R64] 结束进程
来源：http://zyj.cdnleiting.top

kill -9 $(pgrep -f app.py)
来源：http://nbd.fengsongda.top

[R65] 查看端口占用
来源：http://yll.fanxiaobao.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mpv.jqgufenzy.top

[R66] 定时任务
来源：http://uef.havefunace.top

crontab -e;  crontab -l
来源：http://gur.jianghu66.top

[R67] 生成随机十六进制串
来源：http://qco.havefunace.top

openssl rand -hex 16
来源：http://ebm.ppjwa.cn

[R68] 计算文件校验值
来源：http://bsn.shzxlz.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ddh.zhongyouzk.top

[R69] 生成随机密码
来源：http://zij.cucudq.cn

head -c 16 /dev/urandom | base64
来源：http://bna.aibaodan.cn

[R70] 时间戳与互转
来源：http://nso.zdbjq.cn

date +%s;  date -d @1700000000
来源：http://bxq.snrcjt.cn

[R71] 日期格式化
来源：http://txy.yvedp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kaz.cucudq.cn

[R72] 等待端口就绪
来源：http://qub.snrcjt.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pcw.jinyuanbaomall.cn

[R73] 分割大日志
来源：http://ojm.sufxvd.cn

split -l 1000 big.log part_
来源：http://zbf.jianghu66.top

[R74] 批量重命名
来源：http://hmu.andypj.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://riz.fzhhl.top

[R75] 导出环境变量
来源：http://euq.hysaishi.cn

export PATH="$HOME/bin:$PATH"
来源：http://arr.jinghuilouyu.cn

[R76] 使用临时文件
来源：http://blw.zhengqikj.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nqq.ydjk.org.cn

[R77] 读取用户输入
来源：http://xub.yvedp.cn

read -rp "请输入: " ans
来源：http://ouv.yj20258.top

[R78] 交互式菜单
来源：http://ibl.cucudq.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lka.jqgufenzy.top

[R79] 解析命令行选项
来源：http://mnn.jinqigfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nxc.yj20258.top

[R80] 查看脚本执行耗时
来源：http://dag.mhx1999.top

time ./run.sh
来源：http://ost.ydjk.org.cn

================================================================================
来源：http://xem.hysaishi.cn

S. C / C++ 专题
来源：http://owp.guowangkeji.top

================================================================================
来源：http://zkv.guannengcc.top

[S01] C：Hello World
来源：http://mge.quarkkingdee.top

#include <stdio.h>
来源：http://iyv.dashuyun.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nmq.xuetiantiany.cn

[S02] C：变量与格式化输出
来源：http://hws.jyoumei.cn

int a = 10; printf("%d\n", a);
来源：http://ges.chenjidiqi.icu

[S03] C：读入整数
来源：http://ids.jlsjyb.cn

int x; scanf("%d", &x);
来源：http://zcb.jqgufenzy.top

[S04] C：字符串复制
来源：http://okt.quarkkingdee.top

char dst[32]; strcpy(dst, "hi");
来源：http://ydt.sxryk.cn

[S05] C：字符串长度
来源：http://xjf.aizwys.cn

strlen(s)
来源：http://erm.zhiwuduotai.top

[S06] C：字符串比较
来源：http://bzb.aibaodan.cn

strcmp(a, b) == 0
来源：http://gtq.zycfv.cn

[S07] C：数组遍历求和
来源：http://gtw.xylfe.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pjo.gaohongyu789.top

[S08] C：动态内存分配与释放
来源：http://rak.cashguo.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wbc.hywenlv.cn

[S09] C：结构体定义与初始化
来源：http://wbp.guowangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tep.epnwcf.com

[S10] C：指针与解引用
来源：http://aco.guowangkeji.top

int *p = &a;  *p = 5;
来源：http://pvw.tian-w.cn

[S11] C：逐行读文件
来源：http://ocv.ctjpmb.com

FILE *f = fopen("a.txt", "r");
来源：http://rpr.aizwys.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://our.tanke756.top

fclose(f);
来源：http://vzm.mhx1999.top

[S12] C：写文件
来源：http://beo.zhaomingkeji.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xgj.tianlin.xyz

[S13] C：宏定义
来源：http://kfv.jyoumei.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ozz.xuetiantiany.cn

[S14] C：枚举
来源：http://xbp.52xcode.cn

enum Color { RED, GREEN, BLUE };
来源：http://bgj.xuanzx.com

[S15] C：类型转换
来源：http://uqu.pengpengdd.cyou

(double) a / b
来源：http://bzz.yonumen.top

[S16] C：位操作置位
来源：http://azl.hcnkem.com

x |= (1 << 3);
来源：http://fbx.zhijiandao.cn

[S17] C：安全拼接字符串
来源：http://wfj.mhx1999.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dxc.bbcook.cn

[S18] C：命令行参数
来源：http://hgr.birdmap.top

int main(int argc, char **argv)
来源：http://had.0kj1m.cn

[S19] C：快速排序
来源：http://jrd.chenzaomai.com

qsort(a, n, sizeof(int), cmp);
来源：http://jni.zdqjudy.top

[S20] C：二分查找
来源：http://bkl.nanxinkj.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kjy.yangfankeji.com

[S21] C：字符类别判断
来源：http://qvi.vqdsnc.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vfy.316326.xyz

[S22] C：字符串转数字
来源：http://hvi.shanyushiyangtech.top

atoi("42");  strtod("3.14", NULL);
来源：http://bby.aibaodan.cn

[S23] C：随机数
来源：http://syb.yonumen.top

srand(time(NULL));  int r = rand() % 100;
来源：http://rqr.0kj1m.cn

[S24] C：获取本地时间
来源：http://cdl.yongpay.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nii.gaohongyu789.top

[S25] C：内存拷贝
来源：http://jvs.shzxlz.cn

memcpy(dst, src, n);
来源：http://rod.zhaomingkeji.xyz

[S26] C：内存清零
来源：http://fsu.mhx1999.top

memset(a, 0, sizeof a);
来源：http://sye.sxryk.cn

[S27] C：定义常量
来源：http://nml.feifeiyinyue.top

const double PI = 3.14159;
来源：http://zee.zhijiandao.cn

[S28] C：静态变量
来源：http://tzh.bbcook.cn

static int counter = 0;
来源：http://gxz.ybcxt.top

[S29] C：变参函数
来源：http://dkk.shanyushiyangkeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bvl.mhx1999.top

[S30] C：头文件保护
来源：http://gxb.smart0.xyz

#ifndef X_H
来源：http://txd.zhijiandao.cn

#define X_H
来源：http://nio.sysykeji.top

#endif
来源：http://hwi.hesvh.cn

[S31] C++：Hello World
来源：http://rjd.chenjidiqi.icu

#include <iostream>
来源：http://grt.iojbl.cn

int main() { std::cout << "Hello\n"; }
来源：http://qxb.ivvv.top

[S32] C++：字符串
来源：http://fol.zhoulong.xyz

std::string s = "hi";  s += "!";
来源：http://upa.gotoacloud.top

[S33] C++：vector 增删
来源：http://wok.mhx1999.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://udh.jinghuilouyu.cn

[S34] C++：遍历 vector
来源：http://lwi.chenjidiqi.icu

for (auto &x : v) { std::cout << x; }
来源：http://zvv.hnqzz.top

[S35] C++：map
来源：http://hvq.zhijiandao.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vyj.c1oappe.top

[S36] C++：unordered_map
来源：http://eba.pengpengdd.cyou

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hop.hywenlv.cn

[S37] C++：set
来源：http://mfg.zycfv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dml.zhoulong.xyz

[S38] C++：排序
来源：http://jxu.cashguo.top

std::sort(v.begin(), v.end());
来源：http://nqk.xuetiantiany.cn

[S39] C++：自定义比较器排序
来源：http://srj.shangyingyoupin.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bdo.yj20258888.top

[S40] C++：查找元素
来源：http://jam.ehwqpu.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ibc.dianchejie.cn

[S41] C++：类与构造函数
来源：http://bgk.nwbrower.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hsc.hnxiangtu.top

[S42] C++：继承与虚函数
来源：http://ewa.shzxlz.cn

class B : public Base { public: void f() override {} };
来源：http://app.fengsongda.top

[S43] C++：智能指针
来源：http://ley.ybcxt.top

auto p = std::make_unique<int>(5);
来源：http://knq.yueranfly.top

[S44] C++：引用传参
来源：http://ekh.yj202588.top

void inc(int &x) { ++x; }
来源：http://peu.kuanghao11.cn

[S45] C++：lambda
来源：http://ssf.fzhhl.top

auto add = [](int a, int b) { return a + b; };
来源：http://cgs.zhijiandao.cn

[S46] C++：函数模板
来源：http://ccg.ehwqpu.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://eth.yvedp.cn

[S47] C++：结构化绑定遍历
来源：http://ihz.yj20258.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dvr.tian-w.cn

[S48] C++：逐行读文件
来源：http://lvr.cucudq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wkq.0kj1m.cn

while (std::getline(in, line)) { }
来源：http://mri.fanxiaobao.xyz

[S49] C++：写文件
来源：http://ons.yongpay.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zlo.yvedp.cn

[S50] C++：格式化数字
来源：http://mvf.zdqjudy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vak.haohaochexian.top

[S51] C++：显式类型转换
来源：http://xmf.ehwqpu.com

static_cast<double>(a) / b
来源：http://lhf.sufxvd.cn

[S52] C++：const 与 noexcept
来源：http://rcs.ivvv.top

int size() const noexcept { return n_; }
来源：http://eah.zdbjq.cn

[S53] C++：移动语义
来源：http://ewy.zhongyouzk.top

std::vector<int> w = std::move(v);
来源：http://mjt.ydzc1.top

[S54] C++：异常处理
来源：http://wfv.yonumen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rtb.daria6918.cn

[S55] C++：结构化绑定
来源：http://tqz.nanxinkj.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ube.sjlbkw.cn

[S56] C++：optional
来源：http://ffu.aizwys.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rov.chenzaomai.com

[S57] C++：编译期常量
来源：http://rvc.yj20258888.top

constexpr int N = 10;
来源：http://wso.hysaishi.cn

[S58] C++：命名空间
来源：http://ubp.vehdjk.com

namespace ns { int f() { return 1; } }
来源：http://nrd.meibo888.top

[S59] C++：静态断言
来源：http://gad.zhixingplan.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sop.fengsongda.top

[S60] C++：遍历并删除元素
来源：http://fbo.zycfv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cfu.jqgufenzy.top

================================================================================
来源：http://egj.shzxlz.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gaq.0kj1m.cn

================================================================================
来源：http://zwi.fanxiaobao.xyz

[T01] Kotlin：Hello World
来源：http://qzf.xuetiantiany.cn

println("Hello")
来源：http://vqd.wangshuangyany.cn

[T02] Kotlin：变量
来源：http://rpd.xuanzx.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://roj.316326.xyz

[T03] Kotlin：字符串模板
来源：http://ugf.jqgfzy.top

"值: $b"
来源：http://uly.hesvh.cn

[T04] Kotlin：空安全
来源：http://mtf.daxiang520.top

val n: String? = null;  n?.length
来源：http://foy.daria6918.cn

[T05] Kotlin：when 表达式
来源：http://rqw.guannengcc.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yql.redwolf501.top

[T06] Kotlin：集合映射
来源：http://bip.jianghu66.top

listOf(1, 2, 3).map { it * 2 }
来源：http://xqi.kuanghao11.cn

[T07] Kotlin：集合过滤
来源：http://sye.feifeiyinyue.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ykd.dianchejie.cn

[T08] Kotlin：数据类
来源：http://vra.sweek.top

data class User(val name: String, val age: Int)
来源：http://hcs.quarkkingdee.top

[T09] Kotlin：扩展函数
来源：http://moy.xuanzx.com

fun String.exclaim() = this + "!"
来源：http://eob.chenjidiqi.icu

[T10] Kotlin：默认参数
来源：http://tth.xylfe.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://syw.yj20258.top

[T11] Kotlin：协程
来源：http://fro.bjfxy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://wrn.jinqigfzy.top

[T12] Kotlin：解构声明
来源：http://fkw.chenzaomai.com

val (a, b) = Pair(1, 2)
来源：http://chm.zycfv.cn

[T13] Kotlin：只读 Map
来源：http://knk.feifeiyinyue.top

val m = mapOf("a" to 1)
来源：http://udj.gogol.net.cn

[T14] Kotlin：循环
来源：http://hrj.redwolf501.top

for (i in 1..10) println(i)
来源：http://zea.svipenyu.cn

[T15] Kotlin：接口
来源：http://azg.sufxvd.cn

interface Shape { fun area(): Double }
来源：http://xrg.hfpthk.cn

[T16] Swift：Hello World
来源：http://bkd.cucudq.cn

print("Hello")
来源：http://hnu.pycfn.com

[T17] Swift：变量与常量
来源：http://hbz.zhongyouzk.top

var a = 1;  let b = 2
来源：http://udt.fengsongda.top

[T18] Swift：字符串插值
来源：http://euj.guannengcc.top

"值: \(b)"
来源：http://wux.hnxiangtu.top

[T19] Swift：可选绑定
来源：http://iwo.tianlin.xyz

if let n = opt { print(n) }
来源：http://wcg.fengsongda.top

[T20] Swift：数组操作
来源：http://msh.vehdjk.com

var a = [1, 2, 3];  a.append(4)
来源：http://rvd.zhixingplan.top

[T21] Swift：遍历
来源：http://ath.nwbrower.top

for x in a { print(x) }
来源：http://ipi.jinyuanbaomall.cn

[T22] Swift：字典
来源：http://rfr.wangdashe.top

var d = ["a": 1];  d["b"] = 2
来源：http://mzt.smart0.xyz

[T23] Swift：函数
来源：http://sgk.meibo888.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://civ.jinyuanbaomall.cn

[T24] Swift：闭包
来源：http://gme.zycfv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wwu.zhaomingkeji.xyz

[T25] Swift：结构体
来源：http://aek.zycfv.cn

struct P { var x: Int }
来源：http://tgh.vehdjk.com

[T26] Swift：类与重写
来源：http://dai.fanxiaobao.xyz

class A: Base { override func f() {} }
来源：http://ujr.yj20258888.top

[T27] Swift：错误处理
来源：http://uqq.tian-w.cn

do { try f() } catch { print(error) }
来源：http://jhx.hongshengwenyu.top

[T28] Swift：枚举
来源：http://fes.gogol.net.cn

enum Color { case red, green }
来源：http://zdj.hfpthk.cn

[T29] Swift：guard 提前返回
来源：http://bhd.jqgufenzy.top

guard let x = opt else { return }
来源：http://rqm.jinqigufen.top

[T30] Swift：协议
来源：http://vpa.yueranfly.top

protocol Shape { func area() -> Double }
来源：http://evq.dianchejie.cn

[T31] Lua：Hello World
来源：http://day.fanxiaobao.xyz

print("Hello")
来源：http://nzq.nanxuanxn.top

[T32] Lua：局部变量
来源：http://vsf.ydzc1.top

local a = 1
来源：http://qns.zdbjq.cn

[T33] Lua：表（数组）
来源：http://bme.ydjk.org.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wft.hywenlv.cn

[T34] Lua：遍历表
来源：http://irk.tarul.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gbh.havefunace.top

[T35] Lua：字典表
来源：http://rkp.cashguo.top

local d = { a = 1 };  d.b = 2
来源：http://pzm.yonumen.top

[T36] Lua：函数
来源：http://enx.guannengcc.top

function add(a, b) return a + b end
来源：http://lwc.nanxinkj.top


<!-- 参考信息 -->