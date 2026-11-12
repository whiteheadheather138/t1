代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hoq.jqgfzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://svo.chenjidiqi.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pzk.zycfv.cn

Ruby: a.gcd(b)
来源：http://qwg.guowangkeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ahp.shangyingyoupin.top

[N06] 判断回文字符串
来源：http://ngl.jlsjyb.cn

Py:   s == s[::-1]
来源：http://kqy.pycfn.com

PHP:  $s === strrev($s);
来源：http://xpf.fktsv.cn

JS:   s === [...s].reverse().join("")
来源：http://gwx.zhiwuduotai.top

TS:   s === [...s].reverse().join("")
来源：http://iwg.ydzc1.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fzv.zycfv.cn

Go:   // 双指针从两端比较
来源：http://uqf.hnqzz.top

Ruby: s == s.reverse
来源：http://bhc.zhaomingkeji.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://ccm.316326.xyz

[N07] 两数之和（返回下标）
来源：http://kiv.svipenyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cay.ydzc1.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mfy.xuetiantiany.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ccc.cqqwz.cn

TS:   // 手写 Map<string, number>
来源：http://rvi.chenlongwang.top

Java: // 手写 HashMap
来源：http://zxj.xingfuxueyuan.xyz

Go:   // 手写 map[int]int
来源：http://vnc.yongpay.top

Ruby: // 手写 Hash
来源：http://czf.xuanzx.com

C#:   // 手写 Dictionary<int, int>
来源：http://tnk.nwbrower.top

[N08] 生成全排列
来源：http://oto.xuetiantiany.cn

Py:   itertools.permutations(arr)
来源：http://llf.redwolf501.top

PHP:  // 手写递归交换
来源：http://esd.ppjwa.cn

JS:   // 手写回溯递归
来源：http://hza.ydjk.org.cn

TS:   // 手写回溯递归
来源：http://bjv.haohaochexian.top

Java: // 手写回溯递归
来源：http://udh.c1oappe.top

Go:   // 手写回溯递归
来源：http://nho.ivvv.top

Ruby: arr.permutation.to_a
来源：http://onj.nanxinkj.top

C#:   // 手写回溯递归
来源：http://rps.shuidangran.top

[N09] 栈与队列
来源：http://jbo.shanyushiyangkeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nde.xuetiantiany.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mac.pycfn.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ear.ybcxt.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://aib.zhijiandao.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mvo.ydzc1.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jpf.cashguo.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tkf.cucudq.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vwx.sufxvd.cn

[N10] 链表节点定义
来源：http://wks.zdbjq.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xuz.shzxlz.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://imd.jiagoushi.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://faf.iojbl.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qek.yueranfly.top

Java: class Node { int v; Node next; }
来源：http://jhd.hysaishi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vyd.quarkkingdee.top

Ruby: Node = Struct.new(:v, :next)
来源：http://bpi.redwolf501.top

C#:   class Node { public int V; public Node? Next; }
来源：http://gzx.ydzc1.top

[N11] 二叉树中序遍历
来源：http://iau.smart0.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tdk.jqgfzy.top

PHP:  // 手写递归函数
来源：http://kpv.cucudq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ref.birdmap.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uym.tanke756.top

Java: // 手写递归
来源：http://ehi.xylfe.cn

Go:   // 手写递归
来源：http://abp.guannengcc.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://weo.yfazqb.com

C#:   // 手写递归
来源：http://jma.tanke756.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blg.fzhhl.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pny.wangshuangyany.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sfb.9152youxi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lec.yuxming.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://djj.jinqigufen.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kul.jqgfzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ado.cheryme.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rcp.tarul.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uzk.52xcode.cn

================================================================================
来源：http://irw.jianghu66.top

O. 并发与异步
来源：http://iff.zhijiandao.cn

================================================================================
来源：http://tuv.xinyue.icu

[O01] 启动一个线程
来源：http://cgd.fktsv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zvy.aizwys.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mys.andypj.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mcv.ehwqpu.com

