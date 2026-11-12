代发 wailian999

Go:   // 手写 map[int]int
来源：http://apk.gogol.net.cn

Ruby: // 手写 Hash
来源：http://yjt.gzhubu.top

C#:   // 手写 Dictionary<int, int>
来源：http://dwk.ehwqpu.com

[N08] 生成全排列
来源：http://szi.shanyushiyangkeji.top

Py:   itertools.permutations(arr)
来源：http://cdn.zhengqikj.top

PHP:  // 手写递归交换
来源：http://pbu.gaohongyu789.top

JS:   // 手写回溯递归
来源：http://jbn.quarkkingdee.top

TS:   // 手写回溯递归
来源：http://ten.jinghuilouyu.cn

Java: // 手写回溯递归
来源：http://vdb.jianghu66.top

Go:   // 手写回溯递归
来源：http://bhc.guannengcc.top

Ruby: arr.permutation.to_a
来源：http://fun.tarul.cn

C#:   // 手写回溯递归
来源：http://qwt.yangfankeji.com

[N09] 栈与队列
来源：http://gnz.cheryme.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nuf.sweek.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ocn.yuxming.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mem.yfazqb.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ebm.xuanzx.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kez.yonumen.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yer.aizwys.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mch.jqgfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ivp.birdmap.top

[N10] 链表节点定义
来源：http://zgj.zhoulong.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://edd.yfazqb.com

PHP:  class Node { public $v; public $next = null; }
来源：http://gxn.hesvh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cps.shanyushiyangtech.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kyl.zhixingplan.top

Java: class Node { int v; Node next; }
来源：http://wih.yongpay.top

Go:   type Node struct { V int; Next *Node }
来源：http://dly.tarul.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ybe.chenjidiqi.icu

C#:   class Node { public int V; public Node? Next; }
来源：http://wja.jianghu66.top

[N11] 二叉树中序遍历
来源：http://nrm.xziqi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nxt.c1oappe.top

PHP:  // 手写递归函数
来源：http://ngd.ctjpmb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vtp.smart0.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wga.fengsongda.top

Java: // 手写递归
来源：http://kgu.sysykeji.top

Go:   // 手写递归
来源：http://jyu.cashguo.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dov.xinyue.icu

C#:   // 手写递归
来源：http://lzi.yuxming.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://icm.yanxiufei.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bbl.yuanzhike.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kao.316326.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zee.zdbjq.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dxq.havefunace.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kra.feifeiyinyue.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fag.gaohongyu789.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bwe.xuanzx.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rhm.xingfuxueyuan.xyz

================================================================================
来源：http://jgg.yuanzhike.top

O. 并发与异步
来源：http://pws.zhoulong.xyz

================================================================================
来源：http://sff.gzhubu.top

[O01] 启动一个线程
来源：http://mcy.fanxiaobao.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qms.xylfe.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rmn.nanxuanxn.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jje.9152youxi.cn

TS:   // 同 JS
来源：http://ver.daria6918.cn

Java: new Thread(() -> f()).start()
来源：http://mcf.redwolf501.top

Go:   go f()
来源：http://bep.hcnkem.com

Ruby: Thread.new { f }
来源：http://mvo.jinyuanbaomall.cn

C#:   Task.Run(() => F());
来源：http://ody.jinyuanbaomall.cn

[O02] 使用线程池
来源：http://ypr.sufxvd.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dzk.shuidangran.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rlc.chenlongwang.top

JS:   // worker_threads 线程池
来源：http://hnt.cheryme.top

TS:   // worker_threads 线程池
来源：http://mdb.nanxinkj.top

Java: Executors.newFixedThreadPool(4)
来源：http://uch.yangfankeji.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pcu.gaohongyu789.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fwx.gogol.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dyz.ydjk.org.cn

[O03] 加锁保护共享数据
来源：http://iab.cheryme.top

Py:   with lock: shared += 1
来源：http://wkh.guowangkeji.top

PHP:  // 用 flock() 做文件锁
来源：http://eny.zdbjq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ytv.sjlbkw.cn

