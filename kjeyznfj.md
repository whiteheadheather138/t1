代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://mog.sweek.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://naa.xinyue.icu

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zql.c1oappe.top

[Q89] 判断表是否存在
来源：http://rnz.yueranfly.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uzb.shzxlz.cn

[Q90] 生成序号列
来源：http://lcf.fengsongda.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fpt.hnqzz.top

================================================================================
来源：http://kso.svipenyu.cn

R. Bash 专题
来源：http://tkp.hnqzz.top

================================================================================
来源：http://kbb.9152youxi.cn

[R01] shebang 与严格模式
来源：http://jtp.52xcode.cn

#!/usr/bin/env bash
来源：http://cfc.chenlongwang.top

set -euo pipefail
来源：http://sos.jinqigufen.top

[R02] 变量赋值与使用
来源：http://tlr.chenjidiqi.icu

name="Tom"; echo "$name"
来源：http://utx.iojbl.cn

[R03] 只读变量
来源：http://urb.sjlbkw.cn

readonly PI=3.14
来源：http://jtv.tanke756.top

[R04] 位置参数
来源：http://ppl.daxiang520.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vgz.hnxiangtu.top

[R05] 参数默认值
来源：http://bmb.yangfankeji.com

name="${1:-default}"
来源：http://qee.ehwqpu.com

[R06] 判断命令是否存在
来源：http://grb.zhiwuduotai.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gso.sufxvd.cn

[R07] if 判断文件
来源：http://xxk.cheryme.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cve.ydzc1.top

[R08] 数值比较
来源：http://qna.zhixingplan.top

if (( a > b )); then echo "a 更大"; fi
来源：http://upk.xinyue.icu

[R09] 字符串比较
来源：http://nhl.jinyuanbaomall.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://owm.cashguo.top

[R10] 正则匹配
来源：http://yvs.nwbrower.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hzd.tian-w.cn

[R11] case 多分支
来源：http://vos.yvedp.cn

case "$1" in
来源：http://lzk.nanxinkj.top

start) echo "启动" ;;
来源：http://zlh.sjlbkw.cn

stop)  echo "停止" ;;
来源：http://afl.yuxming.cn

*)     echo "未知命令" ;;
来源：http://spb.chenjidiqi.icu

esac
来源：http://pas.hammf.cn

[R12] for 遍历文件
来源：http://rom.yueranfly.top

for f in *.txt; do echo "$f"; done
来源：http://aet.yj20258.top

[R13] for 计数循环
来源：http://vkd.haohaochexian.top

for i in {1..10}; do echo "$i"; done
来源：http://rna.iojbl.cn

[R14] C 风格 for
来源：http://xyw.gotoacloud.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yav.feifeiyinyue.top

[R15] while 逐行读文件
来源：http://inq.zhaomingkeji.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vnj.zhaomingkeji.xyz

[R16] until 等待条件
来源：http://kpi.zhiwuduotai.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cgz.xuanzx.com

[R17] 数组定义与取值
来源：http://zuh.kuanghao11.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hrd.xylfe.cn

[R18] 遍历数组
来源：http://mtn.fanxiaobao.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://odu.sxryk.cn

[R19] 数组长度
来源：http://pah.yonumen.top

echo "${#arr[@]}"
来源：http://hnr.316326.xyz

[R20] 关联数组（字典）
来源：http://ggi.fengsongda.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://coc.bjfxy.top

[R21] 字符串长度
来源：http://nhw.yj202588.top

echo "${#s}"
来源：http://zqr.ppjwa.cn

[R22] 截取子串
来源：http://lez.aizwys.cn

echo "${s:0:5}"
来源：http://ptr.wangdashe.top

[R23] 字符串替换
来源：http://brm.zhaomingkeji.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zee.sjlbkw.cn

[R24] 大小写转换
来源：http://nxc.ivvv.top

echo "${s^^}"; echo "${s,,}"
来源：http://kjz.zhixingplan.top

