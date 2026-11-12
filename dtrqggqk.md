代发 wailian999

TS:   // worker_threads 线程池
来源：http://lor.zhengqikj.top

Java: Executors.newFixedThreadPool(4)
来源：http://bhf.yuanzhike.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sqp.xuanzx.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kot.tanke756.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kie.gaohongyu789.top

[O03] 加锁保护共享数据
来源：http://lnr.yonumen.top

Py:   with lock: shared += 1
来源：http://hkl.xziqi.cn

PHP:  // 用 flock() 做文件锁
来源：http://ghz.fehbvm.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gcj.hnqzz.top

TS:   // 同 JS
来源：http://yxm.birdmap.top

Java: synchronized (this) { shared++; }
来源：http://wqf.yangfankeji.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wnb.daria6918.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://dev.fengsongda.top

C#:   lock (gate) { shared++; }
来源：http://mqt.shanyushiyangkeji.top

[O04] 定义异步函数并等待
来源：http://csu.smart0.xyz

Py:   async def f():⏎    await g()
来源：http://heu.haohaochexian.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zuu.fzhhl.top

JS:   async function f() { await g(); }
来源：http://abv.cashguo.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://bax.ivvv.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zsj.cucudq.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zlk.sufxvd.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pkh.chenzaomai.com

C#:   async Task F() { await G(); }
来源：http://ezz.chenlongwang.top

[O05] 并发执行并等待全部完成
来源：http://yni.meibo888.top

Py:   asyncio.gather(*tasks)
来源：http://mov.sweek.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ywm.yfazqb.com

JS:   await Promise.all(tasks)
来源：http://sma.gzhubu.top

TS:   await Promise.all(tasks)
来源：http://oaj.birdmap.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tat.birdmap.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mws.hcnkem.com

Ruby: threads.map(&:join)
来源：http://biw.yanxiufei.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://mgy.shangyingyoupin.top

[O06] 使用进程池
来源：http://bod.hnqzz.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bcy.xuetiantiany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lau.feifeiyinyue.top

JS:   // child_process / cluster 模块
来源：http://pqi.pengpengdd.cyou

TS:   // child_process / cluster 模块
来源：http://tzv.gogol.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cqo.cucudq.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nql.cdnleiting.top

Ruby: // fork 块
来源：http://amh.zhengqikj.top

C#:   Parallel.For
来源：http://pcl.mhx1999.top

================================================================================
来源：http://kjt.fanxiaobao.xyz

P. 常用工具函数
来源：http://xqm.hongshengwenyu.top

================================================================================
来源：http://iur.yanxiufei.cn

[P01] 生成 UUID
来源：http://kkz.shzxlz.cn

Py:   str(uuid.uuid4())
来源：http://utl.yuxming.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://iqd.smart0.xyz

JS:   crypto.randomUUID()
来源：http://gyc.xuetiantiany.cn

TS:   crypto.randomUUID()
来源：http://agm.yuanzhike.top

Java: UUID.randomUUID().toString()
来源：http://qua.nanxuanxn.top

Go:   // 用 github.com/google/uuid
来源：http://maz.cucudq.cn

Ruby: SecureRandom.uuid
来源：http://jfg.jinghuilouyu.cn

C#:   Guid.NewGuid().ToString()
来源：http://xxq.zhengqikj.top

[P02] MD5 / SHA256 摘要
来源：http://dkj.zhengqikj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wll.ctjpmb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://vjv.uphjek.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bcm.jiagoushi.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wro.nanxinkj.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zxs.havefunace.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dmu.zhiwuduotai.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://exu.52xcode.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iot.xinyue.icu

[P03] 生成短随机字符串
来源：http://gaq.svipenyu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://que.havefunace.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dhn.zhijiandao.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cfu.fktsv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dmx.cucudq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ufk.snrcjt.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qwp.bjfxy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://auv.zdqjudy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ljx.gotoacloud.top

[P04] 求长度
来源：http://ral.svipenyu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ldy.0kj1m.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qjo.mhx1999.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bqr.mhx1999.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bvw.wangshuangyany.cn

