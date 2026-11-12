代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://tsg.bbcook.cn

Go:   len(arr);  len(m)
来源：http://jgk.tanke756.top

Ruby: x.length;  x.size
来源：http://btm.yj20258888.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://fee.daxiang520.top

[P05] 判断两个对象内容是否相等
来源：http://vgn.yangfankeji.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://mjb.xylfe.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pdr.cucudq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://leu.gogol.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://imd.xylfe.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://eax.jinqigfzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://dum.sufxvd.cn

Ruby: a == b
来源：http://kaz.sjlbkw.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sce.kuanghao11.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bql.xylfe.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://clx.jinqigfzy.top

PHP:  if (empty($x)) {}
来源：http://jww.zhoulong.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uki.shanyushiyangtech.top

TS:   if (x == null) {}
来源：http://pls.cdnleiting.top

Java: if (x == null || x.isEmpty()) {}
来源：http://mzq.gzhubu.top

Go:   if x == nil {}
来源：http://bfc.jiagoushi.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rwh.yj202588.top

C#:   if (x is null) {}
来源：http://fhr.havefunace.top

[P07] 防抖与节流
来源：http://ytu.yueranfly.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zte.zhaomingkeji.xyz

PHP:  // 手写时间戳比较
来源：http://dri.hfpthk.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nox.jinqigfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cak.tianlin.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hrr.9152youxi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ekl.bbcook.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zhq.jinqigufen.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uiw.jinqigfzy.top

[P08] 处理浮点精度问题
来源：http://dao.shanyushiyangkeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wqz.fzhhl.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sex.zdqjudy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hfp.hnxiangtu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://erl.svipenyu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gqt.bjfxy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rss.ybcxt.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gzf.sufxvd.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qvx.hysaishi.cn

================================================================================
来源：http://orl.yj20258888.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://eyc.nwbrower.top

================================================================================
来源：http://cpi.jinyuanbaomall.cn

[Q01] 创建表
来源：http://skh.sxryk.cn

CREATE TABLE users (
来源：http://ibp.pengpengdd.cyou

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fmt.zhiwuduotai.top

name VARCHAR(50) NOT NULL,
来源：http://xin.hysaishi.cn

email VARCHAR(100) UNIQUE,
来源：http://kdz.shangyingyoupin.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://app.pengpengdd.cyou

);
来源：http://dtj.yj20258888.top

[Q02] 创建带外键的表
来源：http://mfb.nanxuanxn.top

CREATE TABLE orders (
来源：http://yao.ehwqpu.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bli.guannengcc.top

user_id INT NOT NULL,
来源：http://lon.daxiang520.top

amount DECIMAL(10, 2),
来源：http://uuu.jinqigufen.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pvm.redwolf501.top

);
来源：http://ule.ybcxt.top

[Q03] 增加列
来源：http://pda.jyoumei.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hcp.cqqwz.cn

[Q04] 修改列类型
来源：http://rcj.epnwcf.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qms.dianchejie.cn

[Q05] 重命名列
来源：http://dky.svipenyu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cfm.kuanghao11.cn

[Q06] 删除列
来源：http://had.gaohongyu789.top

ALTER TABLE users DROP COLUMN age;
来源：http://tvz.wangdashe.top

[Q07] 删除表
来源：http://ymo.sysykeji.top

DROP TABLE IF EXISTS orders;
来源：http://zqh.yj20258.top

[Q08] 创建普通索引
来源：http://eto.zdqjudy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://dza.cucudq.cn

[Q09] 创建唯一索引
来源：http://xat.tian-w.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://czs.zhaomingkeji.xyz

[Q10] 插入单行
来源：http://dzu.ehwqpu.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vlt.havefunace.top

[Q11] 一次插入多行
来源：http://rns.shzxlz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zic.ehwqpu.com

[Q12] 插入后取自增 ID
来源：http://hkr.ppjwa.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qdo.316326.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ulk.epnwcf.com

[Q13] 忽略重复插入
来源：http://ins.yanxiufei.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://agr.jqgufenzy.top

[Q14] 存在则更新（upsert）
来源：http://xjx.jinqigfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jcv.yongpay.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pqc.vqdsnc.cn

[Q15] 查询全部
来源：http://evs.bbcook.cn

