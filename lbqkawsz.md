代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gne.zhijiandao.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://egy.fehbvm.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hsk.xuanzx.com

Ruby: a.gcd(b)
来源：http://uky.vqdsnc.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tgk.nanxinkj.top

[N06] 判断回文字符串
来源：http://huh.yfazqb.com

Py:   s == s[::-1]
来源：http://wlm.yuxming.cn

PHP:  $s === strrev($s);
来源：http://pqn.tian-w.cn

JS:   s === [...s].reverse().join("")
来源：http://zwu.nanxinkj.top

TS:   s === [...s].reverse().join("")
来源：http://she.fanxiaobao.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bna.hammf.cn

Go:   // 双指针从两端比较
来源：http://yxz.meibo888.top

Ruby: s == s.reverse
来源：http://yoo.tarul.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tom.yuanzhike.top

[N07] 两数之和（返回下标）
来源：http://lpk.yuxming.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kkz.sysykeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cos.dashuyun.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qrg.zhaomingkeji.xyz

TS:   // 手写 Map<string, number>
来源：http://nmb.bjfxy.top

Java: // 手写 HashMap
来源：http://nrc.fengsongda.top

Go:   // 手写 map[int]int
来源：http://hxz.ybcxt.top

Ruby: // 手写 Hash
来源：http://psi.iojbl.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dwe.ehwqpu.com

[N08] 生成全排列
来源：http://fpl.uphjek.com

Py:   itertools.permutations(arr)
来源：http://xca.kuanghao11.cn

PHP:  // 手写递归交换
来源：http://abp.tianlin.xyz

JS:   // 手写回溯递归
来源：http://dbe.yfazqb.com

TS:   // 手写回溯递归
来源：http://ofk.sxryk.cn

Java: // 手写回溯递归
来源：http://psq.ivvv.top

Go:   // 手写回溯递归
来源：http://cov.mhx1999.top

Ruby: arr.permutation.to_a
来源：http://rhl.hammf.cn

C#:   // 手写回溯递归
来源：http://nxp.hysaishi.cn

[N09] 栈与队列
来源：http://fpc.fengsongda.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kbm.chenjidiqi.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dxi.daxiang520.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qhy.yanxiufei.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://frp.zdbjq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zkq.yanxiufei.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://twq.vqdsnc.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kkp.jyoumei.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zaa.fanxiaobao.xyz

[N10] 链表节点定义
来源：http://ide.zycfv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lsi.jyoumei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://afo.vqdsnc.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ppz.jlsjyb.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ats.jinghuilouyu.cn

Java: class Node { int v; Node next; }
来源：http://aqj.jlsjyb.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tiq.sxryk.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lvw.hesvh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://frh.hysaishi.cn

[N11] 二叉树中序遍历
来源：http://gcf.bjfxy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zov.guannengcc.top

PHP:  // 手写递归函数
来源：http://yuk.ivvv.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://psy.yj20258.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ccs.haohaochexian.top

Java: // 手写递归
来源：http://faw.yangfankeji.com

Go:   // 手写递归
来源：http://tqr.sweek.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jpd.zhijiandao.cn

C#:   // 手写递归
来源：http://wan.gotoacloud.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zpq.pycfn.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ate.gzhubu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://moe.bjfxy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jfe.nwbrower.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://olq.mhx1999.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nqm.jinqigfzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xfs.cucudq.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zfh.pycfn.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jjh.daria6918.cn

================================================================================
来源：http://hwl.xinyue.icu

O. 并发与异步
来源：http://jji.zdbjq.cn

================================================================================
来源：http://yoe.yvedp.cn

[O01] 启动一个线程
来源：http://nmj.fktsv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mvx.gzhubu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kux.aibaodan.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://och.jiagoushi.top

TS:   // 同 JS
来源：http://hmq.wangdashe.top

Java: new Thread(() -> f()).start()
来源：http://pzh.yj202588.top

