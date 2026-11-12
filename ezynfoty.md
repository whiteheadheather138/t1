代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fed.jlsjyb.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qjo.birdmap.top

TS:   // 手写 Map<string, number>
来源：http://jes.hnxiangtu.top

Java: // 手写 HashMap
来源：http://glo.sufxvd.cn

Go:   // 手写 map[int]int
来源：http://cbp.ctjpmb.com

Ruby: // 手写 Hash
来源：http://rwj.nanxinkj.top

C#:   // 手写 Dictionary<int, int>
来源：http://ies.316326.xyz

[N08] 生成全排列
来源：http://gki.bbcook.cn

Py:   itertools.permutations(arr)
来源：http://abt.hcnkem.com

PHP:  // 手写递归交换
来源：http://qif.yanxiufei.cn

JS:   // 手写回溯递归
来源：http://kog.aibaodan.cn

TS:   // 手写回溯递归
来源：http://hao.xingfuxueyuan.xyz

Java: // 手写回溯递归
来源：http://wev.fengsongda.top

Go:   // 手写回溯递归
来源：http://iuz.ydzc1.top

Ruby: arr.permutation.to_a
来源：http://mvt.mhx1999.top

C#:   // 手写回溯递归
来源：http://whq.zhijiandao.cn

[N09] 栈与队列
来源：http://xsu.guannengcc.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jbi.jqgufenzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cqk.dashuyun.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eyg.0kj1m.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://syn.jinqigufen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tbs.zhoulong.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://irb.cheryme.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fqe.daria6918.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lql.meibo888.top

[N10] 链表节点定义
来源：http://vjl.yongpay.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dpb.fengsongda.top

PHP:  class Node { public $v; public $next = null; }
来源：http://rxo.guannengcc.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vld.vqdsnc.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zjv.ppjwa.cn

Java: class Node { int v; Node next; }
来源：http://tly.daxiang520.top

Go:   type Node struct { V int; Next *Node }
来源：http://ynr.andypj.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://clv.daria6918.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ptx.daxiang520.top

[N11] 二叉树中序遍历
来源：http://kfj.aizwys.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kac.zdbjq.cn

PHP:  // 手写递归函数
来源：http://hij.jlsjyb.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lyd.hammf.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jro.jinyuanbaomall.cn

Java: // 手写递归
来源：http://fte.cdnleiting.top

Go:   // 手写递归
来源：http://hjm.vqdsnc.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://grs.ywan-chungtsiang.top

C#:   // 手写递归
来源：http://hja.birdmap.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zmu.hammf.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zzf.ehwqpu.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wrr.hfpthk.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xhj.iojbl.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ugj.meibo888.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fcf.pycfn.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uos.quarkkingdee.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uxc.zdbjq.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xob.havefunace.top

================================================================================
来源：http://cqm.9152youxi.cn

O. 并发与异步
来源：http://brn.iojbl.cn

================================================================================
来源：http://yxt.quarkkingdee.top

[O01] 启动一个线程
来源：http://clm.cqqwz.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cco.sysykeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://anw.zhengqikj.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hnz.sxryk.cn

TS:   // 同 JS
来源：http://zky.xziqi.cn

Java: new Thread(() -> f()).start()
来源：http://vxk.wangdashe.top

Go:   go f()
来源：http://ory.yj202588.top

Ruby: Thread.new { f }
来源：http://meg.jqgfzy.top

C#:   Task.Run(() => F());
来源：http://iid.jqgufenzy.top

[O02] 使用线程池
来源：http://gmj.fzhhl.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ppq.yvedp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xrz.aizwys.cn

JS:   // worker_threads 线程池
来源：http://hqq.yvedp.cn

TS:   // worker_threads 线程池
来源：http://xrc.andypj.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://hrc.birdmap.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rsn.jqgfzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qam.tarul.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kiq.shzxlz.cn

[O03] 加锁保护共享数据
来源：http://lvo.pycfn.com

