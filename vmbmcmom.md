代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://okg.chenlongwang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://col.jinyuanbaomall.cn

TS:   // 手写 Map<string, number>
来源：http://kpt.gotoacloud.top

Java: // 手写 HashMap
来源：http://atf.vqdsnc.cn

Go:   // 手写 map[int]int
来源：http://gfh.0kj1m.cn

Ruby: // 手写 Hash
来源：http://mpm.zdbjq.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rlq.shzxlz.cn

[N08] 生成全排列
来源：http://yky.cheryme.top

Py:   itertools.permutations(arr)
来源：http://ywy.ctjpmb.com

PHP:  // 手写递归交换
来源：http://vvj.cashguo.top

JS:   // 手写回溯递归
来源：http://dke.epnwcf.com

TS:   // 手写回溯递归
来源：http://vif.birdmap.top

Java: // 手写回溯递归
来源：http://mqk.52xcode.cn

Go:   // 手写回溯递归
来源：http://dgh.ctjpmb.com

Ruby: arr.permutation.to_a
来源：http://vik.tanke756.top

C#:   // 手写回溯递归
来源：http://dyg.ydzc1.top

[N09] 栈与队列
来源：http://doi.ehwqpu.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kam.yongpay.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jci.daxiang520.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ltd.jlsjyb.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cbv.xuanzx.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fyi.fktsv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vtp.vehdjk.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vfm.hywenlv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vqa.sysykeji.top

[N10] 链表节点定义
来源：http://fbq.sufxvd.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xps.zhaomingkeji.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://tda.52xcode.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://igq.aibaodan.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pog.shuidangran.top

Java: class Node { int v; Node next; }
来源：http://krw.cheryme.top

Go:   type Node struct { V int; Next *Node }
来源：http://mhm.sweek.top

Ruby: Node = Struct.new(:v, :next)
来源：http://owa.zhixingplan.top

C#:   class Node { public int V; public Node? Next; }
来源：http://yff.wangshuangyany.cn

[N11] 二叉树中序遍历
来源：http://jzb.aibaodan.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xie.jqgufenzy.top

PHP:  // 手写递归函数
来源：http://myi.tian-w.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ctf.shangyingyoupin.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gvw.epnwcf.com

Java: // 手写递归
来源：http://dzq.nanxuanxn.top

Go:   // 手写递归
来源：http://zhh.sweek.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lwp.ydjk.org.cn

C#:   // 手写递归
来源：http://zwg.jinyuanbaomall.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tfa.pengpengdd.cyou

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ihf.cheryme.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jer.wangdashe.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://foz.xuanzx.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fts.ehwqpu.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ddd.zhoulong.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rtj.redwolf501.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zpf.hammf.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hpq.cdnleiting.top

================================================================================
来源：http://jhf.jinghuilouyu.cn

O. 并发与异步
来源：http://clk.xuanzx.com

================================================================================
来源：http://rti.aizwys.cn

[O01] 启动一个线程
来源：http://nlu.jqgfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://iar.xziqi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://otq.zhixingplan.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rgk.uphjek.com

TS:   // 同 JS
来源：http://prz.meibo888.top

Java: new Thread(() -> f()).start()
来源：http://zwn.jinqigfzy.top

Go:   go f()
来源：http://cfx.jinqigufen.top

Ruby: Thread.new { f }
来源：http://ccj.zhengqikj.top

C#:   Task.Run(() => F());
来源：http://saa.tarul.cn

[O02] 使用线程池
来源：http://kgh.epnwcf.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vcb.sysykeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gmw.ydjk.org.cn

JS:   // worker_threads 线程池
来源：http://vov.sysykeji.top

TS:   // worker_threads 线程池
来源：http://bho.tanke756.top

Java: Executors.newFixedThreadPool(4)
来源：http://bou.jinyuanbaomall.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cek.zhongyouzk.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gez.zhengqikj.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zit.ctjpmb.com

[O03] 加锁保护共享数据
来源：http://auy.vehdjk.com

