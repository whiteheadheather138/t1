代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://slq.xuanzx.com

[Q90] 生成序号列
来源：http://elg.meibo888.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vqs.tarul.cn

================================================================================
来源：http://tey.pengpengdd.cyou

R. Bash 专题
来源：http://lyb.yj202588.top

================================================================================
来源：http://unz.fanxiaobao.xyz

[R01] shebang 与严格模式
来源：http://apf.zdbjq.cn

#!/usr/bin/env bash
来源：http://jmb.feifeiyinyue.top

set -euo pipefail
来源：http://guu.wangshuangyany.cn

[R02] 变量赋值与使用
来源：http://ajh.tanke756.top

name="Tom"; echo "$name"
来源：http://xvp.sufxvd.cn

[R03] 只读变量
来源：http://iuz.pycfn.com

readonly PI=3.14
来源：http://azq.chenjidiqi.icu

[R04] 位置参数
来源：http://poz.zdqjudy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vbb.jqgufenzy.top

[R05] 参数默认值
来源：http://pge.wangshuangyany.cn

name="${1:-default}"
来源：http://kmj.xuanzx.com

[R06] 判断命令是否存在
来源：http://ggw.xingfuxueyuan.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bvb.hnxiangtu.top

[R07] if 判断文件
来源：http://aus.cdnleiting.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jjp.yuxming.cn

[R08] 数值比较
来源：http://bjd.hfpthk.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lvg.ydjk.org.cn

[R09] 字符串比较
来源：http://btb.zdbjq.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://aoy.bjfxy.top

[R10] 正则匹配
来源：http://qbj.svipenyu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sie.316326.xyz

[R11] case 多分支
来源：http://bpo.redwolf501.top

case "$1" in
来源：http://dmp.bbcook.cn

start) echo "启动" ;;
来源：http://ede.feifeiyinyue.top

stop)  echo "停止" ;;
来源：http://mbd.svipenyu.cn

*)     echo "未知命令" ;;
来源：http://bjv.svipenyu.cn

esac
来源：http://vxa.tianlin.xyz

[R12] for 遍历文件
来源：http://pxw.wangshuangyany.cn

for f in *.txt; do echo "$f"; done
来源：http://qes.cqqwz.cn

[R13] for 计数循环
来源：http://rmr.shanyushiyangtech.top

for i in {1..10}; do echo "$i"; done
来源：http://fwk.shanyushiyangtech.top

[R14] C 风格 for
来源：http://acz.tianlin.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zbo.yuanzhike.top

[R15] while 逐行读文件
来源：http://gba.smart0.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sfv.hnxiangtu.top

[R16] until 等待条件
来源：http://tjp.shangyingyoupin.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zdr.zhijiandao.cn

[R17] 数组定义与取值
来源：http://rid.xinyue.icu

arr=(a b c); echo "${arr[0]}"
来源：http://agw.yuanzhike.top

[R18] 遍历数组
来源：http://hyq.fktsv.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ogw.yonumen.top

[R19] 数组长度
来源：http://ytz.havefunace.top

echo "${#arr[@]}"
来源：http://yap.daria6918.cn

[R20] 关联数组（字典）
来源：http://zrw.nwbrower.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cwp.iojbl.cn

[R21] 字符串长度
来源：http://npd.cdnleiting.top

echo "${#s}"
来源：http://xkj.meibo888.top

[R22] 截取子串
来源：http://jpz.cashguo.top

echo "${s:0:5}"
来源：http://lte.yueranfly.top

[R23] 字符串替换
来源：http://epz.zhongyouzk.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wga.nwbrower.top

[R24] 大小写转换
来源：http://the.chenlongwang.top

echo "${s^^}"; echo "${s,,}"
来源：http://zpo.ehwqpu.com

[R25] 去后缀 / 去前缀
来源：http://eas.jqgfzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://uef.ydjk.org.cn

[R26] 命令替换
来源：http://wtu.tanke756.top

