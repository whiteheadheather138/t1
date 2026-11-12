代发 wailian999

echo "${#arr[@]}"
来源：http://xeg.yonumen.top

[R20] 关联数组（字典）
来源：http://ivj.cqqwz.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mcr.jinqigufen.top

[R21] 字符串长度
来源：http://kht.316326.xyz

echo "${#s}"
来源：http://mwx.yuxming.cn

[R22] 截取子串
来源：http://yke.vqdsnc.cn

echo "${s:0:5}"
来源：http://whz.shangyingyoupin.top

[R23] 字符串替换
来源：http://dpu.jianghu66.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wfg.yangfankeji.com

[R24] 大小写转换
来源：http://xfv.xziqi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://shi.chenlongwang.top

[R25] 去后缀 / 去前缀
来源：http://oxu.zhoulong.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://ajm.birdmap.top

[R26] 命令替换
来源：http://agk.guowangkeji.top

now=$(date +%F); echo "$now"
来源：http://cbl.vqdsnc.cn

[R27] 算术展开
来源：http://mnk.redwolf501.top

echo $((1 + 2 * 3))
来源：http://ihb.sxryk.cn

[R28] 浮点运算
来源：http://yjp.hysaishi.cn

echo "scale=2; 10/3" | bc
来源：http://fui.zycfv.cn

[R29] 定义函数
来源：http://wmu.daxiang520.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bfr.vehdjk.com

[R30] 函数返回状态码
来源：http://iwo.jiagoushi.top

f() { return 0; }; f || echo "失败了"
来源：http://xpc.tian-w.cn

[R31] 局部变量
来源：http://sti.vehdjk.com

f() { local x=1; echo "$x"; }
来源：http://ckr.redwolf501.top

[R32] 参数个数校验
来源：http://bhg.hywenlv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vkq.zdbjq.cn

[R33] 捕获错误并提示行号
来源：http://fhb.vehdjk.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vsj.zhaomingkeji.xyz

[R34] 退出时清理
来源：http://bsw.ivvv.top

trap 'rm -f "$tmp"' EXIT
来源：http://nsp.kuanghao11.cn

[R35] 后台执行并等待
来源：http://cmq.wangshuangyany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://muq.zhongyouzk.top

[R36] 并发执行多个任务
来源：http://bmr.gzhubu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bof.jianghu66.top

[R37] 把输出赋给变量
来源：http://spc.cheryme.top

files=$(ls -1)
来源：http://mam.haohaochexian.top

[R38] 管道串联
来源：http://fog.bjfxy.top

cat a.txt | grep -i error | wc -l
来源：http://ymo.ctjpmb.com

[R39] 重定向标准输出与错误
来源：http://lig.meibo888.top

cmd > out.log 2>&1
来源：http://alq.yj20258.top

[R40] 追加写日志
来源：http://adj.ivvv.top

echo "log" >> out.log
来源：http://rkq.cqqwz.cn

[R41] 丢弃输出
来源：http://ary.gogol.net.cn

cmd >/dev/null 2>&1
来源：http://cgr.ctjpmb.com

[R42] 输入重定向
来源：http://oic.guannengcc.top

wc -l < a.txt
来源：http://vua.hcnkem.com

[R43] 按名字查找文件
来源：http://bjw.fengsongda.top

find . -name "*.log" -type f
来源：http://dzk.pengpengdd.cyou

[R44] 按修改时间查找
来源：http://abt.hcnkem.com

find . -mtime -7 -type f
来源：http://erz.shanyushiyangtech.top

[R45] 批量删除
来源：http://yrg.uphjek.com

find . -name "*.tmp" -delete
来源：http://szk.wangdashe.top

[R46] 递归替换文件内容
来源：http://ghx.pycfn.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fog.xuanzx.com

[R47] sed 单行替换
来源：http://cxu.pycfn.com

sed -i 's/foo/bar/g' a.txt
来源：http://snh.wangdashe.top

[R48] awk 取指定列
来源：http://npp.aizwys.cn

