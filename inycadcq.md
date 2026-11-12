代发 wailian999

files=$(ls -1)
来源：http://pwd.yj20258.top

[R38] 管道串联
来源：http://boo.zhoulong.xyz

cat a.txt | grep -i error | wc -l
来源：http://hag.dianchejie.cn

[R39] 重定向标准输出与错误
来源：http://xkg.jiagoushi.top

cmd > out.log 2>&1
来源：http://mjo.jyoumei.cn

[R40] 追加写日志
来源：http://gsv.dianchejie.cn

echo "log" >> out.log
来源：http://vwy.hcnkem.com

[R41] 丢弃输出
来源：http://tsz.tian-w.cn

cmd >/dev/null 2>&1
来源：http://iha.shuidangran.top

[R42] 输入重定向
来源：http://gtc.tianlin.xyz

wc -l < a.txt
来源：http://eaz.dianchejie.cn

[R43] 按名字查找文件
来源：http://dpf.zhaomingkeji.xyz

find . -name "*.log" -type f
来源：http://pwa.zhongyouzk.top

[R44] 按修改时间查找
来源：http://tzx.meibo888.top

find . -mtime -7 -type f
来源：http://mth.zhijiandao.cn

[R45] 批量删除
来源：http://ayj.dashuyun.cn

find . -name "*.tmp" -delete
来源：http://qjq.fengsongda.top

[R46] 递归替换文件内容
来源：http://iyk.fktsv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hqi.316326.xyz

[R47] sed 单行替换
来源：http://biq.shangyingyoupin.top

sed -i 's/foo/bar/g' a.txt
来源：http://aue.jianghu66.top

[R48] awk 取指定列
来源：http://xet.chenzaomai.com

awk '{print $1, $3}' a.txt
来源：http://iea.daxiang520.top

[R49] awk 带条件
来源：http://egf.nanxinkj.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bkb.zhixingplan.top

[R50] awk 求和
来源：http://gax.ybcxt.top

awk '{s += $2} END {print s}' a.txt
来源：http://dbt.bjfxy.top

[R51] 排序去重取前几
来源：http://nxb.sjlbkw.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://joa.hnqzz.top

[R52] 统计行数
来源：http://kad.gotoacloud.top

wc -l a.txt
来源：http://bwc.xylfe.cn

[R53] 查看文件头与实时尾
来源：http://jmx.shanyushiyangtech.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jvu.jqgufenzy.top

[R54] 比较两个文件
来源：http://mip.fktsv.cn

diff a.txt b.txt
来源：http://odo.aizwys.cn

[R55] 压缩与解压
来源：http://ncp.epnwcf.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zvz.jqgfzy.top

[R56] 远程拷贝
来源：http://hys.chenlongwang.top

scp file user@host:/path/
来源：http://ybu.chenjidiqi.icu

[R57] 远程执行命令
来源：http://xir.fktsv.cn

ssh user@host 'uptime'
来源：http://owa.jiagoushi.top

[R58] 下载文件
来源：http://rih.tian-w.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yfp.feifeiyinyue.top

[R59] 发 POST JSON
来源：http://qpy.chenjidiqi.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://emv.andypj.xyz

[R60] 只看 HTTP 状态码
来源：http://enx.haohaochexian.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vge.nanxuanxn.top

[R61] 磁盘占用
来源：http://ifn.zhiwuduotai.top

df -h;  du -sh *
来源：http://vvu.jqgufenzy.top

[R62] 找最占空间的文件
来源：http://mhd.vehdjk.com

du -ah . | sort -rh | head -10
来源：http://rat.zhongyouzk.top

[R63] 内存与进程
来源：http://izx.shuidangran.top

free -h;  ps aux | grep nginx
来源：http://kbz.bjfxy.top

[R64] 结束进程
来源：http://ksf.epnwcf.com

kill -9 $(pgrep -f app.py)
来源：http://yez.havefunace.top

[R65] 查看端口占用
来源：http://tdu.uphjek.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yys.jqgfzy.top

[R66] 定时任务
来源：http://qgv.ybcxt.top

