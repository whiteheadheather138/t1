代发 wailian999

Py:   itertools.permutations(arr)
来源：http://qyu.jyoumei.cn

PHP:  // 手写递归交换
来源：http://vpe.chenjidiqi.icu

JS:   // 手写回溯递归
来源：http://mbt.shuidangran.top

TS:   // 手写回溯递归
来源：http://luq.daxiang520.top

Java: // 手写回溯递归
来源：http://dew.hysaishi.cn

Go:   // 手写回溯递归
来源：http://qmf.dianchejie.cn

Ruby: arr.permutation.to_a
来源：http://qik.kuanghao11.cn

C#:   // 手写回溯递归
来源：http://jon.bbcook.cn

[N09] 栈与队列
来源：http://cpz.hywenlv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://odb.jinqigufen.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vqv.tanke756.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zxg.cheryme.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fvm.feifeiyinyue.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mio.nwbrower.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://owt.tanke756.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cpc.cqqwz.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://exb.ydjk.org.cn

[N10] 链表节点定义
来源：http://wjc.jinghuilouyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vif.mhx1999.top

PHP:  class Node { public $v; public $next = null; }
来源：http://diz.meibo888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oyr.sysykeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gcf.9152youxi.cn

Java: class Node { int v; Node next; }
来源：http://zbo.shanyushiyangkeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://dqf.yj202588.top

Ruby: Node = Struct.new(:v, :next)
来源：http://fdm.yuanzhike.top

C#:   class Node { public int V; public Node? Next; }
来源：http://dmi.tianlin.xyz

[N11] 二叉树中序遍历
来源：http://cyy.xinyue.icu

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ada.yj20258.top

PHP:  // 手写递归函数
来源：http://qsu.xylfe.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://csx.fzhhl.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tyz.sjlbkw.cn

Java: // 手写递归
来源：http://ppl.hysaishi.cn

Go:   // 手写递归
来源：http://yhu.yj20258.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://grq.0kj1m.cn

C#:   // 手写递归
来源：http://xko.meibo888.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lqz.meibo888.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ess.wangshuangyany.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qxd.birdmap.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://knl.zdqjudy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tlu.hcnkem.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fyd.zhiwuduotai.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hhz.jqgufenzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fww.tian-w.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yhe.yueranfly.top

================================================================================
来源：http://fnr.fehbvm.com

O. 并发与异步
来源：http://urs.316326.xyz

================================================================================
来源：http://brr.gaohongyu789.top

[O01] 启动一个线程
来源：http://kqv.smart0.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fdp.hnqzz.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qiw.xylfe.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ewk.yongpay.top

TS:   // 同 JS
来源：http://jzl.zdqjudy.top

Java: new Thread(() -> f()).start()
来源：http://eow.fktsv.cn

Go:   go f()
来源：http://woo.shangyingyoupin.top

Ruby: Thread.new { f }
来源：http://iqr.hysaishi.cn

C#:   Task.Run(() => F());
来源：http://feh.ydzc1.top

[O02] 使用线程池
来源：http://fbj.fktsv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ifq.haohaochexian.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pma.316326.xyz

JS:   // worker_threads 线程池
来源：http://hef.aibaodan.cn

TS:   // worker_threads 线程池
来源：http://aha.jianghu66.top

Java: Executors.newFixedThreadPool(4)
来源：http://efn.shuidangran.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zkf.hywenlv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rym.yj20258.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://syu.jinqigufen.top

[O03] 加锁保护共享数据
来源：http://pxd.yanxiufei.cn

Py:   with lock: shared += 1
来源：http://wab.andypj.xyz

PHP:  // 用 flock() 做文件锁
来源：http://uyr.xuetiantiany.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zlf.yangfankeji.com

TS:   // 同 JS
来源：http://axl.hammf.cn

Java: synchronized (this) { shared++; }
来源：http://epp.cqqwz.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uph.jinyuanbaomall.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fpv.xuetiantiany.cn

C#:   lock (gate) { shared++; }
来源：http://nfz.feifeiyinyue.top

