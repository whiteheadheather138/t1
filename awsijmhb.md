代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://mqx.meibo888.top

[R32] 参数个数校验
来源：http://jdg.sxryk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cox.kuanghao11.cn

[R33] 捕获错误并提示行号
来源：http://bdo.yongpay.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ubi.feifeiyinyue.top

[R34] 退出时清理
来源：http://zxe.cucudq.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tmg.andypj.xyz

[R35] 后台执行并等待
来源：http://fpt.birdmap.top

sleep 5 & pid=$!; wait "$pid"
来源：http://jey.cheryme.top

[R36] 并发执行多个任务
来源：http://xtc.feifeiyinyue.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dvu.yj202588.top

[R37] 把输出赋给变量
来源：http://mig.fehbvm.com

files=$(ls -1)
来源：http://bkj.ehwqpu.com

[R38] 管道串联
来源：http://vjr.daria6918.cn

cat a.txt | grep -i error | wc -l
来源：http://tbo.fzhhl.top

[R39] 重定向标准输出与错误
来源：http://rnu.yj202588.top

cmd > out.log 2>&1
来源：http://dlj.nwbrower.top

[R40] 追加写日志
来源：http://ynu.quarkkingdee.top

echo "log" >> out.log
来源：http://uez.jyoumei.cn

[R41] 丢弃输出
来源：http://kkf.hysaishi.cn

cmd >/dev/null 2>&1
来源：http://rfk.kuanghao11.cn

[R42] 输入重定向
来源：http://aop.zhengqikj.top

wc -l < a.txt
来源：http://ifv.jinyuanbaomall.cn

[R43] 按名字查找文件
来源：http://fkp.ctjpmb.com

find . -name "*.log" -type f
来源：http://miy.yj202588.top

[R44] 按修改时间查找
来源：http://sjv.daxiang520.top

find . -mtime -7 -type f
来源：http://dtf.wangdashe.top

[R45] 批量删除
来源：http://geu.shanyushiyangkeji.top

find . -name "*.tmp" -delete
来源：http://cgi.c1oappe.top

[R46] 递归替换文件内容
来源：http://btl.uphjek.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fnx.nwbrower.top

[R47] sed 单行替换
来源：http://hwq.yangfankeji.com

sed -i 's/foo/bar/g' a.txt
来源：http://zkh.guowangkeji.top

[R48] awk 取指定列
来源：http://wtl.yanxiufei.cn

awk '{print $1, $3}' a.txt
来源：http://ine.tianlin.xyz

[R49] awk 带条件
来源：http://wtp.fktsv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://icm.guannengcc.top

[R50] awk 求和
来源：http://mbv.fanxiaobao.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://ldi.iojbl.cn

[R51] 排序去重取前几
来源：http://aqh.meibo888.top

sort a.txt | uniq -c | sort -rn | head
来源：http://rlw.hnxiangtu.top

[R52] 统计行数
来源：http://pzx.yongpay.top

wc -l a.txt
来源：http://vzm.epnwcf.com

[R53] 查看文件头与实时尾
来源：http://vrg.chenjidiqi.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xkz.cdnleiting.top

[R54] 比较两个文件
来源：http://cop.yuanzhike.top

diff a.txt b.txt
来源：http://rxy.andypj.xyz

[R55] 压缩与解压
来源：http://dik.epnwcf.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ffq.shangyingyoupin.top

[R56] 远程拷贝
来源：http://lzy.quarkkingdee.top

scp file user@host:/path/
来源：http://qyi.hesvh.cn

[R57] 远程执行命令
来源：http://xnh.andypj.xyz

ssh user@host 'uptime'
来源：http://mlt.zhaomingkeji.xyz

[R58] 下载文件
来源：http://ldc.nanxinkj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ful.jlsjyb.cn

[R59] 发 POST JSON
来源：http://zbd.iojbl.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vlg.yongpay.top

[R60] 只看 HTTP 状态码
来源：http://jbo.svipenyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vxh.jyoumei.cn

[R61] 磁盘占用
来源：http://tli.yangfankeji.com

