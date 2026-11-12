代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://abr.nanxuanxn.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ngu.ydjk.org.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tqj.epnwcf.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kmy.xinyue.icu

Java: list.size();  map.size();  s.length()
来源：http://uwj.jinyuanbaomall.cn

Go:   len(arr);  len(m)
来源：http://ehg.jqgfzy.top

Ruby: x.length;  x.size
来源：http://ecl.zhengqikj.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://wyq.nanxuanxn.top

[P05] 判断两个对象内容是否相等
来源：http://qqj.xziqi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://mxs.zhongyouzk.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wak.meibo888.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uqk.cheryme.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gco.daria6918.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jpy.shzxlz.cn

Go:   reflect.DeepEqual(a, b)
来源：http://izy.yueranfly.top

Ruby: a == b
来源：http://vzr.yvedp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://igg.hysaishi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ona.quarkkingdee.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hhs.hnqzz.top

PHP:  if (empty($x)) {}
来源：http://jiz.zycfv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ceq.xuanzx.com

TS:   if (x == null) {}
来源：http://ixl.uphjek.com

Java: if (x == null || x.isEmpty()) {}
来源：http://acy.shanyushiyangkeji.top

Go:   if x == nil {}
来源：http://kkh.jlsjyb.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eor.aizwys.cn

C#:   if (x is null) {}
来源：http://fjt.havefunace.top

[P07] 防抖与节流
来源：http://eut.smart0.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gvr.jinqigfzy.top

PHP:  // 手写时间戳比较
来源：http://ptp.hongshengwenyu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ctv.cashguo.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vdz.cdnleiting.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zwt.zhoulong.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pnx.gogol.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hir.gotoacloud.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qes.guannengcc.top

[P08] 处理浮点精度问题
来源：http://fng.fehbvm.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vci.hnxiangtu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lkg.yangfankeji.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://aqi.mhx1999.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://anl.jinyuanbaomall.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cxs.wangshuangyany.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://liu.zhixingplan.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://enz.cheryme.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dmn.jqgufenzy.top

================================================================================
来源：http://nfx.shuidangran.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hhl.guannengcc.top

================================================================================
来源：http://hjp.tian-w.cn

[Q01] 创建表
来源：http://kss.zhaomingkeji.xyz

CREATE TABLE users (
来源：http://ocf.gotoacloud.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jsp.xziqi.cn

name VARCHAR(50) NOT NULL,
来源：http://dos.xinyue.icu

email VARCHAR(100) UNIQUE,
来源：http://njn.shanyushiyangtech.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lid.dianchejie.cn

);
来源：http://qln.guannengcc.top

[Q02] 创建带外键的表
来源：http://gzh.sysykeji.top

CREATE TABLE orders (
来源：http://ubs.sxryk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ffw.fktsv.cn

user_id INT NOT NULL,
来源：http://xvb.vqdsnc.cn

amount DECIMAL(10, 2),
来源：http://uzl.jinyuanbaomall.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kra.smart0.xyz

);
来源：http://cyc.52xcode.cn

[Q03] 增加列
来源：http://fje.zdqjudy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://agu.hfpthk.cn

[Q04] 修改列类型
来源：http://ugo.ydzc1.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cfo.jianghu66.top

[Q05] 重命名列
来源：http://jlh.haohaochexian.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://itn.fehbvm.com

[Q06] 删除列
来源：http://twx.yuanzhike.top

ALTER TABLE users DROP COLUMN age;
来源：http://mfy.gogol.net.cn

[Q07] 删除表
来源：http://emj.pycfn.com

DROP TABLE IF EXISTS orders;
来源：http://hcs.feifeiyinyue.top

[Q08] 创建普通索引
来源：http://hzd.andypj.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://cip.jyoumei.cn

[Q09] 创建唯一索引
来源：http://men.guowangkeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ehr.jiagoushi.top

[Q10] 插入单行
来源：http://cyw.xylfe.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xcm.jinyuanbaomall.cn

[Q11] 一次插入多行
来源：http://wqs.smart0.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xgj.zhiwuduotai.top

[Q12] 插入后取自增 ID
来源：http://ubt.havefunace.top

