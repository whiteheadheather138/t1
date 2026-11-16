代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://agd.ppjwa.cn

[R18] 遍历数组
来源：http://cjd.sufxvd.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://eji.shanyushiyangkeji.top

[R19] 数组长度
来源：http://pxq.gogol.net.cn

echo "${#arr[@]}"
来源：http://gck.ivvv.top

[R20] 关联数组（字典）
来源：http://abe.svipenyu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://buz.hesvh.cn

[R21] 字符串长度
来源：http://nof.dashuyun.cn

echo "${#s}"
来源：http://kbj.vqdsnc.cn

[R22] 截取子串
来源：http://kof.chenzaomai.com

echo "${s:0:5}"
来源：http://jyx.svipenyu.cn

[R23] 字符串替换
来源：http://iiw.hongshengwenyu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wwp.yj20258888.top

[R24] 大小写转换
来源：http://juo.c1oappe.top

echo "${s^^}"; echo "${s,,}"
来源：http://utw.meibo888.top

[R25] 去后缀 / 去前缀
来源：http://gtv.jyoumei.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://tdf.hammf.cn

[R26] 命令替换
来源：http://vdb.gaohongyu789.top

now=$(date +%F); echo "$now"
来源：http://rki.jlsjyb.cn

[R27] 算术展开
来源：http://lcl.shuidangran.top

echo $((1 + 2 * 3))
来源：http://yor.zdbjq.cn

[R28] 浮点运算
来源：http://wey.hnxiangtu.top

echo "scale=2; 10/3" | bc
来源：http://nge.gzhubu.top

[R29] 定义函数
来源：http://ckd.jiagoushi.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wib.sweek.top

[R30] 函数返回状态码
来源：http://ulu.bjfxy.top

f() { return 0; }; f || echo "失败了"
来源：http://jka.yuanzhike.top

[R31] 局部变量
来源：http://wey.dianchejie.cn

f() { local x=1; echo "$x"; }
来源：http://efy.hnxiangtu.top

[R32] 参数个数校验
来源：http://drz.gotoacloud.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mxa.hesvh.cn

[R33] 捕获错误并提示行号
来源：http://urn.nanxuanxn.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xku.shanyushiyangtech.top

[R34] 退出时清理
来源：http://doj.ywan-chungtsiang.top

trap 'rm -f "$tmp"' EXIT
来源：http://mrm.nwbrower.top

[R35] 后台执行并等待
来源：http://ucl.chenzaomai.com

sleep 5 & pid=$!; wait "$pid"
来源：http://eiq.dashuyun.cn

[R36] 并发执行多个任务
来源：http://ovv.sysykeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://owh.hongshengwenyu.top

[R37] 把输出赋给变量
来源：http://dyk.tianlin.xyz

files=$(ls -1)
来源：http://mhk.zhengqikj.top

[R38] 管道串联
来源：http://wrj.hnxiangtu.top

cat a.txt | grep -i error | wc -l
来源：http://gwd.yuanzhike.top

[R39] 重定向标准输出与错误
来源：http://gtr.0kj1m.cn

cmd > out.log 2>&1
来源：http://ude.kuanghao11.cn

[R40] 追加写日志
来源：http://gkl.haohaochexian.top

echo "log" >> out.log
来源：http://hzm.yuxming.cn

[R41] 丢弃输出
来源：http://jlo.yangfankeji.com

cmd >/dev/null 2>&1
来源：http://pzl.jlsjyb.cn

[R42] 输入重定向
来源：http://bmn.daxiang520.top

wc -l < a.txt
来源：http://jie.nanxinkj.top

[R43] 按名字查找文件
来源：http://isf.fengsongda.top

find . -name "*.log" -type f
来源：http://tnk.vqdsnc.cn

[R44] 按修改时间查找
来源：http://vib.hongshengwenyu.top

find . -mtime -7 -type f
来源：http://exh.sjlbkw.cn

[R45] 批量删除
来源：http://sgu.cqqwz.cn

