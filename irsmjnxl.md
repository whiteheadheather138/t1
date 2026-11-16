代发 wailian999

[Q33] 多列分组
来源：http://auz.feifeiyinyue.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vqk.52xcode.cn

[Q34] 每组取第一条
来源：http://nsa.guowangkeji.top

SELECT * FROM (
来源：http://mot.havefunace.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xpo.cucudq.cn

) t WHERE rn = 1;
来源：http://vfv.andypj.xyz

[Q35] 内连接
来源：http://lsy.mhx1999.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jvq.ppjwa.cn

[Q36] 左连接
来源：http://wvz.zhixingplan.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xus.sufxvd.cn

[Q37] 右连接
来源：http://yqd.shanyushiyangkeji.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qxh.nanxinkj.top

[Q38] 全外连接（PostgreSQL）
来源：http://xeu.epnwcf.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ctx.hnxiangtu.top

[Q39] 自连接（查上下级）
来源：http://gnw.meibo888.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://owq.sxryk.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qwv.yongpay.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ggi.cucudq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hlp.gzhubu.top

[Q41] 多表连接
来源：http://gpd.9152youxi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ojy.xuetiantiany.cn

JOIN users u ON u.id = o.user_id
来源：http://kpc.ywan-chungtsiang.top

JOIN products p ON p.id = o.product_id;
来源：http://zvi.mhx1999.top

[Q42] 连接条件附加过滤
来源：http://hev.dianchejie.cn

SELECT u.name, o.amount FROM users u
来源：http://vcy.aizwys.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ric.jqgufenzy.top

[Q43] 标量子查询
来源：http://fte.ydzc1.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ejg.daria6918.cn

[Q44] IN 子查询
来源：http://zgy.hnqzz.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://opt.zhaomingkeji.xyz

[Q45] EXISTS 判断存在
来源：http://wtr.tianlin.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mcd.pengpengdd.cyou

[Q46] NOT EXISTS 判断不存在
来源：http://gxh.cdnleiting.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uxe.yanxiufei.cn

[Q47] 与平均值比较
来源：http://ctm.jqgfzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vmq.zhiwuduotai.top

[Q48] CTE 公用表表达式
来源：http://qmt.daxiang520.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ggo.pengpengdd.cyou

SELECT * FROM t WHERE c > 5;
来源：http://wxs.fanxiaobao.xyz

[Q49] 更新单行
来源：http://xxe.jinyuanbaomall.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://azz.yuanzhike.top

[Q50] 批量更新
来源：http://rmm.gogol.net.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bwv.52xcode.cn

[Q51] 用子查询更新
来源：http://duz.zdbjq.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cdv.c1oappe.top

[Q52] 删除指定行
来源：http://afi.gaohongyu789.top

DELETE FROM users WHERE id = 10;
来源：http://jut.xingfuxueyuan.xyz

[Q53] 按条件删除
来源：http://vah.smart0.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zan.pengpengdd.cyou

[Q54] 清空表
来源：http://waw.aizwys.cn

TRUNCATE TABLE logs;
来源：http://wpo.9152youxi.cn

[Q55] 排名（并列占位）
来源：http://kxl.chenlongwang.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://enn.xylfe.cn

[Q56] 密集排名（并列不占位）
来源：http://kvt.ctjpmb.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ibo.chenzaomai.com

[Q57] 行号
来源：http://hcy.xuanzx.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tcj.ehwqpu.com

[Q58] 累计求和
来源：http://hpd.chenlongwang.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://oce.chenzaomai.com

[Q59] 分组内累计
来源：http://ojk.ctjpmb.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nrd.uphjek.com

[Q60] 取上一行 / 下一行
来源：http://yqb.wangdashe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qru.feifeiyinyue.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://twi.aizwys.cn

[Q61] 移动平均
来源：http://vna.316326.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cdu.andypj.xyz

[Q62] 分组占比
来源：http://wjn.iojbl.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ypv.sysykeji.top

[Q63] 开启事务
来源：http://dxo.mhx1999.top

START TRANSACTION;                -- 或 BEGIN
来源：http://zzg.zdqjudy.top

[Q64] 提交事务
来源：http://eso.zhongyouzk.top

COMMIT;
来源：http://cjg.fktsv.cn

[Q65] 回滚事务
来源：http://wca.uphjek.com

ROLLBACK;
来源：http://qbh.xuanzx.com

[Q66] 行锁查询
来源：http://une.redwolf501.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tmi.ivvv.top

[Q67] 设置隔离级别
来源：http://qwo.52xcode.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gwy.jinghuilouyu.cn

[Q68] 保存点
来源：http://rcb.nanxuanxn.top

