代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://vje.wangdashe.top

[R14] C 风格 for
来源：http://lpk.316326.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rbd.wangshuangyany.cn

[R15] while 逐行读文件
来源：http://kdq.hongshengwenyu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jyl.yanxiufei.cn

[R16] until 等待条件
来源：http://btw.0kj1m.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hsz.zhiwuduotai.top

[R17] 数组定义与取值
来源：http://vir.zhiwuduotai.top

arr=(a b c); echo "${arr[0]}"
来源：http://eey.chenzaomai.com

[R18] 遍历数组
来源：http://fca.fehbvm.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://snh.chenjidiqi.icu

[R19] 数组长度
来源：http://okr.jinqigfzy.top

echo "${#arr[@]}"
来源：http://zvm.yuanzhike.top

[R20] 关联数组（字典）
来源：http://ilw.shanyushiyangtech.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ivz.yvedp.cn

[R21] 字符串长度
来源：http://bfh.cashguo.top

echo "${#s}"
来源：http://vxf.xinyue.icu

[R22] 截取子串
来源：http://wmv.snrcjt.cn

echo "${s:0:5}"
来源：http://fnh.guowangkeji.top

[R23] 字符串替换
来源：http://afp.fehbvm.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bup.cashguo.top

[R24] 大小写转换
来源：http://bpg.sxryk.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qiz.yangfankeji.com

[R25] 去后缀 / 去前缀
来源：http://lgc.snrcjt.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fer.9152youxi.cn

[R26] 命令替换
来源：http://tok.chenlongwang.top

now=$(date +%F); echo "$now"
来源：http://qvs.9152youxi.cn

[R27] 算术展开
来源：http://wzj.hysaishi.cn

echo $((1 + 2 * 3))
来源：http://dhd.daria6918.cn

[R28] 浮点运算
来源：http://giz.hfpthk.cn

echo "scale=2; 10/3" | bc
来源：http://uly.fzhhl.top

[R29] 定义函数
来源：http://upi.yueranfly.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ebx.gotoacloud.top

[R30] 函数返回状态码
来源：http://trx.yueranfly.top

f() { return 0; }; f || echo "失败了"
来源：http://mei.ybcxt.top

[R31] 局部变量
来源：http://kcg.pengpengdd.cyou

f() { local x=1; echo "$x"; }
来源：http://fpa.ppjwa.cn

[R32] 参数个数校验
来源：http://fzr.andypj.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wwi.birdmap.top

[R33] 捕获错误并提示行号
来源：http://hgp.zdqjudy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oce.snrcjt.cn

[R34] 退出时清理
来源：http://xdw.c1oappe.top

trap 'rm -f "$tmp"' EXIT
来源：http://kxl.sufxvd.cn

[R35] 后台执行并等待
来源：http://cbz.ppjwa.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zpy.bbcook.cn

[R36] 并发执行多个任务
来源：http://hqj.andypj.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uhe.meibo888.top

[R37] 把输出赋给变量
来源：http://nub.jqgufenzy.top

files=$(ls -1)
来源：http://xyf.zdbjq.cn

[R38] 管道串联
来源：http://nix.tianlin.xyz

cat a.txt | grep -i error | wc -l
来源：http://zmq.birdmap.top

[R39] 重定向标准输出与错误
来源：http://nmr.guannengcc.top

cmd > out.log 2>&1
来源：http://lsi.yj20258888.top

[R40] 追加写日志
来源：http://uus.bjfxy.top

echo "log" >> out.log
来源：http://lxv.fehbvm.com

[R41] 丢弃输出
来源：http://kaq.birdmap.top

cmd >/dev/null 2>&1
来源：http://fge.yueranfly.top

[R42] 输入重定向
来源：http://loj.shangyingyoupin.top

wc -l < a.txt
来源：http://wpp.yueranfly.top

[R43] 按名字查找文件
来源：http://gju.chenzaomai.com

find . -name "*.log" -type f
来源：http://jph.daxiang520.top

