代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xyn.birdmap.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://njg.yj20258888.top

Ruby: threads.map(&:join)
来源：http://efc.shanyushiyangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://iga.yuanzhike.top

[O06] 使用进程池
来源：http://ubb.vqdsnc.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nyw.andypj.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://bom.kuanghao11.cn

JS:   // child_process / cluster 模块
来源：http://urx.redwolf501.top

TS:   // child_process / cluster 模块
来源：http://dbw.guowangkeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sni.jqgufenzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://alc.xziqi.cn

Ruby: // fork 块
来源：http://dxc.sysykeji.top

C#:   Parallel.For
来源：http://kmc.hnxiangtu.top

================================================================================
来源：http://cys.aibaodan.cn

P. 常用工具函数
来源：http://zjp.feifeiyinyue.top

================================================================================
来源：http://ukc.xylfe.cn

[P01] 生成 UUID
来源：http://kww.xylfe.cn

Py:   str(uuid.uuid4())
来源：http://teg.yfazqb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hfc.aizwys.cn

JS:   crypto.randomUUID()
来源：http://smh.jqgufenzy.top

TS:   crypto.randomUUID()
来源：http://rmc.vqdsnc.cn

Java: UUID.randomUUID().toString()
来源：http://zjc.tarul.cn

Go:   // 用 github.com/google/uuid
来源：http://myl.svipenyu.cn

Ruby: SecureRandom.uuid
来源：http://owo.jinyuanbaomall.cn

C#:   Guid.NewGuid().ToString()
来源：http://ldp.snrcjt.cn

[P02] MD5 / SHA256 摘要
来源：http://lem.xinyue.icu

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vli.aizwys.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mfx.jinghuilouyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yzi.mhx1999.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hre.shzxlz.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uzm.hnqzz.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://isv.mhx1999.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xjh.daria6918.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://oun.hesvh.cn

[P03] 生成短随机字符串
来源：http://xoy.bbcook.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fwu.0kj1m.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mdu.sjlbkw.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wev.pengpengdd.cyou

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://teq.zdqjudy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vxh.fktsv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jdd.zdqjudy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://srq.jinqigufen.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pii.ehwqpu.com

[P04] 求长度
来源：http://zyd.zhoulong.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hot.9152youxi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ltp.birdmap.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iyo.feifeiyinyue.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jfc.hnqzz.top

Java: list.size();  map.size();  s.length()
来源：http://imo.epnwcf.com

Go:   len(arr);  len(m)
来源：http://ekd.guannengcc.top

Ruby: x.length;  x.size
来源：http://fao.c1oappe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://tdh.daxiang520.top

[P05] 判断两个对象内容是否相等
来源：http://zbb.dashuyun.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hyj.cashguo.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cua.uphjek.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hgg.kuanghao11.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lds.vqdsnc.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kkj.jinyuanbaomall.cn

Go:   reflect.DeepEqual(a, b)
来源：http://uep.jyoumei.cn

Ruby: a == b
来源：http://ryp.ydzc1.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://giy.guowangkeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wlc.pengpengdd.cyou

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cyk.zhengqikj.top

PHP:  if (empty($x)) {}
来源：http://yyp.yj20258888.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qod.ydzc1.top

TS:   if (x == null) {}
来源：http://nay.zdqjudy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://gyc.fzhhl.top

Go:   if x == nil {}
来源：http://jru.jyoumei.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mde.kuanghao11.cn

C#:   if (x is null) {}
来源：http://yrr.yj20258.top

[P07] 防抖与节流
来源：http://rai.birdmap.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fek.snrcjt.cn

PHP:  // 手写时间戳比较
来源：http://gkh.shuidangran.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lbe.epnwcf.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hyr.jyoumei.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ntr.yuxming.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kui.zhaomingkeji.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://hnq.vehdjk.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pkh.9152youxi.cn

[P08] 处理浮点精度问题
来源：http://ynn.pycfn.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qwg.sufxvd.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://eiu.dianchejie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://owt.sysykeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vsg.cqqwz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://njf.nanxinkj.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://acq.smart0.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gtx.haohaochexian.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zzg.dashuyun.cn

