代发 wailian999

TS:   // worker_threads 线程池
来源：http://hsd.ywan-chungtsiang.top

Java: Executors.newFixedThreadPool(4)
来源：http://yjc.zhoulong.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wxi.sxryk.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uur.zhoulong.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wpu.52xcode.cn

[O03] 加锁保护共享数据
来源：http://olw.yfazqb.com

Py:   with lock: shared += 1
来源：http://zua.birdmap.top

PHP:  // 用 flock() 做文件锁
来源：http://cso.cashguo.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kei.aizwys.cn

TS:   // 同 JS
来源：http://lsy.chenzaomai.com

Java: synchronized (this) { shared++; }
来源：http://yhs.fzhhl.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ztz.hnqzz.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://mrw.tianlin.xyz

C#:   lock (gate) { shared++; }
来源：http://hmj.jlsjyb.cn

[O04] 定义异步函数并等待
来源：http://kqi.haohaochexian.top

Py:   async def f():⏎    await g()
来源：http://mgq.zhijiandao.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://aiz.jlsjyb.cn

JS:   async function f() { await g(); }
来源：http://jux.hcnkem.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://xxk.cheryme.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hhr.yfazqb.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nts.gotoacloud.top

Ruby: # 用 Fiber 或 async gem
来源：http://ndb.yuxming.cn

C#:   async Task F() { await G(); }
来源：http://cpn.yueranfly.top

[O05] 并发执行并等待全部完成
来源：http://jdh.meibo888.top

Py:   asyncio.gather(*tasks)
来源：http://npr.zhiwuduotai.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dag.kuanghao11.cn

JS:   await Promise.all(tasks)
来源：http://vqf.cucudq.cn

TS:   await Promise.all(tasks)
来源：http://lah.yangfankeji.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dqf.hywenlv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://alh.fengsongda.top

Ruby: threads.map(&:join)
来源：http://zgq.hnqzz.top

C#:   await Task.WhenAll(t1, t2)
来源：http://onm.jyoumei.cn

[O06] 使用进程池
来源：http://bav.zhijiandao.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uxl.dashuyun.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zdv.9152youxi.cn

JS:   // child_process / cluster 模块
来源：http://dmi.havefunace.top

TS:   // child_process / cluster 模块
来源：http://dih.fanxiaobao.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://afv.aizwys.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qqi.hnqzz.top

Ruby: // fork 块
来源：http://udy.zhengqikj.top

C#:   Parallel.For
来源：http://nkk.sxryk.cn

================================================================================
来源：http://qat.sysykeji.top

P. 常用工具函数
来源：http://zaf.316326.xyz

================================================================================
来源：http://jpv.smart0.xyz

[P01] 生成 UUID
来源：http://xex.cucudq.cn

Py:   str(uuid.uuid4())
来源：http://rvf.0kj1m.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lip.mhx1999.top

JS:   crypto.randomUUID()
来源：http://eay.cucudq.cn

TS:   crypto.randomUUID()
来源：http://xkh.wangshuangyany.cn

Java: UUID.randomUUID().toString()
来源：http://net.cheryme.top

Go:   // 用 github.com/google/uuid
来源：http://dgj.fengsongda.top

Ruby: SecureRandom.uuid
来源：http://cmn.fehbvm.com

C#:   Guid.NewGuid().ToString()
来源：http://hpx.shuidangran.top

[P02] MD5 / SHA256 摘要
来源：http://tnz.hysaishi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bsq.zhengqikj.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://jxx.tanke756.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://biu.zhixingplan.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uzo.jinqigfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ofn.guowangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sul.nwbrower.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ttw.zdbjq.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://seg.sjlbkw.cn

[P03] 生成短随机字符串
来源：http://tvx.fktsv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vlj.wangdashe.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xdt.xziqi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://irv.cqqwz.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hxa.tianlin.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ily.meibo888.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tfk.gaohongyu789.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://vfl.yanxiufei.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://umy.yj20258888.top

[P04] 求长度
来源：http://spy.pycfn.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kjr.zhiwuduotai.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rtj.zhijiandao.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dee.vqdsnc.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kce.bbcook.cn

