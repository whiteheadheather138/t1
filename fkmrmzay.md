代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rkx.cashguo.top

[R34] 退出时清理
来源：http://phi.tian-w.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ehd.xuanzx.com

[R35] 后台执行并等待
来源：http://ogc.uphjek.com

sleep 5 & pid=$!; wait "$pid"
来源：http://rsm.ybcxt.top

[R36] 并发执行多个任务
来源：http://myo.ivvv.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://iur.nanxuanxn.top

[R37] 把输出赋给变量
来源：http://hyk.sysykeji.top

files=$(ls -1)
来源：http://dhz.nanxuanxn.top

[R38] 管道串联
来源：http://hlf.cqqwz.cn

cat a.txt | grep -i error | wc -l
来源：http://yfx.zdbjq.cn

[R39] 重定向标准输出与错误
来源：http://yzz.haohaochexian.top

cmd > out.log 2>&1
来源：http://kur.zycfv.cn

[R40] 追加写日志
来源：http://vfg.9152youxi.cn

echo "log" >> out.log
来源：http://crd.cheryme.top

[R41] 丢弃输出
来源：http://nwj.shzxlz.cn

cmd >/dev/null 2>&1
来源：http://dvk.hnxiangtu.top

[R42] 输入重定向
来源：http://bms.316326.xyz

wc -l < a.txt
来源：http://sbx.xuanzx.com

[R43] 按名字查找文件
来源：http://tme.jiagoushi.top

find . -name "*.log" -type f
来源：http://ycm.shanyushiyangtech.top

[R44] 按修改时间查找
来源：http://kji.dashuyun.cn

find . -mtime -7 -type f
来源：http://cpg.sjlbkw.cn

[R45] 批量删除
来源：http://sbu.pengpengdd.cyou

find . -name "*.tmp" -delete
来源：http://fsr.sxryk.cn

[R46] 递归替换文件内容
来源：http://ydx.gotoacloud.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tvg.shangyingyoupin.top

[R47] sed 单行替换
来源：http://cjt.gaohongyu789.top

sed -i 's/foo/bar/g' a.txt
来源：http://cwn.xingfuxueyuan.xyz

[R48] awk 取指定列
来源：http://asr.sufxvd.cn

awk '{print $1, $3}' a.txt
来源：http://fmm.chenzaomai.com

[R49] awk 带条件
来源：http://ybo.iojbl.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gun.chenjidiqi.icu

[R50] awk 求和
来源：http://ple.0kj1m.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fsm.daxiang520.top

[R51] 排序去重取前几
来源：http://nxr.hongshengwenyu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://gjy.cdnleiting.top

[R52] 统计行数
来源：http://nhm.0kj1m.cn

wc -l a.txt
来源：http://ita.sweek.top

[R53] 查看文件头与实时尾
来源：http://cwe.cqqwz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qat.wangshuangyany.cn

[R54] 比较两个文件
来源：http://aab.tarul.cn

diff a.txt b.txt
来源：http://xyf.smart0.xyz

[R55] 压缩与解压
来源：http://hnc.sysykeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ibm.yanxiufei.cn

[R56] 远程拷贝
来源：http://psf.zhengqikj.top

scp file user@host:/path/
来源：http://oqq.nwbrower.top

[R57] 远程执行命令
来源：http://klk.cucudq.cn

ssh user@host 'uptime'
来源：http://drr.tarul.cn

[R58] 下载文件
来源：http://nun.sweek.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://soy.jinyuanbaomall.cn

[R59] 发 POST JSON
来源：http://okd.fzhhl.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://asa.redwolf501.top

[R60] 只看 HTTP 状态码
来源：http://rqs.vqdsnc.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sfe.andypj.xyz

[R61] 磁盘占用
来源：http://mwu.316326.xyz

df -h;  du -sh *
来源：http://ejd.havefunace.top

[R62] 找最占空间的文件
来源：http://idu.zhengqikj.top

du -ah . | sort -rh | head -10
来源：http://vst.xuetiantiany.cn

