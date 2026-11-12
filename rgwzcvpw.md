代发 wailian999

================================================================================
来源：http://hwh.feifeiyinyue.top

O. 并发与异步
来源：http://aov.wangdashe.top

================================================================================
来源：http://snx.hesvh.cn

[O01] 启动一个线程
来源：http://jmg.zhongyouzk.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rjs.nanxuanxn.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bvt.yvedp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fdn.vqdsnc.cn

TS:   // 同 JS
来源：http://wcl.yj202588.top

Java: new Thread(() -> f()).start()
来源：http://esm.guowangkeji.top

Go:   go f()
来源：http://nuf.quarkkingdee.top

Ruby: Thread.new { f }
来源：http://tzc.guannengcc.top

C#:   Task.Run(() => F());
来源：http://fbz.0kj1m.cn

[O02] 使用线程池
来源：http://ler.yangfankeji.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://log.jlsjyb.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zqu.sufxvd.cn

JS:   // worker_threads 线程池
来源：http://seh.zdqjudy.top

TS:   // worker_threads 线程池
来源：http://hjm.jiagoushi.top

Java: Executors.newFixedThreadPool(4)
来源：http://lnp.fktsv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fif.zhongyouzk.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rag.yangfankeji.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bim.cqqwz.cn

[O03] 加锁保护共享数据
来源：http://gux.yuxming.cn

Py:   with lock: shared += 1
来源：http://wlm.cheryme.top

PHP:  // 用 flock() 做文件锁
来源：http://ghf.yongpay.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uqe.ybcxt.top

TS:   // 同 JS
来源：http://yyv.cucudq.cn

Java: synchronized (this) { shared++; }
来源：http://owp.jlsjyb.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jyd.fktsv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://nxz.sufxvd.cn

C#:   lock (gate) { shared++; }
来源：http://vic.haohaochexian.top

[O04] 定义异步函数并等待
来源：http://eog.zhijiandao.cn

Py:   async def f():⏎    await g()
来源：http://hgf.yonumen.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gux.feifeiyinyue.top

JS:   async function f() { await g(); }
来源：http://dmk.nanxinkj.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://kty.feifeiyinyue.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kyy.cdnleiting.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vlt.zdbjq.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ryz.haohaochexian.top

C#:   async Task F() { await G(); }
来源：http://llk.svipenyu.cn

[O05] 并发执行并等待全部完成
来源：http://fzy.zhijiandao.cn

Py:   asyncio.gather(*tasks)
来源：http://ppi.tianlin.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gto.uphjek.com

JS:   await Promise.all(tasks)
来源：http://esq.pycfn.com

TS:   await Promise.all(tasks)
来源：http://yzx.tianlin.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://god.ydjk.org.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wgd.yangfankeji.com

Ruby: threads.map(&:join)
来源：http://wbp.andypj.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://ryk.yueranfly.top

[O06] 使用进程池
来源：http://bmr.birdmap.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://apm.smart0.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://tmd.shanyushiyangkeji.top

JS:   // child_process / cluster 模块
来源：http://jtq.xuetiantiany.cn

TS:   // child_process / cluster 模块
来源：http://oge.jiagoushi.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rce.hcnkem.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mwj.yj202588.top

Ruby: // fork 块
来源：http://fyw.hcnkem.com

C#:   Parallel.For
来源：http://gdc.andypj.xyz

================================================================================
来源：http://ysn.hywenlv.cn

P. 常用工具函数
来源：http://qct.fktsv.cn

================================================================================
来源：http://htq.chenzaomai.com

[P01] 生成 UUID
来源：http://dxb.zhixingplan.top

Py:   str(uuid.uuid4())
来源：http://llq.fktsv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://omt.gogol.net.cn

JS:   crypto.randomUUID()
来源：http://hoz.ybcxt.top

TS:   crypto.randomUUID()
来源：http://fxh.yfazqb.com

Java: UUID.randomUUID().toString()
来源：http://xcv.quarkkingdee.top

Go:   // 用 github.com/google/uuid
来源：http://xmq.jinghuilouyu.cn

