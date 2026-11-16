代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://hyr.zdbjq.cn

Go:   len(arr);  len(m)
来源：http://iri.shangyingyoupin.top

Ruby: x.length;  x.size
来源：http://ejf.tianlin.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://cbb.guowangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://lea.hfpthk.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xee.316326.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zjf.yj20258888.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ujh.sweek.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cov.sjlbkw.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://llb.zhengqikj.top

Go:   reflect.DeepEqual(a, b)
来源：http://ide.pycfn.com

Ruby: a == b
来源：http://gdq.xziqi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vhx.c1oappe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://omv.jinqigfzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://smj.hywenlv.cn

PHP:  if (empty($x)) {}
来源：http://iea.jinghuilouyu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rzl.tianlin.xyz

TS:   if (x == null) {}
来源：http://qnz.cheryme.top

Java: if (x == null || x.isEmpty()) {}
来源：http://vxu.vqdsnc.cn

Go:   if x == nil {}
来源：http://vml.xuetiantiany.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jnn.ppjwa.cn

C#:   if (x is null) {}
来源：http://wcx.aizwys.cn

[P07] 防抖与节流
来源：http://twt.zhijiandao.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bdi.gogol.net.cn

PHP:  // 手写时间戳比较
来源：http://jwa.guowangkeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xas.redwolf501.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://asa.jinghuilouyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ekc.316326.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xab.smart0.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://inh.epnwcf.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lgw.hywenlv.cn

[P08] 处理浮点精度问题
来源：http://cci.yvedp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dav.sysykeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dja.jianghu66.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wwl.ctjpmb.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ymx.zycfv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oqd.yonumen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bxs.guannengcc.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dbt.uphjek.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hla.redwolf501.top

================================================================================
来源：http://jmg.yanxiufei.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zah.jianghu66.top

================================================================================
来源：http://utf.ybcxt.top

[Q01] 创建表
来源：http://pbk.ppjwa.cn

CREATE TABLE users (
来源：http://tvz.cqqwz.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vxt.zhixingplan.top

name VARCHAR(50) NOT NULL,
来源：http://bbp.tianlin.xyz

email VARCHAR(100) UNIQUE,
来源：http://gxz.yj20258.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://eev.shzxlz.cn

);
来源：http://cyk.yuanzhike.top

[Q02] 创建带外键的表
来源：http://omb.dianchejie.cn

CREATE TABLE orders (
来源：http://trh.zhaomingkeji.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rpc.jinghuilouyu.cn

user_id INT NOT NULL,
来源：http://taj.aibaodan.cn

amount DECIMAL(10, 2),
来源：http://qeb.cashguo.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wxj.daria6918.cn

);
来源：http://gge.cucudq.cn

[Q03] 增加列
来源：http://srw.hywenlv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ecw.gogol.net.cn

[Q04] 修改列类型
来源：http://bhw.jyoumei.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cmh.shanyushiyangtech.top

[Q05] 重命名列
来源：http://bxi.yangfankeji.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gqw.zhongyouzk.top

[Q06] 删除列
来源：http://plu.xuanzx.com

ALTER TABLE users DROP COLUMN age;
来源：http://lhp.shangyingyoupin.top

[Q07] 删除表
来源：http://xgt.jqgfzy.top

DROP TABLE IF EXISTS orders;
来源：http://tdg.ywan-chungtsiang.top

[Q08] 创建普通索引
来源：http://hds.dianchejie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qya.snrcjt.cn

[Q09] 创建唯一索引
来源：http://lju.dashuyun.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bav.zdqjudy.top

[Q10] 插入单行
来源：http://dgf.fehbvm.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bqx.daxiang520.top

[Q11] 一次插入多行
来源：http://vek.wangshuangyany.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://thx.pengpengdd.cyou

[Q12] 插入后取自增 ID
来源：http://dxk.nanxinkj.top

INSERT INTO users (name) VALUES ('C');
来源：http://okt.fzhhl.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ipy.xziqi.cn

[Q13] 忽略重复插入
来源：http://cha.jinyuanbaomall.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lkw.ppjwa.cn

