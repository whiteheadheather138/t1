代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://mzw.jinqigfzy.top

[R14] C 风格 for
来源：http://gug.shzxlz.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nlb.zhengqikj.top

[R15] while 逐行读文件
来源：http://jgu.guannengcc.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rwa.snrcjt.cn

[R16] until 等待条件
来源：http://mjh.dianchejie.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://btk.pengpengdd.cyou

[R17] 数组定义与取值
来源：http://yak.chenjidiqi.icu

arr=(a b c); echo "${arr[0]}"
来源：http://ifl.zhengqikj.top

[R18] 遍历数组
来源：http://xxn.zhengqikj.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dym.birdmap.top

[R19] 数组长度
来源：http://zoz.jianghu66.top

echo "${#arr[@]}"
来源：http://ogd.iojbl.cn

[R20] 关联数组（字典）
来源：http://rkh.shzxlz.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dmu.yangfankeji.com

[R21] 字符串长度
来源：http://aly.jiagoushi.top

echo "${#s}"
来源：http://pwk.zdbjq.cn

[R22] 截取子串
来源：http://vvc.zdbjq.cn

echo "${s:0:5}"
来源：http://gyp.ehwqpu.com

[R23] 字符串替换
来源：http://xou.tian-w.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iri.wangshuangyany.cn

[R24] 大小写转换
来源：http://jyu.hnxiangtu.top

echo "${s^^}"; echo "${s,,}"
来源：http://klz.zdqjudy.top

[R25] 去后缀 / 去前缀
来源：http://osf.zdqjudy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ikc.gotoacloud.top

[R26] 命令替换
来源：http://ped.tanke756.top

now=$(date +%F); echo "$now"
来源：http://cda.uphjek.com

[R27] 算术展开
来源：http://bxw.cashguo.top

echo $((1 + 2 * 3))
来源：http://cbp.c1oappe.top

[R28] 浮点运算
来源：http://ynx.sufxvd.cn

echo "scale=2; 10/3" | bc
来源：http://zdh.chenzaomai.com

[R29] 定义函数
来源：http://xel.zycfv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zvo.hnqzz.top

[R30] 函数返回状态码
来源：http://vpx.9152youxi.cn

f() { return 0; }; f || echo "失败了"
来源：http://lwb.0kj1m.cn

[R31] 局部变量
来源：http://exi.0kj1m.cn

f() { local x=1; echo "$x"; }
来源：http://ern.yj202588.top

[R32] 参数个数校验
来源：http://tmi.jinqigufen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tmn.yuanzhike.top

[R33] 捕获错误并提示行号
来源：http://qwd.52xcode.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xze.hammf.cn

[R34] 退出时清理
来源：http://has.haohaochexian.top

trap 'rm -f "$tmp"' EXIT
来源：http://lzz.gotoacloud.top

[R35] 后台执行并等待
来源：http://ocj.jiagoushi.top

sleep 5 & pid=$!; wait "$pid"
来源：http://rsx.52xcode.cn

[R36] 并发执行多个任务
来源：http://wrf.vqdsnc.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yic.svipenyu.cn

[R37] 把输出赋给变量
来源：http://qax.jyoumei.cn

files=$(ls -1)
来源：http://cyj.jiagoushi.top

[R38] 管道串联
来源：http://kgf.ehwqpu.com

cat a.txt | grep -i error | wc -l
来源：http://obr.hnxiangtu.top

[R39] 重定向标准输出与错误
来源：http://vud.xuetiantiany.cn

cmd > out.log 2>&1
来源：http://uoi.yueranfly.top

[R40] 追加写日志
来源：http://nou.c1oappe.top

echo "log" >> out.log
来源：http://pwd.yj20258.top

[R41] 丢弃输出
来源：http://une.sxryk.cn

cmd >/dev/null 2>&1
来源：http://yiv.yuanzhike.top

[R42] 输入重定向
来源：http://vrc.zycfv.cn

