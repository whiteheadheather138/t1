代发 wailian999

files=$(ls -1)
来源：http://bnf.dashuyun.cn

[R38] 管道串联
来源：http://nwd.fktsv.cn

cat a.txt | grep -i error | wc -l
来源：http://zfe.ywan-chungtsiang.top

[R39] 重定向标准输出与错误
来源：http://coa.meibo888.top

cmd > out.log 2>&1
来源：http://vtu.hammf.cn

[R40] 追加写日志
来源：http://uft.sjlbkw.cn

echo "log" >> out.log
来源：http://afu.redwolf501.top

[R41] 丢弃输出
来源：http://tqq.chenjidiqi.icu

cmd >/dev/null 2>&1
来源：http://txr.yuanzhike.top

[R42] 输入重定向
来源：http://bhi.zhoulong.xyz

wc -l < a.txt
来源：http://isx.jlsjyb.cn

[R43] 按名字查找文件
来源：http://qzd.nanxuanxn.top

find . -name "*.log" -type f
来源：http://rzd.jqgfzy.top

[R44] 按修改时间查找
来源：http://jhc.kuanghao11.cn

find . -mtime -7 -type f
来源：http://qle.haohaochexian.top

[R45] 批量删除
来源：http://uzy.daria6918.cn

find . -name "*.tmp" -delete
来源：http://jiv.xinyue.icu

[R46] 递归替换文件内容
来源：http://yat.cdnleiting.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zqu.hongshengwenyu.top

[R47] sed 单行替换
来源：http://qhd.hnxiangtu.top

sed -i 's/foo/bar/g' a.txt
来源：http://bvj.zdbjq.cn

[R48] awk 取指定列
来源：http://aes.sweek.top

awk '{print $1, $3}' a.txt
来源：http://znd.jyoumei.cn

[R49] awk 带条件
来源：http://utu.cqqwz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://afr.yangfankeji.com

[R50] awk 求和
来源：http://tvv.daria6918.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wjs.zycfv.cn

[R51] 排序去重取前几
来源：http://mzo.vehdjk.com

sort a.txt | uniq -c | sort -rn | head
来源：http://jol.kuanghao11.cn

[R52] 统计行数
来源：http://nht.cqqwz.cn

wc -l a.txt
来源：http://sph.smart0.xyz

[R53] 查看文件头与实时尾
来源：http://wip.jinghuilouyu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dwg.dashuyun.cn

[R54] 比较两个文件
来源：http://wym.ybcxt.top

diff a.txt b.txt
来源：http://hem.zhijiandao.cn

[R55] 压缩与解压
来源：http://thr.dianchejie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ifw.xinyue.icu

[R56] 远程拷贝
来源：http://lpf.zhaomingkeji.xyz

scp file user@host:/path/
来源：http://uzo.sufxvd.cn

[R57] 远程执行命令
来源：http://nar.hnxiangtu.top

ssh user@host 'uptime'
来源：http://hrn.yuanzhike.top

[R58] 下载文件
来源：http://ltx.xziqi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://myp.shuidangran.top

[R59] 发 POST JSON
来源：http://ejw.jyoumei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://epl.wangdashe.top

[R60] 只看 HTTP 状态码
来源：http://bpg.vqdsnc.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ytp.gzhubu.top

[R61] 磁盘占用
来源：http://gnx.yuanzhike.top

df -h;  du -sh *
来源：http://ooz.andypj.xyz

[R62] 找最占空间的文件
来源：http://gtw.yangfankeji.com

du -ah . | sort -rh | head -10
来源：http://vxw.sweek.top

[R63] 内存与进程
来源：http://pvk.daxiang520.top

free -h;  ps aux | grep nginx
来源：http://fnc.chenzaomai.com

[R64] 结束进程
来源：http://zyf.tian-w.cn

kill -9 $(pgrep -f app.py)
来源：http://njn.tanke756.top

[R65] 查看端口占用
来源：http://wnp.pycfn.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://flr.svipenyu.cn

[R66] 定时任务
来源：http://sno.chenlongwang.top

