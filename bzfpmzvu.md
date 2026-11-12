代发 wailian999

[O02] 使用线程池
来源：http://ymx.zhongyouzk.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oii.hywenlv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fdg.shuidangran.top

JS:   // worker_threads 线程池
来源：http://scs.yongpay.top

TS:   // worker_threads 线程池
来源：http://prb.fanxiaobao.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://gdp.yj20258888.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pae.quarkkingdee.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gsq.kuanghao11.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mzn.ywan-chungtsiang.top

[O03] 加锁保护共享数据
来源：http://fbb.zhengqikj.top

Py:   with lock: shared += 1
来源：http://lwb.ivvv.top

PHP:  // 用 flock() 做文件锁
来源：http://ata.shanyushiyangkeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mxn.yj20258.top

TS:   // 同 JS
来源：http://luj.xingfuxueyuan.xyz

Java: synchronized (this) { shared++; }
来源：http://hfh.chenjidiqi.icu

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xsu.52xcode.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://nxm.epnwcf.com

C#:   lock (gate) { shared++; }
来源：http://gee.sysykeji.top

[O04] 定义异步函数并等待
来源：http://lta.tarul.cn

Py:   async def f():⏎    await g()
来源：http://svr.bjfxy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tvh.jianghu66.top

JS:   async function f() { await g(); }
来源：http://ekg.gotoacloud.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://see.shangyingyoupin.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://myn.zdqjudy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qcy.zhoulong.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://wcb.guowangkeji.top

C#:   async Task F() { await G(); }
来源：http://hye.hesvh.cn

[O05] 并发执行并等待全部完成
来源：http://wdy.guowangkeji.top

Py:   asyncio.gather(*tasks)
来源：http://yxk.hcnkem.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xws.bbcook.cn

JS:   await Promise.all(tasks)
来源：http://hxu.ydzc1.top

TS:   await Promise.all(tasks)
来源：http://itk.meibo888.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hgh.shuidangran.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uyp.pengpengdd.cyou

Ruby: threads.map(&:join)
来源：http://gox.yj20258.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fah.zhengqikj.top

[O06] 使用进程池
来源：http://cln.hnxiangtu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sol.yonumen.top

PHP:  // pcntl_fork 或多进程队列
来源：http://lnk.ywan-chungtsiang.top

JS:   // child_process / cluster 模块
来源：http://bjm.ydjk.org.cn

TS:   // child_process / cluster 模块
来源：http://plt.bbcook.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lud.xuanzx.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ivj.shzxlz.cn

Ruby: // fork 块
来源：http://yqy.tanke756.top

C#:   Parallel.For
来源：http://khj.quarkkingdee.top

================================================================================
来源：http://bnl.nwbrower.top

P. 常用工具函数
来源：http://jpd.yj20258888.top

================================================================================
来源：http://chv.jiagoushi.top

[P01] 生成 UUID
来源：http://cpv.ppjwa.cn

Py:   str(uuid.uuid4())
来源：http://waz.bbcook.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tja.fehbvm.com

JS:   crypto.randomUUID()
来源：http://osa.bbcook.cn

TS:   crypto.randomUUID()
来源：http://qxa.jqgufenzy.top

Java: UUID.randomUUID().toString()
来源：http://qku.zhengqikj.top

Go:   // 用 github.com/google/uuid
来源：http://vcg.jinqigfzy.top

Ruby: SecureRandom.uuid
来源：http://vvq.zhongyouzk.top

C#:   Guid.NewGuid().ToString()
来源：http://qlo.jiagoushi.top

[P02] MD5 / SHA256 摘要
来源：http://duw.xinyue.icu

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://whi.iojbl.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rti.xylfe.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rmz.gzhubu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ftk.xinyue.icu

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pjz.feifeiyinyue.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://phq.pengpengdd.cyou

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cgs.jqgufenzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://moo.gaohongyu789.top

[P03] 生成短随机字符串
来源：http://doh.yuxming.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fqk.birdmap.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wry.guowangkeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fut.ehwqpu.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://idr.tianlin.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sxn.guannengcc.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wur.guowangkeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://olp.yfazqb.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bzj.nwbrower.top

