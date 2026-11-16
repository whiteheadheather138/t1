代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dme.epnwcf.com

[R30] 函数返回状态码
来源：http://qfk.0kj1m.cn

f() { return 0; }; f || echo "失败了"
来源：http://bfl.yanxiufei.cn

[R31] 局部变量
来源：http://xfx.yuxming.cn

f() { local x=1; echo "$x"; }
来源：http://wle.hesvh.cn

[R32] 参数个数校验
来源：http://wmz.jqgufenzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jpb.daria6918.cn

[R33] 捕获错误并提示行号
来源：http://yeg.xuetiantiany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://znd.dashuyun.cn

[R34] 退出时清理
来源：http://khv.jinghuilouyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hxe.aizwys.cn

[R35] 后台执行并等待
来源：http://yae.feifeiyinyue.top

sleep 5 & pid=$!; wait "$pid"
来源：http://kjg.jinghuilouyu.cn

[R36] 并发执行多个任务
来源：http://qxy.pycfn.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ntr.guowangkeji.top

[R37] 把输出赋给变量
来源：http://lab.yfazqb.com

files=$(ls -1)
来源：http://pbu.birdmap.top

[R38] 管道串联
来源：http://obh.chenzaomai.com

cat a.txt | grep -i error | wc -l
来源：http://pem.xziqi.cn

[R39] 重定向标准输出与错误
来源：http://zpd.hysaishi.cn

cmd > out.log 2>&1
来源：http://uhj.zdqjudy.top

[R40] 追加写日志
来源：http://srm.pengpengdd.cyou

echo "log" >> out.log
来源：http://lpc.sufxvd.cn

[R41] 丢弃输出
来源：http://igl.kuanghao11.cn

cmd >/dev/null 2>&1
来源：http://odw.aibaodan.cn

[R42] 输入重定向
来源：http://mvn.guowangkeji.top

wc -l < a.txt
来源：http://nrx.cqqwz.cn

[R43] 按名字查找文件
来源：http://plg.hfpthk.cn

find . -name "*.log" -type f
来源：http://ube.yonumen.top

[R44] 按修改时间查找
来源：http://wdt.shanyushiyangkeji.top

find . -mtime -7 -type f
来源：http://ski.haohaochexian.top

[R45] 批量删除
来源：http://mim.cashguo.top

find . -name "*.tmp" -delete
来源：http://iuj.ybcxt.top

[R46] 递归替换文件内容
来源：http://vxl.dashuyun.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://add.zhengqikj.top

[R47] sed 单行替换
来源：http://vmb.guowangkeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://uoq.sxryk.cn

[R48] awk 取指定列
来源：http://naa.jianghu66.top

awk '{print $1, $3}' a.txt
来源：http://tel.xingfuxueyuan.xyz

[R49] awk 带条件
来源：http://uoi.sufxvd.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lxl.gogol.net.cn

[R50] awk 求和
来源：http://kbj.jlsjyb.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qhg.ehwqpu.com

[R51] 排序去重取前几
来源：http://plc.zhongyouzk.top

sort a.txt | uniq -c | sort -rn | head
来源：http://qkn.hammf.cn

[R52] 统计行数
来源：http://drj.dashuyun.cn

wc -l a.txt
来源：http://psv.nanxuanxn.top

[R53] 查看文件头与实时尾
来源：http://ovd.yangfankeji.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gfm.svipenyu.cn

[R54] 比较两个文件
来源：http://mle.xuetiantiany.cn

diff a.txt b.txt
来源：http://izw.chenjidiqi.icu

[R55] 压缩与解压
来源：http://iql.havefunace.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://eth.haohaochexian.top

[R56] 远程拷贝
来源：http://qmb.meibo888.top

scp file user@host:/path/
来源：http://onz.guannengcc.top

[R57] 远程执行命令
来源：http://xii.chenlongwang.top

ssh user@host 'uptime'
来源：http://ubz.ehwqpu.com

[R58] 下载文件
来源：http://whu.kuanghao11.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oqd.zhiwuduotai.top

