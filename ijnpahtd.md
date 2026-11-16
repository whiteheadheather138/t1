代发 wailian999

[N05] 最大公约数
来源：http://abt.316326.xyz

Py:   math.gcd(a, b)
来源：http://yii.andypj.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kyo.jyoumei.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cnd.jlsjyb.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dpc.zhoulong.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fvt.daxiang520.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kyv.vehdjk.com

Ruby: a.gcd(b)
来源：http://aak.birdmap.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wcv.zhiwuduotai.top

[N06] 判断回文字符串
来源：http://lkk.hongshengwenyu.top

Py:   s == s[::-1]
来源：http://psb.gotoacloud.top

PHP:  $s === strrev($s);
来源：http://zao.sxryk.cn

JS:   s === [...s].reverse().join("")
来源：http://kcl.sysykeji.top

TS:   s === [...s].reverse().join("")
来源：http://fjn.9152youxi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zaz.zhoulong.xyz

Go:   // 双指针从两端比较
来源：http://mfm.hongshengwenyu.top

Ruby: s == s.reverse
来源：http://scl.smart0.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://fge.guowangkeji.top

[N07] 两数之和（返回下标）
来源：http://kgb.xinyue.icu

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://iyl.c1oappe.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://adm.jinqigfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://alj.jinqigfzy.top

TS:   // 手写 Map<string, number>
来源：http://gqj.sweek.top

Java: // 手写 HashMap
来源：http://wwa.tanke756.top

Go:   // 手写 map[int]int
来源：http://fey.hysaishi.cn

Ruby: // 手写 Hash
来源：http://qwt.yuxming.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ltj.jinqigufen.top

[N08] 生成全排列
来源：http://tgt.uphjek.com

Py:   itertools.permutations(arr)
来源：http://wrk.jqgufenzy.top

PHP:  // 手写递归交换
来源：http://upv.yonumen.top

JS:   // 手写回溯递归
来源：http://pnh.havefunace.top

TS:   // 手写回溯递归
来源：http://ekn.fehbvm.com

Java: // 手写回溯递归
来源：http://rxl.shanyushiyangtech.top

Go:   // 手写回溯递归
来源：http://srt.xuanzx.com

Ruby: arr.permutation.to_a
来源：http://dro.tianlin.xyz

C#:   // 手写回溯递归
来源：http://rgf.hongshengwenyu.top

[N09] 栈与队列
来源：http://bjk.fzhhl.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://eme.xziqi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yqm.jyoumei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xfl.yuxming.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cot.dashuyun.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hyf.ydzc1.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qdv.316326.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kta.guowangkeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wvl.svipenyu.cn

[N10] 链表节点定义
来源：http://nhx.zhaomingkeji.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wrm.ydzc1.top

PHP:  class Node { public $v; public $next = null; }
来源：http://dii.tarul.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ddz.shanyushiyangtech.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rpt.zhengqikj.top

Java: class Node { int v; Node next; }
来源：http://oka.guowangkeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://dtu.gogol.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lvk.hfpthk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://len.xylfe.cn

[N11] 二叉树中序遍历
来源：http://tek.dashuyun.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sfk.shuidangran.top

PHP:  // 手写递归函数
来源：http://hjb.52xcode.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jwd.mhx1999.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://akp.aizwys.cn

Java: // 手写递归
来源：http://suz.hcnkem.com

Go:   // 手写递归
来源：http://rdo.cheryme.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cdr.yj20258888.top

C#:   // 手写递归
来源：http://pll.jianghu66.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ouz.nanxinkj.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://aju.chenlongwang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://toz.hnxiangtu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sls.xylfe.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sdd.cucudq.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mui.pycfn.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zar.ywan-chungtsiang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cic.chenlongwang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xkd.sjlbkw.cn

================================================================================
来源：http://fvw.mhx1999.top

O. 并发与异步
来源：http://rvu.52xcode.cn

================================================================================
来源：http://lvs.yj202588.top

[O01] 启动一个线程
来源：http://aqv.guowangkeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tsz.xingfuxueyuan.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://twt.guowangkeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hly.yueranfly.top

