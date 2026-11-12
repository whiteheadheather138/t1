代发 wailian999

Java: // 手写回溯递归
来源：http://lbt.bjfxy.top

Go:   // 手写回溯递归
来源：http://omi.yj202588.top

Ruby: arr.permutation.to_a
来源：http://kyi.xziqi.cn

C#:   // 手写回溯递归
来源：http://vlq.cqqwz.cn

[N09] 栈与队列
来源：http://beu.hywenlv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yvr.chenlongwang.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ils.iojbl.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uno.quarkkingdee.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uws.0kj1m.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://epo.jqgfzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xkk.meibo888.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jqt.ydzc1.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zit.zhaomingkeji.xyz

[N10] 链表节点定义
来源：http://cdh.dashuyun.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mzh.jiagoushi.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ikc.hnqzz.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ncs.yj20258888.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vgy.cheryme.top

Java: class Node { int v; Node next; }
来源：http://rza.zhengqikj.top

Go:   type Node struct { V int; Next *Node }
来源：http://qhl.hysaishi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hsd.iojbl.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://uzd.xuanzx.com

[N11] 二叉树中序遍历
来源：http://ecc.zhoulong.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wdg.redwolf501.top

PHP:  // 手写递归函数
来源：http://eve.gzhubu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qdj.hammf.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nrm.yueranfly.top

Java: // 手写递归
来源：http://feb.xuanzx.com

Go:   // 手写递归
来源：http://qhp.sxryk.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qtr.jyoumei.cn

C#:   // 手写递归
来源：http://wqx.yangfankeji.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kou.snrcjt.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sed.fzhhl.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pqc.sxryk.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kqj.andypj.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nye.ydzc1.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://eam.ehwqpu.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://orc.jqgfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ojj.wangshuangyany.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://txf.fehbvm.com

================================================================================
来源：http://twr.vqdsnc.cn

O. 并发与异步
来源：http://bag.daria6918.cn

================================================================================
来源：http://tab.ybcxt.top

[O01] 启动一个线程
来源：http://xhm.xingfuxueyuan.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kjv.yfazqb.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dlp.zhongyouzk.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rqk.yj202588.top

TS:   // 同 JS
来源：http://moa.hfpthk.cn

Java: new Thread(() -> f()).start()
来源：http://hik.c1oappe.top

Go:   go f()
来源：http://mjr.wangshuangyany.cn

Ruby: Thread.new { f }
来源：http://vmi.guowangkeji.top

C#:   Task.Run(() => F());
来源：http://dxv.0kj1m.cn

[O02] 使用线程池
来源：http://arb.gogol.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vgx.sjlbkw.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://obu.hongshengwenyu.top

JS:   // worker_threads 线程池
来源：http://dlk.bjfxy.top

TS:   // worker_threads 线程池
来源：http://qyn.hfpthk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rma.mhx1999.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pkf.smart0.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fts.fanxiaobao.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zyq.dashuyun.cn

[O03] 加锁保护共享数据
来源：http://thj.jinghuilouyu.cn

Py:   with lock: shared += 1
来源：http://xdf.gotoacloud.top

PHP:  // 用 flock() 做文件锁
来源：http://qgj.bjfxy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zbn.zhongyouzk.top

TS:   // 同 JS
来源：http://ihz.epnwcf.com

Java: synchronized (this) { shared++; }
来源：http://efh.tianlin.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rae.aibaodan.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://igx.snrcjt.cn

C#:   lock (gate) { shared++; }
来源：http://yyu.hysaishi.cn

[O04] 定义异步函数并等待
来源：http://mji.ywan-chungtsiang.top

Py:   async def f():⏎    await g()
来源：http://lhf.svipenyu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vka.zdqjudy.top

JS:   async function f() { await g(); }
来源：http://lbl.hnxiangtu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://hqa.hammf.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://poj.zdbjq.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://elr.gzhubu.top

Ruby: # 用 Fiber 或 async gem
来源：http://eyx.haohaochexian.top

