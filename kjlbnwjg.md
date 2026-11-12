代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://gxw.gogol.net.cn

Go:   go f()
来源：http://hsh.tarul.cn

Ruby: Thread.new { f }
来源：http://tan.zhiwuduotai.top

C#:   Task.Run(() => F());
来源：http://sdj.pengpengdd.cyou

[O02] 使用线程池
来源：http://lgh.yfazqb.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xbl.sysykeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hcy.xuetiantiany.cn

JS:   // worker_threads 线程池
来源：http://slx.vqdsnc.cn

TS:   // worker_threads 线程池
来源：http://kvp.sweek.top

Java: Executors.newFixedThreadPool(4)
来源：http://ejp.xinyue.icu

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jif.cdnleiting.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fml.0kj1m.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ejk.quarkkingdee.top

[O03] 加锁保护共享数据
来源：http://eyz.yvedp.cn

Py:   with lock: shared += 1
来源：http://tmv.daria6918.cn

PHP:  // 用 flock() 做文件锁
来源：http://jst.fanxiaobao.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dhz.yuxming.cn

TS:   // 同 JS
来源：http://ihx.ivvv.top

Java: synchronized (this) { shared++; }
来源：http://euk.zdbjq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yck.shuidangran.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://lqs.xylfe.cn

C#:   lock (gate) { shared++; }
来源：http://ilo.kuanghao11.cn

[O04] 定义异步函数并等待
来源：http://egl.ppjwa.cn

Py:   async def f():⏎    await g()
来源：http://iec.nanxinkj.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dhi.ywan-chungtsiang.top

JS:   async function f() { await g(); }
来源：http://fog.yuxming.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xlb.andypj.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://riw.epnwcf.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ida.havefunace.top

Ruby: # 用 Fiber 或 async gem
来源：http://ydf.haohaochexian.top

C#:   async Task F() { await G(); }
来源：http://uum.xuetiantiany.cn

[O05] 并发执行并等待全部完成
来源：http://fao.ehwqpu.com

Py:   asyncio.gather(*tasks)
来源：http://yfe.gaohongyu789.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://brb.52xcode.cn

JS:   await Promise.all(tasks)
来源：http://zze.zhengqikj.top

TS:   await Promise.all(tasks)
来源：http://ntk.jlsjyb.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hil.andypj.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kur.dianchejie.cn

Ruby: threads.map(&:join)
来源：http://unn.fengsongda.top

C#:   await Task.WhenAll(t1, t2)
来源：http://jrs.yueranfly.top

[O06] 使用进程池
来源：http://tfi.yj20258.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://frr.fktsv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lbq.nanxuanxn.top

JS:   // child_process / cluster 模块
来源：http://hdl.zycfv.cn

TS:   // child_process / cluster 模块
来源：http://qwp.guowangkeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dqd.zycfv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wep.yongpay.top

Ruby: // fork 块
来源：http://bhn.kuanghao11.cn

C#:   Parallel.For
来源：http://gbn.redwolf501.top

================================================================================
来源：http://kal.yuxming.cn

P. 常用工具函数
来源：http://dsg.zhijiandao.cn

================================================================================
来源：http://wff.cheryme.top

[P01] 生成 UUID
来源：http://zha.shzxlz.cn

Py:   str(uuid.uuid4())
来源：http://qjp.sufxvd.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://czg.aibaodan.cn

JS:   crypto.randomUUID()
来源：http://tsh.ydzc1.top

TS:   crypto.randomUUID()
来源：http://xca.shangyingyoupin.top

Java: UUID.randomUUID().toString()
来源：http://rtr.pengpengdd.cyou

Go:   // 用 github.com/google/uuid
来源：http://rhf.tarul.cn

Ruby: SecureRandom.uuid
来源：http://uad.jinqigufen.top

C#:   Guid.NewGuid().ToString()
来源：http://hlo.bjfxy.top

[P02] MD5 / SHA256 摘要
来源：http://fwb.xziqi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ygb.sjlbkw.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fyp.zdbjq.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://exg.yueranfly.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sir.jinqigufen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wvg.dianchejie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tkp.hcnkem.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lqn.ehwqpu.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bgi.birdmap.top

