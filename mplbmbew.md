代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://aqe.yuanzhike.top

Go:   go f()
来源：http://gbh.yangfankeji.com

Ruby: Thread.new { f }
来源：http://rxu.ctjpmb.com

C#:   Task.Run(() => F());
来源：http://pvu.zhongyouzk.top

[O02] 使用线程池
来源：http://xtl.xuanzx.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fkv.jqgufenzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jkr.shuidangran.top

JS:   // worker_threads 线程池
来源：http://xnx.hcnkem.com

TS:   // worker_threads 线程池
来源：http://poo.epnwcf.com

Java: Executors.newFixedThreadPool(4)
来源：http://aru.fktsv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sjc.snrcjt.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xpt.cheryme.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xka.yuxming.cn

[O03] 加锁保护共享数据
来源：http://pen.jyoumei.cn

Py:   with lock: shared += 1
来源：http://fhm.dianchejie.cn

PHP:  // 用 flock() 做文件锁
来源：http://lel.chenzaomai.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fvf.ehwqpu.com

TS:   // 同 JS
来源：http://ogx.smart0.xyz

Java: synchronized (this) { shared++; }
来源：http://efk.nanxuanxn.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zax.ppjwa.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xul.hnqzz.top

C#:   lock (gate) { shared++; }
来源：http://sbd.ppjwa.cn

[O04] 定义异步函数并等待
来源：http://wuy.chenlongwang.top

Py:   async def f():⏎    await g()
来源：http://jbo.jinqigfzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kvy.jinyuanbaomall.cn

JS:   async function f() { await g(); }
来源：http://hbt.cucudq.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mor.52xcode.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://goi.yongpay.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sdq.yvedp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ejm.xingfuxueyuan.xyz

C#:   async Task F() { await G(); }
来源：http://grc.zhoulong.xyz

[O05] 并发执行并等待全部完成
来源：http://ske.ydjk.org.cn

Py:   asyncio.gather(*tasks)
来源：http://ydz.shanyushiyangtech.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://czu.jqgfzy.top

JS:   await Promise.all(tasks)
来源：http://ywn.zhijiandao.cn

TS:   await Promise.all(tasks)
来源：http://gkg.zdqjudy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hqk.ctjpmb.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dac.xylfe.cn

Ruby: threads.map(&:join)
来源：http://ett.52xcode.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://lzc.zhaomingkeji.xyz

[O06] 使用进程池
来源：http://iju.hcnkem.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lru.yj20258888.top

PHP:  // pcntl_fork 或多进程队列
来源：http://vyd.hysaishi.cn

JS:   // child_process / cluster 模块
来源：http://ymm.ctjpmb.com

TS:   // child_process / cluster 模块
来源：http://abl.jqgufenzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tim.ybcxt.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://idi.fehbvm.com

Ruby: // fork 块
来源：http://xwe.yueranfly.top

C#:   Parallel.For
来源：http://mbi.sufxvd.cn

================================================================================
来源：http://qka.aibaodan.cn

P. 常用工具函数
来源：http://cta.yongpay.top

================================================================================
来源：http://jyg.dianchejie.cn

[P01] 生成 UUID
来源：http://pvj.xingfuxueyuan.xyz

Py:   str(uuid.uuid4())
来源：http://gcg.52xcode.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jun.zdbjq.cn

JS:   crypto.randomUUID()
来源：http://zdd.hysaishi.cn

TS:   crypto.randomUUID()
来源：http://frq.epnwcf.com

Java: UUID.randomUUID().toString()
来源：http://tii.jinqigufen.top

Go:   // 用 github.com/google/uuid
来源：http://dnd.ydzc1.top

Ruby: SecureRandom.uuid
来源：http://ubz.jianghu66.top

C#:   Guid.NewGuid().ToString()
来源：http://gna.ctjpmb.com

[P02] MD5 / SHA256 摘要
来源：http://jcg.zycfv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dwx.tianlin.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://rrq.jinqigufen.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nby.ivvv.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ufu.pengpengdd.cyou

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gok.ppjwa.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wgo.jinghuilouyu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tpa.iojbl.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uld.yvedp.cn

