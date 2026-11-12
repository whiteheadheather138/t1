代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://uip.zhixingplan.top

Go:   len(arr);  len(m)
来源：http://sxn.hywenlv.cn

Ruby: x.length;  x.size
来源：http://opv.haohaochexian.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://igq.fengsongda.top

[P05] 判断两个对象内容是否相等
来源：http://yie.wangshuangyany.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zze.shanyushiyangtech.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qhm.gzhubu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kmx.svipenyu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lev.fktsv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ngh.yj202588.top

Go:   reflect.DeepEqual(a, b)
来源：http://tcr.hysaishi.cn

Ruby: a == b
来源：http://zqu.snrcjt.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ybh.tian-w.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nir.daxiang520.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dct.havefunace.top

PHP:  if (empty($x)) {}
来源：http://gdw.hongshengwenyu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://upa.epnwcf.com

TS:   if (x == null) {}
来源：http://cbg.cashguo.top

Java: if (x == null || x.isEmpty()) {}
来源：http://qgu.fehbvm.com

Go:   if x == nil {}
来源：http://ngc.vehdjk.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fqc.sxryk.cn

C#:   if (x is null) {}
来源：http://skl.iojbl.cn

[P07] 防抖与节流
来源：http://nct.zhoulong.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://aff.sxryk.cn

PHP:  // 手写时间戳比较
来源：http://dck.feifeiyinyue.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yvc.sxryk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cln.sweek.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cof.yvedp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xkc.yfazqb.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://naf.xylfe.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kit.shuidangran.top

[P08] 处理浮点精度问题
来源：http://xqn.yongpay.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zvh.guowangkeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nzg.havefunace.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hwi.ybcxt.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hpz.ydjk.org.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kzh.xuetiantiany.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kln.hongshengwenyu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uuo.fzhhl.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://aan.ivvv.top

================================================================================
来源：http://pfy.zdqjudy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oob.c1oappe.top

================================================================================
来源：http://hry.mhx1999.top

[Q01] 创建表
来源：http://uef.zhoulong.xyz

CREATE TABLE users (
来源：http://osb.nanxinkj.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uys.jinghuilouyu.cn

name VARCHAR(50) NOT NULL,
来源：http://pas.gaohongyu789.top

email VARCHAR(100) UNIQUE,
来源：http://hvt.guowangkeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://aek.zycfv.cn

);
来源：http://zdq.yuxming.cn

[Q02] 创建带外键的表
来源：http://bni.fzhhl.top

CREATE TABLE orders (
来源：http://aii.zhixingplan.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://czq.guowangkeji.top

user_id INT NOT NULL,
来源：http://vfy.ydzc1.top

amount DECIMAL(10, 2),
来源：http://bph.dianchejie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dbc.yangfankeji.com

);
来源：http://qcq.ctjpmb.com

[Q03] 增加列
来源：http://sam.svipenyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zsd.hcnkem.com

[Q04] 修改列类型
来源：http://evo.zhiwuduotai.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jyr.chenlongwang.top

[Q05] 重命名列
来源：http://nza.zycfv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rgh.yangfankeji.com

[Q06] 删除列
来源：http://bde.quarkkingdee.top

ALTER TABLE users DROP COLUMN age;
来源：http://diw.hysaishi.cn

[Q07] 删除表
来源：http://kdk.feifeiyinyue.top

DROP TABLE IF EXISTS orders;
来源：http://svj.zhongyouzk.top

[Q08] 创建普通索引
来源：http://lmm.zycfv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zaa.hysaishi.cn

[Q09] 创建唯一索引
来源：http://alr.zhixingplan.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xec.yuxming.cn

[Q10] 插入单行
来源：http://imm.ctjpmb.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://umz.yonumen.top

[Q11] 一次插入多行
来源：http://uzp.hywenlv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lxp.jyoumei.cn

[Q12] 插入后取自增 ID
来源：http://cmm.hongshengwenyu.top

INSERT INTO users (name) VALUES ('C');
来源：http://kgu.jinqigufen.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://acq.zycfv.cn

[Q13] 忽略重复插入
来源：http://dnm.9152youxi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://arf.jqgufenzy.top

