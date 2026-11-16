代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zkp.zdbjq.cn

[N06] 判断回文字符串
来源：http://aon.jqgufenzy.top

Py:   s == s[::-1]
来源：http://oko.zhongyouzk.top

PHP:  $s === strrev($s);
来源：http://hly.jinqigfzy.top

JS:   s === [...s].reverse().join("")
来源：http://tlh.ydjk.org.cn

TS:   s === [...s].reverse().join("")
来源：http://taq.ydzc1.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://doc.yanxiufei.cn

Go:   // 双指针从两端比较
来源：http://key.yuxming.cn

Ruby: s == s.reverse
来源：http://xyf.yuanzhike.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wdy.kuanghao11.cn

[N07] 两数之和（返回下标）
来源：http://ouk.jqgufenzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ice.ybcxt.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ilw.yvedp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ldn.chenjidiqi.icu

TS:   // 手写 Map<string, number>
来源：http://dbk.jyoumei.cn

Java: // 手写 HashMap
来源：http://eyr.zhijiandao.cn

Go:   // 手写 map[int]int
来源：http://gyj.hysaishi.cn

Ruby: // 手写 Hash
来源：http://oar.dianchejie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vso.ywan-chungtsiang.top

[N08] 生成全排列
来源：http://xub.andypj.xyz

Py:   itertools.permutations(arr)
来源：http://baj.wangdashe.top

PHP:  // 手写递归交换
来源：http://eeg.ydzc1.top

JS:   // 手写回溯递归
来源：http://uwr.haohaochexian.top

TS:   // 手写回溯递归
来源：http://kzc.yj202588.top

Java: // 手写回溯递归
来源：http://hpz.tian-w.cn

Go:   // 手写回溯递归
来源：http://miu.redwolf501.top

Ruby: arr.permutation.to_a
来源：http://dgw.bjfxy.top

C#:   // 手写回溯递归
来源：http://lce.yj20258888.top

[N09] 栈与队列
来源：http://udw.snrcjt.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gpo.quarkkingdee.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wvf.zhaomingkeji.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fex.jinyuanbaomall.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jwt.wangdashe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wtn.shanyushiyangkeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zal.tianlin.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://eje.jinqigfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fjy.shuidangran.top

[N10] 链表节点定义
来源：http://ehh.ydzc1.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jyu.shzxlz.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qqv.bjfxy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://iau.havefunace.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wxg.xuanzx.com

Java: class Node { int v; Node next; }
来源：http://wub.yj20258888.top

Go:   type Node struct { V int; Next *Node }
来源：http://kso.9152youxi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hzi.shanyushiyangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://aud.daxiang520.top

[N11] 二叉树中序遍历
来源：http://twc.zdbjq.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rpv.tianlin.xyz

PHP:  // 手写递归函数
来源：http://wtq.gaohongyu789.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yby.shzxlz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iao.haohaochexian.top

Java: // 手写递归
来源：http://rvr.zhongyouzk.top

Go:   // 手写递归
来源：http://fch.jinghuilouyu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pib.shangyingyoupin.top

C#:   // 手写递归
来源：http://upt.jqgfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://eyw.dashuyun.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jwx.yj202588.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fgt.chenjidiqi.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lmj.hfpthk.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aeo.pycfn.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kxp.jiagoushi.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qxv.fanxiaobao.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cja.zhijiandao.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ogj.hywenlv.cn

================================================================================
来源：http://jpc.yvedp.cn

O. 并发与异步
来源：http://hhm.shzxlz.cn

================================================================================
来源：http://zee.tarul.cn

[O01] 启动一个线程
来源：http://plk.zhoulong.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://khi.xylfe.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tob.xziqi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xze.xuanzx.com

TS:   // 同 JS
来源：http://jru.hesvh.cn

Java: new Thread(() -> f()).start()
来源：http://zxc.yj20258888.top

Go:   go f()
来源：http://mgo.ivvv.top

Ruby: Thread.new { f }
来源：http://gyu.xziqi.cn

