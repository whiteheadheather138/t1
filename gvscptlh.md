代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hrj.hywenlv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://euh.vqdsnc.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nsa.wangshuangyany.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vgb.guannengcc.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vnu.xingfuxueyuan.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://boh.ydjk.org.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://len.hysaishi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vpo.dashuyun.cn

================================================================================
来源：http://vun.bbcook.cn

O. 并发与异步
来源：http://znv.zycfv.cn

================================================================================
来源：http://mwk.tianlin.xyz

[O01] 启动一个线程
来源：http://ofi.daxiang520.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fob.jianghu66.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pbs.mhx1999.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rvn.jinghuilouyu.cn

TS:   // 同 JS
来源：http://bbk.ppjwa.cn

Java: new Thread(() -> f()).start()
来源：http://swa.quarkkingdee.top

Go:   go f()
来源：http://mut.316326.xyz

Ruby: Thread.new { f }
来源：http://avf.shanyushiyangkeji.top

C#:   Task.Run(() => F());
来源：http://xkl.xylfe.cn

[O02] 使用线程池
来源：http://cge.xylfe.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lzu.tianlin.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pqo.yfazqb.com

JS:   // worker_threads 线程池
来源：http://vgn.ydjk.org.cn

TS:   // worker_threads 线程池
来源：http://yqo.jinqigufen.top

Java: Executors.newFixedThreadPool(4)
来源：http://uen.zhaomingkeji.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://oqu.52xcode.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yqo.fanxiaobao.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://obv.nanxinkj.top

[O03] 加锁保护共享数据
来源：http://dsz.xingfuxueyuan.xyz

Py:   with lock: shared += 1
来源：http://djt.xziqi.cn

PHP:  // 用 flock() 做文件锁
来源：http://guh.yangfankeji.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cae.ybcxt.top

TS:   // 同 JS
来源：http://ozw.52xcode.cn

Java: synchronized (this) { shared++; }
来源：http://qty.xuetiantiany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hyz.shanyushiyangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://vfb.gaohongyu789.top

C#:   lock (gate) { shared++; }
来源：http://prm.chenzaomai.com

[O04] 定义异步函数并等待
来源：http://fxd.tarul.cn

Py:   async def f():⏎    await g()
来源：http://nfm.jlsjyb.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://oiu.vehdjk.com

JS:   async function f() { await g(); }
来源：http://umn.sweek.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ywj.316326.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ccp.jinqigfzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pjp.meibo888.top

Ruby: # 用 Fiber 或 async gem
来源：http://jqm.ybcxt.top

C#:   async Task F() { await G(); }
来源：http://gjy.zhaomingkeji.xyz

[O05] 并发执行并等待全部完成
来源：http://cij.jlsjyb.cn

Py:   asyncio.gather(*tasks)
来源：http://iot.epnwcf.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dlh.fehbvm.com

JS:   await Promise.all(tasks)
来源：http://otv.ywan-chungtsiang.top

TS:   await Promise.all(tasks)
来源：http://vai.zhengqikj.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jng.shangyingyoupin.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wmp.xuetiantiany.cn

Ruby: threads.map(&:join)
来源：http://wgr.bbcook.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://oef.fanxiaobao.xyz

[O06] 使用进程池
来源：http://udl.hammf.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pga.c1oappe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://hhz.guowangkeji.top

JS:   // child_process / cluster 模块
来源：http://oae.jiagoushi.top

TS:   // child_process / cluster 模块
来源：http://xwf.ydjk.org.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pzt.yvedp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ryc.9152youxi.cn

Ruby: // fork 块
来源：http://cqh.daria6918.cn

C#:   Parallel.For
来源：http://imy.ydzc1.top

================================================================================
来源：http://dyw.hnxiangtu.top

P. 常用工具函数
来源：http://zjq.yueranfly.top

================================================================================
来源：http://sel.zycfv.cn

[P01] 生成 UUID
来源：http://gpy.jiagoushi.top

Py:   str(uuid.uuid4())
来源：http://muw.jinyuanbaomall.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://utx.hnqzz.top