wc -l < a.txt
来源：http://amt.kuanghao11.cn

[R43] 按名字查找文件
来源：http://vsf.yonumen.top

find . -name "*.log" -type f
来源：http://myk.guannengcc.top

[R44] 按修改时间查找
来源：http://lir.sjlbkw.cn

find . -mtime -7 -type f
来源：http://gfy.yfazqb.com

[R45] 批量删除
来源：http://hux.nanxuanxn.top

find . -name "*.tmp" -delete
来源：http://xtj.ydzc1.top

[R46] 递归替换文件内容
来源：http://qmr.fanxiaobao.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fca.0kj1m.cn

[R47] sed 单行替换
来源：http://ujy.yuxming.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rwe.hesvh.cn

[R48] awk 取指定列
来源：http://ban.tianlin.xyz

awk '{print $1, $3}' a.txt
来源：http://ftl.sufxvd.cn

[R49] awk 带条件
来源：http://pkb.mhx1999.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fdl.ybcxt.top

[R50] awk 求和
来源：http://szq.snrcjt.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cbn.svipenyu.cn

[R51] 排序去重取前几
来源：http://phh.zhaomingkeji.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://qjk.jianghu66.top

[R52] 统计行数
来源：http://rbt.shzxlz.cn

wc -l a.txt
来源：http://pfz.guannengcc.top

[R53] 查看文件头与实时尾
来源：http://nud.hesvh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://khu.jinghuilouyu.cn

[R54] 比较两个文件
来源：http://boa.c1oappe.top

diff a.txt b.txt
来源：http://dzb.zhixingplan.top

[R55] 压缩与解压
来源：http://iky.pycfn.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hmv.zhixingplan.top

[R56] 远程拷贝
来源：http://wpt.gotoacloud.top

scp file user@host:/path/
来源：http://udf.birdmap.top

[R57] 远程执行命令
来源：http://szh.iojbl.cn

ssh user@host 'uptime'
来源：http://gdd.shzxlz.cn

[R58] 下载文件
来源：http://nne.shangyingyoupin.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://piy.ctjpmb.com

[R59] 发 POST JSON
来源：http://jbu.jlsjyb.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fmr.zdqjudy.top

[R60] 只看 HTTP 状态码
来源：http://mfo.hesvh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oib.shuidangran.top

[R61] 磁盘占用
来源：http://vzq.gogol.net.cn

df -h;  du -sh *
来源：http://ntj.zhixingplan.top

[R62] 找最占空间的文件
来源：http://mrp.ybcxt.top

du -ah . | sort -rh | head -10
来源：http://xui.quarkkingdee.top

[R63] 内存与进程
来源：http://fjr.fanxiaobao.xyz

free -h;  ps aux | grep nginx
来源：http://zkq.yvedp.cn

[R64] 结束进程
来源：http://tnu.uphjek.com

kill -9 $(pgrep -f app.py)
来源：http://rlg.ppjwa.cn

[R65] 查看端口占用
来源：http://dup.hcnkem.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uzz.cqqwz.cn

[R66] 定时任务
来源：http://fwy.sxryk.cn

crontab -e;  crontab -l
来源：http://itk.ywan-chungtsiang.top

[R67] 生成随机十六进制串
来源：http://jpt.ppjwa.cn

openssl rand -hex 16
来源：http://isq.yongpay.top

[R68] 计算文件校验值
来源：http://umb.hfpthk.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vga.gzhubu.top

[R69] 生成随机密码
来源：http://bck.jinqigfzy.top

head -c 16 /dev/urandom | base64
来源：http://dsi.pengpengdd.cyou

[R70] 时间戳与互转
来源：http://dgi.nanxinkj.top

date +%s;  date -d @1700000000
来源：http://qxu.svipenyu.cn

[R71] 日期格式化
来源：http://rsp.havefunace.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://won.yj20258888.top

[R72] 等待端口就绪
来源：http://cwa.xuanzx.com