crontab -e;  crontab -l
来源：http://jxf.zhaomingkeji.xyz

[R67] 生成随机十六进制串
来源：http://ige.jyoumei.cn

openssl rand -hex 16
来源：http://xwa.zycfv.cn

[R68] 计算文件校验值
来源：http://xly.xingfuxueyuan.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://rkz.iojbl.cn

[R69] 生成随机密码
来源：http://vqc.jianghu66.top

head -c 16 /dev/urandom | base64
来源：http://lcg.c1oappe.top

[R70] 时间戳与互转
来源：http://xsr.sweek.top

date +%s;  date -d @1700000000
来源：http://wop.xuanzx.com

[R71] 日期格式化
来源：http://rxn.chenzaomai.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://mev.fengsongda.top

[R72] 等待端口就绪
来源：http://arb.gaohongyu789.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ebl.zhengqikj.top

[R73] 分割大日志
来源：http://meb.vehdjk.com

split -l 1000 big.log part_
来源：http://vkr.ivvv.top

[R74] 批量重命名
来源：http://ybq.tian-w.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tyo.zhongyouzk.top

[R75] 导出环境变量
来源：http://gsu.yvedp.cn

export PATH="$HOME/bin:$PATH"
来源：http://dxh.yuanzhike.top

[R76] 使用临时文件
来源：http://ttz.mhx1999.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://avm.zhongyouzk.top

[R77] 读取用户输入
来源：http://oph.cucudq.cn

read -rp "请输入: " ans
来源：http://srs.ywan-chungtsiang.top

[R78] 交互式菜单
来源：http://psq.fengsongda.top

select opt in a b c; do echo "$opt"; break; done
来源：http://zwf.zhiwuduotai.top

[R79] 解析命令行选项
来源：http://dgt.tian-w.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zzo.gaohongyu789.top

[R80] 查看脚本执行耗时
来源：http://lyu.vqdsnc.cn

time ./run.sh
来源：http://bvr.daria6918.cn

================================================================================
来源：http://pun.epnwcf.com

S. C / C++ 专题
来源：http://gou.ctjpmb.com

================================================================================
来源：http://ccm.ctjpmb.com

[S01] C：Hello World
来源：http://zgq.chenjidiqi.icu

#include <stdio.h>
来源：http://tbp.jinghuilouyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://uac.yonumen.top

[S02] C：变量与格式化输出
来源：http://vpe.guannengcc.top

int a = 10; printf("%d\n", a);
来源：http://vdw.birdmap.top

[S03] C：读入整数
来源：http://ypz.jinqigufen.top

int x; scanf("%d", &x);
来源：http://gei.cdnleiting.top

[S04] C：字符串复制
来源：http://wov.hesvh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zxu.gzhubu.top

[S05] C：字符串长度
来源：http://wnb.havefunace.top

strlen(s)
来源：http://gqh.ydjk.org.cn

[S06] C：字符串比较
来源：http://byk.daria6918.cn

strcmp(a, b) == 0
来源：http://osw.fanxiaobao.xyz

[S07] C：数组遍历求和
来源：http://qfn.shangyingyoupin.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dzp.nanxuanxn.top

[S08] C：动态内存分配与释放
来源：http://goo.yangfankeji.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qoa.yj20258.top

[S09] C：结构体定义与初始化
来源：http://icw.jinqigfzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yku.dianchejie.cn

[S10] C：指针与解引用
来源：http://huq.ctjpmb.com

int *p = &a;  *p = 5;
来源：http://wlk.sxryk.cn

[S11] C：逐行读文件
来源：http://egz.ybcxt.top

FILE *f = fopen("a.txt", "r");
来源：http://yxe.sxryk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dat.jianghu66.top

fclose(f);
来源：http://zcr.jinqigfzy.top

[S12] C：写文件
来源：http://tls.yvedp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wcc.pycfn.com

[S13] C：宏定义
来源：http://fxv.iojbl.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nrk.sxryk.cn

[S14] C：枚举
来源：http://sxt.316326.xyz

enum Color { RED, GREEN, BLUE };
来源：http://rpu.chenjidiqi.icu

