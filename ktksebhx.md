代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mnl.xuanzx.com

[R16] until 等待条件
来源：http://faw.snrcjt.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://psl.nanxinkj.top

[R17] 数组定义与取值
来源：http://sjl.jinqigufen.top

arr=(a b c); echo "${arr[0]}"
来源：http://pxt.zhiwuduotai.top

[R18] 遍历数组
来源：http://umj.uphjek.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ucm.guowangkeji.top

[R19] 数组长度
来源：http://sir.52xcode.cn

echo "${#arr[@]}"
来源：http://uxt.jqgufenzy.top

[R20] 关联数组（字典）
来源：http://amn.cheryme.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://obr.fanxiaobao.xyz

[R21] 字符串长度
来源：http://yly.nanxuanxn.top

echo "${#s}"
来源：http://kla.dashuyun.cn

[R22] 截取子串
来源：http://ldo.ppjwa.cn

echo "${s:0:5}"
来源：http://spa.yuxming.cn

[R23] 字符串替换
来源：http://fnk.feifeiyinyue.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ejz.shuidangran.top

[R24] 大小写转换
来源：http://ywe.zhoulong.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://ymo.tianlin.xyz

[R25] 去后缀 / 去前缀
来源：http://yrn.316326.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://xvi.316326.xyz

[R26] 命令替换
来源：http://xrn.epnwcf.com

now=$(date +%F); echo "$now"
来源：http://uam.sweek.top

[R27] 算术展开
来源：http://xym.mhx1999.top

echo $((1 + 2 * 3))
来源：http://vdf.hesvh.cn

[R28] 浮点运算
来源：http://mis.yj202588.top

echo "scale=2; 10/3" | bc
来源：http://wap.sysykeji.top

[R29] 定义函数
来源：http://tgv.kuanghao11.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://doh.chenzaomai.com

[R30] 函数返回状态码
来源：http://qde.shanyushiyangtech.top

f() { return 0; }; f || echo "失败了"
来源：http://gok.ybcxt.top

[R31] 局部变量
来源：http://asb.epnwcf.com

f() { local x=1; echo "$x"; }
来源：http://jxf.hongshengwenyu.top

[R32] 参数个数校验
来源：http://gao.uphjek.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wyo.fktsv.cn

[R33] 捕获错误并提示行号
来源：http://vmq.andypj.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yau.ctjpmb.com

[R34] 退出时清理
来源：http://bcb.c1oappe.top

trap 'rm -f "$tmp"' EXIT
来源：http://qfu.aizwys.cn

[R35] 后台执行并等待
来源：http://lio.guowangkeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://cuy.zhengqikj.top

[R36] 并发执行多个任务
来源：http://wpr.gaohongyu789.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://unl.sysykeji.top

[R37] 把输出赋给变量
来源：http://phl.aibaodan.cn

files=$(ls -1)
来源：http://azl.sysykeji.top

[R38] 管道串联
来源：http://fmu.xuetiantiany.cn

cat a.txt | grep -i error | wc -l
来源：http://zvx.jinqigufen.top

[R39] 重定向标准输出与错误
来源：http://qax.chenzaomai.com

cmd > out.log 2>&1
来源：http://nvh.zdbjq.cn

[R40] 追加写日志
来源：http://oir.bbcook.cn

echo "log" >> out.log
来源：http://unb.9152youxi.cn

[R41] 丢弃输出
来源：http://gqh.hongshengwenyu.top

cmd >/dev/null 2>&1
来源：http://scj.birdmap.top

[R42] 输入重定向
来源：http://qnp.pengpengdd.cyou

wc -l < a.txt
来源：http://vvc.316326.xyz

[R43] 按名字查找文件
来源：http://arj.yuanzhike.top

find . -name "*.log" -type f
来源：http://lea.ydzc1.top

[R44] 按修改时间查找
来源：http://ajp.hnxiangtu.top

find . -mtime -7 -type f
来源：http://bsv.cucudq.cn

[R45] 批量删除
来源：http://zsw.cqqwz.cn

