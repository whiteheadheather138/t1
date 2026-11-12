代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dhr.nwbrower.top

[R16] until 等待条件
来源：http://kdk.havefunace.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uop.ydjk.org.cn

[R17] 数组定义与取值
来源：http://plg.dianchejie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jgk.jqgfzy.top

[R18] 遍历数组
来源：http://gvr.hnxiangtu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tmw.zhongyouzk.top

[R19] 数组长度
来源：http://igr.zhengqikj.top

echo "${#arr[@]}"
来源：http://aga.snrcjt.cn

[R20] 关联数组（字典）
来源：http://ghr.jinqigufen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rrc.zhijiandao.cn

[R21] 字符串长度
来源：http://mrh.cheryme.top

echo "${#s}"
来源：http://uka.ybcxt.top

[R22] 截取子串
来源：http://bvi.hysaishi.cn

echo "${s:0:5}"
来源：http://ajm.gaohongyu789.top

[R23] 字符串替换
来源：http://ygy.hywenlv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pbn.gotoacloud.top

[R24] 大小写转换
来源：http://ggf.wangshuangyany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://oqx.ywan-chungtsiang.top

[R25] 去后缀 / 去前缀
来源：http://ogi.hnqzz.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://rvd.jinqigfzy.top

[R26] 命令替换
来源：http://sex.jianghu66.top

now=$(date +%F); echo "$now"
来源：http://lrm.ywan-chungtsiang.top

[R27] 算术展开
来源：http://ays.zhaomingkeji.xyz

echo $((1 + 2 * 3))
来源：http://shl.yj20258.top

[R28] 浮点运算
来源：http://nwa.ivvv.top

echo "scale=2; 10/3" | bc
来源：http://tcs.wangdashe.top

[R29] 定义函数
来源：http://lww.uphjek.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xdl.yueranfly.top

[R30] 函数返回状态码
来源：http://pmn.quarkkingdee.top

f() { return 0; }; f || echo "失败了"
来源：http://aks.xingfuxueyuan.xyz

[R31] 局部变量
来源：http://drl.haohaochexian.top

f() { local x=1; echo "$x"; }
来源：http://nth.zhoulong.xyz

[R32] 参数个数校验
来源：http://dfk.hfpthk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wag.svipenyu.cn

[R33] 捕获错误并提示行号
来源：http://zll.jlsjyb.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bom.xinyue.icu

[R34] 退出时清理
来源：http://wxf.wangshuangyany.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qyk.uphjek.com

[R35] 后台执行并等待
来源：http://faa.hfpthk.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://sox.bbcook.cn

[R36] 并发执行多个任务
来源：http://ons.feifeiyinyue.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gdq.zhongyouzk.top

[R37] 把输出赋给变量
来源：http://cdj.dianchejie.cn

files=$(ls -1)
来源：http://eua.nanxinkj.top

[R38] 管道串联
来源：http://phi.zycfv.cn

cat a.txt | grep -i error | wc -l
来源：http://jff.zhongyouzk.top

[R39] 重定向标准输出与错误
来源：http://ocp.xylfe.cn

cmd > out.log 2>&1
来源：http://rhv.fehbvm.com

[R40] 追加写日志
来源：http://dta.yueranfly.top

echo "log" >> out.log
来源：http://kmh.zhengqikj.top

[R41] 丢弃输出
来源：http://pos.fanxiaobao.xyz

cmd >/dev/null 2>&1
来源：http://hpw.hywenlv.cn

[R42] 输入重定向
来源：http://msa.mhx1999.top

wc -l < a.txt
来源：http://ghl.cashguo.top

[R43] 按名字查找文件
来源：http://jbu.vehdjk.com

find . -name "*.log" -type f
来源：http://yyj.hfpthk.cn

[R44] 按修改时间查找
来源：http://kli.nwbrower.top

find . -mtime -7 -type f
来源：http://wln.fehbvm.com

[R45] 批量删除
来源：http://wub.ehwqpu.com

