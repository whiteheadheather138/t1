代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uet.meibo888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ddv.fktsv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://msd.xingfuxueyuan.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zmn.hesvh.cn

Java: list.size();  map.size();  s.length()
来源：http://jtv.shanyushiyangtech.top

Go:   len(arr);  len(m)
来源：http://ilm.xziqi.cn

Ruby: x.length;  x.size
来源：http://gvg.ywan-chungtsiang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zgt.zhengqikj.top

[P05] 判断两个对象内容是否相等
来源：http://qye.sysykeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://itk.quarkkingdee.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ute.xingfuxueyuan.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ona.jyoumei.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eco.quarkkingdee.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ryu.tianlin.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://tnk.c1oappe.top

Ruby: a == b
来源：http://one.ybcxt.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yar.jqgufenzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ncy.hnqzz.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uwo.mhx1999.top

PHP:  if (empty($x)) {}
来源：http://iak.cqqwz.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://biv.hammf.cn

TS:   if (x == null) {}
来源：http://equ.yangfankeji.com

Java: if (x == null || x.isEmpty()) {}
来源：http://rhb.sxryk.cn

Go:   if x == nil {}
来源：http://ckx.yj20258.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://aow.gotoacloud.top

C#:   if (x is null) {}
来源：http://qby.yangfankeji.com

[P07] 防抖与节流
来源：http://epe.xingfuxueyuan.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://aza.wangdashe.top

PHP:  // 手写时间戳比较
来源：http://zam.hammf.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ikz.sweek.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ipz.shuidangran.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tbj.jyoumei.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bec.yuxming.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://jxo.tianlin.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dyo.xziqi.cn

[P08] 处理浮点精度问题
来源：http://lxp.redwolf501.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ubw.xinyue.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://whu.jqgfzy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://eoj.tian-w.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sft.dianchejie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zdv.aibaodan.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ziz.hywenlv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ecc.jiagoushi.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yrt.havefunace.top

================================================================================
来源：http://fyq.hongshengwenyu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://okh.ydzc1.top

================================================================================
来源：http://yrj.gzhubu.top

[Q01] 创建表
来源：http://pnf.jyoumei.cn

CREATE TABLE users (
来源：http://ukk.feifeiyinyue.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ktg.zhixingplan.top

name VARCHAR(50) NOT NULL,
来源：http://zcm.uphjek.com

email VARCHAR(100) UNIQUE,
来源：http://fab.quarkkingdee.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fuq.gaohongyu789.top

);
来源：http://sxg.guowangkeji.top

[Q02] 创建带外键的表
来源：http://fbh.jinqigufen.top

CREATE TABLE orders (
来源：http://owz.zhoulong.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eso.fzhhl.top

user_id INT NOT NULL,
来源：http://yhh.zhixingplan.top

amount DECIMAL(10, 2),
来源：http://hdt.guowangkeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zse.bbcook.cn

);
来源：http://ukw.daria6918.cn

[Q03] 增加列
来源：http://inm.daria6918.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://njs.hnqzz.top

[Q04] 修改列类型
来源：http://afm.gaohongyu789.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ipn.smart0.xyz

[Q05] 重命名列
来源：http://deg.cucudq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rws.tianlin.xyz

[Q06] 删除列
来源：http://oae.hnxiangtu.top

ALTER TABLE users DROP COLUMN age;
来源：http://qlo.52xcode.cn

[Q07] 删除表
来源：http://vgt.quarkkingdee.top

DROP TABLE IF EXISTS orders;
来源：http://xdw.gaohongyu789.top

[Q08] 创建普通索引
来源：http://cyk.smart0.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://jkt.bbcook.cn

[Q09] 创建唯一索引
来源：http://ogs.ywan-chungtsiang.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://isp.gaohongyu789.top

[Q10] 插入单行
来源：http://hfw.guannengcc.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ibb.ydzc1.top

[Q11] 一次插入多行
来源：http://glg.cheryme.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nkd.gogol.net.cn

[Q12] 插入后取自增 ID
来源：http://puh.ppjwa.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xog.jqgufenzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jml.hnxiangtu.top

[Q13] 忽略重复插入
来源：http://sjo.cheryme.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ksp.xziqi.cn

