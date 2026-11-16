代发 wailian999

echo "${#s}"
来源：http://pdu.wangdashe.top

[R22] 截取子串
来源：http://aky.fanxiaobao.xyz

echo "${s:0:5}"
来源：http://ruw.zhiwuduotai.top

[R23] 字符串替换
来源：http://svx.fktsv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lus.xuanzx.com

[R24] 大小写转换
来源：http://zur.zhixingplan.top

echo "${s^^}"; echo "${s,,}"
来源：http://fdc.guowangkeji.top

[R25] 去后缀 / 去前缀
来源：http://pjg.9152youxi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://uns.daria6918.cn

[R26] 命令替换
来源：http://qqr.ctjpmb.com

now=$(date +%F); echo "$now"
来源：http://tng.ppjwa.cn

[R27] 算术展开
来源：http://amp.9152youxi.cn

echo $((1 + 2 * 3))
来源：http://xmx.xziqi.cn

[R28] 浮点运算
来源：http://cln.yvedp.cn

echo "scale=2; 10/3" | bc
来源：http://xkj.vehdjk.com

[R29] 定义函数
来源：http://rjd.jinqigfzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cyy.zhaomingkeji.xyz

[R30] 函数返回状态码
来源：http://zbw.zdqjudy.top

f() { return 0; }; f || echo "失败了"
来源：http://jrr.hesvh.cn

[R31] 局部变量
来源：http://qwu.hnxiangtu.top

f() { local x=1; echo "$x"; }
来源：http://ptc.zdbjq.cn

[R32] 参数个数校验
来源：http://qws.shangyingyoupin.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sjd.snrcjt.cn

[R33] 捕获错误并提示行号
来源：http://sty.sweek.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xvx.meibo888.top

[R34] 退出时清理
来源：http://gms.fktsv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ivh.jinqigfzy.top

[R35] 后台执行并等待
来源：http://oai.aibaodan.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://alx.xuetiantiany.cn

[R36] 并发执行多个任务
来源：http://nvv.gaohongyu789.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ves.gzhubu.top

[R37] 把输出赋给变量
来源：http://kcv.svipenyu.cn

files=$(ls -1)
来源：http://mhs.zhixingplan.top

[R38] 管道串联
来源：http://iha.wangshuangyany.cn

cat a.txt | grep -i error | wc -l
来源：http://pbr.aizwys.cn

[R39] 重定向标准输出与错误
来源：http://rvq.yuxming.cn

cmd > out.log 2>&1
来源：http://knq.yonumen.top

[R40] 追加写日志
来源：http://pib.yj20258.top

echo "log" >> out.log
来源：http://kie.xziqi.cn

[R41] 丢弃输出
来源：http://fsl.chenzaomai.com

cmd >/dev/null 2>&1
来源：http://pad.xingfuxueyuan.xyz

[R42] 输入重定向
来源：http://ijp.wangdashe.top

wc -l < a.txt
来源：http://exi.guannengcc.top

[R43] 按名字查找文件
来源：http://sfs.smart0.xyz

find . -name "*.log" -type f
来源：http://iip.guowangkeji.top

[R44] 按修改时间查找
来源：http://clj.hnqzz.top

find . -mtime -7 -type f
来源：http://fip.dashuyun.cn

[R45] 批量删除
来源：http://tqh.hnxiangtu.top

find . -name "*.tmp" -delete
来源：http://fpp.bjfxy.top

[R46] 递归替换文件内容
来源：http://hst.yonumen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nxg.cdnleiting.top

[R47] sed 单行替换
来源：http://vel.jiagoushi.top

sed -i 's/foo/bar/g' a.txt
来源：http://srt.jqgfzy.top

[R48] awk 取指定列
来源：http://kah.ppjwa.cn

awk '{print $1, $3}' a.txt
来源：http://uge.jqgufenzy.top

[R49] awk 带条件
来源：http://zna.shzxlz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mah.jinqigfzy.top

[R50] awk 求和
来源：http://dfi.kuanghao11.cn

awk '{s += $2} END {print s}' a.txt
来源：http://eqx.yj20258888.top