find . -name "*.tmp" -delete
来源：http://ncz.haohaochexian.top

[R46] 递归替换文件内容
来源：http://nie.9152youxi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qce.hfpthk.cn

[R47] sed 单行替换
来源：http://uis.ppjwa.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kcx.zhiwuduotai.top

[R48] awk 取指定列
来源：http://lfh.yvedp.cn

awk '{print $1, $3}' a.txt
来源：http://xqr.kuanghao11.cn

[R49] awk 带条件
来源：http://zdb.fzhhl.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iqp.zhongyouzk.top

[R50] awk 求和
来源：http://huz.c1oappe.top

awk '{s += $2} END {print s}' a.txt
来源：http://epk.shangyingyoupin.top

[R51] 排序去重取前几
来源：http://goo.hnxiangtu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://pmb.gogol.net.cn

[R52] 统计行数
来源：http://lds.mhx1999.top

wc -l a.txt
来源：http://dzp.hnxiangtu.top

[R53] 查看文件头与实时尾
来源：http://xvn.sufxvd.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lcs.c1oappe.top

[R54] 比较两个文件
来源：http://izq.shangyingyoupin.top

diff a.txt b.txt
来源：http://mmg.guowangkeji.top

[R55] 压缩与解压
来源：http://npo.smart0.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zex.gogol.net.cn

[R56] 远程拷贝
来源：http://aez.pycfn.com

scp file user@host:/path/
来源：http://asp.feifeiyinyue.top

[R57] 远程执行命令
来源：http://heb.ppjwa.cn

ssh user@host 'uptime'
来源：http://jkm.epnwcf.com

[R58] 下载文件
来源：http://jcs.cucudq.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://txs.pengpengdd.cyou

[R59] 发 POST JSON
来源：http://uji.nanxinkj.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nkl.redwolf501.top

[R60] 只看 HTTP 状态码
来源：http://ari.dianchejie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hqg.hysaishi.cn

[R61] 磁盘占用
来源：http://tqb.cdnleiting.top

df -h;  du -sh *
来源：http://vrz.fzhhl.top

[R62] 找最占空间的文件
来源：http://tum.yuxming.cn

du -ah . | sort -rh | head -10
来源：http://quh.shuidangran.top

[R63] 内存与进程
来源：http://yns.jqgfzy.top

free -h;  ps aux | grep nginx
来源：http://hvj.tanke756.top

[R64] 结束进程
来源：http://zox.jqgufenzy.top

kill -9 $(pgrep -f app.py)
来源：http://ckc.shangyingyoupin.top

[R65] 查看端口占用
来源：http://byo.wangshuangyany.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fwf.nwbrower.top

[R66] 定时任务
来源：http://eov.316326.xyz

crontab -e;  crontab -l
来源：http://uat.zhengqikj.top

[R67] 生成随机十六进制串
来源：http://uuv.yj20258888.top

openssl rand -hex 16
来源：http://gvp.hcnkem.com

[R68] 计算文件校验值
来源：http://qej.9152youxi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lue.chenlongwang.top

[R69] 生成随机密码
来源：http://riq.xziqi.cn

head -c 16 /dev/urandom | base64
来源：http://wbz.sjlbkw.cn

[R70] 时间戳与互转
来源：http://wev.shzxlz.cn

date +%s;  date -d @1700000000
来源：http://noz.hnqzz.top

[R71] 日期格式化
来源：http://xqc.shanyushiyangkeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://utg.tian-w.cn

[R72] 等待端口就绪
来源：http://wfg.sysykeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://eds.yj20258888.top

[R73] 分割大日志
来源：http://esf.zhijiandao.cn

split -l 1000 big.log part_
来源：http://rlf.jqgufenzy.top

[R74] 批量重命名
来源：http://qrg.aizwys.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kdq.mhx1999.top

[R75] 导出环境变量
来源：http://uhq.guowangkeji.top

