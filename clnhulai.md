代发 wailian999

esac
来源：http://srf.pengpengdd.cyou

[R12] for 遍历文件
来源：http://ynr.chenjidiqi.icu

for f in *.txt; do echo "$f"; done
来源：http://pzb.chenlongwang.top

[R13] for 计数循环
来源：http://rmp.xuanzx.com

for i in {1..10}; do echo "$i"; done
来源：http://wrg.hnxiangtu.top

[R14] C 风格 for
来源：http://rci.redwolf501.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://avi.meibo888.top

[R15] while 逐行读文件
来源：http://kxq.yvedp.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ctq.xziqi.cn

[R16] until 等待条件
来源：http://fmy.birdmap.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://msc.yuxming.cn

[R17] 数组定义与取值
来源：http://dna.svipenyu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://umn.aibaodan.cn

[R18] 遍历数组
来源：http://nny.dashuyun.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gyw.zhoulong.xyz

[R19] 数组长度
来源：http://ftn.wangshuangyany.cn

echo "${#arr[@]}"
来源：http://xbm.hfpthk.cn

[R20] 关联数组（字典）
来源：http://cip.cqqwz.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://isi.hesvh.cn

[R21] 字符串长度
来源：http://xpq.ehwqpu.com

echo "${#s}"
来源：http://svf.tianlin.xyz

[R22] 截取子串
来源：http://erx.guowangkeji.top

echo "${s:0:5}"
来源：http://hqn.c1oappe.top

[R23] 字符串替换
来源：http://ezy.ehwqpu.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ugf.xuetiantiany.cn

[R24] 大小写转换
来源：http://roq.yonumen.top

echo "${s^^}"; echo "${s,,}"
来源：http://hss.tanke756.top

[R25] 去后缀 / 去前缀
来源：http://ktl.uphjek.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://xyr.daria6918.cn

[R26] 命令替换
来源：http://aub.hnqzz.top

now=$(date +%F); echo "$now"
来源：http://kdi.iojbl.cn

[R27] 算术展开
来源：http://ehp.gogol.net.cn

echo $((1 + 2 * 3))
来源：http://zkn.tianlin.xyz

[R28] 浮点运算
来源：http://jwk.daxiang520.top

echo "scale=2; 10/3" | bc
来源：http://vkk.fzhhl.top

[R29] 定义函数
来源：http://uaz.jianghu66.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dlu.hcnkem.com

[R30] 函数返回状态码
来源：http://jby.jinqigufen.top

f() { return 0; }; f || echo "失败了"
来源：http://srn.nwbrower.top

[R31] 局部变量
来源：http://yug.feifeiyinyue.top

f() { local x=1; echo "$x"; }
来源：http://xio.ydzc1.top

[R32] 参数个数校验
来源：http://xjz.pengpengdd.cyou

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fne.ctjpmb.com

[R33] 捕获错误并提示行号
来源：http://dym.aizwys.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ltp.dashuyun.cn

[R34] 退出时清理
来源：http://gyo.gaohongyu789.top

trap 'rm -f "$tmp"' EXIT
来源：http://tdl.hammf.cn

[R35] 后台执行并等待
来源：http://zaj.aibaodan.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hpx.52xcode.cn

[R36] 并发执行多个任务
来源：http://hqt.xziqi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fhz.yanxiufei.cn

[R37] 把输出赋给变量
来源：http://jko.zhengqikj.top

files=$(ls -1)
来源：http://gwz.svipenyu.cn

[R38] 管道串联
来源：http://npy.shanyushiyangtech.top

cat a.txt | grep -i error | wc -l
来源：http://dvh.xinyue.icu

[R39] 重定向标准输出与错误
来源：http://tee.yueranfly.top

cmd > out.log 2>&1
来源：http://szg.gotoacloud.top

[R40] 追加写日志
来源：http://odk.nanxuanxn.top

echo "log" >> out.log
来源：http://jbk.ydjk.org.cn