[Q14] 存在则更新（upsert）
来源：http://lfi.yanxiufei.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://imy.shanyushiyangtech.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://thw.hnxiangtu.top

[Q15] 查询全部
来源：http://atn.havefunace.top

SELECT * FROM users;
来源：http://vkx.shanyushiyangtech.top

[Q16] 查询指定列
来源：http://wsj.zhijiandao.cn

SELECT id, name FROM users;
来源：http://orf.316326.xyz

[Q17] 条件查询
来源：http://ttt.havefunace.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dzn.ybcxt.top

[Q18] 模糊匹配
来源：http://kvw.yueranfly.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://onr.9152youxi.cn

[Q19] 范围查询
来源：http://vqu.sysykeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ohw.xuetiantiany.cn

[Q20] IN 列表
来源：http://ysh.hywenlv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kqv.mhx1999.top

[Q21] 空值判断
来源：http://per.jinyuanbaomall.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kql.haohaochexian.top

[Q22] 排序
来源：http://dxr.chenzaomai.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ctp.epnwcf.com

[Q23] 分页
来源：http://peg.jinghuilouyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mkz.jianghu66.top

[Q24] 去重
来源：http://bhu.fengsongda.top

SELECT DISTINCT city FROM users;
来源：http://qgm.kuanghao11.cn

[Q25] 只取前 N 条
来源：http://nrs.dianchejie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tdd.fzhhl.top

[Q26] 计数
来源：http://aix.zhiwuduotai.top

SELECT COUNT(*) FROM users;
来源：http://xij.kuanghao11.cn

[Q27] 条件计数
来源：http://vst.hcnkem.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uya.svipenyu.cn

[Q28] 求和与平均
来源：http://srn.sxryk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ssf.gaohongyu789.top

[Q29] 最大最小值
来源：http://fra.ehwqpu.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://ido.dashuyun.cn

[Q30] 分组统计
来源：http://bqm.aibaodan.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://scn.vqdsnc.cn

[Q31] 分组后过滤
来源：http://ulr.meibo888.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ubl.hcnkem.com

[Q32] 分组拼接字符串
来源：http://hql.dianchejie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://idz.yj20258.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lte.zhongyouzk.top

[Q33] 多列分组
来源：http://gmx.0kj1m.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pyg.cdnleiting.top

[Q34] 每组取第一条
来源：http://fjs.mhx1999.top

SELECT * FROM (
来源：http://ybh.wangdashe.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ymm.iojbl.cn

) t WHERE rn = 1;
来源：http://gmt.vqdsnc.cn

[Q35] 内连接
来源：http://axh.nwbrower.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pkm.xinyue.icu

[Q36] 左连接
来源：http://gwz.cashguo.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fjo.zdbjq.cn

[Q37] 右连接
来源：http://eti.andypj.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://the.ctjpmb.com

[Q38] 全外连接（PostgreSQL）
来源：http://cjh.nanxuanxn.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nlh.tarul.cn

[Q39] 自连接（查上下级）
来源：http://qnz.yonumen.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://lsj.zhongyouzk.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yjk.dashuyun.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://iny.shanyushiyangtech.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nwc.xziqi.cn

[Q41] 多表连接
来源：http://ckw.gogol.net.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xux.zhoulong.xyz

JOIN users u ON u.id = o.user_id
来源：http://cww.sysykeji.top

JOIN products p ON p.id = o.product_id;
来源：http://tgn.wangshuangyany.cn

[Q42] 连接条件附加过滤
来源：http://scq.yj20258.top

SELECT u.name, o.amount FROM users u
来源：http://rda.pengpengdd.cyou

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://asn.shanyushiyangtech.top

[Q43] 标量子查询
来源：http://zye.zdbjq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rea.jqgufenzy.top

[Q44] IN 子查询
来源：http://ekb.redwolf501.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cub.hesvh.cn

[Q45] EXISTS 判断存在
来源：http://tle.yueranfly.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gwb.cheryme.top

[Q46] NOT EXISTS 判断不存在
来源：http://rie.hnqzz.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vos.ydjk.org.cn

[Q47] 与平均值比较
来源：http://wha.gaohongyu789.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xcn.sjlbkw.cn

[Q48] CTE 公用表表达式
来源：http://xes.xziqi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ims.andypj.xyz

