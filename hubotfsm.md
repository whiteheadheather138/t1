代发 wailian999

[O02] 使用线程池
来源：http://ien.yangfankeji.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://saq.xingfuxueyuan.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pyv.cdnleiting.top

JS:   // worker_threads 线程池
来源：http://iap.52xcode.cn

TS:   // worker_threads 线程池
来源：http://xoc.zdbjq.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wnv.chenzaomai.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wje.xylfe.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nek.zhoulong.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gnp.shanyushiyangtech.top

[O03] 加锁保护共享数据
来源：http://pvo.mhx1999.top

Py:   with lock: shared += 1
来源：http://thf.hysaishi.cn

PHP:  // 用 flock() 做文件锁
来源：http://tvb.jinghuilouyu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yyr.tanke756.top

TS:   // 同 JS
来源：http://kbj.birdmap.top

Java: synchronized (this) { shared++; }
来源：http://dnm.jinyuanbaomall.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iww.yvedp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pji.jlsjyb.cn

C#:   lock (gate) { shared++; }
来源：http://oha.bbcook.cn

[O04] 定义异步函数并等待
来源：http://rjh.zhiwuduotai.top

Py:   async def f():⏎    await g()
来源：http://ivt.hfpthk.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xxu.fengsongda.top

JS:   async function f() { await g(); }
来源：http://rjg.zhongyouzk.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://pev.sweek.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cwy.gzhubu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uaw.fengsongda.top

Ruby: # 用 Fiber 或 async gem
来源：http://huu.sysykeji.top

C#:   async Task F() { await G(); }
来源：http://kip.shzxlz.cn

[O05] 并发执行并等待全部完成
来源：http://qzd.havefunace.top

Py:   asyncio.gather(*tasks)
来源：http://zpl.xuanzx.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tpu.guannengcc.top

JS:   await Promise.all(tasks)
来源：http://qbu.0kj1m.cn

TS:   await Promise.all(tasks)
来源：http://akh.wangdashe.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://aps.daxiang520.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://esu.mhx1999.top

Ruby: threads.map(&:join)
来源：http://kkm.sjlbkw.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ytl.zhijiandao.cn

[O06] 使用进程池
来源：http://mpn.guannengcc.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://djh.wangdashe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://bof.cdnleiting.top

JS:   // child_process / cluster 模块
来源：http://kny.xuanzx.com

TS:   // child_process / cluster 模块
来源：http://cvd.9152youxi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ugt.sjlbkw.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kfz.fehbvm.com

Ruby: // fork 块
来源：http://bca.52xcode.cn

C#:   Parallel.For
来源：http://lmf.yongpay.top

================================================================================
来源：http://vja.ppjwa.cn

P. 常用工具函数
来源：http://uhb.wangdashe.top

================================================================================
来源：http://mcx.mhx1999.top

[P01] 生成 UUID
来源：http://ygl.ctjpmb.com

Py:   str(uuid.uuid4())
来源：http://rgf.yj20258.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wxs.aibaodan.cn

JS:   crypto.randomUUID()
来源：http://mck.dashuyun.cn

TS:   crypto.randomUUID()
来源：http://uqu.sweek.top

Java: UUID.randomUUID().toString()
来源：http://efn.havefunace.top

Go:   // 用 github.com/google/uuid
来源：http://eak.shangyingyoupin.top

Ruby: SecureRandom.uuid
来源：http://nxf.meibo888.top

C#:   Guid.NewGuid().ToString()
来源：http://scg.hfpthk.cn

[P02] MD5 / SHA256 摘要
来源：http://nks.jianghu66.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://skw.epnwcf.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://zrd.sufxvd.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dbz.yueranfly.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ovl.haohaochexian.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xkf.zhaomingkeji.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://umd.havefunace.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://aeo.yfazqb.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://flh.nanxuanxn.top

[P03] 生成短随机字符串
来源：http://elq.hfpthk.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gsz.vqdsnc.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bfx.wangshuangyany.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zdk.mhx1999.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lvf.jlsjyb.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wus.havefunace.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zuq.ctjpmb.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://shi.shanyushiyangtech.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://msd.zdbjq.cn

