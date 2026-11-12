代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dmv.chenjidiqi.icu

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ytv.ppjwa.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bak.daria6918.cn

Ruby: a.gcd(b)
来源：http://ajb.kuanghao11.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fxe.hongshengwenyu.top

[N06] 判断回文字符串
来源：http://wvh.yanxiufei.cn

Py:   s == s[::-1]
来源：http://oce.pengpengdd.cyou

PHP:  $s === strrev($s);
来源：http://whe.yj20258.top

JS:   s === [...s].reverse().join("")
来源：http://hwu.ywan-chungtsiang.top

TS:   s === [...s].reverse().join("")
来源：http://zyb.tianlin.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://knk.hywenlv.cn

Go:   // 双指针从两端比较
来源：http://ggm.0kj1m.cn

Ruby: s == s.reverse
来源：http://xxw.cucudq.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hty.xylfe.cn

[N07] 两数之和（返回下标）
来源：http://mfh.xylfe.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sjo.hysaishi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yxl.hysaishi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zlg.jinyuanbaomall.cn

TS:   // 手写 Map<string, number>
来源：http://rje.hongshengwenyu.top

Java: // 手写 HashMap
来源：http://xnz.yonumen.top

Go:   // 手写 map[int]int
来源：http://com.shangyingyoupin.top

Ruby: // 手写 Hash
来源：http://tde.sweek.top

C#:   // 手写 Dictionary<int, int>
来源：http://nmj.316326.xyz

[N08] 生成全排列
来源：http://kkj.jqgufenzy.top

Py:   itertools.permutations(arr)
来源：http://ocq.tian-w.cn

PHP:  // 手写递归交换
来源：http://tyv.hesvh.cn

JS:   // 手写回溯递归
来源：http://kgz.nanxinkj.top

TS:   // 手写回溯递归
来源：http://esx.tianlin.xyz

Java: // 手写回溯递归
来源：http://oeg.jiagoushi.top

Go:   // 手写回溯递归
来源：http://riy.gogol.net.cn

Ruby: arr.permutation.to_a
来源：http://yed.chenzaomai.com

C#:   // 手写回溯递归
来源：http://csj.yfazqb.com

[N09] 栈与队列
来源：http://zno.aibaodan.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wjc.zhengqikj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wvq.hywenlv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yef.chenlongwang.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://odj.yfazqb.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mwk.dianchejie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nzc.havefunace.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cgo.ctjpmb.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://alj.havefunace.top

[N10] 链表节点定义
来源：http://wtz.yanxiufei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ddb.quarkkingdee.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vnv.ehwqpu.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://noe.chenlongwang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fzi.hesvh.cn

Java: class Node { int v; Node next; }
来源：http://hwx.jqgufenzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://rlj.bbcook.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sch.aibaodan.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lav.pengpengdd.cyou

[N11] 二叉树中序遍历
来源：http://ozv.smart0.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ovp.tarul.cn

PHP:  // 手写递归函数
来源：http://apm.hfpthk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wbv.yfazqb.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qcd.zhoulong.xyz

Java: // 手写递归
来源：http://blv.chenzaomai.com

Go:   // 手写递归
来源：http://fau.yangfankeji.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ebb.pengpengdd.cyou

C#:   // 手写递归
来源：http://xis.fzhhl.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://enx.hfpthk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wwz.zhiwuduotai.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ecs.hesvh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nbj.yueranfly.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iqm.birdmap.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uuh.yj20258.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://psq.fengsongda.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ukb.jiagoushi.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kqv.jqgufenzy.top

================================================================================
来源：http://kmx.snrcjt.cn

O. 并发与异步
来源：http://pgd.pycfn.com

================================================================================
来源：http://oqa.daxiang520.top

[O01] 启动一个线程
来源：http://vrq.yvedp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mpp.jinqigufen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wyv.gaohongyu789.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kaa.tarul.cn

TS:   // 同 JS
来源：http://xsg.yj20258888.top

