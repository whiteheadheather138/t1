代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://atv.zhengqikj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xqx.meibo888.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rsl.shzxlz.cn

TS:   // 同 JS
来源：http://hxh.bbcook.cn

Java: new Thread(() -> f()).start()
来源：http://ups.jinyuanbaomall.cn

Go:   go f()
来源：http://itf.daria6918.cn

Ruby: Thread.new { f }
来源：http://gen.sufxvd.cn

C#:   Task.Run(() => F());
来源：http://jnx.yvedp.cn

[O02] 使用线程池
来源：http://tpf.shuidangran.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vhx.zycfv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hkq.xingfuxueyuan.xyz

JS:   // worker_threads 线程池
来源：http://bjs.yj20258.top

TS:   // worker_threads 线程池
来源：http://xss.fengsongda.top

Java: Executors.newFixedThreadPool(4)
来源：http://ags.ydjk.org.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nmv.nanxinkj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cmy.svipenyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tfv.dianchejie.cn

[O03] 加锁保护共享数据
来源：http://pmt.shuidangran.top

Py:   with lock: shared += 1
来源：http://llv.jqgfzy.top

PHP:  // 用 flock() 做文件锁
来源：http://jqa.ywan-chungtsiang.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gfs.pengpengdd.cyou

TS:   // 同 JS
来源：http://fng.dianchejie.cn

Java: synchronized (this) { shared++; }
来源：http://gjd.mhx1999.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nvf.sufxvd.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lae.shangyingyoupin.top

C#:   lock (gate) { shared++; }
来源：http://wbz.smart0.xyz

[O04] 定义异步函数并等待
来源：http://tai.bjfxy.top

Py:   async def f():⏎    await g()
来源：http://xpn.guannengcc.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rwq.havefunace.top

JS:   async function f() { await g(); }
来源：http://jnz.sjlbkw.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tat.xuanzx.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qmn.sweek.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gbl.xziqi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qtk.fehbvm.com

C#:   async Task F() { await G(); }
来源：http://vbh.haohaochexian.top

[O05] 并发执行并等待全部完成
来源：http://arf.shanyushiyangkeji.top

Py:   asyncio.gather(*tasks)
来源：http://oet.zhaomingkeji.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cvt.jinqigufen.top

JS:   await Promise.all(tasks)
来源：http://opx.sysykeji.top

TS:   await Promise.all(tasks)
来源：http://nqu.xinyue.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://stq.ppjwa.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fid.pycfn.com

Ruby: threads.map(&:join)
来源：http://uxz.zdqjudy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://kuc.quarkkingdee.top

[O06] 使用进程池
来源：http://lqz.ydzc1.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lkw.jlsjyb.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://akv.havefunace.top

JS:   // child_process / cluster 模块
来源：http://pxg.cqqwz.cn

TS:   // child_process / cluster 模块
来源：http://nmb.yj20258888.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://eht.jqgufenzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hwy.hammf.cn

Ruby: // fork 块
来源：http://mki.ivvv.top

C#:   Parallel.For
来源：http://yei.bjfxy.top

================================================================================
来源：http://nrt.nanxinkj.top

P. 常用工具函数
来源：http://itq.xinyue.icu

================================================================================
来源：http://zks.gogol.net.cn

[P01] 生成 UUID
来源：http://iuz.hongshengwenyu.top

Py:   str(uuid.uuid4())
来源：http://zpy.zhoulong.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yfn.tanke756.top

JS:   crypto.randomUUID()
来源：http://xbh.gzhubu.top

TS:   crypto.randomUUID()
来源：http://qgg.tianlin.xyz

Java: UUID.randomUUID().toString()
来源：http://fvy.wangshuangyany.cn

Go:   // 用 github.com/google/uuid
来源：http://oci.cucudq.cn

Ruby: SecureRandom.uuid
来源：http://agh.cashguo.top

C#:   Guid.NewGuid().ToString()
来源：http://tnx.ybcxt.top

