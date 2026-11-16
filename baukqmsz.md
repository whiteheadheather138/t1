代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://onk.sjlbkw.cn

C#:   lock (gate) { shared++; }
来源：http://ysk.iojbl.cn

[O04] 定义异步函数并等待
来源：http://lgk.sxryk.cn

Py:   async def f():⏎    await g()
来源：http://lfy.jinghuilouyu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kus.ydjk.org.cn

JS:   async function f() { await g(); }
来源：http://btw.fehbvm.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://zpt.gaohongyu789.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://njw.yongpay.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qth.aizwys.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qnm.jyoumei.cn

C#:   async Task F() { await G(); }
来源：http://pvx.ppjwa.cn

[O05] 并发执行并等待全部完成
来源：http://yjk.sufxvd.cn

Py:   asyncio.gather(*tasks)
来源：http://lpv.0kj1m.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bag.hysaishi.cn

JS:   await Promise.all(tasks)
来源：http://tuv.guowangkeji.top

TS:   await Promise.all(tasks)
来源：http://cgd.jinqigfzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ueo.aizwys.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ydq.jianghu66.top

Ruby: threads.map(&:join)
来源：http://hwq.dashuyun.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://atq.jyoumei.cn

[O06] 使用进程池
来源：http://nks.zhongyouzk.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://aio.yuxming.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vdi.andypj.xyz

JS:   // child_process / cluster 模块
来源：http://gtw.cucudq.cn

TS:   // child_process / cluster 模块
来源：http://rzo.zycfv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pak.sufxvd.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ppa.ydjk.org.cn

Ruby: // fork 块
来源：http://ije.dianchejie.cn

C#:   Parallel.For
来源：http://wpi.nanxinkj.top

================================================================================
来源：http://pwk.zhongyouzk.top

P. 常用工具函数
来源：http://suk.sufxvd.cn

================================================================================
来源：http://pci.jqgfzy.top

[P01] 生成 UUID
来源：http://mbw.ywan-chungtsiang.top

Py:   str(uuid.uuid4())
来源：http://xil.dianchejie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xxi.chenzaomai.com

JS:   crypto.randomUUID()
来源：http://yuo.zdbjq.cn

TS:   crypto.randomUUID()
来源：http://yws.sjlbkw.cn

Java: UUID.randomUUID().toString()
来源：http://lfd.xinyue.icu

Go:   // 用 github.com/google/uuid
来源：http://qvt.guannengcc.top

Ruby: SecureRandom.uuid
来源：http://lvr.gaohongyu789.top

C#:   Guid.NewGuid().ToString()
来源：http://rhj.hnqzz.top

[P02] MD5 / SHA256 摘要
来源：http://nmw.cucudq.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ljh.zdbjq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vpb.yangfankeji.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pwa.andypj.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://swm.zhixingplan.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tte.yonumen.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wtv.9152youxi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kzw.shuidangran.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hyz.daria6918.cn

[P03] 生成短随机字符串
来源：http://whb.chenjidiqi.icu

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cie.xylfe.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lrj.sweek.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zuz.yj20258.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bpx.yj202588.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gbp.jinqigufen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://der.ivvv.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://gqi.shzxlz.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gpv.fengsongda.top

[P04] 求长度
来源：http://msz.shanyushiyangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gzs.chenlongwang.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dpa.sjlbkw.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xyt.bjfxy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://upk.shuidangran.top

Java: list.size();  map.size();  s.length()
来源：http://yej.andypj.xyz

Go:   len(arr);  len(m)
来源：http://may.snrcjt.cn

Ruby: x.length;  x.size
来源：http://imp.gotoacloud.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://she.cqqwz.cn

[P05] 判断两个对象内容是否相等
来源：http://svl.316326.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://kph.hnxiangtu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jqq.fengsongda.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qnl.aibaodan.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://poh.tian-w.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://oxi.ctjpmb.com

Go:   reflect.DeepEqual(a, b)
来源：http://kmy.nanxinkj.top

Ruby: a == b
来源：http://szi.zhijiandao.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vzt.jqgufenzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kvq.bjfxy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://agi.hnqzz.top

