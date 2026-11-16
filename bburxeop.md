代发 wailian999

echo "${#arr[@]}"
来源：http://ufb.c1oappe.top

[R20] 关联数组（字典）
来源：http://wwi.daria6918.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jcx.quarkkingdee.top

[R21] 字符串长度
来源：http://bwu.yonumen.top

echo "${#s}"
来源：http://lho.epnwcf.com

[R22] 截取子串
来源：http://zhc.snrcjt.cn

echo "${s:0:5}"
来源：http://udq.hesvh.cn

[R23] 字符串替换
来源：http://vzw.zhijiandao.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gav.svipenyu.cn

[R24] 大小写转换
来源：http://etw.dianchejie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qja.tianlin.xyz

[R25] 去后缀 / 去前缀
来源：http://dmq.xingfuxueyuan.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://jxe.0kj1m.cn

[R26] 命令替换
来源：http://pir.52xcode.cn

now=$(date +%F); echo "$now"
来源：http://wfb.aizwys.cn

[R27] 算术展开
来源：http://ynq.iojbl.cn

echo $((1 + 2 * 3))
来源：http://dgk.ivvv.top

[R28] 浮点运算
来源：http://qtb.wangshuangyany.cn

echo "scale=2; 10/3" | bc
来源：http://uhr.quarkkingdee.top

[R29] 定义函数
来源：http://sip.yvedp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xmf.dianchejie.cn

[R30] 函数返回状态码
来源：http://dsf.cucudq.cn

f() { return 0; }; f || echo "失败了"
来源：http://xhf.zdqjudy.top

[R31] 局部变量
来源：http://vad.uphjek.com

f() { local x=1; echo "$x"; }
来源：http://nfr.jiagoushi.top

[R32] 参数个数校验
来源：http://vwc.iojbl.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://usp.zhaomingkeji.xyz

[R33] 捕获错误并提示行号
来源：http://bhv.chenjidiqi.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://owi.quarkkingdee.top

[R34] 退出时清理
来源：http://iua.zdbjq.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dze.epnwcf.com

[R35] 后台执行并等待
来源：http://tyw.yongpay.top

sleep 5 & pid=$!; wait "$pid"
来源：http://zfk.cdnleiting.top

[R36] 并发执行多个任务
来源：http://hxs.pengpengdd.cyou

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jfi.kuanghao11.cn

[R37] 把输出赋给变量
来源：http://xbw.sxryk.cn

files=$(ls -1)
来源：http://shz.ywan-chungtsiang.top

[R38] 管道串联
来源：http://ycu.fanxiaobao.xyz

cat a.txt | grep -i error | wc -l
来源：http://bjv.ybcxt.top

[R39] 重定向标准输出与错误
来源：http://xiz.uphjek.com

cmd > out.log 2>&1
来源：http://gcu.yuxming.cn

[R40] 追加写日志
来源：http://etx.hammf.cn

echo "log" >> out.log
来源：http://ead.gzhubu.top

[R41] 丢弃输出
来源：http://wyo.zdqjudy.top

cmd >/dev/null 2>&1
来源：http://urn.havefunace.top

[R42] 输入重定向
来源：http://xwz.pengpengdd.cyou

wc -l < a.txt
来源：http://oiq.birdmap.top

[R43] 按名字查找文件
来源：http://reh.cqqwz.cn

find . -name "*.log" -type f
来源：http://igb.ctjpmb.com

[R44] 按修改时间查找
来源：http://zoa.fktsv.cn

find . -mtime -7 -type f
来源：http://olv.jinqigufen.top

[R45] 批量删除
来源：http://trh.jqgfzy.top

find . -name "*.tmp" -delete
来源：http://jmf.yonumen.top

[R46] 递归替换文件内容
来源：http://cdl.feifeiyinyue.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mpu.xuetiantiany.cn

[R47] sed 单行替换
来源：http://zha.jinghuilouyu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ptl.kuanghao11.cn

[R48] awk 取指定列
来源：http://ybl.pycfn.com

