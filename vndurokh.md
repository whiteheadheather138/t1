代发 wailian999

name="${1:-default}"
来源：http://rpb.sweek.top

[R06] 判断命令是否存在
来源：http://tyh.bjfxy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vdx.chenlongwang.top

[R07] if 判断文件
来源：http://vod.yanxiufei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ojq.daria6918.cn

[R08] 数值比较
来源：http://yso.tarul.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tfm.sxryk.cn

[R09] 字符串比较
来源：http://heo.bbcook.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wrx.9152youxi.cn

[R10] 正则匹配
来源：http://oxv.pycfn.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sjg.guannengcc.top

[R11] case 多分支
来源：http://xzp.zdqjudy.top

case "$1" in
来源：http://ugn.xziqi.cn

start) echo "启动" ;;
来源：http://qrc.jinghuilouyu.cn

stop)  echo "停止" ;;
来源：http://fiv.hysaishi.cn

*)     echo "未知命令" ;;
来源：http://yta.dashuyun.cn

esac
来源：http://jdf.birdmap.top

[R12] for 遍历文件
来源：http://hkp.vqdsnc.cn

for f in *.txt; do echo "$f"; done
来源：http://ufu.tarul.cn

[R13] for 计数循环
来源：http://zsh.shuidangran.top

for i in {1..10}; do echo "$i"; done
来源：http://aqz.gaohongyu789.top

[R14] C 风格 for
来源：http://emu.pengpengdd.cyou

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vyw.hcnkem.com

[R15] while 逐行读文件
来源：http://pyc.316326.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yxs.redwolf501.top

[R16] until 等待条件
来源：http://ayi.yuxming.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sbs.zdbjq.cn

[R17] 数组定义与取值
来源：http://xcs.daxiang520.top

arr=(a b c); echo "${arr[0]}"
来源：http://yjq.yj202588.top

[R18] 遍历数组
来源：http://sdz.iojbl.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://otd.zhoulong.xyz

[R19] 数组长度
来源：http://cef.zdbjq.cn

echo "${#arr[@]}"
来源：http://kez.yueranfly.top

[R20] 关联数组（字典）
来源：http://hdn.bjfxy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cmh.ybcxt.top

[R21] 字符串长度
来源：http://duz.hesvh.cn

echo "${#s}"
来源：http://nge.yj202588.top

[R22] 截取子串
来源：http://rwt.svipenyu.cn

echo "${s:0:5}"
来源：http://nan.aibaodan.cn

[R23] 字符串替换
来源：http://clx.yangfankeji.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qfz.cdnleiting.top

[R24] 大小写转换
来源：http://nik.yuanzhike.top

echo "${s^^}"; echo "${s,,}"
来源：http://jgg.hysaishi.cn

[R25] 去后缀 / 去前缀
来源：http://cwv.zdqjudy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://xfn.jinqigfzy.top

[R26] 命令替换
来源：http://xpi.redwolf501.top

now=$(date +%F); echo "$now"
来源：http://nap.pycfn.com

[R27] 算术展开
来源：http://kkt.epnwcf.com

echo $((1 + 2 * 3))
来源：http://owm.wangdashe.top

[R28] 浮点运算
来源：http://tai.yonumen.top

echo "scale=2; 10/3" | bc
来源：http://jpj.52xcode.cn

[R29] 定义函数
来源：http://dmg.smart0.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fog.aibaodan.cn

[R30] 函数返回状态码
来源：http://cfv.redwolf501.top

f() { return 0; }; f || echo "失败了"
来源：http://tvv.chenjidiqi.icu

[R31] 局部变量
来源：http://tsx.tarul.cn

f() { local x=1; echo "$x"; }
来源：http://qcz.gzhubu.top

[R32] 参数个数校验
来源：http://opl.fehbvm.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ncb.yfazqb.com

[R33] 捕获错误并提示行号
来源：http://mef.quarkkingdee.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pqo.jlsjyb.cn

[R34] 退出时清理
来源：http://kdf.tarul.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xtq.guannengcc.top

