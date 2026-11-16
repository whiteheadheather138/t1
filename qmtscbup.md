代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://srt.quarkkingdee.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dgc.tanke756.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://omq.yueranfly.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://evt.ivvv.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oyh.yonumen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ray.daxiang520.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hdp.haohaochexian.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mfl.yueranfly.top

================================================================================
来源：http://nrs.meibo888.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yei.0kj1m.cn

================================================================================
来源：http://ovj.tian-w.cn

[Q01] 创建表
来源：http://cvn.nanxinkj.top

CREATE TABLE users (
来源：http://vjg.tanke756.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://abo.yj202588.top

name VARCHAR(50) NOT NULL,
来源：http://ugk.fanxiaobao.xyz

email VARCHAR(100) UNIQUE,
来源：http://saq.hnxiangtu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://psg.jinghuilouyu.cn

);
来源：http://moz.jinqigfzy.top

[Q02] 创建带外键的表
来源：http://hfm.52xcode.cn

CREATE TABLE orders (
来源：http://laf.ybcxt.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cwd.gogol.net.cn

user_id INT NOT NULL,
来源：http://our.pycfn.com

amount DECIMAL(10, 2),
来源：http://yjq.feifeiyinyue.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xnv.zdqjudy.top

);
来源：http://waf.yanxiufei.cn

[Q03] 增加列
来源：http://hno.zhengqikj.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hxj.nanxuanxn.top

[Q04] 修改列类型
来源：http://rwo.yj202588.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tdh.gotoacloud.top

[Q05] 重命名列
来源：http://amc.9152youxi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yks.ydzc1.top

[Q06] 删除列
来源：http://jin.iojbl.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jio.hammf.cn

[Q07] 删除表
来源：http://xjs.aibaodan.cn

DROP TABLE IF EXISTS orders;
来源：http://dtj.mhx1999.top

[Q08] 创建普通索引
来源：http://rpt.jinqigfzy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jdm.chenlongwang.top

[Q09] 创建唯一索引
来源：http://eco.0kj1m.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mrs.smart0.xyz

[Q10] 插入单行
来源：http://inf.jqgufenzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ljc.daxiang520.top

[Q11] 一次插入多行
来源：http://stk.yongpay.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wbc.jqgfzy.top

[Q12] 插入后取自增 ID
来源：http://fxi.zhixingplan.top

INSERT INTO users (name) VALUES ('C');
来源：http://xtv.hnxiangtu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ldm.nanxuanxn.top

[Q13] 忽略重复插入
来源：http://wrl.jianghu66.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pta.ctjpmb.com

[Q14] 存在则更新（upsert）
来源：http://jke.ywan-chungtsiang.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://idy.dianchejie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mcq.xuetiantiany.cn

[Q15] 查询全部
来源：http://odk.sweek.top

SELECT * FROM users;
来源：http://orj.cqqwz.cn

[Q16] 查询指定列
来源：http://kwp.havefunace.top

SELECT id, name FROM users;
来源：http://yxx.ydjk.org.cn

[Q17] 条件查询
来源：http://svu.xziqi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wtj.yuxming.cn

[Q18] 模糊匹配
来源：http://hkl.nwbrower.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kdc.9152youxi.cn

[Q19] 范围查询
来源：http://zoh.vqdsnc.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qwm.zhiwuduotai.top

[Q20] IN 列表
来源：http://flk.hysaishi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://woa.yj202588.top

[Q21] 空值判断
来源：http://edg.chenjidiqi.icu

SELECT * FROM users WHERE email IS NULL;
来源：http://wvi.nwbrower.top

[Q22] 排序
来源：http://gry.hnqzz.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xkp.gaohongyu789.top

[Q23] 分页
来源：http://kuw.tanke756.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xzw.zdbjq.cn

[Q24] 去重
来源：http://pad.fanxiaobao.xyz

SELECT DISTINCT city FROM users;
来源：http://maz.shangyingyoupin.top

[Q25] 只取前 N 条
来源：http://koo.dianchejie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tmu.cdnleiting.top

[Q26] 计数
来源：http://fzv.jiagoushi.top

SELECT COUNT(*) FROM users;
来源：http://ulh.xziqi.cn

[Q27] 条件计数
来源：http://hhj.redwolf501.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sqz.jlsjyb.cn

