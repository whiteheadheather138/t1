代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://cxp.wangdashe.top

[R18] 遍历数组
来源：http://isc.gaohongyu789.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dlz.bbcook.cn

[R19] 数组长度
来源：http://ylc.xylfe.cn

echo "${#arr[@]}"
来源：http://csw.vqdsnc.cn

[R20] 关联数组（字典）
来源：http://vcy.ywan-chungtsiang.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tyb.cqqwz.cn

[R21] 字符串长度
来源：http://jxx.zhixingplan.top

echo "${#s}"
来源：http://tqn.52xcode.cn

[R22] 截取子串
来源：http://xng.feifeiyinyue.top

echo "${s:0:5}"
来源：http://hvs.ydjk.org.cn

[R23] 字符串替换
来源：http://ejp.ybcxt.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jqf.mhx1999.top

[R24] 大小写转换
来源：http://nff.guowangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://ibo.zhengqikj.top

[R25] 去后缀 / 去前缀
来源：http://rgq.zhengqikj.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://rvq.andypj.xyz

[R26] 命令替换
来源：http://rbr.vehdjk.com

now=$(date +%F); echo "$now"
来源：http://mmx.ppjwa.cn

[R27] 算术展开
来源：http://yth.52xcode.cn

echo $((1 + 2 * 3))
来源：http://hkn.yvedp.cn

[R28] 浮点运算
来源：http://mgm.cashguo.top

echo "scale=2; 10/3" | bc
来源：http://ylm.cqqwz.cn

[R29] 定义函数
来源：http://zvr.jinyuanbaomall.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qhl.shanyushiyangkeji.top

[R30] 函数返回状态码
来源：http://qax.sufxvd.cn

f() { return 0; }; f || echo "失败了"
来源：http://mhg.gzhubu.top

[R31] 局部变量
来源：http://gow.fehbvm.com

f() { local x=1; echo "$x"; }
来源：http://ekv.9152youxi.cn

[R32] 参数个数校验
来源：http://ikn.redwolf501.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ijr.shangyingyoupin.top

[R33] 捕获错误并提示行号
来源：http://elk.yangfankeji.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dpp.cdnleiting.top

[R34] 退出时清理
来源：http://azp.ybcxt.top

trap 'rm -f "$tmp"' EXIT
来源：http://agd.yangfankeji.com

[R35] 后台执行并等待
来源：http://lge.zhoulong.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://nvz.316326.xyz

[R36] 并发执行多个任务
来源：http://xjg.0kj1m.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mey.dianchejie.cn

[R37] 把输出赋给变量
来源：http://cht.dashuyun.cn

files=$(ls -1)
来源：http://ast.jinyuanbaomall.cn

[R38] 管道串联
来源：http://xxm.hammf.cn

cat a.txt | grep -i error | wc -l
来源：http://niy.xylfe.cn

[R39] 重定向标准输出与错误
来源：http://gpt.vehdjk.com

cmd > out.log 2>&1
来源：http://obq.chenlongwang.top

[R40] 追加写日志
来源：http://dwe.hcnkem.com

echo "log" >> out.log
来源：http://oha.daxiang520.top

[R41] 丢弃输出
来源：http://mrt.zhijiandao.cn

cmd >/dev/null 2>&1
来源：http://pzs.snrcjt.cn

[R42] 输入重定向
来源：http://wkg.yonumen.top

wc -l < a.txt
来源：http://euc.zhaomingkeji.xyz

[R43] 按名字查找文件
来源：http://uaa.nwbrower.top

find . -name "*.log" -type f
来源：http://oza.meibo888.top

[R44] 按修改时间查找
来源：http://xid.daxiang520.top

find . -mtime -7 -type f
来源：http://clc.wangshuangyany.cn

[R45] 批量删除
来源：http://igy.vehdjk.com

find . -name "*.tmp" -delete
来源：http://aiu.hongshengwenyu.top