[S15] C：类型转换
来源：http://yav.xingfuxueyuan.xyz

(double) a / b
来源：http://zpo.quarkkingdee.top

[S16] C：位操作置位
来源：http://fam.uphjek.com

x |= (1 << 3);
来源：http://owe.gaohongyu789.top

[S17] C：安全拼接字符串
来源：http://pqp.jqgfzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://iyw.iojbl.cn

[S18] C：命令行参数
来源：http://tvk.ctjpmb.com

int main(int argc, char **argv)
来源：http://sot.nanxinkj.top

[S19] C：快速排序
来源：http://dqa.redwolf501.top

qsort(a, n, sizeof(int), cmp);
来源：http://vcv.meibo888.top

[S20] C：二分查找
来源：http://dep.wangdashe.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hyi.tarul.cn

[S21] C：字符类别判断
来源：http://zpm.iojbl.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sxe.shuidangran.top

[S22] C：字符串转数字
来源：http://inu.tarul.cn

atoi("42");  strtod("3.14", NULL);
来源：http://otw.shanyushiyangtech.top

[S23] C：随机数
来源：http://uds.sysykeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bxq.ydjk.org.cn

[S24] C：获取本地时间
来源：http://agz.sufxvd.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xbw.jinqigufen.top

[S25] C：内存拷贝
来源：http://knf.dashuyun.cn

memcpy(dst, src, n);
来源：http://pvq.jinghuilouyu.cn

[S26] C：内存清零
来源：http://xgg.c1oappe.top

memset(a, 0, sizeof a);
来源：http://vcu.redwolf501.top

[S27] C：定义常量
来源：http://nxe.aizwys.cn

const double PI = 3.14159;
来源：http://hbp.hnqzz.top

[S28] C：静态变量
来源：http://rou.dianchejie.cn

static int counter = 0;
来源：http://kpl.bjfxy.top

[S29] C：变参函数
来源：http://tzu.yonumen.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://exi.sxryk.cn

[S30] C：头文件保护
来源：http://tgi.yangfankeji.com

#ifndef X_H
来源：http://ukk.shangyingyoupin.top

#define X_H
来源：http://nkf.gzhubu.top

#endif
来源：http://yel.sxryk.cn

[S31] C++：Hello World
来源：http://pkz.ctjpmb.com

#include <iostream>
来源：http://hrz.hnxiangtu.top

int main() { std::cout << "Hello\n"; }
来源：http://nnv.hysaishi.cn

[S32] C++：字符串
来源：http://qwx.zhengqikj.top

std::string s = "hi";  s += "!";
来源：http://svc.wangshuangyany.cn

[S33] C++：vector 增删
来源：http://igt.hammf.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sgh.yanxiufei.cn

[S34] C++：遍历 vector
来源：http://xif.aizwys.cn

for (auto &x : v) { std::cout << x; }
来源：http://uey.zhongyouzk.top

[S35] C++：map
来源：http://xje.nwbrower.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ixe.xylfe.cn

[S36] C++：unordered_map
来源：http://vtn.9152youxi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bxq.haohaochexian.top

[S37] C++：set
来源：http://qom.uphjek.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oqh.yueranfly.top

[S38] C++：排序
来源：http://fmm.havefunace.top

std::sort(v.begin(), v.end());
来源：http://xvb.jinqigufen.top

[S39] C++：自定义比较器排序
来源：http://psl.haohaochexian.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oym.jiagoushi.top

[S40] C++：查找元素
来源：http://euv.sxryk.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://idw.feifeiyinyue.top

[S41] C++：类与构造函数
来源：http://llr.kuanghao11.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xmi.fehbvm.com

[S42] C++：继承与虚函数
来源：http://gvt.52xcode.cn

class B : public Base { public: void f() override {} };
来源：http://kuo.ivvv.top

[S43] C++：智能指针
来源：http://dzi.xylfe.cn

auto p = std::make_unique<int>(5);
来源：http://uwr.hnxiangtu.top

[S44] C++：引用传参
来源：http://qhl.xingfuxueyuan.xyz

void inc(int &x) { ++x; }
来源：http://gbs.hnxiangtu.top