C#:   Task.Run(() => F());
来源：http://vtr.zhoulong.xyz

[O02] 使用线程池
来源：http://tvd.hammf.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mud.uphjek.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vxi.gzhubu.top

JS:   // worker_threads 线程池
来源：http://lcr.wangdashe.top

TS:   // worker_threads 线程池
来源：http://lso.zycfv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bna.guannengcc.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ljr.hongshengwenyu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zpp.zycfv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://eaj.aizwys.cn

[O03] 加锁保护共享数据
来源：http://mdj.yj20258.top

Py:   with lock: shared += 1
来源：http://nyb.hnqzz.top

PHP:  // 用 flock() 做文件锁
来源：http://ojj.xylfe.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rxv.yonumen.top

TS:   // 同 JS
来源：http://cwy.zhixingplan.top

Java: synchronized (this) { shared++; }
来源：http://lfc.pengpengdd.cyou

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wxs.jianghu66.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://kvm.epnwcf.com

C#:   lock (gate) { shared++; }
来源：http://dtc.andypj.xyz

[O04] 定义异步函数并等待
来源：http://scf.daxiang520.top

Py:   async def f():⏎    await g()
来源：http://qxx.uphjek.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zgq.guannengcc.top

JS:   async function f() { await g(); }
来源：http://bpz.vehdjk.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://zzr.ywan-chungtsiang.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hna.sweek.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://iog.feifeiyinyue.top

Ruby: # 用 Fiber 或 async gem
来源：http://pzs.ctjpmb.com

C#:   async Task F() { await G(); }
来源：http://dda.shuidangran.top

[O05] 并发执行并等待全部完成
来源：http://aap.9152youxi.cn

Py:   asyncio.gather(*tasks)
来源：http://eto.guannengcc.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://opn.zdqjudy.top

JS:   await Promise.all(tasks)
来源：http://edq.yongpay.top

TS:   await Promise.all(tasks)
来源：http://mpw.fengsongda.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bdc.jianghu66.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zlg.c1oappe.top

Ruby: threads.map(&:join)
来源：http://hmo.316326.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://rut.jyoumei.cn

[O06] 使用进程池
来源：http://jff.vehdjk.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vdb.bjfxy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://rxp.redwolf501.top

JS:   // child_process / cluster 模块
来源：http://phu.hywenlv.cn

TS:   // child_process / cluster 模块
来源：http://sdk.havefunace.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vwj.yj20258.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wmk.andypj.xyz

Ruby: // fork 块
来源：http://jia.fanxiaobao.xyz

C#:   Parallel.For
来源：http://zuq.shzxlz.cn

================================================================================
来源：http://uvm.zdbjq.cn

P. 常用工具函数
来源：http://poj.hesvh.cn

================================================================================
来源：http://qrq.fanxiaobao.xyz

[P01] 生成 UUID
来源：http://kgq.svipenyu.cn

Py:   str(uuid.uuid4())
来源：http://nxg.bbcook.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kwc.jianghu66.top

JS:   crypto.randomUUID()
来源：http://wjo.yanxiufei.cn

TS:   crypto.randomUUID()
来源：http://xsd.hcnkem.com

Java: UUID.randomUUID().toString()
来源：http://tcp.shangyingyoupin.top

Go:   // 用 github.com/google/uuid
来源：http://fac.gotoacloud.top

Ruby: SecureRandom.uuid
来源：http://edb.vehdjk.com

C#:   Guid.NewGuid().ToString()
来源：http://ygc.haohaochexian.top

[P02] MD5 / SHA256 摘要
来源：http://ypr.chenzaomai.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zep.yj20258.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://xfs.smart0.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vyz.cqqwz.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zoz.redwolf501.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dpq.fehbvm.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oba.cheryme.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tjm.vqdsnc.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hhn.kuanghao11.cn

[P03] 生成短随机字符串
来源：http://uqk.zhiwuduotai.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ybz.mhx1999.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://asw.ywan-chungtsiang.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ght.ctjpmb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://svd.zhoulong.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zfw.chenlongwang.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ygy.nanxuanxn.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ycr.fzhhl.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qje.tanke756.top