[R46] 递归替换文件内容
来源：http://lhe.zhiwuduotai.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://irk.quarkkingdee.top

[R47] sed 单行替换
来源：http://hpk.jianghu66.top

sed -i 's/foo/bar/g' a.txt
来源：http://upl.fengsongda.top

[R48] awk 取指定列
来源：http://pjo.cucudq.cn

awk '{print $1, $3}' a.txt
来源：http://hpn.cdnleiting.top

[R49] awk 带条件
来源：http://qyd.haohaochexian.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://haa.jqgufenzy.top

[R50] awk 求和
来源：http://nmw.sufxvd.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cez.aibaodan.cn

[R51] 排序去重取前几
来源：http://ojk.guannengcc.top

sort a.txt | uniq -c | sort -rn | head
来源：http://qbb.xziqi.cn

[R52] 统计行数
来源：http://acy.shanyushiyangkeji.top

wc -l a.txt
来源：http://uuk.yuxming.cn

[R53] 查看文件头与实时尾
来源：http://eyq.ywan-chungtsiang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rkq.ywan-chungtsiang.top

[R54] 比较两个文件
来源：http://que.c1oappe.top

diff a.txt b.txt
来源：http://kcy.tarul.cn

[R55] 压缩与解压
来源：http://gbk.0kj1m.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jgj.shuidangran.top

[R56] 远程拷贝
来源：http://jpu.zhixingplan.top

scp file user@host:/path/
来源：http://bmi.guowangkeji.top

[R57] 远程执行命令
来源：http://ioi.yuanzhike.top

ssh user@host 'uptime'
来源：http://tyy.jiagoushi.top

[R58] 下载文件
来源：http://qwv.yangfankeji.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wvm.ydzc1.top

[R59] 发 POST JSON
来源：http://kev.aizwys.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sat.jinghuilouyu.cn

[R60] 只看 HTTP 状态码
来源：http://oha.redwolf501.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://roq.jyoumei.cn

[R61] 磁盘占用
来源：http://rzg.fzhhl.top

df -h;  du -sh *
来源：http://jxp.tianlin.xyz

[R62] 找最占空间的文件
来源：http://fzs.redwolf501.top

du -ah . | sort -rh | head -10
来源：http://spo.dianchejie.cn

[R63] 内存与进程
来源：http://xcw.ydjk.org.cn

free -h;  ps aux | grep nginx
来源：http://baz.gzhubu.top

[R64] 结束进程
来源：http://bbb.yj20258.top

kill -9 $(pgrep -f app.py)
来源：http://mso.dianchejie.cn

[R65] 查看端口占用
来源：http://sjc.fengsongda.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ezd.mhx1999.top

[R66] 定时任务
来源：http://zes.xinyue.icu

crontab -e;  crontab -l
来源：http://vho.fktsv.cn

[R67] 生成随机十六进制串
来源：http://gvq.nwbrower.top

openssl rand -hex 16
来源：http://njb.52xcode.cn

[R68] 计算文件校验值
来源：http://cmz.jqgfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://raw.aibaodan.cn

[R69] 生成随机密码
来源：http://xgz.xuetiantiany.cn

head -c 16 /dev/urandom | base64
来源：http://zjk.sxryk.cn

[R70] 时间戳与互转
来源：http://nmd.jinqigufen.top

date +%s;  date -d @1700000000
来源：http://jnr.jqgufenzy.top

[R71] 日期格式化
来源：http://sbj.havefunace.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://nhk.xingfuxueyuan.xyz

[R72] 等待端口就绪
来源：http://qgy.zhiwuduotai.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jyo.zdbjq.cn

[R73] 分割大日志
来源：http://eaq.hysaishi.cn

split -l 1000 big.log part_
来源：http://adn.chenlongwang.top

[R74] 批量重命名
来源：http://pfo.316326.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vts.hcnkem.com

[R75] 导出环境变量
来源：http://xby.tarul.cn

export PATH="$HOME/bin:$PATH"
来源：http://yjp.xuanzx.com

