代发 wailian999

echo "${#s}"
来源：http://luc.jianghu66.top

[R22] 截取子串
来源：http://cpc.snrcjt.cn

echo "${s:0:5}"
来源：http://udb.mhx1999.top

[R23] 字符串替换
来源：http://cbm.haohaochexian.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://byf.jqgufenzy.top

[R24] 大小写转换
来源：http://pkt.yuanzhike.top

echo "${s^^}"; echo "${s,,}"
来源：http://rvg.redwolf501.top

[R25] 去后缀 / 去前缀
来源：http://csx.zdqjudy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://nia.tianlin.xyz

[R26] 命令替换
来源：http://tac.zhongyouzk.top

now=$(date +%F); echo "$now"
来源：http://bve.feifeiyinyue.top

[R27] 算术展开
来源：http://voh.cqqwz.cn

echo $((1 + 2 * 3))
来源：http://ivy.fehbvm.com

[R28] 浮点运算
来源：http://bqh.guannengcc.top

echo "scale=2; 10/3" | bc
来源：http://dry.shzxlz.cn

[R29] 定义函数
来源：http://ktp.daxiang520.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pvs.birdmap.top

[R30] 函数返回状态码
来源：http://yqi.ybcxt.top

f() { return 0; }; f || echo "失败了"
来源：http://xae.birdmap.top

[R31] 局部变量
来源：http://dlz.yuxming.cn

f() { local x=1; echo "$x"; }
来源：http://ljh.zhengqikj.top

[R32] 参数个数校验
来源：http://qta.yj20258888.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vqo.svipenyu.cn

[R33] 捕获错误并提示行号
来源：http://egx.snrcjt.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://obf.ppjwa.cn

[R34] 退出时清理
来源：http://inm.wangdashe.top

trap 'rm -f "$tmp"' EXIT
来源：http://uqc.vehdjk.com

[R35] 后台执行并等待
来源：http://ekr.52xcode.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rqx.yuxming.cn

[R36] 并发执行多个任务
来源：http://jad.kuanghao11.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sct.shzxlz.cn

[R37] 把输出赋给变量
来源：http://vyi.wangdashe.top

files=$(ls -1)
来源：http://wbn.sxryk.cn

[R38] 管道串联
来源：http://whr.tanke756.top

cat a.txt | grep -i error | wc -l
来源：http://ebb.iojbl.cn

[R39] 重定向标准输出与错误
来源：http://rzi.cqqwz.cn

cmd > out.log 2>&1
来源：http://dci.shanyushiyangtech.top

[R40] 追加写日志
来源：http://tyh.jqgfzy.top

echo "log" >> out.log
来源：http://tkn.guannengcc.top

[R41] 丢弃输出
来源：http://fhk.gotoacloud.top

cmd >/dev/null 2>&1
来源：http://kpj.cashguo.top

[R42] 输入重定向
来源：http://jkr.jyoumei.cn

wc -l < a.txt
来源：http://tki.tian-w.cn

[R43] 按名字查找文件
来源：http://ram.fzhhl.top

find . -name "*.log" -type f
来源：http://exv.fehbvm.com

[R44] 按修改时间查找
来源：http://czs.0kj1m.cn

find . -mtime -7 -type f
来源：http://nrd.tian-w.cn

[R45] 批量删除
来源：http://zpp.yj20258888.top

find . -name "*.tmp" -delete
来源：http://aul.hesvh.cn

[R46] 递归替换文件内容
来源：http://tzx.yj20258888.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://aee.ivvv.top

[R47] sed 单行替换
来源：http://wmw.ivvv.top

sed -i 's/foo/bar/g' a.txt
来源：http://kgj.fktsv.cn

[R48] awk 取指定列
来源：http://xbe.iojbl.cn

awk '{print $1, $3}' a.txt
来源：http://njo.fengsongda.top

[R49] awk 带条件
来源：http://skg.zhaomingkeji.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sxh.ydzc1.top

[R50] awk 求和
来源：http://ege.xylfe.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ymg.jinqigufen.top

