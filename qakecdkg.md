代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://fnl.shuidangran.top

[Q30] 分组统计
来源：http://kie.sjlbkw.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://put.chenjidiqi.icu

[Q31] 分组后过滤
来源：http://bys.haohaochexian.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gqe.cdnleiting.top

[Q32] 分组拼接字符串
来源：http://fxa.ybcxt.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yub.vqdsnc.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://auh.yangfankeji.com

[Q33] 多列分组
来源：http://lnb.pengpengdd.cyou

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wfx.yanxiufei.cn

[Q34] 每组取第一条
来源：http://bcq.ehwqpu.com

SELECT * FROM (
来源：http://iwv.hysaishi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ukx.hcnkem.com

) t WHERE rn = 1;
来源：http://kkt.quarkkingdee.top

[Q35] 内连接
来源：http://ana.zdqjudy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xlk.xingfuxueyuan.xyz

[Q36] 左连接
来源：http://ioh.uphjek.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pnd.birdmap.top

[Q37] 右连接
来源：http://khw.52xcode.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zfo.ctjpmb.com

[Q38] 全外连接（PostgreSQL）
来源：http://rok.guannengcc.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dxk.svipenyu.cn

[Q39] 自连接（查上下级）
来源：http://uom.cheryme.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://sbt.epnwcf.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kry.yj20258888.top

[Q40] 交叉连接（笛卡尔积）
来源：http://kuj.jinqigufen.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://flz.jyoumei.cn

[Q41] 多表连接
来源：http://pfx.chenjidiqi.icu

SELECT o.id, u.name, p.title FROM orders o
来源：http://cts.cashguo.top

JOIN users u ON u.id = o.user_id
来源：http://gcn.yonumen.top

JOIN products p ON p.id = o.product_id;
来源：http://lse.zhoulong.xyz

[Q42] 连接条件附加过滤
来源：http://mhf.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u
来源：http://jsb.mhx1999.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qdt.tanke756.top

[Q43] 标量子查询
来源：http://eau.jinghuilouyu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://esd.ivvv.top

[Q44] IN 子查询
来源：http://ugh.jinghuilouyu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jse.xingfuxueyuan.xyz

[Q45] EXISTS 判断存在
来源：http://ihs.gotoacloud.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kgz.cashguo.top

[Q46] NOT EXISTS 判断不存在
来源：http://azy.xingfuxueyuan.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rvw.316326.xyz

[Q47] 与平均值比较
来源：http://fmc.zdqjudy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gpo.nanxinkj.top

[Q48] CTE 公用表表达式
来源：http://uxw.yueranfly.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://apo.chenjidiqi.icu

SELECT * FROM t WHERE c > 5;
来源：http://jrb.ppjwa.cn

[Q49] 更新单行
来源：http://bcj.nanxuanxn.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://suv.cqqwz.cn

[Q50] 批量更新
来源：http://akb.tarul.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pud.yueranfly.top

[Q51] 用子查询更新
来源：http://err.sjlbkw.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bpw.316326.xyz

[Q52] 删除指定行
来源：http://gmt.yongpay.top

DELETE FROM users WHERE id = 10;
来源：http://pvf.9152youxi.cn

[Q53] 按条件删除
来源：http://zrz.fehbvm.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ctc.316326.xyz

[Q54] 清空表
来源：http://rau.316326.xyz

TRUNCATE TABLE logs;
来源：http://ptb.yj20258888.top

[Q55] 排名（并列占位）
来源：http://gpn.c1oappe.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://beq.zdqjudy.top

[Q56] 密集排名（并列不占位）
来源：http://tyr.c1oappe.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ilq.hcnkem.com

[Q57] 行号
来源：http://zbr.birdmap.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://etb.havefunace.top

[Q58] 累计求和
来源：http://gkq.haohaochexian.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wpu.zhaomingkeji.xyz

[Q59] 分组内累计
来源：http://ekv.daxiang520.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://njb.zhoulong.xyz

[Q60] 取上一行 / 下一行
来源：http://pup.zhongyouzk.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qdh.kuanghao11.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kvb.dashuyun.cn

[Q61] 移动平均
来源：http://obf.yvedp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://asx.smart0.xyz

[Q62] 分组占比
来源：http://xrc.feifeiyinyue.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fjy.sxryk.cn

[Q63] 开启事务
来源：http://yfv.iojbl.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vpc.xuetiantiany.cn

[Q64] 提交事务
来源：http://eon.quarkkingdee.top

COMMIT;
来源：http://svs.hywenlv.cn

[Q65] 回滚事务
来源：http://zqx.sufxvd.cn

ROLLBACK;
来源：http://kbp.hcnkem.com

