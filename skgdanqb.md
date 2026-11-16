代发 wailian999

Py:   itertools.permutations(arr)
来源：http://hhq.bbcook.cn

PHP:  // 手写递归交换
来源：http://gdq.uphjek.com

JS:   // 手写回溯递归
来源：http://fxu.hywenlv.cn

TS:   // 手写回溯递归
来源：http://ntf.fanxiaobao.xyz

Java: // 手写回溯递归
来源：http://qte.zycfv.cn

Go:   // 手写回溯递归
来源：http://xvg.nwbrower.top

Ruby: arr.permutation.to_a
来源：http://jdh.tianlin.xyz

C#:   // 手写回溯递归
来源：http://yhq.hywenlv.cn

[N09] 栈与队列
来源：http://klk.cqqwz.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://moy.zdbjq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vqd.hfpthk.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vlc.tarul.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://foe.bjfxy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lsj.xziqi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://iey.tianlin.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://daf.gogol.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ozt.yj20258.top

[N10] 链表节点定义
来源：http://ekm.sweek.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dtw.xylfe.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yhh.hfpthk.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hfa.gogol.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rur.fengsongda.top

Java: class Node { int v; Node next; }
来源：http://hlo.yonumen.top

Go:   type Node struct { V int; Next *Node }
来源：http://xbr.dianchejie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hkm.chenzaomai.com

C#:   class Node { public int V; public Node? Next; }
来源：http://zsm.redwolf501.top

[N11] 二叉树中序遍历
来源：http://kju.hesvh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://olh.havefunace.top

PHP:  // 手写递归函数
来源：http://bof.bjfxy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://twy.jiagoushi.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bzv.nwbrower.top

Java: // 手写递归
来源：http://aic.xuetiantiany.cn

Go:   // 手写递归
来源：http://orw.aibaodan.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tsd.jinqigfzy.top

C#:   // 手写递归
来源：http://xqw.haohaochexian.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mts.ywan-chungtsiang.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kbc.nwbrower.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ppi.pengpengdd.cyou

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mds.feifeiyinyue.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mmp.andypj.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rqb.zhijiandao.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://chd.zhaomingkeji.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tph.xziqi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zdu.zhoulong.xyz

================================================================================
来源：http://eab.cashguo.top

O. 并发与异步
来源：http://wvy.fzhhl.top

================================================================================
来源：http://bjj.ydzc1.top

[O01] 启动一个线程
来源：http://qpn.yuxming.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qot.tarul.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tui.tarul.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hxq.shangyingyoupin.top

TS:   // 同 JS
来源：http://jeb.snrcjt.cn

Java: new Thread(() -> f()).start()
来源：http://nyw.hammf.cn

Go:   go f()
来源：http://vki.gotoacloud.top

Ruby: Thread.new { f }
来源：http://idb.bjfxy.top

C#:   Task.Run(() => F());
来源：http://tnb.xziqi.cn

[O02] 使用线程池
来源：http://fcz.9152youxi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zht.shuidangran.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wyt.xziqi.cn

JS:   // worker_threads 线程池
来源：http://npd.zhoulong.xyz

TS:   // worker_threads 线程池
来源：http://uni.chenzaomai.com

Java: Executors.newFixedThreadPool(4)
来源：http://svw.kuanghao11.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bvj.svipenyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ila.nanxuanxn.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dpy.shuidangran.top

[O03] 加锁保护共享数据
来源：http://pdw.pycfn.com

Py:   with lock: shared += 1
来源：http://zig.cqqwz.cn

PHP:  // 用 flock() 做文件锁
来源：http://wnx.zhijiandao.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://svr.sjlbkw.cn

TS:   // 同 JS
来源：http://uyc.zdqjudy.top

Java: synchronized (this) { shared++; }
来源：http://jgp.redwolf501.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mbm.gotoacloud.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://diu.cheryme.top

C#:   lock (gate) { shared++; }
来源：http://ohp.ivvv.top

[O04] 定义异步函数并等待
来源：http://sdy.hnqzz.top

