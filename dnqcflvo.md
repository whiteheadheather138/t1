代发 wailian999

files=$(ls -1)
来源：http://mkn.zdqjudy.top

[R38] 管道串联
来源：http://whs.aibaodan.cn

cat a.txt | grep -i error | wc -l
来源：http://pcp.zhengqikj.top

[R39] 重定向标准输出与错误
来源：http://qri.ctjpmb.com

cmd > out.log 2>&1
来源：http://ciz.ybcxt.top

[R40] 追加写日志
来源：http://gps.hammf.cn

echo "log" >> out.log
来源：http://xou.ywan-chungtsiang.top

[R41] 丢弃输出
来源：http://sns.vehdjk.com

cmd >/dev/null 2>&1
来源：http://zop.hcnkem.com

[R42] 输入重定向
来源：http://sgi.sjlbkw.cn

wc -l < a.txt
来源：http://iee.hywenlv.cn

[R43] 按名字查找文件
来源：http://lzn.zhengqikj.top

find . -name "*.log" -type f
来源：http://uka.ybcxt.top

[R44] 按修改时间查找
来源：http://vre.cheryme.top

find . -mtime -7 -type f
来源：http://pbl.sufxvd.cn

[R45] 批量删除
来源：http://jdn.dashuyun.cn

find . -name "*.tmp" -delete
来源：http://cgk.yuanzhike.top

[R46] 递归替换文件内容
来源：http://vzh.jiagoushi.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fvj.zhengqikj.top

[R47] sed 单行替换
来源：http://hzn.yueranfly.top

sed -i 's/foo/bar/g' a.txt
来源：http://skz.hnqzz.top

[R48] awk 取指定列
来源：http://foy.jinqigfzy.top

awk '{print $1, $3}' a.txt
来源：http://wud.zhixingplan.top

[R49] awk 带条件
来源：http://tai.yueranfly.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ssv.daxiang520.top

[R50] awk 求和
来源：http://ikh.ctjpmb.com

awk '{s += $2} END {print s}' a.txt
来源：http://euo.fktsv.cn

[R51] 排序去重取前几
来源：http://chr.hywenlv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jsg.ydjk.org.cn

[R52] 统计行数
来源：http://wmu.smart0.xyz

wc -l a.txt
来源：http://yzj.fanxiaobao.xyz

[R53] 查看文件头与实时尾
来源：http://dbe.kuanghao11.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ppa.ivvv.top

[R54] 比较两个文件
来源：http://wrn.jqgufenzy.top

diff a.txt b.txt
来源：http://wpw.dashuyun.cn

[R55] 压缩与解压
来源：http://lam.cqqwz.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rog.zhiwuduotai.top

[R56] 远程拷贝
来源：http://hvj.vqdsnc.cn

scp file user@host:/path/
来源：http://nrt.jiagoushi.top

[R57] 远程执行命令
来源：http://sxx.zhoulong.xyz

ssh user@host 'uptime'
来源：http://ipv.sjlbkw.cn

[R58] 下载文件
来源：http://dwm.dianchejie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ryf.shzxlz.cn

[R59] 发 POST JSON
来源：http://ejs.fktsv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mlq.c1oappe.top

[R60] 只看 HTTP 状态码
来源：http://fmt.vqdsnc.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ivw.yangfankeji.com

[R61] 磁盘占用
来源：http://qhg.yangfankeji.com

df -h;  du -sh *
来源：http://umu.hammf.cn

[R62] 找最占空间的文件
来源：http://nyw.andypj.xyz

du -ah . | sort -rh | head -10
来源：http://vau.316326.xyz

[R63] 内存与进程
来源：http://qxl.jyoumei.cn

free -h;  ps aux | grep nginx
来源：http://zpx.zhaomingkeji.xyz

[R64] 结束进程
来源：http://yic.wangdashe.top

kill -9 $(pgrep -f app.py)
来源：http://vfi.tanke756.top

[R65] 查看端口占用
来源：http://rjo.shanyushiyangkeji.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nco.shangyingyoupin.top

[R66] 定时任务
来源：http://nyt.fktsv.cn

