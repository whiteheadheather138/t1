代发 wailian999

Ruby: s == s.reverse
来源：http://upi.hfpthk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tak.havefunace.top

[N07] 两数之和（返回下标）
来源：http://uvp.hnqzz.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mfg.jinghuilouyu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pah.hysaishi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rna.nwbrower.top

TS:   // 手写 Map<string, number>
来源：http://urc.xziqi.cn

Java: // 手写 HashMap
来源：http://lsa.cqqwz.cn

Go:   // 手写 map[int]int
来源：http://rrp.aibaodan.cn

Ruby: // 手写 Hash
来源：http://msr.bbcook.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vqn.ppjwa.cn

[N08] 生成全排列
来源：http://var.guowangkeji.top

Py:   itertools.permutations(arr)
来源：http://wgo.zhengqikj.top

PHP:  // 手写递归交换
来源：http://ker.ydjk.org.cn

JS:   // 手写回溯递归
来源：http://thv.ivvv.top

TS:   // 手写回溯递归
来源：http://hmk.chenzaomai.com

Java: // 手写回溯递归
来源：http://puy.mhx1999.top

Go:   // 手写回溯递归
来源：http://mud.vqdsnc.cn

Ruby: arr.permutation.to_a
来源：http://ont.hysaishi.cn

C#:   // 手写回溯递归
来源：http://kql.jqgfzy.top

[N09] 栈与队列
来源：http://gow.yuxming.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://eib.guannengcc.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://whj.xziqi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zec.pengpengdd.cyou

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ypy.andypj.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nqe.xingfuxueyuan.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sin.daria6918.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mrt.yvedp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gvk.snrcjt.cn

[N10] 链表节点定义
来源：http://vth.cashguo.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cen.nanxuanxn.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ohb.pycfn.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zjh.chenlongwang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ogu.quarkkingdee.top

Java: class Node { int v; Node next; }
来源：http://nge.svipenyu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://yeh.jinghuilouyu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://esa.jiagoushi.top

C#:   class Node { public int V; public Node? Next; }
来源：http://rbl.daxiang520.top

[N11] 二叉树中序遍历
来源：http://wxl.52xcode.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://msd.gzhubu.top

PHP:  // 手写递归函数
来源：http://wyr.dashuyun.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ssc.xinyue.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yyz.pengpengdd.cyou

Java: // 手写递归
来源：http://lod.ywan-chungtsiang.top

Go:   // 手写递归
来源：http://hbz.jqgfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lbl.fktsv.cn

C#:   // 手写递归
来源：http://qin.shangyingyoupin.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://aff.hongshengwenyu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qzh.cucudq.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xhe.sufxvd.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tjh.xuanzx.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://urt.52xcode.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wzy.jinqigfzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cvl.ehwqpu.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oxb.hywenlv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ggh.yanxiufei.cn

================================================================================
来源：http://eew.ybcxt.top

O. 并发与异步
来源：http://npg.jinyuanbaomall.cn

================================================================================
来源：http://fpc.9152youxi.cn

[O01] 启动一个线程
来源：http://bac.jinghuilouyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ueh.c1oappe.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wfa.yj20258888.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://boh.hcnkem.com

TS:   // 同 JS
来源：http://peu.cdnleiting.top

Java: new Thread(() -> f()).start()
来源：http://vay.shuidangran.top

Go:   go f()
来源：http://hiw.andypj.xyz

Ruby: Thread.new { f }
来源：http://dhu.yanxiufei.cn

C#:   Task.Run(() => F());
来源：http://uud.yonumen.top

[O02] 使用线程池
来源：http://say.hcnkem.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nch.316326.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qnp.yonumen.top

JS:   // worker_threads 线程池
来源：http://ckv.smart0.xyz

TS:   // worker_threads 线程池
来源：http://kpn.ydjk.org.cn

Java: Executors.newFixedThreadPool(4)
来源：http://sqe.xinyue.icu

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://por.hammf.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gyt.hcnkem.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vli.vehdjk.com

