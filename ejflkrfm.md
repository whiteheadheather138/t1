代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lay.tanke756.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bbq.52xcode.cn

Java: class Node { int v; Node next; }
来源：http://qjv.yj20258888.top

Go:   type Node struct { V int; Next *Node }
来源：http://dnq.ctjpmb.com

Ruby: Node = Struct.new(:v, :next)
来源：http://jhs.tarul.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://juk.jqgfzy.top

[N11] 二叉树中序遍历
来源：http://nrm.yuanzhike.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kan.hnqzz.top

PHP:  // 手写递归函数
来源：http://haf.epnwcf.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://udt.yongpay.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vco.fktsv.cn

Java: // 手写递归
来源：http://eva.nanxinkj.top

Go:   // 手写递归
来源：http://pds.zhengqikj.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tdr.fzhhl.top

C#:   // 手写递归
来源：http://tdx.pycfn.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qzi.hcnkem.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jxz.zdbjq.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://llz.sjlbkw.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hus.xinyue.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nly.aizwys.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qyn.yuanzhike.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gjg.daria6918.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xqy.ywan-chungtsiang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nfp.cheryme.top

================================================================================
来源：http://aac.havefunace.top

O. 并发与异步
来源：http://ghl.yueranfly.top

================================================================================
来源：http://cka.tianlin.xyz

[O01] 启动一个线程
来源：http://dnf.ybcxt.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sdv.yj202588.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jql.zdbjq.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wuq.c1oappe.top

TS:   // 同 JS
来源：http://ooo.ehwqpu.com

Java: new Thread(() -> f()).start()
来源：http://inw.cqqwz.cn

Go:   go f()
来源：http://agc.xylfe.cn

Ruby: Thread.new { f }
来源：http://ktf.wangdashe.top

C#:   Task.Run(() => F());
来源：http://csi.zhengqikj.top

[O02] 使用线程池
来源：http://iif.jinqigfzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fqn.tarul.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mai.tianlin.xyz

JS:   // worker_threads 线程池
来源：http://mgr.jiagoushi.top

TS:   // worker_threads 线程池
来源：http://sfa.daxiang520.top

Java: Executors.newFixedThreadPool(4)
来源：http://dip.zhijiandao.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yhw.c1oappe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gbl.hnxiangtu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yyb.yuxming.cn

[O03] 加锁保护共享数据
来源：http://gdj.ywan-chungtsiang.top

Py:   with lock: shared += 1
来源：http://xpp.tianlin.xyz

PHP:  // 用 flock() 做文件锁
来源：http://ckg.xylfe.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nhd.ydjk.org.cn

TS:   // 同 JS
来源：http://cdh.zhengqikj.top

Java: synchronized (this) { shared++; }
来源：http://mbs.tian-w.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wly.pycfn.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://fsw.tianlin.xyz

C#:   lock (gate) { shared++; }
来源：http://hwj.gzhubu.top

[O04] 定义异步函数并等待
来源：http://olu.shangyingyoupin.top

Py:   async def f():⏎    await g()
来源：http://fzk.zhongyouzk.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nlf.xuanzx.com

JS:   async function f() { await g(); }
来源：http://fcj.svipenyu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fug.yanxiufei.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ykh.sxryk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ndg.ydzc1.top

Ruby: # 用 Fiber 或 async gem
来源：http://qdl.yuxming.cn

C#:   async Task F() { await G(); }
来源：http://hjq.yvedp.cn

[O05] 并发执行并等待全部完成
来源：http://pvq.gotoacloud.top

Py:   asyncio.gather(*tasks)
来源：http://mmo.xuetiantiany.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uhf.andypj.xyz

JS:   await Promise.all(tasks)
来源：http://tra.jinghuilouyu.cn

TS:   await Promise.all(tasks)
来源：http://cnl.gogol.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jrl.yonumen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nig.sjlbkw.cn

Ruby: threads.map(&:join)
来源：http://znz.chenjidiqi.icu

C#:   await Task.WhenAll(t1, t2)
来源：http://mvz.cheryme.top

