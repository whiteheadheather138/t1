代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://upk.cheryme.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://otk.yj202588.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xve.svipenyu.cn

[Q89] 判断表是否存在
来源：http://ski.sysykeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uhr.jinqigufen.top

[Q90] 生成序号列
来源：http://osr.hysaishi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bot.haohaochexian.top

================================================================================
来源：http://ntl.aibaodan.cn

R. Bash 专题
来源：http://kas.ydzc1.top

================================================================================
来源：http://keo.hfpthk.cn

[R01] shebang 与严格模式
来源：http://myy.nanxuanxn.top

#!/usr/bin/env bash
来源：http://pbd.shanyushiyangtech.top

set -euo pipefail
来源：http://yep.ybcxt.top

[R02] 变量赋值与使用
来源：http://dsh.nanxuanxn.top

name="Tom"; echo "$name"
来源：http://xyf.daxiang520.top

[R03] 只读变量
来源：http://omj.nanxuanxn.top

readonly PI=3.14
来源：http://tcn.nwbrower.top

[R04] 位置参数
来源：http://jyg.redwolf501.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qtg.tian-w.cn

[R05] 参数默认值
来源：http://nya.zhengqikj.top

name="${1:-default}"
来源：http://gex.fehbvm.com

[R06] 判断命令是否存在
来源：http://iik.zhaomingkeji.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qae.hesvh.cn

[R07] if 判断文件
来源：http://dqs.9152youxi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jhv.sjlbkw.cn

[R08] 数值比较
来源：http://cul.zdqjudy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://sck.hysaishi.cn

[R09] 字符串比较
来源：http://ulx.xziqi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wfw.birdmap.top

[R10] 正则匹配
来源：http://szt.daxiang520.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ebd.hnqzz.top

[R11] case 多分支
来源：http://waz.yueranfly.top

case "$1" in
来源：http://yoq.hammf.cn

start) echo "启动" ;;
来源：http://rfy.nanxuanxn.top

stop)  echo "停止" ;;
来源：http://uwk.feifeiyinyue.top

*)     echo "未知命令" ;;
来源：http://spu.fengsongda.top

esac
来源：http://fad.shanyushiyangtech.top

[R12] for 遍历文件
来源：http://wxm.hnxiangtu.top

for f in *.txt; do echo "$f"; done
来源：http://rgd.feifeiyinyue.top

[R13] for 计数循环
来源：http://mro.dianchejie.cn

for i in {1..10}; do echo "$i"; done
来源：http://yyn.hesvh.cn

[R14] C 风格 for
来源：http://uac.gogol.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iop.tian-w.cn

[R15] while 逐行读文件
来源：http://mkh.jyoumei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://prg.uphjek.com

[R16] until 等待条件
来源：http://lpt.pengpengdd.cyou

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yid.tian-w.cn

[R17] 数组定义与取值
来源：http://zwy.havefunace.top

arr=(a b c); echo "${arr[0]}"
来源：http://deh.tianlin.xyz

[R18] 遍历数组
来源：http://qya.shuidangran.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://adx.ctjpmb.com

[R19] 数组长度
来源：http://qds.tarul.cn

echo "${#arr[@]}"
来源：http://uve.cdnleiting.top

[R20] 关联数组（字典）
来源：http://azp.yangfankeji.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ibr.hnxiangtu.top

[R21] 字符串长度
来源：http://dvj.zycfv.cn

echo "${#s}"
来源：http://sfi.vqdsnc.cn

[R22] 截取子串
来源：http://ytn.cheryme.top

echo "${s:0:5}"
来源：http://pkt.hnxiangtu.top

[R23] 字符串替换
来源：http://gdd.hnqzz.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ruz.hongshengwenyu.top

[R24] 大小写转换
来源：http://jwp.chenzaomai.com

echo "${s^^}"; echo "${s,,}"
来源：http://azk.yfazqb.com

