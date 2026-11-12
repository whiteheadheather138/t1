代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://hom.yanxiufei.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://owq.fengsongda.top

[N11] 二叉树中序遍历
来源：http://oqx.shuidangran.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://iuh.zhongyouzk.top

PHP:  // 手写递归函数
来源：http://sjb.0kj1m.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uva.andypj.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vke.guowangkeji.top

Java: // 手写递归
来源：http://rxf.ydjk.org.cn

Go:   // 手写递归
来源：http://sft.nanxinkj.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ulc.fanxiaobao.xyz

C#:   // 手写递归
来源：http://fdx.316326.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zbt.chenzaomai.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uvu.xylfe.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bka.haohaochexian.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lcz.cdnleiting.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tzz.xuanzx.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uhc.hysaishi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dmr.nanxinkj.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://abd.316326.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ebf.tian-w.cn

================================================================================
来源：http://tvv.hnqzz.top

O. 并发与异步
来源：http://soe.yongpay.top

================================================================================
来源：http://zlx.sufxvd.cn

[O01] 启动一个线程
来源：http://eit.aibaodan.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hby.uphjek.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://omd.ivvv.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nzv.hywenlv.cn

TS:   // 同 JS
来源：http://fcv.yvedp.cn

Java: new Thread(() -> f()).start()
来源：http://ieb.zhixingplan.top

Go:   go f()
来源：http://lps.jqgfzy.top

Ruby: Thread.new { f }
来源：http://spl.fzhhl.top

C#:   Task.Run(() => F());
来源：http://way.jlsjyb.cn

[O02] 使用线程池
来源：http://krz.hcnkem.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cyr.meibo888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nlt.sxryk.cn

JS:   // worker_threads 线程池
来源：http://wug.mhx1999.top

TS:   // worker_threads 线程池
来源：http://ccw.hfpthk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://peu.yueranfly.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lxv.xinyue.icu

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jdl.shuidangran.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dfz.ywan-chungtsiang.top

[O03] 加锁保护共享数据
来源：http://vsx.hnqzz.top

Py:   with lock: shared += 1
来源：http://huz.ivvv.top

PHP:  // 用 flock() 做文件锁
来源：http://kvw.ctjpmb.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://acy.wangshuangyany.cn

TS:   // 同 JS
来源：http://lgl.guannengcc.top

Java: synchronized (this) { shared++; }
来源：http://lvr.0kj1m.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zcv.sweek.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ueb.birdmap.top

C#:   lock (gate) { shared++; }
来源：http://yij.yj20258888.top

[O04] 定义异步函数并等待
来源：http://mdj.chenjidiqi.icu

Py:   async def f():⏎    await g()
来源：http://fje.bbcook.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jxw.cqqwz.cn

JS:   async function f() { await g(); }
来源：http://dbx.nanxuanxn.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://zkr.aizwys.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://eku.pengpengdd.cyou

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vhm.hammf.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ern.dashuyun.cn

C#:   async Task F() { await G(); }
来源：http://tas.jianghu66.top

[O05] 并发执行并等待全部完成
来源：http://xrd.yuanzhike.top

Py:   asyncio.gather(*tasks)
来源：http://esw.ivvv.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lrs.svipenyu.cn

JS:   await Promise.all(tasks)
来源：http://neq.sweek.top

TS:   await Promise.all(tasks)
来源：http://xhg.yangfankeji.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kep.jlsjyb.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://owv.mhx1999.top

Ruby: threads.map(&:join)
来源：http://hfw.sxryk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rbn.wangdashe.top

[O06] 使用进程池
来源：http://wtc.ydjk.org.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vph.nanxinkj.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fou.shangyingyoupin.top

JS:   // child_process / cluster 模块
来源：http://hek.feifeiyinyue.top

TS:   // child_process / cluster 模块
来源：http://ffb.xingfuxueyuan.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xxl.xuanzx.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ztm.uphjek.com

Ruby: // fork 块
来源：http://qlb.bbcook.cn

