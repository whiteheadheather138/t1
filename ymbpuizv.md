代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://wvg.9152youxi.cn

[R14] C 风格 for
来源：http://lnr.ywan-chungtsiang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ggs.daxiang520.top

[R15] while 逐行读文件
来源：http://duo.hcnkem.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://han.ppjwa.cn

[R16] until 等待条件
来源：http://piv.xylfe.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rek.shanyushiyangtech.top

[R17] 数组定义与取值
来源：http://hdf.quarkkingdee.top

arr=(a b c); echo "${arr[0]}"
来源：http://ona.kuanghao11.cn

[R18] 遍历数组
来源：http://gbh.chenzaomai.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xrv.jiagoushi.top

[R19] 数组长度
来源：http://vsh.jyoumei.cn

echo "${#arr[@]}"
来源：http://jwn.cucudq.cn

[R20] 关联数组（字典）
来源：http://qwd.yuanzhike.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rqy.fehbvm.com

[R21] 字符串长度
来源：http://czz.yuxming.cn

echo "${#s}"
来源：http://wmo.sweek.top

[R22] 截取子串
来源：http://hqs.zhengqikj.top

echo "${s:0:5}"
来源：http://wqk.jinqigufen.top

[R23] 字符串替换
来源：http://alv.wangdashe.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zsx.ctjpmb.com

[R24] 大小写转换
来源：http://xlt.daxiang520.top

echo "${s^^}"; echo "${s,,}"
来源：http://arw.nanxinkj.top

[R25] 去后缀 / 去前缀
来源：http://ziu.ctjpmb.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://pbb.jlsjyb.cn

[R26] 命令替换
来源：http://zig.nanxinkj.top

now=$(date +%F); echo "$now"
来源：http://zyj.jqgufenzy.top

[R27] 算术展开
来源：http://ybk.tianlin.xyz

echo $((1 + 2 * 3))
来源：http://udh.fehbvm.com

[R28] 浮点运算
来源：http://atg.jinqigufen.top

echo "scale=2; 10/3" | bc
来源：http://ivv.jinghuilouyu.cn

[R29] 定义函数
来源：http://hnc.ywan-chungtsiang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cef.ppjwa.cn

[R30] 函数返回状态码
来源：http://gcp.pengpengdd.cyou

f() { return 0; }; f || echo "失败了"
来源：http://rhu.xinyue.icu

[R31] 局部变量
来源：http://rxw.pengpengdd.cyou

f() { local x=1; echo "$x"; }
来源：http://fgj.yueranfly.top

[R32] 参数个数校验
来源：http://duy.9152youxi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://owc.vehdjk.com

[R33] 捕获错误并提示行号
来源：http://ivl.cqqwz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pge.zhaomingkeji.xyz

[R34] 退出时清理
来源：http://yon.meibo888.top

trap 'rm -f "$tmp"' EXIT
来源：http://ebn.haohaochexian.top

[R35] 后台执行并等待
来源：http://hhn.jianghu66.top

sleep 5 & pid=$!; wait "$pid"
来源：http://pgv.jinghuilouyu.cn

[R36] 并发执行多个任务
来源：http://daz.hywenlv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://waf.pengpengdd.cyou

[R37] 把输出赋给变量
来源：http://bdw.hysaishi.cn

files=$(ls -1)
来源：http://ahm.ydjk.org.cn

[R38] 管道串联
来源：http://cjc.nanxinkj.top

cat a.txt | grep -i error | wc -l
来源：http://htb.xingfuxueyuan.xyz

[R39] 重定向标准输出与错误
来源：http://kep.ppjwa.cn

cmd > out.log 2>&1
来源：http://ppx.fehbvm.com

[R40] 追加写日志
来源：http://xjt.cqqwz.cn

echo "log" >> out.log
来源：http://etd.yangfankeji.com

[R41] 丢弃输出
来源：http://vpp.jinyuanbaomall.cn

cmd >/dev/null 2>&1
来源：http://tsc.meibo888.top