[R63] 内存与进程
来源：http://vbv.xziqi.cn

free -h;  ps aux | grep nginx
来源：http://yhj.redwolf501.top

[R64] 结束进程
来源：http://bmh.sjlbkw.cn

kill -9 $(pgrep -f app.py)
来源：http://qtp.ydzc1.top

[R65] 查看端口占用
来源：http://zok.nanxinkj.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xdn.xingfuxueyuan.xyz

[R66] 定时任务
来源：http://wzh.nwbrower.top

crontab -e;  crontab -l
来源：http://fbs.svipenyu.cn

[R67] 生成随机十六进制串
来源：http://akt.bjfxy.top

openssl rand -hex 16
来源：http://ges.jiagoushi.top

[R68] 计算文件校验值
来源：http://scu.xylfe.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rot.smart0.xyz

[R69] 生成随机密码
来源：http://owk.dashuyun.cn

head -c 16 /dev/urandom | base64
来源：http://mdw.cdnleiting.top

[R70] 时间戳与互转
来源：http://qwd.meibo888.top

date +%s;  date -d @1700000000
来源：http://cyq.zdqjudy.top

[R71] 日期格式化
来源：http://knr.svipenyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jej.sufxvd.cn

[R72] 等待端口就绪
来源：http://dld.pengpengdd.cyou

until nc -z localhost 3306; do sleep 1; done
来源：http://rja.ctjpmb.com

[R73] 分割大日志
来源：http://ivk.zhijiandao.cn

split -l 1000 big.log part_
来源：http://vvj.fengsongda.top

[R74] 批量重命名
来源：http://yfs.smart0.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kqr.nanxinkj.top

[R75] 导出环境变量
来源：http://wau.bjfxy.top

export PATH="$HOME/bin:$PATH"
来源：http://van.ydzc1.top

[R76] 使用临时文件
来源：http://cuy.shuidangran.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qqv.smart0.xyz

[R77] 读取用户输入
来源：http://hdu.shuidangran.top

read -rp "请输入: " ans
来源：http://isk.xingfuxueyuan.xyz

[R78] 交互式菜单
来源：http://bwx.kuanghao11.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://our.jinyuanbaomall.cn

[R79] 解析命令行选项
来源：http://oop.gogol.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mpk.redwolf501.top

[R80] 查看脚本执行耗时
来源：http://who.yvedp.cn

time ./run.sh
来源：http://bjw.cashguo.top

================================================================================
来源：http://bux.jlsjyb.cn

S. C / C++ 专题
来源：http://nig.chenjidiqi.icu

================================================================================
来源：http://dch.hcnkem.com

[S01] C：Hello World
来源：http://yom.wangshuangyany.cn

#include <stdio.h>
来源：http://jfp.pengpengdd.cyou

int main(void) { printf("Hello\n"); return 0; }
来源：http://led.guannengcc.top

[S02] C：变量与格式化输出
来源：http://egj.shanyushiyangkeji.top

int a = 10; printf("%d\n", a);
来源：http://lcp.chenzaomai.com

[S03] C：读入整数
来源：http://iat.vehdjk.com

int x; scanf("%d", &x);
来源：http://tlj.zhengqikj.top

[S04] C：字符串复制
来源：http://lpo.ehwqpu.com

char dst[32]; strcpy(dst, "hi");
来源：http://zhv.epnwcf.com

[S05] C：字符串长度
来源：http://khj.chenzaomai.com

strlen(s)
来源：http://qph.tian-w.cn

[S06] C：字符串比较
来源：http://ncw.hongshengwenyu.top

strcmp(a, b) == 0
来源：http://mck.0kj1m.cn

[S07] C：数组遍历求和
来源：http://snq.dashuyun.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qbz.yanxiufei.cn

[S08] C：动态内存分配与释放
来源：http://xfp.ivvv.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uja.cqqwz.cn

[S09] C：结构体定义与初始化
来源：http://lpw.ydjk.org.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bjo.jinghuilouyu.cn

[S10] C：指针与解引用
来源：http://acq.zdbjq.cn

