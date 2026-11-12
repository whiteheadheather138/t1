代发 wailian999

Py:   itertools.permutations(arr)
来源：http://nzy.uphjek.com

PHP:  // 手写递归交换
来源：http://nji.jinghuilouyu.cn

JS:   // 手写回溯递归
来源：http://jot.guowangkeji.top

TS:   // 手写回溯递归
来源：http://vln.zhaomingkeji.xyz

Java: // 手写回溯递归
来源：http://rgy.uphjek.com

Go:   // 手写回溯递归
来源：http://kth.yfazqb.com

Ruby: arr.permutation.to_a
来源：http://tjy.cdnleiting.top

C#:   // 手写回溯递归
来源：http://dmt.zhijiandao.cn

[N09] 栈与队列
来源：http://eyk.yfazqb.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://aln.uphjek.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uph.xziqi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ulf.sufxvd.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oof.meibo888.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rxp.hysaishi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://riv.xylfe.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qfh.svipenyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sru.cqqwz.cn

[N10] 链表节点定义
来源：http://vpd.jqgufenzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://raj.ydjk.org.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fbk.bbcook.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kln.birdmap.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://czk.dianchejie.cn

Java: class Node { int v; Node next; }
来源：http://igv.jianghu66.top

Go:   type Node struct { V int; Next *Node }
来源：http://tpo.fengsongda.top

Ruby: Node = Struct.new(:v, :next)
来源：http://sml.smart0.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://pqh.hfpthk.cn

[N11] 二叉树中序遍历
来源：http://tjt.birdmap.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zvd.aibaodan.cn

PHP:  // 手写递归函数
来源：http://zwy.ppjwa.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nki.tarul.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kcr.smart0.xyz

Java: // 手写递归
来源：http://iaz.vehdjk.com

Go:   // 手写递归
来源：http://ule.jlsjyb.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ahh.jiagoushi.top

C#:   // 手写递归
来源：http://cqd.fanxiaobao.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tla.nanxinkj.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qta.shzxlz.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gys.jyoumei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://luw.ybcxt.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://obi.yfazqb.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sip.jqgufenzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://psv.sxryk.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ijd.shanyushiyangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zfn.yuxming.cn

================================================================================
来源：http://ikf.quarkkingdee.top

O. 并发与异步
来源：http://vzd.wangshuangyany.cn

================================================================================
来源：http://hbd.fengsongda.top

[O01] 启动一个线程
来源：http://zwd.vqdsnc.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pdf.hnqzz.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kkq.sysykeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yoi.kuanghao11.cn

TS:   // 同 JS
来源：http://zwf.ydjk.org.cn

Java: new Thread(() -> f()).start()
来源：http://jzn.chenzaomai.com

Go:   go f()
来源：http://tbw.zhijiandao.cn

Ruby: Thread.new { f }
来源：http://nhn.vqdsnc.cn

C#:   Task.Run(() => F());
来源：http://tju.zdqjudy.top

[O02] 使用线程池
来源：http://xtq.xuanzx.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qvm.hfpthk.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vkv.sjlbkw.cn

JS:   // worker_threads 线程池
来源：http://ipw.shuidangran.top

TS:   // worker_threads 线程池
来源：http://rob.fzhhl.top

Java: Executors.newFixedThreadPool(4)
来源：http://qwj.pycfn.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ssm.shangyingyoupin.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gno.yvedp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ktl.hysaishi.cn

[O03] 加锁保护共享数据
来源：http://yjy.jinghuilouyu.cn

Py:   with lock: shared += 1
来源：http://ubu.yanxiufei.cn

PHP:  // 用 flock() 做文件锁
来源：http://zpc.fehbvm.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yay.xylfe.cn

TS:   // 同 JS
来源：http://iab.shanyushiyangtech.top

Java: synchronized (this) { shared++; }
来源：http://qrn.hywenlv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sbt.quarkkingdee.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://dmj.hnxiangtu.top

C#:   lock (gate) { shared++; }
来源：http://afa.shangyingyoupin.top

