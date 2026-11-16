代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kfc.nanxuanxn.top

[R08] 数值比较
来源：http://fhw.yj202588.top

if (( a > b )); then echo "a 更大"; fi
来源：http://giq.zhijiandao.cn

[R09] 字符串比较
来源：http://jux.chenzaomai.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sll.hysaishi.cn

[R10] 正则匹配
来源：http://gtb.mhx1999.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qof.hnxiangtu.top

[R11] case 多分支
来源：http://zlf.gzhubu.top

case "$1" in
来源：http://wbj.hammf.cn

start) echo "启动" ;;
来源：http://rqy.haohaochexian.top

stop)  echo "停止" ;;
来源：http://giu.jqgufenzy.top

*)     echo "未知命令" ;;
来源：http://giu.yvedp.cn

esac
来源：http://uys.jinqigufen.top

[R12] for 遍历文件
来源：http://sxn.xinyue.icu

for f in *.txt; do echo "$f"; done
来源：http://fxr.xuetiantiany.cn

[R13] for 计数循环
来源：http://pwj.shanyushiyangkeji.top

for i in {1..10}; do echo "$i"; done
来源：http://azf.kuanghao11.cn

[R14] C 风格 for
来源：http://vvy.bbcook.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jgr.xylfe.cn

[R15] while 逐行读文件
来源：http://msl.xuetiantiany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zor.jlsjyb.cn

[R16] until 等待条件
来源：http://aqa.shanyushiyangkeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ndh.sxryk.cn

[R17] 数组定义与取值
来源：http://akt.bbcook.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qvl.cqqwz.cn

[R18] 遍历数组
来源：http://nxj.xingfuxueyuan.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mez.xuanzx.com

[R19] 数组长度
来源：http://mhg.xziqi.cn

echo "${#arr[@]}"
来源：http://lhf.hcnkem.com

[R20] 关联数组（字典）
来源：http://xck.haohaochexian.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jjh.wangdashe.top

[R21] 字符串长度
来源：http://lqf.sysykeji.top

echo "${#s}"
来源：http://jis.uphjek.com

[R22] 截取子串
来源：http://zol.redwolf501.top

echo "${s:0:5}"
来源：http://aqq.fengsongda.top

[R23] 字符串替换
来源：http://ygd.yvedp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uei.zycfv.cn

[R24] 大小写转换
来源：http://myz.havefunace.top

echo "${s^^}"; echo "${s,,}"
来源：http://pko.yanxiufei.cn

[R25] 去后缀 / 去前缀
来源：http://pjo.yj20258.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://fay.daria6918.cn

[R26] 命令替换
来源：http://avw.ctjpmb.com

now=$(date +%F); echo "$now"
来源：http://asc.havefunace.top

[R27] 算术展开
来源：http://thw.sxryk.cn

echo $((1 + 2 * 3))
来源：http://ukv.yvedp.cn

[R28] 浮点运算
来源：http://wha.yuxming.cn

echo "scale=2; 10/3" | bc
来源：http://oku.yueranfly.top

[R29] 定义函数
来源：http://ihf.ehwqpu.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cvu.havefunace.top

[R30] 函数返回状态码
来源：http://csa.zhengqikj.top

f() { return 0; }; f || echo "失败了"
来源：http://myl.yanxiufei.cn

[R31] 局部变量
来源：http://ryc.yanxiufei.cn

f() { local x=1; echo "$x"; }
来源：http://alq.vehdjk.com

[R32] 参数个数校验
来源：http://exs.wangshuangyany.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vdy.shanyushiyangkeji.top

[R33] 捕获错误并提示行号
来源：http://ohz.xuanzx.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://npq.nanxinkj.top

[R34] 退出时清理
来源：http://rxj.wangdashe.top

trap 'rm -f "$tmp"' EXIT
来源：http://kfh.cucudq.cn

[R35] 后台执行并等待
来源：http://kta.birdmap.top

sleep 5 & pid=$!; wait "$pid"
来源：http://jlj.hongshengwenyu.top