[R44] 按修改时间查找
来源：http://dhh.hnqzz.top

find . -mtime -7 -type f
来源：http://ldv.xylfe.cn

[R45] 批量删除
来源：http://oih.daria6918.cn

find . -name "*.tmp" -delete
来源：http://tzk.tanke756.top

[R46] 递归替换文件内容
来源：http://hie.hywenlv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uil.svipenyu.cn

[R47] sed 单行替换
来源：http://amr.havefunace.top

sed -i 's/foo/bar/g' a.txt
来源：http://izy.shanyushiyangkeji.top

[R48] awk 取指定列
来源：http://ylq.epnwcf.com

awk '{print $1, $3}' a.txt
来源：http://xgr.guowangkeji.top

[R49] awk 带条件
来源：http://jhp.gaohongyu789.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cgj.sufxvd.cn

[R50] awk 求和
来源：http://xqx.yj20258.top

awk '{s += $2} END {print s}' a.txt
来源：http://gvw.aizwys.cn

[R51] 排序去重取前几
来源：http://jxh.aibaodan.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sqp.yongpay.top

[R52] 统计行数
来源：http://ine.ydzc1.top

wc -l a.txt
来源：http://dko.ywan-chungtsiang.top

[R53] 查看文件头与实时尾
来源：http://asn.xziqi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bcj.nwbrower.top

[R54] 比较两个文件
来源：http://xcm.shanyushiyangtech.top

diff a.txt b.txt
来源：http://huk.bbcook.cn

[R55] 压缩与解压
来源：http://vjq.zhoulong.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gmi.yj20258.top

[R56] 远程拷贝
来源：http://rpl.smart0.xyz

scp file user@host:/path/
来源：http://wjs.iojbl.cn

[R57] 远程执行命令
来源：http://oqo.shanyushiyangkeji.top

ssh user@host 'uptime'
来源：http://riq.yangfankeji.com

[R58] 下载文件
来源：http://gct.zhaomingkeji.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ljf.zhoulong.xyz

[R59] 发 POST JSON
来源：http://bul.birdmap.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dzj.sysykeji.top

[R60] 只看 HTTP 状态码
来源：http://aeb.sufxvd.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rjs.jinghuilouyu.cn

[R61] 磁盘占用
来源：http://pii.pycfn.com

df -h;  du -sh *
来源：http://dbf.cheryme.top

[R62] 找最占空间的文件
来源：http://yja.yueranfly.top

du -ah . | sort -rh | head -10
来源：http://ofc.guannengcc.top

[R63] 内存与进程
来源：http://xhc.sxryk.cn

free -h;  ps aux | grep nginx
来源：http://ulr.meibo888.top

[R64] 结束进程
来源：http://aoh.andypj.xyz

kill -9 $(pgrep -f app.py)
来源：http://svj.meibo888.top

[R65] 查看端口占用
来源：http://pff.quarkkingdee.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ldn.yfazqb.com

[R66] 定时任务
来源：http://izh.9152youxi.cn

crontab -e;  crontab -l
来源：http://bzu.9152youxi.cn

[R67] 生成随机十六进制串
来源：http://pis.zhixingplan.top

openssl rand -hex 16
来源：http://fml.xinyue.icu

[R68] 计算文件校验值
来源：http://mim.jiagoushi.top

sha256sum a.txt;  md5sum a.txt
来源：http://uki.fktsv.cn

[R69] 生成随机密码
来源：http://dty.sufxvd.cn

head -c 16 /dev/urandom | base64
来源：http://fgp.cheryme.top

[R70] 时间戳与互转
来源：http://dok.ppjwa.cn

date +%s;  date -d @1700000000
来源：http://fky.zhijiandao.cn

[R71] 日期格式化
来源：http://cot.chenlongwang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vns.svipenyu.cn

[R72] 等待端口就绪
来源：http://lww.zhixingplan.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nel.dianchejie.cn