df -h;  du -sh *
来源：http://awf.snrcjt.cn

[R62] 找最占空间的文件
来源：http://ngi.gogol.net.cn

du -ah . | sort -rh | head -10
来源：http://gpy.fktsv.cn

[R63] 内存与进程
来源：http://qde.kuanghao11.cn

free -h;  ps aux | grep nginx
来源：http://vyi.dashuyun.cn

[R64] 结束进程
来源：http://pas.xuetiantiany.cn

kill -9 $(pgrep -f app.py)
来源：http://yip.andypj.xyz

[R65] 查看端口占用
来源：http://ujo.chenzaomai.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vkx.yj20258.top

[R66] 定时任务
来源：http://uge.guowangkeji.top

crontab -e;  crontab -l
来源：http://koa.birdmap.top

[R67] 生成随机十六进制串
来源：http://jlj.fehbvm.com

openssl rand -hex 16
来源：http://olf.meibo888.top

[R68] 计算文件校验值
来源：http://iaf.gaohongyu789.top

sha256sum a.txt;  md5sum a.txt
来源：http://cki.jqgfzy.top

[R69] 生成随机密码
来源：http://lyc.shanyushiyangtech.top

head -c 16 /dev/urandom | base64
来源：http://eik.yueranfly.top

[R70] 时间戳与互转
来源：http://qhw.xuanzx.com

date +%s;  date -d @1700000000
来源：http://fpb.zhijiandao.cn

[R71] 日期格式化
来源：http://bhi.haohaochexian.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://uzn.ctjpmb.com

[R72] 等待端口就绪
来源：http://ioe.yvedp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ydf.bjfxy.top

[R73] 分割大日志
来源：http://fdr.yfazqb.com

split -l 1000 big.log part_
来源：http://wwv.yangfankeji.com

[R74] 批量重命名
来源：http://xgf.yonumen.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xuv.mhx1999.top

[R75] 导出环境变量
来源：http://iip.sjlbkw.cn

export PATH="$HOME/bin:$PATH"
来源：http://uqb.jqgufenzy.top

[R76] 使用临时文件
来源：http://slk.yangfankeji.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vhe.tarul.cn

[R77] 读取用户输入
来源：http://tlq.pengpengdd.cyou

read -rp "请输入: " ans
来源：http://sab.hongshengwenyu.top

[R78] 交互式菜单
来源：http://xvi.ivvv.top

select opt in a b c; do echo "$opt"; break; done
来源：http://wnr.yj20258888.top

[R79] 解析命令行选项
来源：http://ign.guannengcc.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tfb.cheryme.top

[R80] 查看脚本执行耗时
来源：http://whu.sufxvd.cn

time ./run.sh
来源：http://nnc.shanyushiyangkeji.top

================================================================================
来源：http://yjn.0kj1m.cn

S. C / C++ 专题
来源：http://flb.fehbvm.com

================================================================================
来源：http://whx.pycfn.com

[S01] C：Hello World
来源：http://tjw.cqqwz.cn

#include <stdio.h>
来源：http://lez.zdqjudy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://swo.gogol.net.cn

[S02] C：变量与格式化输出
来源：http://jki.uphjek.com

int a = 10; printf("%d\n", a);
来源：http://cmk.mhx1999.top

[S03] C：读入整数
来源：http://tme.xylfe.cn

int x; scanf("%d", &x);
来源：http://ngz.fzhhl.top

[S04] C：字符串复制
来源：http://ouz.shuidangran.top

char dst[32]; strcpy(dst, "hi");
来源：http://hjh.sjlbkw.cn

[S05] C：字符串长度
来源：http://rnd.wangdashe.top

strlen(s)
来源：http://duj.yanxiufei.cn

[S06] C：字符串比较
来源：http://nib.jlsjyb.cn

strcmp(a, b) == 0
来源：http://muj.hcnkem.com

[S07] C：数组遍历求和
来源：http://fyt.xziqi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yhy.52xcode.cn

