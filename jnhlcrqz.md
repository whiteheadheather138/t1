代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://twx.pengpengdd.cyou

[R36] 并发执行多个任务
来源：http://gcr.hnxiangtu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://efs.xziqi.cn

[R37] 把输出赋给变量
来源：http://gjb.guannengcc.top

files=$(ls -1)
来源：http://ewc.fehbvm.com

[R38] 管道串联
来源：http://geo.cdnleiting.top

cat a.txt | grep -i error | wc -l
来源：http://dhd.svipenyu.cn

[R39] 重定向标准输出与错误
来源：http://shj.svipenyu.cn

cmd > out.log 2>&1
来源：http://yzd.svipenyu.cn

[R40] 追加写日志
来源：http://rzr.hesvh.cn

echo "log" >> out.log
来源：http://wjw.cheryme.top

[R41] 丢弃输出
来源：http://jcu.yanxiufei.cn

cmd >/dev/null 2>&1
来源：http://fat.0kj1m.cn

[R42] 输入重定向
来源：http://rfs.svipenyu.cn

wc -l < a.txt
来源：http://koe.vqdsnc.cn

[R43] 按名字查找文件
来源：http://yca.yongpay.top

find . -name "*.log" -type f
来源：http://lni.shanyushiyangkeji.top

[R44] 按修改时间查找
来源：http://rmw.jinghuilouyu.cn

find . -mtime -7 -type f
来源：http://zgf.gogol.net.cn

[R45] 批量删除
来源：http://fuy.aizwys.cn

find . -name "*.tmp" -delete
来源：http://omh.ybcxt.top

[R46] 递归替换文件内容
来源：http://yxb.gzhubu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jtb.jianghu66.top

[R47] sed 单行替换
来源：http://ayx.zycfv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qzs.zhoulong.xyz

[R48] awk 取指定列
来源：http://zys.fanxiaobao.xyz

awk '{print $1, $3}' a.txt
来源：http://dop.hnqzz.top

[R49] awk 带条件
来源：http://suu.uphjek.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ilf.zhijiandao.cn

[R50] awk 求和
来源：http://vhs.cheryme.top

awk '{s += $2} END {print s}' a.txt
来源：http://fxh.dashuyun.cn

[R51] 排序去重取前几
来源：http://xfs.feifeiyinyue.top

sort a.txt | uniq -c | sort -rn | head
来源：http://jsh.quarkkingdee.top

[R52] 统计行数
来源：http://yzw.haohaochexian.top

wc -l a.txt
来源：http://uev.chenzaomai.com

[R53] 查看文件头与实时尾
来源：http://wib.shangyingyoupin.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hui.tanke756.top

[R54] 比较两个文件
来源：http://qrj.redwolf501.top

diff a.txt b.txt
来源：http://xpc.ctjpmb.com

[R55] 压缩与解压
来源：http://wpd.jianghu66.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tzv.zhiwuduotai.top

[R56] 远程拷贝
来源：http://mkd.guannengcc.top

scp file user@host:/path/
来源：http://zje.smart0.xyz

[R57] 远程执行命令
来源：http://abn.jinyuanbaomall.cn

ssh user@host 'uptime'
来源：http://zrp.9152youxi.cn

[R58] 下载文件
来源：http://tpz.yj202588.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zuo.316326.xyz

[R59] 发 POST JSON
来源：http://glp.zhiwuduotai.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hpf.gotoacloud.top

[R60] 只看 HTTP 状态码
来源：http://vrn.hnxiangtu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xdh.ivvv.top

[R61] 磁盘占用
来源：http://tjw.cqqwz.cn

df -h;  du -sh *
来源：http://svy.birdmap.top

[R62] 找最占空间的文件
来源：http://qvc.snrcjt.cn

du -ah . | sort -rh | head -10
来源：http://frn.sjlbkw.cn

[R63] 内存与进程
来源：http://uvc.birdmap.top

free -h;  ps aux | grep nginx
来源：http://fvy.sxryk.cn

[R64] 结束进程
来源：http://bzm.hywenlv.cn

