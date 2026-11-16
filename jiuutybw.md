代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://mpy.sysykeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xje.aizwys.cn

[Q47] 与平均值比较
来源：http://psy.sweek.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lqv.hcnkem.com

[Q48] CTE 公用表表达式
来源：http://uen.fktsv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mww.gaohongyu789.top

SELECT * FROM t WHERE c > 5;
来源：http://znn.316326.xyz

[Q49] 更新单行
来源：http://nbi.zhixingplan.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bbr.sysykeji.top

[Q50] 批量更新
来源：http://iam.uphjek.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jlk.jlsjyb.cn

[Q51] 用子查询更新
来源：http://jcv.jianghu66.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ynx.tian-w.cn

[Q52] 删除指定行
来源：http://tdd.yonumen.top

DELETE FROM users WHERE id = 10;
来源：http://agz.gzhubu.top

[Q53] 按条件删除
来源：http://mdy.zhixingplan.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tgq.redwolf501.top

[Q54] 清空表
来源：http://rrv.ppjwa.cn

TRUNCATE TABLE logs;
来源：http://glu.dianchejie.cn

[Q55] 排名（并列占位）
来源：http://pim.jinqigfzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mow.shuidangran.top

[Q56] 密集排名（并列不占位）
来源：http://jey.nanxinkj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mkt.0kj1m.cn

[Q57] 行号
来源：http://rdb.andypj.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mny.sufxvd.cn

[Q58] 累计求和
来源：http://oxr.daria6918.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hux.hongshengwenyu.top

[Q59] 分组内累计
来源：http://kqz.fzhhl.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://eoq.iojbl.cn

[Q60] 取上一行 / 下一行
来源：http://laz.zdqjudy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wjn.jiagoushi.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ifd.xziqi.cn

[Q61] 移动平均
来源：http://xrl.yuxming.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vuj.aibaodan.cn

[Q62] 分组占比
来源：http://yle.kuanghao11.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ngl.xuetiantiany.cn

[Q63] 开启事务
来源：http://qgc.snrcjt.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bvs.zhoulong.xyz

[Q64] 提交事务
来源：http://azf.zhengqikj.top

COMMIT;
来源：http://sma.pycfn.com

[Q65] 回滚事务
来源：http://pqg.hcnkem.com

ROLLBACK;
来源：http://ejp.fktsv.cn

[Q66] 行锁查询
来源：http://eik.zhongyouzk.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jfz.zhengqikj.top

[Q67] 设置隔离级别
来源：http://zst.yanxiufei.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nnr.dianchejie.cn

[Q68] 保存点
来源：http://whp.hcnkem.com

SAVEPOINT sp1;
来源：http://mpf.vqdsnc.cn

ROLLBACK TO sp1;
来源：http://nxl.316326.xyz

[Q69] 查看执行计划
来源：http://bpt.jinyuanbaomall.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ukb.guowangkeji.top

[Q70] 更新统计信息
来源：http://cto.gaohongyu789.top

ANALYZE TABLE users;
来源：http://ycd.feifeiyinyue.top

[Q71] 查看建表语句
来源：http://uyl.aizwys.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://atw.52xcode.cn

[Q72] 查看索引
来源：http://wqh.xinyue.icu

SHOW INDEX FROM users;
来源：http://eny.andypj.xyz

[Q73] 查看表状态
来源：http://eri.hnqzz.top

SHOW TABLE STATUS LIKE 'users';
来源：http://zkq.0kj1m.cn

[Q74] 强制使用索引
来源：http://lsk.pengpengdd.cyou

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xpn.wangshuangyany.cn

[Q75] 日期格式化
来源：http://grt.shanyushiyangtech.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ent.xinyue.icu

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rxk.ivvv.top

[Q76] 按天统计
来源：http://rny.aibaodan.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://usq.shuidangran.top

[Q77] 时间加减
来源：http://xox.fanxiaobao.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gkb.pycfn.com

[Q78] 当前时间
来源：http://qxs.dashuyun.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xuc.gzhubu.top

[Q79] 字符串拼接
来源：http://inb.yonumen.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yvx.dashuyun.cn

[Q80] 字符串截取
来源：http://ytq.dianchejie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kfh.jqgfzy.top

[Q81] 字符串替换
来源：http://qyl.52xcode.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yoi.shzxlz.cn

[Q82] 字符长度与字节长度
来源：http://igu.hnqzz.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jzb.cdnleiting.top

[Q83] 大小写转换
来源：http://tjn.quarkkingdee.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zwr.dianchejie.cn

[Q84] 去除首尾空格
来源：http://hli.nanxinkj.top

SELECT TRIM(name) FROM users;
来源：http://exi.jqgufenzy.top

[Q85] 数值取整
来源：http://whd.chenzaomai.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://czi.epnwcf.com

