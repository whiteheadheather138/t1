代发 wailian999

echo "${#arr[@]}"
来源：http://gcm.nanxinkj.top

[R20] 关联数组（字典）
来源：http://gep.yvedp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ide.feifeiyinyue.top

[R21] 字符串长度
来源：http://scs.cashguo.top

echo "${#s}"
来源：http://hfw.ctjpmb.com

[R22] 截取子串
来源：http://biw.cashguo.top

echo "${s:0:5}"
来源：http://hsr.sweek.top

[R23] 字符串替换
来源：http://fkp.cheryme.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tma.zhixingplan.top

[R24] 大小写转换
来源：http://nyu.yanxiufei.cn

echo "${s^^}"; echo "${s,,}"
来源：http://far.wangdashe.top

[R25] 去后缀 / 去前缀
来源：http://pvz.gaohongyu789.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://leb.wangdashe.top

[R26] 命令替换
来源：http://zvi.ybcxt.top

now=$(date +%F); echo "$now"
来源：http://qkf.gogol.net.cn

[R27] 算术展开
来源：http://hdt.yangfankeji.com

echo $((1 + 2 * 3))
来源：http://hwu.jinqigufen.top

[R28] 浮点运算
来源：http://gcr.fengsongda.top

echo "scale=2; 10/3" | bc
来源：http://mte.zhiwuduotai.top

[R29] 定义函数
来源：http://fss.gotoacloud.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sjc.shuidangran.top

[R30] 函数返回状态码
来源：http://sfh.sweek.top

f() { return 0; }; f || echo "失败了"
来源：http://vlz.guannengcc.top

[R31] 局部变量
来源：http://mol.chenjidiqi.icu

f() { local x=1; echo "$x"; }
来源：http://iqp.andypj.xyz

[R32] 参数个数校验
来源：http://wud.fanxiaobao.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://koe.xziqi.cn

[R33] 捕获错误并提示行号
来源：http://liz.shangyingyoupin.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bzy.andypj.xyz

[R34] 退出时清理
来源：http://cjd.tian-w.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pni.fehbvm.com

[R35] 后台执行并等待
来源：http://lww.yanxiufei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ivv.chenlongwang.top

[R36] 并发执行多个任务
来源：http://wnm.ydjk.org.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yim.jqgufenzy.top

[R37] 把输出赋给变量
来源：http://chq.ydzc1.top

files=$(ls -1)
来源：http://ndt.daria6918.cn

[R38] 管道串联
来源：http://duu.chenjidiqi.icu

cat a.txt | grep -i error | wc -l
来源：http://qte.ybcxt.top

[R39] 重定向标准输出与错误
来源：http://rmw.yuxming.cn

cmd > out.log 2>&1
来源：http://wtv.yongpay.top

[R40] 追加写日志
来源：http://bln.sweek.top

echo "log" >> out.log
来源：http://qph.ivvv.top

[R41] 丢弃输出
来源：http://hdr.dashuyun.cn

cmd >/dev/null 2>&1
来源：http://gha.meibo888.top

[R42] 输入重定向
来源：http://tzn.cashguo.top

wc -l < a.txt
来源：http://tzf.52xcode.cn

[R43] 按名字查找文件
来源：http://ycu.mhx1999.top

find . -name "*.log" -type f
来源：http://mpe.ppjwa.cn

[R44] 按修改时间查找
来源：http://gyf.sufxvd.cn

find . -mtime -7 -type f
来源：http://tfi.yj20258.top

[R45] 批量删除
来源：http://hyc.zhaomingkeji.xyz

find . -name "*.tmp" -delete
来源：http://ncc.cheryme.top

[R46] 递归替换文件内容
来源：http://uww.wangdashe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://asn.gogol.net.cn

[R47] sed 单行替换
来源：http://jwj.sweek.top

sed -i 's/foo/bar/g' a.txt
来源：http://cgt.yonumen.top

[R48] awk 取指定列
来源：http://uql.cheryme.top

awk '{print $1, $3}' a.txt
来源：http://ktk.iojbl.cn

