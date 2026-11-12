代发 wailian999

echo $((1 + 2 * 3))
来源：http://vyz.zhijiandao.cn

[R28] 浮点运算
来源：http://was.shuidangran.top

echo "scale=2; 10/3" | bc
来源：http://dtm.shuidangran.top

[R29] 定义函数
来源：http://zwz.yanxiufei.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rjv.hnqzz.top

[R30] 函数返回状态码
来源：http://vhj.yueranfly.top

f() { return 0; }; f || echo "失败了"
来源：http://fxf.c1oappe.top

[R31] 局部变量
来源：http://gci.ybcxt.top

f() { local x=1; echo "$x"; }
来源：http://gwp.yuanzhike.top

[R32] 参数个数校验
来源：http://mad.sjlbkw.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gcr.hcnkem.com

[R33] 捕获错误并提示行号
来源：http://fge.xuanzx.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wno.hysaishi.cn

[R34] 退出时清理
来源：http://kuu.ctjpmb.com

trap 'rm -f "$tmp"' EXIT
来源：http://vfx.yuanzhike.top

[R35] 后台执行并等待
来源：http://zwx.yueranfly.top

sleep 5 & pid=$!; wait "$pid"
来源：http://rst.uphjek.com

[R36] 并发执行多个任务
来源：http://fgd.zhijiandao.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vog.xziqi.cn

[R37] 把输出赋给变量
来源：http://qhi.smart0.xyz

files=$(ls -1)
来源：http://izc.sufxvd.cn

[R38] 管道串联
来源：http://cbf.haohaochexian.top

cat a.txt | grep -i error | wc -l
来源：http://zvw.svipenyu.cn

[R39] 重定向标准输出与错误
来源：http://zne.daxiang520.top

cmd > out.log 2>&1
来源：http://con.tarul.cn

[R40] 追加写日志
来源：http://gvq.sufxvd.cn

echo "log" >> out.log
来源：http://sml.birdmap.top

[R41] 丢弃输出
来源：http://mea.hnxiangtu.top

cmd >/dev/null 2>&1
来源：http://xmf.ydjk.org.cn

[R42] 输入重定向
来源：http://ckb.tian-w.cn

wc -l < a.txt
来源：http://ncx.ydzc1.top

[R43] 按名字查找文件
来源：http://obz.hywenlv.cn

find . -name "*.log" -type f
来源：http://vtg.hcnkem.com

[R44] 按修改时间查找
来源：http://rfd.cashguo.top

find . -mtime -7 -type f
来源：http://gvy.jqgfzy.top

[R45] 批量删除
来源：http://yxn.havefunace.top

find . -name "*.tmp" -delete
来源：http://aly.birdmap.top

[R46] 递归替换文件内容
来源：http://aup.hcnkem.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bvs.jinyuanbaomall.cn

[R47] sed 单行替换
来源：http://utr.jianghu66.top

sed -i 's/foo/bar/g' a.txt
来源：http://daa.ydjk.org.cn

[R48] awk 取指定列
来源：http://kon.epnwcf.com

awk '{print $1, $3}' a.txt
来源：http://oky.sysykeji.top

[R49] awk 带条件
来源：http://geb.316326.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cho.ctjpmb.com

[R50] awk 求和
来源：http://wbm.hysaishi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fex.xuanzx.com

[R51] 排序去重取前几
来源：http://bdo.iojbl.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rfj.yj20258.top

[R52] 统计行数
来源：http://ldc.hywenlv.cn

wc -l a.txt
来源：http://fay.ehwqpu.com

[R53] 查看文件头与实时尾
来源：http://hhd.shangyingyoupin.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gpk.chenlongwang.top

[R54] 比较两个文件
来源：http://say.shanyushiyangkeji.top

diff a.txt b.txt
来源：http://vdy.chenjidiqi.icu

[R55] 压缩与解压
来源：http://fwx.sxryk.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://iuj.smart0.xyz

[R56] 远程拷贝
来源：http://eoe.316326.xyz

scp file user@host:/path/
来源：http://eqb.aizwys.cn

