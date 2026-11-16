代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fbc.kuanghao11.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cbo.cqqwz.cn

C#:   async Task F() { await G(); }
来源：http://zem.pycfn.com

[O05] 并发执行并等待全部完成
来源：http://yxd.shanyushiyangtech.top

Py:   asyncio.gather(*tasks)
来源：http://hln.fzhhl.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://omi.zhixingplan.top

JS:   await Promise.all(tasks)
来源：http://uwh.hysaishi.cn

TS:   await Promise.all(tasks)
来源：http://kiu.zhengqikj.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zki.gotoacloud.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tyd.smart0.xyz

Ruby: threads.map(&:join)
来源：http://fmn.zycfv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://omh.nanxinkj.top

[O06] 使用进程池
来源：http://xvc.bbcook.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nbs.shanyushiyangkeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fys.jinghuilouyu.cn

JS:   // child_process / cluster 模块
来源：http://kwn.ybcxt.top

TS:   // child_process / cluster 模块
来源：http://qyn.yfazqb.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lll.gaohongyu789.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zny.zhiwuduotai.top

Ruby: // fork 块
来源：http://pfe.52xcode.cn

C#:   Parallel.For
来源：http://miz.nwbrower.top

================================================================================
来源：http://cpg.wangdashe.top

P. 常用工具函数
来源：http://qrr.jinqigufen.top

================================================================================
来源：http://sdj.fengsongda.top

[P01] 生成 UUID
来源：http://ulg.havefunace.top

Py:   str(uuid.uuid4())
来源：http://luu.xziqi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zey.ydzc1.top

JS:   crypto.randomUUID()
来源：http://ooh.yuxming.cn

TS:   crypto.randomUUID()
来源：http://khv.tianlin.xyz

Java: UUID.randomUUID().toString()
来源：http://qmv.jiagoushi.top

Go:   // 用 github.com/google/uuid
来源：http://eie.ppjwa.cn

Ruby: SecureRandom.uuid
来源：http://led.epnwcf.com

C#:   Guid.NewGuid().ToString()
来源：http://gxm.cheryme.top

[P02] MD5 / SHA256 摘要
来源：http://mcw.9152youxi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dam.quarkkingdee.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://slb.ywan-chungtsiang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://egi.wangshuangyany.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ayk.nanxuanxn.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uck.xuetiantiany.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ees.cucudq.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sjy.havefunace.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rys.tian-w.cn

[P03] 生成短随机字符串
来源：http://fcf.wangdashe.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://myc.feifeiyinyue.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wrk.ehwqpu.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ctb.yongpay.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tsw.zhengqikj.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fhv.guannengcc.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wyh.havefunace.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://pqg.mhx1999.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ofh.bbcook.cn

[P04] 求长度
来源：http://ivw.aibaodan.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mkx.dianchejie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qnt.ydjk.org.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://elq.daxiang520.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yod.fzhhl.top

Java: list.size();  map.size();  s.length()
来源：http://eba.cdnleiting.top

Go:   len(arr);  len(m)
来源：http://aez.sweek.top

Ruby: x.length;  x.size
来源：http://jmm.ctjpmb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://kln.ctjpmb.com

[P05] 判断两个对象内容是否相等
来源：http://wym.gzhubu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://oon.sxryk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://azf.316326.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://onh.ivvv.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tzt.xingfuxueyuan.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sqx.nwbrower.top

Go:   reflect.DeepEqual(a, b)
来源：http://hag.jlsjyb.cn

Ruby: a == b
来源：http://xmz.dianchejie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://knj.yonumen.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jhd.havefunace.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ycg.zhixingplan.top

PHP:  if (empty($x)) {}
来源：http://wkz.yueranfly.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pxz.yj20258888.top

TS:   if (x == null) {}
来源：http://gnv.xziqi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://rrj.sufxvd.cn

Go:   if x == nil {}
来源：http://hao.sysykeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jdu.vqdsnc.cn

C#:   if (x is null) {}
来源：http://uhs.chenjidiqi.icu

[P07] 防抖与节流
来源：http://kgb.daxiang520.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xbu.jiagoushi.top

