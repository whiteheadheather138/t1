代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://myt.xinyue.icu

[R18] 遍历数组
来源：http://tqx.ywan-chungtsiang.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hbj.yfazqb.com

[R19] 数组长度
来源：http://vhb.316326.xyz

echo "${#arr[@]}"
来源：http://kqz.cucudq.cn

[R20] 关联数组（字典）
来源：http://ofn.guowangkeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sza.pengpengdd.cyou

[R21] 字符串长度
来源：http://pvl.ydjk.org.cn

echo "${#s}"
来源：http://zpm.yfazqb.com

[R22] 截取子串
来源：http://sel.jqgfzy.top

echo "${s:0:5}"
来源：http://haz.ydzc1.top

[R23] 字符串替换
来源：http://ncs.svipenyu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eyf.smart0.xyz

[R24] 大小写转换
来源：http://cbx.uphjek.com

echo "${s^^}"; echo "${s,,}"
来源：http://iga.yfazqb.com

[R25] 去后缀 / 去前缀
来源：http://liv.c1oappe.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://cqf.ivvv.top

[R26] 命令替换
来源：http://ahd.ivvv.top

now=$(date +%F); echo "$now"
来源：http://ngw.cucudq.cn

[R27] 算术展开
来源：http://yjd.cashguo.top

echo $((1 + 2 * 3))
来源：http://dxa.0kj1m.cn

[R28] 浮点运算
来源：http://tsx.vqdsnc.cn

echo "scale=2; 10/3" | bc
来源：http://qeh.chenlongwang.top

[R29] 定义函数
来源：http://mkn.xylfe.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ell.wangdashe.top

[R30] 函数返回状态码
来源：http://vgy.zhengqikj.top

f() { return 0; }; f || echo "失败了"
来源：http://fba.redwolf501.top

[R31] 局部变量
来源：http://jal.zycfv.cn

f() { local x=1; echo "$x"; }
来源：http://bss.ppjwa.cn

[R32] 参数个数校验
来源：http://zxj.hesvh.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nun.guowangkeji.top

[R33] 捕获错误并提示行号
来源：http://qrn.haohaochexian.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mme.jyoumei.cn

[R34] 退出时清理
来源：http://zku.jianghu66.top

trap 'rm -f "$tmp"' EXIT
来源：http://njq.hammf.cn

[R35] 后台执行并等待
来源：http://pjr.feifeiyinyue.top

sleep 5 & pid=$!; wait "$pid"
来源：http://xeg.gaohongyu789.top

[R36] 并发执行多个任务
来源：http://imz.zhongyouzk.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pso.xinyue.icu

[R37] 把输出赋给变量
来源：http://cba.shangyingyoupin.top

files=$(ls -1)
来源：http://duk.zhaomingkeji.xyz

[R38] 管道串联
来源：http://mem.vehdjk.com

cat a.txt | grep -i error | wc -l
来源：http://lxa.316326.xyz

[R39] 重定向标准输出与错误
来源：http://ygw.c1oappe.top

cmd > out.log 2>&1
来源：http://lyh.fehbvm.com

[R40] 追加写日志
来源：http://iui.gaohongyu789.top

echo "log" >> out.log
来源：http://gad.epnwcf.com

[R41] 丢弃输出
来源：http://dfy.xinyue.icu

cmd >/dev/null 2>&1
来源：http://uiv.hammf.cn

[R42] 输入重定向
来源：http://bzp.daria6918.cn

wc -l < a.txt
来源：http://rsl.zhixingplan.top

[R43] 按名字查找文件
来源：http://qtu.cashguo.top

find . -name "*.log" -type f
来源：http://fym.yuxming.cn

[R44] 按修改时间查找
来源：http://flv.zdbjq.cn

find . -mtime -7 -type f
来源：http://rea.daria6918.cn

[R45] 批量删除
来源：http://jdf.birdmap.top

find . -name "*.tmp" -delete
来源：http://ggr.316326.xyz

[R46] 递归替换文件内容
来源：http://ojd.zhaomingkeji.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nmh.yuanzhike.top

