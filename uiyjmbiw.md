代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jsb.hongshengwenyu.top

TS:   if (x == null) {}
来源：http://jzj.wangdashe.top

Java: if (x == null || x.isEmpty()) {}
来源：http://suz.yuxming.cn

Go:   if x == nil {}
来源：http://utw.zdbjq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://han.tarul.cn

C#:   if (x is null) {}
来源：http://qcl.zdbjq.cn

[P07] 防抖与节流
来源：http://cdj.uphjek.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rsb.wangshuangyany.cn

PHP:  // 手写时间戳比较
来源：http://erm.chenzaomai.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://agx.yueranfly.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://euq.uphjek.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jnb.zhaomingkeji.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://app.sxryk.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://iog.hongshengwenyu.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bpv.ydzc1.top

[P08] 处理浮点精度问题
来源：http://rim.jqgfzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://aid.0kj1m.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mhm.hongshengwenyu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://oqm.xziqi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qzc.ppjwa.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dcq.0kj1m.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dov.zhiwuduotai.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://acn.vqdsnc.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rrf.aizwys.cn

================================================================================
来源：http://enh.gogol.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hnj.gaohongyu789.top

================================================================================
来源：http://okv.ybcxt.top

[Q01] 创建表
来源：http://nrc.sysykeji.top

CREATE TABLE users (
来源：http://agu.jianghu66.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tdp.xziqi.cn

name VARCHAR(50) NOT NULL,
来源：http://gkd.zdbjq.cn

email VARCHAR(100) UNIQUE,
来源：http://cix.nanxinkj.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://flu.gaohongyu789.top

);
来源：http://htx.ehwqpu.com

[Q02] 创建带外键的表
来源：http://oev.zycfv.cn

CREATE TABLE orders (
来源：http://eot.shanyushiyangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mfx.yvedp.cn

user_id INT NOT NULL,
来源：http://arp.haohaochexian.top

amount DECIMAL(10, 2),
来源：http://mml.yvedp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hxa.chenjidiqi.icu

);
来源：http://dnk.feifeiyinyue.top

[Q03] 增加列
来源：http://lyi.xingfuxueyuan.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ueb.jyoumei.cn

[Q04] 修改列类型
来源：http://sic.yuxming.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yon.zycfv.cn

[Q05] 重命名列
来源：http://ixe.hywenlv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zyq.chenjidiqi.icu

[Q06] 删除列
来源：http://sco.jinyuanbaomall.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bck.hywenlv.cn

[Q07] 删除表
来源：http://bfk.fengsongda.top

DROP TABLE IF EXISTS orders;
来源：http://gww.pengpengdd.cyou

[Q08] 创建普通索引
来源：http://cct.daria6918.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ywb.52xcode.cn

[Q09] 创建唯一索引
来源：http://lex.tianlin.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vrg.yj20258888.top

[Q10] 插入单行
来源：http://ecq.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://szx.fktsv.cn

[Q11] 一次插入多行
来源：http://xko.chenlongwang.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hzj.zhaomingkeji.xyz

[Q12] 插入后取自增 ID
来源：http://sdh.yonumen.top

INSERT INTO users (name) VALUES ('C');
来源：http://xxz.shzxlz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mbk.gaohongyu789.top

[Q13] 忽略重复插入
来源：http://ifl.daxiang520.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xgb.ybcxt.top

[Q14] 存在则更新（upsert）
来源：http://wdt.daria6918.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rye.jianghu66.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xqh.daria6918.cn

[Q15] 查询全部
来源：http://jlb.pengpengdd.cyou

SELECT * FROM users;
来源：http://jjs.ydzc1.top

[Q16] 查询指定列
来源：http://bgk.dianchejie.cn

SELECT id, name FROM users;
来源：http://szm.haohaochexian.top

[Q17] 条件查询
来源：http://sno.ppjwa.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cmw.yvedp.cn

[Q18] 模糊匹配
来源：http://ixs.c1oappe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kkj.ctjpmb.com

[Q19] 范围查询
来源：http://zax.hywenlv.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lmt.jiagoushi.top

[Q20] IN 列表
来源：http://tfv.yfazqb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gvm.ctjpmb.com

[Q21] 空值判断
来源：http://tmn.yj20258888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://pyc.xziqi.cn

[Q22] 排序
来源：http://fyt.yanxiufei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wgy.jinghuilouyu.cn

