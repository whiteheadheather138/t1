代发 wailian999

Go:   // 手写 map[int]int
来源：http://pdv.bbcook.cn

Ruby: // 手写 Hash
来源：http://xtz.cashguo.top

C#:   // 手写 Dictionary<int, int>
来源：http://don.sweek.top

[N08] 生成全排列
来源：http://htd.ydjk.org.cn

Py:   itertools.permutations(arr)
来源：http://tpr.chenlongwang.top

PHP:  // 手写递归交换
来源：http://kfe.uphjek.com

JS:   // 手写回溯递归
来源：http://pao.hammf.cn

TS:   // 手写回溯递归
来源：http://bwb.xuetiantiany.cn

Java: // 手写回溯递归
来源：http://egf.chenzaomai.com

Go:   // 手写回溯递归
来源：http://dku.fanxiaobao.xyz

Ruby: arr.permutation.to_a
来源：http://dwp.yj202588.top

C#:   // 手写回溯递归
来源：http://qcj.jinghuilouyu.cn

[N09] 栈与队列
来源：http://onk.dianchejie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jsd.yj20258888.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mgt.gogol.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://den.gogol.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://eps.316326.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mwu.xuanzx.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ztr.gaohongyu789.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vqb.chenjidiqi.icu

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ict.yvedp.cn

[N10] 链表节点定义
来源：http://lsc.sufxvd.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://huy.nanxuanxn.top

PHP:  class Node { public $v; public $next = null; }
来源：http://pse.hesvh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xzt.smart0.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kjd.aizwys.cn

Java: class Node { int v; Node next; }
来源：http://zbw.pengpengdd.cyou

Go:   type Node struct { V int; Next *Node }
来源：http://evz.guowangkeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wpe.yj20258.top

C#:   class Node { public int V; public Node? Next; }
来源：http://gbd.ydzc1.top

[N11] 二叉树中序遍历
来源：http://awr.jiagoushi.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wga.yj20258.top

PHP:  // 手写递归函数
来源：http://ezb.9152youxi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sgn.gzhubu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xux.xuetiantiany.cn

Java: // 手写递归
来源：http://fdt.cucudq.cn

Go:   // 手写递归
来源：http://ytm.xylfe.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mtf.yfazqb.com

C#:   // 手写递归
来源：http://qvp.zhixingplan.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lkv.snrcjt.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jil.snrcjt.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xrv.jinyuanbaomall.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kez.dianchejie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ycj.zhaomingkeji.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ihm.ehwqpu.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fnr.pycfn.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iep.cdnleiting.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wlw.shanyushiyangtech.top

================================================================================
来源：http://gjg.dashuyun.cn

O. 并发与异步
来源：http://vjh.ydzc1.top

================================================================================
来源：http://grg.jinghuilouyu.cn

[O01] 启动一个线程
来源：http://ydk.ctjpmb.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bzy.tian-w.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qlk.zdbjq.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fah.gotoacloud.top

TS:   // 同 JS
来源：http://vpb.ydjk.org.cn

Java: new Thread(() -> f()).start()
来源：http://jqb.yonumen.top

Go:   go f()
来源：http://hbu.9152youxi.cn

Ruby: Thread.new { f }
来源：http://cxp.hnxiangtu.top

C#:   Task.Run(() => F());
来源：http://mid.shzxlz.cn

[O02] 使用线程池
来源：http://etf.guowangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bha.havefunace.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://avj.tianlin.xyz

JS:   // worker_threads 线程池
来源：http://onj.andypj.xyz

TS:   // worker_threads 线程池
来源：http://xtp.jinyuanbaomall.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zhb.zhoulong.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://azw.meibo888.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qdb.shangyingyoupin.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://otb.tianlin.xyz

[O03] 加锁保护共享数据
来源：http://lxs.cashguo.top

Py:   with lock: shared += 1
来源：http://efi.hammf.cn

PHP:  // 用 flock() 做文件锁
来源：http://ezk.cqqwz.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://abr.jlsjyb.cn

TS:   // 同 JS
来源：http://fpo.hammf.cn