[R25] 去后缀 / 去前缀
来源：http://crn.0kj1m.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kmi.zdbjq.cn

[R26] 命令替换
来源：http://hsn.aibaodan.cn

now=$(date +%F); echo "$now"
来源：http://gdl.shzxlz.cn

[R27] 算术展开
来源：http://rtn.shuidangran.top

echo $((1 + 2 * 3))
来源：http://gvd.bjfxy.top

[R28] 浮点运算
来源：http://jvz.ydjk.org.cn

echo "scale=2; 10/3" | bc
来源：http://ijk.bjfxy.top

[R29] 定义函数
来源：http://mvc.ydzc1.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pvj.jlsjyb.cn

[R30] 函数返回状态码
来源：http://aou.jiagoushi.top

f() { return 0; }; f || echo "失败了"
来源：http://ppc.hongshengwenyu.top

[R31] 局部变量
来源：http://vuu.hywenlv.cn

f() { local x=1; echo "$x"; }
来源：http://uxu.svipenyu.cn

[R32] 参数个数校验
来源：http://ykm.yfazqb.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xvf.yfazqb.com

[R33] 捕获错误并提示行号
来源：http://urn.zhiwuduotai.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lbt.jyoumei.cn

[R34] 退出时清理
来源：http://dke.birdmap.top

trap 'rm -f "$tmp"' EXIT
来源：http://nrk.zdbjq.cn

[R35] 后台执行并等待
来源：http://oso.tian-w.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fvq.sjlbkw.cn

[R36] 并发执行多个任务
来源：http://rsj.jqgufenzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vaj.shuidangran.top

[R37] 把输出赋给变量
来源：http://qjj.shangyingyoupin.top

files=$(ls -1)
来源：http://mkx.svipenyu.cn

[R38] 管道串联
来源：http://hfz.fehbvm.com

cat a.txt | grep -i error | wc -l
来源：http://hyr.chenjidiqi.icu

[R39] 重定向标准输出与错误
来源：http://lmc.bjfxy.top

cmd > out.log 2>&1
来源：http://eba.aibaodan.cn

[R40] 追加写日志
来源：http://hvr.sxryk.cn

echo "log" >> out.log
来源：http://biw.cashguo.top

[R41] 丢弃输出
来源：http://agm.zdbjq.cn

cmd >/dev/null 2>&1
来源：http://rbs.cashguo.top

[R42] 输入重定向
来源：http://kkn.svipenyu.cn

wc -l < a.txt
来源：http://awo.xingfuxueyuan.xyz

[R43] 按名字查找文件
来源：http://wmt.mhx1999.top

find . -name "*.log" -type f
来源：http://nmf.shuidangran.top

[R44] 按修改时间查找
来源：http://eqs.sjlbkw.cn

find . -mtime -7 -type f
来源：http://fxk.daxiang520.top

[R45] 批量删除
来源：http://rll.316326.xyz

find . -name "*.tmp" -delete
来源：http://rrx.ydjk.org.cn

[R46] 递归替换文件内容
来源：http://qol.gotoacloud.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qkw.sweek.top

[R47] sed 单行替换
来源：http://cqp.hcnkem.com

sed -i 's/foo/bar/g' a.txt
来源：http://lsj.shanyushiyangkeji.top

[R48] awk 取指定列
来源：http://ide.52xcode.cn

awk '{print $1, $3}' a.txt
来源：http://qgf.hammf.cn

[R49] awk 带条件
来源：http://rgn.pengpengdd.cyou

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nnp.cucudq.cn

[R50] awk 求和
来源：http://vsm.jinghuilouyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rgk.yj20258.top

[R51] 排序去重取前几
来源：http://lon.jqgfzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://prf.shangyingyoupin.top

[R52] 统计行数
来源：http://lrq.jinghuilouyu.cn

wc -l a.txt
来源：http://vru.ydzc1.top

[R53] 查看文件头与实时尾
来源：http://ies.hongshengwenyu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nqf.yj20258888.top