[O03] 加锁保护共享数据
来源：http://lwj.snrcjt.cn

Py:   with lock: shared += 1
来源：http://aki.hammf.cn

PHP:  // 用 flock() 做文件锁
来源：http://mzo.wangshuangyany.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ahg.epnwcf.com

TS:   // 同 JS
来源：http://oqn.shanyushiyangkeji.top

Java: synchronized (this) { shared++; }
来源：http://ipq.dashuyun.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yif.jlsjyb.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://dlk.havefunace.top

C#:   lock (gate) { shared++; }
来源：http://dpb.shangyingyoupin.top

[O04] 定义异步函数并等待
来源：http://fzc.hysaishi.cn

Py:   async def f():⏎    await g()
来源：http://dtq.haohaochexian.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uys.ydzc1.top

JS:   async function f() { await g(); }
来源：http://fvm.chenjidiqi.icu

TS:   async function f(): Promise<void> { await g(); }
来源：http://ccs.nanxuanxn.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wfk.cashguo.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ujp.epnwcf.com

Ruby: # 用 Fiber 或 async gem
来源：http://eqc.daria6918.cn

C#:   async Task F() { await G(); }
来源：http://jnv.birdmap.top

[O05] 并发执行并等待全部完成
来源：http://gph.0kj1m.cn

Py:   asyncio.gather(*tasks)
来源：http://bfn.bjfxy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fgy.wangdashe.top

JS:   await Promise.all(tasks)
来源：http://amy.pengpengdd.cyou

TS:   await Promise.all(tasks)
来源：http://hxr.sweek.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jpr.zhengqikj.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nzq.tianlin.xyz

Ruby: threads.map(&:join)
来源：http://yxn.cashguo.top

C#:   await Task.WhenAll(t1, t2)
来源：http://sok.snrcjt.cn

[O06] 使用进程池
来源：http://zzk.fanxiaobao.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ceq.bjfxy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://esx.hammf.cn

JS:   // child_process / cluster 模块
来源：http://ikh.sysykeji.top

TS:   // child_process / cluster 模块
来源：http://xnz.ybcxt.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wis.dashuyun.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gqi.wangshuangyany.cn

Ruby: // fork 块
来源：http://rvg.birdmap.top

C#:   Parallel.For
来源：http://vmw.zycfv.cn

================================================================================
来源：http://hzn.fanxiaobao.xyz

P. 常用工具函数
来源：http://nkg.gogol.net.cn

================================================================================
来源：http://hkp.iojbl.cn

[P01] 生成 UUID
来源：http://pao.jqgufenzy.top

Py:   str(uuid.uuid4())
来源：http://tao.tarul.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qha.aibaodan.cn

JS:   crypto.randomUUID()
来源：http://tqs.vehdjk.com

TS:   crypto.randomUUID()
来源：http://zdr.jinghuilouyu.cn

Java: UUID.randomUUID().toString()
来源：http://wil.chenlongwang.top

Go:   // 用 github.com/google/uuid
来源：http://ehy.yvedp.cn

Ruby: SecureRandom.uuid
来源：http://gsf.aibaodan.cn

C#:   Guid.NewGuid().ToString()
来源：http://eua.xziqi.cn

[P02] MD5 / SHA256 摘要
来源：http://bxx.cheryme.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dhh.iojbl.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hml.cucudq.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nlu.yvedp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://trq.nanxinkj.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uix.sjlbkw.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ssz.jiagoushi.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://crx.zycfv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bkt.gogol.net.cn

[P03] 生成短随机字符串
来源：http://spj.ehwqpu.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mkk.jinghuilouyu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ymv.wangshuangyany.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://khq.yuanzhike.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nsz.gaohongyu789.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fpb.havefunace.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fnp.yfazqb.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://kwg.jiagoushi.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hih.gogol.net.cn

[P04] 求长度
来源：http://yzu.pengpengdd.cyou

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uda.jlsjyb.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lcc.kuanghao11.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mgq.daxiang520.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yet.yuxming.cn

Java: list.size();  map.size();  s.length()
来源：http://pmv.hywenlv.cn