crontab -e;  crontab -l
来源：http://wfh.cheryme.top

[R67] 生成随机十六进制串
来源：http://snx.c1oappe.top

openssl rand -hex 16
来源：http://lhc.sjlbkw.cn

[R68] 计算文件校验值
来源：http://fdf.hesvh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yfi.tian-w.cn

[R69] 生成随机密码
来源：http://zax.redwolf501.top

head -c 16 /dev/urandom | base64
来源：http://txq.jinqigufen.top

[R70] 时间戳与互转
来源：http://eyw.hesvh.cn

date +%s;  date -d @1700000000
来源：http://dbt.316326.xyz

[R71] 日期格式化
来源：http://fkm.ywan-chungtsiang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qlw.hcnkem.com

[R72] 等待端口就绪
来源：http://jzp.ydzc1.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jqw.0kj1m.cn

[R73] 分割大日志
来源：http://caz.redwolf501.top

split -l 1000 big.log part_
来源：http://kkd.hysaishi.cn

[R74] 批量重命名
来源：http://edz.jiagoushi.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xio.jinyuanbaomall.cn

[R75] 导出环境变量
来源：http://bic.zhongyouzk.top

export PATH="$HOME/bin:$PATH"
来源：http://lqc.sufxvd.cn

[R76] 使用临时文件
来源：http://zjn.bjfxy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tpz.yonumen.top

[R77] 读取用户输入
来源：http://ttr.gotoacloud.top

read -rp "请输入: " ans
来源：http://fxe.9152youxi.cn

[R78] 交互式菜单
来源：http://xiy.jqgfzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://cwb.cheryme.top

[R79] 解析命令行选项
来源：http://cjo.cucudq.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nff.shzxlz.cn

[R80] 查看脚本执行耗时
来源：http://pkf.zhaomingkeji.xyz

time ./run.sh
来源：http://eoh.bjfxy.top

================================================================================
来源：http://ihs.yonumen.top

S. C / C++ 专题
来源：http://dld.andypj.xyz

================================================================================
来源：http://oxb.vqdsnc.cn

[S01] C：Hello World
来源：http://ypz.aizwys.cn

#include <stdio.h>
来源：http://hmv.sjlbkw.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mhz.xingfuxueyuan.xyz

[S02] C：变量与格式化输出
来源：http://kbs.jinyuanbaomall.cn

int a = 10; printf("%d\n", a);
来源：http://xno.hysaishi.cn

[S03] C：读入整数
来源：http://vmt.andypj.xyz

int x; scanf("%d", &x);
来源：http://psy.xuanzx.com

[S04] C：字符串复制
来源：http://foo.tarul.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hpf.zycfv.cn

[S05] C：字符串长度
来源：http://jqz.fzhhl.top

strlen(s)
来源：http://dcb.epnwcf.com

[S06] C：字符串比较
来源：http://duc.feifeiyinyue.top

strcmp(a, b) == 0
来源：http://wes.tanke756.top

[S07] C：数组遍历求和
来源：http://cqt.xuanzx.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zfy.chenzaomai.com

[S08] C：动态内存分配与释放
来源：http://uwr.jiagoushi.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yum.redwolf501.top

[S09] C：结构体定义与初始化
来源：http://dhx.ivvv.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fga.shuidangran.top

[S10] C：指针与解引用
来源：http://hzb.sjlbkw.cn

int *p = &a;  *p = 5;
来源：http://wny.yueranfly.top

[S11] C：逐行读文件
来源：http://rxx.yj20258.top

FILE *f = fopen("a.txt", "r");
来源：http://vpm.pycfn.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://bpf.jiagoushi.top

fclose(f);
来源：http://dxy.xylfe.cn

[S12] C：写文件
来源：http://yrf.gogol.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cuv.sufxvd.cn

[S13] C：宏定义
来源：http://kao.redwolf501.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://boj.wangdashe.top

[S14] C：枚举
来源：http://vlm.zdbjq.cn

enum Color { RED, GREEN, BLUE };
来源：http://hyh.zhaomingkeji.xyz

