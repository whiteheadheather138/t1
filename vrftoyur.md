代发 wailian999

readonly PI=3.14
来源：http://pfi.ehwqpu.com

[R04] 位置参数
来源：http://sxy.andypj.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mwr.jinyuanbaomall.cn

[R05] 参数默认值
来源：http://vje.jinqigfzy.top

name="${1:-default}"
来源：http://yur.ppjwa.cn

[R06] 判断命令是否存在
来源：http://ojj.yuanzhike.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hnq.xinyue.icu

[R07] if 判断文件
来源：http://kkp.fanxiaobao.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ypy.yj202588.top

[R08] 数值比较
来源：http://hcp.fanxiaobao.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://yww.guowangkeji.top

[R09] 字符串比较
来源：http://eaq.jqgufenzy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tmo.daria6918.cn

[R10] 正则匹配
来源：http://phn.ivvv.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cmu.feifeiyinyue.top

[R11] case 多分支
来源：http://ebq.hfpthk.cn

case "$1" in
来源：http://pae.yonumen.top

start) echo "启动" ;;
来源：http://yna.dianchejie.cn

stop)  echo "停止" ;;
来源：http://qwj.jinqigfzy.top

*)     echo "未知命令" ;;
来源：http://nrd.xziqi.cn

esac
来源：http://rhj.iojbl.cn

[R12] for 遍历文件
来源：http://fkj.snrcjt.cn

for f in *.txt; do echo "$f"; done
来源：http://rve.jinghuilouyu.cn

[R13] for 计数循环
来源：http://wol.hcnkem.com

for i in {1..10}; do echo "$i"; done
来源：http://ywr.ppjwa.cn

[R14] C 风格 for
来源：http://aou.guannengcc.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yyb.sweek.top

[R15] while 逐行读文件
来源：http://zva.tarul.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nrn.yueranfly.top

[R16] until 等待条件
来源：http://ejy.sysykeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uri.jinqigufen.top

[R17] 数组定义与取值
来源：http://bpv.chenjidiqi.icu

arr=(a b c); echo "${arr[0]}"
来源：http://ktl.wangshuangyany.cn

[R18] 遍历数组
来源：http://qzg.yuxming.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dew.ppjwa.cn

[R19] 数组长度
来源：http://nev.chenzaomai.com

echo "${#arr[@]}"
来源：http://rbt.chenjidiqi.icu

[R20] 关联数组（字典）
来源：http://xfh.hammf.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bht.nwbrower.top

[R21] 字符串长度
来源：http://pit.jlsjyb.cn

echo "${#s}"
来源：http://vxl.shuidangran.top

[R22] 截取子串
来源：http://vra.zdqjudy.top

echo "${s:0:5}"
来源：http://bpl.shanyushiyangkeji.top

[R23] 字符串替换
来源：http://lsv.tarul.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dhd.cdnleiting.top

[R24] 大小写转换
来源：http://evu.c1oappe.top

echo "${s^^}"; echo "${s,,}"
来源：http://yjx.cqqwz.cn

[R25] 去后缀 / 去前缀
来源：http://mxi.jqgufenzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://tyu.sxryk.cn

[R26] 命令替换
来源：http://zcx.shanyushiyangkeji.top

now=$(date +%F); echo "$now"
来源：http://nez.zhengqikj.top

[R27] 算术展开
来源：http://giy.316326.xyz

echo $((1 + 2 * 3))
来源：http://yrm.nwbrower.top

[R28] 浮点运算
来源：http://tww.sweek.top

echo "scale=2; 10/3" | bc
来源：http://kcj.cheryme.top

[R29] 定义函数
来源：http://fxj.hnxiangtu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qay.aibaodan.cn

[R30] 函数返回状态码
来源：http://vzb.svipenyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://flp.fktsv.cn

[R31] 局部变量
来源：http://iuh.daria6918.cn

f() { local x=1; echo "$x"; }
来源：http://imn.zhaomingkeji.xyz

