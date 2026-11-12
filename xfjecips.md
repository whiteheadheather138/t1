代发 wailian999

[O06] 使用进程池
来源：http://wcu.shanyushiyangtech.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lzf.zhiwuduotai.top

PHP:  // pcntl_fork 或多进程队列
来源：http://epw.jiagoushi.top

JS:   // child_process / cluster 模块
来源：http://wpp.feifeiyinyue.top

TS:   // child_process / cluster 模块
来源：http://gbj.jianghu66.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zxa.svipenyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bxg.iojbl.cn

Ruby: // fork 块
来源：http://wzn.tianlin.xyz

C#:   Parallel.For
来源：http://tfk.hfpthk.cn

================================================================================
来源：http://cwg.ppjwa.cn

P. 常用工具函数
来源：http://awr.hcnkem.com

================================================================================
来源：http://plo.yuanzhike.top

[P01] 生成 UUID
来源：http://yll.ywan-chungtsiang.top

Py:   str(uuid.uuid4())
来源：http://pvk.guannengcc.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xkm.aibaodan.cn

JS:   crypto.randomUUID()
来源：http://atm.gaohongyu789.top

TS:   crypto.randomUUID()
来源：http://vvh.jiagoushi.top

Java: UUID.randomUUID().toString()
来源：http://qyo.sysykeji.top

Go:   // 用 github.com/google/uuid
来源：http://klo.iojbl.cn

Ruby: SecureRandom.uuid
来源：http://ltm.tian-w.cn

C#:   Guid.NewGuid().ToString()
来源：http://emy.yuxming.cn

[P02] MD5 / SHA256 摘要
来源：http://buu.bbcook.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mbi.jqgfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://nrq.fehbvm.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://smq.hfpthk.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://asu.svipenyu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bxt.ydzc1.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dlj.yj202588.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://clw.sysykeji.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dwu.jinqigfzy.top

[P03] 生成短随机字符串
来源：http://rcx.vehdjk.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dbd.52xcode.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ftg.yonumen.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pnv.jiagoushi.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nvy.zhijiandao.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jku.fengsongda.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ont.wangshuangyany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://sjm.yuxming.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mgq.0kj1m.cn

[P04] 求长度
来源：http://aad.chenjidiqi.icu

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ran.uphjek.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rwa.bbcook.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kya.pengpengdd.cyou

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tgn.dianchejie.cn

Java: list.size();  map.size();  s.length()
来源：http://dzy.shzxlz.cn

Go:   len(arr);  len(m)
来源：http://nbb.fehbvm.com

Ruby: x.length;  x.size
来源：http://lzb.sweek.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://kzv.yfazqb.com

[P05] 判断两个对象内容是否相等
来源：http://nyp.shuidangran.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ckl.yuanzhike.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dhn.ybcxt.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rvs.c1oappe.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ewt.hywenlv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xna.vqdsnc.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qxq.hesvh.cn

Ruby: a == b
来源：http://rov.zdqjudy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zdr.ehwqpu.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gul.tianlin.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://evf.jqgufenzy.top

PHP:  if (empty($x)) {}
来源：http://tan.ctjpmb.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gij.aibaodan.cn

TS:   if (x == null) {}
来源：http://uhv.uphjek.com

Java: if (x == null || x.isEmpty()) {}
来源：http://imd.shanyushiyangkeji.top

Go:   if x == nil {}
来源：http://mev.birdmap.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hux.gzhubu.top

C#:   if (x is null) {}
来源：http://ctb.yj202588.top

[P07] 防抖与节流
来源：http://wlo.kuanghao11.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://aba.chenjidiqi.icu

PHP:  // 手写时间戳比较
来源：http://rae.zdqjudy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uzw.zhixingplan.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qwj.c1oappe.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rdr.zhengqikj.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rvn.svipenyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://iwm.jqgufenzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jez.chenjidiqi.icu

[P08] 处理浮点精度问题
来源：http://vli.daria6918.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zsy.ybcxt.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yrb.ydzc1.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bds.meibo888.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ykq.xinyue.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dxc.yfazqb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gee.zhengqikj.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wfx.pengpengdd.cyou

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cnr.yongpay.top

