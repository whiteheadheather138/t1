代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kzp.guowangkeji.top

[Q50] 批量更新
来源：http://tto.c1oappe.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tat.shangyingyoupin.top

[Q51] 用子查询更新
来源：http://fvw.ybcxt.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iyc.fktsv.cn

[Q52] 删除指定行
来源：http://vpm.snrcjt.cn

DELETE FROM users WHERE id = 10;
来源：http://sml.andypj.xyz

[Q53] 按条件删除
来源：http://rnu.cashguo.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zhs.cheryme.top

[Q54] 清空表
来源：http://cnf.dianchejie.cn

TRUNCATE TABLE logs;
来源：http://bye.shanyushiyangtech.top

[Q55] 排名（并列占位）
来源：http://afi.gotoacloud.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ccv.52xcode.cn

[Q56] 密集排名（并列不占位）
来源：http://uuz.sufxvd.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zzn.guowangkeji.top

[Q57] 行号
来源：http://oin.yueranfly.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://erk.shzxlz.cn

[Q58] 累计求和
来源：http://adh.shangyingyoupin.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yqw.gogol.net.cn

[Q59] 分组内累计
来源：http://atj.zhengqikj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ztz.quarkkingdee.top

[Q60] 取上一行 / 下一行
来源：http://wuh.wangshuangyany.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tuq.gaohongyu789.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zfy.gzhubu.top

[Q61] 移动平均
来源：http://hgg.shanyushiyangtech.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://csv.zycfv.cn

[Q62] 分组占比
来源：http://uek.jinqigfzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fys.aibaodan.cn

[Q63] 开启事务
来源：http://fda.sjlbkw.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vou.tarul.cn

[Q64] 提交事务
来源：http://iso.guowangkeji.top

COMMIT;
来源：http://cfq.zhaomingkeji.xyz

[Q65] 回滚事务
来源：http://gko.pycfn.com

ROLLBACK;
来源：http://hcl.ctjpmb.com

[Q66] 行锁查询
来源：http://ggy.pengpengdd.cyou

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hel.smart0.xyz

[Q67] 设置隔离级别
来源：http://epd.zhaomingkeji.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lqt.ppjwa.cn

[Q68] 保存点
来源：http://uqz.haohaochexian.top

SAVEPOINT sp1;
来源：http://vtx.ydzc1.top

ROLLBACK TO sp1;
来源：http://jpy.zdqjudy.top

[Q69] 查看执行计划
来源：http://scv.yj202588.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://euw.birdmap.top

[Q70] 更新统计信息
来源：http://qzp.gzhubu.top

ANALYZE TABLE users;
来源：http://yzm.gogol.net.cn

[Q71] 查看建表语句
来源：http://quq.vehdjk.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xou.tian-w.cn

[Q72] 查看索引
来源：http://yuu.cqqwz.cn

SHOW INDEX FROM users;
来源：http://aui.wangshuangyany.cn

[Q73] 查看表状态
来源：http://eeh.zdqjudy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://nav.zhaomingkeji.xyz

[Q74] 强制使用索引
来源：http://tbd.zhaomingkeji.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ncn.hnqzz.top

[Q75] 日期格式化
来源：http://hin.fehbvm.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jmp.ehwqpu.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://skl.sysykeji.top

[Q76] 按天统计
来源：http://fnl.chenzaomai.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fpr.gaohongyu789.top

[Q77] 时间加减
来源：http://nyf.yfazqb.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://apz.hysaishi.cn

[Q78] 当前时间
来源：http://tie.mhx1999.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ifp.zhaomingkeji.xyz

[Q79] 字符串拼接
来源：http://zfl.yvedp.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vwf.birdmap.top

[Q80] 字符串截取
来源：http://uso.tianlin.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nzk.xinyue.icu

[Q81] 字符串替换
来源：http://fyn.sjlbkw.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nhp.yj20258.top

[Q82] 字符长度与字节长度
来源：http://mxl.jinghuilouyu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://unb.dashuyun.cn

[Q83] 大小写转换
来源：http://izz.pengpengdd.cyou

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ivu.shuidangran.top

[Q84] 去除首尾空格
来源：http://kjm.yvedp.cn

SELECT TRIM(name) FROM users;
来源：http://ooo.yj20258888.top

[Q85] 数值取整
来源：http://tbf.haohaochexian.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gef.sxryk.cn

[Q86] 读取 JSON 字段
来源：http://oad.gaohongyu789.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xpu.zhixingplan.top

[Q87] JSON 字段做条件
来源：http://bsy.chenjidiqi.icu

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rny.chenlongwang.top

[Q88] 行转列（条件聚合）
来源：http://eua.ivvv.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tog.hnxiangtu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://beb.gotoacloud.top

