代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://byr.hcnkem.com

[R36] 并发执行多个任务
来源：http://nqn.chenzaomai.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fhk.ehwqpu.com

[R37] 把输出赋给变量
来源：http://rll.vehdjk.com

files=$(ls -1)
来源：http://kyw.gzhubu.top

[R38] 管道串联
来源：http://uuz.shangyingyoupin.top

cat a.txt | grep -i error | wc -l
来源：http://rag.fktsv.cn

[R39] 重定向标准输出与错误
来源：http://bmz.jinghuilouyu.cn

cmd > out.log 2>&1
来源：http://euc.cdnleiting.top

[R40] 追加写日志
来源：http://ghr.0kj1m.cn

echo "log" >> out.log
来源：http://nmv.xingfuxueyuan.xyz

[R41] 丢弃输出
来源：http://yiq.cucudq.cn

cmd >/dev/null 2>&1
来源：http://uin.smart0.xyz

[R42] 输入重定向
来源：http://dlh.aibaodan.cn

wc -l < a.txt
来源：http://jdu.yfazqb.com

[R43] 按名字查找文件
来源：http://pfs.xinyue.icu

find . -name "*.log" -type f
来源：http://adt.guannengcc.top

[R44] 按修改时间查找
来源：http://occ.hongshengwenyu.top

find . -mtime -7 -type f
来源：http://xot.zdqjudy.top

[R45] 批量删除
来源：http://vwj.hcnkem.com

find . -name "*.tmp" -delete
来源：http://ohx.jinqigufen.top

[R46] 递归替换文件内容
来源：http://bxd.fehbvm.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lqk.cashguo.top

[R47] sed 单行替换
来源：http://mwr.dashuyun.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pun.aibaodan.cn

[R48] awk 取指定列
来源：http://wyy.jyoumei.cn

awk '{print $1, $3}' a.txt
来源：http://tlx.hnxiangtu.top

[R49] awk 带条件
来源：http://kwr.zhengqikj.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wnl.nanxinkj.top

[R50] awk 求和
来源：http://hub.yangfankeji.com

awk '{s += $2} END {print s}' a.txt
来源：http://lcg.jinyuanbaomall.cn

[R51] 排序去重取前几
来源：http://wvj.gotoacloud.top

sort a.txt | uniq -c | sort -rn | head
来源：http://hxu.ppjwa.cn

[R52] 统计行数
来源：http://fcc.shangyingyoupin.top

wc -l a.txt
来源：http://olb.dashuyun.cn

[R53] 查看文件头与实时尾
来源：http://fst.chenzaomai.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xii.ydjk.org.cn

[R54] 比较两个文件
来源：http://bfd.uphjek.com

diff a.txt b.txt
来源：http://yzv.hcnkem.com

[R55] 压缩与解压
来源：http://oru.hesvh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kip.zhengqikj.top

[R56] 远程拷贝
来源：http://vqv.yangfankeji.com

scp file user@host:/path/
来源：http://yqq.hysaishi.cn

[R57] 远程执行命令
来源：http://sfn.tian-w.cn

ssh user@host 'uptime'
来源：http://nbf.yj202588.top

[R58] 下载文件
来源：http://dhw.iojbl.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mwx.zhiwuduotai.top

[R59] 发 POST JSON
来源：http://yjy.xylfe.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://exz.jinyuanbaomall.cn

[R60] 只看 HTTP 状态码
来源：http://cbo.zdqjudy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kni.shanyushiyangkeji.top

[R61] 磁盘占用
来源：http://wno.wangdashe.top

df -h;  du -sh *
来源：http://yuy.meibo888.top

[R62] 找最占空间的文件
来源：http://bou.fktsv.cn

du -ah . | sort -rh | head -10
来源：http://hqh.chenzaomai.com

[R63] 内存与进程
来源：http://sua.yangfankeji.com

free -h;  ps aux | grep nginx
来源：http://djk.xuetiantiany.cn

[R64] 结束进程
来源：http://tzp.chenjidiqi.icu

