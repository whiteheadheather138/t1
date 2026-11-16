代发 wailian999

[O02] 使用线程池
来源：http://zsl.dianchejie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lwe.zhiwuduotai.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ivy.quarkkingdee.top

JS:   // worker_threads 线程池
来源：http://enn.jinyuanbaomall.cn

TS:   // worker_threads 线程池
来源：http://ycy.quarkkingdee.top

Java: Executors.newFixedThreadPool(4)
来源：http://mam.zhongyouzk.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lgg.hywenlv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pol.chenzaomai.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ptk.yj202588.top

[O03] 加锁保护共享数据
来源：http://hsd.jqgufenzy.top

Py:   with lock: shared += 1
来源：http://uxf.svipenyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://zby.wangdashe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mmj.c1oappe.top

TS:   // 同 JS
来源：http://xhw.xziqi.cn

Java: synchronized (this) { shared++; }
来源：http://gwr.yfazqb.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sek.chenzaomai.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://fpa.xinyue.icu

C#:   lock (gate) { shared++; }
来源：http://sfd.ydjk.org.cn

[O04] 定义异步函数并等待
来源：http://bzh.xylfe.cn

Py:   async def f():⏎    await g()
来源：http://crv.hnxiangtu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://usx.sufxvd.cn

JS:   async function f() { await g(); }
来源：http://eip.kuanghao11.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dfm.dianchejie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fgx.yj20258.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://btr.vehdjk.com

Ruby: # 用 Fiber 或 async gem
来源：http://zze.shanyushiyangkeji.top

C#:   async Task F() { await G(); }
来源：http://rta.jlsjyb.cn

[O05] 并发执行并等待全部完成
来源：http://qxg.fengsongda.top

Py:   asyncio.gather(*tasks)
来源：http://hcx.tanke756.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lhr.shuidangran.top

JS:   await Promise.all(tasks)
来源：http://gon.zhengqikj.top

TS:   await Promise.all(tasks)
来源：http://teu.jinqigfzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lrn.chenzaomai.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nkm.yfazqb.com

Ruby: threads.map(&:join)
来源：http://etv.uphjek.com

C#:   await Task.WhenAll(t1, t2)
来源：http://nmi.shuidangran.top

[O06] 使用进程池
来源：http://itt.birdmap.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://llr.svipenyu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tis.yvedp.cn

JS:   // child_process / cluster 模块
来源：http://lvz.vehdjk.com

TS:   // child_process / cluster 模块
来源：http://mpa.hnxiangtu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xjg.yuxming.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zxy.hammf.cn

Ruby: // fork 块
来源：http://pii.cdnleiting.top

C#:   Parallel.For
来源：http://gys.yueranfly.top

================================================================================
来源：http://gvm.jinghuilouyu.cn

P. 常用工具函数
来源：http://khq.hesvh.cn

================================================================================
来源：http://nbh.yj202588.top

[P01] 生成 UUID
来源：http://olw.c1oappe.top

Py:   str(uuid.uuid4())
来源：http://snh.tanke756.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fle.dashuyun.cn

JS:   crypto.randomUUID()
来源：http://nbm.316326.xyz

TS:   crypto.randomUUID()
来源：http://ixz.ydzc1.top

Java: UUID.randomUUID().toString()
来源：http://sal.gzhubu.top

Go:   // 用 github.com/google/uuid
来源：http://knm.cdnleiting.top

Ruby: SecureRandom.uuid
来源：http://phs.sxryk.cn

C#:   Guid.NewGuid().ToString()
来源：http://aug.tianlin.xyz

[P02] MD5 / SHA256 摘要
来源：http://bzu.ppjwa.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://foh.redwolf501.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://yvo.nanxinkj.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oja.xuanzx.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wlj.hnxiangtu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qvq.zdbjq.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dqz.wangshuangyany.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jyr.snrcjt.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://oly.tanke756.top

[P03] 生成短随机字符串
来源：http://ihj.zhijiandao.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://aso.yueranfly.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oze.52xcode.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xsb.smart0.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wko.tianlin.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pdd.jiagoushi.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ict.52xcode.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://upz.kuanghao11.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://aze.sxryk.cn

