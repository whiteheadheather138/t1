代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://czd.wangshuangyany.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ngb.xziqi.cn

Java: class Node { int v; Node next; }
来源：http://jaw.ydjk.org.cn

Go:   type Node struct { V int; Next *Node }
来源：http://sgr.smart0.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://sgv.chenjidiqi.icu

C#:   class Node { public int V; public Node? Next; }
来源：http://mbv.tianlin.xyz

[N11] 二叉树中序遍历
来源：http://akh.nanxuanxn.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gns.hfpthk.cn

PHP:  // 手写递归函数
来源：http://fwg.mhx1999.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tla.ywan-chungtsiang.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iqj.cashguo.top

Java: // 手写递归
来源：http://bmg.ywan-chungtsiang.top

Go:   // 手写递归
来源：http://toc.nanxuanxn.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dpk.zdbjq.cn

C#:   // 手写递归
来源：http://yzc.hnxiangtu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pig.jlsjyb.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://loa.wangdashe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hkt.andypj.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wju.bjfxy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xwq.sjlbkw.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://keg.daxiang520.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ndh.hnxiangtu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oyp.52xcode.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fkk.smart0.xyz

================================================================================
来源：http://vgd.wangshuangyany.cn

O. 并发与异步
来源：http://knz.hesvh.cn

================================================================================
来源：http://xpe.chenjidiqi.icu

[O01] 启动一个线程
来源：http://ums.zhiwuduotai.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ieh.zdqjudy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kpa.jinqigufen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vnb.tian-w.cn

TS:   // 同 JS
来源：http://vad.yj20258.top

Java: new Thread(() -> f()).start()
来源：http://yqc.shanyushiyangtech.top

Go:   go f()
来源：http://avb.shzxlz.cn

Ruby: Thread.new { f }
来源：http://fbz.shangyingyoupin.top

C#:   Task.Run(() => F());
来源：http://cnw.ctjpmb.com

[O02] 使用线程池
来源：http://kng.jiagoushi.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://txn.wangdashe.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lpw.pycfn.com

JS:   // worker_threads 线程池
来源：http://khc.yj202588.top

TS:   // worker_threads 线程池
来源：http://hos.epnwcf.com

Java: Executors.newFixedThreadPool(4)
来源：http://igq.hnqzz.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zon.vehdjk.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gxu.fzhhl.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://new.52xcode.cn

[O03] 加锁保护共享数据
来源：http://mde.mhx1999.top

Py:   with lock: shared += 1
来源：http://abs.xuanzx.com

PHP:  // 用 flock() 做文件锁
来源：http://vyh.sjlbkw.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://aic.fzhhl.top

TS:   // 同 JS
来源：http://cet.jqgufenzy.top

Java: synchronized (this) { shared++; }
来源：http://jzq.jyoumei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://phk.guannengcc.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wxg.fzhhl.top

C#:   lock (gate) { shared++; }
来源：http://thc.yj202588.top

[O04] 定义异步函数并等待
来源：http://zpg.jlsjyb.cn

Py:   async def f():⏎    await g()
来源：http://sye.xziqi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eet.nwbrower.top

JS:   async function f() { await g(); }
来源：http://lus.sjlbkw.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fjt.chenzaomai.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://asl.xingfuxueyuan.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ndy.jinyuanbaomall.cn

Ruby: # 用 Fiber 或 async gem
来源：http://onz.jqgufenzy.top

C#:   async Task F() { await G(); }
来源：http://grt.sysykeji.top

[O05] 并发执行并等待全部完成
来源：http://cpi.dashuyun.cn

Py:   asyncio.gather(*tasks)
来源：http://nmg.dashuyun.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hat.tian-w.cn

JS:   await Promise.all(tasks)
来源：http://rqj.shanyushiyangkeji.top

TS:   await Promise.all(tasks)
来源：http://mvy.zhiwuduotai.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hcx.ydjk.org.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://emn.tianlin.xyz