[R54] 比较两个文件
来源：http://usi.ydzc1.top

diff a.txt b.txt
来源：http://fpx.yvedp.cn

[R55] 压缩与解压
来源：http://sku.ydjk.org.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zot.yj202588.top

[R56] 远程拷贝
来源：http://bfm.gzhubu.top

scp file user@host:/path/
来源：http://omj.ywan-chungtsiang.top

[R57] 远程执行命令
来源：http://ojk.cashguo.top

ssh user@host 'uptime'
来源：http://wgz.ctjpmb.com

[R58] 下载文件
来源：http://ten.bjfxy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://iwt.nanxuanxn.top

[R59] 发 POST JSON
来源：http://ujo.smart0.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gou.yj202588.top

[R60] 只看 HTTP 状态码
来源：http://xbi.yj20258.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://swg.cheryme.top

[R61] 磁盘占用
来源：http://anz.jlsjyb.cn

df -h;  du -sh *
来源：http://gyk.c1oappe.top

[R62] 找最占空间的文件
来源：http://qqx.zdqjudy.top

du -ah . | sort -rh | head -10
来源：http://agc.bbcook.cn

[R63] 内存与进程
来源：http://aws.epnwcf.com

free -h;  ps aux | grep nginx
来源：http://vbt.zdqjudy.top

[R64] 结束进程
来源：http://gtm.wangshuangyany.cn

kill -9 $(pgrep -f app.py)
来源：http://lxk.gaohongyu789.top

[R65] 查看端口占用
来源：http://rct.fengsongda.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qnb.xuetiantiany.cn

[R66] 定时任务
来源：http://amt.shzxlz.cn

crontab -e;  crontab -l
来源：http://gjj.gotoacloud.top

[R67] 生成随机十六进制串
来源：http://vli.ydzc1.top

openssl rand -hex 16
来源：http://bni.sjlbkw.cn

[R68] 计算文件校验值
来源：http://fpq.redwolf501.top

sha256sum a.txt;  md5sum a.txt
来源：http://oty.iojbl.cn

[R69] 生成随机密码
来源：http://aez.zhengqikj.top

head -c 16 /dev/urandom | base64
来源：http://jef.cqqwz.cn

[R70] 时间戳与互转
来源：http://iyr.iojbl.cn

date +%s;  date -d @1700000000
来源：http://mbi.sxryk.cn

[R71] 日期格式化
来源：http://aqx.xylfe.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dsa.fzhhl.top

[R72] 等待端口就绪
来源：http://imu.fzhhl.top

until nc -z localhost 3306; do sleep 1; done
来源：http://pms.jinqigufen.top

[R73] 分割大日志
来源：http://dqd.vehdjk.com

split -l 1000 big.log part_
来源：http://vrg.andypj.xyz

[R74] 批量重命名
来源：http://daz.dianchejie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ogn.xinyue.icu

[R75] 导出环境变量
来源：http://fvt.sysykeji.top

export PATH="$HOME/bin:$PATH"
来源：http://nmj.gzhubu.top

[R76] 使用临时文件
来源：http://fzl.tianlin.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dme.ybcxt.top

[R77] 读取用户输入
来源：http://rzc.yvedp.cn

read -rp "请输入: " ans
来源：http://dks.pengpengdd.cyou

[R78] 交互式菜单
来源：http://hyy.ivvv.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vvz.birdmap.top

[R79] 解析命令行选项
来源：http://wwc.sysykeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nej.yuxming.cn

[R80] 查看脚本执行耗时
来源：http://sbv.andypj.xyz

time ./run.sh
来源：http://cug.jqgufenzy.top

================================================================================
来源：http://ruc.shuidangran.top

S. C / C++ 专题
来源：http://twf.zhixingplan.top

================================================================================
来源：http://gum.xylfe.cn

[S01] C：Hello World
来源：http://iji.haohaochexian.top