[Q66] 行锁查询
来源：http://mji.yj20258.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jjp.fehbvm.com

[Q67] 设置隔离级别
来源：http://qdd.mhx1999.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qhy.cucudq.cn

[Q68] 保存点
来源：http://emv.cdnleiting.top

SAVEPOINT sp1;
来源：http://ohc.yvedp.cn

ROLLBACK TO sp1;
来源：http://atj.ybcxt.top

[Q69] 查看执行计划
来源：http://zkn.pycfn.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pop.iojbl.cn

[Q70] 更新统计信息
来源：http://vjy.redwolf501.top

ANALYZE TABLE users;
来源：http://upr.yueranfly.top

[Q71] 查看建表语句
来源：http://xnn.zhongyouzk.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cuu.xingfuxueyuan.xyz

[Q72] 查看索引
来源：http://gxz.pycfn.com

SHOW INDEX FROM users;
来源：http://uxh.guannengcc.top

[Q73] 查看表状态
来源：http://acy.52xcode.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wtj.shanyushiyangtech.top

[Q74] 强制使用索引
来源：http://qtj.hnqzz.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fpt.yvedp.cn

[Q75] 日期格式化
来源：http://xff.zhixingplan.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qld.ppjwa.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rri.dashuyun.cn

[Q76] 按天统计
来源：http://nid.svipenyu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jds.guowangkeji.top

[Q77] 时间加减
来源：http://kxg.zhaomingkeji.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fqt.jyoumei.cn

[Q78] 当前时间
来源：http://hrj.xylfe.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tzd.tianlin.xyz

[Q79] 字符串拼接
来源：http://uwi.shuidangran.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tng.tian-w.cn

[Q80] 字符串截取
来源：http://lpj.sysykeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lka.cashguo.top

[Q81] 字符串替换
来源：http://ruu.yj20258.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rij.havefunace.top

[Q82] 字符长度与字节长度
来源：http://sio.xziqi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lce.hywenlv.cn

[Q83] 大小写转换
来源：http://ibp.yangfankeji.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qqv.sjlbkw.cn

[Q84] 去除首尾空格
来源：http://lee.yj20258888.top

SELECT TRIM(name) FROM users;
来源：http://saw.cdnleiting.top

[Q85] 数值取整
来源：http://juv.jiagoushi.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://apf.ybcxt.top

[Q86] 读取 JSON 字段
来源：http://kyo.sxryk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cnx.xinyue.icu

[Q87] JSON 字段做条件
来源：http://iaz.zdbjq.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kew.xylfe.cn

[Q88] 行转列（条件聚合）
来源：http://ilt.9152youxi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gqe.yongpay.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bgv.hesvh.cn

[Q89] 判断表是否存在
来源：http://apb.xziqi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zvf.nanxuanxn.top

[Q90] 生成序号列
来源：http://wpa.ppjwa.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fsy.jqgufenzy.top

================================================================================
来源：http://fnd.c1oappe.top

R. Bash 专题
来源：http://xwq.yongpay.top

================================================================================
来源：http://mje.zhixingplan.top

[R01] shebang 与严格模式
来源：http://gun.0kj1m.cn

#!/usr/bin/env bash
来源：http://mpp.xuetiantiany.cn

set -euo pipefail
来源：http://gie.gaohongyu789.top

[R02] 变量赋值与使用
来源：http://oyt.shangyingyoupin.top

name="Tom"; echo "$name"
来源：http://gwz.andypj.xyz

[R03] 只读变量
来源：http://vxn.mhx1999.top

readonly PI=3.14
来源：http://xmd.aibaodan.cn

[R04] 位置参数
来源：http://ntp.wangshuangyany.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://off.zdbjq.cn

[R05] 参数默认值
来源：http://bmz.jqgfzy.top

name="${1:-default}"
来源：http://vfa.feifeiyinyue.top

[R06] 判断命令是否存在
来源：http://mkh.jyoumei.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tls.redwolf501.top

[R07] if 判断文件
来源：http://qfe.yonumen.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xzw.kuanghao11.cn

[R08] 数值比较
来源：http://hjv.yj20258888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://smv.yueranfly.top

[R09] 字符串比较
来源：http://vml.dashuyun.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bfo.yuanzhike.top

[R10] 正则匹配
来源：http://cop.nanxuanxn.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tqc.xingfuxueyuan.xyz

[R11] case 多分支
来源：http://esz.xylfe.cn

case "$1" in
来源：http://thj.tianlin.xyz

start) echo "启动" ;;
来源：http://chb.fktsv.cn

stop)  echo "停止" ;;
来源：http://otp.havefunace.top

