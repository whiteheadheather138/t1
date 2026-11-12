代发 wailian999

set -euo pipefail
来源：http://mlb.gaohongyu789.top

[R02] 变量赋值与使用
来源：http://ewg.yj20258888.top

name="Tom"; echo "$name"
来源：http://aau.ydjk.org.cn

[R03] 只读变量
来源：http://hxt.yj20258888.top

readonly PI=3.14
来源：http://duu.xinyue.icu

[R04] 位置参数
来源：http://alt.jlsjyb.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mlj.wangdashe.top

[R05] 参数默认值
来源：http://vhi.nwbrower.top

name="${1:-default}"
来源：http://tjk.fehbvm.com

[R06] 判断命令是否存在
来源：http://lzb.fzhhl.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xhl.vqdsnc.cn

[R07] if 判断文件
来源：http://uqa.kuanghao11.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ubn.vehdjk.com

[R08] 数值比较
来源：http://iam.shuidangran.top

if (( a > b )); then echo "a 更大"; fi
来源：http://gkh.xuetiantiany.cn

[R09] 字符串比较
来源：http://awa.aibaodan.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ffy.tarul.cn

[R10] 正则匹配
来源：http://jim.ppjwa.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jnk.zdbjq.cn

[R11] case 多分支
来源：http://ovz.zhengqikj.top

case "$1" in
来源：http://jxr.guowangkeji.top

start) echo "启动" ;;
来源：http://xaw.yuanzhike.top

stop)  echo "停止" ;;
来源：http://qkh.bjfxy.top

*)     echo "未知命令" ;;
来源：http://civ.9152youxi.cn

esac
来源：http://flk.hnqzz.top

[R12] for 遍历文件
来源：http://gun.hnxiangtu.top

for f in *.txt; do echo "$f"; done
来源：http://ozg.zhijiandao.cn

[R13] for 计数循环
来源：http://edw.zdqjudy.top

for i in {1..10}; do echo "$i"; done
来源：http://ogz.shanyushiyangtech.top

[R14] C 风格 for
来源：http://nlg.wangshuangyany.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://oex.gaohongyu789.top

[R15] while 逐行读文件
来源：http://okz.ivvv.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dci.vqdsnc.cn

[R16] until 等待条件
来源：http://jta.havefunace.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bmd.guowangkeji.top

[R17] 数组定义与取值
来源：http://qqx.cucudq.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zkz.sxryk.cn

[R18] 遍历数组
来源：http://mbg.cqqwz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://trj.hesvh.cn

[R19] 数组长度
来源：http://xlg.bbcook.cn

echo "${#arr[@]}"
来源：http://oxy.hfpthk.cn

[R20] 关联数组（字典）
来源：http://bll.guannengcc.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wup.wangshuangyany.cn

[R21] 字符串长度
来源：http://nap.zdqjudy.top

echo "${#s}"
来源：http://idr.nanxinkj.top

[R22] 截取子串
来源：http://wqa.jinghuilouyu.cn

echo "${s:0:5}"
来源：http://ary.zdbjq.cn

[R23] 字符串替换
来源：http://oex.jqgfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jvb.zdqjudy.top

[R24] 大小写转换
来源：http://bml.kuanghao11.cn

echo "${s^^}"; echo "${s,,}"
来源：http://moj.nanxuanxn.top

[R25] 去后缀 / 去前缀
来源：http://yzt.havefunace.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://pxt.hysaishi.cn

[R26] 命令替换
来源：http://cjm.jinyuanbaomall.cn

now=$(date +%F); echo "$now"
来源：http://syi.hfpthk.cn

[R27] 算术展开
来源：http://qbb.nanxinkj.top

echo $((1 + 2 * 3))
来源：http://ahy.jinqigufen.top

[R28] 浮点运算
来源：http://maw.yanxiufei.cn

echo "scale=2; 10/3" | bc
来源：http://mdi.gzhubu.top

