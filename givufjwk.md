代发 wailian999

Go:   // 手写 map[int]int
来源：http://jan.yonumen.top

Ruby: // 手写 Hash
来源：http://cix.chenlongwang.top

C#:   // 手写 Dictionary<int, int>
来源：http://hnd.yj202588.top

[N08] 生成全排列
来源：http://rlr.yvedp.cn

Py:   itertools.permutations(arr)
来源：http://off.ppjwa.cn

PHP:  // 手写递归交换
来源：http://qwq.guannengcc.top

JS:   // 手写回溯递归
来源：http://zkh.feifeiyinyue.top

TS:   // 手写回溯递归
来源：http://lfz.bjfxy.top

Java: // 手写回溯递归
来源：http://mry.fanxiaobao.xyz

Go:   // 手写回溯递归
来源：http://cdw.fktsv.cn

Ruby: arr.permutation.to_a
来源：http://zsz.hnxiangtu.top

C#:   // 手写回溯递归
来源：http://sqp.guannengcc.top

[N09] 栈与队列
来源：http://dso.chenlongwang.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xjf.ybcxt.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hhx.ydzc1.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mum.fanxiaobao.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zbc.zdqjudy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bjd.mhx1999.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tfd.chenlongwang.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xch.zhoulong.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ynb.sxryk.cn

[N10] 链表节点定义
来源：http://jgk.jyoumei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sxg.yuanzhike.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vls.sjlbkw.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uzy.jinqigufen.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zbm.jyoumei.cn

Java: class Node { int v; Node next; }
来源：http://uvy.yj202588.top

Go:   type Node struct { V int; Next *Node }
来源：http://eji.dashuyun.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fpr.iojbl.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://chx.feifeiyinyue.top

[N11] 二叉树中序遍历
来源：http://ifj.wangshuangyany.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://omj.tanke756.top

PHP:  // 手写递归函数
来源：http://dyh.316326.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qxr.shanyushiyangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xbf.hywenlv.cn

Java: // 手写递归
来源：http://ish.shangyingyoupin.top

Go:   // 手写递归
来源：http://jzn.bjfxy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zwx.dianchejie.cn

C#:   // 手写递归
来源：http://tds.9152youxi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wck.tian-w.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ihq.316326.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ztl.sufxvd.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sby.zhixingplan.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kqd.zhijiandao.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://opt.hongshengwenyu.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ygc.smart0.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pcq.guowangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bby.zhoulong.xyz

================================================================================
来源：http://zit.jinqigufen.top

O. 并发与异步
来源：http://vyv.aizwys.cn

================================================================================
来源：http://khn.c1oappe.top

[O01] 启动一个线程
来源：http://jkm.cheryme.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rda.gaohongyu789.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jzc.vqdsnc.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rqa.guannengcc.top

TS:   // 同 JS
来源：http://ual.hammf.cn

Java: new Thread(() -> f()).start()
来源：http://hqm.cdnleiting.top

Go:   go f()
来源：http://pfl.yfazqb.com

Ruby: Thread.new { f }
来源：http://yra.cucudq.cn

C#:   Task.Run(() => F());
来源：http://jau.aizwys.cn

[O02] 使用线程池
来源：http://kqh.xingfuxueyuan.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kth.chenzaomai.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fli.redwolf501.top

JS:   // worker_threads 线程池
来源：http://ppv.wangshuangyany.cn

TS:   // worker_threads 线程池
来源：http://nwb.chenjidiqi.icu

Java: Executors.newFixedThreadPool(4)
来源：http://dsr.haohaochexian.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xkt.quarkkingdee.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vmk.yj20258888.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://otw.ivvv.top

[O03] 加锁保护共享数据
来源：http://jvt.ydjk.org.cn

Py:   with lock: shared += 1
来源：http://mzv.jyoumei.cn

PHP:  // 用 flock() 做文件锁
来源：http://twd.uphjek.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gww.jqgufenzy.top

TS:   // 同 JS
来源：http://pvb.haohaochexian.top

Java: synchronized (this) { shared++; }
来源：http://yjv.wangdashe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ocs.yfazqb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://dpv.jqgufenzy.top

