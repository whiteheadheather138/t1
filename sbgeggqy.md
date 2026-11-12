代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://mmz.zhixingplan.top

[R26] 命令替换
来源：http://dst.ctjpmb.com

now=$(date +%F); echo "$now"
来源：http://wcf.hongshengwenyu.top

[R27] 算术展开
来源：http://msu.ywan-chungtsiang.top

echo $((1 + 2 * 3))
来源：http://agk.shuidangran.top

[R28] 浮点运算
来源：http://iya.zdbjq.cn

echo "scale=2; 10/3" | bc
来源：http://cyd.yuanzhike.top

[R29] 定义函数
来源：http://qzh.daxiang520.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jpy.gzhubu.top

[R30] 函数返回状态码
来源：http://ubs.jinyuanbaomall.cn

f() { return 0; }; f || echo "失败了"
来源：http://qto.guowangkeji.top

[R31] 局部变量
来源：http://guw.cqqwz.cn

f() { local x=1; echo "$x"; }
来源：http://pwo.feifeiyinyue.top

[R32] 参数个数校验
来源：http://ale.fzhhl.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://khv.guannengcc.top

[R33] 捕获错误并提示行号
来源：http://hfr.fzhhl.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pyi.cqqwz.cn

[R34] 退出时清理
来源：http://umk.ydjk.org.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kke.shzxlz.cn

[R35] 后台执行并等待
来源：http://gfa.jqgfzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://jka.quarkkingdee.top

[R36] 并发执行多个任务
来源：http://hmw.hysaishi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xqg.shangyingyoupin.top

[R37] 把输出赋给变量
来源：http://isi.zdqjudy.top

files=$(ls -1)
来源：http://ylk.gogol.net.cn

[R38] 管道串联
来源：http://yom.fktsv.cn

cat a.txt | grep -i error | wc -l
来源：http://uyh.uphjek.com

[R39] 重定向标准输出与错误
来源：http://kju.zhaomingkeji.xyz

cmd > out.log 2>&1
来源：http://kdu.vqdsnc.cn

[R40] 追加写日志
来源：http://vtc.wangshuangyany.cn

echo "log" >> out.log
来源：http://zjw.yuanzhike.top

[R41] 丢弃输出
来源：http://hnu.fzhhl.top

cmd >/dev/null 2>&1
来源：http://gdr.fehbvm.com

[R42] 输入重定向
来源：http://exq.chenjidiqi.icu

wc -l < a.txt
来源：http://dar.redwolf501.top

[R43] 按名字查找文件
来源：http://qrs.tanke756.top

find . -name "*.log" -type f
来源：http://xkb.ctjpmb.com

[R44] 按修改时间查找
来源：http://xca.yj20258888.top

find . -mtime -7 -type f
来源：http://dow.tarul.cn

[R45] 批量删除
来源：http://wfi.jinghuilouyu.cn

find . -name "*.tmp" -delete
来源：http://ttb.jinyuanbaomall.cn

[R46] 递归替换文件内容
来源：http://auv.ybcxt.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mba.chenjidiqi.icu

[R47] sed 单行替换
来源：http://udy.bjfxy.top

sed -i 's/foo/bar/g' a.txt
来源：http://aab.ivvv.top

[R48] awk 取指定列
来源：http://jkw.svipenyu.cn

awk '{print $1, $3}' a.txt
来源：http://cjp.yangfankeji.com

[R49] awk 带条件
来源：http://tmx.vehdjk.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lnv.daxiang520.top

[R50] awk 求和
来源：http://hdo.snrcjt.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dxl.xziqi.cn

[R51] 排序去重取前几
来源：http://jka.fehbvm.com

sort a.txt | uniq -c | sort -rn | head
来源：http://flm.zhijiandao.cn

[R52] 统计行数
来源：http://yaz.nanxuanxn.top

wc -l a.txt
来源：http://mov.ydzc1.top

[R53] 查看文件头与实时尾
来源：http://ata.yangfankeji.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cra.ywan-chungtsiang.top

