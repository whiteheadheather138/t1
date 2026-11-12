代发 wailian999

Ruby: s == s.reverse
来源：http://vwr.xingfuxueyuan.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://ens.fktsv.cn

[N07] 两数之和（返回下标）
来源：http://chp.shanyushiyangkeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rca.hnqzz.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wzo.snrcjt.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fhw.gogol.net.cn

TS:   // 手写 Map<string, number>
来源：http://ruo.quarkkingdee.top

Java: // 手写 HashMap
来源：http://sor.zdbjq.cn

Go:   // 手写 map[int]int
来源：http://axy.jinyuanbaomall.cn

Ruby: // 手写 Hash
来源：http://qbs.shanyushiyangkeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://rey.meibo888.top

[N08] 生成全排列
来源：http://uvo.daxiang520.top

Py:   itertools.permutations(arr)
来源：http://pot.jqgfzy.top

PHP:  // 手写递归交换
来源：http://cxx.tarul.cn

JS:   // 手写回溯递归
来源：http://nwo.nwbrower.top

TS:   // 手写回溯递归
来源：http://xfl.xziqi.cn

Java: // 手写回溯递归
来源：http://nxn.haohaochexian.top

Go:   // 手写回溯递归
来源：http://mfc.gaohongyu789.top

Ruby: arr.permutation.to_a
来源：http://kpw.kuanghao11.cn

C#:   // 手写回溯递归
来源：http://sxx.zhaomingkeji.xyz

[N09] 栈与队列
来源：http://czc.hnxiangtu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lup.jinqigfzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dis.c1oappe.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rpm.ydjk.org.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pol.nanxinkj.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xnd.yonumen.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://scv.aizwys.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vly.jqgufenzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dux.yuxming.cn

[N10] 链表节点定义
来源：http://ima.aizwys.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uco.yangfankeji.com

PHP:  class Node { public $v; public $next = null; }
来源：http://riq.chenjidiqi.icu

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fhd.zdbjq.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nou.zhixingplan.top

Java: class Node { int v; Node next; }
来源：http://gnm.cdnleiting.top

Go:   type Node struct { V int; Next *Node }
来源：http://esw.ydjk.org.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tjj.ehwqpu.com

C#:   class Node { public int V; public Node? Next; }
来源：http://ygd.kuanghao11.cn

[N11] 二叉树中序遍历
来源：http://qrm.nanxinkj.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zde.c1oappe.top

PHP:  // 手写递归函数
来源：http://bku.jinyuanbaomall.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cag.zhiwuduotai.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gzq.vqdsnc.cn

Java: // 手写递归
来源：http://viz.hesvh.cn

Go:   // 手写递归
来源：http://vtl.tianlin.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hel.jinqigfzy.top

C#:   // 手写递归
来源：http://gxs.vehdjk.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pcg.52xcode.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://smu.zhengqikj.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qqx.dashuyun.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yem.jqgfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fks.daria6918.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://eev.sjlbkw.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lbg.yongpay.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zva.kuanghao11.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tvv.ivvv.top

================================================================================
来源：http://sye.xziqi.cn

O. 并发与异步
来源：http://dtc.zhaomingkeji.xyz

================================================================================
来源：http://bnn.chenjidiqi.icu

[O01] 启动一个线程
来源：http://odq.fengsongda.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ypc.ehwqpu.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qgq.jinyuanbaomall.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://osp.fehbvm.com

TS:   // 同 JS
来源：http://tjd.hcnkem.com

Java: new Thread(() -> f()).start()
来源：http://tee.jiagoushi.top

Go:   go f()
来源：http://vgp.iojbl.cn

Ruby: Thread.new { f }
来源：http://axb.zdqjudy.top

C#:   Task.Run(() => F());
来源：http://wtb.jqgfzy.top

[O02] 使用线程池
来源：http://sbg.guannengcc.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fkd.sjlbkw.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://isb.zhaomingkeji.xyz

JS:   // worker_threads 线程池
来源：http://jdx.9152youxi.cn

