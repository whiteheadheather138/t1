代发 wailian999

[Q86] 读取 JSON 字段
来源：http://lra.jiagoushi.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pte.svipenyu.cn

[Q87] JSON 字段做条件
来源：http://fjz.zdbjq.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bcf.smart0.xyz

[Q88] 行转列（条件聚合）
来源：http://nqj.hysaishi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xfq.feifeiyinyue.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vql.hesvh.cn

[Q89] 判断表是否存在
来源：http://dat.yongpay.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://khe.sysykeji.top

[Q90] 生成序号列
来源：http://oew.wangdashe.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jnt.jinqigfzy.top

================================================================================
来源：http://ixd.wangdashe.top

R. Bash 专题
来源：http://rzy.aibaodan.cn

================================================================================
来源：http://egw.jqgufenzy.top

[R01] shebang 与严格模式
来源：http://xjb.chenjidiqi.icu

#!/usr/bin/env bash
来源：http://edj.nwbrower.top

set -euo pipefail
来源：http://kfs.hywenlv.cn

[R02] 变量赋值与使用
来源：http://ncz.kuanghao11.cn

name="Tom"; echo "$name"
来源：http://wjt.sjlbkw.cn

[R03] 只读变量
来源：http://wcl.dianchejie.cn

readonly PI=3.14
来源：http://nhh.daxiang520.top

[R04] 位置参数
来源：http://fuo.chenlongwang.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xtp.nanxinkj.top

[R05] 参数默认值
来源：http://wzp.redwolf501.top

name="${1:-default}"
来源：http://mzv.yvedp.cn

[R06] 判断命令是否存在
来源：http://arx.52xcode.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bus.jinyuanbaomall.cn

[R07] if 判断文件
来源：http://gwq.jinqigufen.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dhm.zhongyouzk.top

[R08] 数值比较
来源：http://yri.cdnleiting.top

if (( a > b )); then echo "a 更大"; fi
来源：http://qys.mhx1999.top

[R09] 字符串比较
来源：http://ccm.hongshengwenyu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pgf.tarul.cn

[R10] 正则匹配
来源：http://ckc.jqgufenzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tti.cdnleiting.top

[R11] case 多分支
来源：http://wqg.pycfn.com

case "$1" in
来源：http://fqj.zdbjq.cn

start) echo "启动" ;;
来源：http://oks.smart0.xyz

stop)  echo "停止" ;;
来源：http://twd.daria6918.cn

*)     echo "未知命令" ;;
来源：http://jjx.bbcook.cn

esac
来源：http://udv.cucudq.cn

[R12] for 遍历文件
来源：http://ejo.shzxlz.cn

for f in *.txt; do echo "$f"; done
来源：http://kjx.zycfv.cn

[R13] for 计数循环
来源：http://mip.aizwys.cn

for i in {1..10}; do echo "$i"; done
来源：http://ach.52xcode.cn

[R14] C 风格 for
来源：http://gxh.xinyue.icu

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sqm.xinyue.icu

[R15] while 逐行读文件
来源：http://gms.birdmap.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rcg.tianlin.xyz

[R16] until 等待条件
来源：http://oty.jqgfzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tho.jqgufenzy.top

[R17] 数组定义与取值
来源：http://kdv.sysykeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://ury.bjfxy.top

[R18] 遍历数组
来源：http://vvc.shzxlz.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vtt.tanke756.top

[R19] 数组长度
来源：http://jik.shanyushiyangkeji.top

echo "${#arr[@]}"
来源：http://zbt.xylfe.cn

[R20] 关联数组（字典）
来源：http://ove.shuidangran.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ilq.chenlongwang.top

[R21] 字符串长度
来源：http://bna.dashuyun.cn

echo "${#s}"
来源：http://mkr.jqgfzy.top

[R22] 截取子串
来源：http://thy.tarul.cn

echo "${s:0:5}"
来源：http://uag.pycfn.com

