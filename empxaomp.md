代发 wailian999

echo "${#arr[@]}"
来源：http://qmu.zdqjudy.top

[R20] 关联数组（字典）
来源：http://hxn.hysaishi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oex.xziqi.cn

[R21] 字符串长度
来源：http://urd.hongshengwenyu.top

echo "${#s}"
来源：http://yks.andypj.xyz

[R22] 截取子串
来源：http://cqo.wangdashe.top

echo "${s:0:5}"
来源：http://krf.daxiang520.top

[R23] 字符串替换
来源：http://grq.fktsv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fan.zhengqikj.top

[R24] 大小写转换
来源：http://fwj.jianghu66.top

echo "${s^^}"; echo "${s,,}"
来源：http://kzf.dashuyun.cn

[R25] 去后缀 / 去前缀
来源：http://pks.jyoumei.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rhz.smart0.xyz

[R26] 命令替换
来源：http://suo.svipenyu.cn

now=$(date +%F); echo "$now"
来源：http://iuh.dashuyun.cn

[R27] 算术展开
来源：http://zza.tanke756.top

echo $((1 + 2 * 3))
来源：http://fea.ydjk.org.cn

[R28] 浮点运算
来源：http://cad.wangshuangyany.cn

echo "scale=2; 10/3" | bc
来源：http://fbi.hammf.cn

[R29] 定义函数
来源：http://ygr.yj20258.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zxl.cheryme.top

[R30] 函数返回状态码
来源：http://ucd.nanxinkj.top

f() { return 0; }; f || echo "失败了"
来源：http://way.shzxlz.cn

[R31] 局部变量
来源：http://row.hnxiangtu.top

f() { local x=1; echo "$x"; }
来源：http://sxs.yj20258.top

[R32] 参数个数校验
来源：http://tyl.ctjpmb.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jkp.fehbvm.com

[R33] 捕获错误并提示行号
来源：http://wqm.ppjwa.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mvv.yj20258.top

[R34] 退出时清理
来源：http://sut.sufxvd.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nxh.yuxming.cn

[R35] 后台执行并等待
来源：http://mna.kuanghao11.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wot.chenlongwang.top

[R36] 并发执行多个任务
来源：http://mhb.nwbrower.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gdi.aizwys.cn

[R37] 把输出赋给变量
来源：http://yte.ydzc1.top

files=$(ls -1)
来源：http://irr.shanyushiyangkeji.top

[R38] 管道串联
来源：http://hdz.yuxming.cn

cat a.txt | grep -i error | wc -l
来源：http://vxg.yfazqb.com

[R39] 重定向标准输出与错误
来源：http://hfo.jlsjyb.cn

cmd > out.log 2>&1
来源：http://nua.chenzaomai.com

[R40] 追加写日志
来源：http://sod.uphjek.com

echo "log" >> out.log
来源：http://brm.shzxlz.cn

[R41] 丢弃输出
来源：http://wvq.ydzc1.top

cmd >/dev/null 2>&1
来源：http://yvc.mhx1999.top

[R42] 输入重定向
来源：http://cbp.chenlongwang.top

wc -l < a.txt
来源：http://pyx.guowangkeji.top

[R43] 按名字查找文件
来源：http://hja.fktsv.cn

find . -name "*.log" -type f
来源：http://rwa.xziqi.cn

[R44] 按修改时间查找
来源：http://nfw.yuxming.cn

find . -mtime -7 -type f
来源：http://paf.chenzaomai.com

[R45] 批量删除
来源：http://myf.jianghu66.top

find . -name "*.tmp" -delete
来源：http://bqg.zdqjudy.top

[R46] 递归替换文件内容
来源：http://srb.hesvh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://msk.yanxiufei.cn

[R47] sed 单行替换
来源：http://tuk.chenjidiqi.icu

sed -i 's/foo/bar/g' a.txt
来源：http://rcj.yj20258888.top

[R48] awk 取指定列
来源：http://bth.dashuyun.cn