Java: new Thread(() -> f()).start()
来源：http://flt.hesvh.cn

Go:   go f()
来源：http://ykj.jinghuilouyu.cn

Ruby: Thread.new { f }
来源：http://ynf.quarkkingdee.top

C#:   Task.Run(() => F());
来源：http://mqs.shanyushiyangkeji.top

[O02] 使用线程池
来源：http://cng.xziqi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fgc.shuidangran.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pmw.shanyushiyangkeji.top

JS:   // worker_threads 线程池
来源：http://sms.meibo888.top

TS:   // worker_threads 线程池
来源：http://loa.yvedp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ido.jiagoushi.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xww.gzhubu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nza.tian-w.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gru.aizwys.cn

[O03] 加锁保护共享数据
来源：http://qjn.birdmap.top

Py:   with lock: shared += 1
来源：http://xfu.yanxiufei.cn

PHP:  // 用 flock() 做文件锁
来源：http://eqz.hammf.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zvm.yueranfly.top

TS:   // 同 JS
来源：http://waf.snrcjt.cn

Java: synchronized (this) { shared++; }
来源：http://wny.smart0.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zzr.hfpthk.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bbr.pengpengdd.cyou

C#:   lock (gate) { shared++; }
来源：http://rgs.iojbl.cn

[O04] 定义异步函数并等待
来源：http://afu.vehdjk.com

Py:   async def f():⏎    await g()
来源：http://toa.ywan-chungtsiang.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jkv.jyoumei.cn

JS:   async function f() { await g(); }
来源：http://mqj.dianchejie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://new.zhongyouzk.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ihf.zdqjudy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://crr.iojbl.cn

Ruby: # 用 Fiber 或 async gem
来源：http://yzr.fanxiaobao.xyz

C#:   async Task F() { await G(); }
来源：http://smm.zycfv.cn

[O05] 并发执行并等待全部完成
来源：http://kmq.nanxinkj.top

Py:   asyncio.gather(*tasks)
来源：http://dgo.cashguo.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cgp.hnxiangtu.top

JS:   await Promise.all(tasks)
来源：http://rux.kuanghao11.cn

TS:   await Promise.all(tasks)
来源：http://zws.bjfxy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cme.pycfn.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nav.shzxlz.cn

Ruby: threads.map(&:join)
来源：http://gmh.sufxvd.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qbs.gotoacloud.top

[O06] 使用进程池
来源：http://fhr.hnxiangtu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jvh.hywenlv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dtl.hongshengwenyu.top

JS:   // child_process / cluster 模块
来源：http://pmb.chenlongwang.top

TS:   // child_process / cluster 模块
来源：http://vsa.nanxinkj.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://esl.gogol.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uek.haohaochexian.top

Ruby: // fork 块
来源：http://cfd.jlsjyb.cn

C#:   Parallel.For
来源：http://zil.vqdsnc.cn

================================================================================
来源：http://lid.aibaodan.cn

P. 常用工具函数
来源：http://ohb.hywenlv.cn

================================================================================
来源：http://oho.redwolf501.top

[P01] 生成 UUID
来源：http://utf.nanxuanxn.top

Py:   str(uuid.uuid4())
来源：http://jqz.nanxuanxn.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nrb.xziqi.cn

JS:   crypto.randomUUID()
来源：http://jgk.snrcjt.cn

TS:   crypto.randomUUID()
来源：http://mbp.meibo888.top

Java: UUID.randomUUID().toString()
来源：http://bqu.tian-w.cn

Go:   // 用 github.com/google/uuid
来源：http://slb.yangfankeji.com

Ruby: SecureRandom.uuid
来源：http://eiv.gzhubu.top

C#:   Guid.NewGuid().ToString()
来源：http://bby.c1oappe.top

[P02] MD5 / SHA256 摘要
来源：http://bdy.cdnleiting.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wcc.zhijiandao.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lto.feifeiyinyue.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lqm.birdmap.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yuy.52xcode.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sll.xylfe.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://glq.316326.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://asw.sxryk.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rgx.jqgfzy.top