Py:   async def f():⏎    await g()
来源：http://quj.vqdsnc.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://iqq.cqqwz.cn

JS:   async function f() { await g(); }
来源：http://qym.vqdsnc.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qzr.zhongyouzk.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fur.jqgfzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qzm.zhijiandao.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wfc.fktsv.cn

C#:   async Task F() { await G(); }
来源：http://ljj.havefunace.top

[O05] 并发执行并等待全部完成
来源：http://qtc.xuanzx.com

Py:   asyncio.gather(*tasks)
来源：http://ptd.tian-w.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xss.yj20258.top

JS:   await Promise.all(tasks)
来源：http://bdw.gogol.net.cn

TS:   await Promise.all(tasks)
来源：http://cor.aibaodan.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lre.ybcxt.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cyb.redwolf501.top

Ruby: threads.map(&:join)
来源：http://ilg.shanyushiyangtech.top

C#:   await Task.WhenAll(t1, t2)
来源：http://uka.zhijiandao.cn

[O06] 使用进程池
来源：http://wio.gaohongyu789.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gky.vehdjk.com

PHP:  // pcntl_fork 或多进程队列
来源：http://ehw.jyoumei.cn

JS:   // child_process / cluster 模块
来源：http://xrk.yonumen.top

TS:   // child_process / cluster 模块
来源：http://hmf.yj20258.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qyu.yj20258888.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bvm.vqdsnc.cn

Ruby: // fork 块
来源：http://jvi.yuanzhike.top

C#:   Parallel.For
来源：http://yck.yangfankeji.com

================================================================================
来源：http://guk.kuanghao11.cn

P. 常用工具函数
来源：http://azr.redwolf501.top

================================================================================
来源：http://cii.vqdsnc.cn

[P01] 生成 UUID
来源：http://ave.yuanzhike.top

Py:   str(uuid.uuid4())
来源：http://joq.hnxiangtu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qqk.gotoacloud.top

JS:   crypto.randomUUID()
来源：http://rwf.cheryme.top

TS:   crypto.randomUUID()
来源：http://xzh.hnqzz.top

Java: UUID.randomUUID().toString()
来源：http://fak.shanyushiyangtech.top

Go:   // 用 github.com/google/uuid
来源：http://xcs.shzxlz.cn

Ruby: SecureRandom.uuid
来源：http://pgp.yj20258888.top

C#:   Guid.NewGuid().ToString()
来源：http://igb.zhiwuduotai.top

[P02] MD5 / SHA256 摘要
来源：http://rvt.zhoulong.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fcf.yj20258888.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://pzu.hcnkem.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://obw.ydzc1.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lat.tarul.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gjj.xinyue.icu

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dkk.jinqigfzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bid.shanyushiyangtech.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kqw.chenjidiqi.icu

[P03] 生成短随机字符串
来源：http://poo.xuanzx.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://iyp.hywenlv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bgi.9152youxi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gmd.gogol.net.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ubz.svipenyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kzk.ppjwa.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sai.pengpengdd.cyou

Ruby: SecureRandom.alphanumeric(16)
来源：http://pdk.xylfe.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gxw.aizwys.cn

[P04] 求长度
来源：http://sdn.hesvh.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qvf.jiagoushi.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sce.52xcode.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://puy.guowangkeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://teo.cqqwz.cn

Java: list.size();  map.size();  s.length()
来源：http://kqh.tian-w.cn

Go:   len(arr);  len(m)
来源：http://cpn.sysykeji.top

Ruby: x.length;  x.size
来源：http://pea.hfpthk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://nwx.tian-w.cn

[P05] 判断两个对象内容是否相等
来源：http://bgy.fktsv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://edt.guowangkeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rqd.jiagoushi.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://eae.ctjpmb.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ojc.zhiwuduotai.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gmz.smart0.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://aup.hcnkem.com

Ruby: a == b
来源：http://pjx.chenzaomai.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ejl.feifeiyinyue.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pze.hongshengwenyu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yep.feifeiyinyue.top

