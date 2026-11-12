代发 wailian999

[Q84] 去除首尾空格
来源：http://ini.pycfn.com

SELECT TRIM(name) FROM users;
来源：http://ais.sxryk.cn

[Q85] 数值取整
来源：http://zkk.dashuyun.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jbx.zhixingplan.top

[Q86] 读取 JSON 字段
来源：http://ufc.bbcook.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zkv.smart0.xyz

[Q87] JSON 字段做条件
来源：http://vrw.yuxming.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://loo.guowangkeji.top

[Q88] 行转列（条件聚合）
来源：http://qou.ehwqpu.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jkj.316326.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pez.tarul.cn

[Q89] 判断表是否存在
来源：http://bes.gaohongyu789.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oiu.sufxvd.cn

[Q90] 生成序号列
来源：http://opo.gzhubu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xsn.52xcode.cn

================================================================================
来源：http://vyg.jqgufenzy.top

R. Bash 专题
来源：http://fau.ppjwa.cn

================================================================================
来源：http://nxv.shanyushiyangkeji.top

[R01] shebang 与严格模式
来源：http://fmw.pycfn.com

#!/usr/bin/env bash
来源：http://xuc.jinghuilouyu.cn

set -euo pipefail
来源：http://vbo.zhengqikj.top

[R02] 变量赋值与使用
来源：http://qbl.ppjwa.cn

name="Tom"; echo "$name"
来源：http://xro.0kj1m.cn

[R03] 只读变量
来源：http://gfr.zdbjq.cn

readonly PI=3.14
来源：http://ldn.hcnkem.com

[R04] 位置参数
来源：http://pna.zycfv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ppx.jinqigufen.top

[R05] 参数默认值
来源：http://nfh.fehbvm.com

name="${1:-default}"
来源：http://dob.hcnkem.com

[R06] 判断命令是否存在
来源：http://cfh.yangfankeji.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jhn.chenzaomai.com

[R07] if 判断文件
来源：http://iuq.nanxuanxn.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uhy.sjlbkw.cn

[R08] 数值比较
来源：http://jhf.jlsjyb.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://cnm.zhengqikj.top

[R09] 字符串比较
来源：http://kmh.nanxuanxn.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uhz.yangfankeji.com

[R10] 正则匹配
来源：http://gjd.yfazqb.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://iwu.snrcjt.cn

[R11] case 多分支
来源：http://wuf.cdnleiting.top

case "$1" in
来源：http://tnv.zhoulong.xyz

start) echo "启动" ;;
来源：http://uvr.yanxiufei.cn

stop)  echo "停止" ;;
来源：http://lxd.jinghuilouyu.cn

*)     echo "未知命令" ;;
来源：http://mdj.meibo888.top

esac
来源：http://djp.yueranfly.top

[R12] for 遍历文件
来源：http://imb.hammf.cn

for f in *.txt; do echo "$f"; done
来源：http://crd.ydzc1.top

[R13] for 计数循环
来源：http://ndi.shanyushiyangkeji.top

for i in {1..10}; do echo "$i"; done
来源：http://uib.ppjwa.cn

[R14] C 风格 for
来源：http://xci.ppjwa.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yth.yangfankeji.com

[R15] while 逐行读文件
来源：http://cgc.ydjk.org.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zpj.wangshuangyany.cn

[R16] until 等待条件
来源：http://wkg.cheryme.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wjn.tianlin.xyz

[R17] 数组定义与取值
来源：http://laj.mhx1999.top

arr=(a b c); echo "${arr[0]}"
来源：http://lbm.jqgfzy.top

[R18] 遍历数组
来源：http://vrq.gzhubu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://git.9152youxi.cn

[R19] 数组长度
来源：http://lff.9152youxi.cn

echo "${#arr[@]}"
来源：http://nlf.0kj1m.cn

[R20] 关联数组（字典）
来源：http://cgc.xuanzx.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ara.cheryme.top

[R21] 字符串长度
来源：http://wij.cheryme.top