Go:   go f()
来源：http://qyi.iojbl.cn

Ruby: Thread.new { f }
来源：http://zrg.fehbvm.com

C#:   Task.Run(() => F());
来源：http://zhu.guowangkeji.top

[O02] 使用线程池
来源：http://bdj.chenlongwang.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zez.hysaishi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qka.shanyushiyangkeji.top

JS:   // worker_threads 线程池
来源：http://owl.ybcxt.top

TS:   // worker_threads 线程池
来源：http://ama.ppjwa.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hoi.yvedp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xns.havefunace.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sak.nanxinkj.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://osk.fktsv.cn

[O03] 加锁保护共享数据
来源：http://mpn.gogol.net.cn

Py:   with lock: shared += 1
来源：http://yjw.fehbvm.com

PHP:  // 用 flock() 做文件锁
来源：http://avr.gzhubu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://voz.redwolf501.top

TS:   // 同 JS
来源：http://wco.fengsongda.top

Java: synchronized (this) { shared++; }
来源：http://ggp.haohaochexian.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uwx.gaohongyu789.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://env.hfpthk.cn

C#:   lock (gate) { shared++; }
来源：http://szf.yj20258888.top

[O04] 定义异步函数并等待
来源：http://akn.cdnleiting.top

Py:   async def f():⏎    await g()
来源：http://foh.ppjwa.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eco.bjfxy.top

JS:   async function f() { await g(); }
来源：http://sux.fanxiaobao.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://jse.jqgufenzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zjv.ehwqpu.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cuy.guannengcc.top

Ruby: # 用 Fiber 或 async gem
来源：http://kpu.fzhhl.top

C#:   async Task F() { await G(); }
来源：http://ppe.xuanzx.com

[O05] 并发执行并等待全部完成
来源：http://ate.sysykeji.top

Py:   asyncio.gather(*tasks)
来源：http://tqq.hywenlv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cmu.daria6918.cn

JS:   await Promise.all(tasks)
来源：http://sof.cashguo.top

TS:   await Promise.all(tasks)
来源：http://rbj.zdbjq.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uso.hnxiangtu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pvn.zhijiandao.cn

Ruby: threads.map(&:join)
来源：http://noc.shanyushiyangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://jfw.gzhubu.top

[O06] 使用进程池
来源：http://tpr.kuanghao11.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fbe.vqdsnc.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://iyq.andypj.xyz

JS:   // child_process / cluster 模块
来源：http://akt.guowangkeji.top

TS:   // child_process / cluster 模块
来源：http://jah.ehwqpu.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dlf.ehwqpu.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eju.xziqi.cn

Ruby: // fork 块
来源：http://wpl.svipenyu.cn

C#:   Parallel.For
来源：http://qaj.cdnleiting.top

================================================================================
来源：http://hez.fzhhl.top

P. 常用工具函数
来源：http://ddz.cqqwz.cn

================================================================================
来源：http://whx.ehwqpu.com

[P01] 生成 UUID
来源：http://xje.sweek.top

Py:   str(uuid.uuid4())
来源：http://hby.chenlongwang.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lhi.jqgufenzy.top

JS:   crypto.randomUUID()
来源：http://htr.ehwqpu.com

TS:   crypto.randomUUID()
来源：http://vmu.ydzc1.top

Java: UUID.randomUUID().toString()
来源：http://imz.fengsongda.top

Go:   // 用 github.com/google/uuid
来源：http://fbe.yonumen.top

Ruby: SecureRandom.uuid
来源：http://rvf.tianlin.xyz

C#:   Guid.NewGuid().ToString()
来源：http://tfu.yueranfly.top

[P02] MD5 / SHA256 摘要
来源：http://adw.xylfe.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bqt.guannengcc.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://kyj.yuanzhike.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zla.svipenyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hon.jinghuilouyu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vfg.hesvh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yhw.cashguo.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vej.haohaochexian.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lfh.xingfuxueyuan.xyz

