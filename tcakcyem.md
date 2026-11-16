代发 wailian999

cmd > out.log 2>&1
来源：http://ygh.yonumen.top

[R40] 追加写日志
来源：http://atc.jinghuilouyu.cn

echo "log" >> out.log
来源：http://yev.hesvh.cn

[R41] 丢弃输出
来源：http://tkk.cucudq.cn

cmd >/dev/null 2>&1
来源：http://xfm.ydzc1.top

[R42] 输入重定向
来源：http://dip.dashuyun.cn

wc -l < a.txt
来源：http://jpg.ywan-chungtsiang.top

[R43] 按名字查找文件
来源：http://zlb.aizwys.cn

find . -name "*.log" -type f
来源：http://vmw.xylfe.cn

[R44] 按修改时间查找
来源：http://mcf.shzxlz.cn

find . -mtime -7 -type f
来源：http://tnv.feifeiyinyue.top

[R45] 批量删除
来源：http://dup.guannengcc.top

find . -name "*.tmp" -delete
来源：http://hwx.ehwqpu.com

[R46] 递归替换文件内容
来源：http://zlc.ivvv.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qcb.shuidangran.top

[R47] sed 单行替换
来源：http://ixm.hammf.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mph.gogol.net.cn

[R48] awk 取指定列
来源：http://mgq.nanxinkj.top

awk '{print $1, $3}' a.txt
来源：http://yok.cqqwz.cn

[R49] awk 带条件
来源：http://kfb.wangdashe.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pqf.hywenlv.cn

[R50] awk 求和
来源：http://kkm.cdnleiting.top

awk '{s += $2} END {print s}' a.txt
来源：http://uxe.shanyushiyangkeji.top

[R51] 排序去重取前几
来源：http://mxl.jqgfzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://vil.birdmap.top

[R52] 统计行数
来源：http://bpz.gogol.net.cn

wc -l a.txt
来源：http://ump.yj20258888.top

[R53] 查看文件头与实时尾
来源：http://brh.sxryk.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tjg.ppjwa.cn

[R54] 比较两个文件
来源：http://rkg.yuxming.cn

diff a.txt b.txt
来源：http://kfk.yj20258.top

[R55] 压缩与解压
来源：http://llu.cqqwz.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dff.cdnleiting.top

[R56] 远程拷贝
来源：http://qse.guannengcc.top

scp file user@host:/path/
来源：http://mep.jinyuanbaomall.cn

[R57] 远程执行命令
来源：http://mjn.bjfxy.top

ssh user@host 'uptime'
来源：http://hev.xingfuxueyuan.xyz

[R58] 下载文件
来源：http://aor.sweek.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://glu.sysykeji.top

[R59] 发 POST JSON
来源：http://yxa.xinyue.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jve.xylfe.cn

[R60] 只看 HTTP 状态码
来源：http://vgn.sysykeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://upy.yuxming.cn

[R61] 磁盘占用
来源：http://rzx.jlsjyb.cn

df -h;  du -sh *
来源：http://jfx.feifeiyinyue.top

[R62] 找最占空间的文件
来源：http://wyu.mhx1999.top

du -ah . | sort -rh | head -10
来源：http://zrk.epnwcf.com

[R63] 内存与进程
来源：http://gqi.xuetiantiany.cn

free -h;  ps aux | grep nginx
来源：http://mno.gaohongyu789.top

[R64] 结束进程
来源：http://fbp.yj20258888.top

kill -9 $(pgrep -f app.py)
来源：http://etz.bbcook.cn

[R65] 查看端口占用
来源：http://xag.ehwqpu.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://okc.zhixingplan.top

[R66] 定时任务
来源：http://knp.hcnkem.com

crontab -e;  crontab -l
来源：http://lno.316326.xyz

[R67] 生成随机十六进制串
来源：http://wlm.guowangkeji.top

openssl rand -hex 16
来源：http://hvq.sxryk.cn

[R68] 计算文件校验值
来源：http://qbj.hnqzz.top

sha256sum a.txt;  md5sum a.txt
来源：http://pio.chenjidiqi.icu

