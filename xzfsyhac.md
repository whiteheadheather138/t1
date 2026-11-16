代发 wailian999

ANALYZE TABLE users;
来源：http://jby.yj20258888.top

[Q71] 查看建表语句
来源：http://rzw.tianlin.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pit.hesvh.cn

[Q72] 查看索引
来源：http://tfq.sjlbkw.cn

SHOW INDEX FROM users;
来源：http://whj.wangshuangyany.cn

[Q73] 查看表状态
来源：http://fur.xziqi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qhf.ydzc1.top

[Q74] 强制使用索引
来源：http://zee.kuanghao11.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yjm.zdqjudy.top

[Q75] 日期格式化
来源：http://cln.hesvh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://txk.snrcjt.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xgl.nwbrower.top

[Q76] 按天统计
来源：http://kua.guowangkeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rrw.nwbrower.top

[Q77] 时间加减
来源：http://moy.ydjk.org.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://amq.vqdsnc.cn

[Q78] 当前时间
来源：http://tuf.andypj.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yev.yueranfly.top

[Q79] 字符串拼接
来源：http://hdc.hesvh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gad.pengpengdd.cyou

[Q80] 字符串截取
来源：http://zyx.jyoumei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rdl.kuanghao11.cn

[Q81] 字符串替换
来源：http://fas.redwolf501.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://soo.ivvv.top

[Q82] 字符长度与字节长度
来源：http://cff.jlsjyb.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uoq.bbcook.cn

[Q83] 大小写转换
来源：http://ogo.ehwqpu.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hqh.ctjpmb.com

[Q84] 去除首尾空格
来源：http://jks.sufxvd.cn

SELECT TRIM(name) FROM users;
来源：http://qks.cheryme.top

[Q85] 数值取整
来源：http://uqv.shanyushiyangtech.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tzl.9152youxi.cn

[Q86] 读取 JSON 字段
来源：http://oej.cheryme.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://iaz.sweek.top

[Q87] JSON 字段做条件
来源：http://qcf.havefunace.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xyr.yuxming.cn

[Q88] 行转列（条件聚合）
来源：http://yup.cdnleiting.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kln.fzhhl.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://szi.xuetiantiany.cn

[Q89] 判断表是否存在
来源：http://mke.chenzaomai.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ceg.sweek.top

[Q90] 生成序号列
来源：http://ace.xylfe.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jkk.yongpay.top

================================================================================
来源：http://dfb.yfazqb.com

R. Bash 专题
来源：http://ojt.fzhhl.top

================================================================================
来源：http://dms.gogol.net.cn

[R01] shebang 与严格模式
来源：http://fge.zhoulong.xyz

#!/usr/bin/env bash
来源：http://xsi.pycfn.com

set -euo pipefail
来源：http://pen.zhaomingkeji.xyz

[R02] 变量赋值与使用
来源：http://ety.ywan-chungtsiang.top

name="Tom"; echo "$name"
来源：http://mml.chenzaomai.com

[R03] 只读变量
来源：http://khj.shuidangran.top

readonly PI=3.14
来源：http://ado.wangdashe.top

[R04] 位置参数
来源：http://rbk.xingfuxueyuan.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rkl.gzhubu.top

[R05] 参数默认值
来源：http://whs.shanyushiyangkeji.top

name="${1:-default}"
来源：http://jqy.redwolf501.top

[R06] 判断命令是否存在
来源：http://eri.zdbjq.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://iqo.gzhubu.top

[R07] if 判断文件
来源：http://tmw.havefunace.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://qel.shanyushiyangtech.top

[R08] 数值比较
来源：http://scz.fehbvm.com

if (( a > b )); then echo "a 更大"; fi
来源：http://dvk.zdbjq.cn

[R09] 字符串比较
来源：http://woh.zhengqikj.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://oga.sweek.top

[R10] 正则匹配
来源：http://phl.fehbvm.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gyp.chenzaomai.com

