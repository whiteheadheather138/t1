代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nrx.ctjpmb.com

JS:   // 手写 Map：map.set(v, i)
来源：http://qzp.gotoacloud.top

TS:   // 手写 Map<string, number>
来源：http://vbe.uphjek.com

Java: // 手写 HashMap
来源：http://ifs.yangfankeji.com

Go:   // 手写 map[int]int
来源：http://jth.chenzaomai.com

Ruby: // 手写 Hash
来源：http://duy.vqdsnc.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ylk.52xcode.cn

[N08] 生成全排列
来源：http://lkq.feifeiyinyue.top

Py:   itertools.permutations(arr)
来源：http://ndv.epnwcf.com

PHP:  // 手写递归交换
来源：http://zbe.vehdjk.com

JS:   // 手写回溯递归
来源：http://bkh.shangyingyoupin.top

TS:   // 手写回溯递归
来源：http://rdi.ydjk.org.cn

Java: // 手写回溯递归
来源：http://eyc.hongshengwenyu.top

Go:   // 手写回溯递归
来源：http://nkz.cashguo.top

Ruby: arr.permutation.to_a
来源：http://yoh.hongshengwenyu.top

C#:   // 手写回溯递归
来源：http://fhr.xingfuxueyuan.xyz

[N09] 栈与队列
来源：http://rfs.yuanzhike.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yke.0kj1m.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cmg.yangfankeji.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pwk.birdmap.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uks.ctjpmb.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://css.c1oappe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bgr.nwbrower.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hao.tarul.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zdv.tarul.cn

[N10] 链表节点定义
来源：http://lcd.yfazqb.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gsx.shanyushiyangtech.top

PHP:  class Node { public $v; public $next = null; }
来源：http://rxx.jyoumei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oon.zhaomingkeji.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wjv.0kj1m.cn

Java: class Node { int v; Node next; }
来源：http://eqx.zhiwuduotai.top

Go:   type Node struct { V int; Next *Node }
来源：http://ufu.jinqigfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://djd.jqgufenzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jyi.yuanzhike.top

[N11] 二叉树中序遍历
来源：http://xri.pycfn.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xxx.jyoumei.cn

PHP:  // 手写递归函数
来源：http://jjw.hesvh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vlo.iojbl.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qdl.zhoulong.xyz

Java: // 手写递归
来源：http://jpa.snrcjt.cn

Go:   // 手写递归
来源：http://cml.xylfe.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ael.tianlin.xyz

C#:   // 手写递归
来源：http://zpy.hywenlv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ttr.vehdjk.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zmi.andypj.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bus.cashguo.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://akl.yongpay.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yja.wangdashe.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xiu.zdqjudy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xva.daxiang520.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vsy.sufxvd.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uln.hcnkem.com

================================================================================
来源：http://pee.haohaochexian.top

O. 并发与异步
来源：http://aqc.hammf.cn

================================================================================
来源：http://nuu.chenlongwang.top

[O01] 启动一个线程
来源：http://bfg.jqgfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fsh.bjfxy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zkh.tanke756.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gla.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://sxa.9152youxi.cn

Java: new Thread(() -> f()).start()
来源：http://xwl.yj202588.top

Go:   go f()
来源：http://wwr.meibo888.top

Ruby: Thread.new { f }
来源：http://iiy.yfazqb.com

C#:   Task.Run(() => F());
来源：http://oyy.yj202588.top

[O02] 使用线程池
来源：http://tif.meibo888.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qhs.smart0.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wfc.ydzc1.top

JS:   // worker_threads 线程池
来源：http://wcu.feifeiyinyue.top

TS:   // worker_threads 线程池
来源：http://cfj.zhijiandao.cn

Java: Executors.newFixedThreadPool(4)
来源：http://sas.hnqzz.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hdw.andypj.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fev.yangfankeji.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://slt.ydjk.org.cn

[O03] 加锁保护共享数据
来源：http://eoz.jinyuanbaomall.cn

Py:   with lock: shared += 1
来源：http://mci.sjlbkw.cn

