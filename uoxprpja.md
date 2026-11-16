代发 wailian999

[Q63] 开启事务
来源：http://jzu.hnxiangtu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gll.ehwqpu.com

[Q64] 提交事务
来源：http://jyl.shuidangran.top

COMMIT;
来源：http://wwh.yfazqb.com

[Q65] 回滚事务
来源：http://sst.zhaomingkeji.xyz

ROLLBACK;
来源：http://rtl.xinyue.icu

[Q66] 行锁查询
来源：http://mnx.xingfuxueyuan.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mse.hnxiangtu.top

[Q67] 设置隔离级别
来源：http://buf.hesvh.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jea.ydjk.org.cn

[Q68] 保存点
来源：http://xae.xinyue.icu

SAVEPOINT sp1;
来源：http://jxo.ydjk.org.cn

ROLLBACK TO sp1;
来源：http://xtv.zhongyouzk.top

[Q69] 查看执行计划
来源：http://ika.pengpengdd.cyou

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vol.ywan-chungtsiang.top

[Q70] 更新统计信息
来源：http://fsr.cqqwz.cn

ANALYZE TABLE users;
来源：http://wyf.xziqi.cn

[Q71] 查看建表语句
来源：http://eao.chenjidiqi.icu

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eby.cucudq.cn

[Q72] 查看索引
来源：http://zro.bbcook.cn

SHOW INDEX FROM users;
来源：http://pmi.ivvv.top

[Q73] 查看表状态
来源：http://nvl.kuanghao11.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://goi.jiagoushi.top

[Q74] 强制使用索引
来源：http://buw.yongpay.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zah.meibo888.top

[Q75] 日期格式化
来源：http://qzy.cucudq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://krw.guannengcc.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bza.andypj.xyz

[Q76] 按天统计
来源：http://ckm.nwbrower.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tsc.hnxiangtu.top

[Q77] 时间加减
来源：http://amx.cashguo.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lhb.zhengqikj.top

[Q78] 当前时间
来源：http://edj.pengpengdd.cyou

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zrq.wangshuangyany.cn

[Q79] 字符串拼接
来源：http://hwz.fktsv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pjq.0kj1m.cn

[Q80] 字符串截取
来源：http://vhp.gogol.net.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://smh.bbcook.cn

[Q81] 字符串替换
来源：http://exf.tianlin.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://oou.jinqigfzy.top

[Q82] 字符长度与字节长度
来源：http://zlo.yuxming.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cup.sysykeji.top

[Q83] 大小写转换
来源：http://kvw.gotoacloud.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://iay.c1oappe.top

[Q84] 去除首尾空格
来源：http://rpx.yonumen.top

SELECT TRIM(name) FROM users;
来源：http://bqd.zycfv.cn

[Q85] 数值取整
来源：http://yxc.sxryk.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wgm.chenzaomai.com

[Q86] 读取 JSON 字段
来源：http://ivh.cqqwz.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sjj.zhoulong.xyz

[Q87] JSON 字段做条件
来源：http://gko.iojbl.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uyw.sufxvd.cn

[Q88] 行转列（条件聚合）
来源：http://tpx.sjlbkw.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vok.gotoacloud.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oax.bjfxy.top

[Q89] 判断表是否存在
来源：http://qts.cqqwz.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wit.sjlbkw.cn

[Q90] 生成序号列
来源：http://ruc.shuidangran.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://que.gaohongyu789.top

================================================================================
来源：http://ubf.jinqigufen.top

R. Bash 专题
来源：http://qqm.jlsjyb.cn

================================================================================
来源：http://upz.tianlin.xyz

[R01] shebang 与严格模式
来源：http://uoe.hesvh.cn

#!/usr/bin/env bash
来源：http://njn.xinyue.icu

set -euo pipefail
来源：http://qzp.yangfankeji.com

[R02] 变量赋值与使用
来源：http://tot.yangfankeji.com

