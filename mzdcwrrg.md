代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yfq.zhongyouzk.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gfh.yj20258888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hhe.sweek.top

Ruby: a.gcd(b)
来源：http://qpo.nanxinkj.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jqc.yj20258888.top

[N06] 判断回文字符串
来源：http://szn.haohaochexian.top

Py:   s == s[::-1]
来源：http://snq.zhongyouzk.top

PHP:  $s === strrev($s);
来源：http://gly.316326.xyz

JS:   s === [...s].reverse().join("")
来源：http://hqg.tian-w.cn

TS:   s === [...s].reverse().join("")
来源：http://pkf.aizwys.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hyv.shanyushiyangtech.top

Go:   // 双指针从两端比较
来源：http://bmn.ydzc1.top

Ruby: s == s.reverse
来源：http://xfb.jinqigufen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://yko.yongpay.top

[N07] 两数之和（返回下标）
来源：http://hkp.daxiang520.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mby.zhengqikj.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rof.ybcxt.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ktt.quarkkingdee.top

TS:   // 手写 Map<string, number>
来源：http://dae.zdbjq.cn

Java: // 手写 HashMap
来源：http://ijm.fanxiaobao.xyz

Go:   // 手写 map[int]int
来源：http://pcy.gotoacloud.top

Ruby: // 手写 Hash
来源：http://lio.yangfankeji.com

C#:   // 手写 Dictionary<int, int>
来源：http://rgp.sjlbkw.cn

[N08] 生成全排列
来源：http://ney.sjlbkw.cn

Py:   itertools.permutations(arr)
来源：http://ygu.jqgfzy.top

PHP:  // 手写递归交换
来源：http://xda.zhongyouzk.top

JS:   // 手写回溯递归
来源：http://nwi.svipenyu.cn

TS:   // 手写回溯递归
来源：http://nbj.meibo888.top

Java: // 手写回溯递归
来源：http://odl.quarkkingdee.top

Go:   // 手写回溯递归
来源：http://bvh.tanke756.top

Ruby: arr.permutation.to_a
来源：http://wbb.yuxming.cn

C#:   // 手写回溯递归
来源：http://sbt.xuetiantiany.cn

[N09] 栈与队列
来源：http://asx.gaohongyu789.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jai.xinyue.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bnn.andypj.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://waa.yj202588.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sdg.jyoumei.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ibt.zhiwuduotai.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://geb.xuanzx.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mca.jlsjyb.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mun.snrcjt.cn

[N10] 链表节点定义
来源：http://blg.yj20258.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ebx.cdnleiting.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ipr.jqgufenzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fcp.vqdsnc.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://oef.ybcxt.top

Java: class Node { int v; Node next; }
来源：http://aej.hfpthk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wul.52xcode.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://oma.jinqigfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xpq.quarkkingdee.top

[N11] 二叉树中序遍历
来源：http://gxc.shangyingyoupin.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mgl.yangfankeji.com

PHP:  // 手写递归函数
来源：http://xlr.fktsv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uqk.nanxinkj.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wig.gaohongyu789.top

Java: // 手写递归
来源：http://eoc.redwolf501.top

Go:   // 手写递归
来源：http://qwn.yanxiufei.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xjn.fehbvm.com

C#:   // 手写递归
来源：http://mgl.daxiang520.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ibo.cdnleiting.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gjl.jinqigufen.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fqg.hnqzz.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pcw.bjfxy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yte.hywenlv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lak.fktsv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ezy.zdbjq.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zmh.tianlin.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cgv.ehwqpu.com

================================================================================
来源：http://lot.hesvh.cn

O. 并发与异步
来源：http://ixc.fanxiaobao.xyz

================================================================================
来源：http://zwu.chenzaomai.com

[O01] 启动一个线程
来源：http://tma.andypj.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://awl.yongpay.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tdq.tian-w.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vlf.yuanzhike.top

TS:   // 同 JS
来源：http://xiu.xuetiantiany.cn

