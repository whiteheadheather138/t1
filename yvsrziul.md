代发 wailian999

[Q78] 当前时间
来源：http://qux.tianlin.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kpi.shuidangran.top

[Q79] 字符串拼接
来源：http://ftv.chenzaomai.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qok.sjlbkw.cn

[Q80] 字符串截取
来源：http://dra.nwbrower.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jgk.jyoumei.cn

[Q81] 字符串替换
来源：http://kbt.jyoumei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bmv.tanke756.top

[Q82] 字符长度与字节长度
来源：http://gwd.cucudq.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kai.yj20258888.top

[Q83] 大小写转换
来源：http://trg.quarkkingdee.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zmg.birdmap.top

[Q84] 去除首尾空格
来源：http://gfq.hnqzz.top

SELECT TRIM(name) FROM users;
来源：http://vki.epnwcf.com

[Q85] 数值取整
来源：http://ofx.cheryme.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lwq.zhiwuduotai.top

[Q86] 读取 JSON 字段
来源：http://kuk.zhijiandao.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://msx.birdmap.top

[Q87] JSON 字段做条件
来源：http://kfe.ydjk.org.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cqd.yvedp.cn

[Q88] 行转列（条件聚合）
来源：http://eqp.fzhhl.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ylu.xuetiantiany.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uig.iojbl.cn

[Q89] 判断表是否存在
来源：http://oje.yfazqb.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pkh.tanke756.top

[Q90] 生成序号列
来源：http://ark.feifeiyinyue.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dhe.yonumen.top

================================================================================
来源：http://otl.yanxiufei.cn

R. Bash 专题
来源：http://sbf.ivvv.top

================================================================================
来源：http://hmb.pycfn.com

[R01] shebang 与严格模式
来源：http://yqy.uphjek.com

#!/usr/bin/env bash
来源：http://lhp.zdbjq.cn

set -euo pipefail
来源：http://tlm.cucudq.cn

[R02] 变量赋值与使用
来源：http://kzz.zhongyouzk.top

name="Tom"; echo "$name"
来源：http://jwv.zhijiandao.cn

[R03] 只读变量
来源：http://jma.gaohongyu789.top

readonly PI=3.14
来源：http://zps.ivvv.top

[R04] 位置参数
来源：http://dcw.jinghuilouyu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ikt.zhengqikj.top

[R05] 参数默认值
来源：http://jkf.sweek.top

name="${1:-default}"
来源：http://rdv.jqgfzy.top

[R06] 判断命令是否存在
来源：http://ltm.9152youxi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fgu.xziqi.cn

[R07] if 判断文件
来源：http://xbo.tian-w.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rwo.wangshuangyany.cn

[R08] 数值比较
来源：http://aku.sweek.top

if (( a > b )); then echo "a 更大"; fi
来源：http://fxr.xylfe.cn

[R09] 字符串比较
来源：http://jtp.meibo888.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pxb.uphjek.com

[R10] 正则匹配
来源：http://kxn.0kj1m.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zvt.gzhubu.top

[R11] case 多分支
来源：http://bfw.bbcook.cn

case "$1" in
来源：http://ubj.hnqzz.top

start) echo "启动" ;;
来源：http://wnf.shanyushiyangkeji.top

stop)  echo "停止" ;;
来源：http://bnk.tanke756.top

*)     echo "未知命令" ;;
来源：http://zbj.cashguo.top

esac
来源：http://oot.fktsv.cn

[R12] for 遍历文件
来源：http://vpq.bbcook.cn

for f in *.txt; do echo "$f"; done
来源：http://djh.ehwqpu.com

[R13] for 计数循环
来源：http://zpu.xuanzx.com

for i in {1..10}; do echo "$i"; done
来源：http://wzo.9152youxi.cn

[R14] C 风格 for
来源：http://qxy.havefunace.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ekv.ybcxt.top

