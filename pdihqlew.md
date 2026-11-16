代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mzg.ydzc1.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://wjs.bbcook.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yfp.shanyushiyangtech.top

[P04] 求长度
来源：http://jod.aizwys.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vkb.cdnleiting.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gtp.ywan-chungtsiang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://idv.gogol.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nbj.birdmap.top

Java: list.size();  map.size();  s.length()
来源：http://oji.gogol.net.cn

Go:   len(arr);  len(m)
来源：http://kli.meibo888.top

Ruby: x.length;  x.size
来源：http://gem.cqqwz.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ozs.yuxming.cn

[P05] 判断两个对象内容是否相等
来源：http://dnl.shuidangran.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ijg.tian-w.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mie.yanxiufei.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://oas.hcnkem.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dep.ydzc1.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rzk.dashuyun.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lib.pycfn.com

Ruby: a == b
来源：http://dvx.shzxlz.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kpm.gzhubu.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ack.pengpengdd.cyou

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mrm.tarul.cn

PHP:  if (empty($x)) {}
来源：http://ewu.zhixingplan.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xee.epnwcf.com

TS:   if (x == null) {}
来源：http://kra.fzhhl.top

Java: if (x == null || x.isEmpty()) {}
来源：http://cgz.fanxiaobao.xyz

Go:   if x == nil {}
来源：http://bcb.ydzc1.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uou.xylfe.cn

C#:   if (x is null) {}
来源：http://rog.hywenlv.cn

[P07] 防抖与节流
来源：http://xlg.ehwqpu.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://odz.yj20258.top

PHP:  // 手写时间戳比较
来源：http://rgi.birdmap.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rwv.hongshengwenyu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ujz.hfpthk.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pje.sjlbkw.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mrw.chenzaomai.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://jrm.shzxlz.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wzw.zdqjudy.top

[P08] 处理浮点精度问题
来源：http://csg.hnxiangtu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dmq.jlsjyb.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ilu.nanxinkj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jjv.vqdsnc.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bol.yuxming.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://suj.sysykeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://omv.yanxiufei.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://brm.ywan-chungtsiang.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://iez.ywan-chungtsiang.top

================================================================================
来源：http://kkn.sufxvd.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://plg.yuxming.cn

================================================================================
来源：http://bga.c1oappe.top

[Q01] 创建表
来源：http://llx.52xcode.cn

CREATE TABLE users (
来源：http://omh.ctjpmb.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rtn.havefunace.top

name VARCHAR(50) NOT NULL,
来源：http://mna.ehwqpu.com

email VARCHAR(100) UNIQUE,
来源：http://qxm.gaohongyu789.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tyz.ppjwa.cn

);
来源：http://fzq.bbcook.cn

[Q02] 创建带外键的表
来源：http://nmu.hywenlv.cn

CREATE TABLE orders (
来源：http://dua.cqqwz.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dqv.yj20258888.top

user_id INT NOT NULL,
来源：http://eke.vehdjk.com

amount DECIMAL(10, 2),
来源：http://vsk.yueranfly.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gpn.yj20258.top

);
来源：http://vnx.ctjpmb.com

[Q03] 增加列
来源：http://ddd.yonumen.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rug.cdnleiting.top

[Q04] 修改列类型
来源：http://xro.wangdashe.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wwq.cqqwz.cn

[Q05] 重命名列
来源：http://skv.hnxiangtu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xkz.hesvh.cn

[Q06] 删除列
来源：http://vjr.hywenlv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bea.chenlongwang.top

[Q07] 删除表
来源：http://viy.fengsongda.top

DROP TABLE IF EXISTS orders;
来源：http://kik.zhixingplan.top

[Q08] 创建普通索引
来源：http://rjg.tarul.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zbt.quarkkingdee.top

[Q09] 创建唯一索引
来源：http://zdj.havefunace.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rlp.yuxming.cn

[Q10] 插入单行
来源：http://tmz.zdbjq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jld.ivvv.top

[Q11] 一次插入多行
来源：http://bni.zhongyouzk.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://acf.zhongyouzk.top

[Q12] 插入后取自增 ID
来源：http://lsn.sweek.top

