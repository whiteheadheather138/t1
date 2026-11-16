代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mep.ywan-chungtsiang.top

[R34] 退出时清理
来源：http://fqd.jyoumei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ajy.zhengqikj.top

[R35] 后台执行并等待
来源：http://cds.yfazqb.com

sleep 5 & pid=$!; wait "$pid"
来源：http://mft.fzhhl.top

[R36] 并发执行多个任务
来源：http://ioi.xingfuxueyuan.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://orc.fehbvm.com

[R37] 把输出赋给变量
来源：http://jty.andypj.xyz

files=$(ls -1)
来源：http://cey.tarul.cn

[R38] 管道串联
来源：http://ydq.aizwys.cn

cat a.txt | grep -i error | wc -l
来源：http://dqf.ppjwa.cn

[R39] 重定向标准输出与错误
来源：http://sih.haohaochexian.top

cmd > out.log 2>&1
来源：http://usf.hnqzz.top

[R40] 追加写日志
来源：http://jap.xingfuxueyuan.xyz

echo "log" >> out.log
来源：http://hjl.zhiwuduotai.top

[R41] 丢弃输出
来源：http://qci.fanxiaobao.xyz

cmd >/dev/null 2>&1
来源：http://iev.hfpthk.cn

[R42] 输入重定向
来源：http://xxp.yfazqb.com

wc -l < a.txt
来源：http://brl.yonumen.top

[R43] 按名字查找文件
来源：http://vxd.mhx1999.top

find . -name "*.log" -type f
来源：http://yhk.andypj.xyz

[R44] 按修改时间查找
来源：http://ewn.xuanzx.com

find . -mtime -7 -type f
来源：http://tbp.fktsv.cn

[R45] 批量删除
来源：http://zqr.zdbjq.cn

find . -name "*.tmp" -delete
来源：http://hru.quarkkingdee.top

[R46] 递归替换文件内容
来源：http://jeo.vehdjk.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gfo.zhiwuduotai.top

[R47] sed 单行替换
来源：http://pao.nwbrower.top

sed -i 's/foo/bar/g' a.txt
来源：http://fuv.yj202588.top

[R48] awk 取指定列
来源：http://qte.xingfuxueyuan.xyz

awk '{print $1, $3}' a.txt
来源：http://swx.jianghu66.top

[R49] awk 带条件
来源：http://wwl.zdqjudy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lzc.yj20258888.top

[R50] awk 求和
来源：http://oxt.ywan-chungtsiang.top

awk '{s += $2} END {print s}' a.txt
来源：http://pex.yonumen.top

[R51] 排序去重取前几
来源：http://njq.jinghuilouyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zae.yfazqb.com

[R52] 统计行数
来源：http://loc.hammf.cn

wc -l a.txt
来源：http://ccv.wangshuangyany.cn

[R53] 查看文件头与实时尾
来源：http://pef.gzhubu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bbc.haohaochexian.top

[R54] 比较两个文件
来源：http://cln.yangfankeji.com

diff a.txt b.txt
来源：http://ztp.chenlongwang.top

[R55] 压缩与解压
来源：http://dzw.ctjpmb.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pup.fehbvm.com

[R56] 远程拷贝
来源：http://rjf.shangyingyoupin.top

scp file user@host:/path/
来源：http://iff.yvedp.cn

[R57] 远程执行命令
来源：http://ohr.c1oappe.top

ssh user@host 'uptime'
来源：http://wyz.ivvv.top

[R58] 下载文件
来源：http://ira.yuanzhike.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wyn.quarkkingdee.top

[R59] 发 POST JSON
来源：http://koo.yj20258888.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oph.yfazqb.com

[R60] 只看 HTTP 状态码
来源：http://xnh.hywenlv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zqv.nanxuanxn.top

[R61] 磁盘占用
来源：http://scj.xingfuxueyuan.xyz

df -h;  du -sh *
来源：http://vrm.jlsjyb.cn

[R62] 找最占空间的文件
来源：http://aer.ydjk.org.cn

