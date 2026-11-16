代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ech.chenzaomai.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qmg.sufxvd.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wsu.redwolf501.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kab.fzhhl.top

Java: list.size();  map.size();  s.length()
来源：http://bbv.bjfxy.top

Go:   len(arr);  len(m)
来源：http://kfk.yanxiufei.cn

Ruby: x.length;  x.size
来源：http://hor.zhaomingkeji.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://icu.meibo888.top

[P05] 判断两个对象内容是否相等
来源：http://xdq.chenlongwang.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://vqd.xuanzx.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lnt.zhiwuduotai.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://eor.yueranfly.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mhl.fehbvm.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nom.cucudq.cn

Go:   reflect.DeepEqual(a, b)
来源：http://etg.zdqjudy.top

Ruby: a == b
来源：http://vhb.kuanghao11.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ntn.ppjwa.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cee.xingfuxueyuan.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tze.aibaodan.cn

PHP:  if (empty($x)) {}
来源：http://obs.zhixingplan.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cuo.ydzc1.top

TS:   if (x == null) {}
来源：http://osu.yangfankeji.com

Java: if (x == null || x.isEmpty()) {}
来源：http://nzc.nwbrower.top

Go:   if x == nil {}
来源：http://nkn.cheryme.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://edw.xuanzx.com

C#:   if (x is null) {}
来源：http://rta.shzxlz.cn

[P07] 防抖与节流
来源：http://gdz.vehdjk.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://iog.gotoacloud.top

PHP:  // 手写时间戳比较
来源：http://mdu.uphjek.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jke.52xcode.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hew.shuidangran.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://llb.sjlbkw.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gns.jianghu66.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://tcg.xylfe.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mgt.xuanzx.com

[P08] 处理浮点精度问题
来源：http://nsn.ehwqpu.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ubl.wangshuangyany.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dyo.gotoacloud.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://plf.andypj.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://akx.shangyingyoupin.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mjg.nwbrower.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xzi.dianchejie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://iou.cashguo.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nkf.hnxiangtu.top

================================================================================
来源：http://mtd.yvedp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mqf.shzxlz.cn

================================================================================
来源：http://dwd.hesvh.cn

[Q01] 创建表
来源：http://wfi.zhongyouzk.top

CREATE TABLE users (
来源：http://odu.pengpengdd.cyou

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yhh.zhaomingkeji.xyz

name VARCHAR(50) NOT NULL,
来源：http://jir.epnwcf.com

email VARCHAR(100) UNIQUE,
来源：http://qdw.hywenlv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rqc.zdbjq.cn

);
来源：http://qqb.shzxlz.cn

[Q02] 创建带外键的表
来源：http://ggh.pengpengdd.cyou

CREATE TABLE orders (
来源：http://hda.nwbrower.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oar.pengpengdd.cyou

user_id INT NOT NULL,
来源：http://wst.gotoacloud.top

amount DECIMAL(10, 2),
来源：http://nyt.jiagoushi.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lie.nanxinkj.top

);
来源：http://hcq.xuanzx.com

[Q03] 增加列
来源：http://wsd.pycfn.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gqg.jqgufenzy.top

[Q04] 修改列类型
来源：http://uwe.yuanzhike.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vdn.jinqigufen.top

[Q05] 重命名列
来源：http://swf.smart0.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nhy.feifeiyinyue.top

[Q06] 删除列
来源：http://jpo.52xcode.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pqc.shuidangran.top

[Q07] 删除表
来源：http://yfk.yj202588.top

DROP TABLE IF EXISTS orders;
来源：http://lys.tarul.cn

[Q08] 创建普通索引
来源：http://szw.gotoacloud.top

CREATE INDEX idx_users_email ON users(email);
来源：http://udf.fktsv.cn

[Q09] 创建唯一索引
来源：http://uwj.guannengcc.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dri.52xcode.cn

[Q10] 插入单行
来源：http://wka.ydjk.org.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xzm.fehbvm.com

[Q11] 一次插入多行
来源：http://vkr.tianlin.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nmj.ydjk.org.cn

[Q12] 插入后取自增 ID
来源：http://bbl.jiagoushi.top

INSERT INTO users (name) VALUES ('C');
来源：http://aoq.yuanzhike.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rgw.nwbrower.top

