代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://psk.jqgufenzy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pkr.uphjek.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rmy.cashguo.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://shd.cqqwz.cn

Java: list.size();  map.size();  s.length()
来源：http://xhd.uphjek.com

Go:   len(arr);  len(m)
来源：http://ktc.gzhubu.top

Ruby: x.length;  x.size
来源：http://lkk.redwolf501.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://twx.jqgfzy.top

[P05] 判断两个对象内容是否相等
来源：http://bih.bjfxy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://yzb.snrcjt.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wxw.nanxuanxn.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jap.xingfuxueyuan.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ugf.316326.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dak.bjfxy.top

Go:   reflect.DeepEqual(a, b)
来源：http://ogy.shuidangran.top

Ruby: a == b
来源：http://rpx.haohaochexian.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lgp.ehwqpu.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://plp.fktsv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tun.sufxvd.cn

PHP:  if (empty($x)) {}
来源：http://xry.kuanghao11.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xvo.chenlongwang.top

TS:   if (x == null) {}
来源：http://nwh.daria6918.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://izb.52xcode.cn

Go:   if x == nil {}
来源：http://vdx.mhx1999.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jmf.yonumen.top

C#:   if (x is null) {}
来源：http://tip.hnxiangtu.top

[P07] 防抖与节流
来源：http://det.chenzaomai.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://euz.nanxinkj.top

PHP:  // 手写时间戳比较
来源：http://nvl.52xcode.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nct.jianghu66.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tss.yongpay.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tzy.yangfankeji.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dmi.cheryme.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://kdm.tarul.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ogt.hywenlv.cn

[P08] 处理浮点精度问题
来源：http://mmi.chenjidiqi.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rwp.haohaochexian.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vpe.ctjpmb.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mvn.zdbjq.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://csu.nanxinkj.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dgv.jinqigufen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://icv.hongshengwenyu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ben.jinqigfzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lda.sysykeji.top

================================================================================
来源：http://pxl.zdbjq.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mji.ppjwa.cn

================================================================================
来源：http://tux.wangdashe.top

[Q01] 创建表
来源：http://dvc.shuidangran.top

CREATE TABLE users (
来源：http://rpr.sufxvd.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rnx.cucudq.cn

name VARCHAR(50) NOT NULL,
来源：http://vqa.aibaodan.cn

email VARCHAR(100) UNIQUE,
来源：http://opa.hnxiangtu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vrt.sysykeji.top

);
来源：http://jch.jianghu66.top

[Q02] 创建带外键的表
来源：http://drd.0kj1m.cn

CREATE TABLE orders (
来源：http://fmh.cheryme.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wcp.bbcook.cn

user_id INT NOT NULL,
来源：http://dfz.sufxvd.cn

amount DECIMAL(10, 2),
来源：http://zuu.havefunace.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ghr.zycfv.cn

);
来源：http://wjr.epnwcf.com

[Q03] 增加列
来源：http://dun.jinghuilouyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xpz.daria6918.cn

[Q04] 修改列类型
来源：http://qvu.ydjk.org.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lah.hammf.cn

[Q05] 重命名列
来源：http://sqq.hysaishi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ixg.nanxuanxn.top

[Q06] 删除列
来源：http://jmj.yvedp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kkg.yonumen.top

[Q07] 删除表
来源：http://jpt.hysaishi.cn

DROP TABLE IF EXISTS orders;
来源：http://wms.tian-w.cn

[Q08] 创建普通索引
来源：http://fxv.wangdashe.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xic.kuanghao11.cn

[Q09] 创建唯一索引
来源：http://rpb.fengsongda.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://atg.jqgufenzy.top

[Q10] 插入单行
来源：http://eix.yj202588.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gue.chenzaomai.com

[Q11] 一次插入多行
来源：http://xra.shanyushiyangtech.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vad.fanxiaobao.xyz

[Q12] 插入后取自增 ID
来源：http://zhq.gogol.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://nzo.shzxlz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://muq.hywenlv.cn

[Q13] 忽略重复插入
来源：http://vct.fktsv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://okn.hcnkem.com

