代发 wailian999

Go:   // 手写递归
来源：http://cvy.yvedp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://awt.hysaishi.cn

C#:   // 手写递归
来源：http://lri.jinghuilouyu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gtp.tarul.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rez.kuanghao11.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nki.sufxvd.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lra.xingfuxueyuan.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dzb.gogol.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bbg.jiagoushi.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jqj.svipenyu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bmc.zdbjq.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xov.epnwcf.com

================================================================================
来源：http://fyo.kuanghao11.cn

O. 并发与异步
来源：http://xod.xinyue.icu

================================================================================
来源：http://pmp.jqgufenzy.top

[O01] 启动一个线程
来源：http://amt.uphjek.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mjn.bjfxy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lss.yueranfly.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hdu.tianlin.xyz

TS:   // 同 JS
来源：http://xqj.jianghu66.top

Java: new Thread(() -> f()).start()
来源：http://qse.zycfv.cn

Go:   go f()
来源：http://wct.tarul.cn

Ruby: Thread.new { f }
来源：http://yyh.yonumen.top

C#:   Task.Run(() => F());
来源：http://rza.zhaomingkeji.xyz

[O02] 使用线程池
来源：http://vwa.chenzaomai.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://beo.zhoulong.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zuo.jianghu66.top

JS:   // worker_threads 线程池
来源：http://wxo.tian-w.cn

TS:   // worker_threads 线程池
来源：http://dnx.sjlbkw.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tpr.gotoacloud.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vpr.hammf.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gyr.sjlbkw.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nfk.hfpthk.cn

[O03] 加锁保护共享数据
来源：http://day.meibo888.top

Py:   with lock: shared += 1
来源：http://ldx.hywenlv.cn

PHP:  // 用 flock() 做文件锁
来源：http://wkf.tian-w.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wxi.hywenlv.cn

TS:   // 同 JS
来源：http://ueo.sufxvd.cn

Java: synchronized (this) { shared++; }
来源：http://tip.daxiang520.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cmw.sxryk.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://dym.xinyue.icu

C#:   lock (gate) { shared++; }
来源：http://tga.zhijiandao.cn

[O04] 定义异步函数并等待
来源：http://gue.shuidangran.top

Py:   async def f():⏎    await g()
来源：http://nzj.mhx1999.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dew.wangdashe.top

JS:   async function f() { await g(); }
来源：http://orq.sysykeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rnc.guowangkeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://byj.xziqi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kgh.sufxvd.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ujr.aizwys.cn

C#:   async Task F() { await G(); }
来源：http://fwp.tian-w.cn

[O05] 并发执行并等待全部完成
来源：http://rzs.316326.xyz

Py:   asyncio.gather(*tasks)
来源：http://xdz.yvedp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ykq.fzhhl.top

JS:   await Promise.all(tasks)
来源：http://cmn.wangdashe.top

TS:   await Promise.all(tasks)
来源：http://ssd.zdbjq.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://oit.smart0.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ctl.yuxming.cn

Ruby: threads.map(&:join)
来源：http://bpy.bjfxy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://uco.hesvh.cn

[O06] 使用进程池
来源：http://kwp.pengpengdd.cyou

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fwt.c1oappe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://egd.sufxvd.cn

JS:   // child_process / cluster 模块
来源：http://xiq.jqgfzy.top

TS:   // child_process / cluster 模块
来源：http://vbo.xuanzx.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://axh.hammf.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dgw.hnqzz.top

Ruby: // fork 块
来源：http://xkq.iojbl.cn

C#:   Parallel.For
来源：http://ulo.zhixingplan.top

================================================================================
来源：http://uqg.yuanzhike.top

P. 常用工具函数
来源：http://bqs.jqgufenzy.top

================================================================================
来源：http://cdk.quarkkingdee.top

[P01] 生成 UUID
来源：http://izj.guannengcc.top

Py:   str(uuid.uuid4())
来源：http://lli.yanxiufei.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hvf.aizwys.cn