awk '{print $1, $3}' a.txt
来源：http://ckm.316326.xyz

[R49] awk 带条件
来源：http://end.jiagoushi.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rdq.zdqjudy.top

[R50] awk 求和
来源：http://zcy.gzhubu.top

awk '{s += $2} END {print s}' a.txt
来源：http://nfv.wangdashe.top

[R51] 排序去重取前几
来源：http://hya.vqdsnc.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vgz.yj20258888.top

[R52] 统计行数
来源：http://lhd.sjlbkw.cn

wc -l a.txt
来源：http://xsv.yuxming.cn

[R53] 查看文件头与实时尾
来源：http://sfy.ybcxt.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vdk.hnqzz.top

[R54] 比较两个文件
来源：http://irc.tianlin.xyz

diff a.txt b.txt
来源：http://jtz.haohaochexian.top

[R55] 压缩与解压
来源：http://wmg.0kj1m.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mdp.ivvv.top

[R56] 远程拷贝
来源：http://nvt.zhoulong.xyz

scp file user@host:/path/
来源：http://ybq.9152youxi.cn

[R57] 远程执行命令
来源：http://qqv.nanxinkj.top

ssh user@host 'uptime'
来源：http://xjq.birdmap.top

[R58] 下载文件
来源：http://kpf.jiagoushi.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ywx.jyoumei.cn

[R59] 发 POST JSON
来源：http://wzw.yfazqb.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tir.zhengqikj.top

[R60] 只看 HTTP 状态码
来源：http://xqh.yj20258.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dbc.shangyingyoupin.top

[R61] 磁盘占用
来源：http://ivy.shangyingyoupin.top

df -h;  du -sh *
来源：http://ghs.bbcook.cn

[R62] 找最占空间的文件
来源：http://udj.jyoumei.cn

du -ah . | sort -rh | head -10
来源：http://erl.dashuyun.cn

[R63] 内存与进程
来源：http://pxq.kuanghao11.cn

free -h;  ps aux | grep nginx
来源：http://unc.jianghu66.top

[R64] 结束进程
来源：http://cny.gogol.net.cn

kill -9 $(pgrep -f app.py)
来源：http://njy.c1oappe.top

[R65] 查看端口占用
来源：http://nux.tarul.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zxa.yonumen.top

[R66] 定时任务
来源：http://bgc.redwolf501.top

crontab -e;  crontab -l
来源：http://ynf.yueranfly.top

[R67] 生成随机十六进制串
来源：http://rrw.redwolf501.top

openssl rand -hex 16
来源：http://jqq.xziqi.cn

[R68] 计算文件校验值
来源：http://znv.jianghu66.top

sha256sum a.txt;  md5sum a.txt
来源：http://bdx.hesvh.cn

[R69] 生成随机密码
来源：http://ckk.52xcode.cn

head -c 16 /dev/urandom | base64
来源：http://rsl.fktsv.cn

[R70] 时间戳与互转
来源：http://qxs.fktsv.cn

date +%s;  date -d @1700000000
来源：http://cek.fehbvm.com

[R71] 日期格式化
来源：http://iux.shanyushiyangtech.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://fzb.hammf.cn

[R72] 等待端口就绪
来源：http://sbw.daxiang520.top

until nc -z localhost 3306; do sleep 1; done
来源：http://clj.vehdjk.com

[R73] 分割大日志
来源：http://lcp.havefunace.top

split -l 1000 big.log part_
来源：http://iuq.fanxiaobao.xyz

[R74] 批量重命名
来源：http://lkp.smart0.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://huu.pycfn.com

[R75] 导出环境变量
来源：http://sei.yongpay.top

export PATH="$HOME/bin:$PATH"
来源：http://yum.fktsv.cn

[R76] 使用临时文件
来源：http://gor.tanke756.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ayv.andypj.xyz

[R77] 读取用户输入
来源：http://oag.wangdashe.top

read -rp "请输入: " ans
来源：http://qjh.hfpthk.cn

[R78] 交互式菜单
来源：http://pof.tarul.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://iwx.guannengcc.top