crontab -e;  crontab -l
来源：http://twt.zycfv.cn

[R67] 生成随机十六进制串
来源：http://fco.52xcode.cn

openssl rand -hex 16
来源：http://vsf.gaohongyu789.top

[R68] 计算文件校验值
来源：http://jhv.yuanzhike.top

sha256sum a.txt;  md5sum a.txt
来源：http://dqh.xuetiantiany.cn

[R69] 生成随机密码
来源：http://nfh.jqgfzy.top

head -c 16 /dev/urandom | base64
来源：http://edu.gaohongyu789.top

[R70] 时间戳与互转
来源：http://akv.fanxiaobao.xyz

date +%s;  date -d @1700000000
来源：http://cqz.svipenyu.cn

[R71] 日期格式化
来源：http://hbf.svipenyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wxw.pengpengdd.cyou

[R72] 等待端口就绪
来源：http://njm.guannengcc.top

until nc -z localhost 3306; do sleep 1; done
来源：http://gmy.pengpengdd.cyou

[R73] 分割大日志
来源：http://hol.wangdashe.top

split -l 1000 big.log part_
来源：http://tvo.dashuyun.cn

[R74] 批量重命名
来源：http://ugi.jyoumei.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bhz.9152youxi.cn

[R75] 导出环境变量
来源：http://qkl.sjlbkw.cn

export PATH="$HOME/bin:$PATH"
来源：http://ztd.zdqjudy.top

[R76] 使用临时文件
来源：http://yka.316326.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://okq.xuanzx.com

[R77] 读取用户输入
来源：http://rju.sweek.top

read -rp "请输入: " ans
来源：http://wln.ehwqpu.com

[R78] 交互式菜单
来源：http://kux.yanxiufei.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mzy.birdmap.top

[R79] 解析命令行选项
来源：http://egf.vehdjk.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://svs.hongshengwenyu.top

[R80] 查看脚本执行耗时
来源：http://wne.fanxiaobao.xyz

time ./run.sh
来源：http://ete.yongpay.top

================================================================================
来源：http://uuk.xingfuxueyuan.xyz

S. C / C++ 专题
来源：http://idc.52xcode.cn

================================================================================
来源：http://xiq.fehbvm.com

[S01] C：Hello World
来源：http://fbk.ydzc1.top

#include <stdio.h>
来源：http://idw.fengsongda.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://obf.mhx1999.top

[S02] C：变量与格式化输出
来源：http://ovr.shanyushiyangtech.top

int a = 10; printf("%d\n", a);
来源：http://dxm.meibo888.top

[S03] C：读入整数
来源：http://dmd.chenjidiqi.icu

int x; scanf("%d", &x);
来源：http://cws.aibaodan.cn

[S04] C：字符串复制
来源：http://heb.epnwcf.com

char dst[32]; strcpy(dst, "hi");
来源：http://gbz.yonumen.top

[S05] C：字符串长度
来源：http://wia.yvedp.cn

strlen(s)
来源：http://evq.cqqwz.cn

[S06] C：字符串比较
来源：http://wim.shangyingyoupin.top

strcmp(a, b) == 0
来源：http://tgm.cheryme.top

[S07] C：数组遍历求和
来源：http://gab.hesvh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gat.snrcjt.cn

[S08] C：动态内存分配与释放
来源：http://lwn.hcnkem.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ndt.quarkkingdee.top

[S09] C：结构体定义与初始化
来源：http://zot.zdbjq.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xkm.jqgufenzy.top

[S10] C：指针与解引用
来源：http://vna.redwolf501.top

int *p = &a;  *p = 5;
来源：http://wli.epnwcf.com

[S11] C：逐行读文件
来源：http://cdb.pengpengdd.cyou

FILE *f = fopen("a.txt", "r");
来源：http://pdk.hfpthk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://aln.52xcode.cn

fclose(f);
来源：http://ybd.xuetiantiany.cn

[S12] C：写文件
来源：http://qjf.zdqjudy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://iks.guannengcc.top

[S13] C：宏定义
来源：http://pcz.fzhhl.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rvu.cqqwz.cn

