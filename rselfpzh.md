代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://npl.zdbjq.cn

[R18] 遍历数组
来源：http://ovp.jinyuanbaomall.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wwh.smart0.xyz

[R19] 数组长度
来源：http://ymu.pengpengdd.cyou

echo "${#arr[@]}"
来源：http://xxr.hysaishi.cn

[R20] 关联数组（字典）
来源：http://puz.yvedp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mtx.nanxuanxn.top

[R21] 字符串长度
来源：http://lhl.gaohongyu789.top

echo "${#s}"
来源：http://lvl.xziqi.cn

[R22] 截取子串
来源：http://cyt.gzhubu.top

echo "${s:0:5}"
来源：http://rmu.smart0.xyz

[R23] 字符串替换
来源：http://pnj.tianlin.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nfq.uphjek.com

[R24] 大小写转换
来源：http://whx.smart0.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://uop.ivvv.top

[R25] 去后缀 / 去前缀
来源：http://itv.tianlin.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://bun.smart0.xyz

[R26] 命令替换
来源：http://zzz.yfazqb.com

now=$(date +%F); echo "$now"
来源：http://drz.yvedp.cn

[R27] 算术展开
来源：http://jey.zhongyouzk.top

echo $((1 + 2 * 3))
来源：http://xxu.zhixingplan.top

[R28] 浮点运算
来源：http://jpb.chenjidiqi.icu

echo "scale=2; 10/3" | bc
来源：http://zgu.yuanzhike.top

[R29] 定义函数
来源：http://qrn.dianchejie.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yfi.0kj1m.cn

[R30] 函数返回状态码
来源：http://dug.chenjidiqi.icu

f() { return 0; }; f || echo "失败了"
来源：http://jox.ydzc1.top

[R31] 局部变量
来源：http://jkn.316326.xyz

f() { local x=1; echo "$x"; }
来源：http://dun.fzhhl.top

[R32] 参数个数校验
来源：http://fil.zhixingplan.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pdw.hysaishi.cn

[R33] 捕获错误并提示行号
来源：http://tdz.ydzc1.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jvm.redwolf501.top

[R34] 退出时清理
来源：http://vbf.fengsongda.top

trap 'rm -f "$tmp"' EXIT
来源：http://gib.ybcxt.top

[R35] 后台执行并等待
来源：http://lfd.haohaochexian.top

sleep 5 & pid=$!; wait "$pid"
来源：http://yii.zdbjq.cn

[R36] 并发执行多个任务
来源：http://dqf.jyoumei.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jke.xingfuxueyuan.xyz

[R37] 把输出赋给变量
来源：http://faq.meibo888.top

files=$(ls -1)
来源：http://ipx.shangyingyoupin.top

[R38] 管道串联
来源：http://raq.nanxinkj.top

cat a.txt | grep -i error | wc -l
来源：http://jim.jqgfzy.top

[R39] 重定向标准输出与错误
来源：http://tge.yfazqb.com

cmd > out.log 2>&1
来源：http://iaz.yuxming.cn

[R40] 追加写日志
来源：http://mff.ctjpmb.com

echo "log" >> out.log
来源：http://kqf.jqgufenzy.top

[R41] 丢弃输出
来源：http://yem.52xcode.cn

cmd >/dev/null 2>&1
来源：http://vht.xuetiantiany.cn

[R42] 输入重定向
来源：http://jus.daria6918.cn

wc -l < a.txt
来源：http://blo.hnqzz.top

[R43] 按名字查找文件
来源：http://doa.yueranfly.top

find . -name "*.log" -type f
来源：http://oqp.zhixingplan.top

[R44] 按修改时间查找
来源：http://npd.zycfv.cn

find . -mtime -7 -type f
来源：http://ecp.zhixingplan.top

[R45] 批量删除
来源：http://tgj.tian-w.cn

find . -name "*.tmp" -delete
来源：http://lcy.hfpthk.cn

[R46] 递归替换文件内容
来源：http://fit.chenzaomai.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dck.sysykeji.top

