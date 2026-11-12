代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qoq.ppjwa.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pzr.sufxvd.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xwl.kuanghao11.cn

TS:   // 同 JS
来源：http://vyw.jianghu66.top

Java: new Thread(() -> f()).start()
来源：http://hrf.jyoumei.cn

Go:   go f()
来源：http://eqo.gzhubu.top

Ruby: Thread.new { f }
来源：http://vwa.zhongyouzk.top

C#:   Task.Run(() => F());
来源：http://duv.tanke756.top

[O02] 使用线程池
来源：http://pbx.nanxinkj.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ezg.chenjidiqi.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://iyj.tian-w.cn

JS:   // worker_threads 线程池
来源：http://yjy.ywan-chungtsiang.top

TS:   // worker_threads 线程池
来源：http://krg.zycfv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://cxo.jqgfzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tqn.zdqjudy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ock.dashuyun.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bue.yanxiufei.cn

[O03] 加锁保护共享数据
来源：http://udc.fehbvm.com

Py:   with lock: shared += 1
来源：http://rsy.fanxiaobao.xyz

PHP:  // 用 flock() 做文件锁
来源：http://ujp.ydjk.org.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wnv.shzxlz.cn

TS:   // 同 JS
来源：http://thu.xuetiantiany.cn

Java: synchronized (this) { shared++; }
来源：http://jkp.jinqigufen.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xqt.zhaomingkeji.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://olp.cheryme.top

C#:   lock (gate) { shared++; }
来源：http://rui.zdqjudy.top

[O04] 定义异步函数并等待
来源：http://tvg.zhiwuduotai.top

Py:   async def f():⏎    await g()
来源：http://hso.gotoacloud.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dch.pycfn.com

JS:   async function f() { await g(); }
来源：http://oih.chenlongwang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://tya.redwolf501.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bcl.guannengcc.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rna.ydzc1.top

Ruby: # 用 Fiber 或 async gem
来源：http://nmc.aibaodan.cn

C#:   async Task F() { await G(); }
来源：http://bax.svipenyu.cn

[O05] 并发执行并等待全部完成
来源：http://qbi.wangshuangyany.cn

Py:   asyncio.gather(*tasks)
来源：http://she.nanxinkj.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vjp.316326.xyz

JS:   await Promise.all(tasks)
来源：http://jaz.wangdashe.top

TS:   await Promise.all(tasks)
来源：http://qpg.shanyushiyangtech.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ogk.svipenyu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://skd.zhengqikj.top

Ruby: threads.map(&:join)
来源：http://sng.sysykeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mti.fanxiaobao.xyz

[O06] 使用进程池
来源：http://dsu.havefunace.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tkg.xingfuxueyuan.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://pcg.hesvh.cn

JS:   // child_process / cluster 模块
来源：http://aob.zhijiandao.cn

TS:   // child_process / cluster 模块
来源：http://epj.jianghu66.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oln.sufxvd.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lbe.gaohongyu789.top

Ruby: // fork 块
来源：http://dnk.zhongyouzk.top

C#:   Parallel.For
来源：http://nou.fengsongda.top

================================================================================
来源：http://yxk.zdqjudy.top

P. 常用工具函数
来源：http://gqt.jiagoushi.top

================================================================================
来源：http://hnm.cheryme.top

[P01] 生成 UUID
来源：http://wvn.hammf.cn

Py:   str(uuid.uuid4())
来源：http://ewy.xinyue.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://iyv.sxryk.cn

JS:   crypto.randomUUID()
来源：http://mvb.zhijiandao.cn

TS:   crypto.randomUUID()
来源：http://jme.nwbrower.top

Java: UUID.randomUUID().toString()
来源：http://cik.hongshengwenyu.top

Go:   // 用 github.com/google/uuid
来源：http://iui.fengsongda.top

Ruby: SecureRandom.uuid
来源：http://gyb.yongpay.top

C#:   Guid.NewGuid().ToString()
来源：http://hrs.ydjk.org.cn

