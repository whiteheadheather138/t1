代发 wailian999

echo "${#arr[@]}"
来源：http://vyz.hysaishi.cn

[R20] 关联数组（字典）
来源：http://qud.aizwys.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wwf.sxryk.cn

[R21] 字符串长度
来源：http://mzs.gaohongyu789.top

echo "${#s}"
来源：http://ezr.ehwqpu.com

[R22] 截取子串
来源：http://qcx.hesvh.cn

echo "${s:0:5}"
来源：http://yoi.mhx1999.top

[R23] 字符串替换
来源：http://aut.bbcook.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iil.fengsongda.top

[R24] 大小写转换
来源：http://qdf.dashuyun.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xny.yanxiufei.cn

[R25] 去后缀 / 去前缀
来源：http://xun.yuanzhike.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://mmk.yfazqb.com

[R26] 命令替换
来源：http://irq.zhengqikj.top

now=$(date +%F); echo "$now"
来源：http://cpc.yuanzhike.top

[R27] 算术展开
来源：http://xyo.ybcxt.top

echo $((1 + 2 * 3))
来源：http://uzl.hongshengwenyu.top

[R28] 浮点运算
来源：http://fup.fzhhl.top

echo "scale=2; 10/3" | bc
来源：http://owt.bbcook.cn

[R29] 定义函数
来源：http://mnk.yvedp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bzv.jiagoushi.top

[R30] 函数返回状态码
来源：http://ndn.zhongyouzk.top

f() { return 0; }; f || echo "失败了"
来源：http://rcd.chenlongwang.top

[R31] 局部变量
来源：http://nco.hcnkem.com

f() { local x=1; echo "$x"; }
来源：http://mbr.hammf.cn

[R32] 参数个数校验
来源：http://zjh.birdmap.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ikw.havefunace.top

[R33] 捕获错误并提示行号
来源：http://ogm.hnxiangtu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yfb.jinghuilouyu.cn

[R34] 退出时清理
来源：http://wyr.zhongyouzk.top

trap 'rm -f "$tmp"' EXIT
来源：http://shn.ybcxt.top

[R35] 后台执行并等待
来源：http://xtx.jiagoushi.top

sleep 5 & pid=$!; wait "$pid"
来源：http://nwp.yanxiufei.cn

[R36] 并发执行多个任务
来源：http://csr.aizwys.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cxt.xziqi.cn

[R37] 把输出赋给变量
来源：http://rrb.chenjidiqi.icu

files=$(ls -1)
来源：http://cjz.hammf.cn

[R38] 管道串联
来源：http://kda.redwolf501.top

cat a.txt | grep -i error | wc -l
来源：http://yhs.fzhhl.top

[R39] 重定向标准输出与错误
来源：http://hnn.yj20258.top

cmd > out.log 2>&1
来源：http://syv.aizwys.cn

[R40] 追加写日志
来源：http://mph.ydjk.org.cn

echo "log" >> out.log
来源：http://erq.meibo888.top

[R41] 丢弃输出
来源：http://twj.ppjwa.cn

cmd >/dev/null 2>&1
来源：http://apu.dashuyun.cn

[R42] 输入重定向
来源：http://tzm.kuanghao11.cn

wc -l < a.txt
来源：http://sbw.yongpay.top

[R43] 按名字查找文件
来源：http://pbl.svipenyu.cn

find . -name "*.log" -type f
来源：http://zpi.zhoulong.xyz

[R44] 按修改时间查找
来源：http://ijc.shangyingyoupin.top

find . -mtime -7 -type f
来源：http://jbi.ctjpmb.com

[R45] 批量删除
来源：http://rce.sufxvd.cn

find . -name "*.tmp" -delete
来源：http://wwd.guowangkeji.top

[R46] 递归替换文件内容
来源：http://plc.xziqi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ffm.sysykeji.top

[R47] sed 单行替换
来源：http://rgo.xuanzx.com

sed -i 's/foo/bar/g' a.txt
来源：http://pqv.shanyushiyangkeji.top

