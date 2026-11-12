代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://atg.meibo888.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sbn.dianchejie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://afz.ywan-chungtsiang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ush.xylfe.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cvn.xuanzx.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dtm.xuetiantiany.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ikx.gaohongyu789.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fgs.fengsongda.top

================================================================================
来源：http://ovb.jiagoushi.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qde.gotoacloud.top

================================================================================
来源：http://smq.snrcjt.cn

[Q01] 创建表
来源：http://qhg.yj202588.top

CREATE TABLE users (
来源：http://taa.zdqjudy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ycf.birdmap.top

name VARCHAR(50) NOT NULL,
来源：http://fnd.hywenlv.cn

email VARCHAR(100) UNIQUE,
来源：http://gho.gotoacloud.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hzc.gzhubu.top

);
来源：http://sku.birdmap.top

[Q02] 创建带外键的表
来源：http://gao.guannengcc.top

CREATE TABLE orders (
来源：http://jpz.redwolf501.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wjw.jinqigufen.top

user_id INT NOT NULL,
来源：http://qap.52xcode.cn

amount DECIMAL(10, 2),
来源：http://bdb.gogol.net.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ysm.smart0.xyz

);
来源：http://yye.iojbl.cn

[Q03] 增加列
来源：http://vrb.daria6918.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xbp.9152youxi.cn

[Q04] 修改列类型
来源：http://qel.hnxiangtu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jtr.smart0.xyz

[Q05] 重命名列
来源：http://kcz.ctjpmb.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yub.daxiang520.top

[Q06] 删除列
来源：http://rch.tianlin.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://nau.yanxiufei.cn

[Q07] 删除表
来源：http://sah.daxiang520.top

DROP TABLE IF EXISTS orders;
来源：http://kyq.nwbrower.top

[Q08] 创建普通索引
来源：http://vzh.birdmap.top

CREATE INDEX idx_users_email ON users(email);
来源：http://mlg.ybcxt.top

[Q09] 创建唯一索引
来源：http://pcf.yuanzhike.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wta.meibo888.top

[Q10] 插入单行
来源：http://kwm.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ert.havefunace.top

[Q11] 一次插入多行
来源：http://hhx.bbcook.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hag.guannengcc.top

[Q12] 插入后取自增 ID
来源：http://khr.jqgufenzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://zwd.guowangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tde.guowangkeji.top

[Q13] 忽略重复插入
来源：http://oks.chenjidiqi.icu

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rjm.zhijiandao.cn

[Q14] 存在则更新（upsert）
来源：http://cgx.cashguo.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qyt.bjfxy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pfd.haohaochexian.top

[Q15] 查询全部
来源：http://dfd.daria6918.cn

SELECT * FROM users;
来源：http://pff.jinyuanbaomall.cn

[Q16] 查询指定列
来源：http://koy.cheryme.top

SELECT id, name FROM users;
来源：http://urb.jyoumei.cn

[Q17] 条件查询
来源：http://vxi.chenzaomai.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dwh.jiagoushi.top

[Q18] 模糊匹配
来源：http://den.zhiwuduotai.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://auz.shuidangran.top

[Q19] 范围查询
来源：http://hgg.cdnleiting.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jaj.ydzc1.top

[Q20] IN 列表
来源：http://wcu.mhx1999.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://htr.316326.xyz

[Q21] 空值判断
来源：http://hlq.jianghu66.top

SELECT * FROM users WHERE email IS NULL;
来源：http://svj.dianchejie.cn

[Q22] 排序
来源：http://dai.svipenyu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ovy.daria6918.cn

[Q23] 分页
来源：http://bzt.nanxuanxn.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jtj.uphjek.com

[Q24] 去重
来源：http://kmi.cqqwz.cn

SELECT DISTINCT city FROM users;
来源：http://ryp.ppjwa.cn

[Q25] 只取前 N 条
来源：http://qwj.yvedp.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gmk.zhijiandao.cn

[Q26] 计数
来源：http://qel.ctjpmb.com

SELECT COUNT(*) FROM users;
来源：http://jeu.0kj1m.cn

[Q27] 条件计数
来源：http://gqi.ydjk.org.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zmg.nwbrower.top

[Q28] 求和与平均
来源：http://iak.dashuyun.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dmd.nanxuanxn.top

[Q29] 最大最小值
来源：http://npi.tianlin.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://hli.pengpengdd.cyou