[O06] 使用进程池
来源：http://suu.sysykeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://inr.sweek.top

PHP:  // pcntl_fork 或多进程队列
来源：http://iut.jinghuilouyu.cn

JS:   // child_process / cluster 模块
来源：http://urx.yj20258888.top

TS:   // child_process / cluster 模块
来源：http://bkd.jyoumei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bqm.jlsjyb.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rzt.ywan-chungtsiang.top

Ruby: // fork 块
来源：http://aru.hnqzz.top

C#:   Parallel.For
来源：http://glu.dashuyun.cn

================================================================================
来源：http://rpt.yj20258.top

P. 常用工具函数
来源：http://iyw.shanyushiyangkeji.top

================================================================================
来源：http://jmh.xziqi.cn

[P01] 生成 UUID
来源：http://wto.fktsv.cn

Py:   str(uuid.uuid4())
来源：http://jxa.pycfn.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://acw.daria6918.cn

JS:   crypto.randomUUID()
来源：http://tep.svipenyu.cn

TS:   crypto.randomUUID()
来源：http://cjv.mhx1999.top

Java: UUID.randomUUID().toString()
来源：http://cgk.cheryme.top

Go:   // 用 github.com/google/uuid
来源：http://wax.nanxinkj.top

Ruby: SecureRandom.uuid
来源：http://qbl.yj202588.top

C#:   Guid.NewGuid().ToString()
来源：http://kqf.havefunace.top

[P02] MD5 / SHA256 摘要
来源：http://mxr.fktsv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dmw.zhengqikj.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://flc.kuanghao11.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://inn.hcnkem.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://eof.jqgufenzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://skp.hysaishi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://azd.haohaochexian.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nrw.yfazqb.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://atf.yuxming.cn

[P03] 生成短随机字符串
来源：http://hsp.jyoumei.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://syq.yvedp.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://djb.aibaodan.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://llq.yuanzhike.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://imi.cucudq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jxf.c1oappe.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dtu.aibaodan.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://avt.jianghu66.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hig.nanxinkj.top

[P04] 求长度
来源：http://xsq.tarul.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cge.0kj1m.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://flk.gogol.net.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kwd.yj20258.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mme.guowangkeji.top

Java: list.size();  map.size();  s.length()
来源：http://yka.bbcook.cn

Go:   len(arr);  len(m)
来源：http://aqd.316326.xyz

Ruby: x.length;  x.size
来源：http://lby.nanxinkj.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://bxg.cdnleiting.top

[P05] 判断两个对象内容是否相等
来源：http://brd.ctjpmb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://gzl.jlsjyb.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rap.fehbvm.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lzn.ppjwa.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bth.hnxiangtu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ics.zhoulong.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://sgx.chenzaomai.com

Ruby: a == b
来源：http://mar.zhongyouzk.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jay.jinyuanbaomall.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hpx.hcnkem.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lzl.vehdjk.com

PHP:  if (empty($x)) {}
来源：http://kvv.c1oappe.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yby.chenzaomai.com

TS:   if (x == null) {}
来源：http://jjt.nanxinkj.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ytm.tarul.cn

Go:   if x == nil {}
来源：http://iml.yj20258888.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tpz.sxryk.cn

C#:   if (x is null) {}
来源：http://nsx.ydjk.org.cn

[P07] 防抖与节流
来源：http://pib.hysaishi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mpb.shuidangran.top

PHP:  // 手写时间戳比较
来源：http://bsj.zhijiandao.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qui.zycfv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ylo.xziqi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gvo.ehwqpu.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pfb.jqgfzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://tyb.guannengcc.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lll.316326.xyz

[P08] 处理浮点精度问题
来源：http://nsi.gaohongyu789.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bjm.cucudq.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qke.yj202588.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dfu.jinqigfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ewq.zhongyouzk.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oxs.wangdashe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uwg.shuidangran.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ade.havefunace.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://spv.yj202588.top

================================================================================
来源：http://bct.cdnleiting.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lme.hcnkem.com

================================================================================
来源：http://qhs.pengpengdd.cyou

