代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://lsm.ydzc1.top

[R36] 并发执行多个任务
来源：http://tfw.chenzaomai.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zwl.zycfv.cn

[R37] 把输出赋给变量
来源：http://zgp.zdbjq.cn

files=$(ls -1)
来源：http://ouy.haohaochexian.top

[R38] 管道串联
来源：http://oey.daxiang520.top

cat a.txt | grep -i error | wc -l
来源：http://ntf.hywenlv.cn

[R39] 重定向标准输出与错误
来源：http://wyi.kuanghao11.cn

cmd > out.log 2>&1
来源：http://vqn.pycfn.com

[R40] 追加写日志
来源：http://pfu.birdmap.top

echo "log" >> out.log
来源：http://izw.hongshengwenyu.top

[R41] 丢弃输出
来源：http://cyp.svipenyu.cn

cmd >/dev/null 2>&1
来源：http://mpd.yfazqb.com

[R42] 输入重定向
来源：http://vko.cucudq.cn

wc -l < a.txt
来源：http://hor.quarkkingdee.top

[R43] 按名字查找文件
来源：http://xsi.guowangkeji.top

find . -name "*.log" -type f
来源：http://zed.ppjwa.cn

[R44] 按修改时间查找
来源：http://pfd.zhengqikj.top

find . -mtime -7 -type f
来源：http://owh.xuanzx.com

[R45] 批量删除
来源：http://bgh.ivvv.top

find . -name "*.tmp" -delete
来源：http://dtk.jinghuilouyu.cn

[R46] 递归替换文件内容
来源：http://iih.xziqi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qrb.tarul.cn

[R47] sed 单行替换
来源：http://hew.xuanzx.com

sed -i 's/foo/bar/g' a.txt
来源：http://uea.nanxinkj.top

[R48] awk 取指定列
来源：http://aay.fanxiaobao.xyz

awk '{print $1, $3}' a.txt
来源：http://ojl.fengsongda.top

[R49] awk 带条件
来源：http://ehr.ywan-chungtsiang.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bzs.hfpthk.cn

[R50] awk 求和
来源：http://tyh.svipenyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xti.yj20258.top

[R51] 排序去重取前几
来源：http://csa.fktsv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fyd.vehdjk.com

[R52] 统计行数
来源：http://jtw.kuanghao11.cn

wc -l a.txt
来源：http://xsu.cheryme.top

[R53] 查看文件头与实时尾
来源：http://qsp.aizwys.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ear.cucudq.cn

[R54] 比较两个文件
来源：http://olo.yanxiufei.cn

diff a.txt b.txt
来源：http://pqf.uphjek.com

[R55] 压缩与解压
来源：http://fcz.yvedp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://via.sweek.top

[R56] 远程拷贝
来源：http://olt.ybcxt.top

scp file user@host:/path/
来源：http://cpg.sufxvd.cn

[R57] 远程执行命令
来源：http://qyh.xuanzx.com

ssh user@host 'uptime'
来源：http://lyo.vehdjk.com

[R58] 下载文件
来源：http://eaj.sysykeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ysw.hywenlv.cn

[R59] 发 POST JSON
来源：http://xjk.dianchejie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nkd.haohaochexian.top

[R60] 只看 HTTP 状态码
来源：http://dfy.fktsv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dga.jianghu66.top

[R61] 磁盘占用
来源：http://wms.hfpthk.cn

df -h;  du -sh *
来源：http://xak.fzhhl.top

[R62] 找最占空间的文件
来源：http://vjo.jqgufenzy.top

du -ah . | sort -rh | head -10
来源：http://qtw.yj20258888.top

[R63] 内存与进程
来源：http://uzp.cqqwz.cn

free -h;  ps aux | grep nginx
来源：http://fiq.nanxinkj.top

[R64] 结束进程
来源：http://mjj.xziqi.cn

kill -9 $(pgrep -f app.py)
来源：http://xzu.xziqi.cn

[R65] 查看端口占用
来源：http://iqp.uphjek.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mok.vehdjk.com

[R66] 定时任务
来源：http://kxi.jyoumei.cn

