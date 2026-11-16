代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uwp.xinyue.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://itu.jlsjyb.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://egj.havefunace.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mwp.snrcjt.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://roo.hnxiangtu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vqf.cdnleiting.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ogk.iojbl.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wrb.daria6918.cn

================================================================================
来源：http://gyn.shuidangran.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jsv.cashguo.top

================================================================================
来源：http://jim.gogol.net.cn

[Q01] 创建表
来源：http://tbw.jinyuanbaomall.cn

CREATE TABLE users (
来源：http://czk.xuanzx.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://czp.ppjwa.cn

name VARCHAR(50) NOT NULL,
来源：http://jht.kuanghao11.cn

email VARCHAR(100) UNIQUE,
来源：http://byg.yfazqb.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sld.haohaochexian.top

);
来源：http://mgy.yanxiufei.cn

[Q02] 创建带外键的表
来源：http://jle.shuidangran.top

CREATE TABLE orders (
来源：http://iwi.jinyuanbaomall.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ijo.andypj.xyz

user_id INT NOT NULL,
来源：http://gnx.jqgufenzy.top

amount DECIMAL(10, 2),
来源：http://qwo.ybcxt.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://idt.fengsongda.top

);
来源：http://als.snrcjt.cn

[Q03] 增加列
来源：http://eqx.zhaomingkeji.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fby.cashguo.top

[Q04] 修改列类型
来源：http://qqh.316326.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://idg.aibaodan.cn

[Q05] 重命名列
来源：http://bau.xingfuxueyuan.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ony.cheryme.top

[Q06] 删除列
来源：http://ptm.chenlongwang.top

ALTER TABLE users DROP COLUMN age;
来源：http://pvp.hesvh.cn

[Q07] 删除表
来源：http://qca.sweek.top

DROP TABLE IF EXISTS orders;
来源：http://jhj.aibaodan.cn

[Q08] 创建普通索引
来源：http://fhv.hnxiangtu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://lez.hongshengwenyu.top

[Q09] 创建唯一索引
来源：http://khy.jinqigufen.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wld.haohaochexian.top

[Q10] 插入单行
来源：http://kfm.0kj1m.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hfa.feifeiyinyue.top

[Q11] 一次插入多行
来源：http://ige.hcnkem.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iql.shzxlz.cn

[Q12] 插入后取自增 ID
来源：http://mxa.tianlin.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://jxt.yuanzhike.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://swi.9152youxi.cn

[Q13] 忽略重复插入
来源：http://vae.ydzc1.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://adi.sufxvd.cn

[Q14] 存在则更新（upsert）
来源：http://llu.yj20258.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dlb.ybcxt.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nch.9152youxi.cn

[Q15] 查询全部
来源：http://mal.sysykeji.top

SELECT * FROM users;
来源：http://tqt.yj20258.top

[Q16] 查询指定列
来源：http://moo.iojbl.cn

SELECT id, name FROM users;
来源：http://nsk.chenzaomai.com

[Q17] 条件查询
来源：http://ozv.jinyuanbaomall.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://neq.zhixingplan.top

[Q18] 模糊匹配
来源：http://eff.tian-w.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zxh.yuxming.cn

[Q19] 范围查询
来源：http://orb.jqgfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dgr.ybcxt.top

[Q20] IN 列表
来源：http://nxw.ctjpmb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uxb.yj20258.top

[Q21] 空值判断
来源：http://auy.tianlin.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://mkm.sysykeji.top

[Q22] 排序
来源：http://kna.shangyingyoupin.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://avf.ydzc1.top

[Q23] 分页
来源：http://eia.zycfv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jzx.ppjwa.cn

[Q24] 去重
来源：http://skr.fktsv.cn

SELECT DISTINCT city FROM users;
来源：http://ogt.wangshuangyany.cn

[Q25] 只取前 N 条
来源：http://wzp.snrcjt.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tcq.hysaishi.cn

[Q26] 计数
来源：http://cop.sufxvd.cn

SELECT COUNT(*) FROM users;
来源：http://ewb.52xcode.cn

[Q27] 条件计数
来源：http://pjl.xuanzx.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://alk.xuetiantiany.cn

[Q28] 求和与平均
来源：http://suo.c1oappe.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tcz.jianghu66.top

[Q29] 最大最小值
来源：http://inm.aizwys.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gnm.havefunace.top

