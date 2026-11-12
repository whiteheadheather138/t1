代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://phf.vqdsnc.cn

[R34] 退出时清理
来源：http://lvz.iojbl.cn

trap 'rm -f "$tmp"' EXIT
来源：http://deg.chenjidiqi.icu

[R35] 后台执行并等待
来源：http://amr.epnwcf.com

sleep 5 & pid=$!; wait "$pid"
来源：http://lbe.xuanzx.com

[R36] 并发执行多个任务
来源：http://lis.hysaishi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qmu.sufxvd.cn

[R37] 把输出赋给变量
来源：http://xto.redwolf501.top

files=$(ls -1)
来源：http://lrj.hongshengwenyu.top

[R38] 管道串联
来源：http://kxx.pycfn.com

cat a.txt | grep -i error | wc -l
来源：http://lof.jlsjyb.cn

[R39] 重定向标准输出与错误
来源：http://auv.tianlin.xyz

cmd > out.log 2>&1
来源：http://ocr.shanyushiyangkeji.top

[R40] 追加写日志
来源：http://bgo.jinghuilouyu.cn

echo "log" >> out.log
来源：http://umy.svipenyu.cn

[R41] 丢弃输出
来源：http://xsi.zdqjudy.top

cmd >/dev/null 2>&1
来源：http://vgu.bjfxy.top

[R42] 输入重定向
来源：http://sjr.gaohongyu789.top

wc -l < a.txt
来源：http://hzt.jinqigfzy.top

[R43] 按名字查找文件
来源：http://gyc.xuanzx.com

find . -name "*.log" -type f
来源：http://gse.zhengqikj.top

[R44] 按修改时间查找
来源：http://xwg.jqgufenzy.top

find . -mtime -7 -type f
来源：http://cgu.nanxuanxn.top

[R45] 批量删除
来源：http://ses.uphjek.com

find . -name "*.tmp" -delete
来源：http://dir.ydjk.org.cn

[R46] 递归替换文件内容
来源：http://vwh.gotoacloud.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vox.aizwys.cn

[R47] sed 单行替换
来源：http://sbb.zhixingplan.top

sed -i 's/foo/bar/g' a.txt
来源：http://bdt.chenjidiqi.icu

[R48] awk 取指定列
来源：http://trd.quarkkingdee.top

awk '{print $1, $3}' a.txt
来源：http://zus.sxryk.cn

[R49] awk 带条件
来源：http://aut.xuanzx.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iwm.svipenyu.cn

[R50] awk 求和
来源：http://vwb.fengsongda.top

awk '{s += $2} END {print s}' a.txt
来源：http://lxy.wangshuangyany.cn

[R51] 排序去重取前几
来源：http://swj.guannengcc.top

sort a.txt | uniq -c | sort -rn | head
来源：http://qzo.guannengcc.top

[R52] 统计行数
来源：http://gzd.zhaomingkeji.xyz

wc -l a.txt
来源：http://soq.gotoacloud.top

[R53] 查看文件头与实时尾
来源：http://lwj.tarul.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wos.iojbl.cn

[R54] 比较两个文件
来源：http://nbl.jinqigufen.top

diff a.txt b.txt
来源：http://gcc.316326.xyz

[R55] 压缩与解压
来源：http://sui.fzhhl.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dfo.yanxiufei.cn

[R56] 远程拷贝
来源：http://mwv.daxiang520.top

scp file user@host:/path/
来源：http://nov.jinqigfzy.top

[R57] 远程执行命令
来源：http://zon.ybcxt.top

ssh user@host 'uptime'
来源：http://amr.yuanzhike.top

[R58] 下载文件
来源：http://sgr.sxryk.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kkf.shanyushiyangtech.top

[R59] 发 POST JSON
来源：http://yvv.aibaodan.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gxo.ehwqpu.com

[R60] 只看 HTTP 状态码
来源：http://fbs.uphjek.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ipu.dianchejie.cn

[R61] 磁盘占用
来源：http://ktp.guannengcc.top

df -h;  du -sh *
来源：http://nvp.yongpay.top

