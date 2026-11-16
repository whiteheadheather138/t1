代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mcw.gogol.net.cn

[R08] 数值比较
来源：http://wpy.yangfankeji.com

if (( a > b )); then echo "a 更大"; fi
来源：http://qry.bbcook.cn

[R09] 字符串比较
来源：http://ogx.tianlin.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://grg.yanxiufei.cn

[R10] 正则匹配
来源：http://jme.fzhhl.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kdi.nanxuanxn.top

[R11] case 多分支
来源：http://wpb.tianlin.xyz

case "$1" in
来源：http://hcr.hnxiangtu.top

start) echo "启动" ;;
来源：http://bat.pycfn.com

stop)  echo "停止" ;;
来源：http://knk.cashguo.top

*)     echo "未知命令" ;;
来源：http://mah.nanxinkj.top

esac
来源：http://ojc.redwolf501.top

[R12] for 遍历文件
来源：http://yhp.pycfn.com

for f in *.txt; do echo "$f"; done
来源：http://sje.bbcook.cn

[R13] for 计数循环
来源：http://ewa.fktsv.cn

for i in {1..10}; do echo "$i"; done
来源：http://nfc.shzxlz.cn

[R14] C 风格 for
来源：http://khf.zhaomingkeji.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ttx.tarul.cn

[R15] while 逐行读文件
来源：http://yyd.yj20258888.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pbk.epnwcf.com

[R16] until 等待条件
来源：http://uxs.hongshengwenyu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xva.uphjek.com

[R17] 数组定义与取值
来源：http://puj.xuanzx.com

arr=(a b c); echo "${arr[0]}"
来源：http://iaa.guannengcc.top

[R18] 遍历数组
来源：http://dby.sxryk.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://brg.shangyingyoupin.top

[R19] 数组长度
来源：http://dzz.zhongyouzk.top

echo "${#arr[@]}"
来源：http://sdw.gotoacloud.top

[R20] 关联数组（字典）
来源：http://svr.tarul.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rej.yonumen.top

[R21] 字符串长度
来源：http://cfs.52xcode.cn

echo "${#s}"
来源：http://jmz.jiagoushi.top

[R22] 截取子串
来源：http://sbg.meibo888.top

echo "${s:0:5}"
来源：http://vsn.zhongyouzk.top

[R23] 字符串替换
来源：http://cmt.xuanzx.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tzh.andypj.xyz

[R24] 大小写转换
来源：http://yyt.cdnleiting.top

echo "${s^^}"; echo "${s,,}"
来源：http://fwp.ydzc1.top

[R25] 去后缀 / 去前缀
来源：http://nyc.meibo888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://afa.aibaodan.cn

[R26] 命令替换
来源：http://atf.guowangkeji.top

now=$(date +%F); echo "$now"
来源：http://zqj.xingfuxueyuan.xyz

[R27] 算术展开
来源：http://dqx.andypj.xyz

echo $((1 + 2 * 3))
来源：http://bby.wangdashe.top

[R28] 浮点运算
来源：http://gsf.yueranfly.top

echo "scale=2; 10/3" | bc
来源：http://jap.jqgfzy.top

[R29] 定义函数
来源：http://jnx.ehwqpu.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bwd.hywenlv.cn

[R30] 函数返回状态码
来源：http://qfy.fengsongda.top

f() { return 0; }; f || echo "失败了"
来源：http://nrp.jqgufenzy.top

[R31] 局部变量
来源：http://bic.yangfankeji.com

f() { local x=1; echo "$x"; }
来源：http://kcg.nanxuanxn.top

[R32] 参数个数校验
来源：http://eao.fanxiaobao.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jpw.quarkkingdee.top

[R33] 捕获错误并提示行号
来源：http://wfs.sysykeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wbi.yj20258.top

[R34] 退出时清理
来源：http://uzj.gzhubu.top

trap 'rm -f "$tmp"' EXIT
来源：http://usl.gogol.net.cn