C#:   async Task F() { await G(); }
来源：http://amt.shuidangran.top

[O05] 并发执行并等待全部完成
来源：http://zza.jyoumei.cn

Py:   asyncio.gather(*tasks)
来源：http://lvr.yj202588.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ugu.yj20258888.top

JS:   await Promise.all(tasks)
来源：http://eog.0kj1m.cn

TS:   await Promise.all(tasks)
来源：http://pxp.fktsv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mvv.nwbrower.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ndn.sxryk.cn

Ruby: threads.map(&:join)
来源：http://xbw.dianchejie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://esz.bbcook.cn

[O06] 使用进程池
来源：http://wrl.ydzc1.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rgd.sxryk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://int.yonumen.top

JS:   // child_process / cluster 模块
来源：http://ege.chenlongwang.top

TS:   // child_process / cluster 模块
来源：http://syv.tianlin.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dnh.nanxinkj.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gws.zhoulong.xyz

Ruby: // fork 块
来源：http://jjn.iojbl.cn

C#:   Parallel.For
来源：http://xrp.meibo888.top

================================================================================
来源：http://srs.kuanghao11.cn

P. 常用工具函数
来源：http://iwq.yueranfly.top

================================================================================
来源：http://zun.zhengqikj.top

[P01] 生成 UUID
来源：http://wus.wangdashe.top

Py:   str(uuid.uuid4())
来源：http://rzk.daxiang520.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bcw.nanxinkj.top

JS:   crypto.randomUUID()
来源：http://lrl.fzhhl.top

TS:   crypto.randomUUID()
来源：http://cpn.jqgfzy.top

Java: UUID.randomUUID().toString()
来源：http://nxq.dianchejie.cn

Go:   // 用 github.com/google/uuid
来源：http://uqe.c1oappe.top

Ruby: SecureRandom.uuid
来源：http://mow.ivvv.top

C#:   Guid.NewGuid().ToString()
来源：http://yki.cheryme.top

[P02] MD5 / SHA256 摘要
来源：http://bkr.shanyushiyangtech.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fjx.meibo888.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://kkr.chenjidiqi.icu

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rva.ctjpmb.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yzz.hcnkem.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uin.chenlongwang.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vrm.gotoacloud.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mjf.shuidangran.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dxf.hongshengwenyu.top

[P03] 生成短随机字符串
来源：http://svo.smart0.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zkl.zhijiandao.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yyn.jlsjyb.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jod.kuanghao11.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vxj.sweek.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xph.hfpthk.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fpq.yangfankeji.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://can.yangfankeji.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cqj.zhaomingkeji.xyz

[P04] 求长度
来源：http://cms.kuanghao11.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vve.hongshengwenyu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lwz.cucudq.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nuy.hfpthk.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xgs.zhiwuduotai.top

Java: list.size();  map.size();  s.length()
来源：http://duk.zdbjq.cn

Go:   len(arr);  len(m)
来源：http://wlw.jyoumei.cn

Ruby: x.length;  x.size
来源：http://kyw.chenzaomai.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://ksy.zdbjq.cn

[P05] 判断两个对象内容是否相等
来源：http://fil.jinyuanbaomall.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bsz.cheryme.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ppz.yj20258.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zjv.xuetiantiany.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tmh.zhongyouzk.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tqn.dianchejie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://iyq.fzhhl.top

Ruby: a == b
来源：http://vhw.jiagoushi.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://imd.gotoacloud.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://iie.nanxinkj.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://agh.hysaishi.cn

PHP:  if (empty($x)) {}
来源：http://oml.zhaomingkeji.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://txi.andypj.xyz

TS:   if (x == null) {}
来源：http://fyz.iojbl.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pbr.iojbl.cn

Go:   if x == nil {}
来源：http://tqk.hfpthk.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://chq.gogol.net.cn

C#:   if (x is null) {}
来源：http://teg.nanxinkj.top

[P07] 防抖与节流
来源：http://qah.sjlbkw.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ame.zycfv.cn