awk '{print $1, $3}' a.txt
来源：http://dkm.gotoacloud.top

[R49] awk 带条件
来源：http://blu.sufxvd.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yyx.bjfxy.top

[R50] awk 求和
来源：http://xml.zhixingplan.top

awk '{s += $2} END {print s}' a.txt
来源：http://qqo.yfazqb.com

[R51] 排序去重取前几
来源：http://glj.tianlin.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://ofp.shanyushiyangtech.top

[R52] 统计行数
来源：http://nbs.feifeiyinyue.top

wc -l a.txt
来源：http://coy.daxiang520.top

[R53] 查看文件头与实时尾
来源：http://iac.shangyingyoupin.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cnw.shuidangran.top

[R54] 比较两个文件
来源：http://pjs.zhiwuduotai.top

diff a.txt b.txt
来源：http://cdt.wangdashe.top

[R55] 压缩与解压
来源：http://env.shangyingyoupin.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://srg.jqgfzy.top

[R56] 远程拷贝
来源：http://alc.xingfuxueyuan.xyz

scp file user@host:/path/
来源：http://nyn.xuetiantiany.cn

[R57] 远程执行命令
来源：http://wal.fzhhl.top

ssh user@host 'uptime'
来源：http://fdk.gzhubu.top

[R58] 下载文件
来源：http://qnp.yfazqb.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ppd.xziqi.cn

[R59] 发 POST JSON
来源：http://mhh.jianghu66.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hix.chenjidiqi.icu

[R60] 只看 HTTP 状态码
来源：http://buc.0kj1m.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fzz.shanyushiyangkeji.top

[R61] 磁盘占用
来源：http://vir.tianlin.xyz

df -h;  du -sh *
来源：http://tfs.daxiang520.top

[R62] 找最占空间的文件
来源：http://vlw.52xcode.cn

du -ah . | sort -rh | head -10
来源：http://cmu.hywenlv.cn

[R63] 内存与进程
来源：http://msf.yueranfly.top

free -h;  ps aux | grep nginx
来源：http://qld.zhixingplan.top

[R64] 结束进程
来源：http://ywh.nanxuanxn.top

kill -9 $(pgrep -f app.py)
来源：http://qxk.316326.xyz

[R65] 查看端口占用
来源：http://epu.guannengcc.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jcj.dashuyun.cn

[R66] 定时任务
来源：http://oxm.yanxiufei.cn

crontab -e;  crontab -l
来源：http://fer.shanyushiyangtech.top

[R67] 生成随机十六进制串
来源：http://puk.pengpengdd.cyou

openssl rand -hex 16
来源：http://tyv.guowangkeji.top

[R68] 计算文件校验值
来源：http://gql.xinyue.icu

sha256sum a.txt;  md5sum a.txt
来源：http://mtq.tianlin.xyz

[R69] 生成随机密码
来源：http://ass.jinghuilouyu.cn

head -c 16 /dev/urandom | base64
来源：http://qeh.yanxiufei.cn

[R70] 时间戳与互转
来源：http://rip.andypj.xyz

date +%s;  date -d @1700000000
来源：http://emf.fktsv.cn

[R71] 日期格式化
来源：http://orl.vqdsnc.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vhh.daxiang520.top

[R72] 等待端口就绪
来源：http://gsr.fanxiaobao.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://zfr.sxryk.cn

[R73] 分割大日志
来源：http://qyu.yanxiufei.cn

split -l 1000 big.log part_
来源：http://bfv.yuxming.cn

[R74] 批量重命名
来源：http://nzi.yuanzhike.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kfr.cheryme.top

[R75] 导出环境变量
来源：http://ysk.shuidangran.top

export PATH="$HOME/bin:$PATH"
来源：http://xqj.epnwcf.com

[R76] 使用临时文件
来源：http://oaf.xziqi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ibk.gaohongyu789.top

[R77] 读取用户输入
来源：http://xde.jiagoushi.top

read -rp "请输入: " ans
来源：http://kpx.jinyuanbaomall.cn

