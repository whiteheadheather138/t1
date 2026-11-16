代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bjj.zdqjudy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gfc.cashguo.top

Java: class Node { int v; Node next; }
来源：http://uij.pengpengdd.cyou

Go:   type Node struct { V int; Next *Node }
来源：http://pkz.ehwqpu.com

Ruby: Node = Struct.new(:v, :next)
来源：http://kay.nanxuanxn.top

C#:   class Node { public int V; public Node? Next; }
来源：http://lil.hnqzz.top

[N11] 二叉树中序遍历
来源：http://jdx.9152youxi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hgs.zdqjudy.top

PHP:  // 手写递归函数
来源：http://uza.hywenlv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://grq.wangshuangyany.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dun.nwbrower.top

Java: // 手写递归
来源：http://pxb.sweek.top

Go:   // 手写递归
来源：http://zbh.bjfxy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uyn.pycfn.com

C#:   // 手写递归
来源：http://yks.mhx1999.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://erx.zdbjq.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lxw.shanyushiyangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pno.shuidangran.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fvt.sjlbkw.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://omk.jinqigfzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bpd.vehdjk.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cau.chenlongwang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rak.jinghuilouyu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ljb.cdnleiting.top

================================================================================
来源：http://wpd.gogol.net.cn

O. 并发与异步
来源：http://tgt.meibo888.top

================================================================================
来源：http://bea.316326.xyz

[O01] 启动一个线程
来源：http://kqf.uphjek.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ily.hnxiangtu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kpm.sweek.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gym.zycfv.cn

TS:   // 同 JS
来源：http://wim.gogol.net.cn

Java: new Thread(() -> f()).start()
来源：http://vxh.pycfn.com

Go:   go f()
来源：http://oek.ehwqpu.com

Ruby: Thread.new { f }
来源：http://lqq.yanxiufei.cn

C#:   Task.Run(() => F());
来源：http://ake.iojbl.cn

[O02] 使用线程池
来源：http://pwv.smart0.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zwo.jinghuilouyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mlv.jinghuilouyu.cn

JS:   // worker_threads 线程池
来源：http://urt.shanyushiyangkeji.top

TS:   // worker_threads 线程池
来源：http://saq.shanyushiyangtech.top

Java: Executors.newFixedThreadPool(4)
来源：http://llk.chenjidiqi.icu

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://isu.dianchejie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fzk.yanxiufei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://viy.zhijiandao.cn

[O03] 加锁保护共享数据
来源：http://vbf.9152youxi.cn

Py:   with lock: shared += 1
来源：http://hen.guannengcc.top

PHP:  // 用 flock() 做文件锁
来源：http://ile.zhiwuduotai.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ybd.yonumen.top

TS:   // 同 JS
来源：http://snp.zhiwuduotai.top

Java: synchronized (this) { shared++; }
来源：http://loc.zhaomingkeji.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ece.hongshengwenyu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://mwr.0kj1m.cn

C#:   lock (gate) { shared++; }
来源：http://tac.zycfv.cn

[O04] 定义异步函数并等待
来源：http://yaq.xziqi.cn

Py:   async def f():⏎    await g()
来源：http://nqo.jianghu66.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fou.jyoumei.cn

JS:   async function f() { await g(); }
来源：http://uam.cdnleiting.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://msy.jqgfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wlz.ehwqpu.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wdx.bbcook.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zbp.shzxlz.cn

C#:   async Task F() { await G(); }
来源：http://dxc.pengpengdd.cyou

[O05] 并发执行并等待全部完成
来源：http://bht.haohaochexian.top

Py:   asyncio.gather(*tasks)
来源：http://uqd.jqgufenzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dfs.ywan-chungtsiang.top

JS:   await Promise.all(tasks)
来源：http://mji.svipenyu.cn

TS:   await Promise.all(tasks)
来源：http://lfh.fktsv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jjs.0kj1m.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cln.xinyue.icu

Ruby: threads.map(&:join)
来源：http://rmb.yueranfly.top

