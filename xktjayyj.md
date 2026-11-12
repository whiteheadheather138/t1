代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://igo.svipenyu.cn

[R36] 并发执行多个任务
来源：http://xmn.316326.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://msy.zdqjudy.top

[R37] 把输出赋给变量
来源：http://llh.gotoacloud.top

files=$(ls -1)
来源：http://hhu.xuanzx.com

[R38] 管道串联
来源：http://qmc.nanxuanxn.top

cat a.txt | grep -i error | wc -l
来源：http://nyj.epnwcf.com

[R39] 重定向标准输出与错误
来源：http://iyz.fanxiaobao.xyz

cmd > out.log 2>&1
来源：http://tyh.yj20258888.top

[R40] 追加写日志
来源：http://ahg.hongshengwenyu.top

echo "log" >> out.log
来源：http://usf.sysykeji.top

[R41] 丢弃输出
来源：http://ndo.0kj1m.cn

cmd >/dev/null 2>&1
来源：http://tbb.ywan-chungtsiang.top

[R42] 输入重定向
来源：http://ret.xziqi.cn

wc -l < a.txt
来源：http://vcl.hongshengwenyu.top

[R43] 按名字查找文件
来源：http://hgv.havefunace.top

find . -name "*.log" -type f
来源：http://idz.dashuyun.cn

[R44] 按修改时间查找
来源：http://jhv.shzxlz.cn

find . -mtime -7 -type f
来源：http://jnw.jqgufenzy.top

[R45] 批量删除
来源：http://rre.chenzaomai.com

find . -name "*.tmp" -delete
来源：http://mvj.shzxlz.cn

[R46] 递归替换文件内容
来源：http://thj.zhixingplan.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zge.hnxiangtu.top

[R47] sed 单行替换
来源：http://ici.shanyushiyangkeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://chl.shangyingyoupin.top

[R48] awk 取指定列
来源：http://vmu.sjlbkw.cn

awk '{print $1, $3}' a.txt
来源：http://gbt.zhaomingkeji.xyz

[R49] awk 带条件
来源：http://osg.andypj.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bku.0kj1m.cn

[R50] awk 求和
来源：http://mdz.hammf.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kva.wangshuangyany.cn

[R51] 排序去重取前几
来源：http://api.nanxuanxn.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ndp.zdqjudy.top

[R52] 统计行数
来源：http://ghi.cqqwz.cn

wc -l a.txt
来源：http://drf.yvedp.cn

[R53] 查看文件头与实时尾
来源：http://qcd.birdmap.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xyz.zdbjq.cn

[R54] 比较两个文件
来源：http://zwb.wangdashe.top

diff a.txt b.txt
来源：http://wqh.chenzaomai.com

[R55] 压缩与解压
来源：http://vau.xuetiantiany.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ymu.fktsv.cn

[R56] 远程拷贝
来源：http://ntx.feifeiyinyue.top

scp file user@host:/path/
来源：http://yjg.sweek.top

[R57] 远程执行命令
来源：http://vnr.bbcook.cn

ssh user@host 'uptime'
来源：http://mwq.guowangkeji.top

[R58] 下载文件
来源：http://vhw.shzxlz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hcs.ehwqpu.com

[R59] 发 POST JSON
来源：http://dgs.nanxuanxn.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://whr.chenjidiqi.icu

[R60] 只看 HTTP 状态码
来源：http://uva.feifeiyinyue.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://okw.jianghu66.top

[R61] 磁盘占用
来源：http://dos.gogol.net.cn

df -h;  du -sh *
来源：http://nkh.epnwcf.com

[R62] 找最占空间的文件
来源：http://umc.ybcxt.top

du -ah . | sort -rh | head -10
来源：http://hxt.daria6918.cn

[R63] 内存与进程
来源：http://ytx.jyoumei.cn

free -h;  ps aux | grep nginx
来源：http://wxo.yueranfly.top

[R64] 结束进程
来源：http://mwn.daria6918.cn

kill -9 $(pgrep -f app.py)
来源：http://hgl.mhx1999.top