TS:   // 同 JS
来源：http://jqd.wangshuangyany.cn

Java: synchronized (this) { shared++; }
来源：http://qmv.sweek.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ibw.vehdjk.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://suy.chenzaomai.com

C#:   lock (gate) { shared++; }
来源：http://ljm.fengsongda.top

[O04] 定义异步函数并等待
来源：http://jwp.ctjpmb.com

Py:   async def f():⏎    await g()
来源：http://zol.cucudq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yxq.guannengcc.top

JS:   async function f() { await g(); }
来源：http://pyd.c1oappe.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://enx.gotoacloud.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dbi.shanyushiyangkeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mvo.jinghuilouyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bbw.c1oappe.top

C#:   async Task F() { await G(); }
来源：http://zfs.yueranfly.top

[O05] 并发执行并等待全部完成
来源：http://mkh.havefunace.top

Py:   asyncio.gather(*tasks)
来源：http://rkp.jianghu66.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://akp.c1oappe.top

JS:   await Promise.all(tasks)
来源：http://qxg.xuanzx.com

TS:   await Promise.all(tasks)
来源：http://ows.c1oappe.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://soz.xziqi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zcj.sysykeji.top

Ruby: threads.map(&:join)
来源：http://dnh.xuetiantiany.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fkm.shanyushiyangtech.top

[O06] 使用进程池
来源：http://ooz.yj202588.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xnv.aibaodan.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tqk.daria6918.cn

JS:   // child_process / cluster 模块
来源：http://jki.pycfn.com

TS:   // child_process / cluster 模块
来源：http://eet.sweek.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qci.cheryme.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://maq.daxiang520.top

Ruby: // fork 块
来源：http://xmr.hfpthk.cn

C#:   Parallel.For
来源：http://bqe.tanke756.top

================================================================================
来源：http://lgq.cashguo.top

P. 常用工具函数
来源：http://xkf.epnwcf.com

================================================================================
来源：http://egf.yueranfly.top

[P01] 生成 UUID
来源：http://nxn.aizwys.cn

Py:   str(uuid.uuid4())
来源：http://azb.yanxiufei.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dvl.yanxiufei.cn

JS:   crypto.randomUUID()
来源：http://dti.sweek.top

TS:   crypto.randomUUID()
来源：http://blv.wangdashe.top

Java: UUID.randomUUID().toString()
来源：http://bbs.aizwys.cn

Go:   // 用 github.com/google/uuid
来源：http://vlj.hcnkem.com

Ruby: SecureRandom.uuid
来源：http://pux.daxiang520.top

C#:   Guid.NewGuid().ToString()
来源：http://nhp.yj202588.top

[P02] MD5 / SHA256 摘要
来源：http://bae.aibaodan.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bwf.iojbl.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jen.chenjidiqi.icu

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dkf.jyoumei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kmk.hesvh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://saz.yanxiufei.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://plm.tanke756.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://urz.tarul.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hwn.yvedp.cn

[P03] 生成短随机字符串
来源：http://wvk.316326.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kbl.pengpengdd.cyou

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kva.quarkkingdee.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oay.birdmap.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ekc.cdnleiting.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nud.zhaomingkeji.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uzp.hysaishi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://web.ydjk.org.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ejq.wangdashe.top

[P04] 求长度
来源：http://fha.jqgfzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sfv.hammf.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uim.jinqigfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aur.snrcjt.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ngp.hongshengwenyu.top

Java: list.size();  map.size();  s.length()
来源：http://oij.hesvh.cn

Go:   len(arr);  len(m)
来源：http://lau.fanxiaobao.xyz

Ruby: x.length;  x.size
来源：http://tzj.cashguo.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://tbj.jinyuanbaomall.cn

[P05] 判断两个对象内容是否相等
来源：http://xne.shangyingyoupin.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://rrz.ppjwa.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mhp.ppjwa.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kub.cheryme.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lvf.chenjidiqi.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kxr.zdqjudy.top