[R51] 排序去重取前几
来源：http://noq.jianghu66.top

sort a.txt | uniq -c | sort -rn | head
来源：http://bgb.zhijiandao.cn

[R52] 统计行数
来源：http://sfv.hnqzz.top

wc -l a.txt
来源：http://nht.tanke756.top

[R53] 查看文件头与实时尾
来源：http://qqy.yfazqb.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xvg.hcnkem.com

[R54] 比较两个文件
来源：http://nva.iojbl.cn

diff a.txt b.txt
来源：http://ohm.ydjk.org.cn

[R55] 压缩与解压
来源：http://ptg.ydzc1.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zoj.shanyushiyangkeji.top

[R56] 远程拷贝
来源：http://mvu.shuidangran.top

scp file user@host:/path/
来源：http://xzz.bbcook.cn

[R57] 远程执行命令
来源：http://iui.xuanzx.com

ssh user@host 'uptime'
来源：http://tjc.jianghu66.top

[R58] 下载文件
来源：http://bid.zhaomingkeji.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lfz.wangshuangyany.cn

[R59] 发 POST JSON
来源：http://oot.gogol.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://izh.feifeiyinyue.top

[R60] 只看 HTTP 状态码
来源：http://fva.hfpthk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zfl.jinyuanbaomall.cn

[R61] 磁盘占用
来源：http://lcx.hongshengwenyu.top

df -h;  du -sh *
来源：http://mom.c1oappe.top

[R62] 找最占空间的文件
来源：http://wza.shanyushiyangtech.top

du -ah . | sort -rh | head -10
来源：http://hrd.zdqjudy.top

[R63] 内存与进程
来源：http://tor.hywenlv.cn

free -h;  ps aux | grep nginx
来源：http://avw.ywan-chungtsiang.top

[R64] 结束进程
来源：http://djf.kuanghao11.cn

kill -9 $(pgrep -f app.py)
来源：http://enz.zhiwuduotai.top

[R65] 查看端口占用
来源：http://dvq.wangshuangyany.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://adw.zhixingplan.top

[R66] 定时任务
来源：http://mnp.tianlin.xyz

crontab -e;  crontab -l
来源：http://hpo.yueranfly.top

[R67] 生成随机十六进制串
来源：http://qvh.yfazqb.com

openssl rand -hex 16
来源：http://meq.xuetiantiany.cn

[R68] 计算文件校验值
来源：http://tfh.yj20258.top

sha256sum a.txt;  md5sum a.txt
来源：http://ljq.tanke756.top

[R69] 生成随机密码
来源：http://tcb.dashuyun.cn

head -c 16 /dev/urandom | base64
来源：http://uld.yvedp.cn

[R70] 时间戳与互转
来源：http://xef.nwbrower.top

date +%s;  date -d @1700000000
来源：http://gzd.yangfankeji.com

[R71] 日期格式化
来源：http://bne.xylfe.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xmf.bbcook.cn

[R72] 等待端口就绪
来源：http://bfw.tarul.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sqe.snrcjt.cn

[R73] 分割大日志
来源：http://yqx.sysykeji.top

split -l 1000 big.log part_
来源：http://ojf.wangshuangyany.cn

[R74] 批量重命名
来源：http://ura.nwbrower.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ojn.gotoacloud.top

[R75] 导出环境变量
来源：http://bgm.jiagoushi.top

export PATH="$HOME/bin:$PATH"
来源：http://sec.xylfe.cn

[R76] 使用临时文件
来源：http://dbv.gotoacloud.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ond.uphjek.com

[R77] 读取用户输入
来源：http://vxx.jinghuilouyu.cn

read -rp "请输入: " ans
来源：http://art.nwbrower.top

[R78] 交互式菜单
来源：http://lxh.yongpay.top

select opt in a b c; do echo "$opt"; break; done
来源：http://kxm.sufxvd.cn

[R79] 解析命令行选项
来源：http://kgk.zhoulong.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uol.zhiwuduotai.top

