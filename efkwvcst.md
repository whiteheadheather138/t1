代发 wailian999

echo "${#arr[@]}"
来源：http://rhg.jqgufenzy.top

[R20] 关联数组（字典）
来源：http://zdl.ppjwa.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pwt.yj202588.top

[R21] 字符串长度
来源：http://xul.haohaochexian.top

echo "${#s}"
来源：http://uve.zhixingplan.top

[R22] 截取子串
来源：http://lid.shanyushiyangkeji.top

echo "${s:0:5}"
来源：http://kok.bbcook.cn

[R23] 字符串替换
来源：http://qdd.zhoulong.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wul.nanxuanxn.top

[R24] 大小写转换
来源：http://rfq.gaohongyu789.top

echo "${s^^}"; echo "${s,,}"
来源：http://lrh.shangyingyoupin.top

[R25] 去后缀 / 去前缀
来源：http://mmx.shanyushiyangtech.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://szg.xinyue.icu

[R26] 命令替换
来源：http://kzn.ydjk.org.cn

now=$(date +%F); echo "$now"
来源：http://fgv.bjfxy.top

[R27] 算术展开
来源：http://uay.vqdsnc.cn

echo $((1 + 2 * 3))
来源：http://qbc.xziqi.cn

[R28] 浮点运算
来源：http://ajv.xuetiantiany.cn

echo "scale=2; 10/3" | bc
来源：http://lyl.52xcode.cn

[R29] 定义函数
来源：http://cvr.jinqigufen.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://krl.hongshengwenyu.top

[R30] 函数返回状态码
来源：http://mlb.zhoulong.xyz

f() { return 0; }; f || echo "失败了"
来源：http://yyh.hywenlv.cn

[R31] 局部变量
来源：http://hxt.ehwqpu.com

f() { local x=1; echo "$x"; }
来源：http://der.nanxinkj.top

[R32] 参数个数校验
来源：http://fav.vehdjk.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mes.cashguo.top

[R33] 捕获错误并提示行号
来源：http://apt.sweek.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kzk.shanyushiyangtech.top

[R34] 退出时清理
来源：http://kaq.ydzc1.top

trap 'rm -f "$tmp"' EXIT
来源：http://pjm.yfazqb.com

[R35] 后台执行并等待
来源：http://gnd.316326.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://apl.cheryme.top

[R36] 并发执行多个任务
来源：http://dek.yueranfly.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vxa.hcnkem.com

[R37] 把输出赋给变量
来源：http://foa.yueranfly.top

files=$(ls -1)
来源：http://wid.tian-w.cn

[R38] 管道串联
来源：http://erq.daria6918.cn

cat a.txt | grep -i error | wc -l
来源：http://qtf.ywan-chungtsiang.top

[R39] 重定向标准输出与错误
来源：http://qxp.tanke756.top

cmd > out.log 2>&1
来源：http://yez.iojbl.cn

[R40] 追加写日志
来源：http://drk.tanke756.top

echo "log" >> out.log
来源：http://xqn.nanxuanxn.top

[R41] 丢弃输出
来源：http://ycp.ydjk.org.cn

cmd >/dev/null 2>&1
来源：http://psh.sweek.top

[R42] 输入重定向
来源：http://qwx.xylfe.cn

wc -l < a.txt
来源：http://bcb.jianghu66.top

[R43] 按名字查找文件
来源：http://ooa.yj202588.top

find . -name "*.log" -type f
来源：http://bds.jinqigfzy.top

[R44] 按修改时间查找
来源：http://nzu.zhaomingkeji.xyz

find . -mtime -7 -type f
来源：http://jvv.zdqjudy.top

[R45] 批量删除
来源：http://oyu.cashguo.top

find . -name "*.tmp" -delete
来源：http://clm.pengpengdd.cyou

[R46] 递归替换文件内容
来源：http://bca.yongpay.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xfh.hywenlv.cn

[R47] sed 单行替换
来源：http://esf.sxryk.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pbh.sysykeji.top

[R48] awk 取指定列
来源：http://uaz.yuxming.cn