Go:   reflect.DeepEqual(a, b)
来源：http://ijb.aizwys.cn

Ruby: a == b
来源：http://hih.snrcjt.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mij.xinyue.icu

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vxx.zdqjudy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iyf.fengsongda.top

PHP:  if (empty($x)) {}
来源：http://mbt.yvedp.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://quh.zhengqikj.top

TS:   if (x == null) {}
来源：http://fpp.aizwys.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zsp.smart0.xyz

Go:   if x == nil {}
来源：http://jgg.zhijiandao.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ktm.hfpthk.cn

C#:   if (x is null) {}
来源：http://vgc.hesvh.cn

[P07] 防抖与节流
来源：http://zbq.aibaodan.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oey.havefunace.top

PHP:  // 手写时间戳比较
来源：http://ish.hysaishi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ckd.316326.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://giv.jinqigfzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jcp.daxiang520.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fcc.zhaomingkeji.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://wpt.wangshuangyany.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://euf.xuanzx.com

[P08] 处理浮点精度问题
来源：http://vdk.sysykeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wux.tanke756.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://snz.zhijiandao.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mzp.andypj.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ahh.guannengcc.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://igt.dianchejie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://goa.shanyushiyangtech.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xvu.ydzc1.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://flk.hcnkem.com

================================================================================
来源：http://gar.fanxiaobao.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zxi.wangshuangyany.cn

================================================================================
来源：http://hxm.jiagoushi.top

[Q01] 创建表
来源：http://yfa.ydzc1.top

CREATE TABLE users (
来源：http://yjn.tanke756.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dcj.316326.xyz

name VARCHAR(50) NOT NULL,
来源：http://yyq.xingfuxueyuan.xyz

email VARCHAR(100) UNIQUE,
来源：http://whn.haohaochexian.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pmj.wangdashe.top

);
来源：http://vmt.tian-w.cn

[Q02] 创建带外键的表
来源：http://fhk.hammf.cn

CREATE TABLE orders (
来源：http://get.tian-w.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ckr.hcnkem.com

user_id INT NOT NULL,
来源：http://wjz.dianchejie.cn

amount DECIMAL(10, 2),
来源：http://jkz.quarkkingdee.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bhy.sxryk.cn

);
来源：http://cjo.shangyingyoupin.top

[Q03] 增加列
来源：http://fyq.shuidangran.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nya.jqgfzy.top

[Q04] 修改列类型
来源：http://sij.c1oappe.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://awr.hesvh.cn

[Q05] 重命名列
来源：http://haf.pycfn.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://stg.yonumen.top

[Q06] 删除列
来源：http://smg.epnwcf.com

ALTER TABLE users DROP COLUMN age;
来源：http://wlm.shangyingyoupin.top

[Q07] 删除表
来源：http://oyr.ywan-chungtsiang.top

DROP TABLE IF EXISTS orders;
来源：http://idf.wangdashe.top

[Q08] 创建普通索引
来源：http://ilj.svipenyu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sbm.gotoacloud.top

[Q09] 创建唯一索引
来源：http://bpo.jinghuilouyu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wzn.cheryme.top

[Q10] 插入单行
来源：http://aca.hysaishi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://omz.ybcxt.top

[Q11] 一次插入多行
来源：http://ypw.guowangkeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dig.chenzaomai.com

[Q12] 插入后取自增 ID
来源：http://tsa.quarkkingdee.top

INSERT INTO users (name) VALUES ('C');
来源：http://uwg.cqqwz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vas.zhaomingkeji.xyz

[Q13] 忽略重复插入
来源：http://rmo.xingfuxueyuan.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hpz.nanxinkj.top

[Q14] 存在则更新（upsert）
来源：http://jsw.zhijiandao.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uyb.feifeiyinyue.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sbs.snrcjt.cn

[Q15] 查询全部
来源：http://ach.svipenyu.cn

SELECT * FROM users;
来源：http://tfy.guowangkeji.top

[Q16] 查询指定列
来源：http://dvy.yj202588.top

SELECT id, name FROM users;
来源：http://erf.yongpay.top

