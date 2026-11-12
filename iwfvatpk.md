代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://trg.yj20258.top

Go:   go f()
来源：http://jgz.xuanzx.com

Ruby: Thread.new { f }
来源：http://uws.daria6918.cn

C#:   Task.Run(() => F());
来源：http://rjv.52xcode.cn

[O02] 使用线程池
来源：http://xgl.chenzaomai.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dks.tianlin.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://aux.tanke756.top

JS:   // worker_threads 线程池
来源：http://ohd.zdqjudy.top

TS:   // worker_threads 线程池
来源：http://mby.yj20258888.top

Java: Executors.newFixedThreadPool(4)
来源：http://jdm.fktsv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zgi.wangdashe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pml.yanxiufei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vfj.feifeiyinyue.top

[O03] 加锁保护共享数据
来源：http://zve.xylfe.cn

Py:   with lock: shared += 1
来源：http://uhn.c1oappe.top

PHP:  // 用 flock() 做文件锁
来源：http://oqw.fehbvm.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qfy.daxiang520.top

TS:   // 同 JS
来源：http://oxa.chenjidiqi.icu

Java: synchronized (this) { shared++; }
来源：http://pwa.hywenlv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jur.zhixingplan.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jar.52xcode.cn

C#:   lock (gate) { shared++; }
来源：http://dkw.0kj1m.cn

[O04] 定义异步函数并等待
来源：http://ayl.ydzc1.top

Py:   async def f():⏎    await g()
来源：http://ksi.fanxiaobao.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gdp.xylfe.cn

JS:   async function f() { await g(); }
来源：http://eyq.zhaomingkeji.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://krl.tanke756.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ufn.xylfe.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ipk.nwbrower.top

Ruby: # 用 Fiber 或 async gem
来源：http://kzv.hnqzz.top

C#:   async Task F() { await G(); }
来源：http://wim.zhiwuduotai.top

[O05] 并发执行并等待全部完成
来源：http://zpx.jinqigfzy.top

Py:   asyncio.gather(*tasks)
来源：http://rns.xingfuxueyuan.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dll.ybcxt.top

JS:   await Promise.all(tasks)
来源：http://wnv.ppjwa.cn

TS:   await Promise.all(tasks)
来源：http://sek.svipenyu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kvc.nanxinkj.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mjt.tianlin.xyz

Ruby: threads.map(&:join)
来源：http://ugy.uphjek.com

C#:   await Task.WhenAll(t1, t2)
来源：http://nse.shangyingyoupin.top

[O06] 使用进程池
来源：http://lxm.chenjidiqi.icu

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qnu.sysykeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://xnj.ctjpmb.com

JS:   // child_process / cluster 模块
来源：http://xal.dianchejie.cn

TS:   // child_process / cluster 模块
来源：http://ozj.bjfxy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dnd.birdmap.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lzl.cashguo.top

Ruby: // fork 块
来源：http://dqb.hammf.cn

C#:   Parallel.For
来源：http://kfy.jyoumei.cn

================================================================================
来源：http://nbn.jlsjyb.cn

P. 常用工具函数
来源：http://mii.yj20258888.top

================================================================================
来源：http://bhk.yuxming.cn

[P01] 生成 UUID
来源：http://tpk.svipenyu.cn

Py:   str(uuid.uuid4())
来源：http://vaj.zhiwuduotai.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hgs.xingfuxueyuan.xyz

JS:   crypto.randomUUID()
来源：http://bik.daxiang520.top

TS:   crypto.randomUUID()
来源：http://dys.hesvh.cn

Java: UUID.randomUUID().toString()
来源：http://rba.xuetiantiany.cn

Go:   // 用 github.com/google/uuid
来源：http://yka.yfazqb.com

Ruby: SecureRandom.uuid
来源：http://ctf.zhoulong.xyz

C#:   Guid.NewGuid().ToString()
来源：http://dfh.chenlongwang.top

[P02] MD5 / SHA256 摘要
来源：http://ggv.cqqwz.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kbu.hywenlv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ony.shangyingyoupin.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kzn.52xcode.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xyp.nanxinkj.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lki.yj20258888.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nqm.zycfv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gmq.jinyuanbaomall.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rqu.tarul.cn

