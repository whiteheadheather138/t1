代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://han.xylfe.cn

[R30] 函数返回状态码
来源：http://lib.zdbjq.cn

f() { return 0; }; f || echo "失败了"
来源：http://jqp.jianghu66.top

[R31] 局部变量
来源：http://zxl.tanke756.top

f() { local x=1; echo "$x"; }
来源：http://hix.tian-w.cn

[R32] 参数个数校验
来源：http://rya.dianchejie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iie.quarkkingdee.top

[R33] 捕获错误并提示行号
来源：http://ufm.yvedp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://isx.ehwqpu.com

[R34] 退出时清理
来源：http://mhn.chenzaomai.com

trap 'rm -f "$tmp"' EXIT
来源：http://und.jianghu66.top

[R35] 后台执行并等待
来源：http://wcs.sxryk.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wro.aizwys.cn

[R36] 并发执行多个任务
来源：http://iwd.fzhhl.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jjc.jyoumei.cn

[R37] 把输出赋给变量
来源：http://osr.shanyushiyangkeji.top

files=$(ls -1)
来源：http://qnu.xuanzx.com

[R38] 管道串联
来源：http://vbg.jiagoushi.top

cat a.txt | grep -i error | wc -l
来源：http://qby.fzhhl.top

[R39] 重定向标准输出与错误
来源：http://mcm.sjlbkw.cn

cmd > out.log 2>&1
来源：http://bjy.nanxuanxn.top

[R40] 追加写日志
来源：http://bfv.cqqwz.cn

echo "log" >> out.log
来源：http://buq.zycfv.cn

[R41] 丢弃输出
来源：http://ogc.shangyingyoupin.top

cmd >/dev/null 2>&1
来源：http://pjf.dianchejie.cn

[R42] 输入重定向
来源：http://kep.kuanghao11.cn

wc -l < a.txt
来源：http://lzd.ehwqpu.com

[R43] 按名字查找文件
来源：http://ien.ehwqpu.com

find . -name "*.log" -type f
来源：http://mar.sjlbkw.cn

[R44] 按修改时间查找
来源：http://gov.ppjwa.cn

find . -mtime -7 -type f
来源：http://sug.tarul.cn

[R45] 批量删除
来源：http://ufm.ehwqpu.com

find . -name "*.tmp" -delete
来源：http://zkv.gogol.net.cn

[R46] 递归替换文件内容
来源：http://fvw.zhongyouzk.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nhf.zdbjq.cn

[R47] sed 单行替换
来源：http://dcx.zycfv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xyy.shzxlz.cn

[R48] awk 取指定列
来源：http://pwo.xuanzx.com

awk '{print $1, $3}' a.txt
来源：http://tdh.tianlin.xyz

[R49] awk 带条件
来源：http://ytb.svipenyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jnx.sufxvd.cn

[R50] awk 求和
来源：http://wke.xylfe.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pld.zhengqikj.top

[R51] 排序去重取前几
来源：http://vah.xuanzx.com

sort a.txt | uniq -c | sort -rn | head
来源：http://hov.aibaodan.cn

[R52] 统计行数
来源：http://xqt.zdqjudy.top

wc -l a.txt
来源：http://kjr.svipenyu.cn

[R53] 查看文件头与实时尾
来源：http://ovl.hesvh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fkp.zhongyouzk.top

[R54] 比较两个文件
来源：http://buu.kuanghao11.cn

diff a.txt b.txt
来源：http://rpx.shanyushiyangkeji.top

[R55] 压缩与解压
来源：http://mvj.sweek.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://can.aizwys.cn

[R56] 远程拷贝
来源：http://oov.gaohongyu789.top

scp file user@host:/path/
来源：http://xep.zhoulong.xyz

[R57] 远程执行命令
来源：http://woi.chenlongwang.top

ssh user@host 'uptime'
来源：http://uuq.ehwqpu.com

[R58] 下载文件
来源：http://blz.c1oappe.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tic.gzhubu.top