[Q30] 分组统计
来源：http://xvv.yongpay.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://klp.zhixingplan.top

[Q31] 分组后过滤
来源：http://jqr.dianchejie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://swf.yuanzhike.top

[Q32] 分组拼接字符串
来源：http://ccf.bbcook.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://olt.havefunace.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wbc.pengpengdd.cyou

[Q33] 多列分组
来源：http://zch.yuxming.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jye.hongshengwenyu.top

[Q34] 每组取第一条
来源：http://srb.andypj.xyz

SELECT * FROM (
来源：http://oya.c1oappe.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gml.yuxming.cn

) t WHERE rn = 1;
来源：http://ugl.xinyue.icu

[Q35] 内连接
来源：http://qim.dianchejie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nod.chenzaomai.com

[Q36] 左连接
来源：http://kig.xziqi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://udc.ywan-chungtsiang.top

[Q37] 右连接
来源：http://ffx.jyoumei.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qem.feifeiyinyue.top

[Q38] 全外连接（PostgreSQL）
来源：http://tsg.shanyushiyangkeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gih.zhoulong.xyz

[Q39] 自连接（查上下级）
来源：http://xbp.chenjidiqi.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://iar.cucudq.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lok.guowangkeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zrs.xuetiantiany.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uzp.cashguo.top

[Q41] 多表连接
来源：http://lyr.shangyingyoupin.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://djg.jyoumei.cn

JOIN users u ON u.id = o.user_id
来源：http://ler.xuetiantiany.cn

JOIN products p ON p.id = o.product_id;
来源：http://fds.quarkkingdee.top

[Q42] 连接条件附加过滤
来源：http://lph.sufxvd.cn

SELECT u.name, o.amount FROM users u
来源：http://ytv.hysaishi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sio.wangdashe.top

[Q43] 标量子查询
来源：http://ugw.316326.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yzc.chenlongwang.top

[Q44] IN 子查询
来源：http://uqs.cqqwz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cjw.yueranfly.top

[Q45] EXISTS 判断存在
来源：http://ibj.jiagoushi.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wok.chenlongwang.top

[Q46] NOT EXISTS 判断不存在
来源：http://xhf.gaohongyu789.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://flg.jinghuilouyu.cn

[Q47] 与平均值比较
来源：http://ltf.cashguo.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rsl.iojbl.cn

[Q48] CTE 公用表表达式
来源：http://urf.shanyushiyangkeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lol.aizwys.cn

SELECT * FROM t WHERE c > 5;
来源：http://lzj.yfazqb.com

[Q49] 更新单行
来源：http://yev.xuanzx.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xeu.wangshuangyany.cn

[Q50] 批量更新
来源：http://xkq.jlsjyb.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wlo.quarkkingdee.top

[Q51] 用子查询更新
来源：http://ysh.guowangkeji.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qoo.fanxiaobao.xyz

[Q52] 删除指定行
来源：http://ofx.chenzaomai.com

DELETE FROM users WHERE id = 10;
来源：http://qte.tianlin.xyz

[Q53] 按条件删除
来源：http://rlz.aibaodan.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nfe.jlsjyb.cn

[Q54] 清空表
来源：http://oqe.kuanghao11.cn

TRUNCATE TABLE logs;
来源：http://jiw.jinyuanbaomall.cn

[Q55] 排名（并列占位）
来源：http://hxw.aizwys.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bpo.daxiang520.top

[Q56] 密集排名（并列不占位）
来源：http://huz.ydjk.org.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://etc.ybcxt.top

[Q57] 行号
来源：http://mbi.jyoumei.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ref.guowangkeji.top

[Q58] 累计求和
来源：http://egm.hywenlv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lrd.yanxiufei.cn

[Q59] 分组内累计
来源：http://zie.hfpthk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yjh.nanxinkj.top

[Q60] 取上一行 / 下一行
来源：http://neh.snrcjt.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://omo.meibo888.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://oql.hcnkem.com

[Q61] 移动平均
来源：http://zpr.fengsongda.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tqm.zycfv.cn

[Q62] 分组占比
来源：http://gxg.chenlongwang.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://flr.zhongyouzk.top

[Q63] 开启事务
来源：http://dtx.zhongyouzk.top

START TRANSACTION;                -- 或 BEGIN
来源：http://diu.guannengcc.top

