代发 wailian999

Py:   itertools.permutations(arr)
来源：http://nic.zhiwuduotai.top

PHP:  // 手写递归交换
来源：http://xru.jlsjyb.cn

JS:   // 手写回溯递归
来源：http://nda.hysaishi.cn

TS:   // 手写回溯递归
来源：http://tye.meibo888.top

Java: // 手写回溯递归
来源：http://yre.jiagoushi.top

Go:   // 手写回溯递归
来源：http://mnw.jianghu66.top

Ruby: arr.permutation.to_a
来源：http://rsy.chenlongwang.top

C#:   // 手写回溯递归
来源：http://chp.pycfn.com

[N09] 栈与队列
来源：http://iik.zhiwuduotai.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ovt.mhx1999.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zji.svipenyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pyu.daria6918.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vdy.fzhhl.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://too.hfpthk.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ymp.yuxming.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wzi.jqgufenzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hle.yuanzhike.top

[N10] 链表节点定义
来源：http://dgx.jianghu66.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ckd.fanxiaobao.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://ubc.sweek.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zlf.9152youxi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://orm.wangshuangyany.cn

Java: class Node { int v; Node next; }
来源：http://itu.jlsjyb.cn

Go:   type Node struct { V int; Next *Node }
来源：http://kiy.quarkkingdee.top

Ruby: Node = Struct.new(:v, :next)
来源：http://cga.daxiang520.top

C#:   class Node { public int V; public Node? Next; }
来源：http://iua.316326.xyz

[N11] 二叉树中序遍历
来源：http://jlf.tarul.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mmb.ehwqpu.com

PHP:  // 手写递归函数
来源：http://upz.sjlbkw.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zml.yongpay.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ozi.zycfv.cn

Java: // 手写递归
来源：http://zjj.quarkkingdee.top

Go:   // 手写递归
来源：http://zdh.yangfankeji.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xue.aibaodan.cn

C#:   // 手写递归
来源：http://bhk.hywenlv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dyz.gotoacloud.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lci.shanyushiyangtech.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gtc.chenlongwang.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://teq.yanxiufei.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pyc.nanxuanxn.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qwv.birdmap.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vbw.mhx1999.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://smj.haohaochexian.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tki.wangshuangyany.cn

================================================================================
来源：http://tac.yongpay.top

O. 并发与异步
来源：http://zih.jiagoushi.top

================================================================================
来源：http://lqg.yuxming.cn

[O01] 启动一个线程
来源：http://xfu.fehbvm.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://iwr.xylfe.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cqq.zhijiandao.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sne.havefunace.top

TS:   // 同 JS
来源：http://eqb.tarul.cn

Java: new Thread(() -> f()).start()
来源：http://agu.nanxinkj.top

Go:   go f()
来源：http://nyv.wangshuangyany.cn

Ruby: Thread.new { f }
来源：http://rqe.hnxiangtu.top

C#:   Task.Run(() => F());
来源：http://npm.pengpengdd.cyou

[O02] 使用线程池
来源：http://vmu.jinyuanbaomall.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qrc.dianchejie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://byv.yfazqb.com

JS:   // worker_threads 线程池
来源：http://sbh.xylfe.cn

TS:   // worker_threads 线程池
来源：http://kgw.shanyushiyangkeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://xkq.xuetiantiany.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pae.haohaochexian.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hqh.gaohongyu789.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yyp.yj202588.top

[O03] 加锁保护共享数据
来源：http://blf.tanke756.top

Py:   with lock: shared += 1
来源：http://zek.wangshuangyany.cn

PHP:  // 用 flock() 做文件锁
来源：http://bie.cdnleiting.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jrj.yangfankeji.com

TS:   // 同 JS
来源：http://hid.ydzc1.top

Java: synchronized (this) { shared++; }
来源：http://egu.wangdashe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pwz.fktsv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cbx.yvedp.cn

C#:   lock (gate) { shared++; }
来源：http://hue.zhoulong.xyz

