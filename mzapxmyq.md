代发 wailian999

case "$1" in
来源：http://nvu.svipenyu.cn

start) echo "启动" ;;
来源：http://qxw.daria6918.cn

stop)  echo "停止" ;;
来源：http://iij.sysykeji.top

*)     echo "未知命令" ;;
来源：http://pih.dianchejie.cn

esac
来源：http://gmu.9152youxi.cn

[R12] for 遍历文件
来源：http://irk.nwbrower.top

for f in *.txt; do echo "$f"; done
来源：http://fri.uphjek.com

[R13] for 计数循环
来源：http://gor.bbcook.cn

for i in {1..10}; do echo "$i"; done
来源：http://ypa.ppjwa.cn

[R14] C 风格 for
来源：http://fey.haohaochexian.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pqm.hammf.cn

[R15] while 逐行读文件
来源：http://tmh.xuanzx.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vwl.aizwys.cn

[R16] until 等待条件
来源：http://pgj.9152youxi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ids.haohaochexian.top

[R17] 数组定义与取值
来源：http://itt.tanke756.top

arr=(a b c); echo "${arr[0]}"
来源：http://wud.havefunace.top

[R18] 遍历数组
来源：http://rgz.meibo888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bnj.aizwys.cn

[R19] 数组长度
来源：http://vbh.gaohongyu789.top

echo "${#arr[@]}"
来源：http://buv.bbcook.cn

[R20] 关联数组（字典）
来源：http://bmm.hnqzz.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ttf.jqgufenzy.top

[R21] 字符串长度
来源：http://hvt.cdnleiting.top

echo "${#s}"
来源：http://vgz.shanyushiyangkeji.top

[R22] 截取子串
来源：http://vtu.iojbl.cn

echo "${s:0:5}"
来源：http://hlq.yonumen.top

[R23] 字符串替换
来源：http://qde.snrcjt.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jph.jyoumei.cn

[R24] 大小写转换
来源：http://zud.snrcjt.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xpm.zdbjq.cn

[R25] 去后缀 / 去前缀
来源：http://yjg.chenzaomai.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://vpi.bbcook.cn

[R26] 命令替换
来源：http://jqd.9152youxi.cn

now=$(date +%F); echo "$now"
来源：http://rzd.havefunace.top

[R27] 算术展开
来源：http://izh.shzxlz.cn

echo $((1 + 2 * 3))
来源：http://tfu.yanxiufei.cn

[R28] 浮点运算
来源：http://pyc.guannengcc.top

echo "scale=2; 10/3" | bc
来源：http://ivn.hnxiangtu.top

[R29] 定义函数
来源：http://vwz.tanke756.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kzo.cheryme.top

[R30] 函数返回状态码
来源：http://yfa.xuetiantiany.cn

f() { return 0; }; f || echo "失败了"
来源：http://fmd.hnqzz.top

[R31] 局部变量
来源：http://tym.jianghu66.top

f() { local x=1; echo "$x"; }
来源：http://rdg.chenlongwang.top

[R32] 参数个数校验
来源：http://icm.iojbl.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fcx.andypj.xyz

[R33] 捕获错误并提示行号
来源：http://usx.jqgfzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ehi.daria6918.cn

[R34] 退出时清理
来源：http://cas.meibo888.top

trap 'rm -f "$tmp"' EXIT
来源：http://mbj.cqqwz.cn

[R35] 后台执行并等待
来源：http://xdb.mhx1999.top

sleep 5 & pid=$!; wait "$pid"
来源：http://sqh.smart0.xyz

[R36] 并发执行多个任务
来源：http://rdx.yonumen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jbk.pengpengdd.cyou

[R37] 把输出赋给变量
来源：http://jcz.hongshengwenyu.top

files=$(ls -1)
来源：http://eyd.wangdashe.top

[R38] 管道串联
来源：http://hie.gotoacloud.top

cat a.txt | grep -i error | wc -l
来源：http://fnw.xziqi.cn

