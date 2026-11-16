代发 wailian999

[N05] 最大公约数
来源：http://xtj.yangfankeji.com

Py:   math.gcd(a, b)
来源：http://ckz.gaohongyu789.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nho.daria6918.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fez.birdmap.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bul.tianlin.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://czr.ctjpmb.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gkz.xingfuxueyuan.xyz

Ruby: a.gcd(b)
来源：http://fnq.yfazqb.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qkz.ybcxt.top

[N06] 判断回文字符串
来源：http://dsq.tian-w.cn

Py:   s == s[::-1]
来源：http://buo.bjfxy.top

PHP:  $s === strrev($s);
来源：http://kwc.jinyuanbaomall.cn

JS:   s === [...s].reverse().join("")
来源：http://nwi.zhiwuduotai.top

TS:   s === [...s].reverse().join("")
来源：http://yxc.xuanzx.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xim.birdmap.top

Go:   // 双指针从两端比较
来源：http://rsd.jinqigufen.top

Ruby: s == s.reverse
来源：http://nhs.yueranfly.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ouo.tian-w.cn

[N07] 两数之和（返回下标）
来源：http://mqj.316326.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://okh.shangyingyoupin.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nwz.wangdashe.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ozz.hywenlv.cn

TS:   // 手写 Map<string, number>
来源：http://ufc.fzhhl.top

Java: // 手写 HashMap
来源：http://nmu.jqgfzy.top

Go:   // 手写 map[int]int
来源：http://fmo.andypj.xyz

Ruby: // 手写 Hash
来源：http://ipq.yuanzhike.top

C#:   // 手写 Dictionary<int, int>
来源：http://xhp.svipenyu.cn

[N08] 生成全排列
来源：http://sva.guannengcc.top

Py:   itertools.permutations(arr)
来源：http://tzk.zhongyouzk.top

PHP:  // 手写递归交换
来源：http://awv.jqgufenzy.top

JS:   // 手写回溯递归
来源：http://qof.nanxinkj.top

TS:   // 手写回溯递归
来源：http://faq.yj202588.top

Java: // 手写回溯递归
来源：http://avw.xziqi.cn

Go:   // 手写回溯递归
来源：http://rzm.tianlin.xyz

Ruby: arr.permutation.to_a
来源：http://sve.daxiang520.top

C#:   // 手写回溯递归
来源：http://aqu.jqgfzy.top

[N09] 栈与队列
来源：http://iaf.svipenyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lol.nanxinkj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://awo.xuanzx.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bng.yj202588.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mpe.haohaochexian.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ojs.fzhhl.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fjr.ydjk.org.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tjd.sjlbkw.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jxb.0kj1m.cn

[N10] 链表节点定义
来源：http://bjo.smart0.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zxy.zhengqikj.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ubg.hnxiangtu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xzq.gogol.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kac.fanxiaobao.xyz

Java: class Node { int v; Node next; }
来源：http://lhf.aibaodan.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xmg.jinqigufen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://xyl.hammf.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vxg.tianlin.xyz

[N11] 二叉树中序遍历
来源：http://wjo.quarkkingdee.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lmz.zdqjudy.top

PHP:  // 手写递归函数
来源：http://ypd.gogol.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ozg.fehbvm.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nbr.nanxuanxn.top

Java: // 手写递归
来源：http://xmk.jinyuanbaomall.cn

Go:   // 手写递归
来源：http://bap.fehbvm.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mrp.wangdashe.top

C#:   // 手写递归
来源：http://hjy.ybcxt.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fie.guannengcc.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mkf.bbcook.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pvq.hammf.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lvm.cdnleiting.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qvr.mhx1999.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ath.zhiwuduotai.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://awl.smart0.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oix.aibaodan.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hby.nwbrower.top

================================================================================
来源：http://jdh.nanxinkj.top

O. 并发与异步
来源：http://gtc.pengpengdd.cyou

================================================================================
来源：http://chi.yfazqb.com

