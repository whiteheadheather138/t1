代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nbo.hammf.cn

[R24] 大小写转换
来源：http://ilu.mhx1999.top

echo "${s^^}"; echo "${s,,}"
来源：http://kdj.hammf.cn

[R25] 去后缀 / 去前缀
来源：http://bpt.jinghuilouyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mui.sjlbkw.cn

[R26] 命令替换
来源：http://bxo.yj20258.top

now=$(date +%F); echo "$now"
来源：http://mil.smart0.xyz

[R27] 算术展开
来源：http://rck.tianlin.xyz

echo $((1 + 2 * 3))
来源：http://xse.shanyushiyangtech.top

[R28] 浮点运算
来源：http://kff.guannengcc.top

echo "scale=2; 10/3" | bc
来源：http://biq.gotoacloud.top

[R29] 定义函数
来源：http://lbp.shanyushiyangtech.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kdn.xuanzx.com

[R30] 函数返回状态码
来源：http://ovp.yuanzhike.top

f() { return 0; }; f || echo "失败了"
来源：http://hkm.cheryme.top

[R31] 局部变量
来源：http://ecu.tarul.cn

f() { local x=1; echo "$x"; }
来源：http://qib.jinqigufen.top

[R32] 参数个数校验
来源：http://vpb.xuetiantiany.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qic.cheryme.top

[R33] 捕获错误并提示行号
来源：http://zre.redwolf501.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jtm.daxiang520.top

[R34] 退出时清理
来源：http://kqz.aizwys.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mgt.haohaochexian.top

[R35] 后台执行并等待
来源：http://naz.pycfn.com

sleep 5 & pid=$!; wait "$pid"
来源：http://abu.guowangkeji.top

[R36] 并发执行多个任务
来源：http://dvo.bbcook.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nqm.aibaodan.cn

[R37] 把输出赋给变量
来源：http://iyg.sysykeji.top

files=$(ls -1)
来源：http://qna.yongpay.top

[R38] 管道串联
来源：http://gjq.guowangkeji.top

cat a.txt | grep -i error | wc -l
来源：http://pib.bjfxy.top

[R39] 重定向标准输出与错误
来源：http://rtx.chenjidiqi.icu

cmd > out.log 2>&1
来源：http://dfw.quarkkingdee.top

[R40] 追加写日志
来源：http://yfa.yj20258.top

echo "log" >> out.log
来源：http://azh.guannengcc.top

[R41] 丢弃输出
来源：http://sqg.shzxlz.cn

cmd >/dev/null 2>&1
来源：http://dnc.fktsv.cn

[R42] 输入重定向
来源：http://qke.nanxinkj.top

wc -l < a.txt
来源：http://nlm.jianghu66.top

[R43] 按名字查找文件
来源：http://nqg.haohaochexian.top

find . -name "*.log" -type f
来源：http://lck.shzxlz.cn

[R44] 按修改时间查找
来源：http://oly.tarul.cn

find . -mtime -7 -type f
来源：http://jzp.0kj1m.cn

[R45] 批量删除
来源：http://fnl.zdbjq.cn

find . -name "*.tmp" -delete
来源：http://ihq.cqqwz.cn

[R46] 递归替换文件内容
来源：http://njd.hesvh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vst.haohaochexian.top

[R47] sed 单行替换
来源：http://ehg.nwbrower.top

sed -i 's/foo/bar/g' a.txt
来源：http://gxz.xuanzx.com

[R48] awk 取指定列
来源：http://qge.xylfe.cn

awk '{print $1, $3}' a.txt
来源：http://uey.nanxuanxn.top

[R49] awk 带条件
来源：http://coa.snrcjt.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ivs.ywan-chungtsiang.top

[R50] awk 求和
来源：http://xmd.gotoacloud.top

awk '{s += $2} END {print s}' a.txt
来源：http://dtx.ppjwa.cn

[R51] 排序去重取前几
来源：http://qzd.sysykeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://cox.xylfe.cn

[R52] 统计行数
来源：http://sos.hywenlv.cn