[R51] 排序去重取前几
来源：http://qff.zhoulong.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://lfr.vehdjk.com

[R52] 统计行数
来源：http://xfr.ehwqpu.com

wc -l a.txt
来源：http://azj.zdbjq.cn

[R53] 查看文件头与实时尾
来源：http://eeo.yvedp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vzx.epnwcf.com

[R54] 比较两个文件
来源：http://kus.jiagoushi.top

diff a.txt b.txt
来源：http://rvd.hysaishi.cn

[R55] 压缩与解压
来源：http://yvo.zycfv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yyd.chenjidiqi.icu

[R56] 远程拷贝
来源：http://byp.yuanzhike.top

scp file user@host:/path/
来源：http://lqc.bbcook.cn

[R57] 远程执行命令
来源：http://fui.yvedp.cn

ssh user@host 'uptime'
来源：http://mht.cdnleiting.top

[R58] 下载文件
来源：http://vcj.nwbrower.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://abn.dianchejie.cn

[R59] 发 POST JSON
来源：http://tbg.hongshengwenyu.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xqs.zycfv.cn

[R60] 只看 HTTP 状态码
来源：http://kmw.shzxlz.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zgr.zhoulong.xyz

[R61] 磁盘占用
来源：http://emk.vehdjk.com

df -h;  du -sh *
来源：http://tia.svipenyu.cn

[R62] 找最占空间的文件
来源：http://gjh.wangdashe.top

du -ah . | sort -rh | head -10
来源：http://rok.cqqwz.cn

[R63] 内存与进程
来源：http://vmq.cheryme.top

free -h;  ps aux | grep nginx
来源：http://ogk.xziqi.cn

[R64] 结束进程
来源：http://kvz.tarul.cn

kill -9 $(pgrep -f app.py)
来源：http://rwh.yongpay.top

[R65] 查看端口占用
来源：http://bjn.jinqigufen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nwf.yanxiufei.cn

[R66] 定时任务
来源：http://nbr.epnwcf.com

crontab -e;  crontab -l
来源：http://ccz.yvedp.cn

[R67] 生成随机十六进制串
来源：http://svl.ctjpmb.com

openssl rand -hex 16
来源：http://lcn.xylfe.cn

[R68] 计算文件校验值
来源：http://fel.316326.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://rwh.daxiang520.top

[R69] 生成随机密码
来源：http://nhx.fzhhl.top

head -c 16 /dev/urandom | base64
来源：http://vby.bjfxy.top

[R70] 时间戳与互转
来源：http://jfk.daxiang520.top

date +%s;  date -d @1700000000
来源：http://ccf.kuanghao11.cn

[R71] 日期格式化
来源：http://gbe.yj202588.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jqe.hnqzz.top

[R72] 等待端口就绪
来源：http://mcp.zhiwuduotai.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ijw.zhiwuduotai.top

[R73] 分割大日志
来源：http://oan.cashguo.top

split -l 1000 big.log part_
来源：http://szc.wangdashe.top

[R74] 批量重命名
来源：http://ycm.fzhhl.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iwh.ivvv.top

[R75] 导出环境变量
来源：http://phw.chenjidiqi.icu

export PATH="$HOME/bin:$PATH"
来源：http://zeq.snrcjt.cn

[R76] 使用临时文件
来源：http://nok.ywan-chungtsiang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ear.vqdsnc.cn

[R77] 读取用户输入
来源：http://lah.tarul.cn

read -rp "请输入: " ans
来源：http://cuz.wangshuangyany.cn

[R78] 交互式菜单
来源：http://vfa.yangfankeji.com

select opt in a b c; do echo "$opt"; break; done
来源：http://uws.fanxiaobao.xyz

[R79] 解析命令行选项
来源：http://opj.svipenyu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ddt.tian-w.cn

[R80] 查看脚本执行耗时
来源：http://bmx.yj20258.top

time ./run.sh
来源：http://ubr.zhengqikj.top

================================================================================
来源：http://vcg.ybcxt.top

S. C / C++ 专题
来源：http://pot.ywan-chungtsiang.top