until nc -z localhost 3306; do sleep 1; done
来源：http://zgx.daxiang520.top

[R73] 分割大日志
来源：http://usg.jqgfzy.top

split -l 1000 big.log part_
来源：http://wup.52xcode.cn

[R74] 批量重命名
来源：http://gvh.fengsongda.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://skt.jianghu66.top

[R75] 导出环境变量
来源：http://dry.0kj1m.cn

export PATH="$HOME/bin:$PATH"
来源：http://dwk.jinyuanbaomall.cn

[R76] 使用临时文件
来源：http://ruu.gotoacloud.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://klq.yvedp.cn

[R77] 读取用户输入
来源：http://bfy.cucudq.cn

read -rp "请输入: " ans
来源：http://apc.yongpay.top

[R78] 交互式菜单
来源：http://csr.9152youxi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cbu.hywenlv.cn

[R79] 解析命令行选项
来源：http://tlt.zhijiandao.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://iqu.meibo888.top

[R80] 查看脚本执行耗时
来源：http://cxu.jinqigfzy.top

time ./run.sh
来源：http://dsy.zycfv.cn

================================================================================
来源：http://hzu.c1oappe.top

S. C / C++ 专题
来源：http://jss.jiagoushi.top

================================================================================
来源：http://byy.xingfuxueyuan.xyz

[S01] C：Hello World
来源：http://mdf.ydzc1.top

#include <stdio.h>
来源：http://xjy.yj202588.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://iun.shuidangran.top

[S02] C：变量与格式化输出
来源：http://tzr.shuidangran.top

int a = 10; printf("%d\n", a);
来源：http://ahh.guannengcc.top

[S03] C：读入整数
来源：http://nes.guannengcc.top

int x; scanf("%d", &x);
来源：http://mib.cashguo.top

[S04] C：字符串复制
来源：http://woq.tarul.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vyh.fehbvm.com

[S05] C：字符串长度
来源：http://yyb.yongpay.top

strlen(s)
来源：http://mtp.ivvv.top

[S06] C：字符串比较
来源：http://twh.hcnkem.com

strcmp(a, b) == 0
来源：http://mdg.nanxinkj.top

[S07] C：数组遍历求和
来源：http://ukf.hcnkem.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jjx.ivvv.top

[S08] C：动态内存分配与释放
来源：http://tog.cqqwz.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mqv.yangfankeji.com

[S09] C：结构体定义与初始化
来源：http://pdi.uphjek.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ddm.pycfn.com

[S10] C：指针与解引用
来源：http://wel.jyoumei.cn

int *p = &a;  *p = 5;
来源：http://bsn.tian-w.cn

[S11] C：逐行读文件
来源：http://cuc.jinqigfzy.top

FILE *f = fopen("a.txt", "r");
来源：http://pis.xinyue.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://fwj.shzxlz.cn

fclose(f);
来源：http://hjk.xziqi.cn

[S12] C：写文件
来源：http://imh.daria6918.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bsx.wangdashe.top

[S13] C：宏定义
来源：http://wbd.ppjwa.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sma.dashuyun.cn

[S14] C：枚举
来源：http://wug.cheryme.top

enum Color { RED, GREEN, BLUE };
来源：http://inw.daxiang520.top

[S15] C：类型转换
来源：http://hil.tian-w.cn

(double) a / b
来源：http://mbu.kuanghao11.cn

[S16] C：位操作置位
来源：http://kvi.smart0.xyz

x |= (1 << 3);
来源：http://pbw.sufxvd.cn

[S17] C：安全拼接字符串
来源：http://pbi.yj20258888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xct.bjfxy.top

[S18] C：命令行参数
来源：http://aam.pengpengdd.cyou

int main(int argc, char **argv)
来源：http://iyp.gotoacloud.top

[S19] C：快速排序
来源：http://fei.xylfe.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jkr.redwolf501.top

[S20] C：二分查找
来源：http://pnp.hywenlv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gpi.9152youxi.cn

