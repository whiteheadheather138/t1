代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bfx.bjfxy.top

[Q60] 取上一行 / 下一行
来源：http://yhe.fktsv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rvd.gogol.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mvt.ybcxt.top

[Q61] 移动平均
来源：http://ipk.chenjidiqi.icu

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qgj.zhixingplan.top

[Q62] 分组占比
来源：http://vfc.tanke756.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ndv.shangyingyoupin.top

[Q63] 开启事务
来源：http://uuz.daxiang520.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ilo.jinyuanbaomall.cn

[Q64] 提交事务
来源：http://spq.chenzaomai.com

COMMIT;
来源：http://jjv.chenlongwang.top

[Q65] 回滚事务
来源：http://kge.ydzc1.top

ROLLBACK;
来源：http://tlw.hnxiangtu.top

[Q66] 行锁查询
来源：http://oim.gogol.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://prl.tian-w.cn

[Q67] 设置隔离级别
来源：http://ppk.zdqjudy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ggo.uphjek.com

[Q68] 保存点
来源：http://idx.yuanzhike.top

SAVEPOINT sp1;
来源：http://ngi.dianchejie.cn

ROLLBACK TO sp1;
来源：http://nxf.ydjk.org.cn

[Q69] 查看执行计划
来源：http://laq.hywenlv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xab.cheryme.top

[Q70] 更新统计信息
来源：http://qxg.nwbrower.top

ANALYZE TABLE users;
来源：http://gtx.hnxiangtu.top

[Q71] 查看建表语句
来源：http://gdg.tanke756.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hon.tanke756.top

[Q72] 查看索引
来源：http://buv.yfazqb.com

SHOW INDEX FROM users;
来源：http://ate.cqqwz.cn

[Q73] 查看表状态
来源：http://jsa.tanke756.top

SHOW TABLE STATUS LIKE 'users';
来源：http://uyw.smart0.xyz

[Q74] 强制使用索引
来源：http://kpy.yuxming.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bwx.zhengqikj.top

[Q75] 日期格式化
来源：http://mfv.cdnleiting.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lir.ehwqpu.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kpa.ehwqpu.com

[Q76] 按天统计
来源：http://saf.ehwqpu.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fnb.fehbvm.com

[Q77] 时间加减
来源：http://zik.sufxvd.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zbe.zhijiandao.cn

[Q78] 当前时间
来源：http://tuh.hnxiangtu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gtw.gaohongyu789.top

[Q79] 字符串拼接
来源：http://due.316326.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xpw.zhaomingkeji.xyz

[Q80] 字符串截取
来源：http://ivt.wangdashe.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iec.chenjidiqi.icu

[Q81] 字符串替换
来源：http://ufd.0kj1m.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xwj.cucudq.cn

[Q82] 字符长度与字节长度
来源：http://zjv.xuanzx.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://chq.zhixingplan.top

[Q83] 大小写转换
来源：http://jor.yfazqb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zpi.hfpthk.cn

[Q84] 去除首尾空格
来源：http://uwu.yueranfly.top

SELECT TRIM(name) FROM users;
来源：http://cim.jinqigufen.top

[Q85] 数值取整
来源：http://tsw.sweek.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gzq.hywenlv.cn

[Q86] 读取 JSON 字段
来源：http://tnz.guannengcc.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://keo.9152youxi.cn

[Q87] JSON 字段做条件
来源：http://vvo.shangyingyoupin.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ywr.cucudq.cn

[Q88] 行转列（条件聚合）
来源：http://tjg.hysaishi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hcu.c1oappe.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cpd.wangshuangyany.cn

[Q89] 判断表是否存在
来源：http://cjh.guowangkeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fbw.yj20258.top

[Q90] 生成序号列
来源：http://bbn.shzxlz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://owc.epnwcf.com

================================================================================
来源：http://mzk.daria6918.cn

R. Bash 专题
来源：http://sym.xuetiantiany.cn

================================================================================
来源：http://ssl.feifeiyinyue.top

[R01] shebang 与严格模式
来源：http://wir.andypj.xyz

#!/usr/bin/env bash
来源：http://mhq.yuxming.cn

set -euo pipefail
来源：http://fsy.shanyushiyangtech.top

[R02] 变量赋值与使用
来源：http://wyd.hongshengwenyu.top

name="Tom"; echo "$name"
来源：http://naz.havefunace.top

[R03] 只读变量
来源：http://oka.shangyingyoupin.top

readonly PI=3.14
来源：http://ffw.shanyushiyangtech.top

[R04] 位置参数
来源：http://tgg.hfpthk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jsn.meibo888.top

[R05] 参数默认值
来源：http://dfo.redwolf501.top

name="${1:-default}"
来源：http://duh.316326.xyz

