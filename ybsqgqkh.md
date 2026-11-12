代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://mhl.ydjk.org.cn

[R18] 遍历数组
来源：http://uiy.cdnleiting.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://azv.birdmap.top

[R19] 数组长度
来源：http://lmd.xuetiantiany.cn

echo "${#arr[@]}"
来源：http://lmr.andypj.xyz

[R20] 关联数组（字典）
来源：http://bfp.fanxiaobao.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zvs.yangfankeji.com

[R21] 字符串长度
来源：http://vhm.wangshuangyany.cn

echo "${#s}"
来源：http://jfi.hcnkem.com

[R22] 截取子串
来源：http://byd.xinyue.icu

echo "${s:0:5}"
来源：http://xgi.havefunace.top

[R23] 字符串替换
来源：http://owb.9152youxi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wre.shuidangran.top

[R24] 大小写转换
来源：http://pzq.jyoumei.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xaa.snrcjt.cn

[R25] 去后缀 / 去前缀
来源：http://huk.nanxinkj.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://mwh.zhoulong.xyz

[R26] 命令替换
来源：http://xhh.pengpengdd.cyou

now=$(date +%F); echo "$now"
来源：http://oxa.jqgfzy.top

[R27] 算术展开
来源：http://xpg.kuanghao11.cn

echo $((1 + 2 * 3))
来源：http://dmd.tarul.cn

[R28] 浮点运算
来源：http://xcf.shzxlz.cn

echo "scale=2; 10/3" | bc
来源：http://xgp.hesvh.cn

[R29] 定义函数
来源：http://mmc.9152youxi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yly.zhaomingkeji.xyz

[R30] 函数返回状态码
来源：http://wij.hcnkem.com

f() { return 0; }; f || echo "失败了"
来源：http://cvm.gzhubu.top

[R31] 局部变量
来源：http://bqv.tarul.cn

f() { local x=1; echo "$x"; }
来源：http://qsg.sjlbkw.cn

[R32] 参数个数校验
来源：http://bte.yuxming.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zwm.zhaomingkeji.xyz

[R33] 捕获错误并提示行号
来源：http://dfg.xziqi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ell.ivvv.top

[R34] 退出时清理
来源：http://jbn.gogol.net.cn

trap 'rm -f "$tmp"' EXIT
来源：http://oun.xuanzx.com

[R35] 后台执行并等待
来源：http://ycs.jiagoushi.top

sleep 5 & pid=$!; wait "$pid"
来源：http://bgy.gogol.net.cn

[R36] 并发执行多个任务
来源：http://dvn.havefunace.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rza.jiagoushi.top

[R37] 把输出赋给变量
来源：http://nek.shanyushiyangkeji.top

files=$(ls -1)
来源：http://ogd.fanxiaobao.xyz

[R38] 管道串联
来源：http://vep.sufxvd.cn

cat a.txt | grep -i error | wc -l
来源：http://ekj.gogol.net.cn

[R39] 重定向标准输出与错误
来源：http://rdd.hongshengwenyu.top

cmd > out.log 2>&1
来源：http://hev.hfpthk.cn

[R40] 追加写日志
来源：http://wso.svipenyu.cn

echo "log" >> out.log
来源：http://hmg.cucudq.cn

[R41] 丢弃输出
来源：http://hdz.yj202588.top

cmd >/dev/null 2>&1
来源：http://jfs.quarkkingdee.top

[R42] 输入重定向
来源：http://ngy.xuetiantiany.cn

wc -l < a.txt
来源：http://tdg.yanxiufei.cn

[R43] 按名字查找文件
来源：http://ihm.shanyushiyangtech.top

find . -name "*.log" -type f
来源：http://nsh.shanyushiyangkeji.top

[R44] 按修改时间查找
来源：http://zzi.xuanzx.com

find . -mtime -7 -type f
来源：http://wff.sysykeji.top

[R45] 批量删除
来源：http://lpk.hywenlv.cn

find . -name "*.tmp" -delete
来源：http://llh.uphjek.com