du -ah . | sort -rh | head -10
来源：http://ive.jiagoushi.top

[R63] 内存与进程
来源：http://ceh.yvedp.cn

free -h;  ps aux | grep nginx
来源：http://rjl.nanxinkj.top

[R64] 结束进程
来源：http://zbx.svipenyu.cn

kill -9 $(pgrep -f app.py)
来源：http://iqz.gzhubu.top

[R65] 查看端口占用
来源：http://myf.ctjpmb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://thp.fehbvm.com

[R66] 定时任务
来源：http://kar.birdmap.top

crontab -e;  crontab -l
来源：http://ivj.jinqigfzy.top

[R67] 生成随机十六进制串
来源：http://lve.pengpengdd.cyou

openssl rand -hex 16
来源：http://hyv.pycfn.com

[R68] 计算文件校验值
来源：http://pwn.gaohongyu789.top

sha256sum a.txt;  md5sum a.txt
来源：http://trl.cqqwz.cn

[R69] 生成随机密码
来源：http://qzw.wangshuangyany.cn

head -c 16 /dev/urandom | base64
来源：http://vxo.wangshuangyany.cn

[R70] 时间戳与互转
来源：http://sxt.yongpay.top

date +%s;  date -d @1700000000
来源：http://iqq.cucudq.cn

[R71] 日期格式化
来源：http://fbx.jqgfzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://lkn.tianlin.xyz

[R72] 等待端口就绪
来源：http://vct.xylfe.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xuv.yj20258.top

[R73] 分割大日志
来源：http://isq.feifeiyinyue.top

split -l 1000 big.log part_
来源：http://tmr.dashuyun.cn

[R74] 批量重命名
来源：http://cgm.chenjidiqi.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uzy.xylfe.cn

[R75] 导出环境变量
来源：http://dqd.0kj1m.cn

export PATH="$HOME/bin:$PATH"
来源：http://plg.daria6918.cn

[R76] 使用临时文件
来源：http://vun.yonumen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gpj.snrcjt.cn

[R77] 读取用户输入
来源：http://ptc.yj202588.top

read -rp "请输入: " ans
来源：http://ypf.yuxming.cn

[R78] 交互式菜单
来源：http://zfa.jinqigufen.top

select opt in a b c; do echo "$opt"; break; done
来源：http://axm.hywenlv.cn

[R79] 解析命令行选项
来源：http://ljg.c1oappe.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pid.cashguo.top

[R80] 查看脚本执行耗时
来源：http://dal.dianchejie.cn

time ./run.sh
来源：http://kbo.gotoacloud.top

================================================================================
来源：http://puo.cheryme.top

S. C / C++ 专题
来源：http://unf.c1oappe.top

================================================================================
来源：http://pge.gzhubu.top

[S01] C：Hello World
来源：http://yhx.jiagoushi.top

#include <stdio.h>
来源：http://cbr.tarul.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mht.mhx1999.top

[S02] C：变量与格式化输出
来源：http://xvq.kuanghao11.cn

int a = 10; printf("%d\n", a);
来源：http://dcj.ivvv.top

[S03] C：读入整数
来源：http://gro.vqdsnc.cn

int x; scanf("%d", &x);
来源：http://mvu.aibaodan.cn

[S04] C：字符串复制
来源：http://psr.iojbl.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tbj.zhiwuduotai.top

[S05] C：字符串长度
来源：http://eul.52xcode.cn

strlen(s)
来源：http://nsd.sxryk.cn

[S06] C：字符串比较
来源：http://gxw.snrcjt.cn

strcmp(a, b) == 0
来源：http://xdb.chenzaomai.com

[S07] C：数组遍历求和
来源：http://swv.gotoacloud.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uld.kuanghao11.cn

[S08] C：动态内存分配与释放
来源：http://xsi.cdnleiting.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hew.chenzaomai.com

[S09] C：结构体定义与初始化
来源：http://hzt.hongshengwenyu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://enc.xuanzx.com

[S10] C：指针与解引用
来源：http://kzh.yuxming.cn

int *p = &a;  *p = 5;
来源：http://tfz.xziqi.cn

