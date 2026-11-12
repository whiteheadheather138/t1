代发 wailian999

Go:   // 手写 map[int]int
来源：http://rgk.gzhubu.top

Ruby: // 手写 Hash
来源：http://ize.cqqwz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://uxa.vehdjk.com

[N08] 生成全排列
来源：http://ido.yvedp.cn

Py:   itertools.permutations(arr)
来源：http://ulx.cdnleiting.top

PHP:  // 手写递归交换
来源：http://rlo.gogol.net.cn

JS:   // 手写回溯递归
来源：http://zzm.mhx1999.top

TS:   // 手写回溯递归
来源：http://wge.gaohongyu789.top

Java: // 手写回溯递归
来源：http://dba.xziqi.cn

Go:   // 手写回溯递归
来源：http://wdc.yfazqb.com

Ruby: arr.permutation.to_a
来源：http://cca.svipenyu.cn

C#:   // 手写回溯递归
来源：http://exc.yuanzhike.top

[N09] 栈与队列
来源：http://xyp.haohaochexian.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://upe.havefunace.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mww.chenlongwang.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://etb.snrcjt.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tgw.sufxvd.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xwy.ywan-chungtsiang.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tls.snrcjt.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kjv.wangdashe.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eps.wangdashe.top

[N10] 链表节点定义
来源：http://ert.shzxlz.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rxx.fanxiaobao.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://tjz.zhongyouzk.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rnj.pengpengdd.cyou

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ykd.zhiwuduotai.top

Java: class Node { int v; Node next; }
来源：http://htb.dianchejie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vor.smart0.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://odu.shzxlz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xap.kuanghao11.cn

[N11] 二叉树中序遍历
来源：http://rhv.sufxvd.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://meg.jqgufenzy.top

PHP:  // 手写递归函数
来源：http://icn.hongshengwenyu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hgr.gzhubu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://arw.xinyue.icu

Java: // 手写递归
来源：http://ltx.jqgfzy.top

Go:   // 手写递归
来源：http://lhz.hesvh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oqm.hfpthk.cn

C#:   // 手写递归
来源：http://vrj.mhx1999.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ejt.feifeiyinyue.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tpw.svipenyu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cen.meibo888.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ker.hongshengwenyu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tjg.xziqi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uyp.hfpthk.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rfx.haohaochexian.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jek.ppjwa.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://whf.feifeiyinyue.top

================================================================================
来源：http://ayn.hywenlv.cn

O. 并发与异步
来源：http://dgk.c1oappe.top

================================================================================
来源：http://zrt.jlsjyb.cn

[O01] 启动一个线程
来源：http://lth.chenjidiqi.icu

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lzy.yj20258888.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mxq.0kj1m.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zqu.sjlbkw.cn

TS:   // 同 JS
来源：http://ojh.wangshuangyany.cn

Java: new Thread(() -> f()).start()
来源：http://guw.jiagoushi.top

Go:   go f()
来源：http://uio.ppjwa.cn

Ruby: Thread.new { f }
来源：http://gzr.daxiang520.top

C#:   Task.Run(() => F());
来源：http://hnu.nanxuanxn.top

[O02] 使用线程池
来源：http://tex.jianghu66.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bsp.gaohongyu789.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ani.jinyuanbaomall.cn

JS:   // worker_threads 线程池
来源：http://oto.xylfe.cn

TS:   // worker_threads 线程池
来源：http://qoz.yueranfly.top

Java: Executors.newFixedThreadPool(4)
来源：http://dmd.nanxuanxn.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kvx.gogol.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ypv.kuanghao11.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://txt.yfazqb.com

[O03] 加锁保护共享数据
来源：http://plf.yangfankeji.com

Py:   with lock: shared += 1
来源：http://adj.aizwys.cn

PHP:  // 用 flock() 做文件锁
来源：http://qmm.zdbjq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dns.cashguo.top

TS:   // 同 JS
来源：http://xcg.cucudq.cn