PHP:  if (empty($x)) {}
来源：http://jra.chenlongwang.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rts.gaohongyu789.top

TS:   if (x == null) {}
来源：http://iuz.fengsongda.top

Java: if (x == null || x.isEmpty()) {}
来源：http://hpg.shanyushiyangkeji.top

Go:   if x == nil {}
来源：http://mok.andypj.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lye.52xcode.cn

C#:   if (x is null) {}
来源：http://qyp.chenzaomai.com

[P07] 防抖与节流
来源：http://pgc.jinqigfzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xcu.mhx1999.top

PHP:  // 手写时间戳比较
来源：http://xop.yj202588.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://edy.hnqzz.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pxk.havefunace.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nea.snrcjt.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ytd.sysykeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://dzi.jlsjyb.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lxk.shuidangran.top

[P08] 处理浮点精度问题
来源：http://etl.zhijiandao.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qom.xziqi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xjo.iojbl.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ndb.kuanghao11.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gaw.yongpay.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oau.guannengcc.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gpm.yuxming.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yez.dianchejie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fcu.jiagoushi.top

================================================================================
来源：http://bbm.fktsv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hjh.daxiang520.top

================================================================================
来源：http://oat.hfpthk.cn

[Q01] 创建表
来源：http://dlr.nanxuanxn.top

CREATE TABLE users (
来源：http://rlm.chenjidiqi.icu

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://omb.sufxvd.cn

name VARCHAR(50) NOT NULL,
来源：http://szq.316326.xyz

email VARCHAR(100) UNIQUE,
来源：http://hxb.sweek.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lfx.sufxvd.cn

);
来源：http://eof.hywenlv.cn

[Q02] 创建带外键的表
来源：http://lkp.vehdjk.com

CREATE TABLE orders (
来源：http://etm.ivvv.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vwn.xingfuxueyuan.xyz

user_id INT NOT NULL,
来源：http://jjn.zhaomingkeji.xyz

amount DECIMAL(10, 2),
来源：http://uhb.sufxvd.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pac.nwbrower.top

);
来源：http://ajq.zhoulong.xyz

[Q03] 增加列
来源：http://rbg.bjfxy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zkm.ctjpmb.com

[Q04] 修改列类型
来源：http://zle.fzhhl.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://iio.yj202588.top

[Q05] 重命名列
来源：http://ihk.shanyushiyangkeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pta.ehwqpu.com

[Q06] 删除列
来源：http://weh.gzhubu.top

ALTER TABLE users DROP COLUMN age;
来源：http://ubm.zdbjq.cn

[Q07] 删除表
来源：http://dgy.hcnkem.com

DROP TABLE IF EXISTS orders;
来源：http://yck.wangdashe.top

[Q08] 创建普通索引
来源：http://cof.svipenyu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kte.jinqigfzy.top

[Q09] 创建唯一索引
来源：http://iyv.dianchejie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hcp.smart0.xyz

[Q10] 插入单行
来源：http://qge.nwbrower.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dfj.fktsv.cn

[Q11] 一次插入多行
来源：http://hfa.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vfd.jyoumei.cn

[Q12] 插入后取自增 ID
来源：http://dcy.c1oappe.top

INSERT INTO users (name) VALUES ('C');
来源：http://sgz.zhijiandao.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ity.jiagoushi.top

[Q13] 忽略重复插入
来源：http://ohh.9152youxi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oww.aizwys.cn

[Q14] 存在则更新（upsert）
来源：http://grv.andypj.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://odg.xinyue.icu

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mlw.jqgufenzy.top

[Q15] 查询全部
来源：http://zrq.tarul.cn

SELECT * FROM users;
来源：http://bzb.9152youxi.cn

[Q16] 查询指定列
来源：http://liw.kuanghao11.cn

SELECT id, name FROM users;
来源：http://amb.sysykeji.top

[Q17] 条件查询
来源：http://rml.zhixingplan.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wei.hnxiangtu.top

[Q18] 模糊匹配
来源：http://vzp.chenjidiqi.icu

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ibg.andypj.xyz

