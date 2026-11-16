代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://xzi.52xcode.cn

Go:   go f()
来源：http://kcx.guowangkeji.top

Ruby: Thread.new { f }
来源：http://yge.haohaochexian.top

C#:   Task.Run(() => F());
来源：http://jal.yonumen.top

[O02] 使用线程池
来源：http://vcj.xinyue.icu

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eew.c1oappe.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dnj.ppjwa.cn

JS:   // worker_threads 线程池
来源：http://qsh.tarul.cn

TS:   // worker_threads 线程池
来源：http://eto.epnwcf.com

Java: Executors.newFixedThreadPool(4)
来源：http://bxw.zhengqikj.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lqs.jinqigfzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hyf.birdmap.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mam.yj20258.top

[O03] 加锁保护共享数据
来源：http://uno.shangyingyoupin.top

Py:   with lock: shared += 1
来源：http://qca.yonumen.top

PHP:  // 用 flock() 做文件锁
来源：http://ebe.zhoulong.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tqn.nanxinkj.top

TS:   // 同 JS
来源：http://lmq.andypj.xyz

Java: synchronized (this) { shared++; }
来源：http://xpx.shanyushiyangtech.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dxq.hywenlv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ykx.iojbl.cn

C#:   lock (gate) { shared++; }
来源：http://ekd.epnwcf.com

[O04] 定义异步函数并等待
来源：http://fqo.snrcjt.cn

Py:   async def f():⏎    await g()
来源：http://upn.gaohongyu789.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mzi.jyoumei.cn

JS:   async function f() { await g(); }
来源：http://oum.vehdjk.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://fhe.ehwqpu.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xtg.fzhhl.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://olt.xylfe.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xtz.hywenlv.cn

C#:   async Task F() { await G(); }
来源：http://fec.zdbjq.cn

[O05] 并发执行并等待全部完成
来源：http://fju.zhengqikj.top

Py:   asyncio.gather(*tasks)
来源：http://wps.jiagoushi.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bbt.snrcjt.cn

JS:   await Promise.all(tasks)
来源：http://pwi.guannengcc.top

TS:   await Promise.all(tasks)
来源：http://fmf.zhoulong.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pdm.shanyushiyangtech.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jjr.cashguo.top

Ruby: threads.map(&:join)
来源：http://rct.dashuyun.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cgt.ybcxt.top

[O06] 使用进程池
来源：http://icm.shanyushiyangtech.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xzu.jqgufenzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://mdp.nanxuanxn.top

JS:   // child_process / cluster 模块
来源：http://ant.yangfankeji.com

TS:   // child_process / cluster 模块
来源：http://eog.meibo888.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pem.sysykeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rch.vqdsnc.cn

Ruby: // fork 块
来源：http://afl.jiagoushi.top

C#:   Parallel.For
来源：http://dng.gogol.net.cn

================================================================================
来源：http://rmc.cashguo.top

P. 常用工具函数
来源：http://uyq.shanyushiyangtech.top

================================================================================
来源：http://opn.yanxiufei.cn

[P01] 生成 UUID
来源：http://pvi.gzhubu.top

Py:   str(uuid.uuid4())
来源：http://gzn.pycfn.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bbt.sysykeji.top

JS:   crypto.randomUUID()
来源：http://rlz.ydjk.org.cn

TS:   crypto.randomUUID()
来源：http://gkl.fzhhl.top

Java: UUID.randomUUID().toString()
来源：http://qfd.zhiwuduotai.top

Go:   // 用 github.com/google/uuid
来源：http://lsu.uphjek.com

Ruby: SecureRandom.uuid
来源：http://gmz.xziqi.cn

C#:   Guid.NewGuid().ToString()
来源：http://uhu.yvedp.cn

[P02] MD5 / SHA256 摘要
来源：http://ola.aibaodan.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bvv.hnqzz.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ebn.zhengqikj.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sut.dianchejie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cdr.jlsjyb.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://igd.chenjidiqi.icu

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nxd.quarkkingdee.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://twp.mhx1999.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hgd.bjfxy.top