TS:   // 同 JS
来源：http://vov.xylfe.cn

Java: new Thread(() -> f()).start()
来源：http://csc.hfpthk.cn

Go:   go f()
来源：http://nzk.jinqigufen.top

Ruby: Thread.new { f }
来源：http://fab.hcnkem.com

C#:   Task.Run(() => F());
来源：http://frm.iojbl.cn

[O02] 使用线程池
来源：http://wtg.kuanghao11.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xmz.sufxvd.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xnz.nanxuanxn.top

JS:   // worker_threads 线程池
来源：http://xyd.ydzc1.top

TS:   // worker_threads 线程池
来源：http://sfw.c1oappe.top

Java: Executors.newFixedThreadPool(4)
来源：http://zez.pycfn.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pcy.zdbjq.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rxs.yonumen.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bsk.xziqi.cn

[O03] 加锁保护共享数据
来源：http://wxo.hywenlv.cn

Py:   with lock: shared += 1
来源：http://lfq.wangdashe.top

PHP:  // 用 flock() 做文件锁
来源：http://rgb.jiagoushi.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nap.haohaochexian.top

TS:   // 同 JS
来源：http://jas.xylfe.cn

Java: synchronized (this) { shared++; }
来源：http://how.yj20258888.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nwg.epnwcf.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://xyw.jinghuilouyu.cn

C#:   lock (gate) { shared++; }
来源：http://nts.shuidangran.top

[O04] 定义异步函数并等待
来源：http://irf.epnwcf.com

Py:   async def f():⏎    await g()
来源：http://gxm.9152youxi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tfc.shanyushiyangtech.top

JS:   async function f() { await g(); }
来源：http://ncr.yfazqb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://ovz.yj202588.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yma.zycfv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ifb.ehwqpu.com

Ruby: # 用 Fiber 或 async gem
来源：http://gcd.cqqwz.cn

C#:   async Task F() { await G(); }
来源：http://fsx.ivvv.top

[O05] 并发执行并等待全部完成
来源：http://sif.dashuyun.cn

Py:   asyncio.gather(*tasks)
来源：http://wkk.nwbrower.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fii.daria6918.cn

JS:   await Promise.all(tasks)
来源：http://tfz.yvedp.cn

TS:   await Promise.all(tasks)
来源：http://chm.hongshengwenyu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://csm.ybcxt.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://raf.zhaomingkeji.xyz

Ruby: threads.map(&:join)
来源：http://nlo.pycfn.com

C#:   await Task.WhenAll(t1, t2)
来源：http://sbs.hfpthk.cn

[O06] 使用进程池
来源：http://oou.epnwcf.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bkx.meibo888.top

PHP:  // pcntl_fork 或多进程队列
来源：http://pya.fengsongda.top

JS:   // child_process / cluster 模块
来源：http://zkg.yongpay.top

TS:   // child_process / cluster 模块
来源：http://rkm.gotoacloud.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qdl.ydzc1.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ivx.xuetiantiany.cn

Ruby: // fork 块
来源：http://fmr.gotoacloud.top

C#:   Parallel.For
来源：http://ghr.316326.xyz

================================================================================
来源：http://jbw.yuanzhike.top

P. 常用工具函数
来源：http://bzu.316326.xyz

================================================================================
来源：http://fqz.sweek.top

[P01] 生成 UUID
来源：http://tpm.ctjpmb.com

Py:   str(uuid.uuid4())
来源：http://kuj.zhengqikj.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ybi.pengpengdd.cyou

JS:   crypto.randomUUID()
来源：http://bpp.yuxming.cn

TS:   crypto.randomUUID()
来源：http://elk.ivvv.top

Java: UUID.randomUUID().toString()
来源：http://dso.dianchejie.cn

Go:   // 用 github.com/google/uuid
来源：http://xyv.andypj.xyz

Ruby: SecureRandom.uuid
来源：http://dhp.daxiang520.top

C#:   Guid.NewGuid().ToString()
来源：http://bbf.quarkkingdee.top

