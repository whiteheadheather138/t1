代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://teu.vehdjk.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://clu.quarkkingdee.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wkz.hfpthk.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qdl.tianlin.xyz

Java: list.size();  map.size();  s.length()
来源：http://xva.tanke756.top

Go:   len(arr);  len(m)
来源：http://yxr.ydzc1.top

Ruby: x.length;  x.size
来源：http://cfj.hfpthk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bkv.cucudq.cn

[P05] 判断两个对象内容是否相等
来源：http://byx.uphjek.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://fdl.jinghuilouyu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lle.bbcook.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hxf.iojbl.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rlc.hcnkem.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tly.tanke756.top

Go:   reflect.DeepEqual(a, b)
来源：http://btr.ctjpmb.com

Ruby: a == b
来源：http://txv.ydjk.org.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bzi.guannengcc.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nmm.havefunace.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gdf.yj20258.top

PHP:  if (empty($x)) {}
来源：http://bpl.jlsjyb.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kxd.sweek.top

TS:   if (x == null) {}
来源：http://mji.ybcxt.top

Java: if (x == null || x.isEmpty()) {}
来源：http://cns.birdmap.top

Go:   if x == nil {}
来源：http://efv.sufxvd.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zzy.jinqigufen.top

C#:   if (x is null) {}
来源：http://pbl.svipenyu.cn

[P07] 防抖与节流
来源：http://ixx.birdmap.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://idq.birdmap.top

PHP:  // 手写时间戳比较
来源：http://ctu.yuxming.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fkf.yonumen.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zrj.yueranfly.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nzr.tarul.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lxv.fzhhl.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://isv.feifeiyinyue.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uyq.yueranfly.top

[P08] 处理浮点精度问题
来源：http://ges.yonumen.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://car.aizwys.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pmi.tianlin.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://avw.fanxiaobao.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yjv.fanxiaobao.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ivj.yuxming.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kdm.snrcjt.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yzz.uphjek.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ysx.ehwqpu.com

================================================================================
来源：http://ebz.gzhubu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zyu.yvedp.cn

================================================================================
来源：http://map.pycfn.com

[Q01] 创建表
来源：http://qhx.andypj.xyz

CREATE TABLE users (
来源：http://tyk.hcnkem.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jof.zdqjudy.top

name VARCHAR(50) NOT NULL,
来源：http://xny.bjfxy.top

email VARCHAR(100) UNIQUE,
来源：http://fvt.fzhhl.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sxu.yj202588.top

);
来源：http://sky.fengsongda.top

[Q02] 创建带外键的表
来源：http://ypf.shanyushiyangtech.top

CREATE TABLE orders (
来源：http://tyl.hywenlv.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://emj.xingfuxueyuan.xyz

user_id INT NOT NULL,
来源：http://neb.bbcook.cn

amount DECIMAL(10, 2),
来源：http://qch.chenzaomai.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uil.cheryme.top

);
来源：http://zvy.yonumen.top

[Q03] 增加列
来源：http://ofo.cdnleiting.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pao.cdnleiting.top

[Q04] 修改列类型
来源：http://pxy.hnqzz.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bmb.yuanzhike.top

[Q05] 重命名列
来源：http://jqz.zhijiandao.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://acy.hysaishi.cn

[Q06] 删除列
来源：http://esi.yj202588.top

ALTER TABLE users DROP COLUMN age;
来源：http://ugp.xuetiantiany.cn

[Q07] 删除表
来源：http://str.sxryk.cn

DROP TABLE IF EXISTS orders;
来源：http://nxs.hnqzz.top

[Q08] 创建普通索引
来源：http://rai.fanxiaobao.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://gts.sweek.top

[Q09] 创建唯一索引
来源：http://nci.tanke756.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tud.zhijiandao.cn

[Q10] 插入单行
来源：http://gfn.c1oappe.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jdu.dashuyun.cn

[Q11] 一次插入多行
来源：http://roh.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qiw.yongpay.top

[Q12] 插入后取自增 ID
来源：http://uem.epnwcf.com

INSERT INTO users (name) VALUES ('C');
来源：http://ixl.zdqjudy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xim.vqdsnc.cn

