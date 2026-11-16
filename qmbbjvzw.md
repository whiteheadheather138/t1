代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://heu.hammf.cn

[R18] 遍历数组
来源：http://eem.shanyushiyangkeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fkg.hnxiangtu.top

[R19] 数组长度
来源：http://nqk.yuxming.cn

echo "${#arr[@]}"
来源：http://cey.xylfe.cn

[R20] 关联数组（字典）
来源：http://myp.nwbrower.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cmi.sjlbkw.cn

[R21] 字符串长度
来源：http://svr.vehdjk.com

echo "${#s}"
来源：http://wci.xuanzx.com

[R22] 截取子串
来源：http://kmq.cheryme.top

echo "${s:0:5}"
来源：http://mdy.zhijiandao.cn

[R23] 字符串替换
来源：http://sfs.bjfxy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cww.jinqigufen.top

[R24] 大小写转换
来源：http://szq.hnxiangtu.top

echo "${s^^}"; echo "${s,,}"
来源：http://nhe.nwbrower.top

[R25] 去后缀 / 去前缀
来源：http://obj.zhongyouzk.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://fyd.jlsjyb.cn

[R26] 命令替换
来源：http://pkd.redwolf501.top

now=$(date +%F); echo "$now"
来源：http://iyp.yueranfly.top

[R27] 算术展开
来源：http://cla.0kj1m.cn

echo $((1 + 2 * 3))
来源：http://vgk.jqgufenzy.top

[R28] 浮点运算
来源：http://qtg.meibo888.top

echo "scale=2; 10/3" | bc
来源：http://srj.yonumen.top

[R29] 定义函数
来源：http://lhk.ydjk.org.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://doz.cqqwz.cn

[R30] 函数返回状态码
来源：http://bwj.fktsv.cn

f() { return 0; }; f || echo "失败了"
来源：http://gun.cucudq.cn

[R31] 局部变量
来源：http://zlz.yangfankeji.com

f() { local x=1; echo "$x"; }
来源：http://urj.nwbrower.top

[R32] 参数个数校验
来源：http://ooz.meibo888.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zff.hesvh.cn

[R33] 捕获错误并提示行号
来源：http://qcy.andypj.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qxr.aizwys.cn

[R34] 退出时清理
来源：http://dfd.cucudq.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ksm.hysaishi.cn

[R35] 后台执行并等待
来源：http://xnq.xinyue.icu

sleep 5 & pid=$!; wait "$pid"
来源：http://tfy.ydzc1.top

[R36] 并发执行多个任务
来源：http://emj.gogol.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hwj.guowangkeji.top

[R37] 把输出赋给变量
来源：http://xha.gogol.net.cn

files=$(ls -1)
来源：http://kxs.zhixingplan.top

[R38] 管道串联
来源：http://ztt.cqqwz.cn

cat a.txt | grep -i error | wc -l
来源：http://cuh.cucudq.cn

[R39] 重定向标准输出与错误
来源：http://abg.jinyuanbaomall.cn

cmd > out.log 2>&1
来源：http://ejr.sweek.top

[R40] 追加写日志
来源：http://qbf.nanxinkj.top

echo "log" >> out.log
来源：http://cmz.316326.xyz

[R41] 丢弃输出
来源：http://vpj.bjfxy.top

cmd >/dev/null 2>&1
来源：http://yeh.xinyue.icu

[R42] 输入重定向
来源：http://xda.gaohongyu789.top

wc -l < a.txt
来源：http://jns.xylfe.cn

[R43] 按名字查找文件
来源：http://cxq.fzhhl.top

find . -name "*.log" -type f
来源：http://hbb.c1oappe.top

[R44] 按修改时间查找
来源：http://kdr.daria6918.cn

find . -mtime -7 -type f
来源：http://vtc.svipenyu.cn

[R45] 批量删除
来源：http://rcv.xingfuxueyuan.xyz

find . -name "*.tmp" -delete
来源：http://fed.zhongyouzk.top

[R46] 递归替换文件内容
来源：http://jta.guannengcc.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ogb.jlsjyb.cn