[R29] 定义函数
来源：http://reg.hammf.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nnn.sxryk.cn

[R30] 函数返回状态码
来源：http://oab.yj20258.top

f() { return 0; }; f || echo "失败了"
来源：http://rsz.zhoulong.xyz

[R31] 局部变量
来源：http://ldd.zhongyouzk.top

f() { local x=1; echo "$x"; }
来源：http://ksl.sweek.top

[R32] 参数个数校验
来源：http://guw.xuetiantiany.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fzs.birdmap.top

[R33] 捕获错误并提示行号
来源：http://fkh.jqgfzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eyk.zhiwuduotai.top

[R34] 退出时清理
来源：http://zpz.jlsjyb.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lcm.hfpthk.cn

[R35] 后台执行并等待
来源：http://npm.zhengqikj.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ygj.quarkkingdee.top

[R36] 并发执行多个任务
来源：http://fde.wangshuangyany.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bqr.cashguo.top

[R37] 把输出赋给变量
来源：http://uuh.jyoumei.cn

files=$(ls -1)
来源：http://rtz.cdnleiting.top

[R38] 管道串联
来源：http://ltw.xziqi.cn

cat a.txt | grep -i error | wc -l
来源：http://did.ybcxt.top

[R39] 重定向标准输出与错误
来源：http://jvb.ybcxt.top

cmd > out.log 2>&1
来源：http://gdl.jinqigufen.top

[R40] 追加写日志
来源：http://wje.shangyingyoupin.top

echo "log" >> out.log
来源：http://wvx.ppjwa.cn

[R41] 丢弃输出
来源：http://wyq.jiagoushi.top

cmd >/dev/null 2>&1
来源：http://xch.xingfuxueyuan.xyz

[R42] 输入重定向
来源：http://hmk.nwbrower.top

wc -l < a.txt
来源：http://oqt.aizwys.cn

[R43] 按名字查找文件
来源：http://kig.hnxiangtu.top

find . -name "*.log" -type f
来源：http://pgt.ivvv.top

[R44] 按修改时间查找
来源：http://zfj.redwolf501.top

find . -mtime -7 -type f
来源：http://ncf.gaohongyu789.top

[R45] 批量删除
来源：http://llq.fanxiaobao.xyz

find . -name "*.tmp" -delete
来源：http://qif.bbcook.cn

[R46] 递归替换文件内容
来源：http://orl.jinyuanbaomall.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tyh.yvedp.cn

[R47] sed 单行替换
来源：http://pst.nanxinkj.top

sed -i 's/foo/bar/g' a.txt
来源：http://trx.yueranfly.top

[R48] awk 取指定列
来源：http://zzj.yuxming.cn

awk '{print $1, $3}' a.txt
来源：http://etm.0kj1m.cn

[R49] awk 带条件
来源：http://hkx.0kj1m.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jaq.tanke756.top

[R50] awk 求和
来源：http://clm.ctjpmb.com

awk '{s += $2} END {print s}' a.txt
来源：http://vlu.cheryme.top

[R51] 排序去重取前几
来源：http://usl.gogol.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wwe.sufxvd.cn

[R52] 统计行数
来源：http://xnw.9152youxi.cn

wc -l a.txt
来源：http://zhz.shangyingyoupin.top

[R53] 查看文件头与实时尾
来源：http://svt.aizwys.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://azy.fktsv.cn

[R54] 比较两个文件
来源：http://abw.shuidangran.top

diff a.txt b.txt
来源：http://njc.yonumen.top

[R55] 压缩与解压
来源：http://nhl.yj202588.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lbi.nwbrower.top

[R56] 远程拷贝
来源：http://bgn.daria6918.cn

scp file user@host:/path/
来源：http://pti.tian-w.cn

[R57] 远程执行命令
来源：http://awi.hesvh.cn

ssh user@host 'uptime'
来源：http://koz.gotoacloud.top

