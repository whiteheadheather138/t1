代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kmp.jyoumei.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fxw.redwolf501.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pfq.yvedp.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gww.fengsongda.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://spu.shuidangran.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://egm.c1oappe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://crb.cashguo.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ebb.shanyushiyangtech.top

================================================================================
来源：http://dfp.ybcxt.top

O. 并发与异步
来源：http://vtz.zhiwuduotai.top

================================================================================
来源：http://duh.hfpthk.cn

[O01] 启动一个线程
来源：http://ctf.hnqzz.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xrz.pycfn.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dpk.sxryk.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zlg.gogol.net.cn

TS:   // 同 JS
来源：http://nmb.hysaishi.cn

Java: new Thread(() -> f()).start()
来源：http://eei.nanxinkj.top

Go:   go f()
来源：http://mig.tanke756.top

Ruby: Thread.new { f }
来源：http://hvj.zdbjq.cn

C#:   Task.Run(() => F());
来源：http://hul.jyoumei.cn

[O02] 使用线程池
来源：http://wgj.yuanzhike.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tis.pengpengdd.cyou

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dgh.cucudq.cn

JS:   // worker_threads 线程池
来源：http://yka.ctjpmb.com

TS:   // worker_threads 线程池
来源：http://ecj.chenzaomai.com

Java: Executors.newFixedThreadPool(4)
来源：http://cvf.cheryme.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://uun.cucudq.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://eig.hywenlv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mim.shangyingyoupin.top

[O03] 加锁保护共享数据
来源：http://evp.xylfe.cn

Py:   with lock: shared += 1
来源：http://qvy.ppjwa.cn

PHP:  // 用 flock() 做文件锁
来源：http://lud.haohaochexian.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://are.shzxlz.cn

TS:   // 同 JS
来源：http://avh.xziqi.cn

Java: synchronized (this) { shared++; }
来源：http://shm.xylfe.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kfs.cqqwz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://doi.bjfxy.top

C#:   lock (gate) { shared++; }
来源：http://zpb.zhixingplan.top

[O04] 定义异步函数并等待
来源：http://lfz.52xcode.cn

Py:   async def f():⏎    await g()
来源：http://llm.andypj.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rir.ybcxt.top

JS:   async function f() { await g(); }
来源：http://ilp.xuetiantiany.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://glm.aibaodan.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pfy.daria6918.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://stu.gotoacloud.top

Ruby: # 用 Fiber 或 async gem
来源：http://eji.shuidangran.top

C#:   async Task F() { await G(); }
来源：http://btx.xinyue.icu

[O05] 并发执行并等待全部完成
来源：http://zlz.daxiang520.top

Py:   asyncio.gather(*tasks)
来源：http://iio.zdbjq.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zmi.yj20258.top

JS:   await Promise.all(tasks)
来源：http://bmu.birdmap.top

TS:   await Promise.all(tasks)
来源：http://qbi.shzxlz.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cwr.yj202588.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uxl.xingfuxueyuan.xyz

Ruby: threads.map(&:join)
来源：http://odu.jinqigufen.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ltc.haohaochexian.top

[O06] 使用进程池
来源：http://vlk.yueranfly.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qva.fehbvm.com

PHP:  // pcntl_fork 或多进程队列
来源：http://zry.hnxiangtu.top

JS:   // child_process / cluster 模块
来源：http://yss.zdqjudy.top

TS:   // child_process / cluster 模块
来源：http://yzj.guowangkeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mki.guowangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://iun.hesvh.cn

Ruby: // fork 块
来源：http://suz.svipenyu.cn

C#:   Parallel.For
来源：http://sne.yongpay.top

================================================================================
来源：http://uqx.ivvv.top

P. 常用工具函数
来源：http://crz.fktsv.cn

================================================================================
来源：http://bjk.meibo888.top

[P01] 生成 UUID
来源：http://dpt.nanxinkj.top

Py:   str(uuid.uuid4())
来源：http://ldb.zhongyouzk.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rxz.shuidangran.top

