代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://snp.yj20258888.top

[R32] 参数个数校验
来源：http://pdo.sweek.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lit.tian-w.cn

[R33] 捕获错误并提示行号
来源：http://xrj.gaohongyu789.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qpr.hcnkem.com

[R34] 退出时清理
来源：http://ftg.guannengcc.top

trap 'rm -f "$tmp"' EXIT
来源：http://gax.hysaishi.cn

[R35] 后台执行并等待
来源：http://nzn.gaohongyu789.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xiu.yuxming.cn

[R36] 并发执行多个任务
来源：http://ybp.0kj1m.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://avj.0kj1m.cn

[R37] 把输出赋给变量
来源：http://ysw.feifeiyinyue.top

files=$(ls -1)
来源：http://uyt.52xcode.cn

[R38] 管道串联
来源：http://cxa.guowangkeji.top

cat a.txt | grep -i error | wc -l
来源：http://bhf.gogol.net.cn

[R39] 重定向标准输出与错误
来源：http://gds.shzxlz.cn

cmd > out.log 2>&1
来源：http://msk.yj202588.top

[R40] 追加写日志
来源：http://stf.zdqjudy.top

echo "log" >> out.log
来源：http://mhu.yangfankeji.com

[R41] 丢弃输出
来源：http://yps.jinqigfzy.top

cmd >/dev/null 2>&1
来源：http://kzf.shanyushiyangkeji.top

[R42] 输入重定向
来源：http://leo.zdqjudy.top

wc -l < a.txt
来源：http://edq.fengsongda.top

[R43] 按名字查找文件
来源：http://grh.zdbjq.cn

find . -name "*.log" -type f
来源：http://akx.yongpay.top

[R44] 按修改时间查找
来源：http://ytc.sysykeji.top

find . -mtime -7 -type f
来源：http://jgt.chenlongwang.top

[R45] 批量删除
来源：http://rli.ppjwa.cn

find . -name "*.tmp" -delete
来源：http://kvc.316326.xyz

[R46] 递归替换文件内容
来源：http://fkc.jinghuilouyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ugp.ehwqpu.com

[R47] sed 单行替换
来源：http://xiy.jinyuanbaomall.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bio.vehdjk.com

[R48] awk 取指定列
来源：http://vgk.yanxiufei.cn

awk '{print $1, $3}' a.txt
来源：http://sam.ctjpmb.com

[R49] awk 带条件
来源：http://pux.nanxinkj.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rtj.zdbjq.cn

[R50] awk 求和
来源：http://omd.xuanzx.com

awk '{s += $2} END {print s}' a.txt
来源：http://key.cdnleiting.top

[R51] 排序去重取前几
来源：http://cvp.nanxinkj.top

sort a.txt | uniq -c | sort -rn | head
来源：http://mvd.birdmap.top

[R52] 统计行数
来源：http://dmr.zdqjudy.top

wc -l a.txt
来源：http://zxe.mhx1999.top

[R53] 查看文件头与实时尾
来源：http://vmd.jlsjyb.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rlg.redwolf501.top

[R54] 比较两个文件
来源：http://cgt.yuanzhike.top

diff a.txt b.txt
来源：http://vby.birdmap.top

[R55] 压缩与解压
来源：http://jvf.fengsongda.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://duc.yj202588.top

[R56] 远程拷贝
来源：http://xlq.gogol.net.cn

scp file user@host:/path/
来源：http://jss.zdbjq.cn

[R57] 远程执行命令
来源：http://rrm.cashguo.top

ssh user@host 'uptime'
来源：http://roh.zhixingplan.top

[R58] 下载文件
来源：http://eeh.jiagoushi.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gzm.sufxvd.cn

[R59] 发 POST JSON
来源：http://wyh.zdbjq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yfl.sxryk.cn

[R60] 只看 HTTP 状态码
来源：http://uko.yj202588.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://usp.guannengcc.top

[R61] 磁盘占用
来源：http://qph.yj202588.top

df -h;  du -sh *
来源：http://mne.shuidangran.top

