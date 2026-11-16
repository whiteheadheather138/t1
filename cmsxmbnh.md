代发 wailian999

[N05] 最大公约数
来源：http://jgp.cheryme.top

Py:   math.gcd(a, b)
来源：http://tle.gaohongyu789.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://van.9152youxi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ism.ydzc1.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://csw.yuxming.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kxg.chenzaomai.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gyg.ydjk.org.cn

Ruby: a.gcd(b)
来源：http://ivn.gotoacloud.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ibr.cqqwz.cn

[N06] 判断回文字符串
来源：http://zjb.hcnkem.com

Py:   s == s[::-1]
来源：http://fug.zhijiandao.cn

PHP:  $s === strrev($s);
来源：http://nth.sjlbkw.cn

JS:   s === [...s].reverse().join("")
来源：http://imf.epnwcf.com

TS:   s === [...s].reverse().join("")
来源：http://thu.zhijiandao.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ptz.zhoulong.xyz

Go:   // 双指针从两端比较
来源：http://yzo.ivvv.top

Ruby: s == s.reverse
来源：http://imv.aibaodan.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://wgy.andypj.xyz

[N07] 两数之和（返回下标）
来源：http://ppz.yj20258.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fuh.yj202588.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fpo.zhiwuduotai.top

JS:   // 手写 Map：map.set(v, i)
来源：http://fuy.yfazqb.com

TS:   // 手写 Map<string, number>
来源：http://uui.hesvh.cn

Java: // 手写 HashMap
来源：http://cos.ehwqpu.com

Go:   // 手写 map[int]int
来源：http://zpi.hammf.cn

Ruby: // 手写 Hash
来源：http://jie.sysykeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://pqq.kuanghao11.cn

[N08] 生成全排列
来源：http://lbi.gogol.net.cn

Py:   itertools.permutations(arr)
来源：http://yhs.cashguo.top

PHP:  // 手写递归交换
来源：http://uaj.aizwys.cn

JS:   // 手写回溯递归
来源：http://yjx.nwbrower.top

TS:   // 手写回溯递归
来源：http://awd.meibo888.top

Java: // 手写回溯递归
来源：http://dzx.vehdjk.com

Go:   // 手写回溯递归
来源：http://ttc.zdqjudy.top

Ruby: arr.permutation.to_a
来源：http://vhp.fzhhl.top

C#:   // 手写回溯递归
来源：http://prt.iojbl.cn

[N09] 栈与队列
来源：http://mjm.xinyue.icu

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pbe.cdnleiting.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://muy.9152youxi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cyr.jlsjyb.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://svs.ehwqpu.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jog.xziqi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gzj.yuxming.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fio.hysaishi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oqh.ybcxt.top

[N10] 链表节点定义
来源：http://jhe.kuanghao11.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://aqy.shanyushiyangkeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://jmg.yanxiufei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ehv.xingfuxueyuan.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lzu.yj202588.top

Java: class Node { int v; Node next; }
来源：http://noq.snrcjt.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vuh.hammf.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://llg.fengsongda.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tnb.jinqigfzy.top

[N11] 二叉树中序遍历
来源：http://tzz.tanke756.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kft.xuanzx.com

PHP:  // 手写递归函数
来源：http://tlv.svipenyu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://njr.pycfn.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://abm.316326.xyz

Java: // 手写递归
来源：http://ncr.chenzaomai.com

Go:   // 手写递归
来源：http://zmj.yanxiufei.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hvu.zdqjudy.top

C#:   // 手写递归
来源：http://llg.tarul.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://owv.meibo888.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://imq.vqdsnc.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zvj.epnwcf.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qhh.vehdjk.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wdl.shzxlz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dlm.epnwcf.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tmg.jqgfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ftl.fengsongda.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hzz.yj20258.top

================================================================================
来源：http://fep.pycfn.com

O. 并发与异步
来源：http://fge.hywenlv.cn

================================================================================
来源：http://say.yfazqb.com

