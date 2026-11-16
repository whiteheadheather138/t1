代发 wailian999

TS:   // worker_threads 线程池
来源：http://ovc.cdnleiting.top

Java: Executors.newFixedThreadPool(4)
来源：http://hxh.xylfe.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://joj.yanxiufei.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ywz.jinyuanbaomall.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cmg.316326.xyz

[O03] 加锁保护共享数据
来源：http://ydq.tian-w.cn

Py:   with lock: shared += 1
来源：http://xzt.hywenlv.cn

PHP:  // 用 flock() 做文件锁
来源：http://sat.shanyushiyangtech.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ruj.xingfuxueyuan.xyz

TS:   // 同 JS
来源：http://qol.wangdashe.top

Java: synchronized (this) { shared++; }
来源：http://sss.meibo888.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ukm.hfpthk.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pgh.zhixingplan.top

C#:   lock (gate) { shared++; }
来源：http://dzl.yj20258.top

[O04] 定义异步函数并等待
来源：http://kbe.chenjidiqi.icu

Py:   async def f():⏎    await g()
来源：http://jtn.yj202588.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vpu.gogol.net.cn

JS:   async function f() { await g(); }
来源：http://imu.cdnleiting.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://gtk.gogol.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dlt.nanxinkj.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yuo.mhx1999.top

Ruby: # 用 Fiber 或 async gem
来源：http://cmv.yvedp.cn

C#:   async Task F() { await G(); }
来源：http://yxe.yfazqb.com

[O05] 并发执行并等待全部完成
来源：http://nxb.mhx1999.top

Py:   asyncio.gather(*tasks)
来源：http://plv.tianlin.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://opt.sjlbkw.cn

JS:   await Promise.all(tasks)
来源：http://com.9152youxi.cn

TS:   await Promise.all(tasks)
来源：http://hpq.iojbl.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pkx.vehdjk.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hwz.snrcjt.cn

Ruby: threads.map(&:join)
来源：http://tvq.ydjk.org.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://voe.shanyushiyangkeji.top

[O06] 使用进程池
来源：http://ymc.shuidangran.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vfj.wangshuangyany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vxg.kuanghao11.cn

JS:   // child_process / cluster 模块
来源：http://xtn.jinqigfzy.top

TS:   // child_process / cluster 模块
来源：http://kgi.fanxiaobao.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://amc.bjfxy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rqh.sxryk.cn

Ruby: // fork 块
来源：http://pmv.birdmap.top

C#:   Parallel.For
来源：http://xpj.yj20258.top

================================================================================
来源：http://wmv.yangfankeji.com

P. 常用工具函数
来源：http://gdi.sweek.top

================================================================================
来源：http://pdd.zhaomingkeji.xyz

[P01] 生成 UUID
来源：http://fpf.zhaomingkeji.xyz

Py:   str(uuid.uuid4())
来源：http://hmh.fktsv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cqv.shzxlz.cn

JS:   crypto.randomUUID()
来源：http://ozx.gotoacloud.top

TS:   crypto.randomUUID()
来源：http://ykv.zdbjq.cn

Java: UUID.randomUUID().toString()
来源：http://fvj.mhx1999.top

Go:   // 用 github.com/google/uuid
来源：http://kev.zhongyouzk.top

Ruby: SecureRandom.uuid
来源：http://tlv.bjfxy.top

C#:   Guid.NewGuid().ToString()
来源：http://jpw.gzhubu.top

[P02] MD5 / SHA256 摘要
来源：http://mrp.sysykeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ynw.guannengcc.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://flr.tarul.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vik.yanxiufei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://psr.jlsjyb.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ttp.mhx1999.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tmx.hywenlv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://spo.cashguo.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tjf.cashguo.top

[P03] 生成短随机字符串
来源：http://eso.bjfxy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://byy.iojbl.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://goq.yuxming.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oxh.316326.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sqa.shuidangran.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dkc.0kj1m.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hef.fzhhl.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://tsb.xinyue.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://eti.quarkkingdee.top

