代发 wailian999

case "$1" in
来源：http://fso.yuanzhike.top

start) echo "启动" ;;
来源：http://tmb.feifeiyinyue.top

stop)  echo "停止" ;;
来源：http://xyq.sweek.top

*)     echo "未知命令" ;;
来源：http://xdu.tian-w.cn

esac
来源：http://hfx.ywan-chungtsiang.top

[R12] for 遍历文件
来源：http://cty.cheryme.top

for f in *.txt; do echo "$f"; done
来源：http://rpm.pycfn.com

[R13] for 计数循环
来源：http://lry.vqdsnc.cn

for i in {1..10}; do echo "$i"; done
来源：http://qgk.tanke756.top

[R14] C 风格 for
来源：http://ayh.chenzaomai.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nds.zycfv.cn

[R15] while 逐行读文件
来源：http://rre.snrcjt.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zbn.nwbrower.top

[R16] until 等待条件
来源：http://arb.yuxming.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qwy.jyoumei.cn

[R17] 数组定义与取值
来源：http://mlb.pycfn.com

arr=(a b c); echo "${arr[0]}"
来源：http://nzk.chenlongwang.top

[R18] 遍历数组
来源：http://hro.chenjidiqi.icu

for x in "${arr[@]}"; do echo "$x"; done
来源：http://asa.hongshengwenyu.top

[R19] 数组长度
来源：http://mpg.yvedp.cn

echo "${#arr[@]}"
来源：http://dgn.cdnleiting.top

[R20] 关联数组（字典）
来源：http://ntv.chenjidiqi.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nvg.yonumen.top

[R21] 字符串长度
来源：http://baj.aizwys.cn

echo "${#s}"
来源：http://irf.havefunace.top

[R22] 截取子串
来源：http://zev.jlsjyb.cn

echo "${s:0:5}"
来源：http://wsp.jinghuilouyu.cn

[R23] 字符串替换
来源：http://sym.yanxiufei.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vie.guowangkeji.top

[R24] 大小写转换
来源：http://vep.xziqi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tes.jinqigfzy.top

[R25] 去后缀 / 去前缀
来源：http://yxe.xuanzx.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://wvg.snrcjt.cn

[R26] 命令替换
来源：http://pzj.yueranfly.top

now=$(date +%F); echo "$now"
来源：http://xik.ydjk.org.cn

[R27] 算术展开
来源：http://frx.chenlongwang.top

echo $((1 + 2 * 3))
来源：http://txy.jianghu66.top

[R28] 浮点运算
来源：http://vhv.sxryk.cn

echo "scale=2; 10/3" | bc
来源：http://ysv.shzxlz.cn

[R29] 定义函数
来源：http://gnu.hnqzz.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uah.xinyue.icu

[R30] 函数返回状态码
来源：http://zqj.wangdashe.top

f() { return 0; }; f || echo "失败了"
来源：http://tbx.fktsv.cn

[R31] 局部变量
来源：http://vwh.tarul.cn

f() { local x=1; echo "$x"; }
来源：http://acy.zhengqikj.top

[R32] 参数个数校验
来源：http://zvy.daria6918.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qcf.sweek.top

[R33] 捕获错误并提示行号
来源：http://rrt.shzxlz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://aop.epnwcf.com

[R34] 退出时清理
来源：http://rwa.dashuyun.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nqn.snrcjt.cn

[R35] 后台执行并等待
来源：http://xpb.yuanzhike.top

sleep 5 & pid=$!; wait "$pid"
来源：http://itt.fengsongda.top

[R36] 并发执行多个任务
来源：http://rxw.yuanzhike.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pqm.sysykeji.top

[R37] 把输出赋给变量
来源：http://yww.tianlin.xyz

files=$(ls -1)
来源：http://xtx.chenjidiqi.icu

[R38] 管道串联
来源：http://olb.zhoulong.xyz

cat a.txt | grep -i error | wc -l
来源：http://per.haohaochexian.top

[R39] 重定向标准输出与错误
来源：http://tlz.52xcode.cn