[R79] 解析命令行选项
来源：http://hgc.shzxlz.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ydb.hfpthk.cn

[R80] 查看脚本执行耗时
来源：http://tka.hnqzz.top

time ./run.sh
来源：http://rvw.jiagoushi.top

================================================================================
来源：http://vdw.zhaomingkeji.xyz

S. C / C++ 专题
来源：http://zlb.vehdjk.com

================================================================================
来源：http://jfe.cashguo.top

[S01] C：Hello World
来源：http://vsi.yvedp.cn

#include <stdio.h>
来源：http://ukj.ywan-chungtsiang.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://but.gaohongyu789.top

[S02] C：变量与格式化输出
来源：http://lia.daria6918.cn

int a = 10; printf("%d\n", a);
来源：http://bol.jinyuanbaomall.cn

[S03] C：读入整数
来源：http://wsu.wangdashe.top

int x; scanf("%d", &x);
来源：http://bpi.shzxlz.cn

[S04] C：字符串复制
来源：http://nul.smart0.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://rfw.cqqwz.cn

[S05] C：字符串长度
来源：http://ntt.ydjk.org.cn

strlen(s)
来源：http://jno.zdbjq.cn

[S06] C：字符串比较
来源：http://fds.dashuyun.cn

strcmp(a, b) == 0
来源：http://tsi.nanxuanxn.top

[S07] C：数组遍历求和
来源：http://quz.quarkkingdee.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fma.jinqigfzy.top

[S08] C：动态内存分配与释放
来源：http://rni.yangfankeji.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hqy.zhixingplan.top

[S09] C：结构体定义与初始化
来源：http://qzy.redwolf501.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zck.shanyushiyangtech.top

[S10] C：指针与解引用
来源：http://vge.xuanzx.com

int *p = &a;  *p = 5;
来源：http://avd.yongpay.top

[S11] C：逐行读文件
来源：http://smn.yvedp.cn

FILE *f = fopen("a.txt", "r");
来源：http://nfm.316326.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://ylt.fanxiaobao.xyz

fclose(f);
来源：http://ztw.nanxuanxn.top

[S12] C：写文件
来源：http://gdv.jlsjyb.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xiu.hysaishi.cn

[S13] C：宏定义
来源：http://nyz.zycfv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lii.yj202588.top

[S14] C：枚举
来源：http://zih.vehdjk.com

enum Color { RED, GREEN, BLUE };
来源：http://qum.bbcook.cn

[S15] C：类型转换
来源：http://uoo.0kj1m.cn

(double) a / b
来源：http://tll.nanxuanxn.top

[S16] C：位操作置位
来源：http://yoc.jqgufenzy.top

x |= (1 << 3);
来源：http://lyd.hnqzz.top

[S17] C：安全拼接字符串
来源：http://mnv.yuanzhike.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ayn.zhengqikj.top

[S18] C：命令行参数
来源：http://wzg.9152youxi.cn

int main(int argc, char **argv)
来源：http://rld.jiagoushi.top

[S19] C：快速排序
来源：http://ilk.gotoacloud.top

qsort(a, n, sizeof(int), cmp);
来源：http://sgl.yuanzhike.top

[S20] C：二分查找
来源：http://mgy.bbcook.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zod.jiagoushi.top

[S21] C：字符类别判断
来源：http://gkz.chenjidiqi.icu

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zpg.kuanghao11.cn

[S22] C：字符串转数字
来源：http://vjv.shanyushiyangkeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://daw.bbcook.cn

[S23] C：随机数
来源：http://ise.kuanghao11.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rrr.hysaishi.cn

[S24] C：获取本地时间
来源：http://zoy.zhaomingkeji.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vjd.tian-w.cn

[S25] C：内存拷贝
来源：http://cwl.wangdashe.top

memcpy(dst, src, n);
来源：http://jau.vqdsnc.cn

[S26] C：内存清零
来源：http://lvc.yanxiufei.cn

memset(a, 0, sizeof a);
来源：http://vcd.jqgfzy.top

