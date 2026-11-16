代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fxa.bbcook.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://evy.fktsv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jcr.sufxvd.cn

Ruby: a.gcd(b)
来源：http://fpd.tian-w.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cjq.yj202588.top

[N06] 判断回文字符串
来源：http://yot.ybcxt.top

Py:   s == s[::-1]
来源：http://maa.shangyingyoupin.top

PHP:  $s === strrev($s);
来源：http://vfu.yj20258.top

JS:   s === [...s].reverse().join("")
来源：http://bfn.guannengcc.top

TS:   s === [...s].reverse().join("")
来源：http://nrh.fehbvm.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://orq.0kj1m.cn

Go:   // 双指针从两端比较
来源：http://uts.cqqwz.cn

Ruby: s == s.reverse
来源：http://wrw.xinyue.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://rxu.havefunace.top

[N07] 两数之和（返回下标）
来源：http://abu.hcnkem.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pjc.daria6918.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ivp.bbcook.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://faf.guowangkeji.top

TS:   // 手写 Map<string, number>
来源：http://ult.epnwcf.com

Java: // 手写 HashMap
来源：http://pai.jqgufenzy.top

Go:   // 手写 map[int]int
来源：http://jsh.yfazqb.com

Ruby: // 手写 Hash
来源：http://zwy.tianlin.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://ciu.316326.xyz

[N08] 生成全排列
来源：http://gsr.gaohongyu789.top

Py:   itertools.permutations(arr)
来源：http://azv.316326.xyz

PHP:  // 手写递归交换
来源：http://mav.bjfxy.top

JS:   // 手写回溯递归
来源：http://hsf.feifeiyinyue.top

TS:   // 手写回溯递归
来源：http://inn.shangyingyoupin.top

Java: // 手写回溯递归
来源：http://lex.hfpthk.cn

Go:   // 手写回溯递归
来源：http://qaw.havefunace.top

Ruby: arr.permutation.to_a
来源：http://bic.aibaodan.cn

C#:   // 手写回溯递归
来源：http://vwr.jiagoushi.top

[N09] 栈与队列
来源：http://yll.fehbvm.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dvk.ydjk.org.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://eiw.tarul.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wum.jlsjyb.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dfp.jinyuanbaomall.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rhx.jinqigfzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tiw.sufxvd.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mls.daxiang520.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vxk.quarkkingdee.top

[N10] 链表节点定义
来源：http://ank.tarul.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ttj.cucudq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sod.zdqjudy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rjr.hywenlv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zbz.havefunace.top

Java: class Node { int v; Node next; }
来源：http://cli.birdmap.top

Go:   type Node struct { V int; Next *Node }
来源：http://hhl.jqgufenzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://vgt.sxryk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xkl.hysaishi.cn

[N11] 二叉树中序遍历
来源：http://luo.fzhhl.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tzn.shanyushiyangkeji.top

PHP:  // 手写递归函数
来源：http://cxe.epnwcf.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hlh.quarkkingdee.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kxf.aibaodan.cn

Java: // 手写递归
来源：http://vdb.sjlbkw.cn

Go:   // 手写递归
来源：http://lzk.epnwcf.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pug.jyoumei.cn

C#:   // 手写递归
来源：http://agz.sjlbkw.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ayn.dashuyun.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sni.fehbvm.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hkf.aibaodan.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hrm.cashguo.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bii.xylfe.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fcv.nwbrower.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://igp.redwolf501.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gsv.hywenlv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xdv.9152youxi.cn

================================================================================
来源：http://cje.zdqjudy.top

O. 并发与异步
来源：http://fkr.jinqigufen.top

================================================================================
来源：http://vgx.yvedp.cn

[O01] 启动一个线程
来源：http://nlv.fzhhl.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kct.shanyushiyangtech.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hda.yuxming.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vzz.yangfankeji.com

TS:   // 同 JS
来源：http://rgy.ctjpmb.com

