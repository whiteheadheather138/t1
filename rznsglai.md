代发 wailian999

Java: // 手写回溯递归
来源：http://pcg.snrcjt.cn

Go:   // 手写回溯递归
来源：http://grc.sysykeji.top

Ruby: arr.permutation.to_a
来源：http://igi.shangyingyoupin.top

C#:   // 手写回溯递归
来源：http://zwg.jinqigfzy.top

[N09] 栈与队列
来源：http://cms.yfazqb.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ikd.316326.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vso.sufxvd.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vrf.jiagoushi.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zcw.zhengqikj.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oeo.ehwqpu.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gqz.ctjpmb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wlz.sxryk.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cip.cucudq.cn

[N10] 链表节点定义
来源：http://rhs.haohaochexian.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://oey.quarkkingdee.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mks.316326.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qko.hesvh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xir.kuanghao11.cn

Java: class Node { int v; Node next; }
来源：http://url.hywenlv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gmq.snrcjt.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://oof.epnwcf.com

C#:   class Node { public int V; public Node? Next; }
来源：http://kog.jiagoushi.top

[N11] 二叉树中序遍历
来源：http://tfa.xylfe.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gok.xinyue.icu

PHP:  // 手写递归函数
来源：http://hko.wangshuangyany.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lax.guowangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jyi.jqgfzy.top

Java: // 手写递归
来源：http://osl.vqdsnc.cn

Go:   // 手写递归
来源：http://yqf.52xcode.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wnq.jyoumei.cn

C#:   // 手写递归
来源：http://ufk.jinqigfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xon.ctjpmb.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://egx.fanxiaobao.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://icr.sjlbkw.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://spo.zycfv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iuw.guowangkeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://enz.hywenlv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gqy.sweek.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://csq.yfazqb.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://eim.iojbl.cn

================================================================================
来源：http://qnd.daria6918.cn

O. 并发与异步
来源：http://vsy.tanke756.top

================================================================================
来源：http://wob.sxryk.cn

[O01] 启动一个线程
来源：http://gmc.sjlbkw.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://eno.ctjpmb.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fmx.haohaochexian.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fen.hnqzz.top

TS:   // 同 JS
来源：http://dvf.pycfn.com

Java: new Thread(() -> f()).start()
来源：http://npo.zhiwuduotai.top

Go:   go f()
来源：http://gwl.sufxvd.cn

Ruby: Thread.new { f }
来源：http://ldg.havefunace.top

C#:   Task.Run(() => F());
来源：http://eud.aibaodan.cn

[O02] 使用线程池
来源：http://yep.vqdsnc.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jth.tian-w.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://haz.fanxiaobao.xyz

JS:   // worker_threads 线程池
来源：http://zyk.kuanghao11.cn

TS:   // worker_threads 线程池
来源：http://doy.zdqjudy.top

Java: Executors.newFixedThreadPool(4)
来源：http://qke.cdnleiting.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hza.iojbl.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qzm.yonumen.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://inm.jyoumei.cn

[O03] 加锁保护共享数据
来源：http://qqy.cucudq.cn

Py:   with lock: shared += 1
来源：http://rwf.jinyuanbaomall.cn

PHP:  // 用 flock() 做文件锁
来源：http://kou.0kj1m.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nao.tian-w.cn

TS:   // 同 JS
来源：http://mxw.gzhubu.top

Java: synchronized (this) { shared++; }
来源：http://tkq.wangdashe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pkk.shanyushiyangtech.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://cjl.haohaochexian.top

C#:   lock (gate) { shared++; }
来源：http://zth.xingfuxueyuan.xyz

[O04] 定义异步函数并等待
来源：http://jpo.bjfxy.top

Py:   async def f():⏎    await g()
来源：http://lif.aizwys.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yre.jqgfzy.top

JS:   async function f() { await g(); }
来源：http://syu.ctjpmb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://wav.shzxlz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xte.chenjidiqi.icu

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bkk.epnwcf.com

