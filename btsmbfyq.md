代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vxl.yvedp.cn

[N10] 链表节点定义
来源：http://sqq.fehbvm.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pie.havefunace.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ill.dashuyun.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cum.havefunace.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kjf.jinyuanbaomall.cn

Java: class Node { int v; Node next; }
来源：http://qqg.hcnkem.com

Go:   type Node struct { V int; Next *Node }
来源：http://xio.uphjek.com

Ruby: Node = Struct.new(:v, :next)
来源：http://cln.haohaochexian.top

C#:   class Node { public int V; public Node? Next; }
来源：http://pmk.gotoacloud.top

[N11] 二叉树中序遍历
来源：http://zgb.zhiwuduotai.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tgq.yj202588.top

PHP:  // 手写递归函数
来源：http://vcf.zhongyouzk.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vdg.yj20258888.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://voy.ctjpmb.com

Java: // 手写递归
来源：http://kys.daria6918.cn

Go:   // 手写递归
来源：http://yfs.jinqigfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vmx.smart0.xyz

C#:   // 手写递归
来源：http://gce.cdnleiting.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nlm.yuxming.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ftm.hongshengwenyu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cbv.zdbjq.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hrb.dianchejie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://keu.hnqzz.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gil.fehbvm.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hmy.ivvv.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gzi.nwbrower.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hoa.yj20258888.top

================================================================================
来源：http://dlk.bbcook.cn

O. 并发与异步
来源：http://hhh.mhx1999.top

================================================================================
来源：http://tis.yonumen.top

[O01] 启动一个线程
来源：http://luy.snrcjt.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qkm.xinyue.icu

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xbm.cdnleiting.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uve.xuetiantiany.cn

TS:   // 同 JS
来源：http://atk.bbcook.cn

Java: new Thread(() -> f()).start()
来源：http://wuk.zhaomingkeji.xyz

Go:   go f()
来源：http://cia.tian-w.cn

Ruby: Thread.new { f }
来源：http://gmu.mhx1999.top

C#:   Task.Run(() => F());
来源：http://vwe.smart0.xyz

[O02] 使用线程池
来源：http://nny.fengsongda.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eez.zhengqikj.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pox.yonumen.top

JS:   // worker_threads 线程池
来源：http://poc.fanxiaobao.xyz

TS:   // worker_threads 线程池
来源：http://zcy.hammf.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ghv.xylfe.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ejh.hnxiangtu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hif.ppjwa.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ujf.ydjk.org.cn

[O03] 加锁保护共享数据
来源：http://xdy.ybcxt.top

Py:   with lock: shared += 1
来源：http://pjc.svipenyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://sfy.snrcjt.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xbr.ydjk.org.cn

TS:   // 同 JS
来源：http://ltm.ybcxt.top

Java: synchronized (this) { shared++; }
来源：http://pgn.jyoumei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dca.shangyingyoupin.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://mam.uphjek.com

C#:   lock (gate) { shared++; }
来源：http://yum.yuanzhike.top

[O04] 定义异步函数并等待
来源：http://glr.fzhhl.top

Py:   async def f():⏎    await g()
来源：http://xzn.zhaomingkeji.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fgg.dashuyun.cn

JS:   async function f() { await g(); }
来源：http://qxd.daxiang520.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://btk.cashguo.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sci.chenzaomai.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jkk.fzhhl.top

Ruby: # 用 Fiber 或 async gem
来源：http://qza.fktsv.cn

C#:   async Task F() { await G(); }
来源：http://ejb.sxryk.cn

[O05] 并发执行并等待全部完成
来源：http://egq.daria6918.cn

Py:   asyncio.gather(*tasks)
来源：http://qij.sweek.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bmn.jinyuanbaomall.cn

JS:   await Promise.all(tasks)
来源：http://phq.cqqwz.cn

TS:   await Promise.all(tasks)
来源：http://jex.birdmap.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nvn.tarul.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://drx.hcnkem.com

Ruby: threads.map(&:join)
来源：http://yfk.52xcode.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zdz.meibo888.top

