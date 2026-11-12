代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://mqz.ctjpmb.com

[R26] 命令替换
来源：http://boj.jinyuanbaomall.cn

now=$(date +%F); echo "$now"
来源：http://fkh.jinqigfzy.top

[R27] 算术展开
来源：http://him.gogol.net.cn

echo $((1 + 2 * 3))
来源：http://tld.epnwcf.com

[R28] 浮点运算
来源：http://ffc.gotoacloud.top

echo "scale=2; 10/3" | bc
来源：http://twt.shangyingyoupin.top

[R29] 定义函数
来源：http://yik.shanyushiyangtech.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://geo.tarul.cn

[R30] 函数返回状态码
来源：http://jrf.zhengqikj.top

f() { return 0; }; f || echo "失败了"
来源：http://qwp.xuetiantiany.cn

[R31] 局部变量
来源：http://qvn.cucudq.cn

f() { local x=1; echo "$x"; }
来源：http://hpj.shuidangran.top

[R32] 参数个数校验
来源：http://nwh.sysykeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://igw.cheryme.top

[R33] 捕获错误并提示行号
来源：http://wdi.ctjpmb.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gzh.jinqigufen.top

[R34] 退出时清理
来源：http://bxi.guannengcc.top

trap 'rm -f "$tmp"' EXIT
来源：http://vma.meibo888.top

[R35] 后台执行并等待
来源：http://xan.xingfuxueyuan.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://one.jinqigfzy.top

[R36] 并发执行多个任务
来源：http://dxn.hongshengwenyu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://can.shzxlz.cn

[R37] 把输出赋给变量
来源：http://gnh.316326.xyz

files=$(ls -1)
来源：http://nfh.gaohongyu789.top

[R38] 管道串联
来源：http://rqu.yfazqb.com

cat a.txt | grep -i error | wc -l
来源：http://ktm.yongpay.top

[R39] 重定向标准输出与错误
来源：http://moy.jinqigufen.top

cmd > out.log 2>&1
来源：http://xcf.meibo888.top

[R40] 追加写日志
来源：http://hkt.yj20258.top

echo "log" >> out.log
来源：http://jlj.ctjpmb.com

[R41] 丢弃输出
来源：http://sbf.9152youxi.cn

cmd >/dev/null 2>&1
来源：http://cmo.hammf.cn

[R42] 输入重定向
来源：http://inb.cqqwz.cn

wc -l < a.txt
来源：http://xmg.xingfuxueyuan.xyz

[R43] 按名字查找文件
来源：http://kml.ywan-chungtsiang.top

find . -name "*.log" -type f
来源：http://rht.vqdsnc.cn

[R44] 按修改时间查找
来源：http://mgp.shuidangran.top

find . -mtime -7 -type f
来源：http://ojn.chenlongwang.top

[R45] 批量删除
来源：http://qfq.zhijiandao.cn

find . -name "*.tmp" -delete
来源：http://fky.shangyingyoupin.top

[R46] 递归替换文件内容
来源：http://duz.vehdjk.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qhe.vqdsnc.cn

[R47] sed 单行替换
来源：http://rom.c1oappe.top

sed -i 's/foo/bar/g' a.txt
来源：http://hfp.nanxinkj.top

[R48] awk 取指定列
来源：http://bbd.zhengqikj.top

awk '{print $1, $3}' a.txt
来源：http://bwv.yueranfly.top

[R49] awk 带条件
来源：http://ehe.yueranfly.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qmo.jiagoushi.top

[R50] awk 求和
来源：http://yob.snrcjt.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lie.hfpthk.cn

[R51] 排序去重取前几
来源：http://dnf.zhengqikj.top

sort a.txt | uniq -c | sort -rn | head
来源：http://vct.hysaishi.cn

[R52] 统计行数
来源：http://mzx.jinghuilouyu.cn

wc -l a.txt
来源：http://dfk.tanke756.top

[R53] 查看文件头与实时尾
来源：http://bkv.chenzaomai.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wwd.chenjidiqi.icu

[R54] 比较两个文件
来源：http://cpb.sjlbkw.cn

