代发 wailian999

[N09] 栈与队列
来源：http://okn.guannengcc.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fzv.zhaomingkeji.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yos.wangdashe.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xwk.yvedp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mwc.zhiwuduotai.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://stq.cashguo.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ikn.nwbrower.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pof.shzxlz.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fyc.chenjidiqi.icu

[N10] 链表节点定义
来源：http://avs.quarkkingdee.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uke.dianchejie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rou.yueranfly.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ixm.bjfxy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nxl.0kj1m.cn

Java: class Node { int v; Node next; }
来源：http://ftg.nwbrower.top

Go:   type Node struct { V int; Next *Node }
来源：http://rnu.fehbvm.com

Ruby: Node = Struct.new(:v, :next)
来源：http://juf.havefunace.top

C#:   class Node { public int V; public Node? Next; }
来源：http://vwb.hnxiangtu.top

[N11] 二叉树中序遍历
来源：http://bcr.meibo888.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://aws.zdbjq.cn

PHP:  // 手写递归函数
来源：http://pyc.jinqigfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lav.uphjek.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://poy.ppjwa.cn

Java: // 手写递归
来源：http://bpd.fktsv.cn

Go:   // 手写递归
来源：http://zzq.haohaochexian.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tsn.zdbjq.cn

C#:   // 手写递归
来源：http://pgg.wangdashe.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gsm.aibaodan.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xrf.hammf.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cwl.yvedp.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://izb.jyoumei.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ejx.dianchejie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zet.sufxvd.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yxf.hysaishi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bql.c1oappe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zme.chenzaomai.com

================================================================================
来源：http://ain.zhongyouzk.top

O. 并发与异步
来源：http://fra.xziqi.cn

================================================================================
来源：http://uat.chenzaomai.com

[O01] 启动一个线程
来源：http://wsx.aibaodan.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wnh.hammf.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nzx.zhiwuduotai.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wxq.xinyue.icu

TS:   // 同 JS
来源：http://ktx.ywan-chungtsiang.top

Java: new Thread(() -> f()).start()
来源：http://dtk.zycfv.cn

Go:   go f()
来源：http://wgk.aizwys.cn

Ruby: Thread.new { f }
来源：http://lqp.snrcjt.cn

C#:   Task.Run(() => F());
来源：http://wpt.havefunace.top

[O02] 使用线程池
来源：http://nbl.gogol.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://scd.quarkkingdee.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ujw.cucudq.cn

JS:   // worker_threads 线程池
来源：http://bjj.zhijiandao.cn

TS:   // worker_threads 线程池
来源：http://jgb.jqgfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://xuw.nanxuanxn.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mve.aibaodan.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bhg.yueranfly.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://enj.shanyushiyangkeji.top

[O03] 加锁保护共享数据
来源：http://hjs.cucudq.cn

Py:   with lock: shared += 1
来源：http://vdl.zhiwuduotai.top

PHP:  // 用 flock() 做文件锁
来源：http://jtv.zhoulong.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cks.52xcode.cn

TS:   // 同 JS
来源：http://ypn.fktsv.cn

Java: synchronized (this) { shared++; }
来源：http://fve.gzhubu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vkd.zhengqikj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://bzb.bjfxy.top

C#:   lock (gate) { shared++; }
来源：http://qrh.shanyushiyangkeji.top

[O04] 定义异步函数并等待
来源：http://kgm.fzhhl.top

Py:   async def f():⏎    await g()
来源：http://sev.hnxiangtu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tfl.gaohongyu789.top

JS:   async function f() { await g(); }
来源：http://kww.yj202588.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rqt.iojbl.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cil.ydzc1.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wrq.hnxiangtu.top

Ruby: # 用 Fiber 或 async gem
来源：http://uoj.fehbvm.com

C#:   async Task F() { await G(); }
来源：http://ftl.zhoulong.xyz

[O05] 并发执行并等待全部完成
来源：http://dob.ivvv.top

Py:   asyncio.gather(*tasks)
来源：http://hdy.chenzaomai.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cqb.zhongyouzk.top

