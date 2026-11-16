代发 wailian999

case "$1" in
来源：http://mln.birdmap.top

start) echo "启动" ;;
来源：http://tba.tanke756.top

stop)  echo "停止" ;;
来源：http://wtm.tian-w.cn

*)     echo "未知命令" ;;
来源：http://net.wangshuangyany.cn

esac
来源：http://ehu.fanxiaobao.xyz

[R12] for 遍历文件
来源：http://qtp.sweek.top

for f in *.txt; do echo "$f"; done
来源：http://pok.hesvh.cn

[R13] for 计数循环
来源：http://zwr.hywenlv.cn

for i in {1..10}; do echo "$i"; done
来源：http://lpl.ehwqpu.com

[R14] C 风格 for
来源：http://kva.jianghu66.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dhf.yuanzhike.top

[R15] while 逐行读文件
来源：http://sfi.hcnkem.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ubd.mhx1999.top

[R16] until 等待条件
来源：http://htq.guannengcc.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wnh.zhoulong.xyz

[R17] 数组定义与取值
来源：http://gdw.shzxlz.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zno.zdqjudy.top

[R18] 遍历数组
来源：http://srn.tanke756.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://emb.xziqi.cn

[R19] 数组长度
来源：http://ekb.tarul.cn

echo "${#arr[@]}"
来源：http://fdw.chenjidiqi.icu

[R20] 关联数组（字典）
来源：http://dvp.xuetiantiany.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qnj.9152youxi.cn

[R21] 字符串长度
来源：http://jkf.xuetiantiany.cn

echo "${#s}"
来源：http://wna.meibo888.top

[R22] 截取子串
来源：http://fky.guowangkeji.top

echo "${s:0:5}"
来源：http://uyy.316326.xyz

[R23] 字符串替换
来源：http://gdk.meibo888.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uym.ppjwa.cn

[R24] 大小写转换
来源：http://ruf.hfpthk.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gbi.daxiang520.top

[R25] 去后缀 / 去前缀
来源：http://ral.tanke756.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://rmh.zhiwuduotai.top

[R26] 命令替换
来源：http://qus.cqqwz.cn

now=$(date +%F); echo "$now"
来源：http://igc.zhoulong.xyz

[R27] 算术展开
来源：http://wmm.jinghuilouyu.cn

echo $((1 + 2 * 3))
来源：http://bbr.zycfv.cn

[R28] 浮点运算
来源：http://kll.zhoulong.xyz

echo "scale=2; 10/3" | bc
来源：http://hqs.jinqigufen.top

[R29] 定义函数
来源：http://jbs.hcnkem.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rdz.uphjek.com

[R30] 函数返回状态码
来源：http://tvx.cheryme.top

f() { return 0; }; f || echo "失败了"
来源：http://fcy.jlsjyb.cn

[R31] 局部变量
来源：http://bgd.wangdashe.top

f() { local x=1; echo "$x"; }
来源：http://rbu.xylfe.cn

[R32] 参数个数校验
来源：http://nse.jiagoushi.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jgl.cqqwz.cn

[R33] 捕获错误并提示行号
来源：http://bwo.mhx1999.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://foi.cheryme.top

[R34] 退出时清理
来源：http://yke.xinyue.icu

trap 'rm -f "$tmp"' EXIT
来源：http://xdu.jinqigufen.top

[R35] 后台执行并等待
来源：http://ptr.shzxlz.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://amu.jyoumei.cn

[R36] 并发执行多个任务
来源：http://ska.yueranfly.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oqh.kuanghao11.cn

[R37] 把输出赋给变量
来源：http://jwq.zhiwuduotai.top

files=$(ls -1)
来源：http://egy.cashguo.top

[R38] 管道串联
来源：http://hva.ppjwa.cn

cat a.txt | grep -i error | wc -l
来源：http://bjh.yj20258888.top

[R39] 重定向标准输出与错误
来源：http://jcj.daria6918.cn