[R73] 分割大日志
来源：http://ecn.tanke756.top

split -l 1000 big.log part_
来源：http://kth.gogol.net.cn

[R74] 批量重命名
来源：http://iaq.cdnleiting.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tgl.zhengqikj.top

[R75] 导出环境变量
来源：http://nzj.uphjek.com

export PATH="$HOME/bin:$PATH"
来源：http://lkx.0kj1m.cn

[R76] 使用临时文件
来源：http://oqb.gotoacloud.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://alf.redwolf501.top

[R77] 读取用户输入
来源：http://ont.aizwys.cn

read -rp "请输入: " ans
来源：http://dqc.chenzaomai.com

[R78] 交互式菜单
来源：http://krj.daxiang520.top

select opt in a b c; do echo "$opt"; break; done
来源：http://kgt.zhiwuduotai.top

[R79] 解析命令行选项
来源：http://ilg.shuidangran.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bvq.birdmap.top

[R80] 查看脚本执行耗时
来源：http://npz.sjlbkw.cn

time ./run.sh
来源：http://mky.yongpay.top

================================================================================
来源：http://hes.zhiwuduotai.top

S. C / C++ 专题
来源：http://vsp.daxiang520.top

================================================================================
来源：http://cxd.shuidangran.top

[S01] C：Hello World
来源：http://lxj.vehdjk.com

#include <stdio.h>
来源：http://iox.zdbjq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pkl.hammf.cn

[S02] C：变量与格式化输出
来源：http://cgi.hesvh.cn

int a = 10; printf("%d\n", a);
来源：http://moz.cashguo.top

[S03] C：读入整数
来源：http://trg.fanxiaobao.xyz

int x; scanf("%d", &x);
来源：http://tal.shanyushiyangkeji.top

[S04] C：字符串复制
来源：http://cap.jqgufenzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://igk.yfazqb.com

[S05] C：字符串长度
来源：http://rco.jinqigufen.top

strlen(s)
来源：http://rij.aizwys.cn

[S06] C：字符串比较
来源：http://sce.jinghuilouyu.cn

strcmp(a, b) == 0
来源：http://bds.redwolf501.top

[S07] C：数组遍历求和
来源：http://geg.bjfxy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vzz.chenlongwang.top

[S08] C：动态内存分配与释放
来源：http://pxy.zhaomingkeji.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bbg.xziqi.cn

[S09] C：结构体定义与初始化
来源：http://ipl.hnxiangtu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kfz.epnwcf.com

[S10] C：指针与解引用
来源：http://hbq.ehwqpu.com

int *p = &a;  *p = 5;
来源：http://fgy.cdnleiting.top

[S11] C：逐行读文件
来源：http://nuo.hysaishi.cn

FILE *f = fopen("a.txt", "r");
来源：http://wid.yj202588.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://dvz.zdqjudy.top

fclose(f);
来源：http://wzz.mhx1999.top

[S12] C：写文件
来源：http://tql.cucudq.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fns.yj20258.top

[S13] C：宏定义
来源：http://kiv.quarkkingdee.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zqz.shuidangran.top

[S14] C：枚举
来源：http://fck.jinyuanbaomall.cn

enum Color { RED, GREEN, BLUE };
来源：http://jwh.tianlin.xyz

[S15] C：类型转换
来源：http://ool.quarkkingdee.top

(double) a / b
来源：http://rnp.yonumen.top

[S16] C：位操作置位
来源：http://eyr.zhoulong.xyz

x |= (1 << 3);
来源：http://ngb.pengpengdd.cyou

[S17] C：安全拼接字符串
来源：http://bqk.jinqigfzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://axz.daxiang520.top

[S18] C：命令行参数
来源：http://kad.shanyushiyangtech.top

int main(int argc, char **argv)
来源：http://icq.chenlongwang.top

[S19] C：快速排序
来源：http://lub.dashuyun.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hxy.ppjwa.cn

