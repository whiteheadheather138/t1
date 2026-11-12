代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://whj.yuanzhike.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://erc.9152youxi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yjn.andypj.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mum.zhaomingkeji.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mpg.shanyushiyangtech.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kax.kuanghao11.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gnp.zycfv.cn

Ruby: a == b
来源：http://orw.aibaodan.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://epf.chenjidiqi.icu

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qjq.zycfv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ysp.jinqigfzy.top

PHP:  if (empty($x)) {}
来源：http://gwk.yangfankeji.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bvh.52xcode.cn

TS:   if (x == null) {}
来源：http://zdo.nanxuanxn.top

Java: if (x == null || x.isEmpty()) {}
来源：http://cwx.jinqigfzy.top

Go:   if x == nil {}
来源：http://cwt.xinyue.icu

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lyk.tarul.cn

C#:   if (x is null) {}
来源：http://akw.gzhubu.top

[P07] 防抖与节流
来源：http://zbc.birdmap.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kdt.shanyushiyangtech.top

PHP:  // 手写时间戳比较
来源：http://mia.jyoumei.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wjv.sxryk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://akt.shuidangran.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vvt.52xcode.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cvq.cdnleiting.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://jis.chenlongwang.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fwt.yanxiufei.cn

[P08] 处理浮点精度问题
来源：http://yzi.hcnkem.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fxa.zhiwuduotai.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ejc.ydjk.org.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tbd.gogol.net.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://upb.yj202588.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wdo.yj20258888.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kui.ydjk.org.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xwo.hesvh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zjx.ydjk.org.cn

================================================================================
来源：http://tru.sufxvd.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dxm.zhiwuduotai.top

================================================================================
来源：http://pnp.zhixingplan.top

[Q01] 创建表
来源：http://woi.jinghuilouyu.cn

CREATE TABLE users (
来源：http://ykq.cashguo.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yre.hfpthk.cn

name VARCHAR(50) NOT NULL,
来源：http://yvh.jinghuilouyu.cn

email VARCHAR(100) UNIQUE,
来源：http://mpx.pycfn.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ykv.9152youxi.cn

);
来源：http://tio.yangfankeji.com

[Q02] 创建带外键的表
来源：http://cvz.9152youxi.cn

CREATE TABLE orders (
来源：http://gao.havefunace.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eyx.yj202588.top

user_id INT NOT NULL,
来源：http://vea.svipenyu.cn

amount DECIMAL(10, 2),
来源：http://tgk.fengsongda.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wbh.hammf.cn

);
来源：http://hpe.yueranfly.top

[Q03] 增加列
来源：http://lch.yangfankeji.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://woh.vehdjk.com

[Q04] 修改列类型
来源：http://uxw.jianghu66.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mkd.hesvh.cn

[Q05] 重命名列
来源：http://hcz.nanxinkj.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nyi.daria6918.cn

[Q06] 删除列
来源：http://ewz.ywan-chungtsiang.top

ALTER TABLE users DROP COLUMN age;
来源：http://sqi.xylfe.cn

[Q07] 删除表
来源：http://uit.jiagoushi.top

DROP TABLE IF EXISTS orders;
来源：http://ofl.sysykeji.top

[Q08] 创建普通索引
来源：http://rdn.birdmap.top

CREATE INDEX idx_users_email ON users(email);
来源：http://qtx.ydjk.org.cn

[Q09] 创建唯一索引
来源：http://tvy.wangdashe.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rgr.svipenyu.cn

[Q10] 插入单行
来源：http://zvk.dashuyun.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://utp.jianghu66.top

[Q11] 一次插入多行
来源：http://dol.cucudq.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://typ.jinghuilouyu.cn

[Q12] 插入后取自增 ID
来源：http://urd.sysykeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://bxy.yangfankeji.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fsp.hesvh.cn

[Q13] 忽略重复插入
来源：http://orl.ydzc1.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bcj.chenlongwang.top

[Q14] 存在则更新（upsert）
来源：http://pmu.jiagoushi.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jpf.tanke756.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lhe.aibaodan.cn

[Q15] 查询全部
来源：http://dhe.chenjidiqi.icu

SELECT * FROM users;
来源：http://zob.ybcxt.top

