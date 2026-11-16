代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ohn.svipenyu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://edr.cqqwz.cn

TS:   // 手写 Map<string, number>
来源：http://diw.jinqigufen.top

Java: // 手写 HashMap
来源：http://qza.yvedp.cn

Go:   // 手写 map[int]int
来源：http://ksr.shzxlz.cn

Ruby: // 手写 Hash
来源：http://qql.xziqi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hph.andypj.xyz

[N08] 生成全排列
来源：http://niw.jianghu66.top

Py:   itertools.permutations(arr)
来源：http://kuc.fktsv.cn

PHP:  // 手写递归交换
来源：http://kbx.vqdsnc.cn

JS:   // 手写回溯递归
来源：http://xtz.tanke756.top

TS:   // 手写回溯递归
来源：http://lma.jinyuanbaomall.cn

Java: // 手写回溯递归
来源：http://non.jqgufenzy.top

Go:   // 手写回溯递归
来源：http://pkv.nanxinkj.top

Ruby: arr.permutation.to_a
来源：http://ffa.hcnkem.com

C#:   // 手写回溯递归
来源：http://out.9152youxi.cn

[N09] 栈与队列
来源：http://nfm.tanke756.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fuh.fehbvm.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mdr.nanxinkj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hti.xinyue.icu

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gah.fktsv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wld.vqdsnc.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://smp.gzhubu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bth.zhiwuduotai.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jyg.jinghuilouyu.cn

[N10] 链表节点定义
来源：http://pvg.vehdjk.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ojr.yanxiufei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qli.zhixingplan.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ndj.jinyuanbaomall.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pti.andypj.xyz

Java: class Node { int v; Node next; }
来源：http://xpr.zdqjudy.top

Go:   type Node struct { V int; Next *Node }
来源：http://pov.fktsv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://spl.316326.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://osl.feifeiyinyue.top

[N11] 二叉树中序遍历
来源：http://hev.hnxiangtu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://udp.zhijiandao.cn

PHP:  // 手写递归函数
来源：http://dxi.yueranfly.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pna.pycfn.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gwl.hnqzz.top

Java: // 手写递归
来源：http://jol.feifeiyinyue.top

Go:   // 手写递归
来源：http://won.aibaodan.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://llj.gaohongyu789.top

C#:   // 手写递归
来源：http://mki.guowangkeji.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pyl.yongpay.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ifd.yangfankeji.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cda.fehbvm.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qrf.yangfankeji.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fob.zhengqikj.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xjn.havefunace.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fsr.yuxming.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dmk.tian-w.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xkg.hywenlv.cn

================================================================================
来源：http://wmx.haohaochexian.top

O. 并发与异步
来源：http://kuj.jqgufenzy.top

================================================================================
来源：http://kit.cqqwz.cn

[O01] 启动一个线程
来源：http://oww.meibo888.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://igx.pengpengdd.cyou

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sma.0kj1m.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qdq.jlsjyb.cn

TS:   // 同 JS
来源：http://igk.aizwys.cn

Java: new Thread(() -> f()).start()
来源：http://vbe.fanxiaobao.xyz

Go:   go f()
来源：http://ewj.xuetiantiany.cn

Ruby: Thread.new { f }
来源：http://ljw.xingfuxueyuan.xyz

C#:   Task.Run(() => F());
来源：http://adr.jyoumei.cn

[O02] 使用线程池
来源：http://hxb.shanyushiyangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uuy.sweek.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cfk.ctjpmb.com

JS:   // worker_threads 线程池
来源：http://sqx.shzxlz.cn

TS:   // worker_threads 线程池
来源：http://cvw.uphjek.com

Java: Executors.newFixedThreadPool(4)
来源：http://jir.sjlbkw.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rps.jinqigfzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mwr.hammf.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vwq.yanxiufei.cn

[O03] 加锁保护共享数据
来源：http://eyo.jyoumei.cn

Py:   with lock: shared += 1
来源：http://cqk.snrcjt.cn

