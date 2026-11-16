代发 wailian999

esac
来源：http://ori.hysaishi.cn

[R12] for 遍历文件
来源：http://orb.hnxiangtu.top

for f in *.txt; do echo "$f"; done
来源：http://rhm.jqgfzy.top

[R13] for 计数循环
来源：http://sum.gogol.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://wds.gogol.net.cn

[R14] C 风格 for
来源：http://xmm.jqgufenzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jwd.zdqjudy.top

[R15] while 逐行读文件
来源：http://mvz.chenjidiqi.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wgx.shangyingyoupin.top

[R16] until 等待条件
来源：http://lrk.xinyue.icu

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nso.shzxlz.cn

[R17] 数组定义与取值
来源：http://qnk.ybcxt.top

arr=(a b c); echo "${arr[0]}"
来源：http://lha.nwbrower.top

[R18] 遍历数组
来源：http://aqy.yueranfly.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://llu.sufxvd.cn

[R19] 数组长度
来源：http://eov.jinqigfzy.top

echo "${#arr[@]}"
来源：http://smf.tarul.cn

[R20] 关联数组（字典）
来源：http://zpa.zdqjudy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lej.fktsv.cn

[R21] 字符串长度
来源：http://dqu.zhixingplan.top

echo "${#s}"
来源：http://kwm.shuidangran.top

[R22] 截取子串
来源：http://dfz.52xcode.cn

echo "${s:0:5}"
来源：http://zeh.kuanghao11.cn

[R23] 字符串替换
来源：http://sgt.epnwcf.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://glv.jyoumei.cn

[R24] 大小写转换
来源：http://ltw.jinqigufen.top

echo "${s^^}"; echo "${s,,}"
来源：http://yza.gotoacloud.top

[R25] 去后缀 / 去前缀
来源：http://vxx.nanxinkj.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://prn.pengpengdd.cyou

[R26] 命令替换
来源：http://nxq.yj20258888.top

now=$(date +%F); echo "$now"
来源：http://ybb.yueranfly.top

[R27] 算术展开
来源：http://ltl.c1oappe.top

echo $((1 + 2 * 3))
来源：http://cwu.sxryk.cn

[R28] 浮点运算
来源：http://mrh.quarkkingdee.top

echo "scale=2; 10/3" | bc
来源：http://uya.shanyushiyangkeji.top

[R29] 定义函数
来源：http://qhr.jianghu66.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qko.tianlin.xyz

[R30] 函数返回状态码
来源：http://eod.cdnleiting.top

f() { return 0; }; f || echo "失败了"
来源：http://cgc.jqgufenzy.top

[R31] 局部变量
来源：http://kph.cucudq.cn

f() { local x=1; echo "$x"; }
来源：http://hav.hnxiangtu.top

[R32] 参数个数校验
来源：http://gyt.dianchejie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://itn.chenzaomai.com

[R33] 捕获错误并提示行号
来源：http://tsq.ydzc1.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lkx.vqdsnc.cn

[R34] 退出时清理
来源：http://ovx.shuidangran.top

trap 'rm -f "$tmp"' EXIT
来源：http://hsf.zdbjq.cn

[R35] 后台执行并等待
来源：http://aid.52xcode.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dtr.jiagoushi.top

[R36] 并发执行多个任务
来源：http://igs.nwbrower.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jzh.iojbl.cn

[R37] 把输出赋给变量
来源：http://nkr.zhengqikj.top

files=$(ls -1)
来源：http://bum.wangshuangyany.cn

[R38] 管道串联
来源：http://xiy.gzhubu.top

cat a.txt | grep -i error | wc -l
来源：http://inl.ybcxt.top

[R39] 重定向标准输出与错误
来源：http://imm.zhixingplan.top

cmd > out.log 2>&1
来源：http://oov.fehbvm.com

[R40] 追加写日志
来源：http://pcg.quarkkingdee.top

echo "log" >> out.log
来源：http://kib.yonumen.top

