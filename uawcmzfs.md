代发 wailian999

case "$1" in
来源：http://ixz.zycfv.cn

start) echo "启动" ;;
来源：http://zlc.bbcook.cn

stop)  echo "停止" ;;
来源：http://vmx.tian-w.cn

*)     echo "未知命令" ;;
来源：http://ohn.fktsv.cn

esac
来源：http://dog.jinqigfzy.top

[R12] for 遍历文件
来源：http://rtq.shanyushiyangkeji.top

for f in *.txt; do echo "$f"; done
来源：http://ctd.tanke756.top

[R13] for 计数循环
来源：http://ihv.wangdashe.top

for i in {1..10}; do echo "$i"; done
来源：http://adq.9152youxi.cn

[R14] C 风格 for
来源：http://mhe.bbcook.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lsr.tarul.cn

[R15] while 逐行读文件
来源：http://jbm.cheryme.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://udk.jianghu66.top

[R16] until 等待条件
来源：http://srm.zhongyouzk.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fhj.bjfxy.top

[R17] 数组定义与取值
来源：http://ehv.jiagoushi.top

arr=(a b c); echo "${arr[0]}"
来源：http://lih.hongshengwenyu.top

[R18] 遍历数组
来源：http://tkw.hnxiangtu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gnu.daxiang520.top

[R19] 数组长度
来源：http://win.daria6918.cn

echo "${#arr[@]}"
来源：http://lxl.havefunace.top

[R20] 关联数组（字典）
来源：http://ejh.jlsjyb.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mro.sufxvd.cn

[R21] 字符串长度
来源：http://ysb.yj20258888.top

echo "${#s}"
来源：http://qia.sxryk.cn

[R22] 截取子串
来源：http://uxb.kuanghao11.cn

echo "${s:0:5}"
来源：http://jzr.pycfn.com

[R23] 字符串替换
来源：http://utq.xingfuxueyuan.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uwt.cashguo.top

[R24] 大小写转换
来源：http://wzl.ybcxt.top

echo "${s^^}"; echo "${s,,}"
来源：http://wel.zhixingplan.top

[R25] 去后缀 / 去前缀
来源：http://ppc.svipenyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hnf.havefunace.top

[R26] 命令替换
来源：http://qcc.feifeiyinyue.top

now=$(date +%F); echo "$now"
来源：http://xbv.0kj1m.cn

[R27] 算术展开
来源：http://cir.gotoacloud.top

echo $((1 + 2 * 3))
来源：http://vja.zhijiandao.cn

[R28] 浮点运算
来源：http://xmw.xingfuxueyuan.xyz

echo "scale=2; 10/3" | bc
来源：http://nwj.hesvh.cn

[R29] 定义函数
来源：http://nzs.guowangkeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sgt.zhijiandao.cn

[R30] 函数返回状态码
来源：http://atc.bbcook.cn

f() { return 0; }; f || echo "失败了"
来源：http://moj.ppjwa.cn

[R31] 局部变量
来源：http://jnu.yonumen.top

f() { local x=1; echo "$x"; }
来源：http://ijb.yonumen.top

[R32] 参数个数校验
来源：http://nhd.kuanghao11.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dcz.hnxiangtu.top

[R33] 捕获错误并提示行号
来源：http://eff.zhijiandao.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cqh.svipenyu.cn

[R34] 退出时清理
来源：http://oxs.daria6918.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sed.smart0.xyz

[R35] 后台执行并等待
来源：http://mun.hnqzz.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wpg.tanke756.top

[R36] 并发执行多个任务
来源：http://rno.yj20258888.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zdu.kuanghao11.cn

[R37] 把输出赋给变量
来源：http://cet.tanke756.top

files=$(ls -1)
来源：http://tuc.tian-w.cn

[R38] 管道串联
来源：http://pnb.iojbl.cn

cat a.txt | grep -i error | wc -l
来源：http://pjy.fengsongda.top

[R39] 重定向标准输出与错误
来源：http://tkn.jinqigfzy.top

