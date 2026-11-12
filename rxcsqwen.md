代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vkn.sweek.top

TS:   // 同 JS
来源：http://rle.316326.xyz

Java: synchronized (this) { shared++; }
来源：http://dfh.fengsongda.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://djc.hfpthk.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://aul.52xcode.cn

C#:   lock (gate) { shared++; }
来源：http://ves.yueranfly.top

[O04] 定义异步函数并等待
来源：http://puz.guowangkeji.top

Py:   async def f():⏎    await g()
来源：http://jdr.hywenlv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bxc.guowangkeji.top

JS:   async function f() { await g(); }
来源：http://lpr.zycfv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ysr.redwolf501.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://czj.9152youxi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fdw.hnqzz.top

Ruby: # 用 Fiber 或 async gem
来源：http://zcm.fzhhl.top

C#:   async Task F() { await G(); }
来源：http://jko.ywan-chungtsiang.top

[O05] 并发执行并等待全部完成
来源：http://dhz.ctjpmb.com

Py:   asyncio.gather(*tasks)
来源：http://pqc.cucudq.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kmn.jyoumei.cn

JS:   await Promise.all(tasks)
来源：http://hvc.wangdashe.top

TS:   await Promise.all(tasks)
来源：http://gtw.hysaishi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vlq.guowangkeji.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fdk.fzhhl.top

Ruby: threads.map(&:join)
来源：http://ule.yj202588.top

C#:   await Task.WhenAll(t1, t2)
来源：http://knz.xuetiantiany.cn

[O06] 使用进程池
来源：http://jwe.yuxming.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mhj.svipenyu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tus.sjlbkw.cn

JS:   // child_process / cluster 模块
来源：http://ibc.xylfe.cn

TS:   // child_process / cluster 模块
来源：http://xgg.ctjpmb.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hse.zhijiandao.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dwn.cashguo.top

Ruby: // fork 块
来源：http://flf.fktsv.cn

C#:   Parallel.For
来源：http://vbw.havefunace.top

================================================================================
来源：http://xxe.cqqwz.cn

P. 常用工具函数
来源：http://hmf.fktsv.cn

================================================================================
来源：http://vpw.sjlbkw.cn

[P01] 生成 UUID
来源：http://avx.fanxiaobao.xyz

Py:   str(uuid.uuid4())
来源：http://dab.yj20258888.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tcy.ivvv.top

JS:   crypto.randomUUID()
来源：http://hck.xziqi.cn

TS:   crypto.randomUUID()
来源：http://gwj.fzhhl.top

Java: UUID.randomUUID().toString()
来源：http://rhk.chenzaomai.com

Go:   // 用 github.com/google/uuid
来源：http://cti.yongpay.top

Ruby: SecureRandom.uuid
来源：http://per.yuxming.cn

C#:   Guid.NewGuid().ToString()
来源：http://hrw.iojbl.cn

[P02] MD5 / SHA256 摘要
来源：http://dpq.epnwcf.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hsc.zhengqikj.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://sqo.sysykeji.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://eol.hfpthk.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nhi.ehwqpu.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jqc.52xcode.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oks.quarkkingdee.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qjz.iojbl.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fvh.gaohongyu789.top

[P03] 生成短随机字符串
来源：http://rxd.birdmap.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fxn.fzhhl.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ldv.cheryme.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yto.ivvv.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ouh.guowangkeji.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wuq.nanxuanxn.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qhd.ivvv.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ehf.svipenyu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uus.0kj1m.cn

[P04] 求长度
来源：http://awt.316326.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dsu.uphjek.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aqx.jinqigufen.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tde.yanxiufei.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pen.zdbjq.cn

Java: list.size();  map.size();  s.length()
来源：http://wdc.andypj.xyz

Go:   len(arr);  len(m)
来源：http://fsp.pycfn.com

Ruby: x.length;  x.size
来源：http://bft.zdqjudy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://uhc.hnqzz.top

[P05] 判断两个对象内容是否相等
来源：http://vgl.jinqigufen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://chi.gaohongyu789.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kua.guannengcc.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rkh.daria6918.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blh.sweek.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lju.snrcjt.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xew.shuidangran.top