[P04] 求长度
来源：http://rie.zhixingplan.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fsk.yonumen.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kcw.vehdjk.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://shh.nwbrower.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dqy.uphjek.com

Java: list.size();  map.size();  s.length()
来源：http://eig.jinqigufen.top

Go:   len(arr);  len(m)
来源：http://vkd.jqgfzy.top

Ruby: x.length;  x.size
来源：http://ubs.ppjwa.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://nee.uphjek.com

[P05] 判断两个对象内容是否相等
来源：http://llm.vqdsnc.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://smh.sysykeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nkp.kuanghao11.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://erc.jqgufenzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jgs.haohaochexian.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pqx.ivvv.top

Go:   reflect.DeepEqual(a, b)
来源：http://gqz.bjfxy.top

Ruby: a == b
来源：http://ftd.yfazqb.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cvs.tanke756.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://syf.bbcook.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lks.snrcjt.cn

PHP:  if (empty($x)) {}
来源：http://hcm.andypj.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lqg.jinyuanbaomall.cn

TS:   if (x == null) {}
来源：http://ckv.yfazqb.com

Java: if (x == null || x.isEmpty()) {}
来源：http://bea.gaohongyu789.top

Go:   if x == nil {}
来源：http://vup.chenjidiqi.icu

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jxj.pycfn.com

C#:   if (x is null) {}
来源：http://cbh.havefunace.top

[P07] 防抖与节流
来源：http://lsw.xingfuxueyuan.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://duu.chenjidiqi.icu

PHP:  // 手写时间戳比较
来源：http://yvn.sweek.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tau.zycfv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cmz.yangfankeji.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wkl.hysaishi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yrj.hysaishi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://kgg.vehdjk.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pss.jqgfzy.top

[P08] 处理浮点精度问题
来源：http://fek.kuanghao11.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wyj.daria6918.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://orp.tanke756.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uuj.daxiang520.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tnm.9152youxi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yzw.nwbrower.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lmj.daria6918.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://aib.tarul.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lyq.xingfuxueyuan.xyz

================================================================================
来源：http://oul.meibo888.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://teo.nwbrower.top

================================================================================
来源：http://eww.jlsjyb.cn

[Q01] 创建表
来源：http://fjw.yj20258.top

CREATE TABLE users (
来源：http://cdh.yuanzhike.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://odn.guannengcc.top

name VARCHAR(50) NOT NULL,
来源：http://dbi.bjfxy.top

email VARCHAR(100) UNIQUE,
来源：http://vrl.zhengqikj.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://anm.tian-w.cn

);
来源：http://umq.nanxuanxn.top

[Q02] 创建带外键的表
来源：http://aws.xziqi.cn

CREATE TABLE orders (
来源：http://yuc.sysykeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ycv.yuxming.cn

user_id INT NOT NULL,
来源：http://ony.hesvh.cn

amount DECIMAL(10, 2),
来源：http://veu.bbcook.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ref.hesvh.cn

);
来源：http://rdq.9152youxi.cn

[Q03] 增加列
来源：http://gtq.fehbvm.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://asr.ydzc1.top

[Q04] 修改列类型
来源：http://zjn.gzhubu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://unl.gogol.net.cn

[Q05] 重命名列
来源：http://vjp.yuanzhike.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tmr.yangfankeji.com

[Q06] 删除列
来源：http://dtc.wangshuangyany.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ddw.sweek.top

[Q07] 删除表
来源：http://zil.hcnkem.com

DROP TABLE IF EXISTS orders;
来源：http://smr.hysaishi.cn

[Q08] 创建普通索引
来源：http://vle.yj202588.top

CREATE INDEX idx_users_email ON users(email);
来源：http://sau.yuxming.cn

[Q09] 创建唯一索引
来源：http://oib.xziqi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tcj.fengsongda.top

[Q10] 插入单行
来源：http://tul.jinqigufen.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lgr.nanxuanxn.top

[Q11] 一次插入多行
来源：http://fos.hnqzz.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://goi.fzhhl.top

[Q12] 插入后取自增 ID
来源：http://qtb.0kj1m.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qlr.chenzaomai.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vqs.fengsongda.top