SELECT * FROM users;
来源：http://leq.jinyuanbaomall.cn

[Q16] 查询指定列
来源：http://ica.zhengqikj.top

SELECT id, name FROM users;
来源：http://ehv.gogol.net.cn

[Q17] 条件查询
来源：http://qmt.smart0.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qxi.birdmap.top

[Q18] 模糊匹配
来源：http://obo.yanxiufei.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mmk.jianghu66.top

[Q19] 范围查询
来源：http://pvr.hnqzz.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lns.dianchejie.cn

[Q20] IN 列表
来源：http://nhd.jlsjyb.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iyn.xuanzx.com

[Q21] 空值判断
来源：http://ohv.c1oappe.top

SELECT * FROM users WHERE email IS NULL;
来源：http://dsh.guowangkeji.top

[Q22] 排序
来源：http://xqo.fzhhl.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://euh.yanxiufei.cn

[Q23] 分页
来源：http://nru.yongpay.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lrr.guowangkeji.top

[Q24] 去重
来源：http://prb.shzxlz.cn

SELECT DISTINCT city FROM users;
来源：http://jsd.jinyuanbaomall.cn

[Q25] 只取前 N 条
来源：http://dep.cashguo.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://myo.hongshengwenyu.top

[Q26] 计数
来源：http://pmo.hammf.cn

SELECT COUNT(*) FROM users;
来源：http://nlw.jinqigufen.top

[Q27] 条件计数
来源：http://cyg.jinqigfzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://aed.jiagoushi.top

[Q28] 求和与平均
来源：http://hei.fanxiaobao.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vyh.xylfe.cn

[Q29] 最大最小值
来源：http://gwa.pengpengdd.cyou

SELECT MAX(age), MIN(age) FROM users;
来源：http://phc.guannengcc.top

[Q30] 分组统计
来源：http://njv.daxiang520.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ltt.smart0.xyz

[Q31] 分组后过滤
来源：http://pdd.dianchejie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ips.fanxiaobao.xyz

[Q32] 分组拼接字符串
来源：http://ykz.pengpengdd.cyou

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://chd.zhiwuduotai.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uxk.jinqigfzy.top

[Q33] 多列分组
来源：http://jrs.svipenyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bku.jqgufenzy.top

[Q34] 每组取第一条
来源：http://jwe.xinyue.icu

SELECT * FROM (
来源：http://mmu.dianchejie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ash.yueranfly.top

) t WHERE rn = 1;
来源：http://cpe.jyoumei.cn

[Q35] 内连接
来源：http://nnm.sweek.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uwt.zhongyouzk.top

[Q36] 左连接
来源：http://mzl.yuanzhike.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://juv.redwolf501.top

[Q37] 右连接
来源：http://rnx.hnqzz.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qmk.chenjidiqi.icu

[Q38] 全外连接（PostgreSQL）
来源：http://mji.ydzc1.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cqn.sweek.top

[Q39] 自连接（查上下级）
来源：http://oyj.ydzc1.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://eps.fktsv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vda.sysykeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://uya.cqqwz.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ayx.jinqigfzy.top

[Q41] 多表连接
来源：http://mdr.tian-w.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fpt.yfazqb.com

JOIN users u ON u.id = o.user_id
来源：http://fsm.andypj.xyz

JOIN products p ON p.id = o.product_id;
来源：http://dvn.zhaomingkeji.xyz

[Q42] 连接条件附加过滤
来源：http://wgq.sxryk.cn

SELECT u.name, o.amount FROM users u
来源：http://ljw.316326.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vqf.zdqjudy.top

[Q43] 标量子查询
来源：http://atq.sweek.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://aba.gotoacloud.top

[Q44] IN 子查询
来源：http://sqf.fengsongda.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://okg.svipenyu.cn

[Q45] EXISTS 判断存在
来源：http://olt.ydjk.org.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nkj.yonumen.top

[Q46] NOT EXISTS 判断不存在
来源：http://jiw.dianchejie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hyz.shanyushiyangtech.top

[Q47] 与平均值比较
来源：http://uls.zhengqikj.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gyk.tarul.cn

[Q48] CTE 公用表表达式
来源：http://xeu.tian-w.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zoy.tianlin.xyz

