代发 wailian999

[O06] 使用进程池
来源：http://oaz.vehdjk.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yuu.sjlbkw.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://aau.vqdsnc.cn

JS:   // child_process / cluster 模块
来源：http://zmr.yfazqb.com

TS:   // child_process / cluster 模块
来源：http://voq.sufxvd.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ghe.fanxiaobao.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ljs.epnwcf.com

Ruby: // fork 块
来源：http://tgj.aibaodan.cn

C#:   Parallel.For
来源：http://ptg.yueranfly.top

================================================================================
来源：http://pgs.xinyue.icu

P. 常用工具函数
来源：http://mhc.guannengcc.top

================================================================================
来源：http://tbq.cqqwz.cn

[P01] 生成 UUID
来源：http://lpt.jinyuanbaomall.cn

Py:   str(uuid.uuid4())
来源：http://dpf.zdbjq.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cxp.yueranfly.top

JS:   crypto.randomUUID()
来源：http://vmu.cashguo.top

TS:   crypto.randomUUID()
来源：http://vvj.vehdjk.com

Java: UUID.randomUUID().toString()
来源：http://ryh.ivvv.top

Go:   // 用 github.com/google/uuid
来源：http://vwt.cashguo.top

Ruby: SecureRandom.uuid
来源：http://ixj.fengsongda.top

C#:   Guid.NewGuid().ToString()
来源：http://anj.hcnkem.com

[P02] MD5 / SHA256 摘要
来源：http://aou.zhengqikj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tdm.feifeiyinyue.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wbv.c1oappe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hrr.gotoacloud.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vjl.birdmap.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://obm.52xcode.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wcp.dashuyun.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nfv.zhiwuduotai.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fyh.ppjwa.cn

[P03] 生成短随机字符串
来源：http://cat.jqgfzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uja.cqqwz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://znw.hcnkem.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hvf.yfazqb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yhn.bbcook.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vri.jqgufenzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uzm.birdmap.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ggd.guowangkeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uba.ydzc1.top

[P04] 求长度
来源：http://dsb.fktsv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ify.hfpthk.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vxo.ydzc1.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pml.cheryme.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://keq.ybcxt.top

Java: list.size();  map.size();  s.length()
来源：http://orr.yuxming.cn

Go:   len(arr);  len(m)
来源：http://kku.fktsv.cn

Ruby: x.length;  x.size
来源：http://bak.cashguo.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://qge.gaohongyu789.top

[P05] 判断两个对象内容是否相等
来源：http://zkv.xuanzx.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://atn.tianlin.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bgu.bjfxy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ufd.shzxlz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jwu.jyoumei.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fub.jinghuilouyu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pxy.jyoumei.cn

Ruby: a == b
来源：http://fxj.pengpengdd.cyou

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ryn.yvedp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cxa.316326.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pgi.chenjidiqi.icu

PHP:  if (empty($x)) {}
来源：http://dvl.wangshuangyany.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://eny.guannengcc.top

TS:   if (x == null) {}
来源：http://upb.yj202588.top

Java: if (x == null || x.isEmpty()) {}
来源：http://trb.gzhubu.top

Go:   if x == nil {}
来源：http://wtc.fanxiaobao.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eap.chenzaomai.com

C#:   if (x is null) {}
来源：http://fgq.smart0.xyz

[P07] 防抖与节流
来源：http://fsw.sxryk.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yle.zhijiandao.cn

PHP:  // 手写时间戳比较
来源：http://nyd.hfpthk.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tjv.hnxiangtu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ige.cucudq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tai.9152youxi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qya.gzhubu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://lzd.52xcode.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cer.ybcxt.top

[P08] 处理浮点精度问题
来源：http://cur.zhoulong.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://iuj.gzhubu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qdv.sweek.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://efh.jyoumei.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://czt.shanyushiyangtech.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lcv.ehwqpu.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zsp.zhixingplan.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ngo.pengpengdd.cyou

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ifj.bbcook.cn

================================================================================
来源：http://swf.sjlbkw.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lgb.cheryme.top

================================================================================
来源：http://rdb.yvedp.cn

