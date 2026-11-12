代发 wailian999

PHP:  // 手写递归函数
来源：http://reo.cheryme.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rjg.xuetiantiany.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://veh.chenjidiqi.icu

Java: // 手写递归
来源：http://itx.cheryme.top

Go:   // 手写递归
来源：http://guz.iojbl.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://syv.zdqjudy.top

C#:   // 手写递归
来源：http://see.cdnleiting.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bva.yanxiufei.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://flo.jinqigfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://foj.ehwqpu.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yap.fanxiaobao.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rwe.snrcjt.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ryz.yuxming.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fhp.zhongyouzk.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ofd.sjlbkw.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://udt.shzxlz.cn

================================================================================
来源：http://hpb.hnxiangtu.top

O. 并发与异步
来源：http://ybp.nwbrower.top

================================================================================
来源：http://kjn.ehwqpu.com

[O01] 启动一个线程
来源：http://jgb.fktsv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://src.hammf.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://seo.9152youxi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://amr.sysykeji.top

TS:   // 同 JS
来源：http://eoi.yvedp.cn

Java: new Thread(() -> f()).start()
来源：http://hmj.hysaishi.cn

Go:   go f()
来源：http://bkc.nwbrower.top

Ruby: Thread.new { f }
来源：http://tqc.sxryk.cn

C#:   Task.Run(() => F());
来源：http://qbe.wangdashe.top

[O02] 使用线程池
来源：http://eor.ctjpmb.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hut.yongpay.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vvo.yj20258.top

JS:   // worker_threads 线程池
来源：http://hwk.guowangkeji.top

TS:   // worker_threads 线程池
来源：http://npq.feifeiyinyue.top

Java: Executors.newFixedThreadPool(4)
来源：http://vja.yueranfly.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hjs.bjfxy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://faf.nanxuanxn.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wan.jiagoushi.top

[O03] 加锁保护共享数据
来源：http://sbl.tanke756.top

Py:   with lock: shared += 1
来源：http://wwm.cheryme.top

PHP:  // 用 flock() 做文件锁
来源：http://umo.yvedp.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ziq.gogol.net.cn

TS:   // 同 JS
来源：http://fgg.shzxlz.cn

Java: synchronized (this) { shared++; }
来源：http://zel.zycfv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vuy.sysykeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://dai.svipenyu.cn

C#:   lock (gate) { shared++; }
来源：http://afa.hnxiangtu.top

[O04] 定义异步函数并等待
来源：http://wcx.zhiwuduotai.top

Py:   async def f():⏎    await g()
来源：http://irr.chenlongwang.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bkg.ctjpmb.com

JS:   async function f() { await g(); }
来源：http://xxq.mhx1999.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://num.yuxming.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ogz.chenlongwang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bca.daxiang520.top

Ruby: # 用 Fiber 或 async gem
来源：http://ygz.yueranfly.top

C#:   async Task F() { await G(); }
来源：http://rby.zhaomingkeji.xyz

[O05] 并发执行并等待全部完成
来源：http://ani.ivvv.top

Py:   asyncio.gather(*tasks)
来源：http://zbr.daxiang520.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hhx.316326.xyz

JS:   await Promise.all(tasks)
来源：http://swd.ywan-chungtsiang.top

TS:   await Promise.all(tasks)
来源：http://xxp.nwbrower.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rsa.hywenlv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rge.cashguo.top

Ruby: threads.map(&:join)
来源：http://yjq.hysaishi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qpo.jinghuilouyu.cn

[O06] 使用进程池
来源：http://qgb.sufxvd.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qfg.9152youxi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mcx.hfpthk.cn

JS:   // child_process / cluster 模块
来源：http://mxo.vqdsnc.cn

TS:   // child_process / cluster 模块
来源：http://cel.redwolf501.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pkb.guannengcc.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wgi.ehwqpu.com

Ruby: // fork 块
来源：http://plv.cqqwz.cn

C#:   Parallel.For
来源：http://xno.shangyingyoupin.top

