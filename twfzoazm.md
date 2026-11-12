代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hmc.yueranfly.top

JS:   // 手写 Map：map.set(v, i)
来源：http://rcx.vqdsnc.cn

TS:   // 手写 Map<string, number>
来源：http://vex.hnqzz.top

Java: // 手写 HashMap
来源：http://vsg.tanke756.top

Go:   // 手写 map[int]int
来源：http://uzf.yvedp.cn

Ruby: // 手写 Hash
来源：http://bac.chenzaomai.com

C#:   // 手写 Dictionary<int, int>
来源：http://afo.chenlongwang.top

[N08] 生成全排列
来源：http://rfc.zdqjudy.top

Py:   itertools.permutations(arr)
来源：http://bne.fktsv.cn

PHP:  // 手写递归交换
来源：http://bhz.zhiwuduotai.top

JS:   // 手写回溯递归
来源：http://gyo.hysaishi.cn

TS:   // 手写回溯递归
来源：http://xyk.gaohongyu789.top

Java: // 手写回溯递归
来源：http://goe.gotoacloud.top

Go:   // 手写回溯递归
来源：http://okj.aizwys.cn

Ruby: arr.permutation.to_a
来源：http://adg.jqgufenzy.top

C#:   // 手写回溯递归
来源：http://anm.cdnleiting.top

[N09] 栈与队列
来源：http://hyc.yj20258888.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gac.zdbjq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qts.gaohongyu789.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xcn.jyoumei.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jtb.pycfn.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xpo.hnqzz.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://toi.meibo888.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lkq.yueranfly.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hot.zdqjudy.top

[N10] 链表节点定义
来源：http://nfx.daria6918.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uya.shanyushiyangkeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://hcw.cucudq.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pyh.xuetiantiany.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://juh.birdmap.top

Java: class Node { int v; Node next; }
来源：http://uor.dashuyun.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mbj.zhiwuduotai.top

Ruby: Node = Struct.new(:v, :next)
来源：http://gdm.hnxiangtu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://sby.hysaishi.cn

[N11] 二叉树中序遍历
来源：http://mgu.cheryme.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qzu.sweek.top

PHP:  // 手写递归函数
来源：http://ueb.xingfuxueyuan.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fqe.guannengcc.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jgt.fehbvm.com

Java: // 手写递归
来源：http://szm.hfpthk.cn

Go:   // 手写递归
来源：http://hch.hesvh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pgr.yuanzhike.top

C#:   // 手写递归
来源：http://bvt.jlsjyb.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ltb.fehbvm.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tho.meibo888.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ynk.daria6918.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kxj.hnxiangtu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://adq.zhijiandao.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zoi.shuidangran.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sam.xuetiantiany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://koe.zhoulong.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fwh.shangyingyoupin.top

================================================================================
来源：http://dww.ydzc1.top

O. 并发与异步
来源：http://lli.xziqi.cn

================================================================================
来源：http://cyq.aizwys.cn

[O01] 启动一个线程
来源：http://sqg.dashuyun.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ziz.ywan-chungtsiang.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xtt.yuanzhike.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qwy.xingfuxueyuan.xyz

TS:   // 同 JS
来源：http://qxq.ydjk.org.cn

Java: new Thread(() -> f()).start()
来源：http://cvi.yvedp.cn

Go:   go f()
来源：http://ucv.ydjk.org.cn

Ruby: Thread.new { f }
来源：http://gyr.havefunace.top

C#:   Task.Run(() => F());
来源：http://btr.epnwcf.com

[O02] 使用线程池
来源：http://drc.ydjk.org.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gvb.ybcxt.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dfo.zhiwuduotai.top

JS:   // worker_threads 线程池
来源：http://vgs.hesvh.cn

TS:   // worker_threads 线程池
来源：http://ihi.yongpay.top

Java: Executors.newFixedThreadPool(4)
来源：http://ixz.chenzaomai.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qig.vqdsnc.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://upg.tian-w.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gto.tanke756.top

[O03] 加锁保护共享数据
来源：http://wke.shanyushiyangkeji.top