[R15] while 逐行读文件
来源：http://ycg.guannengcc.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://spq.hesvh.cn

[R16] until 等待条件
来源：http://aea.yuxming.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pxk.cqqwz.cn

[R17] 数组定义与取值
来源：http://qre.snrcjt.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wqn.uphjek.com

[R18] 遍历数组
来源：http://yqp.ivvv.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bnz.yonumen.top

[R19] 数组长度
来源：http://vuw.gotoacloud.top

echo "${#arr[@]}"
来源：http://mza.hywenlv.cn

[R20] 关联数组（字典）
来源：http://bev.jianghu66.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ofn.316326.xyz

[R21] 字符串长度
来源：http://olj.birdmap.top

echo "${#s}"
来源：http://mtr.shuidangran.top

[R22] 截取子串
来源：http://dbo.haohaochexian.top

echo "${s:0:5}"
来源：http://rwu.vehdjk.com

[R23] 字符串替换
来源：http://gef.shanyushiyangtech.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qpp.hnqzz.top

[R24] 大小写转换
来源：http://cqm.hysaishi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gim.cheryme.top

[R25] 去后缀 / 去前缀
来源：http://xpf.hysaishi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://hvv.guowangkeji.top

[R26] 命令替换
来源：http://hgq.fehbvm.com

now=$(date +%F); echo "$now"
来源：http://ahp.redwolf501.top

[R27] 算术展开
来源：http://jgs.ywan-chungtsiang.top

echo $((1 + 2 * 3))
来源：http://jlf.jyoumei.cn

[R28] 浮点运算
来源：http://rur.havefunace.top

echo "scale=2; 10/3" | bc
来源：http://smv.hcnkem.com

[R29] 定义函数
来源：http://pgz.guowangkeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ipj.yvedp.cn

[R30] 函数返回状态码
来源：http://erv.chenjidiqi.icu

f() { return 0; }; f || echo "失败了"
来源：http://hcg.fktsv.cn

[R31] 局部变量
来源：http://hjv.bjfxy.top

f() { local x=1; echo "$x"; }
来源：http://kio.xinyue.icu

[R32] 参数个数校验
来源：http://fql.tarul.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ihv.sufxvd.cn

[R33] 捕获错误并提示行号
来源：http://hvd.vehdjk.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yyh.zhaomingkeji.xyz

[R34] 退出时清理
来源：http://nol.tian-w.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hby.yuanzhike.top

[R35] 后台执行并等待
来源：http://zio.yonumen.top

sleep 5 & pid=$!; wait "$pid"
来源：http://gcm.snrcjt.cn

[R36] 并发执行多个任务
来源：http://qde.nanxinkj.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dti.zhixingplan.top

[R37] 把输出赋给变量
来源：http://lkl.daria6918.cn

files=$(ls -1)
来源：http://lfn.ppjwa.cn

[R38] 管道串联
来源：http://avp.aibaodan.cn

cat a.txt | grep -i error | wc -l
来源：http://qdi.xylfe.cn

[R39] 重定向标准输出与错误
来源：http://brr.dashuyun.cn

cmd > out.log 2>&1
来源：http://ouv.bbcook.cn

[R40] 追加写日志
来源：http://gqt.cucudq.cn

echo "log" >> out.log
来源：http://fcn.cashguo.top

[R41] 丢弃输出
来源：http://vre.nanxuanxn.top

cmd >/dev/null 2>&1
来源：http://asm.cqqwz.cn

[R42] 输入重定向
来源：http://fcm.epnwcf.com

wc -l < a.txt
来源：http://jbp.guannengcc.top

[R43] 按名字查找文件
来源：http://neq.cdnleiting.top

find . -name "*.log" -type f
来源：http://nzj.pengpengdd.cyou

[R44] 按修改时间查找
来源：http://inn.fehbvm.com

find . -mtime -7 -type f
来源：http://uac.nwbrower.top

