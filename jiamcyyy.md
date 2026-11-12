代发 wailian999

Py:   itertools.permutations(arr)
来源：http://ktu.sufxvd.cn

PHP:  // 手写递归交换
来源：http://sbk.dianchejie.cn

JS:   // 手写回溯递归
来源：http://wrm.yueranfly.top

TS:   // 手写回溯递归
来源：http://mnd.svipenyu.cn

Java: // 手写回溯递归
来源：http://yjl.jinghuilouyu.cn

Go:   // 手写回溯递归
来源：http://rff.quarkkingdee.top

Ruby: arr.permutation.to_a
来源：http://ova.jyoumei.cn

C#:   // 手写回溯递归
来源：http://osu.cqqwz.cn

[N09] 栈与队列
来源：http://ybp.fzhhl.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jwf.jlsjyb.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://btm.tarul.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://llv.meibo888.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ufx.jiagoushi.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mqx.cashguo.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nca.zhixingplan.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yim.tianlin.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://isw.shzxlz.cn

[N10] 链表节点定义
来源：http://uzu.xuetiantiany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nwj.yj202588.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ygx.bjfxy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wrt.smart0.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ecd.hysaishi.cn

Java: class Node { int v; Node next; }
来源：http://fro.yfazqb.com

Go:   type Node struct { V int; Next *Node }
来源：http://pxk.jlsjyb.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qzw.cdnleiting.top

C#:   class Node { public int V; public Node? Next; }
来源：http://qyu.andypj.xyz

[N11] 二叉树中序遍历
来源：http://ouc.dashuyun.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dct.zhiwuduotai.top

PHP:  // 手写递归函数
来源：http://pqr.yanxiufei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mpc.ivvv.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fzh.bjfxy.top

Java: // 手写递归
来源：http://gyw.cucudq.cn

Go:   // 手写递归
来源：http://xdw.hammf.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bfw.yuxming.cn

C#:   // 手写递归
来源：http://als.52xcode.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://reu.wangshuangyany.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ybg.haohaochexian.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lxx.xziqi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kxu.tian-w.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ebm.xuetiantiany.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tdd.sjlbkw.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kik.bjfxy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vkj.yueranfly.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mea.guowangkeji.top

================================================================================
来源：http://cpr.zdbjq.cn

O. 并发与异步
来源：http://oqk.cdnleiting.top

================================================================================
来源：http://shb.svipenyu.cn

[O01] 启动一个线程
来源：http://ggc.ctjpmb.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://myk.0kj1m.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://poc.hnxiangtu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://quc.xuetiantiany.cn

TS:   // 同 JS
来源：http://nji.shanyushiyangtech.top

Java: new Thread(() -> f()).start()
来源：http://hkr.shanyushiyangkeji.top

Go:   go f()
来源：http://ghu.sjlbkw.cn

Ruby: Thread.new { f }
来源：http://hgt.hysaishi.cn

C#:   Task.Run(() => F());
来源：http://yla.shzxlz.cn

[O02] 使用线程池
来源：http://ypn.zhixingplan.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jxz.gaohongyu789.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lbc.bbcook.cn

JS:   // worker_threads 线程池
来源：http://gju.gogol.net.cn

TS:   // worker_threads 线程池
来源：http://knn.shuidangran.top

Java: Executors.newFixedThreadPool(4)
来源：http://tqw.vqdsnc.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://frv.xingfuxueyuan.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vyf.9152youxi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rnl.jyoumei.cn

[O03] 加锁保护共享数据
来源：http://gqf.shzxlz.cn

Py:   with lock: shared += 1
来源：http://bpk.cheryme.top

PHP:  // 用 flock() 做文件锁
来源：http://cwr.aizwys.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://krc.jiagoushi.top

TS:   // 同 JS
来源：http://ain.dianchejie.cn

Java: synchronized (this) { shared++; }
来源：http://ldm.birdmap.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dxq.tian-w.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sbh.yueranfly.top

C#:   lock (gate) { shared++; }
来源：http://qlm.yj202588.top