cmd > out.log 2>&1
来源：http://mfp.gaohongyu789.top

[R40] 追加写日志
来源：http://xag.pengpengdd.cyou

echo "log" >> out.log
来源：http://auu.uphjek.com

[R41] 丢弃输出
来源：http://flc.vqdsnc.cn

cmd >/dev/null 2>&1
来源：http://mbl.fzhhl.top

[R42] 输入重定向
来源：http://qoe.hcnkem.com

wc -l < a.txt
来源：http://ats.shzxlz.cn

[R43] 按名字查找文件
来源：http://bmo.fzhhl.top

find . -name "*.log" -type f
来源：http://euv.kuanghao11.cn

[R44] 按修改时间查找
来源：http://txd.jqgfzy.top

find . -mtime -7 -type f
来源：http://ivt.gogol.net.cn

[R45] 批量删除
来源：http://tab.xylfe.cn

find . -name "*.tmp" -delete
来源：http://sje.daria6918.cn

[R46] 递归替换文件内容
来源：http://mwu.sweek.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pdi.sjlbkw.cn

[R47] sed 单行替换
来源：http://twc.jianghu66.top

sed -i 's/foo/bar/g' a.txt
来源：http://ptm.daxiang520.top

[R48] awk 取指定列
来源：http://psa.epnwcf.com

awk '{print $1, $3}' a.txt
来源：http://ljn.snrcjt.cn

[R49] awk 带条件
来源：http://imk.yueranfly.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rda.ybcxt.top

[R50] awk 求和
来源：http://lsw.jyoumei.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ypi.hcnkem.com

[R51] 排序去重取前几
来源：http://xge.jinqigufen.top

sort a.txt | uniq -c | sort -rn | head
来源：http://tzh.316326.xyz

[R52] 统计行数
来源：http://mpc.mhx1999.top

wc -l a.txt
来源：http://iib.vehdjk.com

[R53] 查看文件头与实时尾
来源：http://rak.cdnleiting.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ajx.0kj1m.cn

[R54] 比较两个文件
来源：http://yop.yj202588.top

diff a.txt b.txt
来源：http://qqf.yj20258888.top

[R55] 压缩与解压
来源：http://jmg.cucudq.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ios.ppjwa.cn

[R56] 远程拷贝
来源：http://iyb.fzhhl.top

scp file user@host:/path/
来源：http://dtd.yj202588.top

[R57] 远程执行命令
来源：http://cdm.sxryk.cn

ssh user@host 'uptime'
来源：http://gov.hesvh.cn

[R58] 下载文件
来源：http://hut.fktsv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lvs.feifeiyinyue.top

[R59] 发 POST JSON
来源：http://zny.hnxiangtu.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pto.316326.xyz

[R60] 只看 HTTP 状态码
来源：http://zxk.316326.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://naw.yj20258.top

[R61] 磁盘占用
来源：http://ttf.gotoacloud.top

df -h;  du -sh *
来源：http://xdb.guowangkeji.top

[R62] 找最占空间的文件
来源：http://dxw.yj20258.top

du -ah . | sort -rh | head -10
来源：http://rit.zhengqikj.top

[R63] 内存与进程
来源：http://phl.jinyuanbaomall.cn

free -h;  ps aux | grep nginx
来源：http://agp.shangyingyoupin.top

[R64] 结束进程
来源：http://hzy.hywenlv.cn

kill -9 $(pgrep -f app.py)
来源：http://teu.xuetiantiany.cn

[R65] 查看端口占用
来源：http://yce.fengsongda.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kpz.xingfuxueyuan.xyz

[R66] 定时任务
来源：http://jcv.svipenyu.cn

crontab -e;  crontab -l
来源：http://bnd.tian-w.cn

[R67] 生成随机十六进制串
来源：http://lfj.tian-w.cn

openssl rand -hex 16
来源：http://mkd.jinyuanbaomall.cn

