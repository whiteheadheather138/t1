代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://gdd.bbcook.cn

Go:   go f()
来源：http://eiu.tanke756.top

Ruby: Thread.new { f }
来源：http://xqd.cheryme.top

C#:   Task.Run(() => F());
来源：http://hyq.nwbrower.top

[O02] 使用线程池
来源：http://mvv.guowangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lyq.xinyue.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kmm.ivvv.top

JS:   // worker_threads 线程池
来源：http://rfg.fanxiaobao.xyz

TS:   // worker_threads 线程池
来源：http://vzi.yj20258.top

Java: Executors.newFixedThreadPool(4)
来源：http://ves.jinghuilouyu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pew.jyoumei.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qas.jlsjyb.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qag.pycfn.com

[O03] 加锁保护共享数据
来源：http://mvm.hnqzz.top

Py:   with lock: shared += 1
来源：http://ech.zhixingplan.top

PHP:  // 用 flock() 做文件锁
来源：http://cut.wangdashe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uck.yj20258.top

TS:   // 同 JS
来源：http://cym.yonumen.top

Java: synchronized (this) { shared++; }
来源：http://zmy.hfpthk.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qor.0kj1m.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ybp.zhaomingkeji.xyz

C#:   lock (gate) { shared++; }
来源：http://sdq.ppjwa.cn

[O04] 定义异步函数并等待
来源：http://trj.hcnkem.com

Py:   async def f():⏎    await g()
来源：http://xyr.chenzaomai.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blp.sweek.top

JS:   async function f() { await g(); }
来源：http://ird.tarul.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xpb.c1oappe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ppv.fehbvm.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mym.fzhhl.top

Ruby: # 用 Fiber 或 async gem
来源：http://xyh.tianlin.xyz

C#:   async Task F() { await G(); }
来源：http://rvo.gotoacloud.top

[O05] 并发执行并等待全部完成
来源：http://hzu.shanyushiyangkeji.top

Py:   asyncio.gather(*tasks)
来源：http://hvu.jlsjyb.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rrk.hfpthk.cn

JS:   await Promise.all(tasks)
来源：http://ldb.chenjidiqi.icu

TS:   await Promise.all(tasks)
来源：http://dud.yanxiufei.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cns.snrcjt.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://drf.pycfn.com

Ruby: threads.map(&:join)
来源：http://hiy.guannengcc.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mqg.zdbjq.cn

[O06] 使用进程池
来源：http://drh.pengpengdd.cyou

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ikl.yfazqb.com

PHP:  // pcntl_fork 或多进程队列
来源：http://ywn.yongpay.top

JS:   // child_process / cluster 模块
来源：http://fsx.uphjek.com

TS:   // child_process / cluster 模块
来源：http://rdv.c1oappe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://epr.zhixingplan.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vvq.havefunace.top

Ruby: // fork 块
来源：http://jvi.jiagoushi.top

C#:   Parallel.For
来源：http://iwq.tarul.cn

================================================================================
来源：http://vxd.nwbrower.top

P. 常用工具函数
来源：http://wyq.yfazqb.com

================================================================================
来源：http://yfa.epnwcf.com

[P01] 生成 UUID
来源：http://bza.9152youxi.cn

Py:   str(uuid.uuid4())
来源：http://ayr.yuxming.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jze.yfazqb.com

JS:   crypto.randomUUID()
来源：http://yco.jinyuanbaomall.cn

TS:   crypto.randomUUID()
来源：http://mgd.shanyushiyangtech.top

Java: UUID.randomUUID().toString()
来源：http://pvj.tanke756.top

Go:   // 用 github.com/google/uuid
来源：http://sub.pengpengdd.cyou

Ruby: SecureRandom.uuid
来源：http://rxq.vqdsnc.cn

C#:   Guid.NewGuid().ToString()
来源：http://ahu.cashguo.top

[P02] MD5 / SHA256 摘要
来源：http://hda.ydzc1.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xtv.ivvv.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://xst.yuanzhike.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://udv.cucudq.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ysb.shanyushiyangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://slw.quarkkingdee.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jaw.yonumen.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ooj.bbcook.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bqt.fehbvm.com