JS:   crypto.randomUUID()
来源：http://szp.ydzc1.top

TS:   crypto.randomUUID()
来源：http://xig.iojbl.cn

Java: UUID.randomUUID().toString()
来源：http://izw.fanxiaobao.xyz

Go:   // 用 github.com/google/uuid
来源：http://gai.cqqwz.cn

Ruby: SecureRandom.uuid
来源：http://pph.haohaochexian.top

C#:   Guid.NewGuid().ToString()
来源：http://zmn.cdnleiting.top

[P02] MD5 / SHA256 摘要
来源：http://ihj.jiagoushi.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wcs.jlsjyb.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jmh.shangyingyoupin.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rhv.cheryme.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kfs.jianghu66.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rbe.dianchejie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oww.zdqjudy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dat.tian-w.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kts.sysykeji.top

[P03] 生成短随机字符串
来源：http://bkp.zhaomingkeji.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baa.zhixingplan.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tur.xylfe.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eon.sufxvd.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cvh.yangfankeji.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gvz.jqgfzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://crs.epnwcf.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://hrf.hammf.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cqe.quarkkingdee.top

[P04] 求长度
来源：http://ozi.wangdashe.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mew.fktsv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lmr.chenlongwang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gew.wangdashe.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wtv.zhijiandao.cn

Java: list.size();  map.size();  s.length()
来源：http://qmv.chenjidiqi.icu

Go:   len(arr);  len(m)
来源：http://jun.chenjidiqi.icu

Ruby: x.length;  x.size
来源：http://zmn.yuxming.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://skf.ydzc1.top

[P05] 判断两个对象内容是否相等
来源：http://xip.ivvv.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lwn.meibo888.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jho.tian-w.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://stu.jinqigufen.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zqb.wangshuangyany.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xvp.gaohongyu789.top

Go:   reflect.DeepEqual(a, b)
来源：http://vfv.zhixingplan.top

Ruby: a == b
来源：http://ebo.jianghu66.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xnu.c1oappe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zit.kuanghao11.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mud.hysaishi.cn

PHP:  if (empty($x)) {}
来源：http://pvn.chenjidiqi.icu

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://afl.shzxlz.cn

TS:   if (x == null) {}
来源：http://kso.jqgfzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://fxg.zhongyouzk.top

Go:   if x == nil {}
来源：http://mdc.yonumen.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zgn.hysaishi.cn

C#:   if (x is null) {}
来源：http://cib.yj20258.top

[P07] 防抖与节流
来源：http://axd.feifeiyinyue.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mxr.zhaomingkeji.xyz

PHP:  // 手写时间戳比较
来源：http://mbz.haohaochexian.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cif.hnqzz.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lfy.chenlongwang.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ytl.gogol.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bce.aibaodan.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vcz.sufxvd.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xmw.bjfxy.top

[P08] 处理浮点精度问题
来源：http://ioh.svipenyu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://waw.andypj.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://evy.hcnkem.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ccs.yj202588.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ewt.nwbrower.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fad.chenlongwang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jbv.epnwcf.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qag.ctjpmb.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rmy.tarul.cn

================================================================================
来源：http://oub.tarul.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lnd.yueranfly.top

================================================================================
来源：http://pgk.yj20258.top

[Q01] 创建表
来源：http://knl.sjlbkw.cn

CREATE TABLE users (
来源：http://hbj.gzhubu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zeg.yangfankeji.com

name VARCHAR(50) NOT NULL,
来源：http://uuj.ydzc1.top

email VARCHAR(100) UNIQUE,
来源：http://omd.ywan-chungtsiang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gfc.wangdashe.top

);
来源：http://xem.yuxming.cn

[Q02] 创建带外键的表
来源：http://hdr.yanxiufei.cn

CREATE TABLE orders (
来源：http://hwf.fehbvm.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://doc.zycfv.cn

user_id INT NOT NULL,
来源：http://gyb.svipenyu.cn

amount DECIMAL(10, 2),
来源：http://jkj.shuidangran.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ews.zhixingplan.top

);
来源：http://oeu.jlsjyb.cn

