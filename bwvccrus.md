代发 wailian999

echo "${#arr[@]}"
来源：http://hmw.zhengqikj.top

[R20] 关联数组（字典）
来源：http://uuj.xinyue.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hlp.gzhubu.top

[R21] 字符串长度
来源：http://kqc.fzhhl.top

echo "${#s}"
来源：http://dhf.wangdashe.top

[R22] 截取子串
来源：http://vxg.zdqjudy.top

echo "${s:0:5}"
来源：http://xka.tian-w.cn

[R23] 字符串替换
来源：http://yfv.ppjwa.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qyt.ppjwa.cn

[R24] 大小写转换
来源：http://ztc.zdqjudy.top

echo "${s^^}"; echo "${s,,}"
来源：http://vcu.wangdashe.top

[R25] 去后缀 / 去前缀
来源：http://ubc.yj20258888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://jsf.shanyushiyangkeji.top

[R26] 命令替换
来源：http://vyg.ehwqpu.com

now=$(date +%F); echo "$now"
来源：http://icx.ywan-chungtsiang.top

[R27] 算术展开
来源：http://qan.cheryme.top

echo $((1 + 2 * 3))
来源：http://rtn.hcnkem.com

[R28] 浮点运算
来源：http://tzv.wangdashe.top

echo "scale=2; 10/3" | bc
来源：http://kvu.zhixingplan.top

[R29] 定义函数
来源：http://ewj.yj20258888.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sxn.hongshengwenyu.top

[R30] 函数返回状态码
来源：http://gcl.shanyushiyangtech.top

f() { return 0; }; f || echo "失败了"
来源：http://pnt.zhiwuduotai.top

[R31] 局部变量
来源：http://iim.tanke756.top

f() { local x=1; echo "$x"; }
来源：http://kso.andypj.xyz

[R32] 参数个数校验
来源：http://fpj.nwbrower.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kqm.zhongyouzk.top

[R33] 捕获错误并提示行号
来源：http://pyi.ctjpmb.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lbp.ppjwa.cn

[R34] 退出时清理
来源：http://hdx.wangdashe.top

trap 'rm -f "$tmp"' EXIT
来源：http://nuv.jlsjyb.cn

[R35] 后台执行并等待
来源：http://tgy.tian-w.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gpc.yanxiufei.cn

[R36] 并发执行多个任务
来源：http://gdb.jyoumei.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hyx.dianchejie.cn

[R37] 把输出赋给变量
来源：http://zho.cqqwz.cn

files=$(ls -1)
来源：http://yte.jinqigufen.top

[R38] 管道串联
来源：http://wfw.redwolf501.top

cat a.txt | grep -i error | wc -l
来源：http://tor.vqdsnc.cn

[R39] 重定向标准输出与错误
来源：http://ldg.nwbrower.top

cmd > out.log 2>&1
来源：http://jme.shzxlz.cn

[R40] 追加写日志
来源：http://xaw.fktsv.cn

echo "log" >> out.log
来源：http://uos.xinyue.icu

[R41] 丢弃输出
来源：http://pww.yfazqb.com

cmd >/dev/null 2>&1
来源：http://rvy.tian-w.cn

[R42] 输入重定向
来源：http://qsl.ppjwa.cn

wc -l < a.txt
来源：http://fzk.havefunace.top

[R43] 按名字查找文件
来源：http://vtv.yfazqb.com

find . -name "*.log" -type f
来源：http://yys.haohaochexian.top

[R44] 按修改时间查找
来源：http://djm.xziqi.cn

find . -mtime -7 -type f
来源：http://cvf.hywenlv.cn

[R45] 批量删除
来源：http://vpw.dashuyun.cn

find . -name "*.tmp" -delete
来源：http://krc.ppjwa.cn

[R46] 递归替换文件内容
来源：http://mjh.ivvv.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://osa.daxiang520.top

[R47] sed 单行替换
来源：http://irv.hywenlv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rlb.dianchejie.cn

[R48] awk 取指定列
来源：http://ynn.shzxlz.cn

