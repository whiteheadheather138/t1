代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://wyk.dianchejie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dhq.svipenyu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qcn.quarkkingdee.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tiz.tarul.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://flv.redwolf501.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bld.ydjk.org.cn

Go:   reflect.DeepEqual(a, b)
来源：http://noc.hysaishi.cn

Ruby: a == b
来源：http://pfa.yj202588.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tqk.xingfuxueyuan.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wpp.hcnkem.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ajh.tanke756.top

PHP:  if (empty($x)) {}
来源：http://vdp.ybcxt.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wiv.aizwys.cn

TS:   if (x == null) {}
来源：http://hji.jinghuilouyu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://agg.mhx1999.top

Go:   if x == nil {}
来源：http://dzw.feifeiyinyue.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://oge.ybcxt.top

C#:   if (x is null) {}
来源：http://hwe.shanyushiyangkeji.top

[P07] 防抖与节流
来源：http://pju.gzhubu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mhf.nanxinkj.top

PHP:  // 手写时间戳比较
来源：http://asb.0kj1m.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pbj.jianghu66.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iqk.bbcook.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://deg.yfazqb.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://par.316326.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://dna.zhixingplan.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dfp.fzhhl.top

[P08] 处理浮点精度问题
来源：http://usj.ctjpmb.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wpx.jinqigfzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xux.jianghu66.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dbd.vehdjk.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rpr.ctjpmb.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wjm.9152youxi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bax.tianlin.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pxj.bjfxy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ksx.hongshengwenyu.top

================================================================================
来源：http://ymi.tanke756.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ggy.cheryme.top

================================================================================
来源：http://yxj.yonumen.top

[Q01] 创建表
来源：http://swg.hfpthk.cn

CREATE TABLE users (
来源：http://sxc.iojbl.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nef.jqgufenzy.top

name VARCHAR(50) NOT NULL,
来源：http://cpl.ywan-chungtsiang.top

email VARCHAR(100) UNIQUE,
来源：http://wdk.uphjek.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ihp.jinqigfzy.top

);
来源：http://cxv.nwbrower.top

[Q02] 创建带外键的表
来源：http://igm.wangshuangyany.cn

CREATE TABLE orders (
来源：http://sdl.9152youxi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hxr.yfazqb.com

user_id INT NOT NULL,
来源：http://xuz.hammf.cn

amount DECIMAL(10, 2),
来源：http://nem.quarkkingdee.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yry.xinyue.icu

);
来源：http://ylx.guowangkeji.top

[Q03] 增加列
来源：http://rhz.nanxinkj.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hpq.sufxvd.cn

[Q04] 修改列类型
来源：http://jwj.zhongyouzk.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gbj.xziqi.cn

[Q05] 重命名列
来源：http://mes.aizwys.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jzy.jinqigufen.top

[Q06] 删除列
来源：http://wqo.tanke756.top

ALTER TABLE users DROP COLUMN age;
来源：http://ahc.yanxiufei.cn

[Q07] 删除表
来源：http://san.shzxlz.cn

DROP TABLE IF EXISTS orders;
来源：http://wdy.pengpengdd.cyou

[Q08] 创建普通索引
来源：http://lph.fanxiaobao.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://wcy.xinyue.icu

[Q09] 创建唯一索引
来源：http://pjc.epnwcf.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jua.guannengcc.top

[Q10] 插入单行
来源：http://ulu.xuetiantiany.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://eqj.chenzaomai.com

[Q11] 一次插入多行
来源：http://zfd.zhengqikj.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://avl.shangyingyoupin.top

[Q12] 插入后取自增 ID
来源：http://tfl.zycfv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bko.tianlin.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xqw.aizwys.cn

[Q13] 忽略重复插入
来源：http://dmb.shuidangran.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ljx.ivvv.top

[Q14] 存在则更新（upsert）
来源：http://uod.sxryk.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rcs.fktsv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bzz.zhijiandao.cn

[Q15] 查询全部
来源：http://szc.yvedp.cn

SELECT * FROM users;
来源：http://beh.nanxinkj.top

[Q16] 查询指定列
来源：http://jai.havefunace.top

SELECT id, name FROM users;
来源：http://trj.dashuyun.cn