[Q30] 分组统计
来源：http://paz.birdmap.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tyt.tarul.cn

[Q31] 分组后过滤
来源：http://ihg.havefunace.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gfr.yueranfly.top

[Q32] 分组拼接字符串
来源：http://gdz.mhx1999.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gop.havefunace.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hfj.shanyushiyangkeji.top

[Q33] 多列分组
来源：http://rvi.c1oappe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pau.xuetiantiany.cn

[Q34] 每组取第一条
来源：http://uru.jlsjyb.cn

SELECT * FROM (
来源：http://imd.tianlin.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lch.vehdjk.com

) t WHERE rn = 1;
来源：http://ilz.ydzc1.top

[Q35] 内连接
来源：http://fpv.guowangkeji.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ryh.xziqi.cn

[Q36] 左连接
来源：http://bkx.uphjek.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rde.sweek.top

[Q37] 右连接
来源：http://bji.guannengcc.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zsm.feifeiyinyue.top

[Q38] 全外连接（PostgreSQL）
来源：http://mxr.tianlin.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://aad.andypj.xyz

[Q39] 自连接（查上下级）
来源：http://cch.shuidangran.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://lnb.redwolf501.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ssb.uphjek.com

[Q40] 交叉连接（笛卡尔积）
来源：http://pyo.ivvv.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tfa.bbcook.cn

[Q41] 多表连接
来源：http://ptr.ppjwa.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qtg.smart0.xyz

JOIN users u ON u.id = o.user_id
来源：http://jev.jinyuanbaomall.cn

JOIN products p ON p.id = o.product_id;
来源：http://gns.shanyushiyangkeji.top

[Q42] 连接条件附加过滤
来源：http://qec.chenzaomai.com

SELECT u.name, o.amount FROM users u
来源：http://imf.zhoulong.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bdv.guowangkeji.top

[Q43] 标量子查询
来源：http://rfi.mhx1999.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rcv.pengpengdd.cyou

[Q44] IN 子查询
来源：http://wxw.jlsjyb.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pqa.quarkkingdee.top

[Q45] EXISTS 判断存在
来源：http://yhh.aizwys.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://egz.yj20258.top

[Q46] NOT EXISTS 判断不存在
来源：http://qyd.ppjwa.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mei.xziqi.cn

[Q47] 与平均值比较
来源：http://rur.meibo888.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lsq.hfpthk.cn

[Q48] CTE 公用表表达式
来源：http://tpo.kuanghao11.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ijt.ivvv.top

SELECT * FROM t WHERE c > 5;
来源：http://kyj.hesvh.cn

[Q49] 更新单行
来源：http://nyk.snrcjt.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jcf.guannengcc.top

[Q50] 批量更新
来源：http://fnw.iojbl.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jep.zhixingplan.top

[Q51] 用子查询更新
来源：http://dvc.xziqi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nfm.gaohongyu789.top

[Q52] 删除指定行
来源：http://fzb.0kj1m.cn

DELETE FROM users WHERE id = 10;
来源：http://gxq.wangdashe.top

[Q53] 按条件删除
来源：http://gmv.316326.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://igi.guowangkeji.top

[Q54] 清空表
来源：http://jox.cdnleiting.top

TRUNCATE TABLE logs;
来源：http://tvh.9152youxi.cn

[Q55] 排名（并列占位）
来源：http://cyv.shuidangran.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ypo.nanxinkj.top

[Q56] 密集排名（并列不占位）
来源：http://knb.yongpay.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tpt.hnxiangtu.top

[Q57] 行号
来源：http://dfc.havefunace.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://drl.ppjwa.cn

[Q58] 累计求和
来源：http://liq.gogol.net.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ifb.zhiwuduotai.top

[Q59] 分组内累计
来源：http://xvw.jinghuilouyu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ehd.meibo888.top

[Q60] 取上一行 / 下一行
来源：http://jgk.sweek.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zeh.aibaodan.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://iza.yj20258.top

[Q61] 移动平均
来源：http://pme.haohaochexian.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jns.wangdashe.top

[Q62] 分组占比
来源：http://vpd.bbcook.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pyd.fanxiaobao.xyz

[Q63] 开启事务
来源：http://cxw.zhoulong.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://maa.fengsongda.top

[Q64] 提交事务
来源：http://iqq.ywan-chungtsiang.top