[R58] 下载文件
来源：http://bup.jiagoushi.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uya.jyoumei.cn

[R59] 发 POST JSON
来源：http://keq.xuetiantiany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cai.yonumen.top

[R60] 只看 HTTP 状态码
来源：http://pxb.dashuyun.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ilz.jinqigufen.top

[R61] 磁盘占用
来源：http://gtj.xingfuxueyuan.xyz

df -h;  du -sh *
来源：http://fmn.smart0.xyz

[R62] 找最占空间的文件
来源：http://txc.iojbl.cn

du -ah . | sort -rh | head -10
来源：http://owf.pengpengdd.cyou

[R63] 内存与进程
来源：http://igz.jiagoushi.top

free -h;  ps aux | grep nginx
来源：http://uda.vehdjk.com

[R64] 结束进程
来源：http://hyf.mhx1999.top

kill -9 $(pgrep -f app.py)
来源：http://vsg.cucudq.cn

[R65] 查看端口占用
来源：http://wfk.xylfe.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qlb.yueranfly.top

[R66] 定时任务
来源：http://qza.52xcode.cn

crontab -e;  crontab -l
来源：http://bpe.ctjpmb.com

[R67] 生成随机十六进制串
来源：http://pia.9152youxi.cn

openssl rand -hex 16
来源：http://bqh.nanxinkj.top

[R68] 计算文件校验值
来源：http://yie.jyoumei.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bza.ctjpmb.com

[R69] 生成随机密码
来源：http://ndg.ehwqpu.com

head -c 16 /dev/urandom | base64
来源：http://hxw.yj202588.top

[R70] 时间戳与互转
来源：http://xtp.gaohongyu789.top

date +%s;  date -d @1700000000
来源：http://aps.fanxiaobao.xyz

[R71] 日期格式化
来源：http://hah.zycfv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ylx.sweek.top

[R72] 等待端口就绪
来源：http://kzu.aizwys.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zjx.fehbvm.com

[R73] 分割大日志
来源：http://her.nwbrower.top

split -l 1000 big.log part_
来源：http://ubz.guowangkeji.top

[R74] 批量重命名
来源：http://aha.cucudq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ozu.cheryme.top

[R75] 导出环境变量
来源：http://kjn.yuxming.cn

export PATH="$HOME/bin:$PATH"
来源：http://rtr.jlsjyb.cn

[R76] 使用临时文件
来源：http://toj.sxryk.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lnf.jinghuilouyu.cn

[R77] 读取用户输入
来源：http://oax.fanxiaobao.xyz

read -rp "请输入: " ans
来源：http://kqz.hnqzz.top

[R78] 交互式菜单
来源：http://gdd.zycfv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gfg.hfpthk.cn

[R79] 解析命令行选项
来源：http://ftb.daria6918.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hzh.ywan-chungtsiang.top

[R80] 查看脚本执行耗时
来源：http://dci.sysykeji.top

time ./run.sh
来源：http://mhe.daria6918.cn

================================================================================
来源：http://ioq.ybcxt.top

S. C / C++ 专题
来源：http://mwv.dashuyun.cn

================================================================================
来源：http://anj.yvedp.cn

[S01] C：Hello World
来源：http://sgp.guannengcc.top

#include <stdio.h>
来源：http://hqz.fanxiaobao.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://bgw.ehwqpu.com

[S02] C：变量与格式化输出
来源：http://mba.cdnleiting.top

int a = 10; printf("%d\n", a);
来源：http://tsk.fanxiaobao.xyz

[S03] C：读入整数
来源：http://tup.cashguo.top

int x; scanf("%d", &x);
来源：http://pmx.ctjpmb.com

[S04] C：字符串复制
来源：http://yuj.tianlin.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://qlr.yonumen.top

[S05] C：字符串长度
来源：http://feg.yangfankeji.com

strlen(s)
来源：http://nlb.yanxiufei.cn

[S06] C：字符串比较
来源：http://xyi.fzhhl.top

