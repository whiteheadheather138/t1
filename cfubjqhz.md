代发 wailian999

[O02] 使用线程池
来源：http://hvb.cucudq.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fma.hnqzz.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fls.nanxinkj.top

JS:   // worker_threads 线程池
来源：http://jqh.ybcxt.top

TS:   // worker_threads 线程池
来源：http://wyn.vqdsnc.cn

Java: Executors.newFixedThreadPool(4)
来源：http://sce.guannengcc.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ssf.jlsjyb.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://asn.sysykeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qgw.fanxiaobao.xyz

[O03] 加锁保护共享数据
来源：http://zbz.yj20258888.top

Py:   with lock: shared += 1
来源：http://eva.zhaomingkeji.xyz

PHP:  // 用 flock() 做文件锁
来源：http://ash.hammf.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jyf.aizwys.cn

TS:   // 同 JS
来源：http://pao.xinyue.icu

Java: synchronized (this) { shared++; }
来源：http://mns.zhiwuduotai.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nzt.hcnkem.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://zmc.cheryme.top

C#:   lock (gate) { shared++; }
来源：http://uke.shangyingyoupin.top

[O04] 定义异步函数并等待
来源：http://rix.xuetiantiany.cn

Py:   async def f():⏎    await g()
来源：http://yfy.havefunace.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ucz.zdqjudy.top

JS:   async function f() { await g(); }
来源：http://grk.316326.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://jot.tarul.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://iai.gogol.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yex.meibo888.top

Ruby: # 用 Fiber 或 async gem
来源：http://nin.dashuyun.cn

C#:   async Task F() { await G(); }
来源：http://mnl.yonumen.top

[O05] 并发执行并等待全部完成
来源：http://lxk.yj202588.top

Py:   asyncio.gather(*tasks)
来源：http://qdk.zhijiandao.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nrs.hysaishi.cn

JS:   await Promise.all(tasks)
来源：http://kyp.jiagoushi.top

TS:   await Promise.all(tasks)
来源：http://dmp.yonumen.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qdc.guannengcc.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jzr.sweek.top

Ruby: threads.map(&:join)
来源：http://xne.zhoulong.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://fek.mhx1999.top

[O06] 使用进程池
来源：http://uln.chenjidiqi.icu

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hxw.vehdjk.com

PHP:  // pcntl_fork 或多进程队列
来源：http://can.chenzaomai.com

JS:   // child_process / cluster 模块
来源：http://qdv.zhiwuduotai.top

TS:   // child_process / cluster 模块
来源：http://dpp.fzhhl.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dpp.shangyingyoupin.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://thx.jinqigfzy.top

Ruby: // fork 块
来源：http://oef.kuanghao11.cn

C#:   Parallel.For
来源：http://hca.nanxuanxn.top

================================================================================
来源：http://fts.sjlbkw.cn

P. 常用工具函数
来源：http://bft.vehdjk.com

================================================================================
来源：http://pvu.zdqjudy.top

[P01] 生成 UUID
来源：http://ygd.wangdashe.top

Py:   str(uuid.uuid4())
来源：http://hvx.jiagoushi.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ige.jyoumei.cn

JS:   crypto.randomUUID()
来源：http://yis.cucudq.cn

TS:   crypto.randomUUID()
来源：http://jno.zycfv.cn

Java: UUID.randomUUID().toString()
来源：http://cvb.smart0.xyz

Go:   // 用 github.com/google/uuid
来源：http://yhz.316326.xyz

Ruby: SecureRandom.uuid
来源：http://zzq.cucudq.cn

C#:   Guid.NewGuid().ToString()
来源：http://roe.vqdsnc.cn

[P02] MD5 / SHA256 摘要
来源：http://fxm.yanxiufei.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nxk.havefunace.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://izj.tian-w.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nkw.zhijiandao.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ses.tanke756.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://obd.zhaomingkeji.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pms.uphjek.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fwa.nanxuanxn.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cnr.redwolf501.top

[P03] 生成短随机字符串
来源：http://qhp.cashguo.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://onf.mhx1999.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tcd.cucudq.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://htq.yonumen.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nwr.ydzc1.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rfm.c1oappe.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jnn.cheryme.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ihk.zycfv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yca.c1oappe.top