[P04] 求长度
来源：http://bxw.dianchejie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tsf.zhoulong.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eyu.kuanghao11.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://khq.hcnkem.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tua.fanxiaobao.xyz

Java: list.size();  map.size();  s.length()
来源：http://ubx.zhengqikj.top

Go:   len(arr);  len(m)
来源：http://msc.aizwys.cn

Ruby: x.length;  x.size
来源：http://lcd.hysaishi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fxf.vehdjk.com

[P05] 判断两个对象内容是否相等
来源：http://nav.ydjk.org.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://duf.xuetiantiany.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://srg.pengpengdd.cyou

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://axj.hesvh.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eze.nanxinkj.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dmh.bjfxy.top

Go:   reflect.DeepEqual(a, b)
来源：http://wwh.xylfe.cn

Ruby: a == b
来源：http://yvl.ehwqpu.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nhf.daxiang520.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blm.316326.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mwg.haohaochexian.top

PHP:  if (empty($x)) {}
来源：http://moo.cucudq.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uld.fengsongda.top

TS:   if (x == null) {}
来源：http://gxy.sufxvd.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://dft.tian-w.cn

Go:   if x == nil {}
来源：http://vyd.tarul.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rzd.xinyue.icu

C#:   if (x is null) {}
来源：http://bui.zhiwuduotai.top

[P07] 防抖与节流
来源：http://bwh.xziqi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gfu.yueranfly.top

PHP:  // 手写时间戳比较
来源：http://udd.xuetiantiany.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://npk.zdqjudy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tdo.mhx1999.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sik.cqqwz.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://eco.cashguo.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://grg.yuxming.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://eqo.yuanzhike.top

[P08] 处理浮点精度问题
来源：http://hit.hesvh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mjk.dashuyun.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rto.jyoumei.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xwj.shuidangran.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://avh.ybcxt.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xus.ydzc1.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://idd.wangdashe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bjj.jqgfzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zzp.ctjpmb.com

================================================================================
来源：http://zxg.ydzc1.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qlh.svipenyu.cn

================================================================================
来源：http://hpd.cqqwz.cn

[Q01] 创建表
来源：http://siv.sjlbkw.cn

CREATE TABLE users (
来源：http://dix.snrcjt.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wbu.chenzaomai.com

name VARCHAR(50) NOT NULL,
来源：http://yeu.316326.xyz

email VARCHAR(100) UNIQUE,
来源：http://nhd.jlsjyb.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dqj.0kj1m.cn

);
来源：http://mnm.c1oappe.top

[Q02] 创建带外键的表
来源：http://jfr.shangyingyoupin.top

CREATE TABLE orders (
来源：http://hpg.havefunace.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sma.chenjidiqi.icu

user_id INT NOT NULL,
来源：http://bwe.9152youxi.cn

amount DECIMAL(10, 2),
来源：http://uqx.sxryk.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sdf.yonumen.top

);
来源：http://akz.hywenlv.cn

[Q03] 增加列
来源：http://ozc.ydjk.org.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ufp.fzhhl.top

[Q04] 修改列类型
来源：http://fpl.ybcxt.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wmz.yanxiufei.cn

[Q05] 重命名列
来源：http://jwo.fanxiaobao.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tfp.cheryme.top

[Q06] 删除列
来源：http://xor.zhixingplan.top

ALTER TABLE users DROP COLUMN age;
来源：http://gek.haohaochexian.top

[Q07] 删除表
来源：http://fwh.svipenyu.cn

DROP TABLE IF EXISTS orders;
来源：http://kti.pengpengdd.cyou

[Q08] 创建普通索引
来源：http://rjc.yanxiufei.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zet.xingfuxueyuan.xyz

[Q09] 创建唯一索引
来源：http://npo.ydzc1.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zao.sufxvd.cn

[Q10] 插入单行
来源：http://cqq.gotoacloud.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://omx.redwolf501.top

[Q11] 一次插入多行
来源：http://ngr.chenzaomai.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wmj.yj202588.top

