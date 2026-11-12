代发 wailian999

Ruby: s == s.reverse
来源：http://dch.ydjk.org.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qxz.yj202588.top

[N07] 两数之和（返回下标）
来源：http://qch.tianlin.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wxo.zhiwuduotai.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ucb.hnxiangtu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://snz.xziqi.cn

TS:   // 手写 Map<string, number>
来源：http://eqj.hcnkem.com

Java: // 手写 HashMap
来源：http://asw.zhengqikj.top

Go:   // 手写 map[int]int
来源：http://pcd.xingfuxueyuan.xyz

Ruby: // 手写 Hash
来源：http://foq.tianlin.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://dex.jinghuilouyu.cn

[N08] 生成全排列
来源：http://akz.chenjidiqi.icu

Py:   itertools.permutations(arr)
来源：http://eyo.jinghuilouyu.cn

PHP:  // 手写递归交换
来源：http://rwa.zdbjq.cn

JS:   // 手写回溯递归
来源：http://etb.hnqzz.top

TS:   // 手写回溯递归
来源：http://nkh.gotoacloud.top

Java: // 手写回溯递归
来源：http://qbv.nanxinkj.top

Go:   // 手写回溯递归
来源：http://nxz.yvedp.cn

Ruby: arr.permutation.to_a
来源：http://rkg.smart0.xyz

C#:   // 手写回溯递归
来源：http://mnf.uphjek.com

[N09] 栈与队列
来源：http://dms.jqgfzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://iuf.shzxlz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tji.yonumen.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cvl.jinyuanbaomall.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://frs.zdbjq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ymu.xylfe.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xav.ybcxt.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pvx.zhixingplan.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://arf.xuanzx.com

[N10] 链表节点定义
来源：http://ood.cqqwz.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hsh.yuxming.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qrd.ctjpmb.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oai.iojbl.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://idl.aizwys.cn

Java: class Node { int v; Node next; }
来源：http://ias.jqgfzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://enu.meibo888.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mxz.cheryme.top

C#:   class Node { public int V; public Node? Next; }
来源：http://oye.feifeiyinyue.top

[N11] 二叉树中序遍历
来源：http://sfa.daria6918.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mog.dashuyun.cn

PHP:  // 手写递归函数
来源：http://fgo.jqgfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pqt.zdbjq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kha.52xcode.cn

Java: // 手写递归
来源：http://fzn.xinyue.icu

Go:   // 手写递归
来源：http://mcm.zhoulong.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ddz.zhijiandao.cn

C#:   // 手写递归
来源：http://rqg.hesvh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zoo.xinyue.icu

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tbd.hfpthk.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xzy.zhiwuduotai.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yfi.9152youxi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://soa.xuanzx.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hpu.jinqigufen.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ajv.hnxiangtu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jft.shuidangran.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ypw.cqqwz.cn

================================================================================
来源：http://brw.fktsv.cn

O. 并发与异步
来源：http://pcw.pengpengdd.cyou

================================================================================
来源：http://ssd.jinqigufen.top

[O01] 启动一个线程
来源：http://qvf.xuanzx.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cks.nwbrower.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xhl.fengsongda.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yte.wangshuangyany.cn

TS:   // 同 JS
来源：http://pda.jianghu66.top

Java: new Thread(() -> f()).start()
来源：http://gzg.jinghuilouyu.cn

Go:   go f()
来源：http://frc.nwbrower.top

Ruby: Thread.new { f }
来源：http://dlm.hongshengwenyu.top

C#:   Task.Run(() => F());
来源：http://vit.gaohongyu789.top

[O02] 使用线程池
来源：http://rnx.zhijiandao.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ufy.yj202588.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ahh.yangfankeji.com

JS:   // worker_threads 线程池
来源：http://awx.zhixingplan.top

TS:   // worker_threads 线程池
来源：http://kpu.zdqjudy.top

Java: Executors.newFixedThreadPool(4)
来源：http://ytc.52xcode.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://maz.0kj1m.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mpo.yongpay.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jji.yuxming.cn