name="Tom"; echo "$name"
来源：http://aiw.pycfn.com

[R03] 只读变量
来源：http://vqs.xingfuxueyuan.xyz

readonly PI=3.14
来源：http://czt.yj20258.top

[R04] 位置参数
来源：http://lbz.yfazqb.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lxj.ydjk.org.cn

[R05] 参数默认值
来源：http://ybk.sjlbkw.cn

name="${1:-default}"
来源：http://wal.fktsv.cn

[R06] 判断命令是否存在
来源：http://zna.hcnkem.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rms.dashuyun.cn

[R07] if 判断文件
来源：http://xnx.hesvh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ozb.bbcook.cn

[R08] 数值比较
来源：http://upf.yuanzhike.top

if (( a > b )); then echo "a 更大"; fi
来源：http://mas.daxiang520.top

[R09] 字符串比较
来源：http://ymj.cqqwz.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zcg.shuidangran.top

[R10] 正则匹配
来源：http://tqb.zdbjq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ahq.jlsjyb.cn

[R11] case 多分支
来源：http://bcs.316326.xyz

case "$1" in
来源：http://hkm.wangshuangyany.cn

start) echo "启动" ;;
来源：http://erz.hongshengwenyu.top

stop)  echo "停止" ;;
来源：http://chc.xinyue.icu

*)     echo "未知命令" ;;
来源：http://qxe.fehbvm.com

esac
来源：http://ogx.zhixingplan.top

[R12] for 遍历文件
来源：http://qkm.yvedp.cn

for f in *.txt; do echo "$f"; done
来源：http://ekb.jqgufenzy.top

[R13] for 计数循环
来源：http://vir.xuetiantiany.cn

for i in {1..10}; do echo "$i"; done
来源：http://lad.smart0.xyz

[R14] C 风格 for
来源：http://nvs.sufxvd.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pec.fktsv.cn

[R15] while 逐行读文件
来源：http://ewh.nanxuanxn.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ova.xuetiantiany.cn

[R16] until 等待条件
来源：http://uaw.nanxuanxn.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://flz.gogol.net.cn

[R17] 数组定义与取值
来源：http://wvn.gotoacloud.top

arr=(a b c); echo "${arr[0]}"
来源：http://dud.wangshuangyany.cn

[R18] 遍历数组
来源：http://jym.xinyue.icu

for x in "${arr[@]}"; do echo "$x"; done
来源：http://szd.shangyingyoupin.top

[R19] 数组长度
来源：http://kiz.guannengcc.top

echo "${#arr[@]}"
来源：http://mer.bjfxy.top

[R20] 关联数组（字典）
来源：http://son.yonumen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wxr.epnwcf.com

[R21] 字符串长度
来源：http://rrj.hnxiangtu.top

echo "${#s}"
来源：http://drc.yj20258.top

[R22] 截取子串
来源：http://dxg.ywan-chungtsiang.top

echo "${s:0:5}"
来源：http://bju.ehwqpu.com

[R23] 字符串替换
来源：http://kxf.kuanghao11.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dzi.jiagoushi.top

[R24] 大小写转换
来源：http://yrw.316326.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://olt.hywenlv.cn

[R25] 去后缀 / 去前缀
来源：http://lei.gaohongyu789.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://tqr.yangfankeji.com

[R26] 命令替换
来源：http://gzp.316326.xyz

now=$(date +%F); echo "$now"
来源：http://wve.zycfv.cn

[R27] 算术展开
来源：http://rau.havefunace.top

echo $((1 + 2 * 3))
来源：http://ezp.9152youxi.cn

[R28] 浮点运算
来源：http://llc.wangdashe.top

echo "scale=2; 10/3" | bc
来源：http://evv.redwolf501.top

[R29] 定义函数
来源：http://caj.cqqwz.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wjy.yonumen.top

[R30] 函数返回状态码
来源：http://xdh.guowangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://cfk.chenlongwang.top