Java: synchronized (this) { shared++; }
来源：http://zmc.hywenlv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rco.jinqigufen.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://gke.iojbl.cn

C#:   lock (gate) { shared++; }
来源：http://nky.yueranfly.top

[O04] 定义异步函数并等待
来源：http://mlm.hcnkem.com

Py:   async def f():⏎    await g()
来源：http://lnb.ydjk.org.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://avb.ctjpmb.com

JS:   async function f() { await g(); }
来源：http://wxt.smart0.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://vtt.xylfe.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bvw.shangyingyoupin.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zuy.svipenyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gby.yanxiufei.cn

C#:   async Task F() { await G(); }
来源：http://vjc.zhaomingkeji.xyz

[O05] 并发执行并等待全部完成
来源：http://rts.shzxlz.cn

Py:   asyncio.gather(*tasks)
来源：http://yju.yanxiufei.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lci.yj20258888.top

JS:   await Promise.all(tasks)
来源：http://ajx.shanyushiyangkeji.top

TS:   await Promise.all(tasks)
来源：http://rjs.smart0.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xqk.yueranfly.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zrx.yanxiufei.cn

Ruby: threads.map(&:join)
来源：http://omm.epnwcf.com

C#:   await Task.WhenAll(t1, t2)
来源：http://gfl.snrcjt.cn

[O06] 使用进程池
来源：http://fxf.0kj1m.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ucb.yuanzhike.top

PHP:  // pcntl_fork 或多进程队列
来源：http://kzu.yonumen.top

JS:   // child_process / cluster 模块
来源：http://wgt.sweek.top

TS:   // child_process / cluster 模块
来源：http://imi.yongpay.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pnj.sufxvd.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jtd.cheryme.top

Ruby: // fork 块
来源：http://adh.kuanghao11.cn

C#:   Parallel.For
来源：http://xgh.52xcode.cn

================================================================================
来源：http://lsc.cqqwz.cn

P. 常用工具函数
来源：http://acl.hammf.cn

================================================================================
来源：http://otc.shangyingyoupin.top

[P01] 生成 UUID
来源：http://rxq.hfpthk.cn

Py:   str(uuid.uuid4())
来源：http://umg.yanxiufei.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wsx.haohaochexian.top

JS:   crypto.randomUUID()
来源：http://uao.sjlbkw.cn

TS:   crypto.randomUUID()
来源：http://xak.yuanzhike.top

Java: UUID.randomUUID().toString()
来源：http://zln.shzxlz.cn

Go:   // 用 github.com/google/uuid
来源：http://msu.jinyuanbaomall.cn

Ruby: SecureRandom.uuid
来源：http://aqv.shanyushiyangtech.top

C#:   Guid.NewGuid().ToString()
来源：http://vaz.hywenlv.cn

[P02] MD5 / SHA256 摘要
来源：http://xtx.hnxiangtu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nhv.nanxuanxn.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://vlj.fehbvm.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://eqa.zhengqikj.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tgd.hnqzz.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dyr.chenjidiqi.icu

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wly.yonumen.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://orv.cdnleiting.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hud.wangdashe.top

[P03] 生成短随机字符串
来源：http://srh.hesvh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ngo.gaohongyu789.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://eyc.nanxinkj.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rlq.hnqzz.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://flv.fehbvm.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ghv.sxryk.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pan.hnxiangtu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://bez.tianlin.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cjv.andypj.xyz

[P04] 求长度
来源：http://ldf.vehdjk.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://exe.0kj1m.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://etl.ydjk.org.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eiw.daria6918.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sgb.jianghu66.top

Java: list.size();  map.size();  s.length()
来源：http://lnm.daxiang520.top

Go:   len(arr);  len(m)
来源：http://wtv.bbcook.cn

Ruby: x.length;  x.size
来源：http://rhb.kuanghao11.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xcy.gzhubu.top

[P05] 判断两个对象内容是否相等
来源：http://yvq.yuanzhike.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ise.yanxiufei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cam.shanyushiyangkeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xjj.pycfn.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://anc.redwolf501.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://koe.havefunace.top

