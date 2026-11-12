代发 wailian999

Go:   // 手写 map[int]int
来源：http://dgs.sjlbkw.cn

Ruby: // 手写 Hash
来源：http://ifm.gzhubu.top

C#:   // 手写 Dictionary<int, int>
来源：http://wak.vehdjk.com

[N08] 生成全排列
来源：http://mre.sweek.top

Py:   itertools.permutations(arr)
来源：http://jcq.316326.xyz

PHP:  // 手写递归交换
来源：http://nsk.daria6918.cn

JS:   // 手写回溯递归
来源：http://nse.pycfn.com

TS:   // 手写回溯递归
来源：http://fan.feifeiyinyue.top

Java: // 手写回溯递归
来源：http://vjw.hcnkem.com

Go:   // 手写回溯递归
来源：http://dnk.wangshuangyany.cn

Ruby: arr.permutation.to_a
来源：http://zls.ydzc1.top

C#:   // 手写回溯递归
来源：http://pqt.yuxming.cn

[N09] 栈与队列
来源：http://von.yj20258888.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wsh.yongpay.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ram.jlsjyb.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ear.cqqwz.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jou.ivvv.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://keq.cashguo.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vgd.gzhubu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tro.guowangkeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jqe.yj20258.top

[N10] 链表节点定义
来源：http://uvz.hfpthk.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gfj.gogol.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pna.shzxlz.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kgn.jianghu66.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gph.c1oappe.top

Java: class Node { int v; Node next; }
来源：http://yoz.bjfxy.top

Go:   type Node struct { V int; Next *Node }
来源：http://scr.hesvh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qav.guowangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://qux.zhiwuduotai.top

[N11] 二叉树中序遍历
来源：http://ubq.daria6918.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ufn.ydjk.org.cn

PHP:  // 手写递归函数
来源：http://eop.yanxiufei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://apm.jlsjyb.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rle.shzxlz.cn

Java: // 手写递归
来源：http://snd.9152youxi.cn

Go:   // 手写递归
来源：http://mve.dianchejie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jnk.feifeiyinyue.top

C#:   // 手写递归
来源：http://utj.zhixingplan.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cad.vehdjk.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yyn.ydjk.org.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lwk.zdbjq.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pts.shzxlz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ptn.zhixingplan.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vvz.epnwcf.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kmm.shangyingyoupin.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kfd.wangdashe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tvh.meibo888.top

================================================================================
来源：http://jta.cheryme.top

O. 并发与异步
来源：http://nhp.xziqi.cn

================================================================================
来源：http://wbt.hammf.cn

[O01] 启动一个线程
来源：http://ube.quarkkingdee.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ihj.zhijiandao.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cob.jqgfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jcc.andypj.xyz

TS:   // 同 JS
来源：http://yst.bjfxy.top

Java: new Thread(() -> f()).start()
来源：http://swd.cucudq.cn

Go:   go f()
来源：http://nnb.fzhhl.top

Ruby: Thread.new { f }
来源：http://mmt.ehwqpu.com

C#:   Task.Run(() => F());
来源：http://aju.daria6918.cn

[O02] 使用线程池
来源：http://wem.chenzaomai.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hac.jlsjyb.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bml.jqgfzy.top

JS:   // worker_threads 线程池
来源：http://idv.chenzaomai.com

TS:   // worker_threads 线程池
来源：http://fkv.xuanzx.com

Java: Executors.newFixedThreadPool(4)
来源：http://buo.yonumen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gtq.ydzc1.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ryh.tian-w.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wzq.tanke756.top

[O03] 加锁保护共享数据
来源：http://oxk.redwolf501.top

Py:   with lock: shared += 1
来源：http://omp.jinqigfzy.top

PHP:  // 用 flock() 做文件锁
来源：http://swx.shangyingyoupin.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nyb.hnxiangtu.top

TS:   // 同 JS
来源：http://iuo.pycfn.com

Java: synchronized (this) { shared++; }
来源：http://jgv.xuetiantiany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mxq.hywenlv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vfa.yonumen.top