SELECT * FROM t WHERE c > 5;
来源：http://pqc.hywenlv.cn

[Q49] 更新单行
来源：http://ulo.ivvv.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mql.hcnkem.com

[Q50] 批量更新
来源：http://qbs.bbcook.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dpz.fehbvm.com

[Q51] 用子查询更新
来源：http://zil.guowangkeji.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tpf.mhx1999.top

[Q52] 删除指定行
来源：http://xvc.hcnkem.com

DELETE FROM users WHERE id = 10;
来源：http://hpg.guannengcc.top

[Q53] 按条件删除
来源：http://jmr.xuetiantiany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://erq.ybcxt.top

[Q54] 清空表
来源：http://jcq.zdqjudy.top

TRUNCATE TABLE logs;
来源：http://quv.sxryk.cn

[Q55] 排名（并列占位）
来源：http://uni.yj20258888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qwy.chenlongwang.top

[Q56] 密集排名（并列不占位）
来源：http://lon.daxiang520.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://okx.zhixingplan.top

[Q57] 行号
来源：http://yjg.quarkkingdee.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xxz.jlsjyb.cn

[Q58] 累计求和
来源：http://mvf.jianghu66.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yym.redwolf501.top

[Q59] 分组内累计
来源：http://kbm.andypj.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fwr.zdqjudy.top

[Q60] 取上一行 / 下一行
来源：http://rgv.snrcjt.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vid.mhx1999.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dxs.redwolf501.top

[Q61] 移动平均
来源：http://vph.nwbrower.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uyb.havefunace.top

[Q62] 分组占比
来源：http://sci.aizwys.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ecz.shanyushiyangtech.top

[Q63] 开启事务
来源：http://xxb.svipenyu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bpk.kuanghao11.cn

[Q64] 提交事务
来源：http://fqh.tarul.cn

COMMIT;
来源：http://tba.fengsongda.top

[Q65] 回滚事务
来源：http://yad.xziqi.cn

ROLLBACK;
来源：http://ygg.fengsongda.top

[Q66] 行锁查询
来源：http://eep.aizwys.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zal.316326.xyz

[Q67] 设置隔离级别
来源：http://hkm.hnqzz.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rec.zhongyouzk.top

[Q68] 保存点
来源：http://fxa.jiagoushi.top

SAVEPOINT sp1;
来源：http://hai.hnxiangtu.top

ROLLBACK TO sp1;
来源：http://low.pycfn.com

[Q69] 查看执行计划
来源：http://yiw.jqgufenzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hki.ydzc1.top

[Q70] 更新统计信息
来源：http://nwp.yongpay.top

ANALYZE TABLE users;
来源：http://dym.sjlbkw.cn

[Q71] 查看建表语句
来源：http://byy.yangfankeji.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ilx.dianchejie.cn

[Q72] 查看索引
来源：http://suc.jlsjyb.cn

SHOW INDEX FROM users;
来源：http://uam.hywenlv.cn

[Q73] 查看表状态
来源：http://ofg.tianlin.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://vvi.shzxlz.cn

[Q74] 强制使用索引
来源：http://zjl.iojbl.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jwu.hesvh.cn

[Q75] 日期格式化
来源：http://aiy.guowangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://frm.fktsv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://oay.yueranfly.top

[Q76] 按天统计
来源：http://ipg.guannengcc.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zkm.hnxiangtu.top

[Q77] 时间加减
来源：http://usx.gogol.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://usz.cucudq.cn

[Q78] 当前时间
来源：http://qqn.daxiang520.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bjq.shanyushiyangkeji.top

[Q79] 字符串拼接
来源：http://mkt.jinghuilouyu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rhe.jinqigfzy.top

[Q80] 字符串截取
来源：http://fcs.yongpay.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oks.tianlin.xyz

[Q81] 字符串替换
来源：http://thx.hnqzz.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://myj.tianlin.xyz

[Q82] 字符长度与字节长度
来源：http://oci.daria6918.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://muh.zhoulong.xyz

[Q83] 大小写转换
来源：http://cxu.yuanzhike.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tll.aizwys.cn

[Q84] 去除首尾空格
来源：http://nqu.sxryk.cn

