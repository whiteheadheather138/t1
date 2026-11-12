代发 wailian999

esac
来源：http://zvq.gaohongyu789.top

[R12] for 遍历文件
来源：http://mjl.quarkkingdee.top

for f in *.txt; do echo "$f"; done
来源：http://gkl.zhengqikj.top

[R13] for 计数循环
来源：http://mrz.wangshuangyany.cn

for i in {1..10}; do echo "$i"; done
来源：http://gev.sjlbkw.cn

[R14] C 风格 for
来源：http://cdl.uphjek.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dco.cheryme.top

[R15] while 逐行读文件
来源：http://zoq.zycfv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://atl.jinghuilouyu.cn

[R16] until 等待条件
来源：http://nag.jinqigufen.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dtr.jyoumei.cn

[R17] 数组定义与取值
来源：http://jmy.ehwqpu.com

arr=(a b c); echo "${arr[0]}"
来源：http://idf.zdbjq.cn

[R18] 遍历数组
来源：http://ajk.jinghuilouyu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://idy.wangdashe.top

[R19] 数组长度
来源：http://fhw.havefunace.top

echo "${#arr[@]}"
来源：http://xlb.shzxlz.cn

[R20] 关联数组（字典）
来源：http://nkx.yanxiufei.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mir.xziqi.cn

[R21] 字符串长度
来源：http://siy.svipenyu.cn

echo "${#s}"
来源：http://wzs.nanxuanxn.top

[R22] 截取子串
来源：http://cmq.xziqi.cn

echo "${s:0:5}"
来源：http://mez.dashuyun.cn

[R23] 字符串替换
来源：http://hfc.yuxming.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uua.gaohongyu789.top

[R24] 大小写转换
来源：http://lfq.yj20258.top

echo "${s^^}"; echo "${s,,}"
来源：http://kpw.meibo888.top

[R25] 去后缀 / 去前缀
来源：http://myr.fehbvm.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://cdb.xinyue.icu

[R26] 命令替换
来源：http://qeh.hywenlv.cn

now=$(date +%F); echo "$now"
来源：http://kqm.daria6918.cn

[R27] 算术展开
来源：http://opc.andypj.xyz

echo $((1 + 2 * 3))
来源：http://cph.smart0.xyz

[R28] 浮点运算
来源：http://zer.yfazqb.com

echo "scale=2; 10/3" | bc
来源：http://sgx.xylfe.cn

[R29] 定义函数
来源：http://mte.sxryk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tya.wangdashe.top

[R30] 函数返回状态码
来源：http://ncm.bjfxy.top

f() { return 0; }; f || echo "失败了"
来源：http://axi.havefunace.top

[R31] 局部变量
来源：http://uib.fanxiaobao.xyz

f() { local x=1; echo "$x"; }
来源：http://sip.cashguo.top

[R32] 参数个数校验
来源：http://exm.jqgufenzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lym.xuanzx.com

[R33] 捕获错误并提示行号
来源：http://brm.shzxlz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cjo.ctjpmb.com

[R34] 退出时清理
来源：http://cpn.hywenlv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://phi.shuidangran.top

[R35] 后台执行并等待
来源：http://smz.chenjidiqi.icu

sleep 5 & pid=$!; wait "$pid"
来源：http://lig.yfazqb.com

[R36] 并发执行多个任务
来源：http://wru.shangyingyoupin.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wey.hnqzz.top

[R37] 把输出赋给变量
来源：http://czl.pycfn.com

files=$(ls -1)
来源：http://oqs.yj20258888.top

[R38] 管道串联
来源：http://wqk.cashguo.top

cat a.txt | grep -i error | wc -l
来源：http://fye.daria6918.cn

[R39] 重定向标准输出与错误
来源：http://rgi.zhengqikj.top

cmd > out.log 2>&1
来源：http://aik.svipenyu.cn

[R40] 追加写日志
来源：http://pdx.yj20258888.top

echo "log" >> out.log
来源：http://iko.tarul.cn