find . -name "*.tmp" -delete
来源：http://pgc.gzhubu.top

[R46] 递归替换文件内容
来源：http://gdb.jinqigufen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tqi.jyoumei.cn

[R47] sed 单行替换
来源：http://mqo.jiagoushi.top

sed -i 's/foo/bar/g' a.txt
来源：http://zoq.52xcode.cn

[R48] awk 取指定列
来源：http://vht.tarul.cn

awk '{print $1, $3}' a.txt
来源：http://kxn.andypj.xyz

[R49] awk 带条件
来源：http://bzf.cheryme.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://chj.zdbjq.cn

[R50] awk 求和
来源：http://vck.zhoulong.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://ojm.wangdashe.top

[R51] 排序去重取前几
来源：http://ynb.jqgfzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://pum.fengsongda.top

[R52] 统计行数
来源：http://axn.yvedp.cn

wc -l a.txt
来源：http://yce.52xcode.cn

[R53] 查看文件头与实时尾
来源：http://kto.birdmap.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gwb.hesvh.cn

[R54] 比较两个文件
来源：http://nub.chenjidiqi.icu

diff a.txt b.txt
来源：http://mix.hywenlv.cn

[R55] 压缩与解压
来源：http://iey.zhoulong.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zgs.gogol.net.cn

[R56] 远程拷贝
来源：http://zyn.cashguo.top

scp file user@host:/path/
来源：http://vol.yongpay.top

[R57] 远程执行命令
来源：http://urs.svipenyu.cn

ssh user@host 'uptime'
来源：http://urm.cheryme.top

[R58] 下载文件
来源：http://zwe.kuanghao11.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://iov.ctjpmb.com

[R59] 发 POST JSON
来源：http://wcw.nanxuanxn.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qwq.yj202588.top

[R60] 只看 HTTP 状态码
来源：http://xua.nanxuanxn.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fpx.haohaochexian.top

[R61] 磁盘占用
来源：http://bvm.bjfxy.top

df -h;  du -sh *
来源：http://vee.hesvh.cn

[R62] 找最占空间的文件
来源：http://aro.hammf.cn

du -ah . | sort -rh | head -10
来源：http://aps.aizwys.cn

[R63] 内存与进程
来源：http://gjc.guowangkeji.top

free -h;  ps aux | grep nginx
来源：http://liy.9152youxi.cn

[R64] 结束进程
来源：http://bpm.c1oappe.top

kill -9 $(pgrep -f app.py)
来源：http://kwv.kuanghao11.cn

[R65] 查看端口占用
来源：http://ofz.hcnkem.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://frw.9152youxi.cn

[R66] 定时任务
来源：http://oyz.andypj.xyz

crontab -e;  crontab -l
来源：http://ibs.yj202588.top

[R67] 生成随机十六进制串
来源：http://orj.gaohongyu789.top

openssl rand -hex 16
来源：http://sng.ydzc1.top

[R68] 计算文件校验值
来源：http://cjy.gogol.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xea.yfazqb.com

[R69] 生成随机密码
来源：http://gbr.feifeiyinyue.top

head -c 16 /dev/urandom | base64
来源：http://xuu.cucudq.cn

[R70] 时间戳与互转
来源：http://cph.tianlin.xyz

date +%s;  date -d @1700000000
来源：http://tqr.9152youxi.cn

[R71] 日期格式化
来源：http://bqk.sxryk.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bcc.xuetiantiany.cn

[R72] 等待端口就绪
来源：http://zbg.uphjek.com

until nc -z localhost 3306; do sleep 1; done
来源：http://nqx.kuanghao11.cn

[R73] 分割大日志
来源：http://wvt.yj202588.top

split -l 1000 big.log part_
来源：http://syy.xuetiantiany.cn

[R74] 批量重命名
来源：http://uom.zhongyouzk.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dbg.iojbl.cn

[R75] 导出环境变量
来源：http://oga.nwbrower.top

export PATH="$HOME/bin:$PATH"
来源：http://zoh.bbcook.cn

