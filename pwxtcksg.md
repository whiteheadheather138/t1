代发 wailian999

files=$(ls -1)
来源：http://cye.yfazqb.com

[R38] 管道串联
来源：http://siz.tianlin.xyz

cat a.txt | grep -i error | wc -l
来源：http://dpl.9152youxi.cn

[R39] 重定向标准输出与错误
来源：http://rvh.sufxvd.cn

cmd > out.log 2>&1
来源：http://qqe.yvedp.cn

[R40] 追加写日志
来源：http://isg.ydzc1.top

echo "log" >> out.log
来源：http://pad.yvedp.cn

[R41] 丢弃输出
来源：http://ytr.bbcook.cn

cmd >/dev/null 2>&1
来源：http://qfx.hesvh.cn

[R42] 输入重定向
来源：http://xfp.ivvv.top

wc -l < a.txt
来源：http://uva.ctjpmb.com

[R43] 按名字查找文件
来源：http://gnu.ehwqpu.com

find . -name "*.log" -type f
来源：http://dqf.bjfxy.top

[R44] 按修改时间查找
来源：http://uzx.nwbrower.top

find . -mtime -7 -type f
来源：http://vxq.hesvh.cn

[R45] 批量删除
来源：http://tcs.cdnleiting.top

find . -name "*.tmp" -delete
来源：http://gmc.hcnkem.com

[R46] 递归替换文件内容
来源：http://gij.hysaishi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tpr.haohaochexian.top

[R47] sed 单行替换
来源：http://jjr.chenjidiqi.icu

sed -i 's/foo/bar/g' a.txt
来源：http://zwg.aizwys.cn

[R48] awk 取指定列
来源：http://vgh.yonumen.top

awk '{print $1, $3}' a.txt
来源：http://mpg.sufxvd.cn

[R49] awk 带条件
来源：http://hzo.cucudq.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pyx.jinghuilouyu.cn

[R50] awk 求和
来源：http://nll.hammf.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nuf.shangyingyoupin.top

[R51] 排序去重取前几
来源：http://mmp.sufxvd.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fhz.chenjidiqi.icu

[R52] 统计行数
来源：http://dev.sjlbkw.cn

wc -l a.txt
来源：http://khj.yueranfly.top

[R53] 查看文件头与实时尾
来源：http://wrg.quarkkingdee.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xlz.tian-w.cn

[R54] 比较两个文件
来源：http://oqp.jianghu66.top

diff a.txt b.txt
来源：http://bgt.hysaishi.cn

[R55] 压缩与解压
来源：http://kyb.tianlin.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://klq.jlsjyb.cn

[R56] 远程拷贝
来源：http://gxx.zhijiandao.cn

scp file user@host:/path/
来源：http://nxs.yuxming.cn

[R57] 远程执行命令
来源：http://dqd.0kj1m.cn

ssh user@host 'uptime'
来源：http://imw.pycfn.com

[R58] 下载文件
来源：http://mxu.epnwcf.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ugr.zhixingplan.top

[R59] 发 POST JSON
来源：http://fdj.yongpay.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qnt.andypj.xyz

[R60] 只看 HTTP 状态码
来源：http://ety.xylfe.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qqf.jinqigufen.top

[R61] 磁盘占用
来源：http://wmj.ctjpmb.com

df -h;  du -sh *
来源：http://zki.hcnkem.com

[R62] 找最占空间的文件
来源：http://ylt.xuetiantiany.cn

du -ah . | sort -rh | head -10
来源：http://hlk.ydzc1.top

[R63] 内存与进程
来源：http://sic.birdmap.top

free -h;  ps aux | grep nginx
来源：http://bzx.gotoacloud.top

[R64] 结束进程
来源：http://fjm.hnxiangtu.top

kill -9 $(pgrep -f app.py)
来源：http://bsv.chenjidiqi.icu

[R65] 查看端口占用
来源：http://rpr.cucudq.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wvj.yuanzhike.top

[R66] 定时任务
来源：http://glx.vqdsnc.cn

crontab -e;  crontab -l
来源：http://fgr.daria6918.cn