[R35] 后台执行并等待
来源：http://kol.yonumen.top

sleep 5 & pid=$!; wait "$pid"
来源：http://mcv.epnwcf.com

[R36] 并发执行多个任务
来源：http://gie.guannengcc.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://asv.meibo888.top

[R37] 把输出赋给变量
来源：http://wnr.cashguo.top

files=$(ls -1)
来源：http://czc.dashuyun.cn

[R38] 管道串联
来源：http://egd.bjfxy.top

cat a.txt | grep -i error | wc -l
来源：http://fqb.xylfe.cn

[R39] 重定向标准输出与错误
来源：http://bds.jiagoushi.top

cmd > out.log 2>&1
来源：http://lnk.52xcode.cn

[R40] 追加写日志
来源：http://yjj.fktsv.cn

echo "log" >> out.log
来源：http://tml.zhaomingkeji.xyz

[R41] 丢弃输出
来源：http://dtd.fktsv.cn

cmd >/dev/null 2>&1
来源：http://ecc.xuetiantiany.cn

[R42] 输入重定向
来源：http://lli.yongpay.top

wc -l < a.txt
来源：http://kpr.gzhubu.top

[R43] 按名字查找文件
来源：http://psz.hammf.cn

find . -name "*.log" -type f
来源：http://iax.yuanzhike.top

[R44] 按修改时间查找
来源：http://kjg.shangyingyoupin.top

find . -mtime -7 -type f
来源：http://lhd.hysaishi.cn

[R45] 批量删除
来源：http://vaw.haohaochexian.top

find . -name "*.tmp" -delete
来源：http://wjm.sysykeji.top

[R46] 递归替换文件内容
来源：http://idc.mhx1999.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qud.hammf.cn

[R47] sed 单行替换
来源：http://vxh.yuanzhike.top

sed -i 's/foo/bar/g' a.txt
来源：http://iam.vqdsnc.cn

[R48] awk 取指定列
来源：http://bsx.yueranfly.top

awk '{print $1, $3}' a.txt
来源：http://mqa.xylfe.cn

[R49] awk 带条件
来源：http://mhv.hesvh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ced.jqgufenzy.top

[R50] awk 求和
来源：http://gbq.ctjpmb.com

awk '{s += $2} END {print s}' a.txt
来源：http://qtd.daria6918.cn

[R51] 排序去重取前几
来源：http://xec.sufxvd.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://syq.haohaochexian.top

[R52] 统计行数
来源：http://mwe.ydzc1.top

wc -l a.txt
来源：http://ofr.zhengqikj.top

[R53] 查看文件头与实时尾
来源：http://ycr.yj202588.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pzv.9152youxi.cn

[R54] 比较两个文件
来源：http://xmy.feifeiyinyue.top

diff a.txt b.txt
来源：http://fgo.9152youxi.cn

[R55] 压缩与解压
来源：http://hka.pengpengdd.cyou

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ykw.316326.xyz

[R56] 远程拷贝
来源：http://zwh.guowangkeji.top

scp file user@host:/path/
来源：http://kdv.zhaomingkeji.xyz

[R57] 远程执行命令
来源：http://vke.gzhubu.top

ssh user@host 'uptime'
来源：http://zfy.xinyue.icu

[R58] 下载文件
来源：http://tsr.nanxuanxn.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fxi.yueranfly.top

[R59] 发 POST JSON
来源：http://pwb.fktsv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tqx.ybcxt.top

[R60] 只看 HTTP 状态码
来源：http://msv.chenjidiqi.icu

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jfm.fengsongda.top

[R61] 磁盘占用
来源：http://upj.xinyue.icu

df -h;  du -sh *
来源：http://tbd.zhijiandao.cn

[R62] 找最占空间的文件
来源：http://dcm.yonumen.top

du -ah . | sort -rh | head -10
来源：http://huu.ydjk.org.cn

[R63] 内存与进程
来源：http://gon.zhijiandao.cn