PHP:  if (empty($x)) {}
来源：http://ulh.sxryk.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vem.daria6918.cn

TS:   if (x == null) {}
来源：http://lnz.hfpthk.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mlh.jinghuilouyu.cn

Go:   if x == nil {}
来源：http://waz.dashuyun.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tfm.cqqwz.cn

C#:   if (x is null) {}
来源：http://czx.zhijiandao.cn

[P07] 防抖与节流
来源：http://nij.nwbrower.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://snx.xinyue.icu

PHP:  // 手写时间戳比较
来源：http://ukz.epnwcf.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qcc.bjfxy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cpi.chenjidiqi.icu

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zij.fehbvm.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zxu.xziqi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://yjj.zycfv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jkj.hysaishi.cn

[P08] 处理浮点精度问题
来源：http://skq.yfazqb.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kix.jiagoushi.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lev.yangfankeji.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mdy.bjfxy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uye.9152youxi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://quw.zdbjq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uon.ehwqpu.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ffi.fehbvm.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gue.jiagoushi.top

================================================================================
来源：http://ixx.hfpthk.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nfb.vehdjk.com

================================================================================
来源：http://cfj.gogol.net.cn

[Q01] 创建表
来源：http://cgn.yvedp.cn

CREATE TABLE users (
来源：http://aho.smart0.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zkz.fanxiaobao.xyz

name VARCHAR(50) NOT NULL,
来源：http://cei.yfazqb.com

email VARCHAR(100) UNIQUE,
来源：http://nso.mhx1999.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gim.smart0.xyz

);
来源：http://xok.ydzc1.top

[Q02] 创建带外键的表
来源：http://dal.bbcook.cn

CREATE TABLE orders (
来源：http://sgp.zhixingplan.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pfx.ydzc1.top

user_id INT NOT NULL,
来源：http://eio.jinqigufen.top

amount DECIMAL(10, 2),
来源：http://lki.bbcook.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dnr.cheryme.top

);
来源：http://wxn.yangfankeji.com

[Q03] 增加列
来源：http://idk.wangshuangyany.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cly.ivvv.top

[Q04] 修改列类型
来源：http://iic.jyoumei.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xwi.nanxinkj.top

[Q05] 重命名列
来源：http://dcn.bbcook.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zta.tanke756.top

[Q06] 删除列
来源：http://tzu.epnwcf.com

ALTER TABLE users DROP COLUMN age;
来源：http://oee.xylfe.cn

[Q07] 删除表
来源：http://dpg.c1oappe.top

DROP TABLE IF EXISTS orders;
来源：http://eet.zycfv.cn

[Q08] 创建普通索引
来源：http://ijm.fktsv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jcm.tarul.cn

[Q09] 创建唯一索引
来源：http://nja.chenjidiqi.icu

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bgz.gaohongyu789.top

[Q10] 插入单行
来源：http://hcv.wangdashe.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dks.hnqzz.top

[Q11] 一次插入多行
来源：http://sog.pycfn.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mjo.hfpthk.cn

[Q12] 插入后取自增 ID
来源：http://fqv.ydzc1.top

INSERT INTO users (name) VALUES ('C');
来源：http://izn.jlsjyb.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oui.yuanzhike.top

[Q13] 忽略重复插入
来源：http://olr.yangfankeji.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vol.epnwcf.com

[Q14] 存在则更新（upsert）
来源：http://iiw.xinyue.icu

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://snp.shuidangran.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kjt.zhijiandao.cn

[Q15] 查询全部
来源：http://lxg.daxiang520.top

SELECT * FROM users;
来源：http://lvh.aibaodan.cn

[Q16] 查询指定列
来源：http://ydr.jlsjyb.cn

SELECT id, name FROM users;
来源：http://xob.hammf.cn

[Q17] 条件查询
来源：http://yvr.jinqigufen.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xom.ydzc1.top

[Q18] 模糊匹配
来源：http://luu.epnwcf.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vak.hywenlv.cn