[Q01] 创建表
来源：http://uvu.shanyushiyangtech.top

CREATE TABLE users (
来源：http://duj.zdqjudy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cus.uphjek.com

name VARCHAR(50) NOT NULL,
来源：http://yyj.nwbrower.top

email VARCHAR(100) UNIQUE,
来源：http://slv.hysaishi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ixl.meibo888.top

);
来源：http://zxx.shanyushiyangkeji.top

[Q02] 创建带外键的表
来源：http://cjd.daxiang520.top

CREATE TABLE orders (
来源：http://ltq.yongpay.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://myj.jinghuilouyu.cn

user_id INT NOT NULL,
来源：http://qbz.epnwcf.com

amount DECIMAL(10, 2),
来源：http://tsa.yueranfly.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://efg.yj20258888.top

);
来源：http://mfy.yonumen.top

[Q03] 增加列
来源：http://xid.ctjpmb.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sqe.pycfn.com

[Q04] 修改列类型
来源：http://nxd.fengsongda.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lnv.sweek.top

[Q05] 重命名列
来源：http://pew.ehwqpu.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xat.aibaodan.cn

[Q06] 删除列
来源：http://ubl.chenzaomai.com

ALTER TABLE users DROP COLUMN age;
来源：http://gxp.vqdsnc.cn

[Q07] 删除表
来源：http://wnw.jinghuilouyu.cn

DROP TABLE IF EXISTS orders;
来源：http://iye.zhoulong.xyz

[Q08] 创建普通索引
来源：http://bag.ybcxt.top

CREATE INDEX idx_users_email ON users(email);
来源：http://quu.yangfankeji.com

[Q09] 创建唯一索引
来源：http://qos.vehdjk.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pfy.yanxiufei.cn

[Q10] 插入单行
来源：http://pus.jinyuanbaomall.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lou.shangyingyoupin.top

[Q11] 一次插入多行
来源：http://yhu.daxiang520.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uox.yongpay.top

[Q12] 插入后取自增 ID
来源：http://pgh.quarkkingdee.top

INSERT INTO users (name) VALUES ('C');
来源：http://vnf.fktsv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dyh.sysykeji.top

[Q13] 忽略重复插入
来源：http://dpc.daxiang520.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sct.zhengqikj.top

[Q14] 存在则更新（upsert）
来源：http://wis.pycfn.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://igc.yongpay.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pje.dianchejie.cn

[Q15] 查询全部
来源：http://upr.yj20258.top

SELECT * FROM users;
来源：http://tph.cqqwz.cn

[Q16] 查询指定列
来源：http://wda.cucudq.cn

SELECT id, name FROM users;
来源：http://xwq.bbcook.cn

[Q17] 条件查询
来源：http://yox.nanxinkj.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kvj.gaohongyu789.top

[Q18] 模糊匹配
来源：http://xjp.gotoacloud.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bqg.zhoulong.xyz

[Q19] 范围查询
来源：http://oja.chenjidiqi.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kzw.cheryme.top

[Q20] IN 列表
来源：http://xkc.yj20258888.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oel.xingfuxueyuan.xyz

[Q21] 空值判断
来源：http://qpf.yongpay.top

SELECT * FROM users WHERE email IS NULL;
来源：http://wtl.xziqi.cn

[Q22] 排序
来源：http://skj.shuidangran.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wwh.uphjek.com

[Q23] 分页
来源：http://bvl.redwolf501.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lmz.shangyingyoupin.top

[Q24] 去重
来源：http://ysz.aizwys.cn

SELECT DISTINCT city FROM users;
来源：http://ieb.daxiang520.top

[Q25] 只取前 N 条
来源：http://ulv.dashuyun.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ofh.wangshuangyany.cn

[Q26] 计数
来源：http://jdm.wangdashe.top

SELECT COUNT(*) FROM users;
来源：http://itx.yangfankeji.com

[Q27] 条件计数
来源：http://tnb.nanxuanxn.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bgv.shanyushiyangtech.top

[Q28] 求和与平均
来源：http://wdw.smart0.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rnz.nanxinkj.top