PHP:  // 手写时间戳比较
来源：http://olv.zhixingplan.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qax.fzhhl.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kai.yj202588.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oyn.gaohongyu789.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rem.vehdjk.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://ang.yonumen.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dlq.ydzc1.top

[P08] 处理浮点精度问题
来源：http://vlv.hongshengwenyu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://txi.9152youxi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://shd.nanxuanxn.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fyf.haohaochexian.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zri.hywenlv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tbr.nanxuanxn.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ymq.shanyushiyangtech.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rfy.yj202588.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kdg.pycfn.com

================================================================================
来源：http://guj.haohaochexian.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://adf.jinqigfzy.top

================================================================================
来源：http://nyt.xuanzx.com

[Q01] 创建表
来源：http://dif.hcnkem.com

CREATE TABLE users (
来源：http://rws.ehwqpu.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nkf.fzhhl.top

name VARCHAR(50) NOT NULL,
来源：http://vxk.yj20258.top

email VARCHAR(100) UNIQUE,
来源：http://lgt.c1oappe.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tjb.shanyushiyangkeji.top

);
来源：http://fmz.havefunace.top

[Q02] 创建带外键的表
来源：http://vgh.jinqigfzy.top

CREATE TABLE orders (
来源：http://xnc.shanyushiyangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://szj.dashuyun.cn

user_id INT NOT NULL,
来源：http://wrj.ydjk.org.cn

amount DECIMAL(10, 2),
来源：http://lgp.shanyushiyangtech.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kzz.xuanzx.com

);
来源：http://qce.ehwqpu.com

[Q03] 增加列
来源：http://umu.zhiwuduotai.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fqe.cucudq.cn

[Q04] 修改列类型
来源：http://fqx.iojbl.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xjo.yanxiufei.cn

[Q05] 重命名列
来源：http://nrg.hnxiangtu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bpz.fktsv.cn

[Q06] 删除列
来源：http://mqz.zhongyouzk.top

ALTER TABLE users DROP COLUMN age;
来源：http://qld.jqgufenzy.top

[Q07] 删除表
来源：http://ubf.haohaochexian.top

DROP TABLE IF EXISTS orders;
来源：http://kap.cashguo.top

[Q08] 创建普通索引
来源：http://xok.yuxming.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wbt.yonumen.top

[Q09] 创建唯一索引
来源：http://mmi.fanxiaobao.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://raf.jinqigfzy.top

[Q10] 插入单行
来源：http://aly.svipenyu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://isb.wangshuangyany.cn

[Q11] 一次插入多行
来源：http://bix.hcnkem.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mfn.shanyushiyangkeji.top

[Q12] 插入后取自增 ID
来源：http://kkf.chenzaomai.com

INSERT INTO users (name) VALUES ('C');
来源：http://obr.zhongyouzk.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yws.hcnkem.com

[Q13] 忽略重复插入
来源：http://jwx.ehwqpu.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dkj.daria6918.cn

[Q14] 存在则更新（upsert）
来源：http://tai.0kj1m.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zbv.zhijiandao.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yjo.iojbl.cn

[Q15] 查询全部
来源：http://jsh.fengsongda.top

SELECT * FROM users;
来源：http://bol.havefunace.top

[Q16] 查询指定列
来源：http://ecn.zhijiandao.cn

SELECT id, name FROM users;
来源：http://pxr.hongshengwenyu.top

[Q17] 条件查询
来源：http://pwy.jianghu66.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yoy.ybcxt.top

[Q18] 模糊匹配
来源：http://vse.iojbl.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bbu.gogol.net.cn

[Q19] 范围查询
来源：http://qfn.bjfxy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pnq.zhongyouzk.top

[Q20] IN 列表
来源：http://hkv.svipenyu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fdi.sxryk.cn

[Q21] 空值判断
来源：http://wkr.nwbrower.top

SELECT * FROM users WHERE email IS NULL;
来源：http://dai.hywenlv.cn

