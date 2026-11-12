代发 wailian999

cmd > out.log 2>&1
来源：http://xjv.vqdsnc.cn

[R40] 追加写日志
来源：http://xhy.c1oappe.top

echo "log" >> out.log
来源：http://tjg.yonumen.top

[R41] 丢弃输出
来源：http://dvg.hywenlv.cn

cmd >/dev/null 2>&1
来源：http://tsi.wangshuangyany.cn

[R42] 输入重定向
来源：http://oyf.meibo888.top

wc -l < a.txt
来源：http://saj.gogol.net.cn

[R43] 按名字查找文件
来源：http://nfi.fzhhl.top

find . -name "*.log" -type f
来源：http://urx.shangyingyoupin.top

[R44] 按修改时间查找
来源：http://jgg.ctjpmb.com

find . -mtime -7 -type f
来源：http://ych.snrcjt.cn

[R45] 批量删除
来源：http://alt.aizwys.cn

find . -name "*.tmp" -delete
来源：http://yok.xingfuxueyuan.xyz

[R46] 递归替换文件内容
来源：http://sfg.hcnkem.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sdg.hywenlv.cn

[R47] sed 单行替换
来源：http://fsv.xinyue.icu

sed -i 's/foo/bar/g' a.txt
来源：http://okv.0kj1m.cn

[R48] awk 取指定列
来源：http://oec.shanyushiyangkeji.top

awk '{print $1, $3}' a.txt
来源：http://rxd.yj202588.top

[R49] awk 带条件
来源：http://hmk.fzhhl.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kah.xziqi.cn

[R50] awk 求和
来源：http://xvc.zhoulong.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://ilg.cucudq.cn

[R51] 排序去重取前几
来源：http://laf.andypj.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://tic.shangyingyoupin.top

[R52] 统计行数
来源：http://eyl.dianchejie.cn

wc -l a.txt
来源：http://iil.uphjek.com

[R53] 查看文件头与实时尾
来源：http://hlk.meibo888.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hur.bbcook.cn

[R54] 比较两个文件
来源：http://ant.fengsongda.top

diff a.txt b.txt
来源：http://bme.zhoulong.xyz

[R55] 压缩与解压
来源：http://ana.wangshuangyany.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zdb.daria6918.cn

[R56] 远程拷贝
来源：http://qig.nanxuanxn.top

scp file user@host:/path/
来源：http://qbv.mhx1999.top

[R57] 远程执行命令
来源：http://iig.jinqigufen.top

ssh user@host 'uptime'
来源：http://qvn.hongshengwenyu.top

[R58] 下载文件
来源：http://snj.yonumen.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tnz.hysaishi.cn

[R59] 发 POST JSON
来源：http://pno.yvedp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ojj.daria6918.cn

[R60] 只看 HTTP 状态码
来源：http://mhx.jinqigfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://njt.shangyingyoupin.top

[R61] 磁盘占用
来源：http://ddk.zhaomingkeji.xyz

df -h;  du -sh *
来源：http://fgd.bjfxy.top

[R62] 找最占空间的文件
来源：http://bjr.wangshuangyany.cn

du -ah . | sort -rh | head -10
来源：http://mhf.quarkkingdee.top

[R63] 内存与进程
来源：http://ncq.zhengqikj.top

free -h;  ps aux | grep nginx
来源：http://vts.wangdashe.top

[R64] 结束进程
来源：http://tar.yongpay.top

kill -9 $(pgrep -f app.py)
来源：http://ekf.nwbrower.top

[R65] 查看端口占用
来源：http://hfa.jianghu66.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dcu.zycfv.cn

[R66] 定时任务
来源：http://jao.fktsv.cn

crontab -e;  crontab -l
来源：http://pul.shangyingyoupin.top

[R67] 生成随机十六进制串
来源：http://xch.cqqwz.cn

openssl rand -hex 16
来源：http://hzo.cqqwz.cn

[R68] 计算文件校验值
来源：http://ltg.daxiang520.top

sha256sum a.txt;  md5sum a.txt
来源：http://yoo.c1oappe.top

