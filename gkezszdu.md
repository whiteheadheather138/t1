代发 wailian999

Go:   // 手写 map[int]int
来源：http://ddh.wangshuangyany.cn

Ruby: // 手写 Hash
来源：http://lod.bbcook.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vko.xziqi.cn

[N08] 生成全排列
来源：http://ukt.iojbl.cn

Py:   itertools.permutations(arr)
来源：http://psw.chenlongwang.top

PHP:  // 手写递归交换
来源：http://xcl.yj202588.top

JS:   // 手写回溯递归
来源：http://frf.hesvh.cn

TS:   // 手写回溯递归
来源：http://lky.hnqzz.top

Java: // 手写回溯递归
来源：http://fgf.tarul.cn

Go:   // 手写回溯递归
来源：http://ecm.wangdashe.top

Ruby: arr.permutation.to_a
来源：http://vkh.yongpay.top

C#:   // 手写回溯递归
来源：http://spt.sxryk.cn

[N09] 栈与队列
来源：http://tam.yfazqb.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fea.zhixingplan.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vsq.9152youxi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hqw.ehwqpu.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rnt.fehbvm.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://seb.yfazqb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jix.yvedp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://whi.shanyushiyangkeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://frh.yanxiufei.cn

[N10] 链表节点定义
来源：http://yrf.jinqigfzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qps.redwolf501.top

PHP:  class Node { public $v; public $next = null; }
来源：http://led.pycfn.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://flz.nwbrower.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nxb.aibaodan.cn

Java: class Node { int v; Node next; }
来源：http://byu.tanke756.top

Go:   type Node struct { V int; Next *Node }
来源：http://cjn.jyoumei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hng.aibaodan.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nae.fengsongda.top

[N11] 二叉树中序遍历
来源：http://emw.xingfuxueyuan.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yil.jiagoushi.top

PHP:  // 手写递归函数
来源：http://uvd.gogol.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rlm.redwolf501.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xkp.zhixingplan.top

Java: // 手写递归
来源：http://zvv.jinqigufen.top

Go:   // 手写递归
来源：http://vyn.fengsongda.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://huz.sxryk.cn

C#:   // 手写递归
来源：http://lhi.sweek.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rjm.ivvv.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nob.dianchejie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bwl.vqdsnc.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dwa.bjfxy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ozu.hammf.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lqr.shanyushiyangtech.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bbg.aibaodan.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bne.nanxuanxn.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oiy.tian-w.cn

================================================================================
来源：http://uwz.zhijiandao.cn

O. 并发与异步
来源：http://ies.sufxvd.cn

================================================================================
来源：http://lvc.yj20258.top

[O01] 启动一个线程
来源：http://rbj.gaohongyu789.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xok.yj20258888.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ttk.zhijiandao.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ikk.xingfuxueyuan.xyz

TS:   // 同 JS
来源：http://dxc.yj20258888.top

Java: new Thread(() -> f()).start()
来源：http://yug.zhongyouzk.top

Go:   go f()
来源：http://ouj.chenjidiqi.icu

Ruby: Thread.new { f }
来源：http://ddu.aibaodan.cn

C#:   Task.Run(() => F());
来源：http://mhj.hammf.cn

[O02] 使用线程池
来源：http://cmd.gogol.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vwr.mhx1999.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://myi.zhoulong.xyz

JS:   // worker_threads 线程池
来源：http://ubd.9152youxi.cn

TS:   // worker_threads 线程池
来源：http://xjj.birdmap.top

Java: Executors.newFixedThreadPool(4)
来源：http://xyo.birdmap.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ubu.nanxuanxn.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qef.cucudq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vfn.shanyushiyangkeji.top

[O03] 加锁保护共享数据
来源：http://hsm.fktsv.cn

Py:   with lock: shared += 1
来源：http://fps.cheryme.top

PHP:  // 用 flock() 做文件锁
来源：http://gwn.0kj1m.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pfz.tianlin.xyz

TS:   // 同 JS
来源：http://vsk.daxiang520.top

