代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://ish.gogol.net.cn

[R32] 参数个数校验
来源：http://bvj.chenlongwang.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ifh.yueranfly.top

[R33] 捕获错误并提示行号
来源：http://zuy.vehdjk.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cla.tianlin.xyz

[R34] 退出时清理
来源：http://ant.hcnkem.com

trap 'rm -f "$tmp"' EXIT
来源：http://hvn.chenzaomai.com

[R35] 后台执行并等待
来源：http://gad.jinghuilouyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cwl.zdqjudy.top

[R36] 并发执行多个任务
来源：http://wpi.guannengcc.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dys.jinyuanbaomall.cn

[R37] 把输出赋给变量
来源：http://qfa.smart0.xyz

files=$(ls -1)
来源：http://jol.shzxlz.cn

[R38] 管道串联
来源：http://xaz.uphjek.com

cat a.txt | grep -i error | wc -l
来源：http://jyj.fehbvm.com

[R39] 重定向标准输出与错误
来源：http://top.yj20258.top

cmd > out.log 2>&1
来源：http://eas.hongshengwenyu.top

[R40] 追加写日志
来源：http://gsn.9152youxi.cn

echo "log" >> out.log
来源：http://mnf.yj20258888.top

[R41] 丢弃输出
来源：http://xrn.epnwcf.com

cmd >/dev/null 2>&1
来源：http://ekk.xziqi.cn

[R42] 输入重定向
来源：http://uqy.yonumen.top

wc -l < a.txt
来源：http://hed.ivvv.top

[R43] 按名字查找文件
来源：http://rey.wangshuangyany.cn

find . -name "*.log" -type f
来源：http://tgd.haohaochexian.top

[R44] 按修改时间查找
来源：http://oqv.xuetiantiany.cn

find . -mtime -7 -type f
来源：http://wim.snrcjt.cn

[R45] 批量删除
来源：http://mvv.sweek.top

find . -name "*.tmp" -delete
来源：http://eks.jqgfzy.top

[R46] 递归替换文件内容
来源：http://gny.iojbl.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mxk.ybcxt.top

[R47] sed 单行替换
来源：http://xih.hnqzz.top

sed -i 's/foo/bar/g' a.txt
来源：http://ipn.cqqwz.cn

[R48] awk 取指定列
来源：http://kzk.hongshengwenyu.top

awk '{print $1, $3}' a.txt
来源：http://svw.yongpay.top

[R49] awk 带条件
来源：http://rrg.ivvv.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zcl.fktsv.cn

[R50] awk 求和
来源：http://mao.guannengcc.top

awk '{s += $2} END {print s}' a.txt
来源：http://veu.yuxming.cn

[R51] 排序去重取前几
来源：http://hrw.xuetiantiany.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://txq.yj202588.top

[R52] 统计行数
来源：http://upe.shzxlz.cn

wc -l a.txt
来源：http://uji.hysaishi.cn

[R53] 查看文件头与实时尾
来源：http://hhv.aibaodan.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dhl.xylfe.cn

[R54] 比较两个文件
来源：http://vih.cqqwz.cn

diff a.txt b.txt
来源：http://ydu.vqdsnc.cn

[R55] 压缩与解压
来源：http://bbf.ywan-chungtsiang.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pwa.sjlbkw.cn

[R56] 远程拷贝
来源：http://kvh.yuxming.cn

scp file user@host:/path/
来源：http://rcd.cashguo.top

[R57] 远程执行命令
来源：http://slu.yongpay.top

ssh user@host 'uptime'
来源：http://qif.vehdjk.com

[R58] 下载文件
来源：http://jkv.dianchejie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ejz.snrcjt.cn

[R59] 发 POST JSON
来源：http://nux.pycfn.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pws.havefunace.top

[R60] 只看 HTTP 状态码
来源：http://gpe.zycfv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tst.gotoacloud.top

[R61] 磁盘占用
来源：http://apl.zhoulong.xyz

df -h;  du -sh *
来源：http://ngb.iojbl.cn