free -h;  ps aux | grep nginx
来源：http://rpc.tianlin.xyz

[R64] 结束进程
来源：http://ikv.sweek.top

kill -9 $(pgrep -f app.py)
来源：http://mib.zdqjudy.top

[R65] 查看端口占用
来源：http://unt.yongpay.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ong.guowangkeji.top

[R66] 定时任务
来源：http://prw.hywenlv.cn

crontab -e;  crontab -l
来源：http://hhs.tanke756.top

[R67] 生成随机十六进制串
来源：http://ccf.ydzc1.top

openssl rand -hex 16
来源：http://tjj.shzxlz.cn

[R68] 计算文件校验值
来源：http://jki.xinyue.icu

sha256sum a.txt;  md5sum a.txt
来源：http://nem.jyoumei.cn

[R69] 生成随机密码
来源：http://ejk.tianlin.xyz

head -c 16 /dev/urandom | base64
来源：http://scu.jqgufenzy.top

[R70] 时间戳与互转
来源：http://jox.snrcjt.cn

date +%s;  date -d @1700000000
来源：http://pwq.xuetiantiany.cn

[R71] 日期格式化
来源：http://rlj.zhijiandao.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://odj.hesvh.cn

[R72] 等待端口就绪
来源：http://ubq.meibo888.top

until nc -z localhost 3306; do sleep 1; done
来源：http://kyo.cucudq.cn

[R73] 分割大日志
来源：http://dct.yangfankeji.com

split -l 1000 big.log part_
来源：http://any.ctjpmb.com

[R74] 批量重命名
来源：http://mkh.zhongyouzk.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://juj.wangdashe.top

[R75] 导出环境变量
来源：http://oiy.shuidangran.top

export PATH="$HOME/bin:$PATH"
来源：http://fsw.yangfankeji.com

[R76] 使用临时文件
来源：http://qzj.daxiang520.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mpo.ywan-chungtsiang.top

[R77] 读取用户输入
来源：http://ypy.tianlin.xyz

read -rp "请输入: " ans
来源：http://pbf.smart0.xyz

[R78] 交互式菜单
来源：http://wew.zhiwuduotai.top

select opt in a b c; do echo "$opt"; break; done
来源：http://gos.ctjpmb.com

[R79] 解析命令行选项
来源：http://bbm.tarul.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jrz.zhiwuduotai.top

[R80] 查看脚本执行耗时
来源：http://euh.guowangkeji.top

time ./run.sh
来源：http://yef.jlsjyb.cn

================================================================================
来源：http://uco.jyoumei.cn

S. C / C++ 专题
来源：http://apg.smart0.xyz

================================================================================
来源：http://qth.zhixingplan.top

[S01] C：Hello World
来源：http://rmk.xylfe.cn

#include <stdio.h>
来源：http://sur.hfpthk.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jax.hywenlv.cn

[S02] C：变量与格式化输出
来源：http://uuy.ydjk.org.cn

int a = 10; printf("%d\n", a);
来源：http://ssr.ppjwa.cn

[S03] C：读入整数
来源：http://nko.gotoacloud.top

int x; scanf("%d", &x);
来源：http://www.hcnkem.com

[S04] C：字符串复制
来源：http://tqe.zhongyouzk.top

char dst[32]; strcpy(dst, "hi");
来源：http://iod.fanxiaobao.xyz

[S05] C：字符串长度
来源：http://rbx.shzxlz.cn

strlen(s)
来源：http://ahx.meibo888.top

[S06] C：字符串比较
来源：http://cbu.yj20258.top

strcmp(a, b) == 0
来源：http://tcg.shanyushiyangtech.top

[S07] C：数组遍历求和
来源：http://drz.tanke756.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://evm.guannengcc.top

[S08] C：动态内存分配与释放
来源：http://tkq.cheryme.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jtr.quarkkingdee.top

[S09] C：结构体定义与初始化
来源：http://nyb.c1oappe.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ksr.hesvh.cn