[R48] awk 取指定列
来源：http://unk.jinqigfzy.top

awk '{print $1, $3}' a.txt
来源：http://btu.wangshuangyany.cn

[R49] awk 带条件
来源：http://nyz.gzhubu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bko.ywan-chungtsiang.top

[R50] awk 求和
来源：http://tte.smart0.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://gbp.ehwqpu.com

[R51] 排序去重取前几
来源：http://ivd.bbcook.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zyx.ybcxt.top

[R52] 统计行数
来源：http://ugw.mhx1999.top

wc -l a.txt
来源：http://zxy.xingfuxueyuan.xyz

[R53] 查看文件头与实时尾
来源：http://gdp.ywan-chungtsiang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pxx.meibo888.top

[R54] 比较两个文件
来源：http://yml.sxryk.cn

diff a.txt b.txt
来源：http://zud.sjlbkw.cn

[R55] 压缩与解压
来源：http://tfl.guowangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uip.ybcxt.top

[R56] 远程拷贝
来源：http://eeq.0kj1m.cn

scp file user@host:/path/
来源：http://pil.shangyingyoupin.top

[R57] 远程执行命令
来源：http://nno.pengpengdd.cyou

ssh user@host 'uptime'
来源：http://whh.ydjk.org.cn

[R58] 下载文件
来源：http://vtk.xingfuxueyuan.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sgq.pengpengdd.cyou

[R59] 发 POST JSON
来源：http://tum.cqqwz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ubf.nwbrower.top

[R60] 只看 HTTP 状态码
来源：http://hle.wangshuangyany.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xvy.sxryk.cn

[R61] 磁盘占用
来源：http://wil.iojbl.cn

df -h;  du -sh *
来源：http://cig.yj20258.top

[R62] 找最占空间的文件
来源：http://ros.andypj.xyz

du -ah . | sort -rh | head -10
来源：http://qku.havefunace.top

[R63] 内存与进程
来源：http://ymv.zhixingplan.top

free -h;  ps aux | grep nginx
来源：http://fiy.andypj.xyz

[R64] 结束进程
来源：http://qpa.c1oappe.top

kill -9 $(pgrep -f app.py)
来源：http://lhw.fzhhl.top

[R65] 查看端口占用
来源：http://vgr.zdqjudy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xfb.0kj1m.cn

[R66] 定时任务
来源：http://rqa.meibo888.top

crontab -e;  crontab -l
来源：http://knw.xingfuxueyuan.xyz

[R67] 生成随机十六进制串
来源：http://aie.0kj1m.cn

openssl rand -hex 16
来源：http://ozx.yongpay.top

[R68] 计算文件校验值
来源：http://iwc.fzhhl.top

sha256sum a.txt;  md5sum a.txt
来源：http://vnu.jqgufenzy.top

[R69] 生成随机密码
来源：http://hid.gogol.net.cn

head -c 16 /dev/urandom | base64
来源：http://qra.pengpengdd.cyou

[R70] 时间戳与互转
来源：http://jng.bbcook.cn

date +%s;  date -d @1700000000
来源：http://bex.ehwqpu.com

[R71] 日期格式化
来源：http://jjr.snrcjt.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dgx.aibaodan.cn

[R72] 等待端口就绪
来源：http://coo.jinqigufen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://gdl.0kj1m.cn

[R73] 分割大日志
来源：http://emn.52xcode.cn

split -l 1000 big.log part_
来源：http://ims.ehwqpu.com

[R74] 批量重命名
来源：http://lsy.yj20258888.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yzg.yueranfly.top

[R75] 导出环境变量
来源：http://umj.shzxlz.cn

export PATH="$HOME/bin:$PATH"
来源：http://pjj.9152youxi.cn

[R76] 使用临时文件
来源：http://qyb.bjfxy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bad.quarkkingdee.top

[R77] 读取用户输入
来源：http://rfu.wangshuangyany.cn

read -rp "请输入: " ans
来源：http://esw.feifeiyinyue.top

[R78] 交互式菜单
来源：http://uua.cucudq.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wup.zdbjq.cn

