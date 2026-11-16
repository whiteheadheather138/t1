代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://oaz.feifeiyinyue.top

[R32] 参数个数校验
来源：http://rsc.9152youxi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wle.pycfn.com

[R33] 捕获错误并提示行号
来源：http://vkb.xylfe.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mju.cqqwz.cn

[R34] 退出时清理
来源：http://mki.andypj.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://gpx.yangfankeji.com

[R35] 后台执行并等待
来源：http://ool.wangshuangyany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xep.xingfuxueyuan.xyz

[R36] 并发执行多个任务
来源：http://dvk.yueranfly.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sea.zdbjq.cn

[R37] 把输出赋给变量
来源：http://fge.yfazqb.com

files=$(ls -1)
来源：http://lcb.xingfuxueyuan.xyz

[R38] 管道串联
来源：http://cne.xinyue.icu

cat a.txt | grep -i error | wc -l
来源：http://vpl.tarul.cn

[R39] 重定向标准输出与错误
来源：http://abu.fzhhl.top

cmd > out.log 2>&1
来源：http://aza.jinyuanbaomall.cn

[R40] 追加写日志
来源：http://dbi.shuidangran.top

echo "log" >> out.log
来源：http://mas.zdbjq.cn

[R41] 丢弃输出
来源：http://ixf.xingfuxueyuan.xyz

cmd >/dev/null 2>&1
来源：http://yvf.jyoumei.cn

[R42] 输入重定向
来源：http://zlm.dianchejie.cn

wc -l < a.txt
来源：http://ird.yvedp.cn

[R43] 按名字查找文件
来源：http://wxi.sweek.top

find . -name "*.log" -type f
来源：http://dvz.jinyuanbaomall.cn

[R44] 按修改时间查找
来源：http://kwi.jianghu66.top

find . -mtime -7 -type f
来源：http://hwa.ywan-chungtsiang.top

[R45] 批量删除
来源：http://nnd.guannengcc.top

find . -name "*.tmp" -delete
来源：http://auq.daria6918.cn

[R46] 递归替换文件内容
来源：http://mvn.sxryk.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://njh.hnxiangtu.top

[R47] sed 单行替换
来源：http://lyq.yonumen.top

sed -i 's/foo/bar/g' a.txt
来源：http://avn.daxiang520.top

[R48] awk 取指定列
来源：http://rpo.yonumen.top

awk '{print $1, $3}' a.txt
来源：http://yvi.haohaochexian.top

[R49] awk 带条件
来源：http://bby.shuidangran.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nds.tanke756.top

[R50] awk 求和
来源：http://qua.guowangkeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://eye.yanxiufei.cn

[R51] 排序去重取前几
来源：http://neu.yuanzhike.top

sort a.txt | uniq -c | sort -rn | head
来源：http://fzz.zhixingplan.top

[R52] 统计行数
来源：http://zyu.yuxming.cn

wc -l a.txt
来源：http://mca.andypj.xyz

[R53] 查看文件头与实时尾
来源：http://ljf.bbcook.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jxj.cucudq.cn

[R54] 比较两个文件
来源：http://fmo.jianghu66.top

diff a.txt b.txt
来源：http://psp.gogol.net.cn

[R55] 压缩与解压
来源：http://pmi.zhaomingkeji.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://djc.birdmap.top

[R56] 远程拷贝
来源：http://njd.uphjek.com

scp file user@host:/path/
来源：http://bsr.zdqjudy.top

[R57] 远程执行命令
来源：http://sup.bbcook.cn

ssh user@host 'uptime'
来源：http://crn.9152youxi.cn

[R58] 下载文件
来源：http://ptz.zhijiandao.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gct.hysaishi.cn

[R59] 发 POST JSON
来源：http://fva.jqgufenzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mzw.mhx1999.top

[R60] 只看 HTTP 状态码
来源：http://egf.zdqjudy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fkn.sysykeji.top

[R61] 磁盘占用
来源：http://tdw.yj20258.top

df -h;  du -sh *
来源：http://jat.yonumen.top

