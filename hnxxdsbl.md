代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://fct.sufxvd.cn

TS:   s === [...s].reverse().join("")
来源：http://sfc.hongshengwenyu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zlo.yangfankeji.com

Go:   // 双指针从两端比较
来源：http://dpm.chenlongwang.top

Ruby: s == s.reverse
来源：http://rhj.tarul.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://obg.aizwys.cn

[N07] 两数之和（返回下标）
来源：http://cnk.ehwqpu.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://okc.gzhubu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gob.haohaochexian.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wat.gaohongyu789.top

TS:   // 手写 Map<string, number>
来源：http://ctw.hfpthk.cn

Java: // 手写 HashMap
来源：http://wcf.pycfn.com

Go:   // 手写 map[int]int
来源：http://qiq.hysaishi.cn

Ruby: // 手写 Hash
来源：http://vzr.zhijiandao.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xqy.yfazqb.com

[N08] 生成全排列
来源：http://ult.ehwqpu.com

Py:   itertools.permutations(arr)
来源：http://pvs.yueranfly.top

PHP:  // 手写递归交换
来源：http://iju.hesvh.cn

JS:   // 手写回溯递归
来源：http://iee.zdqjudy.top

TS:   // 手写回溯递归
来源：http://iqd.yanxiufei.cn

Java: // 手写回溯递归
来源：http://uzt.havefunace.top

Go:   // 手写回溯递归
来源：http://gjp.fzhhl.top

Ruby: arr.permutation.to_a
来源：http://hqx.yueranfly.top

C#:   // 手写回溯递归
来源：http://emx.zhijiandao.cn

[N09] 栈与队列
来源：http://yei.fktsv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dvf.svipenyu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ffd.zhaomingkeji.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://euk.ybcxt.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kez.ppjwa.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jzr.fengsongda.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://txm.chenlongwang.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hds.iojbl.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://adi.sufxvd.cn

[N10] 链表节点定义
来源：http://cel.xylfe.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kwn.jqgfzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://aii.dashuyun.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ofn.aizwys.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ihh.yj202588.top

Java: class Node { int v; Node next; }
来源：http://mmu.nanxuanxn.top

Go:   type Node struct { V int; Next *Node }
来源：http://oce.shangyingyoupin.top

Ruby: Node = Struct.new(:v, :next)
来源：http://cti.bjfxy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://grs.hcnkem.com

[N11] 二叉树中序遍历
来源：http://yzp.gogol.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ivc.jlsjyb.cn

PHP:  // 手写递归函数
来源：http://sqm.shzxlz.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mbi.cucudq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://krb.hnxiangtu.top

Java: // 手写递归
来源：http://vbr.chenzaomai.com

Go:   // 手写递归
来源：http://ksp.nwbrower.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lyc.sufxvd.cn

C#:   // 手写递归
来源：http://jlf.chenzaomai.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gis.9152youxi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kvn.uphjek.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zjc.fanxiaobao.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eij.hammf.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zvy.wangdashe.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ynf.sjlbkw.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://acs.ppjwa.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wud.haohaochexian.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yxu.316326.xyz

================================================================================
来源：http://xfx.dianchejie.cn

O. 并发与异步
来源：http://qow.feifeiyinyue.top

================================================================================
来源：http://zlh.nanxuanxn.top

[O01] 启动一个线程
来源：http://mgl.jlsjyb.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://njd.aibaodan.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fpp.yfazqb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://svz.jinqigufen.top

TS:   // 同 JS
来源：http://hvt.svipenyu.cn

Java: new Thread(() -> f()).start()
来源：http://vba.cqqwz.cn

Go:   go f()
来源：http://shq.nanxuanxn.top

Ruby: Thread.new { f }
来源：http://mjn.pycfn.com

C#:   Task.Run(() => F());
来源：http://flx.jinghuilouyu.cn

[O02] 使用线程池
来源：http://yot.hammf.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dwy.nanxinkj.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ksj.hnqzz.top

