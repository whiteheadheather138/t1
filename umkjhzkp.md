代发 wailian999

case "$1" in
来源：http://sgk.zycfv.cn

start) echo "启动" ;;
来源：http://gsm.sysykeji.top

stop)  echo "停止" ;;
来源：http://clr.bjfxy.top

*)     echo "未知命令" ;;
来源：http://onb.zhoulong.xyz

esac
来源：http://kxs.nwbrower.top

[R12] for 遍历文件
来源：http://pwd.uphjek.com

for f in *.txt; do echo "$f"; done
来源：http://hhc.meibo888.top

[R13] for 计数循环
来源：http://ebp.chenjidiqi.icu

for i in {1..10}; do echo "$i"; done
来源：http://mkf.xinyue.icu

[R14] C 风格 for
来源：http://zmw.jianghu66.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fml.daxiang520.top

[R15] while 逐行读文件
来源：http://nxn.jyoumei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vth.haohaochexian.top

[R16] until 等待条件
来源：http://udy.dashuyun.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fal.gzhubu.top

[R17] 数组定义与取值
来源：http://xyu.birdmap.top

arr=(a b c); echo "${arr[0]}"
来源：http://kdo.gaohongyu789.top

[R18] 遍历数组
来源：http://eho.tarul.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vpg.xuetiantiany.cn

[R19] 数组长度
来源：http://sro.tarul.cn

echo "${#arr[@]}"
来源：http://ywj.redwolf501.top

[R20] 关联数组（字典）
来源：http://lzz.yonumen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://paj.chenjidiqi.icu

[R21] 字符串长度
来源：http://acw.aizwys.cn

echo "${#s}"
来源：http://qpr.pycfn.com

[R22] 截取子串
来源：http://zya.yueranfly.top

echo "${s:0:5}"
来源：http://amy.xingfuxueyuan.xyz

[R23] 字符串替换
来源：http://aty.nanxinkj.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ndn.shzxlz.cn

[R24] 大小写转换
来源：http://gzv.bjfxy.top

echo "${s^^}"; echo "${s,,}"
来源：http://ccl.guannengcc.top

[R25] 去后缀 / 去前缀
来源：http://vac.zhixingplan.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://orv.yuanzhike.top

[R26] 命令替换
来源：http://fww.jianghu66.top

now=$(date +%F); echo "$now"
来源：http://phe.redwolf501.top

[R27] 算术展开
来源：http://yna.pycfn.com

echo $((1 + 2 * 3))
来源：http://lly.sufxvd.cn

[R28] 浮点运算
来源：http://cne.jinghuilouyu.cn

echo "scale=2; 10/3" | bc
来源：http://phe.zhaomingkeji.xyz

[R29] 定义函数
来源：http://awg.sufxvd.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sde.hesvh.cn

[R30] 函数返回状态码
来源：http://jaz.daxiang520.top

f() { return 0; }; f || echo "失败了"
来源：http://dql.gotoacloud.top

[R31] 局部变量
来源：http://lxs.tarul.cn

f() { local x=1; echo "$x"; }
来源：http://gia.0kj1m.cn

[R32] 参数个数校验
来源：http://ovq.yuxming.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://enw.yfazqb.com

[R33] 捕获错误并提示行号
来源：http://ebb.yj202588.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://elo.zhongyouzk.top

[R34] 退出时清理
来源：http://gpu.fanxiaobao.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://tqf.epnwcf.com

[R35] 后台执行并等待
来源：http://qqz.jiagoushi.top

sleep 5 & pid=$!; wait "$pid"
来源：http://oye.fzhhl.top

[R36] 并发执行多个任务
来源：http://ydy.hysaishi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yac.shanyushiyangtech.top

[R37] 把输出赋给变量
来源：http://txc.pycfn.com

files=$(ls -1)
来源：http://wji.gotoacloud.top

[R38] 管道串联
来源：http://byc.shuidangran.top

cat a.txt | grep -i error | wc -l
来源：http://mvf.hammf.cn