[R67] 生成随机十六进制串
来源：http://lnr.mhx1999.top

openssl rand -hex 16
来源：http://vzp.vqdsnc.cn

[R68] 计算文件校验值
来源：http://kis.nwbrower.top

sha256sum a.txt;  md5sum a.txt
来源：http://qds.jqgufenzy.top

[R69] 生成随机密码
来源：http://nzc.zhoulong.xyz

head -c 16 /dev/urandom | base64
来源：http://wcu.bbcook.cn

[R70] 时间戳与互转
来源：http://oht.yongpay.top

date +%s;  date -d @1700000000
来源：http://uuq.hywenlv.cn

[R71] 日期格式化
来源：http://knq.dianchejie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://usp.chenzaomai.com

[R72] 等待端口就绪
来源：http://qci.yuanzhike.top

until nc -z localhost 3306; do sleep 1; done
来源：http://hnk.316326.xyz

[R73] 分割大日志
来源：http://mvj.ydzc1.top

split -l 1000 big.log part_
来源：http://suf.kuanghao11.cn

[R74] 批量重命名
来源：http://owm.nanxuanxn.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qms.hywenlv.cn

[R75] 导出环境变量
来源：http://zuk.nanxinkj.top

export PATH="$HOME/bin:$PATH"
来源：http://gir.shzxlz.cn

[R76] 使用临时文件
来源：http://pkh.havefunace.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://epi.cdnleiting.top

[R77] 读取用户输入
来源：http://rdq.gzhubu.top

read -rp "请输入: " ans
来源：http://thd.dashuyun.cn

[R78] 交互式菜单
来源：http://xut.guowangkeji.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ugc.chenlongwang.top

[R79] 解析命令行选项
来源：http://ync.52xcode.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rbf.snrcjt.cn

[R80] 查看脚本执行耗时
来源：http://dzr.hysaishi.cn

time ./run.sh
来源：http://tcn.hnqzz.top

================================================================================
来源：http://jpk.zycfv.cn

S. C / C++ 专题
来源：http://dqv.zdqjudy.top

================================================================================
来源：http://yeb.redwolf501.top

[S01] C：Hello World
来源：http://ohy.dianchejie.cn

#include <stdio.h>
来源：http://rhv.tianlin.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://lzg.hfpthk.cn

[S02] C：变量与格式化输出
来源：http://fwu.9152youxi.cn

int a = 10; printf("%d\n", a);
来源：http://iql.havefunace.top

[S03] C：读入整数
来源：http://emz.yuxming.cn

int x; scanf("%d", &x);
来源：http://ndc.aizwys.cn

[S04] C：字符串复制
来源：http://lhv.fengsongda.top

char dst[32]; strcpy(dst, "hi");
来源：http://ccl.yongpay.top

[S05] C：字符串长度
来源：http://uht.meibo888.top

strlen(s)
来源：http://idt.ctjpmb.com

[S06] C：字符串比较
来源：http://cqj.sweek.top

strcmp(a, b) == 0
来源：http://lru.jqgfzy.top

[S07] C：数组遍历求和
来源：http://tsj.gzhubu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kmb.jqgfzy.top

[S08] C：动态内存分配与释放
来源：http://akp.daria6918.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nqs.0kj1m.cn

[S09] C：结构体定义与初始化
来源：http://lbo.xylfe.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lcz.guannengcc.top

[S10] C：指针与解引用
来源：http://kly.aizwys.cn

int *p = &a;  *p = 5;
来源：http://ael.yonumen.top

[S11] C：逐行读文件
来源：http://naa.jinqigfzy.top

FILE *f = fopen("a.txt", "r");
来源：http://tqi.hnqzz.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://hpj.zhongyouzk.top

fclose(f);
来源：http://sqo.hywenlv.cn

[S12] C：写文件
来源：http://ibt.guannengcc.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rur.shuidangran.top

[S13] C：宏定义
来源：http://jrj.xingfuxueyuan.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wey.vehdjk.com

[S14] C：枚举
来源：http://agr.yanxiufei.cn

enum Color { RED, GREEN, BLUE };
来源：http://xvb.zhengqikj.top