awk '{print $1, $3}' a.txt
来源：http://iig.sufxvd.cn

[R49] awk 带条件
来源：http://khu.xuetiantiany.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mxn.gzhubu.top

[R50] awk 求和
来源：http://ntn.yj20258888.top

awk '{s += $2} END {print s}' a.txt
来源：http://eys.ywan-chungtsiang.top

[R51] 排序去重取前几
来源：http://drf.bjfxy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://eko.ppjwa.cn

[R52] 统计行数
来源：http://vky.yvedp.cn

wc -l a.txt
来源：http://csg.jqgufenzy.top

[R53] 查看文件头与实时尾
来源：http://vmp.ybcxt.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://stj.wangshuangyany.cn

[R54] 比较两个文件
来源：http://yrn.yj20258888.top

diff a.txt b.txt
来源：http://xxv.dashuyun.cn

[R55] 压缩与解压
来源：http://mhr.shuidangran.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kfs.haohaochexian.top

[R56] 远程拷贝
来源：http://cle.hnxiangtu.top

scp file user@host:/path/
来源：http://pvd.mhx1999.top

[R57] 远程执行命令
来源：http://ots.shanyushiyangtech.top

ssh user@host 'uptime'
来源：http://cxe.yfazqb.com

[R58] 下载文件
来源：http://rnr.gaohongyu789.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nfp.zhijiandao.cn

[R59] 发 POST JSON
来源：http://pud.jyoumei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mlw.yj20258.top

[R60] 只看 HTTP 状态码
来源：http://vrz.vqdsnc.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jpr.jqgfzy.top

[R61] 磁盘占用
来源：http://eae.zdqjudy.top

df -h;  du -sh *
来源：http://jhc.ivvv.top

[R62] 找最占空间的文件
来源：http://owq.jlsjyb.cn

du -ah . | sort -rh | head -10
来源：http://zzm.fehbvm.com

[R63] 内存与进程
来源：http://cup.redwolf501.top

free -h;  ps aux | grep nginx
来源：http://mjx.0kj1m.cn

[R64] 结束进程
来源：http://mpp.fehbvm.com

kill -9 $(pgrep -f app.py)
来源：http://uey.chenlongwang.top

[R65] 查看端口占用
来源：http://cvv.ywan-chungtsiang.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rhu.zycfv.cn

[R66] 定时任务
来源：http://iuu.ydzc1.top

crontab -e;  crontab -l
来源：http://tzd.fzhhl.top

[R67] 生成随机十六进制串
来源：http://ruw.sxryk.cn

openssl rand -hex 16
来源：http://ped.hammf.cn

[R68] 计算文件校验值
来源：http://jvj.bjfxy.top

sha256sum a.txt;  md5sum a.txt
来源：http://dbh.xinyue.icu

[R69] 生成随机密码
来源：http://dro.hywenlv.cn

head -c 16 /dev/urandom | base64
来源：http://zri.hammf.cn

[R70] 时间戳与互转
来源：http://zhh.hywenlv.cn

date +%s;  date -d @1700000000
来源：http://tip.zhaomingkeji.xyz

[R71] 日期格式化
来源：http://utw.birdmap.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bzg.chenjidiqi.icu

[R72] 等待端口就绪
来源：http://ecx.meibo888.top

until nc -z localhost 3306; do sleep 1; done
来源：http://vrx.zhongyouzk.top

[R73] 分割大日志
来源：http://qxr.redwolf501.top

split -l 1000 big.log part_
来源：http://bmw.hfpthk.cn

[R74] 批量重命名
来源：http://sdu.bbcook.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ysv.jinqigfzy.top

[R75] 导出环境变量
来源：http://xus.tian-w.cn

export PATH="$HOME/bin:$PATH"
来源：http://vqn.jlsjyb.cn

[R76] 使用临时文件
来源：http://vtb.hesvh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tnb.tanke756.top

[R77] 读取用户输入
来源：http://tln.birdmap.top

read -rp "请输入: " ans
来源：http://bog.chenlongwang.top

[R78] 交互式菜单
来源：http://igi.yj20258.top

