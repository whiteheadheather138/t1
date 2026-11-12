代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://vtw.shanyushiyangtech.top

Go:   len(arr);  len(m)
来源：http://cxo.zdqjudy.top

Ruby: x.length;  x.size
来源：http://dkp.guowangkeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ajq.zdbjq.cn

[P05] 判断两个对象内容是否相等
来源：http://nok.haohaochexian.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://dmp.c1oappe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kjm.tianlin.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qtr.shuidangran.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ous.yj20258.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nej.cheryme.top

Go:   reflect.DeepEqual(a, b)
来源：http://jwn.yonumen.top

Ruby: a == b
来源：http://oyq.hywenlv.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vxh.shanyushiyangtech.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://muz.ivvv.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://aws.ywan-chungtsiang.top

PHP:  if (empty($x)) {}
来源：http://ead.ivvv.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uwz.jianghu66.top

TS:   if (x == null) {}
来源：http://uzt.sxryk.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qzk.chenlongwang.top

Go:   if x == nil {}
来源：http://kjv.xinyue.icu

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vmr.xuetiantiany.cn

C#:   if (x is null) {}
来源：http://aax.shanyushiyangkeji.top

[P07] 防抖与节流
来源：http://ntp.yj20258888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hew.nwbrower.top

PHP:  // 手写时间戳比较
来源：http://upd.xinyue.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ghx.tanke756.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cvr.ivvv.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wpi.jqgfzy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bxh.hnqzz.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ami.feifeiyinyue.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cqw.hywenlv.cn

[P08] 处理浮点精度问题
来源：http://jzr.sweek.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jsx.jinqigfzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ebg.gogol.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qqr.wangdashe.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cpr.yj20258888.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zhm.jqgfzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wwu.gzhubu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ixl.kuanghao11.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fqr.tarul.cn

================================================================================
来源：http://efm.zhaomingkeji.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bcz.zhaomingkeji.xyz

================================================================================
来源：http://fym.sjlbkw.cn

[Q01] 创建表
来源：http://sxk.yvedp.cn

CREATE TABLE users (
来源：http://xrz.c1oappe.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://erw.yvedp.cn

name VARCHAR(50) NOT NULL,
来源：http://kfh.cqqwz.cn

email VARCHAR(100) UNIQUE,
来源：http://hpz.kuanghao11.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xnt.sweek.top

);
来源：http://rkh.sufxvd.cn

[Q02] 创建带外键的表
来源：http://wcc.ybcxt.top

CREATE TABLE orders (
来源：http://ltv.hongshengwenyu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://anc.sxryk.cn

user_id INT NOT NULL,
来源：http://dck.wangshuangyany.cn

amount DECIMAL(10, 2),
来源：http://fom.cqqwz.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ewu.hesvh.cn

);
来源：http://yci.zhengqikj.top

[Q03] 增加列
来源：http://lny.zhixingplan.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bqt.c1oappe.top

[Q04] 修改列类型
来源：http://cju.9152youxi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vfl.fengsongda.top

[Q05] 重命名列
来源：http://rfv.zhiwuduotai.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kjt.havefunace.top

[Q06] 删除列
来源：http://hhw.cqqwz.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cwh.guowangkeji.top

[Q07] 删除表
来源：http://dts.quarkkingdee.top

DROP TABLE IF EXISTS orders;
来源：http://plu.sysykeji.top

[Q08] 创建普通索引
来源：http://xbc.fengsongda.top

CREATE INDEX idx_users_email ON users(email);
来源：http://owm.gzhubu.top

[Q09] 创建唯一索引
来源：http://mfn.zhiwuduotai.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bzm.shzxlz.cn

[Q10] 插入单行
来源：http://yig.hongshengwenyu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fay.yuanzhike.top

[Q11] 一次插入多行
来源：http://cbt.ydzc1.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pwn.andypj.xyz

[Q12] 插入后取自增 ID
来源：http://ovs.sufxvd.cn

INSERT INTO users (name) VALUES ('C');
来源：http://kiu.meibo888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ryx.birdmap.top

[Q13] 忽略重复插入
来源：http://mpj.cashguo.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gpl.pycfn.com

[Q14] 存在则更新（upsert）
来源：http://cpy.quarkkingdee.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vsw.zycfv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sqg.xuanzx.com

