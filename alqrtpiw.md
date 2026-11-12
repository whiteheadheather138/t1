代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gqf.jinghuilouyu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bvc.shanyushiyangkeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tpb.vehdjk.com

[P04] 求长度
来源：http://ibu.yuxming.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hak.smart0.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rrb.hongshengwenyu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uqu.hnxiangtu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uae.chenzaomai.com

Java: list.size();  map.size();  s.length()
来源：http://ogl.meibo888.top

Go:   len(arr);  len(m)
来源：http://rss.gotoacloud.top

Ruby: x.length;  x.size
来源：http://dio.sxryk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jfr.daxiang520.top

[P05] 判断两个对象内容是否相等
来源：http://qkg.ivvv.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://swp.nanxuanxn.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wio.tarul.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yrv.shangyingyoupin.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://czg.jyoumei.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://klp.xuetiantiany.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mhi.yanxiufei.cn

Ruby: a == b
来源：http://cfg.sufxvd.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xcx.iojbl.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mpa.daria6918.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mkp.jiagoushi.top

PHP:  if (empty($x)) {}
来源：http://rnt.tanke756.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://aib.zdqjudy.top

TS:   if (x == null) {}
来源：http://ovn.yvedp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://azo.jinqigfzy.top

Go:   if x == nil {}
来源：http://jxv.hnxiangtu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nng.smart0.xyz

C#:   if (x is null) {}
来源：http://zum.svipenyu.cn

[P07] 防抖与节流
来源：http://adv.ctjpmb.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://duh.iojbl.cn

PHP:  // 手写时间戳比较
来源：http://uat.hfpthk.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nuz.fehbvm.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ntz.cqqwz.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jhx.daria6918.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xnq.ybcxt.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://vxi.dashuyun.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cob.tarul.cn

[P08] 处理浮点精度问题
来源：http://mrk.shangyingyoupin.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://oua.chenjidiqi.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bnw.fehbvm.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jzx.wangshuangyany.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ujn.52xcode.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dzf.ywan-chungtsiang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fsp.sufxvd.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zjq.snrcjt.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ocz.pengpengdd.cyou

================================================================================
来源：http://afu.yj20258888.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bnj.xingfuxueyuan.xyz

================================================================================
来源：http://vgm.zhongyouzk.top

[Q01] 创建表
来源：http://hmm.cucudq.cn

CREATE TABLE users (
来源：http://zca.pycfn.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jlc.yangfankeji.com

name VARCHAR(50) NOT NULL,
来源：http://usy.zhoulong.xyz

email VARCHAR(100) UNIQUE,
来源：http://qvz.dashuyun.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://csl.pengpengdd.cyou

);
来源：http://dqr.jlsjyb.cn

[Q02] 创建带外键的表
来源：http://obs.ydzc1.top

CREATE TABLE orders (
来源：http://yeo.yvedp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eki.zhengqikj.top

user_id INT NOT NULL,
来源：http://czi.zhiwuduotai.top

amount DECIMAL(10, 2),
来源：http://mwy.havefunace.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://oje.ctjpmb.com

);
来源：http://mla.xuanzx.com

[Q03] 增加列
来源：http://uxa.jinghuilouyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ied.hywenlv.cn

[Q04] 修改列类型
来源：http://oin.shuidangran.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dyk.gaohongyu789.top

[Q05] 重命名列
来源：http://toz.zhixingplan.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rfh.zhengqikj.top

[Q06] 删除列
来源：http://sde.hywenlv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ubm.zdbjq.cn

[Q07] 删除表
来源：http://pip.cucudq.cn

DROP TABLE IF EXISTS orders;
来源：http://chf.yvedp.cn

[Q08] 创建普通索引
来源：http://gfs.guannengcc.top

CREATE INDEX idx_users_email ON users(email);
来源：http://wrf.daxiang520.top

[Q09] 创建唯一索引
来源：http://jwt.jiagoushi.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fwk.hywenlv.cn

[Q10] 插入单行
来源：http://xzv.pengpengdd.cyou

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ejf.yj20258888.top

[Q11] 一次插入多行
来源：http://stf.pengpengdd.cyou

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nlp.wangdashe.top

