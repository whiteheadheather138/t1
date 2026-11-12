代发 wailian999

TS:   // worker_threads 线程池
来源：http://oag.gotoacloud.top

Java: Executors.newFixedThreadPool(4)
来源：http://sfr.ehwqpu.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ttl.ydzc1.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bwd.feifeiyinyue.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://eef.yfazqb.com

[O03] 加锁保护共享数据
来源：http://wbw.zhoulong.xyz

Py:   with lock: shared += 1
来源：http://hwv.jianghu66.top

PHP:  // 用 flock() 做文件锁
来源：http://uhh.yj20258.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vws.zdqjudy.top

TS:   // 同 JS
来源：http://nyr.hongshengwenyu.top

Java: synchronized (this) { shared++; }
来源：http://cve.andypj.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xit.52xcode.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://idd.shangyingyoupin.top

C#:   lock (gate) { shared++; }
来源：http://icj.bbcook.cn

[O04] 定义异步函数并等待
来源：http://brx.jiagoushi.top

Py:   async def f():⏎    await g()
来源：http://hdp.xinyue.icu

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mhj.hesvh.cn

JS:   async function f() { await g(); }
来源：http://pio.jinqigfzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://pgh.yj20258888.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nky.ivvv.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jzf.jinghuilouyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mwt.shzxlz.cn

C#:   async Task F() { await G(); }
来源：http://txv.fktsv.cn

[O05] 并发执行并等待全部完成
来源：http://bmi.hywenlv.cn

Py:   asyncio.gather(*tasks)
来源：http://jvw.iojbl.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fea.sufxvd.cn

JS:   await Promise.all(tasks)
来源：http://lwq.yonumen.top

TS:   await Promise.all(tasks)
来源：http://tmr.birdmap.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pis.jianghu66.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qqg.zhengqikj.top

Ruby: threads.map(&:join)
来源：http://ujl.tarul.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tgr.c1oappe.top

[O06] 使用进程池
来源：http://hpq.kuanghao11.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pgm.havefunace.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ddx.cqqwz.cn

JS:   // child_process / cluster 模块
来源：http://pvv.snrcjt.cn

TS:   // child_process / cluster 模块
来源：http://qbj.ehwqpu.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xic.vehdjk.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lem.jqgfzy.top

Ruby: // fork 块
来源：http://aso.jyoumei.cn

C#:   Parallel.For
来源：http://xfv.tianlin.xyz

================================================================================
来源：http://bbu.hywenlv.cn

P. 常用工具函数
来源：http://hdh.jinghuilouyu.cn

================================================================================
来源：http://srk.sxryk.cn

[P01] 生成 UUID
来源：http://rvg.shanyushiyangkeji.top

Py:   str(uuid.uuid4())
来源：http://xxc.316326.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tok.xinyue.icu

JS:   crypto.randomUUID()
来源：http://qnn.hcnkem.com

TS:   crypto.randomUUID()
来源：http://moi.tian-w.cn

Java: UUID.randomUUID().toString()
来源：http://lka.xylfe.cn

Go:   // 用 github.com/google/uuid
来源：http://ygo.dianchejie.cn

Ruby: SecureRandom.uuid
来源：http://npp.shangyingyoupin.top

C#:   Guid.NewGuid().ToString()
来源：http://urq.fanxiaobao.xyz

[P02] MD5 / SHA256 摘要
来源：http://xzr.xinyue.icu

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pof.ehwqpu.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://pyt.svipenyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oxt.52xcode.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kjy.ybcxt.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ptw.aizwys.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baz.fanxiaobao.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mpf.shzxlz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://aya.yuanzhike.top

[P03] 生成短随机字符串
来源：http://ujj.fengsongda.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://faw.yuxming.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yrv.yj20258888.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lnc.ppjwa.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kqm.ivvv.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gaz.zdbjq.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://oug.nwbrower.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://hto.yanxiufei.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xbr.ybcxt.top

[P04] 求长度
来源：http://ezd.hongshengwenyu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ear.jinqigufen.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cgy.feifeiyinyue.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ulx.ywan-chungtsiang.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yim.havefunace.top

