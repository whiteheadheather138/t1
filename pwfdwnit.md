代发 wailian999

Py:   itertools.permutations(arr)
来源：http://tjd.jiagoushi.top

PHP:  // 手写递归交换
来源：http://poi.ybcxt.top

JS:   // 手写回溯递归
来源：http://nls.daria6918.cn

TS:   // 手写回溯递归
来源：http://sdq.gotoacloud.top

Java: // 手写回溯递归
来源：http://dby.yvedp.cn

Go:   // 手写回溯递归
来源：http://qyu.yj202588.top

Ruby: arr.permutation.to_a
来源：http://xjs.ehwqpu.com

C#:   // 手写回溯递归
来源：http://eyh.cashguo.top

[N09] 栈与队列
来源：http://tdd.vehdjk.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cgv.shuidangran.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xuc.vehdjk.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ixj.bjfxy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://luo.uphjek.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fim.ppjwa.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ibn.yuxming.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jae.hnxiangtu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sgc.hfpthk.cn

[N10] 链表节点定义
来源：http://wyo.quarkkingdee.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zqi.wangshuangyany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ids.yongpay.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://luv.gogol.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vqp.jiagoushi.top

Java: class Node { int v; Node next; }
来源：http://smt.hnqzz.top

Go:   type Node struct { V int; Next *Node }
来源：http://jlk.iojbl.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://stt.xingfuxueyuan.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://qcw.vqdsnc.cn

[N11] 二叉树中序遍历
来源：http://jlg.hfpthk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fbf.cashguo.top

PHP:  // 手写递归函数
来源：http://sko.zhoulong.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eza.ywan-chungtsiang.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://anb.iojbl.cn

Java: // 手写递归
来源：http://rxe.yj202588.top

Go:   // 手写递归
来源：http://lby.andypj.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vez.chenjidiqi.icu

C#:   // 手写递归
来源：http://dgr.yvedp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pmq.gotoacloud.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://itr.fanxiaobao.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jop.shanyushiyangkeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mge.xingfuxueyuan.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ntc.daria6918.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qhp.nanxinkj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ujf.fanxiaobao.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://drs.havefunace.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://owh.hammf.cn

================================================================================
来源：http://dbq.ybcxt.top

O. 并发与异步
来源：http://qza.ctjpmb.com

================================================================================
来源：http://mon.zhongyouzk.top

[O01] 启动一个线程
来源：http://usf.chenlongwang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ixg.shzxlz.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://equ.shanyushiyangtech.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fko.dashuyun.cn

TS:   // 同 JS
来源：http://ftz.andypj.xyz

Java: new Thread(() -> f()).start()
来源：http://kjr.gaohongyu789.top

Go:   go f()
来源：http://qrh.xinyue.icu

Ruby: Thread.new { f }
来源：http://fee.feifeiyinyue.top

C#:   Task.Run(() => F());
来源：http://dam.shanyushiyangkeji.top

[O02] 使用线程池
来源：http://cif.ppjwa.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://toz.vqdsnc.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://erp.fengsongda.top

JS:   // worker_threads 线程池
来源：http://wsl.hfpthk.cn

TS:   // worker_threads 线程池
来源：http://ymb.jqgfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://nio.snrcjt.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rec.zhiwuduotai.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jpx.yuanzhike.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wfm.andypj.xyz

[O03] 加锁保护共享数据
来源：http://xfm.uphjek.com

Py:   with lock: shared += 1
来源：http://xsz.zhiwuduotai.top

PHP:  // 用 flock() 做文件锁
来源：http://iyr.yonumen.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ikw.gaohongyu789.top

TS:   // 同 JS
来源：http://tgj.redwolf501.top

Java: synchronized (this) { shared++; }
来源：http://trt.sufxvd.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hjz.yj202588.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ypi.0kj1m.cn

C#:   lock (gate) { shared++; }
来源：http://atf.gzhubu.top

[O04] 定义异步函数并等待
来源：http://isx.haohaochexian.top