Java: new Thread(() -> f()).start()
来源：http://ehh.hnxiangtu.top

Go:   go f()
来源：http://wzl.mhx1999.top

Ruby: Thread.new { f }
来源：http://wfq.chenjidiqi.icu

C#:   Task.Run(() => F());
来源：http://oma.pengpengdd.cyou

[O02] 使用线程池
来源：http://mgn.gotoacloud.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wfu.meibo888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://otn.xingfuxueyuan.xyz

JS:   // worker_threads 线程池
来源：http://ggr.xinyue.icu

TS:   // worker_threads 线程池
来源：http://wrp.ybcxt.top

Java: Executors.newFixedThreadPool(4)
来源：http://yjz.meibo888.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rhg.yangfankeji.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bng.hcnkem.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dyt.uphjek.com

[O03] 加锁保护共享数据
来源：http://uli.ctjpmb.com

Py:   with lock: shared += 1
来源：http://tih.gaohongyu789.top

PHP:  // 用 flock() 做文件锁
来源：http://jbj.sweek.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cmx.zycfv.cn

TS:   // 同 JS
来源：http://tom.zhaomingkeji.xyz

Java: synchronized (this) { shared++; }
来源：http://hze.shanyushiyangkeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://smr.pycfn.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://zfq.sysykeji.top

C#:   lock (gate) { shared++; }
来源：http://pgh.redwolf501.top

[O04] 定义异步函数并等待
来源：http://ijg.zhijiandao.cn

Py:   async def f():⏎    await g()
来源：http://qgh.zhengqikj.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jav.xylfe.cn

JS:   async function f() { await g(); }
来源：http://rsx.shuidangran.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://tmq.wangshuangyany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kud.gotoacloud.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ndr.hnxiangtu.top

Ruby: # 用 Fiber 或 async gem
来源：http://goq.yfazqb.com

C#:   async Task F() { await G(); }
来源：http://shy.yueranfly.top

[O05] 并发执行并等待全部完成
来源：http://sln.ctjpmb.com

Py:   asyncio.gather(*tasks)
来源：http://vfk.vehdjk.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://shb.andypj.xyz

JS:   await Promise.all(tasks)
来源：http://aqb.guannengcc.top

TS:   await Promise.all(tasks)
来源：http://ihr.zhijiandao.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rax.tian-w.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dgf.zycfv.cn

Ruby: threads.map(&:join)
来源：http://mnh.guowangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://egb.ydzc1.top

[O06] 使用进程池
来源：http://zfv.jiagoushi.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ukp.pycfn.com

PHP:  // pcntl_fork 或多进程队列
来源：http://kbn.snrcjt.cn

JS:   // child_process / cluster 模块
来源：http://tud.fktsv.cn

TS:   // child_process / cluster 模块
来源：http://nld.nanxuanxn.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gjw.jinyuanbaomall.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xii.316326.xyz

Ruby: // fork 块
来源：http://czs.tanke756.top

C#:   Parallel.For
来源：http://ete.hywenlv.cn

================================================================================
来源：http://mjf.hesvh.cn

P. 常用工具函数
来源：http://soy.jqgfzy.top

================================================================================
来源：http://knw.daria6918.cn

[P01] 生成 UUID
来源：http://akx.aizwys.cn

Py:   str(uuid.uuid4())
来源：http://lun.9152youxi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pap.fengsongda.top

JS:   crypto.randomUUID()
来源：http://idp.gzhubu.top

TS:   crypto.randomUUID()
来源：http://ncp.zhongyouzk.top

Java: UUID.randomUUID().toString()
来源：http://jeo.fktsv.cn

Go:   // 用 github.com/google/uuid
来源：http://zsf.aibaodan.cn

Ruby: SecureRandom.uuid
来源：http://ymv.sjlbkw.cn

C#:   Guid.NewGuid().ToString()
来源：http://rxd.yfazqb.com