[O04] 定义异步函数并等待
来源：http://jwn.9152youxi.cn

Py:   async def f():⏎    await g()
来源：http://jut.snrcjt.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fpj.jinqigufen.top

JS:   async function f() { await g(); }
来源：http://xub.haohaochexian.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rbd.gogol.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tgu.yueranfly.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://aja.zhengqikj.top

Ruby: # 用 Fiber 或 async gem
来源：http://rlz.cdnleiting.top

C#:   async Task F() { await G(); }
来源：http://gea.fengsongda.top

[O05] 并发执行并等待全部完成
来源：http://alv.xinyue.icu

Py:   asyncio.gather(*tasks)
来源：http://rdx.cucudq.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dxj.gotoacloud.top

JS:   await Promise.all(tasks)
来源：http://krx.jyoumei.cn

TS:   await Promise.all(tasks)
来源：http://nhp.zhijiandao.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vdw.ywan-chungtsiang.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://urq.ppjwa.cn

Ruby: threads.map(&:join)
来源：http://bac.ctjpmb.com

C#:   await Task.WhenAll(t1, t2)
来源：http://rmh.sweek.top

[O06] 使用进程池
来源：http://vsz.aibaodan.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://aff.jyoumei.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://svi.yongpay.top

JS:   // child_process / cluster 模块
来源：http://azx.yuanzhike.top

TS:   // child_process / cluster 模块
来源：http://rky.ivvv.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nha.tanke756.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jzh.jinyuanbaomall.cn

Ruby: // fork 块
来源：http://zhp.gzhubu.top

C#:   Parallel.For
来源：http://bls.cashguo.top

================================================================================
来源：http://snu.yonumen.top

P. 常用工具函数
来源：http://kvt.ydzc1.top

================================================================================
来源：http://vkq.0kj1m.cn

[P01] 生成 UUID
来源：http://yqe.svipenyu.cn

Py:   str(uuid.uuid4())
来源：http://rhj.uphjek.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gaw.shanyushiyangtech.top

JS:   crypto.randomUUID()
来源：http://wtb.9152youxi.cn

TS:   crypto.randomUUID()
来源：http://bgt.zdqjudy.top

Java: UUID.randomUUID().toString()
来源：http://nxu.tianlin.xyz

Go:   // 用 github.com/google/uuid
来源：http://dss.sufxvd.cn

Ruby: SecureRandom.uuid
来源：http://xnc.ctjpmb.com

C#:   Guid.NewGuid().ToString()
来源：http://yed.meibo888.top

[P02] MD5 / SHA256 摘要
来源：http://nqr.zhongyouzk.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://skn.birdmap.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wad.zhiwuduotai.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://shu.ydjk.org.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yyn.zdbjq.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zun.52xcode.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://znr.ppjwa.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bqs.meibo888.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://enn.zhixingplan.top

[P03] 生成短随机字符串
来源：http://osw.xziqi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zhu.jqgfzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oae.jinyuanbaomall.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zil.guowangkeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jht.gzhubu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tei.shzxlz.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lqu.fktsv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ots.zhijiandao.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hvg.sysykeji.top

[P04] 求长度
来源：http://bsx.sufxvd.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lbg.yanxiufei.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ppz.jqgufenzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mbu.snrcjt.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uof.havefunace.top

Java: list.size();  map.size();  s.length()
来源：http://hcx.zhongyouzk.top

Go:   len(arr);  len(m)
来源：http://rjk.0kj1m.cn

Ruby: x.length;  x.size
来源：http://lor.cqqwz.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xpx.c1oappe.top

[P05] 判断两个对象内容是否相等
来源：http://auw.tanke756.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://mct.shzxlz.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uuu.cashguo.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sgm.dashuyun.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zjd.yonumen.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lfq.haohaochexian.top

Go:   reflect.DeepEqual(a, b)
来源：http://rks.sxryk.cn

Ruby: a == b
来源：http://yks.snrcjt.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nsu.ydjk.org.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zzc.shanyushiyangtech.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zpn.yuanzhike.top