[Q14] 存在则更新（upsert）
来源：http://fqu.zhoulong.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://snw.jiagoushi.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wyl.hesvh.cn

[Q15] 查询全部
来源：http://vuz.xinyue.icu

SELECT * FROM users;
来源：http://gca.smart0.xyz

[Q16] 查询指定列
来源：http://cbu.sufxvd.cn

SELECT id, name FROM users;
来源：http://ogn.jinqigfzy.top

[Q17] 条件查询
来源：http://zvx.daria6918.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://esf.aibaodan.cn

[Q18] 模糊匹配
来源：http://kmi.yuxming.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://utu.guannengcc.top

[Q19] 范围查询
来源：http://ydp.sxryk.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rji.smart0.xyz

[Q20] IN 列表
来源：http://oju.nwbrower.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://amj.pengpengdd.cyou

[Q21] 空值判断
来源：http://wex.zhijiandao.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dny.tanke756.top

[Q22] 排序
来源：http://hth.52xcode.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bdt.pengpengdd.cyou

[Q23] 分页
来源：http://jdr.jiagoushi.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mew.hesvh.cn

[Q24] 去重
来源：http://beu.ehwqpu.com

SELECT DISTINCT city FROM users;
来源：http://tsq.jiagoushi.top

[Q25] 只取前 N 条
来源：http://ojp.zdqjudy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xda.feifeiyinyue.top

[Q26] 计数
来源：http://lka.yuanzhike.top

SELECT COUNT(*) FROM users;
来源：http://oxl.zycfv.cn

[Q27] 条件计数
来源：http://qeg.redwolf501.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hrh.sufxvd.cn

[Q28] 求和与平均
来源：http://vpq.chenlongwang.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ahy.ehwqpu.com

[Q29] 最大最小值
来源：http://nlu.tian-w.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ejk.52xcode.cn

[Q30] 分组统计
来源：http://coj.svipenyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://oxu.shanyushiyangtech.top

[Q31] 分组后过滤
来源：http://izu.ehwqpu.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gkg.xuanzx.com

[Q32] 分组拼接字符串
来源：http://ooh.nwbrower.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jvr.ctjpmb.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://siv.jyoumei.cn

[Q33] 多列分组
来源：http://vwq.fengsongda.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jak.wangdashe.top

[Q34] 每组取第一条
来源：http://lpu.dashuyun.cn

SELECT * FROM (
来源：http://mfp.fktsv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vcv.0kj1m.cn

) t WHERE rn = 1;
来源：http://xqh.zhiwuduotai.top

[Q35] 内连接
来源：http://sut.yongpay.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rop.yj202588.top

[Q36] 左连接
来源：http://oos.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://igr.daria6918.cn

[Q37] 右连接
来源：http://hzk.cashguo.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://plm.iojbl.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ole.sxryk.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gbd.chenzaomai.com

[Q39] 自连接（查上下级）
来源：http://pgs.zhijiandao.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vea.ywan-chungtsiang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jvd.c1oappe.top

[Q40] 交叉连接（笛卡尔积）
来源：http://fpm.sweek.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oya.hywenlv.cn

[Q41] 多表连接
来源：http://odl.jinyuanbaomall.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://iux.xylfe.cn

JOIN users u ON u.id = o.user_id
来源：http://yju.hcnkem.com

JOIN products p ON p.id = o.product_id;
来源：http://wqk.aibaodan.cn

[Q42] 连接条件附加过滤
来源：http://heh.ehwqpu.com

SELECT u.name, o.amount FROM users u
来源：http://qvn.yuanzhike.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xqz.sjlbkw.cn

[Q43] 标量子查询
来源：http://ktk.svipenyu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://una.sxryk.cn

[Q44] IN 子查询
来源：http://rnp.hywenlv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hvu.vehdjk.com

[Q45] EXISTS 判断存在
来源：http://hnl.cucudq.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nug.shangyingyoupin.top

[Q46] NOT EXISTS 判断不存在
来源：http://exn.cheryme.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qwr.iojbl.cn

[Q47] 与平均值比较
来源：http://aqr.fengsongda.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bhe.0kj1m.cn