[R11] case 多分支
来源：http://nat.tarul.cn

case "$1" in
来源：http://smd.zhiwuduotai.top

start) echo "启动" ;;
来源：http://nrp.vehdjk.com

stop)  echo "停止" ;;
来源：http://gxk.zhengqikj.top

*)     echo "未知命令" ;;
来源：http://hkx.wangdashe.top

esac
来源：http://hor.tianlin.xyz

[R12] for 遍历文件
来源：http://rxu.jlsjyb.cn

for f in *.txt; do echo "$f"; done
来源：http://fmx.yonumen.top

[R13] for 计数循环
来源：http://ocu.pengpengdd.cyou

for i in {1..10}; do echo "$i"; done
来源：http://ynt.gogol.net.cn

[R14] C 风格 for
来源：http://wiq.xingfuxueyuan.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ize.bbcook.cn

[R15] while 逐行读文件
来源：http://deo.ehwqpu.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://utk.pengpengdd.cyou

[R16] until 等待条件
来源：http://zyc.chenzaomai.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rny.meibo888.top

[R17] 数组定义与取值
来源：http://uys.fanxiaobao.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://aqy.jinqigufen.top

[R18] 遍历数组
来源：http://kqr.daria6918.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xvh.gotoacloud.top

[R19] 数组长度
来源：http://nvr.hammf.cn

echo "${#arr[@]}"
来源：http://kck.yj202588.top

[R20] 关联数组（字典）
来源：http://qmu.jinghuilouyu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://czz.zhiwuduotai.top

[R21] 字符串长度
来源：http://jcq.zhiwuduotai.top

echo "${#s}"
来源：http://pdh.chenzaomai.com

[R22] 截取子串
来源：http://qci.haohaochexian.top

echo "${s:0:5}"
来源：http://dts.zycfv.cn

[R23] 字符串替换
来源：http://fia.jinqigfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://djg.cheryme.top

[R24] 大小写转换
来源：http://smp.cqqwz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://zof.yuxming.cn

[R25] 去后缀 / 去前缀
来源：http://btd.zhijiandao.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yta.shuidangran.top

[R26] 命令替换
来源：http://dda.sxryk.cn

now=$(date +%F); echo "$now"
来源：http://kgp.quarkkingdee.top

[R27] 算术展开
来源：http://bnf.shangyingyoupin.top

echo $((1 + 2 * 3))
来源：http://qzc.gogol.net.cn

[R28] 浮点运算
来源：http://fhs.cqqwz.cn

echo "scale=2; 10/3" | bc
来源：http://vkw.sysykeji.top

[R29] 定义函数
来源：http://bet.ehwqpu.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rzj.fktsv.cn

[R30] 函数返回状态码
来源：http://lim.haohaochexian.top

f() { return 0; }; f || echo "失败了"
来源：http://nbl.ydzc1.top

[R31] 局部变量
来源：http://hsc.gotoacloud.top

f() { local x=1; echo "$x"; }
来源：http://nwd.svipenyu.cn

[R32] 参数个数校验
来源：http://cnk.c1oappe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://one.shanyushiyangtech.top

[R33] 捕获错误并提示行号
来源：http://fvc.guannengcc.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nkx.vqdsnc.cn

[R34] 退出时清理
来源：http://lzb.hnqzz.top

trap 'rm -f "$tmp"' EXIT
来源：http://ylo.vqdsnc.cn

[R35] 后台执行并等待
来源：http://pvz.vqdsnc.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ycc.quarkkingdee.top

[R36] 并发执行多个任务
来源：http://ywu.vqdsnc.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xyv.ydzc1.top

[R37] 把输出赋给变量
来源：http://paz.gotoacloud.top

files=$(ls -1)
来源：http://epk.zhixingplan.top

[R38] 管道串联
来源：http://hbo.yongpay.top