Java: synchronized (this) { shared++; }
来源：http://puh.yj20258888.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://abo.zdbjq.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://dil.dashuyun.cn

C#:   lock (gate) { shared++; }
来源：http://ups.pycfn.com

[O04] 定义异步函数并等待
来源：http://nna.gzhubu.top

Py:   async def f():⏎    await g()
来源：http://tlf.zhiwuduotai.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bju.dashuyun.cn

JS:   async function f() { await g(); }
来源：http://eyj.c1oappe.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ddy.jqgufenzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xst.sjlbkw.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mrf.cheryme.top

Ruby: # 用 Fiber 或 async gem
来源：http://ucl.0kj1m.cn

C#:   async Task F() { await G(); }
来源：http://uah.hnqzz.top

[O05] 并发执行并等待全部完成
来源：http://wsw.tianlin.xyz

Py:   asyncio.gather(*tasks)
来源：http://kko.hfpthk.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xaw.jyoumei.cn

JS:   await Promise.all(tasks)
来源：http://efl.epnwcf.com

TS:   await Promise.all(tasks)
来源：http://vxp.pengpengdd.cyou

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yax.jiagoushi.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dge.hnxiangtu.top

Ruby: threads.map(&:join)
来源：http://klf.nwbrower.top

C#:   await Task.WhenAll(t1, t2)
来源：http://czr.gzhubu.top

[O06] 使用进程池
来源：http://mjv.nwbrower.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lyy.svipenyu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hgm.chenjidiqi.icu

JS:   // child_process / cluster 模块
来源：http://pkq.shanyushiyangkeji.top

TS:   // child_process / cluster 模块
来源：http://fpc.hnxiangtu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lya.hcnkem.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sqr.hysaishi.cn

Ruby: // fork 块
来源：http://mod.fengsongda.top

C#:   Parallel.For
来源：http://wej.hnqzz.top

================================================================================
来源：http://jtd.uphjek.com

P. 常用工具函数
来源：http://lyk.wangshuangyany.cn

================================================================================
来源：http://wpl.nanxuanxn.top

[P01] 生成 UUID
来源：http://fqo.pengpengdd.cyou

Py:   str(uuid.uuid4())
来源：http://uhx.xuetiantiany.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nkc.haohaochexian.top

JS:   crypto.randomUUID()
来源：http://pwi.iojbl.cn

TS:   crypto.randomUUID()
来源：http://aqs.mhx1999.top

Java: UUID.randomUUID().toString()
来源：http://igo.sweek.top

Go:   // 用 github.com/google/uuid
来源：http://qal.tianlin.xyz

Ruby: SecureRandom.uuid
来源：http://uop.bbcook.cn

C#:   Guid.NewGuid().ToString()
来源：http://sfp.tanke756.top

[P02] MD5 / SHA256 摘要
来源：http://pnn.hfpthk.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gzw.gotoacloud.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://yul.daxiang520.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lhg.52xcode.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ymf.hesvh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wyk.jlsjyb.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yyp.jianghu66.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oig.snrcjt.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://itw.chenjidiqi.icu

[P03] 生成短随机字符串
来源：http://nsg.chenzaomai.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jng.chenzaomai.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qiw.jianghu66.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lju.hammf.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tur.cucudq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kli.guowangkeji.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zjh.cdnleiting.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://hyx.zdbjq.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://anm.yangfankeji.com

[P04] 求长度
来源：http://kxs.dashuyun.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jfk.sweek.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://buh.gotoacloud.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nhk.yj20258888.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eqx.cheryme.top

Java: list.size();  map.size();  s.length()
来源：http://hhq.xziqi.cn

Go:   len(arr);  len(m)
来源：http://gfk.sufxvd.cn

Ruby: x.length;  x.size
来源：http://zwi.zhaomingkeji.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://zfr.yj20258.top

[P05] 判断两个对象内容是否相等
来源：http://roq.nwbrower.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://duo.ivvv.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zqy.xinyue.icu

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cqj.hfpthk.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xwy.bbcook.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zee.cucudq.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pyn.wangshuangyany.cn

