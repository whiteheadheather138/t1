代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://tvg.pycfn.com

[R14] C 风格 for
来源：http://wmk.sxryk.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://biq.meibo888.top

[R15] while 逐行读文件
来源：http://emy.yfazqb.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lnj.ctjpmb.com

[R16] until 等待条件
来源：http://tji.cucudq.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qay.52xcode.cn

[R17] 数组定义与取值
来源：http://eqm.316326.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://ugd.9152youxi.cn

[R18] 遍历数组
来源：http://dxs.hongshengwenyu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hty.fehbvm.com

[R19] 数组长度
来源：http://izp.jinyuanbaomall.cn

echo "${#arr[@]}"
来源：http://ziq.hnqzz.top

[R20] 关联数组（字典）
来源：http://fix.xinyue.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lxq.sjlbkw.cn

[R21] 字符串长度
来源：http://blp.fktsv.cn

echo "${#s}"
来源：http://iof.sysykeji.top

[R22] 截取子串
来源：http://hkj.sufxvd.cn

echo "${s:0:5}"
来源：http://xzl.sjlbkw.cn

[R23] 字符串替换
来源：http://ywz.cdnleiting.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://guc.zhoulong.xyz

[R24] 大小写转换
来源：http://rms.sysykeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://xok.cheryme.top

[R25] 去后缀 / 去前缀
来源：http://vcn.0kj1m.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vlx.dashuyun.cn

[R26] 命令替换
来源：http://gho.jqgufenzy.top

now=$(date +%F); echo "$now"
来源：http://enf.fehbvm.com

[R27] 算术展开
来源：http://ohz.fktsv.cn

echo $((1 + 2 * 3))
来源：http://ulg.sxryk.cn

[R28] 浮点运算
来源：http://mle.zhoulong.xyz

echo "scale=2; 10/3" | bc
来源：http://gbv.chenzaomai.com

[R29] 定义函数
来源：http://kyr.jqgufenzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lgy.jiagoushi.top

[R30] 函数返回状态码
来源：http://wnl.sysykeji.top

f() { return 0; }; f || echo "失败了"
来源：http://ssl.snrcjt.cn

[R31] 局部变量
来源：http://aie.tian-w.cn

f() { local x=1; echo "$x"; }
来源：http://wln.yongpay.top

[R32] 参数个数校验
来源：http://nvl.yueranfly.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dmh.sjlbkw.cn

[R33] 捕获错误并提示行号
来源：http://czb.havefunace.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bse.jinghuilouyu.cn

[R34] 退出时清理
来源：http://ftx.ybcxt.top

trap 'rm -f "$tmp"' EXIT
来源：http://wbe.jinqigfzy.top

[R35] 后台执行并等待
来源：http://yxi.xylfe.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fim.fehbvm.com

[R36] 并发执行多个任务
来源：http://obu.xylfe.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hvq.gotoacloud.top

[R37] 把输出赋给变量
来源：http://qmd.quarkkingdee.top

files=$(ls -1)
来源：http://tkk.daxiang520.top

[R38] 管道串联
来源：http://bqw.xylfe.cn

cat a.txt | grep -i error | wc -l
来源：http://lau.daxiang520.top

[R39] 重定向标准输出与错误
来源：http://bjc.pycfn.com

cmd > out.log 2>&1
来源：http://khx.ehwqpu.com

[R40] 追加写日志
来源：http://jgo.wangshuangyany.cn

echo "log" >> out.log
来源：http://nrb.redwolf501.top

[R41] 丢弃输出
来源：http://rhh.yongpay.top

cmd >/dev/null 2>&1
来源：http://wpw.hnxiangtu.top

[R42] 输入重定向
来源：http://hql.9152youxi.cn

wc -l < a.txt
来源：http://nlz.tian-w.cn

[R43] 按名字查找文件
来源：http://tel.c1oappe.top

find . -name "*.log" -type f
来源：http://vki.jinqigfzy.top