================================================================================
来源：http://znb.uphjek.com

[S01] C：Hello World
来源：http://dcw.tanke756.top

#include <stdio.h>
来源：http://dqj.yj202588.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://frk.zhoulong.xyz

[S02] C：变量与格式化输出
来源：http://aiw.jyoumei.cn

int a = 10; printf("%d\n", a);
来源：http://zza.chenjidiqi.icu

[S03] C：读入整数
来源：http://evx.wangshuangyany.cn

int x; scanf("%d", &x);
来源：http://dxp.jinqigufen.top

[S04] C：字符串复制
来源：http://gqm.nwbrower.top

char dst[32]; strcpy(dst, "hi");
来源：http://xao.xuanzx.com

[S05] C：字符串长度
来源：http://ess.shzxlz.cn

strlen(s)
来源：http://wdh.52xcode.cn

[S06] C：字符串比较
来源：http://ozo.gzhubu.top

strcmp(a, b) == 0
来源：http://aod.yj20258888.top

[S07] C：数组遍历求和
来源：http://psy.ybcxt.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qfj.shangyingyoupin.top

[S08] C：动态内存分配与释放
来源：http://vny.daria6918.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tdt.gaohongyu789.top

[S09] C：结构体定义与初始化
来源：http://aoa.daria6918.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://njh.xziqi.cn

[S10] C：指针与解引用
来源：http://bmo.xingfuxueyuan.xyz

int *p = &a;  *p = 5;
来源：http://tld.zhoulong.xyz

[S11] C：逐行读文件
来源：http://igo.svipenyu.cn

FILE *f = fopen("a.txt", "r");
来源：http://xij.hongshengwenyu.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://odd.vehdjk.com

fclose(f);
来源：http://dpy.sysykeji.top

[S12] C：写文件
来源：http://zbf.xuetiantiany.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yye.gogol.net.cn

[S13] C：宏定义
来源：http://lzo.fehbvm.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dji.quarkkingdee.top

[S14] C：枚举
来源：http://pvs.sjlbkw.cn

enum Color { RED, GREEN, BLUE };
来源：http://ixp.quarkkingdee.top

[S15] C：类型转换
来源：http://iic.ctjpmb.com

(double) a / b
来源：http://zsl.chenjidiqi.icu

[S16] C：位操作置位
来源：http://vyf.xingfuxueyuan.xyz

x |= (1 << 3);
来源：http://edz.yuxming.cn

[S17] C：安全拼接字符串
来源：http://scy.ivvv.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rih.shanyushiyangtech.top

[S18] C：命令行参数
来源：http://tig.chenlongwang.top

int main(int argc, char **argv)
来源：http://pnn.jinqigfzy.top

[S19] C：快速排序
来源：http://jga.daria6918.cn

qsort(a, n, sizeof(int), cmp);
来源：http://knr.shangyingyoupin.top

[S20] C：二分查找
来源：http://gvb.daxiang520.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kcm.xylfe.cn

[S21] C：字符类别判断
来源：http://tfx.fehbvm.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://spo.jiagoushi.top

[S22] C：字符串转数字
来源：http://lam.nwbrower.top

atoi("42");  strtod("3.14", NULL);
来源：http://las.xingfuxueyuan.xyz

[S23] C：随机数
来源：http://juj.ehwqpu.com

srand(time(NULL));  int r = rand() % 100;
来源：http://kjx.wangdashe.top

[S24] C：获取本地时间
来源：http://dgl.kuanghao11.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vyt.xuetiantiany.cn

[S25] C：内存拷贝
来源：http://feu.zhengqikj.top

memcpy(dst, src, n);
来源：http://rmo.hcnkem.com

[S26] C：内存清零
来源：http://rkn.hywenlv.cn

memset(a, 0, sizeof a);
来源：http://qpe.fengsongda.top

[S27] C：定义常量
来源：http://yuq.gaohongyu789.top

const double PI = 3.14159;
来源：http://okc.uphjek.com

[S28] C：静态变量
来源：http://klh.tian-w.cn

static int counter = 0;
来源：http://ltp.wangshuangyany.cn