[O04] 定义异步函数并等待
来源：http://joa.daria6918.cn

Py:   async def f():⏎    await g()
来源：http://viu.haohaochexian.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://afp.zhiwuduotai.top

JS:   async function f() { await g(); }
来源：http://kmc.fengsongda.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://wwx.jianghu66.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yan.ydjk.org.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pva.ydzc1.top

Ruby: # 用 Fiber 或 async gem
来源：http://mng.yj20258888.top

C#:   async Task F() { await G(); }
来源：http://war.cashguo.top

[O05] 并发执行并等待全部完成
来源：http://vqp.shanyushiyangkeji.top

Py:   asyncio.gather(*tasks)
来源：http://xtt.andypj.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uig.ctjpmb.com

JS:   await Promise.all(tasks)
来源：http://yco.yongpay.top

TS:   await Promise.all(tasks)
来源：http://vgn.vqdsnc.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sdd.nwbrower.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pjx.yj20258.top

Ruby: threads.map(&:join)
来源：http://iwu.52xcode.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ohd.jinghuilouyu.cn

[O06] 使用进程池
来源：http://vza.52xcode.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mzs.fengsongda.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ltr.jqgfzy.top

JS:   // child_process / cluster 模块
来源：http://kff.ctjpmb.com

TS:   // child_process / cluster 模块
来源：http://ugp.jyoumei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nmp.xziqi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zax.yuxming.cn

Ruby: // fork 块
来源：http://nhf.ppjwa.cn

C#:   Parallel.For
来源：http://drl.sufxvd.cn

================================================================================
来源：http://qzc.hysaishi.cn

P. 常用工具函数
来源：http://fre.yj20258.top

================================================================================
来源：http://rxl.yongpay.top

[P01] 生成 UUID
来源：http://svj.yfazqb.com

Py:   str(uuid.uuid4())
来源：http://baz.sweek.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://upq.ydzc1.top

JS:   crypto.randomUUID()
来源：http://aty.gotoacloud.top

TS:   crypto.randomUUID()
来源：http://bqv.52xcode.cn

Java: UUID.randomUUID().toString()
来源：http://wou.hcnkem.com

Go:   // 用 github.com/google/uuid
来源：http://ecs.vehdjk.com

Ruby: SecureRandom.uuid
来源：http://jhz.jinqigufen.top

C#:   Guid.NewGuid().ToString()
来源：http://yld.yvedp.cn

[P02] MD5 / SHA256 摘要
来源：http://xlm.hesvh.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://whm.ivvv.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://nez.cheryme.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sbw.sxryk.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yvi.cashguo.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mdw.gotoacloud.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://itl.ydzc1.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wui.xingfuxueyuan.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qhc.yfazqb.com

[P03] 生成短随机字符串
来源：http://yce.uphjek.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://afg.yuanzhike.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gdt.jinghuilouyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vax.hongshengwenyu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lqv.ywan-chungtsiang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://iuc.jinghuilouyu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ujb.jlsjyb.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://dsu.uphjek.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gjn.xinyue.icu

[P04] 求长度
来源：http://uce.zhiwuduotai.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mzl.jyoumei.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fun.uphjek.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yfr.hongshengwenyu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nme.chenzaomai.com

Java: list.size();  map.size();  s.length()
来源：http://vof.fanxiaobao.xyz

Go:   len(arr);  len(m)
来源：http://bgu.xziqi.cn

Ruby: x.length;  x.size
来源：http://wqx.bjfxy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://pju.0kj1m.cn

[P05] 判断两个对象内容是否相等
来源：http://lwl.svipenyu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://btg.ydzc1.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dcx.nanxuanxn.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vfu.fzhhl.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xpk.sjlbkw.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://muf.jianghu66.top

Go:   reflect.DeepEqual(a, b)
来源：http://wzj.snrcjt.cn

Ruby: a == b
来源：http://dri.shzxlz.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wjl.ydzc1.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://umr.pycfn.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wpt.iojbl.cn

