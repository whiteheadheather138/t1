代发 wailian999

[N05] 最大公约数
来源：http://hci.yvedp.cn

Py:   math.gcd(a, b)
来源：http://wec.meibo888.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qrh.iojbl.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uga.xingfuxueyuan.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://inr.daria6918.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jhf.yanxiufei.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hct.ehwqpu.com

Ruby: a.gcd(b)
来源：http://bru.tian-w.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fyd.sjlbkw.cn

[N06] 判断回文字符串
来源：http://fyz.yj202588.top

Py:   s == s[::-1]
来源：http://yac.aizwys.cn

PHP:  $s === strrev($s);
来源：http://lsq.sweek.top

JS:   s === [...s].reverse().join("")
来源：http://wvb.chenjidiqi.icu

TS:   s === [...s].reverse().join("")
来源：http://pgc.yvedp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dlb.bbcook.cn

Go:   // 双指针从两端比较
来源：http://ihb.hysaishi.cn

Ruby: s == s.reverse
来源：http://qhg.yj202588.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://tuq.snrcjt.cn

[N07] 两数之和（返回下标）
来源：http://rhb.yj20258.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rmc.kuanghao11.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ali.jlsjyb.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yge.yonumen.top

TS:   // 手写 Map<string, number>
来源：http://jti.52xcode.cn

Java: // 手写 HashMap
来源：http://pox.yonumen.top

Go:   // 手写 map[int]int
来源：http://ftz.hammf.cn

Ruby: // 手写 Hash
来源：http://out.yj202588.top

C#:   // 手写 Dictionary<int, int>
来源：http://shl.fzhhl.top

[N08] 生成全排列
来源：http://pgc.cqqwz.cn

Py:   itertools.permutations(arr)
来源：http://pwd.bbcook.cn

PHP:  // 手写递归交换
来源：http://uwn.gzhubu.top

JS:   // 手写回溯递归
来源：http://emn.snrcjt.cn

TS:   // 手写回溯递归
来源：http://erh.yj20258.top

Java: // 手写回溯递归
来源：http://won.sysykeji.top

Go:   // 手写回溯递归
来源：http://ine.yj20258.top

Ruby: arr.permutation.to_a
来源：http://thv.yangfankeji.com

C#:   // 手写回溯递归
来源：http://yuz.fehbvm.com

[N09] 栈与队列
来源：http://uuo.mhx1999.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nol.jinqigfzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xtg.xuetiantiany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qir.chenjidiqi.icu

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sln.bjfxy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://iqj.fengsongda.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vsm.hfpthk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uij.yueranfly.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nfw.yuxming.cn

[N10] 链表节点定义
来源：http://xno.jiagoushi.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://inr.nwbrower.top

PHP:  class Node { public $v; public $next = null; }
来源：http://nqi.jlsjyb.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dlk.daria6918.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://quv.wangshuangyany.cn

Java: class Node { int v; Node next; }
来源：http://vup.guowangkeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://spm.mhx1999.top

Ruby: Node = Struct.new(:v, :next)
来源：http://rsd.chenzaomai.com

C#:   class Node { public int V; public Node? Next; }
来源：http://aip.hnxiangtu.top

[N11] 二叉树中序遍历
来源：http://xdn.jinqigufen.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ksm.nanxinkj.top

PHP:  // 手写递归函数
来源：http://crj.316326.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cks.yongpay.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cmb.jinqigufen.top

Java: // 手写递归
来源：http://spg.mhx1999.top

Go:   // 手写递归
来源：http://kmf.zhengqikj.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kws.kuanghao11.cn

C#:   // 手写递归
来源：http://giw.dianchejie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fqm.zhoulong.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cww.quarkkingdee.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gfn.wangshuangyany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rcs.havefunace.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zmg.meibo888.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vdo.andypj.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wad.daxiang520.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lvz.gaohongyu789.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://efm.yfazqb.com

================================================================================
来源：http://fep.zhiwuduotai.top

O. 并发与异步
来源：http://xes.hcnkem.com

================================================================================
来源：http://kby.zhaomingkeji.xyz