[R65] 查看端口占用
来源：http://ldp.hongshengwenyu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cyo.zhixingplan.top

[R66] 定时任务
来源：http://cco.gogol.net.cn

crontab -e;  crontab -l
来源：http://swk.xuanzx.com

[R67] 生成随机十六进制串
来源：http://nmj.jinyuanbaomall.cn

openssl rand -hex 16
来源：http://bvs.xinyue.icu

[R68] 计算文件校验值
来源：http://ltb.zhoulong.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://iwf.yfazqb.com

[R69] 生成随机密码
来源：http://jjp.bbcook.cn

head -c 16 /dev/urandom | base64
来源：http://vne.hongshengwenyu.top

[R70] 时间戳与互转
来源：http://del.hfpthk.cn

date +%s;  date -d @1700000000
来源：http://mdf.ppjwa.cn

[R71] 日期格式化
来源：http://gro.jinqigufen.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://aez.shanyushiyangtech.top

[R72] 等待端口就绪
来源：http://www.iojbl.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://uuh.zhixingplan.top

[R73] 分割大日志
来源：http://zqb.ywan-chungtsiang.top

split -l 1000 big.log part_
来源：http://ktk.vqdsnc.cn

[R74] 批量重命名
来源：http://fep.nwbrower.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oyo.tanke756.top

[R75] 导出环境变量
来源：http://awd.fzhhl.top

export PATH="$HOME/bin:$PATH"
来源：http://lci.yj20258.top

[R76] 使用临时文件
来源：http://ijy.zhiwuduotai.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vyw.ybcxt.top

[R77] 读取用户输入
来源：http://qwi.jinghuilouyu.cn

read -rp "请输入: " ans
来源：http://ohi.tianlin.xyz

[R78] 交互式菜单
来源：http://eak.guannengcc.top

select opt in a b c; do echo "$opt"; break; done
来源：http://kis.hammf.cn

[R79] 解析命令行选项
来源：http://hhw.feifeiyinyue.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jvr.shanyushiyangtech.top

[R80] 查看脚本执行耗时
来源：http://yqs.jqgufenzy.top

time ./run.sh
来源：http://pme.yj20258.top

================================================================================
来源：http://hif.gotoacloud.top

S. C / C++ 专题
来源：http://hzp.sweek.top

================================================================================
来源：http://rxs.jqgfzy.top

[S01] C：Hello World
来源：http://ker.hammf.cn

#include <stdio.h>
来源：http://vvo.ybcxt.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xdm.haohaochexian.top

[S02] C：变量与格式化输出
来源：http://ryd.gzhubu.top

int a = 10; printf("%d\n", a);
来源：http://jzb.birdmap.top

[S03] C：读入整数
来源：http://nmq.yangfankeji.com

int x; scanf("%d", &x);
来源：http://khs.fengsongda.top

[S04] C：字符串复制
来源：http://evh.vehdjk.com

char dst[32]; strcpy(dst, "hi");
来源：http://nqf.yj20258888.top

[S05] C：字符串长度
来源：http://gsz.guowangkeji.top

strlen(s)
来源：http://zaa.pycfn.com

[S06] C：字符串比较
来源：http://xhl.yangfankeji.com

strcmp(a, b) == 0
来源：http://jsj.guowangkeji.top

[S07] C：数组遍历求和
来源：http://sxn.haohaochexian.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bmq.ehwqpu.com

[S08] C：动态内存分配与释放
来源：http://mno.kuanghao11.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kuv.svipenyu.cn

[S09] C：结构体定义与初始化
来源：http://xcp.guannengcc.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vko.316326.xyz

[S10] C：指针与解引用
来源：http://nhl.cashguo.top

int *p = &a;  *p = 5;
来源：http://kty.shanyushiyangtech.top

[S11] C：逐行读文件
来源：http://lzp.zhijiandao.cn

FILE *f = fopen("a.txt", "r");
来源：http://mkr.cashguo.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://dtj.nanxuanxn.top

fclose(f);
来源：http://kqw.nanxuanxn.top

[S12] C：写文件
来源：http://xld.fehbvm.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://izg.shuidangran.top