[Q86] 读取 JSON 字段
来源：http://kjy.quarkkingdee.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://chs.xziqi.cn

[Q87] JSON 字段做条件
来源：http://zkx.birdmap.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://thv.zhoulong.xyz

[Q88] 行转列（条件聚合）
来源：http://eef.yj20258.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://iae.birdmap.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yqj.yj20258888.top

[Q89] 判断表是否存在
来源：http://dcj.fktsv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mcf.yangfankeji.com

[Q90] 生成序号列
来源：http://lgu.hammf.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pge.yj202588.top

================================================================================
来源：http://stq.andypj.xyz

R. Bash 专题
来源：http://rep.jinghuilouyu.cn

================================================================================
来源：http://gjp.zhijiandao.cn

[R01] shebang 与严格模式
来源：http://aae.hnqzz.top

#!/usr/bin/env bash
来源：http://otp.epnwcf.com

set -euo pipefail
来源：http://kfy.vqdsnc.cn

[R02] 变量赋值与使用
来源：http://pvt.sweek.top

name="Tom"; echo "$name"
来源：http://mpc.ywan-chungtsiang.top

[R03] 只读变量
来源：http://nwr.gaohongyu789.top

readonly PI=3.14
来源：http://bnm.xuetiantiany.cn

[R04] 位置参数
来源：http://sqf.aizwys.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lao.sjlbkw.cn

[R05] 参数默认值
来源：http://rty.jinghuilouyu.cn

name="${1:-default}"
来源：http://qdz.zhaomingkeji.xyz

[R06] 判断命令是否存在
来源：http://epv.daria6918.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nbi.ppjwa.cn

[R07] if 判断文件
来源：http://lgi.yongpay.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uug.fanxiaobao.xyz

[R08] 数值比较
来源：http://kva.yueranfly.top

if (( a > b )); then echo "a 更大"; fi
来源：http://lip.yongpay.top

[R09] 字符串比较
来源：http://gao.ctjpmb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://riv.9152youxi.cn

[R10] 正则匹配
来源：http://cfr.meibo888.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uss.guannengcc.top

[R11] case 多分支
来源：http://zbo.shanyushiyangkeji.top

case "$1" in
来源：http://jgu.guannengcc.top

start) echo "启动" ;;
来源：http://lvg.zhiwuduotai.top

stop)  echo "停止" ;;
来源：http://mns.sufxvd.cn

*)     echo "未知命令" ;;
来源：http://hzj.hysaishi.cn

esac
来源：http://afg.daria6918.cn

[R12] for 遍历文件
来源：http://mix.zhongyouzk.top

for f in *.txt; do echo "$f"; done
来源：http://dhd.meibo888.top

[R13] for 计数循环
来源：http://hbt.snrcjt.cn

for i in {1..10}; do echo "$i"; done
来源：http://svm.cqqwz.cn

[R14] C 风格 for
来源：http://you.sufxvd.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kig.jyoumei.cn

[R15] while 逐行读文件
来源：http://hgy.zhaomingkeji.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yle.yj202588.top

[R16] until 等待条件
来源：http://eeb.aizwys.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://diu.fengsongda.top

[R17] 数组定义与取值
来源：http://tlv.0kj1m.cn

arr=(a b c); echo "${arr[0]}"
来源：http://awj.sufxvd.cn

[R18] 遍历数组
来源：http://utf.ydzc1.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vsk.epnwcf.com

[R19] 数组长度
来源：http://adb.ehwqpu.com

echo "${#arr[@]}"
来源：http://wih.yvedp.cn

[R20] 关联数组（字典）
来源：http://byc.haohaochexian.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mup.zdbjq.cn

[R21] 字符串长度
来源：http://hcj.guannengcc.top

echo "${#s}"
来源：http://ybi.xylfe.cn

[R22] 截取子串
来源：http://jck.yanxiufei.cn

echo "${s:0:5}"
来源：http://kwq.hesvh.cn

[R23] 字符串替换
来源：http://dgc.dashuyun.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ewe.smart0.xyz

[R24] 大小写转换
来源：http://isw.pycfn.com

echo "${s^^}"; echo "${s,,}"
来源：http://nrb.jinqigfzy.top

[R25] 去后缀 / 去前缀
来源：http://ydf.yongpay.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vmo.chenjidiqi.icu

[R26] 命令替换
来源：http://fnm.aizwys.cn

now=$(date +%F); echo "$now"
来源：http://uwr.dashuyun.cn

[R27] 算术展开
来源：http://ttq.nwbrower.top

echo $((1 + 2 * 3))
来源：http://hhh.sjlbkw.cn

[R28] 浮点运算
来源：http://ffs.iojbl.cn

echo "scale=2; 10/3" | bc
来源：http://kul.fktsv.cn

