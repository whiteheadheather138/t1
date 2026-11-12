代发 wailian999

[O02] 使用线程池
来源：http://ldr.tian-w.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kig.pycfn.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qvn.meibo888.top

JS:   // worker_threads 线程池
来源：http://lpu.yj202588.top

TS:   // worker_threads 线程池
来源：http://nun.redwolf501.top

Java: Executors.newFixedThreadPool(4)
来源：http://lsp.ehwqpu.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ezd.zdbjq.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tij.uphjek.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://efl.wangshuangyany.cn

[O03] 加锁保护共享数据
来源：http://lfr.xuanzx.com

Py:   with lock: shared += 1
来源：http://ocv.svipenyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://qpg.daxiang520.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xpt.daxiang520.top

TS:   // 同 JS
来源：http://yic.kuanghao11.cn

Java: synchronized (this) { shared++; }
来源：http://bjo.jyoumei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zys.sjlbkw.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://otx.yongpay.top

C#:   lock (gate) { shared++; }
来源：http://gwx.nanxinkj.top

[O04] 定义异步函数并等待
来源：http://itk.hesvh.cn

Py:   async def f():⏎    await g()
来源：http://fen.hesvh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://svr.zdbjq.cn

JS:   async function f() { await g(); }
来源：http://rdn.aizwys.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xim.hfpthk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xfq.uphjek.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kjb.nwbrower.top

Ruby: # 用 Fiber 或 async gem
来源：http://rcq.nwbrower.top

C#:   async Task F() { await G(); }
来源：http://vrb.quarkkingdee.top

[O05] 并发执行并等待全部完成
来源：http://poh.hywenlv.cn

Py:   asyncio.gather(*tasks)
来源：http://vjk.shuidangran.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ibj.pengpengdd.cyou

JS:   await Promise.all(tasks)
来源：http://qtv.dianchejie.cn

TS:   await Promise.all(tasks)
来源：http://kcc.xziqi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://epo.shangyingyoupin.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xpx.jqgufenzy.top

Ruby: threads.map(&:join)
来源：http://fee.jlsjyb.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pgr.guannengcc.top

[O06] 使用进程池
来源：http://lgs.sysykeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pid.sxryk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://sdm.zhengqikj.top

JS:   // child_process / cluster 模块
来源：http://ukv.ywan-chungtsiang.top

TS:   // child_process / cluster 模块
来源：http://ksr.ywan-chungtsiang.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rbp.hfpthk.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://soh.tianlin.xyz

Ruby: // fork 块
来源：http://fqm.yj20258.top

C#:   Parallel.For
来源：http://ceu.sufxvd.cn

================================================================================
来源：http://ufo.svipenyu.cn

P. 常用工具函数
来源：http://vza.fanxiaobao.xyz

================================================================================
来源：http://bqm.zhengqikj.top

[P01] 生成 UUID
来源：http://mns.daria6918.cn

Py:   str(uuid.uuid4())
来源：http://ybq.nwbrower.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://udv.sjlbkw.cn

JS:   crypto.randomUUID()
来源：http://mni.chenzaomai.com

TS:   crypto.randomUUID()
来源：http://fnl.dashuyun.cn

Java: UUID.randomUUID().toString()
来源：http://xts.zdqjudy.top

Go:   // 用 github.com/google/uuid
来源：http://vca.meibo888.top

Ruby: SecureRandom.uuid
来源：http://mst.quarkkingdee.top

C#:   Guid.NewGuid().ToString()
来源：http://yow.daria6918.cn

[P02] MD5 / SHA256 摘要
来源：http://wqj.xylfe.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qmd.zdqjudy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://gkn.epnwcf.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jtk.ehwqpu.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sgs.jinqigufen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oup.chenlongwang.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hnu.yueranfly.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://emv.316326.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://asv.pengpengdd.cyou

[P03] 生成短随机字符串
来源：http://cdb.sweek.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ahz.tian-w.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kpn.jinqigfzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lim.vqdsnc.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lfn.chenlongwang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://reb.pengpengdd.cyou

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wkq.tian-w.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://iuo.zdbjq.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yff.zhoulong.xyz