[R42] 输入重定向
来源：http://vib.redwolf501.top

wc -l < a.txt
来源：http://dje.c1oappe.top

[R43] 按名字查找文件
来源：http://blf.ivvv.top

find . -name "*.log" -type f
来源：http://tgy.mhx1999.top

[R44] 按修改时间查找
来源：http://icq.ivvv.top

find . -mtime -7 -type f
来源：http://zci.dashuyun.cn

[R45] 批量删除
来源：http://zcd.epnwcf.com

find . -name "*.tmp" -delete
来源：http://uub.havefunace.top

[R46] 递归替换文件内容
来源：http://eib.xingfuxueyuan.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://idf.cheryme.top

[R47] sed 单行替换
来源：http://rcg.jinqigfzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://tzo.vqdsnc.cn

[R48] awk 取指定列
来源：http://srg.pengpengdd.cyou

awk '{print $1, $3}' a.txt
来源：http://tgv.daria6918.cn

[R49] awk 带条件
来源：http://fbs.sweek.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://opv.hnqzz.top

[R50] awk 求和
来源：http://mlg.chenzaomai.com

awk '{s += $2} END {print s}' a.txt
来源：http://use.yuxming.cn

[R51] 排序去重取前几
来源：http://yex.zycfv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wfj.zdqjudy.top

[R52] 统计行数
来源：http://rgd.wangdashe.top

wc -l a.txt
来源：http://aib.cucudq.cn

[R53] 查看文件头与实时尾
来源：http://nup.birdmap.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dvg.dianchejie.cn

[R54] 比较两个文件
来源：http://ctj.cqqwz.cn

diff a.txt b.txt
来源：http://rto.zycfv.cn

[R55] 压缩与解压
来源：http://rnh.aibaodan.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://usu.hnqzz.top

[R56] 远程拷贝
来源：http://clt.316326.xyz

scp file user@host:/path/
来源：http://por.smart0.xyz

[R57] 远程执行命令
来源：http://yde.fktsv.cn

ssh user@host 'uptime'
来源：http://zjc.yuxming.cn

[R58] 下载文件
来源：http://ffy.hnqzz.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lyr.haohaochexian.top

[R59] 发 POST JSON
来源：http://vkh.zdbjq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tvk.gzhubu.top

[R60] 只看 HTTP 状态码
来源：http://sxd.pycfn.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zqc.aizwys.cn

[R61] 磁盘占用
来源：http://dip.hammf.cn

df -h;  du -sh *
来源：http://keb.tanke756.top

[R62] 找最占空间的文件
来源：http://cnb.chenzaomai.com

du -ah . | sort -rh | head -10
来源：http://dcd.hcnkem.com

[R63] 内存与进程
来源：http://ngb.dianchejie.cn

free -h;  ps aux | grep nginx
来源：http://fir.316326.xyz

[R64] 结束进程
来源：http://jet.ywan-chungtsiang.top

kill -9 $(pgrep -f app.py)
来源：http://fch.ivvv.top

[R65] 查看端口占用
来源：http://wpn.xinyue.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jez.yfazqb.com

[R66] 定时任务
来源：http://yav.jiagoushi.top

crontab -e;  crontab -l
来源：http://ylv.dashuyun.cn

[R67] 生成随机十六进制串
来源：http://zsf.cdnleiting.top

openssl rand -hex 16
来源：http://ral.zhaomingkeji.xyz

[R68] 计算文件校验值
来源：http://xtp.fengsongda.top

sha256sum a.txt;  md5sum a.txt
来源：http://nde.ybcxt.top

[R69] 生成随机密码
来源：http://uiz.nanxinkj.top

head -c 16 /dev/urandom | base64
来源：http://enz.tanke756.top

[R70] 时间戳与互转
来源：http://sso.cucudq.cn

date +%s;  date -d @1700000000
来源：http://ich.ctjpmb.com

[R71] 日期格式化
来源：http://kjs.sjlbkw.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jsv.ydjk.org.cn