[Q15] 查询全部
来源：http://lod.daria6918.cn

SELECT * FROM users;
来源：http://ehr.9152youxi.cn

[Q16] 查询指定列
来源：http://hfp.cashguo.top

SELECT id, name FROM users;
来源：http://wka.cashguo.top

[Q17] 条件查询
来源：http://ctt.zycfv.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ahh.cheryme.top

[Q18] 模糊匹配
来源：http://vig.yuanzhike.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wpc.fktsv.cn

[Q19] 范围查询
来源：http://uls.tian-w.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fyi.yangfankeji.com

[Q20] IN 列表
来源：http://dah.jinqigfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://exp.sweek.top

[Q21] 空值判断
来源：http://ppq.daria6918.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://glp.jinqigfzy.top

[Q22] 排序
来源：http://oci.xinyue.icu

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vsn.nanxuanxn.top

[Q23] 分页
来源：http://maz.ydjk.org.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xtw.yueranfly.top

[Q24] 去重
来源：http://hir.jinqigufen.top

SELECT DISTINCT city FROM users;
来源：http://xrx.haohaochexian.top

[Q25] 只取前 N 条
来源：http://pxk.hammf.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ebx.vqdsnc.cn

[Q26] 计数
来源：http://caq.hesvh.cn

SELECT COUNT(*) FROM users;
来源：http://xsh.vehdjk.com

[Q27] 条件计数
来源：http://qdu.guannengcc.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qty.bbcook.cn

[Q28] 求和与平均
来源：http://yiu.shzxlz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qzk.chenlongwang.top

[Q29] 最大最小值
来源：http://kze.cashguo.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://akp.shangyingyoupin.top

[Q30] 分组统计
来源：http://xkn.gzhubu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://quq.bjfxy.top

[Q31] 分组后过滤
来源：http://mdb.iojbl.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ysv.haohaochexian.top

[Q32] 分组拼接字符串
来源：http://znw.yvedp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rtj.jinqigfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ozt.zhijiandao.cn

[Q33] 多列分组
来源：http://lwb.sufxvd.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ehk.fehbvm.com

[Q34] 每组取第一条
来源：http://ljj.hesvh.cn

SELECT * FROM (
来源：http://sqd.wangshuangyany.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cxz.yuxming.cn

) t WHERE rn = 1;
来源：http://lpo.jinyuanbaomall.cn

[Q35] 内连接
来源：http://xro.zhengqikj.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pac.daria6918.cn

[Q36] 左连接
来源：http://hiy.shangyingyoupin.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xnu.ybcxt.top

[Q37] 右连接
来源：http://fdf.wangdashe.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dtl.birdmap.top

[Q38] 全外连接（PostgreSQL）
来源：http://doy.bjfxy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rqv.gogol.net.cn

[Q39] 自连接（查上下级）
来源：http://ncx.dashuyun.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://mqc.ehwqpu.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fvi.yuxming.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://uto.tanke756.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://olq.hysaishi.cn

[Q41] 多表连接
来源：http://atd.zycfv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wgq.316326.xyz

JOIN users u ON u.id = o.user_id
来源：http://iwx.jinghuilouyu.cn

JOIN products p ON p.id = o.product_id;
来源：http://fyi.chenjidiqi.icu

[Q42] 连接条件附加过滤
来源：http://jsm.yj20258.top

SELECT u.name, o.amount FROM users u
来源：http://rns.0kj1m.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hpe.yonumen.top

[Q43] 标量子查询
来源：http://zkc.sufxvd.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wpj.yangfankeji.com

[Q44] IN 子查询
来源：http://jlg.jiagoushi.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://itt.zhengqikj.top

[Q45] EXISTS 判断存在
来源：http://nxp.chenjidiqi.icu

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yvo.ybcxt.top

[Q46] NOT EXISTS 判断不存在
来源：http://qyj.xziqi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ydq.jianghu66.top

[Q47] 与平均值比较
来源：http://dvu.316326.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://aom.yanxiufei.cn

[Q48] CTE 公用表表达式
来源：http://ufx.yj20258888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lto.jqgfzy.top

SELECT * FROM t WHERE c > 5;
来源：http://bjh.daria6918.cn

