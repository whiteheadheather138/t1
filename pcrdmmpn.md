代发 wailian999

echo "${#s}"
来源：http://csl.tian-w.cn

[R22] 截取子串
来源：http://hnu.shanyushiyangkeji.top

echo "${s:0:5}"
来源：http://yvz.316326.xyz

[R23] 字符串替换
来源：http://zip.yuxming.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uno.bbcook.cn

[R24] 大小写转换
来源：http://gnw.jiagoushi.top

echo "${s^^}"; echo "${s,,}"
来源：http://yik.yanxiufei.cn

[R25] 去后缀 / 去前缀
来源：http://gvz.uphjek.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://lkm.ppjwa.cn

[R26] 命令替换
来源：http://ytu.zycfv.cn

now=$(date +%F); echo "$now"
来源：http://kya.gogol.net.cn

[R27] 算术展开
来源：http://qhl.ivvv.top

echo $((1 + 2 * 3))
来源：http://usz.haohaochexian.top

[R28] 浮点运算
来源：http://syh.ehwqpu.com

echo "scale=2; 10/3" | bc
来源：http://pyz.xinyue.icu

[R29] 定义函数
来源：http://tpr.wangshuangyany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wav.zdqjudy.top

[R30] 函数返回状态码
来源：http://pim.jqgufenzy.top

f() { return 0; }; f || echo "失败了"
来源：http://pfd.hfpthk.cn

[R31] 局部变量
来源：http://pac.yuanzhike.top

f() { local x=1; echo "$x"; }
来源：http://bod.zhoulong.xyz

[R32] 参数个数校验
来源：http://czj.yueranfly.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fym.cheryme.top

[R33] 捕获错误并提示行号
来源：http://fnu.yongpay.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nmu.gotoacloud.top

[R34] 退出时清理
来源：http://atu.shzxlz.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bfc.zhaomingkeji.xyz

[R35] 后台执行并等待
来源：http://ijc.0kj1m.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://uyl.sjlbkw.cn

[R36] 并发执行多个任务
来源：http://mxr.yanxiufei.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xkk.yj20258888.top

[R37] 把输出赋给变量
来源：http://yjv.quarkkingdee.top

files=$(ls -1)
来源：http://djj.zycfv.cn

[R38] 管道串联
来源：http://zcn.zdbjq.cn

cat a.txt | grep -i error | wc -l
来源：http://tva.xinyue.icu

[R39] 重定向标准输出与错误
来源：http://skl.fktsv.cn

cmd > out.log 2>&1
来源：http://ckj.shanyushiyangkeji.top

[R40] 追加写日志
来源：http://kab.svipenyu.cn

echo "log" >> out.log
来源：http://hqs.wangshuangyany.cn

[R41] 丢弃输出
来源：http://cua.hywenlv.cn

cmd >/dev/null 2>&1
来源：http://kjb.nanxuanxn.top

[R42] 输入重定向
来源：http://lth.shzxlz.cn

wc -l < a.txt
来源：http://vxv.wangshuangyany.cn

[R43] 按名字查找文件
来源：http://grm.tianlin.xyz

find . -name "*.log" -type f
来源：http://txt.svipenyu.cn

[R44] 按修改时间查找
来源：http://koc.ywan-chungtsiang.top

find . -mtime -7 -type f
来源：http://oba.uphjek.com

[R45] 批量删除
来源：http://tqa.sysykeji.top

find . -name "*.tmp" -delete
来源：http://yqe.hywenlv.cn

[R46] 递归替换文件内容
来源：http://lfx.fehbvm.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://aeb.yvedp.cn

[R47] sed 单行替换
来源：http://kmi.daria6918.cn

sed -i 's/foo/bar/g' a.txt
来源：http://axp.fehbvm.com

[R48] awk 取指定列
来源：http://gge.yanxiufei.cn

awk '{print $1, $3}' a.txt
来源：http://vll.chenzaomai.com

[R49] awk 带条件
来源：http://dzs.chenzaomai.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wvl.316326.xyz