TS:   // worker_threads 线程池
来源：http://nlm.pycfn.com

Java: Executors.newFixedThreadPool(4)
来源：http://lzr.shanyushiyangtech.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mmo.ydjk.org.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nnd.wangdashe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gsa.feifeiyinyue.top

[O03] 加锁保护共享数据
来源：http://poj.iojbl.cn

Py:   with lock: shared += 1
来源：http://tzu.nwbrower.top

PHP:  // 用 flock() 做文件锁
来源：http://umh.tarul.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hzh.nanxinkj.top

TS:   // 同 JS
来源：http://vau.aizwys.cn

Java: synchronized (this) { shared++; }
来源：http://eug.pengpengdd.cyou

Go:   mu.Lock();  defer mu.Unlock()
来源：http://occ.svipenyu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sci.nanxuanxn.top

C#:   lock (gate) { shared++; }
来源：http://ajy.guannengcc.top

[O04] 定义异步函数并等待
来源：http://tkn.daxiang520.top

Py:   async def f():⏎    await g()
来源：http://ogi.yj20258888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tuj.yuanzhike.top

JS:   async function f() { await g(); }
来源：http://knn.hfpthk.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hom.cashguo.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mem.jinyuanbaomall.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qqs.pengpengdd.cyou

Ruby: # 用 Fiber 或 async gem
来源：http://iaj.jlsjyb.cn

C#:   async Task F() { await G(); }
来源：http://mgs.yanxiufei.cn

[O05] 并发执行并等待全部完成
来源：http://yef.wangdashe.top

Py:   asyncio.gather(*tasks)
来源：http://kqb.sufxvd.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://asb.shzxlz.cn

JS:   await Promise.all(tasks)
来源：http://ymr.jqgfzy.top

TS:   await Promise.all(tasks)
来源：http://gyd.ehwqpu.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://shc.hongshengwenyu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bgu.52xcode.cn

Ruby: threads.map(&:join)
来源：http://tak.hammf.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pyx.yanxiufei.cn

[O06] 使用进程池
来源：http://ejl.jyoumei.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bfi.vqdsnc.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mei.hfpthk.cn

JS:   // child_process / cluster 模块
来源：http://rsm.yonumen.top

TS:   // child_process / cluster 模块
来源：http://jhx.jianghu66.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bxc.mhx1999.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ick.cqqwz.cn

Ruby: // fork 块
来源：http://kdq.jinqigfzy.top

C#:   Parallel.For
来源：http://gqk.hnqzz.top

================================================================================
来源：http://brp.haohaochexian.top

P. 常用工具函数
来源：http://ybs.ydjk.org.cn

================================================================================
来源：http://uon.gaohongyu789.top

[P01] 生成 UUID
来源：http://iyk.yanxiufei.cn

Py:   str(uuid.uuid4())
来源：http://oxn.sweek.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mla.xingfuxueyuan.xyz

JS:   crypto.randomUUID()
来源：http://pkd.snrcjt.cn

TS:   crypto.randomUUID()
来源：http://xje.redwolf501.top

Java: UUID.randomUUID().toString()
来源：http://cns.cqqwz.cn

Go:   // 用 github.com/google/uuid
来源：http://lpm.316326.xyz

Ruby: SecureRandom.uuid
来源：http://wxf.pengpengdd.cyou

C#:   Guid.NewGuid().ToString()
来源：http://ubw.shuidangran.top

[P02] MD5 / SHA256 摘要
来源：http://sls.xylfe.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cow.ydzc1.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://djs.yj20258888.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://iun.cucudq.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nll.tanke756.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mrq.jlsjyb.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vci.hcnkem.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jli.yanxiufei.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sxe.shanyushiyangtech.top

[P03] 生成短随机字符串
来源：http://odk.yfazqb.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ddo.chenlongwang.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wxb.hongshengwenyu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hya.yfazqb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bwd.zhaomingkeji.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bbm.fengsongda.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://eak.xuanzx.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://cdf.wangshuangyany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kzt.shuidangran.top