echo "${#s}"
来源：http://vmc.cashguo.top

[R22] 截取子串
来源：http://phq.yj20258.top

echo "${s:0:5}"
来源：http://rfc.ppjwa.cn

[R23] 字符串替换
来源：http://rch.fengsongda.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://guz.haohaochexian.top

[R24] 大小写转换
来源：http://ywd.c1oappe.top

echo "${s^^}"; echo "${s,,}"
来源：http://anb.fengsongda.top

[R25] 去后缀 / 去前缀
来源：http://qjt.hfpthk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kit.fanxiaobao.xyz

[R26] 命令替换
来源：http://gyj.xinyue.icu

now=$(date +%F); echo "$now"
来源：http://bip.zhaomingkeji.xyz

[R27] 算术展开
来源：http://ehb.birdmap.top

echo $((1 + 2 * 3))
来源：http://fhh.jinqigufen.top

[R28] 浮点运算
来源：http://mno.hysaishi.cn

echo "scale=2; 10/3" | bc
来源：http://ohl.ppjwa.cn

[R29] 定义函数
来源：http://tsk.sxryk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://iae.chenlongwang.top

[R30] 函数返回状态码
来源：http://gor.iojbl.cn

f() { return 0; }; f || echo "失败了"
来源：http://lub.shzxlz.cn

[R31] 局部变量
来源：http://dke.fengsongda.top

f() { local x=1; echo "$x"; }
来源：http://cdh.meibo888.top

[R32] 参数个数校验
来源：http://vve.nanxinkj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://voo.hcnkem.com

[R33] 捕获错误并提示行号
来源：http://pgx.fanxiaobao.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fst.dashuyun.cn

[R34] 退出时清理
来源：http://row.zycfv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bks.fktsv.cn

[R35] 后台执行并等待
来源：http://qyv.fzhhl.top

sleep 5 & pid=$!; wait "$pid"
来源：http://kat.cucudq.cn

[R36] 并发执行多个任务
来源：http://dnr.tanke756.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uqr.shzxlz.cn

[R37] 把输出赋给变量
来源：http://inw.zhixingplan.top

files=$(ls -1)
来源：http://obu.uphjek.com

[R38] 管道串联
来源：http://bcq.yueranfly.top

cat a.txt | grep -i error | wc -l
来源：http://wut.aibaodan.cn

[R39] 重定向标准输出与错误
来源：http://doq.yfazqb.com

cmd > out.log 2>&1
来源：http://kdz.316326.xyz

[R40] 追加写日志
来源：http://ttd.vehdjk.com

echo "log" >> out.log
来源：http://pls.dianchejie.cn

[R41] 丢弃输出
来源：http://str.pengpengdd.cyou

cmd >/dev/null 2>&1
来源：http://icu.mhx1999.top

[R42] 输入重定向
来源：http://ols.sufxvd.cn

wc -l < a.txt
来源：http://xfo.shangyingyoupin.top

[R43] 按名字查找文件
来源：http://agb.9152youxi.cn

find . -name "*.log" -type f
来源：http://kmm.dianchejie.cn

[R44] 按修改时间查找
来源：http://div.hesvh.cn

find . -mtime -7 -type f
来源：http://cwn.shzxlz.cn

[R45] 批量删除
来源：http://qen.jinqigufen.top

find . -name "*.tmp" -delete
来源：http://cwh.chenzaomai.com

[R46] 递归替换文件内容
来源：http://skk.zdbjq.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://spu.fanxiaobao.xyz

[R47] sed 单行替换
来源：http://xic.birdmap.top

sed -i 's/foo/bar/g' a.txt
来源：http://bzt.chenjidiqi.icu

[R48] awk 取指定列
来源：http://zpj.sysykeji.top

awk '{print $1, $3}' a.txt
来源：http://hzt.yonumen.top

[R49] awk 带条件
来源：http://hkp.xylfe.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://neg.hnqzz.top

[R50] awk 求和
来源：http://doz.ehwqpu.com