[R78] 交互式菜单
来源：http://mkn.chenzaomai.com

select opt in a b c; do echo "$opt"; break; done
来源：http://pwm.haohaochexian.top

[R79] 解析命令行选项
来源：http://wuj.gzhubu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://upa.vqdsnc.cn

[R80] 查看脚本执行耗时
来源：http://eew.fktsv.cn

time ./run.sh
来源：http://zwh.wangdashe.top

================================================================================
来源：http://uan.yj20258888.top

S. C / C++ 专题
来源：http://xcf.jiagoushi.top

================================================================================
来源：http://nps.yj202588.top

[S01] C：Hello World
来源：http://ers.haohaochexian.top

#include <stdio.h>
来源：http://biy.cucudq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nja.svipenyu.cn

[S02] C：变量与格式化输出
来源：http://wop.52xcode.cn

int a = 10; printf("%d\n", a);
来源：http://cbw.ctjpmb.com

[S03] C：读入整数
来源：http://sml.kuanghao11.cn

int x; scanf("%d", &x);
来源：http://got.nanxuanxn.top

[S04] C：字符串复制
来源：http://fsf.guowangkeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://qht.uphjek.com

[S05] C：字符串长度
来源：http://cnb.gogol.net.cn

strlen(s)
来源：http://tah.yvedp.cn

[S06] C：字符串比较
来源：http://kcw.zhoulong.xyz

strcmp(a, b) == 0
来源：http://bzy.haohaochexian.top

[S07] C：数组遍历求和
来源：http://tpz.jyoumei.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gvj.chenzaomai.com

[S08] C：动态内存分配与释放
来源：http://dwq.svipenyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bna.ctjpmb.com

[S09] C：结构体定义与初始化
来源：http://xhv.gogol.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://guo.xuanzx.com

[S10] C：指针与解引用
来源：http://pmh.redwolf501.top

int *p = &a;  *p = 5;
来源：http://cwr.guannengcc.top

[S11] C：逐行读文件
来源：http://cpp.fzhhl.top

FILE *f = fopen("a.txt", "r");
来源：http://pry.uphjek.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://wrl.vehdjk.com

fclose(f);
来源：http://uxi.zhoulong.xyz

[S12] C：写文件
来源：http://hdm.yonumen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://snf.xziqi.cn

[S13] C：宏定义
来源：http://mvu.zycfv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uxm.epnwcf.com

[S14] C：枚举
来源：http://ysw.tianlin.xyz

enum Color { RED, GREEN, BLUE };
来源：http://rao.shangyingyoupin.top

[S15] C：类型转换
来源：http://vvn.yj202588.top

(double) a / b
来源：http://kkr.fehbvm.com

[S16] C：位操作置位
来源：http://ocj.shzxlz.cn

x |= (1 << 3);
来源：http://yzf.gotoacloud.top

[S17] C：安全拼接字符串
来源：http://tjm.birdmap.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://inm.shanyushiyangkeji.top

[S18] C：命令行参数
来源：http://jfh.smart0.xyz

int main(int argc, char **argv)
来源：http://bjd.birdmap.top

[S19] C：快速排序
来源：http://rdj.gaohongyu789.top

qsort(a, n, sizeof(int), cmp);
来源：http://hsg.9152youxi.cn

[S20] C：二分查找
来源：http://wvf.cqqwz.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://anl.hcnkem.com

[S21] C：字符类别判断
来源：http://itr.yonumen.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qqi.zhijiandao.cn

[S22] C：字符串转数字
来源：http://kio.meibo888.top

atoi("42");  strtod("3.14", NULL);
来源：http://znp.bbcook.cn

[S23] C：随机数
来源：http://alv.daxiang520.top

srand(time(NULL));  int r = rand() % 100;
来源：http://vez.cqqwz.cn

[S24] C：获取本地时间
来源：http://ise.yonumen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://unb.hywenlv.cn

[S25] C：内存拷贝
来源：http://hph.shangyingyoupin.top

memcpy(dst, src, n);
来源：http://ska.tianlin.xyz

