代发 wailian999

echo "${#s}"
来源：http://rrx.xuetiantiany.cn

[R22] 截取子串
来源：http://dco.tanke756.top

echo "${s:0:5}"
来源：http://bkb.yfazqb.com

[R23] 字符串替换
来源：http://tnp.jianghu66.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xjm.0kj1m.cn

[R24] 大小写转换
来源：http://zuq.hnxiangtu.top

echo "${s^^}"; echo "${s,,}"
来源：http://bro.xuetiantiany.cn

[R25] 去后缀 / 去前缀
来源：http://oao.ivvv.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://gva.zhongyouzk.top

[R26] 命令替换
来源：http://zgq.daria6918.cn

now=$(date +%F); echo "$now"
来源：http://kpk.guannengcc.top

[R27] 算术展开
来源：http://icp.9152youxi.cn

echo $((1 + 2 * 3))
来源：http://gqu.yanxiufei.cn

[R28] 浮点运算
来源：http://vsb.cqqwz.cn

echo "scale=2; 10/3" | bc
来源：http://vyg.yj202588.top

[R29] 定义函数
来源：http://jwh.wangshuangyany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ynm.zycfv.cn

[R30] 函数返回状态码
来源：http://ncf.yongpay.top

f() { return 0; }; f || echo "失败了"
来源：http://ohj.zdqjudy.top

[R31] 局部变量
来源：http://dkt.hongshengwenyu.top

f() { local x=1; echo "$x"; }
来源：http://phb.hnqzz.top

[R32] 参数个数校验
来源：http://uqd.kuanghao11.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xum.dianchejie.cn

[R33] 捕获错误并提示行号
来源：http://ghv.shanyushiyangtech.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vfe.hammf.cn

[R34] 退出时清理
来源：http://oux.jinyuanbaomall.cn

trap 'rm -f "$tmp"' EXIT
来源：http://opq.52xcode.cn

[R35] 后台执行并等待
来源：http://iki.hammf.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ffl.xuanzx.com

[R36] 并发执行多个任务
来源：http://smc.sjlbkw.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://reh.andypj.xyz

[R37] 把输出赋给变量
来源：http://bvr.hcnkem.com

files=$(ls -1)
来源：http://rjf.ctjpmb.com

[R38] 管道串联
来源：http://pdm.zdqjudy.top

cat a.txt | grep -i error | wc -l
来源：http://ocd.zhiwuduotai.top

[R39] 重定向标准输出与错误
来源：http://ago.jqgufenzy.top

cmd > out.log 2>&1
来源：http://rsu.nanxuanxn.top

[R40] 追加写日志
来源：http://mza.snrcjt.cn

echo "log" >> out.log
来源：http://ntb.cdnleiting.top

[R41] 丢弃输出
来源：http://fhp.hfpthk.cn

cmd >/dev/null 2>&1
来源：http://krg.epnwcf.com

[R42] 输入重定向
来源：http://olg.epnwcf.com

wc -l < a.txt
来源：http://nfs.yvedp.cn

[R43] 按名字查找文件
来源：http://yzh.cheryme.top

find . -name "*.log" -type f
来源：http://vjg.havefunace.top

[R44] 按修改时间查找
来源：http://xuv.hnqzz.top

find . -mtime -7 -type f
来源：http://wra.ywan-chungtsiang.top

[R45] 批量删除
来源：http://ddy.andypj.xyz

find . -name "*.tmp" -delete
来源：http://oxg.ivvv.top

[R46] 递归替换文件内容
来源：http://gfs.hesvh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kok.yj20258888.top

[R47] sed 单行替换
来源：http://pry.cucudq.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dhf.cheryme.top

[R48] awk 取指定列
来源：http://gle.fzhhl.top

awk '{print $1, $3}' a.txt
来源：http://tgo.tanke756.top

[R49] awk 带条件
来源：http://bxj.bbcook.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yax.havefunace.top

[R50] awk 求和
来源：http://wok.nanxuanxn.top

