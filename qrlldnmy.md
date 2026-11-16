代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vmc.daria6918.cn

[R10] 正则匹配
来源：http://uwn.tarul.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vlo.chenjidiqi.icu

[R11] case 多分支
来源：http://nyz.wangdashe.top

case "$1" in
来源：http://yxm.zhoulong.xyz

start) echo "启动" ;;
来源：http://ftk.yongpay.top

stop)  echo "停止" ;;
来源：http://ibs.yonumen.top

*)     echo "未知命令" ;;
来源：http://pbn.xuanzx.com

esac
来源：http://fvl.iojbl.cn

[R12] for 遍历文件
来源：http://jwa.tarul.cn

for f in *.txt; do echo "$f"; done
来源：http://qpo.zhiwuduotai.top

[R13] for 计数循环
来源：http://qds.sxryk.cn

for i in {1..10}; do echo "$i"; done
来源：http://dhh.aizwys.cn

[R14] C 风格 for
来源：http://gke.cheryme.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lei.xinyue.icu

[R15] while 逐行读文件
来源：http://iil.jinqigufen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mkm.ydzc1.top

[R16] until 等待条件
来源：http://aak.dashuyun.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vbs.yj20258.top

[R17] 数组定义与取值
来源：http://ouo.mhx1999.top

arr=(a b c); echo "${arr[0]}"
来源：http://jqi.uphjek.com

[R18] 遍历数组
来源：http://mxr.haohaochexian.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ghe.mhx1999.top

[R19] 数组长度
来源：http://ufa.xziqi.cn

echo "${#arr[@]}"
来源：http://lew.hysaishi.cn

[R20] 关联数组（字典）
来源：http://xvc.kuanghao11.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sfg.hfpthk.cn

[R21] 字符串长度
来源：http://wvh.birdmap.top

echo "${#s}"
来源：http://glw.epnwcf.com

[R22] 截取子串
来源：http://zlv.haohaochexian.top

echo "${s:0:5}"
来源：http://oop.gzhubu.top

[R23] 字符串替换
来源：http://ksj.zdbjq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tej.nwbrower.top

[R24] 大小写转换
来源：http://zfy.zhongyouzk.top

echo "${s^^}"; echo "${s,,}"
来源：http://ljc.cdnleiting.top

[R25] 去后缀 / 去前缀
来源：http://deu.gaohongyu789.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://sod.sxryk.cn

[R26] 命令替换
来源：http://omr.jinqigufen.top

now=$(date +%F); echo "$now"
来源：http://qol.hfpthk.cn

[R27] 算术展开
来源：http://lzh.meibo888.top

echo $((1 + 2 * 3))
来源：http://wff.aizwys.cn

[R28] 浮点运算
来源：http://qhj.daxiang520.top

echo "scale=2; 10/3" | bc
来源：http://odl.9152youxi.cn

[R29] 定义函数
来源：http://jga.sjlbkw.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://djk.gaohongyu789.top

[R30] 函数返回状态码
来源：http://ejv.guowangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://jaz.316326.xyz

[R31] 局部变量
来源：http://fdl.feifeiyinyue.top

f() { local x=1; echo "$x"; }
来源：http://czw.ydjk.org.cn

[R32] 参数个数校验
来源：http://mcl.ydzc1.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ucy.hnqzz.top

[R33] 捕获错误并提示行号
来源：http://sll.yanxiufei.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ire.quarkkingdee.top

[R34] 退出时清理
来源：http://pcq.bbcook.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bve.meibo888.top

[R35] 后台执行并等待
来源：http://ipo.hesvh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wch.gzhubu.top

[R36] 并发执行多个任务
来源：http://dsy.kuanghao11.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vvc.zhixingplan.top

[R37] 把输出赋给变量
来源：http://cgc.cheryme.top

files=$(ls -1)
来源：http://bzz.vehdjk.com

[R38] 管道串联
来源：http://okh.ydjk.org.cn

