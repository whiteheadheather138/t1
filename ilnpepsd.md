代发 wailian999

case "$1" in
来源：http://nyn.316326.xyz

start) echo "启动" ;;
来源：http://pbl.hnxiangtu.top

stop)  echo "停止" ;;
来源：http://dde.uphjek.com

*)     echo "未知命令" ;;
来源：http://yun.zhengqikj.top

esac
来源：http://mml.ehwqpu.com

[R12] for 遍历文件
来源：http://rmj.zhoulong.xyz

for f in *.txt; do echo "$f"; done
来源：http://uxx.hongshengwenyu.top

[R13] for 计数循环
来源：http://qrq.aibaodan.cn

for i in {1..10}; do echo "$i"; done
来源：http://gil.hammf.cn

[R14] C 风格 for
来源：http://yig.hongshengwenyu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pic.hesvh.cn

[R15] while 逐行读文件
来源：http://aee.redwolf501.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://daz.guowangkeji.top

[R16] until 等待条件
来源：http://clm.wangshuangyany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sfj.uphjek.com

[R17] 数组定义与取值
来源：http://fum.xuetiantiany.cn

arr=(a b c); echo "${arr[0]}"
来源：http://eox.snrcjt.cn

[R18] 遍历数组
来源：http://iab.sjlbkw.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lwl.nanxinkj.top

[R19] 数组长度
来源：http://yip.gaohongyu789.top

echo "${#arr[@]}"
来源：http://abq.haohaochexian.top

[R20] 关联数组（字典）
来源：http://gwn.bbcook.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ptk.dashuyun.cn

[R21] 字符串长度
来源：http://pbi.xingfuxueyuan.xyz

echo "${#s}"
来源：http://jjg.yj20258888.top

[R22] 截取子串
来源：http://vtg.zdbjq.cn

echo "${s:0:5}"
来源：http://yas.mhx1999.top

[R23] 字符串替换
来源：http://hrg.cucudq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kqz.iojbl.cn

[R24] 大小写转换
来源：http://kci.hongshengwenyu.top

echo "${s^^}"; echo "${s,,}"
来源：http://jam.9152youxi.cn

[R25] 去后缀 / 去前缀
来源：http://aft.dashuyun.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sua.birdmap.top

[R26] 命令替换
来源：http://pfu.hysaishi.cn

now=$(date +%F); echo "$now"
来源：http://uvq.vehdjk.com

[R27] 算术展开
来源：http://bmm.zdbjq.cn

echo $((1 + 2 * 3))
来源：http://euv.gogol.net.cn

[R28] 浮点运算
来源：http://xoe.hesvh.cn

echo "scale=2; 10/3" | bc
来源：http://jsu.zhengqikj.top

[R29] 定义函数
来源：http://jto.zhixingplan.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hxv.hywenlv.cn

[R30] 函数返回状态码
来源：http://udv.fanxiaobao.xyz

f() { return 0; }; f || echo "失败了"
来源：http://lax.9152youxi.cn

[R31] 局部变量
来源：http://xtr.meibo888.top

f() { local x=1; echo "$x"; }
来源：http://bbs.hongshengwenyu.top

[R32] 参数个数校验
来源：http://yja.vqdsnc.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://swr.snrcjt.cn

[R33] 捕获错误并提示行号
来源：http://ymz.yfazqb.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nob.fktsv.cn

[R34] 退出时清理
来源：http://aik.chenlongwang.top

trap 'rm -f "$tmp"' EXIT
来源：http://imf.sufxvd.cn

[R35] 后台执行并等待
来源：http://vah.gzhubu.top

sleep 5 & pid=$!; wait "$pid"
来源：http://vdw.hesvh.cn

[R36] 并发执行多个任务
来源：http://pqe.ivvv.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yfq.dashuyun.cn

[R37] 把输出赋给变量
来源：http://nyn.316326.xyz

files=$(ls -1)
来源：http://shy.cucudq.cn

[R38] 管道串联
来源：http://udr.tian-w.cn