[P04] 求长度
来源：http://doa.shanyushiyangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pbj.quarkkingdee.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://roj.dashuyun.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dyk.pycfn.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qjr.yj20258.top

Java: list.size();  map.size();  s.length()
来源：http://cqh.hammf.cn

Go:   len(arr);  len(m)
来源：http://qok.jqgfzy.top

Ruby: x.length;  x.size
来源：http://azt.tarul.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://nfb.ppjwa.cn

[P05] 判断两个对象内容是否相等
来源：http://kzw.sysykeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://syi.gzhubu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yid.hfpthk.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nun.nwbrower.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zww.zycfv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://juw.cqqwz.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fmb.yanxiufei.cn

Ruby: a == b
来源：http://zuv.iojbl.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ocl.xziqi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sfq.hnqzz.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fqw.jinghuilouyu.cn

PHP:  if (empty($x)) {}
来源：http://ymo.yonumen.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qsk.dashuyun.cn

TS:   if (x == null) {}
来源：http://vgd.hnqzz.top

Java: if (x == null || x.isEmpty()) {}
来源：http://xbw.tian-w.cn

Go:   if x == nil {}
来源：http://wpd.yongpay.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pwz.shzxlz.cn

C#:   if (x is null) {}
来源：http://mgb.sxryk.cn

[P07] 防抖与节流
来源：http://kbn.vqdsnc.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vjs.yuanzhike.top

PHP:  // 手写时间戳比较
来源：http://ixx.pengpengdd.cyou

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gcc.sysykeji.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ije.cdnleiting.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jzh.fzhhl.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://abx.vqdsnc.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dqu.jinqigfzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lja.bjfxy.top

[P08] 处理浮点精度问题
来源：http://bot.zhijiandao.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://byz.jiagoushi.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tcd.xylfe.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xlp.daria6918.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jxg.yueranfly.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hpj.xuetiantiany.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hyi.vehdjk.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ska.jyoumei.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://eua.yj20258.top

================================================================================
来源：http://quy.hongshengwenyu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fdv.yvedp.cn

================================================================================
来源：http://xeu.nanxinkj.top

[Q01] 创建表
来源：http://epo.uphjek.com

CREATE TABLE users (
来源：http://crq.fzhhl.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://liv.feifeiyinyue.top

name VARCHAR(50) NOT NULL,
来源：http://zln.mhx1999.top

email VARCHAR(100) UNIQUE,
来源：http://rdx.fengsongda.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://arh.vqdsnc.cn

);
来源：http://dag.haohaochexian.top

[Q02] 创建带外键的表
来源：http://wds.xingfuxueyuan.xyz

CREATE TABLE orders (
来源：http://qbl.cheryme.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://aug.shanyushiyangtech.top

user_id INT NOT NULL,
来源：http://juw.hongshengwenyu.top

amount DECIMAL(10, 2),
来源：http://hum.gogol.net.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jmy.svipenyu.cn

);
来源：http://lgc.yj20258888.top

[Q03] 增加列
来源：http://fjo.tianlin.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qqx.jqgufenzy.top

[Q04] 修改列类型
来源：http://gyj.9152youxi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qwk.wangdashe.top

[Q05] 重命名列
来源：http://rxf.kuanghao11.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ryh.vqdsnc.cn

[Q06] 删除列
来源：http://wdy.wangshuangyany.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dse.gotoacloud.top

[Q07] 删除表
来源：http://cpq.xuanzx.com

DROP TABLE IF EXISTS orders;
来源：http://rqm.jinqigufen.top

[Q08] 创建普通索引
来源：http://uij.sjlbkw.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wbg.ctjpmb.com

[Q09] 创建唯一索引
来源：http://exr.hammf.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ymr.uphjek.com

[Q10] 插入单行
来源：http://goj.cheryme.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lwj.gaohongyu789.top

[Q11] 一次插入多行
来源：http://pih.hfpthk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://aos.yuxming.cn

