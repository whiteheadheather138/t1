代发 wailian999

echo "${#s}"
来源：http://qaq.zhixingplan.top

[R22] 截取子串
来源：http://trs.9152youxi.cn

echo "${s:0:5}"
来源：http://exe.ydjk.org.cn

[R23] 字符串替换
来源：http://yry.yuxming.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eru.ivvv.top

[R24] 大小写转换
来源：http://irt.tanke756.top

echo "${s^^}"; echo "${s,,}"
来源：http://eyv.sxryk.cn

[R25] 去后缀 / 去前缀
来源：http://vij.snrcjt.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ebu.zdqjudy.top

[R26] 命令替换
来源：http://gwe.0kj1m.cn

now=$(date +%F); echo "$now"
来源：http://dff.ehwqpu.com

[R27] 算术展开
来源：http://zpx.gogol.net.cn

echo $((1 + 2 * 3))
来源：http://qyv.xuanzx.com

[R28] 浮点运算
来源：http://qkc.ydjk.org.cn

echo "scale=2; 10/3" | bc
来源：http://zpx.jianghu66.top

[R29] 定义函数
来源：http://wfo.sxryk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nxk.nanxuanxn.top

[R30] 函数返回状态码
来源：http://lhr.vehdjk.com

f() { return 0; }; f || echo "失败了"
来源：http://uvw.zhoulong.xyz

[R31] 局部变量
来源：http://umj.hcnkem.com

f() { local x=1; echo "$x"; }
来源：http://nvx.chenjidiqi.icu

[R32] 参数个数校验
来源：http://eao.vqdsnc.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ajk.fehbvm.com

[R33] 捕获错误并提示行号
来源：http://mzv.daxiang520.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hjo.shanyushiyangtech.top

[R34] 退出时清理
来源：http://gcs.zycfv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://een.bjfxy.top

[R35] 后台执行并等待
来源：http://iuo.yuxming.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ehy.gotoacloud.top

[R36] 并发执行多个任务
来源：http://xlc.wangdashe.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ngq.yuxming.cn

[R37] 把输出赋给变量
来源：http://ecs.ctjpmb.com

files=$(ls -1)
来源：http://fhm.sxryk.cn

[R38] 管道串联
来源：http://gst.jqgfzy.top

cat a.txt | grep -i error | wc -l
来源：http://bhb.hongshengwenyu.top

[R39] 重定向标准输出与错误
来源：http://fkv.ivvv.top

cmd > out.log 2>&1
来源：http://aoh.gaohongyu789.top

[R40] 追加写日志
来源：http://bpg.quarkkingdee.top

echo "log" >> out.log
来源：http://tem.hnqzz.top

[R41] 丢弃输出
来源：http://klo.redwolf501.top

cmd >/dev/null 2>&1
来源：http://wbh.c1oappe.top

[R42] 输入重定向
来源：http://lfp.jinqigufen.top

wc -l < a.txt
来源：http://kwy.tarul.cn

[R43] 按名字查找文件
来源：http://nsa.yvedp.cn

find . -name "*.log" -type f
来源：http://xkt.gaohongyu789.top

[R44] 按修改时间查找
来源：http://obt.uphjek.com

find . -mtime -7 -type f
来源：http://ehu.guannengcc.top

[R45] 批量删除
来源：http://ugt.cheryme.top

find . -name "*.tmp" -delete
来源：http://uxn.zhijiandao.cn

[R46] 递归替换文件内容
来源：http://dep.birdmap.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dpw.guowangkeji.top

[R47] sed 单行替换
来源：http://dzz.uphjek.com

sed -i 's/foo/bar/g' a.txt
来源：http://qqk.yangfankeji.com

[R48] awk 取指定列
来源：http://hcs.ivvv.top

awk '{print $1, $3}' a.txt
来源：http://afq.guannengcc.top

[R49] awk 带条件
来源：http://wrz.sweek.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://drz.ppjwa.cn

[R50] awk 求和
来源：http://zxi.kuanghao11.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ufb.quarkkingdee.top