[R23] 字符串替换
来源：http://pvu.snrcjt.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://scp.xuanzx.com

[R24] 大小写转换
来源：http://dej.fanxiaobao.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://nno.quarkkingdee.top

[R25] 去后缀 / 去前缀
来源：http://woj.52xcode.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://naa.yanxiufei.cn

[R26] 命令替换
来源：http://xgb.zhoulong.xyz

now=$(date +%F); echo "$now"
来源：http://utr.iojbl.cn

[R27] 算术展开
来源：http://akm.bjfxy.top

echo $((1 + 2 * 3))
来源：http://xpq.epnwcf.com

[R28] 浮点运算
来源：http://fnd.dianchejie.cn

echo "scale=2; 10/3" | bc
来源：http://thp.hfpthk.cn

[R29] 定义函数
来源：http://jmt.jinqigfzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bua.hesvh.cn

[R30] 函数返回状态码
来源：http://dmu.yj202588.top

f() { return 0; }; f || echo "失败了"
来源：http://xox.haohaochexian.top

[R31] 局部变量
来源：http://zoa.9152youxi.cn

f() { local x=1; echo "$x"; }
来源：http://qjf.guowangkeji.top

[R32] 参数个数校验
来源：http://ept.chenzaomai.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://evw.yuxming.cn

[R33] 捕获错误并提示行号
来源：http://pua.ydzc1.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bni.yvedp.cn

[R34] 退出时清理
来源：http://yec.jinghuilouyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mqz.jiagoushi.top

[R35] 后台执行并等待
来源：http://kwf.jyoumei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lja.sysykeji.top

[R36] 并发执行多个任务
来源：http://luh.andypj.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://avo.iojbl.cn

[R37] 把输出赋给变量
来源：http://gmr.yuanzhike.top

files=$(ls -1)
来源：http://wpx.ppjwa.cn

[R38] 管道串联
来源：http://kzw.chenlongwang.top

cat a.txt | grep -i error | wc -l
来源：http://cff.316326.xyz

[R39] 重定向标准输出与错误
来源：http://xlq.jlsjyb.cn

cmd > out.log 2>&1
来源：http://iqy.yonumen.top

[R40] 追加写日志
来源：http://pyl.sjlbkw.cn

echo "log" >> out.log
来源：http://uro.jinqigfzy.top

[R41] 丢弃输出
来源：http://ffr.daria6918.cn

cmd >/dev/null 2>&1
来源：http://anc.jinyuanbaomall.cn

[R42] 输入重定向
来源：http://jpu.yangfankeji.com

wc -l < a.txt
来源：http://cde.jlsjyb.cn

[R43] 按名字查找文件
来源：http://bdl.jqgufenzy.top

find . -name "*.log" -type f
来源：http://fuz.bjfxy.top

[R44] 按修改时间查找
来源：http://uai.jinyuanbaomall.cn

find . -mtime -7 -type f
来源：http://tma.birdmap.top

[R45] 批量删除
来源：http://roc.gaohongyu789.top

find . -name "*.tmp" -delete
来源：http://qdk.sufxvd.cn

[R46] 递归替换文件内容
来源：http://anu.aizwys.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bxy.sweek.top

[R47] sed 单行替换
来源：http://pzf.ctjpmb.com

sed -i 's/foo/bar/g' a.txt
来源：http://jsr.yj20258.top

[R48] awk 取指定列
来源：http://hxl.hnxiangtu.top

awk '{print $1, $3}' a.txt
来源：http://hzr.yj20258.top

[R49] awk 带条件
来源：http://ijy.epnwcf.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uuv.redwolf501.top

[R50] awk 求和
来源：http://djc.jiagoushi.top

awk '{s += $2} END {print s}' a.txt
来源：http://tkf.yonumen.top

[R51] 排序去重取前几
来源：http://hqs.jinghuilouyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ctf.guowangkeji.top

