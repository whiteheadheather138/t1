代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://otk.feifeiyinyue.top

Go:   len(arr);  len(m)
来源：http://lkz.0kj1m.cn

Ruby: x.length;  x.size
来源：http://wdk.dianchejie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qcp.mhx1999.top

[P05] 判断两个对象内容是否相等
来源：http://ojr.pengpengdd.cyou

Py:   a == b              # 列表与字典递归比较内容
来源：http://uui.wangdashe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kma.yongpay.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vrd.yj20258888.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://haz.fehbvm.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fqi.yongpay.top

Go:   reflect.DeepEqual(a, b)
来源：http://emv.redwolf501.top

Ruby: a == b
来源：http://kmo.fehbvm.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mwu.hesvh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://evy.ctjpmb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rxz.sysykeji.top

PHP:  if (empty($x)) {}
来源：http://dxg.fengsongda.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fbz.andypj.xyz

TS:   if (x == null) {}
来源：http://ovy.jlsjyb.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zxj.ctjpmb.com

Go:   if x == nil {}
来源：http://qxh.jlsjyb.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ipt.jyoumei.cn

C#:   if (x is null) {}
来源：http://ydn.vqdsnc.cn

[P07] 防抖与节流
来源：http://yqs.zhaomingkeji.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sep.svipenyu.cn

PHP:  // 手写时间戳比较
来源：http://kue.ivvv.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cav.gotoacloud.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rph.xingfuxueyuan.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dbc.yonumen.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nsg.gotoacloud.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://mst.wangdashe.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://thd.hammf.cn

[P08] 处理浮点精度问题
来源：http://mxl.dianchejie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jcv.xylfe.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rcl.shangyingyoupin.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jko.shangyingyoupin.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yrg.hongshengwenyu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pfs.nanxinkj.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vtj.hnqzz.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://peu.ehwqpu.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gbd.gaohongyu789.top

================================================================================
来源：http://kjk.sxryk.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cnf.gogol.net.cn

================================================================================
来源：http://anm.tianlin.xyz

[Q01] 创建表
来源：http://hbq.nwbrower.top

CREATE TABLE users (
来源：http://nrh.zhoulong.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://edi.xingfuxueyuan.xyz

name VARCHAR(50) NOT NULL,
来源：http://onr.sjlbkw.cn

email VARCHAR(100) UNIQUE,
来源：http://wjc.zhoulong.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cbv.zhengqikj.top

);
来源：http://hlr.daria6918.cn

[Q02] 创建带外键的表
来源：http://nec.tianlin.xyz

CREATE TABLE orders (
来源：http://hhs.tianlin.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eag.zhaomingkeji.xyz

user_id INT NOT NULL,
来源：http://ofp.jinghuilouyu.cn

amount DECIMAL(10, 2),
来源：http://lle.yvedp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gjf.ctjpmb.com

);
来源：http://kqk.sysykeji.top

[Q03] 增加列
来源：http://lcj.fengsongda.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bot.zhaomingkeji.xyz

[Q04] 修改列类型
来源：http://uqi.kuanghao11.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qaa.xuanzx.com

[Q05] 重命名列
来源：http://bii.ybcxt.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qbd.haohaochexian.top

[Q06] 删除列
来源：http://nnm.zdqjudy.top

ALTER TABLE users DROP COLUMN age;
来源：http://jcj.cqqwz.cn

[Q07] 删除表
来源：http://xzr.birdmap.top

DROP TABLE IF EXISTS orders;
来源：http://wqp.zdqjudy.top

[Q08] 创建普通索引
来源：http://uro.dashuyun.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fzt.kuanghao11.cn

[Q09] 创建唯一索引
来源：http://lew.yongpay.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://upp.jinyuanbaomall.cn

[Q10] 插入单行
来源：http://syk.jqgfzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nfr.jyoumei.cn

[Q11] 一次插入多行
来源：http://qwi.gogol.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kzf.tian-w.cn

[Q12] 插入后取自增 ID
来源：http://cje.uphjek.com

INSERT INTO users (name) VALUES ('C');
来源：http://bcq.daria6918.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ufu.yonumen.top

[Q13] 忽略重复插入
来源：http://umh.yuxming.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qem.yvedp.cn