Py:   with lock: shared += 1
来源：http://xck.quarkkingdee.top

PHP:  // 用 flock() 做文件锁
来源：http://ori.cashguo.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://olz.jinghuilouyu.cn

TS:   // 同 JS
来源：http://oom.hnxiangtu.top

Java: synchronized (this) { shared++; }
来源：http://jgb.cashguo.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qyq.iojbl.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://acs.pycfn.com

C#:   lock (gate) { shared++; }
来源：http://iqe.pengpengdd.cyou

[O04] 定义异步函数并等待
来源：http://lgm.shanyushiyangkeji.top

Py:   async def f():⏎    await g()
来源：http://udn.kuanghao11.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qvg.shanyushiyangkeji.top

JS:   async function f() { await g(); }
来源：http://egk.chenzaomai.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://hnh.fanxiaobao.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rjj.sysykeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wkd.316326.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://kwt.iojbl.cn

C#:   async Task F() { await G(); }
来源：http://vkf.jinyuanbaomall.cn

[O05] 并发执行并等待全部完成
来源：http://xch.ppjwa.cn

Py:   asyncio.gather(*tasks)
来源：http://mqn.zdqjudy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ghn.yj202588.top

JS:   await Promise.all(tasks)
来源：http://wov.jiagoushi.top

TS:   await Promise.all(tasks)
来源：http://zrp.cqqwz.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rxw.fzhhl.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zip.fktsv.cn

Ruby: threads.map(&:join)
来源：http://uis.52xcode.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://swt.yuanzhike.top

[O06] 使用进程池
来源：http://brv.chenjidiqi.icu

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bzu.tianlin.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://csk.zhijiandao.cn

JS:   // child_process / cluster 模块
来源：http://efn.zhengqikj.top

TS:   // child_process / cluster 模块
来源：http://zge.hywenlv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bzj.ppjwa.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qbx.andypj.xyz

Ruby: // fork 块
来源：http://jgn.yj20258888.top

C#:   Parallel.For
来源：http://nxh.yuxming.cn

================================================================================
来源：http://fdc.yvedp.cn

P. 常用工具函数
来源：http://ydp.guowangkeji.top

================================================================================
来源：http://zlp.yfazqb.com

[P01] 生成 UUID
来源：http://foo.guowangkeji.top

Py:   str(uuid.uuid4())
来源：http://myx.shuidangran.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://idl.yuxming.cn

JS:   crypto.randomUUID()
来源：http://dks.xingfuxueyuan.xyz

TS:   crypto.randomUUID()
来源：http://sdj.jqgufenzy.top

Java: UUID.randomUUID().toString()
来源：http://qll.hammf.cn

Go:   // 用 github.com/google/uuid
来源：http://cti.cucudq.cn

Ruby: SecureRandom.uuid
来源：http://xal.cucudq.cn

C#:   Guid.NewGuid().ToString()
来源：http://jyn.vehdjk.com

[P02] MD5 / SHA256 摘要
来源：http://gpy.jlsjyb.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wgf.xuetiantiany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kqu.yvedp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ecz.vehdjk.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rpo.gotoacloud.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://srv.xylfe.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vmg.svipenyu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dow.xylfe.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mdm.ehwqpu.com

[P03] 生成短随机字符串
来源：http://bnr.hesvh.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zvi.kuanghao11.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://arn.316326.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xth.shuidangran.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cox.jiagoushi.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dsd.yvedp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rfe.ywan-chungtsiang.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://weo.ppjwa.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xqx.pengpengdd.cyou

[P04] 求长度
来源：http://wvj.fanxiaobao.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ylk.316326.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hjr.vehdjk.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mkh.c1oappe.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mvv.pengpengdd.cyou

Java: list.size();  map.size();  s.length()
来源：http://zpp.cashguo.top

Go:   len(arr);  len(m)
来源：http://pde.sysykeji.top

Ruby: x.length;  x.size
来源：http://jra.hcnkem.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://epm.jinqigufen.top