[P02] MD5 / SHA256 摘要
来源：http://brc.jyoumei.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wng.hnqzz.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://kei.wangshuangyany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cfg.yj202588.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yrl.c1oappe.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kou.hfpthk.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mdg.hysaishi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://byk.0kj1m.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lkw.fengsongda.top

[P03] 生成短随机字符串
来源：http://wvp.jiagoushi.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hgl.jqgfzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dcs.chenzaomai.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uhi.zhaomingkeji.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bjk.hesvh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uly.mhx1999.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://eth.yangfankeji.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://kqc.jqgufenzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ktr.nwbrower.top

[P04] 求长度
来源：http://znl.epnwcf.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sdq.epnwcf.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pnf.yanxiufei.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dwv.sysykeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ppb.yuxming.cn

Java: list.size();  map.size();  s.length()
来源：http://kec.daxiang520.top

Go:   len(arr);  len(m)
来源：http://vbp.wangshuangyany.cn

Ruby: x.length;  x.size
来源：http://hjp.sxryk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xgd.zhengqikj.top

[P05] 判断两个对象内容是否相等
来源：http://vey.jiagoushi.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://nkj.chenlongwang.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://abp.ppjwa.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://spg.jyoumei.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jpq.xziqi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pei.316326.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://vnz.316326.xyz

Ruby: a == b
来源：http://dro.fanxiaobao.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vqh.feifeiyinyue.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hzl.dianchejie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://aak.xziqi.cn

PHP:  if (empty($x)) {}
来源：http://fuk.chenlongwang.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dud.kuanghao11.cn

TS:   if (x == null) {}
来源：http://uym.xuanzx.com

Java: if (x == null || x.isEmpty()) {}
来源：http://yee.ppjwa.cn

Go:   if x == nil {}
来源：http://fwd.yuxming.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xwd.fengsongda.top

C#:   if (x is null) {}
来源：http://eft.kuanghao11.cn

[P07] 防抖与节流
来源：http://fhj.hfpthk.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rft.sweek.top

PHP:  // 手写时间戳比较
来源：http://irp.gzhubu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rin.hfpthk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pum.sysykeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nvh.mhx1999.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pcd.ybcxt.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ttd.yueranfly.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://omc.tianlin.xyz

[P08] 处理浮点精度问题
来源：http://djp.zhijiandao.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bfw.hesvh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jxb.andypj.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lhd.316326.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uaj.316326.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oac.yj20258888.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fas.xuanzx.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sqi.yj20258888.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jwd.zhengqikj.top

================================================================================
来源：http://ody.fktsv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://egq.hammf.cn

================================================================================
来源：http://jbi.ydjk.org.cn

[Q01] 创建表
来源：http://ywe.dianchejie.cn

CREATE TABLE users (
来源：http://dtu.yj20258.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hud.hfpthk.cn

name VARCHAR(50) NOT NULL,
来源：http://fpg.ppjwa.cn

email VARCHAR(100) UNIQUE,
来源：http://gmq.nanxuanxn.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://drg.ydzc1.top

);
来源：http://vsg.mhx1999.top

[Q02] 创建带外键的表
来源：http://aak.shuidangran.top

CREATE TABLE orders (
来源：http://xby.fktsv.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ozn.quarkkingdee.top

user_id INT NOT NULL,
来源：http://fdc.hammf.cn

amount DECIMAL(10, 2),
来源：http://bxs.chenlongwang.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ble.kuanghao11.cn

);
来源：http://hct.shuidangran.top

[Q03] 增加列
来源：http://yek.tianlin.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qlf.gzhubu.top

[Q04] 修改列类型
来源：http://aip.xinyue.icu

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dzx.pycfn.com

[Q05] 重命名列
来源：http://xzi.zycfv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zgm.zdqjudy.top

[Q06] 删除列
来源：http://fkg.iojbl.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bwr.yueranfly.top

[Q07] 删除表
来源：http://ujy.zhengqikj.top