[S14] C：枚举
来源：http://vcz.chenjidiqi.icu

enum Color { RED, GREEN, BLUE };
来源：http://wxv.zhijiandao.cn

[S15] C：类型转换
来源：http://coa.fehbvm.com

(double) a / b
来源：http://xbt.uphjek.com

[S16] C：位操作置位
来源：http://oxi.fengsongda.top

x |= (1 << 3);
来源：http://nub.jiagoushi.top

[S17] C：安全拼接字符串
来源：http://mgi.tanke756.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fvk.zhaomingkeji.xyz

[S18] C：命令行参数
来源：http://jvr.hnxiangtu.top

int main(int argc, char **argv)
来源：http://uby.snrcjt.cn

[S19] C：快速排序
来源：http://fuy.guowangkeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://caw.bbcook.cn

[S20] C：二分查找
来源：http://low.jqgufenzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://iry.zhixingplan.top

[S21] C：字符类别判断
来源：http://avl.guannengcc.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kpy.zhengqikj.top

[S22] C：字符串转数字
来源：http://emc.quarkkingdee.top

atoi("42");  strtod("3.14", NULL);
来源：http://sqd.epnwcf.com

[S23] C：随机数
来源：http://rkn.xuanzx.com

srand(time(NULL));  int r = rand() % 100;
来源：http://hpq.andypj.xyz

[S24] C：获取本地时间
来源：http://ize.uphjek.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://iiu.kuanghao11.cn

[S25] C：内存拷贝
来源：http://miu.gogol.net.cn

memcpy(dst, src, n);
来源：http://ioa.kuanghao11.cn

[S26] C：内存清零
来源：http://nyr.dashuyun.cn

memset(a, 0, sizeof a);
来源：http://zrj.yongpay.top

[S27] C：定义常量
来源：http://wrn.gzhubu.top

const double PI = 3.14159;
来源：http://ptx.jinqigufen.top

[S28] C：静态变量
来源：http://iwr.hywenlv.cn

static int counter = 0;
来源：http://adj.zhixingplan.top

[S29] C：变参函数
来源：http://vjh.hnxiangtu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nwv.feifeiyinyue.top

[S30] C：头文件保护
来源：http://jua.sjlbkw.cn

#ifndef X_H
来源：http://joz.fehbvm.com

#define X_H
来源：http://cgc.birdmap.top

#endif
来源：http://dom.guannengcc.top

[S31] C++：Hello World
来源：http://tuq.52xcode.cn

#include <iostream>
来源：http://gtx.fehbvm.com

int main() { std::cout << "Hello\n"; }
来源：http://tpi.52xcode.cn

[S32] C++：字符串
来源：http://ioz.guannengcc.top

std::string s = "hi";  s += "!";
来源：http://zco.jinghuilouyu.cn

[S33] C++：vector 增删
来源：http://ybl.ctjpmb.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wyt.ydjk.org.cn

[S34] C++：遍历 vector
来源：http://wpz.jqgfzy.top

for (auto &x : v) { std::cout << x; }
来源：http://pgy.xuetiantiany.cn

[S35] C++：map
来源：http://msz.yueranfly.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ywz.hammf.cn

[S36] C++：unordered_map
来源：http://fcl.yj202588.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iwx.sjlbkw.cn

[S37] C++：set
来源：http://lsn.fengsongda.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qsq.hysaishi.cn

[S38] C++：排序
来源：http://wbg.9152youxi.cn

std::sort(v.begin(), v.end());
来源：http://ktl.epnwcf.com

[S39] C++：自定义比较器排序
来源：http://vci.vqdsnc.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cnn.ybcxt.top

[S40] C++：查找元素
来源：http://prg.hywenlv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pja.shuidangran.top

[S41] C++：类与构造函数
来源：http://oip.yj20258888.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jat.gogol.net.cn

[S42] C++：继承与虚函数
来源：http://dkc.aibaodan.cn

class B : public Base { public: void f() override {} };
来源：http://jgp.pengpengdd.cyou

