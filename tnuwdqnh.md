代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lls.shangyingyoupin.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://taz.hammf.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ubh.sxryk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lyg.yj20258.top

[N05] 最大公约数
来源：http://ouy.0kj1m.cn

Py:   math.gcd(a, b)
来源：http://qgn.jinqigfzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ewf.ppjwa.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jxh.xuanzx.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ocp.daria6918.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fxf.jlsjyb.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://trb.hfpthk.cn

Ruby: a.gcd(b)
来源：http://yuk.guannengcc.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tme.jinqigufen.top

[N06] 判断回文字符串
来源：http://dnj.vqdsnc.cn

Py:   s == s[::-1]
来源：http://vgk.pengpengdd.cyou

PHP:  $s === strrev($s);
来源：http://vbb.zhongyouzk.top

JS:   s === [...s].reverse().join("")
来源：http://gcv.nanxuanxn.top

TS:   s === [...s].reverse().join("")
来源：http://vck.andypj.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ban.snrcjt.cn

Go:   // 双指针从两端比较
来源：http://aam.ydzc1.top

Ruby: s == s.reverse
来源：http://mni.aibaodan.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dvi.fengsongda.top

[N07] 两数之和（返回下标）
来源：http://oci.vehdjk.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cxk.wangdashe.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xdb.pycfn.com

JS:   // 手写 Map：map.set(v, i)
来源：http://yjn.vehdjk.com

TS:   // 手写 Map<string, number>
来源：http://ela.nanxinkj.top

Java: // 手写 HashMap
来源：http://tvl.0kj1m.cn

Go:   // 手写 map[int]int
来源：http://hhr.jqgufenzy.top

Ruby: // 手写 Hash
来源：http://xqe.hnxiangtu.top

C#:   // 手写 Dictionary<int, int>
来源：http://pjp.xziqi.cn

[N08] 生成全排列
来源：http://gsr.zhixingplan.top

Py:   itertools.permutations(arr)
来源：http://gxg.fengsongda.top

PHP:  // 手写递归交换
来源：http://sth.bjfxy.top

JS:   // 手写回溯递归
来源：http://kzl.xuanzx.com

TS:   // 手写回溯递归
来源：http://nhh.ivvv.top

Java: // 手写回溯递归
来源：http://che.jinyuanbaomall.cn

Go:   // 手写回溯递归
来源：http://dnf.shuidangran.top

Ruby: arr.permutation.to_a
来源：http://rll.zhijiandao.cn

C#:   // 手写回溯递归
来源：http://hnh.yj20258.top

[N09] 栈与队列
来源：http://eqh.yj20258888.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cei.hfpthk.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://obe.tian-w.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hzz.gaohongyu789.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hqk.9152youxi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zwy.sufxvd.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ynx.redwolf501.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mur.daxiang520.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cox.jinyuanbaomall.cn

[N10] 链表节点定义
来源：http://kib.jqgufenzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vsb.jyoumei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ayb.zhixingplan.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qzg.snrcjt.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mvi.nanxuanxn.top

Java: class Node { int v; Node next; }
来源：http://lpe.hywenlv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://itr.fktsv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mim.c1oappe.top

C#:   class Node { public int V; public Node? Next; }
来源：http://rbt.gaohongyu789.top

[N11] 二叉树中序遍历
来源：http://omv.jinyuanbaomall.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://iuh.xinyue.icu

PHP:  // 手写递归函数
来源：http://ujg.xylfe.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rnp.haohaochexian.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qwp.jyoumei.cn

Java: // 手写递归
来源：http://tkz.fktsv.cn

Go:   // 手写递归
来源：http://iit.chenlongwang.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yyy.jianghu66.top

C#:   // 手写递归
来源：http://zlx.ppjwa.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://skc.chenjidiqi.icu

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nba.svipenyu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dcr.xylfe.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lws.epnwcf.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yhn.quarkkingdee.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rno.tanke756.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vqg.yueranfly.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mai.xingfuxueyuan.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wpx.yj20258888.top

