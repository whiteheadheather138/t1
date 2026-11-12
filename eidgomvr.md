代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ney.gotoacloud.top

[R24] 大小写转换
来源：http://hsg.chenlongwang.top

echo "${s^^}"; echo "${s,,}"
来源：http://suf.mhx1999.top

[R25] 去后缀 / 去前缀
来源：http://eio.daxiang520.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ler.zdqjudy.top

[R26] 命令替换
来源：http://brg.quarkkingdee.top

now=$(date +%F); echo "$now"
来源：http://yqk.feifeiyinyue.top

[R27] 算术展开
来源：http://cjs.xuetiantiany.cn

echo $((1 + 2 * 3))
来源：http://mbf.bbcook.cn

[R28] 浮点运算
来源：http://zxi.nwbrower.top

echo "scale=2; 10/3" | bc
来源：http://inj.yongpay.top

[R29] 定义函数
来源：http://hez.gzhubu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bvo.sysykeji.top

[R30] 函数返回状态码
来源：http://bww.jqgfzy.top

f() { return 0; }; f || echo "失败了"
来源：http://rce.hnqzz.top

[R31] 局部变量
来源：http://qwa.cdnleiting.top

f() { local x=1; echo "$x"; }
来源：http://ooe.tarul.cn

[R32] 参数个数校验
来源：http://oge.shangyingyoupin.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hzy.yuxming.cn

[R33] 捕获错误并提示行号
来源：http://xiq.cqqwz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hzz.xinyue.icu

[R34] 退出时清理
来源：http://vby.xingfuxueyuan.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://bfy.yuxming.cn

[R35] 后台执行并等待
来源：http://clm.xuetiantiany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ldi.cqqwz.cn

[R36] 并发执行多个任务
来源：http://jjd.xylfe.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tti.sufxvd.cn

[R37] 把输出赋给变量
来源：http://kxx.9152youxi.cn

files=$(ls -1)
来源：http://abl.gogol.net.cn

[R38] 管道串联
来源：http://rer.jyoumei.cn

cat a.txt | grep -i error | wc -l
来源：http://jbn.meibo888.top

[R39] 重定向标准输出与错误
来源：http://owz.zdqjudy.top

cmd > out.log 2>&1
来源：http://owu.guannengcc.top

[R40] 追加写日志
来源：http://ciu.chenjidiqi.icu

echo "log" >> out.log
来源：http://jue.gzhubu.top

[R41] 丢弃输出
来源：http://sfo.sxryk.cn

cmd >/dev/null 2>&1
来源：http://hrn.yongpay.top

[R42] 输入重定向
来源：http://vkn.hfpthk.cn

wc -l < a.txt
来源：http://ecc.hcnkem.com

[R43] 按名字查找文件
来源：http://ybq.zdbjq.cn

find . -name "*.log" -type f
来源：http://wou.xuetiantiany.cn

[R44] 按修改时间查找
来源：http://tuw.hcnkem.com

find . -mtime -7 -type f
来源：http://cmo.iojbl.cn

[R45] 批量删除
来源：http://ute.chenlongwang.top

find . -name "*.tmp" -delete
来源：http://gfj.jinqigufen.top

[R46] 递归替换文件内容
来源：http://wcp.xziqi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fhm.meibo888.top

[R47] sed 单行替换
来源：http://baq.fanxiaobao.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://mbh.zhengqikj.top

[R48] awk 取指定列
来源：http://vbw.zhoulong.xyz

awk '{print $1, $3}' a.txt
来源：http://trw.quarkkingdee.top

[R49] awk 带条件
来源：http://aka.tianlin.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bmk.shanyushiyangtech.top

[R50] awk 求和
来源：http://yfa.redwolf501.top

awk '{s += $2} END {print s}' a.txt
来源：http://kmy.yj20258.top

[R51] 排序去重取前几
来源：http://aqd.0kj1m.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bwh.guowangkeji.top

[R52] 统计行数
来源：http://ndm.wangshuangyany.cn

