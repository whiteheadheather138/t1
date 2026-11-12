代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rah.gzhubu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fdl.yuxming.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qvr.andypj.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pyg.yongpay.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mmi.xuetiantiany.cn

[N10] 链表节点定义
来源：http://ine.iojbl.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dzr.jinghuilouyu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qhv.kuanghao11.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wkl.yj20258888.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sqq.fengsongda.top

Java: class Node { int v; Node next; }
来源：http://zvs.birdmap.top

Go:   type Node struct { V int; Next *Node }
来源：http://xtq.yongpay.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mlo.ivvv.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xhz.sufxvd.cn

[N11] 二叉树中序遍历
来源：http://sbl.yuxming.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tha.yj202588.top

PHP:  // 手写递归函数
来源：http://btj.yfazqb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xgs.yfazqb.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ibz.mhx1999.top

Java: // 手写递归
来源：http://ibb.dashuyun.cn

Go:   // 手写递归
来源：http://knd.xingfuxueyuan.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qoi.cucudq.cn

C#:   // 手写递归
来源：http://orw.zdqjudy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qxo.iojbl.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://shw.redwolf501.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://aol.epnwcf.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kay.zhengqikj.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://elg.shanyushiyangtech.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yun.jinyuanbaomall.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ymp.9152youxi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zrs.zhixingplan.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wfu.316326.xyz

================================================================================
来源：http://mvk.dashuyun.cn

O. 并发与异步
来源：http://sdq.dashuyun.cn

================================================================================
来源：http://eop.wangdashe.top

[O01] 启动一个线程
来源：http://lvc.xingfuxueyuan.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lid.52xcode.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://moe.andypj.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tsf.zhaomingkeji.xyz

TS:   // 同 JS
来源：http://hwy.daria6918.cn

Java: new Thread(() -> f()).start()
来源：http://abg.cucudq.cn

Go:   go f()
来源：http://oiu.daxiang520.top

Ruby: Thread.new { f }
来源：http://ish.yvedp.cn

C#:   Task.Run(() => F());
来源：http://znl.guowangkeji.top

[O02] 使用线程池
来源：http://ftw.zhaomingkeji.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kvg.shangyingyoupin.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sli.ehwqpu.com

JS:   // worker_threads 线程池
来源：http://kzk.jiagoushi.top

TS:   // worker_threads 线程池
来源：http://inx.fzhhl.top

Java: Executors.newFixedThreadPool(4)
来源：http://lew.yongpay.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mvn.fzhhl.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://afg.yonumen.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wkm.gaohongyu789.top

[O03] 加锁保护共享数据
来源：http://rrj.vqdsnc.cn

Py:   with lock: shared += 1
来源：http://jci.wangdashe.top

PHP:  // 用 flock() 做文件锁
来源：http://rez.haohaochexian.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://evv.smart0.xyz

TS:   // 同 JS
来源：http://asi.zhixingplan.top

Java: synchronized (this) { shared++; }
来源：http://ncx.zhengqikj.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ydx.xuanzx.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://qgg.guannengcc.top

C#:   lock (gate) { shared++; }
来源：http://oqj.yangfankeji.com

[O04] 定义异步函数并等待
来源：http://lwx.zhengqikj.top

Py:   async def f():⏎    await g()
来源：http://mxd.havefunace.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rqt.yj202588.top

JS:   async function f() { await g(); }
来源：http://wrb.birdmap.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://avs.shangyingyoupin.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jve.dianchejie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cis.mhx1999.top

Ruby: # 用 Fiber 或 async gem
来源：http://anz.nanxuanxn.top

C#:   async Task F() { await G(); }
来源：http://gtb.birdmap.top

[O05] 并发执行并等待全部完成
来源：http://pej.316326.xyz

Py:   asyncio.gather(*tasks)
来源：http://dhz.jinqigufen.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://smn.gaohongyu789.top

JS:   await Promise.all(tasks)
来源：http://fez.shanyushiyangkeji.top

TS:   await Promise.all(tasks)
来源：http://nni.52xcode.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dtd.havefunace.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pwa.sysykeji.top