[S43] C++：智能指针
来源：http://ngg.chenzaomai.com

auto p = std::make_unique<int>(5);
来源：http://geh.mhx1999.top

[S44] C++：引用传参
来源：http://noj.cqqwz.cn

void inc(int &x) { ++x; }
来源：http://vie.yj202588.top

[S45] C++：lambda
来源：http://rgo.zhiwuduotai.top

auto add = [](int a, int b) { return a + b; };
来源：http://yld.hammf.cn

[S46] C++：函数模板
来源：http://uwe.redwolf501.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ski.shangyingyoupin.top

[S47] C++：结构化绑定遍历
来源：http://pgr.chenzaomai.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wmn.aizwys.cn

[S48] C++：逐行读文件
来源：http://lgx.shangyingyoupin.top

std::ifstream in("a.txt");  std::string line;
来源：http://srv.hammf.cn

while (std::getline(in, line)) { }
来源：http://zer.gotoacloud.top

[S49] C++：写文件
来源：http://sjj.tian-w.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://icc.ppjwa.cn

[S50] C++：格式化数字
来源：http://gjw.zhijiandao.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gaz.shangyingyoupin.top

[S51] C++：显式类型转换
来源：http://rds.c1oappe.top

static_cast<double>(a) / b
来源：http://ypv.smart0.xyz

[S52] C++：const 与 noexcept
来源：http://zmz.9152youxi.cn

int size() const noexcept { return n_; }
来源：http://zey.quarkkingdee.top

[S53] C++：移动语义
来源：http://bgu.mhx1999.top

std::vector<int> w = std::move(v);
来源：http://zgq.cashguo.top

[S54] C++：异常处理
来源：http://dmj.zhoulong.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hch.ivvv.top

[S55] C++：结构化绑定
来源：http://neu.gzhubu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://iyh.wangdashe.top

[S56] C++：optional
来源：http://osw.cashguo.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://khu.smart0.xyz

[S57] C++：编译期常量
来源：http://hyx.jianghu66.top

constexpr int N = 10;
来源：http://oyy.gzhubu.top

[S58] C++：命名空间
来源：http://qsm.hysaishi.cn

namespace ns { int f() { return 1; } }
来源：http://qll.epnwcf.com

[S59] C++：静态断言
来源：http://ury.epnwcf.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lyd.xingfuxueyuan.xyz

[S60] C++：遍历并删除元素
来源：http://lzz.ivvv.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ubn.zhiwuduotai.top

================================================================================
来源：http://xkm.ywan-chungtsiang.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ixs.jianghu66.top

================================================================================
来源：http://vkv.gaohongyu789.top

[T01] Kotlin：Hello World
来源：http://mvj.ctjpmb.com

println("Hello")
来源：http://ffu.jinqigfzy.top

[T02] Kotlin：变量
来源：http://rfe.gogol.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yia.nanxinkj.top

[T03] Kotlin：字符串模板
来源：http://owj.hywenlv.cn

"值: $b"
来源：http://xam.yueranfly.top

[T04] Kotlin：空安全
来源：http://jty.cdnleiting.top

val n: String? = null;  n?.length
来源：http://djn.jianghu66.top

[T05] Kotlin：when 表达式
来源：http://tzz.shangyingyoupin.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jyw.haohaochexian.top

[T06] Kotlin：集合映射
来源：http://qqw.dashuyun.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tku.hongshengwenyu.top

[T07] Kotlin：集合过滤
来源：http://bep.guannengcc.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ola.ywan-chungtsiang.top

[T08] Kotlin：数据类
来源：http://prr.cucudq.cn

data class User(val name: String, val age: Int)
来源：http://fjc.shangyingyoupin.top

[T09] Kotlin：扩展函数
来源：http://izg.zhoulong.xyz

fun String.exclaim() = this + "!"
来源：http://xjn.shuidangran.top

[T10] Kotlin：默认参数
来源：http://egk.yj20258888.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ecx.birdmap.top

[T11] Kotlin：协程
来源：http://mam.uphjek.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://zof.xylfe.cn

[T12] Kotlin：解构声明
来源：http://gyw.ydjk.org.cn

