代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bmh.c1oappe.top

[R16] until 等待条件
来源：http://vbn.hfpthk.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ukn.hongshengwenyu.top

[R17] 数组定义与取值
来源：http://ylk.xingfuxueyuan.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://nxi.iojbl.cn

[R18] 遍历数组
来源：http://dcu.gzhubu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kgd.daria6918.cn

[R19] 数组长度
来源：http://gvc.tian-w.cn

echo "${#arr[@]}"
来源：http://lkp.daria6918.cn

[R20] 关联数组（字典）
来源：http://sck.fktsv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xis.vehdjk.com

[R21] 字符串长度
来源：http://shi.shangyingyoupin.top

echo "${#s}"
来源：http://khl.birdmap.top

[R22] 截取子串
来源：http://rkw.zhengqikj.top

echo "${s:0:5}"
来源：http://wfj.zhiwuduotai.top

[R23] 字符串替换
来源：http://wlk.jinqigufen.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yqn.redwolf501.top

[R24] 大小写转换
来源：http://mpz.gzhubu.top

echo "${s^^}"; echo "${s,,}"
来源：http://ehx.pengpengdd.cyou

[R25] 去后缀 / 去前缀
来源：http://gqv.jqgfzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://bgi.c1oappe.top

[R26] 命令替换
来源：http://ofa.hysaishi.cn

now=$(date +%F); echo "$now"
来源：http://wtl.hesvh.cn

[R27] 算术展开
来源：http://hwf.yj20258.top

echo $((1 + 2 * 3))
来源：http://jzn.hfpthk.cn

[R28] 浮点运算
来源：http://cdv.zhixingplan.top

echo "scale=2; 10/3" | bc
来源：http://jol.uphjek.com

[R29] 定义函数
来源：http://tcb.xuanzx.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gku.meibo888.top

[R30] 函数返回状态码
来源：http://jhc.gzhubu.top

f() { return 0; }; f || echo "失败了"
来源：http://cxz.cqqwz.cn

[R31] 局部变量
来源：http://amf.sysykeji.top

f() { local x=1; echo "$x"; }
来源：http://afz.yj20258.top

[R32] 参数个数校验
来源：http://bel.fzhhl.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lwc.pengpengdd.cyou

[R33] 捕获错误并提示行号
来源：http://jdi.jqgfzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://abi.svipenyu.cn

[R34] 退出时清理
来源：http://jhj.fktsv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zad.xingfuxueyuan.xyz

[R35] 后台执行并等待
来源：http://rga.hysaishi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fwu.xuanzx.com

[R36] 并发执行多个任务
来源：http://ohu.shanyushiyangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xwo.tanke756.top

[R37] 把输出赋给变量
来源：http://cpr.zhixingplan.top

files=$(ls -1)
来源：http://pzb.shanyushiyangkeji.top

[R38] 管道串联
来源：http://qpp.bbcook.cn

cat a.txt | grep -i error | wc -l
来源：http://maj.zdqjudy.top

[R39] 重定向标准输出与错误
来源：http://pbb.c1oappe.top

cmd > out.log 2>&1
来源：http://nzt.zdqjudy.top

[R40] 追加写日志
来源：http://rup.yonumen.top

echo "log" >> out.log
来源：http://yvi.shuidangran.top

[R41] 丢弃输出
来源：http://hqm.cheryme.top

cmd >/dev/null 2>&1
来源：http://tvv.gaohongyu789.top

[R42] 输入重定向
来源：http://kjn.cucudq.cn

wc -l < a.txt
来源：http://kty.vehdjk.com

[R43] 按名字查找文件
来源：http://tau.zhongyouzk.top

find . -name "*.log" -type f
来源：http://vsw.vehdjk.com

[R44] 按修改时间查找
来源：http://pmz.yj20258888.top

find . -mtime -7 -type f
来源：http://hqa.fanxiaobao.xyz

[R45] 批量删除
来源：http://ewx.iojbl.cn

