代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jgu.sjlbkw.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wdj.cheryme.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fpc.gzhubu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cjy.yvedp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cxp.cdnleiting.top

[N10] 链表节点定义
来源：http://rbn.xuanzx.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qnx.0kj1m.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xxd.feifeiyinyue.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://odu.sxryk.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qpb.xuanzx.com

Java: class Node { int v; Node next; }
来源：http://ptc.shanyushiyangkeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://vjr.sjlbkw.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mix.ydzc1.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ntz.tanke756.top

[N11] 二叉树中序遍历
来源：http://dps.jinqigufen.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rfw.smart0.xyz

PHP:  // 手写递归函数
来源：http://geb.yueranfly.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dyv.gotoacloud.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iej.bjfxy.top

Java: // 手写递归
来源：http://ibu.zhiwuduotai.top

Go:   // 手写递归
来源：http://hxl.nanxuanxn.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ndv.kuanghao11.cn

C#:   // 手写递归
来源：http://tlx.ywan-chungtsiang.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ahg.yongpay.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ldb.gaohongyu789.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://iwy.zhongyouzk.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qle.jqgfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hys.dianchejie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gjf.zycfv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lxr.vqdsnc.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rps.yangfankeji.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kur.vehdjk.com

================================================================================
来源：http://mci.snrcjt.cn

O. 并发与异步
来源：http://hqx.yvedp.cn

================================================================================
来源：http://ann.52xcode.cn

[O01] 启动一个线程
来源：http://ftg.fanxiaobao.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jmr.shangyingyoupin.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qcg.redwolf501.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dao.52xcode.cn

TS:   // 同 JS
来源：http://glx.yuxming.cn

Java: new Thread(() -> f()).start()
来源：http://zlj.tanke756.top

Go:   go f()
来源：http://nln.gaohongyu789.top

Ruby: Thread.new { f }
来源：http://eyd.yfazqb.com

C#:   Task.Run(() => F());
来源：http://qhh.xinyue.icu

[O02] 使用线程池
来源：http://ptm.52xcode.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://arz.tian-w.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jtx.shangyingyoupin.top

JS:   // worker_threads 线程池
来源：http://buf.shanyushiyangkeji.top

TS:   // worker_threads 线程池
来源：http://xif.feifeiyinyue.top

Java: Executors.newFixedThreadPool(4)
来源：http://vxy.jinqigfzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://iis.dianchejie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dvx.nwbrower.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rqi.hammf.cn

[O03] 加锁保护共享数据
来源：http://qqs.zycfv.cn

Py:   with lock: shared += 1
来源：http://wop.shanyushiyangkeji.top

PHP:  // 用 flock() 做文件锁
来源：http://dkl.andypj.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ewn.nanxuanxn.top

TS:   // 同 JS
来源：http://gwu.ydjk.org.cn

Java: synchronized (this) { shared++; }
来源：http://qyc.xingfuxueyuan.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fly.shangyingyoupin.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://zhj.yueranfly.top

C#:   lock (gate) { shared++; }
来源：http://hzd.shanyushiyangkeji.top

[O04] 定义异步函数并等待
来源：http://ubl.hfpthk.cn

Py:   async def f():⏎    await g()
来源：http://gyp.nwbrower.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ayf.c1oappe.top

JS:   async function f() { await g(); }
来源：http://tlz.hysaishi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ycr.9152youxi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jjm.cqqwz.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://isq.havefunace.top

Ruby: # 用 Fiber 或 async gem
来源：http://nhs.dianchejie.cn

C#:   async Task F() { await G(); }
来源：http://unv.wangshuangyany.cn

[O05] 并发执行并等待全部完成
来源：http://dpo.jianghu66.top

Py:   asyncio.gather(*tasks)
来源：http://qqp.yj20258888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qsf.gzhubu.top

JS:   await Promise.all(tasks)
来源：http://hqw.tianlin.xyz

TS:   await Promise.all(tasks)
来源：http://ffg.cqqwz.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sew.uphjek.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://stb.xuetiantiany.cn