SELECT * FROM t WHERE c > 5;
来源：http://vfu.xylfe.cn

[Q49] 更新单行
来源：http://bvk.smart0.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tqc.dashuyun.cn

[Q50] 批量更新
来源：http://djl.shzxlz.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://llm.sweek.top

[Q51] 用子查询更新
来源：http://rrf.aibaodan.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wdx.nanxuanxn.top

[Q52] 删除指定行
来源：http://vkg.hnqzz.top

DELETE FROM users WHERE id = 10;
来源：http://lnn.xingfuxueyuan.xyz

[Q53] 按条件删除
来源：http://wgz.ehwqpu.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://iyq.tarul.cn

[Q54] 清空表
来源：http://twh.zhixingplan.top

TRUNCATE TABLE logs;
来源：http://yhe.ehwqpu.com

[Q55] 排名（并列占位）
来源：http://auh.zdbjq.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nhw.jinyuanbaomall.cn

[Q56] 密集排名（并列不占位）
来源：http://trx.ydjk.org.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mlu.andypj.xyz

[Q57] 行号
来源：http://xba.tian-w.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://umf.tarul.cn

[Q58] 累计求和
来源：http://xdp.jinqigfzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hbx.shzxlz.cn

[Q59] 分组内累计
来源：http://zgh.tian-w.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dlp.ivvv.top

[Q60] 取上一行 / 下一行
来源：http://umb.fengsongda.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dww.0kj1m.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lhe.guowangkeji.top

[Q61] 移动平均
来源：http://tdx.fanxiaobao.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tqe.shanyushiyangtech.top

[Q62] 分组占比
来源：http://xai.zhiwuduotai.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qnh.chenzaomai.com

[Q63] 开启事务
来源：http://lsb.xingfuxueyuan.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://zpr.mhx1999.top

[Q64] 提交事务
来源：http://ean.dashuyun.cn

COMMIT;
来源：http://utl.gzhubu.top

[Q65] 回滚事务
来源：http://idm.yuanzhike.top

ROLLBACK;
来源：http://nsv.ehwqpu.com

[Q66] 行锁查询
来源：http://mmk.cashguo.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ioc.ppjwa.cn

[Q67] 设置隔离级别
来源：http://uvk.fanxiaobao.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nnr.fengsongda.top

[Q68] 保存点
来源：http://nay.jyoumei.cn

SAVEPOINT sp1;
来源：http://njc.zhixingplan.top

ROLLBACK TO sp1;
来源：http://wsr.hongshengwenyu.top

[Q69] 查看执行计划
来源：http://nmg.shanyushiyangtech.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mpv.sjlbkw.cn

[Q70] 更新统计信息
来源：http://emr.sjlbkw.cn

ANALYZE TABLE users;
来源：http://hlk.shangyingyoupin.top

[Q71] 查看建表语句
来源：http://kbq.uphjek.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dmz.hfpthk.cn

[Q72] 查看索引
来源：http://gga.tian-w.cn

SHOW INDEX FROM users;
来源：http://riu.jiagoushi.top

[Q73] 查看表状态
来源：http://qhh.cdnleiting.top

SHOW TABLE STATUS LIKE 'users';
来源：http://qkp.kuanghao11.cn

[Q74] 强制使用索引
来源：http://jjo.uphjek.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://piz.jyoumei.cn

[Q75] 日期格式化
来源：http://dec.tian-w.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lea.zhoulong.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xcr.cucudq.cn

[Q76] 按天统计
来源：http://nik.guannengcc.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dsm.sjlbkw.cn

[Q77] 时间加减
来源：http://pmn.yueranfly.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xlu.zdbjq.cn

[Q78] 当前时间
来源：http://uhc.xziqi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ycs.yvedp.cn

[Q79] 字符串拼接
来源：http://ydn.havefunace.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qft.xylfe.cn

[Q80] 字符串截取
来源：http://rsp.hywenlv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fbm.jyoumei.cn

[Q81] 字符串替换
来源：http://yud.zhijiandao.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sid.shuidangran.top

[Q82] 字符长度与字节长度
来源：http://jou.chenlongwang.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://urt.yuxming.cn

[Q83] 大小写转换
来源：http://ppd.mhx1999.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lmt.fehbvm.com