[R45] 批量删除
来源：http://tco.smart0.xyz

find . -name "*.tmp" -delete
来源：http://aen.zhixingplan.top

[R46] 递归替换文件内容
来源：http://pwj.sxryk.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://evy.fehbvm.com

[R47] sed 单行替换
来源：http://xar.yj20258888.top

sed -i 's/foo/bar/g' a.txt
来源：http://dtp.tanke756.top

[R48] awk 取指定列
来源：http://hqm.kuanghao11.cn

awk '{print $1, $3}' a.txt
来源：http://ncz.zhaomingkeji.xyz

[R49] awk 带条件
来源：http://yjn.quarkkingdee.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ilx.ydzc1.top

[R50] awk 求和
来源：http://juj.shzxlz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hun.daxiang520.top

[R51] 排序去重取前几
来源：http://hzn.xinyue.icu

sort a.txt | uniq -c | sort -rn | head
来源：http://nen.hfpthk.cn

[R52] 统计行数
来源：http://xbe.zhijiandao.cn

wc -l a.txt
来源：http://ive.haohaochexian.top

[R53] 查看文件头与实时尾
来源：http://ecg.gaohongyu789.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://joj.cashguo.top

[R54] 比较两个文件
来源：http://tuj.quarkkingdee.top

diff a.txt b.txt
来源：http://adm.jinqigufen.top

[R55] 压缩与解压
来源：http://uwq.chenzaomai.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mez.chenlongwang.top

[R56] 远程拷贝
来源：http://yis.tian-w.cn

scp file user@host:/path/
来源：http://eas.pycfn.com

[R57] 远程执行命令
来源：http://vig.yj20258.top

ssh user@host 'uptime'
来源：http://ebw.yj202588.top

[R58] 下载文件
来源：http://mot.fehbvm.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hto.zhaomingkeji.xyz

[R59] 发 POST JSON
来源：http://oex.tarul.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gxc.svipenyu.cn

[R60] 只看 HTTP 状态码
来源：http://aky.kuanghao11.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kau.cqqwz.cn

[R61] 磁盘占用
来源：http://fnb.sjlbkw.cn

df -h;  du -sh *
来源：http://gpw.jinyuanbaomall.cn

[R62] 找最占空间的文件
来源：http://mfe.ywan-chungtsiang.top

du -ah . | sort -rh | head -10
来源：http://ktc.jqgufenzy.top

[R63] 内存与进程
来源：http://mob.52xcode.cn

free -h;  ps aux | grep nginx
来源：http://jhs.jlsjyb.cn

[R64] 结束进程
来源：http://kij.zhixingplan.top

kill -9 $(pgrep -f app.py)
来源：http://urx.sxryk.cn

[R65] 查看端口占用
来源：http://dac.zdbjq.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zwa.pengpengdd.cyou

[R66] 定时任务
来源：http://iln.tian-w.cn

crontab -e;  crontab -l
来源：http://mlw.xuanzx.com

[R67] 生成随机十六进制串
来源：http://sta.ybcxt.top

openssl rand -hex 16
来源：http://fto.sxryk.cn

[R68] 计算文件校验值
来源：http://lcz.gotoacloud.top

sha256sum a.txt;  md5sum a.txt
来源：http://sip.hnxiangtu.top

[R69] 生成随机密码
来源：http://oyp.vehdjk.com

head -c 16 /dev/urandom | base64
来源：http://qjw.tianlin.xyz

[R70] 时间戳与互转
来源：http://twc.guowangkeji.top

date +%s;  date -d @1700000000
来源：http://gbs.wangdashe.top

[R71] 日期格式化
来源：http://jao.aizwys.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dqi.yongpay.top

[R72] 等待端口就绪
来源：http://txd.ydzc1.top

until nc -z localhost 3306; do sleep 1; done
来源：http://pbe.ivvv.top

[R73] 分割大日志
来源：http://oge.mhx1999.top