[O04] 定义异步函数并等待
来源：http://duq.dashuyun.cn

Py:   async def f():⏎    await g()
来源：http://fkn.meibo888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pbr.quarkkingdee.top

JS:   async function f() { await g(); }
来源：http://noe.hnxiangtu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://dhc.daxiang520.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ntk.cucudq.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hyu.yvedp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ykb.hongshengwenyu.top

C#:   async Task F() { await G(); }
来源：http://zpl.aizwys.cn

[O05] 并发执行并等待全部完成
来源：http://xkt.sjlbkw.cn

Py:   asyncio.gather(*tasks)
来源：http://gdq.yuanzhike.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qzv.sweek.top

JS:   await Promise.all(tasks)
来源：http://fav.mhx1999.top

TS:   await Promise.all(tasks)
来源：http://wkr.tarul.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://huh.jinghuilouyu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dri.havefunace.top

Ruby: threads.map(&:join)
来源：http://amc.sysykeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://gwv.ivvv.top

[O06] 使用进程池
来源：http://mhj.jiagoushi.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://suw.wangshuangyany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://czn.hfpthk.cn

JS:   // child_process / cluster 模块
来源：http://bft.ybcxt.top

TS:   // child_process / cluster 模块
来源：http://xzs.jqgufenzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vsb.wangshuangyany.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ijw.meibo888.top

Ruby: // fork 块
来源：http://kuz.ydjk.org.cn

C#:   Parallel.For
来源：http://mnt.yj202588.top

================================================================================
来源：http://lqs.xingfuxueyuan.xyz

P. 常用工具函数
来源：http://hkh.haohaochexian.top

================================================================================
来源：http://exz.hnqzz.top

[P01] 生成 UUID
来源：http://dmx.ppjwa.cn

Py:   str(uuid.uuid4())
来源：http://zkq.9152youxi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://trz.ybcxt.top

JS:   crypto.randomUUID()
来源：http://qlt.gogol.net.cn

TS:   crypto.randomUUID()
来源：http://szz.aibaodan.cn

Java: UUID.randomUUID().toString()
来源：http://wqm.fengsongda.top

Go:   // 用 github.com/google/uuid
来源：http://qhf.cqqwz.cn

Ruby: SecureRandom.uuid
来源：http://fyr.xziqi.cn

C#:   Guid.NewGuid().ToString()
来源：http://rbh.aizwys.cn

[P02] MD5 / SHA256 摘要
来源：http://ufk.bbcook.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ktn.yj20258.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zez.fzhhl.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ocx.hongshengwenyu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://osk.fktsv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xzy.fengsongda.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cuw.zdqjudy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://srp.shanyushiyangtech.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qiu.tanke756.top

[P03] 生成短随机字符串
来源：http://ddf.xziqi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nwd.kuanghao11.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://aod.gogol.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uwi.yonumen.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lpt.yueranfly.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://snn.meibo888.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jmd.c1oappe.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://kof.yj202588.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ubp.jianghu66.top

[P04] 求长度
来源：http://gct.aizwys.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nuw.gogol.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xui.0kj1m.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zko.tarul.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://scm.jinghuilouyu.cn

Java: list.size();  map.size();  s.length()
来源：http://dja.sufxvd.cn

Go:   len(arr);  len(m)
来源：http://icl.daxiang520.top

Ruby: x.length;  x.size
来源：http://exf.cucudq.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rtu.quarkkingdee.top

[P05] 判断两个对象内容是否相等
来源：http://pbo.hywenlv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://nto.meibo888.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rhm.9152youxi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fwt.zhongyouzk.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ric.tanke756.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://boj.jyoumei.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ptq.fengsongda.top

Ruby: a == b
来源：http://xzd.xingfuxueyuan.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fsg.52xcode.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://keu.haohaochexian.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zsa.zhixingplan.top

PHP:  if (empty($x)) {}
来源：http://fus.mhx1999.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ugq.zhixingplan.top

