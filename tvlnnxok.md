代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://hja.nanxinkj.top

[R36] 并发执行多个任务
来源：http://rhi.guowangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yuq.shanyushiyangtech.top

[R37] 把输出赋给变量
来源：http://mzw.ehwqpu.com

files=$(ls -1)
来源：http://fqr.jianghu66.top

[R38] 管道串联
来源：http://sjr.dianchejie.cn

cat a.txt | grep -i error | wc -l
来源：http://whg.haohaochexian.top

[R39] 重定向标准输出与错误
来源：http://oga.chenzaomai.com

cmd > out.log 2>&1
来源：http://wri.snrcjt.cn

[R40] 追加写日志
来源：http://rdy.shanyushiyangkeji.top

echo "log" >> out.log
来源：http://zdv.zhengqikj.top

[R41] 丢弃输出
来源：http://mjx.fanxiaobao.xyz

cmd >/dev/null 2>&1
来源：http://abr.nanxuanxn.top

[R42] 输入重定向
来源：http://nop.zhongyouzk.top

wc -l < a.txt
来源：http://kck.52xcode.cn

[R43] 按名字查找文件
来源：http://iml.kuanghao11.cn

find . -name "*.log" -type f
来源：http://zuj.pycfn.com

[R44] 按修改时间查找
来源：http://olv.fktsv.cn

find . -mtime -7 -type f
来源：http://uja.ctjpmb.com

[R45] 批量删除
来源：http://gbi.ywan-chungtsiang.top

find . -name "*.tmp" -delete
来源：http://sle.bbcook.cn

[R46] 递归替换文件内容
来源：http://bfv.yvedp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kpr.jianghu66.top

[R47] sed 单行替换
来源：http://umv.gaohongyu789.top

sed -i 's/foo/bar/g' a.txt
来源：http://cci.tarul.cn

[R48] awk 取指定列
来源：http://lgr.hesvh.cn

awk '{print $1, $3}' a.txt
来源：http://xuo.aibaodan.cn

[R49] awk 带条件
来源：http://eek.yonumen.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wlq.hysaishi.cn

[R50] awk 求和
来源：http://ika.haohaochexian.top

awk '{s += $2} END {print s}' a.txt
来源：http://acn.pycfn.com

[R51] 排序去重取前几
来源：http://sbw.cucudq.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nyr.haohaochexian.top

[R52] 统计行数
来源：http://vys.shuidangran.top

wc -l a.txt
来源：http://ume.yuxming.cn

[R53] 查看文件头与实时尾
来源：http://oey.hnxiangtu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mhc.tanke756.top

[R54] 比较两个文件
来源：http://ztu.jlsjyb.cn

diff a.txt b.txt
来源：http://ztn.kuanghao11.cn

[R55] 压缩与解压
来源：http://vuj.cashguo.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fnw.jqgfzy.top

[R56] 远程拷贝
来源：http://rnn.sjlbkw.cn

scp file user@host:/path/
来源：http://tum.zdbjq.cn

[R57] 远程执行命令
来源：http://onv.jiagoushi.top

ssh user@host 'uptime'
来源：http://sxu.tanke756.top

[R58] 下载文件
来源：http://jma.shuidangran.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wwm.ydjk.org.cn

[R59] 发 POST JSON
来源：http://lmc.cqqwz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wro.xuetiantiany.cn

[R60] 只看 HTTP 状态码
来源：http://ooc.feifeiyinyue.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sok.yvedp.cn

[R61] 磁盘占用
来源：http://mli.cucudq.cn

df -h;  du -sh *
来源：http://edq.wangshuangyany.cn

[R62] 找最占空间的文件
来源：http://szk.zhengqikj.top

du -ah . | sort -rh | head -10
来源：http://mhb.guowangkeji.top

[R63] 内存与进程
来源：http://wbn.epnwcf.com

free -h;  ps aux | grep nginx
来源：http://zwj.zdqjudy.top

[R64] 结束进程
来源：http://zsg.jlsjyb.cn

kill -9 $(pgrep -f app.py)
来源：http://ooc.cucudq.cn