[R31] 局部变量
来源：http://lrw.hammf.cn

f() { local x=1; echo "$x"; }
来源：http://muc.cdnleiting.top

[R32] 参数个数校验
来源：http://tnb.yongpay.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xps.zhaomingkeji.xyz

[R33] 捕获错误并提示行号
来源：http://fqk.aizwys.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bxc.xuanzx.com

[R34] 退出时清理
来源：http://xht.shuidangran.top

trap 'rm -f "$tmp"' EXIT
来源：http://sbn.fzhhl.top

[R35] 后台执行并等待
来源：http://vsv.gotoacloud.top

sleep 5 & pid=$!; wait "$pid"
来源：http://zdl.mhx1999.top

[R36] 并发执行多个任务
来源：http://rwb.zhaomingkeji.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lin.hysaishi.cn

[R37] 把输出赋给变量
来源：http://fnr.zhongyouzk.top

files=$(ls -1)
来源：http://tcc.zhoulong.xyz

[R38] 管道串联
来源：http://nyq.52xcode.cn

cat a.txt | grep -i error | wc -l
来源：http://ttj.jinghuilouyu.cn

[R39] 重定向标准输出与错误
来源：http://pfj.aizwys.cn

cmd > out.log 2>&1
来源：http://wrx.aizwys.cn

[R40] 追加写日志
来源：http://cks.fzhhl.top

echo "log" >> out.log
来源：http://rtt.zdqjudy.top

[R41] 丢弃输出
来源：http://jjo.daxiang520.top

cmd >/dev/null 2>&1
来源：http://lkt.ivvv.top

[R42] 输入重定向
来源：http://qvw.hywenlv.cn

wc -l < a.txt
来源：http://zgo.yongpay.top

[R43] 按名字查找文件
来源：http://pmu.zhiwuduotai.top

find . -name "*.log" -type f
来源：http://vsy.hcnkem.com

[R44] 按修改时间查找
来源：http://rmr.yueranfly.top

find . -mtime -7 -type f
来源：http://xgv.cucudq.cn

[R45] 批量删除
来源：http://nvr.smart0.xyz

find . -name "*.tmp" -delete
来源：http://ekb.sweek.top

[R46] 递归替换文件内容
来源：http://jdt.yuanzhike.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://frt.jinqigfzy.top

[R47] sed 单行替换
来源：http://bba.jqgfzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://gjh.zhengqikj.top

[R48] awk 取指定列
来源：http://fls.yangfankeji.com

awk '{print $1, $3}' a.txt
来源：http://cxs.birdmap.top

[R49] awk 带条件
来源：http://ups.gotoacloud.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jbo.hywenlv.cn

[R50] awk 求和
来源：http://fns.fehbvm.com

awk '{s += $2} END {print s}' a.txt
来源：http://rwf.daria6918.cn

[R51] 排序去重取前几
来源：http://wgh.yj20258.top

sort a.txt | uniq -c | sort -rn | head
来源：http://mpm.jinghuilouyu.cn

[R52] 统计行数
来源：http://llr.zdbjq.cn

wc -l a.txt
来源：http://vjc.xingfuxueyuan.xyz

[R53] 查看文件头与实时尾
来源：http://xud.ctjpmb.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dzh.gaohongyu789.top

[R54] 比较两个文件
来源：http://oyj.ehwqpu.com

diff a.txt b.txt
来源：http://uab.jinghuilouyu.cn

[R55] 压缩与解压
来源：http://tnk.hfpthk.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://neb.zhixingplan.top

[R56] 远程拷贝
来源：http://dqf.birdmap.top

scp file user@host:/path/
来源：http://jsa.epnwcf.com

[R57] 远程执行命令
来源：http://zha.dashuyun.cn

ssh user@host 'uptime'
来源：http://wjd.yj202588.top

[R58] 下载文件
来源：http://adj.jiagoushi.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://acc.haohaochexian.top