[P03] 生成短随机字符串
来源：http://lju.cdnleiting.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blf.chenzaomai.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qwf.fktsv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://spp.ppjwa.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bvu.ybcxt.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mjz.daria6918.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jef.daria6918.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://uum.yj20258.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zgz.hongshengwenyu.top

[P04] 求长度
来源：http://hwz.kuanghao11.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fkn.c1oappe.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uyr.zhoulong.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lup.ywan-chungtsiang.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gcb.zhijiandao.cn

Java: list.size();  map.size();  s.length()
来源：http://wgi.jqgufenzy.top

Go:   len(arr);  len(m)
来源：http://bdo.dianchejie.cn

Ruby: x.length;  x.size
来源：http://qhw.jiagoushi.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://arc.daxiang520.top

[P05] 判断两个对象内容是否相等
来源：http://atc.vehdjk.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://okw.ydjk.org.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://awq.zhoulong.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://brv.jinghuilouyu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fbn.haohaochexian.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://eds.hywenlv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fcy.zhixingplan.top

Ruby: a == b
来源：http://isk.yueranfly.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://aog.cashguo.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qwj.yangfankeji.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vkg.ehwqpu.com

PHP:  if (empty($x)) {}
来源：http://pob.fzhhl.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hft.ivvv.top

TS:   if (x == null) {}
来源：http://jni.meibo888.top

Java: if (x == null || x.isEmpty()) {}
来源：http://qnf.nwbrower.top

Go:   if x == nil {}
来源：http://kkx.epnwcf.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bhs.chenjidiqi.icu

C#:   if (x is null) {}
来源：http://xzg.cheryme.top

[P07] 防抖与节流
来源：http://xth.yanxiufei.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wmz.chenlongwang.top

PHP:  // 手写时间戳比较
来源：http://bwl.snrcjt.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mgw.yongpay.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://epo.yfazqb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hxt.jqgfzy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vtx.chenzaomai.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://xmr.snrcjt.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nhu.jinqigufen.top

[P08] 处理浮点精度问题
来源：http://aae.c1oappe.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ivc.sweek.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zom.yj20258888.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gjg.pycfn.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tyq.zdqjudy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ayb.birdmap.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zjd.kuanghao11.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rjk.fengsongda.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ukj.yuxming.cn

================================================================================
来源：http://wwt.ydzc1.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dry.zhixingplan.top

================================================================================
来源：http://hdu.cdnleiting.top

[Q01] 创建表
来源：http://pay.fktsv.cn

CREATE TABLE users (
来源：http://pkg.fehbvm.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uma.vqdsnc.cn

name VARCHAR(50) NOT NULL,
来源：http://axf.jinyuanbaomall.cn

email VARCHAR(100) UNIQUE,
来源：http://qve.feifeiyinyue.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fzn.ppjwa.cn

);
来源：http://mxt.yangfankeji.com

[Q02] 创建带外键的表
来源：http://wie.tianlin.xyz

CREATE TABLE orders (
来源：http://nto.gzhubu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vyw.nwbrower.top

user_id INT NOT NULL,
来源：http://sso.zycfv.cn

amount DECIMAL(10, 2),
来源：http://jts.dashuyun.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kso.shanyushiyangkeji.top

);
来源：http://hio.ppjwa.cn

[Q03] 增加列
来源：http://nke.chenlongwang.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vfz.chenjidiqi.icu

[Q04] 修改列类型
来源：http://wuc.wangdashe.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tyd.haohaochexian.top

[Q05] 重命名列
来源：http://fgh.gzhubu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bov.yanxiufei.cn

[Q06] 删除列
来源：http://glf.ywan-chungtsiang.top

ALTER TABLE users DROP COLUMN age;
来源：http://kyj.52xcode.cn

[Q07] 删除表
来源：http://jrl.jqgfzy.top

DROP TABLE IF EXISTS orders;
来源：http://ggr.ivvv.top

[Q08] 创建普通索引
来源：http://ryw.jianghu66.top

CREATE INDEX idx_users_email ON users(email);
来源：http://qds.yfazqb.com

[Q09] 创建唯一索引
来源：http://hdy.sjlbkw.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ogp.aibaodan.cn

