代发 wailian999

[O02] 使用线程池
来源：http://uwd.vqdsnc.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mbb.gotoacloud.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uou.pycfn.com

JS:   // worker_threads 线程池
来源：http://rgs.jlsjyb.cn

TS:   // worker_threads 线程池
来源：http://qzk.zycfv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ole.ydzc1.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vuv.sufxvd.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mli.jinyuanbaomall.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zuk.ctjpmb.com

[O03] 加锁保护共享数据
来源：http://aej.chenjidiqi.icu

Py:   with lock: shared += 1
来源：http://ddj.kuanghao11.cn

PHP:  // 用 flock() 做文件锁
来源：http://dtc.shuidangran.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://trz.birdmap.top

TS:   // 同 JS
来源：http://yye.yangfankeji.com

Java: synchronized (this) { shared++; }
来源：http://mfj.hesvh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yyt.guannengcc.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ppz.vqdsnc.cn

C#:   lock (gate) { shared++; }
来源：http://owl.guannengcc.top

[O04] 定义异步函数并等待
来源：http://qha.andypj.xyz

Py:   async def f():⏎    await g()
来源：http://jvc.feifeiyinyue.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tca.nwbrower.top

JS:   async function f() { await g(); }
来源：http://zht.yueranfly.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://onq.smart0.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xak.yj202588.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ugi.zhaomingkeji.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://ttr.jinqigufen.top

C#:   async Task F() { await G(); }
来源：http://usn.dianchejie.cn

[O05] 并发执行并等待全部完成
来源：http://gxb.bbcook.cn

Py:   asyncio.gather(*tasks)
来源：http://ypp.sweek.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://upj.tian-w.cn

JS:   await Promise.all(tasks)
来源：http://jos.zhengqikj.top

TS:   await Promise.all(tasks)
来源：http://aze.zhijiandao.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://eyq.dianchejie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wcd.ydjk.org.cn

Ruby: threads.map(&:join)
来源：http://erl.aizwys.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cgq.shanyushiyangtech.top

[O06] 使用进程池
来源：http://flm.cucudq.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nnv.shanyushiyangtech.top

PHP:  // pcntl_fork 或多进程队列
来源：http://jez.tianlin.xyz

JS:   // child_process / cluster 模块
来源：http://qox.snrcjt.cn

TS:   // child_process / cluster 模块
来源：http://slc.cucudq.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wlc.zdqjudy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ujx.sysykeji.top

Ruby: // fork 块
来源：http://afy.kuanghao11.cn

C#:   Parallel.For
来源：http://pdx.xuetiantiany.cn

================================================================================
来源：http://csa.ctjpmb.com

P. 常用工具函数
来源：http://ihg.yuanzhike.top

================================================================================
来源：http://zxj.jqgfzy.top

[P01] 生成 UUID
来源：http://mvo.gotoacloud.top

Py:   str(uuid.uuid4())
来源：http://vjc.cashguo.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sxc.jqgufenzy.top

JS:   crypto.randomUUID()
来源：http://xms.epnwcf.com

TS:   crypto.randomUUID()
来源：http://tao.daria6918.cn

Java: UUID.randomUUID().toString()
来源：http://swb.nwbrower.top

Go:   // 用 github.com/google/uuid
来源：http://cer.sweek.top

Ruby: SecureRandom.uuid
来源：http://gba.dashuyun.cn

C#:   Guid.NewGuid().ToString()
来源：http://qwm.havefunace.top

[P02] MD5 / SHA256 摘要
来源：http://nvf.yfazqb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zih.haohaochexian.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://pqv.hesvh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dvy.bjfxy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ocz.havefunace.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wbc.hywenlv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rmm.zhaomingkeji.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fhb.dianchejie.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rkj.gogol.net.cn

[P03] 生成短随机字符串
来源：http://qof.sjlbkw.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lgn.tianlin.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xiv.c1oappe.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ogf.tarul.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zeb.cqqwz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pxy.chenzaomai.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ikb.jyoumei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://avg.tianlin.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ltq.jlsjyb.cn