strcmp(a, b) == 0
来源：http://sfl.vehdjk.com

[S07] C：数组遍历求和
来源：http://zsu.dianchejie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dpr.pengpengdd.cyou

[S08] C：动态内存分配与释放
来源：http://hom.sjlbkw.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pry.zhongyouzk.top

[S09] C：结构体定义与初始化
来源：http://pen.dianchejie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zjn.sysykeji.top

[S10] C：指针与解引用
来源：http://ntp.xinyue.icu

int *p = &a;  *p = 5;
来源：http://wwd.dianchejie.cn

[S11] C：逐行读文件
来源：http://lno.nanxuanxn.top

FILE *f = fopen("a.txt", "r");
来源：http://kyh.guowangkeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://gng.xinyue.icu

fclose(f);
来源：http://zdw.sweek.top

[S12] C：写文件
来源：http://bkw.bbcook.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fja.quarkkingdee.top

[S13] C：宏定义
来源：http://ttm.cheryme.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ttm.guannengcc.top

[S14] C：枚举
来源：http://wxe.havefunace.top

enum Color { RED, GREEN, BLUE };
来源：http://fet.uphjek.com

[S15] C：类型转换
来源：http://qih.sweek.top

(double) a / b
来源：http://yra.xuanzx.com

[S16] C：位操作置位
来源：http://bjh.chenjidiqi.icu

x |= (1 << 3);
来源：http://pel.xuanzx.com

[S17] C：安全拼接字符串
来源：http://two.jianghu66.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://saj.yuanzhike.top

[S18] C：命令行参数
来源：http://rfx.cqqwz.cn

int main(int argc, char **argv)
来源：http://ort.xuanzx.com

[S19] C：快速排序
来源：http://fdc.yangfankeji.com

qsort(a, n, sizeof(int), cmp);
来源：http://xeo.uphjek.com

[S20] C：二分查找
来源：http://hxg.yuanzhike.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kku.daria6918.cn

[S21] C：字符类别判断
来源：http://elx.nanxinkj.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://aol.hnqzz.top

[S22] C：字符串转数字
来源：http://zwu.yangfankeji.com

atoi("42");  strtod("3.14", NULL);
来源：http://tik.shanyushiyangkeji.top

[S23] C：随机数
来源：http://lwd.aibaodan.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://omf.jinqigfzy.top

[S24] C：获取本地时间
来源：http://sya.jiagoushi.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://juj.aizwys.cn

[S25] C：内存拷贝
来源：http://ung.vehdjk.com

memcpy(dst, src, n);
来源：http://ssu.chenjidiqi.icu

[S26] C：内存清零
来源：http://nft.zycfv.cn

memset(a, 0, sizeof a);
来源：http://dwm.sweek.top

[S27] C：定义常量
来源：http://onu.zhiwuduotai.top

const double PI = 3.14159;
来源：http://yif.kuanghao11.cn

[S28] C：静态变量
来源：http://typ.meibo888.top

static int counter = 0;
来源：http://cdv.fzhhl.top

[S29] C：变参函数
来源：http://brp.daria6918.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://reg.yueranfly.top

[S30] C：头文件保护
来源：http://ymu.jlsjyb.cn

#ifndef X_H
来源：http://ycj.wangdashe.top

#define X_H
来源：http://mua.mhx1999.top

#endif
来源：http://lxj.hywenlv.cn

[S31] C++：Hello World
来源：http://fve.dashuyun.cn

#include <iostream>
来源：http://ayi.bbcook.cn

int main() { std::cout << "Hello\n"; }
来源：http://jna.fktsv.cn

[S32] C++：字符串
来源：http://ysz.ppjwa.cn

std::string s = "hi";  s += "!";
来源：http://oty.chenjidiqi.icu

[S33] C++：vector 增删
来源：http://gok.zhengqikj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://egx.shanyushiyangkeji.top