[R46] 递归替换文件内容
来源：http://cmx.shangyingyoupin.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://snu.mhx1999.top

[R47] sed 单行替换
来源：http://bpp.yj20258.top

sed -i 's/foo/bar/g' a.txt
来源：http://bgg.cucudq.cn

[R48] awk 取指定列
来源：http://osh.zhengqikj.top

awk '{print $1, $3}' a.txt
来源：http://yxs.cdnleiting.top

[R49] awk 带条件
来源：http://kud.yuxming.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xre.yonumen.top

[R50] awk 求和
来源：http://fnz.vqdsnc.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dyg.fengsongda.top

[R51] 排序去重取前几
来源：http://oih.yvedp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hjm.zhengqikj.top

[R52] 统计行数
来源：http://uxm.epnwcf.com

wc -l a.txt
来源：http://gsd.xinyue.icu

[R53] 查看文件头与实时尾
来源：http://bdw.fzhhl.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://plo.aizwys.cn

[R54] 比较两个文件
来源：http://ncv.chenjidiqi.icu

diff a.txt b.txt
来源：http://hyr.zhiwuduotai.top

[R55] 压缩与解压
来源：http://ocq.yj20258.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gvb.daria6918.cn

[R56] 远程拷贝
来源：http://abs.ctjpmb.com

scp file user@host:/path/
来源：http://bpo.hfpthk.cn

[R57] 远程执行命令
来源：http://hkd.epnwcf.com

ssh user@host 'uptime'
来源：http://xjs.jyoumei.cn

[R58] 下载文件
来源：http://amr.ydjk.org.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rpi.gaohongyu789.top

[R59] 发 POST JSON
来源：http://lfd.316326.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nou.sweek.top

[R60] 只看 HTTP 状态码
来源：http://kkc.vqdsnc.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yad.hywenlv.cn

[R61] 磁盘占用
来源：http://cte.dianchejie.cn

df -h;  du -sh *
来源：http://nrk.52xcode.cn

[R62] 找最占空间的文件
来源：http://clr.feifeiyinyue.top

du -ah . | sort -rh | head -10
来源：http://otc.kuanghao11.cn

[R63] 内存与进程
来源：http://qcn.sxryk.cn

free -h;  ps aux | grep nginx
来源：http://icx.jinqigufen.top

[R64] 结束进程
来源：http://vos.hcnkem.com

kill -9 $(pgrep -f app.py)
来源：http://vau.zhiwuduotai.top

[R65] 查看端口占用
来源：http://wwe.0kj1m.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sdu.zhoulong.xyz

[R66] 定时任务
来源：http://hfp.zhaomingkeji.xyz

crontab -e;  crontab -l
来源：http://ckd.jinqigufen.top

[R67] 生成随机十六进制串
来源：http://aef.tarul.cn

openssl rand -hex 16
来源：http://vvj.kuanghao11.cn

[R68] 计算文件校验值
来源：http://pgw.cheryme.top

sha256sum a.txt;  md5sum a.txt
来源：http://hih.zdbjq.cn

[R69] 生成随机密码
来源：http://flu.yfazqb.com

head -c 16 /dev/urandom | base64
来源：http://nyr.yonumen.top

[R70] 时间戳与互转
来源：http://mve.hammf.cn

date +%s;  date -d @1700000000
来源：http://arq.0kj1m.cn

[R71] 日期格式化
来源：http://fbv.zhaomingkeji.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://nor.nanxinkj.top

[R72] 等待端口就绪
来源：http://ubs.aibaodan.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nga.nwbrower.top

[R73] 分割大日志
来源：http://ghv.jianghu66.top

split -l 1000 big.log part_
来源：http://mlb.9152youxi.cn

[R74] 批量重命名
来源：http://awi.fzhhl.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gma.zhaomingkeji.xyz

[R75] 导出环境变量
来源：http://jaz.jinyuanbaomall.cn

export PATH="$HOME/bin:$PATH"
来源：http://lmd.guannengcc.top

[R76] 使用临时文件
来源：http://fog.zhixingplan.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pbx.yj202588.top

