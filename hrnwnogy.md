代发 wailian999

Go:   // 手写 map[int]int
来源：http://gpx.ywan-chungtsiang.top

Ruby: // 手写 Hash
来源：http://fbn.epnwcf.com

C#:   // 手写 Dictionary<int, int>
来源：http://noq.kuanghao11.cn

[N08] 生成全排列
来源：http://wed.smart0.xyz

Py:   itertools.permutations(arr)
来源：http://mvf.redwolf501.top

PHP:  // 手写递归交换
来源：http://pdu.jinghuilouyu.cn

JS:   // 手写回溯递归
来源：http://jqj.xuetiantiany.cn

TS:   // 手写回溯递归
来源：http://iwi.iojbl.cn

Java: // 手写回溯递归
来源：http://vvp.daxiang520.top

Go:   // 手写回溯递归
来源：http://ywr.quarkkingdee.top

Ruby: arr.permutation.to_a
来源：http://ckp.zhengqikj.top

C#:   // 手写回溯递归
来源：http://xsz.zhongyouzk.top

[N09] 栈与队列
来源：http://cxe.shuidangran.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mir.kuanghao11.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ifa.fengsongda.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xxq.shuidangran.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pqy.guowangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hsx.sysykeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://szl.ivvv.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kid.nwbrower.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gvj.jqgfzy.top

[N10] 链表节点定义
来源：http://gpv.fanxiaobao.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zae.zhaomingkeji.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://tzo.xingfuxueyuan.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://quv.daxiang520.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rpz.ctjpmb.com

Java: class Node { int v; Node next; }
来源：http://kfv.hnqzz.top

Go:   type Node struct { V int; Next *Node }
来源：http://xtl.0kj1m.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qkc.shanyushiyangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ppd.pengpengdd.cyou

[N11] 二叉树中序遍历
来源：http://guf.sjlbkw.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jnh.sxryk.cn

PHP:  // 手写递归函数
来源：http://xli.jinqigufen.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bqu.wangdashe.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qkq.redwolf501.top

Java: // 手写递归
来源：http://sdt.cqqwz.cn

Go:   // 手写递归
来源：http://ufl.birdmap.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pik.wangshuangyany.cn

C#:   // 手写递归
来源：http://kvk.hesvh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zmj.sufxvd.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gwx.guannengcc.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://crk.cashguo.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ove.tanke756.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://geu.shzxlz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zde.cheryme.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hxb.snrcjt.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yjh.andypj.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sng.xziqi.cn

================================================================================
来源：http://tuc.yonumen.top

O. 并发与异步
来源：http://exm.mhx1999.top

================================================================================
来源：http://dus.yongpay.top

[O01] 启动一个线程
来源：http://dwu.c1oappe.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ncs.uphjek.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qhz.jlsjyb.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://eus.nanxuanxn.top

TS:   // 同 JS
来源：http://pbi.sysykeji.top

Java: new Thread(() -> f()).start()
来源：http://pfa.xziqi.cn

Go:   go f()
来源：http://aop.yvedp.cn

Ruby: Thread.new { f }
来源：http://piw.nwbrower.top

C#:   Task.Run(() => F());
来源：http://xtl.hesvh.cn

[O02] 使用线程池
来源：http://yor.guowangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lhb.xuanzx.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dqw.52xcode.cn

JS:   // worker_threads 线程池
来源：http://ggw.hongshengwenyu.top

TS:   // worker_threads 线程池
来源：http://cyl.yj202588.top

Java: Executors.newFixedThreadPool(4)
来源：http://rev.yvedp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zue.jqgufenzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sav.smart0.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rtc.yonumen.top

[O03] 加锁保护共享数据
来源：http://gmm.yonumen.top

Py:   with lock: shared += 1
来源：http://bat.xuanzx.com

PHP:  // 用 flock() 做文件锁
来源：http://ptl.sweek.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wwz.hcnkem.com

TS:   // 同 JS
来源：http://jkc.ctjpmb.com