[S15] C：类型转换
来源：http://tmh.ehwqpu.com

(double) a / b
来源：http://mse.tanke756.top

[S16] C：位操作置位
来源：http://lpk.vehdjk.com

x |= (1 << 3);
来源：http://hpa.sysykeji.top

[S17] C：安全拼接字符串
来源：http://vxn.xingfuxueyuan.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://iin.daxiang520.top

[S18] C：命令行参数
来源：http://nig.meibo888.top

int main(int argc, char **argv)
来源：http://ccd.jyoumei.cn

[S19] C：快速排序
来源：http://sgt.zhijiandao.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tpg.cucudq.cn

[S20] C：二分查找
来源：http://jta.9152youxi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zim.sysykeji.top

[S21] C：字符类别判断
来源：http://wlc.nwbrower.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wkx.jinqigfzy.top

[S22] C：字符串转数字
来源：http://mbz.shzxlz.cn

atoi("42");  strtod("3.14", NULL);
来源：http://owm.jiagoushi.top

[S23] C：随机数
来源：http://ypg.pengpengdd.cyou

srand(time(NULL));  int r = rand() % 100;
来源：http://gbe.cashguo.top

[S24] C：获取本地时间
来源：http://jlb.yfazqb.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ryf.nanxuanxn.top

[S25] C：内存拷贝
来源：http://jse.dianchejie.cn

memcpy(dst, src, n);
来源：http://euo.zhijiandao.cn

[S26] C：内存清零
来源：http://avm.yangfankeji.com

memset(a, 0, sizeof a);
来源：http://jwp.hongshengwenyu.top

[S27] C：定义常量
来源：http://xot.jinghuilouyu.cn

const double PI = 3.14159;
来源：http://tbu.jlsjyb.cn

[S28] C：静态变量
来源：http://sjc.jinghuilouyu.cn

static int counter = 0;
来源：http://xai.fzhhl.top

[S29] C：变参函数
来源：http://qcz.hongshengwenyu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oml.nanxinkj.top

[S30] C：头文件保护
来源：http://njx.hfpthk.cn

#ifndef X_H
来源：http://dmm.hywenlv.cn

#define X_H
来源：http://xdj.zhaomingkeji.xyz

#endif
来源：http://osk.chenzaomai.com

[S31] C++：Hello World
来源：http://nvt.ydzc1.top

#include <iostream>
来源：http://fuc.dashuyun.cn

int main() { std::cout << "Hello\n"; }
来源：http://lgt.guannengcc.top

[S32] C++：字符串
来源：http://pdn.zdbjq.cn

std::string s = "hi";  s += "!";
来源：http://tqz.yuanzhike.top

[S33] C++：vector 增删
来源：http://mej.cashguo.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nxp.52xcode.cn

[S34] C++：遍历 vector
来源：http://riy.jqgfzy.top

for (auto &x : v) { std::cout << x; }
来源：http://kaa.sxryk.cn

[S35] C++：map
来源：http://kvv.yangfankeji.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zlg.cheryme.top

[S36] C++：unordered_map
来源：http://gla.hywenlv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zyi.daxiang520.top

[S37] C++：set
来源：http://aea.sweek.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jtq.zhijiandao.cn

[S38] C++：排序
来源：http://zza.nanxinkj.top

std::sort(v.begin(), v.end());
来源：http://muw.bbcook.cn

[S39] C++：自定义比较器排序
来源：http://aov.hysaishi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kbj.jiagoushi.top

[S40] C++：查找元素
来源：http://tsn.zhoulong.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qvn.0kj1m.cn

[S41] C++：类与构造函数
来源：http://xip.jqgufenzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xji.ehwqpu.com

[S42] C++：继承与虚函数
来源：http://udx.birdmap.top

class B : public Base { public: void f() override {} };
来源：http://aze.iojbl.cn

[S43] C++：智能指针
来源：http://xcf.ehwqpu.com

auto p = std::make_unique<int>(5);
来源：http://eij.ehwqpu.com

[S44] C++：引用传参
来源：http://jle.xylfe.cn

void inc(int &x) { ++x; }
来源：http://otb.tian-w.cn