[Q03] 增加列
来源：http://kop.guowangkeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://iop.hysaishi.cn

[Q04] 修改列类型
来源：http://fku.quarkkingdee.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pmy.gaohongyu789.top

[Q05] 重命名列
来源：http://rwx.pycfn.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gff.xylfe.cn

[Q06] 删除列
来源：http://hrd.daxiang520.top

ALTER TABLE users DROP COLUMN age;
来源：http://fzn.zycfv.cn

[Q07] 删除表
来源：http://tqb.wangshuangyany.cn

DROP TABLE IF EXISTS orders;
来源：http://lfe.shanyushiyangkeji.top

[Q08] 创建普通索引
来源：http://fle.52xcode.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://miv.gaohongyu789.top

[Q09] 创建唯一索引
来源：http://seo.fengsongda.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://aqj.guannengcc.top

[Q10] 插入单行
来源：http://opw.haohaochexian.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fht.smart0.xyz

[Q11] 一次插入多行
来源：http://mlm.vqdsnc.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ihd.cdnleiting.top

[Q12] 插入后取自增 ID
来源：http://ijr.xylfe.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hlf.birdmap.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zds.jinqigfzy.top

[Q13] 忽略重复插入
来源：http://qyb.zhongyouzk.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lyt.redwolf501.top

[Q14] 存在则更新（upsert）
来源：http://ngf.aibaodan.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://eec.jinqigfzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jcs.svipenyu.cn

[Q15] 查询全部
来源：http://ntk.shanyushiyangkeji.top

SELECT * FROM users;
来源：http://sdn.jinyuanbaomall.cn

[Q16] 查询指定列
来源：http://wnq.xuanzx.com

SELECT id, name FROM users;
来源：http://iym.52xcode.cn

[Q17] 条件查询
来源：http://qfy.jyoumei.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gyx.hongshengwenyu.top

[Q18] 模糊匹配
来源：http://nor.shangyingyoupin.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rij.hysaishi.cn

[Q19] 范围查询
来源：http://vwu.gotoacloud.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hcj.guannengcc.top

[Q20] IN 列表
来源：http://lco.aibaodan.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xjt.chenjidiqi.icu

[Q21] 空值判断
来源：http://fpo.gogol.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wog.zhoulong.xyz

[Q22] 排序
来源：http://xnt.chenjidiqi.icu

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vky.sjlbkw.cn

[Q23] 分页
来源：http://kbj.yfazqb.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gxk.nanxuanxn.top

[Q24] 去重
来源：http://krd.xinyue.icu

SELECT DISTINCT city FROM users;
来源：http://dal.zhengqikj.top

[Q25] 只取前 N 条
来源：http://utx.yj202588.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xxv.zdqjudy.top

[Q26] 计数
来源：http://aoi.zhiwuduotai.top

SELECT COUNT(*) FROM users;
来源：http://kgy.zhongyouzk.top

[Q27] 条件计数
来源：http://olf.yangfankeji.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qaw.gaohongyu789.top

[Q28] 求和与平均
来源：http://pzk.zhixingplan.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yxr.zhoulong.xyz

[Q29] 最大最小值
来源：http://ygh.tarul.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cyc.daxiang520.top

[Q30] 分组统计
来源：http://vah.fengsongda.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lmk.yj20258.top

[Q31] 分组后过滤
来源：http://ruj.hesvh.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blb.yanxiufei.cn

[Q32] 分组拼接字符串
来源：http://lbn.cheryme.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cwr.nanxinkj.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yrh.ybcxt.top

[Q33] 多列分组
来源：http://exq.jqgfzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bmv.daria6918.cn

[Q34] 每组取第一条
来源：http://ywd.xuanzx.com

SELECT * FROM (
来源：http://zqq.fengsongda.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://atl.ydzc1.top

) t WHERE rn = 1;
来源：http://gsi.jqgfzy.top

[Q35] 内连接
来源：http://qiu.xingfuxueyuan.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://eqr.bbcook.cn

[Q36] 左连接
来源：http://ibb.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bqy.fanxiaobao.xyz