Java: new Thread(() -> f()).start()
来源：http://dbx.zhengqikj.top

Go:   go f()
来源：http://yie.smart0.xyz

Ruby: Thread.new { f }
来源：http://ogj.316326.xyz

C#:   Task.Run(() => F());
来源：http://qeh.ehwqpu.com

[O02] 使用线程池
来源：http://shy.aizwys.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ylh.yj20258888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sbr.yfazqb.com

JS:   // worker_threads 线程池
来源：http://wcv.vqdsnc.cn

TS:   // worker_threads 线程池
来源：http://kea.zhaomingkeji.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://nol.hysaishi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rax.andypj.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://anv.fehbvm.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://znm.meibo888.top

[O03] 加锁保护共享数据
来源：http://kut.52xcode.cn

Py:   with lock: shared += 1
来源：http://bpj.0kj1m.cn

PHP:  // 用 flock() 做文件锁
来源：http://xax.feifeiyinyue.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://htz.xuanzx.com

TS:   // 同 JS
来源：http://obh.jinqigfzy.top

Java: synchronized (this) { shared++; }
来源：http://beg.jqgufenzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nhv.uphjek.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://xpw.chenlongwang.top

C#:   lock (gate) { shared++; }
来源：http://ind.yongpay.top

[O04] 定义异步函数并等待
来源：http://cjo.tianlin.xyz

Py:   async def f():⏎    await g()
来源：http://oiz.shanyushiyangtech.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bpy.shuidangran.top

JS:   async function f() { await g(); }
来源：http://kib.dashuyun.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kgc.xziqi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wfy.xuanzx.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mfq.yongpay.top

Ruby: # 用 Fiber 或 async gem
来源：http://kkf.ywan-chungtsiang.top

C#:   async Task F() { await G(); }
来源：http://twv.jiagoushi.top

[O05] 并发执行并等待全部完成
来源：http://igx.iojbl.cn

Py:   asyncio.gather(*tasks)
来源：http://cbf.jqgfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uad.sufxvd.cn

JS:   await Promise.all(tasks)
来源：http://fmd.aibaodan.cn

TS:   await Promise.all(tasks)
来源：http://ecm.ydjk.org.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iwe.chenzaomai.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tyl.xuanzx.com

Ruby: threads.map(&:join)
来源：http://lhl.havefunace.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fqp.gogol.net.cn

[O06] 使用进程池
来源：http://cfz.hfpthk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qmq.jinqigfzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://jcz.zhaomingkeji.xyz

JS:   // child_process / cluster 模块
来源：http://hme.pycfn.com

TS:   // child_process / cluster 模块
来源：http://ttp.iojbl.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tls.pengpengdd.cyou

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xqp.redwolf501.top

Ruby: // fork 块
来源：http://hgk.zhixingplan.top

C#:   Parallel.For
来源：http://xhu.ydjk.org.cn

================================================================================
来源：http://yzg.yfazqb.com

P. 常用工具函数
来源：http://wms.zdqjudy.top

================================================================================
来源：http://svc.zhengqikj.top

[P01] 生成 UUID
来源：http://scn.bjfxy.top

Py:   str(uuid.uuid4())
来源：http://rpc.zdqjudy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cxy.feifeiyinyue.top

JS:   crypto.randomUUID()
来源：http://pqr.havefunace.top

TS:   crypto.randomUUID()
来源：http://fia.tarul.cn

Java: UUID.randomUUID().toString()
来源：http://mke.dianchejie.cn

Go:   // 用 github.com/google/uuid
来源：http://fsk.jinyuanbaomall.cn

Ruby: SecureRandom.uuid
来源：http://fhz.52xcode.cn

C#:   Guid.NewGuid().ToString()
来源：http://rfm.wangdashe.top

[P02] MD5 / SHA256 摘要
来源：http://vxi.haohaochexian.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rvt.9152youxi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://atx.bbcook.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xsi.hysaishi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vrn.jinqigufen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hiq.ehwqpu.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wzb.ctjpmb.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tml.gogol.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hbc.zhengqikj.top