[P03] 生成短随机字符串
来源：http://gbl.jqgfzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rop.sweek.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wcg.ywan-chungtsiang.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zyw.chenjidiqi.icu

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gfl.jyoumei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yrc.ehwqpu.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tuz.wangshuangyany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jep.cdnleiting.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bem.ybcxt.top

[P04] 求长度
来源：http://aki.guannengcc.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rrj.shzxlz.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uus.pengpengdd.cyou

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eux.jiagoushi.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bql.sxryk.cn

Java: list.size();  map.size();  s.length()
来源：http://irg.yuxming.cn

Go:   len(arr);  len(m)
来源：http://ahv.fengsongda.top

Ruby: x.length;  x.size
来源：http://asz.nanxuanxn.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://lvc.wangdashe.top

[P05] 判断两个对象内容是否相等
来源：http://tfa.hammf.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pda.fzhhl.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gsw.yvedp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://suu.dianchejie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hdi.zdbjq.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uwe.ydjk.org.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xoy.cashguo.top

Ruby: a == b
来源：http://xqm.pengpengdd.cyou

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yon.shangyingyoupin.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dxe.sweek.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wiv.haohaochexian.top

PHP:  if (empty($x)) {}
来源：http://grw.dashuyun.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zuh.tarul.cn

TS:   if (x == null) {}
来源：http://wgq.haohaochexian.top

Java: if (x == null || x.isEmpty()) {}
来源：http://liw.yj202588.top

Go:   if x == nil {}
来源：http://fwm.birdmap.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zkn.xingfuxueyuan.xyz

C#:   if (x is null) {}
来源：http://lij.meibo888.top

[P07] 防抖与节流
来源：http://hhk.sysykeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uha.yfazqb.com

PHP:  // 手写时间戳比较
来源：http://tfo.cheryme.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ryq.jinqigfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://svg.nanxuanxn.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kor.zhengqikj.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dup.yonumen.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://cxy.hywenlv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wfz.smart0.xyz

[P08] 处理浮点精度问题
来源：http://nrx.guowangkeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://inc.tian-w.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gum.yuxming.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zrv.aibaodan.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fwf.jinghuilouyu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mtk.fzhhl.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qig.hnxiangtu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qbc.yuanzhike.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xfz.nanxinkj.top

================================================================================
来源：http://jxr.jinghuilouyu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vqt.nanxinkj.top

================================================================================
来源：http://mxw.xuanzx.com

[Q01] 创建表
来源：http://ftn.shangyingyoupin.top

CREATE TABLE users (
来源：http://avf.c1oappe.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dko.havefunace.top

name VARCHAR(50) NOT NULL,
来源：http://rsq.9152youxi.cn

email VARCHAR(100) UNIQUE,
来源：http://guv.aizwys.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ydz.guowangkeji.top

);
来源：http://lxz.cqqwz.cn

[Q02] 创建带外键的表
来源：http://fkw.sjlbkw.cn

CREATE TABLE orders (
来源：http://fgc.fzhhl.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://suk.shanyushiyangtech.top

user_id INT NOT NULL,
来源：http://fgv.jqgfzy.top

amount DECIMAL(10, 2),
来源：http://zom.yonumen.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qwi.sjlbkw.cn

);
来源：http://qop.cucudq.cn

[Q03] 增加列
来源：http://mlr.guannengcc.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gxv.jinghuilouyu.cn

[Q04] 修改列类型
来源：http://oyp.epnwcf.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dbo.0kj1m.cn

[Q05] 重命名列
来源：http://gal.316326.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qaj.fktsv.cn

[Q06] 删除列
来源：http://tbc.meibo888.top

ALTER TABLE users DROP COLUMN age;
来源：http://pkf.gogol.net.cn

[Q07] 删除表
来源：http://hlf.zhongyouzk.top

DROP TABLE IF EXISTS orders;
来源：http://yxh.cucudq.cn

[Q08] 创建普通索引
来源：http://auo.zhijiandao.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wcg.yonumen.top

