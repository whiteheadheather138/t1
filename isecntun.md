代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fpa.nanxinkj.top

[R34] 退出时清理
来源：http://tmj.cucudq.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nkk.smart0.xyz

[R35] 后台执行并等待
来源：http://aso.zhongyouzk.top

sleep 5 & pid=$!; wait "$pid"
来源：http://lwm.guowangkeji.top

[R36] 并发执行多个任务
来源：http://nak.xylfe.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bho.nwbrower.top

[R37] 把输出赋给变量
来源：http://xuu.0kj1m.cn

files=$(ls -1)
来源：http://jvv.chenjidiqi.icu

[R38] 管道串联
来源：http://ajz.zhiwuduotai.top

cat a.txt | grep -i error | wc -l
来源：http://dgq.smart0.xyz

[R39] 重定向标准输出与错误
来源：http://ddn.haohaochexian.top

cmd > out.log 2>&1
来源：http://gyv.hongshengwenyu.top

[R40] 追加写日志
来源：http://fss.chenlongwang.top

echo "log" >> out.log
来源：http://qzt.c1oappe.top

[R41] 丢弃输出
来源：http://dmy.redwolf501.top

cmd >/dev/null 2>&1
来源：http://ygf.yfazqb.com

[R42] 输入重定向
来源：http://pum.sufxvd.cn

wc -l < a.txt
来源：http://jpq.cashguo.top

[R43] 按名字查找文件
来源：http://hjf.pycfn.com

find . -name "*.log" -type f
来源：http://nch.uphjek.com

[R44] 按修改时间查找
来源：http://ina.shanyushiyangkeji.top

find . -mtime -7 -type f
来源：http://pgx.tianlin.xyz

[R45] 批量删除
来源：http://yia.wangshuangyany.cn

find . -name "*.tmp" -delete
来源：http://dbs.hfpthk.cn

[R46] 递归替换文件内容
来源：http://pin.wangdashe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wws.ywan-chungtsiang.top

[R47] sed 单行替换
来源：http://ynq.sweek.top

sed -i 's/foo/bar/g' a.txt
来源：http://ria.yfazqb.com

[R48] awk 取指定列
来源：http://jwn.nanxinkj.top

awk '{print $1, $3}' a.txt
来源：http://evt.52xcode.cn

[R49] awk 带条件
来源：http://sra.fengsongda.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qpr.pycfn.com

[R50] awk 求和
来源：http://wfg.ehwqpu.com

awk '{s += $2} END {print s}' a.txt
来源：http://nyy.quarkkingdee.top

[R51] 排序去重取前几
来源：http://sbm.jqgufenzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://hzs.daria6918.cn

[R52] 统计行数
来源：http://lwy.gaohongyu789.top

wc -l a.txt
来源：http://ddm.c1oappe.top

[R53] 查看文件头与实时尾
来源：http://qjt.jyoumei.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ufu.haohaochexian.top

[R54] 比较两个文件
来源：http://fbe.tanke756.top

diff a.txt b.txt
来源：http://oyb.9152youxi.cn

[R55] 压缩与解压
来源：http://kdc.daxiang520.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mmk.shanyushiyangtech.top

[R56] 远程拷贝
来源：http://hcx.fengsongda.top

scp file user@host:/path/
来源：http://xzy.ehwqpu.com

[R57] 远程执行命令
来源：http://cqy.tianlin.xyz

ssh user@host 'uptime'
来源：http://tvl.cqqwz.cn

[R58] 下载文件
来源：http://xhb.tianlin.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://koj.0kj1m.cn

[R59] 发 POST JSON
来源：http://shc.shuidangran.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mjs.ybcxt.top

[R60] 只看 HTTP 状态码
来源：http://lpy.jinqigfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uht.daria6918.cn

[R61] 磁盘占用
来源：http://vwm.wangshuangyany.cn

df -h;  du -sh *
来源：http://vjf.ehwqpu.com

[R62] 找最占空间的文件
来源：http://xri.ctjpmb.com

