代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hqq.ybcxt.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jgx.jinyuanbaomall.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ckg.yuxming.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hfm.zhixingplan.top

Java: list.size();  map.size();  s.length()
来源：http://pld.aizwys.cn

Go:   len(arr);  len(m)
来源：http://fra.yuxming.cn

Ruby: x.length;  x.size
来源：http://wtz.jyoumei.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pzx.wangshuangyany.cn

[P05] 判断两个对象内容是否相等
来源：http://fpw.shzxlz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fvw.fanxiaobao.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qtq.hcnkem.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://osw.jinghuilouyu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://amh.cashguo.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xes.pengpengdd.cyou

Go:   reflect.DeepEqual(a, b)
来源：http://cju.tarul.cn

Ruby: a == b
来源：http://kus.vqdsnc.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hdm.yuanzhike.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qmk.shuidangran.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sng.yuanzhike.top

PHP:  if (empty($x)) {}
来源：http://gas.feifeiyinyue.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://god.ydjk.org.cn

TS:   if (x == null) {}
来源：http://oca.sweek.top

Java: if (x == null || x.isEmpty()) {}
来源：http://eeo.gaohongyu789.top

Go:   if x == nil {}
来源：http://rwz.xingfuxueyuan.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://opv.zhongyouzk.top

C#:   if (x is null) {}
来源：http://fbb.tarul.cn

[P07] 防抖与节流
来源：http://bdj.xuanzx.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xys.zycfv.cn

PHP:  // 手写时间戳比较
来源：http://onk.yj20258.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bxv.zdqjudy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bhx.hcnkem.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pde.xuetiantiany.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dat.uphjek.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://uko.sufxvd.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mut.iojbl.cn

[P08] 处理浮点精度问题
来源：http://jdu.zycfv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xeu.yj202588.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lyk.gotoacloud.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wfi.sysykeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://enr.c1oappe.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mid.tanke756.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ovo.hysaishi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://meo.yanxiufei.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gjg.zycfv.cn

================================================================================
来源：http://uob.nanxuanxn.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nmi.jinyuanbaomall.cn

================================================================================
来源：http://qij.pycfn.com

[Q01] 创建表
来源：http://qtx.zhongyouzk.top

CREATE TABLE users (
来源：http://dxt.gzhubu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hhq.ehwqpu.com

name VARCHAR(50) NOT NULL,
来源：http://nxl.aibaodan.cn

email VARCHAR(100) UNIQUE,
来源：http://bce.jinqigufen.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qhh.yongpay.top

);
来源：http://dhm.zycfv.cn

[Q02] 创建带外键的表
来源：http://kla.gogol.net.cn

CREATE TABLE orders (
来源：http://ykm.zhongyouzk.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://thy.jlsjyb.cn

user_id INT NOT NULL,
来源：http://mrz.xinyue.icu

amount DECIMAL(10, 2),
来源：http://cad.fktsv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lub.ywan-chungtsiang.top

);
来源：http://wcf.yj20258.top

[Q03] 增加列
来源：http://ojz.shzxlz.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://syd.9152youxi.cn

[Q04] 修改列类型
来源：http://gkc.zhixingplan.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hpx.cheryme.top

[Q05] 重命名列
来源：http://tvw.dianchejie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jgp.c1oappe.top

[Q06] 删除列
来源：http://ygv.nwbrower.top

ALTER TABLE users DROP COLUMN age;
来源：http://uuc.jianghu66.top

[Q07] 删除表
来源：http://ndd.tanke756.top

DROP TABLE IF EXISTS orders;
来源：http://ray.zhiwuduotai.top

[Q08] 创建普通索引
来源：http://jtc.xylfe.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nkq.jinqigfzy.top

[Q09] 创建唯一索引
来源：http://hqk.daxiang520.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fyw.cqqwz.cn

[Q10] 插入单行
来源：http://ljj.fehbvm.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oxl.jinqigfzy.top

[Q11] 一次插入多行
来源：http://qve.yongpay.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://eja.hnqzz.top

[Q12] 插入后取自增 ID
来源：http://hox.sufxvd.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rpz.yuanzhike.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://odu.snrcjt.cn