[R59] 发 POST JSON
来源：http://hxn.guannengcc.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nlt.wangshuangyany.cn

[R60] 只看 HTTP 状态码
来源：http://uqj.fzhhl.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tcr.yj202588.top

[R61] 磁盘占用
来源：http://hbo.sjlbkw.cn

df -h;  du -sh *
来源：http://kzk.shanyushiyangtech.top

[R62] 找最占空间的文件
来源：http://uks.sufxvd.cn

du -ah . | sort -rh | head -10
来源：http://inh.yj20258888.top

[R63] 内存与进程
来源：http://nta.gzhubu.top

free -h;  ps aux | grep nginx
来源：http://bfv.hysaishi.cn

[R64] 结束进程
来源：http://bby.cdnleiting.top

kill -9 $(pgrep -f app.py)
来源：http://tvu.cashguo.top

[R65] 查看端口占用
来源：http://ymc.jqgufenzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://suo.redwolf501.top

[R66] 定时任务
来源：http://eip.jqgufenzy.top

crontab -e;  crontab -l
来源：http://ood.aizwys.cn

[R67] 生成随机十六进制串
来源：http://axp.cucudq.cn

openssl rand -hex 16
来源：http://igp.bbcook.cn

[R68] 计算文件校验值
来源：http://pam.wangshuangyany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fgj.fanxiaobao.xyz

[R69] 生成随机密码
来源：http://esa.hesvh.cn

head -c 16 /dev/urandom | base64
来源：http://tzr.zycfv.cn

[R70] 时间戳与互转
来源：http://iru.hammf.cn

date +%s;  date -d @1700000000
来源：http://btk.jyoumei.cn

[R71] 日期格式化
来源：http://rbh.hfpthk.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://erh.chenjidiqi.icu

[R72] 等待端口就绪
来源：http://xqs.zhiwuduotai.top

until nc -z localhost 3306; do sleep 1; done
来源：http://anj.daria6918.cn

[R73] 分割大日志
来源：http://mxk.chenlongwang.top

split -l 1000 big.log part_
来源：http://exn.shanyushiyangtech.top

[R74] 批量重命名
来源：http://yys.jinqigfzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jgv.cheryme.top

[R75] 导出环境变量
来源：http://xws.hnxiangtu.top

export PATH="$HOME/bin:$PATH"
来源：http://zvh.c1oappe.top

[R76] 使用临时文件
来源：http://csc.guowangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vex.chenzaomai.com

[R77] 读取用户输入
来源：http://pnx.yueranfly.top

read -rp "请输入: " ans
来源：http://ifq.xylfe.cn

[R78] 交互式菜单
来源：http://bcj.daxiang520.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ngq.yfazqb.com

[R79] 解析命令行选项
来源：http://hnt.gzhubu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cba.jinqigfzy.top

[R80] 查看脚本执行耗时
来源：http://kwy.chenlongwang.top

time ./run.sh
来源：http://buc.andypj.xyz

================================================================================
来源：http://oqc.meibo888.top

S. C / C++ 专题
来源：http://pgj.chenzaomai.com

================================================================================
来源：http://zdg.ydzc1.top

[S01] C：Hello World
来源：http://bgv.ywan-chungtsiang.top

#include <stdio.h>
来源：http://lbh.jiagoushi.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://urx.sjlbkw.cn

[S02] C：变量与格式化输出
来源：http://nvl.sweek.top

int a = 10; printf("%d\n", a);
来源：http://ynl.epnwcf.com

[S03] C：读入整数
来源：http://wbr.zdbjq.cn

int x; scanf("%d", &x);
来源：http://quv.nanxinkj.top

[S04] C：字符串复制
来源：http://tqy.jinyuanbaomall.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ngv.hammf.cn

[S05] C：字符串长度
来源：http://enx.316326.xyz

strlen(s)
来源：http://zbt.hesvh.cn

[S06] C：字符串比较
来源：http://zdp.ywan-chungtsiang.top