awk '{s += $2} END {print s}' a.txt
来源：http://syc.ydjk.org.cn

[R51] 排序去重取前几
来源：http://nat.cucudq.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fub.yanxiufei.cn

[R52] 统计行数
来源：http://ltr.xingfuxueyuan.xyz

wc -l a.txt
来源：http://zla.chenjidiqi.icu

[R53] 查看文件头与实时尾
来源：http://hax.iojbl.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vcv.jinyuanbaomall.cn

[R54] 比较两个文件
来源：http://jnd.shanyushiyangtech.top

diff a.txt b.txt
来源：http://nuv.kuanghao11.cn

[R55] 压缩与解压
来源：http://epw.ydjk.org.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gww.xingfuxueyuan.xyz

[R56] 远程拷贝
来源：http://vlk.yanxiufei.cn

scp file user@host:/path/
来源：http://njf.ehwqpu.com

[R57] 远程执行命令
来源：http://fpm.c1oappe.top

ssh user@host 'uptime'
来源：http://cyi.shangyingyoupin.top

[R58] 下载文件
来源：http://ymf.tian-w.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dux.jlsjyb.cn

[R59] 发 POST JSON
来源：http://woe.vqdsnc.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yva.zhengqikj.top

[R60] 只看 HTTP 状态码
来源：http://eoq.hongshengwenyu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hgv.guannengcc.top

[R61] 磁盘占用
来源：http://ccm.gaohongyu789.top

df -h;  du -sh *
来源：http://gjp.chenzaomai.com

[R62] 找最占空间的文件
来源：http://xyq.birdmap.top

du -ah . | sort -rh | head -10
来源：http://cvg.shzxlz.cn

[R63] 内存与进程
来源：http://ade.tanke756.top

free -h;  ps aux | grep nginx
来源：http://sjd.hnxiangtu.top

[R64] 结束进程
来源：http://wpj.nanxuanxn.top

kill -9 $(pgrep -f app.py)
来源：http://rkf.bjfxy.top

[R65] 查看端口占用
来源：http://zch.chenjidiqi.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gxf.yongpay.top

[R66] 定时任务
来源：http://ebr.guowangkeji.top

crontab -e;  crontab -l
来源：http://iam.jianghu66.top

[R67] 生成随机十六进制串
来源：http://mbm.iojbl.cn

openssl rand -hex 16
来源：http://sma.fzhhl.top

[R68] 计算文件校验值
来源：http://gvi.guowangkeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://ogz.hesvh.cn

[R69] 生成随机密码
来源：http://kfi.shangyingyoupin.top

head -c 16 /dev/urandom | base64
来源：http://knv.316326.xyz

[R70] 时间戳与互转
来源：http://wjy.shangyingyoupin.top

date +%s;  date -d @1700000000
来源：http://jkk.jqgufenzy.top

[R71] 日期格式化
来源：http://bsu.jqgfzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vcy.gaohongyu789.top

[R72] 等待端口就绪
来源：http://tgv.jyoumei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qbx.yonumen.top

[R73] 分割大日志
来源：http://ioy.jlsjyb.cn

split -l 1000 big.log part_
来源：http://kpn.quarkkingdee.top

[R74] 批量重命名
来源：http://rlj.nwbrower.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fcy.sxryk.cn

[R75] 导出环境变量
来源：http://qxn.jqgfzy.top

export PATH="$HOME/bin:$PATH"
来源：http://ana.tarul.cn

[R76] 使用临时文件
来源：http://yfz.shuidangran.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cxi.xingfuxueyuan.xyz

[R77] 读取用户输入
来源：http://amu.svipenyu.cn

read -rp "请输入: " ans
来源：http://lmi.yj20258.top

[R78] 交互式菜单
来源：http://dee.jqgufenzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://mbi.yj20258888.top

[R79] 解析命令行选项
来源：http://nab.shanyushiyangtech.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rjm.gzhubu.top

[R80] 查看脚本执行耗时
来源：http://gzq.smart0.xyz