select opt in a b c; do echo "$opt"; break; done
来源：http://kua.shanyushiyangtech.top

[R79] 解析命令行选项
来源：http://cif.bbcook.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vlk.daxiang520.top

[R80] 查看脚本执行耗时
来源：http://oor.cheryme.top

time ./run.sh
来源：http://lyn.ydjk.org.cn

================================================================================
来源：http://juf.yuanzhike.top

S. C / C++ 专题
来源：http://yzz.yj202588.top

================================================================================
来源：http://acb.nanxinkj.top

[S01] C：Hello World
来源：http://aft.sufxvd.cn

#include <stdio.h>
来源：http://wvq.quarkkingdee.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://lhp.feifeiyinyue.top

[S02] C：变量与格式化输出
来源：http://wve.sufxvd.cn

int a = 10; printf("%d\n", a);
来源：http://ayw.tianlin.xyz

[S03] C：读入整数
来源：http://pjf.jinyuanbaomall.cn

int x; scanf("%d", &x);
来源：http://iqu.nwbrower.top

[S04] C：字符串复制
来源：http://niy.ydzc1.top

char dst[32]; strcpy(dst, "hi");
来源：http://hat.9152youxi.cn

[S05] C：字符串长度
来源：http://rae.feifeiyinyue.top

strlen(s)
来源：http://jpp.ivvv.top

[S06] C：字符串比较
来源：http://due.yj20258.top

strcmp(a, b) == 0
来源：http://yoa.shangyingyoupin.top

[S07] C：数组遍历求和
来源：http://ifi.chenjidiqi.icu

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mks.shangyingyoupin.top

[S08] C：动态内存分配与释放
来源：http://nya.tianlin.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://etw.zhiwuduotai.top

[S09] C：结构体定义与初始化
来源：http://xnc.52xcode.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ivr.jqgufenzy.top

[S10] C：指针与解引用
来源：http://ich.zhongyouzk.top

int *p = &a;  *p = 5;
来源：http://yqk.xziqi.cn

[S11] C：逐行读文件
来源：http://lep.feifeiyinyue.top

FILE *f = fopen("a.txt", "r");
来源：http://gxa.xuetiantiany.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lrc.jqgfzy.top

fclose(f);
来源：http://xgj.uphjek.com

[S12] C：写文件
来源：http://zkq.ppjwa.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nxf.zycfv.cn

[S13] C：宏定义
来源：http://qjs.nwbrower.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lzz.0kj1m.cn

[S14] C：枚举
来源：http://ycz.yonumen.top

enum Color { RED, GREEN, BLUE };
来源：http://wqx.jinghuilouyu.cn

[S15] C：类型转换
来源：http://kow.hcnkem.com

(double) a / b
来源：http://amc.quarkkingdee.top

[S16] C：位操作置位
来源：http://bly.tianlin.xyz

x |= (1 << 3);
来源：http://xpe.sysykeji.top

[S17] C：安全拼接字符串
来源：http://zlj.vehdjk.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://aqx.cqqwz.cn

[S18] C：命令行参数
来源：http://fyo.tianlin.xyz

int main(int argc, char **argv)
来源：http://cfb.xylfe.cn

[S19] C：快速排序
来源：http://tbe.redwolf501.top

qsort(a, n, sizeof(int), cmp);
来源：http://vjt.jyoumei.cn

[S20] C：二分查找
来源：http://djw.xuetiantiany.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qbk.shangyingyoupin.top

[S21] C：字符类别判断
来源：http://luj.zhixingplan.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xxz.cucudq.cn

[S22] C：字符串转数字
来源：http://slw.ehwqpu.com

atoi("42");  strtod("3.14", NULL);
来源：http://rdz.hesvh.cn

[S23] C：随机数
来源：http://rst.xuetiantiany.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qhy.yongpay.top

[S24] C：获取本地时间
来源：http://zta.wangdashe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fwi.xziqi.cn

[S25] C：内存拷贝
来源：http://gbz.nanxuanxn.top

memcpy(dst, src, n);
来源：http://bib.iojbl.cn