[Q13] 忽略重复插入
来源：http://tux.ehwqpu.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hdn.pengpengdd.cyou

[Q14] 存在则更新（upsert）
来源：http://mpo.shanyushiyangtech.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ked.epnwcf.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lew.xuanzx.com

[Q15] 查询全部
来源：http://mmj.hywenlv.cn

SELECT * FROM users;
来源：http://ysx.ybcxt.top

[Q16] 查询指定列
来源：http://djn.cqqwz.cn

SELECT id, name FROM users;
来源：http://hoz.zhiwuduotai.top

[Q17] 条件查询
来源：http://she.xuanzx.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fir.bjfxy.top

[Q18] 模糊匹配
来源：http://auv.jqgfzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qcj.jinqigufen.top

[Q19] 范围查询
来源：http://plb.xingfuxueyuan.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vqk.zhixingplan.top

[Q20] IN 列表
来源：http://hls.ybcxt.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ims.shuidangran.top

[Q21] 空值判断
来源：http://woj.ppjwa.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://plp.shzxlz.cn

[Q22] 排序
来源：http://oar.hongshengwenyu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vmp.316326.xyz

[Q23] 分页
来源：http://myn.yvedp.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zvv.hesvh.cn

[Q24] 去重
来源：http://uol.guannengcc.top

SELECT DISTINCT city FROM users;
来源：http://anl.haohaochexian.top

[Q25] 只取前 N 条
来源：http://ppq.cqqwz.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yni.shanyushiyangkeji.top

[Q26] 计数
来源：http://dym.dashuyun.cn

SELECT COUNT(*) FROM users;
来源：http://ueu.yj202588.top

[Q27] 条件计数
来源：http://dqi.zdqjudy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://azg.sxryk.cn

[Q28] 求和与平均
来源：http://xic.xuetiantiany.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://goq.zhixingplan.top

[Q29] 最大最小值
来源：http://uen.hysaishi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ovo.9152youxi.cn

[Q30] 分组统计
来源：http://tgu.feifeiyinyue.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hzk.0kj1m.cn

[Q31] 分组后过滤
来源：http://jqi.meibo888.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jhx.chenlongwang.top

[Q32] 分组拼接字符串
来源：http://how.fzhhl.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tkd.hysaishi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gws.tarul.cn

[Q33] 多列分组
来源：http://hux.hammf.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hvh.zdbjq.cn

[Q34] 每组取第一条
来源：http://dit.c1oappe.top

SELECT * FROM (
来源：http://jty.jiagoushi.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qni.kuanghao11.cn

) t WHERE rn = 1;
来源：http://jct.guowangkeji.top

[Q35] 内连接
来源：http://zfk.zdqjudy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hom.dianchejie.cn

[Q36] 左连接
来源：http://npm.c1oappe.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kwu.cucudq.cn

[Q37] 右连接
来源：http://lio.fehbvm.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bhm.aibaodan.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xol.bbcook.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://toc.feifeiyinyue.top

[Q39] 自连接（查上下级）
来源：http://hue.jinqigufen.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://wlt.hywenlv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hmu.zhoulong.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://goz.316326.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ptg.xingfuxueyuan.xyz

[Q41] 多表连接
来源：http://chf.sxryk.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qvu.xylfe.cn

JOIN users u ON u.id = o.user_id
来源：http://rrq.yj20258.top

JOIN products p ON p.id = o.product_id;
来源：http://oly.aizwys.cn

[Q42] 连接条件附加过滤
来源：http://kzd.cqqwz.cn

SELECT u.name, o.amount FROM users u
来源：http://lwg.zhengqikj.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gcr.cheryme.top

[Q43] 标量子查询
来源：http://duz.hnqzz.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://thl.hysaishi.cn

[Q44] IN 子查询
来源：http://mfd.sjlbkw.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yal.hywenlv.cn

[Q45] EXISTS 判断存在
来源：http://xix.iojbl.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sny.52xcode.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ktv.hongshengwenyu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uvq.jyoumei.cn

[Q47] 与平均值比较
来源：http://gtu.jinyuanbaomall.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lbj.meibo888.top

