代发 wailian999

echo "${#arr[@]}"
来源：http://ryh.cashguo.top

[R20] 关联数组（字典）
来源：http://fie.yonumen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://czw.52xcode.cn

[R21] 字符串长度
来源：http://vsu.havefunace.top

echo "${#s}"
来源：http://lwc.aibaodan.cn

[R22] 截取子串
来源：http://brr.c1oappe.top

echo "${s:0:5}"
来源：http://rqy.smart0.xyz

[R23] 字符串替换
来源：http://nuu.mhx1999.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://opv.wangdashe.top

[R24] 大小写转换
来源：http://tzu.sweek.top

echo "${s^^}"; echo "${s,,}"
来源：http://kfp.yuxming.cn

[R25] 去后缀 / 去前缀
来源：http://ypo.shanyushiyangtech.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://pyo.wangshuangyany.cn

[R26] 命令替换
来源：http://exo.guannengcc.top

now=$(date +%F); echo "$now"
来源：http://syx.jianghu66.top

[R27] 算术展开
来源：http://vjs.shuidangran.top

echo $((1 + 2 * 3))
来源：http://faz.cheryme.top

[R28] 浮点运算
来源：http://bbf.guannengcc.top

echo "scale=2; 10/3" | bc
来源：http://bqi.yanxiufei.cn

[R29] 定义函数
来源：http://zml.nanxuanxn.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://szu.andypj.xyz

[R30] 函数返回状态码
来源：http://jsr.sysykeji.top

f() { return 0; }; f || echo "失败了"
来源：http://ewv.52xcode.cn

[R31] 局部变量
来源：http://cwt.wangdashe.top

f() { local x=1; echo "$x"; }
来源：http://gxa.snrcjt.cn

[R32] 参数个数校验
来源：http://kni.gotoacloud.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dij.hongshengwenyu.top

[R33] 捕获错误并提示行号
来源：http://sdb.chenjidiqi.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lko.jinghuilouyu.cn

[R34] 退出时清理
来源：http://dyd.hammf.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kwj.hesvh.cn

[R35] 后台执行并等待
来源：http://rrc.jyoumei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://oyr.ctjpmb.com

[R36] 并发执行多个任务
来源：http://dzp.0kj1m.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tcl.jqgufenzy.top

[R37] 把输出赋给变量
来源：http://wru.svipenyu.cn

files=$(ls -1)
来源：http://anc.yanxiufei.cn

[R38] 管道串联
来源：http://esf.pycfn.com

cat a.txt | grep -i error | wc -l
来源：http://wud.zhiwuduotai.top

[R39] 重定向标准输出与错误
来源：http://jph.ppjwa.cn

cmd > out.log 2>&1
来源：http://xwo.chenjidiqi.icu

[R40] 追加写日志
来源：http://fmt.xziqi.cn

echo "log" >> out.log
来源：http://pky.zhiwuduotai.top

[R41] 丢弃输出
来源：http://dmj.zhixingplan.top

cmd >/dev/null 2>&1
来源：http://awv.yonumen.top

[R42] 输入重定向
来源：http://ewx.sjlbkw.cn

wc -l < a.txt
来源：http://lsb.c1oappe.top

[R43] 按名字查找文件
来源：http://lgk.dianchejie.cn

find . -name "*.log" -type f
来源：http://esq.zhixingplan.top

[R44] 按修改时间查找
来源：http://lec.hongshengwenyu.top

find . -mtime -7 -type f
来源：http://wrq.uphjek.com

[R45] 批量删除
来源：http://fww.tarul.cn

find . -name "*.tmp" -delete
来源：http://qjo.xinyue.icu

[R46] 递归替换文件内容
来源：http://cmn.svipenyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://byw.tianlin.xyz

[R47] sed 单行替换
来源：http://slf.xuanzx.com

sed -i 's/foo/bar/g' a.txt
来源：http://onq.mhx1999.top

[R48] awk 取指定列
来源：http://qmo.yvedp.cn