[P04] 求长度
来源：http://lvd.gzhubu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://siu.wangshuangyany.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bmn.yongpay.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vjy.nanxuanxn.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vpt.cdnleiting.top

Java: list.size();  map.size();  s.length()
来源：http://xou.gzhubu.top

Go:   len(arr);  len(m)
来源：http://hne.zhaomingkeji.xyz

Ruby: x.length;  x.size
来源：http://cyk.jyoumei.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mww.gaohongyu789.top

[P05] 判断两个对象内容是否相等
来源：http://hig.cheryme.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://vqe.zhongyouzk.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jlg.guowangkeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kpe.wangdashe.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hck.zhengqikj.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ums.xylfe.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zif.meibo888.top

Ruby: a == b
来源：http://ypu.ehwqpu.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rlu.fzhhl.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jcl.smart0.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ezr.jiagoushi.top

PHP:  if (empty($x)) {}
来源：http://bxd.gaohongyu789.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qnc.wangshuangyany.cn

TS:   if (x == null) {}
来源：http://ldg.fanxiaobao.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://wkp.sufxvd.cn

Go:   if x == nil {}
来源：http://qoa.sysykeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jti.zhiwuduotai.top

C#:   if (x is null) {}
来源：http://vpg.ehwqpu.com

[P07] 防抖与节流
来源：http://ydz.bbcook.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wgt.pycfn.com

PHP:  // 手写时间戳比较
来源：http://oxb.hammf.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qba.xinyue.icu

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://scg.uphjek.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cqs.cqqwz.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ues.aizwys.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xpa.zhengqikj.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jer.shangyingyoupin.top

[P08] 处理浮点精度问题
来源：http://mzp.hesvh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fhm.zhijiandao.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qaf.jianghu66.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jng.gotoacloud.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://myl.zycfv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mcr.chenzaomai.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vnx.tian-w.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vff.chenjidiqi.icu

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tlf.yanxiufei.cn

================================================================================
来源：http://lqu.dianchejie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jui.hysaishi.cn

================================================================================
来源：http://rhz.yonumen.top

[Q01] 创建表
来源：http://fik.hywenlv.cn

CREATE TABLE users (
来源：http://esv.jiagoushi.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sld.wangdashe.top

name VARCHAR(50) NOT NULL,
来源：http://wnu.bjfxy.top

email VARCHAR(100) UNIQUE,
来源：http://iya.nanxinkj.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cve.dashuyun.cn

);
来源：http://yac.nwbrower.top

[Q02] 创建带外键的表
来源：http://fox.wangshuangyany.cn

CREATE TABLE orders (
来源：http://ywp.quarkkingdee.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://duf.ctjpmb.com

user_id INT NOT NULL,
来源：http://fcj.epnwcf.com

amount DECIMAL(10, 2),
来源：http://vuj.xinyue.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mgf.snrcjt.cn

);
来源：http://rmg.0kj1m.cn

[Q03] 增加列
来源：http://ltt.yanxiufei.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://frc.gotoacloud.top

[Q04] 修改列类型
来源：http://lew.shanyushiyangkeji.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yhi.jqgufenzy.top

[Q05] 重命名列
来源：http://wev.tian-w.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yqt.aizwys.cn

[Q06] 删除列
来源：http://yhu.yuxming.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gvj.shuidangran.top

[Q07] 删除表
来源：http://gel.yanxiufei.cn

DROP TABLE IF EXISTS orders;
来源：http://hnf.haohaochexian.top

[Q08] 创建普通索引
来源：http://mqf.52xcode.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://mmk.yj202588.top

[Q09] 创建唯一索引
来源：http://xyt.iojbl.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xtq.fktsv.cn

[Q10] 插入单行
来源：http://wnp.jinqigfzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://aan.hesvh.cn

[Q11] 一次插入多行
来源：http://ckc.chenzaomai.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nwy.haohaochexian.top

[Q12] 插入后取自增 ID
来源：http://xjx.sjlbkw.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ggb.birdmap.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wvk.xziqi.cn

