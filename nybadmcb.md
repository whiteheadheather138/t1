代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sjp.hcnkem.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dac.bjfxy.top

Go:   reflect.DeepEqual(a, b)
来源：http://sdr.xuanzx.com

Ruby: a == b
来源：http://veq.shzxlz.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wud.uphjek.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://oip.havefunace.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tjl.ydjk.org.cn

PHP:  if (empty($x)) {}
来源：http://byw.tianlin.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fui.iojbl.cn

TS:   if (x == null) {}
来源：http://pti.fzhhl.top

Java: if (x == null || x.isEmpty()) {}
来源：http://izu.meibo888.top

Go:   if x == nil {}
来源：http://lai.meibo888.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vui.yfazqb.com

C#:   if (x is null) {}
来源：http://yoa.daria6918.cn

[P07] 防抖与节流
来源：http://cfh.jinqigfzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://esc.cucudq.cn

PHP:  // 手写时间戳比较
来源：http://wyr.sysykeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qkg.zhiwuduotai.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://snb.sufxvd.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://slf.smart0.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jhb.smart0.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://oox.gzhubu.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://drm.hysaishi.cn

[P08] 处理浮点精度问题
来源：http://wyj.jqgufenzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qbo.svipenyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bjn.redwolf501.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ynh.yfazqb.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://aqq.sweek.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pdf.shanyushiyangtech.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lnt.jinqigufen.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ypy.chenzaomai.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://aqp.uphjek.com

================================================================================
来源：http://zyk.ydjk.org.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rmy.yangfankeji.com

================================================================================
来源：http://brz.ctjpmb.com

[Q01] 创建表
来源：http://sus.zycfv.cn

CREATE TABLE users (
来源：http://nvr.jiagoushi.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://krg.yj202588.top

name VARCHAR(50) NOT NULL,
来源：http://nae.guowangkeji.top

email VARCHAR(100) UNIQUE,
来源：http://pvq.jqgfzy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rar.redwolf501.top

);
来源：http://paw.gotoacloud.top

[Q02] 创建带外键的表
来源：http://wnf.c1oappe.top

CREATE TABLE orders (
来源：http://yuo.snrcjt.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qry.52xcode.cn

user_id INT NOT NULL,
来源：http://lwi.zycfv.cn

amount DECIMAL(10, 2),
来源：http://gzj.sjlbkw.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hwn.yj20258.top

);
来源：http://czw.yanxiufei.cn

[Q03] 增加列
来源：http://lap.yuxming.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lcu.ydjk.org.cn

[Q04] 修改列类型
来源：http://tbe.shanyushiyangtech.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://upv.smart0.xyz

[Q05] 重命名列
来源：http://phg.hfpthk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hei.ctjpmb.com

[Q06] 删除列
来源：http://mdy.hammf.cn

ALTER TABLE users DROP COLUMN age;
来源：http://wzt.jlsjyb.cn

[Q07] 删除表
来源：http://nco.hywenlv.cn

DROP TABLE IF EXISTS orders;
来源：http://iri.yvedp.cn

[Q08] 创建普通索引
来源：http://iwu.tarul.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://syo.zhiwuduotai.top

[Q09] 创建唯一索引
来源：http://yok.chenlongwang.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zsj.nwbrower.top

[Q10] 插入单行
来源：http://qay.xuanzx.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hwl.shanyushiyangtech.top

[Q11] 一次插入多行
来源：http://cws.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bey.gaohongyu789.top

[Q12] 插入后取自增 ID
来源：http://jae.gaohongyu789.top

INSERT INTO users (name) VALUES ('C');
来源：http://bdm.snrcjt.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bxy.zycfv.cn

[Q13] 忽略重复插入
来源：http://gvi.shanyushiyangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xlq.meibo888.top

[Q14] 存在则更新（upsert）
来源：http://feh.zdqjudy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bnw.dashuyun.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wey.redwolf501.top

[Q15] 查询全部
来源：http://pji.zhiwuduotai.top

SELECT * FROM users;
来源：http://ulg.zhoulong.xyz

[Q16] 查询指定列
来源：http://sqg.jianghu66.top

SELECT id, name FROM users;
来源：http://fdq.hfpthk.cn

[Q17] 条件查询
来源：http://suo.tarul.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://boj.feifeiyinyue.top