wc -l a.txt
来源：http://liq.gogol.net.cn

[R53] 查看文件头与实时尾
来源：http://faz.gaohongyu789.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pol.aibaodan.cn

[R54] 比较两个文件
来源：http://rae.kuanghao11.cn

diff a.txt b.txt
来源：http://tjr.ybcxt.top

[R55] 压缩与解压
来源：http://pwo.yanxiufei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hce.birdmap.top

[R56] 远程拷贝
来源：http://qbc.9152youxi.cn

scp file user@host:/path/
来源：http://mqt.fehbvm.com

[R57] 远程执行命令
来源：http://ssi.hfpthk.cn

ssh user@host 'uptime'
来源：http://frv.sufxvd.cn

[R58] 下载文件
来源：http://uol.sweek.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nfh.mhx1999.top

[R59] 发 POST JSON
来源：http://gfn.daria6918.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://egk.chenlongwang.top

[R60] 只看 HTTP 状态码
来源：http://qnu.yuxming.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lbh.chenzaomai.com

[R61] 磁盘占用
来源：http://cng.cucudq.cn

df -h;  du -sh *
来源：http://pnj.jinyuanbaomall.cn

[R62] 找最占空间的文件
来源：http://ijr.chenzaomai.com

du -ah . | sort -rh | head -10
来源：http://fkn.hywenlv.cn

[R63] 内存与进程
来源：http://wkn.tanke756.top

free -h;  ps aux | grep nginx
来源：http://dkb.hammf.cn

[R64] 结束进程
来源：http://xle.zhaomingkeji.xyz

kill -9 $(pgrep -f app.py)
来源：http://wts.xuetiantiany.cn

[R65] 查看端口占用
来源：http://pfg.ehwqpu.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://poo.cqqwz.cn

[R66] 定时任务
来源：http://nty.sjlbkw.cn

crontab -e;  crontab -l
来源：http://zqe.gotoacloud.top

[R67] 生成随机十六进制串
来源：http://xbd.yuxming.cn

openssl rand -hex 16
来源：http://xwq.wangshuangyany.cn

[R68] 计算文件校验值
来源：http://kra.fengsongda.top

sha256sum a.txt;  md5sum a.txt
来源：http://aba.zhixingplan.top

[R69] 生成随机密码
来源：http://jpk.zdqjudy.top

head -c 16 /dev/urandom | base64
来源：http://eor.jyoumei.cn

[R70] 时间戳与互转
来源：http://rcd.jqgfzy.top

date +%s;  date -d @1700000000
来源：http://zlb.cashguo.top

[R71] 日期格式化
来源：http://kus.uphjek.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://gwh.yvedp.cn

[R72] 等待端口就绪
来源：http://lxm.nanxuanxn.top

until nc -z localhost 3306; do sleep 1; done
来源：http://vjd.ydjk.org.cn

[R73] 分割大日志
来源：http://chi.zdqjudy.top

split -l 1000 big.log part_
来源：http://ohq.wangdashe.top

[R74] 批量重命名
来源：http://mzb.iojbl.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wis.wangdashe.top

[R75] 导出环境变量
来源：http://ley.jianghu66.top

export PATH="$HOME/bin:$PATH"
来源：http://dte.hfpthk.cn

[R76] 使用临时文件
来源：http://hhx.nanxuanxn.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fmz.svipenyu.cn

[R77] 读取用户输入
来源：http://gos.hywenlv.cn

read -rp "请输入: " ans
来源：http://iix.chenjidiqi.icu

[R78] 交互式菜单
来源：http://obr.hnxiangtu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://jxc.chenlongwang.top

[R79] 解析命令行选项
来源：http://rcj.smart0.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bkn.bjfxy.top

[R80] 查看脚本执行耗时
来源：http://ygp.pycfn.com

time ./run.sh
来源：http://txe.cheryme.top

================================================================================
来源：http://fkl.ivvv.top

S. C / C++ 专题
来源：http://poz.haohaochexian.top

================================================================================
来源：http://ueh.shanyushiyangtech.top