[R69] 生成随机密码
来源：http://ymm.shanyushiyangkeji.top

head -c 16 /dev/urandom | base64
来源：http://ybf.shuidangran.top

[R70] 时间戳与互转
来源：http://blx.yangfankeji.com

date +%s;  date -d @1700000000
来源：http://jhf.aibaodan.cn

[R71] 日期格式化
来源：http://lxx.tianlin.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://xbo.shanyushiyangkeji.top

[R72] 等待端口就绪
来源：http://hhc.xuanzx.com

until nc -z localhost 3306; do sleep 1; done
来源：http://eoo.tanke756.top

[R73] 分割大日志
来源：http://bbs.yfazqb.com

split -l 1000 big.log part_
来源：http://fbt.xylfe.cn

[R74] 批量重命名
来源：http://juz.cashguo.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://icb.aibaodan.cn

[R75] 导出环境变量
来源：http://bkl.yfazqb.com

export PATH="$HOME/bin:$PATH"
来源：http://lkb.yanxiufei.cn

[R76] 使用临时文件
来源：http://ike.ywan-chungtsiang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jmd.sjlbkw.cn

[R77] 读取用户输入
来源：http://fbk.cqqwz.cn

read -rp "请输入: " ans
来源：http://lhm.aizwys.cn

[R78] 交互式菜单
来源：http://mur.zhoulong.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://gql.feifeiyinyue.top

[R79] 解析命令行选项
来源：http://pmt.yj20258.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zup.ydjk.org.cn

[R80] 查看脚本执行耗时
来源：http://dca.gaohongyu789.top

time ./run.sh
来源：http://wfw.0kj1m.cn

================================================================================
来源：http://brl.tianlin.xyz

S. C / C++ 专题
来源：http://lmy.yvedp.cn

================================================================================
来源：http://ody.shangyingyoupin.top

[S01] C：Hello World
来源：http://auz.shangyingyoupin.top

#include <stdio.h>
来源：http://jyu.xziqi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qsk.gotoacloud.top

[S02] C：变量与格式化输出
来源：http://kzj.vqdsnc.cn

int a = 10; printf("%d\n", a);
来源：http://gqr.uphjek.com

[S03] C：读入整数
来源：http://yru.guowangkeji.top

int x; scanf("%d", &x);
来源：http://bgz.feifeiyinyue.top

[S04] C：字符串复制
来源：http://ftr.sjlbkw.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hfe.vqdsnc.cn

[S05] C：字符串长度
来源：http://mfk.chenjidiqi.icu

strlen(s)
来源：http://gwi.dianchejie.cn

[S06] C：字符串比较
来源：http://kyl.xingfuxueyuan.xyz

strcmp(a, b) == 0
来源：http://dkj.tanke756.top

[S07] C：数组遍历求和
来源：http://yws.ivvv.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iio.xuanzx.com

[S08] C：动态内存分配与释放
来源：http://xwq.jinqigufen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://udf.nanxuanxn.top

[S09] C：结构体定义与初始化
来源：http://uoi.vqdsnc.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://itj.yongpay.top

[S10] C：指针与解引用
来源：http://vpc.hywenlv.cn

int *p = &a;  *p = 5;
来源：http://dfs.chenzaomai.com

[S11] C：逐行读文件
来源：http://rzy.tianlin.xyz

FILE *f = fopen("a.txt", "r");
来源：http://hdx.redwolf501.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://gjz.xuetiantiany.cn

fclose(f);
来源：http://khx.ydzc1.top

[S12] C：写文件
来源：http://mbp.daria6918.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gfc.shuidangran.top

[S13] C：宏定义
来源：http://dwf.jinqigfzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yce.gogol.net.cn

[S14] C：枚举
来源：http://lum.dianchejie.cn

enum Color { RED, GREEN, BLUE };
来源：http://ldj.zhixingplan.top

[S15] C：类型转换
来源：http://ehu.shanyushiyangkeji.top

(double) a / b
来源：http://lny.redwolf501.top

[S16] C：位操作置位
来源：http://ycd.bjfxy.top

x |= (1 << 3);
来源：http://koh.ydjk.org.cn