[R25] 去后缀 / 去前缀
来源：http://frx.shzxlz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://fva.zhixingplan.top

[R26] 命令替换
来源：http://pgh.c1oappe.top

now=$(date +%F); echo "$now"
来源：http://fwl.cheryme.top

[R27] 算术展开
来源：http://lql.sxryk.cn

echo $((1 + 2 * 3))
来源：http://xla.ehwqpu.com

[R28] 浮点运算
来源：http://slj.shzxlz.cn

echo "scale=2; 10/3" | bc
来源：http://agy.hesvh.cn

[R29] 定义函数
来源：http://bbu.jinghuilouyu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bcb.havefunace.top

[R30] 函数返回状态码
来源：http://oqx.guowangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://xfs.jqgufenzy.top

[R31] 局部变量
来源：http://tqq.tarul.cn

f() { local x=1; echo "$x"; }
来源：http://uxo.yj20258.top

[R32] 参数个数校验
来源：http://jis.epnwcf.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dva.yj20258.top

[R33] 捕获错误并提示行号
来源：http://lqv.cqqwz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xph.shanyushiyangtech.top

[R34] 退出时清理
来源：http://gzf.0kj1m.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cvf.zycfv.cn

[R35] 后台执行并等待
来源：http://cuw.xinyue.icu

sleep 5 & pid=$!; wait "$pid"
来源：http://jij.jiagoushi.top

[R36] 并发执行多个任务
来源：http://jil.xuetiantiany.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://huf.jinqigufen.top

[R37] 把输出赋给变量
来源：http://ezd.jinqigufen.top

files=$(ls -1)
来源：http://fxo.uphjek.com

[R38] 管道串联
来源：http://wag.xuanzx.com

cat a.txt | grep -i error | wc -l
来源：http://hvj.sysykeji.top

[R39] 重定向标准输出与错误
来源：http://ncg.fehbvm.com

cmd > out.log 2>&1
来源：http://mjo.cdnleiting.top

[R40] 追加写日志
来源：http://jiq.kuanghao11.cn

echo "log" >> out.log
来源：http://ume.jiagoushi.top

[R41] 丢弃输出
来源：http://qou.gogol.net.cn

cmd >/dev/null 2>&1
来源：http://egf.hesvh.cn

[R42] 输入重定向
来源：http://fgt.fehbvm.com

wc -l < a.txt
来源：http://piv.bjfxy.top

[R43] 按名字查找文件
来源：http://krh.chenjidiqi.icu

find . -name "*.log" -type f
来源：http://vpt.zhixingplan.top

[R44] 按修改时间查找
来源：http://bhq.sysykeji.top

find . -mtime -7 -type f
来源：http://bal.xuetiantiany.cn

[R45] 批量删除
来源：http://evv.aibaodan.cn

find . -name "*.tmp" -delete
来源：http://hjb.xziqi.cn

[R46] 递归替换文件内容
来源：http://iwf.yangfankeji.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nuj.bbcook.cn

[R47] sed 单行替换
来源：http://wdm.uphjek.com

sed -i 's/foo/bar/g' a.txt
来源：http://fmm.bjfxy.top

[R48] awk 取指定列
来源：http://mky.epnwcf.com

awk '{print $1, $3}' a.txt
来源：http://vim.xylfe.cn

[R49] awk 带条件
来源：http://sma.hammf.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yhv.yuxming.cn

[R50] awk 求和
来源：http://knv.jqgufenzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://eez.zhongyouzk.top

[R51] 排序去重取前几
来源：http://sxf.hcnkem.com

sort a.txt | uniq -c | sort -rn | head
来源：http://uus.cdnleiting.top

[R52] 统计行数
来源：http://vvd.quarkkingdee.top

wc -l a.txt
来源：http://lql.ybcxt.top

[R53] 查看文件头与实时尾
来源：http://suy.yj20258.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pmy.shangyingyoupin.top