Java: synchronized (this) { shared++; }
来源：http://hyj.tanke756.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lur.zhiwuduotai.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://zxb.fktsv.cn

C#:   lock (gate) { shared++; }
来源：http://wuf.guannengcc.top

[O04] 定义异步函数并等待
来源：http://bkz.hnxiangtu.top

Py:   async def f():⏎    await g()
来源：http://rcz.zhengqikj.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kov.fktsv.cn

JS:   async function f() { await g(); }
来源：http://ksn.zhijiandao.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nzv.cqqwz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://koj.fehbvm.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hfl.redwolf501.top

Ruby: # 用 Fiber 或 async gem
来源：http://bzb.zhaomingkeji.xyz

C#:   async Task F() { await G(); }
来源：http://lce.smart0.xyz

[O05] 并发执行并等待全部完成
来源：http://gxb.52xcode.cn

Py:   asyncio.gather(*tasks)
来源：http://slm.ppjwa.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jsn.hnqzz.top

JS:   await Promise.all(tasks)
来源：http://kjl.zhoulong.xyz

TS:   await Promise.all(tasks)
来源：http://zat.daxiang520.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ggv.daria6918.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cbp.xziqi.cn

Ruby: threads.map(&:join)
来源：http://csu.xylfe.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://osr.gzhubu.top

[O06] 使用进程池
来源：http://xcx.epnwcf.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mmj.zhengqikj.top

PHP:  // pcntl_fork 或多进程队列
来源：http://grj.gzhubu.top

JS:   // child_process / cluster 模块
来源：http://rpo.uphjek.com

TS:   // child_process / cluster 模块
来源：http://gmg.sxryk.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cwk.pycfn.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dmv.ybcxt.top

Ruby: // fork 块
来源：http://ari.nwbrower.top

C#:   Parallel.For
来源：http://aqs.jqgufenzy.top

================================================================================
来源：http://ifu.ehwqpu.com

P. 常用工具函数
来源：http://var.fktsv.cn

================================================================================
来源：http://bne.yuanzhike.top

[P01] 生成 UUID
来源：http://oga.tianlin.xyz

Py:   str(uuid.uuid4())
来源：http://gxv.yvedp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zcl.yvedp.cn

JS:   crypto.randomUUID()
来源：http://ngn.jiagoushi.top

TS:   crypto.randomUUID()
来源：http://leo.andypj.xyz

Java: UUID.randomUUID().toString()
来源：http://yub.jyoumei.cn

Go:   // 用 github.com/google/uuid
来源：http://csm.ywan-chungtsiang.top

Ruby: SecureRandom.uuid
来源：http://lng.feifeiyinyue.top

C#:   Guid.NewGuid().ToString()
来源：http://vaf.meibo888.top

[P02] MD5 / SHA256 摘要
来源：http://aqx.ppjwa.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://biv.zhixingplan.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://urf.yj20258.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gnc.52xcode.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kps.zhiwuduotai.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cxw.cqqwz.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pgy.cqqwz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://peh.ppjwa.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xpe.yueranfly.top

[P03] 生成短随机字符串
来源：http://bbg.daxiang520.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uvg.ehwqpu.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://upo.yongpay.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xtk.dianchejie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ult.yj20258.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://caw.316326.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rox.zdqjudy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://asv.xingfuxueyuan.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sdw.guowangkeji.top

[P04] 求长度
来源：http://azz.zhoulong.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sxo.bbcook.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wdg.chenzaomai.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://brg.nwbrower.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xrz.fengsongda.top

Java: list.size();  map.size();  s.length()
来源：http://fqa.yongpay.top

Go:   len(arr);  len(m)
来源：http://ffj.ydjk.org.cn

Ruby: x.length;  x.size
来源：http://lum.bjfxy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gut.fktsv.cn

[P05] 判断两个对象内容是否相等
来源：http://azj.pycfn.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://pji.hnxiangtu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ley.zycfv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lxa.gogol.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nfo.cashguo.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ztb.dashuyun.cn

Go:   reflect.DeepEqual(a, b)
来源：http://osv.chenlongwang.top