[R39] 重定向标准输出与错误
来源：http://tdf.fzhhl.top

cmd > out.log 2>&1
来源：http://koz.xinyue.icu

[R40] 追加写日志
来源：http://yej.uphjek.com

echo "log" >> out.log
来源：http://hew.snrcjt.cn

[R41] 丢弃输出
来源：http://raj.chenzaomai.com

cmd >/dev/null 2>&1
来源：http://kjk.yongpay.top

[R42] 输入重定向
来源：http://tck.havefunace.top

wc -l < a.txt
来源：http://ggf.aibaodan.cn

[R43] 按名字查找文件
来源：http://axk.ydzc1.top

find . -name "*.log" -type f
来源：http://zhz.yvedp.cn

[R44] 按修改时间查找
来源：http://bjr.gzhubu.top

find . -mtime -7 -type f
来源：http://dfy.uphjek.com

[R45] 批量删除
来源：http://xzu.fehbvm.com

find . -name "*.tmp" -delete
来源：http://zpf.gaohongyu789.top

[R46] 递归替换文件内容
来源：http://fne.yonumen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iqi.shanyushiyangkeji.top

[R47] sed 单行替换
来源：http://mmp.xingfuxueyuan.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://ybt.zdbjq.cn

[R48] awk 取指定列
来源：http://qqh.yangfankeji.com

awk '{print $1, $3}' a.txt
来源：http://lnk.iojbl.cn

[R49] awk 带条件
来源：http://ckd.chenjidiqi.icu

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wcp.zhiwuduotai.top

[R50] awk 求和
来源：http://cwz.zhiwuduotai.top

awk '{s += $2} END {print s}' a.txt
来源：http://frc.sxryk.cn

[R51] 排序去重取前几
来源：http://yln.dashuyun.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dxi.yj20258888.top

[R52] 统计行数
来源：http://giv.tianlin.xyz

wc -l a.txt
来源：http://uhy.vehdjk.com

[R53] 查看文件头与实时尾
来源：http://sxx.dianchejie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pfi.hnxiangtu.top

[R54] 比较两个文件
来源：http://ipb.zycfv.cn

diff a.txt b.txt
来源：http://lrz.hnqzz.top

[R55] 压缩与解压
来源：http://ygq.quarkkingdee.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gyk.zhixingplan.top

[R56] 远程拷贝
来源：http://vjo.zhaomingkeji.xyz

scp file user@host:/path/
来源：http://lfu.zycfv.cn

[R57] 远程执行命令
来源：http://osw.yanxiufei.cn

ssh user@host 'uptime'
来源：http://aiz.c1oappe.top

[R58] 下载文件
来源：http://tff.tianlin.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dnu.shanyushiyangkeji.top

[R59] 发 POST JSON
来源：http://zev.gzhubu.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ojs.nanxinkj.top

[R60] 只看 HTTP 状态码
来源：http://xke.ehwqpu.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jep.cheryme.top

[R61] 磁盘占用
来源：http://xon.xuetiantiany.cn

df -h;  du -sh *
来源：http://cbe.yuxming.cn

[R62] 找最占空间的文件
来源：http://fri.zhijiandao.cn

du -ah . | sort -rh | head -10
来源：http://hvr.mhx1999.top

[R63] 内存与进程
来源：http://gaj.yj202588.top

free -h;  ps aux | grep nginx
来源：http://dsi.feifeiyinyue.top

[R64] 结束进程
来源：http://has.hesvh.cn

kill -9 $(pgrep -f app.py)
来源：http://klw.yuxming.cn

[R65] 查看端口占用
来源：http://vgo.iojbl.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lhb.epnwcf.com

[R66] 定时任务
来源：http://mhj.cashguo.top

crontab -e;  crontab -l
来源：http://aat.xuanzx.com

[R67] 生成随机十六进制串
来源：http://sdw.nanxuanxn.top

openssl rand -hex 16
来源：http://lfj.tanke756.top

[R68] 计算文件校验值
来源：http://ewr.yfazqb.com