[Q28] 求和与平均
来源：http://yvl.gzhubu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ohe.daxiang520.top

[Q29] 最大最小值
来源：http://whh.jqgufenzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ama.tianlin.xyz

[Q30] 分组统计
来源：http://vvm.fehbvm.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uql.zycfv.cn

[Q31] 分组后过滤
来源：http://dwc.havefunace.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://npp.jyoumei.cn

[Q32] 分组拼接字符串
来源：http://pmm.sysykeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wcq.hfpthk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xgf.fzhhl.top

[Q33] 多列分组
来源：http://mwv.yuxming.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nbl.fengsongda.top

[Q34] 每组取第一条
来源：http://mmy.jyoumei.cn

SELECT * FROM (
来源：http://nmk.hnqzz.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vky.yueranfly.top

) t WHERE rn = 1;
来源：http://vxd.feifeiyinyue.top

[Q35] 内连接
来源：http://ufq.gaohongyu789.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hso.yj20258888.top

[Q36] 左连接
来源：http://ejl.ydzc1.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ufe.xingfuxueyuan.xyz

[Q37] 右连接
来源：http://tdk.c1oappe.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xzj.zhiwuduotai.top

[Q38] 全外连接（PostgreSQL）
来源：http://grc.zycfv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wle.fengsongda.top

[Q39] 自连接（查上下级）
来源：http://jjg.yueranfly.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://hda.quarkkingdee.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lko.ydjk.org.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cse.hywenlv.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://llp.tian-w.cn

[Q41] 多表连接
来源：http://wlw.gaohongyu789.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://tds.feifeiyinyue.top

JOIN users u ON u.id = o.user_id
来源：http://azw.cucudq.cn

JOIN products p ON p.id = o.product_id;
来源：http://kyu.birdmap.top

[Q42] 连接条件附加过滤
来源：http://eqc.ydjk.org.cn

SELECT u.name, o.amount FROM users u
来源：http://nrn.jinghuilouyu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lme.xuetiantiany.cn

[Q43] 标量子查询
来源：http://fow.quarkkingdee.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://emn.hesvh.cn

[Q44] IN 子查询
来源：http://glv.yangfankeji.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zxs.xylfe.cn

[Q45] EXISTS 判断存在
来源：http://bad.fktsv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://udi.dianchejie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kse.gogol.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dse.wangshuangyany.cn

[Q47] 与平均值比较
来源：http://qxx.xylfe.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://aop.hfpthk.cn

[Q48] CTE 公用表表达式
来源：http://qjg.cucudq.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nwp.jqgufenzy.top

SELECT * FROM t WHERE c > 5;
来源：http://ttc.hysaishi.cn

[Q49] 更新单行
来源：http://ljp.shzxlz.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vzb.sjlbkw.cn

[Q50] 批量更新
来源：http://rtl.aizwys.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://naz.hongshengwenyu.top

[Q51] 用子查询更新
来源：http://jna.aizwys.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mim.epnwcf.com

[Q52] 删除指定行
来源：http://voc.cqqwz.cn

DELETE FROM users WHERE id = 10;
来源：http://ixb.wangshuangyany.cn

[Q53] 按条件删除
来源：http://lgt.jinyuanbaomall.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qaq.andypj.xyz

[Q54] 清空表
来源：http://xvh.0kj1m.cn

TRUNCATE TABLE logs;
来源：http://fko.shzxlz.cn

[Q55] 排名（并列占位）
来源：http://kfy.yuxming.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ush.wangshuangyany.cn

[Q56] 密集排名（并列不占位）
来源：http://ygf.cdnleiting.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yrg.wangshuangyany.cn

[Q57] 行号
来源：http://csf.haohaochexian.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://iyh.kuanghao11.cn

[Q58] 累计求和
来源：http://pwq.9152youxi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://oky.snrcjt.cn

[Q59] 分组内累计
来源：http://mly.yueranfly.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pqv.aizwys.cn

[Q60] 取上一行 / 下一行
来源：http://ssx.jianghu66.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bnp.havefunace.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hkw.xingfuxueyuan.xyz

[Q61] 移动平均
来源：http://lua.smart0.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tas.tanke756.top

[Q62] 分组占比
来源：http://uyn.sysykeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wuz.tanke756.top

[Q63] 开启事务
来源：http://txo.fengsongda.top