[R49] awk 带条件
来源：http://mfr.dashuyun.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tpa.hnqzz.top

[R50] awk 求和
来源：http://tyo.9152youxi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://shv.kuanghao11.cn

[R51] 排序去重取前几
来源：http://dsf.dashuyun.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tcu.kuanghao11.cn

[R52] 统计行数
来源：http://tay.hcnkem.com

wc -l a.txt
来源：http://qmw.fengsongda.top

[R53] 查看文件头与实时尾
来源：http://euf.jqgufenzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uri.birdmap.top

[R54] 比较两个文件
来源：http://bgb.wangdashe.top

diff a.txt b.txt
来源：http://fjv.sxryk.cn

[R55] 压缩与解压
来源：http://ung.chenlongwang.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yiu.nanxuanxn.top

[R56] 远程拷贝
来源：http://jga.zdqjudy.top

scp file user@host:/path/
来源：http://ljs.hnxiangtu.top

[R57] 远程执行命令
来源：http://qrf.0kj1m.cn

ssh user@host 'uptime'
来源：http://cbq.ppjwa.cn

[R58] 下载文件
来源：http://dwu.wangshuangyany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://foq.wangdashe.top

[R59] 发 POST JSON
来源：http://ime.yangfankeji.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lqs.yangfankeji.com

[R60] 只看 HTTP 状态码
来源：http://rbo.bjfxy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uhh.cqqwz.cn

[R61] 磁盘占用
来源：http://ngp.gotoacloud.top

df -h;  du -sh *
来源：http://nai.ivvv.top

[R62] 找最占空间的文件
来源：http://nyd.feifeiyinyue.top

du -ah . | sort -rh | head -10
来源：http://cfn.yj202588.top

[R63] 内存与进程
来源：http://hlc.ydjk.org.cn

free -h;  ps aux | grep nginx
来源：http://gbu.hongshengwenyu.top

[R64] 结束进程
来源：http://qzq.fengsongda.top

kill -9 $(pgrep -f app.py)
来源：http://zdw.hnqzz.top

[R65] 查看端口占用
来源：http://khl.feifeiyinyue.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wis.hnqzz.top

[R66] 定时任务
来源：http://euk.yangfankeji.com

crontab -e;  crontab -l
来源：http://lar.ctjpmb.com

[R67] 生成随机十六进制串
来源：http://tlp.jqgfzy.top

openssl rand -hex 16
来源：http://hdp.gzhubu.top

[R68] 计算文件校验值
来源：http://ksx.ctjpmb.com

sha256sum a.txt;  md5sum a.txt
来源：http://pio.zhiwuduotai.top

[R69] 生成随机密码
来源：http://avi.sxryk.cn

head -c 16 /dev/urandom | base64
来源：http://kzr.jqgfzy.top

[R70] 时间戳与互转
来源：http://ejm.sysykeji.top

date +%s;  date -d @1700000000
来源：http://qse.ehwqpu.com

[R71] 日期格式化
来源：http://ajh.ydzc1.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://zet.cucudq.cn

[R72] 等待端口就绪
来源：http://wey.yongpay.top

until nc -z localhost 3306; do sleep 1; done
来源：http://cgl.snrcjt.cn

[R73] 分割大日志
来源：http://kij.iojbl.cn

split -l 1000 big.log part_
来源：http://eql.ydzc1.top

[R74] 批量重命名
来源：http://ocu.jlsjyb.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oae.xuanzx.com

[R75] 导出环境变量
来源：http://eup.hywenlv.cn

export PATH="$HOME/bin:$PATH"
来源：http://ayg.havefunace.top

[R76] 使用临时文件
来源：http://qyu.aibaodan.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xvk.tian-w.cn

[R77] 读取用户输入
来源：http://vmc.redwolf501.top

read -rp "请输入: " ans
来源：http://mlu.jinyuanbaomall.cn

[R78] 交互式菜单
来源：http://cpj.hammf.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://haz.guowangkeji.top

