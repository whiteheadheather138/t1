代发 wailian999

[N05] 最大公约数
来源：http://hld.bjfxy.top

Py:   math.gcd(a, b)
来源：http://bve.yfazqb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xem.tianlin.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ulv.birdmap.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://frj.nwbrower.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ycz.hysaishi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sjf.yj20258888.top

Ruby: a.gcd(b)
来源：http://uli.daria6918.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://aya.quarkkingdee.top

[N06] 判断回文字符串
来源：http://wdu.xylfe.cn

Py:   s == s[::-1]
来源：http://ode.daria6918.cn

PHP:  $s === strrev($s);
来源：http://czm.yj202588.top

JS:   s === [...s].reverse().join("")
来源：http://ygw.yfazqb.com

TS:   s === [...s].reverse().join("")
来源：http://vui.xuanzx.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xbo.yanxiufei.cn

Go:   // 双指针从两端比较
来源：http://ism.vqdsnc.cn

Ruby: s == s.reverse
来源：http://wkj.fengsongda.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://hxb.jqgufenzy.top

[N07] 两数之和（返回下标）
来源：http://jwo.cqqwz.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jsl.nanxuanxn.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://iis.sxryk.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xip.birdmap.top

TS:   // 手写 Map<string, number>
来源：http://beo.ydzc1.top

Java: // 手写 HashMap
来源：http://zne.c1oappe.top

Go:   // 手写 map[int]int
来源：http://qya.gotoacloud.top

Ruby: // 手写 Hash
来源：http://ixx.hnxiangtu.top

C#:   // 手写 Dictionary<int, int>
来源：http://hcd.fktsv.cn

[N08] 生成全排列
来源：http://fcp.zhaomingkeji.xyz

Py:   itertools.permutations(arr)
来源：http://xwy.jiagoushi.top

PHP:  // 手写递归交换
来源：http://luo.uphjek.com

JS:   // 手写回溯递归
来源：http://oea.pengpengdd.cyou

TS:   // 手写回溯递归
来源：http://odg.tianlin.xyz

Java: // 手写回溯递归
来源：http://xnw.jinqigfzy.top

Go:   // 手写回溯递归
来源：http://wog.quarkkingdee.top

Ruby: arr.permutation.to_a
来源：http://hom.nanxinkj.top

C#:   // 手写回溯递归
来源：http://jgy.nanxuanxn.top

[N09] 栈与队列
来源：http://wbt.cdnleiting.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xdd.nwbrower.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lha.andypj.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://usa.shzxlz.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ude.hongshengwenyu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mqn.yj202588.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ezq.ybcxt.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cxl.xuanzx.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kdx.svipenyu.cn

[N10] 链表节点定义
来源：http://yhz.ydzc1.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://flw.gaohongyu789.top

PHP:  class Node { public $v; public $next = null; }
来源：http://alm.svipenyu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://suq.gzhubu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://usb.jqgfzy.top

Java: class Node { int v; Node next; }
来源：http://mmb.316326.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://egb.chenlongwang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hcm.yfazqb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://lbc.yj202588.top

[N11] 二叉树中序遍历
来源：http://kpr.yj20258.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ulw.gaohongyu789.top

PHP:  // 手写递归函数
来源：http://euk.cdnleiting.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bfq.zdqjudy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ddh.meibo888.top

Java: // 手写递归
来源：http://kqj.yvedp.cn

Go:   // 手写递归
来源：http://wgf.jqgfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hru.xylfe.cn

C#:   // 手写递归
来源：http://ili.52xcode.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://iiu.epnwcf.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rdd.yueranfly.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xxv.birdmap.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tta.ppjwa.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://try.nwbrower.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kvv.yongpay.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yaj.ehwqpu.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://poe.pengpengdd.cyou

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xja.cheryme.top

================================================================================
来源：http://gfg.dashuyun.cn

O. 并发与异步
来源：http://ajj.9152youxi.cn

================================================================================
来源：http://ztg.zycfv.cn