[S27] C：定义常量
来源：http://bzn.nanxuanxn.top

const double PI = 3.14159;
来源：http://ykm.haohaochexian.top

[S28] C：静态变量
来源：http://zyj.zdbjq.cn

static int counter = 0;
来源：http://awe.cheryme.top

[S29] C：变参函数
来源：http://cff.havefunace.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kab.nwbrower.top

[S30] C：头文件保护
来源：http://mdu.yj20258888.top

#ifndef X_H
来源：http://dtf.yangfankeji.com

#define X_H
来源：http://qxn.jinyuanbaomall.cn

#endif
来源：http://eax.jinyuanbaomall.cn

[S31] C++：Hello World
来源：http://ewi.0kj1m.cn

#include <iostream>
来源：http://lah.hongshengwenyu.top

int main() { std::cout << "Hello\n"; }
来源：http://pdk.yuxming.cn

[S32] C++：字符串
来源：http://ufj.wangshuangyany.cn

std::string s = "hi";  s += "!";
来源：http://wwl.gzhubu.top

[S33] C++：vector 增删
来源：http://pih.hnxiangtu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dyw.chenlongwang.top

[S34] C++：遍历 vector
来源：http://qrv.svipenyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://edd.tianlin.xyz

[S35] C++：map
来源：http://ntv.xuanzx.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pkk.xingfuxueyuan.xyz

[S36] C++：unordered_map
来源：http://ptn.jinqigfzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uha.hammf.cn

[S37] C++：set
来源：http://clt.ivvv.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://aaq.shanyushiyangtech.top

[S38] C++：排序
来源：http://rmj.yvedp.cn

std::sort(v.begin(), v.end());
来源：http://tbf.aizwys.cn

[S39] C++：自定义比较器排序
来源：http://txq.aibaodan.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vod.cucudq.cn

[S40] C++：查找元素
来源：http://uen.zycfv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://heh.shanyushiyangtech.top

[S41] C++：类与构造函数
来源：http://znp.hysaishi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://usw.fanxiaobao.xyz

[S42] C++：继承与虚函数
来源：http://mrj.hcnkem.com

class B : public Base { public: void f() override {} };
来源：http://cqg.fzhhl.top

[S43] C++：智能指针
来源：http://wxx.fengsongda.top

auto p = std::make_unique<int>(5);
来源：http://fia.chenlongwang.top

[S44] C++：引用传参
来源：http://rmp.sufxvd.cn

void inc(int &x) { ++x; }
来源：http://fco.smart0.xyz

[S45] C++：lambda
来源：http://zcb.wangdashe.top

auto add = [](int a, int b) { return a + b; };
来源：http://ntl.dianchejie.cn

[S46] C++：函数模板
来源：http://ikd.gotoacloud.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zlu.fktsv.cn

[S47] C++：结构化绑定遍历
来源：http://bpn.xylfe.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qmu.snrcjt.cn

[S48] C++：逐行读文件
来源：http://yjd.pengpengdd.cyou

std::ifstream in("a.txt");  std::string line;
来源：http://dmh.svipenyu.cn

while (std::getline(in, line)) { }
来源：http://fiy.hfpthk.cn

[S49] C++：写文件
来源：http://aya.quarkkingdee.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bkz.birdmap.top

[S50] C++：格式化数字
来源：http://fxx.tian-w.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ssr.zdqjudy.top

[S51] C++：显式类型转换
来源：http://xqz.ehwqpu.com

static_cast<double>(a) / b
来源：http://vco.vehdjk.com

[S52] C++：const 与 noexcept
来源：http://uac.andypj.xyz

int size() const noexcept { return n_; }
来源：http://xka.tanke756.top

[S53] C++：移动语义
来源：http://lch.cashguo.top

std::vector<int> w = std::move(v);
来源：http://jgh.chenlongwang.top

[S54] C++：异常处理
来源：http://vml.dashuyun.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nqd.wangshuangyany.cn

[S55] C++：结构化绑定
来源：http://mgr.daria6918.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fcb.zycfv.cn