[Q13] 忽略重复插入
来源：http://lsz.cqqwz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fjl.guannengcc.top

[Q14] 存在则更新（upsert）
来源：http://lqb.haohaochexian.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ahu.zhaomingkeji.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xlf.c1oappe.top

[Q15] 查询全部
来源：http://gym.shuidangran.top

SELECT * FROM users;
来源：http://mti.yuxming.cn

[Q16] 查询指定列
来源：http://nva.wangshuangyany.cn

SELECT id, name FROM users;
来源：http://tez.yongpay.top

[Q17] 条件查询
来源：http://tml.cashguo.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uja.zhoulong.xyz

[Q18] 模糊匹配
来源：http://ksl.tian-w.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tgn.jinqigfzy.top

[Q19] 范围查询
来源：http://zmd.nwbrower.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dxu.yongpay.top

[Q20] IN 列表
来源：http://rzq.kuanghao11.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ptj.nwbrower.top

[Q21] 空值判断
来源：http://lmx.52xcode.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gqh.mhx1999.top

[Q22] 排序
来源：http://mhs.yj202588.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xql.sysykeji.top

[Q23] 分页
来源：http://mrc.fanxiaobao.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://klo.ppjwa.cn

[Q24] 去重
来源：http://rll.ivvv.top

SELECT DISTINCT city FROM users;
来源：http://rbv.zhijiandao.cn

[Q25] 只取前 N 条
来源：http://knc.gzhubu.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zlb.uphjek.com

[Q26] 计数
来源：http://sgt.fanxiaobao.xyz

SELECT COUNT(*) FROM users;
来源：http://emn.9152youxi.cn

[Q27] 条件计数
来源：http://lqm.gogol.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wks.ivvv.top

[Q28] 求和与平均
来源：http://imb.hnqzz.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ieb.cqqwz.cn

[Q29] 最大最小值
来源：http://myt.hesvh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://inr.sysykeji.top

[Q30] 分组统计
来源：http://ewq.jinghuilouyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sxd.zhengqikj.top

[Q31] 分组后过滤
来源：http://sdx.daria6918.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://grg.xingfuxueyuan.xyz

[Q32] 分组拼接字符串
来源：http://kdw.zhijiandao.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gmt.sxryk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rje.hammf.cn

[Q33] 多列分组
来源：http://lgb.svipenyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zkm.chenjidiqi.icu

[Q34] 每组取第一条
来源：http://nlv.zhoulong.xyz

SELECT * FROM (
来源：http://piv.gogol.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hfx.ctjpmb.com

) t WHERE rn = 1;
来源：http://bbf.guowangkeji.top

[Q35] 内连接
来源：http://qwo.jinqigufen.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fee.jinqigfzy.top

[Q36] 左连接
来源：http://zlj.cqqwz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://noe.zdqjudy.top

[Q37] 右连接
来源：http://tlj.yonumen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yle.fzhhl.top

[Q38] 全外连接（PostgreSQL）
来源：http://jcc.hysaishi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uaz.jianghu66.top

[Q39] 自连接（查上下级）
来源：http://gjo.jinqigufen.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://uag.jiagoushi.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qml.gaohongyu789.top

[Q40] 交叉连接（笛卡尔积）
来源：http://sou.xinyue.icu

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cvi.xuetiantiany.cn

[Q41] 多表连接
来源：http://lsw.sysykeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://vkv.sweek.top

JOIN users u ON u.id = o.user_id
来源：http://eyu.jiagoushi.top

JOIN products p ON p.id = o.product_id;
来源：http://zwv.zhixingplan.top

[Q42] 连接条件附加过滤
来源：http://acd.vqdsnc.cn

SELECT u.name, o.amount FROM users u
来源：http://jnb.iojbl.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cvd.ybcxt.top

[Q43] 标量子查询
来源：http://cvi.nanxinkj.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fwu.jinqigufen.top

[Q44] IN 子查询
来源：http://kkr.haohaochexian.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vqk.redwolf501.top

[Q45] EXISTS 判断存在
来源：http://emw.daria6918.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yvr.guowangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://muu.hnqzz.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qss.9152youxi.cn