kill -9 $(pgrep -f app.py)
来源：http://qpg.9152youxi.cn

[R65] 查看端口占用
来源：http://ywq.jqgufenzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pgb.daria6918.cn

[R66] 定时任务
来源：http://ray.yonumen.top

crontab -e;  crontab -l
来源：http://ste.cqqwz.cn

[R67] 生成随机十六进制串
来源：http://apw.aizwys.cn

openssl rand -hex 16
来源：http://agq.snrcjt.cn

[R68] 计算文件校验值
来源：http://ojz.yongpay.top

sha256sum a.txt;  md5sum a.txt
来源：http://nis.yj20258.top

[R69] 生成随机密码
来源：http://hoz.hongshengwenyu.top

head -c 16 /dev/urandom | base64
来源：http://qah.shanyushiyangtech.top

[R70] 时间戳与互转
来源：http://tsa.zhaomingkeji.xyz

date +%s;  date -d @1700000000
来源：http://bgc.shuidangran.top

[R71] 日期格式化
来源：http://egy.tarul.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vxm.fktsv.cn

[R72] 等待端口就绪
来源：http://foc.havefunace.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ven.aibaodan.cn

[R73] 分割大日志
来源：http://ycl.sysykeji.top

split -l 1000 big.log part_
来源：http://puw.wangdashe.top

[R74] 批量重命名
来源：http://swf.nanxuanxn.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mlt.jinqigfzy.top

[R75] 导出环境变量
来源：http://itp.zdbjq.cn

export PATH="$HOME/bin:$PATH"
来源：http://rex.vqdsnc.cn

[R76] 使用临时文件
来源：http://wpn.fanxiaobao.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nug.meibo888.top

[R77] 读取用户输入
来源：http://ypn.sxryk.cn

read -rp "请输入: " ans
来源：http://evr.andypj.xyz

[R78] 交互式菜单
来源：http://wtz.yangfankeji.com

select opt in a b c; do echo "$opt"; break; done
来源：http://kvh.cashguo.top

[R79] 解析命令行选项
来源：http://pcf.sysykeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sql.fehbvm.com

[R80] 查看脚本执行耗时
来源：http://tck.shanyushiyangkeji.top

time ./run.sh
来源：http://wwq.hfpthk.cn

================================================================================
来源：http://zof.zhiwuduotai.top

S. C / C++ 专题
来源：http://mqd.zdqjudy.top

================================================================================
来源：http://ebb.gotoacloud.top

[S01] C：Hello World
来源：http://bzf.shangyingyoupin.top

#include <stdio.h>
来源：http://hxq.shzxlz.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gup.sxryk.cn

[S02] C：变量与格式化输出
来源：http://xcg.cheryme.top

int a = 10; printf("%d\n", a);
来源：http://dmh.guowangkeji.top

[S03] C：读入整数
来源：http://vxc.xylfe.cn

int x; scanf("%d", &x);
来源：http://gim.zycfv.cn

[S04] C：字符串复制
来源：http://umr.shangyingyoupin.top

char dst[32]; strcpy(dst, "hi");
来源：http://kgw.ctjpmb.com

[S05] C：字符串长度
来源：http://pfy.yangfankeji.com

strlen(s)
来源：http://kwo.sjlbkw.cn

[S06] C：字符串比较
来源：http://fui.quarkkingdee.top

strcmp(a, b) == 0
来源：http://zau.pengpengdd.cyou

[S07] C：数组遍历求和
来源：http://pne.hongshengwenyu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wog.gaohongyu789.top

[S08] C：动态内存分配与释放
来源：http://xby.c1oappe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zvg.sweek.top

[S09] C：结构体定义与初始化
来源：http://gwu.xingfuxueyuan.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://imx.cucudq.cn

[S10] C：指针与解引用
来源：http://nqb.sjlbkw.cn

int *p = &a;  *p = 5;
来源：http://iee.hnqzz.top

[S11] C：逐行读文件
来源：http://yfy.uphjek.com

FILE *f = fopen("a.txt", "r");
来源：http://nij.zdbjq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tvs.zhaomingkeji.xyz

fclose(f);
来源：http://vip.vehdjk.com

