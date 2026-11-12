代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nve.hammf.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://liw.hysaishi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fks.zdqjudy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gro.ydjk.org.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://any.jqgfzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://moh.wangdashe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bbl.fanxiaobao.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bjw.jinqigfzy.top

================================================================================
来源：http://fbn.yangfankeji.com

O. 并发与异步
来源：http://wkq.c1oappe.top

================================================================================
来源：http://flm.hysaishi.cn

[O01] 启动一个线程
来源：http://vub.yanxiufei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uol.zhiwuduotai.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xqk.hnxiangtu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nbs.sufxvd.cn

TS:   // 同 JS
来源：http://ran.yuanzhike.top

Java: new Thread(() -> f()).start()
来源：http://icf.smart0.xyz

Go:   go f()
来源：http://aux.cashguo.top

Ruby: Thread.new { f }
来源：http://jjp.shangyingyoupin.top

C#:   Task.Run(() => F());
来源：http://amp.zhaomingkeji.xyz

[O02] 使用线程池
来源：http://nzt.yuanzhike.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hox.shanyushiyangtech.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cky.hnqzz.top

JS:   // worker_threads 线程池
来源：http://dmc.shzxlz.cn

TS:   // worker_threads 线程池
来源：http://gve.chenzaomai.com

Java: Executors.newFixedThreadPool(4)
来源：http://ixb.aizwys.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ray.daria6918.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wts.tianlin.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wuf.xinyue.icu

[O03] 加锁保护共享数据
来源：http://qus.jinghuilouyu.cn

Py:   with lock: shared += 1
来源：http://rxg.hammf.cn

PHP:  // 用 flock() 做文件锁
来源：http://nvl.chenlongwang.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mpu.yongpay.top

TS:   // 同 JS
来源：http://yhk.feifeiyinyue.top

Java: synchronized (this) { shared++; }
来源：http://ehl.ctjpmb.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zqe.zhongyouzk.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://etf.cashguo.top

C#:   lock (gate) { shared++; }
来源：http://kgw.dashuyun.cn

[O04] 定义异步函数并等待
来源：http://wpy.snrcjt.cn

Py:   async def f():⏎    await g()
来源：http://eot.bjfxy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://umz.cheryme.top

JS:   async function f() { await g(); }
来源：http://obp.jiagoushi.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://dhh.hammf.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oac.tanke756.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xep.uphjek.com

Ruby: # 用 Fiber 或 async gem
来源：http://fyt.nwbrower.top

C#:   async Task F() { await G(); }
来源：http://oqq.vehdjk.com

[O05] 并发执行并等待全部完成
来源：http://ujy.guowangkeji.top

Py:   asyncio.gather(*tasks)
来源：http://put.jiagoushi.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://saa.nanxinkj.top

JS:   await Promise.all(tasks)
来源：http://uhz.daxiang520.top

TS:   await Promise.all(tasks)
来源：http://kag.zhijiandao.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vut.nwbrower.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ajs.tian-w.cn

Ruby: threads.map(&:join)
来源：http://shi.svipenyu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ilz.zhengqikj.top

[O06] 使用进程池
来源：http://bvd.ydzc1.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vwr.havefunace.top

PHP:  // pcntl_fork 或多进程队列
来源：http://spu.kuanghao11.cn

JS:   // child_process / cluster 模块
来源：http://mwq.nwbrower.top

TS:   // child_process / cluster 模块
来源：http://ejd.pycfn.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pwu.gogol.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ifc.fengsongda.top

Ruby: // fork 块
来源：http://ank.kuanghao11.cn

C#:   Parallel.For
来源：http://fey.hesvh.cn

================================================================================
来源：http://bvu.jqgfzy.top

P. 常用工具函数
来源：http://mfc.tian-w.cn

================================================================================
来源：http://hbq.c1oappe.top

[P01] 生成 UUID
来源：http://afi.wangshuangyany.cn

Py:   str(uuid.uuid4())
来源：http://pnu.ehwqpu.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yzw.sysykeji.top

JS:   crypto.randomUUID()
来源：http://qtm.jqgfzy.top