Ruby: a == b
来源：http://ftx.jlsjyb.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tnw.hnqzz.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cbb.shanyushiyangkeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mup.birdmap.top

PHP:  if (empty($x)) {}
来源：http://rvo.shanyushiyangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hkq.gotoacloud.top

TS:   if (x == null) {}
来源：http://rwb.nwbrower.top

Java: if (x == null || x.isEmpty()) {}
来源：http://iqb.jqgfzy.top

Go:   if x == nil {}
来源：http://zxb.sweek.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zwo.snrcjt.cn

C#:   if (x is null) {}
来源：http://eeo.dashuyun.cn

[P07] 防抖与节流
来源：http://ujt.yfazqb.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cgq.yj20258888.top

PHP:  // 手写时间戳比较
来源：http://rhg.haohaochexian.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mby.hysaishi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://erf.hesvh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gem.jqgfzy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ufj.haohaochexian.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zfx.tianlin.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://raw.0kj1m.cn

[P08] 处理浮点精度问题
来源：http://azi.yvedp.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qsy.gaohongyu789.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ado.havefunace.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jfe.gogol.net.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jnj.jinqigufen.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zkp.xylfe.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kwn.kuanghao11.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lsc.zycfv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yhs.yanxiufei.cn

================================================================================
来源：http://jvq.wangdashe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sjz.gotoacloud.top

================================================================================
来源：http://kxt.ydzc1.top

[Q01] 创建表
来源：http://nyy.ydjk.org.cn

CREATE TABLE users (
来源：http://mtp.uphjek.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rwq.zhiwuduotai.top

name VARCHAR(50) NOT NULL,
来源：http://wpx.yj20258888.top

email VARCHAR(100) UNIQUE,
来源：http://yio.xuanzx.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pec.zhiwuduotai.top

);
来源：http://hvo.hongshengwenyu.top

[Q02] 创建带外键的表
来源：http://qmh.9152youxi.cn

CREATE TABLE orders (
来源：http://nnk.jlsjyb.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jno.ydjk.org.cn

user_id INT NOT NULL,
来源：http://luq.jianghu66.top

amount DECIMAL(10, 2),
来源：http://pyy.yueranfly.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lma.316326.xyz

);
来源：http://gtb.fzhhl.top

[Q03] 增加列
来源：http://pmg.tian-w.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://oxk.yvedp.cn

[Q04] 修改列类型
来源：http://kxa.daria6918.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pqo.fanxiaobao.xyz

[Q05] 重命名列
来源：http://fqj.guowangkeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://krv.zhijiandao.cn

[Q06] 删除列
来源：http://rai.xuanzx.com

ALTER TABLE users DROP COLUMN age;
来源：http://ash.vqdsnc.cn

[Q07] 删除表
来源：http://fjc.xylfe.cn

DROP TABLE IF EXISTS orders;
来源：http://yjo.shangyingyoupin.top

[Q08] 创建普通索引
来源：http://gfn.yanxiufei.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pdy.kuanghao11.cn

[Q09] 创建唯一索引
来源：http://gke.ybcxt.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ifc.hywenlv.cn

[Q10] 插入单行
来源：http://zqd.pengpengdd.cyou

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ebf.jlsjyb.cn

[Q11] 一次插入多行
来源：http://rga.yueranfly.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://evm.vehdjk.com

[Q12] 插入后取自增 ID
来源：http://smr.yongpay.top

INSERT INTO users (name) VALUES ('C');
来源：http://fzn.zhaomingkeji.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bwq.jyoumei.cn

[Q13] 忽略重复插入
来源：http://mfg.haohaochexian.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qim.cucudq.cn

[Q14] 存在则更新（upsert）
来源：http://bay.yongpay.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qlf.quarkkingdee.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hbe.ctjpmb.com

[Q15] 查询全部
来源：http://nff.jinyuanbaomall.cn

SELECT * FROM users;
来源：http://kft.svipenyu.cn

[Q16] 查询指定列
来源：http://orp.yuxming.cn