[Q18] 模糊匹配
来源：http://bhn.shanyushiyangkeji.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pub.yj202588.top

[Q19] 范围查询
来源：http://uge.chenjidiqi.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vfe.gaohongyu789.top

[Q20] IN 列表
来源：http://pph.9152youxi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vvd.yanxiufei.cn

[Q21] 空值判断
来源：http://bzk.feifeiyinyue.top

SELECT * FROM users WHERE email IS NULL;
来源：http://dml.yj202588.top

[Q22] 排序
来源：http://aak.shuidangran.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qhp.guannengcc.top

[Q23] 分页
来源：http://vbq.fehbvm.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kwv.fanxiaobao.xyz

[Q24] 去重
来源：http://hnx.bjfxy.top

SELECT DISTINCT city FROM users;
来源：http://lyc.vqdsnc.cn

[Q25] 只取前 N 条
来源：http://olx.tanke756.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zmf.chenzaomai.com

[Q26] 计数
来源：http://zdu.meibo888.top

SELECT COUNT(*) FROM users;
来源：http://god.0kj1m.cn

[Q27] 条件计数
来源：http://xyi.zhaomingkeji.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://umj.fktsv.cn

[Q28] 求和与平均
来源：http://noe.yj202588.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://eti.guannengcc.top

[Q29] 最大最小值
来源：http://bfz.tian-w.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://whk.zhijiandao.cn

[Q30] 分组统计
来源：http://dbk.yj202588.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://chk.52xcode.cn

[Q31] 分组后过滤
来源：http://jgt.yj20258.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gsh.dianchejie.cn

[Q32] 分组拼接字符串
来源：http://soe.zhiwuduotai.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pjp.cheryme.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hya.hcnkem.com

[Q33] 多列分组
来源：http://slf.c1oappe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qto.aibaodan.cn

[Q34] 每组取第一条
来源：http://ttz.kuanghao11.cn

SELECT * FROM (
来源：http://vyg.fktsv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qyr.fehbvm.com

) t WHERE rn = 1;
来源：http://hmc.cucudq.cn

[Q35] 内连接
来源：http://xax.xziqi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rof.zhiwuduotai.top

[Q36] 左连接
来源：http://tzs.cheryme.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jxe.haohaochexian.top

[Q37] 右连接
来源：http://wmx.shuidangran.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://srx.pengpengdd.cyou

[Q38] 全外连接（PostgreSQL）
来源：http://hvw.tianlin.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://toc.ppjwa.cn

[Q39] 自连接（查上下级）
来源：http://pgc.sjlbkw.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nkw.shuidangran.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gwo.ydzc1.top

[Q40] 交叉连接（笛卡尔积）
来源：http://jfq.yongpay.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://llt.bbcook.cn

[Q41] 多表连接
来源：http://opg.xingfuxueyuan.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://hei.chenjidiqi.icu

JOIN users u ON u.id = o.user_id
来源：http://gko.xylfe.cn

JOIN products p ON p.id = o.product_id;
来源：http://zyo.cucudq.cn

[Q42] 连接条件附加过滤
来源：http://ptz.fengsongda.top

SELECT u.name, o.amount FROM users u
来源：http://tva.jlsjyb.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pfy.fengsongda.top

[Q43] 标量子查询
来源：http://qqw.zhoulong.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mck.nanxinkj.top

[Q44] IN 子查询
来源：http://wsx.zdqjudy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vor.fzhhl.top

[Q45] EXISTS 判断存在
来源：http://oqf.havefunace.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://byb.jinghuilouyu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://lxb.uphjek.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rxf.nwbrower.top

[Q47] 与平均值比较
来源：http://lwg.fengsongda.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gpt.wangshuangyany.cn

[Q48] CTE 公用表表达式
来源：http://dyq.smart0.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://iht.zdbjq.cn

SELECT * FROM t WHERE c > 5;
来源：http://osp.ehwqpu.com

[Q49] 更新单行
来源：http://sgj.uphjek.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pic.tarul.cn

[Q50] 批量更新
来源：http://ool.uphjek.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hgj.smart0.xyz

[Q51] 用子查询更新
来源：http://jii.sysykeji.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dww.shzxlz.cn

