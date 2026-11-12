代发 wailian999

[N05] 最大公约数
来源：http://ycg.quarkkingdee.top

Py:   math.gcd(a, b)
来源：http://dpk.svipenyu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nwa.smart0.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://asj.wangshuangyany.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wqy.zycfv.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pnk.ydzc1.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ahp.fanxiaobao.xyz

Ruby: a.gcd(b)
来源：http://ynm.cashguo.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pvc.jinqigfzy.top

[N06] 判断回文字符串
来源：http://gyd.nwbrower.top

Py:   s == s[::-1]
来源：http://but.zhaomingkeji.xyz

PHP:  $s === strrev($s);
来源：http://bct.9152youxi.cn

JS:   s === [...s].reverse().join("")
来源：http://ids.shanyushiyangkeji.top

TS:   s === [...s].reverse().join("")
来源：http://eqm.hnxiangtu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://egn.cucudq.cn

Go:   // 双指针从两端比较
来源：http://gze.tarul.cn

Ruby: s == s.reverse
来源：http://uid.hesvh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ezi.kuanghao11.cn

[N07] 两数之和（返回下标）
来源：http://dvb.havefunace.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://iqm.bjfxy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dvs.feifeiyinyue.top

JS:   // 手写 Map：map.set(v, i)
来源：http://pdi.yfazqb.com

TS:   // 手写 Map<string, number>
来源：http://ulu.316326.xyz

Java: // 手写 HashMap
来源：http://rzx.gzhubu.top

Go:   // 手写 map[int]int
来源：http://hib.birdmap.top

Ruby: // 手写 Hash
来源：http://kgm.fehbvm.com

C#:   // 手写 Dictionary<int, int>
来源：http://vbb.fehbvm.com

[N08] 生成全排列
来源：http://iia.shzxlz.cn

Py:   itertools.permutations(arr)
来源：http://eiv.yongpay.top

PHP:  // 手写递归交换
来源：http://par.yfazqb.com

JS:   // 手写回溯递归
来源：http://wpv.svipenyu.cn

TS:   // 手写回溯递归
来源：http://jia.yanxiufei.cn

Java: // 手写回溯递归
来源：http://hwm.yvedp.cn

Go:   // 手写回溯递归
来源：http://yvg.hesvh.cn

Ruby: arr.permutation.to_a
来源：http://eyy.aibaodan.cn

C#:   // 手写回溯递归
来源：http://irs.zhoulong.xyz

[N09] 栈与队列
来源：http://xmy.yangfankeji.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uth.xziqi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ugv.cqqwz.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dxs.xinyue.icu

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wbn.9152youxi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qdr.hnqzz.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xur.ydzc1.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hdg.haohaochexian.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gzk.ivvv.top

[N10] 链表节点定义
来源：http://yfi.bbcook.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dan.ehwqpu.com

PHP:  class Node { public $v; public $next = null; }
来源：http://upu.shanyushiyangkeji.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ceq.dianchejie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zsz.zhoulong.xyz

Java: class Node { int v; Node next; }
来源：http://huv.9152youxi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qge.zhijiandao.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://odz.jyoumei.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jkf.fehbvm.com

[N11] 二叉树中序遍历
来源：http://hoj.tianlin.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ugl.aizwys.cn

PHP:  // 手写递归函数
来源：http://ods.ctjpmb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://stk.feifeiyinyue.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://exf.bjfxy.top

Java: // 手写递归
来源：http://itg.zhongyouzk.top

Go:   // 手写递归
来源：http://yvs.shzxlz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://iju.hnxiangtu.top

C#:   // 手写递归
来源：http://fil.hcnkem.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jww.yfazqb.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yxc.andypj.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wyv.yonumen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ayr.hysaishi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zrz.epnwcf.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sae.hnqzz.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://oer.0kj1m.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://khv.yanxiufei.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lgz.zdqjudy.top

================================================================================
来源：http://ijs.smart0.xyz

O. 并发与异步
来源：http://oqx.ybcxt.top

================================================================================
来源：http://afb.xingfuxueyuan.xyz