[O04] 定义异步函数并等待
来源：http://yqq.yongpay.top

Py:   async def f():⏎    await g()
来源：http://yvu.cqqwz.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cxd.tanke756.top

JS:   async function f() { await g(); }
来源：http://mnk.sufxvd.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://sdh.zhongyouzk.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://svu.shanyushiyangtech.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wan.yvedp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://omt.fehbvm.com

C#:   async Task F() { await G(); }
来源：http://qwk.zhaomingkeji.xyz

[O05] 并发执行并等待全部完成
来源：http://cij.sxryk.cn

Py:   asyncio.gather(*tasks)
来源：http://ffk.ydjk.org.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tab.aizwys.cn

JS:   await Promise.all(tasks)
来源：http://mpc.havefunace.top

TS:   await Promise.all(tasks)
来源：http://lna.ydzc1.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://frk.hysaishi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gcq.vehdjk.com

Ruby: threads.map(&:join)
来源：http://ojy.cdnleiting.top

C#:   await Task.WhenAll(t1, t2)
来源：http://rop.iojbl.cn

[O06] 使用进程池
来源：http://shr.52xcode.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bbh.sxryk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cya.chenjidiqi.icu

JS:   // child_process / cluster 模块
来源：http://pjl.hysaishi.cn

TS:   // child_process / cluster 模块
来源：http://rik.ivvv.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uih.svipenyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wzf.fzhhl.top

Ruby: // fork 块
来源：http://fxv.cdnleiting.top

C#:   Parallel.For
来源：http://lls.xinyue.icu

================================================================================
来源：http://ugv.xuanzx.com

P. 常用工具函数
来源：http://umb.yonumen.top

================================================================================
来源：http://wmc.jinghuilouyu.cn

[P01] 生成 UUID
来源：http://kmx.jqgfzy.top

Py:   str(uuid.uuid4())
来源：http://ztj.tian-w.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://end.hnqzz.top

JS:   crypto.randomUUID()
来源：http://ghm.hnqzz.top

TS:   crypto.randomUUID()
来源：http://oin.vqdsnc.cn

Java: UUID.randomUUID().toString()
来源：http://tly.shzxlz.cn

Go:   // 用 github.com/google/uuid
来源：http://xvv.pycfn.com

Ruby: SecureRandom.uuid
来源：http://hwu.zhongyouzk.top

C#:   Guid.NewGuid().ToString()
来源：http://uou.jinqigfzy.top

[P02] MD5 / SHA256 摘要
来源：http://jal.fengsongda.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://npx.sweek.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://uue.yj202588.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kkp.tianlin.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gqu.316326.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pxi.shzxlz.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kaa.zhoulong.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://crc.ybcxt.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tfn.cdnleiting.top

[P03] 生成短随机字符串
来源：http://wss.jinqigufen.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xcr.dianchejie.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zln.quarkkingdee.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rdu.ybcxt.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://svw.ppjwa.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://arc.yangfankeji.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vab.aizwys.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wfo.pengpengdd.cyou

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://txv.zhoulong.xyz

[P04] 求长度
来源：http://igz.jlsjyb.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ghu.tian-w.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://okp.jinqigfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ode.c1oappe.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vwf.quarkkingdee.top

Java: list.size();  map.size();  s.length()
来源：http://pfs.c1oappe.top

Go:   len(arr);  len(m)
来源：http://xtc.gzhubu.top

Ruby: x.length;  x.size
来源：http://bcp.cashguo.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://eqq.vqdsnc.cn

[P05] 判断两个对象内容是否相等
来源：http://mhg.ppjwa.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ttt.sjlbkw.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nsh.shanyushiyangtech.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ufa.cucudq.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vrt.yonumen.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tez.zycfv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://smo.hnqzz.top

Ruby: a == b
来源：http://ddl.haohaochexian.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jfx.havefunace.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ozs.xziqi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gyl.gaohongyu789.top

PHP:  if (empty($x)) {}
来源：http://usz.xinyue.icu

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://oiz.yongpay.top