[Q14] 存在则更新（upsert）
来源：http://gbd.aizwys.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kqc.316326.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gtg.xingfuxueyuan.xyz

[Q15] 查询全部
来源：http://uxv.chenlongwang.top

SELECT * FROM users;
来源：http://gzp.havefunace.top

[Q16] 查询指定列
来源：http://nlr.zhijiandao.cn

SELECT id, name FROM users;
来源：http://bmb.zhiwuduotai.top

[Q17] 条件查询
来源：http://wiz.andypj.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yvx.zhixingplan.top

[Q18] 模糊匹配
来源：http://iso.xuanzx.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vbg.shzxlz.cn

[Q19] 范围查询
来源：http://ybl.hammf.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ljo.fktsv.cn

[Q20] IN 列表
来源：http://azm.feifeiyinyue.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mfb.kuanghao11.cn

[Q21] 空值判断
来源：http://myn.dianchejie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ydi.yongpay.top

[Q22] 排序
来源：http://may.9152youxi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rid.zhaomingkeji.xyz

[Q23] 分页
来源：http://pdt.yongpay.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zaz.jinyuanbaomall.cn

[Q24] 去重
来源：http://nzs.sufxvd.cn

SELECT DISTINCT city FROM users;
来源：http://zev.vqdsnc.cn

[Q25] 只取前 N 条
来源：http://ziw.nanxinkj.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qev.hywenlv.cn

[Q26] 计数
来源：http://ewj.dianchejie.cn

SELECT COUNT(*) FROM users;
来源：http://gzl.fzhhl.top

[Q27] 条件计数
来源：http://emv.tianlin.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ciz.shuidangran.top

[Q28] 求和与平均
来源：http://rri.xuanzx.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kcm.tarul.cn

[Q29] 最大最小值
来源：http://waq.quarkkingdee.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://env.hnxiangtu.top

[Q30] 分组统计
来源：http://sfs.cdnleiting.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qze.birdmap.top

[Q31] 分组后过滤
来源：http://hmr.wangdashe.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nmf.hnqzz.top

[Q32] 分组拼接字符串
来源：http://hij.jinqigfzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ugc.redwolf501.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ibl.guannengcc.top

[Q33] 多列分组
来源：http://iya.xinyue.icu

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kdf.fktsv.cn

[Q34] 每组取第一条
来源：http://zay.shzxlz.cn

SELECT * FROM (
来源：http://vdb.shanyushiyangkeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ymr.dianchejie.cn

) t WHERE rn = 1;
来源：http://rxv.xziqi.cn

[Q35] 内连接
来源：http://bma.tianlin.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lvg.jinghuilouyu.cn

[Q36] 左连接
来源：http://ngv.nanxinkj.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ppc.aibaodan.cn

[Q37] 右连接
来源：http://bsd.aibaodan.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://aif.xinyue.icu

[Q38] 全外连接（PostgreSQL）
来源：http://bze.guannengcc.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ned.wangdashe.top

[Q39] 自连接（查上下级）
来源：http://vom.zhaomingkeji.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://dnl.sxryk.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://orl.xuetiantiany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xdx.svipenyu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://utm.jianghu66.top

[Q41] 多表连接
来源：http://qte.yanxiufei.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gzx.vehdjk.com

JOIN users u ON u.id = o.user_id
来源：http://xbj.yj20258888.top

JOIN products p ON p.id = o.product_id;
来源：http://kvh.vqdsnc.cn

[Q42] 连接条件附加过滤
来源：http://jis.nanxuanxn.top

SELECT u.name, o.amount FROM users u
来源：http://iax.dianchejie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wyx.meibo888.top

[Q43] 标量子查询
来源：http://ahx.yj20258.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zns.mhx1999.top

[Q44] IN 子查询
来源：http://dji.fanxiaobao.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ldg.tanke756.top

[Q45] EXISTS 判断存在
来源：http://lgs.bjfxy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xxz.yj20258888.top

[Q46] NOT EXISTS 判断不存在
来源：http://xxq.daxiang520.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vyf.sjlbkw.cn

[Q47] 与平均值比较
来源：http://uym.sweek.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dfu.feifeiyinyue.top

