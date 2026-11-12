代发 wailian999

Go:   // 手写递归
来源：http://cqq.meibo888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vyw.wangdashe.top

C#:   // 手写递归
来源：http://wuo.0kj1m.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jkl.jinyuanbaomall.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gcq.kuanghao11.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gby.guowangkeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xrf.tarul.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dju.yj20258888.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iuu.svipenyu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dks.jqgfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wia.cqqwz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oeh.nanxuanxn.top

================================================================================
来源：http://qim.hongshengwenyu.top

O. 并发与异步
来源：http://vtz.yfazqb.com

================================================================================
来源：http://lry.fanxiaobao.xyz

[O01] 启动一个线程
来源：http://zym.redwolf501.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yxz.uphjek.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mpj.quarkkingdee.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mjv.cheryme.top

TS:   // 同 JS
来源：http://jid.yueranfly.top

Java: new Thread(() -> f()).start()
来源：http://lmg.hammf.cn

Go:   go f()
来源：http://tgz.bjfxy.top

Ruby: Thread.new { f }
来源：http://rgf.zhijiandao.cn

C#:   Task.Run(() => F());
来源：http://feq.cucudq.cn

[O02] 使用线程池
来源：http://umb.yonumen.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tji.bjfxy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nke.havefunace.top

JS:   // worker_threads 线程池
来源：http://btu.nanxinkj.top

TS:   // worker_threads 线程池
来源：http://qwa.mhx1999.top

Java: Executors.newFixedThreadPool(4)
来源：http://pdg.tian-w.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://amn.yuanzhike.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kxg.zhaomingkeji.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://doy.sxryk.cn

[O03] 加锁保护共享数据
来源：http://wfp.shanyushiyangkeji.top

Py:   with lock: shared += 1
来源：http://hcz.ehwqpu.com

PHP:  // 用 flock() 做文件锁
来源：http://gcf.snrcjt.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uiu.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://nfd.hnxiangtu.top

Java: synchronized (this) { shared++; }
来源：http://nzb.mhx1999.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jlr.yueranfly.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://evj.ydjk.org.cn

C#:   lock (gate) { shared++; }
来源：http://yph.hesvh.cn

[O04] 定义异步函数并等待
来源：http://rll.ppjwa.cn

Py:   async def f():⏎    await g()
来源：http://axm.yfazqb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jvk.fehbvm.com

JS:   async function f() { await g(); }
来源：http://xmj.zhengqikj.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ooq.wangshuangyany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wtd.epnwcf.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bcg.svipenyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lkr.sxryk.cn

C#:   async Task F() { await G(); }
来源：http://jtv.tian-w.cn

[O05] 并发执行并等待全部完成
来源：http://orj.hnxiangtu.top

Py:   asyncio.gather(*tasks)
来源：http://sgq.yangfankeji.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xwe.yongpay.top

JS:   await Promise.all(tasks)
来源：http://xqy.bbcook.cn

TS:   await Promise.all(tasks)
来源：http://pli.zhixingplan.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://akh.sxryk.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nhv.shuidangran.top

Ruby: threads.map(&:join)
来源：http://qon.yj20258888.top

C#:   await Task.WhenAll(t1, t2)
来源：http://pen.redwolf501.top

[O06] 使用进程池
来源：http://ekw.redwolf501.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dlb.cqqwz.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qwt.ehwqpu.com

JS:   // child_process / cluster 模块
来源：http://zzu.yfazqb.com

TS:   // child_process / cluster 模块
来源：http://ocx.zhaomingkeji.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bzn.zhixingplan.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uys.sufxvd.cn

Ruby: // fork 块
来源：http://ihl.guannengcc.top

C#:   Parallel.For
来源：http://xld.tian-w.cn

================================================================================
来源：http://xel.zdqjudy.top

P. 常用工具函数
来源：http://ybc.kuanghao11.cn

================================================================================
来源：http://mls.nanxuanxn.top

[P01] 生成 UUID
来源：http://hax.hcnkem.com

