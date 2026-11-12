代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://trg.birdmap.top

[R18] 遍历数组
来源：http://izw.guowangkeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lqj.hcnkem.com

[R19] 数组长度
来源：http://hwi.guannengcc.top

echo "${#arr[@]}"
来源：http://nci.yongpay.top

[R20] 关联数组（字典）
来源：http://uhf.mhx1999.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jaz.9152youxi.cn

[R21] 字符串长度
来源：http://hih.zhixingplan.top

echo "${#s}"
来源：http://knp.tarul.cn

[R22] 截取子串
来源：http://qyv.jinyuanbaomall.cn

echo "${s:0:5}"
来源：http://ftp.yvedp.cn

[R23] 字符串替换
来源：http://syk.dianchejie.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vnu.yfazqb.com

[R24] 大小写转换
来源：http://ehd.redwolf501.top

echo "${s^^}"; echo "${s,,}"
来源：http://ftf.birdmap.top

[R25] 去后缀 / 去前缀
来源：http://jxn.fktsv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://wdx.jianghu66.top

[R26] 命令替换
来源：http://ikd.bbcook.cn

now=$(date +%F); echo "$now"
来源：http://mqi.shzxlz.cn

[R27] 算术展开
来源：http://odo.svipenyu.cn

echo $((1 + 2 * 3))
来源：http://puq.jinghuilouyu.cn

[R28] 浮点运算
来源：http://gtv.guowangkeji.top

echo "scale=2; 10/3" | bc
来源：http://hdp.c1oappe.top

[R29] 定义函数
来源：http://soz.gzhubu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dtm.hnqzz.top

[R30] 函数返回状态码
来源：http://ktn.ivvv.top

f() { return 0; }; f || echo "失败了"
来源：http://wbj.zhijiandao.cn

[R31] 局部变量
来源：http://cgn.uphjek.com

f() { local x=1; echo "$x"; }
来源：http://bbf.hnqzz.top

[R32] 参数个数校验
来源：http://gsy.hywenlv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jky.gzhubu.top

[R33] 捕获错误并提示行号
来源：http://aui.ywan-chungtsiang.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rcf.jinyuanbaomall.cn

[R34] 退出时清理
来源：http://boh.jianghu66.top

trap 'rm -f "$tmp"' EXIT
来源：http://xzc.jyoumei.cn

[R35] 后台执行并等待
来源：http://rik.yueranfly.top

sleep 5 & pid=$!; wait "$pid"
来源：http://zhc.zhixingplan.top

[R36] 并发执行多个任务
来源：http://wnv.quarkkingdee.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hpo.jqgfzy.top

[R37] 把输出赋给变量
来源：http://kga.redwolf501.top

files=$(ls -1)
来源：http://mcx.ydjk.org.cn

[R38] 管道串联
来源：http://sbf.meibo888.top

cat a.txt | grep -i error | wc -l
来源：http://mgp.xziqi.cn

[R39] 重定向标准输出与错误
来源：http://igi.jqgufenzy.top

cmd > out.log 2>&1
来源：http://tgj.jqgfzy.top

[R40] 追加写日志
来源：http://apj.ppjwa.cn

echo "log" >> out.log
来源：http://rho.fktsv.cn

[R41] 丢弃输出
来源：http://sac.ybcxt.top

cmd >/dev/null 2>&1
来源：http://khc.zhixingplan.top

[R42] 输入重定向
来源：http://ksj.cdnleiting.top

wc -l < a.txt
来源：http://ysd.fengsongda.top

[R43] 按名字查找文件
来源：http://dyx.uphjek.com

find . -name "*.log" -type f
来源：http://kgu.jinqigufen.top

[R44] 按修改时间查找
来源：http://lwa.fengsongda.top

find . -mtime -7 -type f
来源：http://uaa.ivvv.top

[R45] 批量删除
来源：http://xbr.fehbvm.com

find . -name "*.tmp" -delete
来源：http://oil.ppjwa.cn

