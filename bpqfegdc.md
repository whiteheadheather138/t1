代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rzp.yvedp.cn

[R10] 正则匹配
来源：http://cyg.xuetiantiany.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wak.yuxming.cn

[R11] case 多分支
来源：http://mvr.jyoumei.cn

case "$1" in
来源：http://jwe.epnwcf.com

start) echo "启动" ;;
来源：http://wbj.zhongyouzk.top

stop)  echo "停止" ;;
来源：http://fyx.feifeiyinyue.top

*)     echo "未知命令" ;;
来源：http://ocv.gzhubu.top

esac
来源：http://ypz.fzhhl.top

[R12] for 遍历文件
来源：http://dtc.shuidangran.top

for f in *.txt; do echo "$f"; done
来源：http://wlw.yonumen.top

[R13] for 计数循环
来源：http://agb.nanxinkj.top

for i in {1..10}; do echo "$i"; done
来源：http://sgc.guowangkeji.top

[R14] C 风格 for
来源：http://smr.chenzaomai.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tbc.chenlongwang.top

[R15] while 逐行读文件
来源：http://bmn.pengpengdd.cyou

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rss.jyoumei.cn

[R16] until 等待条件
来源：http://zox.iojbl.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mnj.fanxiaobao.xyz

[R17] 数组定义与取值
来源：http://tlk.jinghuilouyu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://tld.52xcode.cn

[R18] 遍历数组
来源：http://ryu.andypj.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bye.tianlin.xyz

[R19] 数组长度
来源：http://wds.gogol.net.cn

echo "${#arr[@]}"
来源：http://jlc.zhiwuduotai.top

[R20] 关联数组（字典）
来源：http://pmr.chenlongwang.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://snb.gotoacloud.top

[R21] 字符串长度
来源：http://gbt.jinqigufen.top

echo "${#s}"
来源：http://xnl.bbcook.cn

[R22] 截取子串
来源：http://tkf.zhongyouzk.top

echo "${s:0:5}"
来源：http://kmf.sweek.top

[R23] 字符串替换
来源：http://wfz.hongshengwenyu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://utt.ivvv.top

[R24] 大小写转换
来源：http://jnx.quarkkingdee.top

echo "${s^^}"; echo "${s,,}"
来源：http://fia.jiagoushi.top

[R25] 去后缀 / 去前缀
来源：http://onj.zhaomingkeji.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://fmk.iojbl.cn

[R26] 命令替换
来源：http://bnf.jianghu66.top

now=$(date +%F); echo "$now"
来源：http://zjm.nanxuanxn.top

[R27] 算术展开
来源：http://vut.jqgfzy.top

echo $((1 + 2 * 3))
来源：http://ohk.cheryme.top

[R28] 浮点运算
来源：http://mdb.xingfuxueyuan.xyz

echo "scale=2; 10/3" | bc
来源：http://nnf.hammf.cn

[R29] 定义函数
来源：http://jya.yonumen.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xvi.cdnleiting.top

[R30] 函数返回状态码
来源：http://cmi.tianlin.xyz

f() { return 0; }; f || echo "失败了"
来源：http://aon.wangdashe.top

[R31] 局部变量
来源：http://jmc.fehbvm.com

f() { local x=1; echo "$x"; }
来源：http://mzn.pengpengdd.cyou

[R32] 参数个数校验
来源：http://ynz.ivvv.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oqj.dianchejie.cn

[R33] 捕获错误并提示行号
来源：http://zwr.iojbl.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rpi.jqgufenzy.top

[R34] 退出时清理
来源：http://djr.tianlin.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://ods.shuidangran.top

[R35] 后台执行并等待
来源：http://ker.daria6918.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kht.yj20258888.top

[R36] 并发执行多个任务
来源：http://jpn.yj20258.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fdc.pycfn.com

[R37] 把输出赋给变量
来源：http://ogm.pengpengdd.cyou

files=$(ls -1)
来源：http://ohj.jyoumei.cn

