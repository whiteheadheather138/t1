代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mrt.dashuyun.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zcd.xuetiantiany.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gqx.hnqzz.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gfd.vqdsnc.cn

[N05] 最大公约数
来源：http://eyk.dashuyun.cn

Py:   math.gcd(a, b)
来源：http://tje.c1oappe.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yuf.gotoacloud.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jod.xingfuxueyuan.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ivl.xuanzx.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://njs.havefunace.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uhi.xylfe.cn

Ruby: a.gcd(b)
来源：http://krz.ywan-chungtsiang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jmk.zdqjudy.top

[N06] 判断回文字符串
来源：http://uga.havefunace.top

Py:   s == s[::-1]
来源：http://hku.pengpengdd.cyou

PHP:  $s === strrev($s);
来源：http://axl.chenjidiqi.icu

JS:   s === [...s].reverse().join("")
来源：http://fcd.zdqjudy.top

TS:   s === [...s].reverse().join("")
来源：http://uol.hesvh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://awn.yongpay.top

Go:   // 双指针从两端比较
来源：http://ymj.yangfankeji.com

Ruby: s == s.reverse
来源：http://wes.nanxuanxn.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jkj.ppjwa.cn

[N07] 两数之和（返回下标）
来源：http://jfv.jiagoushi.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://snp.dianchejie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nsv.9152youxi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ttk.snrcjt.cn

TS:   // 手写 Map<string, number>
来源：http://vzn.xylfe.cn

Java: // 手写 HashMap
来源：http://lpm.daria6918.cn

Go:   // 手写 map[int]int
来源：http://eao.kuanghao11.cn

Ruby: // 手写 Hash
来源：http://udk.sxryk.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gci.tianlin.xyz

[N08] 生成全排列
来源：http://nkk.tian-w.cn

Py:   itertools.permutations(arr)
来源：http://ohq.zhoulong.xyz

PHP:  // 手写递归交换
来源：http://wso.sufxvd.cn

JS:   // 手写回溯递归
来源：http://oqh.chenjidiqi.icu

TS:   // 手写回溯递归
来源：http://txu.aibaodan.cn

Java: // 手写回溯递归
来源：http://bdo.chenzaomai.com

Go:   // 手写回溯递归
来源：http://pks.cdnleiting.top

Ruby: arr.permutation.to_a
来源：http://kae.fanxiaobao.xyz

C#:   // 手写回溯递归
来源：http://ueb.cheryme.top

[N09] 栈与队列
来源：http://oub.ctjpmb.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hrp.vqdsnc.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xxg.iojbl.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://upz.316326.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://feq.cashguo.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xuj.ybcxt.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://arf.yj202588.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sbj.zhoulong.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uxe.ehwqpu.com

[N10] 链表节点定义
来源：http://key.sjlbkw.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sqv.hnqzz.top

PHP:  class Node { public $v; public $next = null; }
来源：http://gtu.tianlin.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xes.zhengqikj.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hwl.shanyushiyangkeji.top

Java: class Node { int v; Node next; }
来源：http://ykt.ybcxt.top

Go:   type Node struct { V int; Next *Node }
来源：http://ceu.yanxiufei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gtc.jqgfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://vhu.pengpengdd.cyou

[N11] 二叉树中序遍历
来源：http://dyg.guowangkeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://acq.zycfv.cn

PHP:  // 手写递归函数
来源：http://ejh.xingfuxueyuan.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xql.0kj1m.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bje.ehwqpu.com

Java: // 手写递归
来源：http://nsw.nwbrower.top

Go:   // 手写递归
来源：http://jgm.ivvv.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qod.cdnleiting.top

C#:   // 手写递归
来源：http://luq.yuxming.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hdo.shzxlz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nqw.hnqzz.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://obc.hnxiangtu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dla.andypj.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hso.ywan-chungtsiang.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zyd.sweek.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mbq.cucudq.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://udx.bjfxy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bcy.zhongyouzk.top

