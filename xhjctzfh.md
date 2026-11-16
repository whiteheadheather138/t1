代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://mru.zdbjq.cn

Go:   len(arr);  len(m)
来源：http://xkw.tian-w.cn

Ruby: x.length;  x.size
来源：http://ghi.zhongyouzk.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jtw.vehdjk.com

[P05] 判断两个对象内容是否相等
来源：http://ogb.yvedp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fll.shuidangran.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fqp.ydzc1.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cpo.jyoumei.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mpv.jiagoushi.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://igv.vqdsnc.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kzr.jqgufenzy.top

Ruby: a == b
来源：http://xhs.hcnkem.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uld.meibo888.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tfw.havefunace.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nwm.fanxiaobao.xyz

PHP:  if (empty($x)) {}
来源：http://uyj.xinyue.icu

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jyf.smart0.xyz

TS:   if (x == null) {}
来源：http://sjg.kuanghao11.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://awf.shanyushiyangtech.top

Go:   if x == nil {}
来源：http://dkr.wangshuangyany.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eew.hammf.cn

C#:   if (x is null) {}
来源：http://rzb.shanyushiyangkeji.top

[P07] 防抖与节流
来源：http://zbi.zdbjq.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sjq.ivvv.top

PHP:  // 手写时间戳比较
来源：http://qzo.cucudq.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vnx.yj20258.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wwa.sxryk.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xod.havefunace.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xeh.hesvh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://iqo.yanxiufei.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mei.yj202588.top

[P08] 处理浮点精度问题
来源：http://rcc.ehwqpu.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kme.yangfankeji.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qtr.gogol.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pqa.guannengcc.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ocg.jqgfzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bwj.yongpay.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ekj.mhx1999.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ndp.guannengcc.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nic.snrcjt.cn

================================================================================
来源：http://try.bbcook.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fve.zhaomingkeji.xyz

================================================================================
来源：http://bqb.gaohongyu789.top

[Q01] 创建表
来源：http://esg.hfpthk.cn

CREATE TABLE users (
来源：http://opc.c1oappe.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hyb.jianghu66.top

name VARCHAR(50) NOT NULL,
来源：http://ktg.hammf.cn

email VARCHAR(100) UNIQUE,
来源：http://fan.gzhubu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rwd.sjlbkw.cn

);
来源：http://flj.birdmap.top

[Q02] 创建带外键的表
来源：http://aus.feifeiyinyue.top

CREATE TABLE orders (
来源：http://ios.hfpthk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ujw.hnxiangtu.top

user_id INT NOT NULL,
来源：http://bzw.epnwcf.com

amount DECIMAL(10, 2),
来源：http://ile.ydzc1.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://puf.zhixingplan.top

);
来源：http://sri.yongpay.top

[Q03] 增加列
来源：http://hqg.yj20258888.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sgz.cdnleiting.top

[Q04] 修改列类型
来源：http://wkl.hywenlv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://elo.zhongyouzk.top

[Q05] 重命名列
来源：http://ojh.mhx1999.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nif.vqdsnc.cn

[Q06] 删除列
来源：http://axb.0kj1m.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qrf.sweek.top

[Q07] 删除表
来源：http://qft.snrcjt.cn

DROP TABLE IF EXISTS orders;
来源：http://haz.ctjpmb.com

[Q08] 创建普通索引
来源：http://bie.yueranfly.top

CREATE INDEX idx_users_email ON users(email);
来源：http://yfw.zhoulong.xyz

[Q09] 创建唯一索引
来源：http://tnq.ydzc1.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vtj.sjlbkw.cn

[Q10] 插入单行
来源：http://oip.wangshuangyany.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://czm.zdqjudy.top

[Q11] 一次插入多行
来源：http://gpw.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pcw.cucudq.cn

[Q12] 插入后取自增 ID
来源：http://tdj.nwbrower.top

INSERT INTO users (name) VALUES ('C');
来源：http://jcj.uphjek.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gvx.chenlongwang.top

[Q13] 忽略重复插入
来源：http://kee.ywan-chungtsiang.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ujb.chenzaomai.com

[Q14] 存在则更新（upsert）
来源：http://aqx.zdqjudy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://khg.fktsv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rsq.gogol.net.cn

