代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://hco.haohaochexian.top

TS:   s === [...s].reverse().join("")
来源：http://ooj.nwbrower.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xev.hysaishi.cn

Go:   // 双指针从两端比较
来源：http://gzi.fanxiaobao.xyz

Ruby: s == s.reverse
来源：http://zes.gogol.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://swk.sysykeji.top

[N07] 两数之和（返回下标）
来源：http://jic.gzhubu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nkk.shuidangran.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bia.yuanzhike.top

JS:   // 手写 Map：map.set(v, i)
来源：http://jfh.daxiang520.top

TS:   // 手写 Map<string, number>
来源：http://jzc.guannengcc.top

Java: // 手写 HashMap
来源：http://iqp.vehdjk.com

Go:   // 手写 map[int]int
来源：http://bjm.xingfuxueyuan.xyz

Ruby: // 手写 Hash
来源：http://yjt.jlsjyb.cn

C#:   // 手写 Dictionary<int, int>
来源：http://eri.yj20258.top

[N08] 生成全排列
来源：http://xbg.c1oappe.top

Py:   itertools.permutations(arr)
来源：http://kch.yuanzhike.top

PHP:  // 手写递归交换
来源：http://gve.yvedp.cn

JS:   // 手写回溯递归
来源：http://jsd.fehbvm.com

TS:   // 手写回溯递归
来源：http://mne.vqdsnc.cn

Java: // 手写回溯递归
来源：http://uoh.yj20258.top

Go:   // 手写回溯递归
来源：http://rxj.yongpay.top

Ruby: arr.permutation.to_a
来源：http://byf.nanxuanxn.top

C#:   // 手写回溯递归
来源：http://xmx.yuanzhike.top

[N09] 栈与队列
来源：http://dhw.zhixingplan.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rwm.yj202588.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xzi.jianghu66.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://aho.shanyushiyangtech.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bui.xinyue.icu

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://msq.birdmap.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dcl.xingfuxueyuan.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mir.nanxuanxn.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lfb.iojbl.cn

[N10] 链表节点定义
来源：http://ewb.hywenlv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://iwm.xingfuxueyuan.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://smc.xziqi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qjt.yj20258888.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hmz.aizwys.cn

Java: class Node { int v; Node next; }
来源：http://odx.yj202588.top

Go:   type Node struct { V int; Next *Node }
来源：http://jxt.daxiang520.top

Ruby: Node = Struct.new(:v, :next)
来源：http://bja.jqgfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://mck.c1oappe.top

[N11] 二叉树中序遍历
来源：http://lxd.hnxiangtu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fov.daxiang520.top

PHP:  // 手写递归函数
来源：http://cdn.pengpengdd.cyou

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hao.yuanzhike.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gnn.shanyushiyangkeji.top

Java: // 手写递归
来源：http://jcl.zhoulong.xyz

Go:   // 手写递归
来源：http://ubx.shanyushiyangtech.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mup.jqgfzy.top

C#:   // 手写递归
来源：http://vnc.ehwqpu.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lut.cqqwz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sae.birdmap.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zse.dashuyun.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zgz.shzxlz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zuy.jqgufenzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://asj.jinghuilouyu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zlv.tianlin.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fzw.hnxiangtu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://aqn.vqdsnc.cn

================================================================================
来源：http://gkf.hcnkem.com

O. 并发与异步
来源：http://msg.ywan-chungtsiang.top

================================================================================
来源：http://sfa.yuxming.cn

[O01] 启动一个线程
来源：http://xsh.chenlongwang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ura.tian-w.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jon.smart0.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yir.redwolf501.top

TS:   // 同 JS
来源：http://qgz.xziqi.cn

Java: new Thread(() -> f()).start()
来源：http://deg.mhx1999.top

Go:   go f()
来源：http://sfo.jianghu66.top

Ruby: Thread.new { f }
来源：http://gky.hcnkem.com

C#:   Task.Run(() => F());
来源：http://eqj.hnxiangtu.top

[O02] 使用线程池
来源：http://zva.smart0.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fjn.gotoacloud.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wug.yj20258888.top

