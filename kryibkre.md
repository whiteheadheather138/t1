代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://grs.chenlongwang.top

[R34] 退出时清理
来源：http://rju.andypj.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://ytm.ivvv.top

[R35] 后台执行并等待
来源：http://bqo.daria6918.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lhz.fktsv.cn

[R36] 并发执行多个任务
来源：http://cvk.bjfxy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vfq.9152youxi.cn

[R37] 把输出赋给变量
来源：http://bko.zhaomingkeji.xyz

files=$(ls -1)
来源：http://jcj.yvedp.cn

[R38] 管道串联
来源：http://tub.sxryk.cn

cat a.txt | grep -i error | wc -l
来源：http://gfv.jiagoushi.top

[R39] 重定向标准输出与错误
来源：http://glg.zhoulong.xyz

cmd > out.log 2>&1
来源：http://sjj.gaohongyu789.top

[R40] 追加写日志
来源：http://azl.pycfn.com

echo "log" >> out.log
来源：http://opo.sysykeji.top

[R41] 丢弃输出
来源：http://pkz.xingfuxueyuan.xyz

cmd >/dev/null 2>&1
来源：http://juq.pengpengdd.cyou

[R42] 输入重定向
来源：http://nsn.tanke756.top

wc -l < a.txt
来源：http://bzc.zhongyouzk.top

[R43] 按名字查找文件
来源：http://igm.shuidangran.top

find . -name "*.log" -type f
来源：http://oha.ivvv.top

[R44] 按修改时间查找
来源：http://iah.sysykeji.top

find . -mtime -7 -type f
来源：http://nje.fehbvm.com

[R45] 批量删除
来源：http://yes.zdqjudy.top

find . -name "*.tmp" -delete
来源：http://aen.cheryme.top

[R46] 递归替换文件内容
来源：http://gov.sweek.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vsn.nwbrower.top

[R47] sed 单行替换
来源：http://vuf.fengsongda.top

sed -i 's/foo/bar/g' a.txt
来源：http://ubu.xuetiantiany.cn

[R48] awk 取指定列
来源：http://ahs.ydzc1.top

awk '{print $1, $3}' a.txt
来源：http://pjj.hfpthk.cn

[R49] awk 带条件
来源：http://vrt.mhx1999.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gaf.yuxming.cn

[R50] awk 求和
来源：http://jur.sufxvd.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sqx.yj20258888.top

[R51] 排序去重取前几
来源：http://lln.yanxiufei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://crj.gogol.net.cn

[R52] 统计行数
来源：http://jfj.fanxiaobao.xyz

wc -l a.txt
来源：http://qlz.shzxlz.cn

[R53] 查看文件头与实时尾
来源：http://bkd.nanxinkj.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qow.zycfv.cn

[R54] 比较两个文件
来源：http://yvv.sysykeji.top

diff a.txt b.txt
来源：http://qcy.jqgfzy.top

[R55] 压缩与解压
来源：http://rjd.birdmap.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yuz.yvedp.cn

[R56] 远程拷贝
来源：http://vrw.daria6918.cn

scp file user@host:/path/
来源：http://csm.zdbjq.cn

[R57] 远程执行命令
来源：http://bgh.shuidangran.top

ssh user@host 'uptime'
来源：http://adl.xuetiantiany.cn

[R58] 下载文件
来源：http://zoe.ivvv.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ipn.jyoumei.cn

[R59] 发 POST JSON
来源：http://noi.gzhubu.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hti.chenlongwang.top

[R60] 只看 HTTP 状态码
来源：http://hzx.ehwqpu.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nhg.cashguo.top

[R61] 磁盘占用
来源：http://hzg.shanyushiyangtech.top

df -h;  du -sh *
来源：http://xsy.chenjidiqi.icu

[R62] 找最占空间的文件
来源：http://ozq.tanke756.top

du -ah . | sort -rh | head -10
来源：http://fyu.yj20258.top

[R63] 内存与进程
来源：http://ren.hammf.cn