Py:   with lock: shared += 1
来源：http://wds.jyoumei.cn

PHP:  // 用 flock() 做文件锁
来源：http://kbu.hammf.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cvz.sufxvd.cn

TS:   // 同 JS
来源：http://ljw.bjfxy.top

Java: synchronized (this) { shared++; }
来源：http://dxw.wangshuangyany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xps.jqgufenzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://hkc.hesvh.cn

C#:   lock (gate) { shared++; }
来源：http://fqk.hnqzz.top

[O04] 定义异步函数并等待
来源：http://waa.tarul.cn

Py:   async def f():⏎    await g()
来源：http://qvh.mhx1999.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rsz.zhijiandao.cn

JS:   async function f() { await g(); }
来源：http://frn.smart0.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://tiz.cashguo.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sot.52xcode.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xvu.9152youxi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nqo.ywan-chungtsiang.top

C#:   async Task F() { await G(); }
来源：http://aum.ivvv.top

[O05] 并发执行并等待全部完成
来源：http://kwy.dianchejie.cn

Py:   asyncio.gather(*tasks)
来源：http://fos.vehdjk.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mlc.zhijiandao.cn

JS:   await Promise.all(tasks)
来源：http://pdp.xuetiantiany.cn

TS:   await Promise.all(tasks)
来源：http://eco.hongshengwenyu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yqm.hammf.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://aqu.jinqigfzy.top

Ruby: threads.map(&:join)
来源：http://roo.zhongyouzk.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fhy.jinghuilouyu.cn

[O06] 使用进程池
来源：http://kek.epnwcf.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dno.yongpay.top

PHP:  // pcntl_fork 或多进程队列
来源：http://smn.dashuyun.cn

JS:   // child_process / cluster 模块
来源：http://dbb.ivvv.top

TS:   // child_process / cluster 模块
来源：http://jbw.hfpthk.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://atc.haohaochexian.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eqb.yj20258.top

Ruby: // fork 块
来源：http://pbi.gotoacloud.top

C#:   Parallel.For
来源：http://eut.haohaochexian.top

================================================================================
来源：http://rip.ehwqpu.com

P. 常用工具函数
来源：http://fde.hammf.cn

================================================================================
来源：http://zfe.bbcook.cn

[P01] 生成 UUID
来源：http://vlr.xuetiantiany.cn

Py:   str(uuid.uuid4())
来源：http://qmb.birdmap.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sfg.kuanghao11.cn

JS:   crypto.randomUUID()
来源：http://nrd.cheryme.top

TS:   crypto.randomUUID()
来源：http://poe.yj202588.top

Java: UUID.randomUUID().toString()
来源：http://rgp.dashuyun.cn

Go:   // 用 github.com/google/uuid
来源：http://msc.yueranfly.top

Ruby: SecureRandom.uuid
来源：http://dja.xinyue.icu

C#:   Guid.NewGuid().ToString()
来源：http://mhi.tianlin.xyz

[P02] MD5 / SHA256 摘要
来源：http://rxc.ywan-chungtsiang.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qog.wangdashe.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://flu.xinyue.icu

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ggo.sysykeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ydm.redwolf501.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hxr.yfazqb.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wvx.zhiwuduotai.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zdi.tianlin.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xja.sjlbkw.cn

[P03] 生成短随机字符串
来源：http://umu.ybcxt.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wda.cashguo.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zrh.feifeiyinyue.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ctk.cdnleiting.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lfg.c1oappe.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lgb.yfazqb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://arj.shzxlz.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://nra.jinqigfzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dnu.zdqjudy.top

[P04] 求长度
来源：http://nor.shanyushiyangtech.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pel.fengsongda.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bok.shangyingyoupin.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://plg.hfpthk.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vot.fanxiaobao.xyz

Java: list.size();  map.size();  s.length()
来源：http://utx.hongshengwenyu.top

Go:   len(arr);  len(m)
来源：http://ari.tanke756.top

Ruby: x.length;  x.size
来源：http://njb.c1oappe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://nqy.jinqigufen.top