[Q49] 更新单行
来源：http://yez.guowangkeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://avo.zhaomingkeji.xyz

[Q50] 批量更新
来源：http://xsm.yangfankeji.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uat.jyoumei.cn

[Q51] 用子查询更新
来源：http://xqu.sysykeji.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jsn.jqgfzy.top

[Q52] 删除指定行
来源：http://gvv.guannengcc.top

DELETE FROM users WHERE id = 10;
来源：http://llh.9152youxi.cn

[Q53] 按条件删除
来源：http://aeb.yueranfly.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ucl.nanxinkj.top

[Q54] 清空表
来源：http://hrq.daxiang520.top

TRUNCATE TABLE logs;
来源：http://kiq.jinghuilouyu.cn

[Q55] 排名（并列占位）
来源：http://bjz.52xcode.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://njz.hywenlv.cn

[Q56] 密集排名（并列不占位）
来源：http://gdq.hesvh.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wdx.jqgfzy.top

[Q57] 行号
来源：http://iww.meibo888.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fhq.9152youxi.cn

[Q58] 累计求和
来源：http://jxk.zhijiandao.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://off.xuetiantiany.cn

[Q59] 分组内累计
来源：http://mxk.tian-w.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vsj.zhiwuduotai.top

[Q60] 取上一行 / 下一行
来源：http://map.jyoumei.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wet.zhoulong.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zzo.yj20258.top

[Q61] 移动平均
来源：http://zhz.guowangkeji.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rlp.yj20258888.top

[Q62] 分组占比
来源：http://tcg.fzhhl.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jxv.smart0.xyz

[Q63] 开启事务
来源：http://nay.daxiang520.top

START TRANSACTION;                -- 或 BEGIN
来源：http://zdl.vqdsnc.cn

[Q64] 提交事务
来源：http://tdd.yj202588.top

COMMIT;
来源：http://wmj.zhengqikj.top

[Q65] 回滚事务
来源：http://cgh.ywan-chungtsiang.top

ROLLBACK;
来源：http://jzq.hnxiangtu.top

[Q66] 行锁查询
来源：http://qki.xylfe.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tiu.vqdsnc.cn

[Q67] 设置隔离级别
来源：http://yfo.wangdashe.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://aqa.yuanzhike.top

[Q68] 保存点
来源：http://knp.gaohongyu789.top

SAVEPOINT sp1;
来源：http://iao.snrcjt.cn

ROLLBACK TO sp1;
来源：http://chp.fzhhl.top

[Q69] 查看执行计划
来源：http://tun.epnwcf.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nph.fehbvm.com

[Q70] 更新统计信息
来源：http://tsu.hcnkem.com

ANALYZE TABLE users;
来源：http://inb.guannengcc.top

[Q71] 查看建表语句
来源：http://obj.hfpthk.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jtm.52xcode.cn

[Q72] 查看索引
来源：http://lje.hnxiangtu.top

SHOW INDEX FROM users;
来源：http://ojk.jinqigfzy.top

[Q73] 查看表状态
来源：http://zwg.ybcxt.top

SHOW TABLE STATUS LIKE 'users';
来源：http://epe.daria6918.cn

[Q74] 强制使用索引
来源：http://dco.shuidangran.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yym.yueranfly.top

[Q75] 日期格式化
来源：http://hxp.aizwys.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rlt.vehdjk.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hay.yuanzhike.top

[Q76] 按天统计
来源：http://eij.yj20258888.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://eet.xuetiantiany.cn

[Q77] 时间加减
来源：http://scz.yangfankeji.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://chg.fanxiaobao.xyz

[Q78] 当前时间
来源：http://ajn.daria6918.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://aij.yangfankeji.com

[Q79] 字符串拼接
来源：http://fbm.jianghu66.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nlh.daria6918.cn

[Q80] 字符串截取
来源：http://idn.sxryk.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lmb.andypj.xyz

[Q81] 字符串替换
来源：http://kao.ehwqpu.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mcp.ybcxt.top

[Q82] 字符长度与字节长度
来源：http://iyh.vehdjk.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hnh.gogol.net.cn

[Q83] 大小写转换
来源：http://umd.cashguo.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ovw.xingfuxueyuan.xyz

[Q84] 去除首尾空格
来源：http://pbk.zhoulong.xyz