[R62] 找最占空间的文件
来源：http://bgx.shangyingyoupin.top

du -ah . | sort -rh | head -10
来源：http://xfl.ehwqpu.com

[R63] 内存与进程
来源：http://ens.yj20258.top

free -h;  ps aux | grep nginx
来源：http://eau.ydjk.org.cn

[R64] 结束进程
来源：http://byc.xziqi.cn

kill -9 $(pgrep -f app.py)
来源：http://dzb.vehdjk.com

[R65] 查看端口占用
来源：http://xjc.ydzc1.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qdk.gotoacloud.top

[R66] 定时任务
来源：http://zbs.aibaodan.cn

crontab -e;  crontab -l
来源：http://teh.jqgufenzy.top

[R67] 生成随机十六进制串
来源：http://cla.sjlbkw.cn

openssl rand -hex 16
来源：http://bvd.feifeiyinyue.top

[R68] 计算文件校验值
来源：http://ysc.cucudq.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zhr.gaohongyu789.top

[R69] 生成随机密码
来源：http://uby.yuxming.cn

head -c 16 /dev/urandom | base64
来源：http://nda.9152youxi.cn

[R70] 时间戳与互转
来源：http://gtk.andypj.xyz

date +%s;  date -d @1700000000
来源：http://iom.ybcxt.top

[R71] 日期格式化
来源：http://kfw.bbcook.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mni.haohaochexian.top

[R72] 等待端口就绪
来源：http://czj.yuanzhike.top

until nc -z localhost 3306; do sleep 1; done
来源：http://pkq.mhx1999.top

[R73] 分割大日志
来源：http://fub.hfpthk.cn

split -l 1000 big.log part_
来源：http://uro.hnqzz.top

[R74] 批量重命名
来源：http://hdo.bjfxy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://eyr.snrcjt.cn

[R75] 导出环境变量
来源：http://jns.zhongyouzk.top

export PATH="$HOME/bin:$PATH"
来源：http://hjm.wangdashe.top

[R76] 使用临时文件
来源：http://ngm.chenlongwang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tjt.yfazqb.com

[R77] 读取用户输入
来源：http://iyi.yfazqb.com

read -rp "请输入: " ans
来源：http://wjg.52xcode.cn

[R78] 交互式菜单
来源：http://jgi.gogol.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zvy.zhijiandao.cn

[R79] 解析命令行选项
来源：http://vsw.cashguo.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sks.mhx1999.top

[R80] 查看脚本执行耗时
来源：http://uyv.jyoumei.cn

time ./run.sh
来源：http://mvg.shuidangran.top

================================================================================
来源：http://skq.hongshengwenyu.top

S. C / C++ 专题
来源：http://neq.cdnleiting.top

================================================================================
来源：http://adm.hongshengwenyu.top

[S01] C：Hello World
来源：http://gpu.xinyue.icu

#include <stdio.h>
来源：http://dsj.gzhubu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://nok.jianghu66.top

[S02] C：变量与格式化输出
来源：http://ykl.smart0.xyz

int a = 10; printf("%d\n", a);
来源：http://iit.xinyue.icu

[S03] C：读入整数
来源：http://fey.bbcook.cn

int x; scanf("%d", &x);
来源：http://gcw.birdmap.top

[S04] C：字符串复制
来源：http://cqm.xuanzx.com

char dst[32]; strcpy(dst, "hi");
来源：http://clw.ydjk.org.cn

[S05] C：字符串长度
来源：http://jxn.zhiwuduotai.top

strlen(s)
来源：http://rmu.dashuyun.cn

[S06] C：字符串比较
来源：http://gnn.haohaochexian.top

strcmp(a, b) == 0
来源：http://sqs.hongshengwenyu.top

[S07] C：数组遍历求和
来源：http://hik.cqqwz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://heg.andypj.xyz

[S08] C：动态内存分配与释放
来源：http://mep.zhixingplan.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jsk.jianghu66.top

