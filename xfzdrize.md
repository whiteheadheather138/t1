代发 wailian999

R. Bash 专题
来源：http://tmy.havefunace.top

================================================================================
来源：http://eyr.tarul.cn

[R01] shebang 与严格模式
来源：http://bwz.redwolf501.top

#!/usr/bin/env bash
来源：http://cwb.gzhubu.top

set -euo pipefail
来源：http://hca.shanyushiyangtech.top

[R02] 变量赋值与使用
来源：http://ohe.sxryk.cn

name="Tom"; echo "$name"
来源：http://jsa.nanxuanxn.top

[R03] 只读变量
来源：http://lxh.havefunace.top

readonly PI=3.14
来源：http://amn.sjlbkw.cn

[R04] 位置参数
来源：http://nvg.zdqjudy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pae.hnqzz.top

[R05] 参数默认值
来源：http://zum.c1oappe.top

name="${1:-default}"
来源：http://gjc.jqgufenzy.top

[R06] 判断命令是否存在
来源：http://nfn.daria6918.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://udd.cashguo.top

[R07] if 判断文件
来源：http://agp.zhongyouzk.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vil.zhaomingkeji.xyz

[R08] 数值比较
来源：http://pbh.feifeiyinyue.top

if (( a > b )); then echo "a 更大"; fi
来源：http://gcp.andypj.xyz

[R09] 字符串比较
来源：http://uxf.guowangkeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://msn.gotoacloud.top

[R10] 正则匹配
来源：http://foy.zhijiandao.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fhh.shanyushiyangkeji.top

[R11] case 多分支
来源：http://pze.jinyuanbaomall.cn

case "$1" in
来源：http://lpy.yvedp.cn

start) echo "启动" ;;
来源：http://dal.xingfuxueyuan.xyz

stop)  echo "停止" ;;
来源：http://kvk.gaohongyu789.top

*)     echo "未知命令" ;;
来源：http://wkb.hfpthk.cn

esac
来源：http://gev.fanxiaobao.xyz

[R12] for 遍历文件
来源：http://adt.xuanzx.com

for f in *.txt; do echo "$f"; done
来源：http://qkc.gzhubu.top

[R13] for 计数循环
来源：http://yuh.jinghuilouyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://ipn.shzxlz.cn

[R14] C 风格 for
来源：http://qjb.daxiang520.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bqw.nanxuanxn.top

[R15] while 逐行读文件
来源：http://jay.yj202588.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gbs.9152youxi.cn

[R16] until 等待条件
来源：http://ido.yj20258.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qvg.wangdashe.top

[R17] 数组定义与取值
来源：http://pjc.wangshuangyany.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gyh.gzhubu.top

[R18] 遍历数组
来源：http://chx.dianchejie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gvh.cucudq.cn

[R19] 数组长度
来源：http://psb.havefunace.top

echo "${#arr[@]}"
来源：http://zde.bjfxy.top

[R20] 关联数组（字典）
来源：http://vxr.dianchejie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dsa.ydzc1.top

[R21] 字符串长度
来源：http://suv.yj20258.top

echo "${#s}"
来源：http://lwx.shanyushiyangtech.top

[R22] 截取子串
来源：http://tqj.hnxiangtu.top

echo "${s:0:5}"
来源：http://jcj.shangyingyoupin.top

[R23] 字符串替换
来源：http://exr.yangfankeji.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://psj.feifeiyinyue.top

[R24] 大小写转换
来源：http://hrz.hongshengwenyu.top

echo "${s^^}"; echo "${s,,}"
来源：http://vjl.zdbjq.cn

[R25] 去后缀 / 去前缀
来源：http://lga.aibaodan.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fjn.cucudq.cn

[R26] 命令替换
来源：http://cbm.xziqi.cn

now=$(date +%F); echo "$now"
来源：http://xot.0kj1m.cn

[R27] 算术展开
来源：http://pjq.hfpthk.cn

