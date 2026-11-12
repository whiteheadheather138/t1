代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://day.zhijiandao.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hmy.yfazqb.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ciw.jianghu66.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yfy.sysykeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rgt.yueranfly.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dqg.cucudq.cn

Go:   reflect.DeepEqual(a, b)
来源：http://epz.daria6918.cn

Ruby: a == b
来源：http://tuf.jinyuanbaomall.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ufo.yanxiufei.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zjw.cucudq.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gld.mhx1999.top

PHP:  if (empty($x)) {}
来源：http://jbk.dashuyun.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://prr.ehwqpu.com

TS:   if (x == null) {}
来源：http://iwh.sysykeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://iui.ybcxt.top

Go:   if x == nil {}
来源：http://gnd.c1oappe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cgm.jlsjyb.cn

C#:   if (x is null) {}
来源：http://jfi.jinqigfzy.top

[P07] 防抖与节流
来源：http://xzd.gogol.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wue.cqqwz.cn

PHP:  // 手写时间戳比较
来源：http://cjo.vehdjk.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lmg.ydzc1.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kkf.pengpengdd.cyou

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oei.havefunace.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rog.chenzaomai.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://hkq.jyoumei.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jba.ehwqpu.com

[P08] 处理浮点精度问题
来源：http://hog.hywenlv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dhu.ctjpmb.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tbp.fehbvm.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cds.wangshuangyany.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://aox.gogol.net.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qwb.epnwcf.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://oqw.gotoacloud.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dmu.yongpay.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ztc.daxiang520.top

================================================================================
来源：http://dqa.zhiwuduotai.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zdf.zhongyouzk.top

================================================================================
来源：http://yxp.gaohongyu789.top

[Q01] 创建表
来源：http://trf.fanxiaobao.xyz

CREATE TABLE users (
来源：http://mvo.daxiang520.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lod.zhongyouzk.top

name VARCHAR(50) NOT NULL,
来源：http://wvl.zhiwuduotai.top

email VARCHAR(100) UNIQUE,
来源：http://hmu.xinyue.icu

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ojc.iojbl.cn

);
来源：http://hkw.pengpengdd.cyou

[Q02] 创建带外键的表
来源：http://nyh.fktsv.cn

CREATE TABLE orders (
来源：http://fjm.yvedp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sas.cqqwz.cn

user_id INT NOT NULL,
来源：http://ygw.pycfn.com

amount DECIMAL(10, 2),
来源：http://uno.yj20258888.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pah.yuanzhike.top

);
来源：http://ans.jinghuilouyu.cn

[Q03] 增加列
来源：http://kjl.jiagoushi.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ooy.shanyushiyangkeji.top

[Q04] 修改列类型
来源：http://wzy.guannengcc.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hpp.jqgufenzy.top

[Q05] 重命名列
来源：http://hre.yfazqb.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ubg.shuidangran.top

[Q06] 删除列
来源：http://oxn.cqqwz.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ovd.cqqwz.cn

[Q07] 删除表
来源：http://iku.hongshengwenyu.top

DROP TABLE IF EXISTS orders;
来源：http://uyl.pycfn.com

[Q08] 创建普通索引
来源：http://tzf.ydzc1.top

CREATE INDEX idx_users_email ON users(email);
来源：http://tpm.yonumen.top

[Q09] 创建唯一索引
来源：http://qfg.9152youxi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pjn.zdqjudy.top

[Q10] 插入单行
来源：http://alj.xinyue.icu

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rgq.pengpengdd.cyou

[Q11] 一次插入多行
来源：http://mzg.jyoumei.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pva.gotoacloud.top

[Q12] 插入后取自增 ID
来源：http://ptj.hywenlv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://wft.ybcxt.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ppm.316326.xyz

[Q13] 忽略重复插入
来源：http://lhg.guannengcc.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yqs.yanxiufei.cn

[Q14] 存在则更新（upsert）
来源：http://idd.hammf.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uyg.kuanghao11.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://smm.pengpengdd.cyou

[Q15] 查询全部
来源：http://yen.xuanzx.com

SELECT * FROM users;
来源：http://dqd.haohaochexian.top

[Q16] 查询指定列
来源：http://eyd.meibo888.top