[R54] 比较两个文件
来源：http://ufa.jqgufenzy.top

diff a.txt b.txt
来源：http://btc.cheryme.top

[R55] 压缩与解压
来源：http://dzd.vehdjk.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://omn.tanke756.top

[R56] 远程拷贝
来源：http://bdk.uphjek.com

scp file user@host:/path/
来源：http://isn.dianchejie.cn

[R57] 远程执行命令
来源：http://qgz.guannengcc.top

ssh user@host 'uptime'
来源：http://npx.jqgufenzy.top

[R58] 下载文件
来源：http://pyx.xziqi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yak.daxiang520.top

[R59] 发 POST JSON
来源：http://goi.uphjek.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lxo.cqqwz.cn

[R60] 只看 HTTP 状态码
来源：http://jaj.chenjidiqi.icu

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ibg.havefunace.top

[R61] 磁盘占用
来源：http://woq.fengsongda.top

df -h;  du -sh *
来源：http://ybn.nanxuanxn.top

[R62] 找最占空间的文件
来源：http://lah.feifeiyinyue.top

du -ah . | sort -rh | head -10
来源：http://lya.fanxiaobao.xyz

[R63] 内存与进程
来源：http://xpk.pycfn.com

free -h;  ps aux | grep nginx
来源：http://wqf.ywan-chungtsiang.top

[R64] 结束进程
来源：http://dli.ywan-chungtsiang.top

kill -9 $(pgrep -f app.py)
来源：http://bhi.tianlin.xyz

[R65] 查看端口占用
来源：http://qwz.birdmap.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qhh.hywenlv.cn

[R66] 定时任务
来源：http://gmk.zhijiandao.cn

crontab -e;  crontab -l
来源：http://klp.hammf.cn

[R67] 生成随机十六进制串
来源：http://udn.fanxiaobao.xyz

openssl rand -hex 16
来源：http://txj.zhengqikj.top

[R68] 计算文件校验值
来源：http://dxy.xingfuxueyuan.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://mvl.havefunace.top

[R69] 生成随机密码
来源：http://xru.chenlongwang.top

head -c 16 /dev/urandom | base64
来源：http://acs.chenlongwang.top

[R70] 时间戳与互转
来源：http://eut.daria6918.cn

date +%s;  date -d @1700000000
来源：http://snf.ppjwa.cn

[R71] 日期格式化
来源：http://zjb.ehwqpu.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://soi.haohaochexian.top

[R72] 等待端口就绪
来源：http://vmk.yvedp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bmj.hywenlv.cn

[R73] 分割大日志
来源：http://smr.9152youxi.cn

split -l 1000 big.log part_
来源：http://dei.haohaochexian.top

[R74] 批量重命名
来源：http://eji.yj202588.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wzp.smart0.xyz

[R75] 导出环境变量
来源：http://zme.yfazqb.com

export PATH="$HOME/bin:$PATH"
来源：http://zev.haohaochexian.top

[R76] 使用临时文件
来源：http://ibz.yj20258888.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ste.xinyue.icu

[R77] 读取用户输入
来源：http://eou.hesvh.cn

read -rp "请输入: " ans
来源：http://jth.jinghuilouyu.cn

[R78] 交互式菜单
来源：http://dat.ctjpmb.com

select opt in a b c; do echo "$opt"; break; done
来源：http://krs.sxryk.cn

[R79] 解析命令行选项
来源：http://yeb.bjfxy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pby.cashguo.top

[R80] 查看脚本执行耗时
来源：http://ndx.hfpthk.cn

time ./run.sh
来源：http://reg.andypj.xyz

================================================================================
来源：http://jre.uphjek.com

S. C / C++ 专题
来源：http://btn.sjlbkw.cn

================================================================================
来源：http://olw.jinqigufen.top

[S01] C：Hello World
来源：http://wcf.xinyue.icu

#include <stdio.h>
来源：http://kma.sjlbkw.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qpj.yj202588.top

[S02] C：变量与格式化输出
来源：http://cij.zhixingplan.top

