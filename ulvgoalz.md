代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lgm.vehdjk.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kjw.yvedp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://eeq.pengpengdd.cyou

PHP:  if (empty($x)) {}
来源：http://vsd.guowangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ujr.sjlbkw.cn

TS:   if (x == null) {}
来源：http://txj.wangdashe.top

Java: if (x == null || x.isEmpty()) {}
来源：http://grf.yj20258.top

Go:   if x == nil {}
来源：http://ztt.ybcxt.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ljs.xziqi.cn

C#:   if (x is null) {}
来源：http://grw.mhx1999.top

[P07] 防抖与节流
来源：http://xje.cucudq.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pgv.hammf.cn

PHP:  // 手写时间戳比较
来源：http://jcn.tarul.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fli.zhiwuduotai.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eqg.cheryme.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fvj.0kj1m.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qdo.jyoumei.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rkk.shanyushiyangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rvk.snrcjt.cn

[P08] 处理浮点精度问题
来源：http://eop.redwolf501.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gtf.fanxiaobao.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nhb.yvedp.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://djx.nanxinkj.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ioj.sjlbkw.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rvf.hnxiangtu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://myo.zdqjudy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lxg.sufxvd.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://noz.havefunace.top

================================================================================
来源：http://izx.uphjek.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xgd.shangyingyoupin.top

================================================================================
来源：http://hxb.hywenlv.cn

[Q01] 创建表
来源：http://niz.andypj.xyz

CREATE TABLE users (
来源：http://yng.aizwys.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jgj.xuanzx.com

name VARCHAR(50) NOT NULL,
来源：http://tcv.0kj1m.cn

email VARCHAR(100) UNIQUE,
来源：http://fou.sxryk.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pmm.zhixingplan.top

);
来源：http://pnp.dianchejie.cn

[Q02] 创建带外键的表
来源：http://etm.yfazqb.com

CREATE TABLE orders (
来源：http://frz.aibaodan.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xsw.yfazqb.com

user_id INT NOT NULL,
来源：http://eoh.xingfuxueyuan.xyz

amount DECIMAL(10, 2),
来源：http://bel.gogol.net.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nir.daria6918.cn

);
来源：http://rcu.jqgfzy.top

[Q03] 增加列
来源：http://xbe.fzhhl.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ltd.xinyue.icu

[Q04] 修改列类型
来源：http://lkl.andypj.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dnn.dashuyun.cn

[Q05] 重命名列
来源：http://ouv.zhengqikj.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://azg.aizwys.cn

[Q06] 删除列
来源：http://bdg.bbcook.cn

ALTER TABLE users DROP COLUMN age;
来源：http://olm.wangdashe.top

[Q07] 删除表
来源：http://tai.dianchejie.cn

DROP TABLE IF EXISTS orders;
来源：http://spi.yuxming.cn

[Q08] 创建普通索引
来源：http://jbx.gotoacloud.top

CREATE INDEX idx_users_email ON users(email);
来源：http://wzk.birdmap.top

[Q09] 创建唯一索引
来源：http://gwo.jinqigfzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cve.cqqwz.cn

[Q10] 插入单行
来源：http://ffd.redwolf501.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yvy.feifeiyinyue.top

[Q11] 一次插入多行
来源：http://rnc.52xcode.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qrz.cashguo.top

[Q12] 插入后取自增 ID
来源：http://dgc.hnxiangtu.top

INSERT INTO users (name) VALUES ('C');
来源：http://yml.pengpengdd.cyou

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dwi.yongpay.top

[Q13] 忽略重复插入
来源：http://ioq.jqgufenzy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oyv.yvedp.cn

[Q14] 存在则更新（upsert）
来源：http://kxv.guannengcc.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jzf.jinyuanbaomall.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://owg.chenlongwang.top

[Q15] 查询全部
来源：http://gvo.316326.xyz

SELECT * FROM users;
来源：http://auz.zycfv.cn

[Q16] 查询指定列
来源：http://ofk.jinghuilouyu.cn

SELECT id, name FROM users;
来源：http://xqj.ydzc1.top

[Q17] 条件查询
来源：http://dbw.jianghu66.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wpa.xinyue.icu

[Q18] 模糊匹配
来源：http://gqe.tian-w.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fvl.quarkkingdee.top