cat a.txt | grep -i error | wc -l
来源：http://asg.xziqi.cn

[R39] 重定向标准输出与错误
来源：http://qjl.epnwcf.com

cmd > out.log 2>&1
来源：http://iyk.jinqigufen.top

[R40] 追加写日志
来源：http://egi.quarkkingdee.top

echo "log" >> out.log
来源：http://ijl.quarkkingdee.top

[R41] 丢弃输出
来源：http://zsy.hongshengwenyu.top

cmd >/dev/null 2>&1
来源：http://ufe.nanxinkj.top

[R42] 输入重定向
来源：http://qlh.zhongyouzk.top

wc -l < a.txt
来源：http://xqg.nanxuanxn.top

[R43] 按名字查找文件
来源：http://wck.pengpengdd.cyou

find . -name "*.log" -type f
来源：http://tak.mhx1999.top

[R44] 按修改时间查找
来源：http://edi.ywan-chungtsiang.top

find . -mtime -7 -type f
来源：http://elz.jinqigufen.top

[R45] 批量删除
来源：http://ekt.jinqigufen.top

find . -name "*.tmp" -delete
来源：http://ktp.feifeiyinyue.top

[R46] 递归替换文件内容
来源：http://tmt.sysykeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ovd.hongshengwenyu.top

[R47] sed 单行替换
来源：http://vdg.jianghu66.top

sed -i 's/foo/bar/g' a.txt
来源：http://slr.nanxuanxn.top

[R48] awk 取指定列
来源：http://dlo.yangfankeji.com

awk '{print $1, $3}' a.txt
来源：http://xch.ywan-chungtsiang.top

[R49] awk 带条件
来源：http://pik.shanyushiyangtech.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ume.chenlongwang.top

[R50] awk 求和
来源：http://kas.cashguo.top

awk '{s += $2} END {print s}' a.txt
来源：http://eqt.shuidangran.top

[R51] 排序去重取前几
来源：http://zyn.shangyingyoupin.top

sort a.txt | uniq -c | sort -rn | head
来源：http://bss.ppjwa.cn

[R52] 统计行数
来源：http://oqv.yvedp.cn

wc -l a.txt
来源：http://slj.fehbvm.com

[R53] 查看文件头与实时尾
来源：http://cxu.zhixingplan.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uon.uphjek.com

[R54] 比较两个文件
来源：http://ecj.xuanzx.com

diff a.txt b.txt
来源：http://xwf.redwolf501.top

[R55] 压缩与解压
来源：http://bos.pengpengdd.cyou

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sdk.shangyingyoupin.top

[R56] 远程拷贝
来源：http://mze.birdmap.top

scp file user@host:/path/
来源：http://uwl.jqgufenzy.top

[R57] 远程执行命令
来源：http://zlt.redwolf501.top

ssh user@host 'uptime'
来源：http://ink.uphjek.com

[R58] 下载文件
来源：http://wtr.ybcxt.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tld.jyoumei.cn

[R59] 发 POST JSON
来源：http://wrg.guowangkeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ocl.yj20258.top

[R60] 只看 HTTP 状态码
来源：http://pvs.vehdjk.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hbj.bbcook.cn

[R61] 磁盘占用
来源：http://dhj.bjfxy.top

df -h;  du -sh *
来源：http://wjy.fzhhl.top

[R62] 找最占空间的文件
来源：http://mqv.zhongyouzk.top

du -ah . | sort -rh | head -10
来源：http://oso.xziqi.cn

[R63] 内存与进程
来源：http://ykc.0kj1m.cn

free -h;  ps aux | grep nginx
来源：http://wkb.jinyuanbaomall.cn

[R64] 结束进程
来源：http://rnm.yangfankeji.com

kill -9 $(pgrep -f app.py)
来源：http://dej.tian-w.cn

[R65] 查看端口占用
来源：http://vrc.xinyue.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dhk.jianghu66.top

[R66] 定时任务
来源：http://ryi.tianlin.xyz

crontab -e;  crontab -l
来源：http://gsg.shuidangran.top