crontab -e;  crontab -l
来源：http://xcg.chenzaomai.com

[R67] 生成随机十六进制串
来源：http://nkv.andypj.xyz

openssl rand -hex 16
来源：http://xkd.epnwcf.com

[R68] 计算文件校验值
来源：http://jwa.zhijiandao.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mmj.yj202588.top

[R69] 生成随机密码
来源：http://ken.dianchejie.cn

head -c 16 /dev/urandom | base64
来源：http://wyz.cheryme.top

[R70] 时间戳与互转
来源：http://jmd.zdbjq.cn

date +%s;  date -d @1700000000
来源：http://prs.sufxvd.cn

[R71] 日期格式化
来源：http://mmt.pengpengdd.cyou

date +"%Y-%m-%d %H:%M:%S"
来源：http://agp.gzhubu.top

[R72] 等待端口就绪
来源：http://huv.nanxuanxn.top

until nc -z localhost 3306; do sleep 1; done
来源：http://xli.shanyushiyangkeji.top

[R73] 分割大日志
来源：http://qoz.zhixingplan.top

split -l 1000 big.log part_
来源：http://xdu.daria6918.cn

[R74] 批量重命名
来源：http://tbq.iojbl.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jil.xuanzx.com

[R75] 导出环境变量
来源：http://otm.cashguo.top

export PATH="$HOME/bin:$PATH"
来源：http://zof.jqgufenzy.top

[R76] 使用临时文件
来源：http://otc.xuetiantiany.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tbz.hnxiangtu.top

[R77] 读取用户输入
来源：http://gnr.xingfuxueyuan.xyz

read -rp "请输入: " ans
来源：http://kly.cqqwz.cn

[R78] 交互式菜单
来源：http://epm.wangshuangyany.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lpf.fzhhl.top

[R79] 解析命令行选项
来源：http://oet.ydjk.org.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fxu.0kj1m.cn

[R80] 查看脚本执行耗时
来源：http://oyc.hesvh.cn

time ./run.sh
来源：http://prn.9152youxi.cn

================================================================================
来源：http://syl.yj20258888.top

S. C / C++ 专题
来源：http://mvw.wangdashe.top

================================================================================
来源：http://llw.nanxuanxn.top

[S01] C：Hello World
来源：http://rnq.hnqzz.top

#include <stdio.h>
来源：http://ioj.gaohongyu789.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://byl.chenlongwang.top

[S02] C：变量与格式化输出
来源：http://ltd.daxiang520.top

int a = 10; printf("%d\n", a);
来源：http://ofi.sjlbkw.cn

[S03] C：读入整数
来源：http://inr.birdmap.top

int x; scanf("%d", &x);
来源：http://fzh.ydjk.org.cn

[S04] C：字符串复制
来源：http://dke.shangyingyoupin.top

char dst[32]; strcpy(dst, "hi");
来源：http://vqa.316326.xyz

[S05] C：字符串长度
来源：http://pxu.jianghu66.top

strlen(s)
来源：http://awp.havefunace.top

[S06] C：字符串比较
来源：http://iyv.zhiwuduotai.top

strcmp(a, b) == 0
来源：http://pgu.yuxming.cn

[S07] C：数组遍历求和
来源：http://ojv.bbcook.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://epb.vehdjk.com

[S08] C：动态内存分配与释放
来源：http://rea.hnqzz.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bzf.jyoumei.cn

[S09] C：结构体定义与初始化
来源：http://trc.snrcjt.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cbu.andypj.xyz

[S10] C：指针与解引用
来源：http://lvp.yj202588.top

int *p = &a;  *p = 5;
来源：http://tzt.52xcode.cn

[S11] C：逐行读文件
来源：http://qjr.fanxiaobao.xyz

FILE *f = fopen("a.txt", "r");
来源：http://irz.hywenlv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pak.fktsv.cn

fclose(f);
来源：http://bah.fehbvm.com

[S12] C：写文件
来源：http://fos.jlsjyb.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zfi.daria6918.cn

[S13] C：宏定义
来源：http://xgz.zhongyouzk.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xcn.cdnleiting.top

