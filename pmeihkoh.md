代发 wailian999

echo $((1 + 2 * 3))
来源：http://dwl.haohaochexian.top

[R28] 浮点运算
来源：http://bzq.xuetiantiany.cn

echo "scale=2; 10/3" | bc
来源：http://aet.ybcxt.top

[R29] 定义函数
来源：http://tvg.cheryme.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hdj.yuanzhike.top

[R30] 函数返回状态码
来源：http://upp.jinyuanbaomall.cn

f() { return 0; }; f || echo "失败了"
来源：http://sqa.yuxming.cn

[R31] 局部变量
来源：http://rof.yj20258888.top

f() { local x=1; echo "$x"; }
来源：http://bwb.yongpay.top

[R32] 参数个数校验
来源：http://kqx.52xcode.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jjk.jqgufenzy.top

[R33] 捕获错误并提示行号
来源：http://soa.0kj1m.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uca.hysaishi.cn

[R34] 退出时清理
来源：http://bhn.gzhubu.top

trap 'rm -f "$tmp"' EXIT
来源：http://enr.meibo888.top

[R35] 后台执行并等待
来源：http://kpq.tianlin.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://ffh.shanyushiyangtech.top

[R36] 并发执行多个任务
来源：http://pco.feifeiyinyue.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bpf.yj202588.top

[R37] 把输出赋给变量
来源：http://pff.jlsjyb.cn

files=$(ls -1)
来源：http://lsz.chenzaomai.com

[R38] 管道串联
来源：http://qdq.ctjpmb.com

cat a.txt | grep -i error | wc -l
来源：http://ofu.0kj1m.cn

[R39] 重定向标准输出与错误
来源：http://jnm.zhiwuduotai.top

cmd > out.log 2>&1
来源：http://qri.hysaishi.cn

[R40] 追加写日志
来源：http://izx.zhaomingkeji.xyz

echo "log" >> out.log
来源：http://ftz.gogol.net.cn

[R41] 丢弃输出
来源：http://pfc.ctjpmb.com

cmd >/dev/null 2>&1
来源：http://oav.havefunace.top

[R42] 输入重定向
来源：http://jem.cqqwz.cn

wc -l < a.txt
来源：http://nbq.cucudq.cn

[R43] 按名字查找文件
来源：http://gyp.ppjwa.cn

find . -name "*.log" -type f
来源：http://qgf.yj202588.top

[R44] 按修改时间查找
来源：http://hfz.jinghuilouyu.cn

find . -mtime -7 -type f
来源：http://ijf.aibaodan.cn

[R45] 批量删除
来源：http://erw.gotoacloud.top

find . -name "*.tmp" -delete
来源：http://bad.zhixingplan.top

[R46] 递归替换文件内容
来源：http://cxt.hammf.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uqr.sweek.top

[R47] sed 单行替换
来源：http://nqi.jinqigufen.top

sed -i 's/foo/bar/g' a.txt
来源：http://xix.tarul.cn

[R48] awk 取指定列
来源：http://uup.wangdashe.top

awk '{print $1, $3}' a.txt
来源：http://qcn.redwolf501.top

[R49] awk 带条件
来源：http://lvx.fanxiaobao.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tbv.wangdashe.top

[R50] awk 求和
来源：http://tub.kuanghao11.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xkp.daxiang520.top

[R51] 排序去重取前几
来源：http://asz.zhaomingkeji.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://ohw.jinyuanbaomall.cn

[R52] 统计行数
来源：http://att.sxryk.cn

wc -l a.txt
来源：http://fqh.tarul.cn

[R53] 查看文件头与实时尾
来源：http://gpv.yongpay.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nxw.zhijiandao.cn

[R54] 比较两个文件
来源：http://buv.gzhubu.top

diff a.txt b.txt
来源：http://ium.xziqi.cn

[R55] 压缩与解压
来源：http://uhs.gzhubu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hxr.cqqwz.cn

[R56] 远程拷贝
来源：http://hin.cqqwz.cn

scp file user@host:/path/
来源：http://pav.svipenyu.cn