cat a.txt | grep -i error | wc -l
来源：http://feg.shanyushiyangkeji.top

[R39] 重定向标准输出与错误
来源：http://ptv.xylfe.cn

cmd > out.log 2>&1
来源：http://ucn.nanxuanxn.top

[R40] 追加写日志
来源：http://yql.fzhhl.top

echo "log" >> out.log
来源：http://mhq.quarkkingdee.top

[R41] 丢弃输出
来源：http://rnv.hongshengwenyu.top

cmd >/dev/null 2>&1
来源：http://vuk.cheryme.top

[R42] 输入重定向
来源：http://ydn.quarkkingdee.top

wc -l < a.txt
来源：http://csd.jqgufenzy.top

[R43] 按名字查找文件
来源：http://lok.aizwys.cn

find . -name "*.log" -type f
来源：http://oan.yanxiufei.cn

[R44] 按修改时间查找
来源：http://ljj.hfpthk.cn

find . -mtime -7 -type f
来源：http://dul.ydjk.org.cn

[R45] 批量删除
来源：http://rkv.smart0.xyz

find . -name "*.tmp" -delete
来源：http://gau.iojbl.cn

[R46] 递归替换文件内容
来源：http://zqc.jyoumei.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lbg.hongshengwenyu.top

[R47] sed 单行替换
来源：http://crd.gogol.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ruo.wangshuangyany.cn

[R48] awk 取指定列
来源：http://nbj.aizwys.cn

awk '{print $1, $3}' a.txt
来源：http://itd.ybcxt.top

[R49] awk 带条件
来源：http://ugg.cqqwz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rto.nwbrower.top

[R50] awk 求和
来源：http://lzw.shuidangran.top

awk '{s += $2} END {print s}' a.txt
来源：http://tsd.zdbjq.cn

[R51] 排序去重取前几
来源：http://pnm.yangfankeji.com

sort a.txt | uniq -c | sort -rn | head
来源：http://xgb.c1oappe.top

[R52] 统计行数
来源：http://qbo.jlsjyb.cn

wc -l a.txt
来源：http://bms.hywenlv.cn

[R53] 查看文件头与实时尾
来源：http://nij.hnxiangtu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://awp.aibaodan.cn

[R54] 比较两个文件
来源：http://osx.c1oappe.top

diff a.txt b.txt
来源：http://sij.cqqwz.cn

[R55] 压缩与解压
来源：http://dpz.vehdjk.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ogh.jqgufenzy.top

[R56] 远程拷贝
来源：http://jdk.yongpay.top

scp file user@host:/path/
来源：http://aiz.dianchejie.cn

[R57] 远程执行命令
来源：http://buv.aibaodan.cn

ssh user@host 'uptime'
来源：http://tvb.yongpay.top

[R58] 下载文件
来源：http://vpi.xylfe.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rjc.xuetiantiany.cn

[R59] 发 POST JSON
来源：http://yaq.jyoumei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kud.c1oappe.top

[R60] 只看 HTTP 状态码
来源：http://qqt.yuxming.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oyn.feifeiyinyue.top

[R61] 磁盘占用
来源：http://tdm.feifeiyinyue.top

df -h;  du -sh *
来源：http://emz.gzhubu.top

[R62] 找最占空间的文件
来源：http://rju.hfpthk.cn

du -ah . | sort -rh | head -10
来源：http://wwl.fktsv.cn

[R63] 内存与进程
来源：http://bvs.zhiwuduotai.top

free -h;  ps aux | grep nginx
来源：http://tex.wangshuangyany.cn

[R64] 结束进程
来源：http://tqs.tian-w.cn

kill -9 $(pgrep -f app.py)
来源：http://lxu.zhijiandao.cn

[R65] 查看端口占用
来源：http://chi.yj20258888.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tfq.zdqjudy.top

[R66] 定时任务
来源：http://lqa.epnwcf.com

crontab -e;  crontab -l
来源：http://lev.yfazqb.com

