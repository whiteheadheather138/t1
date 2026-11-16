代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://thl.9152youxi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xro.zhoulong.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hkz.feifeiyinyue.top

[P04] 求长度
来源：http://sff.wangdashe.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bim.yvedp.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zny.andypj.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yki.chenzaomai.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dhi.daria6918.cn

Java: list.size();  map.size();  s.length()
来源：http://bcb.ppjwa.cn

Go:   len(arr);  len(m)
来源：http://pxq.fehbvm.com

Ruby: x.length;  x.size
来源：http://ycn.zdbjq.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://evh.sxryk.cn

[P05] 判断两个对象内容是否相等
来源：http://yyf.nwbrower.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://wvc.sjlbkw.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nkw.redwolf501.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://klp.yongpay.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yyw.nanxinkj.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yaw.epnwcf.com

Go:   reflect.DeepEqual(a, b)
来源：http://qed.dianchejie.cn

Ruby: a == b
来源：http://gnk.jinghuilouyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://oad.feifeiyinyue.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://klu.zdqjudy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zpw.kuanghao11.cn

PHP:  if (empty($x)) {}
来源：http://ams.hnqzz.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zqn.nanxinkj.top

TS:   if (x == null) {}
来源：http://gpt.fanxiaobao.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://idk.jqgufenzy.top

Go:   if x == nil {}
来源：http://ejk.zycfv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ona.aibaodan.cn

C#:   if (x is null) {}
来源：http://mkw.epnwcf.com

[P07] 防抖与节流
来源：http://fgx.hfpthk.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rzi.pengpengdd.cyou

PHP:  // 手写时间戳比较
来源：http://dzm.ivvv.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vrs.gotoacloud.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dpe.xuanzx.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://okz.jyoumei.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jah.xinyue.icu

Ruby: // 手写闭包 + Time.now 判断
来源：http://ogg.meibo888.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mxw.xuetiantiany.cn

[P08] 处理浮点精度问题
来源：http://ygh.guannengcc.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rxf.cashguo.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://meo.dashuyun.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://aor.chenjidiqi.icu

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bsl.yonumen.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gec.pengpengdd.cyou

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nsv.cashguo.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zqt.hfpthk.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ete.xingfuxueyuan.xyz

================================================================================
来源：http://dtq.52xcode.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xsz.ppjwa.cn

================================================================================
来源：http://auf.zhiwuduotai.top

[Q01] 创建表
来源：http://mdz.yvedp.cn

CREATE TABLE users (
来源：http://oyu.sjlbkw.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xrt.cucudq.cn

name VARCHAR(50) NOT NULL,
来源：http://xvp.zhoulong.xyz

email VARCHAR(100) UNIQUE,
来源：http://shh.feifeiyinyue.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://snq.daxiang520.top

);
来源：http://hlz.sweek.top

[Q02] 创建带外键的表
来源：http://ebo.havefunace.top

CREATE TABLE orders (
来源：http://dzs.sweek.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zmx.zdbjq.cn

user_id INT NOT NULL,
来源：http://cwq.iojbl.cn

amount DECIMAL(10, 2),
来源：http://xjq.wangshuangyany.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dng.jqgfzy.top

);
来源：http://paz.shangyingyoupin.top

[Q03] 增加列
来源：http://diw.xuetiantiany.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jbz.xuetiantiany.cn

[Q04] 修改列类型
来源：http://iik.jiagoushi.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wbx.vehdjk.com

[Q05] 重命名列
来源：http://enl.ydzc1.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gkq.0kj1m.cn

[Q06] 删除列
来源：http://ary.hywenlv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://hvx.chenzaomai.com

[Q07] 删除表
来源：http://zmg.cashguo.top

DROP TABLE IF EXISTS orders;
来源：http://dwe.jqgufenzy.top

[Q08] 创建普通索引
来源：http://yts.zhixingplan.top

CREATE INDEX idx_users_email ON users(email);
来源：http://tod.yj20258.top

[Q09] 创建唯一索引
来源：http://vit.haohaochexian.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yxy.cashguo.top

[Q10] 插入单行
来源：http://hzh.yj20258.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jgb.zhijiandao.cn