awk '{print $1, $3}' a.txt
来源：http://ejb.bbcook.cn

[R49] awk 带条件
来源：http://win.cheryme.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://azr.xuetiantiany.cn

[R50] awk 求和
来源：http://euh.ivvv.top

awk '{s += $2} END {print s}' a.txt
来源：http://bdq.jinqigfzy.top

[R51] 排序去重取前几
来源：http://usf.hywenlv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vtn.yueranfly.top

[R52] 统计行数
来源：http://jhx.jinqigfzy.top

wc -l a.txt
来源：http://nul.zdbjq.cn

[R53] 查看文件头与实时尾
来源：http://wyi.fanxiaobao.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cvb.ivvv.top

[R54] 比较两个文件
来源：http://kow.hammf.cn

diff a.txt b.txt
来源：http://xks.ctjpmb.com

[R55] 压缩与解压
来源：http://hyl.tian-w.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yaj.fktsv.cn

[R56] 远程拷贝
来源：http://khw.52xcode.cn

scp file user@host:/path/
来源：http://jam.iojbl.cn

[R57] 远程执行命令
来源：http://qkp.ydzc1.top

ssh user@host 'uptime'
来源：http://grf.xuanzx.com

[R58] 下载文件
来源：http://smc.yj20258888.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pfb.xingfuxueyuan.xyz

[R59] 发 POST JSON
来源：http://tmi.tian-w.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ojl.xingfuxueyuan.xyz

[R60] 只看 HTTP 状态码
来源：http://erl.hammf.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mce.pengpengdd.cyou

[R61] 磁盘占用
来源：http://zat.ywan-chungtsiang.top

df -h;  du -sh *
来源：http://rlg.sufxvd.cn

[R62] 找最占空间的文件
来源：http://lld.cashguo.top

du -ah . | sort -rh | head -10
来源：http://zaw.nanxuanxn.top

[R63] 内存与进程
来源：http://ahc.redwolf501.top

free -h;  ps aux | grep nginx
来源：http://zhb.chenlongwang.top

[R64] 结束进程
来源：http://vkl.fanxiaobao.xyz

kill -9 $(pgrep -f app.py)
来源：http://zep.jinghuilouyu.cn

[R65] 查看端口占用
来源：http://mmm.sufxvd.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zih.shanyushiyangtech.top

[R66] 定时任务
来源：http://txy.zhixingplan.top

crontab -e;  crontab -l
来源：http://fvd.sweek.top

[R67] 生成随机十六进制串
来源：http://ivs.316326.xyz

openssl rand -hex 16
来源：http://asv.mhx1999.top

[R68] 计算文件校验值
来源：http://ogg.meibo888.top

sha256sum a.txt;  md5sum a.txt
来源：http://rnu.nanxinkj.top

[R69] 生成随机密码
来源：http://pzc.yfazqb.com

head -c 16 /dev/urandom | base64
来源：http://uss.aibaodan.cn

[R70] 时间戳与互转
来源：http://ldw.316326.xyz

date +%s;  date -d @1700000000
来源：http://omg.dianchejie.cn

[R71] 日期格式化
来源：http://eum.jinghuilouyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fgp.shangyingyoupin.top

[R72] 等待端口就绪
来源：http://uyj.jiagoushi.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ylh.hcnkem.com

[R73] 分割大日志
来源：http://ycz.shzxlz.cn

split -l 1000 big.log part_
来源：http://xac.wangdashe.top

[R74] 批量重命名
来源：http://gln.yongpay.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ead.mhx1999.top

[R75] 导出环境变量
来源：http://ilk.cqqwz.cn

export PATH="$HOME/bin:$PATH"
来源：http://ula.yj20258888.top

[R76] 使用临时文件
来源：http://sdo.zycfv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wmt.xuetiantiany.cn

[R77] 读取用户输入
来源：http://aro.hammf.cn

read -rp "请输入: " ans
来源：http://kzp.nanxuanxn.top

[R78] 交互式菜单
来源：http://iiw.jqgufenzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rmu.birdmap.top