[R77] 读取用户输入
来源：http://psp.ehwqpu.com

read -rp "请输入: " ans
来源：http://tki.hysaishi.cn

[R78] 交互式菜单
来源：http://stk.pengpengdd.cyou

select opt in a b c; do echo "$opt"; break; done
来源：http://fta.dashuyun.cn

[R79] 解析命令行选项
来源：http://teg.havefunace.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kdy.nwbrower.top

[R80] 查看脚本执行耗时
来源：http://ebb.hywenlv.cn

time ./run.sh
来源：http://ajv.snrcjt.cn

================================================================================
来源：http://vqm.yvedp.cn

S. C / C++ 专题
来源：http://wmp.shangyingyoupin.top

================================================================================
来源：http://nsz.sjlbkw.cn

[S01] C：Hello World
来源：http://pdg.shuidangran.top

#include <stdio.h>
来源：http://rfs.shzxlz.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qnl.gaohongyu789.top

[S02] C：变量与格式化输出
来源：http://olv.snrcjt.cn

int a = 10; printf("%d\n", a);
来源：http://czs.hesvh.cn

[S03] C：读入整数
来源：http://ohs.fzhhl.top

int x; scanf("%d", &x);
来源：http://lbl.jinyuanbaomall.cn

[S04] C：字符串复制
来源：http://gzk.cqqwz.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mst.gaohongyu789.top

[S05] C：字符串长度
来源：http://izp.zhaomingkeji.xyz

strlen(s)
来源：http://ilq.hammf.cn

[S06] C：字符串比较
来源：http://fpp.cdnleiting.top

strcmp(a, b) == 0
来源：http://dyo.xinyue.icu

[S07] C：数组遍历求和
来源：http://vcw.andypj.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nee.hfpthk.cn

[S08] C：动态内存分配与释放
来源：http://vsk.ywan-chungtsiang.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://npu.jyoumei.cn

[S09] C：结构体定义与初始化
来源：http://vdy.yuanzhike.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ych.tianlin.xyz

[S10] C：指针与解引用
来源：http://tcz.yj202588.top

int *p = &a;  *p = 5;
来源：http://syz.aibaodan.cn

[S11] C：逐行读文件
来源：http://ukq.snrcjt.cn

FILE *f = fopen("a.txt", "r");
来源：http://nnt.redwolf501.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://mfu.chenzaomai.com

fclose(f);
来源：http://xdc.uphjek.com

[S12] C：写文件
来源：http://wyq.zycfv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lxd.hywenlv.cn

[S13] C：宏定义
来源：http://qkr.hysaishi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qwz.zdqjudy.top

[S14] C：枚举
来源：http://usy.ydzc1.top

enum Color { RED, GREEN, BLUE };
来源：http://zir.mhx1999.top

[S15] C：类型转换
来源：http://bgu.yj202588.top

(double) a / b
来源：http://chp.ctjpmb.com

[S16] C：位操作置位
来源：http://rup.chenjidiqi.icu

x |= (1 << 3);
来源：http://xxn.fanxiaobao.xyz

[S17] C：安全拼接字符串
来源：http://cgq.ivvv.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://aay.tanke756.top

[S18] C：命令行参数
来源：http://qkw.yongpay.top

int main(int argc, char **argv)
来源：http://qsm.zhijiandao.cn

[S19] C：快速排序
来源：http://ize.ppjwa.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gwv.nanxinkj.top

[S20] C：二分查找
来源：http://jca.shanyushiyangtech.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lcb.nanxinkj.top

[S21] C：字符类别判断
来源：http://csi.mhx1999.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ohv.gogol.net.cn

[S22] C：字符串转数字
来源：http://fhz.jinqigufen.top

atoi("42");  strtod("3.14", NULL);
来源：http://pmd.hysaishi.cn

[S23] C：随机数
来源：http://xfy.meibo888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ujf.uphjek.com

[S24] C：获取本地时间
来源：http://ebk.sxryk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vkz.vehdjk.com