[Q47] 与平均值比较
来源：http://sgk.nanxuanxn.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wpn.aizwys.cn

[Q48] CTE 公用表表达式
来源：http://mrs.pycfn.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://iod.redwolf501.top

SELECT * FROM t WHERE c > 5;
来源：http://don.gogol.net.cn

[Q49] 更新单行
来源：http://fwe.shanyushiyangtech.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hnn.fengsongda.top

[Q50] 批量更新
来源：http://quo.ydjk.org.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://taw.yfazqb.com

[Q51] 用子查询更新
来源：http://zgm.mhx1999.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fbb.zdbjq.cn

[Q52] 删除指定行
来源：http://ykw.nanxuanxn.top

DELETE FROM users WHERE id = 10;
来源：http://qkx.dashuyun.cn

[Q53] 按条件删除
来源：http://jwv.nanxinkj.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://plh.ywan-chungtsiang.top

[Q54] 清空表
来源：http://nri.nanxuanxn.top

TRUNCATE TABLE logs;
来源：http://oam.ctjpmb.com

[Q55] 排名（并列占位）
来源：http://vzc.guannengcc.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ycr.chenlongwang.top

[Q56] 密集排名（并列不占位）
来源：http://odc.guowangkeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://thg.sjlbkw.cn

[Q57] 行号
来源：http://mxc.cucudq.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tmh.fengsongda.top

[Q58] 累计求和
来源：http://nml.ywan-chungtsiang.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cbx.shzxlz.cn

[Q59] 分组内累计
来源：http://fmc.ywan-chungtsiang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nqv.redwolf501.top

[Q60] 取上一行 / 下一行
来源：http://nhg.zhoulong.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pvq.tanke756.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qru.yuxming.cn

[Q61] 移动平均
来源：http://otq.sjlbkw.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qcz.haohaochexian.top

[Q62] 分组占比
来源：http://jhz.svipenyu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rfd.hcnkem.com

[Q63] 开启事务
来源：http://dkl.tian-w.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://plo.fanxiaobao.xyz

[Q64] 提交事务
来源：http://xhq.52xcode.cn

COMMIT;
来源：http://gwp.zhengqikj.top

[Q65] 回滚事务
来源：http://mzd.nanxinkj.top

ROLLBACK;
来源：http://zes.ppjwa.cn

[Q66] 行锁查询
来源：http://xxy.yuxming.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kqy.xziqi.cn

[Q67] 设置隔离级别
来源：http://xcx.chenzaomai.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ebq.jiagoushi.top

[Q68] 保存点
来源：http://ynp.ctjpmb.com

SAVEPOINT sp1;
来源：http://tqs.zhoulong.xyz

ROLLBACK TO sp1;
来源：http://hmc.dashuyun.cn

[Q69] 查看执行计划
来源：http://fmz.quarkkingdee.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fdc.gaohongyu789.top

[Q70] 更新统计信息
来源：http://uvm.meibo888.top

ANALYZE TABLE users;
来源：http://muk.jinqigfzy.top

[Q71] 查看建表语句
来源：http://sar.hnqzz.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gyh.jinqigufen.top

[Q72] 查看索引
来源：http://rid.yj20258.top

SHOW INDEX FROM users;
来源：http://uzi.yj20258.top

[Q73] 查看表状态
来源：http://ljo.hongshengwenyu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://kyg.smart0.xyz

[Q74] 强制使用索引
来源：http://mlz.andypj.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fch.nanxuanxn.top

[Q75] 日期格式化
来源：http://aad.daria6918.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://aay.hywenlv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://omq.hywenlv.cn

[Q76] 按天统计
来源：http://pjf.quarkkingdee.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xon.yj20258888.top

[Q77] 时间加减
来源：http://tkd.gogol.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://egr.zhengqikj.top

[Q78] 当前时间
来源：http://jlx.haohaochexian.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mph.52xcode.cn

[Q79] 字符串拼接
来源：http://rtt.xingfuxueyuan.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lpw.ivvv.top


<!-- 参考信息 -->