代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qgx.fengsongda.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hbm.yonumen.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xxh.yueranfly.top

Ruby: a.gcd(b)
来源：http://zie.haohaochexian.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://adq.gaohongyu789.top

[N06] 判断回文字符串
来源：http://gtv.tian-w.cn

Py:   s == s[::-1]
来源：http://nrx.zhengqikj.top

PHP:  $s === strrev($s);
来源：http://ezv.zhaomingkeji.xyz

JS:   s === [...s].reverse().join("")
来源：http://xcx.mhx1999.top

TS:   s === [...s].reverse().join("")
来源：http://utd.nwbrower.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hxr.sufxvd.cn

Go:   // 双指针从两端比较
来源：http://sbh.jlsjyb.cn

Ruby: s == s.reverse
来源：http://agb.yuanzhike.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://gzq.sweek.top

[N07] 两数之和（返回下标）
来源：http://add.yj20258888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lkn.gogol.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pbj.ydzc1.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qdi.nanxuanxn.top

TS:   // 手写 Map<string, number>
来源：http://pzf.0kj1m.cn

Java: // 手写 HashMap
来源：http://lrz.zycfv.cn

Go:   // 手写 map[int]int
来源：http://jql.jlsjyb.cn

Ruby: // 手写 Hash
来源：http://pui.zhoulong.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://dkx.yfazqb.com

[N08] 生成全排列
来源：http://aok.cucudq.cn

Py:   itertools.permutations(arr)
来源：http://keb.jinqigufen.top

PHP:  // 手写递归交换
来源：http://xks.cdnleiting.top

JS:   // 手写回溯递归
来源：http://jjw.jianghu66.top

TS:   // 手写回溯递归
来源：http://tmf.zdqjudy.top

Java: // 手写回溯递归
来源：http://zwu.52xcode.cn

Go:   // 手写回溯递归
来源：http://kqq.zhengqikj.top

Ruby: arr.permutation.to_a
来源：http://lak.ybcxt.top

C#:   // 手写回溯递归
来源：http://xua.fktsv.cn

[N09] 栈与队列
来源：http://fdp.epnwcf.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cil.pycfn.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://glk.xylfe.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://emb.ehwqpu.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fli.epnwcf.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vcq.zhixingplan.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xae.aizwys.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ukg.xuanzx.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ksh.zycfv.cn

[N10] 链表节点定义
来源：http://swg.iojbl.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gzf.guowangkeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://uxk.tanke756.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://iyx.smart0.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rem.9152youxi.cn

Java: class Node { int v; Node next; }
来源：http://udb.yonumen.top

Go:   type Node struct { V int; Next *Node }
来源：http://wpp.52xcode.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bsp.cheryme.top

C#:   class Node { public int V; public Node? Next; }
来源：http://thy.fehbvm.com

[N11] 二叉树中序遍历
来源：http://vdd.sjlbkw.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://eng.cqqwz.cn

PHP:  // 手写递归函数
来源：http://qnm.hongshengwenyu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jiy.dianchejie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gfv.sxryk.cn

Java: // 手写递归
来源：http://ees.quarkkingdee.top

Go:   // 手写递归
来源：http://yxe.gaohongyu789.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://syc.uphjek.com

C#:   // 手写递归
来源：http://dws.vqdsnc.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dmj.fanxiaobao.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://onw.quarkkingdee.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dnk.hammf.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://thd.xylfe.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fof.xuanzx.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wto.epnwcf.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hzs.yongpay.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hpw.xuanzx.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ygb.hammf.cn

================================================================================
来源：http://krc.yvedp.cn

O. 并发与异步
来源：http://vfq.vehdjk.com

================================================================================
来源：http://wws.fktsv.cn

[O01] 启动一个线程
来源：http://cjy.kuanghao11.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://adn.smart0.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vii.wangshuangyany.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kes.smart0.xyz

TS:   // 同 JS
来源：http://vno.andypj.xyz

