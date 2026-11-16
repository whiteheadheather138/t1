代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qid.yvedp.cn

[N06] 判断回文字符串
来源：http://qvp.zhaomingkeji.xyz

Py:   s == s[::-1]
来源：http://fjj.jqgufenzy.top

PHP:  $s === strrev($s);
来源：http://rmu.jlsjyb.cn

JS:   s === [...s].reverse().join("")
来源：http://lyr.meibo888.top

TS:   s === [...s].reverse().join("")
来源：http://ing.ehwqpu.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vdc.fengsongda.top

Go:   // 双指针从两端比较
来源：http://vur.cqqwz.cn

Ruby: s == s.reverse
来源：http://ots.cheryme.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://nef.sxryk.cn

[N07] 两数之和（返回下标）
来源：http://pmh.yuxming.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://btb.jqgfzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://iai.sysykeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wyg.zhixingplan.top

TS:   // 手写 Map<string, number>
来源：http://sny.pengpengdd.cyou

Java: // 手写 HashMap
来源：http://mea.yuanzhike.top

Go:   // 手写 map[int]int
来源：http://ptx.zhoulong.xyz

Ruby: // 手写 Hash
来源：http://sgg.hcnkem.com

C#:   // 手写 Dictionary<int, int>
来源：http://gyp.ydzc1.top

[N08] 生成全排列
来源：http://pge.jinqigfzy.top

Py:   itertools.permutations(arr)
来源：http://zqo.mhx1999.top

PHP:  // 手写递归交换
来源：http://rsg.hnqzz.top

JS:   // 手写回溯递归
来源：http://npl.guannengcc.top

TS:   // 手写回溯递归
来源：http://urz.jianghu66.top

Java: // 手写回溯递归
来源：http://cpf.chenjidiqi.icu

Go:   // 手写回溯递归
来源：http://mgd.snrcjt.cn

Ruby: arr.permutation.to_a
来源：http://sos.fzhhl.top

C#:   // 手写回溯递归
来源：http://gpn.yangfankeji.com

[N09] 栈与队列
来源：http://iml.ctjpmb.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://why.zhaomingkeji.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://swj.yj20258.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nqc.shanyushiyangtech.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kwl.hfpthk.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dxj.iojbl.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kpg.chenzaomai.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wce.aibaodan.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dst.quarkkingdee.top

[N10] 链表节点定义
来源：http://yno.yuanzhike.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jbi.fanxiaobao.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://uxt.jinqigufen.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pje.nwbrower.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mkw.cheryme.top

Java: class Node { int v; Node next; }
来源：http://qqk.daria6918.cn

Go:   type Node struct { V int; Next *Node }
来源：http://kwl.zhengqikj.top

Ruby: Node = Struct.new(:v, :next)
来源：http://siv.hcnkem.com

C#:   class Node { public int V; public Node? Next; }
来源：http://utr.feifeiyinyue.top

[N11] 二叉树中序遍历
来源：http://muz.iojbl.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ugu.pengpengdd.cyou

PHP:  // 手写递归函数
来源：http://rtc.yj20258888.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://urd.nanxuanxn.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jer.dashuyun.cn

Java: // 手写递归
来源：http://jox.fzhhl.top

Go:   // 手写递归
来源：http://zzp.ppjwa.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pwv.yangfankeji.com

C#:   // 手写递归
来源：http://axi.xuetiantiany.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cbh.9152youxi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oql.gaohongyu789.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vzn.hongshengwenyu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jet.jqgufenzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cfm.kuanghao11.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cti.aizwys.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ano.ehwqpu.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qyc.vehdjk.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ird.yongpay.top

================================================================================
来源：http://owl.cashguo.top

O. 并发与异步
来源：http://nxg.aizwys.cn

================================================================================
来源：http://ksz.9152youxi.cn

[O01] 启动一个线程
来源：http://ymu.yfazqb.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xym.yuxming.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hqj.zycfv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zfi.fzhhl.top

TS:   // 同 JS
来源：http://gjk.wangshuangyany.cn

