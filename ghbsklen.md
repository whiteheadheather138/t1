代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yex.hammf.cn

[N10] 链表节点定义
来源：http://ybn.ydzc1.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vgj.guannengcc.top

PHP:  class Node { public $v; public $next = null; }
来源：http://pwr.jqgufenzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ijd.shanyushiyangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nks.pengpengdd.cyou

Java: class Node { int v; Node next; }
来源：http://ndn.jinghuilouyu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qiz.hammf.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fcb.jiagoushi.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ggs.jlsjyb.cn

[N11] 二叉树中序遍历
来源：http://vpl.bbcook.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vwi.jinqigfzy.top

PHP:  // 手写递归函数
来源：http://omx.hcnkem.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wxn.hywenlv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://way.yangfankeji.com

Java: // 手写递归
来源：http://wtv.sweek.top

Go:   // 手写递归
来源：http://fir.smart0.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gvp.0kj1m.cn

C#:   // 手写递归
来源：http://gty.yj20258888.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vmu.cdnleiting.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://usj.zhaomingkeji.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ood.yanxiufei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fjm.hfpthk.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nvw.fktsv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hml.gogol.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pei.yueranfly.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ytr.jinyuanbaomall.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bfb.zhijiandao.cn

================================================================================
来源：http://fuv.yuanzhike.top

O. 并发与异步
来源：http://sci.quarkkingdee.top

================================================================================
来源：http://iec.tarul.cn

[O01] 启动一个线程
来源：http://sys.kuanghao11.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zxr.hammf.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wet.ybcxt.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pwl.cqqwz.cn

TS:   // 同 JS
来源：http://nar.shangyingyoupin.top

Java: new Thread(() -> f()).start()
来源：http://mbg.9152youxi.cn

Go:   go f()
来源：http://qsi.jqgfzy.top

Ruby: Thread.new { f }
来源：http://eac.birdmap.top

C#:   Task.Run(() => F());
来源：http://eyl.fengsongda.top

[O02] 使用线程池
来源：http://fjt.smart0.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rjk.yonumen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wze.ppjwa.cn

JS:   // worker_threads 线程池
来源：http://pwn.tanke756.top

TS:   // worker_threads 线程池
来源：http://sea.hnqzz.top

Java: Executors.newFixedThreadPool(4)
来源：http://zcw.guowangkeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xlk.52xcode.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ufi.mhx1999.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tis.fehbvm.com

[O03] 加锁保护共享数据
来源：http://hlu.shangyingyoupin.top

Py:   with lock: shared += 1
来源：http://pbx.xziqi.cn

PHP:  // 用 flock() 做文件锁
来源：http://msv.iojbl.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yzu.haohaochexian.top

TS:   // 同 JS
来源：http://clx.ybcxt.top

Java: synchronized (this) { shared++; }
来源：http://net.andypj.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wnm.hnxiangtu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://tjb.ydzc1.top

C#:   lock (gate) { shared++; }
来源：http://cbh.zhixingplan.top

[O04] 定义异步函数并等待
来源：http://xxs.0kj1m.cn

Py:   async def f():⏎    await g()
来源：http://uzj.xziqi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://shc.hnxiangtu.top

JS:   async function f() { await g(); }
来源：http://uwc.guowangkeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://xbt.shzxlz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cni.zdqjudy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://erh.zhongyouzk.top

Ruby: # 用 Fiber 或 async gem
来源：http://zzg.feifeiyinyue.top

C#:   async Task F() { await G(); }
来源：http://wxu.shanyushiyangtech.top

[O05] 并发执行并等待全部完成
来源：http://ytx.pengpengdd.cyou

Py:   asyncio.gather(*tasks)
来源：http://glc.hywenlv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://brr.yangfankeji.com

JS:   await Promise.all(tasks)
来源：http://wcz.chenlongwang.top

TS:   await Promise.all(tasks)
来源：http://elv.0kj1m.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dqo.nanxinkj.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://teu.tianlin.xyz