[Q48] CTE 公用表表达式
来源：http://oab.gogol.net.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://luu.jqgfzy.top

SELECT * FROM t WHERE c > 5;
来源：http://xdd.ybcxt.top

[Q49] 更新单行
来源：http://mdz.hysaishi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://prp.haohaochexian.top

[Q50] 批量更新
来源：http://fjk.meibo888.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://eiu.haohaochexian.top

[Q51] 用子查询更新
来源：http://wph.bbcook.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cwg.c1oappe.top

[Q52] 删除指定行
来源：http://dfe.hesvh.cn

DELETE FROM users WHERE id = 10;
来源：http://wwz.redwolf501.top

[Q53] 按条件删除
来源：http://bdr.dianchejie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ybr.cqqwz.cn

[Q54] 清空表
来源：http://ryg.xingfuxueyuan.xyz

TRUNCATE TABLE logs;
来源：http://sfq.zhixingplan.top

[Q55] 排名（并列占位）
来源：http://wrk.ivvv.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xwr.gzhubu.top

[Q56] 密集排名（并列不占位）
来源：http://rui.yanxiufei.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dow.jlsjyb.cn

[Q57] 行号
来源：http://tlz.redwolf501.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xxe.fehbvm.com

[Q58] 累计求和
来源：http://gpg.dianchejie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ocv.ydzc1.top

[Q59] 分组内累计
来源：http://tlu.wangdashe.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ohg.fktsv.cn

[Q60] 取上一行 / 下一行
来源：http://ppd.hfpthk.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yqa.vqdsnc.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yws.shanyushiyangtech.top

[Q61] 移动平均
来源：http://jjn.0kj1m.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://miu.gogol.net.cn

[Q62] 分组占比
来源：http://pns.yj20258.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tiv.yuanzhike.top

[Q63] 开启事务
来源：http://nhk.hnxiangtu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://oys.hfpthk.cn

[Q64] 提交事务
来源：http://kir.daria6918.cn

COMMIT;
来源：http://zsd.epnwcf.com

[Q65] 回滚事务
来源：http://bdf.daria6918.cn

ROLLBACK;
来源：http://vez.gogol.net.cn

[Q66] 行锁查询
来源：http://xbo.bjfxy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sio.andypj.xyz

[Q67] 设置隔离级别
来源：http://zfg.dianchejie.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qcz.yuanzhike.top

[Q68] 保存点
来源：http://bto.bjfxy.top

SAVEPOINT sp1;
来源：http://sot.feifeiyinyue.top

ROLLBACK TO sp1;
来源：http://tjo.cdnleiting.top

[Q69] 查看执行计划
来源：http://xft.ydjk.org.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://idl.fengsongda.top

[Q70] 更新统计信息
来源：http://pzr.ywan-chungtsiang.top

ANALYZE TABLE users;
来源：http://uci.shangyingyoupin.top

[Q71] 查看建表语句
来源：http://bpt.hywenlv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jnb.svipenyu.cn

[Q72] 查看索引
来源：http://xxk.havefunace.top

SHOW INDEX FROM users;
来源：http://dim.yj20258.top

[Q73] 查看表状态
来源：http://oql.jqgufenzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://czg.ywan-chungtsiang.top

[Q74] 强制使用索引
来源：http://xlh.jqgufenzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fde.gotoacloud.top

[Q75] 日期格式化
来源：http://dqb.guannengcc.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tsz.jlsjyb.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dxb.sysykeji.top

[Q76] 按天统计
来源：http://irz.feifeiyinyue.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tva.bbcook.cn

[Q77] 时间加减
来源：http://ofc.havefunace.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vdc.guowangkeji.top

[Q78] 当前时间
来源：http://gse.shuidangran.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pdt.c1oappe.top

[Q79] 字符串拼接
来源：http://sqw.jinqigfzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wsz.shanyushiyangtech.top

[Q80] 字符串截取
来源：http://xhc.mhx1999.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://urb.shanyushiyangkeji.top

[Q81] 字符串替换
来源：http://tfv.yj202588.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nij.shzxlz.cn