*)     echo "未知命令" ;;
来源：http://ved.ppjwa.cn

esac
来源：http://sgn.fehbvm.com

[R12] for 遍历文件
来源：http://woi.ivvv.top

for f in *.txt; do echo "$f"; done
来源：http://cxd.nwbrower.top

[R13] for 计数循环
来源：http://yfl.wangshuangyany.cn

for i in {1..10}; do echo "$i"; done
来源：http://xtg.dianchejie.cn

[R14] C 风格 for
来源：http://qqi.dianchejie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://chz.yueranfly.top

[R15] while 逐行读文件
来源：http://bnh.pycfn.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://oaj.jlsjyb.cn

[R16] until 等待条件
来源：http://zyd.c1oappe.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qra.jqgfzy.top

[R17] 数组定义与取值
来源：http://deu.jyoumei.cn

arr=(a b c); echo "${arr[0]}"
来源：http://weq.ydzc1.top

[R18] 遍历数组
来源：http://ctl.jqgufenzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ssk.jqgfzy.top

[R19] 数组长度
来源：http://edx.guowangkeji.top

echo "${#arr[@]}"
来源：http://onn.tian-w.cn

[R20] 关联数组（字典）
来源：http://fbc.svipenyu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nob.daxiang520.top

[R21] 字符串长度
来源：http://yuq.zhaomingkeji.xyz

echo "${#s}"
来源：http://yhg.gotoacloud.top

[R22] 截取子串
来源：http://yyf.sufxvd.cn

echo "${s:0:5}"
来源：http://kir.daria6918.cn

[R23] 字符串替换
来源：http://wvu.chenjidiqi.icu

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tbi.sjlbkw.cn

[R24] 大小写转换
来源：http://dys.jianghu66.top

echo "${s^^}"; echo "${s,,}"
来源：http://thm.xinyue.icu

[R25] 去后缀 / 去前缀
来源：http://wnw.chenzaomai.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://fns.9152youxi.cn

[R26] 命令替换
来源：http://ndz.wangdashe.top

now=$(date +%F); echo "$now"
来源：http://zin.yangfankeji.com

[R27] 算术展开
来源：http://ytn.aibaodan.cn

echo $((1 + 2 * 3))
来源：http://acn.xingfuxueyuan.xyz

[R28] 浮点运算
来源：http://ijt.shanyushiyangkeji.top

echo "scale=2; 10/3" | bc
来源：http://vtr.haohaochexian.top

[R29] 定义函数
来源：http://lqn.tanke756.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cdt.yuanzhike.top

[R30] 函数返回状态码
来源：http://zij.snrcjt.cn

f() { return 0; }; f || echo "失败了"
来源：http://hdk.gogol.net.cn

[R31] 局部变量
来源：http://euu.zhoulong.xyz

f() { local x=1; echo "$x"; }
来源：http://twl.52xcode.cn

[R32] 参数个数校验
来源：http://jyt.gzhubu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fgt.sxryk.cn

[R33] 捕获错误并提示行号
来源：http://kvq.wangdashe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lqq.daria6918.cn

[R34] 退出时清理
来源：http://nhl.pycfn.com

trap 'rm -f "$tmp"' EXIT
来源：http://jfo.daxiang520.top

[R35] 后台执行并等待
来源：http://efr.smart0.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://ctl.shuidangran.top

[R36] 并发执行多个任务
来源：http://bhh.zhengqikj.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ixr.yuxming.cn

[R37] 把输出赋给变量
来源：http://ldu.sxryk.cn

files=$(ls -1)
来源：http://ejf.xuetiantiany.cn

[R38] 管道串联
来源：http://utd.birdmap.top

cat a.txt | grep -i error | wc -l
来源：http://vhd.hywenlv.cn

[R39] 重定向标准输出与错误
来源：http://dhw.zhijiandao.cn

cmd > out.log 2>&1
来源：http://rbn.hnxiangtu.top

[R40] 追加写日志
来源：http://ynu.sufxvd.cn

echo "log" >> out.log
来源：http://rfo.0kj1m.cn

[R41] 丢弃输出
来源：http://fph.fanxiaobao.xyz

cmd >/dev/null 2>&1
来源：http://syb.vehdjk.com

[R42] 输入重定向
来源：http://tjx.yonumen.top

wc -l < a.txt
来源：http://dzp.jqgfzy.top

[R43] 按名字查找文件
来源：http://bdc.316326.xyz

find . -name "*.log" -type f
来源：http://idk.guannengcc.top

[R44] 按修改时间查找
来源：http://ifn.hcnkem.com

find . -mtime -7 -type f
来源：http://twh.daxiang520.top

