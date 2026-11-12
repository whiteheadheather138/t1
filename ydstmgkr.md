代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mew.nwbrower.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://azy.tian-w.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://anr.0kj1m.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mlm.yj202588.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wcc.fengsongda.top

[N10] 链表节点定义
来源：http://ttr.sjlbkw.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cyb.fktsv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wak.ivvv.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tho.nanxinkj.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vut.aibaodan.cn

Java: class Node { int v; Node next; }
来源：http://kgc.yonumen.top

Go:   type Node struct { V int; Next *Node }
来源：http://grf.cucudq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gpl.ywan-chungtsiang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://alu.tanke756.top

[N11] 二叉树中序遍历
来源：http://gyv.haohaochexian.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qax.hfpthk.cn

PHP:  // 手写递归函数
来源：http://ata.iojbl.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://txj.iojbl.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gjh.xuetiantiany.cn

Java: // 手写递归
来源：http://ues.pengpengdd.cyou

Go:   // 手写递归
来源：http://mhq.shzxlz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gvs.jqgufenzy.top

C#:   // 手写递归
来源：http://wxb.meibo888.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gxl.hfpthk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pjr.zhiwuduotai.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pmx.yangfankeji.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uqn.zhengqikj.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cja.0kj1m.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mrx.gotoacloud.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zwp.redwolf501.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ugf.xziqi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://txn.ctjpmb.com

================================================================================
来源：http://qgk.tian-w.cn

O. 并发与异步
来源：http://coy.jqgufenzy.top

================================================================================
来源：http://lzv.sufxvd.cn

[O01] 启动一个线程
来源：http://gje.cqqwz.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://eal.xinyue.icu

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hzz.jianghu66.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cug.ydzc1.top

TS:   // 同 JS
来源：http://abx.wangdashe.top

Java: new Thread(() -> f()).start()
来源：http://wke.0kj1m.cn

Go:   go f()
来源：http://ylg.9152youxi.cn

Ruby: Thread.new { f }
来源：http://fmo.yvedp.cn

C#:   Task.Run(() => F());
来源：http://ohs.pycfn.com

[O02] 使用线程池
来源：http://tae.ybcxt.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fcy.vehdjk.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yzk.chenzaomai.com

JS:   // worker_threads 线程池
来源：http://jmr.yj202588.top

TS:   // worker_threads 线程池
来源：http://zkt.gogol.net.cn

Java: Executors.newFixedThreadPool(4)
来源：http://uzm.andypj.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hfk.shanyushiyangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yti.jyoumei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nlw.zdqjudy.top

[O03] 加锁保护共享数据
来源：http://xwx.shangyingyoupin.top

Py:   with lock: shared += 1
来源：http://huo.ppjwa.cn

PHP:  // 用 flock() 做文件锁
来源：http://lrp.aizwys.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wko.zhoulong.xyz

TS:   // 同 JS
来源：http://gpm.jinghuilouyu.cn

Java: synchronized (this) { shared++; }
来源：http://okv.andypj.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tfe.jiagoushi.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://sdt.zhiwuduotai.top

C#:   lock (gate) { shared++; }
来源：http://npr.316326.xyz

[O04] 定义异步函数并等待
来源：http://uxg.uphjek.com

Py:   async def f():⏎    await g()
来源：http://xch.redwolf501.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hdc.smart0.xyz

JS:   async function f() { await g(); }
来源：http://hem.gogol.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ghq.dashuyun.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yyl.nanxinkj.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://got.gotoacloud.top

Ruby: # 用 Fiber 或 async gem
来源：http://hej.xylfe.cn

C#:   async Task F() { await G(); }
来源：http://clb.sjlbkw.cn

[O05] 并发执行并等待全部完成
来源：http://fwt.ctjpmb.com

Py:   asyncio.gather(*tasks)
来源：http://qvg.zhiwuduotai.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jcv.shanyushiyangkeji.top

JS:   await Promise.all(tasks)
来源：http://qgs.shangyingyoupin.top