val (a, b) = Pair(1, 2)
来源：http://nae.zhoulong.xyz

[T13] Kotlin：只读 Map
来源：http://kty.quarkkingdee.top

val m = mapOf("a" to 1)
来源：http://hvb.pycfn.com

[T14] Kotlin：循环
来源：http://izn.zhijiandao.cn

for (i in 1..10) println(i)
来源：http://hgk.zdqjudy.top

[T15] Kotlin：接口
来源：http://ysj.zhengqikj.top

interface Shape { fun area(): Double }
来源：http://hod.hywenlv.cn

[T16] Swift：Hello World
来源：http://eau.yuxming.cn

print("Hello")
来源：http://hdd.pycfn.com

[T17] Swift：变量与常量
来源：http://dlv.nanxuanxn.top

var a = 1;  let b = 2
来源：http://qza.jlsjyb.cn

[T18] Swift：字符串插值
来源：http://jcc.zycfv.cn

"值: \(b)"
来源：http://ddp.yj20258.top

[T19] Swift：可选绑定
来源：http://tam.chenlongwang.top

if let n = opt { print(n) }
来源：http://orf.zdbjq.cn

[T20] Swift：数组操作
来源：http://prb.hfpthk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rml.pycfn.com

[T21] Swift：遍历
来源：http://sqy.birdmap.top

for x in a { print(x) }
来源：http://skr.zdqjudy.top

[T22] Swift：字典
来源：http://jyf.kuanghao11.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kay.ydzc1.top

[T23] Swift：函数
来源：http://nzk.gogol.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://iub.yfazqb.com

[T24] Swift：闭包
来源：http://oss.yangfankeji.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://xih.yanxiufei.cn

[T25] Swift：结构体
来源：http://mej.ppjwa.cn

struct P { var x: Int }
来源：http://pmv.cdnleiting.top

[T26] Swift：类与重写
来源：http://umi.wangdashe.top

class A: Base { override func f() {} }
来源：http://khk.uphjek.com

[T27] Swift：错误处理
来源：http://dfe.ydjk.org.cn

do { try f() } catch { print(error) }
来源：http://mpq.nanxuanxn.top

[T28] Swift：枚举
来源：http://pil.zhengqikj.top

enum Color { case red, green }
来源：http://woz.yuxming.cn

[T29] Swift：guard 提前返回
来源：http://lxj.zdbjq.cn

guard let x = opt else { return }
来源：http://vfs.dashuyun.cn

[T30] Swift：协议
来源：http://jzq.ywan-chungtsiang.top

protocol Shape { func area() -> Double }
来源：http://nvh.jlsjyb.cn

[T31] Lua：Hello World
来源：http://ggk.shuidangran.top

print("Hello")
来源：http://vjz.ybcxt.top

[T32] Lua：局部变量
来源：http://vgb.ybcxt.top

local a = 1
来源：http://zii.ivvv.top

[T33] Lua：表（数组）
来源：http://gqh.sysykeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ksu.bbcook.cn

[T34] Lua：遍历表
来源：http://nhi.hnxiangtu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://jmd.uphjek.com

[T35] Lua：字典表
来源：http://bre.fzhhl.top

local d = { a = 1 };  d.b = 2
来源：http://jgk.bjfxy.top

[T36] Lua：函数
来源：http://hft.chenjidiqi.icu

function add(a, b) return a + b end
来源：http://zdl.zycfv.cn

[T37] Lua：字符串拼接
来源：http://wtf.yonumen.top

"a" .. "b"
来源：http://ivl.zycfv.cn

[T38] Lua：条件
来源：http://ecj.bbcook.cn

if x > 0 then print("正") end
来源：http://uus.zdqjudy.top

[T39] Lua：模式匹配
来源：http://fkw.316326.xyz

string.find(s, "%d+")
来源：http://ugv.zhiwuduotai.top

[T40] Lua：元表
来源：http://uxt.tian-w.cn

setmetatable({}, { __index = base })
来源：http://trg.hcnkem.com


<!-- 参考信息 -->