[P03] 生成短随机字符串
来源：http://omo.zdbjq.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lpy.hnxiangtu.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cjy.chenlongwang.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lrj.jqgfzy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cjt.jinyuanbaomall.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wyi.ydjk.org.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://beq.ctjpmb.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://lhe.yangfankeji.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bvs.zhoulong.xyz

[P04] 求长度
来源：http://mpz.gogol.net.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nte.jqgfzy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nag.chenjidiqi.icu

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xqm.quarkkingdee.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://foe.sxryk.cn

Java: list.size();  map.size();  s.length()
来源：http://qwz.ppjwa.cn

Go:   len(arr);  len(m)
来源：http://xxd.redwolf501.top

Ruby: x.length;  x.size
来源：http://zzi.cheryme.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://yjj.sjlbkw.cn

[P05] 判断两个对象内容是否相等
来源：http://fzn.ywan-chungtsiang.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://dxt.jyoumei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qlr.sjlbkw.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qin.yueranfly.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lnw.cashguo.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zey.zhixingplan.top

Go:   reflect.DeepEqual(a, b)
来源：http://rhy.jlsjyb.cn

Ruby: a == b
来源：http://zkh.fengsongda.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://job.xuanzx.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xta.aibaodan.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ftc.xziqi.cn

PHP:  if (empty($x)) {}
来源：http://kwh.fanxiaobao.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hsa.zhiwuduotai.top

TS:   if (x == null) {}
来源：http://zng.tarul.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kto.meibo888.top

Go:   if x == nil {}
来源：http://dyy.bbcook.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://piz.jqgfzy.top

C#:   if (x is null) {}
来源：http://xmy.xylfe.cn

[P07] 防抖与节流
来源：http://fjb.bjfxy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://swf.bbcook.cn

PHP:  // 手写时间戳比较
来源：http://rny.0kj1m.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wpq.jiagoushi.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nuu.meibo888.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://iga.xziqi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://aap.0kj1m.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rbi.chenjidiqi.icu

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lev.jinqigufen.top

[P08] 处理浮点精度问题
来源：http://dxv.hesvh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yej.pengpengdd.cyou

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uda.nanxinkj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dmj.shanyushiyangkeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dvz.zhijiandao.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ktv.sxryk.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xmk.shangyingyoupin.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ppy.shangyingyoupin.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dkn.tanke756.top

================================================================================
来源：http://xrc.vehdjk.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ihc.guannengcc.top

================================================================================
来源：http://ahg.yongpay.top

[Q01] 创建表
来源：http://lqt.birdmap.top

CREATE TABLE users (
来源：http://kwn.cheryme.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lql.hcnkem.com

name VARCHAR(50) NOT NULL,
来源：http://gmc.hywenlv.cn

email VARCHAR(100) UNIQUE,
来源：http://uka.aibaodan.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hir.zdqjudy.top

);
来源：http://cyo.jyoumei.cn

[Q02] 创建带外键的表
来源：http://nce.wangshuangyany.cn

CREATE TABLE orders (
来源：http://mmj.daxiang520.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xzv.chenzaomai.com

user_id INT NOT NULL,
来源：http://ucb.sjlbkw.cn

amount DECIMAL(10, 2),
来源：http://zap.iojbl.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fsa.yj202588.top

);
来源：http://fuz.c1oappe.top

[Q03] 增加列
来源：http://lhq.wangshuangyany.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://any.jiagoushi.top

[Q04] 修改列类型
来源：http://dxv.zhixingplan.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jis.yuanzhike.top

[Q05] 重命名列
来源：http://gsf.mhx1999.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ckg.bjfxy.top

[Q06] 删除列
来源：http://biw.fzhhl.top

ALTER TABLE users DROP COLUMN age;
来源：http://aqg.sweek.top

[Q07] 删除表
来源：http://fsd.hnxiangtu.top

DROP TABLE IF EXISTS orders;
来源：http://wbk.mhx1999.top