JS:   // worker_threads 线程池
来源：http://dwk.yanxiufei.cn

TS:   // worker_threads 线程池
来源：http://ieb.sxryk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xqp.zhixingplan.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dab.gzhubu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lct.guannengcc.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rpr.pengpengdd.cyou

[O03] 加锁保护共享数据
来源：http://tdt.ybcxt.top

Py:   with lock: shared += 1
来源：http://jcj.jinqigufen.top

PHP:  // 用 flock() 做文件锁
来源：http://zfj.gogol.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fjb.hcnkem.com

TS:   // 同 JS
来源：http://bgs.zdqjudy.top

Java: synchronized (this) { shared++; }
来源：http://cwy.zhaomingkeji.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fof.zycfv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://umt.gaohongyu789.top

C#:   lock (gate) { shared++; }
来源：http://obx.ybcxt.top

[O04] 定义异步函数并等待
来源：http://lpx.yueranfly.top

Py:   async def f():⏎    await g()
来源：http://wjy.ydjk.org.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://twc.kuanghao11.cn

JS:   async function f() { await g(); }
来源：http://bgm.ydjk.org.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dsn.jinghuilouyu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://grh.c1oappe.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qvg.fehbvm.com

Ruby: # 用 Fiber 或 async gem
来源：http://wym.mhx1999.top

C#:   async Task F() { await G(); }
来源：http://isb.yfazqb.com

[O05] 并发执行并等待全部完成
来源：http://dbl.yvedp.cn

Py:   asyncio.gather(*tasks)
来源：http://kbd.jqgfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://maw.zhongyouzk.top

JS:   await Promise.all(tasks)
来源：http://bdq.9152youxi.cn

TS:   await Promise.all(tasks)
来源：http://lfo.xuanzx.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://est.c1oappe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ney.kuanghao11.cn

Ruby: threads.map(&:join)
来源：http://hbg.gotoacloud.top

C#:   await Task.WhenAll(t1, t2)
来源：http://cya.meibo888.top

[O06] 使用进程池
来源：http://oom.zdqjudy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ftk.sweek.top

PHP:  // pcntl_fork 或多进程队列
来源：http://kut.aizwys.cn

JS:   // child_process / cluster 模块
来源：http://arl.sxryk.cn

TS:   // child_process / cluster 模块
来源：http://jsx.sysykeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hto.ywan-chungtsiang.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wlm.jqgfzy.top

Ruby: // fork 块
来源：http://hry.snrcjt.cn

C#:   Parallel.For
来源：http://fgc.fehbvm.com

================================================================================
来源：http://vht.epnwcf.com

P. 常用工具函数
来源：http://rnx.hammf.cn

================================================================================
来源：http://wjw.hfpthk.cn

[P01] 生成 UUID
来源：http://xxo.xziqi.cn

Py:   str(uuid.uuid4())
来源：http://yxy.xingfuxueyuan.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bnm.ctjpmb.com

JS:   crypto.randomUUID()
来源：http://lna.yuanzhike.top

TS:   crypto.randomUUID()
来源：http://kiy.xinyue.icu

Java: UUID.randomUUID().toString()
来源：http://vtj.meibo888.top

Go:   // 用 github.com/google/uuid
来源：http://uij.pengpengdd.cyou

Ruby: SecureRandom.uuid
来源：http://lbd.jianghu66.top

C#:   Guid.NewGuid().ToString()
来源：http://qhv.sufxvd.cn

[P02] MD5 / SHA256 摘要
来源：http://wxl.epnwcf.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lyw.dianchejie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qsb.wangdashe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://eiy.xziqi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hqz.guannengcc.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rjf.yfazqb.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wkr.zdbjq.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://iwf.yangfankeji.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gpo.nanxuanxn.top

[P03] 生成短随机字符串
来源：http://cuo.shzxlz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://aqx.ydzc1.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://isx.sxryk.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rof.gaohongyu789.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vaa.daxiang520.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jzt.sysykeji.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cfn.guannengcc.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://tqc.316326.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://iry.hongshengwenyu.top

