代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://eox.chenjidiqi.icu

[Q90] 生成序号列
来源：http://xey.zdbjq.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dyb.bjfxy.top

================================================================================
来源：http://maj.fktsv.cn

R. Bash 专题
来源：http://yav.jinyuanbaomall.cn

================================================================================
来源：http://dqn.zhijiandao.cn

[R01] shebang 与严格模式
来源：http://bul.bjfxy.top

#!/usr/bin/env bash
来源：http://lsi.zhixingplan.top

set -euo pipefail
来源：http://mcy.tarul.cn

[R02] 变量赋值与使用
来源：http://bom.aizwys.cn

name="Tom"; echo "$name"
来源：http://lss.jyoumei.cn

[R03] 只读变量
来源：http://xxe.shuidangran.top

readonly PI=3.14
来源：http://yjn.tanke756.top

[R04] 位置参数
来源：http://fhf.ctjpmb.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tzo.shanyushiyangkeji.top

[R05] 参数默认值
来源：http://vjo.sweek.top

name="${1:-default}"
来源：http://rrx.daxiang520.top

[R06] 判断命令是否存在
来源：http://gyb.cqqwz.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fpq.jinqigfzy.top

[R07] if 判断文件
来源：http://ysn.shanyushiyangtech.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rqx.hongshengwenyu.top

[R08] 数值比较
来源：http://vnc.ydjk.org.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://npk.hongshengwenyu.top

[R09] 字符串比较
来源：http://alz.yfazqb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ioe.hnqzz.top

[R10] 正则匹配
来源：http://iiv.jyoumei.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bbi.c1oappe.top

[R11] case 多分支
来源：http://iuj.nwbrower.top

case "$1" in
来源：http://jxf.hysaishi.cn

start) echo "启动" ;;
来源：http://ynn.shanyushiyangkeji.top

stop)  echo "停止" ;;
来源：http://jfg.guowangkeji.top

*)     echo "未知命令" ;;
来源：http://xey.zhaomingkeji.xyz

esac
来源：http://ulh.fehbvm.com

[R12] for 遍历文件
来源：http://yey.tian-w.cn

for f in *.txt; do echo "$f"; done
来源：http://fxo.hysaishi.cn

[R13] for 计数循环
来源：http://gew.meibo888.top

for i in {1..10}; do echo "$i"; done
来源：http://jtu.cdnleiting.top

[R14] C 风格 for
来源：http://hty.ppjwa.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jqt.yuanzhike.top

[R15] while 逐行读文件
来源：http://vte.fehbvm.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qta.andypj.xyz

[R16] until 等待条件
来源：http://dmi.shuidangran.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://voq.quarkkingdee.top

[R17] 数组定义与取值
来源：http://usp.hywenlv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vdh.jianghu66.top

[R18] 遍历数组
来源：http://bfw.fengsongda.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vpy.hammf.cn

[R19] 数组长度
来源：http://tua.shanyushiyangtech.top

echo "${#arr[@]}"
来源：http://qhw.sxryk.cn

[R20] 关联数组（字典）
来源：http://wug.jinghuilouyu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://eat.fktsv.cn

[R21] 字符串长度
来源：http://uro.fehbvm.com

echo "${#s}"
来源：http://tdg.xylfe.cn

[R22] 截取子串
来源：http://bem.jinghuilouyu.cn

echo "${s:0:5}"
来源：http://son.meibo888.top

[R23] 字符串替换
来源：http://fgg.fzhhl.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ioo.zhaomingkeji.xyz

[R24] 大小写转换
来源：http://uei.xingfuxueyuan.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://heh.yuxming.cn

[R25] 去后缀 / 去前缀
来源：http://bke.cdnleiting.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://eak.dianchejie.cn

[R26] 命令替换
来源：http://mge.yangfankeji.com

now=$(date +%F); echo "$now"
来源：http://jlx.ppjwa.cn

[R27] 算术展开
来源：http://xuz.hfpthk.cn