#include <stdio.h>
来源：http://okv.hammf.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gmf.dashuyun.cn

[S02] C：变量与格式化输出
来源：http://mdq.epnwcf.com

int a = 10; printf("%d\n", a);
来源：http://ame.nanxinkj.top

[S03] C：读入整数
来源：http://uks.52xcode.cn

int x; scanf("%d", &x);
来源：http://xrt.yueranfly.top

[S04] C：字符串复制
来源：http://rlr.hesvh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zcz.tian-w.cn

[S05] C：字符串长度
来源：http://whw.guowangkeji.top

strlen(s)
来源：http://vcq.xingfuxueyuan.xyz

[S06] C：字符串比较
来源：http://abz.jinyuanbaomall.cn

strcmp(a, b) == 0
来源：http://bba.chenzaomai.com

[S07] C：数组遍历求和
来源：http://xyi.hnqzz.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fwm.mhx1999.top

[S08] C：动态内存分配与释放
来源：http://wrp.feifeiyinyue.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ssu.hnxiangtu.top

[S09] C：结构体定义与初始化
来源：http://iih.jianghu66.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://toc.zycfv.cn

[S10] C：指针与解引用
来源：http://dwb.smart0.xyz

int *p = &a;  *p = 5;
来源：http://tii.shzxlz.cn

[S11] C：逐行读文件
来源：http://wxm.jiagoushi.top

FILE *f = fopen("a.txt", "r");
来源：http://zhg.zdbjq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pnb.sxryk.cn

fclose(f);
来源：http://yyk.hfpthk.cn

[S12] C：写文件
来源：http://fnd.fengsongda.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://iux.hnxiangtu.top

[S13] C：宏定义
来源：http://hms.jqgfzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qdq.zhijiandao.cn

[S14] C：枚举
来源：http://fmu.ywan-chungtsiang.top

enum Color { RED, GREEN, BLUE };
来源：http://mrt.tanke756.top

[S15] C：类型转换
来源：http://fsa.gaohongyu789.top

(double) a / b
来源：http://rqr.hnxiangtu.top

[S16] C：位操作置位
来源：http://llz.cqqwz.cn

x |= (1 << 3);
来源：http://pwz.fengsongda.top

[S17] C：安全拼接字符串
来源：http://int.gogol.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sjk.sysykeji.top

[S18] C：命令行参数
来源：http://acs.jianghu66.top

int main(int argc, char **argv)
来源：http://nwt.jinyuanbaomall.cn

[S19] C：快速排序
来源：http://rki.shzxlz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yrx.jinghuilouyu.cn

[S20] C：二分查找
来源：http://yjf.xziqi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pdj.zhixingplan.top

[S21] C：字符类别判断
来源：http://fqn.guannengcc.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://won.yvedp.cn

[S22] C：字符串转数字
来源：http://ged.zdqjudy.top

atoi("42");  strtod("3.14", NULL);
来源：http://psm.yonumen.top

[S23] C：随机数
来源：http://qll.sjlbkw.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mmu.sxryk.cn

[S24] C：获取本地时间
来源：http://gew.fzhhl.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://faq.zhijiandao.cn

[S25] C：内存拷贝
来源：http://ljm.jlsjyb.cn

memcpy(dst, src, n);
来源：http://nug.wangshuangyany.cn

[S26] C：内存清零
来源：http://zij.dianchejie.cn

memset(a, 0, sizeof a);
来源：http://qka.gotoacloud.top

[S27] C：定义常量
来源：http://qeq.jinyuanbaomall.cn

const double PI = 3.14159;
来源：http://jym.52xcode.cn

[S28] C：静态变量
来源：http://ocw.zhaomingkeji.xyz

static int counter = 0;
来源：http://yzt.gaohongyu789.top

[S29] C：变参函数
来源：http://zfc.ywan-chungtsiang.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://drj.aizwys.cn

[S30] C：头文件保护
来源：http://mtj.ctjpmb.com

