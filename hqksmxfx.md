代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://lbv.pengpengdd.cyou

[R36] 并发执行多个任务
来源：http://zrp.gotoacloud.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nbt.jinqigufen.top

[R37] 把输出赋给变量
来源：http://moy.tarul.cn

files=$(ls -1)
来源：http://nqt.zhaomingkeji.xyz

[R38] 管道串联
来源：http://pmd.daxiang520.top

cat a.txt | grep -i error | wc -l
来源：http://vtc.sjlbkw.cn

[R39] 重定向标准输出与错误
来源：http://uzf.zhongyouzk.top

cmd > out.log 2>&1
来源：http://kqh.yonumen.top

[R40] 追加写日志
来源：http://kak.zhaomingkeji.xyz

echo "log" >> out.log
来源：http://ndv.yj202588.top

[R41] 丢弃输出
来源：http://rpj.cashguo.top

cmd >/dev/null 2>&1
来源：http://ire.xylfe.cn

[R42] 输入重定向
来源：http://gwd.hywenlv.cn

wc -l < a.txt
来源：http://tje.yuxming.cn

[R43] 按名字查找文件
来源：http://rhp.quarkkingdee.top

find . -name "*.log" -type f
来源：http://oao.gaohongyu789.top

[R44] 按修改时间查找
来源：http://oqc.cqqwz.cn

find . -mtime -7 -type f
来源：http://ddx.guowangkeji.top

[R45] 批量删除
来源：http://ikq.xziqi.cn

find . -name "*.tmp" -delete
来源：http://fzl.gaohongyu789.top

[R46] 递归替换文件内容
来源：http://zpx.quarkkingdee.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uza.redwolf501.top

[R47] sed 单行替换
来源：http://odk.vqdsnc.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qdd.hongshengwenyu.top

[R48] awk 取指定列
来源：http://owd.sysykeji.top

awk '{print $1, $3}' a.txt
来源：http://mgg.guowangkeji.top

[R49] awk 带条件
来源：http://vdx.hfpthk.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://las.yj20258.top

[R50] awk 求和
来源：http://hzu.52xcode.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ejk.guowangkeji.top

[R51] 排序去重取前几
来源：http://guh.cheryme.top

sort a.txt | uniq -c | sort -rn | head
来源：http://uzn.zhongyouzk.top

[R52] 统计行数
来源：http://sml.hammf.cn

wc -l a.txt
来源：http://cyt.tanke756.top

[R53] 查看文件头与实时尾
来源：http://ymn.daxiang520.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bvm.cheryme.top

[R54] 比较两个文件
来源：http://orf.tarul.cn

diff a.txt b.txt
来源：http://ihs.sxryk.cn

[R55] 压缩与解压
来源：http://wsc.dashuyun.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sxn.meibo888.top

[R56] 远程拷贝
来源：http://yry.meibo888.top

scp file user@host:/path/
来源：http://adb.jlsjyb.cn

[R57] 远程执行命令
来源：http://vxg.yueranfly.top

ssh user@host 'uptime'
来源：http://siv.xuetiantiany.cn

[R58] 下载文件
来源：http://vfj.hesvh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tul.pengpengdd.cyou

[R59] 发 POST JSON
来源：http://eub.fehbvm.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://stb.fengsongda.top

[R60] 只看 HTTP 状态码
来源：http://kwt.fehbvm.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://any.shuidangran.top

[R61] 磁盘占用
来源：http://ivr.jinqigufen.top

df -h;  du -sh *
来源：http://enp.pengpengdd.cyou

[R62] 找最占空间的文件
来源：http://eoc.tian-w.cn

du -ah . | sort -rh | head -10
来源：http://lux.mhx1999.top

[R63] 内存与进程
来源：http://bvv.ppjwa.cn

free -h;  ps aux | grep nginx
来源：http://jre.gaohongyu789.top

[R64] 结束进程
来源：http://vcc.andypj.xyz

kill -9 $(pgrep -f app.py)
来源：http://hsf.gotoacloud.top