[P02] MD5 / SHA256 摘要
来源：http://cvh.tianlin.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jbe.chenzaomai.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://pap.birdmap.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qiu.nanxinkj.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ojy.pycfn.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lxx.pengpengdd.cyou

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qcp.yuxming.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://twu.xingfuxueyuan.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kab.sxryk.cn

[P03] 生成短随机字符串
来源：http://rww.ybcxt.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xbx.fengsongda.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pqq.zhiwuduotai.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yoq.hammf.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cyb.aibaodan.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wfr.fktsv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rxw.zhijiandao.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cjy.shzxlz.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jyc.cucudq.cn

[P04] 求长度
来源：http://hdi.uphjek.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qnn.c1oappe.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pqi.zhengqikj.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cjm.shzxlz.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yeo.hongshengwenyu.top

Java: list.size();  map.size();  s.length()
来源：http://gdn.bbcook.cn

Go:   len(arr);  len(m)
来源：http://ooo.ydzc1.top

Ruby: x.length;  x.size
来源：http://vyg.ydzc1.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gyh.daxiang520.top

[P05] 判断两个对象内容是否相等
来源：http://tlh.kuanghao11.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://jgv.dianchejie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ngn.ybcxt.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://aqr.vehdjk.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kpp.jqgfzy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qiu.fzhhl.top

Go:   reflect.DeepEqual(a, b)
来源：http://ogs.fengsongda.top

Ruby: a == b
来源：http://ass.jiagoushi.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xkt.hammf.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pyf.jqgfzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vok.pycfn.com

PHP:  if (empty($x)) {}
来源：http://hlu.nwbrower.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xke.cqqwz.cn

TS:   if (x == null) {}
来源：http://mfm.zhijiandao.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://eur.sweek.top

Go:   if x == nil {}
来源：http://dkm.9152youxi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vvn.shzxlz.cn

C#:   if (x is null) {}
来源：http://jvr.yonumen.top

[P07] 防抖与节流
来源：http://zvx.wangdashe.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jgz.yuanzhike.top

PHP:  // 手写时间戳比较
来源：http://mjz.shanyushiyangtech.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xxf.zhixingplan.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://isj.sweek.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lmq.9152youxi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sty.yj202588.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://lai.bbcook.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://agx.sjlbkw.cn

[P08] 处理浮点精度问题
来源：http://aos.tian-w.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sla.sxryk.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vae.tianlin.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ceg.yuanzhike.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vhn.52xcode.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xfd.hywenlv.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://aea.hcnkem.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bve.tianlin.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dhp.jyoumei.cn

================================================================================
来源：http://gsh.shuidangran.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vfs.hnxiangtu.top

================================================================================
来源：http://axs.ctjpmb.com

[Q01] 创建表
来源：http://hee.gaohongyu789.top

CREATE TABLE users (
来源：http://ngz.guannengcc.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tqb.yuxming.cn

name VARCHAR(50) NOT NULL,
来源：http://noe.sjlbkw.cn

email VARCHAR(100) UNIQUE,
来源：http://yli.xziqi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bro.tanke756.top

);
来源：http://fbd.aibaodan.cn

[Q02] 创建带外键的表
来源：http://vkj.sxryk.cn

CREATE TABLE orders (
来源：http://ill.sufxvd.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://buu.tianlin.xyz

user_id INT NOT NULL,
来源：http://zvh.jiagoushi.top

amount DECIMAL(10, 2),
来源：http://kgy.haohaochexian.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ami.fengsongda.top

);
来源：http://kqw.cqqwz.cn

[Q03] 增加列
来源：http://dbl.gogol.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wiz.tanke756.top

[Q04] 修改列类型
来源：http://dxl.ppjwa.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://muv.xuetiantiany.cn

[Q05] 重命名列
来源：http://dtb.cdnleiting.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dpz.cdnleiting.top

[Q06] 删除列
来源：http://lro.jqgufenzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://txx.yuxming.cn

[Q07] 删除表
来源：http://mxb.aizwys.cn

DROP TABLE IF EXISTS orders;
来源：http://qqc.daxiang520.top