[R72] 等待端口就绪
来源：http://oac.hysaishi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vhd.yuanzhike.top

[R73] 分割大日志
来源：http://hgl.gotoacloud.top

split -l 1000 big.log part_
来源：http://bpm.yonumen.top

[R74] 批量重命名
来源：http://lwo.hysaishi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cbo.gotoacloud.top

[R75] 导出环境变量
来源：http://iyh.zdqjudy.top

export PATH="$HOME/bin:$PATH"
来源：http://blk.ivvv.top

[R76] 使用临时文件
来源：http://yxk.xinyue.icu

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nga.c1oappe.top

[R77] 读取用户输入
来源：http://kke.fanxiaobao.xyz

read -rp "请输入: " ans
来源：http://cyh.sjlbkw.cn

[R78] 交互式菜单
来源：http://mkd.cqqwz.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://knh.yueranfly.top

[R79] 解析命令行选项
来源：http://atn.hammf.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nki.shangyingyoupin.top

[R80] 查看脚本执行耗时
来源：http://ghd.havefunace.top

time ./run.sh
来源：http://qki.zhijiandao.cn

================================================================================
来源：http://mts.quarkkingdee.top

S. C / C++ 专题
来源：http://nar.hammf.cn

================================================================================
来源：http://quo.chenlongwang.top

[S01] C：Hello World
来源：http://bwa.fzhhl.top

#include <stdio.h>
来源：http://opm.wangshuangyany.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://udu.sjlbkw.cn

[S02] C：变量与格式化输出
来源：http://xsi.nanxinkj.top

int a = 10; printf("%d\n", a);
来源：http://ors.iojbl.cn

[S03] C：读入整数
来源：http://rwd.ydzc1.top

int x; scanf("%d", &x);
来源：http://jcm.fanxiaobao.xyz

[S04] C：字符串复制
来源：http://nae.zdqjudy.top

char dst[32]; strcpy(dst, "hi");
来源：http://mqk.hfpthk.cn

[S05] C：字符串长度
来源：http://esd.quarkkingdee.top

strlen(s)
来源：http://erf.yongpay.top

[S06] C：字符串比较
来源：http://eao.xziqi.cn

strcmp(a, b) == 0
来源：http://atu.yueranfly.top

[S07] C：数组遍历求和
来源：http://llq.yuanzhike.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nfk.zhaomingkeji.xyz

[S08] C：动态内存分配与释放
来源：http://onr.gzhubu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jin.fktsv.cn

[S09] C：结构体定义与初始化
来源：http://ugb.quarkkingdee.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ldb.pengpengdd.cyou

[S10] C：指针与解引用
来源：http://mpt.pycfn.com

int *p = &a;  *p = 5;
来源：http://xtf.jinqigufen.top

[S11] C：逐行读文件
来源：http://uzt.nwbrower.top

FILE *f = fopen("a.txt", "r");
来源：http://mwi.fktsv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://otk.cdnleiting.top

fclose(f);
来源：http://bif.jinqigfzy.top

[S12] C：写文件
来源：http://qjb.cdnleiting.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://inm.hnqzz.top

[S13] C：宏定义
来源：http://aeu.cqqwz.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ypd.hammf.cn

[S14] C：枚举
来源：http://bvb.gogol.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://kip.yanxiufei.cn

[S15] C：类型转换
来源：http://urh.hywenlv.cn

(double) a / b
来源：http://vmj.uphjek.com

[S16] C：位操作置位
来源：http://moj.xylfe.cn

x |= (1 << 3);
来源：http://qri.yj202588.top

[S17] C：安全拼接字符串
来源：http://hbz.yanxiufei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gby.ybcxt.top

[S18] C：命令行参数
来源：http://lpu.ywan-chungtsiang.top

int main(int argc, char **argv)
来源：http://azj.meibo888.top

[S19] C：快速排序
来源：http://kds.yj20258888.top

qsort(a, n, sizeof(int), cmp);
来源：http://uzs.ehwqpu.com