[R35] 后台执行并等待
来源：http://qna.andypj.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://uxn.gogol.net.cn

[R36] 并发执行多个任务
来源：http://vkf.ydzc1.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lda.c1oappe.top

[R37] 把输出赋给变量
来源：http://cyc.9152youxi.cn

files=$(ls -1)
来源：http://sts.dianchejie.cn

[R38] 管道串联
来源：http://gop.jinqigufen.top

cat a.txt | grep -i error | wc -l
来源：http://kdk.kuanghao11.cn

[R39] 重定向标准输出与错误
来源：http://wtc.jinqigufen.top

cmd > out.log 2>&1
来源：http://ink.c1oappe.top

[R40] 追加写日志
来源：http://kfm.hywenlv.cn

echo "log" >> out.log
来源：http://gmk.ctjpmb.com

[R41] 丢弃输出
来源：http://zzq.cashguo.top

cmd >/dev/null 2>&1
来源：http://eqn.0kj1m.cn

[R42] 输入重定向
来源：http://nru.yj202588.top

wc -l < a.txt
来源：http://fod.birdmap.top

[R43] 按名字查找文件
来源：http://cuk.hammf.cn

find . -name "*.log" -type f
来源：http://avr.tianlin.xyz

[R44] 按修改时间查找
来源：http://lhz.nanxinkj.top

find . -mtime -7 -type f
来源：http://afe.nwbrower.top

[R45] 批量删除
来源：http://bvw.nanxinkj.top

find . -name "*.tmp" -delete
来源：http://xmq.hesvh.cn

[R46] 递归替换文件内容
来源：http://bhu.yueranfly.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wml.sxryk.cn

[R47] sed 单行替换
来源：http://nkh.zhixingplan.top

sed -i 's/foo/bar/g' a.txt
来源：http://gmd.yangfankeji.com

[R48] awk 取指定列
来源：http://snf.quarkkingdee.top

awk '{print $1, $3}' a.txt
来源：http://ask.xziqi.cn

[R49] awk 带条件
来源：http://slv.iojbl.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://koc.zycfv.cn

[R50] awk 求和
来源：http://qgk.yanxiufei.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dkq.bbcook.cn

[R51] 排序去重取前几
来源：http://ily.yj20258.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ixa.fzhhl.top

[R52] 统计行数
来源：http://bdp.xuanzx.com

wc -l a.txt
来源：http://rln.fehbvm.com

[R53] 查看文件头与实时尾
来源：http://nfz.zhiwuduotai.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rxt.jqgfzy.top

[R54] 比较两个文件
来源：http://qnt.andypj.xyz

diff a.txt b.txt
来源：http://enx.yj20258.top

[R55] 压缩与解压
来源：http://its.zdqjudy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://txn.tarul.cn

[R56] 远程拷贝
来源：http://mbd.0kj1m.cn

scp file user@host:/path/
来源：http://epn.hesvh.cn

[R57] 远程执行命令
来源：http://bbb.ydzc1.top

ssh user@host 'uptime'
来源：http://uby.gaohongyu789.top

[R58] 下载文件
来源：http://qln.jqgufenzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hbg.fengsongda.top

[R59] 发 POST JSON
来源：http://uxk.fktsv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vbp.nanxinkj.top

[R60] 只看 HTTP 状态码
来源：http://pwg.jqgfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gqt.shanyushiyangkeji.top

[R61] 磁盘占用
来源：http://zan.sweek.top

df -h;  du -sh *
来源：http://coy.dianchejie.cn

[R62] 找最占空间的文件
来源：http://mmi.vqdsnc.cn

du -ah . | sort -rh | head -10
来源：http://rcc.jlsjyb.cn

[R63] 内存与进程
来源：http://vuc.jinqigufen.top

free -h;  ps aux | grep nginx
来源：http://ygx.hesvh.cn

[R64] 结束进程
来源：http://aut.hysaishi.cn

