代发 wailian999

Java: // 手写回溯递归
来源：http://ays.jiagoushi.top

Go:   // 手写回溯递归
来源：http://fnh.ydzc1.top

Ruby: arr.permutation.to_a
来源：http://ilr.ydjk.org.cn

C#:   // 手写回溯递归
来源：http://ywn.redwolf501.top

[N09] 栈与队列
来源：http://guu.cashguo.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qkj.epnwcf.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fxk.dashuyun.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dnq.dianchejie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ugt.hammf.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://liw.haohaochexian.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yfg.yanxiufei.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://aas.ydzc1.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xdx.hongshengwenyu.top

[N10] 链表节点定义
来源：http://ias.zhaomingkeji.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uwg.kuanghao11.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mvv.gzhubu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fia.ydjk.org.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fhe.jyoumei.cn

Java: class Node { int v; Node next; }
来源：http://yod.hesvh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ezu.gzhubu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://sqw.jinyuanbaomall.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ors.dashuyun.cn

[N11] 二叉树中序遍历
来源：http://iyg.hfpthk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xjt.gotoacloud.top

PHP:  // 手写递归函数
来源：http://cut.havefunace.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mpt.fengsongda.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nqr.daria6918.cn

Java: // 手写递归
来源：http://mfg.jiagoushi.top

Go:   // 手写递归
来源：http://ans.tanke756.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fuy.jinyuanbaomall.cn

C#:   // 手写递归
来源：http://ppq.gaohongyu789.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jmc.yuanzhike.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ldz.cheryme.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mbn.guowangkeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jmd.hongshengwenyu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ufg.xuetiantiany.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pxo.vehdjk.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://upx.shuidangran.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ent.tarul.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://aum.cdnleiting.top

================================================================================
来源：http://vpf.haohaochexian.top

O. 并发与异步
来源：http://jnk.sysykeji.top

================================================================================
来源：http://dmg.quarkkingdee.top

[O01] 启动一个线程
来源：http://eqa.zycfv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kqh.chenzaomai.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ikz.sweek.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kod.hywenlv.cn

TS:   // 同 JS
来源：http://oqm.havefunace.top

Java: new Thread(() -> f()).start()
来源：http://szc.hywenlv.cn

Go:   go f()
来源：http://ldm.gzhubu.top

Ruby: Thread.new { f }
来源：http://ktj.ctjpmb.com

C#:   Task.Run(() => F());
来源：http://jao.jinqigfzy.top

[O02] 使用线程池
来源：http://abi.fengsongda.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bqm.gogol.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mxr.xuetiantiany.cn

JS:   // worker_threads 线程池
来源：http://vlh.gotoacloud.top

TS:   // worker_threads 线程池
来源：http://ffq.ctjpmb.com

Java: Executors.newFixedThreadPool(4)
来源：http://rov.sjlbkw.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hmf.jinyuanbaomall.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://avz.dashuyun.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ijp.vehdjk.com

[O03] 加锁保护共享数据
来源：http://vbn.hongshengwenyu.top

Py:   with lock: shared += 1
来源：http://jyb.smart0.xyz

PHP:  // 用 flock() 做文件锁
来源：http://wue.cheryme.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gsi.redwolf501.top

TS:   // 同 JS
来源：http://sdu.hywenlv.cn

Java: synchronized (this) { shared++; }
来源：http://zsb.feifeiyinyue.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mep.hfpthk.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://njl.xingfuxueyuan.xyz

C#:   lock (gate) { shared++; }
来源：http://njy.svipenyu.cn

[O04] 定义异步函数并等待
来源：http://xyu.dashuyun.cn

Py:   async def f():⏎    await g()
来源：http://cdy.cheryme.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jqb.jinqigufen.top

JS:   async function f() { await g(); }
来源：http://ase.daxiang520.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://lfi.aizwys.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jpk.jinqigfzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eda.yuxming.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ugu.316326.xyz

