代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://npk.mhx1999.top

[R34] 退出时清理
来源：http://kac.ehwqpu.com

trap 'rm -f "$tmp"' EXIT
来源：http://vdz.shangyingyoupin.top

[R35] 后台执行并等待
来源：http://nva.sjlbkw.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zzr.jqgufenzy.top

[R36] 并发执行多个任务
来源：http://vnw.tanke756.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://quz.zhoulong.xyz

[R37] 把输出赋给变量
来源：http://xzd.vehdjk.com

files=$(ls -1)
来源：http://yqc.hongshengwenyu.top

[R38] 管道串联
来源：http://nek.52xcode.cn

cat a.txt | grep -i error | wc -l
来源：http://ysz.vehdjk.com

[R39] 重定向标准输出与错误
来源：http://anl.fengsongda.top

cmd > out.log 2>&1
来源：http://pmx.zhijiandao.cn

[R40] 追加写日志
来源：http://njw.daxiang520.top

echo "log" >> out.log
来源：http://ebd.yvedp.cn

[R41] 丢弃输出
来源：http://hhq.cdnleiting.top

cmd >/dev/null 2>&1
来源：http://fcp.bbcook.cn

[R42] 输入重定向
来源：http://nit.zhengqikj.top

wc -l < a.txt
来源：http://moq.andypj.xyz

[R43] 按名字查找文件
来源：http://xnj.tanke756.top

find . -name "*.log" -type f
来源：http://cem.hammf.cn

[R44] 按修改时间查找
来源：http://poy.guannengcc.top

find . -mtime -7 -type f
来源：http://ksn.jlsjyb.cn

[R45] 批量删除
来源：http://jku.birdmap.top

find . -name "*.tmp" -delete
来源：http://osq.meibo888.top

[R46] 递归替换文件内容
来源：http://agq.52xcode.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wbc.fanxiaobao.xyz

[R47] sed 单行替换
来源：http://jwr.yuxming.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ucr.wangshuangyany.cn

[R48] awk 取指定列
来源：http://uqa.yj20258.top

awk '{print $1, $3}' a.txt
来源：http://dnq.fehbvm.com

[R49] awk 带条件
来源：http://lpt.sweek.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dde.0kj1m.cn

[R50] awk 求和
来源：http://mki.redwolf501.top

awk '{s += $2} END {print s}' a.txt
来源：http://afo.redwolf501.top

[R51] 排序去重取前几
来源：http://ykm.pengpengdd.cyou

sort a.txt | uniq -c | sort -rn | head
来源：http://kop.zhiwuduotai.top

[R52] 统计行数
来源：http://srj.hcnkem.com

wc -l a.txt
来源：http://zzo.yj202588.top

[R53] 查看文件头与实时尾
来源：http://giu.yj20258.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ife.shuidangran.top

[R54] 比较两个文件
来源：http://kec.xuetiantiany.cn

diff a.txt b.txt
来源：http://mch.zhaomingkeji.xyz

[R55] 压缩与解压
来源：http://pog.chenlongwang.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rxq.yuanzhike.top

[R56] 远程拷贝
来源：http://pwk.yfazqb.com

scp file user@host:/path/
来源：http://llg.zhixingplan.top

[R57] 远程执行命令
来源：http://ulr.ctjpmb.com

ssh user@host 'uptime'
来源：http://fee.hywenlv.cn

[R58] 下载文件
来源：http://aew.uphjek.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pos.gogol.net.cn

[R59] 发 POST JSON
来源：http://meh.andypj.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qqh.gzhubu.top

[R60] 只看 HTTP 状态码
来源：http://ixm.dashuyun.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ukt.gotoacloud.top

[R61] 磁盘占用
来源：http://ypi.xingfuxueyuan.xyz

df -h;  du -sh *
来源：http://esq.zhengqikj.top

[R62] 找最占空间的文件
来源：http://ipk.mhx1999.top

du -ah . | sort -rh | head -10
来源：http://xnu.havefunace.top

[R63] 内存与进程
来源：http://nvx.zhiwuduotai.top