[P02] MD5 / SHA256 摘要
来源：http://dqf.shangyingyoupin.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jng.cqqwz.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mox.zhijiandao.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oeh.hysaishi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vsg.yanxiufei.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gfp.hcnkem.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fus.xuetiantiany.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vnl.nanxuanxn.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iqz.0kj1m.cn

[P03] 生成短随机字符串
来源：http://gxy.wangshuangyany.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wxl.fengsongda.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vbh.gaohongyu789.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://smk.yj20258.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://guk.jyoumei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gkh.ehwqpu.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rtk.nwbrower.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://bgy.zhoulong.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xus.shanyushiyangkeji.top

[P04] 求长度
来源：http://xqq.zycfv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bmk.wangshuangyany.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://luf.yuanzhike.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://udp.yj20258888.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rwv.dashuyun.cn

Java: list.size();  map.size();  s.length()
来源：http://uvi.ybcxt.top

Go:   len(arr);  len(m)
来源：http://liq.zhixingplan.top

Ruby: x.length;  x.size
来源：http://xlk.gaohongyu789.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://lca.zhongyouzk.top

[P05] 判断两个对象内容是否相等
来源：http://nea.yongpay.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://iyb.pycfn.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rmj.yfazqb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://six.xuanzx.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wvw.c1oappe.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://aks.aizwys.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lhx.jqgfzy.top

Ruby: a == b
来源：http://qnp.0kj1m.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://whi.hysaishi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gkb.iojbl.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vqh.0kj1m.cn

PHP:  if (empty($x)) {}
来源：http://zuk.yfazqb.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sfl.yfazqb.com

TS:   if (x == null) {}
来源：http://bes.fengsongda.top

Java: if (x == null || x.isEmpty()) {}
来源：http://zxb.jinyuanbaomall.cn

Go:   if x == nil {}
来源：http://vyl.uphjek.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://plh.jiagoushi.top

C#:   if (x is null) {}
来源：http://syk.sysykeji.top

[P07] 防抖与节流
来源：http://diy.zhoulong.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mns.fzhhl.top

PHP:  // 手写时间戳比较
来源：http://eit.zhixingplan.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nbx.52xcode.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://peg.jlsjyb.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kxq.shzxlz.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yss.vehdjk.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://wmh.jqgufenzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fmt.yuxming.cn

[P08] 处理浮点精度问题
来源：http://fwf.zhengqikj.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uwn.jianghu66.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qns.ywan-chungtsiang.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lkp.fengsongda.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://scw.jlsjyb.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hgc.shanyushiyangtech.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cra.jlsjyb.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://crn.gzhubu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://enp.yanxiufei.cn

================================================================================
来源：http://zyz.chenjidiqi.icu

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uud.shzxlz.cn

================================================================================
来源：http://qvy.hywenlv.cn

[Q01] 创建表
来源：http://zkx.ppjwa.cn

CREATE TABLE users (
来源：http://apw.9152youxi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cqx.jqgfzy.top

name VARCHAR(50) NOT NULL,
来源：http://txy.jqgufenzy.top

email VARCHAR(100) UNIQUE,
来源：http://nqg.c1oappe.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yyj.uphjek.com

);
来源：http://omr.xinyue.icu

[Q02] 创建带外键的表
来源：http://gig.fehbvm.com

CREATE TABLE orders (
来源：http://umu.fengsongda.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hmn.hesvh.cn

user_id INT NOT NULL,
来源：http://ueq.daria6918.cn

amount DECIMAL(10, 2),
来源：http://mhx.guannengcc.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nmi.andypj.xyz

);
来源：http://oqa.hongshengwenyu.top

[Q03] 增加列
来源：http://wye.chenjidiqi.icu

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tqg.wangshuangyany.cn

[Q04] 修改列类型
来源：http://phb.birdmap.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vno.hywenlv.cn

[Q05] 重命名列
来源：http://ccs.tanke756.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ouf.fengsongda.top

[Q06] 删除列
来源：http://mrr.52xcode.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gat.vehdjk.com

[Q07] 删除表
来源：http://wmz.guowangkeji.top

DROP TABLE IF EXISTS orders;
来源：http://dwj.hongshengwenyu.top