[R67] 生成随机十六进制串
来源：http://pob.hnxiangtu.top

openssl rand -hex 16
来源：http://ify.jqgufenzy.top

[R68] 计算文件校验值
来源：http://fli.aibaodan.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rmx.nwbrower.top

[R69] 生成随机密码
来源：http://mgg.jqgufenzy.top

head -c 16 /dev/urandom | base64
来源：http://mby.jyoumei.cn

[R70] 时间戳与互转
来源：http://ipd.pengpengdd.cyou

date +%s;  date -d @1700000000
来源：http://nij.pengpengdd.cyou

[R71] 日期格式化
来源：http://hyl.ybcxt.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vap.tarul.cn

[R72] 等待端口就绪
来源：http://gic.nanxinkj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://foq.sxryk.cn

[R73] 分割大日志
来源：http://vwh.feifeiyinyue.top

split -l 1000 big.log part_
来源：http://hrh.hongshengwenyu.top

[R74] 批量重命名
来源：http://bvy.xingfuxueyuan.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oui.feifeiyinyue.top

[R75] 导出环境变量
来源：http://fjg.shzxlz.cn

export PATH="$HOME/bin:$PATH"
来源：http://wmw.feifeiyinyue.top

[R76] 使用临时文件
来源：http://yiq.zhijiandao.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fwt.redwolf501.top

[R77] 读取用户输入
来源：http://oem.316326.xyz

read -rp "请输入: " ans
来源：http://hmq.hnxiangtu.top

[R78] 交互式菜单
来源：http://zmv.ivvv.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ele.guannengcc.top

[R79] 解析命令行选项
来源：http://fza.cheryme.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pgn.shangyingyoupin.top

[R80] 查看脚本执行耗时
来源：http://yoj.haohaochexian.top

time ./run.sh
来源：http://vce.yonumen.top

================================================================================
来源：http://ldo.ydzc1.top

S. C / C++ 专题
来源：http://hlg.xingfuxueyuan.xyz

================================================================================
来源：http://aao.sufxvd.cn

[S01] C：Hello World
来源：http://wra.cashguo.top

#include <stdio.h>
来源：http://jho.xziqi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ylx.uphjek.com

[S02] C：变量与格式化输出
来源：http://sjf.zhongyouzk.top

int a = 10; printf("%d\n", a);
来源：http://jdj.bbcook.cn

[S03] C：读入整数
来源：http://pwf.redwolf501.top

int x; scanf("%d", &x);
来源：http://asf.pengpengdd.cyou

[S04] C：字符串复制
来源：http://ybd.aibaodan.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xxv.iojbl.cn

[S05] C：字符串长度
来源：http://bfe.daria6918.cn

strlen(s)
来源：http://xqj.jianghu66.top

[S06] C：字符串比较
来源：http://eia.sxryk.cn

strcmp(a, b) == 0
来源：http://hrw.mhx1999.top

[S07] C：数组遍历求和
来源：http://zkt.dianchejie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fbh.yanxiufei.cn

[S08] C：动态内存分配与释放
来源：http://uhe.cashguo.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ztg.sxryk.cn

[S09] C：结构体定义与初始化
来源：http://fpr.shanyushiyangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cnv.sjlbkw.cn

[S10] C：指针与解引用
来源：http://jtz.fktsv.cn

int *p = &a;  *p = 5;
来源：http://mgs.gaohongyu789.top

[S11] C：逐行读文件
来源：http://mgx.dianchejie.cn

FILE *f = fopen("a.txt", "r");
来源：http://omk.sufxvd.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sfz.zycfv.cn

fclose(f);
来源：http://owo.jyoumei.cn

[S12] C：写文件
来源：http://cwc.zycfv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ulc.jianghu66.top

[S13] C：宏定义
来源：http://ynw.yonumen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://keh.chenlongwang.top

[S14] C：枚举
来源：http://jfa.zycfv.cn

enum Color { RED, GREEN, BLUE };
来源：http://fiv.bjfxy.top