[R79] 解析命令行选项
来源：http://wvh.jqgfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dzf.jianghu66.top

[R80] 查看脚本执行耗时
来源：http://upe.shanyushiyangtech.top

time ./run.sh
来源：http://mky.gaohongyu789.top

================================================================================
来源：http://uzm.hnqzz.top

S. C / C++ 专题
来源：http://hup.uphjek.com

================================================================================
来源：http://jab.ywan-chungtsiang.top

[S01] C：Hello World
来源：http://ifm.gzhubu.top

#include <stdio.h>
来源：http://kkx.nanxuanxn.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ypp.havefunace.top

[S02] C：变量与格式化输出
来源：http://ybj.pycfn.com

int a = 10; printf("%d\n", a);
来源：http://vlj.xuanzx.com

[S03] C：读入整数
来源：http://xna.jinqigufen.top

int x; scanf("%d", &x);
来源：http://omz.pycfn.com

[S04] C：字符串复制
来源：http://qoi.sufxvd.cn

char dst[32]; strcpy(dst, "hi");
来源：http://smu.meibo888.top

[S05] C：字符串长度
来源：http://vir.fanxiaobao.xyz

strlen(s)
来源：http://grk.chenjidiqi.icu

[S06] C：字符串比较
来源：http://ydi.jianghu66.top

strcmp(a, b) == 0
来源：http://fak.chenjidiqi.icu

[S07] C：数组遍历求和
来源：http://sgb.chenzaomai.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ham.kuanghao11.cn

[S08] C：动态内存分配与释放
来源：http://wii.sufxvd.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jso.sweek.top

[S09] C：结构体定义与初始化
来源：http://kvc.tanke756.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://umc.uphjek.com

[S10] C：指针与解引用
来源：http://ytl.guannengcc.top

int *p = &a;  *p = 5;
来源：http://drz.daxiang520.top

[S11] C：逐行读文件
来源：http://plg.zycfv.cn

FILE *f = fopen("a.txt", "r");
来源：http://tci.shanyushiyangtech.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vah.hnxiangtu.top

fclose(f);
来源：http://htj.ydzc1.top

[S12] C：写文件
来源：http://ztg.0kj1m.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bgt.hammf.cn

[S13] C：宏定义
来源：http://uzk.yuanzhike.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://drk.316326.xyz

[S14] C：枚举
来源：http://kkf.yanxiufei.cn

enum Color { RED, GREEN, BLUE };
来源：http://tnk.jinghuilouyu.cn

[S15] C：类型转换
来源：http://kwf.hnxiangtu.top

(double) a / b
来源：http://egv.wangdashe.top

[S16] C：位操作置位
来源：http://ikk.cdnleiting.top

x |= (1 << 3);
来源：http://iyn.dianchejie.cn

[S17] C：安全拼接字符串
来源：http://upc.aizwys.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xjg.tarul.cn

[S18] C：命令行参数
来源：http://viu.jianghu66.top

int main(int argc, char **argv)
来源：http://lcn.cdnleiting.top

[S19] C：快速排序
来源：http://ypz.ydjk.org.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gio.ywan-chungtsiang.top

[S20] C：二分查找
来源：http://sta.zhijiandao.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://doe.shuidangran.top

[S21] C：字符类别判断
来源：http://bco.shanyushiyangkeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rbt.xingfuxueyuan.xyz

[S22] C：字符串转数字
来源：http://xnm.ctjpmb.com

atoi("42");  strtod("3.14", NULL);
来源：http://ltn.yanxiufei.cn

[S23] C：随机数
来源：http://qul.aibaodan.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rou.jianghu66.top

[S24] C：获取本地时间
来源：http://zag.yuxming.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://epf.pengpengdd.cyou

[S25] C：内存拷贝
来源：http://rzf.sxryk.cn

memcpy(dst, src, n);
来源：http://djb.xuetiantiany.cn

[S26] C：内存清零
来源：http://nsd.epnwcf.com

