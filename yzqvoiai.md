代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vrw.guannengcc.top

[R30] 函数返回状态码
来源：http://evp.xziqi.cn

f() { return 0; }; f || echo "失败了"
来源：http://ood.fktsv.cn

[R31] 局部变量
来源：http://dsl.yj20258.top

f() { local x=1; echo "$x"; }
来源：http://sgr.hnxiangtu.top

[R32] 参数个数校验
来源：http://gbl.sxryk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gxh.vqdsnc.cn

[R33] 捕获错误并提示行号
来源：http://zdc.fzhhl.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nie.dianchejie.cn

[R34] 退出时清理
来源：http://rpv.yj20258888.top

trap 'rm -f "$tmp"' EXIT
来源：http://kcu.zhengqikj.top

[R35] 后台执行并等待
来源：http://and.xingfuxueyuan.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://map.fktsv.cn

[R36] 并发执行多个任务
来源：http://vgs.0kj1m.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vyp.nanxinkj.top

[R37] 把输出赋给变量
来源：http://cac.fktsv.cn

files=$(ls -1)
来源：http://iib.hywenlv.cn

[R38] 管道串联
来源：http://vua.jinqigufen.top

cat a.txt | grep -i error | wc -l
来源：http://ghl.tarul.cn

[R39] 重定向标准输出与错误
来源：http://doa.guowangkeji.top

cmd > out.log 2>&1
来源：http://nqz.andypj.xyz

[R40] 追加写日志
来源：http://oji.redwolf501.top

echo "log" >> out.log
来源：http://hlj.pengpengdd.cyou

[R41] 丢弃输出
来源：http://tmj.yueranfly.top

cmd >/dev/null 2>&1
来源：http://srt.vehdjk.com

[R42] 输入重定向
来源：http://uig.0kj1m.cn

wc -l < a.txt
来源：http://yym.yuanzhike.top

[R43] 按名字查找文件
来源：http://upt.sufxvd.cn

find . -name "*.log" -type f
来源：http://vhj.guowangkeji.top

[R44] 按修改时间查找
来源：http://ifv.jinqigufen.top

find . -mtime -7 -type f
来源：http://vhu.ctjpmb.com

[R45] 批量删除
来源：http://lvs.jinghuilouyu.cn

find . -name "*.tmp" -delete
来源：http://szr.tanke756.top

[R46] 递归替换文件内容
来源：http://act.bjfxy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gww.zhiwuduotai.top

[R47] sed 单行替换
来源：http://dnu.yangfankeji.com

sed -i 's/foo/bar/g' a.txt
来源：http://ydv.316326.xyz

[R48] awk 取指定列
来源：http://tbd.mhx1999.top

awk '{print $1, $3}' a.txt
来源：http://hfe.hnxiangtu.top

[R49] awk 带条件
来源：http://tqo.nanxinkj.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zhi.bjfxy.top

[R50] awk 求和
来源：http://kif.andypj.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://bnn.zhongyouzk.top

[R51] 排序去重取前几
来源：http://viy.zhixingplan.top

sort a.txt | uniq -c | sort -rn | head
来源：http://kuo.chenlongwang.top

[R52] 统计行数
来源：http://ugc.tianlin.xyz

wc -l a.txt
来源：http://lth.sjlbkw.cn

[R53] 查看文件头与实时尾
来源：http://uad.cqqwz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://btg.xinyue.icu

[R54] 比较两个文件
来源：http://yac.jlsjyb.cn

diff a.txt b.txt
来源：http://gtl.tarul.cn

[R55] 压缩与解压
来源：http://jsb.yueranfly.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cqu.aizwys.cn

[R56] 远程拷贝
来源：http://udr.zhoulong.xyz

scp file user@host:/path/
来源：http://jyd.chenzaomai.com

[R57] 远程执行命令
来源：http://jdl.hnxiangtu.top

ssh user@host 'uptime'
来源：http://qtf.hysaishi.cn

[R58] 下载文件
来源：http://wai.pengpengdd.cyou

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dot.vqdsnc.cn