[S01] C：Hello World
来源：http://mnu.cucudq.cn

#include <stdio.h>
来源：http://hws.zhengqikj.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xlq.nwbrower.top

[S02] C：变量与格式化输出
来源：http://cle.fktsv.cn

int a = 10; printf("%d\n", a);
来源：http://tzd.shanyushiyangtech.top

[S03] C：读入整数
来源：http://xlb.birdmap.top

int x; scanf("%d", &x);
来源：http://bau.xziqi.cn

[S04] C：字符串复制
来源：http://kfz.316326.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://lkp.hcnkem.com

[S05] C：字符串长度
来源：http://bqd.ywan-chungtsiang.top

strlen(s)
来源：http://onj.jinqigfzy.top

[S06] C：字符串比较
来源：http://vuz.wangshuangyany.cn

strcmp(a, b) == 0
来源：http://fao.shuidangran.top

[S07] C：数组遍历求和
来源：http://ghq.ybcxt.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iue.shanyushiyangkeji.top

[S08] C：动态内存分配与释放
来源：http://iku.yj202588.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zeu.yanxiufei.cn

[S09] C：结构体定义与初始化
来源：http://kqj.hfpthk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sat.fehbvm.com

[S10] C：指针与解引用
来源：http://bir.zdbjq.cn

int *p = &a;  *p = 5;
来源：http://bwl.nanxinkj.top

[S11] C：逐行读文件
来源：http://waf.cdnleiting.top

FILE *f = fopen("a.txt", "r");
来源：http://vwf.yangfankeji.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://nao.fktsv.cn

fclose(f);
来源：http://lez.jqgfzy.top

[S12] C：写文件
来源：http://iic.hfpthk.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lks.ydzc1.top

[S13] C：宏定义
来源：http://lsj.yj20258.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vza.zhoulong.xyz

[S14] C：枚举
来源：http://jrn.hesvh.cn

enum Color { RED, GREEN, BLUE };
来源：http://bqg.ehwqpu.com

[S15] C：类型转换
来源：http://znm.sufxvd.cn

(double) a / b
来源：http://xiz.316326.xyz

[S16] C：位操作置位
来源：http://yjw.haohaochexian.top

x |= (1 << 3);
来源：http://eap.shanyushiyangkeji.top

[S17] C：安全拼接字符串
来源：http://wav.hnqzz.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://enr.yj202588.top

[S18] C：命令行参数
来源：http://ysb.jinqigufen.top

int main(int argc, char **argv)
来源：http://zxh.jianghu66.top

[S19] C：快速排序
来源：http://kzg.ppjwa.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lry.xingfuxueyuan.xyz

[S20] C：二分查找
来源：http://wfc.jianghu66.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lwe.xuetiantiany.cn

[S21] C：字符类别判断
来源：http://umh.yj20258.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lif.cheryme.top

[S22] C：字符串转数字
来源：http://tsu.cashguo.top

atoi("42");  strtod("3.14", NULL);
来源：http://fal.daxiang520.top

[S23] C：随机数
来源：http://yve.smart0.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://klw.pycfn.com

[S24] C：获取本地时间
来源：http://add.wangdashe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gky.ybcxt.top

[S25] C：内存拷贝
来源：http://pqk.jlsjyb.cn

memcpy(dst, src, n);
来源：http://wtw.xuetiantiany.cn

[S26] C：内存清零
来源：http://txu.bbcook.cn

memset(a, 0, sizeof a);
来源：http://rgm.shuidangran.top

[S27] C：定义常量
来源：http://khj.wangdashe.top

const double PI = 3.14159;
来源：http://xmt.bbcook.cn

[S28] C：静态变量
来源：http://pkv.zycfv.cn

static int counter = 0;
来源：http://ynq.tian-w.cn

[S29] C：变参函数
来源：http://vzs.c1oappe.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wdh.shanyushiyangkeji.top

[S30] C：头文件保护
来源：http://zud.bbcook.cn

#ifndef X_H
来源：http://zpw.cqqwz.cn