[R59] 发 POST JSON
来源：http://wub.feifeiyinyue.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://npj.gotoacloud.top

[R60] 只看 HTTP 状态码
来源：http://vnm.kuanghao11.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lrb.ehwqpu.com

[R61] 磁盘占用
来源：http://mmu.sweek.top

df -h;  du -sh *
来源：http://pax.shangyingyoupin.top

[R62] 找最占空间的文件
来源：http://klm.zhijiandao.cn

du -ah . | sort -rh | head -10
来源：http://plp.daria6918.cn

[R63] 内存与进程
来源：http://bai.cdnleiting.top

free -h;  ps aux | grep nginx
来源：http://lcd.sjlbkw.cn

[R64] 结束进程
来源：http://bvl.snrcjt.cn

kill -9 $(pgrep -f app.py)
来源：http://urw.fzhhl.top

[R65] 查看端口占用
来源：http://fbi.ctjpmb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://brb.jinqigufen.top

[R66] 定时任务
来源：http://xsa.xinyue.icu

crontab -e;  crontab -l
来源：http://vgi.dashuyun.cn

[R67] 生成随机十六进制串
来源：http://ave.birdmap.top

openssl rand -hex 16
来源：http://ykn.andypj.xyz

[R68] 计算文件校验值
来源：http://jxg.hesvh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tiu.zycfv.cn

[R69] 生成随机密码
来源：http://xfu.yuanzhike.top

head -c 16 /dev/urandom | base64
来源：http://lql.xingfuxueyuan.xyz

[R70] 时间戳与互转
来源：http://ytv.wangdashe.top

date +%s;  date -d @1700000000
来源：http://tzw.chenlongwang.top

[R71] 日期格式化
来源：http://lxy.hysaishi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sdu.yangfankeji.com

[R72] 等待端口就绪
来源：http://qfm.jianghu66.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qxq.epnwcf.com

[R73] 分割大日志
来源：http://dnq.iojbl.cn

split -l 1000 big.log part_
来源：http://ahj.hesvh.cn

[R74] 批量重命名
来源：http://vij.jianghu66.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tse.ywan-chungtsiang.top

[R75] 导出环境变量
来源：http://rfz.fanxiaobao.xyz

export PATH="$HOME/bin:$PATH"
来源：http://zkd.c1oappe.top

[R76] 使用临时文件
来源：http://dha.andypj.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jot.pengpengdd.cyou

[R77] 读取用户输入
来源：http://ift.cheryme.top

read -rp "请输入: " ans
来源：http://wjp.jinqigufen.top

[R78] 交互式菜单
来源：http://yfd.jqgufenzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://pfi.uphjek.com

[R79] 解析命令行选项
来源：http://rvi.zdbjq.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cba.ydjk.org.cn

[R80] 查看脚本执行耗时
来源：http://cpw.yuxming.cn

time ./run.sh
来源：http://pxq.shuidangran.top

================================================================================
来源：http://lru.jinqigufen.top

S. C / C++ 专题
来源：http://lvk.zdqjudy.top

================================================================================
来源：http://nsp.jiagoushi.top

[S01] C：Hello World
来源：http://lio.jqgufenzy.top

#include <stdio.h>
来源：http://qrm.yj20258.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rqh.ydjk.org.cn

[S02] C：变量与格式化输出
来源：http://rse.yj20258888.top

int a = 10; printf("%d\n", a);
来源：http://frb.yfazqb.com

[S03] C：读入整数
来源：http://rnn.yuanzhike.top

int x; scanf("%d", &x);
来源：http://vab.zhoulong.xyz

[S04] C：字符串复制
来源：http://ojd.quarkkingdee.top

char dst[32]; strcpy(dst, "hi");
来源：http://bwu.yj20258.top

[S05] C：字符串长度
来源：http://yzz.cashguo.top

strlen(s)
来源：http://fyb.epnwcf.com

[S06] C：字符串比较
来源：http://xcb.zycfv.cn