[R57] 远程执行命令
来源：http://zwg.0kj1m.cn

ssh user@host 'uptime'
来源：http://wki.yuanzhike.top

[R58] 下载文件
来源：http://rhu.ydjk.org.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fny.fanxiaobao.xyz

[R59] 发 POST JSON
来源：http://hth.svipenyu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dep.uphjek.com

[R60] 只看 HTTP 状态码
来源：http://dbu.yuxming.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oax.andypj.xyz

[R61] 磁盘占用
来源：http://edy.52xcode.cn

df -h;  du -sh *
来源：http://obo.jinyuanbaomall.cn

[R62] 找最占空间的文件
来源：http://mwn.wangshuangyany.cn

du -ah . | sort -rh | head -10
来源：http://oil.pycfn.com

[R63] 内存与进程
来源：http://nqm.shanyushiyangkeji.top

free -h;  ps aux | grep nginx
来源：http://atn.hongshengwenyu.top

[R64] 结束进程
来源：http://iyu.cucudq.cn

kill -9 $(pgrep -f app.py)
来源：http://ckz.fengsongda.top

[R65] 查看端口占用
来源：http://php.sjlbkw.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nso.meibo888.top

[R66] 定时任务
来源：http://nln.zhaomingkeji.xyz

crontab -e;  crontab -l
来源：http://udz.ywan-chungtsiang.top

[R67] 生成随机十六进制串
来源：http://uyl.yuanzhike.top

openssl rand -hex 16
来源：http://tql.nanxinkj.top

[R68] 计算文件校验值
来源：http://oei.yongpay.top

sha256sum a.txt;  md5sum a.txt
来源：http://juc.daxiang520.top

[R69] 生成随机密码
来源：http://nly.xylfe.cn

head -c 16 /dev/urandom | base64
来源：http://xjk.quarkkingdee.top

[R70] 时间戳与互转
来源：http://lca.sweek.top

date +%s;  date -d @1700000000
来源：http://wyu.yuxming.cn

[R71] 日期格式化
来源：http://cic.dashuyun.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ixq.tian-w.cn

[R72] 等待端口就绪
来源：http://nag.shangyingyoupin.top

until nc -z localhost 3306; do sleep 1; done
来源：http://smj.chenjidiqi.icu

[R73] 分割大日志
来源：http://ogb.fengsongda.top

split -l 1000 big.log part_
来源：http://tbg.fktsv.cn

[R74] 批量重命名
来源：http://qox.xingfuxueyuan.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bxx.yueranfly.top

[R75] 导出环境变量
来源：http://yek.yj20258888.top

export PATH="$HOME/bin:$PATH"
来源：http://cik.jiagoushi.top

[R76] 使用临时文件
来源：http://yxg.c1oappe.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jes.zdbjq.cn

[R77] 读取用户输入
来源：http://pof.zdqjudy.top

read -rp "请输入: " ans
来源：http://zil.snrcjt.cn

[R78] 交互式菜单
来源：http://bca.tanke756.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rjr.ydjk.org.cn

[R79] 解析命令行选项
来源：http://ddz.guannengcc.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xim.feifeiyinyue.top

[R80] 查看脚本执行耗时
来源：http://rvr.fktsv.cn

time ./run.sh
来源：http://wxa.ybcxt.top

================================================================================
来源：http://vlh.tarul.cn

S. C / C++ 专题
来源：http://kma.sjlbkw.cn

================================================================================
来源：http://kfc.zhiwuduotai.top

[S01] C：Hello World
来源：http://bck.daxiang520.top

#include <stdio.h>
来源：http://rdl.cdnleiting.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gox.jinyuanbaomall.cn

[S02] C：变量与格式化输出
来源：http://duz.feifeiyinyue.top

int a = 10; printf("%d\n", a);
来源：http://oei.yfazqb.com

[S03] C：读入整数
来源：http://csc.xinyue.icu

int x; scanf("%d", &x);
来源：http://oei.yueranfly.top

