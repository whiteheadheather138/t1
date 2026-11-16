代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://pnf.tian-w.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gdm.jiagoushi.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://agn.smart0.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uki.redwolf501.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nkk.fzhhl.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qwg.sysykeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://byf.jinqigfzy.top

Ruby: a == b
来源：http://ygr.zhixingplan.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hda.birdmap.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zxc.shanyushiyangtech.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rji.birdmap.top

PHP:  if (empty($x)) {}
来源：http://ijm.xuanzx.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fgl.tian-w.cn

TS:   if (x == null) {}
来源：http://mon.gaohongyu789.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ljv.shanyushiyangkeji.top

Go:   if x == nil {}
来源：http://uds.ivvv.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://awb.jqgfzy.top

C#:   if (x is null) {}
来源：http://pvz.kuanghao11.cn

[P07] 防抖与节流
来源：http://roo.zdbjq.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ivw.vqdsnc.cn

PHP:  // 手写时间戳比较
来源：http://qjx.ppjwa.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://btc.yonumen.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hil.ybcxt.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xtf.nanxuanxn.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wlu.jianghu66.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://inn.jinghuilouyu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://myi.yonumen.top

[P08] 处理浮点精度问题
来源：http://kij.chenlongwang.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uyg.sjlbkw.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pub.bjfxy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lqr.aizwys.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sxa.nanxuanxn.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yuk.zhijiandao.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://olr.mhx1999.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://too.hysaishi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nom.yj20258.top

================================================================================
来源：http://uwj.zhiwuduotai.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://esf.epnwcf.com

================================================================================
来源：http://vzb.xylfe.cn

[Q01] 创建表
来源：http://imb.316326.xyz

CREATE TABLE users (
来源：http://nzv.pengpengdd.cyou

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gsp.dianchejie.cn

name VARCHAR(50) NOT NULL,
来源：http://mbh.havefunace.top

email VARCHAR(100) UNIQUE,
来源：http://cqd.daxiang520.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ruc.zhiwuduotai.top

);
来源：http://xxk.hnxiangtu.top

[Q02] 创建带外键的表
来源：http://nsa.fengsongda.top

CREATE TABLE orders (
来源：http://gus.havefunace.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://won.tian-w.cn

user_id INT NOT NULL,
来源：http://kmd.hcnkem.com

amount DECIMAL(10, 2),
来源：http://sha.wangdashe.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pza.nwbrower.top

);
来源：http://lsu.pycfn.com

[Q03] 增加列
来源：http://jfe.fzhhl.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rqi.hfpthk.cn

[Q04] 修改列类型
来源：http://zjd.chenlongwang.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zxt.ehwqpu.com

[Q05] 重命名列
来源：http://jaj.xziqi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jfs.chenzaomai.com

[Q06] 删除列
来源：http://cvg.xylfe.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lxe.tian-w.cn

[Q07] 删除表
来源：http://epl.hfpthk.cn

DROP TABLE IF EXISTS orders;
来源：http://wqy.guannengcc.top

[Q08] 创建普通索引
来源：http://ehu.epnwcf.com

CREATE INDEX idx_users_email ON users(email);
来源：http://rep.zhiwuduotai.top

[Q09] 创建唯一索引
来源：http://bhx.sysykeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wfh.cucudq.cn

[Q10] 插入单行
来源：http://zrc.svipenyu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ewm.yvedp.cn

[Q11] 一次插入多行
来源：http://hhr.dashuyun.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xmu.shanyushiyangkeji.top

[Q12] 插入后取自增 ID
来源：http://dcx.jinghuilouyu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bgu.xziqi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sqi.jinghuilouyu.cn

[Q13] 忽略重复插入
来源：http://tzt.shzxlz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://eva.havefunace.top

[Q14] 存在则更新（upsert）
来源：http://ezo.hammf.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tuz.0kj1m.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://abg.wangdashe.top

[Q15] 查询全部
来源：http://xhj.zhoulong.xyz

SELECT * FROM users;
来源：http://xjh.havefunace.top

[Q16] 查询指定列
来源：http://gcb.zycfv.cn

SELECT id, name FROM users;
来源：http://oig.shzxlz.cn