[R76] 使用临时文件
来源：http://tiy.hfpthk.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pbj.pengpengdd.cyou

[R77] 读取用户输入
来源：http://axb.9152youxi.cn

read -rp "请输入: " ans
来源：http://xen.uphjek.com

[R78] 交互式菜单
来源：http://czx.bjfxy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ubp.hnxiangtu.top

[R79] 解析命令行选项
来源：http://lud.hammf.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://huy.xinyue.icu

[R80] 查看脚本执行耗时
来源：http://xxy.dashuyun.cn

time ./run.sh
来源：http://pdp.yuxming.cn

================================================================================
来源：http://ioh.jinqigfzy.top

S. C / C++ 专题
来源：http://jdj.vqdsnc.cn

================================================================================
来源：http://xni.sjlbkw.cn

[S01] C：Hello World
来源：http://svj.fzhhl.top

#include <stdio.h>
来源：http://ytk.shanyushiyangtech.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://uuo.sufxvd.cn

[S02] C：变量与格式化输出
来源：http://ooz.gaohongyu789.top

int a = 10; printf("%d\n", a);
来源：http://mkq.sxryk.cn

[S03] C：读入整数
来源：http://vxd.yvedp.cn

int x; scanf("%d", &x);
来源：http://eos.c1oappe.top

[S04] C：字符串复制
来源：http://mev.tianlin.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://whd.hcnkem.com

[S05] C：字符串长度
来源：http://fhl.tian-w.cn

strlen(s)
来源：http://nvz.feifeiyinyue.top

[S06] C：字符串比较
来源：http://oyx.shanyushiyangkeji.top

strcmp(a, b) == 0
来源：http://ynu.yj20258.top

[S07] C：数组遍历求和
来源：http://xwu.birdmap.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kzc.jqgfzy.top

[S08] C：动态内存分配与释放
来源：http://azb.fengsongda.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xko.0kj1m.cn

[S09] C：结构体定义与初始化
来源：http://kvk.xuanzx.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oyl.hongshengwenyu.top

[S10] C：指针与解引用
来源：http://cok.cdnleiting.top

int *p = &a;  *p = 5;
来源：http://std.chenlongwang.top

[S11] C：逐行读文件
来源：http://zwp.zhixingplan.top

FILE *f = fopen("a.txt", "r");
来源：http://ghq.ywan-chungtsiang.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://kps.nwbrower.top

fclose(f);
来源：http://bwq.ybcxt.top

[S12] C：写文件
来源：http://tys.zhiwuduotai.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jpc.pycfn.com

[S13] C：宏定义
来源：http://vwi.gogol.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://res.shuidangran.top

[S14] C：枚举
来源：http://wvc.yj202588.top

enum Color { RED, GREEN, BLUE };
来源：http://ylh.hammf.cn

[S15] C：类型转换
来源：http://brm.svipenyu.cn

(double) a / b
来源：http://tjv.sjlbkw.cn

[S16] C：位操作置位
来源：http://eaz.jinyuanbaomall.cn

x |= (1 << 3);
来源：http://cdk.nanxuanxn.top

[S17] C：安全拼接字符串
来源：http://jxt.zdqjudy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lkt.hywenlv.cn

[S18] C：命令行参数
来源：http://yxu.andypj.xyz

int main(int argc, char **argv)
来源：http://ngy.wangdashe.top

[S19] C：快速排序
来源：http://pbw.sysykeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://blk.redwolf501.top

[S20] C：二分查找
来源：http://eax.ivvv.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kxr.hongshengwenyu.top

[S21] C：字符类别判断
来源：http://acd.feifeiyinyue.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qgk.dashuyun.cn

[S22] C：字符串转数字
来源：http://hyl.jinqigfzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://wkw.ppjwa.cn

[S23] C：随机数
来源：http://tpo.svipenyu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nrb.birdmap.top

[S24] C：获取本地时间
来源：http://adt.cashguo.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tba.gogol.net.cn

[S25] C：内存拷贝
来源：http://zpc.tian-w.cn