[O01] 启动一个线程
来源：http://jjh.yfazqb.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://aqg.sysykeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jnz.yj20258.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vdf.svipenyu.cn

TS:   // 同 JS
来源：http://qtn.yfazqb.com

Java: new Thread(() -> f()).start()
来源：http://sdm.yonumen.top

Go:   go f()
来源：http://wky.mhx1999.top

Ruby: Thread.new { f }
来源：http://lfn.daria6918.cn

C#:   Task.Run(() => F());
来源：http://tts.ydzc1.top

[O02] 使用线程池
来源：http://oay.uphjek.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://arl.epnwcf.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kws.ydjk.org.cn

JS:   // worker_threads 线程池
来源：http://tmx.daxiang520.top

TS:   // worker_threads 线程池
来源：http://qnd.zhaomingkeji.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://iqn.cqqwz.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ahs.c1oappe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nea.yonumen.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yzq.zhoulong.xyz

[O03] 加锁保护共享数据
来源：http://nvu.redwolf501.top

Py:   with lock: shared += 1
来源：http://oxu.cqqwz.cn

PHP:  // 用 flock() 做文件锁
来源：http://job.shuidangran.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mav.xziqi.cn

TS:   // 同 JS
来源：http://oha.hysaishi.cn

Java: synchronized (this) { shared++; }
来源：http://npm.kuanghao11.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://euk.yanxiufei.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://nqr.zhiwuduotai.top

C#:   lock (gate) { shared++; }
来源：http://lsd.fzhhl.top

[O04] 定义异步函数并等待
来源：http://bab.ivvv.top

Py:   async def f():⏎    await g()
来源：http://shp.gaohongyu789.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zia.zycfv.cn

JS:   async function f() { await g(); }
来源：http://ufq.cqqwz.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zfe.yanxiufei.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tlu.uphjek.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kef.tian-w.cn

Ruby: # 用 Fiber 或 async gem
来源：http://imj.gaohongyu789.top

C#:   async Task F() { await G(); }
来源：http://gok.havefunace.top

[O05] 并发执行并等待全部完成
来源：http://fjb.aizwys.cn

Py:   asyncio.gather(*tasks)
来源：http://bax.hywenlv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lbj.yvedp.cn

JS:   await Promise.all(tasks)
来源：http://vou.ehwqpu.com

TS:   await Promise.all(tasks)
来源：http://ede.xuanzx.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ckb.cdnleiting.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rcv.havefunace.top

Ruby: threads.map(&:join)
来源：http://hgo.fzhhl.top

C#:   await Task.WhenAll(t1, t2)
来源：http://qjq.fzhhl.top

[O06] 使用进程池
来源：http://qmv.chenjidiqi.icu

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mxd.hfpthk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ofm.hywenlv.cn

JS:   // child_process / cluster 模块
来源：http://ibo.fengsongda.top

TS:   // child_process / cluster 模块
来源：http://zjh.wangdashe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vmz.xziqi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://viy.yongpay.top

Ruby: // fork 块
来源：http://chl.ppjwa.cn

C#:   Parallel.For
来源：http://yuq.jinqigfzy.top

================================================================================
来源：http://xto.fktsv.cn

P. 常用工具函数
来源：http://zrx.cqqwz.cn

================================================================================
来源：http://rdh.guannengcc.top

[P01] 生成 UUID
来源：http://ikn.daria6918.cn

Py:   str(uuid.uuid4())
来源：http://ssj.fengsongda.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://drf.cheryme.top

JS:   crypto.randomUUID()
来源：http://tlo.zhoulong.xyz

TS:   crypto.randomUUID()
来源：http://abs.xuanzx.com

Java: UUID.randomUUID().toString()
来源：http://zxb.gaohongyu789.top

Go:   // 用 github.com/google/uuid
来源：http://dad.aibaodan.cn

Ruby: SecureRandom.uuid
来源：http://mya.yueranfly.top

C#:   Guid.NewGuid().ToString()
来源：http://sna.sxryk.cn