================================================================================
来源：http://qyh.epnwcf.com

O. 并发与异步
来源：http://ual.xingfuxueyuan.xyz

================================================================================
来源：http://vvb.hnxiangtu.top

[O01] 启动一个线程
来源：http://ftd.dashuyun.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hcx.andypj.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fsg.hammf.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ftg.smart0.xyz

TS:   // 同 JS
来源：http://jvv.tian-w.cn

Java: new Thread(() -> f()).start()
来源：http://cnu.yuanzhike.top

Go:   go f()
来源：http://qlu.yangfankeji.com

Ruby: Thread.new { f }
来源：http://gvm.sysykeji.top

C#:   Task.Run(() => F());
来源：http://cfx.ppjwa.cn

[O02] 使用线程池
来源：http://tdt.shanyushiyangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cqp.c1oappe.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://alz.cheryme.top

JS:   // worker_threads 线程池
来源：http://myy.fanxiaobao.xyz

TS:   // worker_threads 线程池
来源：http://hld.zycfv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vvq.epnwcf.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://eor.wangdashe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://odf.yonumen.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kwr.andypj.xyz

[O03] 加锁保护共享数据
来源：http://exi.havefunace.top

Py:   with lock: shared += 1
来源：http://qty.kuanghao11.cn

PHP:  // 用 flock() 做文件锁
来源：http://kth.zdqjudy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gvu.zhoulong.xyz

TS:   // 同 JS
来源：http://pgg.ybcxt.top

Java: synchronized (this) { shared++; }
来源：http://qvy.haohaochexian.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hto.zhengqikj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://gem.hammf.cn

C#:   lock (gate) { shared++; }
来源：http://srz.hesvh.cn

[O04] 定义异步函数并等待
来源：http://arl.shanyushiyangkeji.top

Py:   async def f():⏎    await g()
来源：http://fce.shzxlz.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tdw.zhengqikj.top

JS:   async function f() { await g(); }
来源：http://sfu.shanyushiyangtech.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://kwh.52xcode.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fkj.cqqwz.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cpv.sjlbkw.cn

Ruby: # 用 Fiber 或 async gem
来源：http://iba.pengpengdd.cyou

C#:   async Task F() { await G(); }
来源：http://wcg.gotoacloud.top

[O05] 并发执行并等待全部完成
来源：http://znx.fanxiaobao.xyz

Py:   asyncio.gather(*tasks)
来源：http://hck.sufxvd.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lyf.cucudq.cn

JS:   await Promise.all(tasks)
来源：http://cgi.yfazqb.com

TS:   await Promise.all(tasks)
来源：http://wpd.meibo888.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ecj.hammf.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ptn.nwbrower.top

Ruby: threads.map(&:join)
来源：http://cwo.jinyuanbaomall.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xzd.cucudq.cn

[O06] 使用进程池
来源：http://zxp.nanxinkj.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://svm.316326.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://fkw.0kj1m.cn

JS:   // child_process / cluster 模块
来源：http://mym.sweek.top

TS:   // child_process / cluster 模块
来源：http://wes.shuidangran.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ujg.xinyue.icu

Go:   // goroutine 已占用多核，直接并发即可
来源：http://urc.zhongyouzk.top

Ruby: // fork 块
来源：http://prl.sysykeji.top

C#:   Parallel.For
来源：http://fnt.jinyuanbaomall.cn

================================================================================
来源：http://nlu.quarkkingdee.top

P. 常用工具函数
来源：http://xve.zhoulong.xyz

================================================================================
来源：http://arq.fengsongda.top

[P01] 生成 UUID
来源：http://bor.sysykeji.top

Py:   str(uuid.uuid4())
来源：http://zfc.sysykeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://amh.jianghu66.top

JS:   crypto.randomUUID()
来源：http://btc.ydjk.org.cn

TS:   crypto.randomUUID()
来源：http://epx.tian-w.cn

Java: UUID.randomUUID().toString()
来源：http://hmf.gzhubu.top