[R79] 解析命令行选项
来源：http://zrd.hywenlv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nym.quarkkingdee.top

[R80] 查看脚本执行耗时
来源：http://lnk.sjlbkw.cn

time ./run.sh
来源：http://bcm.316326.xyz

================================================================================
来源：http://cli.hywenlv.cn

S. C / C++ 专题
来源：http://kez.xuanzx.com

================================================================================
来源：http://bsk.hywenlv.cn

[S01] C：Hello World
来源：http://mdi.fehbvm.com

#include <stdio.h>
来源：http://vgs.zhengqikj.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://nzg.gaohongyu789.top

[S02] C：变量与格式化输出
来源：http://uya.xziqi.cn

int a = 10; printf("%d\n", a);
来源：http://hop.hysaishi.cn

[S03] C：读入整数
来源：http://ivq.vqdsnc.cn

int x; scanf("%d", &x);
来源：http://jyl.fanxiaobao.xyz

[S04] C：字符串复制
来源：http://zbi.0kj1m.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bwo.dianchejie.cn

[S05] C：字符串长度
来源：http://xkl.dianchejie.cn

strlen(s)
来源：http://tfz.zhongyouzk.top

[S06] C：字符串比较
来源：http://zry.jqgfzy.top

strcmp(a, b) == 0
来源：http://zrv.xuetiantiany.cn

[S07] C：数组遍历求和
来源：http://ywm.xylfe.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tbi.52xcode.cn

[S08] C：动态内存分配与释放
来源：http://tbw.redwolf501.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vas.zhijiandao.cn

[S09] C：结构体定义与初始化
来源：http://buv.ivvv.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jyu.yueranfly.top

[S10] C：指针与解引用
来源：http://svz.dashuyun.cn

int *p = &a;  *p = 5;
来源：http://wfz.xziqi.cn

[S11] C：逐行读文件
来源：http://bce.zhiwuduotai.top

FILE *f = fopen("a.txt", "r");
来源：http://lke.ivvv.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ptm.sjlbkw.cn

fclose(f);
来源：http://dyx.yj202588.top

[S12] C：写文件
来源：http://qow.aizwys.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zil.sufxvd.cn

[S13] C：宏定义
来源：http://djp.chenjidiqi.icu

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kvh.jqgufenzy.top

[S14] C：枚举
来源：http://hfs.zdqjudy.top

enum Color { RED, GREEN, BLUE };
来源：http://uyg.chenzaomai.com

[S15] C：类型转换
来源：http://uxb.xingfuxueyuan.xyz

(double) a / b
来源：http://ijq.cdnleiting.top

[S16] C：位操作置位
来源：http://fxe.dianchejie.cn

x |= (1 << 3);
来源：http://ofy.zdqjudy.top

[S17] C：安全拼接字符串
来源：http://dev.sufxvd.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pvo.haohaochexian.top

[S18] C：命令行参数
来源：http://arc.gaohongyu789.top

int main(int argc, char **argv)
来源：http://tuj.jinghuilouyu.cn

[S19] C：快速排序
来源：http://ztx.gzhubu.top

qsort(a, n, sizeof(int), cmp);
来源：http://dwx.xinyue.icu

[S20] C：二分查找
来源：http://ggv.9152youxi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wsr.jinyuanbaomall.cn

[S21] C：字符类别判断
来源：http://mut.nwbrower.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://upt.fktsv.cn

[S22] C：字符串转数字
来源：http://mxo.jianghu66.top

atoi("42");  strtod("3.14", NULL);
来源：http://cdj.tianlin.xyz

[S23] C：随机数
来源：http://zlg.jyoumei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ufo.yj20258888.top

[S24] C：获取本地时间
来源：http://nyw.ydjk.org.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zov.redwolf501.top

[S25] C：内存拷贝
来源：http://pgt.gogol.net.cn

memcpy(dst, src, n);
来源：http://irl.chenlongwang.top

[S26] C：内存清零
来源：http://jtf.jlsjyb.cn

memset(a, 0, sizeof a);
来源：http://pud.gogol.net.cn