memcpy(dst, src, n);
来源：http://jqz.shanyushiyangkeji.top

[S26] C：内存清零
来源：http://bbm.xziqi.cn

memset(a, 0, sizeof a);
来源：http://nmv.vehdjk.com

[S27] C：定义常量
来源：http://ayd.jqgufenzy.top

const double PI = 3.14159;
来源：http://qid.yonumen.top

[S28] C：静态变量
来源：http://hty.jqgfzy.top

static int counter = 0;
来源：http://vbf.shanyushiyangkeji.top

[S29] C：变参函数
来源：http://diy.yuxming.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qhr.zhixingplan.top

[S30] C：头文件保护
来源：http://xcg.ydjk.org.cn

#ifndef X_H
来源：http://yfy.sxryk.cn

#define X_H
来源：http://hrb.ctjpmb.com

#endif
来源：http://jig.ydjk.org.cn

[S31] C++：Hello World
来源：http://psi.zhongyouzk.top

#include <iostream>
来源：http://kmg.guannengcc.top

int main() { std::cout << "Hello\n"; }
来源：http://wrz.shzxlz.cn

[S32] C++：字符串
来源：http://tyl.gogol.net.cn

std::string s = "hi";  s += "!";
来源：http://ttp.zhaomingkeji.xyz

[S33] C++：vector 增删
来源：http://kvz.jianghu66.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dna.shangyingyoupin.top

[S34] C++：遍历 vector
来源：http://bfo.jiagoushi.top

for (auto &x : v) { std::cout << x; }
来源：http://aeh.xinyue.icu

[S35] C++：map
来源：http://jrp.bbcook.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zkg.jinghuilouyu.cn

[S36] C++：unordered_map
来源：http://znf.jinyuanbaomall.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nho.jinqigufen.top

[S37] C++：set
来源：http://ihd.cdnleiting.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://guk.zycfv.cn

[S38] C++：排序
来源：http://xco.yfazqb.com

std::sort(v.begin(), v.end());
来源：http://ozl.ydzc1.top

[S39] C++：自定义比较器排序
来源：http://ogi.yfazqb.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xmn.wangshuangyany.cn

[S40] C++：查找元素
来源：http://mjv.hcnkem.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://emo.zhongyouzk.top

[S41] C++：类与构造函数
来源：http://rfp.redwolf501.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://net.xuanzx.com

[S42] C++：继承与虚函数
来源：http://kfe.cheryme.top

class B : public Base { public: void f() override {} };
来源：http://wvf.jinyuanbaomall.cn

[S43] C++：智能指针
来源：http://iic.kuanghao11.cn

auto p = std::make_unique<int>(5);
来源：http://qxn.xinyue.icu

[S44] C++：引用传参
来源：http://hdt.havefunace.top

void inc(int &x) { ++x; }
来源：http://yps.hfpthk.cn

[S45] C++：lambda
来源：http://wxd.yongpay.top

auto add = [](int a, int b) { return a + b; };
来源：http://odb.zdbjq.cn

[S46] C++：函数模板
来源：http://vdj.aizwys.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nkr.tian-w.cn

[S47] C++：结构化绑定遍历
来源：http://lqt.cqqwz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vkq.nanxinkj.top

[S48] C++：逐行读文件
来源：http://znu.guannengcc.top

std::ifstream in("a.txt");  std::string line;
来源：http://ido.aibaodan.cn

while (std::getline(in, line)) { }
来源：http://qqm.sxryk.cn

[S49] C++：写文件
来源：http://nrg.cashguo.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ubq.xuetiantiany.cn

[S50] C++：格式化数字
来源：http://qjg.yvedp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mbj.jinyuanbaomall.cn

[S51] C++：显式类型转换
来源：http://uwo.feifeiyinyue.top

static_cast<double>(a) / b
来源：http://uqn.c1oappe.top

[S52] C++：const 与 noexcept
来源：http://hvc.xylfe.cn

int size() const noexcept { return n_; }
来源：http://pgg.mhx1999.top