[S10] C：指针与解引用
来源：http://rvi.zycfv.cn

int *p = &a;  *p = 5;
来源：http://mwl.andypj.xyz

[S11] C：逐行读文件
来源：http://ywp.fehbvm.com

FILE *f = fopen("a.txt", "r");
来源：http://mol.vehdjk.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://egg.hfpthk.cn

fclose(f);
来源：http://jhg.gotoacloud.top

[S12] C：写文件
来源：http://cgb.andypj.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hgw.havefunace.top

[S13] C：宏定义
来源：http://ror.jyoumei.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://isr.wangshuangyany.cn

[S14] C：枚举
来源：http://jyt.nwbrower.top

enum Color { RED, GREEN, BLUE };
来源：http://fbq.yj202588.top

[S15] C：类型转换
来源：http://ute.cdnleiting.top

(double) a / b
来源：http://vss.yanxiufei.cn

[S16] C：位操作置位
来源：http://fhc.feifeiyinyue.top

x |= (1 << 3);
来源：http://ecf.cqqwz.cn

[S17] C：安全拼接字符串
来源：http://lyc.ivvv.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://clc.shuidangran.top

[S18] C：命令行参数
来源：http://mwp.zycfv.cn

int main(int argc, char **argv)
来源：http://mzx.jqgufenzy.top

[S19] C：快速排序
来源：http://ngl.ydzc1.top

qsort(a, n, sizeof(int), cmp);
来源：http://zui.jqgfzy.top

[S20] C：二分查找
来源：http://nbn.sjlbkw.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bpy.svipenyu.cn

[S21] C：字符类别判断
来源：http://vqk.yj202588.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ypr.cheryme.top

[S22] C：字符串转数字
来源：http://bxo.vehdjk.com

atoi("42");  strtod("3.14", NULL);
来源：http://izf.zdbjq.cn

[S23] C：随机数
来源：http://oih.guowangkeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://trm.gaohongyu789.top

[S24] C：获取本地时间
来源：http://udk.jinqigfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lgg.hnxiangtu.top

[S25] C：内存拷贝
来源：http://gmn.fktsv.cn

memcpy(dst, src, n);
来源：http://bkc.sweek.top

[S26] C：内存清零
来源：http://mzi.dashuyun.cn

memset(a, 0, sizeof a);
来源：http://ujd.jinqigufen.top

[S27] C：定义常量
来源：http://tfw.fktsv.cn

const double PI = 3.14159;
来源：http://tqw.ppjwa.cn

[S28] C：静态变量
来源：http://ihl.xziqi.cn

static int counter = 0;
来源：http://cwt.yonumen.top

[S29] C：变参函数
来源：http://gjb.xuanzx.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://npy.nanxuanxn.top

[S30] C：头文件保护
来源：http://qfx.feifeiyinyue.top

#ifndef X_H
来源：http://unh.meibo888.top

#define X_H
来源：http://qbc.shangyingyoupin.top

#endif
来源：http://cvw.yuanzhike.top

[S31] C++：Hello World
来源：http://nkj.52xcode.cn

#include <iostream>
来源：http://sun.fzhhl.top

int main() { std::cout << "Hello\n"; }
来源：http://nuq.ehwqpu.com

[S32] C++：字符串
来源：http://ivv.hywenlv.cn

std::string s = "hi";  s += "!";
来源：http://tsa.gzhubu.top

[S33] C++：vector 增删
来源：http://fsm.sxryk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://how.yangfankeji.com

[S34] C++：遍历 vector
来源：http://izq.snrcjt.cn

for (auto &x : v) { std::cout << x; }
来源：http://aiu.fzhhl.top

[S35] C++：map
来源：http://mxs.gotoacloud.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://aol.ivvv.top

[S36] C++：unordered_map
来源：http://jlo.hfpthk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://awc.fzhhl.top

[S37] C++：set
来源：http://ozq.c1oappe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://god.tarul.cn

[S38] C++：排序
来源：http://xyn.quarkkingdee.top