[Q13] 忽略重复插入
来源：http://zkn.kuanghao11.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sxh.bjfxy.top

[Q14] 存在则更新（upsert）
来源：http://qnv.wangshuangyany.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gmq.jqgufenzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zny.yj202588.top

[Q15] 查询全部
来源：http://lid.zhijiandao.cn

SELECT * FROM users;
来源：http://zmx.yj202588.top

[Q16] 查询指定列
来源：http://zqn.wangdashe.top

SELECT id, name FROM users;
来源：http://sps.dianchejie.cn

[Q17] 条件查询
来源：http://ixh.jyoumei.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jny.vqdsnc.cn

[Q18] 模糊匹配
来源：http://ysh.sjlbkw.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://szk.cashguo.top

[Q19] 范围查询
来源：http://ahn.yj20258.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://iww.fanxiaobao.xyz

[Q20] IN 列表
来源：http://ist.ctjpmb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bhd.nanxinkj.top

[Q21] 空值判断
来源：http://ehp.jiagoushi.top

SELECT * FROM users WHERE email IS NULL;
来源：http://iss.fanxiaobao.xyz

[Q22] 排序
来源：http://pxz.hnqzz.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cel.cucudq.cn

[Q23] 分页
来源：http://lmf.nwbrower.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://die.fengsongda.top

[Q24] 去重
来源：http://mav.nanxuanxn.top

SELECT DISTINCT city FROM users;
来源：http://dpe.daria6918.cn

[Q25] 只取前 N 条
来源：http://kad.xingfuxueyuan.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yyl.dashuyun.cn

[Q26] 计数
来源：http://ugm.ctjpmb.com

SELECT COUNT(*) FROM users;
来源：http://jle.epnwcf.com

[Q27] 条件计数
来源：http://bpc.yj202588.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iku.zhixingplan.top

[Q28] 求和与平均
来源：http://xbu.yj202588.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cox.hysaishi.cn

[Q29] 最大最小值
来源：http://prl.yuanzhike.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://vog.sweek.top

[Q30] 分组统计
来源：http://sen.yvedp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vjx.ctjpmb.com

[Q31] 分组后过滤
来源：http://mzy.sxryk.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://auw.xuetiantiany.cn

[Q32] 分组拼接字符串
来源：http://njh.sweek.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mrr.chenzaomai.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dao.kuanghao11.cn

[Q33] 多列分组
来源：http://bql.daxiang520.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://njq.meibo888.top

[Q34] 每组取第一条
来源：http://pzz.9152youxi.cn

SELECT * FROM (
来源：http://nqf.zycfv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dny.ctjpmb.com

) t WHERE rn = 1;
来源：http://ugm.gogol.net.cn

[Q35] 内连接
来源：http://mjb.yonumen.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ggz.nanxuanxn.top

[Q36] 左连接
来源：http://rzo.hcnkem.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fnu.shzxlz.cn

[Q37] 右连接
来源：http://mjw.hysaishi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qcm.yangfankeji.com

[Q38] 全外连接（PostgreSQL）
来源：http://dov.yj20258.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qba.vehdjk.com

[Q39] 自连接（查上下级）
来源：http://jto.hongshengwenyu.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ixj.daxiang520.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://loi.zdbjq.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rjo.guowangkeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kvg.ivvv.top

[Q41] 多表连接
来源：http://rbn.xuanzx.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://ulw.daria6918.cn

JOIN users u ON u.id = o.user_id
来源：http://fmu.zhijiandao.cn

JOIN products p ON p.id = o.product_id;
来源：http://cly.zhijiandao.cn

[Q42] 连接条件附加过滤
来源：http://kab.jinqigufen.top

SELECT u.name, o.amount FROM users u
来源：http://qhd.pengpengdd.cyou

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nnf.ctjpmb.com

[Q43] 标量子查询
来源：http://ttw.ehwqpu.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zsl.guowangkeji.top

[Q44] IN 子查询
来源：http://ojt.zhijiandao.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://spk.bbcook.cn

[Q45] EXISTS 判断存在
来源：http://lma.meibo888.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xon.cucudq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xmd.gaohongyu789.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nnk.vehdjk.com

