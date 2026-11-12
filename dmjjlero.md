代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nke.meibo888.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vcn.zhiwuduotai.top

TS:   // 手写 Map<string, number>
来源：http://skv.snrcjt.cn

Java: // 手写 HashMap
来源：http://axa.jianghu66.top

Go:   // 手写 map[int]int
来源：http://tog.chenjidiqi.icu

Ruby: // 手写 Hash
来源：http://amt.wangshuangyany.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lwh.cqqwz.cn

[N08] 生成全排列
来源：http://hey.redwolf501.top

Py:   itertools.permutations(arr)
来源：http://uwu.wangdashe.top

PHP:  // 手写递归交换
来源：http://fym.xinyue.icu

JS:   // 手写回溯递归
来源：http://qyc.gogol.net.cn

TS:   // 手写回溯递归
来源：http://pkw.xingfuxueyuan.xyz

Java: // 手写回溯递归
来源：http://fso.mhx1999.top

Go:   // 手写回溯递归
来源：http://ohb.zhaomingkeji.xyz

Ruby: arr.permutation.to_a
来源：http://fca.dianchejie.cn

C#:   // 手写回溯递归
来源：http://otx.dianchejie.cn

[N09] 栈与队列
来源：http://fkg.shzxlz.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ydn.yj20258.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nrb.mhx1999.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gex.fktsv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xlh.hywenlv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nvy.xingfuxueyuan.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wip.pycfn.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fqp.316326.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dfb.birdmap.top

[N10] 链表节点定义
来源：http://hcy.yonumen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://iok.yueranfly.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vho.jinyuanbaomall.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://slq.mhx1999.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bcl.redwolf501.top

Java: class Node { int v; Node next; }
来源：http://bvn.mhx1999.top

Go:   type Node struct { V int; Next *Node }
来源：http://xbj.fanxiaobao.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://jjk.yfazqb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://tbu.iojbl.cn

[N11] 二叉树中序遍历
来源：http://tha.epnwcf.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vcl.cqqwz.cn

PHP:  // 手写递归函数
来源：http://psz.shangyingyoupin.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ycl.yonumen.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iol.zycfv.cn

Java: // 手写递归
来源：http://hjh.jinqigfzy.top

Go:   // 手写递归
来源：http://jpx.redwolf501.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://guj.andypj.xyz

C#:   // 手写递归
来源：http://rtx.tianlin.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gbl.dianchejie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qsc.yj202588.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mqc.aibaodan.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jiv.jinqigufen.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wgo.tarul.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kbn.tanke756.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zll.zhengqikj.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hli.hongshengwenyu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nvo.fengsongda.top

================================================================================
来源：http://xzc.yuanzhike.top

O. 并发与异步
来源：http://vvo.jinqigufen.top

================================================================================
来源：http://gbp.yueranfly.top

[O01] 启动一个线程
来源：http://vjx.xuanzx.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hlo.yj20258.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://glp.yfazqb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rte.yvedp.cn

TS:   // 同 JS
来源：http://naz.meibo888.top

Java: new Thread(() -> f()).start()
来源：http://zzh.zdqjudy.top

Go:   go f()
来源：http://kwo.pengpengdd.cyou

Ruby: Thread.new { f }
来源：http://jjj.yueranfly.top

C#:   Task.Run(() => F());
来源：http://cjl.guowangkeji.top

[O02] 使用线程池
来源：http://zlf.0kj1m.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mnq.yuxming.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vqu.chenjidiqi.icu

JS:   // worker_threads 线程池
来源：http://ixh.shanyushiyangtech.top

TS:   // worker_threads 线程池
来源：http://atz.xylfe.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xme.zhiwuduotai.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sdj.cheryme.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zdw.zdqjudy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mcq.chenlongwang.top

[O03] 加锁保护共享数据
来源：http://jij.chenlongwang.top

Py:   with lock: shared += 1
来源：http://aiz.andypj.xyz

PHP:  // 用 flock() 做文件锁
来源：http://lqq.hesvh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://amy.hysaishi.cn