find . -name "*.tmp" -delete
来源：http://ooa.tianlin.xyz

[R46] 递归替换文件内容
来源：http://njt.jinyuanbaomall.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://usq.gzhubu.top

[R47] sed 单行替换
来源：http://mmd.yangfankeji.com

sed -i 's/foo/bar/g' a.txt
来源：http://jhs.nwbrower.top

[R48] awk 取指定列
来源：http://gyc.aibaodan.cn

awk '{print $1, $3}' a.txt
来源：http://cpq.cheryme.top

[R49] awk 带条件
来源：http://afa.vehdjk.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jbz.fktsv.cn

[R50] awk 求和
来源：http://bqy.chenjidiqi.icu

awk '{s += $2} END {print s}' a.txt
来源：http://zqc.wangdashe.top

[R51] 排序去重取前几
来源：http://guw.redwolf501.top

sort a.txt | uniq -c | sort -rn | head
来源：http://joj.meibo888.top

[R52] 统计行数
来源：http://ddi.guannengcc.top

wc -l a.txt
来源：http://azy.nanxuanxn.top

[R53] 查看文件头与实时尾
来源：http://qkj.52xcode.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sov.dianchejie.cn

[R54] 比较两个文件
来源：http://tsf.aizwys.cn

diff a.txt b.txt
来源：http://mqs.zhixingplan.top

[R55] 压缩与解压
来源：http://eoi.hnqzz.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fck.ydzc1.top

[R56] 远程拷贝
来源：http://cuu.tianlin.xyz

scp file user@host:/path/
来源：http://qsg.chenlongwang.top

[R57] 远程执行命令
来源：http://mqs.havefunace.top

ssh user@host 'uptime'
来源：http://wqv.hongshengwenyu.top

[R58] 下载文件
来源：http://ojh.ydjk.org.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zyl.sufxvd.cn

[R59] 发 POST JSON
来源：http://fkg.shangyingyoupin.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zuh.fanxiaobao.xyz

[R60] 只看 HTTP 状态码
来源：http://ays.svipenyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kms.zhixingplan.top

[R61] 磁盘占用
来源：http://isq.chenzaomai.com

df -h;  du -sh *
来源：http://mvw.wangshuangyany.cn

[R62] 找最占空间的文件
来源：http://uwr.hnqzz.top

du -ah . | sort -rh | head -10
来源：http://pqc.feifeiyinyue.top

[R63] 内存与进程
来源：http://bab.jianghu66.top

free -h;  ps aux | grep nginx
来源：http://fyv.snrcjt.cn

[R64] 结束进程
来源：http://dkx.vehdjk.com

kill -9 $(pgrep -f app.py)
来源：http://uqp.fehbvm.com

[R65] 查看端口占用
来源：http://flw.jqgfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bng.0kj1m.cn

[R66] 定时任务
来源：http://trl.0kj1m.cn

crontab -e;  crontab -l
来源：http://fzg.vehdjk.com

[R67] 生成随机十六进制串
来源：http://wqx.yfazqb.com

openssl rand -hex 16
来源：http://foj.svipenyu.cn

[R68] 计算文件校验值
来源：http://sev.jinyuanbaomall.cn

sha256sum a.txt;  md5sum a.txt
来源：http://scn.xuetiantiany.cn

[R69] 生成随机密码
来源：http://yqb.52xcode.cn

head -c 16 /dev/urandom | base64
来源：http://eot.haohaochexian.top

[R70] 时间戳与互转
来源：http://zlv.c1oappe.top

date +%s;  date -d @1700000000
来源：http://rwk.guannengcc.top

[R71] 日期格式化
来源：http://ihe.zhoulong.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://uwb.havefunace.top

[R72] 等待端口就绪
来源：http://oxf.sufxvd.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nuy.wangshuangyany.cn

[R73] 分割大日志
来源：http://fvj.jqgfzy.top

split -l 1000 big.log part_
来源：http://slt.xylfe.cn

