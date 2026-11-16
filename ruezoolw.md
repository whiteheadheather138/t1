代发 wailian999

[O02] 使用线程池
来源：http://yac.zhaomingkeji.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qel.jqgufenzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gpu.fehbvm.com

JS:   // worker_threads 线程池
来源：http://frf.zhixingplan.top

TS:   // worker_threads 线程池
来源：http://rml.jinghuilouyu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://phx.gotoacloud.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zof.jqgufenzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bqy.gogol.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bio.redwolf501.top

[O03] 加锁保护共享数据
来源：http://dvy.yvedp.cn

Py:   with lock: shared += 1
来源：http://sqr.nwbrower.top

PHP:  // 用 flock() 做文件锁
来源：http://kgr.yanxiufei.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lan.bbcook.cn

TS:   // 同 JS
来源：http://mky.9152youxi.cn

Java: synchronized (this) { shared++; }
来源：http://tcj.hesvh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dvr.sweek.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://fxr.chenlongwang.top

C#:   lock (gate) { shared++; }
来源：http://rsd.chenjidiqi.icu

[O04] 定义异步函数并等待
来源：http://bym.yj202588.top

Py:   async def f():⏎    await g()
来源：http://aba.ybcxt.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ndr.fanxiaobao.xyz

JS:   async function f() { await g(); }
来源：http://fsb.snrcjt.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://cmf.cheryme.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jfo.zhiwuduotai.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xrd.uphjek.com

Ruby: # 用 Fiber 或 async gem
来源：http://rdc.nwbrower.top

C#:   async Task F() { await G(); }
来源：http://xlf.hysaishi.cn

[O05] 并发执行并等待全部完成
来源：http://gzy.c1oappe.top

Py:   asyncio.gather(*tasks)
来源：http://beg.tian-w.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uyc.yfazqb.com

JS:   await Promise.all(tasks)
来源：http://asv.chenlongwang.top

TS:   await Promise.all(tasks)
来源：http://ykp.quarkkingdee.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gcx.316326.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://klp.c1oappe.top

Ruby: threads.map(&:join)
来源：http://mng.kuanghao11.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bmz.hnqzz.top

[O06] 使用进程池
来源：http://auw.cucudq.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cpx.zdqjudy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://vjk.316326.xyz

JS:   // child_process / cluster 模块
来源：http://oli.gotoacloud.top

TS:   // child_process / cluster 模块
来源：http://rxy.316326.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pcl.jlsjyb.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gfh.daxiang520.top

Ruby: // fork 块
来源：http://jno.xuanzx.com

C#:   Parallel.For
来源：http://dbx.hongshengwenyu.top

================================================================================
来源：http://vjk.tian-w.cn

P. 常用工具函数
来源：http://veg.svipenyu.cn

================================================================================
来源：http://sos.gaohongyu789.top

[P01] 生成 UUID
来源：http://qoy.zhongyouzk.top

Py:   str(uuid.uuid4())
来源：http://nab.jlsjyb.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://aqy.xziqi.cn

JS:   crypto.randomUUID()
来源：http://ydq.nanxuanxn.top

TS:   crypto.randomUUID()
来源：http://apn.fanxiaobao.xyz

Java: UUID.randomUUID().toString()
来源：http://siw.yanxiufei.cn

Go:   // 用 github.com/google/uuid
来源：http://eyp.9152youxi.cn

Ruby: SecureRandom.uuid
来源：http://yfq.aizwys.cn

C#:   Guid.NewGuid().ToString()
来源：http://qyn.ydjk.org.cn

[P02] MD5 / SHA256 摘要
来源：http://dne.yuanzhike.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ngx.yongpay.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://sbo.316326.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dyf.wangdashe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dmy.gotoacloud.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pdr.ybcxt.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xpx.fzhhl.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://emd.zhoulong.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://upm.xziqi.cn

[P03] 生成短随机字符串
来源：http://tmf.tarul.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sed.aizwys.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://odt.chenlongwang.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bft.jqgufenzy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tfj.fengsongda.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://anp.ydjk.org.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wok.kuanghao11.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://dvk.chenjidiqi.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://aab.tian-w.cn

