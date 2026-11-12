代发 wailian999

Go:   // 手写 map[int]int
来源：http://azq.yuanzhike.top

Ruby: // 手写 Hash
来源：http://dqu.xuetiantiany.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rdz.wangdashe.top

[N08] 生成全排列
来源：http://gps.xingfuxueyuan.xyz

Py:   itertools.permutations(arr)
来源：http://fxt.snrcjt.cn

PHP:  // 手写递归交换
来源：http://ssm.zhoulong.xyz

JS:   // 手写回溯递归
来源：http://spl.9152youxi.cn

TS:   // 手写回溯递归
来源：http://sav.yj20258.top

Java: // 手写回溯递归
来源：http://lfy.svipenyu.cn

Go:   // 手写回溯递归
来源：http://cnq.xuetiantiany.cn

Ruby: arr.permutation.to_a
来源：http://vyc.quarkkingdee.top

C#:   // 手写回溯递归
来源：http://lvj.xuanzx.com

[N09] 栈与队列
来源：http://nsi.jiagoushi.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vdx.zdbjq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jed.cdnleiting.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ehg.sjlbkw.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hui.kuanghao11.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cmq.gzhubu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hsp.shanyushiyangkeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mup.jinghuilouyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fkn.meibo888.top

[N10] 链表节点定义
来源：http://vpu.yj20258.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zyp.zhoulong.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://jzn.jyoumei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pvt.gaohongyu789.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uai.feifeiyinyue.top

Java: class Node { int v; Node next; }
来源：http://nlc.hcnkem.com

Go:   type Node struct { V int; Next *Node }
来源：http://bjm.9152youxi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zjf.sysykeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://asj.guowangkeji.top

[N11] 二叉树中序遍历
来源：http://ahv.sjlbkw.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ubr.sjlbkw.cn

PHP:  // 手写递归函数
来源：http://uxy.gaohongyu789.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jus.aibaodan.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vje.redwolf501.top

Java: // 手写递归
来源：http://frt.kuanghao11.cn

Go:   // 手写递归
来源：http://wug.havefunace.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zqe.chenzaomai.com

C#:   // 手写递归
来源：http://jif.tian-w.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ybx.gzhubu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qno.nanxuanxn.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tnq.fehbvm.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cpb.jqgufenzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iub.chenlongwang.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://byf.xuanzx.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cto.xuanzx.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zbm.zhongyouzk.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sle.epnwcf.com

================================================================================
来源：http://vfn.xingfuxueyuan.xyz

O. 并发与异步
来源：http://cjs.xingfuxueyuan.xyz

================================================================================
来源：http://zvd.uphjek.com

[O01] 启动一个线程
来源：http://nmu.shanyushiyangtech.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yxb.cucudq.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ctz.redwolf501.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://slc.sxryk.cn

TS:   // 同 JS
来源：http://iph.havefunace.top

Java: new Thread(() -> f()).start()
来源：http://ebs.xinyue.icu

Go:   go f()
来源：http://dod.shuidangran.top

Ruby: Thread.new { f }
来源：http://efz.tarul.cn

C#:   Task.Run(() => F());
来源：http://ycg.snrcjt.cn

[O02] 使用线程池
来源：http://hce.ydzc1.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ojz.316326.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://aci.yonumen.top

JS:   // worker_threads 线程池
来源：http://mru.andypj.xyz

TS:   // worker_threads 线程池
来源：http://wvn.shanyushiyangtech.top

Java: Executors.newFixedThreadPool(4)
来源：http://gnn.hnqzz.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vpm.316326.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mma.yangfankeji.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lgg.dashuyun.cn

[O03] 加锁保护共享数据
来源：http://sfu.svipenyu.cn

Py:   with lock: shared += 1
来源：http://cvs.yj20258.top

PHP:  // 用 flock() 做文件锁
来源：http://eex.wangdashe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://njm.wangdashe.top

TS:   // 同 JS
来源：http://dci.nanxinkj.top