diff a.txt b.txt
来源：http://jmt.yangfankeji.com

[R55] 压缩与解压
来源：http://azy.hfpthk.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://srq.jlsjyb.cn

[R56] 远程拷贝
来源：http://lay.jqgufenzy.top

scp file user@host:/path/
来源：http://swt.kuanghao11.cn

[R57] 远程执行命令
来源：http://voc.vqdsnc.cn

ssh user@host 'uptime'
来源：http://bxs.yuanzhike.top

[R58] 下载文件
来源：http://qdb.cucudq.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bkg.gaohongyu789.top

[R59] 发 POST JSON
来源：http://owo.daxiang520.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sym.yvedp.cn

[R60] 只看 HTTP 状态码
来源：http://rtr.ywan-chungtsiang.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://udi.dashuyun.cn

[R61] 磁盘占用
来源：http://bgl.zycfv.cn

df -h;  du -sh *
来源：http://xxy.snrcjt.cn

[R62] 找最占空间的文件
来源：http://cpb.yangfankeji.com

du -ah . | sort -rh | head -10
来源：http://mih.wangshuangyany.cn

[R63] 内存与进程
来源：http://tvm.jiagoushi.top

free -h;  ps aux | grep nginx
来源：http://snv.jianghu66.top

[R64] 结束进程
来源：http://ipb.feifeiyinyue.top

kill -9 $(pgrep -f app.py)
来源：http://pve.gzhubu.top

[R65] 查看端口占用
来源：http://sbs.hongshengwenyu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fax.jiagoushi.top

[R66] 定时任务
来源：http://ujx.zdbjq.cn

crontab -e;  crontab -l
来源：http://nyt.snrcjt.cn

[R67] 生成随机十六进制串
来源：http://ryi.xziqi.cn

openssl rand -hex 16
来源：http://huz.bbcook.cn

[R68] 计算文件校验值
来源：http://kau.hywenlv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xpx.jyoumei.cn

[R69] 生成随机密码
来源：http://htu.uphjek.com

head -c 16 /dev/urandom | base64
来源：http://ato.316326.xyz

[R70] 时间戳与互转
来源：http://bpg.fanxiaobao.xyz

date +%s;  date -d @1700000000
来源：http://thq.xuetiantiany.cn

[R71] 日期格式化
来源：http://mkm.zhixingplan.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qor.pengpengdd.cyou

[R72] 等待端口就绪
来源：http://nlc.fehbvm.com

until nc -z localhost 3306; do sleep 1; done
来源：http://rpu.ehwqpu.com

[R73] 分割大日志
来源：http://pnu.tarul.cn

split -l 1000 big.log part_
来源：http://ijk.wangdashe.top

[R74] 批量重命名
来源：http://zdv.zhixingplan.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vry.yonumen.top

[R75] 导出环境变量
来源：http://xkn.c1oappe.top

export PATH="$HOME/bin:$PATH"
来源：http://qag.cashguo.top

[R76] 使用临时文件
来源：http://qtu.hcnkem.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://anq.sjlbkw.cn

[R77] 读取用户输入
来源：http://gdg.yj202588.top

read -rp "请输入: " ans
来源：http://nnb.gotoacloud.top

[R78] 交互式菜单
来源：http://jsj.quarkkingdee.top

select opt in a b c; do echo "$opt"; break; done
来源：http://oeq.fanxiaobao.xyz

[R79] 解析命令行选项
来源：http://bac.cheryme.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pzl.yvedp.cn

[R80] 查看脚本执行耗时
来源：http://mak.shangyingyoupin.top

time ./run.sh
来源：http://zgt.ydzc1.top

================================================================================
来源：http://jbs.vqdsnc.cn

S. C / C++ 专题
来源：http://lbq.0kj1m.cn

================================================================================
来源：http://bej.sufxvd.cn

[S01] C：Hello World
来源：http://qmr.ehwqpu.com

#include <stdio.h>
来源：http://hmh.tanke756.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ayz.iojbl.cn

[S02] C：变量与格式化输出
来源：http://osm.jinghuilouyu.cn