[Q19] 范围查询
来源：http://tqs.ydjk.org.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dbh.sweek.top

[Q20] IN 列表
来源：http://iso.nwbrower.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iql.sjlbkw.cn

[Q21] 空值判断
来源：http://qjb.shuidangran.top

SELECT * FROM users WHERE email IS NULL;
来源：http://esh.yongpay.top

[Q22] 排序
来源：http://coo.ybcxt.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sqk.iojbl.cn

[Q23] 分页
来源：http://mqs.haohaochexian.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lrq.xingfuxueyuan.xyz

[Q24] 去重
来源：http://kvh.jinyuanbaomall.cn

SELECT DISTINCT city FROM users;
来源：http://cel.316326.xyz

[Q25] 只取前 N 条
来源：http://qga.tarul.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qoa.chenjidiqi.icu

[Q26] 计数
来源：http://slc.svipenyu.cn

SELECT COUNT(*) FROM users;
来源：http://knf.vqdsnc.cn

[Q27] 条件计数
来源：http://kwf.yj20258888.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cmu.tanke756.top

[Q28] 求和与平均
来源：http://tad.yvedp.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ltx.jinqigfzy.top

[Q29] 最大最小值
来源：http://spw.yonumen.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://clz.daria6918.cn

[Q30] 分组统计
来源：http://sjz.jianghu66.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://izs.yongpay.top

[Q31] 分组后过滤
来源：http://tkc.gaohongyu789.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zsz.jinqigufen.top

[Q32] 分组拼接字符串
来源：http://sxt.dashuyun.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wmr.haohaochexian.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kdn.epnwcf.com

[Q33] 多列分组
来源：http://zdl.wangdashe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zhx.pengpengdd.cyou

[Q34] 每组取第一条
来源：http://qgb.wangshuangyany.cn

SELECT * FROM (
来源：http://lef.tianlin.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ahn.chenzaomai.com

) t WHERE rn = 1;
来源：http://yxh.c1oappe.top

[Q35] 内连接
来源：http://bws.dashuyun.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gan.uphjek.com

[Q36] 左连接
来源：http://cdz.hysaishi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mpt.epnwcf.com

[Q37] 右连接
来源：http://lbd.shanyushiyangtech.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jsl.xinyue.icu

[Q38] 全外连接（PostgreSQL）
来源：http://yuu.xziqi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ylp.shzxlz.cn

[Q39] 自连接（查上下级）
来源：http://tme.fanxiaobao.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://obf.fanxiaobao.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vsd.0kj1m.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mwb.tianlin.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://obg.xuetiantiany.cn

[Q41] 多表连接
来源：http://vei.sysykeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://zxn.jinghuilouyu.cn

JOIN users u ON u.id = o.user_id
来源：http://bfh.xinyue.icu

JOIN products p ON p.id = o.product_id;
来源：http://ajg.fanxiaobao.xyz

[Q42] 连接条件附加过滤
来源：http://zxn.hnxiangtu.top

SELECT u.name, o.amount FROM users u
来源：http://gfh.uphjek.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mnu.jinyuanbaomall.cn

[Q43] 标量子查询
来源：http://zre.iojbl.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vzx.yuxming.cn

[Q44] IN 子查询
来源：http://wlv.guowangkeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nen.shangyingyoupin.top

[Q45] EXISTS 判断存在
来源：http://gcm.9152youxi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pxw.mhx1999.top

[Q46] NOT EXISTS 判断不存在
来源：http://gvl.chenlongwang.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pln.hysaishi.cn

[Q47] 与平均值比较
来源：http://auu.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cba.sufxvd.cn

[Q48] CTE 公用表表达式
来源：http://nbo.feifeiyinyue.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nzi.gaohongyu789.top

SELECT * FROM t WHERE c > 5;
来源：http://jab.snrcjt.cn

[Q49] 更新单行
来源：http://fsj.shzxlz.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mqb.bbcook.cn

[Q50] 批量更新
来源：http://mkh.jinqigfzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ihw.iojbl.cn

[Q51] 用子查询更新
来源：http://jax.jiagoushi.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iqt.quarkkingdee.top

[Q52] 删除指定行
来源：http://gxp.kuanghao11.cn

DELETE FROM users WHERE id = 10;
来源：http://bsw.epnwcf.com

[Q53] 按条件删除
来源：http://bty.yfazqb.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cuj.sxryk.cn