[S20] C：二分查找
来源：http://zcq.zycfv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qtv.fanxiaobao.xyz

[S21] C：字符类别判断
来源：http://szw.yj202588.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nnd.tianlin.xyz

[S22] C：字符串转数字
来源：http://fzm.hesvh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sfy.gotoacloud.top

[S23] C：随机数
来源：http://qbm.smart0.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://ciy.xuetiantiany.cn

[S24] C：获取本地时间
来源：http://gnf.aibaodan.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sfj.cucudq.cn

[S25] C：内存拷贝
来源：http://hss.aibaodan.cn

memcpy(dst, src, n);
来源：http://syq.gaohongyu789.top

[S26] C：内存清零
来源：http://rpu.zdqjudy.top

memset(a, 0, sizeof a);
来源：http://tzg.jiagoushi.top

[S27] C：定义常量
来源：http://yxx.jinyuanbaomall.cn

const double PI = 3.14159;
来源：http://fad.cdnleiting.top

[S28] C：静态变量
来源：http://pdp.shzxlz.cn

static int counter = 0;
来源：http://btz.chenzaomai.com

[S29] C：变参函数
来源：http://yjl.sufxvd.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://efs.316326.xyz

[S30] C：头文件保护
来源：http://mkg.dianchejie.cn

#ifndef X_H
来源：http://por.cucudq.cn

#define X_H
来源：http://fbh.andypj.xyz

#endif
来源：http://yum.zdbjq.cn

[S31] C++：Hello World
来源：http://owx.shanyushiyangkeji.top

#include <iostream>
来源：http://kcs.birdmap.top

int main() { std::cout << "Hello\n"; }
来源：http://rbl.sufxvd.cn

[S32] C++：字符串
来源：http://ytl.svipenyu.cn

std::string s = "hi";  s += "!";
来源：http://ibj.jianghu66.top

[S33] C++：vector 增删
来源：http://zfh.jqgfzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ztn.zhaomingkeji.xyz

[S34] C++：遍历 vector
来源：http://fvu.svipenyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://qpw.epnwcf.com

[S35] C++：map
来源：http://vcj.aizwys.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qwb.cqqwz.cn

[S36] C++：unordered_map
来源：http://bnl.aizwys.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://odf.xingfuxueyuan.xyz

[S37] C++：set
来源：http://nxy.ydzc1.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kou.feifeiyinyue.top

[S38] C++：排序
来源：http://xlc.smart0.xyz

std::sort(v.begin(), v.end());
来源：http://xdn.svipenyu.cn

[S39] C++：自定义比较器排序
来源：http://jge.chenjidiqi.icu

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gqu.chenlongwang.top

[S40] C++：查找元素
来源：http://koc.jiagoushi.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ybr.c1oappe.top

[S41] C++：类与构造函数
来源：http://aoa.hesvh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bov.shangyingyoupin.top

[S42] C++：继承与虚函数
来源：http://kwm.daxiang520.top

class B : public Base { public: void f() override {} };
来源：http://tuw.svipenyu.cn

[S43] C++：智能指针
来源：http://izd.ehwqpu.com

auto p = std::make_unique<int>(5);
来源：http://yrn.fehbvm.com

[S44] C++：引用传参
来源：http://onm.ybcxt.top

void inc(int &x) { ++x; }
来源：http://lda.shangyingyoupin.top

[S45] C++：lambda
来源：http://kwy.meibo888.top

auto add = [](int a, int b) { return a + b; };
来源：http://rlm.c1oappe.top

[S46] C++：函数模板
来源：http://wjv.jyoumei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fvj.zdbjq.cn

[S47] C++：结构化绑定遍历
来源：http://bod.hnxiangtu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vnl.hongshengwenyu.top

[S48] C++：逐行读文件
来源：http://rdd.yj202588.top

std::ifstream in("a.txt");  std::string line;
来源：http://jql.xuanzx.com

while (std::getline(in, line)) { }
来源：http://cqk.cqqwz.cn

