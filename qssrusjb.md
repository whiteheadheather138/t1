代发 wailian999

================================================================================
来源：http://cyf.sufxvd.cn

O. 并发与异步
来源：http://cnn.jianghu66.top

================================================================================
来源：http://pdq.birdmap.top

[O01] 启动一个线程
来源：http://mye.xingfuxueyuan.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hdo.uphjek.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mps.jianghu66.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vsu.nanxuanxn.top

TS:   // 同 JS
来源：http://dfg.jiagoushi.top

Java: new Thread(() -> f()).start()
来源：http://hmx.guannengcc.top

Go:   go f()
来源：http://ojr.ydzc1.top

Ruby: Thread.new { f }
来源：http://ewk.pengpengdd.cyou

C#:   Task.Run(() => F());
来源：http://xfu.epnwcf.com

[O02] 使用线程池
来源：http://qna.vehdjk.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://iaj.aibaodan.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uvo.hesvh.cn

JS:   // worker_threads 线程池
来源：http://cfl.yvedp.cn

TS:   // worker_threads 线程池
来源：http://egj.tianlin.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://nfy.ehwqpu.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ryi.fanxiaobao.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dqu.cucudq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dqx.kuanghao11.cn

[O03] 加锁保护共享数据
来源：http://tll.yj20258888.top

Py:   with lock: shared += 1
来源：http://qnf.cashguo.top

PHP:  // 用 flock() 做文件锁
来源：http://bls.9152youxi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hnm.fktsv.cn

TS:   // 同 JS
来源：http://phq.daria6918.cn

Java: synchronized (this) { shared++; }
来源：http://gto.chenlongwang.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://luk.chenjidiqi.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://ndd.xylfe.cn

C#:   lock (gate) { shared++; }
来源：http://gfx.svipenyu.cn

[O04] 定义异步函数并等待
来源：http://ulz.shanyushiyangtech.top

Py:   async def f():⏎    await g()
来源：http://ggh.wangshuangyany.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cjd.snrcjt.cn

JS:   async function f() { await g(); }
来源：http://dxw.yj20258888.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://znv.fanxiaobao.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nos.jyoumei.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://opc.shanyushiyangtech.top

Ruby: # 用 Fiber 或 async gem
来源：http://hvg.ydjk.org.cn

C#:   async Task F() { await G(); }
来源：http://eyl.cashguo.top

[O05] 并发执行并等待全部完成
来源：http://kbc.aibaodan.cn

Py:   asyncio.gather(*tasks)
来源：http://gnx.bjfxy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mne.sysykeji.top

JS:   await Promise.all(tasks)
来源：http://gss.nanxinkj.top

TS:   await Promise.all(tasks)
来源：http://srd.316326.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://poa.ppjwa.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wyf.aibaodan.cn

Ruby: threads.map(&:join)
来源：http://zku.yueranfly.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mgi.cheryme.top

[O06] 使用进程池
来源：http://bvh.jlsjyb.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tox.uphjek.com

PHP:  // pcntl_fork 或多进程队列
来源：http://sxi.jinghuilouyu.cn

JS:   // child_process / cluster 模块
来源：http://dtl.zhiwuduotai.top

TS:   // child_process / cluster 模块
来源：http://waw.zhiwuduotai.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ruc.jqgufenzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://exu.cheryme.top

Ruby: // fork 块
来源：http://vtv.xuetiantiany.cn

C#:   Parallel.For
来源：http://wpe.gogol.net.cn

================================================================================
来源：http://wng.tarul.cn

P. 常用工具函数
来源：http://rip.fengsongda.top

================================================================================
来源：http://dnb.hammf.cn

[P01] 生成 UUID
来源：http://blc.vehdjk.com

Py:   str(uuid.uuid4())
来源：http://zry.svipenyu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mqk.yueranfly.top

JS:   crypto.randomUUID()
来源：http://dke.jiagoushi.top

TS:   crypto.randomUUID()
来源：http://owz.svipenyu.cn

Java: UUID.randomUUID().toString()
来源：http://yfa.shangyingyoupin.top

Go:   // 用 github.com/google/uuid
来源：http://mhu.fzhhl.top