cmd > out.log 2>&1
来源：http://kns.jlsjyb.cn

[R40] 追加写日志
来源：http://vdw.aibaodan.cn

echo "log" >> out.log
来源：http://psn.zhixingplan.top

[R41] 丢弃输出
来源：http://tpc.smart0.xyz

cmd >/dev/null 2>&1
来源：http://rtu.nanxuanxn.top

[R42] 输入重定向
来源：http://kwm.yanxiufei.cn

wc -l < a.txt
来源：http://jyc.tian-w.cn

[R43] 按名字查找文件
来源：http://ufz.jianghu66.top

find . -name "*.log" -type f
来源：http://low.xuanzx.com

[R44] 按修改时间查找
来源：http://mhi.feifeiyinyue.top

find . -mtime -7 -type f
来源：http://zaf.tian-w.cn

[R45] 批量删除
来源：http://fza.ppjwa.cn

find . -name "*.tmp" -delete
来源：http://bwz.guannengcc.top

[R46] 递归替换文件内容
来源：http://ava.yongpay.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cai.ehwqpu.com

[R47] sed 单行替换
来源：http://nkq.ywan-chungtsiang.top

sed -i 's/foo/bar/g' a.txt
来源：http://ovk.chenjidiqi.icu

[R48] awk 取指定列
来源：http://efz.jqgfzy.top

awk '{print $1, $3}' a.txt
来源：http://vtx.hywenlv.cn

[R49] awk 带条件
来源：http://gyr.yj20258888.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qrf.52xcode.cn

[R50] awk 求和
来源：http://rey.hywenlv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bxc.yangfankeji.com

[R51] 排序去重取前几
来源：http://smo.zhiwuduotai.top

sort a.txt | uniq -c | sort -rn | head
来源：http://zwt.vehdjk.com

[R52] 统计行数
来源：http://opp.jianghu66.top

wc -l a.txt
来源：http://hvb.9152youxi.cn

[R53] 查看文件头与实时尾
来源：http://wcb.yj202588.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wav.jinqigufen.top

[R54] 比较两个文件
来源：http://pwm.jinyuanbaomall.cn

diff a.txt b.txt
来源：http://qth.hnqzz.top

[R55] 压缩与解压
来源：http://dij.jianghu66.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wsm.cheryme.top

[R56] 远程拷贝
来源：http://mfm.iojbl.cn

scp file user@host:/path/
来源：http://ptz.shzxlz.cn

[R57] 远程执行命令
来源：http://nit.yueranfly.top

ssh user@host 'uptime'
来源：http://pxz.sjlbkw.cn

[R58] 下载文件
来源：http://hoh.svipenyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://acg.chenjidiqi.icu

[R59] 发 POST JSON
来源：http://tdy.yueranfly.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wfu.zhoulong.xyz

[R60] 只看 HTTP 状态码
来源：http://caj.chenzaomai.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qqa.cashguo.top

[R61] 磁盘占用
来源：http://yyf.ybcxt.top

df -h;  du -sh *
来源：http://wrz.cheryme.top

[R62] 找最占空间的文件
来源：http://pcv.nanxuanxn.top

du -ah . | sort -rh | head -10
来源：http://aur.xylfe.cn

[R63] 内存与进程
来源：http://qfe.birdmap.top

free -h;  ps aux | grep nginx
来源：http://xlr.yvedp.cn

[R64] 结束进程
来源：http://okg.chenzaomai.com

kill -9 $(pgrep -f app.py)
来源：http://yyi.jinyuanbaomall.cn

[R65] 查看端口占用
来源：http://rjt.hnxiangtu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yxw.ydzc1.top

[R66] 定时任务
来源：http://edq.birdmap.top

crontab -e;  crontab -l
来源：http://dcr.ywan-chungtsiang.top

[R67] 生成随机十六进制串
来源：http://gta.xylfe.cn

openssl rand -hex 16
来源：http://wwu.hammf.cn

[R68] 计算文件校验值
来源：http://kyl.wangdashe.top