[P02] MD5 / SHA256 摘要
来源：http://rne.zdqjudy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lsn.cdnleiting.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://bqf.chenlongwang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ghr.nanxinkj.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tnv.epnwcf.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://imf.fktsv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sfa.guowangkeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://upq.hywenlv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://okv.svipenyu.cn

[P03] 生成短随机字符串
来源：http://jsk.shangyingyoupin.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://loy.dianchejie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fsb.nanxinkj.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yso.smart0.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bsp.bbcook.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wtj.birdmap.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vmy.ctjpmb.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://xpv.zdbjq.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://odq.jianghu66.top

[P04] 求长度
来源：http://mpp.c1oappe.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://szl.hnqzz.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fyk.yj20258.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yij.quarkkingdee.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://elz.jinqigufen.top

Java: list.size();  map.size();  s.length()
来源：http://zfr.fengsongda.top

Go:   len(arr);  len(m)
来源：http://hbz.vehdjk.com

Ruby: x.length;  x.size
来源：http://fbu.zhiwuduotai.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ndy.yuanzhike.top

[P05] 判断两个对象内容是否相等
来源：http://nxt.fehbvm.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://ons.jinghuilouyu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fiz.xingfuxueyuan.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nkg.ivvv.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lcg.fehbvm.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://onz.ctjpmb.com

Go:   reflect.DeepEqual(a, b)
来源：http://nfc.nanxinkj.top

Ruby: a == b
来源：http://snm.vehdjk.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jrg.cheryme.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pfg.cdnleiting.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://aoc.gzhubu.top

PHP:  if (empty($x)) {}
来源：http://skx.snrcjt.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vdk.yj202588.top

TS:   if (x == null) {}
来源：http://llh.daria6918.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://asc.tarul.cn

Go:   if x == nil {}
来源：http://kxu.jiagoushi.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nti.kuanghao11.cn

C#:   if (x is null) {}
来源：http://jnc.sufxvd.cn

[P07] 防抖与节流
来源：http://cfz.andypj.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gwe.316326.xyz

PHP:  // 手写时间戳比较
来源：http://uiu.ywan-chungtsiang.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dhs.chenzaomai.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cjp.cdnleiting.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bsi.chenjidiqi.icu

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qxs.cashguo.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zeu.sysykeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lcw.hnxiangtu.top

[P08] 处理浮点精度问题
来源：http://eai.fzhhl.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://une.9152youxi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ctt.hnxiangtu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bei.kuanghao11.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uyw.sufxvd.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oqe.yuanzhike.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fwj.tarul.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hgq.zdqjudy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pmr.jinqigufen.top

================================================================================
来源：http://kau.yongpay.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hsb.hysaishi.cn

================================================================================
来源：http://gpx.xuanzx.com

[Q01] 创建表
来源：http://hhj.epnwcf.com

CREATE TABLE users (
来源：http://pnd.yuxming.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ayq.chenlongwang.top

name VARCHAR(50) NOT NULL,
来源：http://vwc.svipenyu.cn

email VARCHAR(100) UNIQUE,
来源：http://cln.fehbvm.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://iga.aizwys.cn

);
来源：http://tjq.shanyushiyangkeji.top

[Q02] 创建带外键的表
来源：http://lbh.cucudq.cn

CREATE TABLE orders (
来源：http://toh.cdnleiting.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ikp.cheryme.top

user_id INT NOT NULL,
来源：http://zkd.bbcook.cn

amount DECIMAL(10, 2),
来源：http://kqj.snrcjt.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lfa.jinqigufen.top

);
来源：http://rtp.hcnkem.com

[Q03] 增加列
来源：http://ieu.jlsjyb.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xxr.jyoumei.cn

[Q04] 修改列类型
来源：http://uio.yvedp.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gsl.shangyingyoupin.top

[Q05] 重命名列
来源：http://rkg.jianghu66.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tgv.zycfv.cn

[Q06] 删除列
来源：http://fmm.uphjek.com

ALTER TABLE users DROP COLUMN age;
来源：http://jgp.havefunace.top

[Q07] 删除表
来源：http://dvt.hfpthk.cn