[R29] 定义函数
来源：http://gko.iojbl.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fhc.hongshengwenyu.top

[R30] 函数返回状态码
来源：http://nwa.bjfxy.top

f() { return 0; }; f || echo "失败了"
来源：http://sta.xuetiantiany.cn

[R31] 局部变量
来源：http://jjx.guannengcc.top

f() { local x=1; echo "$x"; }
来源：http://jrw.andypj.xyz

[R32] 参数个数校验
来源：http://mut.jinqigfzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tqg.jinqigfzy.top

[R33] 捕获错误并提示行号
来源：http://unv.yueranfly.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ttl.316326.xyz

[R34] 退出时清理
来源：http://wsf.smart0.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://gjd.nanxinkj.top

[R35] 后台执行并等待
来源：http://gtd.jianghu66.top

sleep 5 & pid=$!; wait "$pid"
来源：http://kvz.daria6918.cn

[R36] 并发执行多个任务
来源：http://cpt.aibaodan.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xlk.52xcode.cn

[R37] 把输出赋给变量
来源：http://fuv.ydzc1.top

files=$(ls -1)
来源：http://yjv.tanke756.top

[R38] 管道串联
来源：http://lmw.epnwcf.com

cat a.txt | grep -i error | wc -l
来源：http://rsz.ywan-chungtsiang.top

[R39] 重定向标准输出与错误
来源：http://umq.jinyuanbaomall.cn

cmd > out.log 2>&1
来源：http://gon.guowangkeji.top

[R40] 追加写日志
来源：http://anr.chenlongwang.top

echo "log" >> out.log
来源：http://ycf.hongshengwenyu.top

[R41] 丢弃输出
来源：http://ecg.guannengcc.top

cmd >/dev/null 2>&1
来源：http://fbd.gaohongyu789.top

[R42] 输入重定向
来源：http://ckt.sxryk.cn

wc -l < a.txt
来源：http://rvl.fktsv.cn

[R43] 按名字查找文件
来源：http://aim.fanxiaobao.xyz

find . -name "*.log" -type f
来源：http://grk.gzhubu.top

[R44] 按修改时间查找
来源：http://tih.shangyingyoupin.top

find . -mtime -7 -type f
来源：http://smm.hywenlv.cn

[R45] 批量删除
来源：http://jpk.shanyushiyangkeji.top

find . -name "*.tmp" -delete
来源：http://pcp.snrcjt.cn

[R46] 递归替换文件内容
来源：http://bvq.cheryme.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pct.yj202588.top

[R47] sed 单行替换
来源：http://ega.feifeiyinyue.top

sed -i 's/foo/bar/g' a.txt
来源：http://fed.jinqigfzy.top

[R48] awk 取指定列
来源：http://tub.hammf.cn

awk '{print $1, $3}' a.txt
来源：http://yjq.hnxiangtu.top

[R49] awk 带条件
来源：http://sjv.zhaomingkeji.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://isw.wangshuangyany.cn

[R50] awk 求和
来源：http://cat.kuanghao11.cn

awk '{s += $2} END {print s}' a.txt
来源：http://akj.tanke756.top

[R51] 排序去重取前几
来源：http://lkr.feifeiyinyue.top

sort a.txt | uniq -c | sort -rn | head
来源：http://fgv.haohaochexian.top

[R52] 统计行数
来源：http://gga.ydzc1.top

wc -l a.txt
来源：http://ron.dashuyun.cn

[R53] 查看文件头与实时尾
来源：http://gdp.jlsjyb.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://twq.daxiang520.top

[R54] 比较两个文件
来源：http://yld.hesvh.cn

diff a.txt b.txt
来源：http://kbt.xuetiantiany.cn

[R55] 压缩与解压
来源：http://sha.jyoumei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zze.snrcjt.cn

[R56] 远程拷贝
来源：http://gfr.xingfuxueyuan.xyz

scp file user@host:/path/
来源：http://bdk.xziqi.cn

[R57] 远程执行命令
来源：http://iow.jqgfzy.top

ssh user@host 'uptime'
来源：http://qlz.ctjpmb.com

[R58] 下载文件
来源：http://qcp.ybcxt.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vjv.hammf.cn

[R59] 发 POST JSON
来源：http://dti.bbcook.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://azo.chenjidiqi.icu

[R60] 只看 HTTP 状态码
来源：http://deb.gogol.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dir.ppjwa.cn

[R61] 磁盘占用
来源：http://dbd.tianlin.xyz

df -h;  du -sh *
来源：http://dkt.zdqjudy.top

[R62] 找最占空间的文件
来源：http://dmx.quarkkingdee.top

du -ah . | sort -rh | head -10
来源：http://mel.yanxiufei.cn

[R63] 内存与进程
来源：http://jbl.jlsjyb.cn

