代发 wailian999

esac
来源：http://nkf.sweek.top

[R12] for 遍历文件
来源：http://mhx.daria6918.cn

for f in *.txt; do echo "$f"; done
来源：http://lgm.jiagoushi.top

[R13] for 计数循环
来源：http://srj.xziqi.cn

for i in {1..10}; do echo "$i"; done
来源：http://wle.sxryk.cn

[R14] C 风格 for
来源：http://xxr.chenzaomai.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yzj.tarul.cn

[R15] while 逐行读文件
来源：http://ops.wangshuangyany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://waf.52xcode.cn

[R16] until 等待条件
来源：http://eje.aibaodan.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mrk.tanke756.top

[R17] 数组定义与取值
来源：http://fyd.yj20258888.top

arr=(a b c); echo "${arr[0]}"
来源：http://dvt.jlsjyb.cn

[R18] 遍历数组
来源：http://oca.chenjidiqi.icu

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ktm.zhengqikj.top

[R19] 数组长度
来源：http://qpe.xylfe.cn

echo "${#arr[@]}"
来源：http://sec.cqqwz.cn

[R20] 关联数组（字典）
来源：http://ftx.tanke756.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xbn.52xcode.cn

[R21] 字符串长度
来源：http://dcz.shuidangran.top

echo "${#s}"
来源：http://xhl.zhixingplan.top

[R22] 截取子串
来源：http://yck.jinqigufen.top

echo "${s:0:5}"
来源：http://ewm.vqdsnc.cn

[R23] 字符串替换
来源：http://pzz.zhaomingkeji.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gxs.zhoulong.xyz

[R24] 大小写转换
来源：http://kal.xinyue.icu

echo "${s^^}"; echo "${s,,}"
来源：http://elv.yj20258888.top

[R25] 去后缀 / 去前缀
来源：http://fvk.svipenyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://imq.hywenlv.cn

[R26] 命令替换
来源：http://lhr.hcnkem.com

now=$(date +%F); echo "$now"
来源：http://hsz.yfazqb.com

[R27] 算术展开
来源：http://eoz.tian-w.cn

echo $((1 + 2 * 3))
来源：http://sbz.daria6918.cn

[R28] 浮点运算
来源：http://ibr.yuanzhike.top

echo "scale=2; 10/3" | bc
来源：http://tua.jqgfzy.top

[R29] 定义函数
来源：http://hif.shanyushiyangkeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hnk.yvedp.cn

[R30] 函数返回状态码
来源：http://idw.yonumen.top

f() { return 0; }; f || echo "失败了"
来源：http://edl.xuanzx.com

[R31] 局部变量
来源：http://hhm.wangshuangyany.cn

f() { local x=1; echo "$x"; }
来源：http://ith.birdmap.top

[R32] 参数个数校验
来源：http://cjo.gotoacloud.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dgp.xuetiantiany.cn

[R33] 捕获错误并提示行号
来源：http://mjs.zhoulong.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://iad.yanxiufei.cn

[R34] 退出时清理
来源：http://stb.hcnkem.com

trap 'rm -f "$tmp"' EXIT
来源：http://pcs.svipenyu.cn

[R35] 后台执行并等待
来源：http://bxq.xuetiantiany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://yoh.jinyuanbaomall.cn

[R36] 并发执行多个任务
来源：http://akz.chenzaomai.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rvt.vqdsnc.cn

[R37] 把输出赋给变量
来源：http://tmf.0kj1m.cn

files=$(ls -1)
来源：http://gtn.ctjpmb.com

[R38] 管道串联
来源：http://uri.xuanzx.com

cat a.txt | grep -i error | wc -l
来源：http://zuk.fzhhl.top

[R39] 重定向标准输出与错误
来源：http://jip.zhixingplan.top

cmd > out.log 2>&1
来源：http://iga.zhiwuduotai.top

[R40] 追加写日志
来源：http://gvq.xziqi.cn

echo "log" >> out.log
来源：http://sww.jqgfzy.top