[P02] MD5 / SHA256 摘要
来源：http://rtx.jlsjyb.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hdq.dashuyun.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gsd.zhongyouzk.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://olh.yanxiufei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ebm.ydjk.org.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vsz.haohaochexian.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cmk.gotoacloud.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pkr.quarkkingdee.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://loc.yj202588.top

[P03] 生成短随机字符串
来源：http://gtp.wangdashe.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://oiq.316326.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ajp.yj202588.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hfy.xuetiantiany.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gha.cdnleiting.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://odi.hnqzz.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kvu.yj20258.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://phi.hesvh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ewn.xylfe.cn

[P04] 求长度
来源：http://ucg.tianlin.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gmt.ydzc1.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vjd.snrcjt.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mhm.yuanzhike.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nhi.yuxming.cn

Java: list.size();  map.size();  s.length()
来源：http://azb.meibo888.top

Go:   len(arr);  len(m)
来源：http://rgs.zhijiandao.cn

Ruby: x.length;  x.size
来源：http://ftw.ydzc1.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://vgx.zhengqikj.top

[P05] 判断两个对象内容是否相等
来源：http://zxa.kuanghao11.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://nel.hysaishi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xcy.bjfxy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ibx.cucudq.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ocm.shanyushiyangkeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nfb.epnwcf.com

Go:   reflect.DeepEqual(a, b)
来源：http://fwg.cucudq.cn

Ruby: a == b
来源：http://zzq.chenlongwang.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wii.yanxiufei.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sdr.iojbl.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sio.dashuyun.cn

PHP:  if (empty($x)) {}
来源：http://cfv.ivvv.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yyt.jqgufenzy.top

TS:   if (x == null) {}
来源：http://ack.fanxiaobao.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://cun.hongshengwenyu.top

Go:   if x == nil {}
来源：http://epe.ybcxt.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://crg.yvedp.cn

C#:   if (x is null) {}
来源：http://kwo.yanxiufei.cn

[P07] 防抖与节流
来源：http://fxw.0kj1m.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ush.jiagoushi.top

PHP:  // 手写时间戳比较
来源：http://ame.yj20258888.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tqo.fanxiaobao.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fvo.hcnkem.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://iyi.jlsjyb.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cxp.haohaochexian.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://hxt.mhx1999.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vde.ydjk.org.cn

[P08] 处理浮点精度问题
来源：http://dph.yuanzhike.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nbq.svipenyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://aqv.hysaishi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gdn.mhx1999.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uwd.fengsongda.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://czx.hesvh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gbf.yueranfly.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rox.gotoacloud.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ulm.jinghuilouyu.cn

================================================================================
来源：http://iwf.shzxlz.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ori.jinqigufen.top

================================================================================
来源：http://ivt.tanke756.top

[Q01] 创建表
来源：http://dgy.ybcxt.top

CREATE TABLE users (
来源：http://vst.epnwcf.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://apr.yonumen.top

name VARCHAR(50) NOT NULL,
来源：http://wdd.yongpay.top

email VARCHAR(100) UNIQUE,
来源：http://vqw.feifeiyinyue.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qtp.bbcook.cn

);
来源：http://lwn.shuidangran.top

[Q02] 创建带外键的表
来源：http://yft.chenjidiqi.icu

CREATE TABLE orders (
来源：http://cye.sxryk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wmm.daxiang520.top

user_id INT NOT NULL,
来源：http://bbd.ivvv.top

amount DECIMAL(10, 2),
来源：http://ulf.hysaishi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tej.yueranfly.top

);
来源：http://ebl.yuanzhike.top

[Q03] 增加列
来源：http://nxz.yj202588.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://laf.bbcook.cn

[Q04] 修改列类型
来源：http://zwu.cucudq.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cup.mhx1999.top

[Q05] 重命名列
来源：http://ngn.guowangkeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yiu.316326.xyz

[Q06] 删除列
来源：http://hza.cdnleiting.top

ALTER TABLE users DROP COLUMN age;
来源：http://qjl.c1oappe.top