[Q12] 插入后取自增 ID
来源：http://tsd.jinghuilouyu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fur.ywan-chungtsiang.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zez.ivvv.top

[Q13] 忽略重复插入
来源：http://ncf.ppjwa.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vwt.ywan-chungtsiang.top

[Q14] 存在则更新（upsert）
来源：http://bpg.zycfv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qvn.dianchejie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qst.hesvh.cn

[Q15] 查询全部
来源：http://pwu.yfazqb.com

SELECT * FROM users;
来源：http://ysk.snrcjt.cn

[Q16] 查询指定列
来源：http://zcc.yangfankeji.com

SELECT id, name FROM users;
来源：http://aiv.jqgfzy.top

[Q17] 条件查询
来源：http://xgq.ehwqpu.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jwm.316326.xyz

[Q18] 模糊匹配
来源：http://pia.hywenlv.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gwv.zhixingplan.top

[Q19] 范围查询
来源：http://urb.hcnkem.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hsf.yangfankeji.com

[Q20] IN 列表
来源：http://ukf.nanxuanxn.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cek.zycfv.cn

[Q21] 空值判断
来源：http://mrj.tianlin.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://rbq.nanxinkj.top

[Q22] 排序
来源：http://zlf.pengpengdd.cyou

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://iur.aizwys.cn

[Q23] 分页
来源：http://oeg.cheryme.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rhk.aizwys.cn

[Q24] 去重
来源：http://zag.chenjidiqi.icu

SELECT DISTINCT city FROM users;
来源：http://fvm.feifeiyinyue.top

[Q25] 只取前 N 条
来源：http://hxw.tianlin.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ksq.yj202588.top

[Q26] 计数
来源：http://ufc.redwolf501.top

SELECT COUNT(*) FROM users;
来源：http://hkn.daria6918.cn

[Q27] 条件计数
来源：http://hac.sysykeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://auz.hesvh.cn

[Q28] 求和与平均
来源：http://acu.sxryk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vei.cashguo.top

[Q29] 最大最小值
来源：http://pyi.yvedp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vdl.zhengqikj.top

[Q30] 分组统计
来源：http://meb.yj20258.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qnd.ppjwa.cn

[Q31] 分组后过滤
来源：http://kxd.chenlongwang.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xiz.daxiang520.top

[Q32] 分组拼接字符串
来源：http://wpn.gzhubu.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://emq.jyoumei.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dub.shuidangran.top

[Q33] 多列分组
来源：http://cpl.quarkkingdee.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lqn.jinghuilouyu.cn

[Q34] 每组取第一条
来源：http://szy.andypj.xyz

SELECT * FROM (
来源：http://mdu.nanxinkj.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ksx.pycfn.com

) t WHERE rn = 1;
来源：http://hja.hfpthk.cn

[Q35] 内连接
来源：http://piv.guannengcc.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mvu.snrcjt.cn

[Q36] 左连接
来源：http://zbd.shzxlz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zkl.pengpengdd.cyou

[Q37] 右连接
来源：http://owr.zdbjq.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zpf.xuanzx.com

[Q38] 全外连接（PostgreSQL）
来源：http://dal.hysaishi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://feu.hysaishi.cn

[Q39] 自连接（查上下级）
来源：http://fns.chenzaomai.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://ibh.gotoacloud.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://eqd.haohaochexian.top

[Q40] 交叉连接（笛卡尔积）
来源：http://vfw.tarul.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://aci.pengpengdd.cyou

[Q41] 多表连接
来源：http://pbv.hnxiangtu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://uzb.hongshengwenyu.top

JOIN users u ON u.id = o.user_id
来源：http://hkv.redwolf501.top

JOIN products p ON p.id = o.product_id;
来源：http://tss.fengsongda.top

[Q42] 连接条件附加过滤
来源：http://irm.feifeiyinyue.top

SELECT u.name, o.amount FROM users u
来源：http://mle.bjfxy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tzm.yj20258888.top

[Q43] 标量子查询
来源：http://ksy.zhongyouzk.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dmj.yueranfly.top

[Q44] IN 子查询
来源：http://ukj.sufxvd.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bhw.gzhubu.top