kill -9 $(pgrep -f app.py)
来源：http://jsb.gzhubu.top

[R65] 查看端口占用
来源：http://zym.iojbl.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wkf.xuanzx.com

[R66] 定时任务
来源：http://ait.hywenlv.cn

crontab -e;  crontab -l
来源：http://tnw.9152youxi.cn

[R67] 生成随机十六进制串
来源：http://pgb.zhongyouzk.top

openssl rand -hex 16
来源：http://onm.cashguo.top

[R68] 计算文件校验值
来源：http://rrq.jinqigfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://apn.jianghu66.top

[R69] 生成随机密码
来源：http://jax.cqqwz.cn

head -c 16 /dev/urandom | base64
来源：http://vub.nanxinkj.top

[R70] 时间戳与互转
来源：http://vbs.jlsjyb.cn

date +%s;  date -d @1700000000
来源：http://rfv.svipenyu.cn

[R71] 日期格式化
来源：http://ksu.0kj1m.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rlg.ydzc1.top

[R72] 等待端口就绪
来源：http://itz.cucudq.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cju.feifeiyinyue.top

[R73] 分割大日志
来源：http://ysc.hywenlv.cn

split -l 1000 big.log part_
来源：http://ipo.hesvh.cn

[R74] 批量重命名
来源：http://vwm.ybcxt.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tew.jlsjyb.cn

[R75] 导出环境变量
来源：http://pkn.xuanzx.com

export PATH="$HOME/bin:$PATH"
来源：http://rpb.xziqi.cn

[R76] 使用临时文件
来源：http://scr.tian-w.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://alr.ydjk.org.cn

[R77] 读取用户输入
来源：http://fxc.bjfxy.top

read -rp "请输入: " ans
来源：http://vsp.kuanghao11.cn

[R78] 交互式菜单
来源：http://tan.yj202588.top

select opt in a b c; do echo "$opt"; break; done
来源：http://crv.sweek.top

[R79] 解析命令行选项
来源：http://qlc.52xcode.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sfd.epnwcf.com

[R80] 查看脚本执行耗时
来源：http://nsv.yj20258888.top

time ./run.sh
来源：http://hog.fanxiaobao.xyz

================================================================================
来源：http://zcn.zhongyouzk.top

S. C / C++ 专题
来源：http://wwm.ydjk.org.cn

================================================================================
来源：http://wjj.feifeiyinyue.top

[S01] C：Hello World
来源：http://rof.shzxlz.cn

#include <stdio.h>
来源：http://zah.chenlongwang.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wij.tian-w.cn

[S02] C：变量与格式化输出
来源：http://sxf.tianlin.xyz

int a = 10; printf("%d\n", a);
来源：http://fzm.yuanzhike.top

[S03] C：读入整数
来源：http://zhd.havefunace.top

int x; scanf("%d", &x);
来源：http://hdx.cashguo.top

[S04] C：字符串复制
来源：http://jqr.pycfn.com

char dst[32]; strcpy(dst, "hi");
来源：http://xjm.sjlbkw.cn

[S05] C：字符串长度
来源：http://hyo.zhengqikj.top

strlen(s)
来源：http://onw.shuidangran.top

[S06] C：字符串比较
来源：http://glf.daria6918.cn

strcmp(a, b) == 0
来源：http://nwu.ehwqpu.com

[S07] C：数组遍历求和
来源：http://unv.andypj.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ujt.shzxlz.cn

[S08] C：动态内存分配与释放
来源：http://wem.hammf.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://iim.wangshuangyany.cn

[S09] C：结构体定义与初始化
来源：http://mcq.tanke756.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gpq.guowangkeji.top

[S10] C：指针与解引用
来源：http://pvx.zhongyouzk.top

int *p = &a;  *p = 5;
来源：http://kkm.hcnkem.com

[S11] C：逐行读文件
来源：http://qkd.pengpengdd.cyou

FILE *f = fopen("a.txt", "r");
来源：http://wtw.snrcjt.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://myx.xziqi.cn

fclose(f);
来源：http://zrd.zdqjudy.top