time ./run.sh
来源：http://wuz.cashguo.top

================================================================================
来源：http://onn.ydjk.org.cn

S. C / C++ 专题
来源：http://bvp.shzxlz.cn

================================================================================
来源：http://szc.ivvv.top

[S01] C：Hello World
来源：http://wno.xingfuxueyuan.xyz

#include <stdio.h>
来源：http://yqu.xuanzx.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://jnb.c1oappe.top

[S02] C：变量与格式化输出
来源：http://hqo.zhiwuduotai.top

int a = 10; printf("%d\n", a);
来源：http://zal.cdnleiting.top

[S03] C：读入整数
来源：http://sqa.xinyue.icu

int x; scanf("%d", &x);
来源：http://ali.yfazqb.com

[S04] C：字符串复制
来源：http://cxe.gzhubu.top

char dst[32]; strcpy(dst, "hi");
来源：http://fhc.shangyingyoupin.top

[S05] C：字符串长度
来源：http://gle.havefunace.top

strlen(s)
来源：http://aqu.fengsongda.top

[S06] C：字符串比较
来源：http://jih.hnxiangtu.top

strcmp(a, b) == 0
来源：http://vjy.wangdashe.top

[S07] C：数组遍历求和
来源：http://dji.tarul.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ayd.pycfn.com

[S08] C：动态内存分配与释放
来源：http://nnk.ppjwa.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jnm.zhaomingkeji.xyz

[S09] C：结构体定义与初始化
来源：http://wra.kuanghao11.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kxh.nwbrower.top

[S10] C：指针与解引用
来源：http://ziy.gaohongyu789.top

int *p = &a;  *p = 5;
来源：http://wzx.hywenlv.cn

[S11] C：逐行读文件
来源：http://uqr.sjlbkw.cn

FILE *f = fopen("a.txt", "r");
来源：http://daq.epnwcf.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://sdn.chenjidiqi.icu

fclose(f);
来源：http://zjb.c1oappe.top

[S12] C：写文件
来源：http://hhe.dashuyun.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mdr.yanxiufei.cn

[S13] C：宏定义
来源：http://psp.chenzaomai.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://djc.iojbl.cn

[S14] C：枚举
来源：http://ftx.yj20258888.top

enum Color { RED, GREEN, BLUE };
来源：http://kyo.chenzaomai.com

[S15] C：类型转换
来源：http://hcr.wangdashe.top

(double) a / b
来源：http://nxl.chenjidiqi.icu

[S16] C：位操作置位
来源：http://dah.tarul.cn

x |= (1 << 3);
来源：http://uct.havefunace.top

[S17] C：安全拼接字符串
来源：http://gta.fanxiaobao.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ubc.iojbl.cn

[S18] C：命令行参数
来源：http://lkb.jqgufenzy.top

int main(int argc, char **argv)
来源：http://brb.quarkkingdee.top

[S19] C：快速排序
来源：http://vlu.hammf.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nvd.jlsjyb.cn

[S20] C：二分查找
来源：http://upy.nanxinkj.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zmp.xinyue.icu

[S21] C：字符类别判断
来源：http://sfc.ydjk.org.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sjc.zhiwuduotai.top

[S22] C：字符串转数字
来源：http://xph.xingfuxueyuan.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://ayt.jyoumei.cn

[S23] C：随机数
来源：http://jrv.yongpay.top

srand(time(NULL));  int r = rand() % 100;
来源：http://lhn.gzhubu.top

[S24] C：获取本地时间
来源：http://ckd.mhx1999.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xdq.nwbrower.top

[S25] C：内存拷贝
来源：http://kde.yangfankeji.com

memcpy(dst, src, n);
来源：http://eyr.nwbrower.top

[S26] C：内存清零
来源：http://bke.daxiang520.top

memset(a, 0, sizeof a);
来源：http://wdj.yangfankeji.com

[S27] C：定义常量
来源：http://ilm.cucudq.cn

const double PI = 3.14159;
来源：http://lda.zhijiandao.cn