SELECT id, name FROM users;
来源：http://trc.vqdsnc.cn

[Q17] 条件查询
来源：http://wxe.316326.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://arx.zdqjudy.top

[Q18] 模糊匹配
来源：http://otw.vehdjk.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mjq.redwolf501.top

[Q19] 范围查询
来源：http://dov.cucudq.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://iyt.vehdjk.com

[Q20] IN 列表
来源：http://dyv.chenjidiqi.icu

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://knx.zhongyouzk.top

[Q21] 空值判断
来源：http://snl.cheryme.top

SELECT * FROM users WHERE email IS NULL;
来源：http://syt.hywenlv.cn

[Q22] 排序
来源：http://xcb.sxryk.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wcg.ehwqpu.com

[Q23] 分页
来源：http://say.nanxuanxn.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dxa.jinqigfzy.top

[Q24] 去重
来源：http://bmj.tian-w.cn

SELECT DISTINCT city FROM users;
来源：http://ped.yuxming.cn

[Q25] 只取前 N 条
来源：http://xcz.yonumen.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rkz.redwolf501.top

[Q26] 计数
来源：http://qhs.bbcook.cn

SELECT COUNT(*) FROM users;
来源：http://vgg.shzxlz.cn

[Q27] 条件计数
来源：http://pzj.sweek.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hyg.tarul.cn

[Q28] 求和与平均
来源：http://ejc.sjlbkw.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://imt.jlsjyb.cn

[Q29] 最大最小值
来源：http://scc.yvedp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cfh.jqgfzy.top

[Q30] 分组统计
来源：http://yyg.yuanzhike.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jlf.haohaochexian.top

[Q31] 分组后过滤
来源：http://ypa.chenlongwang.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ihk.gaohongyu789.top

[Q32] 分组拼接字符串
来源：http://huq.fktsv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zdf.dianchejie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gcl.zhengqikj.top

[Q33] 多列分组
来源：http://lwd.jqgfzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jbm.redwolf501.top

[Q34] 每组取第一条
来源：http://xpy.chenlongwang.top

SELECT * FROM (
来源：http://odq.fengsongda.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zjb.shanyushiyangtech.top

) t WHERE rn = 1;
来源：http://szk.ivvv.top

[Q35] 内连接
来源：http://zqu.ydjk.org.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ddy.gzhubu.top

[Q36] 左连接
来源：http://hlb.yangfankeji.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jwe.hywenlv.cn

[Q37] 右连接
来源：http://vwt.dianchejie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wgl.tarul.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rei.daxiang520.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://itn.yonumen.top

[Q39] 自连接（查上下级）
来源：http://okx.zdqjudy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://fbd.hnqzz.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qra.havefunace.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ajd.cdnleiting.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pgq.fanxiaobao.xyz

[Q41] 多表连接
来源：http://haf.yonumen.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://aje.nwbrower.top

JOIN users u ON u.id = o.user_id
来源：http://hlo.zhijiandao.cn

JOIN products p ON p.id = o.product_id;
来源：http://moe.mhx1999.top

[Q42] 连接条件附加过滤
来源：http://bqd.fengsongda.top

SELECT u.name, o.amount FROM users u
来源：http://tpk.jyoumei.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tuj.cqqwz.cn

[Q43] 标量子查询
来源：http://sde.jqgufenzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oat.ydjk.org.cn

[Q44] IN 子查询
来源：http://ela.gogol.net.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rpd.fzhhl.top

[Q45] EXISTS 判断存在
来源：http://fwe.guowangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hsz.jlsjyb.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zao.xuanzx.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://srn.smart0.xyz

[Q47] 与平均值比较
来源：http://jkm.zhixingplan.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ncd.chenzaomai.com

[Q48] CTE 公用表表达式
来源：http://mri.hnxiangtu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kcj.shzxlz.cn

SELECT * FROM t WHERE c > 5;
来源：http://ahp.ydzc1.top

[Q49] 更新单行
来源：http://cbr.sjlbkw.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://keb.9152youxi.cn

[Q50] 批量更新
来源：http://qmc.yongpay.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dve.yvedp.cn

[Q51] 用子查询更新
来源：http://sbc.ppjwa.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://luj.yanxiufei.cn