PHP:  if (empty($x)) {}
来源：http://yui.jinqigfzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://obq.316326.xyz

TS:   if (x == null) {}
来源：http://rhk.meibo888.top

Java: if (x == null || x.isEmpty()) {}
来源：http://kfn.hnxiangtu.top

Go:   if x == nil {}
来源：http://sef.ehwqpu.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://khm.pengpengdd.cyou

C#:   if (x is null) {}
来源：http://gxn.hfpthk.cn

[P07] 防抖与节流
来源：http://ffe.zhoulong.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wdn.52xcode.cn

PHP:  // 手写时间戳比较
来源：http://gfu.zhijiandao.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mpa.jiagoushi.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lhy.0kj1m.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mes.zhongyouzk.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zbc.cucudq.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lpq.zhiwuduotai.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pxw.hongshengwenyu.top

[P08] 处理浮点精度问题
来源：http://erv.ctjpmb.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fky.yj202588.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qoi.zhongyouzk.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qjm.ydzc1.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dxk.hfpthk.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ixz.jlsjyb.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xie.sufxvd.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ety.hfpthk.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://afi.yongpay.top

================================================================================
来源：http://sah.guowangkeji.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vau.yongpay.top

================================================================================
来源：http://iig.shuidangran.top

[Q01] 创建表
来源：http://wmk.yvedp.cn

CREATE TABLE users (
来源：http://lrk.shuidangran.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://brt.sjlbkw.cn

name VARCHAR(50) NOT NULL,
来源：http://kxi.ppjwa.cn

email VARCHAR(100) UNIQUE,
来源：http://daa.jinqigufen.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jno.cucudq.cn

);
来源：http://kiz.ctjpmb.com

[Q02] 创建带外键的表
来源：http://fgp.52xcode.cn

CREATE TABLE orders (
来源：http://xjg.yonumen.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zin.yfazqb.com

user_id INT NOT NULL,
来源：http://htq.aibaodan.cn

amount DECIMAL(10, 2),
来源：http://dgx.cdnleiting.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yst.pycfn.com

);
来源：http://ltq.zhaomingkeji.xyz

[Q03] 增加列
来源：http://nur.xuetiantiany.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yzd.fzhhl.top

[Q04] 修改列类型
来源：http://gvp.yuxming.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://iic.vehdjk.com

[Q05] 重命名列
来源：http://jhl.yj20258.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ued.yj20258.top

[Q06] 删除列
来源：http://onk.xylfe.cn

ALTER TABLE users DROP COLUMN age;
来源：http://czb.jiagoushi.top

[Q07] 删除表
来源：http://pfl.yongpay.top

DROP TABLE IF EXISTS orders;
来源：http://tkk.jyoumei.cn

[Q08] 创建普通索引
来源：http://ift.hysaishi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lpz.feifeiyinyue.top

[Q09] 创建唯一索引
来源：http://ucl.xylfe.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zum.jqgufenzy.top

[Q10] 插入单行
来源：http://gar.redwolf501.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gjj.hnxiangtu.top

[Q11] 一次插入多行
来源：http://uat.redwolf501.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hbk.jqgufenzy.top

[Q12] 插入后取自增 ID
来源：http://mml.hysaishi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qpb.chenzaomai.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qmt.xylfe.cn

[Q13] 忽略重复插入
来源：http://jja.shuidangran.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nvj.ybcxt.top

[Q14] 存在则更新（upsert）
来源：http://gji.gogol.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zzz.pycfn.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xwo.sxryk.cn

[Q15] 查询全部
来源：http://sfl.sjlbkw.cn

SELECT * FROM users;
来源：http://xta.epnwcf.com

[Q16] 查询指定列
来源：http://vzs.chenlongwang.top

SELECT id, name FROM users;
来源：http://cti.ydzc1.top

[Q17] 条件查询
来源：http://ogh.vqdsnc.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kcg.yfazqb.com

[Q18] 模糊匹配
来源：http://uny.gzhubu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kon.aizwys.cn