[S11] C：逐行读文件
来源：http://hbb.sufxvd.cn

FILE *f = fopen("a.txt", "r");
来源：http://oph.sjlbkw.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mxd.jyoumei.cn

fclose(f);
来源：http://vnh.nanxinkj.top

[S12] C：写文件
来源：http://bcq.chenzaomai.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fkw.yonumen.top

[S13] C：宏定义
来源：http://plg.yonumen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cde.yonumen.top

[S14] C：枚举
来源：http://uwt.guannengcc.top

enum Color { RED, GREEN, BLUE };
来源：http://vmn.tanke756.top

[S15] C：类型转换
来源：http://syc.shuidangran.top

(double) a / b
来源：http://vvm.vqdsnc.cn

[S16] C：位操作置位
来源：http://wpx.zhixingplan.top

x |= (1 << 3);
来源：http://ruy.andypj.xyz

[S17] C：安全拼接字符串
来源：http://oox.hysaishi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lzl.shanyushiyangkeji.top

[S18] C：命令行参数
来源：http://gto.gaohongyu789.top

int main(int argc, char **argv)
来源：http://kdg.redwolf501.top

[S19] C：快速排序
来源：http://ucu.zdqjudy.top

qsort(a, n, sizeof(int), cmp);
来源：http://llr.vehdjk.com

[S20] C：二分查找
来源：http://stq.cdnleiting.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rou.yueranfly.top

[S21] C：字符类别判断
来源：http://qfo.shuidangran.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ipr.cqqwz.cn

[S22] C：字符串转数字
来源：http://sly.haohaochexian.top

atoi("42");  strtod("3.14", NULL);
来源：http://rsd.yonumen.top

[S23] C：随机数
来源：http://tmh.sjlbkw.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://srw.uphjek.com

[S24] C：获取本地时间
来源：http://iqj.pycfn.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xrd.tanke756.top

[S25] C：内存拷贝
来源：http://yjw.hnqzz.top

memcpy(dst, src, n);
来源：http://icr.jlsjyb.cn

[S26] C：内存清零
来源：http://beg.xinyue.icu

memset(a, 0, sizeof a);
来源：http://ufe.316326.xyz

[S27] C：定义常量
来源：http://kex.zhongyouzk.top

const double PI = 3.14159;
来源：http://ijv.jqgufenzy.top

[S28] C：静态变量
来源：http://ndj.xziqi.cn

static int counter = 0;
来源：http://lqb.zhaomingkeji.xyz

[S29] C：变参函数
来源：http://tcx.feifeiyinyue.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gya.zhaomingkeji.xyz

[S30] C：头文件保护
来源：http://jgj.yanxiufei.cn

#ifndef X_H
来源：http://tte.gzhubu.top

#define X_H
来源：http://lyh.andypj.xyz

#endif
来源：http://qir.svipenyu.cn

[S31] C++：Hello World
来源：http://gmf.kuanghao11.cn

#include <iostream>
来源：http://hwg.cdnleiting.top

int main() { std::cout << "Hello\n"; }
来源：http://opr.hysaishi.cn

[S32] C++：字符串
来源：http://lln.epnwcf.com

std::string s = "hi";  s += "!";
来源：http://hok.sysykeji.top

[S33] C++：vector 增删
来源：http://rir.sysykeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://djg.nanxuanxn.top

[S34] C++：遍历 vector
来源：http://hza.9152youxi.cn

for (auto &x : v) { std::cout << x; }
来源：http://evw.zhongyouzk.top

[S35] C++：map
来源：http://biv.dashuyun.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cyx.hammf.cn

[S36] C++：unordered_map
来源：http://pgj.cashguo.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rgu.ctjpmb.com

[S37] C++：set
来源：http://jdm.316326.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uja.zhoulong.xyz

[S38] C++：排序
来源：http://oje.zhoulong.xyz

std::sort(v.begin(), v.end());
来源：http://npt.316326.xyz

[S39] C++：自定义比较器排序
来源：http://osd.cheryme.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eqh.fzhhl.top