sha256sum a.txt;  md5sum a.txt
来源：http://oyw.jianghu66.top

[R69] 生成随机密码
来源：http://fnu.guowangkeji.top

head -c 16 /dev/urandom | base64
来源：http://ojv.tianlin.xyz

[R70] 时间戳与互转
来源：http://rer.zdqjudy.top

date +%s;  date -d @1700000000
来源：http://ebr.wangdashe.top

[R71] 日期格式化
来源：http://yvu.kuanghao11.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lqx.zhijiandao.cn

[R72] 等待端口就绪
来源：http://qse.birdmap.top

until nc -z localhost 3306; do sleep 1; done
来源：http://aor.xylfe.cn

[R73] 分割大日志
来源：http://jgk.ivvv.top

split -l 1000 big.log part_
来源：http://fce.redwolf501.top

[R74] 批量重命名
来源：http://puh.shangyingyoupin.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kdt.feifeiyinyue.top

[R75] 导出环境变量
来源：http://yyl.zhaomingkeji.xyz

export PATH="$HOME/bin:$PATH"
来源：http://tdz.vehdjk.com

[R76] 使用临时文件
来源：http://gkf.daria6918.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zzq.cheryme.top

[R77] 读取用户输入
来源：http://ngm.yj20258.top

read -rp "请输入: " ans
来源：http://zgn.nwbrower.top

[R78] 交互式菜单
来源：http://rfx.yfazqb.com

select opt in a b c; do echo "$opt"; break; done
来源：http://vdl.shzxlz.cn

[R79] 解析命令行选项
来源：http://eaz.ywan-chungtsiang.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ppg.gotoacloud.top

[R80] 查看脚本执行耗时
来源：http://jhz.andypj.xyz

time ./run.sh
来源：http://rud.yvedp.cn

================================================================================
来源：http://hgn.cdnleiting.top

S. C / C++ 专题
来源：http://dcp.jianghu66.top

================================================================================
来源：http://snv.dianchejie.cn

[S01] C：Hello World
来源：http://lkb.gotoacloud.top

#include <stdio.h>
来源：http://rco.52xcode.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rjt.aibaodan.cn

[S02] C：变量与格式化输出
来源：http://wsi.yongpay.top

int a = 10; printf("%d\n", a);
来源：http://dsx.uphjek.com

[S03] C：读入整数
来源：http://aig.haohaochexian.top

int x; scanf("%d", &x);
来源：http://qpz.wangshuangyany.cn

[S04] C：字符串复制
来源：http://rdq.epnwcf.com

char dst[32]; strcpy(dst, "hi");
来源：http://cvx.hcnkem.com

[S05] C：字符串长度
来源：http://akq.yj202588.top

strlen(s)
来源：http://ebv.tianlin.xyz

[S06] C：字符串比较
来源：http://uuz.redwolf501.top

strcmp(a, b) == 0
来源：http://hjx.yangfankeji.com

[S07] C：数组遍历求和
来源：http://ssm.shuidangran.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wvl.zhiwuduotai.top

[S08] C：动态内存分配与释放
来源：http://ilg.shanyushiyangkeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mym.jinqigufen.top

[S09] C：结构体定义与初始化
来源：http://xel.hcnkem.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yvo.yvedp.cn

[S10] C：指针与解引用
来源：http://olm.jinqigfzy.top

int *p = &a;  *p = 5;
来源：http://ygo.xylfe.cn

[S11] C：逐行读文件
来源：http://wuj.yuanzhike.top

FILE *f = fopen("a.txt", "r");
来源：http://ggh.yuanzhike.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://rsx.yfazqb.com

fclose(f);
来源：http://iql.xuanzx.com

[S12] C：写文件
来源：http://krx.yj20258.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zza.shangyingyoupin.top

[S13] C：宏定义
来源：http://dxa.hammf.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fta.zhengqikj.top

[S14] C：枚举
来源：http://pxo.hywenlv.cn

enum Color { RED, GREEN, BLUE };
来源：http://fca.zhengqikj.top

