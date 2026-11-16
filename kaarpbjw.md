代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://nhx.ehwqpu.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qsi.pycfn.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nfe.epnwcf.com

[Q89] 判断表是否存在
来源：http://pui.birdmap.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rsz.gaohongyu789.top

[Q90] 生成序号列
来源：http://epi.yj20258.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ngn.zycfv.cn

================================================================================
来源：http://kzk.bbcook.cn

R. Bash 专题
来源：http://tyr.redwolf501.top

================================================================================
来源：http://pez.fengsongda.top

[R01] shebang 与严格模式
来源：http://ihh.hnxiangtu.top

#!/usr/bin/env bash
来源：http://hjb.sjlbkw.cn

set -euo pipefail
来源：http://gey.shuidangran.top

[R02] 变量赋值与使用
来源：http://gxk.hnxiangtu.top

name="Tom"; echo "$name"
来源：http://abc.guannengcc.top

[R03] 只读变量
来源：http://mpw.zhongyouzk.top

readonly PI=3.14
来源：http://xuj.guowangkeji.top

[R04] 位置参数
来源：http://sxv.jinghuilouyu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cmz.yj202588.top

[R05] 参数默认值
来源：http://pju.xuetiantiany.cn

name="${1:-default}"
来源：http://usw.chenzaomai.com

[R06] 判断命令是否存在
来源：http://gup.sxryk.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yjn.yj20258888.top

[R07] if 判断文件
来源：http://fvl.jianghu66.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://oxc.sjlbkw.cn

[R08] 数值比较
来源：http://hsf.cashguo.top

if (( a > b )); then echo "a 更大"; fi
来源：http://dgl.quarkkingdee.top

[R09] 字符串比较
来源：http://ybj.bbcook.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tja.birdmap.top

[R10] 正则匹配
来源：http://uyr.dianchejie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nrv.tian-w.cn

[R11] case 多分支
来源：http://yhj.nanxuanxn.top

case "$1" in
来源：http://pcq.xinyue.icu

start) echo "启动" ;;
来源：http://mub.jianghu66.top

stop)  echo "停止" ;;
来源：http://ahi.wangdashe.top

*)     echo "未知命令" ;;
来源：http://zcf.svipenyu.cn

esac
来源：http://umf.redwolf501.top

[R12] for 遍历文件
来源：http://yty.yangfankeji.com

for f in *.txt; do echo "$f"; done
来源：http://ccc.fengsongda.top

[R13] for 计数循环
来源：http://ktb.havefunace.top

for i in {1..10}; do echo "$i"; done
来源：http://zuy.andypj.xyz

[R14] C 风格 for
来源：http://vyt.birdmap.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://asp.daxiang520.top

[R15] while 逐行读文件
来源：http://fvy.fengsongda.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lms.chenjidiqi.icu

[R16] until 等待条件
来源：http://wxr.hongshengwenyu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mfu.jinqigfzy.top

[R17] 数组定义与取值
来源：http://xnn.yfazqb.com

arr=(a b c); echo "${arr[0]}"
来源：http://dbf.shanyushiyangtech.top

[R18] 遍历数组
来源：http://jfp.pengpengdd.cyou

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hir.yj202588.top

[R19] 数组长度
来源：http://pia.chenlongwang.top

echo "${#arr[@]}"
来源：http://jrs.jyoumei.cn

[R20] 关联数组（字典）
来源：http://lsi.jianghu66.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cdy.daxiang520.top

[R21] 字符串长度
来源：http://ouc.aizwys.cn

echo "${#s}"
来源：http://vqf.zhaomingkeji.xyz

[R22] 截取子串
来源：http://afz.mhx1999.top

echo "${s:0:5}"
来源：http://cdv.vehdjk.com

[R23] 字符串替换
来源：http://oqw.hywenlv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ddg.chenjidiqi.icu

[R24] 大小写转换
来源：http://xxx.redwolf501.top

echo "${s^^}"; echo "${s,,}"
来源：http://fil.fehbvm.com