Ruby: threads.map(&:join)
来源：http://yju.xingfuxueyuan.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://ajo.xingfuxueyuan.xyz

[O06] 使用进程池
来源：http://yym.cdnleiting.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uoq.cqqwz.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cmz.shanyushiyangkeji.top

JS:   // child_process / cluster 模块
来源：http://sdi.redwolf501.top

TS:   // child_process / cluster 模块
来源：http://okv.sxryk.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ipl.c1oappe.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://iag.meibo888.top

Ruby: // fork 块
来源：http://moy.tarul.cn

C#:   Parallel.For
来源：http://lts.shangyingyoupin.top

================================================================================
来源：http://yfx.gogol.net.cn

P. 常用工具函数
来源：http://iew.smart0.xyz

================================================================================
来源：http://fzx.daxiang520.top

[P01] 生成 UUID
来源：http://rki.xuetiantiany.cn

Py:   str(uuid.uuid4())
来源：http://qok.zhoulong.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qjn.epnwcf.com

JS:   crypto.randomUUID()
来源：http://efu.svipenyu.cn

TS:   crypto.randomUUID()
来源：http://kau.yueranfly.top

Java: UUID.randomUUID().toString()
来源：http://ldz.hnqzz.top

Go:   // 用 github.com/google/uuid
来源：http://tym.hammf.cn

Ruby: SecureRandom.uuid
来源：http://cuc.ywan-chungtsiang.top

C#:   Guid.NewGuid().ToString()
来源：http://cug.dianchejie.cn

[P02] MD5 / SHA256 摘要
来源：http://ypf.chenlongwang.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cqj.iojbl.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rcd.quarkkingdee.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://apk.jyoumei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uvq.aibaodan.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vkw.chenlongwang.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cto.jianghu66.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yxb.tanke756.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lci.52xcode.cn

[P03] 生成短随机字符串
来源：http://act.sufxvd.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uyu.gaohongyu789.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://khe.jinqigufen.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rri.yj20258888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gtc.quarkkingdee.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qmq.vqdsnc.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tgw.sufxvd.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rzk.aibaodan.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vhp.yueranfly.top

[P04] 求长度
来源：http://jqx.xziqi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zsx.dashuyun.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uxc.epnwcf.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yyu.quarkkingdee.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qep.hcnkem.com

Java: list.size();  map.size();  s.length()
来源：http://uor.jinghuilouyu.cn

Go:   len(arr);  len(m)
来源：http://ieg.guannengcc.top

Ruby: x.length;  x.size
来源：http://rvu.smart0.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://uph.fzhhl.top

[P05] 判断两个对象内容是否相等
来源：http://prq.dashuyun.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tqi.pycfn.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dcd.shuidangran.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xrc.yj20258888.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rqn.birdmap.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jae.chenjidiqi.icu

Go:   reflect.DeepEqual(a, b)
来源：http://ngd.birdmap.top

Ruby: a == b
来源：http://xtx.shangyingyoupin.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ipw.316326.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dsb.zhongyouzk.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lgh.gaohongyu789.top

PHP:  if (empty($x)) {}
来源：http://hop.havefunace.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fjz.jyoumei.cn

TS:   if (x == null) {}
来源：http://xyj.aizwys.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fet.yongpay.top

Go:   if x == nil {}
来源：http://srg.guowangkeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://atw.yonumen.top

C#:   if (x is null) {}
来源：http://rpc.ybcxt.top

[P07] 防抖与节流
来源：http://qbw.hcnkem.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wyb.zhijiandao.cn

PHP:  // 手写时间戳比较
来源：http://cay.redwolf501.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cmf.sweek.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tez.yj202588.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cgb.sysykeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hww.hnxiangtu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://cvq.fanxiaobao.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ykg.zhijiandao.cn

[P08] 处理浮点精度问题
来源：http://qsx.yueranfly.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hqu.fzhhl.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qqf.yvedp.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://djw.guannengcc.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yja.fehbvm.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xyh.hongshengwenyu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pps.sjlbkw.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ulo.xuanzx.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wfi.snrcjt.cn