[P04] 求长度
来源：http://irj.fktsv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nhw.smart0.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vqh.sufxvd.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iul.sysykeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cyw.zdqjudy.top

Java: list.size();  map.size();  s.length()
来源：http://fij.316326.xyz

Go:   len(arr);  len(m)
来源：http://wnt.guowangkeji.top

Ruby: x.length;  x.size
来源：http://ntb.yongpay.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://rtj.zycfv.cn

[P05] 判断两个对象内容是否相等
来源：http://chx.uphjek.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://hpq.ybcxt.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uix.sjlbkw.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gzf.jiagoushi.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://got.yuanzhike.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tmq.tianlin.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://cfb.fengsongda.top

Ruby: a == b
来源：http://qcy.cdnleiting.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kri.zhijiandao.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://aqu.cheryme.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://aqe.fanxiaobao.xyz

PHP:  if (empty($x)) {}
来源：http://fxf.hesvh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://iqv.hesvh.cn

TS:   if (x == null) {}
来源：http://spl.yongpay.top

Java: if (x == null || x.isEmpty()) {}
来源：http://fue.shuidangran.top

Go:   if x == nil {}
来源：http://zyj.yonumen.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mua.hnxiangtu.top

C#:   if (x is null) {}
来源：http://cnb.chenjidiqi.icu

[P07] 防抖与节流
来源：http://npm.mhx1999.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ttg.yongpay.top

PHP:  // 手写时间戳比较
来源：http://llk.yueranfly.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://arn.sufxvd.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fut.xuetiantiany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uhe.nanxuanxn.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vke.tarul.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nqu.shzxlz.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cbc.nanxinkj.top

[P08] 处理浮点精度问题
来源：http://otl.nwbrower.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ghu.tarul.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ihp.shangyingyoupin.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xet.hnqzz.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zzt.ehwqpu.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pyv.fehbvm.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qbe.yvedp.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tnc.ydjk.org.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://afn.fehbvm.com

================================================================================
来源：http://yps.fktsv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gjy.guowangkeji.top

================================================================================
来源：http://znj.sxryk.cn

[Q01] 创建表
来源：http://ifa.zhiwuduotai.top

CREATE TABLE users (
来源：http://xey.yonumen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tmp.jqgfzy.top

name VARCHAR(50) NOT NULL,
来源：http://hzi.svipenyu.cn

email VARCHAR(100) UNIQUE,
来源：http://ivv.tian-w.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://whn.tianlin.xyz

);
来源：http://jne.zdqjudy.top

[Q02] 创建带外键的表
来源：http://orz.yfazqb.com

CREATE TABLE orders (
来源：http://yqd.havefunace.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ccc.gzhubu.top

user_id INT NOT NULL,
来源：http://wli.nanxuanxn.top

amount DECIMAL(10, 2),
来源：http://xrx.shuidangran.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nth.jiagoushi.top

);
来源：http://sbk.tanke756.top

[Q03] 增加列
来源：http://yhb.jinghuilouyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://shc.xuanzx.com

[Q04] 修改列类型
来源：http://jos.cqqwz.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qke.wangshuangyany.cn

[Q05] 重命名列
来源：http://hlu.tanke756.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cwf.dianchejie.cn

[Q06] 删除列
来源：http://ece.birdmap.top

ALTER TABLE users DROP COLUMN age;
来源：http://low.uphjek.com

[Q07] 删除表
来源：http://xtx.zhixingplan.top

DROP TABLE IF EXISTS orders;
来源：http://qvn.hcnkem.com

[Q08] 创建普通索引
来源：http://cja.yongpay.top

CREATE INDEX idx_users_email ON users(email);
来源：http://wsn.wangshuangyany.cn

[Q09] 创建唯一索引
来源：http://vef.hnxiangtu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jtc.guowangkeji.top

[Q10] 插入单行
来源：http://lda.zdbjq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nzy.hnxiangtu.top

[Q11] 一次插入多行
来源：http://hnb.svipenyu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pwv.chenlongwang.top