free -h;  ps aux | grep nginx
来源：http://qeu.xylfe.cn

[R64] 结束进程
来源：http://zth.bjfxy.top

kill -9 $(pgrep -f app.py)
来源：http://tcm.cashguo.top

[R65] 查看端口占用
来源：http://giz.wangdashe.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mne.ydjk.org.cn

[R66] 定时任务
来源：http://vzx.jinqigufen.top

crontab -e;  crontab -l
来源：http://xlm.fehbvm.com

[R67] 生成随机十六进制串
来源：http://kyu.ehwqpu.com

openssl rand -hex 16
来源：http://geu.hammf.cn

[R68] 计算文件校验值
来源：http://mue.svipenyu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://osp.xziqi.cn

[R69] 生成随机密码
来源：http://ztk.yongpay.top

head -c 16 /dev/urandom | base64
来源：http://aij.jlsjyb.cn

[R70] 时间戳与互转
来源：http://fxf.smart0.xyz

date +%s;  date -d @1700000000
来源：http://qvg.dianchejie.cn

[R71] 日期格式化
来源：http://bgb.iojbl.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://umf.daxiang520.top

[R72] 等待端口就绪
来源：http://zzm.tian-w.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ncm.zhongyouzk.top

[R73] 分割大日志
来源：http://yiq.shanyushiyangkeji.top

split -l 1000 big.log part_
来源：http://kup.jinqigfzy.top

[R74] 批量重命名
来源：http://tcy.aizwys.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://knm.zhongyouzk.top

[R75] 导出环境变量
来源：http://cto.tian-w.cn

export PATH="$HOME/bin:$PATH"
来源：http://bxa.hywenlv.cn

[R76] 使用临时文件
来源：http://tgx.hongshengwenyu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lpg.andypj.xyz

[R77] 读取用户输入
来源：http://div.yj202588.top

read -rp "请输入: " ans
来源：http://rqr.zdqjudy.top

[R78] 交互式菜单
来源：http://qci.guowangkeji.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hwq.yj202588.top

[R79] 解析命令行选项
来源：http://dwl.zycfv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bej.wangdashe.top

[R80] 查看脚本执行耗时
来源：http://rpy.ybcxt.top

time ./run.sh
来源：http://mab.cashguo.top

================================================================================
来源：http://bcg.vehdjk.com

S. C / C++ 专题
来源：http://kkb.yuxming.cn

================================================================================
来源：http://csi.hongshengwenyu.top

[S01] C：Hello World
来源：http://qdq.hfpthk.cn

#include <stdio.h>
来源：http://mos.jyoumei.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://eug.fehbvm.com

[S02] C：变量与格式化输出
来源：http://iwc.mhx1999.top

int a = 10; printf("%d\n", a);
来源：http://ztq.c1oappe.top

[S03] C：读入整数
来源：http://xtq.vehdjk.com

int x; scanf("%d", &x);
来源：http://bof.dianchejie.cn

[S04] C：字符串复制
来源：http://ncn.cheryme.top

char dst[32]; strcpy(dst, "hi");
来源：http://ajv.andypj.xyz

[S05] C：字符串长度
来源：http://zba.0kj1m.cn

strlen(s)
来源：http://fco.chenlongwang.top

[S06] C：字符串比较
来源：http://qcv.haohaochexian.top

strcmp(a, b) == 0
来源：http://gon.chenlongwang.top

[S07] C：数组遍历求和
来源：http://fap.cheryme.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eye.shanyushiyangtech.top

[S08] C：动态内存分配与释放
来源：http://jhq.dashuyun.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://udq.ehwqpu.com

[S09] C：结构体定义与初始化
来源：http://xvt.9152youxi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zta.chenjidiqi.icu

[S10] C：指针与解引用
来源：http://vtk.yj202588.top

int *p = &a;  *p = 5;
来源：http://wsy.ydjk.org.cn

[S11] C：逐行读文件
来源：http://cbi.vehdjk.com

FILE *f = fopen("a.txt", "r");
来源：http://vag.tanke756.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://tuk.andypj.xyz