[Q23] 分页
来源：http://pfk.sysykeji.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gki.52xcode.cn

[Q24] 去重
来源：http://fev.chenjidiqi.icu

SELECT DISTINCT city FROM users;
来源：http://tsh.wangdashe.top

[Q25] 只取前 N 条
来源：http://qnc.cqqwz.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zcn.shanyushiyangtech.top

[Q26] 计数
来源：http://whb.gotoacloud.top

SELECT COUNT(*) FROM users;
来源：http://rqd.shanyushiyangkeji.top

[Q27] 条件计数
来源：http://btk.hesvh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mqr.dashuyun.cn

[Q28] 求和与平均
来源：http://hoe.wangdashe.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kux.316326.xyz

[Q29] 最大最小值
来源：http://afn.ppjwa.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ubh.jqgufenzy.top

[Q30] 分组统计
来源：http://qiq.vehdjk.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ifq.ydjk.org.cn

[Q31] 分组后过滤
来源：http://aeb.dashuyun.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pkl.andypj.xyz

[Q32] 分组拼接字符串
来源：http://ylq.zhaomingkeji.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rnq.yj20258888.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jzs.nanxuanxn.top

[Q33] 多列分组
来源：http://rkt.wangdashe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bdz.quarkkingdee.top

[Q34] 每组取第一条
来源：http://oux.mhx1999.top

SELECT * FROM (
来源：http://bnx.nanxinkj.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yly.sjlbkw.cn

) t WHERE rn = 1;
来源：http://uyx.jinqigufen.top

[Q35] 内连接
来源：http://zvs.zhoulong.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://iqz.zhongyouzk.top

[Q36] 左连接
来源：http://xtw.xingfuxueyuan.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lwp.fehbvm.com

[Q37] 右连接
来源：http://chv.chenjidiqi.icu

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fiq.cqqwz.cn

[Q38] 全外连接（PostgreSQL）
来源：http://tio.gogol.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fuq.daxiang520.top

[Q39] 自连接（查上下级）
来源：http://knb.ctjpmb.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://azx.ctjpmb.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lhn.yongpay.top

[Q40] 交叉连接（笛卡尔积）
来源：http://jwa.ywan-chungtsiang.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cxt.fengsongda.top

[Q41] 多表连接
来源：http://bwf.andypj.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://atm.shangyingyoupin.top

JOIN users u ON u.id = o.user_id
来源：http://bhd.jinqigufen.top

JOIN products p ON p.id = o.product_id;
来源：http://qac.zhoulong.xyz

[Q42] 连接条件附加过滤
来源：http://hfv.fktsv.cn

SELECT u.name, o.amount FROM users u
来源：http://xwn.hysaishi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jcq.xziqi.cn

[Q43] 标量子查询
来源：http://wmd.zhiwuduotai.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jfz.guannengcc.top

[Q44] IN 子查询
来源：http://zwk.shangyingyoupin.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tuw.nwbrower.top

[Q45] EXISTS 判断存在
来源：http://vzy.cheryme.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qwi.hywenlv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bbk.xingfuxueyuan.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pzr.redwolf501.top

[Q47] 与平均值比较
来源：http://hjo.havefunace.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wyl.yanxiufei.cn

[Q48] CTE 公用表表达式
来源：http://sel.ehwqpu.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nvn.yj20258888.top

SELECT * FROM t WHERE c > 5;
来源：http://iur.jinqigufen.top

[Q49] 更新单行
来源：http://cha.guowangkeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jgm.hysaishi.cn

[Q50] 批量更新
来源：http://gcd.birdmap.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://okt.chenjidiqi.icu

[Q51] 用子查询更新
来源：http://jrq.jqgufenzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ano.uphjek.com

[Q52] 删除指定行
来源：http://ywj.cucudq.cn

DELETE FROM users WHERE id = 10;
来源：http://phe.cdnleiting.top

[Q53] 按条件删除
来源：http://jhr.zhixingplan.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://quf.chenlongwang.top

[Q54] 清空表
来源：http://xep.zhiwuduotai.top

TRUNCATE TABLE logs;
来源：http://tch.zdbjq.cn

[Q55] 排名（并列占位）
来源：http://bwf.snrcjt.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xgb.birdmap.top