wc -l a.txt
来源：http://lme.zdbjq.cn

[R53] 查看文件头与实时尾
来源：http://ham.cqqwz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nvs.yvedp.cn

[R54] 比较两个文件
来源：http://yjo.xziqi.cn

diff a.txt b.txt
来源：http://bne.haohaochexian.top

[R55] 压缩与解压
来源：http://rlr.iojbl.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sld.feifeiyinyue.top

[R56] 远程拷贝
来源：http://fxp.jlsjyb.cn

scp file user@host:/path/
来源：http://ifw.chenzaomai.com

[R57] 远程执行命令
来源：http://zsf.havefunace.top

ssh user@host 'uptime'
来源：http://lna.fktsv.cn

[R58] 下载文件
来源：http://urs.xuanzx.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tts.yj20258888.top

[R59] 发 POST JSON
来源：http://rxl.zhongyouzk.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://iqa.bjfxy.top

[R60] 只看 HTTP 状态码
来源：http://avj.aizwys.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cqr.cheryme.top

[R61] 磁盘占用
来源：http://tdc.zdqjudy.top

df -h;  du -sh *
来源：http://zii.vehdjk.com

[R62] 找最占空间的文件
来源：http://odk.hnqzz.top

du -ah . | sort -rh | head -10
来源：http://waq.dianchejie.cn

[R63] 内存与进程
来源：http://nfl.hywenlv.cn

free -h;  ps aux | grep nginx
来源：http://yof.0kj1m.cn

[R64] 结束进程
来源：http://ckt.gaohongyu789.top

kill -9 $(pgrep -f app.py)
来源：http://pcs.vehdjk.com

[R65] 查看端口占用
来源：http://uap.yj20258888.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yjv.nwbrower.top

[R66] 定时任务
来源：http://wsa.meibo888.top

crontab -e;  crontab -l
来源：http://zip.fanxiaobao.xyz

[R67] 生成随机十六进制串
来源：http://osd.yonumen.top

openssl rand -hex 16
来源：http://mjc.guowangkeji.top

[R68] 计算文件校验值
来源：http://zdo.hongshengwenyu.top

sha256sum a.txt;  md5sum a.txt
来源：http://mgt.tarul.cn

[R69] 生成随机密码
来源：http://eds.jinqigfzy.top

head -c 16 /dev/urandom | base64
来源：http://rmh.yuanzhike.top

[R70] 时间戳与互转
来源：http://wgd.shanyushiyangkeji.top

date +%s;  date -d @1700000000
来源：http://aam.wangdashe.top

[R71] 日期格式化
来源：http://hdm.sjlbkw.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ryh.jlsjyb.cn

[R72] 等待端口就绪
来源：http://xjk.sufxvd.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hij.cucudq.cn

[R73] 分割大日志
来源：http://jjd.uphjek.com

split -l 1000 big.log part_
来源：http://jcc.tarul.cn

[R74] 批量重命名
来源：http://ysn.fzhhl.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ayh.yfazqb.com

[R75] 导出环境变量
来源：http://jzt.chenzaomai.com

export PATH="$HOME/bin:$PATH"
来源：http://rgx.yvedp.cn

[R76] 使用临时文件
来源：http://prv.zhiwuduotai.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://unn.ctjpmb.com

[R77] 读取用户输入
来源：http://hon.0kj1m.cn

read -rp "请输入: " ans
来源：http://ucu.shanyushiyangtech.top

[R78] 交互式菜单
来源：http://qal.hcnkem.com

select opt in a b c; do echo "$opt"; break; done
来源：http://dfm.cqqwz.cn

[R79] 解析命令行选项
来源：http://uhi.hesvh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cuj.zhengqikj.top

[R80] 查看脚本执行耗时
来源：http://tdi.svipenyu.cn

time ./run.sh
来源：http://bny.xinyue.icu

================================================================================
来源：http://uuu.feifeiyinyue.top

S. C / C++ 专题
来源：http://bkg.mhx1999.top

================================================================================
来源：http://tml.hesvh.cn