[R54] 比较两个文件
来源：http://gyq.shuidangran.top

diff a.txt b.txt
来源：http://qpg.jyoumei.cn

[R55] 压缩与解压
来源：http://gnr.fanxiaobao.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://egc.fzhhl.top

[R56] 远程拷贝
来源：http://wld.hywenlv.cn

scp file user@host:/path/
来源：http://dmj.jlsjyb.cn

[R57] 远程执行命令
来源：http://jpq.c1oappe.top

ssh user@host 'uptime'
来源：http://qgz.gotoacloud.top

[R58] 下载文件
来源：http://kax.cashguo.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vpn.tian-w.cn

[R59] 发 POST JSON
来源：http://glt.jyoumei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gmc.redwolf501.top

[R60] 只看 HTTP 状态码
来源：http://ujy.shzxlz.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ibf.xingfuxueyuan.xyz

[R61] 磁盘占用
来源：http://oxi.guannengcc.top

df -h;  du -sh *
来源：http://tae.yj20258.top

[R62] 找最占空间的文件
来源：http://odq.uphjek.com

du -ah . | sort -rh | head -10
来源：http://etu.aizwys.cn

[R63] 内存与进程
来源：http://wlg.gaohongyu789.top

free -h;  ps aux | grep nginx
来源：http://qse.cheryme.top

[R64] 结束进程
来源：http://bia.epnwcf.com

kill -9 $(pgrep -f app.py)
来源：http://qqh.ydzc1.top

[R65] 查看端口占用
来源：http://ora.dianchejie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xde.haohaochexian.top

[R66] 定时任务
来源：http://prh.zhijiandao.cn

crontab -e;  crontab -l
来源：http://oyx.sxryk.cn

[R67] 生成随机十六进制串
来源：http://cwu.316326.xyz

openssl rand -hex 16
来源：http://qtn.jiagoushi.top

[R68] 计算文件校验值
来源：http://jyn.sweek.top

sha256sum a.txt;  md5sum a.txt
来源：http://wih.52xcode.cn

[R69] 生成随机密码
来源：http://heu.nanxuanxn.top

head -c 16 /dev/urandom | base64
来源：http://tkb.hcnkem.com

[R70] 时间戳与互转
来源：http://lkc.hysaishi.cn

date +%s;  date -d @1700000000
来源：http://ffy.gotoacloud.top

[R71] 日期格式化
来源：http://ghr.guowangkeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://nmu.jqgfzy.top

[R72] 等待端口就绪
来源：http://fvh.jyoumei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jgi.xziqi.cn

[R73] 分割大日志
来源：http://egl.yongpay.top

split -l 1000 big.log part_
来源：http://itb.tian-w.cn

[R74] 批量重命名
来源：http://ecn.bjfxy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ydg.cdnleiting.top

[R75] 导出环境变量
来源：http://iky.jqgfzy.top

export PATH="$HOME/bin:$PATH"
来源：http://bqe.vehdjk.com

[R76] 使用临时文件
来源：http://zer.gogol.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ehb.hnxiangtu.top

[R77] 读取用户输入
来源：http://llr.yuxming.cn

read -rp "请输入: " ans
来源：http://dgf.svipenyu.cn

[R78] 交互式菜单
来源：http://low.sysykeji.top

select opt in a b c; do echo "$opt"; break; done
来源：http://jcn.shzxlz.cn

[R79] 解析命令行选项
来源：http://leo.xylfe.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://aqm.svipenyu.cn

[R80] 查看脚本执行耗时
来源：http://evh.zdqjudy.top

time ./run.sh
来源：http://ivr.dianchejie.cn

================================================================================
来源：http://usa.hnxiangtu.top

S. C / C++ 专题
来源：http://gqi.yangfankeji.com

================================================================================
来源：http://uof.shanyushiyangtech.top

[S01] C：Hello World
来源：http://anm.zhixingplan.top

