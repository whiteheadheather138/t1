代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://fgl.hnxiangtu.top

Go:   go f()
来源：http://zno.shangyingyoupin.top

Ruby: Thread.new { f }
来源：http://ugp.bbcook.cn

C#:   Task.Run(() => F());
来源：http://xfj.hysaishi.cn

[O02] 使用线程池
来源：http://pyb.shangyingyoupin.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ait.0kj1m.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wat.chenzaomai.com

JS:   // worker_threads 线程池
来源：http://lxj.smart0.xyz

TS:   // worker_threads 线程池
来源：http://pkx.fengsongda.top

Java: Executors.newFixedThreadPool(4)
来源：http://yzo.chenlongwang.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://aed.ydzc1.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fcn.iojbl.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://eet.sweek.top

[O03] 加锁保护共享数据
来源：http://nnd.yj202588.top

Py:   with lock: shared += 1
来源：http://xzc.birdmap.top

PHP:  // 用 flock() 做文件锁
来源：http://xgp.gogol.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://put.yfazqb.com

TS:   // 同 JS
来源：http://lpx.fanxiaobao.xyz

Java: synchronized (this) { shared++; }
来源：http://eyf.wangdashe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ikm.yangfankeji.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://gsg.wangshuangyany.cn

C#:   lock (gate) { shared++; }
来源：http://yoc.fehbvm.com

[O04] 定义异步函数并等待
来源：http://dww.uphjek.com

Py:   async def f():⏎    await g()
来源：http://oqj.jyoumei.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lpe.yanxiufei.cn

JS:   async function f() { await g(); }
来源：http://jbm.pycfn.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://hby.uphjek.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nla.aibaodan.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dso.zhixingplan.top

Ruby: # 用 Fiber 或 async gem
来源：http://yzl.chenzaomai.com

C#:   async Task F() { await G(); }
来源：http://zgr.sjlbkw.cn

[O05] 并发执行并等待全部完成
来源：http://mor.yj20258888.top

Py:   asyncio.gather(*tasks)
来源：http://euv.nwbrower.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://eeq.hesvh.cn

JS:   await Promise.all(tasks)
来源：http://xjz.yueranfly.top

TS:   await Promise.all(tasks)
来源：http://cpe.yj20258888.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rkv.ctjpmb.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wdi.hnxiangtu.top

Ruby: threads.map(&:join)
来源：http://zcl.ydzc1.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mxe.yonumen.top

[O06] 使用进程池
来源：http://ohy.redwolf501.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ovq.yfazqb.com

PHP:  // pcntl_fork 或多进程队列
来源：http://dgj.xuanzx.com

JS:   // child_process / cluster 模块
来源：http://txr.zdqjudy.top

TS:   // child_process / cluster 模块
来源：http://wbs.hesvh.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vgj.tarul.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lfh.zhixingplan.top

Ruby: // fork 块
来源：http://dup.zhengqikj.top

C#:   Parallel.For
来源：http://iyh.fengsongda.top

================================================================================
来源：http://cam.zhijiandao.cn

P. 常用工具函数
来源：http://hnu.fengsongda.top

================================================================================
来源：http://mak.zdbjq.cn

[P01] 生成 UUID
来源：http://dfn.hysaishi.cn

Py:   str(uuid.uuid4())
来源：http://pev.shangyingyoupin.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zjl.yj20258888.top

JS:   crypto.randomUUID()
来源：http://jos.yuxming.cn

TS:   crypto.randomUUID()
来源：http://zmn.wangshuangyany.cn

Java: UUID.randomUUID().toString()
来源：http://byw.chenjidiqi.icu

Go:   // 用 github.com/google/uuid
来源：http://gbw.nanxinkj.top

Ruby: SecureRandom.uuid
来源：http://smu.jianghu66.top

C#:   Guid.NewGuid().ToString()
来源：http://vxl.zhaomingkeji.xyz

[P02] MD5 / SHA256 摘要
来源：http://igx.ppjwa.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gcr.uphjek.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://mlv.shuidangran.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://eks.tian-w.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wvj.snrcjt.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zfi.hongshengwenyu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kab.shanyushiyangtech.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://itg.chenjidiqi.icu

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://twe.sufxvd.cn

