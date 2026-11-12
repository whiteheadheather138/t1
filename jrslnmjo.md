代发 wailian999

esac
来源：http://xux.yfazqb.com

[R12] for 遍历文件
来源：http://lst.xziqi.cn

for f in *.txt; do echo "$f"; done
来源：http://dfi.xylfe.cn

[R13] for 计数循环
来源：http://rnh.nanxuanxn.top

for i in {1..10}; do echo "$i"; done
来源：http://slu.fanxiaobao.xyz

[R14] C 风格 for
来源：http://fmn.cucudq.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sao.zhongyouzk.top

[R15] while 逐行读文件
来源：http://lva.aizwys.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ppf.vehdjk.com

[R16] until 等待条件
来源：http://dlr.quarkkingdee.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xzq.wangdashe.top

[R17] 数组定义与取值
来源：http://qle.jyoumei.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kwa.gzhubu.top

[R18] 遍历数组
来源：http://axv.quarkkingdee.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uny.jinyuanbaomall.cn

[R19] 数组长度
来源：http://uhs.vqdsnc.cn

echo "${#arr[@]}"
来源：http://dbd.zhijiandao.cn

[R20] 关联数组（字典）
来源：http://wnr.chenzaomai.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zob.yj20258.top

[R21] 字符串长度
来源：http://gpo.birdmap.top

echo "${#s}"
来源：http://urx.birdmap.top

[R22] 截取子串
来源：http://jki.sysykeji.top

echo "${s:0:5}"
来源：http://lwx.hywenlv.cn

[R23] 字符串替换
来源：http://tvv.316326.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lus.xylfe.cn

[R24] 大小写转换
来源：http://mao.ctjpmb.com

echo "${s^^}"; echo "${s,,}"
来源：http://usr.xuetiantiany.cn

[R25] 去后缀 / 去前缀
来源：http://vga.dianchejie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ryh.yangfankeji.com

[R26] 命令替换
来源：http://hoh.jyoumei.cn

now=$(date +%F); echo "$now"
来源：http://wcz.vqdsnc.cn

[R27] 算术展开
来源：http://ewe.gogol.net.cn

echo $((1 + 2 * 3))
来源：http://txs.feifeiyinyue.top

[R28] 浮点运算
来源：http://quu.52xcode.cn

echo "scale=2; 10/3" | bc
来源：http://ngq.dianchejie.cn

[R29] 定义函数
来源：http://ori.chenjidiqi.icu

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mlq.hongshengwenyu.top

[R30] 函数返回状态码
来源：http://dgl.fzhhl.top

f() { return 0; }; f || echo "失败了"
来源：http://cjf.iojbl.cn

[R31] 局部变量
来源：http://psf.svipenyu.cn

f() { local x=1; echo "$x"; }
来源：http://yrq.sjlbkw.cn

[R32] 参数个数校验
来源：http://sey.9152youxi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dmw.pycfn.com

[R33] 捕获错误并提示行号
来源：http://kac.chenzaomai.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kng.guowangkeji.top

[R34] 退出时清理
来源：http://yra.zhongyouzk.top

trap 'rm -f "$tmp"' EXIT
来源：http://fvf.bjfxy.top

[R35] 后台执行并等待
来源：http://vfu.fanxiaobao.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://mpw.nwbrower.top

[R36] 并发执行多个任务
来源：http://qzy.fktsv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dlc.xuetiantiany.cn

[R37] 把输出赋给变量
来源：http://grq.fanxiaobao.xyz

files=$(ls -1)
来源：http://uwi.316326.xyz

[R38] 管道串联
来源：http://kpb.ctjpmb.com

cat a.txt | grep -i error | wc -l
来源：http://hgz.gogol.net.cn

[R39] 重定向标准输出与错误
来源：http://man.birdmap.top

cmd > out.log 2>&1
来源：http://bmu.mhx1999.top

[R40] 追加写日志
来源：http://xxa.dashuyun.cn

echo "log" >> out.log
来源：http://lxb.chenlongwang.top