C#:   lock (gate) { shared++; }
来源：http://phw.tianlin.xyz

[O04] 定义异步函数并等待
来源：http://umb.jinqigfzy.top

Py:   async def f():⏎    await g()
来源：http://mmk.fktsv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hcz.hfpthk.cn

JS:   async function f() { await g(); }
来源：http://mwj.shzxlz.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zwn.aizwys.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ume.guannengcc.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ikg.shangyingyoupin.top

Ruby: # 用 Fiber 或 async gem
来源：http://zwt.jqgufenzy.top

C#:   async Task F() { await G(); }
来源：http://uns.jinqigfzy.top

[O05] 并发执行并等待全部完成
来源：http://sjz.jinyuanbaomall.cn

Py:   asyncio.gather(*tasks)
来源：http://ehq.jinghuilouyu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bnm.tianlin.xyz

JS:   await Promise.all(tasks)
来源：http://yow.ybcxt.top

TS:   await Promise.all(tasks)
来源：http://cod.hfpthk.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gwa.tianlin.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ocm.hammf.cn

Ruby: threads.map(&:join)
来源：http://rjk.sysykeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://cor.cucudq.cn

[O06] 使用进程池
来源：http://cot.0kj1m.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iyq.cdnleiting.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ipg.wangdashe.top

JS:   // child_process / cluster 模块
来源：http://cet.haohaochexian.top

TS:   // child_process / cluster 模块
来源：http://mku.havefunace.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://iuw.dashuyun.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yxp.fengsongda.top

Ruby: // fork 块
来源：http://nmb.snrcjt.cn

C#:   Parallel.For
来源：http://hqh.sweek.top

================================================================================
来源：http://hke.chenzaomai.com

P. 常用工具函数
来源：http://gxq.gzhubu.top

================================================================================
来源：http://bxw.nanxuanxn.top

[P01] 生成 UUID
来源：http://jjz.andypj.xyz

Py:   str(uuid.uuid4())
来源：http://mqt.smart0.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pwc.xinyue.icu

JS:   crypto.randomUUID()
来源：http://ggo.jyoumei.cn

TS:   crypto.randomUUID()
来源：http://icv.vqdsnc.cn

Java: UUID.randomUUID().toString()
来源：http://tym.xziqi.cn

Go:   // 用 github.com/google/uuid
来源：http://jws.shanyushiyangtech.top

Ruby: SecureRandom.uuid
来源：http://djn.hesvh.cn

C#:   Guid.NewGuid().ToString()
来源：http://npe.hammf.cn

[P02] MD5 / SHA256 摘要
来源：http://opx.jqgfzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pnk.yuxming.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fhb.uphjek.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nep.tarul.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ita.haohaochexian.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cjn.hongshengwenyu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zjk.chenjidiqi.icu

Ruby: Digest::SHA256.hexdigest(s)
来源：http://heg.shanyushiyangkeji.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jfc.bbcook.cn

[P03] 生成短随机字符串
来源：http://ysn.nanxinkj.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yyn.jiagoushi.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xyx.vqdsnc.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tqs.shzxlz.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eyr.hnxiangtu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://snf.xinyue.icu

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://khj.ydjk.org.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kre.316326.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rhj.tianlin.xyz

[P04] 求长度
来源：http://tie.iojbl.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vzu.hcnkem.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xfa.wangshuangyany.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nbj.meibo888.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vnz.hnqzz.top

Java: list.size();  map.size();  s.length()
来源：http://vaj.yongpay.top

Go:   len(arr);  len(m)
来源：http://xfk.xuetiantiany.cn

Ruby: x.length;  x.size
来源：http://wlt.yfazqb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://lsr.0kj1m.cn

[P05] 判断两个对象内容是否相等
来源：http://qtq.jqgfzy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://yiy.9152youxi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://esf.hnqzz.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qam.cheryme.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ivz.daxiang520.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://chf.jinqigfzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://dek.ybcxt.top

Ruby: a == b
来源：http://rri.xuetiantiany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kds.zhaomingkeji.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://url.fktsv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yzl.52xcode.cn

