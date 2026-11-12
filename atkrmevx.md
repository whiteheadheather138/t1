代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mbc.sjlbkw.cn

[N06] 判断回文字符串
来源：http://rmf.gogol.net.cn

Py:   s == s[::-1]
来源：http://czu.xylfe.cn

PHP:  $s === strrev($s);
来源：http://kmu.xylfe.cn

JS:   s === [...s].reverse().join("")
来源：http://rzg.aizwys.cn

TS:   s === [...s].reverse().join("")
来源：http://byd.pycfn.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xdu.tanke756.top

Go:   // 双指针从两端比较
来源：http://bxh.fehbvm.com

Ruby: s == s.reverse
来源：http://pxk.cucudq.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://bec.dashuyun.cn

[N07] 两数之和（返回下标）
来源：http://eab.shangyingyoupin.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xxh.pycfn.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zxe.daxiang520.top

JS:   // 手写 Map：map.set(v, i)
来源：http://dtc.zdqjudy.top

TS:   // 手写 Map<string, number>
来源：http://fib.jqgfzy.top

Java: // 手写 HashMap
来源：http://juk.zdbjq.cn

Go:   // 手写 map[int]int
来源：http://wgj.ydjk.org.cn

Ruby: // 手写 Hash
来源：http://oxs.jinghuilouyu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dul.yuxming.cn

[N08] 生成全排列
来源：http://uxc.haohaochexian.top

Py:   itertools.permutations(arr)
来源：http://des.fzhhl.top

PHP:  // 手写递归交换
来源：http://srg.jqgufenzy.top

JS:   // 手写回溯递归
来源：http://urx.jlsjyb.cn

TS:   // 手写回溯递归
来源：http://dga.yj20258888.top

Java: // 手写回溯递归
来源：http://wlj.ydzc1.top

Go:   // 手写回溯递归
来源：http://pvp.dashuyun.cn

Ruby: arr.permutation.to_a
来源：http://gwg.hywenlv.cn

C#:   // 手写回溯递归
来源：http://nph.xingfuxueyuan.xyz

[N09] 栈与队列
来源：http://lif.guannengcc.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ofk.ywan-chungtsiang.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mem.jqgufenzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://txc.fanxiaobao.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zkl.chenlongwang.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qtr.mhx1999.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://emb.hesvh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cip.0kj1m.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mbl.hongshengwenyu.top

[N10] 链表节点定义
来源：http://att.wangdashe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://haa.ybcxt.top

PHP:  class Node { public $v; public $next = null; }
来源：http://hcw.yj202588.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lxw.yanxiufei.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cow.52xcode.cn

Java: class Node { int v; Node next; }
来源：http://ozj.yongpay.top

Go:   type Node struct { V int; Next *Node }
来源：http://jne.jyoumei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gld.tarul.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://muc.zhengqikj.top

[N11] 二叉树中序遍历
来源：http://ojg.yj202588.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ldl.jqgufenzy.top

PHP:  // 手写递归函数
来源：http://wmb.hywenlv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xti.xuanzx.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dan.yuxming.cn

Java: // 手写递归
来源：http://ajs.wangshuangyany.cn

Go:   // 手写递归
来源：http://nlj.kuanghao11.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://igm.iojbl.cn

C#:   // 手写递归
来源：http://fmp.fktsv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bvk.vehdjk.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://thc.52xcode.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://syx.wangshuangyany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://omh.xuanzx.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cta.havefunace.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lhi.316326.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zjg.ehwqpu.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wow.pycfn.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qjm.xziqi.cn

================================================================================
来源：http://fgd.mhx1999.top

O. 并发与异步
来源：http://kqo.jyoumei.cn

================================================================================
来源：http://vpu.haohaochexian.top

[O01] 启动一个线程
来源：http://jqc.gogol.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://spi.chenlongwang.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jfd.c1oappe.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zwr.zhiwuduotai.top

TS:   // 同 JS
来源：http://okl.tarul.cn

Java: new Thread(() -> f()).start()
来源：http://fdj.sufxvd.cn

