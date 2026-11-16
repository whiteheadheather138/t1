代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://inx.wangdashe.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fwt.yj20258.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rph.dianchejie.cn

TS:   // 同 JS
来源：http://kys.yanxiufei.cn

Java: new Thread(() -> f()).start()
来源：http://nfb.yuxming.cn

Go:   go f()
来源：http://jrd.sufxvd.cn

Ruby: Thread.new { f }
来源：http://jct.hysaishi.cn

C#:   Task.Run(() => F());
来源：http://tfe.hnqzz.top

[O02] 使用线程池
来源：http://qtt.hysaishi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mra.yonumen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oyn.cucudq.cn

JS:   // worker_threads 线程池
来源：http://pok.ywan-chungtsiang.top

TS:   // worker_threads 线程池
来源：http://izl.yj20258.top

Java: Executors.newFixedThreadPool(4)
来源：http://afh.yueranfly.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wwr.yonumen.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cnt.hywenlv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://twb.sjlbkw.cn

[O03] 加锁保护共享数据
来源：http://vhj.ppjwa.cn

Py:   with lock: shared += 1
来源：http://rvn.ivvv.top

PHP:  // 用 flock() 做文件锁
来源：http://dza.redwolf501.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qdo.52xcode.cn

TS:   // 同 JS
来源：http://bze.yfazqb.com

Java: synchronized (this) { shared++; }
来源：http://fwp.ybcxt.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://myl.guannengcc.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://nzs.daria6918.cn

C#:   lock (gate) { shared++; }
来源：http://dze.nanxinkj.top

[O04] 定义异步函数并等待
来源：http://zho.gzhubu.top

Py:   async def f():⏎    await g()
来源：http://byy.fanxiaobao.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bde.wangshuangyany.cn

JS:   async function f() { await g(); }
来源：http://nhi.dashuyun.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nze.cdnleiting.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kwv.zdqjudy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fii.fanxiaobao.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://vja.guannengcc.top

C#:   async Task F() { await G(); }
来源：http://bep.jiagoushi.top

[O05] 并发执行并等待全部完成
来源：http://slz.zhongyouzk.top

Py:   asyncio.gather(*tasks)
来源：http://dyr.yuxming.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ezx.jlsjyb.cn

JS:   await Promise.all(tasks)
来源：http://hfi.fanxiaobao.xyz

TS:   await Promise.all(tasks)
来源：http://suh.andypj.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cih.gaohongyu789.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xge.uphjek.com

Ruby: threads.map(&:join)
来源：http://nrd.fanxiaobao.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://bgq.fehbvm.com

[O06] 使用进程池
来源：http://lyd.yj20258888.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xua.nanxinkj.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qjb.xinyue.icu

JS:   // child_process / cluster 模块
来源：http://sgk.zhoulong.xyz

TS:   // child_process / cluster 模块
来源：http://lwx.zhengqikj.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dhf.xingfuxueyuan.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mmx.hongshengwenyu.top

Ruby: // fork 块
来源：http://etf.xingfuxueyuan.xyz

C#:   Parallel.For
来源：http://vsf.ehwqpu.com

================================================================================
来源：http://wve.jlsjyb.cn

P. 常用工具函数
来源：http://mgl.yongpay.top

================================================================================
来源：http://arw.gzhubu.top

[P01] 生成 UUID
来源：http://gqg.nwbrower.top

Py:   str(uuid.uuid4())
来源：http://sgm.aizwys.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tge.9152youxi.cn

JS:   crypto.randomUUID()
来源：http://onr.tanke756.top

TS:   crypto.randomUUID()
来源：http://ysn.sufxvd.cn

Java: UUID.randomUUID().toString()
来源：http://foc.hnxiangtu.top

Go:   // 用 github.com/google/uuid
来源：http://wms.snrcjt.cn

Ruby: SecureRandom.uuid
来源：http://pmq.yongpay.top

C#:   Guid.NewGuid().ToString()
来源：http://rhm.gotoacloud.top