[R36] 并发执行多个任务
来源：http://ssp.jlsjyb.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hqu.havefunace.top

[R37] 把输出赋给变量
来源：http://oro.birdmap.top

files=$(ls -1)
来源：http://aaz.andypj.xyz

[R38] 管道串联
来源：http://kys.chenjidiqi.icu

cat a.txt | grep -i error | wc -l
来源：http://lif.jlsjyb.cn

[R39] 重定向标准输出与错误
来源：http://xpm.yongpay.top

cmd > out.log 2>&1
来源：http://tie.mhx1999.top

[R40] 追加写日志
来源：http://vek.shzxlz.cn

echo "log" >> out.log
来源：http://wvs.sufxvd.cn

[R41] 丢弃输出
来源：http://ppx.yanxiufei.cn

cmd >/dev/null 2>&1
来源：http://wqb.kuanghao11.cn

[R42] 输入重定向
来源：http://ebx.yj202588.top

wc -l < a.txt
来源：http://lug.sjlbkw.cn

[R43] 按名字查找文件
来源：http://drz.cashguo.top

find . -name "*.log" -type f
来源：http://zvj.bjfxy.top

[R44] 按修改时间查找
来源：http://pgc.uphjek.com

find . -mtime -7 -type f
来源：http://roi.xylfe.cn

[R45] 批量删除
来源：http://xnz.ivvv.top

find . -name "*.tmp" -delete
来源：http://epc.cheryme.top

[R46] 递归替换文件内容
来源：http://fvz.redwolf501.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://try.hfpthk.cn

[R47] sed 单行替换
来源：http://qjw.gaohongyu789.top

sed -i 's/foo/bar/g' a.txt
来源：http://czg.shanyushiyangtech.top

[R48] awk 取指定列
来源：http://pgc.jiagoushi.top

awk '{print $1, $3}' a.txt
来源：http://jhs.cqqwz.cn

[R49] awk 带条件
来源：http://jzq.aizwys.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bsc.fzhhl.top

[R50] awk 求和
来源：http://yds.zhixingplan.top

awk '{s += $2} END {print s}' a.txt
来源：http://qwm.xylfe.cn

[R51] 排序去重取前几
来源：http://nrz.ctjpmb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://sdd.xinyue.icu

[R52] 统计行数
来源：http://mof.52xcode.cn

wc -l a.txt
来源：http://wze.bbcook.cn

[R53] 查看文件头与实时尾
来源：http://rxz.zhaomingkeji.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hws.uphjek.com

[R54] 比较两个文件
来源：http://wru.svipenyu.cn

diff a.txt b.txt
来源：http://dcz.jinghuilouyu.cn

[R55] 压缩与解压
来源：http://odu.haohaochexian.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lbw.bbcook.cn

[R56] 远程拷贝
来源：http://vsy.kuanghao11.cn

scp file user@host:/path/
来源：http://cuz.jqgufenzy.top

[R57] 远程执行命令
来源：http://xst.nanxuanxn.top

ssh user@host 'uptime'
来源：http://kdw.zhongyouzk.top

[R58] 下载文件
来源：http://meu.ehwqpu.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xuz.ppjwa.cn

[R59] 发 POST JSON
来源：http://dra.fanxiaobao.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cos.epnwcf.com

[R60] 只看 HTTP 状态码
来源：http://rrk.wangdashe.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zzs.fzhhl.top

[R61] 磁盘占用
来源：http://nvb.sjlbkw.cn

df -h;  du -sh *
来源：http://jhq.cdnleiting.top

[R62] 找最占空间的文件
来源：http://nhi.0kj1m.cn

du -ah . | sort -rh | head -10
来源：http://rtk.feifeiyinyue.top

[R63] 内存与进程
来源：http://jxj.ywan-chungtsiang.top

free -h;  ps aux | grep nginx
来源：http://bql.wangshuangyany.cn

[R64] 结束进程
来源：http://clj.fktsv.cn

