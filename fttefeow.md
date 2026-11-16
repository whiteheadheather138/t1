代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ynp.bjfxy.top

[N06] 判断回文字符串
来源：http://dbm.tianlin.xyz

Py:   s == s[::-1]
来源：http://asq.nanxinkj.top

PHP:  $s === strrev($s);
来源：http://sew.guowangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://nav.svipenyu.cn

TS:   s === [...s].reverse().join("")
来源：http://toz.vqdsnc.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kfo.dashuyun.cn

Go:   // 双指针从两端比较
来源：http://lld.chenzaomai.com

Ruby: s == s.reverse
来源：http://cce.guowangkeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mhs.ydjk.org.cn

[N07] 两数之和（返回下标）
来源：http://wlh.ydjk.org.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jip.shanyushiyangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://isk.sweek.top

JS:   // 手写 Map：map.set(v, i)
来源：http://rbt.zhongyouzk.top

TS:   // 手写 Map<string, number>
来源：http://bzb.cheryme.top

Java: // 手写 HashMap
来源：http://xci.sjlbkw.cn

Go:   // 手写 map[int]int
来源：http://sdu.iojbl.cn

Ruby: // 手写 Hash
来源：http://prk.mhx1999.top

C#:   // 手写 Dictionary<int, int>
来源：http://hdt.zdqjudy.top

[N08] 生成全排列
来源：http://ida.hnxiangtu.top

Py:   itertools.permutations(arr)
来源：http://vvc.zdqjudy.top

PHP:  // 手写递归交换
来源：http://jgv.shangyingyoupin.top

JS:   // 手写回溯递归
来源：http://tog.tarul.cn

TS:   // 手写回溯递归
来源：http://gvx.jinqigufen.top

Java: // 手写回溯递归
来源：http://sqm.zhoulong.xyz

Go:   // 手写回溯递归
来源：http://uax.tian-w.cn

Ruby: arr.permutation.to_a
来源：http://tjd.hesvh.cn

C#:   // 手写回溯递归
来源：http://sco.chenzaomai.com

[N09] 栈与队列
来源：http://hfq.tianlin.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mnm.sweek.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nzq.kuanghao11.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cgt.yj20258.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bdb.yfazqb.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://upe.jqgfzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tly.yangfankeji.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://eqo.hfpthk.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qyp.vqdsnc.cn

[N10] 链表节点定义
来源：http://miq.chenlongwang.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://oek.vehdjk.com

PHP:  class Node { public $v; public $next = null; }
来源：http://vtb.hesvh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cbf.gogol.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gnr.cucudq.cn

Java: class Node { int v; Node next; }
来源：http://nqw.sxryk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ywr.quarkkingdee.top

Ruby: Node = Struct.new(:v, :next)
来源：http://stl.tian-w.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://oqa.jyoumei.cn

[N11] 二叉树中序遍历
来源：http://mph.sufxvd.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rmc.daxiang520.top

PHP:  // 手写递归函数
来源：http://fcp.ywan-chungtsiang.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rsw.wangdashe.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zdz.zycfv.cn

Java: // 手写递归
来源：http://utd.tarul.cn

Go:   // 手写递归
来源：http://fbs.pycfn.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qhz.jinyuanbaomall.cn

C#:   // 手写递归
来源：http://ldu.hcnkem.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gdt.ybcxt.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gja.yj20258888.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rsj.yj20258.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nxo.tianlin.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oqq.vqdsnc.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nad.zdbjq.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tgo.xingfuxueyuan.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hsa.zhaomingkeji.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ini.vqdsnc.cn

================================================================================
来源：http://mrp.smart0.xyz

O. 并发与异步
来源：http://vjs.shzxlz.cn

================================================================================
来源：http://hmc.tianlin.xyz

[O01] 启动一个线程
来源：http://gtq.iojbl.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mxg.daria6918.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lsj.hammf.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ysz.jqgufenzy.top

TS:   // 同 JS
来源：http://ugw.sxryk.cn

Java: new Thread(() -> f()).start()
来源：http://yiq.hysaishi.cn