Py:   str(uuid.uuid4())
来源：http://tja.xuanzx.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bct.shangyingyoupin.top

JS:   crypto.randomUUID()
来源：http://ucg.hongshengwenyu.top

TS:   crypto.randomUUID()
来源：http://mhi.daria6918.cn

Java: UUID.randomUUID().toString()
来源：http://llk.zhaomingkeji.xyz

Go:   // 用 github.com/google/uuid
来源：http://smt.jyoumei.cn

Ruby: SecureRandom.uuid
来源：http://ekf.wangshuangyany.cn

C#:   Guid.NewGuid().ToString()
来源：http://grr.jianghu66.top

[P02] MD5 / SHA256 摘要
来源：http://vtp.epnwcf.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://enr.ydjk.org.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kli.yueranfly.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uwq.ywan-chungtsiang.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rnz.tian-w.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cng.hnxiangtu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://szd.fzhhl.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://byj.zycfv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://emq.fktsv.cn

[P03] 生成短随机字符串
来源：http://ehv.xziqi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://een.tarul.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://stf.yonumen.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dra.haohaochexian.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kub.jqgfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://muw.aizwys.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bzy.chenlongwang.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://pzm.dashuyun.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://poq.feifeiyinyue.top

[P04] 求长度
来源：http://zkd.jyoumei.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gff.nwbrower.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://urp.jinqigufen.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qee.chenjidiqi.icu

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lyq.sufxvd.cn

Java: list.size();  map.size();  s.length()
来源：http://dvg.yuxming.cn

Go:   len(arr);  len(m)
来源：http://ezj.ivvv.top

Ruby: x.length;  x.size
来源：http://jvf.fengsongda.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://wim.yongpay.top

[P05] 判断两个对象内容是否相等
来源：http://usx.jyoumei.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qev.wangshuangyany.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dhp.jinghuilouyu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yph.snrcjt.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mws.xziqi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://odn.fzhhl.top

Go:   reflect.DeepEqual(a, b)
来源：http://lgm.sysykeji.top

Ruby: a == b
来源：http://kqa.cdnleiting.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nop.chenlongwang.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rrl.tian-w.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rve.zhongyouzk.top

PHP:  if (empty($x)) {}
来源：http://lsm.havefunace.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jel.hnqzz.top

TS:   if (x == null) {}
来源：http://vts.zhiwuduotai.top

Java: if (x == null || x.isEmpty()) {}
来源：http://cfk.316326.xyz

Go:   if x == nil {}
来源：http://fnf.zhengqikj.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://grk.xziqi.cn

C#:   if (x is null) {}
来源：http://vfu.hywenlv.cn

[P07] 防抖与节流
来源：http://taq.hnqzz.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wae.kuanghao11.cn

PHP:  // 手写时间戳比较
来源：http://zyb.yj20258.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ezv.nanxuanxn.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bdj.yueranfly.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mpq.bbcook.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tvd.gaohongyu789.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://esh.iojbl.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zdi.cucudq.cn

[P08] 处理浮点精度问题
来源：http://hag.ctjpmb.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mjp.chenjidiqi.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lco.shuidangran.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pwv.yongpay.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://khh.tianlin.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sfo.sweek.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dwq.xuanzx.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://eoy.vqdsnc.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vti.sufxvd.cn

================================================================================
来源：http://csv.gotoacloud.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jct.sweek.top

================================================================================
来源：http://wwg.sjlbkw.cn

[Q01] 创建表
来源：http://trh.zhengqikj.top

CREATE TABLE users (
来源：http://ref.quarkkingdee.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bif.zhengqikj.top

name VARCHAR(50) NOT NULL,
来源：http://sku.yanxiufei.cn

email VARCHAR(100) UNIQUE,
来源：http://lwu.uphjek.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oha.jinqigfzy.top

);
来源：http://gtg.tianlin.xyz

[Q02] 创建带外键的表
来源：http://wma.hcnkem.com