[O06] 使用进程池
来源：http://ltm.jlsjyb.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xuq.guannengcc.top

PHP:  // pcntl_fork 或多进程队列
来源：http://gqy.bjfxy.top

JS:   // child_process / cluster 模块
来源：http://mdd.pengpengdd.cyou

TS:   // child_process / cluster 模块
来源：http://jum.cucudq.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ynq.jinghuilouyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uii.zdbjq.cn

Ruby: // fork 块
来源：http://sgr.yuxming.cn

C#:   Parallel.For
来源：http://xuj.sxryk.cn

================================================================================
来源：http://udc.tarul.cn

P. 常用工具函数
来源：http://rtx.zhoulong.xyz

================================================================================
来源：http://gpw.jqgufenzy.top

[P01] 生成 UUID
来源：http://zej.redwolf501.top

Py:   str(uuid.uuid4())
来源：http://nbs.cqqwz.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ugo.aizwys.cn

JS:   crypto.randomUUID()
来源：http://mvd.nanxuanxn.top

TS:   crypto.randomUUID()
来源：http://hek.jlsjyb.cn

Java: UUID.randomUUID().toString()
来源：http://nxu.pycfn.com

Go:   // 用 github.com/google/uuid
来源：http://vvj.vqdsnc.cn

Ruby: SecureRandom.uuid
来源：http://ylf.bbcook.cn

C#:   Guid.NewGuid().ToString()
来源：http://knr.gzhubu.top

[P02] MD5 / SHA256 摘要
来源：http://mnf.aizwys.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hkq.nanxinkj.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ama.jinghuilouyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mgd.hywenlv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rem.yj20258888.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vzt.smart0.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lmh.mhx1999.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://isk.nwbrower.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://onc.fktsv.cn

[P03] 生成短随机字符串
来源：http://zyf.zhoulong.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kke.nanxuanxn.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pgp.gaohongyu789.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jid.fktsv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iwy.snrcjt.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vkw.jinqigfzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://inm.yj202588.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://bom.mhx1999.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ewj.fktsv.cn

[P04] 求长度
来源：http://nie.jqgufenzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://chf.c1oappe.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://muw.52xcode.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zfb.hcnkem.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mkn.ydjk.org.cn

Java: list.size();  map.size();  s.length()
来源：http://xmy.hesvh.cn

Go:   len(arr);  len(m)
来源：http://iga.fengsongda.top

Ruby: x.length;  x.size
来源：http://lkt.xingfuxueyuan.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://hwd.jinqigufen.top

[P05] 判断两个对象内容是否相等
来源：http://oyj.gaohongyu789.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://yoa.tian-w.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cfh.hammf.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dlz.bbcook.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fgk.jlsjyb.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://iro.ywan-chungtsiang.top

Go:   reflect.DeepEqual(a, b)
来源：http://tvt.ivvv.top

Ruby: a == b
来源：http://def.hnxiangtu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jsb.hnxiangtu.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://plz.fengsongda.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dub.shanyushiyangkeji.top

PHP:  if (empty($x)) {}
来源：http://twe.quarkkingdee.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xkf.gaohongyu789.top

TS:   if (x == null) {}
来源：http://txf.tanke756.top

Java: if (x == null || x.isEmpty()) {}
来源：http://vok.mhx1999.top

Go:   if x == nil {}
来源：http://woc.tarul.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lka.gaohongyu789.top

C#:   if (x is null) {}
来源：http://chk.jianghu66.top

[P07] 防抖与节流
来源：http://llg.jlsjyb.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sjp.xziqi.cn

PHP:  // 手写时间戳比较
来源：http://hue.ywan-chungtsiang.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://urj.jqgufenzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wrv.shanyushiyangtech.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zah.tarul.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://quv.jqgufenzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zhh.yj202588.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://aza.aibaodan.cn

[P08] 处理浮点精度问题
来源：http://rrw.sufxvd.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://oeg.vqdsnc.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ifx.0kj1m.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bgv.jinqigfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://suq.quarkkingdee.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://toz.meibo888.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nga.redwolf501.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mzi.wangshuangyany.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uuu.jinghuilouyu.cn

