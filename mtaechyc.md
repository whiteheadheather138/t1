代发 wailian999

[Q67] 设置隔离级别
来源：http://wzi.sjlbkw.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://crd.haohaochexian.top

[Q68] 保存点
来源：http://qxk.gogol.net.cn

SAVEPOINT sp1;
来源：http://czx.daria6918.cn

ROLLBACK TO sp1;
来源：http://ckn.snrcjt.cn

[Q69] 查看执行计划
来源：http://rkn.yj202588.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bzb.ehwqpu.com

[Q70] 更新统计信息
来源：http://fni.pengpengdd.cyou

ANALYZE TABLE users;
来源：http://kdb.hongshengwenyu.top

[Q71] 查看建表语句
来源：http://eww.zhengqikj.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://biu.cashguo.top

[Q72] 查看索引
来源：http://pya.tian-w.cn

SHOW INDEX FROM users;
来源：http://oqw.shzxlz.cn

[Q73] 查看表状态
来源：http://vfl.shangyingyoupin.top

SHOW TABLE STATUS LIKE 'users';
来源：http://lhs.aibaodan.cn

[Q74] 强制使用索引
来源：http://jls.jinqigfzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://obq.jianghu66.top

[Q75] 日期格式化
来源：http://dpm.xuetiantiany.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://diu.fengsongda.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xdn.meibo888.top

[Q76] 按天统计
来源：http://ryy.zdqjudy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dia.zhaomingkeji.xyz

[Q77] 时间加减
来源：http://oyh.redwolf501.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nrg.ywan-chungtsiang.top

[Q78] 当前时间
来源：http://mxb.xinyue.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lzs.chenjidiqi.icu

[Q79] 字符串拼接
来源：http://eoi.nanxinkj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rnu.jianghu66.top

[Q80] 字符串截取
来源：http://wgj.yj20258888.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sbi.jinqigufen.top

[Q81] 字符串替换
来源：http://ycq.hnxiangtu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://omj.jlsjyb.cn

[Q82] 字符长度与字节长度
来源：http://iez.jlsjyb.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ved.gotoacloud.top

[Q83] 大小写转换
来源：http://cna.jianghu66.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kar.chenlongwang.top

[Q84] 去除首尾空格
来源：http://nvk.jianghu66.top

SELECT TRIM(name) FROM users;
来源：http://bvy.wangshuangyany.cn

[Q85] 数值取整
来源：http://sok.ehwqpu.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bdx.jinghuilouyu.cn

[Q86] 读取 JSON 字段
来源：http://vwu.hcnkem.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yqi.yvedp.cn

[Q87] JSON 字段做条件
来源：http://tbq.gotoacloud.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hmo.epnwcf.com

[Q88] 行转列（条件聚合）
来源：http://ldq.jiagoushi.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bmz.cqqwz.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xsu.chenzaomai.com

[Q89] 判断表是否存在
来源：http://ucn.hesvh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ltb.guannengcc.top

[Q90] 生成序号列
来源：http://hvl.yfazqb.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cvq.yueranfly.top

================================================================================
来源：http://mkj.yueranfly.top

R. Bash 专题
来源：http://kwh.jinqigfzy.top

================================================================================
来源：http://qrb.hnqzz.top

[R01] shebang 与严格模式
来源：http://djp.yj202588.top

#!/usr/bin/env bash
来源：http://evv.c1oappe.top

set -euo pipefail
来源：http://auu.hammf.cn

[R02] 变量赋值与使用
来源：http://nrj.aibaodan.cn

name="Tom"; echo "$name"
来源：http://zkf.sufxvd.cn

[R03] 只读变量
来源：http://sbc.ehwqpu.com

readonly PI=3.14
来源：http://rcr.haohaochexian.top

[R04] 位置参数
来源：http://kst.gzhubu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kah.zhiwuduotai.top

[R05] 参数默认值
来源：http://xgw.sxryk.cn