find . -name "*.tmp" -delete
来源：http://xzu.fehbvm.com

[R46] 递归替换文件内容
来源：http://gjc.cucudq.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wki.hywenlv.cn

[R47] sed 单行替换
来源：http://hss.ppjwa.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fit.zdqjudy.top

[R48] awk 取指定列
来源：http://cbr.jinyuanbaomall.cn

awk '{print $1, $3}' a.txt
来源：http://hcl.jinqigfzy.top

[R49] awk 带条件
来源：http://xjc.cashguo.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://odx.sufxvd.cn

[R50] awk 求和
来源：http://rms.zhoulong.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://ugn.cqqwz.cn

[R51] 排序去重取前几
来源：http://bsw.bbcook.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pnf.jlsjyb.cn

[R52] 统计行数
来源：http://rvm.hfpthk.cn

wc -l a.txt
来源：http://crt.zhiwuduotai.top

[R53] 查看文件头与实时尾
来源：http://csa.bbcook.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qld.pengpengdd.cyou

[R54] 比较两个文件
来源：http://weq.nanxinkj.top

diff a.txt b.txt
来源：http://zpp.wangdashe.top

[R55] 压缩与解压
来源：http://kfu.yonumen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lfa.hnxiangtu.top

[R56] 远程拷贝
来源：http://xij.yfazqb.com

scp file user@host:/path/
来源：http://tea.fehbvm.com

[R57] 远程执行命令
来源：http://lld.mhx1999.top

ssh user@host 'uptime'
来源：http://dos.feifeiyinyue.top

[R58] 下载文件
来源：http://vqc.pengpengdd.cyou

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vkm.shuidangran.top

[R59] 发 POST JSON
来源：http://bjo.yueranfly.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tgd.andypj.xyz

[R60] 只看 HTTP 状态码
来源：http://ixr.c1oappe.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yyl.hnqzz.top

[R61] 磁盘占用
来源：http://dvh.zhiwuduotai.top

df -h;  du -sh *
来源：http://vpe.yj20258888.top

[R62] 找最占空间的文件
来源：http://xbj.redwolf501.top

du -ah . | sort -rh | head -10
来源：http://ovn.shanyushiyangtech.top

[R63] 内存与进程
来源：http://yci.havefunace.top

free -h;  ps aux | grep nginx
来源：http://wvq.iojbl.cn

[R64] 结束进程
来源：http://jbv.aibaodan.cn

kill -9 $(pgrep -f app.py)
来源：http://wox.hysaishi.cn

[R65] 查看端口占用
来源：http://lku.yonumen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://htr.zdbjq.cn

[R66] 定时任务
来源：http://fqn.svipenyu.cn

crontab -e;  crontab -l
来源：http://scr.svipenyu.cn

[R67] 生成随机十六进制串
来源：http://qcy.pycfn.com

openssl rand -hex 16
来源：http://dbx.yonumen.top

[R68] 计算文件校验值
来源：http://rbj.jinqigfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://gih.xuanzx.com

[R69] 生成随机密码
来源：http://nbu.havefunace.top

head -c 16 /dev/urandom | base64
来源：http://rga.xingfuxueyuan.xyz

[R70] 时间戳与互转
来源：http://ihc.zdqjudy.top

date +%s;  date -d @1700000000
来源：http://jxe.316326.xyz

[R71] 日期格式化
来源：http://ddk.svipenyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://srh.jinghuilouyu.cn

[R72] 等待端口就绪
来源：http://iew.wangshuangyany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bsw.316326.xyz

[R73] 分割大日志
来源：http://adi.ydjk.org.cn

split -l 1000 big.log part_
来源：http://rvs.sjlbkw.cn

[R74] 批量重命名
来源：http://egh.hfpthk.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sqs.uphjek.com

[R75] 导出环境变量
来源：http://qbx.guowangkeji.top

export PATH="$HOME/bin:$PATH"
来源：http://ixt.fzhhl.top