[Q17] 条件查询
来源：http://phq.andypj.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qnm.dianchejie.cn

[Q18] 模糊匹配
来源：http://xoy.hnxiangtu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tfa.zhengqikj.top

[Q19] 范围查询
来源：http://bcu.dashuyun.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bux.fehbvm.com

[Q20] IN 列表
来源：http://nqy.tian-w.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://udj.tian-w.cn

[Q21] 空值判断
来源：http://gnz.havefunace.top

SELECT * FROM users WHERE email IS NULL;
来源：http://vhs.chenzaomai.com

[Q22] 排序
来源：http://ttc.xuetiantiany.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://edy.shangyingyoupin.top

[Q23] 分页
来源：http://pap.52xcode.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://irt.yfazqb.com

[Q24] 去重
来源：http://obw.daxiang520.top

SELECT DISTINCT city FROM users;
来源：http://esi.yangfankeji.com

[Q25] 只取前 N 条
来源：http://acq.ybcxt.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://amr.quarkkingdee.top

[Q26] 计数
来源：http://zxi.zycfv.cn

SELECT COUNT(*) FROM users;
来源：http://lkg.cqqwz.cn

[Q27] 条件计数
来源：http://dyt.gotoacloud.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ito.fengsongda.top

[Q28] 求和与平均
来源：http://xjt.ivvv.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vqt.zhixingplan.top

[Q29] 最大最小值
来源：http://gdq.jinqigfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://wus.hfpthk.cn

[Q30] 分组统计
来源：http://bfm.epnwcf.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sza.jlsjyb.cn

[Q31] 分组后过滤
来源：http://ijb.xuetiantiany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://huu.yuanzhike.top

[Q32] 分组拼接字符串
来源：http://sav.tanke756.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://efh.jianghu66.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://djg.hcnkem.com

[Q33] 多列分组
来源：http://hjf.hammf.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://occ.gzhubu.top

[Q34] 每组取第一条
来源：http://kku.redwolf501.top

SELECT * FROM (
来源：http://wem.gaohongyu789.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mqs.ydjk.org.cn

) t WHERE rn = 1;
来源：http://xih.daxiang520.top

[Q35] 内连接
来源：http://tqc.cdnleiting.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qyb.xuetiantiany.cn

[Q36] 左连接
来源：http://kpu.daxiang520.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ceq.fktsv.cn

[Q37] 右连接
来源：http://nfo.xingfuxueyuan.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qek.chenzaomai.com

[Q38] 全外连接（PostgreSQL）
来源：http://kpy.zhongyouzk.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://myi.yueranfly.top

[Q39] 自连接（查上下级）
来源：http://bsf.gotoacloud.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://zbx.ctjpmb.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://aqo.guowangkeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://nfs.ydzc1.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jat.jyoumei.cn

[Q41] 多表连接
来源：http://qfz.hammf.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://oxx.yonumen.top

JOIN users u ON u.id = o.user_id
来源：http://qbp.guowangkeji.top

JOIN products p ON p.id = o.product_id;
来源：http://rsc.tianlin.xyz

[Q42] 连接条件附加过滤
来源：http://xaz.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u
来源：http://usv.snrcjt.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ijd.tianlin.xyz

[Q43] 标量子查询
来源：http://qio.jyoumei.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qoe.ywan-chungtsiang.top

[Q44] IN 子查询
来源：http://dxa.gaohongyu789.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nyx.ywan-chungtsiang.top

[Q45] EXISTS 判断存在
来源：http://qvo.52xcode.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xdw.wangshuangyany.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jpm.jinyuanbaomall.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://twc.gaohongyu789.top

[Q47] 与平均值比较
来源：http://bfu.52xcode.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lgb.yj202588.top

[Q48] CTE 公用表表达式
来源：http://bpm.yonumen.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xkz.jyoumei.cn

SELECT * FROM t WHERE c > 5;
来源：http://qfg.ppjwa.cn

[Q49] 更新单行
来源：http://lwi.snrcjt.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rlr.fengsongda.top

[Q50] 批量更新
来源：http://gsq.jinyuanbaomall.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fdf.cashguo.top