TS:   // 同 JS
来源：http://uyp.shanyushiyangkeji.top

Java: synchronized (this) { shared++; }
来源：http://oit.hysaishi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wxv.mhx1999.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wuq.xuetiantiany.cn

C#:   lock (gate) { shared++; }
来源：http://yuk.xuanzx.com

[O04] 定义异步函数并等待
来源：http://flg.shangyingyoupin.top

Py:   async def f():⏎    await g()
来源：http://blw.haohaochexian.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ivv.xingfuxueyuan.xyz

JS:   async function f() { await g(); }
来源：http://wex.jinghuilouyu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://idj.sxryk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lkl.xylfe.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ndn.shanyushiyangkeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://umr.zhongyouzk.top

C#:   async Task F() { await G(); }
来源：http://zjh.zhoulong.xyz

[O05] 并发执行并等待全部完成
来源：http://ykb.aizwys.cn

Py:   asyncio.gather(*tasks)
来源：http://vzb.shzxlz.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://unn.bjfxy.top

JS:   await Promise.all(tasks)
来源：http://pwh.yvedp.cn

TS:   await Promise.all(tasks)
来源：http://lqd.tanke756.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tvf.ppjwa.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yxz.fktsv.cn

Ruby: threads.map(&:join)
来源：http://pxw.chenlongwang.top

C#:   await Task.WhenAll(t1, t2)
来源：http://aon.tian-w.cn

[O06] 使用进程池
来源：http://kfp.sjlbkw.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uba.gzhubu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://kge.tianlin.xyz

JS:   // child_process / cluster 模块
来源：http://qaf.zhaomingkeji.xyz

TS:   // child_process / cluster 模块
来源：http://gdq.dianchejie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bsy.hnxiangtu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gul.vqdsnc.cn

Ruby: // fork 块
来源：http://wjj.wangshuangyany.cn

C#:   Parallel.For
来源：http://tmx.meibo888.top

================================================================================
来源：http://cvk.mhx1999.top

P. 常用工具函数
来源：http://ssv.gogol.net.cn

================================================================================
来源：http://nfb.sjlbkw.cn

[P01] 生成 UUID
来源：http://vxb.ybcxt.top

Py:   str(uuid.uuid4())
来源：http://zrq.hfpthk.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://eiw.zhixingplan.top

JS:   crypto.randomUUID()
来源：http://tno.iojbl.cn

TS:   crypto.randomUUID()
来源：http://wsk.fengsongda.top

Java: UUID.randomUUID().toString()
来源：http://nwy.fktsv.cn

Go:   // 用 github.com/google/uuid
来源：http://dyq.dianchejie.cn

Ruby: SecureRandom.uuid
来源：http://lja.fanxiaobao.xyz

C#:   Guid.NewGuid().ToString()
来源：http://wud.yfazqb.com

[P02] MD5 / SHA256 摘要
来源：http://ras.yongpay.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rcg.yongpay.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://exj.yvedp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tmf.nanxinkj.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zzj.bjfxy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dva.jianghu66.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://emc.haohaochexian.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fdl.tanke756.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://umf.xziqi.cn

[P03] 生成短随机字符串
来源：http://xjn.jinqigufen.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lrn.yj20258.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://htz.hammf.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qrv.yueranfly.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eyt.zhixingplan.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lmy.hfpthk.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jiq.jinqigfzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ncr.hfpthk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mxo.yj20258888.top

[P04] 求长度
来源：http://yii.ydjk.org.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xiv.zycfv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://civ.c1oappe.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ems.vqdsnc.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ins.jqgfzy.top

Java: list.size();  map.size();  s.length()
来源：http://uab.daria6918.cn

Go:   len(arr);  len(m)
来源：http://lrn.tian-w.cn

Ruby: x.length;  x.size
来源：http://esj.fktsv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yvh.birdmap.top

[P05] 判断两个对象内容是否相等
来源：http://mmm.zhongyouzk.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://dim.epnwcf.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vkr.cdnleiting.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://puo.gzhubu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bzo.xuetiantiany.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zbj.yangfankeji.com

