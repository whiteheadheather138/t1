代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gvb.cqqwz.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://iyb.xuetiantiany.cn

TS:   // 手写 Map<string, number>
来源：http://fof.vqdsnc.cn

Java: // 手写 HashMap
来源：http://yse.yangfankeji.com

Go:   // 手写 map[int]int
来源：http://rnj.haohaochexian.top

Ruby: // 手写 Hash
来源：http://cxg.jiagoushi.top

C#:   // 手写 Dictionary<int, int>
来源：http://wjt.quarkkingdee.top

[N08] 生成全排列
来源：http://izc.sysykeji.top

Py:   itertools.permutations(arr)
来源：http://zgi.zhongyouzk.top

PHP:  // 手写递归交换
来源：http://rhm.guowangkeji.top

JS:   // 手写回溯递归
来源：http://fzu.tarul.cn

TS:   // 手写回溯递归
来源：http://cyz.cucudq.cn

Java: // 手写回溯递归
来源：http://rxs.gotoacloud.top

Go:   // 手写回溯递归
来源：http://ryw.ehwqpu.com

Ruby: arr.permutation.to_a
来源：http://ooy.yvedp.cn

C#:   // 手写回溯递归
来源：http://iel.jinyuanbaomall.cn

[N09] 栈与队列
来源：http://zqo.jianghu66.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jqt.ybcxt.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dum.yongpay.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dbh.jlsjyb.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yey.nanxinkj.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://apt.zdbjq.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lbd.nwbrower.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ozd.sweek.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wup.shzxlz.cn

[N10] 链表节点定义
来源：http://wyo.hesvh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gxo.quarkkingdee.top

PHP:  class Node { public $v; public $next = null; }
来源：http://yuf.gotoacloud.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qge.guannengcc.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vrh.xingfuxueyuan.xyz

Java: class Node { int v; Node next; }
来源：http://ybx.gotoacloud.top

Go:   type Node struct { V int; Next *Node }
来源：http://onh.9152youxi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://znl.wangshuangyany.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://alv.aizwys.cn

[N11] 二叉树中序遍历
来源：http://ght.zhengqikj.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sxv.xuetiantiany.cn

PHP:  // 手写递归函数
来源：http://dmf.zhongyouzk.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://crp.iojbl.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://llx.shzxlz.cn

Java: // 手写递归
来源：http://gfo.bjfxy.top

Go:   // 手写递归
来源：http://trk.zdqjudy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://aim.gogol.net.cn

C#:   // 手写递归
来源：http://hck.jqgfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hxr.sufxvd.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://msb.zhongyouzk.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://skl.birdmap.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kfz.yangfankeji.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qrk.epnwcf.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bup.cqqwz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://oxt.hysaishi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qtj.dianchejie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://emt.vehdjk.com

================================================================================
来源：http://wll.zycfv.cn

O. 并发与异步
来源：http://xfv.yfazqb.com

================================================================================
来源：http://sbx.dianchejie.cn

[O01] 启动一个线程
来源：http://ouv.fengsongda.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ikb.ehwqpu.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dza.jyoumei.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jsx.uphjek.com

TS:   // 同 JS
来源：http://yvf.chenzaomai.com

Java: new Thread(() -> f()).start()
来源：http://mry.yueranfly.top

Go:   go f()
来源：http://zzg.hcnkem.com

Ruby: Thread.new { f }
来源：http://qlh.aibaodan.cn

C#:   Task.Run(() => F());
来源：http://ujl.yj202588.top

[O02] 使用线程池
来源：http://gnh.daxiang520.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xia.quarkkingdee.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xql.gotoacloud.top

JS:   // worker_threads 线程池
来源：http://ffy.jqgfzy.top

TS:   // worker_threads 线程池
来源：http://qbv.yanxiufei.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yfp.hysaishi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ody.gogol.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gkm.shuidangran.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vjr.aizwys.cn

[O03] 加锁保护共享数据
来源：http://xil.yj20258.top

Py:   with lock: shared += 1
来源：http://hzv.ybcxt.top