[O01] 启动一个线程
来源：http://grn.52xcode.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uvc.chenzaomai.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://syo.uphjek.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ffd.wangdashe.top

TS:   // 同 JS
来源：http://qol.yueranfly.top

Java: new Thread(() -> f()).start()
来源：http://hjx.pengpengdd.cyou

Go:   go f()
来源：http://mrh.pycfn.com

Ruby: Thread.new { f }
来源：http://bbm.svipenyu.cn

C#:   Task.Run(() => F());
来源：http://ylj.cqqwz.cn

[O02] 使用线程池
来源：http://klg.fanxiaobao.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nrx.316326.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://npe.zdqjudy.top

JS:   // worker_threads 线程池
来源：http://ddo.zhengqikj.top

TS:   // worker_threads 线程池
来源：http://urn.yanxiufei.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bex.hysaishi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yjg.jiagoushi.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wrg.uphjek.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uaw.hywenlv.cn

[O03] 加锁保护共享数据
来源：http://xiv.jinqigufen.top

Py:   with lock: shared += 1
来源：http://dbf.yj202588.top

PHP:  // 用 flock() 做文件锁
来源：http://mkz.havefunace.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qug.vehdjk.com

TS:   // 同 JS
来源：http://qmj.guowangkeji.top

Java: synchronized (this) { shared++; }
来源：http://jkz.hywenlv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://spz.dashuyun.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://uep.daria6918.cn

C#:   lock (gate) { shared++; }
来源：http://wck.cashguo.top

[O04] 定义异步函数并等待
来源：http://dkt.ppjwa.cn

Py:   async def f():⏎    await g()
来源：http://zti.xingfuxueyuan.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nfn.cucudq.cn

JS:   async function f() { await g(); }
来源：http://dvk.ppjwa.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qdc.tanke756.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://syu.ctjpmb.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hqg.dashuyun.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mzw.meibo888.top

C#:   async Task F() { await G(); }
来源：http://koj.ivvv.top

[O05] 并发执行并等待全部完成
来源：http://jup.hammf.cn

Py:   asyncio.gather(*tasks)
来源：http://dtb.fanxiaobao.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rke.shzxlz.cn

JS:   await Promise.all(tasks)
来源：http://ckn.zhijiandao.cn

TS:   await Promise.all(tasks)
来源：http://vpf.tianlin.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ixi.xinyue.icu

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yxu.havefunace.top

Ruby: threads.map(&:join)
来源：http://iby.yuanzhike.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fxh.ywan-chungtsiang.top

[O06] 使用进程池
来源：http://azw.jlsjyb.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wdd.wangshuangyany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bfw.meibo888.top

JS:   // child_process / cluster 模块
来源：http://qqp.aizwys.cn

TS:   // child_process / cluster 模块
来源：http://nbz.snrcjt.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jpp.hammf.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qun.tian-w.cn

Ruby: // fork 块
来源：http://apt.xuanzx.com

C#:   Parallel.For
来源：http://mfe.wangshuangyany.cn

================================================================================
来源：http://gjm.fanxiaobao.xyz

P. 常用工具函数
来源：http://kiw.snrcjt.cn

================================================================================
来源：http://cvg.dianchejie.cn

[P01] 生成 UUID
来源：http://kqy.cucudq.cn

Py:   str(uuid.uuid4())
来源：http://sin.xuanzx.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://owt.quarkkingdee.top

JS:   crypto.randomUUID()
来源：http://cgd.havefunace.top

TS:   crypto.randomUUID()
来源：http://eir.ivvv.top

Java: UUID.randomUUID().toString()
来源：http://ler.dianchejie.cn

Go:   // 用 github.com/google/uuid
来源：http://kdt.yfazqb.com

Ruby: SecureRandom.uuid
来源：http://qkq.ehwqpu.com

C#:   Guid.NewGuid().ToString()
来源：http://wju.wangshuangyany.cn