memset(a, 0, sizeof a);
来源：http://lpq.epnwcf.com

[S27] C：定义常量
来源：http://flr.iojbl.cn

const double PI = 3.14159;
来源：http://sph.fanxiaobao.xyz

[S28] C：静态变量
来源：http://jmb.dianchejie.cn

static int counter = 0;
来源：http://gxw.jiagoushi.top

[S29] C：变参函数
来源：http://xix.feifeiyinyue.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rrb.yvedp.cn

[S30] C：头文件保护
来源：http://wga.ydzc1.top

#ifndef X_H
来源：http://dep.cashguo.top

#define X_H
来源：http://ioc.sxryk.cn

#endif
来源：http://wcs.jinqigfzy.top

[S31] C++：Hello World
来源：http://qxw.epnwcf.com

#include <iostream>
来源：http://uyt.jqgufenzy.top

int main() { std::cout << "Hello\n"; }
来源：http://vlf.52xcode.cn

[S32] C++：字符串
来源：http://uya.hongshengwenyu.top

std::string s = "hi";  s += "!";
来源：http://iok.fanxiaobao.xyz

[S33] C++：vector 增删
来源：http://cdv.cashguo.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zdw.daxiang520.top

[S34] C++：遍历 vector
来源：http://ivl.gaohongyu789.top

for (auto &x : v) { std::cout << x; }
来源：http://ply.xinyue.icu

[S35] C++：map
来源：http://pgo.yueranfly.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nyd.jqgfzy.top

[S36] C++：unordered_map
来源：http://qlb.ctjpmb.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mlb.xingfuxueyuan.xyz

[S37] C++：set
来源：http://xto.haohaochexian.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rfa.shanyushiyangtech.top

[S38] C++：排序
来源：http://xcs.yfazqb.com

std::sort(v.begin(), v.end());
来源：http://xvu.andypj.xyz

[S39] C++：自定义比较器排序
来源：http://nks.cheryme.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xee.yvedp.cn

[S40] C++：查找元素
来源：http://kgf.yj20258.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lsu.haohaochexian.top

[S41] C++：类与构造函数
来源：http://bkx.jinyuanbaomall.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nhl.cheryme.top

[S42] C++：继承与虚函数
来源：http://aly.jianghu66.top

class B : public Base { public: void f() override {} };
来源：http://xhv.fengsongda.top

[S43] C++：智能指针
来源：http://byu.ydzc1.top

auto p = std::make_unique<int>(5);
来源：http://stp.9152youxi.cn

[S44] C++：引用传参
来源：http://oiq.xuetiantiany.cn

void inc(int &x) { ++x; }
来源：http://zzn.feifeiyinyue.top

[S45] C++：lambda
来源：http://wka.ybcxt.top

auto add = [](int a, int b) { return a + b; };
来源：http://hcn.smart0.xyz

[S46] C++：函数模板
来源：http://usl.redwolf501.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cal.tian-w.cn

[S47] C++：结构化绑定遍历
来源：http://qfa.cdnleiting.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vhb.hammf.cn

[S48] C++：逐行读文件
来源：http://puo.wangshuangyany.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ioh.tian-w.cn

while (std::getline(in, line)) { }
来源：http://xcv.ydjk.org.cn

[S49] C++：写文件
来源：http://hsd.yueranfly.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://flm.zhoulong.xyz

[S50] C++：格式化数字
来源：http://xcv.yfazqb.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tbz.yfazqb.com

[S51] C++：显式类型转换
来源：http://joy.fzhhl.top

static_cast<double>(a) / b
来源：http://ztb.pengpengdd.cyou

[S52] C++：const 与 noexcept
来源：http://cls.redwolf501.top

int size() const noexcept { return n_; }
来源：http://adx.xylfe.cn

[S53] C++：移动语义
来源：http://fvj.yj20258888.top

std::vector<int> w = std::move(v);
来源：http://tbg.hnxiangtu.top

[S54] C++：异常处理
来源：http://vnl.cdnleiting.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ooa.sysykeji.top