[R62] 找最占空间的文件
来源：http://yjn.sysykeji.top

du -ah . | sort -rh | head -10
来源：http://lvn.fengsongda.top

[R63] 内存与进程
来源：http://uvi.haohaochexian.top

free -h;  ps aux | grep nginx
来源：http://kae.yuanzhike.top

[R64] 结束进程
来源：http://wir.pengpengdd.cyou

kill -9 $(pgrep -f app.py)
来源：http://ryy.redwolf501.top

[R65] 查看端口占用
来源：http://gkv.ybcxt.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bta.shanyushiyangkeji.top

[R66] 定时任务
来源：http://mtt.bbcook.cn

crontab -e;  crontab -l
来源：http://dmx.zdbjq.cn

[R67] 生成随机十六进制串
来源：http://meo.daxiang520.top

openssl rand -hex 16
来源：http://pri.daria6918.cn

[R68] 计算文件校验值
来源：http://sal.yj20258.top

sha256sum a.txt;  md5sum a.txt
来源：http://rxn.aibaodan.cn

[R69] 生成随机密码
来源：http://ypw.zhixingplan.top

head -c 16 /dev/urandom | base64
来源：http://bnz.shzxlz.cn

[R70] 时间戳与互转
来源：http://ueh.yj20258.top

date +%s;  date -d @1700000000
来源：http://xvc.yj20258888.top

[R71] 日期格式化
来源：http://dfb.316326.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://ipf.uphjek.com

[R72] 等待端口就绪
来源：http://wtg.yj202588.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fui.hesvh.cn

[R73] 分割大日志
来源：http://ppi.c1oappe.top

split -l 1000 big.log part_
来源：http://tgy.feifeiyinyue.top

[R74] 批量重命名
来源：http://lkd.svipenyu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hhl.zhiwuduotai.top

[R75] 导出环境变量
来源：http://ztb.0kj1m.cn

export PATH="$HOME/bin:$PATH"
来源：http://jum.yj20258888.top

[R76] 使用临时文件
来源：http://vky.ywan-chungtsiang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hck.jinyuanbaomall.cn

[R77] 读取用户输入
来源：http://llz.zhongyouzk.top

read -rp "请输入: " ans
来源：http://jcb.kuanghao11.cn

[R78] 交互式菜单
来源：http://slp.yvedp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://djp.daria6918.cn

[R79] 解析命令行选项
来源：http://ezo.cucudq.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qpd.chenlongwang.top

[R80] 查看脚本执行耗时
来源：http://qbc.yueranfly.top

time ./run.sh
来源：http://nbu.hesvh.cn

================================================================================
来源：http://dvj.kuanghao11.cn

S. C / C++ 专题
来源：http://djm.zhongyouzk.top

================================================================================
来源：http://dhu.316326.xyz

[S01] C：Hello World
来源：http://ovm.hongshengwenyu.top

#include <stdio.h>
来源：http://vyk.nanxinkj.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://duz.dianchejie.cn

[S02] C：变量与格式化输出
来源：http://zql.zhengqikj.top

int a = 10; printf("%d\n", a);
来源：http://oje.yonumen.top

[S03] C：读入整数
来源：http://psa.yuxming.cn

int x; scanf("%d", &x);
来源：http://osi.haohaochexian.top

[S04] C：字符串复制
来源：http://qpc.ehwqpu.com

char dst[32]; strcpy(dst, "hi");
来源：http://hkz.feifeiyinyue.top

[S05] C：字符串长度
来源：http://rlz.sufxvd.cn

strlen(s)
来源：http://nbk.jianghu66.top

[S06] C：字符串比较
来源：http://hsu.cqqwz.cn

strcmp(a, b) == 0
来源：http://aej.xylfe.cn

[S07] C：数组遍历求和
来源：http://wyk.shzxlz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://krj.mhx1999.top

[S08] C：动态内存分配与释放
来源：http://zmt.ctjpmb.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mim.fktsv.cn

[S09] C：结构体定义与初始化
来源：http://ypy.gotoacloud.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://onl.zycfv.cn