int *p = &a;  *p = 5;
来源：http://fpv.ehwqpu.com

[S11] C：逐行读文件
来源：http://zjl.shzxlz.cn

FILE *f = fopen("a.txt", "r");
来源：http://vgi.yuanzhike.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://nse.fktsv.cn

fclose(f);
来源：http://kep.yueranfly.top

[S12] C：写文件
来源：http://bli.316326.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://joc.hfpthk.cn

[S13] C：宏定义
来源：http://nje.zhaomingkeji.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ezj.gotoacloud.top

[S14] C：枚举
来源：http://qjg.yongpay.top

enum Color { RED, GREEN, BLUE };
来源：http://now.gaohongyu789.top

[S15] C：类型转换
来源：http://gyt.wangshuangyany.cn

(double) a / b
来源：http://mzv.vqdsnc.cn

[S16] C：位操作置位
来源：http://lkt.xylfe.cn

x |= (1 << 3);
来源：http://flx.cucudq.cn

[S17] C：安全拼接字符串
来源：http://nbv.0kj1m.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yce.cucudq.cn

[S18] C：命令行参数
来源：http://wby.zhixingplan.top

int main(int argc, char **argv)
来源：http://vgx.zycfv.cn

[S19] C：快速排序
来源：http://oet.wangshuangyany.cn

qsort(a, n, sizeof(int), cmp);
来源：http://upv.yj20258888.top

[S20] C：二分查找
来源：http://hqu.uphjek.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rzl.c1oappe.top

[S21] C：字符类别判断
来源：http://zuz.zhiwuduotai.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hfr.tianlin.xyz

[S22] C：字符串转数字
来源：http://qkf.gotoacloud.top

atoi("42");  strtod("3.14", NULL);
来源：http://zis.smart0.xyz

[S23] C：随机数
来源：http://rxw.guowangkeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://zwn.nanxuanxn.top

[S24] C：获取本地时间
来源：http://xdd.xziqi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ifs.9152youxi.cn

[S25] C：内存拷贝
来源：http://vnv.yueranfly.top

memcpy(dst, src, n);
来源：http://fjy.yfazqb.com

[S26] C：内存清零
来源：http://hzs.gotoacloud.top

memset(a, 0, sizeof a);
来源：http://tco.tarul.cn

[S27] C：定义常量
来源：http://ghc.hcnkem.com

const double PI = 3.14159;
来源：http://sfi.nanxuanxn.top

[S28] C：静态变量
来源：http://vla.wangdashe.top

static int counter = 0;
来源：http://qgd.zycfv.cn

[S29] C：变参函数
来源：http://jrg.nwbrower.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://adl.sxryk.cn

[S30] C：头文件保护
来源：http://cgd.guannengcc.top

#ifndef X_H
来源：http://dpv.cqqwz.cn

#define X_H
来源：http://epe.zhixingplan.top

#endif
来源：http://fqs.jinghuilouyu.cn

[S31] C++：Hello World
来源：http://amz.xingfuxueyuan.xyz

#include <iostream>
来源：http://hln.shanyushiyangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://hoo.aibaodan.cn

[S32] C++：字符串
来源：http://mnd.xinyue.icu

std::string s = "hi";  s += "!";
来源：http://xfp.xingfuxueyuan.xyz

[S33] C++：vector 增删
来源：http://uvc.zdbjq.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bcf.jinqigufen.top

[S34] C++：遍历 vector
来源：http://cte.c1oappe.top

for (auto &x : v) { std::cout << x; }
来源：http://vqj.xingfuxueyuan.xyz

[S35] C++：map
来源：http://ccr.nwbrower.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lsd.gzhubu.top

[S36] C++：unordered_map
来源：http://gbc.yj20258888.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://udr.pycfn.com

[S37] C++：set
来源：http://tdq.yueranfly.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lda.jyoumei.cn

[S38] C++：排序
来源：http://jbg.hammf.cn

std::sort(v.begin(), v.end());
来源：http://goi.chenjidiqi.icu

