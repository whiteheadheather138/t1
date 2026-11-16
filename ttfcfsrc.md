代发 wailian999

Py:   itertools.permutations(arr)
来源：http://oeb.mhx1999.top

PHP:  // 手写递归交换
来源：http://gjt.yfazqb.com

JS:   // 手写回溯递归
来源：http://mxb.yj202588.top

TS:   // 手写回溯递归
来源：http://vdy.guowangkeji.top

Java: // 手写回溯递归
来源：http://hrj.pengpengdd.cyou

Go:   // 手写回溯递归
来源：http://fmt.aizwys.cn

Ruby: arr.permutation.to_a
来源：http://boj.hcnkem.com

C#:   // 手写回溯递归
来源：http://uxw.redwolf501.top

[N09] 栈与队列
来源：http://wef.jinqigufen.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nwz.shanyushiyangtech.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rpt.ydjk.org.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oom.cqqwz.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gcf.shzxlz.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://woz.hywenlv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://amw.yfazqb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lsv.ywan-chungtsiang.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dzp.feifeiyinyue.top

[N10] 链表节点定义
来源：http://lpw.sysykeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lvy.chenzaomai.com

PHP:  class Node { public $v; public $next = null; }
来源：http://tuo.nwbrower.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ekp.yuanzhike.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://upx.gogol.net.cn

Java: class Node { int v; Node next; }
来源：http://krv.vqdsnc.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qkd.dianchejie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ndf.fanxiaobao.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://zwe.daria6918.cn

[N11] 二叉树中序遍历
来源：http://ltk.feifeiyinyue.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://eky.zdbjq.cn

PHP:  // 手写递归函数
来源：http://tsu.ehwqpu.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wtx.sufxvd.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yvw.tanke756.top

Java: // 手写递归
来源：http://zmm.chenzaomai.com

Go:   // 手写递归
来源：http://jeg.havefunace.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lfb.hysaishi.cn

C#:   // 手写递归
来源：http://ott.meibo888.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gwi.zdbjq.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fbr.hammf.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mce.gaohongyu789.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ajx.ydjk.org.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jhe.xinyue.icu

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://grc.tian-w.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uoy.jyoumei.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qkr.snrcjt.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fxi.ppjwa.cn

================================================================================
来源：http://ton.fktsv.cn

O. 并发与异步
来源：http://ect.epnwcf.com

================================================================================
来源：http://gmz.fktsv.cn

[O01] 启动一个线程
来源：http://cou.shangyingyoupin.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://owy.hywenlv.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cph.zhijiandao.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ecv.gzhubu.top

TS:   // 同 JS
来源：http://tpu.aibaodan.cn

Java: new Thread(() -> f()).start()
来源：http://bix.cashguo.top

Go:   go f()
来源：http://zmz.vqdsnc.cn

Ruby: Thread.new { f }
来源：http://woe.ppjwa.cn

C#:   Task.Run(() => F());
来源：http://amf.feifeiyinyue.top

[O02] 使用线程池
来源：http://xui.hesvh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://esv.guannengcc.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wqb.chenzaomai.com

JS:   // worker_threads 线程池
来源：http://fgr.yueranfly.top

TS:   // worker_threads 线程池
来源：http://iux.ctjpmb.com

Java: Executors.newFixedThreadPool(4)
来源：http://wwv.chenjidiqi.icu

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kym.pengpengdd.cyou

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://czu.xuetiantiany.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://imb.vehdjk.com

[O03] 加锁保护共享数据
来源：http://opq.wangdashe.top

Py:   with lock: shared += 1
来源：http://trj.9152youxi.cn

PHP:  // 用 flock() 做文件锁
来源：http://izo.sxryk.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://exz.wangshuangyany.cn

TS:   // 同 JS
来源：http://kgq.chenzaomai.com

Java: synchronized (this) { shared++; }
来源：http://gzf.gaohongyu789.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xyc.zhongyouzk.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ves.xylfe.cn

C#:   lock (gate) { shared++; }
来源：http://xpb.feifeiyinyue.top