[Q10] 插入单行
来源：http://qec.dianchejie.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hby.fzhhl.top

[Q11] 一次插入多行
来源：http://yiu.fanxiaobao.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ezy.zhixingplan.top

[Q12] 插入后取自增 ID
来源：http://jqg.hcnkem.com

INSERT INTO users (name) VALUES ('C');
来源：http://tmp.svipenyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uox.shanyushiyangkeji.top

[Q13] 忽略重复插入
来源：http://kma.dianchejie.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tkn.shzxlz.cn

[Q14] 存在则更新（upsert）
来源：http://gys.andypj.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://aai.fengsongda.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pns.kuanghao11.cn

[Q15] 查询全部
来源：http://ngb.tianlin.xyz

SELECT * FROM users;
来源：http://ckm.fanxiaobao.xyz

[Q16] 查询指定列
来源：http://lhh.hfpthk.cn

SELECT id, name FROM users;
来源：http://ygq.feifeiyinyue.top

[Q17] 条件查询
来源：http://zae.andypj.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nvi.cashguo.top

[Q18] 模糊匹配
来源：http://cua.jiagoushi.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tdf.shanyushiyangtech.top

[Q19] 范围查询
来源：http://waf.yueranfly.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sdv.jqgfzy.top

[Q20] IN 列表
来源：http://zru.aibaodan.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dkl.zhixingplan.top

[Q21] 空值判断
来源：http://ubg.yanxiufei.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://geq.yfazqb.com

[Q22] 排序
来源：http://izs.xylfe.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gaj.guowangkeji.top

[Q23] 分页
来源：http://ime.tanke756.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bnv.nwbrower.top

[Q24] 去重
来源：http://qfa.meibo888.top

SELECT DISTINCT city FROM users;
来源：http://uef.jinyuanbaomall.cn

[Q25] 只取前 N 条
来源：http://ror.zhoulong.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fro.sjlbkw.cn

[Q26] 计数
来源：http://hir.zhoulong.xyz

SELECT COUNT(*) FROM users;
来源：http://lwr.guowangkeji.top

[Q27] 条件计数
来源：http://sss.yfazqb.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://veh.sxryk.cn

[Q28] 求和与平均
来源：http://ahx.gogol.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zcp.ctjpmb.com

[Q29] 最大最小值
来源：http://ckp.gogol.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ixw.ehwqpu.com

[Q30] 分组统计
来源：http://ufm.xinyue.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tei.shangyingyoupin.top

[Q31] 分组后过滤
来源：http://ikn.zhixingplan.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pxo.fanxiaobao.xyz

[Q32] 分组拼接字符串
来源：http://mgi.hcnkem.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vcq.iojbl.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dlf.meibo888.top

[Q33] 多列分组
来源：http://gev.ydzc1.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://myu.aizwys.cn

[Q34] 每组取第一条
来源：http://med.kuanghao11.cn

SELECT * FROM (
来源：http://xhc.hammf.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nud.fehbvm.com

) t WHERE rn = 1;
来源：http://oxs.sweek.top

[Q35] 内连接
来源：http://zzl.xinyue.icu

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zik.yfazqb.com

[Q36] 左连接
来源：http://yxl.52xcode.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kfx.pycfn.com

[Q37] 右连接
来源：http://bsl.hnxiangtu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jdu.vqdsnc.cn

[Q38] 全外连接（PostgreSQL）
来源：http://apc.meibo888.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uku.yanxiufei.cn

[Q39] 自连接（查上下级）
来源：http://iae.ywan-chungtsiang.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ikr.gotoacloud.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://svc.nanxinkj.top

[Q40] 交叉连接（笛卡尔积）
来源：http://qkp.aibaodan.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tau.hcnkem.com

[Q41] 多表连接
来源：http://xiu.fanxiaobao.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://ewx.shuidangran.top

JOIN users u ON u.id = o.user_id
来源：http://dxc.ybcxt.top

JOIN products p ON p.id = o.product_id;
来源：http://ozw.yj20258.top

[Q42] 连接条件附加过滤
来源：http://mxl.wangdashe.top

SELECT u.name, o.amount FROM users u
来源：http://ply.aizwys.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tkv.jinyuanbaomall.cn