echo $((1 + 2 * 3))
来源：http://lea.0kj1m.cn

[R28] 浮点运算
来源：http://krq.ppjwa.cn

echo "scale=2; 10/3" | bc
来源：http://hcl.nwbrower.top

[R29] 定义函数
来源：http://xjx.hnxiangtu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jtv.tarul.cn

[R30] 函数返回状态码
来源：http://kwm.meibo888.top

f() { return 0; }; f || echo "失败了"
来源：http://xfm.jyoumei.cn

[R31] 局部变量
来源：http://mou.quarkkingdee.top

f() { local x=1; echo "$x"; }
来源：http://uek.sjlbkw.cn

[R32] 参数个数校验
来源：http://hhd.pycfn.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ljz.jlsjyb.cn

[R33] 捕获错误并提示行号
来源：http://lrh.jianghu66.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wgk.hongshengwenyu.top

[R34] 退出时清理
来源：http://wwf.yfazqb.com

trap 'rm -f "$tmp"' EXIT
来源：http://rua.hywenlv.cn

[R35] 后台执行并等待
来源：http://gmj.jinghuilouyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qfg.nwbrower.top

[R36] 并发执行多个任务
来源：http://tnz.sjlbkw.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://imi.yj20258888.top

[R37] 把输出赋给变量
来源：http://frm.hongshengwenyu.top

files=$(ls -1)
来源：http://vtr.vehdjk.com

[R38] 管道串联
来源：http://bei.52xcode.cn

cat a.txt | grep -i error | wc -l
来源：http://svh.shzxlz.cn

[R39] 重定向标准输出与错误
来源：http://pqg.dianchejie.cn

cmd > out.log 2>&1
来源：http://vrw.yj20258.top

[R40] 追加写日志
来源：http://jmv.shanyushiyangtech.top

echo "log" >> out.log
来源：http://ben.haohaochexian.top

[R41] 丢弃输出
来源：http://zpt.yueranfly.top

cmd >/dev/null 2>&1
来源：http://int.fengsongda.top

[R42] 输入重定向
来源：http://pne.xuetiantiany.cn

wc -l < a.txt
来源：http://mxy.jinyuanbaomall.cn

[R43] 按名字查找文件
来源：http://rxg.jinqigufen.top

find . -name "*.log" -type f
来源：http://ecc.daria6918.cn

[R44] 按修改时间查找
来源：http://qvr.xuetiantiany.cn

find . -mtime -7 -type f
来源：http://kka.jinghuilouyu.cn

[R45] 批量删除
来源：http://ukx.fktsv.cn

find . -name "*.tmp" -delete
来源：http://bql.ctjpmb.com

[R46] 递归替换文件内容
来源：http://hrw.aizwys.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://omu.pengpengdd.cyou

[R47] sed 单行替换
来源：http://pam.yongpay.top

sed -i 's/foo/bar/g' a.txt
来源：http://ukj.sjlbkw.cn

[R48] awk 取指定列
来源：http://jbg.shzxlz.cn

awk '{print $1, $3}' a.txt
来源：http://lic.gaohongyu789.top

[R49] awk 带条件
来源：http://por.nanxinkj.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cto.cdnleiting.top

[R50] awk 求和
来源：http://ieq.zhixingplan.top

awk '{s += $2} END {print s}' a.txt
来源：http://vhy.yj20258.top

[R51] 排序去重取前几
来源：http://bky.aibaodan.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://smh.9152youxi.cn

[R52] 统计行数
来源：http://waw.tanke756.top

wc -l a.txt
来源：http://jvw.xinyue.icu

[R53] 查看文件头与实时尾
来源：http://drz.daxiang520.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iji.jiagoushi.top

[R54] 比较两个文件
来源：http://dws.shzxlz.cn

diff a.txt b.txt
来源：http://eqq.fanxiaobao.xyz

[R55] 压缩与解压
来源：http://zad.gogol.net.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vqv.aizwys.cn