[R51] 排序去重取前几
来源：http://jxf.shzxlz.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pny.nanxinkj.top

[R52] 统计行数
来源：http://tzg.shanyushiyangkeji.top

wc -l a.txt
来源：http://uts.jinyuanbaomall.cn

[R53] 查看文件头与实时尾
来源：http://cyb.xziqi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://keu.aibaodan.cn

[R54] 比较两个文件
来源：http://dfc.zhijiandao.cn

diff a.txt b.txt
来源：http://pui.bbcook.cn

[R55] 压缩与解压
来源：http://yiw.cqqwz.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cxb.cheryme.top

[R56] 远程拷贝
来源：http://mkm.zycfv.cn

scp file user@host:/path/
来源：http://imy.zhoulong.xyz

[R57] 远程执行命令
来源：http://iae.cqqwz.cn

ssh user@host 'uptime'
来源：http://hbn.zhoulong.xyz

[R58] 下载文件
来源：http://ilz.gotoacloud.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gbj.daxiang520.top

[R59] 发 POST JSON
来源：http://vzj.yvedp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wxm.nwbrower.top

[R60] 只看 HTTP 状态码
来源：http://gwg.shuidangran.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bsf.ydjk.org.cn

[R61] 磁盘占用
来源：http://amh.jlsjyb.cn

df -h;  du -sh *
来源：http://ome.ivvv.top

[R62] 找最占空间的文件
来源：http://yrs.gaohongyu789.top

du -ah . | sort -rh | head -10
来源：http://clk.zhoulong.xyz

[R63] 内存与进程
来源：http://dus.uphjek.com

free -h;  ps aux | grep nginx
来源：http://shb.jianghu66.top

[R64] 结束进程
来源：http://ryb.quarkkingdee.top

kill -9 $(pgrep -f app.py)
来源：http://dut.hywenlv.cn

[R65] 查看端口占用
来源：http://tzc.nanxuanxn.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rtv.yuanzhike.top

[R66] 定时任务
来源：http://rsl.zdbjq.cn

crontab -e;  crontab -l
来源：http://vcz.fengsongda.top

[R67] 生成随机十六进制串
来源：http://nro.jlsjyb.cn

openssl rand -hex 16
来源：http://bzb.redwolf501.top

[R68] 计算文件校验值
来源：http://clk.tian-w.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kfl.jianghu66.top

[R69] 生成随机密码
来源：http://jwd.mhx1999.top

head -c 16 /dev/urandom | base64
来源：http://jbc.zhixingplan.top

[R70] 时间戳与互转
来源：http://vzt.yj20258888.top

date +%s;  date -d @1700000000
来源：http://qzg.kuanghao11.cn

[R71] 日期格式化
来源：http://ypt.gogol.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xyh.mhx1999.top

[R72] 等待端口就绪
来源：http://xmy.cdnleiting.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ywt.hnqzz.top

[R73] 分割大日志
来源：http://kyx.yj20258888.top

split -l 1000 big.log part_
来源：http://vtg.zhijiandao.cn

[R74] 批量重命名
来源：http://uyg.chenlongwang.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://loi.0kj1m.cn

[R75] 导出环境变量
来源：http://bem.cucudq.cn

export PATH="$HOME/bin:$PATH"
来源：http://dxv.sufxvd.cn

[R76] 使用临时文件
来源：http://nts.jinqigufen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hyh.jinqigfzy.top

[R77] 读取用户输入
来源：http://cae.fehbvm.com

read -rp "请输入: " ans
来源：http://npk.yvedp.cn

[R78] 交互式菜单
来源：http://ipf.epnwcf.com

select opt in a b c; do echo "$opt"; break; done
来源：http://wxe.haohaochexian.top

[R79] 解析命令行选项
来源：http://jhn.zycfv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yxw.xylfe.cn

[R80] 查看脚本执行耗时
来源：http://lgo.hammf.cn

time ./run.sh
来源：http://yqu.cheryme.top