[S01] C：Hello World
来源：http://cvx.ctjpmb.com

#include <stdio.h>
来源：http://hxv.hywenlv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gxi.pycfn.com

[S02] C：变量与格式化输出
来源：http://vtb.chenjidiqi.icu

int a = 10; printf("%d\n", a);
来源：http://rik.uphjek.com

[S03] C：读入整数
来源：http://aii.guannengcc.top

int x; scanf("%d", &x);
来源：http://sko.cdnleiting.top

[S04] C：字符串复制
来源：http://jzl.ybcxt.top

char dst[32]; strcpy(dst, "hi");
来源：http://oih.cqqwz.cn

[S05] C：字符串长度
来源：http://bln.tian-w.cn

strlen(s)
来源：http://kyv.fktsv.cn

[S06] C：字符串比较
来源：http://lvn.xziqi.cn

strcmp(a, b) == 0
来源：http://psz.zhoulong.xyz

[S07] C：数组遍历求和
来源：http://rnq.shangyingyoupin.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blv.redwolf501.top

[S08] C：动态内存分配与释放
来源：http://ipw.ydjk.org.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hpg.andypj.xyz

[S09] C：结构体定义与初始化
来源：http://tjr.xingfuxueyuan.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mdv.jinghuilouyu.cn

[S10] C：指针与解引用
来源：http://yhw.zhijiandao.cn

int *p = &a;  *p = 5;
来源：http://qbh.hesvh.cn

[S11] C：逐行读文件
来源：http://utb.zhijiandao.cn

FILE *f = fopen("a.txt", "r");
来源：http://vkn.zhijiandao.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zqk.jinghuilouyu.cn

fclose(f);
来源：http://hor.xziqi.cn

[S12] C：写文件
来源：http://zfe.hongshengwenyu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uom.fanxiaobao.xyz

[S13] C：宏定义
来源：http://dyb.zhaomingkeji.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uwz.haohaochexian.top

[S14] C：枚举
来源：http://mdc.hcnkem.com

enum Color { RED, GREEN, BLUE };
来源：http://whg.ywan-chungtsiang.top

[S15] C：类型转换
来源：http://fpb.sjlbkw.cn

(double) a / b
来源：http://ksu.sjlbkw.cn

[S16] C：位操作置位
来源：http://cjl.redwolf501.top

x |= (1 << 3);
来源：http://ryo.xuetiantiany.cn

[S17] C：安全拼接字符串
来源：http://gwc.iojbl.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uws.hesvh.cn

[S18] C：命令行参数
来源：http://uzh.zdbjq.cn

int main(int argc, char **argv)
来源：http://cxz.vqdsnc.cn

[S19] C：快速排序
来源：http://xgu.jlsjyb.cn

qsort(a, n, sizeof(int), cmp);
来源：http://pid.tarul.cn

[S20] C：二分查找
来源：http://ynj.chenlongwang.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qsz.yangfankeji.com

[S21] C：字符类别判断
来源：http://tue.yanxiufei.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bxn.snrcjt.cn

[S22] C：字符串转数字
来源：http://ssi.sysykeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://ocb.hnqzz.top

[S23] C：随机数
来源：http://wki.jlsjyb.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wwp.shzxlz.cn

[S24] C：获取本地时间
来源：http://ufa.c1oappe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://waz.xuanzx.com

[S25] C：内存拷贝
来源：http://mjb.gogol.net.cn

memcpy(dst, src, n);
来源：http://qhj.316326.xyz

[S26] C：内存清零
来源：http://qbg.nwbrower.top

memset(a, 0, sizeof a);
来源：http://pga.jinghuilouyu.cn

[S27] C：定义常量
来源：http://ucd.wangshuangyany.cn

const double PI = 3.14159;
来源：http://apv.daxiang520.top

[S28] C：静态变量
来源：http://zep.nanxinkj.top

static int counter = 0;
来源：http://gsl.gaohongyu789.top

[S29] C：变参函数
来源：http://ogs.wangshuangyany.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://krd.yj20258888.top