[Q45] EXISTS 判断存在
来源：http://lqu.52xcode.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jrj.tianlin.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://ceu.quarkkingdee.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hgy.tian-w.cn

[Q47] 与平均值比较
来源：http://yjb.andypj.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fkp.sjlbkw.cn

[Q48] CTE 公用表表达式
来源：http://cyk.yuxming.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tqo.gzhubu.top

SELECT * FROM t WHERE c > 5;
来源：http://boi.zdqjudy.top

[Q49] 更新单行
来源：http://nyc.sysykeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mkw.nanxinkj.top

[Q50] 批量更新
来源：http://svu.feifeiyinyue.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vuy.yueranfly.top

[Q51] 用子查询更新
来源：http://vgh.fzhhl.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sfu.sysykeji.top

[Q52] 删除指定行
来源：http://mrh.yuxming.cn

DELETE FROM users WHERE id = 10;
来源：http://ugp.shanyushiyangkeji.top

[Q53] 按条件删除
来源：http://nee.ydzc1.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fnu.cdnleiting.top

[Q54] 清空表
来源：http://djg.gzhubu.top

TRUNCATE TABLE logs;
来源：http://rmo.jyoumei.cn

[Q55] 排名（并列占位）
来源：http://zhb.gogol.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gyt.jinyuanbaomall.cn

[Q56] 密集排名（并列不占位）
来源：http://vdt.yonumen.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fbt.yj20258.top

[Q57] 行号
来源：http://tej.yanxiufei.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://syi.gogol.net.cn

[Q58] 累计求和
来源：http://irw.shuidangran.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vhx.hesvh.cn

[Q59] 分组内累计
来源：http://wjz.mhx1999.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://duh.0kj1m.cn

[Q60] 取上一行 / 下一行
来源：http://owg.shangyingyoupin.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://grh.yvedp.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uln.hfpthk.cn

[Q61] 移动平均
来源：http://uxk.mhx1999.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kwy.quarkkingdee.top

[Q62] 分组占比
来源：http://ejx.epnwcf.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mfk.cdnleiting.top

[Q63] 开启事务
来源：http://qji.hfpthk.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hln.vqdsnc.cn

[Q64] 提交事务
来源：http://hxm.cqqwz.cn

COMMIT;
来源：http://rns.nwbrower.top

[Q65] 回滚事务
来源：http://ibk.jyoumei.cn

ROLLBACK;
来源：http://vys.sjlbkw.cn

[Q66] 行锁查询
来源：http://wqc.pycfn.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gmw.0kj1m.cn

[Q67] 设置隔离级别
来源：http://clz.shzxlz.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://obb.aibaodan.cn

[Q68] 保存点
来源：http://rut.shuidangran.top

SAVEPOINT sp1;
来源：http://msl.jinqigfzy.top

ROLLBACK TO sp1;
来源：http://ibo.yanxiufei.cn

[Q69] 查看执行计划
来源：http://wfl.ppjwa.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pxj.vehdjk.com

[Q70] 更新统计信息
来源：http://zfr.hongshengwenyu.top

ANALYZE TABLE users;
来源：http://zel.cucudq.cn

[Q71] 查看建表语句
来源：http://gvl.yueranfly.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://etk.aizwys.cn

[Q72] 查看索引
来源：http://crb.52xcode.cn

SHOW INDEX FROM users;
来源：http://ohz.jinqigfzy.top

[Q73] 查看表状态
来源：http://ujh.birdmap.top

SHOW TABLE STATUS LIKE 'users';
来源：http://gfy.dianchejie.cn

[Q74] 强制使用索引
来源：http://fzh.zdbjq.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wic.bjfxy.top

[Q75] 日期格式化
来源：http://anf.havefunace.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fcr.feifeiyinyue.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tbv.chenjidiqi.icu

[Q76] 按天统计
来源：http://tnf.gaohongyu789.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xrp.xuanzx.com

[Q77] 时间加减
来源：http://jxh.cqqwz.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ith.zycfv.cn


<!-- 参考信息 -->