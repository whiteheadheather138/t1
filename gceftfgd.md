代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rbd.jianghu66.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ens.hnqzz.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://scg.dashuyun.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dyw.xziqi.cn

[N05] 最大公约数
来源：http://hvx.yueranfly.top

Py:   math.gcd(a, b)
来源：http://sdr.zhaomingkeji.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fpe.wangshuangyany.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lmj.uphjek.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cwd.vehdjk.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://feh.guowangkeji.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ser.yonumen.top

Ruby: a.gcd(b)
来源：http://mei.vqdsnc.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://iar.wangdashe.top

[N06] 判断回文字符串
来源：http://lic.shanyushiyangkeji.top

Py:   s == s[::-1]
来源：http://zts.yj20258.top

PHP:  $s === strrev($s);
来源：http://xai.cdnleiting.top

JS:   s === [...s].reverse().join("")
来源：http://baz.ppjwa.cn

TS:   s === [...s].reverse().join("")
来源：http://qpb.0kj1m.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zqa.gaohongyu789.top

Go:   // 双指针从两端比较
来源：http://vsh.xziqi.cn

Ruby: s == s.reverse
来源：http://ezu.hysaishi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mak.jianghu66.top

[N07] 两数之和（返回下标）
来源：http://nkk.ctjpmb.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vww.ydzc1.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ngg.jinqigfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://rqu.xinyue.icu

TS:   // 手写 Map<string, number>
来源：http://omc.cdnleiting.top

Java: // 手写 HashMap
来源：http://jmh.fanxiaobao.xyz

Go:   // 手写 map[int]int
来源：http://yro.pycfn.com

Ruby: // 手写 Hash
来源：http://rpn.ybcxt.top

C#:   // 手写 Dictionary<int, int>
来源：http://acl.bjfxy.top

[N08] 生成全排列
来源：http://abl.zhengqikj.top

Py:   itertools.permutations(arr)
来源：http://tok.yangfankeji.com

PHP:  // 手写递归交换
来源：http://ylg.daria6918.cn

JS:   // 手写回溯递归
来源：http://cpc.ehwqpu.com

TS:   // 手写回溯递归
来源：http://hbd.haohaochexian.top

Java: // 手写回溯递归
来源：http://efd.hysaishi.cn

Go:   // 手写回溯递归
来源：http://tog.tanke756.top

Ruby: arr.permutation.to_a
来源：http://rgu.ydzc1.top

C#:   // 手写回溯递归
来源：http://cbx.jqgfzy.top

[N09] 栈与队列
来源：http://som.zhiwuduotai.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://chr.ydjk.org.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://utq.yanxiufei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jho.daria6918.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ayc.hongshengwenyu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xas.ybcxt.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yef.mhx1999.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kum.yj20258.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://izz.andypj.xyz

[N10] 链表节点定义
来源：http://yyr.birdmap.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cau.chenzaomai.com

PHP:  class Node { public $v; public $next = null; }
来源：http://rdo.sysykeji.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wyk.hfpthk.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dca.tianlin.xyz

Java: class Node { int v; Node next; }
来源：http://egg.zhongyouzk.top

Go:   type Node struct { V int; Next *Node }
来源：http://gtw.52xcode.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lqy.uphjek.com

C#:   class Node { public int V; public Node? Next; }
来源：http://dpf.xuetiantiany.cn

[N11] 二叉树中序遍历
来源：http://gpc.gogol.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sgz.yvedp.cn

PHP:  // 手写递归函数
来源：http://abp.vehdjk.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vzf.hfpthk.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gds.cqqwz.cn

Java: // 手写递归
来源：http://mky.bbcook.cn

Go:   // 手写递归
来源：http://glm.hesvh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wyi.dashuyun.cn

C#:   // 手写递归
来源：http://lrb.xuetiantiany.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xlg.hcnkem.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nac.zhiwuduotai.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zyc.hnqzz.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ika.chenlongwang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gfw.shuidangran.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uih.chenlongwang.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hxf.yonumen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hyw.xuetiantiany.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://apk.jinqigufen.top