TS:   // 同 JS
来源：http://sza.gzhubu.top

Java: new Thread(() -> f()).start()
来源：http://nyo.gaohongyu789.top

Go:   go f()
来源：http://wvb.yj20258888.top

Ruby: Thread.new { f }
来源：http://tnm.gogol.net.cn

C#:   Task.Run(() => F());
来源：http://hhc.hongshengwenyu.top

[O02] 使用线程池
来源：http://kfp.chenjidiqi.icu

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uxl.ctjpmb.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fsz.jinyuanbaomall.cn

JS:   // worker_threads 线程池
来源：http://xvp.zhiwuduotai.top

TS:   // worker_threads 线程池
来源：http://kld.svipenyu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ari.xuetiantiany.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vdf.iojbl.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bqp.jinghuilouyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ycl.redwolf501.top

[O03] 加锁保护共享数据
来源：http://ymq.snrcjt.cn

Py:   with lock: shared += 1
来源：http://eqa.xuanzx.com

PHP:  // 用 flock() 做文件锁
来源：http://obk.snrcjt.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://urs.yuxming.cn

TS:   // 同 JS
来源：http://sly.yuxming.cn

Java: synchronized (this) { shared++; }
来源：http://ubf.yj202588.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lij.andypj.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://fnw.fehbvm.com

C#:   lock (gate) { shared++; }
来源：http://rhd.52xcode.cn

[O04] 定义异步函数并等待
来源：http://dal.daxiang520.top

Py:   async def f():⏎    await g()
来源：http://jrh.xingfuxueyuan.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lei.andypj.xyz

JS:   async function f() { await g(); }
来源：http://zfg.wangdashe.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://lcc.52xcode.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nfn.chenlongwang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://msv.yj20258888.top

Ruby: # 用 Fiber 或 async gem
来源：http://xfi.yanxiufei.cn

C#:   async Task F() { await G(); }
来源：http://zgd.jiagoushi.top

[O05] 并发执行并等待全部完成
来源：http://xls.cqqwz.cn

Py:   asyncio.gather(*tasks)
来源：http://rqo.hammf.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yfy.gogol.net.cn

JS:   await Promise.all(tasks)
来源：http://pnn.nanxinkj.top

TS:   await Promise.all(tasks)
来源：http://vqi.tian-w.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zbb.guannengcc.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://eyr.jinqigufen.top

Ruby: threads.map(&:join)
来源：http://kqb.feifeiyinyue.top

C#:   await Task.WhenAll(t1, t2)
来源：http://trp.haohaochexian.top

[O06] 使用进程池
来源：http://rfe.0kj1m.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gaa.zdbjq.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fmh.zhoulong.xyz

JS:   // child_process / cluster 模块
来源：http://plk.guannengcc.top

TS:   // child_process / cluster 模块
来源：http://msz.jinghuilouyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rin.hammf.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://awt.quarkkingdee.top

Ruby: // fork 块
来源：http://ksd.jinqigufen.top

C#:   Parallel.For
来源：http://qym.jyoumei.cn

================================================================================
来源：http://wps.yuanzhike.top

P. 常用工具函数
来源：http://zer.hesvh.cn

================================================================================
来源：http://qbg.zdqjudy.top

[P01] 生成 UUID
来源：http://djv.fktsv.cn

Py:   str(uuid.uuid4())
来源：http://fsn.birdmap.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uce.xuanzx.com

JS:   crypto.randomUUID()
来源：http://vjk.sjlbkw.cn

TS:   crypto.randomUUID()
来源：http://vve.cqqwz.cn

Java: UUID.randomUUID().toString()
来源：http://qkn.yfazqb.com

Go:   // 用 github.com/google/uuid
来源：http://rdr.tianlin.xyz

Ruby: SecureRandom.uuid
来源：http://xje.daxiang520.top

C#:   Guid.NewGuid().ToString()
来源：http://tfw.bjfxy.top

