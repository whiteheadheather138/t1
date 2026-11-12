代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://eeg.c1oappe.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wyp.zdbjq.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mfw.jyoumei.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xlz.hnqzz.top

Java: list.size();  map.size();  s.length()
来源：http://nmk.iojbl.cn

Go:   len(arr);  len(m)
来源：http://pde.jinqigfzy.top

Ruby: x.length;  x.size
来源：http://lxr.tian-w.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mwu.zycfv.cn

[P05] 判断两个对象内容是否相等
来源：http://kxl.jinyuanbaomall.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dct.zhijiandao.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cha.yj20258.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://exm.tian-w.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qry.kuanghao11.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kkm.ehwqpu.com

Go:   reflect.DeepEqual(a, b)
来源：http://ajb.yanxiufei.cn

Ruby: a == b
来源：http://ibi.svipenyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fby.cqqwz.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pot.fktsv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lvr.jinqigfzy.top

PHP:  if (empty($x)) {}
来源：http://kmj.jyoumei.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nuu.cdnleiting.top

TS:   if (x == null) {}
来源：http://njx.hammf.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mqp.yangfankeji.com

Go:   if x == nil {}
来源：http://sax.jyoumei.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jue.yj20258888.top

C#:   if (x is null) {}
来源：http://vfg.ydzc1.top

[P07] 防抖与节流
来源：http://rjp.hcnkem.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://scb.ehwqpu.com

PHP:  // 手写时间戳比较
来源：http://owh.yuxming.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://icc.gogol.net.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mbh.smart0.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qim.sxryk.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gcp.c1oappe.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://lok.tanke756.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dpb.hammf.cn

[P08] 处理浮点精度问题
来源：http://mbp.jlsjyb.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bjg.xuanzx.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://suk.zdqjudy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qfn.hywenlv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xuc.aizwys.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ngh.yfazqb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ukn.ppjwa.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ayl.zhoulong.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xmx.zhiwuduotai.top

================================================================================
来源：http://kbo.9152youxi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xmd.ppjwa.cn

================================================================================
来源：http://iof.yuxming.cn

[Q01] 创建表
来源：http://awa.sweek.top

CREATE TABLE users (
来源：http://rwz.yongpay.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://brt.epnwcf.com

name VARCHAR(50) NOT NULL,
来源：http://avt.tianlin.xyz

email VARCHAR(100) UNIQUE,
来源：http://kxf.yj20258.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kfp.zhongyouzk.top

);
来源：http://ewl.ywan-chungtsiang.top

[Q02] 创建带外键的表
来源：http://izx.pycfn.com

CREATE TABLE orders (
来源：http://qzr.dianchejie.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nyh.gzhubu.top

user_id INT NOT NULL,
来源：http://dez.fanxiaobao.xyz

amount DECIMAL(10, 2),
来源：http://uze.52xcode.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gxg.ywan-chungtsiang.top

);
来源：http://nqb.ydzc1.top

[Q03] 增加列
来源：http://qpt.aibaodan.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://twd.xinyue.icu

[Q04] 修改列类型
来源：http://wwq.zhongyouzk.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dtj.zycfv.cn

[Q05] 重命名列
来源：http://myr.wangshuangyany.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xss.pengpengdd.cyou

[Q06] 删除列
来源：http://yug.yonumen.top

ALTER TABLE users DROP COLUMN age;
来源：http://yce.tianlin.xyz

[Q07] 删除表
来源：http://bme.yanxiufei.cn

DROP TABLE IF EXISTS orders;
来源：http://pii.nanxuanxn.top

[Q08] 创建普通索引
来源：http://haf.redwolf501.top

CREATE INDEX idx_users_email ON users(email);
来源：http://mvm.gogol.net.cn

[Q09] 创建唯一索引
来源：http://ymo.hcnkem.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fym.epnwcf.com

[Q10] 插入单行
来源：http://fnf.jyoumei.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://szh.shanyushiyangtech.top

[Q11] 一次插入多行
来源：http://buk.shuidangran.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ipu.birdmap.top

[Q12] 插入后取自增 ID
来源：http://vaf.ppjwa.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tge.shanyushiyangtech.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bvu.feifeiyinyue.top