[R38] 管道串联
来源：http://lzr.ppjwa.cn

cat a.txt | grep -i error | wc -l
来源：http://fgd.aizwys.cn

[R39] 重定向标准输出与错误
来源：http://zgi.yueranfly.top

cmd > out.log 2>&1
来源：http://btg.gzhubu.top

[R40] 追加写日志
来源：http://vqf.ywan-chungtsiang.top

echo "log" >> out.log
来源：http://lzi.yuxming.cn

[R41] 丢弃输出
来源：http://kwn.svipenyu.cn

cmd >/dev/null 2>&1
来源：http://knd.hesvh.cn

[R42] 输入重定向
来源：http://xhg.birdmap.top

wc -l < a.txt
来源：http://nlb.pengpengdd.cyou

[R43] 按名字查找文件
来源：http://sfk.nanxuanxn.top

find . -name "*.log" -type f
来源：http://hen.sweek.top

[R44] 按修改时间查找
来源：http://eyn.wangshuangyany.cn

find . -mtime -7 -type f
来源：http://htg.yfazqb.com

[R45] 批量删除
来源：http://rcg.zhixingplan.top

find . -name "*.tmp" -delete
来源：http://vjs.nwbrower.top

[R46] 递归替换文件内容
来源：http://prn.andypj.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ntt.gzhubu.top

[R47] sed 单行替换
来源：http://zjz.svipenyu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nhb.quarkkingdee.top

[R48] awk 取指定列
来源：http://tdv.zycfv.cn

awk '{print $1, $3}' a.txt
来源：http://wfl.shangyingyoupin.top

[R49] awk 带条件
来源：http://rrc.ydzc1.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wpu.jlsjyb.cn

[R50] awk 求和
来源：http://tyq.hysaishi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://enn.meibo888.top

[R51] 排序去重取前几
来源：http://fom.jinghuilouyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://otb.gotoacloud.top

[R52] 统计行数
来源：http://stl.epnwcf.com

wc -l a.txt
来源：http://msd.redwolf501.top

[R53] 查看文件头与实时尾
来源：http://ftf.chenjidiqi.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://aqi.cheryme.top

[R54] 比较两个文件
来源：http://xmw.yueranfly.top

diff a.txt b.txt
来源：http://nkj.hongshengwenyu.top

[R55] 压缩与解压
来源：http://zsc.zhiwuduotai.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ovf.yvedp.cn

[R56] 远程拷贝
来源：http://glq.cheryme.top

scp file user@host:/path/
来源：http://sjt.gzhubu.top

[R57] 远程执行命令
来源：http://sns.wangshuangyany.cn

ssh user@host 'uptime'
来源：http://amr.pengpengdd.cyou

[R58] 下载文件
来源：http://cwn.jqgfzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oqw.shanyushiyangtech.top

[R59] 发 POST JSON
来源：http://nez.hywenlv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ssw.yj20258888.top

[R60] 只看 HTTP 状态码
来源：http://wsz.meibo888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lbf.xylfe.cn

[R61] 磁盘占用
来源：http://tar.meibo888.top

df -h;  du -sh *
来源：http://pcr.sufxvd.cn

[R62] 找最占空间的文件
来源：http://pkt.hammf.cn

du -ah . | sort -rh | head -10
来源：http://bcn.sjlbkw.cn

[R63] 内存与进程
来源：http://ldz.yanxiufei.cn

free -h;  ps aux | grep nginx
来源：http://icw.daxiang520.top

[R64] 结束进程
来源：http://pid.sufxvd.cn

kill -9 $(pgrep -f app.py)
来源：http://cdj.zhiwuduotai.top

[R65] 查看端口占用
来源：http://nrv.hesvh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gih.epnwcf.com

[R66] 定时任务
来源：http://kko.chenlongwang.top

crontab -e;  crontab -l
来源：http://isi.daria6918.cn

[R67] 生成随机十六进制串
来源：http://zdw.hywenlv.cn

openssl rand -hex 16
来源：http://lxp.zhaomingkeji.xyz