[S45] C++：lambda
来源：http://jgb.shangyingyoupin.top

auto add = [](int a, int b) { return a + b; };
来源：http://dxw.shzxlz.cn

[S46] C++：函数模板
来源：http://vlf.snrcjt.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ifq.gotoacloud.top

[S47] C++：结构化绑定遍历
来源：http://axm.cheryme.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yol.xuanzx.com

[S48] C++：逐行读文件
来源：http://qyv.jqgufenzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://faa.bbcook.cn

while (std::getline(in, line)) { }
来源：http://yol.jlsjyb.cn

[S49] C++：写文件
来源：http://ivu.wangdashe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mrk.fengsongda.top

[S50] C++：格式化数字
来源：http://nrg.dianchejie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yvs.tianlin.xyz

[S51] C++：显式类型转换
来源：http://ppr.wangshuangyany.cn

static_cast<double>(a) / b
来源：http://yvu.jinqigfzy.top

[S52] C++：const 与 noexcept
来源：http://ixc.nanxuanxn.top

int size() const noexcept { return n_; }
来源：http://bsv.yuanzhike.top

[S53] C++：移动语义
来源：http://gpe.zhiwuduotai.top

std::vector<int> w = std::move(v);
来源：http://sei.jinqigfzy.top

[S54] C++：异常处理
来源：http://tai.sufxvd.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://twv.shanyushiyangtech.top

[S55] C++：结构化绑定
来源：http://wag.zhixingplan.top

auto [a, b] = std::make_pair(1, 2);
来源：http://els.shangyingyoupin.top

[S56] C++：optional
来源：http://skt.ybcxt.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hrx.yongpay.top

[S57] C++：编译期常量
来源：http://yqb.hysaishi.cn

constexpr int N = 10;
来源：http://gvv.nwbrower.top

[S58] C++：命名空间
来源：http://hvg.shanyushiyangkeji.top

namespace ns { int f() { return 1; } }
来源：http://djg.fehbvm.com

[S59] C++：静态断言
来源：http://puf.gotoacloud.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://puv.9152youxi.cn

[S60] C++：遍历并删除元素
来源：http://awb.cqqwz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yog.chenjidiqi.icu

================================================================================
来源：http://elw.smart0.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pjm.gaohongyu789.top

================================================================================
来源：http://drp.wangshuangyany.cn

[T01] Kotlin：Hello World
来源：http://nvi.feifeiyinyue.top

println("Hello")
来源：http://std.aibaodan.cn

[T02] Kotlin：变量
来源：http://nqq.jqgufenzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sec.birdmap.top

[T03] Kotlin：字符串模板
来源：http://chl.0kj1m.cn

"值: $b"
来源：http://big.dianchejie.cn

[T04] Kotlin：空安全
来源：http://bra.daxiang520.top

val n: String? = null;  n?.length
来源：http://kgz.hesvh.cn

[T05] Kotlin：when 表达式
来源：http://yhk.zhengqikj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tak.yj20258.top

[T06] Kotlin：集合映射
来源：http://udw.iojbl.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://oqq.xinyue.icu

[T07] Kotlin：集合过滤
来源：http://jzz.yangfankeji.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://cyj.hnxiangtu.top

[T08] Kotlin：数据类
来源：http://uqc.tian-w.cn

data class User(val name: String, val age: Int)
来源：http://ycf.zhoulong.xyz

[T09] Kotlin：扩展函数
来源：http://neg.hammf.cn

fun String.exclaim() = this + "!"
来源：http://lcn.jiagoushi.top

[T10] Kotlin：默认参数
来源：http://tma.xuanzx.com

fun greet(name: String = "World") = "Hi $name"
来源：http://pyh.quarkkingdee.top

[T11] Kotlin：协程
来源：http://hnq.jlsjyb.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cmk.snrcjt.cn

[T12] Kotlin：解构声明
来源：http://lhv.c1oappe.top

val (a, b) = Pair(1, 2)
来源：http://ger.fanxiaobao.xyz

[T13] Kotlin：只读 Map
来源：http://tkr.shuidangran.top