#define X_H
来源：http://tsv.fanxiaobao.xyz

#endif
来源：http://cwc.fehbvm.com

[S31] C++：Hello World
来源：http://pfa.zycfv.cn

#include <iostream>
来源：http://oqr.yvedp.cn

int main() { std::cout << "Hello\n"; }
来源：http://ryy.jinqigfzy.top

[S32] C++：字符串
来源：http://qhd.sjlbkw.cn

std::string s = "hi";  s += "!";
来源：http://lzl.gogol.net.cn

[S33] C++：vector 增删
来源：http://kis.zhijiandao.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://oqg.yuxming.cn

[S34] C++：遍历 vector
来源：http://nmu.andypj.xyz

for (auto &x : v) { std::cout << x; }
来源：http://msp.jinqigufen.top

[S35] C++：map
来源：http://fcv.hysaishi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lpp.hnxiangtu.top

[S36] C++：unordered_map
来源：http://cxi.havefunace.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ecd.hnqzz.top

[S37] C++：set
来源：http://bkr.tanke756.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hwk.chenlongwang.top

[S38] C++：排序
来源：http://mlt.yuanzhike.top

std::sort(v.begin(), v.end());
来源：http://dcd.jlsjyb.cn

[S39] C++：自定义比较器排序
来源：http://yyi.52xcode.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qml.hcnkem.com

[S40] C++：查找元素
来源：http://xcs.meibo888.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qkr.yongpay.top

[S41] C++：类与构造函数
来源：http://arb.yanxiufei.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iie.zhoulong.xyz

[S42] C++：继承与虚函数
来源：http://oft.haohaochexian.top

class B : public Base { public: void f() override {} };
来源：http://yym.yj20258888.top

[S43] C++：智能指针
来源：http://dlx.jinyuanbaomall.cn

auto p = std::make_unique<int>(5);
来源：http://fgj.gogol.net.cn

[S44] C++：引用传参
来源：http://ynx.aizwys.cn

void inc(int &x) { ++x; }
来源：http://ult.pengpengdd.cyou

[S45] C++：lambda
来源：http://hfv.uphjek.com

auto add = [](int a, int b) { return a + b; };
来源：http://exn.zhijiandao.cn

[S46] C++：函数模板
来源：http://vvz.hammf.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gqz.aizwys.cn

[S47] C++：结构化绑定遍历
来源：http://jtz.aizwys.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mpd.shzxlz.cn

[S48] C++：逐行读文件
来源：http://cbr.bbcook.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xnf.xinyue.icu

while (std::getline(in, line)) { }
来源：http://koe.yuxming.cn

[S49] C++：写文件
来源：http://laq.cdnleiting.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jfp.zhengqikj.top

[S50] C++：格式化数字
来源：http://ddm.fktsv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://axk.jianghu66.top

[S51] C++：显式类型转换
来源：http://ruo.xinyue.icu

static_cast<double>(a) / b
来源：http://ngq.52xcode.cn

[S52] C++：const 与 noexcept
来源：http://vfv.yfazqb.com

int size() const noexcept { return n_; }
来源：http://cba.epnwcf.com

[S53] C++：移动语义
来源：http://nnd.quarkkingdee.top

std::vector<int> w = std::move(v);
来源：http://gbs.shuidangran.top

[S54] C++：异常处理
来源：http://dvq.yuxming.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ops.yuxming.cn

[S55] C++：结构化绑定
来源：http://nwu.gotoacloud.top

auto [a, b] = std::make_pair(1, 2);
来源：http://uip.guowangkeji.top

[S56] C++：optional
来源：http://ntt.xziqi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nls.jinqigfzy.top

[S57] C++：编译期常量
来源：http://nks.meibo888.top

constexpr int N = 10;
来源：http://glw.jianghu66.top

[S58] C++：命名空间
来源：http://obo.jinqigfzy.top

namespace ns { int f() { return 1; } }
来源：http://zqs.chenlongwang.top

[S59] C++：静态断言
来源：http://bqu.yj20258.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://srb.cqqwz.cn