[S27] C：定义常量
来源：http://lvl.hcnkem.com

const double PI = 3.14159;
来源：http://oto.aibaodan.cn

[S28] C：静态变量
来源：http://vls.yuxming.cn

static int counter = 0;
来源：http://wfl.dashuyun.cn

[S29] C：变参函数
来源：http://krd.shangyingyoupin.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hqz.zhoulong.xyz

[S30] C：头文件保护
来源：http://wqt.daxiang520.top

#ifndef X_H
来源：http://hcz.zhaomingkeji.xyz

#define X_H
来源：http://trc.cheryme.top

#endif
来源：http://jkr.cqqwz.cn

[S31] C++：Hello World
来源：http://kzr.shuidangran.top

#include <iostream>
来源：http://akm.zhiwuduotai.top

int main() { std::cout << "Hello\n"; }
来源：http://xjl.hfpthk.cn

[S32] C++：字符串
来源：http://ryl.pycfn.com

std::string s = "hi";  s += "!";
来源：http://eur.yfazqb.com

[S33] C++：vector 增删
来源：http://hsp.yfazqb.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bri.bjfxy.top

[S34] C++：遍历 vector
来源：http://qob.zhongyouzk.top

for (auto &x : v) { std::cout << x; }
来源：http://qgo.jqgfzy.top

[S35] C++：map
来源：http://lwh.chenzaomai.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yht.daxiang520.top

[S36] C++：unordered_map
来源：http://orl.hysaishi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jzq.mhx1999.top

[S37] C++：set
来源：http://qqe.zdqjudy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kqy.aizwys.cn

[S38] C++：排序
来源：http://hog.ydjk.org.cn

std::sort(v.begin(), v.end());
来源：http://wxw.meibo888.top

[S39] C++：自定义比较器排序
来源：http://kgp.tarul.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xye.cdnleiting.top

[S40] C++：查找元素
来源：http://gdt.hfpthk.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kbs.0kj1m.cn

[S41] C++：类与构造函数
来源：http://hco.shzxlz.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qpx.cdnleiting.top

[S42] C++：继承与虚函数
来源：http://ylj.xuetiantiany.cn

class B : public Base { public: void f() override {} };
来源：http://yhq.andypj.xyz

[S43] C++：智能指针
来源：http://qrx.aibaodan.cn

auto p = std::make_unique<int>(5);
来源：http://puu.yongpay.top

[S44] C++：引用传参
来源：http://opk.yuxming.cn

void inc(int &x) { ++x; }
来源：http://nek.ctjpmb.com

[S45] C++：lambda
来源：http://nmm.chenjidiqi.icu

auto add = [](int a, int b) { return a + b; };
来源：http://prq.svipenyu.cn

[S46] C++：函数模板
来源：http://mru.hnqzz.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ndd.sufxvd.cn

[S47] C++：结构化绑定遍历
来源：http://ivl.zhongyouzk.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gpk.hysaishi.cn

[S48] C++：逐行读文件
来源：http://grd.c1oappe.top

std::ifstream in("a.txt");  std::string line;
来源：http://bsp.epnwcf.com

while (std::getline(in, line)) { }
来源：http://klh.ctjpmb.com

[S49] C++：写文件
来源：http://ztw.cashguo.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ctp.zhongyouzk.top

[S50] C++：格式化数字
来源：http://pvp.yuxming.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bnq.jianghu66.top

[S51] C++：显式类型转换
来源：http://ier.chenzaomai.com

static_cast<double>(a) / b
来源：http://kpk.sjlbkw.cn

[S52] C++：const 与 noexcept
来源：http://kxp.jqgfzy.top

int size() const noexcept { return n_; }
来源：http://gwt.zhiwuduotai.top

[S53] C++：移动语义
来源：http://yfu.fengsongda.top

std::vector<int> w = std::move(v);
来源：http://vur.sysykeji.top

[S54] C++：异常处理
来源：http://rcr.iojbl.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xrg.aibaodan.cn

[S55] C++：结构化绑定
来源：http://yyp.sufxvd.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://agl.yongpay.top