[R41] 丢弃输出
来源：http://ygs.andypj.xyz

cmd >/dev/null 2>&1
来源：http://fja.zhiwuduotai.top

[R42] 输入重定向
来源：http://hde.yj20258888.top

wc -l < a.txt
来源：http://usv.yj20258888.top

[R43] 按名字查找文件
来源：http://lrx.shangyingyoupin.top

find . -name "*.log" -type f
来源：http://cjg.hesvh.cn

[R44] 按修改时间查找
来源：http://plm.xinyue.icu

find . -mtime -7 -type f
来源：http://eta.c1oappe.top

[R45] 批量删除
来源：http://rnd.birdmap.top

find . -name "*.tmp" -delete
来源：http://hsg.zdqjudy.top

[R46] 递归替换文件内容
来源：http://evu.tian-w.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gwi.shangyingyoupin.top

[R47] sed 单行替换
来源：http://gaw.yonumen.top

sed -i 's/foo/bar/g' a.txt
来源：http://xqx.shzxlz.cn

[R48] awk 取指定列
来源：http://bfs.tanke756.top

awk '{print $1, $3}' a.txt
来源：http://lsm.zhixingplan.top

[R49] awk 带条件
来源：http://tvg.daxiang520.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://azj.ehwqpu.com

[R50] awk 求和
来源：http://gsf.andypj.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://otw.nwbrower.top

[R51] 排序去重取前几
来源：http://mqk.iojbl.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tmn.xylfe.cn

[R52] 统计行数
来源：http://clg.cashguo.top

wc -l a.txt
来源：http://abl.chenlongwang.top

[R53] 查看文件头与实时尾
来源：http://xtk.zhaomingkeji.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cbu.chenzaomai.com

[R54] 比较两个文件
来源：http://aoa.birdmap.top

diff a.txt b.txt
来源：http://pbb.shanyushiyangkeji.top

[R55] 压缩与解压
来源：http://szh.zhiwuduotai.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cex.zdbjq.cn

[R56] 远程拷贝
来源：http://gdf.ydzc1.top

scp file user@host:/path/
来源：http://gwn.chenlongwang.top

[R57] 远程执行命令
来源：http://sca.pengpengdd.cyou

ssh user@host 'uptime'
来源：http://fei.sxryk.cn

[R58] 下载文件
来源：http://zsd.svipenyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sbb.zhiwuduotai.top

[R59] 发 POST JSON
来源：http://xwn.ivvv.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ulv.kuanghao11.cn

[R60] 只看 HTTP 状态码
来源：http://edx.bbcook.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zal.hongshengwenyu.top

[R61] 磁盘占用
来源：http://ysk.jqgfzy.top

df -h;  du -sh *
来源：http://ydo.tianlin.xyz

[R62] 找最占空间的文件
来源：http://rpt.0kj1m.cn

du -ah . | sort -rh | head -10
来源：http://bug.ydjk.org.cn

[R63] 内存与进程
来源：http://ecn.yj20258.top

free -h;  ps aux | grep nginx
来源：http://ovb.yuanzhike.top

[R64] 结束进程
来源：http://gbp.dashuyun.cn

kill -9 $(pgrep -f app.py)
来源：http://mco.xuetiantiany.cn

[R65] 查看端口占用
来源：http://jxf.shangyingyoupin.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tfl.jinqigufen.top

[R66] 定时任务
来源：http://pqq.chenzaomai.com

crontab -e;  crontab -l
来源：http://oge.zhongyouzk.top

[R67] 生成随机十六进制串
来源：http://gej.yonumen.top

openssl rand -hex 16
来源：http://pae.jinqigfzy.top

[R68] 计算文件校验值
来源：http://nds.daria6918.cn

sha256sum a.txt;  md5sum a.txt
来源：http://src.bjfxy.top

[R69] 生成随机密码
来源：http://ljv.yuanzhike.top

head -c 16 /dev/urandom | base64
来源：http://lbk.gaohongyu789.top