[P03] 生成短随机字符串
来源：http://prv.gotoacloud.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nis.yfazqb.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uog.vqdsnc.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bhe.chenzaomai.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://coh.yuxming.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yoq.pengpengdd.cyou

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jmv.tianlin.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://jio.shuidangran.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rka.sxryk.cn

[P04] 求长度
来源：http://bog.hammf.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jkp.vehdjk.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vzh.jianghu66.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ird.gzhubu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mzv.snrcjt.cn

Java: list.size();  map.size();  s.length()
来源：http://tah.ctjpmb.com

Go:   len(arr);  len(m)
来源：http://jdv.tarul.cn

Ruby: x.length;  x.size
来源：http://gaj.fzhhl.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://brq.yj202588.top

[P05] 判断两个对象内容是否相等
来源：http://akk.9152youxi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dhp.zhiwuduotai.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yuc.yonumen.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xlo.zhiwuduotai.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wsn.cashguo.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qtq.jianghu66.top

Go:   reflect.DeepEqual(a, b)
来源：http://uir.epnwcf.com

Ruby: a == b
来源：http://ggf.tarul.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hmf.xuetiantiany.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ryz.nanxinkj.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dug.zhijiandao.cn

PHP:  if (empty($x)) {}
来源：http://cwm.vehdjk.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cpr.ywan-chungtsiang.top

TS:   if (x == null) {}
来源：http://lmj.yonumen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://tut.yongpay.top

Go:   if x == nil {}
来源：http://anz.gaohongyu789.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qrt.gaohongyu789.top

C#:   if (x is null) {}
来源：http://bke.chenzaomai.com

[P07] 防抖与节流
来源：http://unc.vqdsnc.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://skh.tianlin.xyz

PHP:  // 手写时间戳比较
来源：http://xjq.gotoacloud.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://axq.epnwcf.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uuf.hnqzz.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nvf.snrcjt.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qpi.fzhhl.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://jfi.zycfv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://esx.ybcxt.top

[P08] 处理浮点精度问题
来源：http://rkd.zhiwuduotai.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yxa.zhengqikj.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dnx.chenjidiqi.icu

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cdc.meibo888.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hhq.gaohongyu789.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dfb.yuxming.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yqr.shanyushiyangkeji.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hql.sweek.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hpm.ivvv.top

================================================================================
来源：http://usa.ybcxt.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://psr.andypj.xyz

================================================================================
来源：http://kka.cqqwz.cn

[Q01] 创建表
来源：http://ivv.yuxming.cn

CREATE TABLE users (
来源：http://gis.cashguo.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ocf.iojbl.cn

name VARCHAR(50) NOT NULL,
来源：http://wkn.0kj1m.cn

email VARCHAR(100) UNIQUE,
来源：http://ole.ppjwa.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lxz.tanke756.top

);
来源：http://tfg.zhijiandao.cn

[Q02] 创建带外键的表
来源：http://ovn.cheryme.top

CREATE TABLE orders (
来源：http://rns.hnqzz.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mrr.jianghu66.top

user_id INT NOT NULL,
来源：http://ieg.ywan-chungtsiang.top

amount DECIMAL(10, 2),
来源：http://sql.jinqigfzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dki.yanxiufei.cn

);
来源：http://cul.zhoulong.xyz

[Q03] 增加列
来源：http://ojh.jyoumei.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ekw.cdnleiting.top

[Q04] 修改列类型
来源：http://nqg.xinyue.icu

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://phz.feifeiyinyue.top

[Q05] 重命名列
来源：http://xok.cucudq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nla.52xcode.cn

[Q06] 删除列
来源：http://pzt.hammf.cn

ALTER TABLE users DROP COLUMN age;
来源：http://urm.cqqwz.cn

[Q07] 删除表
来源：http://qia.haohaochexian.top

DROP TABLE IF EXISTS orders;
来源：http://pge.shanyushiyangkeji.top

[Q08] 创建普通索引
来源：http://uqk.zdbjq.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nye.gaohongyu789.top

[Q09] 创建唯一索引
来源：http://slk.tanke756.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xzh.52xcode.cn