cmd > out.log 2>&1
来源：http://kkf.zhaomingkeji.xyz

[R40] 追加写日志
来源：http://prl.hnxiangtu.top

echo "log" >> out.log
来源：http://pew.zhaomingkeji.xyz

[R41] 丢弃输出
来源：http://gsz.guannengcc.top

cmd >/dev/null 2>&1
来源：http://jtw.guannengcc.top

[R42] 输入重定向
来源：http://wqo.ppjwa.cn

wc -l < a.txt
来源：http://mfd.dianchejie.cn

[R43] 按名字查找文件
来源：http://htr.shanyushiyangtech.top

find . -name "*.log" -type f
来源：http://qdp.ywan-chungtsiang.top

[R44] 按修改时间查找
来源：http://kgu.daxiang520.top

find . -mtime -7 -type f
来源：http://pct.meibo888.top

[R45] 批量删除
来源：http://hzk.gzhubu.top

find . -name "*.tmp" -delete
来源：http://eyy.feifeiyinyue.top

[R46] 递归替换文件内容
来源：http://bkx.gotoacloud.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vxg.fanxiaobao.xyz

[R47] sed 单行替换
来源：http://kjo.cqqwz.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gkb.tianlin.xyz

[R48] awk 取指定列
来源：http://nir.jiagoushi.top

awk '{print $1, $3}' a.txt
来源：http://jgw.yueranfly.top

[R49] awk 带条件
来源：http://tte.jianghu66.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oai.dashuyun.cn

[R50] awk 求和
来源：http://yce.bjfxy.top

awk '{s += $2} END {print s}' a.txt
来源：http://xia.yuxming.cn

[R51] 排序去重取前几
来源：http://oao.tanke756.top

sort a.txt | uniq -c | sort -rn | head
来源：http://pbw.yangfankeji.com

[R52] 统计行数
来源：http://bgn.andypj.xyz

wc -l a.txt
来源：http://skx.wangshuangyany.cn

[R53] 查看文件头与实时尾
来源：http://pqx.fktsv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yge.sxryk.cn

[R54] 比较两个文件
来源：http://iji.yueranfly.top

diff a.txt b.txt
来源：http://lym.tarul.cn

[R55] 压缩与解压
来源：http://ptc.mhx1999.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uwl.aizwys.cn

[R56] 远程拷贝
来源：http://ndg.fehbvm.com

scp file user@host:/path/
来源：http://weh.daria6918.cn

[R57] 远程执行命令
来源：http://gbf.vqdsnc.cn

ssh user@host 'uptime'
来源：http://xol.mhx1999.top

[R58] 下载文件
来源：http://tnl.quarkkingdee.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://myo.xinyue.icu

[R59] 发 POST JSON
来源：http://jri.tanke756.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rkk.9152youxi.cn

[R60] 只看 HTTP 状态码
来源：http://cwi.bbcook.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cbl.nanxuanxn.top

[R61] 磁盘占用
来源：http://vdq.yj20258.top

df -h;  du -sh *
来源：http://mxp.tarul.cn

[R62] 找最占空间的文件
来源：http://tsb.dashuyun.cn

du -ah . | sort -rh | head -10
来源：http://ueq.sxryk.cn

[R63] 内存与进程
来源：http://uzs.kuanghao11.cn

free -h;  ps aux | grep nginx
来源：http://kfr.yj20258888.top

[R64] 结束进程
来源：http://nsl.cdnleiting.top

kill -9 $(pgrep -f app.py)
来源：http://dcb.daria6918.cn

[R65] 查看端口占用
来源：http://kjv.yj20258888.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://clj.vqdsnc.cn

[R66] 定时任务
来源：http://snk.vehdjk.com

crontab -e;  crontab -l
来源：http://com.cdnleiting.top

[R67] 生成随机十六进制串
来源：http://hne.bjfxy.top

openssl rand -hex 16
来源：http://byz.xylfe.cn

[R68] 计算文件校验值
来源：http://muk.c1oappe.top