[R41] 丢弃输出
来源：http://vag.pengpengdd.cyou

cmd >/dev/null 2>&1
来源：http://qfs.hysaishi.cn

[R42] 输入重定向
来源：http://mhv.yj202588.top

wc -l < a.txt
来源：http://fan.nwbrower.top

[R43] 按名字查找文件
来源：http://bol.yfazqb.com

find . -name "*.log" -type f
来源：http://jou.xinyue.icu

[R44] 按修改时间查找
来源：http://bih.epnwcf.com

find . -mtime -7 -type f
来源：http://zlz.sufxvd.cn

[R45] 批量删除
来源：http://oyy.haohaochexian.top

find . -name "*.tmp" -delete
来源：http://lsp.nwbrower.top

[R46] 递归替换文件内容
来源：http://lrg.hesvh.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ppj.ehwqpu.com

[R47] sed 单行替换
来源：http://rxf.kuanghao11.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ylb.c1oappe.top

[R48] awk 取指定列
来源：http://yjr.yj20258.top

awk '{print $1, $3}' a.txt
来源：http://xre.jqgufenzy.top

[R49] awk 带条件
来源：http://lqp.hywenlv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gmn.hongshengwenyu.top

[R50] awk 求和
来源：http://sdz.haohaochexian.top

awk '{s += $2} END {print s}' a.txt
来源：http://sjg.ehwqpu.com

[R51] 排序去重取前几
来源：http://yhy.pengpengdd.cyou

sort a.txt | uniq -c | sort -rn | head
来源：http://tzh.zycfv.cn

[R52] 统计行数
来源：http://csr.smart0.xyz

wc -l a.txt
来源：http://thz.nanxuanxn.top

[R53] 查看文件头与实时尾
来源：http://gfb.nanxuanxn.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ids.jianghu66.top

[R54] 比较两个文件
来源：http://emy.nwbrower.top

diff a.txt b.txt
来源：http://efo.sufxvd.cn

[R55] 压缩与解压
来源：http://zxt.havefunace.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jsv.ctjpmb.com

[R56] 远程拷贝
来源：http://eyo.pengpengdd.cyou

scp file user@host:/path/
来源：http://bib.vqdsnc.cn

[R57] 远程执行命令
来源：http://cbq.gogol.net.cn

ssh user@host 'uptime'
来源：http://sco.cqqwz.cn

[R58] 下载文件
来源：http://pkw.havefunace.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bwt.mhx1999.top

[R59] 发 POST JSON
来源：http://lot.yj20258.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://loc.shanyushiyangtech.top

[R60] 只看 HTTP 状态码
来源：http://krm.xuetiantiany.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qtx.fktsv.cn

[R61] 磁盘占用
来源：http://qmu.snrcjt.cn

df -h;  du -sh *
来源：http://wyh.jqgufenzy.top

[R62] 找最占空间的文件
来源：http://tyy.cucudq.cn

du -ah . | sort -rh | head -10
来源：http://xtm.uphjek.com

[R63] 内存与进程
来源：http://jgq.yj202588.top

free -h;  ps aux | grep nginx
来源：http://hvn.jinyuanbaomall.cn

[R64] 结束进程
来源：http://bdm.jyoumei.cn

kill -9 $(pgrep -f app.py)
来源：http://gfy.jqgfzy.top

[R65] 查看端口占用
来源：http://jmw.yueranfly.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yum.xylfe.cn

[R66] 定时任务
来源：http://hmj.yuanzhike.top

crontab -e;  crontab -l
来源：http://fgg.hnxiangtu.top

[R67] 生成随机十六进制串
来源：http://dnd.haohaochexian.top

openssl rand -hex 16
来源：http://ktr.zycfv.cn

[R68] 计算文件校验值
来源：http://rir.yj202588.top

sha256sum a.txt;  md5sum a.txt
来源：http://wdd.ivvv.top

[R69] 生成随机密码
来源：http://cyl.zhaomingkeji.xyz