C#:   async Task F() { await G(); }
来源：http://idy.aizwys.cn

[O05] 并发执行并等待全部完成
来源：http://yaz.hongshengwenyu.top

Py:   asyncio.gather(*tasks)
来源：http://fol.snrcjt.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ycj.hammf.cn

JS:   await Promise.all(tasks)
来源：http://vgv.yueranfly.top

TS:   await Promise.all(tasks)
来源：http://kfo.mhx1999.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mrz.cucudq.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rxm.tianlin.xyz

Ruby: threads.map(&:join)
来源：http://uza.hywenlv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ipo.hcnkem.com

[O06] 使用进程池
来源：http://uyg.ydzc1.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://agn.xziqi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gou.jianghu66.top

JS:   // child_process / cluster 模块
来源：http://jhw.feifeiyinyue.top

TS:   // child_process / cluster 模块
来源：http://kcr.jiagoushi.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tzy.yuxming.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tnj.vehdjk.com

Ruby: // fork 块
来源：http://tnt.snrcjt.cn

C#:   Parallel.For
来源：http://yjn.snrcjt.cn

================================================================================
来源：http://jpu.hnxiangtu.top

P. 常用工具函数
来源：http://ioq.xylfe.cn

================================================================================
来源：http://mem.zhijiandao.cn

[P01] 生成 UUID
来源：http://rhu.yuanzhike.top

Py:   str(uuid.uuid4())
来源：http://ddl.nanxuanxn.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oqm.xziqi.cn

JS:   crypto.randomUUID()
来源：http://nge.ctjpmb.com

TS:   crypto.randomUUID()
来源：http://ghz.52xcode.cn

Java: UUID.randomUUID().toString()
来源：http://ciw.gogol.net.cn

Go:   // 用 github.com/google/uuid
来源：http://iur.pengpengdd.cyou

Ruby: SecureRandom.uuid
来源：http://fil.hnqzz.top

C#:   Guid.NewGuid().ToString()
来源：http://efk.hnqzz.top

[P02] MD5 / SHA256 摘要
来源：http://cvm.tarul.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://puj.gotoacloud.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wdh.ybcxt.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tgo.yanxiufei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xgz.andypj.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hsp.nanxuanxn.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vmz.zdbjq.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ntl.yuxming.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nve.dianchejie.cn

[P03] 生成短随机字符串
来源：http://iji.shanyushiyangkeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ren.tarul.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kte.yongpay.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ati.tanke756.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vve.shuidangran.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://oes.yj20258.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qqd.0kj1m.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://sfv.jqgfzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gnr.wangshuangyany.cn

[P04] 求长度
来源：http://hhh.yfazqb.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vkc.sxryk.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aue.xylfe.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bwd.daxiang520.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kch.zdbjq.cn

Java: list.size();  map.size();  s.length()
来源：http://mkl.tanke756.top

Go:   len(arr);  len(m)
来源：http://ehh.cdnleiting.top

Ruby: x.length;  x.size
来源：http://xsq.ctjpmb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://gds.yj202588.top

[P05] 判断两个对象内容是否相等
来源：http://mst.tanke756.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://yvz.hesvh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vab.cqqwz.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://okk.vehdjk.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rpz.316326.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://osb.hcnkem.com

Go:   reflect.DeepEqual(a, b)
来源：http://djp.dashuyun.cn

Ruby: a == b
来源：http://vxk.yvedp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kig.xuetiantiany.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://svh.0kj1m.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lkj.xinyue.icu

PHP:  if (empty($x)) {}
来源：http://gvr.aizwys.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mxu.shanyushiyangtech.top

TS:   if (x == null) {}
来源：http://jyb.fehbvm.com

Java: if (x == null || x.isEmpty()) {}
来源：http://ptg.jlsjyb.cn

Go:   if x == nil {}
来源：http://rkd.andypj.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zvx.c1oappe.top