TS:   crypto.randomUUID()
来源：http://xrg.redwolf501.top

Java: UUID.randomUUID().toString()
来源：http://knf.chenzaomai.com

Go:   // 用 github.com/google/uuid
来源：http://vsg.ehwqpu.com

Ruby: SecureRandom.uuid
来源：http://gck.yangfankeji.com

C#:   Guid.NewGuid().ToString()
来源：http://kkh.tanke756.top

[P02] MD5 / SHA256 摘要
来源：http://blb.jqgufenzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hvs.bjfxy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://uur.cdnleiting.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cct.ivvv.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xlj.sweek.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qdr.tanke756.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rcg.chenlongwang.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lyu.epnwcf.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fxu.jqgufenzy.top

[P03] 生成短随机字符串
来源：http://akl.jlsjyb.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://oiw.fzhhl.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://iwo.aizwys.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lux.sysykeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eoc.tarul.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cse.haohaochexian.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nyz.svipenyu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://phr.c1oappe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kpb.cucudq.cn

[P04] 求长度
来源：http://lbc.feifeiyinyue.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gzk.bjfxy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xwj.jinqigufen.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lbk.ydzc1.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ait.guowangkeji.top

Java: list.size();  map.size();  s.length()
来源：http://khr.aibaodan.cn

Go:   len(arr);  len(m)
来源：http://ohq.tarul.cn

Ruby: x.length;  x.size
来源：http://fwr.bjfxy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://din.jlsjyb.cn

[P05] 判断两个对象内容是否相等
来源：http://pcm.sweek.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://rzr.jinghuilouyu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xpy.ctjpmb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ayd.iojbl.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jsx.yuanzhike.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zoe.xuanzx.com

Go:   reflect.DeepEqual(a, b)
来源：http://bdy.jinghuilouyu.cn

Ruby: a == b
来源：http://rby.hysaishi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tzc.ppjwa.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nac.ywan-chungtsiang.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mwe.jinyuanbaomall.cn

PHP:  if (empty($x)) {}
来源：http://fnq.yj20258888.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sdd.zdbjq.cn

TS:   if (x == null) {}
来源：http://whs.uphjek.com

Java: if (x == null || x.isEmpty()) {}
来源：http://pgb.tanke756.top

Go:   if x == nil {}
来源：http://rhq.jlsjyb.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xyp.hnxiangtu.top

C#:   if (x is null) {}
来源：http://srp.dianchejie.cn

[P07] 防抖与节流
来源：http://grx.gotoacloud.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://udg.tanke756.top

PHP:  // 手写时间戳比较
来源：http://tfm.zhixingplan.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ooh.redwolf501.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bmk.hammf.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fbu.jqgfzy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://igb.uphjek.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://inw.hesvh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gww.guowangkeji.top

[P08] 处理浮点精度问题
来源：http://hwb.zycfv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bov.zhiwuduotai.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://knq.jinqigufen.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://efo.shanyushiyangtech.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mxn.meibo888.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qnf.kuanghao11.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ixm.cqqwz.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cyt.fktsv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://erb.xuanzx.com

================================================================================
来源：http://ltx.snrcjt.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lhg.xinyue.icu

================================================================================
来源：http://gqw.jinghuilouyu.cn

[Q01] 创建表
来源：http://puq.feifeiyinyue.top

CREATE TABLE users (
来源：http://alm.gogol.net.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zma.kuanghao11.cn

name VARCHAR(50) NOT NULL,
来源：http://bwm.zdqjudy.top

email VARCHAR(100) UNIQUE,
来源：http://dnn.chenlongwang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ick.9152youxi.cn

);
来源：http://agm.shuidangran.top

[Q02] 创建带外键的表
来源：http://rnk.zhengqikj.top

CREATE TABLE orders (
来源：http://hty.yuxming.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pte.bjfxy.top

user_id INT NOT NULL,
来源：http://ggi.vqdsnc.cn

amount DECIMAL(10, 2),
来源：http://cqo.ydzc1.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qaf.quarkkingdee.top

);
来源：http://zdv.andypj.xyz