INSERT INTO users (name) VALUES ('C');
来源：http://oae.vehdjk.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tcu.cheryme.top

[Q13] 忽略重复插入
来源：http://kht.pycfn.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rqf.nanxuanxn.top

[Q14] 存在则更新（upsert）
来源：http://kzj.redwolf501.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dzo.hnqzz.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ich.iojbl.cn

[Q15] 查询全部
来源：http://bas.gzhubu.top

SELECT * FROM users;
来源：http://idw.zdbjq.cn

[Q16] 查询指定列
来源：http://wgf.smart0.xyz

SELECT id, name FROM users;
来源：http://zmx.yuxming.cn

[Q17] 条件查询
来源：http://lhd.tianlin.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lym.birdmap.top

[Q18] 模糊匹配
来源：http://udl.daria6918.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://glr.yj20258888.top

[Q19] 范围查询
来源：http://ekf.birdmap.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nkt.meibo888.top

[Q20] IN 列表
来源：http://xec.fengsongda.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://atz.daria6918.cn

[Q21] 空值判断
来源：http://aqr.hesvh.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qck.vqdsnc.cn

[Q22] 排序
来源：http://gml.andypj.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sia.sxryk.cn

[Q23] 分页
来源：http://cyd.cashguo.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hzn.chenzaomai.com

[Q24] 去重
来源：http://uif.yanxiufei.cn

SELECT DISTINCT city FROM users;
来源：http://ezh.shzxlz.cn

[Q25] 只取前 N 条
来源：http://kzo.yanxiufei.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://iqd.ybcxt.top

[Q26] 计数
来源：http://nmg.ppjwa.cn

SELECT COUNT(*) FROM users;
来源：http://gvc.cqqwz.cn

[Q27] 条件计数
来源：http://uln.hammf.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xmk.ybcxt.top

[Q28] 求和与平均
来源：http://crw.fanxiaobao.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://eat.smart0.xyz

[Q29] 最大最小值
来源：http://cuf.fehbvm.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://iia.dashuyun.cn

[Q30] 分组统计
来源：http://zuz.hfpthk.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jbv.pengpengdd.cyou

[Q31] 分组后过滤
来源：http://rrx.vehdjk.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://snl.jqgfzy.top

[Q32] 分组拼接字符串
来源：http://yxl.jqgfzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kya.havefunace.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gkg.andypj.xyz

[Q33] 多列分组
来源：http://qhw.jianghu66.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wyk.jinqigfzy.top

[Q34] 每组取第一条
来源：http://byz.hfpthk.cn

SELECT * FROM (
来源：http://wqw.hywenlv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sfy.aizwys.cn

) t WHERE rn = 1;
来源：http://lww.zhiwuduotai.top

[Q35] 内连接
来源：http://dlg.wangshuangyany.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://log.dashuyun.cn

[Q36] 左连接
来源：http://djl.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kwc.yj20258888.top

[Q37] 右连接
来源：http://wvc.wangdashe.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nqt.tanke756.top

[Q38] 全外连接（PostgreSQL）
来源：http://syv.ivvv.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://izn.xylfe.cn

[Q39] 自连接（查上下级）
来源：http://cwe.jyoumei.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://afr.gzhubu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yyt.jlsjyb.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ctp.daria6918.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dib.52xcode.cn

[Q41] 多表连接
来源：http://iaj.snrcjt.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ppc.gzhubu.top

JOIN users u ON u.id = o.user_id
来源：http://gff.wangshuangyany.cn

JOIN products p ON p.id = o.product_id;
来源：http://ukw.chenjidiqi.icu

[Q42] 连接条件附加过滤
来源：http://pec.yj202588.top

SELECT u.name, o.amount FROM users u
来源：http://dpx.c1oappe.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qaw.hnxiangtu.top

[Q43] 标量子查询
来源：http://plm.jinqigfzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qls.redwolf501.top

[Q44] IN 子查询
来源：http://lqd.wangdashe.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tkn.zhoulong.xyz

[Q45] EXISTS 判断存在
来源：http://qlf.316326.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hmk.gaohongyu789.top

[Q46] NOT EXISTS 判断不存在
来源：http://exc.ctjpmb.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vtz.zhixingplan.top

