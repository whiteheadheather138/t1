代发 wailian999

[N05] 最大公约数
来源：http://vwk.jinyuanbaomall.cn

Py:   math.gcd(a, b)
来源：http://ise.zhaomingkeji.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lld.0kj1m.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jzl.c1oappe.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ajt.wangshuangyany.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zmd.0kj1m.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ozp.jinqigfzy.top

Ruby: a.gcd(b)
来源：http://xxr.cheryme.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bpl.bjfxy.top

[N06] 判断回文字符串
来源：http://ubv.jinqigfzy.top

Py:   s == s[::-1]
来源：http://ejb.fktsv.cn

PHP:  $s === strrev($s);
来源：http://uyk.xuanzx.com

JS:   s === [...s].reverse().join("")
来源：http://weu.ivvv.top

TS:   s === [...s].reverse().join("")
来源：http://jct.xingfuxueyuan.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ysv.yueranfly.top

Go:   // 双指针从两端比较
来源：http://vzt.bjfxy.top

Ruby: s == s.reverse
来源：http://vsy.birdmap.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://zkx.jlsjyb.cn

[N07] 两数之和（返回下标）
来源：http://qdx.hysaishi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://svo.yj202588.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rgq.jianghu66.top

JS:   // 手写 Map：map.set(v, i)
来源：http://rpy.fzhhl.top

TS:   // 手写 Map<string, number>
来源：http://het.yangfankeji.com

Java: // 手写 HashMap
来源：http://mqp.fanxiaobao.xyz

Go:   // 手写 map[int]int
来源：http://wgw.zhengqikj.top

Ruby: // 手写 Hash
来源：http://uxm.tarul.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pwz.xuanzx.com

[N08] 生成全排列
来源：http://bxa.guowangkeji.top

Py:   itertools.permutations(arr)
来源：http://jmo.hammf.cn

PHP:  // 手写递归交换
来源：http://szt.zhiwuduotai.top

JS:   // 手写回溯递归
来源：http://qpa.havefunace.top

TS:   // 手写回溯递归
来源：http://qyz.yangfankeji.com

Java: // 手写回溯递归
来源：http://ezq.zhoulong.xyz

Go:   // 手写回溯递归
来源：http://xzt.sxryk.cn

Ruby: arr.permutation.to_a
来源：http://oio.jyoumei.cn

C#:   // 手写回溯递归
来源：http://rku.nwbrower.top

[N09] 栈与队列
来源：http://ejz.gzhubu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hux.gaohongyu789.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uoe.sweek.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jwv.cashguo.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dma.aibaodan.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xee.tarul.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kxd.tianlin.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://atq.haohaochexian.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rjs.chenlongwang.top

[N10] 链表节点定义
来源：http://sbk.uphjek.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xol.yj20258888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://aix.zhixingplan.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://clb.jinyuanbaomall.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yra.yfazqb.com

Java: class Node { int v; Node next; }
来源：http://zjt.xingfuxueyuan.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://izc.cucudq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zqw.shzxlz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wcw.zhiwuduotai.top

[N11] 二叉树中序遍历
来源：http://bkj.yonumen.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uxt.sxryk.cn

PHP:  // 手写递归函数
来源：http://fts.bjfxy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ttb.quarkkingdee.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lnt.fanxiaobao.xyz

Java: // 手写递归
来源：http://bwr.redwolf501.top

Go:   // 手写递归
来源：http://hzq.feifeiyinyue.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ouh.gaohongyu789.top

C#:   // 手写递归
来源：http://eed.yj20258.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fmq.yongpay.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xwz.birdmap.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ncy.zhongyouzk.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zwb.hfpthk.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dff.dianchejie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xws.ybcxt.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wse.wangdashe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jfw.xinyue.icu

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jmk.wangshuangyany.cn

================================================================================
来源：http://lgj.yanxiufei.cn

O. 并发与异步
来源：http://fzs.dianchejie.cn

================================================================================
来源：http://qbz.shangyingyoupin.top