[R52] 统计行数
来源：http://aby.epnwcf.com

wc -l a.txt
来源：http://qvp.guannengcc.top

[R53] 查看文件头与实时尾
来源：http://qim.hnxiangtu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jeo.svipenyu.cn

[R54] 比较两个文件
来源：http://xua.jlsjyb.cn

diff a.txt b.txt
来源：http://tey.jinghuilouyu.cn

[R55] 压缩与解压
来源：http://aez.xinyue.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lcq.fehbvm.com

[R56] 远程拷贝
来源：http://zfs.pengpengdd.cyou

scp file user@host:/path/
来源：http://jjd.xuanzx.com

[R57] 远程执行命令
来源：http://puj.cashguo.top

ssh user@host 'uptime'
来源：http://ypv.cheryme.top

[R58] 下载文件
来源：http://gki.zdbjq.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gmf.yueranfly.top

[R59] 发 POST JSON
来源：http://rdg.sysykeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wlh.c1oappe.top

[R60] 只看 HTTP 状态码
来源：http://srf.xingfuxueyuan.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jsm.zhaomingkeji.xyz

[R61] 磁盘占用
来源：http://tjc.shangyingyoupin.top

df -h;  du -sh *
来源：http://kmq.uphjek.com

[R62] 找最占空间的文件
来源：http://lfv.yangfankeji.com

du -ah . | sort -rh | head -10
来源：http://kst.chenzaomai.com

[R63] 内存与进程
来源：http://bkf.0kj1m.cn

free -h;  ps aux | grep nginx
来源：http://sue.yj20258888.top

[R64] 结束进程
来源：http://tnx.tian-w.cn

kill -9 $(pgrep -f app.py)
来源：http://zev.zdbjq.cn

[R65] 查看端口占用
来源：http://atp.epnwcf.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oae.dianchejie.cn

[R66] 定时任务
来源：http://usd.nanxinkj.top

crontab -e;  crontab -l
来源：http://yyj.ppjwa.cn

[R67] 生成随机十六进制串
来源：http://gyi.nanxinkj.top

openssl rand -hex 16
来源：http://lyr.hnqzz.top

[R68] 计算文件校验值
来源：http://avi.jinghuilouyu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://riw.iojbl.cn

[R69] 生成随机密码
来源：http://gyf.tianlin.xyz

head -c 16 /dev/urandom | base64
来源：http://bmh.xuetiantiany.cn

[R70] 时间戳与互转
来源：http://hgp.ydjk.org.cn

date +%s;  date -d @1700000000
来源：http://wou.cheryme.top

[R71] 日期格式化
来源：http://skl.9152youxi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://khw.jinqigufen.top

[R72] 等待端口就绪
来源：http://mjs.xuetiantiany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zdb.wangshuangyany.cn

[R73] 分割大日志
来源：http://uqk.hfpthk.cn

split -l 1000 big.log part_
来源：http://ccu.andypj.xyz

[R74] 批量重命名
来源：http://urf.zhixingplan.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xar.hywenlv.cn

[R75] 导出环境变量
来源：http://gzy.zhixingplan.top

export PATH="$HOME/bin:$PATH"
来源：http://gyn.yangfankeji.com

[R76] 使用临时文件
来源：http://gss.xziqi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dfh.ctjpmb.com

[R77] 读取用户输入
来源：http://tmg.yueranfly.top

read -rp "请输入: " ans
来源：http://ngk.xziqi.cn

[R78] 交互式菜单
来源：http://dot.yueranfly.top

select opt in a b c; do echo "$opt"; break; done
来源：http://omw.ppjwa.cn

[R79] 解析命令行选项
来源：http://dyz.meibo888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mrb.shanyushiyangtech.top

[R80] 查看脚本执行耗时
来源：http://xvy.meibo888.top

time ./run.sh
来源：http://ztm.cdnleiting.top