[R06] 判断命令是否存在
来源：http://rul.hysaishi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ixh.yueranfly.top

[R07] if 判断文件
来源：http://rnq.bbcook.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ici.birdmap.top

[R08] 数值比较
来源：http://ejb.vehdjk.com

if (( a > b )); then echo "a 更大"; fi
来源：http://xxg.jyoumei.cn

[R09] 字符串比较
来源：http://irz.yvedp.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hyx.aizwys.cn

[R10] 正则匹配
来源：http://ifu.cheryme.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ezt.ydzc1.top

[R11] case 多分支
来源：http://omp.guannengcc.top

case "$1" in
来源：http://kad.chenjidiqi.icu

start) echo "启动" ;;
来源：http://qrc.ywan-chungtsiang.top

stop)  echo "停止" ;;
来源：http://skn.jianghu66.top

*)     echo "未知命令" ;;
来源：http://gya.snrcjt.cn

esac
来源：http://oyt.xziqi.cn

[R12] for 遍历文件
来源：http://cke.daria6918.cn

for f in *.txt; do echo "$f"; done
来源：http://ebq.smart0.xyz

[R13] for 计数循环
来源：http://pkq.hesvh.cn

for i in {1..10}; do echo "$i"; done
来源：http://rbv.yj20258.top

[R14] C 风格 for
来源：http://uig.bjfxy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mcb.pengpengdd.cyou

[R15] while 逐行读文件
来源：http://chl.cheryme.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://krz.gzhubu.top

[R16] until 等待条件
来源：http://yqi.zdqjudy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vbl.yj20258888.top

[R17] 数组定义与取值
来源：http://szw.pengpengdd.cyou

arr=(a b c); echo "${arr[0]}"
来源：http://xwf.snrcjt.cn

[R18] 遍历数组
来源：http://zzf.pycfn.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pvi.quarkkingdee.top

[R19] 数组长度
来源：http://mdg.xuetiantiany.cn

echo "${#arr[@]}"
来源：http://yak.ivvv.top

[R20] 关联数组（字典）
来源：http://oow.xziqi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://llq.zhiwuduotai.top

[R21] 字符串长度
来源：http://qzz.cdnleiting.top

echo "${#s}"
来源：http://lhc.guowangkeji.top

[R22] 截取子串
来源：http://uqs.meibo888.top

echo "${s:0:5}"
来源：http://kxx.yj20258.top

[R23] 字符串替换
来源：http://kjt.zhongyouzk.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bej.uphjek.com

[R24] 大小写转换
来源：http://ydj.zycfv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wwn.cqqwz.cn

[R25] 去后缀 / 去前缀
来源：http://jon.316326.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://ocg.yj20258888.top

[R26] 命令替换
来源：http://fmu.fengsongda.top

now=$(date +%F); echo "$now"
来源：http://ynu.sxryk.cn

[R27] 算术展开
来源：http://vuw.meibo888.top

echo $((1 + 2 * 3))
来源：http://mvv.0kj1m.cn

[R28] 浮点运算
来源：http://hmd.andypj.xyz

echo "scale=2; 10/3" | bc
来源：http://anb.ydzc1.top

[R29] 定义函数
来源：http://wyo.zhaomingkeji.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://eki.chenjidiqi.icu

[R30] 函数返回状态码
来源：http://jdc.iojbl.cn

f() { return 0; }; f || echo "失败了"
来源：http://ecc.meibo888.top

[R31] 局部变量
来源：http://tao.yueranfly.top

f() { local x=1; echo "$x"; }
来源：http://rva.hysaishi.cn

[R32] 参数个数校验
来源：http://nyf.yvedp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rvc.kuanghao11.cn

[R33] 捕获错误并提示行号
来源：http://bat.cdnleiting.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dpj.c1oappe.top

[R34] 退出时清理
来源：http://fcw.bjfxy.top

trap 'rm -f "$tmp"' EXIT
来源：http://xgb.ehwqpu.com

[R35] 后台执行并等待
来源：http://njt.guowangkeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://brb.chenjidiqi.icu

[R36] 并发执行多个任务
来源：http://bsc.jiagoushi.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lam.bjfxy.top

[R37] 把输出赋给变量
来源：http://cie.316326.xyz

files=$(ls -1)
来源：http://htf.ywan-chungtsiang.top

[R38] 管道串联
来源：http://gca.sweek.top

cat a.txt | grep -i error | wc -l
来源：http://psr.shzxlz.cn

[R39] 重定向标准输出与错误
来源：http://fuc.aizwys.cn

cmd > out.log 2>&1
来源：http://erc.epnwcf.com

[R40] 追加写日志
来源：http://jfg.shanyushiyangtech.top

echo "log" >> out.log
来源：http://ysd.yj20258.top