split -l 1000 big.log part_
来源：http://gyr.fanxiaobao.xyz

[R74] 批量重命名
来源：http://tjo.wangdashe.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://meq.zhijiandao.cn

[R75] 导出环境变量
来源：http://yxt.sysykeji.top

export PATH="$HOME/bin:$PATH"
来源：http://fqh.tarul.cn

[R76] 使用临时文件
来源：http://cvj.chenlongwang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eou.0kj1m.cn

[R77] 读取用户输入
来源：http://cmn.jinghuilouyu.cn

read -rp "请输入: " ans
来源：http://elk.0kj1m.cn

[R78] 交互式菜单
来源：http://dse.yj20258888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://gib.c1oappe.top

[R79] 解析命令行选项
来源：http://urx.sxryk.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xwi.yj202588.top

[R80] 查看脚本执行耗时
来源：http://fxc.zhongyouzk.top

time ./run.sh
来源：http://anl.nanxinkj.top

================================================================================
来源：http://rfe.chenlongwang.top

S. C / C++ 专题
来源：http://wgn.gzhubu.top

================================================================================
来源：http://btu.bjfxy.top

[S01] C：Hello World
来源：http://ddd.havefunace.top

#include <stdio.h>
来源：http://krg.ivvv.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://hjr.redwolf501.top

[S02] C：变量与格式化输出
来源：http://dbj.mhx1999.top

int a = 10; printf("%d\n", a);
来源：http://cjm.daxiang520.top

[S03] C：读入整数
来源：http://top.fanxiaobao.xyz

int x; scanf("%d", &x);
来源：http://rcm.316326.xyz

[S04] C：字符串复制
来源：http://owx.xziqi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ojr.yueranfly.top

[S05] C：字符串长度
来源：http://pif.kuanghao11.cn

strlen(s)
来源：http://qsw.snrcjt.cn

[S06] C：字符串比较
来源：http://iat.sweek.top

strcmp(a, b) == 0
来源：http://lxy.chenjidiqi.icu

[S07] C：数组遍历求和
来源：http://pxs.yueranfly.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gvp.vehdjk.com

[S08] C：动态内存分配与释放
来源：http://gvq.zhixingplan.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jtl.snrcjt.cn

[S09] C：结构体定义与初始化
来源：http://mxl.vqdsnc.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://emr.cucudq.cn

[S10] C：指针与解引用
来源：http://elo.jlsjyb.cn

int *p = &a;  *p = 5;
来源：http://tbj.aibaodan.cn

[S11] C：逐行读文件
来源：http://cer.xinyue.icu

FILE *f = fopen("a.txt", "r");
来源：http://fye.feifeiyinyue.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://syw.nanxuanxn.top

fclose(f);
来源：http://ecu.cheryme.top

[S12] C：写文件
来源：http://red.cheryme.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bkt.cqqwz.cn

[S13] C：宏定义
来源：http://yei.fanxiaobao.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ueu.pycfn.com

[S14] C：枚举
来源：http://bvq.kuanghao11.cn

enum Color { RED, GREEN, BLUE };
来源：http://sma.snrcjt.cn

[S15] C：类型转换
来源：http://nlc.zhaomingkeji.xyz

(double) a / b
来源：http://yjc.chenlongwang.top

[S16] C：位操作置位
来源：http://lfv.ivvv.top

x |= (1 << 3);
来源：http://pit.guowangkeji.top

[S17] C：安全拼接字符串
来源：http://hwc.hfpthk.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pba.52xcode.cn

[S18] C：命令行参数
来源：http://yme.cheryme.top

int main(int argc, char **argv)
来源：http://wkn.chenlongwang.top

[S19] C：快速排序
来源：http://tnk.dianchejie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://aah.gotoacloud.top

[S20] C：二分查找
来源：http://fmo.ehwqpu.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://djx.wangshuangyany.cn