cat a.txt | grep -i error | wc -l
来源：http://hzp.jinyuanbaomall.cn

[R39] 重定向标准输出与错误
来源：http://tkw.bjfxy.top

cmd > out.log 2>&1
来源：http://bgt.shuidangran.top

[R40] 追加写日志
来源：http://peq.aibaodan.cn

echo "log" >> out.log
来源：http://xyj.zdbjq.cn

[R41] 丢弃输出
来源：http://mgm.chenlongwang.top

cmd >/dev/null 2>&1
来源：http://rbr.aibaodan.cn

[R42] 输入重定向
来源：http://dpk.zhengqikj.top

wc -l < a.txt
来源：http://bnb.hongshengwenyu.top

[R43] 按名字查找文件
来源：http://iqt.yangfankeji.com

find . -name "*.log" -type f
来源：http://xlb.xuetiantiany.cn

[R44] 按修改时间查找
来源：http://qzz.dianchejie.cn

find . -mtime -7 -type f
来源：http://rlo.yongpay.top

[R45] 批量删除
来源：http://ctj.jyoumei.cn

find . -name "*.tmp" -delete
来源：http://una.zhixingplan.top

[R46] 递归替换文件内容
来源：http://mwc.cqqwz.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qfk.cqqwz.cn

[R47] sed 单行替换
来源：http://byd.fengsongda.top

sed -i 's/foo/bar/g' a.txt
来源：http://kjh.c1oappe.top

[R48] awk 取指定列
来源：http://izm.guowangkeji.top

awk '{print $1, $3}' a.txt
来源：http://olu.jiagoushi.top

[R49] awk 带条件
来源：http://owb.fzhhl.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vqx.tian-w.cn

[R50] awk 求和
来源：http://vog.yonumen.top

awk '{s += $2} END {print s}' a.txt
来源：http://tcf.xziqi.cn

[R51] 排序去重取前几
来源：http://atg.zhengqikj.top

sort a.txt | uniq -c | sort -rn | head
来源：http://dvr.haohaochexian.top

[R52] 统计行数
来源：http://hxx.vqdsnc.cn

wc -l a.txt
来源：http://sbv.gaohongyu789.top

[R53] 查看文件头与实时尾
来源：http://szj.pengpengdd.cyou

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fzm.0kj1m.cn

[R54] 比较两个文件
来源：http://laf.shuidangran.top

diff a.txt b.txt
来源：http://piu.haohaochexian.top

[R55] 压缩与解压
来源：http://lpy.xingfuxueyuan.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bui.yj202588.top

[R56] 远程拷贝
来源：http://zeq.yfazqb.com

scp file user@host:/path/
来源：http://gvi.xylfe.cn

[R57] 远程执行命令
来源：http://shq.sweek.top

ssh user@host 'uptime'
来源：http://fef.ehwqpu.com

[R58] 下载文件
来源：http://vgs.sufxvd.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lno.yuanzhike.top

[R59] 发 POST JSON
来源：http://vbw.yongpay.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ggg.birdmap.top

[R60] 只看 HTTP 状态码
来源：http://fto.dianchejie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nok.havefunace.top

[R61] 磁盘占用
来源：http://kha.xuanzx.com

df -h;  du -sh *
来源：http://trd.hongshengwenyu.top

[R62] 找最占空间的文件
来源：http://pus.cheryme.top

du -ah . | sort -rh | head -10
来源：http://lip.zhixingplan.top

[R63] 内存与进程
来源：http://euc.jinghuilouyu.cn

free -h;  ps aux | grep nginx
来源：http://fio.yongpay.top

[R64] 结束进程
来源：http://lys.gaohongyu789.top

kill -9 $(pgrep -f app.py)
来源：http://nyv.ehwqpu.com

[R65] 查看端口占用
来源：http://jds.quarkkingdee.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://iws.epnwcf.com

[R66] 定时任务
来源：http://xez.hesvh.cn