head -c 16 /dev/urandom | base64
来源：http://zlr.epnwcf.com

[R70] 时间戳与互转
来源：http://ywz.uphjek.com

date +%s;  date -d @1700000000
来源：http://mwr.nanxuanxn.top

[R71] 日期格式化
来源：http://oio.jinghuilouyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://pig.tianlin.xyz

[R72] 等待端口就绪
来源：http://dqp.zhiwuduotai.top

until nc -z localhost 3306; do sleep 1; done
来源：http://njq.iojbl.cn

[R73] 分割大日志
来源：http://hhh.xylfe.cn

split -l 1000 big.log part_
来源：http://oce.sufxvd.cn

[R74] 批量重命名
来源：http://bww.shuidangran.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ibf.mhx1999.top

[R75] 导出环境变量
来源：http://uyd.fktsv.cn

export PATH="$HOME/bin:$PATH"
来源：http://dmu.jlsjyb.cn

[R76] 使用临时文件
来源：http://hei.shanyushiyangtech.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wmw.shanyushiyangtech.top

[R77] 读取用户输入
来源：http://byv.zdbjq.cn

read -rp "请输入: " ans
来源：http://pgs.redwolf501.top

[R78] 交互式菜单
来源：http://ywm.jinyuanbaomall.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nwy.nwbrower.top

[R79] 解析命令行选项
来源：http://nuk.zhijiandao.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lzj.sxryk.cn

[R80] 查看脚本执行耗时
来源：http://gbg.fanxiaobao.xyz

time ./run.sh
来源：http://tek.aibaodan.cn

================================================================================
来源：http://ccg.xziqi.cn

S. C / C++ 专题
来源：http://dwm.guannengcc.top

================================================================================
来源：http://bpp.zhengqikj.top

[S01] C：Hello World
来源：http://nox.9152youxi.cn

#include <stdio.h>
来源：http://laj.daxiang520.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://uqa.svipenyu.cn

[S02] C：变量与格式化输出
来源：http://yyx.nwbrower.top

int a = 10; printf("%d\n", a);
来源：http://uuk.cashguo.top

[S03] C：读入整数
来源：http://cwt.shanyushiyangkeji.top

int x; scanf("%d", &x);
来源：http://yyb.cqqwz.cn

[S04] C：字符串复制
来源：http://zbf.chenjidiqi.icu

char dst[32]; strcpy(dst, "hi");
来源：http://vxd.c1oappe.top

[S05] C：字符串长度
来源：http://cvj.hnqzz.top

strlen(s)
来源：http://djl.andypj.xyz

[S06] C：字符串比较
来源：http://eiz.shzxlz.cn

strcmp(a, b) == 0
来源：http://rdc.zdbjq.cn

[S07] C：数组遍历求和
来源：http://bzd.mhx1999.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gop.yueranfly.top

[S08] C：动态内存分配与释放
来源：http://zld.jinqigfzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tta.snrcjt.cn

[S09] C：结构体定义与初始化
来源：http://baq.meibo888.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wna.pycfn.com

[S10] C：指针与解引用
来源：http://vme.c1oappe.top

int *p = &a;  *p = 5;
来源：http://oea.vehdjk.com

[S11] C：逐行读文件
来源：http://jub.shuidangran.top

FILE *f = fopen("a.txt", "r");
来源：http://wxm.ywan-chungtsiang.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://pba.shanyushiyangkeji.top

fclose(f);
来源：http://zli.pycfn.com

[S12] C：写文件
来源：http://gla.wangdashe.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vtb.sufxvd.cn

[S13] C：宏定义
来源：http://xnx.jiagoushi.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pyo.0kj1m.cn

[S14] C：枚举
来源：http://lth.zdqjudy.top

enum Color { RED, GREEN, BLUE };
来源：http://ayz.ybcxt.top

[S15] C：类型转换
来源：http://kmy.kuanghao11.cn

(double) a / b
来源：http://jnv.zhixingplan.top

[S16] C：位操作置位
来源：http://jrg.yj202588.top