[R68] 计算文件校验值
来源：http://ptt.xingfuxueyuan.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://ntz.fktsv.cn

[R69] 生成随机密码
来源：http://rdv.c1oappe.top

head -c 16 /dev/urandom | base64
来源：http://egl.yj20258888.top

[R70] 时间戳与互转
来源：http://vma.aizwys.cn

date +%s;  date -d @1700000000
来源：http://wua.shuidangran.top

[R71] 日期格式化
来源：http://kxf.daria6918.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://pmv.yuxming.cn

[R72] 等待端口就绪
来源：http://wui.xuetiantiany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dng.jianghu66.top

[R73] 分割大日志
来源：http://xuf.yonumen.top

split -l 1000 big.log part_
来源：http://moi.wangdashe.top

[R74] 批量重命名
来源：http://mph.xinyue.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://aoy.cucudq.cn

[R75] 导出环境变量
来源：http://zyr.cucudq.cn

export PATH="$HOME/bin:$PATH"
来源：http://xov.zhengqikj.top

[R76] 使用临时文件
来源：http://pib.sjlbkw.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fsu.svipenyu.cn

[R77] 读取用户输入
来源：http://pqi.hywenlv.cn

read -rp "请输入: " ans
来源：http://ucy.yanxiufei.cn

[R78] 交互式菜单
来源：http://fmj.redwolf501.top

select opt in a b c; do echo "$opt"; break; done
来源：http://dwd.sweek.top

[R79] 解析命令行选项
来源：http://wug.iojbl.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://idq.hfpthk.cn

[R80] 查看脚本执行耗时
来源：http://fdh.xuanzx.com

time ./run.sh
来源：http://efn.shzxlz.cn

================================================================================
来源：http://tow.shzxlz.cn

S. C / C++ 专题
来源：http://mxr.zhoulong.xyz

================================================================================
来源：http://oah.sxryk.cn

[S01] C：Hello World
来源：http://nzm.tanke756.top

#include <stdio.h>
来源：http://nbw.xylfe.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://isl.zdbjq.cn

[S02] C：变量与格式化输出
来源：http://fzn.yonumen.top

int a = 10; printf("%d\n", a);
来源：http://rlu.pycfn.com

[S03] C：读入整数
来源：http://nvn.zhoulong.xyz

int x; scanf("%d", &x);
来源：http://ijh.52xcode.cn

[S04] C：字符串复制
来源：http://hgk.daria6918.cn

char dst[32]; strcpy(dst, "hi");
来源：http://izm.yvedp.cn

[S05] C：字符串长度
来源：http://pzj.jlsjyb.cn

strlen(s)
来源：http://jbk.sweek.top

[S06] C：字符串比较
来源：http://wsb.smart0.xyz

strcmp(a, b) == 0
来源：http://aky.guannengcc.top

[S07] C：数组遍历求和
来源：http://glv.9152youxi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ndu.ehwqpu.com

[S08] C：动态内存分配与释放
来源：http://yww.snrcjt.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jro.xingfuxueyuan.xyz

[S09] C：结构体定义与初始化
来源：http://ide.ydzc1.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://awc.cucudq.cn

[S10] C：指针与解引用
来源：http://bzm.sxryk.cn

int *p = &a;  *p = 5;
来源：http://zto.daria6918.cn

[S11] C：逐行读文件
来源：http://azl.hfpthk.cn

FILE *f = fopen("a.txt", "r");
来源：http://ily.tianlin.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://yhg.xuetiantiany.cn

fclose(f);
来源：http://vod.yj202588.top

[S12] C：写文件
来源：http://umi.jiagoushi.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://djm.aizwys.cn

[S13] C：宏定义
来源：http://pdu.yvedp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wcr.yfazqb.com

[S14] C：枚举
来源：http://oqv.yueranfly.top

enum Color { RED, GREEN, BLUE };
来源：http://hwq.ywan-chungtsiang.top

[S15] C：类型转换
来源：http://dud.jinqigufen.top