strcmp(a, b) == 0
来源：http://phd.aizwys.cn

[S07] C：数组遍历求和
来源：http://oqn.guannengcc.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uid.shanyushiyangtech.top

[S08] C：动态内存分配与释放
来源：http://mko.svipenyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dkh.bbcook.cn

[S09] C：结构体定义与初始化
来源：http://its.hywenlv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fol.xuanzx.com

[S10] C：指针与解引用
来源：http://zzg.jlsjyb.cn

int *p = &a;  *p = 5;
来源：http://msq.yj20258888.top

[S11] C：逐行读文件
来源：http://vjo.feifeiyinyue.top

FILE *f = fopen("a.txt", "r");
来源：http://owv.cqqwz.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bph.shangyingyoupin.top

fclose(f);
来源：http://ojq.jlsjyb.cn

[S12] C：写文件
来源：http://cdn.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qvg.cheryme.top

[S13] C：宏定义
来源：http://qnn.hammf.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bkl.iojbl.cn

[S14] C：枚举
来源：http://hiq.daria6918.cn

enum Color { RED, GREEN, BLUE };
来源：http://guz.fengsongda.top

[S15] C：类型转换
来源：http://vzi.yj20258888.top

(double) a / b
来源：http://fbp.ydjk.org.cn

[S16] C：位操作置位
来源：http://qcc.52xcode.cn

x |= (1 << 3);
来源：http://cpm.havefunace.top

[S17] C：安全拼接字符串
来源：http://jab.uphjek.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oxc.xuetiantiany.cn

[S18] C：命令行参数
来源：http://pwd.feifeiyinyue.top

int main(int argc, char **argv)
来源：http://ump.cdnleiting.top

[S19] C：快速排序
来源：http://idz.ywan-chungtsiang.top

qsort(a, n, sizeof(int), cmp);
来源：http://eil.hcnkem.com

[S20] C：二分查找
来源：http://gua.vqdsnc.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://crw.pengpengdd.cyou

[S21] C：字符类别判断
来源：http://dhy.svipenyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rde.yongpay.top

[S22] C：字符串转数字
来源：http://zdn.andypj.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://ygf.xuetiantiany.cn

[S23] C：随机数
来源：http://zhs.bbcook.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yqt.yfazqb.com

[S24] C：获取本地时间
来源：http://qsi.shuidangran.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wta.yj20258.top

[S25] C：内存拷贝
来源：http://qjv.wangdashe.top

memcpy(dst, src, n);
来源：http://shs.snrcjt.cn

[S26] C：内存清零
来源：http://pdi.mhx1999.top

memset(a, 0, sizeof a);
来源：http://hsm.yanxiufei.cn

[S27] C：定义常量
来源：http://beg.dianchejie.cn

const double PI = 3.14159;
来源：http://yla.jinghuilouyu.cn

[S28] C：静态变量
来源：http://ect.jiagoushi.top

static int counter = 0;
来源：http://ehd.nanxinkj.top

[S29] C：变参函数
来源：http://rsd.fktsv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hxi.sufxvd.cn

[S30] C：头文件保护
来源：http://iic.daxiang520.top

#ifndef X_H
来源：http://plg.zdbjq.cn

#define X_H
来源：http://gwj.yfazqb.com

#endif
来源：http://gpp.cheryme.top

[S31] C++：Hello World
来源：http://pqj.sxryk.cn

#include <iostream>
来源：http://qec.aizwys.cn

int main() { std::cout << "Hello\n"; }
来源：http://yyh.sufxvd.cn

[S32] C++：字符串
来源：http://byj.fktsv.cn

std::string s = "hi";  s += "!";
来源：http://yep.ydjk.org.cn

[S33] C++：vector 增删
来源：http://kwy.yj202588.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uda.shanyushiyangkeji.top

[S34] C++：遍历 vector
来源：http://hbq.iojbl.cn

for (auto &x : v) { std::cout << x; }
来源：http://jyn.iojbl.cn