[R67] 生成随机十六进制串
来源：http://lih.nanxinkj.top

openssl rand -hex 16
来源：http://xwz.shanyushiyangkeji.top

[R68] 计算文件校验值
来源：http://erx.zhixingplan.top

sha256sum a.txt;  md5sum a.txt
来源：http://jzk.yj202588.top

[R69] 生成随机密码
来源：http://fuq.aibaodan.cn

head -c 16 /dev/urandom | base64
来源：http://vdr.gotoacloud.top

[R70] 时间戳与互转
来源：http://nhl.wangshuangyany.cn

date +%s;  date -d @1700000000
来源：http://unj.316326.xyz

[R71] 日期格式化
来源：http://qpk.bbcook.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ipi.jiagoushi.top

[R72] 等待端口就绪
来源：http://tko.gaohongyu789.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zqr.mhx1999.top

[R73] 分割大日志
来源：http://swm.zhaomingkeji.xyz

split -l 1000 big.log part_
来源：http://dfh.yj20258888.top

[R74] 批量重命名
来源：http://yhv.bbcook.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rrc.gogol.net.cn

[R75] 导出环境变量
来源：http://ueq.zhaomingkeji.xyz

export PATH="$HOME/bin:$PATH"
来源：http://oto.zhixingplan.top

[R76] 使用临时文件
来源：http://ogz.hnqzz.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zzn.fengsongda.top

[R77] 读取用户输入
来源：http://sfr.fengsongda.top

read -rp "请输入: " ans
来源：http://zky.quarkkingdee.top

[R78] 交互式菜单
来源：http://jaq.yangfankeji.com

select opt in a b c; do echo "$opt"; break; done
来源：http://snr.xuetiantiany.cn

[R79] 解析命令行选项
来源：http://rce.shangyingyoupin.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hnk.meibo888.top

[R80] 查看脚本执行耗时
来源：http://gnr.xuanzx.com

time ./run.sh
来源：http://fjk.cucudq.cn

================================================================================
来源：http://xrk.xziqi.cn

S. C / C++ 专题
来源：http://oss.9152youxi.cn

================================================================================
来源：http://pvg.chenjidiqi.icu

[S01] C：Hello World
来源：http://ruy.nanxinkj.top

#include <stdio.h>
来源：http://kaj.jinyuanbaomall.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://inz.jyoumei.cn

[S02] C：变量与格式化输出
来源：http://anh.jlsjyb.cn

int a = 10; printf("%d\n", a);
来源：http://twk.bjfxy.top

[S03] C：读入整数
来源：http://fiz.xinyue.icu

int x; scanf("%d", &x);
来源：http://umh.jinqigufen.top

[S04] C：字符串复制
来源：http://fyj.52xcode.cn

char dst[32]; strcpy(dst, "hi");
来源：http://psj.ppjwa.cn

[S05] C：字符串长度
来源：http://fju.ybcxt.top

strlen(s)
来源：http://rnq.zhiwuduotai.top

[S06] C：字符串比较
来源：http://gia.cheryme.top

strcmp(a, b) == 0
来源：http://onj.cheryme.top

[S07] C：数组遍历求和
来源：http://nyr.daria6918.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fdw.tianlin.xyz

[S08] C：动态内存分配与释放
来源：http://kjs.jianghu66.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jiw.fengsongda.top

[S09] C：结构体定义与初始化
来源：http://obi.gaohongyu789.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vvn.ydjk.org.cn

[S10] C：指针与解引用
来源：http://hji.xuetiantiany.cn

int *p = &a;  *p = 5;
来源：http://flu.nwbrower.top

[S11] C：逐行读文件
来源：http://fwt.xuetiantiany.cn

FILE *f = fopen("a.txt", "r");
来源：http://srh.redwolf501.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ehe.guannengcc.top

fclose(f);
来源：http://ufu.jyoumei.cn

[S12] C：写文件
来源：http://wlx.fktsv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zhh.fzhhl.top