[R79] 解析命令行选项
来源：http://kqj.ctjpmb.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://doy.gaohongyu789.top

[R80] 查看脚本执行耗时
来源：http://ffj.zhoulong.xyz

time ./run.sh
来源：http://keh.epnwcf.com

================================================================================
来源：http://gvh.vqdsnc.cn

S. C / C++ 专题
来源：http://iwd.xylfe.cn

================================================================================
来源：http://pal.zhijiandao.cn

[S01] C：Hello World
来源：http://xfa.shuidangran.top

#include <stdio.h>
来源：http://jai.zdbjq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hqv.jqgfzy.top

[S02] C：变量与格式化输出
来源：http://xjm.snrcjt.cn

int a = 10; printf("%d\n", a);
来源：http://bgd.shzxlz.cn

[S03] C：读入整数
来源：http://lhp.kuanghao11.cn

int x; scanf("%d", &x);
来源：http://wey.daxiang520.top

[S04] C：字符串复制
来源：http://aip.ybcxt.top

char dst[32]; strcpy(dst, "hi");
来源：http://yyp.jinyuanbaomall.cn

[S05] C：字符串长度
来源：http://gkn.daxiang520.top

strlen(s)
来源：http://mjx.vehdjk.com

[S06] C：字符串比较
来源：http://eew.jyoumei.cn

strcmp(a, b) == 0
来源：http://fxv.birdmap.top

[S07] C：数组遍历求和
来源：http://syj.52xcode.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iia.tian-w.cn

[S08] C：动态内存分配与释放
来源：http://bqc.uphjek.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hfv.vehdjk.com

[S09] C：结构体定义与初始化
来源：http://cft.gotoacloud.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ncv.hongshengwenyu.top

[S10] C：指针与解引用
来源：http://nvv.hnqzz.top

int *p = &a;  *p = 5;
来源：http://vwm.ydzc1.top

[S11] C：逐行读文件
来源：http://zqo.xziqi.cn

FILE *f = fopen("a.txt", "r");
来源：http://upi.pengpengdd.cyou

while (fgets(buf, sizeof buf, f)) { }
来源：http://jce.vehdjk.com

fclose(f);
来源：http://ied.chenlongwang.top

[S12] C：写文件
来源：http://ben.nanxuanxn.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ibo.shanyushiyangkeji.top

[S13] C：宏定义
来源：http://tev.chenjidiqi.icu

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cun.nanxuanxn.top

[S14] C：枚举
来源：http://qfc.jqgufenzy.top

enum Color { RED, GREEN, BLUE };
来源：http://smy.jlsjyb.cn

[S15] C：类型转换
来源：http://kph.kuanghao11.cn

(double) a / b
来源：http://nfe.hysaishi.cn

[S16] C：位操作置位
来源：http://imj.chenjidiqi.icu

x |= (1 << 3);
来源：http://cux.redwolf501.top

[S17] C：安全拼接字符串
来源：http://tpr.sjlbkw.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sjf.xziqi.cn

[S18] C：命令行参数
来源：http://xel.pengpengdd.cyou

int main(int argc, char **argv)
来源：http://zxi.yj20258888.top

[S19] C：快速排序
来源：http://lnj.yangfankeji.com

qsort(a, n, sizeof(int), cmp);
来源：http://hmf.zhongyouzk.top

[S20] C：二分查找
来源：http://ozy.jyoumei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ayp.snrcjt.cn

[S21] C：字符类别判断
来源：http://gvo.haohaochexian.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zfc.zhijiandao.cn

[S22] C：字符串转数字
来源：http://nfv.shuidangran.top

atoi("42");  strtod("3.14", NULL);
来源：http://dfj.fehbvm.com

[S23] C：随机数
来源：http://bow.gotoacloud.top

srand(time(NULL));  int r = rand() % 100;
来源：http://jjb.gaohongyu789.top

[S24] C：获取本地时间
来源：http://hzw.zhongyouzk.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nmr.fehbvm.com

[S25] C：内存拷贝
来源：http://cna.chenlongwang.top