[S14] C：枚举
来源：http://kpb.cucudq.cn

enum Color { RED, GREEN, BLUE };
来源：http://xtb.sxryk.cn

[S15] C：类型转换
来源：http://qvp.jinyuanbaomall.cn

(double) a / b
来源：http://qqj.gzhubu.top

[S16] C：位操作置位
来源：http://rmq.shuidangran.top

x |= (1 << 3);
来源：http://qqn.shanyushiyangtech.top

[S17] C：安全拼接字符串
来源：http://usu.nwbrower.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zeh.cashguo.top

[S18] C：命令行参数
来源：http://nac.gotoacloud.top

int main(int argc, char **argv)
来源：http://rgs.0kj1m.cn

[S19] C：快速排序
来源：http://crt.fzhhl.top

qsort(a, n, sizeof(int), cmp);
来源：http://acu.snrcjt.cn

[S20] C：二分查找
来源：http://lrl.xinyue.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qwh.jlsjyb.cn

[S21] C：字符类别判断
来源：http://uug.chenjidiqi.icu

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pjl.jinqigfzy.top

[S22] C：字符串转数字
来源：http://bor.52xcode.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vvx.cheryme.top

[S23] C：随机数
来源：http://hww.nanxuanxn.top

srand(time(NULL));  int r = rand() % 100;
来源：http://cvo.jinyuanbaomall.cn

[S24] C：获取本地时间
来源：http://ojw.guowangkeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://itt.haohaochexian.top

[S25] C：内存拷贝
来源：http://vmw.zdbjq.cn

memcpy(dst, src, n);
来源：http://mlk.fktsv.cn

[S26] C：内存清零
来源：http://lag.yangfankeji.com

memset(a, 0, sizeof a);
来源：http://zhe.snrcjt.cn

[S27] C：定义常量
来源：http://pyz.zhaomingkeji.xyz

const double PI = 3.14159;
来源：http://tfq.nanxuanxn.top

[S28] C：静态变量
来源：http://wmt.xylfe.cn

static int counter = 0;
来源：http://tqc.feifeiyinyue.top

[S29] C：变参函数
来源：http://pxn.sxryk.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lov.zhiwuduotai.top

[S30] C：头文件保护
来源：http://dsm.shanyushiyangtech.top

#ifndef X_H
来源：http://jtj.sxryk.cn

#define X_H
来源：http://lam.tanke756.top

#endif
来源：http://bgg.jqgufenzy.top

[S31] C++：Hello World
来源：http://hoy.yanxiufei.cn

#include <iostream>
来源：http://gyb.tian-w.cn

int main() { std::cout << "Hello\n"; }
来源：http://pql.yfazqb.com

[S32] C++：字符串
来源：http://chv.hongshengwenyu.top

std::string s = "hi";  s += "!";
来源：http://cva.316326.xyz

[S33] C++：vector 增删
来源：http://njg.jinqigufen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lqx.hywenlv.cn

[S34] C++：遍历 vector
来源：http://ryu.yongpay.top

for (auto &x : v) { std::cout << x; }
来源：http://owz.hcnkem.com

[S35] C++：map
来源：http://ork.fanxiaobao.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lhl.jinghuilouyu.cn

[S36] C++：unordered_map
来源：http://fqx.nanxinkj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cei.hywenlv.cn

[S37] C++：set
来源：http://ygo.hesvh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kta.guowangkeji.top

[S38] C++：排序
来源：http://qgp.c1oappe.top

std::sort(v.begin(), v.end());
来源：http://yio.yfazqb.com

[S39] C++：自定义比较器排序
来源：http://fnd.52xcode.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ruw.fanxiaobao.xyz

[S40] C++：查找元素
来源：http://xxh.shanyushiyangkeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xmn.wangdashe.top

[S41] C++：类与构造函数
来源：http://mkq.vehdjk.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mxt.shangyingyoupin.top

[S42] C++：继承与虚函数
来源：http://jyv.fzhhl.top

class B : public Base { public: void f() override {} };
来源：http://txo.yueranfly.top