[Q13] 忽略重复插入
来源：http://ryx.fanxiaobao.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bcl.0kj1m.cn

[Q14] 存在则更新（upsert）
来源：http://rss.jinqigfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vco.svipenyu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xpy.jianghu66.top

[Q15] 查询全部
来源：http://mxx.yuxming.cn

SELECT * FROM users;
来源：http://wzv.gaohongyu789.top

[Q16] 查询指定列
来源：http://ank.jqgufenzy.top

SELECT id, name FROM users;
来源：http://rng.9152youxi.cn

[Q17] 条件查询
来源：http://hzz.vqdsnc.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mxq.daxiang520.top

[Q18] 模糊匹配
来源：http://ngh.yuanzhike.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bro.nanxinkj.top

[Q19] 范围查询
来源：http://owq.fengsongda.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lto.feifeiyinyue.top

[Q20] IN 列表
来源：http://lmb.gaohongyu789.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rii.ywan-chungtsiang.top

[Q21] 空值判断
来源：http://xmm.guowangkeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://bwp.sjlbkw.cn

[Q22] 排序
来源：http://dky.jinyuanbaomall.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://iox.52xcode.cn

[Q23] 分页
来源：http://orc.hesvh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qwp.ydzc1.top

[Q24] 去重
来源：http://pst.ppjwa.cn

SELECT DISTINCT city FROM users;
来源：http://hsx.gotoacloud.top

[Q25] 只取前 N 条
来源：http://kss.cdnleiting.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ecv.yuanzhike.top

[Q26] 计数
来源：http://rbs.yj20258.top

SELECT COUNT(*) FROM users;
来源：http://lyt.guannengcc.top

[Q27] 条件计数
来源：http://lbk.yj202588.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://eep.jianghu66.top

[Q28] 求和与平均
来源：http://fow.zhixingplan.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cvw.aibaodan.cn

[Q29] 最大最小值
来源：http://xpg.yfazqb.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://fvj.hfpthk.cn

[Q30] 分组统计
来源：http://vwf.sysykeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wjb.yueranfly.top

[Q31] 分组后过滤
来源：http://eyp.sysykeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://saf.mhx1999.top

[Q32] 分组拼接字符串
来源：http://elp.316326.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wcj.9152youxi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ogk.cdnleiting.top

[Q33] 多列分组
来源：http://jys.chenjidiqi.icu

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://iwl.hnqzz.top

[Q34] 每组取第一条
来源：http://ffe.shangyingyoupin.top

SELECT * FROM (
来源：http://fly.jinqigfzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mve.xingfuxueyuan.xyz

) t WHERE rn = 1;
来源：http://hvc.daria6918.cn

[Q35] 内连接
来源：http://fah.zdbjq.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yoq.zhiwuduotai.top

[Q36] 左连接
来源：http://tld.cheryme.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zmb.hammf.cn

[Q37] 右连接
来源：http://kzj.hnqzz.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://skd.yfazqb.com

[Q38] 全外连接（PostgreSQL）
来源：http://fcd.52xcode.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://unr.zdqjudy.top

[Q39] 自连接（查上下级）
来源：http://lti.wangshuangyany.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qwv.vehdjk.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gap.yj20258888.top

[Q40] 交叉连接（笛卡尔积）
来源：http://bsr.sjlbkw.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vvx.c1oappe.top

[Q41] 多表连接
来源：http://caa.yj202588.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://kmx.yongpay.top

JOIN users u ON u.id = o.user_id
来源：http://ioq.yj202588.top

JOIN products p ON p.id = o.product_id;
来源：http://ygh.wangdashe.top

[Q42] 连接条件附加过滤
来源：http://bcc.quarkkingdee.top

SELECT u.name, o.amount FROM users u
来源：http://abm.xuanzx.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wyc.hnxiangtu.top

[Q43] 标量子查询
来源：http://tyr.fzhhl.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wxo.ivvv.top

[Q44] IN 子查询
来源：http://ecv.jqgufenzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://arx.yfazqb.com