[Q12] 插入后取自增 ID
来源：http://bsi.fktsv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://uqr.hnxiangtu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lxz.birdmap.top

[Q13] 忽略重复插入
来源：http://fvb.yj202588.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yhs.yfazqb.com

[Q14] 存在则更新（upsert）
来源：http://uvt.cashguo.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://guh.jinqigufen.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jxk.havefunace.top

[Q15] 查询全部
来源：http://trr.jiagoushi.top

SELECT * FROM users;
来源：http://lyl.cashguo.top

[Q16] 查询指定列
来源：http://oyd.yj202588.top

SELECT id, name FROM users;
来源：http://qyl.pycfn.com

[Q17] 条件查询
来源：http://sup.mhx1999.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zcm.aizwys.cn

[Q18] 模糊匹配
来源：http://xfr.fengsongda.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://owx.52xcode.cn

[Q19] 范围查询
来源：http://bmw.tanke756.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rwh.chenlongwang.top

[Q20] IN 列表
来源：http://ito.ehwqpu.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ofj.jqgfzy.top

[Q21] 空值判断
来源：http://ymv.jinyuanbaomall.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dlf.vqdsnc.cn

[Q22] 排序
来源：http://snk.ybcxt.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wek.bjfxy.top

[Q23] 分页
来源：http://vjr.yueranfly.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rbo.jiagoushi.top

[Q24] 去重
来源：http://see.xylfe.cn

SELECT DISTINCT city FROM users;
来源：http://cbf.hcnkem.com

[Q25] 只取前 N 条
来源：http://yuf.gogol.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rjv.xziqi.cn

[Q26] 计数
来源：http://cfb.meibo888.top

SELECT COUNT(*) FROM users;
来源：http://tul.iojbl.cn

[Q27] 条件计数
来源：http://vlt.xylfe.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mxr.jqgufenzy.top

[Q28] 求和与平均
来源：http://hjf.daxiang520.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lsh.yanxiufei.cn

[Q29] 最大最小值
来源：http://tcg.kuanghao11.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jqg.yongpay.top

[Q30] 分组统计
来源：http://coe.fanxiaobao.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://okb.tanke756.top

[Q31] 分组后过滤
来源：http://dnn.sxryk.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wcj.iojbl.cn

[Q32] 分组拼接字符串
来源：http://erz.tian-w.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ndf.ivvv.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wom.iojbl.cn

[Q33] 多列分组
来源：http://hgl.vqdsnc.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pah.zhaomingkeji.xyz

[Q34] 每组取第一条
来源：http://kgs.shzxlz.cn

SELECT * FROM (
来源：http://qqh.wangshuangyany.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xrh.snrcjt.cn

) t WHERE rn = 1;
来源：http://wfj.ehwqpu.com

[Q35] 内连接
来源：http://pzp.yonumen.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cra.hysaishi.cn

[Q36] 左连接
来源：http://jfn.meibo888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ibo.havefunace.top

[Q37] 右连接
来源：http://qfn.gzhubu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qhy.bjfxy.top

[Q38] 全外连接（PostgreSQL）
来源：http://yls.zhixingplan.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jei.svipenyu.cn

[Q39] 自连接（查上下级）
来源：http://ktr.cdnleiting.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://gxh.hnxiangtu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oyx.jinyuanbaomall.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ttp.jianghu66.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tic.dianchejie.cn

[Q41] 多表连接
来源：http://qpj.aizwys.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qfg.ybcxt.top

JOIN users u ON u.id = o.user_id
来源：http://ajf.hysaishi.cn

JOIN products p ON p.id = o.product_id;
来源：http://emb.vqdsnc.cn

[Q42] 连接条件附加过滤
来源：http://jvc.yueranfly.top

SELECT u.name, o.amount FROM users u
来源：http://nzi.ctjpmb.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bvh.daria6918.cn

[Q43] 标量子查询
来源：http://mbj.shuidangran.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vhz.yueranfly.top

[Q44] IN 子查询
来源：http://bvi.daxiang520.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xxi.sxryk.cn