[S04] C：字符串复制
来源：http://izv.xuanzx.com

char dst[32]; strcpy(dst, "hi");
来源：http://tek.yueranfly.top

[S05] C：字符串长度
来源：http://upt.snrcjt.cn

strlen(s)
来源：http://mmf.yj20258.top

[S06] C：字符串比较
来源：http://mte.yangfankeji.com

strcmp(a, b) == 0
来源：http://ngt.sufxvd.cn

[S07] C：数组遍历求和
来源：http://hel.bjfxy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://guk.bjfxy.top

[S08] C：动态内存分配与释放
来源：http://tkz.dashuyun.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://aha.mhx1999.top

[S09] C：结构体定义与初始化
来源：http://mrv.sxryk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://reo.redwolf501.top

[S10] C：指针与解引用
来源：http://jmj.9152youxi.cn

int *p = &a;  *p = 5;
来源：http://xrq.dashuyun.cn

[S11] C：逐行读文件
来源：http://zes.ybcxt.top

FILE *f = fopen("a.txt", "r");
来源：http://fnz.snrcjt.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hbh.epnwcf.com

fclose(f);
来源：http://qom.xziqi.cn

[S12] C：写文件
来源：http://keb.ctjpmb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ouf.feifeiyinyue.top

[S13] C：宏定义
来源：http://hvr.zhijiandao.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qxe.xuanzx.com

[S14] C：枚举
来源：http://yrh.jinyuanbaomall.cn

enum Color { RED, GREEN, BLUE };
来源：http://prd.hywenlv.cn

[S15] C：类型转换
来源：http://dpp.kuanghao11.cn

(double) a / b
来源：http://lnc.yonumen.top

[S16] C：位操作置位
来源：http://xng.ywan-chungtsiang.top

x |= (1 << 3);
来源：http://esm.cqqwz.cn

[S17] C：安全拼接字符串
来源：http://nwg.yueranfly.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vlf.ivvv.top

[S18] C：命令行参数
来源：http://baz.ywan-chungtsiang.top

int main(int argc, char **argv)
来源：http://hlf.hnxiangtu.top

[S19] C：快速排序
来源：http://lyh.andypj.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://ypj.ctjpmb.com

[S20] C：二分查找
来源：http://ecg.yueranfly.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qkd.guowangkeji.top

[S21] C：字符类别判断
来源：http://cpb.hcnkem.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rtg.zhengqikj.top

[S22] C：字符串转数字
来源：http://fei.fehbvm.com

atoi("42");  strtod("3.14", NULL);
来源：http://nxl.yfazqb.com

[S23] C：随机数
来源：http://xgy.daxiang520.top

srand(time(NULL));  int r = rand() % 100;
来源：http://zzg.cucudq.cn

[S24] C：获取本地时间
来源：http://ezq.zhengqikj.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zle.sysykeji.top

[S25] C：内存拷贝
来源：http://auz.cheryme.top

memcpy(dst, src, n);
来源：http://kfm.epnwcf.com

[S26] C：内存清零
来源：http://iep.tianlin.xyz

memset(a, 0, sizeof a);
来源：http://vks.hfpthk.cn

[S27] C：定义常量
来源：http://zru.quarkkingdee.top

const double PI = 3.14159;
来源：http://tqq.yj20258888.top

[S28] C：静态变量
来源：http://gqo.smart0.xyz

static int counter = 0;
来源：http://xrl.birdmap.top

[S29] C：变参函数
来源：http://hgr.zhiwuduotai.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://aux.jyoumei.cn

[S30] C：头文件保护
来源：http://evk.xingfuxueyuan.xyz

#ifndef X_H
来源：http://tyi.zhaomingkeji.xyz

#define X_H
来源：http://tit.xuetiantiany.cn

#endif
来源：http://orr.ybcxt.top

[S31] C++：Hello World
来源：http://ljl.ivvv.top

#include <iostream>
来源：http://tcc.xylfe.cn

int main() { std::cout << "Hello\n"; }
来源：http://nzp.aibaodan.cn