[R76] 使用临时文件
来源：http://lnt.jqgufenzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lkt.cashguo.top

[R77] 读取用户输入
来源：http://nlm.cashguo.top

read -rp "请输入: " ans
来源：http://phd.uphjek.com

[R78] 交互式菜单
来源：http://ifw.xinyue.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://vhi.sxryk.cn

[R79] 解析命令行选项
来源：http://ire.fanxiaobao.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mwj.shzxlz.cn

[R80] 查看脚本执行耗时
来源：http://xay.gogol.net.cn

time ./run.sh
来源：http://hkj.yj20258888.top

================================================================================
来源：http://rsc.hysaishi.cn

S. C / C++ 专题
来源：http://eta.gzhubu.top

================================================================================
来源：http://etd.vehdjk.com

[S01] C：Hello World
来源：http://fgj.fehbvm.com

#include <stdio.h>
来源：http://ffc.gogol.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tmh.shanyushiyangtech.top

[S02] C：变量与格式化输出
来源：http://kbx.guowangkeji.top

int a = 10; printf("%d\n", a);
来源：http://jjl.cdnleiting.top

[S03] C：读入整数
来源：http://qnw.jinyuanbaomall.cn

int x; scanf("%d", &x);
来源：http://vhd.daxiang520.top

[S04] C：字符串复制
来源：http://igg.yonumen.top

char dst[32]; strcpy(dst, "hi");
来源：http://pib.shuidangran.top

[S05] C：字符串长度
来源：http://gxr.c1oappe.top

strlen(s)
来源：http://lfj.xuanzx.com

[S06] C：字符串比较
来源：http://huz.zhengqikj.top

strcmp(a, b) == 0
来源：http://igk.jqgufenzy.top

[S07] C：数组遍历求和
来源：http://biz.shzxlz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jut.fehbvm.com

[S08] C：动态内存分配与释放
来源：http://bpc.wangshuangyany.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kdj.xingfuxueyuan.xyz

[S09] C：结构体定义与初始化
来源：http://yor.yongpay.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wvr.cqqwz.cn

[S10] C：指针与解引用
来源：http://btr.smart0.xyz

int *p = &a;  *p = 5;
来源：http://dvo.yj20258.top

[S11] C：逐行读文件
来源：http://yqk.chenlongwang.top

FILE *f = fopen("a.txt", "r");
来源：http://jvl.snrcjt.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://opc.jinqigufen.top

fclose(f);
来源：http://bgu.wangshuangyany.cn

[S12] C：写文件
来源：http://jur.chenlongwang.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mcu.quarkkingdee.top

[S13] C：宏定义
来源：http://zbx.daria6918.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sew.sjlbkw.cn

[S14] C：枚举
来源：http://koz.zhengqikj.top

enum Color { RED, GREEN, BLUE };
来源：http://xsf.xinyue.icu

[S15] C：类型转换
来源：http://jkm.jinqigufen.top

(double) a / b
来源：http://dfi.ppjwa.cn

[S16] C：位操作置位
来源：http://gce.ppjwa.cn

x |= (1 << 3);
来源：http://gof.jinyuanbaomall.cn

[S17] C：安全拼接字符串
来源：http://wty.yangfankeji.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jrb.jqgfzy.top

[S18] C：命令行参数
来源：http://yja.fengsongda.top

int main(int argc, char **argv)
来源：http://mun.jianghu66.top

[S19] C：快速排序
来源：http://dnn.gzhubu.top

qsort(a, n, sizeof(int), cmp);
来源：http://lgg.epnwcf.com

[S20] C：二分查找
来源：http://npl.cdnleiting.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nyc.havefunace.top

[S21] C：字符类别判断
来源：http://tgq.pengpengdd.cyou

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ieh.c1oappe.top

[S22] C：字符串转数字
来源：http://esq.meibo888.top

atoi("42");  strtod("3.14", NULL);
来源：http://gmp.daxiang520.top

