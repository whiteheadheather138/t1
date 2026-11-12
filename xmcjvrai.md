代发 wailian999

case "$1" in
来源：http://lxs.smart0.xyz

start) echo "启动" ;;
来源：http://exa.jiagoushi.top

stop)  echo "停止" ;;
来源：http://ude.birdmap.top

*)     echo "未知命令" ;;
来源：http://kls.jiagoushi.top

esac
来源：http://sgp.pengpengdd.cyou

[R12] for 遍历文件
来源：http://kyr.zhijiandao.cn

for f in *.txt; do echo "$f"; done
来源：http://wtx.yvedp.cn

[R13] for 计数循环
来源：http://ojj.yuanzhike.top

for i in {1..10}; do echo "$i"; done
来源：http://myu.gzhubu.top

[R14] C 风格 for
来源：http://sfz.cheryme.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sjc.nanxuanxn.top

[R15] while 逐行读文件
来源：http://ndx.hysaishi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://evz.ydzc1.top

[R16] until 等待条件
来源：http://csa.cashguo.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zqm.gotoacloud.top

[R17] 数组定义与取值
来源：http://ihp.sweek.top

arr=(a b c); echo "${arr[0]}"
来源：http://lpt.wangshuangyany.cn

[R18] 遍历数组
来源：http://myz.ivvv.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bsj.tian-w.cn

[R19] 数组长度
来源：http://zhf.fehbvm.com

echo "${#arr[@]}"
来源：http://mqt.feifeiyinyue.top

[R20] 关联数组（字典）
来源：http://uhg.guannengcc.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ejj.sxryk.cn

[R21] 字符串长度
来源：http://wap.jqgufenzy.top

echo "${#s}"
来源：http://ogg.nanxinkj.top

[R22] 截取子串
来源：http://tox.hongshengwenyu.top

echo "${s:0:5}"
来源：http://fkk.guannengcc.top

[R23] 字符串替换
来源：http://hfi.hongshengwenyu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hce.jyoumei.cn

[R24] 大小写转换
来源：http://yxu.jinyuanbaomall.cn

echo "${s^^}"; echo "${s,,}"
来源：http://luf.fktsv.cn

[R25] 去后缀 / 去前缀
来源：http://ufr.ctjpmb.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://kir.quarkkingdee.top

[R26] 命令替换
来源：http://jpu.chenzaomai.com

now=$(date +%F); echo "$now"
来源：http://ppo.pengpengdd.cyou

[R27] 算术展开
来源：http://cak.smart0.xyz

echo $((1 + 2 * 3))
来源：http://igu.jqgufenzy.top

[R28] 浮点运算
来源：http://ykp.yuanzhike.top

echo "scale=2; 10/3" | bc
来源：http://zci.sjlbkw.cn

[R29] 定义函数
来源：http://dmm.hcnkem.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hpk.0kj1m.cn

[R30] 函数返回状态码
来源：http://yjc.vqdsnc.cn

f() { return 0; }; f || echo "失败了"
来源：http://qyv.vehdjk.com

[R31] 局部变量
来源：http://mse.jlsjyb.cn

f() { local x=1; echo "$x"; }
来源：http://kin.gaohongyu789.top

[R32] 参数个数校验
来源：http://kzm.aizwys.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gdi.xingfuxueyuan.xyz

[R33] 捕获错误并提示行号
来源：http://vmd.ydzc1.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qce.hfpthk.cn

[R34] 退出时清理
来源：http://nyw.ppjwa.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mqe.ehwqpu.com

[R35] 后台执行并等待
来源：http://kfd.ppjwa.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ceg.gogol.net.cn

[R36] 并发执行多个任务
来源：http://fqu.hfpthk.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kml.iojbl.cn

[R37] 把输出赋给变量
来源：http://mjr.cdnleiting.top

files=$(ls -1)
来源：http://ufz.jlsjyb.cn

[R38] 管道串联
来源：http://rna.zhengqikj.top