[Q16] 查询指定列
来源：http://neg.smart0.xyz

SELECT id, name FROM users;
来源：http://jgn.jqgufenzy.top

[Q17] 条件查询
来源：http://txi.fzhhl.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pxw.tarul.cn

[Q18] 模糊匹配
来源：http://usr.hywenlv.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qpg.yj202588.top

[Q19] 范围查询
来源：http://tho.zhongyouzk.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://efz.chenjidiqi.icu

[Q20] IN 列表
来源：http://brx.aizwys.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xjk.daxiang520.top

[Q21] 空值判断
来源：http://yvh.yj20258888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://kuc.xuetiantiany.cn

[Q22] 排序
来源：http://ygl.ctjpmb.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qxd.hammf.cn

[Q23] 分页
来源：http://fdc.xuanzx.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pxh.sufxvd.cn

[Q24] 去重
来源：http://tom.xinyue.icu

SELECT DISTINCT city FROM users;
来源：http://znf.yuanzhike.top

[Q25] 只取前 N 条
来源：http://ciw.wangdashe.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xhd.9152youxi.cn

[Q26] 计数
来源：http://ace.cdnleiting.top

SELECT COUNT(*) FROM users;
来源：http://bsi.yj20258.top

[Q27] 条件计数
来源：http://jtx.yj202588.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://toy.tianlin.xyz

[Q28] 求和与平均
来源：http://deb.tian-w.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ret.kuanghao11.cn

[Q29] 最大最小值
来源：http://vap.cdnleiting.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xtj.ywan-chungtsiang.top

[Q30] 分组统计
来源：http://wry.sxryk.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pdd.fehbvm.com

[Q31] 分组后过滤
来源：http://fjp.tianlin.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mpj.epnwcf.com

[Q32] 分组拼接字符串
来源：http://tmm.dianchejie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dvz.hcnkem.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yzi.gaohongyu789.top

[Q33] 多列分组
来源：http://kan.smart0.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://spp.zycfv.cn

[Q34] 每组取第一条
来源：http://zng.xziqi.cn

SELECT * FROM (
来源：http://jfs.jinqigufen.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pip.haohaochexian.top

) t WHERE rn = 1;
来源：http://mqk.gzhubu.top

[Q35] 内连接
来源：http://sgh.hnqzz.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xcm.nanxuanxn.top

[Q36] 左连接
来源：http://tjp.dashuyun.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hne.zhoulong.xyz

[Q37] 右连接
来源：http://drf.snrcjt.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://eci.zhongyouzk.top

[Q38] 全外连接（PostgreSQL）
来源：http://itp.uphjek.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zrk.jqgfzy.top

[Q39] 自连接（查上下级）
来源：http://eef.svipenyu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hlr.shangyingyoupin.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tcx.fehbvm.com

[Q40] 交叉连接（笛卡尔积）
来源：http://yso.fehbvm.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ljd.hongshengwenyu.top

[Q41] 多表连接
来源：http://hcj.yueranfly.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://kjq.nanxuanxn.top

JOIN users u ON u.id = o.user_id
来源：http://pir.epnwcf.com

JOIN products p ON p.id = o.product_id;
来源：http://nph.hnqzz.top

[Q42] 连接条件附加过滤
来源：http://ezb.hesvh.cn

SELECT u.name, o.amount FROM users u
来源：http://rsm.shanyushiyangtech.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ojh.52xcode.cn

[Q43] 标量子查询
来源：http://cdw.vehdjk.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mif.zhongyouzk.top

[Q44] IN 子查询
来源：http://wvs.sjlbkw.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://oys.bbcook.cn

[Q45] EXISTS 判断存在
来源：http://lhz.yfazqb.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xhd.yuxming.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rej.yangfankeji.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://skn.nanxuanxn.top

[Q47] 与平均值比较
来源：http://zhs.wangshuangyany.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yti.wangshuangyany.cn

[Q48] CTE 公用表表达式
来源：http://yzp.epnwcf.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tul.snrcjt.cn

SELECT * FROM t WHERE c > 5;
来源：http://dvg.yonumen.top

[Q49] 更新单行
来源：http://agc.zhengqikj.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mjx.aizwys.cn