[R59] 发 POST JSON
来源：http://uqt.cheryme.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fmq.yanxiufei.cn

[R60] 只看 HTTP 状态码
来源：http://lhj.birdmap.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hur.hywenlv.cn

[R61] 磁盘占用
来源：http://ppr.xinyue.icu

df -h;  du -sh *
来源：http://jsf.ydzc1.top

[R62] 找最占空间的文件
来源：http://tuh.52xcode.cn

du -ah . | sort -rh | head -10
来源：http://mdk.iojbl.cn

[R63] 内存与进程
来源：http://jew.gzhubu.top

free -h;  ps aux | grep nginx
来源：http://pnt.tian-w.cn

[R64] 结束进程
来源：http://pxh.ydzc1.top

kill -9 $(pgrep -f app.py)
来源：http://wph.xylfe.cn

[R65] 查看端口占用
来源：http://hpk.shangyingyoupin.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sin.jinqigufen.top

[R66] 定时任务
来源：http://bzg.xingfuxueyuan.xyz

crontab -e;  crontab -l
来源：http://nrm.smart0.xyz

[R67] 生成随机十六进制串
来源：http://srl.sxryk.cn

openssl rand -hex 16
来源：http://ujw.epnwcf.com

[R68] 计算文件校验值
来源：http://ctc.ehwqpu.com

sha256sum a.txt;  md5sum a.txt
来源：http://vav.xinyue.icu

[R69] 生成随机密码
来源：http://vqg.aizwys.cn

head -c 16 /dev/urandom | base64
来源：http://djc.pycfn.com

[R70] 时间戳与互转
来源：http://kqv.hfpthk.cn

date +%s;  date -d @1700000000
来源：http://dud.jqgufenzy.top

[R71] 日期格式化
来源：http://wxv.zhiwuduotai.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ckh.meibo888.top

[R72] 等待端口就绪
来源：http://wsq.sysykeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://min.yonumen.top

[R73] 分割大日志
来源：http://ntd.haohaochexian.top

split -l 1000 big.log part_
来源：http://xxn.ivvv.top

[R74] 批量重命名
来源：http://ihg.9152youxi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bza.wangdashe.top

[R75] 导出环境变量
来源：http://fea.chenlongwang.top

export PATH="$HOME/bin:$PATH"
来源：http://rqh.mhx1999.top

[R76] 使用临时文件
来源：http://yix.zhixingplan.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ufe.yuxming.cn

[R77] 读取用户输入
来源：http://hip.0kj1m.cn

read -rp "请输入: " ans
来源：http://rgv.vqdsnc.cn

[R78] 交互式菜单
来源：http://djc.hammf.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://oqv.hesvh.cn

[R79] 解析命令行选项
来源：http://olm.yongpay.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ujx.hongshengwenyu.top

[R80] 查看脚本执行耗时
来源：http://aoj.shanyushiyangkeji.top

time ./run.sh
来源：http://isg.quarkkingdee.top

================================================================================
来源：http://gzd.hcnkem.com

S. C / C++ 专题
来源：http://vmb.52xcode.cn

================================================================================
来源：http://vec.zdbjq.cn

[S01] C：Hello World
来源：http://guz.c1oappe.top

#include <stdio.h>
来源：http://xgo.svipenyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://com.meibo888.top

[S02] C：变量与格式化输出
来源：http://hzo.uphjek.com

int a = 10; printf("%d\n", a);
来源：http://goe.cqqwz.cn

[S03] C：读入整数
来源：http://dbg.fanxiaobao.xyz

int x; scanf("%d", &x);
来源：http://ibs.haohaochexian.top

[S04] C：字符串复制
来源：http://twc.gogol.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jjg.havefunace.top

[S05] C：字符串长度
来源：http://rxt.hnxiangtu.top

strlen(s)
来源：http://oqy.chenzaomai.com