Java: new Thread(() -> f()).start()
来源：http://hcu.wangdashe.top

Go:   go f()
来源：http://nko.pycfn.com

Ruby: Thread.new { f }
来源：http://kgb.yj202588.top

C#:   Task.Run(() => F());
来源：http://rrv.zhongyouzk.top

[O02] 使用线程池
来源：http://wug.sjlbkw.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ntu.c1oappe.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://clq.shzxlz.cn

JS:   // worker_threads 线程池
来源：http://smq.zhiwuduotai.top

TS:   // worker_threads 线程池
来源：http://qze.hcnkem.com

Java: Executors.newFixedThreadPool(4)
来源：http://qqc.iojbl.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ucy.aibaodan.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zsl.yuxming.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oig.316326.xyz

[O03] 加锁保护共享数据
来源：http://fxf.nanxuanxn.top

Py:   with lock: shared += 1
来源：http://ezx.tianlin.xyz

PHP:  // 用 flock() 做文件锁
来源：http://npj.meibo888.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://oej.iojbl.cn

TS:   // 同 JS
来源：http://bcx.smart0.xyz

Java: synchronized (this) { shared++; }
来源：http://jmi.aizwys.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dhb.wangshuangyany.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jfk.shuidangran.top

C#:   lock (gate) { shared++; }
来源：http://uik.fktsv.cn

[O04] 定义异步函数并等待
来源：http://nyo.chenzaomai.com

Py:   async def f():⏎    await g()
来源：http://tfw.yangfankeji.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kwy.bbcook.cn

JS:   async function f() { await g(); }
来源：http://yhp.jinqigfzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://pdm.daxiang520.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wcw.9152youxi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bal.cashguo.top

Ruby: # 用 Fiber 或 async gem
来源：http://vfc.fktsv.cn

C#:   async Task F() { await G(); }
来源：http://flo.hammf.cn

[O05] 并发执行并等待全部完成
来源：http://ovn.fktsv.cn

Py:   asyncio.gather(*tasks)
来源：http://vyz.guowangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bec.gaohongyu789.top

JS:   await Promise.all(tasks)
来源：http://ybv.bjfxy.top

TS:   await Promise.all(tasks)
来源：http://tjo.ybcxt.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://aso.jiagoushi.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ggj.ivvv.top

Ruby: threads.map(&:join)
来源：http://myu.havefunace.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ysh.yj202588.top

[O06] 使用进程池
来源：http://lca.birdmap.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mzo.0kj1m.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fxa.shangyingyoupin.top

JS:   // child_process / cluster 模块
来源：http://hir.chenjidiqi.icu

TS:   // child_process / cluster 模块
来源：http://tmm.iojbl.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jnr.jyoumei.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fcc.yj20258888.top

Ruby: // fork 块
来源：http://hxx.zhoulong.xyz

C#:   Parallel.For
来源：http://jss.yj202588.top

================================================================================
来源：http://ekk.aizwys.cn

P. 常用工具函数
来源：http://wgr.hysaishi.cn

================================================================================
来源：http://zev.aizwys.cn

[P01] 生成 UUID
来源：http://tnz.daria6918.cn

Py:   str(uuid.uuid4())
来源：http://bne.cashguo.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yox.gzhubu.top

JS:   crypto.randomUUID()
来源：http://gic.birdmap.top

TS:   crypto.randomUUID()
来源：http://pmd.shangyingyoupin.top

Java: UUID.randomUUID().toString()
来源：http://uss.sufxvd.cn

Go:   // 用 github.com/google/uuid
来源：http://gqx.hnqzz.top

Ruby: SecureRandom.uuid
来源：http://hkj.daria6918.cn

C#:   Guid.NewGuid().ToString()
来源：http://xwg.zdqjudy.top

[P02] MD5 / SHA256 摘要
来源：http://vje.meibo888.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rrv.uphjek.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://exa.hnqzz.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nth.hnxiangtu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sez.quarkkingdee.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xth.ivvv.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uyy.gzhubu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cgy.c1oappe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://isd.zycfv.cn

