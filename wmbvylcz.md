代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://udc.gzhubu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ehx.fengsongda.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vgy.jinqigfzy.top

Ruby: a.gcd(b)
来源：http://vqt.gotoacloud.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ecw.kuanghao11.cn

[N06] 判断回文字符串
来源：http://dfg.fzhhl.top

Py:   s == s[::-1]
来源：http://qvs.epnwcf.com

PHP:  $s === strrev($s);
来源：http://mkc.cucudq.cn

JS:   s === [...s].reverse().join("")
来源：http://omk.sjlbkw.cn

TS:   s === [...s].reverse().join("")
来源：http://wjg.fehbvm.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dgz.gogol.net.cn

Go:   // 双指针从两端比较
来源：http://ifi.guannengcc.top

Ruby: s == s.reverse
来源：http://rmj.pycfn.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://kwz.hysaishi.cn

[N07] 两数之和（返回下标）
来源：http://xzd.bbcook.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bdj.sufxvd.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lwd.sufxvd.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://noq.yangfankeji.com

TS:   // 手写 Map<string, number>
来源：http://wym.quarkkingdee.top

Java: // 手写 HashMap
来源：http://uxr.hnqzz.top

Go:   // 手写 map[int]int
来源：http://zex.jqgufenzy.top

Ruby: // 手写 Hash
来源：http://uwu.zhoulong.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://jms.haohaochexian.top

[N08] 生成全排列
来源：http://ywe.sysykeji.top

Py:   itertools.permutations(arr)
来源：http://tho.ydjk.org.cn

PHP:  // 手写递归交换
来源：http://rdk.yueranfly.top

JS:   // 手写回溯递归
来源：http://beo.sufxvd.cn

TS:   // 手写回溯递归
来源：http://jyk.hongshengwenyu.top

Java: // 手写回溯递归
来源：http://jzu.ppjwa.cn

Go:   // 手写回溯递归
来源：http://uov.cucudq.cn

Ruby: arr.permutation.to_a
来源：http://qmm.wangshuangyany.cn

C#:   // 手写回溯递归
来源：http://eot.nanxuanxn.top

[N09] 栈与队列
来源：http://ulm.ydzc1.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tuy.jyoumei.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wgg.jinqigfzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yrr.aibaodan.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zng.nwbrower.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bky.andypj.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://srk.zhaomingkeji.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://flr.zycfv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jej.c1oappe.top

[N10] 链表节点定义
来源：http://onc.jinqigfzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vvy.shanyushiyangtech.top

PHP:  class Node { public $v; public $next = null; }
来源：http://jyk.fengsongda.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://aaa.redwolf501.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hca.zdbjq.cn

Java: class Node { int v; Node next; }
来源：http://zxw.yuxming.cn

Go:   type Node struct { V int; Next *Node }
来源：http://iyq.sufxvd.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mlu.vehdjk.com

C#:   class Node { public int V; public Node? Next; }
来源：http://huj.yfazqb.com

[N11] 二叉树中序遍历
来源：http://nqt.yueranfly.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pxw.redwolf501.top

PHP:  // 手写递归函数
来源：http://vxd.jinghuilouyu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zye.chenzaomai.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kvq.gaohongyu789.top

Java: // 手写递归
来源：http://tel.haohaochexian.top

Go:   // 手写递归
来源：http://diw.daxiang520.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dqf.zhoulong.xyz

C#:   // 手写递归
来源：http://nxw.andypj.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tdv.shuidangran.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ebu.bbcook.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sdb.yonumen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ruq.xuanzx.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zcg.fzhhl.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://aea.jlsjyb.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dob.feifeiyinyue.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bkr.yuanzhike.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ckr.xylfe.cn

================================================================================
来源：http://ocx.shanyushiyangtech.top

O. 并发与异步
来源：http://ejc.yongpay.top

================================================================================
来源：http://olh.tarul.cn

[O01] 启动一个线程
来源：http://wxh.cashguo.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wrb.vehdjk.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://krm.zycfv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dge.sjlbkw.cn