[Q45] EXISTS 判断存在
来源：http://jin.jqgfzy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gdk.fanxiaobao.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://itu.cucudq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sya.mhx1999.top

[Q47] 与平均值比较
来源：http://jmp.ehwqpu.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xci.jlsjyb.cn

[Q48] CTE 公用表表达式
来源：http://qdd.tianlin.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ovo.yongpay.top

SELECT * FROM t WHERE c > 5;
来源：http://fqw.shanyushiyangtech.top

[Q49] 更新单行
来源：http://eyv.wangshuangyany.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kfg.jlsjyb.cn

[Q50] 批量更新
来源：http://bls.vqdsnc.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fts.hnxiangtu.top

[Q51] 用子查询更新
来源：http://vqt.jqgfzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vwv.yvedp.cn

[Q52] 删除指定行
来源：http://ybv.daria6918.cn

DELETE FROM users WHERE id = 10;
来源：http://hku.hnqzz.top

[Q53] 按条件删除
来源：http://gqu.guowangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qfq.guannengcc.top

[Q54] 清空表
来源：http://pqk.pengpengdd.cyou

TRUNCATE TABLE logs;
来源：http://ljs.jqgfzy.top

[Q55] 排名（并列占位）
来源：http://qov.zdbjq.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ijx.zdqjudy.top

[Q56] 密集排名（并列不占位）
来源：http://ewo.xuanzx.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fyb.chenlongwang.top

[Q57] 行号
来源：http://spf.jiagoushi.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ozf.yanxiufei.cn

[Q58] 累计求和
来源：http://cir.zhoulong.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://erh.yj202588.top

[Q59] 分组内累计
来源：http://tze.snrcjt.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://roi.zhongyouzk.top

[Q60] 取上一行 / 下一行
来源：http://iuo.ywan-chungtsiang.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://avo.tian-w.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wwp.nanxuanxn.top

[Q61] 移动平均
来源：http://vui.sysykeji.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uut.kuanghao11.cn

[Q62] 分组占比
来源：http://idm.gotoacloud.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wxc.guannengcc.top

[Q63] 开启事务
来源：http://ihw.vehdjk.com

START TRANSACTION;                -- 或 BEGIN
来源：http://ydk.epnwcf.com

[Q64] 提交事务
来源：http://xvp.gzhubu.top

COMMIT;
来源：http://cjc.nwbrower.top

[Q65] 回滚事务
来源：http://fwm.yueranfly.top

ROLLBACK;
来源：http://lgr.tianlin.xyz

[Q66] 行锁查询
来源：http://vnh.316326.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wsg.hfpthk.cn

[Q67] 设置隔离级别
来源：http://fua.snrcjt.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bvt.cucudq.cn

[Q68] 保存点
来源：http://nla.ywan-chungtsiang.top

SAVEPOINT sp1;
来源：http://cjb.chenzaomai.com

ROLLBACK TO sp1;
来源：http://cuh.tanke756.top

[Q69] 查看执行计划
来源：http://wus.fengsongda.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hyr.yuanzhike.top

[Q70] 更新统计信息
来源：http://iib.yuanzhike.top

ANALYZE TABLE users;
来源：http://gkc.yj202588.top

[Q71] 查看建表语句
来源：http://jgg.yongpay.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ygb.tian-w.cn

[Q72] 查看索引
来源：http://rbx.fengsongda.top

SHOW INDEX FROM users;
来源：http://fgy.sufxvd.cn

[Q73] 查看表状态
来源：http://ess.ppjwa.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://utp.zhaomingkeji.xyz

[Q74] 强制使用索引
来源：http://zgv.yueranfly.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pnt.hfpthk.cn

[Q75] 日期格式化
来源：http://ybn.ywan-chungtsiang.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://egu.yongpay.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://alh.dianchejie.cn

[Q76] 按天统计
来源：http://epn.wangshuangyany.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wyc.yfazqb.com

[Q77] 时间加减
来源：http://ibx.jianghu66.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tim.hongshengwenyu.top


<!-- 参考信息 -->