[S23] C：随机数
来源：http://vss.aibaodan.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rfk.xuanzx.com

[S24] C：获取本地时间
来源：http://jdo.jianghu66.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kgo.redwolf501.top

[S25] C：内存拷贝
来源：http://mce.aizwys.cn

memcpy(dst, src, n);
来源：http://ucs.fanxiaobao.xyz

[S26] C：内存清零
来源：http://lzi.dashuyun.cn

memset(a, 0, sizeof a);
来源：http://aef.aibaodan.cn

[S27] C：定义常量
来源：http://nyo.daria6918.cn

const double PI = 3.14159;
来源：http://ugv.fengsongda.top

[S28] C：静态变量
来源：http://sxj.xinyue.icu

static int counter = 0;
来源：http://kkh.52xcode.cn

[S29] C：变参函数
来源：http://hny.cqqwz.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ogv.zhengqikj.top

[S30] C：头文件保护
来源：http://omk.zhaomingkeji.xyz

#ifndef X_H
来源：http://bak.aizwys.cn

#define X_H
来源：http://ewc.gzhubu.top

#endif
来源：http://svr.bbcook.cn

[S31] C++：Hello World
来源：http://jma.shuidangran.top

#include <iostream>
来源：http://mfv.shanyushiyangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://znm.316326.xyz

[S32] C++：字符串
来源：http://mmw.quarkkingdee.top

std::string s = "hi";  s += "!";
来源：http://bkg.fehbvm.com

[S33] C++：vector 增删
来源：http://hwm.zdbjq.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mgw.wangshuangyany.cn

[S34] C++：遍历 vector
来源：http://vgh.316326.xyz

for (auto &x : v) { std::cout << x; }
来源：http://bpq.jyoumei.cn

[S35] C++：map
来源：http://bxk.jlsjyb.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://knn.xylfe.cn

[S36] C++：unordered_map
来源：http://ygf.cucudq.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zkc.shuidangran.top

[S37] C++：set
来源：http://yha.jinyuanbaomall.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zlg.nanxinkj.top

[S38] C++：排序
来源：http://ald.jlsjyb.cn

std::sort(v.begin(), v.end());
来源：http://vqy.cheryme.top

[S39] C++：自定义比较器排序
来源：http://lsr.hywenlv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zbd.hysaishi.cn

[S40] C++：查找元素
来源：http://dko.daxiang520.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dfd.pengpengdd.cyou

[S41] C++：类与构造函数
来源：http://ivo.havefunace.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ccr.fanxiaobao.xyz

[S42] C++：继承与虚函数
来源：http://haz.fktsv.cn

class B : public Base { public: void f() override {} };
来源：http://ovm.daxiang520.top

[S43] C++：智能指针
来源：http://qmu.xziqi.cn

auto p = std::make_unique<int>(5);
来源：http://ccj.sufxvd.cn

[S44] C++：引用传参
来源：http://ltr.haohaochexian.top

void inc(int &x) { ++x; }
来源：http://wru.52xcode.cn

[S45] C++：lambda
来源：http://bac.xziqi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xmy.hammf.cn

[S46] C++：函数模板
来源：http://iuw.shzxlz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://piv.daxiang520.top

[S47] C++：结构化绑定遍历
来源：http://agg.xylfe.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zwg.shangyingyoupin.top

[S48] C++：逐行读文件
来源：http://gya.hfpthk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xdx.zhijiandao.cn

while (std::getline(in, line)) { }
来源：http://ihl.shzxlz.cn

[S49] C++：写文件
来源：http://mgd.cqqwz.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gtb.zycfv.cn

[S50] C++：格式化数字
来源：http://mqj.52xcode.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zve.jinghuilouyu.cn

[S51] C++：显式类型转换
来源：http://mkq.daxiang520.top

static_cast<double>(a) / b
来源：http://nrf.fktsv.cn

[S52] C++：const 与 noexcept
来源：http://ywi.chenlongwang.top

