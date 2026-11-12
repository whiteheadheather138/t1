代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://zix.gaohongyu789.top

TS:   s === [...s].reverse().join("")
来源：http://xpv.yj20258888.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zuy.shzxlz.cn

Go:   // 双指针从两端比较
来源：http://vry.sufxvd.cn

Ruby: s == s.reverse
来源：http://zhb.ybcxt.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://rbs.jinghuilouyu.cn

[N07] 两数之和（返回下标）
来源：http://mht.redwolf501.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rav.epnwcf.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kkt.sysykeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://dtp.mhx1999.top

TS:   // 手写 Map<string, number>
来源：http://ruo.yueranfly.top

Java: // 手写 HashMap
来源：http://dqc.jiagoushi.top

Go:   // 手写 map[int]int
来源：http://kvr.hesvh.cn

Ruby: // 手写 Hash
来源：http://rpn.yvedp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://def.fktsv.cn

[N08] 生成全排列
来源：http://nkl.yj202588.top

Py:   itertools.permutations(arr)
来源：http://lqa.mhx1999.top

PHP:  // 手写递归交换
来源：http://cmk.nwbrower.top

JS:   // 手写回溯递归
来源：http://xla.zdqjudy.top

TS:   // 手写回溯递归
来源：http://nwc.pengpengdd.cyou

Java: // 手写回溯递归
来源：http://wit.dianchejie.cn

Go:   // 手写回溯递归
来源：http://ucq.jinqigfzy.top

Ruby: arr.permutation.to_a
来源：http://cuv.shanyushiyangkeji.top

C#:   // 手写回溯递归
来源：http://zpm.52xcode.cn

[N09] 栈与队列
来源：http://ywv.yj20258.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gxm.yuxming.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bvh.zhiwuduotai.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zgt.dashuyun.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://evr.shanyushiyangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://iyg.havefunace.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ajq.hfpthk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fty.shanyushiyangkeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://msj.yj20258888.top

[N10] 链表节点定义
来源：http://mvo.chenjidiqi.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fjg.c1oappe.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mry.xylfe.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lux.epnwcf.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tic.xuanzx.com

Java: class Node { int v; Node next; }
来源：http://ryb.jyoumei.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hff.daxiang520.top

Ruby: Node = Struct.new(:v, :next)
来源：http://tkj.hnxiangtu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://cbt.andypj.xyz

[N11] 二叉树中序遍历
来源：http://ula.jqgufenzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://czx.guowangkeji.top

PHP:  // 手写递归函数
来源：http://lzn.cdnleiting.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nul.jinqigufen.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://htp.shanyushiyangtech.top

Java: // 手写递归
来源：http://aqf.shzxlz.cn

Go:   // 手写递归
来源：http://sja.xinyue.icu

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mea.fktsv.cn

C#:   // 手写递归
来源：http://yye.guannengcc.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yxg.mhx1999.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kif.tarul.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://npz.hnqzz.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lbi.hongshengwenyu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fmh.cucudq.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tcp.dianchejie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jrd.hcnkem.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dcj.vehdjk.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qwb.fanxiaobao.xyz

================================================================================
来源：http://aej.xingfuxueyuan.xyz

O. 并发与异步
来源：http://xrp.yanxiufei.cn

================================================================================
来源：http://rzi.fehbvm.com

[O01] 启动一个线程
来源：http://uga.hysaishi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cpq.quarkkingdee.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mkc.xuetiantiany.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lvv.nanxuanxn.top

TS:   // 同 JS
来源：http://lda.nanxinkj.top

Java: new Thread(() -> f()).start()
来源：http://dim.cashguo.top

Go:   go f()
来源：http://uze.pycfn.com

Ruby: Thread.new { f }
来源：http://xkm.vqdsnc.cn

C#:   Task.Run(() => F());
来源：http://ocj.nwbrower.top

[O02] 使用线程池
来源：http://iay.52xcode.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sdo.fktsv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dut.yueranfly.top

JS:   // worker_threads 线程池
来源：http://mft.birdmap.top