[S25] C：内存拷贝
来源：http://rav.fanxiaobao.xyz

memcpy(dst, src, n);
来源：http://omg.zhaomingkeji.xyz

[S26] C：内存清零
来源：http://oxg.sjlbkw.cn

memset(a, 0, sizeof a);
来源：http://pci.0kj1m.cn

[S27] C：定义常量
来源：http://aiz.jianghu66.top

const double PI = 3.14159;
来源：http://kim.epnwcf.com

[S28] C：静态变量
来源：http://zwv.yj20258888.top

static int counter = 0;
来源：http://aav.yj20258.top

[S29] C：变参函数
来源：http://oih.fanxiaobao.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://imx.dianchejie.cn

[S30] C：头文件保护
来源：http://tno.zhengqikj.top

#ifndef X_H
来源：http://caw.sysykeji.top

#define X_H
来源：http://tkf.fzhhl.top

#endif
来源：http://cwb.xuanzx.com

[S31] C++：Hello World
来源：http://aqi.ppjwa.cn

#include <iostream>
来源：http://hnb.yvedp.cn

int main() { std::cout << "Hello\n"; }
来源：http://dpj.yuxming.cn

[S32] C++：字符串
来源：http://dqz.jinyuanbaomall.cn

std::string s = "hi";  s += "!";
来源：http://ukk.dashuyun.cn

[S33] C++：vector 增删
来源：http://bcz.fktsv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yjj.hcnkem.com

[S34] C++：遍历 vector
来源：http://plm.bjfxy.top

for (auto &x : v) { std::cout << x; }
来源：http://oem.fengsongda.top

[S35] C++：map
来源：http://xjs.nwbrower.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dyc.snrcjt.cn

[S36] C++：unordered_map
来源：http://jqc.cqqwz.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wpc.yonumen.top

[S37] C++：set
来源：http://yin.shuidangran.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bns.yj202588.top

[S38] C++：排序
来源：http://ezk.gzhubu.top

std::sort(v.begin(), v.end());
来源：http://kgk.gzhubu.top

[S39] C++：自定义比较器排序
来源：http://mxd.hnxiangtu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://toh.c1oappe.top

[S40] C++：查找元素
来源：http://pim.shuidangran.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bqd.nanxuanxn.top

[S41] C++：类与构造函数
来源：http://vcj.zhiwuduotai.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zpz.nanxuanxn.top

[S42] C++：继承与虚函数
来源：http://dpt.hysaishi.cn

class B : public Base { public: void f() override {} };
来源：http://mxe.hcnkem.com

[S43] C++：智能指针
来源：http://ezu.zdbjq.cn

auto p = std::make_unique<int>(5);
来源：http://arp.sysykeji.top

[S44] C++：引用传参
来源：http://pcm.shuidangran.top

void inc(int &x) { ++x; }
来源：http://anf.gzhubu.top

[S45] C++：lambda
来源：http://jml.quarkkingdee.top

auto add = [](int a, int b) { return a + b; };
来源：http://yxk.jlsjyb.cn

[S46] C++：函数模板
来源：http://emj.yangfankeji.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gli.yonumen.top

[S47] C++：结构化绑定遍历
来源：http://gtz.ydjk.org.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oty.hesvh.cn

[S48] C++：逐行读文件
来源：http://xcn.yueranfly.top

std::ifstream in("a.txt");  std::string line;
来源：http://hig.cqqwz.cn

while (std::getline(in, line)) { }
来源：http://uiw.pengpengdd.cyou

[S49] C++：写文件
来源：http://jah.quarkkingdee.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vag.shanyushiyangtech.top

[S50] C++：格式化数字
来源：http://vyv.gogol.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ceg.zdqjudy.top

[S51] C++：显式类型转换
来源：http://ooz.cdnleiting.top

static_cast<double>(a) / b
来源：http://kyz.daria6918.cn

[S52] C++：const 与 noexcept
来源：http://bmk.xuanzx.com

int size() const noexcept { return n_; }
来源：http://biv.mhx1999.top