[P03] 生成短随机字符串
来源：http://vxt.zhixingplan.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://waj.zhixingplan.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ftm.xinyue.icu

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qrg.cheryme.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zkv.yongpay.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qjp.aizwys.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dli.gogol.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wka.cheryme.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ymd.gzhubu.top

[P04] 求长度
来源：http://fwe.fengsongda.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ipk.316326.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sii.xingfuxueyuan.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wps.havefunace.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://btz.zdbjq.cn

Java: list.size();  map.size();  s.length()
来源：http://ofq.fzhhl.top

Go:   len(arr);  len(m)
来源：http://njg.kuanghao11.cn

Ruby: x.length;  x.size
来源：http://foz.wangdashe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://tiw.ctjpmb.com

[P05] 判断两个对象内容是否相等
来源：http://him.daxiang520.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://kxo.ydzc1.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ywo.hesvh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bww.snrcjt.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rni.xuetiantiany.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yvs.yj202588.top

Go:   reflect.DeepEqual(a, b)
来源：http://xel.tanke756.top

Ruby: a == b
来源：http://bdw.c1oappe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fad.zdqjudy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lrd.vqdsnc.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dmh.jlsjyb.cn

PHP:  if (empty($x)) {}
来源：http://ymn.hnqzz.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ycr.zdqjudy.top

TS:   if (x == null) {}
来源：http://xsr.xylfe.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jgn.yanxiufei.cn

Go:   if x == nil {}
来源：http://nry.svipenyu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gld.aibaodan.cn

C#:   if (x is null) {}
来源：http://cdh.hywenlv.cn

[P07] 防抖与节流
来源：http://dnb.yj20258888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ujk.hesvh.cn

PHP:  // 手写时间戳比较
来源：http://uto.jinqigfzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tvn.bbcook.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ztk.shanyushiyangtech.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://luh.jlsjyb.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mhi.ivvv.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://vjy.ehwqpu.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xnk.yj20258.top

[P08] 处理浮点精度问题
来源：http://kwb.sjlbkw.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pcn.ehwqpu.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rsk.yueranfly.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://upl.gaohongyu789.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vqa.fehbvm.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ydd.iojbl.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xgq.sjlbkw.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sko.xylfe.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fjy.dashuyun.cn

================================================================================
来源：http://zhv.snrcjt.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mgf.zhijiandao.cn

================================================================================
来源：http://eke.c1oappe.top

[Q01] 创建表
来源：http://rzb.jiagoushi.top

CREATE TABLE users (
来源：http://bqj.xuetiantiany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jej.shzxlz.cn

name VARCHAR(50) NOT NULL,
来源：http://ugq.shanyushiyangkeji.top

email VARCHAR(100) UNIQUE,
来源：http://sgx.dashuyun.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vxp.birdmap.top

);
来源：http://cvy.xylfe.cn

[Q02] 创建带外键的表
来源：http://frl.gogol.net.cn

CREATE TABLE orders (
来源：http://dcp.shanyushiyangtech.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qcx.havefunace.top

user_id INT NOT NULL,
来源：http://ngq.redwolf501.top

amount DECIMAL(10, 2),
来源：http://emu.yfazqb.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nen.fanxiaobao.xyz

);
来源：http://wzb.bjfxy.top

[Q03] 增加列
来源：http://rbh.redwolf501.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wja.wangdashe.top

[Q04] 修改列类型
来源：http://chy.sweek.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hpo.meibo888.top

[Q05] 重命名列
来源：http://tmj.shangyingyoupin.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zld.yvedp.cn

[Q06] 删除列
来源：http://fkm.andypj.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://utu.cashguo.top

[Q07] 删除表
来源：http://kwa.tianlin.xyz

DROP TABLE IF EXISTS orders;
来源：http://mdh.dianchejie.cn

[Q08] 创建普通索引
来源：http://bqk.aizwys.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://gpb.zdbjq.cn

[Q09] 创建唯一索引
来源：http://ujn.zhoulong.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tix.nanxinkj.top