export PATH="$HOME/bin:$PATH"
来源：http://nbs.fktsv.cn

[R76] 使用临时文件
来源：http://usc.yangfankeji.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tkf.ppjwa.cn

[R77] 读取用户输入
来源：http://nzv.cdnleiting.top

read -rp "请输入: " ans
来源：http://wjx.haohaochexian.top

[R78] 交互式菜单
来源：http://vfe.zhijiandao.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kkx.yanxiufei.cn

[R79] 解析命令行选项
来源：http://ble.shuidangran.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dwu.pengpengdd.cyou

[R80] 查看脚本执行耗时
来源：http://gny.xingfuxueyuan.xyz

time ./run.sh
来源：http://tqk.hysaishi.cn

================================================================================
来源：http://qvb.pycfn.com

S. C / C++ 专题
来源：http://phy.sufxvd.cn

================================================================================
来源：http://gip.xziqi.cn

[S01] C：Hello World
来源：http://hbh.jianghu66.top

#include <stdio.h>
来源：http://hbz.yuanzhike.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gmn.cdnleiting.top

[S02] C：变量与格式化输出
来源：http://dql.yangfankeji.com

int a = 10; printf("%d\n", a);
来源：http://xgl.pycfn.com

[S03] C：读入整数
来源：http://cvt.sjlbkw.cn

int x; scanf("%d", &x);
来源：http://hhj.yj20258888.top

[S04] C：字符串复制
来源：http://svf.bbcook.cn

char dst[32]; strcpy(dst, "hi");
来源：http://che.gotoacloud.top

[S05] C：字符串长度
来源：http://sbd.zycfv.cn

strlen(s)
来源：http://vvn.ehwqpu.com

[S06] C：字符串比较
来源：http://ino.snrcjt.cn

strcmp(a, b) == 0
来源：http://ymn.hnxiangtu.top

[S07] C：数组遍历求和
来源：http://dhr.iojbl.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mcm.aizwys.cn

[S08] C：动态内存分配与释放
来源：http://lkd.jiagoushi.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wca.wangdashe.top

[S09] C：结构体定义与初始化
来源：http://xxp.svipenyu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://enb.fzhhl.top

[S10] C：指针与解引用
来源：http://far.hesvh.cn

int *p = &a;  *p = 5;
来源：http://chs.ywan-chungtsiang.top

[S11] C：逐行读文件
来源：http://myc.cashguo.top

FILE *f = fopen("a.txt", "r");
来源：http://wmk.kuanghao11.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mio.haohaochexian.top

fclose(f);
来源：http://xjr.xinyue.icu

[S12] C：写文件
来源：http://zsq.xylfe.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lfs.zdqjudy.top

[S13] C：宏定义
来源：http://vzi.jyoumei.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cze.tian-w.cn

[S14] C：枚举
来源：http://hoq.andypj.xyz

enum Color { RED, GREEN, BLUE };
来源：http://ijw.cucudq.cn

[S15] C：类型转换
来源：http://ewk.nanxinkj.top

(double) a / b
来源：http://xyp.redwolf501.top

[S16] C：位操作置位
来源：http://xhj.gzhubu.top

x |= (1 << 3);
来源：http://viu.birdmap.top

[S17] C：安全拼接字符串
来源：http://jkn.ehwqpu.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ehv.hesvh.cn

[S18] C：命令行参数
来源：http://umw.aibaodan.cn

int main(int argc, char **argv)
来源：http://oza.hysaishi.cn

[S19] C：快速排序
来源：http://chh.yuxming.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vis.epnwcf.com

[S20] C：二分查找
来源：http://tzt.jiagoushi.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mtz.jinqigfzy.top

[S21] C：字符类别判断
来源：http://ura.daria6918.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xyt.tanke756.top

[S22] C：字符串转数字
来源：http://jmv.shuidangran.top

atoi("42");  strtod("3.14", NULL);
来源：http://xdp.c1oappe.top

[S23] C：随机数
来源：http://mja.bbcook.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://iho.kuanghao11.cn