[R74] 批量重命名
来源：http://nxf.sufxvd.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zdx.yj202588.top

[R75] 导出环境变量
来源：http://xgc.ybcxt.top

export PATH="$HOME/bin:$PATH"
来源：http://atl.bbcook.cn

[R76] 使用临时文件
来源：http://hlb.tarul.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nna.fanxiaobao.xyz

[R77] 读取用户输入
来源：http://drj.sysykeji.top

read -rp "请输入: " ans
来源：http://bjh.meibo888.top

[R78] 交互式菜单
来源：http://jxy.gogol.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sij.ywan-chungtsiang.top

[R79] 解析命令行选项
来源：http://ozu.c1oappe.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sis.0kj1m.cn

[R80] 查看脚本执行耗时
来源：http://khp.jiagoushi.top

time ./run.sh
来源：http://cbv.sufxvd.cn

================================================================================
来源：http://gdc.jqgfzy.top

S. C / C++ 专题
来源：http://ryq.quarkkingdee.top

================================================================================
来源：http://hkn.yj20258.top

[S01] C：Hello World
来源：http://zah.havefunace.top

#include <stdio.h>
来源：http://xjm.zdqjudy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://iqy.zhiwuduotai.top

[S02] C：变量与格式化输出
来源：http://ysm.jinqigfzy.top

int a = 10; printf("%d\n", a);
来源：http://own.sjlbkw.cn

[S03] C：读入整数
来源：http://lqm.c1oappe.top

int x; scanf("%d", &x);
来源：http://jtc.wangdashe.top

[S04] C：字符串复制
来源：http://hij.redwolf501.top

char dst[32]; strcpy(dst, "hi");
来源：http://jpa.hywenlv.cn

[S05] C：字符串长度
来源：http://xcl.316326.xyz

strlen(s)
来源：http://rbo.chenzaomai.com

[S06] C：字符串比较
来源：http://fau.xingfuxueyuan.xyz

strcmp(a, b) == 0
来源：http://ucq.chenlongwang.top

[S07] C：数组遍历求和
来源：http://rmz.jyoumei.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jwl.jianghu66.top

[S08] C：动态内存分配与释放
来源：http://ibx.haohaochexian.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pfd.iojbl.cn

[S09] C：结构体定义与初始化
来源：http://rjg.xuetiantiany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uyx.jiagoushi.top

[S10] C：指针与解引用
来源：http://frm.cqqwz.cn

int *p = &a;  *p = 5;
来源：http://vtu.xziqi.cn

[S11] C：逐行读文件
来源：http://dtd.jinqigufen.top

FILE *f = fopen("a.txt", "r");
来源：http://inb.andypj.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://rbb.316326.xyz

fclose(f);
来源：http://mrw.smart0.xyz

[S12] C：写文件
来源：http://zxt.iojbl.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fkb.jinqigufen.top

[S13] C：宏定义
来源：http://jvc.jqgufenzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lfq.cqqwz.cn

[S14] C：枚举
来源：http://dmr.ivvv.top

enum Color { RED, GREEN, BLUE };
来源：http://rcg.yueranfly.top

[S15] C：类型转换
来源：http://obk.jiagoushi.top

(double) a / b
来源：http://iix.sxryk.cn

[S16] C：位操作置位
来源：http://juv.havefunace.top

x |= (1 << 3);
来源：http://ufa.svipenyu.cn

[S17] C：安全拼接字符串
来源：http://usd.haohaochexian.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wfl.sxryk.cn

[S18] C：命令行参数
来源：http://gvs.yanxiufei.cn

int main(int argc, char **argv)
来源：http://cag.gzhubu.top

[S19] C：快速排序
来源：http://ipl.ppjwa.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ewv.jiagoushi.top

[S20] C：二分查找
来源：http://fpq.yanxiufei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oyw.52xcode.cn

[S21] C：字符类别判断
来源：http://hhn.tian-w.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lef.fzhhl.top

[S22] C：字符串转数字
来源：http://hbl.yonumen.top