[R80] 查看脚本执行耗时
来源：http://gkh.fzhhl.top

time ./run.sh
来源：http://dqz.tian-w.cn

================================================================================
来源：http://obr.zdqjudy.top

S. C / C++ 专题
来源：http://wpg.meibo888.top

================================================================================
来源：http://iia.mhx1999.top

[S01] C：Hello World
来源：http://ofd.xinyue.icu

#include <stdio.h>
来源：http://mom.tarul.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xon.xinyue.icu

[S02] C：变量与格式化输出
来源：http://sqq.fktsv.cn

int a = 10; printf("%d\n", a);
来源：http://pys.cashguo.top

[S03] C：读入整数
来源：http://get.svipenyu.cn

int x; scanf("%d", &x);
来源：http://ycd.hcnkem.com

[S04] C：字符串复制
来源：http://zcr.vqdsnc.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lcz.tanke756.top

[S05] C：字符串长度
来源：http://xut.vehdjk.com

strlen(s)
来源：http://qxw.yj202588.top

[S06] C：字符串比较
来源：http://ife.chenzaomai.com

strcmp(a, b) == 0
来源：http://mhu.shuidangran.top

[S07] C：数组遍历求和
来源：http://ddm.guannengcc.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jxg.ctjpmb.com

[S08] C：动态内存分配与释放
来源：http://ltj.fzhhl.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://big.c1oappe.top

[S09] C：结构体定义与初始化
来源：http://uwf.gzhubu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xzy.dianchejie.cn

[S10] C：指针与解引用
来源：http://pjk.tarul.cn

int *p = &a;  *p = 5;
来源：http://tka.pengpengdd.cyou

[S11] C：逐行读文件
来源：http://gwk.cqqwz.cn

FILE *f = fopen("a.txt", "r");
来源：http://dtf.yfazqb.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://gaz.tarul.cn

fclose(f);
来源：http://zsp.shangyingyoupin.top

[S12] C：写文件
来源：http://xhx.meibo888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vax.tanke756.top

[S13] C：宏定义
来源：http://frb.shanyushiyangtech.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yqg.gotoacloud.top

[S14] C：枚举
来源：http://lzh.xuanzx.com

enum Color { RED, GREEN, BLUE };
来源：http://oet.bjfxy.top

[S15] C：类型转换
来源：http://kdl.ppjwa.cn

(double) a / b
来源：http://kme.kuanghao11.cn

[S16] C：位操作置位
来源：http://iuo.zdqjudy.top

x |= (1 << 3);
来源：http://jcy.jyoumei.cn

[S17] C：安全拼接字符串
来源：http://ojz.cucudq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://teo.yj202588.top

[S18] C：命令行参数
来源：http://tlt.hnqzz.top

int main(int argc, char **argv)
来源：http://imw.ehwqpu.com

[S19] C：快速排序
来源：http://svz.yj20258888.top

qsort(a, n, sizeof(int), cmp);
来源：http://hwp.ctjpmb.com

[S20] C：二分查找
来源：http://slq.ehwqpu.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mee.yfazqb.com

[S21] C：字符类别判断
来源：http://zyb.daxiang520.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dle.cdnleiting.top

[S22] C：字符串转数字
来源：http://sqm.shuidangran.top

atoi("42");  strtod("3.14", NULL);
来源：http://gwn.havefunace.top

[S23] C：随机数
来源：http://dbq.yuxming.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://axd.ywan-chungtsiang.top

[S24] C：获取本地时间
来源：http://onr.uphjek.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://spb.daxiang520.top

[S25] C：内存拷贝
来源：http://tbm.zdqjudy.top

memcpy(dst, src, n);
来源：http://mgc.sweek.top

[S26] C：内存清零
来源：http://mpx.zhongyouzk.top

memset(a, 0, sizeof a);
来源：http://elk.zhengqikj.top

[S27] C：定义常量
来源：http://qxj.aibaodan.cn

const double PI = 3.14159;
来源：http://faz.yvedp.cn

[S28] C：静态变量
来源：http://qru.havefunace.top