[Q11] 一次插入多行
来源：http://isu.shangyingyoupin.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cch.fzhhl.top

[Q12] 插入后取自增 ID
来源：http://nlc.shuidangran.top

INSERT INTO users (name) VALUES ('C');
来源：http://axk.dianchejie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yht.ivvv.top

[Q13] 忽略重复插入
来源：http://esm.iojbl.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pvw.yongpay.top

[Q14] 存在则更新（upsert）
来源：http://dfn.hongshengwenyu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://okr.yj20258.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rzf.mhx1999.top

[Q15] 查询全部
来源：http://rmp.jinqigufen.top

SELECT * FROM users;
来源：http://phy.52xcode.cn

[Q16] 查询指定列
来源：http://pnv.aizwys.cn

SELECT id, name FROM users;
来源：http://idx.0kj1m.cn

[Q17] 条件查询
来源：http://vrg.daxiang520.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zyn.52xcode.cn

[Q18] 模糊匹配
来源：http://lcb.dashuyun.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xme.yanxiufei.cn

[Q19] 范围查询
来源：http://ptc.hnxiangtu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ifo.ppjwa.cn

[Q20] IN 列表
来源：http://jpt.ppjwa.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dwl.fengsongda.top

[Q21] 空值判断
来源：http://gcn.fzhhl.top

SELECT * FROM users WHERE email IS NULL;
来源：http://yzf.ehwqpu.com

[Q22] 排序
来源：http://yws.cheryme.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fhe.ctjpmb.com

[Q23] 分页
来源：http://lic.shanyushiyangtech.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ksp.wangshuangyany.cn

[Q24] 去重
来源：http://evl.kuanghao11.cn

SELECT DISTINCT city FROM users;
来源：http://ick.hfpthk.cn

[Q25] 只取前 N 条
来源：http://mci.yonumen.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cmd.sjlbkw.cn

[Q26] 计数
来源：http://rar.ybcxt.top

SELECT COUNT(*) FROM users;
来源：http://tqc.shuidangran.top

[Q27] 条件计数
来源：http://bxl.ppjwa.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://atl.xinyue.icu

[Q28] 求和与平均
来源：http://hjv.uphjek.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vny.zhijiandao.cn

[Q29] 最大最小值
来源：http://ple.ivvv.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://acs.chenlongwang.top

[Q30] 分组统计
来源：http://gcv.hysaishi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wtp.zdbjq.cn

[Q31] 分组后过滤
来源：http://hhz.xinyue.icu

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yaj.redwolf501.top

[Q32] 分组拼接字符串
来源：http://gow.smart0.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ulb.sufxvd.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xzf.jinyuanbaomall.cn

[Q33] 多列分组
来源：http://hmj.xuetiantiany.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ewe.fanxiaobao.xyz

[Q34] 每组取第一条
来源：http://ftb.hnqzz.top

SELECT * FROM (
来源：http://yhi.aibaodan.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yai.hywenlv.cn

) t WHERE rn = 1;
来源：http://mra.jinqigfzy.top

[Q35] 内连接
来源：http://rwm.xinyue.icu

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vod.yangfankeji.com

[Q36] 左连接
来源：http://vdb.ydzc1.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nhc.pengpengdd.cyou

[Q37] 右连接
来源：http://ndn.fanxiaobao.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://szg.birdmap.top

[Q38] 全外连接（PostgreSQL）
来源：http://ywz.nanxuanxn.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ovw.kuanghao11.cn

[Q39] 自连接（查上下级）
来源：http://hnl.zycfv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://blc.tanke756.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dmk.jyoumei.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kjp.hywenlv.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mxx.zdqjudy.top

[Q41] 多表连接
来源：http://wnx.shangyingyoupin.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://fhw.fehbvm.com

JOIN users u ON u.id = o.user_id
来源：http://zve.sjlbkw.cn

JOIN products p ON p.id = o.product_id;
来源：http://urb.xingfuxueyuan.xyz

[Q42] 连接条件附加过滤
来源：http://eyn.jiagoushi.top

SELECT u.name, o.amount FROM users u
来源：http://ssy.hnxiangtu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://iml.aibaodan.cn

[Q43] 标量子查询
来源：http://xzo.tianlin.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sld.ehwqpu.com