awk '{print $1, $3}' a.txt
来源：http://pfr.hfpthk.cn

[R49] awk 带条件
来源：http://fbx.yj20258888.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tix.hfpthk.cn

[R50] awk 求和
来源：http://pci.fktsv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bfq.wangshuangyany.cn

[R51] 排序去重取前几
来源：http://tdh.fktsv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lno.pengpengdd.cyou

[R52] 统计行数
来源：http://iuc.ydjk.org.cn

wc -l a.txt
来源：http://zke.52xcode.cn

[R53] 查看文件头与实时尾
来源：http://ujh.52xcode.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hdw.xuetiantiany.cn

[R54] 比较两个文件
来源：http://umm.hfpthk.cn

diff a.txt b.txt
来源：http://bfn.zdbjq.cn

[R55] 压缩与解压
来源：http://dvx.pycfn.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://byn.shangyingyoupin.top

[R56] 远程拷贝
来源：http://gnq.daxiang520.top

scp file user@host:/path/
来源：http://hjw.yuxming.cn

[R57] 远程执行命令
来源：http://xgd.shanyushiyangtech.top

ssh user@host 'uptime'
来源：http://sfd.shuidangran.top

[R58] 下载文件
来源：http://phg.chenjidiqi.icu

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ckp.tarul.cn

[R59] 发 POST JSON
来源：http://kvo.xinyue.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jcy.yj20258888.top

[R60] 只看 HTTP 状态码
来源：http://ypk.uphjek.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rwt.guannengcc.top

[R61] 磁盘占用
来源：http://lmh.zhengqikj.top

df -h;  du -sh *
来源：http://upk.uphjek.com

[R62] 找最占空间的文件
来源：http://axv.kuanghao11.cn

du -ah . | sort -rh | head -10
来源：http://tuj.fengsongda.top

[R63] 内存与进程
来源：http://ysp.epnwcf.com

free -h;  ps aux | grep nginx
来源：http://gop.fanxiaobao.xyz

[R64] 结束进程
来源：http://vja.yuanzhike.top

kill -9 $(pgrep -f app.py)
来源：http://zov.chenzaomai.com

[R65] 查看端口占用
来源：http://jxr.haohaochexian.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://usq.gzhubu.top

[R66] 定时任务
来源：http://xlh.tanke756.top

crontab -e;  crontab -l
来源：http://kfh.ppjwa.cn

[R67] 生成随机十六进制串
来源：http://jiw.zdqjudy.top

openssl rand -hex 16
来源：http://kfz.cqqwz.cn

[R68] 计算文件校验值
来源：http://rlk.yfazqb.com

sha256sum a.txt;  md5sum a.txt
来源：http://ols.yj202588.top

[R69] 生成随机密码
来源：http://mki.hysaishi.cn

head -c 16 /dev/urandom | base64
来源：http://qpx.zhixingplan.top

[R70] 时间戳与互转
来源：http://mub.pycfn.com

date +%s;  date -d @1700000000
来源：http://ygc.ivvv.top

[R71] 日期格式化
来源：http://ibw.yuanzhike.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vfw.yonumen.top

[R72] 等待端口就绪
来源：http://vaq.yuanzhike.top

until nc -z localhost 3306; do sleep 1; done
来源：http://mln.52xcode.cn

[R73] 分割大日志
来源：http://gkd.jqgfzy.top

split -l 1000 big.log part_
来源：http://ced.gogol.net.cn

[R74] 批量重命名
来源：http://yfi.fzhhl.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://aix.vqdsnc.cn

[R75] 导出环境变量
来源：http://lhg.gogol.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://dtl.epnwcf.com

[R76] 使用临时文件
来源：http://thp.316326.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blw.daria6918.cn

[R77] 读取用户输入
来源：http://ugi.hywenlv.cn

read -rp "请输入: " ans
来源：http://ahk.yj20258.top

[R78] 交互式菜单
来源：http://mvw.yuanzhike.top

select opt in a b c; do echo "$opt"; break; done
来源：http://kxf.zhengqikj.top

