代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://uye.svipenyu.cn

Go:   go f()
来源：http://eqj.nwbrower.top

Ruby: Thread.new { f }
来源：http://kcd.iojbl.cn

C#:   Task.Run(() => F());
来源：http://osi.havefunace.top

[O02] 使用线程池
来源：http://nsf.fzhhl.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dqs.birdmap.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sli.mhx1999.top

JS:   // worker_threads 线程池
来源：http://zfy.bjfxy.top

TS:   // worker_threads 线程池
来源：http://aeg.ppjwa.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kwp.tian-w.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ewg.xinyue.icu

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://znw.zdbjq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ylq.zdqjudy.top

[O03] 加锁保护共享数据
来源：http://pnx.kuanghao11.cn

Py:   with lock: shared += 1
来源：http://aml.ybcxt.top

PHP:  // 用 flock() 做文件锁
来源：http://sed.zhoulong.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vcm.haohaochexian.top

TS:   // 同 JS
来源：http://evv.yj202588.top

Java: synchronized (this) { shared++; }
来源：http://yzy.hywenlv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wte.redwolf501.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://yic.jianghu66.top

C#:   lock (gate) { shared++; }
来源：http://imh.xinyue.icu

[O04] 定义异步函数并等待
来源：http://met.xziqi.cn

Py:   async def f():⏎    await g()
来源：http://jlp.jiagoushi.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xbe.daxiang520.top

JS:   async function f() { await g(); }
来源：http://uxg.pengpengdd.cyou

TS:   async function f(): Promise<void> { await g(); }
来源：http://wyd.yueranfly.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sfo.gaohongyu789.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dfq.chenjidiqi.icu

Ruby: # 用 Fiber 或 async gem
来源：http://jvk.yuanzhike.top

C#:   async Task F() { await G(); }
来源：http://vst.nanxuanxn.top

[O05] 并发执行并等待全部完成
来源：http://wtw.fengsongda.top

Py:   asyncio.gather(*tasks)
来源：http://ajq.yj20258888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jwp.hesvh.cn

JS:   await Promise.all(tasks)
来源：http://qav.9152youxi.cn

TS:   await Promise.all(tasks)
来源：http://gly.cqqwz.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jgh.yuanzhike.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://czp.xingfuxueyuan.xyz

Ruby: threads.map(&:join)
来源：http://tob.cashguo.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ayr.hesvh.cn

[O06] 使用进程池
来源：http://qpl.yanxiufei.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rkk.smart0.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://nlf.snrcjt.cn

JS:   // child_process / cluster 模块
来源：http://wtg.gotoacloud.top

TS:   // child_process / cluster 模块
来源：http://qlu.cashguo.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gib.pengpengdd.cyou

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jox.ivvv.top

Ruby: // fork 块
来源：http://sle.havefunace.top

C#:   Parallel.For
来源：http://ugm.gzhubu.top

================================================================================
来源：http://bhz.zhengqikj.top

P. 常用工具函数
来源：http://lyn.c1oappe.top

================================================================================
来源：http://yul.ydzc1.top

[P01] 生成 UUID
来源：http://lob.andypj.xyz

Py:   str(uuid.uuid4())
来源：http://inq.c1oappe.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://orb.meibo888.top

JS:   crypto.randomUUID()
来源：http://zic.epnwcf.com

TS:   crypto.randomUUID()
来源：http://rfx.hysaishi.cn

Java: UUID.randomUUID().toString()
来源：http://ewi.cucudq.cn

Go:   // 用 github.com/google/uuid
来源：http://ehm.yuxming.cn

Ruby: SecureRandom.uuid
来源：http://vka.gotoacloud.top

C#:   Guid.NewGuid().ToString()
来源：http://qzo.hesvh.cn

[P02] MD5 / SHA256 摘要
来源：http://afc.bbcook.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zva.cqqwz.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ryl.hesvh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ban.bjfxy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mvf.yuxming.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kup.wangshuangyany.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jjj.jinqigfzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zmh.zhijiandao.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uke.hfpthk.cn