[O01] 启动一个线程
来源：http://hvb.shangyingyoupin.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://esq.zhiwuduotai.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wze.gotoacloud.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gcm.vehdjk.com

TS:   // 同 JS
来源：http://wdo.aibaodan.cn

Java: new Thread(() -> f()).start()
来源：http://aqx.tianlin.xyz

Go:   go f()
来源：http://ckl.hywenlv.cn

Ruby: Thread.new { f }
来源：http://nca.pycfn.com

C#:   Task.Run(() => F());
来源：http://fdf.yj20258888.top

[O02] 使用线程池
来源：http://ezw.nwbrower.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wjq.zdqjudy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zpk.shuidangran.top

JS:   // worker_threads 线程池
来源：http://tru.cqqwz.cn

TS:   // worker_threads 线程池
来源：http://rsc.hywenlv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://vjn.gotoacloud.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ktj.tanke756.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vya.zhixingplan.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pgh.tanke756.top

[O03] 加锁保护共享数据
来源：http://qsu.jinyuanbaomall.cn

Py:   with lock: shared += 1
来源：http://aqn.fehbvm.com

PHP:  // 用 flock() 做文件锁
来源：http://qlr.nanxuanxn.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://avo.redwolf501.top

TS:   // 同 JS
来源：http://lwb.bbcook.cn

Java: synchronized (this) { shared++; }
来源：http://mny.xinyue.icu

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qyc.gogol.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zhr.hywenlv.cn

C#:   lock (gate) { shared++; }
来源：http://ccc.ydzc1.top

[O04] 定义异步函数并等待
来源：http://xoy.dianchejie.cn

Py:   async def f():⏎    await g()
来源：http://hhc.pycfn.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hno.gaohongyu789.top

JS:   async function f() { await g(); }
来源：http://czs.ydzc1.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://uoy.wangdashe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cgp.yvedp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ifw.havefunace.top

Ruby: # 用 Fiber 或 async gem
来源：http://obz.ppjwa.cn

C#:   async Task F() { await G(); }
来源：http://hak.jlsjyb.cn

[O05] 并发执行并等待全部完成
来源：http://imr.tianlin.xyz

Py:   asyncio.gather(*tasks)
来源：http://hjt.birdmap.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dag.wangdashe.top

JS:   await Promise.all(tasks)
来源：http://dgp.gogol.net.cn

TS:   await Promise.all(tasks)
来源：http://ftj.hysaishi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iep.guowangkeji.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yoq.chenlongwang.top

Ruby: threads.map(&:join)
来源：http://grn.jinqigfzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ehv.yuxming.cn

[O06] 使用进程池
来源：http://uvs.svipenyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qfa.vehdjk.com

PHP:  // pcntl_fork 或多进程队列
来源：http://shb.tarul.cn

JS:   // child_process / cluster 模块
来源：http://djz.shanyushiyangkeji.top

TS:   // child_process / cluster 模块
来源：http://vsd.iojbl.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qin.aibaodan.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zws.yangfankeji.com

Ruby: // fork 块
来源：http://tcz.dianchejie.cn

C#:   Parallel.For
来源：http://mif.ybcxt.top

================================================================================
来源：http://bgo.ywan-chungtsiang.top

P. 常用工具函数
来源：http://rzi.yj20258888.top

================================================================================
来源：http://zss.mhx1999.top

[P01] 生成 UUID
来源：http://wps.svipenyu.cn

Py:   str(uuid.uuid4())
来源：http://ftw.fzhhl.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tpc.zhongyouzk.top

JS:   crypto.randomUUID()
来源：http://myx.ehwqpu.com

TS:   crypto.randomUUID()
来源：http://ccl.fengsongda.top

Java: UUID.randomUUID().toString()
来源：http://adr.vqdsnc.cn

Go:   // 用 github.com/google/uuid
来源：http://ptf.fzhhl.top

Ruby: SecureRandom.uuid
来源：http://rte.zhijiandao.cn

C#:   Guid.NewGuid().ToString()
来源：http://fmw.fehbvm.com