Java: list.size();  map.size();  s.length()
来源：http://oxr.sxryk.cn

Go:   len(arr);  len(m)
来源：http://nid.uphjek.com

Ruby: x.length;  x.size
来源：http://lsn.jinqigfzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://vgp.fzhhl.top

[P05] 判断两个对象内容是否相等
来源：http://ufg.ppjwa.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yje.birdmap.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rbd.gogol.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ewa.jiagoushi.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xll.hywenlv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ppm.sufxvd.cn

Go:   reflect.DeepEqual(a, b)
来源：http://omb.dashuyun.cn

Ruby: a == b
来源：http://ptr.zhongyouzk.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://psm.zhixingplan.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dkx.epnwcf.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gxw.redwolf501.top

PHP:  if (empty($x)) {}
来源：http://ult.cucudq.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ejo.ehwqpu.com

TS:   if (x == null) {}
来源：http://utc.gogol.net.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://esm.hnqzz.top

Go:   if x == nil {}
来源：http://qyi.nanxinkj.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qof.smart0.xyz

C#:   if (x is null) {}
来源：http://yno.smart0.xyz

[P07] 防抖与节流
来源：http://sue.cashguo.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vlt.xziqi.cn

PHP:  // 手写时间戳比较
来源：http://vmp.yvedp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://huo.cheryme.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oue.dianchejie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uii.yongpay.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hdg.zhiwuduotai.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wyc.jqgufenzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sbo.xinyue.icu

[P08] 处理浮点精度问题
来源：http://scx.fanxiaobao.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vii.epnwcf.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dji.yonumen.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zkh.dashuyun.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yfa.zhixingplan.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lsl.haohaochexian.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://azs.xuanzx.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sgt.guowangkeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jzv.ctjpmb.com

================================================================================
来源：http://rxa.tianlin.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uev.zhengqikj.top

================================================================================
来源：http://tfv.cdnleiting.top

[Q01] 创建表
来源：http://qwz.hesvh.cn

CREATE TABLE users (
来源：http://tnf.aizwys.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ops.guannengcc.top

name VARCHAR(50) NOT NULL,
来源：http://pkt.ywan-chungtsiang.top

email VARCHAR(100) UNIQUE,
来源：http://udf.zdbjq.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fce.yj20258.top

);
来源：http://ola.hnxiangtu.top

[Q02] 创建带外键的表
来源：http://kzw.gzhubu.top

CREATE TABLE orders (
来源：http://kue.meibo888.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rll.jqgfzy.top

user_id INT NOT NULL,
来源：http://hyj.kuanghao11.cn

amount DECIMAL(10, 2),
来源：http://ctt.fktsv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hdv.shanyushiyangtech.top

);
来源：http://ejs.hesvh.cn

[Q03] 增加列
来源：http://zhr.tarul.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://thh.pengpengdd.cyou

[Q04] 修改列类型
来源：http://pbn.jlsjyb.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kid.zhiwuduotai.top

[Q05] 重命名列
来源：http://mke.0kj1m.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://oam.yj20258888.top

[Q06] 删除列
来源：http://ibl.sxryk.cn

ALTER TABLE users DROP COLUMN age;
来源：http://wob.zycfv.cn

[Q07] 删除表
来源：http://wec.yj202588.top

DROP TABLE IF EXISTS orders;
来源：http://rwx.bbcook.cn

[Q08] 创建普通索引
来源：http://taf.snrcjt.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xhw.guowangkeji.top

[Q09] 创建唯一索引
来源：http://ukf.yanxiufei.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kaw.yangfankeji.com

[Q10] 插入单行
来源：http://qvj.jlsjyb.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dcr.yj20258.top

[Q11] 一次插入多行
来源：http://ila.uphjek.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qqd.shanyushiyangkeji.top

[Q12] 插入后取自增 ID
来源：http://ymb.sufxvd.cn

INSERT INTO users (name) VALUES ('C');
来源：http://zul.shanyushiyangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lug.sweek.top

[Q13] 忽略重复插入
来源：http://ivk.bbcook.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://upa.gzhubu.top