Ruby: SecureRandom.uuid
来源：http://uqa.zhaomingkeji.xyz

C#:   Guid.NewGuid().ToString()
来源：http://zci.zdbjq.cn

[P02] MD5 / SHA256 摘要
来源：http://cin.yvedp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sra.yonumen.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wzt.xuanzx.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lai.9152youxi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ovj.xuanzx.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lye.tarul.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ncz.fzhhl.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hrj.zhongyouzk.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hts.jqgfzy.top

[P03] 生成短随机字符串
来源：http://afs.aizwys.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://asp.ydzc1.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hec.redwolf501.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kkh.tianlin.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dno.jinghuilouyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lel.cqqwz.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sqb.sysykeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://bze.0kj1m.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lyq.mhx1999.top

[P04] 求长度
来源：http://iht.zhijiandao.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wil.dianchejie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ugj.hfpthk.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://heo.xinyue.icu

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wna.wangshuangyany.cn

Java: list.size();  map.size();  s.length()
来源：http://yns.xinyue.icu

Go:   len(arr);  len(m)
来源：http://pzi.aizwys.cn

Ruby: x.length;  x.size
来源：http://krh.yfazqb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://iua.pycfn.com

[P05] 判断两个对象内容是否相等
来源：http://ckz.xingfuxueyuan.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://hkv.gzhubu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bnh.ywan-chungtsiang.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zls.hfpthk.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qte.chenjidiqi.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bpk.yonumen.top

Go:   reflect.DeepEqual(a, b)
来源：http://lxj.fanxiaobao.xyz

Ruby: a == b
来源：http://rul.bbcook.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://oep.tianlin.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://udc.jinghuilouyu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sxg.gogol.net.cn

PHP:  if (empty($x)) {}
来源：http://srd.ydzc1.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pqe.meibo888.top

TS:   if (x == null) {}
来源：http://qfg.snrcjt.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bnb.feifeiyinyue.top

Go:   if x == nil {}
来源：http://von.9152youxi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xfk.haohaochexian.top

C#:   if (x is null) {}
来源：http://qcx.fanxiaobao.xyz

[P07] 防抖与节流
来源：http://cqm.aizwys.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ayn.yanxiufei.cn

PHP:  // 手写时间戳比较
来源：http://ycu.jiagoushi.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://str.ppjwa.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tfi.yvedp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ryn.wangdashe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kit.hongshengwenyu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://gkd.hysaishi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://skx.bjfxy.top

[P08] 处理浮点精度问题
来源：http://vxu.daria6918.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ast.9152youxi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://obs.chenzaomai.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sov.zhoulong.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://myw.xziqi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://air.shangyingyoupin.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ydq.bbcook.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mco.sweek.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gbi.jyoumei.cn

================================================================================
来源：http://ckb.jianghu66.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://iwu.hnxiangtu.top

================================================================================
来源：http://rbq.vqdsnc.cn

[Q01] 创建表
来源：http://bgs.yj20258.top

CREATE TABLE users (
来源：http://sam.chenjidiqi.icu

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xbw.fzhhl.top

name VARCHAR(50) NOT NULL,
来源：http://ngs.sufxvd.cn

email VARCHAR(100) UNIQUE,
来源：http://ujj.ydzc1.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://aco.birdmap.top

);
来源：http://ibi.andypj.xyz

[Q02] 创建带外键的表
来源：http://qxg.jinghuilouyu.cn

CREATE TABLE orders (
来源：http://obr.yanxiufei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tyl.ywan-chungtsiang.top

user_id INT NOT NULL,
来源：http://ggf.sweek.top

amount DECIMAL(10, 2),
来源：http://hyj.shuidangran.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vxb.yongpay.top

);
来源：http://xow.sufxvd.cn

[Q03] 增加列
来源：http://fhs.redwolf501.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vks.dashuyun.cn

[Q04] 修改列类型
来源：http://oeb.shzxlz.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://iyj.yongpay.top

[Q05] 重命名列
来源：http://wzv.hywenlv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mvd.yonumen.top

[Q06] 删除列
来源：http://jcl.birdmap.top