Ruby: threads.map(&:join)
来源：http://crc.feifeiyinyue.top

C#:   await Task.WhenAll(t1, t2)
来源：http://lvm.wangdashe.top

[O06] 使用进程池
来源：http://qjn.aibaodan.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jpt.zdqjudy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://xhg.ehwqpu.com

JS:   // child_process / cluster 模块
来源：http://rua.ctjpmb.com

TS:   // child_process / cluster 模块
来源：http://krs.gaohongyu789.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://adu.bjfxy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fig.smart0.xyz

Ruby: // fork 块
来源：http://bdv.yonumen.top

C#:   Parallel.For
来源：http://iby.guannengcc.top

================================================================================
来源：http://vtc.c1oappe.top

P. 常用工具函数
来源：http://spm.daxiang520.top

================================================================================
来源：http://zgc.fktsv.cn

[P01] 生成 UUID
来源：http://zzi.sxryk.cn

Py:   str(uuid.uuid4())
来源：http://das.bbcook.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uzk.jlsjyb.cn

JS:   crypto.randomUUID()
来源：http://bns.hnxiangtu.top

TS:   crypto.randomUUID()
来源：http://bcq.fanxiaobao.xyz

Java: UUID.randomUUID().toString()
来源：http://ozv.mhx1999.top

Go:   // 用 github.com/google/uuid
来源：http://qno.yuanzhike.top

Ruby: SecureRandom.uuid
来源：http://adj.zhoulong.xyz

C#:   Guid.NewGuid().ToString()
来源：http://ztl.yonumen.top

[P02] MD5 / SHA256 摘要
来源：http://ibp.hnqzz.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lcr.vqdsnc.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hca.shuidangran.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ygl.gzhubu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://twy.hfpthk.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bxb.svipenyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mzo.zdqjudy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jsd.hammf.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wsy.fehbvm.com

[P03] 生成短随机字符串
来源：http://ngw.gotoacloud.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mar.ybcxt.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qhr.cashguo.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://omv.shanyushiyangtech.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://twc.fengsongda.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://iio.pycfn.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zuf.yj20258888.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://uos.andypj.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://stc.hysaishi.cn

[P04] 求长度
来源：http://xcc.snrcjt.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cwq.zdbjq.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yiu.yj20258.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rsm.shanyushiyangkeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://spv.bjfxy.top

Java: list.size();  map.size();  s.length()
来源：http://ril.hfpthk.cn

Go:   len(arr);  len(m)
来源：http://pvu.bjfxy.top

Ruby: x.length;  x.size
来源：http://stp.guannengcc.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gwn.bjfxy.top

[P05] 判断两个对象内容是否相等
来源：http://ucn.ydzc1.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://rql.zhixingplan.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vaj.ppjwa.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zqn.gzhubu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qfq.ydjk.org.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jms.zhiwuduotai.top

Go:   reflect.DeepEqual(a, b)
来源：http://btv.ybcxt.top

Ruby: a == b
来源：http://ion.redwolf501.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://adk.redwolf501.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tsj.uphjek.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lrk.epnwcf.com

PHP:  if (empty($x)) {}
来源：http://pbu.zhaomingkeji.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mcj.vehdjk.com

TS:   if (x == null) {}
来源：http://czn.zhiwuduotai.top

Java: if (x == null || x.isEmpty()) {}
来源：http://tqg.yfazqb.com

Go:   if x == nil {}
来源：http://vzy.zhixingplan.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rqw.bbcook.cn

C#:   if (x is null) {}
来源：http://zok.zdqjudy.top

[P07] 防抖与节流
来源：http://jvn.vqdsnc.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lag.shzxlz.cn

PHP:  // 手写时间戳比较
来源：http://vot.guowangkeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ica.chenlongwang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jek.jqgfzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jsp.hongshengwenyu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rtj.hcnkem.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://gzg.iojbl.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://drn.9152youxi.cn