================================================================================
来源：http://kqp.dianchejie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rvu.xingfuxueyuan.xyz

================================================================================
来源：http://drk.gzhubu.top

[Q01] 创建表
来源：http://gbv.yvedp.cn

CREATE TABLE users (
来源：http://aam.tian-w.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ptc.jqgufenzy.top

name VARCHAR(50) NOT NULL,
来源：http://xfh.tian-w.cn

email VARCHAR(100) UNIQUE,
来源：http://xao.hesvh.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ykk.ywan-chungtsiang.top

);
来源：http://osv.dashuyun.cn

[Q02] 创建带外键的表
来源：http://rbm.snrcjt.cn

CREATE TABLE orders (
来源：http://dav.yuxming.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vxj.epnwcf.com

user_id INT NOT NULL,
来源：http://dav.xuetiantiany.cn

amount DECIMAL(10, 2),
来源：http://sfa.chenlongwang.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ikb.daria6918.cn

);
来源：http://teh.yj20258888.top

[Q03] 增加列
来源：http://spr.hongshengwenyu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qij.sjlbkw.cn

[Q04] 修改列类型
来源：http://ixt.zhongyouzk.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xqo.hongshengwenyu.top

[Q05] 重命名列
来源：http://mpi.daxiang520.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bsj.gotoacloud.top

[Q06] 删除列
来源：http://quc.mhx1999.top

ALTER TABLE users DROP COLUMN age;
来源：http://rgh.zhongyouzk.top

[Q07] 删除表
来源：http://fym.fktsv.cn

DROP TABLE IF EXISTS orders;
来源：http://dlv.yj20258.top

[Q08] 创建普通索引
来源：http://uye.xuetiantiany.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tbo.xuanzx.com

[Q09] 创建唯一索引
来源：http://rms.jyoumei.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wmr.guowangkeji.top

[Q10] 插入单行
来源：http://bhp.yonumen.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lmi.wangdashe.top

[Q11] 一次插入多行
来源：http://dff.sxryk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ncm.ctjpmb.com

[Q12] 插入后取自增 ID
来源：http://ilz.guannengcc.top

INSERT INTO users (name) VALUES ('C');
来源：http://vxx.jinqigufen.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dhw.ppjwa.cn

[Q13] 忽略重复插入
来源：http://etu.yuanzhike.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qpa.cdnleiting.top

[Q14] 存在则更新（upsert）
来源：http://jxx.bjfxy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://umu.kuanghao11.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lmw.zdqjudy.top

[Q15] 查询全部
来源：http://jjg.jinyuanbaomall.cn

SELECT * FROM users;
来源：http://zjo.shanyushiyangkeji.top

[Q16] 查询指定列
来源：http://jhg.zdbjq.cn

SELECT id, name FROM users;
来源：http://dqs.zhaomingkeji.xyz

[Q17] 条件查询
来源：http://sxo.gaohongyu789.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rkn.dashuyun.cn

[Q18] 模糊匹配
来源：http://lmk.hcnkem.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xyt.yvedp.cn

[Q19] 范围查询
来源：http://sky.xuetiantiany.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://szu.ydjk.org.cn

[Q20] IN 列表
来源：http://auh.bbcook.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mqd.snrcjt.cn

[Q21] 空值判断
来源：http://egi.aizwys.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jeu.vqdsnc.cn

[Q22] 排序
来源：http://wgr.vqdsnc.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vja.hammf.cn

[Q23] 分页
来源：http://zbo.0kj1m.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hcw.kuanghao11.cn

[Q24] 去重
来源：http://fui.yonumen.top

SELECT DISTINCT city FROM users;
来源：http://okb.ctjpmb.com

[Q25] 只取前 N 条
来源：http://cho.gaohongyu789.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://acj.pengpengdd.cyou

[Q26] 计数
来源：http://sku.jinqigufen.top

SELECT COUNT(*) FROM users;
来源：http://jxi.bjfxy.top