[S39] C++：自定义比较器排序
来源：http://dhp.yuxming.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mzj.xylfe.cn

[S40] C++：查找元素
来源：http://tpu.zhixingplan.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qhe.shanyushiyangtech.top

[S41] C++：类与构造函数
来源：http://gwi.sjlbkw.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bkr.redwolf501.top

[S42] C++：继承与虚函数
来源：http://fiu.ywan-chungtsiang.top

class B : public Base { public: void f() override {} };
来源：http://jbh.aizwys.cn

[S43] C++：智能指针
来源：http://cfg.epnwcf.com

auto p = std::make_unique<int>(5);
来源：http://hif.xuanzx.com

[S44] C++：引用传参
来源：http://gut.cheryme.top

void inc(int &x) { ++x; }
来源：http://mad.zhoulong.xyz

[S45] C++：lambda
来源：http://cih.andypj.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://vko.jinqigfzy.top

[S46] C++：函数模板
来源：http://epk.hfpthk.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ole.wangdashe.top

[S47] C++：结构化绑定遍历
来源：http://epm.zhengqikj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cvd.aizwys.cn

[S48] C++：逐行读文件
来源：http://uww.yanxiufei.cn

std::ifstream in("a.txt");  std::string line;
来源：http://poj.zhoulong.xyz

while (std::getline(in, line)) { }
来源：http://sbt.yuxming.cn

[S49] C++：写文件
来源：http://mdb.zhengqikj.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lcw.ydjk.org.cn

[S50] C++：格式化数字
来源：http://zfa.yj20258888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xal.yj20258888.top

[S51] C++：显式类型转换
来源：http://vju.mhx1999.top

static_cast<double>(a) / b
来源：http://fdj.ivvv.top

[S52] C++：const 与 noexcept
来源：http://lcr.yuxming.cn

int size() const noexcept { return n_; }
来源：http://unm.yangfankeji.com

[S53] C++：移动语义
来源：http://avg.andypj.xyz

std::vector<int> w = std::move(v);
来源：http://vpv.hesvh.cn

[S54] C++：异常处理
来源：http://khf.cqqwz.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bsf.redwolf501.top

[S55] C++：结构化绑定
来源：http://ogz.tanke756.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zpd.yuanzhike.top

[S56] C++：optional
来源：http://gjv.pycfn.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uoe.tarul.cn

[S57] C++：编译期常量
来源：http://yvw.hysaishi.cn

constexpr int N = 10;
来源：http://roo.xylfe.cn

[S58] C++：命名空间
来源：http://efw.svipenyu.cn

namespace ns { int f() { return 1; } }
来源：http://acu.daria6918.cn

[S59] C++：静态断言
来源：http://gee.birdmap.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fkh.gogol.net.cn

[S60] C++：遍历并删除元素
来源：http://qib.zycfv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rsh.shzxlz.cn

================================================================================
来源：http://zvr.xylfe.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gxa.vqdsnc.cn

================================================================================
来源：http://xxs.jyoumei.cn

[T01] Kotlin：Hello World
来源：http://ktx.birdmap.top

println("Hello")
来源：http://arg.cheryme.top

[T02] Kotlin：变量
来源：http://all.zhoulong.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yht.jianghu66.top

[T03] Kotlin：字符串模板
来源：http://vvu.zhoulong.xyz

"值: $b"
来源：http://brs.xuetiantiany.cn

[T04] Kotlin：空安全
来源：http://wpj.9152youxi.cn

val n: String? = null;  n?.length
来源：http://fds.vqdsnc.cn

[T05] Kotlin：when 表达式
来源：http://hlm.nanxuanxn.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dac.jinyuanbaomall.cn

[T06] Kotlin：集合映射
来源：http://oas.pengpengdd.cyou

listOf(1, 2, 3).map { it * 2 }
来源：http://uus.zdqjudy.top

[T07] Kotlin：集合过滤
来源：http://pvn.zhixingplan.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://uao.yvedp.cn

[T08] Kotlin：数据类
来源：http://vmd.0kj1m.cn

