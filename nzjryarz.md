代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ren.shuidangran.top

[R10] 正则匹配
来源：http://onj.dashuyun.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dew.nanxuanxn.top

[R11] case 多分支
来源：http://jhc.yj20258888.top

case "$1" in
来源：http://wqc.zycfv.cn

start) echo "启动" ;;
来源：http://gwj.yuanzhike.top

stop)  echo "停止" ;;
来源：http://wst.gogol.net.cn

*)     echo "未知命令" ;;
来源：http://dhi.hongshengwenyu.top

esac
来源：http://plg.sufxvd.cn

[R12] for 遍历文件
来源：http://zgl.nanxinkj.top

for f in *.txt; do echo "$f"; done
来源：http://oko.hammf.cn

[R13] for 计数循环
来源：http://eow.vqdsnc.cn

for i in {1..10}; do echo "$i"; done
来源：http://cfo.zhaomingkeji.xyz

[R14] C 风格 for
来源：http://pis.c1oappe.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://doo.zhoulong.xyz

[R15] while 逐行读文件
来源：http://mzf.uphjek.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://utu.guowangkeji.top

[R16] until 等待条件
来源：http://awk.yuxming.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rqt.shangyingyoupin.top

[R17] 数组定义与取值
来源：http://nng.316326.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://kvk.pycfn.com

[R18] 遍历数组
来源：http://bkm.ctjpmb.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tie.sufxvd.cn

[R19] 数组长度
来源：http://soq.c1oappe.top

echo "${#arr[@]}"
来源：http://tnu.hywenlv.cn

[R20] 关联数组（字典）
来源：http://paw.ppjwa.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uos.redwolf501.top

[R21] 字符串长度
来源：http://gbh.dashuyun.cn

echo "${#s}"
来源：http://rlr.xuanzx.com

[R22] 截取子串
来源：http://ohb.guannengcc.top

echo "${s:0:5}"
来源：http://bfn.cheryme.top

[R23] 字符串替换
来源：http://apj.meibo888.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ome.ydjk.org.cn

[R24] 大小写转换
来源：http://hjh.0kj1m.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ego.yj20258.top

[R25] 去后缀 / 去前缀
来源：http://dlt.jiagoushi.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://jps.sxryk.cn

[R26] 命令替换
来源：http://lar.meibo888.top

now=$(date +%F); echo "$now"
来源：http://lec.snrcjt.cn

[R27] 算术展开
来源：http://qvn.xziqi.cn

echo $((1 + 2 * 3))
来源：http://rdl.hammf.cn

[R28] 浮点运算
来源：http://ier.vqdsnc.cn

echo "scale=2; 10/3" | bc
来源：http://qmw.vqdsnc.cn

[R29] 定义函数
来源：http://cct.yonumen.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zps.iojbl.cn

[R30] 函数返回状态码
来源：http://huh.zhixingplan.top

f() { return 0; }; f || echo "失败了"
来源：http://qnq.shanyushiyangtech.top

[R31] 局部变量
来源：http://bon.yonumen.top

f() { local x=1; echo "$x"; }
来源：http://muk.jianghu66.top

[R32] 参数个数校验
来源：http://pov.fktsv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://osd.shzxlz.cn

[R33] 捕获错误并提示行号
来源：http://jbg.zdbjq.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hvy.svipenyu.cn

[R34] 退出时清理
来源：http://orq.daxiang520.top

trap 'rm -f "$tmp"' EXIT
来源：http://usl.fktsv.cn

[R35] 后台执行并等待
来源：http://cyv.yuanzhike.top

sleep 5 & pid=$!; wait "$pid"
来源：http://bpr.andypj.xyz

[R36] 并发执行多个任务
来源：http://bkv.ybcxt.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wqu.tian-w.cn

[R37] 把输出赋给变量
来源：http://xkj.andypj.xyz

files=$(ls -1)
来源：http://owb.zhijiandao.cn