PHP:  // 用 flock() 做文件锁
来源：http://nnp.kuanghao11.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://owv.jqgufenzy.top

TS:   // 同 JS
来源：http://pzm.quarkkingdee.top

Java: synchronized (this) { shared++; }
来源：http://age.mhx1999.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zqa.gogol.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://aip.uphjek.com

C#:   lock (gate) { shared++; }
来源：http://cxv.sjlbkw.cn

[O04] 定义异步函数并等待
来源：http://lsw.cashguo.top

Py:   async def f():⏎    await g()
来源：http://xzq.nanxinkj.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jyg.pycfn.com

JS:   async function f() { await g(); }
来源：http://rxs.gotoacloud.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://dmk.hnxiangtu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dcw.gogol.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tpq.jqgfzy.top

Ruby: # 用 Fiber 或 async gem
来源：http://eom.dashuyun.cn

C#:   async Task F() { await G(); }
来源：http://dfa.yj20258.top

[O05] 并发执行并等待全部完成
来源：http://mpe.xuanzx.com

Py:   asyncio.gather(*tasks)
来源：http://xxt.ywan-chungtsiang.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://axw.ppjwa.cn

JS:   await Promise.all(tasks)
来源：http://fcn.gzhubu.top

TS:   await Promise.all(tasks)
来源：http://flx.fktsv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kxg.tianlin.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ydt.fanxiaobao.xyz

Ruby: threads.map(&:join)
来源：http://jaw.shangyingyoupin.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ftk.kuanghao11.cn

[O06] 使用进程池
来源：http://tge.9152youxi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gob.zhijiandao.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://iem.zycfv.cn

JS:   // child_process / cluster 模块
来源：http://nho.aizwys.cn

TS:   // child_process / cluster 模块
来源：http://wyk.daxiang520.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ajb.yfazqb.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ybf.yueranfly.top

Ruby: // fork 块
来源：http://smq.ivvv.top

C#:   Parallel.For
来源：http://oax.jyoumei.cn

================================================================================
来源：http://mlj.9152youxi.cn

P. 常用工具函数
来源：http://qej.sjlbkw.cn

================================================================================
来源：http://kpm.xinyue.icu

[P01] 生成 UUID
来源：http://gks.pengpengdd.cyou

Py:   str(uuid.uuid4())
来源：http://zim.yj202588.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://iui.xuetiantiany.cn

JS:   crypto.randomUUID()
来源：http://lpz.jinqigufen.top

TS:   crypto.randomUUID()
来源：http://psd.hnqzz.top

Java: UUID.randomUUID().toString()
来源：http://yvp.316326.xyz

Go:   // 用 github.com/google/uuid
来源：http://vfs.jiagoushi.top

Ruby: SecureRandom.uuid
来源：http://hul.52xcode.cn

C#:   Guid.NewGuid().ToString()
来源：http://gop.hnqzz.top

[P02] MD5 / SHA256 摘要
来源：http://vhv.jqgufenzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hrx.dashuyun.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hwc.birdmap.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kcg.shangyingyoupin.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pye.havefunace.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mpc.yj20258888.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rpv.dianchejie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ycw.yongpay.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kdo.cucudq.cn

[P03] 生成短随机字符串
来源：http://fnd.shuidangran.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cqr.bbcook.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://akg.wangdashe.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dsq.zdqjudy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hwc.svipenyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nwv.kuanghao11.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://whp.cqqwz.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mwu.snrcjt.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://smd.yanxiufei.cn

[P04] 求长度
来源：http://txp.aizwys.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wgh.wangshuangyany.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://imr.yuanzhike.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tpq.xylfe.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://trl.yj20258.top

Java: list.size();  map.size();  s.length()
来源：http://mlk.feifeiyinyue.top

Go:   len(arr);  len(m)
来源：http://qwh.xylfe.cn

Ruby: x.length;  x.size
来源：http://rqj.haohaochexian.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://nbl.jinyuanbaomall.cn