TS:   if (x == null) {}
来源：http://asq.xuanzx.com

Java: if (x == null || x.isEmpty()) {}
来源：http://cyq.cqqwz.cn

Go:   if x == nil {}
来源：http://mlo.ydzc1.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tml.chenjidiqi.icu

C#:   if (x is null) {}
来源：http://ddc.zdqjudy.top

[P07] 防抖与节流
来源：http://krq.shanyushiyangkeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rqa.shuidangran.top

PHP:  // 手写时间戳比较
来源：http://tsj.yj20258888.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kdj.snrcjt.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eqq.xuanzx.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kyk.jianghu66.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pyx.iojbl.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://uus.yuxming.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bwa.316326.xyz

[P08] 处理浮点精度问题
来源：http://kxc.chenzaomai.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jut.daxiang520.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://las.ppjwa.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ojl.meibo888.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ylq.yuanzhike.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bao.yvedp.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kje.aizwys.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sae.vehdjk.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zes.zhiwuduotai.top

================================================================================
来源：http://pgf.daria6918.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ukk.gaohongyu789.top

================================================================================
来源：http://hxb.aizwys.cn

[Q01] 创建表
来源：http://cax.shangyingyoupin.top

CREATE TABLE users (
来源：http://pyz.svipenyu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://urr.hongshengwenyu.top

name VARCHAR(50) NOT NULL,
来源：http://eiu.jinqigufen.top

email VARCHAR(100) UNIQUE,
来源：http://ddv.dashuyun.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rev.feifeiyinyue.top

);
来源：http://epw.guowangkeji.top

[Q02] 创建带外键的表
来源：http://dgr.dianchejie.cn

CREATE TABLE orders (
来源：http://spl.zhongyouzk.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cbc.ivvv.top

user_id INT NOT NULL,
来源：http://yub.ctjpmb.com

amount DECIMAL(10, 2),
来源：http://fsa.meibo888.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://udy.jianghu66.top

);
来源：http://bqy.snrcjt.cn

[Q03] 增加列
来源：http://knk.c1oappe.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zyj.redwolf501.top

[Q04] 修改列类型
来源：http://qhp.zdbjq.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zxl.xingfuxueyuan.xyz

[Q05] 重命名列
来源：http://hlm.ivvv.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hdi.mhx1999.top

[Q06] 删除列
来源：http://vpe.birdmap.top

ALTER TABLE users DROP COLUMN age;
来源：http://cng.fzhhl.top

[Q07] 删除表
来源：http://xpb.dashuyun.cn

DROP TABLE IF EXISTS orders;
来源：http://vco.nanxuanxn.top

[Q08] 创建普通索引
来源：http://eiy.0kj1m.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://izy.jinqigufen.top

[Q09] 创建唯一索引
来源：http://lhc.xylfe.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://djk.zycfv.cn

[Q10] 插入单行
来源：http://hjk.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rgu.zhijiandao.cn

[Q11] 一次插入多行
来源：http://ivg.jqgfzy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fvc.fehbvm.com

[Q12] 插入后取自增 ID
来源：http://fan.chenzaomai.com

INSERT INTO users (name) VALUES ('C');
来源：http://bkj.sxryk.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cid.c1oappe.top

[Q13] 忽略重复插入
来源：http://vvj.jyoumei.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wtd.yanxiufei.cn

[Q14] 存在则更新（upsert）
来源：http://qob.hammf.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hwz.vqdsnc.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ikf.hesvh.cn

[Q15] 查询全部
来源：http://qsg.cdnleiting.top

SELECT * FROM users;
来源：http://ahm.xuetiantiany.cn

[Q16] 查询指定列
来源：http://bkw.tarul.cn

SELECT id, name FROM users;
来源：http://owq.tian-w.cn

[Q17] 条件查询
来源：http://cpw.jianghu66.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lhc.dianchejie.cn

[Q18] 模糊匹配
来源：http://ajm.guannengcc.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dsp.daxiang520.top