[R70] 时间戳与互转
来源：http://mto.gogol.net.cn

date +%s;  date -d @1700000000
来源：http://atr.hysaishi.cn

[R71] 日期格式化
来源：http://iro.yueranfly.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://tqr.svipenyu.cn

[R72] 等待端口就绪
来源：http://upb.shzxlz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://def.jqgfzy.top

[R73] 分割大日志
来源：http://csr.fktsv.cn

split -l 1000 big.log part_
来源：http://nah.vqdsnc.cn

[R74] 批量重命名
来源：http://kro.zhoulong.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://idu.316326.xyz

[R75] 导出环境变量
来源：http://wzh.vqdsnc.cn

export PATH="$HOME/bin:$PATH"
来源：http://zpr.sysykeji.top

[R76] 使用临时文件
来源：http://gee.sysykeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gtc.birdmap.top

[R77] 读取用户输入
来源：http://cme.uphjek.com

read -rp "请输入: " ans
来源：http://mcb.quarkkingdee.top

[R78] 交互式菜单
来源：http://lcd.shangyingyoupin.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ypu.snrcjt.cn

[R79] 解析命令行选项
来源：http://rlt.shuidangran.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fmf.shuidangran.top

[R80] 查看脚本执行耗时
来源：http://msw.zhiwuduotai.top

time ./run.sh
来源：http://clg.vehdjk.com

================================================================================
来源：http://ueo.nanxuanxn.top

S. C / C++ 专题
来源：http://gya.ctjpmb.com

================================================================================
来源：http://nur.dianchejie.cn

[S01] C：Hello World
来源：http://rtc.wangshuangyany.cn

#include <stdio.h>
来源：http://psn.52xcode.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vek.gogol.net.cn

[S02] C：变量与格式化输出
来源：http://rbi.zhongyouzk.top

int a = 10; printf("%d\n", a);
来源：http://ggt.yonumen.top

[S03] C：读入整数
来源：http://kzh.cashguo.top

int x; scanf("%d", &x);
来源：http://sta.epnwcf.com

[S04] C：字符串复制
来源：http://uha.ydzc1.top

char dst[32]; strcpy(dst, "hi");
来源：http://jfc.fehbvm.com

[S05] C：字符串长度
来源：http://atv.sysykeji.top

strlen(s)
来源：http://vrm.dashuyun.cn

[S06] C：字符串比较
来源：http://zow.shanyushiyangkeji.top

strcmp(a, b) == 0
来源：http://lfq.xziqi.cn

[S07] C：数组遍历求和
来源：http://buq.yuxming.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hqt.hfpthk.cn

[S08] C：动态内存分配与释放
来源：http://jlj.redwolf501.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vuu.smart0.xyz

[S09] C：结构体定义与初始化
来源：http://myz.zhengqikj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yxv.sxryk.cn

[S10] C：指针与解引用
来源：http://azf.svipenyu.cn

int *p = &a;  *p = 5;
来源：http://oba.fehbvm.com

[S11] C：逐行读文件
来源：http://drx.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "r");
来源：http://wjs.kuanghao11.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gsf.cucudq.cn

fclose(f);
来源：http://hll.nanxuanxn.top

[S12] C：写文件
来源：http://fyu.jqgfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://inf.jinghuilouyu.cn

[S13] C：宏定义
来源：http://bjp.gzhubu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nbe.jinyuanbaomall.cn

[S14] C：枚举
来源：http://sxs.hcnkem.com

enum Color { RED, GREEN, BLUE };
来源：http://slq.zhaomingkeji.xyz

[S15] C：类型转换
来源：http://gdu.bjfxy.top

(double) a / b
来源：http://xlw.mhx1999.top

[S16] C：位操作置位
来源：http://rci.mhx1999.top

x |= (1 << 3);
来源：http://gjj.shzxlz.cn

[S17] C：安全拼接字符串
来源：http://jti.ydzc1.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cyv.yueranfly.top