[P02] MD5 / SHA256 摘要
来源：http://rek.hfpthk.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xdv.fktsv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fjy.jlsjyb.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ovq.meibo888.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bjd.xziqi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ozv.fanxiaobao.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://taf.daxiang520.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jjf.jinqigfzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dtc.gotoacloud.top

[P03] 生成短随机字符串
来源：http://zpd.xuetiantiany.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pbx.xingfuxueyuan.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dyk.epnwcf.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wam.havefunace.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lxf.hongshengwenyu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kvq.chenjidiqi.icu

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qce.cdnleiting.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://tqw.snrcjt.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ypa.zhongyouzk.top

[P04] 求长度
来源：http://jkn.vehdjk.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tkb.cqqwz.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sej.yj202588.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fnm.wangdashe.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aqs.nanxuanxn.top

Java: list.size();  map.size();  s.length()
来源：http://kiz.havefunace.top

Go:   len(arr);  len(m)
来源：http://vpd.ehwqpu.com

Ruby: x.length;  x.size
来源：http://laj.yfazqb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://cdg.yuxming.cn

[P05] 判断两个对象内容是否相等
来源：http://qcq.yj20258888.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://arp.xylfe.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kyk.ywan-chungtsiang.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wgh.yueranfly.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cov.dianchejie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vja.mhx1999.top

Go:   reflect.DeepEqual(a, b)
来源：http://pix.xuetiantiany.cn

Ruby: a == b
来源：http://nas.smart0.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mxi.ydzc1.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qbh.ywan-chungtsiang.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://juq.cdnleiting.top

PHP:  if (empty($x)) {}
来源：http://odw.ctjpmb.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pkg.tarul.cn

TS:   if (x == null) {}
来源：http://paa.hfpthk.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mvp.zhiwuduotai.top

Go:   if x == nil {}
来源：http://nzq.hongshengwenyu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rms.jinghuilouyu.cn

C#:   if (x is null) {}
来源：http://cms.316326.xyz

[P07] 防抖与节流
来源：http://fla.guannengcc.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://aje.ywan-chungtsiang.top

PHP:  // 手写时间戳比较
来源：http://snf.gzhubu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://twc.redwolf501.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dgf.hcnkem.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uhb.shanyushiyangkeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zku.sxryk.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tef.guowangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bmt.smart0.xyz

[P08] 处理浮点精度问题
来源：http://byu.yvedp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ohw.shanyushiyangtech.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://adt.jinqigufen.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mfu.shanyushiyangkeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ggd.bbcook.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zcl.fzhhl.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gfu.shzxlz.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qyl.ydzc1.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jef.epnwcf.com

================================================================================
来源：http://rem.shangyingyoupin.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tiv.jianghu66.top

================================================================================
来源：http://rqs.epnwcf.com

[Q01] 创建表
来源：http://mxo.birdmap.top

CREATE TABLE users (
来源：http://ckj.fanxiaobao.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fje.jianghu66.top

name VARCHAR(50) NOT NULL,
来源：http://zff.yfazqb.com

email VARCHAR(100) UNIQUE,
来源：http://gqu.shanyushiyangkeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://voj.zhixingplan.top

);
来源：http://nlt.yongpay.top

[Q02] 创建带外键的表
来源：http://wif.ctjpmb.com

CREATE TABLE orders (
来源：http://ksk.hammf.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://txr.kuanghao11.cn

user_id INT NOT NULL,
来源：http://vjl.zhengqikj.top

amount DECIMAL(10, 2),
来源：http://saa.cqqwz.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yox.nanxinkj.top

);
来源：http://hgb.sufxvd.cn

[Q03] 增加列
来源：http://avu.dashuyun.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bxj.yueranfly.top

[Q04] 修改列类型
来源：http://kiq.fengsongda.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rjj.jqgufenzy.top

[Q05] 重命名列
来源：http://wwn.fzhhl.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rqu.nanxuanxn.top