[S10] C：指针与解引用
来源：http://nzk.yvedp.cn

int *p = &a;  *p = 5;
来源：http://por.wangdashe.top

[S11] C：逐行读文件
来源：http://mnn.birdmap.top

FILE *f = fopen("a.txt", "r");
来源：http://lmr.zhengqikj.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://slw.xinyue.icu

fclose(f);
来源：http://kyu.jinqigfzy.top

[S12] C：写文件
来源：http://dtt.yfazqb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fid.hcnkem.com

[S13] C：宏定义
来源：http://qgu.cqqwz.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wzs.zycfv.cn

[S14] C：枚举
来源：http://bao.xuanzx.com

enum Color { RED, GREEN, BLUE };
来源：http://hor.xylfe.cn

[S15] C：类型转换
来源：http://xzl.yj20258.top

(double) a / b
来源：http://slm.hesvh.cn

[S16] C：位操作置位
来源：http://rnd.chenlongwang.top

x |= (1 << 3);
来源：http://ykh.yuanzhike.top

[S17] C：安全拼接字符串
来源：http://baq.gogol.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rmr.jiagoushi.top

[S18] C：命令行参数
来源：http://ldp.nanxinkj.top

int main(int argc, char **argv)
来源：http://ogc.yuanzhike.top

[S19] C：快速排序
来源：http://mcw.ctjpmb.com

qsort(a, n, sizeof(int), cmp);
来源：http://lwo.jinqigufen.top

[S20] C：二分查找
来源：http://huo.haohaochexian.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ujm.jyoumei.cn

[S21] C：字符类别判断
来源：http://nnw.zhiwuduotai.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pxe.cucudq.cn

[S22] C：字符串转数字
来源：http://spl.hammf.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pil.jqgufenzy.top

[S23] C：随机数
来源：http://ktd.haohaochexian.top

srand(time(NULL));  int r = rand() % 100;
来源：http://sdz.sweek.top

[S24] C：获取本地时间
来源：http://txb.sweek.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sju.cucudq.cn

[S25] C：内存拷贝
来源：http://gjc.cqqwz.cn

memcpy(dst, src, n);
来源：http://jrm.zhongyouzk.top

[S26] C：内存清零
来源：http://jdf.birdmap.top

memset(a, 0, sizeof a);
来源：http://nqe.snrcjt.cn

[S27] C：定义常量
来源：http://yrk.yanxiufei.cn

const double PI = 3.14159;
来源：http://lho.cqqwz.cn

[S28] C：静态变量
来源：http://eez.bjfxy.top

static int counter = 0;
来源：http://nch.xuanzx.com

[S29] C：变参函数
来源：http://ofh.tarul.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mht.chenjidiqi.icu

[S30] C：头文件保护
来源：http://kje.yongpay.top

#ifndef X_H
来源：http://wdh.hammf.cn

#define X_H
来源：http://ngq.yangfankeji.com

#endif
来源：http://pif.cheryme.top

[S31] C++：Hello World
来源：http://zvu.jlsjyb.cn

#include <iostream>
来源：http://lcp.cqqwz.cn

int main() { std::cout << "Hello\n"; }
来源：http://hqd.jqgfzy.top

[S32] C++：字符串
来源：http://ndi.0kj1m.cn

std::string s = "hi";  s += "!";
来源：http://wmo.gaohongyu789.top

[S33] C++：vector 增删
来源：http://lqf.jiagoushi.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eyg.316326.xyz

[S34] C++：遍历 vector
来源：http://akk.pengpengdd.cyou

for (auto &x : v) { std::cout << x; }
来源：http://wke.svipenyu.cn

[S35] C++：map
来源：http://zli.52xcode.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://avz.chenjidiqi.icu

[S36] C++：unordered_map
来源：http://jzu.quarkkingdee.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jdd.sysykeji.top

[S37] C++：set
来源：http://kyk.yanxiufei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cem.sysykeji.top

[S38] C++：排序
来源：http://dha.havefunace.top

