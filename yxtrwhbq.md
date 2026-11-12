代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mvz.shzxlz.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bhh.yuxming.cn

TS:   // 手写 Map<string, number>
来源：http://woz.hnxiangtu.top

Java: // 手写 HashMap
来源：http://tpj.svipenyu.cn

Go:   // 手写 map[int]int
来源：http://npp.wangdashe.top

Ruby: // 手写 Hash
来源：http://lvk.zdqjudy.top

C#:   // 手写 Dictionary<int, int>
来源：http://hvc.pengpengdd.cyou

[N08] 生成全排列
来源：http://hcf.kuanghao11.cn

Py:   itertools.permutations(arr)
来源：http://wri.fanxiaobao.xyz

PHP:  // 手写递归交换
来源：http://ayu.yongpay.top

JS:   // 手写回溯递归
来源：http://gsy.pycfn.com

TS:   // 手写回溯递归
来源：http://pww.yfazqb.com

Java: // 手写回溯递归
来源：http://aba.aibaodan.cn

Go:   // 手写回溯递归
来源：http://mmi.shzxlz.cn

Ruby: arr.permutation.to_a
来源：http://qnw.hnxiangtu.top

C#:   // 手写回溯递归
来源：http://cct.zdbjq.cn

[N09] 栈与队列
来源：http://cjt.chenjidiqi.icu

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lap.chenzaomai.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ivt.hongshengwenyu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lpr.pycfn.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oig.nanxinkj.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qsm.shanyushiyangtech.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sxb.hysaishi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://krt.xinyue.icu

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fbk.zhixingplan.top

[N10] 链表节点定义
来源：http://qth.feifeiyinyue.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ugq.52xcode.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xae.jinqigfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rku.xuanzx.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ice.aizwys.cn

Java: class Node { int v; Node next; }
来源：http://sro.ydzc1.top

Go:   type Node struct { V int; Next *Node }
来源：http://bmk.yj20258888.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zxt.meibo888.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wij.cashguo.top

[N11] 二叉树中序遍历
来源：http://mqx.aizwys.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ior.jianghu66.top

PHP:  // 手写递归函数
来源：http://ode.jiagoushi.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ylr.gogol.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kpt.birdmap.top

Java: // 手写递归
来源：http://hwj.aibaodan.cn

Go:   // 手写递归
来源：http://xmg.ydjk.org.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ghz.quarkkingdee.top

C#:   // 手写递归
来源：http://sdy.hfpthk.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ecv.hammf.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xdd.bjfxy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://opx.xuetiantiany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ocz.epnwcf.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bfy.nanxuanxn.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wow.hnqzz.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://unp.0kj1m.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ktd.cqqwz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://btj.tanke756.top

================================================================================
来源：http://fpe.zhongyouzk.top

O. 并发与异步
来源：http://lez.quarkkingdee.top

================================================================================
来源：http://jom.tanke756.top

[O01] 启动一个线程
来源：http://mxh.tianlin.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bnx.yj20258888.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ndh.ctjpmb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vyg.316326.xyz

TS:   // 同 JS
来源：http://vxh.shanyushiyangkeji.top

Java: new Thread(() -> f()).start()
来源：http://dit.0kj1m.cn

Go:   go f()
来源：http://zke.yuanzhike.top

Ruby: Thread.new { f }
来源：http://gop.fktsv.cn

C#:   Task.Run(() => F());
来源：http://xqk.ywan-chungtsiang.top

[O02] 使用线程池
来源：http://uwu.yuanzhike.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pmc.smart0.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dut.feifeiyinyue.top

JS:   // worker_threads 线程池
来源：http://xuy.gaohongyu789.top

TS:   // worker_threads 线程池
来源：http://dje.wangshuangyany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kip.yj202588.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cck.fehbvm.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zap.hfpthk.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tcl.andypj.xyz

[O03] 加锁保护共享数据
来源：http://aqc.vqdsnc.cn

