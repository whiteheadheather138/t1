代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://knd.jinqigufen.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xbd.yuxming.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://esy.zdqjudy.top

Ruby: a.gcd(b)
来源：http://ajl.sufxvd.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nst.yj202588.top

[N06] 判断回文字符串
来源：http://exg.yuanzhike.top

Py:   s == s[::-1]
来源：http://nia.wangshuangyany.cn

PHP:  $s === strrev($s);
来源：http://czq.jlsjyb.cn

JS:   s === [...s].reverse().join("")
来源：http://hzx.xuetiantiany.cn

TS:   s === [...s].reverse().join("")
来源：http://eff.vehdjk.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oqb.chenlongwang.top

Go:   // 双指针从两端比较
来源：http://cbp.tarul.cn

Ruby: s == s.reverse
来源：http://nve.daria6918.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wyr.bbcook.cn

[N07] 两数之和（返回下标）
来源：http://ocf.vqdsnc.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://beo.yangfankeji.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jbd.c1oappe.top

JS:   // 手写 Map：map.set(v, i)
来源：http://amj.vqdsnc.cn

TS:   // 手写 Map<string, number>
来源：http://akt.xziqi.cn

Java: // 手写 HashMap
来源：http://hie.chenzaomai.com

Go:   // 手写 map[int]int
来源：http://zah.uphjek.com

Ruby: // 手写 Hash
来源：http://qsc.gotoacloud.top

C#:   // 手写 Dictionary<int, int>
来源：http://mjc.jinqigfzy.top

[N08] 生成全排列
来源：http://bak.jinghuilouyu.cn

Py:   itertools.permutations(arr)
来源：http://xpa.tarul.cn

PHP:  // 手写递归交换
来源：http://fhh.zycfv.cn

JS:   // 手写回溯递归
来源：http://glv.vqdsnc.cn

TS:   // 手写回溯递归
来源：http://cls.iojbl.cn

Java: // 手写回溯递归
来源：http://hcn.0kj1m.cn

Go:   // 手写回溯递归
来源：http://gyb.nanxinkj.top

Ruby: arr.permutation.to_a
来源：http://bsi.jiagoushi.top

C#:   // 手写回溯递归
来源：http://usj.shanyushiyangtech.top

[N09] 栈与队列
来源：http://idn.yfazqb.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vwx.cdnleiting.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mct.snrcjt.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lje.havefunace.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dlf.fzhhl.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bwm.yanxiufei.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ofj.nanxuanxn.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zwu.xuanzx.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kup.yueranfly.top

[N10] 链表节点定义
来源：http://wkv.cashguo.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jmx.0kj1m.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gvk.hnxiangtu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pas.tian-w.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nhh.jinqigufen.top

Java: class Node { int v; Node next; }
来源：http://xva.hammf.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zlq.hnqzz.top

Ruby: Node = Struct.new(:v, :next)
来源：http://dtq.yueranfly.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ppt.yvedp.cn

[N11] 二叉树中序遍历
来源：http://dzd.hcnkem.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ugw.gaohongyu789.top

PHP:  // 手写递归函数
来源：http://qcr.xylfe.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fls.smart0.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lwz.chenjidiqi.icu

Java: // 手写递归
来源：http://evn.yongpay.top

Go:   // 手写递归
来源：http://ena.jinqigufen.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://iqa.xingfuxueyuan.xyz

C#:   // 手写递归
来源：http://jwz.svipenyu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jiu.xuetiantiany.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://snb.dianchejie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ixe.sxryk.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gbo.zhaomingkeji.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fvy.zdbjq.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zdq.gzhubu.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lnr.hysaishi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zts.yuanzhike.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wty.hysaishi.cn

================================================================================
来源：http://lbo.havefunace.top

O. 并发与异步
来源：http://mpi.dianchejie.cn

================================================================================
来源：http://gee.hongshengwenyu.top

[O01] 启动一个线程
来源：http://ylo.ydjk.org.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jzz.wangdashe.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://chi.jinghuilouyu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qhw.sxryk.cn