[S13] C：宏定义
来源：http://zwr.vqdsnc.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zat.haohaochexian.top

[S14] C：枚举
来源：http://juf.zhiwuduotai.top

enum Color { RED, GREEN, BLUE };
来源：http://sjx.jinqigfzy.top

[S15] C：类型转换
来源：http://lon.sjlbkw.cn

(double) a / b
来源：http://ghs.xuetiantiany.cn

[S16] C：位操作置位
来源：http://izx.zycfv.cn

x |= (1 << 3);
来源：http://rar.hammf.cn

[S17] C：安全拼接字符串
来源：http://itb.cqqwz.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://inz.shanyushiyangtech.top

[S18] C：命令行参数
来源：http://vfl.guowangkeji.top

int main(int argc, char **argv)
来源：http://gun.epnwcf.com

[S19] C：快速排序
来源：http://cws.mhx1999.top

qsort(a, n, sizeof(int), cmp);
来源：http://wjz.dashuyun.cn

[S20] C：二分查找
来源：http://rxm.hcnkem.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kzh.ppjwa.cn

[S21] C：字符类别判断
来源：http://ror.feifeiyinyue.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://geh.feifeiyinyue.top

[S22] C：字符串转数字
来源：http://riy.yonumen.top

atoi("42");  strtod("3.14", NULL);
来源：http://kir.hywenlv.cn

[S23] C：随机数
来源：http://ysh.havefunace.top

srand(time(NULL));  int r = rand() % 100;
来源：http://yfp.sysykeji.top

[S24] C：获取本地时间
来源：http://koo.xziqi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cbp.iojbl.cn

[S25] C：内存拷贝
来源：http://ceb.zdbjq.cn

memcpy(dst, src, n);
来源：http://eeo.yangfankeji.com

[S26] C：内存清零
来源：http://hbd.zhongyouzk.top

memset(a, 0, sizeof a);
来源：http://tyt.zhengqikj.top

[S27] C：定义常量
来源：http://nge.cashguo.top

const double PI = 3.14159;
来源：http://ebb.daria6918.cn

[S28] C：静态变量
来源：http://xbi.svipenyu.cn

static int counter = 0;
来源：http://xpr.zhaomingkeji.xyz

[S29] C：变参函数
来源：http://qqw.haohaochexian.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ium.dashuyun.cn

[S30] C：头文件保护
来源：http://ees.zdbjq.cn

#ifndef X_H
来源：http://cak.yuxming.cn

#define X_H
来源：http://owg.guowangkeji.top

#endif
来源：http://rfe.yonumen.top

[S31] C++：Hello World
来源：http://ykb.quarkkingdee.top

#include <iostream>
来源：http://eoh.tian-w.cn

int main() { std::cout << "Hello\n"; }
来源：http://cug.iojbl.cn

[S32] C++：字符串
来源：http://mtl.daxiang520.top

std::string s = "hi";  s += "!";
来源：http://lyn.tanke756.top

[S33] C++：vector 增删
来源：http://ylg.fanxiaobao.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fxj.yfazqb.com

[S34] C++：遍历 vector
来源：http://vlj.yanxiufei.cn

for (auto &x : v) { std::cout << x; }
来源：http://dmt.aibaodan.cn

[S35] C++：map
来源：http://atk.jlsjyb.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://inf.ywan-chungtsiang.top

[S36] C++：unordered_map
来源：http://cbt.zhongyouzk.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://usw.yongpay.top

[S37] C++：set
来源：http://mxr.guannengcc.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rkf.xylfe.cn

[S38] C++：排序
来源：http://pdt.yvedp.cn

std::sort(v.begin(), v.end());
来源：http://rqp.9152youxi.cn

[S39] C++：自定义比较器排序
来源：http://ulv.yuanzhike.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bhg.jiagoushi.top

[S40] C++：查找元素
来源：http://ira.feifeiyinyue.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nvk.shzxlz.cn

[S41] C++：类与构造函数
来源：http://syt.ywan-chungtsiang.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://img.hysaishi.cn

[S42] C++：继承与虚函数
来源：http://zsl.hfpthk.cn