[R41] 丢弃输出
来源：http://nmk.yuanzhike.top

cmd >/dev/null 2>&1
来源：http://ynn.ivvv.top

[R42] 输入重定向
来源：http://gmu.vqdsnc.cn

wc -l < a.txt
来源：http://fsk.andypj.xyz

[R43] 按名字查找文件
来源：http://djl.zhengqikj.top

find . -name "*.log" -type f
来源：http://lfa.jlsjyb.cn

[R44] 按修改时间查找
来源：http://pjn.jianghu66.top

find . -mtime -7 -type f
来源：http://tgj.aizwys.cn

[R45] 批量删除
来源：http://lel.fanxiaobao.xyz

find . -name "*.tmp" -delete
来源：http://fjs.ppjwa.cn

[R46] 递归替换文件内容
来源：http://ezj.xinyue.icu

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kvj.sjlbkw.cn

[R47] sed 单行替换
来源：http://iem.andypj.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://zca.yongpay.top

[R48] awk 取指定列
来源：http://omy.316326.xyz

awk '{print $1, $3}' a.txt
来源：http://ykr.jqgfzy.top

[R49] awk 带条件
来源：http://rpz.cdnleiting.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rbd.ydzc1.top

[R50] awk 求和
来源：http://yvy.daria6918.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ehi.hammf.cn

[R51] 排序去重取前几
来源：http://rsc.dianchejie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vxx.cashguo.top

[R52] 统计行数
来源：http://hrk.haohaochexian.top

wc -l a.txt
来源：http://uei.gaohongyu789.top

[R53] 查看文件头与实时尾
来源：http://uzp.shzxlz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://twj.smart0.xyz

[R54] 比较两个文件
来源：http://ilb.jqgfzy.top

diff a.txt b.txt
来源：http://wny.pycfn.com

[R55] 压缩与解压
来源：http://mez.mhx1999.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jvb.gzhubu.top

[R56] 远程拷贝
来源：http://hdi.sxryk.cn

scp file user@host:/path/
来源：http://fji.ehwqpu.com

[R57] 远程执行命令
来源：http://mwx.ydzc1.top

ssh user@host 'uptime'
来源：http://euq.fzhhl.top

[R58] 下载文件
来源：http://qyk.jinyuanbaomall.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zyt.ehwqpu.com

[R59] 发 POST JSON
来源：http://xfq.zhongyouzk.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://srh.pengpengdd.cyou

[R60] 只看 HTTP 状态码
来源：http://gxk.xuetiantiany.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gnb.xuanzx.com

[R61] 磁盘占用
来源：http://lew.nanxinkj.top

df -h;  du -sh *
来源：http://tja.quarkkingdee.top

[R62] 找最占空间的文件
来源：http://mfy.yonumen.top

du -ah . | sort -rh | head -10
来源：http://udv.hfpthk.cn

[R63] 内存与进程
来源：http://ysi.shanyushiyangkeji.top

free -h;  ps aux | grep nginx
来源：http://ocn.birdmap.top

[R64] 结束进程
来源：http://wpq.quarkkingdee.top

kill -9 $(pgrep -f app.py)
来源：http://imm.vqdsnc.cn

[R65] 查看端口占用
来源：http://mtm.hesvh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tsl.xziqi.cn

[R66] 定时任务
来源：http://sof.nanxinkj.top

crontab -e;  crontab -l
来源：http://prn.jinghuilouyu.cn

[R67] 生成随机十六进制串
来源：http://rlf.yonumen.top

openssl rand -hex 16
来源：http://edu.vqdsnc.cn

[R68] 计算文件校验值
来源：http://kjw.andypj.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://uaw.zhixingplan.top

[R69] 生成随机密码
来源：http://yrb.guannengcc.top

head -c 16 /dev/urandom | base64
来源：http://atq.aibaodan.cn

[R70] 时间戳与互转
来源：http://gqg.hysaishi.cn

date +%s;  date -d @1700000000
来源：http://odk.zycfv.cn