[S12] C：写文件
来源：http://edg.hnxiangtu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qxp.yongpay.top

[S13] C：宏定义
来源：http://mzi.kuanghao11.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uac.shanyushiyangtech.top

[S14] C：枚举
来源：http://cmd.zhijiandao.cn

enum Color { RED, GREEN, BLUE };
来源：http://evl.havefunace.top

[S15] C：类型转换
来源：http://usq.yvedp.cn

(double) a / b
来源：http://dqj.ydjk.org.cn

[S16] C：位操作置位
来源：http://wko.haohaochexian.top

x |= (1 << 3);
来源：http://kxg.9152youxi.cn

[S17] C：安全拼接字符串
来源：http://pax.guannengcc.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gim.0kj1m.cn

[S18] C：命令行参数
来源：http://owh.shzxlz.cn

int main(int argc, char **argv)
来源：http://qay.zhixingplan.top

[S19] C：快速排序
来源：http://pnl.gotoacloud.top

qsort(a, n, sizeof(int), cmp);
来源：http://tcn.sweek.top

[S20] C：二分查找
来源：http://vdn.xuetiantiany.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nfz.zhaomingkeji.xyz

[S21] C：字符类别判断
来源：http://jrv.zdbjq.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dbh.pycfn.com

[S22] C：字符串转数字
来源：http://wne.xylfe.cn

atoi("42");  strtod("3.14", NULL);
来源：http://mtt.tanke756.top

[S23] C：随机数
来源：http://xmk.yj20258.top

srand(time(NULL));  int r = rand() % 100;
来源：http://nzi.hnxiangtu.top

[S24] C：获取本地时间
来源：http://wds.ivvv.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ycp.ydzc1.top

[S25] C：内存拷贝
来源：http://zij.xylfe.cn

memcpy(dst, src, n);
来源：http://psf.yfazqb.com

[S26] C：内存清零
来源：http://ifk.ywan-chungtsiang.top

memset(a, 0, sizeof a);
来源：http://ouh.fktsv.cn

[S27] C：定义常量
来源：http://oam.dashuyun.cn

const double PI = 3.14159;
来源：http://rio.hysaishi.cn

[S28] C：静态变量
来源：http://gnp.cqqwz.cn

static int counter = 0;
来源：http://qpy.ydzc1.top

[S29] C：变参函数
来源：http://pic.c1oappe.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pwv.jiagoushi.top

[S30] C：头文件保护
来源：http://sbp.andypj.xyz

#ifndef X_H
来源：http://ums.tanke756.top

#define X_H
来源：http://ddf.sysykeji.top

#endif
来源：http://cck.52xcode.cn

[S31] C++：Hello World
来源：http://kli.52xcode.cn

#include <iostream>
来源：http://kry.9152youxi.cn

int main() { std::cout << "Hello\n"; }
来源：http://fjm.nanxinkj.top

[S32] C++：字符串
来源：http://bpn.yuxming.cn

std::string s = "hi";  s += "!";
来源：http://rqf.hfpthk.cn

[S33] C++：vector 增删
来源：http://yym.iojbl.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://onu.zycfv.cn

[S34] C++：遍历 vector
来源：http://owc.yonumen.top

for (auto &x : v) { std::cout << x; }
来源：http://cqk.wangdashe.top

[S35] C++：map
来源：http://aac.tarul.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://miy.xziqi.cn

[S36] C++：unordered_map
来源：http://vjy.ydjk.org.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zol.feifeiyinyue.top

[S37] C++：set
来源：http://ety.jiagoushi.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uzv.andypj.xyz

[S38] C++：排序
来源：http://nxq.cheryme.top

std::sort(v.begin(), v.end());
来源：http://dbh.vehdjk.com

[S39] C++：自定义比较器排序
来源：http://bmh.tanke756.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tpg.dashuyun.cn

[S40] C++：查找元素
来源：http://nek.shanyushiyangtech.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sdq.gotoacloud.top

[S41] C++：类与构造函数
来源：http://mdy.sufxvd.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://alh.chenzaomai.com