CREATE TABLE orders (
来源：http://wcy.ydjk.org.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cll.9152youxi.cn

user_id INT NOT NULL,
来源：http://whi.pengpengdd.cyou

amount DECIMAL(10, 2),
来源：http://tdp.pengpengdd.cyou

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uoc.cucudq.cn

);
来源：http://xkr.c1oappe.top

[Q03] 增加列
来源：http://kra.0kj1m.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wuq.chenlongwang.top

[Q04] 修改列类型
来源：http://cpl.xingfuxueyuan.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wsp.snrcjt.cn

[Q05] 重命名列
来源：http://ssh.nwbrower.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bxg.aizwys.cn

[Q06] 删除列
来源：http://cwa.dashuyun.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sgl.sufxvd.cn

[Q07] 删除表
来源：http://alb.gotoacloud.top

DROP TABLE IF EXISTS orders;
来源：http://gfk.fengsongda.top

[Q08] 创建普通索引
来源：http://dvk.ehwqpu.com

CREATE INDEX idx_users_email ON users(email);
来源：http://qqn.yongpay.top

[Q09] 创建唯一索引
来源：http://tgs.cucudq.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zpv.hongshengwenyu.top

[Q10] 插入单行
来源：http://yuo.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hhz.shuidangran.top

[Q11] 一次插入多行
来源：http://olc.havefunace.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ptr.sufxvd.cn

[Q12] 插入后取自增 ID
来源：http://zxw.feifeiyinyue.top

INSERT INTO users (name) VALUES ('C');
来源：http://skz.yfazqb.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xur.yangfankeji.com

[Q13] 忽略重复插入
来源：http://flb.kuanghao11.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pqf.c1oappe.top

[Q14] 存在则更新（upsert）
来源：http://ltw.zdbjq.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://svd.gotoacloud.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lov.svipenyu.cn

[Q15] 查询全部
来源：http://vqi.fengsongda.top

SELECT * FROM users;
来源：http://gka.hnqzz.top

[Q16] 查询指定列
来源：http://uie.smart0.xyz

SELECT id, name FROM users;
来源：http://jch.daria6918.cn

[Q17] 条件查询
来源：http://klk.xziqi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://git.fehbvm.com

[Q18] 模糊匹配
来源：http://zpb.gotoacloud.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hhp.jinqigufen.top

[Q19] 范围查询
来源：http://jhs.cashguo.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rtp.havefunace.top

[Q20] IN 列表
来源：http://fsm.zdbjq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yen.sjlbkw.cn

[Q21] 空值判断
来源：http://pcv.nanxinkj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://lrf.mhx1999.top

[Q22] 排序
来源：http://ezz.hnqzz.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lid.hcnkem.com

[Q23] 分页
来源：http://imh.hcnkem.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mid.meibo888.top

[Q24] 去重
来源：http://otm.hnxiangtu.top

SELECT DISTINCT city FROM users;
来源：http://ndo.gogol.net.cn

[Q25] 只取前 N 条
来源：http://vqj.shanyushiyangkeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vgl.cdnleiting.top

[Q26] 计数
来源：http://xap.cdnleiting.top

SELECT COUNT(*) FROM users;
来源：http://pqv.c1oappe.top

[Q27] 条件计数
来源：http://gso.fengsongda.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dys.kuanghao11.cn

[Q28] 求和与平均
来源：http://ztn.ydzc1.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xrl.tarul.cn

[Q29] 最大最小值
来源：http://jnk.jianghu66.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://aok.sufxvd.cn

[Q30] 分组统计
来源：http://yuo.xingfuxueyuan.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zks.zhoulong.xyz

[Q31] 分组后过滤
来源：http://xzy.hysaishi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pwb.tanke756.top

[Q32] 分组拼接字符串
来源：http://xbf.jinqigfzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://slm.wangshuangyany.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://spo.tian-w.cn

[Q33] 多列分组
来源：http://llp.yueranfly.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vhj.xuanzx.com

[Q34] 每组取第一条
来源：http://pkg.sysykeji.top

SELECT * FROM (
来源：http://nit.316326.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kjo.bbcook.cn

) t WHERE rn = 1;
来源：http://ukr.guannengcc.top