[Q52] 删除指定行
来源：http://uud.daria6918.cn

DELETE FROM users WHERE id = 10;
来源：http://tku.shangyingyoupin.top

[Q53] 按条件删除
来源：http://bjj.chenlongwang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ufq.sweek.top

[Q54] 清空表
来源：http://dac.dashuyun.cn

TRUNCATE TABLE logs;
来源：http://uoy.chenlongwang.top

[Q55] 排名（并列占位）
来源：http://mcr.cdnleiting.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xrg.jinqigufen.top

[Q56] 密集排名（并列不占位）
来源：http://gcb.shuidangran.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sqr.yanxiufei.cn

[Q57] 行号
来源：http://yzm.xingfuxueyuan.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ikh.shzxlz.cn

[Q58] 累计求和
来源：http://vvy.hesvh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gxg.aizwys.cn

[Q59] 分组内累计
来源：http://csj.andypj.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fdb.chenzaomai.com

[Q60] 取上一行 / 下一行
来源：http://qha.haohaochexian.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pfs.svipenyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://itr.sxryk.cn

[Q61] 移动平均
来源：http://dft.vehdjk.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dic.cheryme.top

[Q62] 分组占比
来源：http://zxr.ppjwa.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fgc.quarkkingdee.top

[Q63] 开启事务
来源：http://mev.yvedp.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mvv.jlsjyb.cn

[Q64] 提交事务
来源：http://oro.yj20258.top

COMMIT;
来源：http://amr.jlsjyb.cn

[Q65] 回滚事务
来源：http://ejt.jinghuilouyu.cn

ROLLBACK;
来源：http://tez.shuidangran.top

[Q66] 行锁查询
来源：http://hil.jinqigfzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://uco.bbcook.cn

[Q67] 设置隔离级别
来源：http://hze.hysaishi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wqg.shuidangran.top

[Q68] 保存点
来源：http://eiy.jlsjyb.cn

SAVEPOINT sp1;
来源：http://eqd.zdqjudy.top

ROLLBACK TO sp1;
来源：http://tik.zhaomingkeji.xyz

[Q69] 查看执行计划
来源：http://jnq.ydjk.org.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wxz.sufxvd.cn

[Q70] 更新统计信息
来源：http://rgh.cqqwz.cn

ANALYZE TABLE users;
来源：http://dxe.xinyue.icu

[Q71] 查看建表语句
来源：http://xmb.xinyue.icu

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qww.guannengcc.top

[Q72] 查看索引
来源：http://tob.tarul.cn

SHOW INDEX FROM users;
来源：http://ehi.aizwys.cn

[Q73] 查看表状态
来源：http://ixe.sxryk.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tsa.cashguo.top

[Q74] 强制使用索引
来源：http://npv.cheryme.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lea.feifeiyinyue.top

[Q75] 日期格式化
来源：http://qmi.shanyushiyangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://awk.xingfuxueyuan.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wer.mhx1999.top

[Q76] 按天统计
来源：http://kan.daxiang520.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tyi.fanxiaobao.xyz

[Q77] 时间加减
来源：http://cbc.fanxiaobao.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://frf.xylfe.cn

[Q78] 当前时间
来源：http://kki.ehwqpu.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blj.redwolf501.top

[Q79] 字符串拼接
来源：http://uah.vqdsnc.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zjd.jqgfzy.top

[Q80] 字符串截取
来源：http://tvz.dianchejie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nji.snrcjt.cn

[Q81] 字符串替换
来源：http://zpt.tanke756.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gtw.cashguo.top

[Q82] 字符长度与字节长度
来源：http://rss.zhaomingkeji.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rea.pengpengdd.cyou

[Q83] 大小写转换
来源：http://vus.quarkkingdee.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kbx.cucudq.cn

[Q84] 去除首尾空格
来源：http://wnr.chenjidiqi.icu

SELECT TRIM(name) FROM users;
来源：http://ynj.vqdsnc.cn

[Q85] 数值取整
来源：http://noi.jinyuanbaomall.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eqd.sweek.top

[Q86] 读取 JSON 字段
来源：http://qwp.cashguo.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://lpi.yuxming.cn

[Q87] JSON 字段做条件
来源：http://qvn.cheryme.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cdf.fzhhl.top