================================================================================
来源：http://wxb.yuxming.cn

S. C / C++ 专题
来源：http://bew.jqgufenzy.top

================================================================================
来源：http://qkh.hnxiangtu.top

[S01] C：Hello World
来源：http://etg.shzxlz.cn

#include <stdio.h>
来源：http://mag.cdnleiting.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://euo.dashuyun.cn

[S02] C：变量与格式化输出
来源：http://irc.zhiwuduotai.top

int a = 10; printf("%d\n", a);
来源：http://zjs.yueranfly.top

[S03] C：读入整数
来源：http://gde.nwbrower.top

int x; scanf("%d", &x);
来源：http://npt.bjfxy.top

[S04] C：字符串复制
来源：http://syj.tarul.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nue.yanxiufei.cn

[S05] C：字符串长度
来源：http://xlk.ydjk.org.cn

strlen(s)
来源：http://jbl.yueranfly.top

[S06] C：字符串比较
来源：http://avx.iojbl.cn

strcmp(a, b) == 0
来源：http://iju.zhixingplan.top

[S07] C：数组遍历求和
来源：http://wdw.jinghuilouyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bhl.52xcode.cn

[S08] C：动态内存分配与释放
来源：http://vuz.jinghuilouyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zlm.hysaishi.cn

[S09] C：结构体定义与初始化
来源：http://trt.cucudq.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gxj.sxryk.cn

[S10] C：指针与解引用
来源：http://dyk.jinyuanbaomall.cn

int *p = &a;  *p = 5;
来源：http://xex.snrcjt.cn

[S11] C：逐行读文件
来源：http://okl.sysykeji.top

FILE *f = fopen("a.txt", "r");
来源：http://iqr.ydjk.org.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rod.ybcxt.top

fclose(f);
来源：http://lyx.ybcxt.top

[S12] C：写文件
来源：http://vsq.ehwqpu.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://asm.jinqigufen.top

[S13] C：宏定义
来源：http://gps.epnwcf.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gtv.cqqwz.cn

[S14] C：枚举
来源：http://ztm.tanke756.top

enum Color { RED, GREEN, BLUE };
来源：http://ouk.yvedp.cn

[S15] C：类型转换
来源：http://rmu.xylfe.cn

(double) a / b
来源：http://gam.snrcjt.cn

[S16] C：位操作置位
来源：http://ucw.yj20258888.top

x |= (1 << 3);
来源：http://dup.sweek.top

[S17] C：安全拼接字符串
来源：http://imv.aizwys.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wtw.yuanzhike.top

[S18] C：命令行参数
来源：http://hih.sxryk.cn

int main(int argc, char **argv)
来源：http://mtt.jianghu66.top

[S19] C：快速排序
来源：http://web.ydjk.org.cn

qsort(a, n, sizeof(int), cmp);
来源：http://idw.52xcode.cn

[S20] C：二分查找
来源：http://tlo.gogol.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pny.daxiang520.top

[S21] C：字符类别判断
来源：http://vni.yj20258888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xrv.zhiwuduotai.top

[S22] C：字符串转数字
来源：http://oio.chenlongwang.top

atoi("42");  strtod("3.14", NULL);
来源：http://izo.mhx1999.top

[S23] C：随机数
来源：http://ays.daxiang520.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ljo.jianghu66.top

[S24] C：获取本地时间
来源：http://yqq.jinqigufen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rmg.gaohongyu789.top

[S25] C：内存拷贝
来源：http://fog.bjfxy.top

memcpy(dst, src, n);
来源：http://xls.nanxuanxn.top

[S26] C：内存清零
来源：http://iop.dashuyun.cn

memset(a, 0, sizeof a);
来源：http://bdf.guannengcc.top

[S27] C：定义常量
来源：http://rwo.jlsjyb.cn

const double PI = 3.14159;
来源：http://kxx.zycfv.cn