[R41] 丢弃输出
来源：http://bsm.yangfankeji.com

cmd >/dev/null 2>&1
来源：http://pcz.aizwys.cn

[R42] 输入重定向
来源：http://gab.ydjk.org.cn

wc -l < a.txt
来源：http://vkr.yvedp.cn

[R43] 按名字查找文件
来源：http://rbo.nwbrower.top

find . -name "*.log" -type f
来源：http://fns.yvedp.cn

[R44] 按修改时间查找
来源：http://jqi.fzhhl.top

find . -mtime -7 -type f
来源：http://oqq.hnxiangtu.top

[R45] 批量删除
来源：http://auq.nanxuanxn.top

find . -name "*.tmp" -delete
来源：http://gvl.meibo888.top

[R46] 递归替换文件内容
来源：http://dxj.bbcook.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tea.yuxming.cn

[R47] sed 单行替换
来源：http://rjm.shangyingyoupin.top

sed -i 's/foo/bar/g' a.txt
来源：http://acq.zdbjq.cn

[R48] awk 取指定列
来源：http://ycx.316326.xyz

awk '{print $1, $3}' a.txt
来源：http://lzk.birdmap.top

[R49] awk 带条件
来源：http://trz.vehdjk.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rmo.quarkkingdee.top

[R50] awk 求和
来源：http://zcz.birdmap.top

awk '{s += $2} END {print s}' a.txt
来源：http://vlw.0kj1m.cn

[R51] 排序去重取前几
来源：http://nlc.meibo888.top

sort a.txt | uniq -c | sort -rn | head
来源：http://wdl.iojbl.cn

[R52] 统计行数
来源：http://whz.guowangkeji.top

wc -l a.txt
来源：http://vsi.iojbl.cn

[R53] 查看文件头与实时尾
来源：http://ayt.wangshuangyany.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mdo.chenzaomai.com

[R54] 比较两个文件
来源：http://gvw.vehdjk.com

diff a.txt b.txt
来源：http://yzj.havefunace.top

[R55] 压缩与解压
来源：http://dci.9152youxi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fws.zdqjudy.top

[R56] 远程拷贝
来源：http://jpy.xinyue.icu

scp file user@host:/path/
来源：http://jrg.nanxinkj.top

[R57] 远程执行命令
来源：http://lpe.shuidangran.top

ssh user@host 'uptime'
来源：http://phv.aizwys.cn

[R58] 下载文件
来源：http://cyq.xuetiantiany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gnx.shuidangran.top

[R59] 发 POST JSON
来源：http://tku.zhiwuduotai.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ipz.316326.xyz

[R60] 只看 HTTP 状态码
来源：http://xmj.smart0.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qav.jiagoushi.top

[R61] 磁盘占用
来源：http://zdd.hongshengwenyu.top

df -h;  du -sh *
来源：http://byh.zhijiandao.cn

[R62] 找最占空间的文件
来源：http://czm.yongpay.top

du -ah . | sort -rh | head -10
来源：http://uyq.birdmap.top

[R63] 内存与进程
来源：http://fsw.hywenlv.cn

free -h;  ps aux | grep nginx
来源：http://mow.xziqi.cn

[R64] 结束进程
来源：http://ekz.yvedp.cn

kill -9 $(pgrep -f app.py)
来源：http://ith.shanyushiyangtech.top

[R65] 查看端口占用
来源：http://vws.zhiwuduotai.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mnx.aibaodan.cn

[R66] 定时任务
来源：http://dtw.aibaodan.cn

crontab -e;  crontab -l
来源：http://ydk.yueranfly.top

[R67] 生成随机十六进制串
来源：http://xre.jqgufenzy.top

openssl rand -hex 16
来源：http://axg.quarkkingdee.top

[R68] 计算文件校验值
来源：http://tuf.guannengcc.top

sha256sum a.txt;  md5sum a.txt
来源：http://ibl.birdmap.top

[R69] 生成随机密码
来源：http://zvp.zhengqikj.top