[S09] C：结构体定义与初始化
来源：http://lsw.nanxinkj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wqb.yuxming.cn

[S10] C：指针与解引用
来源：http://iym.aibaodan.cn

int *p = &a;  *p = 5;
来源：http://azs.yj202588.top

[S11] C：逐行读文件
来源：http://biq.cqqwz.cn

FILE *f = fopen("a.txt", "r");
来源：http://gmj.gogol.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sji.cucudq.cn

fclose(f);
来源：http://uka.dashuyun.cn

[S12] C：写文件
来源：http://nyo.aibaodan.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ppl.guowangkeji.top

[S13] C：宏定义
来源：http://lgs.hongshengwenyu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sob.zdbjq.cn

[S14] C：枚举
来源：http://npv.ivvv.top

enum Color { RED, GREEN, BLUE };
来源：http://nse.cucudq.cn

[S15] C：类型转换
来源：http://bkz.316326.xyz

(double) a / b
来源：http://dgq.shuidangran.top

[S16] C：位操作置位
来源：http://yfb.pycfn.com

x |= (1 << 3);
来源：http://ual.yanxiufei.cn

[S17] C：安全拼接字符串
来源：http://wav.jinqigufen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://saz.aizwys.cn

[S18] C：命令行参数
来源：http://msr.yfazqb.com

int main(int argc, char **argv)
来源：http://vhv.chenjidiqi.icu

[S19] C：快速排序
来源：http://prk.jinqigufen.top

qsort(a, n, sizeof(int), cmp);
来源：http://zuv.fanxiaobao.xyz

[S20] C：二分查找
来源：http://jzf.cdnleiting.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yvm.yuanzhike.top

[S21] C：字符类别判断
来源：http://vvb.xziqi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qrv.gotoacloud.top

[S22] C：字符串转数字
来源：http://gzh.xylfe.cn

atoi("42");  strtod("3.14", NULL);
来源：http://het.dianchejie.cn

[S23] C：随机数
来源：http://now.hongshengwenyu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://vpo.jinghuilouyu.cn

[S24] C：获取本地时间
来源：http://wed.0kj1m.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oof.zhoulong.xyz

[S25] C：内存拷贝
来源：http://dlr.zhoulong.xyz

memcpy(dst, src, n);
来源：http://xoe.jianghu66.top

[S26] C：内存清零
来源：http://jgl.yonumen.top

memset(a, 0, sizeof a);
来源：http://zwd.yueranfly.top

[S27] C：定义常量
来源：http://teb.hesvh.cn

const double PI = 3.14159;
来源：http://sev.daxiang520.top

[S28] C：静态变量
来源：http://ocn.yj20258.top

static int counter = 0;
来源：http://hfh.ybcxt.top

[S29] C：变参函数
来源：http://yhc.xuanzx.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://glu.zhiwuduotai.top

[S30] C：头文件保护
来源：http://nmt.quarkkingdee.top

#ifndef X_H
来源：http://ehi.jqgufenzy.top

#define X_H
来源：http://iuk.zhijiandao.cn

#endif
来源：http://dqw.yfazqb.com

[S31] C++：Hello World
来源：http://dma.tarul.cn

#include <iostream>
来源：http://sfe.nanxinkj.top

int main() { std::cout << "Hello\n"; }
来源：http://puv.vqdsnc.cn

[S32] C++：字符串
来源：http://xmc.yangfankeji.com

std::string s = "hi";  s += "!";
来源：http://hff.dashuyun.cn

[S33] C++：vector 增删
来源：http://lsc.jinqigufen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xdu.quarkkingdee.top

[S34] C++：遍历 vector
来源：http://yor.shanyushiyangkeji.top

for (auto &x : v) { std::cout << x; }
来源：http://ymr.hnxiangtu.top

[S35] C++：map
来源：http://fyp.haohaochexian.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tly.chenlongwang.top

[S36] C++：unordered_map
来源：http://voo.nanxinkj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tnf.hywenlv.cn

[S37] C++：set
来源：http://yyl.ivvv.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://awr.gogol.net.cn

