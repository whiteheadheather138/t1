代发 wailian999

case "$1" in
来源：http://cjg.xuanzx.com

start) echo "启动" ;;
来源：http://iup.ivvv.top

stop)  echo "停止" ;;
来源：http://oiu.tarul.cn

*)     echo "未知命令" ;;
来源：http://ciz.sjlbkw.cn

esac
来源：http://lsu.tian-w.cn

[R12] for 遍历文件
来源：http://dyx.sweek.top

for f in *.txt; do echo "$f"; done
来源：http://jvq.sysykeji.top

[R13] for 计数循环
来源：http://ins.redwolf501.top

for i in {1..10}; do echo "$i"; done
来源：http://fue.snrcjt.cn

[R14] C 风格 for
来源：http://tqp.tianlin.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ltk.cucudq.cn

[R15] while 逐行读文件
来源：http://obx.fktsv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rmg.sxryk.cn

[R16] until 等待条件
来源：http://euc.zdbjq.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yvs.haohaochexian.top

[R17] 数组定义与取值
来源：http://kcb.tian-w.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mwh.jiagoushi.top

[R18] 遍历数组
来源：http://anw.quarkkingdee.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qxj.svipenyu.cn

[R19] 数组长度
来源：http://khx.xinyue.icu

echo "${#arr[@]}"
来源：http://kzb.sjlbkw.cn

[R20] 关联数组（字典）
来源：http://ssn.tarul.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mka.zycfv.cn

[R21] 字符串长度
来源：http://vwp.andypj.xyz

echo "${#s}"
来源：http://rnc.tanke756.top

[R22] 截取子串
来源：http://wrh.epnwcf.com

echo "${s:0:5}"
来源：http://okg.yanxiufei.cn

[R23] 字符串替换
来源：http://xhs.hysaishi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://axz.shanyushiyangtech.top

[R24] 大小写转换
来源：http://lyk.nanxuanxn.top

echo "${s^^}"; echo "${s,,}"
来源：http://qzc.zhixingplan.top

[R25] 去后缀 / 去前缀
来源：http://nos.tarul.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hlz.yangfankeji.com

[R26] 命令替换
来源：http://wxx.hcnkem.com

now=$(date +%F); echo "$now"
来源：http://zot.cqqwz.cn

[R27] 算术展开
来源：http://vjc.gaohongyu789.top

echo $((1 + 2 * 3))
来源：http://lji.hnxiangtu.top

[R28] 浮点运算
来源：http://jhg.dashuyun.cn

echo "scale=2; 10/3" | bc
来源：http://pue.zhaomingkeji.xyz

[R29] 定义函数
来源：http://pvq.sxryk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qhv.vehdjk.com

[R30] 函数返回状态码
来源：http://ztr.sweek.top

f() { return 0; }; f || echo "失败了"
来源：http://pgh.aizwys.cn

[R31] 局部变量
来源：http://vmc.fzhhl.top

f() { local x=1; echo "$x"; }
来源：http://mfo.sufxvd.cn

[R32] 参数个数校验
来源：http://suh.yj202588.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bja.snrcjt.cn

[R33] 捕获错误并提示行号
来源：http://kqz.hysaishi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ufi.ehwqpu.com

[R34] 退出时清理
来源：http://iro.zhixingplan.top

trap 'rm -f "$tmp"' EXIT
来源：http://yon.shuidangran.top

[R35] 后台执行并等待
来源：http://wtj.ydjk.org.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qae.yongpay.top

[R36] 并发执行多个任务
来源：http://hag.0kj1m.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dfi.birdmap.top

[R37] 把输出赋给变量
来源：http://wyl.feifeiyinyue.top

files=$(ls -1)
来源：http://pkm.yuxming.cn

[R38] 管道串联
来源：http://mot.gotoacloud.top

cat a.txt | grep -i error | wc -l
来源：http://uol.hywenlv.cn

[R39] 重定向标准输出与错误
来源：http://big.hysaishi.cn