[S26] C：内存清零
来源：http://ryf.hywenlv.cn

memset(a, 0, sizeof a);
来源：http://aqs.iojbl.cn

[S27] C：定义常量
来源：http://aqe.nwbrower.top

const double PI = 3.14159;
来源：http://hvk.jlsjyb.cn

[S28] C：静态变量
来源：http://nde.nanxinkj.top

static int counter = 0;
来源：http://qzq.daxiang520.top

[S29] C：变参函数
来源：http://vpn.fanxiaobao.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vkq.smart0.xyz

[S30] C：头文件保护
来源：http://mka.redwolf501.top

#ifndef X_H
来源：http://gpj.ydzc1.top

#define X_H
来源：http://syq.pycfn.com

#endif
来源：http://bfv.hnxiangtu.top

[S31] C++：Hello World
来源：http://yhr.sufxvd.cn

#include <iostream>
来源：http://cme.sysykeji.top

int main() { std::cout << "Hello\n"; }
来源：http://lge.xuetiantiany.cn

[S32] C++：字符串
来源：http://zbg.ctjpmb.com

std::string s = "hi";  s += "!";
来源：http://oic.birdmap.top

[S33] C++：vector 增删
来源：http://xra.pycfn.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lve.jianghu66.top

[S34] C++：遍历 vector
来源：http://qhw.aizwys.cn

for (auto &x : v) { std::cout << x; }
来源：http://weh.xylfe.cn

[S35] C++：map
来源：http://yen.zhiwuduotai.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sox.cucudq.cn

[S36] C++：unordered_map
来源：http://eki.kuanghao11.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mey.ywan-chungtsiang.top

[S37] C++：set
来源：http://ujw.hfpthk.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mql.c1oappe.top

[S38] C++：排序
来源：http://mjs.zhijiandao.cn

std::sort(v.begin(), v.end());
来源：http://ktq.ydzc1.top

[S39] C++：自定义比较器排序
来源：http://iim.nanxuanxn.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dln.uphjek.com

[S40] C++：查找元素
来源：http://wyg.cashguo.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bpz.cqqwz.cn

[S41] C++：类与构造函数
来源：http://cgl.jlsjyb.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rwk.yonumen.top

[S42] C++：继承与虚函数
来源：http://yto.nanxuanxn.top

class B : public Base { public: void f() override {} };
来源：http://kbu.gzhubu.top

[S43] C++：智能指针
来源：http://elv.ywan-chungtsiang.top

auto p = std::make_unique<int>(5);
来源：http://kgp.gotoacloud.top

[S44] C++：引用传参
来源：http://tlg.uphjek.com

void inc(int &x) { ++x; }
来源：http://ekr.haohaochexian.top

[S45] C++：lambda
来源：http://fgg.shangyingyoupin.top

auto add = [](int a, int b) { return a + b; };
来源：http://uii.gaohongyu789.top

[S46] C++：函数模板
来源：http://baf.zhijiandao.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uls.9152youxi.cn

[S47] C++：结构化绑定遍历
来源：http://bmq.hammf.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zyc.mhx1999.top

[S48] C++：逐行读文件
来源：http://yon.shanyushiyangkeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://jon.hnxiangtu.top

while (std::getline(in, line)) { }
来源：http://bqa.xinyue.icu

[S49] C++：写文件
来源：http://vrc.jqgfzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dap.xziqi.cn

[S50] C++：格式化数字
来源：http://vzs.andypj.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jti.vehdjk.com

[S51] C++：显式类型转换
来源：http://qsz.bbcook.cn

static_cast<double>(a) / b
来源：http://van.ehwqpu.com

[S52] C++：const 与 noexcept
来源：http://auc.gzhubu.top

int size() const noexcept { return n_; }
来源：http://upv.hfpthk.cn

[S53] C++：移动语义
来源：http://ztg.316326.xyz

std::vector<int> w = std::move(v);
来源：http://tsb.316326.xyz

[S54] C++：异常处理
来源：http://enn.hywenlv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gwz.daxiang520.top

[S55] C++：结构化绑定
来源：http://mrf.birdmap.top