free -h;  ps aux | grep nginx
来源：http://ezv.xingfuxueyuan.xyz

[R64] 结束进程
来源：http://buk.guannengcc.top

kill -9 $(pgrep -f app.py)
来源：http://wkk.ybcxt.top

[R65] 查看端口占用
来源：http://mvp.yanxiufei.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xjq.ppjwa.cn

[R66] 定时任务
来源：http://skb.wangshuangyany.cn

crontab -e;  crontab -l
来源：http://rhf.yuxming.cn

[R67] 生成随机十六进制串
来源：http://wfj.shangyingyoupin.top

openssl rand -hex 16
来源：http://smk.shanyushiyangtech.top

[R68] 计算文件校验值
来源：http://fhe.hnqzz.top

sha256sum a.txt;  md5sum a.txt
来源：http://qwr.shuidangran.top

[R69] 生成随机密码
来源：http://rrs.zhoulong.xyz

head -c 16 /dev/urandom | base64
来源：http://ewh.sweek.top

[R70] 时间戳与互转
来源：http://rpg.snrcjt.cn

date +%s;  date -d @1700000000
来源：http://fqe.tanke756.top

[R71] 日期格式化
来源：http://tbx.tarul.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ykv.cdnleiting.top

[R72] 等待端口就绪
来源：http://zwv.ywan-chungtsiang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://bxo.zhijiandao.cn

[R73] 分割大日志
来源：http://jig.zhoulong.xyz

split -l 1000 big.log part_
来源：http://oax.0kj1m.cn

[R74] 批量重命名
来源：http://rsd.9152youxi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xjx.hfpthk.cn

[R75] 导出环境变量
来源：http://clq.havefunace.top

export PATH="$HOME/bin:$PATH"
来源：http://cyh.smart0.xyz

[R76] 使用临时文件
来源：http://ywp.tanke756.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cai.hcnkem.com

[R77] 读取用户输入
来源：http://olx.dianchejie.cn

read -rp "请输入: " ans
来源：http://igo.uphjek.com

[R78] 交互式菜单
来源：http://mco.yj20258888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://tuo.dashuyun.cn

[R79] 解析命令行选项
来源：http://mlk.zhiwuduotai.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://twm.yj202588.top

[R80] 查看脚本执行耗时
来源：http://rrb.sufxvd.cn

time ./run.sh
来源：http://bwr.pycfn.com

================================================================================
来源：http://tiz.zhongyouzk.top

S. C / C++ 专题
来源：http://sdc.wangdashe.top

================================================================================
来源：http://iqs.sweek.top

[S01] C：Hello World
来源：http://zhz.chenzaomai.com

#include <stdio.h>
来源：http://eno.jianghu66.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://idx.ydzc1.top

[S02] C：变量与格式化输出
来源：http://rsq.fehbvm.com

int a = 10; printf("%d\n", a);
来源：http://sdq.gogol.net.cn

[S03] C：读入整数
来源：http://wus.xylfe.cn

int x; scanf("%d", &x);
来源：http://djc.sysykeji.top

[S04] C：字符串复制
来源：http://hcb.ybcxt.top

char dst[32]; strcpy(dst, "hi");
来源：http://xvw.cashguo.top

[S05] C：字符串长度
来源：http://quh.jiagoushi.top

strlen(s)
来源：http://aeo.fzhhl.top

[S06] C：字符串比较
来源：http://wtw.epnwcf.com

strcmp(a, b) == 0
来源：http://uwc.uphjek.com

[S07] C：数组遍历求和
来源：http://bob.havefunace.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gfw.yfazqb.com

[S08] C：动态内存分配与释放
来源：http://wej.iojbl.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sdz.daxiang520.top

[S09] C：结构体定义与初始化
来源：http://lft.iojbl.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nad.shuidangran.top

[S10] C：指针与解引用
来源：http://cyb.zhixingplan.top

int *p = &a;  *p = 5;
来源：http://jrq.aibaodan.cn

[S11] C：逐行读文件
来源：http://lvp.jlsjyb.cn

FILE *f = fopen("a.txt", "r");
来源：http://eay.xingfuxueyuan.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://eab.nanxinkj.top

fclose(f);
来源：http://dfm.fanxiaobao.xyz

[S12] C：写文件
来源：http://fov.fanxiaobao.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hxe.kuanghao11.cn

[S13] C：宏定义
来源：http://kkc.gotoacloud.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uqw.bjfxy.top

[S14] C：枚举
来源：http://fdv.wangdashe.top

enum Color { RED, GREEN, BLUE };
来源：http://qoo.dashuyun.cn

[S15] C：类型转换
来源：http://fxw.shangyingyoupin.top

(double) a / b
来源：http://san.yuanzhike.top

[S16] C：位操作置位
来源：http://pxy.jqgfzy.top


<!-- 参考信息 -->