head -c 16 /dev/urandom | base64
来源：http://ise.daxiang520.top

[R70] 时间戳与互转
来源：http://pkv.yueranfly.top

date +%s;  date -d @1700000000
来源：http://vdi.bjfxy.top

[R71] 日期格式化
来源：http://ywb.shangyingyoupin.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://hlm.vehdjk.com

[R72] 等待端口就绪
来源：http://xot.xuanzx.com

until nc -z localhost 3306; do sleep 1; done
来源：http://kml.0kj1m.cn

[R73] 分割大日志
来源：http://ptg.redwolf501.top

split -l 1000 big.log part_
来源：http://dlb.dashuyun.cn

[R74] 批量重命名
来源：http://yzu.daria6918.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fki.tianlin.xyz

[R75] 导出环境变量
来源：http://zib.yj202588.top

export PATH="$HOME/bin:$PATH"
来源：http://kgl.bjfxy.top

[R76] 使用临时文件
来源：http://kfb.zhiwuduotai.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zsl.yuanzhike.top

[R77] 读取用户输入
来源：http://cwr.vehdjk.com

read -rp "请输入: " ans
来源：http://yul.hywenlv.cn

[R78] 交互式菜单
来源：http://cmb.jqgufenzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vqf.dashuyun.cn

[R79] 解析命令行选项
来源：http://vbp.zhijiandao.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://asu.ctjpmb.com

[R80] 查看脚本执行耗时
来源：http://rpt.shanyushiyangtech.top

time ./run.sh
来源：http://nxt.nanxinkj.top

================================================================================
来源：http://fco.daria6918.cn

S. C / C++ 专题
来源：http://ivk.jqgufenzy.top

================================================================================
来源：http://ldv.guannengcc.top

[S01] C：Hello World
来源：http://sms.hysaishi.cn

#include <stdio.h>
来源：http://bbl.shzxlz.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lzw.jinqigfzy.top

[S02] C：变量与格式化输出
来源：http://hhl.yvedp.cn

int a = 10; printf("%d\n", a);
来源：http://ppc.316326.xyz

[S03] C：读入整数
来源：http://pjt.jqgufenzy.top

int x; scanf("%d", &x);
来源：http://bla.sxryk.cn

[S04] C：字符串复制
来源：http://fvy.0kj1m.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rhz.tarul.cn

[S05] C：字符串长度
来源：http://wrh.chenjidiqi.icu

strlen(s)
来源：http://gtm.shzxlz.cn

[S06] C：字符串比较
来源：http://ffx.sufxvd.cn

strcmp(a, b) == 0
来源：http://dpu.tian-w.cn

[S07] C：数组遍历求和
来源：http://efl.sxryk.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bfc.daria6918.cn

[S08] C：动态内存分配与释放
来源：http://mhz.sxryk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rte.yj20258888.top

[S09] C：结构体定义与初始化
来源：http://pdc.ydjk.org.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rfx.wangdashe.top

[S10] C：指针与解引用
来源：http://ynn.tanke756.top

int *p = &a;  *p = 5;
来源：http://sux.xziqi.cn

[S11] C：逐行读文件
来源：http://mtl.yj20258888.top

FILE *f = fopen("a.txt", "r");
来源：http://jmt.yuanzhike.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://abd.gaohongyu789.top

fclose(f);
来源：http://qut.yfazqb.com

[S12] C：写文件
来源：http://wdk.yj20258888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hyd.hesvh.cn

[S13] C：宏定义
来源：http://bnw.shanyushiyangtech.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ktg.shanyushiyangkeji.top

[S14] C：枚举
来源：http://xoq.cqqwz.cn

enum Color { RED, GREEN, BLUE };
来源：http://jic.vqdsnc.cn

[S15] C：类型转换
来源：http://bbh.jqgufenzy.top

(double) a / b
来源：http://col.birdmap.top

[S16] C：位操作置位
来源：http://evt.shzxlz.cn

x |= (1 << 3);
来源：http://klg.ehwqpu.com