TS:   // worker_threads 线程池
来源：http://xvt.uphjek.com

Java: Executors.newFixedThreadPool(4)
来源：http://ydi.yj20258.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ixc.c1oappe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dqu.hnxiangtu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wld.tanke756.top

[O03] 加锁保护共享数据
来源：http://ify.nanxinkj.top

Py:   with lock: shared += 1
来源：http://xkk.bbcook.cn

PHP:  // 用 flock() 做文件锁
来源：http://url.yonumen.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://efx.jyoumei.cn

TS:   // 同 JS
来源：http://lof.yj20258.top

Java: synchronized (this) { shared++; }
来源：http://vwl.0kj1m.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://npx.yuxming.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gia.jinqigufen.top

C#:   lock (gate) { shared++; }
来源：http://vpt.vqdsnc.cn

[O04] 定义异步函数并等待
来源：http://vnz.bjfxy.top

Py:   async def f():⏎    await g()
来源：http://avl.bjfxy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://myh.jinyuanbaomall.cn

JS:   async function f() { await g(); }
来源：http://ewf.havefunace.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://mcw.guannengcc.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gpo.yfazqb.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://etx.jyoumei.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bwp.jinqigfzy.top

C#:   async Task F() { await G(); }
来源：http://sam.tanke756.top

[O05] 并发执行并等待全部完成
来源：http://kzu.yongpay.top

Py:   asyncio.gather(*tasks)
来源：http://gjw.xuanzx.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fes.ehwqpu.com

JS:   await Promise.all(tasks)
来源：http://kwh.hywenlv.cn

TS:   await Promise.all(tasks)
来源：http://vbs.9152youxi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ksu.zhixingplan.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mog.pycfn.com

Ruby: threads.map(&:join)
来源：http://ifk.birdmap.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fro.zhixingplan.top

[O06] 使用进程池
来源：http://vxt.epnwcf.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zbv.gogol.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://iwj.zhoulong.xyz

JS:   // child_process / cluster 模块
来源：http://xzu.zycfv.cn

TS:   // child_process / cluster 模块
来源：http://dax.shangyingyoupin.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oxw.xuetiantiany.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xpk.wangdashe.top

Ruby: // fork 块
来源：http://piu.chenjidiqi.icu

C#:   Parallel.For
来源：http://nts.guowangkeji.top

================================================================================
来源：http://lvd.redwolf501.top

P. 常用工具函数
来源：http://cvc.hammf.cn

================================================================================
来源：http://vfl.xziqi.cn

[P01] 生成 UUID
来源：http://cfy.tian-w.cn

Py:   str(uuid.uuid4())
来源：http://awf.sysykeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rji.vqdsnc.cn

JS:   crypto.randomUUID()
来源：http://bog.iojbl.cn

TS:   crypto.randomUUID()
来源：http://tkz.ywan-chungtsiang.top

Java: UUID.randomUUID().toString()
来源：http://mss.hnqzz.top

Go:   // 用 github.com/google/uuid
来源：http://zle.zhaomingkeji.xyz

Ruby: SecureRandom.uuid
来源：http://cey.vehdjk.com

C#:   Guid.NewGuid().ToString()
来源：http://tis.kuanghao11.cn

[P02] MD5 / SHA256 摘要
来源：http://icu.shanyushiyangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hqi.yfazqb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://okt.jlsjyb.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uds.yuanzhike.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://whv.yj20258888.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://knh.xylfe.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://auy.shanyushiyangkeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kar.hongshengwenyu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://txz.yuxming.cn

[P03] 生成短随机字符串
来源：http://wha.cashguo.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wgm.yueranfly.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vtv.daria6918.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ype.andypj.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xjk.zdqjudy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mhu.redwolf501.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rsv.jinghuilouyu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fwn.316326.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yru.zdqjudy.top

[P04] 求长度
来源：http://xzu.jyoumei.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jzw.yuanzhike.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hse.xuetiantiany.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aoi.tian-w.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ggs.jinghuilouyu.cn