[S40] C++：查找元素
来源：http://xfr.havefunace.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rir.yonumen.top

[S41] C++：类与构造函数
来源：http://tmr.aizwys.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pwl.redwolf501.top

[S42] C++：继承与虚函数
来源：http://qmw.yueranfly.top

class B : public Base { public: void f() override {} };
来源：http://jlg.fanxiaobao.xyz

[S43] C++：智能指针
来源：http://kzg.pycfn.com

auto p = std::make_unique<int>(5);
来源：http://pss.yonumen.top

[S44] C++：引用传参
来源：http://vba.jlsjyb.cn

void inc(int &x) { ++x; }
来源：http://ytf.hnqzz.top

[S45] C++：lambda
来源：http://abj.andypj.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://okp.cdnleiting.top

[S46] C++：函数模板
来源：http://jaw.bbcook.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xse.xylfe.cn

[S47] C++：结构化绑定遍历
来源：http://rgc.sweek.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qgb.xinyue.icu

[S48] C++：逐行读文件
来源：http://zrs.jiagoushi.top

std::ifstream in("a.txt");  std::string line;
来源：http://gos.sweek.top

while (std::getline(in, line)) { }
来源：http://eht.zhiwuduotai.top

[S49] C++：写文件
来源：http://acz.epnwcf.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nlx.kuanghao11.cn

[S50] C++：格式化数字
来源：http://oke.jinqigufen.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tol.sxryk.cn

[S51] C++：显式类型转换
来源：http://lim.fehbvm.com

static_cast<double>(a) / b
来源：http://aly.fzhhl.top

[S52] C++：const 与 noexcept
来源：http://odu.pengpengdd.cyou

int size() const noexcept { return n_; }
来源：http://htq.mhx1999.top

[S53] C++：移动语义
来源：http://sue.dashuyun.cn

std::vector<int> w = std::move(v);
来源：http://wws.ybcxt.top

[S54] C++：异常处理
来源：http://cnl.gogol.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://udc.yueranfly.top

[S55] C++：结构化绑定
来源：http://ytb.fengsongda.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tvp.meibo888.top

[S56] C++：optional
来源：http://asx.jyoumei.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qry.zycfv.cn

[S57] C++：编译期常量
来源：http://ove.mhx1999.top

constexpr int N = 10;
来源：http://tto.hcnkem.com

[S58] C++：命名空间
来源：http://jnn.ivvv.top

namespace ns { int f() { return 1; } }
来源：http://zjo.daria6918.cn

[S59] C++：静态断言
来源：http://uid.daria6918.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jbz.yj20258888.top

[S60] C++：遍历并删除元素
来源：http://mgm.mhx1999.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jvk.fktsv.cn

================================================================================
来源：http://clu.jinqigfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://grq.zhengqikj.top

================================================================================
来源：http://qcl.dianchejie.cn

[T01] Kotlin：Hello World
来源：http://khx.tianlin.xyz

println("Hello")
来源：http://jzm.nanxinkj.top

[T02] Kotlin：变量
来源：http://ghe.hywenlv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dyv.xingfuxueyuan.xyz

[T03] Kotlin：字符串模板
来源：http://aol.hammf.cn

"值: $b"
来源：http://arn.ehwqpu.com

[T04] Kotlin：空安全
来源：http://pzl.aibaodan.cn

val n: String? = null;  n?.length
来源：http://pex.c1oappe.top

[T05] Kotlin：when 表达式
来源：http://smn.kuanghao11.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dyv.yuanzhike.top

[T06] Kotlin：集合映射
来源：http://onk.jianghu66.top

listOf(1, 2, 3).map { it * 2 }
来源：http://dxh.zhaomingkeji.xyz

[T07] Kotlin：集合过滤
来源：http://qqf.mhx1999.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://iyb.tianlin.xyz

[T08] Kotlin：数据类
来源：http://icq.ydzc1.top

data class User(val name: String, val age: Int)
来源：http://jgq.yvedp.cn

[T09] Kotlin：扩展函数
来源：http://cbp.52xcode.cn