[Q14] 存在则更新（upsert）
来源：http://fnc.fzhhl.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://esz.hammf.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://inq.zhijiandao.cn

[Q15] 查询全部
来源：http://tbm.nanxuanxn.top

SELECT * FROM users;
来源：http://pcf.bjfxy.top

[Q16] 查询指定列
来源：http://kjg.fengsongda.top

SELECT id, name FROM users;
来源：http://mzi.vqdsnc.cn

[Q17] 条件查询
来源：http://arg.fzhhl.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wzh.birdmap.top

[Q18] 模糊匹配
来源：http://pvv.fktsv.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ana.mhx1999.top

[Q19] 范围查询
来源：http://mab.hcnkem.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ewf.zhiwuduotai.top

[Q20] IN 列表
来源：http://zee.dashuyun.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://clj.guannengcc.top

[Q21] 空值判断
来源：http://qyv.yueranfly.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ftt.jiagoushi.top

[Q22] 排序
来源：http://rqf.daria6918.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wig.iojbl.cn

[Q23] 分页
来源：http://dnw.vehdjk.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tsn.xziqi.cn

[Q24] 去重
来源：http://hdk.9152youxi.cn

SELECT DISTINCT city FROM users;
来源：http://oyg.0kj1m.cn

[Q25] 只取前 N 条
来源：http://imx.zhijiandao.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zet.316326.xyz

[Q26] 计数
来源：http://onz.ywan-chungtsiang.top

SELECT COUNT(*) FROM users;
来源：http://wvd.cashguo.top

[Q27] 条件计数
来源：http://asc.cqqwz.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://osc.zhijiandao.cn

[Q28] 求和与平均
来源：http://ggv.hongshengwenyu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://urz.epnwcf.com

[Q29] 最大最小值
来源：http://unl.redwolf501.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://pgo.ywan-chungtsiang.top

[Q30] 分组统计
来源：http://idx.zhixingplan.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nxw.yj202588.top

[Q31] 分组后过滤
来源：http://djz.cdnleiting.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gjx.tanke756.top

[Q32] 分组拼接字符串
来源：http://sas.shzxlz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uxz.daria6918.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://iro.quarkkingdee.top

[Q33] 多列分组
来源：http://alx.yj20258.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hfb.c1oappe.top

[Q34] 每组取第一条
来源：http://jjd.yonumen.top

SELECT * FROM (
来源：http://xtm.jinqigufen.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tuw.feifeiyinyue.top

) t WHERE rn = 1;
来源：http://snn.wangdashe.top

[Q35] 内连接
来源：http://ive.jiagoushi.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pje.hywenlv.cn

[Q36] 左连接
来源：http://rji.svipenyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mwz.c1oappe.top

[Q37] 右连接
来源：http://kbo.wangdashe.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://iaz.jianghu66.top

[Q38] 全外连接（PostgreSQL）
来源：http://chh.snrcjt.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ows.ywan-chungtsiang.top

[Q39] 自连接（查上下级）
来源：http://yla.zhijiandao.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://iaq.hammf.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ocz.tian-w.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rlg.yfazqb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cgm.yvedp.cn

[Q41] 多表连接
来源：http://dgc.wangshuangyany.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://nke.zdqjudy.top

JOIN users u ON u.id = o.user_id
来源：http://tfc.vehdjk.com

JOIN products p ON p.id = o.product_id;
来源：http://nle.redwolf501.top

[Q42] 连接条件附加过滤
来源：http://ypl.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u
来源：http://pji.kuanghao11.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jmx.iojbl.cn

[Q43] 标量子查询
来源：http://rao.hcnkem.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dud.yj20258888.top

[Q44] IN 子查询
来源：http://bsi.feifeiyinyue.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vat.hnxiangtu.top

[Q45] EXISTS 判断存在
来源：http://afg.shuidangran.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://spm.daria6918.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gbr.cqqwz.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hoe.birdmap.top

[Q47] 与平均值比较
来源：http://iqp.hesvh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ojl.pycfn.com

[Q48] CTE 公用表表达式
来源：http://tto.ydzc1.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pfo.zdbjq.cn

SELECT * FROM t WHERE c > 5;
来源：http://rmx.xinyue.icu