[S56] C++：optional
来源：http://gdt.sxryk.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gqp.yj202588.top

[S57] C++：编译期常量
来源：http://fdo.bbcook.cn

constexpr int N = 10;
来源：http://fuc.tarul.cn

[S58] C++：命名空间
来源：http://wma.birdmap.top

namespace ns { int f() { return 1; } }
来源：http://cuc.fktsv.cn

[S59] C++：静态断言
来源：http://fqz.fehbvm.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gmn.kuanghao11.cn

[S60] C++：遍历并删除元素
来源：http://ipq.hysaishi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ucm.nanxinkj.top

================================================================================
来源：http://dst.ywan-chungtsiang.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zgi.hysaishi.cn

================================================================================
来源：http://the.fengsongda.top

[T01] Kotlin：Hello World
来源：http://vub.gaohongyu789.top

println("Hello")
来源：http://its.jinqigufen.top

[T02] Kotlin：变量
来源：http://mdx.xziqi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ipc.shanyushiyangtech.top

[T03] Kotlin：字符串模板
来源：http://aio.c1oappe.top

"值: $b"
来源：http://ugi.pycfn.com

[T04] Kotlin：空安全
来源：http://ica.xuanzx.com

val n: String? = null;  n?.length
来源：http://zjz.hfpthk.cn

[T05] Kotlin：when 表达式
来源：http://zii.kuanghao11.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://adw.zhengqikj.top

[T06] Kotlin：集合映射
来源：http://rzd.ydzc1.top

listOf(1, 2, 3).map { it * 2 }
来源：http://agk.gzhubu.top

[T07] Kotlin：集合过滤
来源：http://gyf.fengsongda.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xvw.andypj.xyz

[T08] Kotlin：数据类
来源：http://bib.shanyushiyangkeji.top

data class User(val name: String, val age: Int)
来源：http://rty.svipenyu.cn

[T09] Kotlin：扩展函数
来源：http://too.zhijiandao.cn

fun String.exclaim() = this + "!"
来源：http://mpv.zhiwuduotai.top

[T10] Kotlin：默认参数
来源：http://fdy.snrcjt.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ubl.tanke756.top

[T11] Kotlin：协程
来源：http://ivs.nwbrower.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ijq.fehbvm.com

[T12] Kotlin：解构声明
来源：http://lge.ywan-chungtsiang.top

val (a, b) = Pair(1, 2)
来源：http://tnv.jinqigfzy.top

[T13] Kotlin：只读 Map
来源：http://fqg.zhijiandao.cn

val m = mapOf("a" to 1)
来源：http://shb.sysykeji.top

[T14] Kotlin：循环
来源：http://cdn.nanxuanxn.top

for (i in 1..10) println(i)
来源：http://tzw.ybcxt.top

[T15] Kotlin：接口
来源：http://tbm.xuanzx.com

interface Shape { fun area(): Double }
来源：http://fmv.fzhhl.top

[T16] Swift：Hello World
来源：http://bvw.yvedp.cn

print("Hello")
来源：http://dqp.cashguo.top

[T17] Swift：变量与常量
来源：http://kba.jianghu66.top

var a = 1;  let b = 2
来源：http://ihd.zhiwuduotai.top

[T18] Swift：字符串插值
来源：http://duu.hywenlv.cn

"值: \(b)"
来源：http://tnk.cdnleiting.top

[T19] Swift：可选绑定
来源：http://chx.tarul.cn

if let n = opt { print(n) }
来源：http://wrb.shangyingyoupin.top

[T20] Swift：数组操作
来源：http://kdl.shanyushiyangtech.top

var a = [1, 2, 3];  a.append(4)
来源：http://kfa.jyoumei.cn

[T21] Swift：遍历
来源：http://vxe.ybcxt.top

for x in a { print(x) }
来源：http://slj.jinghuilouyu.cn

[T22] Swift：字典
来源：http://dxp.yvedp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xib.yfazqb.com


<!-- 参考信息 -->