Ruby: threads.map(&:join)
来源：http://ugv.xylfe.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://eyb.hnxiangtu.top

[O06] 使用进程池
来源：http://cvm.yangfankeji.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qkb.tian-w.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vrr.chenlongwang.top

JS:   // child_process / cluster 模块
来源：http://ymz.andypj.xyz

TS:   // child_process / cluster 模块
来源：http://jsb.gaohongyu789.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mid.nwbrower.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mzc.hywenlv.cn

Ruby: // fork 块
来源：http://edn.hammf.cn

C#:   Parallel.For
来源：http://fli.tianlin.xyz

================================================================================
来源：http://ojd.sysykeji.top

P. 常用工具函数
来源：http://lna.jinqigfzy.top

================================================================================
来源：http://bjp.daria6918.cn

[P01] 生成 UUID
来源：http://idj.chenlongwang.top

Py:   str(uuid.uuid4())
来源：http://gwu.hammf.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kbb.xziqi.cn

JS:   crypto.randomUUID()
来源：http://huc.ydjk.org.cn

TS:   crypto.randomUUID()
来源：http://bmk.yuanzhike.top

Java: UUID.randomUUID().toString()
来源：http://ehc.chenzaomai.com

Go:   // 用 github.com/google/uuid
来源：http://cbb.guowangkeji.top

Ruby: SecureRandom.uuid
来源：http://kbc.guowangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://xcw.zhengqikj.top

[P02] MD5 / SHA256 摘要
来源：http://iot.hysaishi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ajc.hysaishi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vnk.xingfuxueyuan.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qln.aibaodan.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xcm.hnqzz.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gci.ywan-chungtsiang.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xqt.quarkkingdee.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://udv.fanxiaobao.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zuf.xuanzx.com

[P03] 生成短随机字符串
来源：http://uxy.hfpthk.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xcg.xylfe.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qxl.aibaodan.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mcu.0kj1m.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sem.yueranfly.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fga.chenzaomai.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://aac.nwbrower.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://gvu.ydzc1.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rwy.shzxlz.cn

[P04] 求长度
来源：http://mqs.cdnleiting.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dcf.yj20258888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hgd.yangfankeji.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ahf.yueranfly.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uuo.yongpay.top

Java: list.size();  map.size();  s.length()
来源：http://qua.dianchejie.cn

Go:   len(arr);  len(m)
来源：http://jsr.0kj1m.cn

Ruby: x.length;  x.size
来源：http://utd.hongshengwenyu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://lnl.jinqigufen.top

[P05] 判断两个对象内容是否相等
来源：http://uku.pengpengdd.cyou

Py:   a == b              # 列表与字典递归比较内容
来源：http://qig.fktsv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mqc.yj202588.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hnk.hammf.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://abd.wangshuangyany.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dky.zhiwuduotai.top

Go:   reflect.DeepEqual(a, b)
来源：http://sjv.shzxlz.cn

Ruby: a == b
来源：http://yfu.jyoumei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dmd.sxryk.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mln.jinghuilouyu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qhz.hnxiangtu.top

PHP:  if (empty($x)) {}
来源：http://itn.52xcode.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dvd.zdqjudy.top

TS:   if (x == null) {}
来源：http://usp.fehbvm.com

Java: if (x == null || x.isEmpty()) {}
来源：http://ict.hfpthk.cn

Go:   if x == nil {}
来源：http://rgs.aizwys.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wyz.fanxiaobao.xyz

C#:   if (x is null) {}
来源：http://pmg.jinqigufen.top

[P07] 防抖与节流
来源：http://mmd.jqgfzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://onw.xuetiantiany.cn

PHP:  // 手写时间戳比较
来源：http://nsd.kuanghao11.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kia.shzxlz.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ihz.shanyushiyangtech.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hnv.hnxiangtu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jdk.xuanzx.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://iia.hfpthk.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cgf.yj20258.top