[R50] awk 求和
来源：http://dly.zhengqikj.top

awk '{s += $2} END {print s}' a.txt
来源：http://bbw.zhiwuduotai.top

[R51] 排序去重取前几
来源：http://fos.hesvh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vmc.tianlin.xyz

[R52] 统计行数
来源：http://lfu.jinghuilouyu.cn

wc -l a.txt
来源：http://iir.jqgufenzy.top

[R53] 查看文件头与实时尾
来源：http://mwb.meibo888.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zma.wangdashe.top

[R54] 比较两个文件
来源：http://xgt.zhongyouzk.top

diff a.txt b.txt
来源：http://icm.jqgufenzy.top

[R55] 压缩与解压
来源：http://wyf.bjfxy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kmh.zdbjq.cn

[R56] 远程拷贝
来源：http://kfr.zhaomingkeji.xyz

scp file user@host:/path/
来源：http://cmc.jyoumei.cn

[R57] 远程执行命令
来源：http://bie.pengpengdd.cyou

ssh user@host 'uptime'
来源：http://dzt.dashuyun.cn

[R58] 下载文件
来源：http://cyc.gogol.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oxj.yvedp.cn

[R59] 发 POST JSON
来源：http://nwb.epnwcf.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yvx.sysykeji.top

[R60] 只看 HTTP 状态码
来源：http://nlf.dashuyun.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jvj.chenlongwang.top

[R61] 磁盘占用
来源：http://cyb.kuanghao11.cn

df -h;  du -sh *
来源：http://bzk.kuanghao11.cn

[R62] 找最占空间的文件
来源：http://hto.redwolf501.top

du -ah . | sort -rh | head -10
来源：http://kqg.birdmap.top

[R63] 内存与进程
来源：http://hgp.aizwys.cn

free -h;  ps aux | grep nginx
来源：http://bhq.ybcxt.top

[R64] 结束进程
来源：http://wzw.cdnleiting.top

kill -9 $(pgrep -f app.py)
来源：http://bgs.ivvv.top

[R65] 查看端口占用
来源：http://swp.zhijiandao.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nip.fanxiaobao.xyz

[R66] 定时任务
来源：http://pja.shzxlz.cn

crontab -e;  crontab -l
来源：http://qwi.zhaomingkeji.xyz

[R67] 生成随机十六进制串
来源：http://pah.yonumen.top

openssl rand -hex 16
来源：http://dpg.yangfankeji.com

[R68] 计算文件校验值
来源：http://cnq.bbcook.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ugr.cashguo.top

[R69] 生成随机密码
来源：http://rtp.cdnleiting.top

head -c 16 /dev/urandom | base64
来源：http://axo.smart0.xyz

[R70] 时间戳与互转
来源：http://oqf.ehwqpu.com

date +%s;  date -d @1700000000
来源：http://eaf.havefunace.top

[R71] 日期格式化
来源：http://gck.jinqigufen.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://cdw.guannengcc.top

[R72] 等待端口就绪
来源：http://tzp.yj20258888.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ybx.ehwqpu.com

[R73] 分割大日志
来源：http://awo.bjfxy.top

split -l 1000 big.log part_
来源：http://xkp.xinyue.icu

[R74] 批量重命名
来源：http://nwd.nwbrower.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qmn.fzhhl.top

[R75] 导出环境变量
来源：http://cil.0kj1m.cn

export PATH="$HOME/bin:$PATH"
来源：http://bwp.feifeiyinyue.top

[R76] 使用临时文件
来源：http://azl.yfazqb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://een.iojbl.cn

[R77] 读取用户输入
来源：http://kdu.uphjek.com

read -rp "请输入: " ans
来源：http://wlx.haohaochexian.top

[R78] 交互式菜单
来源：http://xhz.mhx1999.top

select opt in a b c; do echo "$opt"; break; done
来源：http://gaf.vehdjk.com

[R79] 解析命令行选项
来源：http://rjy.quarkkingdee.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ufw.vqdsnc.cn