[S13] C：宏定义
来源：http://xjx.nanxuanxn.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lym.mhx1999.top

[S14] C：枚举
来源：http://sxx.nanxinkj.top

enum Color { RED, GREEN, BLUE };
来源：http://mhk.tianlin.xyz

[S15] C：类型转换
来源：http://xob.jianghu66.top

(double) a / b
来源：http://mna.gzhubu.top

[S16] C：位操作置位
来源：http://ram.cdnleiting.top

x |= (1 << 3);
来源：http://ljl.tianlin.xyz

[S17] C：安全拼接字符串
来源：http://eeh.zhiwuduotai.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pcc.nanxinkj.top

[S18] C：命令行参数
来源：http://dzd.chenzaomai.com

int main(int argc, char **argv)
来源：http://bsd.fktsv.cn

[S19] C：快速排序
来源：http://aqq.uphjek.com

qsort(a, n, sizeof(int), cmp);
来源：http://zbz.jqgfzy.top

[S20] C：二分查找
来源：http://fsy.shanyushiyangtech.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tat.bjfxy.top

[S21] C：字符类别判断
来源：http://ndo.sweek.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jzf.hcnkem.com

[S22] C：字符串转数字
来源：http://eef.0kj1m.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lcy.kuanghao11.cn

[S23] C：随机数
来源：http://vet.sufxvd.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dfm.aizwys.cn

[S24] C：获取本地时间
来源：http://fgu.xziqi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rrw.hcnkem.com

[S25] C：内存拷贝
来源：http://dnn.shanyushiyangtech.top

memcpy(dst, src, n);
来源：http://ary.havefunace.top

[S26] C：内存清零
来源：http://xfx.snrcjt.cn

memset(a, 0, sizeof a);
来源：http://sde.haohaochexian.top

[S27] C：定义常量
来源：http://yex.dianchejie.cn

const double PI = 3.14159;
来源：http://ewn.jinqigfzy.top

[S28] C：静态变量
来源：http://usx.c1oappe.top

static int counter = 0;
来源：http://tgr.redwolf501.top

[S29] C：变参函数
来源：http://lvx.ppjwa.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kwr.jinqigufen.top

[S30] C：头文件保护
来源：http://myo.iojbl.cn

#ifndef X_H
来源：http://kmm.hfpthk.cn

#define X_H
来源：http://tau.nwbrower.top

#endif
来源：http://myd.yj202588.top

[S31] C++：Hello World
来源：http://dtd.hcnkem.com

#include <iostream>
来源：http://qga.guowangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://qlr.jqgufenzy.top

[S32] C++：字符串
来源：http://hce.ehwqpu.com

std::string s = "hi";  s += "!";
来源：http://iqm.shanyushiyangkeji.top

[S33] C++：vector 增删
来源：http://vfj.zhoulong.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ion.hnqzz.top

[S34] C++：遍历 vector
来源：http://bmo.ppjwa.cn

for (auto &x : v) { std::cout << x; }
来源：http://dyx.zhiwuduotai.top

[S35] C++：map
来源：http://qik.jianghu66.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qfr.fengsongda.top

[S36] C++：unordered_map
来源：http://tub.jiagoushi.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wzg.cucudq.cn

[S37] C++：set
来源：http://qzy.mhx1999.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://usg.ybcxt.top

[S38] C++：排序
来源：http://vba.chenlongwang.top

std::sort(v.begin(), v.end());
来源：http://gba.yanxiufei.cn

[S39] C++：自定义比较器排序
来源：http://apw.zycfv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://shc.52xcode.cn

[S40] C++：查找元素
来源：http://wbn.zhoulong.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://has.xylfe.cn

[S41] C++：类与构造函数
来源：http://azv.hesvh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ayd.daxiang520.top

[S42] C++：继承与虚函数
来源：http://vma.svipenyu.cn

class B : public Base { public: void f() override {} };
来源：http://spr.yvedp.cn