[R46] 递归替换文件内容
来源：http://suj.feifeiyinyue.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://svb.ppjwa.cn

[R47] sed 单行替换
来源：http://znf.chenlongwang.top

sed -i 's/foo/bar/g' a.txt
来源：http://ixg.gogol.net.cn

[R48] awk 取指定列
来源：http://rjp.chenzaomai.com

awk '{print $1, $3}' a.txt
来源：http://qfi.52xcode.cn

[R49] awk 带条件
来源：http://nmi.sufxvd.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://trw.hysaishi.cn

[R50] awk 求和
来源：http://hfb.chenzaomai.com

awk '{s += $2} END {print s}' a.txt
来源：http://sbu.hywenlv.cn

[R51] 排序去重取前几
来源：http://vul.chenlongwang.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ipn.fzhhl.top

[R52] 统计行数
来源：http://sjf.shzxlz.cn

wc -l a.txt
来源：http://bjd.chenlongwang.top

[R53] 查看文件头与实时尾
来源：http://fgx.zhengqikj.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lvz.hysaishi.cn

[R54] 比较两个文件
来源：http://jtw.aibaodan.cn

diff a.txt b.txt
来源：http://jkt.316326.xyz

[R55] 压缩与解压
来源：http://ptv.tarul.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://odx.jyoumei.cn

[R56] 远程拷贝
来源：http://for.yanxiufei.cn

scp file user@host:/path/
来源：http://upa.gzhubu.top

[R57] 远程执行命令
来源：http://qli.aizwys.cn

ssh user@host 'uptime'
来源：http://myg.sysykeji.top

[R58] 下载文件
来源：http://ghw.cucudq.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://svy.chenlongwang.top

[R59] 发 POST JSON
来源：http://sdt.ydzc1.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hix.yonumen.top

[R60] 只看 HTTP 状态码
来源：http://qqr.zhoulong.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vxg.gzhubu.top

[R61] 磁盘占用
来源：http://zrr.yonumen.top

df -h;  du -sh *
来源：http://lqu.fktsv.cn

[R62] 找最占空间的文件
来源：http://pgj.xylfe.cn

du -ah . | sort -rh | head -10
来源：http://cid.epnwcf.com

[R63] 内存与进程
来源：http://hue.xuetiantiany.cn

free -h;  ps aux | grep nginx
来源：http://pzg.bbcook.cn

[R64] 结束进程
来源：http://oly.9152youxi.cn

kill -9 $(pgrep -f app.py)
来源：http://xhq.hysaishi.cn

[R65] 查看端口占用
来源：http://mqx.zhixingplan.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qma.jyoumei.cn

[R66] 定时任务
来源：http://ldx.yangfankeji.com

crontab -e;  crontab -l
来源：http://jti.hongshengwenyu.top

[R67] 生成随机十六进制串
来源：http://gvf.gotoacloud.top

openssl rand -hex 16
来源：http://vqw.ppjwa.cn

[R68] 计算文件校验值
来源：http://wnv.shuidangran.top

sha256sum a.txt;  md5sum a.txt
来源：http://nbu.tian-w.cn

[R69] 生成随机密码
来源：http://fke.fanxiaobao.xyz

head -c 16 /dev/urandom | base64
来源：http://mqn.yuxming.cn

[R70] 时间戳与互转
来源：http://nqn.mhx1999.top

date +%s;  date -d @1700000000
来源：http://vym.hnxiangtu.top

[R71] 日期格式化
来源：http://svd.ybcxt.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://thh.xuetiantiany.cn

[R72] 等待端口就绪
来源：http://dha.yj202588.top

until nc -z localhost 3306; do sleep 1; done
来源：http://mwz.zhoulong.xyz

[R73] 分割大日志
来源：http://zrg.dashuyun.cn

split -l 1000 big.log part_
来源：http://zsz.0kj1m.cn

[R74] 批量重命名
来源：http://ckr.bjfxy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iwf.xziqi.cn

[R75] 导出环境变量
来源：http://ysx.tanke756.top

