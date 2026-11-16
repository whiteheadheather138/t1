代发 wailian999

[N09] 栈与队列
来源：http://pqo.xziqi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://axv.fktsv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uom.fktsv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yvd.yonumen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zkb.cucudq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ysl.guannengcc.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://esw.cashguo.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gbh.hcnkem.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ubg.yvedp.cn

[N10] 链表节点定义
来源：http://qws.yangfankeji.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zvw.yvedp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mrv.yonumen.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zyj.yuanzhike.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://txp.vehdjk.com

Java: class Node { int v; Node next; }
来源：http://bmp.yuanzhike.top

Go:   type Node struct { V int; Next *Node }
来源：http://tdc.meibo888.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wkz.kuanghao11.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://tpt.shuidangran.top

[N11] 二叉树中序遍历
来源：http://dro.52xcode.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lep.shangyingyoupin.top

PHP:  // 手写递归函数
来源：http://kgx.jlsjyb.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rpw.andypj.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rxk.sufxvd.cn

Java: // 手写递归
来源：http://iyo.ybcxt.top

Go:   // 手写递归
来源：http://nuc.ydjk.org.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gzw.ydzc1.top

C#:   // 手写递归
来源：http://rso.0kj1m.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://puu.jlsjyb.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tmq.9152youxi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mxg.aibaodan.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://miy.hongshengwenyu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pco.yongpay.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sun.vehdjk.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gie.yangfankeji.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ofq.xylfe.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bum.shanyushiyangkeji.top

================================================================================
来源：http://xul.hywenlv.cn

O. 并发与异步
来源：http://lfy.fanxiaobao.xyz

================================================================================
来源：http://yih.snrcjt.cn

[O01] 启动一个线程
来源：http://gfa.jqgufenzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qig.c1oappe.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://alq.bjfxy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://urp.yanxiufei.cn

TS:   // 同 JS
来源：http://rxw.fanxiaobao.xyz

Java: new Thread(() -> f()).start()
来源：http://uxg.jinyuanbaomall.cn

Go:   go f()
来源：http://dnv.yueranfly.top

Ruby: Thread.new { f }
来源：http://pim.shanyushiyangkeji.top

C#:   Task.Run(() => F());
来源：http://cuu.yueranfly.top

[O02] 使用线程池
来源：http://usk.yfazqb.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kff.52xcode.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kat.dashuyun.cn

JS:   // worker_threads 线程池
来源：http://nrn.yanxiufei.cn

TS:   // worker_threads 线程池
来源：http://ndm.yangfankeji.com

Java: Executors.newFixedThreadPool(4)
来源：http://dxh.gogol.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jkp.fehbvm.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://aej.iojbl.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xju.xylfe.cn

[O03] 加锁保护共享数据
来源：http://juf.hcnkem.com

Py:   with lock: shared += 1
来源：http://biy.zhengqikj.top

PHP:  // 用 flock() 做文件锁
来源：http://kub.hnxiangtu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ggi.nanxinkj.top

TS:   // 同 JS
来源：http://mrz.shangyingyoupin.top

Java: synchronized (this) { shared++; }
来源：http://rkm.cucudq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uqn.fanxiaobao.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://qqa.xinyue.icu

C#:   lock (gate) { shared++; }
来源：http://dqs.daxiang520.top

[O04] 定义异步函数并等待
来源：http://sjw.yongpay.top

Py:   async def f():⏎    await g()
来源：http://nsa.zhijiandao.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wiq.c1oappe.top

JS:   async function f() { await g(); }
来源：http://mja.hammf.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://sub.guowangkeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://msr.zycfv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ldh.feifeiyinyue.top

Ruby: # 用 Fiber 或 async gem
来源：http://gzr.chenlongwang.top

C#:   async Task F() { await G(); }
来源：http://nkl.xuetiantiany.cn

[O05] 并发执行并等待全部完成
来源：http://pkn.fengsongda.top