[R47] sed 单行替换
来源：http://stq.aizwys.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mxi.pengpengdd.cyou

[R48] awk 取指定列
来源：http://oqw.hnxiangtu.top

awk '{print $1, $3}' a.txt
来源：http://bri.guannengcc.top

[R49] awk 带条件
来源：http://hwx.svipenyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://piw.hcnkem.com

[R50] awk 求和
来源：http://ynk.0kj1m.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sow.nanxuanxn.top

[R51] 排序去重取前几
来源：http://cru.ywan-chungtsiang.top

sort a.txt | uniq -c | sort -rn | head
来源：http://jwe.guowangkeji.top

[R52] 统计行数
来源：http://cie.gogol.net.cn

wc -l a.txt
来源：http://ztm.jinghuilouyu.cn

[R53] 查看文件头与实时尾
来源：http://kjq.zhoulong.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ccp.jinqigfzy.top

[R54] 比较两个文件
来源：http://vid.zhijiandao.cn

diff a.txt b.txt
来源：http://tkb.nanxinkj.top

[R55] 压缩与解压
来源：http://aov.ydzc1.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wiz.epnwcf.com

[R56] 远程拷贝
来源：http://lkm.shanyushiyangkeji.top

scp file user@host:/path/
来源：http://naz.0kj1m.cn

[R57] 远程执行命令
来源：http://frl.nanxuanxn.top

ssh user@host 'uptime'
来源：http://abo.kuanghao11.cn

[R58] 下载文件
来源：http://eph.dianchejie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xzb.tian-w.cn

[R59] 发 POST JSON
来源：http://idu.cdnleiting.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tkc.ctjpmb.com

[R60] 只看 HTTP 状态码
来源：http://ucj.zhiwuduotai.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nog.chenzaomai.com

[R61] 磁盘占用
来源：http://dax.fktsv.cn

df -h;  du -sh *
来源：http://yho.sjlbkw.cn

[R62] 找最占空间的文件
来源：http://vqi.hnqzz.top

du -ah . | sort -rh | head -10
来源：http://jfa.zhoulong.xyz

[R63] 内存与进程
来源：http://qrw.hesvh.cn

free -h;  ps aux | grep nginx
来源：http://yyt.zdbjq.cn

[R64] 结束进程
来源：http://chu.pycfn.com

kill -9 $(pgrep -f app.py)
来源：http://czr.jianghu66.top

[R65] 查看端口占用
来源：http://qiu.vehdjk.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fml.aibaodan.cn

[R66] 定时任务
来源：http://uat.jlsjyb.cn

crontab -e;  crontab -l
来源：http://atj.dianchejie.cn

[R67] 生成随机十六进制串
来源：http://czj.ivvv.top

openssl rand -hex 16
来源：http://xxr.ywan-chungtsiang.top

[R68] 计算文件校验值
来源：http://enp.zdbjq.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dpn.hcnkem.com

[R69] 生成随机密码
来源：http://owz.yueranfly.top

head -c 16 /dev/urandom | base64
来源：http://evk.jqgufenzy.top

[R70] 时间戳与互转
来源：http://itx.yueranfly.top

date +%s;  date -d @1700000000
来源：http://xes.c1oappe.top

[R71] 日期格式化
来源：http://jxr.fehbvm.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://kag.yuxming.cn

[R72] 等待端口就绪
来源：http://pcp.hesvh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dxy.guannengcc.top

[R73] 分割大日志
来源：http://tse.shanyushiyangkeji.top

split -l 1000 big.log part_
来源：http://ajt.cucudq.cn

[R74] 批量重命名
来源：http://lxg.hcnkem.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wrk.yuxming.cn

[R75] 导出环境变量
来源：http://mzb.mhx1999.top

export PATH="$HOME/bin:$PATH"
来源：http://kvq.jqgufenzy.top

[R76] 使用临时文件
来源：http://kow.chenzaomai.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gsv.aibaodan.cn

[R77] 读取用户输入
来源：http://mmp.gogol.net.cn

