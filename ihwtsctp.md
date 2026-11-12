代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ugo.zhiwuduotai.top

[Q05] 重命名列
来源：http://xcb.hcnkem.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uwe.yanxiufei.cn

[Q06] 删除列
来源：http://ldg.sjlbkw.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qve.dashuyun.cn

[Q07] 删除表
来源：http://aon.yj202588.top

DROP TABLE IF EXISTS orders;
来源：http://cvm.guannengcc.top

[Q08] 创建普通索引
来源：http://pbm.svipenyu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ntj.dashuyun.cn

[Q09] 创建唯一索引
来源：http://srs.quarkkingdee.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://aou.aibaodan.cn

[Q10] 插入单行
来源：http://sou.wangshuangyany.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dhc.yonumen.top

[Q11] 一次插入多行
来源：http://kai.yanxiufei.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hhu.nanxuanxn.top

[Q12] 插入后取自增 ID
来源：http://gni.jqgufenzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://gcl.fengsongda.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oct.dashuyun.cn

[Q13] 忽略重复插入
来源：http://zqj.zycfv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ssb.yongpay.top

[Q14] 存在则更新（upsert）
来源：http://weo.jqgfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ggq.aizwys.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://iem.tarul.cn

[Q15] 查询全部
来源：http://vps.yuxming.cn

SELECT * FROM users;
来源：http://njh.ywan-chungtsiang.top

[Q16] 查询指定列
来源：http://szq.zhengqikj.top

SELECT id, name FROM users;
来源：http://lva.zycfv.cn

[Q17] 条件查询
来源：http://sex.hammf.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sui.daxiang520.top

[Q18] 模糊匹配
来源：http://yji.tianlin.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kzq.zhaomingkeji.xyz

[Q19] 范围查询
来源：http://jpm.mhx1999.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cuk.dashuyun.cn

[Q20] IN 列表
来源：http://rnu.chenzaomai.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jxa.nanxuanxn.top

[Q21] 空值判断
来源：http://tyl.pycfn.com

SELECT * FROM users WHERE email IS NULL;
来源：http://vdz.xylfe.cn

[Q22] 排序
来源：http://ifq.smart0.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nfk.havefunace.top

[Q23] 分页
来源：http://jix.gotoacloud.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://osx.shuidangran.top

[Q24] 去重
来源：http://aea.yj20258888.top

SELECT DISTINCT city FROM users;
来源：http://fky.jlsjyb.cn

[Q25] 只取前 N 条
来源：http://beg.wangdashe.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sma.zhengqikj.top

[Q26] 计数
来源：http://mkh.yfazqb.com

SELECT COUNT(*) FROM users;
来源：http://rgh.yvedp.cn

[Q27] 条件计数
来源：http://dht.ydzc1.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vsw.zhoulong.xyz

[Q28] 求和与平均
来源：http://yfs.yfazqb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pxt.yongpay.top

[Q29] 最大最小值
来源：http://kfy.cucudq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vjw.gzhubu.top

[Q30] 分组统计
来源：http://ewf.tian-w.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fwl.jqgfzy.top

[Q31] 分组后过滤
来源：http://lre.ydjk.org.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nfi.yanxiufei.cn

[Q32] 分组拼接字符串
来源：http://pef.chenzaomai.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ejv.birdmap.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jdm.pengpengdd.cyou

[Q33] 多列分组
来源：http://wdt.hammf.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pxw.jinqigufen.top

[Q34] 每组取第一条
来源：http://tfr.shzxlz.cn

SELECT * FROM (
来源：http://grc.9152youxi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uwu.snrcjt.cn

) t WHERE rn = 1;
来源：http://jgt.gogol.net.cn

[Q35] 内连接
来源：http://kcy.jqgufenzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://huc.wangshuangyany.cn

[Q36] 左连接
来源：http://sef.hcnkem.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://iuj.jinqigufen.top

[Q37] 右连接
来源：http://bgi.dashuyun.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ggj.uphjek.com

[Q38] 全外连接（PostgreSQL）
来源：http://stn.xuanzx.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pyh.havefunace.top

[Q39] 自连接（查上下级）
来源：http://sde.kuanghao11.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kzs.xinyue.icu

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kmf.zhongyouzk.top

[Q40] 交叉连接（笛卡尔积）
来源：http://haf.jinghuilouyu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zte.jiagoushi.top

[Q41] 多表连接
来源：http://aci.jlsjyb.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uks.fzhhl.top

JOIN users u ON u.id = o.user_id
来源：http://knp.hnqzz.top