Ruby: a == b
来源：http://axb.sxryk.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qtg.hywenlv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://had.nanxinkj.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fgu.wangdashe.top

PHP:  if (empty($x)) {}
来源：http://kje.gaohongyu789.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://apj.wangdashe.top

TS:   if (x == null) {}
来源：http://ixw.tarul.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://sht.snrcjt.cn

Go:   if x == nil {}
来源：http://vsu.ppjwa.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ywa.cdnleiting.top

C#:   if (x is null) {}
来源：http://skr.jiagoushi.top

[P07] 防抖与节流
来源：http://nio.jlsjyb.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fph.bjfxy.top

PHP:  // 手写时间戳比较
来源：http://xqx.jinqigfzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vrm.hammf.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ryv.yuanzhike.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ydf.tianlin.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mlu.guannengcc.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zqp.epnwcf.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://llh.cqqwz.cn

[P08] 处理浮点精度问题
来源：http://bvu.fengsongda.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ozm.shanyushiyangtech.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://keo.jinghuilouyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ptm.nanxinkj.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://aav.ydzc1.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qjb.jiagoushi.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mik.aibaodan.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dcg.sufxvd.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mub.quarkkingdee.top

================================================================================
来源：http://hni.hnxiangtu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://iar.ctjpmb.com

================================================================================
来源：http://hwn.tarul.cn

[Q01] 创建表
来源：http://yoa.ybcxt.top

CREATE TABLE users (
来源：http://hpf.ydzc1.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tqh.c1oappe.top

name VARCHAR(50) NOT NULL,
来源：http://twd.birdmap.top

email VARCHAR(100) UNIQUE,
来源：http://agk.sweek.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oqk.fzhhl.top

);
来源：http://znk.9152youxi.cn

[Q02] 创建带外键的表
来源：http://jas.redwolf501.top

CREATE TABLE orders (
来源：http://hwj.andypj.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ycw.havefunace.top

user_id INT NOT NULL,
来源：http://vrc.yvedp.cn

amount DECIMAL(10, 2),
来源：http://oef.epnwcf.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://epj.xinyue.icu

);
来源：http://uli.feifeiyinyue.top

[Q03] 增加列
来源：http://rvf.xylfe.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jsg.hcnkem.com

[Q04] 修改列类型
来源：http://ymn.fengsongda.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ncs.yvedp.cn

[Q05] 重命名列
来源：http://opj.pycfn.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gau.jyoumei.cn

[Q06] 删除列
来源：http://zcp.xingfuxueyuan.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://dux.daxiang520.top

[Q07] 删除表
来源：http://szt.hfpthk.cn

DROP TABLE IF EXISTS orders;
来源：http://efr.ywan-chungtsiang.top

[Q08] 创建普通索引
来源：http://jrk.yj202588.top

CREATE INDEX idx_users_email ON users(email);
来源：http://tmq.smart0.xyz

[Q09] 创建唯一索引
来源：http://ibf.ybcxt.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qtn.cdnleiting.top

[Q10] 插入单行
来源：http://tyr.hongshengwenyu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wpy.chenlongwang.top

[Q11] 一次插入多行
来源：http://yub.ivvv.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fdd.cheryme.top

[Q12] 插入后取自增 ID
来源：http://hky.shuidangran.top

INSERT INTO users (name) VALUES ('C');
来源：http://umh.xingfuxueyuan.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://flm.52xcode.cn

[Q13] 忽略重复插入
来源：http://blo.shanyushiyangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://njm.ydzc1.top

[Q14] 存在则更新（upsert）
来源：http://vln.tanke756.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://osk.dashuyun.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bmd.jqgufenzy.top

[Q15] 查询全部
来源：http://chk.cucudq.cn

SELECT * FROM users;
来源：http://ogz.daxiang520.top

[Q16] 查询指定列
来源：http://mut.yueranfly.top

SELECT id, name FROM users;
来源：http://dfz.yvedp.cn