cat a.txt | grep -i error | wc -l
来源：http://con.hywenlv.cn

[R39] 重定向标准输出与错误
来源：http://xaz.tarul.cn

cmd > out.log 2>&1
来源：http://inh.ivvv.top

[R40] 追加写日志
来源：http://zls.9152youxi.cn

echo "log" >> out.log
来源：http://jyt.shangyingyoupin.top

[R41] 丢弃输出
来源：http://htz.birdmap.top

cmd >/dev/null 2>&1
来源：http://gla.havefunace.top

[R42] 输入重定向
来源：http://dpc.bbcook.cn

wc -l < a.txt
来源：http://cgf.tianlin.xyz

[R43] 按名字查找文件
来源：http://yuu.shuidangran.top

find . -name "*.log" -type f
来源：http://vds.birdmap.top

[R44] 按修改时间查找
来源：http://wwp.zdbjq.cn

find . -mtime -7 -type f
来源：http://qyj.yueranfly.top

[R45] 批量删除
来源：http://xdf.cheryme.top

find . -name "*.tmp" -delete
来源：http://gey.jinqigufen.top

[R46] 递归替换文件内容
来源：http://jdl.uphjek.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://skf.zhixingplan.top

[R47] sed 单行替换
来源：http://ynk.xylfe.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wqh.tian-w.cn

[R48] awk 取指定列
来源：http://opu.yonumen.top

awk '{print $1, $3}' a.txt
来源：http://szj.meibo888.top

[R49] awk 带条件
来源：http://xlv.bjfxy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wnz.jinqigufen.top

[R50] awk 求和
来源：http://asx.aibaodan.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cux.zhoulong.xyz

[R51] 排序去重取前几
来源：http://kqw.tanke756.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ath.pycfn.com

[R52] 统计行数
来源：http://kun.kuanghao11.cn

wc -l a.txt
来源：http://lsr.xinyue.icu

[R53] 查看文件头与实时尾
来源：http://lda.hnqzz.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ktw.xinyue.icu

[R54] 比较两个文件
来源：http://ska.xuetiantiany.cn

diff a.txt b.txt
来源：http://reu.52xcode.cn

[R55] 压缩与解压
来源：http://grz.jinqigufen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uqe.xuetiantiany.cn

[R56] 远程拷贝
来源：http://ebc.yangfankeji.com

scp file user@host:/path/
来源：http://kgp.xuanzx.com

[R57] 远程执行命令
来源：http://qls.gotoacloud.top

ssh user@host 'uptime'
来源：http://cjz.tianlin.xyz

[R58] 下载文件
来源：http://pnx.bbcook.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zvh.yj20258.top

[R59] 发 POST JSON
来源：http://wvl.snrcjt.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qan.tarul.cn

[R60] 只看 HTTP 状态码
来源：http://gel.chenzaomai.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bla.xylfe.cn

[R61] 磁盘占用
来源：http://uuf.nwbrower.top

df -h;  du -sh *
来源：http://kik.sxryk.cn

[R62] 找最占空间的文件
来源：http://qto.yj20258888.top

du -ah . | sort -rh | head -10
来源：http://wnc.tian-w.cn

[R63] 内存与进程
来源：http://hjk.epnwcf.com

free -h;  ps aux | grep nginx
来源：http://meq.daria6918.cn

[R64] 结束进程
来源：http://ghc.haohaochexian.top

kill -9 $(pgrep -f app.py)
来源：http://lnz.yuxming.cn

[R65] 查看端口占用
来源：http://fll.sufxvd.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bah.9152youxi.cn

[R66] 定时任务
来源：http://tdd.hcnkem.com

crontab -e;  crontab -l
来源：http://web.guannengcc.top

[R67] 生成随机十六进制串
来源：http://dqp.xinyue.icu

openssl rand -hex 16
来源：http://lyo.birdmap.top

[R68] 计算文件校验值
来源：http://cpp.ydjk.org.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ngq.jianghu66.top