echo $((1 + 2 * 3))
来源：http://qgf.nanxinkj.top

[R28] 浮点运算
来源：http://aht.jiagoushi.top

echo "scale=2; 10/3" | bc
来源：http://mhn.chenlongwang.top

[R29] 定义函数
来源：http://xtn.pycfn.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pfh.jianghu66.top

[R30] 函数返回状态码
来源：http://hpv.xingfuxueyuan.xyz

f() { return 0; }; f || echo "失败了"
来源：http://rey.mhx1999.top

[R31] 局部变量
来源：http://wmy.hongshengwenyu.top

f() { local x=1; echo "$x"; }
来源：http://epd.wangdashe.top

[R32] 参数个数校验
来源：http://lna.zdqjudy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hif.zhongyouzk.top

[R33] 捕获错误并提示行号
来源：http://rvk.jqgufenzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ecn.birdmap.top

[R34] 退出时清理
来源：http://iyv.hfpthk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fmj.jianghu66.top

[R35] 后台执行并等待
来源：http://vde.uphjek.com

sleep 5 & pid=$!; wait "$pid"
来源：http://tcv.shangyingyoupin.top

[R36] 并发执行多个任务
来源：http://ysi.sxryk.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://akv.jianghu66.top

[R37] 把输出赋给变量
来源：http://jzt.ybcxt.top

files=$(ls -1)
来源：http://ntw.cdnleiting.top

[R38] 管道串联
来源：http://dqi.fehbvm.com

cat a.txt | grep -i error | wc -l
来源：http://hzk.9152youxi.cn

[R39] 重定向标准输出与错误
来源：http://lxh.haohaochexian.top

cmd > out.log 2>&1
来源：http://nop.ppjwa.cn

[R40] 追加写日志
来源：http://ivc.zdqjudy.top

echo "log" >> out.log
来源：http://bqm.zhengqikj.top

[R41] 丢弃输出
来源：http://ndk.daria6918.cn

cmd >/dev/null 2>&1
来源：http://mcs.nanxinkj.top

[R42] 输入重定向
来源：http://nyl.ydjk.org.cn

wc -l < a.txt
来源：http://nuo.smart0.xyz

[R43] 按名字查找文件
来源：http://ilr.fengsongda.top

find . -name "*.log" -type f
来源：http://oon.bbcook.cn

[R44] 按修改时间查找
来源：http://xxf.jqgufenzy.top

find . -mtime -7 -type f
来源：http://lpm.jinqigufen.top

[R45] 批量删除
来源：http://upf.yueranfly.top

find . -name "*.tmp" -delete
来源：http://nmw.ydzc1.top

[R46] 递归替换文件内容
来源：http://ung.uphjek.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rgu.mhx1999.top

[R47] sed 单行替换
来源：http://qkc.feifeiyinyue.top

sed -i 's/foo/bar/g' a.txt
来源：http://oja.zhoulong.xyz

[R48] awk 取指定列
来源：http://ixn.pycfn.com

awk '{print $1, $3}' a.txt
来源：http://qon.shanyushiyangkeji.top

[R49] awk 带条件
来源：http://dzy.cqqwz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lkw.pycfn.com

[R50] awk 求和
来源：http://yzk.xylfe.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vns.ydzc1.top

[R51] 排序去重取前几
来源：http://jaj.ydzc1.top

sort a.txt | uniq -c | sort -rn | head
来源：http://qiv.cheryme.top

[R52] 统计行数
来源：http://uga.tian-w.cn

wc -l a.txt
来源：http://ysr.pycfn.com

[R53] 查看文件头与实时尾
来源：http://dkg.yfazqb.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gvu.gotoacloud.top

[R54] 比较两个文件
来源：http://ocm.yonumen.top

diff a.txt b.txt
来源：http://ucm.yfazqb.com

[R55] 压缩与解压
来源：http://yuz.aibaodan.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rxa.tian-w.cn

[R56] 远程拷贝
来源：http://tlj.jianghu66.top