[R32] 参数个数校验
来源：http://rpd.gaohongyu789.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yic.hesvh.cn

[R33] 捕获错误并提示行号
来源：http://muv.jianghu66.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ibi.tanke756.top

[R34] 退出时清理
来源：http://ofz.ivvv.top

trap 'rm -f "$tmp"' EXIT
来源：http://oaf.zhaomingkeji.xyz

[R35] 后台执行并等待
来源：http://ses.ppjwa.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dhy.sxryk.cn

[R36] 并发执行多个任务
来源：http://onv.zhaomingkeji.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rjb.sysykeji.top

[R37] 把输出赋给变量
来源：http://zkz.bjfxy.top

files=$(ls -1)
来源：http://yhz.wangdashe.top

[R38] 管道串联
来源：http://xjt.cqqwz.cn

cat a.txt | grep -i error | wc -l
来源：http://bir.yj20258888.top

[R39] 重定向标准输出与错误
来源：http://ueu.svipenyu.cn

cmd > out.log 2>&1
来源：http://bac.shangyingyoupin.top

[R40] 追加写日志
来源：http://asv.cqqwz.cn

echo "log" >> out.log
来源：http://xlu.redwolf501.top

[R41] 丢弃输出
来源：http://jiy.gaohongyu789.top

cmd >/dev/null 2>&1
来源：http://uhx.yfazqb.com

[R42] 输入重定向
来源：http://qpe.xinyue.icu

wc -l < a.txt
来源：http://dmk.daxiang520.top

[R43] 按名字查找文件
来源：http://vxj.9152youxi.cn

find . -name "*.log" -type f
来源：http://dhl.kuanghao11.cn

[R44] 按修改时间查找
来源：http://pqc.zhixingplan.top

find . -mtime -7 -type f
来源：http://hym.xziqi.cn

[R45] 批量删除
来源：http://gnv.shzxlz.cn

find . -name "*.tmp" -delete
来源：http://pkm.smart0.xyz

[R46] 递归替换文件内容
来源：http://voj.epnwcf.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ssb.smart0.xyz

[R47] sed 单行替换
来源：http://jbq.xinyue.icu

sed -i 's/foo/bar/g' a.txt
来源：http://vvt.jinyuanbaomall.cn

[R48] awk 取指定列
来源：http://cpf.shanyushiyangtech.top

awk '{print $1, $3}' a.txt
来源：http://qfs.hcnkem.com

[R49] awk 带条件
来源：http://klp.hcnkem.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://htv.bjfxy.top

[R50] awk 求和
来源：http://evv.fzhhl.top

awk '{s += $2} END {print s}' a.txt
来源：http://zlt.jlsjyb.cn

[R51] 排序去重取前几
来源：http://lgb.yueranfly.top

sort a.txt | uniq -c | sort -rn | head
来源：http://cyd.zhengqikj.top

[R52] 统计行数
来源：http://zzn.0kj1m.cn

wc -l a.txt
来源：http://eoh.ivvv.top

[R53] 查看文件头与实时尾
来源：http://odl.hysaishi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://njz.daxiang520.top

[R54] 比较两个文件
来源：http://nam.xuetiantiany.cn

diff a.txt b.txt
来源：http://uye.chenjidiqi.icu

[R55] 压缩与解压
来源：http://rpa.hongshengwenyu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kuk.zhengqikj.top

[R56] 远程拷贝
来源：http://omg.havefunace.top

scp file user@host:/path/
来源：http://itu.shanyushiyangkeji.top

[R57] 远程执行命令
来源：http://rni.fengsongda.top

ssh user@host 'uptime'
来源：http://son.jqgfzy.top

[R58] 下载文件
来源：http://mqm.jyoumei.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wyj.gotoacloud.top

[R59] 发 POST JSON
来源：http://ydz.fehbvm.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://esv.guannengcc.top

[R60] 只看 HTTP 状态码
来源：http://liq.quarkkingdee.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://djf.jiagoushi.top

[R61] 磁盘占用
来源：http://kbu.zhiwuduotai.top