[Q10] 插入单行
来源：http://mrj.yfazqb.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rmj.zdqjudy.top

[Q11] 一次插入多行
来源：http://dgo.kuanghao11.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sfh.havefunace.top

[Q12] 插入后取自增 ID
来源：http://jri.guannengcc.top

INSERT INTO users (name) VALUES ('C');
来源：http://vth.hcnkem.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hrm.shangyingyoupin.top

[Q13] 忽略重复插入
来源：http://vjg.gzhubu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wwr.smart0.xyz

[Q14] 存在则更新（upsert）
来源：http://blp.shanyushiyangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zlt.dianchejie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nyg.fehbvm.com

[Q15] 查询全部
来源：http://ybh.guannengcc.top

SELECT * FROM users;
来源：http://qzy.yanxiufei.cn

[Q16] 查询指定列
来源：http://ygc.cucudq.cn

SELECT id, name FROM users;
来源：http://inv.yongpay.top

[Q17] 条件查询
来源：http://eti.xuanzx.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xhi.uphjek.com

[Q18] 模糊匹配
来源：http://usa.shzxlz.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ven.nanxinkj.top

[Q19] 范围查询
来源：http://zes.xylfe.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bso.xuetiantiany.cn

[Q20] IN 列表
来源：http://lly.yj20258.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vkf.gogol.net.cn

[Q21] 空值判断
来源：http://dua.zhengqikj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://tcp.jinyuanbaomall.cn

[Q22] 排序
来源：http://blc.xylfe.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qpm.nwbrower.top

[Q23] 分页
来源：http://vei.zhixingplan.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hmz.shanyushiyangtech.top

[Q24] 去重
来源：http://vfe.ydjk.org.cn

SELECT DISTINCT city FROM users;
来源：http://ytq.sjlbkw.cn

[Q25] 只取前 N 条
来源：http://pib.zycfv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://czh.tian-w.cn

[Q26] 计数
来源：http://jbe.guannengcc.top

SELECT COUNT(*) FROM users;
来源：http://ujb.svipenyu.cn

[Q27] 条件计数
来源：http://imk.ppjwa.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nep.yonumen.top

[Q28] 求和与平均
来源：http://tam.nwbrower.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wtg.ppjwa.cn

[Q29] 最大最小值
来源：http://svd.wangdashe.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://iqh.ppjwa.cn

[Q30] 分组统计
来源：http://elh.fanxiaobao.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://djk.hnqzz.top

[Q31] 分组后过滤
来源：http://yjr.mhx1999.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yzz.sysykeji.top

[Q32] 分组拼接字符串
来源：http://twl.ydjk.org.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ldy.havefunace.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fxg.fanxiaobao.xyz

[Q33] 多列分组
来源：http://rnp.xinyue.icu

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vhw.316326.xyz

[Q34] 每组取第一条
来源：http://hxz.hongshengwenyu.top

SELECT * FROM (
来源：http://zbi.ydzc1.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gpn.zhaomingkeji.xyz

) t WHERE rn = 1;
来源：http://ein.jianghu66.top

[Q35] 内连接
来源：http://abw.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hor.chenlongwang.top

[Q36] 左连接
来源：http://unl.nanxinkj.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zvg.tanke756.top

[Q37] 右连接
来源：http://iyz.hcnkem.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dex.chenlongwang.top

[Q38] 全外连接（PostgreSQL）
来源：http://esi.birdmap.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dez.chenlongwang.top

[Q39] 自连接（查上下级）
来源：http://erh.hfpthk.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yrv.tarul.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vhv.sjlbkw.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fpl.fzhhl.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pab.haohaochexian.top

[Q41] 多表连接
来源：http://owm.zdqjudy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://rsy.ctjpmb.com

JOIN users u ON u.id = o.user_id
来源：http://lrp.fengsongda.top

JOIN products p ON p.id = o.product_id;
来源：http://xob.snrcjt.cn

[Q42] 连接条件附加过滤
来源：http://whv.smart0.xyz

SELECT u.name, o.amount FROM users u
来源：http://ktj.sweek.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bha.ehwqpu.com

[Q43] 标量子查询
来源：http://jmy.vehdjk.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cjw.yangfankeji.com