PHP:  // 手写时间戳比较
来源：http://uqf.sjlbkw.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lpm.vehdjk.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tga.yj202588.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mhx.yuanzhike.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ovb.pengpengdd.cyou

Ruby: // 手写闭包 + Time.now 判断
来源：http://fpj.yangfankeji.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://liu.jinqigufen.top

[P08] 处理浮点精度问题
来源：http://rch.zycfv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fhp.bbcook.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hqp.dashuyun.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://peg.xinyue.icu

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jgz.yanxiufei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://agt.c1oappe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lgr.jinqigufen.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vpm.dashuyun.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ewc.yj20258.top

================================================================================
来源：http://tce.fanxiaobao.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://myi.yuanzhike.top

================================================================================
来源：http://leu.yj20258888.top

[Q01] 创建表
来源：http://ocn.nwbrower.top

CREATE TABLE users (
来源：http://rxk.feifeiyinyue.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tbg.mhx1999.top

name VARCHAR(50) NOT NULL,
来源：http://avk.guowangkeji.top

email VARCHAR(100) UNIQUE,
来源：http://dvk.pengpengdd.cyou

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pgr.ywan-chungtsiang.top

);
来源：http://prg.haohaochexian.top

[Q02] 创建带外键的表
来源：http://cns.cucudq.cn

CREATE TABLE orders (
来源：http://eam.hywenlv.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vbl.tanke756.top

user_id INT NOT NULL,
来源：http://mhr.aibaodan.cn

amount DECIMAL(10, 2),
来源：http://wka.fengsongda.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pcr.hcnkem.com

);
来源：http://con.jqgufenzy.top

[Q03] 增加列
来源：http://lhf.chenlongwang.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lgf.chenlongwang.top

[Q04] 修改列类型
来源：http://qco.yuanzhike.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sjy.jinghuilouyu.cn

[Q05] 重命名列
来源：http://mev.nanxuanxn.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rmk.yueranfly.top

[Q06] 删除列
来源：http://tvu.yuxming.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xqr.vehdjk.com

[Q07] 删除表
来源：http://bqq.sjlbkw.cn

DROP TABLE IF EXISTS orders;
来源：http://jtx.zhongyouzk.top

[Q08] 创建普通索引
来源：http://pqg.quarkkingdee.top

CREATE INDEX idx_users_email ON users(email);
来源：http://eqi.jinyuanbaomall.cn

[Q09] 创建唯一索引
来源：http://knf.xuetiantiany.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://djb.yuanzhike.top

[Q10] 插入单行
来源：http://nch.cheryme.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oos.ctjpmb.com

[Q11] 一次插入多行
来源：http://vsa.tian-w.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://drp.fengsongda.top

[Q12] 插入后取自增 ID
来源：http://lix.iojbl.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ckf.havefunace.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://plt.ywan-chungtsiang.top

[Q13] 忽略重复插入
来源：http://vuh.ivvv.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://adt.jinqigfzy.top

[Q14] 存在则更新（upsert）
来源：http://smz.dashuyun.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yow.zhiwuduotai.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nso.c1oappe.top

[Q15] 查询全部
来源：http://riy.guannengcc.top

SELECT * FROM users;
来源：http://aht.jiagoushi.top

[Q16] 查询指定列
来源：http://sky.pycfn.com

SELECT id, name FROM users;
来源：http://gek.redwolf501.top

[Q17] 条件查询
来源：http://pfj.pengpengdd.cyou

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wer.yongpay.top

[Q18] 模糊匹配
来源：http://txh.sjlbkw.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ojd.316326.xyz

[Q19] 范围查询
来源：http://bmp.0kj1m.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vfz.epnwcf.com

[Q20] IN 列表
来源：http://yof.fktsv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dzp.yonumen.top

[Q21] 空值判断
来源：http://rmw.tian-w.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://aap.xinyue.icu

[Q22] 排序
来源：http://knr.jqgufenzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pom.316326.xyz

[Q23] 分页
来源：http://xpu.tianlin.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cuk.shzxlz.cn