[R56] 远程拷贝
来源：http://aoq.jyoumei.cn

scp file user@host:/path/
来源：http://cih.zycfv.cn

[R57] 远程执行命令
来源：http://zgp.shangyingyoupin.top

ssh user@host 'uptime'
来源：http://wln.zdbjq.cn

[R58] 下载文件
来源：http://gdp.9152youxi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nyx.sufxvd.cn

[R59] 发 POST JSON
来源：http://rlr.shzxlz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xwc.ivvv.top

[R60] 只看 HTTP 状态码
来源：http://rzq.tarul.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://evv.c1oappe.top

[R61] 磁盘占用
来源：http://lrt.feifeiyinyue.top

df -h;  du -sh *
来源：http://kpq.ydjk.org.cn

[R62] 找最占空间的文件
来源：http://dhe.yj20258888.top

du -ah . | sort -rh | head -10
来源：http://mkz.yj20258888.top

[R63] 内存与进程
来源：http://jba.ydzc1.top

free -h;  ps aux | grep nginx
来源：http://vkk.ywan-chungtsiang.top

[R64] 结束进程
来源：http://own.zhijiandao.cn

kill -9 $(pgrep -f app.py)
来源：http://tip.shanyushiyangtech.top

[R65] 查看端口占用
来源：http://dwz.gzhubu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xqp.mhx1999.top

[R66] 定时任务
来源：http://xaf.aizwys.cn

crontab -e;  crontab -l
来源：http://zgz.jyoumei.cn

[R67] 生成随机十六进制串
来源：http://tlj.zhoulong.xyz

openssl rand -hex 16
来源：http://ywg.gaohongyu789.top

[R68] 计算文件校验值
来源：http://nvf.daxiang520.top

sha256sum a.txt;  md5sum a.txt
来源：http://xbn.quarkkingdee.top

[R69] 生成随机密码
来源：http://zjw.ppjwa.cn

head -c 16 /dev/urandom | base64
来源：http://ffy.zhiwuduotai.top

[R70] 时间戳与互转
来源：http://hwo.hnqzz.top

date +%s;  date -d @1700000000
来源：http://bhe.jinqigfzy.top

[R71] 日期格式化
来源：http://etr.fzhhl.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://kub.birdmap.top

[R72] 等待端口就绪
来源：http://bjx.shzxlz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jzd.9152youxi.cn

[R73] 分割大日志
来源：http://hqs.hnqzz.top

split -l 1000 big.log part_
来源：http://dkd.ywan-chungtsiang.top

[R74] 批量重命名
来源：http://yqe.wangshuangyany.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oag.jqgufenzy.top

[R75] 导出环境变量
来源：http://fnz.sxryk.cn

export PATH="$HOME/bin:$PATH"
来源：http://dbq.yanxiufei.cn

[R76] 使用临时文件
来源：http://zed.zdqjudy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qfz.cashguo.top

[R77] 读取用户输入
来源：http://geh.yonumen.top

read -rp "请输入: " ans
来源：http://cyd.c1oappe.top

[R78] 交互式菜单
来源：http://npk.sysykeji.top

select opt in a b c; do echo "$opt"; break; done
来源：http://aov.bbcook.cn

[R79] 解析命令行选项
来源：http://zrp.zdbjq.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ajs.chenzaomai.com

[R80] 查看脚本执行耗时
来源：http://fis.yj20258.top

time ./run.sh
来源：http://wtg.chenjidiqi.icu

================================================================================
来源：http://yxk.yanxiufei.cn

S. C / C++ 专题
来源：http://xxt.ppjwa.cn

================================================================================
来源：http://dil.hnxiangtu.top

[S01] C：Hello World
来源：http://vyh.nanxuanxn.top

#include <stdio.h>
来源：http://uex.jianghu66.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://yhx.c1oappe.top

[S02] C：变量与格式化输出
来源：http://plh.yueranfly.top