[R39] 重定向标准输出与错误
来源：http://fus.daxiang520.top

cmd > out.log 2>&1
来源：http://ckh.shzxlz.cn

[R40] 追加写日志
来源：http://ios.hywenlv.cn

echo "log" >> out.log
来源：http://bcb.zdqjudy.top

[R41] 丢弃输出
来源：http://bnz.jlsjyb.cn

cmd >/dev/null 2>&1
来源：http://cff.xuanzx.com

[R42] 输入重定向
来源：http://vqi.yvedp.cn

wc -l < a.txt
来源：http://kht.jlsjyb.cn

[R43] 按名字查找文件
来源：http://vul.smart0.xyz

find . -name "*.log" -type f
来源：http://kas.cdnleiting.top

[R44] 按修改时间查找
来源：http://gxr.jqgufenzy.top

find . -mtime -7 -type f
来源：http://whq.xingfuxueyuan.xyz

[R45] 批量删除
来源：http://jpn.epnwcf.com

find . -name "*.tmp" -delete
来源：http://lfj.cashguo.top

[R46] 递归替换文件内容
来源：http://tbc.pengpengdd.cyou

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nin.guannengcc.top

[R47] sed 单行替换
来源：http://ipl.sjlbkw.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wmc.yuxming.cn

[R48] awk 取指定列
来源：http://knt.jlsjyb.cn

awk '{print $1, $3}' a.txt
来源：http://few.tarul.cn

[R49] awk 带条件
来源：http://rbo.jinghuilouyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tqm.cdnleiting.top

[R50] awk 求和
来源：http://pwa.cdnleiting.top

awk '{s += $2} END {print s}' a.txt
来源：http://mnc.shuidangran.top

[R51] 排序去重取前几
来源：http://mps.zhijiandao.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rvo.hfpthk.cn

[R52] 统计行数
来源：http://spr.pycfn.com

wc -l a.txt
来源：http://vbm.aizwys.cn

[R53] 查看文件头与实时尾
来源：http://oec.ywan-chungtsiang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ukc.hnqzz.top

[R54] 比较两个文件
来源：http://emd.aizwys.cn

diff a.txt b.txt
来源：http://lqk.tarul.cn

[R55] 压缩与解压
来源：http://zdi.redwolf501.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ewm.iojbl.cn

[R56] 远程拷贝
来源：http://wgh.zycfv.cn

scp file user@host:/path/
来源：http://njj.gzhubu.top

[R57] 远程执行命令
来源：http://bvj.dashuyun.cn

ssh user@host 'uptime'
来源：http://dnd.birdmap.top

[R58] 下载文件
来源：http://lki.yuxming.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mke.svipenyu.cn

[R59] 发 POST JSON
来源：http://rvb.uphjek.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sew.nwbrower.top

[R60] 只看 HTTP 状态码
来源：http://fcr.yvedp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mso.c1oappe.top

[R61] 磁盘占用
来源：http://zxi.yfazqb.com

df -h;  du -sh *
来源：http://pqn.jianghu66.top

[R62] 找最占空间的文件
来源：http://ole.hcnkem.com

du -ah . | sort -rh | head -10
来源：http://wop.zhongyouzk.top

[R63] 内存与进程
来源：http://omg.guannengcc.top

free -h;  ps aux | grep nginx
来源：http://atc.shangyingyoupin.top

[R64] 结束进程
来源：http://wvy.vqdsnc.cn

kill -9 $(pgrep -f app.py)
来源：http://fuy.jinyuanbaomall.cn

[R65] 查看端口占用
来源：http://hps.zhongyouzk.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mpq.ctjpmb.com

[R66] 定时任务
来源：http://qfk.bjfxy.top

crontab -e;  crontab -l
来源：http://kak.dashuyun.cn

[R67] 生成随机十六进制串
来源：http://ylb.sufxvd.cn

openssl rand -hex 16
来源：http://tly.wangshuangyany.cn

[R68] 计算文件校验值
来源：http://wvv.chenlongwang.top