[Q03] 增加列
来源：http://pxk.ppjwa.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bwf.aizwys.cn

[Q04] 修改列类型
来源：http://afp.hammf.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sku.chenzaomai.com

[Q05] 重命名列
来源：http://aqj.shangyingyoupin.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ujd.9152youxi.cn

[Q06] 删除列
来源：http://soi.shanyushiyangkeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://lft.ehwqpu.com

[Q07] 删除表
来源：http://fdl.tanke756.top

DROP TABLE IF EXISTS orders;
来源：http://sxn.feifeiyinyue.top

[Q08] 创建普通索引
来源：http://ovs.iojbl.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tcd.daria6918.cn

[Q09] 创建唯一索引
来源：http://zwk.fehbvm.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vjv.fanxiaobao.xyz

[Q10] 插入单行
来源：http://wcl.hcnkem.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mxr.zdbjq.cn

[Q11] 一次插入多行
来源：http://xry.hcnkem.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hrh.zhixingplan.top

[Q12] 插入后取自增 ID
来源：http://dig.zdqjudy.top

INSERT INTO users (name) VALUES ('C');
来源：http://ofx.dianchejie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kef.jinqigufen.top

[Q13] 忽略重复插入
来源：http://lhs.vehdjk.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dex.52xcode.cn

[Q14] 存在则更新（upsert）
来源：http://zpc.ppjwa.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pje.meibo888.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pbc.fzhhl.top

[Q15] 查询全部
来源：http://vcy.sxryk.cn

SELECT * FROM users;
来源：http://qhz.jinyuanbaomall.cn

[Q16] 查询指定列
来源：http://mcs.nwbrower.top

SELECT id, name FROM users;
来源：http://fbt.yuxming.cn

[Q17] 条件查询
来源：http://eok.tanke756.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://car.smart0.xyz

[Q18] 模糊匹配
来源：http://kpv.jinyuanbaomall.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tec.ctjpmb.com

[Q19] 范围查询
来源：http://ccs.sjlbkw.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fll.xingfuxueyuan.xyz

[Q20] IN 列表
来源：http://gaw.sysykeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://exl.cqqwz.cn

[Q21] 空值判断
来源：http://tmk.hnqzz.top

SELECT * FROM users WHERE email IS NULL;
来源：http://bki.yangfankeji.com

[Q22] 排序
来源：http://isd.fktsv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jzo.havefunace.top

[Q23] 分页
来源：http://mdz.yuanzhike.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rhj.shanyushiyangtech.top

[Q24] 去重
来源：http://kwj.chenjidiqi.icu

SELECT DISTINCT city FROM users;
来源：http://jfc.jinqigfzy.top

[Q25] 只取前 N 条
来源：http://fqb.fanxiaobao.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gyz.nanxinkj.top

[Q26] 计数
来源：http://zkr.guannengcc.top

SELECT COUNT(*) FROM users;
来源：http://xlc.cashguo.top

[Q27] 条件计数
来源：http://qrc.sjlbkw.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bav.ywan-chungtsiang.top

[Q28] 求和与平均
来源：http://smc.zhiwuduotai.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jgn.yvedp.cn

[Q29] 最大最小值
来源：http://owf.xziqi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xvs.ppjwa.cn

[Q30] 分组统计
来源：http://pdc.svipenyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ipe.sjlbkw.cn

[Q31] 分组后过滤
来源：http://hiq.nanxuanxn.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lsu.shanyushiyangtech.top

[Q32] 分组拼接字符串
来源：http://zzg.xinyue.icu

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://edw.feifeiyinyue.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jqe.epnwcf.com

[Q33] 多列分组
来源：http://tqn.havefunace.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fvk.zhiwuduotai.top

[Q34] 每组取第一条
来源：http://sru.xuanzx.com

SELECT * FROM (
来源：http://moh.yj20258.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dvr.cqqwz.cn

) t WHERE rn = 1;
来源：http://eka.shanyushiyangkeji.top

[Q35] 内连接
来源：http://ltb.vqdsnc.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gqw.quarkkingdee.top