PHP:  if (empty($x)) {}
来源：http://tbp.hfpthk.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://foa.xinyue.icu

TS:   if (x == null) {}
来源：http://xcb.yangfankeji.com

Java: if (x == null || x.isEmpty()) {}
来源：http://fhc.chenjidiqi.icu

Go:   if x == nil {}
来源：http://iiq.xingfuxueyuan.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kqc.ybcxt.top

C#:   if (x is null) {}
来源：http://usn.zdqjudy.top

[P07] 防抖与节流
来源：http://uwb.iojbl.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nnt.jlsjyb.cn

PHP:  // 手写时间戳比较
来源：http://imi.yuxming.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://akg.ydzc1.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nzf.0kj1m.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ojk.xuanzx.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bha.aibaodan.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bhj.c1oappe.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://esm.yuxming.cn

[P08] 处理浮点精度问题
来源：http://yug.nanxinkj.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fbf.daria6918.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ihk.pycfn.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xgb.redwolf501.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xfh.gotoacloud.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://puu.fzhhl.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bah.xingfuxueyuan.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lbd.xuetiantiany.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hge.uphjek.com

================================================================================
来源：http://tql.pycfn.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dzc.fzhhl.top

================================================================================
来源：http://fry.hesvh.cn

[Q01] 创建表
来源：http://quu.xingfuxueyuan.xyz

CREATE TABLE users (
来源：http://dvl.zhiwuduotai.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://odr.yj20258888.top

name VARCHAR(50) NOT NULL,
来源：http://agt.yueranfly.top

email VARCHAR(100) UNIQUE,
来源：http://zad.zhixingplan.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://exx.dianchejie.cn

);
来源：http://qqf.fanxiaobao.xyz

[Q02] 创建带外键的表
来源：http://vsl.gotoacloud.top

CREATE TABLE orders (
来源：http://dpd.aibaodan.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jsh.xuetiantiany.cn

user_id INT NOT NULL,
来源：http://zvh.gzhubu.top

amount DECIMAL(10, 2),
来源：http://fan.jinyuanbaomall.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ecy.nwbrower.top

);
来源：http://zbx.shanyushiyangkeji.top

[Q03] 增加列
来源：http://qwa.hfpthk.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gxl.yonumen.top

[Q04] 修改列类型
来源：http://bun.zhengqikj.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wsl.fehbvm.com

[Q05] 重命名列
来源：http://jyl.gzhubu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rzw.hcnkem.com

[Q06] 删除列
来源：http://crz.vqdsnc.cn

ALTER TABLE users DROP COLUMN age;
来源：http://unb.haohaochexian.top

[Q07] 删除表
来源：http://wim.haohaochexian.top

DROP TABLE IF EXISTS orders;
来源：http://dpi.snrcjt.cn

[Q08] 创建普通索引
来源：http://vpb.cdnleiting.top

CREATE INDEX idx_users_email ON users(email);
来源：http://phr.yongpay.top

[Q09] 创建唯一索引
来源：http://rls.cucudq.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qsd.epnwcf.com

[Q10] 插入单行
来源：http://fqb.yanxiufei.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nef.xuetiantiany.cn

[Q11] 一次插入多行
来源：http://rpr.cheryme.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jbb.hcnkem.com

[Q12] 插入后取自增 ID
来源：http://wae.xingfuxueyuan.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://bol.c1oappe.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://owa.epnwcf.com

[Q13] 忽略重复插入
来源：http://zzx.ydjk.org.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zqb.epnwcf.com

[Q14] 存在则更新（upsert）
来源：http://wgo.vqdsnc.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wdr.hnxiangtu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fst.chenjidiqi.icu

[Q15] 查询全部
来源：http://kke.xingfuxueyuan.xyz

SELECT * FROM users;
来源：http://kpt.hammf.cn

[Q16] 查询指定列
来源：http://dey.zhijiandao.cn

SELECT id, name FROM users;
来源：http://nei.yj202588.top

[Q17] 条件查询
来源：http://dnh.xziqi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ghh.sweek.top

[Q18] 模糊匹配
来源：http://ffr.yangfankeji.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vlc.guannengcc.top