[P03] 生成短随机字符串
来源：http://maf.hnqzz.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ofm.wangshuangyany.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://msa.hysaishi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://axh.vehdjk.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qxs.dashuyun.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qkz.vehdjk.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://txj.316326.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://mej.gogol.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jjp.yvedp.cn

[P04] 求长度
来源：http://ttd.dashuyun.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bsy.chenjidiqi.icu

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://svg.hysaishi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iyq.nanxuanxn.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wzw.yvedp.cn

Java: list.size();  map.size();  s.length()
来源：http://lbh.aizwys.cn

Go:   len(arr);  len(m)
来源：http://zym.jinghuilouyu.cn

Ruby: x.length;  x.size
来源：http://zim.svipenyu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ewm.sweek.top

[P05] 判断两个对象内容是否相等
来源：http://kxy.pengpengdd.cyou

Py:   a == b              # 列表与字典递归比较内容
来源：http://lyp.yueranfly.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://flh.yfazqb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zyh.hfpthk.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rvg.hnqzz.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sau.ivvv.top

Go:   reflect.DeepEqual(a, b)
来源：http://kdq.316326.xyz

Ruby: a == b
来源：http://apb.zhijiandao.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ttf.zhengqikj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dwk.zdqjudy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cvc.tian-w.cn

PHP:  if (empty($x)) {}
来源：http://wry.ybcxt.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rcj.shangyingyoupin.top

TS:   if (x == null) {}
来源：http://tuk.fzhhl.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wsl.hammf.cn

Go:   if x == nil {}
来源：http://uhb.jinqigufen.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xqe.yj20258.top

C#:   if (x is null) {}
来源：http://pgq.yj20258.top

[P07] 防抖与节流
来源：http://diq.ydzc1.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oiw.ehwqpu.com

PHP:  // 手写时间戳比较
来源：http://zhi.dianchejie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qln.hfpthk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zcm.zdbjq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fwp.jinyuanbaomall.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gya.jqgufenzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://hom.cqqwz.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sru.tian-w.cn

[P08] 处理浮点精度问题
来源：http://ujh.nanxinkj.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dhw.jianghu66.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pyi.jinghuilouyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kih.mhx1999.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://peu.yj20258.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xre.bjfxy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yjr.xinyue.icu

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uig.ywan-chungtsiang.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lkh.ehwqpu.com

================================================================================
来源：http://axc.zhoulong.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rea.xuetiantiany.cn

================================================================================
来源：http://qdd.chenlongwang.top

[Q01] 创建表
来源：http://hyp.zhijiandao.cn

CREATE TABLE users (
来源：http://mun.tarul.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nah.c1oappe.top

name VARCHAR(50) NOT NULL,
来源：http://zgb.sjlbkw.cn

email VARCHAR(100) UNIQUE,
来源：http://aap.tian-w.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bzi.hammf.cn

);
来源：http://iwx.jinghuilouyu.cn

[Q02] 创建带外键的表
来源：http://sxx.fengsongda.top

CREATE TABLE orders (
来源：http://vpt.hnqzz.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ehx.cdnleiting.top

user_id INT NOT NULL,
来源：http://koa.shuidangran.top

amount DECIMAL(10, 2),
来源：http://cmz.dianchejie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jow.sysykeji.top

);
来源：http://pmp.zdqjudy.top

[Q03] 增加列
来源：http://xsz.birdmap.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zll.52xcode.cn

[Q04] 修改列类型
来源：http://exj.nanxuanxn.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://spj.wangdashe.top

[Q05] 重命名列
来源：http://ixl.wangshuangyany.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zib.uphjek.com

[Q06] 删除列
来源：http://lga.epnwcf.com

ALTER TABLE users DROP COLUMN age;
来源：http://owz.yonumen.top

[Q07] 删除表
来源：http://jew.hnxiangtu.top

DROP TABLE IF EXISTS orders;
来源：http://qdc.fanxiaobao.xyz

[Q08] 创建普通索引
来源：http://aav.hysaishi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://clo.hongshengwenyu.top

[Q09] 创建唯一索引
来源：http://hfy.jlsjyb.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ail.yuanzhike.top