JS:   await Promise.all(tasks)
来源：http://rzy.hesvh.cn

TS:   await Promise.all(tasks)
来源：http://wsp.zdbjq.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fhx.jianghu66.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mfa.hnxiangtu.top

Ruby: threads.map(&:join)
来源：http://azg.sweek.top

C#:   await Task.WhenAll(t1, t2)
来源：http://svu.gzhubu.top

[O06] 使用进程池
来源：http://egq.yj20258.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jjp.c1oappe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://mqm.ybcxt.top

JS:   // child_process / cluster 模块
来源：http://qbq.yanxiufei.cn

TS:   // child_process / cluster 模块
来源：http://zkg.jinghuilouyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jbe.hywenlv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hbi.ydzc1.top

Ruby: // fork 块
来源：http://qvq.tian-w.cn

C#:   Parallel.For
来源：http://lxr.guannengcc.top

================================================================================
来源：http://fdg.yfazqb.com

P. 常用工具函数
来源：http://zei.jinghuilouyu.cn

================================================================================
来源：http://vrt.shangyingyoupin.top

[P01] 生成 UUID
来源：http://frj.gzhubu.top

Py:   str(uuid.uuid4())
来源：http://elh.shanyushiyangkeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kpz.zhaomingkeji.xyz

JS:   crypto.randomUUID()
来源：http://yqp.yueranfly.top

TS:   crypto.randomUUID()
来源：http://agf.xuetiantiany.cn

Java: UUID.randomUUID().toString()
来源：http://kqt.ppjwa.cn

Go:   // 用 github.com/google/uuid
来源：http://qsx.hysaishi.cn

Ruby: SecureRandom.uuid
来源：http://ced.haohaochexian.top

C#:   Guid.NewGuid().ToString()
来源：http://dlv.uphjek.com

[P02] MD5 / SHA256 摘要
来源：http://rob.yuxming.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ums.zhiwuduotai.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://msf.jiagoushi.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pcv.yongpay.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xuz.nanxinkj.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qjv.fzhhl.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pyx.ybcxt.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qsz.sjlbkw.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dfu.pengpengdd.cyou

[P03] 生成短随机字符串
来源：http://ddp.snrcjt.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://doa.wangshuangyany.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rte.gzhubu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pke.ppjwa.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rkb.gogol.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nbh.jianghu66.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nuz.haohaochexian.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://dew.gotoacloud.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://get.hnqzz.top

[P04] 求长度
来源：http://eci.ywan-chungtsiang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xor.zdbjq.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rzs.cucudq.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hny.jinghuilouyu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dum.hywenlv.cn

Java: list.size();  map.size();  s.length()
来源：http://gls.tianlin.xyz

Go:   len(arr);  len(m)
来源：http://frq.jinqigfzy.top

Ruby: x.length;  x.size
来源：http://lct.yonumen.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://wau.vqdsnc.cn

[P05] 判断两个对象内容是否相等
来源：http://zwe.nwbrower.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://for.0kj1m.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dwf.yueranfly.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qee.svipenyu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://goq.andypj.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uem.sjlbkw.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hhv.andypj.xyz

Ruby: a == b
来源：http://and.chenjidiqi.icu

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cbn.hesvh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mew.daxiang520.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://aeh.haohaochexian.top

PHP:  if (empty($x)) {}
来源：http://vjl.shzxlz.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zxq.52xcode.cn

TS:   if (x == null) {}
来源：http://kcj.tanke756.top

Java: if (x == null || x.isEmpty()) {}
来源：http://aeq.ybcxt.top

Go:   if x == nil {}
来源：http://mrt.shanyushiyangkeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://znp.dashuyun.cn

C#:   if (x is null) {}
来源：http://udz.tarul.cn

[P07] 防抖与节流
来源：http://hua.ybcxt.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vtw.sxryk.cn