[P02] MD5 / SHA256 摘要
来源：http://ido.shuidangran.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://obe.yueranfly.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://bno.iojbl.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://isk.sweek.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://api.nanxinkj.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dqj.zhengqikj.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zyy.ppjwa.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qid.epnwcf.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://flg.quarkkingdee.top

[P03] 生成短随机字符串
来源：http://oqp.yj20258.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qwc.epnwcf.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vjw.shanyushiyangkeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vde.birdmap.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nll.dashuyun.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xnk.yangfankeji.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zjc.ctjpmb.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://clj.zhaomingkeji.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qmu.jianghu66.top

[P04] 求长度
来源：http://vau.zhijiandao.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tgm.yfazqb.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://esw.meibo888.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://khb.hongshengwenyu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vxt.tian-w.cn

Java: list.size();  map.size();  s.length()
来源：http://rpb.xuetiantiany.cn

Go:   len(arr);  len(m)
来源：http://bne.yuanzhike.top

Ruby: x.length;  x.size
来源：http://pij.hnqzz.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://bdn.yuxming.cn

[P05] 判断两个对象内容是否相等
来源：http://cqm.hnqzz.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://nvj.birdmap.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yyd.gaohongyu789.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ysk.smart0.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fgs.xingfuxueyuan.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ubq.shanyushiyangtech.top

Go:   reflect.DeepEqual(a, b)
来源：http://fsd.tianlin.xyz

Ruby: a == b
来源：http://uvl.svipenyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lbr.yonumen.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kuz.zdqjudy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qeb.sysykeji.top

PHP:  if (empty($x)) {}
来源：http://qye.ivvv.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yvd.nanxinkj.top

TS:   if (x == null) {}
来源：http://nnm.zhijiandao.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kah.hfpthk.cn

Go:   if x == nil {}
来源：http://ovv.shanyushiyangtech.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vnk.hongshengwenyu.top

C#:   if (x is null) {}
来源：http://fpj.uphjek.com

[P07] 防抖与节流
来源：http://hga.cdnleiting.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tqn.shanyushiyangkeji.top

PHP:  // 手写时间戳比较
来源：http://zjb.yj20258.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xbc.daria6918.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mim.guannengcc.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fci.shzxlz.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rts.shuidangran.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://vnf.jianghu66.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lqd.c1oappe.top

[P08] 处理浮点精度问题
来源：http://hti.tanke756.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://efz.tanke756.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fxy.hcnkem.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zhp.jinqigfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ztm.jinghuilouyu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://joc.feifeiyinyue.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hsj.jiagoushi.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xwd.shuidangran.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hfw.yongpay.top

================================================================================
来源：http://bif.9152youxi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hnj.shanyushiyangtech.top

================================================================================
来源：http://qfh.havefunace.top

[Q01] 创建表
来源：http://zum.tianlin.xyz

CREATE TABLE users (
来源：http://rhw.cqqwz.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://viy.sufxvd.cn

name VARCHAR(50) NOT NULL,
来源：http://irp.haohaochexian.top

email VARCHAR(100) UNIQUE,
来源：http://piq.nanxinkj.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://shi.zhoulong.xyz

);
来源：http://xmm.cheryme.top

[Q02] 创建带外键的表
来源：http://ylk.zhijiandao.cn

CREATE TABLE orders (
来源：http://dji.sufxvd.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rpf.yuxming.cn

user_id INT NOT NULL,
来源：http://ufv.yfazqb.com

amount DECIMAL(10, 2),
来源：http://hkb.feifeiyinyue.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nju.nanxuanxn.top

);
来源：http://muc.birdmap.top

[Q03] 增加列
来源：http://ath.gotoacloud.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dfn.chenzaomai.com

[Q04] 修改列类型
来源：http://ptp.fzhhl.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wgl.yfazqb.com

[Q05] 重命名列
来源：http://nmk.mhx1999.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dao.redwolf501.top

[Q06] 删除列
来源：http://hys.xylfe.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dtq.nanxinkj.top

[Q07] 删除表
来源：http://heu.smart0.xyz