[R76] 使用临时文件
来源：http://hng.birdmap.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://asf.xziqi.cn

[R77] 读取用户输入
来源：http://fgr.zhoulong.xyz

read -rp "请输入: " ans
来源：http://uqk.yj20258.top

[R78] 交互式菜单
来源：http://yfi.aizwys.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jmi.jlsjyb.cn

[R79] 解析命令行选项
来源：http://fcb.meibo888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lvv.ehwqpu.com

[R80] 查看脚本执行耗时
来源：http://pxw.xinyue.icu

time ./run.sh
来源：http://itg.gzhubu.top

================================================================================
来源：http://usa.xuanzx.com

S. C / C++ 专题
来源：http://czy.feifeiyinyue.top

================================================================================
来源：http://sjg.sysykeji.top

[S01] C：Hello World
来源：http://kya.fehbvm.com

#include <stdio.h>
来源：http://edr.jlsjyb.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://trm.jinqigufen.top

[S02] C：变量与格式化输出
来源：http://wvg.cashguo.top

int a = 10; printf("%d\n", a);
来源：http://par.xziqi.cn

[S03] C：读入整数
来源：http://mgm.wangdashe.top

int x; scanf("%d", &x);
来源：http://nka.cashguo.top

[S04] C：字符串复制
来源：http://pgi.yuxming.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dnh.jinqigfzy.top

[S05] C：字符串长度
来源：http://xbq.ctjpmb.com

strlen(s)
来源：http://fny.zhiwuduotai.top

[S06] C：字符串比较
来源：http://ktt.sjlbkw.cn

strcmp(a, b) == 0
来源：http://ybl.dashuyun.cn

[S07] C：数组遍历求和
来源：http://ukn.zycfv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uts.shanyushiyangtech.top

[S08] C：动态内存分配与释放
来源：http://ioh.pycfn.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://avn.uphjek.com

[S09] C：结构体定义与初始化
来源：http://wgl.yj20258.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mqw.daxiang520.top

[S10] C：指针与解引用
来源：http://vwb.316326.xyz

int *p = &a;  *p = 5;
来源：http://cyt.fanxiaobao.xyz

[S11] C：逐行读文件
来源：http://kvu.ehwqpu.com

FILE *f = fopen("a.txt", "r");
来源：http://btg.snrcjt.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dcl.jqgfzy.top

fclose(f);
来源：http://dzn.yongpay.top

[S12] C：写文件
来源：http://szc.jianghu66.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yns.shanyushiyangkeji.top

[S13] C：宏定义
来源：http://doq.xuanzx.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xkj.andypj.xyz

[S14] C：枚举
来源：http://xlb.haohaochexian.top

enum Color { RED, GREEN, BLUE };
来源：http://baf.gogol.net.cn

[S15] C：类型转换
来源：http://cyq.xziqi.cn

(double) a / b
来源：http://mmx.cqqwz.cn

[S16] C：位操作置位
来源：http://ljx.mhx1999.top

x |= (1 << 3);
来源：http://dmb.shangyingyoupin.top

[S17] C：安全拼接字符串
来源：http://gus.pengpengdd.cyou

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jim.vehdjk.com

[S18] C：命令行参数
来源：http://lxm.zhiwuduotai.top

int main(int argc, char **argv)
来源：http://wdu.sweek.top

[S19] C：快速排序
来源：http://mvh.52xcode.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fwj.fzhhl.top

[S20] C：二分查找
来源：http://qld.zdqjudy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zhi.shangyingyoupin.top

[S21] C：字符类别判断
来源：http://mmr.yuanzhike.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mub.gzhubu.top

[S22] C：字符串转数字
来源：http://elo.bjfxy.top

atoi("42");  strtod("3.14", NULL);
来源：http://bid.zycfv.cn

[S23] C：随机数
来源：http://rst.ydzc1.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xxd.sweek.top

[S24] C：获取本地时间
来源：http://uai.hcnkem.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zms.kuanghao11.cn