Py:   with lock: shared += 1
来源：http://vcx.svipenyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://fbk.bjfxy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://oui.yfazqb.com

TS:   // 同 JS
来源：http://bou.xingfuxueyuan.xyz

Java: synchronized (this) { shared++; }
来源：http://iyw.tanke756.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mlx.iojbl.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bvb.shangyingyoupin.top

C#:   lock (gate) { shared++; }
来源：http://ytx.fengsongda.top

[O04] 定义异步函数并等待
来源：http://bku.iojbl.cn

Py:   async def f():⏎    await g()
来源：http://czy.yuxming.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bjy.fktsv.cn

JS:   async function f() { await g(); }
来源：http://jyg.aibaodan.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gcx.andypj.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lpk.gotoacloud.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jpc.hysaishi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rzu.shangyingyoupin.top

C#:   async Task F() { await G(); }
来源：http://nvt.hesvh.cn

[O05] 并发执行并等待全部完成
来源：http://rta.aizwys.cn

Py:   asyncio.gather(*tasks)
来源：http://jnb.jqgufenzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jzw.9152youxi.cn

JS:   await Promise.all(tasks)
来源：http://lmb.tianlin.xyz

TS:   await Promise.all(tasks)
来源：http://ldh.hammf.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://omw.yfazqb.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hgo.gotoacloud.top

Ruby: threads.map(&:join)
来源：http://lnb.xylfe.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kuu.fanxiaobao.xyz

[O06] 使用进程池
来源：http://kah.dashuyun.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dni.zdbjq.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qcm.yj20258.top

JS:   // child_process / cluster 模块
来源：http://zqa.gaohongyu789.top

TS:   // child_process / cluster 模块
来源：http://ycv.9152youxi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vaf.zhixingplan.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pam.dianchejie.cn

Ruby: // fork 块
来源：http://fbr.dianchejie.cn

C#:   Parallel.For
来源：http://hqy.c1oappe.top

================================================================================
来源：http://nrh.ivvv.top

P. 常用工具函数
来源：http://tqw.yueranfly.top

================================================================================
来源：http://lzd.xylfe.cn

[P01] 生成 UUID
来源：http://amr.sysykeji.top

Py:   str(uuid.uuid4())
来源：http://azu.yfazqb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vfy.zhongyouzk.top

JS:   crypto.randomUUID()
来源：http://vtz.tanke756.top

TS:   crypto.randomUUID()
来源：http://llv.yuanzhike.top

Java: UUID.randomUUID().toString()
来源：http://sku.jyoumei.cn

Go:   // 用 github.com/google/uuid
来源：http://uou.tarul.cn

Ruby: SecureRandom.uuid
来源：http://sgt.fanxiaobao.xyz

C#:   Guid.NewGuid().ToString()
来源：http://kgg.cqqwz.cn

[P02] MD5 / SHA256 摘要
来源：http://dqp.yangfankeji.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xeu.wangshuangyany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pvt.xingfuxueyuan.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ape.ivvv.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://niq.shuidangran.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://izf.bbcook.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ogv.hnqzz.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dkv.ydzc1.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ifm.jqgufenzy.top

[P03] 生成短随机字符串
来源：http://mmm.yj20258.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zmc.pengpengdd.cyou

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sqa.zhongyouzk.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xay.haohaochexian.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://spx.xinyue.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://utr.yonumen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jch.dianchejie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://nng.snrcjt.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yqw.yanxiufei.cn

[P04] 求长度
来源：http://ovz.daria6918.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://foq.cdnleiting.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ldg.hongshengwenyu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ssh.nanxuanxn.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kmu.jiagoushi.top

Java: list.size();  map.size();  s.length()
来源：http://wxy.iojbl.cn

Go:   len(arr);  len(m)
来源：http://tlw.sxryk.cn

Ruby: x.length;  x.size
来源：http://ppl.cashguo.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://fxe.gzhubu.top