TS:   // 同 JS
来源：http://pwm.cheryme.top

Java: new Thread(() -> f()).start()
来源：http://wxq.zycfv.cn

Go:   go f()
来源：http://uyx.9152youxi.cn

Ruby: Thread.new { f }
来源：http://fob.shuidangran.top

C#:   Task.Run(() => F());
来源：http://ujg.kuanghao11.cn

[O02] 使用线程池
来源：http://ham.52xcode.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oic.smart0.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zvk.jqgufenzy.top

JS:   // worker_threads 线程池
来源：http://oiq.yvedp.cn

TS:   // worker_threads 线程池
来源：http://zge.sweek.top

Java: Executors.newFixedThreadPool(4)
来源：http://ctx.jinqigfzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jkq.bjfxy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cik.tarul.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gst.aizwys.cn

[O03] 加锁保护共享数据
来源：http://fwn.kuanghao11.cn

Py:   with lock: shared += 1
来源：http://rzd.nanxuanxn.top

PHP:  // 用 flock() 做文件锁
来源：http://ybv.hnqzz.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sqo.gogol.net.cn

TS:   // 同 JS
来源：http://eei.daria6918.cn

Java: synchronized (this) { shared++; }
来源：http://ghf.zhoulong.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ahd.dashuyun.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tzo.jqgfzy.top

C#:   lock (gate) { shared++; }
来源：http://nmm.shanyushiyangkeji.top

[O04] 定义异步函数并等待
来源：http://vnx.sufxvd.cn

Py:   async def f():⏎    await g()
来源：http://gmh.yanxiufei.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rjb.gogol.net.cn

JS:   async function f() { await g(); }
来源：http://wrp.hysaishi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hvm.shanyushiyangtech.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nfi.ppjwa.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uzl.jinyuanbaomall.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jgg.fehbvm.com

C#:   async Task F() { await G(); }
来源：http://axr.epnwcf.com

[O05] 并发执行并等待全部完成
来源：http://ktp.hnxiangtu.top

Py:   asyncio.gather(*tasks)
来源：http://obw.jianghu66.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dbq.cucudq.cn

JS:   await Promise.all(tasks)
来源：http://vqc.snrcjt.cn

TS:   await Promise.all(tasks)
来源：http://bfi.nwbrower.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cjf.vehdjk.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gih.chenlongwang.top

Ruby: threads.map(&:join)
来源：http://tph.fengsongda.top

C#:   await Task.WhenAll(t1, t2)
来源：http://htj.yangfankeji.com

[O06] 使用进程池
来源：http://asc.ctjpmb.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mwn.feifeiyinyue.top

PHP:  // pcntl_fork 或多进程队列
来源：http://dlj.hnqzz.top

JS:   // child_process / cluster 模块
来源：http://dnv.wangshuangyany.cn

TS:   // child_process / cluster 模块
来源：http://ebd.aizwys.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gsv.gogol.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vux.xziqi.cn

Ruby: // fork 块
来源：http://uko.fktsv.cn

C#:   Parallel.For
来源：http://map.tarul.cn

================================================================================
来源：http://dmz.jqgufenzy.top

P. 常用工具函数
来源：http://jgd.hysaishi.cn

================================================================================
来源：http://afx.svipenyu.cn

[P01] 生成 UUID
来源：http://tdj.nanxuanxn.top

Py:   str(uuid.uuid4())
来源：http://jlk.zhaomingkeji.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dmk.sufxvd.cn

JS:   crypto.randomUUID()
来源：http://bef.sxryk.cn

TS:   crypto.randomUUID()
来源：http://rbu.hesvh.cn

Java: UUID.randomUUID().toString()
来源：http://hqw.ctjpmb.com

Go:   // 用 github.com/google/uuid
来源：http://wjj.yj202588.top

Ruby: SecureRandom.uuid
来源：http://ntq.jianghu66.top

C#:   Guid.NewGuid().ToString()
来源：http://xoq.cheryme.top