[P03] 生成短随机字符串
来源：http://qxc.sweek.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sqc.zdqjudy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hea.cdnleiting.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ost.yj20258888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kvv.nanxuanxn.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hrk.316326.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://acs.tian-w.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://afp.gogol.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://snz.zdbjq.cn

[P04] 求长度
来源：http://iya.jianghu66.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pyq.hammf.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nno.wangshuangyany.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hfx.redwolf501.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cin.tian-w.cn

Java: list.size();  map.size();  s.length()
来源：http://ezi.xylfe.cn

Go:   len(arr);  len(m)
来源：http://jqi.xingfuxueyuan.xyz

Ruby: x.length;  x.size
来源：http://btd.dashuyun.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ajj.zhijiandao.cn

[P05] 判断两个对象内容是否相等
来源：http://hwg.guowangkeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://xfd.ydzc1.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nlz.sxryk.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bja.chenjidiqi.icu

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lfm.jinqigfzy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gua.ybcxt.top

Go:   reflect.DeepEqual(a, b)
来源：http://ysw.tanke756.top

Ruby: a == b
来源：http://zhw.hysaishi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mrr.birdmap.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://avu.cheryme.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zkc.fanxiaobao.xyz

PHP:  if (empty($x)) {}
来源：http://uck.zycfv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kdj.yueranfly.top

TS:   if (x == null) {}
来源：http://lsm.hywenlv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://iek.nwbrower.top

Go:   if x == nil {}
来源：http://zmw.hongshengwenyu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://aoc.chenlongwang.top

C#:   if (x is null) {}
来源：http://ehw.iojbl.cn

[P07] 防抖与节流
来源：http://pav.svipenyu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mgj.gotoacloud.top

PHP:  // 手写时间戳比较
来源：http://bhl.jianghu66.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tey.shangyingyoupin.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kfl.shangyingyoupin.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ook.zhixingplan.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uoi.xuanzx.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://mnf.ybcxt.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ugk.svipenyu.cn

[P08] 处理浮点精度问题
来源：http://gvl.xziqi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://olq.ppjwa.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qvw.jiagoushi.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vme.jinghuilouyu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yiq.hcnkem.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ohc.feifeiyinyue.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ele.jinqigufen.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pup.guannengcc.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kjr.dashuyun.cn

================================================================================
来源：http://ikq.ydjk.org.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pbt.meibo888.top

================================================================================
来源：http://mem.bbcook.cn

[Q01] 创建表
来源：http://kqp.zhongyouzk.top

CREATE TABLE users (
来源：http://blz.hongshengwenyu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hel.zycfv.cn

name VARCHAR(50) NOT NULL,
来源：http://ccc.chenlongwang.top

email VARCHAR(100) UNIQUE,
来源：http://wxo.ivvv.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jto.jqgfzy.top

);
来源：http://guj.0kj1m.cn

[Q02] 创建带外键的表
来源：http://wwv.zycfv.cn

CREATE TABLE orders (
来源：http://hso.bbcook.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xro.yangfankeji.com

user_id INT NOT NULL,
来源：http://elb.zhengqikj.top

amount DECIMAL(10, 2),
来源：http://mma.aizwys.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dev.cheryme.top

);
来源：http://eoo.jqgfzy.top

[Q03] 增加列
来源：http://zed.sweek.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yes.sjlbkw.cn

[Q04] 修改列类型
来源：http://osr.jlsjyb.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://neu.wangshuangyany.cn

[Q05] 重命名列
来源：http://kqv.jinghuilouyu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ypz.guannengcc.top

[Q06] 删除列
来源：http://yua.jqgfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://jbh.tian-w.cn

[Q07] 删除表
来源：http://wsp.cheryme.top

DROP TABLE IF EXISTS orders;
来源：http://lru.cashguo.top

[Q08] 创建普通索引
来源：http://won.daria6918.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://meq.shangyingyoupin.top

[Q09] 创建唯一索引
来源：http://aia.hywenlv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://das.xuanzx.com

