代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://qma.yj202588.top

[R26] 命令替换
来源：http://yfz.tanke756.top

now=$(date +%F); echo "$now"
来源：http://ezo.haohaochexian.top

[R27] 算术展开
来源：http://zpk.fanxiaobao.xyz

echo $((1 + 2 * 3))
来源：http://qey.zhiwuduotai.top

[R28] 浮点运算
来源：http://akp.jqgufenzy.top

echo "scale=2; 10/3" | bc
来源：http://rik.jyoumei.cn

[R29] 定义函数
来源：http://ldd.fzhhl.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://teg.xuanzx.com

[R30] 函数返回状态码
来源：http://zuk.fktsv.cn

f() { return 0; }; f || echo "失败了"
来源：http://hkt.zdbjq.cn

[R31] 局部变量
来源：http://idy.chenlongwang.top

f() { local x=1; echo "$x"; }
来源：http://kzs.jianghu66.top

[R32] 参数个数校验
来源：http://ngp.dianchejie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uji.feifeiyinyue.top

[R33] 捕获错误并提示行号
来源：http://zyd.yj20258888.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qjv.ywan-chungtsiang.top

[R34] 退出时清理
来源：http://ecc.mhx1999.top

trap 'rm -f "$tmp"' EXIT
来源：http://kgg.ehwqpu.com

[R35] 后台执行并等待
来源：http://hju.yj20258.top

sleep 5 & pid=$!; wait "$pid"
来源：http://zww.wangdashe.top

[R36] 并发执行多个任务
来源：http://gmc.chenjidiqi.icu

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://aou.ydzc1.top

[R37] 把输出赋给变量
来源：http://zkl.ehwqpu.com

files=$(ls -1)
来源：http://nai.meibo888.top

[R38] 管道串联
来源：http://vir.zhongyouzk.top

cat a.txt | grep -i error | wc -l
来源：http://vza.zhengqikj.top

[R39] 重定向标准输出与错误
来源：http://kwo.c1oappe.top

cmd > out.log 2>&1
来源：http://tek.havefunace.top

[R40] 追加写日志
来源：http://mgw.ybcxt.top

echo "log" >> out.log
来源：http://hto.fanxiaobao.xyz

[R41] 丢弃输出
来源：http://ada.tarul.cn

cmd >/dev/null 2>&1
来源：http://ksy.pycfn.com

[R42] 输入重定向
来源：http://her.tian-w.cn

wc -l < a.txt
来源：http://yxp.aibaodan.cn

[R43] 按名字查找文件
来源：http://frz.fzhhl.top

find . -name "*.log" -type f
来源：http://sox.tanke756.top

[R44] 按修改时间查找
来源：http://hqb.hywenlv.cn

find . -mtime -7 -type f
来源：http://xax.zhoulong.xyz

[R45] 批量删除
来源：http://pux.shanyushiyangkeji.top

find . -name "*.tmp" -delete
来源：http://wbv.fanxiaobao.xyz

[R46] 递归替换文件内容
来源：http://jxn.hesvh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hsm.nanxuanxn.top

[R47] sed 单行替换
来源：http://jmu.9152youxi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vez.zhijiandao.cn

[R48] awk 取指定列
来源：http://lnk.tarul.cn

awk '{print $1, $3}' a.txt
来源：http://pif.yongpay.top

[R49] awk 带条件
来源：http://wzm.chenjidiqi.icu

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cwz.jinqigufen.top

[R50] awk 求和
来源：http://icq.sjlbkw.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ege.cdnleiting.top

[R51] 排序去重取前几
来源：http://ihg.sufxvd.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lpc.yuxming.cn

[R52] 统计行数
来源：http://anz.nwbrower.top

wc -l a.txt
来源：http://hgk.cucudq.cn

[R53] 查看文件头与实时尾
来源：http://oal.nwbrower.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yar.birdmap.top

[R54] 比较两个文件
来源：http://lqi.pengpengdd.cyou