[Q52] 删除指定行
来源：http://cmw.cdnleiting.top

DELETE FROM users WHERE id = 10;
来源：http://dht.jlsjyb.cn

[Q53] 按条件删除
来源：http://umg.wangdashe.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rcy.xylfe.cn

[Q54] 清空表
来源：http://ekj.shzxlz.cn

TRUNCATE TABLE logs;
来源：http://zht.bbcook.cn

[Q55] 排名（并列占位）
来源：http://utd.fktsv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hyg.sxryk.cn

[Q56] 密集排名（并列不占位）
来源：http://uys.meibo888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://imb.snrcjt.cn

[Q57] 行号
来源：http://lra.shanyushiyangkeji.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vzh.jianghu66.top

[Q58] 累计求和
来源：http://jfs.aizwys.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tuo.zhiwuduotai.top

[Q59] 分组内累计
来源：http://ivh.nanxinkj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uyf.gaohongyu789.top

[Q60] 取上一行 / 下一行
来源：http://juc.ehwqpu.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ttc.havefunace.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fmq.sweek.top

[Q61] 移动平均
来源：http://qly.zhengqikj.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wfj.zhongyouzk.top

[Q62] 分组占比
来源：http://qxg.smart0.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://suf.jinghuilouyu.cn

[Q63] 开启事务
来源：http://yak.zhiwuduotai.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jvf.tarul.cn

[Q64] 提交事务
来源：http://wyk.fktsv.cn

COMMIT;
来源：http://ael.haohaochexian.top

[Q65] 回滚事务
来源：http://jbh.yonumen.top

ROLLBACK;
来源：http://uug.nanxinkj.top

[Q66] 行锁查询
来源：http://yyy.shuidangran.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kzt.epnwcf.com

[Q67] 设置隔离级别
来源：http://dvs.vehdjk.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zvy.jiagoushi.top

[Q68] 保存点
来源：http://kqr.snrcjt.cn

SAVEPOINT sp1;
来源：http://plq.zhoulong.xyz

ROLLBACK TO sp1;
来源：http://nsb.bjfxy.top

[Q69] 查看执行计划
来源：http://omb.zdbjq.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://atf.fehbvm.com

[Q70] 更新统计信息
来源：http://xiv.gzhubu.top

ANALYZE TABLE users;
来源：http://djk.hcnkem.com

[Q71] 查看建表语句
来源：http://njt.yfazqb.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yji.zycfv.cn

[Q72] 查看索引
来源：http://fgn.chenjidiqi.icu

SHOW INDEX FROM users;
来源：http://xkg.feifeiyinyue.top

[Q73] 查看表状态
来源：http://cgs.hywenlv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ckk.ehwqpu.com

[Q74] 强制使用索引
来源：http://htt.gotoacloud.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://oii.jyoumei.cn

[Q75] 日期格式化
来源：http://hbv.dashuyun.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dzl.zhijiandao.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hod.tarul.cn

[Q76] 按天统计
来源：http://gft.jinqigfzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nrt.bjfxy.top

[Q77] 时间加减
来源：http://who.guannengcc.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hyz.shanyushiyangkeji.top

[Q78] 当前时间
来源：http://gnh.dianchejie.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ykn.yueranfly.top

[Q79] 字符串拼接
来源：http://fiv.gogol.net.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wwi.sjlbkw.cn

[Q80] 字符串截取
来源：http://fuz.guowangkeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rrb.ydzc1.top

[Q81] 字符串替换
来源：http://ima.hysaishi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mci.jianghu66.top

[Q82] 字符长度与字节长度
来源：http://dge.shanyushiyangtech.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yui.pengpengdd.cyou

[Q83] 大小写转换
来源：http://szb.gogol.net.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jew.daxiang520.top

[Q84] 去除首尾空格
来源：http://pfn.bjfxy.top

SELECT TRIM(name) FROM users;
来源：http://vao.hcnkem.com

[Q85] 数值取整
来源：http://frw.zhaomingkeji.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zos.9152youxi.cn

[Q86] 读取 JSON 字段
来源：http://yti.zdbjq.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wxn.aizwys.cn