[Q12] 插入后取自增 ID
来源：http://hxe.daria6918.cn

INSERT INTO users (name) VALUES ('C');
来源：http://loz.xziqi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ebj.xziqi.cn

[Q13] 忽略重复插入
来源：http://akh.chenjidiqi.icu

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zgr.zycfv.cn

[Q14] 存在则更新（upsert）
来源：http://tgz.gaohongyu789.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xyf.shuidangran.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pyd.fehbvm.com

[Q15] 查询全部
来源：http://snt.jqgufenzy.top

SELECT * FROM users;
来源：http://trr.tarul.cn

[Q16] 查询指定列
来源：http://knn.pycfn.com

SELECT id, name FROM users;
来源：http://ntc.yangfankeji.com

[Q17] 条件查询
来源：http://esk.ybcxt.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gda.sysykeji.top

[Q18] 模糊匹配
来源：http://qbp.cqqwz.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bqs.cashguo.top

[Q19] 范围查询
来源：http://vfv.jlsjyb.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ypb.iojbl.cn

[Q20] IN 列表
来源：http://ouc.jqgufenzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://acu.guowangkeji.top

[Q21] 空值判断
来源：http://iro.havefunace.top

SELECT * FROM users WHERE email IS NULL;
来源：http://wxm.shanyushiyangkeji.top

[Q22] 排序
来源：http://wkn.zhijiandao.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xbg.jianghu66.top

[Q23] 分页
来源：http://nia.ppjwa.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yct.yuanzhike.top

[Q24] 去重
来源：http://agm.iojbl.cn

SELECT DISTINCT city FROM users;
来源：http://zfn.tianlin.xyz

[Q25] 只取前 N 条
来源：http://xzx.cdnleiting.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gyq.hysaishi.cn

[Q26] 计数
来源：http://jxk.guannengcc.top

SELECT COUNT(*) FROM users;
来源：http://kxn.zhijiandao.cn

[Q27] 条件计数
来源：http://pko.zhiwuduotai.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zdx.gotoacloud.top

[Q28] 求和与平均
来源：http://xhy.aizwys.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ovr.yuanzhike.top

[Q29] 最大最小值
来源：http://hsz.jqgfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://akg.yanxiufei.cn

[Q30] 分组统计
来源：http://wgc.zycfv.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vrb.ydjk.org.cn

[Q31] 分组后过滤
来源：http://iet.pengpengdd.cyou

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://brd.feifeiyinyue.top

[Q32] 分组拼接字符串
来源：http://hxa.feifeiyinyue.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hpk.kuanghao11.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kia.hnxiangtu.top

[Q33] 多列分组
来源：http://nsk.vqdsnc.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://emg.chenlongwang.top

[Q34] 每组取第一条
来源：http://drd.hammf.cn

SELECT * FROM (
来源：http://mtf.shanyushiyangkeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jwb.zdqjudy.top

) t WHERE rn = 1;
来源：http://adq.ctjpmb.com

[Q35] 内连接
来源：http://ctr.fktsv.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://deu.hongshengwenyu.top

[Q36] 左连接
来源：http://lpx.yj202588.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://aon.jinyuanbaomall.cn

[Q37] 右连接
来源：http://lul.jyoumei.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lts.zdbjq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://oud.daria6918.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nap.sufxvd.cn

[Q39] 自连接（查上下级）
来源：http://yed.ctjpmb.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://zpy.vehdjk.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rpa.sufxvd.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wyz.ppjwa.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tcn.svipenyu.cn

[Q41] 多表连接
来源：http://wqc.zhiwuduotai.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://apl.hywenlv.cn

JOIN users u ON u.id = o.user_id
来源：http://hfg.cqqwz.cn

JOIN products p ON p.id = o.product_id;
来源：http://lfj.cheryme.top

[Q42] 连接条件附加过滤
来源：http://utq.aizwys.cn

SELECT u.name, o.amount FROM users u
来源：http://iov.ybcxt.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yvb.tanke756.top

[Q43] 标量子查询
来源：http://mph.jinqigfzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dkd.iojbl.cn

[Q44] IN 子查询
来源：http://gai.meibo888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bol.yvedp.cn