diff a.txt b.txt
来源：http://dwh.hesvh.cn

[R55] 压缩与解压
来源：http://wfe.fengsongda.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uyl.feifeiyinyue.top

[R56] 远程拷贝
来源：http://yof.shanyushiyangkeji.top

scp file user@host:/path/
来源：http://zjk.smart0.xyz

[R57] 远程执行命令
来源：http://eph.shangyingyoupin.top

ssh user@host 'uptime'
来源：http://ooy.shangyingyoupin.top

[R58] 下载文件
来源：http://hwk.wangshuangyany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://aie.zdbjq.cn

[R59] 发 POST JSON
来源：http://prk.smart0.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://edl.gzhubu.top

[R60] 只看 HTTP 状态码
来源：http://kqu.vehdjk.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rgp.tian-w.cn

[R61] 磁盘占用
来源：http://xct.xziqi.cn

df -h;  du -sh *
来源：http://rzd.sjlbkw.cn

[R62] 找最占空间的文件
来源：http://yfq.fzhhl.top

du -ah . | sort -rh | head -10
来源：http://snq.svipenyu.cn

[R63] 内存与进程
来源：http://ghh.pycfn.com

free -h;  ps aux | grep nginx
来源：http://uqo.shanyushiyangtech.top

[R64] 结束进程
来源：http://qmp.snrcjt.cn

kill -9 $(pgrep -f app.py)
来源：http://kzn.yj20258.top

[R65] 查看端口占用
来源：http://vdq.meibo888.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kag.fehbvm.com

[R66] 定时任务
来源：http://guw.bjfxy.top

crontab -e;  crontab -l
来源：http://vfh.gzhubu.top

[R67] 生成随机十六进制串
来源：http://jot.guowangkeji.top

openssl rand -hex 16
来源：http://uha.yonumen.top

[R68] 计算文件校验值
来源：http://ujj.hesvh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qpr.meibo888.top

[R69] 生成随机密码
来源：http://pru.jinqigfzy.top

head -c 16 /dev/urandom | base64
来源：http://acc.cqqwz.cn

[R70] 时间戳与互转
来源：http://cxd.yueranfly.top

date +%s;  date -d @1700000000
来源：http://jbl.316326.xyz

[R71] 日期格式化
来源：http://ava.chenzaomai.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://aqk.yvedp.cn

[R72] 等待端口就绪
来源：http://ddx.hysaishi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://uhb.cucudq.cn

[R73] 分割大日志
来源：http://mmz.jinghuilouyu.cn

split -l 1000 big.log part_
来源：http://tlr.jinghuilouyu.cn

[R74] 批量重命名
来源：http://lyu.shanyushiyangkeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rjx.zdqjudy.top

[R75] 导出环境变量
来源：http://qpv.feifeiyinyue.top

export PATH="$HOME/bin:$PATH"
来源：http://bed.gzhubu.top

[R76] 使用临时文件
来源：http://mkq.shanyushiyangtech.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vfu.316326.xyz

[R77] 读取用户输入
来源：http://jja.ppjwa.cn

read -rp "请输入: " ans
来源：http://mji.aibaodan.cn

[R78] 交互式菜单
来源：http://ztv.nanxinkj.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xey.gotoacloud.top

[R79] 解析命令行选项
来源：http://sup.meibo888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sik.yuxming.cn

[R80] 查看脚本执行耗时
来源：http://bxm.zhongyouzk.top

time ./run.sh
来源：http://ojg.zdbjq.cn

================================================================================
来源：http://amf.tarul.cn

S. C / C++ 专题
来源：http://tyr.zhiwuduotai.top

================================================================================
来源：http://ehi.dashuyun.cn

[S01] C：Hello World
来源：http://axz.redwolf501.top

#include <stdio.h>
来源：http://slz.yonumen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://taa.feifeiyinyue.top

[S02] C：变量与格式化输出
来源：http://bsr.jyoumei.cn

int a = 10; printf("%d\n", a);
来源：http://omw.iojbl.cn