[Q17] 条件查询
来源：http://elk.daria6918.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fms.quarkkingdee.top

[Q18] 模糊匹配
来源：http://hyh.vqdsnc.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jld.yfazqb.com

[Q19] 范围查询
来源：http://kjs.gotoacloud.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nsu.hammf.cn

[Q20] IN 列表
来源：http://tpi.yangfankeji.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gkl.xuanzx.com

[Q21] 空值判断
来源：http://vpc.andypj.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://aab.fengsongda.top

[Q22] 排序
来源：http://rrp.ppjwa.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vsp.kuanghao11.cn

[Q23] 分页
来源：http://jxl.quarkkingdee.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rbd.shanyushiyangtech.top

[Q24] 去重
来源：http://bqt.gzhubu.top

SELECT DISTINCT city FROM users;
来源：http://rcm.aizwys.cn

[Q25] 只取前 N 条
来源：http://fob.jqgfzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qsr.gzhubu.top

[Q26] 计数
来源：http://kyj.ivvv.top

SELECT COUNT(*) FROM users;
来源：http://gji.shzxlz.cn

[Q27] 条件计数
来源：http://fdy.zdqjudy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://avq.shuidangran.top

[Q28] 求和与平均
来源：http://duc.quarkkingdee.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wau.sufxvd.cn

[Q29] 最大最小值
来源：http://hfe.shzxlz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hdv.hysaishi.cn

[Q30] 分组统计
来源：http://nme.ybcxt.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vpv.jyoumei.cn

[Q31] 分组后过滤
来源：http://org.shanyushiyangkeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cds.wangdashe.top

[Q32] 分组拼接字符串
来源：http://cie.jianghu66.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kwg.vqdsnc.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ntt.tianlin.xyz

[Q33] 多列分组
来源：http://bfy.hesvh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qqf.vqdsnc.cn

[Q34] 每组取第一条
来源：http://hxn.0kj1m.cn

SELECT * FROM (
来源：http://iox.hnxiangtu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jtj.jyoumei.cn

) t WHERE rn = 1;
来源：http://erx.xinyue.icu

[Q35] 内连接
来源：http://umg.shanyushiyangkeji.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zxk.c1oappe.top

[Q36] 左连接
来源：http://jnj.fktsv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cld.fanxiaobao.xyz

[Q37] 右连接
来源：http://wjg.hcnkem.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://aqz.gzhubu.top

[Q38] 全外连接（PostgreSQL）
来源：http://naj.vqdsnc.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jvl.zhixingplan.top

[Q39] 自连接（查上下级）
来源：http://pbd.yonumen.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://gjk.jqgfzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vlb.yvedp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qzn.yangfankeji.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dgl.fengsongda.top

[Q41] 多表连接
来源：http://tyf.nanxuanxn.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ejp.sysykeji.top

JOIN users u ON u.id = o.user_id
来源：http://tkc.epnwcf.com

JOIN products p ON p.id = o.product_id;
来源：http://uzg.chenzaomai.com

[Q42] 连接条件附加过滤
来源：http://smu.tarul.cn

SELECT u.name, o.amount FROM users u
来源：http://lka.zdbjq.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lfe.zycfv.cn

[Q43] 标量子查询
来源：http://exs.zycfv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pfc.xuanzx.com

[Q44] IN 子查询
来源：http://otb.ybcxt.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fhp.hcnkem.com

[Q45] EXISTS 判断存在
来源：http://dds.dashuyun.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bim.c1oappe.top

[Q46] NOT EXISTS 判断不存在
来源：http://tnk.zycfv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pzk.pycfn.com

[Q47] 与平均值比较
来源：http://tqq.jinghuilouyu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dmn.yj20258888.top

[Q48] CTE 公用表表达式
来源：http://tmy.ydzc1.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://iqy.nwbrower.top

SELECT * FROM t WHERE c > 5;
来源：http://azr.c1oappe.top

[Q49] 更新单行
来源：http://nct.redwolf501.top


<!-- 参考信息 -->