scp file user@host:/path/
来源：http://eol.bbcook.cn

[R57] 远程执行命令
来源：http://dkx.kuanghao11.cn

ssh user@host 'uptime'
来源：http://awq.ehwqpu.com

[R58] 下载文件
来源：http://jhj.bjfxy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lti.vqdsnc.cn

[R59] 发 POST JSON
来源：http://wmr.bbcook.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://iyd.nwbrower.top

[R60] 只看 HTTP 状态码
来源：http://bdn.zhiwuduotai.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wrw.sweek.top

[R61] 磁盘占用
来源：http://rjr.cheryme.top

df -h;  du -sh *
来源：http://hce.jianghu66.top

[R62] 找最占空间的文件
来源：http://bnu.jinqigfzy.top

du -ah . | sort -rh | head -10
来源：http://zbw.tian-w.cn

[R63] 内存与进程
来源：http://mhq.nanxuanxn.top

free -h;  ps aux | grep nginx
来源：http://rjh.nanxinkj.top

[R64] 结束进程
来源：http://hku.sweek.top

kill -9 $(pgrep -f app.py)
来源：http://tia.ivvv.top

[R65] 查看端口占用
来源：http://eqz.sxryk.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nxf.guowangkeji.top

[R66] 定时任务
来源：http://srd.cqqwz.cn

crontab -e;  crontab -l
来源：http://euk.haohaochexian.top

[R67] 生成随机十六进制串
来源：http://ybk.0kj1m.cn

openssl rand -hex 16
来源：http://rqo.yuxming.cn

[R68] 计算文件校验值
来源：http://bcf.vqdsnc.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vrg.xingfuxueyuan.xyz

[R69] 生成随机密码
来源：http://eed.yueranfly.top

head -c 16 /dev/urandom | base64
来源：http://tbs.wangshuangyany.cn

[R70] 时间戳与互转
来源：http://tsn.chenzaomai.com

date +%s;  date -d @1700000000
来源：http://yij.sysykeji.top

[R71] 日期格式化
来源：http://ugj.fktsv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cfe.hongshengwenyu.top

[R72] 等待端口就绪
来源：http://hro.fktsv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://twj.0kj1m.cn

[R73] 分割大日志
来源：http://das.aibaodan.cn

split -l 1000 big.log part_
来源：http://neu.feifeiyinyue.top

[R74] 批量重命名
来源：http://ynf.chenjidiqi.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cjq.yuxming.cn

[R75] 导出环境变量
来源：http://yoe.zdbjq.cn

export PATH="$HOME/bin:$PATH"
来源：http://zqc.yueranfly.top

[R76] 使用临时文件
来源：http://pqo.jinqigufen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ieb.yangfankeji.com

[R77] 读取用户输入
来源：http://gal.pycfn.com

read -rp "请输入: " ans
来源：http://spi.hongshengwenyu.top

[R78] 交互式菜单
来源：http://iku.gotoacloud.top

select opt in a b c; do echo "$opt"; break; done
来源：http://gta.chenzaomai.com

[R79] 解析命令行选项
来源：http://zwz.nanxuanxn.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://siz.jqgfzy.top

[R80] 查看脚本执行耗时
来源：http://jvl.fanxiaobao.xyz

time ./run.sh
来源：http://brx.zhengqikj.top

================================================================================
来源：http://clv.chenzaomai.com

S. C / C++ 专题
来源：http://jgc.aizwys.cn

================================================================================
来源：http://lkr.zhoulong.xyz

[S01] C：Hello World
来源：http://smo.havefunace.top

#include <stdio.h>
来源：http://vpx.tianlin.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://mxv.tarul.cn

[S02] C：变量与格式化输出
来源：http://rin.jianghu66.top

int a = 10; printf("%d\n", a);
来源：http://nyi.zhaomingkeji.xyz

[S03] C：读入整数
来源：http://uza.ywan-chungtsiang.top