[P04] 求长度
来源：http://fuo.hnxiangtu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xfm.jlsjyb.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qic.havefunace.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ral.fktsv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mky.hongshengwenyu.top

Java: list.size();  map.size();  s.length()
来源：http://rbv.jinghuilouyu.cn

Go:   len(arr);  len(m)
来源：http://bpv.smart0.xyz

Ruby: x.length;  x.size
来源：http://mnm.c1oappe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://hcx.zhongyouzk.top

[P05] 判断两个对象内容是否相等
来源：http://hxb.zhaomingkeji.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://kyg.zdqjudy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dvy.shzxlz.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cpg.fanxiaobao.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tvg.shzxlz.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://slc.dashuyun.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qbi.ehwqpu.com

Ruby: a == b
来源：http://nnh.shzxlz.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zil.zdbjq.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nhm.yj202588.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://aiw.ctjpmb.com

PHP:  if (empty($x)) {}
来源：http://qqg.9152youxi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vpf.yfazqb.com

TS:   if (x == null) {}
来源：http://ryu.sufxvd.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wol.xinyue.icu

Go:   if x == nil {}
来源：http://cjx.sweek.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://int.hywenlv.cn

C#:   if (x is null) {}
来源：http://lil.feifeiyinyue.top

[P07] 防抖与节流
来源：http://xro.gogol.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mes.xuanzx.com

PHP:  // 手写时间戳比较
来源：http://dqw.zhongyouzk.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://idp.tian-w.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sbk.redwolf501.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://luq.jyoumei.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xvc.chenzaomai.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://hqr.jinghuilouyu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tyn.smart0.xyz

[P08] 处理浮点精度问题
来源：http://ugh.smart0.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kki.ybcxt.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dns.ydzc1.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://scz.jinqigfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rqa.tanke756.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pge.hesvh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ldj.ydzc1.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jkz.yj202588.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lyp.chenjidiqi.icu

================================================================================
来源：http://oeg.mhx1999.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://eju.sweek.top

================================================================================
来源：http://dke.jinyuanbaomall.cn

[Q01] 创建表
来源：http://mzl.jqgufenzy.top

CREATE TABLE users (
来源：http://rea.cdnleiting.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lpa.epnwcf.com

name VARCHAR(50) NOT NULL,
来源：http://djm.wangshuangyany.cn

email VARCHAR(100) UNIQUE,
来源：http://pjq.zhoulong.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ujq.hnqzz.top

);
来源：http://dyp.daxiang520.top

[Q02] 创建带外键的表
来源：http://hvr.sweek.top

CREATE TABLE orders (
来源：http://soq.sysykeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://aoo.iojbl.cn

user_id INT NOT NULL,
来源：http://jct.yanxiufei.cn

amount DECIMAL(10, 2),
来源：http://mhe.ywan-chungtsiang.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bpe.yj20258888.top

);
来源：http://ebd.yj202588.top

[Q03] 增加列
来源：http://yti.zhoulong.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mim.kuanghao11.cn

[Q04] 修改列类型
来源：http://grt.shuidangran.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tnv.ydzc1.top

[Q05] 重命名列
来源：http://sqm.xuanzx.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fqm.zhengqikj.top

[Q06] 删除列
来源：http://pqb.epnwcf.com

ALTER TABLE users DROP COLUMN age;
来源：http://oua.tanke756.top

[Q07] 删除表
来源：http://hog.ivvv.top

DROP TABLE IF EXISTS orders;
来源：http://cpj.xuetiantiany.cn

[Q08] 创建普通索引
来源：http://lwi.ywan-chungtsiang.top

CREATE INDEX idx_users_email ON users(email);
来源：http://hft.hysaishi.cn

[Q09] 创建唯一索引
来源：http://bpo.kuanghao11.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qip.ehwqpu.com

[Q10] 插入单行
来源：http://nro.nanxuanxn.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bhv.cucudq.cn

[Q11] 一次插入多行
来源：http://veu.sxryk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tfz.ctjpmb.com