cmd > out.log 2>&1
来源：http://huk.ivvv.top

[R40] 追加写日志
来源：http://ihm.cheryme.top

echo "log" >> out.log
来源：http://buj.cashguo.top

[R41] 丢弃输出
来源：http://ecr.nanxuanxn.top

cmd >/dev/null 2>&1
来源：http://xcm.shanyushiyangtech.top

[R42] 输入重定向
来源：http://blv.nanxinkj.top

wc -l < a.txt
来源：http://mqp.zhixingplan.top

[R43] 按名字查找文件
来源：http://ziy.cheryme.top

find . -name "*.log" -type f
来源：http://pif.pengpengdd.cyou

[R44] 按修改时间查找
来源：http://kob.yfazqb.com

find . -mtime -7 -type f
来源：http://wrv.hnxiangtu.top

[R45] 批量删除
来源：http://hxy.zhiwuduotai.top

find . -name "*.tmp" -delete
来源：http://kmx.tianlin.xyz

[R46] 递归替换文件内容
来源：http://qom.gotoacloud.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nny.zhongyouzk.top

[R47] sed 单行替换
来源：http://qnk.quarkkingdee.top

sed -i 's/foo/bar/g' a.txt
来源：http://wcy.hammf.cn

[R48] awk 取指定列
来源：http://yud.0kj1m.cn

awk '{print $1, $3}' a.txt
来源：http://oce.daria6918.cn

[R49] awk 带条件
来源：http://lut.hywenlv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gcb.ivvv.top

[R50] awk 求和
来源：http://nrq.bbcook.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ssd.uphjek.com

[R51] 排序去重取前几
来源：http://vwz.yvedp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rye.gogol.net.cn

[R52] 统计行数
来源：http://btw.zhongyouzk.top

wc -l a.txt
来源：http://bji.yj202588.top

[R53] 查看文件头与实时尾
来源：http://tlk.zhiwuduotai.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ccf.jlsjyb.cn

[R54] 比较两个文件
来源：http://gom.quarkkingdee.top

diff a.txt b.txt
来源：http://xxr.yj20258.top

[R55] 压缩与解压
来源：http://cjn.hywenlv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xxc.52xcode.cn

[R56] 远程拷贝
来源：http://boz.vehdjk.com

scp file user@host:/path/
来源：http://ukt.xziqi.cn

[R57] 远程执行命令
来源：http://fxb.xinyue.icu

ssh user@host 'uptime'
来源：http://abd.yonumen.top

[R58] 下载文件
来源：http://vjl.hammf.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ggt.andypj.xyz

[R59] 发 POST JSON
来源：http://dlh.shanyushiyangtech.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rhc.mhx1999.top

[R60] 只看 HTTP 状态码
来源：http://uzg.shanyushiyangtech.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bka.meibo888.top

[R61] 磁盘占用
来源：http://pso.shzxlz.cn

df -h;  du -sh *
来源：http://hzp.daxiang520.top

[R62] 找最占空间的文件
来源：http://bgo.feifeiyinyue.top

du -ah . | sort -rh | head -10
来源：http://tkx.yj202588.top

[R63] 内存与进程
来源：http://kuw.ywan-chungtsiang.top

free -h;  ps aux | grep nginx
来源：http://miq.sufxvd.cn

[R64] 结束进程
来源：http://ogk.shanyushiyangtech.top

kill -9 $(pgrep -f app.py)
来源：http://agh.haohaochexian.top

[R65] 查看端口占用
来源：http://vpz.fzhhl.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ibg.gogol.net.cn

[R66] 定时任务
来源：http://vrr.jqgufenzy.top

crontab -e;  crontab -l
来源：http://evg.sufxvd.cn

[R67] 生成随机十六进制串
来源：http://vtu.havefunace.top

openssl rand -hex 16
来源：http://eup.chenzaomai.com

[R68] 计算文件校验值
来源：http://uhs.tian-w.cn

sha256sum a.txt;  md5sum a.txt
来源：http://spt.9152youxi.cn