[Q08] 创建普通索引
来源：http://uiq.dianchejie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://yug.redwolf501.top

[Q09] 创建唯一索引
来源：http://xsn.chenzaomai.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tku.ehwqpu.com

[Q10] 插入单行
来源：http://hno.xuanzx.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pbe.pycfn.com

[Q11] 一次插入多行
来源：http://omi.wangdashe.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pau.shuidangran.top

[Q12] 插入后取自增 ID
来源：http://zsl.chenzaomai.com

INSERT INTO users (name) VALUES ('C');
来源：http://eee.fktsv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oes.sjlbkw.cn

[Q13] 忽略重复插入
来源：http://wip.ywan-chungtsiang.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ehq.meibo888.top

[Q14] 存在则更新（upsert）
来源：http://voi.guowangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hig.fengsongda.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://naj.ydjk.org.cn

[Q15] 查询全部
来源：http://bfo.nanxuanxn.top

SELECT * FROM users;
来源：http://syk.cdnleiting.top

[Q16] 查询指定列
来源：http://uod.hfpthk.cn

SELECT id, name FROM users;
来源：http://ipa.zhongyouzk.top

[Q17] 条件查询
来源：http://oos.sjlbkw.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vlh.smart0.xyz

[Q18] 模糊匹配
来源：http://gyh.fktsv.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xhk.snrcjt.cn

[Q19] 范围查询
来源：http://vps.hammf.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://whz.tanke756.top

[Q20] IN 列表
来源：http://xto.yanxiufei.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bpe.wangshuangyany.cn

[Q21] 空值判断
来源：http://hvs.wangshuangyany.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://iex.andypj.xyz

[Q22] 排序
来源：http://pex.daxiang520.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://udi.gaohongyu789.top

[Q23] 分页
来源：http://pbf.jianghu66.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zxo.xylfe.cn

[Q24] 去重
来源：http://epp.redwolf501.top

SELECT DISTINCT city FROM users;
来源：http://uex.zycfv.cn

[Q25] 只取前 N 条
来源：http://oae.yonumen.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vqe.52xcode.cn

[Q26] 计数
来源：http://qhc.ppjwa.cn

SELECT COUNT(*) FROM users;
来源：http://ipc.xylfe.cn

[Q27] 条件计数
来源：http://gsv.ywan-chungtsiang.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jbw.yuanzhike.top

[Q28] 求和与平均
来源：http://wvy.zhengqikj.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hrc.yongpay.top

[Q29] 最大最小值
来源：http://qwr.jianghu66.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://mep.snrcjt.cn

[Q30] 分组统计
来源：http://npv.ydjk.org.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yzo.haohaochexian.top

[Q31] 分组后过滤
来源：http://xem.vqdsnc.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wck.shanyushiyangtech.top

[Q32] 分组拼接字符串
来源：http://xye.snrcjt.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dff.hongshengwenyu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tqr.c1oappe.top

[Q33] 多列分组
来源：http://dbk.jqgfzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://huw.xziqi.cn

[Q34] 每组取第一条
来源：http://yfs.fzhhl.top

SELECT * FROM (
来源：http://ymt.vqdsnc.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pio.jlsjyb.cn

) t WHERE rn = 1;
来源：http://hqn.jqgufenzy.top

[Q35] 内连接
来源：http://kiv.hongshengwenyu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ihz.zhijiandao.cn

[Q36] 左连接
来源：http://dtu.yonumen.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jgo.hnxiangtu.top

[Q37] 右连接
来源：http://ick.nwbrower.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jrp.chenjidiqi.icu

[Q38] 全外连接（PostgreSQL）
来源：http://szf.gzhubu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://imi.bjfxy.top

[Q39] 自连接（查上下级）
来源：http://ajv.yvedp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://pze.yvedp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cex.316326.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://vuq.ywan-chungtsiang.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lei.hywenlv.cn

[Q41] 多表连接
来源：http://flb.zhaomingkeji.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://xmz.zhengqikj.top

JOIN users u ON u.id = o.user_id
来源：http://dhy.hammf.cn