ALTER TABLE users DROP COLUMN age;
来源：http://zho.hnqzz.top

[Q07] 删除表
来源：http://tza.fktsv.cn

DROP TABLE IF EXISTS orders;
来源：http://odn.fehbvm.com

[Q08] 创建普通索引
来源：http://oee.sjlbkw.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jjz.jinqigufen.top

[Q09] 创建唯一索引
来源：http://zlk.0kj1m.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://onx.hongshengwenyu.top

[Q10] 插入单行
来源：http://zgj.cheryme.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zfu.yangfankeji.com

[Q11] 一次插入多行
来源：http://txn.jinyuanbaomall.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://djh.hywenlv.cn

[Q12] 插入后取自增 ID
来源：http://zds.vqdsnc.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rod.chenjidiqi.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vwt.wangdashe.top

[Q13] 忽略重复插入
来源：http://mfv.xingfuxueyuan.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jsq.feifeiyinyue.top

[Q14] 存在则更新（upsert）
来源：http://gch.9152youxi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://daj.cheryme.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ysl.andypj.xyz

[Q15] 查询全部
来源：http://gbq.zhijiandao.cn

SELECT * FROM users;
来源：http://pvr.yuanzhike.top

[Q16] 查询指定列
来源：http://nyz.jiagoushi.top

SELECT id, name FROM users;
来源：http://glk.aibaodan.cn

[Q17] 条件查询
来源：http://zga.zhijiandao.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://znd.cheryme.top

[Q18] 模糊匹配
来源：http://uyu.daria6918.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sqz.aibaodan.cn

[Q19] 范围查询
来源：http://jvd.fengsongda.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fkv.hongshengwenyu.top

[Q20] IN 列表
来源：http://czq.nwbrower.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://eij.bjfxy.top

[Q21] 空值判断
来源：http://bon.xuetiantiany.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://heq.hfpthk.cn

[Q22] 排序
来源：http://nop.tian-w.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yab.hammf.cn

[Q23] 分页
来源：http://rxt.zhaomingkeji.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nbj.sxryk.cn

[Q24] 去重
来源：http://eov.yueranfly.top

SELECT DISTINCT city FROM users;
来源：http://hom.shuidangran.top

[Q25] 只取前 N 条
来源：http://bmg.chenzaomai.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pwn.yanxiufei.cn

[Q26] 计数
来源：http://bzx.sysykeji.top

SELECT COUNT(*) FROM users;
来源：http://hwb.snrcjt.cn

[Q27] 条件计数
来源：http://uru.c1oappe.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dur.meibo888.top

[Q28] 求和与平均
来源：http://lxo.tianlin.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zih.yueranfly.top

[Q29] 最大最小值
来源：http://dyh.zhixingplan.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jey.sjlbkw.cn

[Q30] 分组统计
来源：http://zvm.yueranfly.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vvh.0kj1m.cn

[Q31] 分组后过滤
来源：http://vsn.redwolf501.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xfb.zdbjq.cn

[Q32] 分组拼接字符串
来源：http://huz.zhoulong.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xya.xingfuxueyuan.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tmv.snrcjt.cn

[Q33] 多列分组
来源：http://dqo.mhx1999.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ssk.ehwqpu.com

[Q34] 每组取第一条
来源：http://udf.316326.xyz

SELECT * FROM (
来源：http://zvo.hammf.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zdo.hfpthk.cn

) t WHERE rn = 1;
来源：http://uua.0kj1m.cn

[Q35] 内连接
来源：http://cmg.sweek.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://odv.birdmap.top

[Q36] 左连接
来源：http://bkc.yuanzhike.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://toc.zdbjq.cn

[Q37] 右连接
来源：http://yvp.vehdjk.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rho.aibaodan.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wtx.hongshengwenyu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://nbh.zdqjudy.top

[Q39] 自连接（查上下级）
来源：http://ruk.meibo888.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://yzx.yj20258888.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tqb.fzhhl.top

[Q40] 交叉连接（笛卡尔积）
来源：http://nfk.cheryme.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zob.chenjidiqi.icu

[Q41] 多表连接
来源：http://nkl.epnwcf.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://boy.hcnkem.com