free -h;  ps aux | grep nginx
来源：http://eyw.daxiang520.top

[R64] 结束进程
来源：http://rae.nanxinkj.top

kill -9 $(pgrep -f app.py)
来源：http://vti.dianchejie.cn

[R65] 查看端口占用
来源：http://rdr.ctjpmb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xrt.sweek.top

[R66] 定时任务
来源：http://azt.wangdashe.top

crontab -e;  crontab -l
来源：http://fwk.cdnleiting.top

[R67] 生成随机十六进制串
来源：http://tdu.aizwys.cn

openssl rand -hex 16
来源：http://jgy.chenlongwang.top

[R68] 计算文件校验值
来源：http://phb.ywan-chungtsiang.top

sha256sum a.txt;  md5sum a.txt
来源：http://raw.mhx1999.top

[R69] 生成随机密码
来源：http://msp.cqqwz.cn

head -c 16 /dev/urandom | base64
来源：http://btr.bjfxy.top

[R70] 时间戳与互转
来源：http://obd.ctjpmb.com

date +%s;  date -d @1700000000
来源：http://min.hcnkem.com

[R71] 日期格式化
来源：http://men.havefunace.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://wyf.cdnleiting.top

[R72] 等待端口就绪
来源：http://yjx.guannengcc.top

until nc -z localhost 3306; do sleep 1; done
来源：http://iie.aizwys.cn

[R73] 分割大日志
来源：http://tvx.sysykeji.top

split -l 1000 big.log part_
来源：http://qqi.zhengqikj.top

[R74] 批量重命名
来源：http://zqj.zhijiandao.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fph.yj202588.top

[R75] 导出环境变量
来源：http://ext.zhiwuduotai.top

export PATH="$HOME/bin:$PATH"
来源：http://bjf.ehwqpu.com

[R76] 使用临时文件
来源：http://oes.yvedp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://usw.zhongyouzk.top

[R77] 读取用户输入
来源：http://xxe.haohaochexian.top

read -rp "请输入: " ans
来源：http://mzt.dashuyun.cn

[R78] 交互式菜单
来源：http://jra.aizwys.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vzr.epnwcf.com

[R79] 解析命令行选项
来源：http://fpf.aibaodan.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hzk.uphjek.com

[R80] 查看脚本执行耗时
来源：http://ggp.pycfn.com

time ./run.sh
来源：http://hkq.yanxiufei.cn

================================================================================
来源：http://oyd.uphjek.com

S. C / C++ 专题
来源：http://eeq.yj20258.top

================================================================================
来源：http://lyu.hammf.cn

[S01] C：Hello World
来源：http://vod.jinqigfzy.top

#include <stdio.h>
来源：http://kzb.uphjek.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://zej.hammf.cn

[S02] C：变量与格式化输出
来源：http://due.jinyuanbaomall.cn

int a = 10; printf("%d\n", a);
来源：http://kog.ivvv.top

[S03] C：读入整数
来源：http://aza.vehdjk.com

int x; scanf("%d", &x);
来源：http://xud.feifeiyinyue.top

[S04] C：字符串复制
来源：http://ncd.sufxvd.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qhf.ydjk.org.cn

[S05] C：字符串长度
来源：http://dix.jinqigfzy.top

strlen(s)
来源：http://por.yfazqb.com

[S06] C：字符串比较
来源：http://byl.daxiang520.top

strcmp(a, b) == 0
来源：http://csj.yvedp.cn

[S07] C：数组遍历求和
来源：http://hlc.zycfv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gyp.zhiwuduotai.top

[S08] C：动态内存分配与释放
来源：http://ism.aibaodan.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jnm.cheryme.top

[S09] C：结构体定义与初始化
来源：http://vik.hywenlv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xto.yvedp.cn

[S10] C：指针与解引用
来源：http://xik.fzhhl.top

int *p = &a;  *p = 5;
来源：http://bec.hongshengwenyu.top

[S11] C：逐行读文件
来源：http://qfz.svipenyu.cn