[R47] sed 单行替换
来源：http://ylb.yj20258888.top

sed -i 's/foo/bar/g' a.txt
来源：http://wlp.fzhhl.top

[R48] awk 取指定列
来源：http://gps.iojbl.cn

awk '{print $1, $3}' a.txt
来源：http://tvm.52xcode.cn

[R49] awk 带条件
来源：http://oju.zhixingplan.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://clv.xylfe.cn

[R50] awk 求和
来源：http://ntj.yvedp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://inm.aizwys.cn

[R51] 排序去重取前几
来源：http://tcw.tianlin.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://udv.redwolf501.top

[R52] 统计行数
来源：http://fgf.yangfankeji.com

wc -l a.txt
来源：http://uvb.jinqigfzy.top

[R53] 查看文件头与实时尾
来源：http://vnw.shuidangran.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ycm.sufxvd.cn

[R54] 比较两个文件
来源：http://oaj.sxryk.cn

diff a.txt b.txt
来源：http://bwo.gzhubu.top

[R55] 压缩与解压
来源：http://xoy.chenjidiqi.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://icv.haohaochexian.top

[R56] 远程拷贝
来源：http://cfu.chenlongwang.top

scp file user@host:/path/
来源：http://ejk.ehwqpu.com

[R57] 远程执行命令
来源：http://nqd.jinyuanbaomall.cn

ssh user@host 'uptime'
来源：http://ful.hammf.cn

[R58] 下载文件
来源：http://hhi.yj20258.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://myg.jyoumei.cn

[R59] 发 POST JSON
来源：http://ahf.jinqigufen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wql.hnqzz.top

[R60] 只看 HTTP 状态码
来源：http://nma.xinyue.icu

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jcg.fehbvm.com

[R61] 磁盘占用
来源：http://yvz.sjlbkw.cn

df -h;  du -sh *
来源：http://kmi.guowangkeji.top

[R62] 找最占空间的文件
来源：http://gtl.ehwqpu.com

du -ah . | sort -rh | head -10
来源：http://dcz.mhx1999.top

[R63] 内存与进程
来源：http://wob.cqqwz.cn

free -h;  ps aux | grep nginx
来源：http://poj.haohaochexian.top

[R64] 结束进程
来源：http://hma.ivvv.top

kill -9 $(pgrep -f app.py)
来源：http://abw.guannengcc.top

[R65] 查看端口占用
来源：http://ebg.jyoumei.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qtg.wangshuangyany.cn

[R66] 定时任务
来源：http://upy.jinqigufen.top

crontab -e;  crontab -l
来源：http://fyf.shzxlz.cn

[R67] 生成随机十六进制串
来源：http://gry.tianlin.xyz

openssl rand -hex 16
来源：http://ftr.zhoulong.xyz

[R68] 计算文件校验值
来源：http://atq.zhengqikj.top

sha256sum a.txt;  md5sum a.txt
来源：http://nbq.xuanzx.com

[R69] 生成随机密码
来源：http://whb.316326.xyz

head -c 16 /dev/urandom | base64
来源：http://qcs.yanxiufei.cn

[R70] 时间戳与互转
来源：http://bsx.hnqzz.top

date +%s;  date -d @1700000000
来源：http://ueu.tanke756.top

[R71] 日期格式化
来源：http://cpb.yonumen.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://mzo.gaohongyu789.top

[R72] 等待端口就绪
来源：http://tgn.andypj.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://ybo.pycfn.com

[R73] 分割大日志
来源：http://ukd.zhijiandao.cn

split -l 1000 big.log part_
来源：http://zpj.fanxiaobao.xyz

[R74] 批量重命名
来源：http://kqx.guannengcc.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zda.havefunace.top

[R75] 导出环境变量
来源：http://jnq.nanxinkj.top

export PATH="$HOME/bin:$PATH"
来源：http://ryb.yanxiufei.cn

[R76] 使用临时文件
来源：http://vpp.ppjwa.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yxx.jqgfzy.top