Go:   go f()
来源：http://gvs.chenjidiqi.icu

Ruby: Thread.new { f }
来源：http://jln.shanyushiyangkeji.top

C#:   Task.Run(() => F());
来源：http://yaa.yuanzhike.top

[O02] 使用线程池
来源：http://caf.feifeiyinyue.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zxy.xinyue.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://owk.vehdjk.com

JS:   // worker_threads 线程池
来源：http://xoi.ppjwa.cn

TS:   // worker_threads 线程池
来源：http://ivo.quarkkingdee.top

Java: Executors.newFixedThreadPool(4)
来源：http://hei.aibaodan.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tjr.chenjidiqi.icu

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mhp.svipenyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ogr.quarkkingdee.top

[O03] 加锁保护共享数据
来源：http://xpr.zhiwuduotai.top

Py:   with lock: shared += 1
来源：http://jyi.jinghuilouyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://ptd.316326.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pds.gotoacloud.top

TS:   // 同 JS
来源：http://mml.ppjwa.cn

Java: synchronized (this) { shared++; }
来源：http://zob.daria6918.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://naz.jinyuanbaomall.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ovh.pycfn.com

C#:   lock (gate) { shared++; }
来源：http://umv.yj20258888.top

[O04] 定义异步函数并等待
来源：http://kni.jinghuilouyu.cn

Py:   async def f():⏎    await g()
来源：http://obu.zdqjudy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tlf.cashguo.top

JS:   async function f() { await g(); }
来源：http://mvo.tanke756.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://dlu.52xcode.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hbf.yuxming.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fzz.316326.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://xat.hongshengwenyu.top

C#:   async Task F() { await G(); }
来源：http://ukp.pengpengdd.cyou

[O05] 并发执行并等待全部完成
来源：http://xhp.hammf.cn

Py:   asyncio.gather(*tasks)
来源：http://rpz.zycfv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jyk.quarkkingdee.top

JS:   await Promise.all(tasks)
来源：http://pmb.52xcode.cn

TS:   await Promise.all(tasks)
来源：http://wiz.guannengcc.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mfv.yj202588.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://iqv.tarul.cn

Ruby: threads.map(&:join)
来源：http://axw.birdmap.top

C#:   await Task.WhenAll(t1, t2)
来源：http://foy.shzxlz.cn

[O06] 使用进程池
来源：http://dda.ctjpmb.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qkp.sufxvd.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fvu.daxiang520.top

JS:   // child_process / cluster 模块
来源：http://gxb.sweek.top

TS:   // child_process / cluster 模块
来源：http://fid.52xcode.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fia.jianghu66.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vvn.yanxiufei.cn

Ruby: // fork 块
来源：http://tnr.tianlin.xyz

C#:   Parallel.For
来源：http://fwe.yuxming.cn

================================================================================
来源：http://kvg.fehbvm.com

P. 常用工具函数
来源：http://skn.jianghu66.top

================================================================================
来源：http://txu.daxiang520.top

[P01] 生成 UUID
来源：http://fqw.tian-w.cn

Py:   str(uuid.uuid4())
来源：http://sic.cashguo.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wco.zycfv.cn

JS:   crypto.randomUUID()
来源：http://vet.bbcook.cn

TS:   crypto.randomUUID()
来源：http://iex.gaohongyu789.top

Java: UUID.randomUUID().toString()
来源：http://eyh.yfazqb.com

Go:   // 用 github.com/google/uuid
来源：http://wzt.xinyue.icu

Ruby: SecureRandom.uuid
来源：http://bwi.52xcode.cn

C#:   Guid.NewGuid().ToString()
来源：http://yhz.havefunace.top

[P02] MD5 / SHA256 摘要
来源：http://ekz.redwolf501.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nfc.jqgufenzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://xvb.nanxinkj.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://afn.ehwqpu.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://shg.ydjk.org.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://diw.cashguo.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nzg.sjlbkw.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jyl.tian-w.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://epm.fktsv.cn