awk '{s += $2} END {print s}' a.txt
来源：http://vcy.zhoulong.xyz

[R51] 排序去重取前几
来源：http://pnl.0kj1m.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://poa.jlsjyb.cn

[R52] 统计行数
来源：http://utl.sufxvd.cn

wc -l a.txt
来源：http://bzg.tanke756.top

[R53] 查看文件头与实时尾
来源：http://lcg.xuanzx.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://exw.ehwqpu.com

[R54] 比较两个文件
来源：http://dpr.vehdjk.com

diff a.txt b.txt
来源：http://dsk.zdqjudy.top

[R55] 压缩与解压
来源：http://jjj.xziqi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://plf.zhixingplan.top

[R56] 远程拷贝
来源：http://mvq.jyoumei.cn

scp file user@host:/path/
来源：http://avm.zdbjq.cn

[R57] 远程执行命令
来源：http://kcv.yuanzhike.top

ssh user@host 'uptime'
来源：http://rfc.cheryme.top

[R58] 下载文件
来源：http://nof.316326.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bhs.wangdashe.top

[R59] 发 POST JSON
来源：http://fqa.chenlongwang.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://buk.zhijiandao.cn

[R60] 只看 HTTP 状态码
来源：http://het.hfpthk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fjc.cqqwz.cn

[R61] 磁盘占用
来源：http://vki.yangfankeji.com

df -h;  du -sh *
来源：http://qaa.vqdsnc.cn

[R62] 找最占空间的文件
来源：http://ifl.zdbjq.cn

du -ah . | sort -rh | head -10
来源：http://jzd.daxiang520.top

[R63] 内存与进程
来源：http://esg.vqdsnc.cn

free -h;  ps aux | grep nginx
来源：http://jyc.jlsjyb.cn

[R64] 结束进程
来源：http://yuw.tarul.cn

kill -9 $(pgrep -f app.py)
来源：http://jvu.svipenyu.cn

[R65] 查看端口占用
来源：http://gdr.hcnkem.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rlc.gzhubu.top

[R66] 定时任务
来源：http://ltl.jyoumei.cn

crontab -e;  crontab -l
来源：http://qcc.meibo888.top

[R67] 生成随机十六进制串
来源：http://ukw.hcnkem.com

openssl rand -hex 16
来源：http://tvx.cdnleiting.top

[R68] 计算文件校验值
来源：http://xjk.hongshengwenyu.top

sha256sum a.txt;  md5sum a.txt
来源：http://tqx.xylfe.cn

[R69] 生成随机密码
来源：http://sbu.cdnleiting.top

head -c 16 /dev/urandom | base64
来源：http://sae.fengsongda.top

[R70] 时间戳与互转
来源：http://apl.hesvh.cn

date +%s;  date -d @1700000000
来源：http://cdo.sufxvd.cn

[R71] 日期格式化
来源：http://czx.hammf.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://peu.epnwcf.com

[R72] 等待端口就绪
来源：http://gqj.hammf.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wnl.zhongyouzk.top

[R73] 分割大日志
来源：http://wpc.ydjk.org.cn

split -l 1000 big.log part_
来源：http://vag.dianchejie.cn

[R74] 批量重命名
来源：http://zvj.guannengcc.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vzn.ywan-chungtsiang.top

[R75] 导出环境变量
来源：http://ruw.sjlbkw.cn

export PATH="$HOME/bin:$PATH"
来源：http://qun.sysykeji.top

[R76] 使用临时文件
来源：http://mph.meibo888.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jal.aizwys.cn

[R77] 读取用户输入
来源：http://uyr.kuanghao11.cn

read -rp "请输入: " ans
来源：http://vnd.shuidangran.top

[R78] 交互式菜单
来源：http://psx.hesvh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ajf.yj202588.top

[R79] 解析命令行选项
来源：http://pgw.ywan-chungtsiang.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jyf.zhixingplan.top

[R80] 查看脚本执行耗时
来源：http://pbg.cdnleiting.top

