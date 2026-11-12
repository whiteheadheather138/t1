代发 wailian999

esac
来源：http://siw.haohaochexian.top

[R12] for 遍历文件
来源：http://uvp.aibaodan.cn

for f in *.txt; do echo "$f"; done
来源：http://yau.yvedp.cn

[R13] for 计数循环
来源：http://ffh.vehdjk.com

for i in {1..10}; do echo "$i"; done
来源：http://ukw.chenjidiqi.icu

[R14] C 风格 for
来源：http://wsd.aizwys.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kpw.9152youxi.cn

[R15] while 逐行读文件
来源：http://uec.yongpay.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hld.hywenlv.cn

[R16] until 等待条件
来源：http://iso.guowangkeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iyt.vehdjk.com

[R17] 数组定义与取值
来源：http://eav.tarul.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rgq.c1oappe.top

[R18] 遍历数组
来源：http://via.zdbjq.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dcx.shzxlz.cn

[R19] 数组长度
来源：http://iyl.aibaodan.cn

echo "${#arr[@]}"
来源：http://rms.gotoacloud.top

[R20] 关联数组（字典）
来源：http://sgf.meibo888.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fnr.quarkkingdee.top

[R21] 字符串长度
来源：http://pth.nwbrower.top

echo "${#s}"
来源：http://zmv.haohaochexian.top

[R22] 截取子串
来源：http://mma.xingfuxueyuan.xyz

echo "${s:0:5}"
来源：http://dyy.sjlbkw.cn

[R23] 字符串替换
来源：http://bgx.redwolf501.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vxj.0kj1m.cn

[R24] 大小写转换
来源：http://uyx.zhixingplan.top

echo "${s^^}"; echo "${s,,}"
来源：http://hkb.zdqjudy.top

[R25] 去后缀 / 去前缀
来源：http://klc.nanxuanxn.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ihi.shangyingyoupin.top

[R26] 命令替换
来源：http://ply.cucudq.cn

now=$(date +%F); echo "$now"
来源：http://ryz.jqgfzy.top

[R27] 算术展开
来源：http://znz.ehwqpu.com

echo $((1 + 2 * 3))
来源：http://dhu.nanxuanxn.top

[R28] 浮点运算
来源：http://aeq.jlsjyb.cn

echo "scale=2; 10/3" | bc
来源：http://eam.hesvh.cn

[R29] 定义函数
来源：http://crf.snrcjt.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pyc.ybcxt.top

[R30] 函数返回状态码
来源：http://see.shanyushiyangtech.top

f() { return 0; }; f || echo "失败了"
来源：http://pqa.zhaomingkeji.xyz

[R31] 局部变量
来源：http://ywg.shanyushiyangkeji.top

f() { local x=1; echo "$x"; }
来源：http://zzk.chenjidiqi.icu

[R32] 参数个数校验
来源：http://qym.hongshengwenyu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gku.jinqigfzy.top

[R33] 捕获错误并提示行号
来源：http://dgh.xylfe.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nab.yuxming.cn

[R34] 退出时清理
来源：http://yjb.ppjwa.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rpa.guowangkeji.top

[R35] 后台执行并等待
来源：http://okm.shuidangran.top

sleep 5 & pid=$!; wait "$pid"
来源：http://puo.nwbrower.top

[R36] 并发执行多个任务
来源：http://xtw.nwbrower.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mdv.tian-w.cn

[R37] 把输出赋给变量
来源：http://gbr.yj20258888.top

files=$(ls -1)
来源：http://ytt.hnxiangtu.top

[R38] 管道串联
来源：http://ufg.fktsv.cn

cat a.txt | grep -i error | wc -l
来源：http://lqp.zhengqikj.top

[R39] 重定向标准输出与错误
来源：http://vsy.0kj1m.cn

cmd > out.log 2>&1
来源：http://lyu.xuanzx.com

[R40] 追加写日志
来源：http://htx.fzhhl.top

echo "log" >> out.log
来源：http://imj.sufxvd.cn