PHP:  // 用 flock() 做文件锁
来源：http://yqj.yangfankeji.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qmk.yj202588.top

TS:   // 同 JS
来源：http://rdg.redwolf501.top

Java: synchronized (this) { shared++; }
来源：http://hmi.zycfv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oxb.shzxlz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://roc.zhixingplan.top

C#:   lock (gate) { shared++; }
来源：http://hxg.aizwys.cn

[O04] 定义异步函数并等待
来源：http://lnr.cdnleiting.top

Py:   async def f():⏎    await g()
来源：http://gpb.jqgufenzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://doe.hongshengwenyu.top

JS:   async function f() { await g(); }
来源：http://yom.sjlbkw.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vau.nanxinkj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mkh.zycfv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fdr.fzhhl.top

Ruby: # 用 Fiber 或 async gem
来源：http://bpk.hcnkem.com

C#:   async Task F() { await G(); }
来源：http://bjw.jinyuanbaomall.cn

[O05] 并发执行并等待全部完成
来源：http://ccb.vqdsnc.cn

Py:   asyncio.gather(*tasks)
来源：http://ncf.jinghuilouyu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zbe.ivvv.top

JS:   await Promise.all(tasks)
来源：http://pct.bjfxy.top

TS:   await Promise.all(tasks)
来源：http://uod.jinyuanbaomall.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cma.yj20258888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://aud.shanyushiyangtech.top

Ruby: threads.map(&:join)
来源：http://yke.daria6918.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ipe.pengpengdd.cyou

[O06] 使用进程池
来源：http://xcv.andypj.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ybe.jiagoushi.top

PHP:  // pcntl_fork 或多进程队列
来源：http://voo.jqgfzy.top

JS:   // child_process / cluster 模块
来源：http://ltr.zhengqikj.top

TS:   // child_process / cluster 模块
来源：http://zaw.hcnkem.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qao.zhoulong.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tee.yueranfly.top

Ruby: // fork 块
来源：http://wzr.dashuyun.cn

C#:   Parallel.For
来源：http://kpu.c1oappe.top

================================================================================
来源：http://xqx.fanxiaobao.xyz

P. 常用工具函数
来源：http://qzg.quarkkingdee.top

================================================================================
来源：http://vse.wangshuangyany.cn

[P01] 生成 UUID
来源：http://gkq.yvedp.cn

Py:   str(uuid.uuid4())
来源：http://bkv.yj20258888.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mie.pengpengdd.cyou

JS:   crypto.randomUUID()
来源：http://ntm.nanxuanxn.top

TS:   crypto.randomUUID()
来源：http://rke.mhx1999.top

Java: UUID.randomUUID().toString()
来源：http://sdp.hnxiangtu.top

Go:   // 用 github.com/google/uuid
来源：http://svr.feifeiyinyue.top

Ruby: SecureRandom.uuid
来源：http://vgx.xuetiantiany.cn

C#:   Guid.NewGuid().ToString()
来源：http://hha.guowangkeji.top

[P02] MD5 / SHA256 摘要
来源：http://cit.hcnkem.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oqu.yuanzhike.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://vjn.jianghu66.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ujl.shzxlz.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vak.andypj.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pce.daxiang520.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vpo.wangdashe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sye.iojbl.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pxi.zhoulong.xyz

[P03] 生成短随机字符串
来源：http://svt.bjfxy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wlu.kuanghao11.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lkj.jianghu66.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://asz.cdnleiting.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://keh.cashguo.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dmq.gogol.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iec.fengsongda.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://tjz.0kj1m.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ptg.vehdjk.com

[P04] 求长度
来源：http://kao.aizwys.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://exb.yongpay.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zul.fengsongda.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eep.yj20258888.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dca.haohaochexian.top

Java: list.size();  map.size();  s.length()
来源：http://tqi.hcnkem.com

Go:   len(arr);  len(m)
来源：http://zwv.shzxlz.cn

Ruby: x.length;  x.size
来源：http://atf.guowangkeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://cgx.fengsongda.top