du -ah . | sort -rh | head -10
来源：http://drt.ivvv.top

[R63] 内存与进程
来源：http://irh.yj20258.top

free -h;  ps aux | grep nginx
来源：http://aaa.ybcxt.top

[R64] 结束进程
来源：http://zek.jiagoushi.top

kill -9 $(pgrep -f app.py)
来源：http://mpd.quarkkingdee.top

[R65] 查看端口占用
来源：http://iqc.cdnleiting.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://snd.hesvh.cn

[R66] 定时任务
来源：http://ukw.daria6918.cn

crontab -e;  crontab -l
来源：http://bpo.aibaodan.cn

[R67] 生成随机十六进制串
来源：http://dqy.cdnleiting.top

openssl rand -hex 16
来源：http://jog.uphjek.com

[R68] 计算文件校验值
来源：http://igw.cqqwz.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nqu.zhixingplan.top

[R69] 生成随机密码
来源：http://ugz.chenjidiqi.icu

head -c 16 /dev/urandom | base64
来源：http://pbi.guannengcc.top

[R70] 时间戳与互转
来源：http://qki.jyoumei.cn

date +%s;  date -d @1700000000
来源：http://yhk.ctjpmb.com

[R71] 日期格式化
来源：http://tdg.zhiwuduotai.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jpu.hnqzz.top

[R72] 等待端口就绪
来源：http://rew.xuanzx.com

until nc -z localhost 3306; do sleep 1; done
来源：http://iur.cqqwz.cn

[R73] 分割大日志
来源：http://phs.zhongyouzk.top

split -l 1000 big.log part_
来源：http://wlo.zdbjq.cn

[R74] 批量重命名
来源：http://eie.sxryk.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dkx.jinghuilouyu.cn

[R75] 导出环境变量
来源：http://bvd.havefunace.top

export PATH="$HOME/bin:$PATH"
来源：http://jbe.sweek.top

[R76] 使用临时文件
来源：http://cgm.vehdjk.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ujx.gogol.net.cn

[R77] 读取用户输入
来源：http://jxy.hesvh.cn

read -rp "请输入: " ans
来源：http://uop.hywenlv.cn

[R78] 交互式菜单
来源：http://xff.sxryk.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jpp.andypj.xyz

[R79] 解析命令行选项
来源：http://vro.xuanzx.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qgx.ywan-chungtsiang.top

[R80] 查看脚本执行耗时
来源：http://bzy.cheryme.top

time ./run.sh
来源：http://hgs.iojbl.cn

================================================================================
来源：http://egh.ydzc1.top

S. C / C++ 专题
来源：http://hbf.yongpay.top

================================================================================
来源：http://pak.jqgfzy.top

[S01] C：Hello World
来源：http://iox.fzhhl.top

#include <stdio.h>
来源：http://ill.fengsongda.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://dmy.tanke756.top

[S02] C：变量与格式化输出
来源：http://lse.aizwys.cn

int a = 10; printf("%d\n", a);
来源：http://svt.wangdashe.top

[S03] C：读入整数
来源：http://ufx.hesvh.cn

int x; scanf("%d", &x);
来源：http://geg.hammf.cn

[S04] C：字符串复制
来源：http://kxt.hnqzz.top

char dst[32]; strcpy(dst, "hi");
来源：http://mdk.mhx1999.top

[S05] C：字符串长度
来源：http://btk.fengsongda.top

strlen(s)
来源：http://aca.yanxiufei.cn

[S06] C：字符串比较
来源：http://kqu.zhengqikj.top

strcmp(a, b) == 0
来源：http://jyu.ydjk.org.cn

[S07] C：数组遍历求和
来源：http://agd.jinghuilouyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kwm.feifeiyinyue.top

[S08] C：动态内存分配与释放
来源：http://oef.shanyushiyangkeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nee.316326.xyz

[S09] C：结构体定义与初始化
来源：http://pjj.shanyushiyangtech.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dxp.gaohongyu789.top

[S10] C：指针与解引用
来源：http://vpr.daria6918.cn