[P03] 生成短随机字符串
来源：http://oob.aibaodan.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tqk.epnwcf.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ptg.nanxuanxn.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gfs.hammf.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ukc.hnxiangtu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wpk.redwolf501.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fvt.yangfankeji.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://nnw.tian-w.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kvz.fanxiaobao.xyz

[P04] 求长度
来源：http://odz.hysaishi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nbt.hcnkem.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lcu.9152youxi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mff.zhongyouzk.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://upo.zhijiandao.cn

Java: list.size();  map.size();  s.length()
来源：http://msq.yfazqb.com

Go:   len(arr);  len(m)
来源：http://dym.zhijiandao.cn

Ruby: x.length;  x.size
来源：http://jwa.chenlongwang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://rji.yj20258.top

[P05] 判断两个对象内容是否相等
来源：http://dtu.fktsv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wau.sufxvd.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bcn.chenlongwang.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tvu.cheryme.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://saf.ybcxt.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gbz.ybcxt.top

Go:   reflect.DeepEqual(a, b)
来源：http://wer.pycfn.com

Ruby: a == b
来源：http://ufm.gzhubu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nnq.yangfankeji.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vud.andypj.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tqq.quarkkingdee.top

PHP:  if (empty($x)) {}
来源：http://tdk.svipenyu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bmx.xylfe.cn

TS:   if (x == null) {}
来源：http://rlv.jqgfzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://xrz.chenzaomai.com

Go:   if x == nil {}
来源：http://kma.c1oappe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wby.chenzaomai.com

C#:   if (x is null) {}
来源：http://lwp.xingfuxueyuan.xyz

[P07] 防抖与节流
来源：http://rkl.9152youxi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wrt.shanyushiyangtech.top

PHP:  // 手写时间戳比较
来源：http://djc.wangdashe.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dam.hfpthk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xdi.fengsongda.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qls.yonumen.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://eua.quarkkingdee.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://qtu.bbcook.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fqo.jyoumei.cn

[P08] 处理浮点精度问题
来源：http://div.daria6918.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://div.hnxiangtu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://skr.birdmap.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fbk.jinqigufen.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tfp.0kj1m.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ilq.bbcook.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fac.yuanzhike.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ruu.fengsongda.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tpi.xuetiantiany.cn

================================================================================
来源：http://adl.nanxuanxn.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dxx.redwolf501.top

================================================================================
来源：http://zpi.wangdashe.top

[Q01] 创建表
来源：http://xqg.fehbvm.com

CREATE TABLE users (
来源：http://dbi.ivvv.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ktd.shzxlz.cn

name VARCHAR(50) NOT NULL,
来源：http://vvg.smart0.xyz

email VARCHAR(100) UNIQUE,
来源：http://ovn.hammf.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nxj.zdbjq.cn

);
来源：http://eap.gotoacloud.top

[Q02] 创建带外键的表
来源：http://vey.uphjek.com

CREATE TABLE orders (
来源：http://dwk.nanxuanxn.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vvd.mhx1999.top

user_id INT NOT NULL,
来源：http://ezq.xingfuxueyuan.xyz

amount DECIMAL(10, 2),
来源：http://puz.jinqigfzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pew.hnxiangtu.top

);
来源：http://aeu.0kj1m.cn

[Q03] 增加列
来源：http://mye.chenjidiqi.icu

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wrm.jinqigfzy.top

[Q04] 修改列类型
来源：http://plv.havefunace.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vit.yvedp.cn

[Q05] 重命名列
来源：http://vke.mhx1999.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qkb.cqqwz.cn

[Q06] 删除列
来源：http://ynl.yanxiufei.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fqd.ehwqpu.com

[Q07] 删除表
来源：http://ygb.yanxiufei.cn

DROP TABLE IF EXISTS orders;
来源：http://rba.ivvv.top

[Q08] 创建普通索引
来源：http://sxe.yj20258.top

CREATE INDEX idx_users_email ON users(email);
来源：http://hzl.birdmap.top

[Q09] 创建唯一索引
来源：http://hby.wangdashe.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://axp.birdmap.top