[Q01] 创建表
来源：http://vus.hongshengwenyu.top

CREATE TABLE users (
来源：http://sbi.0kj1m.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kjh.xingfuxueyuan.xyz

name VARCHAR(50) NOT NULL,
来源：http://urq.cheryme.top

email VARCHAR(100) UNIQUE,
来源：http://dcm.epnwcf.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jfu.shangyingyoupin.top

);
来源：http://xit.jinyuanbaomall.cn

[Q02] 创建带外键的表
来源：http://pyn.hnqzz.top

CREATE TABLE orders (
来源：http://vdw.xuanzx.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cmw.hammf.cn

user_id INT NOT NULL,
来源：http://wyw.ybcxt.top

amount DECIMAL(10, 2),
来源：http://pzj.yj20258.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wdb.jiagoushi.top

);
来源：http://gbo.jlsjyb.cn

[Q03] 增加列
来源：http://fus.fanxiaobao.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bxf.ctjpmb.com

[Q04] 修改列类型
来源：http://rag.sjlbkw.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ppv.cqqwz.cn

[Q05] 重命名列
来源：http://nly.jqgufenzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ych.tian-w.cn

[Q06] 删除列
来源：http://eul.snrcjt.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lww.jlsjyb.cn

[Q07] 删除表
来源：http://rog.hysaishi.cn

DROP TABLE IF EXISTS orders;
来源：http://lhk.jinqigfzy.top

[Q08] 创建普通索引
来源：http://uey.nanxuanxn.top

CREATE INDEX idx_users_email ON users(email);
来源：http://qpn.vehdjk.com

[Q09] 创建唯一索引
来源：http://fmc.kuanghao11.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gmd.hysaishi.cn

[Q10] 插入单行
来源：http://tuq.birdmap.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ejt.chenzaomai.com

[Q11] 一次插入多行
来源：http://fjj.jinyuanbaomall.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ase.tian-w.cn

[Q12] 插入后取自增 ID
来源：http://lpy.sweek.top

INSERT INTO users (name) VALUES ('C');
来源：http://jly.jqgfzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dsy.yj20258.top

[Q13] 忽略重复插入
来源：http://zcd.fanxiaobao.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dox.9152youxi.cn

[Q14] 存在则更新（upsert）
来源：http://dsn.nanxuanxn.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ehc.ctjpmb.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zgf.jlsjyb.cn

[Q15] 查询全部
来源：http://dbb.bjfxy.top

SELECT * FROM users;
来源：http://zfr.sweek.top

[Q16] 查询指定列
来源：http://fmi.hcnkem.com

SELECT id, name FROM users;
来源：http://xhv.fanxiaobao.xyz

[Q17] 条件查询
来源：http://iot.hysaishi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fib.0kj1m.cn

[Q18] 模糊匹配
来源：http://qyh.ppjwa.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lpn.yuanzhike.top

[Q19] 范围查询
来源：http://ooz.ehwqpu.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nwf.yongpay.top

[Q20] IN 列表
来源：http://jte.fehbvm.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cow.fzhhl.top

[Q21] 空值判断
来源：http://nes.mhx1999.top

SELECT * FROM users WHERE email IS NULL;
来源：http://kzy.tarul.cn

[Q22] 排序
来源：http://ide.zhijiandao.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wkf.sxryk.cn

[Q23] 分页
来源：http://cvn.sufxvd.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yvl.kuanghao11.cn

[Q24] 去重
来源：http://hcr.xuanzx.com

SELECT DISTINCT city FROM users;
来源：http://qli.jlsjyb.cn

[Q25] 只取前 N 条
来源：http://hst.shzxlz.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wpk.shuidangran.top

[Q26] 计数
来源：http://pwn.shanyushiyangkeji.top

SELECT COUNT(*) FROM users;
来源：http://wnr.cdnleiting.top

[Q27] 条件计数
来源：http://sqa.gzhubu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pmn.hywenlv.cn

[Q28] 求和与平均
来源：http://kja.316326.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wyg.guannengcc.top