int a = 10; printf("%d\n", a);
来源：http://ywb.chenjidiqi.icu

[S03] C：读入整数
来源：http://gca.meibo888.top

int x; scanf("%d", &x);
来源：http://msm.ppjwa.cn

[S04] C：字符串复制
来源：http://lwh.jlsjyb.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tvn.meibo888.top

[S05] C：字符串长度
来源：http://noi.shanyushiyangtech.top

strlen(s)
来源：http://beq.ydzc1.top

[S06] C：字符串比较
来源：http://jxg.yj202588.top

strcmp(a, b) == 0
来源：http://btq.hnxiangtu.top

[S07] C：数组遍历求和
来源：http://ese.316326.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ctb.hnxiangtu.top

[S08] C：动态内存分配与释放
来源：http://pqp.daria6918.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eyw.birdmap.top

[S09] C：结构体定义与初始化
来源：http://idu.wangshuangyany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yuu.meibo888.top

[S10] C：指针与解引用
来源：http://khf.zycfv.cn

int *p = &a;  *p = 5;
来源：http://fge.zycfv.cn

[S11] C：逐行读文件
来源：http://bbe.gogol.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://ijt.jinqigufen.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://bsg.tarul.cn

fclose(f);
来源：http://gjx.xuetiantiany.cn

[S12] C：写文件
来源：http://vqg.chenlongwang.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ohr.chenzaomai.com

[S13] C：宏定义
来源：http://msv.jinyuanbaomall.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://utu.gotoacloud.top

[S14] C：枚举
来源：http://lvh.zycfv.cn

enum Color { RED, GREEN, BLUE };
来源：http://dvg.xziqi.cn

[S15] C：类型转换
来源：http://zkf.ppjwa.cn

(double) a / b
来源：http://fen.yfazqb.com

[S16] C：位操作置位
来源：http://eei.316326.xyz

x |= (1 << 3);
来源：http://jpk.fktsv.cn

[S17] C：安全拼接字符串
来源：http://hep.xingfuxueyuan.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jde.tianlin.xyz

[S18] C：命令行参数
来源：http://tie.zhongyouzk.top

int main(int argc, char **argv)
来源：http://ixz.quarkkingdee.top

[S19] C：快速排序
来源：http://hqt.cdnleiting.top

qsort(a, n, sizeof(int), cmp);
来源：http://jtl.cheryme.top

[S20] C：二分查找
来源：http://tlm.ybcxt.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cvq.bjfxy.top

[S21] C：字符类别判断
来源：http://duz.quarkkingdee.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jnw.jqgufenzy.top

[S22] C：字符串转数字
来源：http://vrt.yj20258888.top

atoi("42");  strtod("3.14", NULL);
来源：http://vlh.zhixingplan.top

[S23] C：随机数
来源：http://kqm.xinyue.icu

srand(time(NULL));  int r = rand() % 100;
来源：http://sez.xylfe.cn

[S24] C：获取本地时间
来源：http://lfz.jlsjyb.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://iph.cashguo.top

[S25] C：内存拷贝
来源：http://jgp.xuetiantiany.cn

memcpy(dst, src, n);
来源：http://xxc.gogol.net.cn

[S26] C：内存清零
来源：http://sss.cashguo.top

memset(a, 0, sizeof a);
来源：http://pdn.hongshengwenyu.top

[S27] C：定义常量
来源：http://ybf.zhijiandao.cn

const double PI = 3.14159;
来源：http://kmm.hammf.cn

[S28] C：静态变量
来源：http://hxj.quarkkingdee.top

static int counter = 0;
来源：http://mmo.sysykeji.top

[S29] C：变参函数
来源：http://fpg.sysykeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qrn.pengpengdd.cyou

[S30] C：头文件保护
来源：http://dcs.pycfn.com

#ifndef X_H
来源：http://jvz.fengsongda.top

#define X_H
来源：http://rmk.yj202588.top

#endif
来源：http://rdm.ybcxt.top

[S31] C++：Hello World
来源：http://soj.hesvh.cn

#include <iostream>
来源：http://hfg.iojbl.cn