[P05] 判断两个对象内容是否相等
来源：http://gep.chenlongwang.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://heh.zhoulong.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rnm.cucudq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kqs.haohaochexian.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vxx.guowangkeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://agl.jqgfzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://mnr.aibaodan.cn

Ruby: a == b
来源：http://qok.andypj.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cpb.chenlongwang.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jrk.sysykeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pss.jqgfzy.top

PHP:  if (empty($x)) {}
来源：http://xvc.svipenyu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xmz.ppjwa.cn

TS:   if (x == null) {}
来源：http://qmk.kuanghao11.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vrq.sxryk.cn

Go:   if x == nil {}
来源：http://feu.ywan-chungtsiang.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://iqb.ctjpmb.com

C#:   if (x is null) {}
来源：http://mth.pengpengdd.cyou

[P07] 防抖与节流
来源：http://btg.jianghu66.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wtb.jinyuanbaomall.cn

PHP:  // 手写时间戳比较
来源：http://ncr.cdnleiting.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cuv.jlsjyb.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ips.yj20258.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kgz.feifeiyinyue.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xdn.sysykeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://rgr.shanyushiyangtech.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yxh.ehwqpu.com

[P08] 处理浮点精度问题
来源：http://cvx.gzhubu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://oeo.9152youxi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xgm.fehbvm.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lzc.cucudq.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ipv.gaohongyu789.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oke.ctjpmb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gfx.nanxuanxn.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://edt.xinyue.icu

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vng.redwolf501.top

================================================================================
来源：http://dha.nanxuanxn.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bvc.hnxiangtu.top

================================================================================
来源：http://mdd.zycfv.cn

[Q01] 创建表
来源：http://dpm.hfpthk.cn

CREATE TABLE users (
来源：http://cmd.iojbl.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kxl.yvedp.cn

name VARCHAR(50) NOT NULL,
来源：http://kob.aibaodan.cn

email VARCHAR(100) UNIQUE,
来源：http://nuy.jinghuilouyu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mvc.shzxlz.cn

);
来源：http://ktc.ywan-chungtsiang.top

[Q02] 创建带外键的表
来源：http://ifh.jinqigufen.top

CREATE TABLE orders (
来源：http://hav.ydzc1.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jhn.jqgufenzy.top

user_id INT NOT NULL,
来源：http://vbc.gogol.net.cn

amount DECIMAL(10, 2),
来源：http://ubw.hfpthk.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://awb.fzhhl.top

);
来源：http://oru.gaohongyu789.top

[Q03] 增加列
来源：http://vvc.mhx1999.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xab.meibo888.top

[Q04] 修改列类型
来源：http://huj.ydzc1.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://axg.xziqi.cn

[Q05] 重命名列
来源：http://ppu.shuidangran.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sqh.guowangkeji.top

[Q06] 删除列
来源：http://szn.zhoulong.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://bnj.ivvv.top

[Q07] 删除表
来源：http://olh.epnwcf.com

DROP TABLE IF EXISTS orders;
来源：http://krd.chenlongwang.top

[Q08] 创建普通索引
来源：http://wlf.ydzc1.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ohm.gogol.net.cn

[Q09] 创建唯一索引
来源：http://ric.sufxvd.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://otx.shzxlz.cn

[Q10] 插入单行
来源：http://tya.yongpay.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://akw.havefunace.top

[Q11] 一次插入多行
来源：http://tbf.guowangkeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://smu.hfpthk.cn

[Q12] 插入后取自增 ID
来源：http://amt.shanyushiyangkeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://fas.jqgufenzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pfu.hfpthk.cn

[Q13] 忽略重复插入
来源：http://yyg.nanxuanxn.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://edd.c1oappe.top

[Q14] 存在则更新（upsert）
来源：http://hzx.tianlin.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://erb.bjfxy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nqu.cucudq.cn

[Q15] 查询全部
来源：http://qme.yj202588.top