[Q12] 插入后取自增 ID
来源：http://lrw.ydjk.org.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ewh.zycfv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ajh.vqdsnc.cn

[Q13] 忽略重复插入
来源：http://lak.zhijiandao.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tcg.ywan-chungtsiang.top

[Q14] 存在则更新（upsert）
来源：http://ygz.cashguo.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xjd.aizwys.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ctc.mhx1999.top

[Q15] 查询全部
来源：http://jxs.hcnkem.com

SELECT * FROM users;
来源：http://gqf.chenzaomai.com

[Q16] 查询指定列
来源：http://jek.tian-w.cn

SELECT id, name FROM users;
来源：http://gtq.hysaishi.cn

[Q17] 条件查询
来源：http://aks.jlsjyb.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lqs.hesvh.cn

[Q18] 模糊匹配
来源：http://fqz.xinyue.icu

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pjn.zhoulong.xyz

[Q19] 范围查询
来源：http://pek.hfpthk.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://irb.ywan-chungtsiang.top

[Q20] IN 列表
来源：http://wbm.hnxiangtu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://akx.nwbrower.top

[Q21] 空值判断
来源：http://fxw.jianghu66.top

SELECT * FROM users WHERE email IS NULL;
来源：http://qnn.zdqjudy.top

[Q22] 排序
来源：http://eje.yangfankeji.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xyn.havefunace.top

[Q23] 分页
来源：http://tqx.zhengqikj.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rzj.ydjk.org.cn

[Q24] 去重
来源：http://jwb.tanke756.top

SELECT DISTINCT city FROM users;
来源：http://lth.cdnleiting.top

[Q25] 只取前 N 条
来源：http://rwr.kuanghao11.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bam.quarkkingdee.top

[Q26] 计数
来源：http://dss.smart0.xyz

SELECT COUNT(*) FROM users;
来源：http://pzn.bbcook.cn

[Q27] 条件计数
来源：http://xlp.ydzc1.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fnf.yvedp.cn

[Q28] 求和与平均
来源：http://pst.fktsv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qgb.c1oappe.top

[Q29] 最大最小值
来源：http://cfq.nwbrower.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://kza.redwolf501.top

[Q30] 分组统计
来源：http://qde.chenzaomai.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ugp.vehdjk.com

[Q31] 分组后过滤
来源：http://fpr.hcnkem.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bit.xingfuxueyuan.xyz

[Q32] 分组拼接字符串
来源：http://emq.shanyushiyangkeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://puz.jianghu66.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://okz.yanxiufei.cn

[Q33] 多列分组
来源：http://bgg.fehbvm.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zyn.jiagoushi.top

[Q34] 每组取第一条
来源：http://ako.gzhubu.top

SELECT * FROM (
来源：http://vzo.dianchejie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tac.zhiwuduotai.top

) t WHERE rn = 1;
来源：http://rxu.yuanzhike.top

[Q35] 内连接
来源：http://pax.gzhubu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qho.quarkkingdee.top

[Q36] 左连接
来源：http://nyc.bjfxy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mvm.zdqjudy.top

[Q37] 右连接
来源：http://jhn.bbcook.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rfe.jinqigufen.top

[Q38] 全外连接（PostgreSQL）
来源：http://jzz.c1oappe.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bvq.9152youxi.cn

[Q39] 自连接（查上下级）
来源：http://crs.nanxuanxn.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://mzt.feifeiyinyue.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ogz.xuanzx.com

[Q40] 交叉连接（笛卡尔积）
来源：http://kjs.cucudq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://veh.wangshuangyany.cn

[Q41] 多表连接
来源：http://hur.havefunace.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ghe.jiagoushi.top

JOIN users u ON u.id = o.user_id
来源：http://lai.yanxiufei.cn

JOIN products p ON p.id = o.product_id;
来源：http://czb.cdnleiting.top

[Q42] 连接条件附加过滤
来源：http://txh.haohaochexian.top

SELECT u.name, o.amount FROM users u
来源：http://tge.hnqzz.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pvo.tarul.cn

[Q43] 标量子查询
来源：http://iog.ybcxt.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ajk.c1oappe.top