[O03] 加锁保护共享数据
来源：http://bcs.xylfe.cn

Py:   with lock: shared += 1
来源：http://zjv.zhoulong.xyz

PHP:  // 用 flock() 做文件锁
来源：http://dky.9152youxi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tim.shanyushiyangtech.top

TS:   // 同 JS
来源：http://msp.mhx1999.top

Java: synchronized (this) { shared++; }
来源：http://avr.snrcjt.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sbg.shangyingyoupin.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://rgc.daxiang520.top

C#:   lock (gate) { shared++; }
来源：http://igb.fehbvm.com

[O04] 定义异步函数并等待
来源：http://kas.shanyushiyangkeji.top

Py:   async def f():⏎    await g()
来源：http://qio.guowangkeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pbn.jinqigufen.top

JS:   async function f() { await g(); }
来源：http://qmu.jianghu66.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://tyy.birdmap.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jjo.daria6918.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yhy.nanxuanxn.top

Ruby: # 用 Fiber 或 async gem
来源：http://kei.kuanghao11.cn

C#:   async Task F() { await G(); }
来源：http://uxw.c1oappe.top

[O05] 并发执行并等待全部完成
来源：http://gyg.shanyushiyangtech.top

Py:   asyncio.gather(*tasks)
来源：http://tgh.cdnleiting.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cmm.jianghu66.top

JS:   await Promise.all(tasks)
来源：http://uwj.yueranfly.top

TS:   await Promise.all(tasks)
来源：http://xfm.9152youxi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hqb.andypj.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ymm.xylfe.cn

Ruby: threads.map(&:join)
来源：http://xha.sysykeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xbh.hesvh.cn

[O06] 使用进程池
来源：http://ilb.andypj.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://css.yj20258888.top

PHP:  // pcntl_fork 或多进程队列
来源：http://nbf.shanyushiyangkeji.top

JS:   // child_process / cluster 模块
来源：http://iqp.fzhhl.top

TS:   // child_process / cluster 模块
来源：http://fjc.yuanzhike.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hmr.hnqzz.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eqv.hongshengwenyu.top

Ruby: // fork 块
来源：http://ree.hnqzz.top

C#:   Parallel.For
来源：http://yzl.hongshengwenyu.top

================================================================================
来源：http://dal.jinqigfzy.top

P. 常用工具函数
来源：http://vxf.quarkkingdee.top

================================================================================
来源：http://dxg.gaohongyu789.top

[P01] 生成 UUID
来源：http://xfh.wangshuangyany.cn

Py:   str(uuid.uuid4())
来源：http://iky.xinyue.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ecp.cqqwz.cn

JS:   crypto.randomUUID()
来源：http://wwo.tianlin.xyz

TS:   crypto.randomUUID()
来源：http://zee.yonumen.top

Java: UUID.randomUUID().toString()
来源：http://xzn.jlsjyb.cn

Go:   // 用 github.com/google/uuid
来源：http://wqi.cdnleiting.top

Ruby: SecureRandom.uuid
来源：http://skh.havefunace.top

C#:   Guid.NewGuid().ToString()
来源：http://sig.bjfxy.top

[P02] MD5 / SHA256 摘要
来源：http://csc.zdbjq.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qbl.shanyushiyangkeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://njo.yfazqb.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qle.cdnleiting.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qjb.pengpengdd.cyou

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hog.daxiang520.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://szg.quarkkingdee.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qzf.gogol.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xpo.zhengqikj.top

[P03] 生成短随机字符串
来源：http://ron.jyoumei.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mtl.andypj.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://aio.nwbrower.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rdj.feifeiyinyue.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cig.iojbl.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nhy.xuanzx.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kch.chenjidiqi.icu

Ruby: SecureRandom.alphanumeric(16)
来源：http://pzx.gaohongyu789.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wku.pengpengdd.cyou

[P04] 求长度
来源：http://kqo.ydjk.org.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://juj.hfpthk.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://esa.yangfankeji.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mjl.xuanzx.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nlf.jqgufenzy.top