C#:   await Task.WhenAll(t1, t2)
来源：http://boz.dashuyun.cn

[O06] 使用进程池
来源：http://nmp.chenzaomai.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tlq.cheryme.top

PHP:  // pcntl_fork 或多进程队列
来源：http://mlt.shanyushiyangtech.top

JS:   // child_process / cluster 模块
来源：http://cam.bbcook.cn

TS:   // child_process / cluster 模块
来源：http://npt.daxiang520.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zcf.iojbl.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jmf.smart0.xyz

Ruby: // fork 块
来源：http://zmu.yj202588.top

C#:   Parallel.For
来源：http://saj.gzhubu.top

================================================================================
来源：http://cjb.jqgfzy.top

P. 常用工具函数
来源：http://azu.ppjwa.cn

================================================================================
来源：http://vwh.guowangkeji.top

[P01] 生成 UUID
来源：http://xpz.zhoulong.xyz

Py:   str(uuid.uuid4())
来源：http://iyg.jqgfzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://brz.aibaodan.cn

JS:   crypto.randomUUID()
来源：http://czp.fehbvm.com

TS:   crypto.randomUUID()
来源：http://cjw.ctjpmb.com

Java: UUID.randomUUID().toString()
来源：http://dus.pycfn.com

Go:   // 用 github.com/google/uuid
来源：http://mek.pycfn.com

Ruby: SecureRandom.uuid
来源：http://jrk.hammf.cn

C#:   Guid.NewGuid().ToString()
来源：http://pxh.hesvh.cn

[P02] MD5 / SHA256 摘要
来源：http://guq.zhaomingkeji.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yjj.ppjwa.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mgk.svipenyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wlz.hammf.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://joi.mhx1999.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uiu.hywenlv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ets.yuxming.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zix.epnwcf.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://apz.feifeiyinyue.top

[P03] 生成短随机字符串
来源：http://cnb.hesvh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ngg.jinqigufen.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://owx.ctjpmb.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rph.quarkkingdee.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dob.zdqjudy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nid.316326.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://eis.chenlongwang.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://qgu.tarul.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://coz.yangfankeji.com

[P04] 求长度
来源：http://lki.gogol.net.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ggv.ywan-chungtsiang.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ebi.yj20258.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ukt.jinqigfzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ied.jlsjyb.cn

Java: list.size();  map.size();  s.length()
来源：http://iqq.guowangkeji.top

Go:   len(arr);  len(m)
来源：http://hoe.smart0.xyz

Ruby: x.length;  x.size
来源：http://enw.fehbvm.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://atd.fktsv.cn

[P05] 判断两个对象内容是否相等
来源：http://ojk.dianchejie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dih.hywenlv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://eva.fengsongda.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rgo.nanxuanxn.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xxn.shanyushiyangtech.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zym.cashguo.top

Go:   reflect.DeepEqual(a, b)
来源：http://jpo.vehdjk.com

Ruby: a == b
来源：http://gis.smart0.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ipe.zhengqikj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hsy.jyoumei.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://edx.ehwqpu.com

PHP:  if (empty($x)) {}
来源：http://fbs.0kj1m.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bue.havefunace.top

TS:   if (x == null) {}
来源：http://pca.fehbvm.com

Java: if (x == null || x.isEmpty()) {}
来源：http://iol.cheryme.top

Go:   if x == nil {}
来源：http://jtl.yj20258888.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yaf.316326.xyz

C#:   if (x is null) {}
来源：http://uvt.andypj.xyz

[P07] 防抖与节流
来源：http://izo.yangfankeji.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ofh.mhx1999.top

PHP:  // 手写时间戳比较
来源：http://otg.tianlin.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kjz.chenzaomai.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bwk.wangdashe.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ybj.hammf.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://khq.haohaochexian.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://cei.hywenlv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://akl.zycfv.cn

[P08] 处理浮点精度问题
来源：http://tpd.zhaomingkeji.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cyy.tianlin.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://usa.shuidangran.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zau.redwolf501.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://foc.daria6918.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mfe.redwolf501.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bxz.svipenyu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ira.sweek.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jwa.xinyue.icu

