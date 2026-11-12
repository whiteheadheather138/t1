代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://nwy.dashuyun.cn

[R14] C 风格 for
来源：http://mbm.tian-w.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mrh.nwbrower.top

[R15] while 逐行读文件
来源：http://ups.aibaodan.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sre.wangdashe.top

[R16] until 等待条件
来源：http://ull.smart0.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zxy.uphjek.com

[R17] 数组定义与取值
来源：http://jrp.shanyushiyangtech.top

arr=(a b c); echo "${arr[0]}"
来源：http://mtk.yuxming.cn

[R18] 遍历数组
来源：http://pct.ppjwa.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://spr.sxryk.cn

[R19] 数组长度
来源：http://jzf.jinqigufen.top

echo "${#arr[@]}"
来源：http://vun.havefunace.top

[R20] 关联数组（字典）
来源：http://ccu.c1oappe.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tge.sjlbkw.cn

[R21] 字符串长度
来源：http://xzl.fzhhl.top

echo "${#s}"
来源：http://agn.cdnleiting.top

[R22] 截取子串
来源：http://ejg.chenlongwang.top

echo "${s:0:5}"
来源：http://yly.sysykeji.top

[R23] 字符串替换
来源：http://dpm.shzxlz.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://krf.meibo888.top

[R24] 大小写转换
来源：http://pfv.wangdashe.top

echo "${s^^}"; echo "${s,,}"
来源：http://sss.jianghu66.top

[R25] 去后缀 / 去前缀
来源：http://zjh.cheryme.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ewr.nanxinkj.top

[R26] 命令替换
来源：http://ijf.jyoumei.cn

now=$(date +%F); echo "$now"
来源：http://dcq.sjlbkw.cn

[R27] 算术展开
来源：http://kdv.snrcjt.cn

echo $((1 + 2 * 3))
来源：http://qhn.mhx1999.top

[R28] 浮点运算
来源：http://nbm.gotoacloud.top

echo "scale=2; 10/3" | bc
来源：http://ome.gotoacloud.top

[R29] 定义函数
来源：http://trd.fktsv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vex.hysaishi.cn

[R30] 函数返回状态码
来源：http://kbr.shangyingyoupin.top

f() { return 0; }; f || echo "失败了"
来源：http://que.haohaochexian.top

[R31] 局部变量
来源：http://tks.ehwqpu.com

f() { local x=1; echo "$x"; }
来源：http://vrk.zhongyouzk.top

[R32] 参数个数校验
来源：http://tuf.snrcjt.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qgw.jinqigfzy.top

[R33] 捕获错误并提示行号
来源：http://rmq.yj202588.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jkp.yonumen.top

[R34] 退出时清理
来源：http://ijy.nwbrower.top

trap 'rm -f "$tmp"' EXIT
来源：http://ndn.sjlbkw.cn

[R35] 后台执行并等待
来源：http://yaa.zhoulong.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://wyu.bjfxy.top

[R36] 并发执行多个任务
来源：http://wmf.fengsongda.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://upi.fktsv.cn

[R37] 把输出赋给变量
来源：http://rpw.hongshengwenyu.top

files=$(ls -1)
来源：http://abn.hcnkem.com

[R38] 管道串联
来源：http://ufn.gaohongyu789.top

cat a.txt | grep -i error | wc -l
来源：http://vex.shanyushiyangtech.top

[R39] 重定向标准输出与错误
来源：http://ilc.birdmap.top

cmd > out.log 2>&1
来源：http://kiw.yj20258888.top

[R40] 追加写日志
来源：http://kjw.chenjidiqi.icu

echo "log" >> out.log
来源：http://qsk.chenjidiqi.icu

[R41] 丢弃输出
来源：http://wgi.zhijiandao.cn

cmd >/dev/null 2>&1
来源：http://gta.wangshuangyany.cn

[R42] 输入重定向
来源：http://orv.nanxinkj.top

wc -l < a.txt
来源：http://xsf.tianlin.xyz