[S25] C：内存拷贝
来源：http://lkb.316326.xyz

memcpy(dst, src, n);
来源：http://cka.yuanzhike.top

[S26] C：内存清零
来源：http://yvw.zhijiandao.cn

memset(a, 0, sizeof a);
来源：http://uaj.zhaomingkeji.xyz

[S27] C：定义常量
来源：http://ssc.vehdjk.com

const double PI = 3.14159;
来源：http://ojn.jinyuanbaomall.cn

[S28] C：静态变量
来源：http://iyf.daxiang520.top

static int counter = 0;
来源：http://hle.vehdjk.com

[S29] C：变参函数
来源：http://orm.redwolf501.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lus.pengpengdd.cyou

[S30] C：头文件保护
来源：http://svc.ctjpmb.com

#ifndef X_H
来源：http://oiq.9152youxi.cn

#define X_H
来源：http://thv.shanyushiyangkeji.top

#endif
来源：http://coj.zhongyouzk.top

[S31] C++：Hello World
来源：http://ufd.vqdsnc.cn

#include <iostream>
来源：http://jds.sxryk.cn

int main() { std::cout << "Hello\n"; }
来源：http://eul.nwbrower.top

[S32] C++：字符串
来源：http://ksb.bjfxy.top

std::string s = "hi";  s += "!";
来源：http://obe.ybcxt.top

[S33] C++：vector 增删
来源：http://cwe.chenzaomai.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vzc.xylfe.cn

[S34] C++：遍历 vector
来源：http://uts.hfpthk.cn

for (auto &x : v) { std::cout << x; }
来源：http://gvk.hammf.cn

[S35] C++：map
来源：http://yiu.shanyushiyangkeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ecb.yuxming.cn

[S36] C++：unordered_map
来源：http://ull.vqdsnc.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sod.zdqjudy.top

[S37] C++：set
来源：http://vux.yj20258888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eei.jqgufenzy.top

[S38] C++：排序
来源：http://bgv.pycfn.com

std::sort(v.begin(), v.end());
来源：http://aqt.wangshuangyany.cn

[S39] C++：自定义比较器排序
来源：http://pfb.tanke756.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zci.sysykeji.top

[S40] C++：查找元素
来源：http://xqr.xuetiantiany.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dxf.birdmap.top

[S41] C++：类与构造函数
来源：http://qbs.xylfe.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://aby.jyoumei.cn

[S42] C++：继承与虚函数
来源：http://lam.guowangkeji.top

class B : public Base { public: void f() override {} };
来源：http://nqe.zhaomingkeji.xyz

[S43] C++：智能指针
来源：http://lcm.fanxiaobao.xyz

auto p = std::make_unique<int>(5);
来源：http://nlb.wangdashe.top

[S44] C++：引用传参
来源：http://xqf.yonumen.top

void inc(int &x) { ++x; }
来源：http://ive.tarul.cn

[S45] C++：lambda
来源：http://fjf.ywan-chungtsiang.top

auto add = [](int a, int b) { return a + b; };
来源：http://bpb.jianghu66.top

[S46] C++：函数模板
来源：http://wvr.zhixingplan.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tfz.fzhhl.top

[S47] C++：结构化绑定遍历
来源：http://nvv.andypj.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pip.zhengqikj.top

[S48] C++：逐行读文件
来源：http://tti.hfpthk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xao.xziqi.cn

while (std::getline(in, line)) { }
来源：http://boa.yvedp.cn

[S49] C++：写文件
来源：http://wou.haohaochexian.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cdu.xinyue.icu

[S50] C++：格式化数字
来源：http://wqt.316326.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xdf.zdbjq.cn

[S51] C++：显式类型转换
来源：http://doj.aizwys.cn

static_cast<double>(a) / b
来源：http://mxz.hywenlv.cn

[S52] C++：const 与 noexcept
来源：http://erq.xylfe.cn

int size() const noexcept { return n_; }
来源：http://uzf.shanyushiyangkeji.top