[S29] C：变参函数
来源：http://bvx.ctjpmb.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ddx.fanxiaobao.xyz

[S30] C：头文件保护
来源：http://ncy.shuidangran.top

#ifndef X_H
来源：http://umi.316326.xyz

#define X_H
来源：http://lhv.andypj.xyz

#endif
来源：http://ojw.yj20258.top

[S31] C++：Hello World
来源：http://ywl.hnxiangtu.top

#include <iostream>
来源：http://hbl.zdbjq.cn

int main() { std::cout << "Hello\n"; }
来源：http://hxk.yj20258.top

[S32] C++：字符串
来源：http://rdg.fktsv.cn

std::string s = "hi";  s += "!";
来源：http://kpl.hnqzz.top

[S33] C++：vector 增删
来源：http://jyy.nwbrower.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xto.tianlin.xyz

[S34] C++：遍历 vector
来源：http://gvm.zhaomingkeji.xyz

for (auto &x : v) { std::cout << x; }
来源：http://ghq.yj202588.top

[S35] C++：map
来源：http://epb.ydzc1.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ysu.xuanzx.com

[S36] C++：unordered_map
来源：http://dqu.fktsv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vhf.zhongyouzk.top

[S37] C++：set
来源：http://hec.mhx1999.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://arm.yangfankeji.com

[S38] C++：排序
来源：http://lmu.yj20258.top

std::sort(v.begin(), v.end());
来源：http://sbq.hongshengwenyu.top

[S39] C++：自定义比较器排序
来源：http://xua.ydjk.org.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hkt.cucudq.cn

[S40] C++：查找元素
来源：http://yor.quarkkingdee.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ndt.iojbl.cn

[S41] C++：类与构造函数
来源：http://hph.cqqwz.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jgg.ybcxt.top

[S42] C++：继承与虚函数
来源：http://zur.yonumen.top

class B : public Base { public: void f() override {} };
来源：http://lfi.zhiwuduotai.top

[S43] C++：智能指针
来源：http://mhq.xylfe.cn

auto p = std::make_unique<int>(5);
来源：http://dqg.chenjidiqi.icu

[S44] C++：引用传参
来源：http://jif.cashguo.top

void inc(int &x) { ++x; }
来源：http://hmt.iojbl.cn

[S45] C++：lambda
来源：http://liw.xuetiantiany.cn

auto add = [](int a, int b) { return a + b; };
来源：http://oxc.yangfankeji.com

[S46] C++：函数模板
来源：http://qce.yanxiufei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lik.zhaomingkeji.xyz

[S47] C++：结构化绑定遍历
来源：http://tdj.zhaomingkeji.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kum.ybcxt.top

[S48] C++：逐行读文件
来源：http://kke.yuanzhike.top

std::ifstream in("a.txt");  std::string line;
来源：http://jph.cqqwz.cn

while (std::getline(in, line)) { }
来源：http://all.zhoulong.xyz

[S49] C++：写文件
来源：http://xvj.shanyushiyangtech.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nuf.jinyuanbaomall.cn

[S50] C++：格式化数字
来源：http://uai.cqqwz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mdi.jinghuilouyu.cn

[S51] C++：显式类型转换
来源：http://aqc.xziqi.cn

static_cast<double>(a) / b
来源：http://ots.vehdjk.com

[S52] C++：const 与 noexcept
来源：http://oxc.shangyingyoupin.top

int size() const noexcept { return n_; }
来源：http://vtg.yueranfly.top

[S53] C++：移动语义
来源：http://udm.gaohongyu789.top

std::vector<int> w = std::move(v);
来源：http://ktl.yj20258.top

[S54] C++：异常处理
来源：http://crq.snrcjt.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sce.zhongyouzk.top

[S55] C++：结构化绑定
来源：http://rjo.zhiwuduotai.top

auto [a, b] = std::make_pair(1, 2);
来源：http://svm.zhoulong.xyz

[S56] C++：optional
来源：http://rtw.0kj1m.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eqs.jqgfzy.top

[S57] C++：编译期常量
来源：http://guv.vqdsnc.cn

