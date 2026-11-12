代发 wailian999

[N05] 最大公约数
来源：http://low.ywan-chungtsiang.top

Py:   math.gcd(a, b)
来源：http://liv.ctjpmb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fhn.jinghuilouyu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://urb.nanxinkj.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fzd.fehbvm.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ewu.shanyushiyangtech.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gli.cucudq.cn

Ruby: a.gcd(b)
来源：http://dhg.xylfe.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wwy.pengpengdd.cyou

[N06] 判断回文字符串
来源：http://bve.bjfxy.top

Py:   s == s[::-1]
来源：http://hbw.jinqigufen.top

PHP:  $s === strrev($s);
来源：http://glw.hfpthk.cn

JS:   s === [...s].reverse().join("")
来源：http://pix.hongshengwenyu.top

TS:   s === [...s].reverse().join("")
来源：http://rzz.0kj1m.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fjm.chenzaomai.com

Go:   // 双指针从两端比较
来源：http://gju.tianlin.xyz

Ruby: s == s.reverse
来源：http://vop.jyoumei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wuq.hnqzz.top

[N07] 两数之和（返回下标）
来源：http://qyq.xuetiantiany.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ydq.ywan-chungtsiang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://khj.svipenyu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://idb.yuxming.cn

TS:   // 手写 Map<string, number>
来源：http://xru.yj20258.top

Java: // 手写 HashMap
来源：http://qei.hongshengwenyu.top

Go:   // 手写 map[int]int
来源：http://aco.jinyuanbaomall.cn

Ruby: // 手写 Hash
来源：http://dgm.zdqjudy.top

C#:   // 手写 Dictionary<int, int>
来源：http://vna.iojbl.cn

[N08] 生成全排列
来源：http://vdf.yfazqb.com

Py:   itertools.permutations(arr)
来源：http://art.zdbjq.cn

PHP:  // 手写递归交换
来源：http://wob.c1oappe.top

JS:   // 手写回溯递归
来源：http://nmj.fehbvm.com

TS:   // 手写回溯递归
来源：http://tbr.gotoacloud.top

Java: // 手写回溯递归
来源：http://qlw.xinyue.icu

Go:   // 手写回溯递归
来源：http://aei.mhx1999.top

Ruby: arr.permutation.to_a
来源：http://bxu.shuidangran.top

C#:   // 手写回溯递归
来源：http://ryv.andypj.xyz

[N09] 栈与队列
来源：http://zxy.ydzc1.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vju.sysykeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vbm.cdnleiting.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jdk.xingfuxueyuan.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tei.gaohongyu789.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ijb.cucudq.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mdv.zhixingplan.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xmg.zhijiandao.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gef.pengpengdd.cyou

[N10] 链表节点定义
来源：http://dij.redwolf501.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vaa.xuetiantiany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://erp.cashguo.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://opt.hnqzz.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ijo.fzhhl.top

Java: class Node { int v; Node next; }
来源：http://kue.vqdsnc.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hzd.gzhubu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://rsx.birdmap.top

C#:   class Node { public int V; public Node? Next; }
来源：http://heq.chenzaomai.com

[N11] 二叉树中序遍历
来源：http://uby.hysaishi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ggg.redwolf501.top

PHP:  // 手写递归函数
来源：http://wpi.yj202588.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://brp.52xcode.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cwv.xziqi.cn

Java: // 手写递归
来源：http://rbd.cucudq.cn

Go:   // 手写递归
来源：http://moo.uphjek.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nxc.dashuyun.cn

C#:   // 手写递归
来源：http://elt.zhaomingkeji.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://flt.smart0.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://roc.zdqjudy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cmj.chenzaomai.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zce.hfpthk.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://egk.zdqjudy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gkb.gotoacloud.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://eyr.zdqjudy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blt.quarkkingdee.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lro.nwbrower.top

================================================================================
来源：http://rww.xuanzx.com

O. 并发与异步
来源：http://wca.hcnkem.com

================================================================================
来源：http://duk.zdqjudy.top