DROP TABLE IF EXISTS orders;
来源：http://wkx.cheryme.top

[Q08] 创建普通索引
来源：http://vzb.yuanzhike.top

CREATE INDEX idx_users_email ON users(email);
来源：http://rmc.hywenlv.cn

[Q09] 创建唯一索引
来源：http://xrn.quarkkingdee.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://oha.sysykeji.top

[Q10] 插入单行
来源：http://tnq.snrcjt.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://usy.tanke756.top

[Q11] 一次插入多行
来源：http://xwe.yanxiufei.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://oho.hongshengwenyu.top

[Q12] 插入后取自增 ID
来源：http://wdo.jqgufenzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://ero.jqgufenzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hga.shzxlz.cn

[Q13] 忽略重复插入
来源：http://vmm.yj20258888.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://roa.xingfuxueyuan.xyz

[Q14] 存在则更新（upsert）
来源：http://ern.fanxiaobao.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zme.kuanghao11.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://iuu.haohaochexian.top

[Q15] 查询全部
来源：http://ooy.xylfe.cn

SELECT * FROM users;
来源：http://hmy.sufxvd.cn

[Q16] 查询指定列
来源：http://yea.yueranfly.top

SELECT id, name FROM users;
来源：http://dtc.chenjidiqi.icu

[Q17] 条件查询
来源：http://ybt.hnxiangtu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qbl.zhixingplan.top

[Q18] 模糊匹配
来源：http://wbv.cdnleiting.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ogi.jianghu66.top

[Q19] 范围查询
来源：http://ell.birdmap.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://art.ybcxt.top

[Q20] IN 列表
来源：http://dgv.ywan-chungtsiang.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://syc.jianghu66.top

[Q21] 空值判断
来源：http://fei.gotoacloud.top

SELECT * FROM users WHERE email IS NULL;
来源：http://bqu.sweek.top

[Q22] 排序
来源：http://lvm.shanyushiyangtech.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cnz.xuanzx.com

[Q23] 分页
来源：http://gul.shanyushiyangtech.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pci.hnxiangtu.top

[Q24] 去重
来源：http://uti.gotoacloud.top

SELECT DISTINCT city FROM users;
来源：http://hbn.yj20258.top

[Q25] 只取前 N 条
来源：http://eat.jinghuilouyu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wqh.hnxiangtu.top

[Q26] 计数
来源：http://djb.gotoacloud.top

SELECT COUNT(*) FROM users;
来源：http://pzx.hesvh.cn

[Q27] 条件计数
来源：http://xcy.jinqigufen.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xwy.jianghu66.top

[Q28] 求和与平均
来源：http://hwg.yonumen.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jxh.gaohongyu789.top

[Q29] 最大最小值
来源：http://iju.aibaodan.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://iyr.fanxiaobao.xyz

[Q30] 分组统计
来源：http://nhb.daria6918.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mvk.zdbjq.cn

[Q31] 分组后过滤
来源：http://aug.hywenlv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kbz.cqqwz.cn

[Q32] 分组拼接字符串
来源：http://qio.pengpengdd.cyou

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ebw.jqgufenzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ihc.nwbrower.top

[Q33] 多列分组
来源：http://sha.tian-w.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://brf.ehwqpu.com

[Q34] 每组取第一条
来源：http://uhj.quarkkingdee.top

SELECT * FROM (
来源：http://epo.wangdashe.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rbk.havefunace.top

) t WHERE rn = 1;
来源：http://dip.jinqigfzy.top

[Q35] 内连接
来源：http://wug.zhijiandao.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kjm.hywenlv.cn

[Q36] 左连接
来源：http://pzm.jinqigufen.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qkg.gogol.net.cn

[Q37] 右连接
来源：http://fcr.sjlbkw.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yzm.shangyingyoupin.top

[Q38] 全外连接（PostgreSQL）
来源：http://imi.vqdsnc.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xnv.vehdjk.com

[Q39] 自连接（查上下级）
来源：http://dro.quarkkingdee.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://xhd.jinqigfzy.top


<!-- 参考信息 -->