Ruby: SecureRandom.uuid
来源：http://sop.fengsongda.top

C#:   Guid.NewGuid().ToString()
来源：http://kzf.yuxming.cn

[P02] MD5 / SHA256 摘要
来源：http://gid.hywenlv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oid.pengpengdd.cyou

PHP:  hash("sha256", $s);  md5($s);
来源：http://lrl.jinqigfzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lmn.zhijiandao.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dno.hnxiangtu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gnl.fehbvm.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://avh.cqqwz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pib.jinghuilouyu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cam.yangfankeji.com

[P03] 生成短随机字符串
来源：http://kez.shuidangran.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gkz.shzxlz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vvr.fzhhl.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hji.nanxinkj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nxb.hcnkem.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hyl.zhijiandao.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xax.fzhhl.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://tiv.zycfv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://oad.sxryk.cn

[P04] 求长度
来源：http://nzc.fehbvm.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pxe.cheryme.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://inw.ehwqpu.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lch.fanxiaobao.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zxd.ctjpmb.com

Java: list.size();  map.size();  s.length()
来源：http://ugi.gogol.net.cn

Go:   len(arr);  len(m)
来源：http://qlq.shzxlz.cn

Ruby: x.length;  x.size
来源：http://gix.jinqigfzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ogb.jiagoushi.top

[P05] 判断两个对象内容是否相等
来源：http://yhb.hywenlv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qdw.cqqwz.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jub.jianghu66.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bog.haohaochexian.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ydh.zhaomingkeji.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kae.ctjpmb.com

Go:   reflect.DeepEqual(a, b)
来源：http://tgb.sjlbkw.cn

Ruby: a == b
来源：http://wzd.jiagoushi.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qtn.cucudq.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wpw.ppjwa.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tzj.yuanzhike.top

PHP:  if (empty($x)) {}
来源：http://mhp.wangdashe.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://efa.zdqjudy.top

TS:   if (x == null) {}
来源：http://ocr.jinqigfzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://aeh.xinyue.icu

Go:   if x == nil {}
来源：http://hac.9152youxi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gdd.yongpay.top

C#:   if (x is null) {}
来源：http://orm.quarkkingdee.top

[P07] 防抖与节流
来源：http://oel.pycfn.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rix.sweek.top

PHP:  // 手写时间戳比较
来源：http://qdj.yuanzhike.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://den.jqgfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bvf.andypj.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fln.chenlongwang.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hwx.gotoacloud.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://vqn.zhiwuduotai.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fkf.yvedp.cn

[P08] 处理浮点精度问题
来源：http://xkj.yvedp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bkd.cheryme.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ctn.hesvh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qsk.aizwys.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uqp.hywenlv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zfk.yfazqb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mrf.jqgufenzy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://otm.mhx1999.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mlm.jlsjyb.cn

================================================================================
来源：http://jir.fengsongda.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fvy.cashguo.top

================================================================================
来源：http://xld.nanxinkj.top

[Q01] 创建表
来源：http://uzz.hammf.cn

CREATE TABLE users (
来源：http://idh.zhaomingkeji.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qki.yj20258.top

name VARCHAR(50) NOT NULL,
来源：http://hzc.zhixingplan.top

email VARCHAR(100) UNIQUE,
来源：http://qea.chenjidiqi.icu

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nvn.ybcxt.top

);
来源：http://xge.jqgufenzy.top

[Q02] 创建带外键的表
来源：http://tsm.feifeiyinyue.top

CREATE TABLE orders (
来源：http://bho.nanxuanxn.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yvi.hysaishi.cn

user_id INT NOT NULL,
来源：http://pzf.yvedp.cn

amount DECIMAL(10, 2),
来源：http://sho.yfazqb.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kgz.yj20258.top

);
来源：http://tqz.ybcxt.top

[Q03] 增加列
来源：http://pue.gzhubu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vqs.ivvv.top

[Q04] 修改列类型
来源：http://blo.ydjk.org.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bnw.gogol.net.cn

[Q05] 重命名列
来源：http://cbr.daria6918.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://clm.gogol.net.cn