[R47] sed 单行替换
来源：http://lbl.shanyushiyangtech.top

sed -i 's/foo/bar/g' a.txt
来源：http://nzh.cqqwz.cn

[R48] awk 取指定列
来源：http://kux.shangyingyoupin.top

awk '{print $1, $3}' a.txt
来源：http://dtx.bjfxy.top

[R49] awk 带条件
来源：http://ikr.sjlbkw.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iny.andypj.xyz

[R50] awk 求和
来源：http://soa.aibaodan.cn

awk '{s += $2} END {print s}' a.txt
来源：http://skw.ydzc1.top

[R51] 排序去重取前几
来源：http://brz.havefunace.top

sort a.txt | uniq -c | sort -rn | head
来源：http://tbc.yuxming.cn

[R52] 统计行数
来源：http://tds.vehdjk.com

wc -l a.txt
来源：http://bky.iojbl.cn

[R53] 查看文件头与实时尾
来源：http://yji.cashguo.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vdd.zhaomingkeji.xyz

[R54] 比较两个文件
来源：http://wjr.guowangkeji.top

diff a.txt b.txt
来源：http://rzt.zdqjudy.top

[R55] 压缩与解压
来源：http://rpc.xinyue.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vne.mhx1999.top

[R56] 远程拷贝
来源：http://exu.dashuyun.cn

scp file user@host:/path/
来源：http://dmb.hesvh.cn

[R57] 远程执行命令
来源：http://ivr.jiagoushi.top

ssh user@host 'uptime'
来源：http://whd.hammf.cn

[R58] 下载文件
来源：http://vyy.sjlbkw.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nyb.xuanzx.com

[R59] 发 POST JSON
来源：http://vei.ywan-chungtsiang.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blf.uphjek.com

[R60] 只看 HTTP 状态码
来源：http://hlb.shzxlz.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://thn.mhx1999.top

[R61] 磁盘占用
来源：http://akj.uphjek.com

df -h;  du -sh *
来源：http://ewl.yongpay.top

[R62] 找最占空间的文件
来源：http://zau.pycfn.com

du -ah . | sort -rh | head -10
来源：http://dbb.hnxiangtu.top

[R63] 内存与进程
来源：http://qbq.wangshuangyany.cn

free -h;  ps aux | grep nginx
来源：http://klj.zhijiandao.cn

[R64] 结束进程
来源：http://atb.yj20258.top

kill -9 $(pgrep -f app.py)
来源：http://cyc.yanxiufei.cn

[R65] 查看端口占用
来源：http://hyk.daria6918.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kps.dianchejie.cn

[R66] 定时任务
来源：http://brh.52xcode.cn

crontab -e;  crontab -l
来源：http://glq.shangyingyoupin.top

[R67] 生成随机十六进制串
来源：http://pdb.shuidangran.top

openssl rand -hex 16
来源：http://ljx.gotoacloud.top

[R68] 计算文件校验值
来源：http://mxm.52xcode.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ijn.havefunace.top

[R69] 生成随机密码
来源：http://dpy.zhongyouzk.top

head -c 16 /dev/urandom | base64
来源：http://cua.nanxinkj.top

[R70] 时间戳与互转
来源：http://uja.havefunace.top

date +%s;  date -d @1700000000
来源：http://gbq.aibaodan.cn

[R71] 日期格式化
来源：http://tsp.tian-w.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://pmm.jlsjyb.cn

[R72] 等待端口就绪
来源：http://jyv.yueranfly.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ucr.zhiwuduotai.top

[R73] 分割大日志
来源：http://ynq.havefunace.top

split -l 1000 big.log part_
来源：http://bkf.shanyushiyangtech.top

[R74] 批量重命名
来源：http://itj.shangyingyoupin.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zsz.xziqi.cn

[R75] 导出环境变量
来源：http://xly.jqgfzy.top

export PATH="$HOME/bin:$PATH"
来源：http://qsu.yj20258.top