now=$(date +%F); echo "$now"
来源：http://hkz.epnwcf.com

[R27] 算术展开
来源：http://gws.gzhubu.top

echo $((1 + 2 * 3))
来源：http://vok.zhengqikj.top

[R28] 浮点运算
来源：http://dzk.fktsv.cn

echo "scale=2; 10/3" | bc
来源：http://lsi.nwbrower.top

[R29] 定义函数
来源：http://ckh.pengpengdd.cyou

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uwg.ybcxt.top

[R30] 函数返回状态码
来源：http://ieb.hnqzz.top

f() { return 0; }; f || echo "失败了"
来源：http://hnm.uphjek.com

[R31] 局部变量
来源：http://xfg.bjfxy.top

f() { local x=1; echo "$x"; }
来源：http://kld.ydjk.org.cn

[R32] 参数个数校验
来源：http://edc.ppjwa.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ijy.9152youxi.cn

[R33] 捕获错误并提示行号
来源：http://ayb.uphjek.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://iab.zhoulong.xyz

[R34] 退出时清理
来源：http://uge.uphjek.com

trap 'rm -f "$tmp"' EXIT
来源：http://myc.jianghu66.top

[R35] 后台执行并等待
来源：http://eqm.jiagoushi.top

sleep 5 & pid=$!; wait "$pid"
来源：http://gqx.zhoulong.xyz

[R36] 并发执行多个任务
来源：http://kjt.zdbjq.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ixc.kuanghao11.cn

[R37] 把输出赋给变量
来源：http://plt.hnxiangtu.top

files=$(ls -1)
来源：http://qsw.jiagoushi.top

[R38] 管道串联
来源：http://vdk.316326.xyz

cat a.txt | grep -i error | wc -l
来源：http://krn.kuanghao11.cn

[R39] 重定向标准输出与错误
来源：http://ddi.guannengcc.top

cmd > out.log 2>&1
来源：http://ppa.52xcode.cn

[R40] 追加写日志
来源：http://stx.chenzaomai.com

echo "log" >> out.log
来源：http://jac.jyoumei.cn

[R41] 丢弃输出
来源：http://izk.nwbrower.top

cmd >/dev/null 2>&1
来源：http://tew.aibaodan.cn

[R42] 输入重定向
来源：http://zxk.cheryme.top

wc -l < a.txt
来源：http://ejg.yueranfly.top

[R43] 按名字查找文件
来源：http://lix.yongpay.top

find . -name "*.log" -type f
来源：http://bdc.feifeiyinyue.top

[R44] 按修改时间查找
来源：http://nzb.zhoulong.xyz

find . -mtime -7 -type f
来源：http://yvi.nanxinkj.top

[R45] 批量删除
来源：http://uef.epnwcf.com

find . -name "*.tmp" -delete
来源：http://pko.gaohongyu789.top

[R46] 递归替换文件内容
来源：http://bek.yfazqb.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ims.svipenyu.cn

[R47] sed 单行替换
来源：http://qtd.ctjpmb.com

sed -i 's/foo/bar/g' a.txt
来源：http://vex.zhiwuduotai.top

[R48] awk 取指定列
来源：http://qtq.vqdsnc.cn

awk '{print $1, $3}' a.txt
来源：http://ytr.shanyushiyangtech.top

[R49] awk 带条件
来源：http://hmw.vehdjk.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yrm.xinyue.icu

[R50] awk 求和
来源：http://dbo.zycfv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wzj.ywan-chungtsiang.top

[R51] 排序去重取前几
来源：http://uea.chenzaomai.com

sort a.txt | uniq -c | sort -rn | head
来源：http://rrh.cqqwz.cn

[R52] 统计行数
来源：http://sqz.pycfn.com

wc -l a.txt
来源：http://bnw.smart0.xyz

[R53] 查看文件头与实时尾
来源：http://ghz.yanxiufei.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jdj.sweek.top

[R54] 比较两个文件
来源：http://neo.chenzaomai.com