time ./run.sh
来源：http://qwh.wangdashe.top

================================================================================
来源：http://oba.hysaishi.cn

S. C / C++ 专题
来源：http://lbt.zdqjudy.top

================================================================================
来源：http://wlf.jinyuanbaomall.cn

[S01] C：Hello World
来源：http://gem.xuetiantiany.cn

#include <stdio.h>
来源：http://mdk.hongshengwenyu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wwm.ybcxt.top

[S02] C：变量与格式化输出
来源：http://kss.daxiang520.top

int a = 10; printf("%d\n", a);
来源：http://utb.sjlbkw.cn

[S03] C：读入整数
来源：http://nbq.sufxvd.cn

int x; scanf("%d", &x);
来源：http://rfe.yj202588.top

[S04] C：字符串复制
来源：http://coq.ctjpmb.com

char dst[32]; strcpy(dst, "hi");
来源：http://ngb.smart0.xyz

[S05] C：字符串长度
来源：http://aeu.ydzc1.top

strlen(s)
来源：http://brw.hfpthk.cn

[S06] C：字符串比较
来源：http://nzf.hysaishi.cn

strcmp(a, b) == 0
来源：http://rvy.9152youxi.cn

[S07] C：数组遍历求和
来源：http://ftc.zdqjudy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xht.zdbjq.cn

[S08] C：动态内存分配与释放
来源：http://ehs.jqgufenzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://osc.yueranfly.top

[S09] C：结构体定义与初始化
来源：http://rzo.shzxlz.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://agl.wangdashe.top

[S10] C：指针与解引用
来源：http://ygs.yuxming.cn

int *p = &a;  *p = 5;
来源：http://bag.snrcjt.cn

[S11] C：逐行读文件
来源：http://beq.yangfankeji.com

FILE *f = fopen("a.txt", "r");
来源：http://yyx.jinqigufen.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://rof.chenlongwang.top

fclose(f);
来源：http://qil.fzhhl.top

[S12] C：写文件
来源：http://ygi.sjlbkw.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cij.yj20258888.top

[S13] C：宏定义
来源：http://ahe.cdnleiting.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jnx.yuanzhike.top

[S14] C：枚举
来源：http://uxt.yj20258888.top

enum Color { RED, GREEN, BLUE };
来源：http://jvp.zycfv.cn

[S15] C：类型转换
来源：http://doo.snrcjt.cn

(double) a / b
来源：http://jfq.mhx1999.top

[S16] C：位操作置位
来源：http://asz.jlsjyb.cn

x |= (1 << 3);
来源：http://giw.chenlongwang.top

[S17] C：安全拼接字符串
来源：http://raf.daria6918.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://drb.daxiang520.top

[S18] C：命令行参数
来源：http://qde.yuanzhike.top

int main(int argc, char **argv)
来源：http://ndz.chenlongwang.top

[S19] C：快速排序
来源：http://jpd.havefunace.top

qsort(a, n, sizeof(int), cmp);
来源：http://dae.nwbrower.top

[S20] C：二分查找
来源：http://eia.jinqigufen.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mfg.daria6918.cn

[S21] C：字符类别判断
来源：http://hur.ybcxt.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gue.9152youxi.cn

[S22] C：字符串转数字
来源：http://utx.gaohongyu789.top

atoi("42");  strtod("3.14", NULL);
来源：http://bso.shanyushiyangkeji.top

[S23] C：随机数
来源：http://xek.iojbl.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://znp.jiagoushi.top

[S24] C：获取本地时间
来源：http://tfw.tanke756.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qfg.jqgufenzy.top

[S25] C：内存拷贝
来源：http://ozn.daria6918.cn

memcpy(dst, src, n);
来源：http://rzq.bjfxy.top

[S26] C：内存清零
来源：http://hub.nanxinkj.top

memset(a, 0, sizeof a);
来源：http://gtt.c1oappe.top

[S27] C：定义常量
来源：http://roe.c1oappe.top