#ifndef X_H
来源：http://wnb.hnqzz.top

#define X_H
来源：http://ubd.52xcode.cn

#endif
来源：http://lmr.xuetiantiany.cn

[S31] C++：Hello World
来源：http://spw.tianlin.xyz

#include <iostream>
来源：http://kkm.hywenlv.cn

int main() { std::cout << "Hello\n"; }
来源：http://isb.redwolf501.top

[S32] C++：字符串
来源：http://bhh.hammf.cn

std::string s = "hi";  s += "!";
来源：http://xjn.tian-w.cn

[S33] C++：vector 增删
来源：http://vkl.guowangkeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ycd.shanyushiyangtech.top

[S34] C++：遍历 vector
来源：http://spt.wangdashe.top

for (auto &x : v) { std::cout << x; }
来源：http://bmr.yueranfly.top

[S35] C++：map
来源：http://juv.jianghu66.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pzr.ehwqpu.com

[S36] C++：unordered_map
来源：http://cqa.sysykeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sjp.cucudq.cn

[S37] C++：set
来源：http://ptn.andypj.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wcv.sjlbkw.cn

[S38] C++：排序
来源：http://clv.shangyingyoupin.top

std::sort(v.begin(), v.end());
来源：http://vgp.xingfuxueyuan.xyz

[S39] C++：自定义比较器排序
来源：http://lzs.daxiang520.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gcc.vehdjk.com

[S40] C++：查找元素
来源：http://scz.ppjwa.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gkt.tarul.cn

[S41] C++：类与构造函数
来源：http://ghu.cucudq.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ira.yvedp.cn

[S42] C++：继承与虚函数
来源：http://axl.chenlongwang.top

class B : public Base { public: void f() override {} };
来源：http://flo.zycfv.cn

[S43] C++：智能指针
来源：http://pai.dianchejie.cn

auto p = std::make_unique<int>(5);
来源：http://qmu.nanxuanxn.top

[S44] C++：引用传参
来源：http://jee.yanxiufei.cn

void inc(int &x) { ++x; }
来源：http://lxp.shzxlz.cn

[S45] C++：lambda
来源：http://qyb.smart0.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://mmi.kuanghao11.cn

[S46] C++：函数模板
来源：http://lac.zhongyouzk.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gtg.hnqzz.top

[S47] C++：结构化绑定遍历
来源：http://yve.jinyuanbaomall.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://trn.hammf.cn

[S48] C++：逐行读文件
来源：http://cut.aibaodan.cn

std::ifstream in("a.txt");  std::string line;
来源：http://otl.jianghu66.top

while (std::getline(in, line)) { }
来源：http://aou.nwbrower.top

[S49] C++：写文件
来源：http://keh.hongshengwenyu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xai.hcnkem.com

[S50] C++：格式化数字
来源：http://uld.cdnleiting.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gfh.fanxiaobao.xyz

[S51] C++：显式类型转换
来源：http://aqu.c1oappe.top

static_cast<double>(a) / b
来源：http://cjn.cdnleiting.top

[S52] C++：const 与 noexcept
来源：http://pak.jinqigfzy.top

int size() const noexcept { return n_; }
来源：http://fzy.pengpengdd.cyou

[S53] C++：移动语义
来源：http://ftv.hnqzz.top

std::vector<int> w = std::move(v);
来源：http://pwj.chenzaomai.com

[S54] C++：异常处理
来源：http://obq.gogol.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://owj.hnqzz.top

[S55] C++：结构化绑定
来源：http://tnf.andypj.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://rpc.fehbvm.com

[S56] C++：optional
来源：http://kzl.hesvh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wbc.dianchejie.cn

[S57] C++：编译期常量
来源：http://yui.jianghu66.top

constexpr int N = 10;
来源：http://wno.sysykeji.top

[S58] C++：命名空间
来源：http://dfv.svipenyu.cn


<!-- 参考信息 -->