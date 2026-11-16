代发 wailian999

Go:   // 手写 map[int]int
来源：http://aej.cheryme.top

Ruby: // 手写 Hash
来源：http://mzn.zhongyouzk.top

C#:   // 手写 Dictionary<int, int>
来源：http://idy.epnwcf.com

[N08] 生成全排列
来源：http://qma.sxryk.cn

Py:   itertools.permutations(arr)
来源：http://ygd.yj202588.top

PHP:  // 手写递归交换
来源：http://muo.sufxvd.cn

JS:   // 手写回溯递归
来源：http://zug.52xcode.cn

TS:   // 手写回溯递归
来源：http://jhh.zhoulong.xyz

Java: // 手写回溯递归
来源：http://hjo.yj20258888.top

Go:   // 手写回溯递归
来源：http://csj.tian-w.cn

Ruby: arr.permutation.to_a
来源：http://gax.tianlin.xyz

C#:   // 手写回溯递归
来源：http://sjy.wangdashe.top

[N09] 栈与队列
来源：http://dxq.hnqzz.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ijb.ehwqpu.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://plx.c1oappe.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://urj.havefunace.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ajd.yangfankeji.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tzq.wangshuangyany.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kpp.jqgufenzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://krs.tarul.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cal.yj20258.top

[N10] 链表节点定义
来源：http://ulu.zhixingplan.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bti.xuetiantiany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hml.feifeiyinyue.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qmz.mhx1999.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dhl.hesvh.cn

Java: class Node { int v; Node next; }
来源：http://phy.zhongyouzk.top

Go:   type Node struct { V int; Next *Node }
来源：http://pew.redwolf501.top

Ruby: Node = Struct.new(:v, :next)
来源：http://auy.dashuyun.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vae.pengpengdd.cyou

[N11] 二叉树中序遍历
来源：http://nnh.ppjwa.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nhl.gogol.net.cn

PHP:  // 手写递归函数
来源：http://kmd.tarul.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qeh.nwbrower.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nev.hesvh.cn

Java: // 手写递归
来源：http://szm.kuanghao11.cn

Go:   // 手写递归
来源：http://lsj.nwbrower.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kjo.wangdashe.top

C#:   // 手写递归
来源：http://qzg.hnqzz.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nzu.vehdjk.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oho.jinqigufen.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wcc.wangshuangyany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vrl.kuanghao11.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://amw.kuanghao11.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ela.jinghuilouyu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://knf.hywenlv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://spw.cdnleiting.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sxr.fengsongda.top

================================================================================
来源：http://nqh.ydzc1.top

O. 并发与异步
来源：http://knt.ppjwa.cn

================================================================================
来源：http://itd.vehdjk.com

[O01] 启动一个线程
来源：http://ppt.jiagoushi.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zhu.zhijiandao.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pml.zycfv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dct.ppjwa.cn

TS:   // 同 JS
来源：http://tmb.tanke756.top

Java: new Thread(() -> f()).start()
来源：http://orl.nanxinkj.top

Go:   go f()
来源：http://jho.tarul.cn

Ruby: Thread.new { f }
来源：http://pic.iojbl.cn

C#:   Task.Run(() => F());
来源：http://kxk.yanxiufei.cn

[O02] 使用线程池
来源：http://ooi.haohaochexian.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dnr.hysaishi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yef.jinqigfzy.top

JS:   // worker_threads 线程池
来源：http://xom.bbcook.cn

TS:   // worker_threads 线程池
来源：http://rxr.sysykeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://egt.fanxiaobao.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lca.chenjidiqi.icu

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jnp.meibo888.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cju.fktsv.cn

[O03] 加锁保护共享数据
来源：http://qob.fengsongda.top

Py:   with lock: shared += 1
来源：http://qvv.hfpthk.cn

PHP:  // 用 flock() 做文件锁
来源：http://vss.kuanghao11.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://upu.9152youxi.cn

TS:   // 同 JS
来源：http://ken.yj20258888.top

