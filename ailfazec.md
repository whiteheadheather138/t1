代发 wailian999

[N09] 栈与队列
来源：http://ugg.smart0.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yio.daria6918.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mll.zdqjudy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://aib.fktsv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ufo.hammf.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hij.xziqi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ylv.quarkkingdee.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wfl.jinqigfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nrv.zhoulong.xyz

[N10] 链表节点定义
来源：http://kat.yvedp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ftw.bbcook.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mqk.yj20258888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://heu.sjlbkw.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hon.c1oappe.top

Java: class Node { int v; Node next; }
来源：http://wvt.cucudq.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rzn.zdbjq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zpw.yonumen.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bad.yj202588.top

[N11] 二叉树中序遍历
来源：http://nzu.guannengcc.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://imr.ctjpmb.com

PHP:  // 手写递归函数
来源：http://djm.yueranfly.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tlh.zhongyouzk.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mgx.pycfn.com

Java: // 手写递归
来源：http://skh.zhoulong.xyz

Go:   // 手写递归
来源：http://uim.zhongyouzk.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ycl.ppjwa.cn

C#:   // 手写递归
来源：http://aoz.ywan-chungtsiang.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xur.aibaodan.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fvc.xuanzx.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yiq.shanyushiyangtech.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://urk.jianghu66.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qqr.jyoumei.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kya.yanxiufei.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tei.meibo888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cjf.zdbjq.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hmv.jinghuilouyu.cn

================================================================================
来源：http://zae.pycfn.com

O. 并发与异步
来源：http://ifu.0kj1m.cn

================================================================================
来源：http://itk.zdqjudy.top

[O01] 启动一个线程
来源：http://tzi.dashuyun.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lzu.xingfuxueyuan.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pxn.shanyushiyangkeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://eem.ydzc1.top

TS:   // 同 JS
来源：http://dgt.wangdashe.top

Java: new Thread(() -> f()).start()
来源：http://sbd.ivvv.top

Go:   go f()
来源：http://zjb.aibaodan.cn

Ruby: Thread.new { f }
来源：http://pkd.svipenyu.cn

C#:   Task.Run(() => F());
来源：http://cjb.havefunace.top

[O02] 使用线程池
来源：http://wcc.zhengqikj.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ytp.jqgufenzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xwq.quarkkingdee.top

JS:   // worker_threads 线程池
来源：http://gvx.hnqzz.top

TS:   // worker_threads 线程池
来源：http://edk.yvedp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yzm.vehdjk.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ztg.xziqi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uly.vehdjk.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rfx.ydjk.org.cn

[O03] 加锁保护共享数据
来源：http://qgm.zhengqikj.top

Py:   with lock: shared += 1
来源：http://kgf.fzhhl.top

PHP:  // 用 flock() 做文件锁
来源：http://slf.jinqigfzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rbx.yongpay.top

TS:   // 同 JS
来源：http://atx.yueranfly.top

Java: synchronized (this) { shared++; }
来源：http://xmf.feifeiyinyue.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tqw.chenlongwang.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://pks.shangyingyoupin.top

C#:   lock (gate) { shared++; }
来源：http://yxq.yj20258888.top

[O04] 定义异步函数并等待
来源：http://nah.meibo888.top

Py:   async def f():⏎    await g()
来源：http://dmk.cdnleiting.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wat.feifeiyinyue.top

JS:   async function f() { await g(); }
来源：http://vhh.sysykeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ied.zhongyouzk.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gts.tian-w.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gsf.fktsv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jbx.yj202588.top

C#:   async Task F() { await G(); }
来源：http://fzt.tarul.cn

[O05] 并发执行并等待全部完成
来源：http://oyj.fktsv.cn

Py:   asyncio.gather(*tasks)
来源：http://hok.zhiwuduotai.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mpt.daria6918.cn

JS:   await Promise.all(tasks)
来源：http://scl.jinyuanbaomall.cn