[R57] 远程执行命令
来源：http://uhz.chenzaomai.com

ssh user@host 'uptime'
来源：http://qys.pengpengdd.cyou

[R58] 下载文件
来源：http://cwy.yueranfly.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pbx.hcnkem.com

[R59] 发 POST JSON
来源：http://rim.chenjidiqi.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ktg.jinqigufen.top

[R60] 只看 HTTP 状态码
来源：http://mqn.xingfuxueyuan.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kbh.hnqzz.top

[R61] 磁盘占用
来源：http://wjt.zhiwuduotai.top

df -h;  du -sh *
来源：http://dmx.shzxlz.cn

[R62] 找最占空间的文件
来源：http://zxh.zhoulong.xyz

du -ah . | sort -rh | head -10
来源：http://tuc.dashuyun.cn

[R63] 内存与进程
来源：http://csc.hywenlv.cn

free -h;  ps aux | grep nginx
来源：http://lgp.yonumen.top

[R64] 结束进程
来源：http://sly.zhengqikj.top

kill -9 $(pgrep -f app.py)
来源：http://koa.jiagoushi.top

[R65] 查看端口占用
来源：http://yjk.cashguo.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gmo.52xcode.cn

[R66] 定时任务
来源：http://cxd.snrcjt.cn

crontab -e;  crontab -l
来源：http://ehm.jinghuilouyu.cn

[R67] 生成随机十六进制串
来源：http://jyt.shanyushiyangkeji.top

openssl rand -hex 16
来源：http://dbf.jinqigufen.top

[R68] 计算文件校验值
来源：http://ajo.sufxvd.cn

sha256sum a.txt;  md5sum a.txt
来源：http://edy.haohaochexian.top

[R69] 生成随机密码
来源：http://vql.316326.xyz

head -c 16 /dev/urandom | base64
来源：http://emf.316326.xyz

[R70] 时间戳与互转
来源：http://gnx.jlsjyb.cn

date +%s;  date -d @1700000000
来源：http://olz.yj202588.top

[R71] 日期格式化
来源：http://twe.chenlongwang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vmy.xuetiantiany.cn

[R72] 等待端口就绪
来源：http://lsf.jqgfzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qdg.ywan-chungtsiang.top

[R73] 分割大日志
来源：http://qxl.jinghuilouyu.cn

split -l 1000 big.log part_
来源：http://sac.wangdashe.top

[R74] 批量重命名
来源：http://veb.ybcxt.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mnk.guowangkeji.top

[R75] 导出环境变量
来源：http://agt.zhiwuduotai.top

export PATH="$HOME/bin:$PATH"
来源：http://bre.fengsongda.top

[R76] 使用临时文件
来源：http://ywv.sxryk.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qko.jinghuilouyu.cn

[R77] 读取用户输入
来源：http://ypi.fengsongda.top

read -rp "请输入: " ans
来源：http://cwi.c1oappe.top

[R78] 交互式菜单
来源：http://wge.zdbjq.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dxu.dianchejie.cn

[R79] 解析命令行选项
来源：http://tqf.gaohongyu789.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ygi.yj20258888.top

[R80] 查看脚本执行耗时
来源：http://nou.cqqwz.cn

time ./run.sh
来源：http://ypv.tianlin.xyz

================================================================================
来源：http://ojl.smart0.xyz

S. C / C++ 专题
来源：http://csu.jlsjyb.cn

================================================================================
来源：http://pop.jinghuilouyu.cn

[S01] C：Hello World
来源：http://akp.zhiwuduotai.top

#include <stdio.h>
来源：http://axe.zhiwuduotai.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://zxq.yj20258.top

[S02] C：变量与格式化输出
来源：http://eyx.uphjek.com

int a = 10; printf("%d\n", a);
来源：http://wzu.pycfn.com

[S03] C：读入整数
来源：http://cvo.vqdsnc.cn

int x; scanf("%d", &x);
来源：http://rwk.zhoulong.xyz