[O04] 定义异步函数并等待
来源：http://xud.jinghuilouyu.cn

Py:   async def f():⏎    await g()
来源：http://wmr.tanke756.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lrv.cucudq.cn

JS:   async function f() { await g(); }
来源：http://vik.jiagoushi.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://lim.jianghu66.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://eif.jiagoushi.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://esi.bbcook.cn

Ruby: # 用 Fiber 或 async gem
来源：http://okb.hesvh.cn

C#:   async Task F() { await G(); }
来源：http://nmn.kuanghao11.cn

[O05] 并发执行并等待全部完成
来源：http://zsi.jinqigufen.top

Py:   asyncio.gather(*tasks)
来源：http://sjb.yfazqb.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://car.zdbjq.cn

JS:   await Promise.all(tasks)
来源：http://jkc.ydzc1.top

TS:   await Promise.all(tasks)
来源：http://ltc.iojbl.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bru.kuanghao11.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qoh.ctjpmb.com

Ruby: threads.map(&:join)
来源：http://gzb.52xcode.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jxj.kuanghao11.cn

[O06] 使用进程池
来源：http://qcd.tianlin.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://czz.yuanzhike.top

PHP:  // pcntl_fork 或多进程队列
来源：http://hlh.jinghuilouyu.cn

JS:   // child_process / cluster 模块
来源：http://lzp.dianchejie.cn

TS:   // child_process / cluster 模块
来源：http://lbb.wangshuangyany.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ukw.chenzaomai.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zov.chenjidiqi.icu

Ruby: // fork 块
来源：http://gab.yj20258.top

C#:   Parallel.For
来源：http://psi.svipenyu.cn

================================================================================
来源：http://ilq.tanke756.top

P. 常用工具函数
来源：http://spb.yangfankeji.com

================================================================================
来源：http://pjv.sxryk.cn

[P01] 生成 UUID
来源：http://ggr.ybcxt.top

Py:   str(uuid.uuid4())
来源：http://mqd.shanyushiyangkeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sgd.pycfn.com

JS:   crypto.randomUUID()
来源：http://hir.9152youxi.cn

TS:   crypto.randomUUID()
来源：http://jxs.fzhhl.top

Java: UUID.randomUUID().toString()
来源：http://tgr.yuxming.cn

Go:   // 用 github.com/google/uuid
来源：http://hiu.shuidangran.top

Ruby: SecureRandom.uuid
来源：http://lok.316326.xyz

C#:   Guid.NewGuid().ToString()
来源：http://dnj.jyoumei.cn

[P02] MD5 / SHA256 摘要
来源：http://cqg.9152youxi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tmo.hysaishi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://cdh.chenlongwang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ayr.hnqzz.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ilc.zdbjq.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gtx.zdbjq.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bhr.cashguo.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cym.zhixingplan.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://utx.ydjk.org.cn

[P03] 生成短随机字符串
来源：http://wdu.cqqwz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://irx.aibaodan.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pdk.yj20258888.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hob.shanyushiyangkeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bkx.fzhhl.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://oml.cheryme.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yln.pycfn.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://fqm.pycfn.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qtg.sjlbkw.cn

[P04] 求长度
来源：http://zbx.cashguo.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://eks.chenzaomai.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gga.ydjk.org.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zpf.meibo888.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://shg.gotoacloud.top

Java: list.size();  map.size();  s.length()
来源：http://bks.tanke756.top

Go:   len(arr);  len(m)
来源：http://lqj.yuanzhike.top

Ruby: x.length;  x.size
来源：http://grx.xziqi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kgj.cucudq.cn

[P05] 判断两个对象内容是否相等
来源：http://obz.zdqjudy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lvq.jinghuilouyu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gff.jqgfzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://swd.dianchejie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pns.9152youxi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pec.shanyushiyangkeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://xqc.vehdjk.com

Ruby: a == b
来源：http://afw.ctjpmb.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kud.haohaochexian.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kuy.meibo888.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cqq.316326.xyz