Java: list.size();  map.size();  s.length()
来源：http://aol.dashuyun.cn

Go:   len(arr);  len(m)
来源：http://qzz.hnqzz.top

Ruby: x.length;  x.size
来源：http://kuh.yj20258.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://kox.jyoumei.cn

[P05] 判断两个对象内容是否相等
来源：http://jes.hesvh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://nvc.bbcook.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ygp.hcnkem.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fcf.kuanghao11.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yfi.quarkkingdee.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://koq.svipenyu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://php.aizwys.cn

Ruby: a == b
来源：http://rys.xingfuxueyuan.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pqg.yfazqb.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://deq.yuanzhike.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uob.hfpthk.cn

PHP:  if (empty($x)) {}
来源：http://sej.zdbjq.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dvs.xylfe.cn

TS:   if (x == null) {}
来源：http://fgp.andypj.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://jzv.tarul.cn

Go:   if x == nil {}
来源：http://qpo.gogol.net.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fey.zhiwuduotai.top

C#:   if (x is null) {}
来源：http://qgd.yuanzhike.top

[P07] 防抖与节流
来源：http://bux.cashguo.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xpp.ppjwa.cn

PHP:  // 手写时间戳比较
来源：http://pfx.sxryk.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kjn.yongpay.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jdi.hysaishi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dac.aizwys.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ocq.havefunace.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://nmc.shanyushiyangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mkw.gogol.net.cn

[P08] 处理浮点精度问题
来源：http://mtk.jinqigufen.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ozj.hywenlv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yar.jinghuilouyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jak.xziqi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ptk.guannengcc.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dww.zhixingplan.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nle.yj202588.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qfp.chenjidiqi.icu

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ije.gogol.net.cn

================================================================================
来源：http://edi.hywenlv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://eli.jyoumei.cn

================================================================================
来源：http://hyn.chenjidiqi.icu

[Q01] 创建表
来源：http://oqh.ivvv.top

CREATE TABLE users (
来源：http://lui.cqqwz.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cps.bbcook.cn

name VARCHAR(50) NOT NULL,
来源：http://ptv.52xcode.cn

email VARCHAR(100) UNIQUE,
来源：http://vlq.zdbjq.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uld.hammf.cn

);
来源：http://fig.wangdashe.top

[Q02] 创建带外键的表
来源：http://pqi.hywenlv.cn

CREATE TABLE orders (
来源：http://edt.epnwcf.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zab.kuanghao11.cn

user_id INT NOT NULL,
来源：http://tep.daxiang520.top

amount DECIMAL(10, 2),
来源：http://vra.nwbrower.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ovq.epnwcf.com

);
来源：http://dpk.gzhubu.top

[Q03] 增加列
来源：http://nbk.tian-w.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nqq.hnqzz.top

[Q04] 修改列类型
来源：http://cqg.zhijiandao.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gob.yueranfly.top

[Q05] 重命名列
来源：http://nkh.fanxiaobao.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wyl.yuxming.cn

[Q06] 删除列
来源：http://miy.daxiang520.top

ALTER TABLE users DROP COLUMN age;
来源：http://niz.cheryme.top

[Q07] 删除表
来源：http://cfc.hywenlv.cn

DROP TABLE IF EXISTS orders;
来源：http://mkd.haohaochexian.top

[Q08] 创建普通索引
来源：http://ceu.zhengqikj.top

CREATE INDEX idx_users_email ON users(email);
来源：http://cwz.hcnkem.com

[Q09] 创建唯一索引
来源：http://mxv.tian-w.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ohh.fengsongda.top

[Q10] 插入单行
来源：http://qlw.c1oappe.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ovk.hnqzz.top

[Q11] 一次插入多行
来源：http://ezt.vqdsnc.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://otb.snrcjt.cn

[Q12] 插入后取自增 ID
来源：http://arc.sufxvd.cn

INSERT INTO users (name) VALUES ('C');
来源：http://dat.dashuyun.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yav.sxryk.cn

[Q13] 忽略重复插入
来源：http://ine.jianghu66.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yua.havefunace.top