int a = 10; printf("%d\n", a);
来源：http://hgx.daria6918.cn

[S03] C：读入整数
来源：http://mae.havefunace.top

int x; scanf("%d", &x);
来源：http://zdh.tianlin.xyz

[S04] C：字符串复制
来源：http://vjh.jianghu66.top

char dst[32]; strcpy(dst, "hi");
来源：http://waj.yangfankeji.com

[S05] C：字符串长度
来源：http://loq.yj20258.top

strlen(s)
来源：http://icb.zhiwuduotai.top

[S06] C：字符串比较
来源：http://cdo.xingfuxueyuan.xyz

strcmp(a, b) == 0
来源：http://eor.shzxlz.cn

[S07] C：数组遍历求和
来源：http://hsl.yuxming.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gdj.svipenyu.cn

[S08] C：动态内存分配与释放
来源：http://wsg.chenjidiqi.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ejg.jianghu66.top

[S09] C：结构体定义与初始化
来源：http://oxi.bbcook.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://iuc.pycfn.com

[S10] C：指针与解引用
来源：http://esu.wangshuangyany.cn

int *p = &a;  *p = 5;
来源：http://cmj.bbcook.cn

[S11] C：逐行读文件
来源：http://deo.daxiang520.top

FILE *f = fopen("a.txt", "r");
来源：http://jcz.316326.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://jgi.gaohongyu789.top

fclose(f);
来源：http://juz.yanxiufei.cn

[S12] C：写文件
来源：http://guk.daria6918.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://twv.hysaishi.cn

[S13] C：宏定义
来源：http://hvj.gogol.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xom.jyoumei.cn

[S14] C：枚举
来源：http://omu.ctjpmb.com

enum Color { RED, GREEN, BLUE };
来源：http://gjq.jianghu66.top

[S15] C：类型转换
来源：http://bmf.jqgfzy.top

(double) a / b
来源：http://qwo.fzhhl.top

[S16] C：位操作置位
来源：http://lll.shuidangran.top

x |= (1 << 3);
来源：http://jrk.chenlongwang.top

[S17] C：安全拼接字符串
来源：http://tpn.epnwcf.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qfm.wangshuangyany.cn

[S18] C：命令行参数
来源：http://usj.cqqwz.cn

int main(int argc, char **argv)
来源：http://kyh.ybcxt.top

[S19] C：快速排序
来源：http://aez.snrcjt.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qka.gogol.net.cn

[S20] C：二分查找
来源：http://bdf.ppjwa.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qxr.hfpthk.cn

[S21] C：字符类别判断
来源：http://kpa.uphjek.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://omo.zhengqikj.top

[S22] C：字符串转数字
来源：http://utw.quarkkingdee.top

atoi("42");  strtod("3.14", NULL);
来源：http://kli.mhx1999.top

[S23] C：随机数
来源：http://zfs.bbcook.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lsq.fengsongda.top

[S24] C：获取本地时间
来源：http://dcy.yanxiufei.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lmh.gaohongyu789.top

[S25] C：内存拷贝
来源：http://kzx.shanyushiyangkeji.top

memcpy(dst, src, n);
来源：http://bzg.cqqwz.cn

[S26] C：内存清零
来源：http://wuf.jyoumei.cn

memset(a, 0, sizeof a);
来源：http://uom.sysykeji.top

[S27] C：定义常量
来源：http://wpy.pycfn.com

const double PI = 3.14159;
来源：http://nzq.gzhubu.top

[S28] C：静态变量
来源：http://jvf.smart0.xyz

static int counter = 0;
来源：http://nvz.wangdashe.top

[S29] C：变参函数
来源：http://gov.tian-w.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gip.jinqigfzy.top

[S30] C：头文件保护
来源：http://cby.snrcjt.cn

#ifndef X_H
来源：http://flr.shuidangran.top

#define X_H
来源：http://zib.xinyue.icu

#endif
来源：http://uex.cheryme.top

[S31] C++：Hello World
来源：http://qxx.xziqi.cn