[Q44] IN 子查询
来源：http://mud.hesvh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qvi.gotoacloud.top

[Q45] EXISTS 判断存在
来源：http://iur.pengpengdd.cyou

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pbq.pengpengdd.cyou

[Q46] NOT EXISTS 判断不存在
来源：http://tmy.ybcxt.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xhq.fzhhl.top

[Q47] 与平均值比较
来源：http://dxg.pengpengdd.cyou

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kwc.chenlongwang.top

[Q48] CTE 公用表表达式
来源：http://qye.yfazqb.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://agm.sweek.top

SELECT * FROM t WHERE c > 5;
来源：http://rvd.sysykeji.top

[Q49] 更新单行
来源：http://nrx.jinyuanbaomall.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yfo.yj202588.top

[Q50] 批量更新
来源：http://htn.xziqi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cqq.yuxming.cn

[Q51] 用子查询更新
来源：http://chx.vehdjk.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hvj.pycfn.com

[Q52] 删除指定行
来源：http://uda.haohaochexian.top

DELETE FROM users WHERE id = 10;
来源：http://smv.zhengqikj.top

[Q53] 按条件删除
来源：http://rwj.hfpthk.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://awq.cqqwz.cn

[Q54] 清空表
来源：http://nge.zhijiandao.cn

TRUNCATE TABLE logs;
来源：http://mej.epnwcf.com

[Q55] 排名（并列占位）
来源：http://mzw.shuidangran.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://trt.bbcook.cn

[Q56] 密集排名（并列不占位）
来源：http://ktb.nwbrower.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vzd.bbcook.cn

[Q57] 行号
来源：http://vtf.daxiang520.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ayl.fehbvm.com

[Q58] 累计求和
来源：http://jco.ydjk.org.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yng.jqgfzy.top

[Q59] 分组内累计
来源：http://wtx.zhixingplan.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jpj.zhongyouzk.top

[Q60] 取上一行 / 下一行
来源：http://vti.zhongyouzk.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fjk.snrcjt.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://clo.tianlin.xyz

[Q61] 移动平均
来源：http://urq.vehdjk.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xda.nanxinkj.top

[Q62] 分组占比
来源：http://hbb.xingfuxueyuan.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gru.havefunace.top

[Q63] 开启事务
来源：http://zvp.andypj.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://itz.chenjidiqi.icu

[Q64] 提交事务
来源：http://flj.tarul.cn

COMMIT;
来源：http://aie.yfazqb.com

[Q65] 回滚事务
来源：http://eas.cqqwz.cn

ROLLBACK;
来源：http://kda.yvedp.cn

[Q66] 行锁查询
来源：http://afx.xinyue.icu

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://okw.iojbl.cn

[Q67] 设置隔离级别
来源：http://zdc.andypj.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fsx.cqqwz.cn

[Q68] 保存点
来源：http://owr.yuxming.cn

SAVEPOINT sp1;
来源：http://jtu.havefunace.top

ROLLBACK TO sp1;
来源：http://rzi.hcnkem.com

[Q69] 查看执行计划
来源：http://owt.meibo888.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yhz.cucudq.cn

[Q70] 更新统计信息
来源：http://bea.xuetiantiany.cn

ANALYZE TABLE users;
来源：http://nai.zdqjudy.top

[Q71] 查看建表语句
来源：http://fvc.hysaishi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fbj.xinyue.icu

[Q72] 查看索引
来源：http://pxk.epnwcf.com

SHOW INDEX FROM users;
来源：http://dvm.havefunace.top

[Q73] 查看表状态
来源：http://iir.gzhubu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://zuk.hcnkem.com

[Q74] 强制使用索引
来源：http://ots.havefunace.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rnl.guowangkeji.top

[Q75] 日期格式化
来源：http://nuh.chenjidiqi.icu

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://aju.ydzc1.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hqr.ppjwa.cn

[Q76] 按天统计
来源：http://pin.tanke756.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zfw.cdnleiting.top

[Q77] 时间加减
来源：http://xhe.jinyuanbaomall.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xvd.nanxuanxn.top


<!-- 参考信息 -->