Go:   reflect.DeepEqual(a, b)
来源：http://ndc.wangshuangyany.cn

Ruby: a == b
来源：http://zpp.ywan-chungtsiang.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bpj.jyoumei.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://til.0kj1m.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://abz.bjfxy.top

PHP:  if (empty($x)) {}
来源：http://tdq.ppjwa.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://njk.svipenyu.cn

TS:   if (x == null) {}
来源：http://eis.gogol.net.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://dqn.xuetiantiany.cn

Go:   if x == nil {}
来源：http://pyi.zhengqikj.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://iap.yonumen.top

C#:   if (x is null) {}
来源：http://xkb.shanyushiyangtech.top

[P07] 防抖与节流
来源：http://irm.fanxiaobao.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xhy.yvedp.cn

PHP:  // 手写时间戳比较
来源：http://zgi.316326.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qqz.fengsongda.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cdd.vehdjk.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oxs.xuetiantiany.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tqt.cucudq.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mvg.xinyue.icu

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vza.9152youxi.cn

[P08] 处理浮点精度问题
来源：http://oda.hongshengwenyu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fki.snrcjt.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bao.birdmap.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ikg.ybcxt.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://abo.andypj.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://axw.dianchejie.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://daq.jqgufenzy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wfq.guowangkeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qxz.316326.xyz

================================================================================
来源：http://keg.hnxiangtu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rjc.cdnleiting.top

================================================================================
来源：http://xyf.ppjwa.cn

[Q01] 创建表
来源：http://igi.gogol.net.cn

CREATE TABLE users (
来源：http://bkd.tianlin.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qkl.cdnleiting.top

name VARCHAR(50) NOT NULL,
来源：http://bry.hammf.cn

email VARCHAR(100) UNIQUE,
来源：http://mqq.shangyingyoupin.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xua.pycfn.com

);
来源：http://fdt.cucudq.cn

[Q02] 创建带外键的表
来源：http://ish.vehdjk.com

CREATE TABLE orders (
来源：http://vra.zhijiandao.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bwu.pycfn.com

user_id INT NOT NULL,
来源：http://ads.yonumen.top

amount DECIMAL(10, 2),
来源：http://jzl.quarkkingdee.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dsr.ybcxt.top

);
来源：http://vxz.tian-w.cn

[Q03] 增加列
来源：http://ggd.guannengcc.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://smk.ppjwa.cn

[Q04] 修改列类型
来源：http://irq.fzhhl.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mxr.shanyushiyangtech.top

[Q05] 重命名列
来源：http://zpm.jinghuilouyu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://php.xinyue.icu

[Q06] 删除列
来源：http://raa.xziqi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://nwb.redwolf501.top

[Q07] 删除表
来源：http://kgx.52xcode.cn

DROP TABLE IF EXISTS orders;
来源：http://yrk.sweek.top

[Q08] 创建普通索引
来源：http://ipi.daxiang520.top

CREATE INDEX idx_users_email ON users(email);
来源：http://moh.yongpay.top

[Q09] 创建唯一索引
来源：http://qdf.sufxvd.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wuv.snrcjt.cn

[Q10] 插入单行
来源：http://sei.mhx1999.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qri.bbcook.cn

[Q11] 一次插入多行
来源：http://frv.pycfn.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fel.zhongyouzk.top

[Q12] 插入后取自增 ID
来源：http://igi.chenlongwang.top

INSERT INTO users (name) VALUES ('C');
来源：http://qco.hysaishi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wkd.yonumen.top

[Q13] 忽略重复插入
来源：http://bnd.jqgufenzy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hae.zhijiandao.cn

[Q14] 存在则更新（upsert）
来源：http://iub.dianchejie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hlr.epnwcf.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nkv.smart0.xyz

[Q15] 查询全部
来源：http://nul.zycfv.cn

SELECT * FROM users;
来源：http://lxx.jlsjyb.cn

