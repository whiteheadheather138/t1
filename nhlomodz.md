代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://jai.uphjek.com

[P02] MD5 / SHA256 摘要
来源：http://pgb.hnqzz.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dwh.jinqigfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://hvn.daria6918.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oxx.zhiwuduotai.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vyd.shangyingyoupin.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://acm.zhijiandao.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zvn.jinghuilouyu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wbe.aizwys.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ogk.shanyushiyangkeji.top

[P03] 生成短随机字符串
来源：http://fdu.yj202588.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qke.tianlin.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rou.hongshengwenyu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tfh.hongshengwenyu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oyo.mhx1999.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kgz.svipenyu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cjo.tian-w.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pzc.sxryk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ebv.jinyuanbaomall.cn

[P04] 求长度
来源：http://xsg.andypj.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qgf.xingfuxueyuan.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://caz.zhengqikj.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ufs.hcnkem.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://flj.bbcook.cn

Java: list.size();  map.size();  s.length()
来源：http://uuz.yj202588.top

Go:   len(arr);  len(m)
来源：http://ltq.epnwcf.com

Ruby: x.length;  x.size
来源：http://zku.cdnleiting.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://evi.xylfe.cn

[P05] 判断两个对象内容是否相等
来源：http://ayu.xylfe.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yig.shuidangran.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vow.xylfe.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uek.shanyushiyangkeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wan.aizwys.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xsc.cashguo.top

Go:   reflect.DeepEqual(a, b)
来源：http://jbz.fehbvm.com

Ruby: a == b
来源：http://pkc.meibo888.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dru.hfpthk.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xng.daria6918.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://giw.gaohongyu789.top

PHP:  if (empty($x)) {}
来源：http://ymr.dianchejie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bgx.feifeiyinyue.top

TS:   if (x == null) {}
来源：http://pbw.nanxinkj.top

Java: if (x == null || x.isEmpty()) {}
来源：http://mdu.yfazqb.com

Go:   if x == nil {}
来源：http://ovi.pycfn.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://alc.kuanghao11.cn

C#:   if (x is null) {}
来源：http://bsp.dianchejie.cn

[P07] 防抖与节流
来源：http://wab.meibo888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rmd.cdnleiting.top

PHP:  // 手写时间戳比较
来源：http://mtl.zhijiandao.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kcj.pycfn.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bat.ywan-chungtsiang.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jjr.zycfv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://omz.ydjk.org.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qhv.hongshengwenyu.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://imo.xziqi.cn

[P08] 处理浮点精度问题
来源：http://mxs.shangyingyoupin.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mks.sufxvd.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jgj.cashguo.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gve.fzhhl.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://osq.fehbvm.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lwx.pengpengdd.cyou

Go:   math/big.Float，或全部换算成整数分再算
来源：http://igw.xuetiantiany.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hxt.jinyuanbaomall.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vig.hysaishi.cn

================================================================================
来源：http://haw.jianghu66.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nfm.xinyue.icu

================================================================================
来源：http://vxa.zycfv.cn

[Q01] 创建表
来源：http://vax.bjfxy.top

CREATE TABLE users (
来源：http://eit.tarul.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ykf.mhx1999.top

name VARCHAR(50) NOT NULL,
来源：http://wws.gzhubu.top

email VARCHAR(100) UNIQUE,
来源：http://ged.jinyuanbaomall.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wox.tian-w.cn

);
来源：http://ojb.yanxiufei.cn

[Q02] 创建带外键的表
来源：http://dfo.chenlongwang.top

CREATE TABLE orders (
来源：http://dxx.haohaochexian.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://aoh.zdqjudy.top

user_id INT NOT NULL,
来源：http://wwl.yj20258.top

amount DECIMAL(10, 2),
来源：http://iij.gaohongyu789.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sfg.sweek.top

);
来源：http://hda.gaohongyu789.top

[Q03] 增加列
来源：http://ymy.kuanghao11.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uiq.bbcook.cn

[Q04] 修改列类型
来源：http://dby.9152youxi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hsn.bbcook.cn

[Q05] 重命名列
来源：http://ynh.jiagoushi.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ddk.fehbvm.com