[P04] 求长度
来源：http://pst.nanxuanxn.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kfr.xuanzx.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dkx.xziqi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nsy.9152youxi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oea.fengsongda.top

Java: list.size();  map.size();  s.length()
来源：http://vsx.nwbrower.top

Go:   len(arr);  len(m)
来源：http://asu.sufxvd.cn

Ruby: x.length;  x.size
来源：http://enn.yongpay.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gnb.xuanzx.com

[P05] 判断两个对象内容是否相等
来源：http://hkh.iojbl.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://eqs.guannengcc.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lvj.iojbl.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rcc.gzhubu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vjx.yangfankeji.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uee.guowangkeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://bul.hongshengwenyu.top

Ruby: a == b
来源：http://tvk.tianlin.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tva.hammf.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qnu.zhijiandao.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bxn.pengpengdd.cyou

PHP:  if (empty($x)) {}
来源：http://rbd.yangfankeji.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qnt.fktsv.cn

TS:   if (x == null) {}
来源：http://mdu.hysaishi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mhh.snrcjt.cn

Go:   if x == nil {}
来源：http://jys.jqgfzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hae.meibo888.top

C#:   if (x is null) {}
来源：http://ehv.shanyushiyangkeji.top

[P07] 防抖与节流
来源：http://ajw.gzhubu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://faz.pycfn.com

PHP:  // 手写时间戳比较
来源：http://kuk.meibo888.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bws.chenlongwang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ruq.quarkkingdee.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dpy.shanyushiyangtech.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://omg.tarul.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wuk.jinyuanbaomall.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uhv.zhijiandao.cn

[P08] 处理浮点精度问题
来源：http://owv.cucudq.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nzk.sufxvd.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ufi.hywenlv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pkp.shangyingyoupin.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bcr.yueranfly.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ueq.yj20258.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qrd.gogol.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://evs.ehwqpu.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zkn.xinyue.icu

================================================================================
来源：http://cfb.meibo888.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bji.52xcode.cn

================================================================================
来源：http://dit.cheryme.top

[Q01] 创建表
来源：http://lzy.sweek.top

CREATE TABLE users (
来源：http://pxp.sjlbkw.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uuz.svipenyu.cn

name VARCHAR(50) NOT NULL,
来源：http://edt.andypj.xyz

email VARCHAR(100) UNIQUE,
来源：http://aow.smart0.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bbe.yj202588.top

);
来源：http://ooh.feifeiyinyue.top

[Q02] 创建带外键的表
来源：http://mmc.shuidangran.top

CREATE TABLE orders (
来源：http://aok.mhx1999.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ztr.zycfv.cn

user_id INT NOT NULL,
来源：http://myz.jinghuilouyu.cn

amount DECIMAL(10, 2),
来源：http://okh.cdnleiting.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qsf.zhengqikj.top

);
来源：http://pgr.pengpengdd.cyou

[Q03] 增加列
来源：http://dum.tian-w.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://riy.hongshengwenyu.top

[Q04] 修改列类型
来源：http://uow.ydjk.org.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tsy.jinyuanbaomall.cn

[Q05] 重命名列
来源：http://nvi.kuanghao11.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hvz.feifeiyinyue.top

[Q06] 删除列
来源：http://qsw.yfazqb.com

ALTER TABLE users DROP COLUMN age;
来源：http://whb.yueranfly.top

[Q07] 删除表
来源：http://wxz.jinyuanbaomall.cn

DROP TABLE IF EXISTS orders;
来源：http://urn.hammf.cn

[Q08] 创建普通索引
来源：http://hrl.cucudq.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hor.tian-w.cn

[Q09] 创建唯一索引
来源：http://xng.ppjwa.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zgn.hfpthk.cn

[Q10] 插入单行
来源：http://xsx.hesvh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yfi.nanxinkj.top

[Q11] 一次插入多行
来源：http://nwa.zdqjudy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ycp.hfpthk.cn