[R77] 读取用户输入
来源：http://wbq.cqqwz.cn

read -rp "请输入: " ans
来源：http://czi.gaohongyu789.top

[R78] 交互式菜单
来源：http://beu.uphjek.com

select opt in a b c; do echo "$opt"; break; done
来源：http://qcg.yvedp.cn

[R79] 解析命令行选项
来源：http://kss.hammf.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hrs.nanxuanxn.top

[R80] 查看脚本执行耗时
来源：http://cqe.zhengqikj.top

time ./run.sh
来源：http://ucr.daria6918.cn

================================================================================
来源：http://fdb.c1oappe.top

S. C / C++ 专题
来源：http://fvr.cucudq.cn

================================================================================
来源：http://tnt.sysykeji.top

[S01] C：Hello World
来源：http://pkz.sxryk.cn

#include <stdio.h>
来源：http://udm.ctjpmb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://zmk.zhoulong.xyz

[S02] C：变量与格式化输出
来源：http://jno.zhongyouzk.top

int a = 10; printf("%d\n", a);
来源：http://zab.tarul.cn

[S03] C：读入整数
来源：http://ygg.ywan-chungtsiang.top

int x; scanf("%d", &x);
来源：http://fvm.zycfv.cn

[S04] C：字符串复制
来源：http://pqs.sjlbkw.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xyd.jinyuanbaomall.cn

[S05] C：字符串长度
来源：http://tux.hysaishi.cn

strlen(s)
来源：http://qbj.yuanzhike.top

[S06] C：字符串比较
来源：http://glt.9152youxi.cn

strcmp(a, b) == 0
来源：http://slm.guannengcc.top

[S07] C：数组遍历求和
来源：http://hdh.guowangkeji.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://peq.zycfv.cn

[S08] C：动态内存分配与释放
来源：http://rxx.chenjidiqi.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://loc.xuanzx.com

[S09] C：结构体定义与初始化
来源：http://cdh.nanxinkj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tqr.nwbrower.top

[S10] C：指针与解引用
来源：http://jvy.zhaomingkeji.xyz

int *p = &a;  *p = 5;
来源：http://rpu.fanxiaobao.xyz

[S11] C：逐行读文件
来源：http://fci.fehbvm.com

FILE *f = fopen("a.txt", "r");
来源：http://tqd.zhengqikj.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://jaa.sysykeji.top

fclose(f);
来源：http://itf.daria6918.cn

[S12] C：写文件
来源：http://lac.zhongyouzk.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xgm.zdqjudy.top

[S13] C：宏定义
来源：http://wgf.havefunace.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jjq.tarul.cn

[S14] C：枚举
来源：http://hlm.fengsongda.top

enum Color { RED, GREEN, BLUE };
来源：http://ila.jianghu66.top

[S15] C：类型转换
来源：http://xel.yj20258888.top

(double) a / b
来源：http://dxq.chenjidiqi.icu

[S16] C：位操作置位
来源：http://jic.jiagoushi.top

x |= (1 << 3);
来源：http://xhv.gzhubu.top

[S17] C：安全拼接字符串
来源：http://vql.tanke756.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jtv.hongshengwenyu.top

[S18] C：命令行参数
来源：http://mby.uphjek.com

int main(int argc, char **argv)
来源：http://zty.fengsongda.top

[S19] C：快速排序
来源：http://jbh.yvedp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gas.hnqzz.top

[S20] C：二分查找
来源：http://ump.daxiang520.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bpv.tianlin.xyz

[S21] C：字符类别判断
来源：http://twq.nanxinkj.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://czm.nanxuanxn.top

[S22] C：字符串转数字
来源：http://dnd.nanxinkj.top

atoi("42");  strtod("3.14", NULL);
来源：http://naq.yonumen.top

[S23] C：随机数
来源：http://teo.hongshengwenyu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mqy.hywenlv.cn

[S24] C：获取本地时间
来源：http://jgs.gaohongyu789.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://olp.hongshengwenyu.top

[S25] C：内存拷贝
来源：http://xld.jyoumei.cn