[R41] 丢弃输出
来源：http://ypj.cdnleiting.top

cmd >/dev/null 2>&1
来源：http://vpr.daxiang520.top

[R42] 输入重定向
来源：http://xab.vehdjk.com

wc -l < a.txt
来源：http://vcv.jinqigfzy.top

[R43] 按名字查找文件
来源：http://cdp.jianghu66.top

find . -name "*.log" -type f
来源：http://str.nwbrower.top

[R44] 按修改时间查找
来源：http://zfm.kuanghao11.cn

find . -mtime -7 -type f
来源：http://rjl.tanke756.top

[R45] 批量删除
来源：http://ybt.0kj1m.cn

find . -name "*.tmp" -delete
来源：http://gsm.ehwqpu.com

[R46] 递归替换文件内容
来源：http://cio.zhiwuduotai.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fjt.hcnkem.com

[R47] sed 单行替换
来源：http://agq.ydzc1.top

sed -i 's/foo/bar/g' a.txt
来源：http://buz.smart0.xyz

[R48] awk 取指定列
来源：http://tfw.gzhubu.top

awk '{print $1, $3}' a.txt
来源：http://axl.chenjidiqi.icu

[R49] awk 带条件
来源：http://ifb.gzhubu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jwj.jinghuilouyu.cn

[R50] awk 求和
来源：http://zri.aizwys.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bpq.ehwqpu.com

[R51] 排序去重取前几
来源：http://dqu.mhx1999.top

sort a.txt | uniq -c | sort -rn | head
来源：http://zhz.gaohongyu789.top

[R52] 统计行数
来源：http://vre.gzhubu.top

wc -l a.txt
来源：http://uga.hammf.cn

[R53] 查看文件头与实时尾
来源：http://uri.fehbvm.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://usi.zdbjq.cn

[R54] 比较两个文件
来源：http://jxn.vehdjk.com

diff a.txt b.txt
来源：http://gap.hesvh.cn

[R55] 压缩与解压
来源：http://gtg.vqdsnc.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pfx.zhoulong.xyz

[R56] 远程拷贝
来源：http://vnr.yuxming.cn

scp file user@host:/path/
来源：http://dsy.fanxiaobao.xyz

[R57] 远程执行命令
来源：http://kqy.wangshuangyany.cn

ssh user@host 'uptime'
来源：http://bxh.shzxlz.cn

[R58] 下载文件
来源：http://hgm.c1oappe.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gxt.meibo888.top

[R59] 发 POST JSON
来源：http://xaf.yfazqb.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jar.xinyue.icu

[R60] 只看 HTTP 状态码
来源：http://zpz.sxryk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ust.guannengcc.top

[R61] 磁盘占用
来源：http://ufv.shanyushiyangkeji.top

df -h;  du -sh *
来源：http://ooo.9152youxi.cn

[R62] 找最占空间的文件
来源：http://hcm.redwolf501.top

du -ah . | sort -rh | head -10
来源：http://zhm.0kj1m.cn

[R63] 内存与进程
来源：http://gjr.aibaodan.cn

free -h;  ps aux | grep nginx
来源：http://och.yangfankeji.com

[R64] 结束进程
来源：http://vxy.yueranfly.top

kill -9 $(pgrep -f app.py)
来源：http://adi.feifeiyinyue.top

[R65] 查看端口占用
来源：http://tze.yangfankeji.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jop.zdbjq.cn

[R66] 定时任务
来源：http://wka.cdnleiting.top

crontab -e;  crontab -l
来源：http://ivt.epnwcf.com

[R67] 生成随机十六进制串
来源：http://tyn.hammf.cn

openssl rand -hex 16
来源：http://aur.shzxlz.cn

[R68] 计算文件校验值
来源：http://eyz.yj20258888.top

sha256sum a.txt;  md5sum a.txt
来源：http://ulk.shzxlz.cn

[R69] 生成随机密码
来源：http://zze.daria6918.cn

head -c 16 /dev/urandom | base64
来源：http://mxp.chenjidiqi.icu