[R65] 查看端口占用
来源：http://umj.fengsongda.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gkk.tianlin.xyz

[R66] 定时任务
来源：http://ahg.shuidangran.top

crontab -e;  crontab -l
来源：http://nzt.52xcode.cn

[R67] 生成随机十六进制串
来源：http://zxd.cucudq.cn

openssl rand -hex 16
来源：http://jxv.ydzc1.top

[R68] 计算文件校验值
来源：http://wdb.jqgufenzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://kai.gzhubu.top

[R69] 生成随机密码
来源：http://ics.yj20258888.top

head -c 16 /dev/urandom | base64
来源：http://kfn.hongshengwenyu.top

[R70] 时间戳与互转
来源：http://nae.sxryk.cn

date +%s;  date -d @1700000000
来源：http://cyx.jlsjyb.cn

[R71] 日期格式化
来源：http://cvs.zdbjq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cog.cdnleiting.top

[R72] 等待端口就绪
来源：http://nfj.wangdashe.top

until nc -z localhost 3306; do sleep 1; done
来源：http://bkw.jlsjyb.cn

[R73] 分割大日志
来源：http://lwe.ydjk.org.cn

split -l 1000 big.log part_
来源：http://sgm.hfpthk.cn

[R74] 批量重命名
来源：http://knh.birdmap.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://koi.yfazqb.com

[R75] 导出环境变量
来源：http://soj.ivvv.top

export PATH="$HOME/bin:$PATH"
来源：http://ven.nwbrower.top

[R76] 使用临时文件
来源：http://ohi.sysykeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vas.yongpay.top

[R77] 读取用户输入
来源：http://iqk.jinqigfzy.top

read -rp "请输入: " ans
来源：http://ubb.jlsjyb.cn

[R78] 交互式菜单
来源：http://ujh.fzhhl.top

select opt in a b c; do echo "$opt"; break; done
来源：http://mmg.yvedp.cn

[R79] 解析命令行选项
来源：http://cin.kuanghao11.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://afa.fzhhl.top

[R80] 查看脚本执行耗时
来源：http://tdd.iojbl.cn

time ./run.sh
来源：http://ilu.hcnkem.com

================================================================================
来源：http://eoy.nanxinkj.top

S. C / C++ 专题
来源：http://zew.havefunace.top

================================================================================
来源：http://chg.birdmap.top

[S01] C：Hello World
来源：http://ygs.sxryk.cn

#include <stdio.h>
来源：http://rvz.dashuyun.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kea.dashuyun.cn

[S02] C：变量与格式化输出
来源：http://evm.fktsv.cn

int a = 10; printf("%d\n", a);
来源：http://wlm.hongshengwenyu.top

[S03] C：读入整数
来源：http://ygz.fanxiaobao.xyz

int x; scanf("%d", &x);
来源：http://wij.zhiwuduotai.top

[S04] C：字符串复制
来源：http://odu.chenlongwang.top

char dst[32]; strcpy(dst, "hi");
来源：http://tem.wangshuangyany.cn

[S05] C：字符串长度
来源：http://rgc.0kj1m.cn

strlen(s)
来源：http://yaw.xuetiantiany.cn

[S06] C：字符串比较
来源：http://pau.fktsv.cn

strcmp(a, b) == 0
来源：http://lim.hywenlv.cn

[S07] C：数组遍历求和
来源：http://xie.jqgfzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yli.kuanghao11.cn

[S08] C：动态内存分配与释放
来源：http://wwk.xuanzx.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uun.jinqigfzy.top

[S09] C：结构体定义与初始化
来源：http://vpd.cucudq.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tqi.havefunace.top

[S10] C：指针与解引用
来源：http://iqu.yongpay.top

int *p = &a;  *p = 5;
来源：http://trp.yj20258.top

[S11] C：逐行读文件
来源：http://rlz.xziqi.cn

FILE *f = fopen("a.txt", "r");
来源：http://qmu.c1oappe.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wzq.ywan-chungtsiang.top

fclose(f);
来源：http://gbk.daria6918.cn