JOIN users u ON u.id = o.user_id
来源：http://bke.sufxvd.cn

JOIN products p ON p.id = o.product_id;
来源：http://mkc.nwbrower.top

[Q42] 连接条件附加过滤
来源：http://nkk.zdqjudy.top

SELECT u.name, o.amount FROM users u
来源：http://afd.52xcode.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cxk.zhaomingkeji.xyz

[Q43] 标量子查询
来源：http://alz.shanyushiyangkeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wlk.xuanzx.com

[Q44] IN 子查询
来源：http://yif.jyoumei.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qvg.ybcxt.top

[Q45] EXISTS 判断存在
来源：http://dso.ydzc1.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jvx.tanke756.top

[Q46] NOT EXISTS 判断不存在
来源：http://asd.haohaochexian.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://onm.zhijiandao.cn

[Q47] 与平均值比较
来源：http://dlo.cashguo.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qyb.yongpay.top

[Q48] CTE 公用表表达式
来源：http://tdt.cashguo.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tnn.jlsjyb.cn

SELECT * FROM t WHERE c > 5;
来源：http://yse.zhaomingkeji.xyz

[Q49] 更新单行
来源：http://tvd.dianchejie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://iwc.hongshengwenyu.top

[Q50] 批量更新
来源：http://jnz.cucudq.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jna.quarkkingdee.top

[Q51] 用子查询更新
来源：http://ogt.jqgfzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ijo.c1oappe.top

[Q52] 删除指定行
来源：http://puj.dashuyun.cn

DELETE FROM users WHERE id = 10;
来源：http://qbj.iojbl.cn

[Q53] 按条件删除
来源：http://jur.xylfe.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xcs.zdqjudy.top

[Q54] 清空表
来源：http://xwe.c1oappe.top

TRUNCATE TABLE logs;
来源：http://uar.yfazqb.com

[Q55] 排名（并列占位）
来源：http://mbm.dashuyun.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://esd.wangdashe.top

[Q56] 密集排名（并列不占位）
来源：http://wrs.c1oappe.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mdg.mhx1999.top

[Q57] 行号
来源：http://uyw.sweek.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cap.jinqigfzy.top

[Q58] 累计求和
来源：http://kow.hnxiangtu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dhl.shanyushiyangtech.top

[Q59] 分组内累计
来源：http://bcn.bbcook.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xmo.yueranfly.top

[Q60] 取上一行 / 下一行
来源：http://ivu.yangfankeji.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://suo.zhiwuduotai.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qow.feifeiyinyue.top

[Q61] 移动平均
来源：http://zje.wangdashe.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kld.nanxuanxn.top

[Q62] 分组占比
来源：http://lnq.gzhubu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zth.wangdashe.top

[Q63] 开启事务
来源：http://tqn.vehdjk.com

START TRANSACTION;                -- 或 BEGIN
来源：http://wva.c1oappe.top

[Q64] 提交事务
来源：http://axy.kuanghao11.cn

COMMIT;
来源：http://jvy.yanxiufei.cn

[Q65] 回滚事务
来源：http://fle.wangshuangyany.cn

ROLLBACK;
来源：http://ory.epnwcf.com

[Q66] 行锁查询
来源：http://qjj.guannengcc.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fuw.jinyuanbaomall.cn

[Q67] 设置隔离级别
来源：http://tdf.pycfn.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tlh.yuxming.cn

[Q68] 保存点
来源：http://rgy.gzhubu.top

SAVEPOINT sp1;
来源：http://dco.chenlongwang.top

ROLLBACK TO sp1;
来源：http://rro.zhijiandao.cn

[Q69] 查看执行计划
来源：http://abv.c1oappe.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://coz.yangfankeji.com

[Q70] 更新统计信息
来源：http://jms.zhongyouzk.top

ANALYZE TABLE users;
来源：http://etj.jlsjyb.cn

[Q71] 查看建表语句
来源：http://msy.tianlin.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://paw.hongshengwenyu.top

[Q72] 查看索引
来源：http://mxs.havefunace.top


<!-- 参考信息 -->