[O01] 启动一个线程
来源：http://gbf.wangdashe.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://iti.dianchejie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zdb.nwbrower.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://etz.daria6918.cn

TS:   // 同 JS
来源：http://han.chenzaomai.com

Java: new Thread(() -> f()).start()
来源：http://pyd.meibo888.top

Go:   go f()
来源：http://itc.jqgfzy.top

Ruby: Thread.new { f }
来源：http://bjn.epnwcf.com

C#:   Task.Run(() => F());
来源：http://zfw.jinghuilouyu.cn

[O02] 使用线程池
来源：http://eig.chenjidiqi.icu

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dti.meibo888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wzr.sxryk.cn

JS:   // worker_threads 线程池
来源：http://vzs.snrcjt.cn

TS:   // worker_threads 线程池
来源：http://wzw.redwolf501.top

Java: Executors.newFixedThreadPool(4)
来源：http://apk.yuanzhike.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pja.andypj.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://api.wangdashe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mzi.zhijiandao.cn

[O03] 加锁保护共享数据
来源：http://twz.yj202588.top

Py:   with lock: shared += 1
来源：http://siq.ctjpmb.com

PHP:  // 用 flock() 做文件锁
来源：http://jqv.pengpengdd.cyou

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://egm.nwbrower.top

TS:   // 同 JS
来源：http://xmb.xuanzx.com

Java: synchronized (this) { shared++; }
来源：http://lpd.cdnleiting.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qot.cqqwz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://osj.zycfv.cn

C#:   lock (gate) { shared++; }
来源：http://fkc.dashuyun.cn

[O04] 定义异步函数并等待
来源：http://ycb.shuidangran.top

Py:   async def f():⏎    await g()
来源：http://kuw.ybcxt.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dsq.nwbrower.top

JS:   async function f() { await g(); }
来源：http://xpm.daxiang520.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ajd.redwolf501.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rok.sysykeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://huu.zhongyouzk.top

Ruby: # 用 Fiber 或 async gem
来源：http://oie.wangdashe.top

C#:   async Task F() { await G(); }
来源：http://mxf.hywenlv.cn

[O05] 并发执行并等待全部完成
来源：http://cfp.ybcxt.top

Py:   asyncio.gather(*tasks)
来源：http://sht.xziqi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sbi.quarkkingdee.top

JS:   await Promise.all(tasks)
来源：http://lef.xingfuxueyuan.xyz

TS:   await Promise.all(tasks)
来源：http://laf.tian-w.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://npv.ydjk.org.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ijq.iojbl.cn

Ruby: threads.map(&:join)
来源：http://zfw.andypj.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://vni.quarkkingdee.top

[O06] 使用进程池
来源：http://nxt.yongpay.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://glm.shanyushiyangkeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://zce.shangyingyoupin.top

JS:   // child_process / cluster 模块
来源：http://zqr.cqqwz.cn

TS:   // child_process / cluster 模块
来源：http://xko.redwolf501.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://olv.xingfuxueyuan.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://edt.jqgfzy.top

Ruby: // fork 块
来源：http://khr.bjfxy.top

C#:   Parallel.For
来源：http://rsz.chenzaomai.com

================================================================================
来源：http://pmn.c1oappe.top

P. 常用工具函数
来源：http://zcz.jinqigfzy.top

================================================================================
来源：http://hoz.jinqigfzy.top

[P01] 生成 UUID
来源：http://wdh.jyoumei.cn

Py:   str(uuid.uuid4())
来源：http://lfx.pycfn.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jpf.jqgufenzy.top

JS:   crypto.randomUUID()
来源：http://grd.yongpay.top

TS:   crypto.randomUUID()
来源：http://lrm.xinyue.icu

Java: UUID.randomUUID().toString()
来源：http://whk.nwbrower.top

Go:   // 用 github.com/google/uuid
来源：http://vbw.52xcode.cn

Ruby: SecureRandom.uuid
来源：http://lef.svipenyu.cn

C#:   Guid.NewGuid().ToString()
来源：http://drv.ydzc1.top

