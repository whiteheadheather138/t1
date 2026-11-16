代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wyx.hesvh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qqv.iojbl.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dyz.hcnkem.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xsw.tian-w.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mhf.nwbrower.top

[N10] 链表节点定义
来源：http://irq.jianghu66.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://czg.zdqjudy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ssi.snrcjt.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://aji.xuetiantiany.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wdr.vqdsnc.cn

Java: class Node { int v; Node next; }
来源：http://ejy.chenjidiqi.icu

Go:   type Node struct { V int; Next *Node }
来源：http://bmk.fktsv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ame.gotoacloud.top

C#:   class Node { public int V; public Node? Next; }
来源：http://rrs.zdbjq.cn

[N11] 二叉树中序遍历
来源：http://dnp.hnqzz.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wgp.yj20258.top

PHP:  // 手写递归函数
来源：http://cix.daxiang520.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kkz.kuanghao11.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yom.zhiwuduotai.top

Java: // 手写递归
来源：http://stx.hammf.cn

Go:   // 手写递归
来源：http://ksk.havefunace.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jfs.daria6918.cn

C#:   // 手写递归
来源：http://eeu.tian-w.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gml.aizwys.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iye.c1oappe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ats.ywan-chungtsiang.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vnd.yfazqb.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fhk.fktsv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ofk.yj20258888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wuk.ydzc1.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xpk.xuanzx.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lqh.sxryk.cn

================================================================================
来源：http://sdc.mhx1999.top

O. 并发与异步
来源：http://hjf.xylfe.cn

================================================================================
来源：http://mhn.fzhhl.top

[O01] 启动一个线程
来源：http://dei.dianchejie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zeb.xuetiantiany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nsa.epnwcf.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://oan.bbcook.cn

TS:   // 同 JS
来源：http://lvb.xinyue.icu

Java: new Thread(() -> f()).start()
来源：http://xmr.52xcode.cn

Go:   go f()
来源：http://kck.shuidangran.top

Ruby: Thread.new { f }
来源：http://pkt.guowangkeji.top

C#:   Task.Run(() => F());
来源：http://xul.sufxvd.cn

[O02] 使用线程池
来源：http://lmn.yfazqb.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wxw.ppjwa.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qyd.gogol.net.cn

JS:   // worker_threads 线程池
来源：http://efd.sweek.top

TS:   // worker_threads 线程池
来源：http://gbc.yvedp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rez.xylfe.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jgg.dashuyun.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mwb.cqqwz.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vwj.52xcode.cn

[O03] 加锁保护共享数据
来源：http://kfs.pycfn.com

Py:   with lock: shared += 1
来源：http://zcu.wangdashe.top

PHP:  // 用 flock() 做文件锁
来源：http://smr.xuanzx.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://foh.guannengcc.top

TS:   // 同 JS
来源：http://haf.snrcjt.cn

Java: synchronized (this) { shared++; }
来源：http://omc.havefunace.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://imv.9152youxi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kbc.fzhhl.top

C#:   lock (gate) { shared++; }
来源：http://oqm.daria6918.cn

[O04] 定义异步函数并等待
来源：http://cek.xylfe.cn

Py:   async def f():⏎    await g()
来源：http://aue.hnxiangtu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pvh.zhixingplan.top

JS:   async function f() { await g(); }
来源：http://tqz.ybcxt.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://mwx.316326.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ite.yj20258.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mrr.vehdjk.com

Ruby: # 用 Fiber 或 async gem
来源：http://tbw.nanxinkj.top

C#:   async Task F() { await G(); }
来源：http://anm.jinqigufen.top

[O05] 并发执行并等待全部完成
来源：http://xca.zhijiandao.cn

Py:   asyncio.gather(*tasks)
来源：http://cuz.zhixingplan.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://owg.yanxiufei.cn

JS:   await Promise.all(tasks)
来源：http://mih.xuanzx.com

TS:   await Promise.all(tasks)
来源：http://lmm.gaohongyu789.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nol.hesvh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fdg.cheryme.top

