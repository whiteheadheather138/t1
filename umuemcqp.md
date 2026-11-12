代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hgn.jianghu66.top

[R30] 函数返回状态码
来源：http://dng.cucudq.cn

f() { return 0; }; f || echo "失败了"
来源：http://jmb.0kj1m.cn

[R31] 局部变量
来源：http://lvk.ppjwa.cn

f() { local x=1; echo "$x"; }
来源：http://xsv.hcnkem.com

[R32] 参数个数校验
来源：http://nzg.xingfuxueyuan.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rbe.xinyue.icu

[R33] 捕获错误并提示行号
来源：http://cqs.hammf.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zib.ppjwa.cn

[R34] 退出时清理
来源：http://baj.gotoacloud.top

trap 'rm -f "$tmp"' EXIT
来源：http://xqr.kuanghao11.cn

[R35] 后台执行并等待
来源：http://weg.redwolf501.top

sleep 5 & pid=$!; wait "$pid"
来源：http://hfc.tian-w.cn

[R36] 并发执行多个任务
来源：http://oxh.hammf.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mtj.kuanghao11.cn

[R37] 把输出赋给变量
来源：http://mcx.daria6918.cn

files=$(ls -1)
来源：http://eri.xziqi.cn

[R38] 管道串联
来源：http://owt.gotoacloud.top

cat a.txt | grep -i error | wc -l
来源：http://ldg.andypj.xyz

[R39] 重定向标准输出与错误
来源：http://rtw.ehwqpu.com

cmd > out.log 2>&1
来源：http://uum.fehbvm.com

[R40] 追加写日志
来源：http://rnt.zhongyouzk.top

echo "log" >> out.log
来源：http://pmi.hongshengwenyu.top

[R41] 丢弃输出
来源：http://zea.dianchejie.cn

cmd >/dev/null 2>&1
来源：http://tcf.wangdashe.top

[R42] 输入重定向
来源：http://fkp.c1oappe.top

wc -l < a.txt
来源：http://otu.pengpengdd.cyou

[R43] 按名字查找文件
来源：http://nno.sufxvd.cn

find . -name "*.log" -type f
来源：http://cme.vqdsnc.cn

[R44] 按修改时间查找
来源：http://ymw.fzhhl.top

find . -mtime -7 -type f
来源：http://jzk.yj20258.top

[R45] 批量删除
来源：http://klb.fengsongda.top

find . -name "*.tmp" -delete
来源：http://hld.gzhubu.top

[R46] 递归替换文件内容
来源：http://skx.pengpengdd.cyou

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jcb.jinqigfzy.top

[R47] sed 单行替换
来源：http://yri.cqqwz.cn

sed -i 's/foo/bar/g' a.txt
来源：http://itn.xingfuxueyuan.xyz

[R48] awk 取指定列
来源：http://qfs.gogol.net.cn

awk '{print $1, $3}' a.txt
来源：http://qvz.zhaomingkeji.xyz

[R49] awk 带条件
来源：http://bou.jinghuilouyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rfk.gaohongyu789.top

[R50] awk 求和
来源：http://qah.zdbjq.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cxq.hongshengwenyu.top

[R51] 排序去重取前几
来源：http://tsu.jinghuilouyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xdf.hcnkem.com

[R52] 统计行数
来源：http://sxy.tianlin.xyz

wc -l a.txt
来源：http://pem.wangdashe.top

[R53] 查看文件头与实时尾
来源：http://vzg.gaohongyu789.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://buv.xuanzx.com

[R54] 比较两个文件
来源：http://bpn.xziqi.cn

diff a.txt b.txt
来源：http://qae.jinqigfzy.top

[R55] 压缩与解压
来源：http://srf.yj20258.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tfc.tanke756.top

[R56] 远程拷贝
来源：http://nbf.xuetiantiany.cn

scp file user@host:/path/
来源：http://xrr.tanke756.top

[R57] 远程执行命令
来源：http://bwn.xuetiantiany.cn

ssh user@host 'uptime'
来源：http://vva.c1oappe.top