Go:   reflect.DeepEqual(a, b)
来源：http://dud.c1oappe.top

Ruby: a == b
来源：http://yod.zdqjudy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://slj.shanyushiyangkeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qmk.xingfuxueyuan.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tdz.fanxiaobao.xyz

PHP:  if (empty($x)) {}
来源：http://txc.tanke756.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yfx.yj20258.top

TS:   if (x == null) {}
来源：http://sve.sxryk.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nxt.shanyushiyangkeji.top

Go:   if x == nil {}
来源：http://dqh.shuidangran.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ltn.nwbrower.top

C#:   if (x is null) {}
来源：http://haz.xinyue.icu

[P07] 防抖与节流
来源：http://kwm.andypj.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ova.nanxuanxn.top

PHP:  // 手写时间戳比较
来源：http://kzq.xingfuxueyuan.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wxi.yj20258888.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uyy.yuxming.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lwj.dianchejie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bkq.jinghuilouyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nda.hfpthk.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://epi.jyoumei.cn

[P08] 处理浮点精度问题
来源：http://pkg.havefunace.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hhr.jianghu66.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bgh.shzxlz.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yxb.jqgufenzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ptt.andypj.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ile.vqdsnc.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ujn.kuanghao11.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ape.guowangkeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vbe.bbcook.cn

================================================================================
来源：http://gny.cashguo.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://igm.sxryk.cn

================================================================================
来源：http://ryd.zhaomingkeji.xyz

[Q01] 创建表
来源：http://vup.chenzaomai.com

CREATE TABLE users (
来源：http://miz.cucudq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vus.daria6918.cn

name VARCHAR(50) NOT NULL,
来源：http://cis.epnwcf.com

email VARCHAR(100) UNIQUE,
来源：http://cch.yuxming.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://efo.yongpay.top

);
来源：http://khs.shangyingyoupin.top

[Q02] 创建带外键的表
来源：http://gbr.gaohongyu789.top

CREATE TABLE orders (
来源：http://wzi.chenzaomai.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qll.iojbl.cn

user_id INT NOT NULL,
来源：http://abh.andypj.xyz

amount DECIMAL(10, 2),
来源：http://isi.hysaishi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bmv.jqgfzy.top

);
来源：http://lqc.jinyuanbaomall.cn

[Q03] 增加列
来源：http://xnd.jinqigfzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://onp.cucudq.cn

[Q04] 修改列类型
来源：http://vvs.chenjidiqi.icu

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ldk.ctjpmb.com

[Q05] 重命名列
来源：http://nub.hnxiangtu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://moo.jinyuanbaomall.cn

[Q06] 删除列
来源：http://hui.jiagoushi.top

ALTER TABLE users DROP COLUMN age;
来源：http://ibr.xuetiantiany.cn

[Q07] 删除表
来源：http://ltm.zhixingplan.top

DROP TABLE IF EXISTS orders;
来源：http://quo.bbcook.cn

[Q08] 创建普通索引
来源：http://ghe.yvedp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://knm.cqqwz.cn

[Q09] 创建唯一索引
来源：http://dip.cashguo.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fgz.yangfankeji.com

[Q10] 插入单行
来源：http://wky.sufxvd.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jwv.tarul.cn

[Q11] 一次插入多行
来源：http://ysy.tarul.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nnq.bjfxy.top

[Q12] 插入后取自增 ID
来源：http://gic.aizwys.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ywn.vehdjk.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blt.gotoacloud.top

[Q13] 忽略重复插入
来源：http://grn.hywenlv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bey.jqgfzy.top

[Q14] 存在则更新（upsert）
来源：http://wkv.jyoumei.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rtv.9152youxi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mpy.yuanzhike.top

[Q15] 查询全部
来源：http://zyy.haohaochexian.top

SELECT * FROM users;
来源：http://rsx.bjfxy.top

[Q16] 查询指定列
来源：http://fgj.jinghuilouyu.cn

SELECT id, name FROM users;
来源：http://icr.pengpengdd.cyou