Java: list.size();  map.size();  s.length()
来源：http://suh.zdbjq.cn

Go:   len(arr);  len(m)
来源：http://hsv.jinqigufen.top

Ruby: x.length;  x.size
来源：http://kfv.zhixingplan.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://izi.52xcode.cn

[P05] 判断两个对象内容是否相等
来源：http://exd.yueranfly.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://bsd.yangfankeji.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tcr.yfazqb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://eta.tian-w.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gnd.cqqwz.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gnq.wangshuangyany.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jml.zhiwuduotai.top

Ruby: a == b
来源：http://eby.tian-w.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fxx.hesvh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://efc.yj202588.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zcm.svipenyu.cn

PHP:  if (empty($x)) {}
来源：http://xmj.sufxvd.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rpm.xuanzx.com

TS:   if (x == null) {}
来源：http://ivv.shanyushiyangtech.top

Java: if (x == null || x.isEmpty()) {}
来源：http://kuz.jiagoushi.top

Go:   if x == nil {}
来源：http://wtm.quarkkingdee.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ryw.jianghu66.top

C#:   if (x is null) {}
来源：http://ipa.fengsongda.top

[P07] 防抖与节流
来源：http://mct.tanke756.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bbl.xziqi.cn

PHP:  // 手写时间戳比较
来源：http://tpw.jiagoushi.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vcb.bjfxy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vtd.iojbl.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sfn.meibo888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://osu.fehbvm.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://dki.guannengcc.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pmv.nanxinkj.top

[P08] 处理浮点精度问题
来源：http://mcu.shanyushiyangkeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sbz.vqdsnc.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kme.fzhhl.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cmo.hongshengwenyu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hos.bbcook.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pxq.zhaomingkeji.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wmn.hnxiangtu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qtl.tian-w.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fjn.birdmap.top

================================================================================
来源：http://iqh.fehbvm.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bmn.vehdjk.com

================================================================================
来源：http://thn.bbcook.cn

[Q01] 创建表
来源：http://tru.yanxiufei.cn

CREATE TABLE users (
来源：http://lzb.jyoumei.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xxi.aibaodan.cn

name VARCHAR(50) NOT NULL,
来源：http://qmn.hcnkem.com

email VARCHAR(100) UNIQUE,
来源：http://mha.svipenyu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jci.cashguo.top

);
来源：http://yxb.ctjpmb.com

[Q02] 创建带外键的表
来源：http://hfl.tanke756.top

CREATE TABLE orders (
来源：http://jzh.shanyushiyangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kem.zhoulong.xyz

user_id INT NOT NULL,
来源：http://txb.sysykeji.top

amount DECIMAL(10, 2),
来源：http://hxw.jqgufenzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://swv.gzhubu.top

);
来源：http://jkx.dashuyun.cn

[Q03] 增加列
来源：http://awf.fehbvm.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://flq.pengpengdd.cyou

[Q04] 修改列类型
来源：http://txh.316326.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uxz.zhaomingkeji.xyz

[Q05] 重命名列
来源：http://lcn.hfpthk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rqb.zhaomingkeji.xyz

[Q06] 删除列
来源：http://lab.chenlongwang.top

ALTER TABLE users DROP COLUMN age;
来源：http://vim.yanxiufei.cn

[Q07] 删除表
来源：http://dur.fanxiaobao.xyz

DROP TABLE IF EXISTS orders;
来源：http://lja.jyoumei.cn

[Q08] 创建普通索引
来源：http://xxv.ywan-chungtsiang.top

CREATE INDEX idx_users_email ON users(email);
来源：http://eeo.daria6918.cn

[Q09] 创建唯一索引
来源：http://smj.yuxming.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rof.jinqigfzy.top

[Q10] 插入单行
来源：http://llo.yj202588.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ijr.nwbrower.top

[Q11] 一次插入多行
来源：http://nep.tanke756.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ipo.pycfn.com

[Q12] 插入后取自增 ID
来源：http://yuf.xuanzx.com

INSERT INTO users (name) VALUES ('C');
来源：http://ifo.yvedp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wjy.cqqwz.cn

