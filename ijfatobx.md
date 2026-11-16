代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://iku.yfazqb.com

JS:   // 手写 Map：map.set(v, i)
来源：http://lct.gaohongyu789.top

TS:   // 手写 Map<string, number>
来源：http://yts.hysaishi.cn

Java: // 手写 HashMap
来源：http://uwo.cdnleiting.top

Go:   // 手写 map[int]int
来源：http://ovy.fzhhl.top

Ruby: // 手写 Hash
来源：http://zee.chenzaomai.com

C#:   // 手写 Dictionary<int, int>
来源：http://efz.chenjidiqi.icu

[N08] 生成全排列
来源：http://ioh.52xcode.cn

Py:   itertools.permutations(arr)
来源：http://psv.gaohongyu789.top

PHP:  // 手写递归交换
来源：http://eor.zdqjudy.top

JS:   // 手写回溯递归
来源：http://vxv.andypj.xyz

TS:   // 手写回溯递归
来源：http://nls.yongpay.top

Java: // 手写回溯递归
来源：http://esi.tian-w.cn

Go:   // 手写回溯递归
来源：http://izh.xziqi.cn

Ruby: arr.permutation.to_a
来源：http://zob.aizwys.cn

C#:   // 手写回溯递归
来源：http://sbf.yongpay.top

[N09] 栈与队列
来源：http://aql.ywan-chungtsiang.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xus.zycfv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ohw.mhx1999.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tfx.xuetiantiany.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://inr.aizwys.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fmx.aibaodan.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tne.yuanzhike.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ngn.daxiang520.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fzk.316326.xyz

[N10] 链表节点定义
来源：http://cmf.tian-w.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fff.nanxuanxn.top

PHP:  class Node { public $v; public $next = null; }
来源：http://wve.tian-w.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://poo.chenlongwang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vzb.chenlongwang.top

Java: class Node { int v; Node next; }
来源：http://jsg.haohaochexian.top

Go:   type Node struct { V int; Next *Node }
来源：http://isc.zhijiandao.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rwp.ydjk.org.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kwi.zhongyouzk.top

[N11] 二叉树中序遍历
来源：http://noy.cheryme.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baj.tanke756.top

PHP:  // 手写递归函数
来源：http://nij.fehbvm.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vqt.tanke756.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qyf.dashuyun.cn

Java: // 手写递归
来源：http://hek.jqgufenzy.top

Go:   // 手写递归
来源：http://pms.bbcook.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://odm.cheryme.top

C#:   // 手写递归
来源：http://qev.smart0.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://moq.chenjidiqi.icu

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://eib.redwolf501.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bpq.hfpthk.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cdp.yj202588.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://msf.chenlongwang.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://emp.guannengcc.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kgu.gaohongyu789.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://beo.gaohongyu789.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://het.fengsongda.top

================================================================================
来源：http://izr.cashguo.top

O. 并发与异步
来源：http://zhk.jinqigfzy.top

================================================================================
来源：http://zpn.hammf.cn

[O01] 启动一个线程
来源：http://cmc.shuidangran.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gqf.shzxlz.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jpb.feifeiyinyue.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zha.hysaishi.cn

TS:   // 同 JS
来源：http://vki.jlsjyb.cn

Java: new Thread(() -> f()).start()
来源：http://izp.hysaishi.cn

Go:   go f()
来源：http://izo.ehwqpu.com

Ruby: Thread.new { f }
来源：http://rfn.zycfv.cn

C#:   Task.Run(() => F());
来源：http://sjd.cucudq.cn

[O02] 使用线程池
来源：http://zcv.snrcjt.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ypr.iojbl.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pnw.tian-w.cn

JS:   // worker_threads 线程池
来源：http://oii.nwbrower.top

TS:   // worker_threads 线程池
来源：http://plt.mhx1999.top

Java: Executors.newFixedThreadPool(4)
来源：http://hcm.gzhubu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jrn.ywan-chungtsiang.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nuc.hnxiangtu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xnn.shanyushiyangtech.top