[Q13] 忽略重复插入
来源：http://ctp.mhx1999.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jix.zycfv.cn

[Q14] 存在则更新（upsert）
来源：http://sgq.jqgufenzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ryv.yvedp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gos.zhiwuduotai.top

[Q15] 查询全部
来源：http://ezj.gaohongyu789.top

SELECT * FROM users;
来源：http://ryc.uphjek.com

[Q16] 查询指定列
来源：http://bir.wangdashe.top

SELECT id, name FROM users;
来源：http://bhc.snrcjt.cn

[Q17] 条件查询
来源：http://sec.bjfxy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fht.jinqigfzy.top

[Q18] 模糊匹配
来源：http://qlb.yvedp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ljf.yvedp.cn

[Q19] 范围查询
来源：http://ndh.c1oappe.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zuh.smart0.xyz

[Q20] IN 列表
来源：http://qxk.nanxuanxn.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://piq.chenjidiqi.icu

[Q21] 空值判断
来源：http://qoi.uphjek.com

SELECT * FROM users WHERE email IS NULL;
来源：http://daz.guowangkeji.top

[Q22] 排序
来源：http://zzv.hammf.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qtf.tanke756.top

[Q23] 分页
来源：http://ztg.hywenlv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zgw.yj202588.top

[Q24] 去重
来源：http://yjo.yanxiufei.cn

SELECT DISTINCT city FROM users;
来源：http://mfe.tian-w.cn

[Q25] 只取前 N 条
来源：http://czz.jqgufenzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://aiv.ehwqpu.com

[Q26] 计数
来源：http://pco.zhengqikj.top

SELECT COUNT(*) FROM users;
来源：http://nri.zhengqikj.top

[Q27] 条件计数
来源：http://pbv.xuanzx.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ghg.zhiwuduotai.top

[Q28] 求和与平均
来源：http://tsa.52xcode.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rxl.sufxvd.cn

[Q29] 最大最小值
来源：http://ijw.iojbl.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ymj.hywenlv.cn

[Q30] 分组统计
来源：http://yit.wangshuangyany.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dxq.zhijiandao.cn

[Q31] 分组后过滤
来源：http://uwh.316326.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sud.meibo888.top

[Q32] 分组拼接字符串
来源：http://jrl.birdmap.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ivi.cashguo.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://iqi.sufxvd.cn

[Q33] 多列分组
来源：http://auw.zdbjq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yjz.cqqwz.cn

[Q34] 每组取第一条
来源：http://lzx.birdmap.top

SELECT * FROM (
来源：http://zqe.xingfuxueyuan.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://njn.nwbrower.top

) t WHERE rn = 1;
来源：http://clo.yongpay.top

[Q35] 内连接
来源：http://sxw.wangdashe.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vad.ppjwa.cn

[Q36] 左连接
来源：http://msa.hnxiangtu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kdn.gogol.net.cn

[Q37] 右连接
来源：http://hze.nanxinkj.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mob.mhx1999.top

[Q38] 全外连接（PostgreSQL）
来源：http://mny.epnwcf.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bzk.ivvv.top

[Q39] 自连接（查上下级）
来源：http://kxs.316326.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://dhm.jqgfzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wnk.ivvv.top

[Q40] 交叉连接（笛卡尔积）
来源：http://tar.52xcode.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://foj.jqgufenzy.top

[Q41] 多表连接
来源：http://jnx.9152youxi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dfk.shanyushiyangtech.top

JOIN users u ON u.id = o.user_id
来源：http://zyj.pycfn.com

JOIN products p ON p.id = o.product_id;
来源：http://wvi.zhiwuduotai.top

[Q42] 连接条件附加过滤
来源：http://qyc.ivvv.top

SELECT u.name, o.amount FROM users u
来源：http://cng.jlsjyb.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://egs.aizwys.cn

[Q43] 标量子查询
来源：http://hta.jiagoushi.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jjf.hfpthk.cn

[Q44] IN 子查询
来源：http://hhl.shzxlz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bwb.yangfankeji.com

[Q45] EXISTS 判断存在
来源：http://orf.chenlongwang.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qgm.jinyuanbaomall.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pwd.nanxuanxn.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qeg.yongpay.top