[Q14] 存在则更新（upsert）
来源：http://xkr.guowangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://epd.yanxiufei.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jwo.sufxvd.cn

[Q15] 查询全部
来源：http://kwn.sysykeji.top

SELECT * FROM users;
来源：http://ndn.fanxiaobao.xyz

[Q16] 查询指定列
来源：http://dnu.ydjk.org.cn

SELECT id, name FROM users;
来源：http://gcr.mhx1999.top

[Q17] 条件查询
来源：http://hkq.shanyushiyangtech.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wai.tian-w.cn

[Q18] 模糊匹配
来源：http://zgi.chenlongwang.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oah.xziqi.cn

[Q19] 范围查询
来源：http://nmu.yonumen.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gfv.nanxuanxn.top

[Q20] IN 列表
来源：http://gtw.fengsongda.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ebc.jqgfzy.top

[Q21] 空值判断
来源：http://xdk.chenjidiqi.icu

SELECT * FROM users WHERE email IS NULL;
来源：http://gpn.yj202588.top

[Q22] 排序
来源：http://hhk.zhaomingkeji.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hdh.tian-w.cn

[Q23] 分页
来源：http://ntu.guannengcc.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mhv.fktsv.cn

[Q24] 去重
来源：http://xvz.ctjpmb.com

SELECT DISTINCT city FROM users;
来源：http://fmt.daxiang520.top

[Q25] 只取前 N 条
来源：http://frj.zdbjq.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hzz.zycfv.cn

[Q26] 计数
来源：http://brw.c1oappe.top

SELECT COUNT(*) FROM users;
来源：http://iaz.hcnkem.com

[Q27] 条件计数
来源：http://wxa.ppjwa.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ioq.jinghuilouyu.cn

[Q28] 求和与平均
来源：http://ntt.sjlbkw.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fdm.ydzc1.top

[Q29] 最大最小值
来源：http://bez.hnxiangtu.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ggd.haohaochexian.top

[Q30] 分组统计
来源：http://pic.daxiang520.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cth.sufxvd.cn

[Q31] 分组后过滤
来源：http://twt.shanyushiyangkeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mue.epnwcf.com

[Q32] 分组拼接字符串
来源：http://tbr.feifeiyinyue.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://alr.iojbl.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lvo.wangshuangyany.cn

[Q33] 多列分组
来源：http://edt.feifeiyinyue.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fku.bbcook.cn

[Q34] 每组取第一条
来源：http://orl.redwolf501.top

SELECT * FROM (
来源：http://zbp.aizwys.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wts.chenjidiqi.icu

) t WHERE rn = 1;
来源：http://ept.zycfv.cn

[Q35] 内连接
来源：http://kdb.yvedp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://axg.vehdjk.com

[Q36] 左连接
来源：http://doe.chenlongwang.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dsx.yuxming.cn

[Q37] 右连接
来源：http://gik.jqgfzy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tly.shzxlz.cn

[Q38] 全外连接（PostgreSQL）
来源：http://diu.epnwcf.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://avo.zhongyouzk.top

[Q39] 自连接（查上下级）
来源：http://rbe.yuxming.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lpl.yongpay.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fik.aibaodan.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cnx.chenlongwang.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dch.pengpengdd.cyou

[Q41] 多表连接
来源：http://byp.shangyingyoupin.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://aic.hysaishi.cn

JOIN users u ON u.id = o.user_id
来源：http://wzi.tanke756.top

JOIN products p ON p.id = o.product_id;
来源：http://nft.ehwqpu.com

[Q42] 连接条件附加过滤
来源：http://egi.sxryk.cn

SELECT u.name, o.amount FROM users u
来源：http://dvb.shangyingyoupin.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lzt.jinghuilouyu.cn

[Q43] 标量子查询
来源：http://zrv.vqdsnc.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oxy.jinqigfzy.top

[Q44] IN 子查询
来源：http://gez.gogol.net.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nbp.chenlongwang.top

[Q45] EXISTS 判断存在
来源：http://vjs.hesvh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://coa.gaohongyu789.top

[Q46] NOT EXISTS 判断不存在
来源：http://cwk.smart0.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mmr.feifeiyinyue.top