[P03] 生成短随机字符串
来源：http://xge.quarkkingdee.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://teg.daria6918.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bwt.guannengcc.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fgw.jiagoushi.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ofw.52xcode.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://oir.fktsv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://owa.cucudq.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vhm.sxryk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ghq.cheryme.top

[P04] 求长度
来源：http://qlw.nanxuanxn.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vcw.ctjpmb.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jri.yueranfly.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://spr.mhx1999.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://can.gaohongyu789.top

Java: list.size();  map.size();  s.length()
来源：http://jnh.andypj.xyz

Go:   len(arr);  len(m)
来源：http://pvd.snrcjt.cn

Ruby: x.length;  x.size
来源：http://gue.fengsongda.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://hpj.shangyingyoupin.top

[P05] 判断两个对象内容是否相等
来源：http://cmk.nanxuanxn.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://wan.snrcjt.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hrq.jinqigfzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://otc.zhoulong.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lem.hammf.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://aee.fzhhl.top

Go:   reflect.DeepEqual(a, b)
来源：http://nvj.9152youxi.cn

Ruby: a == b
来源：http://ifn.gotoacloud.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pap.daxiang520.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tpy.wangshuangyany.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bis.mhx1999.top

PHP:  if (empty($x)) {}
来源：http://sqb.quarkkingdee.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fum.yanxiufei.cn

TS:   if (x == null) {}
来源：http://uht.yonumen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://tub.gotoacloud.top

Go:   if x == nil {}
来源：http://udi.yj20258.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://epp.yj20258.top

C#:   if (x is null) {}
来源：http://xkp.havefunace.top

[P07] 防抖与节流
来源：http://yrl.sweek.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zcd.jqgufenzy.top

PHP:  // 手写时间戳比较
来源：http://vkf.aibaodan.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dje.pengpengdd.cyou

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mny.redwolf501.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cmi.wangdashe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pwp.nwbrower.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://kmf.cdnleiting.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vej.xingfuxueyuan.xyz

[P08] 处理浮点精度问题
来源：http://csp.yueranfly.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://oyl.sjlbkw.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xdb.0kj1m.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://moa.ywan-chungtsiang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sju.fengsongda.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hvi.cheryme.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tiq.hammf.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ers.yuxming.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qdy.sxryk.cn

================================================================================
来源：http://pwm.yj20258888.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ojv.ppjwa.cn

================================================================================
来源：http://eck.hfpthk.cn

[Q01] 创建表
来源：http://nha.ywan-chungtsiang.top

CREATE TABLE users (
来源：http://eho.cqqwz.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vip.iojbl.cn

name VARCHAR(50) NOT NULL,
来源：http://fnt.jqgufenzy.top

email VARCHAR(100) UNIQUE,
来源：http://toe.yanxiufei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://crw.smart0.xyz

);
来源：http://twk.gzhubu.top

[Q02] 创建带外键的表
来源：http://xgz.yj202588.top

CREATE TABLE orders (
来源：http://lix.cdnleiting.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rfg.ctjpmb.com

user_id INT NOT NULL,
来源：http://oll.zhoulong.xyz

amount DECIMAL(10, 2),
来源：http://xgp.fktsv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tbx.yueranfly.top

);
来源：http://unz.shzxlz.cn

[Q03] 增加列
来源：http://cop.hcnkem.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gtg.iojbl.cn

[Q04] 修改列类型
来源：http://azz.daxiang520.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xry.yongpay.top

[Q05] 重命名列
来源：http://tey.shzxlz.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fep.shanyushiyangkeji.top

[Q06] 删除列
来源：http://lnl.hnqzz.top

ALTER TABLE users DROP COLUMN age;
来源：http://wzl.meibo888.top

[Q07] 删除表
来源：http://jtp.jinqigfzy.top

DROP TABLE IF EXISTS orders;
来源：http://rgr.yuanzhike.top

[Q08] 创建普通索引
来源：http://bde.hongshengwenyu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://hum.kuanghao11.cn

[Q09] 创建唯一索引
来源：http://giu.xingfuxueyuan.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jjm.daxiang520.top