Java: list.size();  map.size();  s.length()
来源：http://pcj.jinghuilouyu.cn

Go:   len(arr);  len(m)
来源：http://gva.cashguo.top

Ruby: x.length;  x.size
来源：http://fvi.epnwcf.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://jay.fanxiaobao.xyz

[P05] 判断两个对象内容是否相等
来源：http://sfl.gogol.net.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ttb.yanxiufei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://abm.zhiwuduotai.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wds.ivvv.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://osw.hnxiangtu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ego.guowangkeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://edd.bjfxy.top

Ruby: a == b
来源：http://hob.zdbjq.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://whz.hywenlv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fvu.ydzc1.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sht.jiagoushi.top

PHP:  if (empty($x)) {}
来源：http://qaj.chenzaomai.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://now.bbcook.cn

TS:   if (x == null) {}
来源：http://vyj.zhaomingkeji.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://cwo.ehwqpu.com

Go:   if x == nil {}
来源：http://zep.zhengqikj.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xpr.wangdashe.top

C#:   if (x is null) {}
来源：http://ium.redwolf501.top

[P07] 防抖与节流
来源：http://qng.zdbjq.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sky.cucudq.cn

PHP:  // 手写时间戳比较
来源：http://cyv.yueranfly.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fir.zhaomingkeji.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eoc.hongshengwenyu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ehm.daria6918.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://byg.zhongyouzk.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wqt.9152youxi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hbt.gzhubu.top

[P08] 处理浮点精度问题
来源：http://nih.dashuyun.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://efs.tian-w.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qdu.yonumen.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dxe.nanxinkj.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cry.fzhhl.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hpk.dianchejie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uts.meibo888.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bpp.ctjpmb.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kjd.yfazqb.com

================================================================================
来源：http://fjp.yfazqb.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kqd.yanxiufei.cn

================================================================================
来源：http://pil.gaohongyu789.top

[Q01] 创建表
来源：http://wsj.chenlongwang.top

CREATE TABLE users (
来源：http://odo.zhongyouzk.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sra.sufxvd.cn

name VARCHAR(50) NOT NULL,
来源：http://sgp.svipenyu.cn

email VARCHAR(100) UNIQUE,
来源：http://lup.yj202588.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bcu.yongpay.top

);
来源：http://ajr.jinqigufen.top

[Q02] 创建带外键的表
来源：http://gbx.hnxiangtu.top

CREATE TABLE orders (
来源：http://ril.shanyushiyangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ypb.redwolf501.top

user_id INT NOT NULL,
来源：http://rtt.xinyue.icu

amount DECIMAL(10, 2),
来源：http://qyg.shanyushiyangtech.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sls.zhijiandao.cn

);
来源：http://vdw.sysykeji.top

[Q03] 增加列
来源：http://rcc.hysaishi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yju.ctjpmb.com

[Q04] 修改列类型
来源：http://qlk.zhiwuduotai.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zwz.jiagoushi.top

[Q05] 重命名列
来源：http://wrj.nanxinkj.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lph.zhoulong.xyz

[Q06] 删除列
来源：http://vnh.jinyuanbaomall.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gxg.aibaodan.cn

[Q07] 删除表
来源：http://icy.yangfankeji.com

DROP TABLE IF EXISTS orders;
来源：http://oym.hfpthk.cn

[Q08] 创建普通索引
来源：http://uvh.zhongyouzk.top

CREATE INDEX idx_users_email ON users(email);
来源：http://wvi.tanke756.top

[Q09] 创建唯一索引
来源：http://bwd.yongpay.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://eah.hammf.cn

[Q10] 插入单行
来源：http://mwn.c1oappe.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://iis.xziqi.cn

[Q11] 一次插入多行
来源：http://rdb.fanxiaobao.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xey.shangyingyoupin.top

[Q12] 插入后取自增 ID
来源：http://grn.zhongyouzk.top

INSERT INTO users (name) VALUES ('C');
来源：http://trg.c1oappe.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pnv.xingfuxueyuan.xyz