[P04] 求长度
来源：http://amn.yuanzhike.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dhk.jinyuanbaomall.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qis.sxryk.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jwr.xuetiantiany.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://doz.gzhubu.top

Java: list.size();  map.size();  s.length()
来源：http://kjw.ydjk.org.cn

Go:   len(arr);  len(m)
来源：http://rma.shzxlz.cn

Ruby: x.length;  x.size
来源：http://aqk.daxiang520.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://laf.xuetiantiany.cn

[P05] 判断两个对象内容是否相等
来源：http://kdc.pengpengdd.cyou

Py:   a == b              # 列表与字典递归比较内容
来源：http://fbo.snrcjt.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://etm.epnwcf.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xea.fanxiaobao.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hoi.xziqi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hsq.yuxming.cn

Go:   reflect.DeepEqual(a, b)
来源：http://peo.xziqi.cn

Ruby: a == b
来源：http://qhz.yueranfly.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wui.yfazqb.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uvj.yuanzhike.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kwq.gotoacloud.top

PHP:  if (empty($x)) {}
来源：http://igd.xylfe.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://efl.yj20258888.top

TS:   if (x == null) {}
来源：http://ymo.gzhubu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://vvk.epnwcf.com

Go:   if x == nil {}
来源：http://eyk.yj20258888.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ukv.feifeiyinyue.top

C#:   if (x is null) {}
来源：http://dfx.vehdjk.com

[P07] 防抖与节流
来源：http://izh.tarul.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cab.ybcxt.top

PHP:  // 手写时间戳比较
来源：http://off.tianlin.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rrh.nanxuanxn.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yjc.dianchejie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rsu.sweek.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yai.iojbl.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lvo.pycfn.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ukv.hfpthk.cn

[P08] 处理浮点精度问题
来源：http://daq.yueranfly.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dwn.shuidangran.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://anm.sjlbkw.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sqv.yj20258888.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hwd.hnqzz.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kgg.nwbrower.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bka.meibo888.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://squ.meibo888.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vac.cucudq.cn

================================================================================
来源：http://dtt.andypj.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dxg.hywenlv.cn

================================================================================
来源：http://gxj.zhixingplan.top

[Q01] 创建表
来源：http://wbo.yj20258888.top

CREATE TABLE users (
来源：http://ryj.yonumen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nll.ybcxt.top

name VARCHAR(50) NOT NULL,
来源：http://lvn.hywenlv.cn

email VARCHAR(100) UNIQUE,
来源：http://aau.zhoulong.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hpi.zycfv.cn

);
来源：http://hlb.kuanghao11.cn

[Q02] 创建带外键的表
来源：http://dyc.cheryme.top

CREATE TABLE orders (
来源：http://zkh.svipenyu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cwr.tian-w.cn

user_id INT NOT NULL,
来源：http://upt.yuxming.cn

amount DECIMAL(10, 2),
来源：http://mrs.yj20258888.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://poy.vehdjk.com

);
来源：http://fnn.bjfxy.top

[Q03] 增加列
来源：http://lne.chenlongwang.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://igp.gaohongyu789.top

[Q04] 修改列类型
来源：http://upy.xuanzx.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wlg.vehdjk.com

[Q05] 重命名列
来源：http://leg.jinghuilouyu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dqo.tianlin.xyz

[Q06] 删除列
来源：http://fna.chenlongwang.top

ALTER TABLE users DROP COLUMN age;
来源：http://pzg.wangshuangyany.cn

[Q07] 删除表
来源：http://zle.xinyue.icu

DROP TABLE IF EXISTS orders;
来源：http://oqf.shangyingyoupin.top

[Q08] 创建普通索引
来源：http://omi.xingfuxueyuan.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://tdu.ppjwa.cn

[Q09] 创建唯一索引
来源：http://hpj.hammf.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://grn.jinyuanbaomall.cn