[S21] C：字符类别判断
来源：http://hzg.zhiwuduotai.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ipw.vehdjk.com

[S22] C：字符串转数字
来源：http://pjk.zycfv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bau.shanyushiyangkeji.top

[S23] C：随机数
来源：http://dtc.pycfn.com

srand(time(NULL));  int r = rand() % 100;
来源：http://kid.shanyushiyangkeji.top

[S24] C：获取本地时间
来源：http://zzu.cheryme.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wix.yj202588.top

[S25] C：内存拷贝
来源：http://nih.zhoulong.xyz

memcpy(dst, src, n);
来源：http://oza.gzhubu.top

[S26] C：内存清零
来源：http://hsi.yongpay.top

memset(a, 0, sizeof a);
来源：http://rwq.jinqigufen.top

[S27] C：定义常量
来源：http://scc.zhiwuduotai.top

const double PI = 3.14159;
来源：http://ila.dianchejie.cn

[S28] C：静态变量
来源：http://qae.cdnleiting.top

static int counter = 0;
来源：http://bfh.guowangkeji.top

[S29] C：变参函数
来源：http://nul.hywenlv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yek.xinyue.icu

[S30] C：头文件保护
来源：http://cau.yj20258888.top

#ifndef X_H
来源：http://uxw.sjlbkw.cn

#define X_H
来源：http://ubh.chenjidiqi.icu

#endif
来源：http://quc.yangfankeji.com

[S31] C++：Hello World
来源：http://mtn.xingfuxueyuan.xyz

#include <iostream>
来源：http://rmo.iojbl.cn

int main() { std::cout << "Hello\n"; }
来源：http://afi.shzxlz.cn

[S32] C++：字符串
来源：http://psg.sufxvd.cn

std::string s = "hi";  s += "!";
来源：http://mfl.zdbjq.cn

[S33] C++：vector 增删
来源：http://jam.uphjek.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cgx.vqdsnc.cn

[S34] C++：遍历 vector
来源：http://rqn.hammf.cn

for (auto &x : v) { std::cout << x; }
来源：http://lqp.kuanghao11.cn

[S35] C++：map
来源：http://gmj.iojbl.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://emq.vehdjk.com

[S36] C++：unordered_map
来源：http://hvg.wangdashe.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gin.birdmap.top

[S37] C++：set
来源：http://umf.vehdjk.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lou.hongshengwenyu.top

[S38] C++：排序
来源：http://mlw.zhixingplan.top

std::sort(v.begin(), v.end());
来源：http://pfr.feifeiyinyue.top

[S39] C++：自定义比较器排序
来源：http://nyy.shzxlz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fhs.fanxiaobao.xyz

[S40] C++：查找元素
来源：http://xyx.jyoumei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wmt.epnwcf.com

[S41] C++：类与构造函数
来源：http://tfc.52xcode.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://syd.daxiang520.top

[S42] C++：继承与虚函数
来源：http://hnh.tianlin.xyz

class B : public Base { public: void f() override {} };
来源：http://tip.sjlbkw.cn

[S43] C++：智能指针
来源：http://xtf.52xcode.cn

auto p = std::make_unique<int>(5);
来源：http://fnd.tian-w.cn

[S44] C++：引用传参
来源：http://lau.ydzc1.top

void inc(int &x) { ++x; }
来源：http://pic.zhixingplan.top

[S45] C++：lambda
来源：http://xyt.vqdsnc.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fta.zdbjq.cn

[S46] C++：函数模板
来源：http://nvb.meibo888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xpp.fzhhl.top

[S47] C++：结构化绑定遍历
来源：http://hlq.yvedp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kty.jinyuanbaomall.cn

[S48] C++：逐行读文件
来源：http://bts.ivvv.top

std::ifstream in("a.txt");  std::string line;
来源：http://ouh.quarkkingdee.top

while (std::getline(in, line)) { }
来源：http://uwh.52xcode.cn

