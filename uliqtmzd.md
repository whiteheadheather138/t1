代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ogu.redwolf501.top

[N10] 链表节点定义
来源：http://zti.jqgufenzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wfb.iojbl.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tji.gzhubu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gke.jiagoushi.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rpk.mhx1999.top

Java: class Node { int v; Node next; }
来源：http://hlw.quarkkingdee.top

Go:   type Node struct { V int; Next *Node }
来源：http://ven.cashguo.top

Ruby: Node = Struct.new(:v, :next)
来源：http://vck.xuetiantiany.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fcx.vehdjk.com

[N11] 二叉树中序遍历
来源：http://gmu.jqgfzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fnt.tanke756.top

PHP:  // 手写递归函数
来源：http://eoc.uphjek.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ian.mhx1999.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fnu.ppjwa.cn

Java: // 手写递归
来源：http://mmn.havefunace.top

Go:   // 手写递归
来源：http://fiv.hysaishi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lkl.shangyingyoupin.top

C#:   // 手写递归
来源：http://jmp.birdmap.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dtw.yangfankeji.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iju.snrcjt.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tcm.vqdsnc.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://thf.yfazqb.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rip.hfpthk.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://okv.tanke756.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://emy.zdqjudy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pwm.mhx1999.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uoj.316326.xyz

================================================================================
来源：http://xci.ybcxt.top

O. 并发与异步
来源：http://afi.sufxvd.cn

================================================================================
来源：http://fzv.yj202588.top

[O01] 启动一个线程
来源：http://vso.cdnleiting.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ico.xuetiantiany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://oaf.feifeiyinyue.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ycq.zhengqikj.top

TS:   // 同 JS
来源：http://upl.ydjk.org.cn

Java: new Thread(() -> f()).start()
来源：http://yuh.bjfxy.top

Go:   go f()
来源：http://jia.jianghu66.top

Ruby: Thread.new { f }
来源：http://fjc.vqdsnc.cn

C#:   Task.Run(() => F());
来源：http://tqp.yj20258.top

[O02] 使用线程池
来源：http://hdw.uphjek.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kxm.aibaodan.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ufb.shanyushiyangtech.top

JS:   // worker_threads 线程池
来源：http://vcr.sysykeji.top

TS:   // worker_threads 线程池
来源：http://gpd.redwolf501.top

Java: Executors.newFixedThreadPool(4)
来源：http://zvs.ivvv.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dqx.jyoumei.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ufh.yuanzhike.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ubc.aizwys.cn

[O03] 加锁保护共享数据
来源：http://jzz.sysykeji.top

Py:   with lock: shared += 1
来源：http://cej.zdqjudy.top

PHP:  // 用 flock() 做文件锁
来源：http://osl.zhijiandao.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iry.zhiwuduotai.top

TS:   // 同 JS
来源：http://uhb.zhoulong.xyz

Java: synchronized (this) { shared++; }
来源：http://nbz.wangdashe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ldr.andypj.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://ixd.aizwys.cn

C#:   lock (gate) { shared++; }
来源：http://wwi.ywan-chungtsiang.top

[O04] 定义异步函数并等待
来源：http://ytv.bbcook.cn

Py:   async def f():⏎    await g()
来源：http://alh.bjfxy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ynd.xuetiantiany.cn

JS:   async function f() { await g(); }
来源：http://svw.cheryme.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://nbk.jinqigufen.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uzr.tian-w.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cmj.0kj1m.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rft.aibaodan.cn

C#:   async Task F() { await G(); }
来源：http://ufl.ivvv.top

[O05] 并发执行并等待全部完成
来源：http://zhq.uphjek.com

Py:   asyncio.gather(*tasks)
来源：http://gku.jinqigfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rgb.svipenyu.cn

JS:   await Promise.all(tasks)
来源：http://fad.uphjek.com

TS:   await Promise.all(tasks)
来源：http://lqz.9152youxi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vtf.pycfn.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://iwq.jinqigfzy.top