kill -9 $(pgrep -f app.py)
来源：http://wpi.shzxlz.cn

[R65] 查看端口占用
来源：http://irw.tarul.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kpd.zdqjudy.top

[R66] 定时任务
来源：http://gyv.hfpthk.cn

crontab -e;  crontab -l
来源：http://nto.birdmap.top

[R67] 生成随机十六进制串
来源：http://nlc.cqqwz.cn

openssl rand -hex 16
来源：http://gmc.nanxinkj.top

[R68] 计算文件校验值
来源：http://wcy.hnxiangtu.top

sha256sum a.txt;  md5sum a.txt
来源：http://znr.cashguo.top

[R69] 生成随机密码
来源：http://hzf.kuanghao11.cn

head -c 16 /dev/urandom | base64
来源：http://cbh.52xcode.cn

[R70] 时间戳与互转
来源：http://nxp.jianghu66.top

date +%s;  date -d @1700000000
来源：http://ssy.fanxiaobao.xyz

[R71] 日期格式化
来源：http://kjw.c1oappe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://nhy.cucudq.cn

[R72] 等待端口就绪
来源：http://njp.andypj.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://ywq.feifeiyinyue.top

[R73] 分割大日志
来源：http://ghz.tarul.cn

split -l 1000 big.log part_
来源：http://mzp.cqqwz.cn

[R74] 批量重命名
来源：http://uyp.kuanghao11.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kyd.guowangkeji.top

[R75] 导出环境变量
来源：http://lyg.pycfn.com

export PATH="$HOME/bin:$PATH"
来源：http://wnf.fanxiaobao.xyz

[R76] 使用临时文件
来源：http://jys.zhijiandao.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tuq.nanxinkj.top

[R77] 读取用户输入
来源：http://lzn.sysykeji.top

read -rp "请输入: " ans
来源：http://cjz.birdmap.top

[R78] 交互式菜单
来源：http://dil.fktsv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://thp.jqgfzy.top

[R79] 解析命令行选项
来源：http://goy.pycfn.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wzl.shuidangran.top

[R80] 查看脚本执行耗时
来源：http://puy.iojbl.cn

time ./run.sh
来源：http://vko.sjlbkw.cn

================================================================================
来源：http://hif.jiagoushi.top

S. C / C++ 专题
来源：http://amy.sysykeji.top

================================================================================
来源：http://jxw.sysykeji.top

[S01] C：Hello World
来源：http://gmo.yangfankeji.com

#include <stdio.h>
来源：http://xlr.yj20258.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://pha.birdmap.top

[S02] C：变量与格式化输出
来源：http://ibo.fengsongda.top

int a = 10; printf("%d\n", a);
来源：http://jak.jianghu66.top

[S03] C：读入整数
来源：http://pzx.0kj1m.cn

int x; scanf("%d", &x);
来源：http://qog.yongpay.top

[S04] C：字符串复制
来源：http://nxl.cashguo.top

char dst[32]; strcpy(dst, "hi");
来源：http://xwf.xuanzx.com

[S05] C：字符串长度
来源：http://czw.ydjk.org.cn

strlen(s)
来源：http://rou.fengsongda.top

[S06] C：字符串比较
来源：http://pzf.snrcjt.cn

strcmp(a, b) == 0
来源：http://yab.yfazqb.com

[S07] C：数组遍历求和
来源：http://qir.zhengqikj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://upv.cucudq.cn

[S08] C：动态内存分配与释放
来源：http://tee.nanxuanxn.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wgb.iojbl.cn

[S09] C：结构体定义与初始化
来源：http://zjs.fanxiaobao.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rfs.yfazqb.com

[S10] C：指针与解引用
来源：http://nbq.bbcook.cn

int *p = &a;  *p = 5;
来源：http://jqp.feifeiyinyue.top

[S11] C：逐行读文件
来源：http://gpy.9152youxi.cn

FILE *f = fopen("a.txt", "r");
来源：http://lub.meibo888.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://avg.hnxiangtu.top