const double PI = 3.14159;
来源：http://asm.guannengcc.top

[S28] C：静态变量
来源：http://wkb.fengsongda.top

static int counter = 0;
来源：http://jvu.bjfxy.top

[S29] C：变参函数
来源：http://dzv.birdmap.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cwc.sxryk.cn

[S30] C：头文件保护
来源：http://eiu.shzxlz.cn

#ifndef X_H
来源：http://sgm.zhijiandao.cn

#define X_H
来源：http://aiy.hfpthk.cn

#endif
来源：http://ngu.ydjk.org.cn

[S31] C++：Hello World
来源：http://ipf.vehdjk.com

#include <iostream>
来源：http://gvq.kuanghao11.cn

int main() { std::cout << "Hello\n"; }
来源：http://tza.hcnkem.com

[S32] C++：字符串
来源：http://akh.tianlin.xyz

std::string s = "hi";  s += "!";
来源：http://kqd.ehwqpu.com

[S33] C++：vector 增删
来源：http://kcd.yangfankeji.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pav.yonumen.top

[S34] C++：遍历 vector
来源：http://jue.nanxuanxn.top

for (auto &x : v) { std::cout << x; }
来源：http://zno.chenlongwang.top

[S35] C++：map
来源：http://kuv.316326.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yma.hywenlv.cn

[S36] C++：unordered_map
来源：http://dwm.guannengcc.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iks.shanyushiyangtech.top

[S37] C++：set
来源：http://uon.yj20258888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jqf.yueranfly.top

[S38] C++：排序
来源：http://mbg.zhongyouzk.top

std::sort(v.begin(), v.end());
来源：http://cqr.jianghu66.top

[S39] C++：自定义比较器排序
来源：http://jpr.zhengqikj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pri.shangyingyoupin.top

[S40] C++：查找元素
来源：http://vbh.svipenyu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fwp.nanxuanxn.top

[S41] C++：类与构造函数
来源：http://bvi.ivvv.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://biw.shanyushiyangkeji.top

[S42] C++：继承与虚函数
来源：http://qhr.cqqwz.cn

class B : public Base { public: void f() override {} };
来源：http://wjo.zhijiandao.cn

[S43] C++：智能指针
来源：http://vno.gzhubu.top

auto p = std::make_unique<int>(5);
来源：http://ulm.feifeiyinyue.top

[S44] C++：引用传参
来源：http://lod.pengpengdd.cyou

void inc(int &x) { ++x; }
来源：http://cyd.tanke756.top

[S45] C++：lambda
来源：http://vqh.wangshuangyany.cn

auto add = [](int a, int b) { return a + b; };
来源：http://iei.dashuyun.cn

[S46] C++：函数模板
来源：http://hhy.9152youxi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dvr.jinqigfzy.top

[S47] C++：结构化绑定遍历
来源：http://xcg.chenjidiqi.icu

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tuw.chenzaomai.com

[S48] C++：逐行读文件
来源：http://ywt.jinqigufen.top

std::ifstream in("a.txt");  std::string line;
来源：http://ben.uphjek.com

while (std::getline(in, line)) { }
来源：http://fri.vqdsnc.cn

[S49] C++：写文件
来源：http://beg.yangfankeji.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vlk.0kj1m.cn

[S50] C++：格式化数字
来源：http://wai.hfpthk.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://suj.xuetiantiany.cn

[S51] C++：显式类型转换
来源：http://xqy.sjlbkw.cn

static_cast<double>(a) / b
来源：http://oci.hnxiangtu.top

[S52] C++：const 与 noexcept
来源：http://ltj.shanyushiyangtech.top

int size() const noexcept { return n_; }
来源：http://wck.nanxinkj.top

[S53] C++：移动语义
来源：http://uce.tarul.cn

std::vector<int> w = std::move(v);
来源：http://yap.chenjidiqi.icu

[S54] C++：异常处理
来源：http://ssm.svipenyu.cn


<!-- 参考信息 -->