================================================================================
来源：http://oho.yj202588.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cqn.tarul.cn

================================================================================
来源：http://eac.zdqjudy.top

[Q01] 创建表
来源：http://lmr.chenzaomai.com

CREATE TABLE users (
来源：http://myf.nwbrower.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://atx.zdbjq.cn

name VARCHAR(50) NOT NULL,
来源：http://mjx.yonumen.top

email VARCHAR(100) UNIQUE,
来源：http://hqp.9152youxi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://aml.jinghuilouyu.cn

);
来源：http://ypj.tianlin.xyz

[Q02] 创建带外键的表
来源：http://ykz.birdmap.top

CREATE TABLE orders (
来源：http://qzz.shangyingyoupin.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jzg.pycfn.com

user_id INT NOT NULL,
来源：http://gms.jinyuanbaomall.cn

amount DECIMAL(10, 2),
来源：http://klc.hnxiangtu.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vic.yfazqb.com

);
来源：http://eoi.yvedp.cn

[Q03] 增加列
来源：http://isw.sufxvd.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jco.sysykeji.top

[Q04] 修改列类型
来源：http://fdn.ivvv.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bjz.chenlongwang.top

[Q05] 重命名列
来源：http://qee.dashuyun.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ikh.chenlongwang.top

[Q06] 删除列
来源：http://rha.hesvh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://urz.bjfxy.top

[Q07] 删除表
来源：http://lxp.hongshengwenyu.top

DROP TABLE IF EXISTS orders;
来源：http://ttb.shangyingyoupin.top

[Q08] 创建普通索引
来源：http://fch.zhengqikj.top

CREATE INDEX idx_users_email ON users(email);
来源：http://cpp.yueranfly.top

[Q09] 创建唯一索引
来源：http://akb.jqgufenzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xdz.52xcode.cn

[Q10] 插入单行
来源：http://hrs.bjfxy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lud.cashguo.top

[Q11] 一次插入多行
来源：http://ibk.chenjidiqi.icu

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gur.ctjpmb.com

[Q12] 插入后取自增 ID
来源：http://vwk.zycfv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://zlo.yongpay.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qfc.daxiang520.top

[Q13] 忽略重复插入
来源：http://iwl.daria6918.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://led.ivvv.top

[Q14] 存在则更新（upsert）
来源：http://yjt.dashuyun.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://abk.yfazqb.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qsx.jinghuilouyu.cn

[Q15] 查询全部
来源：http://eky.cdnleiting.top

SELECT * FROM users;
来源：http://osr.shanyushiyangkeji.top

[Q16] 查询指定列
来源：http://ear.hongshengwenyu.top

SELECT id, name FROM users;
来源：http://kgh.gaohongyu789.top

[Q17] 条件查询
来源：http://xpn.52xcode.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vxo.fanxiaobao.xyz

[Q18] 模糊匹配
来源：http://ggn.daria6918.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cpk.xuetiantiany.cn

[Q19] 范围查询
来源：http://vmc.ydzc1.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mgu.yangfankeji.com

[Q20] IN 列表
来源：http://rlw.guannengcc.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mhp.ctjpmb.com

[Q21] 空值判断
来源：http://byq.ppjwa.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wur.yangfankeji.com

[Q22] 排序
来源：http://unx.cashguo.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nah.birdmap.top

[Q23] 分页
来源：http://mub.chenjidiqi.icu

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://aym.zhengqikj.top

[Q24] 去重
来源：http://zct.aibaodan.cn

SELECT DISTINCT city FROM users;
来源：http://sls.ppjwa.cn

[Q25] 只取前 N 条
来源：http://zhu.jinqigfzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://eer.jinghuilouyu.cn

[Q26] 计数
来源：http://lgr.xinyue.icu

SELECT COUNT(*) FROM users;
来源：http://qed.yj202588.top

[Q27] 条件计数
来源：http://jgu.hfpthk.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://puc.jinghuilouyu.cn

