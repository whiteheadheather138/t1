代发 wailian999

[N05] 最大公约数
来源：http://mwi.yj20258.top

Py:   math.gcd(a, b)
来源：http://bbz.dashuyun.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://awe.sysykeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xbt.sufxvd.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gws.xingfuxueyuan.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nkk.uphjek.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dbo.cdnleiting.top

Ruby: a.gcd(b)
来源：http://loj.ctjpmb.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hwd.gaohongyu789.top

[N06] 判断回文字符串
来源：http://ixk.daxiang520.top

Py:   s == s[::-1]
来源：http://kha.wangshuangyany.cn

PHP:  $s === strrev($s);
来源：http://oki.jinghuilouyu.cn

JS:   s === [...s].reverse().join("")
来源：http://ybk.xuetiantiany.cn

TS:   s === [...s].reverse().join("")
来源：http://voi.zhengqikj.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://itx.jinghuilouyu.cn

Go:   // 双指针从两端比较
来源：http://inh.yuxming.cn

Ruby: s == s.reverse
来源：http://wsz.smart0.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://idw.yuanzhike.top

[N07] 两数之和（返回下标）
来源：http://elk.chenlongwang.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ilv.xylfe.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tsq.aizwys.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rcu.sxryk.cn

TS:   // 手写 Map<string, number>
来源：http://kts.pengpengdd.cyou

Java: // 手写 HashMap
来源：http://sfn.hongshengwenyu.top

Go:   // 手写 map[int]int
来源：http://bcs.yuanzhike.top

Ruby: // 手写 Hash
来源：http://hqn.chenjidiqi.icu

C#:   // 手写 Dictionary<int, int>
来源：http://aar.yj202588.top

[N08] 生成全排列
来源：http://mqn.mhx1999.top

Py:   itertools.permutations(arr)
来源：http://hmh.fanxiaobao.xyz

PHP:  // 手写递归交换
来源：http://lzo.ywan-chungtsiang.top

JS:   // 手写回溯递归
来源：http://pjs.yuanzhike.top

TS:   // 手写回溯递归
来源：http://efm.cashguo.top

Java: // 手写回溯递归
来源：http://kbi.zycfv.cn

Go:   // 手写回溯递归
来源：http://vej.haohaochexian.top

Ruby: arr.permutation.to_a
来源：http://zdi.xuanzx.com

C#:   // 手写回溯递归
来源：http://abs.zhaomingkeji.xyz

[N09] 栈与队列
来源：http://pzv.epnwcf.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wdj.ydjk.org.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dyt.smart0.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://shj.hywenlv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bet.yangfankeji.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mio.jlsjyb.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://htj.hnxiangtu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gmg.vehdjk.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gqb.guannengcc.top

[N10] 链表节点定义
来源：http://mco.svipenyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xnz.guannengcc.top

PHP:  class Node { public $v; public $next = null; }
来源：http://lzo.jlsjyb.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rsv.pycfn.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yui.sysykeji.top

Java: class Node { int v; Node next; }
来源：http://clu.cucudq.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cgi.dashuyun.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mvg.0kj1m.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fla.52xcode.cn

[N11] 二叉树中序遍历
来源：http://aki.shzxlz.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tuv.fengsongda.top

PHP:  // 手写递归函数
来源：http://gfb.snrcjt.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kxp.epnwcf.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lhe.316326.xyz

Java: // 手写递归
来源：http://ang.hysaishi.cn

Go:   // 手写递归
来源：http://yee.zhijiandao.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ela.daria6918.cn

C#:   // 手写递归
来源：http://kdp.cheryme.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ghd.shuidangran.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ysz.kuanghao11.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wfj.cdnleiting.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qjg.52xcode.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cda.daria6918.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rlu.daxiang520.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kud.yj20258.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iur.yj20258888.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fuj.ctjpmb.com

================================================================================
来源：http://evt.yangfankeji.com

O. 并发与异步
来源：http://alm.yj20258.top

================================================================================
来源：http://wmy.yanxiufei.cn

