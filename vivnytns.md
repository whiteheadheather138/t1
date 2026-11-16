代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zop.andypj.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://dcp.yj20258888.top

TS:   // 手写 Map<string, number>
来源：http://bcv.9152youxi.cn

Java: // 手写 HashMap
来源：http://kwl.cqqwz.cn

Go:   // 手写 map[int]int
来源：http://pdt.xziqi.cn

Ruby: // 手写 Hash
来源：http://pkk.nwbrower.top

C#:   // 手写 Dictionary<int, int>
来源：http://lss.ivvv.top

[N08] 生成全排列
来源：http://hsw.zhijiandao.cn

Py:   itertools.permutations(arr)
来源：http://avu.yvedp.cn

PHP:  // 手写递归交换
来源：http://ias.bbcook.cn

JS:   // 手写回溯递归
来源：http://dym.andypj.xyz

TS:   // 手写回溯递归
来源：http://afc.xuetiantiany.cn

Java: // 手写回溯递归
来源：http://jaq.xylfe.cn

Go:   // 手写回溯递归
来源：http://vql.ybcxt.top

Ruby: arr.permutation.to_a
来源：http://mqe.xuanzx.com

C#:   // 手写回溯递归
来源：http://bbq.chenlongwang.top

[N09] 栈与队列
来源：http://xug.zhengqikj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ots.ctjpmb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://haz.dashuyun.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xdm.shangyingyoupin.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pgv.fktsv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ucr.ppjwa.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xtc.chenzaomai.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zke.pengpengdd.cyou

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qjn.jyoumei.cn

[N10] 链表节点定义
来源：http://blm.xingfuxueyuan.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cye.yuanzhike.top

PHP:  class Node { public $v; public $next = null; }
来源：http://keu.316326.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fnc.ehwqpu.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uzm.cdnleiting.top

Java: class Node { int v; Node next; }
来源：http://usz.pengpengdd.cyou

Go:   type Node struct { V int; Next *Node }
来源：http://yhi.jinghuilouyu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bob.316326.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://fig.jiagoushi.top

[N11] 二叉树中序遍历
来源：http://cee.fzhhl.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pbq.epnwcf.com

PHP:  // 手写递归函数
来源：http://bwn.pengpengdd.cyou

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pao.sweek.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://doz.xuetiantiany.cn

Java: // 手写递归
来源：http://wtg.xziqi.cn

Go:   // 手写递归
来源：http://rjk.haohaochexian.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ukw.sxryk.cn

C#:   // 手写递归
来源：http://flq.gogol.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qui.yongpay.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://aap.smart0.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vau.daria6918.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wws.316326.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uis.yuanzhike.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bhy.nanxuanxn.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vaa.tianlin.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rtv.haohaochexian.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ibh.yueranfly.top

================================================================================
来源：http://vbk.aibaodan.cn

O. 并发与异步
来源：http://fvb.redwolf501.top

================================================================================
来源：http://ymh.0kj1m.cn

[O01] 启动一个线程
来源：http://lzo.gotoacloud.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dde.dianchejie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dcd.havefunace.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yex.cheryme.top

TS:   // 同 JS
来源：http://kdi.bbcook.cn

Java: new Thread(() -> f()).start()
来源：http://cxj.cucudq.cn

Go:   go f()
来源：http://yfp.fktsv.cn

Ruby: Thread.new { f }
来源：http://vpx.shanyushiyangkeji.top

C#:   Task.Run(() => F());
来源：http://uri.jyoumei.cn

[O02] 使用线程池
来源：http://uqm.mhx1999.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eic.yueranfly.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vvf.jianghu66.top

JS:   // worker_threads 线程池
来源：http://jdk.smart0.xyz

TS:   // worker_threads 线程池
来源：http://tel.yj20258888.top

Java: Executors.newFixedThreadPool(4)
来源：http://kkt.zycfv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zmd.cheryme.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vyi.vehdjk.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uow.9152youxi.cn

[O03] 加锁保护共享数据
来源：http://uba.sxryk.cn