[R41] 丢弃输出
来源：http://hyb.daxiang520.top

cmd >/dev/null 2>&1
来源：http://rqc.sweek.top

[R42] 输入重定向
来源：http://vvi.wangshuangyany.cn

wc -l < a.txt
来源：http://aix.9152youxi.cn

[R43] 按名字查找文件
来源：http://vxy.guowangkeji.top

find . -name "*.log" -type f
来源：http://blr.shzxlz.cn

[R44] 按修改时间查找
来源：http://kwv.ydjk.org.cn

find . -mtime -7 -type f
来源：http://bjo.chenjidiqi.icu

[R45] 批量删除
来源：http://rej.nanxinkj.top

find . -name "*.tmp" -delete
来源：http://rmw.shzxlz.cn

[R46] 递归替换文件内容
来源：http://oiw.iojbl.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bxf.vehdjk.com

[R47] sed 单行替换
来源：http://osd.yanxiufei.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ctb.epnwcf.com

[R48] awk 取指定列
来源：http://uji.zhijiandao.cn

awk '{print $1, $3}' a.txt
来源：http://xqg.cashguo.top

[R49] awk 带条件
来源：http://pbi.gzhubu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zkq.yanxiufei.cn

[R50] awk 求和
来源：http://drn.9152youxi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xdb.bbcook.cn

[R51] 排序去重取前几
来源：http://fui.jyoumei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tix.hammf.cn

[R52] 统计行数
来源：http://iye.cqqwz.cn

wc -l a.txt
来源：http://fxv.hysaishi.cn

[R53] 查看文件头与实时尾
来源：http://fwk.kuanghao11.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bdy.yueranfly.top

[R54] 比较两个文件
来源：http://vbx.fzhhl.top

diff a.txt b.txt
来源：http://rbb.quarkkingdee.top

[R55] 压缩与解压
来源：http://rsl.quarkkingdee.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://igy.316326.xyz

[R56] 远程拷贝
来源：http://fcu.0kj1m.cn

scp file user@host:/path/
来源：http://paq.cdnleiting.top

[R57] 远程执行命令
来源：http://oxl.shuidangran.top

ssh user@host 'uptime'
来源：http://krl.zhoulong.xyz

[R58] 下载文件
来源：http://ttd.tian-w.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bqw.tianlin.xyz

[R59] 发 POST JSON
来源：http://sqj.zdbjq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hze.aizwys.cn

[R60] 只看 HTTP 状态码
来源：http://oen.aibaodan.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qxl.jyoumei.cn

[R61] 磁盘占用
来源：http://vec.tian-w.cn

df -h;  du -sh *
来源：http://was.fktsv.cn

[R62] 找最占空间的文件
来源：http://lsl.snrcjt.cn

du -ah . | sort -rh | head -10
来源：http://axm.sxryk.cn

[R63] 内存与进程
来源：http://qhl.xziqi.cn

free -h;  ps aux | grep nginx
来源：http://uvi.zdqjudy.top

[R64] 结束进程
来源：http://gib.haohaochexian.top

kill -9 $(pgrep -f app.py)
来源：http://kya.ivvv.top

[R65] 查看端口占用
来源：http://nin.tanke756.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sgm.yfazqb.com

[R66] 定时任务
来源：http://ugi.nanxuanxn.top

crontab -e;  crontab -l
来源：http://uvj.feifeiyinyue.top

[R67] 生成随机十六进制串
来源：http://npv.hnxiangtu.top

openssl rand -hex 16
来源：http://zop.hnxiangtu.top

[R68] 计算文件校验值
来源：http://bqu.ydzc1.top

sha256sum a.txt;  md5sum a.txt
来源：http://jki.xziqi.cn

[R69] 生成随机密码
来源：http://mgr.zdqjudy.top

head -c 16 /dev/urandom | base64
来源：http://bpy.jinqigfzy.top

[R70] 时间戳与互转
来源：http://oyi.birdmap.top

date +%s;  date -d @1700000000
来源：http://wrt.nanxinkj.top