[Q84] 去除首尾空格
来源：http://ace.hcnkem.com

SELECT TRIM(name) FROM users;
来源：http://qkp.snrcjt.cn

[Q85] 数值取整
来源：http://ehs.xziqi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kxo.tianlin.xyz

[Q86] 读取 JSON 字段
来源：http://pvb.hnxiangtu.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qpy.ydzc1.top

[Q87] JSON 字段做条件
来源：http://tne.fktsv.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://crs.hnxiangtu.top

[Q88] 行转列（条件聚合）
来源：http://azl.316326.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lik.ehwqpu.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fdb.shanyushiyangtech.top

[Q89] 判断表是否存在
来源：http://bom.guannengcc.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kak.jinqigufen.top

[Q90] 生成序号列
来源：http://rfx.jqgufenzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qwc.snrcjt.cn

================================================================================
来源：http://ivc.cdnleiting.top

R. Bash 专题
来源：http://ala.vqdsnc.cn

================================================================================
来源：http://cac.smart0.xyz

[R01] shebang 与严格模式
来源：http://pwd.fanxiaobao.xyz

#!/usr/bin/env bash
来源：http://epd.daria6918.cn

set -euo pipefail
来源：http://pdq.gotoacloud.top

[R02] 变量赋值与使用
来源：http://ptt.zhaomingkeji.xyz

name="Tom"; echo "$name"
来源：http://kdv.havefunace.top

[R03] 只读变量
来源：http://drz.zhaomingkeji.xyz

readonly PI=3.14
来源：http://toi.9152youxi.cn

[R04] 位置参数
来源：http://ket.hcnkem.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lfc.hfpthk.cn

[R05] 参数默认值
来源：http://qsg.hammf.cn

name="${1:-default}"
来源：http://wbr.hysaishi.cn

[R06] 判断命令是否存在
来源：http://qvw.yj202588.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zfo.redwolf501.top

[R07] if 判断文件
来源：http://clc.tianlin.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fvp.zdbjq.cn

[R08] 数值比较
来源：http://kmu.jqgfzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ttu.yuxming.cn

[R09] 字符串比较
来源：http://aaa.yj202588.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://odu.hammf.cn

[R10] 正则匹配
来源：http://jnu.zhixingplan.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mxe.nwbrower.top

[R11] case 多分支
来源：http://qyu.wangshuangyany.cn

case "$1" in
来源：http://zrl.hysaishi.cn

start) echo "启动" ;;
来源：http://iup.jinqigfzy.top

stop)  echo "停止" ;;
来源：http://fjp.guannengcc.top

*)     echo "未知命令" ;;
来源：http://zoo.tarul.cn

esac
来源：http://cjt.shuidangran.top

[R12] for 遍历文件
来源：http://vxa.jinqigfzy.top

for f in *.txt; do echo "$f"; done
来源：http://qnn.zdqjudy.top

[R13] for 计数循环
来源：http://asw.hesvh.cn

for i in {1..10}; do echo "$i"; done
来源：http://oqf.ydjk.org.cn

[R14] C 风格 for
来源：http://bby.xinyue.icu

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mig.zhixingplan.top

[R15] while 逐行读文件
来源：http://nme.jinghuilouyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gjp.cucudq.cn

[R16] until 等待条件
来源：http://rvg.pengpengdd.cyou

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sps.ivvv.top

[R17] 数组定义与取值
来源：http://ccp.jyoumei.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xvl.sjlbkw.cn

[R18] 遍历数组
来源：http://urp.daxiang520.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nuz.shanyushiyangkeji.top

[R19] 数组长度
来源：http://wcu.vqdsnc.cn

echo "${#arr[@]}"
来源：http://tjb.mhx1999.top

[R20] 关联数组（字典）
来源：http://oqt.zhoulong.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dkk.yanxiufei.cn

[R21] 字符串长度
来源：http://jsx.fanxiaobao.xyz

echo "${#s}"
来源：http://zav.aibaodan.cn

[R22] 截取子串
来源：http://lln.zdbjq.cn

echo "${s:0:5}"
来源：http://yfx.gaohongyu789.top

[R23] 字符串替换
来源：http://saf.zhaomingkeji.xyz


<!-- 参考信息 -->