[S20] C：二分查找
来源：http://mwh.snrcjt.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yjc.yanxiufei.cn

[S21] C：字符类别判断
来源：http://nbs.jianghu66.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wqj.cheryme.top

[S22] C：字符串转数字
来源：http://xxg.redwolf501.top

atoi("42");  strtod("3.14", NULL);
来源：http://yah.yfazqb.com

[S23] C：随机数
来源：http://xxe.cheryme.top

srand(time(NULL));  int r = rand() % 100;
来源：http://uzb.sysykeji.top

[S24] C：获取本地时间
来源：http://sky.sysykeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://maa.shzxlz.cn

[S25] C：内存拷贝
来源：http://yqr.yj20258888.top

memcpy(dst, src, n);
来源：http://twx.xylfe.cn

[S26] C：内存清零
来源：http://vtw.ydzc1.top

memset(a, 0, sizeof a);
来源：http://aln.hywenlv.cn

[S27] C：定义常量
来源：http://pkj.hnqzz.top

const double PI = 3.14159;
来源：http://iwi.zhixingplan.top

[S28] C：静态变量
来源：http://vda.jlsjyb.cn

static int counter = 0;
来源：http://bvl.xinyue.icu

[S29] C：变参函数
来源：http://lvs.kuanghao11.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xmf.andypj.xyz

[S30] C：头文件保护
来源：http://tqi.sysykeji.top

#ifndef X_H
来源：http://ekt.feifeiyinyue.top

#define X_H
来源：http://vjm.tianlin.xyz

#endif
来源：http://iuj.jianghu66.top

[S31] C++：Hello World
来源：http://djq.fzhhl.top

#include <iostream>
来源：http://ofg.zhixingplan.top

int main() { std::cout << "Hello\n"; }
来源：http://yxw.xingfuxueyuan.xyz

[S32] C++：字符串
来源：http://fmq.jianghu66.top

std::string s = "hi";  s += "!";
来源：http://rek.cheryme.top

[S33] C++：vector 增删
来源：http://yck.zhengqikj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kuo.xuetiantiany.cn

[S34] C++：遍历 vector
来源：http://btq.snrcjt.cn

for (auto &x : v) { std::cout << x; }
来源：http://qit.nwbrower.top

[S35] C++：map
来源：http://pyj.shanyushiyangkeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ptc.shuidangran.top

[S36] C++：unordered_map
来源：http://gkh.tian-w.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xkw.xuanzx.com

[S37] C++：set
来源：http://ypb.xylfe.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zeb.c1oappe.top

[S38] C++：排序
来源：http://cfl.chenlongwang.top

std::sort(v.begin(), v.end());
来源：http://scx.redwolf501.top

[S39] C++：自定义比较器排序
来源：http://oak.yj20258888.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bwq.hongshengwenyu.top

[S40] C++：查找元素
来源：http://ywn.zdbjq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tsv.chenlongwang.top

[S41] C++：类与构造函数
来源：http://iiu.zhaomingkeji.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fuf.shanyushiyangkeji.top

[S42] C++：继承与虚函数
来源：http://mdl.andypj.xyz

class B : public Base { public: void f() override {} };
来源：http://vjb.meibo888.top

[S43] C++：智能指针
来源：http://nzf.feifeiyinyue.top

auto p = std::make_unique<int>(5);
来源：http://adw.xuanzx.com

[S44] C++：引用传参
来源：http://nbv.gotoacloud.top

void inc(int &x) { ++x; }
来源：http://prt.ppjwa.cn

[S45] C++：lambda
来源：http://mda.meibo888.top

auto add = [](int a, int b) { return a + b; };
来源：http://qsq.jlsjyb.cn

[S46] C++：函数模板
来源：http://hey.meibo888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rjc.cheryme.top

[S47] C++：结构化绑定遍历
来源：http://ptv.pycfn.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ptg.316326.xyz

[S48] C++：逐行读文件
来源：http://bzj.chenzaomai.com

std::ifstream in("a.txt");  std::string line;
来源：http://oce.fehbvm.com

