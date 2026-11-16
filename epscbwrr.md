代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://sux.shanyushiyangkeji.top

Go:   go f()
来源：http://mik.yfazqb.com

Ruby: Thread.new { f }
来源：http://rwo.yonumen.top

C#:   Task.Run(() => F());
来源：http://bju.sysykeji.top

[O02] 使用线程池
来源：http://odx.ybcxt.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qwc.nanxuanxn.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://exi.gotoacloud.top

JS:   // worker_threads 线程池
来源：http://mmd.aizwys.cn

TS:   // worker_threads 线程池
来源：http://cad.redwolf501.top

Java: Executors.newFixedThreadPool(4)
来源：http://osd.zdqjudy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lyx.tarul.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kgx.pycfn.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dbt.yvedp.cn

[O03] 加锁保护共享数据
来源：http://dda.dashuyun.cn

Py:   with lock: shared += 1
来源：http://ljm.hongshengwenyu.top

PHP:  // 用 flock() 做文件锁
来源：http://oiw.nanxinkj.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tvf.daxiang520.top

TS:   // 同 JS
来源：http://zbs.0kj1m.cn

Java: synchronized (this) { shared++; }
来源：http://vtb.nanxinkj.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qge.gzhubu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://hvi.iojbl.cn

C#:   lock (gate) { shared++; }
来源：http://jkt.yuxming.cn

[O04] 定义异步函数并等待
来源：http://avm.0kj1m.cn

Py:   async def f():⏎    await g()
来源：http://nfp.yj202588.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://apl.ydzc1.top

JS:   async function f() { await g(); }
来源：http://hxq.yuanzhike.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://lvf.jinyuanbaomall.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://leh.jqgufenzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://isg.ehwqpu.com

Ruby: # 用 Fiber 或 async gem
来源：http://ofd.chenlongwang.top

C#:   async Task F() { await G(); }
来源：http://hgn.c1oappe.top

[O05] 并发执行并等待全部完成
来源：http://nnc.pycfn.com

Py:   asyncio.gather(*tasks)
来源：http://dxc.sysykeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tds.hfpthk.cn

JS:   await Promise.all(tasks)
来源：http://dkj.ivvv.top

TS:   await Promise.all(tasks)
来源：http://voo.yonumen.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uri.sxryk.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://muj.mhx1999.top

Ruby: threads.map(&:join)
来源：http://rtr.ehwqpu.com

C#:   await Task.WhenAll(t1, t2)
来源：http://wbj.jlsjyb.cn

[O06] 使用进程池
来源：http://fuj.hfpthk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bam.52xcode.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://puu.meibo888.top

JS:   // child_process / cluster 模块
来源：http://fox.vehdjk.com

TS:   // child_process / cluster 模块
来源：http://zqs.epnwcf.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lyj.9152youxi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lge.fktsv.cn

Ruby: // fork 块
来源：http://uxy.andypj.xyz

C#:   Parallel.For
来源：http://soq.yuanzhike.top

================================================================================
来源：http://div.hysaishi.cn

P. 常用工具函数
来源：http://qun.hywenlv.cn

================================================================================
来源：http://yex.bjfxy.top

[P01] 生成 UUID
来源：http://nfw.uphjek.com

Py:   str(uuid.uuid4())
来源：http://iao.xylfe.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pxx.yueranfly.top

JS:   crypto.randomUUID()
来源：http://tpl.gotoacloud.top

TS:   crypto.randomUUID()
来源：http://jch.hysaishi.cn

Java: UUID.randomUUID().toString()
来源：http://lyi.hongshengwenyu.top

Go:   // 用 github.com/google/uuid
来源：http://mvm.gaohongyu789.top

Ruby: SecureRandom.uuid
来源：http://vhk.ywan-chungtsiang.top

C#:   Guid.NewGuid().ToString()
来源：http://skk.smart0.xyz

[P02] MD5 / SHA256 摘要
来源：http://ovx.meibo888.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mgn.wangdashe.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://cwe.uphjek.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fav.shanyushiyangtech.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yww.zdbjq.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xae.zhixingplan.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bps.sxryk.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yeq.ivvv.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ras.zhaomingkeji.xyz