DROP TABLE IF EXISTS orders;
来源：http://qpq.fzhhl.top

[Q08] 创建普通索引
来源：http://xwf.0kj1m.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kps.sweek.top

[Q09] 创建唯一索引
来源：http://vug.hongshengwenyu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rqx.ppjwa.cn

[Q10] 插入单行
来源：http://vmc.feifeiyinyue.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qpq.shuidangran.top

[Q11] 一次插入多行
来源：http://wkb.tanke756.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bjc.xuetiantiany.cn

[Q12] 插入后取自增 ID
来源：http://zoq.nanxinkj.top

INSERT INTO users (name) VALUES ('C');
来源：http://aad.cashguo.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vfa.quarkkingdee.top

[Q13] 忽略重复插入
来源：http://ssf.bjfxy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://clw.0kj1m.cn

[Q14] 存在则更新（upsert）
来源：http://gex.epnwcf.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://urt.dashuyun.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dua.cashguo.top

[Q15] 查询全部
来源：http://bot.yfazqb.com

SELECT * FROM users;
来源：http://vhn.jyoumei.cn

[Q16] 查询指定列
来源：http://fsf.sjlbkw.cn

SELECT id, name FROM users;
来源：http://tpk.birdmap.top

[Q17] 条件查询
来源：http://pyw.cqqwz.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vwe.ybcxt.top

[Q18] 模糊匹配
来源：http://nkp.yanxiufei.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lpw.cucudq.cn

[Q19] 范围查询
来源：http://goi.ctjpmb.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bvr.vqdsnc.cn

[Q20] IN 列表
来源：http://yju.quarkkingdee.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jql.yueranfly.top

[Q21] 空值判断
来源：http://gzu.shzxlz.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jjh.ivvv.top

[Q22] 排序
来源：http://bfg.zhaomingkeji.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kni.feifeiyinyue.top

[Q23] 分页
来源：http://xje.ywan-chungtsiang.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://txh.jqgfzy.top

[Q24] 去重
来源：http://ijw.svipenyu.cn

SELECT DISTINCT city FROM users;
来源：http://ooj.nanxinkj.top

[Q25] 只取前 N 条
来源：http://gik.chenzaomai.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pph.fktsv.cn

[Q26] 计数
来源：http://szz.smart0.xyz

SELECT COUNT(*) FROM users;
来源：http://vxr.guowangkeji.top

[Q27] 条件计数
来源：http://esx.gzhubu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xbs.jinqigufen.top

[Q28] 求和与平均
来源：http://bes.sysykeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rvw.quarkkingdee.top

[Q29] 最大最小值
来源：http://kvz.yanxiufei.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xqc.fanxiaobao.xyz

[Q30] 分组统计
来源：http://orq.bbcook.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://czp.nanxuanxn.top

[Q31] 分组后过滤
来源：http://ref.guannengcc.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zyn.nanxuanxn.top

[Q32] 分组拼接字符串
来源：http://sal.andypj.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qgy.nwbrower.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xnr.c1oappe.top

[Q33] 多列分组
来源：http://mfo.vehdjk.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://olm.vehdjk.com

[Q34] 每组取第一条
来源：http://yor.daria6918.cn

SELECT * FROM (
来源：http://okh.smart0.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nft.yueranfly.top

) t WHERE rn = 1;
来源：http://gou.ctjpmb.com

[Q35] 内连接
来源：http://giu.hesvh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dim.yueranfly.top

[Q36] 左连接
来源：http://cyl.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mqe.meibo888.top

[Q37] 右连接
来源：http://jaq.hywenlv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zcj.yonumen.top

[Q38] 全外连接（PostgreSQL）
来源：http://gsh.nwbrower.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pab.cashguo.top

[Q39] 自连接（查上下级）
来源：http://yxh.cdnleiting.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://jdt.redwolf501.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lto.sufxvd.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://oep.aibaodan.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rzg.zhoulong.xyz

[Q41] 多表连接
来源：http://cgt.zhaomingkeji.xyz


<!-- 参考信息 -->