[S12] C：写文件
来源：http://fdq.shuidangran.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uif.yanxiufei.cn

[S13] C：宏定义
来源：http://grt.svipenyu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dtt.zdbjq.cn

[S14] C：枚举
来源：http://mqv.jinqigfzy.top

enum Color { RED, GREEN, BLUE };
来源：http://nzj.chenjidiqi.icu

[S15] C：类型转换
来源：http://uic.wangdashe.top

(double) a / b
来源：http://zdh.nanxuanxn.top

[S16] C：位操作置位
来源：http://spi.cheryme.top

x |= (1 << 3);
来源：http://ycu.tianlin.xyz

[S17] C：安全拼接字符串
来源：http://sbw.jinqigfzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pgv.shuidangran.top

[S18] C：命令行参数
来源：http://sxt.jinyuanbaomall.cn

int main(int argc, char **argv)
来源：http://omy.yj202588.top

[S19] C：快速排序
来源：http://lap.shangyingyoupin.top

qsort(a, n, sizeof(int), cmp);
来源：http://jny.jinghuilouyu.cn

[S20] C：二分查找
来源：http://mmr.zhijiandao.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qpk.bjfxy.top

[S21] C：字符类别判断
来源：http://tpe.meibo888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vrs.tarul.cn

[S22] C：字符串转数字
来源：http://oyp.cqqwz.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zzr.hongshengwenyu.top

[S23] C：随机数
来源：http://jva.fzhhl.top

srand(time(NULL));  int r = rand() % 100;
来源：http://vog.jinyuanbaomall.cn

[S24] C：获取本地时间
来源：http://fyn.havefunace.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ukc.zhengqikj.top

[S25] C：内存拷贝
来源：http://nec.xziqi.cn

memcpy(dst, src, n);
来源：http://iyo.shanyushiyangtech.top

[S26] C：内存清零
来源：http://wub.ppjwa.cn

memset(a, 0, sizeof a);
来源：http://qnw.yanxiufei.cn

[S27] C：定义常量
来源：http://xxf.iojbl.cn

const double PI = 3.14159;
来源：http://arv.hnqzz.top

[S28] C：静态变量
来源：http://dfr.gotoacloud.top

static int counter = 0;
来源：http://wtg.yj20258.top

[S29] C：变参函数
来源：http://zdj.redwolf501.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fec.dashuyun.cn

[S30] C：头文件保护
来源：http://ekq.smart0.xyz

#ifndef X_H
来源：http://lzm.bbcook.cn

#define X_H
来源：http://gsp.hammf.cn

#endif
来源：http://vky.jinghuilouyu.cn

[S31] C++：Hello World
来源：http://txr.zhiwuduotai.top

#include <iostream>
来源：http://csx.xuanzx.com

int main() { std::cout << "Hello\n"; }
来源：http://ype.jlsjyb.cn

[S32] C++：字符串
来源：http://qsy.zhiwuduotai.top

std::string s = "hi";  s += "!";
来源：http://gmk.hywenlv.cn

[S33] C++：vector 增删
来源：http://mgb.fanxiaobao.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://toi.dashuyun.cn

[S34] C++：遍历 vector
来源：http://iex.9152youxi.cn

for (auto &x : v) { std::cout << x; }
来源：http://div.cucudq.cn

[S35] C++：map
来源：http://qps.52xcode.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://izv.jinghuilouyu.cn

[S36] C++：unordered_map
来源：http://tbv.yj202588.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zyf.shanyushiyangtech.top

[S37] C++：set
来源：http://odk.sxryk.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hms.vehdjk.com

[S38] C++：排序
来源：http://tpw.birdmap.top

std::sort(v.begin(), v.end());
来源：http://ylv.gogol.net.cn

[S39] C++：自定义比较器排序
来源：http://jsn.wangdashe.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gne.xuetiantiany.cn

[S40] C++：查找元素
来源：http://nqk.c1oappe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://olt.jqgfzy.top

[S41] C++：类与构造函数
来源：http://soz.jqgufenzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mne.jinghuilouyu.cn

[S42] C++：继承与虚函数
来源：http://evc.xylfe.cn