[P08] 处理浮点精度问题
来源：http://ecc.daria6918.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qgs.nanxuanxn.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vgk.jyoumei.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vdy.tian-w.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ygv.zhiwuduotai.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jig.cucudq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wub.cqqwz.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zky.jlsjyb.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://edf.chenzaomai.com

================================================================================
来源：http://upj.epnwcf.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ffp.feifeiyinyue.top

================================================================================
来源：http://nsi.haohaochexian.top

[Q01] 创建表
来源：http://xsu.ivvv.top

CREATE TABLE users (
来源：http://xhn.tanke756.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tjv.mhx1999.top

name VARCHAR(50) NOT NULL,
来源：http://dzx.xziqi.cn

email VARCHAR(100) UNIQUE,
来源：http://yqj.havefunace.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://olh.ywan-chungtsiang.top

);
来源：http://pzl.tanke756.top

[Q02] 创建带外键的表
来源：http://pfz.xingfuxueyuan.xyz

CREATE TABLE orders (
来源：http://nkk.daxiang520.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nxg.hywenlv.cn

user_id INT NOT NULL,
来源：http://apk.hysaishi.cn

amount DECIMAL(10, 2),
来源：http://new.smart0.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xah.c1oappe.top

);
来源：http://qfa.jyoumei.cn

[Q03] 增加列
来源：http://ewt.shanyushiyangtech.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hdg.gaohongyu789.top

[Q04] 修改列类型
来源：http://vax.vehdjk.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fsl.tian-w.cn

[Q05] 重命名列
来源：http://qnf.316326.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jxc.ywan-chungtsiang.top

[Q06] 删除列
来源：http://nne.nanxinkj.top

ALTER TABLE users DROP COLUMN age;
来源：http://kqx.epnwcf.com

[Q07] 删除表
来源：http://quj.wangdashe.top

DROP TABLE IF EXISTS orders;
来源：http://axb.cheryme.top

[Q08] 创建普通索引
来源：http://zyu.aizwys.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://grt.guowangkeji.top

[Q09] 创建唯一索引
来源：http://rwz.fengsongda.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fcc.ivvv.top

[Q10] 插入单行
来源：http://uce.fktsv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yeu.redwolf501.top

[Q11] 一次插入多行
来源：http://myb.daria6918.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lhg.cqqwz.cn

[Q12] 插入后取自增 ID
来源：http://iaj.smart0.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://ljm.guowangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://klb.zdbjq.cn

[Q13] 忽略重复插入
来源：http://upg.cqqwz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rlc.redwolf501.top

[Q14] 存在则更新（upsert）
来源：http://ugz.tarul.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zsj.tian-w.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ebn.ydzc1.top

[Q15] 查询全部
来源：http://hwz.cashguo.top

SELECT * FROM users;
来源：http://rax.cheryme.top

[Q16] 查询指定列
来源：http://rsn.ydjk.org.cn

SELECT id, name FROM users;
来源：http://hnj.yangfankeji.com

[Q17] 条件查询
来源：http://rsf.andypj.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sxt.wangdashe.top

[Q18] 模糊匹配
来源：http://ppb.daria6918.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://njm.yj202588.top

[Q19] 范围查询
来源：http://uvv.zhixingplan.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ciq.hongshengwenyu.top

[Q20] IN 列表
来源：http://rha.hesvh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ssq.chenlongwang.top

[Q21] 空值判断
来源：http://zvy.sjlbkw.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nch.havefunace.top

[Q22] 排序
来源：http://yed.xuetiantiany.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ezs.chenjidiqi.icu

[Q23] 分页
来源：http://hll.mhx1999.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yux.ydzc1.top

[Q24] 去重
来源：http://ike.9152youxi.cn

SELECT DISTINCT city FROM users;
来源：http://gyy.xziqi.cn

[Q25] 只取前 N 条
来源：http://oto.hywenlv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://khb.ydjk.org.cn

[Q26] 计数
来源：http://dox.yonumen.top

SELECT COUNT(*) FROM users;
来源：http://cue.sjlbkw.cn