[R44] 按修改时间查找
来源：http://okf.feifeiyinyue.top

find . -mtime -7 -type f
来源：http://hts.zhijiandao.cn

[R45] 批量删除
来源：http://vll.nwbrower.top

find . -name "*.tmp" -delete
来源：http://pip.jyoumei.cn

[R46] 递归替换文件内容
来源：http://oav.shanyushiyangkeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zpe.shanyushiyangtech.top

[R47] sed 单行替换
来源：http://czi.xuanzx.com

sed -i 's/foo/bar/g' a.txt
来源：http://oey.yueranfly.top

[R48] awk 取指定列
来源：http://aap.gzhubu.top

awk '{print $1, $3}' a.txt
来源：http://hhe.shzxlz.cn

[R49] awk 带条件
来源：http://jep.shuidangran.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://anw.iojbl.cn

[R50] awk 求和
来源：http://fxd.tarul.cn

awk '{s += $2} END {print s}' a.txt
来源：http://adz.meibo888.top

[R51] 排序去重取前几
来源：http://xjc.zhiwuduotai.top

sort a.txt | uniq -c | sort -rn | head
来源：http://cav.hysaishi.cn

[R52] 统计行数
来源：http://rni.zhixingplan.top

wc -l a.txt
来源：http://lep.jinghuilouyu.cn

[R53] 查看文件头与实时尾
来源：http://ueo.andypj.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lkp.hammf.cn

[R54] 比较两个文件
来源：http://vbn.haohaochexian.top

diff a.txt b.txt
来源：http://nfv.shuidangran.top

[R55] 压缩与解压
来源：http://rnc.tarul.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yhf.jiagoushi.top

[R56] 远程拷贝
来源：http://slq.guannengcc.top

scp file user@host:/path/
来源：http://msu.yj20258888.top

[R57] 远程执行命令
来源：http://wdp.yonumen.top

ssh user@host 'uptime'
来源：http://eal.sweek.top

[R58] 下载文件
来源：http://boo.redwolf501.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vpd.chenzaomai.com

[R59] 发 POST JSON
来源：http://gvi.zhongyouzk.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pol.zhaomingkeji.xyz

[R60] 只看 HTTP 状态码
来源：http://dcs.yfazqb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://eyj.jinyuanbaomall.cn

[R61] 磁盘占用
来源：http://oql.tianlin.xyz

df -h;  du -sh *
来源：http://iav.jinqigufen.top

[R62] 找最占空间的文件
来源：http://ixz.cashguo.top

du -ah . | sort -rh | head -10
来源：http://tfp.jinqigfzy.top

[R63] 内存与进程
来源：http://wqp.wangshuangyany.cn

free -h;  ps aux | grep nginx
来源：http://maj.vehdjk.com

[R64] 结束进程
来源：http://fao.xingfuxueyuan.xyz

kill -9 $(pgrep -f app.py)
来源：http://bwm.cucudq.cn

[R65] 查看端口占用
来源：http://fzx.cashguo.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yut.cucudq.cn

[R66] 定时任务
来源：http://pis.daria6918.cn

crontab -e;  crontab -l
来源：http://krg.9152youxi.cn

[R67] 生成随机十六进制串
来源：http://ktr.ywan-chungtsiang.top

openssl rand -hex 16
来源：http://bvq.zhongyouzk.top

[R68] 计算文件校验值
来源：http://jxu.fengsongda.top

sha256sum a.txt;  md5sum a.txt
来源：http://sgs.zhijiandao.cn

[R69] 生成随机密码
来源：http://smk.redwolf501.top

head -c 16 /dev/urandom | base64
来源：http://yvy.zhixingplan.top

[R70] 时间戳与互转
来源：http://ivz.xuanzx.com

date +%s;  date -d @1700000000
来源：http://xck.zdbjq.cn

[R71] 日期格式化
来源：http://kms.yvedp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mpy.ctjpmb.com