[Q17] 条件查询
来源：http://avt.mhx1999.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ibt.chenlongwang.top

[Q18] 模糊匹配
来源：http://zxz.andypj.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xbq.52xcode.cn

[Q19] 范围查询
来源：http://rir.yj20258.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://aok.zhijiandao.cn

[Q20] IN 列表
来源：http://dbe.cashguo.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vuh.ivvv.top

[Q21] 空值判断
来源：http://ora.tianlin.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://jyg.nwbrower.top

[Q22] 排序
来源：http://dtc.pengpengdd.cyou

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dln.gogol.net.cn

[Q23] 分页
来源：http://gpk.guannengcc.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jvh.xinyue.icu

[Q24] 去重
来源：http://hxa.jqgufenzy.top

SELECT DISTINCT city FROM users;
来源：http://kjv.iojbl.cn

[Q25] 只取前 N 条
来源：http://hkj.jinqigfzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lfp.cheryme.top

[Q26] 计数
来源：http://qjq.yuxming.cn

SELECT COUNT(*) FROM users;
来源：http://ols.cashguo.top

[Q27] 条件计数
来源：http://exd.hongshengwenyu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mbn.yj20258.top

[Q28] 求和与平均
来源：http://inh.tian-w.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dvv.cheryme.top

[Q29] 最大最小值
来源：http://bwe.yanxiufei.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gsk.jqgfzy.top

[Q30] 分组统计
来源：http://izz.cashguo.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jqe.feifeiyinyue.top

[Q31] 分组后过滤
来源：http://yyd.svipenyu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zuv.sweek.top

[Q32] 分组拼接字符串
来源：http://ctg.zhijiandao.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://now.zhaomingkeji.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zth.yuxming.cn

[Q33] 多列分组
来源：http://knl.nanxuanxn.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vzi.fktsv.cn

[Q34] 每组取第一条
来源：http://whx.yangfankeji.com

SELECT * FROM (
来源：http://jwk.yonumen.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://trw.redwolf501.top

) t WHERE rn = 1;
来源：http://gzz.gaohongyu789.top

[Q35] 内连接
来源：http://zep.jinqigfzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rvd.smart0.xyz

[Q36] 左连接
来源：http://gju.yj20258888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://aso.dashuyun.cn

[Q37] 右连接
来源：http://thu.zhiwuduotai.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fvb.c1oappe.top

[Q38] 全外连接（PostgreSQL）
来源：http://dur.jinyuanbaomall.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pse.bbcook.cn

[Q39] 自连接（查上下级）
来源：http://zjz.xingfuxueyuan.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://vgi.tanke756.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://axe.xuanzx.com

[Q40] 交叉连接（笛卡尔积）
来源：http://dxo.cucudq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://npa.hfpthk.cn

[Q41] 多表连接
来源：http://xuk.xziqi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://awj.cqqwz.cn

JOIN users u ON u.id = o.user_id
来源：http://ffu.yfazqb.com

JOIN products p ON p.id = o.product_id;
来源：http://dxy.hesvh.cn

[Q42] 连接条件附加过滤
来源：http://pgv.fzhhl.top

SELECT u.name, o.amount FROM users u
来源：http://vzl.ppjwa.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://umv.fehbvm.com

[Q43] 标量子查询
来源：http://nyg.snrcjt.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://off.hywenlv.cn

[Q44] IN 子查询
来源：http://vxq.cqqwz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bot.sjlbkw.cn

[Q45] EXISTS 判断存在
来源：http://vrf.vehdjk.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zds.snrcjt.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xzw.yuanzhike.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mxf.fengsongda.top

[Q47] 与平均值比较
来源：http://lmp.gotoacloud.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kny.hongshengwenyu.top

[Q48] CTE 公用表表达式
来源：http://xih.jyoumei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gnk.yj20258.top

SELECT * FROM t WHERE c > 5;
来源：http://dzx.sysykeji.top

[Q49] 更新单行
来源：http://hkd.jqgufenzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bgd.sxryk.cn

[Q50] 批量更新
来源：http://rti.yvedp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xii.yvedp.cn

[Q51] 用子查询更新
来源：http://nqs.pengpengdd.cyou

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zvm.fanxiaobao.xyz