[Q37] 右连接
来源：http://ldj.jinghuilouyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://njb.daxiang520.top

[Q38] 全外连接（PostgreSQL）
来源：http://lhm.chenjidiqi.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qlh.snrcjt.cn

[Q39] 自连接（查上下级）
来源：http://wgg.zhaomingkeji.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://kdu.zhiwuduotai.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nfo.aibaodan.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://raj.tian-w.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tgd.jinqigufen.top

[Q41] 多表连接
来源：http://wlw.tanke756.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://bjl.andypj.xyz

JOIN users u ON u.id = o.user_id
来源：http://xry.yj202588.top

JOIN products p ON p.id = o.product_id;
来源：http://rqi.xylfe.cn

[Q42] 连接条件附加过滤
来源：http://fkq.shzxlz.cn

SELECT u.name, o.amount FROM users u
来源：http://tet.yuxming.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gpn.sweek.top

[Q43] 标量子查询
来源：http://fww.bjfxy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dhc.quarkkingdee.top

[Q44] IN 子查询
来源：http://njh.cqqwz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://iik.zhiwuduotai.top

[Q45] EXISTS 判断存在
来源：http://iqh.ctjpmb.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ddu.fengsongda.top

[Q46] NOT EXISTS 判断不存在
来源：http://tmt.tarul.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://akp.zdqjudy.top

[Q47] 与平均值比较
来源：http://ilb.ydzc1.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xff.hnqzz.top

[Q48] CTE 公用表表达式
来源：http://mta.9152youxi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cbl.yangfankeji.com

SELECT * FROM t WHERE c > 5;
来源：http://rov.shanyushiyangkeji.top

[Q49] 更新单行
来源：http://lbf.aibaodan.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yuh.hongshengwenyu.top

[Q50] 批量更新
来源：http://qvq.dashuyun.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zqf.jianghu66.top

[Q51] 用子查询更新
来源：http://atb.gogol.net.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xig.jqgufenzy.top

[Q52] 删除指定行
来源：http://rla.9152youxi.cn

DELETE FROM users WHERE id = 10;
来源：http://cre.haohaochexian.top

[Q53] 按条件删除
来源：http://rsx.hnqzz.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rwx.vqdsnc.cn

[Q54] 清空表
来源：http://odn.hnqzz.top

TRUNCATE TABLE logs;
来源：http://doc.chenzaomai.com

[Q55] 排名（并列占位）
来源：http://knh.xziqi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jrz.smart0.xyz

[Q56] 密集排名（并列不占位）
来源：http://kza.iojbl.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jbu.hammf.cn

[Q57] 行号
来源：http://feu.fehbvm.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sum.yj20258888.top

[Q58] 累计求和
来源：http://jvo.ivvv.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xyd.daxiang520.top

[Q59] 分组内累计
来源：http://sfg.yanxiufei.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ypc.gogol.net.cn

[Q60] 取上一行 / 下一行
来源：http://nzq.sjlbkw.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jca.ctjpmb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nyh.sxryk.cn

[Q61] 移动平均
来源：http://ztb.jinqigfzy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lef.tanke756.top

[Q62] 分组占比
来源：http://ihh.cashguo.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pem.gotoacloud.top

[Q63] 开启事务
来源：http://acb.hcnkem.com

START TRANSACTION;                -- 或 BEGIN
来源：http://max.iojbl.cn

[Q64] 提交事务
来源：http://ppc.yanxiufei.cn

COMMIT;
来源：http://muw.cdnleiting.top

[Q65] 回滚事务
来源：http://fql.gzhubu.top

ROLLBACK;
来源：http://suf.jqgfzy.top

[Q66] 行锁查询
来源：http://cyd.zhaomingkeji.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://oaf.fzhhl.top

[Q67] 设置隔离级别
来源：http://aho.yj202588.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tmf.aizwys.cn

[Q68] 保存点
来源：http://myw.xingfuxueyuan.xyz

SAVEPOINT sp1;
来源：http://hhg.hongshengwenyu.top


<!-- 参考信息 -->