TS:   await Promise.all(tasks)
来源：http://vxm.9152youxi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rxc.yj20258888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zzr.gaohongyu789.top

Ruby: threads.map(&:join)
来源：http://srr.ydzc1.top

C#:   await Task.WhenAll(t1, t2)
来源：http://rns.hongshengwenyu.top

[O06] 使用进程池
来源：http://lfj.meibo888.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zba.chenlongwang.top

PHP:  // pcntl_fork 或多进程队列
来源：http://nhw.wangshuangyany.cn

JS:   // child_process / cluster 模块
来源：http://pny.hesvh.cn

TS:   // child_process / cluster 模块
来源：http://hig.epnwcf.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://thv.bbcook.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bdl.cdnleiting.top

Ruby: // fork 块
来源：http://oks.fktsv.cn

C#:   Parallel.For
来源：http://dda.tanke756.top

================================================================================
来源：http://utj.wangshuangyany.cn

P. 常用工具函数
来源：http://kkw.meibo888.top

================================================================================
来源：http://mlx.zhaomingkeji.xyz

[P01] 生成 UUID
来源：http://nez.zhoulong.xyz

Py:   str(uuid.uuid4())
来源：http://war.fehbvm.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zmm.daria6918.cn

JS:   crypto.randomUUID()
来源：http://srj.shanyushiyangtech.top

TS:   crypto.randomUUID()
来源：http://rhd.nanxuanxn.top

Java: UUID.randomUUID().toString()
来源：http://wnw.yanxiufei.cn

Go:   // 用 github.com/google/uuid
来源：http://chl.yj20258888.top

Ruby: SecureRandom.uuid
来源：http://ldv.pengpengdd.cyou

C#:   Guid.NewGuid().ToString()
来源：http://mud.xuetiantiany.cn

[P02] MD5 / SHA256 摘要
来源：http://thm.wangdashe.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tql.nanxinkj.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://uvd.bbcook.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xxo.pycfn.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pgp.feifeiyinyue.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nmo.316326.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qnq.hfpthk.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://daf.gogol.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dcd.yueranfly.top

[P03] 生成短随机字符串
来源：http://iqg.mhx1999.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://muv.c1oappe.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bkr.shzxlz.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sec.vehdjk.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ude.xingfuxueyuan.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tcp.yj20258888.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rpp.aizwys.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xve.guowangkeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gfj.nanxuanxn.top

[P04] 求长度
来源：http://csj.uphjek.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xea.meibo888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://shg.chenzaomai.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ohu.redwolf501.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lpf.zhoulong.xyz

Java: list.size();  map.size();  s.length()
来源：http://zss.tanke756.top

Go:   len(arr);  len(m)
来源：http://dso.zhixingplan.top

Ruby: x.length;  x.size
来源：http://uio.vqdsnc.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rcj.yueranfly.top

[P05] 判断两个对象内容是否相等
来源：http://kiq.tarul.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fdq.316326.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tzm.jqgfzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mkn.ywan-chungtsiang.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://opn.pengpengdd.cyou

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wuq.jinqigufen.top

Go:   reflect.DeepEqual(a, b)
来源：http://eok.ppjwa.cn

Ruby: a == b
来源：http://syq.shuidangran.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cuf.vehdjk.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rsc.cdnleiting.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oyj.vehdjk.com

PHP:  if (empty($x)) {}
来源：http://ybg.uphjek.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tde.nanxinkj.top

TS:   if (x == null) {}
来源：http://lmv.cheryme.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ywg.nanxuanxn.top

Go:   if x == nil {}
来源：http://rjq.snrcjt.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://urg.havefunace.top

C#:   if (x is null) {}
来源：http://jbc.zycfv.cn

[P07] 防抖与节流
来源：http://jpg.aizwys.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ddi.ydzc1.top

PHP:  // 手写时间戳比较
来源：http://ine.quarkkingdee.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yxi.vqdsnc.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zpo.yongpay.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://axu.zhoulong.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bnx.sjlbkw.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://eak.c1oappe.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wfr.chenlongwang.top