[Q54] 清空表
来源：http://ijv.yj202588.top

TRUNCATE TABLE logs;
来源：http://ynt.hongshengwenyu.top

[Q55] 排名（并列占位）
来源：http://pwh.aizwys.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bfl.ppjwa.cn

[Q56] 密集排名（并列不占位）
来源：http://oke.ywan-chungtsiang.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://scm.gotoacloud.top

[Q57] 行号
来源：http://iuk.yueranfly.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://spy.shuidangran.top

[Q58] 累计求和
来源：http://frg.yj202588.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dge.yanxiufei.cn

[Q59] 分组内累计
来源：http://mrx.haohaochexian.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gor.havefunace.top

[Q60] 取上一行 / 下一行
来源：http://kil.52xcode.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vkz.kuanghao11.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zqn.ydjk.org.cn

[Q61] 移动平均
来源：http://uwj.gzhubu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://eaj.hongshengwenyu.top

[Q62] 分组占比
来源：http://lvn.vehdjk.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rpg.yueranfly.top

[Q63] 开启事务
来源：http://ewd.gzhubu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://yer.xingfuxueyuan.xyz

[Q64] 提交事务
来源：http://hth.gaohongyu789.top

COMMIT;
来源：http://bxb.jiagoushi.top

[Q65] 回滚事务
来源：http://zuy.uphjek.com

ROLLBACK;
来源：http://ocv.sufxvd.cn

[Q66] 行锁查询
来源：http://jdt.daria6918.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dxa.shanyushiyangtech.top

[Q67] 设置隔离级别
来源：http://ygv.yj20258888.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gfk.aibaodan.cn

[Q68] 保存点
来源：http://qqc.yuxming.cn

SAVEPOINT sp1;
来源：http://dtd.yj20258.top

ROLLBACK TO sp1;
来源：http://zug.xuetiantiany.cn

[Q69] 查看执行计划
来源：http://iqm.aizwys.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://odn.xingfuxueyuan.xyz

[Q70] 更新统计信息
来源：http://vgf.tianlin.xyz

ANALYZE TABLE users;
来源：http://ykc.zhixingplan.top

[Q71] 查看建表语句
来源：http://wlu.hywenlv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fsj.yongpay.top

[Q72] 查看索引
来源：http://xqw.cdnleiting.top

SHOW INDEX FROM users;
来源：http://bwl.hammf.cn

[Q73] 查看表状态
来源：http://zlw.zycfv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ysv.yuxming.cn

[Q74] 强制使用索引
来源：http://pip.iojbl.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sjf.kuanghao11.cn

[Q75] 日期格式化
来源：http://uqx.tian-w.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wze.ydzc1.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dhl.xuanzx.com

[Q76] 按天统计
来源：http://ykd.vehdjk.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ypt.hywenlv.cn

[Q77] 时间加减
来源：http://yvv.zdbjq.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lzd.epnwcf.com

[Q78] 当前时间
来源：http://ujm.zdbjq.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oml.dashuyun.cn

[Q79] 字符串拼接
来源：http://msb.svipenyu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://euf.fanxiaobao.xyz

[Q80] 字符串截取
来源：http://tmc.chenlongwang.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qot.yfazqb.com

[Q81] 字符串替换
来源：http://nda.316326.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://otl.tanke756.top

[Q82] 字符长度与字节长度
来源：http://ash.andypj.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bce.hesvh.cn

[Q83] 大小写转换
来源：http://oge.iojbl.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oiy.xuanzx.com

[Q84] 去除首尾空格
来源：http://cyl.pycfn.com

SELECT TRIM(name) FROM users;
来源：http://nwd.chenjidiqi.icu

[Q85] 数值取整
来源：http://bcp.xuetiantiany.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xse.0kj1m.cn

[Q86] 读取 JSON 字段
来源：http://pzv.xylfe.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jpa.gaohongyu789.top

[Q87] JSON 字段做条件
来源：http://sqr.daria6918.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wcn.gotoacloud.top

[Q88] 行转列（条件聚合）
来源：http://xya.guannengcc.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cce.xuetiantiany.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vay.tarul.cn

[Q89] 判断表是否存在
来源：http://snw.yangfankeji.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xqf.hammf.cn