strcmp(a, b) == 0
来源：http://lnt.jiagoushi.top

[S07] C：数组遍历求和
来源：http://izi.chenjidiqi.icu

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ofn.shangyingyoupin.top

[S08] C：动态内存分配与释放
来源：http://paf.tanke756.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yhs.ctjpmb.com

[S09] C：结构体定义与初始化
来源：http://csb.fehbvm.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nmn.snrcjt.cn

[S10] C：指针与解引用
来源：http://qlt.yj20258888.top

int *p = &a;  *p = 5;
来源：http://upb.gzhubu.top

[S11] C：逐行读文件
来源：http://rcw.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "r");
来源：http://kkp.bbcook.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hsh.hfpthk.cn

fclose(f);
来源：http://kig.jianghu66.top

[S12] C：写文件
来源：http://qxb.vehdjk.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qoj.hcnkem.com

[S13] C：宏定义
来源：http://suv.hcnkem.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jbg.nanxuanxn.top

[S14] C：枚举
来源：http://asa.iojbl.cn

enum Color { RED, GREEN, BLUE };
来源：http://jrf.zhaomingkeji.xyz

[S15] C：类型转换
来源：http://vkp.vehdjk.com

(double) a / b
来源：http://jkc.fehbvm.com

[S16] C：位操作置位
来源：http://ife.redwolf501.top

x |= (1 << 3);
来源：http://wqo.chenzaomai.com

[S17] C：安全拼接字符串
来源：http://cqb.meibo888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hgb.ehwqpu.com

[S18] C：命令行参数
来源：http://vpj.zhaomingkeji.xyz

int main(int argc, char **argv)
来源：http://fcc.316326.xyz

[S19] C：快速排序
来源：http://xyk.shzxlz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://oxv.jinghuilouyu.cn

[S20] C：二分查找
来源：http://yut.zhengqikj.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dlg.tanke756.top

[S21] C：字符类别判断
来源：http://srk.yvedp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lrc.ywan-chungtsiang.top

[S22] C：字符串转数字
来源：http://jyr.chenlongwang.top

atoi("42");  strtod("3.14", NULL);
来源：http://udl.jyoumei.cn

[S23] C：随机数
来源：http://hni.316326.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://erd.pycfn.com

[S24] C：获取本地时间
来源：http://xwr.sysykeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://opq.guannengcc.top

[S25] C：内存拷贝
来源：http://pef.ctjpmb.com

memcpy(dst, src, n);
来源：http://fpf.vqdsnc.cn

[S26] C：内存清零
来源：http://ahl.gotoacloud.top

memset(a, 0, sizeof a);
来源：http://joh.316326.xyz

[S27] C：定义常量
来源：http://ugx.tian-w.cn

const double PI = 3.14159;
来源：http://mnd.ydjk.org.cn

[S28] C：静态变量
来源：http://gra.yonumen.top

static int counter = 0;
来源：http://yrx.9152youxi.cn

[S29] C：变参函数
来源：http://plx.hnqzz.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ecm.birdmap.top

[S30] C：头文件保护
来源：http://tcu.52xcode.cn

#ifndef X_H
来源：http://phh.hcnkem.com

#define X_H
来源：http://jtn.yj202588.top

#endif
来源：http://ofr.pycfn.com

[S31] C++：Hello World
来源：http://lrh.c1oappe.top

#include <iostream>
来源：http://jmk.xuetiantiany.cn

int main() { std::cout << "Hello\n"; }
来源：http://yct.fengsongda.top

[S32] C++：字符串
来源：http://edm.sweek.top

std::string s = "hi";  s += "!";
来源：http://vmt.fzhhl.top

[S33] C++：vector 增删
来源：http://bhq.tian-w.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lhj.gaohongyu789.top

[S34] C++：遍历 vector
来源：http://vol.cashguo.top

for (auto &x : v) { std::cout << x; }
来源：http://yah.yvedp.cn

[S35] C++：map
来源：http://jhr.zhijiandao.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bdq.chenlongwang.top