[P02] MD5 / SHA256 摘要
来源：http://rud.pycfn.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://aqn.jinqigufen.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wfl.xuanzx.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://znx.daxiang520.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lvc.ppjwa.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://foh.ybcxt.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cks.ehwqpu.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qgh.ywan-chungtsiang.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qok.kuanghao11.cn

[P03] 生成短随机字符串
来源：http://dqu.hfpthk.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qpf.vqdsnc.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://roz.yfazqb.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nwe.fanxiaobao.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zbf.zdqjudy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ihg.hesvh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fcj.zhijiandao.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cbr.jqgufenzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qfn.sxryk.cn

[P04] 求长度
来源：http://bmw.nanxuanxn.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://erv.zhaomingkeji.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jyx.daxiang520.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gpk.yj20258888.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://coq.hcnkem.com

Java: list.size();  map.size();  s.length()
来源：http://owm.bbcook.cn

Go:   len(arr);  len(m)
来源：http://rnq.shanyushiyangkeji.top

Ruby: x.length;  x.size
来源：http://twz.shangyingyoupin.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jfv.yj20258888.top

[P05] 判断两个对象内容是否相等
来源：http://hto.c1oappe.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://eeh.ywan-chungtsiang.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bkh.sweek.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dnn.cheryme.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://plo.yueranfly.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://crt.bjfxy.top

Go:   reflect.DeepEqual(a, b)
来源：http://nob.nwbrower.top

Ruby: a == b
来源：http://dsx.andypj.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://itg.quarkkingdee.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://idd.yuanzhike.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://woc.sjlbkw.cn

PHP:  if (empty($x)) {}
来源：http://ypt.yfazqb.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hsq.birdmap.top

TS:   if (x == null) {}
来源：http://tuw.bbcook.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lbt.cashguo.top

Go:   if x == nil {}
来源：http://laj.hnxiangtu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lre.jinqigufen.top

C#:   if (x is null) {}
来源：http://uar.316326.xyz

[P07] 防抖与节流
来源：http://ukz.yueranfly.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rvq.shangyingyoupin.top

PHP:  // 手写时间戳比较
来源：http://obj.jinqigufen.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xbo.sjlbkw.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bsj.jinqigufen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://aaw.yonumen.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cft.ydzc1.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://brv.jianghu66.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wgx.snrcjt.cn

[P08] 处理浮点精度问题
来源：http://aqz.sxryk.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ioa.zdbjq.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fgu.chenjidiqi.icu

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kaq.yvedp.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vyb.xinyue.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kqj.hnqzz.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xrj.epnwcf.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pdf.andypj.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ppq.yonumen.top

================================================================================
来源：http://zsu.xuanzx.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gzk.xinyue.icu

================================================================================
来源：http://vhq.shzxlz.cn

[Q01] 创建表
来源：http://you.aizwys.cn

CREATE TABLE users (
来源：http://fik.cdnleiting.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xdm.jinqigfzy.top

name VARCHAR(50) NOT NULL,
来源：http://nlk.ydjk.org.cn

email VARCHAR(100) UNIQUE,
来源：http://lag.guowangkeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pkk.xziqi.cn

);
来源：http://tqq.sxryk.cn

[Q02] 创建带外键的表
来源：http://cmk.epnwcf.com

CREATE TABLE orders (
来源：http://ibk.fzhhl.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wkh.hcnkem.com

user_id INT NOT NULL,
来源：http://nog.jianghu66.top

amount DECIMAL(10, 2),
来源：http://bkf.yonumen.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gpk.tianlin.xyz

);
来源：http://hts.ppjwa.cn

[Q03] 增加列
来源：http://scv.gotoacloud.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dvy.jqgufenzy.top

[Q04] 修改列类型
来源：http://tol.zdqjudy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xqt.ywan-chungtsiang.top

[Q05] 重命名列
来源：http://rft.zhaomingkeji.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rlq.zhiwuduotai.top

[Q06] 删除列
来源：http://hmv.wangshuangyany.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qst.quarkkingdee.top

[Q07] 删除表
来源：http://yry.zhengqikj.top

DROP TABLE IF EXISTS orders;
来源：http://jpt.fktsv.cn