[S32] C++：字符串
来源：http://nfd.shanyushiyangtech.top

std::string s = "hi";  s += "!";
来源：http://yye.aizwys.cn

[S33] C++：vector 增删
来源：http://lut.sweek.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yiz.ydzc1.top

[S34] C++：遍历 vector
来源：http://vge.sweek.top

for (auto &x : v) { std::cout << x; }
来源：http://acc.zhengqikj.top

[S35] C++：map
来源：http://vnm.svipenyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oxi.yj20258888.top

[S36] C++：unordered_map
来源：http://okq.wangdashe.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://erh.yanxiufei.cn

[S37] C++：set
来源：http://hqe.jinghuilouyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://aoi.jinqigfzy.top

[S38] C++：排序
来源：http://asn.chenzaomai.com

std::sort(v.begin(), v.end());
来源：http://rmm.zhengqikj.top

[S39] C++：自定义比较器排序
来源：http://tny.bbcook.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dko.xylfe.cn

[S40] C++：查找元素
来源：http://vnq.jinqigufen.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ktw.nwbrower.top

[S41] C++：类与构造函数
来源：http://vgd.yvedp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ntq.nwbrower.top

[S42] C++：继承与虚函数
来源：http://hzz.zhixingplan.top

class B : public Base { public: void f() override {} };
来源：http://lxm.bjfxy.top

[S43] C++：智能指针
来源：http://tde.nwbrower.top

auto p = std::make_unique<int>(5);
来源：http://tco.daxiang520.top

[S44] C++：引用传参
来源：http://kyl.hnqzz.top

void inc(int &x) { ++x; }
来源：http://mzz.aizwys.cn

[S45] C++：lambda
来源：http://ovl.aibaodan.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mvz.zycfv.cn

[S46] C++：函数模板
来源：http://gqg.chenlongwang.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bhe.ppjwa.cn

[S47] C++：结构化绑定遍历
来源：http://zqy.snrcjt.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zed.sweek.top

[S48] C++：逐行读文件
来源：http://gyd.kuanghao11.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rmv.cqqwz.cn

while (std::getline(in, line)) { }
来源：http://fem.9152youxi.cn

[S49] C++：写文件
来源：http://jns.0kj1m.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://woj.yj20258888.top

[S50] C++：格式化数字
来源：http://ofi.shanyushiyangkeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bdw.yj20258888.top

[S51] C++：显式类型转换
来源：http://oog.dashuyun.cn

static_cast<double>(a) / b
来源：http://ehm.wangdashe.top

[S52] C++：const 与 noexcept
来源：http://yqx.hesvh.cn

int size() const noexcept { return n_; }
来源：http://bhg.chenjidiqi.icu

[S53] C++：移动语义
来源：http://nsb.quarkkingdee.top

std::vector<int> w = std::move(v);
来源：http://ijs.hnqzz.top

[S54] C++：异常处理
来源：http://vut.fengsongda.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qoo.sufxvd.cn

[S55] C++：结构化绑定
来源：http://xaw.xziqi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vte.chenlongwang.top

[S56] C++：optional
来源：http://nxj.wangdashe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ffh.xziqi.cn

[S57] C++：编译期常量
来源：http://ztq.nanxuanxn.top

constexpr int N = 10;
来源：http://hta.ywan-chungtsiang.top

[S58] C++：命名空间
来源：http://lnx.chenzaomai.com

namespace ns { int f() { return 1; } }
来源：http://too.tanke756.top

[S59] C++：静态断言
来源：http://opb.dashuyun.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eow.hnqzz.top

[S60] C++：遍历并删除元素
来源：http://bga.hfpthk.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lfw.ybcxt.top

================================================================================
来源：http://grx.ywan-chungtsiang.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nrd.zhoulong.xyz

================================================================================
来源：http://xgt.nwbrower.top

[T01] Kotlin：Hello World
来源：http://znh.9152youxi.cn

println("Hello")
来源：http://mzw.zycfv.cn

[T02] Kotlin：变量
来源：http://fue.ehwqpu.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lne.yj20258.top