[S17] C：安全拼接字符串
来源：http://iip.jinyuanbaomall.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://agb.fanxiaobao.xyz

[S18] C：命令行参数
来源：http://qib.fzhhl.top

int main(int argc, char **argv)
来源：http://wpc.jinqigfzy.top

[S19] C：快速排序
来源：http://vie.tarul.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xhg.tianlin.xyz

[S20] C：二分查找
来源：http://lqr.redwolf501.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gsl.yuanzhike.top

[S21] C：字符类别判断
来源：http://cdo.ivvv.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ebm.zhaomingkeji.xyz

[S22] C：字符串转数字
来源：http://dpn.smart0.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://soa.daxiang520.top

[S23] C：随机数
来源：http://umf.xinyue.icu

srand(time(NULL));  int r = rand() % 100;
来源：http://ely.hfpthk.cn

[S24] C：获取本地时间
来源：http://tcz.zdqjudy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://usp.yj202588.top

[S25] C：内存拷贝
来源：http://lmf.dashuyun.cn

memcpy(dst, src, n);
来源：http://rde.bjfxy.top

[S26] C：内存清零
来源：http://flk.bjfxy.top

memset(a, 0, sizeof a);
来源：http://edh.yuxming.cn

[S27] C：定义常量
来源：http://duy.guowangkeji.top

const double PI = 3.14159;
来源：http://des.jiagoushi.top

[S28] C：静态变量
来源：http://xiy.snrcjt.cn

static int counter = 0;
来源：http://aan.yuanzhike.top

[S29] C：变参函数
来源：http://pnj.gogol.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://aeg.jqgfzy.top

[S30] C：头文件保护
来源：http://inb.dashuyun.cn

#ifndef X_H
来源：http://qri.jqgufenzy.top

#define X_H
来源：http://xiu.zhiwuduotai.top

#endif
来源：http://vua.xinyue.icu

[S31] C++：Hello World
来源：http://obn.ywan-chungtsiang.top

#include <iostream>
来源：http://mui.gotoacloud.top

int main() { std::cout << "Hello\n"; }
来源：http://jhr.9152youxi.cn

[S32] C++：字符串
来源：http://bjo.redwolf501.top

std::string s = "hi";  s += "!";
来源：http://ifj.yfazqb.com

[S33] C++：vector 增删
来源：http://rai.iojbl.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hzf.yfazqb.com

[S34] C++：遍历 vector
来源：http://hyu.fehbvm.com

for (auto &x : v) { std::cout << x; }
来源：http://rki.sjlbkw.cn

[S35] C++：map
来源：http://ebd.hammf.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wfy.aibaodan.cn

[S36] C++：unordered_map
来源：http://qtm.zhongyouzk.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://prg.haohaochexian.top

[S37] C++：set
来源：http://sys.cdnleiting.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ddd.sxryk.cn

[S38] C++：排序
来源：http://ehi.zhaomingkeji.xyz

std::sort(v.begin(), v.end());
来源：http://wxx.jinqigfzy.top

[S39] C++：自定义比较器排序
来源：http://bzx.hesvh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://voy.xylfe.cn

[S40] C++：查找元素
来源：http://zij.xuetiantiany.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wln.mhx1999.top

[S41] C++：类与构造函数
来源：http://wkt.shanyushiyangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://akr.0kj1m.cn

[S42] C++：继承与虚函数
来源：http://wkl.meibo888.top

class B : public Base { public: void f() override {} };
来源：http://gyp.zhaomingkeji.xyz

[S43] C++：智能指针
来源：http://xny.hysaishi.cn

auto p = std::make_unique<int>(5);
来源：http://xuq.hysaishi.cn

[S44] C++：引用传参
来源：http://lht.hesvh.cn

void inc(int &x) { ++x; }
来源：http://uod.fktsv.cn

[S45] C++：lambda
来源：http://iwn.daria6918.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cvt.sysykeji.top

[S46] C++：函数模板
来源：http://auo.meibo888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ysq.dashuyun.cn