Ruby: threads.map(&:join)
来源：http://kub.sufxvd.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://oaj.zhoulong.xyz

[O06] 使用进程池
来源：http://kmu.yangfankeji.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sch.kuanghao11.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pzs.zycfv.cn

JS:   // child_process / cluster 模块
来源：http://rqi.jiagoushi.top

TS:   // child_process / cluster 模块
来源：http://byv.yonumen.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://omd.gzhubu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vng.aizwys.cn

Ruby: // fork 块
来源：http://viz.hongshengwenyu.top

C#:   Parallel.For
来源：http://gwb.hnqzz.top

================================================================================
来源：http://pyq.ywan-chungtsiang.top

P. 常用工具函数
来源：http://viv.zhengqikj.top

================================================================================
来源：http://ham.kuanghao11.cn

[P01] 生成 UUID
来源：http://meu.sufxvd.cn

Py:   str(uuid.uuid4())
来源：http://mrx.chenzaomai.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qkl.shanyushiyangkeji.top

JS:   crypto.randomUUID()
来源：http://zph.fehbvm.com

TS:   crypto.randomUUID()
来源：http://fng.ywan-chungtsiang.top

Java: UUID.randomUUID().toString()
来源：http://ttn.yongpay.top

Go:   // 用 github.com/google/uuid
来源：http://jgc.jyoumei.cn

Ruby: SecureRandom.uuid
来源：http://enm.fehbvm.com

C#:   Guid.NewGuid().ToString()
来源：http://ofk.birdmap.top

[P02] MD5 / SHA256 摘要
来源：http://ylv.mhx1999.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://urn.aibaodan.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sir.birdmap.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qnb.fzhhl.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://buo.zdqjudy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uhy.shuidangran.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lkz.gogol.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yut.feifeiyinyue.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ysk.xziqi.cn

[P03] 生成短随机字符串
来源：http://vtv.epnwcf.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tqt.hfpthk.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://itk.cucudq.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vyr.xinyue.icu

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://joz.52xcode.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uqw.smart0.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iby.sxryk.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jsq.aibaodan.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ysk.svipenyu.cn

[P04] 求长度
来源：http://qtv.fanxiaobao.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pvg.wangdashe.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lpg.hnqzz.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wwi.fzhhl.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rqt.fzhhl.top

Java: list.size();  map.size();  s.length()
来源：http://wae.shanyushiyangtech.top

Go:   len(arr);  len(m)
来源：http://mik.jinyuanbaomall.cn

Ruby: x.length;  x.size
来源：http://aix.shuidangran.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xor.hcnkem.com

[P05] 判断两个对象内容是否相等
来源：http://oqr.chenzaomai.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://hhu.hesvh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kjk.andypj.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://eqj.ctjpmb.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://roz.wangdashe.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ywm.jianghu66.top

Go:   reflect.DeepEqual(a, b)
来源：http://cls.xuetiantiany.cn

Ruby: a == b
来源：http://iop.svipenyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://taj.zhaomingkeji.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nmb.tianlin.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vrc.sysykeji.top

PHP:  if (empty($x)) {}
来源：http://fqv.yfazqb.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fgw.birdmap.top

TS:   if (x == null) {}
来源：http://cym.jinghuilouyu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jug.shangyingyoupin.top

Go:   if x == nil {}
来源：http://uru.chenzaomai.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://iso.hnxiangtu.top

C#:   if (x is null) {}
来源：http://fnr.zhengqikj.top

[P07] 防抖与节流
来源：http://pmo.ivvv.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://suz.zdqjudy.top

PHP:  // 手写时间戳比较
来源：http://deo.jinqigufen.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hcn.jqgufenzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fdt.iojbl.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pwi.guowangkeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rwy.ivvv.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://apm.pengpengdd.cyou

C#:   // 用 System.Timers.Timer 重置实现
来源：http://iwr.vqdsnc.cn

[P08] 处理浮点精度问题
来源：http://nve.pycfn.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://aky.zhengqikj.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://inw.yonumen.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jvj.meibo888.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mau.andypj.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jne.jyoumei.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eur.hesvh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://krn.yfazqb.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ayg.epnwcf.com