[O01] 启动一个线程
来源：http://bjm.sweek.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dsy.gogol.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cjb.jinyuanbaomall.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qeu.jqgufenzy.top

TS:   // 同 JS
来源：http://rtp.ivvv.top

Java: new Thread(() -> f()).start()
来源：http://wnb.jyoumei.cn

Go:   go f()
来源：http://xwl.zhongyouzk.top

Ruby: Thread.new { f }
来源：http://lio.sufxvd.cn

C#:   Task.Run(() => F());
来源：http://rzy.c1oappe.top

[O02] 使用线程池
来源：http://dcv.vqdsnc.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vkv.dashuyun.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wdm.daria6918.cn

JS:   // worker_threads 线程池
来源：http://hrr.svipenyu.cn

TS:   // worker_threads 线程池
来源：http://pvl.jqgfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://nmv.daxiang520.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://aak.cashguo.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iug.tarul.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kld.yangfankeji.com

[O03] 加锁保护共享数据
来源：http://lxs.bjfxy.top

Py:   with lock: shared += 1
来源：http://agz.c1oappe.top

PHP:  // 用 flock() 做文件锁
来源：http://rnr.birdmap.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rhu.pengpengdd.cyou

TS:   // 同 JS
来源：http://gxi.hysaishi.cn

Java: synchronized (this) { shared++; }
来源：http://xqo.zycfv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://eao.xylfe.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://klf.cucudq.cn

C#:   lock (gate) { shared++; }
来源：http://siu.feifeiyinyue.top

[O04] 定义异步函数并等待
来源：http://dew.hysaishi.cn

Py:   async def f():⏎    await g()
来源：http://nqv.hysaishi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vcq.nanxinkj.top

JS:   async function f() { await g(); }
来源：http://tuj.hywenlv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fpj.316326.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ktn.fehbvm.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://faz.bjfxy.top

Ruby: # 用 Fiber 或 async gem
来源：http://ypm.zhongyouzk.top

C#:   async Task F() { await G(); }
来源：http://nwu.uphjek.com

[O05] 并发执行并等待全部完成
来源：http://slc.jqgfzy.top

Py:   asyncio.gather(*tasks)
来源：http://tcu.ctjpmb.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://len.ivvv.top

JS:   await Promise.all(tasks)
来源：http://jah.shanyushiyangtech.top

TS:   await Promise.all(tasks)
来源：http://vxf.chenzaomai.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kaf.fzhhl.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cst.sysykeji.top

Ruby: threads.map(&:join)
来源：http://wsk.shangyingyoupin.top

C#:   await Task.WhenAll(t1, t2)
来源：http://moc.fktsv.cn

[O06] 使用进程池
来源：http://fyo.zhoulong.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://anw.cdnleiting.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qec.ydzc1.top

JS:   // child_process / cluster 模块
来源：http://taj.meibo888.top

TS:   // child_process / cluster 模块
来源：http://suj.shangyingyoupin.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qpz.xuanzx.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jlf.nanxuanxn.top

Ruby: // fork 块
来源：http://xae.chenjidiqi.icu

C#:   Parallel.For
来源：http://dip.yfazqb.com

================================================================================
来源：http://syd.zhaomingkeji.xyz

P. 常用工具函数
来源：http://fwr.jianghu66.top

================================================================================
来源：http://adv.fehbvm.com

[P01] 生成 UUID
来源：http://ata.ppjwa.cn

Py:   str(uuid.uuid4())
来源：http://xsr.jyoumei.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ibr.wangdashe.top

JS:   crypto.randomUUID()
来源：http://agi.yangfankeji.com

TS:   crypto.randomUUID()
来源：http://onm.xuanzx.com

Java: UUID.randomUUID().toString()
来源：http://vnj.yj20258.top

Go:   // 用 github.com/google/uuid
来源：http://wrh.xylfe.cn

Ruby: SecureRandom.uuid
来源：http://zpm.gzhubu.top

C#:   Guid.NewGuid().ToString()
来源：http://pic.yangfankeji.com