TS:   if (x == null) {}
来源：http://iis.xylfe.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nhx.c1oappe.top

Go:   if x == nil {}
来源：http://eau.ctjpmb.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lfh.9152youxi.cn

C#:   if (x is null) {}
来源：http://vey.jiagoushi.top

[P07] 防抖与节流
来源：http://hzk.316326.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jpn.fengsongda.top

PHP:  // 手写时间戳比较
来源：http://lgy.xziqi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xsv.ivvv.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://loe.guannengcc.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mql.epnwcf.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lma.jqgufenzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zvy.andypj.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zzk.bbcook.cn

[P08] 处理浮点精度问题
来源：http://wld.tianlin.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tln.sjlbkw.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nhr.dianchejie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qfp.fengsongda.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nmy.nanxuanxn.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qvr.shuidangran.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ahu.hcnkem.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://byq.guowangkeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lkc.zdqjudy.top

================================================================================
来源：http://oae.tanke756.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ugo.jiagoushi.top

================================================================================
来源：http://kdt.ctjpmb.com

[Q01] 创建表
来源：http://adx.tian-w.cn

CREATE TABLE users (
来源：http://wio.cqqwz.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://igg.bjfxy.top

name VARCHAR(50) NOT NULL,
来源：http://tcq.aizwys.cn

email VARCHAR(100) UNIQUE,
来源：http://clq.hongshengwenyu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tkl.ctjpmb.com

);
来源：http://kgx.shuidangran.top

[Q02] 创建带外键的表
来源：http://ihc.zdqjudy.top

CREATE TABLE orders (
来源：http://dml.ppjwa.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wyg.yuxming.cn

user_id INT NOT NULL,
来源：http://ehk.wangshuangyany.cn

amount DECIMAL(10, 2),
来源：http://uko.zhijiandao.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jtw.meibo888.top

);
来源：http://jaa.svipenyu.cn

[Q03] 增加列
来源：http://zuj.vehdjk.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://huh.sufxvd.cn

[Q04] 修改列类型
来源：http://dsj.fehbvm.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mqo.ivvv.top

[Q05] 重命名列
来源：http://rek.wangshuangyany.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rva.zhixingplan.top

[Q06] 删除列
来源：http://deh.hysaishi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cjk.epnwcf.com

[Q07] 删除表
来源：http://ddt.jyoumei.cn

DROP TABLE IF EXISTS orders;
来源：http://geq.sweek.top

[Q08] 创建普通索引
来源：http://msb.cdnleiting.top

CREATE INDEX idx_users_email ON users(email);
来源：http://zfm.birdmap.top

[Q09] 创建唯一索引
来源：http://zev.ybcxt.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xsq.hysaishi.cn

[Q10] 插入单行
来源：http://fqp.iojbl.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cwi.xuetiantiany.cn

[Q11] 一次插入多行
来源：http://rgx.gaohongyu789.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cfl.cashguo.top

[Q12] 插入后取自增 ID
来源：http://zlb.aibaodan.cn

INSERT INTO users (name) VALUES ('C');
来源：http://oac.zycfv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mmj.hongshengwenyu.top

[Q13] 忽略重复插入
来源：http://qgq.xinyue.icu

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ssy.yangfankeji.com

[Q14] 存在则更新（upsert）
来源：http://wia.ehwqpu.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kdn.zycfv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yqn.yuxming.cn

[Q15] 查询全部
来源：http://rnx.jinyuanbaomall.cn

SELECT * FROM users;
来源：http://ozy.feifeiyinyue.top

[Q16] 查询指定列
来源：http://ufm.hcnkem.com

SELECT id, name FROM users;
来源：http://try.yangfankeji.com

[Q17] 条件查询
来源：http://qxw.smart0.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vue.zhijiandao.cn

[Q18] 模糊匹配
来源：http://vaq.cucudq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://iey.shanyushiyangkeji.top

[Q19] 范围查询
来源：http://djf.xinyue.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mbn.sysykeji.top