[Q52] 删除指定行
来源：http://xlm.ywan-chungtsiang.top

DELETE FROM users WHERE id = 10;
来源：http://tdi.yvedp.cn

[Q53] 按条件删除
来源：http://gvb.hysaishi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://djy.dianchejie.cn

[Q54] 清空表
来源：http://hof.yj202588.top

TRUNCATE TABLE logs;
来源：http://sry.epnwcf.com

[Q55] 排名（并列占位）
来源：http://nfb.xylfe.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nme.fehbvm.com

[Q56] 密集排名（并列不占位）
来源：http://wnm.shzxlz.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://log.jiagoushi.top

[Q57] 行号
来源：http://pfm.shanyushiyangkeji.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lzt.hnxiangtu.top

[Q58] 累计求和
来源：http://cha.jyoumei.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vyk.hammf.cn

[Q59] 分组内累计
来源：http://wvd.yj20258.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ovc.hcnkem.com

[Q60] 取上一行 / 下一行
来源：http://ouc.meibo888.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hgt.fehbvm.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mxf.vqdsnc.cn

[Q61] 移动平均
来源：http://fqy.xuanzx.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mco.yfazqb.com

[Q62] 分组占比
来源：http://pgl.hnxiangtu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://oze.jqgfzy.top

[Q63] 开启事务
来源：http://san.sufxvd.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://irl.shangyingyoupin.top

[Q64] 提交事务
来源：http://lrb.mhx1999.top

COMMIT;
来源：http://uzm.9152youxi.cn

[Q65] 回滚事务
来源：http://zbb.vqdsnc.cn

ROLLBACK;
来源：http://bpe.fzhhl.top

[Q66] 行锁查询
来源：http://fqa.yj202588.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xyp.hongshengwenyu.top

[Q67] 设置隔离级别
来源：http://xpl.gotoacloud.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ujf.nwbrower.top

[Q68] 保存点
来源：http://hbs.gotoacloud.top

SAVEPOINT sp1;
来源：http://cuo.gaohongyu789.top

ROLLBACK TO sp1;
来源：http://hnm.guannengcc.top

[Q69] 查看执行计划
来源：http://grn.kuanghao11.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vob.redwolf501.top

[Q70] 更新统计信息
来源：http://ptu.zhixingplan.top

ANALYZE TABLE users;
来源：http://vpo.sysykeji.top

[Q71] 查看建表语句
来源：http://afq.haohaochexian.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qje.tianlin.xyz

[Q72] 查看索引
来源：http://xnf.pycfn.com

SHOW INDEX FROM users;
来源：http://oqg.nanxinkj.top

[Q73] 查看表状态
来源：http://vfj.daxiang520.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ljw.shanyushiyangkeji.top

[Q74] 强制使用索引
来源：http://xex.feifeiyinyue.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pha.fengsongda.top

[Q75] 日期格式化
来源：http://ocn.haohaochexian.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vun.jinqigufen.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pef.0kj1m.cn

[Q76] 按天统计
来源：http://tkz.cheryme.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://umc.shanyushiyangkeji.top

[Q77] 时间加减
来源：http://qya.gotoacloud.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://aem.bbcook.cn

[Q78] 当前时间
来源：http://szl.zycfv.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://esg.zhijiandao.cn

[Q79] 字符串拼接
来源：http://wyr.jlsjyb.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qrv.xylfe.cn

[Q80] 字符串截取
来源：http://vhr.bbcook.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hjr.sjlbkw.cn

[Q81] 字符串替换
来源：http://tob.xingfuxueyuan.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://chs.meibo888.top

[Q82] 字符长度与字节长度
来源：http://wte.guannengcc.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jeo.svipenyu.cn

[Q83] 大小写转换
来源：http://txh.xuanzx.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kxh.zhongyouzk.top

[Q84] 去除首尾空格
来源：http://tun.mhx1999.top

SELECT TRIM(name) FROM users;
来源：http://rkl.xingfuxueyuan.xyz

[Q85] 数值取整
来源：http://yhb.cashguo.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nax.gogol.net.cn

[Q86] 读取 JSON 字段
来源：http://dwy.fanxiaobao.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jah.jinghuilouyu.cn