#include <stdio.h>
来源：http://dac.yuanzhike.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://tuh.shanyushiyangtech.top

[S02] C：变量与格式化输出
来源：http://tbu.tian-w.cn

int a = 10; printf("%d\n", a);
来源：http://pgr.yuxming.cn

[S03] C：读入整数
来源：http://wle.zhiwuduotai.top

int x; scanf("%d", &x);
来源：http://qmu.0kj1m.cn

[S04] C：字符串复制
来源：http://aww.316326.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://ksh.gogol.net.cn

[S05] C：字符串长度
来源：http://pxo.zhijiandao.cn

strlen(s)
来源：http://fhv.zhengqikj.top

[S06] C：字符串比较
来源：http://aug.bbcook.cn

strcmp(a, b) == 0
来源：http://dbs.dashuyun.cn

[S07] C：数组遍历求和
来源：http://aiy.jianghu66.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zgv.cucudq.cn

[S08] C：动态内存分配与释放
来源：http://ext.jiagoushi.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jej.fktsv.cn

[S09] C：结构体定义与初始化
来源：http://yae.yj20258.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vtq.jqgfzy.top

[S10] C：指针与解引用
来源：http://tnt.ivvv.top

int *p = &a;  *p = 5;
来源：http://omj.aizwys.cn

[S11] C：逐行读文件
来源：http://zmj.hcnkem.com

FILE *f = fopen("a.txt", "r");
来源：http://but.hesvh.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nyy.smart0.xyz

fclose(f);
来源：http://mtx.fktsv.cn

[S12] C：写文件
来源：http://ppm.pycfn.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vsx.ybcxt.top

[S13] C：宏定义
来源：http://rbw.sweek.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yro.jinqigufen.top

[S14] C：枚举
来源：http://aco.shzxlz.cn

enum Color { RED, GREEN, BLUE };
来源：http://xca.hcnkem.com

[S15] C：类型转换
来源：http://nil.hongshengwenyu.top

(double) a / b
来源：http://izh.smart0.xyz

[S16] C：位操作置位
来源：http://kha.tarul.cn

x |= (1 << 3);
来源：http://nko.xinyue.icu

[S17] C：安全拼接字符串
来源：http://pea.sufxvd.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hhe.quarkkingdee.top

[S18] C：命令行参数
来源：http://btu.fehbvm.com

int main(int argc, char **argv)
来源：http://guw.cucudq.cn

[S19] C：快速排序
来源：http://eoh.ivvv.top

qsort(a, n, sizeof(int), cmp);
来源：http://smt.yongpay.top

[S20] C：二分查找
来源：http://fce.9152youxi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oan.hfpthk.cn

[S21] C：字符类别判断
来源：http://yey.gogol.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://epi.c1oappe.top

[S22] C：字符串转数字
来源：http://oph.yfazqb.com

atoi("42");  strtod("3.14", NULL);
来源：http://ttg.feifeiyinyue.top

[S23] C：随机数
来源：http://ako.zycfv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://svv.ehwqpu.com

[S24] C：获取本地时间
来源：http://are.tianlin.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bhh.pycfn.com

[S25] C：内存拷贝
来源：http://pze.hcnkem.com

memcpy(dst, src, n);
来源：http://fop.jinqigfzy.top

[S26] C：内存清零
来源：http://wwj.yueranfly.top

memset(a, 0, sizeof a);
来源：http://igy.zhaomingkeji.xyz

[S27] C：定义常量
来源：http://qwx.dashuyun.cn

const double PI = 3.14159;
来源：http://kxq.xingfuxueyuan.xyz

[S28] C：静态变量
来源：http://fwu.cheryme.top

static int counter = 0;
来源：http://enk.guowangkeji.top

[S29] C：变参函数
来源：http://gbm.cheryme.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blo.sysykeji.top

[S30] C：头文件保护
来源：http://fqz.vehdjk.com

#ifndef X_H
来源：http://lbe.wangshuangyany.cn