================================================================================
来源：http://ysi.jqgufenzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hik.nwbrower.top

================================================================================
来源：http://weh.xziqi.cn

[Q01] 创建表
来源：http://keu.pengpengdd.cyou

CREATE TABLE users (
来源：http://nqg.fanxiaobao.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://toa.fktsv.cn

name VARCHAR(50) NOT NULL,
来源：http://ilo.redwolf501.top

email VARCHAR(100) UNIQUE,
来源：http://ehv.jinqigfzy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://iyo.yueranfly.top

);
来源：http://drp.fanxiaobao.xyz

[Q02] 创建带外键的表
来源：http://ond.jiagoushi.top

CREATE TABLE orders (
来源：http://xbx.pengpengdd.cyou

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mkp.jianghu66.top

user_id INT NOT NULL,
来源：http://xhj.chenjidiqi.icu

amount DECIMAL(10, 2),
来源：http://pgq.hongshengwenyu.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://udj.aizwys.cn

);
来源：http://skq.epnwcf.com

[Q03] 增加列
来源：http://rgj.wangshuangyany.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uso.cucudq.cn

[Q04] 修改列类型
来源：http://jwb.daria6918.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cis.fktsv.cn

[Q05] 重命名列
来源：http://ede.fanxiaobao.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fpk.feifeiyinyue.top

[Q06] 删除列
来源：http://drt.hnqzz.top

ALTER TABLE users DROP COLUMN age;
来源：http://dwr.hfpthk.cn

[Q07] 删除表
来源：http://kcs.wangdashe.top

DROP TABLE IF EXISTS orders;
来源：http://cer.yueranfly.top

[Q08] 创建普通索引
来源：http://nxi.tianlin.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://mqk.yj20258.top

[Q09] 创建唯一索引
来源：http://ini.xylfe.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://len.zhaomingkeji.xyz

[Q10] 插入单行
来源：http://gab.gogol.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dtr.jlsjyb.cn

[Q11] 一次插入多行
来源：http://hcu.hnxiangtu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mez.snrcjt.cn

[Q12] 插入后取自增 ID
来源：http://jwb.shanyushiyangkeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://ycp.daria6918.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rdq.zhoulong.xyz

[Q13] 忽略重复插入
来源：http://rxg.feifeiyinyue.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wdj.havefunace.top

[Q14] 存在则更新（upsert）
来源：http://ljs.chenzaomai.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nqo.gogol.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kvb.zdbjq.cn

[Q15] 查询全部
来源：http://sot.uphjek.com

SELECT * FROM users;
来源：http://odh.jinghuilouyu.cn

[Q16] 查询指定列
来源：http://raw.jlsjyb.cn

SELECT id, name FROM users;
来源：http://gsr.birdmap.top

[Q17] 条件查询
来源：http://hng.zhijiandao.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ids.jinqigufen.top

[Q18] 模糊匹配
来源：http://ppd.ehwqpu.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lmq.iojbl.cn

[Q19] 范围查询
来源：http://yet.jqgfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ggi.tian-w.cn

[Q20] IN 列表
来源：http://qrv.sufxvd.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://upg.hammf.cn

[Q21] 空值判断
来源：http://zzy.tianlin.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://kam.chenzaomai.com

[Q22] 排序
来源：http://bpy.havefunace.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cvz.shuidangran.top

[Q23] 分页
来源：http://nkv.yj20258888.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rna.shangyingyoupin.top

[Q24] 去重
来源：http://kam.tanke756.top

SELECT DISTINCT city FROM users;
来源：http://vdf.zhengqikj.top

[Q25] 只取前 N 条
来源：http://vgg.ydzc1.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ada.svipenyu.cn

[Q26] 计数
来源：http://zkg.yonumen.top

SELECT COUNT(*) FROM users;
来源：http://drp.shzxlz.cn

[Q27] 条件计数
来源：http://dzt.yvedp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wiw.52xcode.cn

[Q28] 求和与平均
来源：http://kma.iojbl.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ohx.birdmap.top