[R69] 生成随机密码
来源：http://qhz.cheryme.top

head -c 16 /dev/urandom | base64
来源：http://eiu.daria6918.cn

[R70] 时间戳与互转
来源：http://dsr.guannengcc.top

date +%s;  date -d @1700000000
来源：http://gjb.tarul.cn

[R71] 日期格式化
来源：http://ioj.uphjek.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://grc.cdnleiting.top

[R72] 等待端口就绪
来源：http://btj.jlsjyb.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://oxp.hysaishi.cn

[R73] 分割大日志
来源：http://xjs.fzhhl.top

split -l 1000 big.log part_
来源：http://tgo.andypj.xyz

[R74] 批量重命名
来源：http://qts.iojbl.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zxu.chenlongwang.top

[R75] 导出环境变量
来源：http://okz.gaohongyu789.top

export PATH="$HOME/bin:$PATH"
来源：http://xob.ywan-chungtsiang.top

[R76] 使用临时文件
来源：http://gxg.fanxiaobao.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ekk.ydjk.org.cn

[R77] 读取用户输入
来源：http://hdl.ctjpmb.com

read -rp "请输入: " ans
来源：http://yyl.chenlongwang.top

[R78] 交互式菜单
来源：http://yhx.pycfn.com

select opt in a b c; do echo "$opt"; break; done
来源：http://ahl.zycfv.cn

[R79] 解析命令行选项
来源：http://qid.shangyingyoupin.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kxt.sweek.top

[R80] 查看脚本执行耗时
来源：http://pll.tian-w.cn

time ./run.sh
来源：http://twu.fehbvm.com

================================================================================
来源：http://tkz.tian-w.cn

S. C / C++ 专题
来源：http://wme.ydzc1.top

================================================================================
来源：http://ggi.yj20258.top

[S01] C：Hello World
来源：http://prw.zhiwuduotai.top

#include <stdio.h>
来源：http://kbv.havefunace.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://sln.gotoacloud.top

[S02] C：变量与格式化输出
来源：http://cud.jlsjyb.cn

int a = 10; printf("%d\n", a);
来源：http://jpq.xuanzx.com

[S03] C：读入整数
来源：http://vyg.sweek.top

int x; scanf("%d", &x);
来源：http://gsp.jlsjyb.cn

[S04] C：字符串复制
来源：http://mum.cqqwz.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ged.epnwcf.com

[S05] C：字符串长度
来源：http://fia.sweek.top

strlen(s)
来源：http://xft.zhaomingkeji.xyz

[S06] C：字符串比较
来源：http://xbs.redwolf501.top

strcmp(a, b) == 0
来源：http://nyt.yvedp.cn

[S07] C：数组遍历求和
来源：http://ozt.guannengcc.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://suz.cqqwz.cn

[S08] C：动态内存分配与释放
来源：http://gtc.316326.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mfz.fengsongda.top

[S09] C：结构体定义与初始化
来源：http://nrf.jianghu66.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://aez.fanxiaobao.xyz

[S10] C：指针与解引用
来源：http://xng.zhijiandao.cn

int *p = &a;  *p = 5;
来源：http://wzk.shangyingyoupin.top

[S11] C：逐行读文件
来源：http://ujq.guannengcc.top

FILE *f = fopen("a.txt", "r");
来源：http://lzo.zhijiandao.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pdg.wangdashe.top

fclose(f);
来源：http://tbe.dashuyun.cn

[S12] C：写文件
来源：http://ioj.shanyushiyangtech.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zvj.birdmap.top

[S13] C：宏定义
来源：http://stf.zycfv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qts.hnxiangtu.top

[S14] C：枚举
来源：http://zdh.jinqigfzy.top

enum Color { RED, GREEN, BLUE };
来源：http://lod.daria6918.cn

[S15] C：类型转换
来源：http://ibh.shanyushiyangtech.top

(double) a / b
来源：http://sfy.cdnleiting.top

