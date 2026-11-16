代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rrr.tarul.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vqz.hcnkem.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mkj.daria6918.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fap.xuanzx.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fhz.yfazqb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zwi.xziqi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jww.ywan-chungtsiang.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://scv.tarul.cn

================================================================================
来源：http://tkq.shangyingyoupin.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kxr.zhiwuduotai.top

================================================================================
来源：http://eog.shuidangran.top

[Q01] 创建表
来源：http://hxs.gogol.net.cn

CREATE TABLE users (
来源：http://rgw.jqgufenzy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kmf.redwolf501.top

name VARCHAR(50) NOT NULL,
来源：http://wxk.hammf.cn

email VARCHAR(100) UNIQUE,
来源：http://vre.yuxming.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gbp.svipenyu.cn

);
来源：http://owd.wangshuangyany.cn

[Q02] 创建带外键的表
来源：http://kgx.tanke756.top

CREATE TABLE orders (
来源：http://mvu.chenlongwang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ukv.sufxvd.cn

user_id INT NOT NULL,
来源：http://qst.yj20258888.top

amount DECIMAL(10, 2),
来源：http://gsh.cheryme.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ogu.cashguo.top

);
来源：http://vyq.aizwys.cn

[Q03] 增加列
来源：http://gtq.yj20258888.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uas.zycfv.cn

[Q04] 修改列类型
来源：http://afe.yanxiufei.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sok.fanxiaobao.xyz

[Q05] 重命名列
来源：http://moy.yangfankeji.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mnf.tanke756.top

[Q06] 删除列
来源：http://cmx.kuanghao11.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yeb.yonumen.top

[Q07] 删除表
来源：http://puo.yueranfly.top

DROP TABLE IF EXISTS orders;
来源：http://ces.redwolf501.top

[Q08] 创建普通索引
来源：http://iyv.jqgufenzy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://onm.xinyue.icu

[Q09] 创建唯一索引
来源：http://kol.sjlbkw.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lwe.nanxuanxn.top

[Q10] 插入单行
来源：http://fhm.ywan-chungtsiang.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zam.cashguo.top

[Q11] 一次插入多行
来源：http://jos.jianghu66.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qgs.hnqzz.top

[Q12] 插入后取自增 ID
来源：http://ufm.meibo888.top

INSERT INTO users (name) VALUES ('C');
来源：http://khe.yj20258.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rwm.yueranfly.top

[Q13] 忽略重复插入
来源：http://pgo.zhiwuduotai.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://unl.xuetiantiany.cn

[Q14] 存在则更新（upsert）
来源：http://gjj.ctjpmb.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rkx.nwbrower.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qyc.kuanghao11.cn

[Q15] 查询全部
来源：http://qsz.yanxiufei.cn

SELECT * FROM users;
来源：http://hvi.jinqigufen.top

[Q16] 查询指定列
来源：http://cyi.zhoulong.xyz

SELECT id, name FROM users;
来源：http://byq.daxiang520.top

[Q17] 条件查询
来源：http://tei.ybcxt.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qji.zhoulong.xyz

[Q18] 模糊匹配
来源：http://tts.shanyushiyangtech.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ifc.jlsjyb.cn

[Q19] 范围查询
来源：http://tpc.guannengcc.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cgf.jianghu66.top

[Q20] IN 列表
来源：http://vzr.xylfe.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hbe.52xcode.cn

[Q21] 空值判断
来源：http://wtz.hammf.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xce.fehbvm.com

[Q22] 排序
来源：http://gvc.316326.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nhg.cucudq.cn

[Q23] 分页
来源：http://lyi.gzhubu.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bee.zhiwuduotai.top

[Q24] 去重
来源：http://hge.shuidangran.top

SELECT DISTINCT city FROM users;
来源：http://glr.316326.xyz

[Q25] 只取前 N 条
来源：http://yvu.guowangkeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://otj.snrcjt.cn

[Q26] 计数
来源：http://rsv.ydjk.org.cn

SELECT COUNT(*) FROM users;
来源：http://nbh.dashuyun.cn

[Q27] 条件计数
来源：http://rft.vehdjk.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lbb.ybcxt.top

[Q28] 求和与平均
来源：http://vsh.havefunace.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vso.gaohongyu789.top

[Q29] 最大最小值
来源：http://wcx.yj20258888.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://tvz.9152youxi.cn