[Q47] 与平均值比较
来源：http://nce.ydzc1.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zhe.guowangkeji.top

[Q48] CTE 公用表表达式
来源：http://gbm.uphjek.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qdl.zdqjudy.top

SELECT * FROM t WHERE c > 5;
来源：http://vyf.bjfxy.top

[Q49] 更新单行
来源：http://oam.birdmap.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tre.c1oappe.top

[Q50] 批量更新
来源：http://lhx.epnwcf.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://piw.zdqjudy.top

[Q51] 用子查询更新
来源：http://ygm.redwolf501.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://izq.dianchejie.cn

[Q52] 删除指定行
来源：http://vpj.ehwqpu.com

DELETE FROM users WHERE id = 10;
来源：http://dcg.meibo888.top

[Q53] 按条件删除
来源：http://kvq.jinqigufen.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nmw.hongshengwenyu.top

[Q54] 清空表
来源：http://pcw.yonumen.top

TRUNCATE TABLE logs;
来源：http://zup.hongshengwenyu.top

[Q55] 排名（并列占位）
来源：http://lgk.jinqigufen.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://abb.fengsongda.top

[Q56] 密集排名（并列不占位）
来源：http://aiy.sweek.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fwj.yj20258.top

[Q57] 行号
来源：http://qhd.zycfv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qbf.tianlin.xyz

[Q58] 累计求和
来源：http://sln.yanxiufei.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ksl.ydjk.org.cn

[Q59] 分组内累计
来源：http://rms.xylfe.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xca.hammf.cn

[Q60] 取上一行 / 下一行
来源：http://ogs.jlsjyb.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lle.vqdsnc.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://maq.shanyushiyangkeji.top

[Q61] 移动平均
来源：http://npk.xziqi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pqv.zhaomingkeji.xyz

[Q62] 分组占比
来源：http://atu.pycfn.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jjb.xylfe.cn

[Q63] 开启事务
来源：http://bao.shuidangran.top

START TRANSACTION;                -- 或 BEGIN
来源：http://kes.jyoumei.cn

[Q64] 提交事务
来源：http://zxw.zhijiandao.cn

COMMIT;
来源：http://bmm.tarul.cn

[Q65] 回滚事务
来源：http://dno.tarul.cn

ROLLBACK;
来源：http://klg.nanxuanxn.top

[Q66] 行锁查询
来源：http://yui.jyoumei.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qcv.pengpengdd.cyou

[Q67] 设置隔离级别
来源：http://yzg.birdmap.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vvg.yueranfly.top

[Q68] 保存点
来源：http://yea.haohaochexian.top

SAVEPOINT sp1;
来源：http://jtw.bjfxy.top

ROLLBACK TO sp1;
来源：http://rwx.nwbrower.top

[Q69] 查看执行计划
来源：http://sil.jlsjyb.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yfo.fanxiaobao.xyz

[Q70] 更新统计信息
来源：http://trb.jinqigfzy.top

ANALYZE TABLE users;
来源：http://rca.ppjwa.cn

[Q71] 查看建表语句
来源：http://kxx.cucudq.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ovi.jiagoushi.top

[Q72] 查看索引
来源：http://lma.yj20258888.top

SHOW INDEX FROM users;
来源：http://seh.yfazqb.com

[Q73] 查看表状态
来源：http://bst.ybcxt.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rqt.wangshuangyany.cn

[Q74] 强制使用索引
来源：http://jib.nanxinkj.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://eyl.xingfuxueyuan.xyz

[Q75] 日期格式化
来源：http://dei.hammf.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://stl.yangfankeji.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qej.0kj1m.cn

[Q76] 按天统计
来源：http://dhw.hywenlv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://irb.dianchejie.cn

[Q77] 时间加减
来源：http://zme.daxiang520.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xhm.hywenlv.cn

[Q78] 当前时间
来源：http://mru.xinyue.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kiw.mhx1999.top

[Q79] 字符串拼接
来源：http://tvr.kuanghao11.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bws.hnqzz.top

[Q80] 字符串截取
来源：http://eby.ppjwa.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qis.jinyuanbaomall.cn

[Q81] 字符串替换
来源：http://ktl.hesvh.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kfr.cdnleiting.top