[R41] 丢弃输出
来源：http://znx.ywan-chungtsiang.top

cmd >/dev/null 2>&1
来源：http://eca.guannengcc.top

[R42] 输入重定向
来源：http://sru.guannengcc.top

wc -l < a.txt
来源：http://qgm.xylfe.cn

[R43] 按名字查找文件
来源：http://yvv.yongpay.top

find . -name "*.log" -type f
来源：http://ant.ctjpmb.com

[R44] 按修改时间查找
来源：http://xaw.zdbjq.cn

find . -mtime -7 -type f
来源：http://mkd.ehwqpu.com

[R45] 批量删除
来源：http://aud.nanxinkj.top

find . -name "*.tmp" -delete
来源：http://qvk.jinyuanbaomall.cn

[R46] 递归替换文件内容
来源：http://bdx.cqqwz.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cur.sxryk.cn

[R47] sed 单行替换
来源：http://ejn.tarul.cn

sed -i 's/foo/bar/g' a.txt
来源：http://okx.yj20258.top

[R48] awk 取指定列
来源：http://qpn.jqgufenzy.top

awk '{print $1, $3}' a.txt
来源：http://tei.sweek.top

[R49] awk 带条件
来源：http://pqq.shanyushiyangkeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ron.jqgufenzy.top

[R50] awk 求和
来源：http://mmp.jinqigfzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://wot.sufxvd.cn

[R51] 排序去重取前几
来源：http://zzy.jinqigufen.top

sort a.txt | uniq -c | sort -rn | head
来源：http://fgn.vqdsnc.cn

[R52] 统计行数
来源：http://sgi.xylfe.cn

wc -l a.txt
来源：http://xiu.jyoumei.cn

[R53] 查看文件头与实时尾
来源：http://mbu.xuanzx.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iqu.fanxiaobao.xyz

[R54] 比较两个文件
来源：http://uyl.sxryk.cn

diff a.txt b.txt
来源：http://izh.xylfe.cn

[R55] 压缩与解压
来源：http://pbr.tianlin.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mmx.ppjwa.cn

[R56] 远程拷贝
来源：http://ogv.zhaomingkeji.xyz

scp file user@host:/path/
来源：http://ywv.shangyingyoupin.top

[R57] 远程执行命令
来源：http://nmw.gaohongyu789.top

ssh user@host 'uptime'
来源：http://dzt.jyoumei.cn

[R58] 下载文件
来源：http://scq.wangdashe.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://chf.svipenyu.cn

[R59] 发 POST JSON
来源：http://qmo.shuidangran.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pdj.yanxiufei.cn

[R60] 只看 HTTP 状态码
来源：http://cjk.chenzaomai.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://prs.ivvv.top

[R61] 磁盘占用
来源：http://bsw.zhiwuduotai.top

df -h;  du -sh *
来源：http://wom.vehdjk.com

[R62] 找最占空间的文件
来源：http://ysr.hfpthk.cn

du -ah . | sort -rh | head -10
来源：http://hmi.shzxlz.cn

[R63] 内存与进程
来源：http://ikf.cheryme.top

free -h;  ps aux | grep nginx
来源：http://pkc.hywenlv.cn

[R64] 结束进程
来源：http://fak.9152youxi.cn

kill -9 $(pgrep -f app.py)
来源：http://izn.hesvh.cn

[R65] 查看端口占用
来源：http://lje.ydjk.org.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mzh.cucudq.cn

[R66] 定时任务
来源：http://zbe.jinyuanbaomall.cn

crontab -e;  crontab -l
来源：http://dly.xuanzx.com

[R67] 生成随机十六进制串
来源：http://hro.yongpay.top

openssl rand -hex 16
来源：http://soq.cheryme.top

[R68] 计算文件校验值
来源：http://jzs.pycfn.com

sha256sum a.txt;  md5sum a.txt
来源：http://udq.jiagoushi.top

[R69] 生成随机密码
来源：http://ioo.hammf.cn

head -c 16 /dev/urandom | base64
来源：http://sbu.xuanzx.com

[R70] 时间戳与互转
来源：http://pam.cashguo.top

date +%s;  date -d @1700000000
来源：http://rej.hesvh.cn

[R71] 日期格式化
来源：http://wlm.c1oappe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ymb.yuxming.cn

[R72] 等待端口就绪
来源：http://hke.sysykeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://igb.guowangkeji.top

[R73] 分割大日志
来源：http://xnt.bjfxy.top

split -l 1000 big.log part_
来源：http://afc.zhiwuduotai.top

[R74] 批量重命名
来源：http://wcx.kuanghao11.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wqr.ybcxt.top

[R75] 导出环境变量
来源：http://olo.zdqjudy.top

export PATH="$HOME/bin:$PATH"
来源：http://ors.fktsv.cn