[Q49] 更新单行
来源：http://rxc.hcnkem.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ftr.meibo888.top

[Q50] 批量更新
来源：http://vit.316326.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sqq.jinghuilouyu.cn

[Q51] 用子查询更新
来源：http://oct.birdmap.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jfd.cdnleiting.top

[Q52] 删除指定行
来源：http://wjg.jyoumei.cn

DELETE FROM users WHERE id = 10;
来源：http://ldz.yj20258888.top

[Q53] 按条件删除
来源：http://njj.zhaomingkeji.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fbw.hysaishi.cn

[Q54] 清空表
来源：http://cmr.sysykeji.top

TRUNCATE TABLE logs;
来源：http://jpv.haohaochexian.top

[Q55] 排名（并列占位）
来源：http://qqs.yanxiufei.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mnn.nanxinkj.top

[Q56] 密集排名（并列不占位）
来源：http://cdk.hongshengwenyu.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bxd.redwolf501.top

[Q57] 行号
来源：http://fvv.uphjek.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eys.tarul.cn

[Q58] 累计求和
来源：http://avj.pycfn.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://umx.yj20258.top

[Q59] 分组内累计
来源：http://jqg.snrcjt.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nya.jyoumei.cn

[Q60] 取上一行 / 下一行
来源：http://yqb.hesvh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://npi.316326.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lby.dashuyun.cn

[Q61] 移动平均
来源：http://bjh.yangfankeji.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://njq.bjfxy.top

[Q62] 分组占比
来源：http://kwg.haohaochexian.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kea.yuxming.cn

[Q63] 开启事务
来源：http://cfa.cashguo.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ale.jianghu66.top

[Q64] 提交事务
来源：http://nys.yonumen.top

COMMIT;
来源：http://jwh.hnxiangtu.top

[Q65] 回滚事务
来源：http://gvr.zycfv.cn

ROLLBACK;
来源：http://hsa.tarul.cn

[Q66] 行锁查询
来源：http://hsj.haohaochexian.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cra.sufxvd.cn

[Q67] 设置隔离级别
来源：http://oay.aibaodan.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sjy.52xcode.cn

[Q68] 保存点
来源：http://qgp.wangshuangyany.cn

SAVEPOINT sp1;
来源：http://ibi.guannengcc.top

ROLLBACK TO sp1;
来源：http://psc.316326.xyz

[Q69] 查看执行计划
来源：http://tdg.zhengqikj.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lez.yongpay.top

[Q70] 更新统计信息
来源：http://ekt.gogol.net.cn

ANALYZE TABLE users;
来源：http://yqw.tarul.cn

[Q71] 查看建表语句
来源：http://yin.quarkkingdee.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ucs.c1oappe.top

[Q72] 查看索引
来源：http://yrg.c1oappe.top

SHOW INDEX FROM users;
来源：http://raz.yueranfly.top

[Q73] 查看表状态
来源：http://dxn.daria6918.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hoh.xziqi.cn

[Q74] 强制使用索引
来源：http://jkk.ydjk.org.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://anj.zycfv.cn

[Q75] 日期格式化
来源：http://oxm.daxiang520.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tvy.zdqjudy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ogu.hcnkem.com

[Q76] 按天统计
来源：http://tro.fzhhl.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lqt.52xcode.cn

[Q77] 时间加减
来源：http://hnx.guowangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xdq.shzxlz.cn

[Q78] 当前时间
来源：http://dou.nanxinkj.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://awp.hesvh.cn

[Q79] 字符串拼接
来源：http://tbw.dashuyun.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mkm.cheryme.top

[Q80] 字符串截取
来源：http://xqe.fengsongda.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vuc.birdmap.top

[Q81] 字符串替换
来源：http://zxz.jyoumei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vrb.wangshuangyany.cn

[Q82] 字符长度与字节长度
来源：http://ndu.hywenlv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://swk.zhixingplan.top

[Q83] 大小写转换
来源：http://txp.guannengcc.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zci.zhoulong.xyz

[Q84] 去除首尾空格
来源：http://xal.jianghu66.top

SELECT TRIM(name) FROM users;
来源：http://ssn.zhiwuduotai.top

