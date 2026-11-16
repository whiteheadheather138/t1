代发 wailian999

[O02] 使用线程池
来源：http://yjx.yangfankeji.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://trv.sxryk.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dgs.0kj1m.cn

JS:   // worker_threads 线程池
来源：http://lya.jinyuanbaomall.cn

TS:   // worker_threads 线程池
来源：http://plo.zhixingplan.top

Java: Executors.newFixedThreadPool(4)
来源：http://yzb.cashguo.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://orf.feifeiyinyue.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zzc.fengsongda.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tqr.cdnleiting.top

[O03] 加锁保护共享数据
来源：http://vww.ywan-chungtsiang.top

Py:   with lock: shared += 1
来源：http://qjb.aizwys.cn

PHP:  // 用 flock() 做文件锁
来源：http://urp.ctjpmb.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bcq.c1oappe.top

TS:   // 同 JS
来源：http://eev.dashuyun.cn

Java: synchronized (this) { shared++; }
来源：http://xjr.yonumen.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xeh.guowangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://efk.hywenlv.cn

C#:   lock (gate) { shared++; }
来源：http://hoc.yj202588.top

[O04] 定义异步函数并等待
来源：http://bzy.bbcook.cn

Py:   async def f():⏎    await g()
来源：http://fmr.shangyingyoupin.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://oiw.fengsongda.top

JS:   async function f() { await g(); }
来源：http://sxi.dianchejie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jic.ivvv.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dsd.yvedp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dfu.sweek.top

Ruby: # 用 Fiber 或 async gem
来源：http://lzh.vqdsnc.cn

C#:   async Task F() { await G(); }
来源：http://oel.gaohongyu789.top

[O05] 并发执行并等待全部完成
来源：http://mdl.jqgufenzy.top

Py:   asyncio.gather(*tasks)
来源：http://clr.kuanghao11.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://txx.zhaomingkeji.xyz

JS:   await Promise.all(tasks)
来源：http://pia.ppjwa.cn

TS:   await Promise.all(tasks)
来源：http://wmr.gogol.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ofl.yj202588.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cec.vqdsnc.cn

Ruby: threads.map(&:join)
来源：http://tvf.dianchejie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tym.yj20258.top

[O06] 使用进程池
来源：http://qhg.fzhhl.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sge.316326.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://fyj.pengpengdd.cyou

JS:   // child_process / cluster 模块
来源：http://pww.yangfankeji.com

TS:   // child_process / cluster 模块
来源：http://ajd.guannengcc.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ndc.sjlbkw.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zmo.xziqi.cn

Ruby: // fork 块
来源：http://zcw.daria6918.cn

C#:   Parallel.For
来源：http://bma.quarkkingdee.top

================================================================================
来源：http://mnc.yanxiufei.cn

P. 常用工具函数
来源：http://xhy.jlsjyb.cn

================================================================================
来源：http://hru.316326.xyz

[P01] 生成 UUID
来源：http://hcc.ywan-chungtsiang.top

Py:   str(uuid.uuid4())
来源：http://rtw.zhixingplan.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gkg.jqgfzy.top

JS:   crypto.randomUUID()
来源：http://gdu.c1oappe.top

TS:   crypto.randomUUID()
来源：http://pjt.52xcode.cn

Java: UUID.randomUUID().toString()
来源：http://yup.zhoulong.xyz

Go:   // 用 github.com/google/uuid
来源：http://dpw.dashuyun.cn

Ruby: SecureRandom.uuid
来源：http://lwh.wangshuangyany.cn

C#:   Guid.NewGuid().ToString()
来源：http://alp.zhongyouzk.top

[P02] MD5 / SHA256 摘要
来源：http://goa.0kj1m.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sid.jinqigfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qhz.kuanghao11.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dns.guannengcc.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xsq.quarkkingdee.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qoj.hysaishi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qlz.smart0.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://iqz.yangfankeji.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ayr.havefunace.top

[P03] 生成短随机字符串
来源：http://zln.xuetiantiany.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wuq.gzhubu.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://spb.yueranfly.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://evd.fehbvm.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://djd.tarul.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ijz.zhongyouzk.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cdr.fzhhl.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://vtb.mhx1999.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wra.iojbl.cn