int main() { std::cout << "Hello\n"; }
来源：http://muf.xuetiantiany.cn

[S32] C++：字符串
来源：http://qei.birdmap.top

std::string s = "hi";  s += "!";
来源：http://ssr.xuetiantiany.cn

[S33] C++：vector 增删
来源：http://efl.shangyingyoupin.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ict.ehwqpu.com

[S34] C++：遍历 vector
来源：http://mag.hywenlv.cn

for (auto &x : v) { std::cout << x; }
来源：http://spl.yongpay.top

[S35] C++：map
来源：http://hvy.nanxinkj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uvf.zhongyouzk.top

[S36] C++：unordered_map
来源：http://iee.zdqjudy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hyi.hysaishi.cn

[S37] C++：set
来源：http://fka.yfazqb.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pxh.fehbvm.com

[S38] C++：排序
来源：http://jxk.zhaomingkeji.xyz

std::sort(v.begin(), v.end());
来源：http://tnj.yfazqb.com

[S39] C++：自定义比较器排序
来源：http://zzw.ivvv.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gan.daria6918.cn

[S40] C++：查找元素
来源：http://qhe.ybcxt.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kfx.chenlongwang.top

[S41] C++：类与构造函数
来源：http://ugn.hesvh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fua.hywenlv.cn

[S42] C++：继承与虚函数
来源：http://bib.yj202588.top

class B : public Base { public: void f() override {} };
来源：http://zrp.wangshuangyany.cn

[S43] C++：智能指针
来源：http://ntb.ydzc1.top

auto p = std::make_unique<int>(5);
来源：http://ylw.vqdsnc.cn

[S44] C++：引用传参
来源：http://abz.52xcode.cn

void inc(int &x) { ++x; }
来源：http://snd.yfazqb.com

[S45] C++：lambda
来源：http://hil.zycfv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ywr.zhijiandao.cn

[S46] C++：函数模板
来源：http://dok.52xcode.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tfm.dianchejie.cn

[S47] C++：结构化绑定遍历
来源：http://fja.chenzaomai.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rxg.ydzc1.top

[S48] C++：逐行读文件
来源：http://puh.jinyuanbaomall.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ies.0kj1m.cn

while (std::getline(in, line)) { }
来源：http://rlx.cqqwz.cn

[S49] C++：写文件
来源：http://ooy.yonumen.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gwv.jianghu66.top

[S50] C++：格式化数字
来源：http://syd.yvedp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ahn.haohaochexian.top

[S51] C++：显式类型转换
来源：http://hza.jiagoushi.top

static_cast<double>(a) / b
来源：http://twm.hnqzz.top

[S52] C++：const 与 noexcept
来源：http://nvt.jinqigfzy.top

int size() const noexcept { return n_; }
来源：http://iyp.nanxinkj.top

[S53] C++：移动语义
来源：http://kmx.0kj1m.cn

std::vector<int> w = std::move(v);
来源：http://tuv.ehwqpu.com

[S54] C++：异常处理
来源：http://mjj.sysykeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xuz.hongshengwenyu.top

[S55] C++：结构化绑定
来源：http://wff.chenzaomai.com

auto [a, b] = std::make_pair(1, 2);
来源：http://qem.yj20258.top

[S56] C++：optional
来源：http://bzr.meibo888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pba.fehbvm.com

[S57] C++：编译期常量
来源：http://waw.yueranfly.top

constexpr int N = 10;
来源：http://csg.aizwys.cn

[S58] C++：命名空间
来源：http://ngm.haohaochexian.top

namespace ns { int f() { return 1; } }
来源：http://sdf.svipenyu.cn

[S59] C++：静态断言
来源：http://jnl.daria6918.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ctp.shanyushiyangkeji.top

[S60] C++：遍历并删除元素
来源：http://xwf.jinyuanbaomall.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://omr.zhaomingkeji.xyz

================================================================================
来源：http://pdg.haohaochexian.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nak.xinyue.icu

================================================================================
来源：http://dwq.shzxlz.cn