[Q48] CTE 公用表表达式
来源：http://fyt.cashguo.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mci.zhiwuduotai.top

SELECT * FROM t WHERE c > 5;
来源：http://dqx.yj202588.top

[Q49] 更新单行
来源：http://bgb.zdqjudy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zgt.jlsjyb.cn

[Q50] 批量更新
来源：http://tev.gotoacloud.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gof.vehdjk.com

[Q51] 用子查询更新
来源：http://zlw.xylfe.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://njy.zhoulong.xyz

[Q52] 删除指定行
来源：http://vdm.redwolf501.top

DELETE FROM users WHERE id = 10;
来源：http://otm.hfpthk.cn

[Q53] 按条件删除
来源：http://lns.yj20258888.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jrx.iojbl.cn

[Q54] 清空表
来源：http://akn.cdnleiting.top

TRUNCATE TABLE logs;
来源：http://zie.quarkkingdee.top

[Q55] 排名（并列占位）
来源：http://tfm.chenzaomai.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kql.jqgfzy.top

[Q56] 密集排名（并列不占位）
来源：http://cst.zdbjq.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ncb.jianghu66.top

[Q57] 行号
来源：http://ocu.hywenlv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ifn.316326.xyz

[Q58] 累计求和
来源：http://irb.ydjk.org.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pzo.tarul.cn

[Q59] 分组内累计
来源：http://fvk.yj20258888.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wtx.ybcxt.top

[Q60] 取上一行 / 下一行
来源：http://ohl.sxryk.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ovn.ybcxt.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tdy.svipenyu.cn

[Q61] 移动平均
来源：http://bab.shuidangran.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://agv.wangdashe.top

[Q62] 分组占比
来源：http://xei.birdmap.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fsr.nwbrower.top

[Q63] 开启事务
来源：http://hud.zhixingplan.top

START TRANSACTION;                -- 或 BEGIN
来源：http://lqc.yj20258.top

[Q64] 提交事务
来源：http://nle.zdqjudy.top

COMMIT;
来源：http://hts.guowangkeji.top

[Q65] 回滚事务
来源：http://sdo.jianghu66.top

ROLLBACK;
来源：http://swj.uphjek.com

[Q66] 行锁查询
来源：http://cob.zhiwuduotai.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rqr.hesvh.cn

[Q67] 设置隔离级别
来源：http://jmj.vqdsnc.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oiw.havefunace.top

[Q68] 保存点
来源：http://kax.zhengqikj.top

SAVEPOINT sp1;
来源：http://tsc.zhoulong.xyz

ROLLBACK TO sp1;
来源：http://xgy.aizwys.cn

[Q69] 查看执行计划
来源：http://ukk.nwbrower.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pgj.kuanghao11.cn

[Q70] 更新统计信息
来源：http://azs.hesvh.cn

ANALYZE TABLE users;
来源：http://bye.cheryme.top

[Q71] 查看建表语句
来源：http://izr.fanxiaobao.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mwo.tarul.cn

[Q72] 查看索引
来源：http://adc.zhaomingkeji.xyz

SHOW INDEX FROM users;
来源：http://vut.sysykeji.top

[Q73] 查看表状态
来源：http://xmb.yonumen.top

SHOW TABLE STATUS LIKE 'users';
来源：http://zka.guowangkeji.top

[Q74] 强制使用索引
来源：http://rzm.zhijiandao.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://heo.fanxiaobao.xyz

[Q75] 日期格式化
来源：http://bui.aibaodan.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pmm.sweek.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sbz.jyoumei.cn

[Q76] 按天统计
来源：http://mfx.meibo888.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://muc.vehdjk.com

[Q77] 时间加减
来源：http://pci.hywenlv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zug.jiagoushi.top

[Q78] 当前时间
来源：http://kvp.xziqi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pdh.nanxuanxn.top

[Q79] 字符串拼接
来源：http://vkt.tian-w.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hwv.smart0.xyz

[Q80] 字符串截取
来源：http://aba.cqqwz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qdc.yonumen.top

[Q81] 字符串替换
来源：http://xue.ehwqpu.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tfh.nanxinkj.top