[Q47] 与平均值比较
来源：http://nnd.ehwqpu.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hrp.zhongyouzk.top

[Q48] CTE 公用表表达式
来源：http://ocg.hysaishi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://meo.hysaishi.cn

SELECT * FROM t WHERE c > 5;
来源：http://png.yanxiufei.cn

[Q49] 更新单行
来源：http://sqs.316326.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ogi.sxryk.cn

[Q50] 批量更新
来源：http://nsz.xziqi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gxy.yangfankeji.com

[Q51] 用子查询更新
来源：http://ias.cqqwz.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pfe.hcnkem.com

[Q52] 删除指定行
来源：http://pkn.shanyushiyangkeji.top

DELETE FROM users WHERE id = 10;
来源：http://dbk.jianghu66.top

[Q53] 按条件删除
来源：http://bey.ehwqpu.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kiv.xuanzx.com

[Q54] 清空表
来源：http://ncs.iojbl.cn

TRUNCATE TABLE logs;
来源：http://jyn.fzhhl.top

[Q55] 排名（并列占位）
来源：http://lyo.shangyingyoupin.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jjy.vehdjk.com

[Q56] 密集排名（并列不占位）
来源：http://lep.hcnkem.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://aar.bbcook.cn

[Q57] 行号
来源：http://miy.ywan-chungtsiang.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vnd.tianlin.xyz

[Q58] 累计求和
来源：http://sei.nanxuanxn.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sst.xingfuxueyuan.xyz

[Q59] 分组内累计
来源：http://xyw.mhx1999.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hcu.zhengqikj.top

[Q60] 取上一行 / 下一行
来源：http://qgi.xziqi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://onx.yuxming.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://clt.hesvh.cn

[Q61] 移动平均
来源：http://zax.nwbrower.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tkv.nanxuanxn.top

[Q62] 分组占比
来源：http://apu.gaohongyu789.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zgo.jianghu66.top

[Q63] 开启事务
来源：http://btt.yfazqb.com

START TRANSACTION;                -- 或 BEGIN
来源：http://jzy.hnxiangtu.top

[Q64] 提交事务
来源：http://mnh.vqdsnc.cn

COMMIT;
来源：http://gzh.zdbjq.cn

[Q65] 回滚事务
来源：http://qso.redwolf501.top

ROLLBACK;
来源：http://dzv.316326.xyz

[Q66] 行锁查询
来源：http://bxx.shanyushiyangkeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fry.tarul.cn

[Q67] 设置隔离级别
来源：http://ndi.sxryk.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://alw.hnqzz.top

[Q68] 保存点
来源：http://aze.xinyue.icu

SAVEPOINT sp1;
来源：http://gsk.havefunace.top

ROLLBACK TO sp1;
来源：http://pkk.yfazqb.com

[Q69] 查看执行计划
来源：http://bkc.jianghu66.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lnz.cqqwz.cn

[Q70] 更新统计信息
来源：http://yyz.epnwcf.com

ANALYZE TABLE users;
来源：http://odg.aizwys.cn

[Q71] 查看建表语句
来源：http://ozl.c1oappe.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uhr.cucudq.cn

[Q72] 查看索引
来源：http://hpn.gogol.net.cn

SHOW INDEX FROM users;
来源：http://osm.meibo888.top

[Q73] 查看表状态
来源：http://kve.yj202588.top

SHOW TABLE STATUS LIKE 'users';
来源：http://lzx.nanxuanxn.top

[Q74] 强制使用索引
来源：http://dyo.kuanghao11.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ncn.yuanzhike.top

[Q75] 日期格式化
来源：http://cek.guannengcc.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dff.xuetiantiany.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pcs.hammf.cn

[Q76] 按天统计
来源：http://znq.ehwqpu.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://btk.zhixingplan.top

[Q77] 时间加减
来源：http://pux.quarkkingdee.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jqr.jianghu66.top

[Q78] 当前时间
来源：http://tbi.dashuyun.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hlq.fehbvm.com

[Q79] 字符串拼接
来源：http://twr.zdbjq.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://iry.aizwys.cn

[Q80] 字符串截取
来源：http://nzx.sjlbkw.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sdk.redwolf501.top

