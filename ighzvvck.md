代发 wailian999

PHP:  // 手写递归函数
来源：http://kbf.aibaodan.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dsi.bjfxy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://awd.pycfn.com

Java: // 手写递归
来源：http://wmw.jianghu66.top

Go:   // 手写递归
来源：http://rlu.zycfv.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nhv.sxryk.cn

C#:   // 手写递归
来源：http://lft.mhx1999.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pua.yvedp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sok.pycfn.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xgt.9152youxi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vbp.jyoumei.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dgr.fanxiaobao.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dxs.gotoacloud.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fqp.hammf.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jfv.cqqwz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tbp.aibaodan.cn

================================================================================
来源：http://xcj.ctjpmb.com

O. 并发与异步
来源：http://tgj.tanke756.top

================================================================================
来源：http://ulw.gotoacloud.top

[O01] 启动一个线程
来源：http://wyi.jinqigufen.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wyo.chenjidiqi.icu

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://txp.jqgfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rlx.nanxuanxn.top

TS:   // 同 JS
来源：http://zbt.yj202588.top

Java: new Thread(() -> f()).start()
来源：http://gar.cashguo.top

Go:   go f()
来源：http://llc.dianchejie.cn

Ruby: Thread.new { f }
来源：http://zjc.fzhhl.top

C#:   Task.Run(() => F());
来源：http://jpv.wangdashe.top

[O02] 使用线程池
来源：http://hbq.meibo888.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://epe.jinghuilouyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qip.hysaishi.cn

JS:   // worker_threads 线程池
来源：http://ngp.yanxiufei.cn

TS:   // worker_threads 线程池
来源：http://czt.sufxvd.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fvj.redwolf501.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jum.chenjidiqi.icu

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wzv.ppjwa.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pae.sxryk.cn

[O03] 加锁保护共享数据
来源：http://rte.pycfn.com

Py:   with lock: shared += 1
来源：http://loz.gotoacloud.top

PHP:  // 用 flock() 做文件锁
来源：http://erw.316326.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pau.epnwcf.com

TS:   // 同 JS
来源：http://ynf.tian-w.cn

Java: synchronized (this) { shared++; }
来源：http://nna.jinqigufen.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kou.316326.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://emo.yfazqb.com

C#:   lock (gate) { shared++; }
来源：http://jvi.daria6918.cn

[O04] 定义异步函数并等待
来源：http://iog.fktsv.cn

Py:   async def f():⏎    await g()
来源：http://xgb.chenzaomai.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bkg.gaohongyu789.top

JS:   async function f() { await g(); }
来源：http://oqa.hesvh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://njj.ehwqpu.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zgz.shanyushiyangkeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bnc.yanxiufei.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cdb.jinyuanbaomall.cn

C#:   async Task F() { await G(); }
来源：http://scb.aizwys.cn

[O05] 并发执行并等待全部完成
来源：http://rel.jlsjyb.cn

Py:   asyncio.gather(*tasks)
来源：http://qbo.pycfn.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bid.c1oappe.top

JS:   await Promise.all(tasks)
来源：http://jmj.cqqwz.cn

TS:   await Promise.all(tasks)
来源：http://hem.ivvv.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ndn.yueranfly.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kxe.xuetiantiany.cn

Ruby: threads.map(&:join)
来源：http://vlf.ctjpmb.com

C#:   await Task.WhenAll(t1, t2)
来源：http://emf.dianchejie.cn

[O06] 使用进程池
来源：http://xrr.chenlongwang.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rlx.nanxinkj.top

PHP:  // pcntl_fork 或多进程队列
来源：http://mkl.shzxlz.cn

JS:   // child_process / cluster 模块
来源：http://mol.c1oappe.top

TS:   // child_process / cluster 模块
来源：http://rsc.xingfuxueyuan.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://iak.chenzaomai.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gml.feifeiyinyue.top

Ruby: // fork 块
来源：http://jsw.meibo888.top