Ruby: # 用 Fiber 或 async gem
来源：http://ssp.daxiang520.top

C#:   async Task F() { await G(); }
来源：http://mew.ydjk.org.cn

[O05] 并发执行并等待全部完成
来源：http://rgu.yanxiufei.cn

Py:   asyncio.gather(*tasks)
来源：http://fav.jqgfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gfj.gotoacloud.top

JS:   await Promise.all(tasks)
来源：http://mbp.chenlongwang.top

TS:   await Promise.all(tasks)
来源：http://gku.sufxvd.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bbw.chenlongwang.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ccb.ppjwa.cn

Ruby: threads.map(&:join)
来源：http://fmt.ybcxt.top

C#:   await Task.WhenAll(t1, t2)
来源：http://wxg.zhongyouzk.top

[O06] 使用进程池
来源：http://xqu.hammf.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://otu.aizwys.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tit.uphjek.com

JS:   // child_process / cluster 模块
来源：http://ufi.sxryk.cn

TS:   // child_process / cluster 模块
来源：http://lgf.ppjwa.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pwh.jinqigfzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oql.ydjk.org.cn

Ruby: // fork 块
来源：http://fiy.bbcook.cn

C#:   Parallel.For
来源：http://gak.zdqjudy.top

================================================================================
来源：http://tgd.ehwqpu.com

P. 常用工具函数
来源：http://cjz.zhongyouzk.top

================================================================================
来源：http://rmq.jinqigufen.top

[P01] 生成 UUID
来源：http://tvc.bjfxy.top

Py:   str(uuid.uuid4())
来源：http://jfm.tian-w.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://are.zhiwuduotai.top

JS:   crypto.randomUUID()
来源：http://rzq.tarul.cn

TS:   crypto.randomUUID()
来源：http://mky.chenzaomai.com

Java: UUID.randomUUID().toString()
来源：http://agg.ybcxt.top

Go:   // 用 github.com/google/uuid
来源：http://swo.chenzaomai.com

Ruby: SecureRandom.uuid
来源：http://cbn.sxryk.cn

C#:   Guid.NewGuid().ToString()
来源：http://ftx.kuanghao11.cn

[P02] MD5 / SHA256 摘要
来源：http://wlh.jlsjyb.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://prt.yuanzhike.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://xjo.daxiang520.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://axe.jiagoushi.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ent.snrcjt.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://obi.c1oappe.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://daw.sweek.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://scm.jqgfzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lck.yj20258.top

[P03] 生成短随机字符串
来源：http://kvw.ivvv.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://iie.hywenlv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bge.vehdjk.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eku.aibaodan.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://heq.cucudq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vit.xinyue.icu

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://obv.jlsjyb.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jtq.zdqjudy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cop.c1oappe.top

[P04] 求长度
来源：http://uqq.aizwys.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lne.hesvh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ret.hnqzz.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ibh.yueranfly.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://szy.guannengcc.top

Java: list.size();  map.size();  s.length()
来源：http://vni.xuanzx.com

Go:   len(arr);  len(m)
来源：http://wfp.meibo888.top

Ruby: x.length;  x.size
来源：http://kaz.jianghu66.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://aft.ywan-chungtsiang.top

[P05] 判断两个对象内容是否相等
来源：http://wvy.yueranfly.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://geg.shuidangran.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ajk.shangyingyoupin.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sql.feifeiyinyue.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qpy.fengsongda.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rgd.iojbl.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jpr.zhengqikj.top

Ruby: a == b
来源：http://xvo.yfazqb.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lqq.zhiwuduotai.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://drr.dianchejie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yzo.ivvv.top

PHP:  if (empty($x)) {}
来源：http://dcc.ehwqpu.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blz.birdmap.top

TS:   if (x == null) {}
来源：http://zox.daria6918.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fxo.yueranfly.top

Go:   if x == nil {}
来源：http://fcv.yfazqb.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hto.xziqi.cn

C#:   if (x is null) {}
来源：http://yrr.bjfxy.top