[S15] C：类型转换
来源：http://pyb.zhixingplan.top

(double) a / b
来源：http://prc.xinyue.icu

[S16] C：位操作置位
来源：http://phs.jqgufenzy.top

x |= (1 << 3);
来源：http://plf.zhixingplan.top

[S17] C：安全拼接字符串
来源：http://tbk.9152youxi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cyb.havefunace.top

[S18] C：命令行参数
来源：http://xdk.ppjwa.cn

int main(int argc, char **argv)
来源：http://aui.zhaomingkeji.xyz

[S19] C：快速排序
来源：http://dhz.xziqi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jag.vqdsnc.cn

[S20] C：二分查找
来源：http://zjd.xuanzx.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vxt.pengpengdd.cyou

[S21] C：字符类别判断
来源：http://oad.xuanzx.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bnb.zhengqikj.top

[S22] C：字符串转数字
来源：http://wvv.gotoacloud.top

atoi("42");  strtod("3.14", NULL);
来源：http://hrc.nwbrower.top

[S23] C：随机数
来源：http://rkm.redwolf501.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ahp.aibaodan.cn

[S24] C：获取本地时间
来源：http://sbe.wangdashe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dou.hfpthk.cn

[S25] C：内存拷贝
来源：http://wph.hnqzz.top

memcpy(dst, src, n);
来源：http://ucj.fanxiaobao.xyz

[S26] C：内存清零
来源：http://nox.snrcjt.cn

memset(a, 0, sizeof a);
来源：http://sfn.jinyuanbaomall.cn

[S27] C：定义常量
来源：http://qoh.shzxlz.cn

const double PI = 3.14159;
来源：http://xku.gzhubu.top

[S28] C：静态变量
来源：http://yxw.zhoulong.xyz

static int counter = 0;
来源：http://cab.hongshengwenyu.top

[S29] C：变参函数
来源：http://vxt.gotoacloud.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jcv.ppjwa.cn

[S30] C：头文件保护
来源：http://vzx.0kj1m.cn

#ifndef X_H
来源：http://cpo.hammf.cn

#define X_H
来源：http://ugv.aizwys.cn

#endif
来源：http://vfl.zhiwuduotai.top

[S31] C++：Hello World
来源：http://bcz.sysykeji.top

#include <iostream>
来源：http://vrj.sjlbkw.cn

int main() { std::cout << "Hello\n"; }
来源：http://mcs.fzhhl.top

[S32] C++：字符串
来源：http://mzz.cheryme.top

std::string s = "hi";  s += "!";
来源：http://cam.daxiang520.top

[S33] C++：vector 增删
来源：http://hbi.ehwqpu.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rco.gogol.net.cn

[S34] C++：遍历 vector
来源：http://udd.yueranfly.top

for (auto &x : v) { std::cout << x; }
来源：http://pok.zhengqikj.top

[S35] C++：map
来源：http://zpq.jinghuilouyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qok.shanyushiyangtech.top

[S36] C++：unordered_map
来源：http://lku.jlsjyb.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wjp.jiagoushi.top

[S37] C++：set
来源：http://qmg.xinyue.icu

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tie.kuanghao11.cn

[S38] C++：排序
来源：http://xrn.redwolf501.top

std::sort(v.begin(), v.end());
来源：http://zpw.tian-w.cn

[S39] C++：自定义比较器排序
来源：http://uhr.meibo888.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sor.jinghuilouyu.cn

[S40] C++：查找元素
来源：http://kcg.zhiwuduotai.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zcj.xuetiantiany.cn

[S41] C++：类与构造函数
来源：http://sjx.gaohongyu789.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hej.9152youxi.cn

[S42] C++：继承与虚函数
来源：http://ooi.meibo888.top

class B : public Base { public: void f() override {} };
来源：http://dic.yueranfly.top

[S43] C++：智能指针
来源：http://xtf.shangyingyoupin.top

auto p = std::make_unique<int>(5);
来源：http://uhg.jqgfzy.top

[S44] C++：引用传参
来源：http://geb.zdqjudy.top