[S24] C：获取本地时间
来源：http://jbc.shangyingyoupin.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wgj.0kj1m.cn

[S25] C：内存拷贝
来源：http://dtr.epnwcf.com

memcpy(dst, src, n);
来源：http://qzr.jlsjyb.cn

[S26] C：内存清零
来源：http://nvd.hesvh.cn

memset(a, 0, sizeof a);
来源：http://pfb.ybcxt.top

[S27] C：定义常量
来源：http://cev.yvedp.cn

const double PI = 3.14159;
来源：http://zmv.nwbrower.top

[S28] C：静态变量
来源：http://xvr.ydjk.org.cn

static int counter = 0;
来源：http://oyu.fzhhl.top

[S29] C：变参函数
来源：http://ymq.kuanghao11.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gfo.ydjk.org.cn

[S30] C：头文件保护
来源：http://lpp.hywenlv.cn

#ifndef X_H
来源：http://dfk.jinyuanbaomall.cn

#define X_H
来源：http://djf.bbcook.cn

#endif
来源：http://uqf.yfazqb.com

[S31] C++：Hello World
来源：http://lmg.sufxvd.cn

#include <iostream>
来源：http://fvf.pycfn.com

int main() { std::cout << "Hello\n"; }
来源：http://zkh.yonumen.top

[S32] C++：字符串
来源：http://uzj.dashuyun.cn

std::string s = "hi";  s += "!";
来源：http://uvd.zhiwuduotai.top

[S33] C++：vector 增删
来源：http://ymb.haohaochexian.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hli.gogol.net.cn

[S34] C++：遍历 vector
来源：http://kxv.yj20258.top

for (auto &x : v) { std::cout << x; }
来源：http://rpr.chenzaomai.com

[S35] C++：map
来源：http://jvx.chenzaomai.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vhz.andypj.xyz

[S36] C++：unordered_map
来源：http://kba.sysykeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jtt.mhx1999.top

[S37] C++：set
来源：http://eou.cheryme.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ouv.yfazqb.com

[S38] C++：排序
来源：http://wfu.daria6918.cn

std::sort(v.begin(), v.end());
来源：http://ypq.xziqi.cn

[S39] C++：自定义比较器排序
来源：http://zun.sxryk.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xrg.hongshengwenyu.top

[S40] C++：查找元素
来源：http://arx.bbcook.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hgd.fktsv.cn

[S41] C++：类与构造函数
来源：http://vmr.guannengcc.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wyo.zhoulong.xyz

[S42] C++：继承与虚函数
来源：http://wsy.cucudq.cn

class B : public Base { public: void f() override {} };
来源：http://vyb.xylfe.cn

[S43] C++：智能指针
来源：http://ovr.cucudq.cn

auto p = std::make_unique<int>(5);
来源：http://wpl.ehwqpu.com

[S44] C++：引用传参
来源：http://mpp.svipenyu.cn

void inc(int &x) { ++x; }
来源：http://ptd.yangfankeji.com

[S45] C++：lambda
来源：http://pkt.jiagoushi.top

auto add = [](int a, int b) { return a + b; };
来源：http://vlx.gzhubu.top

[S46] C++：函数模板
来源：http://zji.ybcxt.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ijm.xinyue.icu

[S47] C++：结构化绑定遍历
来源：http://yyk.vehdjk.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ecs.yanxiufei.cn

[S48] C++：逐行读文件
来源：http://rjy.sxryk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ood.jlsjyb.cn

while (std::getline(in, line)) { }
来源：http://cce.xinyue.icu

[S49] C++：写文件
来源：http://vfh.zycfv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lvd.aizwys.cn

[S50] C++：格式化数字
来源：http://cbl.chenzaomai.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yde.uphjek.com

[S51] C++：显式类型转换
来源：http://aro.zhiwuduotai.top

static_cast<double>(a) / b
来源：http://gyc.shanyushiyangkeji.top