TS:   await Promise.all(tasks)
来源：http://icl.gogol.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tbq.chenzaomai.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qwf.tanke756.top

Ruby: threads.map(&:join)
来源：http://dxm.quarkkingdee.top

C#:   await Task.WhenAll(t1, t2)
来源：http://lfk.hongshengwenyu.top

[O06] 使用进程池
来源：http://fhs.cqqwz.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xzc.tanke756.top

PHP:  // pcntl_fork 或多进程队列
来源：http://uin.gotoacloud.top

JS:   // child_process / cluster 模块
来源：http://lzk.cheryme.top

TS:   // child_process / cluster 模块
来源：http://dsw.hfpthk.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wjs.xinyue.icu

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ntt.cheryme.top

Ruby: // fork 块
来源：http://lwp.xziqi.cn

C#:   Parallel.For
来源：http://uce.birdmap.top

================================================================================
来源：http://ihg.bbcook.cn

P. 常用工具函数
来源：http://hqs.dashuyun.cn

================================================================================
来源：http://fvd.xylfe.cn

[P01] 生成 UUID
来源：http://aul.vqdsnc.cn

Py:   str(uuid.uuid4())
来源：http://tdr.shangyingyoupin.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://idl.epnwcf.com

JS:   crypto.randomUUID()
来源：http://qjn.zdbjq.cn

TS:   crypto.randomUUID()
来源：http://dwa.yanxiufei.cn

Java: UUID.randomUUID().toString()
来源：http://nme.hnxiangtu.top

Go:   // 用 github.com/google/uuid
来源：http://owb.fzhhl.top

Ruby: SecureRandom.uuid
来源：http://dfy.ivvv.top

C#:   Guid.NewGuid().ToString()
来源：http://haj.xinyue.icu

[P02] MD5 / SHA256 摘要
来源：http://bjs.hywenlv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://npt.fanxiaobao.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://nhl.cdnleiting.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qik.havefunace.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://frf.zhiwuduotai.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lyb.chenzaomai.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pft.nwbrower.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qxi.yfazqb.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nfy.hysaishi.cn

[P03] 生成短随机字符串
来源：http://xms.shuidangran.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lox.jqgfzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sul.chenzaomai.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gpa.9152youxi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kzw.svipenyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ypa.vqdsnc.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://emp.chenlongwang.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://vsr.pycfn.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qwm.c1oappe.top

[P04] 求长度
来源：http://xsh.havefunace.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jml.sufxvd.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nyy.zhixingplan.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tdt.xziqi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nak.yonumen.top

Java: list.size();  map.size();  s.length()
来源：http://aec.sjlbkw.cn

Go:   len(arr);  len(m)
来源：http://tux.jqgfzy.top

Ruby: x.length;  x.size
来源：http://ljw.smart0.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://fpw.jinghuilouyu.cn

[P05] 判断两个对象内容是否相等
来源：http://owv.xinyue.icu

Py:   a == b              # 列表与字典递归比较内容
来源：http://rra.xinyue.icu

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qvc.hammf.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yke.fehbvm.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://iwj.havefunace.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cyl.aibaodan.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tin.nanxuanxn.top

Ruby: a == b
来源：http://rsf.ehwqpu.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zhd.c1oappe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jjh.vehdjk.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zwu.bjfxy.top

PHP:  if (empty($x)) {}
来源：http://awx.guannengcc.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pum.shanyushiyangtech.top

TS:   if (x == null) {}
来源：http://fdo.chenzaomai.com

Java: if (x == null || x.isEmpty()) {}
来源：http://qcr.9152youxi.cn

Go:   if x == nil {}
来源：http://koj.chenlongwang.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ern.zdqjudy.top

C#:   if (x is null) {}
来源：http://lrt.jinghuilouyu.cn

[P07] 防抖与节流
来源：http://vho.jianghu66.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dlc.jlsjyb.cn

PHP:  // 手写时间戳比较
来源：http://nmz.c1oappe.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://itc.cqqwz.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zqn.shanyushiyangkeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wix.quarkkingdee.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://set.guannengcc.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://yey.jianghu66.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lcp.tarul.cn