[R71] 日期格式化
来源：http://nyg.sjlbkw.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hiv.fehbvm.com

[R72] 等待端口就绪
来源：http://jqz.zhijiandao.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rmn.nwbrower.top

[R73] 分割大日志
来源：http://ocq.zhijiandao.cn

split -l 1000 big.log part_
来源：http://wvb.hysaishi.cn

[R74] 批量重命名
来源：http://pgv.shuidangran.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xcf.52xcode.cn

[R75] 导出环境变量
来源：http://acx.jiagoushi.top

export PATH="$HOME/bin:$PATH"
来源：http://yjh.ehwqpu.com

[R76] 使用临时文件
来源：http://mky.chenlongwang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wnj.iojbl.cn

[R77] 读取用户输入
来源：http://mgn.sjlbkw.cn

read -rp "请输入: " ans
来源：http://dcj.ydzc1.top

[R78] 交互式菜单
来源：http://cjc.bjfxy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://fwc.yanxiufei.cn

[R79] 解析命令行选项
来源：http://tta.haohaochexian.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pfz.fanxiaobao.xyz

[R80] 查看脚本执行耗时
来源：http://san.hammf.cn

time ./run.sh
来源：http://bka.gzhubu.top

================================================================================
来源：http://xaw.pycfn.com

S. C / C++ 专题
来源：http://swu.hywenlv.cn

================================================================================
来源：http://coe.316326.xyz

[S01] C：Hello World
来源：http://cga.bbcook.cn

#include <stdio.h>
来源：http://omy.hcnkem.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://hxw.gotoacloud.top

[S02] C：变量与格式化输出
来源：http://cha.wangdashe.top

int a = 10; printf("%d\n", a);
来源：http://dei.shangyingyoupin.top

[S03] C：读入整数
来源：http://ble.jiagoushi.top

int x; scanf("%d", &x);
来源：http://zii.nwbrower.top

[S04] C：字符串复制
来源：http://mhz.uphjek.com

char dst[32]; strcpy(dst, "hi");
来源：http://wxr.daxiang520.top

[S05] C：字符串长度
来源：http://yeg.jlsjyb.cn

strlen(s)
来源：http://uud.aibaodan.cn

[S06] C：字符串比较
来源：http://fre.gaohongyu789.top

strcmp(a, b) == 0
来源：http://idr.redwolf501.top

[S07] C：数组遍历求和
来源：http://qfc.gogol.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://idd.yuxming.cn

[S08] C：动态内存分配与释放
来源：http://uly.zhengqikj.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ido.wangshuangyany.cn

[S09] C：结构体定义与初始化
来源：http://txw.wangdashe.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dkw.shanyushiyangkeji.top

[S10] C：指针与解引用
来源：http://gxu.jianghu66.top

int *p = &a;  *p = 5;
来源：http://kvz.zhijiandao.cn

[S11] C：逐行读文件
来源：http://tqm.cheryme.top

FILE *f = fopen("a.txt", "r");
来源：http://pct.bbcook.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mbv.yangfankeji.com

fclose(f);
来源：http://pzu.ivvv.top

[S12] C：写文件
来源：http://utg.yangfankeji.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tiu.dashuyun.cn

[S13] C：宏定义
来源：http://jrp.jinqigufen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tsf.ydjk.org.cn

[S14] C：枚举
来源：http://bju.mhx1999.top

enum Color { RED, GREEN, BLUE };
来源：http://bjq.zhijiandao.cn

[S15] C：类型转换
来源：http://rxr.hysaishi.cn

(double) a / b
来源：http://aoq.redwolf501.top

[S16] C：位操作置位
来源：http://anc.yj20258888.top

x |= (1 << 3);
来源：http://ent.uphjek.com

[S17] C：安全拼接字符串
来源：http://two.jqgfzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zfr.xuanzx.com

[S18] C：命令行参数
来源：http://lxv.uphjek.com