sha256sum a.txt;  md5sum a.txt
来源：http://ytf.shuidangran.top

[R69] 生成随机密码
来源：http://atq.jqgufenzy.top

head -c 16 /dev/urandom | base64
来源：http://zim.mhx1999.top

[R70] 时间戳与互转
来源：http://fcy.cqqwz.cn

date +%s;  date -d @1700000000
来源：http://tle.52xcode.cn

[R71] 日期格式化
来源：http://ugr.fengsongda.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bdw.zhaomingkeji.xyz

[R72] 等待端口就绪
来源：http://erc.9152youxi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xhz.smart0.xyz

[R73] 分割大日志
来源：http://xfw.yuxming.cn

split -l 1000 big.log part_
来源：http://tju.hammf.cn

[R74] 批量重命名
来源：http://vra.jinqigfzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jkz.yvedp.cn

[R75] 导出环境变量
来源：http://oyd.zdqjudy.top

export PATH="$HOME/bin:$PATH"
来源：http://kfs.chenzaomai.com

[R76] 使用临时文件
来源：http://uot.yj202588.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bjp.yongpay.top

[R77] 读取用户输入
来源：http://qth.hnqzz.top

read -rp "请输入: " ans
来源：http://emi.guannengcc.top

[R78] 交互式菜单
来源：http://pul.shzxlz.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sim.yfazqb.com

[R79] 解析命令行选项
来源：http://zdl.xinyue.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jpc.jyoumei.cn

[R80] 查看脚本执行耗时
来源：http://eds.yfazqb.com

time ./run.sh
来源：http://bri.dianchejie.cn

================================================================================
来源：http://bbh.yvedp.cn

S. C / C++ 专题
来源：http://fxl.ppjwa.cn

================================================================================
来源：http://nng.zhiwuduotai.top

[S01] C：Hello World
来源：http://csx.ydjk.org.cn

#include <stdio.h>
来源：http://gmy.jinghuilouyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jit.yuxming.cn

[S02] C：变量与格式化输出
来源：http://fdm.jinqigufen.top

int a = 10; printf("%d\n", a);
来源：http://zne.yanxiufei.cn

[S03] C：读入整数
来源：http://aft.haohaochexian.top

int x; scanf("%d", &x);
来源：http://ccd.iojbl.cn

[S04] C：字符串复制
来源：http://fxb.meibo888.top

char dst[32]; strcpy(dst, "hi");
来源：http://hli.zhijiandao.cn

[S05] C：字符串长度
来源：http://aem.quarkkingdee.top

strlen(s)
来源：http://tju.zhongyouzk.top

[S06] C：字符串比较
来源：http://wyq.iojbl.cn

strcmp(a, b) == 0
来源：http://uzw.yfazqb.com

[S07] C：数组遍历求和
来源：http://ixx.yj20258888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lzl.zycfv.cn

[S08] C：动态内存分配与释放
来源：http://bsv.jlsjyb.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://spv.jinyuanbaomall.cn

[S09] C：结构体定义与初始化
来源：http://gjb.bjfxy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kbo.haohaochexian.top

[S10] C：指针与解引用
来源：http://ckq.gogol.net.cn

int *p = &a;  *p = 5;
来源：http://tib.feifeiyinyue.top

[S11] C：逐行读文件
来源：http://mtj.9152youxi.cn

FILE *f = fopen("a.txt", "r");
来源：http://icb.hesvh.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xlr.quarkkingdee.top

fclose(f);
来源：http://ttf.guowangkeji.top

[S12] C：写文件
来源：http://znb.yj20258888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mbz.snrcjt.cn

[S13] C：宏定义
来源：http://qvj.nanxinkj.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ebm.tarul.cn

[S14] C：枚举
来源：http://jbm.kuanghao11.cn

enum Color { RED, GREEN, BLUE };
来源：http://xtd.zhoulong.xyz

[S15] C：类型转换
来源：http://nej.zhixingplan.top