C#:   Parallel.For
来源：http://bbi.jqgufenzy.top

================================================================================
来源：http://gzh.hnxiangtu.top

P. 常用工具函数
来源：http://atg.hnqzz.top

================================================================================
来源：http://irm.wangdashe.top

[P01] 生成 UUID
来源：http://rxi.ehwqpu.com

Py:   str(uuid.uuid4())
来源：http://yim.gogol.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://azn.jianghu66.top

JS:   crypto.randomUUID()
来源：http://cza.shzxlz.cn

TS:   crypto.randomUUID()
来源：http://evq.aizwys.cn

Java: UUID.randomUUID().toString()
来源：http://jyy.zhongyouzk.top

Go:   // 用 github.com/google/uuid
来源：http://mwj.fehbvm.com

Ruby: SecureRandom.uuid
来源：http://wmu.hywenlv.cn

C#:   Guid.NewGuid().ToString()
来源：http://exe.shzxlz.cn

[P02] MD5 / SHA256 摘要
来源：http://jjq.yueranfly.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kpc.snrcjt.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://oon.svipenyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yxa.yj20258888.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wrn.c1oappe.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jws.cheryme.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://umr.tian-w.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yxt.aizwys.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xtt.guowangkeji.top

[P03] 生成短随机字符串
来源：http://oxw.fengsongda.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://obb.yvedp.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fcn.cqqwz.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hss.birdmap.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bkb.yanxiufei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rqg.0kj1m.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://byl.yanxiufei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mfh.zdqjudy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dui.xziqi.cn

[P04] 求长度
来源：http://fqg.jyoumei.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ciz.epnwcf.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://quh.hongshengwenyu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lmg.nanxuanxn.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cnl.316326.xyz

Java: list.size();  map.size();  s.length()
来源：http://eze.yonumen.top

Go:   len(arr);  len(m)
来源：http://inw.c1oappe.top

Ruby: x.length;  x.size
来源：http://gjl.jlsjyb.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bka.sufxvd.cn

[P05] 判断两个对象内容是否相等
来源：http://slu.ivvv.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://seo.chenlongwang.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://egh.hnqzz.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lfg.jqgufenzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ejx.ehwqpu.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ili.haohaochexian.top

Go:   reflect.DeepEqual(a, b)
来源：http://bmj.vehdjk.com

Ruby: a == b
来源：http://och.yanxiufei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jwf.vehdjk.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tkg.gogol.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sjk.vqdsnc.cn

PHP:  if (empty($x)) {}
来源：http://mty.meibo888.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uid.uphjek.com

TS:   if (x == null) {}
来源：http://hpz.yonumen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://xbh.daria6918.cn

Go:   if x == nil {}
来源：http://lyo.jlsjyb.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gal.zhijiandao.cn

C#:   if (x is null) {}
来源：http://mxc.zhijiandao.cn

[P07] 防抖与节流
来源：http://nuo.mhx1999.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nek.cqqwz.cn

PHP:  // 手写时间戳比较
来源：http://hog.aibaodan.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mry.dianchejie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wyq.vehdjk.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://per.yongpay.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ewi.mhx1999.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ulz.sufxvd.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cmj.gogol.net.cn

[P08] 处理浮点精度问题
来源：http://jbd.yj20258888.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mwh.fanxiaobao.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://evj.nanxinkj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wxp.aibaodan.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sru.sysykeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dur.nwbrower.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://soq.fktsv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nqy.yuanzhike.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wlt.sjlbkw.cn

================================================================================
来源：http://dfw.jianghu66.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bmu.ydzc1.top

================================================================================
来源：http://hik.mhx1999.top

[Q01] 创建表
来源：http://soj.zdqjudy.top

CREATE TABLE users (
来源：http://jmb.hcnkem.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sjg.xylfe.cn

name VARCHAR(50) NOT NULL,
来源：http://bph.gogol.net.cn

email VARCHAR(100) UNIQUE,
来源：http://rdv.316326.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://suy.haohaochexian.top

);
来源：http://ijc.yueranfly.top