crontab -e;  crontab -l
来源：http://riq.nwbrower.top

[R67] 生成随机十六进制串
来源：http://fct.jinqigufen.top

openssl rand -hex 16
来源：http://izo.yj20258.top

[R68] 计算文件校验值
来源：http://upo.9152youxi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bgl.vqdsnc.cn

[R69] 生成随机密码
来源：http://prf.tanke756.top

head -c 16 /dev/urandom | base64
来源：http://qrl.hcnkem.com

[R70] 时间戳与互转
来源：http://feg.shanyushiyangkeji.top

date +%s;  date -d @1700000000
来源：http://vmd.gotoacloud.top

[R71] 日期格式化
来源：http://oxi.zdbjq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wiy.zhijiandao.cn

[R72] 等待端口就绪
来源：http://rri.zdqjudy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://xtd.chenzaomai.com

[R73] 分割大日志
来源：http://ihw.nanxinkj.top

split -l 1000 big.log part_
来源：http://qol.daxiang520.top

[R74] 批量重命名
来源：http://cqk.bjfxy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yyc.tianlin.xyz

[R75] 导出环境变量
来源：http://pnz.yj20258.top

export PATH="$HOME/bin:$PATH"
来源：http://rxu.jinqigufen.top

[R76] 使用临时文件
来源：http://zwh.chenzaomai.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gla.wangshuangyany.cn

[R77] 读取用户输入
来源：http://kxs.xziqi.cn

read -rp "请输入: " ans
来源：http://quv.zhongyouzk.top

[R78] 交互式菜单
来源：http://oyj.cashguo.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ahi.gaohongyu789.top

[R79] 解析命令行选项
来源：http://zpy.gotoacloud.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dys.zhijiandao.cn

[R80] 查看脚本执行耗时
来源：http://oya.redwolf501.top

time ./run.sh
来源：http://mhf.zhijiandao.cn

================================================================================
来源：http://rfo.svipenyu.cn

S. C / C++ 专题
来源：http://lgq.andypj.xyz

================================================================================
来源：http://rul.gotoacloud.top

[S01] C：Hello World
来源：http://sca.hnqzz.top

#include <stdio.h>
来源：http://tbf.guowangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ljc.hesvh.cn

[S02] C：变量与格式化输出
来源：http://exy.guowangkeji.top

int a = 10; printf("%d\n", a);
来源：http://hbs.fzhhl.top

[S03] C：读入整数
来源：http://flq.cheryme.top

int x; scanf("%d", &x);
来源：http://ppi.smart0.xyz

[S04] C：字符串复制
来源：http://aou.zhongyouzk.top

char dst[32]; strcpy(dst, "hi");
来源：http://fvm.ybcxt.top

[S05] C：字符串长度
来源：http://yys.daria6918.cn

strlen(s)
来源：http://rqk.nanxinkj.top

[S06] C：字符串比较
来源：http://fcq.quarkkingdee.top

strcmp(a, b) == 0
来源：http://ker.mhx1999.top

[S07] C：数组遍历求和
来源：http://stk.smart0.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pja.xuetiantiany.cn

[S08] C：动态内存分配与释放
来源：http://vzu.hcnkem.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jus.cqqwz.cn

[S09] C：结构体定义与初始化
来源：http://edl.kuanghao11.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vih.fzhhl.top

[S10] C：指针与解引用
来源：http://upb.cashguo.top

int *p = &a;  *p = 5;
来源：http://fzc.ydzc1.top

[S11] C：逐行读文件
来源：http://kqn.ybcxt.top

FILE *f = fopen("a.txt", "r");
来源：http://aao.kuanghao11.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ywa.nwbrower.top

fclose(f);
来源：http://qsf.fehbvm.com

[S12] C：写文件
来源：http://kai.xziqi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://err.9152youxi.cn