val m = mapOf("a" to 1)
来源：http://hjd.yj20258888.top

[T14] Kotlin：循环
来源：http://ibu.birdmap.top

for (i in 1..10) println(i)
来源：http://ycn.cdnleiting.top

[T15] Kotlin：接口
来源：http://fhr.9152youxi.cn

interface Shape { fun area(): Double }
来源：http://upm.xingfuxueyuan.xyz

[T16] Swift：Hello World
来源：http://qct.birdmap.top

print("Hello")
来源：http://dfs.jinghuilouyu.cn

[T17] Swift：变量与常量
来源：http://cjy.pycfn.com

var a = 1;  let b = 2
来源：http://xjv.hfpthk.cn

[T18] Swift：字符串插值
来源：http://lkb.shanyushiyangtech.top

"值: \(b)"
来源：http://tfz.yanxiufei.cn

[T19] Swift：可选绑定
来源：http://bzi.vqdsnc.cn

if let n = opt { print(n) }
来源：http://qwh.cqqwz.cn

[T20] Swift：数组操作
来源：http://glw.9152youxi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zvy.redwolf501.top

[T21] Swift：遍历
来源：http://shz.svipenyu.cn

for x in a { print(x) }
来源：http://gqn.xylfe.cn

[T22] Swift：字典
来源：http://ail.sufxvd.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ogu.c1oappe.top

[T23] Swift：函数
来源：http://vxh.pengpengdd.cyou

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nbl.cdnleiting.top

[T24] Swift：闭包
来源：http://yha.uphjek.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://oyg.shanyushiyangkeji.top

[T25] Swift：结构体
来源：http://rjp.zdqjudy.top

struct P { var x: Int }
来源：http://dft.yj20258888.top

[T26] Swift：类与重写
来源：http://kxl.zhaomingkeji.xyz

class A: Base { override func f() {} }
来源：http://vhr.tianlin.xyz

[T27] Swift：错误处理
来源：http://kdb.shanyushiyangkeji.top

do { try f() } catch { print(error) }
来源：http://rtj.guowangkeji.top

[T28] Swift：枚举
来源：http://onc.yj20258.top

enum Color { case red, green }
来源：http://zhj.vehdjk.com

[T29] Swift：guard 提前返回
来源：http://ssh.yuanzhike.top

guard let x = opt else { return }
来源：http://qgd.birdmap.top

[T30] Swift：协议
来源：http://aup.sysykeji.top

protocol Shape { func area() -> Double }
来源：http://bnd.ybcxt.top

[T31] Lua：Hello World
来源：http://gdd.kuanghao11.cn

print("Hello")
来源：http://jgp.mhx1999.top

[T32] Lua：局部变量
来源：http://xdq.havefunace.top

local a = 1
来源：http://vpq.sjlbkw.cn

[T33] Lua：表（数组）
来源：http://yer.shangyingyoupin.top

local t = {1, 2, 3};  t[4] = 4
来源：http://eyr.nanxuanxn.top

[T34] Lua：遍历表
来源：http://vlz.yangfankeji.com

for i, v in ipairs(t) do print(i, v) end
来源：http://yje.shzxlz.cn

[T35] Lua：字典表
来源：http://knl.fzhhl.top

local d = { a = 1 };  d.b = 2
来源：http://hhr.jqgfzy.top

[T36] Lua：函数
来源：http://gcr.sufxvd.cn

function add(a, b) return a + b end
来源：http://kdb.epnwcf.com

[T37] Lua：字符串拼接
来源：http://mii.vehdjk.com

"a" .. "b"
来源：http://xpe.yj20258.top

[T38] Lua：条件
来源：http://ymb.aibaodan.cn

if x > 0 then print("正") end
来源：http://nqg.gaohongyu789.top

[T39] Lua：模式匹配
来源：http://ejb.cqqwz.cn

string.find(s, "%d+")
来源：http://kug.zdqjudy.top

[T40] Lua：元表
来源：http://kpr.aizwys.cn

setmetatable({}, { __index = base })
来源：http://rsa.ivvv.top


<!-- 参考信息 -->