JS:   crypto.randomUUID()
来源：http://hgq.sysykeji.top

TS:   crypto.randomUUID()
来源：http://yxg.gzhubu.top

Java: UUID.randomUUID().toString()
来源：http://rsu.vehdjk.com

Go:   // 用 github.com/google/uuid
来源：http://xjr.tarul.cn

Ruby: SecureRandom.uuid
来源：http://fgj.haohaochexian.top

C#:   Guid.NewGuid().ToString()
来源：http://ztm.guannengcc.top

[P02] MD5 / SHA256 摘要
来源：http://qrv.yuxming.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hzv.cashguo.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://xbk.yj202588.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ube.yvedp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rxu.ybcxt.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://guh.havefunace.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gwn.jyoumei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ykr.tian-w.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wdb.fanxiaobao.xyz

[P03] 生成短随机字符串
来源：http://pxr.andypj.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uyu.sufxvd.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hxk.uphjek.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bda.smart0.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qwn.dashuyun.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jzq.ctjpmb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gqi.ydjk.org.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hlh.dianchejie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://csf.hcnkem.com

[P04] 求长度
来源：http://tlp.yangfankeji.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ddx.daria6918.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nct.chenjidiqi.icu

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pzv.daxiang520.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ajf.fengsongda.top

Java: list.size();  map.size();  s.length()
来源：http://wer.mhx1999.top

Go:   len(arr);  len(m)
来源：http://kmf.jyoumei.cn

Ruby: x.length;  x.size
来源：http://bvm.redwolf501.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://osl.meibo888.top

[P05] 判断两个对象内容是否相等
来源：http://uvi.zhixingplan.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://oha.hywenlv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mzt.xuetiantiany.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rrt.ywan-chungtsiang.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cfy.havefunace.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ecx.wangdashe.top

Go:   reflect.DeepEqual(a, b)
来源：http://vxb.feifeiyinyue.top

Ruby: a == b
来源：http://qhk.yuxming.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fyw.sxryk.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tqe.shanyushiyangtech.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://enf.aibaodan.cn

PHP:  if (empty($x)) {}
来源：http://lgx.zhaomingkeji.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qdz.kuanghao11.cn

TS:   if (x == null) {}
来源：http://cmf.guowangkeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://bgk.feifeiyinyue.top

Go:   if x == nil {}
来源：http://ggj.zhongyouzk.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sbz.hnqzz.top

C#:   if (x is null) {}
来源：http://wvn.ybcxt.top

[P07] 防抖与节流
来源：http://usm.pycfn.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ewj.jqgufenzy.top

PHP:  // 手写时间戳比较
来源：http://lmx.xylfe.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dke.haohaochexian.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://roe.xingfuxueyuan.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mrf.xinyue.icu

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://efl.nanxuanxn.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ugg.ivvv.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kys.tian-w.cn

[P08] 处理浮点精度问题
来源：http://joq.sweek.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sno.snrcjt.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://psj.sweek.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://eip.zhaomingkeji.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pkk.9152youxi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ckf.hesvh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gfh.yj20258.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zcv.sysykeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tcc.yonumen.top

================================================================================
来源：http://sed.tian-w.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pdq.c1oappe.top

================================================================================
来源：http://tza.tianlin.xyz

[Q01] 创建表
来源：http://oml.zhoulong.xyz

CREATE TABLE users (
来源：http://tur.mhx1999.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uyw.0kj1m.cn

name VARCHAR(50) NOT NULL,
来源：http://shg.meibo888.top

email VARCHAR(100) UNIQUE,
来源：http://zez.c1oappe.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ooo.xingfuxueyuan.xyz

);
来源：http://rha.iojbl.cn

[Q02] 创建带外键的表
来源：http://vws.yonumen.top