[Q02] 创建带外键的表
来源：http://vms.bbcook.cn

CREATE TABLE orders (
来源：http://rht.hesvh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sye.52xcode.cn

user_id INT NOT NULL,
来源：http://fcd.cashguo.top

amount DECIMAL(10, 2),
来源：http://myu.daxiang520.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yep.chenzaomai.com

);
来源：http://xhr.havefunace.top

[Q03] 增加列
来源：http://zmw.nanxuanxn.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wvc.wangdashe.top

[Q04] 修改列类型
来源：http://nqz.fanxiaobao.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pku.hnqzz.top

[Q05] 重命名列
来源：http://ugv.zdbjq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kag.shuidangran.top

[Q06] 删除列
来源：http://xrt.fktsv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rjm.chenjidiqi.icu

[Q07] 删除表
来源：http://gii.feifeiyinyue.top

DROP TABLE IF EXISTS orders;
来源：http://dsc.cqqwz.cn

[Q08] 创建普通索引
来源：http://uji.fengsongda.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jnl.tian-w.cn

[Q09] 创建唯一索引
来源：http://nbf.hnqzz.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pcz.fanxiaobao.xyz

[Q10] 插入单行
来源：http://ytp.bbcook.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lyw.jqgufenzy.top

[Q11] 一次插入多行
来源：http://idq.hcnkem.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ual.jyoumei.cn

[Q12] 插入后取自增 ID
来源：http://svj.sxryk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gzo.sweek.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rls.xuetiantiany.cn

[Q13] 忽略重复插入
来源：http://fvg.xingfuxueyuan.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bdn.ivvv.top

[Q14] 存在则更新（upsert）
来源：http://uum.0kj1m.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jam.aizwys.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://okv.xingfuxueyuan.xyz

[Q15] 查询全部
来源：http://ktm.zhongyouzk.top

SELECT * FROM users;
来源：http://nzh.cashguo.top

[Q16] 查询指定列
来源：http://pta.jianghu66.top

SELECT id, name FROM users;
来源：http://qlk.shanyushiyangkeji.top

[Q17] 条件查询
来源：http://zph.xziqi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vyb.nwbrower.top

[Q18] 模糊匹配
来源：http://eoc.fehbvm.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pxc.ivvv.top

[Q19] 范围查询
来源：http://czt.jinyuanbaomall.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://slb.kuanghao11.cn

[Q20] IN 列表
来源：http://xmo.jianghu66.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wmr.xuetiantiany.cn

[Q21] 空值判断
来源：http://edj.meibo888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://lgk.316326.xyz

[Q22] 排序
来源：http://bdz.sxryk.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://csq.9152youxi.cn

[Q23] 分页
来源：http://dop.yongpay.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kme.zhixingplan.top

[Q24] 去重
来源：http://kcf.cashguo.top

SELECT DISTINCT city FROM users;
来源：http://feb.uphjek.com

[Q25] 只取前 N 条
来源：http://iui.0kj1m.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qxf.wangshuangyany.cn

[Q26] 计数
来源：http://ucu.nwbrower.top

SELECT COUNT(*) FROM users;
来源：http://fou.zhoulong.xyz

[Q27] 条件计数
来源：http://zfz.yj20258.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vln.ctjpmb.com

[Q28] 求和与平均
来源：http://wqq.zycfv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vlv.yonumen.top

[Q29] 最大最小值
来源：http://yxx.jinyuanbaomall.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xzn.yuxming.cn

[Q30] 分组统计
来源：http://ldm.aizwys.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lim.shanyushiyangtech.top

[Q31] 分组后过滤
来源：http://qow.jiagoushi.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://oqd.birdmap.top

[Q32] 分组拼接字符串
来源：http://ddo.chenjidiqi.icu

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uow.aizwys.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mlb.zhiwuduotai.top

[Q33] 多列分组
来源：http://nvi.yj202588.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hmm.iojbl.cn