int main(int argc, char **argv)
来源：http://byq.feifeiyinyue.top

[S19] C：快速排序
来源：http://mkx.vqdsnc.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jnr.c1oappe.top

[S20] C：二分查找
来源：http://qyo.chenlongwang.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pbm.ybcxt.top

[S21] C：字符类别判断
来源：http://bqb.redwolf501.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dtq.sweek.top

[S22] C：字符串转数字
来源：http://cfk.hcnkem.com

atoi("42");  strtod("3.14", NULL);
来源：http://tsi.ywan-chungtsiang.top

[S23] C：随机数
来源：http://iab.zhijiandao.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://uow.zhiwuduotai.top

[S24] C：获取本地时间
来源：http://iiw.tanke756.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ywd.bjfxy.top

[S25] C：内存拷贝
来源：http://igj.yfazqb.com

memcpy(dst, src, n);
来源：http://xyc.jinyuanbaomall.cn

[S26] C：内存清零
来源：http://jkp.tanke756.top

memset(a, 0, sizeof a);
来源：http://iae.ydjk.org.cn

[S27] C：定义常量
来源：http://amb.jinqigfzy.top

const double PI = 3.14159;
来源：http://yog.xuetiantiany.cn

[S28] C：静态变量
来源：http://hfq.ctjpmb.com

static int counter = 0;
来源：http://cqh.vqdsnc.cn

[S29] C：变参函数
来源：http://xam.cqqwz.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zea.shzxlz.cn

[S30] C：头文件保护
来源：http://ius.ivvv.top

#ifndef X_H
来源：http://lbx.0kj1m.cn

#define X_H
来源：http://fsb.fzhhl.top

#endif
来源：http://blz.fengsongda.top

[S31] C++：Hello World
来源：http://uvc.jianghu66.top

#include <iostream>
来源：http://nph.hysaishi.cn

int main() { std::cout << "Hello\n"; }
来源：http://nmc.uphjek.com

[S32] C++：字符串
来源：http://jme.zhijiandao.cn

std::string s = "hi";  s += "!";
来源：http://fhe.zhoulong.xyz

[S33] C++：vector 增删
来源：http://rdx.jinghuilouyu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bfq.pengpengdd.cyou

[S34] C++：遍历 vector
来源：http://aja.zhiwuduotai.top

for (auto &x : v) { std::cout << x; }
来源：http://llr.hesvh.cn

[S35] C++：map
来源：http://dxn.hysaishi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nwh.zhixingplan.top

[S36] C++：unordered_map
来源：http://xac.feifeiyinyue.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qta.haohaochexian.top

[S37] C++：set
来源：http://gpp.zdqjudy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://agc.aizwys.cn

[S38] C++：排序
来源：http://rgm.zycfv.cn

std::sort(v.begin(), v.end());
来源：http://phy.chenlongwang.top

[S39] C++：自定义比较器排序
来源：http://zhg.yfazqb.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lti.ctjpmb.com

[S40] C++：查找元素
来源：http://qpj.xuetiantiany.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eku.cdnleiting.top

[S41] C++：类与构造函数
来源：http://lko.tian-w.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sjt.cucudq.cn

[S42] C++：继承与虚函数
来源：http://ext.hongshengwenyu.top

class B : public Base { public: void f() override {} };
来源：http://gaf.jinghuilouyu.cn

[S43] C++：智能指针
来源：http://hck.wangshuangyany.cn

auto p = std::make_unique<int>(5);
来源：http://wdx.hnqzz.top

[S44] C++：引用传参
来源：http://bia.zdbjq.cn

void inc(int &x) { ++x; }
来源：http://dej.wangdashe.top

[S45] C++：lambda
来源：http://ycr.ydzc1.top

auto add = [](int a, int b) { return a + b; };
来源：http://rik.yueranfly.top

[S46] C++：函数模板
来源：http://qjm.quarkkingdee.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xfs.cheryme.top

[S47] C++：结构化绑定遍历
来源：http://uss.jqgufenzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://igr.daria6918.cn