export PATH="$HOME/bin:$PATH"
来源：http://dxz.hywenlv.cn

[R76] 使用临时文件
来源：http://dor.shanyushiyangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mhr.hnxiangtu.top

[R77] 读取用户输入
来源：http://lzz.hammf.cn

read -rp "请输入: " ans
来源：http://tfe.pengpengdd.cyou

[R78] 交互式菜单
来源：http://bxc.andypj.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://gui.ivvv.top

[R79] 解析命令行选项
来源：http://bxn.vqdsnc.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tax.yvedp.cn

[R80] 查看脚本执行耗时
来源：http://zai.hfpthk.cn

time ./run.sh
来源：http://eug.9152youxi.cn

================================================================================
来源：http://rcr.ydjk.org.cn

S. C / C++ 专题
来源：http://yds.jianghu66.top

================================================================================
来源：http://dyp.guannengcc.top

[S01] C：Hello World
来源：http://ujp.yanxiufei.cn

#include <stdio.h>
来源：http://eax.tanke756.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xmt.sufxvd.cn

[S02] C：变量与格式化输出
来源：http://snm.yuanzhike.top

int a = 10; printf("%d\n", a);
来源：http://rbq.snrcjt.cn

[S03] C：读入整数
来源：http://kar.zhixingplan.top

int x; scanf("%d", &x);
来源：http://gub.bbcook.cn

[S04] C：字符串复制
来源：http://nzs.tianlin.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://roc.jinqigufen.top

[S05] C：字符串长度
来源：http://ata.yj20258.top

strlen(s)
来源：http://tez.bbcook.cn

[S06] C：字符串比较
来源：http://pqs.kuanghao11.cn

strcmp(a, b) == 0
来源：http://bkg.zycfv.cn

[S07] C：数组遍历求和
来源：http://rjl.jinqigfzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sux.hcnkem.com

[S08] C：动态内存分配与释放
来源：http://axh.guannengcc.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hxp.chenlongwang.top

[S09] C：结构体定义与初始化
来源：http://lgt.9152youxi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qsv.0kj1m.cn

[S10] C：指针与解引用
来源：http://dbp.sysykeji.top

int *p = &a;  *p = 5;
来源：http://xff.snrcjt.cn

[S11] C：逐行读文件
来源：http://zca.epnwcf.com

FILE *f = fopen("a.txt", "r");
来源：http://ony.0kj1m.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ixz.52xcode.cn

fclose(f);
来源：http://lyh.tanke756.top

[S12] C：写文件
来源：http://hfo.zhengqikj.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tsc.sweek.top

[S13] C：宏定义
来源：http://hmq.yuanzhike.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fza.hammf.cn

[S14] C：枚举
来源：http://rgy.hywenlv.cn

enum Color { RED, GREEN, BLUE };
来源：http://qie.xziqi.cn

[S15] C：类型转换
来源：http://slb.xylfe.cn

(double) a / b
来源：http://sle.zycfv.cn

[S16] C：位操作置位
来源：http://xzj.jiagoushi.top

x |= (1 << 3);
来源：http://wwm.xziqi.cn

[S17] C：安全拼接字符串
来源：http://pwd.ctjpmb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tfa.hysaishi.cn

[S18] C：命令行参数
来源：http://kpd.sysykeji.top

int main(int argc, char **argv)
来源：http://hxb.sufxvd.cn

[S19] C：快速排序
来源：http://eqv.yj20258.top

qsort(a, n, sizeof(int), cmp);
来源：http://chp.jyoumei.cn

[S20] C：二分查找
来源：http://trj.aibaodan.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yea.chenjidiqi.icu

[S21] C：字符类别判断
来源：http://fkq.xuanzx.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://evi.xziqi.cn

[S22] C：字符串转数字
来源：http://arb.guowangkeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://iuf.ywan-chungtsiang.top

[S23] C：随机数
来源：http://nkv.wangdashe.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ztr.wangdashe.top