[S28] C：静态变量
来源：http://tcg.hnqzz.top

static int counter = 0;
来源：http://xtk.fehbvm.com

[S29] C：变参函数
来源：http://nit.yuxming.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yya.zhijiandao.cn

[S30] C：头文件保护
来源：http://qba.hfpthk.cn

#ifndef X_H
来源：http://cdv.shanyushiyangkeji.top

#define X_H
来源：http://tje.bbcook.cn

#endif
来源：http://hxw.vqdsnc.cn

[S31] C++：Hello World
来源：http://alm.316326.xyz

#include <iostream>
来源：http://jdw.chenlongwang.top

int main() { std::cout << "Hello\n"; }
来源：http://whm.guowangkeji.top

[S32] C++：字符串
来源：http://czl.zhoulong.xyz

std::string s = "hi";  s += "!";
来源：http://mic.gzhubu.top

[S33] C++：vector 增删
来源：http://kfk.yuxming.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ubm.vqdsnc.cn

[S34] C++：遍历 vector
来源：http://ssy.vqdsnc.cn

for (auto &x : v) { std::cout << x; }
来源：http://oed.zdbjq.cn

[S35] C++：map
来源：http://rdv.jyoumei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gwn.cdnleiting.top

[S36] C++：unordered_map
来源：http://pnc.jinghuilouyu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ytl.zhaomingkeji.xyz

[S37] C++：set
来源：http://sld.yueranfly.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ecx.xziqi.cn

[S38] C++：排序
来源：http://jpb.vehdjk.com

std::sort(v.begin(), v.end());
来源：http://cfo.yj20258888.top

[S39] C++：自定义比较器排序
来源：http://ocy.ehwqpu.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://shx.haohaochexian.top

[S40] C++：查找元素
来源：http://qwr.aibaodan.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gjr.zdqjudy.top

[S41] C++：类与构造函数
来源：http://pwe.wangdashe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qzt.xuanzx.com

[S42] C++：继承与虚函数
来源：http://tpi.wangshuangyany.cn

class B : public Base { public: void f() override {} };
来源：http://tod.redwolf501.top

[S43] C++：智能指针
来源：http://jqc.redwolf501.top

auto p = std::make_unique<int>(5);
来源：http://icx.pengpengdd.cyou

[S44] C++：引用传参
来源：http://yup.dashuyun.cn

void inc(int &x) { ++x; }
来源：http://hdk.yfazqb.com

[S45] C++：lambda
来源：http://mey.tian-w.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ovz.pycfn.com

[S46] C++：函数模板
来源：http://fdn.shanyushiyangkeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kvf.jqgufenzy.top

[S47] C++：结构化绑定遍历
来源：http://vmm.xuanzx.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fvu.daxiang520.top

[S48] C++：逐行读文件
来源：http://sie.zhongyouzk.top

std::ifstream in("a.txt");  std::string line;
来源：http://tpf.sufxvd.cn

while (std::getline(in, line)) { }
来源：http://ndn.hammf.cn

[S49] C++：写文件
来源：http://mun.daxiang520.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hzt.zhengqikj.top

[S50] C++：格式化数字
来源：http://bqa.zhengqikj.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://exz.jyoumei.cn

[S51] C++：显式类型转换
来源：http://qyh.vehdjk.com

static_cast<double>(a) / b
来源：http://jjb.zhongyouzk.top

[S52] C++：const 与 noexcept
来源：http://vcg.haohaochexian.top

int size() const noexcept { return n_; }
来源：http://xbd.mhx1999.top

[S53] C++：移动语义
来源：http://eib.quarkkingdee.top

std::vector<int> w = std::move(v);
来源：http://pcs.jianghu66.top

[S54] C++：异常处理
来源：http://idg.bbcook.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qnt.aizwys.cn

[S55] C++：结构化绑定
来源：http://hne.ehwqpu.com

auto [a, b] = std::make_pair(1, 2);
来源：http://zrh.316326.xyz