[S34] C++：遍历 vector
来源：http://nyz.cheryme.top

for (auto &x : v) { std::cout << x; }
来源：http://bnk.fktsv.cn

[S35] C++：map
来源：http://osb.zhijiandao.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://idx.dashuyun.cn

[S36] C++：unordered_map
来源：http://gwc.zdqjudy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zbb.hywenlv.cn

[S37] C++：set
来源：http://rul.wangshuangyany.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qvp.nanxinkj.top

[S38] C++：排序
来源：http://viz.havefunace.top

std::sort(v.begin(), v.end());
来源：http://pxm.xuanzx.com

[S39] C++：自定义比较器排序
来源：http://wdg.sweek.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fdw.gaohongyu789.top

[S40] C++：查找元素
来源：http://jhb.hnqzz.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sbc.nanxinkj.top

[S41] C++：类与构造函数
来源：http://rvr.hesvh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://aew.shanyushiyangkeji.top

[S42] C++：继承与虚函数
来源：http://kij.shuidangran.top

class B : public Base { public: void f() override {} };
来源：http://cmy.quarkkingdee.top

[S43] C++：智能指针
来源：http://nfc.smart0.xyz

auto p = std::make_unique<int>(5);
来源：http://spw.cashguo.top

[S44] C++：引用传参
来源：http://ptm.bjfxy.top

void inc(int &x) { ++x; }
来源：http://xvk.xuanzx.com

[S45] C++：lambda
来源：http://qqk.52xcode.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cjo.yangfankeji.com

[S46] C++：函数模板
来源：http://blj.gzhubu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wfo.tarul.cn

[S47] C++：结构化绑定遍历
来源：http://efr.zhaomingkeji.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oqs.hfpthk.cn

[S48] C++：逐行读文件
来源：http://oci.xingfuxueyuan.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://xve.kuanghao11.cn

while (std::getline(in, line)) { }
来源：http://wpb.c1oappe.top

[S49] C++：写文件
来源：http://yww.xuetiantiany.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rlg.c1oappe.top

[S50] C++：格式化数字
来源：http://tal.hnqzz.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cpy.sysykeji.top

[S51] C++：显式类型转换
来源：http://dnx.epnwcf.com

static_cast<double>(a) / b
来源：http://fuq.andypj.xyz

[S52] C++：const 与 noexcept
来源：http://oel.ctjpmb.com

int size() const noexcept { return n_; }
来源：http://iko.vqdsnc.cn

[S53] C++：移动语义
来源：http://ejp.fengsongda.top

std::vector<int> w = std::move(v);
来源：http://dza.yvedp.cn

[S54] C++：异常处理
来源：http://tvl.kuanghao11.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jwb.zhixingplan.top

[S55] C++：结构化绑定
来源：http://rkv.jiagoushi.top

auto [a, b] = std::make_pair(1, 2);
来源：http://nvm.pengpengdd.cyou

[S56] C++：optional
来源：http://yql.yj202588.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qmx.guannengcc.top

[S57] C++：编译期常量
来源：http://prz.jyoumei.cn

constexpr int N = 10;
来源：http://gcs.hywenlv.cn

[S58] C++：命名空间
来源：http://eoh.xingfuxueyuan.xyz

namespace ns { int f() { return 1; } }
来源：http://joy.yj202588.top

[S59] C++：静态断言
来源：http://gzn.tarul.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eqi.xylfe.cn

[S60] C++：遍历并删除元素
来源：http://hln.fanxiaobao.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jvx.hfpthk.cn

================================================================================
来源：http://hev.ppjwa.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://psf.shanyushiyangtech.top

================================================================================
来源：http://hdi.shangyingyoupin.top

[T01] Kotlin：Hello World
来源：http://djg.hysaishi.cn

println("Hello")
来源：http://sct.vehdjk.com

[T02] Kotlin：变量
来源：http://ucn.iojbl.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://als.pycfn.com


<!-- 参考信息 -->