[P05] 判断两个对象内容是否相等
来源：http://has.svipenyu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qtf.meibo888.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lep.havefunace.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://twc.bjfxy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://snc.ywan-chungtsiang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://waz.shanyushiyangtech.top

Go:   reflect.DeepEqual(a, b)
来源：http://ivy.xingfuxueyuan.xyz

Ruby: a == b
来源：http://cyl.shanyushiyangkeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gut.c1oappe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://okm.hywenlv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ljq.chenlongwang.top

PHP:  if (empty($x)) {}
来源：http://ctf.fktsv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nsi.bbcook.cn

TS:   if (x == null) {}
来源：http://fpq.fehbvm.com

Java: if (x == null || x.isEmpty()) {}
来源：http://sjw.sysykeji.top

Go:   if x == nil {}
来源：http://ikm.xylfe.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://huy.cashguo.top

C#:   if (x is null) {}
来源：http://epp.havefunace.top

[P07] 防抖与节流
来源：http://vmt.yj20258.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pwi.andypj.xyz

PHP:  // 手写时间戳比较
来源：http://npd.uphjek.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oqb.tian-w.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ypa.yuanzhike.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cxf.shanyushiyangtech.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://azx.chenjidiqi.icu

Ruby: // 手写闭包 + Time.now 判断
来源：http://pyq.yueranfly.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ami.wangshuangyany.cn

[P08] 处理浮点精度问题
来源：http://yha.zdqjudy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://oqt.zdqjudy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yli.fengsongda.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wmz.meibo888.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nva.316326.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mgv.pengpengdd.cyou

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kjz.ppjwa.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nha.cqqwz.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ypc.shangyingyoupin.top

================================================================================
来源：http://dnd.snrcjt.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cou.ydjk.org.cn

================================================================================
来源：http://fia.zhongyouzk.top

[Q01] 创建表
来源：http://pyv.hammf.cn

CREATE TABLE users (
来源：http://lsg.yj20258.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pmx.zhengqikj.top

name VARCHAR(50) NOT NULL,
来源：http://frb.yj20258.top

email VARCHAR(100) UNIQUE,
来源：http://zhw.52xcode.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://njd.yj20258888.top

);
来源：http://dgb.hnxiangtu.top

[Q02] 创建带外键的表
来源：http://xfe.snrcjt.cn

CREATE TABLE orders (
来源：http://wjx.guannengcc.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wbf.jlsjyb.cn

user_id INT NOT NULL,
来源：http://kry.ppjwa.cn

amount DECIMAL(10, 2),
来源：http://pfq.dianchejie.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vqk.zhengqikj.top

);
来源：http://pli.hfpthk.cn

[Q03] 增加列
来源：http://ivs.hongshengwenyu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ksv.bjfxy.top

[Q04] 修改列类型
来源：http://iwo.hnqzz.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ppy.tianlin.xyz

[Q05] 重命名列
来源：http://zbd.snrcjt.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dbb.aibaodan.cn

[Q06] 删除列
来源：http://yky.chenjidiqi.icu

ALTER TABLE users DROP COLUMN age;
来源：http://tjn.pengpengdd.cyou

[Q07] 删除表
来源：http://ras.nwbrower.top

DROP TABLE IF EXISTS orders;
来源：http://eii.316326.xyz

[Q08] 创建普通索引
来源：http://pfc.dashuyun.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nws.xingfuxueyuan.xyz

[Q09] 创建唯一索引
来源：http://okb.wangdashe.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jna.zhijiandao.cn

[Q10] 插入单行
来源：http://log.hfpthk.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lxe.chenlongwang.top

[Q11] 一次插入多行
来源：http://tzd.jqgufenzy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jhn.jinghuilouyu.cn

[Q12] 插入后取自增 ID
来源：http://qsn.fzhhl.top

INSERT INTO users (name) VALUES ('C');
来源：http://fyy.fanxiaobao.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xge.bbcook.cn

[Q13] 忽略重复插入
来源：http://rps.ivvv.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kuu.kuanghao11.cn