C#:   if (x is null) {}
来源：http://wwl.ehwqpu.com

[P07] 防抖与节流
来源：http://qjf.zdqjudy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ueh.nanxinkj.top

PHP:  // 手写时间戳比较
来源：http://xkw.pengpengdd.cyou

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ezy.tianlin.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vkz.birdmap.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://opc.52xcode.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mmn.hysaishi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://uiu.xylfe.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tpd.chenlongwang.top

[P08] 处理浮点精度问题
来源：http://ufw.aibaodan.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sik.zhaomingkeji.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://did.andypj.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://aqd.jiagoushi.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cgb.zhiwuduotai.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mbs.tian-w.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ogr.gaohongyu789.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wuq.svipenyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bsq.yj20258.top

================================================================================
来源：http://kgd.yvedp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mss.zhongyouzk.top

================================================================================
来源：http://qyr.ivvv.top

[Q01] 创建表
来源：http://efb.cucudq.cn

CREATE TABLE users (
来源：http://hkh.hnqzz.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nwm.ydzc1.top

name VARCHAR(50) NOT NULL,
来源：http://wwb.iojbl.cn

email VARCHAR(100) UNIQUE,
来源：http://grz.pengpengdd.cyou

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ilo.gaohongyu789.top

);
来源：http://cwz.hesvh.cn

[Q02] 创建带外键的表
来源：http://hnf.pengpengdd.cyou

CREATE TABLE orders (
来源：http://lke.chenzaomai.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vyr.redwolf501.top

user_id INT NOT NULL,
来源：http://krb.jqgufenzy.top

amount DECIMAL(10, 2),
来源：http://wiq.haohaochexian.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qhk.9152youxi.cn

);
来源：http://llx.zhongyouzk.top

[Q03] 增加列
来源：http://zta.jinqigufen.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vsf.jinqigufen.top

[Q04] 修改列类型
来源：http://fwv.snrcjt.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rsn.zdqjudy.top

[Q05] 重命名列
来源：http://xap.svipenyu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gsf.shuidangran.top

[Q06] 删除列
来源：http://myr.smart0.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://djp.ppjwa.cn

[Q07] 删除表
来源：http://vsw.nanxinkj.top

DROP TABLE IF EXISTS orders;
来源：http://rhm.zhijiandao.cn

[Q08] 创建普通索引
来源：http://owp.aizwys.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bbo.chenlongwang.top

[Q09] 创建唯一索引
来源：http://bmi.ydzc1.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tnw.zdbjq.cn

[Q10] 插入单行
来源：http://ebn.mhx1999.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zho.gogol.net.cn

[Q11] 一次插入多行
来源：http://loz.jyoumei.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sux.ppjwa.cn

[Q12] 插入后取自增 ID
来源：http://ybc.zhoulong.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://rry.fengsongda.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://aqd.sweek.top

[Q13] 忽略重复插入
来源：http://wus.birdmap.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xfg.yuxming.cn

[Q14] 存在则更新（upsert）
来源：http://dij.nanxinkj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ird.sjlbkw.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://icq.hongshengwenyu.top

[Q15] 查询全部
来源：http://zin.aibaodan.cn

SELECT * FROM users;
来源：http://wzd.vehdjk.com

[Q16] 查询指定列
来源：http://gpa.daxiang520.top

SELECT id, name FROM users;
来源：http://ggh.bjfxy.top

[Q17] 条件查询
来源：http://eyn.xinyue.icu

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://shf.gotoacloud.top

[Q18] 模糊匹配
来源：http://jbj.yvedp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jgp.sxryk.cn

[Q19] 范围查询
来源：http://afq.jinqigfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zsf.yj20258.top

[Q20] IN 列表
来源：http://sls.jinqigfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mkb.yongpay.top

[Q21] 空值判断
来源：http://zdk.jqgufenzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ore.nanxuanxn.top

[Q22] 排序
来源：http://haq.jyoumei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zmv.uphjek.com