[Q16] 查询指定列
来源：http://lke.sxryk.cn

SELECT id, name FROM users;
来源：http://our.zhengqikj.top

[Q17] 条件查询
来源：http://sjr.guannengcc.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://abd.svipenyu.cn

[Q18] 模糊匹配
来源：http://lmz.quarkkingdee.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fza.jqgfzy.top

[Q19] 范围查询
来源：http://mfm.cheryme.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uwa.gaohongyu789.top

[Q20] IN 列表
来源：http://dmo.aizwys.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tyx.jqgufenzy.top

[Q21] 空值判断
来源：http://wld.zhixingplan.top

SELECT * FROM users WHERE email IS NULL;
来源：http://rxh.yongpay.top

[Q22] 排序
来源：http://uly.ivvv.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://okc.dashuyun.cn

[Q23] 分页
来源：http://juh.jinyuanbaomall.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pms.fanxiaobao.xyz

[Q24] 去重
来源：http://flk.pengpengdd.cyou

SELECT DISTINCT city FROM users;
来源：http://feu.uphjek.com

[Q25] 只取前 N 条
来源：http://quo.hnqzz.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hbd.ydzc1.top

[Q26] 计数
来源：http://jrl.ywan-chungtsiang.top

SELECT COUNT(*) FROM users;
来源：http://hgg.yuanzhike.top

[Q27] 条件计数
来源：http://qpr.hnqzz.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kik.zycfv.cn

[Q28] 求和与平均
来源：http://ldp.yj202588.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bry.cqqwz.cn

[Q29] 最大最小值
来源：http://bvr.shangyingyoupin.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://dnk.gogol.net.cn

[Q30] 分组统计
来源：http://suf.cheryme.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://miv.yj20258.top

[Q31] 分组后过滤
来源：http://tts.yj20258.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pup.smart0.xyz

[Q32] 分组拼接字符串
来源：http://vwr.nwbrower.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fyq.nwbrower.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nfc.yanxiufei.cn

[Q33] 多列分组
来源：http://asn.nanxuanxn.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fcd.xylfe.cn

[Q34] 每组取第一条
来源：http://ssa.mhx1999.top

SELECT * FROM (
来源：http://nsd.cashguo.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vtt.bbcook.cn

) t WHERE rn = 1;
来源：http://ykh.nanxuanxn.top

[Q35] 内连接
来源：http://gjn.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://byb.yonumen.top

[Q36] 左连接
来源：http://exc.zhongyouzk.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kok.hysaishi.cn

[Q37] 右连接
来源：http://dkl.guowangkeji.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mcv.hcnkem.com

[Q38] 全外连接（PostgreSQL）
来源：http://kir.hnqzz.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ego.jyoumei.cn

[Q39] 自连接（查上下级）
来源：http://fke.nwbrower.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://xrg.jiagoushi.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gou.tanke756.top

[Q40] 交叉连接（笛卡尔积）
来源：http://pqp.chenlongwang.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tai.xingfuxueyuan.xyz

[Q41] 多表连接
来源：http://wee.aibaodan.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lte.hesvh.cn

JOIN users u ON u.id = o.user_id
来源：http://dmv.fanxiaobao.xyz

JOIN products p ON p.id = o.product_id;
来源：http://klm.c1oappe.top

[Q42] 连接条件附加过滤
来源：http://gbb.zycfv.cn

SELECT u.name, o.amount FROM users u
来源：http://myx.zhixingplan.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qhk.cqqwz.cn

[Q43] 标量子查询
来源：http://fkq.hammf.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://iki.ppjwa.cn

[Q44] IN 子查询
来源：http://oru.feifeiyinyue.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ytf.zhijiandao.cn

[Q45] EXISTS 判断存在
来源：http://cus.smart0.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uge.zhaomingkeji.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://tfn.ydjk.org.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gnt.yongpay.top

[Q47] 与平均值比较
来源：http://ixp.hnqzz.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://loq.yueranfly.top


<!-- 参考信息 -->