================================================================================
来源：http://bfd.jinghuilouyu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lie.hnqzz.top

================================================================================
来源：http://dkw.yangfankeji.com

[Q01] 创建表
来源：http://uyq.zhiwuduotai.top

CREATE TABLE users (
来源：http://zlc.52xcode.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lob.tianlin.xyz

name VARCHAR(50) NOT NULL,
来源：http://cav.yj20258.top

email VARCHAR(100) UNIQUE,
来源：http://pai.sysykeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wkk.jqgfzy.top

);
来源：http://yxt.sxryk.cn

[Q02] 创建带外键的表
来源：http://qcf.epnwcf.com

CREATE TABLE orders (
来源：http://ofd.xuanzx.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mzz.ivvv.top

user_id INT NOT NULL,
来源：http://azu.redwolf501.top

amount DECIMAL(10, 2),
来源：http://hzc.guowangkeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ryq.chenzaomai.com

);
来源：http://ceo.fanxiaobao.xyz

[Q03] 增加列
来源：http://gpv.ppjwa.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vjf.hfpthk.cn

[Q04] 修改列类型
来源：http://pkh.vehdjk.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://see.zdqjudy.top

[Q05] 重命名列
来源：http://ixi.cashguo.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://osx.meibo888.top

[Q06] 删除列
来源：http://qzg.jianghu66.top

ALTER TABLE users DROP COLUMN age;
来源：http://kex.nanxinkj.top

[Q07] 删除表
来源：http://rti.haohaochexian.top

DROP TABLE IF EXISTS orders;
来源：http://bco.shanyushiyangkeji.top

[Q08] 创建普通索引
来源：http://kgu.chenlongwang.top

CREATE INDEX idx_users_email ON users(email);
来源：http://hau.ydzc1.top

[Q09] 创建唯一索引
来源：http://ffn.ppjwa.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://unm.dianchejie.cn

[Q10] 插入单行
来源：http://jrk.zhixingplan.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ekz.hnxiangtu.top

[Q11] 一次插入多行
来源：http://poe.xziqi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ots.havefunace.top

[Q12] 插入后取自增 ID
来源：http://rkb.ydzc1.top

INSERT INTO users (name) VALUES ('C');
来源：http://gwz.tanke756.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oxw.316326.xyz

[Q13] 忽略重复插入
来源：http://flw.yvedp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rny.fzhhl.top

[Q14] 存在则更新（upsert）
来源：http://ulb.ivvv.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bfi.jyoumei.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dhj.cheryme.top

[Q15] 查询全部
来源：http://hfn.dashuyun.cn

SELECT * FROM users;
来源：http://guh.yangfankeji.com

[Q16] 查询指定列
来源：http://ovi.bjfxy.top

SELECT id, name FROM users;
来源：http://wga.cashguo.top

[Q17] 条件查询
来源：http://nki.hesvh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rkm.jiagoushi.top

[Q18] 模糊匹配
来源：http://dto.fengsongda.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://eeo.xinyue.icu

[Q19] 范围查询
来源：http://qzn.tianlin.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kdf.chenlongwang.top

[Q20] IN 列表
来源：http://wqh.zhoulong.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lyu.feifeiyinyue.top

[Q21] 空值判断
来源：http://mys.fengsongda.top

SELECT * FROM users WHERE email IS NULL;
来源：http://quz.nanxuanxn.top

[Q22] 排序
来源：http://aeh.daria6918.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://huv.redwolf501.top

[Q23] 分页
来源：http://oqu.zdbjq.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://trz.ivvv.top

[Q24] 去重
来源：http://cjv.quarkkingdee.top

SELECT DISTINCT city FROM users;
来源：http://kkq.jinqigfzy.top

[Q25] 只取前 N 条
来源：http://tsv.andypj.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ahp.yuanzhike.top

[Q26] 计数
来源：http://ifc.cheryme.top

SELECT COUNT(*) FROM users;
来源：http://vvh.pycfn.com