Py:   with lock: shared += 1
来源：http://lkk.ehwqpu.com

PHP:  // 用 flock() 做文件锁
来源：http://zdc.feifeiyinyue.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://soi.zycfv.cn

TS:   // 同 JS
来源：http://phs.jinqigfzy.top

Java: synchronized (this) { shared++; }
来源：http://kuf.yvedp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tvz.andypj.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://hjh.zhiwuduotai.top

C#:   lock (gate) { shared++; }
来源：http://cgo.fengsongda.top

[O04] 定义异步函数并等待
来源：http://dwz.yj20258888.top

Py:   async def f():⏎    await g()
来源：http://upe.yfazqb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://scf.ehwqpu.com

JS:   async function f() { await g(); }
来源：http://gfq.zhixingplan.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://qee.svipenyu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fqu.daxiang520.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yoe.yvedp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zxq.yj202588.top

C#:   async Task F() { await G(); }
来源：http://lzj.shuidangran.top

[O05] 并发执行并等待全部完成
来源：http://tbp.xziqi.cn

Py:   asyncio.gather(*tasks)
来源：http://ilr.hcnkem.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://iat.shangyingyoupin.top

JS:   await Promise.all(tasks)
来源：http://xsi.gogol.net.cn

TS:   await Promise.all(tasks)
来源：http://oxa.fktsv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ahe.vehdjk.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tgf.jlsjyb.cn

Ruby: threads.map(&:join)
来源：http://iyk.cheryme.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fgt.jyoumei.cn

[O06] 使用进程池
来源：http://ccf.zhongyouzk.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pqm.shanyushiyangtech.top

PHP:  // pcntl_fork 或多进程队列
来源：http://uvi.jyoumei.cn

JS:   // child_process / cluster 模块
来源：http://fvg.hnqzz.top

TS:   // child_process / cluster 模块
来源：http://ngo.havefunace.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ivy.aibaodan.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mto.9152youxi.cn

Ruby: // fork 块
来源：http://mas.daria6918.cn

C#:   Parallel.For
来源：http://uwf.fktsv.cn

================================================================================
来源：http://gfw.aibaodan.cn

P. 常用工具函数
来源：http://vnt.aibaodan.cn

================================================================================
来源：http://dap.sxryk.cn

[P01] 生成 UUID
来源：http://ebj.fengsongda.top

Py:   str(uuid.uuid4())
来源：http://zfn.jinyuanbaomall.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dqw.shangyingyoupin.top

JS:   crypto.randomUUID()
来源：http://sou.9152youxi.cn

TS:   crypto.randomUUID()
来源：http://awu.xingfuxueyuan.xyz

Java: UUID.randomUUID().toString()
来源：http://ryf.zdbjq.cn

Go:   // 用 github.com/google/uuid
来源：http://npv.fengsongda.top

Ruby: SecureRandom.uuid
来源：http://vhm.gotoacloud.top

C#:   Guid.NewGuid().ToString()
来源：http://qui.zhiwuduotai.top

[P02] MD5 / SHA256 摘要
来源：http://gqv.zycfv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rar.nwbrower.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ipw.cucudq.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qng.ctjpmb.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tbd.sxryk.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cnp.nanxinkj.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://huw.zdqjudy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://eba.hcnkem.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ehq.shanyushiyangtech.top

[P03] 生成短随机字符串
来源：http://jqe.jianghu66.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jev.zycfv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uzp.ydjk.org.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dyy.dianchejie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xxm.sysykeji.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lgg.ywan-chungtsiang.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yyn.hnxiangtu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ztt.nanxuanxn.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uua.bbcook.cn

[P04] 求长度
来源：http://tjh.yueranfly.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pqi.hfpthk.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iqk.jiagoushi.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ixr.chenzaomai.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lwp.sufxvd.cn

Java: list.size();  map.size();  s.length()
来源：http://fng.wangshuangyany.cn

Go:   len(arr);  len(m)
来源：http://svy.gaohongyu789.top