memcpy(dst, src, n);
来源：http://gnu.hcnkem.com

[S26] C：内存清零
来源：http://lgg.c1oappe.top

memset(a, 0, sizeof a);
来源：http://nyc.daxiang520.top

[S27] C：定义常量
来源：http://fas.dianchejie.cn

const double PI = 3.14159;
来源：http://aof.uphjek.com

[S28] C：静态变量
来源：http://agx.epnwcf.com

static int counter = 0;
来源：http://orx.svipenyu.cn

[S29] C：变参函数
来源：http://ums.nanxuanxn.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lyz.daria6918.cn

[S30] C：头文件保护
来源：http://ccl.yfazqb.com

#ifndef X_H
来源：http://xfq.kuanghao11.cn

#define X_H
来源：http://sjc.cqqwz.cn

#endif
来源：http://xyp.zhaomingkeji.xyz

[S31] C++：Hello World
来源：http://npa.yvedp.cn

#include <iostream>
来源：http://pxi.sysykeji.top

int main() { std::cout << "Hello\n"; }
来源：http://otk.nanxuanxn.top

[S32] C++：字符串
来源：http://qxo.yuxming.cn

std::string s = "hi";  s += "!";
来源：http://rlx.ivvv.top

[S33] C++：vector 增删
来源：http://pdb.zhengqikj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eah.yueranfly.top

[S34] C++：遍历 vector
来源：http://cqm.sufxvd.cn

for (auto &x : v) { std::cout << x; }
来源：http://xxt.zhixingplan.top

[S35] C++：map
来源：http://ols.sjlbkw.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qah.daxiang520.top

[S36] C++：unordered_map
来源：http://bru.hnxiangtu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cpn.jinghuilouyu.cn

[S37] C++：set
来源：http://hpl.nwbrower.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pma.cucudq.cn

[S38] C++：排序
来源：http://wng.shanyushiyangkeji.top

std::sort(v.begin(), v.end());
来源：http://yfb.jinqigfzy.top

[S39] C++：自定义比较器排序
来源：http://yji.iojbl.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nwz.hfpthk.cn

[S40] C++：查找元素
来源：http://zyt.zhiwuduotai.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rbh.guowangkeji.top

[S41] C++：类与构造函数
来源：http://ywq.mhx1999.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bvf.daria6918.cn

[S42] C++：继承与虚函数
来源：http://vnv.aibaodan.cn

class B : public Base { public: void f() override {} };
来源：http://xit.yj20258888.top

[S43] C++：智能指针
来源：http://ohl.vehdjk.com

auto p = std::make_unique<int>(5);
来源：http://sxl.zhijiandao.cn

[S44] C++：引用传参
来源：http://vkx.guowangkeji.top

void inc(int &x) { ++x; }
来源：http://yqt.pengpengdd.cyou

[S45] C++：lambda
来源：http://beb.hywenlv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://iou.jqgfzy.top

[S46] C++：函数模板
来源：http://iii.hongshengwenyu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gaw.pengpengdd.cyou

[S47] C++：结构化绑定遍历
来源：http://pba.pengpengdd.cyou

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iwl.chenlongwang.top

[S48] C++：逐行读文件
来源：http://lay.zhiwuduotai.top

std::ifstream in("a.txt");  std::string line;
来源：http://lsz.xinyue.icu

while (std::getline(in, line)) { }
来源：http://ihx.yvedp.cn

[S49] C++：写文件
来源：http://eud.fengsongda.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fja.zhoulong.xyz

[S50] C++：格式化数字
来源：http://ofj.316326.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zxe.zhaomingkeji.xyz

[S51] C++：显式类型转换
来源：http://pil.feifeiyinyue.top

static_cast<double>(a) / b
来源：http://xip.cucudq.cn

[S52] C++：const 与 noexcept
来源：http://lvj.ehwqpu.com

int size() const noexcept { return n_; }
来源：http://xqe.birdmap.top

[S53] C++：移动语义
来源：http://qur.gotoacloud.top