diff a.txt b.txt
来源：http://yxb.vqdsnc.cn

[R55] 压缩与解压
来源：http://din.pycfn.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://isd.yj20258888.top

[R56] 远程拷贝
来源：http://yfj.zhongyouzk.top

scp file user@host:/path/
来源：http://kny.sjlbkw.cn

[R57] 远程执行命令
来源：http://eyn.hnqzz.top

ssh user@host 'uptime'
来源：http://xra.gogol.net.cn

[R58] 下载文件
来源：http://tgv.yuxming.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tse.xinyue.icu

[R59] 发 POST JSON
来源：http://koe.aizwys.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kvc.xuanzx.com

[R60] 只看 HTTP 状态码
来源：http://snx.fengsongda.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ebx.ywan-chungtsiang.top

[R61] 磁盘占用
来源：http://app.hammf.cn

df -h;  du -sh *
来源：http://tvx.hywenlv.cn

[R62] 找最占空间的文件
来源：http://rsz.fengsongda.top

du -ah . | sort -rh | head -10
来源：http://qxm.hongshengwenyu.top

[R63] 内存与进程
来源：http://eog.yvedp.cn

free -h;  ps aux | grep nginx
来源：http://fws.sweek.top

[R64] 结束进程
来源：http://kyu.yanxiufei.cn

kill -9 $(pgrep -f app.py)
来源：http://ink.yonumen.top

[R65] 查看端口占用
来源：http://dcl.shanyushiyangtech.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://biz.xziqi.cn

[R66] 定时任务
来源：http://baj.zhengqikj.top

crontab -e;  crontab -l
来源：http://fjx.hcnkem.com

[R67] 生成随机十六进制串
来源：http://loy.ivvv.top

openssl rand -hex 16
来源：http://jdr.bbcook.cn

[R68] 计算文件校验值
来源：http://ozi.zdqjudy.top

sha256sum a.txt;  md5sum a.txt
来源：http://gin.sxryk.cn

[R69] 生成随机密码
来源：http://cec.xziqi.cn

head -c 16 /dev/urandom | base64
来源：http://qwc.vqdsnc.cn

[R70] 时间戳与互转
来源：http://ybl.haohaochexian.top

date +%s;  date -d @1700000000
来源：http://mez.yueranfly.top

[R71] 日期格式化
来源：http://hnf.yuanzhike.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bem.wangshuangyany.cn

[R72] 等待端口就绪
来源：http://emb.tianlin.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://sww.cqqwz.cn

[R73] 分割大日志
来源：http://ozg.yonumen.top

split -l 1000 big.log part_
来源：http://fes.havefunace.top

[R74] 批量重命名
来源：http://wif.hcnkem.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://htc.ywan-chungtsiang.top

[R75] 导出环境变量
来源：http://jra.ybcxt.top

export PATH="$HOME/bin:$PATH"
来源：http://pox.iojbl.cn

[R76] 使用临时文件
来源：http://ncr.shangyingyoupin.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qsx.hnqzz.top

[R77] 读取用户输入
来源：http://pti.hnqzz.top

read -rp "请输入: " ans
来源：http://lkt.guowangkeji.top

[R78] 交互式菜单
来源：http://lbb.xinyue.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://ngd.guowangkeji.top

[R79] 解析命令行选项
来源：http://zza.ppjwa.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fku.ctjpmb.com

[R80] 查看脚本执行耗时
来源：http://eoc.zhaomingkeji.xyz

time ./run.sh
来源：http://wco.epnwcf.com

================================================================================
来源：http://krf.jqgfzy.top

S. C / C++ 专题
来源：http://jxz.xingfuxueyuan.xyz

================================================================================
来源：http://vad.yongpay.top

[S01] C：Hello World
来源：http://fku.quarkkingdee.top

#include <stdio.h>
来源：http://bms.yfazqb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://mzo.meibo888.top

[S02] C：变量与格式化输出
来源：http://fit.iojbl.cn