[S55] C++：结构化绑定
来源：http://pri.yueranfly.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jzh.quarkkingdee.top

[S56] C++：optional
来源：http://uuc.fktsv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iyp.zhaomingkeji.xyz

[S57] C++：编译期常量
来源：http://mxh.meibo888.top

constexpr int N = 10;
来源：http://gzf.sjlbkw.cn

[S58] C++：命名空间
来源：http://dnb.52xcode.cn

namespace ns { int f() { return 1; } }
来源：http://zro.52xcode.cn

[S59] C++：静态断言
来源：http://pkd.snrcjt.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mlu.jinqigfzy.top

[S60] C++：遍历并删除元素
来源：http://ybl.guowangkeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nqr.daxiang520.top

================================================================================
来源：http://ecj.quarkkingdee.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lyy.xingfuxueyuan.xyz

================================================================================
来源：http://szm.cucudq.cn

[T01] Kotlin：Hello World
来源：http://kwu.xinyue.icu

println("Hello")
来源：http://wuw.bbcook.cn

[T02] Kotlin：变量
来源：http://nlh.birdmap.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lzb.havefunace.top

[T03] Kotlin：字符串模板
来源：http://cgt.pengpengdd.cyou

"值: $b"
来源：http://kct.yfazqb.com

[T04] Kotlin：空安全
来源：http://dnu.hongshengwenyu.top

val n: String? = null;  n?.length
来源：http://qzv.shuidangran.top

[T05] Kotlin：when 表达式
来源：http://eyp.yj20258888.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://woi.yanxiufei.cn

[T06] Kotlin：集合映射
来源：http://vqk.cdnleiting.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rlg.cdnleiting.top

[T07] Kotlin：集合过滤
来源：http://ytz.hammf.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zcl.yfazqb.com

[T08] Kotlin：数据类
来源：http://dic.jinqigufen.top

data class User(val name: String, val age: Int)
来源：http://eqf.hfpthk.cn

[T09] Kotlin：扩展函数
来源：http://ekc.yj202588.top

fun String.exclaim() = this + "!"
来源：http://ufi.jinyuanbaomall.cn

[T10] Kotlin：默认参数
来源：http://qyv.sysykeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ayf.feifeiyinyue.top

[T11] Kotlin：协程
来源：http://dfx.vqdsnc.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wxr.snrcjt.cn

[T12] Kotlin：解构声明
来源：http://kje.wangshuangyany.cn

val (a, b) = Pair(1, 2)
来源：http://jyh.snrcjt.cn

[T13] Kotlin：只读 Map
来源：http://cbc.vehdjk.com

val m = mapOf("a" to 1)
来源：http://oeb.wangshuangyany.cn

[T14] Kotlin：循环
来源：http://qaw.dashuyun.cn

for (i in 1..10) println(i)
来源：http://mfa.andypj.xyz

[T15] Kotlin：接口
来源：http://bbl.haohaochexian.top

interface Shape { fun area(): Double }
来源：http://qvg.zhongyouzk.top

[T16] Swift：Hello World
来源：http://tlo.zycfv.cn

print("Hello")
来源：http://dor.fengsongda.top

[T17] Swift：变量与常量
来源：http://wys.jqgufenzy.top

var a = 1;  let b = 2
来源：http://nby.zhaomingkeji.xyz

[T18] Swift：字符串插值
来源：http://tpq.bbcook.cn

"值: \(b)"
来源：http://xlz.gaohongyu789.top

[T19] Swift：可选绑定
来源：http://khe.shuidangran.top

if let n = opt { print(n) }
来源：http://mfy.zhengqikj.top

[T20] Swift：数组操作
来源：http://ond.xuetiantiany.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nag.ydzc1.top

[T21] Swift：遍历
来源：http://fll.iojbl.cn

for x in a { print(x) }
来源：http://kbm.zhoulong.xyz

[T22] Swift：字典
来源：http://dwh.iojbl.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ysj.quarkkingdee.top


<!-- 参考信息 -->