[Q82] 字符长度与字节长度
来源：http://xxd.pengpengdd.cyou

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qpy.gaohongyu789.top

[Q83] 大小写转换
来源：http://fig.yj202588.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xgo.chenjidiqi.icu

[Q84] 去除首尾空格
来源：http://ufd.birdmap.top

SELECT TRIM(name) FROM users;
来源：http://gbb.quarkkingdee.top

[Q85] 数值取整
来源：http://tgb.wangshuangyany.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fpu.hcnkem.com

[Q86] 读取 JSON 字段
来源：http://vaq.sjlbkw.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kqj.svipenyu.cn

[Q87] JSON 字段做条件
来源：http://uhj.pengpengdd.cyou

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xpp.jinyuanbaomall.cn

[Q88] 行转列（条件聚合）
来源：http://jmb.andypj.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bhh.meibo888.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tve.yongpay.top

[Q89] 判断表是否存在
来源：http://scw.yuanzhike.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xra.316326.xyz

[Q90] 生成序号列
来源：http://sui.iojbl.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blu.hammf.cn

================================================================================
来源：http://bun.kuanghao11.cn

R. Bash 专题
来源：http://tyo.dianchejie.cn

================================================================================
来源：http://ate.ydzc1.top

[R01] shebang 与严格模式
来源：http://zfr.sxryk.cn

#!/usr/bin/env bash
来源：http://qiy.zdqjudy.top

set -euo pipefail
来源：http://vbw.meibo888.top

[R02] 变量赋值与使用
来源：http://jvl.hesvh.cn

name="Tom"; echo "$name"
来源：http://vnz.hammf.cn

[R03] 只读变量
来源：http://ykx.dianchejie.cn

readonly PI=3.14
来源：http://jjg.hammf.cn

[R04] 位置参数
来源：http://nha.daria6918.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jiz.316326.xyz

[R05] 参数默认值
来源：http://pfo.svipenyu.cn

name="${1:-default}"
来源：http://och.aizwys.cn

[R06] 判断命令是否存在
来源：http://exo.daxiang520.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://glz.pycfn.com

[R07] if 判断文件
来源：http://gdr.ydzc1.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hwh.yanxiufei.cn

[R08] 数值比较
来源：http://cqx.hcnkem.com

if (( a > b )); then echo "a 更大"; fi
来源：http://nwc.hnqzz.top

[R09] 字符串比较
来源：http://boi.hesvh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gsv.cdnleiting.top

[R10] 正则匹配
来源：http://cmr.zhijiandao.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zuf.hfpthk.cn

[R11] case 多分支
来源：http://bri.jinqigfzy.top

case "$1" in
来源：http://tel.meibo888.top

start) echo "启动" ;;
来源：http://nfz.zhengqikj.top

stop)  echo "停止" ;;
来源：http://cxy.zdqjudy.top

*)     echo "未知命令" ;;
来源：http://tam.shanyushiyangkeji.top

esac
来源：http://nhd.yangfankeji.com

[R12] for 遍历文件
来源：http://rml.cheryme.top

for f in *.txt; do echo "$f"; done
来源：http://vaw.sjlbkw.cn

[R13] for 计数循环
来源：http://xho.bjfxy.top

for i in {1..10}; do echo "$i"; done
来源：http://nyi.hongshengwenyu.top

[R14] C 风格 for
来源：http://als.ydzc1.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rpa.bjfxy.top

[R15] while 逐行读文件
来源：http://lgm.gaohongyu789.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xco.xinyue.icu

[R16] until 等待条件
来源：http://exq.yj20258888.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jgr.cucudq.cn

[R17] 数组定义与取值
来源：http://duv.pycfn.com

arr=(a b c); echo "${arr[0]}"
来源：http://pcj.mhx1999.top

[R18] 遍历数组
来源：http://vbq.zhijiandao.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qci.cdnleiting.top

[R19] 数组长度
来源：http://cbd.ehwqpu.com

echo "${#arr[@]}"
来源：http://cxp.xinyue.icu

[R20] 关联数组（字典）
来源：http://olj.nanxinkj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://stv.haohaochexian.top

[R21] 字符串长度
来源：http://dkl.316326.xyz


<!-- 参考信息 -->