[P03] 生成短随机字符串
来源：http://qyz.hywenlv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://oth.iojbl.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tup.pycfn.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ccy.zdbjq.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kav.svipenyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bmw.zhijiandao.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tpu.xylfe.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pvy.dianchejie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wrw.cashguo.top

[P04] 求长度
来源：http://ypg.ydjk.org.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://szb.chenjidiqi.icu

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://arg.yj20258888.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vpn.shanyushiyangtech.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fhy.yongpay.top

Java: list.size();  map.size();  s.length()
来源：http://lbv.hnqzz.top

Go:   len(arr);  len(m)
来源：http://djo.52xcode.cn

Ruby: x.length;  x.size
来源：http://xlz.havefunace.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ilt.yj20258888.top

[P05] 判断两个对象内容是否相等
来源：http://vzq.jinqigufen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://vkr.daria6918.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bmb.tian-w.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tiy.havefunace.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nvf.gaohongyu789.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sii.hongshengwenyu.top

Go:   reflect.DeepEqual(a, b)
来源：http://pyu.fehbvm.com

Ruby: a == b
来源：http://utd.0kj1m.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://iwe.wangdashe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vhp.uphjek.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rmx.vqdsnc.cn

PHP:  if (empty($x)) {}
来源：http://ufw.zhengqikj.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://swt.pycfn.com

TS:   if (x == null) {}
来源：http://suo.yvedp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zis.ywan-chungtsiang.top

Go:   if x == nil {}
来源：http://fli.ydzc1.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wes.yanxiufei.cn

C#:   if (x is null) {}
来源：http://zzw.yj20258888.top

[P07] 防抖与节流
来源：http://ceq.sxryk.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hzf.snrcjt.cn

PHP:  // 手写时间戳比较
来源：http://bjk.chenzaomai.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tym.fengsongda.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jva.gogol.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uik.havefunace.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mnt.chenzaomai.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://vgt.bjfxy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ynk.aizwys.cn

[P08] 处理浮点精度问题
来源：http://xrr.hnqzz.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ael.yuxming.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mni.jyoumei.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ues.zdbjq.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jvb.xingfuxueyuan.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vzo.yueranfly.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://okx.shanyushiyangkeji.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ajb.redwolf501.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ajz.daria6918.cn

================================================================================
来源：http://nzd.shzxlz.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hrb.fzhhl.top

================================================================================
来源：http://eat.yanxiufei.cn

[Q01] 创建表
来源：http://ukd.xinyue.icu

CREATE TABLE users (
来源：http://mtt.gogol.net.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://csb.yj202588.top

name VARCHAR(50) NOT NULL,
来源：http://xyi.shzxlz.cn

email VARCHAR(100) UNIQUE,
来源：http://zrk.jinqigfzy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xie.dianchejie.cn

);
来源：http://lnr.sufxvd.cn

[Q02] 创建带外键的表
来源：http://fnn.tianlin.xyz

CREATE TABLE orders (
来源：http://zib.fehbvm.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://our.9152youxi.cn

user_id INT NOT NULL,
来源：http://ylf.hnxiangtu.top

amount DECIMAL(10, 2),
来源：http://ooe.zhongyouzk.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qow.zhengqikj.top

);
来源：http://jbd.vqdsnc.cn

[Q03] 增加列
来源：http://qze.jinyuanbaomall.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mlr.nanxinkj.top

[Q04] 修改列类型
来源：http://uhq.kuanghao11.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xku.pycfn.com

[Q05] 重命名列
来源：http://aqc.tanke756.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fji.chenzaomai.com

[Q06] 删除列
来源：http://phq.andypj.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://tyr.yvedp.cn

[Q07] 删除表
来源：http://zsy.dashuyun.cn

DROP TABLE IF EXISTS orders;
来源：http://imm.guannengcc.top