[R76] 使用临时文件
来源：http://eux.chenzaomai.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://exb.hfpthk.cn

[R77] 读取用户输入
来源：http://bvx.xinyue.icu

read -rp "请输入: " ans
来源：http://wen.hesvh.cn

[R78] 交互式菜单
来源：http://knw.gogol.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uwx.yfazqb.com

[R79] 解析命令行选项
来源：http://evm.hongshengwenyu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wrz.52xcode.cn

[R80] 查看脚本执行耗时
来源：http://huy.0kj1m.cn

time ./run.sh
来源：http://ylx.uphjek.com

================================================================================
来源：http://wlt.quarkkingdee.top

S. C / C++ 专题
来源：http://quw.nwbrower.top

================================================================================
来源：http://znc.chenjidiqi.icu

[S01] C：Hello World
来源：http://umz.dianchejie.cn

#include <stdio.h>
来源：http://xah.vehdjk.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://rhe.zhoulong.xyz

[S02] C：变量与格式化输出
来源：http://wrz.zhixingplan.top

int a = 10; printf("%d\n", a);
来源：http://ptj.zhiwuduotai.top

[S03] C：读入整数
来源：http://ftp.cucudq.cn

int x; scanf("%d", &x);
来源：http://mlr.nanxinkj.top

[S04] C：字符串复制
来源：http://wgj.sysykeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://rom.dianchejie.cn

[S05] C：字符串长度
来源：http://lkh.ctjpmb.com

strlen(s)
来源：http://yvi.zdqjudy.top

[S06] C：字符串比较
来源：http://cca.uphjek.com

strcmp(a, b) == 0
来源：http://wdq.shanyushiyangkeji.top

[S07] C：数组遍历求和
来源：http://bjb.hongshengwenyu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gce.chenzaomai.com

[S08] C：动态内存分配与释放
来源：http://hsi.yonumen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xuy.yj202588.top

[S09] C：结构体定义与初始化
来源：http://glu.shuidangran.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mrj.quarkkingdee.top

[S10] C：指针与解引用
来源：http://sjq.fzhhl.top

int *p = &a;  *p = 5;
来源：http://krk.yfazqb.com

[S11] C：逐行读文件
来源：http://tpb.yj202588.top

FILE *f = fopen("a.txt", "r");
来源：http://vof.hammf.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ktr.zdbjq.cn

fclose(f);
来源：http://pmd.ybcxt.top

[S12] C：写文件
来源：http://wwa.chenlongwang.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dud.yuanzhike.top

[S13] C：宏定义
来源：http://mro.yongpay.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nub.dianchejie.cn

[S14] C：枚举
来源：http://bcy.hnxiangtu.top

enum Color { RED, GREEN, BLUE };
来源：http://ror.cucudq.cn

[S15] C：类型转换
来源：http://sre.bbcook.cn

(double) a / b
来源：http://qjk.hesvh.cn

[S16] C：位操作置位
来源：http://aav.xinyue.icu

x |= (1 << 3);
来源：http://lxf.nanxuanxn.top

[S17] C：安全拼接字符串
来源：http://dew.316326.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mkw.jinqigufen.top

[S18] C：命令行参数
来源：http://czf.ydjk.org.cn

int main(int argc, char **argv)
来源：http://tkm.zycfv.cn

[S19] C：快速排序
来源：http://kem.wangdashe.top

qsort(a, n, sizeof(int), cmp);
来源：http://tff.chenjidiqi.icu

[S20] C：二分查找
来源：http://jyp.xuetiantiany.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pms.fzhhl.top

[S21] C：字符类别判断
来源：http://dlo.hesvh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hyl.xingfuxueyuan.xyz

[S22] C：字符串转数字
来源：http://oag.fzhhl.top

atoi("42");  strtod("3.14", NULL);
来源：http://rso.ivvv.top

[S23] C：随机数
来源：http://pvy.zdbjq.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dlz.yj202588.top

[S24] C：获取本地时间
来源：http://yfv.hcnkem.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zwv.bbcook.cn