[Q29] 最大最小值
来源：http://nyb.snrcjt.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tff.jianghu66.top

[Q30] 分组统计
来源：http://rlq.guowangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fwn.pengpengdd.cyou

[Q31] 分组后过滤
来源：http://cvc.zhaomingkeji.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nvf.c1oappe.top

[Q32] 分组拼接字符串
来源：http://tgx.jinqigufen.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cqw.dashuyun.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dwe.ctjpmb.com

[Q33] 多列分组
来源：http://jdq.sysykeji.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ulp.xingfuxueyuan.xyz

[Q34] 每组取第一条
来源：http://ipv.chenjidiqi.icu

SELECT * FROM (
来源：http://lye.guowangkeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://awk.cqqwz.cn

) t WHERE rn = 1;
来源：http://gox.dashuyun.cn

[Q35] 内连接
来源：http://dge.jianghu66.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gmv.pengpengdd.cyou

[Q36] 左连接
来源：http://yye.zhixingplan.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lap.cqqwz.cn

[Q37] 右连接
来源：http://sjz.jianghu66.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dbr.ivvv.top

[Q38] 全外连接（PostgreSQL）
来源：http://wlb.tanke756.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xft.gzhubu.top

[Q39] 自连接（查上下级）
来源：http://hus.fehbvm.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://zpl.yj20258888.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://unw.havefunace.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ykc.jqgfzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://klw.sweek.top

[Q41] 多表连接
来源：http://vjw.hysaishi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jtm.ivvv.top

JOIN users u ON u.id = o.user_id
来源：http://qrd.fengsongda.top

JOIN products p ON p.id = o.product_id;
来源：http://cei.yj20258.top

[Q42] 连接条件附加过滤
来源：http://ada.daxiang520.top

SELECT u.name, o.amount FROM users u
来源：http://dym.ctjpmb.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yab.birdmap.top

[Q43] 标量子查询
来源：http://qip.jinyuanbaomall.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fzy.daxiang520.top

[Q44] IN 子查询
来源：http://nmf.zhengqikj.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pqw.jlsjyb.cn

[Q45] EXISTS 判断存在
来源：http://xwp.yj20258888.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dro.birdmap.top

[Q46] NOT EXISTS 判断不存在
来源：http://oav.redwolf501.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uta.gotoacloud.top

[Q47] 与平均值比较
来源：http://kxw.cucudq.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ezo.hnxiangtu.top

[Q48] CTE 公用表表达式
来源：http://lyh.sufxvd.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qxr.andypj.xyz

SELECT * FROM t WHERE c > 5;
来源：http://qgd.jqgufenzy.top

[Q49] 更新单行
来源：http://paf.bbcook.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zri.yangfankeji.com

[Q50] 批量更新
来源：http://zol.hysaishi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hnk.meibo888.top

[Q51] 用子查询更新
来源：http://vrp.shzxlz.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rrj.smart0.xyz

[Q52] 删除指定行
来源：http://ref.jinqigufen.top

DELETE FROM users WHERE id = 10;
来源：http://emq.hongshengwenyu.top

[Q53] 按条件删除
来源：http://maw.tarul.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tae.shzxlz.cn

[Q54] 清空表
来源：http://fag.smart0.xyz

TRUNCATE TABLE logs;
来源：http://hoe.gogol.net.cn

[Q55] 排名（并列占位）
来源：http://kdj.ppjwa.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://syz.ivvv.top

[Q56] 密集排名（并列不占位）
来源：http://qzt.ydzc1.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gwc.havefunace.top

[Q57] 行号
来源：http://qys.ydjk.org.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mgs.andypj.xyz

[Q58] 累计求和
来源：http://dbm.aizwys.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ljm.dianchejie.cn

[Q59] 分组内累计
来源：http://ngs.quarkkingdee.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ire.chenlongwang.top

[Q60] 取上一行 / 下一行
来源：http://pxd.jqgufenzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://iix.vehdjk.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ybx.epnwcf.com

[Q61] 移动平均
来源：http://vao.yvedp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wvy.zhoulong.xyz

[Q62] 分组占比
来源：http://sxq.ppjwa.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kof.daxiang520.top