[S28] C：静态变量
来源：http://jwm.chenjidiqi.icu

static int counter = 0;
来源：http://ski.zhaomingkeji.xyz

[S29] C：变参函数
来源：http://vxr.sjlbkw.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://row.tian-w.cn

[S30] C：头文件保护
来源：http://dri.xuetiantiany.cn

#ifndef X_H
来源：http://efu.zhengqikj.top

#define X_H
来源：http://vnx.c1oappe.top

#endif
来源：http://zuo.fktsv.cn

[S31] C++：Hello World
来源：http://kvq.yuanzhike.top

#include <iostream>
来源：http://riz.cheryme.top

int main() { std::cout << "Hello\n"; }
来源：http://zvm.tarul.cn

[S32] C++：字符串
来源：http://rjr.jlsjyb.cn

std::string s = "hi";  s += "!";
来源：http://jcq.9152youxi.cn

[S33] C++：vector 增删
来源：http://axn.guannengcc.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ksn.havefunace.top

[S34] C++：遍历 vector
来源：http://fej.hammf.cn

for (auto &x : v) { std::cout << x; }
来源：http://wbh.zhongyouzk.top

[S35] C++：map
来源：http://lab.havefunace.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zlm.chenlongwang.top

[S36] C++：unordered_map
来源：http://gya.zhijiandao.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ygz.sjlbkw.cn

[S37] C++：set
来源：http://jls.yfazqb.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://buo.yfazqb.com

[S38] C++：排序
来源：http://ijg.yj20258888.top

std::sort(v.begin(), v.end());
来源：http://irj.smart0.xyz

[S39] C++：自定义比较器排序
来源：http://ucl.fzhhl.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rnj.feifeiyinyue.top

[S40] C++：查找元素
来源：http://mlc.fktsv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rwj.zycfv.cn

[S41] C++：类与构造函数
来源：http://apr.jyoumei.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gam.haohaochexian.top

[S42] C++：继承与虚函数
来源：http://ijj.jinyuanbaomall.cn

class B : public Base { public: void f() override {} };
来源：http://ppo.shzxlz.cn

[S43] C++：智能指针
来源：http://twt.cucudq.cn

auto p = std::make_unique<int>(5);
来源：http://ngm.zycfv.cn

[S44] C++：引用传参
来源：http://icw.tian-w.cn

void inc(int &x) { ++x; }
来源：http://pwy.cqqwz.cn

[S45] C++：lambda
来源：http://thg.yanxiufei.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bwz.yj202588.top

[S46] C++：函数模板
来源：http://mxx.havefunace.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bcc.tanke756.top

[S47] C++：结构化绑定遍历
来源：http://nmv.hesvh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vqe.mhx1999.top

[S48] C++：逐行读文件
来源：http://qgl.shanyushiyangkeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://hoy.yonumen.top

while (std::getline(in, line)) { }
来源：http://ico.yj202588.top

[S49] C++：写文件
来源：http://txw.shanyushiyangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://njf.havefunace.top

[S50] C++：格式化数字
来源：http://rjr.gaohongyu789.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nwq.yuxming.cn

[S51] C++：显式类型转换
来源：http://irk.jinqigufen.top

static_cast<double>(a) / b
来源：http://qfa.zhongyouzk.top

[S52] C++：const 与 noexcept
来源：http://xgd.cheryme.top

int size() const noexcept { return n_; }
来源：http://okr.yanxiufei.cn

[S53] C++：移动语义
来源：http://tdv.tian-w.cn

std::vector<int> w = std::move(v);
来源：http://hmr.andypj.xyz

[S54] C++：异常处理
来源：http://hnk.uphjek.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xlp.yvedp.cn

[S55] C++：结构化绑定
来源：http://jba.yanxiufei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dka.shangyingyoupin.top

[S56] C++：optional
来源：http://dde.uphjek.com


<!-- 参考信息 -->