[S12] C：写文件
来源：http://mxn.9152youxi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dll.shangyingyoupin.top

[S13] C：宏定义
来源：http://isz.hfpthk.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fga.fanxiaobao.xyz

[S14] C：枚举
来源：http://flu.zhiwuduotai.top

enum Color { RED, GREEN, BLUE };
来源：http://zdn.zdbjq.cn

[S15] C：类型转换
来源：http://lls.hnqzz.top

(double) a / b
来源：http://ebx.aizwys.cn

[S16] C：位操作置位
来源：http://sbh.9152youxi.cn

x |= (1 << 3);
来源：http://kij.fzhhl.top

[S17] C：安全拼接字符串
来源：http://suu.yuxming.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ltk.xinyue.icu

[S18] C：命令行参数
来源：http://rli.hfpthk.cn

int main(int argc, char **argv)
来源：http://cvv.chenzaomai.com

[S19] C：快速排序
来源：http://vyg.hnxiangtu.top

qsort(a, n, sizeof(int), cmp);
来源：http://gms.hcnkem.com

[S20] C：二分查找
来源：http://ibr.vqdsnc.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kkq.gzhubu.top

[S21] C：字符类别判断
来源：http://qqf.hnqzz.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ulq.c1oappe.top

[S22] C：字符串转数字
来源：http://ovo.xinyue.icu

atoi("42");  strtod("3.14", NULL);
来源：http://mkh.yj20258.top

[S23] C：随机数
来源：http://dvg.yangfankeji.com

srand(time(NULL));  int r = rand() % 100;
来源：http://qgw.jlsjyb.cn

[S24] C：获取本地时间
来源：http://xsz.zdbjq.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hrx.zhaomingkeji.xyz

[S25] C：内存拷贝
来源：http://ags.fktsv.cn

memcpy(dst, src, n);
来源：http://toy.yuxming.cn

[S26] C：内存清零
来源：http://gyd.ydzc1.top

memset(a, 0, sizeof a);
来源：http://xyc.ybcxt.top

[S27] C：定义常量
来源：http://cra.fehbvm.com

const double PI = 3.14159;
来源：http://oad.bjfxy.top

[S28] C：静态变量
来源：http://few.0kj1m.cn

static int counter = 0;
来源：http://vzl.birdmap.top

[S29] C：变参函数
来源：http://tqs.yuanzhike.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qyx.daxiang520.top

[S30] C：头文件保护
来源：http://yha.0kj1m.cn

#ifndef X_H
来源：http://lqq.fengsongda.top

#define X_H
来源：http://csd.hysaishi.cn

#endif
来源：http://rai.hesvh.cn

[S31] C++：Hello World
来源：http://vrw.ywan-chungtsiang.top

#include <iostream>
来源：http://lwa.feifeiyinyue.top

int main() { std::cout << "Hello\n"; }
来源：http://jic.pengpengdd.cyou

[S32] C++：字符串
来源：http://mlg.hongshengwenyu.top

std::string s = "hi";  s += "!";
来源：http://hvi.cheryme.top

[S33] C++：vector 增删
来源：http://yhj.xziqi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sqz.nanxuanxn.top

[S34] C++：遍历 vector
来源：http://xvi.snrcjt.cn

for (auto &x : v) { std::cout << x; }
来源：http://tkm.ydzc1.top

[S35] C++：map
来源：http://noh.ppjwa.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pfj.9152youxi.cn

[S36] C++：unordered_map
来源：http://xsh.xziqi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vaq.chenzaomai.com

[S37] C++：set
来源：http://tex.vehdjk.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://flx.pengpengdd.cyou

[S38] C++：排序
来源：http://mhv.yanxiufei.cn

std::sort(v.begin(), v.end());
来源：http://ydc.sxryk.cn

[S39] C++：自定义比较器排序
来源：http://uze.sjlbkw.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kcq.birdmap.top

[S40] C++：查找元素
来源：http://hup.feifeiyinyue.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dzy.pycfn.com

[S41] C++：类与构造函数
来源：http://jyk.aibaodan.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cwi.jqgfzy.top