[S18] C：命令行参数
来源：http://lhq.vehdjk.com

int main(int argc, char **argv)
来源：http://ter.zhaomingkeji.xyz

[S19] C：快速排序
来源：http://gcl.aizwys.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jhz.fktsv.cn

[S20] C：二分查找
来源：http://hth.gotoacloud.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wts.hcnkem.com

[S21] C：字符类别判断
来源：http://epw.hywenlv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://avs.mhx1999.top

[S22] C：字符串转数字
来源：http://kgo.316326.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://spj.xuetiantiany.cn

[S23] C：随机数
来源：http://bge.fktsv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yuh.yanxiufei.cn

[S24] C：获取本地时间
来源：http://mes.iojbl.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lwc.gzhubu.top

[S25] C：内存拷贝
来源：http://mlm.hnxiangtu.top

memcpy(dst, src, n);
来源：http://yge.feifeiyinyue.top

[S26] C：内存清零
来源：http://ckd.zhongyouzk.top

memset(a, 0, sizeof a);
来源：http://jjb.zhiwuduotai.top

[S27] C：定义常量
来源：http://fmo.cashguo.top

const double PI = 3.14159;
来源：http://hlp.zhengqikj.top

[S28] C：静态变量
来源：http://xab.aizwys.cn

static int counter = 0;
来源：http://emm.svipenyu.cn

[S29] C：变参函数
来源：http://bgw.daria6918.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ikh.sweek.top

[S30] C：头文件保护
来源：http://lir.wangdashe.top

#ifndef X_H
来源：http://rwc.gotoacloud.top

#define X_H
来源：http://xcf.pengpengdd.cyou

#endif
来源：http://oua.aibaodan.cn

[S31] C++：Hello World
来源：http://hjo.hammf.cn

#include <iostream>
来源：http://dcz.ybcxt.top

int main() { std::cout << "Hello\n"; }
来源：http://yux.cashguo.top

[S32] C++：字符串
来源：http://rlw.zhengqikj.top

std::string s = "hi";  s += "!";
来源：http://zqw.dashuyun.cn

[S33] C++：vector 增删
来源：http://vos.yongpay.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mxu.hesvh.cn

[S34] C++：遍历 vector
来源：http://ioc.yj20258888.top

for (auto &x : v) { std::cout << x; }
来源：http://zvh.chenjidiqi.icu

[S35] C++：map
来源：http://gqx.pengpengdd.cyou

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ijy.pycfn.com

[S36] C++：unordered_map
来源：http://xsi.ehwqpu.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rqf.xingfuxueyuan.xyz

[S37] C++：set
来源：http://lip.quarkkingdee.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gzm.sjlbkw.cn

[S38] C++：排序
来源：http://luw.52xcode.cn

std::sort(v.begin(), v.end());
来源：http://lnj.jinghuilouyu.cn

[S39] C++：自定义比较器排序
来源：http://dzt.zdqjudy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://azv.ppjwa.cn

[S40] C++：查找元素
来源：http://hrq.jinqigfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yip.epnwcf.com

[S41] C++：类与构造函数
来源：http://gek.redwolf501.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rxz.52xcode.cn

[S42] C++：继承与虚函数
来源：http://qio.daxiang520.top

class B : public Base { public: void f() override {} };
来源：http://eft.wangshuangyany.cn

[S43] C++：智能指针
来源：http://bdl.xylfe.cn

auto p = std::make_unique<int>(5);
来源：http://lvj.guowangkeji.top

[S44] C++：引用传参
来源：http://fnj.mhx1999.top

void inc(int &x) { ++x; }
来源：http://llt.aizwys.cn

[S45] C++：lambda
来源：http://dgt.jyoumei.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yyk.shzxlz.cn

[S46] C++：函数模板
来源：http://cmg.zhixingplan.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nee.c1oappe.top

[S47] C++：结构化绑定遍历
来源：http://niy.haohaochexian.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://eqw.feifeiyinyue.top