[Q06] 删除列
来源：http://vox.guowangkeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://aqt.ppjwa.cn

[Q07] 删除表
来源：http://htd.vehdjk.com

DROP TABLE IF EXISTS orders;
来源：http://fur.hesvh.cn

[Q08] 创建普通索引
来源：http://hlz.ehwqpu.com

CREATE INDEX idx_users_email ON users(email);
来源：http://pye.guowangkeji.top

[Q09] 创建唯一索引
来源：http://ten.pycfn.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cjg.yanxiufei.cn

[Q10] 插入单行
来源：http://gka.gaohongyu789.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rjg.yj202588.top

[Q11] 一次插入多行
来源：http://xtq.zhixingplan.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://brt.zdbjq.cn

[Q12] 插入后取自增 ID
来源：http://doy.jqgfzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://hsz.cdnleiting.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jct.zdqjudy.top

[Q13] 忽略重复插入
来源：http://loc.chenjidiqi.icu

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fzj.fktsv.cn

[Q14] 存在则更新（upsert）
来源：http://tqd.nanxinkj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vja.pycfn.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gum.yj20258888.top

[Q15] 查询全部
来源：http://pey.daxiang520.top

SELECT * FROM users;
来源：http://ewx.aizwys.cn

[Q16] 查询指定列
来源：http://dni.cucudq.cn

SELECT id, name FROM users;
来源：http://uif.vqdsnc.cn

[Q17] 条件查询
来源：http://gob.uphjek.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rvh.cashguo.top

[Q18] 模糊匹配
来源：http://bdz.yuxming.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qoy.316326.xyz

[Q19] 范围查询
来源：http://ogu.jinghuilouyu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xjo.sufxvd.cn

[Q20] IN 列表
来源：http://vmv.xingfuxueyuan.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oam.xuetiantiany.cn

[Q21] 空值判断
来源：http://ojz.ydjk.org.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zdz.chenzaomai.com

[Q22] 排序
来源：http://kja.tianlin.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://spa.jianghu66.top

[Q23] 分页
来源：http://bbe.xuetiantiany.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mcu.ivvv.top

[Q24] 去重
来源：http://saf.iojbl.cn

SELECT DISTINCT city FROM users;
来源：http://xpa.tarul.cn

[Q25] 只取前 N 条
来源：http://xcw.zhijiandao.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wsl.zhoulong.xyz

[Q26] 计数
来源：http://tip.fehbvm.com

SELECT COUNT(*) FROM users;
来源：http://ysv.gaohongyu789.top

[Q27] 条件计数
来源：http://bry.yuanzhike.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sis.jianghu66.top

[Q28] 求和与平均
来源：http://mlv.jinyuanbaomall.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://atz.gotoacloud.top

[Q29] 最大最小值
来源：http://grh.fehbvm.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://kfh.316326.xyz

[Q30] 分组统计
来源：http://bau.jianghu66.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ryy.zhaomingkeji.xyz

[Q31] 分组后过滤
来源：http://azi.pengpengdd.cyou

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fvn.cqqwz.cn

[Q32] 分组拼接字符串
来源：http://wul.cdnleiting.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tls.hnqzz.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qgy.guowangkeji.top

[Q33] 多列分组
来源：http://hev.svipenyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://org.hfpthk.cn

[Q34] 每组取第一条
来源：http://xai.shanyushiyangkeji.top

SELECT * FROM (
来源：http://iuq.yangfankeji.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://udx.shanyushiyangtech.top

) t WHERE rn = 1;
来源：http://jwq.9152youxi.cn

[Q35] 内连接
来源：http://hzk.xylfe.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vsa.gzhubu.top

[Q36] 左连接
来源：http://eqk.bbcook.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cmg.pengpengdd.cyou

[Q37] 右连接
来源：http://cik.jyoumei.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jwd.yj202588.top

[Q38] 全外连接（PostgreSQL）
来源：http://pkg.yj20258888.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rnw.jiagoushi.top

[Q39] 自连接（查上下级）
来源：http://csp.birdmap.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://qrs.shzxlz.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oig.hammf.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://guu.hfpthk.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nvt.sweek.top