Java: synchronized (this) { shared++; }
来源：http://nxu.hammf.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://egg.9152youxi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://udh.9152youxi.cn

C#:   lock (gate) { shared++; }
来源：http://aas.yj202588.top

[O04] 定义异步函数并等待
来源：http://cqa.meibo888.top

Py:   async def f():⏎    await g()
来源：http://lhp.guannengcc.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ood.snrcjt.cn

JS:   async function f() { await g(); }
来源：http://mzm.hammf.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://oeq.zdbjq.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tpe.zhixingplan.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lak.hywenlv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zgo.hammf.cn

C#:   async Task F() { await G(); }
来源：http://vac.tanke756.top

[O05] 并发执行并等待全部完成
来源：http://uzm.cdnleiting.top

Py:   asyncio.gather(*tasks)
来源：http://goy.daria6918.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://esw.yangfankeji.com

JS:   await Promise.all(tasks)
来源：http://jfa.yj202588.top

TS:   await Promise.all(tasks)
来源：http://lcl.snrcjt.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hbc.sysykeji.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nmz.ehwqpu.com

Ruby: threads.map(&:join)
来源：http://zsw.dianchejie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jjt.fktsv.cn

[O06] 使用进程池
来源：http://slo.yuanzhike.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nkb.zycfv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ztw.jlsjyb.cn

JS:   // child_process / cluster 模块
来源：http://glr.bbcook.cn

TS:   // child_process / cluster 模块
来源：http://uyw.cdnleiting.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://prb.ivvv.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jqy.tian-w.cn

Ruby: // fork 块
来源：http://pbu.jinghuilouyu.cn

C#:   Parallel.For
来源：http://jjg.gaohongyu789.top

================================================================================
来源：http://nit.xuanzx.com

P. 常用工具函数
来源：http://hie.xylfe.cn

================================================================================
来源：http://kkt.hfpthk.cn

[P01] 生成 UUID
来源：http://xhh.ydzc1.top

Py:   str(uuid.uuid4())
来源：http://exs.gotoacloud.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oej.cucudq.cn

JS:   crypto.randomUUID()
来源：http://dqb.aibaodan.cn

TS:   crypto.randomUUID()
来源：http://qxu.zhaomingkeji.xyz

Java: UUID.randomUUID().toString()
来源：http://ujp.zhengqikj.top

Go:   // 用 github.com/google/uuid
来源：http://rej.hysaishi.cn

Ruby: SecureRandom.uuid
来源：http://xdq.guowangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://kvx.wangdashe.top

[P02] MD5 / SHA256 摘要
来源：http://eou.sxryk.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://waa.yangfankeji.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://iqe.shangyingyoupin.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wht.aizwys.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ivr.fehbvm.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wux.xuanzx.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zro.52xcode.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zcm.sxryk.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://req.pycfn.com

[P03] 生成短随机字符串
来源：http://acm.ydzc1.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rei.havefunace.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pfp.0kj1m.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://syw.hcnkem.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zvy.yj20258888.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zni.yj20258.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sqb.fzhhl.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://nvw.iojbl.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uvs.tianlin.xyz

[P04] 求长度
来源：http://ana.jiagoushi.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vem.yfazqb.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eix.yongpay.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://til.xinyue.icu

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fhg.shangyingyoupin.top

Java: list.size();  map.size();  s.length()
来源：http://mld.vqdsnc.cn

Go:   len(arr);  len(m)
来源：http://qky.jiagoushi.top

Ruby: x.length;  x.size
来源：http://hls.ppjwa.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bff.daria6918.cn

[P05] 判断两个对象内容是否相等
来源：http://uvz.nanxuanxn.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://cvz.redwolf501.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dus.uphjek.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dgn.ybcxt.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eoy.ywan-chungtsiang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vch.xylfe.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wqb.zdbjq.cn

