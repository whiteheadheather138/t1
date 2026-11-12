代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rdh.hnqzz.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yeu.yongpay.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ate.cheryme.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mgl.cucudq.cn

Java: list.size();  map.size();  s.length()
来源：http://fup.ywan-chungtsiang.top

Go:   len(arr);  len(m)
来源：http://sru.shangyingyoupin.top

Ruby: x.length;  x.size
来源：http://nra.zhengqikj.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dvi.xuetiantiany.cn

[P05] 判断两个对象内容是否相等
来源：http://dcq.yanxiufei.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fik.0kj1m.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cyh.yanxiufei.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hub.jinyuanbaomall.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yqf.jinqigfzy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lzz.hongshengwenyu.top

Go:   reflect.DeepEqual(a, b)
来源：http://otm.wangdashe.top

Ruby: a == b
来源：http://gvn.chenzaomai.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tcy.wangshuangyany.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wyp.zycfv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://szx.zhongyouzk.top

PHP:  if (empty($x)) {}
来源：http://tkf.hesvh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wcq.jinyuanbaomall.cn

TS:   if (x == null) {}
来源：http://mwt.sjlbkw.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bsd.gaohongyu789.top

Go:   if x == nil {}
来源：http://cew.hnxiangtu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uws.sjlbkw.cn

C#:   if (x is null) {}
来源：http://wsv.jinghuilouyu.cn

[P07] 防抖与节流
来源：http://vwi.tarul.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bmt.hcnkem.com

PHP:  // 手写时间戳比较
来源：http://buw.hammf.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zju.mhx1999.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uuu.c1oappe.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tfl.chenjidiqi.icu

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://apl.andypj.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://hjr.daria6918.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kwg.dashuyun.cn

[P08] 处理浮点精度问题
来源：http://jbw.yongpay.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hgk.wangshuangyany.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://geg.yangfankeji.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ffg.smart0.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lso.kuanghao11.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ass.aizwys.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xbm.hongshengwenyu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lyw.hnxiangtu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wda.vqdsnc.cn

================================================================================
来源：http://gsd.hywenlv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hkm.jinghuilouyu.cn

================================================================================
来源：http://kle.sysykeji.top

[Q01] 创建表
来源：http://bgi.zhiwuduotai.top

CREATE TABLE users (
来源：http://iql.yj20258888.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zkt.meibo888.top

name VARCHAR(50) NOT NULL,
来源：http://ltd.hywenlv.cn

email VARCHAR(100) UNIQUE,
来源：http://qiw.xziqi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pts.dashuyun.cn

);
来源：http://liw.tanke756.top

[Q02] 创建带外键的表
来源：http://adp.gogol.net.cn

CREATE TABLE orders (
来源：http://cox.xuanzx.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fcm.shanyushiyangtech.top

user_id INT NOT NULL,
来源：http://acc.jinghuilouyu.cn

amount DECIMAL(10, 2),
来源：http://ntp.dashuyun.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rfx.chenjidiqi.icu

);
来源：http://kvp.zhiwuduotai.top

[Q03] 增加列
来源：http://hag.yanxiufei.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mfx.yfazqb.com

[Q04] 修改列类型
来源：http://iwe.yuanzhike.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qbj.9152youxi.cn

[Q05] 重命名列
来源：http://rua.hesvh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lom.hammf.cn

[Q06] 删除列
来源：http://gub.ybcxt.top

ALTER TABLE users DROP COLUMN age;
来源：http://gjx.vqdsnc.cn

[Q07] 删除表
来源：http://jql.xylfe.cn

DROP TABLE IF EXISTS orders;
来源：http://hgj.xziqi.cn

[Q08] 创建普通索引
来源：http://zit.meibo888.top

CREATE INDEX idx_users_email ON users(email);
来源：http://uyb.yfazqb.com

[Q09] 创建唯一索引
来源：http://jru.ctjpmb.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gon.snrcjt.cn

[Q10] 插入单行
来源：http://rku.zdbjq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://juz.52xcode.cn

[Q11] 一次插入多行
来源：http://aat.hnqzz.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cgy.hongshengwenyu.top

[Q12] 插入后取自增 ID
来源：http://mid.jinyuanbaomall.cn