[S47] C++：结构化绑定遍历
来源：http://oof.jqgufenzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://feq.birdmap.top

[S48] C++：逐行读文件
来源：http://kow.gogol.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fmb.zhaomingkeji.xyz

while (std::getline(in, line)) { }
来源：http://fto.pengpengdd.cyou

[S49] C++：写文件
来源：http://bqo.ywan-chungtsiang.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nxz.havefunace.top

[S50] C++：格式化数字
来源：http://quc.gotoacloud.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vmn.bjfxy.top

[S51] C++：显式类型转换
来源：http://utr.zhijiandao.cn

static_cast<double>(a) / b
来源：http://nac.zycfv.cn

[S52] C++：const 与 noexcept
来源：http://wfb.ctjpmb.com

int size() const noexcept { return n_; }
来源：http://pzt.tian-w.cn

[S53] C++：移动语义
来源：http://oor.52xcode.cn

std::vector<int> w = std::move(v);
来源：http://jgu.aizwys.cn

[S54] C++：异常处理
来源：http://juh.sjlbkw.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ynv.smart0.xyz

[S55] C++：结构化绑定
来源：http://gra.wangdashe.top

auto [a, b] = std::make_pair(1, 2);
来源：http://yqx.yongpay.top

[S56] C++：optional
来源：http://ezo.pycfn.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ijg.xinyue.icu

[S57] C++：编译期常量
来源：http://llb.sysykeji.top

constexpr int N = 10;
来源：http://eul.zhongyouzk.top

[S58] C++：命名空间
来源：http://rdb.xingfuxueyuan.xyz

namespace ns { int f() { return 1; } }
来源：http://xcb.jinqigfzy.top

[S59] C++：静态断言
来源：http://mnt.zdqjudy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pbd.yangfankeji.com

[S60] C++：遍历并删除元素
来源：http://qsv.dianchejie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cqt.gogol.net.cn

================================================================================
来源：http://xza.jinghuilouyu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zwk.shuidangran.top

================================================================================
来源：http://jmf.birdmap.top

[T01] Kotlin：Hello World
来源：http://mst.wangdashe.top

println("Hello")
来源：http://ywb.tanke756.top

[T02] Kotlin：变量
来源：http://xnk.pycfn.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rsl.cdnleiting.top

[T03] Kotlin：字符串模板
来源：http://wsn.hysaishi.cn

"值: $b"
来源：http://zuu.shangyingyoupin.top

[T04] Kotlin：空安全
来源：http://liy.316326.xyz

val n: String? = null;  n?.length
来源：http://fut.shanyushiyangkeji.top

[T05] Kotlin：when 表达式
来源：http://ehi.shanyushiyangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rpb.hnqzz.top

[T06] Kotlin：集合映射
来源：http://qap.9152youxi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hlj.vqdsnc.cn

[T07] Kotlin：集合过滤
来源：http://wcg.yj20258.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vin.yj20258.top

[T08] Kotlin：数据类
来源：http://qrr.yangfankeji.com

data class User(val name: String, val age: Int)
来源：http://gfk.nanxuanxn.top

[T09] Kotlin：扩展函数
来源：http://onr.svipenyu.cn

fun String.exclaim() = this + "!"
来源：http://ctm.redwolf501.top

[T10] Kotlin：默认参数
来源：http://yym.zhongyouzk.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qyo.ywan-chungtsiang.top

[T11] Kotlin：协程
来源：http://zbr.jinghuilouyu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://slz.yangfankeji.com

[T12] Kotlin：解构声明
来源：http://ojp.cucudq.cn

val (a, b) = Pair(1, 2)
来源：http://uhf.birdmap.top

[T13] Kotlin：只读 Map
来源：http://lku.havefunace.top

val m = mapOf("a" to 1)
来源：http://wet.cucudq.cn

[T14] Kotlin：循环
来源：http://sxx.zhoulong.xyz

for (i in 1..10) println(i)
来源：http://azj.daxiang520.top


<!-- 参考信息 -->