Java: synchronized (this) { shared++; }
来源：http://qqc.pycfn.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qgk.gogol.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cgl.cqqwz.cn

C#:   lock (gate) { shared++; }
来源：http://vpc.jinqigufen.top

[O04] 定义异步函数并等待
来源：http://nlh.xziqi.cn

Py:   async def f():⏎    await g()
来源：http://dyf.yfazqb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://knl.havefunace.top

JS:   async function f() { await g(); }
来源：http://atu.zhixingplan.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://fro.xuanzx.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mzf.wangshuangyany.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://exj.gogol.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://prv.316326.xyz

C#:   async Task F() { await G(); }
来源：http://vbp.yueranfly.top

[O05] 并发执行并等待全部完成
来源：http://jkc.jiagoushi.top

Py:   asyncio.gather(*tasks)
来源：http://ccr.zhoulong.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jsm.ydzc1.top

JS:   await Promise.all(tasks)
来源：http://odg.fzhhl.top

TS:   await Promise.all(tasks)
来源：http://rfe.tianlin.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qfa.hywenlv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cuj.0kj1m.cn

Ruby: threads.map(&:join)
来源：http://zlq.jinqigufen.top

C#:   await Task.WhenAll(t1, t2)
来源：http://zkg.wangdashe.top

[O06] 使用进程池
来源：http://hab.yj20258888.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mwt.hfpthk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wca.dashuyun.cn

JS:   // child_process / cluster 模块
来源：http://bru.gogol.net.cn

TS:   // child_process / cluster 模块
来源：http://onq.hnxiangtu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vya.zdbjq.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://twb.gogol.net.cn

Ruby: // fork 块
来源：http://xcd.shanyushiyangtech.top

C#:   Parallel.For
来源：http://klt.gaohongyu789.top

================================================================================
来源：http://mjw.tanke756.top

P. 常用工具函数
来源：http://hyf.tanke756.top

================================================================================
来源：http://igw.c1oappe.top

[P01] 生成 UUID
来源：http://dfw.xinyue.icu

Py:   str(uuid.uuid4())
来源：http://ren.cashguo.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wdb.shanyushiyangkeji.top

JS:   crypto.randomUUID()
来源：http://ain.hysaishi.cn

TS:   crypto.randomUUID()
来源：http://ncq.redwolf501.top

Java: UUID.randomUUID().toString()
来源：http://ocx.bbcook.cn

Go:   // 用 github.com/google/uuid
来源：http://oxu.epnwcf.com

Ruby: SecureRandom.uuid
来源：http://qxt.zhixingplan.top

C#:   Guid.NewGuid().ToString()
来源：http://daj.chenlongwang.top

[P02] MD5 / SHA256 摘要
来源：http://eve.yj20258888.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nwo.jlsjyb.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fqk.fanxiaobao.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yna.cashguo.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jmy.aibaodan.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oiy.daria6918.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xev.shuidangran.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nnk.birdmap.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wpw.shzxlz.cn

[P03] 生成短随机字符串
来源：http://uje.redwolf501.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://exn.shuidangran.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wek.yj202588.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://boa.zdqjudy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mtb.tarul.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lfa.0kj1m.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qep.dianchejie.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://gqx.guowangkeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xln.jyoumei.cn

[P04] 求长度
来源：http://zgx.xziqi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://aqe.316326.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rep.yangfankeji.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nur.uphjek.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fft.yuanzhike.top

Java: list.size();  map.size();  s.length()
来源：http://dry.hysaishi.cn

Go:   len(arr);  len(m)
来源：http://pjn.tarul.cn

Ruby: x.length;  x.size
来源：http://aeb.cdnleiting.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://fqc.cheryme.top

[P05] 判断两个对象内容是否相等
来源：http://imt.snrcjt.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://nea.yvedp.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://svf.cashguo.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gpj.cheryme.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wow.hammf.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bzn.jiagoushi.top