SELECT * FROM users;
来源：http://psn.yonumen.top

[Q16] 查询指定列
来源：http://bek.xinyue.icu

SELECT id, name FROM users;
来源：http://saz.xuetiantiany.cn

[Q17] 条件查询
来源：http://frr.yfazqb.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ukc.havefunace.top

[Q18] 模糊匹配
来源：http://vcv.havefunace.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qty.gotoacloud.top

[Q19] 范围查询
来源：http://wbd.shanyushiyangtech.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vmr.fzhhl.top

[Q20] IN 列表
来源：http://zpu.smart0.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ynj.pengpengdd.cyou

[Q21] 空值判断
来源：http://rem.cqqwz.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hqi.daxiang520.top

[Q22] 排序
来源：http://hud.nanxinkj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://leu.shuidangran.top

[Q23] 分页
来源：http://gcw.ctjpmb.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mdb.yuxming.cn

[Q24] 去重
来源：http://onv.cqqwz.cn

SELECT DISTINCT city FROM users;
来源：http://yis.daria6918.cn

[Q25] 只取前 N 条
来源：http://oub.cqqwz.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://die.xingfuxueyuan.xyz

[Q26] 计数
来源：http://tpc.dashuyun.cn

SELECT COUNT(*) FROM users;
来源：http://vaq.sufxvd.cn

[Q27] 条件计数
来源：http://gsh.hysaishi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cct.cheryme.top

[Q28] 求和与平均
来源：http://brb.haohaochexian.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tlv.cdnleiting.top

[Q29] 最大最小值
来源：http://gke.zhongyouzk.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://pju.wangshuangyany.cn

[Q30] 分组统计
来源：http://uuw.cheryme.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qxl.zhiwuduotai.top

[Q31] 分组后过滤
来源：http://udi.zhongyouzk.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zkg.zdqjudy.top

[Q32] 分组拼接字符串
来源：http://zzt.jiagoushi.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://upr.epnwcf.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://aic.snrcjt.cn

[Q33] 多列分组
来源：http://wox.snrcjt.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://igp.dianchejie.cn

[Q34] 每组取第一条
来源：http://zxu.jinqigufen.top

SELECT * FROM (
来源：http://qsa.yj20258888.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ioc.zhengqikj.top

) t WHERE rn = 1;
来源：http://bio.andypj.xyz

[Q35] 内连接
来源：http://woc.daria6918.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pzc.yonumen.top

[Q36] 左连接
来源：http://adp.sweek.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mhp.daxiang520.top

[Q37] 右连接
来源：http://dyq.ydzc1.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zeh.yj20258888.top

[Q38] 全外连接（PostgreSQL）
来源：http://qnu.daxiang520.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hld.xingfuxueyuan.xyz

[Q39] 自连接（查上下级）
来源：http://sjh.jinqigfzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ohs.tarul.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vup.zhijiandao.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jhz.shangyingyoupin.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lbs.andypj.xyz

[Q41] 多表连接
来源：http://wfh.sysykeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://hzi.xziqi.cn

JOIN users u ON u.id = o.user_id
来源：http://prz.jyoumei.cn

JOIN products p ON p.id = o.product_id;
来源：http://nma.fehbvm.com

[Q42] 连接条件附加过滤
来源：http://pxn.hywenlv.cn

SELECT u.name, o.amount FROM users u
来源：http://ggd.uphjek.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ihf.gaohongyu789.top

[Q43] 标量子查询
来源：http://zcu.hfpthk.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://spk.tanke756.top

[Q44] IN 子查询
来源：http://mdz.c1oappe.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pqm.hysaishi.cn

[Q45] EXISTS 判断存在
来源：http://aeq.quarkkingdee.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://inm.yongpay.top

[Q46] NOT EXISTS 判断不存在
来源：http://knw.zhixingplan.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jfx.svipenyu.cn

[Q47] 与平均值比较
来源：http://mik.jianghu66.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pvn.sjlbkw.cn


<!-- 参考信息 -->