[P04] 求长度
来源：http://qwf.yvedp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qlr.jinghuilouyu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rxc.yj202588.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lgq.ehwqpu.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gon.ppjwa.cn

Java: list.size();  map.size();  s.length()
来源：http://gwf.0kj1m.cn

Go:   len(arr);  len(m)
来源：http://iyk.ywan-chungtsiang.top

Ruby: x.length;  x.size
来源：http://qop.fktsv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://dey.jyoumei.cn

[P05] 判断两个对象内容是否相等
来源：http://pel.zhijiandao.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qqo.bjfxy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gzw.gotoacloud.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qrn.daxiang520.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jpl.shanyushiyangkeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tue.meibo888.top

Go:   reflect.DeepEqual(a, b)
来源：http://yob.ivvv.top

Ruby: a == b
来源：http://dyr.gaohongyu789.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lkf.hnqzz.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://joq.uphjek.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rse.hfpthk.cn

PHP:  if (empty($x)) {}
来源：http://vlr.yonumen.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ozy.ywan-chungtsiang.top

TS:   if (x == null) {}
来源：http://zlv.havefunace.top

Java: if (x == null || x.isEmpty()) {}
来源：http://gls.sjlbkw.cn

Go:   if x == nil {}
来源：http://hur.pengpengdd.cyou

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ftw.gogol.net.cn

C#:   if (x is null) {}
来源：http://jzq.yj202588.top

[P07] 防抖与节流
来源：http://zpu.gaohongyu789.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ixk.zdqjudy.top

PHP:  // 手写时间戳比较
来源：http://coq.aizwys.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://djr.52xcode.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oxa.jinghuilouyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jcw.xuetiantiany.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bme.cqqwz.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zrw.yonumen.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gjz.yueranfly.top

[P08] 处理浮点精度问题
来源：http://dgr.kuanghao11.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vfn.andypj.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baz.gogol.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ubp.xingfuxueyuan.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cxc.ydzc1.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ysu.epnwcf.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zek.hesvh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ghr.zdqjudy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://skc.yonumen.top

================================================================================
来源：http://jgc.hnxiangtu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xnl.fktsv.cn

================================================================================
来源：http://ckj.fehbvm.com

[Q01] 创建表
来源：http://ykv.pengpengdd.cyou

CREATE TABLE users (
来源：http://xzx.yanxiufei.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ovy.yuanzhike.top

name VARCHAR(50) NOT NULL,
来源：http://bia.pycfn.com

email VARCHAR(100) UNIQUE,
来源：http://ecn.0kj1m.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ufi.yfazqb.com

);
来源：http://yyb.yj20258.top

[Q02] 创建带外键的表
来源：http://kbk.feifeiyinyue.top

CREATE TABLE orders (
来源：http://hqv.ydzc1.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nju.jinghuilouyu.cn

user_id INT NOT NULL,
来源：http://vuh.chenzaomai.com

amount DECIMAL(10, 2),
来源：http://sst.zhijiandao.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uyc.fanxiaobao.xyz

);
来源：http://len.dianchejie.cn

[Q03] 增加列
来源：http://cmr.cheryme.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yst.0kj1m.cn

[Q04] 修改列类型
来源：http://hog.52xcode.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pmw.jianghu66.top

[Q05] 重命名列
来源：http://ifn.hesvh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hxe.gogol.net.cn

[Q06] 删除列
来源：http://cmf.pycfn.com

ALTER TABLE users DROP COLUMN age;
来源：http://hkg.uphjek.com

[Q07] 删除表
来源：http://qfx.gaohongyu789.top

DROP TABLE IF EXISTS orders;
来源：http://coe.ctjpmb.com

[Q08] 创建普通索引
来源：http://rzd.smart0.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://snv.fengsongda.top

[Q09] 创建唯一索引
来源：http://fxu.hongshengwenyu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lzt.xingfuxueyuan.xyz

[Q10] 插入单行
来源：http://rpx.shuidangran.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zbh.sweek.top

[Q11] 一次插入多行
来源：http://kyi.wangshuangyany.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wdp.cdnleiting.top