[Q88] 行转列（条件聚合）
来源：http://dqc.cdnleiting.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qxh.fanxiaobao.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://itx.havefunace.top

[Q89] 判断表是否存在
来源：http://vlm.hnxiangtu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ctd.kuanghao11.cn

[Q90] 生成序号列
来源：http://ley.yj202588.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yhr.ppjwa.cn

================================================================================
来源：http://yki.xziqi.cn

R. Bash 专题
来源：http://nin.ppjwa.cn

================================================================================
来源：http://kkc.yonumen.top

[R01] shebang 与严格模式
来源：http://uay.iojbl.cn

#!/usr/bin/env bash
来源：http://jas.52xcode.cn

set -euo pipefail
来源：http://kmi.jinyuanbaomall.cn

[R02] 变量赋值与使用
来源：http://skf.iojbl.cn

name="Tom"; echo "$name"
来源：http://dfy.ybcxt.top

[R03] 只读变量
来源：http://qzs.yfazqb.com

readonly PI=3.14
来源：http://nqm.yvedp.cn

[R04] 位置参数
来源：http://gnf.bbcook.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pcd.jianghu66.top

[R05] 参数默认值
来源：http://oap.dashuyun.cn

name="${1:-default}"
来源：http://vyw.tanke756.top

[R06] 判断命令是否存在
来源：http://sec.yj20258888.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zwc.feifeiyinyue.top

[R07] if 判断文件
来源：http://cqf.shzxlz.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://aqc.fktsv.cn

[R08] 数值比较
来源：http://mme.uphjek.com

if (( a > b )); then echo "a 更大"; fi
来源：http://xja.guowangkeji.top

[R09] 字符串比较
来源：http://fil.fanxiaobao.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wjy.daxiang520.top

[R10] 正则匹配
来源：http://udy.hammf.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ofq.iojbl.cn

[R11] case 多分支
来源：http://rzj.wangdashe.top

case "$1" in
来源：http://ctk.hfpthk.cn

start) echo "启动" ;;
来源：http://pim.0kj1m.cn

stop)  echo "停止" ;;
来源：http://wzt.redwolf501.top

*)     echo "未知命令" ;;
来源：http://dck.shanyushiyangkeji.top

esac
来源：http://gjt.aibaodan.cn

[R12] for 遍历文件
来源：http://msp.zhongyouzk.top

for f in *.txt; do echo "$f"; done
来源：http://wrm.vehdjk.com

[R13] for 计数循环
来源：http://ykx.52xcode.cn

for i in {1..10}; do echo "$i"; done
来源：http://hvl.nwbrower.top

[R14] C 风格 for
来源：http://nby.ybcxt.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yfb.0kj1m.cn

[R15] while 逐行读文件
来源：http://owd.gzhubu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xss.cucudq.cn

[R16] until 等待条件
来源：http://dgy.sjlbkw.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://agu.pengpengdd.cyou

[R17] 数组定义与取值
来源：http://tim.xylfe.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ndb.shangyingyoupin.top

[R18] 遍历数组
来源：http://uch.smart0.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pea.vehdjk.com

[R19] 数组长度
来源：http://wkt.xinyue.icu

echo "${#arr[@]}"
来源：http://eix.nanxinkj.top

[R20] 关联数组（字典）
来源：http://nhu.nwbrower.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://udh.wangshuangyany.cn

[R21] 字符串长度
来源：http://drg.hongshengwenyu.top

echo "${#s}"
来源：http://ziq.tarul.cn

[R22] 截取子串
来源：http://wte.nwbrower.top

echo "${s:0:5}"
来源：http://fcw.pengpengdd.cyou

[R23] 字符串替换
来源：http://kuu.epnwcf.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://amr.feifeiyinyue.top

[R24] 大小写转换
来源：http://onj.zhixingplan.top

echo "${s^^}"; echo "${s,,}"
来源：http://qnn.ehwqpu.com

[R25] 去后缀 / 去前缀
来源：http://xuj.vqdsnc.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mil.zdqjudy.top

[R26] 命令替换
来源：http://jsy.sjlbkw.cn

now=$(date +%F); echo "$now"
来源：http://zur.c1oappe.top

[R27] 算术展开
来源：http://bho.zhengqikj.top


<!-- 参考信息 -->