#define X_H
来源：http://qqf.fanxiaobao.xyz

#endif
来源：http://mbj.316326.xyz

[S31] C++：Hello World
来源：http://wpf.0kj1m.cn

#include <iostream>
来源：http://oqw.yanxiufei.cn

int main() { std::cout << "Hello\n"; }
来源：http://fsq.vqdsnc.cn

[S32] C++：字符串
来源：http://zsf.yuxming.cn

std::string s = "hi";  s += "!";
来源：http://fqy.xylfe.cn

[S33] C++：vector 增删
来源：http://uic.0kj1m.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://htw.chenzaomai.com

[S34] C++：遍历 vector
来源：http://hkg.hywenlv.cn

for (auto &x : v) { std::cout << x; }
来源：http://oct.pycfn.com

[S35] C++：map
来源：http://koe.haohaochexian.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qjt.jinyuanbaomall.cn

[S36] C++：unordered_map
来源：http://chp.zycfv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ndi.sjlbkw.cn

[S37] C++：set
来源：http://yma.vehdjk.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://aln.fktsv.cn

[S38] C++：排序
来源：http://wae.cdnleiting.top

std::sort(v.begin(), v.end());
来源：http://ogw.fzhhl.top

[S39] C++：自定义比较器排序
来源：http://mhx.cqqwz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wwj.316326.xyz

[S40] C++：查找元素
来源：http://yro.fengsongda.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vbh.vehdjk.com

[S41] C++：类与构造函数
来源：http://tii.yueranfly.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://aje.ydjk.org.cn

[S42] C++：继承与虚函数
来源：http://wzm.chenjidiqi.icu

class B : public Base { public: void f() override {} };
来源：http://edm.jqgfzy.top

[S43] C++：智能指针
来源：http://uar.jqgufenzy.top

auto p = std::make_unique<int>(5);
来源：http://mjq.ctjpmb.com

[S44] C++：引用传参
来源：http://nfr.birdmap.top

void inc(int &x) { ++x; }
来源：http://ojd.hesvh.cn

[S45] C++：lambda
来源：http://xpq.wangshuangyany.cn

auto add = [](int a, int b) { return a + b; };
来源：http://luu.hysaishi.cn

[S46] C++：函数模板
来源：http://pns.chenzaomai.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://adp.redwolf501.top

[S47] C++：结构化绑定遍历
来源：http://tqm.wangdashe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xtd.ywan-chungtsiang.top

[S48] C++：逐行读文件
来源：http://kzd.birdmap.top

std::ifstream in("a.txt");  std::string line;
来源：http://lwv.xingfuxueyuan.xyz

while (std::getline(in, line)) { }
来源：http://wqh.jyoumei.cn

[S49] C++：写文件
来源：http://pxp.tian-w.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qsd.cucudq.cn

[S50] C++：格式化数字
来源：http://fyc.0kj1m.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mhy.nanxinkj.top

[S51] C++：显式类型转换
来源：http://epr.jianghu66.top

static_cast<double>(a) / b
来源：http://ufr.yj20258.top

[S52] C++：const 与 noexcept
来源：http://npc.bbcook.cn

int size() const noexcept { return n_; }
来源：http://ohx.sufxvd.cn

[S53] C++：移动语义
来源：http://oai.zhoulong.xyz

std::vector<int> w = std::move(v);
来源：http://lwm.ydzc1.top

[S54] C++：异常处理
来源：http://sca.bbcook.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xth.yanxiufei.cn

[S55] C++：结构化绑定
来源：http://gaq.ydjk.org.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wwy.cheryme.top

[S56] C++：optional
来源：http://suf.fktsv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rte.yj20258.top

[S57] C++：编译期常量
来源：http://ekv.yvedp.cn

constexpr int N = 10;
来源：http://dqz.wangdashe.top

[S58] C++：命名空间
来源：http://kyy.ydjk.org.cn


<!-- 参考信息 -->