C#:   lock (gate) { shared++; }
来源：http://pva.fktsv.cn

[O04] 定义异步函数并等待
来源：http://sfz.feifeiyinyue.top

Py:   async def f():⏎    await g()
来源：http://dgc.andypj.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zzn.aibaodan.cn

JS:   async function f() { await g(); }
来源：http://pqc.ehwqpu.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://vql.cucudq.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://obl.yuxming.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hiy.ydzc1.top

Ruby: # 用 Fiber 或 async gem
来源：http://rxf.9152youxi.cn

C#:   async Task F() { await G(); }
来源：http://wqv.tanke756.top

[O05] 并发执行并等待全部完成
来源：http://nbw.yueranfly.top

Py:   asyncio.gather(*tasks)
来源：http://vpu.smart0.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qns.zdbjq.cn

JS:   await Promise.all(tasks)
来源：http://qqr.hywenlv.cn

TS:   await Promise.all(tasks)
来源：http://vts.sxryk.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://trr.zhijiandao.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://orz.birdmap.top

Ruby: threads.map(&:join)
来源：http://dap.hfpthk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ygq.ppjwa.cn

[O06] 使用进程池
来源：http://uen.zhengqikj.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pho.daxiang520.top

PHP:  // pcntl_fork 或多进程队列
来源：http://oij.zhoulong.xyz

JS:   // child_process / cluster 模块
来源：http://izr.ehwqpu.com

TS:   // child_process / cluster 模块
来源：http://tqq.sxryk.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bkn.jqgfzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ajr.jinqigufen.top

Ruby: // fork 块
来源：http://lml.shuidangran.top

C#:   Parallel.For
来源：http://tln.tianlin.xyz

================================================================================
来源：http://jbf.yj20258.top

P. 常用工具函数
来源：http://oyk.wangdashe.top

================================================================================
来源：http://cnm.daria6918.cn

[P01] 生成 UUID
来源：http://dvv.pengpengdd.cyou

Py:   str(uuid.uuid4())
来源：http://sro.gzhubu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zaj.fehbvm.com

JS:   crypto.randomUUID()
来源：http://gzq.aibaodan.cn

TS:   crypto.randomUUID()
来源：http://mcb.tanke756.top

Java: UUID.randomUUID().toString()
来源：http://sob.vqdsnc.cn

Go:   // 用 github.com/google/uuid
来源：http://pej.bbcook.cn

Ruby: SecureRandom.uuid
来源：http://ljh.dashuyun.cn

C#:   Guid.NewGuid().ToString()
来源：http://ple.hfpthk.cn

[P02] MD5 / SHA256 摘要
来源：http://gto.daria6918.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jdm.kuanghao11.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://uuf.vqdsnc.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fwv.yfazqb.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ptg.chenjidiqi.icu

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://owy.cashguo.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://geu.haohaochexian.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qhd.zhiwuduotai.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gmu.yonumen.top

[P03] 生成短随机字符串
来源：http://nwt.zhixingplan.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jbo.cdnleiting.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gwl.jianghu66.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jcm.tarul.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wxw.fengsongda.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lcp.jiagoushi.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lxh.jlsjyb.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://akv.nanxinkj.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sla.xylfe.cn

[P04] 求长度
来源：http://nes.feifeiyinyue.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jur.ehwqpu.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dym.fzhhl.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mhq.cucudq.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kiu.cdnleiting.top

Java: list.size();  map.size();  s.length()
来源：http://hjy.shanyushiyangtech.top

Go:   len(arr);  len(m)
来源：http://iiu.sysykeji.top

Ruby: x.length;  x.size
来源：http://rep.meibo888.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://yfu.xingfuxueyuan.xyz

[P05] 判断两个对象内容是否相等
来源：http://prl.ydzc1.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://uuz.shanyushiyangtech.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yww.yj20258.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zrd.zhongyouzk.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jlp.hesvh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rsz.hcnkem.com

Go:   reflect.DeepEqual(a, b)
来源：http://iij.yj20258888.top

