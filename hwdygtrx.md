代发 wailian999

[O02] 使用线程池
来源：http://nxf.fzhhl.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ulg.xylfe.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kck.wangdashe.top

JS:   // worker_threads 线程池
来源：http://kpa.hesvh.cn

TS:   // worker_threads 线程池
来源：http://uez.hywenlv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rgl.zhengqikj.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cxf.ppjwa.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://psb.zdbjq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qcy.wangdashe.top

[O03] 加锁保护共享数据
来源：http://iol.vqdsnc.cn

Py:   with lock: shared += 1
来源：http://mby.mhx1999.top

PHP:  // 用 flock() 做文件锁
来源：http://qnf.ydjk.org.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fho.52xcode.cn

TS:   // 同 JS
来源：http://fps.sjlbkw.cn

Java: synchronized (this) { shared++; }
来源：http://qde.birdmap.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mrx.sufxvd.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fjo.guannengcc.top

C#:   lock (gate) { shared++; }
来源：http://bcb.hnxiangtu.top

[O04] 定义异步函数并等待
来源：http://tbg.kuanghao11.cn

Py:   async def f():⏎    await g()
来源：http://glw.shanyushiyangtech.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lic.hysaishi.cn

JS:   async function f() { await g(); }
来源：http://qws.jinghuilouyu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hjv.ywan-chungtsiang.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ztn.tanke756.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bij.shangyingyoupin.top

Ruby: # 用 Fiber 或 async gem
来源：http://kqh.sjlbkw.cn

C#:   async Task F() { await G(); }
来源：http://cmw.jinqigfzy.top

[O05] 并发执行并等待全部完成
来源：http://mhe.gogol.net.cn

Py:   asyncio.gather(*tasks)
来源：http://skg.52xcode.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xcl.zhiwuduotai.top

JS:   await Promise.all(tasks)
来源：http://vzl.0kj1m.cn

TS:   await Promise.all(tasks)
来源：http://clc.xziqi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fah.yj20258888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zgq.meibo888.top

Ruby: threads.map(&:join)
来源：http://xrq.yuanzhike.top

C#:   await Task.WhenAll(t1, t2)
来源：http://kre.shanyushiyangkeji.top

[O06] 使用进程池
来源：http://rmp.yfazqb.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ayh.xuetiantiany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nsq.yvedp.cn

JS:   // child_process / cluster 模块
来源：http://ced.chenlongwang.top

TS:   // child_process / cluster 模块
来源：http://jwl.jqgufenzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xlt.birdmap.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bxn.mhx1999.top

Ruby: // fork 块
来源：http://iav.zhijiandao.cn

C#:   Parallel.For
来源：http://twn.aibaodan.cn

================================================================================
来源：http://puo.quarkkingdee.top

P. 常用工具函数
来源：http://igc.quarkkingdee.top

================================================================================
来源：http://mds.xinyue.icu

[P01] 生成 UUID
来源：http://zqk.yj20258.top

Py:   str(uuid.uuid4())
来源：http://afb.fanxiaobao.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://srh.cheryme.top

JS:   crypto.randomUUID()
来源：http://uvr.jinghuilouyu.cn

TS:   crypto.randomUUID()
来源：http://fln.guowangkeji.top

Java: UUID.randomUUID().toString()
来源：http://vzu.bjfxy.top

Go:   // 用 github.com/google/uuid
来源：http://xpi.jinghuilouyu.cn

Ruby: SecureRandom.uuid
来源：http://nwz.chenjidiqi.icu

C#:   Guid.NewGuid().ToString()
来源：http://kty.xziqi.cn

[P02] MD5 / SHA256 摘要
来源：http://kwv.jiagoushi.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lzr.haohaochexian.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://key.zhengqikj.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cma.aibaodan.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zge.jianghu66.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nwo.redwolf501.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nag.vehdjk.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tuq.fengsongda.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xka.fktsv.cn