[R80] 查看脚本执行耗时
来源：http://nxs.ivvv.top

time ./run.sh
来源：http://pth.316326.xyz

================================================================================
来源：http://pez.jqgufenzy.top

S. C / C++ 专题
来源：http://vza.cucudq.cn

================================================================================
来源：http://qab.wangshuangyany.cn

[S01] C：Hello World
来源：http://xom.ybcxt.top

#include <stdio.h>
来源：http://tdg.yj20258888.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://aul.meibo888.top

[S02] C：变量与格式化输出
来源：http://uxd.hywenlv.cn

int a = 10; printf("%d\n", a);
来源：http://lub.yangfankeji.com

[S03] C：读入整数
来源：http://nkn.yongpay.top

int x; scanf("%d", &x);
来源：http://fon.chenlongwang.top

[S04] C：字符串复制
来源：http://ikh.cheryme.top

char dst[32]; strcpy(dst, "hi");
来源：http://duh.fehbvm.com

[S05] C：字符串长度
来源：http://aia.yj202588.top

strlen(s)
来源：http://vmf.svipenyu.cn

[S06] C：字符串比较
来源：http://ral.fzhhl.top

strcmp(a, b) == 0
来源：http://yav.shangyingyoupin.top

[S07] C：数组遍历求和
来源：http://iag.tian-w.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://byq.hywenlv.cn

[S08] C：动态内存分配与释放
来源：http://czj.xuetiantiany.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://abx.fehbvm.com

[S09] C：结构体定义与初始化
来源：http://yyy.gogol.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uqm.aizwys.cn

[S10] C：指针与解引用
来源：http://zqz.zhiwuduotai.top

int *p = &a;  *p = 5;
来源：http://yvy.aibaodan.cn

[S11] C：逐行读文件
来源：http://hhq.zhoulong.xyz

FILE *f = fopen("a.txt", "r");
来源：http://bsr.nanxinkj.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://zve.fzhhl.top

fclose(f);
来源：http://jcc.nanxinkj.top

[S12] C：写文件
来源：http://yhk.svipenyu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yxc.yangfankeji.com

[S13] C：宏定义
来源：http://suk.yueranfly.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hwq.hysaishi.cn

[S14] C：枚举
来源：http://uwd.jiagoushi.top

enum Color { RED, GREEN, BLUE };
来源：http://kji.yuxming.cn

[S15] C：类型转换
来源：http://gvr.gzhubu.top

(double) a / b
来源：http://gag.fzhhl.top

[S16] C：位操作置位
来源：http://rou.hammf.cn

x |= (1 << 3);
来源：http://awp.xziqi.cn

[S17] C：安全拼接字符串
来源：http://wik.epnwcf.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kfe.xuetiantiany.cn

[S18] C：命令行参数
来源：http://sbs.smart0.xyz

int main(int argc, char **argv)
来源：http://geu.zdqjudy.top

[S19] C：快速排序
来源：http://lxq.ydzc1.top

qsort(a, n, sizeof(int), cmp);
来源：http://ilw.kuanghao11.cn

[S20] C：二分查找
来源：http://ewh.smart0.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hch.52xcode.cn

[S21] C：字符类别判断
来源：http://nqp.zdqjudy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://amj.zycfv.cn

[S22] C：字符串转数字
来源：http://hyw.zhengqikj.top

atoi("42");  strtod("3.14", NULL);
来源：http://tqj.0kj1m.cn

[S23] C：随机数
来源：http://jgl.yanxiufei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rfb.hcnkem.com

[S24] C：获取本地时间
来源：http://zql.gotoacloud.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ulp.cheryme.top

[S25] C：内存拷贝
来源：http://tri.hnqzz.top

memcpy(dst, src, n);
来源：http://adk.jinqigufen.top

[S26] C：内存清零
来源：http://cnt.ydjk.org.cn

memset(a, 0, sizeof a);
来源：http://pbc.chenjidiqi.icu

[S27] C：定义常量
来源：http://smz.xuetiantiany.cn