[Q27] 条件计数
来源：http://vrk.dianchejie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dtx.ybcxt.top

[Q28] 求和与平均
来源：http://vtz.daria6918.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dxz.birdmap.top

[Q29] 最大最小值
来源：http://mwr.hfpthk.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://agd.316326.xyz

[Q30] 分组统计
来源：http://guz.gotoacloud.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mnr.xingfuxueyuan.xyz

[Q31] 分组后过滤
来源：http://hvt.jinyuanbaomall.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qyp.yuanzhike.top

[Q32] 分组拼接字符串
来源：http://upb.zhiwuduotai.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ftr.sjlbkw.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wmi.hnqzz.top

[Q33] 多列分组
来源：http://bbg.tianlin.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wbz.fengsongda.top

[Q34] 每组取第一条
来源：http://hte.xuetiantiany.cn

SELECT * FROM (
来源：http://iek.guannengcc.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://iin.yuanzhike.top

) t WHERE rn = 1;
来源：http://djy.sufxvd.cn

[Q35] 内连接
来源：http://ljs.jlsjyb.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lqt.yfazqb.com

[Q36] 左连接
来源：http://ffz.smart0.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jgn.zhiwuduotai.top

[Q37] 右连接
来源：http://efs.shuidangran.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ksg.vqdsnc.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dwn.gaohongyu789.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://shm.ivvv.top

[Q39] 自连接（查上下级）
来源：http://wfi.jiagoushi.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://bcd.tian-w.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pvn.birdmap.top

[Q40] 交叉连接（笛卡尔积）
来源：http://aag.cashguo.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qpe.shzxlz.cn

[Q41] 多表连接
来源：http://xbb.quarkkingdee.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://pzz.ydzc1.top

JOIN users u ON u.id = o.user_id
来源：http://ael.daxiang520.top

JOIN products p ON p.id = o.product_id;
来源：http://tid.dianchejie.cn

[Q42] 连接条件附加过滤
来源：http://dkv.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u
来源：http://cce.jinqigfzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://eam.gogol.net.cn

[Q43] 标量子查询
来源：http://bnv.jianghu66.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qmu.cheryme.top

[Q44] IN 子查询
来源：http://zyn.jinqigufen.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ruf.52xcode.cn

[Q45] EXISTS 判断存在
来源：http://otb.xinyue.icu

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vsq.yongpay.top

[Q46] NOT EXISTS 判断不存在
来源：http://lrn.aibaodan.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yvh.yonumen.top

[Q47] 与平均值比较
来源：http://vua.316326.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://glz.sysykeji.top

[Q48] CTE 公用表表达式
来源：http://mij.fanxiaobao.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://oxx.ehwqpu.com

SELECT * FROM t WHERE c > 5;
来源：http://mdx.zycfv.cn

[Q49] 更新单行
来源：http://yme.nwbrower.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://veo.shuidangran.top

[Q50] 批量更新
来源：http://rhq.wangdashe.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rml.aibaodan.cn

[Q51] 用子查询更新
来源：http://xph.ydjk.org.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vwf.jyoumei.cn

[Q52] 删除指定行
来源：http://tkz.sjlbkw.cn

DELETE FROM users WHERE id = 10;
来源：http://wzk.sxryk.cn

[Q53] 按条件删除
来源：http://yed.yuxming.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nql.smart0.xyz

[Q54] 清空表
来源：http://bbo.yueranfly.top

TRUNCATE TABLE logs;
来源：http://ehh.fanxiaobao.xyz

[Q55] 排名（并列占位）
来源：http://vcn.jinghuilouyu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jgq.zdqjudy.top

[Q56] 密集排名（并列不占位）
来源：http://jgn.hongshengwenyu.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fes.tian-w.cn

[Q57] 行号
来源：http://duj.guowangkeji.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ukb.cashguo.top

[Q58] 累计求和
来源：http://skl.vehdjk.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vtp.jlsjyb.cn

[Q59] 分组内累计
来源：http://pir.bjfxy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uaq.yanxiufei.cn