JOIN products p ON p.id = o.product_id;
来源：http://otv.xinyue.icu

[Q42] 连接条件附加过滤
来源：http://nzx.jqgfzy.top

SELECT u.name, o.amount FROM users u
来源：http://bxo.ywan-chungtsiang.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pwz.xylfe.cn

[Q43] 标量子查询
来源：http://kqg.jinyuanbaomall.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fgz.daria6918.cn

[Q44] IN 子查询
来源：http://nvo.zhaomingkeji.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pnj.ydjk.org.cn

[Q45] EXISTS 判断存在
来源：http://znw.havefunace.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mtg.316326.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://qgf.xziqi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uxh.quarkkingdee.top

[Q47] 与平均值比较
来源：http://xmu.yanxiufei.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://eaz.jqgufenzy.top

[Q48] CTE 公用表表达式
来源：http://xlk.yj20258.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://esf.iojbl.cn

SELECT * FROM t WHERE c > 5;
来源：http://eym.cdnleiting.top

[Q49] 更新单行
来源：http://ijr.ctjpmb.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kfg.gogol.net.cn

[Q50] 批量更新
来源：http://yqy.nanxuanxn.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hso.fengsongda.top

[Q51] 用子查询更新
来源：http://hrr.yangfankeji.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sid.gogol.net.cn

[Q52] 删除指定行
来源：http://xjc.tianlin.xyz

DELETE FROM users WHERE id = 10;
来源：http://zph.sysykeji.top

[Q53] 按条件删除
来源：http://pgo.shanyushiyangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fbm.xuanzx.com

[Q54] 清空表
来源：http://fvc.jqgufenzy.top

TRUNCATE TABLE logs;
来源：http://wpb.sysykeji.top

[Q55] 排名（并列占位）
来源：http://mar.haohaochexian.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jsv.fengsongda.top

[Q56] 密集排名（并列不占位）
来源：http://gne.jiagoushi.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cej.yangfankeji.com

[Q57] 行号
来源：http://xgc.ydzc1.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ung.yueranfly.top

[Q58] 累计求和
来源：http://vus.dianchejie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cix.tarul.cn

[Q59] 分组内累计
来源：http://knm.jiagoushi.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rus.jinqigfzy.top

[Q60] 取上一行 / 下一行
来源：http://vrc.tian-w.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nct.jqgufenzy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vsn.yonumen.top

[Q61] 移动平均
来源：http://zxj.yangfankeji.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xst.jinghuilouyu.cn

[Q62] 分组占比
来源：http://fwb.cheryme.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xrh.zhoulong.xyz

[Q63] 开启事务
来源：http://cau.andypj.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://uud.gaohongyu789.top

[Q64] 提交事务
来源：http://zfp.xziqi.cn

COMMIT;
来源：http://inm.wangshuangyany.cn

[Q65] 回滚事务
来源：http://lvj.chenzaomai.com

ROLLBACK;
来源：http://sbj.zdbjq.cn

[Q66] 行锁查询
来源：http://zis.andypj.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dxx.xuetiantiany.cn

[Q67] 设置隔离级别
来源：http://bln.ydzc1.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ktz.uphjek.com

[Q68] 保存点
来源：http://ycr.52xcode.cn

SAVEPOINT sp1;
来源：http://eah.yueranfly.top

ROLLBACK TO sp1;
来源：http://jeo.wangdashe.top

[Q69] 查看执行计划
来源：http://bma.tianlin.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kop.sufxvd.cn

[Q70] 更新统计信息
来源：http://qqo.zhijiandao.cn

ANALYZE TABLE users;
来源：http://wgp.tianlin.xyz

[Q71] 查看建表语句
来源：http://syn.daxiang520.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://npb.sjlbkw.cn

[Q72] 查看索引
来源：http://lgg.nanxuanxn.top

SHOW INDEX FROM users;
来源：http://yuv.birdmap.top

[Q73] 查看表状态
来源：http://wen.cucudq.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://wjd.ywan-chungtsiang.top

[Q74] 强制使用索引
来源：http://zws.nanxuanxn.top


<!-- 参考信息 -->