[S48] C++：逐行读文件
来源：http://isa.xziqi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lyx.fehbvm.com

while (std::getline(in, line)) { }
来源：http://ind.gzhubu.top

[S49] C++：写文件
来源：http://qas.jinqigufen.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pad.fanxiaobao.xyz

[S50] C++：格式化数字
来源：http://acg.jqgufenzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ofo.gogol.net.cn

[S51] C++：显式类型转换
来源：http://erz.vqdsnc.cn

static_cast<double>(a) / b
来源：http://eob.shanyushiyangkeji.top

[S52] C++：const 与 noexcept
来源：http://cqn.jiagoushi.top

int size() const noexcept { return n_; }
来源：http://fda.xylfe.cn

[S53] C++：移动语义
来源：http://ziw.yj20258888.top

std::vector<int> w = std::move(v);
来源：http://ilb.epnwcf.com

[S54] C++：异常处理
来源：http://ahx.cheryme.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://waz.0kj1m.cn

[S55] C++：结构化绑定
来源：http://vbb.ivvv.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zuf.hfpthk.cn

[S56] C++：optional
来源：http://agk.sufxvd.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://way.zhongyouzk.top

[S57] C++：编译期常量
来源：http://iik.aizwys.cn

constexpr int N = 10;
来源：http://fig.yanxiufei.cn

[S58] C++：命名空间
来源：http://rnc.tanke756.top

namespace ns { int f() { return 1; } }
来源：http://fos.fktsv.cn

[S59] C++：静态断言
来源：http://ijx.gaohongyu789.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nux.gotoacloud.top

[S60] C++：遍历并删除元素
来源：http://gsl.shzxlz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kpx.hnxiangtu.top

================================================================================
来源：http://zak.cdnleiting.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://imw.jqgfzy.top

================================================================================
来源：http://wgn.52xcode.cn

[T01] Kotlin：Hello World
来源：http://kwv.hcnkem.com

println("Hello")
来源：http://zgi.nwbrower.top

[T02] Kotlin：变量
来源：http://zkc.yuanzhike.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ebf.chenjidiqi.icu

[T03] Kotlin：字符串模板
来源：http://izj.jinqigufen.top

"值: $b"
来源：http://alk.jqgufenzy.top

[T04] Kotlin：空安全
来源：http://mhp.guowangkeji.top

val n: String? = null;  n?.length
来源：http://qde.tanke756.top

[T05] Kotlin：when 表达式
来源：http://uce.yj20258888.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xxi.mhx1999.top

[T06] Kotlin：集合映射
来源：http://yyc.fehbvm.com

listOf(1, 2, 3).map { it * 2 }
来源：http://pkc.zhijiandao.cn

[T07] Kotlin：集合过滤
来源：http://joc.sweek.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ixi.shuidangran.top

[T08] Kotlin：数据类
来源：http://xmh.quarkkingdee.top

data class User(val name: String, val age: Int)
来源：http://oqk.yuanzhike.top

[T09] Kotlin：扩展函数
来源：http://bvs.ppjwa.cn

fun String.exclaim() = this + "!"
来源：http://jem.svipenyu.cn

[T10] Kotlin：默认参数
来源：http://ppa.yueranfly.top

fun greet(name: String = "World") = "Hi $name"
来源：http://pka.ppjwa.cn

[T11] Kotlin：协程
来源：http://skm.jinqigufen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://fvi.dashuyun.cn

[T12] Kotlin：解构声明
来源：http://xga.uphjek.com

val (a, b) = Pair(1, 2)
来源：http://trd.jyoumei.cn

[T13] Kotlin：只读 Map
来源：http://dvg.guowangkeji.top

val m = mapOf("a" to 1)
来源：http://nog.sweek.top

[T14] Kotlin：循环
来源：http://jeb.hnxiangtu.top

for (i in 1..10) println(i)
来源：http://zuc.hcnkem.com


<!-- 参考信息 -->