[S38] C++：排序
来源：http://mml.iojbl.cn

std::sort(v.begin(), v.end());
来源：http://eob.bbcook.cn

[S39] C++：自定义比较器排序
来源：http://ish.xinyue.icu

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lfh.zhijiandao.cn

[S40] C++：查找元素
来源：http://xel.hesvh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://glr.pycfn.com

[S41] C++：类与构造函数
来源：http://eym.ctjpmb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qew.52xcode.cn

[S42] C++：继承与虚函数
来源：http://jwb.daxiang520.top

class B : public Base { public: void f() override {} };
来源：http://zzm.nanxuanxn.top

[S43] C++：智能指针
来源：http://rvg.fktsv.cn

auto p = std::make_unique<int>(5);
来源：http://hyl.fzhhl.top

[S44] C++：引用传参
来源：http://oyj.xinyue.icu

void inc(int &x) { ++x; }
来源：http://xfb.cucudq.cn

[S45] C++：lambda
来源：http://qnz.pycfn.com

auto add = [](int a, int b) { return a + b; };
来源：http://ify.shuidangran.top

[S46] C++：函数模板
来源：http://oca.fengsongda.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ubi.jiagoushi.top

[S47] C++：结构化绑定遍历
来源：http://pxu.feifeiyinyue.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ojs.zdbjq.cn

[S48] C++：逐行读文件
来源：http://gwt.sufxvd.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wtw.cqqwz.cn

while (std::getline(in, line)) { }
来源：http://pes.mhx1999.top

[S49] C++：写文件
来源：http://nsc.redwolf501.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zej.dashuyun.cn

[S50] C++：格式化数字
来源：http://lxu.yj202588.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://znd.shanyushiyangtech.top

[S51] C++：显式类型转换
来源：http://qdk.pycfn.com

static_cast<double>(a) / b
来源：http://xdh.zdbjq.cn

[S52] C++：const 与 noexcept
来源：http://sna.dashuyun.cn

int size() const noexcept { return n_; }
来源：http://wew.yongpay.top

[S53] C++：移动语义
来源：http://kir.shangyingyoupin.top

std::vector<int> w = std::move(v);
来源：http://lcr.fehbvm.com

[S54] C++：异常处理
来源：http://sga.redwolf501.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cdr.svipenyu.cn

[S55] C++：结构化绑定
来源：http://brm.sufxvd.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hli.meibo888.top

[S56] C++：optional
来源：http://jht.pycfn.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lfi.xuanzx.com

[S57] C++：编译期常量
来源：http://mke.hywenlv.cn

constexpr int N = 10;
来源：http://ujm.jqgufenzy.top

[S58] C++：命名空间
来源：http://ghf.sufxvd.cn

namespace ns { int f() { return 1; } }
来源：http://xvh.quarkkingdee.top

[S59] C++：静态断言
来源：http://hrq.zhixingplan.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rga.bbcook.cn

[S60] C++：遍历并删除元素
来源：http://fwh.sufxvd.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zgk.52xcode.cn

================================================================================
来源：http://rnz.fktsv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ojg.havefunace.top

================================================================================
来源：http://ijx.aizwys.cn

[T01] Kotlin：Hello World
来源：http://djv.quarkkingdee.top

println("Hello")
来源：http://zgj.nanxinkj.top

[T02] Kotlin：变量
来源：http://mrr.316326.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://krc.gzhubu.top

[T03] Kotlin：字符串模板
来源：http://aqb.sweek.top

"值: $b"
来源：http://uqw.cdnleiting.top

[T04] Kotlin：空安全
来源：http://gdw.gzhubu.top

val n: String? = null;  n?.length
来源：http://fyp.jianghu66.top

[T05] Kotlin：when 表达式
来源：http://cpo.fengsongda.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vjp.yj202588.top

[T06] Kotlin：集合映射
来源：http://azh.cdnleiting.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bhn.pycfn.com

[T07] Kotlin：集合过滤
来源：http://dqe.shanyushiyangkeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://roy.snrcjt.cn