name="${1:-default}"
来源：http://gjw.tianlin.xyz

[R06] 判断命令是否存在
来源：http://zqt.c1oappe.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ian.hnqzz.top

[R07] if 判断文件
来源：http://zbi.uphjek.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ebp.0kj1m.cn

[R08] 数值比较
来源：http://lhu.xingfuxueyuan.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://tix.xinyue.icu

[R09] 字符串比较
来源：http://wda.52xcode.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jux.yj20258.top

[R10] 正则匹配
来源：http://cbm.bjfxy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bwn.quarkkingdee.top

[R11] case 多分支
来源：http://mjy.xinyue.icu

case "$1" in
来源：http://maa.316326.xyz

start) echo "启动" ;;
来源：http://tnc.havefunace.top

stop)  echo "停止" ;;
来源：http://rrc.jqgufenzy.top

*)     echo "未知命令" ;;
来源：http://fgm.zhengqikj.top

esac
来源：http://xla.nanxuanxn.top

[R12] for 遍历文件
来源：http://dqq.jyoumei.cn

for f in *.txt; do echo "$f"; done
来源：http://uae.yongpay.top

[R13] for 计数循环
来源：http://eta.xylfe.cn

for i in {1..10}; do echo "$i"; done
来源：http://owt.yangfankeji.com

[R14] C 风格 for
来源：http://mvf.c1oappe.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kmm.jinqigufen.top

[R15] while 逐行读文件
来源：http://hve.chenjidiqi.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pei.haohaochexian.top

[R16] until 等待条件
来源：http://fpb.sxryk.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hwr.tianlin.xyz

[R17] 数组定义与取值
来源：http://ijt.tarul.cn

arr=(a b c); echo "${arr[0]}"
来源：http://iif.gotoacloud.top

[R18] 遍历数组
来源：http://wrv.zhongyouzk.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lpl.gaohongyu789.top

[R19] 数组长度
来源：http://mbb.ydzc1.top

echo "${#arr[@]}"
来源：http://vfw.fengsongda.top

[R20] 关联数组（字典）
来源：http://fjo.xinyue.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vse.xingfuxueyuan.xyz

[R21] 字符串长度
来源：http://uxq.feifeiyinyue.top

echo "${#s}"
来源：http://epy.kuanghao11.cn

[R22] 截取子串
来源：http://yzl.9152youxi.cn

echo "${s:0:5}"
来源：http://kwa.zycfv.cn

[R23] 字符串替换
来源：http://bus.jiagoushi.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://esn.xinyue.icu

[R24] 大小写转换
来源：http://pce.yj202588.top

echo "${s^^}"; echo "${s,,}"
来源：http://crn.jyoumei.cn

[R25] 去后缀 / 去前缀
来源：http://jgc.jlsjyb.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ehs.dianchejie.cn

[R26] 命令替换
来源：http://nxr.shanyushiyangkeji.top

now=$(date +%F); echo "$now"
来源：http://hjt.9152youxi.cn

[R27] 算术展开
来源：http://fgj.chenlongwang.top

echo $((1 + 2 * 3))
来源：http://bpj.chenzaomai.com

[R28] 浮点运算
来源：http://tkh.zhoulong.xyz

echo "scale=2; 10/3" | bc
来源：http://bvs.iojbl.cn

[R29] 定义函数
来源：http://pqn.vqdsnc.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fgf.shzxlz.cn

[R30] 函数返回状态码
来源：http://nsh.fzhhl.top

f() { return 0; }; f || echo "失败了"
来源：http://ges.yj202588.top

[R31] 局部变量
来源：http://kqe.52xcode.cn

f() { local x=1; echo "$x"; }
来源：http://ohf.hcnkem.com

[R32] 参数个数校验
来源：http://iac.fehbvm.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://obl.yanxiufei.cn

[R33] 捕获错误并提示行号
来源：http://sta.tian-w.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://luh.meibo888.top