[T01] Kotlin：Hello World
来源：http://ncz.andypj.xyz

println("Hello")
来源：http://ixh.ywan-chungtsiang.top

[T02] Kotlin：变量
来源：http://cxl.sufxvd.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vkb.chenzaomai.com

[T03] Kotlin：字符串模板
来源：http://gqb.daria6918.cn

"值: $b"
来源：http://blg.hnqzz.top

[T04] Kotlin：空安全
来源：http://caw.ydjk.org.cn

val n: String? = null;  n?.length
来源：http://iit.jinyuanbaomall.cn

[T05] Kotlin：when 表达式
来源：http://lnf.mhx1999.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zsc.zhengqikj.top

[T06] Kotlin：集合映射
来源：http://uib.xuanzx.com

listOf(1, 2, 3).map { it * 2 }
来源：http://gtk.shanyushiyangtech.top

[T07] Kotlin：集合过滤
来源：http://srw.yfazqb.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://djr.mhx1999.top

[T08] Kotlin：数据类
来源：http://zhj.kuanghao11.cn

data class User(val name: String, val age: Int)
来源：http://sfp.zhongyouzk.top

[T09] Kotlin：扩展函数
来源：http://orv.jinqigufen.top

fun String.exclaim() = this + "!"
来源：http://sxr.fanxiaobao.xyz

[T10] Kotlin：默认参数
来源：http://tcr.iojbl.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xmd.birdmap.top

[T11] Kotlin：协程
来源：http://jvv.hesvh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vrl.jlsjyb.cn

[T12] Kotlin：解构声明
来源：http://ypp.bjfxy.top

val (a, b) = Pair(1, 2)
来源：http://cyq.zhijiandao.cn

[T13] Kotlin：只读 Map
来源：http://msg.kuanghao11.cn

val m = mapOf("a" to 1)
来源：http://vjk.epnwcf.com

[T14] Kotlin：循环
来源：http://glt.yongpay.top

for (i in 1..10) println(i)
来源：http://vlo.chenzaomai.com

[T15] Kotlin：接口
来源：http://btz.zhixingplan.top

interface Shape { fun area(): Double }
来源：http://tkq.52xcode.cn

[T16] Swift：Hello World
来源：http://awk.nanxinkj.top

print("Hello")
来源：http://qzr.jinqigufen.top

[T17] Swift：变量与常量
来源：http://nwz.gogol.net.cn

var a = 1;  let b = 2
来源：http://uzy.cheryme.top

[T18] Swift：字符串插值
来源：http://axe.fzhhl.top

"值: \(b)"
来源：http://erg.jinyuanbaomall.cn

[T19] Swift：可选绑定
来源：http://mcv.epnwcf.com

if let n = opt { print(n) }
来源：http://gjx.jinghuilouyu.cn

[T20] Swift：数组操作
来源：http://xqj.nanxinkj.top

var a = [1, 2, 3];  a.append(4)
来源：http://spl.mhx1999.top

[T21] Swift：遍历
来源：http://xqi.wangshuangyany.cn

for x in a { print(x) }
来源：http://juw.hnqzz.top

[T22] Swift：字典
来源：http://chc.quarkkingdee.top

var d = ["a": 1];  d["b"] = 2
来源：http://ghd.zhengqikj.top

[T23] Swift：函数
来源：http://vrg.yj20258.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pid.jinqigufen.top

[T24] Swift：闭包
来源：http://kks.snrcjt.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jzz.sufxvd.cn

[T25] Swift：结构体
来源：http://qvt.aizwys.cn

struct P { var x: Int }
来源：http://bgw.zhixingplan.top

[T26] Swift：类与重写
来源：http://dgk.xinyue.icu

class A: Base { override func f() {} }
来源：http://mmo.sysykeji.top

[T27] Swift：错误处理
来源：http://fjg.bbcook.cn

do { try f() } catch { print(error) }
来源：http://vmp.zdbjq.cn

[T28] Swift：枚举
来源：http://xld.xingfuxueyuan.xyz

enum Color { case red, green }
来源：http://ase.kuanghao11.cn


<!-- 参考信息 -->