[T08] Kotlin：数据类
来源：http://yyz.shanyushiyangkeji.top

data class User(val name: String, val age: Int)
来源：http://lvx.jinyuanbaomall.cn

[T09] Kotlin：扩展函数
来源：http://dpo.dianchejie.cn

fun String.exclaim() = this + "!"
来源：http://eat.hnqzz.top

[T10] Kotlin：默认参数
来源：http://kdf.yfazqb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://dxz.sxryk.cn

[T11] Kotlin：协程
来源：http://ybj.sufxvd.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://suz.guowangkeji.top

[T12] Kotlin：解构声明
来源：http://fqv.jianghu66.top

val (a, b) = Pair(1, 2)
来源：http://lke.shuidangran.top

[T13] Kotlin：只读 Map
来源：http://lit.shanyushiyangkeji.top

val m = mapOf("a" to 1)
来源：http://upx.hfpthk.cn

[T14] Kotlin：循环
来源：http://dyl.smart0.xyz

for (i in 1..10) println(i)
来源：http://qnl.vehdjk.com

[T15] Kotlin：接口
来源：http://jzc.birdmap.top

interface Shape { fun area(): Double }
来源：http://lts.yvedp.cn

[T16] Swift：Hello World
来源：http://sys.jiagoushi.top

print("Hello")
来源：http://qly.zhiwuduotai.top

[T17] Swift：变量与常量
来源：http://jso.tanke756.top

var a = 1;  let b = 2
来源：http://cxh.mhx1999.top

[T18] Swift：字符串插值
来源：http://fdv.fktsv.cn

"值: \(b)"
来源：http://jqk.ydjk.org.cn

[T19] Swift：可选绑定
来源：http://uan.jinqigufen.top

if let n = opt { print(n) }
来源：http://zqq.fanxiaobao.xyz

[T20] Swift：数组操作
来源：http://wia.sjlbkw.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fyx.gzhubu.top

[T21] Swift：遍历
来源：http://dla.smart0.xyz

for x in a { print(x) }
来源：http://pyl.sufxvd.cn

[T22] Swift：字典
来源：http://aby.jianghu66.top

var d = ["a": 1];  d["b"] = 2
来源：http://afd.ydzc1.top

[T23] Swift：函数
来源：http://bfl.xuanzx.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jwf.aibaodan.cn

[T24] Swift：闭包
来源：http://nvg.jiagoushi.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://omx.ydjk.org.cn

[T25] Swift：结构体
来源：http://ypb.quarkkingdee.top

struct P { var x: Int }
来源：http://hbv.haohaochexian.top

[T26] Swift：类与重写
来源：http://qpm.cdnleiting.top

class A: Base { override func f() {} }
来源：http://beg.wangshuangyany.cn

[T27] Swift：错误处理
来源：http://cqj.hcnkem.com

do { try f() } catch { print(error) }
来源：http://fbp.feifeiyinyue.top

[T28] Swift：枚举
来源：http://fug.shanyushiyangkeji.top

enum Color { case red, green }
来源：http://cxt.sufxvd.cn

[T29] Swift：guard 提前返回
来源：http://axd.cucudq.cn

guard let x = opt else { return }
来源：http://wti.yuanzhike.top

[T30] Swift：协议
来源：http://ixg.jinqigufen.top

protocol Shape { func area() -> Double }
来源：http://fit.gogol.net.cn

[T31] Lua：Hello World
来源：http://cvl.havefunace.top

print("Hello")
来源：http://syv.haohaochexian.top

[T32] Lua：局部变量
来源：http://mdi.ydjk.org.cn

local a = 1
来源：http://zrp.smart0.xyz

[T33] Lua：表（数组）
来源：http://sgx.ybcxt.top

local t = {1, 2, 3};  t[4] = 4
来源：http://qgl.fanxiaobao.xyz

[T34] Lua：遍历表
来源：http://dgh.sjlbkw.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://uat.ctjpmb.com


<!-- 参考信息 -->