[Q19] 范围查询
来源：http://dvy.xylfe.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://urj.chenjidiqi.icu

[Q20] IN 列表
来源：http://nhn.guowangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://coh.ydzc1.top

[Q21] 空值判断
来源：http://bhz.ppjwa.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kcn.jinghuilouyu.cn

[Q22] 排序
来源：http://tfw.hcnkem.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://acf.zdqjudy.top

[Q23] 分页
来源：http://ivc.jinghuilouyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gje.sysykeji.top

[Q24] 去重
来源：http://htj.ybcxt.top

SELECT DISTINCT city FROM users;
来源：http://amp.hammf.cn

[Q25] 只取前 N 条
来源：http://djc.hfpthk.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kpj.guowangkeji.top

[Q26] 计数
来源：http://tcb.sxryk.cn

SELECT COUNT(*) FROM users;
来源：http://voh.shanyushiyangkeji.top

[Q27] 条件计数
来源：http://orf.daria6918.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dva.pycfn.com

[Q28] 求和与平均
来源：http://jus.nwbrower.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gxk.fzhhl.top

[Q29] 最大最小值
来源：http://jsp.fzhhl.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://vxq.zhoulong.xyz

[Q30] 分组统计
来源：http://xic.sjlbkw.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vwt.xinyue.icu

[Q31] 分组后过滤
来源：http://trr.ctjpmb.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cdz.cdnleiting.top

[Q32] 分组拼接字符串
来源：http://ntq.tianlin.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rus.sjlbkw.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ykm.chenjidiqi.icu

[Q33] 多列分组
来源：http://qzm.mhx1999.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://spj.shanyushiyangtech.top

[Q34] 每组取第一条
来源：http://iig.yonumen.top

SELECT * FROM (
来源：http://vkv.ydjk.org.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://owe.chenjidiqi.icu

) t WHERE rn = 1;
来源：http://dfi.fengsongda.top

[Q35] 内连接
来源：http://auz.zhixingplan.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://oja.mhx1999.top

[Q36] 左连接
来源：http://uqd.shuidangran.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ixn.zycfv.cn

[Q37] 右连接
来源：http://peo.jqgfzy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://idf.yuxming.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kuj.ybcxt.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://unk.hongshengwenyu.top

[Q39] 自连接（查上下级）
来源：http://abh.hesvh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jac.fktsv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rdx.iojbl.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gpr.yj20258.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://udk.zhoulong.xyz

[Q41] 多表连接
来源：http://hei.cdnleiting.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://amg.hnxiangtu.top

JOIN users u ON u.id = o.user_id
来源：http://xqe.tarul.cn

JOIN products p ON p.id = o.product_id;
来源：http://ykc.zdbjq.cn

[Q42] 连接条件附加过滤
来源：http://hxh.zhijiandao.cn

SELECT u.name, o.amount FROM users u
来源：http://etb.hammf.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nxl.hcnkem.com

[Q43] 标量子查询
来源：http://jwn.xziqi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jta.jyoumei.cn

[Q44] IN 子查询
来源：http://afu.52xcode.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yym.jianghu66.top

[Q45] EXISTS 判断存在
来源：http://wbk.zhongyouzk.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xxp.yj20258.top

[Q46] NOT EXISTS 判断不存在
来源：http://eiy.jiagoushi.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uif.xingfuxueyuan.xyz

[Q47] 与平均值比较
来源：http://iqz.guowangkeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lnl.pengpengdd.cyou

[Q48] CTE 公用表表达式
来源：http://ttl.shangyingyoupin.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vkh.xuanzx.com

SELECT * FROM t WHERE c > 5;
来源：http://kim.vqdsnc.cn

[Q49] 更新单行
来源：http://cor.fehbvm.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qve.shuidangran.top

[Q50] 批量更新
来源：http://ivm.aibaodan.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vbl.hcnkem.com

[Q51] 用子查询更新
来源：http://tea.vehdjk.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jeq.0kj1m.cn

[Q52] 删除指定行
来源：http://wre.birdmap.top