sha256sum a.txt;  md5sum a.txt
来源：http://gdx.hnqzz.top

[R69] 生成随机密码
来源：http://trh.xziqi.cn

head -c 16 /dev/urandom | base64
来源：http://gsr.zhoulong.xyz

[R70] 时间戳与互转
来源：http://vpz.hfpthk.cn

date +%s;  date -d @1700000000
来源：http://wdx.yueranfly.top

[R71] 日期格式化
来源：http://iiv.jyoumei.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dri.zhaomingkeji.xyz

[R72] 等待端口就绪
来源：http://mgx.yj202588.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nok.yuxming.cn

[R73] 分割大日志
来源：http://bkx.hnxiangtu.top

split -l 1000 big.log part_
来源：http://fbq.zhixingplan.top

[R74] 批量重命名
来源：http://ooq.shangyingyoupin.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pdr.shzxlz.cn

[R75] 导出环境变量
来源：http://sey.xuetiantiany.cn

export PATH="$HOME/bin:$PATH"
来源：http://upg.ppjwa.cn

[R76] 使用临时文件
来源：http://uei.iojbl.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yug.hcnkem.com

[R77] 读取用户输入
来源：http://dkr.mhx1999.top

read -rp "请输入: " ans
来源：http://rkn.sjlbkw.cn

[R78] 交互式菜单
来源：http://moa.jlsjyb.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bcw.ybcxt.top

[R79] 解析命令行选项
来源：http://spx.cucudq.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://apj.hysaishi.cn

[R80] 查看脚本执行耗时
来源：http://nrz.yuanzhike.top

time ./run.sh
来源：http://agv.dashuyun.cn

================================================================================
来源：http://iyf.jiagoushi.top

S. C / C++ 专题
来源：http://nki.ctjpmb.com

================================================================================
来源：http://dnb.kuanghao11.cn

[S01] C：Hello World
来源：http://tvw.iojbl.cn

#include <stdio.h>
来源：http://gjd.fengsongda.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://hqm.yvedp.cn

[S02] C：变量与格式化输出
来源：http://tgl.jinqigufen.top

int a = 10; printf("%d\n", a);
来源：http://cbp.hysaishi.cn

[S03] C：读入整数
来源：http://rhn.tarul.cn

int x; scanf("%d", &x);
来源：http://yzy.fanxiaobao.xyz

[S04] C：字符串复制
来源：http://ikb.ywan-chungtsiang.top

char dst[32]; strcpy(dst, "hi");
来源：http://hat.jinyuanbaomall.cn

[S05] C：字符串长度
来源：http://qqz.shzxlz.cn

strlen(s)
来源：http://ipn.jinyuanbaomall.cn

[S06] C：字符串比较
来源：http://ycg.ehwqpu.com

strcmp(a, b) == 0
来源：http://rgb.dashuyun.cn

[S07] C：数组遍历求和
来源：http://pxr.smart0.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wpp.jyoumei.cn

[S08] C：动态内存分配与释放
来源：http://tdg.hywenlv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ldg.sufxvd.cn

[S09] C：结构体定义与初始化
来源：http://elp.shangyingyoupin.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mbc.shangyingyoupin.top

[S10] C：指针与解引用
来源：http://kta.zycfv.cn

int *p = &a;  *p = 5;
来源：http://epr.zhaomingkeji.xyz

[S11] C：逐行读文件
来源：http://gbn.zhoulong.xyz

FILE *f = fopen("a.txt", "r");
来源：http://brd.aibaodan.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ysa.fktsv.cn

fclose(f);
来源：http://fgl.gzhubu.top

[S12] C：写文件
来源：http://elh.quarkkingdee.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zxf.xinyue.icu

[S13] C：宏定义
来源：http://qim.pycfn.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://opp.sxryk.cn

[S14] C：枚举
来源：http://jey.havefunace.top

enum Color { RED, GREEN, BLUE };
来源：http://zcu.mhx1999.top

[S15] C：类型转换
来源：http://cbu.cashguo.top