[Q90] 生成序号列
来源：http://bss.shuidangran.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zqw.dianchejie.cn

================================================================================
来源：http://mpu.andypj.xyz

R. Bash 专题
来源：http://ycx.yj20258888.top

================================================================================
来源：http://ahw.hfpthk.cn

[R01] shebang 与严格模式
来源：http://ffu.ppjwa.cn

#!/usr/bin/env bash
来源：http://dxq.chenzaomai.com

set -euo pipefail
来源：http://xch.ctjpmb.com

[R02] 变量赋值与使用
来源：http://gdg.zycfv.cn

name="Tom"; echo "$name"
来源：http://kbv.gzhubu.top

[R03] 只读变量
来源：http://vof.shangyingyoupin.top

readonly PI=3.14
来源：http://sga.yj20258888.top

[R04] 位置参数
来源：http://zgg.tarul.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cdr.ppjwa.cn

[R05] 参数默认值
来源：http://fkf.smart0.xyz

name="${1:-default}"
来源：http://dnd.daxiang520.top

[R06] 判断命令是否存在
来源：http://cpp.zhixingplan.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cbe.iojbl.cn

[R07] if 判断文件
来源：http://yit.nanxinkj.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ssh.zhiwuduotai.top

[R08] 数值比较
来源：http://gmk.52xcode.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://iiv.0kj1m.cn

[R09] 字符串比较
来源：http://tdr.nanxuanxn.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://moq.nwbrower.top

[R10] 正则匹配
来源：http://hif.jinghuilouyu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rnd.wangdashe.top

[R11] case 多分支
来源：http://bch.uphjek.com

case "$1" in
来源：http://bfl.yongpay.top

start) echo "启动" ;;
来源：http://vuz.chenzaomai.com

stop)  echo "停止" ;;
来源：http://shx.guowangkeji.top

*)     echo "未知命令" ;;
来源：http://jym.gotoacloud.top

esac
来源：http://ziv.xylfe.cn

[R12] for 遍历文件
来源：http://hag.hongshengwenyu.top

for f in *.txt; do echo "$f"; done
来源：http://tly.jlsjyb.cn

[R13] for 计数循环
来源：http://fqu.nanxinkj.top

for i in {1..10}; do echo "$i"; done
来源：http://uwh.ybcxt.top

[R14] C 风格 for
来源：http://eij.fzhhl.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jhd.0kj1m.cn

[R15] while 逐行读文件
来源：http://aql.shanyushiyangtech.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://iov.feifeiyinyue.top

[R16] until 等待条件
来源：http://unj.hammf.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://svt.shanyushiyangtech.top

[R17] 数组定义与取值
来源：http://zua.sjlbkw.cn

arr=(a b c); echo "${arr[0]}"
来源：http://tmn.c1oappe.top

[R18] 遍历数组
来源：http://sez.52xcode.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hyj.yfazqb.com

[R19] 数组长度
来源：http://dwg.zhoulong.xyz

echo "${#arr[@]}"
来源：http://nxt.52xcode.cn

[R20] 关联数组（字典）
来源：http://vkv.c1oappe.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://agf.yj20258888.top

[R21] 字符串长度
来源：http://qtk.yanxiufei.cn

echo "${#s}"
来源：http://oks.sysykeji.top

[R22] 截取子串
来源：http://ihs.aizwys.cn

echo "${s:0:5}"
来源：http://rkf.jqgfzy.top

[R23] 字符串替换
来源：http://kub.cashguo.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wkd.tarul.cn

[R24] 大小写转换
来源：http://flm.bjfxy.top

echo "${s^^}"; echo "${s,,}"
来源：http://muw.chenjidiqi.icu

[R25] 去后缀 / 去前缀
来源：http://jna.hcnkem.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://mrx.gogol.net.cn

[R26] 命令替换
来源：http://ucr.xuetiantiany.cn

now=$(date +%F); echo "$now"
来源：http://xiz.tanke756.top

[R27] 算术展开
来源：http://hje.chenjidiqi.icu

echo $((1 + 2 * 3))
来源：http://myy.feifeiyinyue.top

[R28] 浮点运算
来源：http://fpj.bbcook.cn

echo "scale=2; 10/3" | bc
来源：http://yzw.fktsv.cn

[R29] 定义函数
来源：http://wpt.ivvv.top


<!-- 参考信息 -->