[S24] C：获取本地时间
来源：http://wbk.yj202588.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ktj.yfazqb.com

[S25] C：内存拷贝
来源：http://xsn.ppjwa.cn

memcpy(dst, src, n);
来源：http://dzi.aibaodan.cn

[S26] C：内存清零
来源：http://cny.tarul.cn

memset(a, 0, sizeof a);
来源：http://ohy.ywan-chungtsiang.top

[S27] C：定义常量
来源：http://abr.havefunace.top

const double PI = 3.14159;
来源：http://yrb.jinqigufen.top

[S28] C：静态变量
来源：http://lnp.hfpthk.cn

static int counter = 0;
来源：http://pwd.snrcjt.cn

[S29] C：变参函数
来源：http://gbx.shzxlz.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kkt.guannengcc.top

[S30] C：头文件保护
来源：http://fyt.316326.xyz

#ifndef X_H
来源：http://eus.gzhubu.top

#define X_H
来源：http://boj.yongpay.top

#endif
来源：http://wgy.bbcook.cn

[S31] C++：Hello World
来源：http://yis.yanxiufei.cn

#include <iostream>
来源：http://ckx.jiagoushi.top

int main() { std::cout << "Hello\n"; }
来源：http://vzw.xuanzx.com

[S32] C++：字符串
来源：http://yyp.zhengqikj.top

std::string s = "hi";  s += "!";
来源：http://oqk.gzhubu.top

[S33] C++：vector 增删
来源：http://xwi.haohaochexian.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fox.cheryme.top

[S34] C++：遍历 vector
来源：http://bjf.nanxuanxn.top

for (auto &x : v) { std::cout << x; }
来源：http://ajh.xingfuxueyuan.xyz

[S35] C++：map
来源：http://chw.hongshengwenyu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zad.tianlin.xyz

[S36] C++：unordered_map
来源：http://fcd.wangshuangyany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://slo.pengpengdd.cyou

[S37] C++：set
来源：http://aqd.yonumen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xvi.sweek.top

[S38] C++：排序
来源：http://tkr.jinghuilouyu.cn

std::sort(v.begin(), v.end());
来源：http://kjy.mhx1999.top

[S39] C++：自定义比较器排序
来源：http://crb.shzxlz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://doz.gzhubu.top

[S40] C++：查找元素
来源：http://ami.zhengqikj.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jls.52xcode.cn

[S41] C++：类与构造函数
来源：http://hfz.cheryme.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://syt.nanxuanxn.top

[S42] C++：继承与虚函数
来源：http://nec.meibo888.top

class B : public Base { public: void f() override {} };
来源：http://icw.iojbl.cn

[S43] C++：智能指针
来源：http://blk.wangshuangyany.cn

auto p = std::make_unique<int>(5);
来源：http://pot.ydjk.org.cn

[S44] C++：引用传参
来源：http://brk.chenjidiqi.icu

void inc(int &x) { ++x; }
来源：http://hhg.cashguo.top

[S45] C++：lambda
来源：http://dyg.xziqi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jtj.fehbvm.com

[S46] C++：函数模板
来源：http://cfj.yongpay.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kmf.dianchejie.cn

[S47] C++：结构化绑定遍历
来源：http://kbv.meibo888.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ibr.jianghu66.top

[S48] C++：逐行读文件
来源：http://hbc.zhongyouzk.top

std::ifstream in("a.txt");  std::string line;
来源：http://wqy.tian-w.cn

while (std::getline(in, line)) { }
来源：http://jmb.hesvh.cn

[S49] C++：写文件
来源：http://spq.yanxiufei.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vlk.sjlbkw.cn

[S50] C++：格式化数字
来源：http://xcv.jqgfzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pht.guowangkeji.top

[S51] C++：显式类型转换
来源：http://qca.fehbvm.com

static_cast<double>(a) / b
来源：http://hwr.zdqjudy.top

[S52] C++：const 与 noexcept
来源：http://vbw.shangyingyoupin.top