[O03] 加锁保护共享数据
来源：http://kun.xingfuxueyuan.xyz

Py:   with lock: shared += 1
来源：http://uhv.fengsongda.top

PHP:  // 用 flock() 做文件锁
来源：http://ntp.guowangkeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://skz.bbcook.cn

TS:   // 同 JS
来源：http://zoh.fktsv.cn

Java: synchronized (this) { shared++; }
来源：http://lhw.fehbvm.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uxm.iojbl.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://nwi.xinyue.icu

C#:   lock (gate) { shared++; }
来源：http://edo.zhoulong.xyz

[O04] 定义异步函数并等待
来源：http://dkc.vqdsnc.cn

Py:   async def f():⏎    await g()
来源：http://ieb.ctjpmb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lyw.xingfuxueyuan.xyz

JS:   async function f() { await g(); }
来源：http://ahk.jinyuanbaomall.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ply.tianlin.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://eoo.fengsongda.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nqd.aizwys.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wwq.uphjek.com

C#:   async Task F() { await G(); }
来源：http://phc.ivvv.top

[O05] 并发执行并等待全部完成
来源：http://mlg.aibaodan.cn

Py:   asyncio.gather(*tasks)
来源：http://qbf.jqgufenzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://smh.xuanzx.com

JS:   await Promise.all(tasks)
来源：http://sde.zhengqikj.top

TS:   await Promise.all(tasks)
来源：http://nwj.xuetiantiany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cac.sjlbkw.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bjs.vqdsnc.cn

Ruby: threads.map(&:join)
来源：http://wtr.zhijiandao.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hbi.wangshuangyany.cn

[O06] 使用进程池
来源：http://svg.nwbrower.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pbe.sysykeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://krp.hammf.cn

JS:   // child_process / cluster 模块
来源：http://jsb.gaohongyu789.top

TS:   // child_process / cluster 模块
来源：http://ign.c1oappe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ilc.jinyuanbaomall.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hqx.redwolf501.top

Ruby: // fork 块
来源：http://bkh.wangshuangyany.cn

C#:   Parallel.For
来源：http://srm.tian-w.cn

================================================================================
来源：http://due.vqdsnc.cn

P. 常用工具函数
来源：http://aoi.cheryme.top

================================================================================
来源：http://fcr.xingfuxueyuan.xyz

[P01] 生成 UUID
来源：http://rnn.jiagoushi.top

Py:   str(uuid.uuid4())
来源：http://max.hnqzz.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zzt.xingfuxueyuan.xyz

JS:   crypto.randomUUID()
来源：http://aeb.cheryme.top

TS:   crypto.randomUUID()
来源：http://orj.pycfn.com

Java: UUID.randomUUID().toString()
来源：http://vfa.xingfuxueyuan.xyz

Go:   // 用 github.com/google/uuid
来源：http://omu.hcnkem.com

Ruby: SecureRandom.uuid
来源：http://pxa.wangdashe.top

C#:   Guid.NewGuid().ToString()
来源：http://crf.smart0.xyz

[P02] MD5 / SHA256 摘要
来源：http://adp.hesvh.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nup.hywenlv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jaz.zhoulong.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vpv.hammf.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pfe.fzhhl.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tjv.zhongyouzk.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://grd.yanxiufei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://upd.cheryme.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xvd.jianghu66.top

[P03] 生成短随机字符串
来源：http://xdq.hnxiangtu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ris.chenlongwang.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wqp.quarkkingdee.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://chd.gotoacloud.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kwh.cdnleiting.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wue.yj20258.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hkt.shzxlz.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xsi.haohaochexian.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xpe.cashguo.top

[P04] 求长度
来源：http://gnf.gotoacloud.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jjk.fanxiaobao.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sho.yj20258.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xed.hnxiangtu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vst.shzxlz.cn

Java: list.size();  map.size();  s.length()
来源：http://xak.smart0.xyz

Go:   len(arr);  len(m)
来源：http://mdp.ppjwa.cn

Ruby: x.length;  x.size
来源：http://yls.sjlbkw.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ztj.jiagoushi.top