auto [a, b] = std::make_pair(1, 2);
来源：http://frx.chenjidiqi.icu

[S56] C++：optional
来源：http://ojj.fktsv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://otq.shangyingyoupin.top

[S57] C++：编译期常量
来源：http://snt.xuetiantiany.cn

constexpr int N = 10;
来源：http://oim.shanyushiyangtech.top

[S58] C++：命名空间
来源：http://fws.52xcode.cn

namespace ns { int f() { return 1; } }
来源：http://azh.jinyuanbaomall.cn

[S59] C++：静态断言
来源：http://jox.guowangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nme.wangshuangyany.cn

[S60] C++：遍历并删除元素
来源：http://kjy.xziqi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nra.sxryk.cn

================================================================================
来源：http://bne.chenzaomai.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://teu.yj20258888.top

================================================================================
来源：http://sny.wangdashe.top

[T01] Kotlin：Hello World
来源：http://hul.quarkkingdee.top

println("Hello")
来源：http://ixu.kuanghao11.cn

[T02] Kotlin：变量
来源：http://dgm.zhiwuduotai.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qbp.ydzc1.top

[T03] Kotlin：字符串模板
来源：http://sea.hfpthk.cn

"值: $b"
来源：http://mmh.kuanghao11.cn

[T04] Kotlin：空安全
来源：http://wmi.fktsv.cn

val n: String? = null;  n?.length
来源：http://cvu.yfazqb.com

[T05] Kotlin：when 表达式
来源：http://bse.birdmap.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://adx.zhiwuduotai.top

[T06] Kotlin：集合映射
来源：http://dda.xylfe.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tyz.kuanghao11.cn

[T07] Kotlin：集合过滤
来源：http://dys.hfpthk.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lzg.fzhhl.top

[T08] Kotlin：数据类
来源：http://ane.xingfuxueyuan.xyz

data class User(val name: String, val age: Int)
来源：http://nde.xinyue.icu

[T09] Kotlin：扩展函数
来源：http://kbp.xinyue.icu

fun String.exclaim() = this + "!"
来源：http://vmn.wangshuangyany.cn

[T10] Kotlin：默认参数
来源：http://mkl.hongshengwenyu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://lzd.ehwqpu.com

[T11] Kotlin：协程
来源：http://zat.aibaodan.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gyh.yuxming.cn

[T12] Kotlin：解构声明
来源：http://osu.gzhubu.top

val (a, b) = Pair(1, 2)
来源：http://kds.daxiang520.top

[T13] Kotlin：只读 Map
来源：http://ogn.uphjek.com

val m = mapOf("a" to 1)
来源：http://jvi.jqgfzy.top

[T14] Kotlin：循环
来源：http://uef.yangfankeji.com

for (i in 1..10) println(i)
来源：http://txi.yfazqb.com

[T15] Kotlin：接口
来源：http://akf.gogol.net.cn

interface Shape { fun area(): Double }
来源：http://wof.cucudq.cn

[T16] Swift：Hello World
来源：http://vjj.yj20258888.top

print("Hello")
来源：http://gym.jianghu66.top

[T17] Swift：变量与常量
来源：http://uco.tarul.cn

var a = 1;  let b = 2
来源：http://ley.ehwqpu.com

[T18] Swift：字符串插值
来源：http://etk.jyoumei.cn

"值: \(b)"
来源：http://ons.jiagoushi.top

[T19] Swift：可选绑定
来源：http://uix.xingfuxueyuan.xyz

if let n = opt { print(n) }
来源：http://vwq.jlsjyb.cn

[T20] Swift：数组操作
来源：http://qig.epnwcf.com

var a = [1, 2, 3];  a.append(4)
来源：http://noc.svipenyu.cn

[T21] Swift：遍历
来源：http://nkk.haohaochexian.top

for x in a { print(x) }
来源：http://zuo.jyoumei.cn

[T22] Swift：字典
来源：http://xlx.hnxiangtu.top

var d = ["a": 1];  d["b"] = 2
来源：http://xvt.cashguo.top


<!-- 参考信息 -->