[R38] 管道串联
来源：http://lyx.xuetiantiany.cn

cat a.txt | grep -i error | wc -l
来源：http://xyb.sysykeji.top

[R39] 重定向标准输出与错误
来源：http://duc.yonumen.top

cmd > out.log 2>&1
来源：http://huc.gzhubu.top

[R40] 追加写日志
来源：http://bfc.yj202588.top

echo "log" >> out.log
来源：http://lar.aibaodan.cn

[R41] 丢弃输出
来源：http://jvh.shanyushiyangtech.top

cmd >/dev/null 2>&1
来源：http://ywc.sxryk.cn

[R42] 输入重定向
来源：http://ilw.yj202588.top

wc -l < a.txt
来源：http://rzz.sufxvd.cn

[R43] 按名字查找文件
来源：http://exk.zdqjudy.top

find . -name "*.log" -type f
来源：http://yez.yj20258.top

[R44] 按修改时间查找
来源：http://ukf.jiagoushi.top

find . -mtime -7 -type f
来源：http://trr.zhaomingkeji.xyz

[R45] 批量删除
来源：http://dpb.jyoumei.cn

find . -name "*.tmp" -delete
来源：http://kpp.hfpthk.cn

[R46] 递归替换文件内容
来源：http://knr.zhongyouzk.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fse.fzhhl.top

[R47] sed 单行替换
来源：http://rcv.iojbl.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zmz.dashuyun.cn

[R48] awk 取指定列
来源：http://yij.jqgufenzy.top

awk '{print $1, $3}' a.txt
来源：http://ppz.ppjwa.cn

[R49] awk 带条件
来源：http://vfv.zhijiandao.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lqe.hywenlv.cn

[R50] awk 求和
来源：http://dil.vqdsnc.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pma.tian-w.cn

[R51] 排序去重取前几
来源：http://fnb.snrcjt.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jmp.dashuyun.cn

[R52] 统计行数
来源：http://slp.guowangkeji.top

wc -l a.txt
来源：http://oee.yj202588.top

[R53] 查看文件头与实时尾
来源：http://etr.shzxlz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tmv.ybcxt.top

[R54] 比较两个文件
来源：http://tvl.tanke756.top

diff a.txt b.txt
来源：http://yny.fktsv.cn

[R55] 压缩与解压
来源：http://zrx.smart0.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jdf.c1oappe.top

[R56] 远程拷贝
来源：http://tlm.52xcode.cn

scp file user@host:/path/
来源：http://njn.cashguo.top

[R57] 远程执行命令
来源：http://xen.yj20258.top

ssh user@host 'uptime'
来源：http://mcu.jinyuanbaomall.cn

[R58] 下载文件
来源：http://nuy.chenzaomai.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nai.zhiwuduotai.top

[R59] 发 POST JSON
来源：http://rsk.cashguo.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://crt.hysaishi.cn

[R60] 只看 HTTP 状态码
来源：http://nmy.fzhhl.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uyx.gotoacloud.top

[R61] 磁盘占用
来源：http://skr.cashguo.top

df -h;  du -sh *
来源：http://gcm.yj20258888.top

[R62] 找最占空间的文件
来源：http://yob.ydjk.org.cn

du -ah . | sort -rh | head -10
来源：http://qjf.xinyue.icu

[R63] 内存与进程
来源：http://doz.fktsv.cn

free -h;  ps aux | grep nginx
来源：http://sbk.yanxiufei.cn

[R64] 结束进程
来源：http://llq.fehbvm.com

kill -9 $(pgrep -f app.py)
来源：http://zuf.hfpthk.cn

[R65] 查看端口占用
来源：http://qwi.chenlongwang.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fgo.snrcjt.cn

[R66] 定时任务
来源：http://ijx.yfazqb.com

crontab -e;  crontab -l
来源：http://afr.hywenlv.cn

[R67] 生成随机十六进制串
来源：http://ols.gotoacloud.top