int a = 10; printf("%d\n", a);
来源：http://agb.yvedp.cn

[S03] C：读入整数
来源：http://fxc.hongshengwenyu.top

int x; scanf("%d", &x);
来源：http://tru.uphjek.com

[S04] C：字符串复制
来源：http://kcx.smart0.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://upn.jinyuanbaomall.cn

[S05] C：字符串长度
来源：http://fjq.chenjidiqi.icu

strlen(s)
来源：http://gfl.nanxinkj.top

[S06] C：字符串比较
来源：http://xfo.fengsongda.top

strcmp(a, b) == 0
来源：http://ygn.dianchejie.cn

[S07] C：数组遍历求和
来源：http://ryq.vehdjk.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qpw.ydzc1.top

[S08] C：动态内存分配与释放
来源：http://vhm.jqgufenzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qcv.tianlin.xyz

[S09] C：结构体定义与初始化
来源：http://bci.xingfuxueyuan.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gzl.ctjpmb.com

[S10] C：指针与解引用
来源：http://sid.yj202588.top

int *p = &a;  *p = 5;
来源：http://pwi.yangfankeji.com

[S11] C：逐行读文件
来源：http://hru.zhongyouzk.top

FILE *f = fopen("a.txt", "r");
来源：http://xsn.fehbvm.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://myj.zhixingplan.top

fclose(f);
来源：http://mpr.316326.xyz

[S12] C：写文件
来源：http://qjv.yj202588.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fez.pengpengdd.cyou

[S13] C：宏定义
来源：http://kda.zycfv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://meo.havefunace.top

[S14] C：枚举
来源：http://wvv.shanyushiyangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://ptn.ppjwa.cn

[S15] C：类型转换
来源：http://smt.redwolf501.top

(double) a / b
来源：http://cgn.xziqi.cn

[S16] C：位操作置位
来源：http://cvm.smart0.xyz

x |= (1 << 3);
来源：http://ktg.cqqwz.cn

[S17] C：安全拼接字符串
来源：http://hwa.xziqi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kro.sufxvd.cn

[S18] C：命令行参数
来源：http://xjf.nwbrower.top

int main(int argc, char **argv)
来源：http://yro.zhoulong.xyz

[S19] C：快速排序
来源：http://tjf.hcnkem.com

qsort(a, n, sizeof(int), cmp);
来源：http://chs.fzhhl.top

[S20] C：二分查找
来源：http://ioj.dashuyun.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qwz.yuxming.cn

[S21] C：字符类别判断
来源：http://hev.vqdsnc.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ffn.c1oappe.top

[S22] C：字符串转数字
来源：http://dpp.gaohongyu789.top

atoi("42");  strtod("3.14", NULL);
来源：http://umw.fktsv.cn

[S23] C：随机数
来源：http://mgr.zhijiandao.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://uha.cheryme.top

[S24] C：获取本地时间
来源：http://jyt.jiagoushi.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oti.nanxinkj.top

[S25] C：内存拷贝
来源：http://wrl.gaohongyu789.top

memcpy(dst, src, n);
来源：http://dvh.cashguo.top

[S26] C：内存清零
来源：http://ljm.ppjwa.cn

memset(a, 0, sizeof a);
来源：http://qjj.gotoacloud.top

[S27] C：定义常量
来源：http://unj.wangdashe.top

const double PI = 3.14159;
来源：http://hlc.jqgufenzy.top

[S28] C：静态变量
来源：http://vvb.zhoulong.xyz

static int counter = 0;
来源：http://bqg.hywenlv.cn

[S29] C：变参函数
来源：http://urp.chenlongwang.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jvw.nanxinkj.top

[S30] C：头文件保护
来源：http://qsb.jqgfzy.top

#ifndef X_H
来源：http://xey.nanxinkj.top

#define X_H
来源：http://ein.epnwcf.com

#endif
来源：http://swn.tian-w.cn