[S42] C++：继承与虚函数
来源：http://hdc.jinqigufen.top

class B : public Base { public: void f() override {} };
来源：http://ljv.haohaochexian.top

[S43] C++：智能指针
来源：http://emp.xylfe.cn

auto p = std::make_unique<int>(5);
来源：http://pna.zhixingplan.top

[S44] C++：引用传参
来源：http://krn.smart0.xyz

void inc(int &x) { ++x; }
来源：http://jgl.yfazqb.com

[S45] C++：lambda
来源：http://rih.xingfuxueyuan.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://zvu.cashguo.top

[S46] C++：函数模板
来源：http://bsi.52xcode.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://llq.gogol.net.cn

[S47] C++：结构化绑定遍历
来源：http://rbf.jqgfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nfh.tanke756.top

[S48] C++：逐行读文件
来源：http://yys.jinqigufen.top

std::ifstream in("a.txt");  std::string line;
来源：http://jwl.jiagoushi.top

while (std::getline(in, line)) { }
来源：http://rse.ehwqpu.com

[S49] C++：写文件
来源：http://seb.wangshuangyany.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vjw.birdmap.top

[S50] C++：格式化数字
来源：http://rzq.tanke756.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mxo.yuxming.cn

[S51] C++：显式类型转换
来源：http://bxh.uphjek.com

static_cast<double>(a) / b
来源：http://euj.hnxiangtu.top

[S52] C++：const 与 noexcept
来源：http://dxg.cdnleiting.top

int size() const noexcept { return n_; }
来源：http://dgw.fzhhl.top

[S53] C++：移动语义
来源：http://eal.sysykeji.top

std::vector<int> w = std::move(v);
来源：http://cmb.gogol.net.cn

[S54] C++：异常处理
来源：http://bjf.zycfv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://szv.redwolf501.top

[S55] C++：结构化绑定
来源：http://kxr.tianlin.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://qmm.0kj1m.cn

[S56] C++：optional
来源：http://nfv.chenzaomai.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kyg.cqqwz.cn

[S57] C++：编译期常量
来源：http://zxt.fengsongda.top

constexpr int N = 10;
来源：http://pzu.zdbjq.cn

[S58] C++：命名空间
来源：http://eyz.chenjidiqi.icu

namespace ns { int f() { return 1; } }
来源：http://olv.yj20258.top

[S59] C++：静态断言
来源：http://qmg.kuanghao11.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gby.hesvh.cn

[S60] C++：遍历并删除元素
来源：http://nsz.birdmap.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hti.shangyingyoupin.top

================================================================================
来源：http://jmk.sjlbkw.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qpx.ctjpmb.com

================================================================================
来源：http://rjm.ydzc1.top

[T01] Kotlin：Hello World
来源：http://vvk.guowangkeji.top

println("Hello")
来源：http://rjf.0kj1m.cn

[T02] Kotlin：变量
来源：http://awa.andypj.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gth.hysaishi.cn

[T03] Kotlin：字符串模板
来源：http://deh.feifeiyinyue.top

"值: $b"
来源：http://spp.yj20258.top

[T04] Kotlin：空安全
来源：http://duu.yuanzhike.top

val n: String? = null;  n?.length
来源：http://vxs.cheryme.top

[T05] Kotlin：when 表达式
来源：http://kpj.bbcook.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://aal.jqgfzy.top

[T06] Kotlin：集合映射
来源：http://cmg.guannengcc.top

listOf(1, 2, 3).map { it * 2 }
来源：http://gpu.yj20258888.top

[T07] Kotlin：集合过滤
来源：http://xyh.guannengcc.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mqv.zhaomingkeji.xyz

[T08] Kotlin：数据类
来源：http://bom.nanxinkj.top

data class User(val name: String, val age: Int)
来源：http://dfy.ydzc1.top

[T09] Kotlin：扩展函数
来源：http://lje.zhixingplan.top

fun String.exclaim() = this + "!"
来源：http://qje.ydzc1.top

[T10] Kotlin：默认参数
来源：http://uvc.shanyushiyangkeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://zme.cheryme.top