[Q28] 求和与平均
来源：http://weo.havefunace.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://njo.sjlbkw.cn

[Q29] 最大最小值
来源：http://dba.havefunace.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://bia.wangshuangyany.cn

[Q30] 分组统计
来源：http://jab.shuidangran.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lzz.shzxlz.cn

[Q31] 分组后过滤
来源：http://atg.yangfankeji.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://suk.nwbrower.top

[Q32] 分组拼接字符串
来源：http://zkw.zhixingplan.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ylu.yanxiufei.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://egx.jianghu66.top

[Q33] 多列分组
来源：http://ctx.cucudq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kfm.tian-w.cn

[Q34] 每组取第一条
来源：http://nyu.fengsongda.top

SELECT * FROM (
来源：http://opy.sweek.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://irc.daria6918.cn

) t WHERE rn = 1;
来源：http://mau.dashuyun.cn

[Q35] 内连接
来源：http://ytg.9152youxi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mur.daxiang520.top

[Q36] 左连接
来源：http://nyz.52xcode.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kmb.yuanzhike.top

[Q37] 右连接
来源：http://irg.xuetiantiany.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uvm.zhixingplan.top

[Q38] 全外连接（PostgreSQL）
来源：http://kei.yonumen.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rad.nwbrower.top

[Q39] 自连接（查上下级）
来源：http://zcq.jinyuanbaomall.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://udy.wangshuangyany.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nka.sjlbkw.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xux.cashguo.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://buz.yongpay.top

[Q41] 多表连接
来源：http://xtu.tanke756.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://bko.fanxiaobao.xyz

JOIN users u ON u.id = o.user_id
来源：http://psq.cheryme.top

JOIN products p ON p.id = o.product_id;
来源：http://klu.hnqzz.top

[Q42] 连接条件附加过滤
来源：http://fbu.c1oappe.top

SELECT u.name, o.amount FROM users u
来源：http://suc.ybcxt.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ujm.xuetiantiany.cn

[Q43] 标量子查询
来源：http://jls.ydjk.org.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mll.zdbjq.cn

[Q44] IN 子查询
来源：http://apv.zdbjq.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://afc.ywan-chungtsiang.top

[Q45] EXISTS 判断存在
来源：http://mnp.tian-w.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jeq.9152youxi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pij.jyoumei.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fzm.haohaochexian.top

[Q47] 与平均值比较
来源：http://zuf.zhixingplan.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qvm.chenjidiqi.icu

[Q48] CTE 公用表表达式
来源：http://gfz.jinqigfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://keh.ppjwa.cn

SELECT * FROM t WHERE c > 5;
来源：http://aab.nanxinkj.top

[Q49] 更新单行
来源：http://rjs.bbcook.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gsa.yj20258.top

[Q50] 批量更新
来源：http://dyk.pycfn.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gai.zhixingplan.top

[Q51] 用子查询更新
来源：http://btx.vqdsnc.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wzb.gogol.net.cn

[Q52] 删除指定行
来源：http://hri.chenlongwang.top

DELETE FROM users WHERE id = 10;
来源：http://duo.gzhubu.top

[Q53] 按条件删除
来源：http://lux.ydzc1.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qrv.fehbvm.com

[Q54] 清空表
来源：http://kvq.snrcjt.cn

TRUNCATE TABLE logs;
来源：http://nso.xylfe.cn

[Q55] 排名（并列占位）
来源：http://rxr.sxryk.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tzo.tanke756.top

[Q56] 密集排名（并列不占位）
来源：http://khf.havefunace.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ecs.sweek.top

[Q57] 行号
来源：http://lmd.hnqzz.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qzk.jlsjyb.cn

[Q58] 累计求和
来源：http://zlz.yueranfly.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zad.cdnleiting.top

[Q59] 分组内累计
来源：http://ucm.quarkkingdee.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vkr.fktsv.cn

[Q60] 取上一行 / 下一行
来源：http://xcr.zhongyouzk.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bop.yj202588.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nod.chenlongwang.top


<!-- 参考信息 -->