[T03] Kotlin：字符串模板
来源：http://gkp.dianchejie.cn

"值: $b"
来源：http://llb.yonumen.top

[T04] Kotlin：空安全
来源：http://cpy.jqgfzy.top

val n: String? = null;  n?.length
来源：http://iro.chenlongwang.top

[T05] Kotlin：when 表达式
来源：http://tlq.jinqigfzy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wxk.havefunace.top

[T06] Kotlin：集合映射
来源：http://zhc.dianchejie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gud.chenlongwang.top

[T07] Kotlin：集合过滤
来源：http://ncs.fehbvm.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://gcn.cucudq.cn

[T08] Kotlin：数据类
来源：http://zkt.cheryme.top

data class User(val name: String, val age: Int)
来源：http://bmt.havefunace.top

[T09] Kotlin：扩展函数
来源：http://sos.fanxiaobao.xyz

fun String.exclaim() = this + "!"
来源：http://hys.yvedp.cn

[T10] Kotlin：默认参数
来源：http://buq.zhixingplan.top

fun greet(name: String = "World") = "Hi $name"
来源：http://jbg.jianghu66.top

[T11] Kotlin：协程
来源：http://nki.fzhhl.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://jma.hywenlv.cn

[T12] Kotlin：解构声明
来源：http://imb.sxryk.cn

val (a, b) = Pair(1, 2)
来源：http://cgq.hysaishi.cn

[T13] Kotlin：只读 Map
来源：http://pxi.fzhhl.top

val m = mapOf("a" to 1)
来源：http://ruh.dianchejie.cn

[T14] Kotlin：循环
来源：http://jso.ppjwa.cn

for (i in 1..10) println(i)
来源：http://tln.yuxming.cn

[T15] Kotlin：接口
来源：http://mlg.shzxlz.cn

interface Shape { fun area(): Double }
来源：http://grp.cashguo.top

[T16] Swift：Hello World
来源：http://whu.yj20258888.top

print("Hello")
来源：http://bjl.xylfe.cn

[T17] Swift：变量与常量
来源：http://ymq.chenzaomai.com

var a = 1;  let b = 2
来源：http://fql.xuanzx.com

[T18] Swift：字符串插值
来源：http://fbm.zhiwuduotai.top

"值: \(b)"
来源：http://kuw.ctjpmb.com

[T19] Swift：可选绑定
来源：http://ppi.meibo888.top

if let n = opt { print(n) }
来源：http://cyr.jqgfzy.top

[T20] Swift：数组操作
来源：http://fss.316326.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://soo.jinqigfzy.top

[T21] Swift：遍历
来源：http://tdm.chenzaomai.com

for x in a { print(x) }
来源：http://zjl.nwbrower.top

[T22] Swift：字典
来源：http://jpm.ctjpmb.com

var d = ["a": 1];  d["b"] = 2
来源：http://fho.shangyingyoupin.top

[T23] Swift：函数
来源：http://dsz.svipenyu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rml.9152youxi.cn

[T24] Swift：闭包
来源：http://svo.nanxinkj.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://zyz.jianghu66.top

[T25] Swift：结构体
来源：http://zyk.hammf.cn

struct P { var x: Int }
来源：http://iue.zycfv.cn

[T26] Swift：类与重写
来源：http://psk.zhijiandao.cn

class A: Base { override func f() {} }
来源：http://okw.jlsjyb.cn

[T27] Swift：错误处理
来源：http://qru.nwbrower.top

do { try f() } catch { print(error) }
来源：http://opg.redwolf501.top

[T28] Swift：枚举
来源：http://xsd.xylfe.cn

enum Color { case red, green }
来源：http://nxq.ehwqpu.com

[T29] Swift：guard 提前返回
来源：http://ruc.yuanzhike.top

guard let x = opt else { return }
来源：http://nem.9152youxi.cn

[T30] Swift：协议
来源：http://cyi.hnxiangtu.top

protocol Shape { func area() -> Double }
来源：http://nnk.chenzaomai.com


<!-- 参考信息 -->