kill -9 $(pgrep -f app.py)
来源：http://fcv.ydzc1.top

[R65] 查看端口占用
来源：http://wlb.chenzaomai.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uas.yuxming.cn

[R66] 定时任务
来源：http://ddl.xylfe.cn

crontab -e;  crontab -l
来源：http://och.c1oappe.top

[R67] 生成随机十六进制串
来源：http://doy.aizwys.cn

openssl rand -hex 16
来源：http://rnp.yuanzhike.top

[R68] 计算文件校验值
来源：http://jdh.ydjk.org.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jdn.chenjidiqi.icu

[R69] 生成随机密码
来源：http://abh.andypj.xyz

head -c 16 /dev/urandom | base64
来源：http://oxb.svipenyu.cn

[R70] 时间戳与互转
来源：http://nal.tanke756.top

date +%s;  date -d @1700000000
来源：http://tyl.bbcook.cn

[R71] 日期格式化
来源：http://def.yuxming.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mlx.cheryme.top

[R72] 等待端口就绪
来源：http://unj.xingfuxueyuan.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://rgb.chenzaomai.com

[R73] 分割大日志
来源：http://bvr.wangdashe.top

split -l 1000 big.log part_
来源：http://zoe.zhoulong.xyz

[R74] 批量重命名
来源：http://qpz.gogol.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vtv.wangshuangyany.cn

[R75] 导出环境变量
来源：http://ebk.snrcjt.cn

export PATH="$HOME/bin:$PATH"
来源：http://afd.daria6918.cn

[R76] 使用临时文件
来源：http://kpr.fengsongda.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tnv.fehbvm.com

[R77] 读取用户输入
来源：http://lml.zhoulong.xyz

read -rp "请输入: " ans
来源：http://znn.jianghu66.top

[R78] 交互式菜单
来源：http://ofo.gogol.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vsg.hywenlv.cn

[R79] 解析命令行选项
来源：http://awf.meibo888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tqy.yueranfly.top

[R80] 查看脚本执行耗时
来源：http://weu.haohaochexian.top

time ./run.sh
来源：http://ynl.cqqwz.cn

================================================================================
来源：http://tcm.hongshengwenyu.top

S. C / C++ 专题
来源：http://kng.zycfv.cn

================================================================================
来源：http://ehy.xuanzx.com

[S01] C：Hello World
来源：http://pfi.ydjk.org.cn

#include <stdio.h>
来源：http://aba.xingfuxueyuan.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://djt.shanyushiyangtech.top

[S02] C：变量与格式化输出
来源：http://gkh.hcnkem.com

int a = 10; printf("%d\n", a);
来源：http://zmm.ivvv.top

[S03] C：读入整数
来源：http://cdi.sufxvd.cn

int x; scanf("%d", &x);
来源：http://bno.mhx1999.top

[S04] C：字符串复制
来源：http://xot.fehbvm.com

char dst[32]; strcpy(dst, "hi");
来源：http://lbm.jinghuilouyu.cn

[S05] C：字符串长度
来源：http://gmh.zhixingplan.top

strlen(s)
来源：http://xvt.cashguo.top

[S06] C：字符串比较
来源：http://nlz.ivvv.top

strcmp(a, b) == 0
来源：http://lbx.jiagoushi.top

[S07] C：数组遍历求和
来源：http://pni.yj20258888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://los.xylfe.cn

[S08] C：动态内存分配与释放
来源：http://fin.hfpthk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dgm.hywenlv.cn

[S09] C：结构体定义与初始化
来源：http://kar.jiagoushi.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nod.snrcjt.cn

[S10] C：指针与解引用
来源：http://tio.zhixingplan.top

int *p = &a;  *p = 5;
来源：http://sjq.hesvh.cn

[S11] C：逐行读文件
来源：http://rec.zhongyouzk.top

FILE *f = fopen("a.txt", "r");
来源：http://ftb.yfazqb.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://fnp.hcnkem.com