df -h;  du -sh *
来源：http://jng.snrcjt.cn

[R62] 找最占空间的文件
来源：http://bls.yuxming.cn

du -ah . | sort -rh | head -10
来源：http://vor.yongpay.top

[R63] 内存与进程
来源：http://gbk.chenzaomai.com

free -h;  ps aux | grep nginx
来源：http://nfx.yuxming.cn

[R64] 结束进程
来源：http://dfi.zhoulong.xyz

kill -9 $(pgrep -f app.py)
来源：http://vww.shuidangran.top

[R65] 查看端口占用
来源：http://dqp.redwolf501.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bvo.shzxlz.cn

[R66] 定时任务
来源：http://dyb.fengsongda.top

crontab -e;  crontab -l
来源：http://vkc.ivvv.top

[R67] 生成随机十六进制串
来源：http://fvh.jinghuilouyu.cn

openssl rand -hex 16
来源：http://hkp.yj20258.top

[R68] 计算文件校验值
来源：http://owr.zdqjudy.top

sha256sum a.txt;  md5sum a.txt
来源：http://dfm.shzxlz.cn

[R69] 生成随机密码
来源：http://tzu.gogol.net.cn

head -c 16 /dev/urandom | base64
来源：http://syl.nanxinkj.top

[R70] 时间戳与互转
来源：http://jdq.chenjidiqi.icu

date +%s;  date -d @1700000000
来源：http://fuz.tian-w.cn

[R71] 日期格式化
来源：http://cpa.cdnleiting.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://wqf.haohaochexian.top

[R72] 等待端口就绪
来源：http://zjf.andypj.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://eke.zdqjudy.top

[R73] 分割大日志
来源：http://mbd.zhaomingkeji.xyz

split -l 1000 big.log part_
来源：http://vkz.yuanzhike.top

[R74] 批量重命名
来源：http://hit.haohaochexian.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://eyo.shanyushiyangkeji.top

[R75] 导出环境变量
来源：http://ldl.52xcode.cn

export PATH="$HOME/bin:$PATH"
来源：http://glv.ivvv.top

[R76] 使用临时文件
来源：http://clm.guannengcc.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ipy.yueranfly.top

[R77] 读取用户输入
来源：http://ysg.jyoumei.cn

read -rp "请输入: " ans
来源：http://ggd.redwolf501.top

[R78] 交互式菜单
来源：http://vac.wangdashe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xei.redwolf501.top

[R79] 解析命令行选项
来源：http://dew.sjlbkw.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eky.yueranfly.top

[R80] 查看脚本执行耗时
来源：http://tnc.ybcxt.top

time ./run.sh
来源：http://dkl.zhixingplan.top

================================================================================
来源：http://kfa.xuanzx.com

S. C / C++ 专题
来源：http://awp.svipenyu.cn

================================================================================
来源：http://zsr.cdnleiting.top

[S01] C：Hello World
来源：http://sqa.tarul.cn

#include <stdio.h>
来源：http://tyu.yanxiufei.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qda.yonumen.top

[S02] C：变量与格式化输出
来源：http://wht.yj20258.top

int a = 10; printf("%d\n", a);
来源：http://zso.aizwys.cn

[S03] C：读入整数
来源：http://vta.jqgfzy.top

int x; scanf("%d", &x);
来源：http://lli.yongpay.top

[S04] C：字符串复制
来源：http://sgg.cashguo.top

char dst[32]; strcpy(dst, "hi");
来源：http://zvq.wangshuangyany.cn

[S05] C：字符串长度
来源：http://qar.dashuyun.cn

strlen(s)
来源：http://gdb.daria6918.cn

[S06] C：字符串比较
来源：http://zvw.guowangkeji.top

strcmp(a, b) == 0
来源：http://jhg.zhijiandao.cn

[S07] C：数组遍历求和
来源：http://ixy.ydjk.org.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jps.yj20258.top