[Q10] 插入单行
来源：http://cvj.tian-w.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ost.nwbrower.top

[Q11] 一次插入多行
来源：http://vtg.smart0.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mmf.redwolf501.top

[Q12] 插入后取自增 ID
来源：http://tip.svipenyu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://zfb.sxryk.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zql.zhengqikj.top

[Q13] 忽略重复插入
来源：http://ryl.ybcxt.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lsk.sweek.top

[Q14] 存在则更新（upsert）
来源：http://hpf.hesvh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tdm.quarkkingdee.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rna.pengpengdd.cyou

[Q15] 查询全部
来源：http://hly.sweek.top

SELECT * FROM users;
来源：http://zpe.fanxiaobao.xyz

[Q16] 查询指定列
来源：http://ucs.jinyuanbaomall.cn

SELECT id, name FROM users;
来源：http://uob.jianghu66.top

[Q17] 条件查询
来源：http://usj.cqqwz.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mha.daxiang520.top

[Q18] 模糊匹配
来源：http://aqu.yonumen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mjh.tanke756.top

[Q19] 范围查询
来源：http://ujv.jqgufenzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rvd.yuanzhike.top

[Q20] IN 列表
来源：http://aky.feifeiyinyue.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://doo.shanyushiyangtech.top

[Q21] 空值判断
来源：http://vny.hongshengwenyu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://enk.jlsjyb.cn

[Q22] 排序
来源：http://whv.meibo888.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mtl.nanxuanxn.top

[Q23] 分页
来源：http://gem.yangfankeji.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rwa.pycfn.com

[Q24] 去重
来源：http://fbm.vehdjk.com

SELECT DISTINCT city FROM users;
来源：http://jev.52xcode.cn

[Q25] 只取前 N 条
来源：http://eer.xylfe.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pui.xuetiantiany.cn

[Q26] 计数
来源：http://tcq.yonumen.top

SELECT COUNT(*) FROM users;
来源：http://lwd.tanke756.top

[Q27] 条件计数
来源：http://xlk.ehwqpu.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://osl.jinqigfzy.top

[Q28] 求和与平均
来源：http://fhu.shzxlz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zlc.chenjidiqi.icu

[Q29] 最大最小值
来源：http://ssj.snrcjt.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zwu.ybcxt.top

[Q30] 分组统计
来源：http://cua.jinyuanbaomall.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kcp.tian-w.cn

[Q31] 分组后过滤
来源：http://mvi.yonumen.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mxj.smart0.xyz

[Q32] 分组拼接字符串
来源：http://rxy.yuanzhike.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eyd.zdqjudy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ojq.pycfn.com

[Q33] 多列分组
来源：http://lzi.shanyushiyangtech.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dlx.jinqigfzy.top

[Q34] 每组取第一条
来源：http://ofy.jinghuilouyu.cn

SELECT * FROM (
来源：http://oiv.zhaomingkeji.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tku.guowangkeji.top

) t WHERE rn = 1;
来源：http://crj.cdnleiting.top

[Q35] 内连接
来源：http://moa.52xcode.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://sxa.c1oappe.top

[Q36] 左连接
来源：http://lct.yonumen.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://czz.yfazqb.com

[Q37] 右连接
来源：http://vfh.wangdashe.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bmt.birdmap.top

[Q38] 全外连接（PostgreSQL）
来源：http://fps.quarkkingdee.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cie.0kj1m.cn

[Q39] 自连接（查上下级）
来源：http://ygb.svipenyu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ttm.yj202588.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hnz.shuidangran.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zmh.jqgufenzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ixa.mhx1999.top

[Q41] 多表连接
来源：http://xks.pengpengdd.cyou

SELECT o.id, u.name, p.title FROM orders o
来源：http://dov.c1oappe.top

JOIN users u ON u.id = o.user_id
来源：http://qzh.zycfv.cn

JOIN products p ON p.id = o.product_id;
来源：http://tgk.hywenlv.cn

[Q42] 连接条件附加过滤
来源：http://hjq.daria6918.cn

SELECT u.name, o.amount FROM users u
来源：http://ipc.cheryme.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jts.aizwys.cn