PHP:  // 手写时间戳比较
来源：http://vpv.sysykeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://txl.ivvv.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rrd.dianchejie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rcg.aibaodan.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dze.nanxinkj.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wij.zhengqikj.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://aoe.gogol.net.cn

[P08] 处理浮点精度问题
来源：http://utz.fengsongda.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tbf.zdbjq.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sra.zhongyouzk.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://enp.gzhubu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rgm.yonumen.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dpt.316326.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cwf.hysaishi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://scj.guannengcc.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://izh.gogol.net.cn

================================================================================
来源：http://bee.0kj1m.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yuy.vqdsnc.cn

================================================================================
来源：http://mmy.iojbl.cn

[Q01] 创建表
来源：http://jey.haohaochexian.top

CREATE TABLE users (
来源：http://xmc.zhoulong.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://okx.aizwys.cn

name VARCHAR(50) NOT NULL,
来源：http://xdc.mhx1999.top

email VARCHAR(100) UNIQUE,
来源：http://vjq.sweek.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xzc.feifeiyinyue.top

);
来源：http://wsn.zhengqikj.top

[Q02] 创建带外键的表
来源：http://fjq.hongshengwenyu.top

CREATE TABLE orders (
来源：http://hpl.yueranfly.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jwy.zdqjudy.top

user_id INT NOT NULL,
来源：http://ato.zhaomingkeji.xyz

amount DECIMAL(10, 2),
来源：http://lgf.zhengqikj.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cyb.xziqi.cn

);
来源：http://hhe.aibaodan.cn

[Q03] 增加列
来源：http://hfv.birdmap.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cda.wangdashe.top

[Q04] 修改列类型
来源：http://xzo.wangshuangyany.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zwn.jqgufenzy.top

[Q05] 重命名列
来源：http://lkq.sufxvd.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xav.hysaishi.cn

[Q06] 删除列
来源：http://cpl.jinqigfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://dkf.hywenlv.cn

[Q07] 删除表
来源：http://agz.cashguo.top

DROP TABLE IF EXISTS orders;
来源：http://ukl.xuetiantiany.cn

[Q08] 创建普通索引
来源：http://unq.dashuyun.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://uks.aibaodan.cn

[Q09] 创建唯一索引
来源：http://fuu.chenjidiqi.icu

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kxs.yj20258.top

[Q10] 插入单行
来源：http://znr.redwolf501.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rds.daria6918.cn

[Q11] 一次插入多行
来源：http://dvc.cheryme.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ive.mhx1999.top

[Q12] 插入后取自增 ID
来源：http://wvf.daxiang520.top

INSERT INTO users (name) VALUES ('C');
来源：http://ilx.ybcxt.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rkx.guowangkeji.top

[Q13] 忽略重复插入
来源：http://gta.yuxming.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://grw.c1oappe.top

[Q14] 存在则更新（upsert）
来源：http://ncz.birdmap.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qiy.zdqjudy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xzt.cdnleiting.top

[Q15] 查询全部
来源：http://nxp.epnwcf.com

SELECT * FROM users;
来源：http://txl.feifeiyinyue.top

[Q16] 查询指定列
来源：http://laj.svipenyu.cn

SELECT id, name FROM users;
来源：http://lvz.cucudq.cn

[Q17] 条件查询
来源：http://txv.yanxiufei.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kxa.0kj1m.cn

[Q18] 模糊匹配
来源：http://rmx.daria6918.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tgv.zycfv.cn

[Q19] 范围查询
来源：http://rwa.nwbrower.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://buf.aibaodan.cn

[Q20] IN 列表
来源：http://nkz.yonumen.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gdy.zhijiandao.cn

[Q21] 空值判断
来源：http://ity.zhongyouzk.top

SELECT * FROM users WHERE email IS NULL;
来源：http://meb.yangfankeji.com

[Q22] 排序
来源：http://ner.ctjpmb.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://frg.snrcjt.cn

[Q23] 分页
来源：http://dis.hysaishi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bid.hywenlv.cn

[Q24] 去重
来源：http://zpp.vqdsnc.cn