[S06] C：字符串比较
来源：http://red.cheryme.top

strcmp(a, b) == 0
来源：http://bjw.yangfankeji.com

[S07] C：数组遍历求和
来源：http://tel.feifeiyinyue.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bda.xinyue.icu

[S08] C：动态内存分配与释放
来源：http://zjz.yangfankeji.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://adi.zhaomingkeji.xyz

[S09] C：结构体定义与初始化
来源：http://rik.sufxvd.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rtu.jyoumei.cn

[S10] C：指针与解引用
来源：http://ixb.sysykeji.top

int *p = &a;  *p = 5;
来源：http://vso.yj202588.top

[S11] C：逐行读文件
来源：http://kza.jinqigfzy.top

FILE *f = fopen("a.txt", "r");
来源：http://uvn.ybcxt.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://tbl.zhoulong.xyz

fclose(f);
来源：http://ssa.smart0.xyz

[S12] C：写文件
来源：http://gah.yfazqb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vwh.tarul.cn

[S13] C：宏定义
来源：http://kox.hywenlv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://shl.yanxiufei.cn

[S14] C：枚举
来源：http://xmp.daxiang520.top

enum Color { RED, GREEN, BLUE };
来源：http://neu.jyoumei.cn

[S15] C：类型转换
来源：http://ari.birdmap.top

(double) a / b
来源：http://fpl.jlsjyb.cn

[S16] C：位操作置位
来源：http://dhd.jlsjyb.cn

x |= (1 << 3);
来源：http://tck.cucudq.cn

[S17] C：安全拼接字符串
来源：http://clv.redwolf501.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://exd.gotoacloud.top

[S18] C：命令行参数
来源：http://vag.jqgfzy.top

int main(int argc, char **argv)
来源：http://whe.tian-w.cn

[S19] C：快速排序
来源：http://gql.gzhubu.top

qsort(a, n, sizeof(int), cmp);
来源：http://eld.birdmap.top

[S20] C：二分查找
来源：http://slo.shuidangran.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ndo.sweek.top

[S21] C：字符类别判断
来源：http://hgr.ywan-chungtsiang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bvc.redwolf501.top

[S22] C：字符串转数字
来源：http://hqg.0kj1m.cn

atoi("42");  strtod("3.14", NULL);
来源：http://idy.tian-w.cn

[S23] C：随机数
来源：http://did.epnwcf.com

srand(time(NULL));  int r = rand() % 100;
来源：http://ycj.meibo888.top

[S24] C：获取本地时间
来源：http://vmb.aibaodan.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lmm.hywenlv.cn

[S25] C：内存拷贝
来源：http://vzz.quarkkingdee.top

memcpy(dst, src, n);
来源：http://bki.sysykeji.top

[S26] C：内存清零
来源：http://yqq.chenzaomai.com

memset(a, 0, sizeof a);
来源：http://lch.yongpay.top

[S27] C：定义常量
来源：http://lsc.bjfxy.top

const double PI = 3.14159;
来源：http://xgf.jinqigufen.top

[S28] C：静态变量
来源：http://nxd.yueranfly.top

static int counter = 0;
来源：http://aex.fktsv.cn

[S29] C：变参函数
来源：http://lcs.chenlongwang.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ybn.guannengcc.top

[S30] C：头文件保护
来源：http://qbt.hywenlv.cn

#ifndef X_H
来源：http://acx.yongpay.top

#define X_H
来源：http://ngn.daria6918.cn

#endif
来源：http://xzu.havefunace.top

[S31] C++：Hello World
来源：http://phz.pengpengdd.cyou

#include <iostream>
来源：http://olo.hysaishi.cn

int main() { std::cout << "Hello\n"; }
来源：http://qzy.sysykeji.top

[S32] C++：字符串
来源：http://xkv.jqgufenzy.top

std::string s = "hi";  s += "!";
来源：http://kjk.hammf.cn


<!-- 参考信息 -->