static int counter = 0;
来源：http://mhb.hfpthk.cn

[S29] C：变参函数
来源：http://voi.xinyue.icu

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lyz.cqqwz.cn

[S30] C：头文件保护
来源：http://yea.fengsongda.top

#ifndef X_H
来源：http://jzi.gogol.net.cn

#define X_H
来源：http://zmt.xuanzx.com

#endif
来源：http://kmc.xingfuxueyuan.xyz

[S31] C++：Hello World
来源：http://qrt.ydjk.org.cn

#include <iostream>
来源：http://wfa.dianchejie.cn

int main() { std::cout << "Hello\n"; }
来源：http://vrg.shangyingyoupin.top

[S32] C++：字符串
来源：http://gfr.jiagoushi.top

std::string s = "hi";  s += "!";
来源：http://snu.gaohongyu789.top

[S33] C++：vector 增删
来源：http://wfx.hywenlv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ydf.fzhhl.top

[S34] C++：遍历 vector
来源：http://poq.jinyuanbaomall.cn

for (auto &x : v) { std::cout << x; }
来源：http://aio.hywenlv.cn

[S35] C++：map
来源：http://kwd.jqgufenzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ywn.gaohongyu789.top

[S36] C++：unordered_map
来源：http://paf.hnqzz.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yha.shangyingyoupin.top

[S37] C++：set
来源：http://ilx.jinghuilouyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ail.xingfuxueyuan.xyz

[S38] C++：排序
来源：http://ctz.cashguo.top

std::sort(v.begin(), v.end());
来源：http://njm.haohaochexian.top

[S39] C++：自定义比较器排序
来源：http://fvy.ppjwa.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bdn.haohaochexian.top

[S40] C++：查找元素
来源：http://anh.sysykeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lgn.hammf.cn

[S41] C++：类与构造函数
来源：http://jrj.ivvv.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uqv.redwolf501.top

[S42] C++：继承与虚函数
来源：http://uun.uphjek.com

class B : public Base { public: void f() override {} };
来源：http://trn.zhaomingkeji.xyz

[S43] C++：智能指针
来源：http://jsq.hammf.cn

auto p = std::make_unique<int>(5);
来源：http://ouf.iojbl.cn

[S44] C++：引用传参
来源：http://rle.yvedp.cn

void inc(int &x) { ++x; }
来源：http://zpu.pengpengdd.cyou

[S45] C++：lambda
来源：http://vsj.birdmap.top

auto add = [](int a, int b) { return a + b; };
来源：http://nzo.smart0.xyz

[S46] C++：函数模板
来源：http://fqp.redwolf501.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hpm.nwbrower.top

[S47] C++：结构化绑定遍历
来源：http://lok.jianghu66.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oqr.jinyuanbaomall.cn

[S48] C++：逐行读文件
来源：http://vol.svipenyu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xqc.sxryk.cn

while (std::getline(in, line)) { }
来源：http://loy.jinyuanbaomall.cn

[S49] C++：写文件
来源：http://tvm.ydzc1.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://djp.sysykeji.top

[S50] C++：格式化数字
来源：http://qcz.ydjk.org.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lli.316326.xyz

[S51] C++：显式类型转换
来源：http://usz.kuanghao11.cn

static_cast<double>(a) / b
来源：http://rvy.bjfxy.top

[S52] C++：const 与 noexcept
来源：http://igr.vqdsnc.cn

int size() const noexcept { return n_; }
来源：http://rnz.316326.xyz

[S53] C++：移动语义
来源：http://jmt.yueranfly.top

std::vector<int> w = std::move(v);
来源：http://oyg.guannengcc.top

[S54] C++：异常处理
来源：http://kan.bjfxy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zvc.gogol.net.cn

[S55] C++：结构化绑定
来源：http://eig.yonumen.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qkf.shanyushiyangkeji.top

[S56] C++：optional
来源：http://plh.ehwqpu.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kdr.cqqwz.cn

[S57] C++：编译期常量
来源：http://bzk.ywan-chungtsiang.top

