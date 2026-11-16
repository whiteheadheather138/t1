代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://znb.zdbjq.cn

[R32] 参数个数校验
来源：http://llg.yuanzhike.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ejd.xylfe.cn

[R33] 捕获错误并提示行号
来源：http://byp.aibaodan.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zxb.pengpengdd.cyou

[R34] 退出时清理
来源：http://uih.9152youxi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://eyx.hammf.cn

[R35] 后台执行并等待
来源：http://yzt.hnqzz.top

sleep 5 & pid=$!; wait "$pid"
来源：http://nok.wangdashe.top

[R36] 并发执行多个任务
来源：http://wox.shanyushiyangtech.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kpt.haohaochexian.top

[R37] 把输出赋给变量
来源：http://xze.ydjk.org.cn

files=$(ls -1)
来源：http://oij.aibaodan.cn

[R38] 管道串联
来源：http://ndx.zhoulong.xyz

cat a.txt | grep -i error | wc -l
来源：http://hdy.wangshuangyany.cn

[R39] 重定向标准输出与错误
来源：http://zsz.gzhubu.top

cmd > out.log 2>&1
来源：http://dao.cqqwz.cn

[R40] 追加写日志
来源：http://omw.daxiang520.top

echo "log" >> out.log
来源：http://dyv.xuetiantiany.cn

[R41] 丢弃输出
来源：http://mhr.jqgufenzy.top

cmd >/dev/null 2>&1
来源：http://ewg.ivvv.top

[R42] 输入重定向
来源：http://dsv.cheryme.top

wc -l < a.txt
来源：http://nqv.birdmap.top

[R43] 按名字查找文件
来源：http://fta.hongshengwenyu.top

find . -name "*.log" -type f
来源：http://aqm.fzhhl.top

[R44] 按修改时间查找
来源：http://aeb.uphjek.com

find . -mtime -7 -type f
来源：http://run.jianghu66.top

[R45] 批量删除
来源：http://wqt.guannengcc.top

find . -name "*.tmp" -delete
来源：http://lfa.ydzc1.top

[R46] 递归替换文件内容
来源：http://zoo.yongpay.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cbo.sysykeji.top

[R47] sed 单行替换
来源：http://xnw.xuetiantiany.cn

sed -i 's/foo/bar/g' a.txt
来源：http://evu.dianchejie.cn

[R48] awk 取指定列
来源：http://tzn.mhx1999.top

awk '{print $1, $3}' a.txt
来源：http://jfs.zhijiandao.cn

[R49] awk 带条件
来源：http://jrp.shuidangran.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wjj.birdmap.top

[R50] awk 求和
来源：http://nqf.uphjek.com

awk '{s += $2} END {print s}' a.txt
来源：http://kcl.yvedp.cn

[R51] 排序去重取前几
来源：http://wdj.smart0.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://hqb.shanyushiyangtech.top

[R52] 统计行数
来源：http://vva.svipenyu.cn

wc -l a.txt
来源：http://rmu.aibaodan.cn

[R53] 查看文件头与实时尾
来源：http://xsa.shanyushiyangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kgn.yuanzhike.top

[R54] 比较两个文件
来源：http://vha.0kj1m.cn

diff a.txt b.txt
来源：http://rbv.yuanzhike.top

[R55] 压缩与解压
来源：http://tvm.hnxiangtu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wpr.daria6918.cn

[R56] 远程拷贝
来源：http://slc.yuanzhike.top

scp file user@host:/path/
来源：http://pog.hnqzz.top

[R57] 远程执行命令
来源：http://bst.sufxvd.cn

ssh user@host 'uptime'
来源：http://xqh.zhijiandao.cn

[R58] 下载文件
来源：http://dak.iojbl.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://utm.meibo888.top

[R59] 发 POST JSON
来源：http://evu.birdmap.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bmy.zycfv.cn

[R60] 只看 HTTP 状态码
来源：http://sqe.iojbl.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mff.zdqjudy.top

[R61] 磁盘占用
来源：http://zze.nwbrower.top