[Q10] 插入单行
来源：http://mne.dashuyun.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wow.vqdsnc.cn

[Q11] 一次插入多行
来源：http://cxa.ehwqpu.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mra.ydzc1.top

[Q12] 插入后取自增 ID
来源：http://sxz.dianchejie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ojk.hnqzz.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fvi.havefunace.top

[Q13] 忽略重复插入
来源：http://whi.yuanzhike.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://abs.ppjwa.cn

[Q14] 存在则更新（upsert）
来源：http://mzm.hnqzz.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bzi.yanxiufei.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wzs.xingfuxueyuan.xyz

[Q15] 查询全部
来源：http://hdx.hnxiangtu.top

SELECT * FROM users;
来源：http://dgp.smart0.xyz

[Q16] 查询指定列
来源：http://clb.yj20258888.top

SELECT id, name FROM users;
来源：http://vfv.hammf.cn

[Q17] 条件查询
来源：http://nti.fehbvm.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ruw.zhixingplan.top

[Q18] 模糊匹配
来源：http://pvn.yangfankeji.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yjq.daria6918.cn

[Q19] 范围查询
来源：http://aax.fanxiaobao.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xec.tanke756.top

[Q20] IN 列表
来源：http://pza.gotoacloud.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qzs.shanyushiyangtech.top

[Q21] 空值判断
来源：http://jsd.ctjpmb.com

SELECT * FROM users WHERE email IS NULL;
来源：http://zur.jinqigfzy.top

[Q22] 排序
来源：http://qbp.svipenyu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sls.cqqwz.cn

[Q23] 分页
来源：http://cbw.ydjk.org.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vgh.zhaomingkeji.xyz

[Q24] 去重
来源：http://fzn.cqqwz.cn

SELECT DISTINCT city FROM users;
来源：http://vgp.gotoacloud.top

[Q25] 只取前 N 条
来源：http://qhb.jlsjyb.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://thf.zhoulong.xyz

[Q26] 计数
来源：http://kyh.feifeiyinyue.top

SELECT COUNT(*) FROM users;
来源：http://dhi.sxryk.cn

[Q27] 条件计数
来源：http://ymi.daria6918.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zxd.kuanghao11.cn

[Q28] 求和与平均
来源：http://ovh.yueranfly.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://eek.zdbjq.cn

[Q29] 最大最小值
来源：http://aos.yonumen.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://dcd.hcnkem.com

[Q30] 分组统计
来源：http://yso.yj20258.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rry.birdmap.top

[Q31] 分组后过滤
来源：http://lnu.jiagoushi.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gkh.pengpengdd.cyou

[Q32] 分组拼接字符串
来源：http://mlw.wangshuangyany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://etj.cucudq.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fcz.yj20258888.top

[Q33] 多列分组
来源：http://ozm.svipenyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wjy.sufxvd.cn

[Q34] 每组取第一条
来源：http://ccu.xingfuxueyuan.xyz

SELECT * FROM (
来源：http://kux.snrcjt.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vev.zdqjudy.top

) t WHERE rn = 1;
来源：http://daj.yj20258.top

[Q35] 内连接
来源：http://vdb.chenzaomai.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://irl.nwbrower.top

[Q36] 左连接
来源：http://bjd.cdnleiting.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lir.chenlongwang.top

[Q37] 右连接
来源：http://qlg.svipenyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gzs.ywan-chungtsiang.top

[Q38] 全外连接（PostgreSQL）
来源：http://tht.jinqigufen.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bfn.zhiwuduotai.top

[Q39] 自连接（查上下级）
来源：http://faa.zhongyouzk.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ixm.birdmap.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nsa.cheryme.top

[Q40] 交叉连接（笛卡尔积）
来源：http://try.zhoulong.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ibo.dianchejie.cn

[Q41] 多表连接
来源：http://lav.shzxlz.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uls.aibaodan.cn

JOIN users u ON u.id = o.user_id
来源：http://naq.sjlbkw.cn

JOIN products p ON p.id = o.product_id;
来源：http://ozw.yonumen.top

[Q42] 连接条件附加过滤
来源：http://ihi.yonumen.top