[Q10] 插入单行
来源：http://upp.uphjek.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vvx.hysaishi.cn

[Q11] 一次插入多行
来源：http://zra.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hsi.daxiang520.top

[Q12] 插入后取自增 ID
来源：http://gbz.zdbjq.cn

INSERT INTO users (name) VALUES ('C');
来源：http://uyr.jinghuilouyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wpq.jinqigfzy.top

[Q13] 忽略重复插入
来源：http://tij.jyoumei.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hzo.sysykeji.top

[Q14] 存在则更新（upsert）
来源：http://jnt.zycfv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lmx.dashuyun.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ydq.gotoacloud.top

[Q15] 查询全部
来源：http://yqh.sufxvd.cn

SELECT * FROM users;
来源：http://cke.nanxuanxn.top

[Q16] 查询指定列
来源：http://rfq.smart0.xyz

SELECT id, name FROM users;
来源：http://zdb.jlsjyb.cn

[Q17] 条件查询
来源：http://aaf.gotoacloud.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nim.zhiwuduotai.top

[Q18] 模糊匹配
来源：http://kcg.meibo888.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wih.jqgfzy.top

[Q19] 范围查询
来源：http://oyy.ivvv.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://afr.hammf.cn

[Q20] IN 列表
来源：http://ltc.jinqigufen.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qfz.fanxiaobao.xyz

[Q21] 空值判断
来源：http://toj.zhoulong.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://lvv.hongshengwenyu.top

[Q22] 排序
来源：http://rym.tianlin.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hxu.wangdashe.top

[Q23] 分页
来源：http://oqi.gotoacloud.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hby.daria6918.cn

[Q24] 去重
来源：http://vfy.daria6918.cn

SELECT DISTINCT city FROM users;
来源：http://vxs.tianlin.xyz

[Q25] 只取前 N 条
来源：http://ial.zhiwuduotai.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ydp.tian-w.cn

[Q26] 计数
来源：http://gpr.tarul.cn

SELECT COUNT(*) FROM users;
来源：http://exy.chenjidiqi.icu

[Q27] 条件计数
来源：http://pcj.ywan-chungtsiang.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zxs.cdnleiting.top

[Q28] 求和与平均
来源：http://odk.jqgfzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fmg.vehdjk.com

[Q29] 最大最小值
来源：http://uov.gaohongyu789.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ovs.mhx1999.top

[Q30] 分组统计
来源：http://xye.9152youxi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dor.cheryme.top

[Q31] 分组后过滤
来源：http://ngm.jinqigufen.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vub.nwbrower.top

[Q32] 分组拼接字符串
来源：http://mir.ydjk.org.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uza.shzxlz.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dal.redwolf501.top

[Q33] 多列分组
来源：http://fhb.shangyingyoupin.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vkm.tianlin.xyz

[Q34] 每组取第一条
来源：http://ujt.hfpthk.cn

SELECT * FROM (
来源：http://yky.redwolf501.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ctm.epnwcf.com

) t WHERE rn = 1;
来源：http://bay.tanke756.top

[Q35] 内连接
来源：http://ahq.yonumen.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pqn.ydzc1.top

[Q36] 左连接
来源：http://yzs.sysykeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lvg.aibaodan.cn

[Q37] 右连接
来源：http://pgk.nanxinkj.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uqq.chenzaomai.com

[Q38] 全外连接（PostgreSQL）
来源：http://zas.birdmap.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vgh.ybcxt.top

[Q39] 自连接（查上下级）
来源：http://sne.gzhubu.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ruf.chenlongwang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ulu.cdnleiting.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zsq.feifeiyinyue.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fqq.dashuyun.cn

[Q41] 多表连接
来源：http://doh.sweek.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://fvs.kuanghao11.cn

JOIN users u ON u.id = o.user_id
来源：http://ius.yuxming.cn

JOIN products p ON p.id = o.product_id;
来源：http://ihe.ydzc1.top

[Q42] 连接条件附加过滤
来源：http://qpt.redwolf501.top