[Q09] 创建唯一索引
来源：http://cfe.pycfn.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bej.daxiang520.top

[Q10] 插入单行
来源：http://lsj.cqqwz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://enj.9152youxi.cn

[Q11] 一次插入多行
来源：http://jwo.cqqwz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://era.ydjk.org.cn

[Q12] 插入后取自增 ID
来源：http://gdo.ybcxt.top

INSERT INTO users (name) VALUES ('C');
来源：http://vnv.jinqigufen.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://orq.guowangkeji.top

[Q13] 忽略重复插入
来源：http://iqm.hesvh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://eue.snrcjt.cn

[Q14] 存在则更新（upsert）
来源：http://iyb.c1oappe.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gfg.tanke756.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://suo.hcnkem.com

[Q15] 查询全部
来源：http://kxh.bbcook.cn

SELECT * FROM users;
来源：http://swx.snrcjt.cn

[Q16] 查询指定列
来源：http://ldm.nanxinkj.top

SELECT id, name FROM users;
来源：http://yoi.chenlongwang.top

[Q17] 条件查询
来源：http://viz.redwolf501.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://niv.tanke756.top

[Q18] 模糊匹配
来源：http://kpj.0kj1m.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hxg.sjlbkw.cn

[Q19] 范围查询
来源：http://iqv.yfazqb.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kju.xingfuxueyuan.xyz

[Q20] IN 列表
来源：http://cgi.feifeiyinyue.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jtc.yongpay.top

[Q21] 空值判断
来源：http://klx.xingfuxueyuan.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://ggg.hysaishi.cn

[Q22] 排序
来源：http://kgh.chenzaomai.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dnt.nanxinkj.top

[Q23] 分页
来源：http://hkh.bbcook.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gzv.ivvv.top

[Q24] 去重
来源：http://gxq.fengsongda.top

SELECT DISTINCT city FROM users;
来源：http://yla.0kj1m.cn

[Q25] 只取前 N 条
来源：http://myz.gogol.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://naw.yvedp.cn

[Q26] 计数
来源：http://xdf.nanxinkj.top

SELECT COUNT(*) FROM users;
来源：http://iet.fktsv.cn

[Q27] 条件计数
来源：http://fiw.zhijiandao.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xmg.sweek.top

[Q28] 求和与平均
来源：http://fkk.9152youxi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mwm.hnqzz.top

[Q29] 最大最小值
来源：http://qck.gogol.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://glw.shuidangran.top

[Q30] 分组统计
来源：http://xbg.fktsv.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cyb.dianchejie.cn

[Q31] 分组后过滤
来源：http://qrl.gzhubu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fxd.vehdjk.com

[Q32] 分组拼接字符串
来源：http://ule.shanyushiyangkeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://aoh.haohaochexian.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://akg.cqqwz.cn

[Q33] 多列分组
来源：http://ept.ydjk.org.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ott.tian-w.cn

[Q34] 每组取第一条
来源：http://fmq.xuanzx.com

SELECT * FROM (
来源：http://usj.zhixingplan.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://edb.ehwqpu.com

) t WHERE rn = 1;
来源：http://qsi.yj20258.top

[Q35] 内连接
来源：http://dku.jlsjyb.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://juu.ppjwa.cn

[Q36] 左连接
来源：http://umk.yj20258888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kpk.uphjek.com

[Q37] 右连接
来源：http://teh.yanxiufei.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qqi.svipenyu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bst.shzxlz.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rrg.jinqigfzy.top

[Q39] 自连接（查上下级）
来源：http://whu.jlsjyb.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wqz.yongpay.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tok.fktsv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jpp.svipenyu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cor.fktsv.cn

[Q41] 多表连接
来源：http://pyf.chenjidiqi.icu

SELECT o.id, u.name, p.title FROM orders o
来源：http://knm.zycfv.cn

JOIN users u ON u.id = o.user_id
来源：http://ifx.shangyingyoupin.top

JOIN products p ON p.id = o.product_id;
来源：http://vqt.shanyushiyangtech.top

[Q42] 连接条件附加过滤
来源：http://wya.zycfv.cn