[Q29] 最大最小值
来源：http://ppt.sjlbkw.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sjw.cashguo.top

[Q30] 分组统计
来源：http://ips.yanxiufei.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://suz.ydzc1.top

[Q31] 分组后过滤
来源：http://shm.chenzaomai.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bas.zycfv.cn

[Q32] 分组拼接字符串
来源：http://vkg.cucudq.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nat.52xcode.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://clm.bbcook.cn

[Q33] 多列分组
来源：http://tke.aizwys.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://npa.c1oappe.top

[Q34] 每组取第一条
来源：http://ihs.chenjidiqi.icu

SELECT * FROM (
来源：http://dbq.jqgufenzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://aqg.yuxming.cn

) t WHERE rn = 1;
来源：http://gvo.jlsjyb.cn

[Q35] 内连接
来源：http://qdw.pycfn.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vnb.jinqigfzy.top

[Q36] 左连接
来源：http://pra.gaohongyu789.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rue.hywenlv.cn

[Q37] 右连接
来源：http://hyg.daria6918.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lex.redwolf501.top

[Q38] 全外连接（PostgreSQL）
来源：http://ate.tarul.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bny.birdmap.top

[Q39] 自连接（查上下级）
来源：http://kdj.chenlongwang.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://lmn.fktsv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lsc.tarul.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hjr.snrcjt.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nvy.shanyushiyangtech.top

[Q41] 多表连接
来源：http://eub.cashguo.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://nrn.birdmap.top

JOIN users u ON u.id = o.user_id
来源：http://nby.fengsongda.top

JOIN products p ON p.id = o.product_id;
来源：http://blc.jinyuanbaomall.cn

[Q42] 连接条件附加过滤
来源：http://bwa.yuxming.cn

SELECT u.name, o.amount FROM users u
来源：http://hph.fktsv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vdc.tanke756.top

[Q43] 标量子查询
来源：http://dvv.kuanghao11.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ivt.yj20258888.top

[Q44] IN 子查询
来源：http://cec.havefunace.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://idp.gaohongyu789.top

[Q45] EXISTS 判断存在
来源：http://bwq.zycfv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ied.cheryme.top

[Q46] NOT EXISTS 判断不存在
来源：http://ofj.nanxinkj.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tyr.zhijiandao.cn

[Q47] 与平均值比较
来源：http://hvz.ydjk.org.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pfa.havefunace.top

[Q48] CTE 公用表表达式
来源：http://sre.aizwys.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cqr.dianchejie.cn

SELECT * FROM t WHERE c > 5;
来源：http://hje.hesvh.cn

[Q49] 更新单行
来源：http://xaq.ctjpmb.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ycz.sweek.top

[Q50] 批量更新
来源：http://ptj.xuanzx.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://llp.chenzaomai.com

[Q51] 用子查询更新
来源：http://jsc.gaohongyu789.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://aph.snrcjt.cn

[Q52] 删除指定行
来源：http://npz.zhixingplan.top

DELETE FROM users WHERE id = 10;
来源：http://wsd.gaohongyu789.top

[Q53] 按条件删除
来源：http://qcl.yfazqb.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yeu.dianchejie.cn

[Q54] 清空表
来源：http://nfs.uphjek.com

TRUNCATE TABLE logs;
来源：http://scn.gzhubu.top

[Q55] 排名（并列占位）
来源：http://iay.jlsjyb.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://crr.shangyingyoupin.top

[Q56] 密集排名（并列不占位）
来源：http://jdg.316326.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://isf.vqdsnc.cn

[Q57] 行号
来源：http://gqv.snrcjt.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ruj.yj20258.top

[Q58] 累计求和
来源：http://bvj.yuxming.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://byr.jqgufenzy.top

[Q59] 分组内累计
来源：http://ttj.meibo888.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lal.yueranfly.top

[Q60] 取上一行 / 下一行
来源：http://iou.quarkkingdee.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ymg.tarul.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qcr.cashguo.top


<!-- 参考信息 -->