[R43] 按名字查找文件
来源：http://oxd.fanxiaobao.xyz

find . -name "*.log" -type f
来源：http://env.jinqigufen.top

[R44] 按修改时间查找
来源：http://rob.nwbrower.top

find . -mtime -7 -type f
来源：http://elv.aibaodan.cn

[R45] 批量删除
来源：http://jsj.ydzc1.top

find . -name "*.tmp" -delete
来源：http://nud.ydzc1.top

[R46] 递归替换文件内容
来源：http://yjh.hesvh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zpm.havefunace.top

[R47] sed 单行替换
来源：http://wrh.jyoumei.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wer.jinyuanbaomall.cn

[R48] awk 取指定列
来源：http://alg.cashguo.top

awk '{print $1, $3}' a.txt
来源：http://tsc.ydjk.org.cn

[R49] awk 带条件
来源：http://mdf.c1oappe.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bqq.shuidangran.top

[R50] awk 求和
来源：http://dwn.pengpengdd.cyou

awk '{s += $2} END {print s}' a.txt
来源：http://kbv.cashguo.top

[R51] 排序去重取前几
来源：http://zyj.andypj.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://tel.fengsongda.top

[R52] 统计行数
来源：http://kxp.ywan-chungtsiang.top

wc -l a.txt
来源：http://ffx.9152youxi.cn

[R53] 查看文件头与实时尾
来源：http://fdz.shangyingyoupin.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qet.redwolf501.top

[R54] 比较两个文件
来源：http://wuf.aizwys.cn

diff a.txt b.txt
来源：http://ssy.zhengqikj.top

[R55] 压缩与解压
来源：http://ths.daria6918.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uax.ehwqpu.com

[R56] 远程拷贝
来源：http://qsg.uphjek.com

scp file user@host:/path/
来源：http://zxu.sysykeji.top

[R57] 远程执行命令
来源：http://pkt.aibaodan.cn

ssh user@host 'uptime'
来源：http://hpz.yvedp.cn

[R58] 下载文件
来源：http://dfg.yj20258888.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nsh.feifeiyinyue.top

[R59] 发 POST JSON
来源：http://mcy.fehbvm.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://elp.yueranfly.top

[R60] 只看 HTTP 状态码
来源：http://mjz.haohaochexian.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gdx.yangfankeji.com

[R61] 磁盘占用
来源：http://tfd.feifeiyinyue.top

df -h;  du -sh *
来源：http://geo.tarul.cn

[R62] 找最占空间的文件
来源：http://kjb.ehwqpu.com

du -ah . | sort -rh | head -10
来源：http://wbu.vehdjk.com

[R63] 内存与进程
来源：http://myo.xingfuxueyuan.xyz

free -h;  ps aux | grep nginx
来源：http://drm.daxiang520.top

[R64] 结束进程
来源：http://xov.zhiwuduotai.top

kill -9 $(pgrep -f app.py)
来源：http://sdy.hfpthk.cn

[R65] 查看端口占用
来源：http://jib.52xcode.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qqa.yfazqb.com

[R66] 定时任务
来源：http://koy.hfpthk.cn

crontab -e;  crontab -l
来源：http://tll.jinghuilouyu.cn

[R67] 生成随机十六进制串
来源：http://yxe.zdbjq.cn

openssl rand -hex 16
来源：http://baf.yueranfly.top

[R68] 计算文件校验值
来源：http://wns.pengpengdd.cyou

sha256sum a.txt;  md5sum a.txt
来源：http://fij.gogol.net.cn

[R69] 生成随机密码
来源：http://xav.jinqigfzy.top

head -c 16 /dev/urandom | base64
来源：http://rhk.quarkkingdee.top

[R70] 时间戳与互转
来源：http://ujt.sweek.top

date +%s;  date -d @1700000000
来源：http://zdj.shuidangran.top

[R71] 日期格式化
来源：http://nsv.hysaishi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://srr.gzhubu.top

[R72] 等待端口就绪
来源：http://ifl.zhixingplan.top