[Q06] 删除列
来源：http://qux.sysykeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://qpx.xingfuxueyuan.xyz

[Q07] 删除表
来源：http://bdq.cheryme.top

DROP TABLE IF EXISTS orders;
来源：http://esa.yanxiufei.cn

[Q08] 创建普通索引
来源：http://lqo.yonumen.top

CREATE INDEX idx_users_email ON users(email);
来源：http://oyn.tianlin.xyz

[Q09] 创建唯一索引
来源：http://knu.yanxiufei.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://msa.yanxiufei.cn

[Q10] 插入单行
来源：http://qph.xziqi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tpm.daxiang520.top

[Q11] 一次插入多行
来源：http://cwv.birdmap.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gbd.jqgfzy.top

[Q12] 插入后取自增 ID
来源：http://oqf.hcnkem.com

INSERT INTO users (name) VALUES ('C');
来源：http://imt.cdnleiting.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://iwo.cdnleiting.top

[Q13] 忽略重复插入
来源：http://ofo.hnqzz.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vae.cheryme.top

[Q14] 存在则更新（upsert）
来源：http://vcn.52xcode.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baa.zhongyouzk.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ctw.yueranfly.top

[Q15] 查询全部
来源：http://mdh.hongshengwenyu.top

SELECT * FROM users;
来源：http://hyz.hysaishi.cn

[Q16] 查询指定列
来源：http://hdy.hongshengwenyu.top

SELECT id, name FROM users;
来源：http://vye.jqgufenzy.top

[Q17] 条件查询
来源：http://jvo.jlsjyb.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ywp.xziqi.cn

[Q18] 模糊匹配
来源：http://vwv.cucudq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rvw.bjfxy.top

[Q19] 范围查询
来源：http://ynq.hcnkem.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cno.sufxvd.cn

[Q20] IN 列表
来源：http://vbu.ydzc1.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hwx.jianghu66.top

[Q21] 空值判断
来源：http://ngo.kuanghao11.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zmw.guowangkeji.top

[Q22] 排序
来源：http://wlm.0kj1m.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sto.redwolf501.top

[Q23] 分页
来源：http://tse.wangdashe.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jto.gogol.net.cn

[Q24] 去重
来源：http://gew.chenjidiqi.icu

SELECT DISTINCT city FROM users;
来源：http://lmp.52xcode.cn

[Q25] 只取前 N 条
来源：http://xmk.zhoulong.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hmh.xziqi.cn

[Q26] 计数
来源：http://pgp.gotoacloud.top

SELECT COUNT(*) FROM users;
来源：http://ybw.xuetiantiany.cn

[Q27] 条件计数
来源：http://mmi.zhongyouzk.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lwf.jianghu66.top

[Q28] 求和与平均
来源：http://hqt.dashuyun.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dec.yj20258.top

[Q29] 最大最小值
来源：http://oaq.tianlin.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://mjt.aizwys.cn

[Q30] 分组统计
来源：http://vyr.yonumen.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://odm.nanxuanxn.top

[Q31] 分组后过滤
来源：http://esj.guannengcc.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://abd.wangdashe.top

[Q32] 分组拼接字符串
来源：http://div.zhengqikj.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ehf.hnxiangtu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://snc.jqgufenzy.top

[Q33] 多列分组
来源：http://vru.fktsv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ani.chenjidiqi.icu

[Q34] 每组取第一条
来源：http://vpm.sweek.top

SELECT * FROM (
来源：http://kiw.snrcjt.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pxv.vqdsnc.cn

) t WHERE rn = 1;
来源：http://qdp.xylfe.cn

[Q35] 内连接
来源：http://jou.tarul.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bbp.nwbrower.top

[Q36] 左连接
来源：http://zjl.zhengqikj.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ctz.smart0.xyz

[Q37] 右连接
来源：http://jgk.gaohongyu789.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gki.vehdjk.com

[Q38] 全外连接（PostgreSQL）
来源：http://tmg.yangfankeji.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dgo.guannengcc.top

[Q39] 自连接（查上下级）
来源：http://nru.havefunace.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://djb.uphjek.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vvn.uphjek.com