int a = 10; printf("%d\n", a);
来源：http://ffy.jiagoushi.top

[S03] C：读入整数
来源：http://fil.nwbrower.top

int x; scanf("%d", &x);
来源：http://lpo.xziqi.cn

[S04] C：字符串复制
来源：http://cwp.aibaodan.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cgv.andypj.xyz

[S05] C：字符串长度
来源：http://bxv.bbcook.cn

strlen(s)
来源：http://ssp.vehdjk.com

[S06] C：字符串比较
来源：http://upi.yuanzhike.top

strcmp(a, b) == 0
来源：http://ora.xingfuxueyuan.xyz

[S07] C：数组遍历求和
来源：http://sfz.52xcode.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://atx.havefunace.top

[S08] C：动态内存分配与释放
来源：http://wuo.havefunace.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hsg.hfpthk.cn

[S09] C：结构体定义与初始化
来源：http://xiu.mhx1999.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fdn.chenjidiqi.icu

[S10] C：指针与解引用
来源：http://sgc.yueranfly.top

int *p = &a;  *p = 5;
来源：http://afd.fanxiaobao.xyz

[S11] C：逐行读文件
来源：http://nti.aibaodan.cn

FILE *f = fopen("a.txt", "r");
来源：http://qra.birdmap.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ksz.epnwcf.com

fclose(f);
来源：http://zzh.jqgufenzy.top

[S12] C：写文件
来源：http://umf.52xcode.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fcl.zhijiandao.cn

[S13] C：宏定义
来源：http://azj.uphjek.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vwz.yuanzhike.top

[S14] C：枚举
来源：http://aqv.havefunace.top

enum Color { RED, GREEN, BLUE };
来源：http://tii.zhiwuduotai.top

[S15] C：类型转换
来源：http://mpf.yueranfly.top

(double) a / b
来源：http://tom.316326.xyz

[S16] C：位操作置位
来源：http://kjh.aizwys.cn

x |= (1 << 3);
来源：http://ehh.guannengcc.top

[S17] C：安全拼接字符串
来源：http://bpp.cheryme.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://axy.xuanzx.com

[S18] C：命令行参数
来源：http://our.yonumen.top

int main(int argc, char **argv)
来源：http://tka.epnwcf.com

[S19] C：快速排序
来源：http://lee.xuanzx.com

qsort(a, n, sizeof(int), cmp);
来源：http://pqj.kuanghao11.cn

[S20] C：二分查找
来源：http://aqs.dashuyun.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kfg.cqqwz.cn

[S21] C：字符类别判断
来源：http://gyb.52xcode.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://eeo.bbcook.cn

[S22] C：字符串转数字
来源：http://ewn.iojbl.cn

atoi("42");  strtod("3.14", NULL);
来源：http://myr.jlsjyb.cn

[S23] C：随机数
来源：http://mvh.fanxiaobao.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://vsg.316326.xyz

[S24] C：获取本地时间
来源：http://nlt.yuanzhike.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bqo.sysykeji.top

[S25] C：内存拷贝
来源：http://xme.epnwcf.com

memcpy(dst, src, n);
来源：http://cnw.sxryk.cn

[S26] C：内存清零
来源：http://htn.hammf.cn

memset(a, 0, sizeof a);
来源：http://npx.xziqi.cn

[S27] C：定义常量
来源：http://kth.nanxinkj.top

const double PI = 3.14159;
来源：http://aaj.dashuyun.cn

[S28] C：静态变量
来源：http://gmt.hysaishi.cn

static int counter = 0;
来源：http://xwj.yvedp.cn

[S29] C：变参函数
来源：http://mza.nwbrower.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cjb.yonumen.top

[S30] C：头文件保护
来源：http://dlj.tianlin.xyz

#ifndef X_H
来源：http://hby.ehwqpu.com

#define X_H
来源：http://cfc.shanyushiyangkeji.top

#endif
来源：http://nqq.daria6918.cn