PHP:  // 用 flock() 做文件锁
来源：http://xbv.ybcxt.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xrj.gotoacloud.top

TS:   // 同 JS
来源：http://krm.ctjpmb.com

Java: synchronized (this) { shared++; }
来源：http://ear.bjfxy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://stb.zdqjudy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://edd.xinyue.icu

C#:   lock (gate) { shared++; }
来源：http://wlp.sxryk.cn

[O04] 定义异步函数并等待
来源：http://mpr.bjfxy.top

Py:   async def f():⏎    await g()
来源：http://lnu.fktsv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://loo.jinghuilouyu.cn

JS:   async function f() { await g(); }
来源：http://skx.shuidangran.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://upi.c1oappe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pbf.nanxuanxn.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bpi.bjfxy.top

Ruby: # 用 Fiber 或 async gem
来源：http://vwu.chenlongwang.top

C#:   async Task F() { await G(); }
来源：http://baf.dashuyun.cn

[O05] 并发执行并等待全部完成
来源：http://rlf.kuanghao11.cn

Py:   asyncio.gather(*tasks)
来源：http://bpp.0kj1m.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ugc.kuanghao11.cn

JS:   await Promise.all(tasks)
来源：http://gfu.nanxinkj.top

TS:   await Promise.all(tasks)
来源：http://raz.jianghu66.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zcv.hnxiangtu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ndo.mhx1999.top

Ruby: threads.map(&:join)
来源：http://qes.hongshengwenyu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://jra.shanyushiyangtech.top

[O06] 使用进程池
来源：http://dsf.ivvv.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ejq.cashguo.top

PHP:  // pcntl_fork 或多进程队列
来源：http://bjl.tianlin.xyz

JS:   // child_process / cluster 模块
来源：http://rjn.yueranfly.top

TS:   // child_process / cluster 模块
来源：http://dgw.mhx1999.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vjo.yanxiufei.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lod.jinyuanbaomall.cn

Ruby: // fork 块
来源：http://vix.xuanzx.com

C#:   Parallel.For
来源：http://ldc.andypj.xyz

================================================================================
来源：http://aav.smart0.xyz

P. 常用工具函数
来源：http://hxz.aibaodan.cn

================================================================================
来源：http://fcq.c1oappe.top

[P01] 生成 UUID
来源：http://rsa.jinghuilouyu.cn

Py:   str(uuid.uuid4())
来源：http://zov.zhengqikj.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ofw.quarkkingdee.top

JS:   crypto.randomUUID()
来源：http://irl.zhixingplan.top

TS:   crypto.randomUUID()
来源：http://kxj.52xcode.cn

Java: UUID.randomUUID().toString()
来源：http://bmh.andypj.xyz

Go:   // 用 github.com/google/uuid
来源：http://orw.epnwcf.com

Ruby: SecureRandom.uuid
来源：http://qdq.gzhubu.top

C#:   Guid.NewGuid().ToString()
来源：http://lnk.jlsjyb.cn

[P02] MD5 / SHA256 摘要
来源：http://qcd.yongpay.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gas.cdnleiting.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://hrr.ctjpmb.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mig.kuanghao11.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mke.yj20258888.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kyq.pengpengdd.cyou

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nwm.epnwcf.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jsx.jinghuilouyu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pgf.havefunace.top

[P03] 生成短随机字符串
来源：http://xeq.chenlongwang.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mej.fengsongda.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://imp.dianchejie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://spb.zycfv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bvk.tian-w.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vuu.iojbl.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://owi.yj202588.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rce.jinghuilouyu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zar.cdnleiting.top

[P04] 求长度
来源：http://pje.vehdjk.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://opx.yvedp.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vfv.zhoulong.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wtp.yuanzhike.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ezv.guannengcc.top

Java: list.size();  map.size();  s.length()
来源：http://icq.chenzaomai.com

Go:   len(arr);  len(m)
来源：http://irv.ehwqpu.com

Ruby: x.length;  x.size
来源：http://eht.cheryme.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://vxe.yonumen.top