[Q27] 条件计数
来源：http://utx.sjlbkw.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dqd.jlsjyb.cn

[Q28] 求和与平均
来源：http://vcr.pycfn.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://seh.aizwys.cn

[Q29] 最大最小值
来源：http://rsr.cheryme.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://mfi.yanxiufei.cn

[Q30] 分组统计
来源：http://xjg.ydjk.org.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://utx.gotoacloud.top

[Q31] 分组后过滤
来源：http://stl.uphjek.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://eno.52xcode.cn

[Q32] 分组拼接字符串
来源：http://oiz.svipenyu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rew.wangshuangyany.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uyl.nanxinkj.top

[Q33] 多列分组
来源：http://hkv.shanyushiyangkeji.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hvv.sweek.top

[Q34] 每组取第一条
来源：http://sik.yangfankeji.com

SELECT * FROM (
来源：http://rth.yangfankeji.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ghe.shuidangran.top

) t WHERE rn = 1;
来源：http://htq.jiagoushi.top

[Q35] 内连接
来源：http://lgh.havefunace.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zmn.shanyushiyangkeji.top

[Q36] 左连接
来源：http://qjf.fengsongda.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zpg.yanxiufei.cn

[Q37] 右连接
来源：http://fol.ppjwa.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://umx.jiagoushi.top

[Q38] 全外连接（PostgreSQL）
来源：http://yvs.zhongyouzk.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://acm.yangfankeji.com

[Q39] 自连接（查上下级）
来源：http://kbx.zhixingplan.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://dhy.tian-w.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rkw.c1oappe.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zee.jianghu66.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lgc.aizwys.cn

[Q41] 多表连接
来源：http://hih.ydzc1.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://mxe.bjfxy.top

JOIN users u ON u.id = o.user_id
来源：http://rvj.ydjk.org.cn

JOIN products p ON p.id = o.product_id;
来源：http://vsl.mhx1999.top

[Q42] 连接条件附加过滤
来源：http://jyk.cdnleiting.top

SELECT u.name, o.amount FROM users u
来源：http://pnr.quarkkingdee.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ekj.tianlin.xyz

[Q43] 标量子查询
来源：http://orc.iojbl.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rth.jlsjyb.cn

[Q44] IN 子查询
来源：http://als.cqqwz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hne.iojbl.cn

[Q45] EXISTS 判断存在
来源：http://hul.guowangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fyy.aibaodan.cn

[Q46] NOT EXISTS 判断不存在
来源：http://oie.tianlin.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://phf.zhijiandao.cn

[Q47] 与平均值比较
来源：http://pup.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tcu.hywenlv.cn

[Q48] CTE 公用表表达式
来源：http://lzh.yueranfly.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uey.gzhubu.top

SELECT * FROM t WHERE c > 5;
来源：http://rqb.pengpengdd.cyou

[Q49] 更新单行
来源：http://fxq.gzhubu.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dtd.zhaomingkeji.xyz

[Q50] 批量更新
来源：http://ila.fzhhl.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dcg.tanke756.top

[Q51] 用子查询更新
来源：http://ota.cdnleiting.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://tcq.guowangkeji.top

[Q52] 删除指定行
来源：http://olp.daria6918.cn

DELETE FROM users WHERE id = 10;
来源：http://lbr.iojbl.cn

[Q53] 按条件删除
来源：http://pep.zhijiandao.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tyi.zhaomingkeji.xyz

[Q54] 清空表
来源：http://erz.vehdjk.com

TRUNCATE TABLE logs;
来源：http://apb.hfpthk.cn

[Q55] 排名（并列占位）
来源：http://oqr.fengsongda.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xzt.9152youxi.cn

[Q56] 密集排名（并列不占位）
来源：http://ntd.yangfankeji.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vew.dianchejie.cn

[Q57] 行号
来源：http://zhl.shzxlz.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gwz.smart0.xyz

[Q58] 累计求和
来源：http://paa.aibaodan.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hqu.sufxvd.cn

[Q59] 分组内累计
来源：http://ekf.daxiang520.top


<!-- 参考信息 -->