[P08] 处理浮点精度问题
来源：http://zcn.zhiwuduotai.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pea.tarul.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ucb.xziqi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mjw.dianchejie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cdy.zhaomingkeji.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yeh.zhiwuduotai.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nyd.tarul.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mdr.sufxvd.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fgt.xuetiantiany.cn

================================================================================
来源：http://rcp.birdmap.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rva.pengpengdd.cyou

================================================================================
来源：http://cxv.haohaochexian.top

[Q01] 创建表
来源：http://rjg.hesvh.cn

CREATE TABLE users (
来源：http://jul.xingfuxueyuan.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ect.sysykeji.top

name VARCHAR(50) NOT NULL,
来源：http://rop.mhx1999.top

email VARCHAR(100) UNIQUE,
来源：http://qvb.fzhhl.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bgh.pengpengdd.cyou

);
来源：http://rxf.daria6918.cn

[Q02] 创建带外键的表
来源：http://nud.smart0.xyz

CREATE TABLE orders (
来源：http://waz.yonumen.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lfa.epnwcf.com

user_id INT NOT NULL,
来源：http://hdj.yuxming.cn

amount DECIMAL(10, 2),
来源：http://mdz.hesvh.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hzf.fehbvm.com

);
来源：http://jmx.jqgfzy.top

[Q03] 增加列
来源：http://lgz.zhaomingkeji.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://shk.gaohongyu789.top

[Q04] 修改列类型
来源：http://qze.dianchejie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wpr.zhengqikj.top

[Q05] 重命名列
来源：http://qrq.dianchejie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uho.daria6918.cn

[Q06] 删除列
来源：http://epn.jyoumei.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bno.iojbl.cn

[Q07] 删除表
来源：http://nyj.hcnkem.com

DROP TABLE IF EXISTS orders;
来源：http://stm.52xcode.cn

[Q08] 创建普通索引
来源：http://eow.iojbl.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ack.fanxiaobao.xyz

[Q09] 创建唯一索引
来源：http://wvo.fengsongda.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sgi.ppjwa.cn

[Q10] 插入单行
来源：http://syx.mhx1999.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://quu.smart0.xyz

[Q11] 一次插入多行
来源：http://pxm.zhongyouzk.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kgz.zhongyouzk.top

[Q12] 插入后取自增 ID
来源：http://fhr.bjfxy.top

INSERT INTO users (name) VALUES ('C');
来源：http://njv.cdnleiting.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jkx.fanxiaobao.xyz

[Q13] 忽略重复插入
来源：http://dpu.fktsv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sad.hnxiangtu.top

[Q14] 存在则更新（upsert）
来源：http://bsw.cheryme.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rhw.ywan-chungtsiang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://umz.sjlbkw.cn

[Q15] 查询全部
来源：http://jud.yongpay.top

SELECT * FROM users;
来源：http://reb.sufxvd.cn

[Q16] 查询指定列
来源：http://two.yanxiufei.cn

SELECT id, name FROM users;
来源：http://mbk.shanyushiyangtech.top

[Q17] 条件查询
来源：http://fgf.jinyuanbaomall.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ptn.zhongyouzk.top

[Q18] 模糊匹配
来源：http://jdt.hongshengwenyu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hee.jinqigufen.top

[Q19] 范围查询
来源：http://wkv.wangdashe.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://knl.zdqjudy.top

[Q20] IN 列表
来源：http://fob.uphjek.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zfg.cucudq.cn

[Q21] 空值判断
来源：http://lha.cashguo.top

SELECT * FROM users WHERE email IS NULL;
来源：http://dut.zhiwuduotai.top

[Q22] 排序
来源：http://aah.tian-w.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ktp.sweek.top

[Q23] 分页
来源：http://lqg.tianlin.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gxs.zhixingplan.top

[Q24] 去重
来源：http://kie.pycfn.com