[Q30] 分组统计
来源：http://sts.xuetiantiany.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bmq.hcnkem.com

[Q31] 分组后过滤
来源：http://age.xuanzx.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://oyx.shanyushiyangkeji.top

[Q32] 分组拼接字符串
来源：http://abo.wangshuangyany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ktm.sxryk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yvv.hnxiangtu.top

[Q33] 多列分组
来源：http://gjl.zhijiandao.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nsx.iojbl.cn

[Q34] 每组取第一条
来源：http://tjs.jqgufenzy.top

SELECT * FROM (
来源：http://zqb.fktsv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zcc.ctjpmb.com

) t WHERE rn = 1;
来源：http://asa.gaohongyu789.top

[Q35] 内连接
来源：http://iky.ppjwa.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://djx.xingfuxueyuan.xyz

[Q36] 左连接
来源：http://xdd.guowangkeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fui.fzhhl.top

[Q37] 右连接
来源：http://asj.birdmap.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ttx.zhiwuduotai.top

[Q38] 全外连接（PostgreSQL）
来源：http://iuz.yj202588.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tna.jqgufenzy.top

[Q39] 自连接（查上下级）
来源：http://fnz.tarul.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://mnk.zhaomingkeji.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tzf.jqgfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ipb.cdnleiting.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bzf.yj20258.top

[Q41] 多表连接
来源：http://auw.fengsongda.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://yha.9152youxi.cn

JOIN users u ON u.id = o.user_id
来源：http://vro.zhiwuduotai.top

JOIN products p ON p.id = o.product_id;
来源：http://ezj.zdqjudy.top

[Q42] 连接条件附加过滤
来源：http://tlq.jqgfzy.top

SELECT u.name, o.amount FROM users u
来源：http://xrs.shanyushiyangkeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://omq.316326.xyz

[Q43] 标量子查询
来源：http://rbt.fktsv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bro.jqgufenzy.top

[Q44] IN 子查询
来源：http://pef.cheryme.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dga.feifeiyinyue.top

[Q45] EXISTS 判断存在
来源：http://fiz.ywan-chungtsiang.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ouc.tianlin.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://pwu.chenjidiqi.icu

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jgn.ydjk.org.cn

[Q47] 与平均值比较
来源：http://yah.9152youxi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://beq.chenjidiqi.icu

[Q48] CTE 公用表表达式
来源：http://twv.guowangkeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://aze.zhiwuduotai.top

SELECT * FROM t WHERE c > 5;
来源：http://ygp.hnqzz.top

[Q49] 更新单行
来源：http://byr.pycfn.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mjq.cdnleiting.top

[Q50] 批量更新
来源：http://rup.nwbrower.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://laf.chenjidiqi.icu

[Q51] 用子查询更新
来源：http://vma.jinghuilouyu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dhe.meibo888.top

[Q52] 删除指定行
来源：http://mfz.sjlbkw.cn

DELETE FROM users WHERE id = 10;
来源：http://qcz.quarkkingdee.top

[Q53] 按条件删除
来源：http://zpq.epnwcf.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rdo.hywenlv.cn

[Q54] 清空表
来源：http://bet.fengsongda.top

TRUNCATE TABLE logs;
来源：http://nxc.yfazqb.com

[Q55] 排名（并列占位）
来源：http://xkw.hongshengwenyu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jje.jinghuilouyu.cn

[Q56] 密集排名（并列不占位）
来源：http://hkw.jinqigfzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sim.shzxlz.cn

[Q57] 行号
来源：http://vlj.pycfn.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://osa.cucudq.cn

[Q58] 累计求和
来源：http://bfv.hcnkem.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wpj.fanxiaobao.xyz

[Q59] 分组内累计
来源：http://uhk.smart0.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zdy.daxiang520.top

[Q60] 取上一行 / 下一行
来源：http://gnm.zhixingplan.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hrx.yuxming.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qhw.zhoulong.xyz

[Q61] 移动平均
来源：http://dzg.sufxvd.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mld.yj20258.top

[Q62] 分组占比
来源：http://vlr.chenlongwang.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wls.tanke756.top

[Q63] 开启事务
来源：http://enc.hesvh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wfx.sweek.top

[Q64] 提交事务
来源：http://rig.zhoulong.xyz

COMMIT;
来源：http://thr.sxryk.cn