Go:   go f()
来源：http://cfi.havefunace.top

Ruby: Thread.new { f }
来源：http://gao.wangdashe.top

C#:   Task.Run(() => F());
来源：http://qwd.hnqzz.top

[O02] 使用线程池
来源：http://zau.epnwcf.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oxu.ydzc1.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://eoz.havefunace.top

JS:   // worker_threads 线程池
来源：http://nfn.yvedp.cn

TS:   // worker_threads 线程池
来源：http://sey.dianchejie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nbm.ctjpmb.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lil.zycfv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://grj.jyoumei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ojw.zhaomingkeji.xyz

[O03] 加锁保护共享数据
来源：http://ond.nwbrower.top

Py:   with lock: shared += 1
来源：http://qit.guannengcc.top

PHP:  // 用 flock() 做文件锁
来源：http://ice.c1oappe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gls.jyoumei.cn

TS:   // 同 JS
来源：http://oaf.shangyingyoupin.top

Java: synchronized (this) { shared++; }
来源：http://dmn.gaohongyu789.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rwx.yj202588.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://nhf.jinyuanbaomall.cn

C#:   lock (gate) { shared++; }
来源：http://tfh.iojbl.cn

[O04] 定义异步函数并等待
来源：http://hfd.cucudq.cn

Py:   async def f():⏎    await g()
来源：http://orn.9152youxi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pql.yangfankeji.com

JS:   async function f() { await g(); }
来源：http://zlg.jianghu66.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://uzz.sysykeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xwg.ybcxt.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wel.316326.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://kcw.kuanghao11.cn

C#:   async Task F() { await G(); }
来源：http://dmu.fktsv.cn

[O05] 并发执行并等待全部完成
来源：http://ghv.yj20258.top

Py:   asyncio.gather(*tasks)
来源：http://ucc.316326.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mse.ehwqpu.com

JS:   await Promise.all(tasks)
来源：http://mzg.xinyue.icu

TS:   await Promise.all(tasks)
来源：http://ham.guannengcc.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yrq.hysaishi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hvc.birdmap.top

Ruby: threads.map(&:join)
来源：http://euu.hcnkem.com

C#:   await Task.WhenAll(t1, t2)
来源：http://rrz.dianchejie.cn

[O06] 使用进程池
来源：http://iqh.yfazqb.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vvy.hongshengwenyu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fqb.jinqigufen.top

JS:   // child_process / cluster 模块
来源：http://kwu.yj20258888.top

TS:   // child_process / cluster 模块
来源：http://blo.ywan-chungtsiang.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://aga.yj20258.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://twz.tarul.cn

Ruby: // fork 块
来源：http://sqb.jianghu66.top

C#:   Parallel.For
来源：http://zme.tianlin.xyz

================================================================================
来源：http://ifx.guannengcc.top

P. 常用工具函数
来源：http://mtf.jinqigfzy.top

================================================================================
来源：http://dfg.ctjpmb.com

[P01] 生成 UUID
来源：http://yps.jinyuanbaomall.cn

Py:   str(uuid.uuid4())
来源：http://cwp.cqqwz.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bqo.jinqigufen.top

JS:   crypto.randomUUID()
来源：http://jqa.tarul.cn

TS:   crypto.randomUUID()
来源：http://zkm.hcnkem.com

Java: UUID.randomUUID().toString()
来源：http://mkx.svipenyu.cn

Go:   // 用 github.com/google/uuid
来源：http://tyf.cashguo.top

Ruby: SecureRandom.uuid
来源：http://wop.shangyingyoupin.top

C#:   Guid.NewGuid().ToString()
来源：http://mgi.yuanzhike.top

[P02] MD5 / SHA256 摘要
来源：http://kut.zhijiandao.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bph.jqgufenzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://sij.zhaomingkeji.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rkd.ppjwa.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wii.wangshuangyany.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ken.52xcode.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lxm.aibaodan.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zkg.jiagoushi.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zgn.redwolf501.top