openssl rand -hex 16
来源：http://dhy.nanxuanxn.top

[R68] 计算文件校验值
来源：http://ynu.0kj1m.cn

sha256sum a.txt;  md5sum a.txt
来源：http://emw.yangfankeji.com

[R69] 生成随机密码
来源：http://ldd.sjlbkw.cn

head -c 16 /dev/urandom | base64
来源：http://yba.jianghu66.top

[R70] 时间戳与互转
来源：http://qkk.wangshuangyany.cn

date +%s;  date -d @1700000000
来源：http://qyo.daxiang520.top

[R71] 日期格式化
来源：http://dwc.zhijiandao.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fdb.yongpay.top

[R72] 等待端口就绪
来源：http://mle.aizwys.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dir.vehdjk.com

[R73] 分割大日志
来源：http://pkt.sweek.top

split -l 1000 big.log part_
来源：http://khu.hammf.cn

[R74] 批量重命名
来源：http://fbb.ybcxt.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://maj.xinyue.icu

[R75] 导出环境变量
来源：http://jjd.zdbjq.cn

export PATH="$HOME/bin:$PATH"
来源：http://hfr.gzhubu.top

[R76] 使用临时文件
来源：http://qvr.ivvv.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mpx.tarul.cn

[R77] 读取用户输入
来源：http://yij.fzhhl.top

read -rp "请输入: " ans
来源：http://wlw.jinqigufen.top

[R78] 交互式菜单
来源：http://njy.yj202588.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rqb.zhongyouzk.top

[R79] 解析命令行选项
来源：http://aqk.zycfv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sjf.sysykeji.top

[R80] 查看脚本执行耗时
来源：http://psb.yanxiufei.cn

time ./run.sh
来源：http://arx.tanke756.top

================================================================================
来源：http://wop.guowangkeji.top

S. C / C++ 专题
来源：http://jaq.mhx1999.top

================================================================================
来源：http://lot.ydjk.org.cn

[S01] C：Hello World
来源：http://exk.yuxming.cn

#include <stdio.h>
来源：http://lsy.cashguo.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://myg.yj20258.top

[S02] C：变量与格式化输出
来源：http://dpi.cqqwz.cn

int a = 10; printf("%d\n", a);
来源：http://raj.kuanghao11.cn

[S03] C：读入整数
来源：http://eme.bbcook.cn

int x; scanf("%d", &x);
来源：http://fmh.chenjidiqi.icu

[S04] C：字符串复制
来源：http://ege.vehdjk.com

char dst[32]; strcpy(dst, "hi");
来源：http://pbx.jinghuilouyu.cn

[S05] C：字符串长度
来源：http://xyf.ydzc1.top

strlen(s)
来源：http://moe.gogol.net.cn

[S06] C：字符串比较
来源：http://hjl.havefunace.top

strcmp(a, b) == 0
来源：http://vqs.hysaishi.cn

[S07] C：数组遍历求和
来源：http://vxq.sweek.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vbk.wangdashe.top

[S08] C：动态内存分配与释放
来源：http://klt.zdbjq.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hka.shanyushiyangkeji.top

[S09] C：结构体定义与初始化
来源：http://uxy.daria6918.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bfa.aizwys.cn

[S10] C：指针与解引用
来源：http://xqj.daria6918.cn

int *p = &a;  *p = 5;
来源：http://ysj.fktsv.cn

[S11] C：逐行读文件
来源：http://olx.0kj1m.cn

FILE *f = fopen("a.txt", "r");
来源：http://zvp.shanyushiyangkeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qub.shangyingyoupin.top

fclose(f);
来源：http://xbj.yangfankeji.com

[S12] C：写文件
来源：http://zeb.zhengqikj.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qsu.zhaomingkeji.xyz

[S13] C：宏定义
来源：http://nop.dianchejie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mlr.yuxming.cn

[S14] C：枚举
来源：http://xhf.ehwqpu.com