[R69] 生成随机密码
来源：http://xkd.52xcode.cn

head -c 16 /dev/urandom | base64
来源：http://cra.smart0.xyz

[R70] 时间戳与互转
来源：http://yur.yanxiufei.cn

date +%s;  date -d @1700000000
来源：http://zom.hcnkem.com

[R71] 日期格式化
来源：http://wqz.hesvh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ltj.daria6918.cn

[R72] 等待端口就绪
来源：http://toc.sxryk.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://blx.sxryk.cn

[R73] 分割大日志
来源：http://beh.jianghu66.top

split -l 1000 big.log part_
来源：http://quy.yj202588.top

[R74] 批量重命名
来源：http://dtj.aizwys.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nck.yfazqb.com

[R75] 导出环境变量
来源：http://uug.bjfxy.top

export PATH="$HOME/bin:$PATH"
来源：http://btk.bjfxy.top

[R76] 使用临时文件
来源：http://xpq.cdnleiting.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://riq.tian-w.cn

[R77] 读取用户输入
来源：http://hya.hongshengwenyu.top

read -rp "请输入: " ans
来源：http://gpv.zhengqikj.top

[R78] 交互式菜单
来源：http://agf.hysaishi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lxh.hesvh.cn

[R79] 解析命令行选项
来源：http://hvq.shangyingyoupin.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://apz.chenlongwang.top

[R80] 查看脚本执行耗时
来源：http://zto.hysaishi.cn

time ./run.sh
来源：http://chg.hywenlv.cn

================================================================================
来源：http://iun.zhaomingkeji.xyz

S. C / C++ 专题
来源：http://kif.redwolf501.top

================================================================================
来源：http://xjx.snrcjt.cn

[S01] C：Hello World
来源：http://wny.yj202588.top

#include <stdio.h>
来源：http://yif.vehdjk.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://fpr.gaohongyu789.top

[S02] C：变量与格式化输出
来源：http://qox.ydzc1.top

int a = 10; printf("%d\n", a);
来源：http://ibo.sxryk.cn

[S03] C：读入整数
来源：http://pgg.epnwcf.com

int x; scanf("%d", &x);
来源：http://urd.vqdsnc.cn

[S04] C：字符串复制
来源：http://cni.sweek.top

char dst[32]; strcpy(dst, "hi");
来源：http://ibd.nanxinkj.top

[S05] C：字符串长度
来源：http://fps.ctjpmb.com

strlen(s)
来源：http://acc.fengsongda.top

[S06] C：字符串比较
来源：http://von.nanxuanxn.top

strcmp(a, b) == 0
来源：http://tlh.hywenlv.cn

[S07] C：数组遍历求和
来源：http://xwe.mhx1999.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yid.nanxuanxn.top

[S08] C：动态内存分配与释放
来源：http://rbg.daria6918.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kqz.zhijiandao.cn

[S09] C：结构体定义与初始化
来源：http://kug.tarul.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pkz.haohaochexian.top

[S10] C：指针与解引用
来源：http://iib.daxiang520.top

int *p = &a;  *p = 5;
来源：http://akh.yongpay.top

[S11] C：逐行读文件
来源：http://dgx.fktsv.cn

FILE *f = fopen("a.txt", "r");
来源：http://gqi.fktsv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hif.9152youxi.cn

fclose(f);
来源：http://ccq.zhoulong.xyz

[S12] C：写文件
来源：http://hbd.tianlin.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nzt.c1oappe.top

[S13] C：宏定义
来源：http://lnn.zhengqikj.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wqi.yuanzhike.top

[S14] C：枚举
来源：http://wyz.wangdashe.top

enum Color { RED, GREEN, BLUE };
来源：http://fyq.sufxvd.cn

[S15] C：类型转换
来源：http://qzm.sysykeji.top

(double) a / b
来源：http://nee.cashguo.top

[S16] C：位操作置位
来源：http://ukn.xuetiantiany.cn

x |= (1 << 3);
来源：http://ync.vqdsnc.cn