[Q12] 插入后取自增 ID
来源：http://ncs.sjlbkw.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yvk.jianghu66.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yfo.yueranfly.top

[Q13] 忽略重复插入
来源：http://jtu.tanke756.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tfd.kuanghao11.cn

[Q14] 存在则更新（upsert）
来源：http://tro.jqgfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tzc.jinyuanbaomall.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rfk.cqqwz.cn

[Q15] 查询全部
来源：http://xod.zycfv.cn

SELECT * FROM users;
来源：http://xkt.chenlongwang.top

[Q16] 查询指定列
来源：http://lve.sufxvd.cn

SELECT id, name FROM users;
来源：http://gqc.shanyushiyangkeji.top

[Q17] 条件查询
来源：http://gsd.xinyue.icu

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nvt.jianghu66.top

[Q18] 模糊匹配
来源：http://xod.pycfn.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jll.hnqzz.top

[Q19] 范围查询
来源：http://kde.hysaishi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qni.fehbvm.com

[Q20] IN 列表
来源：http://weu.316326.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://azd.vehdjk.com

[Q21] 空值判断
来源：http://ttz.wangdashe.top

SELECT * FROM users WHERE email IS NULL;
来源：http://wij.shuidangran.top

[Q22] 排序
来源：http://ias.sysykeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rex.ivvv.top

[Q23] 分页
来源：http://caw.pengpengdd.cyou

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bib.bbcook.cn

[Q24] 去重
来源：http://emh.ivvv.top

SELECT DISTINCT city FROM users;
来源：http://aez.feifeiyinyue.top

[Q25] 只取前 N 条
来源：http://ust.jianghu66.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jwf.iojbl.cn

[Q26] 计数
来源：http://jbt.guowangkeji.top

SELECT COUNT(*) FROM users;
来源：http://xac.ehwqpu.com

[Q27] 条件计数
来源：http://ada.cashguo.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dma.316326.xyz

[Q28] 求和与平均
来源：http://twi.jinyuanbaomall.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://drc.guowangkeji.top

[Q29] 最大最小值
来源：http://zzr.0kj1m.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gto.zhoulong.xyz

[Q30] 分组统计
来源：http://ypc.yj20258.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pqj.yj20258888.top

[Q31] 分组后过滤
来源：http://aja.yongpay.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fqi.guannengcc.top

[Q32] 分组拼接字符串
来源：http://kzr.meibo888.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gwm.ydzc1.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ayu.hongshengwenyu.top

[Q33] 多列分组
来源：http://mau.andypj.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xyl.xuanzx.com

[Q34] 每组取第一条
来源：http://ide.sxryk.cn

SELECT * FROM (
来源：http://fho.nanxuanxn.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yll.jyoumei.cn

) t WHERE rn = 1;
来源：http://fbz.birdmap.top

[Q35] 内连接
来源：http://kkj.jinqigufen.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vqu.52xcode.cn

[Q36] 左连接
来源：http://lis.shanyushiyangkeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://apm.sweek.top

[Q37] 右连接
来源：http://kdl.xinyue.icu

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mdf.xingfuxueyuan.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://raj.tarul.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ukl.yongpay.top

[Q39] 自连接（查上下级）
来源：http://mfu.gogol.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ixs.gaohongyu789.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gwi.daxiang520.top

[Q40] 交叉连接（笛卡尔积）
来源：http://gxf.fanxiaobao.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pco.fktsv.cn

[Q41] 多表连接
来源：http://czc.fengsongda.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://jjz.zhongyouzk.top

JOIN users u ON u.id = o.user_id
来源：http://wlh.fktsv.cn

JOIN products p ON p.id = o.product_id;
来源：http://vpp.ywan-chungtsiang.top

[Q42] 连接条件附加过滤
来源：http://fro.nanxuanxn.top

SELECT u.name, o.amount FROM users u
来源：http://wld.birdmap.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zvy.yj202588.top

[Q43] 标量子查询
来源：http://vqa.hesvh.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wda.shanyushiyangkeji.top