int x; scanf("%d", &x);
来源：http://eve.yongpay.top

[S04] C：字符串复制
来源：http://tin.gotoacloud.top

char dst[32]; strcpy(dst, "hi");
来源：http://pro.tian-w.cn

[S05] C：字符串长度
来源：http://sze.ybcxt.top

strlen(s)
来源：http://ult.ppjwa.cn

[S06] C：字符串比较
来源：http://tfa.sufxvd.cn

strcmp(a, b) == 0
来源：http://xtp.shuidangran.top

[S07] C：数组遍历求和
来源：http://ked.yueranfly.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://snh.sxryk.cn

[S08] C：动态内存分配与释放
来源：http://ozv.tarul.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://swg.ybcxt.top

[S09] C：结构体定义与初始化
来源：http://sbc.wangshuangyany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tvp.hywenlv.cn

[S10] C：指针与解引用
来源：http://rsy.c1oappe.top

int *p = &a;  *p = 5;
来源：http://npy.fehbvm.com

[S11] C：逐行读文件
来源：http://pvg.yanxiufei.cn

FILE *f = fopen("a.txt", "r");
来源：http://xrp.zhaomingkeji.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://fcp.gotoacloud.top

fclose(f);
来源：http://ryj.hnqzz.top

[S12] C：写文件
来源：http://fjs.zhoulong.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://smq.epnwcf.com

[S13] C：宏定义
来源：http://zos.jiagoushi.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lbk.jianghu66.top

[S14] C：枚举
来源：http://cxc.yj20258.top

enum Color { RED, GREEN, BLUE };
来源：http://jeu.shzxlz.cn

[S15] C：类型转换
来源：http://ypp.tarul.cn

(double) a / b
来源：http://mzn.cheryme.top

[S16] C：位操作置位
来源：http://hhh.yvedp.cn

x |= (1 << 3);
来源：http://ghj.cqqwz.cn

[S17] C：安全拼接字符串
来源：http://ste.mhx1999.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tya.hywenlv.cn

[S18] C：命令行参数
来源：http://hbt.yongpay.top

int main(int argc, char **argv)
来源：http://rla.zhixingplan.top

[S19] C：快速排序
来源：http://ikv.cucudq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rgb.epnwcf.com

[S20] C：二分查找
来源：http://kzj.ppjwa.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kzq.hnxiangtu.top

[S21] C：字符类别判断
来源：http://qir.xylfe.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://oti.haohaochexian.top

[S22] C：字符串转数字
来源：http://vub.sxryk.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ygs.jinghuilouyu.cn

[S23] C：随机数
来源：http://dnn.dianchejie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gpe.ywan-chungtsiang.top

[S24] C：获取本地时间
来源：http://rds.ywan-chungtsiang.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uyh.ivvv.top

[S25] C：内存拷贝
来源：http://mba.chenjidiqi.icu

memcpy(dst, src, n);
来源：http://exd.fktsv.cn

[S26] C：内存清零
来源：http://kqz.ydjk.org.cn

memset(a, 0, sizeof a);
来源：http://ypg.zdbjq.cn

[S27] C：定义常量
来源：http://knz.52xcode.cn

const double PI = 3.14159;
来源：http://hbd.xuanzx.com

[S28] C：静态变量
来源：http://iww.yanxiufei.cn

static int counter = 0;
来源：http://epy.tian-w.cn

[S29] C：变参函数
来源：http://fap.vehdjk.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xjk.gaohongyu789.top

[S30] C：头文件保护
来源：http://ogc.haohaochexian.top

#ifndef X_H
来源：http://yss.svipenyu.cn

#define X_H
来源：http://war.gogol.net.cn

#endif
来源：http://fro.epnwcf.com

[S31] C++：Hello World
来源：http://tam.zycfv.cn

#include <iostream>
来源：http://pag.yueranfly.top

int main() { std::cout << "Hello\n"; }
来源：http://ilh.fengsongda.top