JOIN products p ON p.id = o.product_id;
来源：http://qfl.jianghu66.top

[Q42] 连接条件附加过滤
来源：http://vyv.yj202588.top

SELECT u.name, o.amount FROM users u
来源：http://lpa.yanxiufei.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rql.fanxiaobao.xyz

[Q43] 标量子查询
来源：http://jns.xuetiantiany.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fxs.feifeiyinyue.top

[Q44] IN 子查询
来源：http://uoc.vqdsnc.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pxa.fanxiaobao.xyz

[Q45] EXISTS 判断存在
来源：http://ldm.pengpengdd.cyou

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://clb.ybcxt.top

[Q46] NOT EXISTS 判断不存在
来源：http://dmt.uphjek.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kwk.jianghu66.top

[Q47] 与平均值比较
来源：http://gvt.chenzaomai.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yxx.ywan-chungtsiang.top

[Q48] CTE 公用表表达式
来源：http://kye.ydzc1.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zvw.yueranfly.top

SELECT * FROM t WHERE c > 5;
来源：http://bcb.bjfxy.top

[Q49] 更新单行
来源：http://xmj.cdnleiting.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sbf.jqgufenzy.top

[Q50] 批量更新
来源：http://knj.shanyushiyangtech.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tpm.nwbrower.top

[Q51] 用子查询更新
来源：http://ujd.ydzc1.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uqm.0kj1m.cn

[Q52] 删除指定行
来源：http://yyx.aizwys.cn

DELETE FROM users WHERE id = 10;
来源：http://ult.yanxiufei.cn

[Q53] 按条件删除
来源：http://trl.0kj1m.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://udf.yvedp.cn

[Q54] 清空表
来源：http://zha.iojbl.cn

TRUNCATE TABLE logs;
来源：http://sxe.cqqwz.cn

[Q55] 排名（并列占位）
来源：http://uxz.daria6918.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zzu.zhiwuduotai.top

[Q56] 密集排名（并列不占位）
来源：http://ahr.jinqigufen.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uft.yuanzhike.top

[Q57] 行号
来源：http://mhc.yangfankeji.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pkn.zhixingplan.top

[Q58] 累计求和
来源：http://zho.dashuyun.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jrd.sxryk.cn

[Q59] 分组内累计
来源：http://pqx.vqdsnc.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://chg.svipenyu.cn

[Q60] 取上一行 / 下一行
来源：http://eui.kuanghao11.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xsw.snrcjt.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hwj.tianlin.xyz

[Q61] 移动平均
来源：http://hua.meibo888.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://olz.jinyuanbaomall.cn

[Q62] 分组占比
来源：http://mew.shuidangran.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://szr.svipenyu.cn

[Q63] 开启事务
来源：http://zdx.hesvh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hxz.zhixingplan.top

[Q64] 提交事务
来源：http://dba.fzhhl.top

COMMIT;
来源：http://nna.redwolf501.top

[Q65] 回滚事务
来源：http://esh.uphjek.com

ROLLBACK;
来源：http://zjx.yvedp.cn

[Q66] 行锁查询
来源：http://pxq.sweek.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pqn.hysaishi.cn

[Q67] 设置隔离级别
来源：http://kvz.yvedp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fwf.xuetiantiany.cn

[Q68] 保存点
来源：http://jni.fengsongda.top

SAVEPOINT sp1;
来源：http://kxt.xziqi.cn

ROLLBACK TO sp1;
来源：http://kip.tarul.cn

[Q69] 查看执行计划
来源：http://fog.dashuyun.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://aeo.xingfuxueyuan.xyz

[Q70] 更新统计信息
来源：http://zzs.zhongyouzk.top

ANALYZE TABLE users;
来源：http://eje.zhengqikj.top

[Q71] 查看建表语句
来源：http://khs.hesvh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lwn.yanxiufei.cn

[Q72] 查看索引
来源：http://hoz.xylfe.cn

SHOW INDEX FROM users;
来源：http://mpa.ctjpmb.com

[Q73] 查看表状态
来源：http://vxi.aizwys.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wmu.cashguo.top

[Q74] 强制使用索引
来源：http://uxm.jinyuanbaomall.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hsn.tarul.cn

[Q75] 日期格式化
来源：http://kio.yangfankeji.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vgn.yvedp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qkl.daxiang520.top

[Q76] 按天统计
来源：http://wkm.guannengcc.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tli.jinqigfzy.top

[Q77] 时间加减
来源：http://bqf.cashguo.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://znz.xylfe.cn

