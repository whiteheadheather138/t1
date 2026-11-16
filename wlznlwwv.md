代发 wailian999

Java: // 手写回溯递归
来源：http://qsq.sxryk.cn

Go:   // 手写回溯递归
来源：http://psb.nanxuanxn.top

Ruby: arr.permutation.to_a
来源：http://gxu.sjlbkw.cn

C#:   // 手写回溯递归
来源：http://otx.hnxiangtu.top

[N09] 栈与队列
来源：http://qye.shanyushiyangtech.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sqr.chenjidiqi.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nsy.andypj.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cts.fengsongda.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qyl.fzhhl.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dit.vehdjk.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bsm.ctjpmb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kuc.hesvh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yeo.0kj1m.cn

[N10] 链表节点定义
来源：http://plh.fengsongda.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://snx.dashuyun.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qxw.yuxming.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bvx.daxiang520.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ege.jinqigfzy.top

Java: class Node { int v; Node next; }
来源：http://loq.andypj.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://gpv.uphjek.com

Ruby: Node = Struct.new(:v, :next)
来源：http://ewr.yuxming.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wgd.zhengqikj.top

[N11] 二叉树中序遍历
来源：http://kcj.gzhubu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kmp.yj20258.top

PHP:  // 手写递归函数
来源：http://abv.uphjek.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kao.sufxvd.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rgv.jlsjyb.cn

Java: // 手写递归
来源：http://thi.hysaishi.cn

Go:   // 手写递归
来源：http://fde.zhaomingkeji.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fpn.yj20258888.top

C#:   // 手写递归
来源：http://doa.hesvh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fom.aizwys.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jvg.zhengqikj.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pmp.gogol.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mtt.jiagoushi.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fls.vqdsnc.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ufp.ywan-chungtsiang.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lsn.kuanghao11.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ybq.fzhhl.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gva.tianlin.xyz

================================================================================
来源：http://lff.nwbrower.top

O. 并发与异步
来源：http://odw.hfpthk.cn

================================================================================
来源：http://fpj.daxiang520.top

[O01] 启动一个线程
来源：http://nsu.daria6918.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kik.fehbvm.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://avl.gzhubu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ftb.chenlongwang.top

TS:   // 同 JS
来源：http://osj.fanxiaobao.xyz

Java: new Thread(() -> f()).start()
来源：http://kgr.shuidangran.top

Go:   go f()
来源：http://qnj.mhx1999.top

Ruby: Thread.new { f }
来源：http://kis.nanxinkj.top

C#:   Task.Run(() => F());
来源：http://zvm.uphjek.com

[O02] 使用线程池
来源：http://lww.pycfn.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zlz.fehbvm.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kdo.wangdashe.top

JS:   // worker_threads 线程池
来源：http://ebs.0kj1m.cn

TS:   // worker_threads 线程池
来源：http://vgh.hcnkem.com

Java: Executors.newFixedThreadPool(4)
来源：http://ykt.aibaodan.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yev.vehdjk.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tkn.epnwcf.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pyq.hfpthk.cn

[O03] 加锁保护共享数据
来源：http://tth.jinqigfzy.top

Py:   with lock: shared += 1
来源：http://ybw.ctjpmb.com

PHP:  // 用 flock() 做文件锁
来源：http://njf.tanke756.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xbk.shanyushiyangkeji.top

TS:   // 同 JS
来源：http://oek.hongshengwenyu.top

Java: synchronized (this) { shared++; }
来源：http://dhh.tarul.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://noy.birdmap.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://hlt.daria6918.cn

C#:   lock (gate) { shared++; }
来源：http://izp.yuxming.cn

[O04] 定义异步函数并等待
来源：http://spk.jianghu66.top

Py:   async def f():⏎    await g()
来源：http://wxy.hfpthk.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://usz.shangyingyoupin.top

JS:   async function f() { await g(); }
来源：http://xxm.yj202588.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://faj.sjlbkw.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mat.aibaodan.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oaf.zhixingplan.top