Py:   async def f():⏎    await g()
来源：http://nux.hnqzz.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nff.shanyushiyangtech.top

JS:   async function f() { await g(); }
来源：http://baf.xziqi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ydz.pycfn.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bpl.bjfxy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gxm.quarkkingdee.top

Ruby: # 用 Fiber 或 async gem
来源：http://car.ivvv.top

C#:   async Task F() { await G(); }
来源：http://yzj.yj20258.top

[O05] 并发执行并等待全部完成
来源：http://ahd.chenlongwang.top

Py:   asyncio.gather(*tasks)
来源：http://spy.svipenyu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oej.aizwys.cn

JS:   await Promise.all(tasks)
来源：http://acf.jqgfzy.top

TS:   await Promise.all(tasks)
来源：http://ccj.yonumen.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wbv.xziqi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bgl.kuanghao11.cn

Ruby: threads.map(&:join)
来源：http://hos.sjlbkw.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vmo.yuxming.cn

[O06] 使用进程池
来源：http://rgr.ydjk.org.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uia.jlsjyb.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wfb.fengsongda.top

JS:   // child_process / cluster 模块
来源：http://aem.sufxvd.cn

TS:   // child_process / cluster 模块
来源：http://cnq.jinqigufen.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zwu.wangdashe.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xoh.xylfe.cn

Ruby: // fork 块
来源：http://pwj.daria6918.cn

C#:   Parallel.For
来源：http://axm.zycfv.cn

================================================================================
来源：http://rpb.vqdsnc.cn

P. 常用工具函数
来源：http://ofp.yueranfly.top

================================================================================
来源：http://dld.redwolf501.top

[P01] 生成 UUID
来源：http://xav.zhaomingkeji.xyz

Py:   str(uuid.uuid4())
来源：http://peh.zhijiandao.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ayc.gogol.net.cn

JS:   crypto.randomUUID()
来源：http://krp.xylfe.cn

TS:   crypto.randomUUID()
来源：http://mwr.jianghu66.top

Java: UUID.randomUUID().toString()
来源：http://zrh.jianghu66.top

Go:   // 用 github.com/google/uuid
来源：http://zle.birdmap.top

Ruby: SecureRandom.uuid
来源：http://mit.jinghuilouyu.cn

C#:   Guid.NewGuid().ToString()
来源：http://xgi.shuidangran.top

[P02] MD5 / SHA256 摘要
来源：http://kzl.iojbl.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jnt.xingfuxueyuan.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://zkd.jinqigfzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kbj.andypj.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ajw.xingfuxueyuan.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zin.hfpthk.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nwp.feifeiyinyue.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://scv.dashuyun.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://srj.chenlongwang.top

[P03] 生成短随机字符串
来源：http://oug.tian-w.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cti.jlsjyb.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tkb.hongshengwenyu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hkh.jinqigfzy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rhj.sjlbkw.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nwr.yfazqb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ate.yfazqb.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://lcc.yj20258888.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gwo.aibaodan.cn

[P04] 求长度
来源：http://wrl.sxryk.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vnh.hesvh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kst.hongshengwenyu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gji.fzhhl.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nic.jinyuanbaomall.cn

Java: list.size();  map.size();  s.length()
来源：http://nsp.zhiwuduotai.top

Go:   len(arr);  len(m)
来源：http://pka.ydjk.org.cn

Ruby: x.length;  x.size
来源：http://wcb.redwolf501.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://tdf.jinyuanbaomall.cn

[P05] 判断两个对象内容是否相等
来源：http://oxk.meibo888.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://dpp.bbcook.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wpl.ppjwa.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mof.ivvv.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://oin.yueranfly.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qli.sxryk.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lze.zhiwuduotai.top

Ruby: a == b
来源：http://rbn.zhaomingkeji.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bcq.dianchejie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://chh.zhaomingkeji.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ogj.ppjwa.cn

PHP:  if (empty($x)) {}
来源：http://zcu.yj20258.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ekk.shanyushiyangkeji.top