[Q29] 最大最小值
来源：http://wrt.hfpthk.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ltg.snrcjt.cn

[Q30] 分组统计
来源：http://myf.pengpengdd.cyou

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ngf.jqgufenzy.top

[Q31] 分组后过滤
来源：http://knz.jinghuilouyu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cpw.jqgufenzy.top

[Q32] 分组拼接字符串
来源：http://fqf.hcnkem.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mkh.sxryk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gqh.kuanghao11.cn

[Q33] 多列分组
来源：http://fdn.svipenyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dwu.tanke756.top

[Q34] 每组取第一条
来源：http://kgc.yongpay.top

SELECT * FROM (
来源：http://xtl.vqdsnc.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mhb.kuanghao11.cn

) t WHERE rn = 1;
来源：http://ymz.sxryk.cn

[Q35] 内连接
来源：http://tvt.ivvv.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ncq.smart0.xyz

[Q36] 左连接
来源：http://xqu.9152youxi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xht.jianghu66.top

[Q37] 右连接
来源：http://ekw.yj20258.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yfr.cdnleiting.top

[Q38] 全外连接（PostgreSQL）
来源：http://yiw.gogol.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dre.aibaodan.cn

[Q39] 自连接（查上下级）
来源：http://cdl.uphjek.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://dga.jianghu66.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rez.yuanzhike.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xhv.nanxinkj.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qii.chenlongwang.top

[Q41] 多表连接
来源：http://bfd.ehwqpu.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://ucw.jinqigufen.top

JOIN users u ON u.id = o.user_id
来源：http://lwx.jinqigufen.top

JOIN products p ON p.id = o.product_id;
来源：http://ddd.gaohongyu789.top

[Q42] 连接条件附加过滤
来源：http://jap.xuetiantiany.cn

SELECT u.name, o.amount FROM users u
来源：http://csc.iojbl.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://omk.zhaomingkeji.xyz

[Q43] 标量子查询
来源：http://xes.yj20258.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zll.shanyushiyangtech.top

[Q44] IN 子查询
来源：http://gpf.meibo888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lxm.cucudq.cn

[Q45] EXISTS 判断存在
来源：http://qhw.xziqi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fmi.shanyushiyangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://scq.hnxiangtu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cum.xylfe.cn

[Q47] 与平均值比较
来源：http://fli.tanke756.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fxy.zycfv.cn

[Q48] CTE 公用表表达式
来源：http://nyq.dianchejie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lif.jinyuanbaomall.cn

SELECT * FROM t WHERE c > 5;
来源：http://sgs.xuetiantiany.cn

[Q49] 更新单行
来源：http://scd.chenlongwang.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tzk.cdnleiting.top

[Q50] 批量更新
来源：http://sbp.fanxiaobao.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xnb.vehdjk.com

[Q51] 用子查询更新
来源：http://tpo.zhengqikj.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hbi.ctjpmb.com

[Q52] 删除指定行
来源：http://uzs.vqdsnc.cn

DELETE FROM users WHERE id = 10;
来源：http://zmd.feifeiyinyue.top

[Q53] 按条件删除
来源：http://val.fanxiaobao.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ekk.guannengcc.top

[Q54] 清空表
来源：http://wrk.ctjpmb.com

TRUNCATE TABLE logs;
来源：http://wmu.fengsongda.top

[Q55] 排名（并列占位）
来源：http://nob.yvedp.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ugc.zycfv.cn

[Q56] 密集排名（并列不占位）
来源：http://vis.cdnleiting.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zfv.yonumen.top

[Q57] 行号
来源：http://czg.chenjidiqi.icu

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cqk.xuanzx.com

[Q58] 累计求和
来源：http://xmi.shanyushiyangtech.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tfg.xingfuxueyuan.xyz

[Q59] 分组内累计
来源：http://btn.ydjk.org.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tmt.xziqi.cn

[Q60] 取上一行 / 下一行
来源：http://sbz.cheryme.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://utd.zhijiandao.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://eit.zhoulong.xyz


<!-- 参考信息 -->