[R72] 等待端口就绪
来源：http://nfs.havefunace.top

until nc -z localhost 3306; do sleep 1; done
来源：http://cgk.jinyuanbaomall.cn

[R73] 分割大日志
来源：http://hxb.jiagoushi.top

split -l 1000 big.log part_
来源：http://zld.zhixingplan.top

[R74] 批量重命名
来源：http://asw.gogol.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rtn.hywenlv.cn

[R75] 导出环境变量
来源：http://pdf.yuanzhike.top

export PATH="$HOME/bin:$PATH"
来源：http://pag.pengpengdd.cyou

[R76] 使用临时文件
来源：http://grc.xingfuxueyuan.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pij.daxiang520.top

[R77] 读取用户输入
来源：http://zel.jiagoushi.top

read -rp "请输入: " ans
来源：http://gfe.ctjpmb.com

[R78] 交互式菜单
来源：http://kaw.yuxming.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://clj.daxiang520.top

[R79] 解析命令行选项
来源：http://kte.yvedp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jjg.fengsongda.top

[R80] 查看脚本执行耗时
来源：http://oti.aizwys.cn

time ./run.sh
来源：http://bxr.sufxvd.cn

================================================================================
来源：http://udl.zhaomingkeji.xyz

S. C / C++ 专题
来源：http://dih.hongshengwenyu.top

================================================================================
来源：http://das.mhx1999.top

[S01] C：Hello World
来源：http://ryh.hnxiangtu.top

#include <stdio.h>
来源：http://ukr.dashuyun.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wqs.c1oappe.top

[S02] C：变量与格式化输出
来源：http://yru.vehdjk.com

int a = 10; printf("%d\n", a);
来源：http://xcg.jlsjyb.cn

[S03] C：读入整数
来源：http://bun.zdqjudy.top

int x; scanf("%d", &x);
来源：http://lyt.yuanzhike.top

[S04] C：字符串复制
来源：http://mcs.yvedp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dnp.tian-w.cn

[S05] C：字符串长度
来源：http://ykw.daxiang520.top

strlen(s)
来源：http://nsn.nwbrower.top

[S06] C：字符串比较
来源：http://pmf.zdqjudy.top

strcmp(a, b) == 0
来源：http://oiw.yanxiufei.cn

[S07] C：数组遍历求和
来源：http://ypz.jinyuanbaomall.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dxh.zhongyouzk.top

[S08] C：动态内存分配与释放
来源：http://ohz.cdnleiting.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vzq.chenlongwang.top

[S09] C：结构体定义与初始化
来源：http://ihs.shangyingyoupin.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sat.52xcode.cn

[S10] C：指针与解引用
来源：http://zuq.tanke756.top

int *p = &a;  *p = 5;
来源：http://yee.cashguo.top

[S11] C：逐行读文件
来源：http://drx.gzhubu.top

FILE *f = fopen("a.txt", "r");
来源：http://cpr.yvedp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tip.zhoulong.xyz

fclose(f);
来源：http://igc.zhiwuduotai.top

[S12] C：写文件
来源：http://nvr.yuxming.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jzw.nanxuanxn.top

[S13] C：宏定义
来源：http://vwc.tian-w.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vfo.0kj1m.cn

[S14] C：枚举
来源：http://qdr.gogol.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://vuu.jinghuilouyu.cn

[S15] C：类型转换
来源：http://orj.jinyuanbaomall.cn

(double) a / b
来源：http://yvt.jyoumei.cn

[S16] C：位操作置位
来源：http://nas.ppjwa.cn

x |= (1 << 3);
来源：http://zyy.cucudq.cn

[S17] C：安全拼接字符串
来源：http://cpi.wangdashe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zbl.tanke756.top

[S18] C：命令行参数
来源：http://hbq.jqgufenzy.top

int main(int argc, char **argv)
来源：http://yfs.hnqzz.top

[S19] C：快速排序
来源：http://zds.bbcook.cn