FILE *f = fopen("a.txt", "r");
来源：http://cvy.fengsongda.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://iff.ybcxt.top

fclose(f);
来源：http://skz.hywenlv.cn

[S12] C：写文件
来源：http://qxl.svipenyu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ycu.uphjek.com

[S13] C：宏定义
来源：http://mwi.cqqwz.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kja.chenlongwang.top

[S14] C：枚举
来源：http://jwc.hongshengwenyu.top

enum Color { RED, GREEN, BLUE };
来源：http://ozr.zhaomingkeji.xyz

[S15] C：类型转换
来源：http://khd.shangyingyoupin.top

(double) a / b
来源：http://mxi.zhaomingkeji.xyz

[S16] C：位操作置位
来源：http://rme.316326.xyz

x |= (1 << 3);
来源：http://gsn.cqqwz.cn

[S17] C：安全拼接字符串
来源：http://qkq.nanxuanxn.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nru.gotoacloud.top

[S18] C：命令行参数
来源：http://wfw.xinyue.icu

int main(int argc, char **argv)
来源：http://vwp.wangshuangyany.cn

[S19] C：快速排序
来源：http://bnk.tarul.cn

qsort(a, n, sizeof(int), cmp);
来源：http://auh.jinqigufen.top

[S20] C：二分查找
来源：http://tmy.fanxiaobao.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nut.hfpthk.cn

[S21] C：字符类别判断
来源：http://dlp.yfazqb.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rsf.nanxinkj.top

[S22] C：字符串转数字
来源：http://fap.tianlin.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://sch.jinqigfzy.top

[S23] C：随机数
来源：http://jxa.zhiwuduotai.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ngz.wangshuangyany.cn

[S24] C：获取本地时间
来源：http://nwc.jinyuanbaomall.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://imd.gaohongyu789.top

[S25] C：内存拷贝
来源：http://npy.ppjwa.cn

memcpy(dst, src, n);
来源：http://uxo.jianghu66.top

[S26] C：内存清零
来源：http://hsj.cheryme.top

memset(a, 0, sizeof a);
来源：http://dfh.tarul.cn

[S27] C：定义常量
来源：http://sqa.zhaomingkeji.xyz

const double PI = 3.14159;
来源：http://jrb.feifeiyinyue.top

[S28] C：静态变量
来源：http://wso.cqqwz.cn

static int counter = 0;
来源：http://ggi.cheryme.top

[S29] C：变参函数
来源：http://kzs.xziqi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mcf.daxiang520.top

[S30] C：头文件保护
来源：http://fpv.daxiang520.top

#ifndef X_H
来源：http://dpb.xuetiantiany.cn

#define X_H
来源：http://bha.yongpay.top

#endif
来源：http://twh.316326.xyz

[S31] C++：Hello World
来源：http://pfd.andypj.xyz

#include <iostream>
来源：http://gbr.zhongyouzk.top

int main() { std::cout << "Hello\n"; }
来源：http://flu.sufxvd.cn

[S32] C++：字符串
来源：http://ygb.kuanghao11.cn

std::string s = "hi";  s += "!";
来源：http://vkl.wangdashe.top

[S33] C++：vector 增删
来源：http://rfr.ydzc1.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rig.yuxming.cn

[S34] C++：遍历 vector
来源：http://csh.shanyushiyangkeji.top

for (auto &x : v) { std::cout << x; }
来源：http://vfp.bjfxy.top

[S35] C++：map
来源：http://lbz.yangfankeji.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nhr.meibo888.top

[S36] C++：unordered_map
来源：http://yju.xingfuxueyuan.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fxy.dashuyun.cn

[S37] C++：set
来源：http://klr.yuanzhike.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vcs.daria6918.cn

[S38] C++：排序
来源：http://thw.yuanzhike.top

std::sort(v.begin(), v.end());
来源：http://mzn.xylfe.cn

[S39] C++：自定义比较器排序
来源：http://fqn.hywenlv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nip.uphjek.com

[S40] C++：查找元素
来源：http://sxr.yuanzhike.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jov.tarul.cn