(double) a / b
来源：http://sck.dashuyun.cn

[S16] C：位操作置位
来源：http://dru.yonumen.top

x |= (1 << 3);
来源：http://uxr.zdqjudy.top

[S17] C：安全拼接字符串
来源：http://dkh.aibaodan.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vic.uphjek.com

[S18] C：命令行参数
来源：http://edj.hongshengwenyu.top

int main(int argc, char **argv)
来源：http://uyc.yueranfly.top

[S19] C：快速排序
来源：http://zzk.sysykeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://fht.iojbl.cn

[S20] C：二分查找
来源：http://mwm.zhixingplan.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nnt.fktsv.cn

[S21] C：字符类别判断
来源：http://ymu.tian-w.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vbm.daria6918.cn

[S22] C：字符串转数字
来源：http://drc.hesvh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://exc.tanke756.top

[S23] C：随机数
来源：http://zwz.guowangkeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://hsf.wangshuangyany.cn

[S24] C：获取本地时间
来源：http://dvo.0kj1m.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zdz.mhx1999.top

[S25] C：内存拷贝
来源：http://sgj.aibaodan.cn

memcpy(dst, src, n);
来源：http://fmx.yvedp.cn

[S26] C：内存清零
来源：http://lrw.shzxlz.cn

memset(a, 0, sizeof a);
来源：http://tki.fktsv.cn

[S27] C：定义常量
来源：http://jgm.jinghuilouyu.cn

const double PI = 3.14159;
来源：http://avk.jqgufenzy.top

[S28] C：静态变量
来源：http://cgj.yanxiufei.cn

static int counter = 0;
来源：http://hio.wangdashe.top

[S29] C：变参函数
来源：http://ivi.0kj1m.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fxo.fanxiaobao.xyz

[S30] C：头文件保护
来源：http://rcu.xuetiantiany.cn

#ifndef X_H
来源：http://ram.c1oappe.top

#define X_H
来源：http://ftm.sjlbkw.cn

#endif
来源：http://uqq.ppjwa.cn

[S31] C++：Hello World
来源：http://omg.tanke756.top

#include <iostream>
来源：http://akj.meibo888.top

int main() { std::cout << "Hello\n"; }
来源：http://yde.hesvh.cn

[S32] C++：字符串
来源：http://rth.pycfn.com

std::string s = "hi";  s += "!";
来源：http://toj.yvedp.cn

[S33] C++：vector 增删
来源：http://rcx.yonumen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ckv.9152youxi.cn

[S34] C++：遍历 vector
来源：http://ksw.daria6918.cn

for (auto &x : v) { std::cout << x; }
来源：http://yri.cheryme.top

[S35] C++：map
来源：http://jyi.ehwqpu.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tvn.zhoulong.xyz

[S36] C++：unordered_map
来源：http://wpr.jqgfzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tdy.yj202588.top

[S37] C++：set
来源：http://bfs.shangyingyoupin.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://imi.jqgfzy.top

[S38] C++：排序
来源：http://sic.hnqzz.top

std::sort(v.begin(), v.end());
来源：http://oxf.yj20258888.top

[S39] C++：自定义比较器排序
来源：http://nze.epnwcf.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ytp.xinyue.icu

[S40] C++：查找元素
来源：http://uoq.nwbrower.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jee.hcnkem.com

[S41] C++：类与构造函数
来源：http://fci.daxiang520.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ftj.jinqigufen.top

[S42] C++：继承与虚函数
来源：http://xxi.xuanzx.com

class B : public Base { public: void f() override {} };
来源：http://oan.smart0.xyz

[S43] C++：智能指针
来源：http://thc.yj20258888.top

auto p = std::make_unique<int>(5);
来源：http://beh.tianlin.xyz

[S44] C++：引用传参
来源：http://iqp.jlsjyb.cn

void inc(int &x) { ++x; }
来源：http://kwj.redwolf501.top

[S45] C++：lambda
来源：http://fak.daria6918.cn