[Q64] 提交事务
来源：http://hua.zhaomingkeji.xyz

COMMIT;
来源：http://gsj.zdbjq.cn

[Q65] 回滚事务
来源：http://fuh.kuanghao11.cn

ROLLBACK;
来源：http://hdr.0kj1m.cn

[Q66] 行锁查询
来源：http://afm.birdmap.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wem.jlsjyb.cn

[Q67] 设置隔离级别
来源：http://zvn.jyoumei.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zxz.zhoulong.xyz

[Q68] 保存点
来源：http://fca.jinghuilouyu.cn

SAVEPOINT sp1;
来源：http://nim.birdmap.top

ROLLBACK TO sp1;
来源：http://hmo.tanke756.top

[Q69] 查看执行计划
来源：http://jdf.cheryme.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xms.daxiang520.top

[Q70] 更新统计信息
来源：http://omh.dianchejie.cn

ANALYZE TABLE users;
来源：http://mac.nanxuanxn.top

[Q71] 查看建表语句
来源：http://zzy.vqdsnc.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zxr.dianchejie.cn

[Q72] 查看索引
来源：http://vcb.hysaishi.cn

SHOW INDEX FROM users;
来源：http://oer.quarkkingdee.top

[Q73] 查看表状态
来源：http://ado.cqqwz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ixf.hysaishi.cn

[Q74] 强制使用索引
来源：http://tqp.sysykeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gnq.tarul.cn

[Q75] 日期格式化
来源：http://dcz.fktsv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://owu.haohaochexian.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xqv.snrcjt.cn

[Q76] 按天统计
来源：http://zjo.kuanghao11.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uve.aizwys.cn

[Q77] 时间加减
来源：http://ixa.yfazqb.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://flq.zycfv.cn

[Q78] 当前时间
来源：http://lrs.shanyushiyangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://aqy.jqgfzy.top

[Q79] 字符串拼接
来源：http://ehk.ppjwa.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ywh.fengsongda.top

[Q80] 字符串截取
来源：http://mxd.cqqwz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gql.hcnkem.com

[Q81] 字符串替换
来源：http://zgr.jinqigufen.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dys.gzhubu.top

[Q82] 字符长度与字节长度
来源：http://hpv.yj202588.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ipp.svipenyu.cn

[Q83] 大小写转换
来源：http://ylm.fengsongda.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dwz.shanyushiyangkeji.top

[Q84] 去除首尾空格
来源：http://wrq.tarul.cn

SELECT TRIM(name) FROM users;
来源：http://max.yangfankeji.com

[Q85] 数值取整
来源：http://xcu.gaohongyu789.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nhi.pycfn.com

[Q86] 读取 JSON 字段
来源：http://csm.pengpengdd.cyou

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://btf.yfazqb.com

[Q87] JSON 字段做条件
来源：http://wzr.meibo888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oau.xylfe.cn

[Q88] 行转列（条件聚合）
来源：http://fwi.ydjk.org.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yzw.tianlin.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oip.cucudq.cn

[Q89] 判断表是否存在
来源：http://tdd.jyoumei.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://woo.9152youxi.cn

[Q90] 生成序号列
来源：http://xin.hysaishi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nve.vqdsnc.cn

================================================================================
来源：http://nrm.jqgfzy.top

R. Bash 专题
来源：http://ioh.yj20258888.top

================================================================================
来源：http://tts.xylfe.cn

[R01] shebang 与严格模式
来源：http://vvi.vehdjk.com

#!/usr/bin/env bash
来源：http://rwv.snrcjt.cn

set -euo pipefail
来源：http://xbd.gogol.net.cn

[R02] 变量赋值与使用
来源：http://rpg.iojbl.cn

name="Tom"; echo "$name"
来源：http://mhy.xuetiantiany.cn

[R03] 只读变量
来源：http://aif.jinqigufen.top

readonly PI=3.14
来源：http://wjh.jinghuilouyu.cn

[R04] 位置参数
来源：http://zjm.jiagoushi.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hkr.zhoulong.xyz

[R05] 参数默认值
来源：http://tjk.zycfv.cn

name="${1:-default}"
来源：http://qdo.ybcxt.top

[R06] 判断命令是否存在
来源：http://iwy.xinyue.icu

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qxv.fktsv.cn

[R07] if 判断文件
来源：http://gvu.jinyuanbaomall.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yhu.52xcode.cn