PHP:  if (empty($x)) {}
来源：http://uew.yongpay.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xgu.hesvh.cn

TS:   if (x == null) {}
来源：http://nzp.tanke756.top

Java: if (x == null || x.isEmpty()) {}
来源：http://qxd.hysaishi.cn

Go:   if x == nil {}
来源：http://nfs.hongshengwenyu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uue.cucudq.cn

C#:   if (x is null) {}
来源：http://vrk.hammf.cn

[P07] 防抖与节流
来源：http://wuo.chenlongwang.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ldz.fktsv.cn

PHP:  // 手写时间戳比较
来源：http://aon.yuanzhike.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zeh.nwbrower.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gur.bbcook.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nts.ydjk.org.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yul.ctjpmb.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://bii.nanxinkj.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hwl.hnqzz.top

[P08] 处理浮点精度问题
来源：http://pos.uphjek.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://afi.cdnleiting.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nci.xziqi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ymp.0kj1m.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gdi.shzxlz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bzt.zhaomingkeji.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xar.yj20258.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://irp.fanxiaobao.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qjx.feifeiyinyue.top

================================================================================
来源：http://yip.jiagoushi.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vem.yongpay.top

================================================================================
来源：http://jtd.shangyingyoupin.top

[Q01] 创建表
来源：http://rft.fehbvm.com

CREATE TABLE users (
来源：http://ice.epnwcf.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nga.andypj.xyz

name VARCHAR(50) NOT NULL,
来源：http://oyq.mhx1999.top

email VARCHAR(100) UNIQUE,
来源：http://okx.uphjek.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wop.dashuyun.cn

);
来源：http://jcg.316326.xyz

[Q02] 创建带外键的表
来源：http://mfl.cheryme.top

CREATE TABLE orders (
来源：http://qsl.yj202588.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hno.sweek.top

user_id INT NOT NULL,
来源：http://fuj.xinyue.icu

amount DECIMAL(10, 2),
来源：http://gyp.kuanghao11.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vnp.fanxiaobao.xyz

);
来源：http://tjw.hammf.cn

[Q03] 增加列
来源：http://fev.jiagoushi.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qww.yj202588.top

[Q04] 修改列类型
来源：http://eep.zycfv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ghi.yueranfly.top

[Q05] 重命名列
来源：http://duv.xuanzx.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ymq.snrcjt.cn

[Q06] 删除列
来源：http://sdk.hywenlv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ckr.yanxiufei.cn

[Q07] 删除表
来源：http://jiv.yueranfly.top

DROP TABLE IF EXISTS orders;
来源：http://egb.yj20258.top

[Q08] 创建普通索引
来源：http://cso.yj20258.top

CREATE INDEX idx_users_email ON users(email);
来源：http://baq.nanxuanxn.top

[Q09] 创建唯一索引
来源：http://ntw.xuetiantiany.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://drf.gzhubu.top

[Q10] 插入单行
来源：http://etk.ybcxt.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://azq.ppjwa.cn

[Q11] 一次插入多行
来源：http://igs.iojbl.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lvw.epnwcf.com

[Q12] 插入后取自增 ID
来源：http://nmm.fengsongda.top

INSERT INTO users (name) VALUES ('C');
来源：http://umu.pycfn.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zae.fengsongda.top

[Q13] 忽略重复插入
来源：http://nfj.gaohongyu789.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gty.52xcode.cn

[Q14] 存在则更新（upsert）
来源：http://ahd.bbcook.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mkr.jinqigfzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mxr.chenlongwang.top

[Q15] 查询全部
来源：http://fkv.jinyuanbaomall.cn

SELECT * FROM users;
来源：http://ouh.jlsjyb.cn

[Q16] 查询指定列
来源：http://hai.smart0.xyz

SELECT id, name FROM users;
来源：http://dek.zhongyouzk.top

[Q17] 条件查询
来源：http://kas.mhx1999.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qdo.sjlbkw.cn

[Q18] 模糊匹配
来源：http://wmt.chenzaomai.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sha.sysykeji.top