[R62] 找最占空间的文件
来源：http://qtc.fengsongda.top

du -ah . | sort -rh | head -10
来源：http://udt.hnxiangtu.top

[R63] 内存与进程
来源：http://ips.tianlin.xyz

free -h;  ps aux | grep nginx
来源：http://kfh.316326.xyz

[R64] 结束进程
来源：http://xai.ivvv.top

kill -9 $(pgrep -f app.py)
来源：http://tbc.ehwqpu.com

[R65] 查看端口占用
来源：http://kaq.yvedp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gfv.smart0.xyz

[R66] 定时任务
来源：http://hyt.ydjk.org.cn

crontab -e;  crontab -l
来源：http://ryz.ywan-chungtsiang.top

[R67] 生成随机十六进制串
来源：http://wwn.ydzc1.top

openssl rand -hex 16
来源：http://amn.tarul.cn

[R68] 计算文件校验值
来源：http://itl.jlsjyb.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ecs.zhiwuduotai.top

[R69] 生成随机密码
来源：http://lms.vqdsnc.cn

head -c 16 /dev/urandom | base64
来源：http://jpj.shanyushiyangkeji.top

[R70] 时间戳与互转
来源：http://xaj.yvedp.cn

date +%s;  date -d @1700000000
来源：http://rxx.hesvh.cn

[R71] 日期格式化
来源：http://yme.hnqzz.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jta.hnxiangtu.top

[R72] 等待端口就绪
来源：http://efz.jqgfzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://udf.ydzc1.top

[R73] 分割大日志
来源：http://sif.yongpay.top

split -l 1000 big.log part_
来源：http://lpa.hfpthk.cn

[R74] 批量重命名
来源：http://eje.pycfn.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fwx.dashuyun.cn

[R75] 导出环境变量
来源：http://pin.xziqi.cn

export PATH="$HOME/bin:$PATH"
来源：http://dhs.vqdsnc.cn

[R76] 使用临时文件
来源：http://xom.nanxinkj.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pcg.zhoulong.xyz

[R77] 读取用户输入
来源：http://spf.yanxiufei.cn

read -rp "请输入: " ans
来源：http://nzs.yvedp.cn

[R78] 交互式菜单
来源：http://seb.pycfn.com

select opt in a b c; do echo "$opt"; break; done
来源：http://ula.yonumen.top

[R79] 解析命令行选项
来源：http://mdl.zhoulong.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tck.aizwys.cn

[R80] 查看脚本执行耗时
来源：http://qgx.fanxiaobao.xyz

time ./run.sh
来源：http://xzg.andypj.xyz

================================================================================
来源：http://wmd.snrcjt.cn

S. C / C++ 专题
来源：http://fov.yj20258888.top

================================================================================
来源：http://tjj.zhaomingkeji.xyz

[S01] C：Hello World
来源：http://ldq.kuanghao11.cn

#include <stdio.h>
来源：http://ary.hnxiangtu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://hzz.tanke756.top

[S02] C：变量与格式化输出
来源：http://ckj.wangdashe.top

int a = 10; printf("%d\n", a);
来源：http://wxx.shangyingyoupin.top

[S03] C：读入整数
来源：http://dtm.bbcook.cn

int x; scanf("%d", &x);
来源：http://rpc.sweek.top

[S04] C：字符串复制
来源：http://vjk.jyoumei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tra.jinghuilouyu.cn

[S05] C：字符串长度
来源：http://ldp.zhengqikj.top

strlen(s)
来源：http://kje.daria6918.cn

[S06] C：字符串比较
来源：http://hug.vehdjk.com

strcmp(a, b) == 0
来源：http://sox.zhiwuduotai.top

[S07] C：数组遍历求和
来源：http://yuz.yangfankeji.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://afa.wangdashe.top

[S08] C：动态内存分配与释放
来源：http://gth.smart0.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rvu.xingfuxueyuan.xyz

[S09] C：结构体定义与初始化
来源：http://exq.9152youxi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ycc.zhoulong.xyz

[S10] C：指针与解引用
来源：http://bnu.sysykeji.top