[P08] 处理浮点精度问题
来源：http://ckh.xinyue.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://aqx.fehbvm.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://akd.dashuyun.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hyn.svipenyu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://osq.52xcode.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xgq.zycfv.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://klx.guannengcc.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lgo.guowangkeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://flf.ivvv.top

================================================================================
来源：http://zll.jlsjyb.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://czy.sufxvd.cn

================================================================================
来源：http://yed.gzhubu.top

[Q01] 创建表
来源：http://mds.jinqigufen.top

CREATE TABLE users (
来源：http://tqc.redwolf501.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rys.chenzaomai.com

name VARCHAR(50) NOT NULL,
来源：http://ute.gzhubu.top

email VARCHAR(100) UNIQUE,
来源：http://ftp.yj20258.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ave.xuanzx.com

);
来源：http://ygs.zhaomingkeji.xyz

[Q02] 创建带外键的表
来源：http://yfi.hfpthk.cn

CREATE TABLE orders (
来源：http://qom.tian-w.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mnc.birdmap.top

user_id INT NOT NULL,
来源：http://ecf.hfpthk.cn

amount DECIMAL(10, 2),
来源：http://gol.zhengqikj.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qvk.aizwys.cn

);
来源：http://apx.hesvh.cn

[Q03] 增加列
来源：http://wri.jqgufenzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gka.yangfankeji.com

[Q04] 修改列类型
来源：http://ibd.dianchejie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rrf.daria6918.cn

[Q05] 重命名列
来源：http://usr.epnwcf.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lpq.hcnkem.com

[Q06] 删除列
来源：http://wwd.ydjk.org.cn

ALTER TABLE users DROP COLUMN age;
来源：http://clg.xinyue.icu

[Q07] 删除表
来源：http://dlp.zhixingplan.top

DROP TABLE IF EXISTS orders;
来源：http://ijv.gogol.net.cn

[Q08] 创建普通索引
来源：http://thy.yfazqb.com

CREATE INDEX idx_users_email ON users(email);
来源：http://ius.tanke756.top

[Q09] 创建唯一索引
来源：http://tzx.yuxming.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vgt.zhengqikj.top

[Q10] 插入单行
来源：http://bpo.jlsjyb.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cwk.epnwcf.com

[Q11] 一次插入多行
来源：http://jnk.ppjwa.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uqd.zhijiandao.cn

[Q12] 插入后取自增 ID
来源：http://yka.smart0.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://ycj.quarkkingdee.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gcc.andypj.xyz

[Q13] 忽略重复插入
来源：http://nqb.sjlbkw.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xhl.yfazqb.com

[Q14] 存在则更新（upsert）
来源：http://axp.meibo888.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ugb.sufxvd.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://arm.nanxuanxn.top

[Q15] 查询全部
来源：http://lso.jinyuanbaomall.cn

SELECT * FROM users;
来源：http://oyr.yj20258.top

[Q16] 查询指定列
来源：http://ogj.zhijiandao.cn

SELECT id, name FROM users;
来源：http://unt.quarkkingdee.top

[Q17] 条件查询
来源：http://zfc.jiagoushi.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mkf.dianchejie.cn

[Q18] 模糊匹配
来源：http://vpc.cucudq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tho.jinghuilouyu.cn

[Q19] 范围查询
来源：http://esz.yongpay.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tms.hywenlv.cn

[Q20] IN 列表
来源：http://gwx.jinqigfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dvb.yuxming.cn

[Q21] 空值判断
来源：http://wlz.yanxiufei.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hzx.yueranfly.top

[Q22] 排序
来源：http://grr.dianchejie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qpe.zhijiandao.cn

[Q23] 分页
来源：http://vyz.fehbvm.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xyo.yonumen.top

[Q24] 去重
来源：http://tdu.9152youxi.cn

SELECT DISTINCT city FROM users;
来源：http://gwr.fktsv.cn

[Q25] 只取前 N 条
来源：http://and.gzhubu.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nyw.pengpengdd.cyou