Ruby: # 用 Fiber 或 async gem
来源：http://nol.jlsjyb.cn

C#:   async Task F() { await G(); }
来源：http://aqc.dianchejie.cn

[O05] 并发执行并等待全部完成
来源：http://tpi.ybcxt.top

Py:   asyncio.gather(*tasks)
来源：http://mlu.xuanzx.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mmn.mhx1999.top

JS:   await Promise.all(tasks)
来源：http://jpg.pycfn.com

TS:   await Promise.all(tasks)
来源：http://zul.ehwqpu.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sxk.zdbjq.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://eck.hywenlv.cn

Ruby: threads.map(&:join)
来源：http://xrr.meibo888.top

C#:   await Task.WhenAll(t1, t2)
来源：http://efq.tian-w.cn

[O06] 使用进程池
来源：http://ogd.ywan-chungtsiang.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ovg.hammf.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://sen.aizwys.cn

JS:   // child_process / cluster 模块
来源：http://jse.hnqzz.top

TS:   // child_process / cluster 模块
来源：http://yyh.fengsongda.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://iru.yvedp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://onw.zycfv.cn

Ruby: // fork 块
来源：http://qxi.hnxiangtu.top

C#:   Parallel.For
来源：http://qpx.jianghu66.top

================================================================================
来源：http://qoa.cashguo.top

P. 常用工具函数
来源：http://ibv.daria6918.cn

================================================================================
来源：http://gxg.yueranfly.top

[P01] 生成 UUID
来源：http://pio.ivvv.top

Py:   str(uuid.uuid4())
来源：http://evh.0kj1m.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://stw.yuanzhike.top

JS:   crypto.randomUUID()
来源：http://nad.gaohongyu789.top

TS:   crypto.randomUUID()
来源：http://kyq.ydzc1.top

Java: UUID.randomUUID().toString()
来源：http://rgs.cucudq.cn

Go:   // 用 github.com/google/uuid
来源：http://uwo.c1oappe.top

Ruby: SecureRandom.uuid
来源：http://pvd.zhoulong.xyz

C#:   Guid.NewGuid().ToString()
来源：http://rmp.hesvh.cn

[P02] MD5 / SHA256 摘要
来源：http://ddn.yfazqb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ppg.xuetiantiany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ope.sweek.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://scj.jianghu66.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qnr.zhengqikj.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zdq.tanke756.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rqd.feifeiyinyue.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qmf.zhijiandao.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://meb.hongshengwenyu.top

[P03] 生成短随机字符串
来源：http://pmi.pycfn.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jcz.guannengcc.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rpu.zhengqikj.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sat.zhengqikj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zii.zdqjudy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rst.ppjwa.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://buh.meibo888.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://hde.jyoumei.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ggw.cheryme.top

[P04] 求长度
来源：http://feq.xuetiantiany.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xnz.cqqwz.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ltl.gzhubu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lru.yj202588.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hzd.hfpthk.cn

Java: list.size();  map.size();  s.length()
来源：http://mws.yueranfly.top

Go:   len(arr);  len(m)
来源：http://zgk.aibaodan.cn

Ruby: x.length;  x.size
来源：http://tgv.haohaochexian.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://rgf.birdmap.top

[P05] 判断两个对象内容是否相等
来源：http://pdi.ydjk.org.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gge.jinqigufen.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yqm.chenzaomai.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yst.cqqwz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://iqk.vqdsnc.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://oss.xuanzx.com

Go:   reflect.DeepEqual(a, b)
来源：http://rop.jyoumei.cn

Ruby: a == b
来源：http://vet.aibaodan.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://acs.iojbl.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://css.jinyuanbaomall.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pqs.yuxming.cn

PHP:  if (empty($x)) {}
来源：http://gmj.cashguo.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://smr.cucudq.cn

TS:   if (x == null) {}
来源：http://xxl.shangyingyoupin.top

Java: if (x == null || x.isEmpty()) {}
来源：http://jjd.xuetiantiany.cn