================================================================================
来源：http://lrt.sweek.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mra.aibaodan.cn

================================================================================
来源：http://bru.nwbrower.top

[Q01] 创建表
来源：http://png.nwbrower.top

CREATE TABLE users (
来源：http://tjk.aibaodan.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dpl.fzhhl.top

name VARCHAR(50) NOT NULL,
来源：http://ohb.gogol.net.cn

email VARCHAR(100) UNIQUE,
来源：http://kcz.dianchejie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://adg.aibaodan.cn

);
来源：http://sjt.epnwcf.com

[Q02] 创建带外键的表
来源：http://aqk.ydjk.org.cn

CREATE TABLE orders (
来源：http://nab.mhx1999.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hrl.pycfn.com

user_id INT NOT NULL,
来源：http://ybo.zhongyouzk.top

amount DECIMAL(10, 2),
来源：http://huv.daxiang520.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://keg.0kj1m.cn

);
来源：http://qet.feifeiyinyue.top

[Q03] 增加列
来源：http://abr.shangyingyoupin.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xhx.zdqjudy.top

[Q04] 修改列类型
来源：http://luk.yangfankeji.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lcr.hammf.cn

[Q05] 重命名列
来源：http://yex.yanxiufei.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zgq.gogol.net.cn

[Q06] 删除列
来源：http://uih.yfazqb.com

ALTER TABLE users DROP COLUMN age;
来源：http://uqu.gogol.net.cn

[Q07] 删除表
来源：http://als.0kj1m.cn

DROP TABLE IF EXISTS orders;
来源：http://dfk.gzhubu.top

[Q08] 创建普通索引
来源：http://fjg.haohaochexian.top

CREATE INDEX idx_users_email ON users(email);
来源：http://kbj.sxryk.cn

[Q09] 创建唯一索引
来源：http://tdk.jinqigufen.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vmb.jinqigufen.top

[Q10] 插入单行
来源：http://bzf.ywan-chungtsiang.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vbj.shzxlz.cn

[Q11] 一次插入多行
来源：http://efv.yj202588.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hzu.tanke756.top

[Q12] 插入后取自增 ID
来源：http://ojx.chenzaomai.com

INSERT INTO users (name) VALUES ('C');
来源：http://jvh.shzxlz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kft.hammf.cn

[Q13] 忽略重复插入
来源：http://vot.sxryk.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ykq.cqqwz.cn

[Q14] 存在则更新（upsert）
来源：http://iuo.zhiwuduotai.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pdl.yongpay.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://voa.sysykeji.top

[Q15] 查询全部
来源：http://vtb.yueranfly.top

SELECT * FROM users;
来源：http://pmm.xingfuxueyuan.xyz

[Q16] 查询指定列
来源：http://ypc.zhijiandao.cn

SELECT id, name FROM users;
来源：http://nvp.snrcjt.cn

[Q17] 条件查询
来源：http://gqa.ydjk.org.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xsh.jianghu66.top

[Q18] 模糊匹配
来源：http://bgd.tian-w.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rxc.zdbjq.cn

[Q19] 范围查询
来源：http://aiu.meibo888.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gou.yj202588.top

[Q20] IN 列表
来源：http://ymp.yuxming.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ixp.zdqjudy.top

[Q21] 空值判断
来源：http://sbu.zhaomingkeji.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://cjb.ctjpmb.com

[Q22] 排序
来源：http://pst.sysykeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tde.fanxiaobao.xyz

[Q23] 分页
来源：http://bbr.guannengcc.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yiz.jlsjyb.cn

[Q24] 去重
来源：http://nrr.jinqigufen.top

SELECT DISTINCT city FROM users;
来源：http://axm.svipenyu.cn

[Q25] 只取前 N 条
来源：http://tsp.fzhhl.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://neo.chenjidiqi.icu

[Q26] 计数
来源：http://lfy.chenzaomai.com

SELECT COUNT(*) FROM users;
来源：http://dcu.gzhubu.top

[Q27] 条件计数
来源：http://jds.pycfn.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lmu.meibo888.top

[Q28] 求和与平均
来源：http://txn.tian-w.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hmd.epnwcf.com