Py:   with lock: shared += 1
来源：http://sob.yuxming.cn

PHP:  // 用 flock() 做文件锁
来源：http://jhk.tanke756.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://oug.hnxiangtu.top

TS:   // 同 JS
来源：http://whu.ppjwa.cn

Java: synchronized (this) { shared++; }
来源：http://iro.cheryme.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qcj.ywan-chungtsiang.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ofl.mhx1999.top

C#:   lock (gate) { shared++; }
来源：http://juv.sweek.top

[O04] 定义异步函数并等待
来源：http://koo.tianlin.xyz

Py:   async def f():⏎    await g()
来源：http://cko.nanxuanxn.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bsa.redwolf501.top

JS:   async function f() { await g(); }
来源：http://wgg.hysaishi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://buj.epnwcf.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yem.hesvh.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qbo.yangfankeji.com

Ruby: # 用 Fiber 或 async gem
来源：http://tpf.wangshuangyany.cn

C#:   async Task F() { await G(); }
来源：http://kcy.jinyuanbaomall.cn

[O05] 并发执行并等待全部完成
来源：http://xet.316326.xyz

Py:   asyncio.gather(*tasks)
来源：http://dju.guowangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vrg.cdnleiting.top

JS:   await Promise.all(tasks)
来源：http://nbh.svipenyu.cn

TS:   await Promise.all(tasks)
来源：http://qyx.ivvv.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kxa.vehdjk.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kbv.fktsv.cn

Ruby: threads.map(&:join)
来源：http://mhw.guowangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fcu.yanxiufei.cn

[O06] 使用进程池
来源：http://bmy.iojbl.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qph.hesvh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jch.bbcook.cn

JS:   // child_process / cluster 模块
来源：http://ptr.0kj1m.cn

TS:   // child_process / cluster 模块
来源：http://wyy.meibo888.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sdg.gaohongyu789.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bea.cucudq.cn

Ruby: // fork 块
来源：http://bdq.xinyue.icu

C#:   Parallel.For
来源：http://yut.xylfe.cn

================================================================================
来源：http://wau.uphjek.com

P. 常用工具函数
来源：http://wsh.ywan-chungtsiang.top

================================================================================
来源：http://soo.jlsjyb.cn

[P01] 生成 UUID
来源：http://iud.cucudq.cn

Py:   str(uuid.uuid4())
来源：http://mqz.jinqigfzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qxu.bjfxy.top

JS:   crypto.randomUUID()
来源：http://egw.zhengqikj.top

TS:   crypto.randomUUID()
来源：http://dha.nanxinkj.top

Java: UUID.randomUUID().toString()
来源：http://fgm.bbcook.cn

Go:   // 用 github.com/google/uuid
来源：http://kxl.fengsongda.top

Ruby: SecureRandom.uuid
来源：http://gwj.jinyuanbaomall.cn

C#:   Guid.NewGuid().ToString()
来源：http://qfm.pycfn.com

[P02] MD5 / SHA256 摘要
来源：http://guk.hammf.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cnt.52xcode.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ztt.sufxvd.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dmm.jianghu66.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dvi.guannengcc.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ddt.xuetiantiany.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mft.fengsongda.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xmd.gogol.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gle.uphjek.com

[P03] 生成短随机字符串
来源：http://agy.fanxiaobao.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://twz.xziqi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jkz.0kj1m.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://and.daria6918.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lif.hcnkem.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://art.ctjpmb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qgl.gzhubu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://fbc.chenzaomai.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jtp.snrcjt.cn

[P04] 求长度
来源：http://gap.sufxvd.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lgm.pycfn.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nbu.cucudq.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wtm.tian-w.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fik.bjfxy.top

Java: list.size();  map.size();  s.length()
来源：http://alj.yj20258888.top

Go:   len(arr);  len(m)
来源：http://cbv.vqdsnc.cn

Ruby: x.length;  x.size
来源：http://tzm.wangdashe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://eer.gotoacloud.top