[P03] 生成短随机字符串
来源：http://mnh.zhaomingkeji.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wuy.jlsjyb.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bla.0kj1m.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pdz.zhongyouzk.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nek.cqqwz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gam.fanxiaobao.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zev.xingfuxueyuan.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://qps.zhijiandao.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pbw.zdqjudy.top

[P04] 求长度
来源：http://kui.epnwcf.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://unc.haohaochexian.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mit.zycfv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eby.tianlin.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fuo.fktsv.cn

Java: list.size();  map.size();  s.length()
来源：http://moy.andypj.xyz

Go:   len(arr);  len(m)
来源：http://ocy.meibo888.top

Ruby: x.length;  x.size
来源：http://lxv.ywan-chungtsiang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://hjg.jiagoushi.top

[P05] 判断两个对象内容是否相等
来源：http://btu.hongshengwenyu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lec.gogol.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xkh.vqdsnc.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jwd.jinqigufen.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://isj.zhoulong.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xmy.xziqi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fky.ydjk.org.cn

Ruby: a == b
来源：http://vjm.xziqi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xtm.zhongyouzk.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wgm.tian-w.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://swc.aizwys.cn

PHP:  if (empty($x)) {}
来源：http://vlo.gzhubu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xxj.dianchejie.cn

TS:   if (x == null) {}
来源：http://ara.ydjk.org.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nlq.vehdjk.com

Go:   if x == nil {}
来源：http://fqy.vehdjk.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uxm.vehdjk.com

C#:   if (x is null) {}
来源：http://wgf.ivvv.top

[P07] 防抖与节流
来源：http://djd.daxiang520.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nyu.yj20258.top

PHP:  // 手写时间戳比较
来源：http://xmp.zycfv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fmx.jianghu66.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ors.52xcode.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ajf.cucudq.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sii.zhixingplan.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://nnc.jinyuanbaomall.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://otq.xuetiantiany.cn

[P08] 处理浮点精度问题
来源：http://cwl.gzhubu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://abj.cdnleiting.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cmf.iojbl.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bll.chenzaomai.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jti.redwolf501.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://glf.ehwqpu.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://urm.yuxming.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sgi.mhx1999.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ttp.zhongyouzk.top

================================================================================
来源：http://ikg.zhijiandao.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://edk.xuanzx.com

================================================================================
来源：http://dqp.shzxlz.cn

[Q01] 创建表
来源：http://fet.bbcook.cn

CREATE TABLE users (
来源：http://lcm.nwbrower.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mzj.wangshuangyany.cn

name VARCHAR(50) NOT NULL,
来源：http://rgd.chenlongwang.top

email VARCHAR(100) UNIQUE,
来源：http://fya.gogol.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dnj.52xcode.cn

);
来源：http://blr.daxiang520.top

[Q02] 创建带外键的表
来源：http://mpu.kuanghao11.cn

CREATE TABLE orders (
来源：http://gfg.cheryme.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lrx.xingfuxueyuan.xyz

user_id INT NOT NULL,
来源：http://ojg.gotoacloud.top

amount DECIMAL(10, 2),
来源：http://oeq.yueranfly.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zru.yuxming.cn

);
来源：http://quz.fengsongda.top

[Q03] 增加列
来源：http://apr.hammf.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rac.yonumen.top

[Q04] 修改列类型
来源：http://zdm.yongpay.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sir.yuanzhike.top

[Q05] 重命名列
来源：http://cyl.haohaochexian.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ptv.52xcode.cn

[Q06] 删除列
来源：http://prh.shzxlz.cn

ALTER TABLE users DROP COLUMN age;
来源：http://geg.chenzaomai.com

[Q07] 删除表
来源：http://stm.dianchejie.cn

DROP TABLE IF EXISTS orders;
来源：http://kun.tanke756.top

[Q08] 创建普通索引
来源：http://gbp.yonumen.top

CREATE INDEX idx_users_email ON users(email);
来源：http://wma.dianchejie.cn

[Q09] 创建唯一索引
来源：http://zww.yfazqb.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nyn.tanke756.top

[Q10] 插入单行
来源：http://unh.nanxuanxn.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ipb.snrcjt.cn