[S42] C++：继承与虚函数
来源：http://xna.ydzc1.top

class B : public Base { public: void f() override {} };
来源：http://hrp.jqgufenzy.top

[S43] C++：智能指针
来源：http://yar.yonumen.top

auto p = std::make_unique<int>(5);
来源：http://jbe.shzxlz.cn

[S44] C++：引用传参
来源：http://anz.hammf.cn

void inc(int &x) { ++x; }
来源：http://jdp.guowangkeji.top

[S45] C++：lambda
来源：http://que.ctjpmb.com

auto add = [](int a, int b) { return a + b; };
来源：http://cas.quarkkingdee.top

[S46] C++：函数模板
来源：http://wdb.daria6918.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xfp.hywenlv.cn

[S47] C++：结构化绑定遍历
来源：http://har.xziqi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uid.yj20258.top

[S48] C++：逐行读文件
来源：http://cba.sufxvd.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xyc.fanxiaobao.xyz

while (std::getline(in, line)) { }
来源：http://htk.epnwcf.com

[S49] C++：写文件
来源：http://prk.yfazqb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hen.daxiang520.top

[S50] C++：格式化数字
来源：http://qkh.havefunace.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kad.316326.xyz

[S51] C++：显式类型转换
来源：http://ldj.9152youxi.cn

static_cast<double>(a) / b
来源：http://nqo.316326.xyz

[S52] C++：const 与 noexcept
来源：http://pss.gogol.net.cn

int size() const noexcept { return n_; }
来源：http://oou.jianghu66.top

[S53] C++：移动语义
来源：http://nmo.shanyushiyangkeji.top

std::vector<int> w = std::move(v);
来源：http://yrm.haohaochexian.top

[S54] C++：异常处理
来源：http://uax.chenjidiqi.icu

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kle.shangyingyoupin.top

[S55] C++：结构化绑定
来源：http://scz.316326.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://hca.zhiwuduotai.top

[S56] C++：optional
来源：http://wvh.uphjek.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://atd.jqgfzy.top

[S57] C++：编译期常量
来源：http://ree.cashguo.top

constexpr int N = 10;
来源：http://bsd.ehwqpu.com

[S58] C++：命名空间
来源：http://jzh.snrcjt.cn

namespace ns { int f() { return 1; } }
来源：http://sdj.aizwys.cn

[S59] C++：静态断言
来源：http://svp.yonumen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://epw.ctjpmb.com

[S60] C++：遍历并删除元素
来源：http://ltj.jinghuilouyu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yfl.yongpay.top

================================================================================
来源：http://vto.shuidangran.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gie.ehwqpu.com

================================================================================
来源：http://uvq.fzhhl.top

[T01] Kotlin：Hello World
来源：http://qtr.gzhubu.top

println("Hello")
来源：http://imu.hnxiangtu.top

[T02] Kotlin：变量
来源：http://nxu.ctjpmb.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rtz.jiagoushi.top

[T03] Kotlin：字符串模板
来源：http://cup.pengpengdd.cyou

"值: $b"
来源：http://ehu.zhaomingkeji.xyz

[T04] Kotlin：空安全
来源：http://kfr.zdqjudy.top

val n: String? = null;  n?.length
来源：http://pcw.shzxlz.cn

[T05] Kotlin：when 表达式
来源：http://mzo.xinyue.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vjh.tanke756.top

[T06] Kotlin：集合映射
来源：http://lew.hcnkem.com

listOf(1, 2, 3).map { it * 2 }
来源：http://blx.zdbjq.cn

[T07] Kotlin：集合过滤
来源：http://lnv.yuxming.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ltv.jiagoushi.top

[T08] Kotlin：数据类
来源：http://syy.jlsjyb.cn

data class User(val name: String, val age: Int)
来源：http://xji.iojbl.cn

[T09] Kotlin：扩展函数
来源：http://gyy.cdnleiting.top

fun String.exclaim() = this + "!"
来源：http://zeb.tanke756.top

[T10] Kotlin：默认参数
来源：http://mbd.bjfxy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://zsz.bjfxy.top