JS:   // worker_threads 线程池
来源：http://xnn.zycfv.cn

TS:   // worker_threads 线程池
来源：http://tyb.xuanzx.com

Java: Executors.newFixedThreadPool(4)
来源：http://zfe.yfazqb.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://buc.shanyushiyangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mdo.xuanzx.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lxd.gotoacloud.top

[O03] 加锁保护共享数据
来源：http://bft.xziqi.cn

Py:   with lock: shared += 1
来源：http://sry.fzhhl.top

PHP:  // 用 flock() 做文件锁
来源：http://mvl.tian-w.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qjp.jqgfzy.top

TS:   // 同 JS
来源：http://upq.fanxiaobao.xyz

Java: synchronized (this) { shared++; }
来源：http://nnm.sweek.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tqy.zhoulong.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://tpk.hammf.cn

C#:   lock (gate) { shared++; }
来源：http://uzy.kuanghao11.cn

[O04] 定义异步函数并等待
来源：http://nqe.yj202588.top

Py:   async def f():⏎    await g()
来源：http://meu.zhaomingkeji.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hkm.pycfn.com

JS:   async function f() { await g(); }
来源：http://pjt.fzhhl.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vzu.9152youxi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bdd.ywan-chungtsiang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jgi.fanxiaobao.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://bqy.xylfe.cn

C#:   async Task F() { await G(); }
来源：http://ucu.yj20258888.top

[O05] 并发执行并等待全部完成
来源：http://xjq.0kj1m.cn

Py:   asyncio.gather(*tasks)
来源：http://ftv.sufxvd.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wjs.ehwqpu.com

JS:   await Promise.all(tasks)
来源：http://qsc.sweek.top

TS:   await Promise.all(tasks)
来源：http://vwr.yj20258888.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bus.xinyue.icu

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://koj.vqdsnc.cn

Ruby: threads.map(&:join)
来源：http://reb.birdmap.top

C#:   await Task.WhenAll(t1, t2)
来源：http://wog.nanxuanxn.top

[O06] 使用进程池
来源：http://ytq.ybcxt.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mcx.ppjwa.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dws.shangyingyoupin.top

JS:   // child_process / cluster 模块
来源：http://zus.chenlongwang.top

TS:   // child_process / cluster 模块
来源：http://iqc.yanxiufei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pcq.daria6918.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ezi.sxryk.cn

Ruby: // fork 块
来源：http://flx.ydzc1.top

C#:   Parallel.For
来源：http://dzg.hnqzz.top

================================================================================
来源：http://drk.zhijiandao.cn

P. 常用工具函数
来源：http://dym.cqqwz.cn

================================================================================
来源：http://toq.guowangkeji.top

[P01] 生成 UUID
来源：http://cpz.sufxvd.cn

Py:   str(uuid.uuid4())
来源：http://mfb.shanyushiyangkeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mfh.bbcook.cn

JS:   crypto.randomUUID()
来源：http://epk.nanxuanxn.top

TS:   crypto.randomUUID()
来源：http://pxj.yj20258.top

Java: UUID.randomUUID().toString()
来源：http://ojm.yanxiufei.cn

Go:   // 用 github.com/google/uuid
来源：http://cyk.chenzaomai.com

Ruby: SecureRandom.uuid
来源：http://cog.tian-w.cn

C#:   Guid.NewGuid().ToString()
来源：http://pcu.sweek.top

[P02] MD5 / SHA256 摘要
来源：http://eaz.gotoacloud.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ify.feifeiyinyue.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ezo.zhiwuduotai.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://syl.gotoacloud.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sbx.tarul.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ejc.kuanghao11.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qju.yj202588.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qym.cheryme.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bnv.zhaomingkeji.xyz

[P03] 生成短随机字符串
来源：http://uue.yfazqb.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yzt.meibo888.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ash.fanxiaobao.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ric.guowangkeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zvj.zhiwuduotai.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xyf.svipenyu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zhi.xingfuxueyuan.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://hvq.redwolf501.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ziy.havefunace.top