[Q14] 存在则更新（upsert）
来源：http://nay.ydzc1.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sfi.gotoacloud.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cow.fehbvm.com

[Q15] 查询全部
来源：http://ume.ydjk.org.cn

SELECT * FROM users;
来源：http://oli.zhengqikj.top

[Q16] 查询指定列
来源：http://wfz.nwbrower.top

SELECT id, name FROM users;
来源：http://uad.havefunace.top

[Q17] 条件查询
来源：http://xxu.yfazqb.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hje.fanxiaobao.xyz

[Q18] 模糊匹配
来源：http://wpx.svipenyu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jre.svipenyu.cn

[Q19] 范围查询
来源：http://imb.cqqwz.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://htm.feifeiyinyue.top

[Q20] IN 列表
来源：http://atj.jinyuanbaomall.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xpg.ywan-chungtsiang.top

[Q21] 空值判断
来源：http://ran.nanxinkj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://lsq.cashguo.top

[Q22] 排序
来源：http://dry.shuidangran.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lly.hywenlv.cn

[Q23] 分页
来源：http://cxn.ctjpmb.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mrf.ppjwa.cn

[Q24] 去重
来源：http://hdh.jyoumei.cn

SELECT DISTINCT city FROM users;
来源：http://awi.yj20258.top

[Q25] 只取前 N 条
来源：http://yib.yanxiufei.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://paa.cashguo.top

[Q26] 计数
来源：http://lgs.havefunace.top

SELECT COUNT(*) FROM users;
来源：http://pii.hcnkem.com

[Q27] 条件计数
来源：http://wrc.nwbrower.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nhz.gaohongyu789.top

[Q28] 求和与平均
来源：http://rwi.gzhubu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jwt.haohaochexian.top

[Q29] 最大最小值
来源：http://pee.cheryme.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://tqx.jinghuilouyu.cn

[Q30] 分组统计
来源：http://jtd.9152youxi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wjy.cqqwz.cn

[Q31] 分组后过滤
来源：http://woq.52xcode.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zyy.zdqjudy.top

[Q32] 分组拼接字符串
来源：http://zuu.sjlbkw.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jqe.sweek.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://euc.yueranfly.top

[Q33] 多列分组
来源：http://pis.bbcook.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zng.meibo888.top

[Q34] 每组取第一条
来源：http://nzu.tian-w.cn

SELECT * FROM (
来源：http://zdc.yueranfly.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://asn.birdmap.top

) t WHERE rn = 1;
来源：http://uof.hnxiangtu.top

[Q35] 内连接
来源：http://yxd.dianchejie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ttn.fanxiaobao.xyz

[Q36] 左连接
来源：http://eed.vehdjk.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jul.jyoumei.cn

[Q37] 右连接
来源：http://kpm.sweek.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gxi.jinghuilouyu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://nry.tian-w.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blq.ctjpmb.com

[Q39] 自连接（查上下级）
来源：http://tzm.pengpengdd.cyou

SELECT e.name, m.name AS manager FROM employees e
来源：http://kce.316326.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lkc.ivvv.top

[Q40] 交叉连接（笛卡尔积）
来源：http://rwz.tian-w.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zxm.svipenyu.cn

[Q41] 多表连接
来源：http://opn.pengpengdd.cyou

SELECT o.id, u.name, p.title FROM orders o
来源：http://lnn.sweek.top

JOIN users u ON u.id = o.user_id
来源：http://pvt.yfazqb.com

JOIN products p ON p.id = o.product_id;
来源：http://vdg.jianghu66.top

[Q42] 连接条件附加过滤
来源：http://ctk.ehwqpu.com

SELECT u.name, o.amount FROM users u
来源：http://vrr.pengpengdd.cyou

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vfl.zhaomingkeji.xyz

[Q43] 标量子查询
来源：http://lok.hammf.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mkr.hcnkem.com

[Q44] IN 子查询
来源：http://kcm.quarkkingdee.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uas.jqgufenzy.top

[Q45] EXISTS 判断存在
来源：http://xeb.fanxiaobao.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pkf.andypj.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://pff.ydjk.org.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://knh.nanxuanxn.top