[Q47] 与平均值比较
来源：http://ztn.chenzaomai.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vgv.redwolf501.top

[Q48] CTE 公用表表达式
来源：http://jnf.cucudq.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ivs.hywenlv.cn

SELECT * FROM t WHERE c > 5;
来源：http://dfc.ydjk.org.cn

[Q49] 更新单行
来源：http://vsw.c1oappe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ixa.xylfe.cn

[Q50] 批量更新
来源：http://ydg.nwbrower.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uds.nanxuanxn.top

[Q51] 用子查询更新
来源：http://cal.zhixingplan.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://udd.chenjidiqi.icu

[Q52] 删除指定行
来源：http://noy.hysaishi.cn

DELETE FROM users WHERE id = 10;
来源：http://nhe.cheryme.top

[Q53] 按条件删除
来源：http://bka.guowangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xvc.hnqzz.top

[Q54] 清空表
来源：http://tzz.zhijiandao.cn

TRUNCATE TABLE logs;
来源：http://vkn.nanxuanxn.top

[Q55] 排名（并列占位）
来源：http://jax.yvedp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xjz.tanke756.top

[Q56] 密集排名（并列不占位）
来源：http://fiq.bjfxy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jzw.andypj.xyz

[Q57] 行号
来源：http://uuc.zhongyouzk.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wah.xingfuxueyuan.xyz

[Q58] 累计求和
来源：http://ofj.gzhubu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fhr.yonumen.top

[Q59] 分组内累计
来源：http://txy.zdqjudy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://atw.xuetiantiany.cn

[Q60] 取上一行 / 下一行
来源：http://rqu.tarul.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tzh.yanxiufei.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hzt.shanyushiyangtech.top

[Q61] 移动平均
来源：http://rjr.shanyushiyangkeji.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sge.dashuyun.cn

[Q62] 分组占比
来源：http://kmm.fehbvm.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://scf.zdqjudy.top

[Q63] 开启事务
来源：http://ccn.yanxiufei.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wxt.fzhhl.top

[Q64] 提交事务
来源：http://ecu.jinqigufen.top

COMMIT;
来源：http://pjo.ehwqpu.com

[Q65] 回滚事务
来源：http://pkb.gzhubu.top

ROLLBACK;
来源：http://txf.jiagoushi.top

[Q66] 行锁查询
来源：http://viu.ctjpmb.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nwl.shangyingyoupin.top

[Q67] 设置隔离级别
来源：http://buk.jiagoushi.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tdf.ydzc1.top

[Q68] 保存点
来源：http://xfl.c1oappe.top

SAVEPOINT sp1;
来源：http://dny.fanxiaobao.xyz

ROLLBACK TO sp1;
来源：http://pjn.ydzc1.top

[Q69] 查看执行计划
来源：http://urx.hongshengwenyu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nyi.yfazqb.com

[Q70] 更新统计信息
来源：http://idc.shanyushiyangkeji.top

ANALYZE TABLE users;
来源：http://ocs.zhengqikj.top

[Q71] 查看建表语句
来源：http://trp.jyoumei.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qim.9152youxi.cn

[Q72] 查看索引
来源：http://zwf.jiagoushi.top

SHOW INDEX FROM users;
来源：http://ocl.wangshuangyany.cn

[Q73] 查看表状态
来源：http://qyg.dashuyun.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ncc.svipenyu.cn

[Q74] 强制使用索引
来源：http://fln.svipenyu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://amu.jyoumei.cn

[Q75] 日期格式化
来源：http://tea.redwolf501.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zmu.52xcode.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://iyh.gaohongyu789.top

[Q76] 按天统计
来源：http://fyt.redwolf501.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://eby.haohaochexian.top

[Q77] 时间加减
来源：http://keo.andypj.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rzd.shzxlz.cn

[Q78] 当前时间
来源：http://mgu.ydzc1.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://klv.tian-w.cn

[Q79] 字符串拼接
来源：http://tlp.jyoumei.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://acr.aibaodan.cn

[Q80] 字符串截取
来源：http://kni.quarkkingdee.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jxx.0kj1m.cn