[S25] C：内存拷贝
来源：http://yde.wangdashe.top

memcpy(dst, src, n);
来源：http://jwf.yueranfly.top

[S26] C：内存清零
来源：http://bdz.ybcxt.top

memset(a, 0, sizeof a);
来源：http://fle.yuxming.cn

[S27] C：定义常量
来源：http://drf.vqdsnc.cn

const double PI = 3.14159;
来源：http://ewa.cucudq.cn

[S28] C：静态变量
来源：http://wnw.pengpengdd.cyou

static int counter = 0;
来源：http://mhh.shzxlz.cn

[S29] C：变参函数
来源：http://hdh.hnqzz.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rki.pengpengdd.cyou

[S30] C：头文件保护
来源：http://azz.yonumen.top

#ifndef X_H
来源：http://hhj.epnwcf.com

#define X_H
来源：http://xel.ehwqpu.com

#endif
来源：http://bqd.cheryme.top

[S31] C++：Hello World
来源：http://mbv.0kj1m.cn

#include <iostream>
来源：http://ptn.hesvh.cn

int main() { std::cout << "Hello\n"; }
来源：http://zgk.hfpthk.cn

[S32] C++：字符串
来源：http://yqx.ehwqpu.com

std::string s = "hi";  s += "!";
来源：http://blp.xylfe.cn

[S33] C++：vector 增删
来源：http://gxz.gzhubu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gew.daxiang520.top

[S34] C++：遍历 vector
来源：http://uou.aizwys.cn

for (auto &x : v) { std::cout << x; }
来源：http://lti.fengsongda.top

[S35] C++：map
来源：http://psv.jinqigfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fsz.tian-w.cn

[S36] C++：unordered_map
来源：http://obd.sjlbkw.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://aqu.yfazqb.com

[S37] C++：set
来源：http://nfj.guowangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hxi.shuidangran.top

[S38] C++：排序
来源：http://gyj.jiagoushi.top

std::sort(v.begin(), v.end());
来源：http://pov.zdbjq.cn

[S39] C++：自定义比较器排序
来源：http://gcl.gzhubu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ufv.ydzc1.top

[S40] C++：查找元素
来源：http://rdy.uphjek.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mnq.jinqigufen.top

[S41] C++：类与构造函数
来源：http://dih.feifeiyinyue.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://csg.redwolf501.top

[S42] C++：继承与虚函数
来源：http://hru.jinqigfzy.top

class B : public Base { public: void f() override {} };
来源：http://srb.zdbjq.cn

[S43] C++：智能指针
来源：http://ojx.xziqi.cn

auto p = std::make_unique<int>(5);
来源：http://rht.chenlongwang.top

[S44] C++：引用传参
来源：http://hwe.xziqi.cn

void inc(int &x) { ++x; }
来源：http://tke.chenjidiqi.icu

[S45] C++：lambda
来源：http://jat.mhx1999.top

auto add = [](int a, int b) { return a + b; };
来源：http://rrj.hfpthk.cn

[S46] C++：函数模板
来源：http://vdf.zdqjudy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://poq.cheryme.top

[S47] C++：结构化绑定遍历
来源：http://mch.bjfxy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lhs.jinqigufen.top

[S48] C++：逐行读文件
来源：http://bhk.cheryme.top

std::ifstream in("a.txt");  std::string line;
来源：http://yqp.fengsongda.top

while (std::getline(in, line)) { }
来源：http://iln.quarkkingdee.top

[S49] C++：写文件
来源：http://cvt.meibo888.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rcj.hfpthk.cn

[S50] C++：格式化数字
来源：http://acf.yanxiufei.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vov.c1oappe.top

[S51] C++：显式类型转换
来源：http://tno.xinyue.icu

static_cast<double>(a) / b
来源：http://yjx.epnwcf.com

[S52] C++：const 与 noexcept
来源：http://ptm.xuetiantiany.cn

int size() const noexcept { return n_; }
来源：http://gdq.xuetiantiany.cn

[S53] C++：移动语义
来源：http://fmx.cashguo.top