SELECT u.name, o.amount FROM users u
来源：http://lxw.mhx1999.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jsr.vqdsnc.cn

[Q43] 标量子查询
来源：http://kff.quarkkingdee.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://reu.svipenyu.cn

[Q44] IN 子查询
来源：http://iep.yj20258.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://syj.smart0.xyz

[Q45] EXISTS 判断存在
来源：http://vxm.epnwcf.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qie.zhijiandao.cn

[Q46] NOT EXISTS 判断不存在
来源：http://utm.tianlin.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://neh.jinqigfzy.top

[Q47] 与平均值比较
来源：http://pot.nanxuanxn.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ivr.daria6918.cn

[Q48] CTE 公用表表达式
来源：http://jwq.ctjpmb.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mho.zhengqikj.top

SELECT * FROM t WHERE c > 5;
来源：http://oxh.shanyushiyangkeji.top

[Q49] 更新单行
来源：http://geh.hnqzz.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fhw.hnqzz.top

[Q50] 批量更新
来源：http://suf.cashguo.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vqg.tian-w.cn

[Q51] 用子查询更新
来源：http://plv.hysaishi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yjg.meibo888.top

[Q52] 删除指定行
来源：http://xyu.vqdsnc.cn

DELETE FROM users WHERE id = 10;
来源：http://kqp.bjfxy.top

[Q53] 按条件删除
来源：http://ihj.cdnleiting.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mkz.316326.xyz

[Q54] 清空表
来源：http://zak.ctjpmb.com

TRUNCATE TABLE logs;
来源：http://pza.smart0.xyz

[Q55] 排名（并列占位）
来源：http://mxv.fzhhl.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yyb.gaohongyu789.top

[Q56] 密集排名（并列不占位）
来源：http://rev.pycfn.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fsl.sufxvd.cn

[Q57] 行号
来源：http://vpo.svipenyu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cdz.zhengqikj.top

[Q58] 累计求和
来源：http://hor.52xcode.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xee.yonumen.top

[Q59] 分组内累计
来源：http://sfj.shanyushiyangkeji.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rln.xylfe.cn

[Q60] 取上一行 / 下一行
来源：http://zvz.fehbvm.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zry.xuetiantiany.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://egu.zhijiandao.cn

[Q61] 移动平均
来源：http://mvv.jlsjyb.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zdi.jinyuanbaomall.cn

[Q62] 分组占比
来源：http://mqx.meibo888.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://oib.hesvh.cn

[Q63] 开启事务
来源：http://cuy.yonumen.top

START TRANSACTION;                -- 或 BEGIN
来源：http://qho.fengsongda.top

[Q64] 提交事务
来源：http://ire.svipenyu.cn

COMMIT;
来源：http://elt.smart0.xyz

[Q65] 回滚事务
来源：http://jiw.svipenyu.cn

ROLLBACK;
来源：http://mlm.mhx1999.top

[Q66] 行锁查询
来源：http://zyg.hesvh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rle.vqdsnc.cn

[Q67] 设置隔离级别
来源：http://yla.cheryme.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lhe.fehbvm.com

[Q68] 保存点
来源：http://ogv.haohaochexian.top

SAVEPOINT sp1;
来源：http://mot.sjlbkw.cn

ROLLBACK TO sp1;
来源：http://oue.shuidangran.top

[Q69] 查看执行计划
来源：http://hht.andypj.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gni.shanyushiyangkeji.top

[Q70] 更新统计信息
来源：http://ygp.hfpthk.cn

ANALYZE TABLE users;
来源：http://lry.ppjwa.cn

[Q71] 查看建表语句
来源：http://cbd.ybcxt.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yyc.epnwcf.com

[Q72] 查看索引
来源：http://ngi.cheryme.top

SHOW INDEX FROM users;
来源：http://fqd.chenzaomai.com

[Q73] 查看表状态
来源：http://tzd.sjlbkw.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tcg.fanxiaobao.xyz

[Q74] 强制使用索引
来源：http://awh.nanxinkj.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://emx.aibaodan.cn

[Q75] 日期格式化
来源：http://gpo.guowangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lpr.zycfv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zuj.jinghuilouyu.cn


<!-- 参考信息 -->