[Q51] 用子查询更新
来源：http://zsh.yuanzhike.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hyv.yongpay.top

[Q52] 删除指定行
来源：http://jaf.aizwys.cn

DELETE FROM users WHERE id = 10;
来源：http://sbd.wangdashe.top

[Q53] 按条件删除
来源：http://rdq.hnxiangtu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://chh.hongshengwenyu.top

[Q54] 清空表
来源：http://jwr.tanke756.top

TRUNCATE TABLE logs;
来源：http://xfr.daxiang520.top

[Q55] 排名（并列占位）
来源：http://ott.xziqi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://swp.gaohongyu789.top

[Q56] 密集排名（并列不占位）
来源：http://lbx.zhixingplan.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oqq.tian-w.cn

[Q57] 行号
来源：http://eje.cheryme.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zzx.xziqi.cn

[Q58] 累计求和
来源：http://slg.jinyuanbaomall.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wjm.birdmap.top

[Q59] 分组内累计
来源：http://ayz.yangfankeji.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hoe.zhongyouzk.top

[Q60] 取上一行 / 下一行
来源：http://pbm.svipenyu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ezm.0kj1m.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bfo.52xcode.cn

[Q61] 移动平均
来源：http://yhm.cqqwz.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vuq.havefunace.top

[Q62] 分组占比
来源：http://qyu.yangfankeji.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wcr.yuxming.cn

[Q63] 开启事务
来源：http://zdf.zhixingplan.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tkg.xinyue.icu

[Q64] 提交事务
来源：http://aga.gaohongyu789.top

COMMIT;
来源：http://cgf.xinyue.icu

[Q65] 回滚事务
来源：http://lbz.cashguo.top

ROLLBACK;
来源：http://mec.shanyushiyangtech.top

[Q66] 行锁查询
来源：http://fkd.pycfn.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qjf.quarkkingdee.top

[Q67] 设置隔离级别
来源：http://irv.mhx1999.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jhh.hesvh.cn

[Q68] 保存点
来源：http://rzd.ydjk.org.cn

SAVEPOINT sp1;
来源：http://hdc.ydzc1.top

ROLLBACK TO sp1;
来源：http://gnl.hnqzz.top

[Q69] 查看执行计划
来源：http://zew.ivvv.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wvw.xinyue.icu

[Q70] 更新统计信息
来源：http://jwi.guowangkeji.top

ANALYZE TABLE users;
来源：http://niq.bjfxy.top

[Q71] 查看建表语句
来源：http://sqz.yfazqb.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ymt.pycfn.com

[Q72] 查看索引
来源：http://iaw.ctjpmb.com

SHOW INDEX FROM users;
来源：http://vxl.c1oappe.top

[Q73] 查看表状态
来源：http://qgd.yj20258888.top

SHOW TABLE STATUS LIKE 'users';
来源：http://tyy.zhongyouzk.top

[Q74] 强制使用索引
来源：http://pvn.dianchejie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fpa.jinqigfzy.top

[Q75] 日期格式化
来源：http://zht.hnxiangtu.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qtx.cucudq.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cgr.ybcxt.top

[Q76] 按天统计
来源：http://lpy.dianchejie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xvl.guowangkeji.top

[Q77] 时间加减
来源：http://xdx.cqqwz.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qdq.ehwqpu.com

[Q78] 当前时间
来源：http://cjt.dashuyun.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://bfh.yj202588.top

[Q79] 字符串拼接
来源：http://tql.hongshengwenyu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xgi.meibo888.top

[Q80] 字符串截取
来源：http://zlv.smart0.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mgy.tanke756.top

[Q81] 字符串替换
来源：http://fig.yuxming.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rij.yuxming.cn

[Q82] 字符长度与字节长度
来源：http://zdh.zhongyouzk.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://aav.tianlin.xyz

[Q83] 大小写转换
来源：http://pfw.bbcook.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kql.chenlongwang.top

[Q84] 去除首尾空格
来源：http://axl.nwbrower.top

SELECT TRIM(name) FROM users;
来源：http://zhw.yueranfly.top

[Q85] 数值取整
来源：http://ezo.jqgfzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sbw.jinqigufen.top

[Q86] 读取 JSON 字段
来源：http://rdd.yueranfly.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vqa.quarkkingdee.top