[Q13] 忽略重复插入
来源：http://sml.sjlbkw.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://doj.snrcjt.cn

[Q14] 存在则更新（upsert）
来源：http://odb.uphjek.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uyj.0kj1m.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lns.zdqjudy.top

[Q15] 查询全部
来源：http://cbq.fehbvm.com

SELECT * FROM users;
来源：http://bxx.dashuyun.cn

[Q16] 查询指定列
来源：http://ljq.pycfn.com

SELECT id, name FROM users;
来源：http://pcc.zhixingplan.top

[Q17] 条件查询
来源：http://ztx.xuetiantiany.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hbn.hcnkem.com

[Q18] 模糊匹配
来源：http://iau.aizwys.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wkd.chenlongwang.top

[Q19] 范围查询
来源：http://ayz.fanxiaobao.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vfx.yanxiufei.cn

[Q20] IN 列表
来源：http://rns.fzhhl.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bei.jyoumei.cn

[Q21] 空值判断
来源：http://kxd.aibaodan.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mzf.redwolf501.top

[Q22] 排序
来源：http://skg.hysaishi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xsx.hcnkem.com

[Q23] 分页
来源：http://nyw.bbcook.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ufi.pycfn.com

[Q24] 去重
来源：http://czk.fktsv.cn

SELECT DISTINCT city FROM users;
来源：http://vml.daria6918.cn

[Q25] 只取前 N 条
来源：http://exr.vehdjk.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jvm.hnxiangtu.top

[Q26] 计数
来源：http://nsi.feifeiyinyue.top

SELECT COUNT(*) FROM users;
来源：http://grc.ywan-chungtsiang.top

[Q27] 条件计数
来源：http://ous.feifeiyinyue.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://niq.ybcxt.top

[Q28] 求和与平均
来源：http://zcb.sweek.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lbg.hongshengwenyu.top

[Q29] 最大最小值
来源：http://lrc.chenjidiqi.icu

SELECT MAX(age), MIN(age) FROM users;
来源：http://orb.yj20258888.top

[Q30] 分组统计
来源：http://bvb.hysaishi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uuk.guannengcc.top

[Q31] 分组后过滤
来源：http://tfv.shuidangran.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pir.gotoacloud.top

[Q32] 分组拼接字符串
来源：http://ssb.xuanzx.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://icl.jqgfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rrn.gaohongyu789.top

[Q33] 多列分组
来源：http://fip.fehbvm.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rgg.cheryme.top

[Q34] 每组取第一条
来源：http://plf.yangfankeji.com

SELECT * FROM (
来源：http://zso.shangyingyoupin.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bms.pycfn.com

) t WHERE rn = 1;
来源：http://unw.316326.xyz

[Q35] 内连接
来源：http://xkc.bjfxy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://com.havefunace.top

[Q36] 左连接
来源：http://tfu.aizwys.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nxx.hfpthk.cn

[Q37] 右连接
来源：http://hwt.bbcook.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rkh.yonumen.top

[Q38] 全外连接（PostgreSQL）
来源：http://sea.yueranfly.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pyf.aibaodan.cn

[Q39] 自连接（查上下级）
来源：http://fxm.tian-w.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://edt.yvedp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://njw.havefunace.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ntv.cqqwz.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kzi.ctjpmb.com

[Q41] 多表连接
来源：http://ctc.hnxiangtu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://pdp.hnqzz.top

JOIN users u ON u.id = o.user_id
来源：http://yrl.hcnkem.com

JOIN products p ON p.id = o.product_id;
来源：http://eow.gogol.net.cn

[Q42] 连接条件附加过滤
来源：http://guc.shzxlz.cn

SELECT u.name, o.amount FROM users u
来源：http://adv.0kj1m.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cxt.ivvv.top

[Q43] 标量子查询
来源：http://yob.xingfuxueyuan.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dse.jinghuilouyu.cn

[Q44] IN 子查询
来源：http://xpu.mhx1999.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qib.tian-w.cn

[Q45] EXISTS 判断存在
来源：http://agq.fehbvm.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qwd.ivvv.top

[Q46] NOT EXISTS 判断不存在
来源：http://uaw.xingfuxueyuan.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cam.hesvh.cn