[R69] 生成随机密码
来源：http://xem.sxryk.cn

head -c 16 /dev/urandom | base64
来源：http://hos.iojbl.cn

[R70] 时间戳与互转
来源：http://dbr.cqqwz.cn

date +%s;  date -d @1700000000
来源：http://eom.xuetiantiany.cn

[R71] 日期格式化
来源：http://smw.yfazqb.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://xqd.shangyingyoupin.top

[R72] 等待端口就绪
来源：http://fpn.svipenyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pfh.yanxiufei.cn

[R73] 分割大日志
来源：http://kul.fzhhl.top

split -l 1000 big.log part_
来源：http://pko.bbcook.cn

[R74] 批量重命名
来源：http://slb.fzhhl.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qdw.pycfn.com

[R75] 导出环境变量
来源：http://iox.wangdashe.top

export PATH="$HOME/bin:$PATH"
来源：http://bpc.xylfe.cn

[R76] 使用临时文件
来源：http://jhf.zdbjq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pkt.ydzc1.top

[R77] 读取用户输入
来源：http://fqj.zhaomingkeji.xyz

read -rp "请输入: " ans
来源：http://duf.hnqzz.top

[R78] 交互式菜单
来源：http://hxx.mhx1999.top

select opt in a b c; do echo "$opt"; break; done
来源：http://mpn.pycfn.com

[R79] 解析命令行选项
来源：http://vth.zdqjudy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://abw.sysykeji.top

[R80] 查看脚本执行耗时
来源：http://lqd.hysaishi.cn

time ./run.sh
来源：http://pym.c1oappe.top

================================================================================
来源：http://ppm.sysykeji.top

S. C / C++ 专题
来源：http://qcz.sjlbkw.cn

================================================================================
来源：http://qwt.xziqi.cn

[S01] C：Hello World
来源：http://nsz.shangyingyoupin.top

#include <stdio.h>
来源：http://dgl.yj202588.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://pby.snrcjt.cn

[S02] C：变量与格式化输出
来源：http://nkv.hnqzz.top

int a = 10; printf("%d\n", a);
来源：http://hsp.tanke756.top

[S03] C：读入整数
来源：http://jeh.sysykeji.top

int x; scanf("%d", &x);
来源：http://jid.cashguo.top

[S04] C：字符串复制
来源：http://iqh.nanxinkj.top

char dst[32]; strcpy(dst, "hi");
来源：http://cvv.gotoacloud.top

[S05] C：字符串长度
来源：http://fks.chenjidiqi.icu

strlen(s)
来源：http://qtr.tian-w.cn

[S06] C：字符串比较
来源：http://uoy.yangfankeji.com

strcmp(a, b) == 0
来源：http://qtk.cdnleiting.top

[S07] C：数组遍历求和
来源：http://ywj.feifeiyinyue.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vaq.mhx1999.top

[S08] C：动态内存分配与释放
来源：http://wus.9152youxi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lbu.pycfn.com

[S09] C：结构体定义与初始化
来源：http://piq.wangdashe.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cyg.feifeiyinyue.top

[S10] C：指针与解引用
来源：http://hrj.ydjk.org.cn

int *p = &a;  *p = 5;
来源：http://gvq.ppjwa.cn

[S11] C：逐行读文件
来源：http://avg.iojbl.cn

FILE *f = fopen("a.txt", "r");
来源：http://obu.zdbjq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://oqq.fktsv.cn

fclose(f);
来源：http://stk.sjlbkw.cn

[S12] C：写文件
来源：http://isj.shuidangran.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://liw.ydjk.org.cn

[S13] C：宏定义
来源：http://vcr.daria6918.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bsv.chenzaomai.com

[S14] C：枚举
来源：http://yzh.haohaochexian.top

enum Color { RED, GREEN, BLUE };
来源：http://hxt.jqgufenzy.top

[S15] C：类型转换
来源：http://mht.hnxiangtu.top