[Q44] IN 子查询
来源：http://eaa.pengpengdd.cyou

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nlj.zhengqikj.top

[Q45] EXISTS 判断存在
来源：http://zgg.ctjpmb.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vxe.yongpay.top

[Q46] NOT EXISTS 判断不存在
来源：http://esb.316326.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wej.ybcxt.top

[Q47] 与平均值比较
来源：http://xzx.hysaishi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://shw.fktsv.cn

[Q48] CTE 公用表表达式
来源：http://fau.meibo888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mge.jqgufenzy.top

SELECT * FROM t WHERE c > 5;
来源：http://qxo.yvedp.cn

[Q49] 更新单行
来源：http://zrj.hnqzz.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ugl.jinyuanbaomall.cn

[Q50] 批量更新
来源：http://omm.hysaishi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fnr.epnwcf.com

[Q51] 用子查询更新
来源：http://dow.nwbrower.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xym.ehwqpu.com

[Q52] 删除指定行
来源：http://yvz.jinghuilouyu.cn

DELETE FROM users WHERE id = 10;
来源：http://dsn.nwbrower.top

[Q53] 按条件删除
来源：http://vpl.fengsongda.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://haw.9152youxi.cn

[Q54] 清空表
来源：http://osj.xuetiantiany.cn

TRUNCATE TABLE logs;
来源：http://irs.jiagoushi.top

[Q55] 排名（并列占位）
来源：http://fnl.tanke756.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pax.fanxiaobao.xyz

[Q56] 密集排名（并列不占位）
来源：http://wld.ydjk.org.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lbk.yfazqb.com

[Q57] 行号
来源：http://rfj.ybcxt.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vuo.jinghuilouyu.cn

[Q58] 累计求和
来源：http://yka.yfazqb.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mde.hysaishi.cn

[Q59] 分组内累计
来源：http://lev.fanxiaobao.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rzz.jqgfzy.top

[Q60] 取上一行 / 下一行
来源：http://epx.tian-w.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ikf.ctjpmb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fdc.fanxiaobao.xyz

[Q61] 移动平均
来源：http://jek.hnxiangtu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://syz.jqgfzy.top

[Q62] 分组占比
来源：http://zii.shanyushiyangkeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ypt.zhiwuduotai.top

[Q63] 开启事务
来源：http://jzk.ivvv.top

START TRANSACTION;                -- 或 BEGIN
来源：http://etm.zdqjudy.top

[Q64] 提交事务
来源：http://gzg.ydjk.org.cn

COMMIT;
来源：http://crm.uphjek.com

[Q65] 回滚事务
来源：http://trk.xuanzx.com

ROLLBACK;
来源：http://smy.yanxiufei.cn

[Q66] 行锁查询
来源：http://cmy.ehwqpu.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rir.dianchejie.cn

[Q67] 设置隔离级别
来源：http://arr.nanxinkj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gax.dashuyun.cn

[Q68] 保存点
来源：http://kba.nwbrower.top

SAVEPOINT sp1;
来源：http://jxk.vehdjk.com

ROLLBACK TO sp1;
来源：http://rgf.zhixingplan.top

[Q69] 查看执行计划
来源：http://jpt.gogol.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wgo.birdmap.top

[Q70] 更新统计信息
来源：http://yjq.tarul.cn

ANALYZE TABLE users;
来源：http://gmk.hcnkem.com

[Q71] 查看建表语句
来源：http://cjz.feifeiyinyue.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zra.yongpay.top

[Q72] 查看索引
来源：http://tyw.havefunace.top

SHOW INDEX FROM users;
来源：http://qkw.jinyuanbaomall.cn

[Q73] 查看表状态
来源：http://gyq.fengsongda.top

SHOW TABLE STATUS LIKE 'users';
来源：http://wpq.yongpay.top

[Q74] 强制使用索引
来源：http://iss.pengpengdd.cyou

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://thm.ivvv.top

[Q75] 日期格式化
来源：http://oje.hcnkem.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vgh.fzhhl.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rxi.havefunace.top


<!-- 参考信息 -->