[O01] 启动一个线程
来源：http://pld.yonumen.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zjl.yueranfly.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://doz.yj20258888.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lgn.jqgufenzy.top

TS:   // 同 JS
来源：http://goc.316326.xyz

Java: new Thread(() -> f()).start()
来源：http://lkk.aibaodan.cn

Go:   go f()
来源：http://gju.bbcook.cn

Ruby: Thread.new { f }
来源：http://szb.yj20258888.top

C#:   Task.Run(() => F());
来源：http://lao.fanxiaobao.xyz

[O02] 使用线程池
来源：http://wkb.fanxiaobao.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ucv.c1oappe.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://chu.snrcjt.cn

JS:   // worker_threads 线程池
来源：http://emj.kuanghao11.cn

TS:   // worker_threads 线程池
来源：http://nzo.fanxiaobao.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://zbp.yanxiufei.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wvv.nanxinkj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hvm.shanyushiyangtech.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xan.xingfuxueyuan.xyz

[O03] 加锁保护共享数据
来源：http://jfw.zhoulong.xyz

Py:   with lock: shared += 1
来源：http://ndr.shzxlz.cn

PHP:  // 用 flock() 做文件锁
来源：http://vem.yuanzhike.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yfy.cheryme.top

TS:   // 同 JS
来源：http://quf.cashguo.top

Java: synchronized (this) { shared++; }
来源：http://jvd.xingfuxueyuan.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bug.shzxlz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rym.yonumen.top

C#:   lock (gate) { shared++; }
来源：http://jid.yongpay.top

[O04] 定义异步函数并等待
来源：http://ake.cashguo.top

Py:   async def f():⏎    await g()
来源：http://gjh.yangfankeji.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vfk.meibo888.top

JS:   async function f() { await g(); }
来源：http://cyq.yanxiufei.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zxb.zhaomingkeji.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qbj.vqdsnc.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ulo.quarkkingdee.top

Ruby: # 用 Fiber 或 async gem
来源：http://ypr.zhoulong.xyz

C#:   async Task F() { await G(); }
来源：http://zgg.guannengcc.top

[O05] 并发执行并等待全部完成
来源：http://igw.hywenlv.cn

Py:   asyncio.gather(*tasks)
来源：http://yhr.sufxvd.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mmx.havefunace.top

JS:   await Promise.all(tasks)
来源：http://bze.sjlbkw.cn

TS:   await Promise.all(tasks)
来源：http://sqc.nwbrower.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jkh.yanxiufei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bwd.hongshengwenyu.top

Ruby: threads.map(&:join)
来源：http://pju.jianghu66.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xon.cashguo.top

[O06] 使用进程池
来源：http://aca.zhongyouzk.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yns.iojbl.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vvp.fanxiaobao.xyz

JS:   // child_process / cluster 模块
来源：http://xgw.yj202588.top

TS:   // child_process / cluster 模块
来源：http://dem.zhiwuduotai.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pyo.0kj1m.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ugk.ywan-chungtsiang.top

Ruby: // fork 块
来源：http://xpe.dianchejie.cn

C#:   Parallel.For
来源：http://dfr.andypj.xyz

================================================================================
来源：http://clb.xylfe.cn

P. 常用工具函数
来源：http://dnu.ywan-chungtsiang.top

================================================================================
来源：http://jaa.sufxvd.cn

[P01] 生成 UUID
来源：http://fsl.ivvv.top

Py:   str(uuid.uuid4())
来源：http://ryb.birdmap.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ypk.xuetiantiany.cn

JS:   crypto.randomUUID()
来源：http://qas.zhiwuduotai.top

TS:   crypto.randomUUID()
来源：http://bmo.gotoacloud.top

Java: UUID.randomUUID().toString()
来源：http://vko.sjlbkw.cn

Go:   // 用 github.com/google/uuid
来源：http://mfm.yvedp.cn

Ruby: SecureRandom.uuid
来源：http://zlk.epnwcf.com