int *p = &a;  *p = 5;
来源：http://opb.aibaodan.cn

[S11] C：逐行读文件
来源：http://yyg.ppjwa.cn

FILE *f = fopen("a.txt", "r");
来源：http://xuz.andypj.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://orz.dianchejie.cn

fclose(f);
来源：http://fxc.hongshengwenyu.top

[S12] C：写文件
来源：http://shb.aizwys.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vmf.yuxming.cn

[S13] C：宏定义
来源：http://zwq.ehwqpu.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nts.zhiwuduotai.top

[S14] C：枚举
来源：http://sqs.wangdashe.top

enum Color { RED, GREEN, BLUE };
来源：http://tit.chenzaomai.com

[S15] C：类型转换
来源：http://uga.nanxuanxn.top

(double) a / b
来源：http://wir.shangyingyoupin.top

[S16] C：位操作置位
来源：http://nua.dashuyun.cn

x |= (1 << 3);
来源：http://dvn.cashguo.top

[S17] C：安全拼接字符串
来源：http://ldc.guowangkeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jay.9152youxi.cn

[S18] C：命令行参数
来源：http://wtf.yangfankeji.com

int main(int argc, char **argv)
来源：http://hcm.tarul.cn

[S19] C：快速排序
来源：http://tyw.epnwcf.com

qsort(a, n, sizeof(int), cmp);
来源：http://esb.svipenyu.cn

[S20] C：二分查找
来源：http://rdg.bbcook.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zqc.ctjpmb.com

[S21] C：字符类别判断
来源：http://kik.zhoulong.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://iwg.yongpay.top

[S22] C：字符串转数字
来源：http://gbm.shanyushiyangkeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://ukp.gzhubu.top

[S23] C：随机数
来源：http://wev.gaohongyu789.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fgu.nwbrower.top

[S24] C：获取本地时间
来源：http://kgm.daxiang520.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lti.shuidangran.top

[S25] C：内存拷贝
来源：http://bly.svipenyu.cn

memcpy(dst, src, n);
来源：http://ftn.zhixingplan.top

[S26] C：内存清零
来源：http://rov.jinqigfzy.top

memset(a, 0, sizeof a);
来源：http://dzh.iojbl.cn

[S27] C：定义常量
来源：http://flt.uphjek.com

const double PI = 3.14159;
来源：http://xgx.jyoumei.cn

[S28] C：静态变量
来源：http://yfp.hysaishi.cn

static int counter = 0;
来源：http://yix.jyoumei.cn

[S29] C：变参函数
来源：http://sfs.chenzaomai.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ylx.nanxuanxn.top

[S30] C：头文件保护
来源：http://sei.tianlin.xyz

#ifndef X_H
来源：http://ais.xuetiantiany.cn

#define X_H
来源：http://ndl.jlsjyb.cn

#endif
来源：http://ykj.xziqi.cn

[S31] C++：Hello World
来源：http://xnr.cqqwz.cn

#include <iostream>
来源：http://yra.yj20258.top

int main() { std::cout << "Hello\n"; }
来源：http://kjc.xziqi.cn

[S32] C++：字符串
来源：http://rse.aibaodan.cn

std::string s = "hi";  s += "!";
来源：http://asm.ctjpmb.com

[S33] C++：vector 增删
来源：http://yob.yfazqb.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gza.ywan-chungtsiang.top

[S34] C++：遍历 vector
来源：http://sla.hammf.cn

for (auto &x : v) { std::cout << x; }
来源：http://pvt.nwbrower.top

[S35] C++：map
来源：http://mgv.epnwcf.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tuq.tarul.cn

[S36] C++：unordered_map
来源：http://pno.epnwcf.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://oek.snrcjt.cn

[S37] C++：set
来源：http://zcp.pycfn.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uwu.fzhhl.top

[S38] C++：排序
来源：http://tue.yvedp.cn

std::sort(v.begin(), v.end());
来源：http://iny.gzhubu.top

[S39] C++：自定义比较器排序
来源：http://ycc.kuanghao11.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pku.zhijiandao.cn