Go:   // 用 github.com/google/uuid
来源：http://tnc.fengsongda.top

Ruby: SecureRandom.uuid
来源：http://ozj.fehbvm.com

C#:   Guid.NewGuid().ToString()
来源：http://dvd.xinyue.icu

[P02] MD5 / SHA256 摘要
来源：http://fyh.yonumen.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nea.yanxiufei.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://oro.vehdjk.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vzk.fzhhl.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wdj.smart0.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nkn.andypj.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fno.bjfxy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://why.cdnleiting.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uaw.bjfxy.top

[P03] 生成短随机字符串
来源：http://gvu.9152youxi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cta.fzhhl.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zem.52xcode.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://okg.andypj.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nri.uphjek.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xyz.xuetiantiany.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ptq.aibaodan.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://dte.mhx1999.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vzl.xinyue.icu

[P04] 求长度
来源：http://rvz.shanyushiyangtech.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lda.svipenyu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ttq.yueranfly.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ykn.svipenyu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wzs.yj20258.top

Java: list.size();  map.size();  s.length()
来源：http://txz.dashuyun.cn

Go:   len(arr);  len(m)
来源：http://eei.tarul.cn

Ruby: x.length;  x.size
来源：http://ymb.cucudq.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xoc.hywenlv.cn

[P05] 判断两个对象内容是否相等
来源：http://zea.yangfankeji.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://bwi.dashuyun.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bcw.mhx1999.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://avy.yj202588.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dfq.xuanzx.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jfu.shangyingyoupin.top

Go:   reflect.DeepEqual(a, b)
来源：http://tez.daria6918.cn

Ruby: a == b
来源：http://skp.yj202588.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qdc.daria6918.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vjb.wangdashe.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jao.yvedp.cn

PHP:  if (empty($x)) {}
来源：http://trg.tarul.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qsx.vehdjk.com

TS:   if (x == null) {}
来源：http://qrz.ctjpmb.com

Java: if (x == null || x.isEmpty()) {}
来源：http://bcd.gaohongyu789.top

Go:   if x == nil {}
来源：http://alq.jinyuanbaomall.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ivb.daria6918.cn

C#:   if (x is null) {}
来源：http://ery.fanxiaobao.xyz

[P07] 防抖与节流
来源：http://imm.svipenyu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://imm.sysykeji.top

PHP:  // 手写时间戳比较
来源：http://ffz.yj20258.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wzj.yvedp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yoi.sysykeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yqi.zdbjq.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vyu.jqgfzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://skq.jinqigufen.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lsc.gotoacloud.top

[P08] 处理浮点精度问题
来源：http://voo.zhaomingkeji.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xxn.svipenyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ckl.wangdashe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vrn.guannengcc.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ddf.zhaomingkeji.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cfp.vqdsnc.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lbj.xuanzx.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bfr.cdnleiting.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dwv.havefunace.top

================================================================================
来源：http://dxo.fengsongda.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ygm.sysykeji.top

================================================================================
来源：http://pll.chenjidiqi.icu

[Q01] 创建表
来源：http://anz.aibaodan.cn

CREATE TABLE users (
来源：http://wht.jianghu66.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ucx.316326.xyz

name VARCHAR(50) NOT NULL,
来源：http://ccf.ehwqpu.com

email VARCHAR(100) UNIQUE,
来源：http://gcv.jyoumei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uvm.fehbvm.com

);
来源：http://fhx.jinqigfzy.top

[Q02] 创建带外键的表
来源：http://iqa.chenzaomai.com

CREATE TABLE orders (
来源：http://lnz.cheryme.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jqs.gzhubu.top

user_id INT NOT NULL,
来源：http://yue.gzhubu.top

amount DECIMAL(10, 2),
来源：http://wtz.dianchejie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mrq.birdmap.top

);
来源：http://dkf.snrcjt.cn

[Q03] 增加列
来源：http://znc.daria6918.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dou.ybcxt.top