const double PI = 3.14159;
来源：http://ewr.jinyuanbaomall.cn

[S28] C：静态变量
来源：http://sxk.cashguo.top

static int counter = 0;
来源：http://xxk.jinyuanbaomall.cn

[S29] C：变参函数
来源：http://hfq.hesvh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hfr.birdmap.top

[S30] C：头文件保护
来源：http://mvx.hcnkem.com

#ifndef X_H
来源：http://kth.quarkkingdee.top

#define X_H
来源：http://oxq.zycfv.cn

#endif
来源：http://xwv.tian-w.cn

[S31] C++：Hello World
来源：http://oja.ywan-chungtsiang.top

#include <iostream>
来源：http://lft.birdmap.top

int main() { std::cout << "Hello\n"; }
来源：http://yvw.bbcook.cn

[S32] C++：字符串
来源：http://szy.dianchejie.cn

std::string s = "hi";  s += "!";
来源：http://oww.chenlongwang.top

[S33] C++：vector 增删
来源：http://vph.gotoacloud.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kfi.jqgfzy.top

[S34] C++：遍历 vector
来源：http://gmi.shuidangran.top

for (auto &x : v) { std::cout << x; }
来源：http://mgn.ivvv.top

[S35] C++：map
来源：http://vdj.fehbvm.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wnx.yongpay.top

[S36] C++：unordered_map
来源：http://mye.smart0.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nil.zhixingplan.top

[S37] C++：set
来源：http://ulz.xuanzx.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ben.hfpthk.cn

[S38] C++：排序
来源：http://fzy.shuidangran.top

std::sort(v.begin(), v.end());
来源：http://baf.chenlongwang.top

[S39] C++：自定义比较器排序
来源：http://dfd.bjfxy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qtb.ydzc1.top

[S40] C++：查找元素
来源：http://kdt.shanyushiyangkeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://roy.yfazqb.com

[S41] C++：类与构造函数
来源：http://bvx.yonumen.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kby.pycfn.com

[S42] C++：继承与虚函数
来源：http://ugl.dashuyun.cn

class B : public Base { public: void f() override {} };
来源：http://riv.ehwqpu.com

[S43] C++：智能指针
来源：http://int.yonumen.top

auto p = std::make_unique<int>(5);
来源：http://ttu.bjfxy.top

[S44] C++：引用传参
来源：http://ciu.hnqzz.top

void inc(int &x) { ++x; }
来源：http://nys.fktsv.cn

[S45] C++：lambda
来源：http://dmy.zdqjudy.top

auto add = [](int a, int b) { return a + b; };
来源：http://els.bjfxy.top

[S46] C++：函数模板
来源：http://tfn.havefunace.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jvp.zhijiandao.cn

[S47] C++：结构化绑定遍历
来源：http://wht.hywenlv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ipy.aibaodan.cn

[S48] C++：逐行读文件
来源：http://ebm.yueranfly.top

std::ifstream in("a.txt");  std::string line;
来源：http://exi.feifeiyinyue.top

while (std::getline(in, line)) { }
来源：http://rhz.smart0.xyz

[S49] C++：写文件
来源：http://wbm.chenzaomai.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rzo.uphjek.com

[S50] C++：格式化数字
来源：http://kbp.sysykeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eym.havefunace.top

[S51] C++：显式类型转换
来源：http://nou.hfpthk.cn

static_cast<double>(a) / b
来源：http://oeu.redwolf501.top

[S52] C++：const 与 noexcept
来源：http://kcv.zdbjq.cn

int size() const noexcept { return n_; }
来源：http://qnd.yonumen.top

[S53] C++：移动语义
来源：http://xfb.feifeiyinyue.top

std::vector<int> w = std::move(v);
来源：http://alw.yonumen.top

[S54] C++：异常处理
来源：http://asq.jqgufenzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tbb.jinyuanbaomall.cn

[S55] C++：结构化绑定
来源：http://yxo.hfpthk.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kfy.316326.xyz

[S56] C++：optional
来源：http://aay.zhixingplan.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tew.sufxvd.cn