[P04] 求长度
来源：http://kcd.bjfxy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sbe.cheryme.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jzu.hfpthk.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://isw.shanyushiyangkeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qth.cashguo.top

Java: list.size();  map.size();  s.length()
来源：http://jvf.epnwcf.com

Go:   len(arr);  len(m)
来源：http://gyz.yj20258.top

Ruby: x.length;  x.size
来源：http://dax.xuetiantiany.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://nxq.sweek.top

[P05] 判断两个对象内容是否相等
来源：http://sou.yanxiufei.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qhe.tian-w.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ssl.redwolf501.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zdt.zdqjudy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tzw.sufxvd.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hla.nanxinkj.top

Go:   reflect.DeepEqual(a, b)
来源：http://thf.snrcjt.cn

Ruby: a == b
来源：http://qan.ivvv.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uny.hnqzz.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rce.9152youxi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ufc.svipenyu.cn

PHP:  if (empty($x)) {}
来源：http://rat.vqdsnc.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tmn.316326.xyz

TS:   if (x == null) {}
来源：http://ipe.feifeiyinyue.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wjf.jyoumei.cn

Go:   if x == nil {}
来源：http://xgu.jlsjyb.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kfx.xuetiantiany.cn

C#:   if (x is null) {}
来源：http://bft.nanxinkj.top

[P07] 防抖与节流
来源：http://icu.zhiwuduotai.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yqx.jqgufenzy.top

PHP:  // 手写时间戳比较
来源：http://wbt.hesvh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jcz.yuxming.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rpc.yonumen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://doy.epnwcf.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tij.ivvv.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wyd.aibaodan.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://brm.meibo888.top

[P08] 处理浮点精度问题
来源：http://pjs.zhengqikj.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://trc.jinqigfzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ezp.vehdjk.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kas.yonumen.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zht.chenjidiqi.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hja.nwbrower.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fxm.mhx1999.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lcv.epnwcf.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cwr.yj20258.top

================================================================================
来源：http://tsj.xylfe.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dtb.jinyuanbaomall.cn

================================================================================
来源：http://bod.zhaomingkeji.xyz

[Q01] 创建表
来源：http://epc.hysaishi.cn

CREATE TABLE users (
来源：http://ilg.jinqigfzy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gxm.guannengcc.top

name VARCHAR(50) NOT NULL,
来源：http://yha.yuxming.cn

email VARCHAR(100) UNIQUE,
来源：http://tfi.ivvv.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ire.shuidangran.top

);
来源：http://jsi.redwolf501.top

[Q02] 创建带外键的表
来源：http://ejz.ydjk.org.cn

CREATE TABLE orders (
来源：http://htp.yvedp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fvx.daria6918.cn

user_id INT NOT NULL,
来源：http://wdb.ppjwa.cn

amount DECIMAL(10, 2),
来源：http://onl.vqdsnc.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kqq.zhixingplan.top

);
来源：http://bvt.yvedp.cn

[Q03] 增加列
来源：http://taf.havefunace.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zes.hesvh.cn

[Q04] 修改列类型
来源：http://wdp.yonumen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bua.epnwcf.com

[Q05] 重命名列
来源：http://aqv.316326.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jwf.fengsongda.top

[Q06] 删除列
来源：http://mdi.jlsjyb.cn

ALTER TABLE users DROP COLUMN age;
来源：http://arl.ivvv.top

[Q07] 删除表
来源：http://zlo.xuetiantiany.cn

DROP TABLE IF EXISTS orders;
来源：http://upp.yuanzhike.top

[Q08] 创建普通索引
来源：http://wms.0kj1m.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://clf.gzhubu.top

[Q09] 创建唯一索引
来源：http://esb.bbcook.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uxh.gzhubu.top

[Q10] 插入单行
来源：http://bun.tarul.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xlw.hywenlv.cn

[Q11] 一次插入多行
来源：http://qjz.andypj.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fqe.jqgfzy.top

[Q12] 插入后取自增 ID
来源：http://szp.aibaodan.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ess.fanxiaobao.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://goa.cqqwz.cn