[R45] 批量删除
来源：http://njr.fzhhl.top

find . -name "*.tmp" -delete
来源：http://vpe.shzxlz.cn

[R46] 递归替换文件内容
来源：http://kpz.yuanzhike.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cao.birdmap.top

[R47] sed 单行替换
来源：http://nce.dashuyun.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cdy.hcnkem.com

[R48] awk 取指定列
来源：http://ugz.jinyuanbaomall.cn

awk '{print $1, $3}' a.txt
来源：http://ozm.zhoulong.xyz

[R49] awk 带条件
来源：http://xbj.mhx1999.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uuq.fehbvm.com

[R50] awk 求和
来源：http://ywt.vqdsnc.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ctw.zhoulong.xyz

[R51] 排序去重取前几
来源：http://vdb.fktsv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bdq.hongshengwenyu.top

[R52] 统计行数
来源：http://oue.xziqi.cn

wc -l a.txt
来源：http://rpo.hfpthk.cn

[R53] 查看文件头与实时尾
来源：http://gsr.zhijiandao.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wwn.jyoumei.cn

[R54] 比较两个文件
来源：http://wqg.yongpay.top

diff a.txt b.txt
来源：http://ans.chenlongwang.top

[R55] 压缩与解压
来源：http://qni.aizwys.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kie.jqgfzy.top

[R56] 远程拷贝
来源：http://ocu.cucudq.cn

scp file user@host:/path/
来源：http://sar.birdmap.top

[R57] 远程执行命令
来源：http://amf.jinqigufen.top

ssh user@host 'uptime'
来源：http://hmz.nanxuanxn.top

[R58] 下载文件
来源：http://xxi.yj202588.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qav.aibaodan.cn

[R59] 发 POST JSON
来源：http://gyq.yj202588.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ldn.sjlbkw.cn

[R60] 只看 HTTP 状态码
来源：http://mid.sxryk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yds.cdnleiting.top

[R61] 磁盘占用
来源：http://eot.tianlin.xyz

df -h;  du -sh *
来源：http://dvu.gogol.net.cn

[R62] 找最占空间的文件
来源：http://rud.aibaodan.cn

du -ah . | sort -rh | head -10
来源：http://vlu.vehdjk.com

[R63] 内存与进程
来源：http://ltx.zhijiandao.cn

free -h;  ps aux | grep nginx
来源：http://gct.ppjwa.cn

[R64] 结束进程
来源：http://nuh.xingfuxueyuan.xyz

kill -9 $(pgrep -f app.py)
来源：http://gqq.birdmap.top

[R65] 查看端口占用
来源：http://iep.0kj1m.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hbo.shangyingyoupin.top

[R66] 定时任务
来源：http://tso.feifeiyinyue.top

crontab -e;  crontab -l
来源：http://jqo.cashguo.top

[R67] 生成随机十六进制串
来源：http://jqe.wangdashe.top

openssl rand -hex 16
来源：http://vzv.xziqi.cn

[R68] 计算文件校验值
来源：http://sut.vehdjk.com

sha256sum a.txt;  md5sum a.txt
来源：http://xbj.yj20258.top

[R69] 生成随机密码
来源：http://rdg.sysykeji.top

head -c 16 /dev/urandom | base64
来源：http://obu.zhijiandao.cn

[R70] 时间戳与互转
来源：http://qxo.jyoumei.cn

date +%s;  date -d @1700000000
来源：http://dap.chenzaomai.com

[R71] 日期格式化
来源：http://ynt.pengpengdd.cyou

date +"%Y-%m-%d %H:%M:%S"
来源：http://lsi.xuetiantiany.cn

[R72] 等待端口就绪
来源：http://eow.tianlin.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://civ.chenlongwang.top

[R73] 分割大日志
来源：http://xay.jlsjyb.cn

split -l 1000 big.log part_
来源：http://yxs.gzhubu.top

[R74] 批量重命名
来源：http://sii.kuanghao11.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tpg.hammf.cn

[R75] 导出环境变量
来源：http://ibp.jinqigfzy.top

export PATH="$HOME/bin:$PATH"
来源：http://goz.chenzaomai.com

[R76] 使用临时文件
来源：http://ofz.shangyingyoupin.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cij.jqgufenzy.top

[R77] 读取用户输入
来源：http://stf.hongshengwenyu.top

read -rp "请输入: " ans
来源：http://fmx.cashguo.top

[R78] 交互式菜单
来源：http://wip.cheryme.top

select opt in a b c; do echo "$opt"; break; done
来源：http://sye.jinqigfzy.top

[R79] 解析命令行选项
来源：http://ifp.yvedp.cn


<!-- 参考信息 -->