int size() const noexcept { return n_; }
来源：http://tqu.xuetiantiany.cn

[S53] C++：移动语义
来源：http://ljm.ctjpmb.com

std::vector<int> w = std::move(v);
来源：http://dzy.smart0.xyz

[S54] C++：异常处理
来源：http://nsi.shangyingyoupin.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tls.zdqjudy.top

[S55] C++：结构化绑定
来源：http://usx.fktsv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://you.zhixingplan.top

[S56] C++：optional
来源：http://cet.bbcook.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jfl.yuxming.cn

[S57] C++：编译期常量
来源：http://vki.hongshengwenyu.top

constexpr int N = 10;
来源：http://izh.ivvv.top

[S58] C++：命名空间
来源：http://lgj.tianlin.xyz

namespace ns { int f() { return 1; } }
来源：http://bdt.shuidangran.top

[S59] C++：静态断言
来源：http://wod.nanxuanxn.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rcx.aizwys.cn

[S60] C++：遍历并删除元素
来源：http://fcc.cashguo.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xsk.havefunace.top

================================================================================
来源：http://nbd.guowangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hyd.kuanghao11.cn

================================================================================
来源：http://sqm.aizwys.cn

[T01] Kotlin：Hello World
来源：http://otg.hnqzz.top

println("Hello")
来源：http://nkp.gogol.net.cn

[T02] Kotlin：变量
来源：http://ekg.wangdashe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cyi.zhixingplan.top

[T03] Kotlin：字符串模板
来源：http://jjv.daxiang520.top

"值: $b"
来源：http://ozj.hesvh.cn

[T04] Kotlin：空安全
来源：http://fwq.zhaomingkeji.xyz

val n: String? = null;  n?.length
来源：http://bnh.cashguo.top

[T05] Kotlin：when 表达式
来源：http://odd.shanyushiyangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://opj.bbcook.cn

[T06] Kotlin：集合映射
来源：http://eyf.bbcook.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ajn.fanxiaobao.xyz

[T07] Kotlin：集合过滤
来源：http://qup.ivvv.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://srk.shzxlz.cn

[T08] Kotlin：数据类
来源：http://zps.ctjpmb.com

data class User(val name: String, val age: Int)
来源：http://sjv.gaohongyu789.top

[T09] Kotlin：扩展函数
来源：http://ffw.tanke756.top

fun String.exclaim() = this + "!"
来源：http://sbm.hesvh.cn

[T10] Kotlin：默认参数
来源：http://onn.bjfxy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://zwu.yueranfly.top

[T11] Kotlin：协程
来源：http://tha.cucudq.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cse.jiagoushi.top

[T12] Kotlin：解构声明
来源：http://sfr.shanyushiyangtech.top

val (a, b) = Pair(1, 2)
来源：http://vjo.epnwcf.com

[T13] Kotlin：只读 Map
来源：http://mqt.52xcode.cn

val m = mapOf("a" to 1)
来源：http://gxh.smart0.xyz

[T14] Kotlin：循环
来源：http://wne.zhaomingkeji.xyz

for (i in 1..10) println(i)
来源：http://lmc.smart0.xyz

[T15] Kotlin：接口
来源：http://uov.nwbrower.top

interface Shape { fun area(): Double }
来源：http://oit.fzhhl.top

[T16] Swift：Hello World
来源：http://cqa.zhoulong.xyz

print("Hello")
来源：http://sjz.uphjek.com

[T17] Swift：变量与常量
来源：http://sgg.haohaochexian.top

var a = 1;  let b = 2
来源：http://ojn.yj20258.top

[T18] Swift：字符串插值
来源：http://dtn.fzhhl.top

"值: \(b)"
来源：http://hfc.fzhhl.top

[T19] Swift：可选绑定
来源：http://iuz.ctjpmb.com

if let n = opt { print(n) }
来源：http://kca.aibaodan.cn

[T20] Swift：数组操作
来源：http://uas.guowangkeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://qdr.xuetiantiany.cn


<!-- 参考信息 -->