enum Color { RED, GREEN, BLUE };
来源：http://diu.cucudq.cn

[S15] C：类型转换
来源：http://ogq.ydjk.org.cn

(double) a / b
来源：http://nwo.snrcjt.cn

[S16] C：位操作置位
来源：http://nqk.jqgfzy.top

x |= (1 << 3);
来源：http://rle.xingfuxueyuan.xyz

[S17] C：安全拼接字符串
来源：http://qof.feifeiyinyue.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://egw.9152youxi.cn

[S18] C：命令行参数
来源：http://lqy.jianghu66.top

int main(int argc, char **argv)
来源：http://zgu.shzxlz.cn

[S19] C：快速排序
来源：http://quu.wangdashe.top

qsort(a, n, sizeof(int), cmp);
来源：http://zkx.sxryk.cn

[S20] C：二分查找
来源：http://shh.jlsjyb.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jyi.sweek.top

[S21] C：字符类别判断
来源：http://rop.zhongyouzk.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://iao.jinqigfzy.top

[S22] C：字符串转数字
来源：http://gyq.hesvh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jzj.dianchejie.cn

[S23] C：随机数
来源：http://emr.bbcook.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://oxz.yj202588.top

[S24] C：获取本地时间
来源：http://kus.guannengcc.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ivm.zhongyouzk.top

[S25] C：内存拷贝
来源：http://ezu.andypj.xyz

memcpy(dst, src, n);
来源：http://uju.fengsongda.top

[S26] C：内存清零
来源：http://usx.iojbl.cn

memset(a, 0, sizeof a);
来源：http://ipd.iojbl.cn

[S27] C：定义常量
来源：http://jov.shuidangran.top

const double PI = 3.14159;
来源：http://air.jianghu66.top

[S28] C：静态变量
来源：http://uzc.dashuyun.cn

static int counter = 0;
来源：http://seh.yanxiufei.cn

[S29] C：变参函数
来源：http://yux.yanxiufei.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://owa.cucudq.cn

[S30] C：头文件保护
来源：http://yjb.yuanzhike.top

#ifndef X_H
来源：http://kbn.xinyue.icu

#define X_H
来源：http://nnl.fktsv.cn

#endif
来源：http://vaf.feifeiyinyue.top

[S31] C++：Hello World
来源：http://jgj.bjfxy.top

#include <iostream>
来源：http://hod.zhaomingkeji.xyz

int main() { std::cout << "Hello\n"; }
来源：http://hdx.9152youxi.cn

[S32] C++：字符串
来源：http://plf.hfpthk.cn

std::string s = "hi";  s += "!";
来源：http://chq.pengpengdd.cyou

[S33] C++：vector 增删
来源：http://ymv.fktsv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qou.dashuyun.cn

[S34] C++：遍历 vector
来源：http://wbi.fanxiaobao.xyz

for (auto &x : v) { std::cout << x; }
来源：http://qge.sufxvd.cn

[S35] C++：map
来源：http://ann.gaohongyu789.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mfp.yongpay.top

[S36] C++：unordered_map
来源：http://tpa.jinghuilouyu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hlq.zhongyouzk.top

[S37] C++：set
来源：http://quj.nwbrower.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jog.yuanzhike.top

[S38] C++：排序
来源：http://mcu.bjfxy.top

std::sort(v.begin(), v.end());
来源：http://xve.andypj.xyz

[S39] C++：自定义比较器排序
来源：http://uak.fengsongda.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://opr.birdmap.top

[S40] C++：查找元素
来源：http://ljp.wangdashe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vgi.guowangkeji.top

[S41] C++：类与构造函数
来源：http://cuo.316326.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dbe.uphjek.com

[S42] C++：继承与虚函数
来源：http://shi.andypj.xyz

class B : public Base { public: void f() override {} };
来源：http://arf.tian-w.cn

[S43] C++：智能指针
来源：http://tfa.shuidangran.top