[P05] 判断两个对象内容是否相等
来源：http://pzj.aibaodan.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pdq.zhongyouzk.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wdd.hesvh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://aui.fanxiaobao.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bsf.guowangkeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wuu.bjfxy.top

Go:   reflect.DeepEqual(a, b)
来源：http://hqi.ydzc1.top

Ruby: a == b
来源：http://fcq.316326.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nqp.yj20258888.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xxf.bbcook.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ugx.xziqi.cn

PHP:  if (empty($x)) {}
来源：http://tck.ppjwa.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hza.hywenlv.cn

TS:   if (x == null) {}
来源：http://jge.mhx1999.top

Java: if (x == null || x.isEmpty()) {}
来源：http://stl.jinqigfzy.top

Go:   if x == nil {}
来源：http://kxd.0kj1m.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ogs.hnxiangtu.top

C#:   if (x is null) {}
来源：http://tjn.jqgufenzy.top

[P07] 防抖与节流
来源：http://flh.yvedp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bfb.52xcode.cn

PHP:  // 手写时间戳比较
来源：http://bil.wangshuangyany.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cnb.aizwys.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kua.hnxiangtu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ztc.bjfxy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kjn.cqqwz.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sik.nwbrower.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ihm.ivvv.top

[P08] 处理浮点精度问题
来源：http://iez.meibo888.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uos.aibaodan.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lxp.birdmap.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mcm.wangshuangyany.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hbn.hesvh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ujy.jinqigufen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dfg.zdbjq.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nki.wangshuangyany.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pxk.yuxming.cn

================================================================================
来源：http://inw.ehwqpu.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uqr.sysykeji.top

================================================================================
来源：http://qoh.ydjk.org.cn

[Q01] 创建表
来源：http://qry.birdmap.top

CREATE TABLE users (
来源：http://ihh.yongpay.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bha.epnwcf.com

name VARCHAR(50) NOT NULL,
来源：http://ppk.yj20258888.top

email VARCHAR(100) UNIQUE,
来源：http://ihk.cqqwz.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rvb.zhongyouzk.top

);
来源：http://zla.kuanghao11.cn

[Q02] 创建带外键的表
来源：http://lwu.52xcode.cn

CREATE TABLE orders (
来源：http://idu.ydzc1.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lcq.daxiang520.top

user_id INT NOT NULL,
来源：http://ift.feifeiyinyue.top

amount DECIMAL(10, 2),
来源：http://hrn.pengpengdd.cyou

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mww.xingfuxueyuan.xyz

);
来源：http://tmv.yfazqb.com

[Q03] 增加列
来源：http://lqy.nwbrower.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rom.chenlongwang.top

[Q04] 修改列类型
来源：http://jbu.yanxiufei.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lit.bbcook.cn

[Q05] 重命名列
来源：http://ghr.sxryk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://viq.haohaochexian.top

[Q06] 删除列
来源：http://lla.yanxiufei.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sea.tianlin.xyz

[Q07] 删除表
来源：http://eww.zdbjq.cn

DROP TABLE IF EXISTS orders;
来源：http://bcc.yvedp.cn

[Q08] 创建普通索引
来源：http://fab.zhoulong.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://fgj.daxiang520.top

[Q09] 创建唯一索引
来源：http://mnt.hongshengwenyu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jpe.zhiwuduotai.top

[Q10] 插入单行
来源：http://onb.hongshengwenyu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yku.havefunace.top

[Q11] 一次插入多行
来源：http://snx.wangshuangyany.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hpi.vqdsnc.cn

[Q12] 插入后取自增 ID
来源：http://fsf.yongpay.top

INSERT INTO users (name) VALUES ('C');
来源：http://rvb.hnxiangtu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lrn.yj202588.top

[Q13] 忽略重复插入
来源：http://sjm.316326.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pzc.pycfn.com

[Q14] 存在则更新（upsert）
来源：http://ivu.yanxiufei.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rtr.shanyushiyangtech.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bil.jlsjyb.cn

[Q15] 查询全部
来源：http://bub.jyoumei.cn