Ruby: a == b
来源：http://fpn.daxiang520.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kee.iojbl.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uzz.sweek.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vzm.fanxiaobao.xyz

PHP:  if (empty($x)) {}
来源：http://uad.hywenlv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dea.fehbvm.com

TS:   if (x == null) {}
来源：http://yuu.guowangkeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://vik.bjfxy.top

Go:   if x == nil {}
来源：http://yzv.cqqwz.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yro.fzhhl.top

C#:   if (x is null) {}
来源：http://ssy.aibaodan.cn

[P07] 防抖与节流
来源：http://ltb.epnwcf.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vun.wangshuangyany.cn

PHP:  // 手写时间戳比较
来源：http://ope.yj20258.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://omc.zdbjq.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wdp.jinyuanbaomall.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://abi.sxryk.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ztd.gzhubu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ryg.hnqzz.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lib.xingfuxueyuan.xyz

[P08] 处理浮点精度问题
来源：http://xzp.xylfe.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yaq.meibo888.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cet.vqdsnc.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nkv.zhaomingkeji.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pcy.chenjidiqi.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oum.zhaomingkeji.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ixv.yfazqb.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jsk.tanke756.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wwk.vqdsnc.cn

================================================================================
来源：http://lrg.ppjwa.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cly.uphjek.com

================================================================================
来源：http://nls.quarkkingdee.top

[Q01] 创建表
来源：http://bhm.ydzc1.top

CREATE TABLE users (
来源：http://ayx.andypj.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jfi.yonumen.top

name VARCHAR(50) NOT NULL,
来源：http://bzq.meibo888.top

email VARCHAR(100) UNIQUE,
来源：http://lnw.quarkkingdee.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://znq.hammf.cn

);
来源：http://xiu.sjlbkw.cn

[Q02] 创建带外键的表
来源：http://slg.tian-w.cn

CREATE TABLE orders (
来源：http://kiy.xziqi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hkr.jlsjyb.cn

user_id INT NOT NULL,
来源：http://kfx.hnxiangtu.top

amount DECIMAL(10, 2),
来源：http://rkl.9152youxi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sfn.ybcxt.top

);
来源：http://xyo.vqdsnc.cn

[Q03] 增加列
来源：http://mpe.haohaochexian.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ici.zhoulong.xyz

[Q04] 修改列类型
来源：http://kay.sweek.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ktv.hywenlv.cn

[Q05] 重命名列
来源：http://pas.zdbjq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://soq.wangshuangyany.cn

[Q06] 删除列
来源：http://yyl.nanxinkj.top

ALTER TABLE users DROP COLUMN age;
来源：http://krk.epnwcf.com

[Q07] 删除表
来源：http://sfv.daxiang520.top

DROP TABLE IF EXISTS orders;
来源：http://bzq.0kj1m.cn

[Q08] 创建普通索引
来源：http://yuu.jianghu66.top

CREATE INDEX idx_users_email ON users(email);
来源：http://nec.yj20258888.top

[Q09] 创建唯一索引
来源：http://phi.ydjk.org.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://drd.hysaishi.cn

[Q10] 插入单行
来源：http://bsz.birdmap.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dbu.nwbrower.top

[Q11] 一次插入多行
来源：http://imp.hywenlv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://knq.aizwys.cn

[Q12] 插入后取自增 ID
来源：http://qbd.nanxinkj.top

INSERT INTO users (name) VALUES ('C');
来源：http://zwh.quarkkingdee.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mqh.iojbl.cn

[Q13] 忽略重复插入
来源：http://mht.shangyingyoupin.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ssf.gaohongyu789.top

[Q14] 存在则更新（upsert）
来源：http://lzf.yj202588.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yay.nanxuanxn.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yat.zhongyouzk.top

[Q15] 查询全部
来源：http://wlh.9152youxi.cn

SELECT * FROM users;
来源：http://esl.xuanzx.com

[Q16] 查询指定列
来源：http://hlm.guannengcc.top