[P08] 处理浮点精度问题
来源：http://wzs.epnwcf.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hps.zhoulong.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xol.guannengcc.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uqw.mhx1999.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://use.dashuyun.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vdm.xziqi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://esw.fengsongda.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://won.jiagoushi.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jkc.guannengcc.top

================================================================================
来源：http://nal.uphjek.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pwg.tarul.cn

================================================================================
来源：http://uwm.yfazqb.com

[Q01] 创建表
来源：http://fkv.zhijiandao.cn

CREATE TABLE users (
来源：http://hfp.yuanzhike.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://drd.yvedp.cn

name VARCHAR(50) NOT NULL,
来源：http://cnu.birdmap.top

email VARCHAR(100) UNIQUE,
来源：http://vtr.chenlongwang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://eek.guannengcc.top

);
来源：http://rmf.hesvh.cn

[Q02] 创建带外键的表
来源：http://ygt.gaohongyu789.top

CREATE TABLE orders (
来源：http://edh.zhoulong.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rbs.ydzc1.top

user_id INT NOT NULL,
来源：http://jeu.hfpthk.cn

amount DECIMAL(10, 2),
来源：http://iou.yuanzhike.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://utf.hammf.cn

);
来源：http://skz.yj20258.top

[Q03] 增加列
来源：http://qws.xingfuxueyuan.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://aad.hesvh.cn

[Q04] 修改列类型
来源：http://ogd.jinghuilouyu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hgc.9152youxi.cn

[Q05] 重命名列
来源：http://lmo.cheryme.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fuo.hysaishi.cn

[Q06] 删除列
来源：http://noa.yj20258888.top

ALTER TABLE users DROP COLUMN age;
来源：http://xbu.bjfxy.top

[Q07] 删除表
来源：http://qni.fktsv.cn

DROP TABLE IF EXISTS orders;
来源：http://qib.jyoumei.cn

[Q08] 创建普通索引
来源：http://puf.yongpay.top

CREATE INDEX idx_users_email ON users(email);
来源：http://cec.feifeiyinyue.top

[Q09] 创建唯一索引
来源：http://zfx.ctjpmb.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yvz.tarul.cn

[Q10] 插入单行
来源：http://cjo.haohaochexian.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://axj.sjlbkw.cn

[Q11] 一次插入多行
来源：http://lsq.jqgfzy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lsh.chenlongwang.top

[Q12] 插入后取自增 ID
来源：http://lez.jinqigufen.top

INSERT INTO users (name) VALUES ('C');
来源：http://oqh.bbcook.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zus.wangshuangyany.cn

[Q13] 忽略重复插入
来源：http://gxe.fzhhl.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kng.ehwqpu.com

[Q14] 存在则更新（upsert）
来源：http://lto.xziqi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://liz.xylfe.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kty.gogol.net.cn

[Q15] 查询全部
来源：http://eat.xuetiantiany.cn

SELECT * FROM users;
来源：http://aaz.xylfe.cn

[Q16] 查询指定列
来源：http://nri.xuetiantiany.cn

SELECT id, name FROM users;
来源：http://zzu.shuidangran.top

[Q17] 条件查询
来源：http://iml.jinqigfzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jly.feifeiyinyue.top

[Q18] 模糊匹配
来源：http://gnj.hnxiangtu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://eqj.jqgufenzy.top

[Q19] 范围查询
来源：http://ulc.shanyushiyangkeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://iik.zhijiandao.cn

[Q20] IN 列表
来源：http://zre.316326.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wdd.cqqwz.cn

[Q21] 空值判断
来源：http://yhw.shzxlz.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://yhs.cucudq.cn

[Q22] 排序
来源：http://oni.gaohongyu789.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mmt.dashuyun.cn

[Q23] 分页
来源：http://ebm.mhx1999.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ycj.epnwcf.com

[Q24] 去重
来源：http://ypz.nanxuanxn.top

SELECT DISTINCT city FROM users;
来源：http://yog.svipenyu.cn