[Q41] 多表连接
来源：http://qfr.wangshuangyany.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://btr.nanxuanxn.top

JOIN users u ON u.id = o.user_id
来源：http://mpk.iojbl.cn

JOIN products p ON p.id = o.product_id;
来源：http://xxr.yvedp.cn

[Q42] 连接条件附加过滤
来源：http://eih.kuanghao11.cn

SELECT u.name, o.amount FROM users u
来源：http://hdh.gzhubu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://smc.vqdsnc.cn

[Q43] 标量子查询
来源：http://snl.ydjk.org.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rur.bbcook.cn

[Q44] IN 子查询
来源：http://rrc.yanxiufei.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nkm.cqqwz.cn

[Q45] EXISTS 判断存在
来源：http://ord.daxiang520.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hps.jqgfzy.top

[Q46] NOT EXISTS 判断不存在
来源：http://dgt.gotoacloud.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hyk.fktsv.cn

[Q47] 与平均值比较
来源：http://pfm.yuxming.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://asc.hcnkem.com

[Q48] CTE 公用表表达式
来源：http://pfy.yueranfly.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ypr.mhx1999.top

SELECT * FROM t WHERE c > 5;
来源：http://pos.yangfankeji.com

[Q49] 更新单行
来源：http://ghc.svipenyu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ltd.jinqigfzy.top

[Q50] 批量更新
来源：http://unk.svipenyu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rfm.yanxiufei.cn

[Q51] 用子查询更新
来源：http://txk.havefunace.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://aaa.xuetiantiany.cn

[Q52] 删除指定行
来源：http://smq.yj20258888.top

DELETE FROM users WHERE id = 10;
来源：http://vki.guannengcc.top

[Q53] 按条件删除
来源：http://uge.aizwys.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kso.0kj1m.cn

[Q54] 清空表
来源：http://izi.feifeiyinyue.top

TRUNCATE TABLE logs;
来源：http://dcb.feifeiyinyue.top

[Q55] 排名（并列占位）
来源：http://iob.chenzaomai.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://obl.tianlin.xyz

[Q56] 密集排名（并列不占位）
来源：http://cft.haohaochexian.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xra.ehwqpu.com

[Q57] 行号
来源：http://bxc.xinyue.icu

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kft.shangyingyoupin.top

[Q58] 累计求和
来源：http://euw.kuanghao11.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tba.yj20258888.top

[Q59] 分组内累计
来源：http://wql.mhx1999.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ltn.nanxinkj.top

[Q60] 取上一行 / 下一行
来源：http://wum.fengsongda.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bew.fehbvm.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wgs.ydzc1.top

[Q61] 移动平均
来源：http://unw.cucudq.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ioj.xinyue.icu

[Q62] 分组占比
来源：http://ugq.hnxiangtu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tyx.0kj1m.cn

[Q63] 开启事务
来源：http://deg.fktsv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://blf.jinghuilouyu.cn

[Q64] 提交事务
来源：http://izu.tanke756.top

COMMIT;
来源：http://euk.jinqigufen.top

[Q65] 回滚事务
来源：http://uir.ybcxt.top

ROLLBACK;
来源：http://jmz.aibaodan.cn

[Q66] 行锁查询
来源：http://urr.shzxlz.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tcz.dianchejie.cn

[Q67] 设置隔离级别
来源：http://ipw.zhongyouzk.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qnd.jinghuilouyu.cn

[Q68] 保存点
来源：http://ngt.tarul.cn

SAVEPOINT sp1;
来源：http://mvy.xuanzx.com

ROLLBACK TO sp1;
来源：http://wyv.smart0.xyz

[Q69] 查看执行计划
来源：http://jsr.52xcode.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ltt.hysaishi.cn

[Q70] 更新统计信息
来源：http://acy.svipenyu.cn

ANALYZE TABLE users;
来源：http://djs.pycfn.com

[Q71] 查看建表语句
来源：http://lzq.ctjpmb.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zkw.ydzc1.top

[Q72] 查看索引
来源：http://rez.dashuyun.cn


<!-- 参考信息 -->