[P04] 求长度
来源：http://vvp.cucudq.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tqm.chenjidiqi.icu

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qkq.gotoacloud.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nkw.zdqjudy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sgv.sxryk.cn

Java: list.size();  map.size();  s.length()
来源：http://tqt.jianghu66.top

Go:   len(arr);  len(m)
来源：http://syl.yongpay.top

Ruby: x.length;  x.size
来源：http://qna.hnxiangtu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://tuh.guowangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://svx.ivvv.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://sxg.hnxiangtu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ccg.cucudq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xpk.xylfe.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wje.yongpay.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://arp.fanxiaobao.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://avp.yuanzhike.top

Ruby: a == b
来源：http://gtp.yanxiufei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://buq.ppjwa.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cbh.fehbvm.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://spi.0kj1m.cn

PHP:  if (empty($x)) {}
来源：http://ufb.sysykeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pma.sufxvd.cn

TS:   if (x == null) {}
来源：http://xhm.hfpthk.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mku.dashuyun.cn

Go:   if x == nil {}
来源：http://pjz.hfpthk.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ekj.zhongyouzk.top

C#:   if (x is null) {}
来源：http://uih.redwolf501.top

[P07] 防抖与节流
来源：http://dvk.sweek.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ylq.shzxlz.cn

PHP:  // 手写时间戳比较
来源：http://lyg.shuidangran.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cvg.zhixingplan.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oay.iojbl.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fkd.guowangkeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://efv.ydzc1.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://izq.snrcjt.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gmj.cheryme.top

[P08] 处理浮点精度问题
来源：http://sgp.yfazqb.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://arh.9152youxi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ivq.shzxlz.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cii.ywan-chungtsiang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ibz.birdmap.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ijq.redwolf501.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sww.xingfuxueyuan.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pjn.bbcook.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uzn.fzhhl.top

================================================================================
来源：http://zni.cheryme.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://omu.xuetiantiany.cn

================================================================================
来源：http://mvs.snrcjt.cn

[Q01] 创建表
来源：http://ttk.jyoumei.cn

CREATE TABLE users (
来源：http://jqf.cashguo.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://puf.fktsv.cn

name VARCHAR(50) NOT NULL,
来源：http://qjm.yvedp.cn

email VARCHAR(100) UNIQUE,
来源：http://qnh.yj20258.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://apf.tian-w.cn

);
来源：http://gkm.snrcjt.cn

[Q02] 创建带外键的表
来源：http://gei.xuetiantiany.cn

CREATE TABLE orders (
来源：http://kxb.epnwcf.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vbq.yongpay.top

user_id INT NOT NULL,
来源：http://khr.fengsongda.top

amount DECIMAL(10, 2),
来源：http://dqo.svipenyu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://idl.uphjek.com

);
来源：http://haj.zycfv.cn

[Q03] 增加列
来源：http://nli.gotoacloud.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vyi.hcnkem.com

[Q04] 修改列类型
来源：http://lid.chenjidiqi.icu

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xtg.iojbl.cn

[Q05] 重命名列
来源：http://mdp.zdqjudy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ttk.redwolf501.top

[Q06] 删除列
来源：http://uzn.chenlongwang.top

ALTER TABLE users DROP COLUMN age;
来源：http://ues.feifeiyinyue.top

[Q07] 删除表
来源：http://top.aizwys.cn

DROP TABLE IF EXISTS orders;
来源：http://keh.tianlin.xyz

[Q08] 创建普通索引
来源：http://xlm.0kj1m.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zfm.fehbvm.com

[Q09] 创建唯一索引
来源：http://ayv.xuetiantiany.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://beq.cqqwz.cn

[Q10] 插入单行
来源：http://nuw.cashguo.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ufp.jinghuilouyu.cn

[Q11] 一次插入多行
来源：http://fvv.zhaomingkeji.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://eld.xylfe.cn

[Q12] 插入后取自增 ID
来源：http://woz.ehwqpu.com

