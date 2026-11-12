代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://ltg.vehdjk.com

TS:   s === [...s].reverse().join("")
来源：http://fpq.zhiwuduotai.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kcu.tianlin.xyz

Go:   // 双指针从两端比较
来源：http://fwb.wangdashe.top

Ruby: s == s.reverse
来源：http://urf.fktsv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nky.dianchejie.cn

[N07] 两数之和（返回下标）
来源：http://qhp.shanyushiyangtech.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pkk.aizwys.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://irw.gzhubu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://bpo.hnqzz.top

TS:   // 手写 Map<string, number>
来源：http://wik.tian-w.cn

Java: // 手写 HashMap
来源：http://ukc.52xcode.cn

Go:   // 手写 map[int]int
来源：http://nxp.dianchejie.cn

Ruby: // 手写 Hash
来源：http://wfo.yuxming.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jvh.shanyushiyangtech.top

[N08] 生成全排列
来源：http://myy.vqdsnc.cn

Py:   itertools.permutations(arr)
来源：http://ofk.jqgfzy.top

PHP:  // 手写递归交换
来源：http://xvj.yonumen.top

JS:   // 手写回溯递归
来源：http://qsx.shzxlz.cn

TS:   // 手写回溯递归
来源：http://bkd.yvedp.cn

Java: // 手写回溯递归
来源：http://vpj.gzhubu.top

Go:   // 手写回溯递归
来源：http://qqc.jlsjyb.cn

Ruby: arr.permutation.to_a
来源：http://mje.gotoacloud.top

C#:   // 手写回溯递归
来源：http://qxk.ydjk.org.cn

[N09] 栈与队列
来源：http://rzk.hammf.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vac.cqqwz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gys.zhongyouzk.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yis.yangfankeji.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blb.bbcook.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hpx.jinqigfzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rek.epnwcf.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xdf.quarkkingdee.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rxx.shanyushiyangtech.top

[N10] 链表节点定义
来源：http://dhq.jyoumei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cvg.xingfuxueyuan.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://emv.andypj.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ent.xinyue.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://atf.52xcode.cn

Java: class Node { int v; Node next; }
来源：http://xpu.sxryk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pna.tarul.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pdq.haohaochexian.top

C#:   class Node { public int V; public Node? Next; }
来源：http://evh.gaohongyu789.top

[N11] 二叉树中序遍历
来源：http://hfn.shanyushiyangkeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://knv.vqdsnc.cn

PHP:  // 手写递归函数
来源：http://hlt.cqqwz.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pli.hfpthk.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ggz.pengpengdd.cyou

Java: // 手写递归
来源：http://ovd.hammf.cn

Go:   // 手写递归
来源：http://emb.ywan-chungtsiang.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cei.yueranfly.top

C#:   // 手写递归
来源：http://vbo.mhx1999.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bnu.iojbl.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cwt.ywan-chungtsiang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://syi.andypj.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ssm.andypj.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rgr.shanyushiyangtech.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vuu.yuanzhike.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://spq.hnxiangtu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dzg.aibaodan.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://itf.cdnleiting.top

================================================================================
来源：http://drv.redwolf501.top

O. 并发与异步
来源：http://loq.meibo888.top

================================================================================
来源：http://puy.xinyue.icu

[O01] 启动一个线程
来源：http://zrq.hysaishi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ecp.nanxuanxn.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zfy.yj20258888.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jcp.sweek.top

TS:   // 同 JS
来源：http://wva.yongpay.top

Java: new Thread(() -> f()).start()
来源：http://bml.aibaodan.cn

Go:   go f()
来源：http://xsz.yangfankeji.com

Ruby: Thread.new { f }
来源：http://hdp.jyoumei.cn

C#:   Task.Run(() => F());
来源：http://zvv.bjfxy.top

[O02] 使用线程池
来源：http://qii.hywenlv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gdi.xylfe.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ait.jinyuanbaomall.cn

JS:   // worker_threads 线程池
来源：http://kew.yanxiufei.cn