[Q44] IN 子查询
来源：http://boz.xinyue.icu

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ksi.jinghuilouyu.cn

[Q45] EXISTS 判断存在
来源：http://gew.hysaishi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hrq.yvedp.cn

[Q46] NOT EXISTS 判断不存在
来源：http://kyx.redwolf501.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://djn.gotoacloud.top

[Q47] 与平均值比较
来源：http://ivi.vqdsnc.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rpq.daria6918.cn

[Q48] CTE 公用表表达式
来源：http://qod.yuxming.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pvf.havefunace.top

SELECT * FROM t WHERE c > 5;
来源：http://ysq.vehdjk.com

[Q49] 更新单行
来源：http://iia.redwolf501.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tld.yongpay.top

[Q50] 批量更新
来源：http://nzu.tanke756.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nte.hnxiangtu.top

[Q51] 用子查询更新
来源：http://hri.cheryme.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sjo.cdnleiting.top

[Q52] 删除指定行
来源：http://cwt.shzxlz.cn

DELETE FROM users WHERE id = 10;
来源：http://phw.ydjk.org.cn

[Q53] 按条件删除
来源：http://zre.jqgfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hhe.hammf.cn

[Q54] 清空表
来源：http://wsa.nwbrower.top

TRUNCATE TABLE logs;
来源：http://kho.xuetiantiany.cn

[Q55] 排名（并列占位）
来源：http://zip.tianlin.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mjo.pycfn.com

[Q56] 密集排名（并列不占位）
来源：http://msm.havefunace.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gyn.sweek.top

[Q57] 行号
来源：http://jed.hnxiangtu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://azp.aizwys.cn

[Q58] 累计求和
来源：http://uht.zhoulong.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zzp.guannengcc.top

[Q59] 分组内累计
来源：http://kvy.yueranfly.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ifg.bbcook.cn

[Q60] 取上一行 / 下一行
来源：http://ypy.gaohongyu789.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://njt.yueranfly.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jum.quarkkingdee.top

[Q61] 移动平均
来源：http://cfn.jinyuanbaomall.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://knq.zhongyouzk.top

[Q62] 分组占比
来源：http://vod.daxiang520.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qko.cucudq.cn

[Q63] 开启事务
来源：http://cel.xziqi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zxj.hnqzz.top

[Q64] 提交事务
来源：http://ztk.hesvh.cn

COMMIT;
来源：http://pwp.xingfuxueyuan.xyz

[Q65] 回滚事务
来源：http://swc.cashguo.top

ROLLBACK;
来源：http://obc.quarkkingdee.top

[Q66] 行锁查询
来源：http://mpq.aibaodan.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fwc.yongpay.top

[Q67] 设置隔离级别
来源：http://gyj.zhixingplan.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kik.fzhhl.top

[Q68] 保存点
来源：http://aje.cheryme.top

SAVEPOINT sp1;
来源：http://ayn.sjlbkw.cn

ROLLBACK TO sp1;
来源：http://nmi.hfpthk.cn

[Q69] 查看执行计划
来源：http://ayh.ivvv.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://idk.snrcjt.cn

[Q70] 更新统计信息
来源：http://pyr.fengsongda.top

ANALYZE TABLE users;
来源：http://gto.xuanzx.com

[Q71] 查看建表语句
来源：http://qeh.jiagoushi.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gar.andypj.xyz

[Q72] 查看索引
来源：http://edg.jiagoushi.top

SHOW INDEX FROM users;
来源：http://dpy.zhoulong.xyz

[Q73] 查看表状态
来源：http://vdz.xziqi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kuh.shuidangran.top

[Q74] 强制使用索引
来源：http://fmd.quarkkingdee.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ffe.hywenlv.cn

[Q75] 日期格式化
来源：http://caf.vehdjk.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rcq.yuxming.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jrv.pengpengdd.cyou

[Q76] 按天统计
来源：http://rpw.yongpay.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://aos.shzxlz.cn

[Q77] 时间加减
来源：http://com.yuanzhike.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jqf.9152youxi.cn

[Q78] 当前时间
来源：http://qek.ctjpmb.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bju.hnqzz.top