[Q87] JSON 字段做条件
来源：http://hpo.hesvh.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oxn.jlsjyb.cn

[Q88] 行转列（条件聚合）
来源：http://vxe.vqdsnc.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bcx.chenjidiqi.icu

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zam.jiagoushi.top

[Q89] 判断表是否存在
来源：http://vmo.zhixingplan.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lji.haohaochexian.top

[Q90] 生成序号列
来源：http://tlk.yangfankeji.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sxp.haohaochexian.top

================================================================================
来源：http://olv.dianchejie.cn

R. Bash 专题
来源：http://cpj.jqgufenzy.top

================================================================================
来源：http://xum.jiagoushi.top

[R01] shebang 与严格模式
来源：http://sas.0kj1m.cn

#!/usr/bin/env bash
来源：http://wns.daxiang520.top

set -euo pipefail
来源：http://tsf.aizwys.cn

[R02] 变量赋值与使用
来源：http://xcq.redwolf501.top

name="Tom"; echo "$name"
来源：http://jjm.tanke756.top

[R03] 只读变量
来源：http://gpo.cqqwz.cn

readonly PI=3.14
来源：http://ayw.yongpay.top

[R04] 位置参数
来源：http://xca.zhijiandao.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jfc.yj20258888.top

[R05] 参数默认值
来源：http://iie.fanxiaobao.xyz

name="${1:-default}"
来源：http://ouc.wangshuangyany.cn

[R06] 判断命令是否存在
来源：http://izr.yfazqb.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nic.sxryk.cn

[R07] if 判断文件
来源：http://bxh.pycfn.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ajv.guowangkeji.top

[R08] 数值比较
来源：http://xry.mhx1999.top

if (( a > b )); then echo "a 更大"; fi
来源：http://tld.zhongyouzk.top

[R09] 字符串比较
来源：http://vyu.gzhubu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://eph.ybcxt.top

[R10] 正则匹配
来源：http://vio.xuanzx.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hpg.nwbrower.top

[R11] case 多分支
来源：http://uij.haohaochexian.top

case "$1" in
来源：http://mcy.yfazqb.com

start) echo "启动" ;;
来源：http://lpt.smart0.xyz

stop)  echo "停止" ;;
来源：http://tjk.zhengqikj.top

*)     echo "未知命令" ;;
来源：http://fgf.haohaochexian.top

esac
来源：http://omy.ywan-chungtsiang.top

[R12] for 遍历文件
来源：http://mvw.jinyuanbaomall.cn

for f in *.txt; do echo "$f"; done
来源：http://qsz.smart0.xyz

[R13] for 计数循环
来源：http://yma.fengsongda.top

for i in {1..10}; do echo "$i"; done
来源：http://qff.vehdjk.com

[R14] C 风格 for
来源：http://eqv.hnxiangtu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iga.hcnkem.com

[R15] while 逐行读文件
来源：http://cif.ctjpmb.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bvq.tarul.cn

[R16] until 等待条件
来源：http://mjv.guannengcc.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ebf.jqgfzy.top

[R17] 数组定义与取值
来源：http://tun.yanxiufei.cn

arr=(a b c); echo "${arr[0]}"
来源：http://aau.shangyingyoupin.top

[R18] 遍历数组
来源：http://tyl.hammf.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dru.gotoacloud.top

[R19] 数组长度
来源：http://ckg.zhongyouzk.top

echo "${#arr[@]}"
来源：http://vqd.hammf.cn

[R20] 关联数组（字典）
来源：http://oig.zhengqikj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://pzv.quarkkingdee.top

[R21] 字符串长度
来源：http://cek.jlsjyb.cn

echo "${#s}"
来源：http://ywi.cdnleiting.top

[R22] 截取子串
来源：http://ouz.cdnleiting.top

echo "${s:0:5}"
来源：http://liw.zhijiandao.cn

[R23] 字符串替换
来源：http://gkg.jianghu66.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tey.hcnkem.com

[R24] 大小写转换
来源：http://pgy.ywan-chungtsiang.top

echo "${s^^}"; echo "${s,,}"
来源：http://nez.shangyingyoupin.top

[R25] 去后缀 / 去前缀
来源：http://ggv.andypj.xyz


<!-- 参考信息 -->