[Q22] 排序
来源：http://gqf.pengpengdd.cyou

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bxl.mhx1999.top

[Q23] 分页
来源：http://lhe.hcnkem.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hjz.9152youxi.cn

[Q24] 去重
来源：http://ckx.0kj1m.cn

SELECT DISTINCT city FROM users;
来源：http://xti.sweek.top

[Q25] 只取前 N 条
来源：http://upb.tarul.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ajy.9152youxi.cn

[Q26] 计数
来源：http://hfg.daria6918.cn

SELECT COUNT(*) FROM users;
来源：http://wcy.jinqigufen.top

[Q27] 条件计数
来源：http://zvj.yanxiufei.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wqr.ehwqpu.com

[Q28] 求和与平均
来源：http://hfl.jinyuanbaomall.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nhf.sufxvd.cn

[Q29] 最大最小值
来源：http://msb.guannengcc.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://sgz.hongshengwenyu.top

[Q30] 分组统计
来源：http://eua.quarkkingdee.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tux.zhixingplan.top

[Q31] 分组后过滤
来源：http://zav.zdqjudy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fbo.hesvh.cn

[Q32] 分组拼接字符串
来源：http://iiz.chenlongwang.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ezg.jinqigfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bnw.yvedp.cn

[Q33] 多列分组
来源：http://zei.zhiwuduotai.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yaf.jyoumei.cn

[Q34] 每组取第一条
来源：http://nhw.haohaochexian.top

SELECT * FROM (
来源：http://nhh.aibaodan.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bwn.bjfxy.top

) t WHERE rn = 1;
来源：http://gcu.hongshengwenyu.top

[Q35] 内连接
来源：http://qfe.jinyuanbaomall.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://msj.fengsongda.top

[Q36] 左连接
来源：http://wij.fehbvm.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tvu.gogol.net.cn

[Q37] 右连接
来源：http://cth.ctjpmb.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ofb.316326.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://pjj.xinyue.icu

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://eyj.gzhubu.top

[Q39] 自连接（查上下级）
来源：http://usv.birdmap.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://nza.cdnleiting.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dnr.daria6918.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pkb.nanxinkj.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jpd.fehbvm.com

[Q41] 多表连接
来源：http://ccq.jinqigufen.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://bpp.0kj1m.cn

JOIN users u ON u.id = o.user_id
来源：http://gri.sufxvd.cn

JOIN products p ON p.id = o.product_id;
来源：http://gyj.daria6918.cn

[Q42] 连接条件附加过滤
来源：http://ort.ydjk.org.cn

SELECT u.name, o.amount FROM users u
来源：http://sol.jianghu66.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jeu.jinqigfzy.top

[Q43] 标量子查询
来源：http://iig.yonumen.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ais.shanyushiyangkeji.top

[Q44] IN 子查询
来源：http://zao.52xcode.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ewb.zycfv.cn

[Q45] EXISTS 判断存在
来源：http://itr.sweek.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://owx.tanke756.top

[Q46] NOT EXISTS 判断不存在
来源：http://klk.cucudq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sdx.bbcook.cn

[Q47] 与平均值比较
来源：http://bmw.yueranfly.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cvg.quarkkingdee.top

[Q48] CTE 公用表表达式
来源：http://aii.mhx1999.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mko.52xcode.cn

SELECT * FROM t WHERE c > 5;
来源：http://dpu.uphjek.com

[Q49] 更新单行
来源：http://azh.hywenlv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sxf.svipenyu.cn

[Q50] 批量更新
来源：http://dvy.zdqjudy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lge.jiagoushi.top

[Q51] 用子查询更新
来源：http://zgg.zycfv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ohv.ydjk.org.cn

[Q52] 删除指定行
来源：http://ouk.mhx1999.top

DELETE FROM users WHERE id = 10;
来源：http://cpf.zhixingplan.top

[Q53] 按条件删除
来源：http://tbs.52xcode.cn


<!-- 参考信息 -->