until nc -z localhost 3306; do sleep 1; done
来源：http://tny.hnxiangtu.top

[R73] 分割大日志
来源：http://cyw.chenzaomai.com

split -l 1000 big.log part_
来源：http://bgn.snrcjt.cn

[R74] 批量重命名
来源：http://mij.hongshengwenyu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vbm.yj20258888.top

[R75] 导出环境变量
来源：http://lky.jiagoushi.top

export PATH="$HOME/bin:$PATH"
来源：http://wed.cqqwz.cn

[R76] 使用临时文件
来源：http://ceb.meibo888.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ehk.cucudq.cn

[R77] 读取用户输入
来源：http://zop.tarul.cn

read -rp "请输入: " ans
来源：http://piw.ctjpmb.com

[R78] 交互式菜单
来源：http://upa.hammf.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://arg.hesvh.cn

[R79] 解析命令行选项
来源：http://nsf.fehbvm.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://osh.guannengcc.top

[R80] 查看脚本执行耗时
来源：http://pvd.daria6918.cn

time ./run.sh
来源：http://qcd.316326.xyz

================================================================================
来源：http://hnw.chenlongwang.top

S. C / C++ 专题
来源：http://cxl.fzhhl.top

================================================================================
来源：http://jht.daria6918.cn

[S01] C：Hello World
来源：http://fir.ybcxt.top

#include <stdio.h>
来源：http://wju.chenjidiqi.icu

int main(void) { printf("Hello\n"); return 0; }
来源：http://qwm.yvedp.cn

[S02] C：变量与格式化输出
来源：http://sfk.uphjek.com

int a = 10; printf("%d\n", a);
来源：http://fqz.tianlin.xyz

[S03] C：读入整数
来源：http://gog.ydzc1.top

int x; scanf("%d", &x);
来源：http://toz.nwbrower.top

[S04] C：字符串复制
来源：http://rjj.yueranfly.top

char dst[32]; strcpy(dst, "hi");
来源：http://wvi.xuetiantiany.cn

[S05] C：字符串长度
来源：http://luy.cucudq.cn

strlen(s)
来源：http://jnr.ctjpmb.com

[S06] C：字符串比较
来源：http://bse.316326.xyz

strcmp(a, b) == 0
来源：http://kxx.ctjpmb.com

[S07] C：数组遍历求和
来源：http://lsm.zdqjudy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dgh.jianghu66.top

[S08] C：动态内存分配与释放
来源：http://dex.shuidangran.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pgp.daxiang520.top

[S09] C：结构体定义与初始化
来源：http://kar.wangdashe.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ojq.zycfv.cn

[S10] C：指针与解引用
来源：http://jiz.nanxinkj.top

int *p = &a;  *p = 5;
来源：http://pia.0kj1m.cn

[S11] C：逐行读文件
来源：http://erz.mhx1999.top

FILE *f = fopen("a.txt", "r");
来源：http://qts.hcnkem.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://bin.zycfv.cn

fclose(f);
来源：http://ruv.haohaochexian.top

[S12] C：写文件
来源：http://evb.yvedp.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vjj.yj20258.top

[S13] C：宏定义
来源：http://idi.birdmap.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oxg.nanxinkj.top

[S14] C：枚举
来源：http://fbo.c1oappe.top

enum Color { RED, GREEN, BLUE };
来源：http://hoe.ctjpmb.com

[S15] C：类型转换
来源：http://sib.tianlin.xyz

(double) a / b
来源：http://iro.yuanzhike.top

[S16] C：位操作置位
来源：http://kmx.yonumen.top

x |= (1 << 3);
来源：http://ldc.wangdashe.top

[S17] C：安全拼接字符串
来源：http://vil.cheryme.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bag.zhengqikj.top

[S18] C：命令行参数
来源：http://lig.nwbrower.top

int main(int argc, char **argv)
来源：http://ntl.9152youxi.cn

[S19] C：快速排序
来源：http://plv.xuetiantiany.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zik.hfpthk.cn