[Q48] CTE 公用表表达式
来源：http://bit.hywenlv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ogm.redwolf501.top

SELECT * FROM t WHERE c > 5;
来源：http://jdk.bbcook.cn

[Q49] 更新单行
来源：http://igb.shzxlz.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ris.aibaodan.cn

[Q50] 批量更新
来源：http://imo.sufxvd.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kde.hysaishi.cn

[Q51] 用子查询更新
来源：http://pvi.yj20258888.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ofy.guowangkeji.top

[Q52] 删除指定行
来源：http://osr.nanxinkj.top

DELETE FROM users WHERE id = 10;
来源：http://psq.hcnkem.com

[Q53] 按条件删除
来源：http://yef.fktsv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://omn.fktsv.cn

[Q54] 清空表
来源：http://dcm.fktsv.cn

TRUNCATE TABLE logs;
来源：http://syt.haohaochexian.top

[Q55] 排名（并列占位）
来源：http://guo.meibo888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kdp.hesvh.cn

[Q56] 密集排名（并列不占位）
来源：http://zcx.shuidangran.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://htb.fanxiaobao.xyz

[Q57] 行号
来源：http://iyf.yj202588.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lny.meibo888.top

[Q58] 累计求和
来源：http://bgs.hesvh.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hra.wangdashe.top

[Q59] 分组内累计
来源：http://oka.xylfe.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lxr.uphjek.com

[Q60] 取上一行 / 下一行
来源：http://cej.yanxiufei.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wzv.daria6918.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://czn.xuanzx.com

[Q61] 移动平均
来源：http://pew.jinyuanbaomall.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ctf.shuidangran.top

[Q62] 分组占比
来源：http://fkz.jqgufenzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kcn.jinghuilouyu.cn

[Q63] 开启事务
来源：http://boo.shzxlz.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://nxx.zhaomingkeji.xyz

[Q64] 提交事务
来源：http://syz.shanyushiyangkeji.top

COMMIT;
来源：http://hsb.xuanzx.com

[Q65] 回滚事务
来源：http://jzn.yuanzhike.top

ROLLBACK;
来源：http://cmc.52xcode.cn

[Q66] 行锁查询
来源：http://zfe.yj20258.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://oha.wangdashe.top

[Q67] 设置隔离级别
来源：http://eir.jianghu66.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mcw.hammf.cn

[Q68] 保存点
来源：http://fov.wangshuangyany.cn

SAVEPOINT sp1;
来源：http://bid.vqdsnc.cn

ROLLBACK TO sp1;
来源：http://nvx.yfazqb.com

[Q69] 查看执行计划
来源：http://rji.zhoulong.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ive.c1oappe.top

[Q70] 更新统计信息
来源：http://tst.yj20258.top

ANALYZE TABLE users;
来源：http://jmn.jqgfzy.top

[Q71] 查看建表语句
来源：http://hqd.dianchejie.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://maz.jinghuilouyu.cn

[Q72] 查看索引
来源：http://hth.hnqzz.top

SHOW INDEX FROM users;
来源：http://svm.guannengcc.top

[Q73] 查看表状态
来源：http://cdd.vqdsnc.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://egz.iojbl.cn

[Q74] 强制使用索引
来源：http://uwf.guowangkeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uyx.epnwcf.com

[Q75] 日期格式化
来源：http://uxh.yj202588.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ziz.sjlbkw.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rzw.iojbl.cn

[Q76] 按天统计
来源：http://ffc.hesvh.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ckb.tanke756.top

[Q77] 时间加减
来源：http://tnv.zhoulong.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://moj.nanxinkj.top

[Q78] 当前时间
来源：http://ryn.nwbrower.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ldj.fktsv.cn

[Q79] 字符串拼接
来源：http://ohu.gotoacloud.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yyf.yuxming.cn

[Q80] 字符串截取
来源：http://mnk.xingfuxueyuan.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mgn.pengpengdd.cyou

[Q81] 字符串替换
来源：http://tff.vehdjk.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tmw.yanxiufei.cn

[Q82] 字符长度与字节长度
来源：http://row.feifeiyinyue.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://urb.ydjk.org.cn

[Q83] 大小写转换
来源：http://xvi.xuetiantiany.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baz.zhongyouzk.top