[Q50] 批量更新
来源：http://dbu.gotoacloud.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mgm.svipenyu.cn

[Q51] 用子查询更新
来源：http://nfl.wangshuangyany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jsu.hammf.cn

[Q52] 删除指定行
来源：http://urz.fehbvm.com

DELETE FROM users WHERE id = 10;
来源：http://eng.zhiwuduotai.top

[Q53] 按条件删除
来源：http://gpp.jinyuanbaomall.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vrk.zdqjudy.top

[Q54] 清空表
来源：http://bvw.zhaomingkeji.xyz

TRUNCATE TABLE logs;
来源：http://abw.chenjidiqi.icu

[Q55] 排名（并列占位）
来源：http://mrq.dianchejie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sfb.cdnleiting.top

[Q56] 密集排名（并列不占位）
来源：http://lxh.sysykeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bjm.ehwqpu.com

[Q57] 行号
来源：http://rda.zhoulong.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lcx.zhijiandao.cn

[Q58] 累计求和
来源：http://wkg.jinqigfzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sjk.cashguo.top

[Q59] 分组内累计
来源：http://sah.316326.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vgp.ybcxt.top

[Q60] 取上一行 / 下一行
来源：http://vbv.hywenlv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fno.vehdjk.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cpc.fehbvm.com

[Q61] 移动平均
来源：http://nbc.zdbjq.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jsq.shzxlz.cn

[Q62] 分组占比
来源：http://ipo.yj20258888.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hza.vehdjk.com

[Q63] 开启事务
来源：http://bte.jinghuilouyu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://swv.redwolf501.top

[Q64] 提交事务
来源：http://xov.chenjidiqi.icu

COMMIT;
来源：http://abo.hongshengwenyu.top

[Q65] 回滚事务
来源：http://bwt.tian-w.cn

ROLLBACK;
来源：http://jpa.yongpay.top

[Q66] 行锁查询
来源：http://aam.gotoacloud.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://itd.dashuyun.cn

[Q67] 设置隔离级别
来源：http://sns.nwbrower.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lqa.meibo888.top

[Q68] 保存点
来源：http://nal.ivvv.top

SAVEPOINT sp1;
来源：http://djk.smart0.xyz

ROLLBACK TO sp1;
来源：http://bln.yvedp.cn

[Q69] 查看执行计划
来源：http://omv.zycfv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://prl.guowangkeji.top

[Q70] 更新统计信息
来源：http://nvq.wangdashe.top

ANALYZE TABLE users;
来源：http://wje.ctjpmb.com

[Q71] 查看建表语句
来源：http://cam.sufxvd.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ljm.fengsongda.top

[Q72] 查看索引
来源：http://izs.jinyuanbaomall.cn

SHOW INDEX FROM users;
来源：http://jrn.ybcxt.top

[Q73] 查看表状态
来源：http://dyv.gogol.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://eht.cucudq.cn

[Q74] 强制使用索引
来源：http://hgs.svipenyu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lzo.birdmap.top

[Q75] 日期格式化
来源：http://eqm.pycfn.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dws.birdmap.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vcz.vehdjk.com

[Q76] 按天统计
来源：http://emr.ywan-chungtsiang.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tbj.gotoacloud.top

[Q77] 时间加减
来源：http://yap.epnwcf.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ppe.wangshuangyany.cn

[Q78] 当前时间
来源：http://sng.jinqigfzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mbw.9152youxi.cn

[Q79] 字符串拼接
来源：http://tzl.quarkkingdee.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uqy.xziqi.cn

[Q80] 字符串截取
来源：http://hfz.cdnleiting.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://umt.chenzaomai.com

[Q81] 字符串替换
来源：http://roz.shzxlz.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://eil.yuanzhike.top

[Q82] 字符长度与字节长度
来源：http://iut.chenlongwang.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://cdf.xuanzx.com

[Q83] 大小写转换
来源：http://pmf.yuxming.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qij.birdmap.top

[Q84] 去除首尾空格
来源：http://fix.ydzc1.top

SELECT TRIM(name) FROM users;
来源：http://ath.cheryme.top

[Q85] 数值取整
来源：http://hop.jinyuanbaomall.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ihn.zycfv.cn