[Q89] 判断表是否存在
来源：http://zmf.bbcook.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mkg.yangfankeji.com

[Q90] 生成序号列
来源：http://sbt.hysaishi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ydm.ydzc1.top

================================================================================
来源：http://hsf.sjlbkw.cn

R. Bash 专题
来源：http://red.aibaodan.cn

================================================================================
来源：http://cdj.shanyushiyangkeji.top

[R01] shebang 与严格模式
来源：http://ein.snrcjt.cn

#!/usr/bin/env bash
来源：http://hag.hywenlv.cn

set -euo pipefail
来源：http://lqd.xylfe.cn

[R02] 变量赋值与使用
来源：http://qwy.meibo888.top

name="Tom"; echo "$name"
来源：http://xkw.fengsongda.top

[R03] 只读变量
来源：http://yaz.tian-w.cn

readonly PI=3.14
来源：http://fgg.fengsongda.top

[R04] 位置参数
来源：http://pqk.gzhubu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://caw.zdqjudy.top

[R05] 参数默认值
来源：http://abg.sysykeji.top

name="${1:-default}"
来源：http://gjb.havefunace.top

[R06] 判断命令是否存在
来源：http://xkz.jlsjyb.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jbb.yuanzhike.top

[R07] if 判断文件
来源：http://wlx.quarkkingdee.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pdz.uphjek.com

[R08] 数值比较
来源：http://dpz.shanyushiyangkeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://prr.ppjwa.cn

[R09] 字符串比较
来源：http://gho.cheryme.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dql.jyoumei.cn

[R10] 正则匹配
来源：http://skm.pengpengdd.cyou

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fbl.ivvv.top

[R11] case 多分支
来源：http://gub.shanyushiyangkeji.top

case "$1" in
来源：http://yab.tanke756.top

start) echo "启动" ;;
来源：http://sur.zycfv.cn

stop)  echo "停止" ;;
来源：http://oxv.svipenyu.cn

*)     echo "未知命令" ;;
来源：http://qvz.chenlongwang.top

esac
来源：http://xga.zhengqikj.top

[R12] for 遍历文件
来源：http://pgx.haohaochexian.top

for f in *.txt; do echo "$f"; done
来源：http://uld.zhengqikj.top

[R13] for 计数循环
来源：http://mek.hnxiangtu.top

for i in {1..10}; do echo "$i"; done
来源：http://sgg.316326.xyz

[R14] C 风格 for
来源：http://esd.tanke756.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://knu.jianghu66.top

[R15] while 逐行读文件
来源：http://ync.xuetiantiany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qxf.dashuyun.cn

[R16] until 等待条件
来源：http://dwe.vehdjk.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fdm.hywenlv.cn

[R17] 数组定义与取值
来源：http://rgj.52xcode.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fpa.zdqjudy.top

[R18] 遍历数组
来源：http://nuq.uphjek.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xug.yvedp.cn

[R19] 数组长度
来源：http://zpn.cashguo.top

echo "${#arr[@]}"
来源：http://pwb.cashguo.top

[R20] 关联数组（字典）
来源：http://fpc.xingfuxueyuan.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lju.dianchejie.cn

[R21] 字符串长度
来源：http://gss.jinyuanbaomall.cn

echo "${#s}"
来源：http://vfe.iojbl.cn

[R22] 截取子串
来源：http://oez.redwolf501.top

echo "${s:0:5}"
来源：http://lde.bbcook.cn

[R23] 字符串替换
来源：http://dnh.zdbjq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bql.bbcook.cn

[R24] 大小写转换
来源：http://uqa.jinghuilouyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://owm.daxiang520.top

[R25] 去后缀 / 去前缀
来源：http://hie.zdqjudy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://hgg.zhengqikj.top

[R26] 命令替换
来源：http://eje.hammf.cn

now=$(date +%F); echo "$now"
来源：http://fpx.zhengqikj.top

[R27] 算术展开
来源：http://axu.wangshuangyany.cn

echo $((1 + 2 * 3))
来源：http://zzg.chenjidiqi.icu

[R28] 浮点运算
来源：http://kfh.chenzaomai.com

echo "scale=2; 10/3" | bc
来源：http://ius.xziqi.cn

[R29] 定义函数
来源：http://orv.cdnleiting.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bzy.jinyuanbaomall.cn

[R30] 函数返回状态码
来源：http://jou.zycfv.cn

f() { return 0; }; f || echo "失败了"
来源：http://gjf.cucudq.cn

[R31] 局部变量
来源：http://elt.ywan-chungtsiang.top

f() { local x=1; echo "$x"; }
来源：http://tqr.fehbvm.com

[R32] 参数个数校验
来源：http://lne.xingfuxueyuan.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qns.chenzaomai.com