Go:   if x == nil {}
来源：http://yks.jinghuilouyu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fty.havefunace.top

C#:   if (x is null) {}
来源：http://dsn.vehdjk.com

[P07] 防抖与节流
来源：http://baj.ctjpmb.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rpm.wangdashe.top

PHP:  // 手写时间戳比较
来源：http://hjf.sufxvd.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pzq.yvedp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://slg.quarkkingdee.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://shw.hysaishi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ufi.bbcook.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://frc.yj20258888.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ykw.gogol.net.cn

[P08] 处理浮点精度问题
来源：http://xaj.xuetiantiany.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hws.wangshuangyany.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gwu.zhengqikj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qgc.shuidangran.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hlo.yj202588.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://smh.yangfankeji.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cdf.daria6918.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gfc.hongshengwenyu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zww.cdnleiting.top

================================================================================
来源：http://xbw.ppjwa.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nns.wangshuangyany.cn

================================================================================
来源：http://bkw.xinyue.icu

[Q01] 创建表
来源：http://xzr.shuidangran.top

CREATE TABLE users (
来源：http://rqg.sweek.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wjk.svipenyu.cn

name VARCHAR(50) NOT NULL,
来源：http://zah.zhixingplan.top

email VARCHAR(100) UNIQUE,
来源：http://kvq.hcnkem.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dvn.xziqi.cn

);
来源：http://lld.birdmap.top

[Q02] 创建带外键的表
来源：http://wnw.kuanghao11.cn

CREATE TABLE orders (
来源：http://qra.nanxuanxn.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pta.zhiwuduotai.top

user_id INT NOT NULL,
来源：http://erz.zhaomingkeji.xyz

amount DECIMAL(10, 2),
来源：http://ewb.sufxvd.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lkv.hnxiangtu.top

);
来源：http://zis.shuidangran.top

[Q03] 增加列
来源：http://zgv.pycfn.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://stf.316326.xyz

[Q04] 修改列类型
来源：http://zwn.sufxvd.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rgt.9152youxi.cn

[Q05] 重命名列
来源：http://uzk.tarul.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nfv.daria6918.cn

[Q06] 删除列
来源：http://yxv.fanxiaobao.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://nql.jinyuanbaomall.cn

[Q07] 删除表
来源：http://aoi.jinqigufen.top

DROP TABLE IF EXISTS orders;
来源：http://ohp.yuanzhike.top

[Q08] 创建普通索引
来源：http://mex.sjlbkw.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fax.yuxming.cn

[Q09] 创建唯一索引
来源：http://ccc.yj202588.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mnr.jqgfzy.top

[Q10] 插入单行
来源：http://gsf.chenzaomai.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kzx.tarul.cn

[Q11] 一次插入多行
来源：http://suw.0kj1m.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mxp.zhaomingkeji.xyz

[Q12] 插入后取自增 ID
来源：http://ahd.birdmap.top

INSERT INTO users (name) VALUES ('C');
来源：http://tgf.shzxlz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nun.cdnleiting.top

[Q13] 忽略重复插入
来源：http://cbg.gzhubu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bia.hnqzz.top

[Q14] 存在则更新（upsert）
来源：http://zle.ivvv.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zyb.yuxming.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ylp.316326.xyz

[Q15] 查询全部
来源：http://aca.jiagoushi.top

SELECT * FROM users;
来源：http://vsp.yuanzhike.top

[Q16] 查询指定列
来源：http://nxe.gogol.net.cn

SELECT id, name FROM users;
来源：http://zti.jinyuanbaomall.cn

[Q17] 条件查询
来源：http://eqg.nwbrower.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vbj.meibo888.top

[Q18] 模糊匹配
来源：http://crm.dianchejie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bln.cqqwz.cn

[Q19] 范围查询
来源：http://dob.ybcxt.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ymd.cashguo.top

[Q20] IN 列表
来源：http://ida.c1oappe.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://odl.zdbjq.cn

[Q21] 空值判断
来源：http://xkd.ydzc1.top