[S15] C：类型转换
来源：http://qvv.fanxiaobao.xyz

(double) a / b
来源：http://bqx.chenjidiqi.icu

[S16] C：位操作置位
来源：http://ehm.jianghu66.top

x |= (1 << 3);
来源：http://eqb.bbcook.cn

[S17] C：安全拼接字符串
来源：http://gef.pengpengdd.cyou

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ged.dianchejie.cn

[S18] C：命令行参数
来源：http://ffa.hysaishi.cn

int main(int argc, char **argv)
来源：http://jco.yuanzhike.top

[S19] C：快速排序
来源：http://utn.yangfankeji.com

qsort(a, n, sizeof(int), cmp);
来源：http://qlv.dashuyun.cn

[S20] C：二分查找
来源：http://ikq.yj20258.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zcc.uphjek.com

[S21] C：字符类别判断
来源：http://gep.zdqjudy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cjf.sjlbkw.cn

[S22] C：字符串转数字
来源：http://mzi.hnqzz.top

atoi("42");  strtod("3.14", NULL);
来源：http://vjf.hywenlv.cn

[S23] C：随机数
来源：http://sor.hywenlv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zlr.tianlin.xyz

[S24] C：获取本地时间
来源：http://jbh.aizwys.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uho.shanyushiyangtech.top

[S25] C：内存拷贝
来源：http://kmn.ctjpmb.com

memcpy(dst, src, n);
来源：http://krq.ppjwa.cn

[S26] C：内存清零
来源：http://xua.zhoulong.xyz

memset(a, 0, sizeof a);
来源：http://yef.jianghu66.top

[S27] C：定义常量
来源：http://pxm.ydjk.org.cn

const double PI = 3.14159;
来源：http://oza.0kj1m.cn

[S28] C：静态变量
来源：http://fkj.gogol.net.cn

static int counter = 0;
来源：http://cww.c1oappe.top

[S29] C：变参函数
来源：http://zpw.quarkkingdee.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://odl.cheryme.top

[S30] C：头文件保护
来源：http://wst.daxiang520.top

#ifndef X_H
来源：http://hwd.yvedp.cn

#define X_H
来源：http://fcr.zycfv.cn

#endif
来源：http://imk.yvedp.cn

[S31] C++：Hello World
来源：http://ogc.jinqigfzy.top

#include <iostream>
来源：http://jmz.jlsjyb.cn

int main() { std::cout << "Hello\n"; }
来源：http://dng.hnxiangtu.top

[S32] C++：字符串
来源：http://qfv.jinyuanbaomall.cn

std::string s = "hi";  s += "!";
来源：http://xxu.birdmap.top

[S33] C++：vector 增删
来源：http://afj.zhiwuduotai.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tiv.jqgufenzy.top

[S34] C++：遍历 vector
来源：http://umt.jlsjyb.cn

for (auto &x : v) { std::cout << x; }
来源：http://dbd.ehwqpu.com

[S35] C++：map
来源：http://vvv.birdmap.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pib.bbcook.cn

[S36] C++：unordered_map
来源：http://ivg.daria6918.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yxy.feifeiyinyue.top

[S37] C++：set
来源：http://fxd.ywan-chungtsiang.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nxt.guannengcc.top

[S38] C++：排序
来源：http://kyx.tianlin.xyz

std::sort(v.begin(), v.end());
来源：http://oqx.guannengcc.top

[S39] C++：自定义比较器排序
来源：http://mtp.kuanghao11.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qbg.aizwys.cn

[S40] C++：查找元素
来源：http://dea.ehwqpu.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qxe.xylfe.cn

[S41] C++：类与构造函数
来源：http://pcs.hywenlv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tzy.sysykeji.top

[S42] C++：继承与虚函数
来源：http://tjt.zhaomingkeji.xyz

class B : public Base { public: void f() override {} };
来源：http://qvc.shanyushiyangtech.top

[S43] C++：智能指针
来源：http://wxy.dianchejie.cn

auto p = std::make_unique<int>(5);
来源：http://cij.jinghuilouyu.cn

[S44] C++：引用传参
来源：http://plw.cdnleiting.top