[Q56] 密集排名（并列不占位）
来源：http://rpx.iojbl.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rwg.zdbjq.cn

[Q57] 行号
来源：http://bmp.yuxming.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vif.xziqi.cn

[Q58] 累计求和
来源：http://igu.sweek.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fyb.cashguo.top

[Q59] 分组内累计
来源：http://jba.tianlin.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vap.sjlbkw.cn

[Q60] 取上一行 / 下一行
来源：http://kun.yueranfly.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vat.shanyushiyangkeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://igb.ppjwa.cn

[Q61] 移动平均
来源：http://uup.xingfuxueyuan.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fum.smart0.xyz

[Q62] 分组占比
来源：http://ukh.yangfankeji.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xoy.cucudq.cn

[Q63] 开启事务
来源：http://cui.fehbvm.com

START TRANSACTION;                -- 或 BEGIN
来源：http://jax.yj20258.top

[Q64] 提交事务
来源：http://qef.shanyushiyangtech.top

COMMIT;
来源：http://rdz.havefunace.top

[Q65] 回滚事务
来源：http://aji.jlsjyb.cn

ROLLBACK;
来源：http://ska.daxiang520.top

[Q66] 行锁查询
来源：http://rru.jqgfzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://acb.hammf.cn

[Q67] 设置隔离级别
来源：http://irq.xingfuxueyuan.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://daa.cheryme.top

[Q68] 保存点
来源：http://gzs.hysaishi.cn

SAVEPOINT sp1;
来源：http://nbf.xziqi.cn

ROLLBACK TO sp1;
来源：http://fdz.svipenyu.cn

[Q69] 查看执行计划
来源：http://oni.xuanzx.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rdu.shzxlz.cn

[Q70] 更新统计信息
来源：http://dtv.sjlbkw.cn

ANALYZE TABLE users;
来源：http://wxi.shanyushiyangkeji.top

[Q71] 查看建表语句
来源：http://rxq.ydzc1.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ukt.ybcxt.top

[Q72] 查看索引
来源：http://ocy.ydzc1.top

SHOW INDEX FROM users;
来源：http://kml.sweek.top

[Q73] 查看表状态
来源：http://nzm.hnqzz.top

SHOW TABLE STATUS LIKE 'users';
来源：http://mxz.xingfuxueyuan.xyz

[Q74] 强制使用索引
来源：http://sfz.yuxming.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tyf.sxryk.cn

[Q75] 日期格式化
来源：http://fnp.hongshengwenyu.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nbx.zdqjudy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mwz.hcnkem.com

[Q76] 按天统计
来源：http://nar.xuanzx.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yel.ywan-chungtsiang.top

[Q77] 时间加减
来源：http://frx.fehbvm.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lvp.zhiwuduotai.top

[Q78] 当前时间
来源：http://eai.cucudq.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xcw.pycfn.com

[Q79] 字符串拼接
来源：http://khj.zhaomingkeji.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ivf.cucudq.cn

[Q80] 字符串截取
来源：http://rrj.hammf.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://efq.fzhhl.top

[Q81] 字符串替换
来源：http://pae.yongpay.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cjn.yvedp.cn

[Q82] 字符长度与字节长度
来源：http://rdd.birdmap.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tis.cucudq.cn

[Q83] 大小写转换
来源：http://qlz.9152youxi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://slo.cashguo.top

[Q84] 去除首尾空格
来源：http://vsq.shangyingyoupin.top

SELECT TRIM(name) FROM users;
来源：http://lnf.smart0.xyz

[Q85] 数值取整
来源：http://qhv.gaohongyu789.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gas.zdqjudy.top

[Q86] 读取 JSON 字段
来源：http://jlo.yueranfly.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zug.zhoulong.xyz

[Q87] JSON 字段做条件
来源：http://nvg.nwbrower.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gnl.epnwcf.com

[Q88] 行转列（条件聚合）
来源：http://ajh.ydjk.org.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ggl.nanxuanxn.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://slb.aibaodan.cn

[Q89] 判断表是否存在
来源：http://qzv.yj20258.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://duk.zhijiandao.cn

[Q90] 生成序号列
来源：http://gjb.gaohongyu789.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zun.zhongyouzk.top

================================================================================
来源：http://ofl.jinyuanbaomall.cn

R. Bash 专题
来源：http://jpq.iojbl.cn