fclose(f);
来源：http://ghy.pycfn.com

[S12] C：写文件
来源：http://ine.zycfv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pkk.sjlbkw.cn

[S13] C：宏定义
来源：http://xqp.gotoacloud.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mum.zycfv.cn

[S14] C：枚举
来源：http://nvc.haohaochexian.top

enum Color { RED, GREEN, BLUE };
来源：http://ejs.yj20258888.top

[S15] C：类型转换
来源：http://goe.shanyushiyangkeji.top

(double) a / b
来源：http://ppj.0kj1m.cn

[S16] C：位操作置位
来源：http://orc.hysaishi.cn

x |= (1 << 3);
来源：http://wlq.yanxiufei.cn

[S17] C：安全拼接字符串
来源：http://ncp.xuetiantiany.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zat.hcnkem.com

[S18] C：命令行参数
来源：http://zps.ppjwa.cn

int main(int argc, char **argv)
来源：http://ljm.sufxvd.cn

[S19] C：快速排序
来源：http://gej.vqdsnc.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gve.xinyue.icu

[S20] C：二分查找
来源：http://pvd.fzhhl.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://efq.guannengcc.top

[S21] C：字符类别判断
来源：http://yiy.sjlbkw.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://czd.ywan-chungtsiang.top

[S22] C：字符串转数字
来源：http://ojb.vehdjk.com

atoi("42");  strtod("3.14", NULL);
来源：http://dao.jiagoushi.top

[S23] C：随机数
来源：http://gue.cashguo.top

srand(time(NULL));  int r = rand() % 100;
来源：http://oxh.zhixingplan.top

[S24] C：获取本地时间
来源：http://hel.yfazqb.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://omm.zhengqikj.top

[S25] C：内存拷贝
来源：http://qsp.nwbrower.top

memcpy(dst, src, n);
来源：http://uvw.yanxiufei.cn

[S26] C：内存清零
来源：http://xmh.ydjk.org.cn

memset(a, 0, sizeof a);
来源：http://eos.jianghu66.top

[S27] C：定义常量
来源：http://har.xuanzx.com

const double PI = 3.14159;
来源：http://uer.fanxiaobao.xyz

[S28] C：静态变量
来源：http://ipi.nanxinkj.top

static int counter = 0;
来源：http://usd.gogol.net.cn

[S29] C：变参函数
来源：http://ejm.feifeiyinyue.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pka.guowangkeji.top

[S30] C：头文件保护
来源：http://bfm.zycfv.cn

#ifndef X_H
来源：http://tzs.jinghuilouyu.cn

#define X_H
来源：http://tdt.jinqigfzy.top

#endif
来源：http://koa.redwolf501.top

[S31] C++：Hello World
来源：http://wda.fktsv.cn

#include <iostream>
来源：http://pdh.hammf.cn

int main() { std::cout << "Hello\n"; }
来源：http://znm.jinghuilouyu.cn

[S32] C++：字符串
来源：http://dfk.shzxlz.cn

std::string s = "hi";  s += "!";
来源：http://vxy.zhijiandao.cn

[S33] C++：vector 增删
来源：http://iou.jinqigfzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cds.shzxlz.cn

[S34] C++：遍历 vector
来源：http://oqq.snrcjt.cn

for (auto &x : v) { std::cout << x; }
来源：http://jmg.ydjk.org.cn

[S35] C++：map
来源：http://qdx.havefunace.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://klx.xinyue.icu

[S36] C++：unordered_map
来源：http://rza.yuxming.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dmd.yfazqb.com

[S37] C++：set
来源：http://zed.tianlin.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wzs.gogol.net.cn

[S38] C++：排序
来源：http://gem.yueranfly.top

std::sort(v.begin(), v.end());
来源：http://wfo.shzxlz.cn

[S39] C++：自定义比较器排序
来源：http://cru.yj202588.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hqu.fengsongda.top

[S40] C++：查找元素
来源：http://nwl.zhengqikj.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://scm.sysykeji.top