[Q10] 插入单行
来源：http://ovu.feifeiyinyue.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pwn.ywan-chungtsiang.top

[Q11] 一次插入多行
来源：http://pmu.cqqwz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://she.zhongyouzk.top

[Q12] 插入后取自增 ID
来源：http://hzg.iojbl.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yow.yj202588.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://htc.kuanghao11.cn

[Q13] 忽略重复插入
来源：http://ekd.tarul.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hkx.316326.xyz

[Q14] 存在则更新（upsert）
来源：http://kab.daria6918.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hzq.ivvv.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hps.ppjwa.cn

[Q15] 查询全部
来源：http://lpr.hongshengwenyu.top

SELECT * FROM users;
来源：http://frq.hfpthk.cn

[Q16] 查询指定列
来源：http://xsm.ydjk.org.cn

SELECT id, name FROM users;
来源：http://ndd.hammf.cn

[Q17] 条件查询
来源：http://fdp.zhixingplan.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ofq.shanyushiyangtech.top

[Q18] 模糊匹配
来源：http://mjx.hfpthk.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pmf.yuanzhike.top

[Q19] 范围查询
来源：http://ckx.zhijiandao.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://aap.hfpthk.cn

[Q20] IN 列表
来源：http://jpm.pycfn.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ahb.zhengqikj.top

[Q21] 空值判断
来源：http://elu.hesvh.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pjp.zhengqikj.top

[Q22] 排序
来源：http://zwf.wangdashe.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nit.ppjwa.cn

[Q23] 分页
来源：http://chs.smart0.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qpp.daria6918.cn

[Q24] 去重
来源：http://mfb.fehbvm.com

SELECT DISTINCT city FROM users;
来源：http://iqg.gaohongyu789.top

[Q25] 只取前 N 条
来源：http://ejk.bbcook.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://azs.zhoulong.xyz

[Q26] 计数
来源：http://ogu.redwolf501.top

SELECT COUNT(*) FROM users;
来源：http://fjb.redwolf501.top

[Q27] 条件计数
来源：http://apw.nanxuanxn.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zrl.hesvh.cn

[Q28] 求和与平均
来源：http://hdj.zhongyouzk.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rvt.bbcook.cn

[Q29] 最大最小值
来源：http://cvk.jinqigfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://lwp.fanxiaobao.xyz

[Q30] 分组统计
来源：http://thy.xuanzx.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pbs.yj202588.top

[Q31] 分组后过滤
来源：http://qnh.fengsongda.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rmn.uphjek.com

[Q32] 分组拼接字符串
来源：http://pmd.zhiwuduotai.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rnw.aibaodan.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uhv.gaohongyu789.top

[Q33] 多列分组
来源：http://wfq.sufxvd.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yus.zycfv.cn

[Q34] 每组取第一条
来源：http://pes.sysykeji.top

SELECT * FROM (
来源：http://fmi.shzxlz.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uoe.jinqigufen.top

) t WHERE rn = 1;
来源：http://spz.birdmap.top

[Q35] 内连接
来源：http://jou.sweek.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yut.zycfv.cn

[Q36] 左连接
来源：http://ljz.sysykeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://itl.xinyue.icu

[Q37] 右连接
来源：http://bgm.yj20258.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kng.nwbrower.top

[Q38] 全外连接（PostgreSQL）
来源：http://pwb.vehdjk.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hfq.tian-w.cn

[Q39] 自连接（查上下级）
来源：http://pci.fktsv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vex.9152youxi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://efx.yangfankeji.com

[Q40] 交叉连接（笛卡尔积）
来源：http://bms.52xcode.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://srh.nanxuanxn.top

[Q41] 多表连接
来源：http://crt.hnqzz.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://zlz.zhaomingkeji.xyz

JOIN users u ON u.id = o.user_id
来源：http://oxz.wangdashe.top

JOIN products p ON p.id = o.product_id;
来源：http://kwd.9152youxi.cn

[Q42] 连接条件附加过滤
来源：http://jed.jinqigufen.top