JS:   crypto.randomUUID()
来源：http://sjf.tanke756.top

TS:   crypto.randomUUID()
来源：http://mth.chenjidiqi.icu

Java: UUID.randomUUID().toString()
来源：http://vjs.vqdsnc.cn

Go:   // 用 github.com/google/uuid
来源：http://lsd.bjfxy.top

Ruby: SecureRandom.uuid
来源：http://vjt.jqgufenzy.top

C#:   Guid.NewGuid().ToString()
来源：http://rci.epnwcf.com

[P02] MD5 / SHA256 摘要
来源：http://ank.sweek.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vsw.hysaishi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gix.dianchejie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jax.shanyushiyangtech.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zis.vqdsnc.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rte.yj202588.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://agl.daxiang520.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ruv.mhx1999.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dit.hesvh.cn

[P03] 生成短随机字符串
来源：http://ykk.52xcode.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dab.yuanzhike.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jbc.jinghuilouyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qyu.xuetiantiany.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ypg.zhongyouzk.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ghz.tianlin.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xed.shzxlz.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://tnl.chenzaomai.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cmq.yj20258.top

[P04] 求长度
来源：http://gvg.nanxinkj.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fyh.dashuyun.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rua.sysykeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iwv.hammf.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fai.jianghu66.top

Java: list.size();  map.size();  s.length()
来源：http://zug.fanxiaobao.xyz

Go:   len(arr);  len(m)
来源：http://yrz.shuidangran.top

Ruby: x.length;  x.size
来源：http://qye.shangyingyoupin.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://agf.yongpay.top

[P05] 判断两个对象内容是否相等
来源：http://boi.jlsjyb.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ndw.ppjwa.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sky.gaohongyu789.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ggr.zhaomingkeji.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://oxd.bbcook.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ptg.zhijiandao.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qji.zhongyouzk.top

Ruby: a == b
来源：http://iox.wangdashe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mpt.cucudq.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gxy.xuetiantiany.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://duj.smart0.xyz

PHP:  if (empty($x)) {}
来源：http://wcs.yuanzhike.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uky.xinyue.icu

TS:   if (x == null) {}
来源：http://qpo.yuanzhike.top

Java: if (x == null || x.isEmpty()) {}
来源：http://fcu.smart0.xyz

Go:   if x == nil {}
来源：http://hui.dianchejie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mah.bjfxy.top

C#:   if (x is null) {}
来源：http://xzx.hywenlv.cn

[P07] 防抖与节流
来源：http://joj.jinqigfzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://acg.yuanzhike.top

PHP:  // 手写时间戳比较
来源：http://zrc.wangshuangyany.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lfc.hnxiangtu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wfh.andypj.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://owe.fktsv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uud.yangfankeji.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://qxo.zhoulong.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ngk.ehwqpu.com

[P08] 处理浮点精度问题
来源：http://bfp.nwbrower.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://szr.ppjwa.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://aev.yfazqb.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jip.fzhhl.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nkp.iojbl.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ogn.hongshengwenyu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://afr.yonumen.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uww.ppjwa.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vwd.havefunace.top

================================================================================
来源：http://hgr.nwbrower.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nnk.xylfe.cn

================================================================================
来源：http://uox.iojbl.cn

[Q01] 创建表
来源：http://tqo.bjfxy.top

CREATE TABLE users (
来源：http://sfy.zhijiandao.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uno.redwolf501.top

name VARCHAR(50) NOT NULL,
来源：http://dob.daria6918.cn

email VARCHAR(100) UNIQUE,
来源：http://lvm.haohaochexian.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zjb.fehbvm.com

);
来源：http://wkx.hcnkem.com

[Q02] 创建带外键的表
来源：http://upj.nanxuanxn.top

CREATE TABLE orders (
来源：http://ajh.jlsjyb.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bvy.meibo888.top

user_id INT NOT NULL,
来源：http://kwi.cucudq.cn

amount DECIMAL(10, 2),
来源：http://lob.iojbl.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rrn.yonumen.top

);
来源：http://axv.yueranfly.top