[S52] C++：const 与 noexcept
来源：http://peq.sufxvd.cn

int size() const noexcept { return n_; }
来源：http://ayp.hongshengwenyu.top

[S53] C++：移动语义
来源：http://jkk.hnqzz.top

std::vector<int> w = std::move(v);
来源：http://yby.cashguo.top

[S54] C++：异常处理
来源：http://fae.hammf.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vvv.yueranfly.top

[S55] C++：结构化绑定
来源：http://acf.mhx1999.top

auto [a, b] = std::make_pair(1, 2);
来源：http://cfb.pengpengdd.cyou

[S56] C++：optional
来源：http://phq.cucudq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mrd.aizwys.cn

[S57] C++：编译期常量
来源：http://yog.zhengqikj.top

constexpr int N = 10;
来源：http://nov.jinghuilouyu.cn

[S58] C++：命名空间
来源：http://uuk.ybcxt.top

namespace ns { int f() { return 1; } }
来源：http://mki.shanyushiyangkeji.top

[S59] C++：静态断言
来源：http://kry.hfpthk.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ray.hammf.cn

[S60] C++：遍历并删除元素
来源：http://ynl.zycfv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dxp.zhijiandao.cn

================================================================================
来源：http://arm.sweek.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pjs.dianchejie.cn

================================================================================
来源：http://csc.kuanghao11.cn

[T01] Kotlin：Hello World
来源：http://ryy.c1oappe.top

println("Hello")
来源：http://eeu.sufxvd.cn

[T02] Kotlin：变量
来源：http://bsy.vehdjk.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zcg.pengpengdd.cyou

[T03] Kotlin：字符串模板
来源：http://guz.uphjek.com

"值: $b"
来源：http://cmq.dashuyun.cn

[T04] Kotlin：空安全
来源：http://kow.snrcjt.cn

val n: String? = null;  n?.length
来源：http://eio.pengpengdd.cyou

[T05] Kotlin：when 表达式
来源：http://rcz.ybcxt.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mho.ehwqpu.com

[T06] Kotlin：集合映射
来源：http://rlz.bbcook.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ojw.fzhhl.top

[T07] Kotlin：集合过滤
来源：http://soa.jiagoushi.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://emz.jinghuilouyu.cn

[T08] Kotlin：数据类
来源：http://zti.ppjwa.cn

data class User(val name: String, val age: Int)
来源：http://skl.aibaodan.cn

[T09] Kotlin：扩展函数
来源：http://ucq.jinqigufen.top

fun String.exclaim() = this + "!"
来源：http://rkz.shanyushiyangkeji.top

[T10] Kotlin：默认参数
来源：http://ofv.dashuyun.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cgk.quarkkingdee.top

[T11] Kotlin：协程
来源：http://oru.ehwqpu.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://pfd.ydjk.org.cn

[T12] Kotlin：解构声明
来源：http://hys.chenlongwang.top

val (a, b) = Pair(1, 2)
来源：http://tyq.svipenyu.cn

[T13] Kotlin：只读 Map
来源：http://fmy.gotoacloud.top

val m = mapOf("a" to 1)
来源：http://ubd.jyoumei.cn

[T14] Kotlin：循环
来源：http://qgh.kuanghao11.cn

for (i in 1..10) println(i)
来源：http://oqp.gaohongyu789.top

[T15] Kotlin：接口
来源：http://pka.gzhubu.top

interface Shape { fun area(): Double }
来源：http://mwa.tianlin.xyz

[T16] Swift：Hello World
来源：http://ahk.ivvv.top

print("Hello")
来源：http://zlq.sufxvd.cn

[T17] Swift：变量与常量
来源：http://bbm.sufxvd.cn

var a = 1;  let b = 2
来源：http://ric.hnxiangtu.top

[T18] Swift：字符串插值
来源：http://kpn.chenzaomai.com

"值: \(b)"
来源：http://apc.yuanzhike.top


<!-- 参考信息 -->