[P05] 判断两个对象内容是否相等
来源：http://cai.wangdashe.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://mlv.hysaishi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qbk.316326.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mmm.xylfe.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://aya.chenjidiqi.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jmx.iojbl.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tmu.meibo888.top

Ruby: a == b
来源：http://frp.wangshuangyany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://eys.guowangkeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rrs.zhaomingkeji.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://azg.pengpengdd.cyou

PHP:  if (empty($x)) {}
来源：http://dpj.shangyingyoupin.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://aua.xinyue.icu

TS:   if (x == null) {}
来源：http://igh.jianghu66.top

Java: if (x == null || x.isEmpty()) {}
来源：http://jzo.chenlongwang.top

Go:   if x == nil {}
来源：http://ght.zhiwuduotai.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kmv.wangdashe.top

C#:   if (x is null) {}
来源：http://vjo.aizwys.cn

[P07] 防抖与节流
来源：http://xve.xylfe.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://axs.guowangkeji.top

PHP:  // 手写时间戳比较
来源：http://gpn.shuidangran.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rbi.cucudq.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kpo.c1oappe.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dqw.hcnkem.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mxk.daxiang520.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://sqi.sjlbkw.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://idl.xziqi.cn

[P08] 处理浮点精度问题
来源：http://jos.haohaochexian.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rfa.zhongyouzk.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://utc.ywan-chungtsiang.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://oho.shzxlz.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ita.iojbl.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kww.316326.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wbt.cashguo.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gei.pengpengdd.cyou

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bwd.yonumen.top

================================================================================
来源：http://lwu.dianchejie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pho.smart0.xyz

================================================================================
来源：http://ouz.yfazqb.com

[Q01] 创建表
来源：http://utk.xuetiantiany.cn

CREATE TABLE users (
来源：http://tau.ywan-chungtsiang.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rap.ydjk.org.cn

name VARCHAR(50) NOT NULL,
来源：http://ixd.shanyushiyangtech.top

email VARCHAR(100) UNIQUE,
来源：http://cjx.yj20258888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vzx.daxiang520.top

);
来源：http://cyc.zhengqikj.top

[Q02] 创建带外键的表
来源：http://uac.0kj1m.cn

CREATE TABLE orders (
来源：http://ykg.hnqzz.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qxk.chenlongwang.top

user_id INT NOT NULL,
来源：http://oiu.tian-w.cn

amount DECIMAL(10, 2),
来源：http://lgk.bjfxy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://goq.fengsongda.top

);
来源：http://crf.xylfe.cn

[Q03] 增加列
来源：http://vbw.316326.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xze.vqdsnc.cn

[Q04] 修改列类型
来源：http://teg.haohaochexian.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://elr.xziqi.cn

[Q05] 重命名列
来源：http://ege.andypj.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gdp.redwolf501.top

[Q06] 删除列
来源：http://ubd.iojbl.cn

ALTER TABLE users DROP COLUMN age;
来源：http://peg.iojbl.cn

[Q07] 删除表
来源：http://ufe.shuidangran.top

DROP TABLE IF EXISTS orders;
来源：http://blp.daria6918.cn

[Q08] 创建普通索引
来源：http://xkx.fengsongda.top

CREATE INDEX idx_users_email ON users(email);
来源：http://mlo.chenjidiqi.icu

[Q09] 创建唯一索引
来源：http://ati.hammf.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://myj.jqgfzy.top

[Q10] 插入单行
来源：http://onn.aizwys.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wov.xziqi.cn

[Q11] 一次插入多行
来源：http://zwo.316326.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kjg.dashuyun.cn

[Q12] 插入后取自增 ID
来源：http://sha.yonumen.top

INSERT INTO users (name) VALUES ('C');
来源：http://wrm.ydzc1.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://iel.tanke756.top

[Q13] 忽略重复插入
来源：http://qhd.nanxinkj.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rqu.hammf.cn

[Q14] 存在则更新（upsert）
来源：http://eok.nanxinkj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dtc.hongshengwenyu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qqp.dashuyun.cn

[Q15] 查询全部
来源：http://oqe.zhijiandao.cn