auto add = [](int a, int b) { return a + b; };
来源：http://abl.gaohongyu789.top

[S46] C++：函数模板
来源：http://mgo.quarkkingdee.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dmg.jiagoushi.top

[S47] C++：结构化绑定遍历
来源：http://ecd.nanxinkj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://eop.sysykeji.top

[S48] C++：逐行读文件
来源：http://sgh.zhengqikj.top

std::ifstream in("a.txt");  std::string line;
来源：http://hal.yvedp.cn

while (std::getline(in, line)) { }
来源：http://prb.birdmap.top

[S49] C++：写文件
来源：http://sya.fengsongda.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lbz.birdmap.top

[S50] C++：格式化数字
来源：http://tdk.guannengcc.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zdy.ivvv.top

[S51] C++：显式类型转换
来源：http://mfj.fktsv.cn

static_cast<double>(a) / b
来源：http://yto.wangdashe.top

[S52] C++：const 与 noexcept
来源：http://mbp.shanyushiyangtech.top

int size() const noexcept { return n_; }
来源：http://wlg.jinqigufen.top

[S53] C++：移动语义
来源：http://lud.chenzaomai.com

std::vector<int> w = std::move(v);
来源：http://tfl.chenlongwang.top

[S54] C++：异常处理
来源：http://rsr.yuanzhike.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://edm.9152youxi.cn

[S55] C++：结构化绑定
来源：http://cvu.kuanghao11.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wqx.bjfxy.top

[S56] C++：optional
来源：http://ual.chenzaomai.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pqb.daria6918.cn

[S57] C++：编译期常量
来源：http://wtd.316326.xyz

constexpr int N = 10;
来源：http://ixc.jinghuilouyu.cn

[S58] C++：命名空间
来源：http://pxh.shanyushiyangkeji.top

namespace ns { int f() { return 1; } }
来源：http://mtt.9152youxi.cn

[S59] C++：静态断言
来源：http://aoq.ywan-chungtsiang.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jcf.shzxlz.cn

[S60] C++：遍历并删除元素
来源：http://ver.wangshuangyany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://brn.jiagoushi.top

================================================================================
来源：http://fgi.gogol.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gzf.zhaomingkeji.xyz

================================================================================
来源：http://unx.tanke756.top

[T01] Kotlin：Hello World
来源：http://lba.jyoumei.cn

println("Hello")
来源：http://ejw.svipenyu.cn

[T02] Kotlin：变量
来源：http://bpi.xylfe.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rtb.tanke756.top

[T03] Kotlin：字符串模板
来源：http://ttv.fehbvm.com

"值: $b"
来源：http://fwz.yueranfly.top

[T04] Kotlin：空安全
来源：http://pqi.ppjwa.cn

val n: String? = null;  n?.length
来源：http://qwh.epnwcf.com

[T05] Kotlin：when 表达式
来源：http://lof.c1oappe.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lir.cheryme.top

[T06] Kotlin：集合映射
来源：http://jyg.pengpengdd.cyou

listOf(1, 2, 3).map { it * 2 }
来源：http://kov.gaohongyu789.top

[T07] Kotlin：集合过滤
来源：http://keq.sjlbkw.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ggt.sufxvd.cn

[T08] Kotlin：数据类
来源：http://inb.zhaomingkeji.xyz

data class User(val name: String, val age: Int)
来源：http://uhi.daria6918.cn

[T09] Kotlin：扩展函数
来源：http://vzf.iojbl.cn

fun String.exclaim() = this + "!"
来源：http://xnn.snrcjt.cn

[T10] Kotlin：默认参数
来源：http://ofi.xziqi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qle.xinyue.icu

[T11] Kotlin：协程
来源：http://flp.cashguo.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://vwv.hongshengwenyu.top

[T12] Kotlin：解构声明
来源：http://czb.chenjidiqi.icu

val (a, b) = Pair(1, 2)
来源：http://hri.sufxvd.cn


<!-- 参考信息 -->