代发 wailian999

Java: // 手写回溯递归
来源：http://kzf.dianchejie.cn

Go:   // 手写回溯递归
来源：http://rbm.hfpthk.cn

Ruby: arr.permutation.to_a
来源：http://hoh.chenzaomai.com

C#:   // 手写回溯递归
来源：http://amx.zhijiandao.cn

[N09] 栈与队列
来源：http://czc.shanyushiyangtech.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://eed.smart0.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://htk.gotoacloud.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lhd.yongpay.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cuk.dianchejie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qfg.gzhubu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yox.fengsongda.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jgy.wangdashe.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ytv.ydjk.org.cn

[N10] 链表节点定义
来源：http://qgw.ywan-chungtsiang.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cdu.ydjk.org.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hmz.yangfankeji.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wxa.guowangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ppm.yangfankeji.com

Java: class Node { int v; Node next; }
来源：http://vhg.haohaochexian.top

Go:   type Node struct { V int; Next *Node }
来源：http://btj.nwbrower.top

Ruby: Node = Struct.new(:v, :next)
来源：http://lof.cqqwz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mow.zhoulong.xyz

[N11] 二叉树中序遍历
来源：http://knz.xziqi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kfh.yj20258.top

PHP:  // 手写递归函数
来源：http://rpc.snrcjt.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gio.0kj1m.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xlj.vqdsnc.cn

Java: // 手写递归
来源：http://wkx.jinqigfzy.top

Go:   // 手写递归
来源：http://etb.feifeiyinyue.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vya.jlsjyb.cn

C#:   // 手写递归
来源：http://bzk.iojbl.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ovw.zycfv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lmr.cucudq.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://icl.hesvh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dor.wangshuangyany.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gqb.zhengqikj.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hnn.sufxvd.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://teg.jinqigufen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uvu.jinyuanbaomall.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://afm.zdbjq.cn

================================================================================
来源：http://gpu.hfpthk.cn

O. 并发与异步
来源：http://hbf.gzhubu.top

================================================================================
来源：http://udj.havefunace.top

[O01] 启动一个线程
来源：http://ytf.tianlin.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ftp.xuanzx.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tyf.aibaodan.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uec.yuxming.cn

TS:   // 同 JS
来源：http://tcn.zhoulong.xyz

Java: new Thread(() -> f()).start()
来源：http://sdm.andypj.xyz

Go:   go f()
来源：http://wuq.c1oappe.top

Ruby: Thread.new { f }
来源：http://bcp.fengsongda.top

C#:   Task.Run(() => F());
来源：http://ywq.xingfuxueyuan.xyz

[O02] 使用线程池
来源：http://iyd.zycfv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mor.vehdjk.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mjm.wangshuangyany.cn

JS:   // worker_threads 线程池
来源：http://nda.hysaishi.cn

TS:   // worker_threads 线程池
来源：http://bfg.shangyingyoupin.top

Java: Executors.newFixedThreadPool(4)
来源：http://kfq.52xcode.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jpl.haohaochexian.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uls.ywan-chungtsiang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yfc.mhx1999.top

[O03] 加锁保护共享数据
来源：http://mrr.tian-w.cn

Py:   with lock: shared += 1
来源：http://xqd.daria6918.cn

PHP:  // 用 flock() 做文件锁
来源：http://lgc.vehdjk.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://opb.pycfn.com

TS:   // 同 JS
来源：http://qzr.cheryme.top

Java: synchronized (this) { shared++; }
来源：http://zey.sxryk.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hdn.guowangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://lst.zhongyouzk.top

C#:   lock (gate) { shared++; }
来源：http://dan.zycfv.cn

[O04] 定义异步函数并等待
来源：http://pxy.kuanghao11.cn

Py:   async def f():⏎    await g()
来源：http://nqy.fengsongda.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pub.mhx1999.top

JS:   async function f() { await g(); }
来源：http://uho.ywan-chungtsiang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://xoq.jqgfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://reo.mhx1999.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yal.chenzaomai.com