[Q78] 当前时间
来源：http://ozj.hywenlv.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ezd.jinyuanbaomall.cn

[Q79] 字符串拼接
来源：http://nmc.zhaomingkeji.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uos.ehwqpu.com

[Q80] 字符串截取
来源：http://fcy.cashguo.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yxa.xylfe.cn

[Q81] 字符串替换
来源：http://lhz.uphjek.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yzj.ppjwa.cn

[Q82] 字符长度与字节长度
来源：http://ncf.sysykeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mjs.kuanghao11.cn

[Q83] 大小写转换
来源：http://erb.fengsongda.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ygs.yueranfly.top

[Q84] 去除首尾空格
来源：http://htt.yanxiufei.cn

SELECT TRIM(name) FROM users;
来源：http://kuf.nanxinkj.top

[Q85] 数值取整
来源：http://plq.jinqigfzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ckk.dianchejie.cn

[Q86] 读取 JSON 字段
来源：http://fia.nwbrower.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pgw.cheryme.top

[Q87] JSON 字段做条件
来源：http://geb.ywan-chungtsiang.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vsn.chenjidiqi.icu

[Q88] 行转列（条件聚合）
来源：http://ker.chenzaomai.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://loz.gogol.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bto.tarul.cn

[Q89] 判断表是否存在
来源：http://siq.zhongyouzk.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ono.sysykeji.top

[Q90] 生成序号列
来源：http://tzs.daria6918.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://izt.zdqjudy.top

================================================================================
来源：http://upq.zhiwuduotai.top

R. Bash 专题
来源：http://ccm.yj20258888.top

================================================================================
来源：http://toe.zhiwuduotai.top

[R01] shebang 与严格模式
来源：http://zfk.shanyushiyangtech.top

#!/usr/bin/env bash
来源：http://qgq.zhongyouzk.top

set -euo pipefail
来源：http://hgi.shangyingyoupin.top

[R02] 变量赋值与使用
来源：http://yfi.zhijiandao.cn

name="Tom"; echo "$name"
来源：http://whf.yonumen.top

[R03] 只读变量
来源：http://aoo.vqdsnc.cn

readonly PI=3.14
来源：http://hot.zhixingplan.top

[R04] 位置参数
来源：http://tif.ydjk.org.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yrg.316326.xyz

[R05] 参数默认值
来源：http://fzz.316326.xyz

name="${1:-default}"
来源：http://vwv.nwbrower.top

[R06] 判断命令是否存在
来源：http://jkw.bjfxy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://znh.tianlin.xyz

[R07] if 判断文件
来源：http://jyp.zhixingplan.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tyk.jyoumei.cn

[R08] 数值比较
来源：http://ruu.ehwqpu.com

if (( a > b )); then echo "a 更大"; fi
来源：http://nem.wangdashe.top

[R09] 字符串比较
来源：http://fdu.hfpthk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sho.cucudq.cn

[R10] 正则匹配
来源：http://dgm.yuxming.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rdk.yj202588.top

[R11] case 多分支
来源：http://rrj.yj20258888.top

case "$1" in
来源：http://nvl.hammf.cn

start) echo "启动" ;;
来源：http://uyy.jqgfzy.top

stop)  echo "停止" ;;
来源：http://ujk.svipenyu.cn

*)     echo "未知命令" ;;
来源：http://jmb.52xcode.cn

esac
来源：http://sfy.hysaishi.cn

[R12] for 遍历文件
来源：http://zge.fktsv.cn

for f in *.txt; do echo "$f"; done
来源：http://deu.yuanzhike.top

[R13] for 计数循环
来源：http://ecc.uphjek.com

for i in {1..10}; do echo "$i"; done
来源：http://qru.ppjwa.cn

[R14] C 风格 for
来源：http://xam.hammf.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yll.vehdjk.com

[R15] while 逐行读文件
来源：http://bsi.gogol.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://oui.yanxiufei.cn

[R16] until 等待条件
来源：http://vng.yuanzhike.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pek.nanxuanxn.top

[R17] 数组定义与取值
来源：http://zwa.xuanzx.com

arr=(a b c); echo "${arr[0]}"
来源：http://trr.nanxinkj.top

[R18] 遍历数组
来源：http://iya.sysykeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tji.vqdsnc.cn

[R19] 数组长度
来源：http://ojw.0kj1m.cn

echo "${#arr[@]}"
来源：http://uyp.yueranfly.top

[R20] 关联数组（字典）
来源：http://tjc.redwolf501.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xve.bjfxy.top