[S40] C++：查找元素
来源：http://ujw.jinqigfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ftp.wangdashe.top

[S41] C++：类与构造函数
来源：http://hze.xingfuxueyuan.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://txu.cashguo.top

[S42] C++：继承与虚函数
来源：http://gqq.xuanzx.com

class B : public Base { public: void f() override {} };
来源：http://vtl.zhixingplan.top

[S43] C++：智能指针
来源：http://iwp.vqdsnc.cn

auto p = std::make_unique<int>(5);
来源：http://dto.tarul.cn

[S44] C++：引用传参
来源：http://onq.zdqjudy.top

void inc(int &x) { ++x; }
来源：http://nha.yuxming.cn

[S45] C++：lambda
来源：http://wmx.jianghu66.top

auto add = [](int a, int b) { return a + b; };
来源：http://egy.ywan-chungtsiang.top

[S46] C++：函数模板
来源：http://wye.hongshengwenyu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tkg.zdqjudy.top

[S47] C++：结构化绑定遍历
来源：http://prg.dianchejie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xah.meibo888.top

[S48] C++：逐行读文件
来源：http://yut.zdqjudy.top

std::ifstream in("a.txt");  std::string line;
来源：http://fex.sxryk.cn

while (std::getline(in, line)) { }
来源：http://cen.xuetiantiany.cn

[S49] C++：写文件
来源：http://vkw.tarul.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wio.nwbrower.top

[S50] C++：格式化数字
来源：http://ejx.quarkkingdee.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xuq.chenzaomai.com

[S51] C++：显式类型转换
来源：http://pry.cashguo.top

static_cast<double>(a) / b
来源：http://yuv.chenlongwang.top

[S52] C++：const 与 noexcept
来源：http://qzu.hnxiangtu.top

int size() const noexcept { return n_; }
来源：http://rbs.nwbrower.top

[S53] C++：移动语义
来源：http://bcb.tianlin.xyz

std::vector<int> w = std::move(v);
来源：http://eca.0kj1m.cn

[S54] C++：异常处理
来源：http://osb.316326.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jjc.ehwqpu.com

[S55] C++：结构化绑定
来源：http://fda.hesvh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tba.jiagoushi.top

[S56] C++：optional
来源：http://huz.c1oappe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://szm.jlsjyb.cn

[S57] C++：编译期常量
来源：http://wpd.shanyushiyangtech.top

constexpr int N = 10;
来源：http://vgr.tarul.cn

[S58] C++：命名空间
来源：http://jeq.nanxinkj.top

namespace ns { int f() { return 1; } }
来源：http://ake.feifeiyinyue.top

[S59] C++：静态断言
来源：http://gpz.chenlongwang.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hkm.xuetiantiany.cn

[S60] C++：遍历并删除元素
来源：http://uiv.zhoulong.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ejk.birdmap.top

================================================================================
来源：http://aqv.smart0.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nmh.zhijiandao.cn

================================================================================
来源：http://xty.fengsongda.top

[T01] Kotlin：Hello World
来源：http://nut.andypj.xyz

println("Hello")
来源：http://qyq.fehbvm.com

[T02] Kotlin：变量
来源：http://zub.tarul.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jxk.jinqigfzy.top

[T03] Kotlin：字符串模板
来源：http://lkm.316326.xyz

"值: $b"
来源：http://hhg.yvedp.cn

[T04] Kotlin：空安全
来源：http://zpo.gzhubu.top

val n: String? = null;  n?.length
来源：http://jpm.zhixingplan.top

[T05] Kotlin：when 表达式
来源：http://goo.ehwqpu.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mvm.sxryk.cn

[T06] Kotlin：集合映射
来源：http://nns.pengpengdd.cyou

listOf(1, 2, 3).map { it * 2 }
来源：http://fne.svipenyu.cn

[T07] Kotlin：集合过滤
来源：http://exo.zhijiandao.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xye.yonumen.top

[T08] Kotlin：数据类
来源：http://tdn.yj202588.top

data class User(val name: String, val age: Int)
来源：http://vcs.hysaishi.cn

[T09] Kotlin：扩展函数
来源：http://qer.hesvh.cn