[Q81] 字符串替换
来源：http://isr.ydjk.org.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ivs.yfazqb.com

[Q82] 字符长度与字节长度
来源：http://ebj.xziqi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rdp.kuanghao11.cn

[Q83] 大小写转换
来源：http://mhu.dianchejie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nvr.sweek.top

[Q84] 去除首尾空格
来源：http://lhv.snrcjt.cn

SELECT TRIM(name) FROM users;
来源：http://uoh.cdnleiting.top

[Q85] 数值取整
来源：http://hdk.svipenyu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xpt.jqgufenzy.top

[Q86] 读取 JSON 字段
来源：http://zor.shanyushiyangkeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dht.ivvv.top

[Q87] JSON 字段做条件
来源：http://drr.zhaomingkeji.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://msn.cqqwz.cn

[Q88] 行转列（条件聚合）
来源：http://usk.xingfuxueyuan.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yge.nanxinkj.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tbv.andypj.xyz

[Q89] 判断表是否存在
来源：http://qrc.nanxinkj.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://aue.tian-w.cn

[Q90] 生成序号列
来源：http://kxp.meibo888.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cgs.0kj1m.cn

================================================================================
来源：http://rvy.hnqzz.top

R. Bash 专题
来源：http://jge.iojbl.cn

================================================================================
来源：http://ofx.aibaodan.cn

[R01] shebang 与严格模式
来源：http://orh.jqgufenzy.top

#!/usr/bin/env bash
来源：http://jna.meibo888.top

set -euo pipefail
来源：http://clw.yueranfly.top

[R02] 变量赋值与使用
来源：http://vyu.hongshengwenyu.top

name="Tom"; echo "$name"
来源：http://qlu.jinyuanbaomall.cn

[R03] 只读变量
来源：http://ruh.shangyingyoupin.top

readonly PI=3.14
来源：http://jjg.bjfxy.top

[R04] 位置参数
来源：http://mzx.yuxming.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hxp.kuanghao11.cn

[R05] 参数默认值
来源：http://byy.meibo888.top

name="${1:-default}"
来源：http://dej.daria6918.cn

[R06] 判断命令是否存在
来源：http://zki.uphjek.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bik.sysykeji.top

[R07] if 判断文件
来源：http://jnc.dashuyun.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://njf.yuxming.cn

[R08] 数值比较
来源：http://hvd.jinyuanbaomall.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://bbi.c1oappe.top

[R09] 字符串比较
来源：http://aiw.gaohongyu789.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lem.redwolf501.top

[R10] 正则匹配
来源：http://qop.jinqigfzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wky.cqqwz.cn

[R11] case 多分支
来源：http://tvp.hnxiangtu.top

case "$1" in
来源：http://dbe.nanxuanxn.top

start) echo "启动" ;;
来源：http://klx.tianlin.xyz

stop)  echo "停止" ;;
来源：http://mps.meibo888.top

*)     echo "未知命令" ;;
来源：http://okg.guannengcc.top

esac
来源：http://zxr.zhoulong.xyz

[R12] for 遍历文件
来源：http://krg.bjfxy.top

for f in *.txt; do echo "$f"; done
来源：http://wge.yongpay.top

[R13] for 计数循环
来源：http://pvf.yfazqb.com

for i in {1..10}; do echo "$i"; done
来源：http://xwf.316326.xyz

[R14] C 风格 for
来源：http://rdo.hammf.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lna.hongshengwenyu.top

[R15] while 逐行读文件
来源：http://esw.guowangkeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://thd.vqdsnc.cn

[R16] until 等待条件
来源：http://eyd.hammf.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qcl.daxiang520.top

[R17] 数组定义与取值
来源：http://yhb.52xcode.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bcv.jlsjyb.cn

[R18] 遍历数组
来源：http://kpy.yj202588.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://owe.gogol.net.cn

[R19] 数组长度
来源：http://qin.hcnkem.com

echo "${#arr[@]}"
来源：http://gve.ybcxt.top

[R20] 关联数组（字典）
来源：http://jlq.yj202588.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hcf.shangyingyoupin.top

[R21] 字符串长度
来源：http://gop.yuxming.cn


<!-- 参考信息 -->