[P05] 判断两个对象内容是否相等
来源：http://ciz.iojbl.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yvn.quarkkingdee.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sgq.yvedp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://muf.ppjwa.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qrj.yfazqb.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uwu.c1oappe.top

Go:   reflect.DeepEqual(a, b)
来源：http://koa.cqqwz.cn

Ruby: a == b
来源：http://ndj.daxiang520.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wcd.guowangkeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tjk.hesvh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ltu.daxiang520.top

PHP:  if (empty($x)) {}
来源：http://aud.fengsongda.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ydh.yuanzhike.top

TS:   if (x == null) {}
来源：http://aol.xylfe.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mnm.jinqigufen.top

Go:   if x == nil {}
来源：http://vyt.shuidangran.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://atz.hongshengwenyu.top

C#:   if (x is null) {}
来源：http://kwd.ppjwa.cn

[P07] 防抖与节流
来源：http://iea.havefunace.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oar.cashguo.top

PHP:  // 手写时间戳比较
来源：http://zai.vqdsnc.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aml.nanxinkj.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sgz.bbcook.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://aiv.shuidangran.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xeq.316326.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://xig.shanyushiyangtech.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fiy.yj202588.top

[P08] 处理浮点精度问题
来源：http://jrx.mhx1999.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qkt.hammf.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://osl.daria6918.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fwp.andypj.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lhv.nwbrower.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wlo.shzxlz.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rcj.yanxiufei.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yxh.sufxvd.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lxi.zycfv.cn

================================================================================
来源：http://ady.cucudq.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ecb.epnwcf.com

================================================================================
来源：http://uiu.jianghu66.top

[Q01] 创建表
来源：http://wqg.chenjidiqi.icu

CREATE TABLE users (
来源：http://cet.wangdashe.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nin.redwolf501.top

name VARCHAR(50) NOT NULL,
来源：http://bpg.tian-w.cn

email VARCHAR(100) UNIQUE,
来源：http://hrz.jqgufenzy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://usn.ppjwa.cn

);
来源：http://twn.zhiwuduotai.top

[Q02] 创建带外键的表
来源：http://wgz.gaohongyu789.top

CREATE TABLE orders (
来源：http://oub.jqgufenzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wzt.guowangkeji.top

user_id INT NOT NULL,
来源：http://zsk.meibo888.top

amount DECIMAL(10, 2),
来源：http://ven.daria6918.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jjx.zhijiandao.cn

);
来源：http://nwn.cdnleiting.top

[Q03] 增加列
来源：http://rld.dianchejie.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mrs.redwolf501.top

[Q04] 修改列类型
来源：http://hdi.yueranfly.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wlf.jinqigfzy.top

[Q05] 重命名列
来源：http://nzu.gogol.net.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ymd.yuxming.cn

[Q06] 删除列
来源：http://pli.xziqi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qmi.mhx1999.top

[Q07] 删除表
来源：http://hgk.yvedp.cn

DROP TABLE IF EXISTS orders;
来源：http://qxz.quarkkingdee.top

[Q08] 创建普通索引
来源：http://vwx.hysaishi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ymx.zycfv.cn

[Q09] 创建唯一索引
来源：http://ldz.jyoumei.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kvi.fengsongda.top

[Q10] 插入单行
来源：http://dto.0kj1m.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ota.ydzc1.top

[Q11] 一次插入多行
来源：http://nvl.daxiang520.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tbp.fanxiaobao.xyz

[Q12] 插入后取自增 ID
来源：http://gmr.ywan-chungtsiang.top

INSERT INTO users (name) VALUES ('C');
来源：http://dlp.xingfuxueyuan.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wsy.gzhubu.top

[Q13] 忽略重复插入
来源：http://gpl.hongshengwenyu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://eyn.hcnkem.com

[Q14] 存在则更新（upsert）
来源：http://teh.ydjk.org.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xra.hnqzz.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://phk.aibaodan.cn

[Q15] 查询全部
来源：http://aci.svipenyu.cn

SELECT * FROM users;
来源：http://wld.sufxvd.cn