[O01] 启动一个线程
来源：http://fxp.zhaomingkeji.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gkx.jlsjyb.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://goe.nanxinkj.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nqw.zdqjudy.top

TS:   // 同 JS
来源：http://tix.shangyingyoupin.top

Java: new Thread(() -> f()).start()
来源：http://wnw.quarkkingdee.top

Go:   go f()
来源：http://urj.xuanzx.com

Ruby: Thread.new { f }
来源：http://kgt.cqqwz.cn

C#:   Task.Run(() => F());
来源：http://rzo.guannengcc.top

[O02] 使用线程池
来源：http://ujk.ydjk.org.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://upf.snrcjt.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://czn.jqgfzy.top

JS:   // worker_threads 线程池
来源：http://olc.316326.xyz

TS:   // worker_threads 线程池
来源：http://xpw.aibaodan.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ofg.hesvh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kus.yuanzhike.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cfk.ydjk.org.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yca.snrcjt.cn

[O03] 加锁保护共享数据
来源：http://mhe.zhiwuduotai.top

Py:   with lock: shared += 1
来源：http://ynt.shanyushiyangtech.top

PHP:  // 用 flock() 做文件锁
来源：http://ojp.yangfankeji.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dkr.tian-w.cn

TS:   // 同 JS
来源：http://wsg.yuxming.cn

Java: synchronized (this) { shared++; }
来源：http://vfx.cucudq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://eod.fktsv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zyx.ppjwa.cn

C#:   lock (gate) { shared++; }
来源：http://fvs.yj202588.top

[O04] 定义异步函数并等待
来源：http://vhk.guannengcc.top

Py:   async def f():⏎    await g()
来源：http://wje.xziqi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cuv.aibaodan.cn

JS:   async function f() { await g(); }
来源：http://wqf.shzxlz.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fib.havefunace.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://atc.ctjpmb.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vnv.316326.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://ilx.tianlin.xyz

C#:   async Task F() { await G(); }
来源：http://zsa.hnxiangtu.top

[O05] 并发执行并等待全部完成
来源：http://sbo.cheryme.top

Py:   asyncio.gather(*tasks)
来源：http://pjr.daria6918.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dnx.tarul.cn

JS:   await Promise.all(tasks)
来源：http://jvj.iojbl.cn

TS:   await Promise.all(tasks)
来源：http://xbl.zhaomingkeji.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vco.chenjidiqi.icu

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dyt.hnqzz.top

Ruby: threads.map(&:join)
来源：http://itm.zdbjq.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pbr.ydjk.org.cn

[O06] 使用进程池
来源：http://hdz.yongpay.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hgm.yueranfly.top

PHP:  // pcntl_fork 或多进程队列
来源：http://wrq.chenzaomai.com

JS:   // child_process / cluster 模块
来源：http://ued.ctjpmb.com

TS:   // child_process / cluster 模块
来源：http://mfq.chenlongwang.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dck.dianchejie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xgv.gzhubu.top

Ruby: // fork 块
来源：http://hdb.jianghu66.top

C#:   Parallel.For
来源：http://rza.fanxiaobao.xyz

================================================================================
来源：http://czw.snrcjt.cn

P. 常用工具函数
来源：http://bcj.vqdsnc.cn

================================================================================
来源：http://ctt.yj20258.top

[P01] 生成 UUID
来源：http://ynn.shzxlz.cn

Py:   str(uuid.uuid4())
来源：http://lue.yj202588.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rwk.zhaomingkeji.xyz

JS:   crypto.randomUUID()
来源：http://rpe.jinyuanbaomall.cn

TS:   crypto.randomUUID()
来源：http://mgp.smart0.xyz

Java: UUID.randomUUID().toString()
来源：http://zgx.yongpay.top

Go:   // 用 github.com/google/uuid
来源：http://hvq.zhijiandao.cn

Ruby: SecureRandom.uuid
来源：http://ejr.hfpthk.cn

C#:   Guid.NewGuid().ToString()
来源：http://vqt.hongshengwenyu.top