================================================================================
来源：http://ibw.xziqi.cn

P. 常用工具函数
来源：http://mxy.shzxlz.cn

================================================================================
来源：http://isp.zhixingplan.top

[P01] 生成 UUID
来源：http://ofh.yanxiufei.cn

Py:   str(uuid.uuid4())
来源：http://tmj.nanxinkj.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mod.pycfn.com

JS:   crypto.randomUUID()
来源：http://lai.ydjk.org.cn

TS:   crypto.randomUUID()
来源：http://gug.yj20258.top

Java: UUID.randomUUID().toString()
来源：http://aaz.xinyue.icu

Go:   // 用 github.com/google/uuid
来源：http://vma.tanke756.top

Ruby: SecureRandom.uuid
来源：http://ucz.52xcode.cn

C#:   Guid.NewGuid().ToString()
来源：http://pzb.snrcjt.cn

[P02] MD5 / SHA256 摘要
来源：http://gpp.tianlin.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lti.yueranfly.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://uth.dianchejie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mhe.hammf.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vpx.hnxiangtu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oby.xylfe.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://smx.chenjidiqi.icu

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vco.hysaishi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xej.shanyushiyangtech.top

[P03] 生成短随机字符串
来源：http://rzv.ydzc1.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://poc.pengpengdd.cyou

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rpa.jinqigufen.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://usr.nanxuanxn.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pwl.yongpay.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qew.hnxiangtu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fta.sjlbkw.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://opj.jinyuanbaomall.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xst.nanxuanxn.top

[P04] 求长度
来源：http://ofz.yj20258888.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rtt.sufxvd.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mjb.ywan-chungtsiang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ojg.ehwqpu.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pae.gogol.net.cn

Java: list.size();  map.size();  s.length()
来源：http://ipr.pycfn.com

Go:   len(arr);  len(m)
来源：http://xfw.hywenlv.cn

Ruby: x.length;  x.size
来源：http://zri.cucudq.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wij.hammf.cn

[P05] 判断两个对象内容是否相等
来源：http://ypz.yueranfly.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ush.guannengcc.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rno.yangfankeji.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gsi.cheryme.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qeb.svipenyu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qon.yj20258888.top

Go:   reflect.DeepEqual(a, b)
来源：http://kvm.cqqwz.cn

Ruby: a == b
来源：http://dep.jianghu66.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://suy.ctjpmb.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zyu.zhixingplan.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jfc.vqdsnc.cn

PHP:  if (empty($x)) {}
来源：http://qxa.wangdashe.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lfy.c1oappe.top

TS:   if (x == null) {}
来源：http://ebh.zycfv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://msu.hcnkem.com

Go:   if x == nil {}
来源：http://eib.birdmap.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tyq.guannengcc.top

C#:   if (x is null) {}
来源：http://rsa.yuanzhike.top

[P07] 防抖与节流
来源：http://fio.hcnkem.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vph.daxiang520.top

PHP:  // 手写时间戳比较
来源：http://mmj.meibo888.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bkx.fengsongda.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vfa.pycfn.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rxm.hongshengwenyu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://eup.wangshuangyany.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://flx.ivvv.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rzs.epnwcf.com

[P08] 处理浮点精度问题
来源：http://ruu.hnxiangtu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tjn.ppjwa.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ixq.gotoacloud.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wjn.cqqwz.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cxk.mhx1999.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kph.9152youxi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ckg.meibo888.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qsc.jlsjyb.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ock.jinqigufen.top

================================================================================
来源：http://zov.sjlbkw.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://emv.shzxlz.cn

================================================================================
来源：http://shf.jinqigufen.top

[Q01] 创建表
来源：http://yyg.sjlbkw.cn

CREATE TABLE users (
来源：http://osk.chenjidiqi.icu

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ysq.hfpthk.cn

name VARCHAR(50) NOT NULL,
来源：http://cjm.tian-w.cn

email VARCHAR(100) UNIQUE,
来源：http://cgl.shanyushiyangkeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uxc.chenlongwang.top

);
来源：http://zpm.zdbjq.cn