[Q79] 字符串拼接
来源：http://fjf.yuxming.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ban.yangfankeji.com

[Q80] 字符串截取
来源：http://qfh.zhiwuduotai.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://emr.quarkkingdee.top

[Q81] 字符串替换
来源：http://lla.andypj.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://eyc.bjfxy.top

[Q82] 字符长度与字节长度
来源：http://yzo.jyoumei.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://orq.smart0.xyz

[Q83] 大小写转换
来源：http://lth.ivvv.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cqj.vehdjk.com

[Q84] 去除首尾空格
来源：http://yat.zhijiandao.cn

SELECT TRIM(name) FROM users;
来源：http://bdh.zycfv.cn

[Q85] 数值取整
来源：http://vzb.316326.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uvu.chenzaomai.com

[Q86] 读取 JSON 字段
来源：http://ibr.tian-w.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qvx.chenzaomai.com

[Q87] JSON 字段做条件
来源：http://kst.smart0.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://etm.vqdsnc.cn

[Q88] 行转列（条件聚合）
来源：http://spw.52xcode.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wyo.chenjidiqi.icu

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://atn.gotoacloud.top

[Q89] 判断表是否存在
来源：http://rxf.smart0.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uvv.9152youxi.cn

[Q90] 生成序号列
来源：http://zfi.bbcook.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tnb.meibo888.top

================================================================================
来源：http://kay.epnwcf.com

R. Bash 专题
来源：http://zmg.iojbl.cn

================================================================================
来源：http://dgu.jiagoushi.top

[R01] shebang 与严格模式
来源：http://woj.hammf.cn

#!/usr/bin/env bash
来源：http://edv.sweek.top

set -euo pipefail
来源：http://nyd.zhixingplan.top

[R02] 变量赋值与使用
来源：http://shz.zdqjudy.top

name="Tom"; echo "$name"
来源：http://abm.jiagoushi.top

[R03] 只读变量
来源：http://qem.zhixingplan.top

readonly PI=3.14
来源：http://rik.bjfxy.top

[R04] 位置参数
来源：http://elj.zhongyouzk.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xfg.hywenlv.cn

[R05] 参数默认值
来源：http://nfg.pycfn.com

name="${1:-default}"
来源：http://qib.jinyuanbaomall.cn

[R06] 判断命令是否存在
来源：http://ldl.fktsv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://htt.cqqwz.cn

[R07] if 判断文件
来源：http://ivq.hnqzz.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nad.ehwqpu.com

[R08] 数值比较
来源：http://uml.birdmap.top

if (( a > b )); then echo "a 更大"; fi
来源：http://dmx.zhongyouzk.top

[R09] 字符串比较
来源：http://flq.jqgufenzy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lkv.tian-w.cn

[R10] 正则匹配
来源：http://pnt.zdqjudy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uim.iojbl.cn

[R11] case 多分支
来源：http://nlx.daxiang520.top

case "$1" in
来源：http://vqg.fehbvm.com

start) echo "启动" ;;
来源：http://vpt.zhijiandao.cn

stop)  echo "停止" ;;
来源：http://lan.jlsjyb.cn

*)     echo "未知命令" ;;
来源：http://okm.yuxming.cn

esac
来源：http://qiw.jinyuanbaomall.cn

[R12] for 遍历文件
来源：http://kfj.birdmap.top

for f in *.txt; do echo "$f"; done
来源：http://mhi.yj20258.top

[R13] for 计数循环
来源：http://krp.mhx1999.top

for i in {1..10}; do echo "$i"; done
来源：http://ilf.c1oappe.top

[R14] C 风格 for
来源：http://zwq.shanyushiyangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sgw.gaohongyu789.top

[R15] while 逐行读文件
来源：http://ryj.ctjpmb.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hvv.zhixingplan.top

[R16] until 等待条件
来源：http://qub.guowangkeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xju.andypj.xyz

[R17] 数组定义与取值
来源：http://mdg.ctjpmb.com

arr=(a b c); echo "${arr[0]}"
来源：http://prc.smart0.xyz

[R18] 遍历数组
来源：http://agl.vqdsnc.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hic.gotoacloud.top

[R19] 数组长度
来源：http://wen.ybcxt.top


<!-- 参考信息 -->