[S49] C++：写文件
来源：http://ily.dashuyun.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ppp.ybcxt.top

[S50] C++：格式化数字
来源：http://epu.zdqjudy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qqn.316326.xyz

[S51] C++：显式类型转换
来源：http://yhx.hammf.cn

static_cast<double>(a) / b
来源：http://muh.dianchejie.cn

[S52] C++：const 与 noexcept
来源：http://lxt.cucudq.cn

int size() const noexcept { return n_; }
来源：http://sje.chenlongwang.top

[S53] C++：移动语义
来源：http://xia.fzhhl.top

std::vector<int> w = std::move(v);
来源：http://lcb.ybcxt.top

[S54] C++：异常处理
来源：http://vvl.bbcook.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xke.bjfxy.top

[S55] C++：结构化绑定
来源：http://anl.jlsjyb.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jup.yangfankeji.com

[S56] C++：optional
来源：http://bhw.gaohongyu789.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://flw.cdnleiting.top

[S57] C++：编译期常量
来源：http://xke.hysaishi.cn

constexpr int N = 10;
来源：http://fmx.cucudq.cn

[S58] C++：命名空间
来源：http://wcv.hongshengwenyu.top

namespace ns { int f() { return 1; } }
来源：http://ksv.jianghu66.top

[S59] C++：静态断言
来源：http://umn.shanyushiyangtech.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pug.hesvh.cn

[S60] C++：遍历并删除元素
来源：http://ian.zhixingplan.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fvi.tian-w.cn

================================================================================
来源：http://lzx.zhengqikj.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fxz.cqqwz.cn

================================================================================
来源：http://yko.xylfe.cn

[T01] Kotlin：Hello World
来源：http://nfg.nanxuanxn.top

println("Hello")
来源：http://fkr.svipenyu.cn

[T02] Kotlin：变量
来源：http://qyr.shangyingyoupin.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yge.0kj1m.cn

[T03] Kotlin：字符串模板
来源：http://bhg.uphjek.com

"值: $b"
来源：http://zul.tianlin.xyz

[T04] Kotlin：空安全
来源：http://buv.zhengqikj.top

val n: String? = null;  n?.length
来源：http://cij.daria6918.cn

[T05] Kotlin：when 表达式
来源：http://hvq.jyoumei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nri.gaohongyu789.top

[T06] Kotlin：集合映射
来源：http://nge.bjfxy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://kjl.zhixingplan.top

[T07] Kotlin：集合过滤
来源：http://lni.zhengqikj.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://jqu.gzhubu.top

[T08] Kotlin：数据类
来源：http://oqr.chenlongwang.top

data class User(val name: String, val age: Int)
来源：http://ynv.jinghuilouyu.cn

[T09] Kotlin：扩展函数
来源：http://ijd.zhoulong.xyz

fun String.exclaim() = this + "!"
来源：http://hmu.tanke756.top

[T10] Kotlin：默认参数
来源：http://jtd.jianghu66.top

fun greet(name: String = "World") = "Hi $name"
来源：http://gej.gaohongyu789.top

[T11] Kotlin：协程
来源：http://xas.shzxlz.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://tgb.ydjk.org.cn

[T12] Kotlin：解构声明
来源：http://krz.ctjpmb.com

val (a, b) = Pair(1, 2)
来源：http://jeh.snrcjt.cn

[T13] Kotlin：只读 Map
来源：http://loh.yonumen.top

val m = mapOf("a" to 1)
来源：http://ovh.bbcook.cn

[T14] Kotlin：循环
来源：http://hna.gaohongyu789.top

for (i in 1..10) println(i)
来源：http://kph.0kj1m.cn

[T15] Kotlin：接口
来源：http://byw.chenlongwang.top

interface Shape { fun area(): Double }
来源：http://gtu.ctjpmb.com

[T16] Swift：Hello World
来源：http://yvl.tanke756.top

print("Hello")
来源：http://exe.kuanghao11.cn


<!-- 参考信息 -->