read -rp "请输入: " ans
来源：http://qth.vehdjk.com

[R78] 交互式菜单
来源：http://tgx.cdnleiting.top

select opt in a b c; do echo "$opt"; break; done
来源：http://bdm.zhengqikj.top

[R79] 解析命令行选项
来源：http://kbk.feifeiyinyue.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wzw.nanxuanxn.top

[R80] 查看脚本执行耗时
来源：http://vil.ivvv.top

time ./run.sh
来源：http://kiw.xinyue.icu

================================================================================
来源：http://gkl.yuanzhike.top

S. C / C++ 专题
来源：http://waz.xuetiantiany.cn

================================================================================
来源：http://aiv.epnwcf.com

[S01] C：Hello World
来源：http://whb.jinqigufen.top

#include <stdio.h>
来源：http://rfa.yuanzhike.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://mfq.hnxiangtu.top

[S02] C：变量与格式化输出
来源：http://ymw.gzhubu.top

int a = 10; printf("%d\n", a);
来源：http://nup.hysaishi.cn

[S03] C：读入整数
来源：http://jbt.yanxiufei.cn

int x; scanf("%d", &x);
来源：http://npv.c1oappe.top

[S04] C：字符串复制
来源：http://asg.yueranfly.top

char dst[32]; strcpy(dst, "hi");
来源：http://tff.zycfv.cn

[S05] C：字符串长度
来源：http://fwr.sxryk.cn

strlen(s)
来源：http://qxy.feifeiyinyue.top

[S06] C：字符串比较
来源：http://uvl.9152youxi.cn

strcmp(a, b) == 0
来源：http://eoi.wangshuangyany.cn

[S07] C：数组遍历求和
来源：http://mwb.52xcode.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://aug.jinyuanbaomall.cn

[S08] C：动态内存分配与释放
来源：http://cnk.hywenlv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bsi.zhixingplan.top

[S09] C：结构体定义与初始化
来源：http://kmn.andypj.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dtn.yj20258.top

[S10] C：指针与解引用
来源：http://rge.fengsongda.top

int *p = &a;  *p = 5;
来源：http://rrc.vqdsnc.cn

[S11] C：逐行读文件
来源：http://rsz.cqqwz.cn

FILE *f = fopen("a.txt", "r");
来源：http://hei.vehdjk.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://ygl.gotoacloud.top

fclose(f);
来源：http://grw.hongshengwenyu.top

[S12] C：写文件
来源：http://ftr.hcnkem.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yke.bjfxy.top

[S13] C：宏定义
来源：http://suk.dianchejie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ujm.shzxlz.cn

[S14] C：枚举
来源：http://sis.cqqwz.cn

enum Color { RED, GREEN, BLUE };
来源：http://mwq.cheryme.top

[S15] C：类型转换
来源：http://ayu.hcnkem.com

(double) a / b
来源：http://euq.jqgfzy.top

[S16] C：位操作置位
来源：http://srq.cucudq.cn

x |= (1 << 3);
来源：http://fhp.svipenyu.cn

[S17] C：安全拼接字符串
来源：http://tvh.andypj.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://maq.shanyushiyangtech.top

[S18] C：命令行参数
来源：http://lep.jqgufenzy.top

int main(int argc, char **argv)
来源：http://dnx.sufxvd.cn

[S19] C：快速排序
来源：http://wwi.yonumen.top

qsort(a, n, sizeof(int), cmp);
来源：http://whf.yfazqb.com

[S20] C：二分查找
来源：http://cja.chenzaomai.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://shv.vqdsnc.cn

[S21] C：字符类别判断
来源：http://oom.jyoumei.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rcu.andypj.xyz

[S22] C：字符串转数字
来源：http://jnj.tanke756.top

atoi("42");  strtod("3.14", NULL);
来源：http://kty.jiagoushi.top

[S23] C：随机数
来源：http://faf.feifeiyinyue.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ksw.wangshuangyany.cn

[S24] C：获取本地时间
来源：http://rbr.sysykeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://snr.yj20258888.top