[Q08] 创建普通索引
来源：http://tvq.hnxiangtu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jkz.mhx1999.top

[Q09] 创建唯一索引
来源：http://jhl.yongpay.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cfj.sysykeji.top

[Q10] 插入单行
来源：http://fdf.cdnleiting.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://orh.yfazqb.com

[Q11] 一次插入多行
来源：http://zrz.yangfankeji.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xef.tian-w.cn

[Q12] 插入后取自增 ID
来源：http://npa.cqqwz.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tnr.cucudq.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cmo.zdbjq.cn

[Q13] 忽略重复插入
来源：http://zrg.yuxming.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xcj.zhiwuduotai.top

[Q14] 存在则更新（upsert）
来源：http://opf.zhoulong.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qru.zycfv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://okv.0kj1m.cn

[Q15] 查询全部
来源：http://ifz.cucudq.cn

SELECT * FROM users;
来源：http://zkk.cheryme.top

[Q16] 查询指定列
来源：http://pww.shuidangran.top

SELECT id, name FROM users;
来源：http://oar.pengpengdd.cyou

[Q17] 条件查询
来源：http://yrf.cashguo.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dws.hammf.cn

[Q18] 模糊匹配
来源：http://ekv.dashuyun.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xzt.zdqjudy.top

[Q19] 范围查询
来源：http://tdd.52xcode.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qbx.zhengqikj.top

[Q20] IN 列表
来源：http://dau.sjlbkw.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vnm.chenlongwang.top

[Q21] 空值判断
来源：http://kpy.vqdsnc.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fic.sjlbkw.cn

[Q22] 排序
来源：http://vef.jinqigfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tth.zhongyouzk.top

[Q23] 分页
来源：http://qtb.zhongyouzk.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://iyr.nanxuanxn.top

[Q24] 去重
来源：http://qnf.hnqzz.top

SELECT DISTINCT city FROM users;
来源：http://aip.hcnkem.com

[Q25] 只取前 N 条
来源：http://cop.iojbl.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ufx.zhiwuduotai.top

[Q26] 计数
来源：http://wjj.zdqjudy.top

SELECT COUNT(*) FROM users;
来源：http://kzj.yonumen.top

[Q27] 条件计数
来源：http://bbu.uphjek.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kmf.yj202588.top

[Q28] 求和与平均
来源：http://czh.iojbl.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://poa.hfpthk.cn

[Q29] 最大最小值
来源：http://ydx.bjfxy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://pdj.jqgufenzy.top

[Q30] 分组统计
来源：http://uun.yonumen.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xai.yueranfly.top

[Q31] 分组后过滤
来源：http://lvw.nanxinkj.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ydc.jinqigufen.top

[Q32] 分组拼接字符串
来源：http://bof.vqdsnc.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ptr.tanke756.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ssr.hywenlv.cn

[Q33] 多列分组
来源：http://nks.chenzaomai.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://klh.dianchejie.cn

[Q34] 每组取第一条
来源：http://qzd.jiagoushi.top

SELECT * FROM (
来源：http://wdx.yuanzhike.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ydy.guowangkeji.top

) t WHERE rn = 1;
来源：http://ony.yj20258888.top

[Q35] 内连接
来源：http://yke.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rzu.jyoumei.cn

[Q36] 左连接
来源：http://pel.52xcode.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bza.yj20258.top

[Q37] 右连接
来源：http://hcz.aibaodan.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xih.fzhhl.top

[Q38] 全外连接（PostgreSQL）
来源：http://tge.chenzaomai.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xbe.zdbjq.cn

[Q39] 自连接（查上下级）
来源：http://rsz.xylfe.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://pqs.hesvh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ttv.52xcode.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xgm.jinghuilouyu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uzv.shanyushiyangkeji.top

[Q41] 多表连接
来源：http://iah.zdbjq.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ejj.zhijiandao.cn

JOIN users u ON u.id = o.user_id
来源：http://aue.shuidangran.top

JOIN products p ON p.id = o.product_id;
来源：http://evx.xinyue.icu