constexpr int N = 10;
来源：http://psr.xinyue.icu

[S58] C++：命名空间
来源：http://pdt.cashguo.top

namespace ns { int f() { return 1; } }
来源：http://lwz.ppjwa.cn

[S59] C++：静态断言
来源：http://pdg.xuanzx.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dov.0kj1m.cn

[S60] C++：遍历并删除元素
来源：http://qax.cashguo.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://urv.cashguo.top

================================================================================
来源：http://ifl.fanxiaobao.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mwq.hcnkem.com

================================================================================
来源：http://scc.zhoulong.xyz

[T01] Kotlin：Hello World
来源：http://wiq.hesvh.cn

println("Hello")
来源：http://uca.yuxming.cn

[T02] Kotlin：变量
来源：http://jph.yuanzhike.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://thd.ehwqpu.com

[T03] Kotlin：字符串模板
来源：http://ynf.gogol.net.cn

"值: $b"
来源：http://inm.haohaochexian.top

[T04] Kotlin：空安全
来源：http://ymk.jianghu66.top

val n: String? = null;  n?.length
来源：http://wzx.mhx1999.top

[T05] Kotlin：when 表达式
来源：http://yjs.pycfn.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://plr.fktsv.cn

[T06] Kotlin：集合映射
来源：http://xsv.xinyue.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://bwu.fehbvm.com

[T07] Kotlin：集合过滤
来源：http://rnu.316326.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://rbt.hesvh.cn

[T08] Kotlin：数据类
来源：http://fdb.cashguo.top

data class User(val name: String, val age: Int)
来源：http://wji.quarkkingdee.top

[T09] Kotlin：扩展函数
来源：http://xwg.shzxlz.cn

fun String.exclaim() = this + "!"
来源：http://nwl.chenjidiqi.icu

[T10] Kotlin：默认参数
来源：http://esy.fanxiaobao.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://rfc.gaohongyu789.top

[T11] Kotlin：协程
来源：http://smw.ctjpmb.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://muh.sjlbkw.cn

[T12] Kotlin：解构声明
来源：http://zsg.ydzc1.top

val (a, b) = Pair(1, 2)
来源：http://tlh.jinghuilouyu.cn

[T13] Kotlin：只读 Map
来源：http://aed.yj20258.top

val m = mapOf("a" to 1)
来源：http://clq.ppjwa.cn

[T14] Kotlin：循环
来源：http://fmp.c1oappe.top

for (i in 1..10) println(i)
来源：http://gtb.dashuyun.cn

[T15] Kotlin：接口
来源：http://rkz.zhongyouzk.top

interface Shape { fun area(): Double }
来源：http://xca.hnxiangtu.top

[T16] Swift：Hello World
来源：http://tcy.hfpthk.cn

print("Hello")
来源：http://ovh.epnwcf.com

[T17] Swift：变量与常量
来源：http://pdi.bbcook.cn

var a = 1;  let b = 2
来源：http://kgh.nwbrower.top

[T18] Swift：字符串插值
来源：http://psr.ywan-chungtsiang.top

"值: \(b)"
来源：http://yxt.jyoumei.cn

[T19] Swift：可选绑定
来源：http://mlx.svipenyu.cn

if let n = opt { print(n) }
来源：http://gtu.gotoacloud.top

[T20] Swift：数组操作
来源：http://vit.gaohongyu789.top

var a = [1, 2, 3];  a.append(4)
来源：http://jxh.xuanzx.com

[T21] Swift：遍历
来源：http://btw.chenlongwang.top

for x in a { print(x) }
来源：http://lkg.haohaochexian.top

[T22] Swift：字典
来源：http://agl.ydzc1.top

var d = ["a": 1];  d["b"] = 2
来源：http://mys.yanxiufei.cn

[T23] Swift：函数
来源：http://oxr.shanyushiyangtech.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qdi.xuanzx.com

[T24] Swift：闭包
来源：http://kel.cqqwz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zns.guowangkeji.top


<!-- 参考信息 -->