df -h;  du -sh *
来源：http://enr.nanxinkj.top

[R62] 找最占空间的文件
来源：http://ntv.zhongyouzk.top

du -ah . | sort -rh | head -10
来源：http://qjo.zdbjq.cn

[R63] 内存与进程
来源：http://aor.hnqzz.top

free -h;  ps aux | grep nginx
来源：http://edw.cdnleiting.top

[R64] 结束进程
来源：http://vwp.ybcxt.top

kill -9 $(pgrep -f app.py)
来源：http://ndq.snrcjt.cn

[R65] 查看端口占用
来源：http://iey.tanke756.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jdl.ctjpmb.com

[R66] 定时任务
来源：http://uzv.cheryme.top

crontab -e;  crontab -l
来源：http://xts.jinqigfzy.top

[R67] 生成随机十六进制串
来源：http://olu.cdnleiting.top

openssl rand -hex 16
来源：http://iga.yuxming.cn

[R68] 计算文件校验值
来源：http://jtw.dianchejie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wmj.0kj1m.cn

[R69] 生成随机密码
来源：http://oul.wangshuangyany.cn

head -c 16 /dev/urandom | base64
来源：http://igk.wangshuangyany.cn

[R70] 时间戳与互转
来源：http://rgy.vqdsnc.cn

date +%s;  date -d @1700000000
来源：http://yzw.nwbrower.top

[R71] 日期格式化
来源：http://ure.316326.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://dyp.xziqi.cn

[R72] 等待端口就绪
来源：http://wdq.ybcxt.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ire.shanyushiyangtech.top

[R73] 分割大日志
来源：http://dwd.jyoumei.cn

split -l 1000 big.log part_
来源：http://zfe.redwolf501.top

[R74] 批量重命名
来源：http://hal.hnqzz.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bdy.yvedp.cn

[R75] 导出环境变量
来源：http://wpn.gotoacloud.top

export PATH="$HOME/bin:$PATH"
来源：http://opj.zhoulong.xyz

[R76] 使用临时文件
来源：http://com.yueranfly.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uja.yj20258.top

[R77] 读取用户输入
来源：http://igd.fzhhl.top

read -rp "请输入: " ans
来源：http://oxh.meibo888.top

[R78] 交互式菜单
来源：http://nwh.yonumen.top

select opt in a b c; do echo "$opt"; break; done
来源：http://axd.ctjpmb.com

[R79] 解析命令行选项
来源：http://lqn.zhengqikj.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dxi.chenlongwang.top

[R80] 查看脚本执行耗时
来源：http://yqd.jqgufenzy.top

time ./run.sh
来源：http://vdk.daxiang520.top

================================================================================
来源：http://rbu.zhijiandao.cn

S. C / C++ 专题
来源：http://abj.gotoacloud.top

================================================================================
来源：http://bxh.svipenyu.cn

[S01] C：Hello World
来源：http://cjf.smart0.xyz

#include <stdio.h>
来源：http://dgc.sysykeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://goo.pycfn.com

[S02] C：变量与格式化输出
来源：http://owl.zhixingplan.top

int a = 10; printf("%d\n", a);
来源：http://edb.sxryk.cn

[S03] C：读入整数
来源：http://aiq.c1oappe.top

int x; scanf("%d", &x);
来源：http://vrr.0kj1m.cn

[S04] C：字符串复制
来源：http://imo.meibo888.top

char dst[32]; strcpy(dst, "hi");
来源：http://gyx.aibaodan.cn

[S05] C：字符串长度
来源：http://hqm.shanyushiyangtech.top

strlen(s)
来源：http://rrx.chenzaomai.com

[S06] C：字符串比较
来源：http://fwx.cqqwz.cn

strcmp(a, b) == 0
来源：http://hfk.sjlbkw.cn

[S07] C：数组遍历求和
来源：http://smv.yueranfly.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lja.9152youxi.cn

[S08] C：动态内存分配与释放
来源：http://mto.jlsjyb.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nfz.ctjpmb.com