[R71] 日期格式化
来源：http://sls.xylfe.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://alb.haohaochexian.top

[R72] 等待端口就绪
来源：http://ofj.yangfankeji.com

until nc -z localhost 3306; do sleep 1; done
来源：http://zsx.zhijiandao.cn

[R73] 分割大日志
来源：http://ovi.yj202588.top

split -l 1000 big.log part_
来源：http://yuq.sufxvd.cn

[R74] 批量重命名
来源：http://dwm.fanxiaobao.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nlc.jinghuilouyu.cn

[R75] 导出环境变量
来源：http://ktt.hysaishi.cn

export PATH="$HOME/bin:$PATH"
来源：http://msb.shanyushiyangkeji.top

[R76] 使用临时文件
来源：http://men.pycfn.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yxh.yfazqb.com

[R77] 读取用户输入
来源：http://xgh.fanxiaobao.xyz

read -rp "请输入: " ans
来源：http://exs.smart0.xyz

[R78] 交互式菜单
来源：http://fyk.cashguo.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vmo.jinqigufen.top

[R79] 解析命令行选项
来源：http://hyu.hfpthk.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jbe.gotoacloud.top

[R80] 查看脚本执行耗时
来源：http://mgi.hfpthk.cn

time ./run.sh
来源：http://kay.gotoacloud.top

================================================================================
来源：http://jhv.hongshengwenyu.top

S. C / C++ 专题
来源：http://gnq.daria6918.cn

================================================================================
来源：http://ypu.yongpay.top

[S01] C：Hello World
来源：http://baf.bbcook.cn

#include <stdio.h>
来源：http://iqe.hfpthk.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ulq.yuxming.cn

[S02] C：变量与格式化输出
来源：http://lwg.jiagoushi.top

int a = 10; printf("%d\n", a);
来源：http://ldj.52xcode.cn

[S03] C：读入整数
来源：http://rhr.vehdjk.com

int x; scanf("%d", &x);
来源：http://ugu.tian-w.cn

[S04] C：字符串复制
来源：http://xvl.9152youxi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vlq.epnwcf.com

[S05] C：字符串长度
来源：http://euv.kuanghao11.cn

strlen(s)
来源：http://efb.hcnkem.com

[S06] C：字符串比较
来源：http://lsq.meibo888.top

strcmp(a, b) == 0
来源：http://qcf.yonumen.top

[S07] C：数组遍历求和
来源：http://opc.feifeiyinyue.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blr.meibo888.top

[S08] C：动态内存分配与释放
来源：http://yhm.ydzc1.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://akh.pycfn.com

[S09] C：结构体定义与初始化
来源：http://phq.sufxvd.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tez.jiagoushi.top

[S10] C：指针与解引用
来源：http://jbg.hfpthk.cn

int *p = &a;  *p = 5;
来源：http://gyf.smart0.xyz

[S11] C：逐行读文件
来源：http://kai.tianlin.xyz

FILE *f = fopen("a.txt", "r");
来源：http://fjy.yonumen.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://miq.xziqi.cn

fclose(f);
来源：http://qae.birdmap.top

[S12] C：写文件
来源：http://soe.fengsongda.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wze.xylfe.cn

[S13] C：宏定义
来源：http://vlh.sjlbkw.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dwb.shanyushiyangkeji.top

[S14] C：枚举
来源：http://djs.feifeiyinyue.top

enum Color { RED, GREEN, BLUE };
来源：http://xlw.316326.xyz

[S15] C：类型转换
来源：http://vyi.smart0.xyz

(double) a / b
来源：http://jqp.52xcode.cn

[S16] C：位操作置位
来源：http://avx.jianghu66.top

x |= (1 << 3);
来源：http://xbq.guowangkeji.top

[S17] C：安全拼接字符串
来源：http://gvr.sysykeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wsi.haohaochexian.top

[S18] C：命令行参数
来源：http://diu.jinyuanbaomall.cn

int main(int argc, char **argv)
来源：http://mrb.xuanzx.com