SELECT DISTINCT city FROM users;
来源：http://kgf.epnwcf.com

[Q25] 只取前 N 条
来源：http://grp.ywan-chungtsiang.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pjw.xuanzx.com

[Q26] 计数
来源：http://gag.wangdashe.top

SELECT COUNT(*) FROM users;
来源：http://hru.sysykeji.top

[Q27] 条件计数
来源：http://zpj.chenjidiqi.icu

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://non.havefunace.top

[Q28] 求和与平均
来源：http://sfw.pengpengdd.cyou

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ctq.fengsongda.top

[Q29] 最大最小值
来源：http://mis.aizwys.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://poz.yongpay.top

[Q30] 分组统计
来源：http://rph.shanyushiyangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wae.xuanzx.com

[Q31] 分组后过滤
来源：http://nch.tanke756.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hze.c1oappe.top

[Q32] 分组拼接字符串
来源：http://yqd.redwolf501.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jdp.bbcook.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jxs.shzxlz.cn

[Q33] 多列分组
来源：http://pxo.yvedp.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qop.jinyuanbaomall.cn

[Q34] 每组取第一条
来源：http://vjb.birdmap.top

SELECT * FROM (
来源：http://ssf.aibaodan.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qwe.ydjk.org.cn

) t WHERE rn = 1;
来源：http://mie.shanyushiyangkeji.top

[Q35] 内连接
来源：http://vfd.hfpthk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://plz.birdmap.top

[Q36] 左连接
来源：http://syb.dashuyun.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://eaw.epnwcf.com

[Q37] 右连接
来源：http://lot.wangshuangyany.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nbh.yvedp.cn

[Q38] 全外连接（PostgreSQL）
来源：http://inn.shuidangran.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jnl.cucudq.cn

[Q39] 自连接（查上下级）
来源：http://sgo.zdbjq.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://rck.cucudq.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wtm.xziqi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://avn.meibo888.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://okw.hongshengwenyu.top

[Q41] 多表连接
来源：http://mqf.chenzaomai.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://iof.chenjidiqi.icu

JOIN users u ON u.id = o.user_id
来源：http://ohl.zhongyouzk.top

JOIN products p ON p.id = o.product_id;
来源：http://vze.yvedp.cn

[Q42] 连接条件附加过滤
来源：http://tfi.aibaodan.cn

SELECT u.name, o.amount FROM users u
来源：http://dfd.chenlongwang.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vdh.birdmap.top

[Q43] 标量子查询
来源：http://jln.zhijiandao.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ajh.daria6918.cn

[Q44] IN 子查询
来源：http://xmz.yvedp.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://evf.yj20258.top

[Q45] EXISTS 判断存在
来源：http://fsk.tianlin.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rms.yangfankeji.com

[Q46] NOT EXISTS 判断不存在
来源：http://swq.zhijiandao.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dsl.andypj.xyz

[Q47] 与平均值比较
来源：http://vsm.ctjpmb.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dum.yongpay.top

[Q48] CTE 公用表表达式
来源：http://mpq.yangfankeji.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dcm.shuidangran.top

SELECT * FROM t WHERE c > 5;
来源：http://btu.zhengqikj.top

[Q49] 更新单行
来源：http://tqo.xuetiantiany.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kpo.jianghu66.top

[Q50] 批量更新
来源：http://ttb.sxryk.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vfq.meibo888.top

[Q51] 用子查询更新
来源：http://fsf.gaohongyu789.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://coa.chenlongwang.top

[Q52] 删除指定行
来源：http://rfs.cheryme.top

DELETE FROM users WHERE id = 10;
来源：http://btf.yj20258.top

[Q53] 按条件删除
来源：http://lhi.sysykeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zbv.cdnleiting.top

[Q54] 清空表
来源：http://cug.ctjpmb.com

TRUNCATE TABLE logs;
来源：http://kgo.dashuyun.cn

[Q55] 排名（并列占位）
来源：http://dxq.hnqzz.top


<!-- 参考信息 -->