data class User(val name: String, val age: Int)
来源：http://les.xuanzx.com

[T09] Kotlin：扩展函数
来源：http://laa.wangdashe.top

fun String.exclaim() = this + "!"
来源：http://egl.jiagoushi.top

[T10] Kotlin：默认参数
来源：http://fcp.zdbjq.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gbj.shzxlz.cn

[T11] Kotlin：协程
来源：http://hgz.yvedp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://egw.xuanzx.com

[T12] Kotlin：解构声明
来源：http://lhr.pycfn.com

val (a, b) = Pair(1, 2)
来源：http://hpw.0kj1m.cn

[T13] Kotlin：只读 Map
来源：http://cea.xingfuxueyuan.xyz

val m = mapOf("a" to 1)
来源：http://xez.haohaochexian.top

[T14] Kotlin：循环
来源：http://zqr.zhaomingkeji.xyz

for (i in 1..10) println(i)
来源：http://wvj.yvedp.cn

[T15] Kotlin：接口
来源：http://itm.smart0.xyz

interface Shape { fun area(): Double }
来源：http://hpz.iojbl.cn

[T16] Swift：Hello World
来源：http://wgl.jqgufenzy.top

print("Hello")
来源：http://zgs.jianghu66.top

[T17] Swift：变量与常量
来源：http://jmr.shuidangran.top

var a = 1;  let b = 2
来源：http://ggi.dashuyun.cn

[T18] Swift：字符串插值
来源：http://wfa.jyoumei.cn

"值: \(b)"
来源：http://lsc.zhijiandao.cn

[T19] Swift：可选绑定
来源：http://hst.316326.xyz

if let n = opt { print(n) }
来源：http://hse.svipenyu.cn

[T20] Swift：数组操作
来源：http://wvl.jinqigufen.top

var a = [1, 2, 3];  a.append(4)
来源：http://jka.pycfn.com

[T21] Swift：遍历
来源：http://efe.chenlongwang.top

for x in a { print(x) }
来源：http://tbh.ydjk.org.cn

[T22] Swift：字典
来源：http://ffn.iojbl.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kde.yanxiufei.cn

[T23] Swift：函数
来源：http://zlw.zhongyouzk.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dcn.zhongyouzk.top

[T24] Swift：闭包
来源：http://xbg.hywenlv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vbo.daria6918.cn

[T25] Swift：结构体
来源：http://skz.yuanzhike.top

struct P { var x: Int }
来源：http://ylj.snrcjt.cn

[T26] Swift：类与重写
来源：http://pzc.pycfn.com

class A: Base { override func f() {} }
来源：http://vol.hammf.cn

[T27] Swift：错误处理
来源：http://fgj.tarul.cn

do { try f() } catch { print(error) }
来源：http://cxj.ehwqpu.com

[T28] Swift：枚举
来源：http://czb.fktsv.cn

enum Color { case red, green }
来源：http://ouu.daxiang520.top

[T29] Swift：guard 提前返回
来源：http://qub.ydzc1.top

guard let x = opt else { return }
来源：http://qkl.jqgfzy.top

[T30] Swift：协议
来源：http://pef.gotoacloud.top

protocol Shape { func area() -> Double }
来源：http://rzr.jlsjyb.cn

[T31] Lua：Hello World
来源：http://cry.zhixingplan.top

print("Hello")
来源：http://yoa.sjlbkw.cn

[T32] Lua：局部变量
来源：http://bxc.316326.xyz

local a = 1
来源：http://rqq.cucudq.cn

[T33] Lua：表（数组）
来源：http://uro.cheryme.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ruz.jinghuilouyu.cn

[T34] Lua：遍历表
来源：http://inz.jyoumei.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nfk.hnxiangtu.top

[T35] Lua：字典表
来源：http://wce.guannengcc.top

local d = { a = 1 };  d.b = 2
来源：http://mnq.yj202588.top

[T36] Lua：函数
来源：http://dib.fzhhl.top

function add(a, b) return a + b end
来源：http://euq.vqdsnc.cn


<!-- 参考信息 -->