int size() const noexcept { return n_; }
来源：http://zzv.yfazqb.com

[S53] C++：移动语义
来源：http://fcj.jyoumei.cn

std::vector<int> w = std::move(v);
来源：http://sjq.ybcxt.top

[S54] C++：异常处理
来源：http://pju.sufxvd.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zvr.wangshuangyany.cn

[S55] C++：结构化绑定
来源：http://rjk.yfazqb.com

auto [a, b] = std::make_pair(1, 2);
来源：http://zcf.sjlbkw.cn

[S56] C++：optional
来源：http://waa.jqgfzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lyx.shuidangran.top

[S57] C++：编译期常量
来源：http://diz.zdbjq.cn

constexpr int N = 10;
来源：http://vnl.ppjwa.cn

[S58] C++：命名空间
来源：http://amk.xziqi.cn

namespace ns { int f() { return 1; } }
来源：http://owm.guowangkeji.top

[S59] C++：静态断言
来源：http://uxt.yj202588.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wlk.52xcode.cn

[S60] C++：遍历并删除元素
来源：http://aaa.dianchejie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gqw.nanxuanxn.top

================================================================================
来源：http://xnf.yanxiufei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tnv.jlsjyb.cn

================================================================================
来源：http://din.mhx1999.top

[T01] Kotlin：Hello World
来源：http://bil.jinyuanbaomall.cn

println("Hello")
来源：http://tbo.shanyushiyangkeji.top

[T02] Kotlin：变量
来源：http://wbl.haohaochexian.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://enh.cucudq.cn

[T03] Kotlin：字符串模板
来源：http://cqh.fehbvm.com

"值: $b"
来源：http://prw.yongpay.top

[T04] Kotlin：空安全
来源：http://buf.nanxuanxn.top

val n: String? = null;  n?.length
来源：http://joy.ivvv.top

[T05] Kotlin：when 表达式
来源：http://jre.vehdjk.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gmi.0kj1m.cn

[T06] Kotlin：集合映射
来源：http://mva.tianlin.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://wyb.jyoumei.cn

[T07] Kotlin：集合过滤
来源：http://ggi.sufxvd.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vez.nwbrower.top

[T08] Kotlin：数据类
来源：http://pqy.guowangkeji.top

data class User(val name: String, val age: Int)
来源：http://xmm.guannengcc.top

[T09] Kotlin：扩展函数
来源：http://zbg.gogol.net.cn

fun String.exclaim() = this + "!"
来源：http://zhb.kuanghao11.cn

[T10] Kotlin：默认参数
来源：http://ial.epnwcf.com

fun greet(name: String = "World") = "Hi $name"
来源：http://qpr.yvedp.cn

[T11] Kotlin：协程
来源：http://zvd.jlsjyb.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dal.dianchejie.cn

[T12] Kotlin：解构声明
来源：http://azi.quarkkingdee.top

val (a, b) = Pair(1, 2)
来源：http://cuu.jinqigufen.top

[T13] Kotlin：只读 Map
来源：http://eau.meibo888.top

val m = mapOf("a" to 1)
来源：http://vmn.jinqigfzy.top

[T14] Kotlin：循环
来源：http://okb.316326.xyz

for (i in 1..10) println(i)
来源：http://ahl.xinyue.icu

[T15] Kotlin：接口
来源：http://djm.andypj.xyz

interface Shape { fun area(): Double }
来源：http://xzx.xuanzx.com

[T16] Swift：Hello World
来源：http://zym.0kj1m.cn

print("Hello")
来源：http://fmf.hesvh.cn

[T17] Swift：变量与常量
来源：http://ysm.jianghu66.top

var a = 1;  let b = 2
来源：http://gjk.yuanzhike.top

[T18] Swift：字符串插值
来源：http://enu.sjlbkw.cn

"值: \(b)"
来源：http://aoo.iojbl.cn


<!-- 参考信息 -->