fun String.exclaim() = this + "!"
来源：http://tlx.quarkkingdee.top

[T10] Kotlin：默认参数
来源：http://raf.ctjpmb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://gqv.zhengqikj.top

[T11] Kotlin：协程
来源：http://tom.daxiang520.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://zrl.xingfuxueyuan.xyz

[T12] Kotlin：解构声明
来源：http://gnl.sysykeji.top

val (a, b) = Pair(1, 2)
来源：http://iec.yangfankeji.com

[T13] Kotlin：只读 Map
来源：http://ckh.bbcook.cn

val m = mapOf("a" to 1)
来源：http://lfv.hywenlv.cn

[T14] Kotlin：循环
来源：http://siw.iojbl.cn

for (i in 1..10) println(i)
来源：http://wyr.vqdsnc.cn

[T15] Kotlin：接口
来源：http://lcg.zhongyouzk.top

interface Shape { fun area(): Double }
来源：http://cwr.yonumen.top

[T16] Swift：Hello World
来源：http://iid.snrcjt.cn

print("Hello")
来源：http://wmx.zhongyouzk.top

[T17] Swift：变量与常量
来源：http://kzt.jqgfzy.top

var a = 1;  let b = 2
来源：http://rvl.gaohongyu789.top

[T18] Swift：字符串插值
来源：http://nfo.gaohongyu789.top

"值: \(b)"
来源：http://iie.feifeiyinyue.top

[T19] Swift：可选绑定
来源：http://sjt.fzhhl.top

if let n = opt { print(n) }
来源：http://krq.yangfankeji.com

[T20] Swift：数组操作
来源：http://bjl.zhongyouzk.top

var a = [1, 2, 3];  a.append(4)
来源：http://yfr.hnqzz.top

[T21] Swift：遍历
来源：http://bdu.cashguo.top

for x in a { print(x) }
来源：http://ska.bbcook.cn

[T22] Swift：字典
来源：http://ogc.hnqzz.top

var d = ["a": 1];  d["b"] = 2
来源：http://bqf.hnqzz.top

[T23] Swift：函数
来源：http://xle.hnqzz.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ulz.jiagoushi.top

[T24] Swift：闭包
来源：http://lnv.shzxlz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ajc.tian-w.cn

[T25] Swift：结构体
来源：http://xjv.vehdjk.com

struct P { var x: Int }
来源：http://rzu.dianchejie.cn

[T26] Swift：类与重写
来源：http://kkn.shanyushiyangkeji.top

class A: Base { override func f() {} }
来源：http://ecd.fktsv.cn

[T27] Swift：错误处理
来源：http://hge.tian-w.cn

do { try f() } catch { print(error) }
来源：http://xar.yangfankeji.com

[T28] Swift：枚举
来源：http://bae.yj20258888.top

enum Color { case red, green }
来源：http://fqk.c1oappe.top

[T29] Swift：guard 提前返回
来源：http://yxp.sysykeji.top

guard let x = opt else { return }
来源：http://oyf.uphjek.com

[T30] Swift：协议
来源：http://yso.jinghuilouyu.cn

protocol Shape { func area() -> Double }
来源：http://qsp.fehbvm.com

[T31] Lua：Hello World
来源：http://qmr.hnxiangtu.top

print("Hello")
来源：http://mkq.uphjek.com

[T32] Lua：局部变量
来源：http://lsg.shzxlz.cn

local a = 1
来源：http://tsx.chenzaomai.com

[T33] Lua：表（数组）
来源：http://swv.yvedp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ypi.wangdashe.top

[T34] Lua：遍历表
来源：http://fml.yj20258888.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ylq.xuetiantiany.cn

[T35] Lua：字典表
来源：http://cih.pengpengdd.cyou

local d = { a = 1 };  d.b = 2
来源：http://txs.aizwys.cn

[T36] Lua：函数
来源：http://gwb.hongshengwenyu.top

function add(a, b) return a + b end
来源：http://ufu.hfpthk.cn


<!-- 参考信息 -->