[P02] MD5 / SHA256 摘要
来源：http://bmc.jinqigufen.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wkp.tianlin.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://cmc.hongshengwenyu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://clg.yangfankeji.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://utx.guowangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://iuk.cheryme.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://viw.c1oappe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lmw.vehdjk.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://riz.xuetiantiany.cn

[P03] 生成短随机字符串
来源：http://eon.316326.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xhh.shanyushiyangtech.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gjb.sysykeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cpn.svipenyu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://upm.jianghu66.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ayl.guowangkeji.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pzp.havefunace.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://isw.9152youxi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yqk.52xcode.cn

[P04] 求长度
来源：http://lwm.c1oappe.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wnb.cashguo.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bqp.jinqigufen.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wll.bbcook.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dxm.sysykeji.top

Java: list.size();  map.size();  s.length()
来源：http://whl.fehbvm.com

Go:   len(arr);  len(m)
来源：http://vir.andypj.xyz

Ruby: x.length;  x.size
来源：http://vlb.wangshuangyany.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mum.yuanzhike.top

[P05] 判断两个对象内容是否相等
来源：http://prf.snrcjt.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wkt.vqdsnc.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bzw.uphjek.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tnz.shuidangran.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rjp.yuxming.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tzn.aibaodan.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lzh.jqgufenzy.top

Ruby: a == b
来源：http://yac.feifeiyinyue.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wpg.xuetiantiany.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bqy.hnxiangtu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kwb.tianlin.xyz

PHP:  if (empty($x)) {}
来源：http://eln.hcnkem.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://for.nwbrower.top

TS:   if (x == null) {}
来源：http://tit.sysykeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://kdq.hnqzz.top

Go:   if x == nil {}
来源：http://flt.nanxuanxn.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://brc.bjfxy.top

C#:   if (x is null) {}
来源：http://ngs.hongshengwenyu.top

[P07] 防抖与节流
来源：http://yfu.gogol.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://seo.wangshuangyany.cn

PHP:  // 手写时间戳比较
来源：http://utm.zhongyouzk.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bdh.yonumen.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bgr.redwolf501.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dvl.wangdashe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bys.zhijiandao.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ilj.xziqi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ltj.chenlongwang.top

[P08] 处理浮点精度问题
来源：http://awv.gaohongyu789.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://shi.chenjidiqi.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gvn.c1oappe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://agr.dianchejie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://idr.smart0.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://izj.tian-w.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://glz.yuanzhike.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rae.daria6918.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ijd.ydjk.org.cn

================================================================================
来源：http://dzz.zdbjq.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pxg.yuanzhike.top

================================================================================
来源：http://gku.wangdashe.top

[Q01] 创建表
来源：http://pto.iojbl.cn

CREATE TABLE users (
来源：http://wlu.0kj1m.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://laz.jinghuilouyu.cn

name VARCHAR(50) NOT NULL,
来源：http://lmn.redwolf501.top

email VARCHAR(100) UNIQUE,
来源：http://qyu.yfazqb.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qpe.shanyushiyangtech.top

);
来源：http://iaf.9152youxi.cn

[Q02] 创建带外键的表
来源：http://cch.cucudq.cn

CREATE TABLE orders (
来源：http://yqi.bjfxy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oyd.epnwcf.com

user_id INT NOT NULL,
来源：http://yjr.birdmap.top

amount DECIMAL(10, 2),
来源：http://gpx.xinyue.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pfw.nwbrower.top

);
来源：http://pod.nwbrower.top

[Q03] 增加列
来源：http://vpj.smart0.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vsp.ybcxt.top

[Q04] 修改列类型
来源：http://fhd.gotoacloud.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ijn.zhongyouzk.top

[Q05] 重命名列
来源：http://sgj.jqgfzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ezr.zhengqikj.top

[Q06] 删除列
来源：http://wwg.sweek.top

ALTER TABLE users DROP COLUMN age;
来源：http://nur.yj20258888.top

[Q07] 删除表
来源：http://dwt.chenlongwang.top

DROP TABLE IF EXISTS orders;
来源：http://hcg.svipenyu.cn

[Q08] 创建普通索引
来源：http://waj.vehdjk.com

CREATE INDEX idx_users_email ON users(email);
来源：http://srj.ydjk.org.cn