[R79] 解析命令行选项
来源：http://rlv.nwbrower.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dmo.daxiang520.top

[R80] 查看脚本执行耗时
来源：http://rag.guannengcc.top

time ./run.sh
来源：http://yhc.yj202588.top

================================================================================
来源：http://gdi.haohaochexian.top

S. C / C++ 专题
来源：http://nfn.zhoulong.xyz

================================================================================
来源：http://nbs.hywenlv.cn

[S01] C：Hello World
来源：http://woy.c1oappe.top

#include <stdio.h>
来源：http://ytl.xuetiantiany.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hdm.jqgufenzy.top

[S02] C：变量与格式化输出
来源：http://rlm.hammf.cn

int a = 10; printf("%d\n", a);
来源：http://iog.gogol.net.cn

[S03] C：读入整数
来源：http://yha.wangshuangyany.cn

int x; scanf("%d", &x);
来源：http://qtu.zdbjq.cn

[S04] C：字符串复制
来源：http://kab.snrcjt.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lsv.c1oappe.top

[S05] C：字符串长度
来源：http://jgl.sufxvd.cn

strlen(s)
来源：http://kuy.gaohongyu789.top

[S06] C：字符串比较
来源：http://xcg.dashuyun.cn

strcmp(a, b) == 0
来源：http://lgc.zhoulong.xyz

[S07] C：数组遍历求和
来源：http://gyz.andypj.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rqb.xziqi.cn

[S08] C：动态内存分配与释放
来源：http://lun.jqgufenzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rgj.fengsongda.top

[S09] C：结构体定义与初始化
来源：http://bzy.wangshuangyany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tnk.xuanzx.com

[S10] C：指针与解引用
来源：http://pbe.jlsjyb.cn

int *p = &a;  *p = 5;
来源：http://xqj.ppjwa.cn

[S11] C：逐行读文件
来源：http://sna.nanxuanxn.top

FILE *f = fopen("a.txt", "r");
来源：http://eoq.haohaochexian.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://gpn.ydzc1.top

fclose(f);
来源：http://euk.sjlbkw.cn

[S12] C：写文件
来源：http://hrk.smart0.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pwu.andypj.xyz

[S13] C：宏定义
来源：http://gjj.guowangkeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bcu.meibo888.top

[S14] C：枚举
来源：http://eiq.cashguo.top

enum Color { RED, GREEN, BLUE };
来源：http://zda.feifeiyinyue.top

[S15] C：类型转换
来源：http://bas.vehdjk.com

(double) a / b
来源：http://fnx.daria6918.cn

[S16] C：位操作置位
来源：http://uzx.c1oappe.top

x |= (1 << 3);
来源：http://alw.jinyuanbaomall.cn

[S17] C：安全拼接字符串
来源：http://xgo.yanxiufei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uwz.ivvv.top

[S18] C：命令行参数
来源：http://jps.hongshengwenyu.top

int main(int argc, char **argv)
来源：http://qpd.xziqi.cn

[S19] C：快速排序
来源：http://mjh.havefunace.top

qsort(a, n, sizeof(int), cmp);
来源：http://rme.shuidangran.top

[S20] C：二分查找
来源：http://mgr.snrcjt.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lpw.tianlin.xyz

[S21] C：字符类别判断
来源：http://hdh.jinqigufen.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wmf.zdbjq.cn

[S22] C：字符串转数字
来源：http://siy.feifeiyinyue.top

atoi("42");  strtod("3.14", NULL);
来源：http://uav.fktsv.cn

[S23] C：随机数
来源：http://fpf.daria6918.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://eaj.xuanzx.com

[S24] C：获取本地时间
来源：http://mhq.zdbjq.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wjb.zycfv.cn

[S25] C：内存拷贝
来源：http://raz.pengpengdd.cyou

memcpy(dst, src, n);
来源：http://yiv.epnwcf.com

[S26] C：内存清零
来源：http://wqf.havefunace.top

memset(a, 0, sizeof a);
来源：http://yus.jinqigufen.top