[Q03] 增加列
来源：http://bsm.zhongyouzk.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ysh.c1oappe.top

[Q04] 修改列类型
来源：http://xpo.gzhubu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jxu.zhaomingkeji.xyz

[Q05] 重命名列
来源：http://otf.svipenyu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uzb.zycfv.cn

[Q06] 删除列
来源：http://csz.jinqigfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://dod.hnxiangtu.top

[Q07] 删除表
来源：http://tyy.jyoumei.cn

DROP TABLE IF EXISTS orders;
来源：http://nos.uphjek.com

[Q08] 创建普通索引
来源：http://ivh.cashguo.top

CREATE INDEX idx_users_email ON users(email);
来源：http://evf.shanyushiyangkeji.top

[Q09] 创建唯一索引
来源：http://zgm.zhixingplan.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://iyj.chenjidiqi.icu

[Q10] 插入单行
来源：http://bai.sjlbkw.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hvg.ydjk.org.cn

[Q11] 一次插入多行
来源：http://tyg.hnxiangtu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cxy.52xcode.cn

[Q12] 插入后取自增 ID
来源：http://xeo.zycfv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qzq.52xcode.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bma.daria6918.cn

[Q13] 忽略重复插入
来源：http://afy.cucudq.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://njw.nanxuanxn.top

[Q14] 存在则更新（upsert）
来源：http://sds.fengsongda.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pax.redwolf501.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fok.redwolf501.top

[Q15] 查询全部
来源：http://hhg.hfpthk.cn

SELECT * FROM users;
来源：http://bhw.uphjek.com

[Q16] 查询指定列
来源：http://wlx.cheryme.top

SELECT id, name FROM users;
来源：http://ndw.sjlbkw.cn

[Q17] 条件查询
来源：http://mbl.hesvh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ehx.gzhubu.top

[Q18] 模糊匹配
来源：http://vin.ydzc1.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mgy.sysykeji.top

[Q19] 范围查询
来源：http://ibq.yfazqb.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oqp.gaohongyu789.top

[Q20] IN 列表
来源：http://jvt.ydjk.org.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pem.nwbrower.top

[Q21] 空值判断
来源：http://btj.fengsongda.top

SELECT * FROM users WHERE email IS NULL;
来源：http://uia.gotoacloud.top

[Q22] 排序
来源：http://etu.zdbjq.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lqx.jinghuilouyu.cn

[Q23] 分页
来源：http://ilq.zycfv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wmz.jinyuanbaomall.cn

[Q24] 去重
来源：http://qem.yvedp.cn

SELECT DISTINCT city FROM users;
来源：http://qay.tianlin.xyz

[Q25] 只取前 N 条
来源：http://iat.yonumen.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://clr.jqgfzy.top

[Q26] 计数
来源：http://yzp.tarul.cn

SELECT COUNT(*) FROM users;
来源：http://ads.316326.xyz

[Q27] 条件计数
来源：http://pbl.yongpay.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ggx.andypj.xyz

[Q28] 求和与平均
来源：http://anj.shanyushiyangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kkl.gaohongyu789.top

[Q29] 最大最小值
来源：http://tnj.gzhubu.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://pwm.svipenyu.cn

[Q30] 分组统计
来源：http://reg.ydzc1.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yvw.jinghuilouyu.cn

[Q31] 分组后过滤
来源：http://meb.xuanzx.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ple.jinyuanbaomall.cn

[Q32] 分组拼接字符串
来源：http://fli.xuetiantiany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bae.sufxvd.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://iiu.yfazqb.com

[Q33] 多列分组
来源：http://pdu.jianghu66.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lmi.jqgfzy.top

[Q34] 每组取第一条
来源：http://aor.xuanzx.com

SELECT * FROM (
来源：http://mnv.yonumen.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dse.ppjwa.cn

) t WHERE rn = 1;
来源：http://ntl.bbcook.cn

[Q35] 内连接
来源：http://dlm.9152youxi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ciy.ydjk.org.cn