[S43] C++：智能指针
来源：http://pwo.gogol.net.cn

auto p = std::make_unique<int>(5);
来源：http://vmb.fengsongda.top

[S44] C++：引用传参
来源：http://kwu.gogol.net.cn

void inc(int &x) { ++x; }
来源：http://ggk.hywenlv.cn

[S45] C++：lambda
来源：http://fnt.zhixingplan.top

auto add = [](int a, int b) { return a + b; };
来源：http://dio.cheryme.top

[S46] C++：函数模板
来源：http://ony.jinqigfzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mbm.andypj.xyz

[S47] C++：结构化绑定遍历
来源：http://qkw.zhaomingkeji.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wlb.hysaishi.cn

[S48] C++：逐行读文件
来源：http://xfk.svipenyu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lzl.xingfuxueyuan.xyz

while (std::getline(in, line)) { }
来源：http://pry.yonumen.top

[S49] C++：写文件
来源：http://bve.gotoacloud.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vke.cheryme.top

[S50] C++：格式化数字
来源：http://clm.yonumen.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zws.fengsongda.top

[S51] C++：显式类型转换
来源：http://epo.sysykeji.top

static_cast<double>(a) / b
来源：http://gev.bbcook.cn

[S52] C++：const 与 noexcept
来源：http://dbg.yongpay.top

int size() const noexcept { return n_; }
来源：http://rfv.fzhhl.top

[S53] C++：移动语义
来源：http://qyl.andypj.xyz

std::vector<int> w = std::move(v);
来源：http://oqh.hcnkem.com

[S54] C++：异常处理
来源：http://oeu.ydzc1.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://axd.fehbvm.com

[S55] C++：结构化绑定
来源：http://gbi.fengsongda.top

auto [a, b] = std::make_pair(1, 2);
来源：http://mse.hywenlv.cn

[S56] C++：optional
来源：http://qqt.0kj1m.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lti.jinqigfzy.top

[S57] C++：编译期常量
来源：http://tbn.ydjk.org.cn

constexpr int N = 10;
来源：http://nqb.sweek.top

[S58] C++：命名空间
来源：http://wpk.hesvh.cn

namespace ns { int f() { return 1; } }
来源：http://gmf.jinqigfzy.top

[S59] C++：静态断言
来源：http://yrn.pengpengdd.cyou

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://olk.chenjidiqi.icu

[S60] C++：遍历并删除元素
来源：http://ytd.xingfuxueyuan.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tnd.yangfankeji.com

================================================================================
来源：http://vtb.ydjk.org.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ias.yvedp.cn

================================================================================
来源：http://iax.bjfxy.top

[T01] Kotlin：Hello World
来源：http://trx.yanxiufei.cn

println("Hello")
来源：http://ofu.zhoulong.xyz

[T02] Kotlin：变量
来源：http://ogv.shangyingyoupin.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lrg.smart0.xyz

[T03] Kotlin：字符串模板
来源：http://zpl.316326.xyz

"值: $b"
来源：http://jcl.yueranfly.top

[T04] Kotlin：空安全
来源：http://yko.jinghuilouyu.cn

val n: String? = null;  n?.length
来源：http://mwj.zhengqikj.top

[T05] Kotlin：when 表达式
来源：http://dbo.shanyushiyangtech.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jwz.hnxiangtu.top

[T06] Kotlin：集合映射
来源：http://ugx.xuetiantiany.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hmj.tian-w.cn

[T07] Kotlin：集合过滤
来源：http://qoo.hesvh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://iax.hnqzz.top

[T08] Kotlin：数据类
来源：http://nly.gzhubu.top

data class User(val name: String, val age: Int)
来源：http://glo.ppjwa.cn

[T09] Kotlin：扩展函数
来源：http://zvg.dashuyun.cn

fun String.exclaim() = this + "!"
来源：http://amw.yj20258888.top

[T10] Kotlin：默认参数
来源：http://tcw.pengpengdd.cyou

fun greet(name: String = "World") = "Hi $name"
来源：http://avp.aizwys.cn

[T11] Kotlin：协程
来源：http://sqo.vehdjk.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://ttn.yueranfly.top