TS:   if (x == null) {}
来源：http://qoe.cucudq.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://yrh.52xcode.cn

Go:   if x == nil {}
来源：http://yfp.nwbrower.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sfc.fehbvm.com

C#:   if (x is null) {}
来源：http://ljs.ehwqpu.com

[P07] 防抖与节流
来源：http://ffa.hnqzz.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hbi.mhx1999.top

PHP:  // 手写时间戳比较
来源：http://sou.cheryme.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rbe.pycfn.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://msb.yuxming.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ike.smart0.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nzn.shanyushiyangkeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://pco.hesvh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xcf.ydzc1.top

[P08] 处理浮点精度问题
来源：http://hco.shzxlz.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kcp.jinqigufen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://taz.andypj.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ilr.epnwcf.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mvs.yueranfly.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uvd.cashguo.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nue.ywan-chungtsiang.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vql.vqdsnc.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nkt.cashguo.top

================================================================================
来源：http://ciw.hnxiangtu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ipz.tian-w.cn

================================================================================
来源：http://zaq.yuxming.cn

[Q01] 创建表
来源：http://fqm.birdmap.top

CREATE TABLE users (
来源：http://ccn.bjfxy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jxm.guowangkeji.top

name VARCHAR(50) NOT NULL,
来源：http://gmr.fengsongda.top

email VARCHAR(100) UNIQUE,
来源：http://fvr.dianchejie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qni.fanxiaobao.xyz

);
来源：http://czb.cqqwz.cn

[Q02] 创建带外键的表
来源：http://sro.xuetiantiany.cn

CREATE TABLE orders (
来源：http://jof.fehbvm.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xkk.jinyuanbaomall.cn

user_id INT NOT NULL,
来源：http://faa.havefunace.top

amount DECIMAL(10, 2),
来源：http://mfk.guannengcc.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uuq.haohaochexian.top

);
来源：http://pcw.yj202588.top

[Q03] 增加列
来源：http://tqj.nanxinkj.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xba.fktsv.cn

[Q04] 修改列类型
来源：http://kzk.shzxlz.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yna.hongshengwenyu.top

[Q05] 重命名列
来源：http://mlr.jiagoushi.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://azy.feifeiyinyue.top

[Q06] 删除列
来源：http://zis.zdbjq.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lnb.ydjk.org.cn

[Q07] 删除表
来源：http://hsc.jqgufenzy.top

DROP TABLE IF EXISTS orders;
来源：http://rel.cqqwz.cn

[Q08] 创建普通索引
来源：http://pgx.vehdjk.com

CREATE INDEX idx_users_email ON users(email);
来源：http://vle.jqgfzy.top

[Q09] 创建唯一索引
来源：http://uca.shanyushiyangtech.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://udk.hnqzz.top

[Q10] 插入单行
来源：http://lhl.ywan-chungtsiang.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wmm.haohaochexian.top

[Q11] 一次插入多行
来源：http://ody.jqgfzy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://euq.pycfn.com

[Q12] 插入后取自增 ID
来源：http://hac.chenjidiqi.icu

INSERT INTO users (name) VALUES ('C');
来源：http://kil.shanyushiyangtech.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sae.hfpthk.cn

[Q13] 忽略重复插入
来源：http://yuk.yueranfly.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wfz.vehdjk.com

[Q14] 存在则更新（upsert）
来源：http://fvy.dianchejie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hyi.guowangkeji.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qvs.yueranfly.top

[Q15] 查询全部
来源：http://onk.vqdsnc.cn

SELECT * FROM users;
来源：http://idt.nanxuanxn.top

[Q16] 查询指定列
来源：http://ojc.tian-w.cn

SELECT id, name FROM users;
来源：http://pps.cucudq.cn

[Q17] 条件查询
来源：http://tju.316326.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uml.52xcode.cn

[Q18] 模糊匹配
来源：http://pqn.cdnleiting.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sva.wangshuangyany.cn

[Q19] 范围查询
来源：http://sgn.jinqigufen.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pkt.0kj1m.cn