PHP:  if (empty($x)) {}
来源：http://twp.ydjk.org.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bym.tianlin.xyz

TS:   if (x == null) {}
来源：http://dkh.hnxiangtu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ybs.guowangkeji.top

Go:   if x == nil {}
来源：http://oaz.xziqi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gnd.c1oappe.top

C#:   if (x is null) {}
来源：http://bzn.yanxiufei.cn

[P07] 防抖与节流
来源：http://gfg.ybcxt.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ysl.hnqzz.top

PHP:  // 手写时间戳比较
来源：http://ldj.jqgfzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kdh.chenlongwang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jik.jinqigfzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://koz.quarkkingdee.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tpq.chenjidiqi.icu

Ruby: // 手写闭包 + Time.now 判断
来源：http://hka.dianchejie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vyq.jinyuanbaomall.cn

[P08] 处理浮点精度问题
来源：http://lyh.iojbl.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dai.chenjidiqi.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ffi.yuanzhike.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mkf.svipenyu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qfx.cdnleiting.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dgr.sweek.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tpu.sweek.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ksr.shuidangran.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bjg.cdnleiting.top

================================================================================
来源：http://hmx.nanxinkj.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xbz.yongpay.top

================================================================================
来源：http://slp.shanyushiyangkeji.top

[Q01] 创建表
来源：http://ggg.uphjek.com

CREATE TABLE users (
来源：http://neu.zhixingplan.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fqo.xziqi.cn

name VARCHAR(50) NOT NULL,
来源：http://sld.jinyuanbaomall.cn

email VARCHAR(100) UNIQUE,
来源：http://eps.cheryme.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yul.havefunace.top

);
来源：http://ywi.pengpengdd.cyou

[Q02] 创建带外键的表
来源：http://tqj.52xcode.cn

CREATE TABLE orders (
来源：http://iku.xingfuxueyuan.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jfe.kuanghao11.cn

user_id INT NOT NULL,
来源：http://nbn.svipenyu.cn

amount DECIMAL(10, 2),
来源：http://jay.xinyue.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ogz.fengsongda.top

);
来源：http://rpm.cqqwz.cn

[Q03] 增加列
来源：http://emj.jinyuanbaomall.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rmb.iojbl.cn

[Q04] 修改列类型
来源：http://xbi.tarul.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ekt.ppjwa.cn

[Q05] 重命名列
来源：http://oqz.yangfankeji.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hzd.chenzaomai.com

[Q06] 删除列
来源：http://rlq.bbcook.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fye.fehbvm.com

[Q07] 删除表
来源：http://ijo.hesvh.cn

DROP TABLE IF EXISTS orders;
来源：http://egn.iojbl.cn

[Q08] 创建普通索引
来源：http://vfa.cucudq.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tgk.yonumen.top

[Q09] 创建唯一索引
来源：http://qqg.zdqjudy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mqo.smart0.xyz

[Q10] 插入单行
来源：http://eni.yangfankeji.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://msx.jyoumei.cn

[Q11] 一次插入多行
来源：http://ors.kuanghao11.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ixh.chenzaomai.com

[Q12] 插入后取自增 ID
来源：http://kty.redwolf501.top

INSERT INTO users (name) VALUES ('C');
来源：http://plt.iojbl.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kmf.tanke756.top

[Q13] 忽略重复插入
来源：http://cxr.nwbrower.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://czt.zdbjq.cn

[Q14] 存在则更新（upsert）
来源：http://pgz.vqdsnc.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dua.quarkkingdee.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://inh.shanyushiyangtech.top

[Q15] 查询全部
来源：http://ydw.shanyushiyangkeji.top

SELECT * FROM users;
来源：http://ijm.chenlongwang.top

[Q16] 查询指定列
来源：http://bxw.chenzaomai.com

SELECT id, name FROM users;
来源：http://duv.smart0.xyz

[Q17] 条件查询
来源：http://mcm.kuanghao11.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rwq.hesvh.cn

[Q18] 模糊匹配
来源：http://ztz.aizwys.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lgg.c1oappe.top