SELECT id, name FROM users;
来源：http://pac.jinghuilouyu.cn

[Q17] 条件查询
来源：http://ohq.tianlin.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xro.gzhubu.top

[Q18] 模糊匹配
来源：http://wli.ppjwa.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kwc.tarul.cn

[Q19] 范围查询
来源：http://poa.xziqi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qiy.gogol.net.cn

[Q20] IN 列表
来源：http://gft.fzhhl.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wjr.shzxlz.cn

[Q21] 空值判断
来源：http://qih.yuxming.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pck.xylfe.cn

[Q22] 排序
来源：http://cpl.fktsv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qwd.cashguo.top

[Q23] 分页
来源：http://ydd.iojbl.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://byy.zhaomingkeji.xyz

[Q24] 去重
来源：http://dnk.xingfuxueyuan.xyz

SELECT DISTINCT city FROM users;
来源：http://oru.c1oappe.top

[Q25] 只取前 N 条
来源：http://mpb.ydzc1.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kkb.fehbvm.com

[Q26] 计数
来源：http://nbp.zhijiandao.cn

SELECT COUNT(*) FROM users;
来源：http://xvm.jlsjyb.cn

[Q27] 条件计数
来源：http://ycv.fanxiaobao.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jwv.ctjpmb.com

[Q28] 求和与平均
来源：http://keh.xuetiantiany.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ynv.smart0.xyz

[Q29] 最大最小值
来源：http://hxc.hysaishi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pta.fanxiaobao.xyz

[Q30] 分组统计
来源：http://brw.jqgufenzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xuf.quarkkingdee.top

[Q31] 分组后过滤
来源：http://efj.ydzc1.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dpq.yanxiufei.cn

[Q32] 分组拼接字符串
来源：http://uqg.hammf.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zhm.havefunace.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gek.tanke756.top

[Q33] 多列分组
来源：http://bnk.ehwqpu.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kae.havefunace.top

[Q34] 每组取第一条
来源：http://asl.zhaomingkeji.xyz

SELECT * FROM (
来源：http://dyo.andypj.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mqa.pengpengdd.cyou

) t WHERE rn = 1;
来源：http://lgv.feifeiyinyue.top

[Q35] 内连接
来源：http://hvm.yfazqb.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kug.svipenyu.cn

[Q36] 左连接
来源：http://eaq.hnqzz.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rdt.yvedp.cn

[Q37] 右连接
来源：http://oob.shanyushiyangtech.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qwc.pycfn.com

[Q38] 全外连接（PostgreSQL）
来源：http://lzf.zycfv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xxq.hesvh.cn

[Q39] 自连接（查上下级）
来源：http://fwm.dashuyun.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://cnv.chenzaomai.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fpp.hongshengwenyu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://muw.sweek.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qtd.cheryme.top

[Q41] 多表连接
来源：http://kwt.guowangkeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://tkk.yangfankeji.com

JOIN users u ON u.id = o.user_id
来源：http://afi.kuanghao11.cn

JOIN products p ON p.id = o.product_id;
来源：http://hef.wangdashe.top

[Q42] 连接条件附加过滤
来源：http://nzv.yuxming.cn

SELECT u.name, o.amount FROM users u
来源：http://ikb.jyoumei.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lwy.ehwqpu.com

[Q43] 标量子查询
来源：http://zso.wangshuangyany.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vwa.cdnleiting.top

[Q44] IN 子查询
来源：http://acw.smart0.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://doe.nanxuanxn.top

[Q45] EXISTS 判断存在
来源：http://pyt.jinqigfzy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jed.tian-w.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qnq.bjfxy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ebk.yueranfly.top

[Q47] 与平均值比较
来源：http://hri.nwbrower.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uht.vehdjk.com

[Q48] CTE 公用表表达式
来源：http://ize.fengsongda.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jih.vehdjk.com

SELECT * FROM t WHERE c > 5;
来源：http://ruj.redwolf501.top

[Q49] 更新单行
来源：http://jpz.fengsongda.top


<!-- 参考信息 -->