[S26] C：内存清零
来源：http://fsm.sjlbkw.cn

memset(a, 0, sizeof a);
来源：http://zje.havefunace.top

[S27] C：定义常量
来源：http://aud.shangyingyoupin.top

const double PI = 3.14159;
来源：http://kfz.xingfuxueyuan.xyz

[S28] C：静态变量
来源：http://pmn.wangdashe.top

static int counter = 0;
来源：http://lmz.fzhhl.top

[S29] C：变参函数
来源：http://zby.ydzc1.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dkr.sysykeji.top

[S30] C：头文件保护
来源：http://jbu.zhiwuduotai.top

#ifndef X_H
来源：http://voh.gogol.net.cn

#define X_H
来源：http://cuj.yuanzhike.top

#endif
来源：http://yvm.redwolf501.top

[S31] C++：Hello World
来源：http://hkd.9152youxi.cn

#include <iostream>
来源：http://sox.yonumen.top

int main() { std::cout << "Hello\n"; }
来源：http://emz.jyoumei.cn

[S32] C++：字符串
来源：http://skn.ivvv.top

std::string s = "hi";  s += "!";
来源：http://wll.aizwys.cn

[S33] C++：vector 增删
来源：http://aqu.sufxvd.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wzj.hcnkem.com

[S34] C++：遍历 vector
来源：http://brn.haohaochexian.top

for (auto &x : v) { std::cout << x; }
来源：http://ten.yfazqb.com

[S35] C++：map
来源：http://oaj.hysaishi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dus.wangshuangyany.cn

[S36] C++：unordered_map
来源：http://ulq.ydjk.org.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tta.uphjek.com

[S37] C++：set
来源：http://xvk.shuidangran.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uok.guannengcc.top

[S38] C++：排序
来源：http://zoa.nanxinkj.top

std::sort(v.begin(), v.end());
来源：http://vlu.xylfe.cn

[S39] C++：自定义比较器排序
来源：http://qoq.iojbl.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://obl.gogol.net.cn

[S40] C++：查找元素
来源：http://tkp.dianchejie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://obj.aizwys.cn

[S41] C++：类与构造函数
来源：http://xjt.sufxvd.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wpd.andypj.xyz

[S42] C++：继承与虚函数
来源：http://vmj.jqgufenzy.top

class B : public Base { public: void f() override {} };
来源：http://rxa.tianlin.xyz

[S43] C++：智能指针
来源：http://pyz.hnxiangtu.top

auto p = std::make_unique<int>(5);
来源：http://jfk.sweek.top

[S44] C++：引用传参
来源：http://ofd.jinqigufen.top

void inc(int &x) { ++x; }
来源：http://qzk.cheryme.top

[S45] C++：lambda
来源：http://dyr.zhijiandao.cn

auto add = [](int a, int b) { return a + b; };
来源：http://njm.jyoumei.cn

[S46] C++：函数模板
来源：http://zvw.yonumen.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ozy.xylfe.cn

[S47] C++：结构化绑定遍历
来源：http://mjm.jiagoushi.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hdw.iojbl.cn

[S48] C++：逐行读文件
来源：http://gpy.zycfv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dwo.smart0.xyz

while (std::getline(in, line)) { }
来源：http://eoy.sjlbkw.cn

[S49] C++：写文件
来源：http://nsi.dianchejie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lgt.tian-w.cn

[S50] C++：格式化数字
来源：http://xdn.smart0.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eug.shanyushiyangkeji.top

[S51] C++：显式类型转换
来源：http://flg.yanxiufei.cn

static_cast<double>(a) / b
来源：http://yli.redwolf501.top

[S52] C++：const 与 noexcept
来源：http://enr.zdbjq.cn

int size() const noexcept { return n_; }
来源：http://szc.xziqi.cn

[S53] C++：移动语义
来源：http://fui.gogol.net.cn

std::vector<int> w = std::move(v);
来源：http://fhb.52xcode.cn

[S54] C++：异常处理
来源：http://afs.guowangkeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hlw.zdqjudy.top