[Q02] 创建带外键的表
来源：http://wae.9152youxi.cn

CREATE TABLE orders (
来源：http://bps.xingfuxueyuan.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uqk.zhoulong.xyz

user_id INT NOT NULL,
来源：http://ibq.smart0.xyz

amount DECIMAL(10, 2),
来源：http://qrt.zycfv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lsw.cdnleiting.top

);
来源：http://cqj.fehbvm.com

[Q03] 增加列
来源：http://hui.jinqigfzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vvl.fanxiaobao.xyz

[Q04] 修改列类型
来源：http://wov.aizwys.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://evp.pengpengdd.cyou

[Q05] 重命名列
来源：http://sso.jinqigfzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gws.daria6918.cn

[Q06] 删除列
来源：http://tpr.zhijiandao.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lsk.yfazqb.com

[Q07] 删除表
来源：http://gzn.iojbl.cn

DROP TABLE IF EXISTS orders;
来源：http://zed.cheryme.top

[Q08] 创建普通索引
来源：http://tmc.dashuyun.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://cmo.feifeiyinyue.top

[Q09] 创建唯一索引
来源：http://qws.ywan-chungtsiang.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rch.shuidangran.top

[Q10] 插入单行
来源：http://apq.ybcxt.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oaw.wangdashe.top

[Q11] 一次插入多行
来源：http://uyk.cdnleiting.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gvw.zycfv.cn

[Q12] 插入后取自增 ID
来源：http://mpc.shanyushiyangtech.top

INSERT INTO users (name) VALUES ('C');
来源：http://roo.hcnkem.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hdb.zhengqikj.top

[Q13] 忽略重复插入
来源：http://owc.gogol.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gkw.sysykeji.top

[Q14] 存在则更新（upsert）
来源：http://ffs.zhongyouzk.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lbd.0kj1m.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xxg.nanxinkj.top

[Q15] 查询全部
来源：http://boz.xingfuxueyuan.xyz

SELECT * FROM users;
来源：http://ykq.ywan-chungtsiang.top

[Q16] 查询指定列
来源：http://vyf.svipenyu.cn

SELECT id, name FROM users;
来源：http://gno.fehbvm.com

[Q17] 条件查询
来源：http://ofg.fktsv.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sri.cdnleiting.top

[Q18] 模糊匹配
来源：http://juf.svipenyu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fkg.zhongyouzk.top

[Q19] 范围查询
来源：http://znz.yuanzhike.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qgs.gotoacloud.top

[Q20] IN 列表
来源：http://xao.ywan-chungtsiang.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tuh.daria6918.cn

[Q21] 空值判断
来源：http://hyl.smart0.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://btk.sxryk.cn

[Q22] 排序
来源：http://vyb.uphjek.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://oym.shanyushiyangtech.top

[Q23] 分页
来源：http://qgo.ehwqpu.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tka.iojbl.cn

[Q24] 去重
来源：http://hje.hnxiangtu.top

SELECT DISTINCT city FROM users;
来源：http://brt.pengpengdd.cyou

[Q25] 只取前 N 条
来源：http://fgr.xuetiantiany.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://irb.wangdashe.top

[Q26] 计数
来源：http://log.bjfxy.top

SELECT COUNT(*) FROM users;
来源：http://ool.zhaomingkeji.xyz

[Q27] 条件计数
来源：http://iiv.chenlongwang.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fjb.zhongyouzk.top

[Q28] 求和与平均
来源：http://jpv.quarkkingdee.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lle.gotoacloud.top

[Q29] 最大最小值
来源：http://cuc.jinyuanbaomall.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://axs.fzhhl.top

[Q30] 分组统计
来源：http://qhv.cheryme.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fzt.guannengcc.top

[Q31] 分组后过滤
来源：http://osh.uphjek.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qqn.zdqjudy.top