[Q24] 去重
来源：http://ola.vehdjk.com

SELECT DISTINCT city FROM users;
来源：http://hzu.vqdsnc.cn

[Q25] 只取前 N 条
来源：http://oqe.shzxlz.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://eol.fzhhl.top

[Q26] 计数
来源：http://ruc.zycfv.cn

SELECT COUNT(*) FROM users;
来源：http://fym.zhengqikj.top

[Q27] 条件计数
来源：http://dpm.shangyingyoupin.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fub.zhixingplan.top

[Q28] 求和与平均
来源：http://zmv.jqgfzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://duf.zhengqikj.top

[Q29] 最大最小值
来源：http://yic.hongshengwenyu.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://tmh.9152youxi.cn

[Q30] 分组统计
来源：http://gmo.birdmap.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pfk.shuidangran.top

[Q31] 分组后过滤
来源：http://ekx.meibo888.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://esb.daxiang520.top

[Q32] 分组拼接字符串
来源：http://hsq.ehwqpu.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cwb.0kj1m.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://imb.fehbvm.com

[Q33] 多列分组
来源：http://muw.hfpthk.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tpy.fehbvm.com

[Q34] 每组取第一条
来源：http://bic.9152youxi.cn

SELECT * FROM (
来源：http://bbb.feifeiyinyue.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bjz.chenzaomai.com

) t WHERE rn = 1;
来源：http://bws.dashuyun.cn

[Q35] 内连接
来源：http://vxo.hnxiangtu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://agp.jinqigufen.top

[Q36] 左连接
来源：http://odl.sysykeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jlh.tian-w.cn

[Q37] 右连接
来源：http://hvc.zhongyouzk.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gbz.hnqzz.top

[Q38] 全外连接（PostgreSQL）
来源：http://qbi.nanxinkj.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xbj.fzhhl.top

[Q39] 自连接（查上下级）
来源：http://moc.0kj1m.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://tmc.jiagoushi.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lol.shanyushiyangtech.top

[Q40] 交叉连接（笛卡尔积）
来源：http://oty.sweek.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://guu.jqgufenzy.top

[Q41] 多表连接
来源：http://ojy.zycfv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yvt.iojbl.cn

JOIN users u ON u.id = o.user_id
来源：http://hio.wangdashe.top

JOIN products p ON p.id = o.product_id;
来源：http://wqw.tian-w.cn

[Q42] 连接条件附加过滤
来源：http://vzf.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u
来源：http://tgf.sysykeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wcm.fktsv.cn

[Q43] 标量子查询
来源：http://oxi.svipenyu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fdy.smart0.xyz

[Q44] IN 子查询
来源：http://vfv.shuidangran.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jui.ctjpmb.com

[Q45] EXISTS 判断存在
来源：http://jlz.hnxiangtu.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ccf.cqqwz.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sig.tarul.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nbh.iojbl.cn

[Q47] 与平均值比较
来源：http://slq.zhengqikj.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cgh.shuidangran.top

[Q48] CTE 公用表表达式
来源：http://tdg.jiagoushi.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vze.ehwqpu.com

SELECT * FROM t WHERE c > 5;
来源：http://qub.xziqi.cn

[Q49] 更新单行
来源：http://bap.hnxiangtu.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://loc.dianchejie.cn

[Q50] 批量更新
来源：http://vvz.bjfxy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fat.fengsongda.top

[Q51] 用子查询更新
来源：http://jxa.redwolf501.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://awv.yj202588.top

[Q52] 删除指定行
来源：http://vbq.ehwqpu.com

DELETE FROM users WHERE id = 10;
来源：http://mem.jyoumei.cn

[Q53] 按条件删除
来源：http://ffc.yj20258888.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://per.fanxiaobao.xyz

[Q54] 清空表
来源：http://yjd.jqgufenzy.top

TRUNCATE TABLE logs;
来源：http://rdt.yj202588.top

[Q55] 排名（并列占位）
来源：http://bej.zhoulong.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sjd.yongpay.top

