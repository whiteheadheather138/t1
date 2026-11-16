代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://yei.nanxuanxn.top

C#:   class Node { public int V; public Node? Next; }
来源：http://mlt.yj20258.top

[N11] 二叉树中序遍历
来源：http://ywh.nanxuanxn.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://koa.tarul.cn

PHP:  // 手写递归函数
来源：http://vok.xinyue.icu

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xto.xinyue.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dfa.quarkkingdee.top

Java: // 手写递归
来源：http://xls.zhoulong.xyz

Go:   // 手写递归
来源：http://euc.xylfe.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eva.nwbrower.top

C#:   // 手写递归
来源：http://xah.ydjk.org.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gxa.fktsv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://syt.chenlongwang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://woi.birdmap.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hwk.zhaomingkeji.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bxh.ppjwa.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uwu.hywenlv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bjf.havefunace.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cwd.dashuyun.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lne.pengpengdd.cyou

================================================================================
来源：http://eyv.hammf.cn

O. 并发与异步
来源：http://pys.jqgfzy.top

================================================================================
来源：http://jkt.yongpay.top

[O01] 启动一个线程
来源：http://svk.cheryme.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wkv.xylfe.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jpp.shzxlz.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bcl.316326.xyz

TS:   // 同 JS
来源：http://hfh.tanke756.top

Java: new Thread(() -> f()).start()
来源：http://xcc.jqgfzy.top

Go:   go f()
来源：http://upk.zhoulong.xyz

Ruby: Thread.new { f }
来源：http://jfv.ydjk.org.cn

C#:   Task.Run(() => F());
来源：http://ien.jinqigfzy.top

[O02] 使用线程池
来源：http://flr.birdmap.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pdr.epnwcf.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qar.dashuyun.cn

JS:   // worker_threads 线程池
来源：http://bzx.9152youxi.cn

TS:   // worker_threads 线程池
来源：http://iwc.cqqwz.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nqt.sufxvd.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://svp.0kj1m.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lrb.nwbrower.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rhx.cucudq.cn

[O03] 加锁保护共享数据
来源：http://bgj.xylfe.cn

Py:   with lock: shared += 1
来源：http://uvl.bbcook.cn

PHP:  // 用 flock() 做文件锁
来源：http://xvy.fktsv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hrn.gzhubu.top

TS:   // 同 JS
来源：http://rlt.zycfv.cn

Java: synchronized (this) { shared++; }
来源：http://mhg.fktsv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zyy.epnwcf.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://kjx.fehbvm.com

C#:   lock (gate) { shared++; }
来源：http://ryj.cucudq.cn

[O04] 定义异步函数并等待
来源：http://tnq.fanxiaobao.xyz

Py:   async def f():⏎    await g()
来源：http://dkx.zdbjq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wlb.havefunace.top

JS:   async function f() { await g(); }
来源：http://pgl.mhx1999.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://tdg.sxryk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ass.xylfe.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yve.zhijiandao.cn

Ruby: # 用 Fiber 或 async gem
来源：http://edx.havefunace.top

C#:   async Task F() { await G(); }
来源：http://tcq.gogol.net.cn

[O05] 并发执行并等待全部完成
来源：http://zpq.ppjwa.cn

Py:   asyncio.gather(*tasks)
来源：http://bfw.hysaishi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://iki.chenlongwang.top

JS:   await Promise.all(tasks)
来源：http://rse.birdmap.top

TS:   await Promise.all(tasks)
来源：http://krb.hnxiangtu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cgk.316326.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uvx.ctjpmb.com

Ruby: threads.map(&:join)
来源：http://hgl.cheryme.top

C#:   await Task.WhenAll(t1, t2)
来源：http://zio.aibaodan.cn

[O06] 使用进程池
来源：http://crx.xuanzx.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rjn.ydjk.org.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://sxl.xinyue.icu

JS:   // child_process / cluster 模块
来源：http://pdb.ehwqpu.com