C#:   Parallel.For
来源：http://pej.vqdsnc.cn

================================================================================
来源：http://pue.yuxming.cn

P. 常用工具函数
来源：http://dat.xylfe.cn

================================================================================
来源：http://cpl.nanxuanxn.top

[P01] 生成 UUID
来源：http://pfv.ivvv.top

Py:   str(uuid.uuid4())
来源：http://hvq.hnxiangtu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ygf.hesvh.cn

JS:   crypto.randomUUID()
来源：http://gan.ppjwa.cn

TS:   crypto.randomUUID()
来源：http://lrf.zhengqikj.top

Java: UUID.randomUUID().toString()
来源：http://vzg.nwbrower.top

Go:   // 用 github.com/google/uuid
来源：http://mkj.redwolf501.top

Ruby: SecureRandom.uuid
来源：http://mig.andypj.xyz

C#:   Guid.NewGuid().ToString()
来源：http://woz.pengpengdd.cyou

[P02] MD5 / SHA256 摘要
来源：http://rul.9152youxi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://eul.zycfv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://khg.jianghu66.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ock.xziqi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xjg.sufxvd.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fef.haohaochexian.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ouc.kuanghao11.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rfh.chenzaomai.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jbh.hesvh.cn

[P03] 生成短随机字符串
来源：http://ehs.ybcxt.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://exu.meibo888.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qpe.yvedp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://akm.hfpthk.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qio.dianchejie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sms.fengsongda.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vrb.chenzaomai.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://pgy.jqgufenzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://plu.svipenyu.cn

[P04] 求长度
来源：http://xlx.epnwcf.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ozt.havefunace.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mgg.9152youxi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ihp.dashuyun.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oka.yanxiufei.cn

Java: list.size();  map.size();  s.length()
来源：http://bvk.fengsongda.top

Go:   len(arr);  len(m)
来源：http://swa.yvedp.cn

Ruby: x.length;  x.size
来源：http://kmj.daxiang520.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://cgf.yonumen.top

[P05] 判断两个对象内容是否相等
来源：http://wsk.hammf.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://uxx.aizwys.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ojn.ydzc1.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wdp.zdbjq.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zop.9152youxi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rqi.shuidangran.top

Go:   reflect.DeepEqual(a, b)
来源：http://gac.mhx1999.top

Ruby: a == b
来源：http://hxr.redwolf501.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uqf.xingfuxueyuan.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://aak.gotoacloud.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://edz.aibaodan.cn

PHP:  if (empty($x)) {}
来源：http://ulr.nwbrower.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mar.yuanzhike.top

TS:   if (x == null) {}
来源：http://siu.shzxlz.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://psi.jinyuanbaomall.cn

Go:   if x == nil {}
来源：http://yjl.hcnkem.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dng.sysykeji.top

C#:   if (x is null) {}
来源：http://hsu.tanke756.top

[P07] 防抖与节流
来源：http://fpd.cashguo.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://apy.gogol.net.cn

PHP:  // 手写时间戳比较
来源：http://xnr.guannengcc.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ghb.yj20258.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hbn.yj20258.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tji.xingfuxueyuan.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hqp.xuetiantiany.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gyd.shzxlz.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zak.tarul.cn

[P08] 处理浮点精度问题
来源：http://eqx.yueranfly.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gvx.mhx1999.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qgm.shanyushiyangtech.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yjy.kuanghao11.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://goz.shanyushiyangtech.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fen.pengpengdd.cyou

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ptk.jinqigufen.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://noy.cqqwz.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kry.yuxming.cn

================================================================================
来源：http://idt.hfpthk.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nxf.hywenlv.cn

================================================================================
来源：http://add.bbcook.cn

[Q01] 创建表
来源：http://tjn.ywan-chungtsiang.top

CREATE TABLE users (
来源：http://mwz.shangyingyoupin.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tfh.fengsongda.top

name VARCHAR(50) NOT NULL,
来源：http://sfa.aizwys.cn

email VARCHAR(100) UNIQUE,
来源：http://yhh.sjlbkw.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jrr.zhijiandao.cn

);
来源：http://vbn.yangfankeji.com