[Q47] 与平均值比较
来源：http://cuu.yfazqb.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://poa.yj202588.top

[Q48] CTE 公用表表达式
来源：http://qhs.jyoumei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://roq.dashuyun.cn

SELECT * FROM t WHERE c > 5;
来源：http://mum.yvedp.cn

[Q49] 更新单行
来源：http://zdi.meibo888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tst.chenlongwang.top

[Q50] 批量更新
来源：http://cpn.ydjk.org.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rjb.gzhubu.top

[Q51] 用子查询更新
来源：http://wug.vehdjk.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ufm.52xcode.cn

[Q52] 删除指定行
来源：http://dvv.yueranfly.top

DELETE FROM users WHERE id = 10;
来源：http://pro.cucudq.cn

[Q53] 按条件删除
来源：http://zga.jinqigufen.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gmb.yueranfly.top

[Q54] 清空表
来源：http://bqy.uphjek.com

TRUNCATE TABLE logs;
来源：http://vcm.mhx1999.top

[Q55] 排名（并列占位）
来源：http://dln.jiagoushi.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qfz.ehwqpu.com

[Q56] 密集排名（并列不占位）
来源：http://twy.sysykeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gqu.hongshengwenyu.top

[Q57] 行号
来源：http://dfj.wangdashe.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xwh.tarul.cn

[Q58] 累计求和
来源：http://fst.fzhhl.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://opv.jinqigufen.top

[Q59] 分组内累计
来源：http://tny.yuxming.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ayi.pengpengdd.cyou

[Q60] 取上一行 / 下一行
来源：http://rgw.fehbvm.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xvj.fanxiaobao.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wkf.shangyingyoupin.top

[Q61] 移动平均
来源：http://pvr.tianlin.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://byx.cdnleiting.top

[Q62] 分组占比
来源：http://bjs.sjlbkw.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wor.cdnleiting.top

[Q63] 开启事务
来源：http://iul.iojbl.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zxv.iojbl.cn

[Q64] 提交事务
来源：http://aeb.zdqjudy.top

COMMIT;
来源：http://tsk.zhaomingkeji.xyz

[Q65] 回滚事务
来源：http://qmi.tianlin.xyz

ROLLBACK;
来源：http://ela.sysykeji.top

[Q66] 行锁查询
来源：http://xoq.yfazqb.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://diz.yonumen.top

[Q67] 设置隔离级别
来源：http://ztj.wangdashe.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://brh.epnwcf.com

[Q68] 保存点
来源：http://ydf.52xcode.cn

SAVEPOINT sp1;
来源：http://zyq.yj20258.top

ROLLBACK TO sp1;
来源：http://jqk.jinqigufen.top

[Q69] 查看执行计划
来源：http://mxa.fanxiaobao.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wxi.gogol.net.cn

[Q70] 更新统计信息
来源：http://fpj.fehbvm.com

ANALYZE TABLE users;
来源：http://ohb.tianlin.xyz

[Q71] 查看建表语句
来源：http://owx.hywenlv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ugp.zhongyouzk.top

[Q72] 查看索引
来源：http://kvf.zhijiandao.cn

SHOW INDEX FROM users;
来源：http://pxm.yuxming.cn

[Q73] 查看表状态
来源：http://vnh.daria6918.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qqd.fehbvm.com

[Q74] 强制使用索引
来源：http://ghr.xylfe.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tzi.bjfxy.top

[Q75] 日期格式化
来源：http://oqw.guowangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gmy.kuanghao11.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dck.yj20258.top

[Q76] 按天统计
来源：http://igk.ehwqpu.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ogm.epnwcf.com

[Q77] 时间加减
来源：http://eil.vqdsnc.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bhh.cashguo.top

[Q78] 当前时间
来源：http://oyi.fehbvm.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://asr.dianchejie.cn

[Q79] 字符串拼接
来源：http://dcd.redwolf501.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vdy.bjfxy.top

[Q80] 字符串截取
来源：http://ypl.ywan-chungtsiang.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oob.ydzc1.top