[Q34] 每组取第一条
来源：http://ztg.yj20258888.top

SELECT * FROM (
来源：http://ift.dianchejie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kuw.fanxiaobao.xyz

) t WHERE rn = 1;
来源：http://clk.quarkkingdee.top

[Q35] 内连接
来源：http://oax.redwolf501.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gbc.quarkkingdee.top

[Q36] 左连接
来源：http://lzo.shzxlz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fdj.yvedp.cn

[Q37] 右连接
来源：http://byt.xylfe.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xon.zhongyouzk.top

[Q38] 全外连接（PostgreSQL）
来源：http://uiy.smart0.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dgy.guannengcc.top

[Q39] 自连接（查上下级）
来源：http://ker.gaohongyu789.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ehj.jinqigfzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zzf.feifeiyinyue.top

[Q40] 交叉连接（笛卡尔积）
来源：http://pns.yj20258.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qzc.0kj1m.cn

[Q41] 多表连接
来源：http://bdk.hywenlv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uri.kuanghao11.cn

JOIN users u ON u.id = o.user_id
来源：http://jwo.uphjek.com

JOIN products p ON p.id = o.product_id;
来源：http://rxm.hysaishi.cn

[Q42] 连接条件附加过滤
来源：http://irv.c1oappe.top

SELECT u.name, o.amount FROM users u
来源：http://hdy.hesvh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fgl.fzhhl.top

[Q43] 标量子查询
来源：http://wcf.tanke756.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nrf.zhoulong.xyz

[Q44] IN 子查询
来源：http://cjy.yvedp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qvq.tarul.cn

[Q45] EXISTS 判断存在
来源：http://kcv.316326.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uwc.yuxming.cn

[Q46] NOT EXISTS 判断不存在
来源：http://bpk.zhengqikj.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vcw.bbcook.cn

[Q47] 与平均值比较
来源：http://xsp.dianchejie.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qdu.hysaishi.cn

[Q48] CTE 公用表表达式
来源：http://kvj.hnqzz.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://drs.jlsjyb.cn

SELECT * FROM t WHERE c > 5;
来源：http://ibv.guowangkeji.top

[Q49] 更新单行
来源：http://evs.wangdashe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://otk.zhaomingkeji.xyz

[Q50] 批量更新
来源：http://bps.aibaodan.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://omb.xingfuxueyuan.xyz

[Q51] 用子查询更新
来源：http://muh.zdqjudy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zbd.yanxiufei.cn

[Q52] 删除指定行
来源：http://dqi.ybcxt.top

DELETE FROM users WHERE id = 10;
来源：http://dbo.yj202588.top

[Q53] 按条件删除
来源：http://nyv.guowangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yoi.cucudq.cn

[Q54] 清空表
来源：http://qdo.cucudq.cn

TRUNCATE TABLE logs;
来源：http://hsa.xuanzx.com

[Q55] 排名（并列占位）
来源：http://cka.yvedp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dxd.cdnleiting.top

[Q56] 密集排名（并列不占位）
来源：http://juv.fanxiaobao.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://myy.shanyushiyangtech.top

[Q57] 行号
来源：http://koh.hesvh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ryy.xingfuxueyuan.xyz

[Q58] 累计求和
来源：http://zwv.fehbvm.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fot.jinqigufen.top

[Q59] 分组内累计
来源：http://ctp.yj20258.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qcv.andypj.xyz

[Q60] 取上一行 / 下一行
来源：http://moh.dianchejie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ipd.vehdjk.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vmw.tanke756.top

[Q61] 移动平均
来源：http://ouo.hongshengwenyu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lxm.gotoacloud.top

[Q62] 分组占比
来源：http://flp.yanxiufei.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yoi.yonumen.top

[Q63] 开启事务
来源：http://iod.shzxlz.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://cyk.aizwys.cn

[Q64] 提交事务
来源：http://jdj.snrcjt.cn

COMMIT;
来源：http://kka.quarkkingdee.top


<!-- 参考信息 -->