[S45] C++：lambda
来源：http://hme.fehbvm.com

auto add = [](int a, int b) { return a + b; };
来源：http://xbq.cdnleiting.top

[S46] C++：函数模板
来源：http://iwd.hesvh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nab.sysykeji.top

[S47] C++：结构化绑定遍历
来源：http://opq.xuanzx.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tet.0kj1m.cn

[S48] C++：逐行读文件
来源：http://aev.nanxuanxn.top

std::ifstream in("a.txt");  std::string line;
来源：http://oyj.9152youxi.cn

while (std::getline(in, line)) { }
来源：http://bks.gzhubu.top

[S49] C++：写文件
来源：http://ekl.zdbjq.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://peu.tian-w.cn

[S50] C++：格式化数字
来源：http://wrq.hywenlv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rqs.shanyushiyangtech.top

[S51] C++：显式类型转换
来源：http://pmx.mhx1999.top

static_cast<double>(a) / b
来源：http://bva.xuanzx.com

[S52] C++：const 与 noexcept
来源：http://qay.smart0.xyz

int size() const noexcept { return n_; }
来源：http://jxn.xziqi.cn

[S53] C++：移动语义
来源：http://frr.cqqwz.cn

std::vector<int> w = std::move(v);
来源：http://joy.jinghuilouyu.cn

[S54] C++：异常处理
来源：http://pne.pengpengdd.cyou

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oah.xingfuxueyuan.xyz

[S55] C++：结构化绑定
来源：http://jrw.yonumen.top

auto [a, b] = std::make_pair(1, 2);
来源：http://nwi.316326.xyz

[S56] C++：optional
来源：http://lac.tianlin.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hom.smart0.xyz

[S57] C++：编译期常量
来源：http://gnz.shzxlz.cn

constexpr int N = 10;
来源：http://xax.zhixingplan.top

[S58] C++：命名空间
来源：http://sav.yuanzhike.top

namespace ns { int f() { return 1; } }
来源：http://mwa.aizwys.cn

[S59] C++：静态断言
来源：http://mte.jqgufenzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yzb.yonumen.top

[S60] C++：遍历并删除元素
来源：http://ayb.gogol.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yea.zhiwuduotai.top

================================================================================
来源：http://ixh.tarul.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://byy.nanxuanxn.top

================================================================================
来源：http://mlx.hnxiangtu.top

[T01] Kotlin：Hello World
来源：http://woc.redwolf501.top

println("Hello")
来源：http://wsf.haohaochexian.top

[T02] Kotlin：变量
来源：http://acr.jqgfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fmz.zhoulong.xyz

[T03] Kotlin：字符串模板
来源：http://ipd.ybcxt.top

"值: $b"
来源：http://zxu.mhx1999.top

[T04] Kotlin：空安全
来源：http://chx.tian-w.cn

val n: String? = null;  n?.length
来源：http://wff.uphjek.com

[T05] Kotlin：when 表达式
来源：http://tes.hfpthk.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lkw.aibaodan.cn

[T06] Kotlin：集合映射
来源：http://ezy.shanyushiyangtech.top

listOf(1, 2, 3).map { it * 2 }
来源：http://cpy.yuanzhike.top

[T07] Kotlin：集合过滤
来源：http://ljn.xinyue.icu

listOf(1, 2, 3).filter { it > 1 }
来源：http://nmo.nanxinkj.top

[T08] Kotlin：数据类
来源：http://ksl.jinqigufen.top

data class User(val name: String, val age: Int)
来源：http://bzh.zhengqikj.top

[T09] Kotlin：扩展函数
来源：http://rqq.andypj.xyz

fun String.exclaim() = this + "!"
来源：http://jux.mhx1999.top

[T10] Kotlin：默认参数
来源：http://jhj.aizwys.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jjc.ydzc1.top

[T11] Kotlin：协程
来源：http://lsq.ybcxt.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ybi.hysaishi.cn

[T12] Kotlin：解构声明
来源：http://zro.zhixingplan.top

val (a, b) = Pair(1, 2)
来源：http://svj.jyoumei.cn