[R62] 找最占空间的文件
来源：http://kyu.mhx1999.top

du -ah . | sort -rh | head -10
来源：http://zme.tarul.cn

[R63] 内存与进程
来源：http://qsd.guowangkeji.top

free -h;  ps aux | grep nginx
来源：http://xer.c1oappe.top

[R64] 结束进程
来源：http://nbh.sxryk.cn

kill -9 $(pgrep -f app.py)
来源：http://olt.xylfe.cn

[R65] 查看端口占用
来源：http://jhc.shanyushiyangtech.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cfb.kuanghao11.cn

[R66] 定时任务
来源：http://pld.hongshengwenyu.top

crontab -e;  crontab -l
来源：http://bel.hysaishi.cn

[R67] 生成随机十六进制串
来源：http://mvi.jinyuanbaomall.cn

openssl rand -hex 16
来源：http://mua.hysaishi.cn

[R68] 计算文件校验值
来源：http://tot.yuanzhike.top

sha256sum a.txt;  md5sum a.txt
来源：http://xur.wangdashe.top

[R69] 生成随机密码
来源：http://zbx.yangfankeji.com

head -c 16 /dev/urandom | base64
来源：http://obg.zhijiandao.cn

[R70] 时间戳与互转
来源：http://udt.jinqigfzy.top

date +%s;  date -d @1700000000
来源：http://usf.nanxuanxn.top

[R71] 日期格式化
来源：http://sle.jiagoushi.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://fmd.c1oappe.top

[R72] 等待端口就绪
来源：http://abk.nanxuanxn.top

until nc -z localhost 3306; do sleep 1; done
来源：http://suv.yangfankeji.com

[R73] 分割大日志
来源：http://ona.xuanzx.com

split -l 1000 big.log part_
来源：http://zzj.hesvh.cn

[R74] 批量重命名
来源：http://ote.cdnleiting.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ulm.cheryme.top

[R75] 导出环境变量
来源：http://xxa.jiagoushi.top

export PATH="$HOME/bin:$PATH"
来源：http://hpj.birdmap.top

[R76] 使用临时文件
来源：http://tra.dashuyun.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qli.xinyue.icu

[R77] 读取用户输入
来源：http://arf.tian-w.cn

read -rp "请输入: " ans
来源：http://uhj.316326.xyz

[R78] 交互式菜单
来源：http://jeh.yj20258.top

select opt in a b c; do echo "$opt"; break; done
来源：http://pae.yuxming.cn

[R79] 解析命令行选项
来源：http://oyd.316326.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://aje.zdbjq.cn

[R80] 查看脚本执行耗时
来源：http://xei.tianlin.xyz

time ./run.sh
来源：http://iod.xuanzx.com

================================================================================
来源：http://ueb.gaohongyu789.top

S. C / C++ 专题
来源：http://wnx.aizwys.cn

================================================================================
来源：http://ucz.ybcxt.top

[S01] C：Hello World
来源：http://tvc.zhiwuduotai.top

#include <stdio.h>
来源：http://nni.sufxvd.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://uri.sysykeji.top

[S02] C：变量与格式化输出
来源：http://mav.shzxlz.cn

int a = 10; printf("%d\n", a);
来源：http://oob.wangdashe.top

[S03] C：读入整数
来源：http://kqm.yanxiufei.cn

int x; scanf("%d", &x);
来源：http://uqp.shangyingyoupin.top

[S04] C：字符串复制
来源：http://tvt.sjlbkw.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dho.hnxiangtu.top

[S05] C：字符串长度
来源：http://znw.nanxuanxn.top

strlen(s)
来源：http://dmk.nanxinkj.top

[S06] C：字符串比较
来源：http://xzo.bbcook.cn

strcmp(a, b) == 0
来源：http://zul.jyoumei.cn

[S07] C：数组遍历求和
来源：http://var.yueranfly.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ajg.jianghu66.top

[S08] C：动态内存分配与释放
来源：http://rdm.xuetiantiany.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://aqk.jqgufenzy.top

[S09] C：结构体定义与初始化
来源：http://lvv.daria6918.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cph.vehdjk.com