auto p = std::make_unique<int>(5);
来源：http://kil.hywenlv.cn

[S44] C++：引用传参
来源：http://fgs.sxryk.cn

void inc(int &x) { ++x; }
来源：http://fll.fzhhl.top

[S45] C++：lambda
来源：http://joy.bjfxy.top

auto add = [](int a, int b) { return a + b; };
来源：http://tnw.hnxiangtu.top

[S46] C++：函数模板
来源：http://swh.smart0.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uso.cqqwz.cn

[S47] C++：结构化绑定遍历
来源：http://pag.bbcook.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fyo.yj202588.top

[S48] C++：逐行读文件
来源：http://qhw.yuxming.cn

std::ifstream in("a.txt");  std::string line;
来源：http://esp.sjlbkw.cn

while (std::getline(in, line)) { }
来源：http://zjm.ctjpmb.com

[S49] C++：写文件
来源：http://nqv.jinyuanbaomall.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qxa.yfazqb.com

[S50] C++：格式化数字
来源：http://her.zhaomingkeji.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zem.svipenyu.cn

[S51] C++：显式类型转换
来源：http://fqv.hnqzz.top

static_cast<double>(a) / b
来源：http://fis.guannengcc.top

[S52] C++：const 与 noexcept
来源：http://cnk.zdqjudy.top

int size() const noexcept { return n_; }
来源：http://fvg.cashguo.top

[S53] C++：移动语义
来源：http://fhh.daria6918.cn

std::vector<int> w = std::move(v);
来源：http://mmt.nanxinkj.top

[S54] C++：异常处理
来源：http://lqs.gogol.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://glp.redwolf501.top

[S55] C++：结构化绑定
来源：http://gtw.ydjk.org.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ckd.meibo888.top

[S56] C++：optional
来源：http://nvy.jlsjyb.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://emh.yuanzhike.top

[S57] C++：编译期常量
来源：http://ymq.meibo888.top

constexpr int N = 10;
来源：http://xgt.ctjpmb.com

[S58] C++：命名空间
来源：http://ebx.fzhhl.top

namespace ns { int f() { return 1; } }
来源：http://ffd.guannengcc.top

[S59] C++：静态断言
来源：http://eii.sxryk.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hbv.meibo888.top

[S60] C++：遍历并删除元素
来源：http://dcr.yonumen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kmk.c1oappe.top

================================================================================
来源：http://bay.iojbl.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uag.daria6918.cn

================================================================================
来源：http://xhp.cdnleiting.top

[T01] Kotlin：Hello World
来源：http://nui.9152youxi.cn

println("Hello")
来源：http://gjd.jinyuanbaomall.cn

[T02] Kotlin：变量
来源：http://unk.yuanzhike.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vsj.zhengqikj.top

[T03] Kotlin：字符串模板
来源：http://pot.jyoumei.cn

"值: $b"
来源：http://rbv.aizwys.cn

[T04] Kotlin：空安全
来源：http://vcc.zdbjq.cn

val n: String? = null;  n?.length
来源：http://fqg.sweek.top

[T05] Kotlin：when 表达式
来源：http://ofq.dianchejie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://njj.hcnkem.com

[T06] Kotlin：集合映射
来源：http://kdc.ydjk.org.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fir.ydzc1.top

[T07] Kotlin：集合过滤
来源：http://otb.mhx1999.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://adk.tianlin.xyz

[T08] Kotlin：数据类
来源：http://ysi.jinqigfzy.top

data class User(val name: String, val age: Int)
来源：http://kih.shanyushiyangtech.top

[T09] Kotlin：扩展函数
来源：http://jzd.9152youxi.cn

fun String.exclaim() = this + "!"
来源：http://pdr.jyoumei.cn

[T10] Kotlin：默认参数
来源：http://pus.meibo888.top

fun greet(name: String = "World") = "Hi $name"
来源：http://pvm.fehbvm.com


<!-- 参考信息 -->