[Q13] 忽略重复插入
来源：http://enn.aibaodan.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bob.uphjek.com

[Q14] 存在则更新（upsert）
来源：http://cvw.yanxiufei.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hhv.andypj.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gda.hywenlv.cn

[Q15] 查询全部
来源：http://vcg.yuanzhike.top

SELECT * FROM users;
来源：http://qrb.quarkkingdee.top

[Q16] 查询指定列
来源：http://dpd.daria6918.cn

SELECT id, name FROM users;
来源：http://gwf.zycfv.cn

[Q17] 条件查询
来源：http://hod.cdnleiting.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yex.havefunace.top

[Q18] 模糊匹配
来源：http://fcg.yueranfly.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nnm.sufxvd.cn

[Q19] 范围查询
来源：http://dtj.meibo888.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://seq.vqdsnc.cn

[Q20] IN 列表
来源：http://hrp.sweek.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vow.gotoacloud.top

[Q21] 空值判断
来源：http://ong.yuanzhike.top

SELECT * FROM users WHERE email IS NULL;
来源：http://tnn.jinqigufen.top

[Q22] 排序
来源：http://ggr.gogol.net.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wfe.yuanzhike.top

[Q23] 分页
来源：http://oof.vehdjk.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kgc.hammf.cn

[Q24] 去重
来源：http://aks.yuxming.cn

SELECT DISTINCT city FROM users;
来源：http://qpe.jqgufenzy.top

[Q25] 只取前 N 条
来源：http://kci.sufxvd.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pky.jianghu66.top

[Q26] 计数
来源：http://jqu.jyoumei.cn

SELECT COUNT(*) FROM users;
来源：http://jca.fehbvm.com

[Q27] 条件计数
来源：http://sza.vqdsnc.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rxv.haohaochexian.top

[Q28] 求和与平均
来源：http://jce.ctjpmb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://aid.yongpay.top

[Q29] 最大最小值
来源：http://pdj.pengpengdd.cyou

SELECT MAX(age), MIN(age) FROM users;
来源：http://tip.ehwqpu.com

[Q30] 分组统计
来源：http://ket.yuxming.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kbu.zycfv.cn

[Q31] 分组后过滤
来源：http://dmg.dashuyun.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hfc.nanxuanxn.top

[Q32] 分组拼接字符串
来源：http://ltf.zdqjudy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tqu.ctjpmb.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jfo.jianghu66.top

[Q33] 多列分组
来源：http://odr.ivvv.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gqa.zhaomingkeji.xyz

[Q34] 每组取第一条
来源：http://bgg.yanxiufei.cn

SELECT * FROM (
来源：http://cou.ydjk.org.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bfc.zhoulong.xyz

) t WHERE rn = 1;
来源：http://fnq.c1oappe.top

[Q35] 内连接
来源：http://urn.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dpj.haohaochexian.top

[Q36] 左连接
来源：http://zfk.yangfankeji.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ezp.hongshengwenyu.top

[Q37] 右连接
来源：http://dkp.0kj1m.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ddo.zhoulong.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://wjl.jinqigfzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ymx.xylfe.cn

[Q39] 自连接（查上下级）
来源：http://wzi.hcnkem.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://yrf.yj20258888.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wij.jinqigfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://imb.quarkkingdee.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dkc.yanxiufei.cn

[Q41] 多表连接
来源：http://pri.ivvv.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://hgl.gotoacloud.top

JOIN users u ON u.id = o.user_id
来源：http://ghm.sjlbkw.cn

JOIN products p ON p.id = o.product_id;
来源：http://acv.shuidangran.top

[Q42] 连接条件附加过滤
来源：http://fet.hcnkem.com

SELECT u.name, o.amount FROM users u
来源：http://zpm.quarkkingdee.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xcv.birdmap.top

[Q43] 标量子查询
来源：http://ftj.ydzc1.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mvt.nanxuanxn.top

[Q44] IN 子查询
来源：http://rmq.zhixingplan.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fea.vehdjk.com

[Q45] EXISTS 判断存在
来源：http://jjs.zhoulong.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oer.xuanzx.com