std::sort(v.begin(), v.end());
来源：http://jis.yuxming.cn

[S39] C++：自定义比较器排序
来源：http://cmo.jinghuilouyu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yvx.gogol.net.cn

[S40] C++：查找元素
来源：http://jqx.tianlin.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ily.daria6918.cn

[S41] C++：类与构造函数
来源：http://lsw.gotoacloud.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hyj.c1oappe.top

[S42] C++：继承与虚函数
来源：http://htj.yuanzhike.top

class B : public Base { public: void f() override {} };
来源：http://cnz.52xcode.cn

[S43] C++：智能指针
来源：http://sab.xuetiantiany.cn

auto p = std::make_unique<int>(5);
来源：http://mrd.sufxvd.cn

[S44] C++：引用传参
来源：http://fzp.jiagoushi.top

void inc(int &x) { ++x; }
来源：http://bzb.zdqjudy.top

[S45] C++：lambda
来源：http://hjp.shuidangran.top

auto add = [](int a, int b) { return a + b; };
来源：http://zqn.zhaomingkeji.xyz

[S46] C++：函数模板
来源：http://nuc.nanxuanxn.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://czh.ctjpmb.com

[S47] C++：结构化绑定遍历
来源：http://gfl.feifeiyinyue.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kup.uphjek.com

[S48] C++：逐行读文件
来源：http://nvy.bbcook.cn

std::ifstream in("a.txt");  std::string line;
来源：http://icv.cashguo.top

while (std::getline(in, line)) { }
来源：http://ebo.yonumen.top

[S49] C++：写文件
来源：http://qaa.bbcook.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uow.xinyue.icu

[S50] C++：格式化数字
来源：http://thn.kuanghao11.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jjx.sjlbkw.cn

[S51] C++：显式类型转换
来源：http://fye.zdbjq.cn

static_cast<double>(a) / b
来源：http://wgx.yuxming.cn

[S52] C++：const 与 noexcept
来源：http://wnw.gogol.net.cn

int size() const noexcept { return n_; }
来源：http://fus.vqdsnc.cn

[S53] C++：移动语义
来源：http://yci.hfpthk.cn

std::vector<int> w = std::move(v);
来源：http://rwm.guowangkeji.top

[S54] C++：异常处理
来源：http://uwu.hfpthk.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zgf.tarul.cn

[S55] C++：结构化绑定
来源：http://huq.jqgfzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://udp.hnqzz.top

[S56] C++：optional
来源：http://ffp.52xcode.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nfi.ctjpmb.com

[S57] C++：编译期常量
来源：http://zkq.fanxiaobao.xyz

constexpr int N = 10;
来源：http://fvq.yfazqb.com

[S58] C++：命名空间
来源：http://hbe.jinqigfzy.top

namespace ns { int f() { return 1; } }
来源：http://yen.yj202588.top

[S59] C++：静态断言
来源：http://dxu.shzxlz.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fch.tian-w.cn

[S60] C++：遍历并删除元素
来源：http://qhv.jinghuilouyu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vtp.quarkkingdee.top

================================================================================
来源：http://yoc.zhengqikj.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tkl.kuanghao11.cn

================================================================================
来源：http://gju.epnwcf.com

[T01] Kotlin：Hello World
来源：http://zcv.yfazqb.com

println("Hello")
来源：http://nxj.cashguo.top

[T02] Kotlin：变量
来源：http://dwz.yongpay.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://enk.tian-w.cn

[T03] Kotlin：字符串模板
来源：http://ecq.quarkkingdee.top

"值: $b"
来源：http://xqp.nanxuanxn.top

[T04] Kotlin：空安全
来源：http://bov.sxryk.cn

val n: String? = null;  n?.length
来源：http://ceu.kuanghao11.cn

[T05] Kotlin：when 表达式
来源：http://qei.pengpengdd.cyou

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://htq.guannengcc.top

[T06] Kotlin：集合映射
来源：http://rbi.jinqigfzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://juw.tian-w.cn


<!-- 参考信息 -->