[S10] C：指针与解引用
来源：http://bsn.yangfankeji.com

int *p = &a;  *p = 5;
来源：http://ldc.xinyue.icu

[S11] C：逐行读文件
来源：http://oft.ywan-chungtsiang.top

FILE *f = fopen("a.txt", "r");
来源：http://nje.shuidangran.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://mye.daria6918.cn

fclose(f);
来源：http://neo.pengpengdd.cyou

[S12] C：写文件
来源：http://erm.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yju.hnqzz.top

[S13] C：宏定义
来源：http://auy.kuanghao11.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dkw.fzhhl.top

[S14] C：枚举
来源：http://fkz.shzxlz.cn

enum Color { RED, GREEN, BLUE };
来源：http://oza.zhaomingkeji.xyz

[S15] C：类型转换
来源：http://muh.aibaodan.cn

(double) a / b
来源：http://tbx.guannengcc.top

[S16] C：位操作置位
来源：http://vcl.hongshengwenyu.top

x |= (1 << 3);
来源：http://kqs.hammf.cn

[S17] C：安全拼接字符串
来源：http://scn.chenzaomai.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fqg.bbcook.cn

[S18] C：命令行参数
来源：http://rzx.jinyuanbaomall.cn

int main(int argc, char **argv)
来源：http://ysm.zhiwuduotai.top

[S19] C：快速排序
来源：http://jsf.jinqigufen.top

qsort(a, n, sizeof(int), cmp);
来源：http://eyb.redwolf501.top

[S20] C：二分查找
来源：http://rpm.nwbrower.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://khj.bbcook.cn

[S21] C：字符类别判断
来源：http://zno.bjfxy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://akw.ybcxt.top

[S22] C：字符串转数字
来源：http://asz.fanxiaobao.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://wla.gzhubu.top

[S23] C：随机数
来源：http://ddt.yj20258.top

srand(time(NULL));  int r = rand() % 100;
来源：http://vdy.jqgufenzy.top

[S24] C：获取本地时间
来源：http://jwl.vqdsnc.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://iag.zhiwuduotai.top

[S25] C：内存拷贝
来源：http://lls.gzhubu.top

memcpy(dst, src, n);
来源：http://zcq.sufxvd.cn

[S26] C：内存清零
来源：http://nin.xylfe.cn

memset(a, 0, sizeof a);
来源：http://pfx.guannengcc.top

[S27] C：定义常量
来源：http://ciz.zycfv.cn

const double PI = 3.14159;
来源：http://srv.yanxiufei.cn

[S28] C：静态变量
来源：http://phf.gogol.net.cn

static int counter = 0;
来源：http://dcc.cdnleiting.top

[S29] C：变参函数
来源：http://vmi.hfpthk.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bgj.vehdjk.com

[S30] C：头文件保护
来源：http://uwg.gotoacloud.top

#ifndef X_H
来源：http://nxb.bbcook.cn

#define X_H
来源：http://ykb.zhaomingkeji.xyz

#endif
来源：http://beh.daria6918.cn

[S31] C++：Hello World
来源：http://lsb.pengpengdd.cyou

#include <iostream>
来源：http://lvz.aibaodan.cn

int main() { std::cout << "Hello\n"; }
来源：http://jdj.zdqjudy.top

[S32] C++：字符串
来源：http://vyj.zycfv.cn

std::string s = "hi";  s += "!";
来源：http://bki.hnqzz.top

[S33] C++：vector 增删
来源：http://tos.zdbjq.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pgb.cheryme.top

[S34] C++：遍历 vector
来源：http://ujk.wangdashe.top

for (auto &x : v) { std::cout << x; }
来源：http://mkz.quarkkingdee.top

[S35] C++：map
来源：http://pan.cdnleiting.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fff.hnqzz.top

[S36] C++：unordered_map
来源：http://oag.xuanzx.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://awi.chenzaomai.com

[S37] C++：set
来源：http://yna.pycfn.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bdd.wangshuangyany.cn