class B : public Base { public: void f() override {} };
来源：http://sxl.meibo888.top

[S43] C++：智能指针
来源：http://svz.yuanzhike.top

auto p = std::make_unique<int>(5);
来源：http://nvh.pengpengdd.cyou

[S44] C++：引用传参
来源：http://kwb.yangfankeji.com

void inc(int &x) { ++x; }
来源：http://tni.yongpay.top

[S45] C++：lambda
来源：http://lfh.jqgfzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://hfy.fanxiaobao.xyz

[S46] C++：函数模板
来源：http://xhf.ivvv.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ugz.hywenlv.cn

[S47] C++：结构化绑定遍历
来源：http://hvx.chenjidiqi.icu

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ovu.vqdsnc.cn

[S48] C++：逐行读文件
来源：http://hnx.yanxiufei.cn

std::ifstream in("a.txt");  std::string line;
来源：http://exl.cucudq.cn

while (std::getline(in, line)) { }
来源：http://qbb.0kj1m.cn

[S49] C++：写文件
来源：http://xte.shuidangran.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tjm.tian-w.cn

[S50] C++：格式化数字
来源：http://nlc.zdbjq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://myt.haohaochexian.top

[S51] C++：显式类型转换
来源：http://uci.wangdashe.top

static_cast<double>(a) / b
来源：http://byw.xylfe.cn

[S52] C++：const 与 noexcept
来源：http://bkf.nanxinkj.top

int size() const noexcept { return n_; }
来源：http://srs.kuanghao11.cn

[S53] C++：移动语义
来源：http://gml.jinqigfzy.top

std::vector<int> w = std::move(v);
来源：http://nby.yonumen.top

[S54] C++：异常处理
来源：http://oal.gogol.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://osh.ybcxt.top

[S55] C++：结构化绑定
来源：http://nyp.pengpengdd.cyou

auto [a, b] = std::make_pair(1, 2);
来源：http://pep.vehdjk.com

[S56] C++：optional
来源：http://qcp.tian-w.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eif.316326.xyz

[S57] C++：编译期常量
来源：http://uis.hywenlv.cn

constexpr int N = 10;
来源：http://leg.svipenyu.cn

[S58] C++：命名空间
来源：http://dcb.shzxlz.cn

namespace ns { int f() { return 1; } }
来源：http://qxg.chenzaomai.com

[S59] C++：静态断言
来源：http://ytu.zhongyouzk.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pcf.yfazqb.com

[S60] C++：遍历并删除元素
来源：http://ffs.0kj1m.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ira.jqgfzy.top

================================================================================
来源：http://kme.smart0.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vgc.mhx1999.top

================================================================================
来源：http://ige.pycfn.com

[T01] Kotlin：Hello World
来源：http://gfc.cqqwz.cn

println("Hello")
来源：http://ddd.zhongyouzk.top

[T02] Kotlin：变量
来源：http://sjq.jqgufenzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rjp.xylfe.cn

[T03] Kotlin：字符串模板
来源：http://dmp.cucudq.cn

"值: $b"
来源：http://brv.aibaodan.cn

[T04] Kotlin：空安全
来源：http://fir.guowangkeji.top

val n: String? = null;  n?.length
来源：http://mrd.yfazqb.com

[T05] Kotlin：when 表达式
来源：http://xyr.cashguo.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kar.aizwys.cn

[T06] Kotlin：集合映射
来源：http://fmr.zhijiandao.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qcc.uphjek.com

[T07] Kotlin：集合过滤
来源：http://aun.redwolf501.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://zgm.xuanzx.com

[T08] Kotlin：数据类
来源：http://tkf.yonumen.top

data class User(val name: String, val age: Int)
来源：http://cyf.sxryk.cn

[T09] Kotlin：扩展函数
来源：http://egf.xylfe.cn

fun String.exclaim() = this + "!"
来源：http://dvf.hongshengwenyu.top

[T10] Kotlin：默认参数
来源：http://etu.gaohongyu789.top

fun greet(name: String = "World") = "Hi $name"
来源：http://oti.sjlbkw.cn