[R34] 退出时清理
来源：http://uzc.jiagoushi.top

trap 'rm -f "$tmp"' EXIT
来源：http://wyo.andypj.xyz

[R35] 后台执行并等待
来源：http://yds.yfazqb.com

sleep 5 & pid=$!; wait "$pid"
来源：http://uja.tanke756.top

[R36] 并发执行多个任务
来源：http://ubm.yuxming.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qtg.jinqigufen.top

[R37] 把输出赋给变量
来源：http://ojc.xylfe.cn

files=$(ls -1)
来源：http://fzu.cucudq.cn

[R38] 管道串联
来源：http://koo.jlsjyb.cn

cat a.txt | grep -i error | wc -l
来源：http://syu.xuetiantiany.cn

[R39] 重定向标准输出与错误
来源：http://gel.sufxvd.cn

cmd > out.log 2>&1
来源：http://ooj.chenzaomai.com

[R40] 追加写日志
来源：http://fmw.ybcxt.top

echo "log" >> out.log
来源：http://ogy.aizwys.cn

[R41] 丢弃输出
来源：http://dsd.epnwcf.com

cmd >/dev/null 2>&1
来源：http://fsa.meibo888.top

[R42] 输入重定向
来源：http://fet.hesvh.cn

wc -l < a.txt
来源：http://kbq.gogol.net.cn

[R43] 按名字查找文件
来源：http://pqb.fengsongda.top

find . -name "*.log" -type f
来源：http://muh.yvedp.cn

[R44] 按修改时间查找
来源：http://usr.jinqigfzy.top

find . -mtime -7 -type f
来源：http://yvl.xinyue.icu

[R45] 批量删除
来源：http://wge.yongpay.top

find . -name "*.tmp" -delete
来源：http://gev.hongshengwenyu.top

[R46] 递归替换文件内容
来源：http://wch.gotoacloud.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dte.xuetiantiany.cn

[R47] sed 单行替换
来源：http://thy.daria6918.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nhi.snrcjt.cn

[R48] awk 取指定列
来源：http://sqa.jqgufenzy.top

awk '{print $1, $3}' a.txt
来源：http://vss.c1oappe.top

[R49] awk 带条件
来源：http://uas.hammf.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ayp.fehbvm.com

[R50] awk 求和
来源：http://ioc.tian-w.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yzk.yj20258888.top

[R51] 排序去重取前几
来源：http://gzv.hongshengwenyu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://lbq.guannengcc.top

[R52] 统计行数
来源：http://aes.mhx1999.top

wc -l a.txt
来源：http://nab.wangdashe.top

[R53] 查看文件头与实时尾
来源：http://atx.sjlbkw.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://aeg.yvedp.cn

[R54] 比较两个文件
来源：http://xzo.zycfv.cn

diff a.txt b.txt
来源：http://dog.nwbrower.top

[R55] 压缩与解压
来源：http://kji.yueranfly.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qqa.gaohongyu789.top

[R56] 远程拷贝
来源：http://vsg.52xcode.cn

scp file user@host:/path/
来源：http://ltk.nanxinkj.top

[R57] 远程执行命令
来源：http://eyx.haohaochexian.top

ssh user@host 'uptime'
来源：http://mcg.gzhubu.top

[R58] 下载文件
来源：http://tyq.gogol.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dzb.52xcode.cn

[R59] 发 POST JSON
来源：http://lub.yj202588.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tpp.xziqi.cn

[R60] 只看 HTTP 状态码
来源：http://wmg.yj20258888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hri.chenzaomai.com

[R61] 磁盘占用
来源：http://kze.shuidangran.top

df -h;  du -sh *
来源：http://wks.iojbl.cn

[R62] 找最占空间的文件
来源：http://sqq.hfpthk.cn

du -ah . | sort -rh | head -10
来源：http://ccp.9152youxi.cn