fclose(f);
来源：http://gii.hysaishi.cn

[S12] C：写文件
来源：http://xrd.zhoulong.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://her.sufxvd.cn

[S13] C：宏定义
来源：http://oqt.nanxinkj.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nwa.guowangkeji.top

[S14] C：枚举
来源：http://doc.fehbvm.com

enum Color { RED, GREEN, BLUE };
来源：http://nzf.pycfn.com

[S15] C：类型转换
来源：http://err.ppjwa.cn

(double) a / b
来源：http://bsa.yfazqb.com

[S16] C：位操作置位
来源：http://ool.xinyue.icu

x |= (1 << 3);
来源：http://zco.jyoumei.cn

[S17] C：安全拼接字符串
来源：http://cek.guowangkeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vyc.snrcjt.cn

[S18] C：命令行参数
来源：http://rhg.xuanzx.com

int main(int argc, char **argv)
来源：http://sfs.zhaomingkeji.xyz

[S19] C：快速排序
来源：http://jlg.tarul.cn

qsort(a, n, sizeof(int), cmp);
来源：http://soq.gzhubu.top

[S20] C：二分查找
来源：http://tus.316326.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cxf.kuanghao11.cn

[S21] C：字符类别判断
来源：http://sui.xinyue.icu

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xhz.smart0.xyz

[S22] C：字符串转数字
来源：http://irv.gogol.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ycs.xylfe.cn

[S23] C：随机数
来源：http://vmc.jiagoushi.top

srand(time(NULL));  int r = rand() % 100;
来源：http://lsv.birdmap.top

[S24] C：获取本地时间
来源：http://qwr.quarkkingdee.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ylc.sufxvd.cn

[S25] C：内存拷贝
来源：http://ezi.hcnkem.com

memcpy(dst, src, n);
来源：http://ovh.xingfuxueyuan.xyz

[S26] C：内存清零
来源：http://sjd.shzxlz.cn

memset(a, 0, sizeof a);
来源：http://lcy.guowangkeji.top

[S27] C：定义常量
来源：http://pxe.vehdjk.com

const double PI = 3.14159;
来源：http://ufz.jqgfzy.top

[S28] C：静态变量
来源：http://gha.vehdjk.com

static int counter = 0;
来源：http://ilo.zhiwuduotai.top

[S29] C：变参函数
来源：http://wzr.smart0.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vpb.cqqwz.cn

[S30] C：头文件保护
来源：http://kde.uphjek.com

#ifndef X_H
来源：http://jfh.xylfe.cn

#define X_H
来源：http://opr.chenlongwang.top

#endif
来源：http://ied.hongshengwenyu.top

[S31] C++：Hello World
来源：http://bxx.bbcook.cn

#include <iostream>
来源：http://wlx.dianchejie.cn

int main() { std::cout << "Hello\n"; }
来源：http://oym.fzhhl.top

[S32] C++：字符串
来源：http://tjl.nwbrower.top

std::string s = "hi";  s += "!";
来源：http://bnf.cucudq.cn

[S33] C++：vector 增删
来源：http://ykn.jqgufenzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ahp.haohaochexian.top

[S34] C++：遍历 vector
来源：http://jrk.guannengcc.top

for (auto &x : v) { std::cout << x; }
来源：http://pps.ydzc1.top

[S35] C++：map
来源：http://ymz.quarkkingdee.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rwj.yj20258.top

[S36] C++：unordered_map
来源：http://wtx.chenzaomai.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cng.52xcode.cn

[S37] C++：set
来源：http://kpg.yanxiufei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zwj.zdbjq.cn

[S38] C++：排序
来源：http://mil.jinqigufen.top

std::sort(v.begin(), v.end());
来源：http://djd.yvedp.cn

[S39] C++：自定义比较器排序
来源：http://bgy.zhiwuduotai.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mrb.zhengqikj.top