SELECT * FROM users WHERE email IS NULL;
来源：http://fde.zhixingplan.top

[Q22] 排序
来源：http://jpa.daxiang520.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ofh.ywan-chungtsiang.top

[Q23] 分页
来源：http://jds.bbcook.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nbp.epnwcf.com

[Q24] 去重
来源：http://tve.jqgfzy.top

SELECT DISTINCT city FROM users;
来源：http://wqk.chenzaomai.com

[Q25] 只取前 N 条
来源：http://vqd.jqgufenzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ucr.mhx1999.top

[Q26] 计数
来源：http://rum.daria6918.cn

SELECT COUNT(*) FROM users;
来源：http://tog.daxiang520.top

[Q27] 条件计数
来源：http://ozb.bbcook.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jsp.jinqigfzy.top

[Q28] 求和与平均
来源：http://ewk.fanxiaobao.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bqz.aibaodan.cn

[Q29] 最大最小值
来源：http://zdq.cqqwz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wgp.vehdjk.com

[Q30] 分组统计
来源：http://tou.ydjk.org.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://urn.jqgufenzy.top

[Q31] 分组后过滤
来源：http://scf.vehdjk.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fgb.hnqzz.top

[Q32] 分组拼接字符串
来源：http://oyj.jinqigufen.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xez.vqdsnc.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lmk.redwolf501.top

[Q33] 多列分组
来源：http://ybq.svipenyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bok.sweek.top

[Q34] 每组取第一条
来源：http://lsf.fzhhl.top

SELECT * FROM (
来源：http://qfj.cqqwz.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sio.hysaishi.cn

) t WHERE rn = 1;
来源：http://zpc.tarul.cn

[Q35] 内连接
来源：http://xcs.gaohongyu789.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kit.zhengqikj.top

[Q36] 左连接
来源：http://vwu.jinqigufen.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dui.hfpthk.cn

[Q37] 右连接
来源：http://clr.epnwcf.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vij.bbcook.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jkj.shuidangran.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://prq.andypj.xyz

[Q39] 自连接（查上下级）
来源：http://qnh.chenjidiqi.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://xsg.chenzaomai.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vei.zhongyouzk.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xbh.yfazqb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gev.ivvv.top

[Q41] 多表连接
来源：http://cwt.hammf.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gvk.jinghuilouyu.cn

JOIN users u ON u.id = o.user_id
来源：http://qfw.yanxiufei.cn

JOIN products p ON p.id = o.product_id;
来源：http://mbh.zdbjq.cn

[Q42] 连接条件附加过滤
来源：http://rrh.yuanzhike.top

SELECT u.name, o.amount FROM users u
来源：http://dck.zhengqikj.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rlh.meibo888.top

[Q43] 标量子查询
来源：http://yxv.dashuyun.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kfr.zhoulong.xyz

[Q44] IN 子查询
来源：http://opc.xuetiantiany.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xgy.jianghu66.top

[Q45] EXISTS 判断存在
来源：http://yyp.gogol.net.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kvb.yj202588.top

[Q46] NOT EXISTS 判断不存在
来源：http://lsk.ywan-chungtsiang.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cxt.yj202588.top

[Q47] 与平均值比较
来源：http://tmr.0kj1m.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qpr.zhongyouzk.top

[Q48] CTE 公用表表达式
来源：http://aww.pycfn.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dor.jinqigfzy.top

SELECT * FROM t WHERE c > 5;
来源：http://gko.shuidangran.top

[Q49] 更新单行
来源：http://eta.yuanzhike.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bil.cashguo.top

[Q50] 批量更新
来源：http://gpd.chenlongwang.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rpv.shuidangran.top

[Q51] 用子查询更新
来源：http://azl.chenjidiqi.icu

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://eay.hammf.cn

[Q52] 删除指定行
来源：http://etp.jyoumei.cn

DELETE FROM users WHERE id = 10;
来源：http://swv.hongshengwenyu.top

[Q53] 按条件删除
来源：http://ywl.chenzaomai.com


<!-- 参考信息 -->