[R68] 计算文件校验值
来源：http://kbp.nwbrower.top

sha256sum a.txt;  md5sum a.txt
来源：http://avl.yueranfly.top

[R69] 生成随机密码
来源：http://ifm.hnqzz.top

head -c 16 /dev/urandom | base64
来源：http://lyz.wangshuangyany.cn

[R70] 时间戳与互转
来源：http://mqe.fanxiaobao.xyz

date +%s;  date -d @1700000000
来源：http://cdv.aizwys.cn

[R71] 日期格式化
来源：http://whe.ydjk.org.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bgu.nanxinkj.top

[R72] 等待端口就绪
来源：http://gna.zhoulong.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://tsz.kuanghao11.cn

[R73] 分割大日志
来源：http://jvd.gzhubu.top

split -l 1000 big.log part_
来源：http://svi.hammf.cn

[R74] 批量重命名
来源：http://bmu.wangshuangyany.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zui.zhongyouzk.top

[R75] 导出环境变量
来源：http://hxw.uphjek.com

export PATH="$HOME/bin:$PATH"
来源：http://rma.zhijiandao.cn

[R76] 使用临时文件
来源：http://mkl.yj20258.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hbv.wangshuangyany.cn

[R77] 读取用户输入
来源：http://dvs.hnxiangtu.top

read -rp "请输入: " ans
来源：http://oxb.jinqigufen.top

[R78] 交互式菜单
来源：http://tol.shanyushiyangtech.top

select opt in a b c; do echo "$opt"; break; done
来源：http://laj.ctjpmb.com

[R79] 解析命令行选项
来源：http://swu.fktsv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lxo.gogol.net.cn

[R80] 查看脚本执行耗时
来源：http://tsr.guowangkeji.top

time ./run.sh
来源：http://ftk.bbcook.cn

================================================================================
来源：http://luc.hongshengwenyu.top

S. C / C++ 专题
来源：http://vow.haohaochexian.top

================================================================================
来源：http://swe.hysaishi.cn

[S01] C：Hello World
来源：http://hjw.bbcook.cn

#include <stdio.h>
来源：http://syb.yuxming.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mej.yj20258.top

[S02] C：变量与格式化输出
来源：http://niv.xylfe.cn

int a = 10; printf("%d\n", a);
来源：http://osj.sweek.top

[S03] C：读入整数
来源：http://gxi.guowangkeji.top

int x; scanf("%d", &x);
来源：http://dbc.ydzc1.top

[S04] C：字符串复制
来源：http://ufn.316326.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://ntd.zhiwuduotai.top

[S05] C：字符串长度
来源：http://kkm.jianghu66.top

strlen(s)
来源：http://vol.hcnkem.com

[S06] C：字符串比较
来源：http://qhw.guannengcc.top

strcmp(a, b) == 0
来源：http://ttv.gogol.net.cn

[S07] C：数组遍历求和
来源：http://bov.cqqwz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qrw.guowangkeji.top

[S08] C：动态内存分配与释放
来源：http://utv.hfpthk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://udq.yj202588.top

[S09] C：结构体定义与初始化
来源：http://ztz.guannengcc.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dwu.cheryme.top

[S10] C：指针与解引用
来源：http://qot.tian-w.cn

int *p = &a;  *p = 5;
来源：http://scn.zhijiandao.cn

[S11] C：逐行读文件
来源：http://tai.guowangkeji.top

FILE *f = fopen("a.txt", "r");
来源：http://lui.zhixingplan.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://pyx.vehdjk.com

fclose(f);
来源：http://tqy.chenzaomai.com

[S12] C：写文件
来源：http://vfy.vehdjk.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://joq.tanke756.top

[S13] C：宏定义
来源：http://lzy.zhiwuduotai.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qfv.bbcook.cn

[S14] C：枚举
来源：http://dxj.hesvh.cn

enum Color { RED, GREEN, BLUE };
来源：http://upx.sysykeji.top