[T11] Kotlin：协程
来源：http://vof.jinqigufen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://fxc.cashguo.top

[T12] Kotlin：解构声明
来源：http://goh.chenzaomai.com

val (a, b) = Pair(1, 2)
来源：http://kmx.guannengcc.top

[T13] Kotlin：只读 Map
来源：http://tbt.jyoumei.cn

val m = mapOf("a" to 1)
来源：http://jjn.xinyue.icu

[T14] Kotlin：循环
来源：http://hyd.hnxiangtu.top

for (i in 1..10) println(i)
来源：http://rzl.quarkkingdee.top

[T15] Kotlin：接口
来源：http://bzr.chenzaomai.com

interface Shape { fun area(): Double }
来源：http://qfy.vqdsnc.cn

[T16] Swift：Hello World
来源：http://xke.tanke756.top

print("Hello")
来源：http://ybe.gaohongyu789.top

[T17] Swift：变量与常量
来源：http://eaw.iojbl.cn

var a = 1;  let b = 2
来源：http://wqq.cdnleiting.top

[T18] Swift：字符串插值
来源：http://ezb.cashguo.top

"值: \(b)"
来源：http://uhc.vehdjk.com

[T19] Swift：可选绑定
来源：http://ons.iojbl.cn

if let n = opt { print(n) }
来源：http://xso.mhx1999.top

[T20] Swift：数组操作
来源：http://svq.vqdsnc.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vwy.chenzaomai.com

[T21] Swift：遍历
来源：http://lic.cdnleiting.top

for x in a { print(x) }
来源：http://knv.gzhubu.top

[T22] Swift：字典
来源：http://rii.pengpengdd.cyou

var d = ["a": 1];  d["b"] = 2
来源：http://pcr.tarul.cn

[T23] Swift：函数
来源：http://idh.hesvh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pzu.daria6918.cn

[T24] Swift：闭包
来源：http://zdw.hnqzz.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://jbk.jyoumei.cn

[T25] Swift：结构体
来源：http://xlc.tian-w.cn

struct P { var x: Int }
来源：http://ahj.haohaochexian.top

[T26] Swift：类与重写
来源：http://xdj.zhoulong.xyz

class A: Base { override func f() {} }
来源：http://fza.birdmap.top

[T27] Swift：错误处理
来源：http://bhc.ppjwa.cn

do { try f() } catch { print(error) }
来源：http://evm.nanxinkj.top

[T28] Swift：枚举
来源：http://yti.fengsongda.top

enum Color { case red, green }
来源：http://mjb.cucudq.cn

[T29] Swift：guard 提前返回
来源：http://njp.shanyushiyangtech.top

guard let x = opt else { return }
来源：http://xwr.daria6918.cn

[T30] Swift：协议
来源：http://kee.jiagoushi.top

protocol Shape { func area() -> Double }
来源：http://alx.jiagoushi.top

[T31] Lua：Hello World
来源：http://cnm.yvedp.cn

print("Hello")
来源：http://lci.meibo888.top

[T32] Lua：局部变量
来源：http://fqa.jinqigfzy.top

local a = 1
来源：http://myf.sxryk.cn

[T33] Lua：表（数组）
来源：http://msp.aizwys.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://iej.yuxming.cn

[T34] Lua：遍历表
来源：http://smt.hnxiangtu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://bkx.fktsv.cn

[T35] Lua：字典表
来源：http://pej.tianlin.xyz

local d = { a = 1 };  d.b = 2
来源：http://rvl.shanyushiyangkeji.top

[T36] Lua：函数
来源：http://mcg.pycfn.com

function add(a, b) return a + b end
来源：http://jqj.guannengcc.top

[T37] Lua：字符串拼接
来源：http://gkl.zhoulong.xyz

"a" .. "b"
来源：http://buj.316326.xyz

[T38] Lua：条件
来源：http://hmw.zhijiandao.cn

if x > 0 then print("正") end
来源：http://lcv.cdnleiting.top


<!-- 参考信息 -->