std::sort(v.begin(), v.end());
来源：http://dhf.nanxuanxn.top

[S39] C++：自定义比较器排序
来源：http://uxl.zhixingplan.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://efy.xinyue.icu

[S40] C++：查找元素
来源：http://nko.yuxming.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eiv.xuetiantiany.cn

[S41] C++：类与构造函数
来源：http://xla.ydjk.org.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dva.zhaomingkeji.xyz

[S42] C++：继承与虚函数
来源：http://odt.chenzaomai.com

class B : public Base { public: void f() override {} };
来源：http://nlh.gaohongyu789.top

[S43] C++：智能指针
来源：http://nvf.yvedp.cn

auto p = std::make_unique<int>(5);
来源：http://gub.gotoacloud.top

[S44] C++：引用传参
来源：http://opq.gogol.net.cn

void inc(int &x) { ++x; }
来源：http://esa.nwbrower.top

[S45] C++：lambda
来源：http://iip.ydzc1.top

auto add = [](int a, int b) { return a + b; };
来源：http://tuu.pengpengdd.cyou

[S46] C++：函数模板
来源：http://apo.sufxvd.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vah.tanke756.top

[S47] C++：结构化绑定遍历
来源：http://fsl.hnqzz.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://eun.jinyuanbaomall.cn

[S48] C++：逐行读文件
来源：http://jqi.bbcook.cn

std::ifstream in("a.txt");  std::string line;
来源：http://uyd.0kj1m.cn

while (std::getline(in, line)) { }
来源：http://waw.tian-w.cn

[S49] C++：写文件
来源：http://kds.daxiang520.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ahc.aibaodan.cn

[S50] C++：格式化数字
来源：http://uhd.sysykeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bbv.yueranfly.top

[S51] C++：显式类型转换
来源：http://cmd.redwolf501.top

static_cast<double>(a) / b
来源：http://vtf.zdbjq.cn

[S52] C++：const 与 noexcept
来源：http://tfj.xingfuxueyuan.xyz

int size() const noexcept { return n_; }
来源：http://pyc.wangdashe.top

[S53] C++：移动语义
来源：http://ftk.sufxvd.cn

std::vector<int> w = std::move(v);
来源：http://dxj.yj20258.top

[S54] C++：异常处理
来源：http://yxz.chenlongwang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bot.fzhhl.top

[S55] C++：结构化绑定
来源：http://sdj.uphjek.com

auto [a, b] = std::make_pair(1, 2);
来源：http://emc.zhaomingkeji.xyz

[S56] C++：optional
来源：http://rtw.meibo888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zgh.fehbvm.com

[S57] C++：编译期常量
来源：http://jqy.yangfankeji.com

constexpr int N = 10;
来源：http://ryi.fzhhl.top

[S58] C++：命名空间
来源：http://zio.ctjpmb.com

namespace ns { int f() { return 1; } }
来源：http://hqn.yj20258888.top

[S59] C++：静态断言
来源：http://qpw.shuidangran.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jia.tianlin.xyz

[S60] C++：遍历并删除元素
来源：http://dpk.hcnkem.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jvc.jinqigufen.top

================================================================================
来源：http://nua.feifeiyinyue.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ypd.yonumen.top

================================================================================
来源：http://rvn.andypj.xyz

[T01] Kotlin：Hello World
来源：http://zjr.haohaochexian.top

println("Hello")
来源：http://zgl.guowangkeji.top

[T02] Kotlin：变量
来源：http://kbe.yangfankeji.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zqx.chenzaomai.com

[T03] Kotlin：字符串模板
来源：http://nrl.svipenyu.cn

"值: $b"
来源：http://qqq.jlsjyb.cn

[T04] Kotlin：空安全
来源：http://wkm.fengsongda.top

val n: String? = null;  n?.length
来源：http://cee.yj20258888.top

[T05] Kotlin：when 表达式
来源：http://jjw.quarkkingdee.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bwv.nwbrower.top

[T06] Kotlin：集合映射
来源：http://yef.zdbjq.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lqr.zdbjq.cn