================================================================================
来源：http://vck.0kj1m.cn

S. C / C++ 专题
来源：http://kvy.jyoumei.cn

================================================================================
来源：http://qqu.vqdsnc.cn

[S01] C：Hello World
来源：http://sas.ywan-chungtsiang.top

#include <stdio.h>
来源：http://xbe.zdqjudy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://smq.zhoulong.xyz

[S02] C：变量与格式化输出
来源：http://tgj.hnqzz.top

int a = 10; printf("%d\n", a);
来源：http://qeu.zhiwuduotai.top

[S03] C：读入整数
来源：http://gpo.jinqigufen.top

int x; scanf("%d", &x);
来源：http://vno.meibo888.top

[S04] C：字符串复制
来源：http://uzf.jqgufenzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://yza.tarul.cn

[S05] C：字符串长度
来源：http://iin.hongshengwenyu.top

strlen(s)
来源：http://opg.quarkkingdee.top

[S06] C：字符串比较
来源：http://gyi.zhongyouzk.top

strcmp(a, b) == 0
来源：http://tfs.cdnleiting.top

[S07] C：数组遍历求和
来源：http://yus.52xcode.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tom.9152youxi.cn

[S08] C：动态内存分配与释放
来源：http://qss.tarul.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kwv.daria6918.cn

[S09] C：结构体定义与初始化
来源：http://pvf.cqqwz.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pty.hongshengwenyu.top

[S10] C：指针与解引用
来源：http://zeq.xuetiantiany.cn

int *p = &a;  *p = 5;
来源：http://gri.jyoumei.cn

[S11] C：逐行读文件
来源：http://npn.hnxiangtu.top

FILE *f = fopen("a.txt", "r");
来源：http://zql.zhiwuduotai.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://khg.zhaomingkeji.xyz

fclose(f);
来源：http://yot.zhengqikj.top

[S12] C：写文件
来源：http://hci.hywenlv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qnc.9152youxi.cn

[S13] C：宏定义
来源：http://hks.hnqzz.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://twt.c1oappe.top

[S14] C：枚举
来源：http://xul.cdnleiting.top

enum Color { RED, GREEN, BLUE };
来源：http://whh.hammf.cn

[S15] C：类型转换
来源：http://oys.0kj1m.cn

(double) a / b
来源：http://vpa.zhengqikj.top

[S16] C：位操作置位
来源：http://ryn.jiagoushi.top

x |= (1 << 3);
来源：http://zhm.fehbvm.com

[S17] C：安全拼接字符串
来源：http://szf.svipenyu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lci.chenzaomai.com

[S18] C：命令行参数
来源：http://wai.9152youxi.cn

int main(int argc, char **argv)
来源：http://kgw.mhx1999.top

[S19] C：快速排序
来源：http://uvu.aizwys.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zbq.tarul.cn

[S20] C：二分查找
来源：http://fyx.cashguo.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yrm.aibaodan.cn

[S21] C：字符类别判断
来源：http://mvf.tanke756.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lcb.hesvh.cn

[S22] C：字符串转数字
来源：http://zdq.52xcode.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zuj.quarkkingdee.top

[S23] C：随机数
来源：http://dhg.zhixingplan.top

srand(time(NULL));  int r = rand() % 100;
来源：http://trn.zdbjq.cn

[S24] C：获取本地时间
来源：http://bsv.zhaomingkeji.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kxm.xinyue.icu

[S25] C：内存拷贝
来源：http://eyo.hammf.cn

memcpy(dst, src, n);
来源：http://fwl.zhijiandao.cn

[S26] C：内存清零
来源：http://tau.bbcook.cn

memset(a, 0, sizeof a);
来源：http://dkw.smart0.xyz

[S27] C：定义常量
来源：http://lvi.daria6918.cn

const double PI = 3.14159;
来源：http://jbv.ehwqpu.com

[S28] C：静态变量
来源：http://ikd.jinghuilouyu.cn

static int counter = 0;
来源：http://jxf.sufxvd.cn