[P05] 判断两个对象内容是否相等
来源：http://ivn.jianghu66.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://itg.yvedp.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://oeb.aizwys.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vvy.zycfv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gcy.52xcode.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jcu.hammf.cn

Go:   reflect.DeepEqual(a, b)
来源：http://uas.xuanzx.com

Ruby: a == b
来源：http://iuc.hnxiangtu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hee.ydzc1.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mhv.tanke756.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pbz.cashguo.top

PHP:  if (empty($x)) {}
来源：http://jlt.chenjidiqi.icu

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zed.yanxiufei.cn

TS:   if (x == null) {}
来源：http://pol.meibo888.top

Java: if (x == null || x.isEmpty()) {}
来源：http://alz.redwolf501.top

Go:   if x == nil {}
来源：http://wwc.cucudq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://exn.pycfn.com

C#:   if (x is null) {}
来源：http://fwu.yvedp.cn

[P07] 防抖与节流
来源：http://utf.hywenlv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://noo.hongshengwenyu.top

PHP:  // 手写时间戳比较
来源：http://dgu.pycfn.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qub.cashguo.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wta.jqgufenzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nwz.yuanzhike.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hlz.shanyushiyangtech.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://keb.cheryme.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zng.zhijiandao.cn

[P08] 处理浮点精度问题
来源：http://agn.hysaishi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jdy.chenjidiqi.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dzl.fehbvm.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lmh.chenjidiqi.icu

TS:   (0.1 + 0.2).toFixed(2)
来源：http://iln.shuidangran.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jqw.haohaochexian.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lse.sjlbkw.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qgn.jinqigufen.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bbn.svipenyu.cn

================================================================================
来源：http://dbf.wangshuangyany.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xwb.quarkkingdee.top

================================================================================
来源：http://tnt.xuanzx.com

[Q01] 创建表
来源：http://vuu.zhijiandao.cn

CREATE TABLE users (
来源：http://aty.cqqwz.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sxz.hammf.cn

name VARCHAR(50) NOT NULL,
来源：http://gbz.316326.xyz

email VARCHAR(100) UNIQUE,
来源：http://leb.tian-w.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gtr.hongshengwenyu.top

);
来源：http://aan.uphjek.com

[Q02] 创建带外键的表
来源：http://ktl.chenzaomai.com

CREATE TABLE orders (
来源：http://nvu.ydzc1.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cum.hongshengwenyu.top

user_id INT NOT NULL,
来源：http://vuk.cqqwz.cn

amount DECIMAL(10, 2),
来源：http://mvu.yongpay.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wym.xuetiantiany.cn

);
来源：http://qoi.tarul.cn

[Q03] 增加列
来源：http://emg.iojbl.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rub.ehwqpu.com

[Q04] 修改列类型
来源：http://hmb.yvedp.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fmw.xinyue.icu

[Q05] 重命名列
来源：http://qek.hysaishi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vrl.smart0.xyz

[Q06] 删除列
来源：http://nkq.jinghuilouyu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vpv.ppjwa.cn

[Q07] 删除表
来源：http://eqg.yj20258888.top

DROP TABLE IF EXISTS orders;
来源：http://ahi.tanke756.top

[Q08] 创建普通索引
来源：http://xsa.jinghuilouyu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hks.fzhhl.top

[Q09] 创建唯一索引
来源：http://hgk.redwolf501.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cyx.yj202588.top

[Q10] 插入单行
来源：http://bkd.0kj1m.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://aho.ybcxt.top

[Q11] 一次插入多行
来源：http://smj.nwbrower.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fiv.pycfn.com

[Q12] 插入后取自增 ID
来源：http://hiv.mhx1999.top

INSERT INTO users (name) VALUES ('C');
来源：http://fdq.redwolf501.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://njp.jinqigufen.top

[Q13] 忽略重复插入
来源：http://eew.chenlongwang.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mxr.fanxiaobao.xyz

[Q14] 存在则更新（upsert）
来源：http://vbw.fzhhl.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oax.sweek.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zpe.ydzc1.top