[S04] C：字符串复制
来源：http://cpa.fktsv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://icq.jinqigfzy.top

[S05] C：字符串长度
来源：http://qwn.sufxvd.cn

strlen(s)
来源：http://faw.daria6918.cn

[S06] C：字符串比较
来源：http://aff.tanke756.top

strcmp(a, b) == 0
来源：http://sfy.yuanzhike.top

[S07] C：数组遍历求和
来源：http://umo.cqqwz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ama.smart0.xyz

[S08] C：动态内存分配与释放
来源：http://iwn.zhixingplan.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mdp.wangdashe.top

[S09] C：结构体定义与初始化
来源：http://swq.tarul.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lcp.cqqwz.cn

[S10] C：指针与解引用
来源：http://vcx.pycfn.com

int *p = &a;  *p = 5;
来源：http://rkt.dashuyun.cn

[S11] C：逐行读文件
来源：http://gdn.ywan-chungtsiang.top

FILE *f = fopen("a.txt", "r");
来源：http://qgg.aibaodan.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hgg.gaohongyu789.top

fclose(f);
来源：http://vaa.shanyushiyangtech.top

[S12] C：写文件
来源：http://kkn.zdbjq.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dhv.hnqzz.top

[S13] C：宏定义
来源：http://xyl.zhoulong.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bcf.chenjidiqi.icu

[S14] C：枚举
来源：http://vcz.jlsjyb.cn

enum Color { RED, GREEN, BLUE };
来源：http://zos.epnwcf.com

[S15] C：类型转换
来源：http://rtc.ywan-chungtsiang.top

(double) a / b
来源：http://pip.hcnkem.com

[S16] C：位操作置位
来源：http://rgw.gotoacloud.top

x |= (1 << 3);
来源：http://vts.9152youxi.cn

[S17] C：安全拼接字符串
来源：http://psx.jlsjyb.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ngm.uphjek.com

[S18] C：命令行参数
来源：http://dkn.fktsv.cn

int main(int argc, char **argv)
来源：http://axt.chenzaomai.com

[S19] C：快速排序
来源：http://ugm.xuanzx.com

qsort(a, n, sizeof(int), cmp);
来源：http://smn.chenzaomai.com

[S20] C：二分查找
来源：http://yte.chenlongwang.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kvt.tianlin.xyz

[S21] C：字符类别判断
来源：http://crw.mhx1999.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uoq.cqqwz.cn

[S22] C：字符串转数字
来源：http://cwy.yonumen.top

atoi("42");  strtod("3.14", NULL);
来源：http://kox.chenjidiqi.icu

[S23] C：随机数
来源：http://ymy.yj202588.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qey.shangyingyoupin.top

[S24] C：获取本地时间
来源：http://lms.jinqigfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ryc.feifeiyinyue.top

[S25] C：内存拷贝
来源：http://btm.jianghu66.top

memcpy(dst, src, n);
来源：http://iut.yanxiufei.cn

[S26] C：内存清零
来源：http://lcf.tianlin.xyz

memset(a, 0, sizeof a);
来源：http://rgk.fktsv.cn

[S27] C：定义常量
来源：http://tho.wangshuangyany.cn

const double PI = 3.14159;
来源：http://bgp.fanxiaobao.xyz

[S28] C：静态变量
来源：http://lrj.meibo888.top

static int counter = 0;
来源：http://brj.nanxuanxn.top

[S29] C：变参函数
来源：http://jgy.jianghu66.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eyr.0kj1m.cn

[S30] C：头文件保护
来源：http://rkb.shangyingyoupin.top

#ifndef X_H
来源：http://wxt.xylfe.cn

#define X_H
来源：http://mvz.chenjidiqi.icu

#endif
来源：http://mrt.jqgfzy.top

[S31] C++：Hello World
来源：http://zsr.hfpthk.cn

#include <iostream>
来源：http://vfu.tian-w.cn

int main() { std::cout << "Hello\n"; }
来源：http://zyx.hfpthk.cn

[S32] C++：字符串
来源：http://syg.shzxlz.cn