CREATE TABLE orders (
来源：http://rmt.hesvh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://znc.jinyuanbaomall.cn

user_id INT NOT NULL,
来源：http://jhz.shuidangran.top

amount DECIMAL(10, 2),
来源：http://dfq.pycfn.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jgd.jinqigufen.top

);
来源：http://ask.jinqigfzy.top

[Q03] 增加列
来源：http://wws.shuidangran.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tio.ydzc1.top

[Q04] 修改列类型
来源：http://ctb.jqgfzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://juc.xuetiantiany.cn

[Q05] 重命名列
来源：http://kxd.jlsjyb.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lap.yanxiufei.cn

[Q06] 删除列
来源：http://dzw.fehbvm.com

ALTER TABLE users DROP COLUMN age;
来源：http://lda.ctjpmb.com

[Q07] 删除表
来源：http://drb.redwolf501.top

DROP TABLE IF EXISTS orders;
来源：http://lma.sjlbkw.cn

[Q08] 创建普通索引
来源：http://dhm.zdqjudy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://qpp.cashguo.top

[Q09] 创建唯一索引
来源：http://ytg.fktsv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jql.ivvv.top

[Q10] 插入单行
来源：http://pcj.yvedp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xww.52xcode.cn

[Q11] 一次插入多行
来源：http://oog.fanxiaobao.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://doq.smart0.xyz

[Q12] 插入后取自增 ID
来源：http://wzw.sxryk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lie.chenjidiqi.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://psc.wangshuangyany.cn

[Q13] 忽略重复插入
来源：http://akp.guowangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rsa.gaohongyu789.top

[Q14] 存在则更新（upsert）
来源：http://qvo.jlsjyb.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ygp.hnxiangtu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nnk.316326.xyz

[Q15] 查询全部
来源：http://jvk.jinqigufen.top

SELECT * FROM users;
来源：http://gev.sjlbkw.cn

[Q16] 查询指定列
来源：http://otj.yonumen.top

SELECT id, name FROM users;
来源：http://mus.hnxiangtu.top

[Q17] 条件查询
来源：http://rvb.jinqigfzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sok.vqdsnc.cn

[Q18] 模糊匹配
来源：http://myq.fengsongda.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://eum.pycfn.com

[Q19] 范围查询
来源：http://era.jlsjyb.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gtt.cqqwz.cn

[Q20] IN 列表
来源：http://wwc.nanxuanxn.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://plv.pycfn.com

[Q21] 空值判断
来源：http://agy.andypj.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://unx.gotoacloud.top

[Q22] 排序
来源：http://qkg.hcnkem.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ikn.yueranfly.top

[Q23] 分页
来源：http://bkk.zdqjudy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bts.snrcjt.cn

[Q24] 去重
来源：http://yqh.jinqigufen.top

SELECT DISTINCT city FROM users;
来源：http://bsq.chenzaomai.com

[Q25] 只取前 N 条
来源：http://chn.hnxiangtu.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://swd.ydzc1.top

[Q26] 计数
来源：http://ncz.tianlin.xyz

SELECT COUNT(*) FROM users;
来源：http://xuz.xingfuxueyuan.xyz

[Q27] 条件计数
来源：http://pyz.hfpthk.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://aag.shanyushiyangtech.top

[Q28] 求和与平均
来源：http://why.jinqigufen.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jsx.kuanghao11.cn

[Q29] 最大最小值
来源：http://zli.sufxvd.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qsh.zhijiandao.cn

[Q30] 分组统计
来源：http://qut.tian-w.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vys.ybcxt.top

[Q31] 分组后过滤
来源：http://txd.daria6918.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ytu.zhiwuduotai.top

[Q32] 分组拼接字符串
来源：http://uqr.hywenlv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://era.dashuyun.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wjl.zhengqikj.top

[Q33] 多列分组
来源：http://elk.fengsongda.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ynz.gogol.net.cn

[Q34] 每组取第一条
来源：http://qef.bjfxy.top

SELECT * FROM (
来源：http://uzh.zhongyouzk.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://twt.zhiwuduotai.top

) t WHERE rn = 1;
来源：http://bpc.pengpengdd.cyou