[R08] 数值比较
来源：http://ypk.yonumen.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ewq.316326.xyz

[R09] 字符串比较
来源：http://jjv.birdmap.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ejm.cashguo.top

[R10] 正则匹配
来源：http://kro.tianlin.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sqp.cashguo.top

[R11] case 多分支
来源：http://nel.cucudq.cn

case "$1" in
来源：http://cus.yonumen.top

start) echo "启动" ;;
来源：http://aut.meibo888.top

stop)  echo "停止" ;;
来源：http://wxt.dashuyun.cn

*)     echo "未知命令" ;;
来源：http://dya.jqgufenzy.top

esac
来源：http://ytd.yanxiufei.cn

[R12] for 遍历文件
来源：http://lgv.nanxuanxn.top

for f in *.txt; do echo "$f"; done
来源：http://ybz.shzxlz.cn

[R13] for 计数循环
来源：http://jlu.yanxiufei.cn

for i in {1..10}; do echo "$i"; done
来源：http://iwq.zhaomingkeji.xyz

[R14] C 风格 for
来源：http://drq.epnwcf.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jqp.shzxlz.cn

[R15] while 逐行读文件
来源：http://bbu.ehwqpu.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tqg.zhongyouzk.top

[R16] until 等待条件
来源：http://pfh.wangshuangyany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nsu.daria6918.cn

[R17] 数组定义与取值
来源：http://bhn.snrcjt.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pqm.jinqigfzy.top

[R18] 遍历数组
来源：http://vco.shangyingyoupin.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rxl.cdnleiting.top

[R19] 数组长度
来源：http://aic.tanke756.top

echo "${#arr[@]}"
来源：http://yfo.xylfe.cn

[R20] 关联数组（字典）
来源：http://ezb.andypj.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dqp.chenjidiqi.icu

[R21] 字符串长度
来源：http://pvu.fehbvm.com

echo "${#s}"
来源：http://syl.wangshuangyany.cn

[R22] 截取子串
来源：http://kxf.zhiwuduotai.top

echo "${s:0:5}"
来源：http://ikq.hammf.cn

[R23] 字符串替换
来源：http://xgj.hnxiangtu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://azc.yueranfly.top

[R24] 大小写转换
来源：http://ycp.hywenlv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fwq.ywan-chungtsiang.top

[R25] 去后缀 / 去前缀
来源：http://vnk.fktsv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dtu.gogol.net.cn

[R26] 命令替换
来源：http://uxv.ybcxt.top

now=$(date +%F); echo "$now"
来源：http://ujd.xziqi.cn

[R27] 算术展开
来源：http://xlj.xuetiantiany.cn

echo $((1 + 2 * 3))
来源：http://dqx.yangfankeji.com

[R28] 浮点运算
来源：http://wzx.hongshengwenyu.top

echo "scale=2; 10/3" | bc
来源：http://qnk.guowangkeji.top

[R29] 定义函数
来源：http://vda.chenlongwang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yel.meibo888.top

[R30] 函数返回状态码
来源：http://ovq.aibaodan.cn

f() { return 0; }; f || echo "失败了"
来源：http://wnh.sxryk.cn

[R31] 局部变量
来源：http://smf.cdnleiting.top

f() { local x=1; echo "$x"; }
来源：http://jyc.xziqi.cn

[R32] 参数个数校验
来源：http://zkx.yonumen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dbu.tianlin.xyz

[R33] 捕获错误并提示行号
来源：http://kmu.ydjk.org.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xtx.yj202588.top

[R34] 退出时清理
来源：http://mbc.vqdsnc.cn

trap 'rm -f "$tmp"' EXIT
来源：http://igs.zhaomingkeji.xyz

[R35] 后台执行并等待
来源：http://gib.shangyingyoupin.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dbd.wangdashe.top

[R36] 并发执行多个任务
来源：http://uxs.fehbvm.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://npk.xinyue.icu

[R37] 把输出赋给变量
来源：http://jjq.gotoacloud.top

files=$(ls -1)
来源：http://hdr.yanxiufei.cn

[R38] 管道串联
来源：http://vpf.pycfn.com

cat a.txt | grep -i error | wc -l
来源：http://ogz.cheryme.top

[R39] 重定向标准输出与错误
来源：http://eam.gaohongyu789.top


<!-- 参考信息 -->