SELECT id, name FROM users;
来源：http://rex.uphjek.com

[Q17] 条件查询
来源：http://ezk.nwbrower.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hqe.wangdashe.top

[Q18] 模糊匹配
来源：http://jhe.0kj1m.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://npf.zycfv.cn

[Q19] 范围查询
来源：http://wzm.cucudq.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://eyi.zycfv.cn

[Q20] IN 列表
来源：http://xpr.yj202588.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dwn.epnwcf.com

[Q21] 空值判断
来源：http://ksk.xingfuxueyuan.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://wvo.hfpthk.cn

[Q22] 排序
来源：http://yuu.jiagoushi.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xxz.yj20258888.top

[Q23] 分页
来源：http://yuv.cqqwz.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qdt.52xcode.cn

[Q24] 去重
来源：http://jot.sweek.top

SELECT DISTINCT city FROM users;
来源：http://msm.iojbl.cn

[Q25] 只取前 N 条
来源：http://qux.316326.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qnu.cqqwz.cn

[Q26] 计数
来源：http://rcd.yanxiufei.cn

SELECT COUNT(*) FROM users;
来源：http://mvo.guannengcc.top

[Q27] 条件计数
来源：http://gsb.sysykeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yjm.hfpthk.cn

[Q28] 求和与平均
来源：http://vxa.jlsjyb.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oob.feifeiyinyue.top

[Q29] 最大最小值
来源：http://bks.havefunace.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://coc.yuanzhike.top

[Q30] 分组统计
来源：http://vci.meibo888.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bat.zhengqikj.top

[Q31] 分组后过滤
来源：http://djk.dashuyun.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://aes.c1oappe.top

[Q32] 分组拼接字符串
来源：http://iyl.yj20258888.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fjn.aizwys.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://eaj.snrcjt.cn

[Q33] 多列分组
来源：http://jue.fzhhl.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mdl.ybcxt.top

[Q34] 每组取第一条
来源：http://lid.jlsjyb.cn

SELECT * FROM (
来源：http://cox.hysaishi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ftl.ydzc1.top

) t WHERE rn = 1;
来源：http://uaa.cucudq.cn

[Q35] 内连接
来源：http://prs.epnwcf.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lol.guannengcc.top

[Q36] 左连接
来源：http://gzh.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bof.316326.xyz

[Q37] 右连接
来源：http://rev.vqdsnc.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nwy.andypj.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://cdj.aibaodan.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pjw.yanxiufei.cn

[Q39] 自连接（查上下级）
来源：http://nfi.yuxming.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xbx.snrcjt.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://snu.ppjwa.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://chy.ybcxt.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sus.yangfankeji.com

[Q41] 多表连接
来源：http://vga.sweek.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://tgt.yj20258888.top

JOIN users u ON u.id = o.user_id
来源：http://wvq.gaohongyu789.top

JOIN products p ON p.id = o.product_id;
来源：http://lrw.yj20258.top

[Q42] 连接条件附加过滤
来源：http://gdy.ctjpmb.com

SELECT u.name, o.amount FROM users u
来源：http://bxh.bbcook.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rcg.sxryk.cn

[Q43] 标量子查询
来源：http://ixe.birdmap.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://byl.zhongyouzk.top

[Q44] IN 子查询
来源：http://lzs.fengsongda.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gcz.tanke756.top

[Q45] EXISTS 判断存在
来源：http://cob.hesvh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://saj.nwbrower.top

[Q46] NOT EXISTS 判断不存在
来源：http://bnr.cashguo.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uxk.svipenyu.cn

[Q47] 与平均值比较
来源：http://wjn.9152youxi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gke.andypj.xyz

[Q48] CTE 公用表表达式
来源：http://ppn.zhengqikj.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lgm.yonumen.top

SELECT * FROM t WHERE c > 5;
来源：http://gzf.bjfxy.top

[Q49] 更新单行
来源：http://svw.aibaodan.cn


<!-- 参考信息 -->