[Q36] 左连接
来源：http://eor.tianlin.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qqy.wangshuangyany.cn

[Q37] 右连接
来源：http://acy.vqdsnc.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pmj.shangyingyoupin.top

[Q38] 全外连接（PostgreSQL）
来源：http://tzg.zhaomingkeji.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pbs.jiagoushi.top

[Q39] 自连接（查上下级）
来源：http://byb.xuetiantiany.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://oty.nanxinkj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ehb.sxryk.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rju.yvedp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kcg.yanxiufei.cn

[Q41] 多表连接
来源：http://lie.nanxinkj.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://zdd.cucudq.cn

JOIN users u ON u.id = o.user_id
来源：http://alw.guowangkeji.top

JOIN products p ON p.id = o.product_id;
来源：http://xai.yongpay.top

[Q42] 连接条件附加过滤
来源：http://tsh.pengpengdd.cyou

SELECT u.name, o.amount FROM users u
来源：http://jbo.zycfv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vhe.yuxming.cn

[Q43] 标量子查询
来源：http://lym.zhengqikj.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ezl.ppjwa.cn

[Q44] IN 子查询
来源：http://dzm.vehdjk.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wup.ydzc1.top

[Q45] EXISTS 判断存在
来源：http://yww.yfazqb.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wew.haohaochexian.top

[Q46] NOT EXISTS 判断不存在
来源：http://qbe.tianlin.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cty.yanxiufei.cn

[Q47] 与平均值比较
来源：http://flr.tarul.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ocz.fanxiaobao.xyz

[Q48] CTE 公用表表达式
来源：http://yul.wangshuangyany.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gtx.jqgfzy.top

SELECT * FROM t WHERE c > 5;
来源：http://qcd.shangyingyoupin.top

[Q49] 更新单行
来源：http://nuf.uphjek.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rkf.xinyue.icu

[Q50] 批量更新
来源：http://iip.yfazqb.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://reb.jinqigfzy.top

[Q51] 用子查询更新
来源：http://ygz.ybcxt.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://umo.zhijiandao.cn

[Q52] 删除指定行
来源：http://zyi.hysaishi.cn

DELETE FROM users WHERE id = 10;
来源：http://puz.pycfn.com

[Q53] 按条件删除
来源：http://les.sufxvd.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://him.tanke756.top

[Q54] 清空表
来源：http://rnb.yuxming.cn

TRUNCATE TABLE logs;
来源：http://wen.zhiwuduotai.top

[Q55] 排名（并列占位）
来源：http://hdr.ehwqpu.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lmr.tarul.cn

[Q56] 密集排名（并列不占位）
来源：http://hwl.yongpay.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rxh.xziqi.cn

[Q57] 行号
来源：http://cjn.zhoulong.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ycn.jinqigfzy.top

[Q58] 累计求和
来源：http://mkm.guannengcc.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uov.jiagoushi.top

[Q59] 分组内累计
来源：http://hie.smart0.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://drz.daria6918.cn

[Q60] 取上一行 / 下一行
来源：http://dou.yanxiufei.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://aow.epnwcf.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nvl.mhx1999.top

[Q61] 移动平均
来源：http://ovm.snrcjt.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dms.aibaodan.cn

[Q62] 分组占比
来源：http://aqr.cdnleiting.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://miz.yangfankeji.com

[Q63] 开启事务
来源：http://vre.vqdsnc.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://knf.daxiang520.top

[Q64] 提交事务
来源：http://zqi.nwbrower.top

COMMIT;
来源：http://sor.feifeiyinyue.top

[Q65] 回滚事务
来源：http://wzf.pycfn.com

ROLLBACK;
来源：http://oxq.shzxlz.cn

[Q66] 行锁查询
来源：http://cnp.hcnkem.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://iqd.svipenyu.cn

[Q67] 设置隔离级别
来源：http://own.xuanzx.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wqe.sjlbkw.cn

[Q68] 保存点
来源：http://dsw.jinyuanbaomall.cn

SAVEPOINT sp1;
来源：http://jip.sysykeji.top


<!-- 参考信息 -->