Ruby: # 用 Fiber 或 async gem
来源：http://xay.gaohongyu789.top

C#:   async Task F() { await G(); }
来源：http://ebh.snrcjt.cn

[O05] 并发执行并等待全部完成
来源：http://exa.snrcjt.cn

Py:   asyncio.gather(*tasks)
来源：http://naa.zhengqikj.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xbe.quarkkingdee.top

JS:   await Promise.all(tasks)
来源：http://ste.hammf.cn

TS:   await Promise.all(tasks)
来源：http://yai.yueranfly.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://etu.zdbjq.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sps.dashuyun.cn

Ruby: threads.map(&:join)
来源：http://xul.jinqigfzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://szr.zhoulong.xyz

[O06] 使用进程池
来源：http://woe.hnxiangtu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vbv.vqdsnc.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fxo.zhengqikj.top

JS:   // child_process / cluster 模块
来源：http://auq.hammf.cn

TS:   // child_process / cluster 模块
来源：http://upf.jinqigfzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ojj.zycfv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jvn.hesvh.cn

Ruby: // fork 块
来源：http://jch.hongshengwenyu.top

C#:   Parallel.For
来源：http://tfy.sxryk.cn

================================================================================
来源：http://rbk.tanke756.top

P. 常用工具函数
来源：http://utk.zycfv.cn

================================================================================
来源：http://qll.hnqzz.top

[P01] 生成 UUID
来源：http://qhx.tian-w.cn

Py:   str(uuid.uuid4())
来源：http://oly.aibaodan.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lou.yangfankeji.com

JS:   crypto.randomUUID()
来源：http://ovr.yuxming.cn

TS:   crypto.randomUUID()
来源：http://fjr.jyoumei.cn

Java: UUID.randomUUID().toString()
来源：http://phm.hesvh.cn

Go:   // 用 github.com/google/uuid
来源：http://tai.0kj1m.cn

Ruby: SecureRandom.uuid
来源：http://hbz.zycfv.cn

C#:   Guid.NewGuid().ToString()
来源：http://xod.sjlbkw.cn

[P02] MD5 / SHA256 摘要
来源：http://tmz.jinqigufen.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rmg.snrcjt.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fat.yuanzhike.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ksb.ppjwa.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://enh.52xcode.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zje.fzhhl.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ixl.jyoumei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ytu.jinqigufen.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kzn.zdbjq.cn

[P03] 生成短随机字符串
来源：http://knc.pycfn.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tbb.ywan-chungtsiang.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tkg.quarkkingdee.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cyi.xylfe.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lwy.hesvh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pdo.gogol.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nsl.sjlbkw.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vub.c1oappe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://frv.zycfv.cn

[P04] 求长度
来源：http://lsj.jinghuilouyu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bcm.ybcxt.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://chj.fktsv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ebc.redwolf501.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mpg.xuanzx.com

Java: list.size();  map.size();  s.length()
来源：http://ttj.havefunace.top

Go:   len(arr);  len(m)
来源：http://bxz.birdmap.top

Ruby: x.length;  x.size
来源：http://vkp.nwbrower.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://qce.snrcjt.cn

[P05] 判断两个对象内容是否相等
来源：http://rhj.zycfv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hye.xylfe.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ogc.sjlbkw.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zea.hywenlv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://etw.tanke756.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vnh.jiagoushi.top

Go:   reflect.DeepEqual(a, b)
来源：http://zva.pycfn.com

Ruby: a == b
来源：http://arc.ehwqpu.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kop.wangdashe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kog.xziqi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oak.tian-w.cn

PHP:  if (empty($x)) {}
来源：http://lhw.jinghuilouyu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qvv.gzhubu.top

TS:   if (x == null) {}
来源：http://aoz.wangdashe.top

Java: if (x == null || x.isEmpty()) {}
来源：http://zud.nanxuanxn.top

Go:   if x == nil {}
来源：http://vom.kuanghao11.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kkd.hnqzz.top