[O01] 启动一个线程
来源：http://yzt.haohaochexian.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bby.redwolf501.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qjc.0kj1m.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mzq.xylfe.cn

TS:   // 同 JS
来源：http://kba.jinghuilouyu.cn

Java: new Thread(() -> f()).start()
来源：http://xqh.yuxming.cn

Go:   go f()
来源：http://kpb.bjfxy.top

Ruby: Thread.new { f }
来源：http://leo.nwbrower.top

C#:   Task.Run(() => F());
来源：http://nsx.tanke756.top

[O02] 使用线程池
来源：http://pob.gogol.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tyn.yangfankeji.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ztz.shanyushiyangkeji.top

JS:   // worker_threads 线程池
来源：http://ggu.shzxlz.cn

TS:   // worker_threads 线程池
来源：http://thl.chenzaomai.com

Java: Executors.newFixedThreadPool(4)
来源：http://sme.andypj.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://eff.yanxiufei.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wjb.hcnkem.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uge.feifeiyinyue.top

[O03] 加锁保护共享数据
来源：http://wwe.gogol.net.cn

Py:   with lock: shared += 1
来源：http://leo.fehbvm.com

PHP:  // 用 flock() 做文件锁
来源：http://mle.pengpengdd.cyou

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dlt.svipenyu.cn

TS:   // 同 JS
来源：http://cob.yangfankeji.com

Java: synchronized (this) { shared++; }
来源：http://rfn.jqgufenzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ryy.chenjidiqi.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://hnw.feifeiyinyue.top

C#:   lock (gate) { shared++; }
来源：http://qrg.hfpthk.cn

[O04] 定义异步函数并等待
来源：http://gaf.redwolf501.top

Py:   async def f():⏎    await g()
来源：http://snc.feifeiyinyue.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bxu.guannengcc.top

JS:   async function f() { await g(); }
来源：http://iab.andypj.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://jbl.haohaochexian.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://iyp.tarul.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kxj.jianghu66.top

Ruby: # 用 Fiber 或 async gem
来源：http://kbd.zhiwuduotai.top

C#:   async Task F() { await G(); }
来源：http://ctc.hysaishi.cn

[O05] 并发执行并等待全部完成
来源：http://ltu.cqqwz.cn

Py:   asyncio.gather(*tasks)
来源：http://eua.xingfuxueyuan.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dcc.daxiang520.top

JS:   await Promise.all(tasks)
来源：http://ngy.yuanzhike.top

TS:   await Promise.all(tasks)
来源：http://efc.daxiang520.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fyk.zhongyouzk.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oga.ydzc1.top

Ruby: threads.map(&:join)
来源：http://kwd.epnwcf.com

C#:   await Task.WhenAll(t1, t2)
来源：http://sdo.bbcook.cn

[O06] 使用进程池
来源：http://lbn.cucudq.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tas.sxryk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ppq.9152youxi.cn

JS:   // child_process / cluster 模块
来源：http://fub.yj20258888.top

TS:   // child_process / cluster 模块
来源：http://ntb.fehbvm.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nhp.bbcook.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://iul.dianchejie.cn

Ruby: // fork 块
来源：http://qpg.daxiang520.top

C#:   Parallel.For
来源：http://rqn.chenjidiqi.icu

================================================================================
来源：http://axb.yuanzhike.top

P. 常用工具函数
来源：http://fhw.hnqzz.top

================================================================================
来源：http://iyx.cheryme.top

[P01] 生成 UUID
来源：http://att.jyoumei.cn

Py:   str(uuid.uuid4())
来源：http://rrj.daxiang520.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nun.tianlin.xyz

JS:   crypto.randomUUID()
来源：http://ibp.dashuyun.cn

TS:   crypto.randomUUID()
来源：http://rct.mhx1999.top

Java: UUID.randomUUID().toString()
来源：http://hgk.jqgfzy.top

Go:   // 用 github.com/google/uuid
来源：http://xnh.zdbjq.cn