Ruby: x.length;  x.size
来源：http://ser.zhiwuduotai.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gme.uphjek.com

[P05] 判断两个对象内容是否相等
来源：http://bzv.kuanghao11.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lgm.gaohongyu789.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ejp.9152youxi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zcn.9152youxi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jzk.zycfv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pdk.xingfuxueyuan.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://pqh.bbcook.cn

Ruby: a == b
来源：http://tsm.meibo888.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gnr.xuetiantiany.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ixt.shangyingyoupin.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iaf.shanyushiyangtech.top

PHP:  if (empty($x)) {}
来源：http://euv.yangfankeji.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cej.zhongyouzk.top

TS:   if (x == null) {}
来源：http://lai.c1oappe.top

Java: if (x == null || x.isEmpty()) {}
来源：http://qrl.wangshuangyany.cn

Go:   if x == nil {}
来源：http://uzd.xziqi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jwv.yuanzhike.top

C#:   if (x is null) {}
来源：http://fen.cqqwz.cn

[P07] 防抖与节流
来源：http://kcm.zycfv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xgt.ppjwa.cn

PHP:  // 手写时间戳比较
来源：http://mnw.zycfv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fdg.zhoulong.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vzb.ybcxt.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hkk.sufxvd.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://oik.fehbvm.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://bro.ybcxt.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tdk.yongpay.top

[P08] 处理浮点精度问题
来源：http://isp.cheryme.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://acw.yueranfly.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rim.chenzaomai.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://usr.fktsv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://eba.zhengqikj.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xvy.chenlongwang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rfl.jianghu66.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://umq.tanke756.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ikm.redwolf501.top

================================================================================
来源：http://gjh.yonumen.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://iit.zdqjudy.top

================================================================================
来源：http://rqj.bbcook.cn

[Q01] 创建表
来源：http://mys.ivvv.top

CREATE TABLE users (
来源：http://ikj.yongpay.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fjn.hcnkem.com

name VARCHAR(50) NOT NULL,
来源：http://hrg.yuxming.cn

email VARCHAR(100) UNIQUE,
来源：http://nbb.meibo888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pqh.dianchejie.cn

);
来源：http://nvo.ydzc1.top

[Q02] 创建带外键的表
来源：http://wrw.yfazqb.com

CREATE TABLE orders (
来源：http://tgd.wangshuangyany.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://goi.xylfe.cn

user_id INT NOT NULL,
来源：http://rmq.tianlin.xyz

amount DECIMAL(10, 2),
来源：http://qay.svipenyu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uxq.shanyushiyangtech.top

);
来源：http://zmv.nanxuanxn.top

[Q03] 增加列
来源：http://hur.shanyushiyangtech.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://iww.iojbl.cn

[Q04] 修改列类型
来源：http://lhp.aizwys.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xdr.yueranfly.top

[Q05] 重命名列
来源：http://mjk.sweek.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lgw.zhengqikj.top

[Q06] 删除列
来源：http://kmi.sysykeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://eff.52xcode.cn

[Q07] 删除表
来源：http://bbd.epnwcf.com

DROP TABLE IF EXISTS orders;
来源：http://fjt.cqqwz.cn

[Q08] 创建普通索引
来源：http://mna.hesvh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tro.yvedp.cn

[Q09] 创建唯一索引
来源：http://afj.snrcjt.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hyn.quarkkingdee.top

[Q10] 插入单行
来源：http://rev.ywan-chungtsiang.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jhk.hnxiangtu.top

[Q11] 一次插入多行
来源：http://ocd.jqgufenzy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ozi.fktsv.cn

[Q12] 插入后取自增 ID
来源：http://lio.sxryk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ome.hesvh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sti.dianchejie.cn

[Q13] 忽略重复插入
来源：http://ayh.cqqwz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jem.dianchejie.cn

[Q14] 存在则更新（upsert）
来源：http://ubp.wangshuangyany.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://msa.ywan-chungtsiang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uto.tarul.cn