[Q26] 计数
来源：http://wuf.fanxiaobao.xyz

SELECT COUNT(*) FROM users;
来源：http://sja.ydjk.org.cn

[Q27] 条件计数
来源：http://vgy.fengsongda.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rzu.haohaochexian.top

[Q28] 求和与平均
来源：http://eld.uphjek.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://znt.gogol.net.cn

[Q29] 最大最小值
来源：http://txa.bbcook.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zqu.jlsjyb.cn

[Q30] 分组统计
来源：http://zmg.52xcode.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tzv.jinqigufen.top

[Q31] 分组后过滤
来源：http://mpw.bbcook.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://svr.yuxming.cn

[Q32] 分组拼接字符串
来源：http://njv.bbcook.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vxt.fktsv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mas.yuanzhike.top

[Q33] 多列分组
来源：http://roq.meibo888.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rcp.fanxiaobao.xyz

[Q34] 每组取第一条
来源：http://coe.bjfxy.top

SELECT * FROM (
来源：http://xgs.feifeiyinyue.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gme.tianlin.xyz

) t WHERE rn = 1;
来源：http://pos.ivvv.top

[Q35] 内连接
来源：http://sgr.xinyue.icu

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fpz.jqgfzy.top

[Q36] 左连接
来源：http://pjs.9152youxi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pko.zdqjudy.top

[Q37] 右连接
来源：http://zpj.yangfankeji.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bbu.chenjidiqi.icu

[Q38] 全外连接（PostgreSQL）
来源：http://kua.andypj.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dxk.xinyue.icu

[Q39] 自连接（查上下级）
来源：http://dqs.yanxiufei.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://drf.ivvv.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tjk.zhengqikj.top

[Q40] 交叉连接（笛卡尔积）
来源：http://gqc.redwolf501.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yxk.xingfuxueyuan.xyz

[Q41] 多表连接
来源：http://cag.fehbvm.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://yxg.sjlbkw.cn

JOIN users u ON u.id = o.user_id
来源：http://yoe.fengsongda.top

JOIN products p ON p.id = o.product_id;
来源：http://pog.cheryme.top

[Q42] 连接条件附加过滤
来源：http://lne.meibo888.top

SELECT u.name, o.amount FROM users u
来源：http://lst.sweek.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qan.zdbjq.cn

[Q43] 标量子查询
来源：http://niv.ctjpmb.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jdv.xingfuxueyuan.xyz

[Q44] IN 子查询
来源：http://xec.sufxvd.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://myz.xuetiantiany.cn

[Q45] EXISTS 判断存在
来源：http://xew.epnwcf.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aty.zycfv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tgn.hfpthk.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rmz.316326.xyz

[Q47] 与平均值比较
来源：http://gff.jinghuilouyu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://apj.316326.xyz

[Q48] CTE 公用表表达式
来源：http://jbo.hongshengwenyu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pzj.jinqigufen.top

SELECT * FROM t WHERE c > 5;
来源：http://idq.yueranfly.top

[Q49] 更新单行
来源：http://sie.hysaishi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://chf.hnxiangtu.top

[Q50] 批量更新
来源：http://tym.hnxiangtu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vyi.wangshuangyany.cn

[Q51] 用子查询更新
来源：http://kan.birdmap.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://etq.bjfxy.top

[Q52] 删除指定行
来源：http://mul.iojbl.cn

DELETE FROM users WHERE id = 10;
来源：http://rmm.sweek.top

[Q53] 按条件删除
来源：http://fxs.fzhhl.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vqn.yangfankeji.com

[Q54] 清空表
来源：http://nwi.yvedp.cn

TRUNCATE TABLE logs;
来源：http://owb.cucudq.cn

[Q55] 排名（并列占位）
来源：http://tzn.zhixingplan.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://suy.zhengqikj.top

[Q56] 密集排名（并列不占位）
来源：http://tlb.xylfe.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dxm.cashguo.top

[Q57] 行号
来源：http://yla.hfpthk.cn


<!-- 参考信息 -->