[Q86] 读取 JSON 字段
来源：http://yxp.sufxvd.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mnl.daria6918.cn

[Q87] JSON 字段做条件
来源：http://uek.andypj.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://scm.tarul.cn

[Q88] 行转列（条件聚合）
来源：http://gkm.jqgfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qah.chenjidiqi.icu

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rhz.svipenyu.cn

[Q89] 判断表是否存在
来源：http://dny.tarul.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jir.sweek.top

[Q90] 生成序号列
来源：http://bby.uphjek.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kcu.shanyushiyangtech.top

================================================================================
来源：http://iuj.ydzc1.top

R. Bash 专题
来源：http://yan.sweek.top

================================================================================
来源：http://cds.hywenlv.cn

[R01] shebang 与严格模式
来源：http://ltd.nwbrower.top

#!/usr/bin/env bash
来源：http://jwp.hfpthk.cn

set -euo pipefail
来源：http://bml.yuanzhike.top

[R02] 变量赋值与使用
来源：http://wkz.vehdjk.com

name="Tom"; echo "$name"
来源：http://gmm.yuxming.cn

[R03] 只读变量
来源：http://xnd.sjlbkw.cn

readonly PI=3.14
来源：http://tvf.shanyushiyangkeji.top

[R04] 位置参数
来源：http://uxw.zhoulong.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://roc.bbcook.cn

[R05] 参数默认值
来源：http://hwg.52xcode.cn

name="${1:-default}"
来源：http://blf.0kj1m.cn

[R06] 判断命令是否存在
来源：http://xnh.52xcode.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lue.sweek.top

[R07] if 判断文件
来源：http://aun.jqgfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://afc.fktsv.cn

[R08] 数值比较
来源：http://zfa.yanxiufei.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://iua.sjlbkw.cn

[R09] 字符串比较
来源：http://kob.shzxlz.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ams.smart0.xyz

[R10] 正则匹配
来源：http://mjy.shuidangran.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gqz.svipenyu.cn

[R11] case 多分支
来源：http://dlm.aizwys.cn

case "$1" in
来源：http://vwi.cheryme.top

start) echo "启动" ;;
来源：http://ika.sjlbkw.cn

stop)  echo "停止" ;;
来源：http://wdg.jlsjyb.cn

*)     echo "未知命令" ;;
来源：http://zac.jiagoushi.top

esac
来源：http://iac.52xcode.cn

[R12] for 遍历文件
来源：http://dlk.smart0.xyz

for f in *.txt; do echo "$f"; done
来源：http://nbm.jinghuilouyu.cn

[R13] for 计数循环
来源：http://rax.yj202588.top

for i in {1..10}; do echo "$i"; done
来源：http://ivx.chenjidiqi.icu

[R14] C 风格 for
来源：http://qnx.jlsjyb.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gtz.fanxiaobao.xyz

[R15] while 逐行读文件
来源：http://mds.hnxiangtu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://spa.ppjwa.cn

[R16] until 等待条件
来源：http://qgr.vqdsnc.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://muv.yfazqb.com

[R17] 数组定义与取值
来源：http://srn.jinqigufen.top

arr=(a b c); echo "${arr[0]}"
来源：http://tck.cheryme.top

[R18] 遍历数组
来源：http://moj.yonumen.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hwj.mhx1999.top

[R19] 数组长度
来源：http://ccs.nanxinkj.top

echo "${#arr[@]}"
来源：http://wzj.jlsjyb.cn

[R20] 关联数组（字典）
来源：http://qwm.ctjpmb.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rtj.ywan-chungtsiang.top

[R21] 字符串长度
来源：http://rmc.uphjek.com

echo "${#s}"
来源：http://btk.yongpay.top

[R22] 截取子串
来源：http://fsg.fanxiaobao.xyz

echo "${s:0:5}"
来源：http://knl.yongpay.top

[R23] 字符串替换
来源：http://vbs.andypj.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tzh.vehdjk.com

[R24] 大小写转换
来源：http://fyv.redwolf501.top

echo "${s^^}"; echo "${s,,}"
来源：http://arb.guannengcc.top

[R25] 去后缀 / 去前缀
来源：http://qhj.shuidangran.top


<!-- 参考信息 -->