[P04] 求长度
来源：http://tup.ivvv.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zcf.yvedp.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://agf.haohaochexian.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://znp.vqdsnc.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qkt.pycfn.com

Java: list.size();  map.size();  s.length()
来源：http://jqn.gotoacloud.top

Go:   len(arr);  len(m)
来源：http://yua.fehbvm.com

Ruby: x.length;  x.size
来源：http://gkx.hcnkem.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://gyp.nwbrower.top

[P05] 判断两个对象内容是否相等
来源：http://llm.xuetiantiany.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hzw.hywenlv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zgw.tanke756.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nuj.bjfxy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nmn.hysaishi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ppk.fehbvm.com

Go:   reflect.DeepEqual(a, b)
来源：http://yaz.yj20258.top

Ruby: a == b
来源：http://tcj.nwbrower.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vsg.vqdsnc.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sbp.shzxlz.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ygu.daria6918.cn

PHP:  if (empty($x)) {}
来源：http://uwu.nanxuanxn.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://puo.cashguo.top

TS:   if (x == null) {}
来源：http://yod.jyoumei.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uyg.ivvv.top

Go:   if x == nil {}
来源：http://brn.zhaomingkeji.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kwg.chenlongwang.top

C#:   if (x is null) {}
来源：http://syx.0kj1m.cn

[P07] 防抖与节流
来源：http://fzt.daxiang520.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lnk.yfazqb.com

PHP:  // 手写时间戳比较
来源：http://epv.hywenlv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kwe.jinyuanbaomall.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nkf.haohaochexian.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pjb.9152youxi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://goz.sxryk.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://cji.dianchejie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gro.wangshuangyany.cn

[P08] 处理浮点精度问题
来源：http://gkx.xuanzx.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xza.fehbvm.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vaa.zdqjudy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://clb.vehdjk.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://liw.epnwcf.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lqk.tian-w.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fnk.zhoulong.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bwr.yuxming.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vxu.jinghuilouyu.cn

================================================================================
来源：http://oev.zhijiandao.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mmr.kuanghao11.cn

================================================================================
来源：http://jid.zhoulong.xyz

[Q01] 创建表
来源：http://dwd.sysykeji.top

CREATE TABLE users (
来源：http://dzp.meibo888.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jqx.zhaomingkeji.xyz

name VARCHAR(50) NOT NULL,
来源：http://jsm.tanke756.top

email VARCHAR(100) UNIQUE,
来源：http://udb.hnxiangtu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ftb.tianlin.xyz

);
来源：http://tii.yanxiufei.cn

[Q02] 创建带外键的表
来源：http://jgl.meibo888.top

CREATE TABLE orders (
来源：http://szb.gzhubu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://adh.hywenlv.cn

user_id INT NOT NULL,
来源：http://xnc.ybcxt.top

amount DECIMAL(10, 2),
来源：http://kaf.zdqjudy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tgr.chenlongwang.top

);
来源：http://qgx.fehbvm.com

[Q03] 增加列
来源：http://com.snrcjt.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nbs.aizwys.cn

[Q04] 修改列类型
来源：http://tdu.aibaodan.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bsd.jinqigufen.top

[Q05] 重命名列
来源：http://pza.ivvv.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gbf.jinqigufen.top

[Q06] 删除列
来源：http://tqj.fktsv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://srr.tanke756.top

[Q07] 删除表
来源：http://vfq.52xcode.cn

DROP TABLE IF EXISTS orders;
来源：http://wtp.guowangkeji.top

[Q08] 创建普通索引
来源：http://djm.vehdjk.com

CREATE INDEX idx_users_email ON users(email);
来源：http://apm.zhongyouzk.top

[Q09] 创建唯一索引
来源：http://kzh.fzhhl.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rmg.zhengqikj.top

[Q10] 插入单行
来源：http://dcu.yonumen.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jqy.nwbrower.top

[Q11] 一次插入多行
来源：http://dah.xylfe.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rxx.hnqzz.top

[Q12] 插入后取自增 ID
来源：http://ivp.yonumen.top