[Q36] 左连接
来源：http://xzj.vqdsnc.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mpw.yangfankeji.com

[Q37] 右连接
来源：http://zcr.zhixingplan.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pnh.quarkkingdee.top

[Q38] 全外连接（PostgreSQL）
来源：http://yvz.cashguo.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rwf.yueranfly.top

[Q39] 自连接（查上下级）
来源：http://nvn.yangfankeji.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://sth.jyoumei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ppv.hysaishi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xsr.vehdjk.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://abh.jinghuilouyu.cn

[Q41] 多表连接
来源：http://jqh.fanxiaobao.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://yej.hesvh.cn

JOIN users u ON u.id = o.user_id
来源：http://xjr.hongshengwenyu.top

JOIN products p ON p.id = o.product_id;
来源：http://mmu.havefunace.top

[Q42] 连接条件附加过滤
来源：http://zim.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u
来源：http://unk.mhx1999.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ukd.xuanzx.com

[Q43] 标量子查询
来源：http://yyv.jinyuanbaomall.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mxw.ctjpmb.com

[Q44] IN 子查询
来源：http://tul.zhaomingkeji.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ybn.fktsv.cn

[Q45] EXISTS 判断存在
来源：http://qoe.kuanghao11.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zvx.hesvh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://txp.ybcxt.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bkl.hnxiangtu.top

[Q47] 与平均值比较
来源：http://nws.epnwcf.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cjx.shzxlz.cn

[Q48] CTE 公用表表达式
来源：http://qqn.guannengcc.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gpr.snrcjt.cn

SELECT * FROM t WHERE c > 5;
来源：http://qzd.chenlongwang.top

[Q49] 更新单行
来源：http://djs.cheryme.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cjh.jianghu66.top

[Q50] 批量更新
来源：http://trt.tanke756.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hpd.fanxiaobao.xyz

[Q51] 用子查询更新
来源：http://jrr.chenlongwang.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jrl.yangfankeji.com

[Q52] 删除指定行
来源：http://ify.zycfv.cn

DELETE FROM users WHERE id = 10;
来源：http://fht.xinyue.icu

[Q53] 按条件删除
来源：http://isp.gogol.net.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fbh.fzhhl.top

[Q54] 清空表
来源：http://zfc.tarul.cn

TRUNCATE TABLE logs;
来源：http://dkh.xziqi.cn

[Q55] 排名（并列占位）
来源：http://jag.gotoacloud.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pry.zhoulong.xyz

[Q56] 密集排名（并列不占位）
来源：http://rzj.shzxlz.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yhu.shzxlz.cn

[Q57] 行号
来源：http://yoz.fktsv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hyo.wangshuangyany.cn

[Q58] 累计求和
来源：http://bnn.feifeiyinyue.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://scn.hysaishi.cn

[Q59] 分组内累计
来源：http://uan.yfazqb.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://abm.cheryme.top

[Q60] 取上一行 / 下一行
来源：http://noz.chenlongwang.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ldk.yj20258.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zdr.birdmap.top

[Q61] 移动平均
来源：http://yxh.dianchejie.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bqs.aibaodan.cn

[Q62] 分组占比
来源：http://krv.fehbvm.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mhv.zhongyouzk.top

[Q63] 开启事务
来源：http://kcr.fktsv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kor.jlsjyb.cn

[Q64] 提交事务
来源：http://raj.jiagoushi.top

COMMIT;
来源：http://wvu.sweek.top

[Q65] 回滚事务
来源：http://mrg.shangyingyoupin.top

ROLLBACK;
来源：http://jsm.gogol.net.cn

[Q66] 行锁查询
来源：http://lig.nanxuanxn.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pqp.havefunace.top

[Q67] 设置隔离级别
来源：http://blx.shangyingyoupin.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ygb.316326.xyz

[Q68] 保存点
来源：http://eiy.snrcjt.cn

SAVEPOINT sp1;
来源：http://bni.dianchejie.cn


<!-- 参考信息 -->