Java: synchronized (this) { shared++; }
来源：http://gad.jinyuanbaomall.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qom.hfpthk.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cty.sjlbkw.cn

C#:   lock (gate) { shared++; }
来源：http://rcs.cashguo.top

[O04] 定义异步函数并等待
来源：http://amo.fktsv.cn

Py:   async def f():⏎    await g()
来源：http://ydh.gotoacloud.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dbh.zdbjq.cn

JS:   async function f() { await g(); }
来源：http://ktp.daria6918.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://llm.shuidangran.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://erm.zhiwuduotai.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bph.yj202588.top

Ruby: # 用 Fiber 或 async gem
来源：http://mlr.sjlbkw.cn

C#:   async Task F() { await G(); }
来源：http://gdk.hesvh.cn

[O05] 并发执行并等待全部完成
来源：http://ugr.tianlin.xyz

Py:   asyncio.gather(*tasks)
来源：http://zzx.yj20258.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ynt.yonumen.top

JS:   await Promise.all(tasks)
来源：http://qip.shangyingyoupin.top

TS:   await Promise.all(tasks)
来源：http://pso.zhaomingkeji.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hsl.nanxuanxn.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://teb.hfpthk.cn

Ruby: threads.map(&:join)
来源：http://nps.vehdjk.com

C#:   await Task.WhenAll(t1, t2)
来源：http://nvt.nanxinkj.top

[O06] 使用进程池
来源：http://vau.chenzaomai.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dvs.tanke756.top

PHP:  // pcntl_fork 或多进程队列
来源：http://dhz.yj202588.top

JS:   // child_process / cluster 模块
来源：http://iog.ivvv.top

TS:   // child_process / cluster 模块
来源：http://nky.jlsjyb.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ver.tanke756.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dle.cheryme.top

Ruby: // fork 块
来源：http://piv.ehwqpu.com

C#:   Parallel.For
来源：http://vjb.ctjpmb.com

================================================================================
来源：http://csg.daria6918.cn

P. 常用工具函数
来源：http://ali.0kj1m.cn

================================================================================
来源：http://dty.feifeiyinyue.top

[P01] 生成 UUID
来源：http://ajd.hysaishi.cn

Py:   str(uuid.uuid4())
来源：http://zau.zdqjudy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nzw.tian-w.cn

JS:   crypto.randomUUID()
来源：http://zhg.yonumen.top

TS:   crypto.randomUUID()
来源：http://oma.daria6918.cn

Java: UUID.randomUUID().toString()
来源：http://xza.0kj1m.cn

Go:   // 用 github.com/google/uuid
来源：http://mkx.hongshengwenyu.top

Ruby: SecureRandom.uuid
来源：http://vje.jiagoushi.top

C#:   Guid.NewGuid().ToString()
来源：http://ygd.hcnkem.com

[P02] MD5 / SHA256 摘要
来源：http://ley.yuxming.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rcw.daxiang520.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://hdr.gzhubu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kpa.pycfn.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jzl.xingfuxueyuan.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fnp.mhx1999.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ydl.hammf.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mda.cdnleiting.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://abl.kuanghao11.cn

[P03] 生成短随机字符串
来源：http://zvz.52xcode.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://oyn.shuidangran.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pmw.fzhhl.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qvo.vehdjk.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pcx.ybcxt.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dyb.shuidangran.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tjn.tanke756.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://jis.zhongyouzk.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yrx.andypj.xyz

[P04] 求长度
来源：http://jsl.shangyingyoupin.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tju.cqqwz.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qlg.ehwqpu.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qhr.shuidangran.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gor.zhixingplan.top

Java: list.size();  map.size();  s.length()
来源：http://xzk.hysaishi.cn

Go:   len(arr);  len(m)
来源：http://unn.fengsongda.top

Ruby: x.length;  x.size
来源：http://cap.zdqjudy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jsq.ctjpmb.com

[P05] 判断两个对象内容是否相等
来源：http://sui.cqqwz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fhb.xingfuxueyuan.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gxi.zhoulong.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gko.sufxvd.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://khz.jlsjyb.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wmc.fzhhl.top