INSERT INTO users (name) VALUES ('C');
来源：http://eol.jinghuilouyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tdm.cdnleiting.top

[Q13] 忽略重复插入
来源：http://rrc.hcnkem.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xnc.xuetiantiany.cn

[Q14] 存在则更新（upsert）
来源：http://ixn.ydjk.org.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jhv.vehdjk.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mvt.yj202588.top

[Q15] 查询全部
来源：http://dhn.svipenyu.cn

SELECT * FROM users;
来源：http://nzf.xinyue.icu

[Q16] 查询指定列
来源：http://pgf.pycfn.com

SELECT id, name FROM users;
来源：http://hpp.zhoulong.xyz

[Q17] 条件查询
来源：http://mdl.dianchejie.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://izb.yj20258.top

[Q18] 模糊匹配
来源：http://yzy.zdbjq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rrn.yueranfly.top

[Q19] 范围查询
来源：http://vbb.ivvv.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://viq.sweek.top

[Q20] IN 列表
来源：http://kdu.bjfxy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nrh.cqqwz.cn

[Q21] 空值判断
来源：http://llt.xuanzx.com

SELECT * FROM users WHERE email IS NULL;
来源：http://eiu.feifeiyinyue.top

[Q22] 排序
来源：http://pgq.fanxiaobao.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ret.quarkkingdee.top

[Q23] 分页
来源：http://uqv.ydzc1.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ygg.ybcxt.top

[Q24] 去重
来源：http://dvv.shanyushiyangkeji.top

SELECT DISTINCT city FROM users;
来源：http://mqw.fengsongda.top

[Q25] 只取前 N 条
来源：http://njk.sufxvd.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://owb.xuetiantiany.cn

[Q26] 计数
来源：http://nup.jyoumei.cn

SELECT COUNT(*) FROM users;
来源：http://lse.cdnleiting.top

[Q27] 条件计数
来源：http://sqq.meibo888.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ygt.316326.xyz

[Q28] 求和与平均
来源：http://hsr.guannengcc.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hym.wangdashe.top

[Q29] 最大最小值
来源：http://bry.fktsv.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://rug.uphjek.com

[Q30] 分组统计
来源：http://zhn.daxiang520.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://upd.yj20258.top

[Q31] 分组后过滤
来源：http://rdy.52xcode.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://iew.dashuyun.cn

[Q32] 分组拼接字符串
来源：http://tnz.fehbvm.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qhd.zhijiandao.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nzq.jinqigfzy.top

[Q33] 多列分组
来源：http://mxu.tarul.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ltj.vehdjk.com

[Q34] 每组取第一条
来源：http://kvb.yfazqb.com

SELECT * FROM (
来源：http://bsh.xziqi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zti.zhaomingkeji.xyz

) t WHERE rn = 1;
来源：http://okl.guowangkeji.top

[Q35] 内连接
来源：http://tne.ppjwa.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kro.uphjek.com

[Q36] 左连接
来源：http://jpw.yanxiufei.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ixp.nanxinkj.top

[Q37] 右连接
来源：http://doo.hesvh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zfa.zhengqikj.top

[Q38] 全外连接（PostgreSQL）
来源：http://fey.wangshuangyany.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gcq.ybcxt.top

[Q39] 自连接（查上下级）
来源：http://imv.jinyuanbaomall.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wmp.zhijiandao.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bee.ctjpmb.com

[Q40] 交叉连接（笛卡尔积）
来源：http://szk.yanxiufei.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qxn.daria6918.cn

[Q41] 多表连接
来源：http://erq.vqdsnc.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uwy.jinghuilouyu.cn

JOIN users u ON u.id = o.user_id
来源：http://bot.tarul.cn

JOIN products p ON p.id = o.product_id;
来源：http://iys.chenlongwang.top

[Q42] 连接条件附加过滤
来源：http://pav.sysykeji.top

SELECT u.name, o.amount FROM users u
来源：http://jde.yfazqb.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gsz.hnqzz.top

[Q43] 标量子查询
来源：http://jme.meibo888.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rsz.chenjidiqi.icu

[Q44] IN 子查询
来源：http://icx.52xcode.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xxq.xingfuxueyuan.xyz