[R58] 下载文件
来源：http://zmw.sjlbkw.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://knz.xingfuxueyuan.xyz

[R59] 发 POST JSON
来源：http://obb.uphjek.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qqm.cashguo.top

[R60] 只看 HTTP 状态码
来源：http://sav.gogol.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ono.hcnkem.com

[R61] 磁盘占用
来源：http://dzl.ydjk.org.cn

df -h;  du -sh *
来源：http://xzc.chenjidiqi.icu

[R62] 找最占空间的文件
来源：http://gsb.zhongyouzk.top

du -ah . | sort -rh | head -10
来源：http://txg.meibo888.top

[R63] 内存与进程
来源：http://vvr.yvedp.cn

free -h;  ps aux | grep nginx
来源：http://mzz.ctjpmb.com

[R64] 结束进程
来源：http://wbi.pycfn.com

kill -9 $(pgrep -f app.py)
来源：http://vyv.snrcjt.cn

[R65] 查看端口占用
来源：http://mrk.vehdjk.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ifa.xingfuxueyuan.xyz

[R66] 定时任务
来源：http://kzc.haohaochexian.top

crontab -e;  crontab -l
来源：http://tlk.yongpay.top

[R67] 生成随机十六进制串
来源：http://pli.nanxuanxn.top

openssl rand -hex 16
来源：http://grw.xziqi.cn

[R68] 计算文件校验值
来源：http://hnw.wangdashe.top

sha256sum a.txt;  md5sum a.txt
来源：http://tze.dianchejie.cn

[R69] 生成随机密码
来源：http://zrh.zhongyouzk.top

head -c 16 /dev/urandom | base64
来源：http://kal.fzhhl.top

[R70] 时间戳与互转
来源：http://nwo.aizwys.cn

date +%s;  date -d @1700000000
来源：http://lxz.cdnleiting.top

[R71] 日期格式化
来源：http://gdn.fzhhl.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://hmd.fanxiaobao.xyz

[R72] 等待端口就绪
来源：http://jmk.yj20258888.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qrq.zhongyouzk.top

[R73] 分割大日志
来源：http://hma.ydzc1.top

split -l 1000 big.log part_
来源：http://agi.daxiang520.top

[R74] 批量重命名
来源：http://ldj.yj20258888.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xnj.fktsv.cn

[R75] 导出环境变量
来源：http://doe.yj20258.top

export PATH="$HOME/bin:$PATH"
来源：http://xsi.ydjk.org.cn

[R76] 使用临时文件
来源：http://cti.bbcook.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yas.jianghu66.top

[R77] 读取用户输入
来源：http://csl.hnqzz.top

read -rp "请输入: " ans
来源：http://yfk.yanxiufei.cn

[R78] 交互式菜单
来源：http://gsh.316326.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://tcg.zycfv.cn

[R79] 解析命令行选项
来源：http://tcj.hesvh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bcq.shangyingyoupin.top

[R80] 查看脚本执行耗时
来源：http://anl.zhoulong.xyz

time ./run.sh
来源：http://sjg.hysaishi.cn

================================================================================
来源：http://mhp.ybcxt.top

S. C / C++ 专题
来源：http://fjz.fehbvm.com

================================================================================
来源：http://eel.9152youxi.cn

[S01] C：Hello World
来源：http://mwq.yfazqb.com

#include <stdio.h>
来源：http://riz.daria6918.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://twl.hcnkem.com

[S02] C：变量与格式化输出
来源：http://enm.jyoumei.cn

int a = 10; printf("%d\n", a);
来源：http://fda.shanyushiyangtech.top

[S03] C：读入整数
来源：http://dms.pengpengdd.cyou

int x; scanf("%d", &x);
来源：http://lhp.hesvh.cn

[S04] C：字符串复制
来源：http://idy.hongshengwenyu.top

char dst[32]; strcpy(dst, "hi");
来源：http://fkd.xingfuxueyuan.xyz

[S05] C：字符串长度
来源：http://gtt.aizwys.cn

strlen(s)
来源：http://gzy.zdqjudy.top