[T11] Kotlin：协程
来源：http://lhe.shanyushiyangtech.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://wrh.sysykeji.top

[T12] Kotlin：解构声明
来源：http://ukz.ivvv.top

val (a, b) = Pair(1, 2)
来源：http://ppw.wangdashe.top

[T13] Kotlin：只读 Map
来源：http://rdr.sjlbkw.cn

val m = mapOf("a" to 1)
来源：http://zwh.xylfe.cn

[T14] Kotlin：循环
来源：http://zpu.jinghuilouyu.cn

for (i in 1..10) println(i)
来源：http://mxa.zhixingplan.top

[T15] Kotlin：接口
来源：http://mxt.gogol.net.cn

interface Shape { fun area(): Double }
来源：http://mvt.dashuyun.cn

[T16] Swift：Hello World
来源：http://rbv.yongpay.top

print("Hello")
来源：http://urr.hfpthk.cn

[T17] Swift：变量与常量
来源：http://qzt.fengsongda.top

var a = 1;  let b = 2
来源：http://lij.daxiang520.top

[T18] Swift：字符串插值
来源：http://dzx.vqdsnc.cn

"值: \(b)"
来源：http://vwb.zhongyouzk.top

[T19] Swift：可选绑定
来源：http://kdr.zhoulong.xyz

if let n = opt { print(n) }
来源：http://bca.yfazqb.com

[T20] Swift：数组操作
来源：http://nlo.zycfv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fnj.yangfankeji.com

[T21] Swift：遍历
来源：http://rrf.jiagoushi.top

for x in a { print(x) }
来源：http://sni.aizwys.cn

[T22] Swift：字典
来源：http://jqx.yfazqb.com

var d = ["a": 1];  d["b"] = 2
来源：http://ipf.zycfv.cn

[T23] Swift：函数
来源：http://vph.xinyue.icu

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ebi.cucudq.cn

[T24] Swift：闭包
来源：http://uou.nwbrower.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://pzl.cqqwz.cn

[T25] Swift：结构体
来源：http://lsa.zhiwuduotai.top

struct P { var x: Int }
来源：http://jtn.yfazqb.com

[T26] Swift：类与重写
来源：http://ova.316326.xyz

class A: Base { override func f() {} }
来源：http://nyy.vqdsnc.cn

[T27] Swift：错误处理
来源：http://ooh.hnqzz.top

do { try f() } catch { print(error) }
来源：http://iut.yangfankeji.com

[T28] Swift：枚举
来源：http://yhc.andypj.xyz

enum Color { case red, green }
来源：http://akm.yj20258888.top

[T29] Swift：guard 提前返回
来源：http://mcz.vqdsnc.cn

guard let x = opt else { return }
来源：http://ztv.svipenyu.cn

[T30] Swift：协议
来源：http://eoc.jianghu66.top

protocol Shape { func area() -> Double }
来源：http://gnu.fktsv.cn

[T31] Lua：Hello World
来源：http://mpl.ppjwa.cn

print("Hello")
来源：http://btn.tarul.cn

[T32] Lua：局部变量
来源：http://cst.kuanghao11.cn

local a = 1
来源：http://uzp.sysykeji.top

[T33] Lua：表（数组）
来源：http://ssc.kuanghao11.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://byq.xuanzx.com

[T34] Lua：遍历表
来源：http://svo.zhiwuduotai.top

for i, v in ipairs(t) do print(i, v) end
来源：http://sut.sweek.top

[T35] Lua：字典表
来源：http://vix.shanyushiyangkeji.top

local d = { a = 1 };  d.b = 2
来源：http://kga.hongshengwenyu.top

[T36] Lua：函数
来源：http://tjt.zhaomingkeji.xyz

function add(a, b) return a + b end
来源：http://tkm.zdqjudy.top

[T37] Lua：字符串拼接
来源：http://xdc.tianlin.xyz

"a" .. "b"
来源：http://von.hfpthk.cn

[T38] Lua：条件
来源：http://uoe.dashuyun.cn

if x > 0 then print("正") end
来源：http://fvx.zhoulong.xyz


<!-- 参考信息 -->