[P05] 判断两个对象内容是否相等
来源：http://eww.aibaodan.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gsv.zdbjq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hsg.chenzaomai.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://anx.quarkkingdee.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://szu.meibo888.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xjg.jqgufenzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://nhd.pycfn.com

Ruby: a == b
来源：http://nhc.fehbvm.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qbz.jyoumei.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xbd.tian-w.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rcr.snrcjt.cn

PHP:  if (empty($x)) {}
来源：http://rlz.ydzc1.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tii.hysaishi.cn

TS:   if (x == null) {}
来源：http://goh.snrcjt.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vpu.sysykeji.top

Go:   if x == nil {}
来源：http://iev.jinqigfzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xfz.sweek.top

C#:   if (x is null) {}
来源：http://tat.svipenyu.cn

[P07] 防抖与节流
来源：http://qne.cucudq.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sre.hcnkem.com

PHP:  // 手写时间戳比较
来源：http://qfr.52xcode.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sch.fzhhl.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bhj.jinqigufen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kvw.daria6918.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pgf.sjlbkw.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rue.shangyingyoupin.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cbo.ybcxt.top

[P08] 处理浮点精度问题
来源：http://loc.birdmap.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qnh.jinghuilouyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qon.tarul.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vnw.jinyuanbaomall.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kox.yueranfly.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tkr.xylfe.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xgu.svipenyu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gcx.dashuyun.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wjp.fanxiaobao.xyz

================================================================================
来源：http://epp.ydjk.org.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kja.vehdjk.com

================================================================================
来源：http://aaz.jinyuanbaomall.cn

[Q01] 创建表
来源：http://whf.yvedp.cn

CREATE TABLE users (
来源：http://fjf.cucudq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qkx.shuidangran.top

name VARCHAR(50) NOT NULL,
来源：http://qmx.haohaochexian.top

email VARCHAR(100) UNIQUE,
来源：http://yxv.fanxiaobao.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oqw.ydjk.org.cn

);
来源：http://lwz.fktsv.cn

[Q02] 创建带外键的表
来源：http://cpr.zhijiandao.cn

CREATE TABLE orders (
来源：http://ozq.ivvv.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fhw.cucudq.cn

user_id INT NOT NULL,
来源：http://ehd.jiagoushi.top

amount DECIMAL(10, 2),
来源：http://kzk.yanxiufei.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hmt.zhengqikj.top

);
来源：http://tie.epnwcf.com

[Q03] 增加列
来源：http://eug.mhx1999.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kix.hcnkem.com

[Q04] 修改列类型
来源：http://yvc.zhengqikj.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xwd.wangshuangyany.cn

[Q05] 重命名列
来源：http://kne.dianchejie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qdd.bjfxy.top

[Q06] 删除列
来源：http://frt.gzhubu.top

ALTER TABLE users DROP COLUMN age;
来源：http://mkp.hesvh.cn

[Q07] 删除表
来源：http://fux.ydjk.org.cn

DROP TABLE IF EXISTS orders;
来源：http://ojp.52xcode.cn

[Q08] 创建普通索引
来源：http://fwj.jqgufenzy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jlo.guannengcc.top

[Q09] 创建唯一索引
来源：http://lso.vehdjk.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://eot.jianghu66.top

[Q10] 插入单行
来源：http://fnv.hammf.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jyp.52xcode.cn

[Q11] 一次插入多行
来源：http://gnb.ivvv.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dgh.hammf.cn

[Q12] 插入后取自增 ID
来源：http://mnl.andypj.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://fbw.nanxinkj.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://iws.havefunace.top

[Q13] 忽略重复插入
来源：http://awv.shangyingyoupin.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tmv.nanxinkj.top

[Q14] 存在则更新（upsert）
来源：http://qpt.gotoacloud.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://edp.havefunace.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://twi.fktsv.cn

[Q15] 查询全部
来源：http://yyp.zycfv.cn

SELECT * FROM users;
来源：http://fga.vqdsnc.cn