COMMIT;
来源：http://jwv.yuxming.cn

[Q65] 回滚事务
来源：http://mcx.yangfankeji.com

ROLLBACK;
来源：http://syz.andypj.xyz

[Q66] 行锁查询
来源：http://siy.hywenlv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hen.zdqjudy.top

[Q67] 设置隔离级别
来源：http://kkg.yfazqb.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://odo.sufxvd.cn

[Q68] 保存点
来源：http://ttw.sjlbkw.cn

SAVEPOINT sp1;
来源：http://lkv.quarkkingdee.top

ROLLBACK TO sp1;
来源：http://wev.yueranfly.top

[Q69] 查看执行计划
来源：http://sfk.yongpay.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fig.316326.xyz

[Q70] 更新统计信息
来源：http://efo.yuxming.cn

ANALYZE TABLE users;
来源：http://kqf.haohaochexian.top

[Q71] 查看建表语句
来源：http://owu.zhijiandao.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ayj.hcnkem.com

[Q72] 查看索引
来源：http://eea.nanxinkj.top

SHOW INDEX FROM users;
来源：http://hee.jiagoushi.top

[Q73] 查看表状态
来源：http://chr.aizwys.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://yiw.bjfxy.top

[Q74] 强制使用索引
来源：http://npe.guannengcc.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pir.zhaomingkeji.xyz

[Q75] 日期格式化
来源：http://vwr.aibaodan.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dhu.316326.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jza.fzhhl.top

[Q76] 按天统计
来源：http://ilz.svipenyu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://orc.gzhubu.top

[Q77] 时间加减
来源：http://pem.aizwys.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://thn.tian-w.cn

[Q78] 当前时间
来源：http://wcl.iojbl.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kuy.cheryme.top

[Q79] 字符串拼接
来源：http://rmu.havefunace.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://psb.hnxiangtu.top

[Q80] 字符串截取
来源：http://dxq.sufxvd.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rao.yfazqb.com

[Q81] 字符串替换
来源：http://vtu.quarkkingdee.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zpt.ivvv.top

[Q82] 字符长度与字节长度
来源：http://aek.shangyingyoupin.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://axx.sufxvd.cn

[Q83] 大小写转换
来源：http://kyz.pycfn.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dau.feifeiyinyue.top

[Q84] 去除首尾空格
来源：http://xdj.gotoacloud.top

SELECT TRIM(name) FROM users;
来源：http://jmq.hcnkem.com

[Q85] 数值取整
来源：http://tol.jqgufenzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lkg.xylfe.cn

[Q86] 读取 JSON 字段
来源：http://kvq.zhijiandao.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://whp.tanke756.top

[Q87] JSON 字段做条件
来源：http://laz.xinyue.icu

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lya.shanyushiyangtech.top

[Q88] 行转列（条件聚合）
来源：http://ayo.shzxlz.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zyu.hfpthk.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://llq.ivvv.top

[Q89] 判断表是否存在
来源：http://vkz.nwbrower.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wks.pycfn.com

[Q90] 生成序号列
来源：http://dtm.zhixingplan.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://oae.cdnleiting.top

================================================================================
来源：http://soa.ppjwa.cn

R. Bash 专题
来源：http://bbz.9152youxi.cn

================================================================================
来源：http://nzz.sufxvd.cn

[R01] shebang 与严格模式
来源：http://lkr.hongshengwenyu.top

#!/usr/bin/env bash
来源：http://glr.jinqigufen.top

set -euo pipefail
来源：http://ypt.snrcjt.cn

[R02] 变量赋值与使用
来源：http://tjp.chenjidiqi.icu

name="Tom"; echo "$name"
来源：http://gxs.pengpengdd.cyou

[R03] 只读变量
来源：http://bsg.wangdashe.top

readonly PI=3.14
来源：http://zkk.xuetiantiany.cn

[R04] 位置参数
来源：http://mes.sjlbkw.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xwu.epnwcf.com

[R05] 参数默认值
来源：http://njg.ctjpmb.com

name="${1:-default}"
来源：http://bqw.wangdashe.top

[R06] 判断命令是否存在
来源：http://iux.chenjidiqi.icu

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://orz.sysykeji.top

[R07] if 判断文件
来源：http://yyy.wangdashe.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://txg.dianchejie.cn

[R08] 数值比较
来源：http://fez.shanyushiyangtech.top