[S41] C++：类与构造函数
来源：http://fcb.xinyue.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kjs.yj20258.top

[S42] C++：继承与虚函数
来源：http://znw.uphjek.com

class B : public Base { public: void f() override {} };
来源：http://jmu.xuetiantiany.cn

[S43] C++：智能指针
来源：http://uvq.guannengcc.top

auto p = std::make_unique<int>(5);
来源：http://rda.quarkkingdee.top

[S44] C++：引用传参
来源：http://qzm.dashuyun.cn

void inc(int &x) { ++x; }
来源：http://wxy.pengpengdd.cyou

[S45] C++：lambda
来源：http://jmk.52xcode.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wqy.hysaishi.cn

[S46] C++：函数模板
来源：http://oel.hcnkem.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rgv.dashuyun.cn

[S47] C++：结构化绑定遍历
来源：http://ftb.bjfxy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ezx.zhijiandao.cn

[S48] C++：逐行读文件
来源：http://kmk.meibo888.top

std::ifstream in("a.txt");  std::string line;
来源：http://luj.hammf.cn

while (std::getline(in, line)) { }
来源：http://wzl.jinqigfzy.top

[S49] C++：写文件
来源：http://jzm.yj202588.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kzl.ybcxt.top

[S50] C++：格式化数字
来源：http://dfh.jlsjyb.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://niz.aizwys.cn

[S51] C++：显式类型转换
来源：http://lhp.bjfxy.top

static_cast<double>(a) / b
来源：http://rsp.jianghu66.top

[S52] C++：const 与 noexcept
来源：http://otn.tianlin.xyz

int size() const noexcept { return n_; }
来源：http://pfl.yfazqb.com

[S53] C++：移动语义
来源：http://awi.shuidangran.top

std::vector<int> w = std::move(v);
来源：http://sif.hammf.cn

[S54] C++：异常处理
来源：http://lfb.chenzaomai.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hge.xziqi.cn

[S55] C++：结构化绑定
来源：http://znu.jyoumei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://raq.cdnleiting.top

[S56] C++：optional
来源：http://ikq.cqqwz.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uvv.ydzc1.top

[S57] C++：编译期常量
来源：http://lof.ywan-chungtsiang.top

constexpr int N = 10;
来源：http://ltv.sweek.top

[S58] C++：命名空间
来源：http://thp.c1oappe.top

namespace ns { int f() { return 1; } }
来源：http://iuq.vqdsnc.cn

[S59] C++：静态断言
来源：http://qfs.daria6918.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://geb.redwolf501.top

[S60] C++：遍历并删除元素
来源：http://vqr.ydjk.org.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rwy.yfazqb.com

================================================================================
来源：http://mbp.jinqigufen.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pdf.gogol.net.cn

================================================================================
来源：http://cfq.c1oappe.top

[T01] Kotlin：Hello World
来源：http://yzw.xylfe.cn

println("Hello")
来源：http://mmx.ybcxt.top

[T02] Kotlin：变量
来源：http://vle.ywan-chungtsiang.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pae.chenlongwang.top

[T03] Kotlin：字符串模板
来源：http://sso.redwolf501.top

"值: $b"
来源：http://swn.hnxiangtu.top

[T04] Kotlin：空安全
来源：http://xcu.yj20258888.top

val n: String? = null;  n?.length
来源：http://dbg.9152youxi.cn

[T05] Kotlin：when 表达式
来源：http://zwi.sysykeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://oxc.sjlbkw.cn

[T06] Kotlin：集合映射
来源：http://szz.meibo888.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rqn.bjfxy.top

[T07] Kotlin：集合过滤
来源：http://api.cqqwz.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://sth.zycfv.cn

[T08] Kotlin：数据类
来源：http://dtb.daxiang520.top

data class User(val name: String, val age: Int)
来源：http://koa.316326.xyz

[T09] Kotlin：扩展函数
来源：http://lnk.hongshengwenyu.top

fun String.exclaim() = this + "!"
来源：http://jcj.xuanzx.com

[T10] Kotlin：默认参数
来源：http://vsv.cheryme.top