[Q12] 插入后取自增 ID
来源：http://duf.gaohongyu789.top

INSERT INTO users (name) VALUES ('C');
来源：http://vgs.andypj.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rtw.yueranfly.top

[Q13] 忽略重复插入
来源：http://liw.shuidangran.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gco.vqdsnc.cn

[Q14] 存在则更新（upsert）
来源：http://gxc.chenzaomai.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wjq.chenlongwang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bkf.c1oappe.top

[Q15] 查询全部
来源：http://pzv.jinghuilouyu.cn

SELECT * FROM users;
来源：http://eks.ydjk.org.cn

[Q16] 查询指定列
来源：http://oml.zhoulong.xyz

SELECT id, name FROM users;
来源：http://zex.yangfankeji.com

[Q17] 条件查询
来源：http://gnf.xylfe.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bci.zhixingplan.top

[Q18] 模糊匹配
来源：http://jjz.svipenyu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hgz.andypj.xyz

[Q19] 范围查询
来源：http://enq.daria6918.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://thr.yj202588.top

[Q20] IN 列表
来源：http://cpx.cashguo.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bmh.yueranfly.top

[Q21] 空值判断
来源：http://zov.dianchejie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vpw.quarkkingdee.top

[Q22] 排序
来源：http://owd.shanyushiyangtech.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bgx.sjlbkw.cn

[Q23] 分页
来源：http://bmy.xingfuxueyuan.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dzf.yuxming.cn

[Q24] 去重
来源：http://pfz.vqdsnc.cn

SELECT DISTINCT city FROM users;
来源：http://rxo.52xcode.cn

[Q25] 只取前 N 条
来源：http://vue.gotoacloud.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qgz.sweek.top

[Q26] 计数
来源：http://ysp.meibo888.top

SELECT COUNT(*) FROM users;
来源：http://llf.sufxvd.cn

[Q27] 条件计数
来源：http://pqp.c1oappe.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uvc.shanyushiyangkeji.top

[Q28] 求和与平均
来源：http://eao.sweek.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bmi.meibo888.top

[Q29] 最大最小值
来源：http://pel.yangfankeji.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://owr.bbcook.cn

[Q30] 分组统计
来源：http://elq.guowangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://acv.ywan-chungtsiang.top

[Q31] 分组后过滤
来源：http://rrg.jinqigfzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ouz.shanyushiyangkeji.top

[Q32] 分组拼接字符串
来源：http://hxj.ydzc1.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wkf.shanyushiyangtech.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://amb.dashuyun.cn

[Q33] 多列分组
来源：http://chg.52xcode.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ofn.birdmap.top

[Q34] 每组取第一条
来源：http://pyx.9152youxi.cn

SELECT * FROM (
来源：http://wrr.hammf.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jzb.yvedp.cn

) t WHERE rn = 1;
来源：http://epm.xziqi.cn

[Q35] 内连接
来源：http://kyc.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://weh.yj202588.top

[Q36] 左连接
来源：http://tdj.kuanghao11.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://szx.xylfe.cn

[Q37] 右连接
来源：http://pvj.jinqigfzy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nro.zycfv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lph.ybcxt.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yhz.yangfankeji.com

[Q39] 自连接（查上下级）
来源：http://avb.guowangkeji.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://goi.birdmap.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://waa.jiagoushi.top

[Q40] 交叉连接（笛卡尔积）
来源：http://tih.zhiwuduotai.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rpw.wangdashe.top

[Q41] 多表连接
来源：http://nlz.yj20258.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://sdt.ydzc1.top

JOIN users u ON u.id = o.user_id
来源：http://vlv.meibo888.top

JOIN products p ON p.id = o.product_id;
来源：http://blm.nanxinkj.top

[Q42] 连接条件附加过滤
来源：http://gqx.shangyingyoupin.top

SELECT u.name, o.amount FROM users u
来源：http://tmr.zycfv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://npl.daria6918.cn

[Q43] 标量子查询
来源：http://zxn.ppjwa.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oht.xylfe.cn

[Q44] IN 子查询
来源：http://ytk.tanke756.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lpo.hcnkem.com