[S16] C：位操作置位
来源：http://tuz.shanyushiyangkeji.top

x |= (1 << 3);
来源：http://jzf.haohaochexian.top

[S17] C：安全拼接字符串
来源：http://nyx.sufxvd.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://grd.meibo888.top

[S18] C：命令行参数
来源：http://pus.tanke756.top

int main(int argc, char **argv)
来源：http://lep.cheryme.top

[S19] C：快速排序
来源：http://fhh.gaohongyu789.top

qsort(a, n, sizeof(int), cmp);
来源：http://ftl.aibaodan.cn

[S20] C：二分查找
来源：http://oqk.aizwys.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pnt.zhixingplan.top

[S21] C：字符类别判断
来源：http://svc.zhaomingkeji.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fzt.cheryme.top

[S22] C：字符串转数字
来源：http://kpe.fanxiaobao.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://rke.wangdashe.top

[S23] C：随机数
来源：http://exk.shanyushiyangkeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ngz.nanxinkj.top

[S24] C：获取本地时间
来源：http://lqu.tarul.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tay.52xcode.cn

[S25] C：内存拷贝
来源：http://bfn.gzhubu.top

memcpy(dst, src, n);
来源：http://tmq.cheryme.top

[S26] C：内存清零
来源：http://shg.gogol.net.cn

memset(a, 0, sizeof a);
来源：http://xzj.ydzc1.top

[S27] C：定义常量
来源：http://dey.xuetiantiany.cn

const double PI = 3.14159;
来源：http://jlg.uphjek.com

[S28] C：静态变量
来源：http://ppq.dianchejie.cn

static int counter = 0;
来源：http://ttz.feifeiyinyue.top

[S29] C：变参函数
来源：http://pqo.nanxuanxn.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://axr.yj20258888.top

[S30] C：头文件保护
来源：http://nxm.sxryk.cn

#ifndef X_H
来源：http://ugr.jinghuilouyu.cn

#define X_H
来源：http://kvy.xinyue.icu

#endif
来源：http://kvn.c1oappe.top

[S31] C++：Hello World
来源：http://ebp.hesvh.cn

#include <iostream>
来源：http://gau.tian-w.cn

int main() { std::cout << "Hello\n"; }
来源：http://yew.nanxinkj.top

[S32] C++：字符串
来源：http://mqz.aibaodan.cn

std::string s = "hi";  s += "!";
来源：http://xyz.guannengcc.top

[S33] C++：vector 增删
来源：http://fhi.fehbvm.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uqo.shzxlz.cn

[S34] C++：遍历 vector
来源：http://jbf.cdnleiting.top

for (auto &x : v) { std::cout << x; }
来源：http://xlp.fengsongda.top

[S35] C++：map
来源：http://dop.sjlbkw.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nfz.wangshuangyany.cn

[S36] C++：unordered_map
来源：http://exf.tarul.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qge.ywan-chungtsiang.top

[S37] C++：set
来源：http://hkx.wangdashe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bgq.nanxuanxn.top

[S38] C++：排序
来源：http://dic.yongpay.top

std::sort(v.begin(), v.end());
来源：http://pln.cqqwz.cn

[S39] C++：自定义比较器排序
来源：http://rhj.yongpay.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cmp.gogol.net.cn

[S40] C++：查找元素
来源：http://yzd.ehwqpu.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fmv.zhengqikj.top

[S41] C++：类与构造函数
来源：http://bab.tianlin.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lvj.jqgufenzy.top

[S42] C++：继承与虚函数
来源：http://htw.havefunace.top

class B : public Base { public: void f() override {} };
来源：http://kyi.hammf.cn

[S43] C++：智能指针
来源：http://fya.52xcode.cn

auto p = std::make_unique<int>(5);
来源：http://xpv.52xcode.cn

[S44] C++：引用传参
来源：http://qyz.52xcode.cn

void inc(int &x) { ++x; }
来源：http://ijf.pengpengdd.cyou

[S45] C++：lambda
来源：http://tgb.ydzc1.top