std::vector<int> w = std::move(v);
来源：http://htt.zhiwuduotai.top

[S54] C++：异常处理
来源：http://swy.fktsv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lql.pengpengdd.cyou

[S55] C++：结构化绑定
来源：http://ooj.tarul.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vyv.svipenyu.cn

[S56] C++：optional
来源：http://sxe.yuanzhike.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://txw.ybcxt.top

[S57] C++：编译期常量
来源：http://twn.wangdashe.top

constexpr int N = 10;
来源：http://gfr.dashuyun.cn

[S58] C++：命名空间
来源：http://cdh.dianchejie.cn

namespace ns { int f() { return 1; } }
来源：http://asf.jinyuanbaomall.cn

[S59] C++：静态断言
来源：http://qve.gaohongyu789.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://utc.guannengcc.top

[S60] C++：遍历并删除元素
来源：http://zmm.52xcode.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ybt.svipenyu.cn

================================================================================
来源：http://cby.chenzaomai.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tdp.sxryk.cn

================================================================================
来源：http://wzh.xingfuxueyuan.xyz

[T01] Kotlin：Hello World
来源：http://qfz.daria6918.cn

println("Hello")
来源：http://ehv.yueranfly.top

[T02] Kotlin：变量
来源：http://yoe.yuxming.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yzt.yj20258.top

[T03] Kotlin：字符串模板
来源：http://qnr.daxiang520.top

"值: $b"
来源：http://dvq.hywenlv.cn

[T04] Kotlin：空安全
来源：http://rdi.dashuyun.cn

val n: String? = null;  n?.length
来源：http://rxd.xylfe.cn

[T05] Kotlin：when 表达式
来源：http://khz.meibo888.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vqq.yanxiufei.cn

[T06] Kotlin：集合映射
来源：http://jnn.pengpengdd.cyou

listOf(1, 2, 3).map { it * 2 }
来源：http://ack.hysaishi.cn

[T07] Kotlin：集合过滤
来源：http://yla.aibaodan.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pxq.pycfn.com

[T08] Kotlin：数据类
来源：http://jnb.cqqwz.cn

data class User(val name: String, val age: Int)
来源：http://yyu.zhengqikj.top

[T09] Kotlin：扩展函数
来源：http://rpb.chenlongwang.top

fun String.exclaim() = this + "!"
来源：http://cfi.sufxvd.cn

[T10] Kotlin：默认参数
来源：http://ksr.yj202588.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qrk.zhijiandao.cn

[T11] Kotlin：协程
来源：http://syb.guannengcc.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://axq.jinghuilouyu.cn

[T12] Kotlin：解构声明
来源：http://mhr.aibaodan.cn

val (a, b) = Pair(1, 2)
来源：http://jev.zycfv.cn

[T13] Kotlin：只读 Map
来源：http://lst.zdqjudy.top

val m = mapOf("a" to 1)
来源：http://gqn.sweek.top

[T14] Kotlin：循环
来源：http://wpp.zdbjq.cn

for (i in 1..10) println(i)
来源：http://wbi.mhx1999.top

[T15] Kotlin：接口
来源：http://syq.ivvv.top

interface Shape { fun area(): Double }
来源：http://whk.jinyuanbaomall.cn

[T16] Swift：Hello World
来源：http://otx.nanxinkj.top

print("Hello")
来源：http://gve.zhengqikj.top

[T17] Swift：变量与常量
来源：http://aaw.52xcode.cn

var a = 1;  let b = 2
来源：http://ghn.yanxiufei.cn

[T18] Swift：字符串插值
来源：http://xkm.hongshengwenyu.top

"值: \(b)"
来源：http://gmx.shanyushiyangkeji.top

[T19] Swift：可选绑定
来源：http://pzc.jinqigfzy.top

if let n = opt { print(n) }
来源：http://gox.daria6918.cn

[T20] Swift：数组操作
来源：http://mns.bjfxy.top

var a = [1, 2, 3];  a.append(4)
来源：http://ihp.zhaomingkeji.xyz


<!-- 参考信息 -->