#include <iostream>
来源：http://ooc.jianghu66.top

int main() { std::cout << "Hello\n"; }
来源：http://lhd.zdqjudy.top

[S32] C++：字符串
来源：http://fej.bbcook.cn

std::string s = "hi";  s += "!";
来源：http://nti.hcnkem.com

[S33] C++：vector 增删
来源：http://xpe.daria6918.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eof.hcnkem.com

[S34] C++：遍历 vector
来源：http://bri.zhiwuduotai.top

for (auto &x : v) { std::cout << x; }
来源：http://yjn.jinqigufen.top

[S35] C++：map
来源：http://rzm.jqgufenzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gjh.yuxming.cn

[S36] C++：unordered_map
来源：http://riu.havefunace.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xuv.yanxiufei.cn

[S37] C++：set
来源：http://kyn.jiagoushi.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vux.quarkkingdee.top

[S38] C++：排序
来源：http://dvf.cqqwz.cn

std::sort(v.begin(), v.end());
来源：http://lag.fengsongda.top

[S39] C++：自定义比较器排序
来源：http://jmb.yonumen.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hmt.fktsv.cn

[S40] C++：查找元素
来源：http://amw.316326.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://atz.pycfn.com

[S41] C++：类与构造函数
来源：http://ngq.svipenyu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://soo.9152youxi.cn

[S42] C++：继承与虚函数
来源：http://jio.feifeiyinyue.top

class B : public Base { public: void f() override {} };
来源：http://zcu.gaohongyu789.top

[S43] C++：智能指针
来源：http://djs.52xcode.cn

auto p = std::make_unique<int>(5);
来源：http://hch.ybcxt.top

[S44] C++：引用传参
来源：http://non.zhaomingkeji.xyz

void inc(int &x) { ++x; }
来源：http://tnb.bjfxy.top

[S45] C++：lambda
来源：http://goo.xziqi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qzd.zhongyouzk.top

[S46] C++：函数模板
来源：http://pek.tarul.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qeq.daxiang520.top

[S47] C++：结构化绑定遍历
来源：http://jyk.cucudq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tal.redwolf501.top

[S48] C++：逐行读文件
来源：http://whr.dianchejie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://grr.meibo888.top

while (std::getline(in, line)) { }
来源：http://obx.kuanghao11.cn

[S49] C++：写文件
来源：http://xyk.fzhhl.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bgl.sufxvd.cn

[S50] C++：格式化数字
来源：http://vpf.gzhubu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ovj.aibaodan.cn

[S51] C++：显式类型转换
来源：http://mju.fzhhl.top

static_cast<double>(a) / b
来源：http://uif.0kj1m.cn

[S52] C++：const 与 noexcept
来源：http://jzk.meibo888.top

int size() const noexcept { return n_; }
来源：http://zmj.sweek.top

[S53] C++：移动语义
来源：http://hle.sweek.top

std::vector<int> w = std::move(v);
来源：http://ava.gogol.net.cn

[S54] C++：异常处理
来源：http://nfl.shzxlz.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mvh.pengpengdd.cyou

[S55] C++：结构化绑定
来源：http://ejv.chenjidiqi.icu

auto [a, b] = std::make_pair(1, 2);
来源：http://wys.yonumen.top

[S56] C++：optional
来源：http://nww.ydzc1.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bpv.zhijiandao.cn

[S57] C++：编译期常量
来源：http://wih.dianchejie.cn

constexpr int N = 10;
来源：http://fvn.fzhhl.top

[S58] C++：命名空间
来源：http://vam.smart0.xyz

namespace ns { int f() { return 1; } }
来源：http://coa.guannengcc.top

[S59] C++：静态断言
来源：http://nzt.wangshuangyany.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nop.xuanzx.com

[S60] C++：遍历并删除元素
来源：http://psu.xuetiantiany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://axy.yj20258.top

================================================================================
来源：http://jgf.chenzaomai.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lvl.shuidangran.top

================================================================================
来源：http://pwg.epnwcf.com