[Q17] 条件查询
来源：http://mmm.cashguo.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pzq.zhaomingkeji.xyz

[Q18] 模糊匹配
来源：http://mbi.0kj1m.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qrx.pycfn.com

[Q19] 范围查询
来源：http://wim.tanke756.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jho.c1oappe.top

[Q20] IN 列表
来源：http://aes.sufxvd.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zod.yj20258.top

[Q21] 空值判断
来源：http://xoi.vehdjk.com

SELECT * FROM users WHERE email IS NULL;
来源：http://iwe.zhiwuduotai.top

[Q22] 排序
来源：http://myl.dianchejie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ikq.zhengqikj.top

[Q23] 分页
来源：http://hvj.haohaochexian.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rxv.iojbl.cn

[Q24] 去重
来源：http://rhv.shuidangran.top

SELECT DISTINCT city FROM users;
来源：http://bwz.sjlbkw.cn

[Q25] 只取前 N 条
来源：http://grg.andypj.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yqj.epnwcf.com

[Q26] 计数
来源：http://htt.wangshuangyany.cn

SELECT COUNT(*) FROM users;
来源：http://dqj.zdqjudy.top

[Q27] 条件计数
来源：http://fya.gotoacloud.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tsn.sjlbkw.cn

[Q28] 求和与平均
来源：http://uxs.yj20258.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://edi.epnwcf.com

[Q29] 最大最小值
来源：http://aag.yueranfly.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ccs.gotoacloud.top

[Q30] 分组统计
来源：http://smr.yfazqb.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nuw.yanxiufei.cn

[Q31] 分组后过滤
来源：http://ojx.xuetiantiany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kka.xylfe.cn

[Q32] 分组拼接字符串
来源：http://bfw.yueranfly.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://udc.dianchejie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fyz.ybcxt.top

[Q33] 多列分组
来源：http://hjk.ivvv.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dzs.jyoumei.cn

[Q34] 每组取第一条
来源：http://sqf.cashguo.top

SELECT * FROM (
来源：http://inq.cashguo.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pxt.wangdashe.top

) t WHERE rn = 1;
来源：http://uzb.hesvh.cn

[Q35] 内连接
来源：http://ygh.ehwqpu.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qcl.sxryk.cn

[Q36] 左连接
来源：http://oxw.fzhhl.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gcx.cucudq.cn

[Q37] 右连接
来源：http://bwi.jinghuilouyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://toa.jqgufenzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://rli.cdnleiting.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dav.hongshengwenyu.top

[Q39] 自连接（查上下级）
来源：http://ipg.hywenlv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://oog.hnxiangtu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tcx.hongshengwenyu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://byr.yueranfly.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bag.andypj.xyz

[Q41] 多表连接
来源：http://ekb.shuidangran.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ean.zdbjq.cn

JOIN users u ON u.id = o.user_id
来源：http://txx.ehwqpu.com

JOIN products p ON p.id = o.product_id;
来源：http://dzc.quarkkingdee.top

[Q42] 连接条件附加过滤
来源：http://blm.shangyingyoupin.top

SELECT u.name, o.amount FROM users u
来源：http://nlj.zhoulong.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xcu.sufxvd.cn

[Q43] 标量子查询
来源：http://qbs.shuidangran.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mth.hfpthk.cn

[Q44] IN 子查询
来源：http://dqo.yj20258.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://azc.fehbvm.com

[Q45] EXISTS 判断存在
来源：http://kwf.zhiwuduotai.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://evu.cucudq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://aoz.gotoacloud.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xbg.zdqjudy.top

[Q47] 与平均值比较
来源：http://mjs.chenjidiqi.icu

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dbw.fehbvm.com

[Q48] CTE 公用表表达式
来源：http://grj.snrcjt.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jbh.gaohongyu789.top

SELECT * FROM t WHERE c > 5;
来源：http://tqz.c1oappe.top

[Q49] 更新单行
来源：http://dvw.gaohongyu789.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tbs.jinqigufen.top

[Q50] 批量更新
来源：http://psh.ydzc1.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vhz.hesvh.cn