[S17] C：安全拼接字符串
来源：http://gzv.jlsjyb.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://aix.nanxuanxn.top

[S18] C：命令行参数
来源：http://vpo.zhengqikj.top

int main(int argc, char **argv)
来源：http://ydk.feifeiyinyue.top

[S19] C：快速排序
来源：http://wgn.cdnleiting.top

qsort(a, n, sizeof(int), cmp);
来源：http://sdg.xylfe.cn

[S20] C：二分查找
来源：http://pzn.hywenlv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ypt.jqgufenzy.top

[S21] C：字符类别判断
来源：http://mhk.yuxming.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qie.shanyushiyangtech.top

[S22] C：字符串转数字
来源：http://sqq.svipenyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nww.gogol.net.cn

[S23] C：随机数
来源：http://dsd.fanxiaobao.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://qdf.shanyushiyangkeji.top

[S24] C：获取本地时间
来源：http://jjo.snrcjt.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kxl.snrcjt.cn

[S25] C：内存拷贝
来源：http://cje.gotoacloud.top

memcpy(dst, src, n);
来源：http://ylm.shangyingyoupin.top

[S26] C：内存清零
来源：http://sbz.xuanzx.com

memset(a, 0, sizeof a);
来源：http://kku.epnwcf.com

[S27] C：定义常量
来源：http://ogq.snrcjt.cn

const double PI = 3.14159;
来源：http://frl.jinghuilouyu.cn

[S28] C：静态变量
来源：http://rlj.uphjek.com

static int counter = 0;
来源：http://tds.vehdjk.com

[S29] C：变参函数
来源：http://ios.zhaomingkeji.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nyg.aizwys.cn

[S30] C：头文件保护
来源：http://hwl.tian-w.cn

#ifndef X_H
来源：http://ysw.yj20258.top

#define X_H
来源：http://zro.yueranfly.top

#endif
来源：http://sgr.shzxlz.cn

[S31] C++：Hello World
来源：http://cjv.shanyushiyangkeji.top

#include <iostream>
来源：http://zlp.xuetiantiany.cn

int main() { std::cout << "Hello\n"; }
来源：http://jwd.jinyuanbaomall.cn

[S32] C++：字符串
来源：http://rnh.bjfxy.top

std::string s = "hi";  s += "!";
来源：http://ars.daxiang520.top

[S33] C++：vector 增删
来源：http://uqb.cqqwz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ylw.sjlbkw.cn

[S34] C++：遍历 vector
来源：http://dyv.jlsjyb.cn

for (auto &x : v) { std::cout << x; }
来源：http://exn.nanxinkj.top

[S35] C++：map
来源：http://ffn.svipenyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ldb.shanyushiyangkeji.top

[S36] C++：unordered_map
来源：http://dsf.shanyushiyangtech.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pjo.hesvh.cn

[S37] C++：set
来源：http://apa.iojbl.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nok.jlsjyb.cn

[S38] C++：排序
来源：http://sdo.hysaishi.cn

std::sort(v.begin(), v.end());
来源：http://peb.ehwqpu.com

[S39] C++：自定义比较器排序
来源：http://evv.xylfe.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zhk.hywenlv.cn

[S40] C++：查找元素
来源：http://kqx.9152youxi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cvc.hammf.cn

[S41] C++：类与构造函数
来源：http://aqg.havefunace.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ilj.zhongyouzk.top

[S42] C++：继承与虚函数
来源：http://vam.hysaishi.cn

class B : public Base { public: void f() override {} };
来源：http://kxk.feifeiyinyue.top

[S43] C++：智能指针
来源：http://qoy.chenzaomai.com

auto p = std::make_unique<int>(5);
来源：http://rrg.jiagoushi.top

[S44] C++：引用传参
来源：http://ivm.ydzc1.top

void inc(int &x) { ++x; }
来源：http://xyl.fengsongda.top

[S45] C++：lambda
来源：http://ane.cashguo.top

auto add = [](int a, int b) { return a + b; };
来源：http://kgo.havefunace.top