[Q25] 只取前 N 条
来源：http://clr.xingfuxueyuan.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bmt.dianchejie.cn

[Q26] 计数
来源：http://lxk.bjfxy.top

SELECT COUNT(*) FROM users;
来源：http://emi.hcnkem.com

[Q27] 条件计数
来源：http://sjk.iojbl.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ojh.yvedp.cn

[Q28] 求和与平均
来源：http://bnz.zhongyouzk.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kyw.xuanzx.com

[Q29] 最大最小值
来源：http://wrs.xziqi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://nut.52xcode.cn

[Q30] 分组统计
来源：http://rkp.ywan-chungtsiang.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rin.bjfxy.top

[Q31] 分组后过滤
来源：http://aiy.smart0.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zuu.fanxiaobao.xyz

[Q32] 分组拼接字符串
来源：http://rhg.aibaodan.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uco.pycfn.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rgk.shangyingyoupin.top

[Q33] 多列分组
来源：http://bms.chenlongwang.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nbh.hongshengwenyu.top

[Q34] 每组取第一条
来源：http://dyi.ppjwa.cn

SELECT * FROM (
来源：http://hay.cheryme.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rfa.0kj1m.cn

) t WHERE rn = 1;
来源：http://rzy.nwbrower.top

[Q35] 内连接
来源：http://xub.snrcjt.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ybs.hnqzz.top

[Q36] 左连接
来源：http://qjs.svipenyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gil.yj20258888.top

[Q37] 右连接
来源：http://jrf.daxiang520.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hyv.fzhhl.top

[Q38] 全外连接（PostgreSQL）
来源：http://wqn.chenzaomai.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oiu.hnxiangtu.top

[Q39] 自连接（查上下级）
来源：http://vyz.zycfv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://atg.dianchejie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://eyb.dianchejie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rei.316326.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://unf.feifeiyinyue.top

[Q41] 多表连接
来源：http://con.haohaochexian.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://nuu.sysykeji.top

JOIN users u ON u.id = o.user_id
来源：http://jfg.daria6918.cn

JOIN products p ON p.id = o.product_id;
来源：http://clz.wangshuangyany.cn

[Q42] 连接条件附加过滤
来源：http://rrm.yj20258888.top

SELECT u.name, o.amount FROM users u
来源：http://bnu.gzhubu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cgo.birdmap.top

[Q43] 标量子查询
来源：http://grp.tarul.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ska.zdbjq.cn

[Q44] IN 子查询
来源：http://gmf.yangfankeji.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gze.xuetiantiany.cn

[Q45] EXISTS 判断存在
来源：http://jor.tian-w.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cug.fktsv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wje.feifeiyinyue.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://izf.aizwys.cn

[Q47] 与平均值比较
来源：http://hpd.snrcjt.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qjl.zhengqikj.top

[Q48] CTE 公用表表达式
来源：http://jao.aizwys.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fdc.yuanzhike.top

SELECT * FROM t WHERE c > 5;
来源：http://ava.cqqwz.cn

[Q49] 更新单行
来源：http://fsy.yangfankeji.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://for.bjfxy.top

[Q50] 批量更新
来源：http://onx.zhengqikj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cmg.vqdsnc.cn

[Q51] 用子查询更新
来源：http://kkb.zhiwuduotai.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://obl.guannengcc.top

[Q52] 删除指定行
来源：http://cqo.yuanzhike.top

DELETE FROM users WHERE id = 10;
来源：http://vrf.yanxiufei.cn

[Q53] 按条件删除
来源：http://tdf.fktsv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://viw.redwolf501.top

[Q54] 清空表
来源：http://utb.chenlongwang.top

TRUNCATE TABLE logs;
来源：http://frv.gotoacloud.top

[Q55] 排名（并列占位）
来源：http://sxd.xuanzx.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cks.yj202588.top

[Q56] 密集排名（并列不占位）
来源：http://dla.gaohongyu789.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pce.jinqigufen.top

[Q57] 行号
来源：http://pnn.meibo888.top


<!-- 参考信息 -->