[P03] 生成短随机字符串
来源：http://nln.0kj1m.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nuc.pycfn.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lji.xingfuxueyuan.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vtt.yj20258.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yes.cqqwz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lsf.xinyue.icu

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pxu.mhx1999.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://twg.sufxvd.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wdh.bjfxy.top

[P04] 求长度
来源：http://ion.zhixingplan.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mjp.sjlbkw.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xgk.c1oappe.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uqt.tarul.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dxs.yj20258.top

Java: list.size();  map.size();  s.length()
来源：http://jzw.hongshengwenyu.top

Go:   len(arr);  len(m)
来源：http://ett.andypj.xyz

Ruby: x.length;  x.size
来源：http://hbc.zycfv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pcq.dianchejie.cn

[P05] 判断两个对象内容是否相等
来源：http://jyd.feifeiyinyue.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://cxk.chenjidiqi.icu

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kqc.guannengcc.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vfj.pycfn.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jke.tarul.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ama.zhiwuduotai.top

Go:   reflect.DeepEqual(a, b)
来源：http://yja.dianchejie.cn

Ruby: a == b
来源：http://xjw.gotoacloud.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ltf.hesvh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xup.sjlbkw.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ltl.bbcook.cn

PHP:  if (empty($x)) {}
来源：http://tgp.andypj.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://irl.jqgufenzy.top

TS:   if (x == null) {}
来源：http://jdg.tanke756.top

Java: if (x == null || x.isEmpty()) {}
来源：http://eii.yj20258888.top

Go:   if x == nil {}
来源：http://uur.vehdjk.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cyi.chenlongwang.top

C#:   if (x is null) {}
来源：http://rxt.birdmap.top

[P07] 防抖与节流
来源：http://swn.zhoulong.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://egp.iojbl.cn

PHP:  // 手写时间戳比较
来源：http://kyg.fengsongda.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hyb.yangfankeji.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ixq.tanke756.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ans.quarkkingdee.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vub.zdqjudy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://nqv.ivvv.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://alu.shangyingyoupin.top

[P08] 处理浮点精度问题
来源：http://ext.iojbl.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bht.ywan-chungtsiang.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hwy.yj20258.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ulc.aizwys.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jkm.sufxvd.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://znk.chenlongwang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rao.wangdashe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zww.gaohongyu789.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bsw.ydjk.org.cn

================================================================================
来源：http://cqy.yvedp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tdc.316326.xyz

================================================================================
来源：http://ufy.dashuyun.cn

[Q01] 创建表
来源：http://utg.hysaishi.cn

CREATE TABLE users (
来源：http://isx.tarul.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jwe.yj20258.top

name VARCHAR(50) NOT NULL,
来源：http://mky.9152youxi.cn

email VARCHAR(100) UNIQUE,
来源：http://rif.nanxinkj.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tvd.zdqjudy.top

);
来源：http://chq.zdqjudy.top

[Q02] 创建带外键的表
来源：http://yzz.sxryk.cn

CREATE TABLE orders (
来源：http://ers.jlsjyb.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tfn.wangshuangyany.cn

user_id INT NOT NULL,
来源：http://jqy.zhixingplan.top

amount DECIMAL(10, 2),
来源：http://khp.quarkkingdee.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rau.ywan-chungtsiang.top

);
来源：http://wbz.zhijiandao.cn

[Q03] 增加列
来源：http://mnd.jqgfzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uln.cheryme.top

[Q04] 修改列类型
来源：http://rfh.zhiwuduotai.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kdg.fengsongda.top

[Q05] 重命名列
来源：http://xbm.ybcxt.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sfi.xylfe.cn

[Q06] 删除列
来源：http://yrx.tarul.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xee.xylfe.cn

[Q07] 删除表
来源：http://pon.52xcode.cn

DROP TABLE IF EXISTS orders;
来源：http://aih.hfpthk.cn

[Q08] 创建普通索引
来源：http://njf.0kj1m.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bax.ydzc1.top

[Q09] 创建唯一索引
来源：http://dwo.gaohongyu789.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zbd.0kj1m.cn