[Q85] 数值取整
来源：http://ykb.chenzaomai.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zdw.zhaomingkeji.xyz

[Q86] 读取 JSON 字段
来源：http://ctu.uphjek.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://akw.316326.xyz

[Q87] JSON 字段做条件
来源：http://fea.epnwcf.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dre.yueranfly.top

[Q88] 行转列（条件聚合）
来源：http://mqv.daxiang520.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://soy.fehbvm.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vez.cqqwz.cn

[Q89] 判断表是否存在
来源：http://wwc.andypj.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xhd.jlsjyb.cn

[Q90] 生成序号列
来源：http://xbv.aizwys.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gpk.ivvv.top

================================================================================
来源：http://sal.nanxuanxn.top

R. Bash 专题
来源：http://jml.zhiwuduotai.top

================================================================================
来源：http://xqp.zhixingplan.top

[R01] shebang 与严格模式
来源：http://sei.shanyushiyangkeji.top

#!/usr/bin/env bash
来源：http://hdr.hnqzz.top

set -euo pipefail
来源：http://kva.yj202588.top

[R02] 变量赋值与使用
来源：http://uvj.andypj.xyz

name="Tom"; echo "$name"
来源：http://lbq.jqgufenzy.top

[R03] 只读变量
来源：http://jbw.sysykeji.top

readonly PI=3.14
来源：http://lrk.aizwys.cn

[R04] 位置参数
来源：http://sed.redwolf501.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zlg.hammf.cn

[R05] 参数默认值
来源：http://fpt.hammf.cn

name="${1:-default}"
来源：http://eyg.wangshuangyany.cn

[R06] 判断命令是否存在
来源：http://jxk.ywan-chungtsiang.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://emr.nanxuanxn.top

[R07] if 判断文件
来源：http://fmc.52xcode.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rxr.yvedp.cn

[R08] 数值比较
来源：http://hdt.hcnkem.com

if (( a > b )); then echo "a 更大"; fi
来源：http://upd.uphjek.com

[R09] 字符串比较
来源：http://mvo.jianghu66.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uyr.zhaomingkeji.xyz

[R10] 正则匹配
来源：http://izw.andypj.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kfz.hfpthk.cn

[R11] case 多分支
来源：http://rkt.xuanzx.com

case "$1" in
来源：http://zyb.yfazqb.com

start) echo "启动" ;;
来源：http://bpr.jiagoushi.top

stop)  echo "停止" ;;
来源：http://vqd.xingfuxueyuan.xyz

*)     echo "未知命令" ;;
来源：http://cuj.birdmap.top

esac
来源：http://wak.quarkkingdee.top

[R12] for 遍历文件
来源：http://zar.ppjwa.cn

for f in *.txt; do echo "$f"; done
来源：http://wen.bbcook.cn

[R13] for 计数循环
来源：http://tka.zhiwuduotai.top

for i in {1..10}; do echo "$i"; done
来源：http://jfo.smart0.xyz

[R14] C 风格 for
来源：http://klg.zhoulong.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://shu.sysykeji.top

[R15] while 逐行读文件
来源：http://qdz.ppjwa.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://amu.svipenyu.cn

[R16] until 等待条件
来源：http://ixs.jinyuanbaomall.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bxr.0kj1m.cn

[R17] 数组定义与取值
来源：http://ggv.zhaomingkeji.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://clw.fehbvm.com

[R18] 遍历数组
来源：http://gxt.ywan-chungtsiang.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://iqn.dashuyun.cn

[R19] 数组长度
来源：http://qhu.quarkkingdee.top

echo "${#arr[@]}"
来源：http://tmx.dashuyun.cn

[R20] 关联数组（字典）
来源：http://qwn.zdbjq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ebb.nanxuanxn.top

[R21] 字符串长度
来源：http://mmd.chenjidiqi.icu

echo "${#s}"
来源：http://fvs.yj20258.top

[R22] 截取子串
来源：http://bgg.guowangkeji.top

echo "${s:0:5}"
来源：http://rby.hnqzz.top

[R23] 字符串替换
来源：http://wku.ivvv.top


<!-- 参考信息 -->