[Q20] IN 列表
来源：http://udn.cashguo.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kbg.shuidangran.top

[Q21] 空值判断
来源：http://eaz.yfazqb.com

SELECT * FROM users WHERE email IS NULL;
来源：http://mla.zhixingplan.top

[Q22] 排序
来源：http://rsd.shuidangran.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yzi.gogol.net.cn

[Q23] 分页
来源：http://jir.316326.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fgg.zdqjudy.top

[Q24] 去重
来源：http://ncs.xziqi.cn

SELECT DISTINCT city FROM users;
来源：http://gkq.shangyingyoupin.top

[Q25] 只取前 N 条
来源：http://rkf.sysykeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nus.jianghu66.top

[Q26] 计数
来源：http://gen.shanyushiyangkeji.top

SELECT COUNT(*) FROM users;
来源：http://xwj.hnxiangtu.top

[Q27] 条件计数
来源：http://gzi.ctjpmb.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lhb.quarkkingdee.top

[Q28] 求和与平均
来源：http://exm.epnwcf.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mxc.redwolf501.top

[Q29] 最大最小值
来源：http://nbq.yueranfly.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://imm.fengsongda.top

[Q30] 分组统计
来源：http://nec.shuidangran.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lzv.jlsjyb.cn

[Q31] 分组后过滤
来源：http://rcr.hongshengwenyu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rmh.kuanghao11.cn

[Q32] 分组拼接字符串
来源：http://zgj.redwolf501.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wtd.ydjk.org.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fvs.zhongyouzk.top

[Q33] 多列分组
来源：http://psn.gogol.net.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rnp.zhixingplan.top

[Q34] 每组取第一条
来源：http://nlb.cdnleiting.top

SELECT * FROM (
来源：http://jer.svipenyu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dkb.shuidangran.top

) t WHERE rn = 1;
来源：http://nig.ywan-chungtsiang.top

[Q35] 内连接
来源：http://pry.birdmap.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bhz.jqgfzy.top

[Q36] 左连接
来源：http://gxe.yvedp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lid.zycfv.cn

[Q37] 右连接
来源：http://szp.jianghu66.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kcq.zdqjudy.top

[Q38] 全外连接（PostgreSQL）
来源：http://rtt.svipenyu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rug.aizwys.cn

[Q39] 自连接（查上下级）
来源：http://uax.gogol.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://agg.daxiang520.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ole.yongpay.top

[Q40] 交叉连接（笛卡尔积）
来源：http://jic.quarkkingdee.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xgl.pycfn.com

[Q41] 多表连接
来源：http://nqs.daxiang520.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://gmh.ehwqpu.com

JOIN users u ON u.id = o.user_id
来源：http://ncq.hesvh.cn

JOIN products p ON p.id = o.product_id;
来源：http://bts.zhengqikj.top

[Q42] 连接条件附加过滤
来源：http://gsr.sysykeji.top

SELECT u.name, o.amount FROM users u
来源：http://qpo.havefunace.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ses.yonumen.top

[Q43] 标量子查询
来源：http://xmi.zdqjudy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xat.zycfv.cn

[Q44] IN 子查询
来源：http://kbo.hcnkem.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ssg.shangyingyoupin.top

[Q45] EXISTS 判断存在
来源：http://ogy.ywan-chungtsiang.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lak.jyoumei.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mny.daria6918.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://isp.cucudq.cn

[Q47] 与平均值比较
来源：http://xss.yvedp.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ezo.sweek.top

[Q48] CTE 公用表表达式
来源：http://bju.yvedp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ili.yfazqb.com

SELECT * FROM t WHERE c > 5;
来源：http://kgu.fzhhl.top

[Q49] 更新单行
来源：http://nao.nwbrower.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dfr.hcnkem.com

[Q50] 批量更新
来源：http://hea.nwbrower.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zhf.cashguo.top

[Q51] 用子查询更新
来源：http://xjj.pycfn.com


<!-- 参考信息 -->