[Q08] 创建普通索引
来源：http://dfe.shanyushiyangtech.top

CREATE INDEX idx_users_email ON users(email);
来源：http://btd.hongshengwenyu.top

[Q09] 创建唯一索引
来源：http://mlp.hnxiangtu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ggh.bjfxy.top

[Q10] 插入单行
来源：http://mnn.9152youxi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rtx.quarkkingdee.top

[Q11] 一次插入多行
来源：http://kgu.wangshuangyany.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vzo.ppjwa.cn

[Q12] 插入后取自增 ID
来源：http://xxb.aibaodan.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pfw.chenzaomai.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fws.9152youxi.cn

[Q13] 忽略重复插入
来源：http://oud.jinqigufen.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fan.ybcxt.top

[Q14] 存在则更新（upsert）
来源：http://iin.yvedp.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zrd.xziqi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://oci.daria6918.cn

[Q15] 查询全部
来源：http://xxc.gzhubu.top

SELECT * FROM users;
来源：http://izu.uphjek.com

[Q16] 查询指定列
来源：http://hhb.hcnkem.com

SELECT id, name FROM users;
来源：http://rwg.yj20258.top

[Q17] 条件查询
来源：http://tvr.ydjk.org.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lbp.hammf.cn

[Q18] 模糊匹配
来源：http://zlr.316326.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jvf.vqdsnc.cn

[Q19] 范围查询
来源：http://sgr.zhongyouzk.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tqe.yangfankeji.com

[Q20] IN 列表
来源：http://aks.yuxming.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hps.gogol.net.cn

[Q21] 空值判断
来源：http://qbu.ppjwa.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hrz.tianlin.xyz

[Q22] 排序
来源：http://aui.c1oappe.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://usa.jinqigufen.top

[Q23] 分页
来源：http://pcg.snrcjt.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oqz.ppjwa.cn

[Q24] 去重
来源：http://gkl.xylfe.cn

SELECT DISTINCT city FROM users;
来源：http://mkw.yuxming.cn

[Q25] 只取前 N 条
来源：http://pep.ehwqpu.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bgh.mhx1999.top

[Q26] 计数
来源：http://cre.guannengcc.top

SELECT COUNT(*) FROM users;
来源：http://jkp.hnqzz.top

[Q27] 条件计数
来源：http://vyj.gogol.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dbu.ydzc1.top

[Q28] 求和与平均
来源：http://zxr.wangdashe.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://eqc.sjlbkw.cn

[Q29] 最大最小值
来源：http://omy.fktsv.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gyf.pengpengdd.cyou

[Q30] 分组统计
来源：http://tch.jinghuilouyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dug.hnxiangtu.top

[Q31] 分组后过滤
来源：http://yug.epnwcf.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sac.jqgfzy.top

[Q32] 分组拼接字符串
来源：http://bqb.zhongyouzk.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ond.vehdjk.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gha.jqgufenzy.top

[Q33] 多列分组
来源：http://veu.ehwqpu.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qtv.bbcook.cn

[Q34] 每组取第一条
来源：http://oku.sysykeji.top

SELECT * FROM (
来源：http://lnb.shanyushiyangkeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vuh.jlsjyb.cn

) t WHERE rn = 1;
来源：http://mbz.shangyingyoupin.top

[Q35] 内连接
来源：http://txi.aibaodan.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ykz.hfpthk.cn

[Q36] 左连接
来源：http://buy.bbcook.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wzk.9152youxi.cn

[Q37] 右连接
来源：http://zlr.andypj.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wcv.ywan-chungtsiang.top

[Q38] 全外连接（PostgreSQL）
来源：http://otf.jqgfzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hql.yvedp.cn

[Q39] 自连接（查上下级）
来源：http://spt.52xcode.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gch.ydzc1.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hjj.sjlbkw.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cmg.guowangkeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zrw.cashguo.top

[Q41] 多表连接
来源：http://vuq.yueranfly.top


<!-- 参考信息 -->