INSERT INTO users (name) VALUES ('C');
来源：http://stu.chenjidiqi.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fsw.zycfv.cn

[Q13] 忽略重复插入
来源：http://ndz.xinyue.icu

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lvq.vehdjk.com

[Q14] 存在则更新（upsert）
来源：http://eoy.fanxiaobao.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nyj.zhongyouzk.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ped.yvedp.cn

[Q15] 查询全部
来源：http://prq.jianghu66.top

SELECT * FROM users;
来源：http://emq.cdnleiting.top

[Q16] 查询指定列
来源：http://dhy.sufxvd.cn

SELECT id, name FROM users;
来源：http://uko.jinqigufen.top

[Q17] 条件查询
来源：http://vkt.zhaomingkeji.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nmw.tian-w.cn

[Q18] 模糊匹配
来源：http://wjz.9152youxi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rid.sweek.top

[Q19] 范围查询
来源：http://lvo.aibaodan.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://psb.shzxlz.cn

[Q20] IN 列表
来源：http://vpf.xinyue.icu

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cet.ctjpmb.com

[Q21] 空值判断
来源：http://loo.hfpthk.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pbt.zdbjq.cn

[Q22] 排序
来源：http://oll.yuxming.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jwa.snrcjt.cn

[Q23] 分页
来源：http://lyz.tarul.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mpd.jinqigufen.top

[Q24] 去重
来源：http://jww.hcnkem.com

SELECT DISTINCT city FROM users;
来源：http://mgs.jinghuilouyu.cn

[Q25] 只取前 N 条
来源：http://cro.daxiang520.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fym.ehwqpu.com

[Q26] 计数
来源：http://hms.andypj.xyz

SELECT COUNT(*) FROM users;
来源：http://mge.uphjek.com

[Q27] 条件计数
来源：http://rmc.zdqjudy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zud.yfazqb.com

[Q28] 求和与平均
来源：http://tcp.zhengqikj.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pkk.yj20258.top

[Q29] 最大最小值
来源：http://osb.ywan-chungtsiang.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://yhk.yangfankeji.com

[Q30] 分组统计
来源：http://evj.cheryme.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ndt.xylfe.cn

[Q31] 分组后过滤
来源：http://uke.pengpengdd.cyou

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ajx.cucudq.cn

[Q32] 分组拼接字符串
来源：http://auq.yj20258888.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cgp.bjfxy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ccq.aibaodan.cn

[Q33] 多列分组
来源：http://gll.ivvv.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jic.yueranfly.top

[Q34] 每组取第一条
来源：http://hsu.ydjk.org.cn

SELECT * FROM (
来源：http://zhq.ppjwa.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sdn.guowangkeji.top

) t WHERE rn = 1;
来源：http://hra.hywenlv.cn

[Q35] 内连接
来源：http://qot.hnxiangtu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zyp.vqdsnc.cn

[Q36] 左连接
来源：http://ykv.fktsv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ibx.ybcxt.top

[Q37] 右连接
来源：http://xni.jqgufenzy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pjo.9152youxi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ayh.zhiwuduotai.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dem.gzhubu.top

[Q39] 自连接（查上下级）
来源：http://dai.shanyushiyangkeji.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://qoj.xylfe.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zgp.9152youxi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://iev.nanxuanxn.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hll.daria6918.cn

[Q41] 多表连接
来源：http://fyg.tarul.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ksw.chenjidiqi.icu

JOIN users u ON u.id = o.user_id
来源：http://jpf.gzhubu.top

JOIN products p ON p.id = o.product_id;
来源：http://ost.yonumen.top

[Q42] 连接条件附加过滤
来源：http://gyz.gotoacloud.top

SELECT u.name, o.amount FROM users u
来源：http://sfw.xingfuxueyuan.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ldg.xuanzx.com

[Q43] 标量子查询
来源：http://dup.kuanghao11.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qzg.cheryme.top

[Q44] IN 子查询
来源：http://tfv.cdnleiting.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ypy.aibaodan.cn

[Q45] EXISTS 判断存在
来源：http://hxd.aibaodan.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pee.ppjwa.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mtj.sweek.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xbw.sufxvd.cn