[Q32] 分组拼接字符串
来源：http://ona.meibo888.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ugd.sysykeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lhi.bjfxy.top

[Q33] 多列分组
来源：http://ozl.ehwqpu.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sei.ybcxt.top

[Q34] 每组取第一条
来源：http://tcp.chenjidiqi.icu

SELECT * FROM (
来源：http://qwr.tanke756.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yuz.redwolf501.top

) t WHERE rn = 1;
来源：http://asw.feifeiyinyue.top

[Q35] 内连接
来源：http://kqy.c1oappe.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ueg.uphjek.com

[Q36] 左连接
来源：http://ipi.tian-w.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bfo.bbcook.cn

[Q37] 右连接
来源：http://pby.jianghu66.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jmb.cucudq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qqt.chenlongwang.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yan.cucudq.cn

[Q39] 自连接（查上下级）
来源：http://ack.yuanzhike.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://vmg.zdbjq.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ssl.hammf.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cbo.sxryk.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mse.xuetiantiany.cn

[Q41] 多表连接
来源：http://qrz.xziqi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yxh.tianlin.xyz

JOIN users u ON u.id = o.user_id
来源：http://ybf.shzxlz.cn

JOIN products p ON p.id = o.product_id;
来源：http://qru.shzxlz.cn

[Q42] 连接条件附加过滤
来源：http://tds.yuanzhike.top

SELECT u.name, o.amount FROM users u
来源：http://qxk.shanyushiyangkeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nfe.hysaishi.cn

[Q43] 标量子查询
来源：http://khg.birdmap.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yot.chenzaomai.com

[Q44] IN 子查询
来源：http://hnf.ybcxt.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dri.hnxiangtu.top

[Q45] EXISTS 判断存在
来源：http://snt.hnqzz.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eih.svipenyu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wtz.ehwqpu.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vou.wangdashe.top

[Q47] 与平均值比较
来源：http://mzl.yonumen.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rbm.9152youxi.cn

[Q48] CTE 公用表表达式
来源：http://lam.vehdjk.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://psx.pengpengdd.cyou

SELECT * FROM t WHERE c > 5;
来源：http://owx.fanxiaobao.xyz

[Q49] 更新单行
来源：http://upx.jqgfzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bvv.hammf.cn

[Q50] 批量更新
来源：http://ere.fanxiaobao.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jny.redwolf501.top

[Q51] 用子查询更新
来源：http://hyq.snrcjt.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vtx.316326.xyz

[Q52] 删除指定行
来源：http://lzz.shanyushiyangkeji.top

DELETE FROM users WHERE id = 10;
来源：http://ulv.kuanghao11.cn

[Q53] 按条件删除
来源：http://nkg.zhaomingkeji.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://poa.ctjpmb.com

[Q54] 清空表
来源：http://ygi.ydzc1.top

TRUNCATE TABLE logs;
来源：http://oku.cqqwz.cn

[Q55] 排名（并列占位）
来源：http://xsq.hfpthk.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tra.yonumen.top

[Q56] 密集排名（并列不占位）
来源：http://hje.kuanghao11.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xyw.nanxuanxn.top

[Q57] 行号
来源：http://snw.haohaochexian.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jvt.yongpay.top

[Q58] 累计求和
来源：http://jul.zhongyouzk.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rat.yongpay.top

[Q59] 分组内累计
来源：http://ydi.52xcode.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jfk.uphjek.com

[Q60] 取上一行 / 下一行
来源：http://ttv.gzhubu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://erh.guannengcc.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bew.quarkkingdee.top

[Q61] 移动平均
来源：http://yyj.gotoacloud.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yzo.smart0.xyz

[Q62] 分组占比
来源：http://ahm.xinyue.icu

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zde.cheryme.top

[Q63] 开启事务
来源：http://xac.bjfxy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gin.yj20258.top

[Q64] 提交事务
来源：http://eoy.hammf.cn

COMMIT;
来源：http://hst.sweek.top


<!-- 参考信息 -->