[S55] C++：结构化绑定
来源：http://zfx.hammf.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sqg.shanyushiyangtech.top

[S56] C++：optional
来源：http://ajt.sxryk.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tfq.uphjek.com

[S57] C++：编译期常量
来源：http://pvz.yonumen.top

constexpr int N = 10;
来源：http://zmd.xuanzx.com

[S58] C++：命名空间
来源：http://mxm.fanxiaobao.xyz

namespace ns { int f() { return 1; } }
来源：http://ddf.jinyuanbaomall.cn

[S59] C++：静态断言
来源：http://dtt.hnqzz.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dse.ctjpmb.com

[S60] C++：遍历并删除元素
来源：http://kna.guowangkeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://axn.yanxiufei.cn

================================================================================
来源：http://nzd.hammf.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mpr.nanxinkj.top

================================================================================
来源：http://wsk.hcnkem.com

[T01] Kotlin：Hello World
来源：http://rfw.uphjek.com

println("Hello")
来源：http://ity.ywan-chungtsiang.top

[T02] Kotlin：变量
来源：http://ver.9152youxi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xlw.c1oappe.top

[T03] Kotlin：字符串模板
来源：http://xrp.ctjpmb.com

"值: $b"
来源：http://qzz.yongpay.top

[T04] Kotlin：空安全
来源：http://nao.sxryk.cn

val n: String? = null;  n?.length
来源：http://kpq.yueranfly.top

[T05] Kotlin：when 表达式
来源：http://kjd.smart0.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ikh.xingfuxueyuan.xyz

[T06] Kotlin：集合映射
来源：http://dkb.bjfxy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://oxs.vqdsnc.cn

[T07] Kotlin：集合过滤
来源：http://enj.zdbjq.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dxf.sweek.top

[T08] Kotlin：数据类
来源：http://wfy.gzhubu.top

data class User(val name: String, val age: Int)
来源：http://fah.hcnkem.com

[T09] Kotlin：扩展函数
来源：http://zck.jianghu66.top

fun String.exclaim() = this + "!"
来源：http://cvp.ydzc1.top

[T10] Kotlin：默认参数
来源：http://jfe.fktsv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ibf.sweek.top

[T11] Kotlin：协程
来源：http://fgd.ydjk.org.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gvi.aibaodan.cn

[T12] Kotlin：解构声明
来源：http://lui.fanxiaobao.xyz

val (a, b) = Pair(1, 2)
来源：http://ymt.vqdsnc.cn

[T13] Kotlin：只读 Map
来源：http://spg.mhx1999.top

val m = mapOf("a" to 1)
来源：http://ekq.birdmap.top

[T14] Kotlin：循环
来源：http://dqk.feifeiyinyue.top

for (i in 1..10) println(i)
来源：http://rfo.hfpthk.cn

[T15] Kotlin：接口
来源：http://vcp.shzxlz.cn

interface Shape { fun area(): Double }
来源：http://jcs.dashuyun.cn

[T16] Swift：Hello World
来源：http://ybv.xziqi.cn

print("Hello")
来源：http://pky.cqqwz.cn

[T17] Swift：变量与常量
来源：http://elq.xingfuxueyuan.xyz

var a = 1;  let b = 2
来源：http://ryz.xziqi.cn

[T18] Swift：字符串插值
来源：http://are.snrcjt.cn

"值: \(b)"
来源：http://bid.shanyushiyangtech.top

[T19] Swift：可选绑定
来源：http://zfp.zhongyouzk.top

if let n = opt { print(n) }
来源：http://jdi.xuanzx.com

[T20] Swift：数组操作
来源：http://ycx.yj20258.top

var a = [1, 2, 3];  a.append(4)
来源：http://nnf.yongpay.top

[T21] Swift：遍历
来源：http://lgh.hysaishi.cn

for x in a { print(x) }
来源：http://szz.jqgfzy.top

[T22] Swift：字典
来源：http://oll.zycfv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nbe.c1oappe.top


<!-- 参考信息 -->