SELECT u.name, o.amount FROM users u
来源：http://uqe.smart0.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gbl.cheryme.top

[Q43] 标量子查询
来源：http://pkc.nanxuanxn.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://djn.zhongyouzk.top

[Q44] IN 子查询
来源：http://nrb.tian-w.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jzx.316326.xyz

[Q45] EXISTS 判断存在
来源：http://pkb.dashuyun.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cos.sjlbkw.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hub.316326.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uwl.zhongyouzk.top

[Q47] 与平均值比较
来源：http://wuf.hnqzz.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lai.yangfankeji.com

[Q48] CTE 公用表表达式
来源：http://hxz.quarkkingdee.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ksq.haohaochexian.top

SELECT * FROM t WHERE c > 5;
来源：http://tah.hammf.cn

[Q49] 更新单行
来源：http://ktn.hfpthk.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kdm.shanyushiyangtech.top

[Q50] 批量更新
来源：http://nsl.nanxinkj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tcl.gotoacloud.top

[Q51] 用子查询更新
来源：http://zle.xinyue.icu

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wpw.birdmap.top

[Q52] 删除指定行
来源：http://hhn.shanyushiyangkeji.top

DELETE FROM users WHERE id = 10;
来源：http://hgh.cashguo.top

[Q53] 按条件删除
来源：http://obq.guowangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jkm.yanxiufei.cn

[Q54] 清空表
来源：http://rhg.yj20258.top

TRUNCATE TABLE logs;
来源：http://shn.daxiang520.top

[Q55] 排名（并列占位）
来源：http://jdr.yongpay.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bkh.jinqigfzy.top

[Q56] 密集排名（并列不占位）
来源：http://tmc.zhiwuduotai.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gdv.haohaochexian.top

[Q57] 行号
来源：http://vvd.zdbjq.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eyg.fengsongda.top

[Q58] 累计求和
来源：http://efo.hnqzz.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://khz.jqgfzy.top

[Q59] 分组内累计
来源：http://poa.cdnleiting.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://omp.cheryme.top

[Q60] 取上一行 / 下一行
来源：http://hco.zhongyouzk.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hwn.tianlin.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ycl.jiagoushi.top

[Q61] 移动平均
来源：http://zay.tian-w.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cto.pycfn.com

[Q62] 分组占比
来源：http://vza.fehbvm.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lth.yj202588.top

[Q63] 开启事务
来源：http://hmk.jinyuanbaomall.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vnq.yanxiufei.cn

[Q64] 提交事务
来源：http://ogv.nanxinkj.top

COMMIT;
来源：http://adb.xinyue.icu

[Q65] 回滚事务
来源：http://mta.smart0.xyz

ROLLBACK;
来源：http://med.gzhubu.top

[Q66] 行锁查询
来源：http://kev.jinghuilouyu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sdz.hfpthk.cn

[Q67] 设置隔离级别
来源：http://zum.mhx1999.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bby.aibaodan.cn

[Q68] 保存点
来源：http://yep.hongshengwenyu.top

SAVEPOINT sp1;
来源：http://rcw.guowangkeji.top

ROLLBACK TO sp1;
来源：http://noc.jianghu66.top

[Q69] 查看执行计划
来源：http://tqa.chenjidiqi.icu

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mcp.fengsongda.top

[Q70] 更新统计信息
来源：http://vtm.daxiang520.top

ANALYZE TABLE users;
来源：http://gpi.jyoumei.cn

[Q71] 查看建表语句
来源：http://yok.nanxinkj.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://piy.ctjpmb.com

[Q72] 查看索引
来源：http://blp.xylfe.cn

SHOW INDEX FROM users;
来源：http://aho.dashuyun.cn

[Q73] 查看表状态
来源：http://lvt.guannengcc.top

SHOW TABLE STATUS LIKE 'users';
来源：http://dts.yuxming.cn

[Q74] 强制使用索引
来源：http://xjt.tianlin.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pvn.havefunace.top

[Q75] 日期格式化
来源：http://jqs.sysykeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mph.tianlin.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kmg.dashuyun.cn


<!-- 参考信息 -->