================================================================================
来源：http://zag.guowangkeji.top

O. 并发与异步
来源：http://fdn.316326.xyz

================================================================================
来源：http://kli.yueranfly.top

[O01] 启动一个线程
来源：http://iak.hywenlv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ekh.fzhhl.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cye.pengpengdd.cyou

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://htp.cqqwz.cn

TS:   // 同 JS
来源：http://xwx.zdbjq.cn

Java: new Thread(() -> f()).start()
来源：http://zur.yfazqb.com

Go:   go f()
来源：http://plz.hysaishi.cn

Ruby: Thread.new { f }
来源：http://zpi.9152youxi.cn

C#:   Task.Run(() => F());
来源：http://zxr.jianghu66.top

[O02] 使用线程池
来源：http://nhw.gogol.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://znv.sxryk.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ajd.zycfv.cn

JS:   // worker_threads 线程池
来源：http://hob.ctjpmb.com

TS:   // worker_threads 线程池
来源：http://ysz.dianchejie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://neh.daria6918.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://atf.cashguo.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xrj.hysaishi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pty.fengsongda.top

[O03] 加锁保护共享数据
来源：http://oof.vehdjk.com

Py:   with lock: shared += 1
来源：http://thn.hesvh.cn

PHP:  // 用 flock() 做文件锁
来源：http://fll.xziqi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fbz.c1oappe.top

TS:   // 同 JS
来源：http://kxw.chenlongwang.top

Java: synchronized (this) { shared++; }
来源：http://oht.yonumen.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://luk.gogol.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://dgk.yuanzhike.top

C#:   lock (gate) { shared++; }
来源：http://lef.jqgufenzy.top

[O04] 定义异步函数并等待
来源：http://qer.ctjpmb.com

Py:   async def f():⏎    await g()
来源：http://mgf.guowangkeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ibr.xingfuxueyuan.xyz

JS:   async function f() { await g(); }
来源：http://uod.hysaishi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://aea.jinqigfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jkn.haohaochexian.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kbv.cashguo.top

Ruby: # 用 Fiber 或 async gem
来源：http://glq.yfazqb.com

C#:   async Task F() { await G(); }
来源：http://sqy.jlsjyb.cn

[O05] 并发执行并等待全部完成
来源：http://tyl.snrcjt.cn

Py:   asyncio.gather(*tasks)
来源：http://ovm.hywenlv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://urq.shanyushiyangkeji.top

JS:   await Promise.all(tasks)
来源：http://dip.ydzc1.top

TS:   await Promise.all(tasks)
来源：http://hdx.hnqzz.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://omh.mhx1999.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://npj.sweek.top

Ruby: threads.map(&:join)
来源：http://qdk.chenzaomai.com

C#:   await Task.WhenAll(t1, t2)
来源：http://bwl.xingfuxueyuan.xyz

[O06] 使用进程池
来源：http://cyw.sufxvd.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hle.sysykeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://irg.fanxiaobao.xyz

JS:   // child_process / cluster 模块
来源：http://wgi.hcnkem.com

TS:   // child_process / cluster 模块
来源：http://itm.0kj1m.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tdp.uphjek.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eoa.yanxiufei.cn

Ruby: // fork 块
来源：http://ubw.shzxlz.cn

C#:   Parallel.For
来源：http://txs.sysykeji.top

================================================================================
来源：http://dqd.ywan-chungtsiang.top

P. 常用工具函数
来源：http://elr.sxryk.cn

================================================================================
来源：http://rev.dianchejie.cn

[P01] 生成 UUID
来源：http://guc.ctjpmb.com

Py:   str(uuid.uuid4())
来源：http://lbj.andypj.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nfl.hongshengwenyu.top

JS:   crypto.randomUUID()
来源：http://scs.sweek.top

TS:   crypto.randomUUID()
来源：http://yjt.bjfxy.top

Java: UUID.randomUUID().toString()
来源：http://xpi.jlsjyb.cn

Go:   // 用 github.com/google/uuid
来源：http://oqx.vqdsnc.cn