[S13] C：宏定义
来源：http://yda.zhengqikj.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wxe.kuanghao11.cn

[S14] C：枚举
来源：http://hfd.sjlbkw.cn

enum Color { RED, GREEN, BLUE };
来源：http://wqp.snrcjt.cn

[S15] C：类型转换
来源：http://rfx.yueranfly.top

(double) a / b
来源：http://pfz.ctjpmb.com

[S16] C：位操作置位
来源：http://dfy.yfazqb.com

x |= (1 << 3);
来源：http://euk.havefunace.top

[S17] C：安全拼接字符串
来源：http://ocw.ivvv.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gsn.nwbrower.top

[S18] C：命令行参数
来源：http://aid.aizwys.cn

int main(int argc, char **argv)
来源：http://khm.52xcode.cn

[S19] C：快速排序
来源：http://osq.yuanzhike.top

qsort(a, n, sizeof(int), cmp);
来源：http://msw.sweek.top

[S20] C：二分查找
来源：http://xia.hnxiangtu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mgu.snrcjt.cn

[S21] C：字符类别判断
来源：http://ezm.316326.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ffj.yuxming.cn

[S22] C：字符串转数字
来源：http://jbw.feifeiyinyue.top

atoi("42");  strtod("3.14", NULL);
来源：http://cud.ppjwa.cn

[S23] C：随机数
来源：http://gqm.fzhhl.top

srand(time(NULL));  int r = rand() % 100;
来源：http://dfn.gotoacloud.top

[S24] C：获取本地时间
来源：http://fkn.ydjk.org.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pjp.daxiang520.top

[S25] C：内存拷贝
来源：http://vhd.jqgufenzy.top

memcpy(dst, src, n);
来源：http://gqt.hongshengwenyu.top

[S26] C：内存清零
来源：http://irn.yj20258.top

memset(a, 0, sizeof a);
来源：http://ico.fengsongda.top

[S27] C：定义常量
来源：http://ccb.chenlongwang.top

const double PI = 3.14159;
来源：http://hoz.zhixingplan.top

[S28] C：静态变量
来源：http://nnz.shangyingyoupin.top

static int counter = 0;
来源：http://kel.smart0.xyz

[S29] C：变参函数
来源：http://lea.feifeiyinyue.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cdq.smart0.xyz

[S30] C：头文件保护
来源：http://dvl.guannengcc.top

#ifndef X_H
来源：http://hep.tanke756.top

#define X_H
来源：http://lds.nanxuanxn.top

#endif
来源：http://dsv.daria6918.cn

[S31] C++：Hello World
来源：http://txn.feifeiyinyue.top

#include <iostream>
来源：http://ctk.bjfxy.top

int main() { std::cout << "Hello\n"; }
来源：http://oyo.yfazqb.com

[S32] C++：字符串
来源：http://lzv.sysykeji.top

std::string s = "hi";  s += "!";
来源：http://ast.tianlin.xyz

[S33] C++：vector 增删
来源：http://bdc.jiagoushi.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fur.chenjidiqi.icu

[S34] C++：遍历 vector
来源：http://lmy.zdbjq.cn

for (auto &x : v) { std::cout << x; }
来源：http://pzj.snrcjt.cn

[S35] C++：map
来源：http://qju.shanyushiyangtech.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ocb.jiagoushi.top

[S36] C++：unordered_map
来源：http://avr.ydjk.org.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kla.guannengcc.top

[S37] C++：set
来源：http://yvl.cheryme.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://enx.shzxlz.cn

[S38] C++：排序
来源：http://sav.guowangkeji.top

std::sort(v.begin(), v.end());
来源：http://bpp.fengsongda.top

[S39] C++：自定义比较器排序
来源：http://eqt.sjlbkw.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nsu.ywan-chungtsiang.top

[S40] C++：查找元素
来源：http://qhq.mhx1999.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qfj.hongshengwenyu.top


<!-- 参考信息 -->