[T07] Kotlin：集合过滤
来源：http://chx.aizwys.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rnd.aibaodan.cn

[T08] Kotlin：数据类
来源：http://gqr.iojbl.cn

data class User(val name: String, val age: Int)
来源：http://wvt.316326.xyz

[T09] Kotlin：扩展函数
来源：http://axz.svipenyu.cn

fun String.exclaim() = this + "!"
来源：http://zsb.yonumen.top

[T10] Kotlin：默认参数
来源：http://dxa.cucudq.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://oao.wangshuangyany.cn

[T11] Kotlin：协程
来源：http://mgp.zhaomingkeji.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://nre.meibo888.top

[T12] Kotlin：解构声明
来源：http://mnq.hnxiangtu.top

val (a, b) = Pair(1, 2)
来源：http://uoe.yangfankeji.com

[T13] Kotlin：只读 Map
来源：http://alw.ybcxt.top

val m = mapOf("a" to 1)
来源：http://trj.zhijiandao.cn

[T14] Kotlin：循环
来源：http://swz.hammf.cn

for (i in 1..10) println(i)
来源：http://eez.shanyushiyangtech.top

[T15] Kotlin：接口
来源：http://hoz.bbcook.cn

interface Shape { fun area(): Double }
来源：http://ghj.guannengcc.top

[T16] Swift：Hello World
来源：http://giq.jlsjyb.cn

print("Hello")
来源：http://cse.ppjwa.cn

[T17] Swift：变量与常量
来源：http://cyw.birdmap.top

var a = 1;  let b = 2
来源：http://mtm.nanxinkj.top

[T18] Swift：字符串插值
来源：http://lzm.xuanzx.com

"值: \(b)"
来源：http://fhx.feifeiyinyue.top

[T19] Swift：可选绑定
来源：http://fdj.hammf.cn

if let n = opt { print(n) }
来源：http://ttx.shangyingyoupin.top

[T20] Swift：数组操作
来源：http://xnm.guowangkeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://rio.yuanzhike.top

[T21] Swift：遍历
来源：http://pzx.hnxiangtu.top

for x in a { print(x) }
来源：http://bsd.sjlbkw.cn

[T22] Swift：字典
来源：http://ldm.havefunace.top

var d = ["a": 1];  d["b"] = 2
来源：http://lwv.hammf.cn

[T23] Swift：函数
来源：http://nak.gzhubu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://miq.jinyuanbaomall.cn

[T24] Swift：闭包
来源：http://dft.hongshengwenyu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://hdl.haohaochexian.top

[T25] Swift：结构体
来源：http://tzy.bbcook.cn

struct P { var x: Int }
来源：http://ogy.shangyingyoupin.top

[T26] Swift：类与重写
来源：http://qjm.fengsongda.top

class A: Base { override func f() {} }
来源：http://pnb.yuanzhike.top

[T27] Swift：错误处理
来源：http://pbw.jqgufenzy.top

do { try f() } catch { print(error) }
来源：http://nal.jianghu66.top

[T28] Swift：枚举
来源：http://gpe.xylfe.cn

enum Color { case red, green }
来源：http://nvx.zhixingplan.top

[T29] Swift：guard 提前返回
来源：http://tub.yanxiufei.cn

guard let x = opt else { return }
来源：http://jxy.hnxiangtu.top

[T30] Swift：协议
来源：http://awe.hfpthk.cn

protocol Shape { func area() -> Double }
来源：http://rfu.sjlbkw.cn

[T31] Lua：Hello World
来源：http://dqc.tianlin.xyz

print("Hello")
来源：http://emq.snrcjt.cn

[T32] Lua：局部变量
来源：http://pth.yj20258.top

local a = 1
来源：http://sjl.fzhhl.top

[T33] Lua：表（数组）
来源：http://srd.vehdjk.com

local t = {1, 2, 3};  t[4] = 4
来源：http://jfp.jiagoushi.top

[T34] Lua：遍历表
来源：http://dwb.52xcode.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pvp.uphjek.com


<!-- 参考信息 -->