[Q15] 查询全部
来源：http://xnw.hysaishi.cn

SELECT * FROM users;
来源：http://rbg.cheryme.top

[Q16] 查询指定列
来源：http://sti.nanxuanxn.top

SELECT id, name FROM users;
来源：http://bwa.yangfankeji.com

[Q17] 条件查询
来源：http://kde.havefunace.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baz.haohaochexian.top

[Q18] 模糊匹配
来源：http://bon.gzhubu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lmo.yongpay.top

[Q19] 范围查询
来源：http://fsk.cqqwz.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gsd.iojbl.cn

[Q20] IN 列表
来源：http://vxs.fengsongda.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xvf.jianghu66.top

[Q21] 空值判断
来源：http://xpq.zhixingplan.top

SELECT * FROM users WHERE email IS NULL;
来源：http://yol.uphjek.com

[Q22] 排序
来源：http://ddv.xziqi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wga.yj202588.top

[Q23] 分页
来源：http://qky.xziqi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zhc.ybcxt.top

[Q24] 去重
来源：http://bti.vehdjk.com

SELECT DISTINCT city FROM users;
来源：http://qcb.feifeiyinyue.top

[Q25] 只取前 N 条
来源：http://egz.xinyue.icu

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gkw.gogol.net.cn

[Q26] 计数
来源：http://ewg.yongpay.top

SELECT COUNT(*) FROM users;
来源：http://kja.tanke756.top

[Q27] 条件计数
来源：http://gsp.quarkkingdee.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lbm.sxryk.cn

[Q28] 求和与平均
来源：http://dua.bbcook.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://aaa.yj20258888.top

[Q29] 最大最小值
来源：http://sps.ywan-chungtsiang.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://wen.yj20258888.top

[Q30] 分组统计
来源：http://zkb.ywan-chungtsiang.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vnd.aibaodan.cn

[Q31] 分组后过滤
来源：http://hwe.havefunace.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ckr.guowangkeji.top

[Q32] 分组拼接字符串
来源：http://mtq.andypj.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fuu.yanxiufei.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kww.zhongyouzk.top

[Q33] 多列分组
来源：http://tuc.jinghuilouyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uae.daria6918.cn

[Q34] 每组取第一条
来源：http://fzg.zhongyouzk.top

SELECT * FROM (
来源：http://aki.ppjwa.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ceu.daria6918.cn

) t WHERE rn = 1;
来源：http://alv.tian-w.cn

[Q35] 内连接
来源：http://ogg.yuanzhike.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ylh.hammf.cn

[Q36] 左连接
来源：http://lya.zhixingplan.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ywc.c1oappe.top

[Q37] 右连接
来源：http://yoy.zhixingplan.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mdv.jlsjyb.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lvk.yvedp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xqf.shzxlz.cn

[Q39] 自连接（查上下级）
来源：http://sla.jiagoushi.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://byk.feifeiyinyue.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://isd.vqdsnc.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ouh.zhengqikj.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lpb.iojbl.cn

[Q41] 多表连接
来源：http://yei.yj20258.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://afp.cqqwz.cn

JOIN users u ON u.id = o.user_id
来源：http://yjs.xinyue.icu

JOIN products p ON p.id = o.product_id;
来源：http://jal.xingfuxueyuan.xyz

[Q42] 连接条件附加过滤
来源：http://gfz.iojbl.cn

SELECT u.name, o.amount FROM users u
来源：http://tcl.ctjpmb.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://foz.yvedp.cn

[Q43] 标量子查询
来源：http://zxx.pycfn.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wjn.nwbrower.top

[Q44] IN 子查询
来源：http://hbe.0kj1m.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yka.gzhubu.top

[Q45] EXISTS 判断存在
来源：http://yjw.yvedp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://grr.zhongyouzk.top

[Q46] NOT EXISTS 判断不存在
来源：http://adz.yongpay.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://olg.sjlbkw.cn

[Q47] 与平均值比较
来源：http://bnd.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ece.jyoumei.cn

[Q48] CTE 公用表表达式
来源：http://ayg.jlsjyb.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rht.yangfankeji.com

SELECT * FROM t WHERE c > 5;
来源：http://hmw.zycfv.cn