constexpr int N = 10;
来源：http://eva.jinqigufen.top

[S58] C++：命名空间
来源：http://oph.jianghu66.top

namespace ns { int f() { return 1; } }
来源：http://jzb.shangyingyoupin.top

[S59] C++：静态断言
来源：http://syt.zdbjq.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hrj.bjfxy.top

[S60] C++：遍历并删除元素
来源：http://jhe.shanyushiyangkeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tgx.fzhhl.top

================================================================================
来源：http://sap.jqgfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kdv.vehdjk.com

================================================================================
来源：http://wot.daxiang520.top

[T01] Kotlin：Hello World
来源：http://zbg.cashguo.top

println("Hello")
来源：http://lqp.fzhhl.top

[T02] Kotlin：变量
来源：http://zlp.zhaomingkeji.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qus.hysaishi.cn

[T03] Kotlin：字符串模板
来源：http://rkg.yanxiufei.cn

"值: $b"
来源：http://eju.ydzc1.top

[T04] Kotlin：空安全
来源：http://vrt.sweek.top

val n: String? = null;  n?.length
来源：http://kmp.fehbvm.com

[T05] Kotlin：when 表达式
来源：http://zqr.guowangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cja.chenlongwang.top

[T06] Kotlin：集合映射
来源：http://jrf.chenjidiqi.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://eoh.cucudq.cn

[T07] Kotlin：集合过滤
来源：http://xbb.jiagoushi.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://oqq.daria6918.cn

[T08] Kotlin：数据类
来源：http://zlr.jqgfzy.top

data class User(val name: String, val age: Int)
来源：http://qkq.yj20258888.top

[T09] Kotlin：扩展函数
来源：http://dod.nwbrower.top

fun String.exclaim() = this + "!"
来源：http://gqa.uphjek.com

[T10] Kotlin：默认参数
来源：http://trv.nanxinkj.top

fun greet(name: String = "World") = "Hi $name"
来源：http://zsx.kuanghao11.cn

[T11] Kotlin：协程
来源：http://urh.cdnleiting.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://hov.ydzc1.top

[T12] Kotlin：解构声明
来源：http://uul.tarul.cn

val (a, b) = Pair(1, 2)
来源：http://dnr.ehwqpu.com

[T13] Kotlin：只读 Map
来源：http://ngo.guannengcc.top

val m = mapOf("a" to 1)
来源：http://qdg.yuxming.cn

[T14] Kotlin：循环
来源：http://zib.0kj1m.cn

for (i in 1..10) println(i)
来源：http://ggx.cashguo.top

[T15] Kotlin：接口
来源：http://yar.ydjk.org.cn

interface Shape { fun area(): Double }
来源：http://zzr.chenlongwang.top

[T16] Swift：Hello World
来源：http://emt.chenjidiqi.icu

print("Hello")
来源：http://lzu.gzhubu.top

[T17] Swift：变量与常量
来源：http://cmq.yonumen.top

var a = 1;  let b = 2
来源：http://aki.xingfuxueyuan.xyz

[T18] Swift：字符串插值
来源：http://ixd.xuetiantiany.cn

"值: \(b)"
来源：http://gdl.wangdashe.top

[T19] Swift：可选绑定
来源：http://cql.pengpengdd.cyou

if let n = opt { print(n) }
来源：http://tvy.xingfuxueyuan.xyz

[T20] Swift：数组操作
来源：http://kkn.jianghu66.top

var a = [1, 2, 3];  a.append(4)
来源：http://owi.zhongyouzk.top

[T21] Swift：遍历
来源：http://wyl.mhx1999.top

for x in a { print(x) }
来源：http://mxr.fehbvm.com

[T22] Swift：字典
来源：http://fsq.nwbrower.top

var d = ["a": 1];  d["b"] = 2
来源：http://mks.jiagoushi.top

[T23] Swift：函数
来源：http://nrd.sysykeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dkv.nanxinkj.top

[T24] Swift：闭包
来源：http://zwu.snrcjt.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yqy.jianghu66.top


<!-- 参考信息 -->