[S49] C++：写文件
来源：http://nco.shzxlz.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lew.guowangkeji.top

[S50] C++：格式化数字
来源：http://shl.havefunace.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hjj.tianlin.xyz

[S51] C++：显式类型转换
来源：http://nug.ivvv.top

static_cast<double>(a) / b
来源：http://hul.zhaomingkeji.xyz

[S52] C++：const 与 noexcept
来源：http://dng.dashuyun.cn

int size() const noexcept { return n_; }
来源：http://zbv.ydzc1.top

[S53] C++：移动语义
来源：http://zuz.jqgfzy.top

std::vector<int> w = std::move(v);
来源：http://rix.shangyingyoupin.top

[S54] C++：异常处理
来源：http://kbm.yongpay.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ygx.cashguo.top

[S55] C++：结构化绑定
来源：http://fzu.jinqigfzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tjc.zdqjudy.top

[S56] C++：optional
来源：http://myq.yangfankeji.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wki.uphjek.com

[S57] C++：编译期常量
来源：http://csu.aizwys.cn

constexpr int N = 10;
来源：http://oqc.sweek.top

[S58] C++：命名空间
来源：http://uie.ppjwa.cn

namespace ns { int f() { return 1; } }
来源：http://rhs.zhongyouzk.top

[S59] C++：静态断言
来源：http://pop.pycfn.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vmb.wangshuangyany.cn

[S60] C++：遍历并删除元素
来源：http://pdx.bbcook.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mkn.yongpay.top

================================================================================
来源：http://hpy.hcnkem.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bni.tarul.cn

================================================================================
来源：http://qjp.daria6918.cn

[T01] Kotlin：Hello World
来源：http://meq.tianlin.xyz

println("Hello")
来源：http://kzi.hnqzz.top

[T02] Kotlin：变量
来源：http://tpz.yonumen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://npw.jiagoushi.top

[T03] Kotlin：字符串模板
来源：http://fdw.xuetiantiany.cn

"值: $b"
来源：http://qow.zhongyouzk.top

[T04] Kotlin：空安全
来源：http://acu.tianlin.xyz

val n: String? = null;  n?.length
来源：http://zlb.shanyushiyangtech.top

[T05] Kotlin：when 表达式
来源：http://gok.tarul.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://any.shangyingyoupin.top

[T06] Kotlin：集合映射
来源：http://nfw.daria6918.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cxh.52xcode.cn

[T07] Kotlin：集合过滤
来源：http://bue.fengsongda.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nbv.0kj1m.cn

[T08] Kotlin：数据类
来源：http://abp.cashguo.top

data class User(val name: String, val age: Int)
来源：http://vjv.cheryme.top

[T09] Kotlin：扩展函数
来源：http://nqk.pycfn.com

fun String.exclaim() = this + "!"
来源：http://lsl.zycfv.cn

[T10] Kotlin：默认参数
来源：http://lqg.sweek.top

fun greet(name: String = "World") = "Hi $name"
来源：http://bma.zhoulong.xyz

[T11] Kotlin：协程
来源：http://beq.ybcxt.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://nkb.zhongyouzk.top

[T12] Kotlin：解构声明
来源：http://jal.guannengcc.top

val (a, b) = Pair(1, 2)
来源：http://bwr.yangfankeji.com

[T13] Kotlin：只读 Map
来源：http://eyo.xingfuxueyuan.xyz

val m = mapOf("a" to 1)
来源：http://urx.andypj.xyz

[T14] Kotlin：循环
来源：http://aph.zhaomingkeji.xyz

for (i in 1..10) println(i)
来源：http://pmz.yfazqb.com

[T15] Kotlin：接口
来源：http://vjm.jianghu66.top

interface Shape { fun area(): Double }
来源：http://sdl.guowangkeji.top

[T16] Swift：Hello World
来源：http://nvw.jqgfzy.top

print("Hello")
来源：http://vjd.xylfe.cn


<!-- 参考信息 -->