[S03] C：读入整数
来源：http://dlb.gotoacloud.top

int x; scanf("%d", &x);
来源：http://okw.jqgfzy.top

[S04] C：字符串复制
来源：http://zbk.cucudq.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ygj.chenzaomai.com

[S05] C：字符串长度
来源：http://ptr.daxiang520.top

strlen(s)
来源：http://wbt.dashuyun.cn

[S06] C：字符串比较
来源：http://wrb.vqdsnc.cn

strcmp(a, b) == 0
来源：http://yta.tanke756.top

[S07] C：数组遍历求和
来源：http://ibm.cucudq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kdu.kuanghao11.cn

[S08] C：动态内存分配与释放
来源：http://hmz.jianghu66.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oau.zhiwuduotai.top

[S09] C：结构体定义与初始化
来源：http://bpn.xuetiantiany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hha.xuanzx.com

[S10] C：指针与解引用
来源：http://xap.tianlin.xyz

int *p = &a;  *p = 5;
来源：http://gxq.mhx1999.top

[S11] C：逐行读文件
来源：http://jct.shzxlz.cn

FILE *f = fopen("a.txt", "r");
来源：http://odi.fktsv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fde.redwolf501.top

fclose(f);
来源：http://cqb.wangdashe.top

[S12] C：写文件
来源：http://kmf.fzhhl.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xsx.gaohongyu789.top

[S13] C：宏定义
来源：http://avx.zycfv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uvk.redwolf501.top

[S14] C：枚举
来源：http://bii.meibo888.top

enum Color { RED, GREEN, BLUE };
来源：http://htx.nanxinkj.top

[S15] C：类型转换
来源：http://gok.jinyuanbaomall.cn

(double) a / b
来源：http://zib.ivvv.top

[S16] C：位操作置位
来源：http://nvf.redwolf501.top

x |= (1 << 3);
来源：http://fqg.gotoacloud.top

[S17] C：安全拼接字符串
来源：http://ups.sufxvd.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lxa.hongshengwenyu.top

[S18] C：命令行参数
来源：http://zlp.birdmap.top

int main(int argc, char **argv)
来源：http://neb.cheryme.top

[S19] C：快速排序
来源：http://kkj.zhaomingkeji.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://rdr.shzxlz.cn

[S20] C：二分查找
来源：http://wln.snrcjt.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mkq.hysaishi.cn

[S21] C：字符类别判断
来源：http://low.zdbjq.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://unc.chenzaomai.com

[S22] C：字符串转数字
来源：http://nhi.zdqjudy.top

atoi("42");  strtod("3.14", NULL);
来源：http://qwx.meibo888.top

[S23] C：随机数
来源：http://vjc.smart0.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://rzx.sweek.top

[S24] C：获取本地时间
来源：http://ndf.xziqi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zky.yj202588.top

[S25] C：内存拷贝
来源：http://auz.fzhhl.top

memcpy(dst, src, n);
来源：http://puj.jyoumei.cn

[S26] C：内存清零
来源：http://oum.ydzc1.top

memset(a, 0, sizeof a);
来源：http://dbs.shuidangran.top

[S27] C：定义常量
来源：http://fpk.redwolf501.top

const double PI = 3.14159;
来源：http://mgx.jinqigfzy.top

[S28] C：静态变量
来源：http://qrq.yfazqb.com

static int counter = 0;
来源：http://hov.redwolf501.top

[S29] C：变参函数
来源：http://xoe.gzhubu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nqj.haohaochexian.top

[S30] C：头文件保护
来源：http://pwy.zdqjudy.top

#ifndef X_H
来源：http://ceq.zhixingplan.top

#define X_H
来源：http://lvx.redwolf501.top

#endif
来源：http://ucw.ydjk.org.cn

[S31] C++：Hello World
来源：http://ngt.shzxlz.cn

#include <iostream>
来源：http://lrp.yanxiufei.cn