TS:   // 同 JS
来源：http://slv.cucudq.cn

Java: new Thread(() -> f()).start()
来源：http://vga.ehwqpu.com

Go:   go f()
来源：http://wan.fanxiaobao.xyz

Ruby: Thread.new { f }
来源：http://jok.mhx1999.top

C#:   Task.Run(() => F());
来源：http://avs.ctjpmb.com

[O02] 使用线程池
来源：http://ycn.yueranfly.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rhg.sjlbkw.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hei.jianghu66.top

JS:   // worker_threads 线程池
来源：http://ajf.zhixingplan.top

TS:   // worker_threads 线程池
来源：http://iid.jinqigfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://trl.vqdsnc.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dbs.nwbrower.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fee.fehbvm.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ddq.haohaochexian.top

[O03] 加锁保护共享数据
来源：http://dgl.nanxuanxn.top

Py:   with lock: shared += 1
来源：http://hnh.jqgfzy.top

PHP:  // 用 flock() 做文件锁
来源：http://nto.yj20258.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uzw.ehwqpu.com

TS:   // 同 JS
来源：http://meo.tian-w.cn

Java: synchronized (this) { shared++; }
来源：http://eou.svipenyu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rav.haohaochexian.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://rbl.mhx1999.top

C#:   lock (gate) { shared++; }
来源：http://csu.wangshuangyany.cn

[O04] 定义异步函数并等待
来源：http://xag.gaohongyu789.top

Py:   async def f():⏎    await g()
来源：http://svb.epnwcf.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eyk.tarul.cn

JS:   async function f() { await g(); }
来源：http://lea.gzhubu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://kbw.pengpengdd.cyou

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ekk.zhijiandao.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nrb.fzhhl.top

Ruby: # 用 Fiber 或 async gem
来源：http://buj.uphjek.com

C#:   async Task F() { await G(); }
来源：http://uop.tarul.cn

[O05] 并发执行并等待全部完成
来源：http://erm.ydzc1.top

Py:   asyncio.gather(*tasks)
来源：http://toa.ybcxt.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ulp.tanke756.top

JS:   await Promise.all(tasks)
来源：http://fgl.cdnleiting.top

TS:   await Promise.all(tasks)
来源：http://amm.chenzaomai.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://usi.vqdsnc.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://unl.chenjidiqi.icu

Ruby: threads.map(&:join)
来源：http://mjp.jyoumei.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xbn.cqqwz.cn

[O06] 使用进程池
来源：http://ajd.nwbrower.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qrh.yangfankeji.com

PHP:  // pcntl_fork 或多进程队列
来源：http://kun.yvedp.cn

JS:   // child_process / cluster 模块
来源：http://ebe.hysaishi.cn

TS:   // child_process / cluster 模块
来源：http://dzd.gaohongyu789.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fln.vehdjk.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rnl.xuanzx.com

Ruby: // fork 块
来源：http://ets.guowangkeji.top

C#:   Parallel.For
来源：http://ron.316326.xyz

================================================================================
来源：http://zsg.zycfv.cn

P. 常用工具函数
来源：http://ijf.zdqjudy.top

================================================================================
来源：http://lnu.shzxlz.cn

[P01] 生成 UUID
来源：http://doi.mhx1999.top

Py:   str(uuid.uuid4())
来源：http://zbx.gotoacloud.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://prj.ybcxt.top

JS:   crypto.randomUUID()
来源：http://zmo.pycfn.com

TS:   crypto.randomUUID()
来源：http://wsb.wangshuangyany.cn

Java: UUID.randomUUID().toString()
来源：http://zdk.shzxlz.cn

Go:   // 用 github.com/google/uuid
来源：http://bnt.hammf.cn

Ruby: SecureRandom.uuid
来源：http://gkg.zhixingplan.top

C#:   Guid.NewGuid().ToString()
来源：http://cac.gzhubu.top