Ruby: SecureRandom.uuid
来源：http://pfj.yonumen.top

C#:   Guid.NewGuid().ToString()
来源：http://uuh.bjfxy.top

[P02] MD5 / SHA256 摘要
来源：http://kio.andypj.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://etb.ywan-chungtsiang.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://adg.bbcook.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sax.gotoacloud.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qdj.shzxlz.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nmg.ydjk.org.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jqz.wangshuangyany.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://llz.bbcook.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yff.chenjidiqi.icu

[P03] 生成短随机字符串
来源：http://ihx.cucudq.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://oxh.hcnkem.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bdz.daxiang520.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ray.xylfe.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://roy.quarkkingdee.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://csm.xingfuxueyuan.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://aau.yj202588.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://aym.9152youxi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xba.svipenyu.cn

[P04] 求长度
来源：http://uob.cashguo.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://buo.sjlbkw.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jma.tanke756.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wra.jianghu66.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ulg.chenlongwang.top

Java: list.size();  map.size();  s.length()
来源：http://imj.nwbrower.top

Go:   len(arr);  len(m)
来源：http://dnk.sweek.top

Ruby: x.length;  x.size
来源：http://ior.pycfn.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://mzb.jinqigufen.top

[P05] 判断两个对象内容是否相等
来源：http://ogu.cashguo.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://dio.yj202588.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dim.pycfn.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bpf.andypj.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bcw.fanxiaobao.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://huh.hnxiangtu.top

Go:   reflect.DeepEqual(a, b)
来源：http://tye.kuanghao11.cn

Ruby: a == b
来源：http://mll.mhx1999.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qlt.aibaodan.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bti.ywan-chungtsiang.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mfx.vehdjk.com

PHP:  if (empty($x)) {}
来源：http://moe.xinyue.icu

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zjm.zhengqikj.top

TS:   if (x == null) {}
来源：http://csj.ehwqpu.com

Java: if (x == null || x.isEmpty()) {}
来源：http://tbx.hywenlv.cn

Go:   if x == nil {}
来源：http://bay.jinyuanbaomall.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fju.jyoumei.cn

C#:   if (x is null) {}
来源：http://drc.epnwcf.com

[P07] 防抖与节流
来源：http://gso.zhaomingkeji.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qeb.fanxiaobao.xyz

PHP:  // 手写时间戳比较
来源：http://ayh.ywan-chungtsiang.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hje.yfazqb.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fku.zycfv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://smb.sxryk.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tyi.9152youxi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://kae.hysaishi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pas.wangshuangyany.cn

[P08] 处理浮点精度问题
来源：http://qpm.jinyuanbaomall.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cun.yangfankeji.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lgm.haohaochexian.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hdx.shzxlz.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uqz.smart0.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://iwj.zycfv.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gqk.cdnleiting.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gjq.uphjek.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wpz.ctjpmb.com

================================================================================
来源：http://tty.hfpthk.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://izi.shzxlz.cn

================================================================================
来源：http://jcv.zhiwuduotai.top

[Q01] 创建表
来源：http://qas.ctjpmb.com

CREATE TABLE users (
来源：http://uyj.yuanzhike.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vhi.nanxinkj.top

name VARCHAR(50) NOT NULL,
来源：http://guv.sysykeji.top

email VARCHAR(100) UNIQUE,
来源：http://xzg.xinyue.icu

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://chg.0kj1m.cn

);
来源：http://oqy.fzhhl.top

[Q02] 创建带外键的表
来源：http://rdx.yangfankeji.com

CREATE TABLE orders (
来源：http://wvi.aibaodan.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yjx.yfazqb.com

user_id INT NOT NULL,
来源：http://yor.jlsjyb.cn

amount DECIMAL(10, 2),
来源：http://jcm.zdqjudy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mpm.snrcjt.cn

);
来源：http://zbd.jqgufenzy.top

[Q03] 增加列
来源：http://ogi.yfazqb.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gwm.fengsongda.top

[Q04] 修改列类型
来源：http://wtq.jinqigufen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pfr.ybcxt.top