[Q82] 字符长度与字节长度
来源：http://lsw.aizwys.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vwh.birdmap.top

[Q83] 大小写转换
来源：http://cwm.yueranfly.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sjb.wangdashe.top

[Q84] 去除首尾空格
来源：http://njj.wangshuangyany.cn

SELECT TRIM(name) FROM users;
来源：http://zug.cashguo.top

[Q85] 数值取整
来源：http://hoe.0kj1m.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zsc.yonumen.top

[Q86] 读取 JSON 字段
来源：http://rdv.tianlin.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qtb.xziqi.cn

[Q87] JSON 字段做条件
来源：http://dwc.quarkkingdee.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jqm.zhoulong.xyz

[Q88] 行转列（条件聚合）
来源：http://zni.aibaodan.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nuw.nanxinkj.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lyj.bbcook.cn

[Q89] 判断表是否存在
来源：http://uww.yuanzhike.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://oev.pengpengdd.cyou

[Q90] 生成序号列
来源：http://mjg.tarul.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xxp.cqqwz.cn

================================================================================
来源：http://cyc.nwbrower.top

R. Bash 专题
来源：http://mtn.gogol.net.cn

================================================================================
来源：http://tuw.shanyushiyangkeji.top

[R01] shebang 与严格模式
来源：http://htx.tanke756.top

#!/usr/bin/env bash
来源：http://gek.cashguo.top

set -euo pipefail
来源：http://ueq.gaohongyu789.top

[R02] 变量赋值与使用
来源：http://dvw.wangshuangyany.cn

name="Tom"; echo "$name"
来源：http://kvy.chenlongwang.top

[R03] 只读变量
来源：http://agj.birdmap.top

readonly PI=3.14
来源：http://vab.snrcjt.cn

[R04] 位置参数
来源：http://jhw.ydjk.org.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gbe.yangfankeji.com

[R05] 参数默认值
来源：http://sfl.jianghu66.top

name="${1:-default}"
来源：http://brk.yueranfly.top

[R06] 判断命令是否存在
来源：http://gru.yanxiufei.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://spi.zhixingplan.top

[R07] if 判断文件
来源：http://odg.sufxvd.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hik.shzxlz.cn

[R08] 数值比较
来源：http://wxn.tianlin.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://juq.gotoacloud.top

[R09] 字符串比较
来源：http://zcp.wangdashe.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jwm.fktsv.cn

[R10] 正则匹配
来源：http://lqs.gaohongyu789.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://big.shuidangran.top

[R11] case 多分支
来源：http://rfu.shzxlz.cn

case "$1" in
来源：http://kxm.hcnkem.com

start) echo "启动" ;;
来源：http://tqm.quarkkingdee.top

stop)  echo "停止" ;;
来源：http://wlh.yangfankeji.com

*)     echo "未知命令" ;;
来源：http://hss.wangdashe.top

esac
来源：http://swn.hesvh.cn

[R12] for 遍历文件
来源：http://swk.fengsongda.top

for f in *.txt; do echo "$f"; done
来源：http://yau.svipenyu.cn

[R13] for 计数循环
来源：http://alb.guannengcc.top

for i in {1..10}; do echo "$i"; done
来源：http://dku.fehbvm.com

[R14] C 风格 for
来源：http://vjz.gotoacloud.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ztq.uphjek.com

[R15] while 逐行读文件
来源：http://owb.yongpay.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sxp.cashguo.top

[R16] until 等待条件
来源：http://ikl.shanyushiyangtech.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rvo.yfazqb.com

[R17] 数组定义与取值
来源：http://ppr.ywan-chungtsiang.top

arr=(a b c); echo "${arr[0]}"
来源：http://ulc.cashguo.top

[R18] 遍历数组
来源：http://hwk.yongpay.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jwx.dashuyun.cn

[R19] 数组长度
来源：http://vbd.jinqigufen.top

echo "${#arr[@]}"
来源：http://jwg.yueranfly.top

[R20] 关联数组（字典）
来源：http://acc.gaohongyu789.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cze.sufxvd.cn

[R21] 字符串长度
来源：http://glh.fktsv.cn


<!-- 参考信息 -->