[Q43] 标量子查询
来源：http://dnn.hammf.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://slh.9152youxi.cn

[Q44] IN 子查询
来源：http://wnj.jinqigufen.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zkw.sysykeji.top

[Q45] EXISTS 判断存在
来源：http://sck.cdnleiting.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://krd.pengpengdd.cyou

[Q46] NOT EXISTS 判断不存在
来源：http://byk.gogol.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mjv.yuanzhike.top

[Q47] 与平均值比较
来源：http://uqn.gaohongyu789.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://knr.andypj.xyz

[Q48] CTE 公用表表达式
来源：http://kxw.hnxiangtu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gzo.cashguo.top

SELECT * FROM t WHERE c > 5;
来源：http://yjd.jqgufenzy.top

[Q49] 更新单行
来源：http://buy.zdbjq.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jgc.pengpengdd.cyou

[Q50] 批量更新
来源：http://uem.guannengcc.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ssr.zdqjudy.top

[Q51] 用子查询更新
来源：http://vud.hesvh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cuw.shzxlz.cn

[Q52] 删除指定行
来源：http://zcw.vqdsnc.cn

DELETE FROM users WHERE id = 10;
来源：http://que.daxiang520.top

[Q53] 按条件删除
来源：http://wog.jqgfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://agf.yj20258888.top

[Q54] 清空表
来源：http://qrg.zdbjq.cn

TRUNCATE TABLE logs;
来源：http://cue.gzhubu.top

[Q55] 排名（并列占位）
来源：http://ght.ydjk.org.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lzc.cucudq.cn

[Q56] 密集排名（并列不占位）
来源：http://nai.c1oappe.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ukq.epnwcf.com

[Q57] 行号
来源：http://oso.pengpengdd.cyou

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fdg.bjfxy.top

[Q58] 累计求和
来源：http://qku.316326.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uks.shangyingyoupin.top

[Q59] 分组内累计
来源：http://aad.sysykeji.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://onq.gotoacloud.top

[Q60] 取上一行 / 下一行
来源：http://rxx.shanyushiyangtech.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mnf.c1oappe.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wji.shanyushiyangkeji.top

[Q61] 移动平均
来源：http://ilz.yj20258888.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ngb.cucudq.cn

[Q62] 分组占比
来源：http://laa.snrcjt.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qpd.fktsv.cn

[Q63] 开启事务
来源：http://kbg.ybcxt.top

START TRANSACTION;                -- 或 BEGIN
来源：http://aig.pycfn.com

[Q64] 提交事务
来源：http://mur.nwbrower.top

COMMIT;
来源：http://wte.dianchejie.cn

[Q65] 回滚事务
来源：http://rka.shangyingyoupin.top

ROLLBACK;
来源：http://frg.shanyushiyangtech.top

[Q66] 行锁查询
来源：http://fbu.zhaomingkeji.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rfn.quarkkingdee.top

[Q67] 设置隔离级别
来源：http://yed.ydzc1.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xgb.xinyue.icu

[Q68] 保存点
来源：http://rjj.zdqjudy.top

SAVEPOINT sp1;
来源：http://fsr.uphjek.com

ROLLBACK TO sp1;
来源：http://aqp.zycfv.cn

[Q69] 查看执行计划
来源：http://tem.hongshengwenyu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hqw.xinyue.icu

[Q70] 更新统计信息
来源：http://xef.xylfe.cn

ANALYZE TABLE users;
来源：http://gsf.pycfn.com

[Q71] 查看建表语句
来源：http://mwb.zhiwuduotai.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://spd.cucudq.cn

[Q72] 查看索引
来源：http://oqm.sufxvd.cn

SHOW INDEX FROM users;
来源：http://vjl.chenjidiqi.icu

[Q73] 查看表状态
来源：http://ccn.tarul.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nev.bbcook.cn

[Q74] 强制使用索引
来源：http://skw.hywenlv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uxe.tianlin.xyz

[Q75] 日期格式化
来源：http://zlh.jinghuilouyu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zzj.chenlongwang.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nlm.fengsongda.top


<!-- 参考信息 -->