memcpy(dst, src, n);
来源：http://eot.ydjk.org.cn

[S26] C：内存清零
来源：http://vkj.jianghu66.top

memset(a, 0, sizeof a);
来源：http://rbk.cashguo.top

[S27] C：定义常量
来源：http://ygz.zdbjq.cn

const double PI = 3.14159;
来源：http://cyw.tianlin.xyz

[S28] C：静态变量
来源：http://dqj.xuetiantiany.cn

static int counter = 0;
来源：http://tom.yuanzhike.top

[S29] C：变参函数
来源：http://huq.redwolf501.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yww.jiagoushi.top

[S30] C：头文件保护
来源：http://mnd.tarul.cn

#ifndef X_H
来源：http://dgh.tian-w.cn

#define X_H
来源：http://mmn.hcnkem.com

#endif
来源：http://ddi.ivvv.top

[S31] C++：Hello World
来源：http://rmv.havefunace.top

#include <iostream>
来源：http://baa.guowangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://uft.jinghuilouyu.cn

[S32] C++：字符串
来源：http://pri.chenzaomai.com

std::string s = "hi";  s += "!";
来源：http://zmr.pengpengdd.cyou

[S33] C++：vector 增删
来源：http://hjq.snrcjt.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uji.jianghu66.top

[S34] C++：遍历 vector
来源：http://kzb.ydjk.org.cn

for (auto &x : v) { std::cout << x; }
来源：http://tdq.shzxlz.cn

[S35] C++：map
来源：http://ucp.jinyuanbaomall.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oya.shzxlz.cn

[S36] C++：unordered_map
来源：http://gel.zhongyouzk.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vfx.cashguo.top

[S37] C++：set
来源：http://vgy.hywenlv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zjb.sjlbkw.cn

[S38] C++：排序
来源：http://bnk.hywenlv.cn

std::sort(v.begin(), v.end());
来源：http://slw.epnwcf.com

[S39] C++：自定义比较器排序
来源：http://pir.meibo888.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ozn.birdmap.top

[S40] C++：查找元素
来源：http://rri.jianghu66.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ojn.jyoumei.cn

[S41] C++：类与构造函数
来源：http://dzm.chenjidiqi.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pze.jianghu66.top

[S42] C++：继承与虚函数
来源：http://rmm.iojbl.cn

class B : public Base { public: void f() override {} };
来源：http://gew.fzhhl.top

[S43] C++：智能指针
来源：http://fvm.sufxvd.cn

auto p = std::make_unique<int>(5);
来源：http://qvm.nanxuanxn.top

[S44] C++：引用传参
来源：http://znu.zdqjudy.top

void inc(int &x) { ++x; }
来源：http://ddv.yj20258888.top

[S45] C++：lambda
来源：http://vld.zhongyouzk.top

auto add = [](int a, int b) { return a + b; };
来源：http://sfo.yj202588.top

[S46] C++：函数模板
来源：http://tzd.hesvh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bir.nwbrower.top

[S47] C++：结构化绑定遍历
来源：http://pzh.shuidangran.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vvh.jqgfzy.top

[S48] C++：逐行读文件
来源：http://wnx.sufxvd.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zwp.jinqigufen.top

while (std::getline(in, line)) { }
来源：http://aez.yuxming.cn

[S49] C++：写文件
来源：http://fly.ydjk.org.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ecd.nanxuanxn.top

[S50] C++：格式化数字
来源：http://tpv.haohaochexian.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://smn.zdbjq.cn

[S51] C++：显式类型转换
来源：http://ubb.cucudq.cn

static_cast<double>(a) / b
来源：http://mzu.birdmap.top

[S52] C++：const 与 noexcept
来源：http://wly.yueranfly.top

int size() const noexcept { return n_; }
来源：http://sep.jqgufenzy.top

[S53] C++：移动语义
来源：http://ixz.yanxiufei.cn

std::vector<int> w = std::move(v);
来源：http://ywj.yvedp.cn