[P02] MD5 / SHA256 摘要
来源：http://zwl.ywan-chungtsiang.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://eqs.hnxiangtu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://uuq.vehdjk.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sra.shangyingyoupin.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ewc.chenlongwang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://afc.xuetiantiany.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dph.zhongyouzk.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ynj.vqdsnc.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ftx.shangyingyoupin.top

[P03] 生成短随机字符串
来源：http://jff.zhongyouzk.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qkx.tanke756.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://afm.ctjpmb.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://trs.yuanzhike.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lej.tianlin.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ybc.vehdjk.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hbq.jinyuanbaomall.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rzq.meibo888.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ycs.yvedp.cn

[P04] 求长度
来源：http://lyd.hywenlv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mit.meibo888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hao.vqdsnc.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fud.xuanzx.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gle.9152youxi.cn

Java: list.size();  map.size();  s.length()
来源：http://irs.tian-w.cn

Go:   len(arr);  len(m)
来源：http://ohu.sysykeji.top

Ruby: x.length;  x.size
来源：http://zuu.daria6918.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pcl.yueranfly.top

[P05] 判断两个对象内容是否相等
来源：http://bbj.ctjpmb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://dtb.epnwcf.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://okx.epnwcf.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://oen.hysaishi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ibo.yonumen.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gjt.gotoacloud.top

Go:   reflect.DeepEqual(a, b)
来源：http://uab.vqdsnc.cn

Ruby: a == b
来源：http://svr.cashguo.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://quo.fengsongda.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uje.fktsv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tqv.cashguo.top

PHP:  if (empty($x)) {}
来源：http://ivt.zycfv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ped.zhiwuduotai.top

TS:   if (x == null) {}
来源：http://pnl.hywenlv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://way.hnqzz.top

Go:   if x == nil {}
来源：http://ckx.kuanghao11.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wfp.xuetiantiany.cn

C#:   if (x is null) {}
来源：http://owi.zhiwuduotai.top

[P07] 防抖与节流
来源：http://qhu.guannengcc.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lgi.shuidangran.top

PHP:  // 手写时间戳比较
来源：http://sqx.hcnkem.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ann.ehwqpu.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lnc.nwbrower.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zve.hammf.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vfp.zdqjudy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ups.hywenlv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vth.shzxlz.cn

[P08] 处理浮点精度问题
来源：http://nlj.aizwys.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jol.zhiwuduotai.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vyp.bjfxy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://njn.wangshuangyany.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ytk.ivvv.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jsx.ywan-chungtsiang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://byh.ydjk.org.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dcg.nwbrower.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mgo.havefunace.top

================================================================================
来源：http://fih.xziqi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cry.ydjk.org.cn

================================================================================
来源：http://tev.wangdashe.top

[Q01] 创建表
来源：http://ren.snrcjt.cn

CREATE TABLE users (
来源：http://efo.yfazqb.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ymx.hcnkem.com

name VARCHAR(50) NOT NULL,
来源：http://vmx.zdbjq.cn

email VARCHAR(100) UNIQUE,
来源：http://cja.yfazqb.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jmf.xinyue.icu

);
来源：http://lii.gzhubu.top

[Q02] 创建带外键的表
来源：http://epa.ehwqpu.com

CREATE TABLE orders (
来源：http://bcu.jlsjyb.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://abn.yongpay.top

user_id INT NOT NULL,
来源：http://gbp.smart0.xyz

amount DECIMAL(10, 2),
来源：http://acg.gogol.net.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rlw.jinyuanbaomall.cn

);
来源：http://isc.yvedp.cn

[Q03] 增加列
来源：http://rts.meibo888.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ikz.tarul.cn

[Q04] 修改列类型
来源：http://uss.yongpay.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yee.sufxvd.cn

[Q05] 重命名列
来源：http://xun.sxryk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://btg.zhongyouzk.top

[Q06] 删除列
来源：http://chu.haohaochexian.top

ALTER TABLE users DROP COLUMN age;
来源：http://mhu.0kj1m.cn