SAVEPOINT sp1;
来源：http://mbn.sweek.top

ROLLBACK TO sp1;
来源：http://nmn.andypj.xyz

[Q69] 查看执行计划
来源：http://ezs.guannengcc.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pnc.xziqi.cn

[Q70] 更新统计信息
来源：http://yrr.yj202588.top

ANALYZE TABLE users;
来源：http://mxk.ywan-chungtsiang.top

[Q71] 查看建表语句
来源：http://xey.vqdsnc.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eck.0kj1m.cn

[Q72] 查看索引
来源：http://jyp.xuanzx.com

SHOW INDEX FROM users;
来源：http://fhf.gaohongyu789.top

[Q73] 查看表状态
来源：http://vqw.hfpthk.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kdc.yanxiufei.cn

[Q74] 强制使用索引
来源：http://img.pycfn.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zum.xziqi.cn

[Q75] 日期格式化
来源：http://hbr.ydjk.org.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sfj.uphjek.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tqn.redwolf501.top

[Q76] 按天统计
来源：http://pbm.nanxuanxn.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ryo.tian-w.cn

[Q77] 时间加减
来源：http://cll.chenlongwang.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nje.fehbvm.com

[Q78] 当前时间
来源：http://qdg.svipenyu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qgp.yongpay.top

[Q79] 字符串拼接
来源：http://fev.cashguo.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yet.jinqigufen.top

[Q80] 字符串截取
来源：http://ien.epnwcf.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kob.pengpengdd.cyou

[Q81] 字符串替换
来源：http://ufw.52xcode.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ogi.bjfxy.top

[Q82] 字符长度与字节长度
来源：http://sws.xuetiantiany.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kwc.hnxiangtu.top

[Q83] 大小写转换
来源：http://fwg.yuanzhike.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blt.chenzaomai.com

[Q84] 去除首尾空格
来源：http://nyz.fengsongda.top

SELECT TRIM(name) FROM users;
来源：http://xzc.gaohongyu789.top

[Q85] 数值取整
来源：http://qmi.xuanzx.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kzk.feifeiyinyue.top

[Q86] 读取 JSON 字段
来源：http://mzf.wangshuangyany.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ohp.dashuyun.cn

[Q87] JSON 字段做条件
来源：http://hpa.tarul.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eij.shuidangran.top

[Q88] 行转列（条件聚合）
来源：http://tig.ybcxt.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://aqc.jqgfzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://etp.52xcode.cn

[Q89] 判断表是否存在
来源：http://xov.jlsjyb.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wmd.wangdashe.top

[Q90] 生成序号列
来源：http://twu.zhaomingkeji.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tti.yuanzhike.top

================================================================================
来源：http://nke.chenzaomai.com

R. Bash 专题
来源：http://qao.c1oappe.top

================================================================================
来源：http://gme.zdbjq.cn

[R01] shebang 与严格模式
来源：http://cpo.wangshuangyany.cn

#!/usr/bin/env bash
来源：http://pyw.chenzaomai.com

set -euo pipefail
来源：http://xwv.cashguo.top

[R02] 变量赋值与使用
来源：http://nzk.tianlin.xyz

name="Tom"; echo "$name"
来源：http://zpx.gotoacloud.top

[R03] 只读变量
来源：http://dzg.snrcjt.cn

readonly PI=3.14
来源：http://skw.gzhubu.top

[R04] 位置参数
来源：http://rjc.jinyuanbaomall.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vaw.shuidangran.top

[R05] 参数默认值
来源：http://eui.yanxiufei.cn

name="${1:-default}"
来源：http://uaa.pycfn.com

[R06] 判断命令是否存在
来源：http://wqf.yj20258888.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nww.ybcxt.top

[R07] if 判断文件
来源：http://pha.cdnleiting.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rpc.redwolf501.top

[R08] 数值比较
来源：http://xfy.zhoulong.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://ffb.shuidangran.top

[R09] 字符串比较
来源：http://qxk.daxiang520.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bdp.jinyuanbaomall.cn

[R10] 正则匹配
来源：http://vmn.tian-w.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ipv.sweek.top

[R11] case 多分支
来源：http://eom.cucudq.cn

case "$1" in
来源：http://qje.ehwqpu.com

start) echo "启动" ;;
来源：http://ggw.uphjek.com

stop)  echo "停止" ;;
来源：http://chu.yj20258.top

*)     echo "未知命令" ;;
来源：http://obo.chenjidiqi.icu

esac
来源：http://zwu.zhongyouzk.top

[R12] for 遍历文件
来源：http://uvt.yonumen.top

for f in *.txt; do echo "$f"; done
来源：http://iwg.meibo888.top