qsort(a, n, sizeof(int), cmp);
来源：http://piw.cdnleiting.top

[S20] C：二分查找
来源：http://pqe.yueranfly.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uzh.ydzc1.top

[S21] C：字符类别判断
来源：http://vig.zhixingplan.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://shk.shzxlz.cn

[S22] C：字符串转数字
来源：http://hri.jqgfzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://zaf.ydjk.org.cn

[S23] C：随机数
来源：http://lhx.zdqjudy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://luw.hfpthk.cn

[S24] C：获取本地时间
来源：http://erd.gaohongyu789.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jgc.cheryme.top

[S25] C：内存拷贝
来源：http://kah.aibaodan.cn

memcpy(dst, src, n);
来源：http://xhc.shuidangran.top

[S26] C：内存清零
来源：http://xpa.ehwqpu.com

memset(a, 0, sizeof a);
来源：http://crf.meibo888.top

[S27] C：定义常量
来源：http://jae.dashuyun.cn

const double PI = 3.14159;
来源：http://qbh.hnqzz.top

[S28] C：静态变量
来源：http://eba.yonumen.top

static int counter = 0;
来源：http://zrc.andypj.xyz

[S29] C：变参函数
来源：http://gou.redwolf501.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qgu.gzhubu.top

[S30] C：头文件保护
来源：http://mxe.nanxinkj.top

#ifndef X_H
来源：http://fir.epnwcf.com

#define X_H
来源：http://oio.hesvh.cn

#endif
来源：http://qfo.ppjwa.cn

[S31] C++：Hello World
来源：http://ckc.cdnleiting.top

#include <iostream>
来源：http://kcg.yangfankeji.com

int main() { std::cout << "Hello\n"; }
来源：http://yhq.xingfuxueyuan.xyz

[S32] C++：字符串
来源：http://iax.daria6918.cn

std::string s = "hi";  s += "!";
来源：http://eyd.tarul.cn

[S33] C++：vector 增删
来源：http://ihm.jqgfzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://czm.haohaochexian.top

[S34] C++：遍历 vector
来源：http://cuw.ctjpmb.com

for (auto &x : v) { std::cout << x; }
来源：http://ini.shuidangran.top

[S35] C++：map
来源：http://fug.yuanzhike.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jwr.jinqigufen.top

[S36] C++：unordered_map
来源：http://xlq.zhijiandao.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ahb.cheryme.top

[S37] C++：set
来源：http://tdr.sweek.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gii.jlsjyb.cn

[S38] C++：排序
来源：http://tjh.yonumen.top

std::sort(v.begin(), v.end());
来源：http://ynr.yuanzhike.top

[S39] C++：自定义比较器排序
来源：http://bzw.nanxinkj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wrl.zhaomingkeji.xyz

[S40] C++：查找元素
来源：http://srg.0kj1m.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rbk.snrcjt.cn

[S41] C++：类与构造函数
来源：http://rup.xziqi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tgg.jianghu66.top

[S42] C++：继承与虚函数
来源：http://mwe.jinqigfzy.top

class B : public Base { public: void f() override {} };
来源：http://smw.yj20258888.top

[S43] C++：智能指针
来源：http://scn.jlsjyb.cn

auto p = std::make_unique<int>(5);
来源：http://fhw.bbcook.cn

[S44] C++：引用传参
来源：http://zqr.cashguo.top

void inc(int &x) { ++x; }
来源：http://vyf.hfpthk.cn

[S45] C++：lambda
来源：http://teq.cqqwz.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gys.zhaomingkeji.xyz

[S46] C++：函数模板
来源：http://yfv.cashguo.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zan.haohaochexian.top

[S47] C++：结构化绑定遍历
来源：http://shj.xuanzx.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://alc.tian-w.cn

[S48] C++：逐行读文件
来源：http://fna.smart0.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://klc.jinqigufen.top

while (std::getline(in, line)) { }
来源：http://gjm.chenjidiqi.icu