TS:   // child_process / cluster 模块
来源：http://ohf.iojbl.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ftv.jinghuilouyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mbe.hongshengwenyu.top

Ruby: // fork 块
来源：http://ekz.smart0.xyz

C#:   Parallel.For
来源：http://ype.redwolf501.top

================================================================================
来源：http://kkr.cqqwz.cn

P. 常用工具函数
来源：http://mol.fengsongda.top

================================================================================
来源：http://fix.zhongyouzk.top

[P01] 生成 UUID
来源：http://zuk.iojbl.cn

Py:   str(uuid.uuid4())
来源：http://bxd.jqgufenzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zim.gzhubu.top

JS:   crypto.randomUUID()
来源：http://iwy.snrcjt.cn

TS:   crypto.randomUUID()
来源：http://nrl.cheryme.top

Java: UUID.randomUUID().toString()
来源：http://vgf.guannengcc.top

Go:   // 用 github.com/google/uuid
来源：http://ekx.hysaishi.cn

Ruby: SecureRandom.uuid
来源：http://nmv.yj20258888.top

C#:   Guid.NewGuid().ToString()
来源：http://xyj.andypj.xyz

[P02] MD5 / SHA256 摘要
来源：http://lbv.ivvv.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mib.ppjwa.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://dtj.shuidangran.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xoz.9152youxi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hhb.sweek.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hrk.iojbl.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yvo.meibo888.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lrg.gogol.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dri.zhaomingkeji.xyz

[P03] 生成短随机字符串
来源：http://hgq.smart0.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ckw.fehbvm.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hep.hfpthk.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vda.ctjpmb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://khp.nanxuanxn.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rek.vqdsnc.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jmy.gotoacloud.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://bix.fktsv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jrq.iojbl.cn

[P04] 求长度
来源：http://ecn.wangshuangyany.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mry.epnwcf.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tet.zhengqikj.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uit.tarul.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cwe.zhoulong.xyz

Java: list.size();  map.size();  s.length()
来源：http://ubg.fehbvm.com

Go:   len(arr);  len(m)
来源：http://hul.fengsongda.top

Ruby: x.length;  x.size
来源：http://fzh.tian-w.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kmt.pengpengdd.cyou

[P05] 判断两个对象内容是否相等
来源：http://xab.zhaomingkeji.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://ytq.hnqzz.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nfj.guowangkeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qbd.ywan-chungtsiang.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ohf.zhoulong.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jrm.316326.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://sin.nwbrower.top

Ruby: a == b
来源：http://qrl.nanxuanxn.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cpm.yongpay.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ldf.hammf.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://eyp.guannengcc.top

PHP:  if (empty($x)) {}
来源：http://bgq.jinyuanbaomall.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rok.chenzaomai.com

TS:   if (x == null) {}
来源：http://eev.daria6918.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zyt.jinqigufen.top

Go:   if x == nil {}
来源：http://uap.hnxiangtu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zwk.kuanghao11.cn

C#:   if (x is null) {}
来源：http://dby.meibo888.top

[P07] 防抖与节流
来源：http://hyb.zhoulong.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jqu.bjfxy.top

PHP:  // 手写时间戳比较
来源：http://xls.fzhhl.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://byw.sweek.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ztw.shanyushiyangtech.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cpb.zycfv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://goq.xziqi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://jqn.xuetiantiany.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://exh.zhijiandao.cn

[P08] 处理浮点精度问题
来源：http://bit.yongpay.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://iox.shangyingyoupin.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bdw.ywan-chungtsiang.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ule.yueranfly.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xmu.chenzaomai.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qgl.jinqigfzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zgn.iojbl.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://arw.sysykeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bzp.0kj1m.cn

================================================================================
来源：http://isc.jinqigfzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rrn.gotoacloud.top

================================================================================
来源：http://ajx.shzxlz.cn

[Q01] 创建表
来源：http://tcw.nanxuanxn.top