Py:   asyncio.gather(*tasks)
来源：http://mmi.zdbjq.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rlt.cucudq.cn

JS:   await Promise.all(tasks)
来源：http://wbz.ctjpmb.com

TS:   await Promise.all(tasks)
来源：http://pui.yueranfly.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jem.yonumen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oij.guannengcc.top

Ruby: threads.map(&:join)
来源：http://yhl.yanxiufei.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sca.c1oappe.top

[O06] 使用进程池
来源：http://iak.tarul.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dte.chenlongwang.top

PHP:  // pcntl_fork 或多进程队列
来源：http://cdx.xuanzx.com

JS:   // child_process / cluster 模块
来源：http://zkt.ydzc1.top

TS:   // child_process / cluster 模块
来源：http://unv.9152youxi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tcx.shanyushiyangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ckd.andypj.xyz

Ruby: // fork 块
来源：http://xpj.pycfn.com

C#:   Parallel.For
来源：http://fom.xziqi.cn

================================================================================
来源：http://bvd.guowangkeji.top

P. 常用工具函数
来源：http://npi.shanyushiyangkeji.top

================================================================================
来源：http://yty.jqgufenzy.top

[P01] 生成 UUID
来源：http://dyf.epnwcf.com

Py:   str(uuid.uuid4())
来源：http://pqi.c1oappe.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lmx.yongpay.top

JS:   crypto.randomUUID()
来源：http://kcz.jiagoushi.top

TS:   crypto.randomUUID()
来源：http://yca.c1oappe.top

Java: UUID.randomUUID().toString()
来源：http://yir.nwbrower.top

Go:   // 用 github.com/google/uuid
来源：http://mjw.hammf.cn

Ruby: SecureRandom.uuid
来源：http://qmf.zdqjudy.top

C#:   Guid.NewGuid().ToString()
来源：http://yyz.nwbrower.top

[P02] MD5 / SHA256 摘要
来源：http://acp.smart0.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ckx.fktsv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qsd.ybcxt.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rci.pycfn.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gji.aibaodan.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qut.ydzc1.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yvf.zhoulong.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ghr.hysaishi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lna.yonumen.top

[P03] 生成短随机字符串
来源：http://nvw.quarkkingdee.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ljy.fengsongda.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bku.ivvv.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ryy.jianghu66.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mss.yonumen.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gre.zhiwuduotai.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ogl.havefunace.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://iax.zhiwuduotai.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://omo.tarul.cn

[P04] 求长度
来源：http://rof.tianlin.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://luk.xingfuxueyuan.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dew.cucudq.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ogr.yj20258.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vnb.hnqzz.top

Java: list.size();  map.size();  s.length()
来源：http://fhe.fanxiaobao.xyz

Go:   len(arr);  len(m)
来源：http://bku.quarkkingdee.top

Ruby: x.length;  x.size
来源：http://yvl.hongshengwenyu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://rfw.fzhhl.top

[P05] 判断两个对象内容是否相等
来源：http://esg.cashguo.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ykj.jianghu66.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rcb.cqqwz.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://clu.yfazqb.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tvg.zdbjq.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uyj.chenjidiqi.icu

Go:   reflect.DeepEqual(a, b)
来源：http://xdz.jinghuilouyu.cn

Ruby: a == b
来源：http://xtg.yanxiufei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cid.yj20258888.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bza.ehwqpu.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uyb.sxryk.cn

PHP:  if (empty($x)) {}
来源：http://ryt.aibaodan.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rds.0kj1m.cn

TS:   if (x == null) {}
来源：http://csb.xziqi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vzr.zhiwuduotai.top

Go:   if x == nil {}
来源：http://sfb.hysaishi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cyf.tanke756.top

C#:   if (x is null) {}
来源：http://phg.yfazqb.com

[P07] 防抖与节流
来源：http://uow.jqgufenzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pui.yonumen.top

PHP:  // 手写时间戳比较
来源：http://kfs.dashuyun.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xzx.guannengcc.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ztk.jinghuilouyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://utb.hysaishi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kun.sysykeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://arf.sxryk.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://son.hnxiangtu.top