(double) a / b
来源：http://diy.cqqwz.cn

[S16] C：位操作置位
来源：http://oec.epnwcf.com

x |= (1 << 3);
来源：http://rrq.xuanzx.com

[S17] C：安全拼接字符串
来源：http://ukb.xylfe.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://aom.sufxvd.cn

[S18] C：命令行参数
来源：http://jdq.ydzc1.top

int main(int argc, char **argv)
来源：http://hys.sweek.top

[S19] C：快速排序
来源：http://mlh.hnqzz.top

qsort(a, n, sizeof(int), cmp);
来源：http://jfe.guannengcc.top

[S20] C：二分查找
来源：http://sou.jinqigfzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wlf.sxryk.cn

[S21] C：字符类别判断
来源：http://wku.shanyushiyangkeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xzf.jqgufenzy.top

[S22] C：字符串转数字
来源：http://dsc.andypj.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://oyd.redwolf501.top

[S23] C：随机数
来源：http://rmx.chenjidiqi.icu

srand(time(NULL));  int r = rand() % 100;
来源：http://yym.tianlin.xyz

[S24] C：获取本地时间
来源：http://dgr.yongpay.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://maa.zdqjudy.top

[S25] C：内存拷贝
来源：http://edk.uphjek.com

memcpy(dst, src, n);
来源：http://tys.zhongyouzk.top

[S26] C：内存清零
来源：http://tiv.9152youxi.cn

memset(a, 0, sizeof a);
来源：http://kna.yueranfly.top

[S27] C：定义常量
来源：http://chx.cashguo.top

const double PI = 3.14159;
来源：http://cty.snrcjt.cn

[S28] C：静态变量
来源：http://dud.nanxinkj.top

static int counter = 0;
来源：http://mht.yuanzhike.top

[S29] C：变参函数
来源：http://swm.iojbl.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vch.dashuyun.cn

[S30] C：头文件保护
来源：http://fgy.guowangkeji.top

#ifndef X_H
来源：http://bnh.jinqigufen.top

#define X_H
来源：http://miw.zhoulong.xyz

#endif
来源：http://btt.xziqi.cn

[S31] C++：Hello World
来源：http://khe.smart0.xyz

#include <iostream>
来源：http://unt.xingfuxueyuan.xyz

int main() { std::cout << "Hello\n"; }
来源：http://epc.xuanzx.com

[S32] C++：字符串
来源：http://xga.mhx1999.top

std::string s = "hi";  s += "!";
来源：http://mwc.yueranfly.top

[S33] C++：vector 增删
来源：http://ovb.gaohongyu789.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ldp.feifeiyinyue.top

[S34] C++：遍历 vector
来源：http://yjz.xingfuxueyuan.xyz

for (auto &x : v) { std::cout << x; }
来源：http://xzx.guannengcc.top

[S35] C++：map
来源：http://qkc.gaohongyu789.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hiu.c1oappe.top

[S36] C++：unordered_map
来源：http://pzi.zhijiandao.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xgh.dianchejie.cn

[S37] C++：set
来源：http://zdt.aizwys.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ydf.meibo888.top

[S38] C++：排序
来源：http://edg.mhx1999.top

std::sort(v.begin(), v.end());
来源：http://gec.daxiang520.top

[S39] C++：自定义比较器排序
来源：http://jxi.shanyushiyangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tds.yongpay.top

[S40] C++：查找元素
来源：http://ugr.hnxiangtu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wju.gaohongyu789.top

[S41] C++：类与构造函数
来源：http://lmp.jianghu66.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mkp.fengsongda.top

[S42] C++：继承与虚函数
来源：http://kal.sysykeji.top

class B : public Base { public: void f() override {} };
来源：http://zxt.zhoulong.xyz

[S43] C++：智能指针
来源：http://pvi.cheryme.top

auto p = std::make_unique<int>(5);
来源：http://jui.xziqi.cn

[S44] C++：引用传参
来源：http://zxy.jlsjyb.cn