[Q29] 最大最小值
来源：http://apv.c1oappe.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jnw.fanxiaobao.xyz

[Q30] 分组统计
来源：http://eed.fzhhl.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dup.gaohongyu789.top

[Q31] 分组后过滤
来源：http://jyz.zycfv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dww.aizwys.cn

[Q32] 分组拼接字符串
来源：http://ifa.ywan-chungtsiang.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qam.0kj1m.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nhn.jyoumei.cn

[Q33] 多列分组
来源：http://pth.smart0.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bfy.wangshuangyany.cn

[Q34] 每组取第一条
来源：http://xdq.quarkkingdee.top

SELECT * FROM (
来源：http://rxu.xuanzx.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hwk.jqgufenzy.top

) t WHERE rn = 1;
来源：http://rmm.hnxiangtu.top

[Q35] 内连接
来源：http://qha.nanxinkj.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vtm.ywan-chungtsiang.top

[Q36] 左连接
来源：http://bkp.sweek.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://djv.zycfv.cn

[Q37] 右连接
来源：http://jbv.cheryme.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rci.birdmap.top

[Q38] 全外连接（PostgreSQL）
来源：http://qdb.chenlongwang.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://npg.fanxiaobao.xyz

[Q39] 自连接（查上下级）
来源：http://hhv.ybcxt.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://pky.tian-w.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://asz.xylfe.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xhd.yuanzhike.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sul.cashguo.top

[Q41] 多表连接
来源：http://jur.sysykeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://sqx.sweek.top

JOIN users u ON u.id = o.user_id
来源：http://nrv.hywenlv.cn

JOIN products p ON p.id = o.product_id;
来源：http://fxo.hfpthk.cn

[Q42] 连接条件附加过滤
来源：http://qbq.hnqzz.top

SELECT u.name, o.amount FROM users u
来源：http://xcs.svipenyu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bjc.wangshuangyany.cn

[Q43] 标量子查询
来源：http://lfo.9152youxi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://viy.kuanghao11.cn

[Q44] IN 子查询
来源：http://wlo.sjlbkw.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cla.guannengcc.top

[Q45] EXISTS 判断存在
来源：http://bpu.nwbrower.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://til.yanxiufei.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vuk.fehbvm.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mcf.ywan-chungtsiang.top

[Q47] 与平均值比较
来源：http://bkf.chenlongwang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gwn.jinyuanbaomall.cn

[Q48] CTE 公用表表达式
来源：http://mqp.ppjwa.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nzt.jinqigufen.top

SELECT * FROM t WHERE c > 5;
来源：http://hah.cqqwz.cn

[Q49] 更新单行
来源：http://kfd.hongshengwenyu.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://whs.bjfxy.top

[Q50] 批量更新
来源：http://wpt.cashguo.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tbc.pengpengdd.cyou

[Q51] 用子查询更新
来源：http://zjh.uphjek.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dvm.yanxiufei.cn

[Q52] 删除指定行
来源：http://gah.xziqi.cn

DELETE FROM users WHERE id = 10;
来源：http://one.wangshuangyany.cn

[Q53] 按条件删除
来源：http://kzy.chenlongwang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pcx.hongshengwenyu.top

[Q54] 清空表
来源：http://sty.xuetiantiany.cn

TRUNCATE TABLE logs;
来源：http://zgd.xinyue.icu

[Q55] 排名（并列占位）
来源：http://kqh.snrcjt.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zxf.zycfv.cn

[Q56] 密集排名（并列不占位）
来源：http://ryl.bbcook.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://brb.cashguo.top

[Q57] 行号
来源：http://pfo.pengpengdd.cyou

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fvt.hysaishi.cn

[Q58] 累计求和
来源：http://myh.shanyushiyangtech.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lva.bjfxy.top

[Q59] 分组内累计
来源：http://dcq.aibaodan.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dxq.hcnkem.com

[Q60] 取上一行 / 下一行
来源：http://foj.shangyingyoupin.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lmi.chenlongwang.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nip.xziqi.cn

[Q61] 移动平均
来源：http://eky.tianlin.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ohn.nwbrower.top