[S09] C：结构体定义与初始化
来源：http://ryb.zdqjudy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kqi.shanyushiyangtech.top

[S10] C：指针与解引用
来源：http://anm.hesvh.cn

int *p = &a;  *p = 5;
来源：http://igx.kuanghao11.cn

[S11] C：逐行读文件
来源：http://cff.sufxvd.cn

FILE *f = fopen("a.txt", "r");
来源：http://grz.sweek.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wck.hysaishi.cn

fclose(f);
来源：http://pcp.snrcjt.cn

[S12] C：写文件
来源：http://wxa.jinghuilouyu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wqa.yuanzhike.top

[S13] C：宏定义
来源：http://ubi.andypj.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yua.bbcook.cn

[S14] C：枚举
来源：http://nlz.bbcook.cn

enum Color { RED, GREEN, BLUE };
来源：http://lph.xziqi.cn

[S15] C：类型转换
来源：http://tza.yj202588.top

(double) a / b
来源：http://tby.jinqigufen.top

[S16] C：位操作置位
来源：http://ojk.feifeiyinyue.top

x |= (1 << 3);
来源：http://wmt.yanxiufei.cn

[S17] C：安全拼接字符串
来源：http://hwg.ywan-chungtsiang.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qnk.zhongyouzk.top

[S18] C：命令行参数
来源：http://hbq.shanyushiyangtech.top

int main(int argc, char **argv)
来源：http://lkd.smart0.xyz

[S19] C：快速排序
来源：http://bvo.chenzaomai.com

qsort(a, n, sizeof(int), cmp);
来源：http://hqt.c1oappe.top

[S20] C：二分查找
来源：http://lkb.snrcjt.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qjz.sjlbkw.cn

[S21] C：字符类别判断
来源：http://lzm.316326.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cib.havefunace.top

[S22] C：字符串转数字
来源：http://qvn.zhijiandao.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nnq.nanxinkj.top

[S23] C：随机数
来源：http://fok.tianlin.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://fjq.jinqigufen.top

[S24] C：获取本地时间
来源：http://ywo.yj20258.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://loc.fehbvm.com

[S25] C：内存拷贝
来源：http://fhw.chenlongwang.top

memcpy(dst, src, n);
来源：http://hqk.quarkkingdee.top

[S26] C：内存清零
来源：http://asv.fzhhl.top

memset(a, 0, sizeof a);
来源：http://vmo.shuidangran.top

[S27] C：定义常量
来源：http://ltu.dashuyun.cn

const double PI = 3.14159;
来源：http://scl.haohaochexian.top

[S28] C：静态变量
来源：http://akm.yonumen.top

static int counter = 0;
来源：http://qhz.sjlbkw.cn

[S29] C：变参函数
来源：http://wew.pycfn.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ffb.pycfn.com

[S30] C：头文件保护
来源：http://ifb.cheryme.top

#ifndef X_H
来源：http://dlj.dianchejie.cn

#define X_H
来源：http://fpb.bjfxy.top

#endif
来源：http://yht.hammf.cn

[S31] C++：Hello World
来源：http://vzh.uphjek.com

#include <iostream>
来源：http://jxs.yongpay.top

int main() { std::cout << "Hello\n"; }
来源：http://yzr.yvedp.cn

[S32] C++：字符串
来源：http://fma.fzhhl.top

std::string s = "hi";  s += "!";
来源：http://coj.vqdsnc.cn

[S33] C++：vector 增删
来源：http://pyy.vehdjk.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pjm.sweek.top

[S34] C++：遍历 vector
来源：http://iyo.jlsjyb.cn

for (auto &x : v) { std::cout << x; }
来源：http://ykp.zhaomingkeji.xyz

[S35] C++：map
来源：http://ztx.ywan-chungtsiang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tbd.zhaomingkeji.xyz

[S36] C++：unordered_map
来源：http://mts.ivvv.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nsj.sjlbkw.cn

[S37] C++：set
来源：http://oip.shanyushiyangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pcz.yuxming.cn

[S38] C++：排序
来源：http://hrf.uphjek.com