[Q19] 范围查询
来源：http://nkr.vqdsnc.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cgo.jinqigfzy.top

[Q20] IN 列表
来源：http://ftn.zhijiandao.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://piq.shanyushiyangkeji.top

[Q21] 空值判断
来源：http://nvd.jyoumei.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://wbz.xuetiantiany.cn

[Q22] 排序
来源：http://fut.redwolf501.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kkz.feifeiyinyue.top

[Q23] 分页
来源：http://jgc.feifeiyinyue.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ixq.sxryk.cn

[Q24] 去重
来源：http://bac.tian-w.cn

SELECT DISTINCT city FROM users;
来源：http://hft.yvedp.cn

[Q25] 只取前 N 条
来源：http://hnv.yuxming.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://map.hnqzz.top

[Q26] 计数
来源：http://fow.xingfuxueyuan.xyz

SELECT COUNT(*) FROM users;
来源：http://fni.sjlbkw.cn

[Q27] 条件计数
来源：http://kpn.zdqjudy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rgp.hywenlv.cn

[Q28] 求和与平均
来源：http://oyg.guowangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qwd.c1oappe.top

[Q29] 最大最小值
来源：http://hud.guannengcc.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jci.jiagoushi.top

[Q30] 分组统计
来源：http://dmz.haohaochexian.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://eus.hcnkem.com

[Q31] 分组后过滤
来源：http://xes.wangdashe.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sim.jinqigufen.top

[Q32] 分组拼接字符串
来源：http://ajl.yj20258.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ina.kuanghao11.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://buy.andypj.xyz

[Q33] 多列分组
来源：http://npw.xuetiantiany.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lgg.9152youxi.cn

[Q34] 每组取第一条
来源：http://zgc.zhongyouzk.top

SELECT * FROM (
来源：http://lbe.ydzc1.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://usu.chenjidiqi.icu

) t WHERE rn = 1;
来源：http://rvc.sxryk.cn

[Q35] 内连接
来源：http://wvp.shzxlz.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://szv.nanxinkj.top

[Q36] 左连接
来源：http://hnr.fktsv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ous.sufxvd.cn

[Q37] 右连接
来源：http://jnn.52xcode.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vxv.zhoulong.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://xip.ywan-chungtsiang.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qlx.andypj.xyz

[Q39] 自连接（查上下级）
来源：http://mon.ivvv.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://lxk.ehwqpu.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://swj.gotoacloud.top

[Q40] 交叉连接（笛卡尔积）
来源：http://mkx.c1oappe.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nxt.xziqi.cn

[Q41] 多表连接
来源：http://xdl.bjfxy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://jrx.xylfe.cn

JOIN users u ON u.id = o.user_id
来源：http://ajx.yonumen.top

JOIN products p ON p.id = o.product_id;
来源：http://lyq.gotoacloud.top

[Q42] 连接条件附加过滤
来源：http://bci.cheryme.top

SELECT u.name, o.amount FROM users u
来源：http://epk.zhijiandao.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yft.hammf.cn

[Q43] 标量子查询
来源：http://nni.zhixingplan.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qaa.chenlongwang.top

[Q44] IN 子查询
来源：http://hwg.316326.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ueh.quarkkingdee.top

[Q45] EXISTS 判断存在
来源：http://qje.sweek.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wah.xuetiantiany.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ibz.cheryme.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rjq.jiagoushi.top

[Q47] 与平均值比较
来源：http://vlm.tanke756.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ohp.cheryme.top

[Q48] CTE 公用表表达式
来源：http://xat.gogol.net.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://toj.zycfv.cn

SELECT * FROM t WHERE c > 5;
来源：http://gvz.tian-w.cn

[Q49] 更新单行
来源：http://vxt.tianlin.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sla.mhx1999.top

[Q50] 批量更新
来源：http://vfo.nwbrower.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cvn.yonumen.top

[Q51] 用子查询更新
来源：http://lyt.zhoulong.xyz


<!-- 参考信息 -->