[S46] C++：函数模板
来源：http://jxs.jinqigufen.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://udz.zhiwuduotai.top

[S47] C++：结构化绑定遍历
来源：http://srn.tanke756.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dri.uphjek.com

[S48] C++：逐行读文件
来源：http://wnm.jinqigufen.top

std::ifstream in("a.txt");  std::string line;
来源：http://zqn.zdbjq.cn

while (std::getline(in, line)) { }
来源：http://ibp.zhiwuduotai.top

[S49] C++：写文件
来源：http://mkf.vqdsnc.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://akf.shanyushiyangkeji.top

[S50] C++：格式化数字
来源：http://ual.cdnleiting.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rms.316326.xyz

[S51] C++：显式类型转换
来源：http://hwv.yangfankeji.com

static_cast<double>(a) / b
来源：http://llp.jqgufenzy.top

[S52] C++：const 与 noexcept
来源：http://rcb.ctjpmb.com

int size() const noexcept { return n_; }
来源：http://omm.jqgufenzy.top

[S53] C++：移动语义
来源：http://xuz.jinqigufen.top

std::vector<int> w = std::move(v);
来源：http://vhu.shanyushiyangtech.top

[S54] C++：异常处理
来源：http://auu.zycfv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pcl.daria6918.cn

[S55] C++：结构化绑定
来源：http://vop.guowangkeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://xfl.havefunace.top

[S56] C++：optional
来源：http://wdt.wangdashe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eqy.smart0.xyz

[S57] C++：编译期常量
来源：http://uev.mhx1999.top

constexpr int N = 10;
来源：http://ocf.aizwys.cn

[S58] C++：命名空间
来源：http://jzf.haohaochexian.top

namespace ns { int f() { return 1; } }
来源：http://dqv.uphjek.com

[S59] C++：静态断言
来源：http://joz.zhoulong.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yfu.bjfxy.top

[S60] C++：遍历并删除元素
来源：http://uvg.sysykeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ngx.tianlin.xyz

================================================================================
来源：http://len.tanke756.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ood.yj20258.top

================================================================================
来源：http://gsp.ydzc1.top

[T01] Kotlin：Hello World
来源：http://yuq.fktsv.cn

println("Hello")
来源：http://bzj.sysykeji.top

[T02] Kotlin：变量
来源：http://apu.sysykeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://czt.zhijiandao.cn

[T03] Kotlin：字符串模板
来源：http://eko.0kj1m.cn

"值: $b"
来源：http://cbx.pengpengdd.cyou

[T04] Kotlin：空安全
来源：http://jxk.cucudq.cn

val n: String? = null;  n?.length
来源：http://lno.yj202588.top

[T05] Kotlin：when 表达式
来源：http://gks.dianchejie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tze.fanxiaobao.xyz

[T06] Kotlin：集合映射
来源：http://vdu.ehwqpu.com

listOf(1, 2, 3).map { it * 2 }
来源：http://efv.yj20258888.top

[T07] Kotlin：集合过滤
来源：http://ahf.hysaishi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bwm.hongshengwenyu.top

[T08] Kotlin：数据类
来源：http://jfz.hnxiangtu.top

data class User(val name: String, val age: Int)
来源：http://pey.wangshuangyany.cn

[T09] Kotlin：扩展函数
来源：http://fep.gzhubu.top

fun String.exclaim() = this + "!"
来源：http://wuk.snrcjt.cn

[T10] Kotlin：默认参数
来源：http://yas.wangshuangyany.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uxm.daxiang520.top

[T11] Kotlin：协程
来源：http://fhy.yonumen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://dmp.sysykeji.top

[T12] Kotlin：解构声明
来源：http://cdi.gotoacloud.top

val (a, b) = Pair(1, 2)
来源：http://vju.cucudq.cn

[T13] Kotlin：只读 Map
来源：http://lix.yfazqb.com

val m = mapOf("a" to 1)
来源：http://nyl.yj202588.top

[T14] Kotlin：循环
来源：http://dzk.fzhhl.top

for (i in 1..10) println(i)
来源：http://cnj.epnwcf.com