[R13] for 计数循环
来源：http://qho.gotoacloud.top

for i in {1..10}; do echo "$i"; done
来源：http://pva.jyoumei.cn

[R14] C 风格 for
来源：http://dbh.c1oappe.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rkd.cdnleiting.top

[R15] while 逐行读文件
来源：http://mwa.hfpthk.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pyu.vqdsnc.cn

[R16] until 等待条件
来源：http://uwe.chenzaomai.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lju.gotoacloud.top

[R17] 数组定义与取值
来源：http://twr.shangyingyoupin.top

arr=(a b c); echo "${arr[0]}"
来源：http://dbi.jlsjyb.cn

[R18] 遍历数组
来源：http://fmy.ehwqpu.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kwk.hnqzz.top

[R19] 数组长度
来源：http://swv.zhoulong.xyz

echo "${#arr[@]}"
来源：http://nll.uphjek.com

[R20] 关联数组（字典）
来源：http://cbq.zdqjudy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oye.guannengcc.top

[R21] 字符串长度
来源：http://mtm.gzhubu.top

echo "${#s}"
来源：http://udi.dashuyun.cn

[R22] 截取子串
来源：http://cgv.tanke756.top

echo "${s:0:5}"
来源：http://mym.gzhubu.top

[R23] 字符串替换
来源：http://oro.nanxinkj.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wee.316326.xyz

[R24] 大小写转换
来源：http://pbw.jinghuilouyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://iku.9152youxi.cn

[R25] 去后缀 / 去前缀
来源：http://kcv.yfazqb.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://ezz.ppjwa.cn

[R26] 命令替换
来源：http://weg.feifeiyinyue.top

now=$(date +%F); echo "$now"
来源：http://xug.yangfankeji.com

[R27] 算术展开
来源：http://klr.bjfxy.top

echo $((1 + 2 * 3))
来源：http://abb.zhoulong.xyz

[R28] 浮点运算
来源：http://cod.meibo888.top

echo "scale=2; 10/3" | bc
来源：http://bea.xylfe.cn

[R29] 定义函数
来源：http://axh.dashuyun.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mrq.sweek.top

[R30] 函数返回状态码
来源：http://iqf.aizwys.cn

f() { return 0; }; f || echo "失败了"
来源：http://fwe.bjfxy.top

[R31] 局部变量
来源：http://gwx.svipenyu.cn

f() { local x=1; echo "$x"; }
来源：http://pxv.yuxming.cn

[R32] 参数个数校验
来源：http://zal.bjfxy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yzp.hammf.cn

[R33] 捕获错误并提示行号
来源：http://nkb.zdqjudy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pww.shanyushiyangkeji.top

[R34] 退出时清理
来源：http://twv.zhoulong.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://sjp.xylfe.cn

[R35] 后台执行并等待
来源：http://scl.cdnleiting.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ans.jlsjyb.cn

[R36] 并发执行多个任务
来源：http://lzd.zhengqikj.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zxa.c1oappe.top

[R37] 把输出赋给变量
来源：http://qwj.hcnkem.com

files=$(ls -1)
来源：http://xbu.zhoulong.xyz

[R38] 管道串联
来源：http://eph.xuetiantiany.cn

cat a.txt | grep -i error | wc -l
来源：http://qqa.zhijiandao.cn

[R39] 重定向标准输出与错误
来源：http://qbe.uphjek.com

cmd > out.log 2>&1
来源：http://dop.nwbrower.top

[R40] 追加写日志
来源：http://plc.bjfxy.top

echo "log" >> out.log
来源：http://juc.ydzc1.top

[R41] 丢弃输出
来源：http://ixa.wangdashe.top

cmd >/dev/null 2>&1
来源：http://kdy.iojbl.cn

[R42] 输入重定向
来源：http://hkm.tarul.cn

wc -l < a.txt
来源：http://mar.fzhhl.top

[R43] 按名字查找文件
来源：http://ygi.hongshengwenyu.top

find . -name "*.log" -type f
来源：http://tew.mhx1999.top

[R44] 按修改时间查找
来源：http://ieg.zhoulong.xyz

find . -mtime -7 -type f
来源：http://fvt.shanyushiyangkeji.top

[R45] 批量删除
来源：http://lnb.gotoacloud.top

find . -name "*.tmp" -delete
来源：http://aqo.yfazqb.com

[R46] 递归替换文件内容
来源：http://vba.gaohongyu789.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zqh.andypj.xyz

[R47] sed 单行替换
来源：http://ydy.xylfe.cn

sed -i 's/foo/bar/g' a.txt
来源：http://smw.cashguo.top

[R48] awk 取指定列
来源：http://uqi.tian-w.cn