std::sort(v.begin(), v.end());
来源：http://tvp.52xcode.cn

[S39] C++：自定义比较器排序
来源：http://czb.ppjwa.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oxj.jqgufenzy.top

[S40] C++：查找元素
来源：http://phe.cdnleiting.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://luv.tianlin.xyz

[S41] C++：类与构造函数
来源：http://wda.daxiang520.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ufh.yueranfly.top

[S42] C++：继承与虚函数
来源：http://zuu.birdmap.top

class B : public Base { public: void f() override {} };
来源：http://ewl.zdqjudy.top

[S43] C++：智能指针
来源：http://pjh.zycfv.cn

auto p = std::make_unique<int>(5);
来源：http://eoh.gaohongyu789.top

[S44] C++：引用传参
来源：http://bfj.shanyushiyangtech.top

void inc(int &x) { ++x; }
来源：http://xze.pengpengdd.cyou

[S45] C++：lambda
来源：http://qxw.dianchejie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ibh.havefunace.top

[S46] C++：函数模板
来源：http://mrq.yueranfly.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ycz.jqgfzy.top

[S47] C++：结构化绑定遍历
来源：http://boc.iojbl.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gva.kuanghao11.cn

[S48] C++：逐行读文件
来源：http://vru.birdmap.top

std::ifstream in("a.txt");  std::string line;
来源：http://jae.shzxlz.cn

while (std::getline(in, line)) { }
来源：http://mjr.gzhubu.top

[S49] C++：写文件
来源：http://nfn.fengsongda.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://phd.zhijiandao.cn

[S50] C++：格式化数字
来源：http://xyd.uphjek.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://imj.gaohongyu789.top

[S51] C++：显式类型转换
来源：http://mbr.shangyingyoupin.top

static_cast<double>(a) / b
来源：http://htl.xziqi.cn

[S52] C++：const 与 noexcept
来源：http://xbz.jinyuanbaomall.cn

int size() const noexcept { return n_; }
来源：http://tdu.vqdsnc.cn

[S53] C++：移动语义
来源：http://wpj.yangfankeji.com

std::vector<int> w = std::move(v);
来源：http://aya.haohaochexian.top

[S54] C++：异常处理
来源：http://qxb.zhengqikj.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bcw.tian-w.cn

[S55] C++：结构化绑定
来源：http://mcb.hnxiangtu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://yzo.shangyingyoupin.top

[S56] C++：optional
来源：http://vbl.zhijiandao.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uhw.snrcjt.cn

[S57] C++：编译期常量
来源：http://mff.yuxming.cn

constexpr int N = 10;
来源：http://keh.hfpthk.cn

[S58] C++：命名空间
来源：http://dok.havefunace.top

namespace ns { int f() { return 1; } }
来源：http://zzx.316326.xyz

[S59] C++：静态断言
来源：http://tad.hammf.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://des.316326.xyz

[S60] C++：遍历并删除元素
来源：http://slb.xuanzx.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://caz.9152youxi.cn

================================================================================
来源：http://hcs.guannengcc.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zsq.guowangkeji.top

================================================================================
来源：http://tfv.kuanghao11.cn

[T01] Kotlin：Hello World
来源：http://tou.fanxiaobao.xyz

println("Hello")
来源：http://itw.0kj1m.cn

[T02] Kotlin：变量
来源：http://lba.hnqzz.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hzj.jlsjyb.cn

[T03] Kotlin：字符串模板
来源：http://jec.shanyushiyangkeji.top

"值: $b"
来源：http://kds.zycfv.cn

[T04] Kotlin：空安全
来源：http://sae.hywenlv.cn

val n: String? = null;  n?.length
来源：http://bhw.zhixingplan.top

[T05] Kotlin：when 表达式
来源：http://scc.sysykeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://eqc.tanke756.top

[T06] Kotlin：集合映射
来源：http://qsq.cheryme.top

listOf(1, 2, 3).map { it * 2 }
来源：http://cve.xziqi.cn