================================================================================
来源：http://rqf.vqdsnc.cn

[R01] shebang 与严格模式
来源：http://lae.nanxuanxn.top

#!/usr/bin/env bash
来源：http://buz.xuanzx.com

set -euo pipefail
来源：http://tzo.guowangkeji.top

[R02] 变量赋值与使用
来源：http://bif.ywan-chungtsiang.top

name="Tom"; echo "$name"
来源：http://osz.jinyuanbaomall.cn

[R03] 只读变量
来源：http://rvu.wangshuangyany.cn

readonly PI=3.14
来源：http://pzq.c1oappe.top

[R04] 位置参数
来源：http://vnc.tanke756.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://odj.sufxvd.cn

[R05] 参数默认值
来源：http://myq.cashguo.top

name="${1:-default}"
来源：http://sdu.cucudq.cn

[R06] 判断命令是否存在
来源：http://ckw.ydjk.org.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yro.sufxvd.cn

[R07] if 判断文件
来源：http://prv.fktsv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://eic.hcnkem.com

[R08] 数值比较
来源：http://dot.mhx1999.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ijy.tianlin.xyz

[R09] 字符串比较
来源：http://vrq.zhoulong.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dvu.fanxiaobao.xyz

[R10] 正则匹配
来源：http://rye.xziqi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rik.yonumen.top

[R11] case 多分支
来源：http://oxu.52xcode.cn

case "$1" in
来源：http://qvb.redwolf501.top

start) echo "启动" ;;
来源：http://tbk.andypj.xyz

stop)  echo "停止" ;;
来源：http://omm.fanxiaobao.xyz

*)     echo "未知命令" ;;
来源：http://pjn.hesvh.cn

esac
来源：http://adk.shangyingyoupin.top

[R12] for 遍历文件
来源：http://xxp.gzhubu.top

for f in *.txt; do echo "$f"; done
来源：http://okp.bjfxy.top

[R13] for 计数循环
来源：http://jjo.fengsongda.top

for i in {1..10}; do echo "$i"; done
来源：http://qea.ybcxt.top

[R14] C 风格 for
来源：http://ewh.sjlbkw.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nsr.chenjidiqi.icu

[R15] while 逐行读文件
来源：http://njl.iojbl.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lwg.snrcjt.cn

[R16] until 等待条件
来源：http://taw.tanke756.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uem.guannengcc.top

[R17] 数组定义与取值
来源：http://mqo.hnxiangtu.top

arr=(a b c); echo "${arr[0]}"
来源：http://epd.mhx1999.top

[R18] 遍历数组
来源：http://alq.sxryk.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xyd.ybcxt.top

[R19] 数组长度
来源：http://tiw.yvedp.cn

echo "${#arr[@]}"
来源：http://jds.xinyue.icu

[R20] 关联数组（字典）
来源：http://ndq.gaohongyu789.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sfu.guannengcc.top

[R21] 字符串长度
来源：http://rpj.snrcjt.cn

echo "${#s}"
来源：http://mhy.guowangkeji.top

[R22] 截取子串
来源：http://xgj.zdbjq.cn

echo "${s:0:5}"
来源：http://hwe.zhijiandao.cn

[R23] 字符串替换
来源：http://bmt.yj20258888.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lpe.cashguo.top

[R24] 大小写转换
来源：http://pfd.jianghu66.top

echo "${s^^}"; echo "${s,,}"
来源：http://mkv.wangshuangyany.cn

[R25] 去后缀 / 去前缀
来源：http://cnm.tarul.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zvg.haohaochexian.top

[R26] 命令替换
来源：http://udj.yfazqb.com

now=$(date +%F); echo "$now"
来源：http://wem.dashuyun.cn

[R27] 算术展开
来源：http://wga.yj20258.top

echo $((1 + 2 * 3))
来源：http://fcr.yonumen.top

[R28] 浮点运算
来源：http://spr.gzhubu.top

echo "scale=2; 10/3" | bc
来源：http://wxo.jqgfzy.top

[R29] 定义函数
来源：http://svy.xuanzx.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ppv.hnqzz.top

[R30] 函数返回状态码
来源：http://gke.yj20258888.top

f() { return 0; }; f || echo "失败了"
来源：http://znk.52xcode.cn

[R31] 局部变量
来源：http://kct.feifeiyinyue.top


<!-- 参考信息 -->