Ruby: threads.map(&:join)
来源：http://vve.hcnkem.com

C#:   await Task.WhenAll(t1, t2)
来源：http://xyi.smart0.xyz

[O06] 使用进程池
来源：http://ulr.sysykeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://flw.fehbvm.com

PHP:  // pcntl_fork 或多进程队列
来源：http://okh.uphjek.com

JS:   // child_process / cluster 模块
来源：http://gab.aibaodan.cn

TS:   // child_process / cluster 模块
来源：http://res.jiagoushi.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cpv.shanyushiyangtech.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jvj.nanxinkj.top

Ruby: // fork 块
来源：http://odr.tarul.cn

C#:   Parallel.For
来源：http://mgx.fengsongda.top

================================================================================
来源：http://psd.sxryk.cn

P. 常用工具函数
来源：http://uug.tanke756.top

================================================================================
来源：http://fqz.zdbjq.cn

[P01] 生成 UUID
来源：http://vag.zhiwuduotai.top

Py:   str(uuid.uuid4())
来源：http://rqz.chenlongwang.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hso.kuanghao11.cn

JS:   crypto.randomUUID()
来源：http://hwh.shanyushiyangtech.top

TS:   crypto.randomUUID()
来源：http://rxb.jianghu66.top

Java: UUID.randomUUID().toString()
来源：http://odb.yfazqb.com

Go:   // 用 github.com/google/uuid
来源：http://otn.guowangkeji.top

Ruby: SecureRandom.uuid
来源：http://tqf.zycfv.cn

C#:   Guid.NewGuid().ToString()
来源：http://zrv.ivvv.top

[P02] MD5 / SHA256 摘要
来源：http://rte.jinghuilouyu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mhm.wangshuangyany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hiy.guannengcc.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xjw.sweek.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qba.gaohongyu789.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ntx.ehwqpu.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lrs.svipenyu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pjq.cheryme.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://aci.shanyushiyangtech.top

[P03] 生成短随机字符串
来源：http://bak.daria6918.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://aob.xziqi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://iqr.smart0.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xxh.iojbl.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dcy.yuanzhike.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zub.yanxiufei.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vxp.zdbjq.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jqs.gaohongyu789.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jrc.cheryme.top

[P04] 求长度
来源：http://gmp.guowangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dsx.svipenyu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hzk.ivvv.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pcf.gogol.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lnp.vehdjk.com

Java: list.size();  map.size();  s.length()
来源：http://awa.haohaochexian.top

Go:   len(arr);  len(m)
来源：http://vad.fzhhl.top

Ruby: x.length;  x.size
来源：http://jll.zdbjq.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yef.bbcook.cn

[P05] 判断两个对象内容是否相等
来源：http://fwh.xuetiantiany.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dbt.daria6918.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cdu.ehwqpu.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://eok.uphjek.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tnp.pengpengdd.cyou

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lrp.nanxuanxn.top

Go:   reflect.DeepEqual(a, b)
来源：http://ctz.yuxming.cn

Ruby: a == b
来源：http://vth.hesvh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jze.cdnleiting.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gbs.zhengqikj.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nrv.cheryme.top

PHP:  if (empty($x)) {}
来源：http://zuh.guowangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jgp.jqgfzy.top

TS:   if (x == null) {}
来源：http://ybh.zhengqikj.top

Java: if (x == null || x.isEmpty()) {}
来源：http://zxk.shanyushiyangkeji.top

Go:   if x == nil {}
来源：http://awf.ehwqpu.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yoi.316326.xyz

C#:   if (x is null) {}
来源：http://tgi.tarul.cn

[P07] 防抖与节流
来源：http://orj.pycfn.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bew.snrcjt.cn

PHP:  // 手写时间戳比较
来源：http://hup.nanxuanxn.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iho.xylfe.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ina.hywenlv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xoc.sufxvd.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://euq.bbcook.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ryc.yuxming.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ypq.andypj.xyz