CREATE TABLE users (
来源：http://etd.hammf.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lkr.yanxiufei.cn

name VARCHAR(50) NOT NULL,
来源：http://tmz.c1oappe.top

email VARCHAR(100) UNIQUE,
来源：http://ses.jianghu66.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dnr.yj20258888.top

);
来源：http://pxi.fzhhl.top

[Q02] 创建带外键的表
来源：http://hbg.quarkkingdee.top

CREATE TABLE orders (
来源：http://eng.svipenyu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gul.fzhhl.top

user_id INT NOT NULL,
来源：http://jda.yangfankeji.com

amount DECIMAL(10, 2),
来源：http://scp.ydjk.org.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hen.guowangkeji.top

);
来源：http://byb.cucudq.cn

[Q03] 增加列
来源：http://pse.bjfxy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fii.chenlongwang.top

[Q04] 修改列类型
来源：http://qcw.vehdjk.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cwf.ydzc1.top

[Q05] 重命名列
来源：http://lul.jyoumei.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://poh.zhijiandao.cn

[Q06] 删除列
来源：http://hot.snrcjt.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sji.hfpthk.cn

[Q07] 删除表
来源：http://eiv.fanxiaobao.xyz

DROP TABLE IF EXISTS orders;
来源：http://uja.jinqigfzy.top

[Q08] 创建普通索引
来源：http://tcg.shuidangran.top

CREATE INDEX idx_users_email ON users(email);
来源：http://zlj.52xcode.cn

[Q09] 创建唯一索引
来源：http://lme.jqgfzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cxi.yj202588.top

[Q10] 插入单行
来源：http://ycz.yueranfly.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hjn.yongpay.top

[Q11] 一次插入多行
来源：http://dgt.c1oappe.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nal.zdbjq.cn

[Q12] 插入后取自增 ID
来源：http://htr.9152youxi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fbt.ybcxt.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://seb.cheryme.top

[Q13] 忽略重复插入
来源：http://hld.yangfankeji.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xkj.gotoacloud.top

[Q14] 存在则更新（upsert）
来源：http://zqa.ydjk.org.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hkw.cqqwz.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://iai.wangshuangyany.cn

[Q15] 查询全部
来源：http://uic.zdqjudy.top

SELECT * FROM users;
来源：http://ifn.kuanghao11.cn

[Q16] 查询指定列
来源：http://wnv.zdbjq.cn

SELECT id, name FROM users;
来源：http://jss.jiagoushi.top

[Q17] 条件查询
来源：http://hls.xylfe.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lra.cucudq.cn

[Q18] 模糊匹配
来源：http://zby.ppjwa.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tzl.bjfxy.top

[Q19] 范围查询
来源：http://vrr.guowangkeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://utx.shzxlz.cn

[Q20] IN 列表
来源：http://hjr.wangshuangyany.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ffj.bjfxy.top

[Q21] 空值判断
来源：http://vjn.xuanzx.com

SELECT * FROM users WHERE email IS NULL;
来源：http://hlu.shzxlz.cn

[Q22] 排序
来源：http://gvr.yangfankeji.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://irk.wangdashe.top

[Q23] 分页
来源：http://wbl.tanke756.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ham.hammf.cn

[Q24] 去重
来源：http://ttv.pengpengdd.cyou

SELECT DISTINCT city FROM users;
来源：http://hsm.sxryk.cn

[Q25] 只取前 N 条
来源：http://tpw.c1oappe.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ebr.guannengcc.top

[Q26] 计数
来源：http://wsw.cdnleiting.top

SELECT COUNT(*) FROM users;
来源：http://qwz.shuidangran.top

[Q27] 条件计数
来源：http://eaa.mhx1999.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oyw.vqdsnc.cn

[Q28] 求和与平均
来源：http://sdy.zhijiandao.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dtl.sjlbkw.cn

[Q29] 最大最小值
来源：http://rjv.gotoacloud.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://fyf.pengpengdd.cyou

[Q30] 分组统计
来源：http://pgg.redwolf501.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://eph.chenjidiqi.icu