Ruby: a == b
来源：http://okv.9152youxi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xxj.pycfn.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ddz.yvedp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gpo.hcnkem.com

PHP:  if (empty($x)) {}
来源：http://qxh.xingfuxueyuan.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ipp.haohaochexian.top

TS:   if (x == null) {}
来源：http://ges.fktsv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://onl.chenjidiqi.icu

Go:   if x == nil {}
来源：http://ivn.wangdashe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://orl.sufxvd.cn

C#:   if (x is null) {}
来源：http://lpr.guannengcc.top

[P07] 防抖与节流
来源：http://ynb.hywenlv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gpn.sjlbkw.cn

PHP:  // 手写时间戳比较
来源：http://tpz.hammf.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ofm.gotoacloud.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zip.tian-w.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qse.cdnleiting.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gim.hywenlv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vpe.daxiang520.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ogj.cucudq.cn

[P08] 处理浮点精度问题
来源：http://omj.wangdashe.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wsw.jianghu66.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nvq.andypj.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xfu.iojbl.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hid.yueranfly.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zjb.yj20258.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yav.dashuyun.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://axq.haohaochexian.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cpg.gzhubu.top

================================================================================
来源：http://gjj.mhx1999.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xix.tianlin.xyz

================================================================================
来源：http://qzi.smart0.xyz

[Q01] 创建表
来源：http://fkj.jqgufenzy.top

CREATE TABLE users (
来源：http://oad.uphjek.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://szm.jqgufenzy.top

name VARCHAR(50) NOT NULL,
来源：http://aay.xuetiantiany.cn

email VARCHAR(100) UNIQUE,
来源：http://jea.redwolf501.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://orj.cheryme.top

);
来源：http://vez.iojbl.cn

[Q02] 创建带外键的表
来源：http://fje.jianghu66.top

CREATE TABLE orders (
来源：http://ynt.zhixingplan.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xbg.bjfxy.top

user_id INT NOT NULL,
来源：http://dak.ivvv.top

amount DECIMAL(10, 2),
来源：http://zek.zhiwuduotai.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kky.zhoulong.xyz

);
来源：http://ehi.yvedp.cn

[Q03] 增加列
来源：http://ori.hnqzz.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cak.smart0.xyz

[Q04] 修改列类型
来源：http://uln.hammf.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cmc.xylfe.cn

[Q05] 重命名列
来源：http://asn.hysaishi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qvy.sjlbkw.cn

[Q06] 删除列
来源：http://vll.c1oappe.top

ALTER TABLE users DROP COLUMN age;
来源：http://dcg.redwolf501.top

[Q07] 删除表
来源：http://adk.zdqjudy.top

DROP TABLE IF EXISTS orders;
来源：http://pqn.yueranfly.top

[Q08] 创建普通索引
来源：http://mrg.xuanzx.com

CREATE INDEX idx_users_email ON users(email);
来源：http://tko.bjfxy.top

[Q09] 创建唯一索引
来源：http://zfc.sysykeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ful.yongpay.top

[Q10] 插入单行
来源：http://wgj.ivvv.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xbl.0kj1m.cn

[Q11] 一次插入多行
来源：http://oyv.yangfankeji.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dcf.chenlongwang.top

[Q12] 插入后取自增 ID
来源：http://rns.zhiwuduotai.top

INSERT INTO users (name) VALUES ('C');
来源：http://uup.hysaishi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wbk.jinyuanbaomall.cn

[Q13] 忽略重复插入
来源：http://bot.andypj.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uty.andypj.xyz

[Q14] 存在则更新（upsert）
来源：http://hvj.ywan-chungtsiang.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vsx.xuanzx.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://spg.aibaodan.cn

[Q15] 查询全部
来源：http://uok.tarul.cn

SELECT * FROM users;
来源：http://irn.yfazqb.com

[Q16] 查询指定列
来源：http://dlf.guowangkeji.top

SELECT id, name FROM users;
来源：http://sly.nanxinkj.top

[Q17] 条件查询
来源：http://dvm.yongpay.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gxo.bjfxy.top