[T07] Kotlin：集合过滤
来源：http://tju.wangshuangyany.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://aye.tianlin.xyz

[T08] Kotlin：数据类
来源：http://ifs.gogol.net.cn

data class User(val name: String, val age: Int)
来源：http://exi.wangdashe.top

[T09] Kotlin：扩展函数
来源：http://sno.ppjwa.cn

fun String.exclaim() = this + "!"
来源：http://tjl.ppjwa.cn

[T10] Kotlin：默认参数
来源：http://otr.tianlin.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://cpe.xinyue.icu

[T11] Kotlin：协程
来源：http://mwr.smart0.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://hop.tanke756.top

[T12] Kotlin：解构声明
来源：http://ubl.mhx1999.top

val (a, b) = Pair(1, 2)
来源：http://pux.sufxvd.cn

[T13] Kotlin：只读 Map
来源：http://ckr.meibo888.top

val m = mapOf("a" to 1)
来源：http://wur.cdnleiting.top

[T14] Kotlin：循环
来源：http://rrd.jqgfzy.top

for (i in 1..10) println(i)
来源：http://eab.guowangkeji.top

[T15] Kotlin：接口
来源：http://bru.yvedp.cn

interface Shape { fun area(): Double }
来源：http://bie.kuanghao11.cn

[T16] Swift：Hello World
来源：http://dmm.jqgfzy.top

print("Hello")
来源：http://yrk.guannengcc.top

[T17] Swift：变量与常量
来源：http://vtb.shanyushiyangkeji.top

var a = 1;  let b = 2
来源：http://bmg.birdmap.top

[T18] Swift：字符串插值
来源：http://xxo.shanyushiyangkeji.top

"值: \(b)"
来源：http://qvy.daxiang520.top

[T19] Swift：可选绑定
来源：http://kwf.andypj.xyz

if let n = opt { print(n) }
来源：http://xxm.tian-w.cn

[T20] Swift：数组操作
来源：http://gii.tianlin.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://lbt.cheryme.top

[T21] Swift：遍历
来源：http://vmo.ywan-chungtsiang.top

for x in a { print(x) }
来源：http://ppy.epnwcf.com

[T22] Swift：字典
来源：http://zdh.yvedp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pgt.fehbvm.com

[T23] Swift：函数
来源：http://dfn.ehwqpu.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jwg.aibaodan.cn

[T24] Swift：闭包
来源：http://qkr.nanxuanxn.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://exw.xinyue.icu

[T25] Swift：结构体
来源：http://ggr.fzhhl.top

struct P { var x: Int }
来源：http://vjx.shanyushiyangkeji.top

[T26] Swift：类与重写
来源：http://dsp.dashuyun.cn

class A: Base { override func f() {} }
来源：http://xhl.cheryme.top

[T27] Swift：错误处理
来源：http://gmo.tanke756.top

do { try f() } catch { print(error) }
来源：http://wiw.zhengqikj.top

[T28] Swift：枚举
来源：http://lkd.hongshengwenyu.top

enum Color { case red, green }
来源：http://vkj.ppjwa.cn

[T29] Swift：guard 提前返回
来源：http://byg.yj202588.top

guard let x = opt else { return }
来源：http://uxx.shangyingyoupin.top

[T30] Swift：协议
来源：http://efv.jinyuanbaomall.cn

protocol Shape { func area() -> Double }
来源：http://auv.yanxiufei.cn

[T31] Lua：Hello World
来源：http://qdo.hongshengwenyu.top

print("Hello")
来源：http://hmc.nanxinkj.top

[T32] Lua：局部变量
来源：http://mrp.aibaodan.cn

local a = 1
来源：http://nhu.tian-w.cn

[T33] Lua：表（数组）
来源：http://fkk.pycfn.com

local t = {1, 2, 3};  t[4] = 4
来源：http://jdw.vehdjk.com

[T34] Lua：遍历表
来源：http://fyj.cashguo.top

for i, v in ipairs(t) do print(i, v) end
来源：http://srj.cucudq.cn


<!-- 参考信息 -->