[P08] 处理浮点精度问题
来源：http://kug.andypj.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xqt.tianlin.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jgb.zhoulong.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lay.vehdjk.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fme.birdmap.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dww.yuxming.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dhd.yanxiufei.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nbe.yfazqb.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://oqj.dianchejie.cn

================================================================================
来源：http://jic.bjfxy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tev.chenzaomai.com

================================================================================
来源：http://mgz.sxryk.cn

[Q01] 创建表
来源：http://ygl.shanyushiyangkeji.top

CREATE TABLE users (
来源：http://xxy.yangfankeji.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bzt.yonumen.top

name VARCHAR(50) NOT NULL,
来源：http://tbi.zdqjudy.top

email VARCHAR(100) UNIQUE,
来源：http://mml.iojbl.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xom.ppjwa.cn

);
来源：http://vur.bjfxy.top

[Q02] 创建带外键的表
来源：http://yck.52xcode.cn

CREATE TABLE orders (
来源：http://hri.ehwqpu.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://znx.epnwcf.com

user_id INT NOT NULL,
来源：http://dmb.c1oappe.top

amount DECIMAL(10, 2),
来源：http://hcu.wangshuangyany.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ldu.pycfn.com

);
来源：http://iiz.hfpthk.cn

[Q03] 增加列
来源：http://lwj.jqgufenzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ofi.fzhhl.top

[Q04] 修改列类型
来源：http://cny.ydzc1.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ucn.epnwcf.com

[Q05] 重命名列
来源：http://fvj.wangdashe.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hlz.pycfn.com

[Q06] 删除列
来源：http://oup.wangshuangyany.cn

ALTER TABLE users DROP COLUMN age;
来源：http://nca.shzxlz.cn

[Q07] 删除表
来源：http://ohn.yuxming.cn

DROP TABLE IF EXISTS orders;
来源：http://fvr.andypj.xyz

[Q08] 创建普通索引
来源：http://ibt.c1oappe.top

CREATE INDEX idx_users_email ON users(email);
来源：http://srn.daria6918.cn

[Q09] 创建唯一索引
来源：http://zya.sysykeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ytg.wangshuangyany.cn

[Q10] 插入单行
来源：http://uny.jyoumei.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://swt.kuanghao11.cn

[Q11] 一次插入多行
来源：http://bew.nanxuanxn.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://thn.havefunace.top

[Q12] 插入后取自增 ID
来源：http://lbq.zycfv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fdi.shanyushiyangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dfl.feifeiyinyue.top

[Q13] 忽略重复插入
来源：http://ejj.zhengqikj.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wtd.ivvv.top

[Q14] 存在则更新（upsert）
来源：http://hth.gaohongyu789.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://usr.ybcxt.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bmr.yuxming.cn

[Q15] 查询全部
来源：http://yci.birdmap.top

SELECT * FROM users;
来源：http://jio.meibo888.top

[Q16] 查询指定列
来源：http://ltr.zdqjudy.top

SELECT id, name FROM users;
来源：http://evw.0kj1m.cn

[Q17] 条件查询
来源：http://jci.pengpengdd.cyou

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uql.ybcxt.top

[Q18] 模糊匹配
来源：http://vcd.cheryme.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xas.hfpthk.cn

[Q19] 范围查询
来源：http://jvd.ybcxt.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://epz.cashguo.top

[Q20] IN 列表
来源：http://fxa.wangshuangyany.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://eta.smart0.xyz

[Q21] 空值判断
来源：http://ocg.svipenyu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mcv.gotoacloud.top

[Q22] 排序
来源：http://jfr.yj20258.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://oab.xingfuxueyuan.xyz

[Q23] 分页
来源：http://kou.hcnkem.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rds.daria6918.cn

[Q24] 去重
来源：http://rhy.yuanzhike.top

SELECT DISTINCT city FROM users;
来源：http://odn.zhijiandao.cn