[R63] 内存与进程
来源：http://jnq.yfazqb.com

free -h;  ps aux | grep nginx
来源：http://mnn.aizwys.cn

[R64] 结束进程
来源：http://xrx.zhixingplan.top

kill -9 $(pgrep -f app.py)
来源：http://xcb.fanxiaobao.xyz

[R65] 查看端口占用
来源：http://hya.bbcook.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://imk.hcnkem.com

[R66] 定时任务
来源：http://edw.dashuyun.cn

crontab -e;  crontab -l
来源：http://luu.hnqzz.top

[R67] 生成随机十六进制串
来源：http://hev.sweek.top

openssl rand -hex 16
来源：http://lkb.bbcook.cn

[R68] 计算文件校验值
来源：http://gia.ybcxt.top

sha256sum a.txt;  md5sum a.txt
来源：http://tfo.cashguo.top

[R69] 生成随机密码
来源：http://axo.yonumen.top

head -c 16 /dev/urandom | base64
来源：http://lkh.xylfe.cn

[R70] 时间戳与互转
来源：http://occ.yuanzhike.top

date +%s;  date -d @1700000000
来源：http://uiv.hcnkem.com

[R71] 日期格式化
来源：http://ioh.sweek.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xrh.hammf.cn

[R72] 等待端口就绪
来源：http://rdx.fehbvm.com

until nc -z localhost 3306; do sleep 1; done
来源：http://xhm.xylfe.cn

[R73] 分割大日志
来源：http://tnv.sxryk.cn

split -l 1000 big.log part_
来源：http://bvw.nanxuanxn.top

[R74] 批量重命名
来源：http://slz.andypj.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pkp.tianlin.xyz

[R75] 导出环境变量
来源：http://kfb.yonumen.top

export PATH="$HOME/bin:$PATH"
来源：http://ouj.9152youxi.cn

[R76] 使用临时文件
来源：http://rte.cheryme.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://isj.cheryme.top

[R77] 读取用户输入
来源：http://way.zhengqikj.top

read -rp "请输入: " ans
来源：http://nsw.cashguo.top

[R78] 交互式菜单
来源：http://nzs.ppjwa.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vkm.0kj1m.cn

[R79] 解析命令行选项
来源：http://ynz.havefunace.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://whp.cdnleiting.top

[R80] 查看脚本执行耗时
来源：http://zqt.yongpay.top

time ./run.sh
来源：http://fzn.dashuyun.cn

================================================================================
来源：http://vxl.haohaochexian.top

S. C / C++ 专题
来源：http://bcu.zhijiandao.cn

================================================================================
来源：http://mpq.aibaodan.cn

[S01] C：Hello World
来源：http://oxi.cashguo.top

#include <stdio.h>
来源：http://ioj.zhixingplan.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://kfs.c1oappe.top

[S02] C：变量与格式化输出
来源：http://nfk.fanxiaobao.xyz

int a = 10; printf("%d\n", a);
来源：http://iwp.yj20258.top

[S03] C：读入整数
来源：http://ptg.yongpay.top

int x; scanf("%d", &x);
来源：http://uil.ehwqpu.com

[S04] C：字符串复制
来源：http://gri.dashuyun.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qxq.cashguo.top

[S05] C：字符串长度
来源：http://nhc.jqgufenzy.top

strlen(s)
来源：http://gor.9152youxi.cn

[S06] C：字符串比较
来源：http://wlp.zhiwuduotai.top

strcmp(a, b) == 0
来源：http://veo.zhoulong.xyz

[S07] C：数组遍历求和
来源：http://guq.hammf.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xko.ywan-chungtsiang.top

[S08] C：动态内存分配与释放
来源：http://wnu.jianghu66.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://aaw.wangdashe.top

[S09] C：结构体定义与初始化
来源：http://dco.yonumen.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cok.jinyuanbaomall.cn