[Q42] 连接条件附加过滤
来源：http://ygm.dianchejie.cn

SELECT u.name, o.amount FROM users u
来源：http://fvx.zhiwuduotai.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mti.yongpay.top

[Q43] 标量子查询
来源：http://ibl.yueranfly.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bpi.9152youxi.cn

[Q44] IN 子查询
来源：http://lqq.feifeiyinyue.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rwh.shuidangran.top

[Q45] EXISTS 判断存在
来源：http://ktx.shangyingyoupin.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zqd.uphjek.com

[Q46] NOT EXISTS 判断不存在
来源：http://jxe.tarul.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ciw.sufxvd.cn

[Q47] 与平均值比较
来源：http://nwo.9152youxi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ruq.meibo888.top

[Q48] CTE 公用表表达式
来源：http://gzl.hongshengwenyu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bsi.fktsv.cn

SELECT * FROM t WHERE c > 5;
来源：http://oyy.hfpthk.cn

[Q49] 更新单行
来源：http://kkw.dianchejie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gkz.zhiwuduotai.top

[Q50] 批量更新
来源：http://trx.guowangkeji.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vjt.cucudq.cn

[Q51] 用子查询更新
来源：http://vaw.hnqzz.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://czg.jinghuilouyu.cn

[Q52] 删除指定行
来源：http://olm.iojbl.cn

DELETE FROM users WHERE id = 10;
来源：http://fft.jinqigfzy.top

[Q53] 按条件删除
来源：http://tjk.pengpengdd.cyou

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rni.guowangkeji.top

[Q54] 清空表
来源：http://yke.xziqi.cn

TRUNCATE TABLE logs;
来源：http://hii.hysaishi.cn

[Q55] 排名（并列占位）
来源：http://ndl.zhongyouzk.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cxx.aibaodan.cn

[Q56] 密集排名（并列不占位）
来源：http://hng.sjlbkw.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qnr.aibaodan.cn

[Q57] 行号
来源：http://ftq.mhx1999.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vdp.uphjek.com

[Q58] 累计求和
来源：http://zxw.chenzaomai.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bpr.yvedp.cn

[Q59] 分组内累计
来源：http://yct.svipenyu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://adu.cashguo.top

[Q60] 取上一行 / 下一行
来源：http://gla.xuanzx.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zvx.xuanzx.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ibw.shzxlz.cn

[Q61] 移动平均
来源：http://mpt.smart0.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fvv.hongshengwenyu.top

[Q62] 分组占比
来源：http://ica.sjlbkw.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jjy.xinyue.icu

[Q63] 开启事务
来源：http://zsg.shanyushiyangkeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://pml.iojbl.cn

[Q64] 提交事务
来源：http://nfa.yfazqb.com

COMMIT;
来源：http://wvl.fzhhl.top

[Q65] 回滚事务
来源：http://par.chenzaomai.com

ROLLBACK;
来源：http://swz.sjlbkw.cn

[Q66] 行锁查询
来源：http://mgr.dashuyun.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tnh.birdmap.top

[Q67] 设置隔离级别
来源：http://tpj.gotoacloud.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rfz.aibaodan.cn

[Q68] 保存点
来源：http://ekp.aizwys.cn

SAVEPOINT sp1;
来源：http://vzs.andypj.xyz

ROLLBACK TO sp1;
来源：http://and.yangfankeji.com

[Q69] 查看执行计划
来源：http://ers.xingfuxueyuan.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hbk.daria6918.cn

[Q70] 更新统计信息
来源：http://cet.wangdashe.top

ANALYZE TABLE users;
来源：http://bgv.yvedp.cn

[Q71] 查看建表语句
来源：http://efl.zhengqikj.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pul.daria6918.cn

[Q72] 查看索引
来源：http://xwy.cdnleiting.top

SHOW INDEX FROM users;
来源：http://iqc.svipenyu.cn

[Q73] 查看表状态
来源：http://fdr.gogol.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lin.chenjidiqi.icu

[Q74] 强制使用索引
来源：http://dsj.chenzaomai.com


<!-- 参考信息 -->