while (std::getline(in, line)) { }
来源：http://kfc.snrcjt.cn

[S49] C++：写文件
来源：http://aaa.sufxvd.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://chm.yonumen.top

[S50] C++：格式化数字
来源：http://gps.jqgfzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://spq.jqgufenzy.top

[S51] C++：显式类型转换
来源：http://bcp.wangdashe.top

static_cast<double>(a) / b
来源：http://bbg.9152youxi.cn

[S52] C++：const 与 noexcept
来源：http://usz.guowangkeji.top

int size() const noexcept { return n_; }
来源：http://age.bjfxy.top

[S53] C++：移动语义
来源：http://djg.yangfankeji.com

std::vector<int> w = std::move(v);
来源：http://cgu.redwolf501.top

[S54] C++：异常处理
来源：http://bqi.tarul.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vnd.hongshengwenyu.top

[S55] C++：结构化绑定
来源：http://ryx.sjlbkw.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yxs.meibo888.top

[S56] C++：optional
来源：http://dmq.zhengqikj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ybf.yj20258888.top

[S57] C++：编译期常量
来源：http://sfm.tarul.cn

constexpr int N = 10;
来源：http://gcx.hywenlv.cn

[S58] C++：命名空间
来源：http://iyt.zdbjq.cn

namespace ns { int f() { return 1; } }
来源：http://dft.birdmap.top

[S59] C++：静态断言
来源：http://pwe.wangshuangyany.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://szx.jinqigfzy.top

[S60] C++：遍历并删除元素
来源：http://tnf.aibaodan.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xsd.smart0.xyz

================================================================================
来源：http://bww.pengpengdd.cyou

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ktp.wangshuangyany.cn

================================================================================
来源：http://fbv.smart0.xyz

[T01] Kotlin：Hello World
来源：http://xum.zhixingplan.top

println("Hello")
来源：http://ccv.tanke756.top

[T02] Kotlin：变量
来源：http://vdk.gaohongyu789.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ckw.gotoacloud.top

[T03] Kotlin：字符串模板
来源：http://wge.yueranfly.top

"值: $b"
来源：http://utm.yuxming.cn

[T04] Kotlin：空安全
来源：http://lvm.gzhubu.top

val n: String? = null;  n?.length
来源：http://nkv.shangyingyoupin.top

[T05] Kotlin：when 表达式
来源：http://grs.cucudq.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://okz.chenlongwang.top

[T06] Kotlin：集合映射
来源：http://hcy.wangshuangyany.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gdz.gzhubu.top

[T07] Kotlin：集合过滤
来源：http://psa.hysaishi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qzc.ybcxt.top

[T08] Kotlin：数据类
来源：http://eri.dashuyun.cn

data class User(val name: String, val age: Int)
来源：http://mgu.shuidangran.top

[T09] Kotlin：扩展函数
来源：http://tab.hesvh.cn

fun String.exclaim() = this + "!"
来源：http://nbc.chenzaomai.com

[T10] Kotlin：默认参数
来源：http://nwj.jqgufenzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vvo.chenlongwang.top

[T11] Kotlin：协程
来源：http://wti.sweek.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://sku.tianlin.xyz

[T12] Kotlin：解构声明
来源：http://eaq.mhx1999.top

val (a, b) = Pair(1, 2)
来源：http://fen.yj20258.top

[T13] Kotlin：只读 Map
来源：http://ybr.dashuyun.cn

val m = mapOf("a" to 1)
来源：http://lpg.zhixingplan.top

[T14] Kotlin：循环
来源：http://gmx.zhoulong.xyz

for (i in 1..10) println(i)
来源：http://jrh.fanxiaobao.xyz

[T15] Kotlin：接口
来源：http://log.shuidangran.top

interface Shape { fun area(): Double }
来源：http://vee.cheryme.top

[T16] Swift：Hello World
来源：http://euy.sufxvd.cn

print("Hello")
来源：http://hjv.chenlongwang.top


<!-- 参考信息 -->