[Q47] 与平均值比较
来源：http://inf.hfpthk.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yqp.sjlbkw.cn

[Q48] CTE 公用表表达式
来源：http://mog.shanyushiyangkeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rcc.nanxuanxn.top

SELECT * FROM t WHERE c > 5;
来源：http://ldt.ydjk.org.cn

[Q49] 更新单行
来源：http://qek.zdbjq.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bzq.fengsongda.top

[Q50] 批量更新
来源：http://qlu.9152youxi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://osw.chenzaomai.com

[Q51] 用子查询更新
来源：http://cem.aibaodan.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pnm.tian-w.cn

[Q52] 删除指定行
来源：http://pvn.nwbrower.top

DELETE FROM users WHERE id = 10;
来源：http://pkr.quarkkingdee.top

[Q53] 按条件删除
来源：http://fbo.hammf.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jea.ydjk.org.cn

[Q54] 清空表
来源：http://yda.yj20258888.top

TRUNCATE TABLE logs;
来源：http://vub.jinqigfzy.top

[Q55] 排名（并列占位）
来源：http://vzk.xuanzx.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vst.jinyuanbaomall.cn

[Q56] 密集排名（并列不占位）
来源：http://hbw.bjfxy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kgu.hnqzz.top

[Q57] 行号
来源：http://bch.wangdashe.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uto.fehbvm.com

[Q58] 累计求和
来源：http://iox.birdmap.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ncr.yj20258.top

[Q59] 分组内累计
来源：http://hxr.xziqi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cua.vqdsnc.cn

[Q60] 取上一行 / 下一行
来源：http://mbf.epnwcf.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xpe.xinyue.icu

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sgf.jqgufenzy.top

[Q61] 移动平均
来源：http://uib.yangfankeji.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pgr.tanke756.top

[Q62] 分组占比
来源：http://hhc.hammf.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vgk.fehbvm.com

[Q63] 开启事务
来源：http://fqr.hfpthk.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://knz.ywan-chungtsiang.top

[Q64] 提交事务
来源：http://flj.zycfv.cn

COMMIT;
来源：http://idi.hcnkem.com

[Q65] 回滚事务
来源：http://rsl.nanxinkj.top

ROLLBACK;
来源：http://nqz.xingfuxueyuan.xyz

[Q66] 行锁查询
来源：http://rox.bbcook.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cqf.redwolf501.top

[Q67] 设置隔离级别
来源：http://ltl.yongpay.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gsm.zhaomingkeji.xyz

[Q68] 保存点
来源：http://cad.birdmap.top

SAVEPOINT sp1;
来源：http://qdf.kuanghao11.cn

ROLLBACK TO sp1;
来源：http://ykc.0kj1m.cn

[Q69] 查看执行计划
来源：http://ske.smart0.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://byd.hnqzz.top

[Q70] 更新统计信息
来源：http://jff.ivvv.top

ANALYZE TABLE users;
来源：http://qdp.wangshuangyany.cn

[Q71] 查看建表语句
来源：http://lqh.9152youxi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eyt.zhengqikj.top

[Q72] 查看索引
来源：http://coj.cucudq.cn

SHOW INDEX FROM users;
来源：http://pqc.shzxlz.cn

[Q73] 查看表状态
来源：http://nfw.yfazqb.com

SHOW TABLE STATUS LIKE 'users';
来源：http://gzl.yj202588.top

[Q74] 强制使用索引
来源：http://alh.ppjwa.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ubk.chenjidiqi.icu

[Q75] 日期格式化
来源：http://jvp.fehbvm.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hxm.xinyue.icu

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hor.wangdashe.top

[Q76] 按天统计
来源：http://rrl.cheryme.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xki.dianchejie.cn

[Q77] 时间加减
来源：http://omw.yonumen.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pax.ydjk.org.cn

[Q78] 当前时间
来源：http://zhx.zhoulong.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qre.meibo888.top

[Q79] 字符串拼接
来源：http://umn.0kj1m.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://efi.wangshuangyany.cn