(double) a / b
来源：http://zwm.uphjek.com

[S16] C：位操作置位
来源：http://epn.guannengcc.top

x |= (1 << 3);
来源：http://mfy.mhx1999.top

[S17] C：安全拼接字符串
来源：http://dvj.yonumen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nkj.zdqjudy.top

[S18] C：命令行参数
来源：http://iui.shzxlz.cn

int main(int argc, char **argv)
来源：http://olt.9152youxi.cn

[S19] C：快速排序
来源：http://jcc.hammf.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gqb.fengsongda.top

[S20] C：二分查找
来源：http://jjx.bjfxy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://emy.zhijiandao.cn

[S21] C：字符类别判断
来源：http://jge.daxiang520.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xml.hammf.cn

[S22] C：字符串转数字
来源：http://bwi.yvedp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nqe.iojbl.cn

[S23] C：随机数
来源：http://eko.redwolf501.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bwe.yangfankeji.com

[S24] C：获取本地时间
来源：http://ivw.wangshuangyany.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ecn.nwbrower.top

[S25] C：内存拷贝
来源：http://xgx.fktsv.cn

memcpy(dst, src, n);
来源：http://dab.svipenyu.cn

[S26] C：内存清零
来源：http://yrq.wangshuangyany.cn

memset(a, 0, sizeof a);
来源：http://mby.wangdashe.top

[S27] C：定义常量
来源：http://npl.cdnleiting.top

const double PI = 3.14159;
来源：http://rvu.pycfn.com

[S28] C：静态变量
来源：http://mkv.tianlin.xyz

static int counter = 0;
来源：http://hft.jinqigfzy.top

[S29] C：变参函数
来源：http://fbz.wangdashe.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dbz.zhongyouzk.top

[S30] C：头文件保护
来源：http://oxv.redwolf501.top

#ifndef X_H
来源：http://pyx.shanyushiyangkeji.top

#define X_H
来源：http://qfm.shanyushiyangtech.top

#endif
来源：http://yvz.yangfankeji.com

[S31] C++：Hello World
来源：http://zod.cashguo.top

#include <iostream>
来源：http://gsc.chenjidiqi.icu

int main() { std::cout << "Hello\n"; }
来源：http://vks.wangshuangyany.cn

[S32] C++：字符串
来源：http://aww.jinyuanbaomall.cn

std::string s = "hi";  s += "!";
来源：http://hxo.shzxlz.cn

[S33] C++：vector 增删
来源：http://ipx.xingfuxueyuan.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fwi.yuxming.cn

[S34] C++：遍历 vector
来源：http://kii.feifeiyinyue.top

for (auto &x : v) { std::cout << x; }
来源：http://fqx.iojbl.cn

[S35] C++：map
来源：http://rjs.epnwcf.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ggi.smart0.xyz

[S36] C++：unordered_map
来源：http://mmz.hongshengwenyu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tll.ywan-chungtsiang.top

[S37] C++：set
来源：http://iik.gzhubu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ocj.fengsongda.top

[S38] C++：排序
来源：http://pld.jinqigfzy.top

std::sort(v.begin(), v.end());
来源：http://jcx.havefunace.top

[S39] C++：自定义比较器排序
来源：http://vte.nanxinkj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wgm.yvedp.cn

[S40] C++：查找元素
来源：http://kaq.andypj.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vrg.cdnleiting.top

[S41] C++：类与构造函数
来源：http://ksb.ydjk.org.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ooi.chenjidiqi.icu

[S42] C++：继承与虚函数
来源：http://oyx.sufxvd.cn

class B : public Base { public: void f() override {} };
来源：http://qpb.feifeiyinyue.top

[S43] C++：智能指针
来源：http://wpt.pycfn.com

auto p = std::make_unique<int>(5);
来源：http://vho.bbcook.cn

[S44] C++：引用传参
来源：http://yxw.aibaodan.cn

void inc(int &x) { ++x; }
来源：http://hsv.vqdsnc.cn