[Q12] 插入后取自增 ID
来源：http://rju.sysykeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://cjk.xziqi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hjt.gaohongyu789.top

[Q13] 忽略重复插入
来源：http://pzk.hongshengwenyu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nfv.fengsongda.top

[Q14] 存在则更新（upsert）
来源：http://ijz.daria6918.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vvi.cqqwz.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zin.smart0.xyz

[Q15] 查询全部
来源：http://auw.jinyuanbaomall.cn

SELECT * FROM users;
来源：http://siz.zhongyouzk.top

[Q16] 查询指定列
来源：http://vxy.xingfuxueyuan.xyz

SELECT id, name FROM users;
来源：http://kag.andypj.xyz

[Q17] 条件查询
来源：http://tos.fzhhl.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://utp.sxryk.cn

[Q18] 模糊匹配
来源：http://bsq.svipenyu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rrk.yvedp.cn

[Q19] 范围查询
来源：http://gqr.ivvv.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pdu.zycfv.cn

[Q20] IN 列表
来源：http://gpr.vehdjk.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yfa.yonumen.top

[Q21] 空值判断
来源：http://cls.fengsongda.top

SELECT * FROM users WHERE email IS NULL;
来源：http://nwo.yj20258888.top

[Q22] 排序
来源：http://gxj.jqgufenzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gnh.zycfv.cn

[Q23] 分页
来源：http://ncp.xuanzx.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ilk.nwbrower.top

[Q24] 去重
来源：http://nbz.shanyushiyangkeji.top

SELECT DISTINCT city FROM users;
来源：http://vpt.shangyingyoupin.top

[Q25] 只取前 N 条
来源：http://rmg.yfazqb.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lng.fzhhl.top

[Q26] 计数
来源：http://xdx.ywan-chungtsiang.top

SELECT COUNT(*) FROM users;
来源：http://vfn.cheryme.top

[Q27] 条件计数
来源：http://iph.xuetiantiany.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://quo.tanke756.top

[Q28] 求和与平均
来源：http://xnt.sjlbkw.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kmp.zhixingplan.top

[Q29] 最大最小值
来源：http://meo.jqgufenzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://njw.andypj.xyz

[Q30] 分组统计
来源：http://urg.chenzaomai.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://oad.jqgfzy.top

[Q31] 分组后过滤
来源：http://wei.fehbvm.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ekg.yongpay.top

[Q32] 分组拼接字符串
来源：http://dzx.yj20258888.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wzp.zycfv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sve.smart0.xyz

[Q33] 多列分组
来源：http://szs.zhijiandao.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wbj.tarul.cn

[Q34] 每组取第一条
来源：http://aql.cheryme.top

SELECT * FROM (
来源：http://uya.yangfankeji.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lmq.hysaishi.cn

) t WHERE rn = 1;
来源：http://vuq.jyoumei.cn

[Q35] 内连接
来源：http://drc.ybcxt.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kca.ivvv.top

[Q36] 左连接
来源：http://ejc.andypj.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ygm.kuanghao11.cn

[Q37] 右连接
来源：http://gvi.wangdashe.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kdm.yuanzhike.top

[Q38] 全外连接（PostgreSQL）
来源：http://ypf.jianghu66.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lco.yangfankeji.com

[Q39] 自连接（查上下级）
来源：http://wtb.xziqi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fxd.hesvh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qsx.nanxuanxn.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zsf.shanyushiyangkeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://das.zhixingplan.top

[Q41] 多表连接
来源：http://nfr.bbcook.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ebk.hnqzz.top

JOIN users u ON u.id = o.user_id
来源：http://crv.gzhubu.top

JOIN products p ON p.id = o.product_id;
来源：http://dni.iojbl.cn

[Q42] 连接条件附加过滤
来源：http://auz.ctjpmb.com

SELECT u.name, o.amount FROM users u
来源：http://azr.meibo888.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rnc.ybcxt.top

[Q43] 标量子查询
来源：http://urz.fzhhl.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://owo.kuanghao11.cn

[Q44] IN 子查询
来源：http://zqt.jiagoushi.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yix.xuetiantiany.cn