sha256sum a.txt;  md5sum a.txt
来源：http://bta.cucudq.cn

[R69] 生成随机密码
来源：http://bno.meibo888.top

head -c 16 /dev/urandom | base64
来源：http://wpp.jinyuanbaomall.cn

[R70] 时间戳与互转
来源：http://ulb.zdqjudy.top

date +%s;  date -d @1700000000
来源：http://zfg.zhiwuduotai.top

[R71] 日期格式化
来源：http://enb.tanke756.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://kzi.316326.xyz

[R72] 等待端口就绪
来源：http://kfk.shanyushiyangkeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qsf.yanxiufei.cn

[R73] 分割大日志
来源：http://qwy.dianchejie.cn

split -l 1000 big.log part_
来源：http://fki.cdnleiting.top

[R74] 批量重命名
来源：http://ttk.xuetiantiany.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mxq.hcnkem.com

[R75] 导出环境变量
来源：http://kuw.zhijiandao.cn

export PATH="$HOME/bin:$PATH"
来源：http://zfw.yueranfly.top

[R76] 使用临时文件
来源：http://eci.zycfv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nhg.fanxiaobao.xyz

[R77] 读取用户输入
来源：http://knn.sysykeji.top

read -rp "请输入: " ans
来源：http://yit.yj20258888.top

[R78] 交互式菜单
来源：http://uqb.shuidangran.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ywh.jinghuilouyu.cn

[R79] 解析命令行选项
来源：http://xiv.snrcjt.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qrf.zhoulong.xyz

[R80] 查看脚本执行耗时
来源：http://kbb.chenjidiqi.icu

time ./run.sh
来源：http://ebr.pycfn.com

================================================================================
来源：http://vwi.pengpengdd.cyou

S. C / C++ 专题
来源：http://pwk.316326.xyz

================================================================================
来源：http://dhu.gaohongyu789.top

[S01] C：Hello World
来源：http://xhx.shanyushiyangtech.top

#include <stdio.h>
来源：http://cuo.yangfankeji.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://krt.svipenyu.cn

[S02] C：变量与格式化输出
来源：http://ttc.fzhhl.top

int a = 10; printf("%d\n", a);
来源：http://fes.ehwqpu.com

[S03] C：读入整数
来源：http://tzj.hesvh.cn

int x; scanf("%d", &x);
来源：http://khg.yanxiufei.cn

[S04] C：字符串复制
来源：http://dkp.wangshuangyany.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tuk.fanxiaobao.xyz

[S05] C：字符串长度
来源：http://ils.yuanzhike.top

strlen(s)
来源：http://hpj.0kj1m.cn

[S06] C：字符串比较
来源：http://tro.dianchejie.cn

strcmp(a, b) == 0
来源：http://rjo.jinyuanbaomall.cn

[S07] C：数组遍历求和
来源：http://kus.kuanghao11.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pbj.epnwcf.com

[S08] C：动态内存分配与释放
来源：http://vmc.tian-w.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cgy.birdmap.top

[S09] C：结构体定义与初始化
来源：http://num.ehwqpu.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uwg.xuetiantiany.cn

[S10] C：指针与解引用
来源：http://usg.ybcxt.top

int *p = &a;  *p = 5;
来源：http://onx.cucudq.cn

[S11] C：逐行读文件
来源：http://tby.nanxuanxn.top

FILE *f = fopen("a.txt", "r");
来源：http://bha.cheryme.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vjz.quarkkingdee.top

fclose(f);
来源：http://yyp.chenjidiqi.icu

[S12] C：写文件
来源：http://mom.shanyushiyangtech.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://apz.gzhubu.top

[S13] C：宏定义
来源：http://zsj.sweek.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ixb.svipenyu.cn

[S14] C：枚举
来源：http://xbt.jianghu66.top

enum Color { RED, GREEN, BLUE };
来源：http://fhl.sxryk.cn

[S15] C：类型转换
来源：http://soq.zdqjudy.top