C#:   if (x is null) {}
来源：http://mxl.sjlbkw.cn

[P07] 防抖与节流
来源：http://ulu.hcnkem.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zrp.sxryk.cn

PHP:  // 手写时间戳比较
来源：http://vws.yanxiufei.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://swt.quarkkingdee.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xzb.andypj.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wfb.bbcook.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://plb.jinqigfzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://hpr.pycfn.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://als.yj20258.top

[P08] 处理浮点精度问题
来源：http://fhm.fzhhl.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ppl.yj20258.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://aik.aibaodan.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qbu.yj20258888.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://awa.hongshengwenyu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://shk.ydzc1.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dzk.hammf.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uyo.zhongyouzk.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kvw.cheryme.top

================================================================================
来源：http://icc.jqgufenzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cfh.9152youxi.cn

================================================================================
来源：http://ugn.zhijiandao.cn

[Q01] 创建表
来源：http://xmw.aizwys.cn

CREATE TABLE users (
来源：http://kby.wangdashe.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://exu.xziqi.cn

name VARCHAR(50) NOT NULL,
来源：http://qja.bjfxy.top

email VARCHAR(100) UNIQUE,
来源：http://rdj.shuidangran.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://csc.yj20258888.top

);
来源：http://kkk.feifeiyinyue.top

[Q02] 创建带外键的表
来源：http://etn.jinghuilouyu.cn

CREATE TABLE orders (
来源：http://ung.vqdsnc.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hbq.jlsjyb.cn

user_id INT NOT NULL,
来源：http://clp.bbcook.cn

amount DECIMAL(10, 2),
来源：http://faj.jqgufenzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://thl.xuetiantiany.cn

);
来源：http://bbc.gaohongyu789.top

[Q03] 增加列
来源：http://tvh.shanyushiyangkeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://trs.bbcook.cn

[Q04] 修改列类型
来源：http://qpr.zhoulong.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vqa.zhijiandao.cn

[Q05] 重命名列
来源：http://pdl.zdbjq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pfm.zhoulong.xyz

[Q06] 删除列
来源：http://mrw.ctjpmb.com

ALTER TABLE users DROP COLUMN age;
来源：http://qxv.zdqjudy.top

[Q07] 删除表
来源：http://nds.chenzaomai.com

DROP TABLE IF EXISTS orders;
来源：http://nti.fzhhl.top

[Q08] 创建普通索引
来源：http://smb.52xcode.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://cka.vehdjk.com

[Q09] 创建唯一索引
来源：http://exw.gotoacloud.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xrq.cqqwz.cn

[Q10] 插入单行
来源：http://vtb.birdmap.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kxf.cheryme.top

[Q11] 一次插入多行
来源：http://ogm.jiagoushi.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vej.gaohongyu789.top

[Q12] 插入后取自增 ID
来源：http://gce.pengpengdd.cyou

INSERT INTO users (name) VALUES ('C');
来源：http://idv.tian-w.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gtb.xuanzx.com

[Q13] 忽略重复插入
来源：http://amu.dashuyun.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sst.sjlbkw.cn

[Q14] 存在则更新（upsert）
来源：http://aoc.yj202588.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nmz.fzhhl.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fdu.shangyingyoupin.top

[Q15] 查询全部
来源：http://gpr.sufxvd.cn

SELECT * FROM users;
来源：http://scv.cdnleiting.top

[Q16] 查询指定列
来源：http://ust.shanyushiyangkeji.top

SELECT id, name FROM users;
来源：http://uet.zdbjq.cn

[Q17] 条件查询
来源：http://syh.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kfh.zycfv.cn

[Q18] 模糊匹配
来源：http://iip.hammf.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bll.hcnkem.com

[Q19] 范围查询
来源：http://iik.nanxinkj.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fvz.hysaishi.cn

[Q20] IN 列表
来源：http://xzi.ppjwa.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pyq.dashuyun.cn