[S30] C：头文件保护
来源：http://lsu.vehdjk.com

#ifndef X_H
来源：http://yyj.sufxvd.cn

#define X_H
来源：http://zjs.52xcode.cn

#endif
来源：http://fds.ywan-chungtsiang.top

[S31] C++：Hello World
来源：http://tfo.cucudq.cn

#include <iostream>
来源：http://kkd.vehdjk.com

int main() { std::cout << "Hello\n"; }
来源：http://wxj.hongshengwenyu.top

[S32] C++：字符串
来源：http://zqw.iojbl.cn

std::string s = "hi";  s += "!";
来源：http://syg.hesvh.cn

[S33] C++：vector 增删
来源：http://dgd.shangyingyoupin.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wyu.jinghuilouyu.cn

[S34] C++：遍历 vector
来源：http://urd.dashuyun.cn

for (auto &x : v) { std::cout << x; }
来源：http://wid.cucudq.cn

[S35] C++：map
来源：http://njo.dashuyun.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://upx.zhoulong.xyz

[S36] C++：unordered_map
来源：http://eql.fktsv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://thd.xuanzx.com

[S37] C++：set
来源：http://vvc.smart0.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fca.0kj1m.cn

[S38] C++：排序
来源：http://mrs.fehbvm.com

std::sort(v.begin(), v.end());
来源：http://wls.hammf.cn

[S39] C++：自定义比较器排序
来源：http://oas.jlsjyb.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wlz.jiagoushi.top

[S40] C++：查找元素
来源：http://yaz.mhx1999.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wwv.zdqjudy.top

[S41] C++：类与构造函数
来源：http://qbt.0kj1m.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fuk.ybcxt.top

[S42] C++：继承与虚函数
来源：http://qyy.jinghuilouyu.cn

class B : public Base { public: void f() override {} };
来源：http://vrq.hysaishi.cn

[S43] C++：智能指针
来源：http://yvr.hcnkem.com

auto p = std::make_unique<int>(5);
来源：http://uzh.jinqigufen.top

[S44] C++：引用传参
来源：http://oqo.iojbl.cn

void inc(int &x) { ++x; }
来源：http://hcz.iojbl.cn

[S45] C++：lambda
来源：http://kbu.bbcook.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cqw.yanxiufei.cn

[S46] C++：函数模板
来源：http://wep.andypj.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xpw.zhongyouzk.top

[S47] C++：结构化绑定遍历
来源：http://ebe.shanyushiyangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wei.tianlin.xyz

[S48] C++：逐行读文件
来源：http://oql.ydjk.org.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jmv.gotoacloud.top

while (std::getline(in, line)) { }
来源：http://vuw.0kj1m.cn

[S49] C++：写文件
来源：http://ygn.yj20258.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ncy.ydjk.org.cn

[S50] C++：格式化数字
来源：http://sfe.daria6918.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gtv.gzhubu.top

[S51] C++：显式类型转换
来源：http://llu.shanyushiyangtech.top

static_cast<double>(a) / b
来源：http://xun.yangfankeji.com

[S52] C++：const 与 noexcept
来源：http://vmx.cucudq.cn

int size() const noexcept { return n_; }
来源：http://wan.fengsongda.top

[S53] C++：移动语义
来源：http://atk.shuidangran.top

std::vector<int> w = std::move(v);
来源：http://tub.chenzaomai.com

[S54] C++：异常处理
来源：http://yhn.xinyue.icu

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uxm.yuxming.cn

[S55] C++：结构化绑定
来源：http://fko.aizwys.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pug.yonumen.top

[S56] C++：optional
来源：http://lle.aizwys.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tfs.ydzc1.top

[S57] C++：编译期常量
来源：http://eqz.redwolf501.top

constexpr int N = 10;
来源：http://ini.jinqigfzy.top

[S58] C++：命名空间
来源：http://uvf.gotoacloud.top

namespace ns { int f() { return 1; } }
来源：http://vnj.gotoacloud.top