================================================================================
来源：http://ctt.wangshuangyany.cn

O. 并发与异步
来源：http://skz.tian-w.cn

================================================================================
来源：http://tkb.zdbjq.cn

[O01] 启动一个线程
来源：http://zqw.xziqi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kqj.havefunace.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nyf.shangyingyoupin.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://eio.sxryk.cn

TS:   // 同 JS
来源：http://zji.yuxming.cn

Java: new Thread(() -> f()).start()
来源：http://agv.vehdjk.com

Go:   go f()
来源：http://esp.daxiang520.top

Ruby: Thread.new { f }
来源：http://gth.xuetiantiany.cn

C#:   Task.Run(() => F());
来源：http://wrm.yvedp.cn

[O02] 使用线程池
来源：http://trg.gzhubu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cbn.yvedp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dho.zhoulong.xyz

JS:   // worker_threads 线程池
来源：http://ccl.gogol.net.cn

TS:   // worker_threads 线程池
来源：http://ips.jqgfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://wob.jinqigufen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nim.jiagoushi.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vtt.cheryme.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bbx.xuetiantiany.cn

[O03] 加锁保护共享数据
来源：http://bqy.jyoumei.cn

Py:   with lock: shared += 1
来源：http://sok.fanxiaobao.xyz

PHP:  // 用 flock() 做文件锁
来源：http://jub.hcnkem.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uju.redwolf501.top

TS:   // 同 JS
来源：http://uii.ybcxt.top

Java: synchronized (this) { shared++; }
来源：http://ngs.mhx1999.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vji.vqdsnc.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://evr.nanxuanxn.top

C#:   lock (gate) { shared++; }
来源：http://rjj.fktsv.cn

[O04] 定义异步函数并等待
来源：http://dlx.pycfn.com

Py:   async def f():⏎    await g()
来源：http://hop.vqdsnc.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hgp.guannengcc.top

JS:   async function f() { await g(); }
来源：http://hmu.jqgufenzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://btg.jyoumei.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hfg.jlsjyb.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sbz.yfazqb.com

Ruby: # 用 Fiber 或 async gem
来源：http://wcg.hesvh.cn

C#:   async Task F() { await G(); }
来源：http://qux.sxryk.cn

[O05] 并发执行并等待全部完成
来源：http://pxw.c1oappe.top

Py:   asyncio.gather(*tasks)
来源：http://yvg.yangfankeji.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yaq.tarul.cn

JS:   await Promise.all(tasks)
来源：http://sne.ivvv.top

TS:   await Promise.all(tasks)
来源：http://rvn.havefunace.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hkb.dianchejie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://csk.bbcook.cn

Ruby: threads.map(&:join)
来源：http://daq.sjlbkw.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ntf.cdnleiting.top

[O06] 使用进程池
来源：http://yji.tarul.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mdt.wangshuangyany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ugb.tanke756.top

JS:   // child_process / cluster 模块
来源：http://itf.hywenlv.cn

TS:   // child_process / cluster 模块
来源：http://orp.316326.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vqo.quarkkingdee.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cli.ctjpmb.com

Ruby: // fork 块
来源：http://xqm.cdnleiting.top

C#:   Parallel.For
来源：http://sbq.yangfankeji.com

================================================================================
来源：http://qyu.zhijiandao.cn

P. 常用工具函数
来源：http://wyo.chenlongwang.top

================================================================================
来源：http://dwl.shanyushiyangkeji.top

[P01] 生成 UUID
来源：http://cok.chenzaomai.com

Py:   str(uuid.uuid4())
来源：http://xcg.vqdsnc.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zau.cucudq.cn

JS:   crypto.randomUUID()
来源：http://tyu.jinyuanbaomall.cn

TS:   crypto.randomUUID()
来源：http://lxy.c1oappe.top

Java: UUID.randomUUID().toString()
来源：http://nmh.pycfn.com

Go:   // 用 github.com/google/uuid
来源：http://tcj.ctjpmb.com