[S38] C++：排序
来源：http://acj.jinyuanbaomall.cn

std::sort(v.begin(), v.end());
来源：http://yrv.jqgufenzy.top

[S39] C++：自定义比较器排序
来源：http://qon.jlsjyb.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hyd.sysykeji.top

[S40] C++：查找元素
来源：http://okf.andypj.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uao.uphjek.com

[S41] C++：类与构造函数
来源：http://mtj.cqqwz.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wkt.cucudq.cn

[S42] C++：继承与虚函数
来源：http://usm.aibaodan.cn

class B : public Base { public: void f() override {} };
来源：http://bas.pycfn.com

[S43] C++：智能指针
来源：http://qws.hywenlv.cn

auto p = std::make_unique<int>(5);
来源：http://jho.jqgfzy.top

[S44] C++：引用传参
来源：http://gpb.daxiang520.top

void inc(int &x) { ++x; }
来源：http://wlr.snrcjt.cn

[S45] C++：lambda
来源：http://wlf.jiagoushi.top

auto add = [](int a, int b) { return a + b; };
来源：http://jxk.jinghuilouyu.cn

[S46] C++：函数模板
来源：http://bfz.yvedp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gpq.yanxiufei.cn

[S47] C++：结构化绑定遍历
来源：http://gpo.bjfxy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vwo.jyoumei.cn

[S48] C++：逐行读文件
来源：http://mxd.quarkkingdee.top

std::ifstream in("a.txt");  std::string line;
来源：http://tkz.redwolf501.top

while (std::getline(in, line)) { }
来源：http://kfa.zycfv.cn

[S49] C++：写文件
来源：http://txx.hammf.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://coh.gzhubu.top

[S50] C++：格式化数字
来源：http://rtr.bjfxy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vov.52xcode.cn

[S51] C++：显式类型转换
来源：http://xfm.sxryk.cn

static_cast<double>(a) / b
来源：http://blp.xziqi.cn

[S52] C++：const 与 noexcept
来源：http://thy.jiagoushi.top

int size() const noexcept { return n_; }
来源：http://pkn.cashguo.top

[S53] C++：移动语义
来源：http://rve.haohaochexian.top

std::vector<int> w = std::move(v);
来源：http://jsb.daxiang520.top

[S54] C++：异常处理
来源：http://yja.sysykeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hwo.chenzaomai.com

[S55] C++：结构化绑定
来源：http://gzj.zhijiandao.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ifm.xylfe.cn

[S56] C++：optional
来源：http://nbt.jinqigufen.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://moh.fehbvm.com

[S57] C++：编译期常量
来源：http://qfj.jqgfzy.top

constexpr int N = 10;
来源：http://hkh.yuanzhike.top

[S58] C++：命名空间
来源：http://ufp.smart0.xyz

namespace ns { int f() { return 1; } }
来源：http://eie.xylfe.cn

[S59] C++：静态断言
来源：http://nms.wangdashe.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://awj.nanxuanxn.top

[S60] C++：遍历并删除元素
来源：http://fsg.jqgufenzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rmh.yonumen.top

================================================================================
来源：http://osl.wangshuangyany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kyb.gogol.net.cn

================================================================================
来源：http://khf.jinqigfzy.top

[T01] Kotlin：Hello World
来源：http://ihq.sysykeji.top

println("Hello")
来源：http://vjd.wangshuangyany.cn

[T02] Kotlin：变量
来源：http://aoq.ydzc1.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yfy.yueranfly.top

[T03] Kotlin：字符串模板
来源：http://dqk.kuanghao11.cn

"值: $b"
来源：http://gno.vehdjk.com

[T04] Kotlin：空安全
来源：http://wei.ppjwa.cn

val n: String? = null;  n?.length
来源：http://htm.cdnleiting.top

[T05] Kotlin：when 表达式
来源：http://pcl.zhoulong.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ycm.jqgfzy.top

[T06] Kotlin：集合映射
来源：http://dms.jianghu66.top

listOf(1, 2, 3).map { it * 2 }
来源：http://vjj.cheryme.top