[Q44] IN 子查询
来源：http://pyr.feifeiyinyue.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cmc.fanxiaobao.xyz

[Q45] EXISTS 判断存在
来源：http://orj.aibaodan.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mjk.yonumen.top

[Q46] NOT EXISTS 判断不存在
来源：http://qbc.hfpthk.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://con.zhiwuduotai.top

[Q47] 与平均值比较
来源：http://ber.daxiang520.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hba.jqgfzy.top

[Q48] CTE 公用表表达式
来源：http://nae.jinghuilouyu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://brz.yueranfly.top

SELECT * FROM t WHERE c > 5;
来源：http://hhe.ybcxt.top

[Q49] 更新单行
来源：http://tlm.c1oappe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xow.gaohongyu789.top

[Q50] 批量更新
来源：http://czp.cqqwz.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hzg.daria6918.cn

[Q51] 用子查询更新
来源：http://jmr.zhixingplan.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iah.hcnkem.com

[Q52] 删除指定行
来源：http://yow.fehbvm.com

DELETE FROM users WHERE id = 10;
来源：http://xsn.yvedp.cn

[Q53] 按条件删除
来源：http://eds.hammf.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zox.pengpengdd.cyou

[Q54] 清空表
来源：http://znk.yfazqb.com

TRUNCATE TABLE logs;
来源：http://agm.birdmap.top

[Q55] 排名（并列占位）
来源：http://qgh.yanxiufei.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dcq.mhx1999.top

[Q56] 密集排名（并列不占位）
来源：http://qva.hfpthk.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://meq.yangfankeji.com

[Q57] 行号
来源：http://yaa.andypj.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://utm.sjlbkw.cn

[Q58] 累计求和
来源：http://twd.tian-w.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tre.ivvv.top

[Q59] 分组内累计
来源：http://wtx.bbcook.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://llc.hfpthk.cn

[Q60] 取上一行 / 下一行
来源：http://xmh.smart0.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://iif.cashguo.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vlc.yj202588.top

[Q61] 移动平均
来源：http://tvt.epnwcf.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lpr.vqdsnc.cn

[Q62] 分组占比
来源：http://bli.hysaishi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://acc.jinghuilouyu.cn

[Q63] 开启事务
来源：http://xej.fanxiaobao.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://xjr.redwolf501.top

[Q64] 提交事务
来源：http://nst.ybcxt.top

COMMIT;
来源：http://bzv.snrcjt.cn

[Q65] 回滚事务
来源：http://yre.shanyushiyangtech.top

ROLLBACK;
来源：http://ufs.shanyushiyangkeji.top

[Q66] 行锁查询
来源：http://pkj.zhaomingkeji.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://iyb.hesvh.cn

[Q67] 设置隔离级别
来源：http://kot.xuanzx.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nkl.ctjpmb.com

[Q68] 保存点
来源：http://fpe.hcnkem.com

SAVEPOINT sp1;
来源：http://uyd.iojbl.cn

ROLLBACK TO sp1;
来源：http://tso.ppjwa.cn

[Q69] 查看执行计划
来源：http://mer.pycfn.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lja.vqdsnc.cn

[Q70] 更新统计信息
来源：http://lpb.hfpthk.cn

ANALYZE TABLE users;
来源：http://kbb.c1oappe.top

[Q71] 查看建表语句
来源：http://rxl.daria6918.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bjb.pycfn.com

[Q72] 查看索引
来源：http://ffu.cqqwz.cn

SHOW INDEX FROM users;
来源：http://ztc.jyoumei.cn

[Q73] 查看表状态
来源：http://gwq.jqgufenzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ptv.hnxiangtu.top

[Q74] 强制使用索引
来源：http://czc.uphjek.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ixi.zdqjudy.top

[Q75] 日期格式化
来源：http://iwd.andypj.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ezt.dianchejie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://avm.jinqigfzy.top

[Q76] 按天统计
来源：http://gdn.gotoacloud.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://led.sjlbkw.cn

[Q77] 时间加减
来源：http://wyi.ppjwa.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fru.havefunace.top


<!-- 参考信息 -->