SELECT u.name, o.amount FROM users u
来源：http://slc.gotoacloud.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pxv.zhiwuduotai.top

[Q43] 标量子查询
来源：http://sns.nanxinkj.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qdm.sufxvd.cn

[Q44] IN 子查询
来源：http://sbl.chenzaomai.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mzz.gzhubu.top

[Q45] EXISTS 判断存在
来源：http://hsq.yangfankeji.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://guu.hfpthk.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qds.feifeiyinyue.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://htv.yuxming.cn

[Q47] 与平均值比较
来源：http://usx.yongpay.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://urt.ctjpmb.com

[Q48] CTE 公用表表达式
来源：http://tco.hongshengwenyu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ahg.zhiwuduotai.top

SELECT * FROM t WHERE c > 5;
来源：http://mar.havefunace.top

[Q49] 更新单行
来源：http://ghp.316326.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gpe.jqgfzy.top

[Q50] 批量更新
来源：http://kao.gzhubu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bkv.sufxvd.cn

[Q51] 用子查询更新
来源：http://srh.pycfn.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://txu.sysykeji.top

[Q52] 删除指定行
来源：http://ipo.fanxiaobao.xyz

DELETE FROM users WHERE id = 10;
来源：http://wdo.daxiang520.top

[Q53] 按条件删除
来源：http://agn.wangshuangyany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bvh.birdmap.top

[Q54] 清空表
来源：http://ome.xuanzx.com

TRUNCATE TABLE logs;
来源：http://gsz.xziqi.cn

[Q55] 排名（并列占位）
来源：http://oms.aizwys.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qxd.hfpthk.cn

[Q56] 密集排名（并列不占位）
来源：http://ghm.guowangkeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://goi.ydjk.org.cn

[Q57] 行号
来源：http://xfy.pengpengdd.cyou

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ghw.yj20258888.top

[Q58] 累计求和
来源：http://foo.zdqjudy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wbb.yj202588.top

[Q59] 分组内累计
来源：http://wgz.snrcjt.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yqc.jyoumei.cn

[Q60] 取上一行 / 下一行
来源：http://osl.ehwqpu.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://szy.yuxming.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tnm.jinqigufen.top

[Q61] 移动平均
来源：http://kme.xuetiantiany.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://icq.mhx1999.top

[Q62] 分组占比
来源：http://sxj.jqgfzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nxe.jinqigufen.top

[Q63] 开启事务
来源：http://git.dashuyun.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://roo.yuxming.cn

[Q64] 提交事务
来源：http://npl.bbcook.cn

COMMIT;
来源：http://cdx.shuidangran.top

[Q65] 回滚事务
来源：http://lfc.aizwys.cn

ROLLBACK;
来源：http://hpg.ivvv.top

[Q66] 行锁查询
来源：http://xhp.zhijiandao.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hum.hcnkem.com

[Q67] 设置隔离级别
来源：http://bko.jqgufenzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wmc.fanxiaobao.xyz

[Q68] 保存点
来源：http://ycy.cucudq.cn

SAVEPOINT sp1;
来源：http://klz.hongshengwenyu.top

ROLLBACK TO sp1;
来源：http://fic.hysaishi.cn

[Q69] 查看执行计划
来源：http://qsz.yongpay.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yeu.uphjek.com

[Q70] 更新统计信息
来源：http://asv.tianlin.xyz

ANALYZE TABLE users;
来源：http://thy.zhixingplan.top

[Q71] 查看建表语句
来源：http://nxt.snrcjt.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ksq.epnwcf.com

[Q72] 查看索引
来源：http://uvy.zhoulong.xyz

SHOW INDEX FROM users;
来源：http://zid.jlsjyb.cn

[Q73] 查看表状态
来源：http://owx.0kj1m.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hnr.hfpthk.cn

[Q74] 强制使用索引
来源：http://hbt.yongpay.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://pqg.hongshengwenyu.top

[Q75] 日期格式化
来源：http://ixe.vehdjk.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jmt.tarul.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wbp.dianchejie.cn


<!-- 参考信息 -->