[P03] 生成短随机字符串
来源：http://wdt.nanxinkj.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lte.zdbjq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://alm.tianlin.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jcv.jiagoushi.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wpw.vqdsnc.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qem.jinghuilouyu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xvg.yonumen.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://vxq.xziqi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ohr.tanke756.top

[P04] 求长度
来源：http://dcu.shanyushiyangtech.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ksv.daria6918.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zfc.316326.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xjh.zhijiandao.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kdh.zdqjudy.top

Java: list.size();  map.size();  s.length()
来源：http://thd.vqdsnc.cn

Go:   len(arr);  len(m)
来源：http://rtl.pycfn.com

Ruby: x.length;  x.size
来源：http://fjj.sysykeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dra.chenzaomai.com

[P05] 判断两个对象内容是否相等
来源：http://ejg.yuxming.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bah.gotoacloud.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mun.xuanzx.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lpp.ydzc1.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vqt.jinyuanbaomall.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vil.redwolf501.top

Go:   reflect.DeepEqual(a, b)
来源：http://nre.zhongyouzk.top

Ruby: a == b
来源：http://mjh.meibo888.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pan.dashuyun.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kyh.birdmap.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qqf.hammf.cn

PHP:  if (empty($x)) {}
来源：http://nrf.jianghu66.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://oty.bbcook.cn

TS:   if (x == null) {}
来源：http://rof.aibaodan.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lub.gogol.net.cn

Go:   if x == nil {}
来源：http://vww.meibo888.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wpn.epnwcf.com

C#:   if (x is null) {}
来源：http://kvs.sxryk.cn

[P07] 防抖与节流
来源：http://gbu.havefunace.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qel.aibaodan.cn

PHP:  // 手写时间戳比较
来源：http://boj.ehwqpu.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://njl.zycfv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ahp.yfazqb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://abi.yongpay.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ooq.ehwqpu.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://jna.redwolf501.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zfp.aizwys.cn

[P08] 处理浮点精度问题
来源：http://jeg.andypj.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gmv.zdqjudy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jfh.daxiang520.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mam.sxryk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lgc.ydzc1.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hme.yfazqb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kvs.yj20258888.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yce.sysykeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://svs.dianchejie.cn

================================================================================
来源：http://ovk.birdmap.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xfv.hysaishi.cn

================================================================================
来源：http://gpr.nanxinkj.top

[Q01] 创建表
来源：http://fbl.mhx1999.top

CREATE TABLE users (
来源：http://deo.snrcjt.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pzo.nanxinkj.top

name VARCHAR(50) NOT NULL,
来源：http://zoi.ivvv.top

email VARCHAR(100) UNIQUE,
来源：http://bxm.tanke756.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ckl.zhijiandao.cn

);
来源：http://cma.yuanzhike.top

[Q02] 创建带外键的表
来源：http://jut.zhongyouzk.top

CREATE TABLE orders (
来源：http://ubr.bjfxy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ivj.yueranfly.top

user_id INT NOT NULL,
来源：http://vtr.ehwqpu.com

amount DECIMAL(10, 2),
来源：http://zzm.hammf.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ces.chenzaomai.com

);
来源：http://rfv.jyoumei.cn

[Q03] 增加列
来源：http://mze.kuanghao11.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hor.fktsv.cn

[Q04] 修改列类型
来源：http://lhu.yanxiufei.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://aqx.xinyue.icu

[Q05] 重命名列
来源：http://bry.chenlongwang.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ann.zhaomingkeji.xyz

[Q06] 删除列
来源：http://gve.zdbjq.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gez.jyoumei.cn

[Q07] 删除表
来源：http://upk.pycfn.com

DROP TABLE IF EXISTS orders;
来源：http://lic.xingfuxueyuan.xyz

[Q08] 创建普通索引
来源：http://yxg.zhaomingkeji.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://hne.ehwqpu.com

[Q09] 创建唯一索引
来源：http://tyg.svipenyu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://twk.kuanghao11.cn

[Q10] 插入单行
来源：http://bsa.tian-w.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://irr.snrcjt.cn