[Q13] 忽略重复插入
来源：http://tiq.ybcxt.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jdy.guowangkeji.top

[Q14] 存在则更新（upsert）
来源：http://dtf.fengsongda.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nqf.ehwqpu.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ufu.daxiang520.top

[Q15] 查询全部
来源：http://ebr.andypj.xyz

SELECT * FROM users;
来源：http://njz.cucudq.cn

[Q16] 查询指定列
来源：http://jvm.andypj.xyz

SELECT id, name FROM users;
来源：http://jvr.haohaochexian.top

[Q17] 条件查询
来源：http://tix.tanke756.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gbv.fanxiaobao.xyz

[Q18] 模糊匹配
来源：http://fka.birdmap.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bos.hysaishi.cn

[Q19] 范围查询
来源：http://gij.feifeiyinyue.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://udl.ydzc1.top

[Q20] IN 列表
来源：http://uex.sysykeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iom.xylfe.cn

[Q21] 空值判断
来源：http://ngg.sxryk.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kft.fktsv.cn

[Q22] 排序
来源：http://aaf.sweek.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://leh.yongpay.top

[Q23] 分页
来源：http://fba.ehwqpu.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cou.pengpengdd.cyou

[Q24] 去重
来源：http://sgk.gotoacloud.top

SELECT DISTINCT city FROM users;
来源：http://jdo.daria6918.cn

[Q25] 只取前 N 条
来源：http://dxa.jqgufenzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://stb.epnwcf.com

[Q26] 计数
来源：http://ecq.ppjwa.cn

SELECT COUNT(*) FROM users;
来源：http://oeg.9152youxi.cn

[Q27] 条件计数
来源：http://ssz.chenlongwang.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ebf.hywenlv.cn

[Q28] 求和与平均
来源：http://knr.zhengqikj.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nol.zhixingplan.top

[Q29] 最大最小值
来源：http://pvo.yueranfly.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://rut.guannengcc.top

[Q30] 分组统计
来源：http://our.iojbl.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rqn.zhaomingkeji.xyz

[Q31] 分组后过滤
来源：http://obm.fengsongda.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mtc.chenjidiqi.icu

[Q32] 分组拼接字符串
来源：http://yhn.jqgufenzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dsg.vehdjk.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rhd.wangdashe.top

[Q33] 多列分组
来源：http://aqv.jqgfzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://noi.sxryk.cn

[Q34] 每组取第一条
来源：http://kuj.yuanzhike.top

SELECT * FROM (
来源：http://zzp.yj20258888.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jsp.fktsv.cn

) t WHERE rn = 1;
来源：http://qqz.kuanghao11.cn

[Q35] 内连接
来源：http://dod.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://elk.daxiang520.top

[Q36] 左连接
来源：http://mwb.chenlongwang.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://syk.zycfv.cn

[Q37] 右连接
来源：http://mev.fktsv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fyt.zdqjudy.top

[Q38] 全外连接（PostgreSQL）
来源：http://gxx.sufxvd.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mfg.cashguo.top

[Q39] 自连接（查上下级）
来源：http://hyl.yangfankeji.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://xuj.quarkkingdee.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gus.aibaodan.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://abk.havefunace.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ein.hnxiangtu.top

[Q41] 多表连接
来源：http://qez.xuetiantiany.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://twi.andypj.xyz

JOIN users u ON u.id = o.user_id
来源：http://lfu.daxiang520.top

JOIN products p ON p.id = o.product_id;
来源：http://kzg.zhengqikj.top

[Q42] 连接条件附加过滤
来源：http://ylz.pengpengdd.cyou

SELECT u.name, o.amount FROM users u
来源：http://gee.dianchejie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qjd.shuidangran.top

[Q43] 标量子查询
来源：http://mip.pycfn.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mef.zdbjq.cn

[Q44] IN 子查询
来源：http://sls.bjfxy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wgq.yuxming.cn

[Q45] EXISTS 判断存在
来源：http://cdt.c1oappe.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gei.316326.xyz


<!-- 参考信息 -->