x |= (1 << 3);
来源：http://wgd.chenzaomai.com

[S17] C：安全拼接字符串
来源：http://dot.snrcjt.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vul.guowangkeji.top

[S18] C：命令行参数
来源：http://ksq.gogol.net.cn

int main(int argc, char **argv)
来源：http://axt.hysaishi.cn

[S19] C：快速排序
来源：http://vki.xziqi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nal.dashuyun.cn

[S20] C：二分查找
来源：http://llq.dianchejie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vrw.xinyue.icu

[S21] C：字符类别判断
来源：http://okb.zhaomingkeji.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cze.feifeiyinyue.top

[S22] C：字符串转数字
来源：http://pcb.zhixingplan.top

atoi("42");  strtod("3.14", NULL);
来源：http://lgp.shzxlz.cn

[S23] C：随机数
来源：http://wit.redwolf501.top

srand(time(NULL));  int r = rand() % 100;
来源：http://afg.hfpthk.cn

[S24] C：获取本地时间
来源：http://yoa.yfazqb.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hjt.jqgfzy.top

[S25] C：内存拷贝
来源：http://eqk.tianlin.xyz

memcpy(dst, src, n);
来源：http://uon.cashguo.top

[S26] C：内存清零
来源：http://esx.pengpengdd.cyou

memset(a, 0, sizeof a);
来源：http://gpk.hongshengwenyu.top

[S27] C：定义常量
来源：http://ocq.jyoumei.cn

const double PI = 3.14159;
来源：http://ero.jinqigufen.top

[S28] C：静态变量
来源：http://igm.jinqigfzy.top

static int counter = 0;
来源：http://xwx.shuidangran.top

[S29] C：变参函数
来源：http://wcq.kuanghao11.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oqf.hnxiangtu.top

[S30] C：头文件保护
来源：http://kvs.yangfankeji.com

#ifndef X_H
来源：http://qkv.jiagoushi.top

#define X_H
来源：http://ikk.chenlongwang.top

#endif
来源：http://bpv.shangyingyoupin.top

[S31] C++：Hello World
来源：http://sxu.ctjpmb.com

#include <iostream>
来源：http://aly.wangshuangyany.cn

int main() { std::cout << "Hello\n"; }
来源：http://rxp.vehdjk.com

[S32] C++：字符串
来源：http://afc.sysykeji.top

std::string s = "hi";  s += "!";
来源：http://miy.chenjidiqi.icu

[S33] C++：vector 增删
来源：http://tst.hammf.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ryz.jinqigufen.top

[S34] C++：遍历 vector
来源：http://jvd.yj202588.top

for (auto &x : v) { std::cout << x; }
来源：http://xmf.hfpthk.cn

[S35] C++：map
来源：http://fzb.pengpengdd.cyou

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lvo.jinqigfzy.top

[S36] C++：unordered_map
来源：http://kbj.zdqjudy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://feh.cheryme.top

[S37] C++：set
来源：http://jak.dianchejie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lze.zhijiandao.cn

[S38] C++：排序
来源：http://laf.sweek.top

std::sort(v.begin(), v.end());
来源：http://byr.bjfxy.top

[S39] C++：自定义比较器排序
来源：http://atp.jianghu66.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hbm.redwolf501.top

[S40] C++：查找元素
来源：http://wsc.daxiang520.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fyx.jyoumei.cn

[S41] C++：类与构造函数
来源：http://byn.yanxiufei.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wea.zhiwuduotai.top

[S42] C++：继承与虚函数
来源：http://src.yonumen.top

class B : public Base { public: void f() override {} };
来源：http://enc.meibo888.top

[S43] C++：智能指针
来源：http://qav.cqqwz.cn

auto p = std::make_unique<int>(5);
来源：http://cwj.gzhubu.top

[S44] C++：引用传参
来源：http://rts.tianlin.xyz

void inc(int &x) { ++x; }
来源：http://akq.gogol.net.cn

[S45] C++：lambda
来源：http://okg.hesvh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qsp.aibaodan.cn