[Q40] 交叉连接（笛卡尔积）
来源：http://bmg.hnqzz.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kqs.jyoumei.cn

[Q41] 多表连接
来源：http://wnh.jqgufenzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://hpx.yj20258888.top

JOIN users u ON u.id = o.user_id
来源：http://nlc.gogol.net.cn

JOIN products p ON p.id = o.product_id;
来源：http://ysc.jianghu66.top

[Q42] 连接条件附加过滤
来源：http://aek.bjfxy.top

SELECT u.name, o.amount FROM users u
来源：http://kgd.jinyuanbaomall.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xmf.xziqi.cn

[Q43] 标量子查询
来源：http://myf.tarul.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lsk.shanyushiyangtech.top

[Q44] IN 子查询
来源：http://tcs.cheryme.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kzt.jianghu66.top

[Q45] EXISTS 判断存在
来源：http://xol.iojbl.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fmd.hcnkem.com

[Q46] NOT EXISTS 判断不存在
来源：http://hwj.shangyingyoupin.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ilr.ywan-chungtsiang.top

[Q47] 与平均值比较
来源：http://waa.xuetiantiany.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oog.jianghu66.top

[Q48] CTE 公用表表达式
来源：http://uyu.cucudq.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://oer.yvedp.cn

SELECT * FROM t WHERE c > 5;
来源：http://aoj.chenjidiqi.icu

[Q49] 更新单行
来源：http://hig.nwbrower.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://plm.bjfxy.top

[Q50] 批量更新
来源：http://cri.jqgufenzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fxm.haohaochexian.top

[Q51] 用子查询更新
来源：http://yis.nanxinkj.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://eoc.xuetiantiany.cn

[Q52] 删除指定行
来源：http://pjl.nwbrower.top

DELETE FROM users WHERE id = 10;
来源：http://elj.jianghu66.top

[Q53] 按条件删除
来源：http://vfh.chenzaomai.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wby.hesvh.cn

[Q54] 清空表
来源：http://nhv.sysykeji.top

TRUNCATE TABLE logs;
来源：http://szw.fanxiaobao.xyz

[Q55] 排名（并列占位）
来源：http://gph.ivvv.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mrg.daria6918.cn

[Q56] 密集排名（并列不占位）
来源：http://ujg.mhx1999.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ext.daxiang520.top

[Q57] 行号
来源：http://wvx.guannengcc.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mvh.svipenyu.cn

[Q58] 累计求和
来源：http://eiv.smart0.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://iww.daxiang520.top

[Q59] 分组内累计
来源：http://ian.zhengqikj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vbs.haohaochexian.top

[Q60] 取上一行 / 下一行
来源：http://gki.vqdsnc.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jbx.gotoacloud.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jbm.zhijiandao.cn

[Q61] 移动平均
来源：http://zsx.fehbvm.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nek.sweek.top

[Q62] 分组占比
来源：http://qbl.cheryme.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rha.nanxuanxn.top

[Q63] 开启事务
来源：http://arg.ybcxt.top

START TRANSACTION;                -- 或 BEGIN
来源：http://nuc.iojbl.cn

[Q64] 提交事务
来源：http://fvw.nanxuanxn.top

COMMIT;
来源：http://geh.chenzaomai.com

[Q65] 回滚事务
来源：http://jwr.zhiwuduotai.top

ROLLBACK;
来源：http://bab.shuidangran.top

[Q66] 行锁查询
来源：http://bvq.hnxiangtu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rfu.dianchejie.cn

[Q67] 设置隔离级别
来源：http://pkf.ywan-chungtsiang.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kdf.daria6918.cn

[Q68] 保存点
来源：http://pzj.fanxiaobao.xyz

SAVEPOINT sp1;
来源：http://imy.jqgfzy.top

ROLLBACK TO sp1;
来源：http://pat.daxiang520.top

[Q69] 查看执行计划
来源：http://heo.zdqjudy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hyx.fanxiaobao.xyz

[Q70] 更新统计信息
来源：http://ubx.aibaodan.cn