std::string s = "hi";  s += "!";
来源：http://wst.pengpengdd.cyou

[S33] C++：vector 增删
来源：http://fio.bbcook.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qoe.yueranfly.top

[S34] C++：遍历 vector
来源：http://ith.cdnleiting.top

for (auto &x : v) { std::cout << x; }
来源：http://zva.gogol.net.cn

[S35] C++：map
来源：http://lul.yj20258888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://frt.shzxlz.cn

[S36] C++：unordered_map
来源：http://pea.yangfankeji.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vjh.gotoacloud.top

[S37] C++：set
来源：http://uxs.mhx1999.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mkw.daria6918.cn

[S38] C++：排序
来源：http://fbq.cqqwz.cn

std::sort(v.begin(), v.end());
来源：http://pqa.svipenyu.cn

[S39] C++：自定义比较器排序
来源：http://pji.ehwqpu.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cfr.ivvv.top

[S40] C++：查找元素
来源：http://tpl.nwbrower.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wtw.fengsongda.top

[S41] C++：类与构造函数
来源：http://kpc.hnqzz.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://giu.fzhhl.top

[S42] C++：继承与虚函数
来源：http://nkc.shuidangran.top

class B : public Base { public: void f() override {} };
来源：http://zbg.tianlin.xyz

[S43] C++：智能指针
来源：http://hak.yuxming.cn

auto p = std::make_unique<int>(5);
来源：http://woh.svipenyu.cn

[S44] C++：引用传参
来源：http://bjt.ppjwa.cn

void inc(int &x) { ++x; }
来源：http://lvb.yonumen.top

[S45] C++：lambda
来源：http://bap.zdbjq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zxt.tian-w.cn

[S46] C++：函数模板
来源：http://rrd.yj202588.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://imm.fktsv.cn

[S47] C++：结构化绑定遍历
来源：http://slg.yj20258888.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qnl.gaohongyu789.top

[S48] C++：逐行读文件
来源：http://pct.yj20258888.top

std::ifstream in("a.txt");  std::string line;
来源：http://okn.vqdsnc.cn

while (std::getline(in, line)) { }
来源：http://hfx.cucudq.cn

[S49] C++：写文件
来源：http://byh.dianchejie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ezy.tarul.cn

[S50] C++：格式化数字
来源：http://fsr.vehdjk.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tcz.hnqzz.top

[S51] C++：显式类型转换
来源：http://fmj.52xcode.cn

static_cast<double>(a) / b
来源：http://xsa.tian-w.cn

[S52] C++：const 与 noexcept
来源：http://pkw.jlsjyb.cn

int size() const noexcept { return n_; }
来源：http://snk.ydzc1.top

[S53] C++：移动语义
来源：http://ras.iojbl.cn

std::vector<int> w = std::move(v);
来源：http://yef.iojbl.cn

[S54] C++：异常处理
来源：http://oli.c1oappe.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bem.uphjek.com

[S55] C++：结构化绑定
来源：http://cet.0kj1m.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rfh.aizwys.cn

[S56] C++：optional
来源：http://yqm.aizwys.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sho.wangshuangyany.cn

[S57] C++：编译期常量
来源：http://kfg.guannengcc.top

constexpr int N = 10;
来源：http://ree.hysaishi.cn

[S58] C++：命名空间
来源：http://dhe.pycfn.com

namespace ns { int f() { return 1; } }
来源：http://egp.xinyue.icu

[S59] C++：静态断言
来源：http://mlp.hysaishi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bay.ctjpmb.com

[S60] C++：遍历并删除元素
来源：http://bar.hysaishi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gbl.pycfn.com

================================================================================
来源：http://pla.nwbrower.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rjb.jlsjyb.cn

================================================================================
来源：http://ipk.hammf.cn

[T01] Kotlin：Hello World
来源：http://hbp.fzhhl.top

println("Hello")
来源：http://nyh.xingfuxueyuan.xyz

[T02] Kotlin：变量
来源：http://rmt.zhaomingkeji.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tbo.haohaochexian.top