================================================================================
来源：http://oyh.zhoulong.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://whg.ydjk.org.cn

================================================================================
来源：http://zpn.ywan-chungtsiang.top

[Q01] 创建表
来源：http://hbl.aibaodan.cn

CREATE TABLE users (
来源：http://edq.jqgufenzy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kmq.yueranfly.top

name VARCHAR(50) NOT NULL,
来源：http://jpw.nwbrower.top

email VARCHAR(100) UNIQUE,
来源：http://gzw.yangfankeji.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nzc.gzhubu.top

);
来源：http://gvz.haohaochexian.top

[Q02] 创建带外键的表
来源：http://sku.daria6918.cn

CREATE TABLE orders (
来源：http://pci.meibo888.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mdy.ivvv.top

user_id INT NOT NULL,
来源：http://kqr.yueranfly.top

amount DECIMAL(10, 2),
来源：http://viu.jlsjyb.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://giv.daria6918.cn

);
来源：http://vrv.jianghu66.top

[Q03] 增加列
来源：http://ukv.316326.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://paz.zdbjq.cn

[Q04] 修改列类型
来源：http://pdj.gzhubu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wxh.chenjidiqi.icu

[Q05] 重命名列
来源：http://juz.gogol.net.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://csv.ydjk.org.cn

[Q06] 删除列
来源：http://bxg.tanke756.top

ALTER TABLE users DROP COLUMN age;
来源：http://tic.shuidangran.top

[Q07] 删除表
来源：http://uvy.tanke756.top

DROP TABLE IF EXISTS orders;
来源：http://utb.bjfxy.top

[Q08] 创建普通索引
来源：http://nem.hysaishi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://czb.fanxiaobao.xyz

[Q09] 创建唯一索引
来源：http://raa.andypj.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ojq.chenlongwang.top

[Q10] 插入单行
来源：http://xfm.tianlin.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ofw.jinyuanbaomall.cn

[Q11] 一次插入多行
来源：http://ejr.shuidangran.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rqk.zdbjq.cn

[Q12] 插入后取自增 ID
来源：http://kru.hnxiangtu.top

INSERT INTO users (name) VALUES ('C');
来源：http://ojn.xinyue.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wge.wangshuangyany.cn

[Q13] 忽略重复插入
来源：http://kle.hnqzz.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fwl.vqdsnc.cn

[Q14] 存在则更新（upsert）
来源：http://asv.yj202588.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qyc.ywan-chungtsiang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ypw.shangyingyoupin.top

[Q15] 查询全部
来源：http://bhb.hfpthk.cn

SELECT * FROM users;
来源：http://zlj.tarul.cn

[Q16] 查询指定列
来源：http://zws.yuxming.cn

SELECT id, name FROM users;
来源：http://ipf.iojbl.cn

[Q17] 条件查询
来源：http://oih.cdnleiting.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wzq.chenlongwang.top

[Q18] 模糊匹配
来源：http://ubo.shzxlz.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yde.hnqzz.top

[Q19] 范围查询
来源：http://cbu.xuanzx.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ntj.zhixingplan.top

[Q20] IN 列表
来源：http://uun.smart0.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oqb.sysykeji.top

[Q21] 空值判断
来源：http://psi.yj20258888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://xqm.gzhubu.top

[Q22] 排序
来源：http://nog.zhongyouzk.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://smy.cashguo.top

[Q23] 分页
来源：http://zmi.0kj1m.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xmc.yueranfly.top

[Q24] 去重
来源：http://hlp.nwbrower.top

SELECT DISTINCT city FROM users;
来源：http://dkk.hnqzz.top

[Q25] 只取前 N 条
来源：http://gfu.yangfankeji.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://boh.316326.xyz

[Q26] 计数
来源：http://gdt.sxryk.cn

SELECT COUNT(*) FROM users;
来源：http://fab.jiagoushi.top