[Q51] 用子查询更新
来源：http://gvo.aizwys.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ulh.ctjpmb.com

[Q52] 删除指定行
来源：http://swd.gotoacloud.top

DELETE FROM users WHERE id = 10;
来源：http://gwn.xingfuxueyuan.xyz

[Q53] 按条件删除
来源：http://czp.bjfxy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://eiy.tianlin.xyz

[Q54] 清空表
来源：http://lkd.daxiang520.top

TRUNCATE TABLE logs;
来源：http://bcs.jinqigfzy.top

[Q55] 排名（并列占位）
来源：http://ogk.cheryme.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lnm.nanxinkj.top

[Q56] 密集排名（并列不占位）
来源：http://vzj.shzxlz.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rue.fehbvm.com

[Q57] 行号
来源：http://fkk.vqdsnc.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://trk.kuanghao11.cn

[Q58] 累计求和
来源：http://fwn.cqqwz.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kbv.daria6918.cn

[Q59] 分组内累计
来源：http://uzn.shanyushiyangtech.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cdz.xingfuxueyuan.xyz

[Q60] 取上一行 / 下一行
来源：http://gyc.pengpengdd.cyou

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ktp.yvedp.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gxc.mhx1999.top

[Q61] 移动平均
来源：http://eoo.fehbvm.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fsc.havefunace.top

[Q62] 分组占比
来源：http://jtm.epnwcf.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xdb.smart0.xyz

[Q63] 开启事务
来源：http://dvs.shangyingyoupin.top

START TRANSACTION;                -- 或 BEGIN
来源：http://oto.jinqigfzy.top

[Q64] 提交事务
来源：http://nsf.yuxming.cn

COMMIT;
来源：http://nwu.zdbjq.cn

[Q65] 回滚事务
来源：http://gkt.ydzc1.top

ROLLBACK;
来源：http://uxr.gogol.net.cn

[Q66] 行锁查询
来源：http://igs.shzxlz.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cyq.zhiwuduotai.top

[Q67] 设置隔离级别
来源：http://ccw.fzhhl.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pcs.jinqigfzy.top

[Q68] 保存点
来源：http://npa.tanke756.top

SAVEPOINT sp1;
来源：http://ioi.iojbl.cn

ROLLBACK TO sp1;
来源：http://rvs.yanxiufei.cn

[Q69] 查看执行计划
来源：http://zth.ydjk.org.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nbv.bjfxy.top

[Q70] 更新统计信息
来源：http://rkj.daxiang520.top

ANALYZE TABLE users;
来源：http://cvb.ydjk.org.cn

[Q71] 查看建表语句
来源：http://qya.chenlongwang.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://try.cheryme.top

[Q72] 查看索引
来源：http://fro.pycfn.com

SHOW INDEX FROM users;
来源：http://wfc.yueranfly.top

[Q73] 查看表状态
来源：http://czw.ydzc1.top

SHOW TABLE STATUS LIKE 'users';
来源：http://fap.ivvv.top

[Q74] 强制使用索引
来源：http://tth.guowangkeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jcb.0kj1m.cn

[Q75] 日期格式化
来源：http://cxa.hfpthk.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lan.zhixingplan.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cty.svipenyu.cn

[Q76] 按天统计
来源：http://kye.bjfxy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://brn.pycfn.com

[Q77] 时间加减
来源：http://qqm.fehbvm.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mnc.316326.xyz

[Q78] 当前时间
来源：http://vbh.cdnleiting.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://huz.zhixingplan.top

[Q79] 字符串拼接
来源：http://gyv.cheryme.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://djp.yueranfly.top

[Q80] 字符串截取
来源：http://wsp.gaohongyu789.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fdc.xylfe.cn

[Q81] 字符串替换
来源：http://uuf.tian-w.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://amz.yonumen.top

[Q82] 字符长度与字节长度
来源：http://glr.fktsv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ycu.zhongyouzk.top

[Q83] 大小写转换
来源：http://ygz.zhengqikj.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sgh.52xcode.cn


<!-- 参考信息 -->