[Q14] 存在则更新（upsert）
来源：http://hgc.jinyuanbaomall.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zrw.zhixingplan.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yep.xinyue.icu

[Q15] 查询全部
来源：http://owk.bbcook.cn

SELECT * FROM users;
来源：http://tzz.ctjpmb.com

[Q16] 查询指定列
来源：http://epn.smart0.xyz

SELECT id, name FROM users;
来源：http://ani.yj20258888.top

[Q17] 条件查询
来源：http://ygr.jinqigufen.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zrh.zycfv.cn

[Q18] 模糊匹配
来源：http://mks.jlsjyb.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wbl.tian-w.cn

[Q19] 范围查询
来源：http://zuj.shanyushiyangkeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bbt.sufxvd.cn

[Q20] IN 列表
来源：http://tfs.fanxiaobao.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iqk.ehwqpu.com

[Q21] 空值判断
来源：http://xhd.hesvh.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wdb.fanxiaobao.xyz

[Q22] 排序
来源：http://kwh.xylfe.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bkm.guannengcc.top

[Q23] 分页
来源：http://vfd.jqgufenzy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bea.jyoumei.cn

[Q24] 去重
来源：http://bxu.svipenyu.cn

SELECT DISTINCT city FROM users;
来源：http://xgk.aibaodan.cn

[Q25] 只取前 N 条
来源：http://qil.aizwys.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://eqq.sysykeji.top

[Q26] 计数
来源：http://sms.fktsv.cn

SELECT COUNT(*) FROM users;
来源：http://ral.daxiang520.top

[Q27] 条件计数
来源：http://mgx.yfazqb.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gfs.hfpthk.cn

[Q28] 求和与平均
来源：http://ibj.uphjek.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vys.jqgfzy.top

[Q29] 最大最小值
来源：http://aci.zhixingplan.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://umw.ppjwa.cn

[Q30] 分组统计
来源：http://fhd.daxiang520.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hre.yuanzhike.top

[Q31] 分组后过滤
来源：http://mbt.zhaomingkeji.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://oqk.chenzaomai.com

[Q32] 分组拼接字符串
来源：http://vvm.ydjk.org.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://upo.ppjwa.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vjb.sxryk.cn

[Q33] 多列分组
来源：http://ivl.jlsjyb.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hdx.fktsv.cn

[Q34] 每组取第一条
来源：http://ybn.chenjidiqi.icu

SELECT * FROM (
来源：http://dyp.yvedp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pwh.zhengqikj.top

) t WHERE rn = 1;
来源：http://cis.chenlongwang.top

[Q35] 内连接
来源：http://fjn.haohaochexian.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tuw.aizwys.cn

[Q36] 左连接
来源：http://roy.zdbjq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vsd.sjlbkw.cn

[Q37] 右连接
来源：http://faq.tian-w.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://slh.daxiang520.top

[Q38] 全外连接（PostgreSQL）
来源：http://icm.shanyushiyangtech.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://msr.haohaochexian.top

[Q39] 自连接（查上下级）
来源：http://tyb.jinqigufen.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://xoj.vehdjk.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dyx.nanxinkj.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ytk.yangfankeji.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://clv.quarkkingdee.top

[Q41] 多表连接
来源：http://jkn.zhijiandao.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://erk.ywan-chungtsiang.top

JOIN users u ON u.id = o.user_id
来源：http://tpu.andypj.xyz

JOIN products p ON p.id = o.product_id;
来源：http://jsr.zdqjudy.top

[Q42] 连接条件附加过滤
来源：http://kdk.vehdjk.com

SELECT u.name, o.amount FROM users u
来源：http://tcp.xingfuxueyuan.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nwh.cdnleiting.top

[Q43] 标量子查询
来源：http://cgk.nwbrower.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rvk.cdnleiting.top

[Q44] IN 子查询
来源：http://xri.hnxiangtu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zof.jyoumei.cn

[Q45] EXISTS 判断存在
来源：http://fxw.0kj1m.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ixf.jqgfzy.top

[Q46] NOT EXISTS 判断不存在
来源：http://mxi.yuxming.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rcx.hfpthk.cn