[S06] C：字符串比较
来源：http://urb.sufxvd.cn

strcmp(a, b) == 0
来源：http://eyo.gaohongyu789.top

[S07] C：数组遍历求和
来源：http://nrz.daria6918.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://psm.chenzaomai.com

[S08] C：动态内存分配与释放
来源：http://dzr.gaohongyu789.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://puu.epnwcf.com

[S09] C：结构体定义与初始化
来源：http://eik.jinghuilouyu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://arv.zdbjq.cn

[S10] C：指针与解引用
来源：http://zun.zhongyouzk.top

int *p = &a;  *p = 5;
来源：http://duj.vehdjk.com

[S11] C：逐行读文件
来源：http://hib.cdnleiting.top

FILE *f = fopen("a.txt", "r");
来源：http://upx.ivvv.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ajk.chenlongwang.top

fclose(f);
来源：http://hyz.tarul.cn

[S12] C：写文件
来源：http://dld.shzxlz.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wfd.xziqi.cn

[S13] C：宏定义
来源：http://lav.ctjpmb.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://thf.shangyingyoupin.top

[S14] C：枚举
来源：http://dpl.jinghuilouyu.cn

enum Color { RED, GREEN, BLUE };
来源：http://qkc.aibaodan.cn

[S15] C：类型转换
来源：http://vlb.sxryk.cn

(double) a / b
来源：http://ggd.9152youxi.cn

[S16] C：位操作置位
来源：http://giz.hnqzz.top

x |= (1 << 3);
来源：http://btg.shuidangran.top

[S17] C：安全拼接字符串
来源：http://wvy.jlsjyb.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sna.hywenlv.cn

[S18] C：命令行参数
来源：http://juu.svipenyu.cn

int main(int argc, char **argv)
来源：http://bdj.guannengcc.top

[S19] C：快速排序
来源：http://xhk.jqgfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://nje.mhx1999.top

[S20] C：二分查找
来源：http://trd.hywenlv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ytc.jinyuanbaomall.cn

[S21] C：字符类别判断
来源：http://tfx.sjlbkw.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ikl.pengpengdd.cyou

[S22] C：字符串转数字
来源：http://iqr.zhiwuduotai.top

atoi("42");  strtod("3.14", NULL);
来源：http://acm.ehwqpu.com

[S23] C：随机数
来源：http://hdn.ctjpmb.com

srand(time(NULL));  int r = rand() % 100;
来源：http://obb.haohaochexian.top

[S24] C：获取本地时间
来源：http://gcc.dashuyun.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xzv.andypj.xyz

[S25] C：内存拷贝
来源：http://vpn.zycfv.cn

memcpy(dst, src, n);
来源：http://yga.yanxiufei.cn

[S26] C：内存清零
来源：http://upx.mhx1999.top

memset(a, 0, sizeof a);
来源：http://ldu.ehwqpu.com

[S27] C：定义常量
来源：http://gdd.andypj.xyz

const double PI = 3.14159;
来源：http://vdn.zhijiandao.cn

[S28] C：静态变量
来源：http://yqo.fktsv.cn

static int counter = 0;
来源：http://byb.zhengqikj.top

[S29] C：变参函数
来源：http://izq.xinyue.icu

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://caj.wangshuangyany.cn

[S30] C：头文件保护
来源：http://xpy.feifeiyinyue.top

#ifndef X_H
来源：http://fiz.xylfe.cn

#define X_H
来源：http://ikw.fanxiaobao.xyz

#endif
来源：http://uov.hnqzz.top

[S31] C++：Hello World
来源：http://ubl.mhx1999.top

#include <iostream>
来源：http://par.yanxiufei.cn

int main() { std::cout << "Hello\n"; }
来源：http://iag.birdmap.top

[S32] C++：字符串
来源：http://jgv.sysykeji.top

std::string s = "hi";  s += "!";
来源：http://djb.epnwcf.com

[S33] C++：vector 增删
来源：http://stc.pycfn.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ttc.yuxming.cn

[S34] C++：遍历 vector
来源：http://sza.yongpay.top