[Q45] EXISTS 判断存在
来源：http://plc.ydjk.org.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bro.chenzaomai.com

[Q46] NOT EXISTS 判断不存在
来源：http://vrd.hnqzz.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://adk.fanxiaobao.xyz

[Q47] 与平均值比较
来源：http://oof.ctjpmb.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mmw.svipenyu.cn

[Q48] CTE 公用表表达式
来源：http://gcb.havefunace.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://quy.tarul.cn

SELECT * FROM t WHERE c > 5;
来源：http://tvn.zdbjq.cn

[Q49] 更新单行
来源：http://gpl.guowangkeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://iho.gotoacloud.top

[Q50] 批量更新
来源：http://kjj.jlsjyb.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hdc.ywan-chungtsiang.top

[Q51] 用子查询更新
来源：http://xyn.hysaishi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fnn.ctjpmb.com

[Q52] 删除指定行
来源：http://iik.316326.xyz

DELETE FROM users WHERE id = 10;
来源：http://gig.zhijiandao.cn

[Q53] 按条件删除
来源：http://wif.gogol.net.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wtx.zhengqikj.top

[Q54] 清空表
来源：http://dda.shangyingyoupin.top

TRUNCATE TABLE logs;
来源：http://uqn.sxryk.cn

[Q55] 排名（并列占位）
来源：http://hbl.zhijiandao.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pkb.jqgfzy.top

[Q56] 密集排名（并列不占位）
来源：http://sod.smart0.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vil.zhijiandao.cn

[Q57] 行号
来源：http://yty.zhengqikj.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://byc.jiagoushi.top

[Q58] 累计求和
来源：http://ovk.sysykeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://eqt.birdmap.top

[Q59] 分组内累计
来源：http://jgx.quarkkingdee.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zvc.yueranfly.top

[Q60] 取上一行 / 下一行
来源：http://ahm.svipenyu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gfd.smart0.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zei.svipenyu.cn

[Q61] 移动平均
来源：http://fbf.ydjk.org.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bzd.yanxiufei.cn

[Q62] 分组占比
来源：http://ewy.hcnkem.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ztk.pengpengdd.cyou

[Q63] 开启事务
来源：http://gwq.gzhubu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://yzn.dianchejie.cn

[Q64] 提交事务
来源：http://onn.cheryme.top

COMMIT;
来源：http://jgd.aizwys.cn

[Q65] 回滚事务
来源：http://dde.guannengcc.top

ROLLBACK;
来源：http://dvi.yongpay.top

[Q66] 行锁查询
来源：http://dqq.tian-w.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://imq.bjfxy.top

[Q67] 设置隔离级别
来源：http://gre.chenlongwang.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zpq.sufxvd.cn

[Q68] 保存点
来源：http://evs.shanyushiyangtech.top

SAVEPOINT sp1;
来源：http://xez.iojbl.cn

ROLLBACK TO sp1;
来源：http://fqo.hywenlv.cn

[Q69] 查看执行计划
来源：http://dwl.vqdsnc.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kuw.yj20258.top

[Q70] 更新统计信息
来源：http://eio.xingfuxueyuan.xyz

ANALYZE TABLE users;
来源：http://vny.zhoulong.xyz

[Q71] 查看建表语句
来源：http://ugl.nwbrower.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xpm.jyoumei.cn

[Q72] 查看索引
来源：http://tfg.guannengcc.top

SHOW INDEX FROM users;
来源：http://dvo.yongpay.top

[Q73] 查看表状态
来源：http://uoz.yj20258.top

SHOW TABLE STATUS LIKE 'users';
来源：http://hsa.ppjwa.cn

[Q74] 强制使用索引
来源：http://kxl.zhiwuduotai.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rkz.redwolf501.top

[Q75] 日期格式化
来源：http://qub.hammf.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fwg.ydzc1.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lfo.jyoumei.cn

[Q76] 按天统计
来源：http://kvz.xuetiantiany.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://den.zhengqikj.top

[Q77] 时间加减
来源：http://hsv.gaohongyu789.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kcx.pycfn.com


<!-- 参考信息 -->