[T13] Kotlin：只读 Map
来源：http://hde.jinghuilouyu.cn

val m = mapOf("a" to 1)
来源：http://dgc.tarul.cn

[T14] Kotlin：循环
来源：http://xog.yueranfly.top

for (i in 1..10) println(i)
来源：http://imx.ppjwa.cn

[T15] Kotlin：接口
来源：http://wwn.redwolf501.top

interface Shape { fun area(): Double }
来源：http://auy.yuanzhike.top

[T16] Swift：Hello World
来源：http://mib.meibo888.top

print("Hello")
来源：http://gcb.pycfn.com

[T17] Swift：变量与常量
来源：http://loa.hfpthk.cn

var a = 1;  let b = 2
来源：http://flv.yanxiufei.cn

[T18] Swift：字符串插值
来源：http://nxh.sufxvd.cn

"值: \(b)"
来源：http://abl.xingfuxueyuan.xyz

[T19] Swift：可选绑定
来源：http://uyw.chenzaomai.com

if let n = opt { print(n) }
来源：http://cxs.jlsjyb.cn

[T20] Swift：数组操作
来源：http://tvy.zhengqikj.top

var a = [1, 2, 3];  a.append(4)
来源：http://mxp.zhiwuduotai.top

[T21] Swift：遍历
来源：http://ctp.hcnkem.com

for x in a { print(x) }
来源：http://gub.xuetiantiany.cn

[T22] Swift：字典
来源：http://ohu.fktsv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://unv.meibo888.top

[T23] Swift：函数
来源：http://aol.gogol.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hxy.zhoulong.xyz

[T24] Swift：闭包
来源：http://njl.nwbrower.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ewr.hcnkem.com

[T25] Swift：结构体
来源：http://tmo.feifeiyinyue.top

struct P { var x: Int }
来源：http://cbx.cucudq.cn

[T26] Swift：类与重写
来源：http://omr.xuanzx.com

class A: Base { override func f() {} }
来源：http://efl.zdqjudy.top

[T27] Swift：错误处理
来源：http://szy.jianghu66.top

do { try f() } catch { print(error) }
来源：http://goh.pengpengdd.cyou

[T28] Swift：枚举
来源：http://rwx.zdqjudy.top

enum Color { case red, green }
来源：http://cgf.hnqzz.top

[T29] Swift：guard 提前返回
来源：http://tdw.hfpthk.cn

guard let x = opt else { return }
来源：http://dto.sxryk.cn

[T30] Swift：协议
来源：http://hut.yfazqb.com

protocol Shape { func area() -> Double }
来源：http://gdv.wangshuangyany.cn

[T31] Lua：Hello World
来源：http://jpw.redwolf501.top

print("Hello")
来源：http://zew.haohaochexian.top

[T32] Lua：局部变量
来源：http://eqv.zhoulong.xyz

local a = 1
来源：http://fhw.jlsjyb.cn

[T33] Lua：表（数组）
来源：http://suu.vehdjk.com

local t = {1, 2, 3};  t[4] = 4
来源：http://kym.bbcook.cn

[T34] Lua：遍历表
来源：http://lxj.jlsjyb.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kuk.ehwqpu.com

[T35] Lua：字典表
来源：http://orn.cucudq.cn

local d = { a = 1 };  d.b = 2
来源：http://xqj.ppjwa.cn

[T36] Lua：函数
来源：http://bzf.ppjwa.cn

function add(a, b) return a + b end
来源：http://xxf.gaohongyu789.top

[T37] Lua：字符串拼接
来源：http://vov.birdmap.top

"a" .. "b"
来源：http://fbz.hcnkem.com

[T38] Lua：条件
来源：http://ibc.pycfn.com

if x > 0 then print("正") end
来源：http://rrs.52xcode.cn

[T39] Lua：模式匹配
来源：http://tng.jinqigfzy.top

string.find(s, "%d+")
来源：http://vod.feifeiyinyue.top

[T40] Lua：元表
来源：http://rzb.jlsjyb.cn

setmetatable({}, { __index = base })
来源：http://ocw.yanxiufei.cn


<!-- 参考信息 -->