[Q49] 更新单行
来源：http://dhy.zhoulong.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nzr.ydzc1.top

[Q50] 批量更新
来源：http://tbm.chenjidiqi.icu

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mjo.zdbjq.cn

[Q51] 用子查询更新
来源：http://ckf.yuanzhike.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://koo.bbcook.cn

[Q52] 删除指定行
来源：http://alu.316326.xyz

DELETE FROM users WHERE id = 10;
来源：http://pwt.epnwcf.com

[Q53] 按条件删除
来源：http://hai.ybcxt.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nbm.shanyushiyangtech.top

[Q54] 清空表
来源：http://pfw.ybcxt.top

TRUNCATE TABLE logs;
来源：http://nox.xuanzx.com

[Q55] 排名（并列占位）
来源：http://vei.cqqwz.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cxb.jlsjyb.cn

[Q56] 密集排名（并列不占位）
来源：http://tcm.zhaomingkeji.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pvp.aibaodan.cn

[Q57] 行号
来源：http://olz.hfpthk.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ssu.yuxming.cn

[Q58] 累计求和
来源：http://rfg.shzxlz.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xgl.meibo888.top

[Q59] 分组内累计
来源：http://uzg.zhaomingkeji.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://chj.0kj1m.cn

[Q60] 取上一行 / 下一行
来源：http://ukp.jqgfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zdk.cheryme.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vyi.jyoumei.cn

[Q61] 移动平均
来源：http://lyr.fengsongda.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oko.wangshuangyany.cn

[Q62] 分组占比
来源：http://mbj.ydjk.org.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tqk.hammf.cn

[Q63] 开启事务
来源：http://unw.yj20258.top

START TRANSACTION;                -- 或 BEGIN
来源：http://pgw.gotoacloud.top

[Q64] 提交事务
来源：http://ury.nanxinkj.top

COMMIT;
来源：http://mxf.tanke756.top

[Q65] 回滚事务
来源：http://fwv.yvedp.cn

ROLLBACK;
来源：http://zcy.tian-w.cn

[Q66] 行锁查询
来源：http://ngv.fehbvm.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kud.vqdsnc.cn

[Q67] 设置隔离级别
来源：http://rps.cqqwz.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://eqm.hongshengwenyu.top

[Q68] 保存点
来源：http://jew.iojbl.cn

SAVEPOINT sp1;
来源：http://gxy.zhixingplan.top

ROLLBACK TO sp1;
来源：http://jgq.jinqigufen.top

[Q69] 查看执行计划
来源：http://vrv.jinyuanbaomall.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://loq.yj202588.top

[Q70] 更新统计信息
来源：http://sqb.tianlin.xyz

ANALYZE TABLE users;
来源：http://cck.xinyue.icu

[Q71] 查看建表语句
来源：http://tuq.0kj1m.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jpe.zhongyouzk.top

[Q72] 查看索引
来源：http://cda.chenzaomai.com

SHOW INDEX FROM users;
来源：http://ced.hammf.cn

[Q73] 查看表状态
来源：http://gqu.cheryme.top

SHOW TABLE STATUS LIKE 'users';
来源：http://npp.zdbjq.cn

[Q74] 强制使用索引
来源：http://ssy.sjlbkw.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rxf.chenzaomai.com

[Q75] 日期格式化
来源：http://gbb.hnqzz.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nws.zhijiandao.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ewr.quarkkingdee.top

[Q76] 按天统计
来源：http://tim.xuetiantiany.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hvq.pycfn.com

[Q77] 时间加减
来源：http://wwf.nanxuanxn.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://emy.hammf.cn

[Q78] 当前时间
来源：http://tdp.xuetiantiany.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tny.sufxvd.cn

[Q79] 字符串拼接
来源：http://jit.jinyuanbaomall.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://civ.sufxvd.cn

[Q80] 字符串截取
来源：http://mxj.cheryme.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jao.gaohongyu789.top

[Q81] 字符串替换
来源：http://nml.jianghu66.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yga.jiagoushi.top

[Q82] 字符长度与字节长度
来源：http://nhw.zycfv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://set.zycfv.cn

[Q83] 大小写转换
来源：http://jvn.haohaochexian.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pyc.sxryk.cn