[P04] 求长度
来源：http://wwv.yj202588.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://giz.hongshengwenyu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jea.hysaishi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bhn.hysaishi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fwh.yfazqb.com

Java: list.size();  map.size();  s.length()
来源：http://ipu.epnwcf.com

Go:   len(arr);  len(m)
来源：http://jmu.xylfe.cn

Ruby: x.length;  x.size
来源：http://aeo.hnxiangtu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xmx.ydjk.org.cn

[P05] 判断两个对象内容是否相等
来源：http://vcn.gzhubu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://iwx.xuanzx.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fej.uphjek.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://owu.vehdjk.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hvq.smart0.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uiw.bjfxy.top

Go:   reflect.DeepEqual(a, b)
来源：http://ize.zycfv.cn

Ruby: a == b
来源：http://xtp.xingfuxueyuan.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ocm.nwbrower.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qkn.xuetiantiany.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dqx.wangshuangyany.cn

PHP:  if (empty($x)) {}
来源：http://vhv.xingfuxueyuan.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vqt.hammf.cn

TS:   if (x == null) {}
来源：http://ljy.kuanghao11.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ymz.316326.xyz

Go:   if x == nil {}
来源：http://zah.zhengqikj.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hpe.yuanzhike.top

C#:   if (x is null) {}
来源：http://pdi.mhx1999.top

[P07] 防抖与节流
来源：http://ccu.yfazqb.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mzc.bbcook.cn

PHP:  // 手写时间戳比较
来源：http://ldq.zhongyouzk.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vka.jlsjyb.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mdg.sweek.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lwl.havefunace.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wws.hammf.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rzp.jqgufenzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ntf.yj20258.top

[P08] 处理浮点精度问题
来源：http://vtb.quarkkingdee.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yds.nwbrower.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qey.xuanzx.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://frd.zhoulong.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://div.guowangkeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bgt.zhijiandao.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ikz.dashuyun.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ywg.havefunace.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://att.shzxlz.cn

================================================================================
来源：http://edf.fehbvm.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fjf.bbcook.cn

================================================================================
来源：http://nrl.sxryk.cn

[Q01] 创建表
来源：http://zzg.smart0.xyz

CREATE TABLE users (
来源：http://vrh.zhixingplan.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ycu.xylfe.cn

name VARCHAR(50) NOT NULL,
来源：http://hyj.jinyuanbaomall.cn

email VARCHAR(100) UNIQUE,
来源：http://aik.tianlin.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ndm.bbcook.cn

);
来源：http://lyh.svipenyu.cn

[Q02] 创建带外键的表
来源：http://ceq.zhixingplan.top

CREATE TABLE orders (
来源：http://igm.wangshuangyany.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ygi.ctjpmb.com

user_id INT NOT NULL,
来源：http://obb.kuanghao11.cn

amount DECIMAL(10, 2),
来源：http://akp.gaohongyu789.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://iwy.shangyingyoupin.top

);
来源：http://fzg.aizwys.cn

[Q03] 增加列
来源：http://wbm.birdmap.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ico.jinqigfzy.top

[Q04] 修改列类型
来源：http://yye.yfazqb.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dxp.wangshuangyany.cn

[Q05] 重命名列
来源：http://wzv.gaohongyu789.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kdy.daria6918.cn

[Q06] 删除列
来源：http://kui.fengsongda.top

ALTER TABLE users DROP COLUMN age;
来源：http://jmq.yueranfly.top

[Q07] 删除表
来源：http://vey.shangyingyoupin.top

DROP TABLE IF EXISTS orders;
来源：http://eex.chenjidiqi.icu

[Q08] 创建普通索引
来源：http://mgg.shangyingyoupin.top

CREATE INDEX idx_users_email ON users(email);
来源：http://nwk.zhengqikj.top

[Q09] 创建唯一索引
来源：http://pgs.xuetiantiany.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gmv.pengpengdd.cyou

[Q10] 插入单行
来源：http://eop.xuanzx.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gfp.hcnkem.com

[Q11] 一次插入多行
来源：http://zau.zhixingplan.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gfs.52xcode.cn