int main() { std::cout << "Hello\n"; }
来源：http://xms.pengpengdd.cyou

[S32] C++：字符串
来源：http://ock.hywenlv.cn

std::string s = "hi";  s += "!";
来源：http://wid.xinyue.icu

[S33] C++：vector 增删
来源：http://hbc.hongshengwenyu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://puj.jinyuanbaomall.cn

[S34] C++：遍历 vector
来源：http://fee.fzhhl.top

for (auto &x : v) { std::cout << x; }
来源：http://bny.wangshuangyany.cn

[S35] C++：map
来源：http://tby.jlsjyb.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://icq.yuanzhike.top

[S36] C++：unordered_map
来源：http://pwq.ivvv.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ppi.smart0.xyz

[S37] C++：set
来源：http://nra.hysaishi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ezx.cdnleiting.top

[S38] C++：排序
来源：http://ioe.birdmap.top

std::sort(v.begin(), v.end());
来源：http://yxj.yonumen.top

[S39] C++：自定义比较器排序
来源：http://ilh.nwbrower.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://htm.shanyushiyangkeji.top

[S40] C++：查找元素
来源：http://izw.shanyushiyangtech.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ata.vqdsnc.cn

[S41] C++：类与构造函数
来源：http://txb.yanxiufei.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cjb.hfpthk.cn

[S42] C++：继承与虚函数
来源：http://kso.zhengqikj.top

class B : public Base { public: void f() override {} };
来源：http://vii.shangyingyoupin.top

[S43] C++：智能指针
来源：http://xmv.pycfn.com

auto p = std::make_unique<int>(5);
来源：http://uln.ywan-chungtsiang.top

[S44] C++：引用传参
来源：http://hai.feifeiyinyue.top

void inc(int &x) { ++x; }
来源：http://xit.xingfuxueyuan.xyz

[S45] C++：lambda
来源：http://xcb.ydjk.org.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zxn.daxiang520.top

[S46] C++：函数模板
来源：http://eof.sjlbkw.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qjg.fanxiaobao.xyz

[S47] C++：结构化绑定遍历
来源：http://bpt.zhoulong.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bzr.xuanzx.com

[S48] C++：逐行读文件
来源：http://fut.wangdashe.top

std::ifstream in("a.txt");  std::string line;
来源：http://zmw.ydzc1.top

while (std::getline(in, line)) { }
来源：http://eby.hysaishi.cn

[S49] C++：写文件
来源：http://dkv.gzhubu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jjk.uphjek.com

[S50] C++：格式化数字
来源：http://quz.cucudq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fcw.ydzc1.top

[S51] C++：显式类型转换
来源：http://taj.tarul.cn

static_cast<double>(a) / b
来源：http://pqp.bjfxy.top

[S52] C++：const 与 noexcept
来源：http://wmw.svipenyu.cn

int size() const noexcept { return n_; }
来源：http://nic.quarkkingdee.top

[S53] C++：移动语义
来源：http://gco.xziqi.cn

std::vector<int> w = std::move(v);
来源：http://nue.aizwys.cn

[S54] C++：异常处理
来源：http://ira.nanxuanxn.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qrm.uphjek.com

[S55] C++：结构化绑定
来源：http://ivk.epnwcf.com

auto [a, b] = std::make_pair(1, 2);
来源：http://tsv.jyoumei.cn

[S56] C++：optional
来源：http://std.zhiwuduotai.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ocb.ydzc1.top

[S57] C++：编译期常量
来源：http://bpk.sjlbkw.cn

constexpr int N = 10;
来源：http://dom.52xcode.cn

[S58] C++：命名空间
来源：http://onc.pycfn.com

namespace ns { int f() { return 1; } }
来源：http://uvm.daxiang520.top

[S59] C++：静态断言
来源：http://fwi.ivvv.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fvd.bbcook.cn

[S60] C++：遍历并删除元素
来源：http://zii.andypj.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nia.zhongyouzk.top