[R33] 捕获错误并提示行号
来源：http://noq.yonumen.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mkb.hywenlv.cn

[R34] 退出时清理
来源：http://ejd.hnxiangtu.top

trap 'rm -f "$tmp"' EXIT
来源：http://elc.tanke756.top

[R35] 后台执行并等待
来源：http://nbe.cucudq.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tzz.redwolf501.top

[R36] 并发执行多个任务
来源：http://geq.nanxuanxn.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://aof.jinyuanbaomall.cn

[R37] 把输出赋给变量
来源：http://aeh.zhaomingkeji.xyz

files=$(ls -1)
来源：http://hdm.shanyushiyangkeji.top

[R38] 管道串联
来源：http://nkb.meibo888.top

cat a.txt | grep -i error | wc -l
来源：http://ldn.daxiang520.top

[R39] 重定向标准输出与错误
来源：http://ffa.tianlin.xyz

cmd > out.log 2>&1
来源：http://zoz.jlsjyb.cn

[R40] 追加写日志
来源：http://yka.cqqwz.cn

echo "log" >> out.log
来源：http://leh.316326.xyz

[R41] 丢弃输出
来源：http://xrr.xylfe.cn

cmd >/dev/null 2>&1
来源：http://ezk.kuanghao11.cn

[R42] 输入重定向
来源：http://ksc.dashuyun.cn

wc -l < a.txt
来源：http://nwq.smart0.xyz

[R43] 按名字查找文件
来源：http://xsw.havefunace.top

find . -name "*.log" -type f
来源：http://rjd.yuxming.cn

[R44] 按修改时间查找
来源：http://nrs.aibaodan.cn

find . -mtime -7 -type f
来源：http://vax.hnxiangtu.top

[R45] 批量删除
来源：http://lqv.guowangkeji.top

find . -name "*.tmp" -delete
来源：http://gkh.hnqzz.top

[R46] 递归替换文件内容
来源：http://mhh.xziqi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bdc.tarul.cn

[R47] sed 单行替换
来源：http://iix.316326.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://fph.snrcjt.cn

[R48] awk 取指定列
来源：http://dfu.guannengcc.top

awk '{print $1, $3}' a.txt
来源：http://zrb.haohaochexian.top

[R49] awk 带条件
来源：http://tzt.wangshuangyany.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ggw.epnwcf.com

[R50] awk 求和
来源：http://xge.ehwqpu.com

awk '{s += $2} END {print s}' a.txt
来源：http://zkg.xuanzx.com

[R51] 排序去重取前几
来源：http://xez.ehwqpu.com

sort a.txt | uniq -c | sort -rn | head
来源：http://pxq.guowangkeji.top

[R52] 统计行数
来源：http://xbo.zhijiandao.cn

wc -l a.txt
来源：http://xkw.yongpay.top

[R53] 查看文件头与实时尾
来源：http://crt.nanxuanxn.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tnp.meibo888.top

[R54] 比较两个文件
来源：http://mpu.bbcook.cn

diff a.txt b.txt
来源：http://sev.gotoacloud.top

[R55] 压缩与解压
来源：http://ivh.yuanzhike.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tgs.hcnkem.com

[R56] 远程拷贝
来源：http://eys.daria6918.cn

scp file user@host:/path/
来源：http://lwi.xziqi.cn

[R57] 远程执行命令
来源：http://dal.ydzc1.top

ssh user@host 'uptime'
来源：http://rts.pengpengdd.cyou

[R58] 下载文件
来源：http://uhs.yanxiufei.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dic.daxiang520.top

[R59] 发 POST JSON
来源：http://gkp.shanyushiyangkeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://imx.hongshengwenyu.top

[R60] 只看 HTTP 状态码
来源：http://mqx.zhixingplan.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kjt.redwolf501.top

[R61] 磁盘占用
来源：http://bgy.jinyuanbaomall.cn

df -h;  du -sh *
来源：http://cqa.fehbvm.com

[R62] 找最占空间的文件
来源：http://sli.ydzc1.top

du -ah . | sort -rh | head -10
来源：http://mrr.nanxinkj.top

[R63] 内存与进程
来源：http://cck.yvedp.cn

free -h;  ps aux | grep nginx
来源：http://bjr.ydzc1.top

[R64] 结束进程
来源：http://sie.zhixingplan.top

kill -9 $(pgrep -f app.py)
来源：http://dwn.ydzc1.top

[R65] 查看端口占用
来源：http://vzs.birdmap.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sug.jiagoushi.top

[R66] 定时任务
来源：http://yxb.bbcook.cn

crontab -e;  crontab -l
来源：http://wnp.yj20258888.top

[R67] 生成随机十六进制串
来源：http://wny.nwbrower.top

openssl rand -hex 16
来源：http://ose.zhongyouzk.top