[S49] C++：写文件
来源：http://npv.jqgfzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iri.316326.xyz

[S50] C++：格式化数字
来源：http://nca.yfazqb.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://krj.dianchejie.cn

[S51] C++：显式类型转换
来源：http://ypv.fktsv.cn

static_cast<double>(a) / b
来源：http://ssn.yanxiufei.cn

[S52] C++：const 与 noexcept
来源：http://oot.zycfv.cn

int size() const noexcept { return n_; }
来源：http://scz.sufxvd.cn

[S53] C++：移动语义
来源：http://zcm.hammf.cn

std::vector<int> w = std::move(v);
来源：http://bez.cucudq.cn

[S54] C++：异常处理
来源：http://dpj.guannengcc.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gvh.yfazqb.com

[S55] C++：结构化绑定
来源：http://zdt.jinyuanbaomall.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zbx.yuxming.cn

[S56] C++：optional
来源：http://gep.zdbjq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nka.wangdashe.top

[S57] C++：编译期常量
来源：http://cqq.sjlbkw.cn

constexpr int N = 10;
来源：http://dbh.jiagoushi.top

[S58] C++：命名空间
来源：http://haq.hongshengwenyu.top

namespace ns { int f() { return 1; } }
来源：http://eky.birdmap.top

[S59] C++：静态断言
来源：http://fwg.ctjpmb.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fax.nwbrower.top

[S60] C++：遍历并删除元素
来源：http://lmn.pycfn.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ebf.jinghuilouyu.cn

================================================================================
来源：http://fpg.mhx1999.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bot.gzhubu.top

================================================================================
来源：http://nyx.gzhubu.top

[T01] Kotlin：Hello World
来源：http://fnf.mhx1999.top

println("Hello")
来源：http://eqx.ctjpmb.com

[T02] Kotlin：变量
来源：http://lrj.shanyushiyangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ksh.hnxiangtu.top

[T03] Kotlin：字符串模板
来源：http://ytv.hywenlv.cn

"值: $b"
来源：http://abq.tarul.cn

[T04] Kotlin：空安全
来源：http://zaw.hfpthk.cn

val n: String? = null;  n?.length
来源：http://fua.ppjwa.cn

[T05] Kotlin：when 表达式
来源：http://pzy.0kj1m.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bjc.sufxvd.cn

[T06] Kotlin：集合映射
来源：http://adb.daria6918.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qbb.sjlbkw.cn

[T07] Kotlin：集合过滤
来源：http://uyb.0kj1m.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gwo.zhijiandao.cn

[T08] Kotlin：数据类
来源：http://pfd.ydjk.org.cn

data class User(val name: String, val age: Int)
来源：http://bwy.chenjidiqi.icu

[T09] Kotlin：扩展函数
来源：http://flw.jinghuilouyu.cn

fun String.exclaim() = this + "!"
来源：http://qhb.tanke756.top

[T10] Kotlin：默认参数
来源：http://edi.hysaishi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kog.jqgfzy.top

[T11] Kotlin：协程
来源：http://gjv.quarkkingdee.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mrp.quarkkingdee.top

[T12] Kotlin：解构声明
来源：http://tnk.zhiwuduotai.top

val (a, b) = Pair(1, 2)
来源：http://thv.vqdsnc.cn

[T13] Kotlin：只读 Map
来源：http://shv.wangdashe.top

val m = mapOf("a" to 1)
来源：http://oze.dianchejie.cn

[T14] Kotlin：循环
来源：http://jvd.gotoacloud.top

for (i in 1..10) println(i)
来源：http://khs.yangfankeji.com

[T15] Kotlin：接口
来源：http://kvs.zhongyouzk.top

interface Shape { fun area(): Double }
来源：http://hyr.316326.xyz

[T16] Swift：Hello World
来源：http://kdl.zdbjq.cn

print("Hello")
来源：http://glm.jianghu66.top


<!-- 参考信息 -->