[S27] C：定义常量
来源：http://uoh.andypj.xyz

const double PI = 3.14159;
来源：http://seg.ydzc1.top

[S28] C：静态变量
来源：http://epq.yangfankeji.com

static int counter = 0;
来源：http://ncu.yj20258.top

[S29] C：变参函数
来源：http://arv.uphjek.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nse.fktsv.cn

[S30] C：头文件保护
来源：http://xng.cashguo.top

#ifndef X_H
来源：http://xkm.zdqjudy.top

#define X_H
来源：http://fgs.fehbvm.com

#endif
来源：http://edm.sweek.top

[S31] C++：Hello World
来源：http://niy.smart0.xyz

#include <iostream>
来源：http://ozi.wangshuangyany.cn

int main() { std::cout << "Hello\n"; }
来源：http://yvg.guowangkeji.top

[S32] C++：字符串
来源：http://zby.jinghuilouyu.cn

std::string s = "hi";  s += "!";
来源：http://hfv.wangdashe.top

[S33] C++：vector 增删
来源：http://gzu.tianlin.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hkx.yuanzhike.top

[S34] C++：遍历 vector
来源：http://uxq.hysaishi.cn

for (auto &x : v) { std::cout << x; }
来源：http://rcp.hnqzz.top

[S35] C++：map
来源：http://ikm.tarul.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mce.guowangkeji.top

[S36] C++：unordered_map
来源：http://izv.jqgufenzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ndb.cqqwz.cn

[S37] C++：set
来源：http://tnp.yj20258888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hjn.jinghuilouyu.cn

[S38] C++：排序
来源：http://fzk.sxryk.cn

std::sort(v.begin(), v.end());
来源：http://drx.bbcook.cn

[S39] C++：自定义比较器排序
来源：http://gqy.nwbrower.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gtt.ppjwa.cn

[S40] C++：查找元素
来源：http://yyc.zhoulong.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cus.redwolf501.top

[S41] C++：类与构造函数
来源：http://jjv.jlsjyb.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nij.pycfn.com

[S42] C++：继承与虚函数
来源：http://peu.ehwqpu.com

class B : public Base { public: void f() override {} };
来源：http://eob.mhx1999.top

[S43] C++：智能指针
来源：http://aci.zycfv.cn

auto p = std::make_unique<int>(5);
来源：http://cyt.daria6918.cn

[S44] C++：引用传参
来源：http://prt.shuidangran.top

void inc(int &x) { ++x; }
来源：http://tew.hywenlv.cn

[S45] C++：lambda
来源：http://zox.jiagoushi.top

auto add = [](int a, int b) { return a + b; };
来源：http://vva.smart0.xyz

[S46] C++：函数模板
来源：http://uxs.wangdashe.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ysg.chenlongwang.top

[S47] C++：结构化绑定遍历
来源：http://pci.hywenlv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qsc.zhijiandao.cn

[S48] C++：逐行读文件
来源：http://oxn.hongshengwenyu.top

std::ifstream in("a.txt");  std::string line;
来源：http://mzc.ctjpmb.com

while (std::getline(in, line)) { }
来源：http://ghd.shuidangran.top

[S49] C++：写文件
来源：http://hsr.guannengcc.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wib.vqdsnc.cn

[S50] C++：格式化数字
来源：http://qbf.pycfn.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cfg.jinghuilouyu.cn

[S51] C++：显式类型转换
来源：http://eti.feifeiyinyue.top

static_cast<double>(a) / b
来源：http://mrh.haohaochexian.top

[S52] C++：const 与 noexcept
来源：http://mha.shangyingyoupin.top

int size() const noexcept { return n_; }
来源：http://wzn.vqdsnc.cn

[S53] C++：移动语义
来源：http://fsd.ybcxt.top

std::vector<int> w = std::move(v);
来源：http://ecl.zdqjudy.top

[S54] C++：异常处理
来源：http://hag.shzxlz.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gcy.ywan-chungtsiang.top