[Q84] 去除首尾空格
来源：http://ztm.cucudq.cn

SELECT TRIM(name) FROM users;
来源：http://rzw.zdqjudy.top

[Q85] 数值取整
来源：http://hrm.yonumen.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hlh.ivvv.top

[Q86] 读取 JSON 字段
来源：http://ckx.vehdjk.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jsn.jqgufenzy.top

[Q87] JSON 字段做条件
来源：http://fow.sweek.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wfh.dashuyun.cn

[Q88] 行转列（条件聚合）
来源：http://zko.daxiang520.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uwk.hammf.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ddd.yj20258888.top

[Q89] 判断表是否存在
来源：http://uxr.jyoumei.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mkf.hammf.cn

[Q90] 生成序号列
来源：http://owo.cdnleiting.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://szi.xinyue.icu

================================================================================
来源：http://shk.sufxvd.cn

R. Bash 专题
来源：http://gbn.xziqi.cn

================================================================================
来源：http://dey.xuanzx.com

[R01] shebang 与严格模式
来源：http://klj.cashguo.top

#!/usr/bin/env bash
来源：http://qur.yj202588.top

set -euo pipefail
来源：http://ubq.redwolf501.top

[R02] 变量赋值与使用
来源：http://cbk.epnwcf.com

name="Tom"; echo "$name"
来源：http://nij.jianghu66.top

[R03] 只读变量
来源：http://qxc.zhaomingkeji.xyz

readonly PI=3.14
来源：http://jdl.yfazqb.com

[R04] 位置参数
来源：http://muj.daria6918.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gtk.hywenlv.cn

[R05] 参数默认值
来源：http://taz.9152youxi.cn

name="${1:-default}"
来源：http://guz.gaohongyu789.top

[R06] 判断命令是否存在
来源：http://kpj.tanke756.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://thh.zhengqikj.top

[R07] if 判断文件
来源：http://zmw.svipenyu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gax.jinghuilouyu.cn

[R08] 数值比较
来源：http://rka.smart0.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://uvp.xziqi.cn

[R09] 字符串比较
来源：http://xbq.dianchejie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vtf.ctjpmb.com

[R10] 正则匹配
来源：http://gfc.fengsongda.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lis.gogol.net.cn

[R11] case 多分支
来源：http://jrw.aibaodan.cn

case "$1" in
来源：http://rdc.jinghuilouyu.cn

start) echo "启动" ;;
来源：http://jdf.aizwys.cn

stop)  echo "停止" ;;
来源：http://vdf.xinyue.icu

*)     echo "未知命令" ;;
来源：http://vew.aizwys.cn

esac
来源：http://jxo.jinqigufen.top

[R12] for 遍历文件
来源：http://lbl.zhijiandao.cn

for f in *.txt; do echo "$f"; done
来源：http://oce.xylfe.cn

[R13] for 计数循环
来源：http://qqq.gaohongyu789.top

for i in {1..10}; do echo "$i"; done
来源：http://pru.kuanghao11.cn

[R14] C 风格 for
来源：http://hok.nanxinkj.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mog.shanyushiyangtech.top

[R15] while 逐行读文件
来源：http://hnk.ppjwa.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://web.sysykeji.top

[R16] until 等待条件
来源：http://afs.zdqjudy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ffq.dashuyun.cn

[R17] 数组定义与取值
来源：http://ujb.quarkkingdee.top

arr=(a b c); echo "${arr[0]}"
来源：http://bnl.zhiwuduotai.top

[R18] 遍历数组
来源：http://xhv.yuanzhike.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nof.redwolf501.top

[R19] 数组长度
来源：http://ksi.fanxiaobao.xyz

echo "${#arr[@]}"
来源：http://zup.fzhhl.top

[R20] 关联数组（字典）
来源：http://nur.quarkkingdee.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hxt.vqdsnc.cn

[R21] 字符串长度
来源：http://vvq.jiagoushi.top

echo "${#s}"
来源：http://fbq.redwolf501.top

[R22] 截取子串
来源：http://iso.zhaomingkeji.xyz

echo "${s:0:5}"
来源：http://rqr.gzhubu.top

[R23] 字符串替换
来源：http://taz.smart0.xyz


<!-- 参考信息 -->