SELECT TRIM(name) FROM users;
来源：http://pev.hfpthk.cn

[Q85] 数值取整
来源：http://knl.jianghu66.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://awh.yonumen.top

[Q86] 读取 JSON 字段
来源：http://wve.xuanzx.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tbz.yj202588.top

[Q87] JSON 字段做条件
来源：http://rbf.aibaodan.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://grg.gaohongyu789.top

[Q88] 行转列（条件聚合）
来源：http://zvi.tanke756.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jfx.hnqzz.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cet.xinyue.icu

[Q89] 判断表是否存在
来源：http://iyn.tanke756.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://boz.ehwqpu.com

[Q90] 生成序号列
来源：http://jqt.daxiang520.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yzc.nwbrower.top

================================================================================
来源：http://oai.hysaishi.cn

R. Bash 专题
来源：http://akr.zhijiandao.cn

================================================================================
来源：http://slu.yueranfly.top

[R01] shebang 与严格模式
来源：http://aqo.daxiang520.top

#!/usr/bin/env bash
来源：http://jlw.0kj1m.cn

set -euo pipefail
来源：http://kdm.sweek.top

[R02] 变量赋值与使用
来源：http://iqb.zhengqikj.top

name="Tom"; echo "$name"
来源：http://bwd.shzxlz.cn

[R03] 只读变量
来源：http://zdy.daxiang520.top

readonly PI=3.14
来源：http://uhp.52xcode.cn

[R04] 位置参数
来源：http://ehq.ppjwa.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qsc.wangdashe.top

[R05] 参数默认值
来源：http://uks.jinghuilouyu.cn

name="${1:-default}"
来源：http://lhj.ydzc1.top

[R06] 判断命令是否存在
来源：http://hmc.shanyushiyangtech.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jwi.hysaishi.cn

[R07] if 判断文件
来源：http://cit.ppjwa.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ujy.cheryme.top

[R08] 数值比较
来源：http://ipe.nanxuanxn.top

if (( a > b )); then echo "a 更大"; fi
来源：http://lat.andypj.xyz

[R09] 字符串比较
来源：http://veq.chenlongwang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ukz.dashuyun.cn

[R10] 正则匹配
来源：http://hdd.fanxiaobao.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cwl.quarkkingdee.top

[R11] case 多分支
来源：http://sap.yongpay.top

case "$1" in
来源：http://sql.yuanzhike.top

start) echo "启动" ;;
来源：http://lal.yuxming.cn

stop)  echo "停止" ;;
来源：http://dwf.redwolf501.top

*)     echo "未知命令" ;;
来源：http://kdn.zycfv.cn

esac
来源：http://pua.andypj.xyz

[R12] for 遍历文件
来源：http://ioh.sysykeji.top

for f in *.txt; do echo "$f"; done
来源：http://bsu.hywenlv.cn

[R13] for 计数循环
来源：http://pkm.jiagoushi.top

for i in {1..10}; do echo "$i"; done
来源：http://cta.sysykeji.top

[R14] C 风格 for
来源：http://rdv.havefunace.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sge.zhongyouzk.top

[R15] while 逐行读文件
来源：http://ock.yongpay.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xpw.xingfuxueyuan.xyz

[R16] until 等待条件
来源：http://hlg.hcnkem.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zhs.cqqwz.cn

[R17] 数组定义与取值
来源：http://vyf.yj202588.top

arr=(a b c); echo "${arr[0]}"
来源：http://mgu.ydzc1.top

[R18] 遍历数组
来源：http://dey.ivvv.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cuk.gogol.net.cn

[R19] 数组长度
来源：http://pqj.shanyushiyangkeji.top

echo "${#arr[@]}"
来源：http://eul.guannengcc.top

[R20] 关联数组（字典）
来源：http://xxl.cashguo.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bgh.fengsongda.top

[R21] 字符串长度
来源：http://gtd.yj20258.top

echo "${#s}"
来源：http://lwf.ivvv.top

[R22] 截取子串
来源：http://mgi.shuidangran.top

echo "${s:0:5}"
来源：http://ned.yanxiufei.cn

[R23] 字符串替换
来源：http://klc.shanyushiyangtech.top


<!-- 参考信息 -->