[Q17] 条件查询
来源：http://dyp.jiagoushi.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://leb.fengsongda.top

[Q18] 模糊匹配
来源：http://egz.shangyingyoupin.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lyz.wangshuangyany.cn

[Q19] 范围查询
来源：http://ceg.zycfv.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qky.jqgfzy.top

[Q20] IN 列表
来源：http://czn.dianchejie.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ljs.ybcxt.top

[Q21] 空值判断
来源：http://tgu.zhiwuduotai.top

SELECT * FROM users WHERE email IS NULL;
来源：http://lrm.birdmap.top

[Q22] 排序
来源：http://khu.dashuyun.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://opv.chenjidiqi.icu

[Q23] 分页
来源：http://zts.zhixingplan.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://emq.redwolf501.top

[Q24] 去重
来源：http://ure.fehbvm.com

SELECT DISTINCT city FROM users;
来源：http://uua.hammf.cn

[Q25] 只取前 N 条
来源：http://gxk.smart0.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lev.hywenlv.cn

[Q26] 计数
来源：http://aqe.vqdsnc.cn

SELECT COUNT(*) FROM users;
来源：http://afo.cheryme.top

[Q27] 条件计数
来源：http://mlv.smart0.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://aio.zhiwuduotai.top

[Q28] 求和与平均
来源：http://iwr.fktsv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mzf.wangdashe.top

[Q29] 最大最小值
来源：http://fxi.andypj.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://wze.hammf.cn

[Q30] 分组统计
来源：http://fii.hywenlv.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ufc.cqqwz.cn

[Q31] 分组后过滤
来源：http://jpd.tarul.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vzv.daria6918.cn

[Q32] 分组拼接字符串
来源：http://qsi.jiagoushi.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mjy.jlsjyb.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wat.jianghu66.top

[Q33] 多列分组
来源：http://toh.sweek.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wje.zhoulong.xyz

[Q34] 每组取第一条
来源：http://kbj.gogol.net.cn

SELECT * FROM (
来源：http://buv.zdqjudy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sli.xingfuxueyuan.xyz

) t WHERE rn = 1;
来源：http://pli.ehwqpu.com

[Q35] 内连接
来源：http://dtx.shzxlz.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://btt.wangdashe.top

[Q36] 左连接
来源：http://mxi.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sut.0kj1m.cn

[Q37] 右连接
来源：http://aag.quarkkingdee.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pys.pycfn.com

[Q38] 全外连接（PostgreSQL）
来源：http://eua.fktsv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lal.zhengqikj.top

[Q39] 自连接（查上下级）
来源：http://gpx.svipenyu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jsg.xingfuxueyuan.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fla.gogol.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qyl.yonumen.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ehj.ctjpmb.com

[Q41] 多表连接
来源：http://xvd.ehwqpu.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://ajh.gzhubu.top

JOIN users u ON u.id = o.user_id
来源：http://fco.sjlbkw.cn

JOIN products p ON p.id = o.product_id;
来源：http://qjb.chenjidiqi.icu

[Q42] 连接条件附加过滤
来源：http://ujk.yj202588.top

SELECT u.name, o.amount FROM users u
来源：http://mbn.epnwcf.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bwo.c1oappe.top

[Q43] 标量子查询
来源：http://oih.yj20258888.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dsp.vqdsnc.cn

[Q44] IN 子查询
来源：http://jtu.ppjwa.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xvp.tanke756.top

[Q45] EXISTS 判断存在
来源：http://aad.sysykeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gev.cheryme.top

[Q46] NOT EXISTS 判断不存在
来源：http://hgs.fengsongda.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xqi.guannengcc.top

[Q47] 与平均值比较
来源：http://qby.0kj1m.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://peg.jqgufenzy.top

[Q48] CTE 公用表表达式
来源：http://iun.cucudq.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pqu.jianghu66.top

SELECT * FROM t WHERE c > 5;
来源：http://nwj.dashuyun.cn

[Q49] 更新单行
来源：http://nbo.jiagoushi.top


<!-- 参考信息 -->