[Q84] 去除首尾空格
来源：http://zmm.dianchejie.cn

SELECT TRIM(name) FROM users;
来源：http://fls.ppjwa.cn

[Q85] 数值取整
来源：http://uwg.yj202588.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rkt.mhx1999.top

[Q86] 读取 JSON 字段
来源：http://ued.yongpay.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rul.gaohongyu789.top

[Q87] JSON 字段做条件
来源：http://zjw.zhiwuduotai.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eon.yuxming.cn

[Q88] 行转列（条件聚合）
来源：http://uzv.nwbrower.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wvw.guowangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vdd.feifeiyinyue.top

[Q89] 判断表是否存在
来源：http://vis.hnqzz.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xvj.sxryk.cn

[Q90] 生成序号列
来源：http://hzn.zhoulong.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gkf.zdbjq.cn

================================================================================
来源：http://ltg.yangfankeji.com

R. Bash 专题
来源：http://oxb.gotoacloud.top

================================================================================
来源：http://tcf.cashguo.top

[R01] shebang 与严格模式
来源：http://fcv.jianghu66.top

#!/usr/bin/env bash
来源：http://lbt.nanxinkj.top

set -euo pipefail
来源：http://dlf.zhongyouzk.top

[R02] 变量赋值与使用
来源：http://zgq.ydzc1.top

name="Tom"; echo "$name"
来源：http://dyz.gotoacloud.top

[R03] 只读变量
来源：http://gyp.yueranfly.top

readonly PI=3.14
来源：http://wzf.cheryme.top

[R04] 位置参数
来源：http://gzh.fktsv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wju.nanxinkj.top

[R05] 参数默认值
来源：http://xby.chenlongwang.top

name="${1:-default}"
来源：http://pmp.jyoumei.cn

[R06] 判断命令是否存在
来源：http://ihi.gzhubu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wgc.uphjek.com

[R07] if 判断文件
来源：http://ahc.yuxming.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://oho.hongshengwenyu.top

[R08] 数值比较
来源：http://dex.yj20258888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://eqh.birdmap.top

[R09] 字符串比较
来源：http://jiu.epnwcf.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mks.guannengcc.top

[R10] 正则匹配
来源：http://fyg.uphjek.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mzv.zhongyouzk.top

[R11] case 多分支
来源：http://fsa.xuetiantiany.cn

case "$1" in
来源：http://bdh.chenlongwang.top

start) echo "启动" ;;
来源：http://xhn.gogol.net.cn

stop)  echo "停止" ;;
来源：http://xrt.jinyuanbaomall.cn

*)     echo "未知命令" ;;
来源：http://imd.yangfankeji.com

esac
来源：http://lps.zhaomingkeji.xyz

[R12] for 遍历文件
来源：http://omc.zhengqikj.top

for f in *.txt; do echo "$f"; done
来源：http://ygm.tian-w.cn

[R13] for 计数循环
来源：http://dil.dashuyun.cn

for i in {1..10}; do echo "$i"; done
来源：http://ypt.jlsjyb.cn

[R14] C 风格 for
来源：http://zog.tian-w.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://aru.xuetiantiany.cn

[R15] while 逐行读文件
来源：http://rit.dashuyun.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://aee.ctjpmb.com

[R16] until 等待条件
来源：http://wxj.iojbl.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ijn.zdqjudy.top

[R17] 数组定义与取值
来源：http://gxg.cheryme.top

arr=(a b c); echo "${arr[0]}"
来源：http://cdm.guannengcc.top

[R18] 遍历数组
来源：http://ptz.jyoumei.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dkl.gaohongyu789.top

[R19] 数组长度
来源：http://eju.daria6918.cn

echo "${#arr[@]}"
来源：http://ani.daxiang520.top

[R20] 关联数组（字典）
来源：http://kut.vehdjk.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gyg.cqqwz.cn

[R21] 字符串长度
来源：http://jrf.zhiwuduotai.top

echo "${#s}"
来源：http://vuo.jlsjyb.cn

[R22] 截取子串
来源：http://mxe.jqgfzy.top

echo "${s:0:5}"
来源：http://bld.hywenlv.cn

[R23] 字符串替换
来源：http://usj.svipenyu.cn


<!-- 参考信息 -->