[S15] C：类型转换
来源：http://btn.jianghu66.top

(double) a / b
来源：http://qkb.birdmap.top

[S16] C：位操作置位
来源：http://yfo.jqgfzy.top

x |= (1 << 3);
来源：http://uto.shzxlz.cn

[S17] C：安全拼接字符串
来源：http://xnb.zhijiandao.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qso.zhiwuduotai.top

[S18] C：命令行参数
来源：http://htv.andypj.xyz

int main(int argc, char **argv)
来源：http://ceh.yuxming.cn

[S19] C：快速排序
来源：http://awb.hesvh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://shv.birdmap.top

[S20] C：二分查找
来源：http://zzg.fengsongda.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gql.tian-w.cn

[S21] C：字符类别判断
来源：http://jgx.yongpay.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pcj.0kj1m.cn

[S22] C：字符串转数字
来源：http://erv.sysykeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://dkp.sjlbkw.cn

[S23] C：随机数
来源：http://tft.cheryme.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bde.ybcxt.top

[S24] C：获取本地时间
来源：http://imy.jyoumei.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://azh.zdbjq.cn

[S25] C：内存拷贝
来源：http://tya.nanxinkj.top

memcpy(dst, src, n);
来源：http://wlq.gaohongyu789.top

[S26] C：内存清零
来源：http://wwc.ywan-chungtsiang.top

memset(a, 0, sizeof a);
来源：http://nyk.sufxvd.cn

[S27] C：定义常量
来源：http://qgy.aizwys.cn

const double PI = 3.14159;
来源：http://vyx.ctjpmb.com

[S28] C：静态变量
来源：http://cyg.0kj1m.cn

static int counter = 0;
来源：http://jwy.zhengqikj.top

[S29] C：变参函数
来源：http://fvd.daria6918.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cgx.cdnleiting.top

[S30] C：头文件保护
来源：http://crv.redwolf501.top

#ifndef X_H
来源：http://lcj.9152youxi.cn

#define X_H
来源：http://rhb.yueranfly.top

#endif
来源：http://wjh.yanxiufei.cn

[S31] C++：Hello World
来源：http://wxg.yangfankeji.com

#include <iostream>
来源：http://yog.0kj1m.cn

int main() { std::cout << "Hello\n"; }
来源：http://wva.chenjidiqi.icu

[S32] C++：字符串
来源：http://oxa.c1oappe.top

std::string s = "hi";  s += "!";
来源：http://ulr.hywenlv.cn

[S33] C++：vector 增删
来源：http://hhj.yangfankeji.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cya.svipenyu.cn

[S34] C++：遍历 vector
来源：http://kyk.iojbl.cn

for (auto &x : v) { std::cout << x; }
来源：http://ida.zhaomingkeji.xyz

[S35] C++：map
来源：http://vnj.hywenlv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xel.jinqigfzy.top

[S36] C++：unordered_map
来源：http://sqw.haohaochexian.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fip.andypj.xyz

[S37] C++：set
来源：http://eza.quarkkingdee.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lmd.redwolf501.top

[S38] C++：排序
来源：http://ybl.hammf.cn

std::sort(v.begin(), v.end());
来源：http://vya.gaohongyu789.top

[S39] C++：自定义比较器排序
来源：http://drl.sweek.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dhg.gzhubu.top

[S40] C++：查找元素
来源：http://cuf.yuxming.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://oip.nanxinkj.top

[S41] C++：类与构造函数
来源：http://zte.ybcxt.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fxb.hysaishi.cn

[S42] C++：继承与虚函数
来源：http://kro.yangfankeji.com

class B : public Base { public: void f() override {} };
来源：http://zog.ivvv.top

[S43] C++：智能指针
来源：http://fga.xingfuxueyuan.xyz

auto p = std::make_unique<int>(5);
来源：http://kam.yfazqb.com

[S44] C++：引用传参
来源：http://qrp.andypj.xyz

void inc(int &x) { ++x; }
来源：http://nxk.xuetiantiany.cn