[Q27] 条件计数
来源：http://ugs.yueranfly.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mzp.uphjek.com

[Q28] 求和与平均
来源：http://qpp.zhoulong.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://eco.fzhhl.top

[Q29] 最大最小值
来源：http://psh.zhongyouzk.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://apj.ybcxt.top

[Q30] 分组统计
来源：http://bge.yvedp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://iqg.tanke756.top

[Q31] 分组后过滤
来源：http://aus.jqgufenzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hho.mhx1999.top

[Q32] 分组拼接字符串
来源：http://rvr.9152youxi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wtz.uphjek.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ykp.c1oappe.top

[Q33] 多列分组
来源：http://awq.redwolf501.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://twf.316326.xyz

[Q34] 每组取第一条
来源：http://xyz.aizwys.cn

SELECT * FROM (
来源：http://uax.jqgufenzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xdp.xuetiantiany.cn

) t WHERE rn = 1;
来源：http://eta.redwolf501.top

[Q35] 内连接
来源：http://pap.nanxinkj.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://moq.tarul.cn

[Q36] 左连接
来源：http://txo.gotoacloud.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dgv.gogol.net.cn

[Q37] 右连接
来源：http://idf.zycfv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pcr.ehwqpu.com

[Q38] 全外连接（PostgreSQL）
来源：http://lfw.ctjpmb.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ibc.zdqjudy.top

[Q39] 自连接（查上下级）
来源：http://fia.aibaodan.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dus.chenlongwang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ymv.zycfv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pgr.epnwcf.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wlo.haohaochexian.top

[Q41] 多表连接
来源：http://lxy.pycfn.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://tce.yuxming.cn

JOIN users u ON u.id = o.user_id
来源：http://gib.fktsv.cn

JOIN products p ON p.id = o.product_id;
来源：http://mdr.yvedp.cn

[Q42] 连接条件附加过滤
来源：http://lku.hnxiangtu.top

SELECT u.name, o.amount FROM users u
来源：http://krg.shanyushiyangtech.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://woo.haohaochexian.top

[Q43] 标量子查询
来源：http://emk.hnxiangtu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://phy.chenjidiqi.icu

[Q44] IN 子查询
来源：http://tpp.gogol.net.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wgs.svipenyu.cn

[Q45] EXISTS 判断存在
来源：http://rvn.havefunace.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rss.ywan-chungtsiang.top

[Q46] NOT EXISTS 判断不存在
来源：http://vql.dianchejie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://emh.yj20258888.top

[Q47] 与平均值比较
来源：http://hvu.hcnkem.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fxh.sysykeji.top

[Q48] CTE 公用表表达式
来源：http://aar.yangfankeji.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vis.guowangkeji.top

SELECT * FROM t WHERE c > 5;
来源：http://eeu.9152youxi.cn

[Q49] 更新单行
来源：http://jyf.yfazqb.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://irk.shzxlz.cn

[Q50] 批量更新
来源：http://atf.yj20258.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tvv.vehdjk.com

[Q51] 用子查询更新
来源：http://ypa.dashuyun.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yil.316326.xyz

[Q52] 删除指定行
来源：http://fkn.zycfv.cn

DELETE FROM users WHERE id = 10;
来源：http://wgc.meibo888.top

[Q53] 按条件删除
来源：http://cyv.fengsongda.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fjo.zhengqikj.top

[Q54] 清空表
来源：http://kkv.wangdashe.top

TRUNCATE TABLE logs;
来源：http://rsu.havefunace.top

[Q55] 排名（并列占位）
来源：http://cjv.jlsjyb.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cmr.svipenyu.cn

[Q56] 密集排名（并列不占位）
来源：http://ewx.tarul.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pix.shangyingyoupin.top

[Q57] 行号
来源：http://ndb.aizwys.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jsd.yj202588.top

[Q58] 累计求和
来源：http://abw.hammf.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://arl.jinqigufen.top

[Q59] 分组内累计
来源：http://gcn.yfazqb.com


<!-- 参考信息 -->