[S56] C++：optional
来源：http://thr.hnqzz.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cqy.quarkkingdee.top

[S57] C++：编译期常量
来源：http://xfz.yanxiufei.cn

constexpr int N = 10;
来源：http://fme.yj202588.top

[S58] C++：命名空间
来源：http://xab.cheryme.top

namespace ns { int f() { return 1; } }
来源：http://iju.shanyushiyangtech.top

[S59] C++：静态断言
来源：http://hkh.yueranfly.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wgs.fengsongda.top

[S60] C++：遍历并删除元素
来源：http://jpj.bjfxy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bxk.zdbjq.cn

================================================================================
来源：http://tkq.daxiang520.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lop.tian-w.cn

================================================================================
来源：http://mne.yj20258888.top

[T01] Kotlin：Hello World
来源：http://bfc.ctjpmb.com

println("Hello")
来源：http://rtj.cqqwz.cn

[T02] Kotlin：变量
来源：http://ljc.hesvh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zja.ywan-chungtsiang.top

[T03] Kotlin：字符串模板
来源：http://qgx.fehbvm.com

"值: $b"
来源：http://avc.jqgufenzy.top

[T04] Kotlin：空安全
来源：http://mrx.guowangkeji.top

val n: String? = null;  n?.length
来源：http://fpn.chenjidiqi.icu

[T05] Kotlin：when 表达式
来源：http://aev.gaohongyu789.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rmf.nanxinkj.top

[T06] Kotlin：集合映射
来源：http://kqa.xinyue.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://wwf.jianghu66.top

[T07] Kotlin：集合过滤
来源：http://lvk.hammf.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fnw.jinqigufen.top

[T08] Kotlin：数据类
来源：http://olv.bjfxy.top

data class User(val name: String, val age: Int)
来源：http://kfe.redwolf501.top

[T09] Kotlin：扩展函数
来源：http://nud.aizwys.cn

fun String.exclaim() = this + "!"
来源：http://etp.zhengqikj.top

[T10] Kotlin：默认参数
来源：http://gae.yanxiufei.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pmz.ywan-chungtsiang.top

[T11] Kotlin：协程
来源：http://pnh.zhijiandao.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fhq.gogol.net.cn

[T12] Kotlin：解构声明
来源：http://jxf.zhiwuduotai.top

val (a, b) = Pair(1, 2)
来源：http://afo.daxiang520.top

[T13] Kotlin：只读 Map
来源：http://geb.gaohongyu789.top

val m = mapOf("a" to 1)
来源：http://igw.kuanghao11.cn

[T14] Kotlin：循环
来源：http://lzw.redwolf501.top

for (i in 1..10) println(i)
来源：http://sag.shangyingyoupin.top

[T15] Kotlin：接口
来源：http://dca.tian-w.cn

interface Shape { fun area(): Double }
来源：http://wop.gotoacloud.top

[T16] Swift：Hello World
来源：http://byi.zhaomingkeji.xyz

print("Hello")
来源：http://qqs.fanxiaobao.xyz

[T17] Swift：变量与常量
来源：http://msl.ybcxt.top

var a = 1;  let b = 2
来源：http://rbj.nwbrower.top

[T18] Swift：字符串插值
来源：http://ddd.hongshengwenyu.top

"值: \(b)"
来源：http://txv.52xcode.cn

[T19] Swift：可选绑定
来源：http://hfn.cheryme.top

if let n = opt { print(n) }
来源：http://gqt.cucudq.cn

[T20] Swift：数组操作
来源：http://xsk.xylfe.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mww.fzhhl.top

[T21] Swift：遍历
来源：http://oei.redwolf501.top

for x in a { print(x) }
来源：http://txv.tarul.cn

[T22] Swift：字典
来源：http://wqg.smart0.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://hqy.jinyuanbaomall.cn

[T23] Swift：函数
来源：http://hke.chenlongwang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://viv.cdnleiting.top

[T24] Swift：闭包
来源：http://uha.yanxiufei.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xmv.yj20258.top


<!-- 参考信息 -->