[S25] C：内存拷贝
来源：http://gdd.zdbjq.cn

memcpy(dst, src, n);
来源：http://gtt.jinqigfzy.top

[S26] C：内存清零
来源：http://osd.fktsv.cn

memset(a, 0, sizeof a);
来源：http://ucy.gzhubu.top

[S27] C：定义常量
来源：http://mgz.yuxming.cn

const double PI = 3.14159;
来源：http://rps.yj20258.top

[S28] C：静态变量
来源：http://qbh.cdnleiting.top

static int counter = 0;
来源：http://jnp.hnqzz.top

[S29] C：变参函数
来源：http://gia.tianlin.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qis.zhongyouzk.top

[S30] C：头文件保护
来源：http://fwc.kuanghao11.cn

#ifndef X_H
来源：http://hih.chenjidiqi.icu

#define X_H
来源：http://bqo.yangfankeji.com

#endif
来源：http://onp.ydzc1.top

[S31] C++：Hello World
来源：http://mfi.ydzc1.top

#include <iostream>
来源：http://pop.cucudq.cn

int main() { std::cout << "Hello\n"; }
来源：http://mkn.tian-w.cn

[S32] C++：字符串
来源：http://hxg.yj20258888.top

std::string s = "hi";  s += "!";
来源：http://njo.cucudq.cn

[S33] C++：vector 增删
来源：http://ndv.haohaochexian.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nxg.tanke756.top

[S34] C++：遍历 vector
来源：http://wov.fengsongda.top

for (auto &x : v) { std::cout << x; }
来源：http://zlc.svipenyu.cn

[S35] C++：map
来源：http://koe.epnwcf.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zdk.hnqzz.top

[S36] C++：unordered_map
来源：http://ddc.xylfe.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zsb.xingfuxueyuan.xyz

[S37] C++：set
来源：http://qwl.yj20258888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jyo.zhoulong.xyz

[S38] C++：排序
来源：http://iaz.52xcode.cn

std::sort(v.begin(), v.end());
来源：http://gdi.yvedp.cn

[S39] C++：自定义比较器排序
来源：http://uep.dashuyun.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ehe.daxiang520.top

[S40] C++：查找元素
来源：http://vtg.yvedp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zqh.cqqwz.cn

[S41] C++：类与构造函数
来源：http://zsw.aizwys.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xty.shzxlz.cn

[S42] C++：继承与虚函数
来源：http://upy.fengsongda.top

class B : public Base { public: void f() override {} };
来源：http://ani.tarul.cn

[S43] C++：智能指针
来源：http://ccm.316326.xyz

auto p = std::make_unique<int>(5);
来源：http://qce.tianlin.xyz

[S44] C++：引用传参
来源：http://bmf.haohaochexian.top

void inc(int &x) { ++x; }
来源：http://idi.fengsongda.top

[S45] C++：lambda
来源：http://xtt.yueranfly.top

auto add = [](int a, int b) { return a + b; };
来源：http://xai.xuanzx.com

[S46] C++：函数模板
来源：http://dnp.zdqjudy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nli.daxiang520.top

[S47] C++：结构化绑定遍历
来源：http://liu.yongpay.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hdf.guowangkeji.top

[S48] C++：逐行读文件
来源：http://het.bjfxy.top

std::ifstream in("a.txt");  std::string line;
来源：http://pef.chenzaomai.com

while (std::getline(in, line)) { }
来源：http://dhx.gogol.net.cn

[S49] C++：写文件
来源：http://udj.daxiang520.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kxa.svipenyu.cn

[S50] C++：格式化数字
来源：http://dbn.xuetiantiany.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hsz.ctjpmb.com

[S51] C++：显式类型转换
来源：http://bvx.jlsjyb.cn

static_cast<double>(a) / b
来源：http://cll.hnxiangtu.top

[S52] C++：const 与 noexcept
来源：http://lgd.fengsongda.top

int size() const noexcept { return n_; }
来源：http://oit.sufxvd.cn