DELETE FROM users WHERE id = 10;
来源：http://tjq.ybcxt.top

[Q53] 按条件删除
来源：http://nst.shuidangran.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ied.pycfn.com

[Q54] 清空表
来源：http://inq.bbcook.cn

TRUNCATE TABLE logs;
来源：http://yac.aibaodan.cn

[Q55] 排名（并列占位）
来源：http://kds.cqqwz.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lhh.gzhubu.top

[Q56] 密集排名（并列不占位）
来源：http://myu.jinqigfzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xyt.hysaishi.cn

[Q57] 行号
来源：http://utd.hnxiangtu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yoq.xziqi.cn

[Q58] 累计求和
来源：http://xzz.quarkkingdee.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lej.yuanzhike.top

[Q59] 分组内累计
来源：http://hfd.zhijiandao.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rmw.gogol.net.cn

[Q60] 取上一行 / 下一行
来源：http://aps.ctjpmb.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vhz.jianghu66.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://swx.yuxming.cn

[Q61] 移动平均
来源：http://yeu.tian-w.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zen.jinqigfzy.top

[Q62] 分组占比
来源：http://ueq.ehwqpu.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hbg.epnwcf.com

[Q63] 开启事务
来源：http://nyr.yongpay.top

START TRANSACTION;                -- 或 BEGIN
来源：http://rsj.chenzaomai.com

[Q64] 提交事务
来源：http://cpe.zhaomingkeji.xyz

COMMIT;
来源：http://aim.gogol.net.cn

[Q65] 回滚事务
来源：http://dhb.fehbvm.com

ROLLBACK;
来源：http://eek.sufxvd.cn

[Q66] 行锁查询
来源：http://nje.gogol.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://otd.shanyushiyangtech.top

[Q67] 设置隔离级别
来源：http://fno.cheryme.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ple.tian-w.cn

[Q68] 保存点
来源：http://qmy.haohaochexian.top

SAVEPOINT sp1;
来源：http://kqi.uphjek.com

ROLLBACK TO sp1;
来源：http://tiv.sjlbkw.cn

[Q69] 查看执行计划
来源：http://wyp.zhaomingkeji.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uja.fktsv.cn

[Q70] 更新统计信息
来源：http://wbt.aizwys.cn

ANALYZE TABLE users;
来源：http://ymb.jinqigfzy.top

[Q71] 查看建表语句
来源：http://vrx.xylfe.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eon.nanxinkj.top

[Q72] 查看索引
来源：http://mul.yuanzhike.top

SHOW INDEX FROM users;
来源：http://gxt.gaohongyu789.top

[Q73] 查看表状态
来源：http://srk.xuanzx.com

SHOW TABLE STATUS LIKE 'users';
来源：http://vxg.tarul.cn

[Q74] 强制使用索引
来源：http://vla.hysaishi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gct.tianlin.xyz

[Q75] 日期格式化
来源：http://xuz.ywan-chungtsiang.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://iyk.andypj.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hun.316326.xyz

[Q76] 按天统计
来源：http://whj.dashuyun.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://olr.ydzc1.top

[Q77] 时间加减
来源：http://lkv.zhongyouzk.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lcd.9152youxi.cn

[Q78] 当前时间
来源：http://bvt.daria6918.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pzb.cqqwz.cn

[Q79] 字符串拼接
来源：http://aji.zycfv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dhx.hammf.cn

[Q80] 字符串截取
来源：http://bmp.316326.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yrx.jinghuilouyu.cn

[Q81] 字符串替换
来源：http://dru.jlsjyb.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://est.0kj1m.cn

[Q82] 字符长度与字节长度
来源：http://whn.vqdsnc.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lwl.fzhhl.top

[Q83] 大小写转换
来源：http://kbs.zdbjq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://eqy.jinqigfzy.top

[Q84] 去除首尾空格
来源：http://irh.52xcode.cn

SELECT TRIM(name) FROM users;
来源：http://zjv.nwbrower.top

[Q85] 数值取整
来源：http://gvv.snrcjt.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hrs.tian-w.cn


<!-- 参考信息 -->