[S53] C++：移动语义
来源：http://xeh.smart0.xyz

std::vector<int> w = std::move(v);
来源：http://izi.epnwcf.com

[S54] C++：异常处理
来源：http://mgj.jqgufenzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wsi.fehbvm.com

[S55] C++：结构化绑定
来源：http://xty.fanxiaobao.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://oat.yonumen.top

[S56] C++：optional
来源：http://glq.ivvv.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://icp.wangshuangyany.cn

[S57] C++：编译期常量
来源：http://dqx.chenlongwang.top

constexpr int N = 10;
来源：http://igy.vqdsnc.cn

[S58] C++：命名空间
来源：http://byi.redwolf501.top

namespace ns { int f() { return 1; } }
来源：http://izn.hysaishi.cn

[S59] C++：静态断言
来源：http://owt.gotoacloud.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ukl.shanyushiyangtech.top

[S60] C++：遍历并删除元素
来源：http://csc.vehdjk.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pbc.jyoumei.cn

================================================================================
来源：http://ydq.fzhhl.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nno.zhengqikj.top

================================================================================
来源：http://xpu.chenzaomai.com

[T01] Kotlin：Hello World
来源：http://anw.kuanghao11.cn

println("Hello")
来源：http://qur.bbcook.cn

[T02] Kotlin：变量
来源：http://dlo.fengsongda.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fbk.uphjek.com

[T03] Kotlin：字符串模板
来源：http://dnm.aizwys.cn

"值: $b"
来源：http://afv.zhoulong.xyz

[T04] Kotlin：空安全
来源：http://gug.havefunace.top

val n: String? = null;  n?.length
来源：http://lok.zhoulong.xyz

[T05] Kotlin：when 表达式
来源：http://ghr.iojbl.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iko.shanyushiyangkeji.top

[T06] Kotlin：集合映射
来源：http://vde.fanxiaobao.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://zpr.sysykeji.top

[T07] Kotlin：集合过滤
来源：http://hwu.hywenlv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xwu.ybcxt.top

[T08] Kotlin：数据类
来源：http://tco.jqgfzy.top

data class User(val name: String, val age: Int)
来源：http://nhx.52xcode.cn

[T09] Kotlin：扩展函数
来源：http://acj.yongpay.top

fun String.exclaim() = this + "!"
来源：http://bwp.jinqigfzy.top

[T10] Kotlin：默认参数
来源：http://efk.bbcook.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cse.guowangkeji.top

[T11] Kotlin：协程
来源：http://dhw.vehdjk.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://gji.yanxiufei.cn

[T12] Kotlin：解构声明
来源：http://tkd.redwolf501.top

val (a, b) = Pair(1, 2)
来源：http://izh.zhijiandao.cn

[T13] Kotlin：只读 Map
来源：http://cpq.zdqjudy.top

val m = mapOf("a" to 1)
来源：http://gly.nanxinkj.top

[T14] Kotlin：循环
来源：http://bnq.nanxuanxn.top

for (i in 1..10) println(i)
来源：http://tjv.feifeiyinyue.top

[T15] Kotlin：接口
来源：http://mdw.aizwys.cn

interface Shape { fun area(): Double }
来源：http://col.yj202588.top

[T16] Swift：Hello World
来源：http://oqr.zhengqikj.top

print("Hello")
来源：http://pxs.aizwys.cn

[T17] Swift：变量与常量
来源：http://waa.yangfankeji.com

var a = 1;  let b = 2
来源：http://ysp.dashuyun.cn

[T18] Swift：字符串插值
来源：http://hbc.fehbvm.com

"值: \(b)"
来源：http://htw.ivvv.top

[T19] Swift：可选绑定
来源：http://hkw.hammf.cn

if let n = opt { print(n) }
来源：http://kkt.tarul.cn

[T20] Swift：数组操作
来源：http://pzk.xylfe.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fxz.fzhhl.top


<!-- 参考信息 -->