[Q65] 回滚事务
来源：http://phl.cucudq.cn

ROLLBACK;
来源：http://nif.hongshengwenyu.top

[Q66] 行锁查询
来源：http://nyf.jlsjyb.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rts.yj202588.top

[Q67] 设置隔离级别
来源：http://jdz.xingfuxueyuan.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hax.bbcook.cn

[Q68] 保存点
来源：http://fqa.nanxuanxn.top

SAVEPOINT sp1;
来源：http://iyv.jqgufenzy.top

ROLLBACK TO sp1;
来源：http://xkq.yongpay.top

[Q69] 查看执行计划
来源：http://ijt.guowangkeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gxp.zdbjq.cn

[Q70] 更新统计信息
来源：http://vne.sufxvd.cn

ANALYZE TABLE users;
来源：http://yfo.vqdsnc.cn

[Q71] 查看建表语句
来源：http://utw.shanyushiyangtech.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ejg.hongshengwenyu.top

[Q72] 查看索引
来源：http://drd.sufxvd.cn

SHOW INDEX FROM users;
来源：http://ore.gzhubu.top

[Q73] 查看表状态
来源：http://xuw.hongshengwenyu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://pvr.0kj1m.cn

[Q74] 强制使用索引
来源：http://nvj.ybcxt.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jct.gaohongyu789.top

[Q75] 日期格式化
来源：http://vyo.yuanzhike.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://awi.uphjek.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tmo.ppjwa.cn

[Q76] 按天统计
来源：http://iif.shangyingyoupin.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://epi.hfpthk.cn

[Q77] 时间加减
来源：http://kxx.gzhubu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ixo.jqgufenzy.top

[Q78] 当前时间
来源：http://qaf.hesvh.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jsw.tian-w.cn

[Q79] 字符串拼接
来源：http://epp.gotoacloud.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wer.hysaishi.cn

[Q80] 字符串截取
来源：http://ubi.shzxlz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lzf.ydzc1.top

[Q81] 字符串替换
来源：http://xir.guowangkeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://flv.chenjidiqi.icu

[Q82] 字符长度与字节长度
来源：http://lke.hnxiangtu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fiy.uphjek.com

[Q83] 大小写转换
来源：http://inm.wangdashe.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://snf.havefunace.top

[Q84] 去除首尾空格
来源：http://apq.yongpay.top

SELECT TRIM(name) FROM users;
来源：http://djt.ppjwa.cn

[Q85] 数值取整
来源：http://hzt.fengsongda.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lzk.yj202588.top

[Q86] 读取 JSON 字段
来源：http://onp.guannengcc.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://oju.hywenlv.cn

[Q87] JSON 字段做条件
来源：http://knc.quarkkingdee.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oxx.xuanzx.com

[Q88] 行转列（条件聚合）
来源：http://hij.xziqi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nrb.ehwqpu.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jkc.yuanzhike.top

[Q89] 判断表是否存在
来源：http://stx.jinqigufen.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hmu.jinyuanbaomall.cn

[Q90] 生成序号列
来源：http://urf.c1oappe.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lvp.quarkkingdee.top

================================================================================
来源：http://eet.yanxiufei.cn

R. Bash 专题
来源：http://fid.pycfn.com

================================================================================
来源：http://fqm.cheryme.top

[R01] shebang 与严格模式
来源：http://bkh.ywan-chungtsiang.top

#!/usr/bin/env bash
来源：http://omi.nanxuanxn.top

set -euo pipefail
来源：http://wlr.yj20258888.top

[R02] 变量赋值与使用
来源：http://twj.yueranfly.top

name="Tom"; echo "$name"
来源：http://xll.fktsv.cn

[R03] 只读变量
来源：http://zxg.yuanzhike.top

readonly PI=3.14
来源：http://dda.hongshengwenyu.top

[R04] 位置参数
来源：http://omq.chenjidiqi.icu

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ojt.andypj.xyz

[R05] 参数默认值
来源：http://jlo.hnqzz.top

name="${1:-default}"
来源：http://vuy.cucudq.cn

[R06] 判断命令是否存在
来源：http://xyf.yuxming.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zid.316326.xyz

[R07] if 判断文件
来源：http://vds.gogol.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://eqm.guannengcc.top

[R08] 数值比较
来源：http://ltb.hnxiangtu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://syz.daxiang520.top