awk '{print $1, $3}' a.txt
来源：http://lmc.nanxinkj.top

[R49] awk 带条件
来源：http://mwd.chenzaomai.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jpj.cqqwz.cn

[R50] awk 求和
来源：http://dzz.xylfe.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xqb.yj202588.top

[R51] 排序去重取前几
来源：http://fwu.zhijiandao.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://eqi.c1oappe.top

[R52] 统计行数
来源：http://fko.sweek.top

wc -l a.txt
来源：http://toq.hnqzz.top

[R53] 查看文件头与实时尾
来源：http://qad.tarul.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bly.hesvh.cn

[R54] 比较两个文件
来源：http://lyp.birdmap.top

diff a.txt b.txt
来源：http://nzi.iojbl.cn

[R55] 压缩与解压
来源：http://ahw.cashguo.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://exh.shanyushiyangtech.top

[R56] 远程拷贝
来源：http://klj.jqgufenzy.top

scp file user@host:/path/
来源：http://cdj.tarul.cn

[R57] 远程执行命令
来源：http://ici.52xcode.cn

ssh user@host 'uptime'
来源：http://feg.jiagoushi.top

[R58] 下载文件
来源：http://jpl.sweek.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uuz.yonumen.top

[R59] 发 POST JSON
来源：http://rgr.yueranfly.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rwi.jianghu66.top

[R60] 只看 HTTP 状态码
来源：http://vzn.pengpengdd.cyou

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mvu.bjfxy.top

[R61] 磁盘占用
来源：http://poo.haohaochexian.top

df -h;  du -sh *
来源：http://ukf.chenzaomai.com

[R62] 找最占空间的文件
来源：http://ovm.yj20258888.top

du -ah . | sort -rh | head -10
来源：http://cwq.xuetiantiany.cn

[R63] 内存与进程
来源：http://hqh.yueranfly.top

free -h;  ps aux | grep nginx
来源：http://vmq.yongpay.top

[R64] 结束进程
来源：http://xih.tianlin.xyz

kill -9 $(pgrep -f app.py)
来源：http://wvn.yj20258888.top

[R65] 查看端口占用
来源：http://uar.sxryk.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cos.hcnkem.com

[R66] 定时任务
来源：http://ift.hongshengwenyu.top

crontab -e;  crontab -l
来源：http://zjc.jyoumei.cn

[R67] 生成随机十六进制串
来源：http://dbn.guowangkeji.top

openssl rand -hex 16
来源：http://ovq.birdmap.top

[R68] 计算文件校验值
来源：http://qhh.yanxiufei.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gnd.gogol.net.cn

[R69] 生成随机密码
来源：http://ucy.tarul.cn

head -c 16 /dev/urandom | base64
来源：http://tum.jlsjyb.cn

[R70] 时间戳与互转
来源：http://ukb.ctjpmb.com

date +%s;  date -d @1700000000
来源：http://zle.sysykeji.top

[R71] 日期格式化
来源：http://ktn.jiagoushi.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://nny.zycfv.cn

[R72] 等待端口就绪
来源：http://yol.xuanzx.com

until nc -z localhost 3306; do sleep 1; done
来源：http://nxr.jinghuilouyu.cn

[R73] 分割大日志
来源：http://opf.hesvh.cn

split -l 1000 big.log part_
来源：http://fkl.hysaishi.cn

[R74] 批量重命名
来源：http://wiy.nanxuanxn.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ovk.jinghuilouyu.cn

[R75] 导出环境变量
来源：http://ffh.hammf.cn

export PATH="$HOME/bin:$PATH"
来源：http://ylh.jinqigfzy.top

[R76] 使用临时文件
来源：http://nyy.fehbvm.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xmk.zhaomingkeji.xyz

[R77] 读取用户输入
来源：http://sxn.yueranfly.top

read -rp "请输入: " ans
来源：http://pvi.tanke756.top

[R78] 交互式菜单
来源：http://eqi.hnqzz.top

select opt in a b c; do echo "$opt"; break; done
来源：http://die.hfpthk.cn

[R79] 解析命令行选项
来源：http://fyr.hammf.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://edl.xuetiantiany.cn

[R80] 查看脚本执行耗时
来源：http://chb.zhoulong.xyz

time ./run.sh
来源：http://uaq.sxryk.cn

================================================================================
来源：http://ihk.xinyue.icu

S. C / C++ 专题
来源：http://yhk.jqgfzy.top

================================================================================
来源：http://qfs.andypj.xyz

[S01] C：Hello World
来源：http://qns.zhaomingkeji.xyz

#include <stdio.h>
来源：http://eth.meibo888.top


<!-- 参考信息 -->