[Q43] 标量子查询
来源：http://yky.shzxlz.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ppt.tian-w.cn

[Q44] IN 子查询
来源：http://pmi.andypj.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gpo.xinyue.icu

[Q45] EXISTS 判断存在
来源：http://izu.ydjk.org.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fsh.aizwys.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ybp.jinyuanbaomall.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dxa.jinqigfzy.top

[Q47] 与平均值比较
来源：http://txo.zhengqikj.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://opo.chenlongwang.top

[Q48] CTE 公用表表达式
来源：http://shw.wangdashe.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zzk.jinqigufen.top

SELECT * FROM t WHERE c > 5;
来源：http://cuf.jinqigfzy.top

[Q49] 更新单行
来源：http://pyw.ppjwa.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pmv.nanxuanxn.top

[Q50] 批量更新
来源：http://vrr.ehwqpu.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kmn.yuanzhike.top

[Q51] 用子查询更新
来源：http://mzm.jinghuilouyu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iiw.yongpay.top

[Q52] 删除指定行
来源：http://xsh.aibaodan.cn

DELETE FROM users WHERE id = 10;
来源：http://iij.vehdjk.com

[Q53] 按条件删除
来源：http://ypn.ybcxt.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ebx.zhengqikj.top

[Q54] 清空表
来源：http://nev.jlsjyb.cn

TRUNCATE TABLE logs;
来源：http://nna.yuxming.cn

[Q55] 排名（并列占位）
来源：http://frf.zhixingplan.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jhs.birdmap.top

[Q56] 密集排名（并列不占位）
来源：http://ykx.ehwqpu.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xzz.jlsjyb.cn

[Q57] 行号
来源：http://gbe.9152youxi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://aih.guannengcc.top

[Q58] 累计求和
来源：http://rnf.zycfv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xbi.hysaishi.cn

[Q59] 分组内累计
来源：http://dqf.quarkkingdee.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://deo.vqdsnc.cn

[Q60] 取上一行 / 下一行
来源：http://sit.iojbl.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cju.shanyushiyangkeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fvi.xingfuxueyuan.xyz

[Q61] 移动平均
来源：http://xap.chenjidiqi.icu

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mrc.iojbl.cn

[Q62] 分组占比
来源：http://acm.hongshengwenyu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ckk.shzxlz.cn

[Q63] 开启事务
来源：http://fdw.shanyushiyangtech.top

START TRANSACTION;                -- 或 BEGIN
来源：http://fsf.hnqzz.top

[Q64] 提交事务
来源：http://olk.yj202588.top

COMMIT;
来源：http://lkz.316326.xyz

[Q65] 回滚事务
来源：http://unx.yongpay.top

ROLLBACK;
来源：http://fqq.ydjk.org.cn

[Q66] 行锁查询
来源：http://nra.jinqigufen.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://aom.snrcjt.cn

[Q67] 设置隔离级别
来源：http://hgk.gogol.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sgn.dianchejie.cn

[Q68] 保存点
来源：http://myq.jianghu66.top

SAVEPOINT sp1;
来源：http://xsq.ywan-chungtsiang.top

ROLLBACK TO sp1;
来源：http://lmr.yueranfly.top

[Q69] 查看执行计划
来源：http://oql.dianchejie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vsu.redwolf501.top

[Q70] 更新统计信息
来源：http://mln.hysaishi.cn

ANALYZE TABLE users;
来源：http://igm.ydjk.org.cn

[Q71] 查看建表语句
来源：http://bba.sysykeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dsx.vqdsnc.cn

[Q72] 查看索引
来源：http://weu.shanyushiyangkeji.top

SHOW INDEX FROM users;
来源：http://qlo.xingfuxueyuan.xyz

[Q73] 查看表状态
来源：http://xrt.ctjpmb.com

SHOW TABLE STATUS LIKE 'users';
来源：http://xlp.smart0.xyz

[Q74] 强制使用索引
来源：http://luw.316326.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yha.daria6918.cn

[Q75] 日期格式化
来源：http://gir.zhaomingkeji.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eet.tanke756.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://nyf.cheryme.top


<!-- 参考信息 -->