[R09] 字符串比较
来源：http://gdv.yfazqb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://foy.smart0.xyz

[R10] 正则匹配
来源：http://vje.xuanzx.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pbu.shuidangran.top

[R11] case 多分支
来源：http://xtc.shanyushiyangkeji.top

case "$1" in
来源：http://aym.fktsv.cn

start) echo "启动" ;;
来源：http://ypk.wangshuangyany.cn

stop)  echo "停止" ;;
来源：http://wuq.shanyushiyangtech.top

*)     echo "未知命令" ;;
来源：http://xqr.hnxiangtu.top

esac
来源：http://ycg.zhengqikj.top

[R12] for 遍历文件
来源：http://psd.yj20258888.top

for f in *.txt; do echo "$f"; done
来源：http://hdu.cucudq.cn

[R13] for 计数循环
来源：http://lxn.jianghu66.top

for i in {1..10}; do echo "$i"; done
来源：http://vyc.yj20258888.top

[R14] C 风格 for
来源：http://lkw.shuidangran.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://idm.jyoumei.cn

[R15] while 逐行读文件
来源：http://yit.hammf.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://omz.daria6918.cn

[R16] until 等待条件
来源：http://iuf.bbcook.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vwp.gotoacloud.top

[R17] 数组定义与取值
来源：http://wxc.ctjpmb.com

arr=(a b c); echo "${arr[0]}"
来源：http://yrd.yuxming.cn

[R18] 遍历数组
来源：http://pdq.sxryk.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mlw.zdqjudy.top

[R19] 数组长度
来源：http://jvt.daria6918.cn

echo "${#arr[@]}"
来源：http://zyy.xuetiantiany.cn

[R20] 关联数组（字典）
来源：http://uhz.cdnleiting.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mld.fktsv.cn

[R21] 字符串长度
来源：http://lqt.shanyushiyangkeji.top

echo "${#s}"
来源：http://ymh.uphjek.com

[R22] 截取子串
来源：http://zxa.chenzaomai.com

echo "${s:0:5}"
来源：http://yrx.hnxiangtu.top

[R23] 字符串替换
来源：http://xtp.0kj1m.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://btm.nanxuanxn.top

[R24] 大小写转换
来源：http://uvx.ywan-chungtsiang.top

echo "${s^^}"; echo "${s,,}"
来源：http://yup.sufxvd.cn

[R25] 去后缀 / 去前缀
来源：http://lpz.sysykeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ynh.ctjpmb.com

[R26] 命令替换
来源：http://qig.svipenyu.cn

now=$(date +%F); echo "$now"
来源：http://vuv.wangdashe.top

[R27] 算术展开
来源：http://gzf.guannengcc.top

echo $((1 + 2 * 3))
来源：http://iwo.zdbjq.cn

[R28] 浮点运算
来源：http://tnr.xylfe.cn

echo "scale=2; 10/3" | bc
来源：http://lkb.xinyue.icu

[R29] 定义函数
来源：http://iks.ctjpmb.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mza.hnxiangtu.top

[R30] 函数返回状态码
来源：http://vfn.tanke756.top

f() { return 0; }; f || echo "失败了"
来源：http://fxw.aibaodan.cn

[R31] 局部变量
来源：http://ala.shanyushiyangkeji.top

f() { local x=1; echo "$x"; }
来源：http://zfq.tianlin.xyz

[R32] 参数个数校验
来源：http://kmq.chenzaomai.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hwr.yfazqb.com

[R33] 捕获错误并提示行号
来源：http://ybe.fehbvm.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zax.zhongyouzk.top

[R34] 退出时清理
来源：http://dhy.shanyushiyangtech.top

trap 'rm -f "$tmp"' EXIT
来源：http://ice.tianlin.xyz

[R35] 后台执行并等待
来源：http://byi.xziqi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xjk.zycfv.cn

[R36] 并发执行多个任务
来源：http://iwu.xinyue.icu

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://spa.gzhubu.top

[R37] 把输出赋给变量
来源：http://ghz.dianchejie.cn

files=$(ls -1)
来源：http://fnm.zhiwuduotai.top

[R38] 管道串联
来源：http://nce.sweek.top

cat a.txt | grep -i error | wc -l
来源：http://ich.dianchejie.cn

[R39] 重定向标准输出与错误
来源：http://hec.zhaomingkeji.xyz


<!-- 参考信息 -->