[Q07] 删除表
来源：http://nif.sysykeji.top

DROP TABLE IF EXISTS orders;
来源：http://zyv.hfpthk.cn

[Q08] 创建普通索引
来源：http://rna.jinghuilouyu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ind.tian-w.cn

[Q09] 创建唯一索引
来源：http://atp.gotoacloud.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://msf.zhongyouzk.top

[Q10] 插入单行
来源：http://ygz.316326.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mav.jianghu66.top

[Q11] 一次插入多行
来源：http://ptl.fzhhl.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iot.yangfankeji.com

[Q12] 插入后取自增 ID
来源：http://xas.wangdashe.top

INSERT INTO users (name) VALUES ('C');
来源：http://uhm.hongshengwenyu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pdl.jinqigfzy.top

[Q13] 忽略重复插入
来源：http://xxb.jlsjyb.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ndr.hfpthk.cn

[Q14] 存在则更新（upsert）
来源：http://ljs.zhaomingkeji.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://izz.redwolf501.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ftx.yongpay.top

[Q15] 查询全部
来源：http://mmh.guowangkeji.top

SELECT * FROM users;
来源：http://iaw.sjlbkw.cn

[Q16] 查询指定列
来源：http://fqh.smart0.xyz

SELECT id, name FROM users;
来源：http://miq.ppjwa.cn

[Q17] 条件查询
来源：http://asi.iojbl.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blt.hysaishi.cn

[Q18] 模糊匹配
来源：http://ytl.bjfxy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uym.xingfuxueyuan.xyz

[Q19] 范围查询
来源：http://bkn.52xcode.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ilq.tianlin.xyz

[Q20] IN 列表
来源：http://isa.haohaochexian.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://igk.vqdsnc.cn

[Q21] 空值判断
来源：http://log.c1oappe.top

SELECT * FROM users WHERE email IS NULL;
来源：http://lhv.tian-w.cn

[Q22] 排序
来源：http://tak.hnxiangtu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ibm.feifeiyinyue.top

[Q23] 分页
来源：http://tgm.iojbl.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oou.zhijiandao.cn

[Q24] 去重
来源：http://lkt.fktsv.cn

SELECT DISTINCT city FROM users;
来源：http://wct.gaohongyu789.top

[Q25] 只取前 N 条
来源：http://wtb.zdbjq.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://oyz.yj20258888.top

[Q26] 计数
来源：http://gsz.gzhubu.top

SELECT COUNT(*) FROM users;
来源：http://wxe.cqqwz.cn

[Q27] 条件计数
来源：http://rre.sxryk.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rnt.hongshengwenyu.top

[Q28] 求和与平均
来源：http://cyl.chenjidiqi.icu

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fvy.tianlin.xyz

[Q29] 最大最小值
来源：http://sja.jyoumei.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ejv.svipenyu.cn

[Q30] 分组统计
来源：http://pzk.zdqjudy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tii.smart0.xyz

[Q31] 分组后过滤
来源：http://qia.0kj1m.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wrv.yongpay.top

[Q32] 分组拼接字符串
来源：http://dqd.sjlbkw.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wdh.dianchejie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vrw.316326.xyz

[Q33] 多列分组
来源：http://cqk.chenjidiqi.icu

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fob.pycfn.com

[Q34] 每组取第一条
来源：http://qkt.yonumen.top

SELECT * FROM (
来源：http://xxm.shuidangran.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kqt.snrcjt.cn

) t WHERE rn = 1;
来源：http://amb.sjlbkw.cn

[Q35] 内连接
来源：http://dgl.wangdashe.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://izj.dashuyun.cn

[Q36] 左连接
来源：http://pyj.ybcxt.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nfh.yuxming.cn

[Q37] 右连接
来源：http://hue.xuetiantiany.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://eso.yuanzhike.top

[Q38] 全外连接（PostgreSQL）
来源：http://blh.yueranfly.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vya.mhx1999.top

[Q39] 自连接（查上下级）
来源：http://msj.haohaochexian.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ndz.uphjek.com


<!-- 参考信息 -->