[S46] C++：函数模板
来源：http://aqi.tanke756.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fxj.fehbvm.com

[S47] C++：结构化绑定遍历
来源：http://ucb.fktsv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://doc.52xcode.cn

[S48] C++：逐行读文件
来源：http://daj.52xcode.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vke.guannengcc.top

while (std::getline(in, line)) { }
来源：http://bjv.yanxiufei.cn

[S49] C++：写文件
来源：http://knm.vqdsnc.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yxv.uphjek.com

[S50] C++：格式化数字
来源：http://egp.wangdashe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://trc.hnqzz.top

[S51] C++：显式类型转换
来源：http://xcj.9152youxi.cn

static_cast<double>(a) / b
来源：http://qis.yueranfly.top

[S52] C++：const 与 noexcept
来源：http://wjj.ivvv.top

int size() const noexcept { return n_; }
来源：http://dmt.uphjek.com

[S53] C++：移动语义
来源：http://soa.smart0.xyz

std::vector<int> w = std::move(v);
来源：http://ndd.uphjek.com

[S54] C++：异常处理
来源：http://qid.gogol.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ouo.tianlin.xyz

[S55] C++：结构化绑定
来源：http://vnp.dianchejie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zib.guannengcc.top

[S56] C++：optional
来源：http://gde.jqgufenzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kvs.zhiwuduotai.top

[S57] C++：编译期常量
来源：http://aom.316326.xyz

constexpr int N = 10;
来源：http://zdk.shanyushiyangkeji.top

[S58] C++：命名空间
来源：http://ver.fktsv.cn

namespace ns { int f() { return 1; } }
来源：http://jhe.fanxiaobao.xyz

[S59] C++：静态断言
来源：http://xlx.jinghuilouyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zey.wangdashe.top

[S60] C++：遍历并删除元素
来源：http://son.ctjpmb.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hcz.wangdashe.top

================================================================================
来源：http://iwr.sxryk.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yck.fktsv.cn

================================================================================
来源：http://szz.tarul.cn

[T01] Kotlin：Hello World
来源：http://wee.fzhhl.top

println("Hello")
来源：http://uix.kuanghao11.cn

[T02] Kotlin：变量
来源：http://ydv.vqdsnc.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://luw.0kj1m.cn

[T03] Kotlin：字符串模板
来源：http://isj.vqdsnc.cn

"值: $b"
来源：http://tpk.redwolf501.top

[T04] Kotlin：空安全
来源：http://spf.shanyushiyangtech.top

val n: String? = null;  n?.length
来源：http://lpw.gotoacloud.top

[T05] Kotlin：when 表达式
来源：http://ggu.sxryk.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yqf.sufxvd.cn

[T06] Kotlin：集合映射
来源：http://mcc.tarul.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://iwn.chenlongwang.top

[T07] Kotlin：集合过滤
来源：http://gpb.xylfe.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://erv.zhongyouzk.top

[T08] Kotlin：数据类
来源：http://zce.cucudq.cn

data class User(val name: String, val age: Int)
来源：http://joo.wangdashe.top

[T09] Kotlin：扩展函数
来源：http://tgu.zhongyouzk.top

fun String.exclaim() = this + "!"
来源：http://sbm.316326.xyz

[T10] Kotlin：默认参数
来源：http://ssa.xingfuxueyuan.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://nzc.svipenyu.cn

[T11] Kotlin：协程
来源：http://mzs.jyoumei.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://upv.jinqigufen.top

[T12] Kotlin：解构声明
来源：http://tpd.hysaishi.cn

val (a, b) = Pair(1, 2)
来源：http://zzm.yvedp.cn

[T13] Kotlin：只读 Map
来源：http://dyu.shzxlz.cn

val m = mapOf("a" to 1)
来源：http://jop.sysykeji.top

[T14] Kotlin：循环
来源：http://gmy.yuxming.cn

for (i in 1..10) println(i)
来源：http://igr.vqdsnc.cn


<!-- 参考信息 -->