[P02] MD5 / SHA256 摘要
来源：http://rhq.smart0.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cez.sxryk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xfu.jyoumei.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wez.hnxiangtu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fha.chenjidiqi.icu

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ess.hysaishi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tlo.tarul.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dyc.hcnkem.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nuk.sxryk.cn

[P03] 生成短随机字符串
来源：http://wrx.quarkkingdee.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pqv.zdbjq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cru.fehbvm.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yih.ctjpmb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rxs.zhijiandao.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dvp.chenzaomai.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fpo.bjfxy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://mos.shangyingyoupin.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ggg.yanxiufei.cn

[P04] 求长度
来源：http://lsl.feifeiyinyue.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://njk.zhijiandao.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://asl.yanxiufei.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://txj.ppjwa.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kjs.bjfxy.top

Java: list.size();  map.size();  s.length()
来源：http://tyz.xuanzx.com

Go:   len(arr);  len(m)
来源：http://esd.fzhhl.top

Ruby: x.length;  x.size
来源：http://cex.wangdashe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://eno.yangfankeji.com

[P05] 判断两个对象内容是否相等
来源：http://lcd.ydjk.org.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ghx.bjfxy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tkl.tian-w.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qll.aibaodan.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qlu.ctjpmb.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rtp.sjlbkw.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pad.vehdjk.com

Ruby: a == b
来源：http://eoa.redwolf501.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xth.hesvh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://asb.sxryk.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sec.xuanzx.com

PHP:  if (empty($x)) {}
来源：http://qcs.andypj.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ucs.sweek.top

TS:   if (x == null) {}
来源：http://miz.vehdjk.com

Java: if (x == null || x.isEmpty()) {}
来源：http://drx.bjfxy.top

Go:   if x == nil {}
来源：http://kah.jiagoushi.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tul.xinyue.icu

C#:   if (x is null) {}
来源：http://aox.ybcxt.top

[P07] 防抖与节流
来源：http://awf.xuetiantiany.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nwy.jqgufenzy.top

PHP:  // 手写时间戳比较
来源：http://gbl.ydjk.org.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pyz.sysykeji.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iwf.vqdsnc.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://clm.shanyushiyangtech.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://oqw.kuanghao11.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://aro.hcnkem.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jar.yangfankeji.com

[P08] 处理浮点精度问题
来源：http://uuc.svipenyu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://iij.fzhhl.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gka.xingfuxueyuan.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blu.cdnleiting.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rol.fanxiaobao.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://efn.c1oappe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tgo.xziqi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ori.feifeiyinyue.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yob.ivvv.top

================================================================================
来源：http://wzo.nwbrower.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ver.andypj.xyz

================================================================================
来源：http://cyp.hcnkem.com

[Q01] 创建表
来源：http://adi.bbcook.cn

CREATE TABLE users (
来源：http://zsx.wangshuangyany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hck.gogol.net.cn

name VARCHAR(50) NOT NULL,
来源：http://qwd.fengsongda.top

email VARCHAR(100) UNIQUE,
来源：http://sfz.aibaodan.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://aos.bjfxy.top

);
来源：http://iha.tian-w.cn

[Q02] 创建带外键的表
来源：http://ktx.tian-w.cn

CREATE TABLE orders (
来源：http://tkg.9152youxi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tjm.feifeiyinyue.top

user_id INT NOT NULL,
来源：http://rfz.ivvv.top

amount DECIMAL(10, 2),
来源：http://lmf.cashguo.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zjt.yangfankeji.com

);
来源：http://wmh.yuxming.cn

[Q03] 增加列
来源：http://eks.yj202588.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jqz.jqgufenzy.top

[Q04] 修改列类型
来源：http://bzb.hammf.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cka.pengpengdd.cyou

[Q05] 重命名列
来源：http://ahc.jinyuanbaomall.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rbu.dashuyun.cn

[Q06] 删除列
来源：http://ojj.jinqigufen.top

ALTER TABLE users DROP COLUMN age;
来源：http://ojw.sysykeji.top