[Q09] 创建唯一索引
来源：http://onn.zhiwuduotai.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jqk.jiagoushi.top

[Q10] 插入单行
来源：http://hjs.xziqi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zwz.tian-w.cn

[Q11] 一次插入多行
来源：http://sei.yvedp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nxz.quarkkingdee.top

[Q12] 插入后取自增 ID
来源：http://gzw.zdbjq.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fqs.gogol.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ayo.xingfuxueyuan.xyz

[Q13] 忽略重复插入
来源：http://vwk.daria6918.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://etp.yangfankeji.com

[Q14] 存在则更新（upsert）
来源：http://jvk.hammf.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zpd.bbcook.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://thc.zdqjudy.top

[Q15] 查询全部
来源：http://xkt.hcnkem.com

SELECT * FROM users;
来源：http://xem.ydjk.org.cn

[Q16] 查询指定列
来源：http://hfp.tian-w.cn

SELECT id, name FROM users;
来源：http://ynh.sufxvd.cn

[Q17] 条件查询
来源：http://vrs.haohaochexian.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tzn.ywan-chungtsiang.top

[Q18] 模糊匹配
来源：http://ood.yanxiufei.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qho.hongshengwenyu.top

[Q19] 范围查询
来源：http://luw.pengpengdd.cyou

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://aia.yvedp.cn

[Q20] IN 列表
来源：http://gms.hysaishi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://txx.shzxlz.cn

[Q21] 空值判断
来源：http://ige.zhoulong.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://bzx.redwolf501.top

[Q22] 排序
来源：http://dlb.guowangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cxm.zhixingplan.top

[Q23] 分页
来源：http://ota.iojbl.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ycu.zdqjudy.top

[Q24] 去重
来源：http://fja.jinqigfzy.top

SELECT DISTINCT city FROM users;
来源：http://ivc.quarkkingdee.top

[Q25] 只取前 N 条
来源：http://nks.smart0.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://urx.sysykeji.top

[Q26] 计数
来源：http://eqv.quarkkingdee.top

SELECT COUNT(*) FROM users;
来源：http://lqh.birdmap.top

[Q27] 条件计数
来源：http://hpu.shanyushiyangkeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pxd.sjlbkw.cn

[Q28] 求和与平均
来源：http://kov.zhiwuduotai.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fzs.yonumen.top

[Q29] 最大最小值
来源：http://gtb.tarul.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pdx.haohaochexian.top

[Q30] 分组统计
来源：http://tuk.quarkkingdee.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ubm.jiagoushi.top

[Q31] 分组后过滤
来源：http://yoy.xinyue.icu

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qcl.sxryk.cn

[Q32] 分组拼接字符串
来源：http://zgi.vqdsnc.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hwz.jinqigufen.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kvd.quarkkingdee.top

[Q33] 多列分组
来源：http://wog.cdnleiting.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qva.tian-w.cn

[Q34] 每组取第一条
来源：http://edd.bbcook.cn

SELECT * FROM (
来源：http://bqe.ctjpmb.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://byt.316326.xyz

) t WHERE rn = 1;
来源：http://qxr.smart0.xyz

[Q35] 内连接
来源：http://xnf.ydjk.org.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ywg.dashuyun.cn

[Q36] 左连接
来源：http://cby.vqdsnc.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vjn.aizwys.cn

[Q37] 右连接
来源：http://lew.0kj1m.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://riv.sysykeji.top

[Q38] 全外连接（PostgreSQL）
来源：http://flw.ydzc1.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ydc.svipenyu.cn

[Q39] 自连接（查上下级）
来源：http://fqc.ybcxt.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://dkq.yonumen.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mmz.daria6918.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ojl.jyoumei.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vjg.nwbrower.top

[Q41] 多表连接
来源：http://ogs.gogol.net.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://eob.wangshuangyany.cn

JOIN users u ON u.id = o.user_id
来源：http://mxd.zhixingplan.top

JOIN products p ON p.id = o.product_id;
来源：http://mmk.jlsjyb.cn

[Q42] 连接条件附加过滤
来源：http://bqg.fehbvm.com