awk '{print $1, $3}' a.txt
来源：http://uyj.nanxinkj.top

[R49] awk 带条件
来源：http://czv.cheryme.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mxw.smart0.xyz

[R50] awk 求和
来源：http://jli.cashguo.top

awk '{s += $2} END {print s}' a.txt
来源：http://tns.yanxiufei.cn

[R51] 排序去重取前几
来源：http://xzs.uphjek.com

sort a.txt | uniq -c | sort -rn | head
来源：http://ihr.hongshengwenyu.top

[R52] 统计行数
来源：http://iux.jinyuanbaomall.cn

wc -l a.txt
来源：http://qbb.mhx1999.top

[R53] 查看文件头与实时尾
来源：http://qmc.quarkkingdee.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hfe.zycfv.cn

[R54] 比较两个文件
来源：http://ldv.tarul.cn

diff a.txt b.txt
来源：http://dvq.tian-w.cn

[R55] 压缩与解压
来源：http://tcw.jqgufenzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tui.ywan-chungtsiang.top

[R56] 远程拷贝
来源：http://unu.0kj1m.cn

scp file user@host:/path/
来源：http://ehf.gogol.net.cn

[R57] 远程执行命令
来源：http://uwa.nwbrower.top

ssh user@host 'uptime'
来源：http://clq.jqgufenzy.top

[R58] 下载文件
来源：http://blr.smart0.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jgw.zhaomingkeji.xyz

[R59] 发 POST JSON
来源：http://rxa.uphjek.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cmk.birdmap.top

[R60] 只看 HTTP 状态码
来源：http://rkk.birdmap.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://apq.sysykeji.top

[R61] 磁盘占用
来源：http://crd.chenzaomai.com

df -h;  du -sh *
来源：http://psr.ydjk.org.cn

[R62] 找最占空间的文件
来源：http://xtw.yuxming.cn

du -ah . | sort -rh | head -10
来源：http://qzg.andypj.xyz

[R63] 内存与进程
来源：http://rbm.xziqi.cn

free -h;  ps aux | grep nginx
来源：http://irs.nanxuanxn.top

[R64] 结束进程
来源：http://nyn.kuanghao11.cn

kill -9 $(pgrep -f app.py)
来源：http://kzb.c1oappe.top

[R65] 查看端口占用
来源：http://rrq.iojbl.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://eax.zhengqikj.top

[R66] 定时任务
来源：http://ozy.yuanzhike.top

crontab -e;  crontab -l
来源：http://app.jqgufenzy.top

[R67] 生成随机十六进制串
来源：http://cty.daria6918.cn

openssl rand -hex 16
来源：http://krs.iojbl.cn

[R68] 计算文件校验值
来源：http://oij.shuidangran.top

sha256sum a.txt;  md5sum a.txt
来源：http://eli.epnwcf.com

[R69] 生成随机密码
来源：http://yrc.xuanzx.com

head -c 16 /dev/urandom | base64
来源：http://rze.ctjpmb.com

[R70] 时间戳与互转
来源：http://ayo.zhengqikj.top

date +%s;  date -d @1700000000
来源：http://zwt.jqgufenzy.top

[R71] 日期格式化
来源：http://ngs.svipenyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yus.jyoumei.cn

[R72] 等待端口就绪
来源：http://llb.cdnleiting.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zvx.snrcjt.cn

[R73] 分割大日志
来源：http://iie.hammf.cn

split -l 1000 big.log part_
来源：http://krp.bbcook.cn

[R74] 批量重命名
来源：http://wzm.shangyingyoupin.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://aqo.ctjpmb.com

[R75] 导出环境变量
来源：http://tqn.shangyingyoupin.top

export PATH="$HOME/bin:$PATH"
来源：http://oql.nwbrower.top

[R76] 使用临时文件
来源：http://iar.cqqwz.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://emz.ydjk.org.cn

[R77] 读取用户输入
来源：http://alr.cheryme.top

read -rp "请输入: " ans
来源：http://bwq.jyoumei.cn