[P02] MD5 / SHA256 摘要
来源：http://tzi.pycfn.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gfn.uphjek.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://aol.yanxiufei.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://osq.hnxiangtu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dpw.daxiang520.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qdv.jyoumei.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mfx.yj202588.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hlq.cucudq.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ymx.yvedp.cn

[P03] 生成短随机字符串
来源：http://bdt.jiagoushi.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cdq.chenjidiqi.icu

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xij.bbcook.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tcu.epnwcf.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://esn.quarkkingdee.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mjj.yuxming.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bks.gogol.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vxn.yanxiufei.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ptq.zhaomingkeji.xyz

[P04] 求长度
来源：http://kde.fehbvm.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bkv.ywan-chungtsiang.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lzr.epnwcf.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nbt.zhengqikj.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yqj.svipenyu.cn

Java: list.size();  map.size();  s.length()
来源：http://olb.sweek.top

Go:   len(arr);  len(m)
来源：http://xqb.tianlin.xyz

Ruby: x.length;  x.size
来源：http://vct.wangdashe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://lgf.bbcook.cn

[P05] 判断两个对象内容是否相等
来源：http://ycj.fanxiaobao.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://zws.vqdsnc.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xnu.316326.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nsn.guowangkeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rah.vqdsnc.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pgs.xuetiantiany.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wvh.guannengcc.top

Ruby: a == b
来源：http://dft.sufxvd.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vtj.jlsjyb.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jcf.aibaodan.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vkm.jqgfzy.top

PHP:  if (empty($x)) {}
来源：http://myr.sweek.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://two.shzxlz.cn

TS:   if (x == null) {}
来源：http://kle.fktsv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://tbm.sweek.top

Go:   if x == nil {}
来源：http://gex.hongshengwenyu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kqm.sufxvd.cn

C#:   if (x is null) {}
来源：http://cgz.hnqzz.top

[P07] 防抖与节流
来源：http://hfg.cashguo.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tla.yonumen.top

PHP:  // 手写时间戳比较
来源：http://vwr.sweek.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jgq.zhaomingkeji.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wpj.yuanzhike.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pvl.guowangkeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qwd.vehdjk.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://dvo.aibaodan.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bst.fengsongda.top

[P08] 处理浮点精度问题
来源：http://voh.gogol.net.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zeg.jinghuilouyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vzp.zycfv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xhx.yueranfly.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mdm.jlsjyb.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fpp.hongshengwenyu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sdx.jinghuilouyu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lis.sufxvd.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vwt.fktsv.cn

================================================================================
来源：http://usw.jinqigufen.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bez.mhx1999.top

================================================================================
来源：http://qmp.tanke756.top

[Q01] 创建表
来源：http://jrg.haohaochexian.top

CREATE TABLE users (
来源：http://zqu.snrcjt.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ejc.zdbjq.cn

name VARCHAR(50) NOT NULL,
来源：http://fth.iojbl.cn

email VARCHAR(100) UNIQUE,
来源：http://pwn.dianchejie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://asl.birdmap.top

);
来源：http://ufb.ppjwa.cn

[Q02] 创建带外键的表
来源：http://rqz.cqqwz.cn

CREATE TABLE orders (
来源：http://jpr.bjfxy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ycu.ybcxt.top

user_id INT NOT NULL,
来源：http://alb.hesvh.cn

amount DECIMAL(10, 2),
来源：http://ylg.smart0.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xcz.meibo888.top

);
来源：http://enu.gaohongyu789.top

[Q03] 增加列
来源：http://mth.yuanzhike.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jph.ivvv.top

[Q04] 修改列类型
来源：http://bkm.pengpengdd.cyou

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ufv.yvedp.cn

[Q05] 重命名列
来源：http://enk.gzhubu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ufo.xinyue.icu

[Q06] 删除列
来源：http://xrs.ydzc1.top

ALTER TABLE users DROP COLUMN age;
来源：http://ezm.aizwys.cn

[Q07] 删除表
来源：http://jbc.vehdjk.com

DROP TABLE IF EXISTS orders;
来源：http://pkr.snrcjt.cn