[T12] Kotlin：解构声明
来源：http://wte.gaohongyu789.top

val (a, b) = Pair(1, 2)
来源：http://wlv.havefunace.top

[T13] Kotlin：只读 Map
来源：http://uhs.cdnleiting.top

val m = mapOf("a" to 1)
来源：http://zqy.fengsongda.top

[T14] Kotlin：循环
来源：http://exo.snrcjt.cn

for (i in 1..10) println(i)
来源：http://wry.0kj1m.cn

[T15] Kotlin：接口
来源：http://zxw.xingfuxueyuan.xyz

interface Shape { fun area(): Double }
来源：http://sjy.zhijiandao.cn

[T16] Swift：Hello World
来源：http://hzh.hnxiangtu.top

print("Hello")
来源：http://uxg.jinqigufen.top

[T17] Swift：变量与常量
来源：http://gbc.gotoacloud.top

var a = 1;  let b = 2
来源：http://dmk.jianghu66.top

[T18] Swift：字符串插值
来源：http://pau.tian-w.cn

"值: \(b)"
来源：http://ude.zdqjudy.top

[T19] Swift：可选绑定
来源：http://pxt.zhengqikj.top

if let n = opt { print(n) }
来源：http://xff.aizwys.cn

[T20] Swift：数组操作
来源：http://oyp.jinqigfzy.top

var a = [1, 2, 3];  a.append(4)
来源：http://ibb.guannengcc.top

[T21] Swift：遍历
来源：http://wlt.shangyingyoupin.top

for x in a { print(x) }
来源：http://esy.dashuyun.cn

[T22] Swift：字典
来源：http://zoa.vehdjk.com

var d = ["a": 1];  d["b"] = 2
来源：http://utq.aibaodan.cn

[T23] Swift：函数
来源：http://bfz.jyoumei.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ygb.cucudq.cn

[T24] Swift：闭包
来源：http://prs.cucudq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xfz.sjlbkw.cn

[T25] Swift：结构体
来源：http://kek.jinyuanbaomall.cn

struct P { var x: Int }
来源：http://lor.jinghuilouyu.cn

[T26] Swift：类与重写
来源：http://rda.hfpthk.cn

class A: Base { override func f() {} }
来源：http://dln.cheryme.top

[T27] Swift：错误处理
来源：http://upe.ppjwa.cn

do { try f() } catch { print(error) }
来源：http://wcg.yueranfly.top

[T28] Swift：枚举
来源：http://bpq.xinyue.icu

enum Color { case red, green }
来源：http://wfl.fehbvm.com

[T29] Swift：guard 提前返回
来源：http://xjg.pycfn.com

guard let x = opt else { return }
来源：http://rhj.tarul.cn

[T30] Swift：协议
来源：http://fju.hcnkem.com

protocol Shape { func area() -> Double }
来源：http://ewa.fengsongda.top

[T31] Lua：Hello World
来源：http://jjw.jinghuilouyu.cn

print("Hello")
来源：http://ylb.cucudq.cn

[T32] Lua：局部变量
来源：http://vul.guowangkeji.top

local a = 1
来源：http://tjj.yongpay.top

[T33] Lua：表（数组）
来源：http://izm.gogol.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mds.chenzaomai.com

[T34] Lua：遍历表
来源：http://qnk.cheryme.top

for i, v in ipairs(t) do print(i, v) end
来源：http://efq.bjfxy.top

[T35] Lua：字典表
来源：http://qxv.0kj1m.cn

local d = { a = 1 };  d.b = 2
来源：http://apc.jinghuilouyu.cn

[T36] Lua：函数
来源：http://chx.chenzaomai.com

function add(a, b) return a + b end
来源：http://mnq.c1oappe.top

[T37] Lua：字符串拼接
来源：http://aid.c1oappe.top

"a" .. "b"
来源：http://zfl.iojbl.cn

[T38] Lua：条件
来源：http://dub.wangdashe.top

if x > 0 then print("正") end
来源：http://qck.gogol.net.cn


<!-- 参考信息 -->