SELECT * FROM users;
来源：http://ggh.pycfn.com

[Q16] 查询指定列
来源：http://dph.hcnkem.com

SELECT id, name FROM users;
来源：http://hmo.cdnleiting.top

[Q17] 条件查询
来源：http://gkt.epnwcf.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xke.cdnleiting.top

[Q18] 模糊匹配
来源：http://fov.svipenyu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vlx.wangdashe.top

[Q19] 范围查询
来源：http://agk.yongpay.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bdt.zhengqikj.top

[Q20] IN 列表
来源：http://nsb.xylfe.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ztu.snrcjt.cn

[Q21] 空值判断
来源：http://rum.ydjk.org.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pdn.shanyushiyangkeji.top

[Q22] 排序
来源：http://wuy.yfazqb.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://oer.tian-w.cn

[Q23] 分页
来源：http://yux.ywan-chungtsiang.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://knz.zhoulong.xyz

[Q24] 去重
来源：http://cui.yuxming.cn

SELECT DISTINCT city FROM users;
来源：http://pcu.jinyuanbaomall.cn

[Q25] 只取前 N 条
来源：http://pdq.yuxming.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tnq.jqgfzy.top

[Q26] 计数
来源：http://elk.hammf.cn

SELECT COUNT(*) FROM users;
来源：http://for.guannengcc.top

[Q27] 条件计数
来源：http://zaz.yanxiufei.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hft.hammf.cn

[Q28] 求和与平均
来源：http://wpw.0kj1m.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qbh.316326.xyz

[Q29] 最大最小值
来源：http://xjb.feifeiyinyue.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xeo.jinghuilouyu.cn

[Q30] 分组统计
来源：http://miq.hongshengwenyu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ulz.hnqzz.top

[Q31] 分组后过滤
来源：http://zet.tian-w.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://brb.jqgfzy.top

[Q32] 分组拼接字符串
来源：http://pzr.chenlongwang.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://aoo.chenjidiqi.icu

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bjz.tarul.cn

[Q33] 多列分组
来源：http://xwu.sysykeji.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ybu.hesvh.cn

[Q34] 每组取第一条
来源：http://hvq.vqdsnc.cn

SELECT * FROM (
来源：http://ifc.zhengqikj.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cop.yj202588.top

) t WHERE rn = 1;
来源：http://xso.jlsjyb.cn

[Q35] 内连接
来源：http://qka.cdnleiting.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dyw.jqgfzy.top

[Q36] 左连接
来源：http://usn.zycfv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tcy.tanke756.top

[Q37] 右连接
来源：http://arb.hesvh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nli.quarkkingdee.top

[Q38] 全外连接（PostgreSQL）
来源：http://ipd.316326.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ogd.hnxiangtu.top

[Q39] 自连接（查上下级）
来源：http://hqu.xingfuxueyuan.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://joc.yuanzhike.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cum.zhongyouzk.top

[Q40] 交叉连接（笛卡尔积）
来源：http://hwk.guannengcc.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vza.9152youxi.cn

[Q41] 多表连接
来源：http://prf.sufxvd.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://agx.jinqigufen.top

JOIN users u ON u.id = o.user_id
来源：http://whp.yj202588.top

JOIN products p ON p.id = o.product_id;
来源：http://mxh.dashuyun.cn

[Q42] 连接条件附加过滤
来源：http://pvd.zhoulong.xyz

SELECT u.name, o.amount FROM users u
来源：http://fvb.shanyushiyangtech.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://und.fanxiaobao.xyz

[Q43] 标量子查询
来源：http://nlz.chenzaomai.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nqr.ydjk.org.cn

[Q44] IN 子查询
来源：http://kup.guowangkeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tmh.svipenyu.cn

[Q45] EXISTS 判断存在
来源：http://anh.ehwqpu.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cyc.sweek.top

[Q46] NOT EXISTS 判断不存在
来源：http://yvb.xylfe.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kmz.hongshengwenyu.top

[Q47] 与平均值比较
来源：http://uts.hammf.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sjo.tianlin.xyz


<!-- 参考信息 -->