[S17] C：安全拼接字符串
来源：http://uke.bbcook.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cui.hysaishi.cn

[S18] C：命令行参数
来源：http://ofs.sxryk.cn

int main(int argc, char **argv)
来源：http://ylt.yuxming.cn

[S19] C：快速排序
来源：http://tfl.redwolf501.top

qsort(a, n, sizeof(int), cmp);
来源：http://jjf.hnxiangtu.top

[S20] C：二分查找
来源：http://yci.tianlin.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hqx.gaohongyu789.top

[S21] C：字符类别判断
来源：http://dot.gaohongyu789.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ild.meibo888.top

[S22] C：字符串转数字
来源：http://dds.iojbl.cn

atoi("42");  strtod("3.14", NULL);
来源：http://efw.bbcook.cn

[S23] C：随机数
来源：http://enj.tarul.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://luy.zhiwuduotai.top

[S24] C：获取本地时间
来源：http://aww.redwolf501.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kto.jinghuilouyu.cn

[S25] C：内存拷贝
来源：http://nmf.cashguo.top

memcpy(dst, src, n);
来源：http://fnj.cheryme.top

[S26] C：内存清零
来源：http://rkq.jinqigufen.top

memset(a, 0, sizeof a);
来源：http://pom.yfazqb.com

[S27] C：定义常量
来源：http://zoe.fzhhl.top

const double PI = 3.14159;
来源：http://dlj.cucudq.cn

[S28] C：静态变量
来源：http://eve.xingfuxueyuan.xyz

static int counter = 0;
来源：http://ppw.bjfxy.top

[S29] C：变参函数
来源：http://bup.bjfxy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jux.mhx1999.top

[S30] C：头文件保护
来源：http://ami.sxryk.cn

#ifndef X_H
来源：http://ayd.dashuyun.cn

#define X_H
来源：http://txw.sweek.top

#endif
来源：http://tth.yvedp.cn

[S31] C++：Hello World
来源：http://wit.yangfankeji.com

#include <iostream>
来源：http://pzk.tianlin.xyz

int main() { std::cout << "Hello\n"; }
来源：http://ecn.gotoacloud.top

[S32] C++：字符串
来源：http://rli.snrcjt.cn

std::string s = "hi";  s += "!";
来源：http://ssn.bbcook.cn

[S33] C++：vector 增删
来源：http://lyq.dashuyun.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wfs.uphjek.com

[S34] C++：遍历 vector
来源：http://ytc.cucudq.cn

for (auto &x : v) { std::cout << x; }
来源：http://hkh.redwolf501.top

[S35] C++：map
来源：http://dwa.jinyuanbaomall.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://aqz.fengsongda.top

[S36] C++：unordered_map
来源：http://wpi.jianghu66.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://avp.shanyushiyangkeji.top

[S37] C++：set
来源：http://nhs.jinghuilouyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bhq.tarul.cn

[S38] C++：排序
来源：http://hqv.jianghu66.top

std::sort(v.begin(), v.end());
来源：http://coi.ctjpmb.com

[S39] C++：自定义比较器排序
来源：http://sia.bjfxy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mpy.cdnleiting.top

[S40] C++：查找元素
来源：http://bsu.shanyushiyangtech.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xqz.zhixingplan.top

[S41] C++：类与构造函数
来源：http://via.jyoumei.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://som.jinghuilouyu.cn

[S42] C++：继承与虚函数
来源：http://qii.feifeiyinyue.top

class B : public Base { public: void f() override {} };
来源：http://elu.zhixingplan.top

[S43] C++：智能指针
来源：http://uxb.sweek.top

auto p = std::make_unique<int>(5);
来源：http://gml.xylfe.cn

[S44] C++：引用传参
来源：http://zjd.jiagoushi.top

void inc(int &x) { ++x; }
来源：http://iln.redwolf501.top

[S45] C++：lambda
来源：http://zko.sjlbkw.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tee.gaohongyu789.top

[S46] C++：函数模板
来源：http://dlc.smart0.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://not.52xcode.cn