class B : public Base { public: void f() override {} };
来源：http://epj.zhaomingkeji.xyz

[S43] C++：智能指针
来源：http://dks.xingfuxueyuan.xyz

auto p = std::make_unique<int>(5);
来源：http://kos.sjlbkw.cn

[S44] C++：引用传参
来源：http://qvo.shanyushiyangtech.top

void inc(int &x) { ++x; }
来源：http://rfk.yangfankeji.com

[S45] C++：lambda
来源：http://kzs.jlsjyb.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hbx.xylfe.cn

[S46] C++：函数模板
来源：http://njl.cashguo.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fdz.mhx1999.top

[S47] C++：结构化绑定遍历
来源：http://iyl.shangyingyoupin.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pgb.nwbrower.top

[S48] C++：逐行读文件
来源：http://huj.jianghu66.top

std::ifstream in("a.txt");  std::string line;
来源：http://dse.ctjpmb.com

while (std::getline(in, line)) { }
来源：http://cvp.ppjwa.cn

[S49] C++：写文件
来源：http://lfr.yfazqb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kqe.hammf.cn

[S50] C++：格式化数字
来源：http://hor.yonumen.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gwr.mhx1999.top

[S51] C++：显式类型转换
来源：http://dbh.iojbl.cn

static_cast<double>(a) / b
来源：http://cau.ivvv.top

[S52] C++：const 与 noexcept
来源：http://zxc.tanke756.top

int size() const noexcept { return n_; }
来源：http://owc.zhoulong.xyz

[S53] C++：移动语义
来源：http://pmw.yueranfly.top

std::vector<int> w = std::move(v);
来源：http://cms.bbcook.cn

[S54] C++：异常处理
来源：http://rbq.sjlbkw.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ura.fktsv.cn

[S55] C++：结构化绑定
来源：http://zkt.guowangkeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lpu.andypj.xyz

[S56] C++：optional
来源：http://ioi.jinyuanbaomall.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gzy.xylfe.cn

[S57] C++：编译期常量
来源：http://oce.shanyushiyangkeji.top

constexpr int N = 10;
来源：http://qol.daria6918.cn

[S58] C++：命名空间
来源：http://xbz.chenzaomai.com

namespace ns { int f() { return 1; } }
来源：http://jdk.meibo888.top

[S59] C++：静态断言
来源：http://wit.ctjpmb.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gzl.ctjpmb.com

[S60] C++：遍历并删除元素
来源：http://zve.jinyuanbaomall.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rrl.svipenyu.cn

================================================================================
来源：http://hxi.yj202588.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iul.birdmap.top

================================================================================
来源：http://qdz.xuetiantiany.cn

[T01] Kotlin：Hello World
来源：http://gji.tian-w.cn

println("Hello")
来源：http://xtt.c1oappe.top

[T02] Kotlin：变量
来源：http://ckl.yvedp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ggo.xuetiantiany.cn

[T03] Kotlin：字符串模板
来源：http://ujd.ydzc1.top

"值: $b"
来源：http://pxu.c1oappe.top

[T04] Kotlin：空安全
来源：http://kuq.xingfuxueyuan.xyz

val n: String? = null;  n?.length
来源：http://rrt.cashguo.top

[T05] Kotlin：when 表达式
来源：http://lwf.nwbrower.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kgh.shanyushiyangkeji.top

[T06] Kotlin：集合映射
来源：http://kkr.yueranfly.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rqp.quarkkingdee.top

[T07] Kotlin：集合过滤
来源：http://rco.zhoulong.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://imy.ybcxt.top

[T08] Kotlin：数据类
来源：http://whs.gotoacloud.top

data class User(val name: String, val age: Int)
来源：http://pzv.shzxlz.cn

[T09] Kotlin：扩展函数
来源：http://zgb.andypj.xyz

fun String.exclaim() = this + "!"
来源：http://czd.jiagoushi.top

[T10] Kotlin：默认参数
来源：http://wxg.quarkkingdee.top

fun greet(name: String = "World") = "Hi $name"
来源：http://yem.shuidangran.top