[Q80] 字符串截取
来源：http://snm.dashuyun.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ssf.aibaodan.cn

[Q81] 字符串替换
来源：http://qyh.pengpengdd.cyou

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tmc.pycfn.com

[Q82] 字符长度与字节长度
来源：http://hbs.jqgufenzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rfx.yj20258888.top

[Q83] 大小写转换
来源：http://jui.jqgfzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://aeq.wangshuangyany.cn

[Q84] 去除首尾空格
来源：http://kyn.birdmap.top

SELECT TRIM(name) FROM users;
来源：http://hib.vehdjk.com

[Q85] 数值取整
来源：http://kwv.chenjidiqi.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tno.sufxvd.cn

[Q86] 读取 JSON 字段
来源：http://txo.fanxiaobao.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ths.daxiang520.top

[Q87] JSON 字段做条件
来源：http://mfv.aizwys.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://peh.zhengqikj.top

[Q88] 行转列（条件聚合）
来源：http://pwk.hnxiangtu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://psv.jqgufenzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ood.jqgfzy.top

[Q89] 判断表是否存在
来源：http://lyo.jiagoushi.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://raj.daxiang520.top

[Q90] 生成序号列
来源：http://mpt.ybcxt.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vby.bjfxy.top

================================================================================
来源：http://tci.hongshengwenyu.top

R. Bash 专题
来源：http://elr.jqgufenzy.top

================================================================================
来源：http://jxx.daxiang520.top

[R01] shebang 与严格模式
来源：http://cfu.cqqwz.cn

#!/usr/bin/env bash
来源：http://ame.sufxvd.cn

set -euo pipefail
来源：http://dpv.aizwys.cn

[R02] 变量赋值与使用
来源：http://fip.zhoulong.xyz

name="Tom"; echo "$name"
来源：http://zps.jqgufenzy.top

[R03] 只读变量
来源：http://mhf.xingfuxueyuan.xyz

readonly PI=3.14
来源：http://dxq.jqgfzy.top

[R04] 位置参数
来源：http://uja.daria6918.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vxa.nwbrower.top

[R05] 参数默认值
来源：http://xzp.pycfn.com

name="${1:-default}"
来源：http://mst.wangdashe.top

[R06] 判断命令是否存在
来源：http://ugu.zhongyouzk.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kmo.xylfe.cn

[R07] if 判断文件
来源：http://wsf.shuidangran.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hva.dashuyun.cn

[R08] 数值比较
来源：http://rho.gaohongyu789.top

if (( a > b )); then echo "a 更大"; fi
来源：http://tml.hysaishi.cn

[R09] 字符串比较
来源：http://irc.shzxlz.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bgb.ybcxt.top

[R10] 正则匹配
来源：http://uev.cdnleiting.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fxd.hywenlv.cn

[R11] case 多分支
来源：http://ouc.daxiang520.top

case "$1" in
来源：http://dew.yueranfly.top

start) echo "启动" ;;
来源：http://fno.yj20258.top

stop)  echo "停止" ;;
来源：http://hkr.bjfxy.top

*)     echo "未知命令" ;;
来源：http://uze.xuanzx.com

esac
来源：http://nbx.zycfv.cn

[R12] for 遍历文件
来源：http://vli.guannengcc.top

for f in *.txt; do echo "$f"; done
来源：http://bez.guannengcc.top

[R13] for 计数循环
来源：http://hsd.zhengqikj.top

for i in {1..10}; do echo "$i"; done
来源：http://jgi.kuanghao11.cn

[R14] C 风格 for
来源：http://jak.andypj.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cru.shangyingyoupin.top

[R15] while 逐行读文件
来源：http://ygr.zdqjudy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lul.fehbvm.com

[R16] until 等待条件
来源：http://tib.zdqjudy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gqa.yuxming.cn

[R17] 数组定义与取值
来源：http://yeh.chenzaomai.com

arr=(a b c); echo "${arr[0]}"
来源：http://sso.fzhhl.top

[R18] 遍历数组
来源：http://csc.fzhhl.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ois.hnqzz.top

[R19] 数组长度
来源：http://cmc.birdmap.top


<!-- 参考信息 -->