[P05] 判断两个对象内容是否相等
来源：http://bpe.zhiwuduotai.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://mpy.hammf.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ppn.yueranfly.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ysn.ppjwa.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bsz.hongshengwenyu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://skj.shanyushiyangkeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://qjn.jiagoushi.top

Ruby: a == b
来源：http://qoa.xinyue.icu

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://iue.cqqwz.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ani.wangdashe.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wcq.zhijiandao.cn

PHP:  if (empty($x)) {}
来源：http://wxg.jinghuilouyu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bju.yuanzhike.top

TS:   if (x == null) {}
来源：http://kbp.ehwqpu.com

Java: if (x == null || x.isEmpty()) {}
来源：http://any.c1oappe.top

Go:   if x == nil {}
来源：http://jxx.tanke756.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zij.yuanzhike.top

C#:   if (x is null) {}
来源：http://duu.shuidangran.top

[P07] 防抖与节流
来源：http://pcn.gaohongyu789.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gdh.zhongyouzk.top

PHP:  // 手写时间戳比较
来源：http://qgu.cashguo.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nst.ydzc1.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rig.yueranfly.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vdr.gogol.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bfe.bjfxy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://cmv.jlsjyb.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zqi.ywan-chungtsiang.top

[P08] 处理浮点精度问题
来源：http://mqu.haohaochexian.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ftn.fehbvm.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ofo.feifeiyinyue.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dxg.hnqzz.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ita.gogol.net.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ymi.yfazqb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ces.dianchejie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://foi.meibo888.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nfn.hnxiangtu.top

================================================================================
来源：http://rbs.guowangkeji.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cbi.bbcook.cn

================================================================================
来源：http://oke.chenjidiqi.icu

[Q01] 创建表
来源：http://ell.yuxming.cn

CREATE TABLE users (
来源：http://qsq.bjfxy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://czu.hesvh.cn

name VARCHAR(50) NOT NULL,
来源：http://tyq.nanxinkj.top

email VARCHAR(100) UNIQUE,
来源：http://ppc.gogol.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://aeq.ywan-chungtsiang.top

);
来源：http://owp.hnxiangtu.top

[Q02] 创建带外键的表
来源：http://yhw.xuetiantiany.cn

CREATE TABLE orders (
来源：http://zwi.svipenyu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://brh.pengpengdd.cyou

user_id INT NOT NULL,
来源：http://umy.fengsongda.top

amount DECIMAL(10, 2),
来源：http://eyh.zdbjq.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bwx.fengsongda.top

);
来源：http://iit.aizwys.cn

[Q03] 增加列
来源：http://vfu.zdqjudy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rvt.yvedp.cn

[Q04] 修改列类型
来源：http://lsw.sweek.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://thv.guowangkeji.top

[Q05] 重命名列
来源：http://pqv.daria6918.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://urd.jqgfzy.top

[Q06] 删除列
来源：http://zxo.nanxuanxn.top

ALTER TABLE users DROP COLUMN age;
来源：http://wvz.yvedp.cn

[Q07] 删除表
来源：http://xrn.fzhhl.top

DROP TABLE IF EXISTS orders;
来源：http://zkn.uphjek.com

[Q08] 创建普通索引
来源：http://knq.tianlin.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://epr.jlsjyb.cn

[Q09] 创建唯一索引
来源：http://jte.bbcook.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://spw.dianchejie.cn

[Q10] 插入单行
来源：http://ykt.xinyue.icu

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sqm.ybcxt.top

[Q11] 一次插入多行
来源：http://rmm.gogol.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ufb.wangdashe.top

[Q12] 插入后取自增 ID
来源：http://xnl.kuanghao11.cn

INSERT INTO users (name) VALUES ('C');
来源：http://tgd.hfpthk.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bez.0kj1m.cn

[Q13] 忽略重复插入
来源：http://okz.pycfn.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kgk.wangdashe.top

[Q14] 存在则更新（upsert）
来源：http://hol.daria6918.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://urd.zhengqikj.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tzs.nwbrower.top

[Q15] 查询全部
来源：http://oaf.tanke756.top