[S60] C++：遍历并删除元素
来源：http://uvg.hnqzz.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fev.0kj1m.cn

================================================================================
来源：http://ust.yuanzhike.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://opw.xylfe.cn

================================================================================
来源：http://gez.chenjidiqi.icu

[T01] Kotlin：Hello World
来源：http://ptw.yfazqb.com

println("Hello")
来源：http://ldz.nwbrower.top

[T02] Kotlin：变量
来源：http://qeg.andypj.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://khq.shangyingyoupin.top

[T03] Kotlin：字符串模板
来源：http://gni.shzxlz.cn

"值: $b"
来源：http://kbg.haohaochexian.top

[T04] Kotlin：空安全
来源：http://qlg.sxryk.cn

val n: String? = null;  n?.length
来源：http://enh.fehbvm.com

[T05] Kotlin：when 表达式
来源：http://erm.daxiang520.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kre.zdbjq.cn

[T06] Kotlin：集合映射
来源：http://ugd.chenlongwang.top

listOf(1, 2, 3).map { it * 2 }
来源：http://lbc.ybcxt.top

[T07] Kotlin：集合过滤
来源：http://lzm.zdbjq.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fkw.zhoulong.xyz

[T08] Kotlin：数据类
来源：http://nmk.chenlongwang.top

data class User(val name: String, val age: Int)
来源：http://ote.ydjk.org.cn

[T09] Kotlin：扩展函数
来源：http://nwh.xziqi.cn

fun String.exclaim() = this + "!"
来源：http://pky.epnwcf.com

[T10] Kotlin：默认参数
来源：http://cxy.cashguo.top

fun greet(name: String = "World") = "Hi $name"
来源：http://fkt.daria6918.cn

[T11] Kotlin：协程
来源：http://qkc.gotoacloud.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://xmf.xylfe.cn

[T12] Kotlin：解构声明
来源：http://ggw.tianlin.xyz

val (a, b) = Pair(1, 2)
来源：http://oko.yj20258888.top

[T13] Kotlin：只读 Map
来源：http://van.gaohongyu789.top

val m = mapOf("a" to 1)
来源：http://mow.havefunace.top

[T14] Kotlin：循环
来源：http://elm.kuanghao11.cn

for (i in 1..10) println(i)
来源：http://dch.hongshengwenyu.top

[T15] Kotlin：接口
来源：http://gha.havefunace.top

interface Shape { fun area(): Double }
来源：http://eok.chenzaomai.com

[T16] Swift：Hello World
来源：http://sag.xingfuxueyuan.xyz

print("Hello")
来源：http://qjw.sufxvd.cn

[T17] Swift：变量与常量
来源：http://tgz.quarkkingdee.top

var a = 1;  let b = 2
来源：http://smj.yangfankeji.com

[T18] Swift：字符串插值
来源：http://lxy.yangfankeji.com

"值: \(b)"
来源：http://jky.feifeiyinyue.top

[T19] Swift：可选绑定
来源：http://uxp.9152youxi.cn

if let n = opt { print(n) }
来源：http://exc.xylfe.cn

[T20] Swift：数组操作
来源：http://fkd.mhx1999.top

var a = [1, 2, 3];  a.append(4)
来源：http://qot.shuidangran.top

[T21] Swift：遍历
来源：http://azv.haohaochexian.top

for x in a { print(x) }
来源：http://xrt.ybcxt.top

[T22] Swift：字典
来源：http://qrq.xuetiantiany.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sdz.pengpengdd.cyou

[T23] Swift：函数
来源：http://aee.cheryme.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://peb.yonumen.top

[T24] Swift：闭包
来源：http://ram.shzxlz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hnf.jqgfzy.top

[T25] Swift：结构体
来源：http://wgl.jiagoushi.top

struct P { var x: Int }
来源：http://gdk.tanke756.top

[T26] Swift：类与重写
来源：http://axe.ctjpmb.com

class A: Base { override func f() {} }
来源：http://dfx.yj20258.top


<!-- 参考信息 -->