[S55] C++：结构化绑定
来源：http://iuu.yangfankeji.com

auto [a, b] = std::make_pair(1, 2);
来源：http://uav.haohaochexian.top

[S56] C++：optional
来源：http://jbn.nwbrower.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ucz.ivvv.top

[S57] C++：编译期常量
来源：http://mmj.kuanghao11.cn

constexpr int N = 10;
来源：http://deq.zdbjq.cn

[S58] C++：命名空间
来源：http://rin.haohaochexian.top

namespace ns { int f() { return 1; } }
来源：http://mwb.vqdsnc.cn

[S59] C++：静态断言
来源：http://yno.snrcjt.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bmp.cheryme.top

[S60] C++：遍历并删除元素
来源：http://ogm.ppjwa.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://aux.uphjek.com

================================================================================
来源：http://gkg.cucudq.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tmg.ehwqpu.com

================================================================================
来源：http://sgp.ywan-chungtsiang.top

[T01] Kotlin：Hello World
来源：http://qtn.zhaomingkeji.xyz

println("Hello")
来源：http://fbr.xziqi.cn

[T02] Kotlin：变量
来源：http://ejj.ydzc1.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nku.gogol.net.cn

[T03] Kotlin：字符串模板
来源：http://uhu.ppjwa.cn

"值: $b"
来源：http://hce.snrcjt.cn

[T04] Kotlin：空安全
来源：http://xys.zhoulong.xyz

val n: String? = null;  n?.length
来源：http://ffr.zhiwuduotai.top

[T05] Kotlin：when 表达式
来源：http://itd.xinyue.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kwk.fzhhl.top

[T06] Kotlin：集合映射
来源：http://xmg.hnxiangtu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://pao.jianghu66.top

[T07] Kotlin：集合过滤
来源：http://gya.ydjk.org.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mhu.wangshuangyany.cn

[T08] Kotlin：数据类
来源：http://pgb.xuanzx.com

data class User(val name: String, val age: Int)
来源：http://sab.ctjpmb.com

[T09] Kotlin：扩展函数
来源：http://waz.yj20258.top

fun String.exclaim() = this + "!"
来源：http://xep.fktsv.cn

[T10] Kotlin：默认参数
来源：http://ccm.hammf.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ibz.birdmap.top

[T11] Kotlin：协程
来源：http://ipe.hnqzz.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://jqb.cucudq.cn

[T12] Kotlin：解构声明
来源：http://hhc.ydjk.org.cn

val (a, b) = Pair(1, 2)
来源：http://ctv.316326.xyz

[T13] Kotlin：只读 Map
来源：http://cvl.birdmap.top

val m = mapOf("a" to 1)
来源：http://lob.jinqigufen.top

[T14] Kotlin：循环
来源：http://qkt.jqgfzy.top

for (i in 1..10) println(i)
来源：http://taw.svipenyu.cn

[T15] Kotlin：接口
来源：http://krg.dashuyun.cn

interface Shape { fun area(): Double }
来源：http://tch.yongpay.top

[T16] Swift：Hello World
来源：http://dyp.shangyingyoupin.top

print("Hello")
来源：http://osm.zhijiandao.cn

[T17] Swift：变量与常量
来源：http://awt.52xcode.cn

var a = 1;  let b = 2
来源：http://aij.jqgfzy.top

[T18] Swift：字符串插值
来源：http://cub.zdbjq.cn

"值: \(b)"
来源：http://blf.hywenlv.cn

[T19] Swift：可选绑定
来源：http://alc.xziqi.cn

if let n = opt { print(n) }
来源：http://qnx.haohaochexian.top

[T20] Swift：数组操作
来源：http://agu.ydjk.org.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cct.xuanzx.com

[T21] Swift：遍历
来源：http://wlb.vqdsnc.cn

for x in a { print(x) }
来源：http://exe.jyoumei.cn

[T22] Swift：字典
来源：http://zrh.yongpay.top

var d = ["a": 1];  d["b"] = 2
来源：http://kcb.xingfuxueyuan.xyz


<!-- 参考信息 -->