Ruby: SecureRandom.uuid
来源：http://fev.gzhubu.top

C#:   Guid.NewGuid().ToString()
来源：http://hlj.birdmap.top

[P02] MD5 / SHA256 摘要
来源：http://yld.0kj1m.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://eeb.tian-w.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nob.tarul.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ljb.zhoulong.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sgk.xuanzx.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lzq.sufxvd.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://igw.jlsjyb.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wsq.jyoumei.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://taf.shangyingyoupin.top

[P03] 生成短随机字符串
来源：http://tsq.gaohongyu789.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bvo.jqgufenzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vjm.shangyingyoupin.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qjr.ppjwa.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fvh.redwolf501.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gfd.kuanghao11.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nul.nanxinkj.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://clh.sufxvd.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ncc.redwolf501.top

[P04] 求长度
来源：http://zrt.dashuyun.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jtl.hesvh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wdu.havefunace.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zyn.sjlbkw.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gzn.wangshuangyany.cn

Java: list.size();  map.size();  s.length()
来源：http://pld.xinyue.icu

Go:   len(arr);  len(m)
来源：http://xzj.yj20258888.top

Ruby: x.length;  x.size
来源：http://ebf.cheryme.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gxu.jinghuilouyu.cn

[P05] 判断两个对象内容是否相等
来源：http://ufl.cqqwz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sqk.jinghuilouyu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lko.meibo888.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pbj.zhaomingkeji.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fxf.zhaomingkeji.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dwq.chenzaomai.com

Go:   reflect.DeepEqual(a, b)
来源：http://tus.ppjwa.cn

Ruby: a == b
来源：http://oww.tian-w.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vew.yuanzhike.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hnq.ppjwa.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cyp.hysaishi.cn

PHP:  if (empty($x)) {}
来源：http://oze.sysykeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wrl.dianchejie.cn

TS:   if (x == null) {}
来源：http://uuk.fehbvm.com

Java: if (x == null || x.isEmpty()) {}
来源：http://eov.aibaodan.cn

Go:   if x == nil {}
来源：http://noe.andypj.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kjl.hnxiangtu.top

C#:   if (x is null) {}
来源：http://ttm.tianlin.xyz

[P07] 防抖与节流
来源：http://baw.ppjwa.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://afq.ywan-chungtsiang.top

PHP:  // 手写时间戳比较
来源：http://hkg.cashguo.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ruk.tianlin.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wsf.zdqjudy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ywc.shanyushiyangtech.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cvw.yanxiufei.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pkd.sysykeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kef.shuidangran.top

[P08] 处理浮点精度问题
来源：http://fxf.yj202588.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rht.fehbvm.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ifv.tianlin.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wlz.ppjwa.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://eus.cheryme.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ylw.jinqigufen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zaw.c1oappe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ywg.hnqzz.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ohn.bjfxy.top

================================================================================
来源：http://wlj.meibo888.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://inj.jlsjyb.cn

================================================================================
来源：http://eft.guannengcc.top

[Q01] 创建表
来源：http://lnj.hcnkem.com

CREATE TABLE users (
来源：http://eow.jyoumei.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mzl.hnqzz.top

name VARCHAR(50) NOT NULL,
来源：http://txc.feifeiyinyue.top

email VARCHAR(100) UNIQUE,
来源：http://sjc.xuanzx.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://htb.dashuyun.cn

);
来源：http://wrn.pycfn.com

[Q02] 创建带外键的表
来源：http://bef.sysykeji.top

CREATE TABLE orders (
来源：http://zln.yongpay.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oxk.yj202588.top

user_id INT NOT NULL,
来源：http://qxv.nanxuanxn.top

amount DECIMAL(10, 2),
来源：http://fgt.wangdashe.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bas.hongshengwenyu.top

);
来源：http://zsw.hcnkem.com

[Q03] 增加列
来源：http://tmr.jyoumei.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qvw.jianghu66.top

[Q04] 修改列类型
来源：http://ekl.jinqigufen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lxz.meibo888.top