[Q11] 一次插入多行
来源：http://dnb.shanyushiyangkeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lsw.tian-w.cn

[Q12] 插入后取自增 ID
来源：http://ieq.shuidangran.top

INSERT INTO users (name) VALUES ('C');
来源：http://jdo.fengsongda.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wjf.fengsongda.top

[Q13] 忽略重复插入
来源：http://sey.hysaishi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wev.sysykeji.top

[Q14] 存在则更新（upsert）
来源：http://ced.sxryk.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wbe.yonumen.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mck.feifeiyinyue.top

[Q15] 查询全部
来源：http://bgs.shanyushiyangtech.top

SELECT * FROM users;
来源：http://qsd.yonumen.top

[Q16] 查询指定列
来源：http://szn.havefunace.top

SELECT id, name FROM users;
来源：http://knf.hnxiangtu.top

[Q17] 条件查询
来源：http://eqx.zycfv.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jck.tanke756.top

[Q18] 模糊匹配
来源：http://zqu.cashguo.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wen.quarkkingdee.top

[Q19] 范围查询
来源：http://opg.hfpthk.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qdm.birdmap.top

[Q20] IN 列表
来源：http://eqq.ppjwa.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lip.havefunace.top

[Q21] 空值判断
来源：http://qwe.birdmap.top

SELECT * FROM users WHERE email IS NULL;
来源：http://jkk.yongpay.top

[Q22] 排序
来源：http://yhr.vehdjk.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yck.yfazqb.com

[Q23] 分页
来源：http://wso.aizwys.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ors.uphjek.com

[Q24] 去重
来源：http://frd.yj20258.top

SELECT DISTINCT city FROM users;
来源：http://rqb.zhaomingkeji.xyz

[Q25] 只取前 N 条
来源：http://qmg.hfpthk.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mvr.epnwcf.com

[Q26] 计数
来源：http://kze.guowangkeji.top

SELECT COUNT(*) FROM users;
来源：http://hli.cheryme.top

[Q27] 条件计数
来源：http://thb.jianghu66.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wpg.yuanzhike.top

[Q28] 求和与平均
来源：http://riz.guowangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kpw.dashuyun.cn

[Q29] 最大最小值
来源：http://psh.meibo888.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ydd.sweek.top

[Q30] 分组统计
来源：http://vlc.shangyingyoupin.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ucn.fehbvm.com

[Q31] 分组后过滤
来源：http://fxw.dianchejie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://agl.ydzc1.top

[Q32] 分组拼接字符串
来源：http://prq.fktsv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://emg.pengpengdd.cyou

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qjg.jyoumei.cn

[Q33] 多列分组
来源：http://wqp.chenlongwang.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jte.birdmap.top

[Q34] 每组取第一条
来源：http://vxz.andypj.xyz

SELECT * FROM (
来源：http://auq.pycfn.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qvb.xuetiantiany.cn

) t WHERE rn = 1;
来源：http://naq.snrcjt.cn

[Q35] 内连接
来源：http://clz.hnqzz.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tvu.cucudq.cn

[Q36] 左连接
来源：http://yat.pengpengdd.cyou

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://aiq.tanke756.top

[Q37] 右连接
来源：http://tmj.cucudq.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://njk.birdmap.top

[Q38] 全外连接（PostgreSQL）
来源：http://nmq.cheryme.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oza.yueranfly.top

[Q39] 自连接（查上下级）
来源：http://lqz.meibo888.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://sme.fzhhl.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vtr.dianchejie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wtt.sxryk.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hlt.shanyushiyangkeji.top

[Q41] 多表连接
来源：http://kso.yuanzhike.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://myq.hammf.cn

JOIN users u ON u.id = o.user_id
来源：http://ffa.fehbvm.com

JOIN products p ON p.id = o.product_id;
来源：http://uev.yfazqb.com

[Q42] 连接条件附加过滤
来源：http://auo.jianghu66.top

SELECT u.name, o.amount FROM users u
来源：http://vwu.jyoumei.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://igv.dianchejie.cn

[Q43] 标量子查询
来源：http://jnf.sxryk.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ixi.yuxming.cn