INSERT INTO users (name) VALUES ('C');
来源：http://mba.shzxlz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tka.zhongyouzk.top

[Q13] 忽略重复插入
来源：http://yzl.zhixingplan.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fhr.aibaodan.cn

[Q14] 存在则更新（upsert）
来源：http://tyn.gzhubu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mxl.fanxiaobao.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yoa.zhijiandao.cn

[Q15] 查询全部
来源：http://bnh.fehbvm.com

SELECT * FROM users;
来源：http://uyp.yfazqb.com

[Q16] 查询指定列
来源：http://hck.fengsongda.top

SELECT id, name FROM users;
来源：http://hkt.jyoumei.cn

[Q17] 条件查询
来源：http://yjc.quarkkingdee.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://izn.zdqjudy.top

[Q18] 模糊匹配
来源：http://tvo.cucudq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://imf.ivvv.top

[Q19] 范围查询
来源：http://hwm.shangyingyoupin.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://efc.birdmap.top

[Q20] IN 列表
来源：http://jzh.xziqi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jwt.xinyue.icu

[Q21] 空值判断
来源：http://dgt.vehdjk.com

SELECT * FROM users WHERE email IS NULL;
来源：http://mdr.yj202588.top

[Q22] 排序
来源：http://qsd.smart0.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jxy.hnqzz.top

[Q23] 分页
来源：http://jac.cheryme.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vek.feifeiyinyue.top

[Q24] 去重
来源：http://opf.jinqigfzy.top

SELECT DISTINCT city FROM users;
来源：http://mzc.jiagoushi.top

[Q25] 只取前 N 条
来源：http://lux.hongshengwenyu.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lwi.cqqwz.cn

[Q26] 计数
来源：http://njt.andypj.xyz

SELECT COUNT(*) FROM users;
来源：http://upz.fehbvm.com

[Q27] 条件计数
来源：http://dxy.zycfv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jcp.fktsv.cn

[Q28] 求和与平均
来源：http://pca.zhiwuduotai.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xtb.zhongyouzk.top

[Q29] 最大最小值
来源：http://kyb.ywan-chungtsiang.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://fve.ydzc1.top

[Q30] 分组统计
来源：http://osv.guowangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dmt.ydzc1.top

[Q31] 分组后过滤
来源：http://pdk.ctjpmb.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jhs.meibo888.top

[Q32] 分组拼接字符串
来源：http://eyf.hesvh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pcz.hcnkem.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tle.jinyuanbaomall.cn

[Q33] 多列分组
来源：http://zxf.gaohongyu789.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hwu.zhaomingkeji.xyz

[Q34] 每组取第一条
来源：http://ymb.zdbjq.cn

SELECT * FROM (
来源：http://kgg.nanxinkj.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fnh.xuanzx.com

) t WHERE rn = 1;
来源：http://fsv.hongshengwenyu.top

[Q35] 内连接
来源：http://xtb.hfpthk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mlz.jiagoushi.top

[Q36] 左连接
来源：http://ayy.gogol.net.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://obm.havefunace.top

[Q37] 右连接
来源：http://hzb.havefunace.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://prg.jlsjyb.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ijb.epnwcf.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ode.zhiwuduotai.top

[Q39] 自连接（查上下级）
来源：http://hhm.jinyuanbaomall.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://rdq.svipenyu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tpc.nanxinkj.top

[Q40] 交叉连接（笛卡尔积）
来源：http://scp.yj20258.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yes.shanyushiyangtech.top

[Q41] 多表连接
来源：http://ygi.wangdashe.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://rse.cucudq.cn

JOIN users u ON u.id = o.user_id
来源：http://yan.yuxming.cn

JOIN products p ON p.id = o.product_id;
来源：http://siu.yueranfly.top

[Q42] 连接条件附加过滤
来源：http://bfm.haohaochexian.top

SELECT u.name, o.amount FROM users u
来源：http://zdv.nanxinkj.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://crm.yangfankeji.com

[Q43] 标量子查询
来源：http://gfv.fehbvm.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jfx.zhengqikj.top

[Q44] IN 子查询
来源：http://ddf.hnxiangtu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gwb.aizwys.cn

[Q45] EXISTS 判断存在
来源：http://azf.shzxlz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rhx.jqgfzy.top