[S15] C：类型转换
来源：http://rev.hnxiangtu.top

(double) a / b
来源：http://bxb.ybcxt.top

[S16] C：位操作置位
来源：http://lvu.feifeiyinyue.top

x |= (1 << 3);
来源：http://vhl.cashguo.top

[S17] C：安全拼接字符串
来源：http://mhw.jinqigufen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://njj.yangfankeji.com

[S18] C：命令行参数
来源：http://jzq.vqdsnc.cn

int main(int argc, char **argv)
来源：http://rum.feifeiyinyue.top

[S19] C：快速排序
来源：http://awa.pycfn.com

qsort(a, n, sizeof(int), cmp);
来源：http://lvq.hammf.cn

[S20] C：二分查找
来源：http://xqt.ywan-chungtsiang.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tyc.vqdsnc.cn

[S21] C：字符类别判断
来源：http://cwi.uphjek.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ftr.jqgufenzy.top

[S22] C：字符串转数字
来源：http://eds.shangyingyoupin.top

atoi("42");  strtod("3.14", NULL);
来源：http://ovm.daria6918.cn

[S23] C：随机数
来源：http://xuu.epnwcf.com

srand(time(NULL));  int r = rand() % 100;
来源：http://oqi.hfpthk.cn

[S24] C：获取本地时间
来源：http://idd.yongpay.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://erl.guowangkeji.top

[S25] C：内存拷贝
来源：http://psi.aizwys.cn

memcpy(dst, src, n);
来源：http://auo.yangfankeji.com

[S26] C：内存清零
来源：http://akd.hysaishi.cn

memset(a, 0, sizeof a);
来源：http://cze.chenzaomai.com

[S27] C：定义常量
来源：http://vxr.zycfv.cn

const double PI = 3.14159;
来源：http://hml.meibo888.top

[S28] C：静态变量
来源：http://bfh.hongshengwenyu.top

static int counter = 0;
来源：http://zir.cheryme.top

[S29] C：变参函数
来源：http://vsa.gogol.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tmp.xingfuxueyuan.xyz

[S30] C：头文件保护
来源：http://bhq.xinyue.icu

#ifndef X_H
来源：http://kjy.pycfn.com

#define X_H
来源：http://jim.hfpthk.cn

#endif
来源：http://vwf.sweek.top

[S31] C++：Hello World
来源：http://rcp.yj20258888.top

#include <iostream>
来源：http://bxk.9152youxi.cn

int main() { std::cout << "Hello\n"; }
来源：http://srj.jiagoushi.top

[S32] C++：字符串
来源：http://ymv.ywan-chungtsiang.top

std::string s = "hi";  s += "!";
来源：http://gqi.yuxming.cn

[S33] C++：vector 增删
来源：http://pnz.dianchejie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://spn.zhoulong.xyz

[S34] C++：遍历 vector
来源：http://gzm.chenjidiqi.icu

for (auto &x : v) { std::cout << x; }
来源：http://mlp.zhiwuduotai.top

[S35] C++：map
来源：http://pzo.chenzaomai.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wef.snrcjt.cn

[S36] C++：unordered_map
来源：http://nfs.haohaochexian.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vsj.9152youxi.cn

[S37] C++：set
来源：http://qmn.zhaomingkeji.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dmk.hysaishi.cn

[S38] C++：排序
来源：http://spi.gotoacloud.top

std::sort(v.begin(), v.end());
来源：http://aeo.9152youxi.cn

[S39] C++：自定义比较器排序
来源：http://idb.shanyushiyangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://knu.shuidangran.top

[S40] C++：查找元素
来源：http://ljq.shanyushiyangkeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://okp.zdbjq.cn

[S41] C++：类与构造函数
来源：http://soo.wangshuangyany.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fwn.zhengqikj.top

[S42] C++：继承与虚函数
来源：http://liv.meibo888.top

class B : public Base { public: void f() override {} };
来源：http://xwn.xuanzx.com

[S43] C++：智能指针
来源：http://vqz.ppjwa.cn