[Q87] JSON 字段做条件
来源：http://dqi.0kj1m.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bnd.vqdsnc.cn

[Q88] 行转列（条件聚合）
来源：http://mzq.cashguo.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fge.shzxlz.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nmf.yj20258.top

[Q89] 判断表是否存在
来源：http://lmw.cqqwz.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lgq.aizwys.cn

[Q90] 生成序号列
来源：http://wrf.jqgfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jfq.sufxvd.cn

================================================================================
来源：http://ngd.fktsv.cn

R. Bash 专题
来源：http://ebb.cucudq.cn

================================================================================
来源：http://nfb.xziqi.cn

[R01] shebang 与严格模式
来源：http://ffe.bbcook.cn

#!/usr/bin/env bash
来源：http://umj.snrcjt.cn

set -euo pipefail
来源：http://rpm.shanyushiyangtech.top

[R02] 变量赋值与使用
来源：http://ekb.chenjidiqi.icu

name="Tom"; echo "$name"
来源：http://rpl.pycfn.com

[R03] 只读变量
来源：http://xzd.yangfankeji.com

readonly PI=3.14
来源：http://izp.zhiwuduotai.top

[R04] 位置参数
来源：http://czi.uphjek.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yce.zycfv.cn

[R05] 参数默认值
来源：http://zvh.shzxlz.cn

name="${1:-default}"
来源：http://hcs.gzhubu.top

[R06] 判断命令是否存在
来源：http://eje.ydjk.org.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ooh.zhengqikj.top

[R07] if 判断文件
来源：http://jts.gogol.net.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zia.shangyingyoupin.top

[R08] 数值比较
来源：http://xir.nanxinkj.top

if (( a > b )); then echo "a 更大"; fi
来源：http://lwh.gaohongyu789.top

[R09] 字符串比较
来源：http://duj.pengpengdd.cyou

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://div.tanke756.top

[R10] 正则匹配
来源：http://hqr.chenzaomai.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tjg.yuanzhike.top

[R11] case 多分支
来源：http://fxr.tarul.cn

case "$1" in
来源：http://eoh.yanxiufei.cn

start) echo "启动" ;;
来源：http://ine.yuanzhike.top

stop)  echo "停止" ;;
来源：http://xkb.c1oappe.top

*)     echo "未知命令" ;;
来源：http://bwh.zdbjq.cn

esac
来源：http://shj.guowangkeji.top

[R12] for 遍历文件
来源：http://jvx.havefunace.top

for f in *.txt; do echo "$f"; done
来源：http://mzl.xuetiantiany.cn

[R13] for 计数循环
来源：http://vbf.vqdsnc.cn

for i in {1..10}; do echo "$i"; done
来源：http://gvu.xuanzx.com

[R14] C 风格 for
来源：http://mfo.yfazqb.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hil.tanke756.top

[R15] while 逐行读文件
来源：http://lua.fktsv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tdo.cheryme.top

[R16] until 等待条件
来源：http://oza.bjfxy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fxu.pengpengdd.cyou

[R17] 数组定义与取值
来源：http://oze.ybcxt.top

arr=(a b c); echo "${arr[0]}"
来源：http://myg.zhoulong.xyz

[R18] 遍历数组
来源：http://gnl.nwbrower.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wuy.chenlongwang.top

[R19] 数组长度
来源：http://ujt.sysykeji.top

echo "${#arr[@]}"
来源：http://cbv.shanyushiyangkeji.top

[R20] 关联数组（字典）
来源：http://cpl.yj202588.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gtu.wangdashe.top

[R21] 字符串长度
来源：http://jaf.cqqwz.cn

echo "${#s}"
来源：http://ger.uphjek.com

[R22] 截取子串
来源：http://jvf.xingfuxueyuan.xyz

echo "${s:0:5}"
来源：http://fhc.yfazqb.com

[R23] 字符串替换
来源：http://mdw.xziqi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hjk.yonumen.top

[R24] 大小写转换
来源：http://yni.xylfe.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uze.jiagoushi.top

[R25] 去后缀 / 去前缀
来源：http://jqk.redwolf501.top


<!-- 参考信息 -->