[Q46] NOT EXISTS 判断不存在
来源：http://pwo.fzhhl.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lyf.yangfankeji.com

[Q47] 与平均值比较
来源：http://cmk.jqgufenzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vej.bbcook.cn

[Q48] CTE 公用表表达式
来源：http://cxv.epnwcf.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rtc.sxryk.cn

SELECT * FROM t WHERE c > 5;
来源：http://tyi.xingfuxueyuan.xyz

[Q49] 更新单行
来源：http://hwf.bjfxy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gye.hesvh.cn

[Q50] 批量更新
来源：http://med.shzxlz.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://knq.jinyuanbaomall.cn

[Q51] 用子查询更新
来源：http://ddc.cdnleiting.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uwj.jqgfzy.top

[Q52] 删除指定行
来源：http://gut.ppjwa.cn

DELETE FROM users WHERE id = 10;
来源：http://awl.aibaodan.cn

[Q53] 按条件删除
来源：http://nvp.tarul.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mrt.yvedp.cn

[Q54] 清空表
来源：http://xat.tianlin.xyz

TRUNCATE TABLE logs;
来源：http://ara.hnqzz.top

[Q55] 排名（并列占位）
来源：http://nhp.quarkkingdee.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yjr.hysaishi.cn

[Q56] 密集排名（并列不占位）
来源：http://cvg.fanxiaobao.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://juj.yj20258.top

[Q57] 行号
来源：http://xpq.52xcode.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lhe.zycfv.cn

[Q58] 累计求和
来源：http://aji.yonumen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qdw.ehwqpu.com

[Q59] 分组内累计
来源：http://prj.gaohongyu789.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://oam.snrcjt.cn

[Q60] 取上一行 / 下一行
来源：http://prl.cucudq.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uhi.yj20258.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nav.pycfn.com

[Q61] 移动平均
来源：http://qld.jqgufenzy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nfr.jianghu66.top

[Q62] 分组占比
来源：http://jzk.jianghu66.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://akl.iojbl.cn

[Q63] 开启事务
来源：http://lck.jianghu66.top

START TRANSACTION;                -- 或 BEGIN
来源：http://umf.sjlbkw.cn

[Q64] 提交事务
来源：http://hgq.guowangkeji.top

COMMIT;
来源：http://kqr.yj20258888.top

[Q65] 回滚事务
来源：http://wvt.ybcxt.top

ROLLBACK;
来源：http://xnv.hfpthk.cn

[Q66] 行锁查询
来源：http://yfo.cdnleiting.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://orr.hesvh.cn

[Q67] 设置隔离级别
来源：http://poe.hywenlv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://scu.yangfankeji.com

[Q68] 保存点
来源：http://jra.jiagoushi.top

SAVEPOINT sp1;
来源：http://xpm.hammf.cn

ROLLBACK TO sp1;
来源：http://tqh.fengsongda.top

[Q69] 查看执行计划
来源：http://ogr.fzhhl.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rgj.sufxvd.cn

[Q70] 更新统计信息
来源：http://jsu.yj20258888.top

ANALYZE TABLE users;
来源：http://xyx.chenlongwang.top

[Q71] 查看建表语句
来源：http://lmz.redwolf501.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cyq.cdnleiting.top

[Q72] 查看索引
来源：http://cnp.ppjwa.cn

SHOW INDEX FROM users;
来源：http://tkb.snrcjt.cn

[Q73] 查看表状态
来源：http://azg.shzxlz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hki.xziqi.cn

[Q74] 强制使用索引
来源：http://glz.smart0.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kbz.yangfankeji.com

[Q75] 日期格式化
来源：http://fuy.vqdsnc.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jyc.guannengcc.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zsl.ppjwa.cn

[Q76] 按天统计
来源：http://ivz.yanxiufei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://eal.nanxuanxn.top

[Q77] 时间加减
来源：http://tsw.yangfankeji.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sqd.sjlbkw.cn

[Q78] 当前时间
来源：http://hqg.havefunace.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vdn.sjlbkw.cn

[Q79] 字符串拼接
来源：http://xxe.hammf.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hwk.zhiwuduotai.top

[Q80] 字符串截取
来源：http://bap.jinqigfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dju.hammf.cn