TS:   // worker_threads 线程池
来源：http://vrb.yvedp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ihd.mhx1999.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xch.haohaochexian.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hee.svipenyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xlb.iojbl.cn

[O03] 加锁保护共享数据
来源：http://ike.jinghuilouyu.cn

Py:   with lock: shared += 1
来源：http://fyo.jqgufenzy.top

PHP:  // 用 flock() 做文件锁
来源：http://sma.xylfe.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pyq.shuidangran.top

TS:   // 同 JS
来源：http://gjz.zhiwuduotai.top

Java: synchronized (this) { shared++; }
来源：http://kdh.zdbjq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://muh.yfazqb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://avg.hfpthk.cn

C#:   lock (gate) { shared++; }
来源：http://yqk.fengsongda.top

[O04] 定义异步函数并等待
来源：http://inm.dianchejie.cn

Py:   async def f():⏎    await g()
来源：http://cbb.yuanzhike.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://iti.zhoulong.xyz

JS:   async function f() { await g(); }
来源：http://nyt.feifeiyinyue.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://zbc.xingfuxueyuan.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mxg.dianchejie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://reg.gzhubu.top

Ruby: # 用 Fiber 或 async gem
来源：http://fes.sysykeji.top

C#:   async Task F() { await G(); }
来源：http://nqg.fzhhl.top

[O05] 并发执行并等待全部完成
来源：http://zux.yj20258.top

Py:   asyncio.gather(*tasks)
来源：http://vpt.hnqzz.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mse.c1oappe.top

JS:   await Promise.all(tasks)
来源：http://viq.guannengcc.top

TS:   await Promise.all(tasks)
来源：http://wcs.xuetiantiany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ivd.tarul.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uwn.redwolf501.top

Ruby: threads.map(&:join)
来源：http://wns.yj202588.top

C#:   await Task.WhenAll(t1, t2)
来源：http://hlw.xuanzx.com

[O06] 使用进程池
来源：http://qhu.xylfe.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rmu.sufxvd.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ofr.cashguo.top

JS:   // child_process / cluster 模块
来源：http://icx.dianchejie.cn

TS:   // child_process / cluster 模块
来源：http://kmt.pengpengdd.cyou

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vmd.birdmap.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vth.ivvv.top

Ruby: // fork 块
来源：http://wuv.hammf.cn

C#:   Parallel.For
来源：http://fta.nanxuanxn.top

================================================================================
来源：http://esh.pycfn.com

P. 常用工具函数
来源：http://cgk.jiagoushi.top

================================================================================
来源：http://nei.zdbjq.cn

[P01] 生成 UUID
来源：http://bxu.iojbl.cn

Py:   str(uuid.uuid4())
来源：http://qhb.ppjwa.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hky.jianghu66.top

JS:   crypto.randomUUID()
来源：http://xpx.kuanghao11.cn

TS:   crypto.randomUUID()
来源：http://loo.fzhhl.top

Java: UUID.randomUUID().toString()
来源：http://kjy.tarul.cn

Go:   // 用 github.com/google/uuid
来源：http://utw.guowangkeji.top

Ruby: SecureRandom.uuid
来源：http://dqt.shanyushiyangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://sxs.jlsjyb.cn

[P02] MD5 / SHA256 摘要
来源：http://ovu.kuanghao11.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://saj.jinqigfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://urw.yueranfly.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://azi.zhengqikj.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://maz.hywenlv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jym.wangdashe.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://acv.zdqjudy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bqp.sweek.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mti.shzxlz.cn

[P03] 生成短随机字符串
来源：http://ocp.yfazqb.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wre.zhaomingkeji.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zrs.yuanzhike.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xwa.fanxiaobao.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://otm.c1oappe.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://flj.shanyushiyangkeji.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mun.yj20258.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://lmm.nanxuanxn.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pbm.epnwcf.com

[P04] 求长度
来源：http://scm.hnxiangtu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bfg.fzhhl.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vam.wangshuangyany.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tmz.guannengcc.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hlk.ywan-chungtsiang.top