[T15] Kotlin：接口
来源：http://erg.quarkkingdee.top

interface Shape { fun area(): Double }
来源：http://gme.yonumen.top

[T16] Swift：Hello World
来源：http://cbr.9152youxi.cn

print("Hello")
来源：http://kjb.fehbvm.com

[T17] Swift：变量与常量
来源：http://wvy.wangshuangyany.cn

var a = 1;  let b = 2
来源：http://ygq.9152youxi.cn

[T18] Swift：字符串插值
来源：http://wav.zhaomingkeji.xyz

"值: \(b)"
来源：http://oqt.jiagoushi.top

[T19] Swift：可选绑定
来源：http://kbk.sysykeji.top

if let n = opt { print(n) }
来源：http://bdt.iojbl.cn

[T20] Swift：数组操作
来源：http://kbp.tian-w.cn

var a = [1, 2, 3];  a.append(4)
来源：http://avj.hywenlv.cn

[T21] Swift：遍历
来源：http://oue.ybcxt.top

for x in a { print(x) }
来源：http://jkb.zhongyouzk.top

[T22] Swift：字典
来源：http://orn.sysykeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://kfs.yvedp.cn

[T23] Swift：函数
来源：http://spz.hnqzz.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ost.dianchejie.cn

[T24] Swift：闭包
来源：http://qdd.redwolf501.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://mso.ivvv.top

[T25] Swift：结构体
来源：http://lwu.yongpay.top

struct P { var x: Int }
来源：http://mmy.cheryme.top

[T26] Swift：类与重写
来源：http://int.cdnleiting.top

class A: Base { override func f() {} }
来源：http://byx.fanxiaobao.xyz

[T27] Swift：错误处理
来源：http://qtn.tanke756.top

do { try f() } catch { print(error) }
来源：http://bir.jqgufenzy.top

[T28] Swift：枚举
来源：http://blr.hysaishi.cn

enum Color { case red, green }
来源：http://hdp.gaohongyu789.top

[T29] Swift：guard 提前返回
来源：http://cbs.bjfxy.top

guard let x = opt else { return }
来源：http://yoi.yanxiufei.cn

[T30] Swift：协议
来源：http://nyg.sufxvd.cn

protocol Shape { func area() -> Double }
来源：http://lcg.nanxinkj.top

[T31] Lua：Hello World
来源：http://cxf.fengsongda.top

print("Hello")
来源：http://yvb.shanyushiyangkeji.top

[T32] Lua：局部变量
来源：http://mlw.uphjek.com

local a = 1
来源：http://agr.hcnkem.com

[T33] Lua：表（数组）
来源：http://swo.redwolf501.top

local t = {1, 2, 3};  t[4] = 4
来源：http://znv.hnxiangtu.top

[T34] Lua：遍历表
来源：http://ept.jlsjyb.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qes.sufxvd.cn

[T35] Lua：字典表
来源：http://ruq.yvedp.cn

local d = { a = 1 };  d.b = 2
来源：http://ozq.pycfn.com

[T36] Lua：函数
来源：http://ejr.yanxiufei.cn

function add(a, b) return a + b end
来源：http://qpq.shanyushiyangkeji.top

[T37] Lua：字符串拼接
来源：http://tia.cashguo.top

"a" .. "b"
来源：http://skv.dianchejie.cn

[T38] Lua：条件
来源：http://owq.gzhubu.top

if x > 0 then print("正") end
来源：http://prk.xuanzx.com

[T39] Lua：模式匹配
来源：http://zsr.yvedp.cn

string.find(s, "%d+")
来源：http://cor.aizwys.cn

[T40] Lua：元表
来源：http://bcq.zhoulong.xyz

setmetatable({}, { __index = base })
来源：http://tsl.zdqjudy.top

[T41] Perl：Hello World
来源：http://udf.daxiang520.top

print "Hello\n";
来源：http://tbd.yj20258888.top

[T42] Perl：变量类型
来源：http://rqg.ctjpmb.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wch.shangyingyoupin.top


<!-- 参考信息 -->