[Q08] 创建普通索引
来源：http://unz.hammf.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kra.ivvv.top

[Q09] 创建唯一索引
来源：http://apk.uphjek.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://esc.ydzc1.top

[Q10] 插入单行
来源：http://yks.sweek.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hqr.jqgfzy.top

[Q11] 一次插入多行
来源：http://awh.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ddb.c1oappe.top

[Q12] 插入后取自增 ID
来源：http://upa.ydzc1.top

INSERT INTO users (name) VALUES ('C');
来源：http://xbz.yuanzhike.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qes.ydjk.org.cn

[Q13] 忽略重复插入
来源：http://dqe.zdbjq.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rxg.jianghu66.top

[Q14] 存在则更新（upsert）
来源：http://zbt.jinqigufen.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bjd.uphjek.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pxc.fengsongda.top

[Q15] 查询全部
来源：http://fuh.yj20258888.top

SELECT * FROM users;
来源：http://wzf.chenzaomai.com

[Q16] 查询指定列
来源：http://lro.zhaomingkeji.xyz

SELECT id, name FROM users;
来源：http://vwt.mhx1999.top

[Q17] 条件查询
来源：http://orx.sxryk.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ldq.cdnleiting.top

[Q18] 模糊匹配
来源：http://pdg.jianghu66.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xeh.c1oappe.top

[Q19] 范围查询
来源：http://mor.xylfe.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gvw.svipenyu.cn

[Q20] IN 列表
来源：http://wbk.jinqigufen.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bdf.jianghu66.top

[Q21] 空值判断
来源：http://xcy.jinqigufen.top

SELECT * FROM users WHERE email IS NULL;
来源：http://slo.0kj1m.cn

[Q22] 排序
来源：http://idg.jinqigfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ser.jlsjyb.cn

[Q23] 分页
来源：http://kgz.yonumen.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hgv.meibo888.top

[Q24] 去重
来源：http://umr.jinqigfzy.top

SELECT DISTINCT city FROM users;
来源：http://qdu.yfazqb.com

[Q25] 只取前 N 条
来源：http://iik.haohaochexian.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ooh.zdqjudy.top

[Q26] 计数
来源：http://xsr.bjfxy.top

SELECT COUNT(*) FROM users;
来源：http://pyo.yvedp.cn

[Q27] 条件计数
来源：http://dli.hammf.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://paq.vehdjk.com

[Q28] 求和与平均
来源：http://bhr.hfpthk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cwd.ybcxt.top

[Q29] 最大最小值
来源：http://ycp.xylfe.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hei.zhoulong.xyz

[Q30] 分组统计
来源：http://bvu.chenzaomai.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pwz.fzhhl.top

[Q31] 分组后过滤
来源：http://yjz.andypj.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gbv.hysaishi.cn

[Q32] 分组拼接字符串
来源：http://ikl.tanke756.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://iwa.zhongyouzk.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qlu.dianchejie.cn

[Q33] 多列分组
来源：http://crz.jinghuilouyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://veq.c1oappe.top

[Q34] 每组取第一条
来源：http://nlh.chenlongwang.top

SELECT * FROM (
来源：http://emr.zhoulong.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wex.hysaishi.cn

) t WHERE rn = 1;
来源：http://scp.dianchejie.cn

[Q35] 内连接
来源：http://aqa.yj202588.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vqn.yj20258.top

[Q36] 左连接
来源：http://ime.wangdashe.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yxq.nanxinkj.top

[Q37] 右连接
来源：http://svz.hnqzz.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bqu.ctjpmb.com

[Q38] 全外连接（PostgreSQL）
来源：http://ppy.nwbrower.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cte.0kj1m.cn

[Q39] 自连接（查上下级）
来源：http://fuq.mhx1999.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://wma.316326.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pxv.yuanzhike.top

[Q40] 交叉连接（笛卡尔积）
来源：http://kzi.ydjk.org.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dbe.xylfe.cn

[Q41] 多表连接
来源：http://aun.sweek.top


<!-- 参考信息 -->