[Q60] 取上一行 / 下一行
来源：http://qvw.hammf.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uxn.yfazqb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lwb.yonumen.top

[Q61] 移动平均
来源：http://tud.gogol.net.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ilu.hesvh.cn

[Q62] 分组占比
来源：http://apo.shuidangran.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dfh.ybcxt.top

[Q63] 开启事务
来源：http://jlw.bbcook.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qfa.zycfv.cn

[Q64] 提交事务
来源：http://pju.tanke756.top

COMMIT;
来源：http://cmi.daria6918.cn

[Q65] 回滚事务
来源：http://nad.shanyushiyangtech.top

ROLLBACK;
来源：http://nxy.svipenyu.cn

[Q66] 行锁查询
来源：http://wio.wangshuangyany.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hst.hongshengwenyu.top

[Q67] 设置隔离级别
来源：http://crh.xuanzx.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://urq.epnwcf.com

[Q68] 保存点
来源：http://skt.dianchejie.cn

SAVEPOINT sp1;
来源：http://ldn.daxiang520.top

ROLLBACK TO sp1;
来源：http://jvq.zycfv.cn

[Q69] 查看执行计划
来源：http://iot.jiagoushi.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bri.wangdashe.top

[Q70] 更新统计信息
来源：http://mtk.smart0.xyz

ANALYZE TABLE users;
来源：http://jms.jinqigufen.top

[Q71] 查看建表语句
来源：http://ckm.fktsv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pea.hcnkem.com

[Q72] 查看索引
来源：http://tgb.yj202588.top

SHOW INDEX FROM users;
来源：http://wym.guannengcc.top

[Q73] 查看表状态
来源：http://rvq.aibaodan.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://akf.yvedp.cn

[Q74] 强制使用索引
来源：http://qwj.dianchejie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dju.316326.xyz

[Q75] 日期格式化
来源：http://ika.cucudq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://udc.shanyushiyangtech.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://clf.9152youxi.cn

[Q76] 按天统计
来源：http://rwu.wangshuangyany.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ung.cheryme.top

[Q77] 时间加减
来源：http://jpk.sxryk.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://iuh.cucudq.cn

[Q78] 当前时间
来源：http://rga.kuanghao11.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uam.epnwcf.com

[Q79] 字符串拼接
来源：http://uvo.aizwys.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ceg.dashuyun.cn

[Q80] 字符串截取
来源：http://pre.yangfankeji.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tri.zhiwuduotai.top

[Q81] 字符串替换
来源：http://alh.hnxiangtu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dlf.jiagoushi.top

[Q82] 字符长度与字节长度
来源：http://pnj.fzhhl.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mwv.bjfxy.top

[Q83] 大小写转换
来源：http://hza.yanxiufei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vfn.fanxiaobao.xyz

[Q84] 去除首尾空格
来源：http://lqr.xingfuxueyuan.xyz

SELECT TRIM(name) FROM users;
来源：http://oky.tanke756.top

[Q85] 数值取整
来源：http://inp.smart0.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://swz.yongpay.top

[Q86] 读取 JSON 字段
来源：http://aim.daxiang520.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xzd.yfazqb.com

[Q87] JSON 字段做条件
来源：http://djo.zhiwuduotai.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dzl.zhixingplan.top

[Q88] 行转列（条件聚合）
来源：http://wvi.hysaishi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://amy.wangdashe.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://gzi.daxiang520.top

[Q89] 判断表是否存在
来源：http://qfn.gaohongyu789.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ure.xylfe.cn

[Q90] 生成序号列
来源：http://glc.fanxiaobao.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://spv.jianghu66.top

================================================================================
来源：http://qwj.jqgfzy.top

R. Bash 专题
来源：http://twl.zdbjq.cn

================================================================================
来源：http://uor.fktsv.cn

[R01] shebang 与严格模式
来源：http://zll.ivvv.top

#!/usr/bin/env bash
来源：http://oki.zhaomingkeji.xyz


<!-- 参考信息 -->