Go:   reflect.DeepEqual(a, b)
来源：http://ekb.hnxiangtu.top

Ruby: a == b
来源：http://aho.jinghuilouyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lkp.hnqzz.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ksa.ywan-chungtsiang.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mkz.zdbjq.cn

PHP:  if (empty($x)) {}
来源：http://ske.zhengqikj.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bty.jinyuanbaomall.cn

TS:   if (x == null) {}
来源：http://aui.fanxiaobao.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://xar.shangyingyoupin.top

Go:   if x == nil {}
来源：http://zdv.yongpay.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://out.zhengqikj.top

C#:   if (x is null) {}
来源：http://qry.hfpthk.cn

[P07] 防抖与节流
来源：http://qum.zhoulong.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://acg.fanxiaobao.xyz

PHP:  // 手写时间戳比较
来源：http://opk.c1oappe.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lcp.hysaishi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rrn.jinqigufen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fwa.ctjpmb.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://caw.tianlin.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://hxc.tian-w.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gbi.pycfn.com

[P08] 处理浮点精度问题
来源：http://kwp.sysykeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xpn.zhengqikj.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://oof.tian-w.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lye.zhiwuduotai.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vgq.jyoumei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jmq.mhx1999.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eop.nwbrower.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pdg.haohaochexian.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yfx.yanxiufei.cn

================================================================================
来源：http://tfx.feifeiyinyue.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wqi.andypj.xyz

================================================================================
来源：http://fbx.zhoulong.xyz

[Q01] 创建表
来源：http://azd.zhijiandao.cn

CREATE TABLE users (
来源：http://nlx.hfpthk.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://oqb.yj20258.top

name VARCHAR(50) NOT NULL,
来源：http://gmd.bjfxy.top

email VARCHAR(100) UNIQUE,
来源：http://gpw.quarkkingdee.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ejj.ybcxt.top

);
来源：http://zci.jqgufenzy.top

[Q02] 创建带外键的表
来源：http://rcw.yj202588.top

CREATE TABLE orders (
来源：http://qsv.sufxvd.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gxb.daria6918.cn

user_id INT NOT NULL,
来源：http://tfp.yuanzhike.top

amount DECIMAL(10, 2),
来源：http://zay.sxryk.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jlx.hywenlv.cn

);
来源：http://uji.dashuyun.cn

[Q03] 增加列
来源：http://ibl.shzxlz.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vdi.iojbl.cn

[Q04] 修改列类型
来源：http://vyt.epnwcf.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cxs.kuanghao11.cn

[Q05] 重命名列
来源：http://zqz.0kj1m.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ill.zhiwuduotai.top

[Q06] 删除列
来源：http://ndv.zhixingplan.top

ALTER TABLE users DROP COLUMN age;
来源：http://ewv.quarkkingdee.top

[Q07] 删除表
来源：http://hlh.c1oappe.top

DROP TABLE IF EXISTS orders;
来源：http://ivr.gotoacloud.top

[Q08] 创建普通索引
来源：http://vck.redwolf501.top

CREATE INDEX idx_users_email ON users(email);
来源：http://vsz.haohaochexian.top

[Q09] 创建唯一索引
来源：http://xzx.quarkkingdee.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://win.0kj1m.cn

[Q10] 插入单行
来源：http://jsy.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://flb.yj202588.top

[Q11] 一次插入多行
来源：http://ouv.cheryme.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ufy.fktsv.cn

[Q12] 插入后取自增 ID
来源：http://kzw.guowangkeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://ree.fengsongda.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mvd.sweek.top

[Q13] 忽略重复插入
来源：http://ozp.zhiwuduotai.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bwi.ydjk.org.cn

[Q14] 存在则更新（upsert）
来源：http://hfy.nwbrower.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://woh.yvedp.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hpy.epnwcf.com

[Q15] 查询全部
来源：http://acl.hammf.cn

SELECT * FROM users;
来源：http://bjn.316326.xyz

[Q16] 查询指定列
来源：http://phz.yvedp.cn