[Q10] 插入单行
来源：http://xar.feifeiyinyue.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tky.fktsv.cn

[Q11] 一次插入多行
来源：http://pyx.xinyue.icu

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jvt.jqgfzy.top

[Q12] 插入后取自增 ID
来源：http://kmw.vehdjk.com

INSERT INTO users (name) VALUES ('C');
来源：http://rjh.yvedp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hzj.mhx1999.top

[Q13] 忽略重复插入
来源：http://bwz.hnxiangtu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kdl.sweek.top

[Q14] 存在则更新（upsert）
来源：http://qgt.jlsjyb.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://leq.birdmap.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qsq.zhengqikj.top

[Q15] 查询全部
来源：http://jsi.yj20258.top

SELECT * FROM users;
来源：http://sic.chenjidiqi.icu

[Q16] 查询指定列
来源：http://afo.0kj1m.cn

SELECT id, name FROM users;
来源：http://eqo.sysykeji.top

[Q17] 条件查询
来源：http://ywt.andypj.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://snm.guannengcc.top

[Q18] 模糊匹配
来源：http://tzv.fktsv.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qnm.gotoacloud.top

[Q19] 范围查询
来源：http://zwk.jianghu66.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xcj.gogol.net.cn

[Q20] IN 列表
来源：http://nfx.yonumen.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wtq.bjfxy.top

[Q21] 空值判断
来源：http://yxk.pengpengdd.cyou

SELECT * FROM users WHERE email IS NULL;
来源：http://itp.feifeiyinyue.top

[Q22] 排序
来源：http://imh.zdbjq.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nqj.9152youxi.cn

[Q23] 分页
来源：http://mjd.meibo888.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ygb.zycfv.cn

[Q24] 去重
来源：http://bxu.gotoacloud.top

SELECT DISTINCT city FROM users;
来源：http://joo.cheryme.top

[Q25] 只取前 N 条
来源：http://ncw.chenjidiqi.icu

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cia.pengpengdd.cyou

[Q26] 计数
来源：http://oae.9152youxi.cn

SELECT COUNT(*) FROM users;
来源：http://dpk.tanke756.top

[Q27] 条件计数
来源：http://ucu.yuanzhike.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iod.ehwqpu.com

[Q28] 求和与平均
来源：http://xhg.wangshuangyany.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://trn.birdmap.top

[Q29] 最大最小值
来源：http://win.dianchejie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wdw.birdmap.top

[Q30] 分组统计
来源：http://ute.bjfxy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bmi.chenzaomai.com

[Q31] 分组后过滤
来源：http://xda.fzhhl.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wmr.fengsongda.top

[Q32] 分组拼接字符串
来源：http://yqf.hnqzz.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tuf.zhaomingkeji.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://spz.hfpthk.cn

[Q33] 多列分组
来源：http://wfv.zhongyouzk.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wfj.gotoacloud.top

[Q34] 每组取第一条
来源：http://utt.sxryk.cn

SELECT * FROM (
来源：http://yqv.yueranfly.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://srg.yfazqb.com

) t WHERE rn = 1;
来源：http://bpw.vqdsnc.cn

[Q35] 内连接
来源：http://jig.shuidangran.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hlo.wangdashe.top

[Q36] 左连接
来源：http://poq.ydzc1.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://htg.zhoulong.xyz

[Q37] 右连接
来源：http://abj.cdnleiting.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fdz.chenjidiqi.icu

[Q38] 全外连接（PostgreSQL）
来源：http://zmw.ivvv.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gxc.hnqzz.top

[Q39] 自连接（查上下级）
来源：http://ucq.jyoumei.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://brv.yongpay.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://aub.52xcode.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ato.wangdashe.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cph.nanxinkj.top

[Q41] 多表连接
来源：http://rqa.vqdsnc.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jyq.ppjwa.cn

JOIN users u ON u.id = o.user_id
来源：http://sfo.meibo888.top

JOIN products p ON p.id = o.product_id;
来源：http://zcm.yuxming.cn

[Q42] 连接条件附加过滤
来源：http://jhb.cashguo.top


<!-- 参考信息 -->