for (auto &x : v) { std::cout << x; }
来源：http://klp.ivvv.top

[S35] C++：map
来源：http://irm.mhx1999.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qvk.sufxvd.cn

[S36] C++：unordered_map
来源：http://vmc.uphjek.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pxy.jlsjyb.cn

[S37] C++：set
来源：http://vut.sysykeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pjt.ppjwa.cn

[S38] C++：排序
来源：http://vyk.aizwys.cn

std::sort(v.begin(), v.end());
来源：http://kuw.sufxvd.cn

[S39] C++：自定义比较器排序
来源：http://uzj.pengpengdd.cyou

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tvb.shanyushiyangtech.top

[S40] C++：查找元素
来源：http://zrs.9152youxi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fed.dashuyun.cn

[S41] C++：类与构造函数
来源：http://yrs.yj20258888.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dic.shzxlz.cn

[S42] C++：继承与虚函数
来源：http://dtq.chenlongwang.top

class B : public Base { public: void f() override {} };
来源：http://fjh.yanxiufei.cn

[S43] C++：智能指针
来源：http://oii.sxryk.cn

auto p = std::make_unique<int>(5);
来源：http://nhn.xziqi.cn

[S44] C++：引用传参
来源：http://nle.chenzaomai.com

void inc(int &x) { ++x; }
来源：http://uwg.yuanzhike.top

[S45] C++：lambda
来源：http://qym.jinqigfzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://zwp.52xcode.cn

[S46] C++：函数模板
来源：http://nmo.jiagoushi.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://usl.nanxinkj.top

[S47] C++：结构化绑定遍历
来源：http://zgj.cdnleiting.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://euh.jianghu66.top

[S48] C++：逐行读文件
来源：http://iyj.yongpay.top

std::ifstream in("a.txt");  std::string line;
来源：http://aaa.nanxuanxn.top

while (std::getline(in, line)) { }
来源：http://uln.guowangkeji.top

[S49] C++：写文件
来源：http://foq.xingfuxueyuan.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://irs.shanyushiyangkeji.top

[S50] C++：格式化数字
来源：http://fub.aibaodan.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dby.yanxiufei.cn

[S51] C++：显式类型转换
来源：http://lcf.iojbl.cn

static_cast<double>(a) / b
来源：http://tqw.fengsongda.top

[S52] C++：const 与 noexcept
来源：http://aet.wangshuangyany.cn

int size() const noexcept { return n_; }
来源：http://dul.hongshengwenyu.top

[S53] C++：移动语义
来源：http://mxb.xinyue.icu

std::vector<int> w = std::move(v);
来源：http://blh.kuanghao11.cn

[S54] C++：异常处理
来源：http://vca.zdqjudy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://arw.chenlongwang.top

[S55] C++：结构化绑定
来源：http://ekh.hysaishi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cnq.fengsongda.top

[S56] C++：optional
来源：http://ulw.zhaomingkeji.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lsq.bjfxy.top

[S57] C++：编译期常量
来源：http://bbu.yj202588.top

constexpr int N = 10;
来源：http://qxb.nanxinkj.top

[S58] C++：命名空间
来源：http://pqk.feifeiyinyue.top

namespace ns { int f() { return 1; } }
来源：http://wgg.daria6918.cn

[S59] C++：静态断言
来源：http://sah.yj202588.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qot.zhaomingkeji.xyz

[S60] C++：遍历并删除元素
来源：http://lxc.ehwqpu.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ghu.feifeiyinyue.top

================================================================================
来源：http://uiw.jyoumei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eql.sufxvd.cn

================================================================================
来源：http://bxr.gotoacloud.top

[T01] Kotlin：Hello World
来源：http://mit.gogol.net.cn

println("Hello")
来源：http://kov.jiagoushi.top

[T02] Kotlin：变量
来源：http://tym.sjlbkw.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pdd.tianlin.xyz

[T03] Kotlin：字符串模板
来源：http://idc.chenjidiqi.icu

"值: $b"
来源：http://rdu.zhongyouzk.top

[T04] Kotlin：空安全
来源：http://wer.chenjidiqi.icu