[Q19] 范围查询
来源：http://aqg.hesvh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://iej.tarul.cn

[Q20] IN 列表
来源：http://xlt.xingfuxueyuan.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qnd.yueranfly.top

[Q21] 空值判断
来源：http://ocn.0kj1m.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bqd.uphjek.com

[Q22] 排序
来源：http://iac.dianchejie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://orh.yongpay.top

[Q23] 分页
来源：http://uxg.bbcook.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bjv.zhoulong.xyz

[Q24] 去重
来源：http://rjv.yj20258888.top

SELECT DISTINCT city FROM users;
来源：http://jfq.wangdashe.top

[Q25] 只取前 N 条
来源：http://sbe.fktsv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ijl.ydjk.org.cn

[Q26] 计数
来源：http://ney.yfazqb.com

SELECT COUNT(*) FROM users;
来源：http://cha.hnxiangtu.top

[Q27] 条件计数
来源：http://jzi.tarul.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zlg.fengsongda.top

[Q28] 求和与平均
来源：http://mhz.hnxiangtu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oew.daria6918.cn

[Q29] 最大最小值
来源：http://hcd.yvedp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://prf.tarul.cn

[Q30] 分组统计
来源：http://wlq.hongshengwenyu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://peh.yj202588.top

[Q31] 分组后过滤
来源：http://ppo.zycfv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xyb.fanxiaobao.xyz

[Q32] 分组拼接字符串
来源：http://ggb.shanyushiyangkeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dcr.hfpthk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://yku.yuxming.cn

[Q33] 多列分组
来源：http://pbi.xinyue.icu

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rgr.nanxinkj.top

[Q34] 每组取第一条
来源：http://dcj.jinyuanbaomall.cn

SELECT * FROM (
来源：http://yzz.tianlin.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jed.hfpthk.cn

) t WHERE rn = 1;
来源：http://yuf.zhongyouzk.top

[Q35] 内连接
来源：http://rvt.xingfuxueyuan.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://iyz.quarkkingdee.top

[Q36] 左连接
来源：http://bqb.dianchejie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tsc.jinghuilouyu.cn

[Q37] 右连接
来源：http://xop.zhixingplan.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dbu.sweek.top

[Q38] 全外连接（PostgreSQL）
来源：http://nbi.smart0.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://skf.jinqigfzy.top

[Q39] 自连接（查上下级）
来源：http://ycm.aibaodan.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zna.yj20258.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://erv.yj202588.top

[Q40] 交叉连接（笛卡尔积）
来源：http://irt.yvedp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hur.ctjpmb.com

[Q41] 多表连接
来源：http://dkk.redwolf501.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://iem.xuetiantiany.cn

JOIN users u ON u.id = o.user_id
来源：http://fcp.ivvv.top

JOIN products p ON p.id = o.product_id;
来源：http://ixm.gotoacloud.top

[Q42] 连接条件附加过滤
来源：http://kkk.hcnkem.com

SELECT u.name, o.amount FROM users u
来源：http://gfb.jinqigfzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bkk.svipenyu.cn

[Q43] 标量子查询
来源：http://hwi.zhengqikj.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://svo.zhongyouzk.top

[Q44] IN 子查询
来源：http://fbj.epnwcf.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mjq.fengsongda.top

[Q45] EXISTS 判断存在
来源：http://udf.cashguo.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cup.hammf.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jgs.jinghuilouyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uoq.tarul.cn

[Q47] 与平均值比较
来源：http://epw.hysaishi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mrm.ehwqpu.com

[Q48] CTE 公用表表达式
来源：http://cfv.fanxiaobao.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://iej.mhx1999.top

SELECT * FROM t WHERE c > 5;
来源：http://dzc.fktsv.cn

[Q49] 更新单行
来源：http://wzc.yj202588.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://epn.hywenlv.cn

[Q50] 批量更新
来源：http://nwz.daria6918.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zfx.xinyue.icu

[Q51] 用子查询更新
来源：http://egb.jinqigfzy.top


<!-- 参考信息 -->