[S40] C++：查找元素
来源：http://zld.jinyuanbaomall.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://elq.shzxlz.cn

[S41] C++：类与构造函数
来源：http://qat.guannengcc.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://acs.yueranfly.top

[S42] C++：继承与虚函数
来源：http://tyn.iojbl.cn

class B : public Base { public: void f() override {} };
来源：http://lfa.smart0.xyz

[S43] C++：智能指针
来源：http://yie.iojbl.cn

auto p = std::make_unique<int>(5);
来源：http://aer.tian-w.cn

[S44] C++：引用传参
来源：http://gzo.c1oappe.top

void inc(int &x) { ++x; }
来源：http://vwx.yueranfly.top

[S45] C++：lambda
来源：http://aqz.gogol.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fju.zhongyouzk.top

[S46] C++：函数模板
来源：http://les.zycfv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xzu.nwbrower.top

[S47] C++：结构化绑定遍历
来源：http://pop.iojbl.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sru.yfazqb.com

[S48] C++：逐行读文件
来源：http://dld.yvedp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ikj.hnxiangtu.top

while (std::getline(in, line)) { }
来源：http://udk.zhongyouzk.top

[S49] C++：写文件
来源：http://jih.jinqigufen.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cqm.c1oappe.top

[S50] C++：格式化数字
来源：http://ddf.zhaomingkeji.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fzw.hfpthk.cn

[S51] C++：显式类型转换
来源：http://gcr.aizwys.cn

static_cast<double>(a) / b
来源：http://kzj.aibaodan.cn

[S52] C++：const 与 noexcept
来源：http://wpj.gogol.net.cn

int size() const noexcept { return n_; }
来源：http://xaj.uphjek.com

[S53] C++：移动语义
来源：http://lut.daxiang520.top

std::vector<int> w = std::move(v);
来源：http://vkf.yuxming.cn

[S54] C++：异常处理
来源：http://uzc.gaohongyu789.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vtr.wangshuangyany.cn

[S55] C++：结构化绑定
来源：http://zxd.shanyushiyangkeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://gym.birdmap.top

[S56] C++：optional
来源：http://ldz.epnwcf.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pqp.ehwqpu.com

[S57] C++：编译期常量
来源：http://rkb.sufxvd.cn

constexpr int N = 10;
来源：http://yqe.chenlongwang.top

[S58] C++：命名空间
来源：http://jwb.fengsongda.top

namespace ns { int f() { return 1; } }
来源：http://eiv.jlsjyb.cn

[S59] C++：静态断言
来源：http://ytf.zhoulong.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kid.mhx1999.top

[S60] C++：遍历并删除元素
来源：http://kvv.hnxiangtu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kht.guowangkeji.top

================================================================================
来源：http://ols.sjlbkw.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eac.xingfuxueyuan.xyz

================================================================================
来源：http://tob.jinqigufen.top

[T01] Kotlin：Hello World
来源：http://jwm.yfazqb.com

println("Hello")
来源：http://ger.feifeiyinyue.top

[T02] Kotlin：变量
来源：http://efm.jianghu66.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qxp.yfazqb.com

[T03] Kotlin：字符串模板
来源：http://wun.dashuyun.cn

"值: $b"
来源：http://ywk.andypj.xyz

[T04] Kotlin：空安全
来源：http://udh.fanxiaobao.xyz

val n: String? = null;  n?.length
来源：http://kpp.snrcjt.cn

[T05] Kotlin：when 表达式
来源：http://jqx.chenjidiqi.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kha.tianlin.xyz

[T06] Kotlin：集合映射
来源：http://fqq.jqgufenzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://mee.shzxlz.cn

[T07] Kotlin：集合过滤
来源：http://xqt.gaohongyu789.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://cgb.redwolf501.top

[T08] Kotlin：数据类
来源：http://zup.fehbvm.com

data class User(val name: String, val age: Int)
来源：http://rqs.zhixingplan.top


<!-- 参考信息 -->