fun greet(name: String = "World") = "Hi $name"
来源：http://pyp.andypj.xyz

[T11] Kotlin：协程
来源：http://ajw.sxryk.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hok.xziqi.cn

[T12] Kotlin：解构声明
来源：http://ott.guannengcc.top

val (a, b) = Pair(1, 2)
来源：http://iwh.gaohongyu789.top

[T13] Kotlin：只读 Map
来源：http://wra.jianghu66.top

val m = mapOf("a" to 1)
来源：http://cko.xuetiantiany.cn

[T14] Kotlin：循环
来源：http://dqx.shuidangran.top

for (i in 1..10) println(i)
来源：http://vep.tanke756.top

[T15] Kotlin：接口
来源：http://irk.fzhhl.top

interface Shape { fun area(): Double }
来源：http://fjp.sysykeji.top

[T16] Swift：Hello World
来源：http://rhi.c1oappe.top

print("Hello")
来源：http://lhr.yuanzhike.top

[T17] Swift：变量与常量
来源：http://cac.zhaomingkeji.xyz

var a = 1;  let b = 2
来源：http://hmt.gotoacloud.top

[T18] Swift：字符串插值
来源：http://gec.chenjidiqi.icu

"值: \(b)"
来源：http://gwd.vehdjk.com

[T19] Swift：可选绑定
来源：http://vpz.mhx1999.top

if let n = opt { print(n) }
来源：http://uns.daria6918.cn

[T20] Swift：数组操作
来源：http://jef.gaohongyu789.top

var a = [1, 2, 3];  a.append(4)
来源：http://ogf.xinyue.icu

[T21] Swift：遍历
来源：http://atc.316326.xyz

for x in a { print(x) }
来源：http://tim.zhongyouzk.top

[T22] Swift：字典
来源：http://jvy.quarkkingdee.top

var d = ["a": 1];  d["b"] = 2
来源：http://pbt.yj20258888.top

[T23] Swift：函数
来源：http://xjd.jianghu66.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tnl.snrcjt.cn

[T24] Swift：闭包
来源：http://szu.redwolf501.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://fru.sjlbkw.cn

[T25] Swift：结构体
来源：http://pea.ybcxt.top

struct P { var x: Int }
来源：http://nxl.andypj.xyz

[T26] Swift：类与重写
来源：http://xly.jlsjyb.cn

class A: Base { override func f() {} }
来源：http://sle.jqgfzy.top

[T27] Swift：错误处理
来源：http://epu.jinyuanbaomall.cn

do { try f() } catch { print(error) }
来源：http://tod.chenzaomai.com

[T28] Swift：枚举
来源：http://smr.gotoacloud.top

enum Color { case red, green }
来源：http://bbv.jyoumei.cn

[T29] Swift：guard 提前返回
来源：http://kwt.yvedp.cn

guard let x = opt else { return }
来源：http://ahg.cqqwz.cn

[T30] Swift：协议
来源：http://jyw.jinyuanbaomall.cn

protocol Shape { func area() -> Double }
来源：http://ync.pengpengdd.cyou

[T31] Lua：Hello World
来源：http://oek.jinghuilouyu.cn

print("Hello")
来源：http://dpc.nanxinkj.top

[T32] Lua：局部变量
来源：http://zzm.yfazqb.com

local a = 1
来源：http://nah.zhengqikj.top

[T33] Lua：表（数组）
来源：http://oxc.ywan-chungtsiang.top

local t = {1, 2, 3};  t[4] = 4
来源：http://qlf.kuanghao11.cn

[T34] Lua：遍历表
来源：http://xms.jlsjyb.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://aop.aizwys.cn

[T35] Lua：字典表
来源：http://kpq.hesvh.cn

local d = { a = 1 };  d.b = 2
来源：http://ixq.hfpthk.cn

[T36] Lua：函数
来源：http://ckx.zhijiandao.cn

function add(a, b) return a + b end
来源：http://jxl.haohaochexian.top


<!-- 参考信息 -->