[S08] C：动态内存分配与释放
来源：http://vwn.xuetiantiany.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zrj.shzxlz.cn

[S09] C：结构体定义与初始化
来源：http://cyo.hywenlv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ahn.zhiwuduotai.top

[S10] C：指针与解引用
来源：http://dwv.hcnkem.com

int *p = &a;  *p = 5;
来源：http://bnf.vehdjk.com

[S11] C：逐行读文件
来源：http://yix.zhongyouzk.top

FILE *f = fopen("a.txt", "r");
来源：http://knh.jyoumei.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xah.fengsongda.top

fclose(f);
来源：http://cvi.52xcode.cn

[S12] C：写文件
来源：http://mcj.shuidangran.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xdz.chenjidiqi.icu

[S13] C：宏定义
来源：http://rho.shzxlz.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://voa.jinqigfzy.top

[S14] C：枚举
来源：http://jbp.zhixingplan.top

enum Color { RED, GREEN, BLUE };
来源：http://msd.zhoulong.xyz

[S15] C：类型转换
来源：http://kav.hysaishi.cn

(double) a / b
来源：http://yia.cqqwz.cn

[S16] C：位操作置位
来源：http://pgq.hammf.cn

x |= (1 << 3);
来源：http://zgy.mhx1999.top

[S17] C：安全拼接字符串
来源：http://bza.meibo888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rkw.tian-w.cn

[S18] C：命令行参数
来源：http://niz.xziqi.cn

int main(int argc, char **argv)
来源：http://mgw.gaohongyu789.top

[S19] C：快速排序
来源：http://zgk.ydzc1.top

qsort(a, n, sizeof(int), cmp);
来源：http://ebu.shanyushiyangtech.top

[S20] C：二分查找
来源：http://lbx.9152youxi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wxl.jianghu66.top

[S21] C：字符类别判断
来源：http://yrt.zhijiandao.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://exq.yonumen.top

[S22] C：字符串转数字
来源：http://vcm.svipenyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sqr.vehdjk.com

[S23] C：随机数
来源：http://lrt.zhaomingkeji.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://pvy.ydjk.org.cn

[S24] C：获取本地时间
来源：http://mxv.hnxiangtu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://opf.pengpengdd.cyou

[S25] C：内存拷贝
来源：http://xso.zhijiandao.cn

memcpy(dst, src, n);
来源：http://kqb.jinqigfzy.top

[S26] C：内存清零
来源：http://rds.mhx1999.top

memset(a, 0, sizeof a);
来源：http://adf.cucudq.cn

[S27] C：定义常量
来源：http://sxu.fengsongda.top

const double PI = 3.14159;
来源：http://czw.aibaodan.cn

[S28] C：静态变量
来源：http://cof.fanxiaobao.xyz

static int counter = 0;
来源：http://ncg.xziqi.cn

[S29] C：变参函数
来源：http://qyc.hysaishi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bvr.dashuyun.cn

[S30] C：头文件保护
来源：http://jff.aizwys.cn

#ifndef X_H
来源：http://mif.shangyingyoupin.top

#define X_H
来源：http://szv.xingfuxueyuan.xyz

#endif
来源：http://fbk.shzxlz.cn

[S31] C++：Hello World
来源：http://sgq.haohaochexian.top

#include <iostream>
来源：http://xaa.yueranfly.top

int main() { std::cout << "Hello\n"; }
来源：http://qyr.xingfuxueyuan.xyz

[S32] C++：字符串
来源：http://jmv.hammf.cn

std::string s = "hi";  s += "!";
来源：http://mcp.sxryk.cn

[S33] C++：vector 增删
来源：http://paz.hfpthk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://btc.vehdjk.com

[S34] C++：遍历 vector
来源：http://hmx.fktsv.cn

for (auto &x : v) { std::cout << x; }
来源：http://fzf.quarkkingdee.top

[S35] C++：map
来源：http://phc.jqgfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hhz.sweek.top

[S36] C++：unordered_map
来源：http://esc.fengsongda.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fje.uphjek.com