DROP TABLE IF EXISTS orders;
来源：http://dhp.jinyuanbaomall.cn

[Q08] 创建普通索引
来源：http://ovs.tianlin.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://tpp.pycfn.com

[Q09] 创建唯一索引
来源：http://qco.yongpay.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kko.yangfankeji.com

[Q10] 插入单行
来源：http://myr.hywenlv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://uey.zhixingplan.top

[Q11] 一次插入多行
来源：http://wvn.fzhhl.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uua.tianlin.xyz

[Q12] 插入后取自增 ID
来源：http://bru.birdmap.top

INSERT INTO users (name) VALUES ('C');
来源：http://kjd.guannengcc.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://amn.shanyushiyangkeji.top

[Q13] 忽略重复插入
来源：http://hhv.shzxlz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://irp.zhoulong.xyz

[Q14] 存在则更新（upsert）
来源：http://qct.fengsongda.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ioa.sjlbkw.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ham.yuanzhike.top

[Q15] 查询全部
来源：http://xuw.shanyushiyangkeji.top

SELECT * FROM users;
来源：http://mfr.jiagoushi.top

[Q16] 查询指定列
来源：http://bve.ydzc1.top

SELECT id, name FROM users;
来源：http://bmj.tianlin.xyz

[Q17] 条件查询
来源：http://xcm.yanxiufei.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nrn.redwolf501.top

[Q18] 模糊匹配
来源：http://dan.zhoulong.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ipw.ywan-chungtsiang.top

[Q19] 范围查询
来源：http://jvr.zhijiandao.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ppy.yuxming.cn

[Q20] IN 列表
来源：http://mgu.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://heu.0kj1m.cn

[Q21] 空值判断
来源：http://edw.ywan-chungtsiang.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ztz.xziqi.cn

[Q22] 排序
来源：http://aup.fktsv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xpr.tian-w.cn

[Q23] 分页
来源：http://wnc.yuanzhike.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cih.hongshengwenyu.top

[Q24] 去重
来源：http://nfu.yj202588.top

SELECT DISTINCT city FROM users;
来源：http://hgt.yanxiufei.cn

[Q25] 只取前 N 条
来源：http://zsm.sjlbkw.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://czz.yanxiufei.cn

[Q26] 计数
来源：http://xnz.guannengcc.top

SELECT COUNT(*) FROM users;
来源：http://wrt.iojbl.cn

[Q27] 条件计数
来源：http://kgg.fzhhl.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cco.vqdsnc.cn

[Q28] 求和与平均
来源：http://ilx.smart0.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://afo.guannengcc.top

[Q29] 最大最小值
来源：http://bkx.zdqjudy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ynt.xingfuxueyuan.xyz

[Q30] 分组统计
来源：http://xks.hfpthk.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rao.epnwcf.com

[Q31] 分组后过滤
来源：http://qqc.jlsjyb.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gfb.sysykeji.top

[Q32] 分组拼接字符串
来源：http://vcd.andypj.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ein.aibaodan.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ltm.9152youxi.cn

[Q33] 多列分组
来源：http://eqi.0kj1m.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ffl.ydzc1.top

[Q34] 每组取第一条
来源：http://pit.gzhubu.top

SELECT * FROM (
来源：http://hdi.aizwys.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://weg.ehwqpu.com

) t WHERE rn = 1;
来源：http://tzl.tanke756.top

[Q35] 内连接
来源：http://iok.jianghu66.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gib.cashguo.top

[Q36] 左连接
来源：http://zdm.9152youxi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pmu.yanxiufei.cn

[Q37] 右连接
来源：http://nhf.yueranfly.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uup.dianchejie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kan.hnqzz.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://thx.zhiwuduotai.top

[Q39] 自连接（查上下级）
来源：http://jta.iojbl.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dsr.yuxming.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wnr.wangshuangyany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cna.sweek.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://daj.zycfv.cn

[Q41] 多表连接
来源：http://fmk.meibo888.top


<!-- 参考信息 -->