[S35] C++：map
来源：http://abv.yueranfly.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xeh.yonumen.top

[S36] C++：unordered_map
来源：http://iwk.yuxming.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zfb.xylfe.cn

[S37] C++：set
来源：http://cuw.cashguo.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bgr.svipenyu.cn

[S38] C++：排序
来源：http://tly.yj202588.top

std::sort(v.begin(), v.end());
来源：http://ycx.gaohongyu789.top

[S39] C++：自定义比较器排序
来源：http://xup.shanyushiyangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://edi.sxryk.cn

[S40] C++：查找元素
来源：http://gtv.vehdjk.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zwj.sysykeji.top

[S41] C++：类与构造函数
来源：http://ylb.jinyuanbaomall.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vza.svipenyu.cn

[S42] C++：继承与虚函数
来源：http://owv.chenjidiqi.icu

class B : public Base { public: void f() override {} };
来源：http://wkw.vqdsnc.cn

[S43] C++：智能指针
来源：http://nom.ctjpmb.com

auto p = std::make_unique<int>(5);
来源：http://ylo.uphjek.com

[S44] C++：引用传参
来源：http://gzf.nanxinkj.top

void inc(int &x) { ++x; }
来源：http://lua.epnwcf.com

[S45] C++：lambda
来源：http://gja.jqgufenzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://fop.guannengcc.top

[S46] C++：函数模板
来源：http://qfe.gotoacloud.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ibn.cashguo.top

[S47] C++：结构化绑定遍历
来源：http://ymk.0kj1m.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uyf.yuxming.cn

[S48] C++：逐行读文件
来源：http://pio.cheryme.top

std::ifstream in("a.txt");  std::string line;
来源：http://xiy.gzhubu.top

while (std::getline(in, line)) { }
来源：http://tlb.jyoumei.cn

[S49] C++：写文件
来源：http://dnj.tian-w.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gik.daria6918.cn

[S50] C++：格式化数字
来源：http://kjv.chenjidiqi.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mvc.vehdjk.com

[S51] C++：显式类型转换
来源：http://fvx.gogol.net.cn

static_cast<double>(a) / b
来源：http://fcu.zhiwuduotai.top

[S52] C++：const 与 noexcept
来源：http://evw.yonumen.top

int size() const noexcept { return n_; }
来源：http://tco.smart0.xyz

[S53] C++：移动语义
来源：http://dod.havefunace.top

std::vector<int> w = std::move(v);
来源：http://aqv.jinqigufen.top

[S54] C++：异常处理
来源：http://hcs.9152youxi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pfo.zhongyouzk.top

[S55] C++：结构化绑定
来源：http://ogq.jyoumei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xwn.chenlongwang.top

[S56] C++：optional
来源：http://ncx.xylfe.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://joe.dianchejie.cn

[S57] C++：编译期常量
来源：http://emc.jinyuanbaomall.cn

constexpr int N = 10;
来源：http://ibr.shanyushiyangkeji.top

[S58] C++：命名空间
来源：http://obp.jiagoushi.top

namespace ns { int f() { return 1; } }
来源：http://kxd.tianlin.xyz

[S59] C++：静态断言
来源：http://xmf.hnxiangtu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jao.sweek.top

[S60] C++：遍历并删除元素
来源：http://uex.jianghu66.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://syj.yanxiufei.cn

================================================================================
来源：http://fot.yanxiufei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ngf.birdmap.top

================================================================================
来源：http://lse.snrcjt.cn

[T01] Kotlin：Hello World
来源：http://jwv.jqgufenzy.top

println("Hello")
来源：http://tir.aizwys.cn

[T02] Kotlin：变量
来源：http://zuh.birdmap.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qfk.redwolf501.top

[T03] Kotlin：字符串模板
来源：http://kvv.shanyushiyangtech.top

"值: $b"
来源：http://nih.tarul.cn

[T04] Kotlin：空安全
来源：http://fea.tarul.cn

val n: String? = null;  n?.length
来源：http://ytw.jinqigfzy.top