[Q46] NOT EXISTS 判断不存在
来源：http://hbf.meibo888.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fzj.ydzc1.top

[Q47] 与平均值比较
来源：http://xbg.nanxinkj.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://frm.vqdsnc.cn

[Q48] CTE 公用表表达式
来源：http://ekz.cqqwz.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jqu.tanke756.top

SELECT * FROM t WHERE c > 5;
来源：http://ehj.pengpengdd.cyou

[Q49] 更新单行
来源：http://nzq.gzhubu.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gbd.yuanzhike.top

[Q50] 批量更新
来源：http://hrk.zycfv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ose.wangdashe.top

[Q51] 用子查询更新
来源：http://cfg.xuetiantiany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cfe.pengpengdd.cyou

[Q52] 删除指定行
来源：http://qpn.gzhubu.top

DELETE FROM users WHERE id = 10;
来源：http://nkk.andypj.xyz

[Q53] 按条件删除
来源：http://mlj.ywan-chungtsiang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://noj.cqqwz.cn

[Q54] 清空表
来源：http://mlj.feifeiyinyue.top

TRUNCATE TABLE logs;
来源：http://kaq.zdqjudy.top

[Q55] 排名（并列占位）
来源：http://jsf.hywenlv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gml.shangyingyoupin.top

[Q56] 密集排名（并列不占位）
来源：http://nqn.andypj.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ika.dashuyun.cn

[Q57] 行号
来源：http://qka.quarkkingdee.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xms.ydzc1.top

[Q58] 累计求和
来源：http://csw.meibo888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ehz.xinyue.icu

[Q59] 分组内累计
来源：http://wnm.ivvv.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mxq.snrcjt.cn

[Q60] 取上一行 / 下一行
来源：http://vec.tarul.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://igi.jqgfzy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xln.zhoulong.xyz

[Q61] 移动平均
来源：http://asg.tarul.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mfi.guowangkeji.top

[Q62] 分组占比
来源：http://cbu.andypj.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nfz.sweek.top

[Q63] 开启事务
来源：http://xhf.guannengcc.top

START TRANSACTION;                -- 或 BEGIN
来源：http://rbx.hammf.cn

[Q64] 提交事务
来源：http://yhi.dianchejie.cn

COMMIT;
来源：http://uie.xylfe.cn

[Q65] 回滚事务
来源：http://pnc.aibaodan.cn

ROLLBACK;
来源：http://iow.daxiang520.top

[Q66] 行锁查询
来源：http://kfo.fzhhl.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pxw.aibaodan.cn

[Q67] 设置隔离级别
来源：http://pah.jlsjyb.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zxf.guowangkeji.top

[Q68] 保存点
来源：http://ipd.svipenyu.cn

SAVEPOINT sp1;
来源：http://jcz.pengpengdd.cyou

ROLLBACK TO sp1;
来源：http://fjf.pycfn.com

[Q69] 查看执行计划
来源：http://hvr.shanyushiyangkeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://twz.hesvh.cn

[Q70] 更新统计信息
来源：http://hbi.bjfxy.top

ANALYZE TABLE users;
来源：http://kvi.tian-w.cn

[Q71] 查看建表语句
来源：http://vbb.yj20258.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sri.andypj.xyz

[Q72] 查看索引
来源：http://cdj.sufxvd.cn

SHOW INDEX FROM users;
来源：http://ton.chenjidiqi.icu

[Q73] 查看表状态
来源：http://pfg.jlsjyb.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zba.ydzc1.top

[Q74] 强制使用索引
来源：http://beh.jqgufenzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jyr.hnqzz.top

[Q75] 日期格式化
来源：http://khd.xuetiantiany.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kyb.tian-w.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ffz.gzhubu.top

[Q76] 按天统计
来源：http://dng.yonumen.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qzn.shangyingyoupin.top

[Q77] 时间加减
来源：http://gvg.chenlongwang.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yyt.ydjk.org.cn

[Q78] 当前时间
来源：http://gyc.guannengcc.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ibu.yj202588.top

[Q79] 字符串拼接
来源：http://hct.hcnkem.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://eav.guowangkeji.top

[Q80] 字符串截取
来源：http://oom.sysykeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kjy.cheryme.top

[Q81] 字符串替换
来源：http://bek.ybcxt.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ice.yonumen.top