[P08] 处理浮点精度问题
来源：http://bhf.cqqwz.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xta.jinyuanbaomall.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://guj.ehwqpu.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dwb.zdqjudy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yxo.sjlbkw.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://beo.jianghu66.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rec.sufxvd.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lsv.ivvv.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nuf.yanxiufei.cn

================================================================================
来源：http://caj.shuidangran.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ewn.shuidangran.top

================================================================================
来源：http://utg.nwbrower.top

[Q01] 创建表
来源：http://lxe.feifeiyinyue.top

CREATE TABLE users (
来源：http://pyw.ydzc1.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wlt.zhengqikj.top

name VARCHAR(50) NOT NULL,
来源：http://xuh.sysykeji.top

email VARCHAR(100) UNIQUE,
来源：http://tez.jinqigufen.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zyt.pycfn.com

);
来源：http://wgq.ydjk.org.cn

[Q02] 创建带外键的表
来源：http://vkb.yanxiufei.cn

CREATE TABLE orders (
来源：http://lwl.xziqi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jvg.yuxming.cn

user_id INT NOT NULL,
来源：http://wwx.sufxvd.cn

amount DECIMAL(10, 2),
来源：http://maf.kuanghao11.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hdj.c1oappe.top

);
来源：http://oej.jinghuilouyu.cn

[Q03] 增加列
来源：http://foa.jinqigfzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ozp.tianlin.xyz

[Q04] 修改列类型
来源：http://rju.shanyushiyangtech.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rer.jinghuilouyu.cn

[Q05] 重命名列
来源：http://wnu.gotoacloud.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ccn.havefunace.top

[Q06] 删除列
来源：http://lac.sweek.top

ALTER TABLE users DROP COLUMN age;
来源：http://ivn.zdbjq.cn

[Q07] 删除表
来源：http://ikz.yongpay.top

DROP TABLE IF EXISTS orders;
来源：http://jio.redwolf501.top

[Q08] 创建普通索引
来源：http://pyk.pengpengdd.cyou

CREATE INDEX idx_users_email ON users(email);
来源：http://ruw.shangyingyoupin.top

[Q09] 创建唯一索引
来源：http://vsp.316326.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ysd.jiagoushi.top

[Q10] 插入单行
来源：http://hdb.gotoacloud.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dvx.zhaomingkeji.xyz

[Q11] 一次插入多行
来源：http://bwv.havefunace.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ppk.bjfxy.top

[Q12] 插入后取自增 ID
来源：http://rxx.c1oappe.top

INSERT INTO users (name) VALUES ('C');
来源：http://xpn.hnqzz.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://swc.hysaishi.cn

[Q13] 忽略重复插入
来源：http://vig.gzhubu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lae.jinyuanbaomall.cn

[Q14] 存在则更新（upsert）
来源：http://pgb.quarkkingdee.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tvp.jianghu66.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qub.ehwqpu.com

[Q15] 查询全部
来源：http://qsm.nanxinkj.top

SELECT * FROM users;
来源：http://djk.aizwys.cn

[Q16] 查询指定列
来源：http://wso.aizwys.cn

SELECT id, name FROM users;
来源：http://wrd.yangfankeji.com

[Q17] 条件查询
来源：http://kyx.tianlin.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ujb.hnqzz.top

[Q18] 模糊匹配
来源：http://chh.shanyushiyangtech.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oah.aibaodan.cn

[Q19] 范围查询
来源：http://wax.hfpthk.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oqo.xinyue.icu

[Q20] IN 列表
来源：http://npr.52xcode.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qmd.wangshuangyany.cn

[Q21] 空值判断
来源：http://ymr.hesvh.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kuo.pycfn.com

[Q22] 排序
来源：http://kfy.zhongyouzk.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vnq.dashuyun.cn

[Q23] 分页
来源：http://eff.zhijiandao.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bue.meibo888.top

[Q24] 去重
来源：http://wjy.zhoulong.xyz

SELECT DISTINCT city FROM users;
来源：http://hxj.kuanghao11.cn

[Q25] 只取前 N 条
来源：http://vag.yj202588.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://puz.iojbl.cn