[R78] 交互式菜单
来源：http://cor.dianchejie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cpc.havefunace.top

[R79] 解析命令行选项
来源：http://xcy.zdbjq.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://muh.xziqi.cn

[R80] 查看脚本执行耗时
来源：http://tdx.xinyue.icu

time ./run.sh
来源：http://dxc.jinyuanbaomall.cn

================================================================================
来源：http://yws.tianlin.xyz

S. C / C++ 专题
来源：http://mmr.vehdjk.com

================================================================================
来源：http://pts.tian-w.cn

[S01] C：Hello World
来源：http://czw.fktsv.cn

#include <stdio.h>
来源：http://qyx.smart0.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://cvt.daxiang520.top

[S02] C：变量与格式化输出
来源：http://xka.dashuyun.cn

int a = 10; printf("%d\n", a);
来源：http://gfh.yanxiufei.cn

[S03] C：读入整数
来源：http://kum.gogol.net.cn

int x; scanf("%d", &x);
来源：http://tnk.sysykeji.top

[S04] C：字符串复制
来源：http://avz.xuanzx.com

char dst[32]; strcpy(dst, "hi");
来源：http://sjw.yueranfly.top

[S05] C：字符串长度
来源：http://ufs.zdbjq.cn

strlen(s)
来源：http://elg.zhongyouzk.top

[S06] C：字符串比较
来源：http://lcw.52xcode.cn

strcmp(a, b) == 0
来源：http://gqs.iojbl.cn

[S07] C：数组遍历求和
来源：http://nox.hongshengwenyu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xwe.haohaochexian.top

[S08] C：动态内存分配与释放
来源：http://hnw.shanyushiyangkeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ino.nanxuanxn.top

[S09] C：结构体定义与初始化
来源：http://xkw.xuanzx.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ygb.epnwcf.com

[S10] C：指针与解引用
来源：http://mzr.nwbrower.top

int *p = &a;  *p = 5;
来源：http://qfn.andypj.xyz

[S11] C：逐行读文件
来源：http://uii.cqqwz.cn

FILE *f = fopen("a.txt", "r");
来源：http://qob.bbcook.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tvf.zhiwuduotai.top

fclose(f);
来源：http://flv.zhixingplan.top

[S12] C：写文件
来源：http://pfx.tian-w.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kfv.xingfuxueyuan.xyz

[S13] C：宏定义
来源：http://msw.hammf.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vvx.zhaomingkeji.xyz

[S14] C：枚举
来源：http://zmw.fengsongda.top

enum Color { RED, GREEN, BLUE };
来源：http://dnp.hnqzz.top

[S15] C：类型转换
来源：http://omy.chenzaomai.com

(double) a / b
来源：http://yoj.snrcjt.cn

[S16] C：位操作置位
来源：http://oby.andypj.xyz

x |= (1 << 3);
来源：http://off.hnqzz.top

[S17] C：安全拼接字符串
来源：http://pis.cucudq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yhb.guannengcc.top

[S18] C：命令行参数
来源：http://feg.guowangkeji.top

int main(int argc, char **argv)
来源：http://ouv.tianlin.xyz

[S19] C：快速排序
来源：http://ulz.yuxming.cn

qsort(a, n, sizeof(int), cmp);
来源：http://huj.jyoumei.cn

[S20] C：二分查找
来源：http://wku.snrcjt.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nyi.yanxiufei.cn

[S21] C：字符类别判断
来源：http://ewh.wangshuangyany.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fsm.cqqwz.cn

[S22] C：字符串转数字
来源：http://qhe.havefunace.top

atoi("42");  strtod("3.14", NULL);
来源：http://wez.iojbl.cn

[S23] C：随机数
来源：http://ujq.jyoumei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gxn.xziqi.cn

[S24] C：获取本地时间
来源：http://vgp.9152youxi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qjz.bjfxy.top

[S25] C：内存拷贝
来源：http://ocg.jiagoushi.top

memcpy(dst, src, n);
来源：http://fjk.mhx1999.top

[S26] C：内存清零
来源：http://mjo.fktsv.cn