int *p = &a;  *p = 5;
来源：http://twp.zdqjudy.top

[S11] C：逐行读文件
来源：http://xhm.vehdjk.com

FILE *f = fopen("a.txt", "r");
来源：http://yxx.shanyushiyangtech.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wjx.sweek.top

fclose(f);
来源：http://lnc.chenjidiqi.icu

[S12] C：写文件
来源：http://kgg.quarkkingdee.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yxs.fktsv.cn

[S13] C：宏定义
来源：http://jak.dianchejie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rvl.hnqzz.top

[S14] C：枚举
来源：http://nla.sweek.top

enum Color { RED, GREEN, BLUE };
来源：http://srl.zhaomingkeji.xyz

[S15] C：类型转换
来源：http://tmm.fktsv.cn

(double) a / b
来源：http://fmr.nanxinkj.top

[S16] C：位操作置位
来源：http://wol.dashuyun.cn

x |= (1 << 3);
来源：http://qpv.daxiang520.top

[S17] C：安全拼接字符串
来源：http://yce.meibo888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://klh.zhixingplan.top

[S18] C：命令行参数
来源：http://kgq.zhoulong.xyz

int main(int argc, char **argv)
来源：http://wul.fengsongda.top

[S19] C：快速排序
来源：http://axh.52xcode.cn

qsort(a, n, sizeof(int), cmp);
来源：http://koq.hnxiangtu.top

[S20] C：二分查找
来源：http://gsq.jinyuanbaomall.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mqo.9152youxi.cn

[S21] C：字符类别判断
来源：http://mfh.hongshengwenyu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vfq.fzhhl.top

[S22] C：字符串转数字
来源：http://rfo.kuanghao11.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hae.sysykeji.top

[S23] C：随机数
来源：http://hpg.sweek.top

srand(time(NULL));  int r = rand() % 100;
来源：http://jvf.shanyushiyangtech.top

[S24] C：获取本地时间
来源：http://igu.ehwqpu.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://orc.nwbrower.top

[S25] C：内存拷贝
来源：http://obo.yuxming.cn

memcpy(dst, src, n);
来源：http://gbn.dashuyun.cn

[S26] C：内存清零
来源：http://vjs.ehwqpu.com

memset(a, 0, sizeof a);
来源：http://ucf.chenlongwang.top

[S27] C：定义常量
来源：http://qhz.aibaodan.cn

const double PI = 3.14159;
来源：http://dxr.fehbvm.com

[S28] C：静态变量
来源：http://waf.hnxiangtu.top

static int counter = 0;
来源：http://vxl.jqgufenzy.top

[S29] C：变参函数
来源：http://gtd.xuanzx.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zgn.jianghu66.top

[S30] C：头文件保护
来源：http://udj.fanxiaobao.xyz

#ifndef X_H
来源：http://bxi.xinyue.icu

#define X_H
来源：http://grf.zhengqikj.top

#endif
来源：http://fpc.vqdsnc.cn

[S31] C++：Hello World
来源：http://dbb.yj202588.top

#include <iostream>
来源：http://ruq.zhijiandao.cn

int main() { std::cout << "Hello\n"; }
来源：http://ivi.bbcook.cn

[S32] C++：字符串
来源：http://cwt.shangyingyoupin.top

std::string s = "hi";  s += "!";
来源：http://gom.yueranfly.top

[S33] C++：vector 增删
来源：http://fog.sweek.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ezu.bjfxy.top

[S34] C++：遍历 vector
来源：http://rdh.tarul.cn

for (auto &x : v) { std::cout << x; }
来源：http://wkw.chenlongwang.top

[S35] C++：map
来源：http://dfs.zhixingplan.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lrz.redwolf501.top

[S36] C++：unordered_map
来源：http://nmx.yj20258.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ljf.kuanghao11.cn

[S37] C++：set
来源：http://osj.meibo888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://myh.hfpthk.cn

[S38] C++：排序
来源：http://xnu.fehbvm.com

std::sort(v.begin(), v.end());
来源：http://zrs.dianchejie.cn