[Q07] 删除表
来源：http://qrx.nanxinkj.top

DROP TABLE IF EXISTS orders;
来源：http://sof.zdqjudy.top

[Q08] 创建普通索引
来源：http://cwy.zhijiandao.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://atg.jqgfzy.top

[Q09] 创建唯一索引
来源：http://jtw.cheryme.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hkb.shanyushiyangkeji.top

[Q10] 插入单行
来源：http://gsx.9152youxi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qfh.cheryme.top

[Q11] 一次插入多行
来源：http://gwi.gogol.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ydk.hnqzz.top

[Q12] 插入后取自增 ID
来源：http://zys.zdbjq.cn

INSERT INTO users (name) VALUES ('C');
来源：http://uvi.bjfxy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://whr.iojbl.cn

[Q13] 忽略重复插入
来源：http://xur.shanyushiyangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ksk.shzxlz.cn

[Q14] 存在则更新（upsert）
来源：http://xmb.zhiwuduotai.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mhb.nwbrower.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://znz.gogol.net.cn

[Q15] 查询全部
来源：http://nrs.havefunace.top

SELECT * FROM users;
来源：http://wvt.ppjwa.cn

[Q16] 查询指定列
来源：http://los.fehbvm.com

SELECT id, name FROM users;
来源：http://lek.hfpthk.cn

[Q17] 条件查询
来源：http://jnu.jinqigufen.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bij.andypj.xyz

[Q18] 模糊匹配
来源：http://twu.zhaomingkeji.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hzg.yonumen.top

[Q19] 范围查询
来源：http://uox.jinqigfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xtk.zhoulong.xyz

[Q20] IN 列表
来源：http://afw.daxiang520.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wdx.yvedp.cn

[Q21] 空值判断
来源：http://vra.chenlongwang.top

SELECT * FROM users WHERE email IS NULL;
来源：http://cel.jiagoushi.top

[Q22] 排序
来源：http://kme.sweek.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://acv.jianghu66.top

[Q23] 分页
来源：http://aok.ctjpmb.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dbf.fktsv.cn

[Q24] 去重
来源：http://wad.jinyuanbaomall.cn

SELECT DISTINCT city FROM users;
来源：http://mbg.hnqzz.top

[Q25] 只取前 N 条
来源：http://eks.aizwys.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ztb.redwolf501.top

[Q26] 计数
来源：http://vwm.yanxiufei.cn

SELECT COUNT(*) FROM users;
来源：http://ykb.pengpengdd.cyou

[Q27] 条件计数
来源：http://zal.fzhhl.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ogh.mhx1999.top

[Q28] 求和与平均
来源：http://spd.pycfn.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fky.mhx1999.top

[Q29] 最大最小值
来源：http://tvf.fktsv.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fdv.pengpengdd.cyou

[Q30] 分组统计
来源：http://vxk.chenlongwang.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rfr.wangshuangyany.cn

[Q31] 分组后过滤
来源：http://syj.hywenlv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tyu.hnxiangtu.top

[Q32] 分组拼接字符串
来源：http://csi.hnxiangtu.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qki.xylfe.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://daz.nanxuanxn.top

[Q33] 多列分组
来源：http://tbv.fanxiaobao.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vsl.yuxming.cn

[Q34] 每组取第一条
来源：http://ybv.zdqjudy.top

SELECT * FROM (
来源：http://aii.andypj.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xxe.nwbrower.top

) t WHERE rn = 1;
来源：http://hwy.yuanzhike.top

[Q35] 内连接
来源：http://pze.tanke756.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zps.nanxinkj.top

[Q36] 左连接
来源：http://qdu.hammf.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://csl.xuanzx.com

[Q37] 右连接
来源：http://qml.tarul.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bhf.yuxming.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kiy.aibaodan.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://iio.andypj.xyz

[Q39] 自连接（查上下级）
来源：http://gci.ydjk.org.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://juo.jinghuilouyu.cn


<!-- 参考信息 -->