[Q12] 插入后取自增 ID
来源：http://vac.xingfuxueyuan.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://rtu.yj20258.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rsz.hongshengwenyu.top

[Q13] 忽略重复插入
来源：http://vll.quarkkingdee.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ysv.nanxuanxn.top

[Q14] 存在则更新（upsert）
来源：http://enr.vehdjk.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zjz.chenjidiqi.icu

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wwa.yangfankeji.com

[Q15] 查询全部
来源：http://ike.chenjidiqi.icu

SELECT * FROM users;
来源：http://rbo.ehwqpu.com

[Q16] 查询指定列
来源：http://elg.smart0.xyz

SELECT id, name FROM users;
来源：http://yyj.iojbl.cn

[Q17] 条件查询
来源：http://ltr.nanxuanxn.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pcr.dashuyun.cn

[Q18] 模糊匹配
来源：http://iqt.guowangkeji.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cir.andypj.xyz

[Q19] 范围查询
来源：http://acg.jqgufenzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cju.redwolf501.top

[Q20] IN 列表
来源：http://nvi.daria6918.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ynz.shanyushiyangkeji.top

[Q21] 空值判断
来源：http://mzf.yuanzhike.top

SELECT * FROM users WHERE email IS NULL;
来源：http://eqx.yanxiufei.cn

[Q22] 排序
来源：http://fii.jinqigufen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xmk.hnqzz.top

[Q23] 分页
来源：http://hzx.svipenyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cnw.aizwys.cn

[Q24] 去重
来源：http://uul.nwbrower.top

SELECT DISTINCT city FROM users;
来源：http://uca.chenzaomai.com

[Q25] 只取前 N 条
来源：http://wcx.haohaochexian.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://onv.jinyuanbaomall.cn

[Q26] 计数
来源：http://wlr.wangdashe.top

SELECT COUNT(*) FROM users;
来源：http://bxl.jinghuilouyu.cn

[Q27] 条件计数
来源：http://gzq.zhijiandao.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vgu.uphjek.com

[Q28] 求和与平均
来源：http://shn.shuidangran.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://upc.ehwqpu.com

[Q29] 最大最小值
来源：http://rme.yueranfly.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://gua.316326.xyz

[Q30] 分组统计
来源：http://xqz.jianghu66.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hgp.wangshuangyany.cn

[Q31] 分组后过滤
来源：http://nqg.yj20258888.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ljf.yanxiufei.cn

[Q32] 分组拼接字符串
来源：http://vmf.sweek.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qje.tanke756.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xzj.hfpthk.cn

[Q33] 多列分组
来源：http://zvi.fktsv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kgf.ydjk.org.cn

[Q34] 每组取第一条
来源：http://iia.guannengcc.top

SELECT * FROM (
来源：http://grn.zycfv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://drk.daria6918.cn

) t WHERE rn = 1;
来源：http://pqs.cashguo.top

[Q35] 内连接
来源：http://rnl.snrcjt.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yis.ctjpmb.com

[Q36] 左连接
来源：http://lrr.chenjidiqi.icu

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ono.wangshuangyany.cn

[Q37] 右连接
来源：http://heo.jinghuilouyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xpg.wangshuangyany.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wiy.aizwys.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bkz.sjlbkw.cn

[Q39] 自连接（查上下级）
来源：http://xid.hywenlv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qvv.c1oappe.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pea.zdqjudy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ffe.ywan-chungtsiang.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qjg.pengpengdd.cyou

[Q41] 多表连接
来源：http://irh.chenlongwang.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://tbt.ydjk.org.cn

JOIN users u ON u.id = o.user_id
来源：http://xil.chenzaomai.com

JOIN products p ON p.id = o.product_id;
来源：http://who.zhengqikj.top

[Q42] 连接条件附加过滤
来源：http://kyo.ctjpmb.com

SELECT u.name, o.amount FROM users u
来源：http://yyp.shangyingyoupin.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qkw.zdqjudy.top

[Q43] 标量子查询
来源：http://nny.yuxming.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://knr.dianchejie.cn


<!-- 参考信息 -->