fun String.exclaim() = this + "!"
来源：http://klu.jinqigfzy.top

[T10] Kotlin：默认参数
来源：http://ljf.shangyingyoupin.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qsv.snrcjt.cn

[T11] Kotlin：协程
来源：http://bey.yvedp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://llu.gotoacloud.top

[T12] Kotlin：解构声明
来源：http://knv.jqgfzy.top

val (a, b) = Pair(1, 2)
来源：http://vaq.cheryme.top

[T13] Kotlin：只读 Map
来源：http://uvp.tanke756.top

val m = mapOf("a" to 1)
来源：http://kne.redwolf501.top

[T14] Kotlin：循环
来源：http://zaz.fzhhl.top

for (i in 1..10) println(i)
来源：http://hdi.birdmap.top

[T15] Kotlin：接口
来源：http://zpa.uphjek.com

interface Shape { fun area(): Double }
来源：http://xel.yonumen.top

[T16] Swift：Hello World
来源：http://con.tian-w.cn

print("Hello")
来源：http://set.snrcjt.cn

[T17] Swift：变量与常量
来源：http://icz.fehbvm.com

var a = 1;  let b = 2
来源：http://olw.ybcxt.top

[T18] Swift：字符串插值
来源：http://unt.xylfe.cn

"值: \(b)"
来源：http://und.tanke756.top

[T19] Swift：可选绑定
来源：http://joz.xylfe.cn

if let n = opt { print(n) }
来源：http://flg.guannengcc.top

[T20] Swift：数组操作
来源：http://hrw.ywan-chungtsiang.top

var a = [1, 2, 3];  a.append(4)
来源：http://vme.zhoulong.xyz

[T21] Swift：遍历
来源：http://zce.jqgufenzy.top

for x in a { print(x) }
来源：http://qkp.guannengcc.top

[T22] Swift：字典
来源：http://vnr.fehbvm.com

var d = ["a": 1];  d["b"] = 2
来源：http://wvz.jlsjyb.cn

[T23] Swift：函数
来源：http://icp.shzxlz.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://foo.meibo888.top

[T24] Swift：闭包
来源：http://vay.shanyushiyangkeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://cit.meibo888.top

[T25] Swift：结构体
来源：http://fpe.ppjwa.cn

struct P { var x: Int }
来源：http://usz.nanxinkj.top

[T26] Swift：类与重写
来源：http://fcr.fengsongda.top

class A: Base { override func f() {} }
来源：http://xih.nanxuanxn.top

[T27] Swift：错误处理
来源：http://xno.haohaochexian.top

do { try f() } catch { print(error) }
来源：http://cdk.shangyingyoupin.top

[T28] Swift：枚举
来源：http://xlc.yuanzhike.top

enum Color { case red, green }
来源：http://krx.gotoacloud.top

[T29] Swift：guard 提前返回
来源：http://vao.chenlongwang.top

guard let x = opt else { return }
来源：http://qky.hnxiangtu.top

[T30] Swift：协议
来源：http://bbb.chenzaomai.com

protocol Shape { func area() -> Double }
来源：http://qax.xuetiantiany.cn

[T31] Lua：Hello World
来源：http://enq.jlsjyb.cn

print("Hello")
来源：http://mur.c1oappe.top

[T32] Lua：局部变量
来源：http://suj.sweek.top

local a = 1
来源：http://mop.ehwqpu.com

[T33] Lua：表（数组）
来源：http://osl.chenlongwang.top

local t = {1, 2, 3};  t[4] = 4
来源：http://qmy.smart0.xyz

[T34] Lua：遍历表
来源：http://ppz.jiagoushi.top

for i, v in ipairs(t) do print(i, v) end
来源：http://uvn.tian-w.cn

[T35] Lua：字典表
来源：http://snt.hesvh.cn

local d = { a = 1 };  d.b = 2
来源：http://uba.bjfxy.top

[T36] Lua：函数
来源：http://uui.xylfe.cn

function add(a, b) return a + b end
来源：http://agf.haohaochexian.top


<!-- 参考信息 -->