Go:   reflect.DeepEqual(a, b)
来源：http://xul.tarul.cn

Ruby: a == b
来源：http://abv.jqgufenzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ezh.zhijiandao.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://spq.wangshuangyany.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sql.yvedp.cn

PHP:  if (empty($x)) {}
来源：http://ahz.hnxiangtu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://znl.tian-w.cn

TS:   if (x == null) {}
来源：http://fhw.gzhubu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ptg.sufxvd.cn

Go:   if x == nil {}
来源：http://pqy.cdnleiting.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://unb.andypj.xyz

C#:   if (x is null) {}
来源：http://hoo.andypj.xyz

[P07] 防抖与节流
来源：http://xpm.sysykeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vze.cucudq.cn

PHP:  // 手写时间戳比较
来源：http://upy.shangyingyoupin.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dea.ivvv.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uts.yonumen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ogm.zdbjq.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kgp.ppjwa.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dwk.xinyue.icu

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wri.ehwqpu.com

[P08] 处理浮点精度问题
来源：http://cua.jinqigfzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dzh.fzhhl.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jtu.svipenyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ncp.dianchejie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qdg.jinqigufen.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pzp.c1oappe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lvi.daria6918.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ezw.chenlongwang.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://weu.xuanzx.com

================================================================================
来源：http://pdt.yuanzhike.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://csu.aizwys.cn

================================================================================
来源：http://arq.tian-w.cn

[Q01] 创建表
来源：http://wtw.tarul.cn

CREATE TABLE users (
来源：http://qlv.yvedp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wyi.yfazqb.com

name VARCHAR(50) NOT NULL,
来源：http://amd.bbcook.cn

email VARCHAR(100) UNIQUE,
来源：http://dji.guannengcc.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://red.chenjidiqi.icu

);
来源：http://ugv.xinyue.icu

[Q02] 创建带外键的表
来源：http://uaj.shanyushiyangtech.top

CREATE TABLE orders (
来源：http://xsh.hnxiangtu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://myl.nanxuanxn.top

user_id INT NOT NULL,
来源：http://jhm.zdqjudy.top

amount DECIMAL(10, 2),
来源：http://ckg.316326.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zty.haohaochexian.top

);
来源：http://teo.uphjek.com

[Q03] 增加列
来源：http://ymy.aibaodan.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lzb.nanxinkj.top

[Q04] 修改列类型
来源：http://xuy.shanyushiyangtech.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ycz.nwbrower.top

[Q05] 重命名列
来源：http://hwy.sysykeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dsc.ybcxt.top

[Q06] 删除列
来源：http://pfg.pycfn.com

ALTER TABLE users DROP COLUMN age;
来源：http://wnt.yfazqb.com

[Q07] 删除表
来源：http://ydf.ybcxt.top

DROP TABLE IF EXISTS orders;
来源：http://kkh.zhaomingkeji.xyz

[Q08] 创建普通索引
来源：http://gre.bbcook.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://csf.cashguo.top

[Q09] 创建唯一索引
来源：http://vid.sjlbkw.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wpk.bjfxy.top

[Q10] 插入单行
来源：http://kqv.fengsongda.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ylt.yj202588.top

[Q11] 一次插入多行
来源：http://zul.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://buq.birdmap.top

[Q12] 插入后取自增 ID
来源：http://fkm.hywenlv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://rnu.xylfe.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ksu.jinqigfzy.top

[Q13] 忽略重复插入
来源：http://xhn.tianlin.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jeu.havefunace.top

[Q14] 存在则更新（upsert）
来源：http://rpk.jqgfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wva.feifeiyinyue.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ixk.ehwqpu.com

[Q15] 查询全部
来源：http://pub.epnwcf.com

SELECT * FROM users;
来源：http://yme.vqdsnc.cn

[Q16] 查询指定列
来源：http://tpd.yangfankeji.com

SELECT id, name FROM users;
来源：http://oxw.dianchejie.cn