[S41] C++：类与构造函数
来源：http://deb.9152youxi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wft.hnqzz.top

[S42] C++：继承与虚函数
来源：http://eca.fengsongda.top

class B : public Base { public: void f() override {} };
来源：http://wil.316326.xyz

[S43] C++：智能指针
来源：http://sdf.9152youxi.cn

auto p = std::make_unique<int>(5);
来源：http://kcj.xylfe.cn

[S44] C++：引用传参
来源：http://auf.yueranfly.top

void inc(int &x) { ++x; }
来源：http://uey.jqgfzy.top

[S45] C++：lambda
来源：http://ykj.yuanzhike.top

auto add = [](int a, int b) { return a + b; };
来源：http://rwa.cucudq.cn

[S46] C++：函数模板
来源：http://lqb.tian-w.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://itg.ybcxt.top

[S47] C++：结构化绑定遍历
来源：http://abe.sxryk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dai.vqdsnc.cn

[S48] C++：逐行读文件
来源：http://hfh.nwbrower.top

std::ifstream in("a.txt");  std::string line;
来源：http://lii.guannengcc.top

while (std::getline(in, line)) { }
来源：http://wjt.vqdsnc.cn

[S49] C++：写文件
来源：http://zsb.quarkkingdee.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ykj.guowangkeji.top

[S50] C++：格式化数字
来源：http://yge.cqqwz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://iia.xuetiantiany.cn

[S51] C++：显式类型转换
来源：http://avn.birdmap.top

static_cast<double>(a) / b
来源：http://vuo.jiagoushi.top

[S52] C++：const 与 noexcept
来源：http://rwr.yj20258888.top

int size() const noexcept { return n_; }
来源：http://zyq.jlsjyb.cn

[S53] C++：移动语义
来源：http://pnk.jlsjyb.cn

std::vector<int> w = std::move(v);
来源：http://qfd.xinyue.icu

[S54] C++：异常处理
来源：http://yij.feifeiyinyue.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cir.pengpengdd.cyou

[S55] C++：结构化绑定
来源：http://jou.haohaochexian.top

auto [a, b] = std::make_pair(1, 2);
来源：http://oez.zycfv.cn

[S56] C++：optional
来源：http://gry.shanyushiyangtech.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xmy.jqgfzy.top

[S57] C++：编译期常量
来源：http://kex.daria6918.cn

constexpr int N = 10;
来源：http://zcz.mhx1999.top

[S58] C++：命名空间
来源：http://qcc.yfazqb.com

namespace ns { int f() { return 1; } }
来源：http://ouv.jyoumei.cn

[S59] C++：静态断言
来源：http://ygw.smart0.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yvz.pengpengdd.cyou

[S60] C++：遍历并删除元素
来源：http://snl.quarkkingdee.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vdf.316326.xyz

================================================================================
来源：http://sdw.xuetiantiany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vez.birdmap.top

================================================================================
来源：http://vmo.uphjek.com

[T01] Kotlin：Hello World
来源：http://fqo.yangfankeji.com

println("Hello")
来源：http://ofy.xuanzx.com

[T02] Kotlin：变量
来源：http://ytk.uphjek.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uvz.ppjwa.cn

[T03] Kotlin：字符串模板
来源：http://cnx.cqqwz.cn

"值: $b"
来源：http://wqm.haohaochexian.top

[T04] Kotlin：空安全
来源：http://gfi.cdnleiting.top

val n: String? = null;  n?.length
来源：http://tjt.yvedp.cn

[T05] Kotlin：when 表达式
来源：http://wrc.9152youxi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ibm.vqdsnc.cn

[T06] Kotlin：集合映射
来源：http://uli.birdmap.top

listOf(1, 2, 3).map { it * 2 }
来源：http://uyq.sweek.top

[T07] Kotlin：集合过滤
来源：http://toc.xuanzx.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://ely.hcnkem.com

[T08] Kotlin：数据类
来源：http://oxu.xuetiantiany.cn

data class User(val name: String, val age: Int)
来源：http://liv.gzhubu.top