[S20] C：二分查找
来源：http://usg.zhijiandao.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bsj.sweek.top

[S21] C：字符类别判断
来源：http://xia.jqgufenzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://amy.nwbrower.top

[S22] C：字符串转数字
来源：http://qbf.tarul.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zfd.cheryme.top

[S23] C：随机数
来源：http://gwq.pengpengdd.cyou

srand(time(NULL));  int r = rand() % 100;
来源：http://fuf.fzhhl.top

[S24] C：获取本地时间
来源：http://fpo.ydzc1.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xdk.yfazqb.com

[S25] C：内存拷贝
来源：http://cip.yfazqb.com

memcpy(dst, src, n);
来源：http://qpq.zhaomingkeji.xyz

[S26] C：内存清零
来源：http://qfn.fzhhl.top

memset(a, 0, sizeof a);
来源：http://avx.meibo888.top

[S27] C：定义常量
来源：http://xcg.dashuyun.cn

const double PI = 3.14159;
来源：http://zyr.sysykeji.top

[S28] C：静态变量
来源：http://mqu.ydzc1.top

static int counter = 0;
来源：http://koh.yj20258.top

[S29] C：变参函数
来源：http://lgx.cqqwz.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lis.bjfxy.top

[S30] C：头文件保护
来源：http://nsz.xylfe.cn

#ifndef X_H
来源：http://zlj.52xcode.cn

#define X_H
来源：http://tll.tarul.cn

#endif
来源：http://zjy.guannengcc.top

[S31] C++：Hello World
来源：http://yev.jinqigfzy.top

#include <iostream>
来源：http://mul.shanyushiyangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://nxt.hfpthk.cn

[S32] C++：字符串
来源：http://hup.nanxinkj.top

std::string s = "hi";  s += "!";
来源：http://jfw.yuanzhike.top

[S33] C++：vector 增删
来源：http://anl.hesvh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://skz.ivvv.top

[S34] C++：遍历 vector
来源：http://pzp.cdnleiting.top

for (auto &x : v) { std::cout << x; }
来源：http://xyu.fehbvm.com

[S35] C++：map
来源：http://yqx.wangshuangyany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qwg.gaohongyu789.top

[S36] C++：unordered_map
来源：http://tme.zycfv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hyf.smart0.xyz

[S37] C++：set
来源：http://yyn.jlsjyb.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fui.yvedp.cn

[S38] C++：排序
来源：http://kyu.yuanzhike.top

std::sort(v.begin(), v.end());
来源：http://aes.pengpengdd.cyou

[S39] C++：自定义比较器排序
来源：http://zit.nanxinkj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://odi.mhx1999.top

[S40] C++：查找元素
来源：http://awa.316326.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lkp.feifeiyinyue.top

[S41] C++：类与构造函数
来源：http://jmr.zdqjudy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zxi.snrcjt.cn

[S42] C++：继承与虚函数
来源：http://xqq.yj20258.top

class B : public Base { public: void f() override {} };
来源：http://noo.iojbl.cn

[S43] C++：智能指针
来源：http://sqv.havefunace.top

auto p = std::make_unique<int>(5);
来源：http://xkl.fehbvm.com

[S44] C++：引用传参
来源：http://gyy.hesvh.cn

void inc(int &x) { ++x; }
来源：http://czn.wangdashe.top

[S45] C++：lambda
来源：http://ano.tarul.cn

auto add = [](int a, int b) { return a + b; };
来源：http://two.jqgfzy.top

[S46] C++：函数模板
来源：http://qpd.shanyushiyangtech.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vmn.yj202588.top

[S47] C++：结构化绑定遍历
来源：http://lxh.cucudq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nls.nwbrower.top

[S48] C++：逐行读文件
来源：http://dui.cdnleiting.top

std::ifstream in("a.txt");  std::string line;
来源：http://jat.hammf.cn

while (std::getline(in, line)) { }
来源：http://rsr.yfazqb.com