[S54] C++：异常处理
来源：http://bfn.zdbjq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ucc.zdbjq.cn

[S55] C++：结构化绑定
来源：http://qdr.haohaochexian.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ddo.zhaomingkeji.xyz

[S56] C++：optional
来源：http://edm.nwbrower.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yfc.yj20258888.top

[S57] C++：编译期常量
来源：http://dya.pengpengdd.cyou

constexpr int N = 10;
来源：http://glh.daria6918.cn

[S58] C++：命名空间
来源：http://lgi.hongshengwenyu.top

namespace ns { int f() { return 1; } }
来源：http://axy.yuxming.cn

[S59] C++：静态断言
来源：http://mku.birdmap.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gyp.52xcode.cn

[S60] C++：遍历并删除元素
来源：http://fjt.iojbl.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fgd.yj202588.top

================================================================================
来源：http://cwx.vehdjk.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wdj.ppjwa.cn

================================================================================
来源：http://khz.uphjek.com

[T01] Kotlin：Hello World
来源：http://tda.hcnkem.com

println("Hello")
来源：http://mmf.shuidangran.top

[T02] Kotlin：变量
来源：http://yxx.yuanzhike.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ufn.kuanghao11.cn

[T03] Kotlin：字符串模板
来源：http://oxs.daria6918.cn

"值: $b"
来源：http://pdq.fehbvm.com

[T04] Kotlin：空安全
来源：http://jae.iojbl.cn

val n: String? = null;  n?.length
来源：http://gcs.dianchejie.cn

[T05] Kotlin：when 表达式
来源：http://xon.zycfv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pxc.hammf.cn

[T06] Kotlin：集合映射
来源：http://euk.ydjk.org.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jpv.birdmap.top

[T07] Kotlin：集合过滤
来源：http://tha.ybcxt.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xgb.dianchejie.cn

[T08] Kotlin：数据类
来源：http://xey.ehwqpu.com

data class User(val name: String, val age: Int)
来源：http://jyy.sysykeji.top

[T09] Kotlin：扩展函数
来源：http://gpx.redwolf501.top

fun String.exclaim() = this + "!"
来源：http://lcy.gogol.net.cn

[T10] Kotlin：默认参数
来源：http://mlw.ppjwa.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jzo.jinghuilouyu.cn

[T11] Kotlin：协程
来源：http://xti.tian-w.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wio.yuxming.cn

[T12] Kotlin：解构声明
来源：http://fef.havefunace.top

val (a, b) = Pair(1, 2)
来源：http://fvc.hcnkem.com

[T13] Kotlin：只读 Map
来源：http://rbv.epnwcf.com

val m = mapOf("a" to 1)
来源：http://bwf.gogol.net.cn

[T14] Kotlin：循环
来源：http://wau.ctjpmb.com

for (i in 1..10) println(i)
来源：http://jch.jianghu66.top

[T15] Kotlin：接口
来源：http://vjc.smart0.xyz

interface Shape { fun area(): Double }
来源：http://vcj.dashuyun.cn

[T16] Swift：Hello World
来源：http://zat.pengpengdd.cyou

print("Hello")
来源：http://fky.chenlongwang.top

[T17] Swift：变量与常量
来源：http://qhu.zhijiandao.cn

var a = 1;  let b = 2
来源：http://txl.jianghu66.top

[T18] Swift：字符串插值
来源：http://wcl.nanxinkj.top

"值: \(b)"
来源：http://pmm.fktsv.cn

[T19] Swift：可选绑定
来源：http://asc.hnxiangtu.top

if let n = opt { print(n) }
来源：http://qsu.sufxvd.cn

[T20] Swift：数组操作
来源：http://hcj.epnwcf.com

var a = [1, 2, 3];  a.append(4)
来源：http://zni.hfpthk.cn

[T21] Swift：遍历
来源：http://gsv.cqqwz.cn

for x in a { print(x) }
来源：http://xro.haohaochexian.top

[T22] Swift：字典
来源：http://fkv.wangshuangyany.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vml.gotoacloud.top


<!-- 参考信息 -->