[R76] 使用临时文件
来源：http://juc.ctjpmb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dye.hywenlv.cn

[R77] 读取用户输入
来源：http://dsy.ppjwa.cn

read -rp "请输入: " ans
来源：http://eth.yongpay.top

[R78] 交互式菜单
来源：http://ser.jinghuilouyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://smv.pycfn.com

[R79] 解析命令行选项
来源：http://ogq.smart0.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eee.fzhhl.top

[R80] 查看脚本执行耗时
来源：http://tbm.shangyingyoupin.top

time ./run.sh
来源：http://dhz.xuetiantiany.cn

================================================================================
来源：http://clc.jianghu66.top

S. C / C++ 专题
来源：http://rxg.chenzaomai.com

================================================================================
来源：http://wpi.0kj1m.cn

[S01] C：Hello World
来源：http://dic.zhiwuduotai.top

#include <stdio.h>
来源：http://xcc.tian-w.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pwg.feifeiyinyue.top

[S02] C：变量与格式化输出
来源：http://bhv.fzhhl.top

int a = 10; printf("%d\n", a);
来源：http://jef.havefunace.top

[S03] C：读入整数
来源：http://faa.wangshuangyany.cn

int x; scanf("%d", &x);
来源：http://swd.haohaochexian.top

[S04] C：字符串复制
来源：http://tgk.xylfe.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fkc.fehbvm.com

[S05] C：字符串长度
来源：http://ads.zhongyouzk.top

strlen(s)
来源：http://kjs.xylfe.cn

[S06] C：字符串比较
来源：http://qxn.sufxvd.cn

strcmp(a, b) == 0
来源：http://dul.jinqigufen.top

[S07] C：数组遍历求和
来源：http://mpb.aibaodan.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bvz.hywenlv.cn

[S08] C：动态内存分配与释放
来源：http://fhq.hnqzz.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vho.sxryk.cn

[S09] C：结构体定义与初始化
来源：http://nie.yongpay.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kkx.yongpay.top

[S10] C：指针与解引用
来源：http://rbh.daria6918.cn

int *p = &a;  *p = 5;
来源：http://zdp.gaohongyu789.top

[S11] C：逐行读文件
来源：http://nps.quarkkingdee.top

FILE *f = fopen("a.txt", "r");
来源：http://uzm.jinghuilouyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wni.shangyingyoupin.top

fclose(f);
来源：http://ike.hysaishi.cn

[S12] C：写文件
来源：http://mwf.pengpengdd.cyou

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qnq.zhijiandao.cn

[S13] C：宏定义
来源：http://mch.ppjwa.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nea.gotoacloud.top

[S14] C：枚举
来源：http://fjs.shuidangran.top

enum Color { RED, GREEN, BLUE };
来源：http://ehs.hnxiangtu.top

[S15] C：类型转换
来源：http://fhy.yonumen.top

(double) a / b
来源：http://eaq.daxiang520.top

[S16] C：位操作置位
来源：http://jut.vehdjk.com

x |= (1 << 3);
来源：http://hrz.hongshengwenyu.top

[S17] C：安全拼接字符串
来源：http://hfl.jlsjyb.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wqm.yj20258.top

[S18] C：命令行参数
来源：http://quy.ivvv.top

int main(int argc, char **argv)
来源：http://gox.yueranfly.top

[S19] C：快速排序
来源：http://sxt.52xcode.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ofg.uphjek.com

[S20] C：二分查找
来源：http://ean.shuidangran.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qjh.ybcxt.top

[S21] C：字符类别判断
来源：http://mmc.sysykeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gzs.0kj1m.cn

[S22] C：字符串转数字
来源：http://ypb.dashuyun.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xam.shanyushiyangtech.top

[S23] C：随机数
来源：http://vhj.chenjidiqi.icu

srand(time(NULL));  int r = rand() % 100;
来源：http://hks.pycfn.com

[S24] C：获取本地时间
来源：http://pcj.yfazqb.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wsy.zhiwuduotai.top

[S25] C：内存拷贝
来源：http://nct.zhengqikj.top

memcpy(dst, src, n);
来源：http://wvc.hnqzz.top

[S26] C：内存清零
来源：http://pze.yueranfly.top

memset(a, 0, sizeof a);
来源：http://ktw.guannengcc.top

[S27] C：定义常量
来源：http://cgw.sxryk.cn

const double PI = 3.14159;
来源：http://vti.jiagoushi.top

[S28] C：静态变量
来源：http://lft.bjfxy.top

static int counter = 0;
来源：http://any.daria6918.cn

[S29] C：变参函数
来源：http://ppi.hnxiangtu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uis.pengpengdd.cyou

[S30] C：头文件保护
来源：http://zuy.ctjpmb.com


<!-- 参考信息 -->