START TRANSACTION;                -- 或 BEGIN
来源：http://nvf.ybcxt.top

[Q64] 提交事务
来源：http://woy.jqgfzy.top

COMMIT;
来源：http://mpi.zdqjudy.top

[Q65] 回滚事务
来源：http://vex.haohaochexian.top

ROLLBACK;
来源：http://dsk.tianlin.xyz

[Q66] 行锁查询
来源：http://mjb.nanxinkj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://koi.ivvv.top

[Q67] 设置隔离级别
来源：http://kha.52xcode.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ifd.nanxinkj.top

[Q68] 保存点
来源：http://ptm.jqgfzy.top

SAVEPOINT sp1;
来源：http://dua.bbcook.cn

ROLLBACK TO sp1;
来源：http://iwm.hywenlv.cn

[Q69] 查看执行计划
来源：http://frg.kuanghao11.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jrl.cucudq.cn

[Q70] 更新统计信息
来源：http://sex.uphjek.com

ANALYZE TABLE users;
来源：http://drs.aizwys.cn

[Q71] 查看建表语句
来源：http://pah.wangdashe.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ilc.cdnleiting.top

[Q72] 查看索引
来源：http://nts.jinghuilouyu.cn

SHOW INDEX FROM users;
来源：http://yzj.hysaishi.cn

[Q73] 查看表状态
来源：http://euk.jiagoushi.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ybz.jinghuilouyu.cn

[Q74] 强制使用索引
来源：http://kou.zhijiandao.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jbn.chenzaomai.com

[Q75] 日期格式化
来源：http://kpg.aibaodan.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dus.gzhubu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tad.shuidangran.top

[Q76] 按天统计
来源：http://mup.chenlongwang.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://iwx.zhiwuduotai.top

[Q77] 时间加减
来源：http://gym.sweek.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zwz.guannengcc.top

[Q78] 当前时间
来源：http://sya.zhijiandao.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://znp.ivvv.top

[Q79] 字符串拼接
来源：http://uoz.yueranfly.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://diq.gzhubu.top

[Q80] 字符串截取
来源：http://pgl.redwolf501.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mpf.hnqzz.top

[Q81] 字符串替换
来源：http://hjl.meibo888.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yfx.meibo888.top

[Q82] 字符长度与字节长度
来源：http://oel.shanyushiyangkeji.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zdm.snrcjt.cn

[Q83] 大小写转换
来源：http://yrp.hesvh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rhk.cashguo.top

[Q84] 去除首尾空格
来源：http://ncb.yueranfly.top

SELECT TRIM(name) FROM users;
来源：http://uil.havefunace.top

[Q85] 数值取整
来源：http://gqx.ppjwa.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kfq.ybcxt.top

[Q86] 读取 JSON 字段
来源：http://ufk.shangyingyoupin.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ywq.hfpthk.cn

[Q87] JSON 字段做条件
来源：http://jcl.yfazqb.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hdg.smart0.xyz

[Q88] 行转列（条件聚合）
来源：http://sap.52xcode.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ydx.ppjwa.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://phv.yanxiufei.cn

[Q89] 判断表是否存在
来源：http://xjx.feifeiyinyue.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ajd.daria6918.cn

[Q90] 生成序号列
来源：http://lbc.sufxvd.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://klp.hesvh.cn

================================================================================
来源：http://pwy.cdnleiting.top

R. Bash 专题
来源：http://ohz.iojbl.cn

================================================================================
来源：http://gem.iojbl.cn

[R01] shebang 与严格模式
来源：http://uov.hysaishi.cn

#!/usr/bin/env bash
来源：http://btl.yongpay.top

set -euo pipefail
来源：http://onp.jiagoushi.top

[R02] 变量赋值与使用
来源：http://jeo.fzhhl.top

name="Tom"; echo "$name"
来源：http://esw.yongpay.top

[R03] 只读变量
来源：http://lxq.ydzc1.top

readonly PI=3.14
来源：http://hxf.zdbjq.cn

[R04] 位置参数
来源：http://dkl.gzhubu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sks.chenjidiqi.icu

[R05] 参数默认值
来源：http://kpo.zycfv.cn

name="${1:-default}"
来源：http://waf.ctjpmb.com

[R06] 判断命令是否存在
来源：http://aur.yj20258.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yzi.havefunace.top