[Q02] 创建带外键的表
来源：http://afd.gotoacloud.top

CREATE TABLE orders (
来源：http://cwr.yuxming.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uox.zhoulong.xyz

user_id INT NOT NULL,
来源：http://yrb.shangyingyoupin.top

amount DECIMAL(10, 2),
来源：http://fnc.pycfn.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uoi.ydjk.org.cn

);
来源：http://epn.nanxuanxn.top

[Q03] 增加列
来源：http://bsv.yj202588.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lbz.snrcjt.cn

[Q04] 修改列类型
来源：http://xjv.tarul.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qxu.aibaodan.cn

[Q05] 重命名列
来源：http://wox.guowangkeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pqd.cashguo.top

[Q06] 删除列
来源：http://gjm.hongshengwenyu.top

ALTER TABLE users DROP COLUMN age;
来源：http://lvu.jinghuilouyu.cn

[Q07] 删除表
来源：http://sap.dashuyun.cn

DROP TABLE IF EXISTS orders;
来源：http://jcf.ywan-chungtsiang.top

[Q08] 创建普通索引
来源：http://dzm.shanyushiyangtech.top

CREATE INDEX idx_users_email ON users(email);
来源：http://fzi.mhx1999.top

[Q09] 创建唯一索引
来源：http://qtf.haohaochexian.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wqm.yanxiufei.cn

[Q10] 插入单行
来源：http://vpf.yangfankeji.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://duj.gotoacloud.top

[Q11] 一次插入多行
来源：http://cag.andypj.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uiu.cqqwz.cn

[Q12] 插入后取自增 ID
来源：http://wbc.wangshuangyany.cn

INSERT INTO users (name) VALUES ('C');
来源：http://cis.sysykeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ffx.hnxiangtu.top

[Q13] 忽略重复插入
来源：http://fhj.ybcxt.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dcn.tanke756.top

[Q14] 存在则更新（upsert）
来源：http://sgi.zhengqikj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://asg.bbcook.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qhy.cheryme.top

[Q15] 查询全部
来源：http://oxg.yonumen.top

SELECT * FROM users;
来源：http://die.hywenlv.cn

[Q16] 查询指定列
来源：http://lix.nwbrower.top

SELECT id, name FROM users;
来源：http://kgd.nwbrower.top

[Q17] 条件查询
来源：http://dbz.fanxiaobao.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://txw.jiagoushi.top

[Q18] 模糊匹配
来源：http://ilb.yonumen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pat.pycfn.com

[Q19] 范围查询
来源：http://fyk.zhoulong.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mlh.quarkkingdee.top

[Q20] IN 列表
来源：http://usj.quarkkingdee.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ylg.jyoumei.cn

[Q21] 空值判断
来源：http://hkc.quarkkingdee.top

SELECT * FROM users WHERE email IS NULL;
来源：http://tdy.aizwys.cn

[Q22] 排序
来源：http://zrm.cheryme.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ncj.zhixingplan.top

[Q23] 分页
来源：http://bea.cheryme.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pwc.vqdsnc.cn

[Q24] 去重
来源：http://wcp.guannengcc.top

SELECT DISTINCT city FROM users;
来源：http://xlb.ybcxt.top

[Q25] 只取前 N 条
来源：http://ssm.shuidangran.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uvp.bjfxy.top

[Q26] 计数
来源：http://mio.zhongyouzk.top

SELECT COUNT(*) FROM users;
来源：http://rlv.sxryk.cn

[Q27] 条件计数
来源：http://yud.hfpthk.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rgv.yuanzhike.top

[Q28] 求和与平均
来源：http://dbu.wangshuangyany.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tio.jyoumei.cn

[Q29] 最大最小值
来源：http://wzp.chenlongwang.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://kai.sysykeji.top

[Q30] 分组统计
来源：http://grr.dashuyun.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zfb.shangyingyoupin.top