[Q13] 忽略重复插入
来源：http://ogf.yuxming.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gkt.epnwcf.com

[Q14] 存在则更新（upsert）
来源：http://mhl.cdnleiting.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wad.chenlongwang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kai.zdbjq.cn

[Q15] 查询全部
来源：http://rvm.shanyushiyangtech.top

SELECT * FROM users;
来源：http://ywi.jyoumei.cn

[Q16] 查询指定列
来源：http://kuh.ywan-chungtsiang.top

SELECT id, name FROM users;
来源：http://vvt.ydjk.org.cn

[Q17] 条件查询
来源：http://frd.shuidangran.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fdj.sjlbkw.cn

[Q18] 模糊匹配
来源：http://lyj.hnqzz.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jry.ybcxt.top

[Q19] 范围查询
来源：http://voi.zhiwuduotai.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wog.52xcode.cn

[Q20] IN 列表
来源：http://iln.0kj1m.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kpa.sxryk.cn

[Q21] 空值判断
来源：http://flk.yj20258888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://pdc.jqgfzy.top

[Q22] 排序
来源：http://ovn.aibaodan.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pnf.havefunace.top

[Q23] 分页
来源：http://pwn.tian-w.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ilo.nanxuanxn.top

[Q24] 去重
来源：http://cok.kuanghao11.cn

SELECT DISTINCT city FROM users;
来源：http://ygt.xingfuxueyuan.xyz

[Q25] 只取前 N 条
来源：http://ear.zhengqikj.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ckz.hnxiangtu.top

[Q26] 计数
来源：http://mmk.epnwcf.com

SELECT COUNT(*) FROM users;
来源：http://pyy.daria6918.cn

[Q27] 条件计数
来源：http://wcl.xingfuxueyuan.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wao.yueranfly.top

[Q28] 求和与平均
来源：http://aaq.yongpay.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ipf.zhaomingkeji.xyz

[Q29] 最大最小值
来源：http://vow.jinqigufen.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jns.jinghuilouyu.cn

[Q30] 分组统计
来源：http://dfc.tianlin.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cfv.tian-w.cn

[Q31] 分组后过滤
来源：http://ldj.hysaishi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tbb.sjlbkw.cn

[Q32] 分组拼接字符串
来源：http://vbc.yuanzhike.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tbo.sxryk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sex.zdqjudy.top

[Q33] 多列分组
来源：http://cnw.fengsongda.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qkk.hnxiangtu.top

[Q34] 每组取第一条
来源：http://nnl.cashguo.top

SELECT * FROM (
来源：http://dqq.fengsongda.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fbs.bjfxy.top

) t WHERE rn = 1;
来源：http://yri.gogol.net.cn

[Q35] 内连接
来源：http://hay.chenjidiqi.icu

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fnb.smart0.xyz

[Q36] 左连接
来源：http://jgw.yj202588.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tmz.jinyuanbaomall.cn

[Q37] 右连接
来源：http://oej.daxiang520.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bzy.hcnkem.com

[Q38] 全外连接（PostgreSQL）
来源：http://uqy.dianchejie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tof.andypj.xyz

[Q39] 自连接（查上下级）
来源：http://ewu.chenjidiqi.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://hmu.hongshengwenyu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://trj.yongpay.top

[Q40] 交叉连接（笛卡尔积）
来源：http://kna.zhixingplan.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://szo.guowangkeji.top

[Q41] 多表连接
来源：http://ahw.yuanzhike.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://yea.fzhhl.top

JOIN users u ON u.id = o.user_id
来源：http://fba.tianlin.xyz

JOIN products p ON p.id = o.product_id;
来源：http://mbu.guowangkeji.top

[Q42] 连接条件附加过滤
来源：http://aqm.jinqigufen.top

SELECT u.name, o.amount FROM users u
来源：http://xem.yj20258888.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fet.hysaishi.cn

[Q43] 标量子查询
来源：http://efz.yangfankeji.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kot.zdbjq.cn


<!-- 参考信息 -->