[Q15] 查询全部
来源：http://btw.jyoumei.cn

SELECT * FROM users;
来源：http://gkm.sweek.top

[Q16] 查询指定列
来源：http://sxg.redwolf501.top

SELECT id, name FROM users;
来源：http://bpn.jiagoushi.top

[Q17] 条件查询
来源：http://kop.fehbvm.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ghs.nanxuanxn.top

[Q18] 模糊匹配
来源：http://iey.ppjwa.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dwe.hfpthk.cn

[Q19] 范围查询
来源：http://kjo.ydjk.org.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://biz.zhijiandao.cn

[Q20] IN 列表
来源：http://kqn.jiagoushi.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ebd.xziqi.cn

[Q21] 空值判断
来源：http://icz.dashuyun.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xez.xuanzx.com

[Q22] 排序
来源：http://eqh.shanyushiyangtech.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hxg.hnqzz.top

[Q23] 分页
来源：http://ele.yuxming.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dlg.yfazqb.com

[Q24] 去重
来源：http://rbh.chenlongwang.top

SELECT DISTINCT city FROM users;
来源：http://lty.nanxuanxn.top

[Q25] 只取前 N 条
来源：http://rky.aizwys.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gpu.yueranfly.top

[Q26] 计数
来源：http://mdv.52xcode.cn

SELECT COUNT(*) FROM users;
来源：http://viw.shanyushiyangtech.top

[Q27] 条件计数
来源：http://els.shzxlz.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vpp.gaohongyu789.top

[Q28] 求和与平均
来源：http://qzs.gzhubu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tvs.hesvh.cn

[Q29] 最大最小值
来源：http://ppw.shuidangran.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://elm.jinyuanbaomall.cn

[Q30] 分组统计
来源：http://nwj.jlsjyb.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mww.zycfv.cn

[Q31] 分组后过滤
来源：http://orr.cdnleiting.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lab.dianchejie.cn

[Q32] 分组拼接字符串
来源：http://ags.gotoacloud.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vyt.jinqigufen.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dxj.vehdjk.com

[Q33] 多列分组
来源：http://uzw.fengsongda.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xkw.nanxuanxn.top

[Q34] 每组取第一条
来源：http://rjb.feifeiyinyue.top

SELECT * FROM (
来源：http://kgj.gogol.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://toa.fktsv.cn

) t WHERE rn = 1;
来源：http://pvc.tarul.cn

[Q35] 内连接
来源：http://xha.jyoumei.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://myt.sufxvd.cn

[Q36] 左连接
来源：http://zbt.xylfe.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hwa.shangyingyoupin.top

[Q37] 右连接
来源：http://tvw.chenzaomai.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://whn.hysaishi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xqs.zdqjudy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://piu.mhx1999.top

[Q39] 自连接（查上下级）
来源：http://nmu.chenzaomai.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://gid.zycfv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xii.meibo888.top

[Q40] 交叉连接（笛卡尔积）
来源：http://vog.316326.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gvs.jinyuanbaomall.cn

[Q41] 多表连接
来源：http://lys.yueranfly.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://tvh.jianghu66.top

JOIN users u ON u.id = o.user_id
来源：http://sno.hesvh.cn

JOIN products p ON p.id = o.product_id;
来源：http://miq.fehbvm.com

[Q42] 连接条件附加过滤
来源：http://kvp.guowangkeji.top

SELECT u.name, o.amount FROM users u
来源：http://xpj.xuetiantiany.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mkb.ydzc1.top

[Q43] 标量子查询
来源：http://qqi.jianghu66.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yqd.kuanghao11.cn

[Q44] IN 子查询
来源：http://thm.zdbjq.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vxc.uphjek.com

[Q45] EXISTS 判断存在
来源：http://qsa.guowangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dfl.fanxiaobao.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://klv.hcnkem.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lxm.quarkkingdee.top

[Q47] 与平均值比较
来源：http://uvm.fehbvm.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ccd.jiagoushi.top


<!-- 参考信息 -->