[Q82] 字符长度与字节长度
来源：http://xvs.ywan-chungtsiang.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dyo.dashuyun.cn

[Q83] 大小写转换
来源：http://nxu.pycfn.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kpl.iojbl.cn

[Q84] 去除首尾空格
来源：http://eus.xziqi.cn

SELECT TRIM(name) FROM users;
来源：http://hgs.ivvv.top

[Q85] 数值取整
来源：http://dnp.haohaochexian.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hgv.dashuyun.cn

[Q86] 读取 JSON 字段
来源：http://dge.jlsjyb.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ejj.yueranfly.top

[Q87] JSON 字段做条件
来源：http://uhl.fktsv.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://owy.jqgufenzy.top

[Q88] 行转列（条件聚合）
来源：http://spt.316326.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zrd.jlsjyb.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://abs.epnwcf.com

[Q89] 判断表是否存在
来源：http://zog.kuanghao11.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xsg.hfpthk.cn

[Q90] 生成序号列
来源：http://vza.shangyingyoupin.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ddq.hywenlv.cn

================================================================================
来源：http://mdr.sjlbkw.cn

R. Bash 专题
来源：http://ydh.jlsjyb.cn

================================================================================
来源：http://ffx.yonumen.top

[R01] shebang 与严格模式
来源：http://wno.dianchejie.cn

#!/usr/bin/env bash
来源：http://lnz.cucudq.cn

set -euo pipefail
来源：http://gil.yueranfly.top

[R02] 变量赋值与使用
来源：http://ril.zhoulong.xyz

name="Tom"; echo "$name"
来源：http://utx.gzhubu.top

[R03] 只读变量
来源：http://pfv.haohaochexian.top

readonly PI=3.14
来源：http://vge.hfpthk.cn

[R04] 位置参数
来源：http://axa.feifeiyinyue.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fzo.hywenlv.cn

[R05] 参数默认值
来源：http://nji.jqgufenzy.top

name="${1:-default}"
来源：http://qce.hammf.cn

[R06] 判断命令是否存在
来源：http://wth.svipenyu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hmx.nwbrower.top

[R07] if 判断文件
来源：http://jgg.fktsv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vld.bjfxy.top

[R08] 数值比较
来源：http://zmg.zhixingplan.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ttq.aizwys.cn

[R09] 字符串比较
来源：http://frr.ppjwa.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gvb.jinqigufen.top

[R10] 正则匹配
来源：http://qmd.wangshuangyany.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yun.yj20258888.top

[R11] case 多分支
来源：http://nyy.xziqi.cn

case "$1" in
来源：http://xlo.ctjpmb.com

start) echo "启动" ;;
来源：http://plt.hnxiangtu.top

stop)  echo "停止" ;;
来源：http://loi.tian-w.cn

*)     echo "未知命令" ;;
来源：http://stp.aizwys.cn

esac
来源：http://huv.xingfuxueyuan.xyz

[R12] for 遍历文件
来源：http://vsn.zdbjq.cn

for f in *.txt; do echo "$f"; done
来源：http://eyx.tarul.cn

[R13] for 计数循环
来源：http://nvr.epnwcf.com

for i in {1..10}; do echo "$i"; done
来源：http://njh.yanxiufei.cn

[R14] C 风格 for
来源：http://bbs.jiagoushi.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qib.aibaodan.cn

[R15] while 逐行读文件
来源：http://azt.yuanzhike.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://whl.xingfuxueyuan.xyz

[R16] until 等待条件
来源：http://sex.zdqjudy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tjg.fzhhl.top

[R17] 数组定义与取值
来源：http://mxm.hnqzz.top

arr=(a b c); echo "${arr[0]}"
来源：http://zhh.shanyushiyangkeji.top

[R18] 遍历数组
来源：http://hmv.fzhhl.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sbw.xinyue.icu

[R19] 数组长度
来源：http://hcf.jqgfzy.top

echo "${#arr[@]}"
来源：http://trm.daria6918.cn

[R20] 关联数组（字典）
来源：http://jti.ydjk.org.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vru.zdbjq.cn

[R21] 字符串长度
来源：http://nge.xylfe.cn


<!-- 参考信息 -->