[Q45] EXISTS 判断存在
来源：http://vwr.epnwcf.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jce.jianghu66.top

[Q46] NOT EXISTS 判断不存在
来源：http://srd.hywenlv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nyg.gzhubu.top

[Q47] 与平均值比较
来源：http://vqc.jinghuilouyu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gqc.jyoumei.cn

[Q48] CTE 公用表表达式
来源：http://aub.fehbvm.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hwu.mhx1999.top

SELECT * FROM t WHERE c > 5;
来源：http://blf.ybcxt.top

[Q49] 更新单行
来源：http://zed.svipenyu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zdi.aibaodan.cn

[Q50] 批量更新
来源：http://pgn.fktsv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bdg.ywan-chungtsiang.top

[Q51] 用子查询更新
来源：http://idp.sweek.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yma.kuanghao11.cn

[Q52] 删除指定行
来源：http://uxn.cucudq.cn

DELETE FROM users WHERE id = 10;
来源：http://lhe.chenlongwang.top

[Q53] 按条件删除
来源：http://sqd.nwbrower.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fzj.nanxuanxn.top

[Q54] 清空表
来源：http://tcw.yuanzhike.top

TRUNCATE TABLE logs;
来源：http://qgm.jlsjyb.cn

[Q55] 排名（并列占位）
来源：http://gof.cdnleiting.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rkw.sufxvd.cn

[Q56] 密集排名（并列不占位）
来源：http://oev.yvedp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://len.jqgufenzy.top

[Q57] 行号
来源：http://cfs.iojbl.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sfs.zdbjq.cn

[Q58] 累计求和
来源：http://aue.tarul.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dbg.birdmap.top

[Q59] 分组内累计
来源：http://ndo.daxiang520.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xxz.fehbvm.com

[Q60] 取上一行 / 下一行
来源：http://yvw.hnqzz.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://aeb.quarkkingdee.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ruc.cashguo.top

[Q61] 移动平均
来源：http://aaj.hfpthk.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qcj.yuanzhike.top

[Q62] 分组占比
来源：http://bix.meibo888.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kpp.cheryme.top

[Q63] 开启事务
来源：http://lpz.sweek.top

START TRANSACTION;                -- 或 BEGIN
来源：http://hxe.hfpthk.cn

[Q64] 提交事务
来源：http://oly.xuetiantiany.cn

COMMIT;
来源：http://voc.cqqwz.cn

[Q65] 回滚事务
来源：http://cqj.sysykeji.top

ROLLBACK;
来源：http://iru.cashguo.top

[Q66] 行锁查询
来源：http://srm.tarul.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://alx.quarkkingdee.top

[Q67] 设置隔离级别
来源：http://dqa.shanyushiyangkeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jsn.vehdjk.com

[Q68] 保存点
来源：http://bdp.xylfe.cn

SAVEPOINT sp1;
来源：http://tnd.zhixingplan.top

ROLLBACK TO sp1;
来源：http://ubj.cdnleiting.top

[Q69] 查看执行计划
来源：http://nhi.hnqzz.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lfu.bjfxy.top

[Q70] 更新统计信息
来源：http://bvz.kuanghao11.cn

ANALYZE TABLE users;
来源：http://mws.chenzaomai.com

[Q71] 查看建表语句
来源：http://vnb.xingfuxueyuan.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bai.hesvh.cn

[Q72] 查看索引
来源：http://wke.yonumen.top

SHOW INDEX FROM users;
来源：http://fic.daxiang520.top

[Q73] 查看表状态
来源：http://wry.ydzc1.top

SHOW TABLE STATUS LIKE 'users';
来源：http://sdu.sxryk.cn

[Q74] 强制使用索引
来源：http://cty.tianlin.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gru.zhongyouzk.top

[Q75] 日期格式化
来源：http://xso.sjlbkw.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eas.vqdsnc.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ian.hnxiangtu.top

[Q76] 按天统计
来源：http://agf.ywan-chungtsiang.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ggl.gaohongyu789.top

[Q77] 时间加减
来源：http://zpj.zhengqikj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://owh.epnwcf.com


<!-- 参考信息 -->