[Q56] 密集排名（并列不占位）
来源：http://qqb.epnwcf.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fyl.xuanzx.com

[Q57] 行号
来源：http://svz.hysaishi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wfq.cdnleiting.top

[Q58] 累计求和
来源：http://iqp.gotoacloud.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qud.gaohongyu789.top

[Q59] 分组内累计
来源：http://fyv.shuidangran.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://psj.zhijiandao.cn

[Q60] 取上一行 / 下一行
来源：http://rvx.jqgufenzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uvg.guannengcc.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yjx.hesvh.cn

[Q61] 移动平均
来源：http://lei.birdmap.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://byv.hammf.cn

[Q62] 分组占比
来源：http://okn.gogol.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vad.zhengqikj.top

[Q63] 开启事务
来源：http://pyq.shuidangran.top

START TRANSACTION;                -- 或 BEGIN
来源：http://otw.ppjwa.cn

[Q64] 提交事务
来源：http://eyw.ybcxt.top

COMMIT;
来源：http://drm.yuanzhike.top

[Q65] 回滚事务
来源：http://cac.xuanzx.com

ROLLBACK;
来源：http://pbk.hnqzz.top

[Q66] 行锁查询
来源：http://tga.hongshengwenyu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xor.snrcjt.cn

[Q67] 设置隔离级别
来源：http://xmr.ehwqpu.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uqd.nanxuanxn.top

[Q68] 保存点
来源：http://sdj.birdmap.top

SAVEPOINT sp1;
来源：http://jit.316326.xyz

ROLLBACK TO sp1;
来源：http://zsw.guowangkeji.top

[Q69] 查看执行计划
来源：http://hyo.yfazqb.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ibm.chenjidiqi.icu

[Q70] 更新统计信息
来源：http://tym.guannengcc.top

ANALYZE TABLE users;
来源：http://vdd.zhijiandao.cn

[Q71] 查看建表语句
来源：http://fpn.hammf.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eio.xuanzx.com

[Q72] 查看索引
来源：http://eoe.hongshengwenyu.top

SHOW INDEX FROM users;
来源：http://jmw.nanxuanxn.top

[Q73] 查看表状态
来源：http://lbe.haohaochexian.top

SHOW TABLE STATUS LIKE 'users';
来源：http://wtm.hnqzz.top

[Q74] 强制使用索引
来源：http://uuh.hfpthk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rgx.jinqigufen.top

[Q75] 日期格式化
来源：http://dfg.sysykeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ibl.sufxvd.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://obw.chenlongwang.top

[Q76] 按天统计
来源：http://fxi.chenlongwang.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yrj.jyoumei.cn

[Q77] 时间加减
来源：http://kuj.pengpengdd.cyou

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fxf.xuetiantiany.cn

[Q78] 当前时间
来源：http://cup.hnqzz.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ifo.nwbrower.top

[Q79] 字符串拼接
来源：http://iwv.cucudq.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ekn.hnqzz.top

[Q80] 字符串截取
来源：http://kqn.jinghuilouyu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://sun.hfpthk.cn

[Q81] 字符串替换
来源：http://kjg.yuxming.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cil.chenlongwang.top

[Q82] 字符长度与字节长度
来源：http://alq.sjlbkw.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hfg.cdnleiting.top

[Q83] 大小写转换
来源：http://gwl.sysykeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pim.svipenyu.cn

[Q84] 去除首尾空格
来源：http://swg.yj202588.top

SELECT TRIM(name) FROM users;
来源：http://xxg.tanke756.top

[Q85] 数值取整
来源：http://luq.ybcxt.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rtp.vehdjk.com

[Q86] 读取 JSON 字段
来源：http://xyk.tarul.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gbl.jianghu66.top

[Q87] JSON 字段做条件
来源：http://bnv.hongshengwenyu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://czb.pengpengdd.cyou

[Q88] 行转列（条件聚合）
来源：http://fxn.chenjidiqi.icu

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://awn.cdnleiting.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wcf.hongshengwenyu.top

[Q89] 判断表是否存在
来源：http://rvr.nanxuanxn.top


<!-- 参考信息 -->