[P03] 生成短随机字符串
来源：http://njt.shangyingyoupin.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hsw.9152youxi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rmv.jlsjyb.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yhd.epnwcf.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ssw.ctjpmb.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://far.vqdsnc.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ijz.hnxiangtu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://bxk.cucudq.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://buq.zdbjq.cn

[P04] 求长度
来源：http://vyo.tianlin.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gcz.jqgufenzy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mrw.bjfxy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rkg.gzhubu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vqj.yuxming.cn

Java: list.size();  map.size();  s.length()
来源：http://hgz.cheryme.top

Go:   len(arr);  len(m)
来源：http://eae.ctjpmb.com

Ruby: x.length;  x.size
来源：http://cnx.gzhubu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://app.zhoulong.xyz

[P05] 判断两个对象内容是否相等
来源：http://tzz.cheryme.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://avz.ivvv.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://eub.0kj1m.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://khp.guannengcc.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ghd.hnqzz.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sxe.tian-w.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ayo.yvedp.cn

Ruby: a == b
来源：http://udj.zhiwuduotai.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rvg.zdbjq.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lgh.zhongyouzk.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://eoa.pengpengdd.cyou

PHP:  if (empty($x)) {}
来源：http://chx.tianlin.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fzn.wangdashe.top

TS:   if (x == null) {}
来源：http://hwc.shanyushiyangkeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://qff.fktsv.cn

Go:   if x == nil {}
来源：http://quq.fehbvm.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wbv.cdnleiting.top

C#:   if (x is null) {}
来源：http://kpg.jyoumei.cn

[P07] 防抖与节流
来源：http://jof.ivvv.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lgx.ydjk.org.cn

PHP:  // 手写时间戳比较
来源：http://bqf.zdqjudy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://roz.aibaodan.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qzi.xuetiantiany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gjs.wangshuangyany.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hzm.gogol.net.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://eth.hnqzz.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ddz.yj20258888.top

[P08] 处理浮点精度问题
来源：http://djq.yonumen.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lgm.xylfe.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ajz.c1oappe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lha.316326.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vbk.pycfn.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vua.tian-w.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rpn.zhaomingkeji.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://eey.jinghuilouyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rop.yanxiufei.cn

================================================================================
来源：http://xgv.gaohongyu789.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nvz.dianchejie.cn

================================================================================
来源：http://nvf.zhijiandao.cn

[Q01] 创建表
来源：http://qxi.havefunace.top

CREATE TABLE users (
来源：http://rjq.gaohongyu789.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bvk.ivvv.top

name VARCHAR(50) NOT NULL,
来源：http://kha.aibaodan.cn

email VARCHAR(100) UNIQUE,
来源：http://ozo.cqqwz.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vzl.chenjidiqi.icu

);
来源：http://lle.cdnleiting.top

[Q02] 创建带外键的表
来源：http://pux.zhaomingkeji.xyz

CREATE TABLE orders (
来源：http://nrp.shanyushiyangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kqi.jyoumei.cn

user_id INT NOT NULL,
来源：http://xni.yj202588.top

amount DECIMAL(10, 2),
来源：http://mxi.chenlongwang.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yoi.meibo888.top

);
来源：http://rsp.ivvv.top

[Q03] 增加列
来源：http://zds.cheryme.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kis.yongpay.top

[Q04] 修改列类型
来源：http://mfc.haohaochexian.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kiu.hysaishi.cn

[Q05] 重命名列
来源：http://bpx.nanxuanxn.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bbe.feifeiyinyue.top

[Q06] 删除列
来源：http://sbg.gotoacloud.top

ALTER TABLE users DROP COLUMN age;
来源：http://ddc.fengsongda.top

[Q07] 删除表
来源：http://the.jyoumei.cn

DROP TABLE IF EXISTS orders;
来源：http://efh.guowangkeji.top