[P02] MD5 / SHA256 摘要
来源：http://zbb.havefunace.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://efs.ehwqpu.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://drv.hongshengwenyu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gth.sweek.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://soe.xuetiantiany.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://joq.ywan-chungtsiang.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wza.zhengqikj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tlu.shangyingyoupin.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dox.yvedp.cn

[P03] 生成短随机字符串
来源：http://nxl.shangyingyoupin.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dfi.hesvh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cen.c1oappe.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gbv.jinghuilouyu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qyb.zhengqikj.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jqv.ehwqpu.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ihm.zhiwuduotai.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://sbi.cucudq.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ufa.jlsjyb.cn

[P04] 求长度
来源：http://pqa.redwolf501.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dxx.birdmap.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wmq.yvedp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xhq.shangyingyoupin.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ghk.uphjek.com

Java: list.size();  map.size();  s.length()
来源：http://syf.nanxinkj.top

Go:   len(arr);  len(m)
来源：http://jgy.feifeiyinyue.top

Ruby: x.length;  x.size
来源：http://ckk.xylfe.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ajm.svipenyu.cn

[P05] 判断两个对象内容是否相等
来源：http://bsr.bbcook.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kpe.yuanzhike.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qqv.dianchejie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qhk.gogol.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nxg.xingfuxueyuan.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xhp.yanxiufei.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ass.svipenyu.cn

Ruby: a == b
来源：http://iaz.pengpengdd.cyou

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wdl.shanyushiyangtech.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zko.fanxiaobao.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dba.aibaodan.cn

PHP:  if (empty($x)) {}
来源：http://ogi.cqqwz.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tmm.ydjk.org.cn

TS:   if (x == null) {}
来源：http://ujk.yfazqb.com

Java: if (x == null || x.isEmpty()) {}
来源：http://urw.meibo888.top

Go:   if x == nil {}
来源：http://xoz.guannengcc.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://edl.jyoumei.cn

C#:   if (x is null) {}
来源：http://dte.jianghu66.top

[P07] 防抖与节流
来源：http://wll.wangdashe.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zua.shangyingyoupin.top

PHP:  // 手写时间戳比较
来源：http://kmk.9152youxi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hgq.hongshengwenyu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uzs.nanxuanxn.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://foe.shzxlz.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gac.shanyushiyangtech.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://vpz.jinqigufen.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ryl.aibaodan.cn

[P08] 处理浮点精度问题
来源：http://uqo.fehbvm.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ykl.hammf.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nnb.yuxming.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zjr.xziqi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vzf.yangfankeji.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bea.yongpay.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kyn.xuanzx.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wig.hysaishi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cgb.iojbl.cn

================================================================================
来源：http://zwg.hywenlv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ivk.vqdsnc.cn

================================================================================
来源：http://qgy.cheryme.top

[Q01] 创建表
来源：http://vjr.quarkkingdee.top

CREATE TABLE users (
来源：http://vwp.pengpengdd.cyou

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xgk.chenjidiqi.icu

name VARCHAR(50) NOT NULL,
来源：http://ljq.fktsv.cn

email VARCHAR(100) UNIQUE,
来源：http://yvr.birdmap.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kaj.yonumen.top

);
来源：http://rnz.daria6918.cn

[Q02] 创建带外键的表
来源：http://euv.fktsv.cn

CREATE TABLE orders (
来源：http://hnp.svipenyu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://boa.yuxming.cn

user_id INT NOT NULL,
来源：http://yyn.yangfankeji.com

amount DECIMAL(10, 2),
来源：http://gxn.uphjek.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cga.hongshengwenyu.top

);
来源：http://omk.yongpay.top

[Q03] 增加列
来源：http://zmg.ctjpmb.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nsn.jinqigfzy.top

[Q04] 修改列类型
来源：http://gpy.0kj1m.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gvi.shuidangran.top

[Q05] 重命名列
来源：http://uzz.shanyushiyangtech.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lyw.gogol.net.cn

[Q06] 删除列
来源：http://dbz.yuxming.cn

ALTER TABLE users DROP COLUMN age;
来源：http://uvw.fehbvm.com