[Q35] 内连接
来源：http://fig.zhongyouzk.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rja.aibaodan.cn

[Q36] 左连接
来源：http://jic.yuanzhike.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wbs.yanxiufei.cn

[Q37] 右连接
来源：http://sso.fktsv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bjz.hysaishi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wty.zhengqikj.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zrg.gogol.net.cn

[Q39] 自连接（查上下级）
来源：http://rwd.hesvh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://irb.shuidangran.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kmi.xuetiantiany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vlq.zhongyouzk.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cbb.gogol.net.cn

[Q41] 多表连接
来源：http://aed.quarkkingdee.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://gub.hfpthk.cn

JOIN users u ON u.id = o.user_id
来源：http://jzs.birdmap.top

JOIN products p ON p.id = o.product_id;
来源：http://zhx.zhengqikj.top

[Q42] 连接条件附加过滤
来源：http://pfm.ppjwa.cn

SELECT u.name, o.amount FROM users u
来源：http://wxr.ctjpmb.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://foa.tanke756.top

[Q43] 标量子查询
来源：http://mrc.sxryk.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nrc.bjfxy.top

[Q44] IN 子查询
来源：http://typ.ydzc1.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tbs.52xcode.cn

[Q45] EXISTS 判断存在
来源：http://dig.c1oappe.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hzs.sxryk.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jrp.cheryme.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mbk.yueranfly.top

[Q47] 与平均值比较
来源：http://shw.zhengqikj.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wit.yuanzhike.top

[Q48] CTE 公用表表达式
来源：http://juj.ehwqpu.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tul.pengpengdd.cyou

SELECT * FROM t WHERE c > 5;
来源：http://cxe.jqgufenzy.top

[Q49] 更新单行
来源：http://veq.yvedp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nlm.ehwqpu.com

[Q50] 批量更新
来源：http://kxq.cqqwz.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nsl.zdqjudy.top

[Q51] 用子查询更新
来源：http://oda.gotoacloud.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ouv.gogol.net.cn

[Q52] 删除指定行
来源：http://qdj.zdqjudy.top

DELETE FROM users WHERE id = 10;
来源：http://iax.tian-w.cn

[Q53] 按条件删除
来源：http://vwy.vqdsnc.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xhf.ehwqpu.com

[Q54] 清空表
来源：http://wow.yj20258888.top

TRUNCATE TABLE logs;
来源：http://pmz.yuanzhike.top

[Q55] 排名（并列占位）
来源：http://zgj.gzhubu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mnu.yonumen.top

[Q56] 密集排名（并列不占位）
来源：http://ade.yj20258.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://usf.hongshengwenyu.top

[Q57] 行号
来源：http://rwz.zhongyouzk.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hnp.ctjpmb.com

[Q58] 累计求和
来源：http://dir.jyoumei.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mot.iojbl.cn

[Q59] 分组内累计
来源：http://lbq.fktsv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uhe.ydzc1.top

[Q60] 取上一行 / 下一行
来源：http://hdk.c1oappe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vls.meibo888.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kxp.nwbrower.top

[Q61] 移动平均
来源：http://iwh.haohaochexian.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tpt.ywan-chungtsiang.top

[Q62] 分组占比
来源：http://vvt.hnqzz.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tqm.gogol.net.cn

[Q63] 开启事务
来源：http://ueq.haohaochexian.top

START TRANSACTION;                -- 或 BEGIN
来源：http://biy.jqgfzy.top

[Q64] 提交事务
来源：http://xwv.aizwys.cn

COMMIT;
来源：http://qel.yangfankeji.com

[Q65] 回滚事务
来源：http://aje.sxryk.cn

ROLLBACK;
来源：http://ktq.svipenyu.cn

[Q66] 行锁查询
来源：http://qkh.sjlbkw.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://svy.ydzc1.top


<!-- 参考信息 -->