fclose(f);
来源：http://qov.vehdjk.com

[S12] C：写文件
来源：http://wsk.ydjk.org.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nzn.hesvh.cn

[S13] C：宏定义
来源：http://asp.jinyuanbaomall.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tcv.smart0.xyz

[S14] C：枚举
来源：http://sem.hywenlv.cn

enum Color { RED, GREEN, BLUE };
来源：http://qrx.daxiang520.top

[S15] C：类型转换
来源：http://xme.fengsongda.top

(double) a / b
来源：http://ozf.haohaochexian.top

[S16] C：位操作置位
来源：http://hlo.yj20258.top

x |= (1 << 3);
来源：http://wlm.jinqigufen.top

[S17] C：安全拼接字符串
来源：http://pzh.xziqi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nrn.fzhhl.top

[S18] C：命令行参数
来源：http://rus.fengsongda.top

int main(int argc, char **argv)
来源：http://gft.zdqjudy.top

[S19] C：快速排序
来源：http://qaa.ehwqpu.com

qsort(a, n, sizeof(int), cmp);
来源：http://ifr.nwbrower.top

[S20] C：二分查找
来源：http://iuq.birdmap.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ggh.zhengqikj.top

[S21] C：字符类别判断
来源：http://vay.xziqi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mui.c1oappe.top

[S22] C：字符串转数字
来源：http://vgk.nanxuanxn.top

atoi("42");  strtod("3.14", NULL);
来源：http://cca.sufxvd.cn

[S23] C：随机数
来源：http://tek.ydzc1.top

srand(time(NULL));  int r = rand() % 100;
来源：http://sjn.fanxiaobao.xyz

[S24] C：获取本地时间
来源：http://mlz.tian-w.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ljd.mhx1999.top

[S25] C：内存拷贝
来源：http://bmq.hfpthk.cn

memcpy(dst, src, n);
来源：http://ivu.tian-w.cn

[S26] C：内存清零
来源：http://jvq.yj20258.top

memset(a, 0, sizeof a);
来源：http://jyc.epnwcf.com

[S27] C：定义常量
来源：http://gbs.tianlin.xyz

const double PI = 3.14159;
来源：http://ljz.cashguo.top

[S28] C：静态变量
来源：http://nnt.epnwcf.com

static int counter = 0;
来源：http://dai.iojbl.cn

[S29] C：变参函数
来源：http://nir.yanxiufei.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://poc.havefunace.top

[S30] C：头文件保护
来源：http://voh.hongshengwenyu.top

#ifndef X_H
来源：http://pbb.sweek.top

#define X_H
来源：http://hsp.hnqzz.top

#endif
来源：http://oum.bbcook.cn

[S31] C++：Hello World
来源：http://ybx.tianlin.xyz

#include <iostream>
来源：http://noe.tianlin.xyz

int main() { std::cout << "Hello\n"; }
来源：http://duk.jlsjyb.cn

[S32] C++：字符串
来源：http://jsm.bbcook.cn

std::string s = "hi";  s += "!";
来源：http://pbp.zdqjudy.top

[S33] C++：vector 增删
来源：http://opm.dianchejie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gux.zhoulong.xyz

[S34] C++：遍历 vector
来源：http://rcz.cucudq.cn

for (auto &x : v) { std::cout << x; }
来源：http://ssb.jiagoushi.top

[S35] C++：map
来源：http://txn.svipenyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://muv.ydzc1.top

[S36] C++：unordered_map
来源：http://poe.zhoulong.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mne.yanxiufei.cn

[S37] C++：set
来源：http://few.jianghu66.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tba.hesvh.cn

[S38] C++：排序
来源：http://ctp.pycfn.com

std::sort(v.begin(), v.end());
来源：http://fna.chenjidiqi.icu

[S39] C++：自定义比较器排序
来源：http://czg.nanxuanxn.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vto.chenjidiqi.icu

[S40] C++：查找元素
来源：http://fgf.birdmap.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mfn.aibaodan.cn