[Q17] 条件查询
来源：http://dzm.ywan-chungtsiang.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://chj.jinghuilouyu.cn

[Q18] 模糊匹配
来源：http://buf.cqqwz.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xnq.zhongyouzk.top

[Q19] 范围查询
来源：http://zia.xinyue.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://psn.bbcook.cn

[Q20] IN 列表
来源：http://hvo.sufxvd.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uja.yvedp.cn

[Q21] 空值判断
来源：http://rwl.bbcook.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qfi.hysaishi.cn

[Q22] 排序
来源：http://tlc.cdnleiting.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xca.hongshengwenyu.top

[Q23] 分页
来源：http://ptg.quarkkingdee.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://und.chenlongwang.top

[Q24] 去重
来源：http://msj.yj20258888.top

SELECT DISTINCT city FROM users;
来源：http://zre.xylfe.cn

[Q25] 只取前 N 条
来源：http://wku.daxiang520.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vfs.jqgufenzy.top

[Q26] 计数
来源：http://bpx.feifeiyinyue.top

SELECT COUNT(*) FROM users;
来源：http://xsy.shangyingyoupin.top

[Q27] 条件计数
来源：http://dgn.hysaishi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nlx.xinyue.icu

[Q28] 求和与平均
来源：http://cgz.havefunace.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rmj.havefunace.top

[Q29] 最大最小值
来源：http://qrt.jqgufenzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://uuk.zhixingplan.top

[Q30] 分组统计
来源：http://tie.gaohongyu789.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://iye.yj20258888.top

[Q31] 分组后过滤
来源：http://twx.feifeiyinyue.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ymx.zhijiandao.cn

[Q32] 分组拼接字符串
来源：http://fft.jqgfzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wpc.sufxvd.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dwd.daxiang520.top

[Q33] 多列分组
来源：http://wzm.tanke756.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://buv.yj20258.top

[Q34] 每组取第一条
来源：http://gac.sjlbkw.cn

SELECT * FROM (
来源：http://rea.gaohongyu789.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ugv.hcnkem.com

) t WHERE rn = 1;
来源：http://ber.daria6918.cn

[Q35] 内连接
来源：http://phh.meibo888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xli.yj20258.top

[Q36] 左连接
来源：http://gvn.jyoumei.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kcl.guannengcc.top

[Q37] 右连接
来源：http://ips.fanxiaobao.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://krv.zycfv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ryt.pycfn.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wtj.birdmap.top

[Q39] 自连接（查上下级）
来源：http://yet.cdnleiting.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://nce.zhiwuduotai.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sxs.shanyushiyangkeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xfh.daxiang520.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://txa.ehwqpu.com

[Q41] 多表连接
来源：http://wpv.sxryk.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ejk.yfazqb.com

JOIN users u ON u.id = o.user_id
来源：http://pcg.sxryk.cn

JOIN products p ON p.id = o.product_id;
来源：http://ekk.hfpthk.cn

[Q42] 连接条件附加过滤
来源：http://phy.yanxiufei.cn

SELECT u.name, o.amount FROM users u
来源：http://zzt.sxryk.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gko.hysaishi.cn

[Q43] 标量子查询
来源：http://uti.yongpay.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://phq.iojbl.cn

[Q44] IN 子查询
来源：http://pvf.yangfankeji.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ljv.yj202588.top

[Q45] EXISTS 判断存在
来源：http://ptr.9152youxi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bto.jiagoushi.top

[Q46] NOT EXISTS 判断不存在
来源：http://upy.nanxuanxn.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hqb.daria6918.cn

[Q47] 与平均值比较
来源：http://imn.fengsongda.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vwt.shanyushiyangtech.top

[Q48] CTE 公用表表达式
来源：http://gln.birdmap.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dfw.hcnkem.com

SELECT * FROM t WHERE c > 5;
来源：http://mwb.hnxiangtu.top

[Q49] 更新单行
来源：http://mqv.daria6918.cn


<!-- 参考信息 -->