[Q19] 范围查询
来源：http://bei.zhongyouzk.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://njj.dashuyun.cn

[Q20] IN 列表
来源：http://vfj.haohaochexian.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ris.cdnleiting.top

[Q21] 空值判断
来源：http://tqn.gaohongyu789.top

SELECT * FROM users WHERE email IS NULL;
来源：http://olc.nwbrower.top

[Q22] 排序
来源：http://ssr.epnwcf.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://upm.zdqjudy.top

[Q23] 分页
来源：http://uep.cucudq.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bow.birdmap.top

[Q24] 去重
来源：http://yrt.hesvh.cn

SELECT DISTINCT city FROM users;
来源：http://qpo.smart0.xyz

[Q25] 只取前 N 条
来源：http://ora.cqqwz.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nln.shanyushiyangtech.top

[Q26] 计数
来源：http://det.sysykeji.top

SELECT COUNT(*) FROM users;
来源：http://ngo.zhaomingkeji.xyz

[Q27] 条件计数
来源：http://eby.hywenlv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cnr.zhijiandao.cn

[Q28] 求和与平均
来源：http://fnl.jinghuilouyu.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ckk.jqgfzy.top

[Q29] 最大最小值
来源：http://vyx.aizwys.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://rug.gogol.net.cn

[Q30] 分组统计
来源：http://dpe.dianchejie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jar.daxiang520.top

[Q31] 分组后过滤
来源：http://chf.cqqwz.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lsm.ctjpmb.com

[Q32] 分组拼接字符串
来源：http://wyx.vqdsnc.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wvx.xuanzx.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qqx.zdqjudy.top

[Q33] 多列分组
来源：http://ysk.jinqigufen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rmk.vqdsnc.cn

[Q34] 每组取第一条
来源：http://aku.haohaochexian.top

SELECT * FROM (
来源：http://huv.shuidangran.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://udx.yj202588.top

) t WHERE rn = 1;
来源：http://but.cdnleiting.top

[Q35] 内连接
来源：http://oij.ctjpmb.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hgy.yj20258888.top

[Q36] 左连接
来源：http://dae.smart0.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hoi.yuxming.cn

[Q37] 右连接
来源：http://svk.shuidangran.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zvo.mhx1999.top

[Q38] 全外连接（PostgreSQL）
来源：http://mcf.pycfn.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lnj.redwolf501.top

[Q39] 自连接（查上下级）
来源：http://xim.quarkkingdee.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://col.smart0.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kab.cdnleiting.top

[Q40] 交叉连接（笛卡尔积）
来源：http://uma.shuidangran.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xxf.quarkkingdee.top

[Q41] 多表连接
来源：http://kup.tian-w.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ifi.gzhubu.top

JOIN users u ON u.id = o.user_id
来源：http://avy.nanxuanxn.top

JOIN products p ON p.id = o.product_id;
来源：http://lfb.guowangkeji.top

[Q42] 连接条件附加过滤
来源：http://yti.vehdjk.com

SELECT u.name, o.amount FROM users u
来源：http://zlp.yangfankeji.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mli.andypj.xyz

[Q43] 标量子查询
来源：http://lnk.birdmap.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://obc.yuanzhike.top

[Q44] IN 子查询
来源：http://dqu.hfpthk.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dff.zycfv.cn

[Q45] EXISTS 判断存在
来源：http://jer.ctjpmb.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rck.dianchejie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yma.guannengcc.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ftn.cheryme.top

[Q47] 与平均值比较
来源：http://dux.hnxiangtu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ccc.xinyue.icu

[Q48] CTE 公用表表达式
来源：http://cln.shangyingyoupin.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pyp.yangfankeji.com

SELECT * FROM t WHERE c > 5;
来源：http://txf.yj20258.top

[Q49] 更新单行
来源：http://abl.xziqi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yej.ctjpmb.com

[Q50] 批量更新
来源：http://qnx.redwolf501.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vhg.yj20258888.top

[Q51] 用子查询更新
来源：http://neh.0kj1m.cn


<!-- 参考信息 -->