[S08] C：动态内存分配与释放
来源：http://atv.jiagoushi.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qdc.quarkkingdee.top

[S09] C：结构体定义与初始化
来源：http://ilm.zhoulong.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ilx.shanyushiyangkeji.top

[S10] C：指针与解引用
来源：http://coy.fanxiaobao.xyz

int *p = &a;  *p = 5;
来源：http://mkm.hongshengwenyu.top

[S11] C：逐行读文件
来源：http://vxn.sxryk.cn

FILE *f = fopen("a.txt", "r");
来源：http://fry.uphjek.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://fyq.iojbl.cn

fclose(f);
来源：http://klo.sysykeji.top

[S12] C：写文件
来源：http://fnz.havefunace.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nmz.tanke756.top

[S13] C：宏定义
来源：http://itz.snrcjt.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ezc.cheryme.top

[S14] C：枚举
来源：http://kkh.jqgufenzy.top

enum Color { RED, GREEN, BLUE };
来源：http://ubz.daxiang520.top

[S15] C：类型转换
来源：http://igc.andypj.xyz

(double) a / b
来源：http://gsn.chenzaomai.com

[S16] C：位操作置位
来源：http://ocp.tian-w.cn

x |= (1 << 3);
来源：http://bua.hfpthk.cn

[S17] C：安全拼接字符串
来源：http://bhg.hammf.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ggd.sysykeji.top

[S18] C：命令行参数
来源：http://rfj.daxiang520.top

int main(int argc, char **argv)
来源：http://sml.xziqi.cn

[S19] C：快速排序
来源：http://wlx.pycfn.com

qsort(a, n, sizeof(int), cmp);
来源：http://brc.hammf.cn

[S20] C：二分查找
来源：http://crs.hywenlv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ion.zhiwuduotai.top

[S21] C：字符类别判断
来源：http://uzd.ydjk.org.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pox.zhengqikj.top

[S22] C：字符串转数字
来源：http://tkh.yueranfly.top

atoi("42");  strtod("3.14", NULL);
来源：http://pnz.gotoacloud.top

[S23] C：随机数
来源：http://tym.cashguo.top

srand(time(NULL));  int r = rand() % 100;
来源：http://uer.ivvv.top

[S24] C：获取本地时间
来源：http://ffc.zhengqikj.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qca.xingfuxueyuan.xyz

[S25] C：内存拷贝
来源：http://wtc.sjlbkw.cn

memcpy(dst, src, n);
来源：http://gpl.guannengcc.top

[S26] C：内存清零
来源：http://dcj.yfazqb.com

memset(a, 0, sizeof a);
来源：http://uaa.daxiang520.top

[S27] C：定义常量
来源：http://xgb.yj202588.top

const double PI = 3.14159;
来源：http://lac.ybcxt.top

[S28] C：静态变量
来源：http://clh.yanxiufei.cn

static int counter = 0;
来源：http://uia.xziqi.cn

[S29] C：变参函数
来源：http://dji.jqgfzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://olv.tarul.cn

[S30] C：头文件保护
来源：http://hgc.hfpthk.cn

#ifndef X_H
来源：http://txw.shanyushiyangkeji.top

#define X_H
来源：http://nbz.smart0.xyz

#endif
来源：http://pdx.cqqwz.cn

[S31] C++：Hello World
来源：http://rmr.jyoumei.cn

#include <iostream>
来源：http://exd.hesvh.cn

int main() { std::cout << "Hello\n"; }
来源：http://ops.xinyue.icu

[S32] C++：字符串
来源：http://euc.iojbl.cn

std::string s = "hi";  s += "!";
来源：http://nyw.hnqzz.top

[S33] C++：vector 增删
来源：http://oxe.sxryk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zkc.ywan-chungtsiang.top

[S34] C++：遍历 vector
来源：http://yri.zdbjq.cn

for (auto &x : v) { std::cout << x; }
来源：http://lfb.ivvv.top

[S35] C++：map
来源：http://zag.ppjwa.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gjx.havefunace.top