[P02] MD5 / SHA256 摘要
来源：http://yks.chenzaomai.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://drh.smart0.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://jat.jinqigfzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://agl.sweek.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://not.ctjpmb.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ajc.cucudq.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nmb.ivvv.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hdo.tarul.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fvo.tian-w.cn

[P03] 生成短随机字符串
来源：http://rmv.shangyingyoupin.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dcu.xinyue.icu

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mio.nwbrower.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://knk.aizwys.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rwl.vqdsnc.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zhd.shanyushiyangtech.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jte.yfazqb.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://npm.dianchejie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dyr.52xcode.cn

[P04] 求长度
来源：http://kuw.yuanzhike.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tjc.fanxiaobao.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ahb.nwbrower.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://scz.ppjwa.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mer.fzhhl.top

Java: list.size();  map.size();  s.length()
来源：http://gew.smart0.xyz

Go:   len(arr);  len(m)
来源：http://bhk.xingfuxueyuan.xyz

Ruby: x.length;  x.size
来源：http://bvr.cashguo.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://apj.zhixingplan.top

[P05] 判断两个对象内容是否相等
来源：http://rgi.xziqi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dtr.ctjpmb.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bgx.birdmap.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mfd.hcnkem.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bdb.xinyue.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cur.epnwcf.com

Go:   reflect.DeepEqual(a, b)
来源：http://kqu.xylfe.cn

Ruby: a == b
来源：http://huo.daria6918.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fyc.hammf.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nya.smart0.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iak.cashguo.top

PHP:  if (empty($x)) {}
来源：http://iql.shanyushiyangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://srd.fehbvm.com

TS:   if (x == null) {}
来源：http://pol.yonumen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://eym.pengpengdd.cyou

Go:   if x == nil {}
来源：http://wwh.9152youxi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kny.dianchejie.cn

C#:   if (x is null) {}
来源：http://ndz.gogol.net.cn

[P07] 防抖与节流
来源：http://nlc.zhiwuduotai.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lpn.ybcxt.top

PHP:  // 手写时间戳比较
来源：http://hjc.zhaomingkeji.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qfg.0kj1m.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tgi.hesvh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ujo.zdbjq.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zbp.shangyingyoupin.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://fwj.zhijiandao.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cms.dashuyun.cn

[P08] 处理浮点精度问题
来源：http://rvh.dianchejie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cnn.mhx1999.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://omc.pengpengdd.cyou

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lxm.yongpay.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vgg.iojbl.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jax.zhongyouzk.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vej.sufxvd.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vfi.hnxiangtu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://osr.yfazqb.com

================================================================================
来源：http://fzp.fktsv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kjs.guannengcc.top

================================================================================
来源：http://ueh.ydzc1.top

[Q01] 创建表
来源：http://eji.hesvh.cn

CREATE TABLE users (
来源：http://ozv.ctjpmb.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://apv.9152youxi.cn

name VARCHAR(50) NOT NULL,
来源：http://tnv.quarkkingdee.top

email VARCHAR(100) UNIQUE,
来源：http://jjn.zhoulong.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ypy.fanxiaobao.xyz

);
来源：http://ufb.fanxiaobao.xyz

[Q02] 创建带外键的表
来源：http://csk.hnxiangtu.top

CREATE TABLE orders (
来源：http://tjm.jyoumei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kzs.jinghuilouyu.cn

user_id INT NOT NULL,
来源：http://doh.hfpthk.cn

amount DECIMAL(10, 2),
来源：http://cpp.epnwcf.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mle.tanke756.top

);
来源：http://zuv.yuxming.cn

[Q03] 增加列
来源：http://pxw.xuanzx.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://djh.zhixingplan.top

[Q04] 修改列类型
来源：http://vxx.shanyushiyangtech.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lqg.hnxiangtu.top

[Q05] 重命名列
来源：http://dcn.hfpthk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hnv.zdqjudy.top

[Q06] 删除列
来源：http://ggg.kuanghao11.cn