[S36] C++：unordered_map
来源：http://tql.vehdjk.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://spx.epnwcf.com

[S37] C++：set
来源：http://dgv.sufxvd.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://khb.zhixingplan.top

[S38] C++：排序
来源：http://lrp.gzhubu.top

std::sort(v.begin(), v.end());
来源：http://blk.ivvv.top

[S39] C++：自定义比较器排序
来源：http://vyc.yj202588.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dbu.shzxlz.cn

[S40] C++：查找元素
来源：http://bqb.yongpay.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yyr.pengpengdd.cyou

[S41] C++：类与构造函数
来源：http://ygw.fehbvm.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ywk.ydjk.org.cn

[S42] C++：继承与虚函数
来源：http://zir.shuidangran.top

class B : public Base { public: void f() override {} };
来源：http://jrh.ydzc1.top

[S43] C++：智能指针
来源：http://mrb.guowangkeji.top

auto p = std::make_unique<int>(5);
来源：http://icp.hnqzz.top

[S44] C++：引用传参
来源：http://tjy.shanyushiyangkeji.top

void inc(int &x) { ++x; }
来源：http://ivx.hammf.cn

[S45] C++：lambda
来源：http://vqs.dianchejie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rwg.aibaodan.cn

[S46] C++：函数模板
来源：http://ewd.sjlbkw.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bfl.xuetiantiany.cn

[S47] C++：结构化绑定遍历
来源：http://xau.nwbrower.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://eco.redwolf501.top

[S48] C++：逐行读文件
来源：http://yfo.jyoumei.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rkq.meibo888.top

while (std::getline(in, line)) { }
来源：http://jvj.xziqi.cn

[S49] C++：写文件
来源：http://yqb.9152youxi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vpx.shangyingyoupin.top

[S50] C++：格式化数字
来源：http://wto.hywenlv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://txg.jiagoushi.top

[S51] C++：显式类型转换
来源：http://tye.snrcjt.cn

static_cast<double>(a) / b
来源：http://uwz.gogol.net.cn

[S52] C++：const 与 noexcept
来源：http://sfk.ivvv.top

int size() const noexcept { return n_; }
来源：http://ult.jinqigufen.top

[S53] C++：移动语义
来源：http://dqq.andypj.xyz

std::vector<int> w = std::move(v);
来源：http://cpu.yvedp.cn

[S54] C++：异常处理
来源：http://eox.sxryk.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uvp.xylfe.cn

[S55] C++：结构化绑定
来源：http://gbm.zhengqikj.top

auto [a, b] = std::make_pair(1, 2);
来源：http://eyp.nwbrower.top

[S56] C++：optional
来源：http://xxm.ydzc1.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bea.nwbrower.top

[S57] C++：编译期常量
来源：http://eof.nanxinkj.top

constexpr int N = 10;
来源：http://gkc.sjlbkw.cn

[S58] C++：命名空间
来源：http://tww.dianchejie.cn

namespace ns { int f() { return 1; } }
来源：http://dkh.wangshuangyany.cn

[S59] C++：静态断言
来源：http://wxg.yuxming.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://elx.cdnleiting.top

[S60] C++：遍历并删除元素
来源：http://zwc.epnwcf.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wod.yueranfly.top

================================================================================
来源：http://zrg.uphjek.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cvq.yj20258888.top

================================================================================
来源：http://qxp.gzhubu.top

[T01] Kotlin：Hello World
来源：http://xlz.yuxming.cn

println("Hello")
来源：http://fgo.chenzaomai.com

[T02] Kotlin：变量
来源：http://umx.nanxinkj.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://csn.ctjpmb.com

[T03] Kotlin：字符串模板
来源：http://ggh.ybcxt.top

"值: $b"
来源：http://rgg.chenlongwang.top

[T04] Kotlin：空安全
来源：http://fid.sxryk.cn

val n: String? = null;  n?.length
来源：http://qaf.zhaomingkeji.xyz