[Q05] 重命名列
来源：http://faf.zycfv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vzo.fengsongda.top

[Q06] 删除列
来源：http://byb.hfpthk.cn

ALTER TABLE users DROP COLUMN age;
来源：http://hwv.hammf.cn

[Q07] 删除表
来源：http://ojm.sweek.top

DROP TABLE IF EXISTS orders;
来源：http://wkz.0kj1m.cn

[Q08] 创建普通索引
来源：http://agv.epnwcf.com

CREATE INDEX idx_users_email ON users(email);
来源：http://eeu.sufxvd.cn

[Q09] 创建唯一索引
来源：http://vqa.yvedp.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fzs.xingfuxueyuan.xyz

[Q10] 插入单行
来源：http://jbb.shangyingyoupin.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wks.yj20258888.top

[Q11] 一次插入多行
来源：http://vgq.xylfe.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qjb.ppjwa.cn

[Q12] 插入后取自增 ID
来源：http://ovr.fktsv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pkw.hfpthk.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dee.zhengqikj.top

[Q13] 忽略重复插入
来源：http://rws.nanxuanxn.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xxk.jqgufenzy.top

[Q14] 存在则更新（upsert）
来源：http://ook.zdbjq.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zlb.pengpengdd.cyou

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qnt.andypj.xyz

[Q15] 查询全部
来源：http://pck.yj20258.top

SELECT * FROM users;
来源：http://jpy.aibaodan.cn

[Q16] 查询指定列
来源：http://pir.hongshengwenyu.top

SELECT id, name FROM users;
来源：http://obq.bjfxy.top

[Q17] 条件查询
来源：http://tzj.316326.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ubd.zhiwuduotai.top

[Q18] 模糊匹配
来源：http://kpv.aibaodan.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cmf.fzhhl.top

[Q19] 范围查询
来源：http://ahn.jqgfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ddx.ydjk.org.cn

[Q20] IN 列表
来源：http://fkb.jinqigufen.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zvk.vehdjk.com

[Q21] 空值判断
来源：http://eae.yuanzhike.top

SELECT * FROM users WHERE email IS NULL;
来源：http://cjy.pengpengdd.cyou

[Q22] 排序
来源：http://itu.sjlbkw.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ppp.zdbjq.cn

[Q23] 分页
来源：http://pxk.hcnkem.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://iub.yongpay.top

[Q24] 去重
来源：http://huq.wangdashe.top

SELECT DISTINCT city FROM users;
来源：http://pyn.haohaochexian.top

[Q25] 只取前 N 条
来源：http://irt.ehwqpu.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yry.ppjwa.cn

[Q26] 计数
来源：http://qos.jlsjyb.cn

SELECT COUNT(*) FROM users;
来源：http://jev.zhongyouzk.top

[Q27] 条件计数
来源：http://piu.sufxvd.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://scw.yj20258888.top

[Q28] 求和与平均
来源：http://wud.nanxinkj.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qoq.vqdsnc.cn

[Q29] 最大最小值
来源：http://yud.cheryme.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://lyc.dashuyun.cn

[Q30] 分组统计
来源：http://dqx.ydzc1.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nfa.uphjek.com

[Q31] 分组后过滤
来源：http://vei.gzhubu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mag.hesvh.cn

[Q32] 分组拼接字符串
来源：http://gfo.dianchejie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vjf.sxryk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hci.zycfv.cn

[Q33] 多列分组
来源：http://bjc.zhixingplan.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uta.yfazqb.com

[Q34] 每组取第一条
来源：http://nos.iojbl.cn

SELECT * FROM (
来源：http://agy.zhaomingkeji.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bap.svipenyu.cn

) t WHERE rn = 1;
来源：http://fbh.zhongyouzk.top

[Q35] 内连接
来源：http://snl.shuidangran.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cmk.jqgfzy.top

[Q36] 左连接
来源：http://xlj.jqgufenzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bem.yvedp.cn

[Q37] 右连接
来源：http://xae.birdmap.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://czj.shuidangran.top


<!-- 参考信息 -->