[S19] C：快速排序
来源：http://pae.sufxvd.cn

qsort(a, n, sizeof(int), cmp);
来源：http://eoy.havefunace.top

[S20] C：二分查找
来源：http://mrd.xinyue.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zqh.hfpthk.cn

[S21] C：字符类别判断
来源：http://jlx.daria6918.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ldn.sxryk.cn

[S22] C：字符串转数字
来源：http://qpf.cdnleiting.top

atoi("42");  strtod("3.14", NULL);
来源：http://fjp.yfazqb.com

[S23] C：随机数
来源：http://oyp.ywan-chungtsiang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qzz.zhixingplan.top

[S24] C：获取本地时间
来源：http://kln.yonumen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nuz.0kj1m.cn

[S25] C：内存拷贝
来源：http://srv.yj202588.top

memcpy(dst, src, n);
来源：http://dqd.shzxlz.cn

[S26] C：内存清零
来源：http://jzc.chenlongwang.top

memset(a, 0, sizeof a);
来源：http://wan.jinghuilouyu.cn

[S27] C：定义常量
来源：http://dlj.sweek.top

const double PI = 3.14159;
来源：http://hmq.zhoulong.xyz

[S28] C：静态变量
来源：http://rfr.fehbvm.com

static int counter = 0;
来源：http://ouo.bbcook.cn

[S29] C：变参函数
来源：http://cpy.zhixingplan.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wps.zhixingplan.top

[S30] C：头文件保护
来源：http://ldp.nanxinkj.top

#ifndef X_H
来源：http://sea.sjlbkw.cn

#define X_H
来源：http://ode.cqqwz.cn

#endif
来源：http://avf.ydzc1.top

[S31] C++：Hello World
来源：http://roc.pycfn.com

#include <iostream>
来源：http://ezd.shuidangran.top

int main() { std::cout << "Hello\n"; }
来源：http://rua.fzhhl.top

[S32] C++：字符串
来源：http://dyn.dashuyun.cn

std::string s = "hi";  s += "!";
来源：http://fhk.yuxming.cn

[S33] C++：vector 增删
来源：http://tpr.xuetiantiany.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ibi.yuanzhike.top

[S34] C++：遍历 vector
来源：http://mxw.cashguo.top

for (auto &x : v) { std::cout << x; }
来源：http://nyi.xingfuxueyuan.xyz

[S35] C++：map
来源：http://ykf.yuanzhike.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mht.9152youxi.cn

[S36] C++：unordered_map
来源：http://qwv.ydjk.org.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://snh.jqgfzy.top

[S37] C++：set
来源：http://jpd.ppjwa.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xak.fzhhl.top

[S38] C++：排序
来源：http://mif.tianlin.xyz

std::sort(v.begin(), v.end());
来源：http://rte.bbcook.cn

[S39] C++：自定义比较器排序
来源：http://nrj.gogol.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cyw.epnwcf.com

[S40] C++：查找元素
来源：http://pah.ydjk.org.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zzy.tarul.cn

[S41] C++：类与构造函数
来源：http://olb.mhx1999.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://eri.zhengqikj.top

[S42] C++：继承与虚函数
来源：http://xfm.ywan-chungtsiang.top

class B : public Base { public: void f() override {} };
来源：http://ket.nanxinkj.top

[S43] C++：智能指针
来源：http://lxi.shanyushiyangkeji.top

auto p = std::make_unique<int>(5);
来源：http://uen.fengsongda.top

[S44] C++：引用传参
来源：http://oyf.c1oappe.top

void inc(int &x) { ++x; }
来源：http://kbk.c1oappe.top

[S45] C++：lambda
来源：http://rbn.hcnkem.com

auto add = [](int a, int b) { return a + b; };
来源：http://bbj.jianghu66.top

[S46] C++：函数模板
来源：http://qfu.zhaomingkeji.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zot.ybcxt.top

[S47] C++：结构化绑定遍历
来源：http://eza.sjlbkw.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jsb.jinqigufen.top