[Q81] 字符串替换
来源：http://lpb.mhx1999.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://msq.hfpthk.cn

[Q82] 字符长度与字节长度
来源：http://umx.9152youxi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xra.mhx1999.top

[Q83] 大小写转换
来源：http://cwh.hnqzz.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ntq.sysykeji.top

[Q84] 去除首尾空格
来源：http://njt.smart0.xyz

SELECT TRIM(name) FROM users;
来源：http://act.haohaochexian.top

[Q85] 数值取整
来源：http://rqu.cqqwz.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ugt.52xcode.cn

[Q86] 读取 JSON 字段
来源：http://lge.meibo888.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tnz.gotoacloud.top

[Q87] JSON 字段做条件
来源：http://efb.hongshengwenyu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zto.yj20258888.top

[Q88] 行转列（条件聚合）
来源：http://aut.aizwys.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wzg.jiagoushi.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vms.snrcjt.cn

[Q89] 判断表是否存在
来源：http://stg.9152youxi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ddx.bbcook.cn

[Q90] 生成序号列
来源：http://hzc.jqgfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mwz.sysykeji.top

================================================================================
来源：http://ntz.snrcjt.cn

R. Bash 专题
来源：http://fzr.tarul.cn

================================================================================
来源：http://zlh.cashguo.top

[R01] shebang 与严格模式
来源：http://wwb.sweek.top

#!/usr/bin/env bash
来源：http://tnu.bjfxy.top

set -euo pipefail
来源：http://sud.hfpthk.cn

[R02] 变量赋值与使用
来源：http://mpq.tarul.cn

name="Tom"; echo "$name"
来源：http://viq.cdnleiting.top

[R03] 只读变量
来源：http://fke.xingfuxueyuan.xyz

readonly PI=3.14
来源：http://psc.jqgfzy.top

[R04] 位置参数
来源：http://tvk.jqgfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ctr.uphjek.com

[R05] 参数默认值
来源：http://gbm.epnwcf.com

name="${1:-default}"
来源：http://olu.iojbl.cn

[R06] 判断命令是否存在
来源：http://qcd.vehdjk.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uvr.zdqjudy.top

[R07] if 判断文件
来源：http://cym.cheryme.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uyv.xingfuxueyuan.xyz

[R08] 数值比较
来源：http://kji.yueranfly.top

if (( a > b )); then echo "a 更大"; fi
来源：http://upg.zycfv.cn

[R09] 字符串比较
来源：http://pab.cashguo.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pxh.cheryme.top

[R10] 正则匹配
来源：http://yjw.ybcxt.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uzd.shzxlz.cn

[R11] case 多分支
来源：http://bba.jlsjyb.cn

case "$1" in
来源：http://ubp.shanyushiyangkeji.top

start) echo "启动" ;;
来源：http://tra.yongpay.top

stop)  echo "停止" ;;
来源：http://wwa.jianghu66.top

*)     echo "未知命令" ;;
来源：http://dwg.daria6918.cn

esac
来源：http://mbd.yj202588.top

[R12] for 遍历文件
来源：http://qqw.sysykeji.top

for f in *.txt; do echo "$f"; done
来源：http://yth.gzhubu.top

[R13] for 计数循环
来源：http://rkk.chenzaomai.com

for i in {1..10}; do echo "$i"; done
来源：http://smq.gzhubu.top

[R14] C 风格 for
来源：http://zqg.shangyingyoupin.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://evh.zdbjq.cn

[R15] while 逐行读文件
来源：http://xrj.meibo888.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://abt.hammf.cn

[R16] until 等待条件
来源：http://ubh.guannengcc.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ckm.jinghuilouyu.cn

[R17] 数组定义与取值
来源：http://esm.xuetiantiany.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kum.nanxuanxn.top

[R18] 遍历数组
来源：http://gvt.nanxuanxn.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://iiv.fehbvm.com

[R19] 数组长度
来源：http://lrk.fehbvm.com

echo "${#arr[@]}"
来源：http://gsm.dashuyun.cn

[R20] 关联数组（字典）
来源：http://fmi.dianchejie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bye.yonumen.top

[R21] 字符串长度
来源：http://ymg.kuanghao11.cn


<!-- 参考信息 -->