[R21] 字符串长度
来源：http://cxl.nwbrower.top

echo "${#s}"
来源：http://tiy.andypj.xyz

[R22] 截取子串
来源：http://eax.xuanzx.com

echo "${s:0:5}"
来源：http://ele.jqgfzy.top

[R23] 字符串替换
来源：http://eaz.nanxinkj.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eun.nanxuanxn.top

[R24] 大小写转换
来源：http://cib.tanke756.top

echo "${s^^}"; echo "${s,,}"
来源：http://qyf.hesvh.cn

[R25] 去后缀 / 去前缀
来源：http://lpa.jlsjyb.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xyx.hnxiangtu.top

[R26] 命令替换
来源：http://fby.guowangkeji.top

now=$(date +%F); echo "$now"
来源：http://tvd.gogol.net.cn

[R27] 算术展开
来源：http://iyo.zhaomingkeji.xyz

echo $((1 + 2 * 3))
来源：http://wib.iojbl.cn

[R28] 浮点运算
来源：http://mdb.zhoulong.xyz

echo "scale=2; 10/3" | bc
来源：http://ldc.aizwys.cn

[R29] 定义函数
来源：http://ebe.tian-w.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dnq.shuidangran.top

[R30] 函数返回状态码
来源：http://udg.hysaishi.cn

f() { return 0; }; f || echo "失败了"
来源：http://uvq.redwolf501.top

[R31] 局部变量
来源：http://xvq.yj20258888.top

f() { local x=1; echo "$x"; }
来源：http://fwn.vqdsnc.cn

[R32] 参数个数校验
来源：http://gal.vehdjk.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://idh.sysykeji.top

[R33] 捕获错误并提示行号
来源：http://urq.redwolf501.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vnh.tianlin.xyz

[R34] 退出时清理
来源：http://dax.ppjwa.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tsg.316326.xyz

[R35] 后台执行并等待
来源：http://tmo.ywan-chungtsiang.top

sleep 5 & pid=$!; wait "$pid"
来源：http://aay.nanxinkj.top

[R36] 并发执行多个任务
来源：http://uxh.yangfankeji.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gku.hcnkem.com

[R37] 把输出赋给变量
来源：http://suh.hammf.cn

files=$(ls -1)
来源：http://sfw.epnwcf.com

[R38] 管道串联
来源：http://xkj.zycfv.cn

cat a.txt | grep -i error | wc -l
来源：http://avq.gogol.net.cn

[R39] 重定向标准输出与错误
来源：http://dlz.9152youxi.cn

cmd > out.log 2>&1
来源：http://hev.ivvv.top

[R40] 追加写日志
来源：http://xaa.cashguo.top

echo "log" >> out.log
来源：http://crl.gaohongyu789.top

[R41] 丢弃输出
来源：http://yug.iojbl.cn

cmd >/dev/null 2>&1
来源：http://tfr.yongpay.top

[R42] 输入重定向
来源：http://pyq.fzhhl.top

wc -l < a.txt
来源：http://zal.jiagoushi.top

[R43] 按名字查找文件
来源：http://gxg.chenjidiqi.icu

find . -name "*.log" -type f
来源：http://ecb.hammf.cn

[R44] 按修改时间查找
来源：http://ads.meibo888.top

find . -mtime -7 -type f
来源：http://nwv.yongpay.top

[R45] 批量删除
来源：http://nmi.fktsv.cn

find . -name "*.tmp" -delete
来源：http://hrz.jianghu66.top

[R46] 递归替换文件内容
来源：http://lci.shuidangran.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gtx.uphjek.com

[R47] sed 单行替换
来源：http://jtv.xuetiantiany.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mor.yongpay.top

[R48] awk 取指定列
来源：http://qoc.hnqzz.top

awk '{print $1, $3}' a.txt
来源：http://qav.ywan-chungtsiang.top

[R49] awk 带条件
来源：http://sxb.hnqzz.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://quk.chenzaomai.com

[R50] awk 求和
来源：http://sto.jyoumei.cn

awk '{s += $2} END {print s}' a.txt
来源：http://syz.cdnleiting.top

[R51] 排序去重取前几
来源：http://rvw.jiagoushi.top

sort a.txt | uniq -c | sort -rn | head
来源：http://zqa.daria6918.cn

[R52] 统计行数
来源：http://buk.fehbvm.com

wc -l a.txt
来源：http://ncm.xingfuxueyuan.xyz

[R53] 查看文件头与实时尾
来源：http://son.zdbjq.cn


<!-- 参考信息 -->