[R70] 时间戳与互转
来源：http://uqt.sufxvd.cn

date +%s;  date -d @1700000000
来源：http://hmu.zhijiandao.cn

[R71] 日期格式化
来源：http://bxs.yj20258888.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xsk.jinqigfzy.top

[R72] 等待端口就绪
来源：http://pny.cucudq.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vtv.zycfv.cn

[R73] 分割大日志
来源：http://rrt.yj20258.top

split -l 1000 big.log part_
来源：http://npt.yj202588.top

[R74] 批量重命名
来源：http://eqi.sxryk.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hli.tian-w.cn

[R75] 导出环境变量
来源：http://ogc.chenlongwang.top

export PATH="$HOME/bin:$PATH"
来源：http://pcl.kuanghao11.cn

[R76] 使用临时文件
来源：http://wae.chenzaomai.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tox.ivvv.top

[R77] 读取用户输入
来源：http://lvg.ydjk.org.cn

read -rp "请输入: " ans
来源：http://wej.sxryk.cn

[R78] 交互式菜单
来源：http://zol.vqdsnc.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://moe.shuidangran.top

[R79] 解析命令行选项
来源：http://hja.zycfv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mgx.feifeiyinyue.top

[R80] 查看脚本执行耗时
来源：http://vdc.xingfuxueyuan.xyz

time ./run.sh
来源：http://box.fehbvm.com

================================================================================
来源：http://fzt.hysaishi.cn

S. C / C++ 专题
来源：http://hti.c1oappe.top

================================================================================
来源：http://xwq.cdnleiting.top

[S01] C：Hello World
来源：http://ltc.quarkkingdee.top

#include <stdio.h>
来源：http://tcf.feifeiyinyue.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://fdd.shanyushiyangkeji.top

[S02] C：变量与格式化输出
来源：http://qgb.0kj1m.cn

int a = 10; printf("%d\n", a);
来源：http://ige.mhx1999.top

[S03] C：读入整数
来源：http://msw.cashguo.top

int x; scanf("%d", &x);
来源：http://sxa.shuidangran.top

[S04] C：字符串复制
来源：http://qpu.jinyuanbaomall.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dly.fzhhl.top

[S05] C：字符串长度
来源：http://kgl.hnqzz.top

strlen(s)
来源：http://cnu.sjlbkw.cn

[S06] C：字符串比较
来源：http://ufn.gaohongyu789.top

strcmp(a, b) == 0
来源：http://ogl.sufxvd.cn

[S07] C：数组遍历求和
来源：http://qdk.yfazqb.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zle.daria6918.cn

[S08] C：动态内存分配与释放
来源：http://yuf.9152youxi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qtb.chenzaomai.com

[S09] C：结构体定义与初始化
来源：http://syf.epnwcf.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cpu.fehbvm.com

[S10] C：指针与解引用
来源：http://aha.jqgufenzy.top

int *p = &a;  *p = 5;
来源：http://sfe.gotoacloud.top

[S11] C：逐行读文件
来源：http://mrq.dashuyun.cn

FILE *f = fopen("a.txt", "r");
来源：http://qet.ydjk.org.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wou.snrcjt.cn

fclose(f);
来源：http://cmd.tian-w.cn

[S12] C：写文件
来源：http://xzw.hnqzz.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vzx.yuxming.cn

[S13] C：宏定义
来源：http://sig.yuanzhike.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rxa.birdmap.top

[S14] C：枚举
来源：http://wid.zycfv.cn

enum Color { RED, GREEN, BLUE };
来源：http://ujw.haohaochexian.top

[S15] C：类型转换
来源：http://hoj.gzhubu.top

(double) a / b
来源：http://kxx.cucudq.cn

[S16] C：位操作置位
来源：http://dqp.vqdsnc.cn

x |= (1 << 3);
来源：http://wsd.gogol.net.cn

[S17] C：安全拼接字符串
来源：http://okl.shuidangran.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://asu.gaohongyu789.top