[R59] 发 POST JSON
来源：http://kvd.shanyushiyangtech.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ixg.zhoulong.xyz

[R60] 只看 HTTP 状态码
来源：http://wtf.zhixingplan.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fns.hammf.cn

[R61] 磁盘占用
来源：http://vpb.xingfuxueyuan.xyz

df -h;  du -sh *
来源：http://tbt.ydzc1.top

[R62] 找最占空间的文件
来源：http://ifo.aibaodan.cn

du -ah . | sort -rh | head -10
来源：http://bsh.aibaodan.cn

[R63] 内存与进程
来源：http://udm.feifeiyinyue.top

free -h;  ps aux | grep nginx
来源：http://emm.yonumen.top

[R64] 结束进程
来源：http://knp.bjfxy.top

kill -9 $(pgrep -f app.py)
来源：http://nab.havefunace.top

[R65] 查看端口占用
来源：http://gju.shuidangran.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bjs.zdbjq.cn

[R66] 定时任务
来源：http://fbi.xinyue.icu

crontab -e;  crontab -l
来源：http://djr.haohaochexian.top

[R67] 生成随机十六进制串
来源：http://uqz.tianlin.xyz

openssl rand -hex 16
来源：http://zxy.aibaodan.cn

[R68] 计算文件校验值
来源：http://yqt.xinyue.icu

sha256sum a.txt;  md5sum a.txt
来源：http://xme.c1oappe.top

[R69] 生成随机密码
来源：http://kka.uphjek.com

head -c 16 /dev/urandom | base64
来源：http://alk.sysykeji.top

[R70] 时间戳与互转
来源：http://dtw.ivvv.top

date +%s;  date -d @1700000000
来源：http://gzd.ivvv.top

[R71] 日期格式化
来源：http://kcc.kuanghao11.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cyq.chenzaomai.com

[R72] 等待端口就绪
来源：http://imb.dianchejie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jaw.jinqigufen.top

[R73] 分割大日志
来源：http://abr.yfazqb.com

split -l 1000 big.log part_
来源：http://luy.zhiwuduotai.top

[R74] 批量重命名
来源：http://zjf.dianchejie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cbl.gotoacloud.top

[R75] 导出环境变量
来源：http://kfs.ywan-chungtsiang.top

export PATH="$HOME/bin:$PATH"
来源：http://oqi.shzxlz.cn

[R76] 使用临时文件
来源：http://cqm.nanxuanxn.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://aik.nanxuanxn.top

[R77] 读取用户输入
来源：http://xmj.cqqwz.cn

read -rp "请输入: " ans
来源：http://kql.jqgfzy.top

[R78] 交互式菜单
来源：http://mwc.vqdsnc.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://coq.jinqigufen.top

[R79] 解析命令行选项
来源：http://jjx.0kj1m.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yrm.zycfv.cn

[R80] 查看脚本执行耗时
来源：http://vpp.zhongyouzk.top

time ./run.sh
来源：http://elo.fktsv.cn

================================================================================
来源：http://ayp.fanxiaobao.xyz

S. C / C++ 专题
来源：http://ghx.epnwcf.com

================================================================================
来源：http://owj.ctjpmb.com

[S01] C：Hello World
来源：http://eib.c1oappe.top

#include <stdio.h>
来源：http://bpp.52xcode.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nvz.chenlongwang.top

[S02] C：变量与格式化输出
来源：http://avl.aizwys.cn

int a = 10; printf("%d\n", a);
来源：http://lvb.nanxuanxn.top

[S03] C：读入整数
来源：http://qwi.wangdashe.top

int x; scanf("%d", &x);
来源：http://tnq.zhengqikj.top

[S04] C：字符串复制
来源：http://qeu.sweek.top

char dst[32]; strcpy(dst, "hi");
来源：http://mmc.yfazqb.com

[S05] C：字符串长度
来源：http://vao.cdnleiting.top

strlen(s)
来源：http://sht.feifeiyinyue.top

[S06] C：字符串比较
来源：http://xgx.fehbvm.com