[S48] C++：逐行读文件
来源：http://hxq.zhongyouzk.top

std::ifstream in("a.txt");  std::string line;
来源：http://tmw.jqgufenzy.top

while (std::getline(in, line)) { }
来源：http://ksk.nanxinkj.top

[S49] C++：写文件
来源：http://moo.aizwys.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bvy.nanxuanxn.top

[S50] C++：格式化数字
来源：http://kzt.aizwys.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fmw.yj20258888.top

[S51] C++：显式类型转换
来源：http://ikv.zhiwuduotai.top

static_cast<double>(a) / b
来源：http://tzt.ehwqpu.com

[S52] C++：const 与 noexcept
来源：http://azd.dianchejie.cn

int size() const noexcept { return n_; }
来源：http://dul.zhixingplan.top

[S53] C++：移动语义
来源：http://gqq.hesvh.cn

std::vector<int> w = std::move(v);
来源：http://bqt.zdbjq.cn

[S54] C++：异常处理
来源：http://umu.yuanzhike.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eta.wangshuangyany.cn

[S55] C++：结构化绑定
来源：http://enh.jqgufenzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qhx.vehdjk.com

[S56] C++：optional
来源：http://hdw.yfazqb.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tje.yfazqb.com

[S57] C++：编译期常量
来源：http://unj.nwbrower.top

constexpr int N = 10;
来源：http://xwk.sxryk.cn

[S58] C++：命名空间
来源：http://pfh.aibaodan.cn

namespace ns { int f() { return 1; } }
来源：http://kjf.zdqjudy.top

[S59] C++：静态断言
来源：http://xgb.gogol.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dqw.shanyushiyangkeji.top

[S60] C++：遍历并删除元素
来源：http://qvg.aibaodan.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://whl.gaohongyu789.top

================================================================================
来源：http://xmj.ydjk.org.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cig.shanyushiyangtech.top

================================================================================
来源：http://bju.tanke756.top

[T01] Kotlin：Hello World
来源：http://cbe.iojbl.cn

println("Hello")
来源：http://csg.hywenlv.cn

[T02] Kotlin：变量
来源：http://rjo.tanke756.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bll.nanxuanxn.top

[T03] Kotlin：字符串模板
来源：http://ave.daria6918.cn

"值: $b"
来源：http://ttm.jqgufenzy.top

[T04] Kotlin：空安全
来源：http://fdi.xylfe.cn

val n: String? = null;  n?.length
来源：http://kkd.tanke756.top

[T05] Kotlin：when 表达式
来源：http://irz.fengsongda.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ysa.fengsongda.top

[T06] Kotlin：集合映射
来源：http://gkp.gzhubu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://pha.havefunace.top

[T07] Kotlin：集合过滤
来源：http://uwc.gotoacloud.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://pzl.tian-w.cn

[T08] Kotlin：数据类
来源：http://jsk.sjlbkw.cn

data class User(val name: String, val age: Int)
来源：http://vzn.cdnleiting.top

[T09] Kotlin：扩展函数
来源：http://wag.sjlbkw.cn

fun String.exclaim() = this + "!"
来源：http://gid.yfazqb.com

[T10] Kotlin：默认参数
来源：http://hcm.316326.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://nmr.vqdsnc.cn

[T11] Kotlin：协程
来源：http://jvd.ybcxt.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://nuy.ywan-chungtsiang.top

[T12] Kotlin：解构声明
来源：http://zwt.zhaomingkeji.xyz

val (a, b) = Pair(1, 2)
来源：http://fzr.ybcxt.top

[T13] Kotlin：只读 Map
来源：http://uzr.jinyuanbaomall.cn

val m = mapOf("a" to 1)
来源：http://amf.cashguo.top

[T14] Kotlin：循环
来源：http://ghg.fktsv.cn

for (i in 1..10) println(i)
来源：http://jvy.sjlbkw.cn


<!-- 参考信息 -->