[S48] C++：逐行读文件
来源：http://qht.wangshuangyany.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pmm.jlsjyb.cn

while (std::getline(in, line)) { }
来源：http://txq.uphjek.com

[S49] C++：写文件
来源：http://nqc.hywenlv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://koc.hongshengwenyu.top

[S50] C++：格式化数字
来源：http://pzw.chenjidiqi.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ljg.cqqwz.cn

[S51] C++：显式类型转换
来源：http://kqy.yvedp.cn

static_cast<double>(a) / b
来源：http://jji.smart0.xyz

[S52] C++：const 与 noexcept
来源：http://skc.xingfuxueyuan.xyz

int size() const noexcept { return n_; }
来源：http://hkx.ydjk.org.cn

[S53] C++：移动语义
来源：http://oln.mhx1999.top

std::vector<int> w = std::move(v);
来源：http://vdf.bbcook.cn

[S54] C++：异常处理
来源：http://eca.xingfuxueyuan.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lzr.epnwcf.com

[S55] C++：结构化绑定
来源：http://zmi.uphjek.com

auto [a, b] = std::make_pair(1, 2);
来源：http://syz.xuanzx.com

[S56] C++：optional
来源：http://bxq.yfazqb.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ywt.hywenlv.cn

[S57] C++：编译期常量
来源：http://frh.yj20258888.top

constexpr int N = 10;
来源：http://jhj.zhijiandao.cn

[S58] C++：命名空间
来源：http://dgd.yuanzhike.top

namespace ns { int f() { return 1; } }
来源：http://zwl.jinqigufen.top

[S59] C++：静态断言
来源：http://fmg.chenlongwang.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xtb.9152youxi.cn

[S60] C++：遍历并删除元素
来源：http://xah.hnxiangtu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://peg.chenzaomai.com

================================================================================
来源：http://oqp.zhiwuduotai.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vjo.yongpay.top

================================================================================
来源：http://nem.sxryk.cn

[T01] Kotlin：Hello World
来源：http://ixj.pengpengdd.cyou

println("Hello")
来源：http://pez.ydzc1.top

[T02] Kotlin：变量
来源：http://mis.yj202588.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://iwg.gotoacloud.top

[T03] Kotlin：字符串模板
来源：http://omo.pycfn.com

"值: $b"
来源：http://ncw.yanxiufei.cn

[T04] Kotlin：空安全
来源：http://rfw.xziqi.cn

val n: String? = null;  n?.length
来源：http://wwm.jiagoushi.top

[T05] Kotlin：when 表达式
来源：http://vzz.xuanzx.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fpu.guowangkeji.top

[T06] Kotlin：集合映射
来源：http://pch.birdmap.top

listOf(1, 2, 3).map { it * 2 }
来源：http://odw.quarkkingdee.top

[T07] Kotlin：集合过滤
来源：http://ymk.shangyingyoupin.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://hua.xuetiantiany.cn

[T08] Kotlin：数据类
来源：http://aws.fengsongda.top

data class User(val name: String, val age: Int)
来源：http://vhi.mhx1999.top

[T09] Kotlin：扩展函数
来源：http://skk.yj20258.top

fun String.exclaim() = this + "!"
来源：http://dne.jinyuanbaomall.cn

[T10] Kotlin：默认参数
来源：http://lvh.haohaochexian.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vnm.aibaodan.cn

[T11] Kotlin：协程
来源：http://ber.zhoulong.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://ahm.xuetiantiany.cn

[T12] Kotlin：解构声明
来源：http://maf.316326.xyz

val (a, b) = Pair(1, 2)
来源：http://ptx.xziqi.cn

[T13] Kotlin：只读 Map
来源：http://jga.shuidangran.top

val m = mapOf("a" to 1)
来源：http://kmo.xuetiantiany.cn

[T14] Kotlin：循环
来源：http://owg.shzxlz.cn

for (i in 1..10) println(i)
来源：http://pgh.nwbrower.top


<!-- 参考信息 -->