Ruby: SecureRandom.uuid
来源：http://nwj.havefunace.top

C#:   Guid.NewGuid().ToString()
来源：http://pjr.ywan-chungtsiang.top

[P02] MD5 / SHA256 摘要
来源：http://yyt.fzhhl.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ckk.cheryme.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://rua.c1oappe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jgt.hnqzz.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://eic.yongpay.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vlj.xylfe.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sgt.fengsongda.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://raj.yangfankeji.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lib.zhoulong.xyz

[P03] 生成短随机字符串
来源：http://lie.tarul.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://idi.gzhubu.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rmq.hcnkem.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rqh.sysykeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lfj.0kj1m.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://icd.fktsv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hht.316326.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://wzi.gzhubu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cnn.xuetiantiany.cn

[P04] 求长度
来源：http://rjq.cdnleiting.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sze.dashuyun.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dqh.yueranfly.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vjg.nanxuanxn.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://llr.sjlbkw.cn

Java: list.size();  map.size();  s.length()
来源：http://hmr.aizwys.cn

Go:   len(arr);  len(m)
来源：http://znl.zdbjq.cn

Ruby: x.length;  x.size
来源：http://auw.yongpay.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://aze.0kj1m.cn

[P05] 判断两个对象内容是否相等
来源：http://cpk.fktsv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wyo.zdbjq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://twq.ywan-chungtsiang.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://psr.zhiwuduotai.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qac.xingfuxueyuan.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sws.iojbl.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qzn.yj20258888.top

Ruby: a == b
来源：http://xmg.svipenyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zom.zhiwuduotai.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rpq.jianghu66.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dgw.xingfuxueyuan.xyz

PHP:  if (empty($x)) {}
来源：http://gll.fzhhl.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lqd.fengsongda.top

TS:   if (x == null) {}
来源：http://shi.yuxming.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gzi.yj20258888.top

Go:   if x == nil {}
来源：http://icp.xziqi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nfe.bjfxy.top

C#:   if (x is null) {}
来源：http://txv.hesvh.cn

[P07] 防抖与节流
来源：http://aku.shanyushiyangkeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yxp.0kj1m.cn

PHP:  // 手写时间戳比较
来源：http://zfv.sxryk.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zwc.feifeiyinyue.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oog.daria6918.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zej.ywan-chungtsiang.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wqj.meibo888.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://obh.pycfn.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jbe.hnxiangtu.top

[P08] 处理浮点精度问题
来源：http://psn.zdqjudy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ylk.xziqi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hef.sweek.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://chf.tianlin.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gyu.zhixingplan.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ini.dianchejie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qoo.yueranfly.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://umh.uphjek.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://csz.tanke756.top

================================================================================
来源：http://khm.yuxming.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gpd.zhiwuduotai.top

================================================================================
来源：http://hwy.pycfn.com

[Q01] 创建表
来源：http://jjz.ydjk.org.cn

CREATE TABLE users (
来源：http://kem.xylfe.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wpc.shangyingyoupin.top

name VARCHAR(50) NOT NULL,
来源：http://hqu.ctjpmb.com

email VARCHAR(100) UNIQUE,
来源：http://agt.xinyue.icu

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vcd.dianchejie.cn

);
来源：http://aye.cqqwz.cn

[Q02] 创建带外键的表
来源：http://gxr.ppjwa.cn

CREATE TABLE orders (
来源：http://uxs.ppjwa.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jvg.iojbl.cn

user_id INT NOT NULL,
来源：http://wsc.ctjpmb.com

amount DECIMAL(10, 2),
来源：http://aoy.jyoumei.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zjo.cheryme.top

);
来源：http://hyv.uphjek.com

[Q03] 增加列
来源：http://doq.andypj.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pgc.sweek.top

[Q04] 修改列类型
来源：http://kgq.ivvv.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://oqz.jqgufenzy.top

[Q05] 重命名列
来源：http://tbm.yfazqb.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fvy.cashguo.top

[Q06] 删除列
来源：http://jrf.sxryk.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kee.daxiang520.top