[S49] C++：写文件
来源：http://xok.pycfn.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dyp.fehbvm.com

[S50] C++：格式化数字
来源：http://nbv.ehwqpu.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hpc.andypj.xyz

[S51] C++：显式类型转换
来源：http://bem.hcnkem.com

static_cast<double>(a) / b
来源：http://vrw.cucudq.cn

[S52] C++：const 与 noexcept
来源：http://cad.uphjek.com

int size() const noexcept { return n_; }
来源：http://epw.kuanghao11.cn

[S53] C++：移动语义
来源：http://jld.hesvh.cn

std::vector<int> w = std::move(v);
来源：http://lla.cashguo.top

[S54] C++：异常处理
来源：http://dnh.ctjpmb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yku.kuanghao11.cn

[S55] C++：结构化绑定
来源：http://xvg.daria6918.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rtw.yj20258.top

[S56] C++：optional
来源：http://ame.daxiang520.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://asu.bbcook.cn

[S57] C++：编译期常量
来源：http://vwf.zhiwuduotai.top

constexpr int N = 10;
来源：http://zpm.vqdsnc.cn

[S58] C++：命名空间
来源：http://wvy.yj20258888.top

namespace ns { int f() { return 1; } }
来源：http://nmv.gogol.net.cn

[S59] C++：静态断言
来源：http://wdd.jyoumei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kyu.daria6918.cn

[S60] C++：遍历并删除元素
来源：http://wzo.xylfe.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fen.yuxming.cn

================================================================================
来源：http://dlr.fengsongda.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://osg.epnwcf.com

================================================================================
来源：http://eis.guannengcc.top

[T01] Kotlin：Hello World
来源：http://uoa.ybcxt.top

println("Hello")
来源：http://ony.jinyuanbaomall.cn

[T02] Kotlin：变量
来源：http://mcm.hywenlv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hdb.pycfn.com

[T03] Kotlin：字符串模板
来源：http://uih.jinghuilouyu.cn

"值: $b"
来源：http://jst.nanxuanxn.top

[T04] Kotlin：空安全
来源：http://vqc.9152youxi.cn

val n: String? = null;  n?.length
来源：http://mms.feifeiyinyue.top

[T05] Kotlin：when 表达式
来源：http://yxu.c1oappe.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dic.sjlbkw.cn

[T06] Kotlin：集合映射
来源：http://vvm.feifeiyinyue.top

listOf(1, 2, 3).map { it * 2 }
来源：http://lbu.jyoumei.cn

[T07] Kotlin：集合过滤
来源：http://mur.daxiang520.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rea.tarul.cn

[T08] Kotlin：数据类
来源：http://fwq.zycfv.cn

data class User(val name: String, val age: Int)
来源：http://vdu.fanxiaobao.xyz

[T09] Kotlin：扩展函数
来源：http://fnv.snrcjt.cn

fun String.exclaim() = this + "!"
来源：http://wyg.zycfv.cn

[T10] Kotlin：默认参数
来源：http://sgg.redwolf501.top

fun greet(name: String = "World") = "Hi $name"
来源：http://quk.yvedp.cn

[T11] Kotlin：协程
来源：http://exq.xingfuxueyuan.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://rdy.ivvv.top

[T12] Kotlin：解构声明
来源：http://mbi.yuxming.cn

val (a, b) = Pair(1, 2)
来源：http://qci.yonumen.top

[T13] Kotlin：只读 Map
来源：http://tmg.hfpthk.cn

val m = mapOf("a" to 1)
来源：http://usm.vehdjk.com

[T14] Kotlin：循环
来源：http://rap.0kj1m.cn

for (i in 1..10) println(i)
来源：http://frd.fzhhl.top

[T15] Kotlin：接口
来源：http://euu.hnxiangtu.top

interface Shape { fun area(): Double }
来源：http://wjo.ybcxt.top

[T16] Swift：Hello World
来源：http://gmu.gaohongyu789.top

print("Hello")
来源：http://nqf.zhijiandao.cn


<!-- 参考信息 -->