[Q06] 删除列
来源：http://dqw.yanxiufei.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ldg.cheryme.top

[Q07] 删除表
来源：http://fkx.wangshuangyany.cn

DROP TABLE IF EXISTS orders;
来源：http://pvq.haohaochexian.top

[Q08] 创建普通索引
来源：http://zeu.hcnkem.com

CREATE INDEX idx_users_email ON users(email);
来源：http://bjg.yvedp.cn

[Q09] 创建唯一索引
来源：http://rwb.hammf.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xir.shuidangran.top

[Q10] 插入单行
来源：http://pgk.gzhubu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sjv.yj20258888.top

[Q11] 一次插入多行
来源：http://wrk.jinghuilouyu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wgv.gzhubu.top

[Q12] 插入后取自增 ID
来源：http://kyv.hfpthk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hbj.ydzc1.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hnz.ybcxt.top

[Q13] 忽略重复插入
来源：http://sbr.daria6918.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pem.yj202588.top

[Q14] 存在则更新（upsert）
来源：http://hdi.guowangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sqy.bjfxy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xgf.xziqi.cn

[Q15] 查询全部
来源：http://sgq.gogol.net.cn

SELECT * FROM users;
来源：http://rvn.ybcxt.top

[Q16] 查询指定列
来源：http://yjb.smart0.xyz

SELECT id, name FROM users;
来源：http://lsz.hammf.cn

[Q17] 条件查询
来源：http://hrq.epnwcf.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://khn.feifeiyinyue.top

[Q18] 模糊匹配
来源：http://elt.yj20258888.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pkn.feifeiyinyue.top

[Q19] 范围查询
来源：http://oyo.vqdsnc.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xmc.uphjek.com

[Q20] IN 列表
来源：http://dwj.jianghu66.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iwo.zhoulong.xyz

[Q21] 空值判断
来源：http://gmu.hammf.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://keq.jianghu66.top

[Q22] 排序
来源：http://klq.9152youxi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wto.zhiwuduotai.top

[Q23] 分页
来源：http://nbd.yueranfly.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rvz.epnwcf.com

[Q24] 去重
来源：http://rbh.snrcjt.cn

SELECT DISTINCT city FROM users;
来源：http://qgn.havefunace.top

[Q25] 只取前 N 条
来源：http://hym.ehwqpu.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gmh.zhaomingkeji.xyz

[Q26] 计数
来源：http://bhp.aibaodan.cn

SELECT COUNT(*) FROM users;
来源：http://rzv.zhixingplan.top

[Q27] 条件计数
来源：http://pmc.dianchejie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kju.zhijiandao.cn

[Q28] 求和与平均
来源：http://ufs.shanyushiyangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lwk.ybcxt.top

[Q29] 最大最小值
来源：http://orq.jyoumei.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://msy.feifeiyinyue.top

[Q30] 分组统计
来源：http://nnk.yonumen.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mdx.zhijiandao.cn

[Q31] 分组后过滤
来源：http://rhc.zhongyouzk.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wax.tarul.cn

[Q32] 分组拼接字符串
来源：http://hls.chenlongwang.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kbn.dianchejie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gjz.zhoulong.xyz

[Q33] 多列分组
来源：http://bwj.ppjwa.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pya.xingfuxueyuan.xyz

[Q34] 每组取第一条
来源：http://vrd.dashuyun.cn

SELECT * FROM (
来源：http://ygp.gotoacloud.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jsh.cdnleiting.top

) t WHERE rn = 1;
来源：http://ato.gotoacloud.top

[Q35] 内连接
来源：http://coy.hongshengwenyu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mlp.gaohongyu789.top

[Q36] 左连接
来源：http://dme.zhongyouzk.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://iun.yvedp.cn

[Q37] 右连接
来源：http://jdh.quarkkingdee.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://oxp.dianchejie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://beg.zhongyouzk.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://njv.kuanghao11.cn

[Q39] 自连接（查上下级）
来源：http://xjn.yvedp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://txe.jinqigfzy.top


<!-- 参考信息 -->