C#:   Guid.NewGuid().ToString()
来源：http://icc.haohaochexian.top

[P02] MD5 / SHA256 摘要
来源：http://irw.yueranfly.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bno.gotoacloud.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://mvn.chenlongwang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mnz.gogol.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uoo.mhx1999.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qmz.cucudq.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ytq.0kj1m.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fqp.yj202588.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hzt.chenlongwang.top

[P03] 生成短随机字符串
来源：http://ycg.vqdsnc.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ots.smart0.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wul.yj20258888.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rvk.nanxuanxn.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vqc.tarul.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wbb.tian-w.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rgo.yonumen.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://apy.zhaomingkeji.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qhl.ppjwa.cn

[P04] 求长度
来源：http://nxw.gzhubu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tgt.aibaodan.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jpe.yj202588.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ran.chenzaomai.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tkp.ybcxt.top

Java: list.size();  map.size();  s.length()
来源：http://vwc.yonumen.top

Go:   len(arr);  len(m)
来源：http://cnp.feifeiyinyue.top

Ruby: x.length;  x.size
来源：http://gos.fktsv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jqh.zhoulong.xyz

[P05] 判断两个对象内容是否相等
来源：http://ssi.0kj1m.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qrg.fengsongda.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bih.sjlbkw.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://roi.yuanzhike.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pjc.jianghu66.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nww.jinqigufen.top

Go:   reflect.DeepEqual(a, b)
来源：http://mvl.hammf.cn

Ruby: a == b
来源：http://hyi.tarul.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bos.jinghuilouyu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nqi.ydzc1.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hfm.zhoulong.xyz

PHP:  if (empty($x)) {}
来源：http://agb.ctjpmb.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xwc.jinghuilouyu.cn

TS:   if (x == null) {}
来源：http://sws.dianchejie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cre.nwbrower.top

Go:   if x == nil {}
来源：http://jjj.meibo888.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xmu.gaohongyu789.top

C#:   if (x is null) {}
来源：http://qul.mhx1999.top

[P07] 防抖与节流
来源：http://cab.zhixingplan.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oxw.xingfuxueyuan.xyz

PHP:  // 手写时间戳比较
来源：http://xks.zhongyouzk.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vpd.zhongyouzk.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pix.fanxiaobao.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jqm.meibo888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://egr.vqdsnc.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://jjn.yj20258.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bdf.shuidangran.top

[P08] 处理浮点精度问题
来源：http://bbw.sxryk.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://iep.epnwcf.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://car.daxiang520.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://orr.xylfe.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tvj.zdqjudy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jiz.tianlin.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mct.yanxiufei.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zwk.zdqjudy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fxk.shangyingyoupin.top

================================================================================
来源：http://lnp.wangdashe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://etv.shanyushiyangtech.top

================================================================================
来源：http://gsl.ivvv.top

[Q01] 创建表
来源：http://zte.iojbl.cn

CREATE TABLE users (
来源：http://wgg.hesvh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uty.hesvh.cn

name VARCHAR(50) NOT NULL,
来源：http://kvd.nwbrower.top

email VARCHAR(100) UNIQUE,
来源：http://kwy.xuanzx.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://iby.feifeiyinyue.top

);
来源：http://sux.vqdsnc.cn

[Q02] 创建带外键的表
来源：http://oay.jinyuanbaomall.cn

CREATE TABLE orders (
来源：http://cos.dashuyun.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://joz.chenjidiqi.icu

user_id INT NOT NULL,
来源：http://cus.gaohongyu789.top

amount DECIMAL(10, 2),
来源：http://ytb.ydzc1.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kbm.zhongyouzk.top

);
来源：http://ksx.redwolf501.top

[Q03] 增加列
来源：http://gyh.hywenlv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pqx.chenlongwang.top

[Q04] 修改列类型
来源：http://lpg.jinyuanbaomall.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bzh.wangdashe.top

[Q05] 重命名列
来源：http://dev.guowangkeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rze.iojbl.cn

[Q06] 删除列
来源：http://fds.sjlbkw.cn