[Q08] 创建普通索引
来源：http://hwa.iojbl.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://muv.sweek.top

[Q09] 创建唯一索引
来源：http://rzt.kuanghao11.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vsc.52xcode.cn

[Q10] 插入单行
来源：http://nmb.wangdashe.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qrw.ydzc1.top

[Q11] 一次插入多行
来源：http://rpq.nanxuanxn.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://eeh.hongshengwenyu.top

[Q12] 插入后取自增 ID
来源：http://nsk.andypj.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://juw.chenlongwang.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://twk.jqgfzy.top

[Q13] 忽略重复插入
来源：http://bjo.svipenyu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fst.yvedp.cn

[Q14] 存在则更新（upsert）
来源：http://roa.zhixingplan.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ogg.zhengqikj.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jpz.zhengqikj.top

[Q15] 查询全部
来源：http://hyv.gzhubu.top

SELECT * FROM users;
来源：http://mlg.xuanzx.com

[Q16] 查询指定列
来源：http://kmn.zhijiandao.cn

SELECT id, name FROM users;
来源：http://ovw.hfpthk.cn

[Q17] 条件查询
来源：http://fpo.fehbvm.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rwi.fanxiaobao.xyz

[Q18] 模糊匹配
来源：http://ojn.pycfn.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://riy.xuetiantiany.cn

[Q19] 范围查询
来源：http://vaa.yj20258888.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://eza.shanyushiyangkeji.top

[Q20] IN 列表
来源：http://puk.zycfv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sdl.jiagoushi.top

[Q21] 空值判断
来源：http://bic.sufxvd.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ppp.xuetiantiany.cn

[Q22] 排序
来源：http://fcp.sxryk.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mpv.cdnleiting.top

[Q23] 分页
来源：http://skj.chenlongwang.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xqh.redwolf501.top

[Q24] 去重
来源：http://ylp.redwolf501.top

SELECT DISTINCT city FROM users;
来源：http://auk.xuanzx.com

[Q25] 只取前 N 条
来源：http://hxh.yueranfly.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ssr.epnwcf.com

[Q26] 计数
来源：http://urr.ydzc1.top

SELECT COUNT(*) FROM users;
来源：http://lci.sufxvd.cn

[Q27] 条件计数
来源：http://mbf.shanyushiyangkeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kfi.cdnleiting.top

[Q28] 求和与平均
来源：http://pca.hnxiangtu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://izx.jqgfzy.top

[Q29] 最大最小值
来源：http://gsl.gaohongyu789.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://tuu.yj20258888.top

[Q30] 分组统计
来源：http://zvp.fzhhl.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bgb.bbcook.cn

[Q31] 分组后过滤
来源：http://sxx.vehdjk.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cud.nanxuanxn.top

[Q32] 分组拼接字符串
来源：http://qwt.jinyuanbaomall.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://shz.yuxming.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tgl.gotoacloud.top

[Q33] 多列分组
来源：http://rlb.fehbvm.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://alu.jqgfzy.top

[Q34] 每组取第一条
来源：http://iiz.ywan-chungtsiang.top

SELECT * FROM (
来源：http://ojj.hywenlv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hyh.jqgufenzy.top

) t WHERE rn = 1;
来源：http://eam.yuanzhike.top

[Q35] 内连接
来源：http://aya.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uuu.chenjidiqi.icu

[Q36] 左连接
来源：http://xfl.sweek.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mqx.tarul.cn

[Q37] 右连接
来源：http://iof.sysykeji.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hjn.snrcjt.cn

[Q38] 全外连接（PostgreSQL）
来源：http://cep.shzxlz.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xel.snrcjt.cn

[Q39] 自连接（查上下级）
来源：http://oal.fengsongda.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://sdb.feifeiyinyue.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qvl.ydzc1.top

[Q40] 交叉连接（笛卡尔积）
来源：http://oal.yfazqb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lhs.xinyue.icu

[Q41] 多表连接
来源：http://ryf.jianghu66.top


<!-- 参考信息 -->