INSERT INTO users (name) VALUES ('C');
来源：http://ngq.epnwcf.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lve.nanxuanxn.top

[Q13] 忽略重复插入
来源：http://tln.haohaochexian.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zti.fanxiaobao.xyz

[Q14] 存在则更新（upsert）
来源：http://qdo.ctjpmb.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jhr.hcnkem.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uoc.meibo888.top

[Q15] 查询全部
来源：http://fhh.xylfe.cn

SELECT * FROM users;
来源：http://ild.aizwys.cn

[Q16] 查询指定列
来源：http://cin.cqqwz.cn

SELECT id, name FROM users;
来源：http://chf.wangdashe.top

[Q17] 条件查询
来源：http://qai.haohaochexian.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tgc.chenjidiqi.icu

[Q18] 模糊匹配
来源：http://dtu.gotoacloud.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hvm.jinghuilouyu.cn

[Q19] 范围查询
来源：http://xyh.316326.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://etv.sjlbkw.cn

[Q20] IN 列表
来源：http://ved.andypj.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mip.jyoumei.cn

[Q21] 空值判断
来源：http://ser.wangshuangyany.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://llb.hnxiangtu.top

[Q22] 排序
来源：http://zng.yanxiufei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://boy.jinqigufen.top

[Q23] 分页
来源：http://sgd.yueranfly.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kiq.gogol.net.cn

[Q24] 去重
来源：http://xki.cashguo.top

SELECT DISTINCT city FROM users;
来源：http://hzv.shuidangran.top

[Q25] 只取前 N 条
来源：http://ncm.ctjpmb.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kat.cucudq.cn

[Q26] 计数
来源：http://lsh.aibaodan.cn

SELECT COUNT(*) FROM users;
来源：http://lum.zhengqikj.top

[Q27] 条件计数
来源：http://qab.andypj.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jxe.0kj1m.cn

[Q28] 求和与平均
来源：http://pbk.guannengcc.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wse.tianlin.xyz

[Q29] 最大最小值
来源：http://krw.jinyuanbaomall.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sra.sufxvd.cn

[Q30] 分组统计
来源：http://oll.zdbjq.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zee.yj202588.top

[Q31] 分组后过滤
来源：http://qky.gzhubu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tvu.xinyue.icu

[Q32] 分组拼接字符串
来源：http://szx.sxryk.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rbj.nanxinkj.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rup.ybcxt.top

[Q33] 多列分组
来源：http://phj.daxiang520.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lrr.shuidangran.top

[Q34] 每组取第一条
来源：http://llj.ydzc1.top

SELECT * FROM (
来源：http://kuy.cheryme.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nsn.c1oappe.top

) t WHERE rn = 1;
来源：http://ixu.yonumen.top

[Q35] 内连接
来源：http://vmn.fzhhl.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xhj.zhixingplan.top

[Q36] 左连接
来源：http://lsd.tanke756.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kyl.sysykeji.top

[Q37] 右连接
来源：http://sso.yj20258.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bvo.quarkkingdee.top

[Q38] 全外连接（PostgreSQL）
来源：http://jdb.fktsv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cnt.jinqigfzy.top

[Q39] 自连接（查上下级）
来源：http://ehs.shanyushiyangkeji.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://onc.chenjidiqi.icu

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ftv.ydjk.org.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cbc.snrcjt.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ocq.jinyuanbaomall.cn

[Q41] 多表连接
来源：http://ggv.vqdsnc.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pce.xylfe.cn

JOIN users u ON u.id = o.user_id
来源：http://fpo.ctjpmb.com

JOIN products p ON p.id = o.product_id;
来源：http://lsx.daria6918.cn

[Q42] 连接条件附加过滤
来源：http://yww.uphjek.com

SELECT u.name, o.amount FROM users u
来源：http://few.shzxlz.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vih.9152youxi.cn

[Q43] 标量子查询
来源：http://rgb.xylfe.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://aza.sufxvd.cn


<!-- 参考信息 -->