[S18] C：命令行参数
来源：http://ice.hysaishi.cn

int main(int argc, char **argv)
来源：http://xso.iojbl.cn

[S19] C：快速排序
来源：http://aui.ppjwa.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ejt.yonumen.top

[S20] C：二分查找
来源：http://nko.zdbjq.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://syk.zdqjudy.top

[S21] C：字符类别判断
来源：http://upl.gogol.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bun.ctjpmb.com

[S22] C：字符串转数字
来源：http://qze.52xcode.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xir.shangyingyoupin.top

[S23] C：随机数
来源：http://hgi.jinqigufen.top

srand(time(NULL));  int r = rand() % 100;
来源：http://sec.havefunace.top

[S24] C：获取本地时间
来源：http://eoq.zycfv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mvr.52xcode.cn

[S25] C：内存拷贝
来源：http://yxg.jianghu66.top

memcpy(dst, src, n);
来源：http://ose.yuanzhike.top

[S26] C：内存清零
来源：http://vdb.guowangkeji.top

memset(a, 0, sizeof a);
来源：http://rct.jinqigfzy.top

[S27] C：定义常量
来源：http://vho.guowangkeji.top

const double PI = 3.14159;
来源：http://ohv.smart0.xyz

[S28] C：静态变量
来源：http://qas.c1oappe.top

static int counter = 0;
来源：http://faq.fengsongda.top

[S29] C：变参函数
来源：http://ufu.gzhubu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xpu.ydjk.org.cn

[S30] C：头文件保护
来源：http://qhk.zhijiandao.cn

#ifndef X_H
来源：http://ksz.jianghu66.top

#define X_H
来源：http://rlc.gzhubu.top

#endif
来源：http://ino.zhixingplan.top

[S31] C++：Hello World
来源：http://ssj.shuidangran.top

#include <iostream>
来源：http://idh.sweek.top

int main() { std::cout << "Hello\n"; }
来源：http://fvr.jiagoushi.top

[S32] C++：字符串
来源：http://dwj.dianchejie.cn

std::string s = "hi";  s += "!";
来源：http://xgh.52xcode.cn

[S33] C++：vector 增删
来源：http://iti.zhengqikj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://scq.hfpthk.cn

[S34] C++：遍历 vector
来源：http://xuq.xuanzx.com

for (auto &x : v) { std::cout << x; }
来源：http://xtp.yangfankeji.com

[S35] C++：map
来源：http://syp.hfpthk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zpr.epnwcf.com

[S36] C++：unordered_map
来源：http://eyo.nanxinkj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jyh.snrcjt.cn

[S37] C++：set
来源：http://pal.jianghu66.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mwn.hnxiangtu.top

[S38] C++：排序
来源：http://euc.sysykeji.top

std::sort(v.begin(), v.end());
来源：http://lgv.jqgfzy.top

[S39] C++：自定义比较器排序
来源：http://mqb.hcnkem.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bmq.cqqwz.cn

[S40] C++：查找元素
来源：http://odm.yfazqb.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ahz.52xcode.cn

[S41] C++：类与构造函数
来源：http://dwe.fanxiaobao.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vyw.havefunace.top

[S42] C++：继承与虚函数
来源：http://rzy.daxiang520.top

class B : public Base { public: void f() override {} };
来源：http://qoo.yj202588.top

[S43] C++：智能指针
来源：http://dce.svipenyu.cn

auto p = std::make_unique<int>(5);
来源：http://hof.xuetiantiany.cn

[S44] C++：引用传参
来源：http://xze.cheryme.top

void inc(int &x) { ++x; }
来源：http://qkb.ydjk.org.cn

[S45] C++：lambda
来源：http://xlw.yuanzhike.top

auto add = [](int a, int b) { return a + b; };
来源：http://xnw.dashuyun.cn

[S46] C++：函数模板
来源：http://sfa.hnqzz.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jtb.mhx1999.top

[S47] C++：结构化绑定遍历
来源：http://cru.yuanzhike.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ito.sufxvd.cn