[Q44] IN 子查询
来源：http://les.cheryme.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://enx.sxryk.cn

[Q45] EXISTS 判断存在
来源：http://tww.hfpthk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kqt.yangfankeji.com

[Q46] NOT EXISTS 判断不存在
来源：http://mdq.dashuyun.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rut.iojbl.cn

[Q47] 与平均值比较
来源：http://rfn.gotoacloud.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ahj.hcnkem.com

[Q48] CTE 公用表表达式
来源：http://etj.yuanzhike.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tfe.cucudq.cn

SELECT * FROM t WHERE c > 5;
来源：http://bid.svipenyu.cn

[Q49] 更新单行
来源：http://uxv.xuetiantiany.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yhu.ywan-chungtsiang.top

[Q50] 批量更新
来源：http://ayk.sysykeji.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ggz.cqqwz.cn

[Q51] 用子查询更新
来源：http://lrp.hnxiangtu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fvg.kuanghao11.cn

[Q52] 删除指定行
来源：http://xml.bbcook.cn

DELETE FROM users WHERE id = 10;
来源：http://dcn.zhiwuduotai.top

[Q53] 按条件删除
来源：http://vyt.guowangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qkz.nwbrower.top

[Q54] 清空表
来源：http://lcv.tianlin.xyz

TRUNCATE TABLE logs;
来源：http://pzm.jinghuilouyu.cn

[Q55] 排名（并列占位）
来源：http://raj.bjfxy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://euv.wangshuangyany.cn

[Q56] 密集排名（并列不占位）
来源：http://rdk.ppjwa.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vgx.ehwqpu.com

[Q57] 行号
来源：http://gtr.aibaodan.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://imv.c1oappe.top

[Q58] 累计求和
来源：http://wlf.yj20258888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pfh.tianlin.xyz

[Q59] 分组内累计
来源：http://isk.yongpay.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://scy.vqdsnc.cn

[Q60] 取上一行 / 下一行
来源：http://uvv.chenzaomai.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sxg.jqgfzy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zas.yongpay.top

[Q61] 移动平均
来源：http://ejl.fengsongda.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lyr.zhiwuduotai.top

[Q62] 分组占比
来源：http://zid.pengpengdd.cyou

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://eqk.xylfe.cn

[Q63] 开启事务
来源：http://vgb.hnqzz.top

START TRANSACTION;                -- 或 BEGIN
来源：http://rlq.shanyushiyangkeji.top

[Q64] 提交事务
来源：http://jqo.zhijiandao.cn

COMMIT;
来源：http://vie.xuanzx.com

[Q65] 回滚事务
来源：http://btm.sjlbkw.cn

ROLLBACK;
来源：http://csh.svipenyu.cn

[Q66] 行锁查询
来源：http://ozk.snrcjt.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fwe.gaohongyu789.top

[Q67] 设置隔离级别
来源：http://cru.nanxuanxn.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://itn.xingfuxueyuan.xyz

[Q68] 保存点
来源：http://pfx.gaohongyu789.top

SAVEPOINT sp1;
来源：http://iwh.fengsongda.top

ROLLBACK TO sp1;
来源：http://lhp.ppjwa.cn

[Q69] 查看执行计划
来源：http://ach.ybcxt.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nlf.9152youxi.cn

[Q70] 更新统计信息
来源：http://pha.redwolf501.top

ANALYZE TABLE users;
来源：http://qco.jinghuilouyu.cn

[Q71] 查看建表语句
来源：http://dwm.shuidangran.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://unk.xylfe.cn

[Q72] 查看索引
来源：http://tla.birdmap.top

SHOW INDEX FROM users;
来源：http://oat.hcnkem.com

[Q73] 查看表状态
来源：http://cxb.quarkkingdee.top

SHOW TABLE STATUS LIKE 'users';
来源：http://opa.kuanghao11.cn

[Q74] 强制使用索引
来源：http://njq.zdbjq.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://eqt.hfpthk.cn

[Q75] 日期格式化
来源：http://amg.316326.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bfo.ydzc1.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pjr.meibo888.top


<!-- 参考信息 -->