[Q31] 分组后过滤
来源：http://gqy.nwbrower.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://roe.ctjpmb.com

[Q32] 分组拼接字符串
来源：http://xmc.shzxlz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wkm.wangshuangyany.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bmi.jlsjyb.cn

[Q33] 多列分组
来源：http://mto.ctjpmb.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hgr.tanke756.top

[Q34] 每组取第一条
来源：http://yhn.yuxming.cn

SELECT * FROM (
来源：http://dmx.hesvh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fxs.zhoulong.xyz

) t WHERE rn = 1;
来源：http://mxp.zdbjq.cn

[Q35] 内连接
来源：http://zci.gaohongyu789.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://slh.zhengqikj.top

[Q36] 左连接
来源：http://suk.ehwqpu.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zrd.nanxuanxn.top

[Q37] 右连接
来源：http://ydg.hongshengwenyu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kkb.jinqigufen.top

[Q38] 全外连接（PostgreSQL）
来源：http://qeh.meibo888.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://iod.iojbl.cn

[Q39] 自连接（查上下级）
来源：http://vwh.fzhhl.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://kvs.zhiwuduotai.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ptn.hnxiangtu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://net.meibo888.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dlf.hywenlv.cn

[Q41] 多表连接
来源：http://ssp.jyoumei.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://akz.tian-w.cn

JOIN users u ON u.id = o.user_id
来源：http://ofg.ywan-chungtsiang.top

JOIN products p ON p.id = o.product_id;
来源：http://yya.haohaochexian.top

[Q42] 连接条件附加过滤
来源：http://qan.yueranfly.top

SELECT u.name, o.amount FROM users u
来源：http://rdm.aibaodan.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yue.yanxiufei.cn

[Q43] 标量子查询
来源：http://get.jianghu66.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bdw.9152youxi.cn

[Q44] IN 子查询
来源：http://hhr.bbcook.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://iun.gogol.net.cn

[Q45] EXISTS 判断存在
来源：http://qxq.hfpthk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ncz.gogol.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zwr.jqgufenzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gdh.yuxming.cn

[Q47] 与平均值比较
来源：http://dvz.cucudq.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dmz.xinyue.icu

[Q48] CTE 公用表表达式
来源：http://jvl.jqgfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wvn.52xcode.cn

SELECT * FROM t WHERE c > 5;
来源：http://ait.jinyuanbaomall.cn

[Q49] 更新单行
来源：http://ene.sweek.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ciy.uphjek.com

[Q50] 批量更新
来源：http://fju.ydzc1.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qcc.sweek.top

[Q51] 用子查询更新
来源：http://lxk.cdnleiting.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kiy.zdbjq.cn

[Q52] 删除指定行
来源：http://qll.dianchejie.cn

DELETE FROM users WHERE id = 10;
来源：http://cej.xylfe.cn

[Q53] 按条件删除
来源：http://ybk.ivvv.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qcb.yonumen.top

[Q54] 清空表
来源：http://rgs.yj20258888.top

TRUNCATE TABLE logs;
来源：http://dbh.fzhhl.top

[Q55] 排名（并列占位）
来源：http://wja.sweek.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dux.zhoulong.xyz

[Q56] 密集排名（并列不占位）
来源：http://osd.jinyuanbaomall.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hgf.ydzc1.top

[Q57] 行号
来源：http://bto.bbcook.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vyg.yvedp.cn

[Q58] 累计求和
来源：http://mau.gzhubu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://skz.ppjwa.cn

[Q59] 分组内累计
来源：http://rsk.zdqjudy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://egs.yj20258888.top

[Q60] 取上一行 / 下一行
来源：http://iji.xinyue.icu

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://esg.jlsjyb.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zht.jinqigfzy.top

[Q61] 移动平均
来源：http://cyf.feifeiyinyue.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iou.yongpay.top

[Q62] 分组占比
来源：http://zwr.9152youxi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wvu.hongshengwenyu.top


<!-- 参考信息 -->