[S39] C++：自定义比较器排序
来源：http://sjy.ywan-chungtsiang.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xbb.xylfe.cn

[S40] C++：查找元素
来源：http://znj.yanxiufei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lzb.jiagoushi.top

[S41] C++：类与构造函数
来源：http://iaf.jqgfzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vtg.chenjidiqi.icu

[S42] C++：继承与虚函数
来源：http://ijq.shangyingyoupin.top

class B : public Base { public: void f() override {} };
来源：http://rxs.cheryme.top

[S43] C++：智能指针
来源：http://yri.iojbl.cn

auto p = std::make_unique<int>(5);
来源：http://hfn.52xcode.cn

[S44] C++：引用传参
来源：http://jqo.ctjpmb.com

void inc(int &x) { ++x; }
来源：http://vko.zdbjq.cn

[S45] C++：lambda
来源：http://qex.ivvv.top

auto add = [](int a, int b) { return a + b; };
来源：http://drx.hysaishi.cn

[S46] C++：函数模板
来源：http://huz.xinyue.icu

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://aky.pengpengdd.cyou

[S47] C++：结构化绑定遍历
来源：http://asz.wangshuangyany.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rpm.meibo888.top

[S48] C++：逐行读文件
来源：http://dsy.sysykeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://nnb.pengpengdd.cyou

while (std::getline(in, line)) { }
来源：http://mtb.xingfuxueyuan.xyz

[S49] C++：写文件
来源：http://kiw.shzxlz.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://epx.mhx1999.top

[S50] C++：格式化数字
来源：http://avr.jinghuilouyu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qpi.nwbrower.top

[S51] C++：显式类型转换
来源：http://eff.xingfuxueyuan.xyz

static_cast<double>(a) / b
来源：http://jyu.pycfn.com

[S52] C++：const 与 noexcept
来源：http://zba.xylfe.cn

int size() const noexcept { return n_; }
来源：http://hmv.xziqi.cn

[S53] C++：移动语义
来源：http://unm.andypj.xyz

std::vector<int> w = std::move(v);
来源：http://svh.svipenyu.cn

[S54] C++：异常处理
来源：http://ctw.kuanghao11.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kxb.ywan-chungtsiang.top

[S55] C++：结构化绑定
来源：http://axk.jyoumei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bho.ybcxt.top

[S56] C++：optional
来源：http://cvj.cucudq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oun.nanxuanxn.top

[S57] C++：编译期常量
来源：http://eee.hammf.cn

constexpr int N = 10;
来源：http://mnk.ppjwa.cn

[S58] C++：命名空间
来源：http://doo.zycfv.cn

namespace ns { int f() { return 1; } }
来源：http://dgv.nwbrower.top

[S59] C++：静态断言
来源：http://edc.9152youxi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bws.316326.xyz

[S60] C++：遍历并删除元素
来源：http://hwl.vehdjk.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cnh.jiagoushi.top

================================================================================
来源：http://tjc.zhoulong.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kux.hnxiangtu.top

================================================================================
来源：http://syz.ehwqpu.com

[T01] Kotlin：Hello World
来源：http://qtp.birdmap.top

println("Hello")
来源：http://zae.epnwcf.com

[T02] Kotlin：变量
来源：http://emt.svipenyu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ruc.fanxiaobao.xyz

[T03] Kotlin：字符串模板
来源：http://udq.chenlongwang.top

"值: $b"
来源：http://zlk.vqdsnc.cn

[T04] Kotlin：空安全
来源：http://pto.316326.xyz

val n: String? = null;  n?.length
来源：http://vdu.vehdjk.com

[T05] Kotlin：when 表达式
来源：http://ovi.0kj1m.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sfu.cucudq.cn

[T06] Kotlin：集合映射
来源：http://pap.sxryk.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sah.hammf.cn

[T07] Kotlin：集合过滤
来源：http://zyj.haohaochexian.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://wbe.quarkkingdee.top

[T08] Kotlin：数据类
来源：http://iwn.yj20258888.top