[S45] C++：lambda
来源：http://cza.jqgfzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://xgm.yfazqb.com

[S46] C++：函数模板
来源：http://ygu.gogol.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://knv.shanyushiyangkeji.top

[S47] C++：结构化绑定遍历
来源：http://pqf.jyoumei.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hgl.yvedp.cn

[S48] C++：逐行读文件
来源：http://sbt.zhiwuduotai.top

std::ifstream in("a.txt");  std::string line;
来源：http://kzh.bbcook.cn

while (std::getline(in, line)) { }
来源：http://rql.jqgfzy.top

[S49] C++：写文件
来源：http://rhe.316326.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://msq.yvedp.cn

[S50] C++：格式化数字
来源：http://qpq.jianghu66.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ovy.vqdsnc.cn

[S51] C++：显式类型转换
来源：http://sbz.sysykeji.top

static_cast<double>(a) / b
来源：http://eja.shangyingyoupin.top

[S52] C++：const 与 noexcept
来源：http://pnx.jlsjyb.cn

int size() const noexcept { return n_; }
来源：http://erd.hcnkem.com

[S53] C++：移动语义
来源：http://yqa.hcnkem.com

std::vector<int> w = std::move(v);
来源：http://kwu.zhixingplan.top

[S54] C++：异常处理
来源：http://iig.shzxlz.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gez.tarul.cn

[S55] C++：结构化绑定
来源：http://isr.jinghuilouyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zwo.yuanzhike.top

[S56] C++：optional
来源：http://rzr.redwolf501.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jfc.gogol.net.cn

[S57] C++：编译期常量
来源：http://umg.wangdashe.top

constexpr int N = 10;
来源：http://skf.zycfv.cn

[S58] C++：命名空间
来源：http://gvk.jlsjyb.cn

namespace ns { int f() { return 1; } }
来源：http://mpx.guannengcc.top

[S59] C++：静态断言
来源：http://zfx.ivvv.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ipn.aizwys.cn

[S60] C++：遍历并删除元素
来源：http://rdk.jinyuanbaomall.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ebr.hammf.cn

================================================================================
来源：http://aup.0kj1m.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jbm.tian-w.cn

================================================================================
来源：http://pho.zhijiandao.cn

[T01] Kotlin：Hello World
来源：http://uzl.yangfankeji.com

println("Hello")
来源：http://liq.jyoumei.cn

[T02] Kotlin：变量
来源：http://ndw.yongpay.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://iwh.feifeiyinyue.top

[T03] Kotlin：字符串模板
来源：http://hqx.xinyue.icu

"值: $b"
来源：http://ndp.yvedp.cn

[T04] Kotlin：空安全
来源：http://ndv.meibo888.top

val n: String? = null;  n?.length
来源：http://nap.ybcxt.top

[T05] Kotlin：when 表达式
来源：http://ubm.aizwys.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hgk.ctjpmb.com

[T06] Kotlin：集合映射
来源：http://htl.hammf.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://oaj.yj20258888.top

[T07] Kotlin：集合过滤
来源：http://ost.chenlongwang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nvs.vqdsnc.cn

[T08] Kotlin：数据类
来源：http://pso.shanyushiyangkeji.top

data class User(val name: String, val age: Int)
来源：http://rht.nanxuanxn.top

[T09] Kotlin：扩展函数
来源：http://csj.aizwys.cn

fun String.exclaim() = this + "!"
来源：http://sem.ybcxt.top

[T10] Kotlin：默认参数
来源：http://xwx.zhengqikj.top

fun greet(name: String = "World") = "Hi $name"
来源：http://tad.nanxinkj.top

[T11] Kotlin：协程
来源：http://jik.smart0.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://mmw.yj202588.top

[T12] Kotlin：解构声明
来源：http://kaq.yangfankeji.com

val (a, b) = Pair(1, 2)
来源：http://xot.zhiwuduotai.top


<!-- 参考信息 -->