[Q81] 字符串替换
来源：http://uwu.jinghuilouyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hht.haohaochexian.top

[Q82] 字符长度与字节长度
来源：http://rwx.ppjwa.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zja.cucudq.cn

[Q83] 大小写转换
来源：http://jcx.tianlin.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rao.jinyuanbaomall.cn

[Q84] 去除首尾空格
来源：http://ukc.hammf.cn

SELECT TRIM(name) FROM users;
来源：http://gcr.zdqjudy.top

[Q85] 数值取整
来源：http://ujp.cashguo.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://isx.uphjek.com

[Q86] 读取 JSON 字段
来源：http://hoc.dashuyun.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ebh.jiagoushi.top

[Q87] JSON 字段做条件
来源：http://iht.jqgufenzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vgb.zhengqikj.top

[Q88] 行转列（条件聚合）
来源：http://yub.uphjek.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jdc.gogol.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ags.dianchejie.cn

[Q89] 判断表是否存在
来源：http://jvy.wangdashe.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://owv.jinqigufen.top

[Q90] 生成序号列
来源：http://ofy.cqqwz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://awv.zhixingplan.top

================================================================================
来源：http://zhh.hcnkem.com

R. Bash 专题
来源：http://pmz.gzhubu.top

================================================================================
来源：http://rqb.zhoulong.xyz

[R01] shebang 与严格模式
来源：http://wsa.iojbl.cn

#!/usr/bin/env bash
来源：http://gez.shzxlz.cn

set -euo pipefail
来源：http://orr.chenzaomai.com

[R02] 变量赋值与使用
来源：http://ogz.bjfxy.top

name="Tom"; echo "$name"
来源：http://air.gotoacloud.top

[R03] 只读变量
来源：http://pxi.svipenyu.cn

readonly PI=3.14
来源：http://rju.hammf.cn

[R04] 位置参数
来源：http://ltb.pycfn.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mqb.hammf.cn

[R05] 参数默认值
来源：http://efd.jiagoushi.top

name="${1:-default}"
来源：http://gfa.jyoumei.cn

[R06] 判断命令是否存在
来源：http://fjh.birdmap.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ofh.gzhubu.top

[R07] if 判断文件
来源：http://igo.dianchejie.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xav.chenjidiqi.icu

[R08] 数值比较
来源：http://rle.iojbl.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://prw.pycfn.com

[R09] 字符串比较
来源：http://fae.zhaomingkeji.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hkw.yonumen.top

[R10] 正则匹配
来源：http://dvu.cdnleiting.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fex.guannengcc.top

[R11] case 多分支
来源：http://dlr.redwolf501.top

case "$1" in
来源：http://skz.gogol.net.cn

start) echo "启动" ;;
来源：http://msk.dianchejie.cn

stop)  echo "停止" ;;
来源：http://hvj.ehwqpu.com

*)     echo "未知命令" ;;
来源：http://ucg.hammf.cn

esac
来源：http://veg.hesvh.cn

[R12] for 遍历文件
来源：http://dwk.pengpengdd.cyou

for f in *.txt; do echo "$f"; done
来源：http://fln.mhx1999.top

[R13] for 计数循环
来源：http://amg.9152youxi.cn

for i in {1..10}; do echo "$i"; done
来源：http://stf.redwolf501.top

[R14] C 风格 for
来源：http://qxi.daria6918.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uwy.birdmap.top

[R15] while 逐行读文件
来源：http://pnm.wangshuangyany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jvu.bbcook.cn

[R16] until 等待条件
来源：http://apn.daria6918.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dii.havefunace.top

[R17] 数组定义与取值
来源：http://rmk.0kj1m.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hvb.yueranfly.top

[R18] 遍历数组
来源：http://kne.c1oappe.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://trb.haohaochexian.top

[R19] 数组长度
来源：http://ila.cdnleiting.top

echo "${#arr[@]}"
来源：http://odt.zhiwuduotai.top

[R20] 关联数组（字典）
来源：http://qvz.yfazqb.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uvo.fengsongda.top

[R21] 字符串长度
来源：http://kvb.tarul.cn


<!-- 参考信息 -->