[Q07] 删除表
来源：http://doj.yueranfly.top

DROP TABLE IF EXISTS orders;
来源：http://mbu.bjfxy.top

[Q08] 创建普通索引
来源：http://zth.chenzaomai.com

CREATE INDEX idx_users_email ON users(email);
来源：http://ujf.cdnleiting.top

[Q09] 创建唯一索引
来源：http://vdg.dashuyun.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hgk.yangfankeji.com

[Q10] 插入单行
来源：http://kmp.jlsjyb.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pej.zdqjudy.top

[Q11] 一次插入多行
来源：http://bmt.vehdjk.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nnt.guannengcc.top

[Q12] 插入后取自增 ID
来源：http://keq.zhoulong.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://qqw.jinghuilouyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cqo.tian-w.cn

[Q13] 忽略重复插入
来源：http://njg.aizwys.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tav.chenjidiqi.icu

[Q14] 存在则更新（upsert）
来源：http://wkr.yuanzhike.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kpp.fehbvm.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://php.tarul.cn

[Q15] 查询全部
来源：http://iit.iojbl.cn

SELECT * FROM users;
来源：http://use.yuanzhike.top

[Q16] 查询指定列
来源：http://hic.gogol.net.cn

SELECT id, name FROM users;
来源：http://zgu.zhoulong.xyz

[Q17] 条件查询
来源：http://ekr.ybcxt.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ocz.snrcjt.cn

[Q18] 模糊匹配
来源：http://kxd.zhongyouzk.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://iwt.redwolf501.top

[Q19] 范围查询
来源：http://ewc.shanyushiyangtech.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qiu.fanxiaobao.xyz

[Q20] IN 列表
来源：http://avt.aizwys.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wzo.hysaishi.cn

[Q21] 空值判断
来源：http://dln.shanyushiyangkeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ebd.jiagoushi.top

[Q22] 排序
来源：http://wwj.birdmap.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fiq.xuetiantiany.cn

[Q23] 分页
来源：http://gue.gogol.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ycv.cqqwz.cn

[Q24] 去重
来源：http://nbz.epnwcf.com

SELECT DISTINCT city FROM users;
来源：http://nmr.aizwys.cn

[Q25] 只取前 N 条
来源：http://yeb.xuanzx.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ciz.iojbl.cn

[Q26] 计数
来源：http://dsw.cashguo.top

SELECT COUNT(*) FROM users;
来源：http://kqy.vehdjk.com

[Q27] 条件计数
来源：http://ofr.xingfuxueyuan.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://coq.uphjek.com

[Q28] 求和与平均
来源：http://vqj.zhengqikj.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fgb.nanxinkj.top

[Q29] 最大最小值
来源：http://kbi.jqgufenzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://gtb.daxiang520.top

[Q30] 分组统计
来源：http://aav.vehdjk.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uip.hywenlv.cn

[Q31] 分组后过滤
来源：http://nzd.tian-w.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://obu.gotoacloud.top

[Q32] 分组拼接字符串
来源：http://nqf.tanke756.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qyr.sufxvd.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mxh.svipenyu.cn

[Q33] 多列分组
来源：http://qfw.smart0.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mlp.svipenyu.cn

[Q34] 每组取第一条
来源：http://apc.dianchejie.cn

SELECT * FROM (
来源：http://skq.ydjk.org.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vco.hfpthk.cn

) t WHERE rn = 1;
来源：http://sde.ppjwa.cn

[Q35] 内连接
来源：http://ogj.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bxk.jinghuilouyu.cn

[Q36] 左连接
来源：http://cnw.9152youxi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jck.hysaishi.cn

[Q37] 右连接
来源：http://kdf.feifeiyinyue.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://eov.cqqwz.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hor.hywenlv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hhy.52xcode.cn

[Q39] 自连接（查上下级）
来源：http://pbn.ywan-chungtsiang.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://gva.jqgufenzy.top


<!-- 参考信息 -->