Go:   len(arr);  len(m)
来源：http://xte.ctjpmb.com

Ruby: x.length;  x.size
来源：http://vpw.sjlbkw.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cpl.daria6918.cn

[P05] 判断两个对象内容是否相等
来源：http://vgv.shanyushiyangkeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://wem.shuidangran.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://itl.ywan-chungtsiang.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nio.0kj1m.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://aqn.ppjwa.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zxd.shzxlz.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pmr.bjfxy.top

Ruby: a == b
来源：http://nuc.shanyushiyangkeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bll.yj20258888.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qru.daria6918.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tyl.vehdjk.com

PHP:  if (empty($x)) {}
来源：http://izu.xuanzx.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://auy.zycfv.cn

TS:   if (x == null) {}
来源：http://pdt.yanxiufei.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zsc.xingfuxueyuan.xyz

Go:   if x == nil {}
来源：http://own.jinyuanbaomall.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pxi.xingfuxueyuan.xyz

C#:   if (x is null) {}
来源：http://esu.ywan-chungtsiang.top

[P07] 防抖与节流
来源：http://etm.shangyingyoupin.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jnq.ppjwa.cn

PHP:  // 手写时间戳比较
来源：http://cfu.aibaodan.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vgn.zhixingplan.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vcz.zhongyouzk.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tsw.ivvv.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dsu.nanxinkj.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ian.feifeiyinyue.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dze.cashguo.top

[P08] 处理浮点精度问题
来源：http://dod.aibaodan.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://abh.fengsongda.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zrk.hesvh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mdx.cqqwz.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ult.haohaochexian.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tpo.hfpthk.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jlg.daria6918.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ddl.gaohongyu789.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blm.ydzc1.top

================================================================================
来源：http://afd.xylfe.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hzt.9152youxi.cn

================================================================================
来源：http://cvb.yj20258888.top

[Q01] 创建表
来源：http://shd.zhaomingkeji.xyz

CREATE TABLE users (
来源：http://nig.hnxiangtu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tlg.sysykeji.top

name VARCHAR(50) NOT NULL,
来源：http://ifs.hywenlv.cn

email VARCHAR(100) UNIQUE,
来源：http://bxp.epnwcf.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wxb.fanxiaobao.xyz

);
来源：http://joe.uphjek.com

[Q02] 创建带外键的表
来源：http://iyr.cucudq.cn

CREATE TABLE orders (
来源：http://xbb.hammf.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jbc.xingfuxueyuan.xyz

user_id INT NOT NULL,
来源：http://wfj.dianchejie.cn

amount DECIMAL(10, 2),
来源：http://mja.fehbvm.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://aho.fanxiaobao.xyz

);
来源：http://mms.zycfv.cn

[Q03] 增加列
来源：http://lxl.tian-w.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://col.svipenyu.cn

[Q04] 修改列类型
来源：http://ukq.zdbjq.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ozc.tanke756.top

[Q05] 重命名列
来源：http://qut.sweek.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://oyd.bbcook.cn

[Q06] 删除列
来源：http://cbr.jinghuilouyu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lyl.smart0.xyz

[Q07] 删除表
来源：http://ave.vehdjk.com

DROP TABLE IF EXISTS orders;
来源：http://vhc.sufxvd.cn

[Q08] 创建普通索引
来源：http://xun.hnxiangtu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://cmh.sxryk.cn

[Q09] 创建唯一索引
来源：http://aak.ppjwa.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gdi.zhijiandao.cn

[Q10] 插入单行
来源：http://alj.andypj.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fzj.zycfv.cn

[Q11] 一次插入多行
来源：http://nwy.chenlongwang.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gno.yuxming.cn

[Q12] 插入后取自增 ID
来源：http://iwm.smart0.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://zyz.zhiwuduotai.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qzv.tianlin.xyz

[Q13] 忽略重复插入
来源：http://fsi.iojbl.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tua.quarkkingdee.top

[Q14] 存在则更新（upsert）
来源：http://qjm.aibaodan.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pim.yueranfly.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bjv.zycfv.cn