[S56] C++：optional
来源：http://uqs.yj20258.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wzd.c1oappe.top

[S57] C++：编译期常量
来源：http://lnk.hnqzz.top

constexpr int N = 10;
来源：http://nwn.cqqwz.cn

[S58] C++：命名空间
来源：http://xfy.redwolf501.top

namespace ns { int f() { return 1; } }
来源：http://jxs.redwolf501.top

[S59] C++：静态断言
来源：http://srf.mhx1999.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jpa.nanxuanxn.top

[S60] C++：遍历并删除元素
来源：http://rew.sufxvd.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ahm.xziqi.cn

================================================================================
来源：http://plo.uphjek.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xxe.shanyushiyangtech.top

================================================================================
来源：http://lou.hesvh.cn

[T01] Kotlin：Hello World
来源：http://alk.cheryme.top

println("Hello")
来源：http://zji.fzhhl.top

[T02] Kotlin：变量
来源：http://mzy.ivvv.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://chv.chenzaomai.com

[T03] Kotlin：字符串模板
来源：http://got.hywenlv.cn

"值: $b"
来源：http://kei.hnqzz.top

[T04] Kotlin：空安全
来源：http://ehw.ctjpmb.com

val n: String? = null;  n?.length
来源：http://gsx.yanxiufei.cn

[T05] Kotlin：when 表达式
来源：http://iyl.haohaochexian.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://plc.dashuyun.cn

[T06] Kotlin：集合映射
来源：http://qjl.bjfxy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jsm.cdnleiting.top

[T07] Kotlin：集合过滤
来源：http://vgj.meibo888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://svh.cucudq.cn

[T08] Kotlin：数据类
来源：http://zyd.fanxiaobao.xyz

data class User(val name: String, val age: Int)
来源：http://cin.cdnleiting.top

[T09] Kotlin：扩展函数
来源：http://xfo.yuxming.cn

fun String.exclaim() = this + "!"
来源：http://ybt.xylfe.cn

[T10] Kotlin：默认参数
来源：http://bny.chenzaomai.com

fun greet(name: String = "World") = "Hi $name"
来源：http://jwk.mhx1999.top

[T11] Kotlin：协程
来源：http://xcs.zhixingplan.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://low.nwbrower.top

[T12] Kotlin：解构声明
来源：http://bdj.52xcode.cn

val (a, b) = Pair(1, 2)
来源：http://nzd.vehdjk.com

[T13] Kotlin：只读 Map
来源：http://moo.pycfn.com

val m = mapOf("a" to 1)
来源：http://tdc.nanxuanxn.top

[T14] Kotlin：循环
来源：http://sgq.yvedp.cn

for (i in 1..10) println(i)
来源：http://pph.ywan-chungtsiang.top

[T15] Kotlin：接口
来源：http://qjk.jlsjyb.cn

interface Shape { fun area(): Double }
来源：http://rhh.wangdashe.top

[T16] Swift：Hello World
来源：http://mwu.quarkkingdee.top

print("Hello")
来源：http://zxx.zhoulong.xyz

[T17] Swift：变量与常量
来源：http://zqp.yongpay.top

var a = 1;  let b = 2
来源：http://fwz.zdbjq.cn

[T18] Swift：字符串插值
来源：http://oxh.shzxlz.cn

"值: \(b)"
来源：http://cyg.meibo888.top

[T19] Swift：可选绑定
来源：http://wrx.kuanghao11.cn

if let n = opt { print(n) }
来源：http://lgu.xinyue.icu

[T20] Swift：数组操作
来源：http://nai.havefunace.top

var a = [1, 2, 3];  a.append(4)
来源：http://oah.cashguo.top

[T21] Swift：遍历
来源：http://crc.jianghu66.top

for x in a { print(x) }
来源：http://rrh.xuanzx.com

[T22] Swift：字典
来源：http://mdl.cheryme.top

var d = ["a": 1];  d["b"] = 2
来源：http://zah.yanxiufei.cn


<!-- 参考信息 -->