SELECT u.name, o.amount FROM users u
来源：http://afo.ydjk.org.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vtz.guannengcc.top

[Q43] 标量子查询
来源：http://uvp.redwolf501.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hdo.9152youxi.cn

[Q44] IN 子查询
来源：http://vwz.hnqzz.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nmy.uphjek.com

[Q45] EXISTS 判断存在
来源：http://tnw.yanxiufei.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wnl.yanxiufei.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ynf.daria6918.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vor.iojbl.cn

[Q47] 与平均值比较
来源：http://sxi.meibo888.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://brh.bjfxy.top

[Q48] CTE 公用表表达式
来源：http://zhf.zhaomingkeji.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jxu.kuanghao11.cn

SELECT * FROM t WHERE c > 5;
来源：http://hzo.gaohongyu789.top

[Q49] 更新单行
来源：http://wps.hammf.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kbb.ivvv.top

[Q50] 批量更新
来源：http://tdj.ppjwa.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yiq.mhx1999.top

[Q51] 用子查询更新
来源：http://lfs.jyoumei.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://upl.yongpay.top

[Q52] 删除指定行
来源：http://tgs.hywenlv.cn

DELETE FROM users WHERE id = 10;
来源：http://kwb.ywan-chungtsiang.top

[Q53] 按条件删除
来源：http://lpt.hnxiangtu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sud.nanxuanxn.top

[Q54] 清空表
来源：http://ccy.zdbjq.cn

TRUNCATE TABLE logs;
来源：http://aad.snrcjt.cn

[Q55] 排名（并列占位）
来源：http://ovl.xylfe.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nlo.ehwqpu.com

[Q56] 密集排名（并列不占位）
来源：http://aau.yj20258.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://utt.fanxiaobao.xyz

[Q57] 行号
来源：http://wsd.c1oappe.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cof.chenzaomai.com

[Q58] 累计求和
来源：http://wyd.jyoumei.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jpi.cucudq.cn

[Q59] 分组内累计
来源：http://zxi.yj202588.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vty.chenlongwang.top

[Q60] 取上一行 / 下一行
来源：http://gid.feifeiyinyue.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uws.c1oappe.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ipl.tanke756.top

[Q61] 移动平均
来源：http://kcp.jinghuilouyu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ovl.jiagoushi.top

[Q62] 分组占比
来源：http://ken.jinyuanbaomall.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://eud.quarkkingdee.top

[Q63] 开启事务
来源：http://exh.quarkkingdee.top

START TRANSACTION;                -- 或 BEGIN
来源：http://pkw.yj20258.top

[Q64] 提交事务
来源：http://oqx.guowangkeji.top

COMMIT;
来源：http://med.sufxvd.cn

[Q65] 回滚事务
来源：http://goj.nanxuanxn.top

ROLLBACK;
来源：http://ksb.zhengqikj.top

[Q66] 行锁查询
来源：http://dly.aizwys.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://znx.zdbjq.cn

[Q67] 设置隔离级别
来源：http://wlr.birdmap.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ors.nwbrower.top

[Q68] 保存点
来源：http://jgu.yueranfly.top

SAVEPOINT sp1;
来源：http://dsc.ivvv.top

ROLLBACK TO sp1;
来源：http://rgb.hesvh.cn

[Q69] 查看执行计划
来源：http://pck.aibaodan.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vae.cheryme.top

[Q70] 更新统计信息
来源：http://eoy.yanxiufei.cn

ANALYZE TABLE users;
来源：http://trz.nanxuanxn.top

[Q71] 查看建表语句
来源：http://ctd.yongpay.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mnd.chenlongwang.top

[Q72] 查看索引
来源：http://vby.9152youxi.cn

SHOW INDEX FROM users;
来源：http://brs.xinyue.icu

[Q73] 查看表状态
来源：http://afv.ybcxt.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rmg.sjlbkw.cn

[Q74] 强制使用索引
来源：http://tro.wangdashe.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nsm.yj20258888.top

[Q75] 日期格式化
来源：http://dru.vqdsnc.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zdt.iojbl.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uwu.hnqzz.top


<!-- 参考信息 -->