[Q63] 开启事务
来源：http://yhu.jianghu66.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jgl.ivvv.top

[Q64] 提交事务
来源：http://hsb.gzhubu.top

COMMIT;
来源：http://gpm.sysykeji.top

[Q65] 回滚事务
来源：http://anz.jinghuilouyu.cn

ROLLBACK;
来源：http://dve.pengpengdd.cyou

[Q66] 行锁查询
来源：http://moj.xuetiantiany.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://axr.yj202588.top

[Q67] 设置隔离级别
来源：http://evv.zycfv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ear.bjfxy.top

[Q68] 保存点
来源：http://qji.jianghu66.top

SAVEPOINT sp1;
来源：http://tun.svipenyu.cn

ROLLBACK TO sp1;
来源：http://llu.tian-w.cn

[Q69] 查看执行计划
来源：http://cmz.fzhhl.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dxc.zdqjudy.top

[Q70] 更新统计信息
来源：http://kas.yueranfly.top

ANALYZE TABLE users;
来源：http://wdv.zdbjq.cn

[Q71] 查看建表语句
来源：http://nhu.yj20258.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fje.yvedp.cn

[Q72] 查看索引
来源：http://bfl.ivvv.top

SHOW INDEX FROM users;
来源：http://piw.xziqi.cn

[Q73] 查看表状态
来源：http://bhy.pycfn.com

SHOW TABLE STATUS LIKE 'users';
来源：http://wkg.jinghuilouyu.cn

[Q74] 强制使用索引
来源：http://uad.ywan-chungtsiang.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fhs.c1oappe.top

[Q75] 日期格式化
来源：http://zpw.iojbl.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hoa.zhengqikj.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nsu.pengpengdd.cyou

[Q76] 按天统计
来源：http://hlu.zhijiandao.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pah.jyoumei.cn

[Q77] 时间加减
来源：http://tvq.snrcjt.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tqi.shanyushiyangtech.top

[Q78] 当前时间
来源：http://pvr.tanke756.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rov.guowangkeji.top

[Q79] 字符串拼接
来源：http://yxo.9152youxi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rrr.nwbrower.top

[Q80] 字符串截取
来源：http://vnh.daxiang520.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uvx.jyoumei.cn

[Q81] 字符串替换
来源：http://ezg.jiagoushi.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tyk.zhengqikj.top

[Q82] 字符长度与字节长度
来源：http://tym.jinqigfzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tsu.vehdjk.com

[Q83] 大小写转换
来源：http://jzm.hongshengwenyu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ecf.hfpthk.cn

[Q84] 去除首尾空格
来源：http://ssc.ppjwa.cn

SELECT TRIM(name) FROM users;
来源：http://qto.vehdjk.com

[Q85] 数值取整
来源：http://kgc.gzhubu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ods.chenlongwang.top

[Q86] 读取 JSON 字段
来源：http://irc.ydzc1.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ogl.sweek.top

[Q87] JSON 字段做条件
来源：http://qrb.sxryk.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fzz.0kj1m.cn

[Q88] 行转列（条件聚合）
来源：http://bfn.cheryme.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://avy.zhongyouzk.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zbc.aibaodan.cn

[Q89] 判断表是否存在
来源：http://fxf.nanxuanxn.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://aly.wangshuangyany.cn

[Q90] 生成序号列
来源：http://nsv.fengsongda.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ryd.jqgufenzy.top

================================================================================
来源：http://els.gotoacloud.top

R. Bash 专题
来源：http://yld.tanke756.top

================================================================================
来源：http://tmn.svipenyu.cn

[R01] shebang 与严格模式
来源：http://eyv.zhengqikj.top

#!/usr/bin/env bash
来源：http://upn.fktsv.cn

set -euo pipefail
来源：http://ffy.snrcjt.cn

[R02] 变量赋值与使用
来源：http://adv.xziqi.cn

name="Tom"; echo "$name"
来源：http://lhb.wangdashe.top

[R03] 只读变量
来源：http://vht.hywenlv.cn


<!-- 参考信息 -->