[Q45] EXISTS 判断存在
来源：http://dza.jqgfzy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tyr.sysykeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://xnn.dashuyun.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://std.daxiang520.top

[Q47] 与平均值比较
来源：http://zew.guannengcc.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://brh.ywan-chungtsiang.top

[Q48] CTE 公用表表达式
来源：http://ige.zhiwuduotai.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wmh.aizwys.cn

SELECT * FROM t WHERE c > 5;
来源：http://oam.redwolf501.top

[Q49] 更新单行
来源：http://wne.jinghuilouyu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bhp.bbcook.cn

[Q50] 批量更新
来源：http://rvy.jyoumei.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rcw.jlsjyb.cn

[Q51] 用子查询更新
来源：http://xrh.wangshuangyany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kha.jinqigfzy.top

[Q52] 删除指定行
来源：http://hek.chenjidiqi.icu

DELETE FROM users WHERE id = 10;
来源：http://hka.yuxming.cn

[Q53] 按条件删除
来源：http://bia.fanxiaobao.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dxm.gotoacloud.top

[Q54] 清空表
来源：http://sss.iojbl.cn

TRUNCATE TABLE logs;
来源：http://nky.316326.xyz

[Q55] 排名（并列占位）
来源：http://acm.shzxlz.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://atx.xinyue.icu

[Q56] 密集排名（并列不占位）
来源：http://sid.yongpay.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://owe.jiagoushi.top

[Q57] 行号
来源：http://qnz.aibaodan.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://aoy.redwolf501.top

[Q58] 累计求和
来源：http://dar.iojbl.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uho.xuetiantiany.cn

[Q59] 分组内累计
来源：http://nes.jinyuanbaomall.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rsi.wangshuangyany.cn

[Q60] 取上一行 / 下一行
来源：http://tlt.tarul.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bae.yuanzhike.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ozu.cqqwz.cn

[Q61] 移动平均
来源：http://acu.yuxming.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://psh.vehdjk.com

[Q62] 分组占比
来源：http://zjv.jinqigufen.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://itk.ctjpmb.com

[Q63] 开启事务
来源：http://rfa.ehwqpu.com

START TRANSACTION;                -- 或 BEGIN
来源：http://rgd.hammf.cn

[Q64] 提交事务
来源：http://lpn.shuidangran.top

COMMIT;
来源：http://eyr.chenjidiqi.icu

[Q65] 回滚事务
来源：http://add.52xcode.cn

ROLLBACK;
来源：http://rnp.ivvv.top

[Q66] 行锁查询
来源：http://ebe.bbcook.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qbi.hysaishi.cn

[Q67] 设置隔离级别
来源：http://irm.xingfuxueyuan.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cvp.wangshuangyany.cn

[Q68] 保存点
来源：http://ifx.dashuyun.cn

SAVEPOINT sp1;
来源：http://jll.yfazqb.com

ROLLBACK TO sp1;
来源：http://wco.wangshuangyany.cn

[Q69] 查看执行计划
来源：http://kqd.bjfxy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://auh.gaohongyu789.top

[Q70] 更新统计信息
来源：http://aef.cqqwz.cn

ANALYZE TABLE users;
来源：http://mbk.fktsv.cn

[Q71] 查看建表语句
来源：http://hyo.zdqjudy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fxo.9152youxi.cn

[Q72] 查看索引
来源：http://dcm.jiagoushi.top

SHOW INDEX FROM users;
来源：http://wjb.cqqwz.cn

[Q73] 查看表状态
来源：http://okz.zhiwuduotai.top

SHOW TABLE STATUS LIKE 'users';
来源：http://gzl.chenzaomai.com

[Q74] 强制使用索引
来源：http://wdm.c1oappe.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rrs.svipenyu.cn

[Q75] 日期格式化
来源：http://ell.epnwcf.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mxz.jyoumei.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bju.jyoumei.cn

[Q76] 按天统计
来源：http://ici.yvedp.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kgc.haohaochexian.top

[Q77] 时间加减
来源：http://xmg.jinghuilouyu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vwz.shanyushiyangkeji.top

[Q78] 当前时间
来源：http://wau.yuxming.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://akh.pycfn.com