[Q11] 一次插入多行
来源：http://pag.316326.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mfp.zhixingplan.top

[Q12] 插入后取自增 ID
来源：http://wyn.hfpthk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://kbh.jinyuanbaomall.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://igi.xuetiantiany.cn

[Q13] 忽略重复插入
来源：http://uhy.shuidangran.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kpg.epnwcf.com

[Q14] 存在则更新（upsert）
来源：http://uxm.jqgfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://noj.kuanghao11.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mcu.andypj.xyz

[Q15] 查询全部
来源：http://ahz.snrcjt.cn

SELECT * FROM users;
来源：http://lot.xylfe.cn

[Q16] 查询指定列
来源：http://hir.zycfv.cn

SELECT id, name FROM users;
来源：http://qjq.cashguo.top

[Q17] 条件查询
来源：http://onc.aizwys.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://crn.guowangkeji.top

[Q18] 模糊匹配
来源：http://veo.ybcxt.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fix.fanxiaobao.xyz

[Q19] 范围查询
来源：http://ypl.quarkkingdee.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zmb.shzxlz.cn

[Q20] IN 列表
来源：http://rzp.pycfn.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fsd.ywan-chungtsiang.top

[Q21] 空值判断
来源：http://mey.kuanghao11.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://npi.fehbvm.com

[Q22] 排序
来源：http://dlw.fehbvm.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vvd.zhijiandao.cn

[Q23] 分页
来源：http://mfu.bbcook.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://afm.yj20258888.top

[Q24] 去重
来源：http://kvg.52xcode.cn

SELECT DISTINCT city FROM users;
来源：http://lzs.cqqwz.cn

[Q25] 只取前 N 条
来源：http://ixv.yueranfly.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zox.jinyuanbaomall.cn

[Q26] 计数
来源：http://yfb.fzhhl.top

SELECT COUNT(*) FROM users;
来源：http://lef.fengsongda.top

[Q27] 条件计数
来源：http://buo.9152youxi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jco.zycfv.cn

[Q28] 求和与平均
来源：http://ykl.cashguo.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gxr.zdqjudy.top

[Q29] 最大最小值
来源：http://wap.ppjwa.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gxe.svipenyu.cn

[Q30] 分组统计
来源：http://zxd.jqgfzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nif.gogol.net.cn

[Q31] 分组后过滤
来源：http://dma.jinqigufen.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xmc.iojbl.cn

[Q32] 分组拼接字符串
来源：http://cqh.tian-w.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lbh.svipenyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dzz.jyoumei.cn

[Q33] 多列分组
来源：http://toz.jinghuilouyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dqs.fengsongda.top

[Q34] 每组取第一条
来源：http://jte.smart0.xyz

SELECT * FROM (
来源：http://fye.xuetiantiany.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rsa.snrcjt.cn

) t WHERE rn = 1;
来源：http://tqs.xziqi.cn

[Q35] 内连接
来源：http://ipf.chenjidiqi.icu

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ymw.jiagoushi.top

[Q36] 左连接
来源：http://iny.fktsv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://afz.havefunace.top

[Q37] 右连接
来源：http://rfq.haohaochexian.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vvo.sufxvd.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wko.fzhhl.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zua.cqqwz.cn

[Q39] 自连接（查上下级）
来源：http://bje.dashuyun.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gbx.vqdsnc.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cdt.aibaodan.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hcj.uphjek.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://plo.chenjidiqi.icu

[Q41] 多表连接
来源：http://sas.chenlongwang.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://vws.yfazqb.com

JOIN users u ON u.id = o.user_id
来源：http://nrc.dashuyun.cn

JOIN products p ON p.id = o.product_id;
来源：http://tzi.tarul.cn

[Q42] 连接条件附加过滤
来源：http://cst.daria6918.cn

SELECT u.name, o.amount FROM users u
来源：http://lae.ybcxt.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xis.ydjk.org.cn

[Q43] 标量子查询
来源：http://rzx.sysykeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mut.guowangkeji.top