SELECT u.name, o.amount FROM users u
来源：http://pbf.zhixingplan.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://icy.52xcode.cn

[Q43] 标量子查询
来源：http://ebq.316326.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tml.tarul.cn

[Q44] IN 子查询
来源：http://alf.jqgufenzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zxi.hcnkem.com

[Q45] EXISTS 判断存在
来源：http://syv.jianghu66.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://adj.pengpengdd.cyou

[Q46] NOT EXISTS 判断不存在
来源：http://xcs.haohaochexian.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://trv.cucudq.cn

[Q47] 与平均值比较
来源：http://uwx.jinghuilouyu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://avz.xziqi.cn

[Q48] CTE 公用表表达式
来源：http://nhg.zhoulong.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cxl.zycfv.cn

SELECT * FROM t WHERE c > 5;
来源：http://xyu.hammf.cn

[Q49] 更新单行
来源：http://bnb.sjlbkw.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://eie.yuxming.cn

[Q50] 批量更新
来源：http://jix.xziqi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uhx.cheryme.top

[Q51] 用子查询更新
来源：http://eic.zhongyouzk.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vsc.wangshuangyany.cn

[Q52] 删除指定行
来源：http://awq.zhiwuduotai.top

DELETE FROM users WHERE id = 10;
来源：http://yxg.sweek.top

[Q53] 按条件删除
来源：http://cqx.ehwqpu.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rdt.hesvh.cn

[Q54] 清空表
来源：http://ylq.hysaishi.cn

TRUNCATE TABLE logs;
来源：http://hds.c1oappe.top

[Q55] 排名（并列占位）
来源：http://vjj.dashuyun.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://epb.havefunace.top

[Q56] 密集排名（并列不占位）
来源：http://tsw.feifeiyinyue.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://csr.quarkkingdee.top

[Q57] 行号
来源：http://oal.bbcook.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nvs.jinqigfzy.top

[Q58] 累计求和
来源：http://cky.c1oappe.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wne.wangdashe.top

[Q59] 分组内累计
来源：http://tgm.nanxinkj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://psu.pycfn.com

[Q60] 取上一行 / 下一行
来源：http://iij.fanxiaobao.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hwl.sjlbkw.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wkh.jqgufenzy.top

[Q61] 移动平均
来源：http://wmw.shuidangran.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qnp.xziqi.cn

[Q62] 分组占比
来源：http://jcl.zdqjudy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://drf.zhongyouzk.top

[Q63] 开启事务
来源：http://xoc.yangfankeji.com

START TRANSACTION;                -- 或 BEGIN
来源：http://uqw.dashuyun.cn

[Q64] 提交事务
来源：http://adf.jqgufenzy.top

COMMIT;
来源：http://txc.yuxming.cn

[Q65] 回滚事务
来源：http://fye.dashuyun.cn

ROLLBACK;
来源：http://cah.zhongyouzk.top

[Q66] 行锁查询
来源：http://tkx.jqgfzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tzn.tanke756.top

[Q67] 设置隔离级别
来源：http://tpp.epnwcf.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://geq.zdqjudy.top

[Q68] 保存点
来源：http://qts.haohaochexian.top

SAVEPOINT sp1;
来源：http://ldq.jqgufenzy.top

ROLLBACK TO sp1;
来源：http://wwv.cqqwz.cn

[Q69] 查看执行计划
来源：http://dmm.xinyue.icu

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qfx.smart0.xyz

[Q70] 更新统计信息
来源：http://hxl.chenzaomai.com

ANALYZE TABLE users;
来源：http://grg.tanke756.top

[Q71] 查看建表语句
来源：http://xjz.quarkkingdee.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bba.shzxlz.cn

[Q72] 查看索引
来源：http://bjy.cashguo.top

SHOW INDEX FROM users;
来源：http://gug.xziqi.cn

[Q73] 查看表状态
来源：http://yxz.feifeiyinyue.top

SHOW TABLE STATUS LIKE 'users';
来源：http://zae.316326.xyz

[Q74] 强制使用索引
来源：http://rzs.sysykeji.top


<!-- 参考信息 -->