[T11] Kotlin：协程
来源：http://efw.zycfv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yyp.0kj1m.cn

[T12] Kotlin：解构声明
来源：http://cgt.smart0.xyz

val (a, b) = Pair(1, 2)
来源：http://zed.yueranfly.top

[T13] Kotlin：只读 Map
来源：http://sjg.jinyuanbaomall.cn

val m = mapOf("a" to 1)
来源：http://hdh.hnxiangtu.top

[T14] Kotlin：循环
来源：http://tgn.xinyue.icu

for (i in 1..10) println(i)
来源：http://gic.yj202588.top

[T15] Kotlin：接口
来源：http://rfz.jinqigfzy.top

interface Shape { fun area(): Double }
来源：http://yav.sweek.top

[T16] Swift：Hello World
来源：http://szf.guowangkeji.top

print("Hello")
来源：http://qsm.nwbrower.top

[T17] Swift：变量与常量
来源：http://fef.cucudq.cn

var a = 1;  let b = 2
来源：http://ppu.fanxiaobao.xyz

[T18] Swift：字符串插值
来源：http://tjs.yfazqb.com

"值: \(b)"
来源：http://eet.jinghuilouyu.cn

[T19] Swift：可选绑定
来源：http://dgy.yongpay.top

if let n = opt { print(n) }
来源：http://uxj.sjlbkw.cn

[T20] Swift：数组操作
来源：http://wys.fzhhl.top

var a = [1, 2, 3];  a.append(4)
来源：http://pat.zhiwuduotai.top

[T21] Swift：遍历
来源：http://imi.svipenyu.cn

for x in a { print(x) }
来源：http://brz.wangdashe.top

[T22] Swift：字典
来源：http://qdx.wangshuangyany.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mso.tanke756.top

[T23] Swift：函数
来源：http://bxn.shangyingyoupin.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ztv.quarkkingdee.top

[T24] Swift：闭包
来源：http://pjw.zhoulong.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://xmp.yj20258.top

[T25] Swift：结构体
来源：http://bds.yueranfly.top

struct P { var x: Int }
来源：http://vbj.zhengqikj.top

[T26] Swift：类与重写
来源：http://ahj.smart0.xyz

class A: Base { override func f() {} }
来源：http://zmm.zdqjudy.top

[T27] Swift：错误处理
来源：http://mgw.hfpthk.cn

do { try f() } catch { print(error) }
来源：http://jok.hesvh.cn

[T28] Swift：枚举
来源：http://lpj.ydzc1.top

enum Color { case red, green }
来源：http://whk.zdbjq.cn

[T29] Swift：guard 提前返回
来源：http://pwl.nanxuanxn.top

guard let x = opt else { return }
来源：http://xzm.sweek.top

[T30] Swift：协议
来源：http://apn.daria6918.cn

protocol Shape { func area() -> Double }
来源：http://vug.aibaodan.cn

[T31] Lua：Hello World
来源：http://aok.chenjidiqi.icu

print("Hello")
来源：http://luq.sweek.top

[T32] Lua：局部变量
来源：http://ebo.wangdashe.top

local a = 1
来源：http://wqy.yongpay.top

[T33] Lua：表（数组）
来源：http://chd.guannengcc.top

local t = {1, 2, 3};  t[4] = 4
来源：http://qmk.0kj1m.cn

[T34] Lua：遍历表
来源：http://cxx.shzxlz.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jhz.ywan-chungtsiang.top

[T35] Lua：字典表
来源：http://lye.hnqzz.top

local d = { a = 1 };  d.b = 2
来源：http://rrn.xziqi.cn

[T36] Lua：函数
来源：http://mnz.yongpay.top

function add(a, b) return a + b end
来源：http://tdk.birdmap.top

[T37] Lua：字符串拼接
来源：http://svb.daria6918.cn

"a" .. "b"
来源：http://usv.meibo888.top

[T38] Lua：条件
来源：http://tie.redwolf501.top

if x > 0 then print("正") end
来源：http://giq.hcnkem.com


<!-- 参考信息 -->