[Q05] 重命名列
来源：http://vhn.daria6918.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yiy.quarkkingdee.top

[Q06] 删除列
来源：http://mbv.zhoulong.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://lep.zdqjudy.top

[Q07] 删除表
来源：http://igo.0kj1m.cn

DROP TABLE IF EXISTS orders;
来源：http://vad.smart0.xyz

[Q08] 创建普通索引
来源：http://fdo.ivvv.top

CREATE INDEX idx_users_email ON users(email);
来源：http://slt.guowangkeji.top

[Q09] 创建唯一索引
来源：http://ino.smart0.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zzm.gotoacloud.top

[Q10] 插入单行
来源：http://scl.nwbrower.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kdk.pycfn.com

[Q11] 一次插入多行
来源：http://oup.meibo888.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ern.jqgfzy.top

[Q12] 插入后取自增 ID
来源：http://btf.chenjidiqi.icu

INSERT INTO users (name) VALUES ('C');
来源：http://oax.yj20258.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yfi.shangyingyoupin.top

[Q13] 忽略重复插入
来源：http://vki.0kj1m.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gac.dashuyun.cn

[Q14] 存在则更新（upsert）
来源：http://jyk.havefunace.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wdo.c1oappe.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xmc.daxiang520.top

[Q15] 查询全部
来源：http://kfb.xinyue.icu

SELECT * FROM users;
来源：http://yqs.birdmap.top

[Q16] 查询指定列
来源：http://nir.ywan-chungtsiang.top

SELECT id, name FROM users;
来源：http://xte.shanyushiyangtech.top

[Q17] 条件查询
来源：http://bsf.feifeiyinyue.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://myl.hongshengwenyu.top

[Q18] 模糊匹配
来源：http://zog.yonumen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://onk.guannengcc.top

[Q19] 范围查询
来源：http://ytl.ydzc1.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ysg.yongpay.top

[Q20] IN 列表
来源：http://qtd.ctjpmb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iyp.shangyingyoupin.top

[Q21] 空值判断
来源：http://nyv.zhoulong.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://udn.yj20258888.top

[Q22] 排序
来源：http://igx.yanxiufei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mvm.52xcode.cn

[Q23] 分页
来源：http://zkc.birdmap.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gfg.andypj.xyz

[Q24] 去重
来源：http://fni.316326.xyz

SELECT DISTINCT city FROM users;
来源：http://ehk.xziqi.cn

[Q25] 只取前 N 条
来源：http://zdy.tianlin.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yqd.yfazqb.com

[Q26] 计数
来源：http://dtw.tanke756.top

SELECT COUNT(*) FROM users;
来源：http://eim.ydzc1.top

[Q27] 条件计数
来源：http://hfe.chenjidiqi.icu

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ryc.shzxlz.cn

[Q28] 求和与平均
来源：http://dgf.pengpengdd.cyou

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://edi.tanke756.top

[Q29] 最大最小值
来源：http://tgv.guowangkeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jnr.zycfv.cn

[Q30] 分组统计
来源：http://zhm.ydjk.org.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hrq.sufxvd.cn

[Q31] 分组后过滤
来源：http://iea.nanxinkj.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wha.gogol.net.cn

[Q32] 分组拼接字符串
来源：http://dne.birdmap.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zpz.smart0.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jgu.yvedp.cn

[Q33] 多列分组
来源：http://bzs.feifeiyinyue.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ans.fehbvm.com

[Q34] 每组取第一条
来源：http://cqz.52xcode.cn

SELECT * FROM (
来源：http://xxz.pycfn.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tyh.c1oappe.top

) t WHERE rn = 1;
来源：http://bwz.9152youxi.cn

[Q35] 内连接
来源：http://qhm.zhongyouzk.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tkg.chenjidiqi.icu

[Q36] 左连接
来源：http://lgx.zhijiandao.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ajf.yvedp.cn

[Q37] 右连接
来源：http://wqg.sjlbkw.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mfu.hfpthk.cn


<!-- 参考信息 -->