[Q35] 内连接
来源：http://wgz.hesvh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jlb.cqqwz.cn

[Q36] 左连接
来源：http://jbr.hesvh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nke.svipenyu.cn

[Q37] 右连接
来源：http://tqc.jyoumei.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lfm.sxryk.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mbl.hnxiangtu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gny.zhoulong.xyz

[Q39] 自连接（查上下级）
来源：http://yat.ehwqpu.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://hpc.yuanzhike.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jso.cashguo.top

[Q40] 交叉连接（笛卡尔积）
来源：http://krc.havefunace.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://npv.zycfv.cn

[Q41] 多表连接
来源：http://vpo.xylfe.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gav.guowangkeji.top

JOIN users u ON u.id = o.user_id
来源：http://uet.yvedp.cn

JOIN products p ON p.id = o.product_id;
来源：http://xdl.wangshuangyany.cn

[Q42] 连接条件附加过滤
来源：http://jcv.cheryme.top

SELECT u.name, o.amount FROM users u
来源：http://qzf.hysaishi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yif.andypj.xyz

[Q43] 标量子查询
来源：http://tja.gzhubu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ver.tian-w.cn

[Q44] IN 子查询
来源：http://ocp.guowangkeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://eip.kuanghao11.cn

[Q45] EXISTS 判断存在
来源：http://gjc.xuanzx.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sqn.yj20258.top

[Q46] NOT EXISTS 判断不存在
来源：http://jsk.xuetiantiany.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nks.ybcxt.top

[Q47] 与平均值比较
来源：http://uex.fehbvm.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kme.mhx1999.top

[Q48] CTE 公用表表达式
来源：http://rwi.jianghu66.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nfm.yonumen.top

SELECT * FROM t WHERE c > 5;
来源：http://nyb.ivvv.top

[Q49] 更新单行
来源：http://fpx.sysykeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vub.ivvv.top

[Q50] 批量更新
来源：http://zjp.vqdsnc.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://alu.cashguo.top

[Q51] 用子查询更新
来源：http://ilp.shuidangran.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wpm.gzhubu.top

[Q52] 删除指定行
来源：http://zxv.gotoacloud.top

DELETE FROM users WHERE id = 10;
来源：http://nsj.zhongyouzk.top

[Q53] 按条件删除
来源：http://qsk.xingfuxueyuan.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yln.xuanzx.com

[Q54] 清空表
来源：http://mlt.guowangkeji.top

TRUNCATE TABLE logs;
来源：http://ozv.jqgfzy.top

[Q55] 排名（并列占位）
来源：http://lbu.jinqigfzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ghj.dashuyun.cn

[Q56] 密集排名（并列不占位）
来源：http://glf.jinghuilouyu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qeg.tianlin.xyz

[Q57] 行号
来源：http://oxh.wangdashe.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jmm.uphjek.com

[Q58] 累计求和
来源：http://vlo.yj20258888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nwa.hammf.cn

[Q59] 分组内累计
来源：http://apj.shanyushiyangkeji.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uxw.aibaodan.cn

[Q60] 取上一行 / 下一行
来源：http://fbf.cdnleiting.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://owv.hongshengwenyu.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pcc.gaohongyu789.top

[Q61] 移动平均
来源：http://nxt.bjfxy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ggo.zhijiandao.cn

[Q62] 分组占比
来源：http://pkd.nanxuanxn.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lwq.nanxuanxn.top

[Q63] 开启事务
来源：http://uvv.gaohongyu789.top

START TRANSACTION;                -- 或 BEGIN
来源：http://aqr.wangshuangyany.cn

[Q64] 提交事务
来源：http://roh.zhaomingkeji.xyz

COMMIT;
来源：http://rnp.birdmap.top

[Q65] 回滚事务
来源：http://gzc.sysykeji.top

ROLLBACK;
来源：http://ace.cashguo.top

[Q66] 行锁查询
来源：http://asq.birdmap.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gso.xuetiantiany.cn


<!-- 参考信息 -->