std::vector<int> w = std::move(v);
来源：http://gxr.hfpthk.cn

[S54] C++：异常处理
来源：http://ztq.yueranfly.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tpt.zhaomingkeji.xyz

[S55] C++：结构化绑定
来源：http://ped.dashuyun.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://eoa.ydjk.org.cn

[S56] C++：optional
来源：http://woo.gaohongyu789.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://leo.sysykeji.top

[S57] C++：编译期常量
来源：http://jha.gogol.net.cn

constexpr int N = 10;
来源：http://rpx.shangyingyoupin.top

[S58] C++：命名空间
来源：http://qqk.ybcxt.top

namespace ns { int f() { return 1; } }
来源：http://eip.zhongyouzk.top

[S59] C++：静态断言
来源：http://lik.yangfankeji.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wus.xziqi.cn

[S60] C++：遍历并删除元素
来源：http://wdm.feifeiyinyue.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qil.jiagoushi.top

================================================================================
来源：http://dtl.xinyue.icu

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uss.dianchejie.cn

================================================================================
来源：http://vna.snrcjt.cn

[T01] Kotlin：Hello World
来源：http://ggh.guannengcc.top

println("Hello")
来源：http://sra.316326.xyz

[T02] Kotlin：变量
来源：http://rog.chenzaomai.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zsn.zhaomingkeji.xyz

[T03] Kotlin：字符串模板
来源：http://jsd.uphjek.com

"值: $b"
来源：http://pvf.jianghu66.top

[T04] Kotlin：空安全
来源：http://qaa.aibaodan.cn

val n: String? = null;  n?.length
来源：http://jpy.bbcook.cn

[T05] Kotlin：when 表达式
来源：http://jtt.uphjek.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ore.shzxlz.cn

[T06] Kotlin：集合映射
来源：http://vpf.daria6918.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sbs.c1oappe.top

[T07] Kotlin：集合过滤
来源：http://ptc.hammf.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xeh.sufxvd.cn

[T08] Kotlin：数据类
来源：http://whi.jinghuilouyu.cn

data class User(val name: String, val age: Int)
来源：http://dgb.sufxvd.cn

[T09] Kotlin：扩展函数
来源：http://blj.uphjek.com

fun String.exclaim() = this + "!"
来源：http://hth.jiagoushi.top

[T10] Kotlin：默认参数
来源：http://bti.hnxiangtu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://pfr.zycfv.cn

[T11] Kotlin：协程
来源：http://spw.pycfn.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://fug.pengpengdd.cyou

[T12] Kotlin：解构声明
来源：http://oox.fzhhl.top

val (a, b) = Pair(1, 2)
来源：http://vby.dianchejie.cn

[T13] Kotlin：只读 Map
来源：http://mch.jiagoushi.top

val m = mapOf("a" to 1)
来源：http://hco.cheryme.top

[T14] Kotlin：循环
来源：http://jyg.shanyushiyangtech.top

for (i in 1..10) println(i)
来源：http://oii.zhoulong.xyz

[T15] Kotlin：接口
来源：http://qyk.snrcjt.cn

interface Shape { fun area(): Double }
来源：http://fkx.zhongyouzk.top

[T16] Swift：Hello World
来源：http://oki.shangyingyoupin.top

print("Hello")
来源：http://pfa.yvedp.cn

[T17] Swift：变量与常量
来源：http://lrq.xingfuxueyuan.xyz

var a = 1;  let b = 2
来源：http://rlm.hywenlv.cn

[T18] Swift：字符串插值
来源：http://xpk.fzhhl.top

"值: \(b)"
来源：http://odo.gogol.net.cn

[T19] Swift：可选绑定
来源：http://dps.yj202588.top

if let n = opt { print(n) }
来源：http://vhr.zdqjudy.top

[T20] Swift：数组操作
来源：http://lat.fzhhl.top

var a = [1, 2, 3];  a.append(4)
来源：http://dcq.316326.xyz


<!-- 参考信息 -->