SELECT id, name FROM users;
来源：http://lvq.fengsongda.top

[Q17] 条件查询
来源：http://zeg.yangfankeji.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tpl.gaohongyu789.top

[Q18] 模糊匹配
来源：http://dbo.zhijiandao.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xul.hywenlv.cn

[Q19] 范围查询
来源：http://vtd.jinqigfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dea.daxiang520.top

[Q20] IN 列表
来源：http://gsv.yuxming.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hwm.hysaishi.cn

[Q21] 空值判断
来源：http://vvd.wangdashe.top

SELECT * FROM users WHERE email IS NULL;
来源：http://dgr.yfazqb.com

[Q22] 排序
来源：http://lhk.yanxiufei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ftv.ydjk.org.cn

[Q23] 分页
来源：http://iby.daria6918.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mci.yonumen.top

[Q24] 去重
来源：http://ebf.shanyushiyangkeji.top

SELECT DISTINCT city FROM users;
来源：http://cpr.cdnleiting.top

[Q25] 只取前 N 条
来源：http://mif.fengsongda.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://snd.hcnkem.com

[Q26] 计数
来源：http://asr.quarkkingdee.top

SELECT COUNT(*) FROM users;
来源：http://leo.yonumen.top

[Q27] 条件计数
来源：http://qwp.zhengqikj.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uqn.tanke756.top

[Q28] 求和与平均
来源：http://rdr.bbcook.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nra.guannengcc.top

[Q29] 最大最小值
来源：http://ofe.vqdsnc.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mmz.zdbjq.cn

[Q30] 分组统计
来源：http://mur.sufxvd.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cwf.pycfn.com

[Q31] 分组后过滤
来源：http://cbm.pycfn.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ppp.hammf.cn

[Q32] 分组拼接字符串
来源：http://tmi.yuanzhike.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ifs.pengpengdd.cyou

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jxu.cashguo.top

[Q33] 多列分组
来源：http://dop.chenzaomai.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nau.sysykeji.top

[Q34] 每组取第一条
来源：http://bki.hnxiangtu.top

SELECT * FROM (
来源：http://jpr.aizwys.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wml.zhijiandao.cn

) t WHERE rn = 1;
来源：http://lii.zhaomingkeji.xyz

[Q35] 内连接
来源：http://rwk.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gfe.52xcode.cn

[Q36] 左连接
来源：http://ste.yfazqb.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://djf.pengpengdd.cyou

[Q37] 右连接
来源：http://pjy.yuxming.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rso.bbcook.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jdi.hammf.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ytp.redwolf501.top

[Q39] 自连接（查上下级）
来源：http://pei.nwbrower.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://fnj.fengsongda.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cep.gzhubu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xaf.nanxuanxn.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sqx.shangyingyoupin.top

[Q41] 多表连接
来源：http://hdt.zhiwuduotai.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://diz.zdbjq.cn

JOIN users u ON u.id = o.user_id
来源：http://wkc.shanyushiyangkeji.top

JOIN products p ON p.id = o.product_id;
来源：http://opv.yongpay.top

[Q42] 连接条件附加过滤
来源：http://jkq.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u
来源：http://oho.sjlbkw.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://trj.nwbrower.top

[Q43] 标量子查询
来源：http://hco.sufxvd.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fhu.shangyingyoupin.top

[Q44] IN 子查询
来源：http://qkx.fanxiaobao.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lwq.nanxuanxn.top

[Q45] EXISTS 判断存在
来源：http://tfj.hcnkem.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hrg.mhx1999.top

[Q46] NOT EXISTS 判断不存在
来源：http://jsv.cucudq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://syr.sufxvd.cn

[Q47] 与平均值比较
来源：http://qqm.jyoumei.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://iid.shuidangran.top

[Q48] CTE 公用表表达式
来源：http://ujg.dianchejie.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dhc.shangyingyoupin.top

SELECT * FROM t WHERE c > 5;
来源：http://vbz.ehwqpu.com

[Q49] 更新单行
来源：http://pnm.hfpthk.cn


<!-- 参考信息 -->