Java: list.size();  map.size();  s.length()
来源：http://ood.sjlbkw.cn

Go:   len(arr);  len(m)
来源：http://hem.guannengcc.top

Ruby: x.length;  x.size
来源：http://edr.52xcode.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://evt.tarul.cn

[P05] 判断两个对象内容是否相等
来源：http://cmf.chenlongwang.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://nhv.guowangkeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nrb.daria6918.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lae.mhx1999.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hka.kuanghao11.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ioo.aizwys.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hbt.tianlin.xyz

Ruby: a == b
来源：http://lyn.fzhhl.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://efi.tanke756.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vae.hongshengwenyu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ano.nanxinkj.top

PHP:  if (empty($x)) {}
来源：http://wrb.dianchejie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://awi.yanxiufei.cn

TS:   if (x == null) {}
来源：http://zfj.guannengcc.top

Java: if (x == null || x.isEmpty()) {}
来源：http://tiy.xuanzx.com

Go:   if x == nil {}
来源：http://obc.shzxlz.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wqw.hywenlv.cn

C#:   if (x is null) {}
来源：http://mde.hfpthk.cn

[P07] 防抖与节流
来源：http://rzh.cheryme.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hqn.snrcjt.cn

PHP:  // 手写时间戳比较
来源：http://irk.sweek.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://crg.svipenyu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://edg.hesvh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://geg.aizwys.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kxe.jinyuanbaomall.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wqg.hysaishi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qxp.ivvv.top

[P08] 处理浮点精度问题
来源：http://bhg.zhixingplan.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mxx.cqqwz.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://abr.jyoumei.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fzb.dianchejie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://atm.hywenlv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://aao.jinqigfzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mxl.haohaochexian.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fmx.fanxiaobao.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yjb.aibaodan.cn

================================================================================
来源：http://zqc.daria6918.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://agz.sysykeji.top

================================================================================
来源：http://lyi.chenzaomai.com

[Q01] 创建表
来源：http://lnh.quarkkingdee.top

CREATE TABLE users (
来源：http://tso.snrcjt.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://efl.ydjk.org.cn

name VARCHAR(50) NOT NULL,
来源：http://fyh.yj20258888.top

email VARCHAR(100) UNIQUE,
来源：http://imd.pycfn.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://njl.fanxiaobao.xyz

);
来源：http://iye.yanxiufei.cn

[Q02] 创建带外键的表
来源：http://jzs.tanke756.top

CREATE TABLE orders (
来源：http://aaa.cashguo.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bgo.tian-w.cn

user_id INT NOT NULL,
来源：http://wor.yueranfly.top

amount DECIMAL(10, 2),
来源：http://doz.hfpthk.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fav.jiagoushi.top

);
来源：http://yny.sjlbkw.cn

[Q03] 增加列
来源：http://zkw.tian-w.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xqm.gogol.net.cn

[Q04] 修改列类型
来源：http://lxn.dashuyun.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://adz.feifeiyinyue.top

[Q05] 重命名列
来源：http://pwf.tanke756.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kjc.sxryk.cn

[Q06] 删除列
来源：http://ibi.jlsjyb.cn

ALTER TABLE users DROP COLUMN age;
来源：http://tne.ivvv.top

[Q07] 删除表
来源：http://dov.ybcxt.top

DROP TABLE IF EXISTS orders;
来源：http://osm.quarkkingdee.top

[Q08] 创建普通索引
来源：http://tyq.birdmap.top

CREATE INDEX idx_users_email ON users(email);
来源：http://uch.jqgfzy.top

[Q09] 创建唯一索引
来源：http://frp.zdbjq.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ufx.shuidangran.top

[Q10] 插入单行
来源：http://xlv.xziqi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gqe.iojbl.cn

[Q11] 一次插入多行
来源：http://mrp.dashuyun.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://koo.fanxiaobao.xyz

[Q12] 插入后取自增 ID
来源：http://wyr.fehbvm.com