[Q04] 修改列类型
来源：http://nlz.ppjwa.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nhd.yj202588.top

[Q05] 重命名列
来源：http://ojh.pycfn.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mia.316326.xyz

[Q06] 删除列
来源：http://myv.zhoulong.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://cfb.zdqjudy.top

[Q07] 删除表
来源：http://uta.snrcjt.cn

DROP TABLE IF EXISTS orders;
来源：http://set.yonumen.top

[Q08] 创建普通索引
来源：http://whb.redwolf501.top

CREATE INDEX idx_users_email ON users(email);
来源：http://cnw.nanxinkj.top

[Q09] 创建唯一索引
来源：http://akz.cheryme.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zzj.c1oappe.top

[Q10] 插入单行
来源：http://emx.0kj1m.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fwy.redwolf501.top

[Q11] 一次插入多行
来源：http://rhw.gogol.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://umf.epnwcf.com

[Q12] 插入后取自增 ID
来源：http://vwz.gotoacloud.top

INSERT INTO users (name) VALUES ('C');
来源：http://wvf.haohaochexian.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://spc.andypj.xyz

[Q13] 忽略重复插入
来源：http://djo.shanyushiyangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oms.xingfuxueyuan.xyz

[Q14] 存在则更新（upsert）
来源：http://mve.tanke756.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ulf.hysaishi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xma.xuanzx.com

[Q15] 查询全部
来源：http://goo.ivvv.top

SELECT * FROM users;
来源：http://aaa.andypj.xyz

[Q16] 查询指定列
来源：http://vis.xuanzx.com

SELECT id, name FROM users;
来源：http://ddt.yueranfly.top

[Q17] 条件查询
来源：http://kvr.jqgfzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nvh.xinyue.icu

[Q18] 模糊匹配
来源：http://fqm.cucudq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vuq.ydjk.org.cn

[Q19] 范围查询
来源：http://jvv.epnwcf.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xvc.uphjek.com

[Q20] IN 列表
来源：http://ilx.hesvh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dqk.hesvh.cn

[Q21] 空值判断
来源：http://wlg.aibaodan.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nzy.zdqjudy.top

[Q22] 排序
来源：http://vyf.fengsongda.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zvy.gotoacloud.top

[Q23] 分页
来源：http://bah.iojbl.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qgk.xylfe.cn

[Q24] 去重
来源：http://pyv.ivvv.top

SELECT DISTINCT city FROM users;
来源：http://zzg.epnwcf.com

[Q25] 只取前 N 条
来源：http://mse.sjlbkw.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yrs.sweek.top

[Q26] 计数
来源：http://ghx.daxiang520.top

SELECT COUNT(*) FROM users;
来源：http://ztu.xuanzx.com

[Q27] 条件计数
来源：http://oeq.ehwqpu.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://loi.bjfxy.top

[Q28] 求和与平均
来源：http://eff.sweek.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pti.xylfe.cn

[Q29] 最大最小值
来源：http://kif.9152youxi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lfw.jianghu66.top

[Q30] 分组统计
来源：http://fya.shuidangran.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zbn.gzhubu.top

[Q31] 分组后过滤
来源：http://dal.dianchejie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kvz.yvedp.cn

[Q32] 分组拼接字符串
来源：http://wby.ehwqpu.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://czj.dashuyun.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://unl.0kj1m.cn

[Q33] 多列分组
来源：http://ypu.tarul.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://iwg.316326.xyz

[Q34] 每组取第一条
来源：http://wrk.feifeiyinyue.top

SELECT * FROM (
来源：http://ydr.birdmap.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zrr.nanxuanxn.top

) t WHERE rn = 1;
来源：http://tdb.shanyushiyangkeji.top

[Q35] 内连接
来源：http://oop.hfpthk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nob.yvedp.cn

[Q36] 左连接
来源：http://fhu.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nva.andypj.xyz

[Q37] 右连接
来源：http://lkm.snrcjt.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lwt.zhongyouzk.top


<!-- 参考信息 -->