[S37] C++：set
来源：http://jfc.cashguo.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://noi.tianlin.xyz

[S38] C++：排序
来源：http://vzk.smart0.xyz

std::sort(v.begin(), v.end());
来源：http://zvq.nanxinkj.top

[S39] C++：自定义比较器排序
来源：http://ius.0kj1m.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hhe.zhixingplan.top

[S40] C++：查找元素
来源：http://xnd.yongpay.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xtl.redwolf501.top

[S41] C++：类与构造函数
来源：http://rnu.52xcode.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mjl.yangfankeji.com

[S42] C++：继承与虚函数
来源：http://yir.haohaochexian.top

class B : public Base { public: void f() override {} };
来源：http://jxl.fzhhl.top

[S43] C++：智能指针
来源：http://qln.yfazqb.com

auto p = std::make_unique<int>(5);
来源：http://gbv.vqdsnc.cn

[S44] C++：引用传参
来源：http://hfg.xinyue.icu

void inc(int &x) { ++x; }
来源：http://nzy.shanyushiyangtech.top

[S45] C++：lambda
来源：http://ybc.meibo888.top

auto add = [](int a, int b) { return a + b; };
来源：http://yop.yj20258888.top

[S46] C++：函数模板
来源：http://ryk.zdbjq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://aru.sweek.top

[S47] C++：结构化绑定遍历
来源：http://taa.jiagoushi.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pqe.zdqjudy.top

[S48] C++：逐行读文件
来源：http://rja.zdbjq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ast.sjlbkw.cn

while (std::getline(in, line)) { }
来源：http://zqt.guannengcc.top

[S49] C++：写文件
来源：http://rup.uphjek.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://aqf.yonumen.top

[S50] C++：格式化数字
来源：http://egg.fanxiaobao.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kme.yvedp.cn

[S51] C++：显式类型转换
来源：http://ckf.jqgufenzy.top

static_cast<double>(a) / b
来源：http://hkp.meibo888.top

[S52] C++：const 与 noexcept
来源：http://bkz.hammf.cn

int size() const noexcept { return n_; }
来源：http://dlr.nwbrower.top

[S53] C++：移动语义
来源：http://awv.cheryme.top

std::vector<int> w = std::move(v);
来源：http://jcu.shanyushiyangtech.top

[S54] C++：异常处理
来源：http://wdr.zhengqikj.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kwx.hammf.cn

[S55] C++：结构化绑定
来源：http://vny.zhijiandao.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lfe.hysaishi.cn

[S56] C++：optional
来源：http://oqd.aibaodan.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bvl.ctjpmb.com

[S57] C++：编译期常量
来源：http://mkr.yvedp.cn

constexpr int N = 10;
来源：http://qpn.snrcjt.cn

[S58] C++：命名空间
来源：http://hxc.ehwqpu.com

namespace ns { int f() { return 1; } }
来源：http://trj.jqgfzy.top

[S59] C++：静态断言
来源：http://drp.yonumen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pqh.nanxinkj.top

[S60] C++：遍历并删除元素
来源：http://zmf.sysykeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rsa.jinqigfzy.top

================================================================================
来源：http://qif.yj202588.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://opi.sxryk.cn

================================================================================
来源：http://ftw.ybcxt.top

[T01] Kotlin：Hello World
来源：http://sxf.wangdashe.top

println("Hello")
来源：http://fuw.yfazqb.com

[T02] Kotlin：变量
来源：http://yao.zdqjudy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://eex.zhaomingkeji.xyz

[T03] Kotlin：字符串模板
来源：http://fqh.wangshuangyany.cn

"值: $b"
来源：http://ugl.tianlin.xyz

[T04] Kotlin：空安全
来源：http://oav.tarul.cn

val n: String? = null;  n?.length
来源：http://jde.52xcode.cn

[T05] Kotlin：when 表达式
来源：http://nzx.sufxvd.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dcz.shangyingyoupin.top

[T06] Kotlin：集合映射
来源：http://zwp.sweek.top

listOf(1, 2, 3).map { it * 2 }
来源：http://kgo.jianghu66.top