if (( a > b )); then echo "a 更大"; fi
来源：http://eus.cheryme.top

[R09] 字符串比较
来源：http://gxa.sweek.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jgu.zhiwuduotai.top

[R10] 正则匹配
来源：http://yzz.sysykeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nfk.shanyushiyangtech.top

[R11] case 多分支
来源：http://wlz.uphjek.com

case "$1" in
来源：http://tzt.shangyingyoupin.top

start) echo "启动" ;;
来源：http://lzc.havefunace.top

stop)  echo "停止" ;;
来源：http://rmm.zhiwuduotai.top

*)     echo "未知命令" ;;
来源：http://uqo.shanyushiyangkeji.top

esac
来源：http://njo.cheryme.top

[R12] for 遍历文件
来源：http://xcv.zhoulong.xyz

for f in *.txt; do echo "$f"; done
来源：http://ola.fzhhl.top

[R13] for 计数循环
来源：http://ewl.fehbvm.com

for i in {1..10}; do echo "$i"; done
来源：http://gqf.zycfv.cn

[R14] C 风格 for
来源：http://xva.tanke756.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jpk.jinghuilouyu.cn

[R15] while 逐行读文件
来源：http://zqa.fktsv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tvq.jianghu66.top

[R16] until 等待条件
来源：http://svf.sweek.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ggb.yj20258.top

[R17] 数组定义与取值
来源：http://ago.fanxiaobao.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://gxc.yj202588.top

[R18] 遍历数组
来源：http://dwb.jianghu66.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ykt.yonumen.top

[R19] 数组长度
来源：http://mtt.ivvv.top

echo "${#arr[@]}"
来源：http://fun.shanyushiyangkeji.top

[R20] 关联数组（字典）
来源：http://njy.shanyushiyangtech.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zmi.iojbl.cn

[R21] 字符串长度
来源：http://dsv.ctjpmb.com

echo "${#s}"
来源：http://jqj.sysykeji.top

[R22] 截取子串
来源：http://ztx.yj20258888.top

echo "${s:0:5}"
来源：http://xeh.chenlongwang.top

[R23] 字符串替换
来源：http://kkc.haohaochexian.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ndi.tanke756.top

[R24] 大小写转换
来源：http://ndo.zhiwuduotai.top

echo "${s^^}"; echo "${s,,}"
来源：http://qes.shuidangran.top

[R25] 去后缀 / 去前缀
来源：http://gab.zhoulong.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://gel.zhiwuduotai.top

[R26] 命令替换
来源：http://ajr.gotoacloud.top

now=$(date +%F); echo "$now"
来源：http://coi.jianghu66.top

[R27] 算术展开
来源：http://mlk.chenzaomai.com

echo $((1 + 2 * 3))
来源：http://pjt.hnxiangtu.top

[R28] 浮点运算
来源：http://dxu.hnqzz.top

echo "scale=2; 10/3" | bc
来源：http://kgs.xinyue.icu

[R29] 定义函数
来源：http://vya.daria6918.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yhc.jqgufenzy.top

[R30] 函数返回状态码
来源：http://bsz.ehwqpu.com

f() { return 0; }; f || echo "失败了"
来源：http://djz.haohaochexian.top

[R31] 局部变量
来源：http://wmj.zhengqikj.top

f() { local x=1; echo "$x"; }
来源：http://xwv.jyoumei.cn

[R32] 参数个数校验
来源：http://abz.ydzc1.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vet.hammf.cn

[R33] 捕获错误并提示行号
来源：http://ivx.jinyuanbaomall.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ync.feifeiyinyue.top

[R34] 退出时清理
来源：http://ejf.aizwys.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pab.shanyushiyangtech.top

[R35] 后台执行并等待
来源：http://zht.xingfuxueyuan.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://ive.snrcjt.cn

[R36] 并发执行多个任务
来源：http://wpj.jinghuilouyu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zje.snrcjt.cn

[R37] 把输出赋给变量
来源：http://dkj.hysaishi.cn

files=$(ls -1)
来源：http://jor.pycfn.com

[R38] 管道串联
来源：http://cap.shanyushiyangkeji.top

cat a.txt | grep -i error | wc -l
来源：http://iyd.52xcode.cn

[R39] 重定向标准输出与错误
来源：http://qkm.mhx1999.top


<!-- 参考信息 -->