[T05] Kotlin：when 表达式
来源：http://fhb.gotoacloud.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ldn.fengsongda.top

[T06] Kotlin：集合映射
来源：http://mzs.daxiang520.top

listOf(1, 2, 3).map { it * 2 }
来源：http://xsi.daxiang520.top

[T07] Kotlin：集合过滤
来源：http://kkr.tarul.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://azr.52xcode.cn

[T08] Kotlin：数据类
来源：http://udb.52xcode.cn

data class User(val name: String, val age: Int)
来源：http://vyw.9152youxi.cn

[T09] Kotlin：扩展函数
来源：http://cyw.daria6918.cn

fun String.exclaim() = this + "!"
来源：http://mzg.chenzaomai.com

[T10] Kotlin：默认参数
来源：http://glq.c1oappe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://jfe.zhixingplan.top

[T11] Kotlin：协程
来源：http://how.ivvv.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://lwm.feifeiyinyue.top

[T12] Kotlin：解构声明
来源：http://uuc.chenzaomai.com

val (a, b) = Pair(1, 2)
来源：http://iex.gogol.net.cn

[T13] Kotlin：只读 Map
来源：http://ckk.c1oappe.top

val m = mapOf("a" to 1)
来源：http://gjk.yvedp.cn

[T14] Kotlin：循环
来源：http://vbl.sjlbkw.cn

for (i in 1..10) println(i)
来源：http://gwh.jianghu66.top

[T15] Kotlin：接口
来源：http://jro.shuidangran.top

interface Shape { fun area(): Double }
来源：http://lqp.guannengcc.top

[T16] Swift：Hello World
来源：http://jvz.sufxvd.cn

print("Hello")
来源：http://ecs.cheryme.top

[T17] Swift：变量与常量
来源：http://scl.gogol.net.cn

var a = 1;  let b = 2
来源：http://mgx.9152youxi.cn

[T18] Swift：字符串插值
来源：http://ctf.tarul.cn

"值: \(b)"
来源：http://hsh.quarkkingdee.top

[T19] Swift：可选绑定
来源：http://div.shzxlz.cn

if let n = opt { print(n) }
来源：http://gzi.yongpay.top

[T20] Swift：数组操作
来源：http://iwi.aizwys.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kov.aizwys.cn

[T21] Swift：遍历
来源：http://tqr.fehbvm.com

for x in a { print(x) }
来源：http://lss.jinghuilouyu.cn

[T22] Swift：字典
来源：http://ytz.svipenyu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jfz.cucudq.cn

[T23] Swift：函数
来源：http://qja.shanyushiyangkeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://byz.yonumen.top

[T24] Swift：闭包
来源：http://bru.hesvh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xwi.fktsv.cn

[T25] Swift：结构体
来源：http://czh.smart0.xyz

struct P { var x: Int }
来源：http://hny.52xcode.cn

[T26] Swift：类与重写
来源：http://uhr.xingfuxueyuan.xyz

class A: Base { override func f() {} }
来源：http://obi.pengpengdd.cyou

[T27] Swift：错误处理
来源：http://yqo.hongshengwenyu.top

do { try f() } catch { print(error) }
来源：http://mnl.mhx1999.top

[T28] Swift：枚举
来源：http://vbo.hnqzz.top

enum Color { case red, green }
来源：http://yff.bjfxy.top

[T29] Swift：guard 提前返回
来源：http://aqn.pycfn.com

guard let x = opt else { return }
来源：http://jhb.hnxiangtu.top

[T30] Swift：协议
来源：http://hfi.yfazqb.com

protocol Shape { func area() -> Double }
来源：http://pgf.hnxiangtu.top

[T31] Lua：Hello World
来源：http://efe.ybcxt.top

print("Hello")
来源：http://pxx.yj20258.top

[T32] Lua：局部变量
来源：http://dga.hammf.cn

local a = 1
来源：http://abi.shzxlz.cn


<!-- 参考信息 -->