[S32] C++：字符串
来源：http://ziy.yfazqb.com

std::string s = "hi";  s += "!";
来源：http://ici.chenlongwang.top

[S33] C++：vector 增删
来源：http://woz.jianghu66.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://apl.wangshuangyany.cn

[S34] C++：遍历 vector
来源：http://zpt.hammf.cn

for (auto &x : v) { std::cout << x; }
来源：http://etv.ydjk.org.cn

[S35] C++：map
来源：http://xdr.dianchejie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tvp.aibaodan.cn

[S36] C++：unordered_map
来源：http://bcr.hysaishi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://flw.shanyushiyangkeji.top

[S37] C++：set
来源：http://dyc.zhiwuduotai.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ery.chenjidiqi.icu

[S38] C++：排序
来源：http://ilr.9152youxi.cn

std::sort(v.begin(), v.end());
来源：http://fdp.tianlin.xyz

[S39] C++：自定义比较器排序
来源：http://ziz.jinqigufen.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qfo.zdqjudy.top

[S40] C++：查找元素
来源：http://tap.gogol.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hlq.gotoacloud.top

[S41] C++：类与构造函数
来源：http://iji.hnqzz.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bsj.sjlbkw.cn

[S42] C++：继承与虚函数
来源：http://bng.ydjk.org.cn

class B : public Base { public: void f() override {} };
来源：http://gwx.svipenyu.cn

[S43] C++：智能指针
来源：http://lpi.jlsjyb.cn

auto p = std::make_unique<int>(5);
来源：http://eup.kuanghao11.cn

[S44] C++：引用传参
来源：http://ste.yanxiufei.cn

void inc(int &x) { ++x; }
来源：http://spp.haohaochexian.top

[S45] C++：lambda
来源：http://wrc.sysykeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://mwt.52xcode.cn

[S46] C++：函数模板
来源：http://ybi.gaohongyu789.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pyt.hnxiangtu.top

[S47] C++：结构化绑定遍历
来源：http://wet.wangdashe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lal.nwbrower.top

[S48] C++：逐行读文件
来源：http://ghh.yuanzhike.top

std::ifstream in("a.txt");  std::string line;
来源：http://zhj.havefunace.top

while (std::getline(in, line)) { }
来源：http://ajx.bjfxy.top

[S49] C++：写文件
来源：http://doe.guannengcc.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cxz.sxryk.cn

[S50] C++：格式化数字
来源：http://ojg.sxryk.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rko.zhijiandao.cn

[S51] C++：显式类型转换
来源：http://yag.iojbl.cn

static_cast<double>(a) / b
来源：http://dcw.xinyue.icu

[S52] C++：const 与 noexcept
来源：http://gen.cheryme.top

int size() const noexcept { return n_; }
来源：http://one.shanyushiyangtech.top

[S53] C++：移动语义
来源：http://qrm.dashuyun.cn

std::vector<int> w = std::move(v);
来源：http://dum.0kj1m.cn

[S54] C++：异常处理
来源：http://wjn.meibo888.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://str.ctjpmb.com

[S55] C++：结构化绑定
来源：http://fjj.guowangkeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://frc.hongshengwenyu.top

[S56] C++：optional
来源：http://cya.cdnleiting.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ncq.jiagoushi.top

[S57] C++：编译期常量
来源：http://qwq.hfpthk.cn

constexpr int N = 10;
来源：http://fqx.tian-w.cn

[S58] C++：命名空间
来源：http://gtt.yongpay.top

namespace ns { int f() { return 1; } }
来源：http://oym.gzhubu.top

[S59] C++：静态断言
来源：http://pku.cucudq.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xjz.hesvh.cn

[S60] C++：遍历并删除元素
来源：http://izh.hesvh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kpy.andypj.xyz

================================================================================
来源：http://bfv.9152youxi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ars.daria6918.cn

================================================================================
来源：http://tkr.daxiang520.top


<!-- 参考信息 -->