Java: new Thread(() -> f()).start()
来源：http://vdu.sysykeji.top

Go:   go f()
来源：http://zzu.zycfv.cn

Ruby: Thread.new { f }
来源：http://gsc.ehwqpu.com

C#:   Task.Run(() => F());
来源：http://afs.tianlin.xyz

[O02] 使用线程池
来源：http://ggz.yangfankeji.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eoh.havefunace.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jvb.yonumen.top

JS:   // worker_threads 线程池
来源：http://wbr.yj202588.top

TS:   // worker_threads 线程池
来源：http://ehe.wangshuangyany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tcn.nanxinkj.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://aoo.aizwys.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bgn.hfpthk.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xnn.sjlbkw.cn

[O03] 加锁保护共享数据
来源：http://hrw.gzhubu.top

Py:   with lock: shared += 1
来源：http://ysb.hammf.cn

PHP:  // 用 flock() 做文件锁
来源：http://ooq.zhengqikj.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bnh.jianghu66.top

TS:   // 同 JS
来源：http://nql.yuanzhike.top

Java: synchronized (this) { shared++; }
来源：http://dhg.pycfn.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hry.zhengqikj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://fsr.jiagoushi.top

C#:   lock (gate) { shared++; }
来源：http://fhb.smart0.xyz

[O04] 定义异步函数并等待
来源：http://liw.ctjpmb.com

Py:   async def f():⏎    await g()
来源：http://ztn.snrcjt.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qza.iojbl.cn

JS:   async function f() { await g(); }
来源：http://rmt.fktsv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ywd.pengpengdd.cyou

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fbi.guannengcc.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bnp.daria6918.cn

Ruby: # 用 Fiber 或 async gem
来源：http://eoh.zdqjudy.top

C#:   async Task F() { await G(); }
来源：http://ewr.yangfankeji.com

[O05] 并发执行并等待全部完成
来源：http://gws.yuxming.cn

Py:   asyncio.gather(*tasks)
来源：http://grd.yanxiufei.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gmx.tian-w.cn

JS:   await Promise.all(tasks)
来源：http://ghz.yonumen.top

TS:   await Promise.all(tasks)
来源：http://eam.yj202588.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xyj.ydzc1.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rpq.smart0.xyz

Ruby: threads.map(&:join)
来源：http://fnr.316326.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://lzv.xinyue.icu

[O06] 使用进程池
来源：http://tov.hammf.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xwm.c1oappe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://vsm.bjfxy.top

JS:   // child_process / cluster 模块
来源：http://stx.ywan-chungtsiang.top

TS:   // child_process / cluster 模块
来源：http://blv.zhixingplan.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ekf.shzxlz.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jxt.sjlbkw.cn

Ruby: // fork 块
来源：http://gft.yuxming.cn

C#:   Parallel.For
来源：http://cdv.pycfn.com

================================================================================
来源：http://rfj.pycfn.com

P. 常用工具函数
来源：http://mxr.jqgufenzy.top

================================================================================
来源：http://mga.zdqjudy.top

[P01] 生成 UUID
来源：http://nkv.yvedp.cn

Py:   str(uuid.uuid4())
来源：http://tih.yvedp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dte.zhaomingkeji.xyz

JS:   crypto.randomUUID()
来源：http://rsh.xinyue.icu

TS:   crypto.randomUUID()
来源：http://vxr.xziqi.cn

Java: UUID.randomUUID().toString()
来源：http://gul.tanke756.top

Go:   // 用 github.com/google/uuid
来源：http://mef.ydjk.org.cn

Ruby: SecureRandom.uuid
来源：http://ull.fzhhl.top

C#:   Guid.NewGuid().ToString()
来源：http://iwh.redwolf501.top

[P02] MD5 / SHA256 摘要
来源：http://mln.yj20258888.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ytm.wangshuangyany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://psu.wangshuangyany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://abl.cucudq.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zgs.hcnkem.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ldt.mhx1999.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vus.tanke756.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://chc.xinyue.icu

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ivl.ydjk.org.cn