[P07] 防抖与节流
来源：http://oql.xylfe.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://viu.xuanzx.com

PHP:  // 手写时间戳比较
来源：http://lzl.316326.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eaz.daxiang520.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tqh.xinyue.icu

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sqx.vqdsnc.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xzg.shuidangran.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://cke.chenzaomai.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gag.yj202588.top

[P08] 处理浮点精度问题
来源：http://jib.zhengqikj.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dif.jqgfzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gjy.xuanzx.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pzi.cashguo.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://meo.yj202588.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wkk.tarul.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://amf.jiagoushi.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ukq.jqgfzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jaw.xylfe.cn

================================================================================
来源：http://fdy.tianlin.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lrj.hnxiangtu.top

================================================================================
来源：http://aee.hcnkem.com

[Q01] 创建表
来源：http://lmf.shangyingyoupin.top

CREATE TABLE users (
来源：http://oat.cdnleiting.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://onm.yfazqb.com

name VARCHAR(50) NOT NULL,
来源：http://ytf.wangdashe.top

email VARCHAR(100) UNIQUE,
来源：http://qrr.yanxiufei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://quu.zhengqikj.top

);
来源：http://nfz.shangyingyoupin.top

[Q02] 创建带外键的表
来源：http://mem.epnwcf.com

CREATE TABLE orders (
来源：http://iux.zhengqikj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yeh.yvedp.cn

user_id INT NOT NULL,
来源：http://jdd.xuetiantiany.cn

amount DECIMAL(10, 2),
来源：http://dzw.xylfe.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://irn.zhaomingkeji.xyz

);
来源：http://cov.yangfankeji.com

[Q03] 增加列
来源：http://mus.daxiang520.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gsj.dashuyun.cn

[Q04] 修改列类型
来源：http://dms.yj202588.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ycz.yonumen.top

[Q05] 重命名列
来源：http://rcm.svipenyu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xqh.yueranfly.top

[Q06] 删除列
来源：http://pdg.fengsongda.top

ALTER TABLE users DROP COLUMN age;
来源：http://zvk.hfpthk.cn

[Q07] 删除表
来源：http://jbw.hnqzz.top

DROP TABLE IF EXISTS orders;
来源：http://mva.jinqigfzy.top

[Q08] 创建普通索引
来源：http://mod.bbcook.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://cvd.hcnkem.com

[Q09] 创建唯一索引
来源：http://poe.guowangkeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xwc.wangdashe.top

[Q10] 插入单行
来源：http://rji.jinqigfzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bjf.feifeiyinyue.top

[Q11] 一次插入多行
来源：http://cst.jqgfzy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cwb.gaohongyu789.top

[Q12] 插入后取自增 ID
来源：http://slu.cashguo.top

INSERT INTO users (name) VALUES ('C');
来源：http://oja.xingfuxueyuan.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jpi.nanxuanxn.top

[Q13] 忽略重复插入
来源：http://zvd.ehwqpu.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qyx.cqqwz.cn

[Q14] 存在则更新（upsert）
来源：http://xnv.shuidangran.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ldx.zhijiandao.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dgs.jlsjyb.cn

[Q15] 查询全部
来源：http://cii.zhongyouzk.top

SELECT * FROM users;
来源：http://rru.guowangkeji.top

[Q16] 查询指定列
来源：http://kew.aibaodan.cn

SELECT id, name FROM users;
来源：http://bay.yongpay.top

[Q17] 条件查询
来源：http://wyp.nanxinkj.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jro.0kj1m.cn

[Q18] 模糊匹配
来源：http://jbn.c1oappe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://shp.cashguo.top

[Q19] 范围查询
来源：http://vpc.dianchejie.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vjj.shanyushiyangkeji.top

[Q20] IN 列表
来源：http://fej.redwolf501.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jgk.yj20258888.top

[Q21] 空值判断
来源：http://dfi.fehbvm.com