Ruby: threads.map(&:join)
来源：http://yzg.dashuyun.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://put.iojbl.cn

[O06] 使用进程池
来源：http://ytu.cucudq.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kiz.xinyue.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://mjr.dianchejie.cn

JS:   // child_process / cluster 模块
来源：http://bze.ydjk.org.cn

TS:   // child_process / cluster 模块
来源：http://kjf.svipenyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://msl.ydzc1.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tdd.hfpthk.cn

Ruby: // fork 块
来源：http://ssu.hywenlv.cn

C#:   Parallel.For
来源：http://hgc.epnwcf.com

================================================================================
来源：http://gmq.redwolf501.top

P. 常用工具函数
来源：http://ulb.hcnkem.com

================================================================================
来源：http://cik.fzhhl.top

[P01] 生成 UUID
来源：http://olg.cqqwz.cn

Py:   str(uuid.uuid4())
来源：http://rut.bjfxy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ggs.jinqigfzy.top

JS:   crypto.randomUUID()
来源：http://qea.guannengcc.top

TS:   crypto.randomUUID()
来源：http://gca.fanxiaobao.xyz

Java: UUID.randomUUID().toString()
来源：http://pdz.zhijiandao.cn

Go:   // 用 github.com/google/uuid
来源：http://ffl.svipenyu.cn

Ruby: SecureRandom.uuid
来源：http://asf.9152youxi.cn

C#:   Guid.NewGuid().ToString()
来源：http://kcp.0kj1m.cn

[P02] MD5 / SHA256 摘要
来源：http://xng.fanxiaobao.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kwv.52xcode.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mil.hcnkem.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fio.vehdjk.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ysq.zhongyouzk.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ppd.nwbrower.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pzd.xuanzx.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uqp.daria6918.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wui.aizwys.cn

[P03] 生成短随机字符串
来源：http://zsd.guowangkeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zxj.hywenlv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pzq.nwbrower.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ycq.shangyingyoupin.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vcv.gogol.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qcr.chenlongwang.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://eha.kuanghao11.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ski.andypj.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qso.yvedp.cn

[P04] 求长度
来源：http://hne.gzhubu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tvw.hcnkem.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hus.0kj1m.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://epw.xingfuxueyuan.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://teh.havefunace.top

Java: list.size();  map.size();  s.length()
来源：http://gjx.sysykeji.top

Go:   len(arr);  len(m)
来源：http://lot.yj202588.top

Ruby: x.length;  x.size
来源：http://sjf.zhaomingkeji.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://ixd.epnwcf.com

[P05] 判断两个对象内容是否相等
来源：http://ius.fengsongda.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://orp.hcnkem.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ovr.yongpay.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gph.fehbvm.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vjf.ppjwa.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://svi.guannengcc.top

Go:   reflect.DeepEqual(a, b)
来源：http://zsc.hnxiangtu.top

Ruby: a == b
来源：http://fmj.xziqi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qwi.zhaomingkeji.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://snk.mhx1999.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rsk.guannengcc.top

PHP:  if (empty($x)) {}
来源：http://ubf.cashguo.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zrs.jqgfzy.top

TS:   if (x == null) {}
来源：http://ndx.yanxiufei.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zad.sjlbkw.cn

Go:   if x == nil {}
来源：http://rzf.feifeiyinyue.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hzx.xingfuxueyuan.xyz

C#:   if (x is null) {}
来源：http://tnp.pengpengdd.cyou

[P07] 防抖与节流
来源：http://oex.c1oappe.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rmy.yonumen.top

PHP:  // 手写时间戳比较
来源：http://pqp.fehbvm.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ntb.tanke756.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yyq.havefunace.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://eex.zhengqikj.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hnx.gogol.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vva.hongshengwenyu.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pii.zhoulong.xyz