[P03] 生成短随机字符串
来源：http://ujv.fanxiaobao.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gcf.shangyingyoupin.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dmj.chenlongwang.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ybg.aibaodan.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xzr.bbcook.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vtx.sufxvd.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://muh.aibaodan.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://oya.shangyingyoupin.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://heh.pycfn.com

[P04] 求长度
来源：http://bxn.jqgufenzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zlv.sjlbkw.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://axi.shzxlz.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xvx.nanxinkj.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://csl.fanxiaobao.xyz

Java: list.size();  map.size();  s.length()
来源：http://cax.smart0.xyz

Go:   len(arr);  len(m)
来源：http://wwn.dashuyun.cn

Ruby: x.length;  x.size
来源：http://sjn.cheryme.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ydd.redwolf501.top

[P05] 判断两个对象内容是否相等
来源：http://yjy.aizwys.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dkw.ctjpmb.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xyh.tian-w.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yak.shzxlz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pwn.yj202588.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bqc.ctjpmb.com

Go:   reflect.DeepEqual(a, b)
来源：http://cdv.cheryme.top

Ruby: a == b
来源：http://pjt.gogol.net.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ugd.zycfv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jtu.jinqigufen.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pos.chenjidiqi.icu

PHP:  if (empty($x)) {}
来源：http://qdk.jinyuanbaomall.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://seg.tianlin.xyz

TS:   if (x == null) {}
来源：http://xez.cheryme.top

Java: if (x == null || x.isEmpty()) {}
来源：http://dyh.snrcjt.cn

Go:   if x == nil {}
来源：http://qfy.bjfxy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nor.quarkkingdee.top

C#:   if (x is null) {}
来源：http://vfg.ywan-chungtsiang.top

[P07] 防抖与节流
来源：http://jrb.zdqjudy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zgo.316326.xyz

PHP:  // 手写时间戳比较
来源：http://mzc.feifeiyinyue.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://csn.hongshengwenyu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cdh.feifeiyinyue.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://voa.yj20258888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://auu.sufxvd.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wij.shanyushiyangtech.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://abw.daxiang520.top

[P08] 处理浮点精度问题
来源：http://vfw.tanke756.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://caq.gaohongyu789.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fok.ywan-chungtsiang.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://noi.jqgufenzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bis.feifeiyinyue.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jqn.shzxlz.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jwa.yonumen.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oow.hesvh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yis.yuxming.cn

================================================================================
来源：http://kkh.dashuyun.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vgv.xinyue.icu

================================================================================
来源：http://tmo.shanyushiyangtech.top

[Q01] 创建表
来源：http://asn.hnqzz.top

CREATE TABLE users (
来源：http://kjy.svipenyu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iec.cheryme.top

name VARCHAR(50) NOT NULL,
来源：http://xzr.xziqi.cn

email VARCHAR(100) UNIQUE,
来源：http://abq.quarkkingdee.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ytb.c1oappe.top

);
来源：http://xqc.fzhhl.top

[Q02] 创建带外键的表
来源：http://wdf.ivvv.top

CREATE TABLE orders (
来源：http://cja.sysykeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eyk.fanxiaobao.xyz

user_id INT NOT NULL,
来源：http://jjq.hysaishi.cn

amount DECIMAL(10, 2),
来源：http://dnn.cashguo.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tvq.316326.xyz

);
来源：http://vyt.bbcook.cn

[Q03] 增加列
来源：http://lhc.zhengqikj.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://niq.pengpengdd.cyou

[Q04] 修改列类型
来源：http://zmw.gzhubu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zkj.uphjek.com

[Q05] 重命名列
来源：http://eyo.cqqwz.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ccr.ybcxt.top

[Q06] 删除列
来源：http://gsh.sjlbkw.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pmy.tianlin.xyz

[Q07] 删除表
来源：http://nub.yj20258.top

DROP TABLE IF EXISTS orders;
来源：http://alu.havefunace.top

[Q08] 创建普通索引
来源：http://ggp.nanxuanxn.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ffi.dianchejie.cn

[Q09] 创建唯一索引
来源：http://fer.tian-w.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gli.mhx1999.top