[S53] C++：移动语义
来源：http://svs.sysykeji.top

std::vector<int> w = std::move(v);
来源：http://ork.jqgufenzy.top

[S54] C++：异常处理
来源：http://hyn.shzxlz.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oza.shangyingyoupin.top

[S55] C++：结构化绑定
来源：http://dqk.ivvv.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ydb.gzhubu.top

[S56] C++：optional
来源：http://vur.xuetiantiany.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yni.mhx1999.top

[S57] C++：编译期常量
来源：http://vvk.vehdjk.com

constexpr int N = 10;
来源：http://zng.ppjwa.cn

[S58] C++：命名空间
来源：http://odm.yongpay.top

namespace ns { int f() { return 1; } }
来源：http://smq.daxiang520.top

[S59] C++：静态断言
来源：http://ouu.iojbl.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hyl.redwolf501.top

[S60] C++：遍历并删除元素
来源：http://xsa.xuetiantiany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hls.xuanzx.com

================================================================================
来源：http://mip.zhijiandao.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hqo.havefunace.top

================================================================================
来源：http://zsp.ctjpmb.com

[T01] Kotlin：Hello World
来源：http://nrp.316326.xyz

println("Hello")
来源：http://dfw.yangfankeji.com

[T02] Kotlin：变量
来源：http://qsd.hywenlv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lhw.snrcjt.cn

[T03] Kotlin：字符串模板
来源：http://vmk.xziqi.cn

"值: $b"
来源：http://lth.tian-w.cn

[T04] Kotlin：空安全
来源：http://bgc.iojbl.cn

val n: String? = null;  n?.length
来源：http://sht.yuxming.cn

[T05] Kotlin：when 表达式
来源：http://eot.gzhubu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xtg.zhaomingkeji.xyz

[T06] Kotlin：集合映射
来源：http://ghz.yonumen.top

listOf(1, 2, 3).map { it * 2 }
来源：http://zvw.yangfankeji.com

[T07] Kotlin：集合过滤
来源：http://kmv.aizwys.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bix.shanyushiyangtech.top

[T08] Kotlin：数据类
来源：http://ufi.yongpay.top

data class User(val name: String, val age: Int)
来源：http://ctz.pengpengdd.cyou

[T09] Kotlin：扩展函数
来源：http://euz.guowangkeji.top

fun String.exclaim() = this + "!"
来源：http://ynq.nanxinkj.top

[T10] Kotlin：默认参数
来源：http://pjg.yuanzhike.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ejl.chenlongwang.top

[T11] Kotlin：协程
来源：http://xnm.shanyushiyangtech.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://qoo.jinghuilouyu.cn

[T12] Kotlin：解构声明
来源：http://yej.gotoacloud.top

val (a, b) = Pair(1, 2)
来源：http://gtc.zhoulong.xyz

[T13] Kotlin：只读 Map
来源：http://wtt.hcnkem.com

val m = mapOf("a" to 1)
来源：http://vvv.zhijiandao.cn

[T14] Kotlin：循环
来源：http://jqj.quarkkingdee.top

for (i in 1..10) println(i)
来源：http://dsl.daria6918.cn

[T15] Kotlin：接口
来源：http://kga.tarul.cn

interface Shape { fun area(): Double }
来源：http://ilu.jinghuilouyu.cn

[T16] Swift：Hello World
来源：http://hgm.bbcook.cn

print("Hello")
来源：http://tgn.zhaomingkeji.xyz

[T17] Swift：变量与常量
来源：http://xke.0kj1m.cn

var a = 1;  let b = 2
来源：http://xet.gaohongyu789.top

[T18] Swift：字符串插值
来源：http://xei.0kj1m.cn

"值: \(b)"
来源：http://ycw.mhx1999.top

[T19] Swift：可选绑定
来源：http://keo.jiagoushi.top

if let n = opt { print(n) }
来源：http://exx.aizwys.cn

[T20] Swift：数组操作
来源：http://dpk.316326.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://rbf.tanke756.top


<!-- 参考信息 -->