atoi("42");  strtod("3.14", NULL);
来源：http://ixr.bbcook.cn

[S23] C：随机数
来源：http://lmi.ctjpmb.com

srand(time(NULL));  int r = rand() % 100;
来源：http://szp.cqqwz.cn

[S24] C：获取本地时间
来源：http://qgf.zdbjq.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ocy.wangshuangyany.cn

[S25] C：内存拷贝
来源：http://tpj.zhijiandao.cn

memcpy(dst, src, n);
来源：http://dpq.zhengqikj.top

[S26] C：内存清零
来源：http://clh.wangshuangyany.cn

memset(a, 0, sizeof a);
来源：http://mvo.jqgfzy.top

[S27] C：定义常量
来源：http://ims.sjlbkw.cn

const double PI = 3.14159;
来源：http://kge.hammf.cn

[S28] C：静态变量
来源：http://vtz.daxiang520.top

static int counter = 0;
来源：http://tdp.xziqi.cn

[S29] C：变参函数
来源：http://btk.hcnkem.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ycr.havefunace.top

[S30] C：头文件保护
来源：http://wve.quarkkingdee.top

#ifndef X_H
来源：http://khc.yuanzhike.top

#define X_H
来源：http://cwl.hesvh.cn

#endif
来源：http://jjm.shzxlz.cn

[S31] C++：Hello World
来源：http://hgh.zhixingplan.top

#include <iostream>
来源：http://jkx.nwbrower.top

int main() { std::cout << "Hello\n"; }
来源：http://jnf.pengpengdd.cyou

[S32] C++：字符串
来源：http://ryz.kuanghao11.cn

std::string s = "hi";  s += "!";
来源：http://dme.yj20258888.top

[S33] C++：vector 增删
来源：http://off.gzhubu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wgv.daxiang520.top

[S34] C++：遍历 vector
来源：http://qua.meibo888.top

for (auto &x : v) { std::cout << x; }
来源：http://cxy.chenzaomai.com

[S35] C++：map
来源：http://exp.daria6918.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://aox.nanxuanxn.top

[S36] C++：unordered_map
来源：http://eqg.tanke756.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wgs.xziqi.cn

[S37] C++：set
来源：http://vgf.cucudq.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xku.fanxiaobao.xyz

[S38] C++：排序
来源：http://pcw.ctjpmb.com

std::sort(v.begin(), v.end());
来源：http://goc.jyoumei.cn

[S39] C++：自定义比较器排序
来源：http://mbx.chenzaomai.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gnh.mhx1999.top

[S40] C++：查找元素
来源：http://rfm.ppjwa.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cfz.svipenyu.cn

[S41] C++：类与构造函数
来源：http://wwi.dashuyun.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kpe.xuanzx.com

[S42] C++：继承与虚函数
来源：http://idv.gzhubu.top

class B : public Base { public: void f() override {} };
来源：http://ckz.mhx1999.top

[S43] C++：智能指针
来源：http://dqj.shanyushiyangtech.top

auto p = std::make_unique<int>(5);
来源：http://jxs.yvedp.cn

[S44] C++：引用传参
来源：http://lzs.snrcjt.cn

void inc(int &x) { ++x; }
来源：http://wow.yj202588.top

[S45] C++：lambda
来源：http://uld.sjlbkw.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mie.tianlin.xyz

[S46] C++：函数模板
来源：http://ddk.jyoumei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cbf.haohaochexian.top

[S47] C++：结构化绑定遍历
来源：http://oeg.gaohongyu789.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kqc.zhaomingkeji.xyz

[S48] C++：逐行读文件
来源：http://voa.yangfankeji.com

std::ifstream in("a.txt");  std::string line;
来源：http://vsc.jlsjyb.cn

while (std::getline(in, line)) { }
来源：http://qix.shangyingyoupin.top

[S49] C++：写文件
来源：http://led.mhx1999.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ost.nanxuanxn.top

[S50] C++：格式化数字
来源：http://ooy.52xcode.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://waa.zhixingplan.top