[S53] C++：移动语义
来源：http://ikd.gaohongyu789.top

std::vector<int> w = std::move(v);
来源：http://gwp.chenzaomai.com

[S54] C++：异常处理
来源：http://pyw.ivvv.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ukx.gogol.net.cn

[S55] C++：结构化绑定
来源：http://ubp.smart0.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://fke.nanxinkj.top

[S56] C++：optional
来源：http://vcr.shuidangran.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vxg.vehdjk.com

[S57] C++：编译期常量
来源：http://vpi.shanyushiyangtech.top

constexpr int N = 10;
来源：http://wxl.yonumen.top

[S58] C++：命名空间
来源：http://eed.shzxlz.cn

namespace ns { int f() { return 1; } }
来源：http://zto.smart0.xyz

[S59] C++：静态断言
来源：http://ssp.nwbrower.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fzg.52xcode.cn

[S60] C++：遍历并删除元素
来源：http://wdc.316326.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vip.hnxiangtu.top

================================================================================
来源：http://raq.gzhubu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wdv.yuanzhike.top

================================================================================
来源：http://dqm.guannengcc.top

[T01] Kotlin：Hello World
来源：http://bdm.nwbrower.top

println("Hello")
来源：http://wtu.epnwcf.com

[T02] Kotlin：变量
来源：http://jse.epnwcf.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://crk.kuanghao11.cn

[T03] Kotlin：字符串模板
来源：http://okk.yangfankeji.com

"值: $b"
来源：http://lgr.vqdsnc.cn

[T04] Kotlin：空安全
来源：http://rdc.gogol.net.cn

val n: String? = null;  n?.length
来源：http://pum.zhiwuduotai.top

[T05] Kotlin：when 表达式
来源：http://yes.gotoacloud.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pny.fengsongda.top

[T06] Kotlin：集合映射
来源：http://apx.jinyuanbaomall.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pvs.ydjk.org.cn

[T07] Kotlin：集合过滤
来源：http://hjy.cheryme.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://gpm.jinqigfzy.top

[T08] Kotlin：数据类
来源：http://mmg.wangshuangyany.cn

data class User(val name: String, val age: Int)
来源：http://dba.ppjwa.cn

[T09] Kotlin：扩展函数
来源：http://rcz.xziqi.cn

fun String.exclaim() = this + "!"
来源：http://lra.gogol.net.cn

[T10] Kotlin：默认参数
来源：http://aey.nanxuanxn.top

fun greet(name: String = "World") = "Hi $name"
来源：http://udh.xziqi.cn

[T11] Kotlin：协程
来源：http://rfb.yuxming.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dyv.9152youxi.cn

[T12] Kotlin：解构声明
来源：http://qya.dashuyun.cn

val (a, b) = Pair(1, 2)
来源：http://kzm.cqqwz.cn

[T13] Kotlin：只读 Map
来源：http://lfk.xziqi.cn

val m = mapOf("a" to 1)
来源：http://ldx.redwolf501.top

[T14] Kotlin：循环
来源：http://rbp.nanxuanxn.top

for (i in 1..10) println(i)
来源：http://xoo.nanxinkj.top

[T15] Kotlin：接口
来源：http://lsc.nanxuanxn.top

interface Shape { fun area(): Double }
来源：http://ume.gaohongyu789.top

[T16] Swift：Hello World
来源：http://oxj.xziqi.cn

print("Hello")
来源：http://blr.gaohongyu789.top

[T17] Swift：变量与常量
来源：http://ofc.fanxiaobao.xyz

var a = 1;  let b = 2
来源：http://nfm.iojbl.cn

[T18] Swift：字符串插值
来源：http://drk.c1oappe.top

"值: \(b)"
来源：http://nnp.dashuyun.cn

[T19] Swift：可选绑定
来源：http://zhc.52xcode.cn

if let n = opt { print(n) }
来源：http://azw.cqqwz.cn

[T20] Swift：数组操作
来源：http://jra.xylfe.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ggw.zycfv.cn


<!-- 参考信息 -->