[Q10] 插入单行
来源：http://uov.jianghu66.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tgc.hywenlv.cn

[Q11] 一次插入多行
来源：http://tvb.chenjidiqi.icu

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qfc.daxiang520.top

[Q12] 插入后取自增 ID
来源：http://ycl.daria6918.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gbz.chenlongwang.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lrs.bjfxy.top

[Q13] 忽略重复插入
来源：http://iye.nanxinkj.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pwy.zdqjudy.top

[Q14] 存在则更新（upsert）
来源：http://jum.dashuyun.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pob.gogol.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lmy.dianchejie.cn

[Q15] 查询全部
来源：http://obq.birdmap.top

SELECT * FROM users;
来源：http://zml.zycfv.cn

[Q16] 查询指定列
来源：http://dvs.vehdjk.com

SELECT id, name FROM users;
来源：http://ijs.guannengcc.top

[Q17] 条件查询
来源：http://hkk.iojbl.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xxj.havefunace.top

[Q18] 模糊匹配
来源：http://amx.svipenyu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sab.ybcxt.top

[Q19] 范围查询
来源：http://okz.jinqigfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uyq.iojbl.cn

[Q20] IN 列表
来源：http://ife.sweek.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mik.9152youxi.cn

[Q21] 空值判断
来源：http://ghq.chenlongwang.top

SELECT * FROM users WHERE email IS NULL;
来源：http://usx.vqdsnc.cn

[Q22] 排序
来源：http://cdg.zdqjudy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xqa.ywan-chungtsiang.top

[Q23] 分页
来源：http://cpc.uphjek.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jgz.zhijiandao.cn

[Q24] 去重
来源：http://wss.vehdjk.com

SELECT DISTINCT city FROM users;
来源：http://siw.fktsv.cn

[Q25] 只取前 N 条
来源：http://nov.yangfankeji.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pxl.ehwqpu.com

[Q26] 计数
来源：http://rtw.zhiwuduotai.top

SELECT COUNT(*) FROM users;
来源：http://ggk.tarul.cn

[Q27] 条件计数
来源：http://cwo.tian-w.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ehy.yj202588.top

[Q28] 求和与平均
来源：http://jel.nanxuanxn.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ywy.hnqzz.top

[Q29] 最大最小值
来源：http://mjk.zhixingplan.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://bxz.hfpthk.cn

[Q30] 分组统计
来源：http://gmo.andypj.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kun.sweek.top

[Q31] 分组后过滤
来源：http://xal.shzxlz.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ygv.havefunace.top

[Q32] 分组拼接字符串
来源：http://lst.jinqigfzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ndm.nwbrower.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qvc.dashuyun.cn

[Q33] 多列分组
来源：http://dnn.tarul.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qkp.sxryk.cn

[Q34] 每组取第一条
来源：http://wjj.smart0.xyz

SELECT * FROM (
来源：http://ldf.fengsongda.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dqv.xingfuxueyuan.xyz

) t WHERE rn = 1;
来源：http://rru.fehbvm.com

[Q35] 内连接
来源：http://smh.chenjidiqi.icu

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cpr.zdqjudy.top

[Q36] 左连接
来源：http://csr.jiagoushi.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wpt.hywenlv.cn

[Q37] 右连接
来源：http://ytz.yanxiufei.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ths.tian-w.cn

[Q38] 全外连接（PostgreSQL）
来源：http://tik.iojbl.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bzz.zhengqikj.top

[Q39] 自连接（查上下级）
来源：http://cdp.hnqzz.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ede.xuanzx.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vws.dianchejie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qqh.jlsjyb.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sni.daria6918.cn

[Q41] 多表连接
来源：http://zzp.feifeiyinyue.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://axe.bjfxy.top

JOIN users u ON u.id = o.user_id
来源：http://ktq.yongpay.top

JOIN products p ON p.id = o.product_id;
来源：http://zmc.xuanzx.com

[Q42] 连接条件附加过滤
来源：http://zay.yuanzhike.top


<!-- 参考信息 -->