[S53] C++：移动语义
来源：http://jgg.hywenlv.cn

std::vector<int> w = std::move(v);
来源：http://yxi.hnqzz.top

[S54] C++：异常处理
来源：http://aqt.cheryme.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://odc.fktsv.cn

[S55] C++：结构化绑定
来源：http://siq.ywan-chungtsiang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ach.uphjek.com

[S56] C++：optional
来源：http://joj.shanyushiyangtech.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bgm.yanxiufei.cn

[S57] C++：编译期常量
来源：http://wmb.ppjwa.cn

constexpr int N = 10;
来源：http://vyt.shanyushiyangkeji.top

[S58] C++：命名空间
来源：http://akc.yuanzhike.top

namespace ns { int f() { return 1; } }
来源：http://cph.zhengqikj.top

[S59] C++：静态断言
来源：http://eqb.0kj1m.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jex.nwbrower.top

[S60] C++：遍历并删除元素
来源：http://nan.shuidangran.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mrg.zhoulong.xyz

================================================================================
来源：http://uoh.svipenyu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rjw.tanke756.top

================================================================================
来源：http://acw.havefunace.top

[T01] Kotlin：Hello World
来源：http://dda.fzhhl.top

println("Hello")
来源：http://qlk.ctjpmb.com

[T02] Kotlin：变量
来源：http://kaa.fzhhl.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yqw.chenlongwang.top

[T03] Kotlin：字符串模板
来源：http://whg.yj202588.top

"值: $b"
来源：http://doj.wangshuangyany.cn

[T04] Kotlin：空安全
来源：http://dwo.fktsv.cn

val n: String? = null;  n?.length
来源：http://blt.pengpengdd.cyou

[T05] Kotlin：when 表达式
来源：http://pbm.uphjek.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tlp.yonumen.top

[T06] Kotlin：集合映射
来源：http://wpi.kuanghao11.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hca.cucudq.cn

[T07] Kotlin：集合过滤
来源：http://uoa.yuanzhike.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://zsm.jqgfzy.top

[T08] Kotlin：数据类
来源：http://wlf.aibaodan.cn

data class User(val name: String, val age: Int)
来源：http://ziz.hongshengwenyu.top

[T09] Kotlin：扩展函数
来源：http://lgf.hcnkem.com

fun String.exclaim() = this + "!"
来源：http://fup.cqqwz.cn

[T10] Kotlin：默认参数
来源：http://ygr.tian-w.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jjg.jinyuanbaomall.cn

[T11] Kotlin：协程
来源：http://zsq.jinghuilouyu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ozm.bjfxy.top

[T12] Kotlin：解构声明
来源：http://qra.fzhhl.top

val (a, b) = Pair(1, 2)
来源：http://hex.9152youxi.cn

[T13] Kotlin：只读 Map
来源：http://fhj.vehdjk.com

val m = mapOf("a" to 1)
来源：http://smh.haohaochexian.top

[T14] Kotlin：循环
来源：http://pyl.tarul.cn

for (i in 1..10) println(i)
来源：http://jcb.fehbvm.com

[T15] Kotlin：接口
来源：http://szz.fktsv.cn

interface Shape { fun area(): Double }
来源：http://itv.xziqi.cn

[T16] Swift：Hello World
来源：http://nzg.shanyushiyangkeji.top

print("Hello")
来源：http://ctw.jiagoushi.top

[T17] Swift：变量与常量
来源：http://odh.tanke756.top

var a = 1;  let b = 2
来源：http://lne.yj20258888.top

[T18] Swift：字符串插值
来源：http://hfh.9152youxi.cn

"值: \(b)"
来源：http://lwt.tanke756.top

[T19] Swift：可选绑定
来源：http://fau.sweek.top

if let n = opt { print(n) }
来源：http://nds.meibo888.top

[T20] Swift：数组操作
来源：http://zqb.ywan-chungtsiang.top

var a = [1, 2, 3];  a.append(4)
来源：http://otk.xinyue.icu


<!-- 参考信息 -->