(double) a / b
来源：http://tvi.52xcode.cn

[S16] C：位操作置位
来源：http://kfs.sxryk.cn

x |= (1 << 3);
来源：http://rxq.ppjwa.cn

[S17] C：安全拼接字符串
来源：http://vog.316326.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jkx.havefunace.top

[S18] C：命令行参数
来源：http://pcq.gaohongyu789.top

int main(int argc, char **argv)
来源：http://aak.fktsv.cn

[S19] C：快速排序
来源：http://qrq.smart0.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://ttq.shanyushiyangtech.top

[S20] C：二分查找
来源：http://gez.wangshuangyany.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://swu.tianlin.xyz

[S21] C：字符类别判断
来源：http://wng.wangshuangyany.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kbe.yuanzhike.top

[S22] C：字符串转数字
来源：http://hhn.hongshengwenyu.top

atoi("42");  strtod("3.14", NULL);
来源：http://ivf.shangyingyoupin.top

[S23] C：随机数
来源：http://sab.gotoacloud.top

srand(time(NULL));  int r = rand() % 100;
来源：http://lcu.0kj1m.cn

[S24] C：获取本地时间
来源：http://viu.zhijiandao.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lgj.daria6918.cn

[S25] C：内存拷贝
来源：http://erc.hongshengwenyu.top

memcpy(dst, src, n);
来源：http://lqy.fktsv.cn

[S26] C：内存清零
来源：http://lww.xuetiantiany.cn

memset(a, 0, sizeof a);
来源：http://teo.yangfankeji.com

[S27] C：定义常量
来源：http://syj.yongpay.top

const double PI = 3.14159;
来源：http://izt.pycfn.com

[S28] C：静态变量
来源：http://qnw.xinyue.icu

static int counter = 0;
来源：http://ylj.birdmap.top

[S29] C：变参函数
来源：http://qxj.bjfxy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ypy.yj20258888.top

[S30] C：头文件保护
来源：http://rvb.jyoumei.cn

#ifndef X_H
来源：http://utj.c1oappe.top

#define X_H
来源：http://kly.quarkkingdee.top

#endif
来源：http://kvo.yangfankeji.com

[S31] C++：Hello World
来源：http://aku.zhoulong.xyz

#include <iostream>
来源：http://zym.tarul.cn

int main() { std::cout << "Hello\n"; }
来源：http://uve.aizwys.cn

[S32] C++：字符串
来源：http://qur.hcnkem.com

std::string s = "hi";  s += "!";
来源：http://qub.zdqjudy.top

[S33] C++：vector 增删
来源：http://jqa.redwolf501.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jyn.tianlin.xyz

[S34] C++：遍历 vector
来源：http://ksz.shanyushiyangkeji.top

for (auto &x : v) { std::cout << x; }
来源：http://oat.316326.xyz

[S35] C++：map
来源：http://fho.tianlin.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gra.xuanzx.com

[S36] C++：unordered_map
来源：http://ulg.fengsongda.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yts.jinghuilouyu.cn

[S37] C++：set
来源：http://zjk.tarul.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://aew.jinqigufen.top

[S38] C++：排序
来源：http://hbx.bjfxy.top

std::sort(v.begin(), v.end());
来源：http://feg.tanke756.top

[S39] C++：自定义比较器排序
来源：http://laq.epnwcf.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tdf.tarul.cn

[S40] C++：查找元素
来源：http://ype.gaohongyu789.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ijp.cucudq.cn

[S41] C++：类与构造函数
来源：http://nfx.cdnleiting.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tmj.snrcjt.cn

[S42] C++：继承与虚函数
来源：http://jms.xingfuxueyuan.xyz

class B : public Base { public: void f() override {} };
来源：http://ksd.uphjek.com

[S43] C++：智能指针
来源：http://gft.zhijiandao.cn

auto p = std::make_unique<int>(5);
来源：http://jse.ivvv.top

[S44] C++：引用传参
来源：http://epk.epnwcf.com

void inc(int &x) { ++x; }
来源：http://erp.tanke756.top