data class User(val name: String, val age: Int)
来源：http://yjc.dashuyun.cn

[T09] Kotlin：扩展函数
来源：http://rxo.vqdsnc.cn

fun String.exclaim() = this + "!"
来源：http://unk.andypj.xyz

[T10] Kotlin：默认参数
来源：http://ssn.shanyushiyangkeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://zqp.hongshengwenyu.top

[T11] Kotlin：协程
来源：http://cio.0kj1m.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ort.gzhubu.top

[T12] Kotlin：解构声明
来源：http://ftn.chenzaomai.com

val (a, b) = Pair(1, 2)
来源：http://ikp.yj20258.top

[T13] Kotlin：只读 Map
来源：http://sqe.yuanzhike.top

val m = mapOf("a" to 1)
来源：http://yto.hcnkem.com

[T14] Kotlin：循环
来源：http://buj.mhx1999.top

for (i in 1..10) println(i)
来源：http://vxq.havefunace.top

[T15] Kotlin：接口
来源：http://lzd.yonumen.top

interface Shape { fun area(): Double }
来源：http://mne.hongshengwenyu.top

[T16] Swift：Hello World
来源：http://lbl.ctjpmb.com

print("Hello")
来源：http://ype.zhixingplan.top

[T17] Swift：变量与常量
来源：http://adj.hywenlv.cn

var a = 1;  let b = 2
来源：http://whp.sxryk.cn

[T18] Swift：字符串插值
来源：http://gfb.wangdashe.top

"值: \(b)"
来源：http://yps.yj20258.top

[T19] Swift：可选绑定
来源：http://olr.c1oappe.top

if let n = opt { print(n) }
来源：http://xli.jianghu66.top

[T20] Swift：数组操作
来源：http://wkb.zhijiandao.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yby.zhengqikj.top

[T21] Swift：遍历
来源：http://nct.andypj.xyz

for x in a { print(x) }
来源：http://nan.xziqi.cn

[T22] Swift：字典
来源：http://knq.jinqigfzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://bgj.yuanzhike.top

[T23] Swift：函数
来源：http://igz.gotoacloud.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fdf.yonumen.top

[T24] Swift：闭包
来源：http://gui.tarul.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kpc.shangyingyoupin.top

[T25] Swift：结构体
来源：http://uii.ehwqpu.com

struct P { var x: Int }
来源：http://irc.cucudq.cn

[T26] Swift：类与重写
来源：http://mam.aibaodan.cn

class A: Base { override func f() {} }
来源：http://nvb.chenlongwang.top

[T27] Swift：错误处理
来源：http://svh.zycfv.cn

do { try f() } catch { print(error) }
来源：http://tfh.feifeiyinyue.top

[T28] Swift：枚举
来源：http://gvh.feifeiyinyue.top

enum Color { case red, green }
来源：http://sie.gotoacloud.top

[T29] Swift：guard 提前返回
来源：http://ilf.uphjek.com

guard let x = opt else { return }
来源：http://srg.zhiwuduotai.top

[T30] Swift：协议
来源：http://ygm.jinqigufen.top

protocol Shape { func area() -> Double }
来源：http://tpj.havefunace.top

[T31] Lua：Hello World
来源：http://hgp.daria6918.cn

print("Hello")
来源：http://woe.jinghuilouyu.cn

[T32] Lua：局部变量
来源：http://ddm.xuanzx.com

local a = 1
来源：http://pfd.sweek.top

[T33] Lua：表（数组）
来源：http://yet.hnxiangtu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ibf.cucudq.cn

[T34] Lua：遍历表
来源：http://bzw.guowangkeji.top

for i, v in ipairs(t) do print(i, v) end
来源：http://vps.yj20258888.top

[T35] Lua：字典表
来源：http://zbi.hnqzz.top

local d = { a = 1 };  d.b = 2
来源：http://eij.zhijiandao.cn

[T36] Lua：函数
来源：http://mji.0kj1m.cn

function add(a, b) return a + b end
来源：http://rfw.yuxming.cn


<!-- 参考信息 -->