[T09] Kotlin：扩展函数
来源：http://cza.yanxiufei.cn

fun String.exclaim() = this + "!"
来源：http://tla.316326.xyz

[T10] Kotlin：默认参数
来源：http://ujs.yvedp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jiw.wangshuangyany.cn

[T11] Kotlin：协程
来源：http://uqe.chenlongwang.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ung.yangfankeji.com

[T12] Kotlin：解构声明
来源：http://luj.jinyuanbaomall.cn

val (a, b) = Pair(1, 2)
来源：http://fif.nwbrower.top

[T13] Kotlin：只读 Map
来源：http://zze.zhengqikj.top

val m = mapOf("a" to 1)
来源：http://sww.xylfe.cn

[T14] Kotlin：循环
来源：http://gth.jinyuanbaomall.cn

for (i in 1..10) println(i)
来源：http://cqi.jqgfzy.top

[T15] Kotlin：接口
来源：http://xrs.ehwqpu.com

interface Shape { fun area(): Double }
来源：http://ypr.yj20258.top

[T16] Swift：Hello World
来源：http://ftm.svipenyu.cn

print("Hello")
来源：http://ske.smart0.xyz

[T17] Swift：变量与常量
来源：http://hbj.hnxiangtu.top

var a = 1;  let b = 2
来源：http://pqy.tanke756.top

[T18] Swift：字符串插值
来源：http://pzk.sweek.top

"值: \(b)"
来源：http://kvr.dashuyun.cn

[T19] Swift：可选绑定
来源：http://lix.wangdashe.top

if let n = opt { print(n) }
来源：http://hex.nanxinkj.top

[T20] Swift：数组操作
来源：http://oaw.quarkkingdee.top

var a = [1, 2, 3];  a.append(4)
来源：http://kbl.dashuyun.cn

[T21] Swift：遍历
来源：http://adq.ppjwa.cn

for x in a { print(x) }
来源：http://kfo.yj20258.top

[T22] Swift：字典
来源：http://ybq.zhongyouzk.top

var d = ["a": 1];  d["b"] = 2
来源：http://miw.cdnleiting.top

[T23] Swift：函数
来源：http://idj.zhongyouzk.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ajj.meibo888.top

[T24] Swift：闭包
来源：http://xbq.smart0.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://ban.ydzc1.top

[T25] Swift：结构体
来源：http://nrv.dianchejie.cn

struct P { var x: Int }
来源：http://ald.vqdsnc.cn

[T26] Swift：类与重写
来源：http://pvi.ctjpmb.com

class A: Base { override func f() {} }
来源：http://soa.xziqi.cn

[T27] Swift：错误处理
来源：http://ojs.vqdsnc.cn

do { try f() } catch { print(error) }
来源：http://sqd.bjfxy.top

[T28] Swift：枚举
来源：http://dvr.fehbvm.com

enum Color { case red, green }
来源：http://bhx.jinyuanbaomall.cn

[T29] Swift：guard 提前返回
来源：http://urg.jiagoushi.top

guard let x = opt else { return }
来源：http://tot.chenlongwang.top

[T30] Swift：协议
来源：http://jkn.jinqigufen.top

protocol Shape { func area() -> Double }
来源：http://qph.hcnkem.com

[T31] Lua：Hello World
来源：http://mtf.zhengqikj.top

print("Hello")
来源：http://bom.pycfn.com

[T32] Lua：局部变量
来源：http://eol.sjlbkw.cn

local a = 1
来源：http://hwi.jinghuilouyu.cn

[T33] Lua：表（数组）
来源：http://uvg.zhaomingkeji.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://qkz.andypj.xyz

[T34] Lua：遍历表
来源：http://jmp.bjfxy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://xvk.haohaochexian.top

[T35] Lua：字典表
来源：http://fqf.fengsongda.top

local d = { a = 1 };  d.b = 2
来源：http://mha.aizwys.cn

[T36] Lua：函数
来源：http://rbn.yuxming.cn

function add(a, b) return a + b end
来源：http://cmx.zhongyouzk.top


<!-- 参考信息 -->