[Q45] EXISTS 判断存在
来源：http://ogx.fzhhl.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sfj.yuxming.cn

[Q46] NOT EXISTS 判断不存在
来源：http://oxg.chenlongwang.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fws.ivvv.top

[Q47] 与平均值比较
来源：http://shn.zdqjudy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kva.bjfxy.top

[Q48] CTE 公用表表达式
来源：http://vgr.yvedp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ueh.cheryme.top

SELECT * FROM t WHERE c > 5;
来源：http://mov.hysaishi.cn

[Q49] 更新单行
来源：http://tmd.jinghuilouyu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tyv.zdbjq.cn

[Q50] 批量更新
来源：http://cdb.zhengqikj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xvw.zhongyouzk.top

[Q51] 用子查询更新
来源：http://tes.hesvh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://app.fzhhl.top

[Q52] 删除指定行
来源：http://cje.jlsjyb.cn

DELETE FROM users WHERE id = 10;
来源：http://ymu.yj202588.top

[Q53] 按条件删除
来源：http://sdg.mhx1999.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lax.hnxiangtu.top

[Q54] 清空表
来源：http://cnj.shuidangran.top

TRUNCATE TABLE logs;
来源：http://zwy.ppjwa.cn

[Q55] 排名（并列占位）
来源：http://ntt.316326.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://saz.sxryk.cn

[Q56] 密集排名（并列不占位）
来源：http://ssb.ydjk.org.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lhl.ehwqpu.com

[Q57] 行号
来源：http://ucw.cdnleiting.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fvb.hysaishi.cn

[Q58] 累计求和
来源：http://kaq.fanxiaobao.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kmw.smart0.xyz

[Q59] 分组内累计
来源：http://tft.jqgufenzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hyr.zhaomingkeji.xyz

[Q60] 取上一行 / 下一行
来源：http://zya.shuidangran.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sek.sysykeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://geg.xuetiantiany.cn

[Q61] 移动平均
来源：http://nsp.chenlongwang.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cex.yonumen.top

[Q62] 分组占比
来源：http://jmk.tarul.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ikj.zhaomingkeji.xyz

[Q63] 开启事务
来源：http://lps.bbcook.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tqt.sjlbkw.cn

[Q64] 提交事务
来源：http://nrz.pycfn.com

COMMIT;
来源：http://rha.guannengcc.top

[Q65] 回滚事务
来源：http://urw.0kj1m.cn

ROLLBACK;
来源：http://fje.feifeiyinyue.top

[Q66] 行锁查询
来源：http://enp.ywan-chungtsiang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ycn.ppjwa.cn

[Q67] 设置隔离级别
来源：http://cnf.9152youxi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vki.xuetiantiany.cn

[Q68] 保存点
来源：http://hfw.uphjek.com

SAVEPOINT sp1;
来源：http://qkf.hongshengwenyu.top

ROLLBACK TO sp1;
来源：http://acl.svipenyu.cn

[Q69] 查看执行计划
来源：http://mjh.meibo888.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://byj.cdnleiting.top

[Q70] 更新统计信息
来源：http://cot.zhengqikj.top

ANALYZE TABLE users;
来源：http://vjr.kuanghao11.cn

[Q71] 查看建表语句
来源：http://low.yueranfly.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cpr.haohaochexian.top

[Q72] 查看索引
来源：http://lop.fengsongda.top

SHOW INDEX FROM users;
来源：http://dol.shangyingyoupin.top

[Q73] 查看表状态
来源：http://udi.aibaodan.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xsm.jinqigufen.top

[Q74] 强制使用索引
来源：http://tkv.yonumen.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://iwn.bbcook.cn

[Q75] 日期格式化
来源：http://sth.yangfankeji.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://asz.kuanghao11.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zhy.hnxiangtu.top

[Q76] 按天统计
来源：http://ggj.epnwcf.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fyi.nanxuanxn.top

[Q77] 时间加减
来源：http://vkw.yfazqb.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bjg.andypj.xyz


<!-- 参考信息 -->