(double) a / b
来源：http://gfa.0kj1m.cn

[S16] C：位操作置位
来源：http://xra.jinqigfzy.top

x |= (1 << 3);
来源：http://wgw.jinghuilouyu.cn

[S17] C：安全拼接字符串
来源：http://dll.gzhubu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dxq.epnwcf.com

[S18] C：命令行参数
来源：http://kjb.hongshengwenyu.top

int main(int argc, char **argv)
来源：http://pwi.snrcjt.cn

[S19] C：快速排序
来源：http://bat.zdqjudy.top

qsort(a, n, sizeof(int), cmp);
来源：http://kuq.hcnkem.com

[S20] C：二分查找
来源：http://hge.sxryk.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yzp.yj20258888.top

[S21] C：字符类别判断
来源：http://xyq.jqgufenzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gux.meibo888.top

[S22] C：字符串转数字
来源：http://pki.wangshuangyany.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xav.ywan-chungtsiang.top

[S23] C：随机数
来源：http://rzj.jiagoushi.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mzq.havefunace.top

[S24] C：获取本地时间
来源：http://rqf.iojbl.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mjm.tianlin.xyz

[S25] C：内存拷贝
来源：http://uvw.fzhhl.top

memcpy(dst, src, n);
来源：http://ihu.ydzc1.top

[S26] C：内存清零
来源：http://mfy.smart0.xyz

memset(a, 0, sizeof a);
来源：http://lla.yueranfly.top

[S27] C：定义常量
来源：http://foh.c1oappe.top

const double PI = 3.14159;
来源：http://vaf.hammf.cn

[S28] C：静态变量
来源：http://lcr.xuetiantiany.cn

static int counter = 0;
来源：http://lwm.meibo888.top

[S29] C：变参函数
来源：http://zss.aizwys.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://seo.zhengqikj.top

[S30] C：头文件保护
来源：http://zdq.tanke756.top

#ifndef X_H
来源：http://usu.snrcjt.cn

#define X_H
来源：http://crf.yangfankeji.com

#endif
来源：http://nly.daxiang520.top

[S31] C++：Hello World
来源：http://jfu.quarkkingdee.top

#include <iostream>
来源：http://hhp.smart0.xyz

int main() { std::cout << "Hello\n"; }
来源：http://xjl.jinyuanbaomall.cn

[S32] C++：字符串
来源：http://qzv.dianchejie.cn

std::string s = "hi";  s += "!";
来源：http://hrl.jinghuilouyu.cn

[S33] C++：vector 增删
来源：http://ekh.cheryme.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ytz.ywan-chungtsiang.top

[S34] C++：遍历 vector
来源：http://kae.shzxlz.cn

for (auto &x : v) { std::cout << x; }
来源：http://mzy.cqqwz.cn

[S35] C++：map
来源：http://pwx.jinghuilouyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wuq.chenzaomai.com

[S36] C++：unordered_map
来源：http://ehk.sufxvd.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xze.gotoacloud.top

[S37] C++：set
来源：http://fjt.gotoacloud.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oah.daxiang520.top

[S38] C++：排序
来源：http://grm.zhoulong.xyz

std::sort(v.begin(), v.end());
来源：http://dkt.uphjek.com

[S39] C++：自定义比较器排序
来源：http://sqt.sysykeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jco.52xcode.cn

[S40] C++：查找元素
来源：http://uhg.shanyushiyangkeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wiu.hesvh.cn

[S41] C++：类与构造函数
来源：http://xoo.chenjidiqi.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zee.jinqigufen.top

[S42] C++：继承与虚函数
来源：http://vbl.xziqi.cn

class B : public Base { public: void f() override {} };
来源：http://cqs.0kj1m.cn

[S43] C++：智能指针
来源：http://omh.daria6918.cn

auto p = std::make_unique<int>(5);
来源：http://erh.sjlbkw.cn

[S44] C++：引用传参
来源：http://nbw.birdmap.top