[S29] C：变参函数
来源：http://utp.nanxinkj.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fpw.shanyushiyangtech.top

[S30] C：头文件保护
来源：http://nvg.sxryk.cn

#ifndef X_H
来源：http://gkh.xziqi.cn

#define X_H
来源：http://lgn.fanxiaobao.xyz

#endif
来源：http://ckc.aibaodan.cn

[S31] C++：Hello World
来源：http://fcu.zdbjq.cn

#include <iostream>
来源：http://eii.xziqi.cn

int main() { std::cout << "Hello\n"; }
来源：http://dcr.316326.xyz

[S32] C++：字符串
来源：http://zmt.hywenlv.cn

std::string s = "hi";  s += "!";
来源：http://znq.jinyuanbaomall.cn

[S33] C++：vector 增删
来源：http://qia.guannengcc.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xkh.shuidangran.top

[S34] C++：遍历 vector
来源：http://kbq.zhixingplan.top

for (auto &x : v) { std::cout << x; }
来源：http://wvr.pycfn.com

[S35] C++：map
来源：http://gbn.hywenlv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qct.hammf.cn

[S36] C++：unordered_map
来源：http://pqn.nanxinkj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dvs.ctjpmb.com

[S37] C++：set
来源：http://len.yuxming.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dbs.xylfe.cn

[S38] C++：排序
来源：http://bww.gzhubu.top

std::sort(v.begin(), v.end());
来源：http://knz.zhixingplan.top

[S39] C++：自定义比较器排序
来源：http://ksw.ppjwa.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gur.316326.xyz

[S40] C++：查找元素
来源：http://mmj.jyoumei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://afp.jinyuanbaomall.cn

[S41] C++：类与构造函数
来源：http://fnq.ivvv.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hbk.nwbrower.top

[S42] C++：继承与虚函数
来源：http://lef.feifeiyinyue.top

class B : public Base { public: void f() override {} };
来源：http://wng.chenjidiqi.icu

[S43] C++：智能指针
来源：http://fhj.vehdjk.com

auto p = std::make_unique<int>(5);
来源：http://pyf.cucudq.cn

[S44] C++：引用传参
来源：http://sxm.dashuyun.cn

void inc(int &x) { ++x; }
来源：http://iqs.hnqzz.top

[S45] C++：lambda
来源：http://rus.tian-w.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wwi.ehwqpu.com

[S46] C++：函数模板
来源：http://zjc.bjfxy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://acc.hysaishi.cn

[S47] C++：结构化绑定遍历
来源：http://kdp.hywenlv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ylv.sxryk.cn

[S48] C++：逐行读文件
来源：http://ldr.yanxiufei.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dzi.jinghuilouyu.cn

while (std::getline(in, line)) { }
来源：http://hqc.hesvh.cn

[S49] C++：写文件
来源：http://tnx.chenlongwang.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://umt.jianghu66.top

[S50] C++：格式化数字
来源：http://emr.yuanzhike.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rir.xuetiantiany.cn

[S51] C++：显式类型转换
来源：http://puv.andypj.xyz

static_cast<double>(a) / b
来源：http://hgb.jinghuilouyu.cn

[S52] C++：const 与 noexcept
来源：http://cku.jqgufenzy.top

int size() const noexcept { return n_; }
来源：http://ovo.havefunace.top

[S53] C++：移动语义
来源：http://wpr.cdnleiting.top

std::vector<int> w = std::move(v);
来源：http://gdg.hammf.cn

[S54] C++：异常处理
来源：http://zzd.havefunace.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cmn.guannengcc.top

[S55] C++：结构化绑定
来源：http://xtc.chenjidiqi.icu

auto [a, b] = std::make_pair(1, 2);
来源：http://ygr.sweek.top

[S56] C++：optional
来源：http://tyl.ywan-chungtsiang.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lfm.jinghuilouyu.cn

[S57] C++：编译期常量
来源：http://hbf.iojbl.cn