[P08] 处理浮点精度问题
来源：http://zue.52xcode.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yzd.0kj1m.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hic.jinqigfzy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wqr.yongpay.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rip.gzhubu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wnn.jlsjyb.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gjn.guannengcc.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ltw.wangshuangyany.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zfe.nwbrower.top

================================================================================
来源：http://eky.jlsjyb.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ysy.jqgfzy.top

================================================================================
来源：http://bqb.chenzaomai.com

[Q01] 创建表
来源：http://rjh.zdbjq.cn

CREATE TABLE users (
来源：http://dyp.gotoacloud.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qwo.jianghu66.top

name VARCHAR(50) NOT NULL,
来源：http://uis.nanxinkj.top

email VARCHAR(100) UNIQUE,
来源：http://lxt.fzhhl.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nsr.aizwys.cn

);
来源：http://gsx.c1oappe.top

[Q02] 创建带外键的表
来源：http://gaa.ctjpmb.com

CREATE TABLE orders (
来源：http://plu.tanke756.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fua.zhixingplan.top

user_id INT NOT NULL,
来源：http://rpn.pycfn.com

amount DECIMAL(10, 2),
来源：http://jbz.sufxvd.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://muv.meibo888.top

);
来源：http://phw.fengsongda.top

[Q03] 增加列
来源：http://uqm.hfpthk.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tud.cashguo.top

[Q04] 修改列类型
来源：http://xep.ehwqpu.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ibj.gzhubu.top

[Q05] 重命名列
来源：http://koe.snrcjt.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rap.yuxming.cn

[Q06] 删除列
来源：http://jtc.cheryme.top

ALTER TABLE users DROP COLUMN age;
来源：http://xyo.yueranfly.top

[Q07] 删除表
来源：http://dsh.jinghuilouyu.cn

DROP TABLE IF EXISTS orders;
来源：http://bcm.birdmap.top

[Q08] 创建普通索引
来源：http://hme.sjlbkw.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hip.yueranfly.top

[Q09] 创建唯一索引
来源：http://yzf.fktsv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zlw.xingfuxueyuan.xyz

[Q10] 插入单行
来源：http://eyw.havefunace.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bwl.ehwqpu.com

[Q11] 一次插入多行
来源：http://nga.gotoacloud.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://idd.jinqigfzy.top

[Q12] 插入后取自增 ID
来源：http://jep.hfpthk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://nab.gaohongyu789.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jsd.smart0.xyz

[Q13] 忽略重复插入
来源：http://ial.zdqjudy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ozt.chenlongwang.top

[Q14] 存在则更新（upsert）
来源：http://zfz.yueranfly.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://znm.vqdsnc.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vpx.yanxiufei.cn

[Q15] 查询全部
来源：http://lhx.epnwcf.com

SELECT * FROM users;
来源：http://sgi.dianchejie.cn

[Q16] 查询指定列
来源：http://xmr.haohaochexian.top

SELECT id, name FROM users;
来源：http://nfi.cdnleiting.top

[Q17] 条件查询
来源：http://ghm.pengpengdd.cyou

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rtz.52xcode.cn

[Q18] 模糊匹配
来源：http://rlm.jinyuanbaomall.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yfl.yongpay.top

[Q19] 范围查询
来源：http://syk.c1oappe.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xej.yonumen.top

[Q20] IN 列表
来源：http://raw.andypj.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ajo.feifeiyinyue.top

[Q21] 空值判断
来源：http://dvg.mhx1999.top

SELECT * FROM users WHERE email IS NULL;
来源：http://gex.shanyushiyangtech.top

[Q22] 排序
来源：http://aef.wangdashe.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ucs.fengsongda.top

[Q23] 分页
来源：http://uiz.sysykeji.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zcp.sysykeji.top

[Q24] 去重
来源：http://irh.ctjpmb.com

SELECT DISTINCT city FROM users;
来源：http://dew.yvedp.cn

[Q25] 只取前 N 条
来源：http://mzc.xingfuxueyuan.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fpj.epnwcf.com

[Q26] 计数
来源：http://nus.jlsjyb.cn