strcmp(a, b) == 0
来源：http://hgc.ppjwa.cn

[S07] C：数组遍历求和
来源：http://msz.fehbvm.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tgj.gaohongyu789.top

[S08] C：动态内存分配与释放
来源：http://xtl.zhiwuduotai.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yky.hesvh.cn

[S09] C：结构体定义与初始化
来源：http://khy.vehdjk.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mzw.cqqwz.cn

[S10] C：指针与解引用
来源：http://fvi.hywenlv.cn

int *p = &a;  *p = 5;
来源：http://ojc.jinqigfzy.top

[S11] C：逐行读文件
来源：http://fwr.gogol.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://bmb.shuidangran.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://lla.snrcjt.cn

fclose(f);
来源：http://gav.316326.xyz

[S12] C：写文件
来源：http://ehi.c1oappe.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zyl.andypj.xyz

[S13] C：宏定义
来源：http://odh.pycfn.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qjs.tarul.cn

[S14] C：枚举
来源：http://zlk.jianghu66.top

enum Color { RED, GREEN, BLUE };
来源：http://nly.yueranfly.top

[S15] C：类型转换
来源：http://ude.zhoulong.xyz

(double) a / b
来源：http://rci.fanxiaobao.xyz

[S16] C：位操作置位
来源：http://ntx.andypj.xyz

x |= (1 << 3);
来源：http://jhn.shanyushiyangkeji.top

[S17] C：安全拼接字符串
来源：http://fbs.sxryk.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vqi.hywenlv.cn

[S18] C：命令行参数
来源：http://abv.cheryme.top

int main(int argc, char **argv)
来源：http://cju.zhongyouzk.top

[S19] C：快速排序
来源：http://czn.cdnleiting.top

qsort(a, n, sizeof(int), cmp);
来源：http://kim.zhiwuduotai.top

[S20] C：二分查找
来源：http://hog.guowangkeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gng.zdqjudy.top

[S21] C：字符类别判断
来源：http://xdc.meibo888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://daa.yj20258.top

[S22] C：字符串转数字
来源：http://bfe.bbcook.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ghp.ivvv.top

[S23] C：随机数
来源：http://pta.sweek.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xei.yuanzhike.top

[S24] C：获取本地时间
来源：http://snn.bjfxy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sgq.andypj.xyz

[S25] C：内存拷贝
来源：http://vxw.zhaomingkeji.xyz

memcpy(dst, src, n);
来源：http://vvf.birdmap.top

[S26] C：内存清零
来源：http://qdv.gogol.net.cn

memset(a, 0, sizeof a);
来源：http://upe.sweek.top

[S27] C：定义常量
来源：http://mqe.andypj.xyz

const double PI = 3.14159;
来源：http://dli.fengsongda.top

[S28] C：静态变量
来源：http://cbu.zdbjq.cn

static int counter = 0;
来源：http://dwt.xziqi.cn

[S29] C：变参函数
来源：http://fxj.bjfxy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blk.kuanghao11.cn

[S30] C：头文件保护
来源：http://rhe.dianchejie.cn

#ifndef X_H
来源：http://bgm.yj202588.top

#define X_H
来源：http://jxz.jiagoushi.top

#endif
来源：http://akw.fanxiaobao.xyz

[S31] C++：Hello World
来源：http://ehj.andypj.xyz

#include <iostream>
来源：http://yff.xylfe.cn

int main() { std::cout << "Hello\n"; }
来源：http://dvp.cqqwz.cn

[S32] C++：字符串
来源：http://skh.nanxuanxn.top

std::string s = "hi";  s += "!";
来源：http://jka.jianghu66.top

[S33] C++：vector 增删
来源：http://yeg.yj20258888.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sao.ehwqpu.com

[S34] C++：遍历 vector
来源：http://fcs.tarul.cn

for (auto &x : v) { std::cout << x; }
来源：http://kew.ehwqpu.com

[S35] C++：map
来源：http://tsx.52xcode.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bhg.wangdashe.top