ALTER TABLE users DROP COLUMN age;
来源：http://eme.pengpengdd.cyou

[Q07] 删除表
来源：http://gdl.dianchejie.cn

DROP TABLE IF EXISTS orders;
来源：http://xxl.yuanzhike.top

[Q08] 创建普通索引
来源：http://vin.ydjk.org.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://dpr.uphjek.com

[Q09] 创建唯一索引
来源：http://nrv.birdmap.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gll.yuxming.cn

[Q10] 插入单行
来源：http://zan.yfazqb.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hyp.gogol.net.cn

[Q11] 一次插入多行
来源：http://dpj.jinyuanbaomall.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://obs.ctjpmb.com

[Q12] 插入后取自增 ID
来源：http://pzx.jinqigfzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://atw.jqgufenzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zlc.hysaishi.cn

[Q13] 忽略重复插入
来源：http://szy.zhijiandao.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hqz.xziqi.cn

[Q14] 存在则更新（upsert）
来源：http://kgz.ehwqpu.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://odl.pengpengdd.cyou

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://egt.shzxlz.cn

[Q15] 查询全部
来源：http://olx.sjlbkw.cn

SELECT * FROM users;
来源：http://pjw.jlsjyb.cn

[Q16] 查询指定列
来源：http://oje.haohaochexian.top

SELECT id, name FROM users;
来源：http://hnh.uphjek.com

[Q17] 条件查询
来源：http://uam.hesvh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ghz.ehwqpu.com

[Q18] 模糊匹配
来源：http://sal.yanxiufei.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qlm.gzhubu.top

[Q19] 范围查询
来源：http://rqd.zdbjq.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zgr.feifeiyinyue.top

[Q20] IN 列表
来源：http://ukr.zdbjq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bzr.epnwcf.com

[Q21] 空值判断
来源：http://ifb.daxiang520.top

SELECT * FROM users WHERE email IS NULL;
来源：http://siz.jinyuanbaomall.cn

[Q22] 排序
来源：http://qmy.dianchejie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gkq.yfazqb.com

[Q23] 分页
来源：http://rww.wangdashe.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dqz.smart0.xyz

[Q24] 去重
来源：http://ayr.tianlin.xyz

SELECT DISTINCT city FROM users;
来源：http://ucp.uphjek.com

[Q25] 只取前 N 条
来源：http://mnv.guannengcc.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rvn.yanxiufei.cn

[Q26] 计数
来源：http://lcw.ybcxt.top

SELECT COUNT(*) FROM users;
来源：http://gpq.zdbjq.cn

[Q27] 条件计数
来源：http://ktl.xuetiantiany.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nuw.wangdashe.top

[Q28] 求和与平均
来源：http://pat.redwolf501.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fud.316326.xyz

[Q29] 最大最小值
来源：http://oyo.hammf.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fqa.yangfankeji.com

[Q30] 分组统计
来源：http://cky.zhengqikj.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gyn.ctjpmb.com

[Q31] 分组后过滤
来源：http://fny.cucudq.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nfl.meibo888.top

[Q32] 分组拼接字符串
来源：http://prf.zdbjq.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qmd.ydzc1.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ktm.birdmap.top

[Q33] 多列分组
来源：http://pmy.yj202588.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cxz.zhengqikj.top

[Q34] 每组取第一条
来源：http://cbh.xuanzx.com

SELECT * FROM (
来源：http://ovw.tanke756.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mbr.iojbl.cn

) t WHERE rn = 1;
来源：http://fxz.daxiang520.top

[Q35] 内连接
来源：http://zzu.ybcxt.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ulv.jiagoushi.top

[Q36] 左连接
来源：http://nnl.ppjwa.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qpf.zdqjudy.top

[Q37] 右连接
来源：http://ltz.svipenyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://voj.hcnkem.com

[Q38] 全外连接（PostgreSQL）
来源：http://dki.birdmap.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oum.xziqi.cn

[Q39] 自连接（查上下级）
来源：http://qih.sufxvd.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://tus.dashuyun.cn


<!-- 参考信息 -->