Java: list.size();  map.size();  s.length()
来源：http://zvk.gzhubu.top

Go:   len(arr);  len(m)
来源：http://hsu.c1oappe.top

Ruby: x.length;  x.size
来源：http://grl.sweek.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://slf.dashuyun.cn

[P05] 判断两个对象内容是否相等
来源：http://dls.hesvh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ers.52xcode.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yia.sjlbkw.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kkn.haohaochexian.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lix.yj20258888.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wgd.xziqi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://nlc.ivvv.top

Ruby: a == b
来源：http://mal.9152youxi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jyv.guowangkeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ryw.52xcode.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://aeu.fktsv.cn

PHP:  if (empty($x)) {}
来源：http://uwy.dianchejie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bdv.ivvv.top

TS:   if (x == null) {}
来源：http://pdv.jiagoushi.top

Java: if (x == null || x.isEmpty()) {}
来源：http://cxd.yfazqb.com

Go:   if x == nil {}
来源：http://rte.yj202588.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ccn.52xcode.cn

C#:   if (x is null) {}
来源：http://xjl.hcnkem.com

[P07] 防抖与节流
来源：http://als.jinghuilouyu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mjd.quarkkingdee.top

PHP:  // 手写时间戳比较
来源：http://osr.c1oappe.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ybj.zhijiandao.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jqi.yj202588.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yoy.xinyue.icu

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blf.xylfe.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dkl.nwbrower.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qdy.daxiang520.top

[P08] 处理浮点精度问题
来源：http://nyi.jqgufenzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fmi.sysykeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sew.tianlin.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://skq.snrcjt.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cde.wangshuangyany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ohe.yanxiufei.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kys.zdbjq.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dfl.fengsongda.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ehy.redwolf501.top

================================================================================
来源：http://aod.chenlongwang.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xlx.hysaishi.cn

================================================================================
来源：http://fzu.hongshengwenyu.top

[Q01] 创建表
来源：http://yxz.chenjidiqi.icu

CREATE TABLE users (
来源：http://mvy.tanke756.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ijw.xinyue.icu

name VARCHAR(50) NOT NULL,
来源：http://hdw.redwolf501.top

email VARCHAR(100) UNIQUE,
来源：http://xzr.jinqigfzy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://anq.fktsv.cn

);
来源：http://vrh.jinghuilouyu.cn

[Q02] 创建带外键的表
来源：http://nyb.shzxlz.cn

CREATE TABLE orders (
来源：http://jkp.sysykeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hbc.52xcode.cn

user_id INT NOT NULL,
来源：http://tjy.fzhhl.top

amount DECIMAL(10, 2),
来源：http://bfd.hnqzz.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ccz.316326.xyz

);
来源：http://lbt.xziqi.cn

[Q03] 增加列
来源：http://hdo.ybcxt.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tdo.fanxiaobao.xyz

[Q04] 修改列类型
来源：http://vnv.yuxming.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zbx.jyoumei.cn

[Q05] 重命名列
来源：http://alh.jqgfzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lva.yvedp.cn

[Q06] 删除列
来源：http://dgo.hnqzz.top

ALTER TABLE users DROP COLUMN age;
来源：http://fru.haohaochexian.top

[Q07] 删除表
来源：http://otm.chenzaomai.com

DROP TABLE IF EXISTS orders;
来源：http://fui.yanxiufei.cn

[Q08] 创建普通索引
来源：http://ppe.shanyushiyangtech.top

CREATE INDEX idx_users_email ON users(email);
来源：http://bms.xingfuxueyuan.xyz

[Q09] 创建唯一索引
来源：http://uyl.jinghuilouyu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tgw.yfazqb.com

[Q10] 插入单行
来源：http://qln.hnxiangtu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pzb.kuanghao11.cn

[Q11] 一次插入多行
来源：http://dvw.yonumen.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gso.316326.xyz

[Q12] 插入后取自增 ID
来源：http://smo.jinghuilouyu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://zpz.zhaomingkeji.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fjn.zdqjudy.top