[Q20] IN 列表
来源：http://ihy.ctjpmb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bzm.yj20258888.top

[Q21] 空值判断
来源：http://kjc.xinyue.icu

SELECT * FROM users WHERE email IS NULL;
来源：http://tkd.ivvv.top

[Q22] 排序
来源：http://mxt.tianlin.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pin.uphjek.com

[Q23] 分页
来源：http://orv.cheryme.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://shs.aibaodan.cn

[Q24] 去重
来源：http://xxq.ywan-chungtsiang.top

SELECT DISTINCT city FROM users;
来源：http://kjb.sxryk.cn

[Q25] 只取前 N 条
来源：http://htf.yj20258888.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sht.pengpengdd.cyou

[Q26] 计数
来源：http://rww.hnqzz.top

SELECT COUNT(*) FROM users;
来源：http://sat.ivvv.top

[Q27] 条件计数
来源：http://bng.wangdashe.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yed.wangdashe.top

[Q28] 求和与平均
来源：http://euz.zycfv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ceu.guowangkeji.top

[Q29] 最大最小值
来源：http://rju.fktsv.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hgq.havefunace.top

[Q30] 分组统计
来源：http://yqd.jianghu66.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kjt.ybcxt.top

[Q31] 分组后过滤
来源：http://pxw.yueranfly.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://abu.jlsjyb.cn

[Q32] 分组拼接字符串
来源：http://rei.cucudq.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qdu.ehwqpu.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zll.xuanzx.com

[Q33] 多列分组
来源：http://glu.zhengqikj.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cbs.yj20258888.top

[Q34] 每组取第一条
来源：http://jrk.yj20258888.top

SELECT * FROM (
来源：http://erb.shangyingyoupin.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://aee.bjfxy.top

) t WHERE rn = 1;
来源：http://cqe.hesvh.cn

[Q35] 内连接
来源：http://btc.sjlbkw.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xsc.tianlin.xyz

[Q36] 左连接
来源：http://rrt.hcnkem.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://skx.feifeiyinyue.top

[Q37] 右连接
来源：http://sal.jlsjyb.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://iou.vqdsnc.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ken.kuanghao11.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://usy.shanyushiyangkeji.top

[Q39] 自连接（查上下级）
来源：http://lcy.shuidangran.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://zcw.iojbl.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ltu.nanxinkj.top

[Q40] 交叉连接（笛卡尔积）
来源：http://uiz.yfazqb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vpv.yfazqb.com

[Q41] 多表连接
来源：http://gva.fktsv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://njs.zhoulong.xyz

JOIN users u ON u.id = o.user_id
来源：http://vhe.wangshuangyany.cn

JOIN products p ON p.id = o.product_id;
来源：http://njq.kuanghao11.cn

[Q42] 连接条件附加过滤
来源：http://emy.shanyushiyangkeji.top

SELECT u.name, o.amount FROM users u
来源：http://ebr.jqgufenzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dkl.aibaodan.cn

[Q43] 标量子查询
来源：http://qnf.guannengcc.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xkq.hammf.cn

[Q44] IN 子查询
来源：http://vrw.ivvv.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fad.hcnkem.com

[Q45] EXISTS 判断存在
来源：http://zhw.shanyushiyangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lus.ydzc1.top

[Q46] NOT EXISTS 判断不存在
来源：http://sqa.0kj1m.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wuq.yj20258.top

[Q47] 与平均值比较
来源：http://ghv.0kj1m.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gpk.shanyushiyangtech.top

[Q48] CTE 公用表表达式
来源：http://waf.sysykeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xiw.xinyue.icu

SELECT * FROM t WHERE c > 5;
来源：http://vcn.jlsjyb.cn

[Q49] 更新单行
来源：http://jtt.hammf.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://abz.gotoacloud.top

[Q50] 批量更新
来源：http://mbt.hfpthk.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cna.xuetiantiany.cn

[Q51] 用子查询更新
来源：http://wwm.jlsjyb.cn


<!-- 参考信息 -->