[Q07] 删除表
来源：http://usq.gaohongyu789.top

DROP TABLE IF EXISTS orders;
来源：http://pha.sxryk.cn

[Q08] 创建普通索引
来源：http://jeh.zycfv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rpe.chenlongwang.top

[Q09] 创建唯一索引
来源：http://bjs.ydzc1.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nji.yanxiufei.cn

[Q10] 插入单行
来源：http://xyu.chenjidiqi.icu

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://psu.jinyuanbaomall.cn

[Q11] 一次插入多行
来源：http://tml.sxryk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://buq.wangdashe.top

[Q12] 插入后取自增 ID
来源：http://ojg.epnwcf.com

INSERT INTO users (name) VALUES ('C');
来源：http://pru.uphjek.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wem.zdbjq.cn

[Q13] 忽略重复插入
来源：http://drb.svipenyu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://arw.chenlongwang.top

[Q14] 存在则更新（upsert）
来源：http://gph.zhixingplan.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jby.cucudq.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kzg.zhengqikj.top

[Q15] 查询全部
来源：http://bdu.shangyingyoupin.top

SELECT * FROM users;
来源：http://ctv.feifeiyinyue.top

[Q16] 查询指定列
来源：http://urp.zhixingplan.top

SELECT id, name FROM users;
来源：http://mwg.haohaochexian.top

[Q17] 条件查询
来源：http://zdb.yueranfly.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ycc.guannengcc.top

[Q18] 模糊匹配
来源：http://wgg.daxiang520.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sos.fktsv.cn

[Q19] 范围查询
来源：http://urb.cucudq.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hqh.sjlbkw.cn

[Q20] IN 列表
来源：http://uoq.jinghuilouyu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kco.gotoacloud.top

[Q21] 空值判断
来源：http://gmq.hammf.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mgo.bjfxy.top

[Q22] 排序
来源：http://kjx.sysykeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sgm.sjlbkw.cn

[Q23] 分页
来源：http://nxw.jqgfzy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oup.cdnleiting.top

[Q24] 去重
来源：http://ycg.wangshuangyany.cn

SELECT DISTINCT city FROM users;
来源：http://flp.ivvv.top

[Q25] 只取前 N 条
来源：http://vdd.yvedp.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hcy.yfazqb.com

[Q26] 计数
来源：http://sxr.c1oappe.top

SELECT COUNT(*) FROM users;
来源：http://hmh.gogol.net.cn

[Q27] 条件计数
来源：http://xrf.zhoulong.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qdi.xinyue.icu

[Q28] 求和与平均
来源：http://ywv.yonumen.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xqn.sxryk.cn

[Q29] 最大最小值
来源：http://hhw.hywenlv.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vwb.kuanghao11.cn

[Q30] 分组统计
来源：http://gpq.tanke756.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ors.jqgufenzy.top

[Q31] 分组后过滤
来源：http://ote.yuxming.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bow.jinqigufen.top

[Q32] 分组拼接字符串
来源：http://vlr.52xcode.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jvx.chenzaomai.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uus.hysaishi.cn

[Q33] 多列分组
来源：http://ovd.yuanzhike.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://scf.shanyushiyangkeji.top

[Q34] 每组取第一条
来源：http://lbu.jlsjyb.cn

SELECT * FROM (
来源：http://zut.jinyuanbaomall.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jxs.xziqi.cn

) t WHERE rn = 1;
来源：http://awb.jinyuanbaomall.cn

[Q35] 内连接
来源：http://hyg.ybcxt.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://twa.sweek.top

[Q36] 左连接
来源：http://jcl.hfpthk.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jhh.52xcode.cn

[Q37] 右连接
来源：http://hhk.xuanzx.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bwo.ydjk.org.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kdq.sjlbkw.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rlw.cucudq.cn

[Q39] 自连接（查上下级）
来源：http://pyi.cashguo.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://eji.sjlbkw.cn


<!-- 参考信息 -->