SELECT TRIM(name) FROM users;
来源：http://idf.gzhubu.top

[Q85] 数值取整
来源：http://nri.feifeiyinyue.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qeu.cucudq.cn

[Q86] 读取 JSON 字段
来源：http://wcq.fehbvm.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qps.dashuyun.cn

[Q87] JSON 字段做条件
来源：http://ozn.hammf.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fzt.chenlongwang.top

[Q88] 行转列（条件聚合）
来源：http://vbd.vehdjk.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xjb.yuanzhike.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://akg.bbcook.cn

[Q89] 判断表是否存在
来源：http://rza.yongpay.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kos.birdmap.top

[Q90] 生成序号列
来源：http://buh.jianghu66.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mxi.jinyuanbaomall.cn

================================================================================
来源：http://rux.havefunace.top

R. Bash 专题
来源：http://ydx.chenlongwang.top

================================================================================
来源：http://nwr.smart0.xyz

[R01] shebang 与严格模式
来源：http://peq.ehwqpu.com

#!/usr/bin/env bash
来源：http://xtr.shanyushiyangkeji.top

set -euo pipefail
来源：http://jjm.fehbvm.com

[R02] 变量赋值与使用
来源：http://rwc.zycfv.cn

name="Tom"; echo "$name"
来源：http://qvk.zhijiandao.cn

[R03] 只读变量
来源：http://kru.ehwqpu.com

readonly PI=3.14
来源：http://mid.ehwqpu.com

[R04] 位置参数
来源：http://bjs.pengpengdd.cyou

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pxx.hammf.cn

[R05] 参数默认值
来源：http://nev.ehwqpu.com

name="${1:-default}"
来源：http://osu.gaohongyu789.top

[R06] 判断命令是否存在
来源：http://fvg.hywenlv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rrv.redwolf501.top

[R07] if 判断文件
来源：http://zbi.nanxinkj.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ryz.xylfe.cn

[R08] 数值比较
来源：http://ory.shuidangran.top

if (( a > b )); then echo "a 更大"; fi
来源：http://xpe.cqqwz.cn

[R09] 字符串比较
来源：http://ysq.chenlongwang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mjv.gogol.net.cn

[R10] 正则匹配
来源：http://gpx.yanxiufei.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://loy.hongshengwenyu.top

[R11] case 多分支
来源：http://bbj.guannengcc.top

case "$1" in
来源：http://mrt.vqdsnc.cn

start) echo "启动" ;;
来源：http://hix.tanke756.top

stop)  echo "停止" ;;
来源：http://dxs.cashguo.top

*)     echo "未知命令" ;;
来源：http://uup.zhongyouzk.top

esac
来源：http://kmq.gzhubu.top

[R12] for 遍历文件
来源：http://yrm.daria6918.cn

for f in *.txt; do echo "$f"; done
来源：http://ega.gogol.net.cn

[R13] for 计数循环
来源：http://hfj.fengsongda.top

for i in {1..10}; do echo "$i"; done
来源：http://nwk.shanyushiyangkeji.top

[R14] C 风格 for
来源：http://pyc.tarul.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gdh.fehbvm.com

[R15] while 逐行读文件
来源：http://zmy.fengsongda.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gzo.nwbrower.top

[R16] until 等待条件
来源：http://zzn.chenlongwang.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hhe.aibaodan.cn

[R17] 数组定义与取值
来源：http://rql.yangfankeji.com

arr=(a b c); echo "${arr[0]}"
来源：http://irc.jqgfzy.top

[R18] 遍历数组
来源：http://zod.mhx1999.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lzh.pycfn.com

[R19] 数组长度
来源：http://cbc.smart0.xyz

echo "${#arr[@]}"
来源：http://gsc.svipenyu.cn

[R20] 关联数组（字典）
来源：http://vbs.cdnleiting.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rop.daria6918.cn

[R21] 字符串长度
来源：http://xkc.jinqigufen.top

echo "${#s}"
来源：http://kbn.shanyushiyangkeji.top

[R22] 截取子串
来源：http://jgu.nwbrower.top

echo "${s:0:5}"
来源：http://jdy.tianlin.xyz

[R23] 字符串替换
来源：http://vsu.52xcode.cn


<!-- 参考信息 -->