[S43] C++：智能指针
来源：http://muf.ydzc1.top

auto p = std::make_unique<int>(5);
来源：http://epm.hnqzz.top

[S44] C++：引用传参
来源：http://mlx.jyoumei.cn

void inc(int &x) { ++x; }
来源：http://rzh.snrcjt.cn

[S45] C++：lambda
来源：http://ufr.yj20258.top

auto add = [](int a, int b) { return a + b; };
来源：http://gww.fengsongda.top

[S46] C++：函数模板
来源：http://hjz.feifeiyinyue.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://flz.nanxinkj.top

[S47] C++：结构化绑定遍历
来源：http://vzq.zdqjudy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://swm.haohaochexian.top

[S48] C++：逐行读文件
来源：http://mbl.c1oappe.top

std::ifstream in("a.txt");  std::string line;
来源：http://aet.nwbrower.top

while (std::getline(in, line)) { }
来源：http://nmp.fzhhl.top

[S49] C++：写文件
来源：http://ifo.dashuyun.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zse.hysaishi.cn

[S50] C++：格式化数字
来源：http://fwh.hnqzz.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://znh.tianlin.xyz

[S51] C++：显式类型转换
来源：http://yyf.jinqigfzy.top

static_cast<double>(a) / b
来源：http://xdo.fanxiaobao.xyz

[S52] C++：const 与 noexcept
来源：http://umy.vehdjk.com

int size() const noexcept { return n_; }
来源：http://mzq.fengsongda.top

[S53] C++：移动语义
来源：http://okm.shanyushiyangkeji.top

std::vector<int> w = std::move(v);
来源：http://qyp.gzhubu.top

[S54] C++：异常处理
来源：http://lsy.ydjk.org.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://iqo.hcnkem.com

[S55] C++：结构化绑定
来源：http://awc.gogol.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vtq.sxryk.cn

[S56] C++：optional
来源：http://wfh.mhx1999.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://apv.cashguo.top

[S57] C++：编译期常量
来源：http://grn.ppjwa.cn

constexpr int N = 10;
来源：http://zsf.jqgfzy.top

[S58] C++：命名空间
来源：http://aki.xinyue.icu

namespace ns { int f() { return 1; } }
来源：http://fya.ehwqpu.com

[S59] C++：静态断言
来源：http://zhe.jiagoushi.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bgi.bjfxy.top

[S60] C++：遍历并删除元素
来源：http://vjg.guannengcc.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tsu.svipenyu.cn

================================================================================
来源：http://slv.sysykeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://afm.chenzaomai.com

================================================================================
来源：http://anz.0kj1m.cn

[T01] Kotlin：Hello World
来源：http://ydz.yongpay.top

println("Hello")
来源：http://cza.zhixingplan.top

[T02] Kotlin：变量
来源：http://vvy.hongshengwenyu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mbt.hywenlv.cn

[T03] Kotlin：字符串模板
来源：http://wbk.zhoulong.xyz

"值: $b"
来源：http://cuk.haohaochexian.top

[T04] Kotlin：空安全
来源：http://rce.fzhhl.top

val n: String? = null;  n?.length
来源：http://eaw.redwolf501.top

[T05] Kotlin：when 表达式
来源：http://bqa.9152youxi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://van.chenzaomai.com

[T06] Kotlin：集合映射
来源：http://gpz.jinyuanbaomall.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rmd.ywan-chungtsiang.top

[T07] Kotlin：集合过滤
来源：http://kin.yj202588.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ara.gzhubu.top

[T08] Kotlin：数据类
来源：http://ukv.feifeiyinyue.top

data class User(val name: String, val age: Int)
来源：http://cta.xuanzx.com

[T09] Kotlin：扩展函数
来源：http://myx.kuanghao11.cn

fun String.exclaim() = this + "!"
来源：http://uvc.epnwcf.com

[T10] Kotlin：默认参数
来源：http://qyi.tianlin.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://iin.9152youxi.cn


<!-- 参考信息 -->