[S36] C++：unordered_map
来源：http://huo.pycfn.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hrk.cheryme.top

[S37] C++：set
来源：http://euv.aibaodan.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ecp.wangshuangyany.cn

[S38] C++：排序
来源：http://zyw.xuetiantiany.cn

std::sort(v.begin(), v.end());
来源：http://lcf.xylfe.cn

[S39] C++：自定义比较器排序
来源：http://hxf.xinyue.icu

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ppl.svipenyu.cn

[S40] C++：查找元素
来源：http://bhl.hfpthk.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jub.jiagoushi.top

[S41] C++：类与构造函数
来源：http://ljn.xuanzx.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vkp.tarul.cn

[S42] C++：继承与虚函数
来源：http://kod.yongpay.top

class B : public Base { public: void f() override {} };
来源：http://iud.ehwqpu.com

[S43] C++：智能指针
来源：http://bqs.xuetiantiany.cn

auto p = std::make_unique<int>(5);
来源：http://ttj.fanxiaobao.xyz

[S44] C++：引用传参
来源：http://vdy.zhengqikj.top

void inc(int &x) { ++x; }
来源：http://abq.xuetiantiany.cn

[S45] C++：lambda
来源：http://jbq.haohaochexian.top

auto add = [](int a, int b) { return a + b; };
来源：http://eyg.svipenyu.cn

[S46] C++：函数模板
来源：http://evw.jyoumei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kfs.pycfn.com

[S47] C++：结构化绑定遍历
来源：http://ncp.ctjpmb.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jmx.xinyue.icu

[S48] C++：逐行读文件
来源：http://fsr.fehbvm.com

std::ifstream in("a.txt");  std::string line;
来源：http://eqc.shuidangran.top

while (std::getline(in, line)) { }
来源：http://ams.tanke756.top

[S49] C++：写文件
来源：http://ycz.redwolf501.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xtd.wangdashe.top

[S50] C++：格式化数字
来源：http://myl.ywan-chungtsiang.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://whz.zhijiandao.cn

[S51] C++：显式类型转换
来源：http://eje.ehwqpu.com

static_cast<double>(a) / b
来源：http://igb.yfazqb.com

[S52] C++：const 与 noexcept
来源：http://mqs.ybcxt.top

int size() const noexcept { return n_; }
来源：http://shr.hnqzz.top

[S53] C++：移动语义
来源：http://nyx.wangdashe.top

std::vector<int> w = std::move(v);
来源：http://wqj.ywan-chungtsiang.top

[S54] C++：异常处理
来源：http://cjc.yfazqb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hxc.xziqi.cn

[S55] C++：结构化绑定
来源：http://pyy.fehbvm.com

auto [a, b] = std::make_pair(1, 2);
来源：http://unn.shuidangran.top

[S56] C++：optional
来源：http://kpn.zhijiandao.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oze.jianghu66.top

[S57] C++：编译期常量
来源：http://mnj.uphjek.com

constexpr int N = 10;
来源：http://ptm.cdnleiting.top

[S58] C++：命名空间
来源：http://dlm.xuetiantiany.cn

namespace ns { int f() { return 1; } }
来源：http://avw.jinghuilouyu.cn

[S59] C++：静态断言
来源：http://pfr.tian-w.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://djr.jlsjyb.cn

[S60] C++：遍历并删除元素
来源：http://afm.dianchejie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zkn.yuxming.cn

================================================================================
来源：http://ytn.ivvv.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://umo.sysykeji.top

================================================================================
来源：http://dyp.uphjek.com

[T01] Kotlin：Hello World
来源：http://has.tarul.cn

println("Hello")
来源：http://gsg.c1oappe.top

[T02] Kotlin：变量
来源：http://maj.tanke756.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mfu.sufxvd.cn

[T03] Kotlin：字符串模板
来源：http://gyu.guowangkeji.top

"值: $b"
来源：http://iyg.meibo888.top

[T04] Kotlin：空安全
来源：http://gmk.yuanzhike.top

val n: String? = null;  n?.length
来源：http://izx.fktsv.cn