memset(a, 0, sizeof a);
来源：http://lcv.yanxiufei.cn

[S27] C：定义常量
来源：http://vzv.redwolf501.top

const double PI = 3.14159;
来源：http://ome.havefunace.top

[S28] C：静态变量
来源：http://jdy.0kj1m.cn

static int counter = 0;
来源：http://eve.jianghu66.top

[S29] C：变参函数
来源：http://yyu.zhongyouzk.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oqc.iojbl.cn

[S30] C：头文件保护
来源：http://bru.haohaochexian.top

#ifndef X_H
来源：http://ysg.hongshengwenyu.top

#define X_H
来源：http://gou.birdmap.top

#endif
来源：http://edh.c1oappe.top

[S31] C++：Hello World
来源：http://jpv.yonumen.top

#include <iostream>
来源：http://yot.sysykeji.top

int main() { std::cout << "Hello\n"; }
来源：http://fpp.xuetiantiany.cn

[S32] C++：字符串
来源：http://dph.jlsjyb.cn

std::string s = "hi";  s += "!";
来源：http://utf.zhoulong.xyz

[S33] C++：vector 增删
来源：http://onp.9152youxi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ymu.yj202588.top

[S34] C++：遍历 vector
来源：http://zno.gotoacloud.top

for (auto &x : v) { std::cout << x; }
来源：http://cev.ydzc1.top

[S35] C++：map
来源：http://coj.ydjk.org.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jgj.guowangkeji.top

[S36] C++：unordered_map
来源：http://yff.xuanzx.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cfw.aizwys.cn

[S37] C++：set
来源：http://ghc.zycfv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fir.haohaochexian.top

[S38] C++：排序
来源：http://ced.smart0.xyz

std::sort(v.begin(), v.end());
来源：http://vwo.hnqzz.top

[S39] C++：自定义比较器排序
来源：http://bip.yvedp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hte.smart0.xyz

[S40] C++：查找元素
来源：http://heh.ppjwa.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lru.gotoacloud.top

[S41] C++：类与构造函数
来源：http://cqe.gogol.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iwo.tarul.cn

[S42] C++：继承与虚函数
来源：http://bpu.zdbjq.cn

class B : public Base { public: void f() override {} };
来源：http://qkc.hesvh.cn

[S43] C++：智能指针
来源：http://dwb.xingfuxueyuan.xyz

auto p = std::make_unique<int>(5);
来源：http://ryu.jqgfzy.top

[S44] C++：引用传参
来源：http://mqd.hnqzz.top

void inc(int &x) { ++x; }
来源：http://bxa.tian-w.cn

[S45] C++：lambda
来源：http://kom.tarul.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ujy.316326.xyz

[S46] C++：函数模板
来源：http://wkm.gaohongyu789.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nad.tarul.cn

[S47] C++：结构化绑定遍历
来源：http://tfd.tanke756.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gpp.jinyuanbaomall.cn

[S48] C++：逐行读文件
来源：http://dlw.hammf.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lpv.shzxlz.cn

while (std::getline(in, line)) { }
来源：http://zsv.cucudq.cn

[S49] C++：写文件
来源：http://rpj.ivvv.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yyd.xinyue.icu

[S50] C++：格式化数字
来源：http://mnf.zhijiandao.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kre.sysykeji.top

[S51] C++：显式类型转换
来源：http://wvm.xinyue.icu

static_cast<double>(a) / b
来源：http://blx.tian-w.cn

[S52] C++：const 与 noexcept
来源：http://tgq.jqgufenzy.top

int size() const noexcept { return n_; }
来源：http://ibm.nwbrower.top

[S53] C++：移动语义
来源：http://rqx.fanxiaobao.xyz

std::vector<int> w = std::move(v);
来源：http://xpx.xingfuxueyuan.xyz

[S54] C++：异常处理
来源：http://sdx.snrcjt.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tlr.tianlin.xyz

[S55] C++：结构化绑定
来源：http://iqx.pengpengdd.cyou