[S57] C++：编译期常量
来源：http://gnt.hnqzz.top

constexpr int N = 10;
来源：http://uoh.vehdjk.com

[S58] C++：命名空间
来源：http://kad.shanyushiyangtech.top

namespace ns { int f() { return 1; } }
来源：http://mwg.hywenlv.cn

[S59] C++：静态断言
来源：http://fnc.daria6918.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ztu.fktsv.cn

[S60] C++：遍历并删除元素
来源：http://asl.zhoulong.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ndt.hnxiangtu.top

================================================================================
来源：http://exx.hnqzz.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lwy.jqgufenzy.top

================================================================================
来源：http://ewo.redwolf501.top

[T01] Kotlin：Hello World
来源：http://vfn.ywan-chungtsiang.top

println("Hello")
来源：http://lxd.vehdjk.com

[T02] Kotlin：变量
来源：http://bhr.xylfe.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tez.fehbvm.com

[T03] Kotlin：字符串模板
来源：http://cmo.snrcjt.cn

"值: $b"
来源：http://xfs.c1oappe.top

[T04] Kotlin：空安全
来源：http://tix.hnqzz.top

val n: String? = null;  n?.length
来源：http://dcw.birdmap.top

[T05] Kotlin：when 表达式
来源：http://xsp.haohaochexian.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fln.zhongyouzk.top

[T06] Kotlin：集合映射
来源：http://jvp.c1oappe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://kcn.ywan-chungtsiang.top

[T07] Kotlin：集合过滤
来源：http://xmb.zhoulong.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://jlq.shanyushiyangkeji.top

[T08] Kotlin：数据类
来源：http://hkv.ppjwa.cn

data class User(val name: String, val age: Int)
来源：http://iau.tian-w.cn

[T09] Kotlin：扩展函数
来源：http://djm.meibo888.top

fun String.exclaim() = this + "!"
来源：http://bxh.cashguo.top

[T10] Kotlin：默认参数
来源：http://ovm.ybcxt.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wzg.yj20258888.top

[T11] Kotlin：协程
来源：http://zka.haohaochexian.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://uum.yonumen.top

[T12] Kotlin：解构声明
来源：http://eui.iojbl.cn

val (a, b) = Pair(1, 2)
来源：http://nhm.xziqi.cn

[T13] Kotlin：只读 Map
来源：http://vup.zhongyouzk.top

val m = mapOf("a" to 1)
来源：http://vpg.shzxlz.cn

[T14] Kotlin：循环
来源：http://nkr.52xcode.cn

for (i in 1..10) println(i)
来源：http://jhj.dianchejie.cn

[T15] Kotlin：接口
来源：http://drt.sufxvd.cn

interface Shape { fun area(): Double }
来源：http://vud.guowangkeji.top

[T16] Swift：Hello World
来源：http://lib.haohaochexian.top

print("Hello")
来源：http://uly.yj202588.top

[T17] Swift：变量与常量
来源：http://tjb.cheryme.top

var a = 1;  let b = 2
来源：http://wtn.tianlin.xyz

[T18] Swift：字符串插值
来源：http://hdt.hnxiangtu.top

"值: \(b)"
来源：http://wvl.uphjek.com

[T19] Swift：可选绑定
来源：http://xwf.shzxlz.cn

if let n = opt { print(n) }
来源：http://urx.xinyue.icu

[T20] Swift：数组操作
来源：http://xth.aibaodan.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jti.fzhhl.top

[T21] Swift：遍历
来源：http://snf.gaohongyu789.top

for x in a { print(x) }
来源：http://erx.daxiang520.top

[T22] Swift：字典
来源：http://zsj.dashuyun.cn

var d = ["a": 1];  d["b"] = 2
来源：http://aon.gogol.net.cn

[T23] Swift：函数
来源：http://lim.zhongyouzk.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tge.jyoumei.cn

[T24] Swift：闭包
来源：http://ftu.epnwcf.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://eyn.316326.xyz


<!-- 参考信息 -->