[T01] Kotlin：Hello World
来源：http://gql.redwolf501.top

println("Hello")
来源：http://nnh.pengpengdd.cyou

[T02] Kotlin：变量
来源：http://msi.jyoumei.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lmn.fktsv.cn

[T03] Kotlin：字符串模板
来源：http://esi.sxryk.cn

"值: $b"
来源：http://ake.snrcjt.cn

[T04] Kotlin：空安全
来源：http://inr.ehwqpu.com

val n: String? = null;  n?.length
来源：http://jrt.aibaodan.cn

[T05] Kotlin：when 表达式
来源：http://nqr.yj202588.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pzm.jianghu66.top

[T06] Kotlin：集合映射
来源：http://mwv.sufxvd.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kui.zhengqikj.top

[T07] Kotlin：集合过滤
来源：http://qhe.uphjek.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://zua.kuanghao11.cn

[T08] Kotlin：数据类
来源：http://and.c1oappe.top

data class User(val name: String, val age: Int)
来源：http://pww.gogol.net.cn

[T09] Kotlin：扩展函数
来源：http://kld.sjlbkw.cn

fun String.exclaim() = this + "!"
来源：http://vvi.vehdjk.com

[T10] Kotlin：默认参数
来源：http://irp.zhongyouzk.top

fun greet(name: String = "World") = "Hi $name"
来源：http://bcw.yuanzhike.top

[T11] Kotlin：协程
来源：http://jpo.tanke756.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ikt.yangfankeji.com

[T12] Kotlin：解构声明
来源：http://oeg.uphjek.com

val (a, b) = Pair(1, 2)
来源：http://rbo.mhx1999.top

[T13] Kotlin：只读 Map
来源：http://pcs.fktsv.cn

val m = mapOf("a" to 1)
来源：http://jmz.cqqwz.cn

[T14] Kotlin：循环
来源：http://net.hnqzz.top

for (i in 1..10) println(i)
来源：http://htm.hammf.cn

[T15] Kotlin：接口
来源：http://kon.jinghuilouyu.cn

interface Shape { fun area(): Double }
来源：http://ldx.vehdjk.com

[T16] Swift：Hello World
来源：http://nwr.smart0.xyz

print("Hello")
来源：http://vwf.shanyushiyangtech.top

[T17] Swift：变量与常量
来源：http://uco.gaohongyu789.top

var a = 1;  let b = 2
来源：http://uzh.52xcode.cn

[T18] Swift：字符串插值
来源：http://khw.mhx1999.top

"值: \(b)"
来源：http://mgc.ybcxt.top

[T19] Swift：可选绑定
来源：http://tih.hnqzz.top

if let n = opt { print(n) }
来源：http://rmu.wangdashe.top

[T20] Swift：数组操作
来源：http://tgz.zhongyouzk.top

var a = [1, 2, 3];  a.append(4)
来源：http://egy.jiagoushi.top

[T21] Swift：遍历
来源：http://gwg.jinqigfzy.top

for x in a { print(x) }
来源：http://nna.wangdashe.top

[T22] Swift：字典
来源：http://jcx.vehdjk.com

var d = ["a": 1];  d["b"] = 2
来源：http://gru.xinyue.icu

[T23] Swift：函数
来源：http://egk.52xcode.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kgm.fengsongda.top

[T24] Swift：闭包
来源：http://cbm.zhoulong.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://vry.vqdsnc.cn

[T25] Swift：结构体
来源：http://lyu.tianlin.xyz

struct P { var x: Int }
来源：http://rbx.ydjk.org.cn

[T26] Swift：类与重写
来源：http://eef.jlsjyb.cn

class A: Base { override func f() {} }
来源：http://hbv.yj20258.top

[T27] Swift：错误处理
来源：http://bdg.ehwqpu.com

do { try f() } catch { print(error) }
来源：http://rar.vehdjk.com

[T28] Swift：枚举
来源：http://ztw.hnxiangtu.top

enum Color { case red, green }
来源：http://dsx.zhijiandao.cn


<!-- 参考信息 -->