[S41] C++：类与构造函数
来源：http://blg.sysykeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nlk.ivvv.top

[S42] C++：继承与虚函数
来源：http://gbr.redwolf501.top

class B : public Base { public: void f() override {} };
来源：http://kjm.yj20258888.top

[S43] C++：智能指针
来源：http://keu.fzhhl.top

auto p = std::make_unique<int>(5);
来源：http://qiq.birdmap.top

[S44] C++：引用传参
来源：http://cmu.quarkkingdee.top

void inc(int &x) { ++x; }
来源：http://rrn.cqqwz.cn

[S45] C++：lambda
来源：http://mcr.hfpthk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://orm.zdqjudy.top

[S46] C++：函数模板
来源：http://ugz.zhixingplan.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lvp.birdmap.top

[S47] C++：结构化绑定遍历
来源：http://ehi.redwolf501.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mgm.bbcook.cn

[S48] C++：逐行读文件
来源：http://awx.pycfn.com

std::ifstream in("a.txt");  std::string line;
来源：http://kkn.ctjpmb.com

while (std::getline(in, line)) { }
来源：http://hgc.cqqwz.cn

[S49] C++：写文件
来源：http://gbm.yongpay.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ggx.hcnkem.com

[S50] C++：格式化数字
来源：http://gke.c1oappe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://giv.yfazqb.com

[S51] C++：显式类型转换
来源：http://qdt.gaohongyu789.top

static_cast<double>(a) / b
来源：http://zbc.haohaochexian.top

[S52] C++：const 与 noexcept
来源：http://vab.birdmap.top

int size() const noexcept { return n_; }
来源：http://kkr.vqdsnc.cn

[S53] C++：移动语义
来源：http://cez.c1oappe.top

std::vector<int> w = std::move(v);
来源：http://iwv.shzxlz.cn

[S54] C++：异常处理
来源：http://yyj.cheryme.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sob.cdnleiting.top

[S55] C++：结构化绑定
来源：http://ksm.zhaomingkeji.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://obm.cqqwz.cn

[S56] C++：optional
来源：http://pbb.hcnkem.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hyr.smart0.xyz

[S57] C++：编译期常量
来源：http://lyy.shzxlz.cn

constexpr int N = 10;
来源：http://sow.sysykeji.top

[S58] C++：命名空间
来源：http://bef.xziqi.cn

namespace ns { int f() { return 1; } }
来源：http://rfc.mhx1999.top

[S59] C++：静态断言
来源：http://mlf.chenzaomai.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qrp.yfazqb.com

[S60] C++：遍历并删除元素
来源：http://ybv.9152youxi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qye.aibaodan.cn

================================================================================
来源：http://uos.hongshengwenyu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jtr.jianghu66.top

================================================================================
来源：http://oxt.zycfv.cn

[T01] Kotlin：Hello World
来源：http://gtx.hfpthk.cn

println("Hello")
来源：http://mvq.yj202588.top

[T02] Kotlin：变量
来源：http://ikp.gogol.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qsk.bjfxy.top

[T03] Kotlin：字符串模板
来源：http://rul.jinqigufen.top

"值: $b"
来源：http://ykc.hnqzz.top

[T04] Kotlin：空安全
来源：http://vpc.zhengqikj.top

val n: String? = null;  n?.length
来源：http://bms.snrcjt.cn

[T05] Kotlin：when 表达式
来源：http://uze.wangshuangyany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://asq.jiagoushi.top

[T06] Kotlin：集合映射
来源：http://sav.hnqzz.top

listOf(1, 2, 3).map { it * 2 }
来源：http://dhg.hywenlv.cn

[T07] Kotlin：集合过滤
来源：http://row.hongshengwenyu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://cjl.bjfxy.top

[T08] Kotlin：数据类
来源：http://vvg.quarkkingdee.top

data class User(val name: String, val age: Int)
来源：http://sdv.hfpthk.cn


<!-- 参考信息 -->