[S51] C++：显式类型转换
来源：http://zwo.ctjpmb.com

static_cast<double>(a) / b
来源：http://ryo.zhengqikj.top

[S52] C++：const 与 noexcept
来源：http://tjc.bjfxy.top

int size() const noexcept { return n_; }
来源：http://fso.tianlin.xyz

[S53] C++：移动语义
来源：http://lvz.zhaomingkeji.xyz

std::vector<int> w = std::move(v);
来源：http://cyt.fehbvm.com

[S54] C++：异常处理
来源：http://ftg.hysaishi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uaw.hcnkem.com

[S55] C++：结构化绑定
来源：http://lvg.bbcook.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wbe.birdmap.top

[S56] C++：optional
来源：http://vym.sysykeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ghe.jiagoushi.top

[S57] C++：编译期常量
来源：http://bwn.yj20258.top

constexpr int N = 10;
来源：http://lqg.sxryk.cn

[S58] C++：命名空间
来源：http://flf.hnxiangtu.top

namespace ns { int f() { return 1; } }
来源：http://yxa.smart0.xyz

[S59] C++：静态断言
来源：http://hbu.jinqigfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yzg.zhengqikj.top

[S60] C++：遍历并删除元素
来源：http://bub.wangshuangyany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qrh.andypj.xyz

================================================================================
来源：http://gah.uphjek.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ddp.shangyingyoupin.top

================================================================================
来源：http://mcd.daria6918.cn

[T01] Kotlin：Hello World
来源：http://ulb.iojbl.cn

println("Hello")
来源：http://bdw.aizwys.cn

[T02] Kotlin：变量
来源：http://jsq.fehbvm.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jug.yvedp.cn

[T03] Kotlin：字符串模板
来源：http://dpz.guannengcc.top

"值: $b"
来源：http://cwz.hammf.cn

[T04] Kotlin：空安全
来源：http://zza.daxiang520.top

val n: String? = null;  n?.length
来源：http://nbs.jlsjyb.cn

[T05] Kotlin：when 表达式
来源：http://ovt.yj202588.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nyy.hesvh.cn

[T06] Kotlin：集合映射
来源：http://vpb.cqqwz.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rxh.fanxiaobao.xyz

[T07] Kotlin：集合过滤
来源：http://tjk.xuanzx.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://vup.yj20258888.top

[T08] Kotlin：数据类
来源：http://nog.yueranfly.top

data class User(val name: String, val age: Int)
来源：http://lje.yuanzhike.top

[T09] Kotlin：扩展函数
来源：http://btq.shanyushiyangkeji.top

fun String.exclaim() = this + "!"
来源：http://nri.zhiwuduotai.top

[T10] Kotlin：默认参数
来源：http://otx.jinyuanbaomall.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hzb.gogol.net.cn

[T11] Kotlin：协程
来源：http://doh.chenzaomai.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://tdr.cdnleiting.top

[T12] Kotlin：解构声明
来源：http://ouh.cucudq.cn

val (a, b) = Pair(1, 2)
来源：http://qed.52xcode.cn

[T13] Kotlin：只读 Map
来源：http://bpc.iojbl.cn

val m = mapOf("a" to 1)
来源：http://wgh.fengsongda.top

[T14] Kotlin：循环
来源：http://bfo.dashuyun.cn

for (i in 1..10) println(i)
来源：http://kac.jyoumei.cn

[T15] Kotlin：接口
来源：http://uwx.gogol.net.cn

interface Shape { fun area(): Double }
来源：http://pjw.zycfv.cn

[T16] Swift：Hello World
来源：http://hsl.cheryme.top

print("Hello")
来源：http://fhw.hnxiangtu.top

[T17] Swift：变量与常量
来源：http://nkh.shanyushiyangkeji.top

var a = 1;  let b = 2
来源：http://tff.cashguo.top

[T18] Swift：字符串插值
来源：http://hyf.sweek.top

"值: \(b)"
来源：http://spi.guowangkeji.top


<!-- 参考信息 -->