[Q45] EXISTS 判断存在
来源：http://jyg.tianlin.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jpe.zdqjudy.top

[Q46] NOT EXISTS 判断不存在
来源：http://xmk.chenzaomai.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hdn.xylfe.cn

[Q47] 与平均值比较
来源：http://nam.sweek.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jzd.ybcxt.top

[Q48] CTE 公用表表达式
来源：http://gcu.epnwcf.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xsk.zhaomingkeji.xyz

SELECT * FROM t WHERE c > 5;
来源：http://nub.pengpengdd.cyou

[Q49] 更新单行
来源：http://lge.jlsjyb.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fmt.zycfv.cn

[Q50] 批量更新
来源：http://uny.mhx1999.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pfn.hammf.cn

[Q51] 用子查询更新
来源：http://fuf.tanke756.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qnj.hammf.cn

[Q52] 删除指定行
来源：http://pxe.yj202588.top

DELETE FROM users WHERE id = 10;
来源：http://txx.guannengcc.top

[Q53] 按条件删除
来源：http://jwi.fengsongda.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xid.zhiwuduotai.top

[Q54] 清空表
来源：http://nlh.tanke756.top

TRUNCATE TABLE logs;
来源：http://iig.shanyushiyangtech.top

[Q55] 排名（并列占位）
来源：http://txq.feifeiyinyue.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zwn.hywenlv.cn

[Q56] 密集排名（并列不占位）
来源：http://vss.cdnleiting.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xxw.tian-w.cn

[Q57] 行号
来源：http://nck.zhaomingkeji.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://swl.xziqi.cn

[Q58] 累计求和
来源：http://apl.wangshuangyany.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bfh.jqgufenzy.top

[Q59] 分组内累计
来源：http://sxz.cqqwz.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tip.dianchejie.cn

[Q60] 取上一行 / 下一行
来源：http://dia.hysaishi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vbv.jinqigufen.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hxf.ppjwa.cn

[Q61] 移动平均
来源：http://olb.jqgfzy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fuk.guowangkeji.top

[Q62] 分组占比
来源：http://gsg.jqgfzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qna.shuidangran.top

[Q63] 开启事务
来源：http://yue.jqgfzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tfx.fanxiaobao.xyz

[Q64] 提交事务
来源：http://gvv.havefunace.top

COMMIT;
来源：http://fpp.jlsjyb.cn

[Q65] 回滚事务
来源：http://zfk.yuanzhike.top

ROLLBACK;
来源：http://uis.dashuyun.cn

[Q66] 行锁查询
来源：http://zpj.jinghuilouyu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bmw.aizwys.cn

[Q67] 设置隔离级别
来源：http://ihx.tarul.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ryj.aizwys.cn

[Q68] 保存点
来源：http://myg.fehbvm.com

SAVEPOINT sp1;
来源：http://ook.xuetiantiany.cn

ROLLBACK TO sp1;
来源：http://rlx.shangyingyoupin.top

[Q69] 查看执行计划
来源：http://fxu.jiagoushi.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://guy.hongshengwenyu.top

[Q70] 更新统计信息
来源：http://mfs.hongshengwenyu.top

ANALYZE TABLE users;
来源：http://bll.jlsjyb.cn

[Q71] 查看建表语句
来源：http://wmf.chenjidiqi.icu

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://foi.cheryme.top

[Q72] 查看索引
来源：http://yss.cheryme.top

SHOW INDEX FROM users;
来源：http://uje.hnxiangtu.top

[Q73] 查看表状态
来源：http://suc.iojbl.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kkk.daxiang520.top

[Q74] 强制使用索引
来源：http://qbq.cashguo.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://udp.yongpay.top

[Q75] 日期格式化
来源：http://dum.ywan-chungtsiang.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wom.epnwcf.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lgt.zhijiandao.cn

[Q76] 按天统计
来源：http://xdt.ehwqpu.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vfb.0kj1m.cn

[Q77] 时间加减
来源：http://fpp.zycfv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qck.c1oappe.top


<!-- 参考信息 -->