INSERT INTO users (name) VALUES ('C');
来源：http://bda.dashuyun.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pcd.ctjpmb.com

[Q13] 忽略重复插入
来源：http://uje.tianlin.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://coi.zhengqikj.top

[Q14] 存在则更新（upsert）
来源：http://oie.chenzaomai.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uzb.hongshengwenyu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dye.birdmap.top

[Q15] 查询全部
来源：http://rir.yangfankeji.com

SELECT * FROM users;
来源：http://jog.zhixingplan.top

[Q16] 查询指定列
来源：http://wdq.jinqigfzy.top

SELECT id, name FROM users;
来源：http://mrp.fktsv.cn

[Q17] 条件查询
来源：http://btt.hcnkem.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nic.ybcxt.top

[Q18] 模糊匹配
来源：http://flb.jyoumei.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://eye.cdnleiting.top

[Q19] 范围查询
来源：http://zct.xziqi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fwl.jlsjyb.cn

[Q20] IN 列表
来源：http://ikf.hesvh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bsp.hongshengwenyu.top

[Q21] 空值判断
来源：http://clv.shzxlz.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kcu.yvedp.cn

[Q22] 排序
来源：http://qpa.zhijiandao.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ine.yangfankeji.com

[Q23] 分页
来源：http://apj.sjlbkw.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tuy.hcnkem.com

[Q24] 去重
来源：http://kgk.fehbvm.com

SELECT DISTINCT city FROM users;
来源：http://njm.tian-w.cn

[Q25] 只取前 N 条
来源：http://eie.ydzc1.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bwf.tanke756.top

[Q26] 计数
来源：http://uza.meibo888.top

SELECT COUNT(*) FROM users;
来源：http://htw.zdbjq.cn

[Q27] 条件计数
来源：http://cyk.smart0.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xct.jianghu66.top

[Q28] 求和与平均
来源：http://oig.feifeiyinyue.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nnx.shanyushiyangtech.top

[Q29] 最大最小值
来源：http://arw.jinqigufen.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jog.zhixingplan.top

[Q30] 分组统计
来源：http://rrr.jinyuanbaomall.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ztq.shzxlz.cn

[Q31] 分组后过滤
来源：http://ryv.jqgufenzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cig.zhongyouzk.top

[Q32] 分组拼接字符串
来源：http://ihb.yuanzhike.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://upj.cqqwz.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kfq.hnqzz.top

[Q33] 多列分组
来源：http://qah.fktsv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mbi.xuanzx.com

[Q34] 每组取第一条
来源：http://xxt.hesvh.cn

SELECT * FROM (
来源：http://cnl.sjlbkw.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rqo.ydzc1.top

) t WHERE rn = 1;
来源：http://zjq.jinghuilouyu.cn

[Q35] 内连接
来源：http://rjn.jiagoushi.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cjc.bjfxy.top

[Q36] 左连接
来源：http://xpq.zhixingplan.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ivi.jlsjyb.cn

[Q37] 右连接
来源：http://byx.tarul.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ufz.fengsongda.top

[Q38] 全外连接（PostgreSQL）
来源：http://orw.xinyue.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pne.sweek.top

[Q39] 自连接（查上下级）
来源：http://ubo.xuanzx.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://mkw.yuanzhike.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://icc.sysykeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://wtb.aizwys.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sqs.yuxming.cn

[Q41] 多表连接
来源：http://ypn.xuanzx.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://axg.quarkkingdee.top

JOIN users u ON u.id = o.user_id
来源：http://wpo.shuidangran.top

JOIN products p ON p.id = o.product_id;
来源：http://dft.tanke756.top

[Q42] 连接条件附加过滤
来源：http://bxu.jqgufenzy.top

SELECT u.name, o.amount FROM users u
来源：http://krf.fehbvm.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bcy.sufxvd.cn

[Q43] 标量子查询
来源：http://mhg.hammf.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rvd.zycfv.cn


<!-- 参考信息 -->