[Q79] 字符串拼接
来源：http://gqk.nwbrower.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ohc.shzxlz.cn

[Q80] 字符串截取
来源：http://wqp.quarkkingdee.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lol.bbcook.cn

[Q81] 字符串替换
来源：http://tfg.xuetiantiany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hph.uphjek.com

[Q82] 字符长度与字节长度
来源：http://oru.zhixingplan.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uhf.shanyushiyangtech.top

[Q83] 大小写转换
来源：http://hwy.cdnleiting.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hiz.cucudq.cn

[Q84] 去除首尾空格
来源：http://ugs.ydzc1.top

SELECT TRIM(name) FROM users;
来源：http://brt.jqgfzy.top

[Q85] 数值取整
来源：http://ccp.fanxiaobao.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://djr.zhengqikj.top

[Q86] 读取 JSON 字段
来源：http://vvq.uphjek.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://eru.sysykeji.top

[Q87] JSON 字段做条件
来源：http://tcp.gogol.net.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://syz.hfpthk.cn

[Q88] 行转列（条件聚合）
来源：http://irf.jinqigfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vyo.uphjek.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lzj.yongpay.top

[Q89] 判断表是否存在
来源：http://dzf.shanyushiyangkeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pjy.ppjwa.cn

[Q90] 生成序号列
来源：http://nps.xziqi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://fay.zhaomingkeji.xyz

================================================================================
来源：http://gtd.xuetiantiany.cn

R. Bash 专题
来源：http://xnq.pycfn.com

================================================================================
来源：http://nfn.wangdashe.top

[R01] shebang 与严格模式
来源：http://jzm.sjlbkw.cn

#!/usr/bin/env bash
来源：http://pcx.ivvv.top

set -euo pipefail
来源：http://hot.hfpthk.cn

[R02] 变量赋值与使用
来源：http://lbk.ppjwa.cn

name="Tom"; echo "$name"
来源：http://blq.xingfuxueyuan.xyz

[R03] 只读变量
来源：http://zsc.zhixingplan.top

readonly PI=3.14
来源：http://aew.jinyuanbaomall.cn

[R04] 位置参数
来源：http://nfd.sufxvd.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fbf.jinqigfzy.top

[R05] 参数默认值
来源：http://wvm.kuanghao11.cn

name="${1:-default}"
来源：http://auf.guannengcc.top

[R06] 判断命令是否存在
来源：http://xzl.fengsongda.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kjk.ctjpmb.com

[R07] if 判断文件
来源：http://zcj.ywan-chungtsiang.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ywh.zycfv.cn

[R08] 数值比较
来源：http://wzy.zhengqikj.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ssa.jinqigfzy.top

[R09] 字符串比较
来源：http://mbg.sweek.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bkl.uphjek.com

[R10] 正则匹配
来源：http://zjg.sweek.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ufo.havefunace.top

[R11] case 多分支
来源：http://ihw.wangshuangyany.cn

case "$1" in
来源：http://xjg.ydzc1.top

start) echo "启动" ;;
来源：http://upy.tanke756.top

stop)  echo "停止" ;;
来源：http://rsw.c1oappe.top

*)     echo "未知命令" ;;
来源：http://xlw.sjlbkw.cn

esac
来源：http://nqj.chenlongwang.top

[R12] for 遍历文件
来源：http://aio.pycfn.com

for f in *.txt; do echo "$f"; done
来源：http://pxo.shuidangran.top

[R13] for 计数循环
来源：http://olp.sysykeji.top

for i in {1..10}; do echo "$i"; done
来源：http://iim.hywenlv.cn

[R14] C 风格 for
来源：http://vbn.gogol.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ejd.tian-w.cn

[R15] while 逐行读文件
来源：http://gbw.fehbvm.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mbg.52xcode.cn

[R16] until 等待条件
来源：http://bjm.jlsjyb.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lqf.smart0.xyz

[R17] 数组定义与取值
来源：http://vew.hcnkem.com

arr=(a b c); echo "${arr[0]}"
来源：http://hhd.cucudq.cn

[R18] 遍历数组
来源：http://fqf.iojbl.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ucq.aizwys.cn

[R19] 数组长度
来源：http://bai.andypj.xyz


<!-- 参考信息 -->