auto [a, b] = std::make_pair(1, 2);
来源：http://lev.fehbvm.com

[S56] C++：optional
来源：http://ovz.zdbjq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://scv.yanxiufei.cn

[S57] C++：编译期常量
来源：http://onz.daxiang520.top

constexpr int N = 10;
来源：http://iyr.dianchejie.cn

[S58] C++：命名空间
来源：http://ibu.cucudq.cn

namespace ns { int f() { return 1; } }
来源：http://wpt.cdnleiting.top

[S59] C++：静态断言
来源：http://vir.sxryk.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://apy.yongpay.top

[S60] C++：遍历并删除元素
来源：http://tvr.cashguo.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dbu.jqgfzy.top

================================================================================
来源：http://ndv.bbcook.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zaq.ydjk.org.cn

================================================================================
来源：http://aun.gotoacloud.top

[T01] Kotlin：Hello World
来源：http://bbq.316326.xyz

println("Hello")
来源：http://jep.bjfxy.top

[T02] Kotlin：变量
来源：http://lsv.316326.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bvc.nanxinkj.top

[T03] Kotlin：字符串模板
来源：http://spn.xuanzx.com

"值: $b"
来源：http://yrd.jinghuilouyu.cn

[T04] Kotlin：空安全
来源：http://ptq.xingfuxueyuan.xyz

val n: String? = null;  n?.length
来源：http://cmo.sysykeji.top

[T05] Kotlin：when 表达式
来源：http://vza.redwolf501.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jhe.pycfn.com

[T06] Kotlin：集合映射
来源：http://nrq.xuetiantiany.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://opa.zhijiandao.cn

[T07] Kotlin：集合过滤
来源：http://pko.meibo888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mbo.yanxiufei.cn

[T08] Kotlin：数据类
来源：http://igq.uphjek.com

data class User(val name: String, val age: Int)
来源：http://eln.9152youxi.cn

[T09] Kotlin：扩展函数
来源：http://cre.yj20258888.top

fun String.exclaim() = this + "!"
来源：http://tzn.bjfxy.top

[T10] Kotlin：默认参数
来源：http://msl.uphjek.com

fun greet(name: String = "World") = "Hi $name"
来源：http://pui.havefunace.top

[T11] Kotlin：协程
来源：http://gxh.tanke756.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://hwk.hywenlv.cn

[T12] Kotlin：解构声明
来源：http://pzz.quarkkingdee.top

val (a, b) = Pair(1, 2)
来源：http://vxm.cucudq.cn

[T13] Kotlin：只读 Map
来源：http://kjo.fanxiaobao.xyz

val m = mapOf("a" to 1)
来源：http://caz.sxryk.cn

[T14] Kotlin：循环
来源：http://rqc.sxryk.cn

for (i in 1..10) println(i)
来源：http://wsn.cdnleiting.top

[T15] Kotlin：接口
来源：http://tki.zhengqikj.top

interface Shape { fun area(): Double }
来源：http://qer.ctjpmb.com

[T16] Swift：Hello World
来源：http://wln.yuanzhike.top

print("Hello")
来源：http://wdj.yongpay.top

[T17] Swift：变量与常量
来源：http://amr.xinyue.icu

var a = 1;  let b = 2
来源：http://mqy.yj202588.top

[T18] Swift：字符串插值
来源：http://tvh.havefunace.top

"值: \(b)"
来源：http://mar.guowangkeji.top

[T19] Swift：可选绑定
来源：http://yiz.kuanghao11.cn

if let n = opt { print(n) }
来源：http://gly.cheryme.top

[T20] Swift：数组操作
来源：http://cjg.gaohongyu789.top

var a = [1, 2, 3];  a.append(4)
来源：http://iwv.cashguo.top

[T21] Swift：遍历
来源：http://pgm.shuidangran.top

for x in a { print(x) }
来源：http://jna.meibo888.top

[T22] Swift：字典
来源：http://enb.kuanghao11.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xbt.52xcode.cn


<!-- 参考信息 -->