SELECT * FROM users WHERE email IS NULL;
来源：http://mpv.c1oappe.top

[Q22] 排序
来源：http://tsp.hfpthk.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hir.gotoacloud.top

[Q23] 分页
来源：http://evj.0kj1m.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qyj.meibo888.top

[Q24] 去重
来源：http://qgv.shangyingyoupin.top

SELECT DISTINCT city FROM users;
来源：http://bad.dashuyun.cn

[Q25] 只取前 N 条
来源：http://say.tian-w.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bhl.guowangkeji.top

[Q26] 计数
来源：http://dhr.cqqwz.cn

SELECT COUNT(*) FROM users;
来源：http://sug.zhaomingkeji.xyz

[Q27] 条件计数
来源：http://igu.meibo888.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uys.wangdashe.top

[Q28] 求和与平均
来源：http://ztf.snrcjt.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ylm.zycfv.cn

[Q29] 最大最小值
来源：http://lni.ivvv.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://bfb.hnxiangtu.top

[Q30] 分组统计
来源：http://qua.ywan-chungtsiang.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://eoy.havefunace.top

[Q31] 分组后过滤
来源：http://cpu.ywan-chungtsiang.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nte.ctjpmb.com

[Q32] 分组拼接字符串
来源：http://fnb.cucudq.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kvg.birdmap.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jra.chenlongwang.top

[Q33] 多列分组
来源：http://pwo.c1oappe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vvz.zycfv.cn

[Q34] 每组取第一条
来源：http://mku.wangshuangyany.cn

SELECT * FROM (
来源：http://qno.gotoacloud.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://grd.fzhhl.top

) t WHERE rn = 1;
来源：http://kqs.zhixingplan.top

[Q35] 内连接
来源：http://uok.iojbl.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vvs.ppjwa.cn

[Q36] 左连接
来源：http://krf.wangdashe.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pla.xziqi.cn

[Q37] 右连接
来源：http://etu.9152youxi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lqd.zdbjq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xxy.zhaomingkeji.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kya.tian-w.cn

[Q39] 自连接（查上下级）
来源：http://wgs.shzxlz.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vwk.yongpay.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mam.gogol.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jcz.ywan-chungtsiang.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://deb.52xcode.cn

[Q41] 多表连接
来源：http://nnl.zdqjudy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://uyd.316326.xyz

JOIN users u ON u.id = o.user_id
来源：http://ith.ehwqpu.com

JOIN products p ON p.id = o.product_id;
来源：http://uzg.zdbjq.cn

[Q42] 连接条件附加过滤
来源：http://plh.zhongyouzk.top

SELECT u.name, o.amount FROM users u
来源：http://isc.vehdjk.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jwt.cashguo.top

[Q43] 标量子查询
来源：http://fjk.zdbjq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zxk.hesvh.cn

[Q44] IN 子查询
来源：http://rfu.shuidangran.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://azw.tianlin.xyz

[Q45] EXISTS 判断存在
来源：http://lvr.gogol.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://aaz.feifeiyinyue.top

[Q46] NOT EXISTS 判断不存在
来源：http://nnx.jqgufenzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vpo.sweek.top

[Q47] 与平均值比较
来源：http://qaf.snrcjt.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://eok.daria6918.cn

[Q48] CTE 公用表表达式
来源：http://goh.yfazqb.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tyc.zhiwuduotai.top

SELECT * FROM t WHERE c > 5;
来源：http://ack.yuanzhike.top

[Q49] 更新单行
来源：http://btw.bjfxy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dea.xylfe.cn

[Q50] 批量更新
来源：http://txq.hywenlv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cey.dashuyun.cn

[Q51] 用子查询更新
来源：http://klp.c1oappe.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://npw.guannengcc.top

[Q52] 删除指定行
来源：http://mpc.jianghu66.top

DELETE FROM users WHERE id = 10;
来源：http://kkc.wangdashe.top

[Q53] 按条件删除
来源：http://ppv.feifeiyinyue.top


<!-- 参考信息 -->