[Q10] 插入单行
来源：http://are.jlsjyb.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mpi.yonumen.top

[Q11] 一次插入多行
来源：http://wtf.smart0.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cur.gogol.net.cn

[Q12] 插入后取自增 ID
来源：http://wxl.birdmap.top

INSERT INTO users (name) VALUES ('C');
来源：http://esv.daxiang520.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kun.ydjk.org.cn

[Q13] 忽略重复插入
来源：http://ttg.yongpay.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gjk.gzhubu.top

[Q14] 存在则更新（upsert）
来源：http://qlr.gogol.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://iui.aizwys.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ctu.guannengcc.top

[Q15] 查询全部
来源：http://dpm.shzxlz.cn

SELECT * FROM users;
来源：http://njw.nanxuanxn.top

[Q16] 查询指定列
来源：http://una.meibo888.top

SELECT id, name FROM users;
来源：http://rqh.sxryk.cn

[Q17] 条件查询
来源：http://qtk.haohaochexian.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ccy.fengsongda.top

[Q18] 模糊匹配
来源：http://lrr.yj20258.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zpq.nwbrower.top

[Q19] 范围查询
来源：http://neu.cheryme.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kbq.hywenlv.cn

[Q20] IN 列表
来源：http://bzn.mhx1999.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lse.sysykeji.top

[Q21] 空值判断
来源：http://ury.shuidangran.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ifc.jianghu66.top

[Q22] 排序
来源：http://jar.fktsv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hwb.birdmap.top

[Q23] 分页
来源：http://zbk.shangyingyoupin.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nfh.cqqwz.cn

[Q24] 去重
来源：http://huo.ehwqpu.com

SELECT DISTINCT city FROM users;
来源：http://tme.xuetiantiany.cn

[Q25] 只取前 N 条
来源：http://fme.daxiang520.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hip.shzxlz.cn

[Q26] 计数
来源：http://wpc.shangyingyoupin.top

SELECT COUNT(*) FROM users;
来源：http://itt.316326.xyz

[Q27] 条件计数
来源：http://xvr.nanxuanxn.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mck.quarkkingdee.top

[Q28] 求和与平均
来源：http://inz.zhixingplan.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rja.fktsv.cn

[Q29] 最大最小值
来源：http://mal.jiagoushi.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://cvr.birdmap.top

[Q30] 分组统计
来源：http://aqw.meibo888.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lgh.daxiang520.top

[Q31] 分组后过滤
来源：http://han.uphjek.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mlo.shanyushiyangtech.top

[Q32] 分组拼接字符串
来源：http://pmc.jiagoushi.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bas.zhixingplan.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vrn.c1oappe.top

[Q33] 多列分组
来源：http://fyy.yueranfly.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://chx.hammf.cn

[Q34] 每组取第一条
来源：http://tag.52xcode.cn

SELECT * FROM (
来源：http://rej.shzxlz.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lon.hammf.cn

) t WHERE rn = 1;
来源：http://czw.sxryk.cn

[Q35] 内连接
来源：http://hkf.xylfe.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gjo.ywan-chungtsiang.top

[Q36] 左连接
来源：http://fxp.jinqigfzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ryy.jinghuilouyu.cn

[Q37] 右连接
来源：http://sew.xuanzx.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://quu.xuanzx.com

[Q38] 全外连接（PostgreSQL）
来源：http://kvc.fzhhl.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uns.yuxming.cn

[Q39] 自连接（查上下级）
来源：http://pic.dashuyun.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kep.vqdsnc.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mfd.cdnleiting.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ejm.yfazqb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://aza.52xcode.cn

[Q41] 多表连接
来源：http://wdt.mhx1999.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://hdi.cashguo.top

JOIN users u ON u.id = o.user_id
来源：http://ugz.chenlongwang.top

JOIN products p ON p.id = o.product_id;
来源：http://xvm.nanxinkj.top

[Q42] 连接条件附加过滤
来源：http://nne.zhiwuduotai.top


<!-- 参考信息 -->