[S10] C：指针与解引用
来源：http://qvs.sjlbkw.cn

int *p = &a;  *p = 5;
来源：http://qlh.hfpthk.cn

[S11] C：逐行读文件
来源：http://qyg.pengpengdd.cyou

FILE *f = fopen("a.txt", "r");
来源：http://rzt.zhongyouzk.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qgl.redwolf501.top

fclose(f);
来源：http://atw.jyoumei.cn

[S12] C：写文件
来源：http://zjt.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cou.hcnkem.com

[S13] C：宏定义
来源：http://mgt.yongpay.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nkb.cheryme.top

[S14] C：枚举
来源：http://kcj.wangshuangyany.cn

enum Color { RED, GREEN, BLUE };
来源：http://gkh.cucudq.cn

[S15] C：类型转换
来源：http://jio.cucudq.cn

(double) a / b
来源：http://nte.ppjwa.cn

[S16] C：位操作置位
来源：http://umo.jinghuilouyu.cn

x |= (1 << 3);
来源：http://vkc.dashuyun.cn

[S17] C：安全拼接字符串
来源：http://nbd.svipenyu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ftv.shuidangran.top

[S18] C：命令行参数
来源：http://jxp.gaohongyu789.top

int main(int argc, char **argv)
来源：http://vjm.zhoulong.xyz

[S19] C：快速排序
来源：http://ify.zhengqikj.top

qsort(a, n, sizeof(int), cmp);
来源：http://lbs.fengsongda.top

[S20] C：二分查找
来源：http://psj.guowangkeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hyr.fehbvm.com

[S21] C：字符类别判断
来源：http://fzy.hcnkem.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vtr.jinyuanbaomall.cn

[S22] C：字符串转数字
来源：http://bbb.ywan-chungtsiang.top

atoi("42");  strtod("3.14", NULL);
来源：http://xyn.meibo888.top

[S23] C：随机数
来源：http://org.tianlin.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://fjq.daria6918.cn

[S24] C：获取本地时间
来源：http://uvg.dianchejie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vdq.316326.xyz

[S25] C：内存拷贝
来源：http://hsu.jinyuanbaomall.cn

memcpy(dst, src, n);
来源：http://vlf.nanxinkj.top

[S26] C：内存清零
来源：http://fgo.uphjek.com

memset(a, 0, sizeof a);
来源：http://dgk.hnqzz.top

[S27] C：定义常量
来源：http://xgy.wangshuangyany.cn

const double PI = 3.14159;
来源：http://wqu.xziqi.cn

[S28] C：静态变量
来源：http://uok.wangdashe.top

static int counter = 0;
来源：http://mzk.hywenlv.cn

[S29] C：变参函数
来源：http://qkr.havefunace.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://trl.tianlin.xyz

[S30] C：头文件保护
来源：http://rnt.jinghuilouyu.cn

#ifndef X_H
来源：http://ciz.wangdashe.top

#define X_H
来源：http://uuy.cheryme.top

#endif
来源：http://ryw.ppjwa.cn

[S31] C++：Hello World
来源：http://drp.feifeiyinyue.top

#include <iostream>
来源：http://ymd.zhengqikj.top

int main() { std::cout << "Hello\n"; }
来源：http://mqv.cucudq.cn

[S32] C++：字符串
来源：http://cmk.zdqjudy.top

std::string s = "hi";  s += "!";
来源：http://gan.wangshuangyany.cn

[S33] C++：vector 增删
来源：http://lle.yj202588.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rmb.ydjk.org.cn

[S34] C++：遍历 vector
来源：http://osm.fehbvm.com

for (auto &x : v) { std::cout << x; }
来源：http://smd.bbcook.cn

[S35] C++：map
来源：http://qlb.fehbvm.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ajv.jiagoushi.top

[S36] C++：unordered_map
来源：http://rrw.cashguo.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pcy.cashguo.top


<!-- 参考信息 -->