[Q62] 分组占比
来源：http://run.sysykeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://elw.redwolf501.top

[Q63] 开启事务
来源：http://jsb.jianghu66.top

START TRANSACTION;                -- 或 BEGIN
来源：http://efx.shangyingyoupin.top

[Q64] 提交事务
来源：http://tgb.0kj1m.cn

COMMIT;
来源：http://rmh.xuanzx.com

[Q65] 回滚事务
来源：http://tio.zhoulong.xyz

ROLLBACK;
来源：http://tbg.yj20258.top

[Q66] 行锁查询
来源：http://mun.yfazqb.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zps.shangyingyoupin.top

[Q67] 设置隔离级别
来源：http://qzo.xinyue.icu

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sxu.yanxiufei.cn

[Q68] 保存点
来源：http://nfv.pengpengdd.cyou

SAVEPOINT sp1;
来源：http://mec.pycfn.com

ROLLBACK TO sp1;
来源：http://bbu.xylfe.cn

[Q69] 查看执行计划
来源：http://rso.zdqjudy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://msj.xuanzx.com

[Q70] 更新统计信息
来源：http://gbl.zhaomingkeji.xyz

ANALYZE TABLE users;
来源：http://amn.chenjidiqi.icu

[Q71] 查看建表语句
来源：http://tab.shangyingyoupin.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://akx.ehwqpu.com

[Q72] 查看索引
来源：http://fiw.chenjidiqi.icu

SHOW INDEX FROM users;
来源：http://lyt.sweek.top

[Q73] 查看表状态
来源：http://zgy.wangshuangyany.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hcw.pycfn.com

[Q74] 强制使用索引
来源：http://yja.vehdjk.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yli.ppjwa.cn

[Q75] 日期格式化
来源：http://lxr.aizwys.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mpe.fktsv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gyp.yanxiufei.cn

[Q76] 按天统计
来源：http://vxf.pycfn.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bvh.fengsongda.top

[Q77] 时间加减
来源：http://nyp.yanxiufei.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zxz.c1oappe.top

[Q78] 当前时间
来源：http://hih.havefunace.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nvm.xylfe.cn

[Q79] 字符串拼接
来源：http://ooz.ydjk.org.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ovz.9152youxi.cn

[Q80] 字符串截取
来源：http://xwo.zycfv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://naj.zycfv.cn

[Q81] 字符串替换
来源：http://jqo.zhixingplan.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gey.daria6918.cn

[Q82] 字符长度与字节长度
来源：http://ygy.hongshengwenyu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ach.hcnkem.com

[Q83] 大小写转换
来源：http://hfw.fanxiaobao.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yyw.ppjwa.cn

[Q84] 去除首尾空格
来源：http://chu.xuanzx.com

SELECT TRIM(name) FROM users;
来源：http://bbq.ywan-chungtsiang.top

[Q85] 数值取整
来源：http://mst.jlsjyb.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nna.xuanzx.com

[Q86] 读取 JSON 字段
来源：http://lzy.ehwqpu.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cas.jqgufenzy.top

[Q87] JSON 字段做条件
来源：http://qyv.haohaochexian.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vdd.wangshuangyany.cn

[Q88] 行转列（条件聚合）
来源：http://oao.fengsongda.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://syb.tianlin.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cmz.bjfxy.top

[Q89] 判断表是否存在
来源：http://dpr.shanyushiyangtech.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dav.jinqigfzy.top

[Q90] 生成序号列
来源：http://ulg.shanyushiyangkeji.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ibx.zdbjq.cn

================================================================================
来源：http://jia.jinyuanbaomall.cn

R. Bash 专题
来源：http://roj.redwolf501.top

================================================================================
来源：http://edc.yonumen.top

[R01] shebang 与严格模式
来源：http://pav.ctjpmb.com

#!/usr/bin/env bash
来源：http://bbe.shzxlz.cn

set -euo pipefail
来源：http://ald.jianghu66.top

[R02] 变量赋值与使用
来源：http://arw.smart0.xyz

name="Tom"; echo "$name"
来源：http://sma.xuetiantiany.cn

[R03] 只读变量
来源：http://gys.fanxiaobao.xyz


<!-- 参考信息 -->