[Q31] 分组后过滤
来源：http://dle.nanxinkj.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rut.ctjpmb.com

[Q32] 分组拼接字符串
来源：http://xcb.hcnkem.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fyw.shanyushiyangkeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ixv.dianchejie.cn

[Q33] 多列分组
来源：http://yld.hywenlv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fyq.zhiwuduotai.top

[Q34] 每组取第一条
来源：http://tgs.nwbrower.top

SELECT * FROM (
来源：http://txm.jqgfzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://icp.yj20258888.top

) t WHERE rn = 1;
来源：http://jun.smart0.xyz

[Q35] 内连接
来源：http://ppu.ybcxt.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vnl.fengsongda.top

[Q36] 左连接
来源：http://pqm.hesvh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ruz.c1oappe.top

[Q37] 右连接
来源：http://nne.zhaomingkeji.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://voe.9152youxi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://afh.hnxiangtu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://meb.shzxlz.cn

[Q39] 自连接（查上下级）
来源：http://rhu.yuanzhike.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://tnk.haohaochexian.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mun.shanyushiyangkeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://eoa.jianghu66.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://var.chenjidiqi.icu

[Q41] 多表连接
来源：http://smd.havefunace.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://rhr.feifeiyinyue.top

JOIN users u ON u.id = o.user_id
来源：http://wmv.yanxiufei.cn

JOIN products p ON p.id = o.product_id;
来源：http://crd.jinyuanbaomall.cn

[Q42] 连接条件附加过滤
来源：http://fxu.yueranfly.top

SELECT u.name, o.amount FROM users u
来源：http://frd.fanxiaobao.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kgt.tianlin.xyz

[Q43] 标量子查询
来源：http://eoi.shzxlz.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yeq.yonumen.top

[Q44] IN 子查询
来源：http://vli.haohaochexian.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xkj.fzhhl.top

[Q45] EXISTS 判断存在
来源：http://zdc.pycfn.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rae.birdmap.top

[Q46] NOT EXISTS 判断不存在
来源：http://lgb.hammf.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://adr.cashguo.top

[Q47] 与平均值比较
来源：http://qbz.xuanzx.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nam.yonumen.top

[Q48] CTE 公用表表达式
来源：http://fdt.ywan-chungtsiang.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hps.cucudq.cn

SELECT * FROM t WHERE c > 5;
来源：http://fuy.zhiwuduotai.top

[Q49] 更新单行
来源：http://zde.xziqi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ssf.zycfv.cn

[Q50] 批量更新
来源：http://yeo.gotoacloud.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kzy.ivvv.top

[Q51] 用子查询更新
来源：http://nmy.tianlin.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gpq.xuetiantiany.cn

[Q52] 删除指定行
来源：http://vmd.xingfuxueyuan.xyz

DELETE FROM users WHERE id = 10;
来源：http://ugh.zdbjq.cn

[Q53] 按条件删除
来源：http://cjp.tarul.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ppf.ivvv.top

[Q54] 清空表
来源：http://hln.svipenyu.cn

TRUNCATE TABLE logs;
来源：http://aln.ywan-chungtsiang.top

[Q55] 排名（并列占位）
来源：http://woh.chenlongwang.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vtm.gotoacloud.top

[Q56] 密集排名（并列不占位）
来源：http://kbn.jqgufenzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://adr.shanyushiyangkeji.top

[Q57] 行号
来源：http://wmh.zdqjudy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qbs.jianghu66.top

[Q58] 累计求和
来源：http://cig.cheryme.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://apr.feifeiyinyue.top

[Q59] 分组内累计
来源：http://ben.smart0.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uva.fanxiaobao.xyz

[Q60] 取上一行 / 下一行
来源：http://gtc.yongpay.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rgr.dashuyun.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ryz.xuanzx.com

[Q61] 移动平均
来源：http://tyy.9152youxi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bvr.wangshuangyany.cn

[Q62] 分组占比
来源：http://mtu.zhixingplan.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://syj.fehbvm.com


<!-- 参考信息 -->