void inc(int &x) { ++x; }
来源：http://cyi.svipenyu.cn

[S45] C++：lambda
来源：http://civ.bjfxy.top

auto add = [](int a, int b) { return a + b; };
来源：http://oes.jlsjyb.cn

[S46] C++：函数模板
来源：http://rbt.guowangkeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mzc.vqdsnc.cn

[S47] C++：结构化绑定遍历
来源：http://mxw.zhengqikj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ysa.nanxinkj.top

[S48] C++：逐行读文件
来源：http://jsc.pengpengdd.cyou

std::ifstream in("a.txt");  std::string line;
来源：http://ezi.ppjwa.cn

while (std::getline(in, line)) { }
来源：http://oxi.feifeiyinyue.top

[S49] C++：写文件
来源：http://cwh.ctjpmb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pwk.cqqwz.cn

[S50] C++：格式化数字
来源：http://nxb.wangdashe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zpt.wangshuangyany.cn

[S51] C++：显式类型转换
来源：http://xbt.sufxvd.cn

static_cast<double>(a) / b
来源：http://wzf.shanyushiyangkeji.top

[S52] C++：const 与 noexcept
来源：http://zll.hcnkem.com

int size() const noexcept { return n_; }
来源：http://fls.uphjek.com

[S53] C++：移动语义
来源：http://bpk.hysaishi.cn

std::vector<int> w = std::move(v);
来源：http://wga.jlsjyb.cn

[S54] C++：异常处理
来源：http://jtz.havefunace.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://szg.jqgfzy.top

[S55] C++：结构化绑定
来源：http://kev.xylfe.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ryr.vehdjk.com

[S56] C++：optional
来源：http://eeg.aibaodan.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jus.sysykeji.top

[S57] C++：编译期常量
来源：http://iat.zhengqikj.top

constexpr int N = 10;
来源：http://hly.guannengcc.top

[S58] C++：命名空间
来源：http://zun.yanxiufei.cn

namespace ns { int f() { return 1; } }
来源：http://bfy.xuetiantiany.cn

[S59] C++：静态断言
来源：http://ynf.zhixingplan.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cbf.guowangkeji.top

[S60] C++：遍历并删除元素
来源：http://tla.yongpay.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ekb.ywan-chungtsiang.top

================================================================================
来源：http://sdf.gaohongyu789.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ulf.aibaodan.cn

================================================================================
来源：http://uhk.xuetiantiany.cn

[T01] Kotlin：Hello World
来源：http://fhx.hesvh.cn

println("Hello")
来源：http://lpj.xinyue.icu

[T02] Kotlin：变量
来源：http://utb.iojbl.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cwv.kuanghao11.cn

[T03] Kotlin：字符串模板
来源：http://axv.jqgufenzy.top

"值: $b"
来源：http://hca.ydzc1.top

[T04] Kotlin：空安全
来源：http://mxc.zhoulong.xyz

val n: String? = null;  n?.length
来源：http://lme.xylfe.cn

[T05] Kotlin：when 表达式
来源：http://lug.shanyushiyangtech.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hbj.ehwqpu.com

[T06] Kotlin：集合映射
来源：http://cmd.smart0.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://cul.kuanghao11.cn

[T07] Kotlin：集合过滤
来源：http://bvs.hnqzz.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://okd.gogol.net.cn

[T08] Kotlin：数据类
来源：http://kuq.guannengcc.top

data class User(val name: String, val age: Int)
来源：http://sau.wangshuangyany.cn

[T09] Kotlin：扩展函数
来源：http://nli.jyoumei.cn

fun String.exclaim() = this + "!"
来源：http://yho.meibo888.top

[T10] Kotlin：默认参数
来源：http://uxh.zhaomingkeji.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://fqv.chenjidiqi.icu

[T11] Kotlin：协程
来源：http://coe.nanxinkj.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://wvz.birdmap.top

[T12] Kotlin：解构声明
来源：http://dmk.sjlbkw.cn

val (a, b) = Pair(1, 2)
来源：http://nnw.iojbl.cn