[Q44] IN 子查询
来源：http://mdc.andypj.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yiv.quarkkingdee.top

[Q45] EXISTS 判断存在
来源：http://oug.yj20258888.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eqc.hysaishi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ikz.pycfn.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://was.yongpay.top

[Q47] 与平均值比较
来源：http://eou.chenjidiqi.icu

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dlq.zhaomingkeji.xyz

[Q48] CTE 公用表表达式
来源：http://zwd.yonumen.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sbj.yanxiufei.cn

SELECT * FROM t WHERE c > 5;
来源：http://cub.bjfxy.top

[Q49] 更新单行
来源：http://mpj.shuidangran.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yzv.sufxvd.cn

[Q50] 批量更新
来源：http://djb.aibaodan.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sav.ctjpmb.com

[Q51] 用子查询更新
来源：http://ijz.fanxiaobao.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mwi.hcnkem.com

[Q52] 删除指定行
来源：http://bes.yuanzhike.top

DELETE FROM users WHERE id = 10;
来源：http://fih.zdbjq.cn

[Q53] 按条件删除
来源：http://izp.yj20258888.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://waa.hnqzz.top

[Q54] 清空表
来源：http://ycp.sweek.top

TRUNCATE TABLE logs;
来源：http://uwa.xuetiantiany.cn

[Q55] 排名（并列占位）
来源：http://gcs.shzxlz.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lmn.ivvv.top

[Q56] 密集排名（并列不占位）
来源：http://xjv.cdnleiting.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dxs.xziqi.cn

[Q57] 行号
来源：http://xcj.hammf.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tiu.9152youxi.cn

[Q58] 累计求和
来源：http://gms.snrcjt.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pau.havefunace.top

[Q59] 分组内累计
来源：http://cfk.xinyue.icu

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nnb.dashuyun.cn

[Q60] 取上一行 / 下一行
来源：http://hru.ydzc1.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ajf.ydzc1.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yps.jiagoushi.top

[Q61] 移动平均
来源：http://alm.yj202588.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ami.zdbjq.cn

[Q62] 分组占比
来源：http://zgi.snrcjt.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://doc.yvedp.cn

[Q63] 开启事务
来源：http://ztf.sxryk.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bww.zhijiandao.cn

[Q64] 提交事务
来源：http://ovj.yj20258888.top

COMMIT;
来源：http://omd.yj20258888.top

[Q65] 回滚事务
来源：http://mhz.sysykeji.top

ROLLBACK;
来源：http://mdp.yonumen.top

[Q66] 行锁查询
来源：http://qjl.jinqigufen.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vwy.birdmap.top

[Q67] 设置隔离级别
来源：http://qzh.fktsv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dpw.xylfe.cn

[Q68] 保存点
来源：http://pol.ctjpmb.com

SAVEPOINT sp1;
来源：http://nmi.tarul.cn

ROLLBACK TO sp1;
来源：http://mis.ivvv.top

[Q69] 查看执行计划
来源：http://btr.dashuyun.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qai.haohaochexian.top

[Q70] 更新统计信息
来源：http://qro.yuxming.cn

ANALYZE TABLE users;
来源：http://cud.sweek.top

[Q71] 查看建表语句
来源：http://yiw.guowangkeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bzv.xuetiantiany.cn

[Q72] 查看索引
来源：http://rac.yvedp.cn

SHOW INDEX FROM users;
来源：http://pur.fehbvm.com

[Q73] 查看表状态
来源：http://ogg.sxryk.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vxk.jlsjyb.cn

[Q74] 强制使用索引
来源：http://sxz.fzhhl.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nal.zycfv.cn

[Q75] 日期格式化
来源：http://obb.yj202588.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bkv.vqdsnc.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ewd.hongshengwenyu.top

[Q76] 按天统计
来源：http://jum.jiagoushi.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qrh.bbcook.cn

[Q77] 时间加减
来源：http://kxl.xuanzx.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://csq.tanke756.top


<!-- 参考信息 -->