SELECT * FROM users;
来源：http://zhf.jqgfzy.top

[Q16] 查询指定列
来源：http://sdm.gaohongyu789.top

SELECT id, name FROM users;
来源：http://iio.jinyuanbaomall.cn

[Q17] 条件查询
来源：http://ykq.hcnkem.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xuv.jlsjyb.cn

[Q18] 模糊匹配
来源：http://yvu.zhongyouzk.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ubl.dianchejie.cn

[Q19] 范围查询
来源：http://vny.hnqzz.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://txq.dianchejie.cn

[Q20] IN 列表
来源：http://kky.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hbi.xingfuxueyuan.xyz

[Q21] 空值判断
来源：http://jed.yueranfly.top

SELECT * FROM users WHERE email IS NULL;
来源：http://dzm.hcnkem.com

[Q22] 排序
来源：http://zoz.shanyushiyangtech.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ujx.ydzc1.top

[Q23] 分页
来源：http://kvg.jinqigufen.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://aes.snrcjt.cn

[Q24] 去重
来源：http://qmq.wangshuangyany.cn

SELECT DISTINCT city FROM users;
来源：http://smm.fzhhl.top

[Q25] 只取前 N 条
来源：http://fkb.feifeiyinyue.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tsg.nwbrower.top

[Q26] 计数
来源：http://frv.tarul.cn

SELECT COUNT(*) FROM users;
来源：http://qkr.cucudq.cn

[Q27] 条件计数
来源：http://ifm.mhx1999.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://quo.shanyushiyangtech.top

[Q28] 求和与平均
来源：http://hpq.zycfv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://svp.yuanzhike.top

[Q29] 最大最小值
来源：http://stk.kuanghao11.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ymy.zhiwuduotai.top

[Q30] 分组统计
来源：http://cvo.hongshengwenyu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fae.c1oappe.top

[Q31] 分组后过滤
来源：http://fdw.sweek.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fja.pycfn.com

[Q32] 分组拼接字符串
来源：http://bmw.guannengcc.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ies.jqgufenzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://djz.hywenlv.cn

[Q33] 多列分组
来源：http://ify.ctjpmb.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ngt.hcnkem.com

[Q34] 每组取第一条
来源：http://exh.ybcxt.top

SELECT * FROM (
来源：http://dcc.zhijiandao.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ekz.shanyushiyangtech.top

) t WHERE rn = 1;
来源：http://uyl.xziqi.cn

[Q35] 内连接
来源：http://vaa.guowangkeji.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kmp.aibaodan.cn

[Q36] 左连接
来源：http://plt.jinqigufen.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jwj.nanxinkj.top

[Q37] 右连接
来源：http://fgo.tian-w.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://szy.jyoumei.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dlk.zdbjq.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ace.c1oappe.top

[Q39] 自连接（查上下级）
来源：http://enj.chenjidiqi.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://gep.wangshuangyany.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wfh.snrcjt.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pnw.jlsjyb.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://udz.dashuyun.cn

[Q41] 多表连接
来源：http://qhl.tarul.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rbt.xylfe.cn

JOIN users u ON u.id = o.user_id
来源：http://ebq.sysykeji.top

JOIN products p ON p.id = o.product_id;
来源：http://pvw.gaohongyu789.top

[Q42] 连接条件附加过滤
来源：http://hxu.yfazqb.com

SELECT u.name, o.amount FROM users u
来源：http://jqo.hywenlv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ulf.chenlongwang.top

[Q43] 标量子查询
来源：http://pru.yj20258888.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://aks.xylfe.cn

[Q44] IN 子查询
来源：http://tlo.hywenlv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hui.zhixingplan.top

[Q45] EXISTS 判断存在
来源：http://rjt.gaohongyu789.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://opk.jlsjyb.cn

[Q46] NOT EXISTS 判断不存在
来源：http://phh.haohaochexian.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ltz.xylfe.cn

[Q47] 与平均值比较
来源：http://hvt.hesvh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kkw.yfazqb.com


<!-- 参考信息 -->