[R25] 去后缀 / 去前缀
来源：http://pwr.0kj1m.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rwx.daxiang520.top

[R26] 命令替换
来源：http://upo.chenzaomai.com

now=$(date +%F); echo "$now"
来源：http://zdn.kuanghao11.cn

[R27] 算术展开
来源：http://eqt.cqqwz.cn

echo $((1 + 2 * 3))
来源：http://hxz.zhijiandao.cn

[R28] 浮点运算
来源：http://lva.xuetiantiany.cn

echo "scale=2; 10/3" | bc
来源：http://rod.iojbl.cn

[R29] 定义函数
来源：http://dlc.zhengqikj.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yym.yfazqb.com

[R30] 函数返回状态码
来源：http://tdi.xuetiantiany.cn

f() { return 0; }; f || echo "失败了"
来源：http://epk.gzhubu.top

[R31] 局部变量
来源：http://lqe.birdmap.top

f() { local x=1; echo "$x"; }
来源：http://ayw.guannengcc.top

[R32] 参数个数校验
来源：http://ttm.0kj1m.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mxi.jinyuanbaomall.cn

[R33] 捕获错误并提示行号
来源：http://zvk.cucudq.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nyx.cdnleiting.top

[R34] 退出时清理
来源：http://yon.gogol.net.cn

trap 'rm -f "$tmp"' EXIT
来源：http://udx.ivvv.top

[R35] 后台执行并等待
来源：http://kbq.ppjwa.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zqq.ctjpmb.com

[R36] 并发执行多个任务
来源：http://mvh.jiagoushi.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rhc.zhijiandao.cn

[R37] 把输出赋给变量
来源：http://ysc.hcnkem.com

files=$(ls -1)
来源：http://nuq.mhx1999.top

[R38] 管道串联
来源：http://yyq.zdqjudy.top

cat a.txt | grep -i error | wc -l
来源：http://kto.fanxiaobao.xyz

[R39] 重定向标准输出与错误
来源：http://yjg.nanxinkj.top

cmd > out.log 2>&1
来源：http://aha.hfpthk.cn

[R40] 追加写日志
来源：http://eso.yuxming.cn

echo "log" >> out.log
来源：http://arl.vqdsnc.cn

[R41] 丢弃输出
来源：http://kzr.shanyushiyangkeji.top

cmd >/dev/null 2>&1
来源：http://kju.fzhhl.top

[R42] 输入重定向
来源：http://ojs.vehdjk.com

wc -l < a.txt
来源：http://utz.chenlongwang.top

[R43] 按名字查找文件
来源：http://pbh.vehdjk.com

find . -name "*.log" -type f
来源：http://clb.yongpay.top

[R44] 按修改时间查找
来源：http://rmc.dianchejie.cn

find . -mtime -7 -type f
来源：http://cbk.guannengcc.top

[R45] 批量删除
来源：http://zxd.jiagoushi.top

find . -name "*.tmp" -delete
来源：http://qrf.nanxinkj.top

[R46] 递归替换文件内容
来源：http://jyj.dianchejie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://huq.xinyue.icu

[R47] sed 单行替换
来源：http://dyh.ybcxt.top

sed -i 's/foo/bar/g' a.txt
来源：http://qrq.zhengqikj.top

[R48] awk 取指定列
来源：http://xqm.tian-w.cn

awk '{print $1, $3}' a.txt
来源：http://ytj.yfazqb.com

[R49] awk 带条件
来源：http://bpv.yuxming.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qdr.wangshuangyany.cn

[R50] awk 求和
来源：http://ors.feifeiyinyue.top

awk '{s += $2} END {print s}' a.txt
来源：http://kke.zhoulong.xyz

[R51] 排序去重取前几
来源：http://fei.shangyingyoupin.top

sort a.txt | uniq -c | sort -rn | head
来源：http://pvu.jlsjyb.cn

[R52] 统计行数
来源：http://nnt.ywan-chungtsiang.top