[T03] Kotlin：字符串模板
来源：http://tbk.yangfankeji.com

"值: $b"
来源：http://wje.guowangkeji.top

[T04] Kotlin：空安全
来源：http://fuk.aibaodan.cn

val n: String? = null;  n?.length
来源：http://ztr.zdqjudy.top

[T05] Kotlin：when 表达式
来源：http://vso.smart0.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xfk.tarul.cn

[T06] Kotlin：集合映射
来源：http://kgd.sufxvd.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ciy.yanxiufei.cn

[T07] Kotlin：集合过滤
来源：http://tbu.havefunace.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://qbh.sxryk.cn

[T08] Kotlin：数据类
来源：http://add.zhoulong.xyz

data class User(val name: String, val age: Int)
来源：http://mbj.bbcook.cn

[T09] Kotlin：扩展函数
来源：http://nuy.316326.xyz

fun String.exclaim() = this + "!"
来源：http://uoz.iojbl.cn

[T10] Kotlin：默认参数
来源：http://gfk.yj202588.top

fun greet(name: String = "World") = "Hi $name"
来源：http://csx.fzhhl.top

[T11] Kotlin：协程
来源：http://pfi.fehbvm.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://eux.sufxvd.cn

[T12] Kotlin：解构声明
来源：http://mmj.fengsongda.top

val (a, b) = Pair(1, 2)
来源：http://eko.ehwqpu.com

[T13] Kotlin：只读 Map
来源：http://fcg.shzxlz.cn

val m = mapOf("a" to 1)
来源：http://grm.52xcode.cn

[T14] Kotlin：循环
来源：http://ald.jinqigufen.top

for (i in 1..10) println(i)
来源：http://gyh.hesvh.cn

[T15] Kotlin：接口
来源：http://hmh.vehdjk.com

interface Shape { fun area(): Double }
来源：http://beb.zhijiandao.cn

[T16] Swift：Hello World
来源：http://aax.ydzc1.top

print("Hello")
来源：http://lmi.ppjwa.cn

[T17] Swift：变量与常量
来源：http://ypv.316326.xyz

var a = 1;  let b = 2
来源：http://bvr.bjfxy.top

[T18] Swift：字符串插值
来源：http://vgg.ydjk.org.cn

"值: \(b)"
来源：http://vsi.zdqjudy.top

[T19] Swift：可选绑定
来源：http://nrt.shzxlz.cn

if let n = opt { print(n) }
来源：http://eoa.ydzc1.top

[T20] Swift：数组操作
来源：http://zkb.xuetiantiany.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vaw.sufxvd.cn

[T21] Swift：遍历
来源：http://pre.jyoumei.cn

for x in a { print(x) }
来源：http://wje.bbcook.cn

[T22] Swift：字典
来源：http://its.jlsjyb.cn

var d = ["a": 1];  d["b"] = 2
来源：http://luf.nwbrower.top

[T23] Swift：函数
来源：http://mio.fzhhl.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dwm.andypj.xyz

[T24] Swift：闭包
来源：http://fwu.yj20258888.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://uyp.jinqigufen.top

[T25] Swift：结构体
来源：http://xqf.wangdashe.top

struct P { var x: Int }
来源：http://fju.tarul.cn

[T26] Swift：类与重写
来源：http://nxe.dashuyun.cn

class A: Base { override func f() {} }
来源：http://hvo.meibo888.top

[T27] Swift：错误处理
来源：http://pyy.ydzc1.top

do { try f() } catch { print(error) }
来源：http://uqq.xingfuxueyuan.xyz

[T28] Swift：枚举
来源：http://smp.daria6918.cn

enum Color { case red, green }
来源：http://iez.andypj.xyz

[T29] Swift：guard 提前返回
来源：http://qxs.gzhubu.top

guard let x = opt else { return }
来源：http://kvr.ppjwa.cn

[T30] Swift：协议
来源：http://wkg.fzhhl.top

protocol Shape { func area() -> Double }
来源：http://ikj.zhoulong.xyz


<!-- 参考信息 -->