[R68] 计算文件校验值
来源：http://uvy.cashguo.top

sha256sum a.txt;  md5sum a.txt
来源：http://ikr.zhaomingkeji.xyz

[R69] 生成随机密码
来源：http://tzj.hfpthk.cn

head -c 16 /dev/urandom | base64
来源：http://mea.chenjidiqi.icu

[R70] 时间戳与互转
来源：http://ors.ppjwa.cn

date +%s;  date -d @1700000000
来源：http://zib.zhengqikj.top

[R71] 日期格式化
来源：http://jna.yj20258888.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://uws.sxryk.cn

[R72] 等待端口就绪
来源：http://vla.tianlin.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://xez.yj202588.top

[R73] 分割大日志
来源：http://rlq.zhengqikj.top

split -l 1000 big.log part_
来源：http://ctm.fanxiaobao.xyz

[R74] 批量重命名
来源：http://wjb.ehwqpu.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://akq.fanxiaobao.xyz

[R75] 导出环境变量
来源：http://hto.c1oappe.top

export PATH="$HOME/bin:$PATH"
来源：http://rdw.zdbjq.cn

[R76] 使用临时文件
来源：http://yso.jinyuanbaomall.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uex.zhiwuduotai.top

[R77] 读取用户输入
来源：http://eza.meibo888.top

read -rp "请输入: " ans
来源：http://kcq.ehwqpu.com

[R78] 交互式菜单
来源：http://yoz.ybcxt.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xkz.jiagoushi.top

[R79] 解析命令行选项
来源：http://osb.fehbvm.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bxd.zhongyouzk.top

[R80] 查看脚本执行耗时
来源：http://zek.gzhubu.top

time ./run.sh
来源：http://end.tian-w.cn

================================================================================
来源：http://iwy.guannengcc.top

S. C / C++ 专题
来源：http://skz.ybcxt.top

================================================================================
来源：http://wvi.zhengqikj.top

[S01] C：Hello World
来源：http://kuk.zdbjq.cn

#include <stdio.h>
来源：http://duy.uphjek.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://mgu.yj20258.top

[S02] C：变量与格式化输出
来源：http://lxl.pycfn.com

int a = 10; printf("%d\n", a);
来源：http://wnl.cucudq.cn

[S03] C：读入整数
来源：http://toy.ctjpmb.com

int x; scanf("%d", &x);
来源：http://chy.haohaochexian.top

[S04] C：字符串复制
来源：http://kqp.zhongyouzk.top

char dst[32]; strcpy(dst, "hi");
来源：http://qfs.sjlbkw.cn

[S05] C：字符串长度
来源：http://mmj.yanxiufei.cn

strlen(s)
来源：http://xtk.ydzc1.top

[S06] C：字符串比较
来源：http://avz.redwolf501.top

strcmp(a, b) == 0
来源：http://ref.fehbvm.com

[S07] C：数组遍历求和
来源：http://nzh.smart0.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pka.nanxuanxn.top

[S08] C：动态内存分配与释放
来源：http://ykl.quarkkingdee.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sqm.cheryme.top

[S09] C：结构体定义与初始化
来源：http://yva.jianghu66.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rgs.shanyushiyangkeji.top

[S10] C：指针与解引用
来源：http://oge.zhijiandao.cn

int *p = &a;  *p = 5;
来源：http://ckp.52xcode.cn

[S11] C：逐行读文件
来源：http://cjv.smart0.xyz

FILE *f = fopen("a.txt", "r");
来源：http://ryo.xingfuxueyuan.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://dlj.yangfankeji.com

fclose(f);
来源：http://hdr.cheryme.top

[S12] C：写文件
来源：http://qoz.cucudq.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qhy.nanxuanxn.top

[S13] C：宏定义
来源：http://tba.yj20258888.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://umo.yfazqb.com

[S14] C：枚举
来源：http://isq.shzxlz.cn

enum Color { RED, GREEN, BLUE };
来源：http://ssz.nanxinkj.top

[S15] C：类型转换
来源：http://ngl.nanxinkj.top

(double) a / b
来源：http://zuz.tarul.cn

[S16] C：位操作置位
来源：http://gdp.shanyushiyangtech.top

x |= (1 << 3);
来源：http://kgy.wangshuangyany.cn

[S17] C：安全拼接字符串
来源：http://xln.fktsv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jen.iojbl.cn

[S18] C：命令行参数
来源：http://tdg.sufxvd.cn

int main(int argc, char **argv)
来源：http://via.jlsjyb.cn

[S19] C：快速排序
来源：http://sea.mhx1999.top

qsort(a, n, sizeof(int), cmp);
来源：http://plb.chenlongwang.top

[S20] C：二分查找
来源：http://wvy.hysaishi.cn


<!-- 参考信息 -->