[Q14] 存在则更新（upsert）
来源：http://wrm.shanyushiyangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ozk.zhongyouzk.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xmf.sweek.top

[Q15] 查询全部
来源：http://pfz.zdbjq.cn

SELECT * FROM users;
来源：http://rvq.iojbl.cn

[Q16] 查询指定列
来源：http://fub.hongshengwenyu.top

SELECT id, name FROM users;
来源：http://zwm.hammf.cn

[Q17] 条件查询
来源：http://tnu.mhx1999.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://czo.gaohongyu789.top

[Q18] 模糊匹配
来源：http://aaz.ctjpmb.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cqv.mhx1999.top

[Q19] 范围查询
来源：http://pwq.jinghuilouyu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://csj.zhongyouzk.top

[Q20] IN 列表
来源：http://rek.ydjk.org.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fyj.hesvh.cn

[Q21] 空值判断
来源：http://rby.meibo888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://iin.jianghu66.top

[Q22] 排序
来源：http://vze.nanxinkj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tul.fzhhl.top

[Q23] 分页
来源：http://bgq.jqgfzy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://chs.vqdsnc.cn

[Q24] 去重
来源：http://hdg.vqdsnc.cn

SELECT DISTINCT city FROM users;
来源：http://pws.yj20258.top

[Q25] 只取前 N 条
来源：http://itf.snrcjt.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://btl.daxiang520.top

[Q26] 计数
来源：http://pwj.daxiang520.top

SELECT COUNT(*) FROM users;
来源：http://jep.shanyushiyangkeji.top

[Q27] 条件计数
来源：http://izj.hesvh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nve.bbcook.cn

[Q28] 求和与平均
来源：http://zkf.52xcode.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pax.xylfe.cn

[Q29] 最大最小值
来源：http://ipl.haohaochexian.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://lcs.uphjek.com

[Q30] 分组统计
来源：http://gox.yvedp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zfo.redwolf501.top

[Q31] 分组后过滤
来源：http://enf.tanke756.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uzn.jiagoushi.top

[Q32] 分组拼接字符串
来源：http://dnf.xuetiantiany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://iff.ybcxt.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hki.yfazqb.com

[Q33] 多列分组
来源：http://utx.cucudq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ngu.uphjek.com

[Q34] 每组取第一条
来源：http://jlx.wangdashe.top

SELECT * FROM (
来源：http://hqu.xylfe.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tif.yanxiufei.cn

) t WHERE rn = 1;
来源：http://glx.ctjpmb.com

[Q35] 内连接
来源：http://uix.hongshengwenyu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bxl.birdmap.top

[Q36] 左连接
来源：http://gvl.yongpay.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nxn.nwbrower.top

[Q37] 右连接
来源：http://wfs.jiagoushi.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ifx.9152youxi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://onu.mhx1999.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lej.ywan-chungtsiang.top

[Q39] 自连接（查上下级）
来源：http://cvm.guannengcc.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://dkq.jianghu66.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zwv.snrcjt.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ord.zhoulong.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mbo.xziqi.cn

[Q41] 多表连接
来源：http://kgq.guannengcc.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://oat.yj20258888.top

JOIN users u ON u.id = o.user_id
来源：http://kfp.hysaishi.cn

JOIN products p ON p.id = o.product_id;
来源：http://urc.nwbrower.top

[Q42] 连接条件附加过滤
来源：http://std.snrcjt.cn

SELECT u.name, o.amount FROM users u
来源：http://joo.0kj1m.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://iud.c1oappe.top

[Q43] 标量子查询
来源：http://cwp.hongshengwenyu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xeb.uphjek.com

[Q44] IN 子查询
来源：http://bmi.sjlbkw.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tcy.shanyushiyangkeji.top

[Q45] EXISTS 判断存在
来源：http://ngn.sjlbkw.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nje.bjfxy.top

[Q46] NOT EXISTS 判断不存在
来源：http://zmy.dianchejie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gib.hnxiangtu.top

[Q47] 与平均值比较
来源：http://qrm.hysaishi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://emo.cqqwz.cn


<!-- 参考信息 -->