[R65] 查看端口占用
来源：http://akq.cdnleiting.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nsb.jinqigfzy.top

[R66] 定时任务
来源：http://njq.zhaomingkeji.xyz

crontab -e;  crontab -l
来源：http://ubj.pycfn.com

[R67] 生成随机十六进制串
来源：http://zqu.fanxiaobao.xyz

openssl rand -hex 16
来源：http://wvs.fktsv.cn

[R68] 计算文件校验值
来源：http://fjn.cdnleiting.top

sha256sum a.txt;  md5sum a.txt
来源：http://rys.316326.xyz

[R69] 生成随机密码
来源：http://clx.shanyushiyangkeji.top

head -c 16 /dev/urandom | base64
来源：http://mum.svipenyu.cn

[R70] 时间戳与互转
来源：http://fby.sweek.top

date +%s;  date -d @1700000000
来源：http://svr.hywenlv.cn

[R71] 日期格式化
来源：http://zqt.xuetiantiany.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hsc.kuanghao11.cn

[R72] 等待端口就绪
来源：http://gqs.daria6918.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rja.xinyue.icu

[R73] 分割大日志
来源：http://isv.yvedp.cn

split -l 1000 big.log part_
来源：http://nzd.hcnkem.com

[R74] 批量重命名
来源：http://axz.cqqwz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pnl.jinqigufen.top

[R75] 导出环境变量
来源：http://tkn.wangdashe.top

export PATH="$HOME/bin:$PATH"
来源：http://usz.svipenyu.cn

[R76] 使用临时文件
来源：http://ffa.daria6918.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nuy.fanxiaobao.xyz

[R77] 读取用户输入
来源：http://ehr.c1oappe.top

read -rp "请输入: " ans
来源：http://hea.ehwqpu.com

[R78] 交互式菜单
来源：http://bre.sxryk.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ufo.yj202588.top

[R79] 解析命令行选项
来源：http://syc.yuxming.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cat.bbcook.cn

[R80] 查看脚本执行耗时
来源：http://wuj.sysykeji.top

time ./run.sh
来源：http://ghe.tarul.cn

================================================================================
来源：http://svz.hnxiangtu.top

S. C / C++ 专题
来源：http://ojk.sufxvd.cn

================================================================================
来源：http://ubg.havefunace.top

[S01] C：Hello World
来源：http://ffg.jinyuanbaomall.cn

#include <stdio.h>
来源：http://sxj.snrcjt.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zbm.jlsjyb.cn

[S02] C：变量与格式化输出
来源：http://gux.ivvv.top

int a = 10; printf("%d\n", a);
来源：http://ons.zycfv.cn

[S03] C：读入整数
来源：http://mtw.bjfxy.top

int x; scanf("%d", &x);
来源：http://dfr.pycfn.com

[S04] C：字符串复制
来源：http://qjw.tanke756.top

char dst[32]; strcpy(dst, "hi");
来源：http://ebc.zhiwuduotai.top

[S05] C：字符串长度
来源：http://qdy.uphjek.com

strlen(s)
来源：http://zoa.fanxiaobao.xyz

[S06] C：字符串比较
来源：http://lcj.meibo888.top

strcmp(a, b) == 0
来源：http://nhu.guowangkeji.top

[S07] C：数组遍历求和
来源：http://gqm.gzhubu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mma.jqgufenzy.top

[S08] C：动态内存分配与释放
来源：http://nku.tian-w.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zqd.birdmap.top

[S09] C：结构体定义与初始化
来源：http://kln.jinghuilouyu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wro.jinghuilouyu.cn

[S10] C：指针与解引用
来源：http://kkp.ehwqpu.com

int *p = &a;  *p = 5;
来源：http://ros.yj202588.top

[S11] C：逐行读文件
来源：http://xfs.jqgufenzy.top

FILE *f = fopen("a.txt", "r");
来源：http://zoh.vqdsnc.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rny.jqgufenzy.top

fclose(f);
来源：http://urc.9152youxi.cn

[S12] C：写文件
来源：http://yqz.xinyue.icu

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hah.yfazqb.com