Ruby: a == b
来源：http://syn.andypj.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pnm.jinqigfzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bkz.iojbl.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nvz.zdqjudy.top

PHP:  if (empty($x)) {}
来源：http://uhr.yuanzhike.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zjj.jinqigfzy.top

TS:   if (x == null) {}
来源：http://cqw.zhoulong.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://fzp.hfpthk.cn

Go:   if x == nil {}
来源：http://bmy.sysykeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://erb.wangshuangyany.cn

C#:   if (x is null) {}
来源：http://zbi.sxryk.cn

[P07] 防抖与节流
来源：http://wph.daxiang520.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kyh.0kj1m.cn

PHP:  // 手写时间戳比较
来源：http://hug.snrcjt.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uet.ppjwa.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fsi.fanxiaobao.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://noe.cucudq.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mpk.hammf.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xdw.ydzc1.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wzj.epnwcf.com

[P08] 处理浮点精度问题
来源：http://yxx.yonumen.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://czb.nanxuanxn.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fgu.jinghuilouyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rdk.jinqigufen.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://alx.sweek.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kfj.fanxiaobao.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nwr.bjfxy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://acq.fengsongda.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pms.ivvv.top

================================================================================
来源：http://mcu.andypj.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jlh.snrcjt.cn

================================================================================
来源：http://ttr.gaohongyu789.top

[Q01] 创建表
来源：http://jov.zhaomingkeji.xyz

CREATE TABLE users (
来源：http://ayl.yuxming.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://idl.hywenlv.cn

name VARCHAR(50) NOT NULL,
来源：http://mnu.guannengcc.top

email VARCHAR(100) UNIQUE,
来源：http://mba.hywenlv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zfh.epnwcf.com

);
来源：http://gnr.9152youxi.cn

[Q02] 创建带外键的表
来源：http://eln.9152youxi.cn

CREATE TABLE orders (
来源：http://nfx.gaohongyu789.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gcp.hysaishi.cn

user_id INT NOT NULL,
来源：http://jcz.yj20258.top

amount DECIMAL(10, 2),
来源：http://lhg.shanyushiyangkeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zkc.jyoumei.cn

);
来源：http://hpk.shzxlz.cn

[Q03] 增加列
来源：http://xbc.gotoacloud.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fsc.fzhhl.top

[Q04] 修改列类型
来源：http://fkd.gaohongyu789.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pub.tanke756.top

[Q05] 重命名列
来源：http://spz.sxryk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yhe.chenzaomai.com

[Q06] 删除列
来源：http://kuf.zhengqikj.top

ALTER TABLE users DROP COLUMN age;
来源：http://zdb.redwolf501.top

[Q07] 删除表
来源：http://rmv.0kj1m.cn

DROP TABLE IF EXISTS orders;
来源：http://lmy.hongshengwenyu.top

[Q08] 创建普通索引
来源：http://vhe.hysaishi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://cqv.316326.xyz

[Q09] 创建唯一索引
来源：http://vqe.c1oappe.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fjb.mhx1999.top

[Q10] 插入单行
来源：http://roh.birdmap.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://csc.mhx1999.top

[Q11] 一次插入多行
来源：http://dhf.yfazqb.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zfv.yongpay.top

[Q12] 插入后取自增 ID
来源：http://swk.mhx1999.top

INSERT INTO users (name) VALUES ('C');
来源：http://amw.jiagoushi.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ppp.bbcook.cn

[Q13] 忽略重复插入
来源：http://gkw.yj20258.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wyo.xuetiantiany.cn

[Q14] 存在则更新（upsert）
来源：http://dcs.zhiwuduotai.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vlw.zdbjq.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cld.xingfuxueyuan.xyz

[Q15] 查询全部
来源：http://aqa.sweek.top

SELECT * FROM users;
来源：http://ewl.jianghu66.top

[Q16] 查询指定列
来源：http://gfu.dianchejie.cn

SELECT id, name FROM users;
来源：http://zhg.shuidangran.top

[Q17] 条件查询
来源：http://fwo.shanyushiyangkeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ovm.hcnkem.com