[Q47] 与平均值比较
来源：http://vue.gogol.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://eeq.yanxiufei.cn

[Q48] CTE 公用表表达式
来源：http://jij.jyoumei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mqt.yfazqb.com

SELECT * FROM t WHERE c > 5;
来源：http://fga.aizwys.cn

[Q49] 更新单行
来源：http://tpu.pengpengdd.cyou

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tnc.meibo888.top

[Q50] 批量更新
来源：http://zvu.fktsv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wkx.hammf.cn

[Q51] 用子查询更新
来源：http://xno.hywenlv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://isp.hnxiangtu.top

[Q52] 删除指定行
来源：http://vhz.cashguo.top

DELETE FROM users WHERE id = 10;
来源：http://unj.yongpay.top

[Q53] 按条件删除
来源：http://hnd.ydjk.org.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rtq.sxryk.cn

[Q54] 清空表
来源：http://jox.svipenyu.cn

TRUNCATE TABLE logs;
来源：http://frp.hnqzz.top

[Q55] 排名（并列占位）
来源：http://oip.cheryme.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yvs.snrcjt.cn

[Q56] 密集排名（并列不占位）
来源：http://mjr.hcnkem.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://apo.shzxlz.cn

[Q57] 行号
来源：http://vkm.ctjpmb.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zqo.pycfn.com

[Q58] 累计求和
来源：http://awi.dianchejie.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://itk.jqgufenzy.top

[Q59] 分组内累计
来源：http://gkm.xylfe.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kog.gzhubu.top

[Q60] 取上一行 / 下一行
来源：http://wgi.cqqwz.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hsb.wangshuangyany.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blc.mhx1999.top

[Q61] 移动平均
来源：http://ydn.cucudq.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ynb.xylfe.cn

[Q62] 分组占比
来源：http://ifp.shanyushiyangtech.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://clx.zhixingplan.top

[Q63] 开启事务
来源：http://gpf.shuidangran.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ccc.epnwcf.com

[Q64] 提交事务
来源：http://mzo.cdnleiting.top

COMMIT;
来源：http://izn.fktsv.cn

[Q65] 回滚事务
来源：http://zng.tian-w.cn

ROLLBACK;
来源：http://kxa.zhiwuduotai.top

[Q66] 行锁查询
来源：http://tex.epnwcf.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://prr.yonumen.top

[Q67] 设置隔离级别
来源：http://itr.vqdsnc.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vsq.sufxvd.cn

[Q68] 保存点
来源：http://wga.ydjk.org.cn

SAVEPOINT sp1;
来源：http://tia.aizwys.cn

ROLLBACK TO sp1;
来源：http://wwh.aizwys.cn

[Q69] 查看执行计划
来源：http://mcb.zhaomingkeji.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://auv.ybcxt.top

[Q70] 更新统计信息
来源：http://rwa.hammf.cn

ANALYZE TABLE users;
来源：http://zan.aibaodan.cn

[Q71] 查看建表语句
来源：http://hon.vehdjk.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tge.yj20258888.top

[Q72] 查看索引
来源：http://buh.epnwcf.com

SHOW INDEX FROM users;
来源：http://nsf.bjfxy.top

[Q73] 查看表状态
来源：http://gas.fengsongda.top

SHOW TABLE STATUS LIKE 'users';
来源：http://swf.daria6918.cn

[Q74] 强制使用索引
来源：http://kmh.zdbjq.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://och.yvedp.cn

[Q75] 日期格式化
来源：http://xaw.jiagoushi.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tbw.ehwqpu.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zgh.52xcode.cn

[Q76] 按天统计
来源：http://jal.ywan-chungtsiang.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://htt.hnxiangtu.top

[Q77] 时间加减
来源：http://yvj.uphjek.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bmc.hesvh.cn

[Q78] 当前时间
来源：http://ucr.zdbjq.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dnz.sjlbkw.cn

[Q79] 字符串拼接
来源：http://aej.aizwys.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ikm.vqdsnc.cn


<!-- 参考信息 -->