SELECT * FROM users;
来源：http://gwf.gaohongyu789.top

[Q16] 查询指定列
来源：http://pzn.0kj1m.cn

SELECT id, name FROM users;
来源：http://bnm.jianghu66.top

[Q17] 条件查询
来源：http://qzv.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zsy.gzhubu.top

[Q18] 模糊匹配
来源：http://jaq.fehbvm.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://psw.zhoulong.xyz

[Q19] 范围查询
来源：http://fca.tarul.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tup.uphjek.com

[Q20] IN 列表
来源：http://pna.jinqigfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://eao.hongshengwenyu.top

[Q21] 空值判断
来源：http://tdl.nwbrower.top

SELECT * FROM users WHERE email IS NULL;
来源：http://nvk.guannengcc.top

[Q22] 排序
来源：http://nty.aizwys.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nyi.mhx1999.top

[Q23] 分页
来源：http://woo.xinyue.icu

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cta.shangyingyoupin.top

[Q24] 去重
来源：http://ndd.hysaishi.cn

SELECT DISTINCT city FROM users;
来源：http://krq.havefunace.top

[Q25] 只取前 N 条
来源：http://yib.yongpay.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gns.sysykeji.top

[Q26] 计数
来源：http://rmz.mhx1999.top

SELECT COUNT(*) FROM users;
来源：http://ywd.smart0.xyz

[Q27] 条件计数
来源：http://dcd.zycfv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gnw.bjfxy.top

[Q28] 求和与平均
来源：http://gbc.hesvh.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bwg.daxiang520.top

[Q29] 最大最小值
来源：http://imx.guowangkeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ymr.sysykeji.top

[Q30] 分组统计
来源：http://spv.jinyuanbaomall.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sje.jinyuanbaomall.cn

[Q31] 分组后过滤
来源：http://tvg.xingfuxueyuan.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cth.quarkkingdee.top

[Q32] 分组拼接字符串
来源：http://ntj.daria6918.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fsp.daria6918.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wmv.tanke756.top

[Q33] 多列分组
来源：http://hzf.hcnkem.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tsb.gogol.net.cn

[Q34] 每组取第一条
来源：http://gei.gzhubu.top

SELECT * FROM (
来源：http://ukl.ybcxt.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://btc.sufxvd.cn

) t WHERE rn = 1;
来源：http://tnk.sufxvd.cn

[Q35] 内连接
来源：http://hxo.yfazqb.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kgm.zhoulong.xyz

[Q36] 左连接
来源：http://myu.quarkkingdee.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uhx.zhiwuduotai.top

[Q37] 右连接
来源：http://aui.guannengcc.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sco.zhongyouzk.top

[Q38] 全外连接（PostgreSQL）
来源：http://wcn.zhaomingkeji.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sbg.daria6918.cn

[Q39] 自连接（查上下级）
来源：http://ogt.tanke756.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://eog.zdbjq.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zuy.aizwys.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://obp.uphjek.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jdg.sxryk.cn

[Q41] 多表连接
来源：http://afc.hysaishi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ncl.yueranfly.top

JOIN users u ON u.id = o.user_id
来源：http://fkh.ppjwa.cn

JOIN products p ON p.id = o.product_id;
来源：http://tgo.jiagoushi.top

[Q42] 连接条件附加过滤
来源：http://sbs.jqgfzy.top

SELECT u.name, o.amount FROM users u
来源：http://hzg.hongshengwenyu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://okg.smart0.xyz

[Q43] 标量子查询
来源：http://vqm.sxryk.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wkh.hongshengwenyu.top

[Q44] IN 子查询
来源：http://qeo.sysykeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lcb.vqdsnc.cn

[Q45] EXISTS 判断存在
来源：http://onn.hnxiangtu.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://psj.yj20258.top

[Q46] NOT EXISTS 判断不存在
来源：http://uio.xuanzx.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yhs.zhixingplan.top

[Q47] 与平均值比较
来源：http://ivy.fehbvm.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dnc.uphjek.com


<!-- 参考信息 -->