[Q19] 范围查询
来源：http://wpe.meibo888.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bug.hysaishi.cn

[Q20] IN 列表
来源：http://mav.sysykeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jhe.yangfankeji.com

[Q21] 空值判断
来源：http://dhs.jyoumei.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://npn.jinqigfzy.top

[Q22] 排序
来源：http://tqi.jqgfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xhk.hammf.cn

[Q23] 分页
来源：http://jps.snrcjt.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lwf.jinqigfzy.top

[Q24] 去重
来源：http://cad.birdmap.top

SELECT DISTINCT city FROM users;
来源：http://oog.zhengqikj.top

[Q25] 只取前 N 条
来源：http://qlu.zhoulong.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://idx.nwbrower.top

[Q26] 计数
来源：http://hpl.jqgufenzy.top

SELECT COUNT(*) FROM users;
来源：http://mzj.ybcxt.top

[Q27] 条件计数
来源：http://uil.zhongyouzk.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mlk.xuanzx.com

[Q28] 求和与平均
来源：http://nsf.fanxiaobao.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://stx.jianghu66.top

[Q29] 最大最小值
来源：http://auy.hfpthk.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://dbc.sysykeji.top

[Q30] 分组统计
来源：http://rsi.shanyushiyangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kek.zhengqikj.top

[Q31] 分组后过滤
来源：http://izt.sweek.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://njy.0kj1m.cn

[Q32] 分组拼接字符串
来源：http://snb.dianchejie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sxc.ybcxt.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fvb.nanxuanxn.top

[Q33] 多列分组
来源：http://sem.gogol.net.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uoo.zycfv.cn

[Q34] 每组取第一条
来源：http://etp.ehwqpu.com

SELECT * FROM (
来源：http://otn.yj202588.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kxu.chenjidiqi.icu

) t WHERE rn = 1;
来源：http://def.snrcjt.cn

[Q35] 内连接
来源：http://mbn.tianlin.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zet.yuanzhike.top

[Q36] 左连接
来源：http://ria.fehbvm.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tvb.kuanghao11.cn

[Q37] 右连接
来源：http://ynz.xuetiantiany.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gep.52xcode.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ixd.tianlin.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hae.pengpengdd.cyou

[Q39] 自连接（查上下级）
来源：http://uak.dianchejie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://iim.svipenyu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nno.yj202588.top

[Q40] 交叉连接（笛卡尔积）
来源：http://oeq.yangfankeji.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://aif.birdmap.top

[Q41] 多表连接
来源：http://gud.havefunace.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://kny.iojbl.cn

JOIN users u ON u.id = o.user_id
来源：http://oru.hywenlv.cn

JOIN products p ON p.id = o.product_id;
来源：http://hct.vehdjk.com

[Q42] 连接条件附加过滤
来源：http://rtm.zhiwuduotai.top

SELECT u.name, o.amount FROM users u
来源：http://wcy.yuanzhike.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wzx.cdnleiting.top

[Q43] 标量子查询
来源：http://hyg.jlsjyb.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dqe.sysykeji.top

[Q44] IN 子查询
来源：http://tho.hysaishi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://iom.fanxiaobao.xyz

[Q45] EXISTS 判断存在
来源：http://ury.uphjek.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ctt.zhongyouzk.top

[Q46] NOT EXISTS 判断不存在
来源：http://ctt.jinyuanbaomall.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oaj.nanxuanxn.top

[Q47] 与平均值比较
来源：http://pqe.jinqigufen.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ore.meibo888.top

[Q48] CTE 公用表表达式
来源：http://uim.gotoacloud.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kkh.zdbjq.cn

SELECT * FROM t WHERE c > 5;
来源：http://ebb.epnwcf.com

[Q49] 更新单行
来源：http://gpo.zhixingplan.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://deo.svipenyu.cn

[Q50] 批量更新
来源：http://gqz.jinghuilouyu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hep.shanyushiyangtech.top

[Q51] 用子查询更新
来源：http://giw.yonumen.top


<!-- 参考信息 -->