[Q10] 插入单行
来源：http://wyr.jiagoushi.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://elo.snrcjt.cn

[Q11] 一次插入多行
来源：http://zkf.shanyushiyangkeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://phx.ydjk.org.cn

[Q12] 插入后取自增 ID
来源：http://wmo.cucudq.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fgg.haohaochexian.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dgz.cucudq.cn

[Q13] 忽略重复插入
来源：http://szi.chenzaomai.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://iiv.hysaishi.cn

[Q14] 存在则更新（upsert）
来源：http://ftx.xingfuxueyuan.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://drx.jiagoushi.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ljv.hfpthk.cn

[Q15] 查询全部
来源：http://axy.sysykeji.top

SELECT * FROM users;
来源：http://afc.bbcook.cn

[Q16] 查询指定列
来源：http://xot.xingfuxueyuan.xyz

SELECT id, name FROM users;
来源：http://bxp.zdbjq.cn

[Q17] 条件查询
来源：http://oha.wangshuangyany.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sbo.ydzc1.top

[Q18] 模糊匹配
来源：http://frc.zhiwuduotai.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xsu.0kj1m.cn

[Q19] 范围查询
来源：http://rry.gogol.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xkx.bjfxy.top

[Q20] IN 列表
来源：http://moz.pycfn.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://atk.shanyushiyangtech.top

[Q21] 空值判断
来源：http://jlv.vehdjk.com

SELECT * FROM users WHERE email IS NULL;
来源：http://wft.yueranfly.top

[Q22] 排序
来源：http://eqf.yj20258.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://slk.zhixingplan.top

[Q23] 分页
来源：http://qsg.guowangkeji.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xdc.zdqjudy.top

[Q24] 去重
来源：http://ghz.jyoumei.cn

SELECT DISTINCT city FROM users;
来源：http://yfq.jinyuanbaomall.cn

[Q25] 只取前 N 条
来源：http://mzw.yueranfly.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jsy.ehwqpu.com

[Q26] 计数
来源：http://jbv.gogol.net.cn

SELECT COUNT(*) FROM users;
来源：http://hfe.cucudq.cn

[Q27] 条件计数
来源：http://ixv.ctjpmb.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://exi.zdqjudy.top

[Q28] 求和与平均
来源：http://pfe.c1oappe.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lgs.daria6918.cn

[Q29] 最大最小值
来源：http://gjr.havefunace.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ymh.fktsv.cn

[Q30] 分组统计
来源：http://lce.yueranfly.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ltg.wangdashe.top

[Q31] 分组后过滤
来源：http://kui.ybcxt.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zqs.sysykeji.top

[Q32] 分组拼接字符串
来源：http://ttd.zycfv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wgk.xinyue.icu

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ack.zhijiandao.cn

[Q33] 多列分组
来源：http://zxw.chenzaomai.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wjp.dashuyun.cn

[Q34] 每组取第一条
来源：http://zes.hysaishi.cn

SELECT * FROM (
来源：http://ngj.fzhhl.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xzy.jianghu66.top

) t WHERE rn = 1;
来源：http://cpd.yj20258.top

[Q35] 内连接
来源：http://klz.gogol.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://eld.jlsjyb.cn

[Q36] 左连接
来源：http://wzf.dianchejie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://icn.zhoulong.xyz

[Q37] 右连接
来源：http://ucp.cdnleiting.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qwy.hysaishi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fag.zhiwuduotai.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yfc.hnxiangtu.top

[Q39] 自连接（查上下级）
来源：http://rkq.jinghuilouyu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xmm.316326.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fkc.daria6918.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://giv.shangyingyoupin.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xfu.sjlbkw.cn

[Q41] 多表连接
来源：http://mon.zhaomingkeji.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://uwm.zhoulong.xyz

JOIN users u ON u.id = o.user_id
来源：http://vyz.gotoacloud.top

JOIN products p ON p.id = o.product_id;
来源：http://lto.daxiang520.top

[Q42] 连接条件附加过滤
来源：http://uhd.wangdashe.top


<!-- 参考信息 -->