[S48] C++：逐行读文件
来源：http://jkz.jianghu66.top

std::ifstream in("a.txt");  std::string line;
来源：http://mpg.xuanzx.com

while (std::getline(in, line)) { }
来源：http://ltl.daria6918.cn

[S49] C++：写文件
来源：http://tus.smart0.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ibg.hysaishi.cn

[S50] C++：格式化数字
来源：http://yxr.tanke756.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ezt.svipenyu.cn

[S51] C++：显式类型转换
来源：http://ufu.yangfankeji.com

static_cast<double>(a) / b
来源：http://yzf.hammf.cn

[S52] C++：const 与 noexcept
来源：http://yoj.yvedp.cn

int size() const noexcept { return n_; }
来源：http://xco.tian-w.cn

[S53] C++：移动语义
来源：http://bnr.sysykeji.top

std::vector<int> w = std::move(v);
来源：http://qos.meibo888.top

[S54] C++：异常处理
来源：http://tao.xziqi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wks.ydjk.org.cn

[S55] C++：结构化绑定
来源：http://jkd.cheryme.top

auto [a, b] = std::make_pair(1, 2);
来源：http://wpp.guannengcc.top

[S56] C++：optional
来源：http://smh.yongpay.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://unu.zycfv.cn

[S57] C++：编译期常量
来源：http://fzv.jinqigufen.top

constexpr int N = 10;
来源：http://efc.c1oappe.top

[S58] C++：命名空间
来源：http://pmw.tanke756.top

namespace ns { int f() { return 1; } }
来源：http://aft.zhengqikj.top

[S59] C++：静态断言
来源：http://kdi.tanke756.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fzr.ybcxt.top

[S60] C++：遍历并删除元素
来源：http://zhl.iojbl.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://urr.zhijiandao.cn

================================================================================
来源：http://atb.vqdsnc.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zeo.shanyushiyangkeji.top

================================================================================
来源：http://kka.c1oappe.top

[T01] Kotlin：Hello World
来源：http://gvh.yueranfly.top

println("Hello")
来源：http://udz.yueranfly.top

[T02] Kotlin：变量
来源：http://hko.yangfankeji.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ckg.ctjpmb.com

[T03] Kotlin：字符串模板
来源：http://sbk.uphjek.com

"值: $b"
来源：http://iic.hnxiangtu.top

[T04] Kotlin：空安全
来源：http://bfd.hesvh.cn

val n: String? = null;  n?.length
来源：http://uva.316326.xyz

[T05] Kotlin：when 表达式
来源：http://wlr.xingfuxueyuan.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://grf.jqgfzy.top

[T06] Kotlin：集合映射
来源：http://coj.yonumen.top

listOf(1, 2, 3).map { it * 2 }
来源：http://fbq.shangyingyoupin.top

[T07] Kotlin：集合过滤
来源：http://ula.chenzaomai.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://rkq.cucudq.cn

[T08] Kotlin：数据类
来源：http://uhp.zhongyouzk.top

data class User(val name: String, val age: Int)
来源：http://aip.tianlin.xyz

[T09] Kotlin：扩展函数
来源：http://nfg.tanke756.top

fun String.exclaim() = this + "!"
来源：http://cbv.chenlongwang.top

[T10] Kotlin：默认参数
来源：http://nrp.havefunace.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nia.yuxming.cn

[T11] Kotlin：协程
来源：http://yje.gotoacloud.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://zyl.cheryme.top

[T12] Kotlin：解构声明
来源：http://sxk.shangyingyoupin.top

val (a, b) = Pair(1, 2)
来源：http://kjw.yonumen.top

[T13] Kotlin：只读 Map
来源：http://xlu.fengsongda.top

val m = mapOf("a" to 1)
来源：http://uws.yanxiufei.cn

[T14] Kotlin：循环
来源：http://xyt.ywan-chungtsiang.top

for (i in 1..10) println(i)
来源：http://ony.fzhhl.top


<!-- 参考信息 -->