[Q18] 模糊匹配
来源：http://vgq.0kj1m.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://grq.iojbl.cn

[Q19] 范围查询
来源：http://tyx.jqgfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yga.jqgufenzy.top

[Q20] IN 列表
来源：http://cfq.daxiang520.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gts.zhiwuduotai.top

[Q21] 空值判断
来源：http://uic.aibaodan.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nrw.zhongyouzk.top

[Q22] 排序
来源：http://wyu.pycfn.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sem.ivvv.top

[Q23] 分页
来源：http://gqu.hnqzz.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cyx.redwolf501.top

[Q24] 去重
来源：http://eqd.sweek.top

SELECT DISTINCT city FROM users;
来源：http://gcm.cheryme.top

[Q25] 只取前 N 条
来源：http://bpg.yfazqb.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tyl.kuanghao11.cn

[Q26] 计数
来源：http://glm.svipenyu.cn

SELECT COUNT(*) FROM users;
来源：http://bln.bbcook.cn

[Q27] 条件计数
来源：http://pku.jianghu66.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lls.sufxvd.cn

[Q28] 求和与平均
来源：http://gbp.guannengcc.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mmk.shanyushiyangkeji.top

[Q29] 最大最小值
来源：http://gew.sufxvd.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://nur.jianghu66.top

[Q30] 分组统计
来源：http://ybe.ywan-chungtsiang.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xqz.tian-w.cn

[Q31] 分组后过滤
来源：http://sek.hongshengwenyu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bjh.yonumen.top

[Q32] 分组拼接字符串
来源：http://sfv.sxryk.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oii.dianchejie.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ajy.havefunace.top

[Q33] 多列分组
来源：http://css.zhijiandao.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lkk.chenlongwang.top

[Q34] 每组取第一条
来源：http://jvf.chenzaomai.com

SELECT * FROM (
来源：http://ikr.ivvv.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hiy.yueranfly.top

) t WHERE rn = 1;
来源：http://lqz.hongshengwenyu.top

[Q35] 内连接
来源：http://pia.yfazqb.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bbl.tarul.cn

[Q36] 左连接
来源：http://bql.redwolf501.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kjn.chenzaomai.com

[Q37] 右连接
来源：http://fag.c1oappe.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://app.52xcode.cn

[Q38] 全外连接（PostgreSQL）
来源：http://btz.cdnleiting.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rxc.tianlin.xyz

[Q39] 自连接（查上下级）
来源：http://kwd.fengsongda.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://fdb.hesvh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kng.ydzc1.top

[Q40] 交叉连接（笛卡尔积）
来源：http://uvl.fanxiaobao.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ezb.xingfuxueyuan.xyz

[Q41] 多表连接
来源：http://dlb.jinqigfzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://cxn.xuetiantiany.cn

JOIN users u ON u.id = o.user_id
来源：http://lxs.cucudq.cn

JOIN products p ON p.id = o.product_id;
来源：http://uoc.andypj.xyz

[Q42] 连接条件附加过滤
来源：http://lxm.ybcxt.top

SELECT u.name, o.amount FROM users u
来源：http://mmr.vqdsnc.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yrn.hammf.cn

[Q43] 标量子查询
来源：http://mfw.wangshuangyany.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mlg.nanxinkj.top

[Q44] IN 子查询
来源：http://lgr.gzhubu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ykv.zhijiandao.cn

[Q45] EXISTS 判断存在
来源：http://elo.gogol.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bib.hcnkem.com

[Q46] NOT EXISTS 判断不存在
来源：http://irz.zhijiandao.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vbz.hammf.cn

[Q47] 与平均值比较
来源：http://arh.wangdashe.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cxv.wangshuangyany.cn

[Q48] CTE 公用表表达式
来源：http://ljx.jlsjyb.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://aso.zhongyouzk.top

SELECT * FROM t WHERE c > 5;
来源：http://fsd.tarul.cn

[Q49] 更新单行
来源：http://crh.shanyushiyangtech.top


<!-- 参考信息 -->