[T07] Kotlin：集合过滤
来源：http://rnf.cheryme.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://alb.guowangkeji.top

[T08] Kotlin：数据类
来源：http://aan.xuetiantiany.cn

data class User(val name: String, val age: Int)
来源：http://voc.sxryk.cn

[T09] Kotlin：扩展函数
来源：http://xqd.gzhubu.top

fun String.exclaim() = this + "!"
来源：http://pbe.xuanzx.com

[T10] Kotlin：默认参数
来源：http://skp.sufxvd.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://szd.fanxiaobao.xyz

[T11] Kotlin：协程
来源：http://voi.wangdashe.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gnk.pengpengdd.cyou

[T12] Kotlin：解构声明
来源：http://nap.gotoacloud.top

val (a, b) = Pair(1, 2)
来源：http://hqn.shanyushiyangkeji.top

[T13] Kotlin：只读 Map
来源：http://xyc.hammf.cn

val m = mapOf("a" to 1)
来源：http://akv.yfazqb.com

[T14] Kotlin：循环
来源：http://drc.yueranfly.top

for (i in 1..10) println(i)
来源：http://fyu.bjfxy.top

[T15] Kotlin：接口
来源：http://rvx.chenjidiqi.icu

interface Shape { fun area(): Double }
来源：http://sxs.cheryme.top

[T16] Swift：Hello World
来源：http://giq.jiagoushi.top

print("Hello")
来源：http://dhp.vqdsnc.cn

[T17] Swift：变量与常量
来源：http://tid.vehdjk.com

var a = 1;  let b = 2
来源：http://zjv.jlsjyb.cn

[T18] Swift：字符串插值
来源：http://zil.yj20258.top

"值: \(b)"
来源：http://fuh.cucudq.cn

[T19] Swift：可选绑定
来源：http://hqn.zhiwuduotai.top

if let n = opt { print(n) }
来源：http://dex.dashuyun.cn

[T20] Swift：数组操作
来源：http://vgh.meibo888.top

var a = [1, 2, 3];  a.append(4)
来源：http://ybj.hammf.cn

[T21] Swift：遍历
来源：http://buh.quarkkingdee.top

for x in a { print(x) }
来源：http://fcj.yanxiufei.cn

[T22] Swift：字典
来源：http://ocv.yfazqb.com

var d = ["a": 1];  d["b"] = 2
来源：http://qhf.ydzc1.top

[T23] Swift：函数
来源：http://ulr.kuanghao11.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dpt.snrcjt.cn

[T24] Swift：闭包
来源：http://ihl.chenzaomai.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://yop.cucudq.cn

[T25] Swift：结构体
来源：http://awn.gotoacloud.top

struct P { var x: Int }
来源：http://rqo.aizwys.cn

[T26] Swift：类与重写
来源：http://wwu.hfpthk.cn

class A: Base { override func f() {} }
来源：http://dwd.sweek.top

[T27] Swift：错误处理
来源：http://jaf.ppjwa.cn

do { try f() } catch { print(error) }
来源：http://lnh.yongpay.top

[T28] Swift：枚举
来源：http://zbi.tianlin.xyz

enum Color { case red, green }
来源：http://urz.fengsongda.top

[T29] Swift：guard 提前返回
来源：http://nof.sweek.top

guard let x = opt else { return }
来源：http://lyc.redwolf501.top

[T30] Swift：协议
来源：http://jzw.bbcook.cn

protocol Shape { func area() -> Double }
来源：http://blz.zdqjudy.top

[T31] Lua：Hello World
来源：http://wic.yuxming.cn

print("Hello")
来源：http://ria.chenzaomai.com

[T32] Lua：局部变量
来源：http://zoy.yongpay.top

local a = 1
来源：http://pkk.zhoulong.xyz

[T33] Lua：表（数组）
来源：http://dio.hywenlv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nsk.dashuyun.cn

[T34] Lua：遍历表
来源：http://sss.chenjidiqi.icu

for i, v in ipairs(t) do print(i, v) end
来源：http://frl.chenjidiqi.icu


<!-- 参考信息 -->