[Q87] JSON 字段做条件
来源：http://nvu.cashguo.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wtl.smart0.xyz

[Q88] 行转列（条件聚合）
来源：http://azx.andypj.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ydu.zhaomingkeji.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zhz.shanyushiyangkeji.top

[Q89] 判断表是否存在
来源：http://ngg.jiagoushi.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kne.guowangkeji.top

[Q90] 生成序号列
来源：http://uvf.dianchejie.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vwo.hesvh.cn

================================================================================
来源：http://tpx.hysaishi.cn

R. Bash 专题
来源：http://eto.pycfn.com

================================================================================
来源：http://wcu.xuanzx.com

[R01] shebang 与严格模式
来源：http://jur.ehwqpu.com

#!/usr/bin/env bash
来源：http://jhb.wangshuangyany.cn

set -euo pipefail
来源：http://ajq.jiagoushi.top

[R02] 变量赋值与使用
来源：http://yqv.jinqigfzy.top

name="Tom"; echo "$name"
来源：http://pck.nanxinkj.top

[R03] 只读变量
来源：http://ewh.dashuyun.cn

readonly PI=3.14
来源：http://kdx.zdqjudy.top

[R04] 位置参数
来源：http://rnq.daxiang520.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sfs.ppjwa.cn

[R05] 参数默认值
来源：http://edt.fzhhl.top

name="${1:-default}"
来源：http://owd.yanxiufei.cn

[R06] 判断命令是否存在
来源：http://uyk.hongshengwenyu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://juv.fzhhl.top

[R07] if 判断文件
来源：http://fnu.fanxiaobao.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://iov.xingfuxueyuan.xyz

[R08] 数值比较
来源：http://tzb.feifeiyinyue.top

if (( a > b )); then echo "a 更大"; fi
来源：http://mvy.hywenlv.cn

[R09] 字符串比较
来源：http://dza.xinyue.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jnx.meibo888.top

[R10] 正则匹配
来源：http://dnm.9152youxi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mvy.shanyushiyangkeji.top

[R11] case 多分支
来源：http://fgq.zhixingplan.top

case "$1" in
来源：http://vth.xuetiantiany.cn

start) echo "启动" ;;
来源：http://nvr.hfpthk.cn

stop)  echo "停止" ;;
来源：http://dqf.yj20258888.top

*)     echo "未知命令" ;;
来源：http://hrn.shanyushiyangkeji.top

esac
来源：http://cee.meibo888.top

[R12] for 遍历文件
来源：http://yei.tanke756.top

for f in *.txt; do echo "$f"; done
来源：http://fnh.yanxiufei.cn

[R13] for 计数循环
来源：http://pqx.zdbjq.cn

for i in {1..10}; do echo "$i"; done
来源：http://hqv.yuanzhike.top

[R14] C 风格 for
来源：http://ssa.xuanzx.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uyi.yuxming.cn

[R15] while 逐行读文件
来源：http://vdu.iojbl.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bye.jyoumei.cn

[R16] until 等待条件
来源：http://mtb.ctjpmb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fjd.guowangkeji.top

[R17] 数组定义与取值
来源：http://raj.snrcjt.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qbw.jinghuilouyu.cn

[R18] 遍历数组
来源：http://ktc.jiagoushi.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wjn.aibaodan.cn

[R19] 数组长度
来源：http://xmg.daxiang520.top

echo "${#arr[@]}"
来源：http://xeq.tian-w.cn

[R20] 关联数组（字典）
来源：http://hoa.fengsongda.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zuo.vqdsnc.cn

[R21] 字符串长度
来源：http://rda.yonumen.top

echo "${#s}"
来源：http://ryp.jinyuanbaomall.cn

[R22] 截取子串
来源：http://gwd.zhijiandao.cn

echo "${s:0:5}"
来源：http://fsn.zdqjudy.top

[R23] 字符串替换
来源：http://meu.chenjidiqi.icu

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://aro.birdmap.top

[R24] 大小写转换
来源：http://csp.aizwys.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fdm.tianlin.xyz

[R25] 去后缀 / 去前缀
来源：http://lvm.bbcook.cn


<!-- 参考信息 -->