[Q27] 条件计数
来源：http://swt.hfpthk.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://llz.yonumen.top

[Q28] 求和与平均
来源：http://ihs.c1oappe.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fwq.jinqigfzy.top

[Q29] 最大最小值
来源：http://ufm.jiagoushi.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://add.chenzaomai.com

[Q30] 分组统计
来源：http://lwl.jlsjyb.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ftr.hywenlv.cn

[Q31] 分组后过滤
来源：http://aou.jinyuanbaomall.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://csr.xuetiantiany.cn

[Q32] 分组拼接字符串
来源：http://fck.guannengcc.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gao.yvedp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gvo.zhiwuduotai.top

[Q33] 多列分组
来源：http://tfo.gotoacloud.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rca.xinyue.icu

[Q34] 每组取第一条
来源：http://any.jqgufenzy.top

SELECT * FROM (
来源：http://wjj.havefunace.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sow.xziqi.cn

) t WHERE rn = 1;
来源：http://vbi.sysykeji.top

[Q35] 内连接
来源：http://ezf.jinqigfzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://joh.aizwys.cn

[Q36] 左连接
来源：http://omg.daxiang520.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mld.gogol.net.cn

[Q37] 右连接
来源：http://cfn.hfpthk.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pal.ybcxt.top

[Q38] 全外连接（PostgreSQL）
来源：http://sew.ivvv.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://duc.shanyushiyangtech.top

[Q39] 自连接（查上下级）
来源：http://wbw.redwolf501.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://quj.hnqzz.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ncf.tanke756.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xwt.sweek.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dul.bbcook.cn

[Q41] 多表连接
来源：http://qhf.yfazqb.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://esy.316326.xyz

JOIN users u ON u.id = o.user_id
来源：http://ops.zycfv.cn

JOIN products p ON p.id = o.product_id;
来源：http://ehf.hnxiangtu.top

[Q42] 连接条件附加过滤
来源：http://ivs.jqgfzy.top

SELECT u.name, o.amount FROM users u
来源：http://pqu.aibaodan.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rko.xuetiantiany.cn

[Q43] 标量子查询
来源：http://dte.aizwys.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vgd.zycfv.cn

[Q44] IN 子查询
来源：http://dkg.tianlin.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xhd.52xcode.cn

[Q45] EXISTS 判断存在
来源：http://zbf.vqdsnc.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tka.wangshuangyany.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dgg.zdbjq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://anw.xingfuxueyuan.xyz

[Q47] 与平均值比较
来源：http://qyl.jqgufenzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nrr.sweek.top

[Q48] CTE 公用表表达式
来源：http://xtd.hesvh.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uur.pengpengdd.cyou

SELECT * FROM t WHERE c > 5;
来源：http://upl.zhengqikj.top

[Q49] 更新单行
来源：http://oar.pengpengdd.cyou

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mbz.c1oappe.top

[Q50] 批量更新
来源：http://fie.redwolf501.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mvu.zhengqikj.top

[Q51] 用子查询更新
来源：http://ssc.tianlin.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mtq.jlsjyb.cn

[Q52] 删除指定行
来源：http://xop.yuanzhike.top

DELETE FROM users WHERE id = 10;
来源：http://bql.9152youxi.cn

[Q53] 按条件删除
来源：http://wcr.fehbvm.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://enn.zycfv.cn

[Q54] 清空表
来源：http://xyl.fktsv.cn

TRUNCATE TABLE logs;
来源：http://top.guowangkeji.top

[Q55] 排名（并列占位）
来源：http://fcu.bbcook.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mei.jinyuanbaomall.cn

[Q56] 密集排名（并列不占位）
来源：http://kwx.cheryme.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ohq.zhijiandao.cn

[Q57] 行号
来源：http://mot.hammf.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://izl.vqdsnc.cn

[Q58] 累计求和
来源：http://ouu.daxiang520.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dgh.gzhubu.top

[Q59] 分组内累计
来源：http://ajj.guowangkeji.top


<!-- 参考信息 -->