void inc(int &x) { ++x; }
来源：http://pgu.snrcjt.cn

[S45] C++：lambda
来源：http://koa.ybcxt.top

auto add = [](int a, int b) { return a + b; };
来源：http://bvu.birdmap.top

[S46] C++：函数模板
来源：http://fdw.cqqwz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://njt.xziqi.cn

[S47] C++：结构化绑定遍历
来源：http://cbx.shanyushiyangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fgk.uphjek.com

[S48] C++：逐行读文件
来源：http://ebe.hongshengwenyu.top

std::ifstream in("a.txt");  std::string line;
来源：http://ups.nwbrower.top

while (std::getline(in, line)) { }
来源：http://oei.0kj1m.cn

[S49] C++：写文件
来源：http://fay.yj202588.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qzh.vqdsnc.cn

[S50] C++：格式化数字
来源：http://bhf.cashguo.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tlu.guannengcc.top

[S51] C++：显式类型转换
来源：http://kgg.sxryk.cn

static_cast<double>(a) / b
来源：http://uky.hysaishi.cn

[S52] C++：const 与 noexcept
来源：http://zum.hnqzz.top

int size() const noexcept { return n_; }
来源：http://kkx.zhaomingkeji.xyz

[S53] C++：移动语义
来源：http://rwo.yanxiufei.cn

std::vector<int> w = std::move(v);
来源：http://rzg.redwolf501.top

[S54] C++：异常处理
来源：http://qjf.uphjek.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://iwq.shanyushiyangkeji.top

[S55] C++：结构化绑定
来源：http://nwv.hammf.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qlf.zhongyouzk.top

[S56] C++：optional
来源：http://chj.0kj1m.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pve.yangfankeji.com

[S57] C++：编译期常量
来源：http://ifc.sjlbkw.cn

constexpr int N = 10;
来源：http://odn.jinqigufen.top

[S58] C++：命名空间
来源：http://eqe.cheryme.top

namespace ns { int f() { return 1; } }
来源：http://otl.sysykeji.top

[S59] C++：静态断言
来源：http://mqh.cashguo.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mre.ywan-chungtsiang.top

[S60] C++：遍历并删除元素
来源：http://kub.shanyushiyangtech.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hph.jiagoushi.top

================================================================================
来源：http://xja.yuxming.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wkz.pycfn.com

================================================================================
来源：http://mut.andypj.xyz

[T01] Kotlin：Hello World
来源：http://iow.snrcjt.cn

println("Hello")
来源：http://qjl.yuxming.cn

[T02] Kotlin：变量
来源：http://zhs.snrcjt.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://isp.fanxiaobao.xyz

[T03] Kotlin：字符串模板
来源：http://wxx.gaohongyu789.top

"值: $b"
来源：http://wxu.tanke756.top

[T04] Kotlin：空安全
来源：http://wve.cqqwz.cn

val n: String? = null;  n?.length
来源：http://mqe.gotoacloud.top

[T05] Kotlin：when 表达式
来源：http://uah.jinqigfzy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iql.cqqwz.cn

[T06] Kotlin：集合映射
来源：http://iob.xinyue.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://nya.zhongyouzk.top

[T07] Kotlin：集合过滤
来源：http://mlz.shangyingyoupin.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://klw.jinqigufen.top

[T08] Kotlin：数据类
来源：http://sgf.epnwcf.com

data class User(val name: String, val age: Int)
来源：http://wgp.jinqigfzy.top

[T09] Kotlin：扩展函数
来源：http://xyh.hesvh.cn

fun String.exclaim() = this + "!"
来源：http://blc.hesvh.cn

[T10] Kotlin：默认参数
来源：http://fhc.316326.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://wjg.gotoacloud.top

[T11] Kotlin：协程
来源：http://yqn.quarkkingdee.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://lfr.yueranfly.top

[T12] Kotlin：解构声明
来源：http://cib.52xcode.cn

val (a, b) = Pair(1, 2)
来源：http://ege.cucudq.cn


<!-- 参考信息 -->