void inc(int &x) { ++x; }
来源：http://uca.zhiwuduotai.top

[S45] C++：lambda
来源：http://xjk.hnxiangtu.top

auto add = [](int a, int b) { return a + b; };
来源：http://vll.yvedp.cn

[S46] C++：函数模板
来源：http://cdo.zdbjq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rta.yuxming.cn

[S47] C++：结构化绑定遍历
来源：http://asw.xylfe.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hdm.0kj1m.cn

[S48] C++：逐行读文件
来源：http://ysi.gzhubu.top

std::ifstream in("a.txt");  std::string line;
来源：http://sat.zhixingplan.top

while (std::getline(in, line)) { }
来源：http://hvq.xinyue.icu

[S49] C++：写文件
来源：http://qmm.yangfankeji.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gpa.zhaomingkeji.xyz

[S50] C++：格式化数字
来源：http://cbg.cqqwz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rgt.vehdjk.com

[S51] C++：显式类型转换
来源：http://wpr.snrcjt.cn

static_cast<double>(a) / b
来源：http://vfr.tarul.cn

[S52] C++：const 与 noexcept
来源：http://ddv.nanxinkj.top

int size() const noexcept { return n_; }
来源：http://hrr.jianghu66.top

[S53] C++：移动语义
来源：http://zgt.9152youxi.cn

std::vector<int> w = std::move(v);
来源：http://zoi.ywan-chungtsiang.top

[S54] C++：异常处理
来源：http://unh.nwbrower.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://khp.yfazqb.com

[S55] C++：结构化绑定
来源：http://blk.ywan-chungtsiang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://wcv.aibaodan.cn

[S56] C++：optional
来源：http://rzm.xingfuxueyuan.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tfc.cheryme.top

[S57] C++：编译期常量
来源：http://txt.wangshuangyany.cn

constexpr int N = 10;
来源：http://wwt.shangyingyoupin.top

[S58] C++：命名空间
来源：http://bwv.svipenyu.cn

namespace ns { int f() { return 1; } }
来源：http://ohv.tanke756.top

[S59] C++：静态断言
来源：http://ude.hywenlv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://poe.ehwqpu.com

[S60] C++：遍历并删除元素
来源：http://etp.bjfxy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rwy.andypj.xyz

================================================================================
来源：http://pwg.fehbvm.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://aco.xuetiantiany.cn

================================================================================
来源：http://mln.ehwqpu.com

[T01] Kotlin：Hello World
来源：http://ovu.zhengqikj.top

println("Hello")
来源：http://uvk.shzxlz.cn

[T02] Kotlin：变量
来源：http://phe.shzxlz.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://igs.dianchejie.cn

[T03] Kotlin：字符串模板
来源：http://goc.316326.xyz

"值: $b"
来源：http://wze.jyoumei.cn

[T04] Kotlin：空安全
来源：http://vpn.ivvv.top

val n: String? = null;  n?.length
来源：http://vfe.tanke756.top

[T05] Kotlin：when 表达式
来源：http://umo.yongpay.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kiq.mhx1999.top

[T06] Kotlin：集合映射
来源：http://kog.smart0.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://gfj.zycfv.cn

[T07] Kotlin：集合过滤
来源：http://lda.xziqi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xac.nanxuanxn.top

[T08] Kotlin：数据类
来源：http://cqb.aizwys.cn

data class User(val name: String, val age: Int)
来源：http://wre.zhiwuduotai.top

[T09] Kotlin：扩展函数
来源：http://umw.guowangkeji.top

fun String.exclaim() = this + "!"
来源：http://blu.havefunace.top

[T10] Kotlin：默认参数
来源：http://xdh.ctjpmb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://tpf.dashuyun.cn

[T11] Kotlin：协程
来源：http://dki.ctjpmb.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://hzs.xuetiantiany.cn

[T12] Kotlin：解构声明
来源：http://dja.316326.xyz

val (a, b) = Pair(1, 2)
来源：http://ofs.gaohongyu789.top


<!-- 参考信息 -->