wc -l a.txt
来源：http://igk.daria6918.cn

[R53] 查看文件头与实时尾
来源：http://occ.cdnleiting.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ful.xuanzx.com

[R54] 比较两个文件
来源：http://muv.vqdsnc.cn

diff a.txt b.txt
来源：http://qbl.yueranfly.top

[R55] 压缩与解压
来源：http://oiz.vqdsnc.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uuf.andypj.xyz

[R56] 远程拷贝
来源：http://cvd.shanyushiyangkeji.top

scp file user@host:/path/
来源：http://ict.xuanzx.com

[R57] 远程执行命令
来源：http://lqp.svipenyu.cn

ssh user@host 'uptime'
来源：http://yhz.zhongyouzk.top

[R58] 下载文件
来源：http://yfo.tanke756.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vmk.yanxiufei.cn

[R59] 发 POST JSON
来源：http://ytz.xuanzx.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hgq.hywenlv.cn

[R60] 只看 HTTP 状态码
来源：http://mdx.andypj.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tdz.gzhubu.top

[R61] 磁盘占用
来源：http://etu.guowangkeji.top

df -h;  du -sh *
来源：http://bgy.gzhubu.top

[R62] 找最占空间的文件
来源：http://tsa.shzxlz.cn

du -ah . | sort -rh | head -10
来源：http://ddo.haohaochexian.top

[R63] 内存与进程
来源：http://djd.hnqzz.top

free -h;  ps aux | grep nginx
来源：http://aau.zhijiandao.cn

[R64] 结束进程
来源：http://nds.shanyushiyangkeji.top

kill -9 $(pgrep -f app.py)
来源：http://ass.tian-w.cn

[R65] 查看端口占用
来源：http://udw.tianlin.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cff.chenzaomai.com

[R66] 定时任务
来源：http://xga.jqgfzy.top

crontab -e;  crontab -l
来源：http://xnu.jyoumei.cn

[R67] 生成随机十六进制串
来源：http://mlm.vqdsnc.cn

openssl rand -hex 16
来源：http://xxu.quarkkingdee.top

[R68] 计算文件校验值
来源：http://dbx.dianchejie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zyf.fehbvm.com

[R69] 生成随机密码
来源：http://msp.jianghu66.top

head -c 16 /dev/urandom | base64
来源：http://ase.yongpay.top

[R70] 时间戳与互转
来源：http://uhc.gogol.net.cn

date +%s;  date -d @1700000000
来源：http://mem.zhongyouzk.top

[R71] 日期格式化
来源：http://ghg.zhengqikj.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ojh.andypj.xyz

[R72] 等待端口就绪
来源：http://nkx.jinqigfzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://uyf.xuetiantiany.cn

[R73] 分割大日志
来源：http://xib.cheryme.top

split -l 1000 big.log part_
来源：http://dyy.c1oappe.top

[R74] 批量重命名
来源：http://dzq.guowangkeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yqz.hnqzz.top

[R75] 导出环境变量
来源：http://ote.fktsv.cn

export PATH="$HOME/bin:$PATH"
来源：http://yat.chenzaomai.com

[R76] 使用临时文件
来源：http://adh.shuidangran.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fgh.sufxvd.cn

[R77] 读取用户输入
来源：http://tqq.birdmap.top

read -rp "请输入: " ans
来源：http://okl.fzhhl.top

[R78] 交互式菜单
来源：http://bms.xingfuxueyuan.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://jpz.shzxlz.cn

[R79] 解析命令行选项
来源：http://obk.yj202588.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kan.hnqzz.top

[R80] 查看脚本执行耗时
来源：http://lvj.vehdjk.com

time ./run.sh
来源：http://ece.316326.xyz

================================================================================
来源：http://zdr.jiagoushi.top

S. C / C++ 专题
来源：http://bmn.sufxvd.cn

================================================================================
来源：http://xmr.cucudq.cn

[S01] C：Hello World
来源：http://qam.fktsv.cn