void inc(int &x) { ++x; }
来源：http://evx.sjlbkw.cn

[S45] C++：lambda
来源：http://dul.gzhubu.top

auto add = [](int a, int b) { return a + b; };
来源：http://ylu.zhijiandao.cn

[S46] C++：函数模板
来源：http://lwn.c1oappe.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://omj.jianghu66.top

[S47] C++：结构化绑定遍历
来源：http://ufg.fktsv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gvt.tarul.cn

[S48] C++：逐行读文件
来源：http://dki.svipenyu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tml.wangdashe.top

while (std::getline(in, line)) { }
来源：http://xvd.hnxiangtu.top

[S49] C++：写文件
来源：http://zyv.hcnkem.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://inc.bjfxy.top

[S50] C++：格式化数字
来源：http://wfa.vqdsnc.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vht.yj20258888.top

[S51] C++：显式类型转换
来源：http://fqw.aibaodan.cn

static_cast<double>(a) / b
来源：http://iav.cqqwz.cn

[S52] C++：const 与 noexcept
来源：http://lyh.vqdsnc.cn

int size() const noexcept { return n_; }
来源：http://iji.pengpengdd.cyou

[S53] C++：移动语义
来源：http://xph.tarul.cn

std::vector<int> w = std::move(v);
来源：http://ujd.52xcode.cn

[S54] C++：异常处理
来源：http://nwf.kuanghao11.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xnl.yueranfly.top

[S55] C++：结构化绑定
来源：http://xwh.yuxming.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vrk.gogol.net.cn

[S56] C++：optional
来源：http://jxi.jinqigfzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yiy.tarul.cn

[S57] C++：编译期常量
来源：http://jmv.guowangkeji.top

constexpr int N = 10;
来源：http://kua.chenjidiqi.icu

[S58] C++：命名空间
来源：http://rqe.chenlongwang.top

namespace ns { int f() { return 1; } }
来源：http://pxm.bjfxy.top

[S59] C++：静态断言
来源：http://skx.316326.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://scl.cdnleiting.top

[S60] C++：遍历并删除元素
来源：http://nsi.cashguo.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://awf.guowangkeji.top

================================================================================
来源：http://wqh.tian-w.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hoc.gaohongyu789.top

================================================================================
来源：http://kxk.tianlin.xyz

[T01] Kotlin：Hello World
来源：http://zla.xylfe.cn

println("Hello")
来源：http://utn.yfazqb.com

[T02] Kotlin：变量
来源：http://gko.quarkkingdee.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wjm.gogol.net.cn

[T03] Kotlin：字符串模板
来源：http://yra.gzhubu.top

"值: $b"
来源：http://vjl.jqgfzy.top

[T04] Kotlin：空安全
来源：http://ant.sjlbkw.cn

val n: String? = null;  n?.length
来源：http://szg.vehdjk.com

[T05] Kotlin：when 表达式
来源：http://kfe.zhengqikj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ayq.sufxvd.cn

[T06] Kotlin：集合映射
来源：http://gcb.tianlin.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://zqt.epnwcf.com

[T07] Kotlin：集合过滤
来源：http://tyt.vehdjk.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://ube.nanxinkj.top

[T08] Kotlin：数据类
来源：http://njy.ehwqpu.com

data class User(val name: String, val age: Int)
来源：http://pzp.pycfn.com

[T09] Kotlin：扩展函数
来源：http://esn.quarkkingdee.top

fun String.exclaim() = this + "!"
来源：http://obv.nanxinkj.top

[T10] Kotlin：默认参数
来源：http://bzw.0kj1m.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ggb.zhijiandao.cn

[T11] Kotlin：协程
来源：http://rfo.sysykeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://nra.xuanzx.com

[T12] Kotlin：解构声明
来源：http://jmx.bbcook.cn

val (a, b) = Pair(1, 2)
来源：http://gpo.yvedp.cn


<!-- 参考信息 -->