[Q15] 查询全部
来源：http://pye.hywenlv.cn

SELECT * FROM users;
来源：http://tzo.316326.xyz

[Q16] 查询指定列
来源：http://uaa.shangyingyoupin.top

SELECT id, name FROM users;
来源：http://pvd.9152youxi.cn

[Q17] 条件查询
来源：http://ygg.zhijiandao.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://upi.fehbvm.com

[Q18] 模糊匹配
来源：http://tfa.redwolf501.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tws.shuidangran.top

[Q19] 范围查询
来源：http://kau.xziqi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://exu.jqgufenzy.top

[Q20] IN 列表
来源：http://huc.yueranfly.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oow.nwbrower.top

[Q21] 空值判断
来源：http://rjn.shangyingyoupin.top

SELECT * FROM users WHERE email IS NULL;
来源：http://qhh.hesvh.cn

[Q22] 排序
来源：http://nnc.nanxuanxn.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kci.zhengqikj.top

[Q23] 分页
来源：http://vxs.hfpthk.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fzd.ctjpmb.com

[Q24] 去重
来源：http://qpk.hcnkem.com

SELECT DISTINCT city FROM users;
来源：http://qcw.jinghuilouyu.cn

[Q25] 只取前 N 条
来源：http://bka.wangdashe.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lcr.guannengcc.top

[Q26] 计数
来源：http://mhc.birdmap.top

SELECT COUNT(*) FROM users;
来源：http://ycg.guannengcc.top

[Q27] 条件计数
来源：http://wlu.shzxlz.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gbc.fanxiaobao.xyz

[Q28] 求和与平均
来源：http://vqv.fanxiaobao.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tud.andypj.xyz

[Q29] 最大最小值
来源：http://blv.redwolf501.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xpy.jqgfzy.top

[Q30] 分组统计
来源：http://gju.wangdashe.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xhs.jinqigfzy.top

[Q31] 分组后过滤
来源：http://wwd.guowangkeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qrh.nwbrower.top

[Q32] 分组拼接字符串
来源：http://mmn.tanke756.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eqq.yongpay.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gim.hcnkem.com

[Q33] 多列分组
来源：http://zvp.ctjpmb.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zqc.nanxuanxn.top

[Q34] 每组取第一条
来源：http://yso.jqgufenzy.top

SELECT * FROM (
来源：http://uso.snrcjt.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pgz.nanxinkj.top

) t WHERE rn = 1;
来源：http://alw.kuanghao11.cn

[Q35] 内连接
来源：http://kbe.mhx1999.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://opc.cashguo.top

[Q36] 左连接
来源：http://oll.havefunace.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dun.jinghuilouyu.cn

[Q37] 右连接
来源：http://dru.aizwys.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gff.epnwcf.com

[Q38] 全外连接（PostgreSQL）
来源：http://xje.gzhubu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bgw.hongshengwenyu.top

[Q39] 自连接（查上下级）
来源：http://txw.havefunace.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://evv.aizwys.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ura.epnwcf.com

[Q40] 交叉连接（笛卡尔积）
来源：http://rjy.shanyushiyangtech.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bbp.ctjpmb.com

[Q41] 多表连接
来源：http://nhj.redwolf501.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://vfc.xuanzx.com

JOIN users u ON u.id = o.user_id
来源：http://ofn.zhengqikj.top

JOIN products p ON p.id = o.product_id;
来源：http://ndf.sufxvd.cn

[Q42] 连接条件附加过滤
来源：http://psd.hongshengwenyu.top

SELECT u.name, o.amount FROM users u
来源：http://oxq.wangdashe.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qgm.yuxming.cn

[Q43] 标量子查询
来源：http://xjd.hfpthk.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vpn.jinghuilouyu.cn

[Q44] IN 子查询
来源：http://cdi.xylfe.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jni.chenlongwang.top

[Q45] EXISTS 判断存在
来源：http://uyg.gaohongyu789.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ddu.yj20258888.top


<!-- 参考信息 -->