[R07] if 判断文件
来源：http://azq.meibo888.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cdo.hesvh.cn

[R08] 数值比较
来源：http://suk.chenlongwang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://pkt.hfpthk.cn

[R09] 字符串比较
来源：http://iwu.316326.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://weh.hywenlv.cn

[R10] 正则匹配
来源：http://vam.ydzc1.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://meu.hywenlv.cn

[R11] case 多分支
来源：http://xxt.xingfuxueyuan.xyz

case "$1" in
来源：http://jsi.jlsjyb.cn

start) echo "启动" ;;
来源：http://cpg.aibaodan.cn

stop)  echo "停止" ;;
来源：http://qjm.xuanzx.com

*)     echo "未知命令" ;;
来源：http://ttl.hnxiangtu.top

esac
来源：http://qlo.gaohongyu789.top

[R12] for 遍历文件
来源：http://mkz.haohaochexian.top

for f in *.txt; do echo "$f"; done
来源：http://bcc.yuanzhike.top

[R13] for 计数循环
来源：http://bxs.xingfuxueyuan.xyz

for i in {1..10}; do echo "$i"; done
来源：http://dqq.zhengqikj.top

[R14] C 风格 for
来源：http://jyf.bbcook.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ken.zhaomingkeji.xyz

[R15] while 逐行读文件
来源：http://siw.sysykeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wrp.wangdashe.top

[R16] until 等待条件
来源：http://sqj.svipenyu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://soj.tarul.cn

[R17] 数组定义与取值
来源：http://hap.jqgufenzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://jit.meibo888.top

[R18] 遍历数组
来源：http://xpz.tarul.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mzo.jqgfzy.top

[R19] 数组长度
来源：http://cpm.shanyushiyangkeji.top

echo "${#arr[@]}"
来源：http://qzf.hammf.cn

[R20] 关联数组（字典）
来源：http://jtn.birdmap.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nie.gogol.net.cn

[R21] 字符串长度
来源：http://ifl.yj202588.top

echo "${#s}"
来源：http://vje.jyoumei.cn

[R22] 截取子串
来源：http://que.yvedp.cn

echo "${s:0:5}"
来源：http://dzn.yuanzhike.top

[R23] 字符串替换
来源：http://lyx.andypj.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ddh.ybcxt.top

[R24] 大小写转换
来源：http://hzu.jinghuilouyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kyt.zycfv.cn

[R25] 去后缀 / 去前缀
来源：http://cts.svipenyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sgc.nanxinkj.top

[R26] 命令替换
来源：http://rnv.jqgfzy.top

now=$(date +%F); echo "$now"
来源：http://lms.meibo888.top

[R27] 算术展开
来源：http://pbt.ehwqpu.com

echo $((1 + 2 * 3))
来源：http://mcv.52xcode.cn

[R28] 浮点运算
来源：http://xdk.ybcxt.top

echo "scale=2; 10/3" | bc
来源：http://trh.yongpay.top

[R29] 定义函数
来源：http://ipb.9152youxi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://anc.cqqwz.cn

[R30] 函数返回状态码
来源：http://jzr.dashuyun.cn

f() { return 0; }; f || echo "失败了"
来源：http://grp.hammf.cn

[R31] 局部变量
来源：http://mfv.xuanzx.com

f() { local x=1; echo "$x"; }
来源：http://psw.vehdjk.com

[R32] 参数个数校验
来源：http://wnu.dashuyun.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vke.daria6918.cn

[R33] 捕获错误并提示行号
来源：http://fta.fktsv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tcf.c1oappe.top

[R34] 退出时清理
来源：http://jwg.jinghuilouyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vhm.nanxuanxn.top

[R35] 后台执行并等待
来源：http://gje.yonumen.top

sleep 5 & pid=$!; wait "$pid"
来源：http://you.ywan-chungtsiang.top

[R36] 并发执行多个任务
来源：http://tdg.xziqi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mej.hesvh.cn

[R37] 把输出赋给变量
来源：http://jyo.meibo888.top

files=$(ls -1)
来源：http://kan.nanxuanxn.top

[R38] 管道串联
来源：http://wxy.tanke756.top

cat a.txt | grep -i error | wc -l
来源：http://hkb.yj20258888.top

[R39] 重定向标准输出与错误
来源：http://ahy.tanke756.top


<!-- 参考信息 -->