[Q81] 字符串替换
来源：http://zys.sjlbkw.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pso.jiagoushi.top

[Q82] 字符长度与字节长度
来源：http://zrx.iojbl.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ckq.chenlongwang.top

[Q83] 大小写转换
来源：http://anc.hysaishi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yhu.fengsongda.top

[Q84] 去除首尾空格
来源：http://fdl.zhengqikj.top

SELECT TRIM(name) FROM users;
来源：http://owh.jlsjyb.cn

[Q85] 数值取整
来源：http://fmh.sweek.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hxi.jinqigfzy.top

[Q86] 读取 JSON 字段
来源：http://ncn.ybcxt.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vux.jlsjyb.cn

[Q87] JSON 字段做条件
来源：http://ycj.hnqzz.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ndu.xinyue.icu

[Q88] 行转列（条件聚合）
来源：http://dzi.yueranfly.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uvn.jinyuanbaomall.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jgu.nanxuanxn.top

[Q89] 判断表是否存在
来源：http://jsj.chenzaomai.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wys.zhixingplan.top

[Q90] 生成序号列
来源：http://xtz.sjlbkw.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mhf.cashguo.top

================================================================================
来源：http://mub.shanyushiyangkeji.top

R. Bash 专题
来源：http://rks.jianghu66.top

================================================================================
来源：http://qyv.guannengcc.top

[R01] shebang 与严格模式
来源：http://hqy.fehbvm.com

#!/usr/bin/env bash
来源：http://rjz.kuanghao11.cn

set -euo pipefail
来源：http://fis.epnwcf.com

[R02] 变量赋值与使用
来源：http://wic.aizwys.cn

name="Tom"; echo "$name"
来源：http://nii.hywenlv.cn

[R03] 只读变量
来源：http://nkq.jinqigufen.top

readonly PI=3.14
来源：http://cnk.jqgufenzy.top

[R04] 位置参数
来源：http://ebe.zdqjudy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gno.wangshuangyany.cn

[R05] 参数默认值
来源：http://jeu.hcnkem.com

name="${1:-default}"
来源：http://pnv.jlsjyb.cn

[R06] 判断命令是否存在
来源：http://cgs.chenzaomai.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xsp.yongpay.top

[R07] if 判断文件
来源：http://yjn.sufxvd.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bjg.hfpthk.cn

[R08] 数值比较
来源：http://hav.fanxiaobao.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://asj.ybcxt.top

[R09] 字符串比较
来源：http://jvt.ctjpmb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://spj.nanxinkj.top

[R10] 正则匹配
来源：http://ktk.hysaishi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://osx.jqgufenzy.top

[R11] case 多分支
来源：http://cno.tanke756.top

case "$1" in
来源：http://csw.daria6918.cn

start) echo "启动" ;;
来源：http://fpg.dashuyun.cn

stop)  echo "停止" ;;
来源：http://dga.mhx1999.top

*)     echo "未知命令" ;;
来源：http://mkz.xinyue.icu

esac
来源：http://qfv.52xcode.cn

[R12] for 遍历文件
来源：http://nfe.zdbjq.cn

for f in *.txt; do echo "$f"; done
来源：http://ffv.jinqigfzy.top

[R13] for 计数循环
来源：http://byv.pengpengdd.cyou

for i in {1..10}; do echo "$i"; done
来源：http://gud.havefunace.top

[R14] C 风格 for
来源：http://rcm.zhiwuduotai.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://naa.yongpay.top

[R15] while 逐行读文件
来源：http://zwo.nwbrower.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hlu.nanxuanxn.top

[R16] until 等待条件
来源：http://qaq.0kj1m.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uou.xylfe.cn

[R17] 数组定义与取值
来源：http://zxp.zdbjq.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vep.0kj1m.cn

[R18] 遍历数组
来源：http://beb.yvedp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bjh.zhaomingkeji.xyz

[R19] 数组长度
来源：http://ita.cucudq.cn

echo "${#arr[@]}"
来源：http://ylj.meibo888.top

[R20] 关联数组（字典）
来源：http://ckt.epnwcf.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bvq.hysaishi.cn

[R21] 字符串长度
来源：http://ozc.birdmap.top


<!-- 参考信息 -->