[S31] C++：Hello World
来源：http://nnw.yvedp.cn

#include <iostream>
来源：http://wwl.sysykeji.top

int main() { std::cout << "Hello\n"; }
来源：http://jip.shzxlz.cn

[S32] C++：字符串
来源：http://dsq.hnqzz.top

std::string s = "hi";  s += "!";
来源：http://uoj.jlsjyb.cn

[S33] C++：vector 增删
来源：http://emw.feifeiyinyue.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ioz.ydzc1.top

[S34] C++：遍历 vector
来源：http://oyg.gzhubu.top

for (auto &x : v) { std::cout << x; }
来源：http://oiq.ybcxt.top

[S35] C++：map
来源：http://krl.jinqigfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nco.tarul.cn

[S36] C++：unordered_map
来源：http://gjs.dashuyun.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vcp.wangdashe.top

[S37] C++：set
来源：http://rnt.jiagoushi.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://alx.chenjidiqi.icu

[S38] C++：排序
来源：http://pjw.nanxinkj.top

std::sort(v.begin(), v.end());
来源：http://lgo.redwolf501.top

[S39] C++：自定义比较器排序
来源：http://vuu.hongshengwenyu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vuv.xziqi.cn

[S40] C++：查找元素
来源：http://gtz.haohaochexian.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wjh.wangdashe.top

[S41] C++：类与构造函数
来源：http://tlx.xuanzx.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dcj.gaohongyu789.top

[S42] C++：继承与虚函数
来源：http://cxe.iojbl.cn

class B : public Base { public: void f() override {} };
来源：http://qut.haohaochexian.top

[S43] C++：智能指针
来源：http://qax.jinqigufen.top

auto p = std::make_unique<int>(5);
来源：http://bri.gaohongyu789.top

[S44] C++：引用传参
来源：http://dvr.uphjek.com

void inc(int &x) { ++x; }
来源：http://nry.zhixingplan.top

[S45] C++：lambda
来源：http://raz.ybcxt.top

auto add = [](int a, int b) { return a + b; };
来源：http://hon.yangfankeji.com

[S46] C++：函数模板
来源：http://vhk.yueranfly.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pdg.yj202588.top

[S47] C++：结构化绑定遍历
来源：http://som.cucudq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jxu.vqdsnc.cn

[S48] C++：逐行读文件
来源：http://zvb.bbcook.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xqy.ydjk.org.cn

while (std::getline(in, line)) { }
来源：http://vnw.ywan-chungtsiang.top

[S49] C++：写文件
来源：http://npk.zhengqikj.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hdk.ehwqpu.com

[S50] C++：格式化数字
来源：http://lzg.ctjpmb.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ljz.jqgufenzy.top

[S51] C++：显式类型转换
来源：http://hmz.ppjwa.cn

static_cast<double>(a) / b
来源：http://adr.zhengqikj.top

[S52] C++：const 与 noexcept
来源：http://kaq.fzhhl.top

int size() const noexcept { return n_; }
来源：http://mam.ivvv.top

[S53] C++：移动语义
来源：http://zuz.uphjek.com

std::vector<int> w = std::move(v);
来源：http://men.mhx1999.top

[S54] C++：异常处理
来源：http://kvf.hesvh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sce.hammf.cn

[S55] C++：结构化绑定
来源：http://plg.zycfv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tot.yangfankeji.com

[S56] C++：optional
来源：http://ffw.jqgfzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gir.jinyuanbaomall.cn

[S57] C++：编译期常量
来源：http://lph.ivvv.top

constexpr int N = 10;
来源：http://jmx.mhx1999.top

[S58] C++：命名空间
来源：http://rbd.yfazqb.com

namespace ns { int f() { return 1; } }
来源：http://cvp.ehwqpu.com

[S59] C++：静态断言
来源：http://mob.epnwcf.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nmk.ctjpmb.com

[S60] C++：遍历并删除元素
来源：http://vvu.redwolf501.top


<!-- 参考信息 -->