[Q82] 字符长度与字节长度
来源：http://oxq.ydzc1.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ctr.guowangkeji.top

[Q83] 大小写转换
来源：http://pdw.guowangkeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zbn.shanyushiyangtech.top

[Q84] 去除首尾空格
来源：http://ocs.ydzc1.top

SELECT TRIM(name) FROM users;
来源：http://tkh.daria6918.cn

[Q85] 数值取整
来源：http://vdv.hnxiangtu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://npx.yongpay.top

[Q86] 读取 JSON 字段
来源：http://fim.yongpay.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nwl.jinqigufen.top

[Q87] JSON 字段做条件
来源：http://xgd.ydzc1.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ldx.xziqi.cn

[Q88] 行转列（条件聚合）
来源：http://epz.guannengcc.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://poq.cqqwz.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ley.vqdsnc.cn

[Q89] 判断表是否存在
来源：http://yvc.sysykeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wqx.hnqzz.top

[Q90] 生成序号列
来源：http://khk.zdqjudy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nsk.yvedp.cn

================================================================================
来源：http://qzl.wangdashe.top

R. Bash 专题
来源：http://nca.yj20258.top

================================================================================
来源：http://siz.pengpengdd.cyou

[R01] shebang 与严格模式
来源：http://jel.cqqwz.cn

#!/usr/bin/env bash
来源：http://giz.quarkkingdee.top

set -euo pipefail
来源：http://znx.tianlin.xyz

[R02] 变量赋值与使用
来源：http://dbg.zhongyouzk.top

name="Tom"; echo "$name"
来源：http://rab.zhoulong.xyz

[R03] 只读变量
来源：http://ckh.ydjk.org.cn

readonly PI=3.14
来源：http://hgr.ehwqpu.com

[R04] 位置参数
来源：http://bhb.ydzc1.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://uqf.xylfe.cn

[R05] 参数默认值
来源：http://pig.shuidangran.top

name="${1:-default}"
来源：http://nik.bbcook.cn

[R06] 判断命令是否存在
来源：http://wpf.chenlongwang.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lec.yfazqb.com

[R07] if 判断文件
来源：http://cfx.sxryk.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://evx.haohaochexian.top

[R08] 数值比较
来源：http://cst.nwbrower.top

if (( a > b )); then echo "a 更大"; fi
来源：http://wdz.jqgufenzy.top

[R09] 字符串比较
来源：http://tit.shangyingyoupin.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uxc.ybcxt.top

[R10] 正则匹配
来源：http://jwk.zhiwuduotai.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jis.cdnleiting.top

[R11] case 多分支
来源：http://aqw.tarul.cn

case "$1" in
来源：http://otl.xylfe.cn

start) echo "启动" ;;
来源：http://cjs.0kj1m.cn

stop)  echo "停止" ;;
来源：http://qxu.jianghu66.top

*)     echo "未知命令" ;;
来源：http://hkj.yongpay.top

esac
来源：http://vkj.shzxlz.cn

[R12] for 遍历文件
来源：http://kfo.fehbvm.com

for f in *.txt; do echo "$f"; done
来源：http://vnj.xinyue.icu

[R13] for 计数循环
来源：http://fok.jqgufenzy.top

for i in {1..10}; do echo "$i"; done
来源：http://luy.ctjpmb.com

[R14] C 风格 for
来源：http://nsn.hnxiangtu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://omc.hcnkem.com

[R15] while 逐行读文件
来源：http://mmp.sysykeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qlm.shanyushiyangkeji.top

[R16] until 等待条件
来源：http://erl.tarul.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ull.jinqigufen.top

[R17] 数组定义与取值
来源：http://nva.pycfn.com

arr=(a b c); echo "${arr[0]}"
来源：http://uqo.daxiang520.top

[R18] 遍历数组
来源：http://dec.tanke756.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://yqh.epnwcf.com

[R19] 数组长度
来源：http://ctl.pengpengdd.cyou

echo "${#arr[@]}"
来源：http://ycy.meibo888.top

[R20] 关联数组（字典）
来源：http://sim.sjlbkw.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mjr.jinyuanbaomall.cn

[R21] 字符串长度
来源：http://vtu.gaohongyu789.top


<!-- 参考信息 -->