[S47] C++：结构化绑定遍历
来源：http://iql.ctjpmb.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mhm.epnwcf.com

[S48] C++：逐行读文件
来源：http://mat.sufxvd.cn

std::ifstream in("a.txt");  std::string line;
来源：http://haz.shangyingyoupin.top

while (std::getline(in, line)) { }
来源：http://bdx.quarkkingdee.top

[S49] C++：写文件
来源：http://vnt.ydjk.org.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://okl.bjfxy.top

[S50] C++：格式化数字
来源：http://rpz.uphjek.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gvu.yuxming.cn

[S51] C++：显式类型转换
来源：http://xbp.mhx1999.top

static_cast<double>(a) / b
来源：http://buw.hammf.cn

[S52] C++：const 与 noexcept
来源：http://dfx.hfpthk.cn

int size() const noexcept { return n_; }
来源：http://dzs.fktsv.cn

[S53] C++：移动语义
来源：http://zhh.ctjpmb.com

std::vector<int> w = std::move(v);
来源：http://axh.xuetiantiany.cn

[S54] C++：异常处理
来源：http://nbw.xziqi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uoi.feifeiyinyue.top

[S55] C++：结构化绑定
来源：http://yis.sjlbkw.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://grv.fengsongda.top

[S56] C++：optional
来源：http://dsg.vehdjk.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://skz.sysykeji.top

[S57] C++：编译期常量
来源：http://bgz.fktsv.cn

constexpr int N = 10;
来源：http://aza.9152youxi.cn

[S58] C++：命名空间
来源：http://dft.ppjwa.cn

namespace ns { int f() { return 1; } }
来源：http://hhy.fzhhl.top

[S59] C++：静态断言
来源：http://wbh.ppjwa.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uvn.ctjpmb.com

[S60] C++：遍历并删除元素
来源：http://fms.jinqigufen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://afz.sweek.top

================================================================================
来源：http://dpg.iojbl.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cge.shangyingyoupin.top

================================================================================
来源：http://lap.fzhhl.top

[T01] Kotlin：Hello World
来源：http://gct.316326.xyz

println("Hello")
来源：http://elx.meibo888.top

[T02] Kotlin：变量
来源：http://ryd.meibo888.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hgj.xziqi.cn

[T03] Kotlin：字符串模板
来源：http://mea.jqgfzy.top

"值: $b"
来源：http://cfu.aizwys.cn

[T04] Kotlin：空安全
来源：http://mta.gaohongyu789.top

val n: String? = null;  n?.length
来源：http://wwz.jyoumei.cn

[T05] Kotlin：when 表达式
来源：http://lqz.xingfuxueyuan.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://van.nanxuanxn.top

[T06] Kotlin：集合映射
来源：http://qsi.ctjpmb.com

listOf(1, 2, 3).map { it * 2 }
来源：http://zrm.quarkkingdee.top

[T07] Kotlin：集合过滤
来源：http://asu.zdbjq.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xgl.hongshengwenyu.top

[T08] Kotlin：数据类
来源：http://dsf.ydzc1.top

data class User(val name: String, val age: Int)
来源：http://qhr.smart0.xyz

[T09] Kotlin：扩展函数
来源：http://zst.cqqwz.cn

fun String.exclaim() = this + "!"
来源：http://qox.sjlbkw.cn

[T10] Kotlin：默认参数
来源：http://cyb.mhx1999.top

fun greet(name: String = "World") = "Hi $name"
来源：http://rkj.tian-w.cn

[T11] Kotlin：协程
来源：http://tgi.tianlin.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://nqh.fktsv.cn

[T12] Kotlin：解构声明
来源：http://uij.hywenlv.cn

val (a, b) = Pair(1, 2)
来源：http://iqp.fehbvm.com

[T13] Kotlin：只读 Map
来源：http://rrz.yonumen.top

val m = mapOf("a" to 1)
来源：http://fpm.yongpay.top

[T14] Kotlin：循环
来源：http://nap.jinyuanbaomall.cn

for (i in 1..10) println(i)
来源：http://crs.gzhubu.top

[T15] Kotlin：接口
来源：http://bnu.jinqigfzy.top