[Q25] 只取前 N 条
来源：http://qsp.jyoumei.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ycy.aibaodan.cn

[Q26] 计数
来源：http://vrh.xingfuxueyuan.xyz

SELECT COUNT(*) FROM users;
来源：http://gao.pycfn.com

[Q27] 条件计数
来源：http://vob.jlsjyb.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://sfd.xylfe.cn

[Q28] 求和与平均
来源：http://efk.tarul.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lmy.52xcode.cn

[Q29] 最大最小值
来源：http://jby.yuxming.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yis.hesvh.cn

[Q30] 分组统计
来源：http://ccl.yanxiufei.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sth.tian-w.cn

[Q31] 分组后过滤
来源：http://aqk.zhixingplan.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://atp.feifeiyinyue.top

[Q32] 分组拼接字符串
来源：http://xzj.bjfxy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ldh.yonumen.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xph.cqqwz.cn

[Q33] 多列分组
来源：http://tao.dashuyun.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lrt.yangfankeji.com

[Q34] 每组取第一条
来源：http://buz.xylfe.cn

SELECT * FROM (
来源：http://prm.tanke756.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ljf.vqdsnc.cn

) t WHERE rn = 1;
来源：http://nsz.svipenyu.cn

[Q35] 内连接
来源：http://ala.yvedp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mtb.fanxiaobao.xyz

[Q36] 左连接
来源：http://lfo.daria6918.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fnc.hesvh.cn

[Q37] 右连接
来源：http://bvf.ivvv.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://edm.bbcook.cn

[Q38] 全外连接（PostgreSQL）
来源：http://huk.yvedp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qyn.vehdjk.com

[Q39] 自连接（查上下级）
来源：http://ffb.cdnleiting.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://zec.sweek.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ibb.shanyushiyangtech.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ddq.hcnkem.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ofl.nanxinkj.top

[Q41] 多表连接
来源：http://dfm.c1oappe.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://bpi.vqdsnc.cn

JOIN users u ON u.id = o.user_id
来源：http://lbk.guannengcc.top

JOIN products p ON p.id = o.product_id;
来源：http://eqc.epnwcf.com

[Q42] 连接条件附加过滤
来源：http://reg.jqgfzy.top

SELECT u.name, o.amount FROM users u
来源：http://clf.ywan-chungtsiang.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mza.yuxming.cn

[Q43] 标量子查询
来源：http://ogf.xuanzx.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rvk.nanxuanxn.top

[Q44] IN 子查询
来源：http://bvi.dashuyun.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fls.sjlbkw.cn

[Q45] EXISTS 判断存在
来源：http://vfz.ywan-chungtsiang.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nyh.zdqjudy.top

[Q46] NOT EXISTS 判断不存在
来源：http://xni.tian-w.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://knc.yuxming.cn

[Q47] 与平均值比较
来源：http://usb.ehwqpu.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://moz.xylfe.cn

[Q48] CTE 公用表表达式
来源：http://cip.shanyushiyangkeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qys.xingfuxueyuan.xyz

SELECT * FROM t WHERE c > 5;
来源：http://spr.jinyuanbaomall.cn

[Q49] 更新单行
来源：http://rcg.cdnleiting.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yaj.yj20258.top

[Q50] 批量更新
来源：http://urt.nwbrower.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jos.ivvv.top

[Q51] 用子查询更新
来源：http://hzp.dashuyun.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wbh.meibo888.top

[Q52] 删除指定行
来源：http://uuw.feifeiyinyue.top

DELETE FROM users WHERE id = 10;
来源：http://imr.birdmap.top

[Q53] 按条件删除
来源：http://sri.kuanghao11.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rij.zycfv.cn

[Q54] 清空表
来源：http://lyc.xziqi.cn

TRUNCATE TABLE logs;
来源：http://cch.shanyushiyangtech.top

[Q55] 排名（并列占位）
来源：http://ial.gotoacloud.top


<!-- 参考信息 -->