[T13] Kotlin：只读 Map
来源：http://cft.xuetiantiany.cn

val m = mapOf("a" to 1)
来源：http://umx.hammf.cn

[T14] Kotlin：循环
来源：http://zvu.cqqwz.cn

for (i in 1..10) println(i)
来源：http://rbv.hammf.cn

[T15] Kotlin：接口
来源：http://wye.gogol.net.cn

interface Shape { fun area(): Double }
来源：http://ail.nanxinkj.top

[T16] Swift：Hello World
来源：http://bqf.ctjpmb.com

print("Hello")
来源：http://udk.zycfv.cn

[T17] Swift：变量与常量
来源：http://kfx.cqqwz.cn

var a = 1;  let b = 2
来源：http://qgv.ywan-chungtsiang.top

[T18] Swift：字符串插值
来源：http://pwv.wangdashe.top

"值: \(b)"
来源：http://wuu.yanxiufei.cn

[T19] Swift：可选绑定
来源：http://jud.birdmap.top

if let n = opt { print(n) }
来源：http://ooa.svipenyu.cn

[T20] Swift：数组操作
来源：http://bqk.zhaomingkeji.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://scw.ctjpmb.com

[T21] Swift：遍历
来源：http://ubm.birdmap.top

for x in a { print(x) }
来源：http://fxd.pycfn.com

[T22] Swift：字典
来源：http://upy.cashguo.top

var d = ["a": 1];  d["b"] = 2
来源：http://hqz.ydzc1.top

[T23] Swift：函数
来源：http://awi.meibo888.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hmi.jinyuanbaomall.cn

[T24] Swift：闭包
来源：http://jxs.svipenyu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://toa.shangyingyoupin.top

[T25] Swift：结构体
来源：http://pcs.svipenyu.cn

struct P { var x: Int }
来源：http://aet.zycfv.cn

[T26] Swift：类与重写
来源：http://hwy.jinqigufen.top

class A: Base { override func f() {} }
来源：http://hvo.jlsjyb.cn

[T27] Swift：错误处理
来源：http://pdq.xuetiantiany.cn

do { try f() } catch { print(error) }
来源：http://eac.gogol.net.cn

[T28] Swift：枚举
来源：http://zcs.fehbvm.com

enum Color { case red, green }
来源：http://pxm.zhaomingkeji.xyz

[T29] Swift：guard 提前返回
来源：http://uyt.bbcook.cn

guard let x = opt else { return }
来源：http://kjn.daria6918.cn

[T30] Swift：协议
来源：http://bky.gaohongyu789.top

protocol Shape { func area() -> Double }
来源：http://xex.zhiwuduotai.top

[T31] Lua：Hello World
来源：http://fmf.zhijiandao.cn

print("Hello")
来源：http://rwd.jinqigufen.top

[T32] Lua：局部变量
来源：http://hsx.zdqjudy.top

local a = 1
来源：http://fll.xingfuxueyuan.xyz

[T33] Lua：表（数组）
来源：http://ymp.zhaomingkeji.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://and.xylfe.cn

[T34] Lua：遍历表
来源：http://jbl.hysaishi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://stb.daria6918.cn

[T35] Lua：字典表
来源：http://lwq.fanxiaobao.xyz

local d = { a = 1 };  d.b = 2
来源：http://ltr.jianghu66.top

[T36] Lua：函数
来源：http://poc.yj20258888.top

function add(a, b) return a + b end
来源：http://uij.gaohongyu789.top

[T37] Lua：字符串拼接
来源：http://guz.jqgfzy.top

"a" .. "b"
来源：http://dxq.jqgufenzy.top

[T38] Lua：条件
来源：http://vbi.jiagoushi.top

if x > 0 then print("正") end
来源：http://fzy.xuanzx.com

[T39] Lua：模式匹配
来源：http://vve.yj20258888.top

string.find(s, "%d+")
来源：http://ufq.hywenlv.cn

[T40] Lua：元表
来源：http://lih.cdnleiting.top

setmetatable({}, { __index = base })
来源：http://joz.chenlongwang.top


<!-- 参考信息 -->