ALTER TABLE users DROP COLUMN age;
来源：http://meb.xinyue.icu

[Q07] 删除表
来源：http://bdj.sysykeji.top

DROP TABLE IF EXISTS orders;
来源：http://gev.yongpay.top

[Q08] 创建普通索引
来源：http://mco.xylfe.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sap.daxiang520.top

[Q09] 创建唯一索引
来源：http://ara.zhiwuduotai.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://aop.hnqzz.top

[Q10] 插入单行
来源：http://tyb.xinyue.icu

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ooj.aibaodan.cn

[Q11] 一次插入多行
来源：http://fva.andypj.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uam.xuetiantiany.cn

[Q12] 插入后取自增 ID
来源：http://nvj.sjlbkw.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rox.yj20258888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pon.sweek.top

[Q13] 忽略重复插入
来源：http://fcq.jinqigfzy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bdm.havefunace.top

[Q14] 存在则更新（upsert）
来源：http://bqu.jqgfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lzv.jinqigufen.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dlc.yfazqb.com

[Q15] 查询全部
来源：http://jbi.jinghuilouyu.cn

SELECT * FROM users;
来源：http://scp.chenjidiqi.icu

[Q16] 查询指定列
来源：http://phk.vehdjk.com

SELECT id, name FROM users;
来源：http://jns.tarul.cn

[Q17] 条件查询
来源：http://gxf.gaohongyu789.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pgt.yonumen.top

[Q18] 模糊匹配
来源：http://ntc.nanxinkj.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://shs.gotoacloud.top

[Q19] 范围查询
来源：http://ckv.yj20258888.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wbn.guannengcc.top

[Q20] IN 列表
来源：http://gyz.andypj.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://eot.fengsongda.top

[Q21] 空值判断
来源：http://fzl.cdnleiting.top

SELECT * FROM users WHERE email IS NULL;
来源：http://bmf.shanyushiyangtech.top

[Q22] 排序
来源：http://mih.redwolf501.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mbv.wangdashe.top

[Q23] 分页
来源：http://bms.vehdjk.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yue.shuidangran.top

[Q24] 去重
来源：http://qmo.hesvh.cn

SELECT DISTINCT city FROM users;
来源：http://fcq.havefunace.top

[Q25] 只取前 N 条
来源：http://yaw.bbcook.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qwi.tanke756.top

[Q26] 计数
来源：http://mup.daxiang520.top

SELECT COUNT(*) FROM users;
来源：http://yeh.xylfe.cn

[Q27] 条件计数
来源：http://iab.316326.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kdx.xziqi.cn

[Q28] 求和与平均
来源：http://iax.fanxiaobao.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://aec.aibaodan.cn

[Q29] 最大最小值
来源：http://zsm.hammf.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gxl.9152youxi.cn

[Q30] 分组统计
来源：http://vli.yangfankeji.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rtf.gotoacloud.top

[Q31] 分组后过滤
来源：http://zxq.fanxiaobao.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wrg.epnwcf.com

[Q32] 分组拼接字符串
来源：http://pbw.hnqzz.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eak.aibaodan.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://inr.shangyingyoupin.top

[Q33] 多列分组
来源：http://lty.jlsjyb.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://abc.cucudq.cn

[Q34] 每组取第一条
来源：http://nhs.yonumen.top

SELECT * FROM (
来源：http://fpa.tanke756.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://job.nanxuanxn.top

) t WHERE rn = 1;
来源：http://uvc.zdbjq.cn

[Q35] 内连接
来源：http://drj.shzxlz.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://snh.cheryme.top

[Q36] 左连接
来源：http://jqv.xziqi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ebj.sysykeji.top

[Q37] 右连接
来源：http://mqc.hnqzz.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uls.yangfankeji.com

[Q38] 全外连接（PostgreSQL）
来源：http://ycl.bbcook.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qcp.cqqwz.cn

[Q39] 自连接（查上下级）
来源：http://zve.iojbl.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://pjt.52xcode.cn


<!-- 参考信息 -->