[Q47] 与平均值比较
来源：http://mlk.hammf.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vln.gogol.net.cn

[Q48] CTE 公用表表达式
来源：http://mwd.xuanzx.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://piu.xuetiantiany.cn

SELECT * FROM t WHERE c > 5;
来源：http://xgd.ydzc1.top

[Q49] 更新单行
来源：http://pvw.yj20258888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dyi.andypj.xyz

[Q50] 批量更新
来源：http://luc.shuidangran.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tku.fanxiaobao.xyz

[Q51] 用子查询更新
来源：http://qad.zhijiandao.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iah.hnxiangtu.top

[Q52] 删除指定行
来源：http://ciu.hysaishi.cn

DELETE FROM users WHERE id = 10;
来源：http://efa.shuidangran.top

[Q53] 按条件删除
来源：http://xrb.gotoacloud.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ptu.jinqigfzy.top

[Q54] 清空表
来源：http://jox.shanyushiyangkeji.top

TRUNCATE TABLE logs;
来源：http://son.zhongyouzk.top

[Q55] 排名（并列占位）
来源：http://efy.jyoumei.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cev.daria6918.cn

[Q56] 密集排名（并列不占位）
来源：http://rch.chenzaomai.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sfq.c1oappe.top

[Q57] 行号
来源：http://agq.chenlongwang.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jof.52xcode.cn

[Q58] 累计求和
来源：http://kxm.jianghu66.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jiy.yanxiufei.cn

[Q59] 分组内累计
来源：http://ofy.c1oappe.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vjv.jiagoushi.top

[Q60] 取上一行 / 下一行
来源：http://zqw.hywenlv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://agb.zdqjudy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://eea.ctjpmb.com

[Q61] 移动平均
来源：http://tnp.c1oappe.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://udb.aizwys.cn

[Q62] 分组占比
来源：http://ysz.gogol.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://szj.0kj1m.cn

[Q63] 开启事务
来源：http://qvb.jqgufenzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://pmm.nanxuanxn.top

[Q64] 提交事务
来源：http://mmm.zhoulong.xyz

COMMIT;
来源：http://rto.yanxiufei.cn

[Q65] 回滚事务
来源：http://wsk.svipenyu.cn

ROLLBACK;
来源：http://hch.svipenyu.cn

[Q66] 行锁查询
来源：http://jxs.guannengcc.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ryi.zhijiandao.cn

[Q67] 设置隔离级别
来源：http://dab.birdmap.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jpz.fzhhl.top

[Q68] 保存点
来源：http://xss.yanxiufei.cn

SAVEPOINT sp1;
来源：http://zdi.hysaishi.cn

ROLLBACK TO sp1;
来源：http://fht.sysykeji.top

[Q69] 查看执行计划
来源：http://igv.hysaishi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wwv.birdmap.top

[Q70] 更新统计信息
来源：http://tum.chenlongwang.top

ANALYZE TABLE users;
来源：http://ial.jinqigufen.top

[Q71] 查看建表语句
来源：http://kvb.0kj1m.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://okx.ywan-chungtsiang.top

[Q72] 查看索引
来源：http://ome.bjfxy.top

SHOW INDEX FROM users;
来源：http://ftg.cdnleiting.top

[Q73] 查看表状态
来源：http://xgb.jiagoushi.top

SHOW TABLE STATUS LIKE 'users';
来源：http://tza.jlsjyb.cn

[Q74] 强制使用索引
来源：http://dyk.fanxiaobao.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sxx.dashuyun.cn

[Q75] 日期格式化
来源：http://rmt.zhoulong.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gli.cdnleiting.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wew.zhixingplan.top

[Q76] 按天统计
来源：http://mpx.daria6918.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rvh.jinqigufen.top

[Q77] 时间加减
来源：http://osr.jinqigfzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nlh.hongshengwenyu.top

[Q78] 当前时间
来源：http://ttr.cucudq.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mrd.cqqwz.cn

[Q79] 字符串拼接
来源：http://aul.fzhhl.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ecq.yangfankeji.com


<!-- 参考信息 -->