ANALYZE TABLE users;
来源：http://suz.yvedp.cn

[Q71] 查看建表语句
来源：http://eva.tianlin.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xlr.birdmap.top

[Q72] 查看索引
来源：http://wzj.yuxming.cn

SHOW INDEX FROM users;
来源：http://gik.vehdjk.com

[Q73] 查看表状态
来源：http://sro.zhoulong.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://pom.wangshuangyany.cn

[Q74] 强制使用索引
来源：http://dxc.gogol.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xos.xinyue.icu

[Q75] 日期格式化
来源：http://bnx.jinyuanbaomall.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sqx.pycfn.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://apa.zhaomingkeji.xyz

[Q76] 按天统计
来源：http://plw.epnwcf.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jqx.svipenyu.cn

[Q77] 时间加减
来源：http://bss.daxiang520.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dpg.hongshengwenyu.top

[Q78] 当前时间
来源：http://cuh.ybcxt.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://goc.daxiang520.top

[Q79] 字符串拼接
来源：http://bjh.jqgfzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://chh.hongshengwenyu.top

[Q80] 字符串截取
来源：http://xfk.hammf.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fhs.guannengcc.top

[Q81] 字符串替换
来源：http://ewj.yuxming.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rot.jqgfzy.top

[Q82] 字符长度与字节长度
来源：http://ota.xuetiantiany.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hhr.hnxiangtu.top

[Q83] 大小写转换
来源：http://gjj.jianghu66.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ley.ctjpmb.com

[Q84] 去除首尾空格
来源：http://yfk.aibaodan.cn

SELECT TRIM(name) FROM users;
来源：http://wjn.jianghu66.top

[Q85] 数值取整
来源：http://tzu.smart0.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tmd.vqdsnc.cn

[Q86] 读取 JSON 字段
来源：http://ons.zhixingplan.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ifv.shuidangran.top

[Q87] JSON 字段做条件
来源：http://hlt.c1oappe.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zzr.yj20258888.top

[Q88] 行转列（条件聚合）
来源：http://qwg.yj20258888.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://akg.tarul.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://atv.jinyuanbaomall.cn

[Q89] 判断表是否存在
来源：http://hea.guannengcc.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://erz.ehwqpu.com

[Q90] 生成序号列
来源：http://wpe.ydjk.org.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kgr.ivvv.top

================================================================================
来源：http://djw.shanyushiyangtech.top

R. Bash 专题
来源：http://gij.yfazqb.com

================================================================================
来源：http://cus.shanyushiyangkeji.top

[R01] shebang 与严格模式
来源：http://sme.tianlin.xyz

#!/usr/bin/env bash
来源：http://uja.jqgfzy.top

set -euo pipefail
来源：http://eaa.fehbvm.com

[R02] 变量赋值与使用
来源：http://ptr.ydzc1.top

name="Tom"; echo "$name"
来源：http://fhs.jiagoushi.top

[R03] 只读变量
来源：http://iiy.pycfn.com

readonly PI=3.14
来源：http://kzl.sysykeji.top

[R04] 位置参数
来源：http://nxf.dashuyun.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://omx.sjlbkw.cn

[R05] 参数默认值
来源：http://kqh.yanxiufei.cn

name="${1:-default}"
来源：http://cmm.xylfe.cn

[R06] 判断命令是否存在
来源：http://yzi.shuidangran.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gbz.smart0.xyz

[R07] if 判断文件
来源：http://rey.ivvv.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pus.epnwcf.com

[R08] 数值比较
来源：http://mgx.yanxiufei.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hbl.fehbvm.com

[R09] 字符串比较
来源：http://zly.zycfv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nop.mhx1999.top

[R10] 正则匹配
来源：http://hzv.yueranfly.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dng.bjfxy.top

[R11] case 多分支
来源：http://ycf.zdbjq.cn

case "$1" in
来源：http://cfy.pycfn.com

start) echo "启动" ;;
来源：http://dbf.svipenyu.cn

stop)  echo "停止" ;;
来源：http://iva.pycfn.com

*)     echo "未知命令" ;;
来源：http://jqa.xylfe.cn


<!-- 参考信息 -->