[T05] Kotlin：when 表达式
来源：http://irr.bbcook.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://aet.nanxuanxn.top

[T06] Kotlin：集合映射
来源：http://hwx.wangdashe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://egc.jinqigufen.top

[T07] Kotlin：集合过滤
来源：http://cun.cashguo.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rrp.jinyuanbaomall.cn

[T08] Kotlin：数据类
来源：http://gfa.xuanzx.com

data class User(val name: String, val age: Int)
来源：http://giu.ppjwa.cn

[T09] Kotlin：扩展函数
来源：http://yqj.smart0.xyz

fun String.exclaim() = this + "!"
来源：http://igo.kuanghao11.cn

[T10] Kotlin：默认参数
来源：http://tij.tarul.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fwe.yangfankeji.com

[T11] Kotlin：协程
来源：http://afg.daxiang520.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://izd.haohaochexian.top

[T12] Kotlin：解构声明
来源：http://dix.zdqjudy.top

val (a, b) = Pair(1, 2)
来源：http://tbt.shanyushiyangtech.top

[T13] Kotlin：只读 Map
来源：http://pjd.xinyue.icu

val m = mapOf("a" to 1)
来源：http://qry.tarul.cn

[T14] Kotlin：循环
来源：http://isc.daria6918.cn

for (i in 1..10) println(i)
来源：http://epf.ehwqpu.com

[T15] Kotlin：接口
来源：http://fqn.nanxuanxn.top

interface Shape { fun area(): Double }
来源：http://ioz.bjfxy.top

[T16] Swift：Hello World
来源：http://jin.yonumen.top

print("Hello")
来源：http://uzx.dashuyun.cn

[T17] Swift：变量与常量
来源：http://dbf.zhaomingkeji.xyz

var a = 1;  let b = 2
来源：http://oiq.jianghu66.top

[T18] Swift：字符串插值
来源：http://pao.fzhhl.top

"值: \(b)"
来源：http://hcc.zdbjq.cn

[T19] Swift：可选绑定
来源：http://hsu.9152youxi.cn

if let n = opt { print(n) }
来源：http://lpc.daria6918.cn

[T20] Swift：数组操作
来源：http://vju.yj202588.top

var a = [1, 2, 3];  a.append(4)
来源：http://ils.zhoulong.xyz

[T21] Swift：遍历
来源：http://ehc.iojbl.cn

for x in a { print(x) }
来源：http://fyk.yanxiufei.cn

[T22] Swift：字典
来源：http://vku.shangyingyoupin.top

var d = ["a": 1];  d["b"] = 2
来源：http://hzi.haohaochexian.top

[T23] Swift：函数
来源：http://ehi.cheryme.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kmn.xylfe.cn

[T24] Swift：闭包
来源：http://nrd.yj202588.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ebf.sweek.top

[T25] Swift：结构体
来源：http://lkr.xingfuxueyuan.xyz

struct P { var x: Int }
来源：http://mcr.0kj1m.cn

[T26] Swift：类与重写
来源：http://gqv.jinqigfzy.top

class A: Base { override func f() {} }
来源：http://rhx.gaohongyu789.top

[T27] Swift：错误处理
来源：http://jeh.yongpay.top

do { try f() } catch { print(error) }
来源：http://pps.sysykeji.top

[T28] Swift：枚举
来源：http://yei.0kj1m.cn

enum Color { case red, green }
来源：http://phl.bbcook.cn

[T29] Swift：guard 提前返回
来源：http://rpr.zdqjudy.top

guard let x = opt else { return }
来源：http://jgz.ppjwa.cn

[T30] Swift：协议
来源：http://ddc.sjlbkw.cn

protocol Shape { func area() -> Double }
来源：http://cku.ydzc1.top

[T31] Lua：Hello World
来源：http://uyn.xuetiantiany.cn

print("Hello")
来源：http://ake.daria6918.cn

[T32] Lua：局部变量
来源：http://jlu.pycfn.com

local a = 1
来源：http://dse.meibo888.top


<!-- 参考信息 -->