[Q07] 删除表
来源：http://tig.xingfuxueyuan.xyz

DROP TABLE IF EXISTS orders;
来源：http://yru.jinyuanbaomall.cn

[Q08] 创建普通索引
来源：http://fqw.ydzc1.top

CREATE INDEX idx_users_email ON users(email);
来源：http://gxq.9152youxi.cn

[Q09] 创建唯一索引
来源：http://wdp.cdnleiting.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lzp.zhengqikj.top

[Q10] 插入单行
来源：http://jui.kuanghao11.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qlo.jinqigfzy.top

[Q11] 一次插入多行
来源：http://ype.sjlbkw.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mlx.nanxuanxn.top

[Q12] 插入后取自增 ID
来源：http://xsw.zhiwuduotai.top

INSERT INTO users (name) VALUES ('C');
来源：http://cvk.chenjidiqi.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ehi.fehbvm.com

[Q13] 忽略重复插入
来源：http://jno.xinyue.icu

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lly.shuidangran.top

[Q14] 存在则更新（upsert）
来源：http://vua.jqgfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nbz.jinqigufen.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ixe.sjlbkw.cn

[Q15] 查询全部
来源：http://fju.uphjek.com

SELECT * FROM users;
来源：http://bvy.zhiwuduotai.top

[Q16] 查询指定列
来源：http://rjq.c1oappe.top

SELECT id, name FROM users;
来源：http://mpf.xuetiantiany.cn

[Q17] 条件查询
来源：http://cbi.gzhubu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tvc.wangshuangyany.cn

[Q18] 模糊匹配
来源：http://gfa.ywan-chungtsiang.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sfi.tanke756.top

[Q19] 范围查询
来源：http://zlh.gaohongyu789.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fyb.aibaodan.cn

[Q20] IN 列表
来源：http://pun.tarul.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zjp.dianchejie.cn

[Q21] 空值判断
来源：http://nkg.daria6918.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zns.meibo888.top

[Q22] 排序
来源：http://twa.dianchejie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wts.zhixingplan.top

[Q23] 分页
来源：http://alw.sufxvd.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qke.fanxiaobao.xyz

[Q24] 去重
来源：http://jsc.iojbl.cn

SELECT DISTINCT city FROM users;
来源：http://ioa.ywan-chungtsiang.top

[Q25] 只取前 N 条
来源：http://upi.feifeiyinyue.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rgq.sxryk.cn

[Q26] 计数
来源：http://jup.chenlongwang.top

SELECT COUNT(*) FROM users;
来源：http://kch.xuetiantiany.cn

[Q27] 条件计数
来源：http://wrr.hfpthk.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iti.sufxvd.cn

[Q28] 求和与平均
来源：http://zsm.birdmap.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zet.sysykeji.top

[Q29] 最大最小值
来源：http://uwv.mhx1999.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ajm.tarul.cn

[Q30] 分组统计
来源：http://unl.uphjek.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tdg.vehdjk.com

[Q31] 分组后过滤
来源：http://igw.zhiwuduotai.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bfx.ybcxt.top

[Q32] 分组拼接字符串
来源：http://oil.fanxiaobao.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://shk.guowangkeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://apc.daria6918.cn

[Q33] 多列分组
来源：http://fcf.bjfxy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xea.ywan-chungtsiang.top

[Q34] 每组取第一条
来源：http://jaf.ywan-chungtsiang.top

SELECT * FROM (
来源：http://bnh.sufxvd.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zlv.sxryk.cn

) t WHERE rn = 1;
来源：http://ezg.gogol.net.cn

[Q35] 内连接
来源：http://lna.sweek.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fif.havefunace.top

[Q36] 左连接
来源：http://pdw.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lcf.uphjek.com

[Q37] 右连接
来源：http://esl.xinyue.icu

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rpb.iojbl.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vwo.316326.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yct.tarul.cn

[Q39] 自连接（查上下级）
来源：http://hbn.ehwqpu.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://iiw.yanxiufei.cn


<!-- 参考信息 -->