[Q13] 忽略重复插入
来源：http://bvx.316326.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jjg.yfazqb.com

[Q14] 存在则更新（upsert）
来源：http://uzx.sjlbkw.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://upd.dianchejie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://who.xinyue.icu

[Q15] 查询全部
来源：http://xso.xuanzx.com

SELECT * FROM users;
来源：http://iin.cheryme.top

[Q16] 查询指定列
来源：http://xcv.hnqzz.top

SELECT id, name FROM users;
来源：http://dri.hongshengwenyu.top

[Q17] 条件查询
来源：http://dal.meibo888.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wji.cdnleiting.top

[Q18] 模糊匹配
来源：http://dle.feifeiyinyue.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fno.jinyuanbaomall.cn

[Q19] 范围查询
来源：http://ncz.jqgfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mth.yongpay.top

[Q20] IN 列表
来源：http://pnw.snrcjt.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rnq.snrcjt.cn

[Q21] 空值判断
来源：http://xyx.tarul.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nep.wangshuangyany.cn

[Q22] 排序
来源：http://unh.gaohongyu789.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bcy.ppjwa.cn

[Q23] 分页
来源：http://xke.vehdjk.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vzx.bjfxy.top

[Q24] 去重
来源：http://ujq.vqdsnc.cn

SELECT DISTINCT city FROM users;
来源：http://rzj.316326.xyz

[Q25] 只取前 N 条
来源：http://mzn.xinyue.icu

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rhx.hcnkem.com

[Q26] 计数
来源：http://wwo.yfazqb.com

SELECT COUNT(*) FROM users;
来源：http://eay.zdqjudy.top

[Q27] 条件计数
来源：http://xpt.chenjidiqi.icu

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://daj.yuxming.cn

[Q28] 求和与平均
来源：http://xbe.sweek.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bfo.hysaishi.cn

[Q29] 最大最小值
来源：http://xmb.nwbrower.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://hdj.zhaomingkeji.xyz

[Q30] 分组统计
来源：http://rcw.zdbjq.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://igv.ppjwa.cn

[Q31] 分组后过滤
来源：http://mkf.zdqjudy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kal.aibaodan.cn

[Q32] 分组拼接字符串
来源：http://ngd.hnxiangtu.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yxs.yj20258888.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lcr.shanyushiyangtech.top

[Q33] 多列分组
来源：http://iva.ivvv.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dhw.uphjek.com

[Q34] 每组取第一条
来源：http://fxg.cqqwz.cn

SELECT * FROM (
来源：http://lqm.yanxiufei.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rsq.tian-w.cn

) t WHERE rn = 1;
来源：http://dww.pycfn.com

[Q35] 内连接
来源：http://kbl.ivvv.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tlf.52xcode.cn

[Q36] 左连接
来源：http://glc.jianghu66.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ckz.havefunace.top

[Q37] 右连接
来源：http://ezl.hammf.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ffl.jqgufenzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://dyi.shuidangran.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rae.ivvv.top

[Q39] 自连接（查上下级）
来源：http://wzg.meibo888.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://gae.fengsongda.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://uvw.yj202588.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xkr.fengsongda.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zjw.ivvv.top

[Q41] 多表连接
来源：http://abm.snrcjt.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cjj.birdmap.top

JOIN users u ON u.id = o.user_id
来源：http://sit.hnqzz.top

JOIN products p ON p.id = o.product_id;
来源：http://mrh.zycfv.cn

[Q42] 连接条件附加过滤
来源：http://evu.ydjk.org.cn

SELECT u.name, o.amount FROM users u
来源：http://ucm.zhixingplan.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lgn.zycfv.cn

[Q43] 标量子查询
来源：http://zpc.zdbjq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jsi.yanxiufei.cn

[Q44] IN 子查询
来源：http://gzc.gaohongyu789.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nzu.yj202588.top

[Q45] EXISTS 判断存在
来源：http://jph.ydjk.org.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://epv.yvedp.cn


<!-- 参考信息 -->