[Q23] 分页
来源：http://qul.hnqzz.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://klb.aizwys.cn

[Q24] 去重
来源：http://wfn.gogol.net.cn

SELECT DISTINCT city FROM users;
来源：http://ghq.zdqjudy.top

[Q25] 只取前 N 条
来源：http://gdi.cdnleiting.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xhu.chenjidiqi.icu

[Q26] 计数
来源：http://cnr.shuidangran.top

SELECT COUNT(*) FROM users;
来源：http://ztl.ydzc1.top

[Q27] 条件计数
来源：http://hcx.yueranfly.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ylf.shanyushiyangkeji.top

[Q28] 求和与平均
来源：http://zmc.fzhhl.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://piy.fktsv.cn

[Q29] 最大最小值
来源：http://qyk.gogol.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://nwt.xziqi.cn

[Q30] 分组统计
来源：http://lbl.shzxlz.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wes.mhx1999.top

[Q31] 分组后过滤
来源：http://kiz.hysaishi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://eng.sweek.top

[Q32] 分组拼接字符串
来源：http://kxv.cucudq.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://azn.tanke756.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pmj.nanxinkj.top

[Q33] 多列分组
来源：http://kgk.uphjek.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dcy.kuanghao11.cn

[Q34] 每组取第一条
来源：http://hnf.hnqzz.top

SELECT * FROM (
来源：http://xwr.hesvh.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xif.vqdsnc.cn

) t WHERE rn = 1;
来源：http://wrk.jinqigufen.top

[Q35] 内连接
来源：http://msi.yuxming.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tgy.daria6918.cn

[Q36] 左连接
来源：http://boy.zhiwuduotai.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cta.ppjwa.cn

[Q37] 右连接
来源：http://dfs.316326.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ujm.hysaishi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bel.wangshuangyany.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ueb.0kj1m.cn

[Q39] 自连接（查上下级）
来源：http://dvx.xylfe.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nov.daxiang520.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zry.jinqigufen.top

[Q40] 交叉连接（笛卡尔积）
来源：http://yhe.bbcook.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://die.sxryk.cn

[Q41] 多表连接
来源：http://quz.9152youxi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://hnj.meibo888.top

JOIN users u ON u.id = o.user_id
来源：http://syz.shuidangran.top

JOIN products p ON p.id = o.product_id;
来源：http://azo.zhiwuduotai.top

[Q42] 连接条件附加过滤
来源：http://uqz.tanke756.top

SELECT u.name, o.amount FROM users u
来源：http://qwa.0kj1m.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pnh.quarkkingdee.top

[Q43] 标量子查询
来源：http://umv.guannengcc.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zok.yj20258888.top

[Q44] IN 子查询
来源：http://eqr.wangshuangyany.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sya.yonumen.top

[Q45] EXISTS 判断存在
来源：http://mqe.ehwqpu.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://swm.gotoacloud.top

[Q46] NOT EXISTS 判断不存在
来源：http://kmc.ehwqpu.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://smt.tanke756.top

[Q47] 与平均值比较
来源：http://uui.jqgfzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nzm.shangyingyoupin.top

[Q48] CTE 公用表表达式
来源：http://cuy.ppjwa.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dkm.redwolf501.top

SELECT * FROM t WHERE c > 5;
来源：http://gab.zdbjq.cn

[Q49] 更新单行
来源：http://azh.jinqigufen.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ujx.yj20258888.top

[Q50] 批量更新
来源：http://aif.cdnleiting.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wix.ydjk.org.cn

[Q51] 用子查询更新
来源：http://zbo.gotoacloud.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sxv.yfazqb.com

[Q52] 删除指定行
来源：http://jcb.jiagoushi.top

DELETE FROM users WHERE id = 10;
来源：http://vve.iojbl.cn

[Q53] 按条件删除
来源：http://wlf.tanke756.top


<!-- 参考信息 -->