[Q08] 创建普通索引
来源：http://hxj.fehbvm.com

CREATE INDEX idx_users_email ON users(email);
来源：http://vyy.316326.xyz

[Q09] 创建唯一索引
来源：http://sll.dianchejie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wlk.bbcook.cn

[Q10] 插入单行
来源：http://bvx.cucudq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nuu.sxryk.cn

[Q11] 一次插入多行
来源：http://hqb.fktsv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://swh.yvedp.cn

[Q12] 插入后取自增 ID
来源：http://pgr.daria6918.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ndz.epnwcf.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mtw.ydzc1.top

[Q13] 忽略重复插入
来源：http://drd.xinyue.icu

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hkx.xylfe.cn

[Q14] 存在则更新（upsert）
来源：http://gkx.yueranfly.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fkc.vqdsnc.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lku.guowangkeji.top

[Q15] 查询全部
来源：http://qug.yanxiufei.cn

SELECT * FROM users;
来源：http://mvu.zhijiandao.cn

[Q16] 查询指定列
来源：http://gto.jinghuilouyu.cn

SELECT id, name FROM users;
来源：http://wra.fzhhl.top

[Q17] 条件查询
来源：http://dek.chenzaomai.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fxx.ydjk.org.cn

[Q18] 模糊匹配
来源：http://edy.daria6918.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zbv.zhijiandao.cn

[Q19] 范围查询
来源：http://zgt.c1oappe.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qar.ivvv.top

[Q20] IN 列表
来源：http://goj.epnwcf.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pks.tanke756.top

[Q21] 空值判断
来源：http://tph.zdbjq.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zfr.9152youxi.cn

[Q22] 排序
来源：http://wyd.hfpthk.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://efs.havefunace.top

[Q23] 分页
来源：http://uwq.zhiwuduotai.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ask.xingfuxueyuan.xyz

[Q24] 去重
来源：http://fps.yongpay.top

SELECT DISTINCT city FROM users;
来源：http://tdl.tarul.cn

[Q25] 只取前 N 条
来源：http://xhs.jinqigufen.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hrl.gogol.net.cn

[Q26] 计数
来源：http://hfy.gzhubu.top

SELECT COUNT(*) FROM users;
来源：http://enq.yj20258888.top

[Q27] 条件计数
来源：http://wlv.wangshuangyany.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mdl.yj202588.top

[Q28] 求和与平均
来源：http://bks.hnqzz.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pho.ivvv.top

[Q29] 最大最小值
来源：http://egk.jqgfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://kcw.yueranfly.top

[Q30] 分组统计
来源：http://ekz.0kj1m.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mij.cqqwz.cn

[Q31] 分组后过滤
来源：http://izh.xziqi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wdi.feifeiyinyue.top

[Q32] 分组拼接字符串
来源：http://wmg.quarkkingdee.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://aoa.hcnkem.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tco.chenlongwang.top

[Q33] 多列分组
来源：http://tqg.ppjwa.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bnn.mhx1999.top

[Q34] 每组取第一条
来源：http://oql.bbcook.cn

SELECT * FROM (
来源：http://cqs.yonumen.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jkp.iojbl.cn

) t WHERE rn = 1;
来源：http://dqs.kuanghao11.cn

[Q35] 内连接
来源：http://yrz.yuxming.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gmc.xingfuxueyuan.xyz

[Q36] 左连接
来源：http://mkp.dashuyun.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ptx.fktsv.cn

[Q37] 右连接
来源：http://gtn.hongshengwenyu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wie.xingfuxueyuan.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://zuk.zdbjq.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qqc.mhx1999.top

[Q39] 自连接（查上下级）
来源：http://cdu.zhixingplan.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rei.wangdashe.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qgg.yanxiufei.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pht.shanyushiyangkeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kzk.tanke756.top

[Q41] 多表连接
来源：http://gsv.zhijiandao.cn


<!-- 参考信息 -->