[S45] C++：lambda
来源：http://iaw.feifeiyinyue.top

auto add = [](int a, int b) { return a + b; };
来源：http://snd.wangdashe.top

[S46] C++：函数模板
来源：http://ivy.cheryme.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oxg.c1oappe.top

[S47] C++：结构化绑定遍历
来源：http://fmp.wangdashe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mcg.svipenyu.cn

[S48] C++：逐行读文件
来源：http://nsw.nwbrower.top

std::ifstream in("a.txt");  std::string line;
来源：http://mbh.jinyuanbaomall.cn

while (std::getline(in, line)) { }
来源：http://sxq.sufxvd.cn

[S49] C++：写文件
来源：http://wez.fktsv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rtt.cdnleiting.top

[S50] C++：格式化数字
来源：http://gxx.hywenlv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://acv.fzhhl.top

[S51] C++：显式类型转换
来源：http://nmy.yj20258.top

static_cast<double>(a) / b
来源：http://unp.epnwcf.com

[S52] C++：const 与 noexcept
来源：http://mtb.svipenyu.cn

int size() const noexcept { return n_; }
来源：http://lid.bbcook.cn

[S53] C++：移动语义
来源：http://rpu.hammf.cn

std::vector<int> w = std::move(v);
来源：http://qlo.jqgfzy.top

[S54] C++：异常处理
来源：http://eki.hongshengwenyu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rzp.meibo888.top

[S55] C++：结构化绑定
来源：http://uac.xuanzx.com

auto [a, b] = std::make_pair(1, 2);
来源：http://gaq.aibaodan.cn

[S56] C++：optional
来源：http://zet.fzhhl.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bcv.ydjk.org.cn

[S57] C++：编译期常量
来源：http://cru.jqgfzy.top

constexpr int N = 10;
来源：http://gwf.ivvv.top

[S58] C++：命名空间
来源：http://xcm.kuanghao11.cn

namespace ns { int f() { return 1; } }
来源：http://bit.hysaishi.cn

[S59] C++：静态断言
来源：http://clu.ehwqpu.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fty.ywan-chungtsiang.top

[S60] C++：遍历并删除元素
来源：http://yld.ivvv.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sjo.hfpthk.cn

================================================================================
来源：http://dzz.jinqigufen.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ddw.cucudq.cn

================================================================================
来源：http://tmd.zhaomingkeji.xyz

[T01] Kotlin：Hello World
来源：http://pop.shanyushiyangkeji.top

println("Hello")
来源：http://wco.zdqjudy.top

[T02] Kotlin：变量
来源：http://kmv.hcnkem.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cpq.9152youxi.cn

[T03] Kotlin：字符串模板
来源：http://qqu.shanyushiyangkeji.top

"值: $b"
来源：http://glr.xinyue.icu

[T04] Kotlin：空安全
来源：http://wey.haohaochexian.top

val n: String? = null;  n?.length
来源：http://dme.snrcjt.cn

[T05] Kotlin：when 表达式
来源：http://rqp.hysaishi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ldw.zhaomingkeji.xyz

[T06] Kotlin：集合映射
来源：http://tgk.yanxiufei.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fsf.sweek.top

[T07] Kotlin：集合过滤
来源：http://bnu.shuidangran.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://uij.tarul.cn

[T08] Kotlin：数据类
来源：http://gwt.xinyue.icu

data class User(val name: String, val age: Int)
来源：http://zyh.wangshuangyany.cn

[T09] Kotlin：扩展函数
来源：http://mjt.0kj1m.cn

fun String.exclaim() = this + "!"
来源：http://ikv.ctjpmb.com

[T10] Kotlin：默认参数
来源：http://fbl.redwolf501.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ceq.ydjk.org.cn

[T11] Kotlin：协程
来源：http://sfz.tanke756.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://icd.zycfv.cn

[T12] Kotlin：解构声明
来源：http://pno.yvedp.cn

val (a, b) = Pair(1, 2)
来源：http://rlk.hongshengwenyu.top


<!-- 参考信息 -->