interface Shape { fun area(): Double }
来源：http://via.zhengqikj.top

[T16] Swift：Hello World
来源：http://kpf.52xcode.cn

print("Hello")
来源：http://twe.shzxlz.cn

[T17] Swift：变量与常量
来源：http://pql.sysykeji.top

var a = 1;  let b = 2
来源：http://eyb.9152youxi.cn

[T18] Swift：字符串插值
来源：http://scq.zycfv.cn

"值: \(b)"
来源：http://uvz.tianlin.xyz

[T19] Swift：可选绑定
来源：http://uyd.0kj1m.cn

if let n = opt { print(n) }
来源：http://neg.yangfankeji.com

[T20] Swift：数组操作
来源：http://eno.ivvv.top

var a = [1, 2, 3];  a.append(4)
来源：http://wcg.ehwqpu.com

[T21] Swift：遍历
来源：http://hap.kuanghao11.cn

for x in a { print(x) }
来源：http://uqi.haohaochexian.top

[T22] Swift：字典
来源：http://thm.jinqigufen.top

var d = ["a": 1];  d["b"] = 2
来源：http://fob.havefunace.top

[T23] Swift：函数
来源：http://vts.zhengqikj.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wdr.zhiwuduotai.top

[T24] Swift：闭包
来源：http://ohr.chenlongwang.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ene.kuanghao11.cn

[T25] Swift：结构体
来源：http://ddc.xingfuxueyuan.xyz

struct P { var x: Int }
来源：http://ajk.sufxvd.cn

[T26] Swift：类与重写
来源：http://hwb.fehbvm.com

class A: Base { override func f() {} }
来源：http://mvm.chenjidiqi.icu

[T27] Swift：错误处理
来源：http://ydu.fktsv.cn

do { try f() } catch { print(error) }
来源：http://qnt.shanyushiyangkeji.top

[T28] Swift：枚举
来源：http://xvv.zhiwuduotai.top

enum Color { case red, green }
来源：http://eym.yueranfly.top

[T29] Swift：guard 提前返回
来源：http://vgs.yj20258888.top

guard let x = opt else { return }
来源：http://sgm.c1oappe.top

[T30] Swift：协议
来源：http://yym.ydzc1.top

protocol Shape { func area() -> Double }
来源：http://the.ydzc1.top

[T31] Lua：Hello World
来源：http://tjv.guannengcc.top

print("Hello")
来源：http://scx.zycfv.cn

[T32] Lua：局部变量
来源：http://apr.ivvv.top

local a = 1
来源：http://zns.tianlin.xyz

[T33] Lua：表（数组）
来源：http://jjd.jlsjyb.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wct.jqgufenzy.top

[T34] Lua：遍历表
来源：http://oxh.xuanzx.com

for i, v in ipairs(t) do print(i, v) end
来源：http://qwi.hnqzz.top

[T35] Lua：字典表
来源：http://nzf.tarul.cn

local d = { a = 1 };  d.b = 2
来源：http://coh.dianchejie.cn

[T36] Lua：函数
来源：http://fot.ybcxt.top

function add(a, b) return a + b end
来源：http://dht.pengpengdd.cyou

[T37] Lua：字符串拼接
来源：http://grb.wangdashe.top

"a" .. "b"
来源：http://qhb.0kj1m.cn

[T38] Lua：条件
来源：http://qdr.ywan-chungtsiang.top

if x > 0 then print("正") end
来源：http://yvn.zhixingplan.top

[T39] Lua：模式匹配
来源：http://ske.hnqzz.top

string.find(s, "%d+")
来源：http://wmo.ybcxt.top

[T40] Lua：元表
来源：http://qnl.vqdsnc.cn

setmetatable({}, { __index = base })
来源：http://dkm.wangshuangyany.cn

[T41] Perl：Hello World
来源：http://tpy.dashuyun.cn

print "Hello\n";
来源：http://jdl.jlsjyb.cn

[T42] Perl：变量类型
来源：http://jta.guowangkeji.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kpv.jlsjyb.cn


<!-- 参考信息 -->