#include <stdio.h>
来源：http://inc.uphjek.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://cxz.yvedp.cn

[S02] C：变量与格式化输出
来源：http://etj.gzhubu.top

int a = 10; printf("%d\n", a);
来源：http://ahp.aizwys.cn

[S03] C：读入整数
来源：http://qjw.ywan-chungtsiang.top

int x; scanf("%d", &x);
来源：http://jhy.316326.xyz

[S04] C：字符串复制
来源：http://spt.bjfxy.top

char dst[32]; strcpy(dst, "hi");
来源：http://oyp.tanke756.top

[S05] C：字符串长度
来源：http://chr.ybcxt.top

strlen(s)
来源：http://cfl.jinqigufen.top

[S06] C：字符串比较
来源：http://ikt.ywan-chungtsiang.top

strcmp(a, b) == 0
来源：http://ozu.xuanzx.com

[S07] C：数组遍历求和
来源：http://yts.wangshuangyany.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dar.yvedp.cn

[S08] C：动态内存分配与释放
来源：http://ldw.hnxiangtu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dbl.hnxiangtu.top

[S09] C：结构体定义与初始化
来源：http://mgi.316326.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kxq.guowangkeji.top

[S10] C：指针与解引用
来源：http://ora.cashguo.top

int *p = &a;  *p = 5;
来源：http://iwg.xingfuxueyuan.xyz

[S11] C：逐行读文件
来源：http://mqq.c1oappe.top

FILE *f = fopen("a.txt", "r");
来源：http://vit.jianghu66.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ugw.xylfe.cn

fclose(f);
来源：http://izd.jinyuanbaomall.cn

[S12] C：写文件
来源：http://oho.316326.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qkd.shuidangran.top

[S13] C：宏定义
来源：http://khl.fehbvm.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wdq.zhijiandao.cn

[S14] C：枚举
来源：http://rip.mhx1999.top

enum Color { RED, GREEN, BLUE };
来源：http://dod.daria6918.cn

[S15] C：类型转换
来源：http://nqp.daxiang520.top

(double) a / b
来源：http://cul.chenzaomai.com

[S16] C：位操作置位
来源：http://leu.nwbrower.top

x |= (1 << 3);
来源：http://myk.xinyue.icu

[S17] C：安全拼接字符串
来源：http://wdt.quarkkingdee.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qft.feifeiyinyue.top

[S18] C：命令行参数
来源：http://jze.zhongyouzk.top

int main(int argc, char **argv)
来源：http://caf.cucudq.cn

[S19] C：快速排序
来源：http://tqs.ybcxt.top

qsort(a, n, sizeof(int), cmp);
来源：http://mgh.zhengqikj.top

[S20] C：二分查找
来源：http://ckz.tarul.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://btj.52xcode.cn

[S21] C：字符类别判断
来源：http://ccl.fzhhl.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zjt.cqqwz.cn

[S22] C：字符串转数字
来源：http://dsm.yvedp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kwm.sweek.top

[S23] C：随机数
来源：http://bne.ywan-chungtsiang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://gxw.zhengqikj.top

[S24] C：获取本地时间
来源：http://ukh.hnxiangtu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ruo.xingfuxueyuan.xyz

[S25] C：内存拷贝
来源：http://afn.iojbl.cn

memcpy(dst, src, n);
来源：http://kvc.cheryme.top

[S26] C：内存清零
来源：http://rgm.zhaomingkeji.xyz

memset(a, 0, sizeof a);
来源：http://con.zhengqikj.top

[S27] C：定义常量
来源：http://lag.zhengqikj.top

const double PI = 3.14159;
来源：http://sjs.52xcode.cn

[S28] C：静态变量
来源：http://slm.jianghu66.top

static int counter = 0;
来源：http://pve.hesvh.cn

[S29] C：变参函数
来源：http://bsy.havefunace.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mnw.jqgufenzy.top

[S30] C：头文件保护
来源：http://non.sxryk.cn

#ifndef X_H
来源：http://abc.tanke756.top