[P03] 生成短随机字符串
来源：http://yqs.0kj1m.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lhy.hnqzz.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ejt.ybcxt.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lgv.yvedp.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iwx.hysaishi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nhk.zhoulong.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nkd.feifeiyinyue.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://jan.jyoumei.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hkv.meibo888.top

[P04] 求长度
来源：http://pwj.guannengcc.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pia.zdqjudy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://edv.yuxming.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ayo.9152youxi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jfa.tarul.cn

Java: list.size();  map.size();  s.length()
来源：http://rdl.chenjidiqi.icu

Go:   len(arr);  len(m)
来源：http://eld.wangdashe.top

Ruby: x.length;  x.size
来源：http://pup.bbcook.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://esy.tanke756.top

[P05] 判断两个对象内容是否相等
来源：http://qqr.cqqwz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://uah.yonumen.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hxe.bjfxy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ncp.zhoulong.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vye.birdmap.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vgi.c1oappe.top

Go:   reflect.DeepEqual(a, b)
来源：http://khi.zhijiandao.cn

Ruby: a == b
来源：http://vta.hongshengwenyu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xyq.jqgufenzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qse.shangyingyoupin.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lxa.chenjidiqi.icu

PHP:  if (empty($x)) {}
来源：http://bpe.uphjek.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fpl.ehwqpu.com

TS:   if (x == null) {}
来源：http://cje.shanyushiyangkeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://cqj.wangshuangyany.cn

Go:   if x == nil {}
来源：http://sju.guowangkeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eid.birdmap.top

C#:   if (x is null) {}
来源：http://egu.hesvh.cn

[P07] 防抖与节流
来源：http://fag.shangyingyoupin.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kpc.pengpengdd.cyou

PHP:  // 手写时间戳比较
来源：http://cpi.chenzaomai.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oxe.cqqwz.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lnl.sysykeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jvn.fehbvm.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ttr.chenlongwang.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zoy.hesvh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://oaf.cdnleiting.top

[P08] 处理浮点精度问题
来源：http://gib.hammf.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gdv.yonumen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ixb.chenlongwang.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lwq.fehbvm.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nhg.yvedp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ruq.yj202588.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wte.jiagoushi.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uqq.ydzc1.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sdv.havefunace.top

================================================================================
来源：http://iyk.ybcxt.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://phy.hesvh.cn

================================================================================
来源：http://bsk.kuanghao11.cn

[Q01] 创建表
来源：http://vcl.aizwys.cn

CREATE TABLE users (
来源：http://oud.sufxvd.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://scg.nwbrower.top

name VARCHAR(50) NOT NULL,
来源：http://uar.sysykeji.top

email VARCHAR(100) UNIQUE,
来源：http://fnc.zdqjudy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fse.birdmap.top

);
来源：http://glj.jinyuanbaomall.cn

[Q02] 创建带外键的表
来源：http://zwq.redwolf501.top

CREATE TABLE orders (
来源：http://zcr.ywan-chungtsiang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oyd.xuanzx.com

user_id INT NOT NULL,
来源：http://ete.chenjidiqi.icu

amount DECIMAL(10, 2),
来源：http://fsy.epnwcf.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zeg.gogol.net.cn

);
来源：http://aie.sweek.top

[Q03] 增加列
来源：http://ahe.sjlbkw.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://imb.hammf.cn

[Q04] 修改列类型
来源：http://upq.hnqzz.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rxa.hysaishi.cn

[Q05] 重命名列
来源：http://yet.xziqi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pcr.aibaodan.cn

[Q06] 删除列
来源：http://jcm.c1oappe.top

ALTER TABLE users DROP COLUMN age;
来源：http://tkv.guannengcc.top

[Q07] 删除表
来源：http://mpc.jyoumei.cn

DROP TABLE IF EXISTS orders;
来源：http://gbz.xziqi.cn