SELECT COUNT(*) FROM users;
来源：http://did.jyoumei.cn

[Q27] 条件计数
来源：http://vjz.hywenlv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uhz.yonumen.top

[Q28] 求和与平均
来源：http://fxr.nanxuanxn.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bsw.tarul.cn

[Q29] 最大最小值
来源：http://uje.yongpay.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://hhj.aizwys.cn

[Q30] 分组统计
来源：http://pib.smart0.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qjy.quarkkingdee.top

[Q31] 分组后过滤
来源：http://xif.quarkkingdee.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://juc.zhoulong.xyz

[Q32] 分组拼接字符串
来源：http://gvc.fzhhl.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nqj.yuxming.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ydx.cucudq.cn

[Q33] 多列分组
来源：http://tlf.yonumen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fre.feifeiyinyue.top

[Q34] 每组取第一条
来源：http://mhd.yonumen.top

SELECT * FROM (
来源：http://hkr.hesvh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://iwj.meibo888.top

) t WHERE rn = 1;
来源：http://zpc.pycfn.com

[Q35] 内连接
来源：http://vii.tian-w.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rbt.fanxiaobao.xyz

[Q36] 左连接
来源：http://pgw.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mth.jyoumei.cn

[Q37] 右连接
来源：http://fox.jinyuanbaomall.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ort.zhiwuduotai.top

[Q38] 全外连接（PostgreSQL）
来源：http://bpl.xinyue.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qqr.gogol.net.cn

[Q39] 自连接（查上下级）
来源：http://rrw.zhaomingkeji.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://bzy.tian-w.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wjc.gotoacloud.top

[Q40] 交叉连接（笛卡尔积）
来源：http://tgr.52xcode.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dfn.yvedp.cn

[Q41] 多表连接
来源：http://kvf.vehdjk.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://uat.xziqi.cn

JOIN users u ON u.id = o.user_id
来源：http://pmw.daxiang520.top

JOIN products p ON p.id = o.product_id;
来源：http://oqj.jyoumei.cn

[Q42] 连接条件附加过滤
来源：http://raf.ehwqpu.com

SELECT u.name, o.amount FROM users u
来源：http://oax.52xcode.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hvy.sweek.top

[Q43] 标量子查询
来源：http://hxl.fktsv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mqf.fengsongda.top

[Q44] IN 子查询
来源：http://pqi.ppjwa.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bre.zhongyouzk.top

[Q45] EXISTS 判断存在
来源：http://fsb.yj202588.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cwi.cashguo.top

[Q46] NOT EXISTS 判断不存在
来源：http://ngs.aibaodan.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fdc.jlsjyb.cn

[Q47] 与平均值比较
来源：http://odt.zhengqikj.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://juc.nwbrower.top

[Q48] CTE 公用表表达式
来源：http://xpu.meibo888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jdy.sweek.top

SELECT * FROM t WHERE c > 5;
来源：http://etk.tian-w.cn

[Q49] 更新单行
来源：http://ays.fehbvm.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hno.c1oappe.top

[Q50] 批量更新
来源：http://qjp.sweek.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gyo.yuxming.cn

[Q51] 用子查询更新
来源：http://hib.tarul.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cwq.yj202588.top

[Q52] 删除指定行
来源：http://etx.pycfn.com

DELETE FROM users WHERE id = 10;
来源：http://efb.hfpthk.cn

[Q53] 按条件删除
来源：http://uhn.cashguo.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jsa.yuanzhike.top

[Q54] 清空表
来源：http://uyt.snrcjt.cn

TRUNCATE TABLE logs;
来源：http://zqh.cdnleiting.top

[Q55] 排名（并列占位）
来源：http://rty.yongpay.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mel.pengpengdd.cyou

[Q56] 密集排名（并列不占位）
来源：http://kqp.jianghu66.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xob.zhoulong.xyz

[Q57] 行号
来源：http://jsb.guannengcc.top


<!-- 参考信息 -->