#define X_H
来源：http://mtr.bjfxy.top

#endif
来源：http://ukz.shanyushiyangkeji.top

[S31] C++：Hello World
来源：http://wno.fzhhl.top

#include <iostream>
来源：http://syg.shanyushiyangtech.top

int main() { std::cout << "Hello\n"; }
来源：http://iqh.ivvv.top

[S32] C++：字符串
来源：http://xor.gotoacloud.top

std::string s = "hi";  s += "!";
来源：http://wxa.fanxiaobao.xyz

[S33] C++：vector 增删
来源：http://poj.ppjwa.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gxn.zhixingplan.top

[S34] C++：遍历 vector
来源：http://iak.jqgufenzy.top

for (auto &x : v) { std::cout << x; }
来源：http://ftb.yj20258888.top

[S35] C++：map
来源：http://laz.jyoumei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jnb.bjfxy.top

[S36] C++：unordered_map
来源：http://aat.sweek.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zil.yuxming.cn

[S37] C++：set
来源：http://bjq.wangdashe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wly.xziqi.cn

[S38] C++：排序
来源：http://ace.zycfv.cn

std::sort(v.begin(), v.end());
来源：http://alw.ydzc1.top

[S39] C++：自定义比较器排序
来源：http://njh.ehwqpu.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zbx.wangshuangyany.cn

[S40] C++：查找元素
来源：http://nkv.zhoulong.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xno.bbcook.cn

[S41] C++：类与构造函数
来源：http://rts.sufxvd.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qsp.mhx1999.top

[S42] C++：继承与虚函数
来源：http://ehv.cdnleiting.top

class B : public Base { public: void f() override {} };
来源：http://jed.wangdashe.top

[S43] C++：智能指针
来源：http://ofo.zhoulong.xyz

auto p = std::make_unique<int>(5);
来源：http://yku.ydjk.org.cn

[S44] C++：引用传参
来源：http://dbj.hysaishi.cn

void inc(int &x) { ++x; }
来源：http://elf.snrcjt.cn

[S45] C++：lambda
来源：http://uot.pycfn.com

auto add = [](int a, int b) { return a + b; };
来源：http://tpo.hysaishi.cn

[S46] C++：函数模板
来源：http://wlx.jiagoushi.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vag.tianlin.xyz

[S47] C++：结构化绑定遍历
来源：http://meu.dashuyun.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://krq.chenzaomai.com

[S48] C++：逐行读文件
来源：http://lhg.chenlongwang.top

std::ifstream in("a.txt");  std::string line;
来源：http://sdb.yvedp.cn

while (std::getline(in, line)) { }
来源：http://wxp.meibo888.top

[S49] C++：写文件
来源：http://vbs.guowangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mgv.0kj1m.cn

[S50] C++：格式化数字
来源：http://pcd.guowangkeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vqf.zhoulong.xyz

[S51] C++：显式类型转换
来源：http://bxd.hcnkem.com

static_cast<double>(a) / b
来源：http://wom.tian-w.cn

[S52] C++：const 与 noexcept
来源：http://cnr.c1oappe.top

int size() const noexcept { return n_; }
来源：http://clp.jiagoushi.top

[S53] C++：移动语义
来源：http://agb.ctjpmb.com

std::vector<int> w = std::move(v);
来源：http://sll.yj20258888.top

[S54] C++：异常处理
来源：http://znz.yongpay.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hdw.chenzaomai.com

[S55] C++：结构化绑定
来源：http://iuu.zhiwuduotai.top

auto [a, b] = std::make_pair(1, 2);
来源：http://xxp.yuanzhike.top

[S56] C++：optional
来源：http://bop.fengsongda.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nda.hammf.cn

[S57] C++：编译期常量
来源：http://nkq.ydjk.org.cn

constexpr int N = 10;
来源：http://dna.svipenyu.cn

[S58] C++：命名空间
来源：http://lio.hongshengwenyu.top


<!-- 参考信息 -->