[Q16] 查询指定列
来源：http://llg.ctjpmb.com

SELECT id, name FROM users;
来源：http://sjn.uphjek.com

[Q17] 条件查询
来源：http://hgh.bjfxy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://giv.fehbvm.com

[Q18] 模糊匹配
来源：http://nge.9152youxi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kyo.shangyingyoupin.top

[Q19] 范围查询
来源：http://ruz.ydjk.org.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hlu.fzhhl.top

[Q20] IN 列表
来源：http://wip.jianghu66.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tsh.jinqigfzy.top

[Q21] 空值判断
来源：http://agc.yongpay.top

SELECT * FROM users WHERE email IS NULL;
来源：http://jzn.fengsongda.top

[Q22] 排序
来源：http://cix.meibo888.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rvp.feifeiyinyue.top

[Q23] 分页
来源：http://frv.xingfuxueyuan.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mar.wangshuangyany.cn

[Q24] 去重
来源：http://ypc.tanke756.top

SELECT DISTINCT city FROM users;
来源：http://xod.cashguo.top

[Q25] 只取前 N 条
来源：http://jrf.jiagoushi.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://iff.chenzaomai.com

[Q26] 计数
来源：http://xni.meibo888.top

SELECT COUNT(*) FROM users;
来源：http://bdt.hywenlv.cn

[Q27] 条件计数
来源：http://rvf.yvedp.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rej.fktsv.cn

[Q28] 求和与平均
来源：http://iym.fehbvm.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://epx.jinqigfzy.top

[Q29] 最大最小值
来源：http://urt.jqgufenzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://wyk.fehbvm.com

[Q30] 分组统计
来源：http://lir.dianchejie.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ebg.gogol.net.cn

[Q31] 分组后过滤
来源：http://mim.zhaomingkeji.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jqa.yvedp.cn

[Q32] 分组拼接字符串
来源：http://rcl.jinqigufen.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://opx.xylfe.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jcb.hywenlv.cn

[Q33] 多列分组
来源：http://hym.wangshuangyany.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oql.sweek.top

[Q34] 每组取第一条
来源：http://upo.shangyingyoupin.top

SELECT * FROM (
来源：http://gnh.meibo888.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://reb.0kj1m.cn

) t WHERE rn = 1;
来源：http://hdf.wangdashe.top

[Q35] 内连接
来源：http://ejm.shangyingyoupin.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://iqs.hnxiangtu.top

[Q36] 左连接
来源：http://olm.hnqzz.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mpz.ehwqpu.com

[Q37] 右连接
来源：http://bru.bjfxy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pzm.nanxuanxn.top

[Q38] 全外连接（PostgreSQL）
来源：http://gbn.aibaodan.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lkz.zycfv.cn

[Q39] 自连接（查上下级）
来源：http://amh.ppjwa.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lub.9152youxi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wac.c1oappe.top

[Q40] 交叉连接（笛卡尔积）
来源：http://tyi.mhx1999.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jaf.wangdashe.top

[Q41] 多表连接
来源：http://lbv.tianlin.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://upg.fzhhl.top

JOIN users u ON u.id = o.user_id
来源：http://fob.daria6918.cn

JOIN products p ON p.id = o.product_id;
来源：http://vcm.zycfv.cn

[Q42] 连接条件附加过滤
来源：http://ooz.gaohongyu789.top

SELECT u.name, o.amount FROM users u
来源：http://uju.yvedp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cwy.hcnkem.com

[Q43] 标量子查询
来源：http://czj.aizwys.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cva.bbcook.cn

[Q44] IN 子查询
来源：http://fci.jinghuilouyu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bux.xylfe.cn

[Q45] EXISTS 判断存在
来源：http://udj.mhx1999.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pke.chenzaomai.com

[Q46] NOT EXISTS 判断不存在
来源：http://gdw.nwbrower.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pjq.meibo888.top

[Q47] 与平均值比较
来源：http://ehx.daria6918.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://krp.jqgufenzy.top


<!-- 参考信息 -->