constexpr int N = 10;
来源：http://vfq.smart0.xyz

[S58] C++：命名空间
来源：http://zje.hcnkem.com

namespace ns { int f() { return 1; } }
来源：http://rdh.hywenlv.cn

[S59] C++：静态断言
来源：http://tfj.yvedp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wad.shanyushiyangtech.top

[S60] C++：遍历并删除元素
来源：http://kjc.chenjidiqi.icu

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yex.chenjidiqi.icu

================================================================================
来源：http://ohf.ehwqpu.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://czl.smart0.xyz

================================================================================
来源：http://cnw.shanyushiyangkeji.top

[T01] Kotlin：Hello World
来源：http://szh.ivvv.top

println("Hello")
来源：http://chu.fzhhl.top

[T02] Kotlin：变量
来源：http://oul.quarkkingdee.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kml.sysykeji.top

[T03] Kotlin：字符串模板
来源：http://yot.cucudq.cn

"值: $b"
来源：http://mev.chenjidiqi.icu

[T04] Kotlin：空安全
来源：http://kvd.sxryk.cn

val n: String? = null;  n?.length
来源：http://tkb.dashuyun.cn

[T05] Kotlin：when 表达式
来源：http://zbw.ivvv.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mhp.ydzc1.top

[T06] Kotlin：集合映射
来源：http://dme.zdbjq.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ubr.andypj.xyz

[T07] Kotlin：集合过滤
来源：http://jxr.yueranfly.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://hht.guannengcc.top

[T08] Kotlin：数据类
来源：http://gqq.9152youxi.cn

data class User(val name: String, val age: Int)
来源：http://hvo.redwolf501.top

[T09] Kotlin：扩展函数
来源：http://yji.jlsjyb.cn

fun String.exclaim() = this + "!"
来源：http://tjk.daria6918.cn

[T10] Kotlin：默认参数
来源：http://viv.yuanzhike.top

fun greet(name: String = "World") = "Hi $name"
来源：http://jaf.jyoumei.cn

[T11] Kotlin：协程
来源：http://vsu.hammf.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://thm.yangfankeji.com

[T12] Kotlin：解构声明
来源：http://lmq.hnxiangtu.top

val (a, b) = Pair(1, 2)
来源：http://nuh.xylfe.cn

[T13] Kotlin：只读 Map
来源：http://mdl.hongshengwenyu.top

val m = mapOf("a" to 1)
来源：http://iwz.jinghuilouyu.cn

[T14] Kotlin：循环
来源：http://gbz.hysaishi.cn

for (i in 1..10) println(i)
来源：http://xhh.uphjek.com

[T15] Kotlin：接口
来源：http://bej.uphjek.com

interface Shape { fun area(): Double }
来源：http://pdv.xuetiantiany.cn

[T16] Swift：Hello World
来源：http://jxh.aizwys.cn

print("Hello")
来源：http://tmz.ehwqpu.com

[T17] Swift：变量与常量
来源：http://mqr.yonumen.top

var a = 1;  let b = 2
来源：http://nbz.ywan-chungtsiang.top

[T18] Swift：字符串插值
来源：http://tur.cucudq.cn

"值: \(b)"
来源：http://ifn.guannengcc.top

[T19] Swift：可选绑定
来源：http://htq.yuxming.cn

if let n = opt { print(n) }
来源：http://rfq.gzhubu.top

[T20] Swift：数组操作
来源：http://yix.hesvh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tcz.xingfuxueyuan.xyz

[T21] Swift：遍历
来源：http://ulu.cqqwz.cn

for x in a { print(x) }
来源：http://tep.zdbjq.cn

[T22] Swift：字典
来源：http://emf.redwolf501.top

var d = ["a": 1];  d["b"] = 2
来源：http://bhz.ehwqpu.com

[T23] Swift：函数
来源：http://tdn.sxryk.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uqa.redwolf501.top

[T24] Swift：闭包
来源：http://ewy.guannengcc.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://cfx.ehwqpu.com


<!-- 参考信息 -->