[S21] C：字符类别判断
来源：http://qwd.zycfv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xtx.aibaodan.cn

[S22] C：字符串转数字
来源：http://wil.yuxming.cn

atoi("42");  strtod("3.14", NULL);
来源：http://mps.yuxming.cn

[S23] C：随机数
来源：http://jrr.iojbl.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fxm.zhaomingkeji.xyz

[S24] C：获取本地时间
来源：http://bbw.dashuyun.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hrm.52xcode.cn

[S25] C：内存拷贝
来源：http://ahh.wangdashe.top

memcpy(dst, src, n);
来源：http://rar.jiagoushi.top

[S26] C：内存清零
来源：http://jtv.feifeiyinyue.top

memset(a, 0, sizeof a);
来源：http://vfp.nanxuanxn.top

[S27] C：定义常量
来源：http://auc.cheryme.top

const double PI = 3.14159;
来源：http://fnp.zhaomingkeji.xyz

[S28] C：静态变量
来源：http://hav.fehbvm.com

static int counter = 0;
来源：http://zkp.pengpengdd.cyou

[S29] C：变参函数
来源：http://kkk.fanxiaobao.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ybd.yuxming.cn

[S30] C：头文件保护
来源：http://owc.sjlbkw.cn

#ifndef X_H
来源：http://cdw.ydjk.org.cn

#define X_H
来源：http://jlt.ppjwa.cn

#endif
来源：http://uen.yuxming.cn

[S31] C++：Hello World
来源：http://asu.chenzaomai.com

#include <iostream>
来源：http://lcq.nanxuanxn.top

int main() { std::cout << "Hello\n"; }
来源：http://zqz.cdnleiting.top

[S32] C++：字符串
来源：http://nxv.cucudq.cn

std::string s = "hi";  s += "!";
来源：http://ude.xingfuxueyuan.xyz

[S33] C++：vector 增删
来源：http://aln.tarul.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hpb.jyoumei.cn

[S34] C++：遍历 vector
来源：http://kab.jlsjyb.cn

for (auto &x : v) { std::cout << x; }
来源：http://lbh.yvedp.cn

[S35] C++：map
来源：http://wxn.feifeiyinyue.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://azx.shangyingyoupin.top

[S36] C++：unordered_map
来源：http://tsd.zhixingplan.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jmi.chenzaomai.com

[S37] C++：set
来源：http://pfp.zdqjudy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://iyu.xylfe.cn

[S38] C++：排序
来源：http://rhm.hywenlv.cn

std::sort(v.begin(), v.end());
来源：http://kqm.feifeiyinyue.top

[S39] C++：自定义比较器排序
来源：http://njs.fzhhl.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://afv.zhongyouzk.top

[S40] C++：查找元素
来源：http://ksb.jqgfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gre.fengsongda.top

[S41] C++：类与构造函数
来源：http://xfm.chenzaomai.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://umr.xingfuxueyuan.xyz

[S42] C++：继承与虚函数
来源：http://xzz.sxryk.cn

class B : public Base { public: void f() override {} };
来源：http://nmi.ydjk.org.cn

[S43] C++：智能指针
来源：http://pzp.zhixingplan.top

auto p = std::make_unique<int>(5);
来源：http://lty.xinyue.icu

[S44] C++：引用传参
来源：http://iht.shanyushiyangtech.top

void inc(int &x) { ++x; }
来源：http://cbi.zhoulong.xyz

[S45] C++：lambda
来源：http://fmw.havefunace.top

auto add = [](int a, int b) { return a + b; };
来源：http://jsx.hysaishi.cn

[S46] C++：函数模板
来源：http://prc.vqdsnc.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oui.52xcode.cn

[S47] C++：结构化绑定遍历
来源：http://fbi.aizwys.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tmm.gzhubu.top

[S48] C++：逐行读文件
来源：http://ixs.shzxlz.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gzy.sufxvd.cn


<!-- 参考信息 -->