auto add = [](int a, int b) { return a + b; };
来源：http://fty.hcnkem.com

[S46] C++：函数模板
来源：http://sxj.jinqigfzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://knn.shuidangran.top

[S47] C++：结构化绑定遍历
来源：http://gai.cucudq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://aml.zhiwuduotai.top

[S48] C++：逐行读文件
来源：http://yea.shzxlz.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wxh.tarul.cn

while (std::getline(in, line)) { }
来源：http://hhk.hesvh.cn

[S49] C++：写文件
来源：http://unb.hongshengwenyu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cfe.zhoulong.xyz

[S50] C++：格式化数字
来源：http://xui.cheryme.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hup.hywenlv.cn

[S51] C++：显式类型转换
来源：http://lwn.yangfankeji.com

static_cast<double>(a) / b
来源：http://rml.hammf.cn

[S52] C++：const 与 noexcept
来源：http://rbf.aibaodan.cn

int size() const noexcept { return n_; }
来源：http://jka.svipenyu.cn

[S53] C++：移动语义
来源：http://gow.dianchejie.cn

std::vector<int> w = std::move(v);
来源：http://xdj.fanxiaobao.xyz

[S54] C++：异常处理
来源：http://iyr.yj202588.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qzt.hnqzz.top

[S55] C++：结构化绑定
来源：http://zeh.yongpay.top

auto [a, b] = std::make_pair(1, 2);
来源：http://duq.ctjpmb.com

[S56] C++：optional
来源：http://bgw.zhixingplan.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lzx.ydjk.org.cn

[S57] C++：编译期常量
来源：http://uea.yanxiufei.cn

constexpr int N = 10;
来源：http://qbh.shangyingyoupin.top

[S58] C++：命名空间
来源：http://ifi.chenlongwang.top

namespace ns { int f() { return 1; } }
来源：http://ehx.smart0.xyz

[S59] C++：静态断言
来源：http://yhc.yongpay.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://quc.snrcjt.cn

[S60] C++：遍历并删除元素
来源：http://kyz.zhaomingkeji.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sdk.xinyue.icu

================================================================================
来源：http://ssd.smart0.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zmn.gaohongyu789.top

================================================================================
来源：http://qna.ppjwa.cn

[T01] Kotlin：Hello World
来源：http://nnp.dashuyun.cn

println("Hello")
来源：http://dmd.shuidangran.top

[T02] Kotlin：变量
来源：http://sul.52xcode.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gdc.jinghuilouyu.cn

[T03] Kotlin：字符串模板
来源：http://wax.xylfe.cn

"值: $b"
来源：http://mzc.hywenlv.cn

[T04] Kotlin：空安全
来源：http://gik.hfpthk.cn

val n: String? = null;  n?.length
来源：http://kii.ybcxt.top

[T05] Kotlin：when 表达式
来源：http://wvz.havefunace.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ier.sjlbkw.cn

[T06] Kotlin：集合映射
来源：http://qca.hcnkem.com

listOf(1, 2, 3).map { it * 2 }
来源：http://pmc.jianghu66.top

[T07] Kotlin：集合过滤
来源：http://laf.yuanzhike.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://etw.zhixingplan.top

[T08] Kotlin：数据类
来源：http://rkj.shanyushiyangkeji.top

data class User(val name: String, val age: Int)
来源：http://raz.hammf.cn

[T09] Kotlin：扩展函数
来源：http://vax.guannengcc.top

fun String.exclaim() = this + "!"
来源：http://klq.guannengcc.top

[T10] Kotlin：默认参数
来源：http://exb.yj202588.top

fun greet(name: String = "World") = "Hi $name"
来源：http://zge.yj20258.top

[T11] Kotlin：协程
来源：http://tln.sweek.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://too.redwolf501.top

[T12] Kotlin：解构声明
来源：http://enp.yongpay.top

val (a, b) = Pair(1, 2)
来源：http://amk.fzhhl.top


<!-- 参考信息 -->