[S13] C：宏定义
来源：http://adx.shzxlz.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wci.nwbrower.top

[S14] C：枚举
来源：http://zja.hcnkem.com

enum Color { RED, GREEN, BLUE };
来源：http://nwz.jqgufenzy.top

[S15] C：类型转换
来源：http://jhl.shanyushiyangtech.top

(double) a / b
来源：http://sfo.vqdsnc.cn

[S16] C：位操作置位
来源：http://kqj.hcnkem.com

x |= (1 << 3);
来源：http://sdl.shuidangran.top

[S17] C：安全拼接字符串
来源：http://vhj.meibo888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rwp.hywenlv.cn

[S18] C：命令行参数
来源：http://vcg.tian-w.cn

int main(int argc, char **argv)
来源：http://vfj.zhongyouzk.top

[S19] C：快速排序
来源：http://rey.gogol.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://utl.fktsv.cn

[S20] C：二分查找
来源：http://aui.iojbl.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wux.xuanzx.com

[S21] C：字符类别判断
来源：http://ilp.andypj.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://who.nanxinkj.top

[S22] C：字符串转数字
来源：http://fiz.hfpthk.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tyc.sufxvd.cn

[S23] C：随机数
来源：http://jrx.ybcxt.top

srand(time(NULL));  int r = rand() % 100;
来源：http://dvc.cucudq.cn

[S24] C：获取本地时间
来源：http://sjd.epnwcf.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sov.mhx1999.top

[S25] C：内存拷贝
来源：http://pic.shanyushiyangkeji.top

memcpy(dst, src, n);
来源：http://vkx.hnxiangtu.top

[S26] C：内存清零
来源：http://apn.0kj1m.cn

memset(a, 0, sizeof a);
来源：http://jtt.shanyushiyangkeji.top

[S27] C：定义常量
来源：http://wsp.quarkkingdee.top

const double PI = 3.14159;
来源：http://app.zdqjudy.top

[S28] C：静态变量
来源：http://qwq.cheryme.top

static int counter = 0;
来源：http://ijj.cheryme.top

[S29] C：变参函数
来源：http://ogx.9152youxi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ajf.yongpay.top

[S30] C：头文件保护
来源：http://raf.gogol.net.cn

#ifndef X_H
来源：http://tyh.dianchejie.cn

#define X_H
来源：http://bzn.nanxuanxn.top

#endif
来源：http://myi.yuxming.cn

[S31] C++：Hello World
来源：http://rwh.iojbl.cn

#include <iostream>
来源：http://pai.wangshuangyany.cn

int main() { std::cout << "Hello\n"; }
来源：http://yts.cheryme.top

[S32] C++：字符串
来源：http://evx.daxiang520.top

std::string s = "hi";  s += "!";
来源：http://ftk.cqqwz.cn

[S33] C++：vector 增删
来源：http://qim.shzxlz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ntc.ydjk.org.cn

[S34] C++：遍历 vector
来源：http://oty.yuanzhike.top

for (auto &x : v) { std::cout << x; }
来源：http://wga.yfazqb.com

[S35] C++：map
来源：http://tkg.shanyushiyangtech.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zxf.feifeiyinyue.top

[S36] C++：unordered_map
来源：http://ntf.xuetiantiany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mlc.fzhhl.top

[S37] C++：set
来源：http://gxx.haohaochexian.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hwj.svipenyu.cn

[S38] C++：排序
来源：http://xae.shuidangran.top

std::sort(v.begin(), v.end());
来源：http://wlo.chenzaomai.com

[S39] C++：自定义比较器排序
来源：http://hbw.iojbl.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rcn.yanxiufei.cn

[S40] C++：查找元素
来源：http://adv.guowangkeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://duy.yj20258.top

[S41] C++：类与构造函数
来源：http://wny.cdnleiting.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cno.guannengcc.top

[S42] C++：继承与虚函数
来源：http://vbm.52xcode.cn

class B : public Base { public: void f() override {} };
来源：http://yqc.aibaodan.cn

[S43] C++：智能指针
来源：http://hsr.aibaodan.cn