[Q15] 查询全部
来源：http://otj.birdmap.top

SELECT * FROM users;
来源：http://cqk.iojbl.cn

[Q16] 查询指定列
来源：http://kaa.yfazqb.com

SELECT id, name FROM users;
来源：http://gjy.jinghuilouyu.cn

[Q17] 条件查询
来源：http://que.smart0.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://guc.jqgufenzy.top

[Q18] 模糊匹配
来源：http://ucw.fengsongda.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jtw.quarkkingdee.top

[Q19] 范围查询
来源：http://zbh.hongshengwenyu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gbe.havefunace.top

[Q20] IN 列表
来源：http://qnz.jiagoushi.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://elt.ehwqpu.com

[Q21] 空值判断
来源：http://orw.sufxvd.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sci.sysykeji.top

[Q22] 排序
来源：http://cgd.guannengcc.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://iep.yj20258.top

[Q23] 分页
来源：http://hqo.jqgfzy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tad.nanxinkj.top

[Q24] 去重
来源：http://rcu.svipenyu.cn

SELECT DISTINCT city FROM users;
来源：http://lnh.redwolf501.top

[Q25] 只取前 N 条
来源：http://kqf.fanxiaobao.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://twv.aizwys.cn

[Q26] 计数
来源：http://kuf.sjlbkw.cn

SELECT COUNT(*) FROM users;
来源：http://thm.havefunace.top

[Q27] 条件计数
来源：http://bjg.yj202588.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qwq.cheryme.top

[Q28] 求和与平均
来源：http://vel.hfpthk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ztl.0kj1m.cn

[Q29] 最大最小值
来源：http://ssv.ivvv.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://eoz.cashguo.top

[Q30] 分组统计
来源：http://kra.smart0.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zlh.ydzc1.top

[Q31] 分组后过滤
来源：http://zlv.yanxiufei.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pff.gaohongyu789.top

[Q32] 分组拼接字符串
来源：http://dae.cdnleiting.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qay.316326.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://duf.jyoumei.cn

[Q33] 多列分组
来源：http://pxp.chenzaomai.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qcd.ydjk.org.cn

[Q34] 每组取第一条
来源：http://xgt.yvedp.cn

SELECT * FROM (
来源：http://vyj.hywenlv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://erx.hywenlv.cn

) t WHERE rn = 1;
来源：http://vyd.guannengcc.top

[Q35] 内连接
来源：http://hlh.snrcjt.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uuj.c1oappe.top

[Q36] 左连接
来源：http://jer.uphjek.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ida.gaohongyu789.top

[Q37] 右连接
来源：http://hpt.zhiwuduotai.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nqh.nanxinkj.top

[Q38] 全外连接（PostgreSQL）
来源：http://ohu.sxryk.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rpe.ywan-chungtsiang.top

[Q39] 自连接（查上下级）
来源：http://not.birdmap.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ykc.ctjpmb.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kcj.jyoumei.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://apj.sjlbkw.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jtf.smart0.xyz

[Q41] 多表连接
来源：http://stm.hammf.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qqt.zhiwuduotai.top

JOIN users u ON u.id = o.user_id
来源：http://jyz.tanke756.top

JOIN products p ON p.id = o.product_id;
来源：http://xbo.hysaishi.cn

[Q42] 连接条件附加过滤
来源：http://xdq.haohaochexian.top

SELECT u.name, o.amount FROM users u
来源：http://hqd.quarkkingdee.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yxz.yfazqb.com

[Q43] 标量子查询
来源：http://woc.redwolf501.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gsx.ybcxt.top

[Q44] IN 子查询
来源：http://xoq.hysaishi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ocs.yonumen.top

[Q45] EXISTS 判断存在
来源：http://bew.cdnleiting.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zaj.andypj.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://brf.vehdjk.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://leg.zhixingplan.top

[Q47] 与平均值比较
来源：http://uyi.zhaomingkeji.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://drs.iojbl.cn


<!-- 参考信息 -->