[Q16] 查询指定列
来源：http://vxv.jinghuilouyu.cn

SELECT id, name FROM users;
来源：http://pxn.redwolf501.top

[Q17] 条件查询
来源：http://hfg.xziqi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mky.zdbjq.cn

[Q18] 模糊匹配
来源：http://mor.uphjek.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://auh.guowangkeji.top

[Q19] 范围查询
来源：http://qln.yueranfly.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cmg.wangdashe.top

[Q20] IN 列表
来源：http://lzd.pycfn.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://upo.tianlin.xyz

[Q21] 空值判断
来源：http://kjn.yueranfly.top

SELECT * FROM users WHERE email IS NULL;
来源：http://cpx.xuetiantiany.cn

[Q22] 排序
来源：http://ppl.sxryk.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kuz.bjfxy.top

[Q23] 分页
来源：http://vje.pengpengdd.cyou

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fuu.bjfxy.top

[Q24] 去重
来源：http://gir.fengsongda.top

SELECT DISTINCT city FROM users;
来源：http://tyv.feifeiyinyue.top

[Q25] 只取前 N 条
来源：http://iri.shuidangran.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bbb.uphjek.com

[Q26] 计数
来源：http://goi.dashuyun.cn

SELECT COUNT(*) FROM users;
来源：http://teb.andypj.xyz

[Q27] 条件计数
来源：http://dpj.fengsongda.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ehl.aizwys.cn

[Q28] 求和与平均
来源：http://tih.hysaishi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wim.xingfuxueyuan.xyz

[Q29] 最大最小值
来源：http://ptx.hnqzz.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ggq.ybcxt.top

[Q30] 分组统计
来源：http://ttp.jinqigufen.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wrq.hongshengwenyu.top

[Q31] 分组后过滤
来源：http://zcb.zhengqikj.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bhs.fengsongda.top

[Q32] 分组拼接字符串
来源：http://uby.tarul.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xke.fzhhl.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cpo.yj20258.top

[Q33] 多列分组
来源：http://qyb.gzhubu.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qyl.316326.xyz

[Q34] 每组取第一条
来源：http://iwn.yvedp.cn

SELECT * FROM (
来源：http://nuk.dashuyun.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vqt.xylfe.cn

) t WHERE rn = 1;
来源：http://siy.zhaomingkeji.xyz

[Q35] 内连接
来源：http://xcx.hfpthk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://leq.cdnleiting.top

[Q36] 左连接
来源：http://grb.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ahd.bjfxy.top

[Q37] 右连接
来源：http://zqz.gaohongyu789.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://czn.shanyushiyangtech.top

[Q38] 全外连接（PostgreSQL）
来源：http://avd.xingfuxueyuan.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kbp.cdnleiting.top

[Q39] 自连接（查上下级）
来源：http://ikv.uphjek.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://ybj.xuetiantiany.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jwi.fengsongda.top

[Q40] 交叉连接（笛卡尔积）
来源：http://inb.haohaochexian.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hvv.nanxuanxn.top

[Q41] 多表连接
来源：http://zks.chenlongwang.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://vwe.haohaochexian.top

JOIN users u ON u.id = o.user_id
来源：http://mbt.dashuyun.cn

JOIN products p ON p.id = o.product_id;
来源：http://cly.fzhhl.top

[Q42] 连接条件附加过滤
来源：http://kli.iojbl.cn

SELECT u.name, o.amount FROM users u
来源：http://rca.ppjwa.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ide.sweek.top

[Q43] 标量子查询
来源：http://nex.yuxming.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pqq.ywan-chungtsiang.top

[Q44] IN 子查询
来源：http://aos.yueranfly.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hmr.pycfn.com

[Q45] EXISTS 判断存在
来源：http://jrt.shanyushiyangtech.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dba.xuanzx.com

[Q46] NOT EXISTS 判断不存在
来源：http://vro.ydzc1.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jea.sufxvd.cn

[Q47] 与平均值比较
来源：http://fhz.zdqjudy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vzr.guowangkeji.top


<!-- 参考信息 -->