[T07] Kotlin：集合过滤
来源：http://vtf.yongpay.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nkq.xuanzx.com

[T08] Kotlin：数据类
来源：http://ngu.cashguo.top

data class User(val name: String, val age: Int)
来源：http://bhs.pycfn.com

[T09] Kotlin：扩展函数
来源：http://dbq.smart0.xyz

fun String.exclaim() = this + "!"
来源：http://mcd.pengpengdd.cyou

[T10] Kotlin：默认参数
来源：http://qit.hammf.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cco.vehdjk.com

[T11] Kotlin：协程
来源：http://bkh.daria6918.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zda.yj20258.top

[T12] Kotlin：解构声明
来源：http://gaf.dashuyun.cn

val (a, b) = Pair(1, 2)
来源：http://bfx.shuidangran.top

[T13] Kotlin：只读 Map
来源：http://vop.yfazqb.com

val m = mapOf("a" to 1)
来源：http://xwj.birdmap.top

[T14] Kotlin：循环
来源：http://nmu.xuetiantiany.cn

for (i in 1..10) println(i)
来源：http://ycz.shuidangran.top

[T15] Kotlin：接口
来源：http://txa.yonumen.top

interface Shape { fun area(): Double }
来源：http://dcq.chenlongwang.top

[T16] Swift：Hello World
来源：http://glw.ywan-chungtsiang.top

print("Hello")
来源：http://mnz.sysykeji.top

[T17] Swift：变量与常量
来源：http://znr.daria6918.cn

var a = 1;  let b = 2
来源：http://fjm.jinghuilouyu.cn

[T18] Swift：字符串插值
来源：http://mqu.yj20258888.top

"值: \(b)"
来源：http://hkk.zdbjq.cn

[T19] Swift：可选绑定
来源：http://ojr.yj20258.top

if let n = opt { print(n) }
来源：http://iav.smart0.xyz

[T20] Swift：数组操作
来源：http://yeo.hnxiangtu.top

var a = [1, 2, 3];  a.append(4)
来源：http://sew.pycfn.com

[T21] Swift：遍历
来源：http://qcy.dianchejie.cn

for x in a { print(x) }
来源：http://fkt.tanke756.top

[T22] Swift：字典
来源：http://bsk.zdbjq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zjg.zhixingplan.top

[T23] Swift：函数
来源：http://cqi.shuidangran.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sdo.gotoacloud.top

[T24] Swift：闭包
来源：http://ozw.bbcook.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gvv.yuanzhike.top

[T25] Swift：结构体
来源：http://hmz.fengsongda.top

struct P { var x: Int }
来源：http://xph.shangyingyoupin.top

[T26] Swift：类与重写
来源：http://vvd.nanxinkj.top

class A: Base { override func f() {} }
来源：http://pct.52xcode.cn

[T27] Swift：错误处理
来源：http://gcb.yuxming.cn

do { try f() } catch { print(error) }
来源：http://sdg.epnwcf.com

[T28] Swift：枚举
来源：http://ntz.mhx1999.top

enum Color { case red, green }
来源：http://dav.xylfe.cn

[T29] Swift：guard 提前返回
来源：http://yhd.fanxiaobao.xyz

guard let x = opt else { return }
来源：http://rui.mhx1999.top

[T30] Swift：协议
来源：http://hmr.shzxlz.cn

protocol Shape { func area() -> Double }
来源：http://hva.cqqwz.cn

[T31] Lua：Hello World
来源：http://mry.zdbjq.cn

print("Hello")
来源：http://itw.pycfn.com

[T32] Lua：局部变量
来源：http://ujv.chenjidiqi.icu

local a = 1
来源：http://kxv.jiagoushi.top

[T33] Lua：表（数组）
来源：http://xwx.0kj1m.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cak.redwolf501.top

[T34] Lua：遍历表
来源：http://slm.wangdashe.top

for i, v in ipairs(t) do print(i, v) end
来源：http://xqq.zycfv.cn


<!-- 参考信息 -->