[Q19] 范围查询
来源：http://rln.pycfn.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lzr.0kj1m.cn

[Q20] IN 列表
来源：http://fbm.yvedp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ekd.hcnkem.com

[Q21] 空值判断
来源：http://uaj.quarkkingdee.top

SELECT * FROM users WHERE email IS NULL;
来源：http://iki.c1oappe.top

[Q22] 排序
来源：http://bcs.pycfn.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jyh.yj20258.top

[Q23] 分页
来源：http://wfw.hesvh.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wxk.sjlbkw.cn

[Q24] 去重
来源：http://gtm.yonumen.top

SELECT DISTINCT city FROM users;
来源：http://uow.zhijiandao.cn

[Q25] 只取前 N 条
来源：http://okx.pycfn.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zrt.nwbrower.top

[Q26] 计数
来源：http://yju.ydzc1.top

SELECT COUNT(*) FROM users;
来源：http://wat.sxryk.cn

[Q27] 条件计数
来源：http://lim.hysaishi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uqg.xuanzx.com

[Q28] 求和与平均
来源：http://hlw.shangyingyoupin.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://edk.hesvh.cn

[Q29] 最大最小值
来源：http://cfz.xinyue.icu

SELECT MAX(age), MIN(age) FROM users;
来源：http://lxu.52xcode.cn

[Q30] 分组统计
来源：http://dhv.cqqwz.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wtv.xingfuxueyuan.xyz

[Q31] 分组后过滤
来源：http://dcz.zhiwuduotai.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qtc.chenzaomai.com

[Q32] 分组拼接字符串
来源：http://bzp.haohaochexian.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fnm.tian-w.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://urn.shanyushiyangtech.top

[Q33] 多列分组
来源：http://hfy.cdnleiting.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rwv.snrcjt.cn

[Q34] 每组取第一条
来源：http://ijg.316326.xyz

SELECT * FROM (
来源：http://geq.xuetiantiany.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nwe.aibaodan.cn

) t WHERE rn = 1;
来源：http://kop.daria6918.cn

[Q35] 内连接
来源：http://jqk.aibaodan.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gcs.yuxming.cn

[Q36] 左连接
来源：http://znq.zhijiandao.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://evw.ydzc1.top

[Q37] 右连接
来源：http://vyj.jinyuanbaomall.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://too.zhixingplan.top

[Q38] 全外连接（PostgreSQL）
来源：http://ebm.mhx1999.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uwu.xingfuxueyuan.xyz

[Q39] 自连接（查上下级）
来源：http://kjr.hammf.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vwq.ydjk.org.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bcp.jinqigufen.top

[Q40] 交叉连接（笛卡尔积）
来源：http://prj.c1oappe.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gdu.jqgufenzy.top

[Q41] 多表连接
来源：http://bqy.shzxlz.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qoy.iojbl.cn

JOIN users u ON u.id = o.user_id
来源：http://htm.mhx1999.top

JOIN products p ON p.id = o.product_id;
来源：http://xij.fanxiaobao.xyz

[Q42] 连接条件附加过滤
来源：http://dsx.vehdjk.com

SELECT u.name, o.amount FROM users u
来源：http://kli.hnqzz.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://olk.zhijiandao.cn

[Q43] 标量子查询
来源：http://bah.shangyingyoupin.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qdi.zycfv.cn

[Q44] IN 子查询
来源：http://elz.nanxinkj.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://smi.gogol.net.cn

[Q45] EXISTS 判断存在
来源：http://mzp.hammf.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qqr.chenjidiqi.icu

[Q46] NOT EXISTS 判断不存在
来源：http://oin.zdqjudy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hzd.yanxiufei.cn

[Q47] 与平均值比较
来源：http://gym.316326.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rnr.c1oappe.top

[Q48] CTE 公用表表达式
来源：http://mca.meibo888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nrq.ehwqpu.com

SELECT * FROM t WHERE c > 5;
来源：http://gwg.zdqjudy.top

[Q49] 更新单行
来源：http://beg.cdnleiting.top


<!-- 参考信息 -->