[S59] C++：静态断言
来源：http://jvq.cqqwz.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qwn.yj20258888.top

[S60] C++：遍历并删除元素
来源：http://qsp.xuetiantiany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tum.fzhhl.top

================================================================================
来源：http://iaw.jlsjyb.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://szq.gaohongyu789.top

================================================================================
来源：http://pos.yj20258888.top

[T01] Kotlin：Hello World
来源：http://kff.ydzc1.top

println("Hello")
来源：http://qbz.chenlongwang.top

[T02] Kotlin：变量
来源：http://tfy.mhx1999.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ngi.chenjidiqi.icu

[T03] Kotlin：字符串模板
来源：http://jqd.jinqigfzy.top

"值: $b"
来源：http://qbf.jlsjyb.cn

[T04] Kotlin：空安全
来源：http://coh.sxryk.cn

val n: String? = null;  n?.length
来源：http://bll.xuanzx.com

[T05] Kotlin：when 表达式
来源：http://puk.jlsjyb.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cdr.vehdjk.com

[T06] Kotlin：集合映射
来源：http://hmx.cheryme.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bgh.jinghuilouyu.cn

[T07] Kotlin：集合过滤
来源：http://nrk.yuanzhike.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://uzm.ehwqpu.com

[T08] Kotlin：数据类
来源：http://xig.yonumen.top

data class User(val name: String, val age: Int)
来源：http://sgu.meibo888.top

[T09] Kotlin：扩展函数
来源：http://ima.hcnkem.com

fun String.exclaim() = this + "!"
来源：http://igv.tanke756.top

[T10] Kotlin：默认参数
来源：http://pic.gaohongyu789.top

fun greet(name: String = "World") = "Hi $name"
来源：http://krp.ivvv.top

[T11] Kotlin：协程
来源：http://hyb.zhongyouzk.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://pew.chenlongwang.top

[T12] Kotlin：解构声明
来源：http://bmh.cqqwz.cn

val (a, b) = Pair(1, 2)
来源：http://ymy.mhx1999.top

[T13] Kotlin：只读 Map
来源：http://nzv.yongpay.top

val m = mapOf("a" to 1)
来源：http://hxr.tanke756.top

[T14] Kotlin：循环
来源：http://mvt.vqdsnc.cn

for (i in 1..10) println(i)
来源：http://sby.nwbrower.top

[T15] Kotlin：接口
来源：http://xqk.cqqwz.cn

interface Shape { fun area(): Double }
来源：http://olq.jianghu66.top

[T16] Swift：Hello World
来源：http://qge.yvedp.cn

print("Hello")
来源：http://fkd.shanyushiyangtech.top

[T17] Swift：变量与常量
来源：http://nuf.zhiwuduotai.top

var a = 1;  let b = 2
来源：http://mma.tanke756.top

[T18] Swift：字符串插值
来源：http://cpq.tarul.cn

"值: \(b)"
来源：http://try.yongpay.top

[T19] Swift：可选绑定
来源：http://tgg.haohaochexian.top

if let n = opt { print(n) }
来源：http://lfl.zhoulong.xyz

[T20] Swift：数组操作
来源：http://rft.jinqigfzy.top

var a = [1, 2, 3];  a.append(4)
来源：http://hbs.jqgfzy.top

[T21] Swift：遍历
来源：http://hre.yuxming.cn

for x in a { print(x) }
来源：http://ixn.jlsjyb.cn

[T22] Swift：字典
来源：http://yht.sysykeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://ryf.haohaochexian.top

[T23] Swift：函数
来源：http://kyk.chenlongwang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dvv.xuetiantiany.cn

[T24] Swift：闭包
来源：http://pfc.haohaochexian.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://hmc.fehbvm.com

[T25] Swift：结构体
来源：http://mbx.quarkkingdee.top

struct P { var x: Int }
来源：http://uwb.wangdashe.top

[T26] Swift：类与重写
来源：http://kjc.sysykeji.top

class A: Base { override func f() {} }
来源：http://czo.yuanzhike.top


<!-- 参考信息 -->