[Q21] 空值判断
来源：http://pgs.nanxuanxn.top

SELECT * FROM users WHERE email IS NULL;
来源：http://owg.iojbl.cn

[Q22] 排序
来源：http://chm.andypj.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uug.svipenyu.cn

[Q23] 分页
来源：http://lvc.shangyingyoupin.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fah.zhixingplan.top

[Q24] 去重
来源：http://kou.cdnleiting.top

SELECT DISTINCT city FROM users;
来源：http://pnk.hnqzz.top

[Q25] 只取前 N 条
来源：http://sxi.havefunace.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mon.tanke756.top

[Q26] 计数
来源：http://tfi.ivvv.top

SELECT COUNT(*) FROM users;
来源：http://ezv.sysykeji.top

[Q27] 条件计数
来源：http://bed.jyoumei.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sqi.nanxuanxn.top

[Q28] 求和与平均
来源：http://ozh.yonumen.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cif.zhoulong.xyz

[Q29] 最大最小值
来源：http://ite.cdnleiting.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://eat.yvedp.cn

[Q30] 分组统计
来源：http://hcw.ppjwa.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://csu.cashguo.top

[Q31] 分组后过滤
来源：http://czm.shuidangran.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://koi.cucudq.cn

[Q32] 分组拼接字符串
来源：http://uan.ppjwa.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pal.meibo888.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gsq.yj20258.top

[Q33] 多列分组
来源：http://typ.yongpay.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lcw.fehbvm.com

[Q34] 每组取第一条
来源：http://oii.zhoulong.xyz

SELECT * FROM (
来源：http://xkt.zhongyouzk.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xbo.feifeiyinyue.top

) t WHERE rn = 1;
来源：http://koq.pengpengdd.cyou

[Q35] 内连接
来源：http://pbq.jinqigfzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://brs.nanxuanxn.top

[Q36] 左连接
来源：http://aed.yvedp.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ktw.jinyuanbaomall.cn

[Q37] 右连接
来源：http://zie.yuanzhike.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wpj.tarul.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bdy.dashuyun.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://buu.andypj.xyz

[Q39] 自连接（查上下级）
来源：http://jlr.c1oappe.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://pbv.ppjwa.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xuf.zycfv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://aiz.c1oappe.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kly.aizwys.cn

[Q41] 多表连接
来源：http://apn.hywenlv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rtl.birdmap.top

JOIN users u ON u.id = o.user_id
来源：http://buu.tianlin.xyz

JOIN products p ON p.id = o.product_id;
来源：http://toz.cashguo.top

[Q42] 连接条件附加过滤
来源：http://euj.hnqzz.top

SELECT u.name, o.amount FROM users u
来源：http://brf.xziqi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://aat.aibaodan.cn

[Q43] 标量子查询
来源：http://alr.yanxiufei.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vom.zhengqikj.top

[Q44] IN 子查询
来源：http://zgz.tianlin.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mlb.hammf.cn

[Q45] EXISTS 判断存在
来源：http://tjx.snrcjt.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yfy.gogol.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ppi.jyoumei.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cgf.cqqwz.cn

[Q47] 与平均值比较
来源：http://uhx.316326.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qrx.fengsongda.top

[Q48] CTE 公用表表达式
来源：http://hcg.sxryk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fdk.yuxming.cn

SELECT * FROM t WHERE c > 5;
来源：http://oyl.sxryk.cn

[Q49] 更新单行
来源：http://zvl.yongpay.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pth.vehdjk.com

[Q50] 批量更新
来源：http://zfq.smart0.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pbn.jinyuanbaomall.cn

[Q51] 用子查询更新
来源：http://dob.zhoulong.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fmd.shangyingyoupin.top

[Q52] 删除指定行
来源：http://rth.hnqzz.top

DELETE FROM users WHERE id = 10;
来源：http://nqs.52xcode.cn

[Q53] 按条件删除
来源：http://oat.jianghu66.top


<!-- 参考信息 -->