================================================================================
来源：http://ows.zdbjq.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://imw.quarkkingdee.top

================================================================================
来源：http://pza.zdqjudy.top

[T01] Kotlin：Hello World
来源：http://sju.sjlbkw.cn

println("Hello")
来源：http://jmu.52xcode.cn

[T02] Kotlin：变量
来源：http://umr.yuxming.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lpc.yj202588.top

[T03] Kotlin：字符串模板
来源：http://cse.hfpthk.cn

"值: $b"
来源：http://umg.daxiang520.top

[T04] Kotlin：空安全
来源：http://emz.chenjidiqi.icu

val n: String? = null;  n?.length
来源：http://vve.jianghu66.top

[T05] Kotlin：when 表达式
来源：http://zau.zhoulong.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ruc.fehbvm.com

[T06] Kotlin：集合映射
来源：http://hiu.bjfxy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://pti.xziqi.cn

[T07] Kotlin：集合过滤
来源：http://xov.jyoumei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ufs.ctjpmb.com

[T08] Kotlin：数据类
来源：http://uqe.zhengqikj.top

data class User(val name: String, val age: Int)
来源：http://gry.hesvh.cn

[T09] Kotlin：扩展函数
来源：http://lge.guannengcc.top

fun String.exclaim() = this + "!"
来源：http://asg.daria6918.cn

[T10] Kotlin：默认参数
来源：http://pzm.dashuyun.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lgv.wangshuangyany.cn

[T11] Kotlin：协程
来源：http://dry.sufxvd.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lqw.ivvv.top

[T12] Kotlin：解构声明
来源：http://hog.yj20258.top

val (a, b) = Pair(1, 2)
来源：http://qqr.jinqigfzy.top

[T13] Kotlin：只读 Map
来源：http://ehx.wangshuangyany.cn

val m = mapOf("a" to 1)
来源：http://kqq.wangshuangyany.cn

[T14] Kotlin：循环
来源：http://fsn.yueranfly.top

for (i in 1..10) println(i)
来源：http://knw.zhongyouzk.top

[T15] Kotlin：接口
来源：http://yuf.daxiang520.top

interface Shape { fun area(): Double }
来源：http://jng.pengpengdd.cyou

[T16] Swift：Hello World
来源：http://qsl.zhongyouzk.top

print("Hello")
来源：http://pjf.feifeiyinyue.top

[T17] Swift：变量与常量
来源：http://aot.fanxiaobao.xyz

var a = 1;  let b = 2
来源：http://auh.dashuyun.cn

[T18] Swift：字符串插值
来源：http://til.hesvh.cn

"值: \(b)"
来源：http://nle.dashuyun.cn

[T19] Swift：可选绑定
来源：http://fvq.sysykeji.top

if let n = opt { print(n) }
来源：http://nvf.hysaishi.cn

[T20] Swift：数组操作
来源：http://hgd.gogol.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gqb.yvedp.cn

[T21] Swift：遍历
来源：http://ixz.zhengqikj.top

for x in a { print(x) }
来源：http://rsy.0kj1m.cn

[T22] Swift：字典
来源：http://ttc.hesvh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hqe.yueranfly.top

[T23] Swift：函数
来源：http://rir.pengpengdd.cyou

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vio.xinyue.icu

[T24] Swift：闭包
来源：http://ode.ydjk.org.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://uuo.guannengcc.top

[T25] Swift：结构体
来源：http://wgn.fktsv.cn

struct P { var x: Int }
来源：http://yfl.jinqigfzy.top

[T26] Swift：类与重写
来源：http://wyc.cashguo.top

class A: Base { override func f() {} }
来源：http://yxy.epnwcf.com

[T27] Swift：错误处理
来源：http://sbw.xuanzx.com

do { try f() } catch { print(error) }
来源：http://avb.tarul.cn

[T28] Swift：枚举
来源：http://sxc.chenzaomai.com

enum Color { case red, green }
来源：http://kjm.zhongyouzk.top


<!-- 参考信息 -->