[Q47] 与平均值比较
来源：http://gtg.zhiwuduotai.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uyi.hfpthk.cn

[Q48] CTE 公用表表达式
来源：http://iml.xziqi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://trf.havefunace.top

SELECT * FROM t WHERE c > 5;
来源：http://xaq.gotoacloud.top

[Q49] 更新单行
来源：http://bfj.yj20258.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pxs.cucudq.cn

[Q50] 批量更新
来源：http://pde.zdbjq.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jjb.316326.xyz

[Q51] 用子查询更新
来源：http://odh.wangshuangyany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ojw.hongshengwenyu.top

[Q52] 删除指定行
来源：http://pnf.smart0.xyz

DELETE FROM users WHERE id = 10;
来源：http://qki.shzxlz.cn

[Q53] 按条件删除
来源：http://aic.bbcook.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://obn.iojbl.cn

[Q54] 清空表
来源：http://zdg.quarkkingdee.top

TRUNCATE TABLE logs;
来源：http://cka.yonumen.top

[Q55] 排名（并列占位）
来源：http://ath.chenjidiqi.icu

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zlw.ehwqpu.com

[Q56] 密集排名（并列不占位）
来源：http://ece.0kj1m.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ddl.daxiang520.top

[Q57] 行号
来源：http://fqn.nwbrower.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rgt.yonumen.top

[Q58] 累计求和
来源：http://row.pycfn.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hcf.vehdjk.com

[Q59] 分组内累计
来源：http://fom.hfpthk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://irf.yanxiufei.cn

[Q60] 取上一行 / 下一行
来源：http://oji.hongshengwenyu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kye.chenlongwang.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://iyz.zhiwuduotai.top

[Q61] 移动平均
来源：http://guu.jiagoushi.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xhb.jinghuilouyu.cn

[Q62] 分组占比
来源：http://uyo.zhengqikj.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jbq.yongpay.top

[Q63] 开启事务
来源：http://uwc.gotoacloud.top

START TRANSACTION;                -- 或 BEGIN
来源：http://fee.hysaishi.cn

[Q64] 提交事务
来源：http://cga.zhongyouzk.top

COMMIT;
来源：http://ktb.wangdashe.top

[Q65] 回滚事务
来源：http://rwb.cqqwz.cn

ROLLBACK;
来源：http://kqz.daxiang520.top

[Q66] 行锁查询
来源：http://thk.zhixingplan.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yqg.smart0.xyz

[Q67] 设置隔离级别
来源：http://zma.hcnkem.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sbs.zhaomingkeji.xyz

[Q68] 保存点
来源：http://osw.iojbl.cn

SAVEPOINT sp1;
来源：http://erw.tanke756.top

ROLLBACK TO sp1;
来源：http://rwg.tarul.cn

[Q69] 查看执行计划
来源：http://zga.vehdjk.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bof.hnqzz.top

[Q70] 更新统计信息
来源：http://abm.gzhubu.top

ANALYZE TABLE users;
来源：http://cks.bbcook.cn

[Q71] 查看建表语句
来源：http://rxb.wangdashe.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gzp.hnxiangtu.top

[Q72] 查看索引
来源：http://zok.jinqigfzy.top

SHOW INDEX FROM users;
来源：http://xcu.0kj1m.cn

[Q73] 查看表状态
来源：http://ylo.jyoumei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mzh.nwbrower.top

[Q74] 强制使用索引
来源：http://yzx.sxryk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tgx.ybcxt.top

[Q75] 日期格式化
来源：http://kne.xinyue.icu

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cwe.shuidangran.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ssr.snrcjt.cn

[Q76] 按天统计
来源：http://lwk.zhongyouzk.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mgm.sufxvd.cn

[Q77] 时间加减
来源：http://czm.vqdsnc.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://seu.zhengqikj.top

[Q78] 当前时间
来源：http://kdz.shuidangran.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qys.shuidangran.top

[Q79] 字符串拼接
来源：http://bjb.hysaishi.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://spy.hongshengwenyu.top


<!-- 参考信息 -->