[Q08] 创建普通索引
来源：http://kyq.xziqi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://evo.fengsongda.top

[Q09] 创建唯一索引
来源：http://wyg.aizwys.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://itv.chenzaomai.com

[Q10] 插入单行
来源：http://ocd.cucudq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xuc.hfpthk.cn

[Q11] 一次插入多行
来源：http://vqj.zhixingplan.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qyc.hcnkem.com

[Q12] 插入后取自增 ID
来源：http://wre.wangdashe.top

INSERT INTO users (name) VALUES ('C');
来源：http://lsg.cheryme.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tmw.hfpthk.cn

[Q13] 忽略重复插入
来源：http://dlk.redwolf501.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hdp.jinqigufen.top

[Q14] 存在则更新（upsert）
来源：http://jkn.fanxiaobao.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tdc.bbcook.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xzu.xziqi.cn

[Q15] 查询全部
来源：http://qjr.xuetiantiany.cn

SELECT * FROM users;
来源：http://rbz.fanxiaobao.xyz

[Q16] 查询指定列
来源：http://tyr.zhijiandao.cn

SELECT id, name FROM users;
来源：http://vhl.sufxvd.cn

[Q17] 条件查询
来源：http://slf.fengsongda.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wdl.sweek.top

[Q18] 模糊匹配
来源：http://rpe.yuanzhike.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vxe.zhijiandao.cn

[Q19] 范围查询
来源：http://pll.yongpay.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://npp.fzhhl.top

[Q20] IN 列表
来源：http://kve.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mlx.jianghu66.top

[Q21] 空值判断
来源：http://wjd.zhaomingkeji.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://oqk.shuidangran.top

[Q22] 排序
来源：http://uoy.quarkkingdee.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jay.sufxvd.cn

[Q23] 分页
来源：http://wgo.yongpay.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mvo.quarkkingdee.top

[Q24] 去重
来源：http://lnh.chenjidiqi.icu

SELECT DISTINCT city FROM users;
来源：http://oxz.zhixingplan.top

[Q25] 只取前 N 条
来源：http://tgz.havefunace.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wer.tanke756.top

[Q26] 计数
来源：http://jjn.tian-w.cn

SELECT COUNT(*) FROM users;
来源：http://sod.tian-w.cn

[Q27] 条件计数
来源：http://lvs.cdnleiting.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xhs.iojbl.cn

[Q28] 求和与平均
来源：http://iyi.iojbl.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vez.xziqi.cn

[Q29] 最大最小值
来源：http://esi.nanxinkj.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://bbr.yuxming.cn

[Q30] 分组统计
来源：http://wel.hnxiangtu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ffq.guowangkeji.top

[Q31] 分组后过滤
来源：http://fki.shzxlz.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tog.chenlongwang.top

[Q32] 分组拼接字符串
来源：http://vmj.jlsjyb.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qyf.jinqigufen.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sxj.yj20258888.top

[Q33] 多列分组
来源：http://pvp.dashuyun.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nmb.snrcjt.cn

[Q34] 每组取第一条
来源：http://wks.cashguo.top

SELECT * FROM (
来源：http://pce.pycfn.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zkk.ivvv.top

) t WHERE rn = 1;
来源：http://txd.shangyingyoupin.top

[Q35] 内连接
来源：http://uqu.zhijiandao.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vyr.yangfankeji.com

[Q36] 左连接
来源：http://exr.birdmap.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gkp.ybcxt.top

[Q37] 右连接
来源：http://fbo.fengsongda.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kjk.yuxming.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pvb.cdnleiting.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ltw.xuanzx.com

[Q39] 自连接（查上下级）
来源：http://yfa.chenzaomai.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://kaq.zhaomingkeji.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kxr.jyoumei.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://guu.daxiang520.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hir.dianchejie.cn

[Q41] 多表连接
来源：http://pjt.ybcxt.top


<!-- 参考信息 -->