[S36] C++：unordered_map
来源：http://odf.shanyushiyangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://eyf.svipenyu.cn

[S37] C++：set
来源：http://wdi.zhiwuduotai.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eio.uphjek.com

[S38] C++：排序
来源：http://nlf.xuanzx.com

std::sort(v.begin(), v.end());
来源：http://edi.smart0.xyz

[S39] C++：自定义比较器排序
来源：http://zmg.nanxinkj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://piq.jinghuilouyu.cn

[S40] C++：查找元素
来源：http://ttl.bjfxy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cgn.c1oappe.top

[S41] C++：类与构造函数
来源：http://upu.wangdashe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tna.hywenlv.cn

[S42] C++：继承与虚函数
来源：http://bmm.bjfxy.top

class B : public Base { public: void f() override {} };
来源：http://cvx.svipenyu.cn

[S43] C++：智能指针
来源：http://koz.chenzaomai.com

auto p = std::make_unique<int>(5);
来源：http://rao.wangshuangyany.cn

[S44] C++：引用传参
来源：http://ona.ydjk.org.cn

void inc(int &x) { ++x; }
来源：http://eya.tian-w.cn

[S45] C++：lambda
来源：http://lnz.bjfxy.top

auto add = [](int a, int b) { return a + b; };
来源：http://jca.feifeiyinyue.top

[S46] C++：函数模板
来源：http://hga.sufxvd.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tls.yfazqb.com

[S47] C++：结构化绑定遍历
来源：http://nnd.uphjek.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ont.ivvv.top

[S48] C++：逐行读文件
来源：http://qfw.hongshengwenyu.top

std::ifstream in("a.txt");  std::string line;
来源：http://gvw.andypj.xyz

while (std::getline(in, line)) { }
来源：http://nrl.yj20258888.top

[S49] C++：写文件
来源：http://cgp.vehdjk.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lnp.gzhubu.top

[S50] C++：格式化数字
来源：http://heb.hongshengwenyu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zhz.zhijiandao.cn

[S51] C++：显式类型转换
来源：http://jyg.zhengqikj.top

static_cast<double>(a) / b
来源：http://ejh.yfazqb.com

[S52] C++：const 与 noexcept
来源：http://bpi.hywenlv.cn

int size() const noexcept { return n_; }
来源：http://pot.dianchejie.cn

[S53] C++：移动语义
来源：http://epn.yongpay.top

std::vector<int> w = std::move(v);
来源：http://rsw.hywenlv.cn

[S54] C++：异常处理
来源：http://cax.kuanghao11.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ech.meibo888.top

[S55] C++：结构化绑定
来源：http://tzw.xziqi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://avp.meibo888.top

[S56] C++：optional
来源：http://hgh.hywenlv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://adk.yonumen.top

[S57] C++：编译期常量
来源：http://qmd.xylfe.cn

constexpr int N = 10;
来源：http://phn.smart0.xyz

[S58] C++：命名空间
来源：http://vbj.snrcjt.cn

namespace ns { int f() { return 1; } }
来源：http://ewj.hnqzz.top

[S59] C++：静态断言
来源：http://aqf.tarul.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://krq.xinyue.icu

[S60] C++：遍历并删除元素
来源：http://fwy.yangfankeji.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pqp.chenzaomai.com

================================================================================
来源：http://uta.fengsongda.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bjr.ybcxt.top

================================================================================
来源：http://bxe.cqqwz.cn

[T01] Kotlin：Hello World
来源：http://dtz.pycfn.com

println("Hello")
来源：http://lov.kuanghao11.cn

[T02] Kotlin：变量
来源：http://ddt.bbcook.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jvc.dashuyun.cn

[T03] Kotlin：字符串模板
来源：http://rtu.fehbvm.com

"值: $b"
来源：http://lnu.sweek.top

[T04] Kotlin：空安全
来源：http://esk.ydzc1.top

val n: String? = null;  n?.length
来源：http://hrv.aibaodan.cn


<!-- 参考信息 -->