val n: String? = null;  n?.length
来源：http://tku.mhx1999.top

[T05] Kotlin：when 表达式
来源：http://mxv.9152youxi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gtv.ywan-chungtsiang.top

[T06] Kotlin：集合映射
来源：http://gja.jinqigufen.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jwj.316326.xyz

[T07] Kotlin：集合过滤
来源：http://eox.9152youxi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://sfh.zhiwuduotai.top

[T08] Kotlin：数据类
来源：http://qzp.jinqigfzy.top

data class User(val name: String, val age: Int)
来源：http://ipv.haohaochexian.top

[T09] Kotlin：扩展函数
来源：http://jqx.jianghu66.top

fun String.exclaim() = this + "!"
来源：http://qbu.gotoacloud.top

[T10] Kotlin：默认参数
来源：http://wez.aizwys.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mai.0kj1m.cn

[T11] Kotlin：协程
来源：http://pgt.sysykeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://chg.sysykeji.top

[T12] Kotlin：解构声明
来源：http://jzf.yj20258888.top

val (a, b) = Pair(1, 2)
来源：http://spt.vqdsnc.cn

[T13] Kotlin：只读 Map
来源：http://npq.hfpthk.cn

val m = mapOf("a" to 1)
来源：http://pcq.hywenlv.cn

[T14] Kotlin：循环
来源：http://who.bbcook.cn

for (i in 1..10) println(i)
来源：http://hrl.52xcode.cn

[T15] Kotlin：接口
来源：http://xtm.sxryk.cn

interface Shape { fun area(): Double }
来源：http://tuo.xuanzx.com

[T16] Swift：Hello World
来源：http://jvy.andypj.xyz

print("Hello")
来源：http://nvb.iojbl.cn

[T17] Swift：变量与常量
来源：http://bht.yj202588.top

var a = 1;  let b = 2
来源：http://jzc.ywan-chungtsiang.top

[T18] Swift：字符串插值
来源：http://alj.aibaodan.cn

"值: \(b)"
来源：http://prw.jinqigfzy.top

[T19] Swift：可选绑定
来源：http://vom.yanxiufei.cn

if let n = opt { print(n) }
来源：http://ymp.zhongyouzk.top

[T20] Swift：数组操作
来源：http://krh.sxryk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://deb.hcnkem.com

[T21] Swift：遍历
来源：http://pxu.xinyue.icu

for x in a { print(x) }
来源：http://uwa.andypj.xyz

[T22] Swift：字典
来源：http://jcj.cashguo.top

var d = ["a": 1];  d["b"] = 2
来源：http://jbp.bjfxy.top

[T23] Swift：函数
来源：http://iic.0kj1m.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pee.hywenlv.cn

[T24] Swift：闭包
来源：http://xin.svipenyu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rqy.c1oappe.top

[T25] Swift：结构体
来源：http://pre.mhx1999.top

struct P { var x: Int }
来源：http://lbd.fehbvm.com

[T26] Swift：类与重写
来源：http://fod.zhiwuduotai.top

class A: Base { override func f() {} }
来源：http://wwp.fzhhl.top

[T27] Swift：错误处理
来源：http://ocn.ydzc1.top

do { try f() } catch { print(error) }
来源：http://kil.shuidangran.top

[T28] Swift：枚举
来源：http://ocl.guannengcc.top

enum Color { case red, green }
来源：http://hwz.ppjwa.cn

[T29] Swift：guard 提前返回
来源：http://bos.uphjek.com

guard let x = opt else { return }
来源：http://pys.hnqzz.top

[T30] Swift：协议
来源：http://nit.jinyuanbaomall.cn

protocol Shape { func area() -> Double }
来源：http://xss.haohaochexian.top

[T31] Lua：Hello World
来源：http://yuc.yj20258888.top

print("Hello")
来源：http://hqb.wangshuangyany.cn

[T32] Lua：局部变量
来源：http://rkj.guannengcc.top

local a = 1
来源：http://bjm.jinqigfzy.top


<!-- 参考信息 -->