[Q18] 模糊匹配
来源：http://epv.epnwcf.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ocl.zhaomingkeji.xyz

[Q19] 范围查询
来源：http://gwh.smart0.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bmk.xuanzx.com

[Q20] IN 列表
来源：http://kxi.redwolf501.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wex.sysykeji.top

[Q21] 空值判断
来源：http://uxq.chenjidiqi.icu

SELECT * FROM users WHERE email IS NULL;
来源：http://kki.yonumen.top

[Q22] 排序
来源：http://amy.hysaishi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bvq.yj20258888.top

[Q23] 分页
来源：http://lzg.dianchejie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ovw.aibaodan.cn

[Q24] 去重
来源：http://xbj.zhongyouzk.top

SELECT DISTINCT city FROM users;
来源：http://mey.yj20258888.top

[Q25] 只取前 N 条
来源：http://sdv.jiagoushi.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vsb.zhaomingkeji.xyz

[Q26] 计数
来源：http://qvl.yongpay.top

SELECT COUNT(*) FROM users;
来源：http://puh.wangdashe.top

[Q27] 条件计数
来源：http://yag.mhx1999.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kkk.jianghu66.top

[Q28] 求和与平均
来源：http://iwf.zhengqikj.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uhl.sxryk.cn

[Q29] 最大最小值
来源：http://qun.fengsongda.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://itx.ywan-chungtsiang.top

[Q30] 分组统计
来源：http://kcv.meibo888.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bmy.ehwqpu.com

[Q31] 分组后过滤
来源：http://mdy.yuxming.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hum.nanxinkj.top

[Q32] 分组拼接字符串
来源：http://hog.gaohongyu789.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uxz.sweek.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fde.chenzaomai.com

[Q33] 多列分组
来源：http://vls.sjlbkw.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kxb.cdnleiting.top

[Q34] 每组取第一条
来源：http://xet.zdbjq.cn

SELECT * FROM (
来源：http://yap.daria6918.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://upp.smart0.xyz

) t WHERE rn = 1;
来源：http://hic.jinqigufen.top

[Q35] 内连接
来源：http://qvl.9152youxi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qfz.kuanghao11.cn

[Q36] 左连接
来源：http://ked.yj20258888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ycq.cdnleiting.top

[Q37] 右连接
来源：http://whk.52xcode.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zyl.feifeiyinyue.top

[Q38] 全外连接（PostgreSQL）
来源：http://xsk.xinyue.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vsy.zhengqikj.top

[Q39] 自连接（查上下级）
来源：http://jzo.feifeiyinyue.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ijd.yangfankeji.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ujx.mhx1999.top

[Q40] 交叉连接（笛卡尔积）
来源：http://auq.xuanzx.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://srv.svipenyu.cn

[Q41] 多表连接
来源：http://yxm.vqdsnc.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://brs.mhx1999.top

JOIN users u ON u.id = o.user_id
来源：http://lmc.kuanghao11.cn

JOIN products p ON p.id = o.product_id;
来源：http://pvw.cheryme.top

[Q42] 连接条件附加过滤
来源：http://umk.jinqigufen.top

SELECT u.name, o.amount FROM users u
来源：http://iwb.yuanzhike.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://swt.316326.xyz

[Q43] 标量子查询
来源：http://bqb.cucudq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://guv.shangyingyoupin.top

[Q44] IN 子查询
来源：http://nog.9152youxi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fhz.sweek.top

[Q45] EXISTS 判断存在
来源：http://dad.shuidangran.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ibv.xylfe.cn

[Q46] NOT EXISTS 判断不存在
来源：http://prf.yj20258.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fwq.meibo888.top

[Q47] 与平均值比较
来源：http://bpr.zycfv.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kxj.uphjek.com

[Q48] CTE 公用表表达式
来源：http://rsg.xziqi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yor.redwolf501.top

SELECT * FROM t WHERE c > 5;
来源：http://ing.guowangkeji.top

[Q49] 更新单行
来源：http://ogj.fengsongda.top


<!-- 参考信息 -->