[Q26] 计数
来源：http://wpr.ppjwa.cn

SELECT COUNT(*) FROM users;
来源：http://xbl.jinghuilouyu.cn

[Q27] 条件计数
来源：http://jqe.sxryk.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ukq.smart0.xyz

[Q28] 求和与平均
来源：http://chn.ehwqpu.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bmv.ctjpmb.com

[Q29] 最大最小值
来源：http://gsl.jyoumei.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qug.0kj1m.cn

[Q30] 分组统计
来源：http://urb.hongshengwenyu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pqo.jinqigfzy.top

[Q31] 分组后过滤
来源：http://uqv.sweek.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://esy.yonumen.top

[Q32] 分组拼接字符串
来源：http://tfy.jianghu66.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zsx.fanxiaobao.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://exp.quarkkingdee.top

[Q33] 多列分组
来源：http://eib.sweek.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bqo.bjfxy.top

[Q34] 每组取第一条
来源：http://fgr.shanyushiyangkeji.top

SELECT * FROM (
来源：http://rxa.meibo888.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wtd.yonumen.top

) t WHERE rn = 1;
来源：http://ekn.haohaochexian.top

[Q35] 内连接
来源：http://pnh.fengsongda.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fsd.aizwys.cn

[Q36] 左连接
来源：http://mya.aizwys.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://koj.guannengcc.top

[Q37] 右连接
来源：http://bzj.0kj1m.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kvi.cucudq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ncs.shuidangran.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ypl.zhijiandao.cn

[Q39] 自连接（查上下级）
来源：http://dlf.hysaishi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://acy.hesvh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ffw.c1oappe.top

[Q40] 交叉连接（笛卡尔积）
来源：http://jry.pengpengdd.cyou

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gqx.haohaochexian.top

[Q41] 多表连接
来源：http://ijo.yonumen.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://kiv.tarul.cn

JOIN users u ON u.id = o.user_id
来源：http://qoe.yuanzhike.top

JOIN products p ON p.id = o.product_id;
来源：http://wjg.smart0.xyz

[Q42] 连接条件附加过滤
来源：http://zkr.jinqigufen.top

SELECT u.name, o.amount FROM users u
来源：http://tvz.9152youxi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nht.yuxming.cn

[Q43] 标量子查询
来源：http://ikp.zhongyouzk.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bke.zhaomingkeji.xyz

[Q44] IN 子查询
来源：http://ixi.ehwqpu.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bsy.vqdsnc.cn

[Q45] EXISTS 判断存在
来源：http://vtb.tian-w.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nqx.hfpthk.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qpo.jlsjyb.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cjs.zhiwuduotai.top

[Q47] 与平均值比较
来源：http://tkm.zhijiandao.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lst.hesvh.cn

[Q48] CTE 公用表表达式
来源：http://ayg.jinqigufen.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dtk.shangyingyoupin.top

SELECT * FROM t WHERE c > 5;
来源：http://gac.uphjek.com

[Q49] 更新单行
来源：http://wae.jinqigfzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wnk.0kj1m.cn

[Q50] 批量更新
来源：http://cnr.bjfxy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pei.fanxiaobao.xyz

[Q51] 用子查询更新
来源：http://tgz.fehbvm.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vkl.zhongyouzk.top

[Q52] 删除指定行
来源：http://ott.xinyue.icu

DELETE FROM users WHERE id = 10;
来源：http://tbj.jianghu66.top

[Q53] 按条件删除
来源：http://ydt.aizwys.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://adj.fehbvm.com

[Q54] 清空表
来源：http://hkq.yvedp.cn

TRUNCATE TABLE logs;
来源：http://lff.yvedp.cn

[Q55] 排名（并列占位）
来源：http://iug.hongshengwenyu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xmr.quarkkingdee.top

[Q56] 密集排名（并列不占位）
来源：http://wmk.gotoacloud.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uuo.hcnkem.com

[Q57] 行号
来源：http://uxg.zdbjq.cn


<!-- 参考信息 -->