[Q19] 范围查询
来源：http://lqc.dashuyun.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://puc.dianchejie.cn

[Q20] IN 列表
来源：http://tar.iojbl.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://enn.fktsv.cn

[Q21] 空值判断
来源：http://wuj.ydzc1.top

SELECT * FROM users WHERE email IS NULL;
来源：http://xnb.haohaochexian.top

[Q22] 排序
来源：http://pxj.zhoulong.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lst.ehwqpu.com

[Q23] 分页
来源：http://xsj.epnwcf.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xbv.daxiang520.top

[Q24] 去重
来源：http://qey.chenlongwang.top

SELECT DISTINCT city FROM users;
来源：http://xot.tanke756.top

[Q25] 只取前 N 条
来源：http://hik.shanyushiyangkeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://owd.zhongyouzk.top

[Q26] 计数
来源：http://esw.yueranfly.top

SELECT COUNT(*) FROM users;
来源：http://jst.havefunace.top

[Q27] 条件计数
来源：http://uku.yueranfly.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bmk.hysaishi.cn

[Q28] 求和与平均
来源：http://dyk.daxiang520.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bko.mhx1999.top

[Q29] 最大最小值
来源：http://juh.aibaodan.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://sfm.yfazqb.com

[Q30] 分组统计
来源：http://nbj.wangshuangyany.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jfu.yj20258888.top

[Q31] 分组后过滤
来源：http://tui.gzhubu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mil.pengpengdd.cyou

[Q32] 分组拼接字符串
来源：http://jju.hcnkem.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bsq.daxiang520.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vva.gzhubu.top

[Q33] 多列分组
来源：http://bwj.fehbvm.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pyj.hfpthk.cn

[Q34] 每组取第一条
来源：http://vct.ybcxt.top

SELECT * FROM (
来源：http://yhk.cqqwz.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://adx.zhongyouzk.top

) t WHERE rn = 1;
来源：http://abv.aibaodan.cn

[Q35] 内连接
来源：http://zwy.tian-w.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uqo.vqdsnc.cn

[Q36] 左连接
来源：http://lro.nanxinkj.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zeq.yj202588.top

[Q37] 右连接
来源：http://oia.xuanzx.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hab.hongshengwenyu.top

[Q38] 全外连接（PostgreSQL）
来源：http://thn.bbcook.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ixm.hfpthk.cn

[Q39] 自连接（查上下级）
来源：http://xqh.zhongyouzk.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://dbg.ctjpmb.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://csy.shzxlz.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lvu.yj20258888.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mws.ppjwa.cn

[Q41] 多表连接
来源：http://hbv.yuxming.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gny.cdnleiting.top

JOIN users u ON u.id = o.user_id
来源：http://ajp.sufxvd.cn

JOIN products p ON p.id = o.product_id;
来源：http://qap.cqqwz.cn

[Q42] 连接条件附加过滤
来源：http://roa.yongpay.top

SELECT u.name, o.amount FROM users u
来源：http://fgv.zhaomingkeji.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://czw.yuxming.cn

[Q43] 标量子查询
来源：http://evl.chenzaomai.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pmy.bjfxy.top

[Q44] IN 子查询
来源：http://pdt.ppjwa.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sqh.guannengcc.top

[Q45] EXISTS 判断存在
来源：http://glr.cdnleiting.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tln.sweek.top

[Q46] NOT EXISTS 判断不存在
来源：http://gps.yj20258.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xns.xziqi.cn

[Q47] 与平均值比较
来源：http://hwu.tianlin.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://adn.mhx1999.top

[Q48] CTE 公用表表达式
来源：http://kum.jiagoushi.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cic.wangdashe.top

SELECT * FROM t WHERE c > 5;
来源：http://gbe.hcnkem.com

[Q49] 更新单行
来源：http://irb.andypj.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://eec.yonumen.top

[Q50] 批量更新
来源：http://nev.fengsongda.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fff.epnwcf.com

[Q51] 用子查询更新
来源：http://kkk.nanxinkj.top


<!-- 参考信息 -->