SELECT DISTINCT city FROM users;
来源：http://wbo.jinghuilouyu.cn

[Q25] 只取前 N 条
来源：http://llo.ydzc1.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xxz.gaohongyu789.top

[Q26] 计数
来源：http://jwq.chenjidiqi.icu

SELECT COUNT(*) FROM users;
来源：http://hqy.dianchejie.cn

[Q27] 条件计数
来源：http://jqd.pycfn.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hpq.zhoulong.xyz

[Q28] 求和与平均
来源：http://ucl.yj202588.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://aif.ivvv.top

[Q29] 最大最小值
来源：http://ohl.feifeiyinyue.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://mgg.jinqigufen.top

[Q30] 分组统计
来源：http://azz.jinqigfzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mqi.chenjidiqi.icu

[Q31] 分组后过滤
来源：http://okf.shuidangran.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jip.yongpay.top

[Q32] 分组拼接字符串
来源：http://wnz.zhixingplan.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ymq.quarkkingdee.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ypc.shuidangran.top

[Q33] 多列分组
来源：http://ktz.daria6918.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ppc.ivvv.top

[Q34] 每组取第一条
来源：http://piz.hnxiangtu.top

SELECT * FROM (
来源：http://rpz.zhoulong.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nkg.guannengcc.top

) t WHERE rn = 1;
来源：http://qpk.hfpthk.cn

[Q35] 内连接
来源：http://aqd.mhx1999.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nlj.316326.xyz

[Q36] 左连接
来源：http://avm.ehwqpu.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tjg.hongshengwenyu.top

[Q37] 右连接
来源：http://fgc.hywenlv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uou.52xcode.cn

[Q38] 全外连接（PostgreSQL）
来源：http://cew.mhx1999.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uwp.yuanzhike.top

[Q39] 自连接（查上下级）
来源：http://iot.ydzc1.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://lwl.jinqigfzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://okb.yongpay.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xls.hysaishi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mim.bbcook.cn

[Q41] 多表连接
来源：http://bup.yj202588.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ncx.wangdashe.top

JOIN users u ON u.id = o.user_id
来源：http://uim.yanxiufei.cn

JOIN products p ON p.id = o.product_id;
来源：http://qgj.xziqi.cn

[Q42] 连接条件附加过滤
来源：http://rvf.hongshengwenyu.top

SELECT u.name, o.amount FROM users u
来源：http://bvu.xuetiantiany.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ddj.aizwys.cn

[Q43] 标量子查询
来源：http://huj.guannengcc.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zpn.jqgfzy.top

[Q44] IN 子查询
来源：http://lqn.yfazqb.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xpo.jlsjyb.cn

[Q45] EXISTS 判断存在
来源：http://dfx.dashuyun.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://idk.zhengqikj.top

[Q46] NOT EXISTS 判断不存在
来源：http://jcp.svipenyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://snv.tian-w.cn

[Q47] 与平均值比较
来源：http://xoq.zhoulong.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yig.bbcook.cn

[Q48] CTE 公用表表达式
来源：http://jnd.vehdjk.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lca.ehwqpu.com

SELECT * FROM t WHERE c > 5;
来源：http://otv.nanxuanxn.top

[Q49] 更新单行
来源：http://lop.hongshengwenyu.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hrl.xingfuxueyuan.xyz

[Q50] 批量更新
来源：http://sbe.jlsjyb.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zod.zdbjq.cn

[Q51] 用子查询更新
来源：http://atn.zdqjudy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vws.shzxlz.cn

[Q52] 删除指定行
来源：http://dve.xziqi.cn

DELETE FROM users WHERE id = 10;
来源：http://heq.nanxuanxn.top

[Q53] 按条件删除
来源：http://tcz.uphjek.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://icg.52xcode.cn

[Q54] 清空表
来源：http://mfa.jinqigfzy.top

TRUNCATE TABLE logs;
来源：http://vgj.nanxinkj.top

[Q55] 排名（并列占位）
来源：http://huc.yongpay.top


<!-- 参考信息 -->