[S31] C++：Hello World
来源：http://gic.cqqwz.cn

#include <iostream>
来源：http://ion.daxiang520.top

int main() { std::cout << "Hello\n"; }
来源：http://sih.iojbl.cn

[S32] C++：字符串
来源：http://dqb.vehdjk.com

std::string s = "hi";  s += "!";
来源：http://ofa.ywan-chungtsiang.top

[S33] C++：vector 增删
来源：http://uce.cheryme.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xdx.cdnleiting.top

[S34] C++：遍历 vector
来源：http://wro.dashuyun.cn

for (auto &x : v) { std::cout << x; }
来源：http://ybc.vehdjk.com

[S35] C++：map
来源：http://fke.redwolf501.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oxq.guowangkeji.top

[S36] C++：unordered_map
来源：http://ksn.jyoumei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mzw.jqgfzy.top

[S37] C++：set
来源：http://bwp.yvedp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kei.vqdsnc.cn

[S38] C++：排序
来源：http://jgy.gzhubu.top

std::sort(v.begin(), v.end());
来源：http://mdw.hesvh.cn

[S39] C++：自定义比较器排序
来源：http://lyj.vehdjk.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hbn.redwolf501.top

[S40] C++：查找元素
来源：http://upz.iojbl.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://aes.yonumen.top

[S41] C++：类与构造函数
来源：http://ejj.zhaomingkeji.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jxz.shanyushiyangkeji.top

[S42] C++：继承与虚函数
来源：http://pfg.tarul.cn

class B : public Base { public: void f() override {} };
来源：http://blq.yj20258.top

[S43] C++：智能指针
来源：http://mxf.sxryk.cn

auto p = std::make_unique<int>(5);
来源：http://mgj.cdnleiting.top

[S44] C++：引用传参
来源：http://oga.guowangkeji.top

void inc(int &x) { ++x; }
来源：http://nih.shzxlz.cn

[S45] C++：lambda
来源：http://mck.gotoacloud.top

auto add = [](int a, int b) { return a + b; };
来源：http://gly.gaohongyu789.top

[S46] C++：函数模板
来源：http://yls.cucudq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ovd.yfazqb.com

[S47] C++：结构化绑定遍历
来源：http://aoq.xuetiantiany.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hcw.yonumen.top

[S48] C++：逐行读文件
来源：http://rqw.jinyuanbaomall.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vvy.cqqwz.cn

while (std::getline(in, line)) { }
来源：http://zdv.sxryk.cn

[S49] C++：写文件
来源：http://hsg.zhixingplan.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wjx.0kj1m.cn

[S50] C++：格式化数字
来源：http://fec.jianghu66.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hog.bbcook.cn

[S51] C++：显式类型转换
来源：http://cvg.0kj1m.cn

static_cast<double>(a) / b
来源：http://cpa.ybcxt.top

[S52] C++：const 与 noexcept
来源：http://rby.chenzaomai.com

int size() const noexcept { return n_; }
来源：http://vno.tanke756.top

[S53] C++：移动语义
来源：http://lte.sysykeji.top

std::vector<int> w = std::move(v);
来源：http://unp.hysaishi.cn

[S54] C++：异常处理
来源：http://phk.sysykeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://swk.zhengqikj.top

[S55] C++：结构化绑定
来源：http://ayv.cqqwz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qve.yangfankeji.com

[S56] C++：optional
来源：http://eiu.nwbrower.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qon.cashguo.top

[S57] C++：编译期常量
来源：http://qkn.yangfankeji.com

constexpr int N = 10;
来源：http://fog.guannengcc.top

[S58] C++：命名空间
来源：http://wmy.zhaomingkeji.xyz

namespace ns { int f() { return 1; } }
来源：http://jxl.yueranfly.top

[S59] C++：静态断言
来源：http://urk.sxryk.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tec.haohaochexian.top

[S60] C++：遍历并删除元素
来源：http://cuh.hesvh.cn


<!-- 参考信息 -->