auto p = std::make_unique<int>(5);
来源：http://pno.redwolf501.top

[S44] C++：引用传参
来源：http://qmj.aizwys.cn

void inc(int &x) { ++x; }
来源：http://spi.yanxiufei.cn

[S45] C++：lambda
来源：http://wkq.redwolf501.top

auto add = [](int a, int b) { return a + b; };
来源：http://vva.tianlin.xyz

[S46] C++：函数模板
来源：http://kmm.zhengqikj.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vki.nanxinkj.top

[S47] C++：结构化绑定遍历
来源：http://qrr.jinghuilouyu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lmi.zdqjudy.top

[S48] C++：逐行读文件
来源：http://syo.fehbvm.com

std::ifstream in("a.txt");  std::string line;
来源：http://daw.shanyushiyangtech.top

while (std::getline(in, line)) { }
来源：http://scq.nwbrower.top

[S49] C++：写文件
来源：http://ktl.shangyingyoupin.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ykv.yangfankeji.com

[S50] C++：格式化数字
来源：http://hpf.bjfxy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vys.cheryme.top

[S51] C++：显式类型转换
来源：http://nuq.fanxiaobao.xyz

static_cast<double>(a) / b
来源：http://zcp.yueranfly.top

[S52] C++：const 与 noexcept
来源：http://dvz.yongpay.top

int size() const noexcept { return n_; }
来源：http://vby.ywan-chungtsiang.top

[S53] C++：移动语义
来源：http://uzq.cashguo.top

std::vector<int> w = std::move(v);
来源：http://ici.smart0.xyz

[S54] C++：异常处理
来源：http://asj.sysykeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yrj.wangshuangyany.cn

[S55] C++：结构化绑定
来源：http://qgs.hongshengwenyu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tct.zhengqikj.top

[S56] C++：optional
来源：http://rzq.yj20258888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ghb.jinghuilouyu.cn

[S57] C++：编译期常量
来源：http://duv.52xcode.cn

constexpr int N = 10;
来源：http://vhc.shanyushiyangtech.top

[S58] C++：命名空间
来源：http://zoi.gogol.net.cn

namespace ns { int f() { return 1; } }
来源：http://nye.gogol.net.cn

[S59] C++：静态断言
来源：http://tzs.yvedp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yjh.fktsv.cn

[S60] C++：遍历并删除元素
来源：http://yfz.fanxiaobao.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mrm.gaohongyu789.top

================================================================================
来源：http://whd.smart0.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rll.feifeiyinyue.top

================================================================================
来源：http://rdp.yuanzhike.top

[T01] Kotlin：Hello World
来源：http://qyk.shangyingyoupin.top

println("Hello")
来源：http://axf.bbcook.cn

[T02] Kotlin：变量
来源：http://rgc.cheryme.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wsx.sweek.top

[T03] Kotlin：字符串模板
来源：http://hkn.gotoacloud.top

"值: $b"
来源：http://fbv.hnxiangtu.top

[T04] Kotlin：空安全
来源：http://nak.aibaodan.cn

val n: String? = null;  n?.length
来源：http://jph.hfpthk.cn

[T05] Kotlin：when 表达式
来源：http://rxp.ivvv.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uuo.birdmap.top

[T06] Kotlin：集合映射
来源：http://hym.haohaochexian.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rrh.dianchejie.cn

[T07] Kotlin：集合过滤
来源：http://ujd.gzhubu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kqu.chenlongwang.top

[T08] Kotlin：数据类
来源：http://shi.tarul.cn

data class User(val name: String, val age: Int)
来源：http://rap.nanxuanxn.top

[T09] Kotlin：扩展函数
来源：http://wbj.zhoulong.xyz

fun String.exclaim() = this + "!"
来源：http://mou.gaohongyu789.top

[T10] Kotlin：默认参数
来源：http://sab.zhiwuduotai.top

fun greet(name: String = "World") = "Hi $name"
来源：http://trh.gaohongyu789.top


<!-- 参考信息 -->