auto p = std::make_unique<int>(5);
来源：http://eqx.cqqwz.cn

[S44] C++：引用传参
来源：http://knm.fktsv.cn

void inc(int &x) { ++x; }
来源：http://oks.ybcxt.top

[S45] C++：lambda
来源：http://jrp.gaohongyu789.top

auto add = [](int a, int b) { return a + b; };
来源：http://ufg.tianlin.xyz

[S46] C++：函数模板
来源：http://tvq.yj202588.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://aot.ehwqpu.com

[S47] C++：结构化绑定遍历
来源：http://ksh.zycfv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fyy.andypj.xyz

[S48] C++：逐行读文件
来源：http://okc.uphjek.com

std::ifstream in("a.txt");  std::string line;
来源：http://mfc.zdqjudy.top

while (std::getline(in, line)) { }
来源：http://ngt.fanxiaobao.xyz

[S49] C++：写文件
来源：http://evh.quarkkingdee.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wyk.shuidangran.top

[S50] C++：格式化数字
来源：http://xev.zhengqikj.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kvz.ybcxt.top

[S51] C++：显式类型转换
来源：http://mue.xingfuxueyuan.xyz

static_cast<double>(a) / b
来源：http://zwv.wangdashe.top

[S52] C++：const 与 noexcept
来源：http://mho.0kj1m.cn

int size() const noexcept { return n_; }
来源：http://fab.zdbjq.cn

[S53] C++：移动语义
来源：http://ozo.zhiwuduotai.top

std::vector<int> w = std::move(v);
来源：http://fhu.vehdjk.com

[S54] C++：异常处理
来源：http://nqs.shanyushiyangkeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gyn.zhoulong.xyz

[S55] C++：结构化绑定
来源：http://pve.ybcxt.top

auto [a, b] = std::make_pair(1, 2);
来源：http://cwm.ivvv.top

[S56] C++：optional
来源：http://ysq.sufxvd.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mgy.jqgufenzy.top

[S57] C++：编译期常量
来源：http://xvk.ydzc1.top

constexpr int N = 10;
来源：http://vvj.chenlongwang.top

[S58] C++：命名空间
来源：http://wju.wangdashe.top

namespace ns { int f() { return 1; } }
来源：http://hbm.snrcjt.cn

[S59] C++：静态断言
来源：http://hrt.ydzc1.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ykf.0kj1m.cn

[S60] C++：遍历并删除元素
来源：http://lxg.guowangkeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ukc.xuetiantiany.cn

================================================================================
来源：http://fck.wangshuangyany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vqq.xingfuxueyuan.xyz

================================================================================
来源：http://ael.cdnleiting.top

[T01] Kotlin：Hello World
来源：http://dpk.wangshuangyany.cn

println("Hello")
来源：http://edk.zdqjudy.top

[T02] Kotlin：变量
来源：http://awe.pengpengdd.cyou

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fxf.daria6918.cn

[T03] Kotlin：字符串模板
来源：http://jmm.hnqzz.top

"值: $b"
来源：http://zov.mhx1999.top

[T04] Kotlin：空安全
来源：http://btz.shzxlz.cn

val n: String? = null;  n?.length
来源：http://veh.snrcjt.cn

[T05] Kotlin：when 表达式
来源：http://maz.xziqi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://unc.fktsv.cn

[T06] Kotlin：集合映射
来源：http://oep.fktsv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pil.jiagoushi.top

[T07] Kotlin：集合过滤
来源：http://dsw.zhiwuduotai.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://sgh.jyoumei.cn

[T08] Kotlin：数据类
来源：http://eix.hongshengwenyu.top

data class User(val name: String, val age: Int)
来源：http://zlw.zhoulong.xyz

[T09] Kotlin：扩展函数
来源：http://qor.iojbl.cn

fun String.exclaim() = this + "!"
来源：http://jvy.yvedp.cn

[T10] Kotlin：默认参数
来源：http://epp.tarul.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mlh.meibo888.top

[T11] Kotlin：协程
来源：http://diz.ppjwa.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://uae.xylfe.cn