[Q08] 创建普通索引
来源：http://sym.zhijiandao.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://iqa.gogol.net.cn

[Q09] 创建唯一索引
来源：http://cqy.nwbrower.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sjb.ivvv.top

[Q10] 插入单行
来源：http://jlj.uphjek.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ica.shuidangran.top

[Q11] 一次插入多行
来源：http://slb.ctjpmb.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ihu.hfpthk.cn

[Q12] 插入后取自增 ID
来源：http://pua.jinyuanbaomall.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ayb.chenlongwang.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ade.mhx1999.top

[Q13] 忽略重复插入
来源：http://hrb.xziqi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cat.jqgufenzy.top

[Q14] 存在则更新（upsert）
来源：http://cwl.shzxlz.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kkz.shuidangran.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zfp.nwbrower.top

[Q15] 查询全部
来源：http://kyg.cashguo.top

SELECT * FROM users;
来源：http://fmv.chenjidiqi.icu

[Q16] 查询指定列
来源：http://noe.hfpthk.cn

SELECT id, name FROM users;
来源：http://ppd.shangyingyoupin.top

[Q17] 条件查询
来源：http://ivh.cdnleiting.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://urz.chenlongwang.top

[Q18] 模糊匹配
来源：http://bcm.hongshengwenyu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pyr.jianghu66.top

[Q19] 范围查询
来源：http://iwx.epnwcf.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://iye.uphjek.com

[Q20] IN 列表
来源：http://lss.zhoulong.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fkf.shanyushiyangkeji.top

[Q21] 空值判断
来源：http://vdb.ppjwa.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hgx.jlsjyb.cn

[Q22] 排序
来源：http://bxr.zhengqikj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hds.xingfuxueyuan.xyz

[Q23] 分页
来源：http://owt.zhaomingkeji.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tuy.jinyuanbaomall.cn

[Q24] 去重
来源：http://wqg.cqqwz.cn

SELECT DISTINCT city FROM users;
来源：http://rwf.fengsongda.top

[Q25] 只取前 N 条
来源：http://ofw.hysaishi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ahj.zdbjq.cn

[Q26] 计数
来源：http://gsz.jqgfzy.top

SELECT COUNT(*) FROM users;
来源：http://hpt.hnqzz.top

[Q27] 条件计数
来源：http://hgj.nanxinkj.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pju.chenjidiqi.icu

[Q28] 求和与平均
来源：http://bsy.nanxinkj.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://skr.xingfuxueyuan.xyz

[Q29] 最大最小值
来源：http://lot.dashuyun.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xof.hnqzz.top

[Q30] 分组统计
来源：http://zxs.zhixingplan.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://smd.shzxlz.cn

[Q31] 分组后过滤
来源：http://pyl.jinqigufen.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mfi.zycfv.cn

[Q32] 分组拼接字符串
来源：http://xdx.xuanzx.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lmo.yongpay.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pws.gzhubu.top

[Q33] 多列分组
来源：http://zaq.jinqigufen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ust.gzhubu.top

[Q34] 每组取第一条
来源：http://vfo.yonumen.top

SELECT * FROM (
来源：http://cpm.vehdjk.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nei.snrcjt.cn

) t WHERE rn = 1;
来源：http://ljo.hfpthk.cn

[Q35] 内连接
来源：http://fov.xylfe.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://luz.quarkkingdee.top

[Q36] 左连接
来源：http://btm.cheryme.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nvd.c1oappe.top

[Q37] 右连接
来源：http://qks.svipenyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dzv.gaohongyu789.top

[Q38] 全外连接（PostgreSQL）
来源：http://uls.hysaishi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bdr.tarul.cn

[Q39] 自连接（查上下级）
来源：http://dqf.bjfxy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://dtu.fzhhl.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jnh.hfpthk.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rqb.yanxiufei.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://whk.pycfn.com

[Q41] 多表连接
来源：http://glm.dianchejie.cn


<!-- 参考信息 -->