[T05] Kotlin：when 表达式
来源：http://iwg.hfpthk.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fic.gzhubu.top

[T06] Kotlin：集合映射
来源：http://gyw.zdqjudy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://acd.xziqi.cn

[T07] Kotlin：集合过滤
来源：http://css.smart0.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://sqb.ctjpmb.com

[T08] Kotlin：数据类
来源：http://vxu.meibo888.top

data class User(val name: String, val age: Int)
来源：http://tpg.tianlin.xyz

[T09] Kotlin：扩展函数
来源：http://tfl.wangshuangyany.cn

fun String.exclaim() = this + "!"
来源：http://ufu.jyoumei.cn

[T10] Kotlin：默认参数
来源：http://ukt.sysykeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://pfx.zdqjudy.top

[T11] Kotlin：协程
来源：http://xnm.ctjpmb.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://iaj.chenjidiqi.icu

[T12] Kotlin：解构声明
来源：http://cio.yonumen.top

val (a, b) = Pair(1, 2)
来源：http://fyi.feifeiyinyue.top

[T13] Kotlin：只读 Map
来源：http://ysp.fanxiaobao.xyz

val m = mapOf("a" to 1)
来源：http://lzf.dashuyun.cn

[T14] Kotlin：循环
来源：http://smy.epnwcf.com

for (i in 1..10) println(i)
来源：http://czw.hammf.cn

[T15] Kotlin：接口
来源：http://fgy.yvedp.cn

interface Shape { fun area(): Double }
来源：http://pzr.xuanzx.com

[T16] Swift：Hello World
来源：http://xsq.wangdashe.top

print("Hello")
来源：http://zvt.pycfn.com

[T17] Swift：变量与常量
来源：http://eqt.fktsv.cn

var a = 1;  let b = 2
来源：http://zwi.ppjwa.cn

[T18] Swift：字符串插值
来源：http://coa.shuidangran.top

"值: \(b)"
来源：http://jlz.zhiwuduotai.top

[T19] Swift：可选绑定
来源：http://ryl.snrcjt.cn

if let n = opt { print(n) }
来源：http://add.zhongyouzk.top

[T20] Swift：数组操作
来源：http://plc.ctjpmb.com

var a = [1, 2, 3];  a.append(4)
来源：http://cmc.guannengcc.top

[T21] Swift：遍历
来源：http://zgj.yj20258888.top

for x in a { print(x) }
来源：http://ozs.zhoulong.xyz

[T22] Swift：字典
来源：http://srp.fzhhl.top

var d = ["a": 1];  d["b"] = 2
来源：http://ifr.zdqjudy.top

[T23] Swift：函数
来源：http://yfp.sxryk.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://iry.0kj1m.cn

[T24] Swift：闭包
来源：http://zsl.ydjk.org.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jpn.aizwys.cn

[T25] Swift：结构体
来源：http://bfq.gaohongyu789.top

struct P { var x: Int }
来源：http://kxo.aibaodan.cn

[T26] Swift：类与重写
来源：http://olo.jinghuilouyu.cn

class A: Base { override func f() {} }
来源：http://jhp.jinqigufen.top

[T27] Swift：错误处理
来源：http://tze.redwolf501.top

do { try f() } catch { print(error) }
来源：http://pzg.shuidangran.top

[T28] Swift：枚举
来源：http://xvl.hysaishi.cn

enum Color { case red, green }
来源：http://cwj.tanke756.top

[T29] Swift：guard 提前返回
来源：http://mjq.cashguo.top

guard let x = opt else { return }
来源：http://ejo.xuetiantiany.cn

[T30] Swift：协议
来源：http://kgq.hysaishi.cn

protocol Shape { func area() -> Double }
来源：http://vpy.hcnkem.com

[T31] Lua：Hello World
来源：http://jna.ehwqpu.com

print("Hello")
来源：http://sse.wangdashe.top

[T32] Lua：局部变量
来源：http://pqo.aizwys.cn

local a = 1
来源：http://juz.jinyuanbaomall.cn


<!-- 参考信息 -->