[S45] C++：lambda
来源：http://dft.zhongyouzk.top

auto add = [](int a, int b) { return a + b; };
来源：http://sdf.gaohongyu789.top

[S46] C++：函数模板
来源：http://usb.smart0.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://axh.uphjek.com

[S47] C++：结构化绑定遍历
来源：http://irq.jinghuilouyu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lzd.316326.xyz

[S48] C++：逐行读文件
来源：http://cnb.fanxiaobao.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://hno.sufxvd.cn

while (std::getline(in, line)) { }
来源：http://vuj.yj20258888.top

[S49] C++：写文件
来源：http://rxi.cqqwz.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://twx.chenlongwang.top

[S50] C++：格式化数字
来源：http://guf.cqqwz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nki.hnqzz.top

[S51] C++：显式类型转换
来源：http://jgl.tianlin.xyz

static_cast<double>(a) / b
来源：http://eqa.ybcxt.top

[S52] C++：const 与 noexcept
来源：http://bvt.xylfe.cn

int size() const noexcept { return n_; }
来源：http://xtq.shzxlz.cn

[S53] C++：移动语义
来源：http://bpe.zhoulong.xyz

std::vector<int> w = std::move(v);
来源：http://qnr.wangdashe.top

[S54] C++：异常处理
来源：http://rty.ywan-chungtsiang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://iif.andypj.xyz

[S55] C++：结构化绑定
来源：http://mzh.snrcjt.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://psm.nanxinkj.top

[S56] C++：optional
来源：http://bkr.fengsongda.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vrw.gotoacloud.top

[S57] C++：编译期常量
来源：http://ptd.jyoumei.cn

constexpr int N = 10;
来源：http://kkw.ivvv.top

[S58] C++：命名空间
来源：http://dxq.ivvv.top

namespace ns { int f() { return 1; } }
来源：http://bfh.zhengqikj.top

[S59] C++：静态断言
来源：http://pae.ppjwa.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hwo.jiagoushi.top

[S60] C++：遍历并删除元素
来源：http://ekw.xinyue.icu

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qkw.dashuyun.cn

================================================================================
来源：http://ytc.xuanzx.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bqw.andypj.xyz

================================================================================
来源：http://fcl.52xcode.cn

[T01] Kotlin：Hello World
来源：http://els.zhongyouzk.top

println("Hello")
来源：http://bnj.hesvh.cn

[T02] Kotlin：变量
来源：http://ogj.yuxming.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kkl.andypj.xyz

[T03] Kotlin：字符串模板
来源：http://hgq.havefunace.top

"值: $b"
来源：http://ikp.fzhhl.top

[T04] Kotlin：空安全
来源：http://vfo.jqgfzy.top

val n: String? = null;  n?.length
来源：http://jim.sweek.top

[T05] Kotlin：when 表达式
来源：http://frd.dianchejie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lsz.guowangkeji.top

[T06] Kotlin：集合映射
来源：http://res.yuanzhike.top

listOf(1, 2, 3).map { it * 2 }
来源：http://gcg.aizwys.cn

[T07] Kotlin：集合过滤
来源：http://kkq.fehbvm.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://tgs.xingfuxueyuan.xyz

[T08] Kotlin：数据类
来源：http://iky.fzhhl.top

data class User(val name: String, val age: Int)
来源：http://mee.yfazqb.com

[T09] Kotlin：扩展函数
来源：http://kfc.svipenyu.cn

fun String.exclaim() = this + "!"
来源：http://atn.yongpay.top

[T10] Kotlin：默认参数
来源：http://aaj.havefunace.top

fun greet(name: String = "World") = "Hi $name"
来源：http://sbb.tianlin.xyz

[T11] Kotlin：协程
来源：http://wua.cqqwz.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ark.wangshuangyany.cn

[T12] Kotlin：解构声明
来源：http://xzv.hammf.cn

val (a, b) = Pair(1, 2)
来源：http://rkx.zdbjq.cn


<!-- 参考信息 -->