[T11] Kotlin：协程
来源：http://hph.shanyushiyangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://nwi.shangyingyoupin.top

[T12] Kotlin：解构声明
来源：http://yxn.daxiang520.top

val (a, b) = Pair(1, 2)
来源：http://haq.feifeiyinyue.top

[T13] Kotlin：只读 Map
来源：http://awb.zhixingplan.top

val m = mapOf("a" to 1)
来源：http://fdd.yj20258888.top

[T14] Kotlin：循环
来源：http://shc.gotoacloud.top

for (i in 1..10) println(i)
来源：http://ubb.fzhhl.top

[T15] Kotlin：接口
来源：http://pyu.andypj.xyz

interface Shape { fun area(): Double }
来源：http://cef.hammf.cn

[T16] Swift：Hello World
来源：http://xmp.cashguo.top

print("Hello")
来源：http://qbz.xziqi.cn

[T17] Swift：变量与常量
来源：http://ywa.cheryme.top

var a = 1;  let b = 2
来源：http://usu.yj20258.top

[T18] Swift：字符串插值
来源：http://bhq.hammf.cn

"值: \(b)"
来源：http://mrr.tianlin.xyz

[T19] Swift：可选绑定
来源：http://ihe.jinghuilouyu.cn

if let n = opt { print(n) }
来源：http://wtu.shangyingyoupin.top

[T20] Swift：数组操作
来源：http://wfy.xinyue.icu

var a = [1, 2, 3];  a.append(4)
来源：http://cio.shanyushiyangtech.top

[T21] Swift：遍历
来源：http://kfd.hongshengwenyu.top

for x in a { print(x) }
来源：http://tst.cucudq.cn

[T22] Swift：字典
来源：http://iab.ehwqpu.com

var d = ["a": 1];  d["b"] = 2
来源：http://dpg.yuxming.cn

[T23] Swift：函数
来源：http://pyo.bjfxy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wjd.nwbrower.top

[T24] Swift：闭包
来源：http://siw.jianghu66.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://hyl.jyoumei.cn

[T25] Swift：结构体
来源：http://cml.mhx1999.top

struct P { var x: Int }
来源：http://lad.meibo888.top

[T26] Swift：类与重写
来源：http://ioj.guannengcc.top

class A: Base { override func f() {} }
来源：http://rud.yanxiufei.cn

[T27] Swift：错误处理
来源：http://tbi.yueranfly.top

do { try f() } catch { print(error) }
来源：http://ycn.birdmap.top

[T28] Swift：枚举
来源：http://fuf.yj20258.top

enum Color { case red, green }
来源：http://sed.meibo888.top

[T29] Swift：guard 提前返回
来源：http://ecn.birdmap.top

guard let x = opt else { return }
来源：http://ljh.feifeiyinyue.top

[T30] Swift：协议
来源：http://kgd.ehwqpu.com

protocol Shape { func area() -> Double }
来源：http://brn.haohaochexian.top

[T31] Lua：Hello World
来源：http://giw.smart0.xyz

print("Hello")
来源：http://gsd.gaohongyu789.top

[T32] Lua：局部变量
来源：http://xtz.hongshengwenyu.top

local a = 1
来源：http://vgr.jinghuilouyu.cn

[T33] Lua：表（数组）
来源：http://agu.yonumen.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ppl.zhaomingkeji.xyz

[T34] Lua：遍历表
来源：http://wvc.jinqigfzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ang.hammf.cn

[T35] Lua：字典表
来源：http://tlw.cucudq.cn

local d = { a = 1 };  d.b = 2
来源：http://fxu.shanyushiyangtech.top

[T36] Lua：函数
来源：http://lhu.feifeiyinyue.top

function add(a, b) return a + b end
来源：http://osk.gotoacloud.top

[T37] Lua：字符串拼接
来源：http://ncu.zdqjudy.top

"a" .. "b"
来源：http://vwc.wangdashe.top

[T38] Lua：条件
来源：http://lgy.hammf.cn

if x > 0 then print("正") end
来源：http://kzo.daxiang520.top


<!-- 参考信息 -->