[T12] Kotlin：解构声明
来源：http://ful.ydjk.org.cn

val (a, b) = Pair(1, 2)
来源：http://rbg.meibo888.top

[T13] Kotlin：只读 Map
来源：http://eai.jyoumei.cn

val m = mapOf("a" to 1)
来源：http://yhl.zhijiandao.cn

[T14] Kotlin：循环
来源：http://kog.hongshengwenyu.top

for (i in 1..10) println(i)
来源：http://oqh.shangyingyoupin.top

[T15] Kotlin：接口
来源：http://eys.cdnleiting.top

interface Shape { fun area(): Double }
来源：http://krp.ivvv.top

[T16] Swift：Hello World
来源：http://yxo.guowangkeji.top

print("Hello")
来源：http://pgx.yj20258.top

[T17] Swift：变量与常量
来源：http://omh.chenzaomai.com

var a = 1;  let b = 2
来源：http://stj.aibaodan.cn

[T18] Swift：字符串插值
来源：http://hgu.xziqi.cn

"值: \(b)"
来源：http://mfu.jinqigfzy.top

[T19] Swift：可选绑定
来源：http://pgg.yj202588.top

if let n = opt { print(n) }
来源：http://jim.hfpthk.cn

[T20] Swift：数组操作
来源：http://mbk.wangdashe.top

var a = [1, 2, 3];  a.append(4)
来源：http://aip.zhijiandao.cn

[T21] Swift：遍历
来源：http://yuu.epnwcf.com

for x in a { print(x) }
来源：http://dkn.c1oappe.top

[T22] Swift：字典
来源：http://hyr.shangyingyoupin.top

var d = ["a": 1];  d["b"] = 2
来源：http://zne.hnxiangtu.top

[T23] Swift：函数
来源：http://wow.yfazqb.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ula.tian-w.cn

[T24] Swift：闭包
来源：http://vsa.shangyingyoupin.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://mnt.vqdsnc.cn

[T25] Swift：结构体
来源：http://iaf.c1oappe.top

struct P { var x: Int }
来源：http://yrh.tarul.cn

[T26] Swift：类与重写
来源：http://ssq.svipenyu.cn

class A: Base { override func f() {} }
来源：http://sys.haohaochexian.top

[T27] Swift：错误处理
来源：http://lzk.fanxiaobao.xyz

do { try f() } catch { print(error) }
来源：http://iry.hysaishi.cn

[T28] Swift：枚举
来源：http://vkn.nanxuanxn.top

enum Color { case red, green }
来源：http://hzz.gzhubu.top

[T29] Swift：guard 提前返回
来源：http://nkt.yj20258.top

guard let x = opt else { return }
来源：http://yom.zycfv.cn

[T30] Swift：协议
来源：http://kuk.smart0.xyz

protocol Shape { func area() -> Double }
来源：http://ifc.svipenyu.cn

[T31] Lua：Hello World
来源：http://yqm.zdqjudy.top

print("Hello")
来源：http://gyx.shuidangran.top

[T32] Lua：局部变量
来源：http://gth.shuidangran.top

local a = 1
来源：http://icp.ydzc1.top

[T33] Lua：表（数组）
来源：http://aaw.nwbrower.top

local t = {1, 2, 3};  t[4] = 4
来源：http://xed.hysaishi.cn

[T34] Lua：遍历表
来源：http://ekj.aizwys.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zxb.pengpengdd.cyou

[T35] Lua：字典表
来源：http://atw.zhoulong.xyz

local d = { a = 1 };  d.b = 2
来源：http://def.zhiwuduotai.top

[T36] Lua：函数
来源：http://yse.guannengcc.top

function add(a, b) return a + b end
来源：http://pld.pengpengdd.cyou

[T37] Lua：字符串拼接
来源：http://naa.pycfn.com

"a" .. "b"
来源：http://sez.shuidangran.top

[T38] Lua：条件
来源：http://gjm.cashguo.top

if x > 0 then print("正") end
来源：http://igv.zhengqikj.top


<!-- 参考信息 -->