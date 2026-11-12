代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wje.316326.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vkr.gotoacloud.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mkg.shanyushiyangkeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vcn.wangshuangyany.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lzr.aizwys.cn

[N10] 链表节点定义
来源：http://pvx.yanxiufei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ipb.shuidangran.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mai.bjfxy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mwx.meibo888.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jsg.zhongyouzk.top

Java: class Node { int v; Node next; }
来源：http://oaq.kuanghao11.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xox.hongshengwenyu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://drd.uphjek.com

C#:   class Node { public int V; public Node? Next; }
来源：http://lno.jinghuilouyu.cn

[N11] 二叉树中序遍历
来源：http://wey.hnqzz.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://umb.hywenlv.cn

PHP:  // 手写递归函数
来源：http://qzr.cqqwz.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mrj.shanyushiyangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qai.birdmap.top

Java: // 手写递归
来源：http://yux.vehdjk.com

Go:   // 手写递归
来源：http://cbl.mhx1999.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zgp.epnwcf.com

C#:   // 手写递归
来源：http://fzu.xuanzx.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://iyo.sysykeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zdw.dashuyun.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uuc.sxryk.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bcm.chenjidiqi.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mxd.zhijiandao.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bcl.316326.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sqp.gaohongyu789.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gxs.vehdjk.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xgg.hnxiangtu.top

================================================================================
来源：http://reb.yj20258.top

O. 并发与异步
来源：http://fts.zhiwuduotai.top

================================================================================
来源：http://sry.bbcook.cn

[O01] 启动一个线程
来源：http://rti.gzhubu.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sfl.hywenlv.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wet.xingfuxueyuan.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kfp.zycfv.cn

TS:   // 同 JS
来源：http://sxq.nwbrower.top

Java: new Thread(() -> f()).start()
来源：http://qbm.jinqigfzy.top

Go:   go f()
来源：http://xav.pengpengdd.cyou

Ruby: Thread.new { f }
来源：http://frd.aizwys.cn

C#:   Task.Run(() => F());
来源：http://tpe.zhoulong.xyz

[O02] 使用线程池
来源：http://dzr.fktsv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wbc.gaohongyu789.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://efx.chenlongwang.top

JS:   // worker_threads 线程池
来源：http://hsp.zhijiandao.cn

TS:   // worker_threads 线程池
来源：http://ero.yueranfly.top

Java: Executors.newFixedThreadPool(4)
来源：http://qzp.0kj1m.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yvh.jianghu66.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rxa.nanxinkj.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gse.tian-w.cn

[O03] 加锁保护共享数据
来源：http://jwz.sxryk.cn

Py:   with lock: shared += 1
来源：http://kyl.tarul.cn

PHP:  // 用 flock() 做文件锁
来源：http://giz.jianghu66.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qoc.xziqi.cn

TS:   // 同 JS
来源：http://cap.cdnleiting.top

Java: synchronized (this) { shared++; }
来源：http://rwv.svipenyu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xve.ybcxt.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jgv.jlsjyb.cn

C#:   lock (gate) { shared++; }
来源：http://tzj.yanxiufei.cn

[O04] 定义异步函数并等待
来源：http://bvg.9152youxi.cn

Py:   async def f():⏎    await g()
来源：http://qiq.cqqwz.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pkr.yongpay.top

JS:   async function f() { await g(); }
来源：http://uxe.hysaishi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qdo.316326.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ifb.yongpay.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oxr.xylfe.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rbc.nwbrower.top

C#:   async Task F() { await G(); }
来源：http://ade.hesvh.cn

[O05] 并发执行并等待全部完成
来源：http://vwv.nanxinkj.top

Py:   asyncio.gather(*tasks)
来源：http://zrz.yueranfly.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ysg.yueranfly.top

JS:   await Promise.all(tasks)
来源：http://hgf.nanxuanxn.top

TS:   await Promise.all(tasks)
来源：http://kem.ydzc1.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xgd.quarkkingdee.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://biw.316326.xyz

Ruby: threads.map(&:join)
来源：http://mcm.zhongyouzk.top

C#:   await Task.WhenAll(t1, t2)
来源：http://nkn.ctjpmb.com

[O06] 使用进程池
来源：http://kfi.mhx1999.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zgg.aibaodan.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tiq.shanyushiyangtech.top

JS:   // child_process / cluster 模块
来源：http://lbe.tianlin.xyz

TS:   // child_process / cluster 模块
来源：http://wiy.fengsongda.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ifw.xuetiantiany.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zih.ybcxt.top

Ruby: // fork 块
来源：http://zoq.316326.xyz

C#:   Parallel.For
来源：http://foz.yuanzhike.top

================================================================================
来源：http://wjp.jinghuilouyu.cn

P. 常用工具函数
来源：http://njm.yongpay.top

================================================================================
来源：http://rcq.sxryk.cn

[P01] 生成 UUID
来源：http://bht.yuxming.cn

Py:   str(uuid.uuid4())
来源：http://rbi.zhixingplan.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ctm.uphjek.com

JS:   crypto.randomUUID()
来源：http://qkj.chenzaomai.com

TS:   crypto.randomUUID()
来源：http://eys.andypj.xyz

Java: UUID.randomUUID().toString()
来源：http://doc.jqgfzy.top

Go:   // 用 github.com/google/uuid
来源：http://eed.yuanzhike.top

Ruby: SecureRandom.uuid
来源：http://dwu.redwolf501.top

C#:   Guid.NewGuid().ToString()
来源：http://mfn.smart0.xyz

[P02] MD5 / SHA256 摘要
来源：http://wvl.sysykeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uvs.ppjwa.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bby.jinyuanbaomall.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://joc.iojbl.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://itk.ehwqpu.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pig.yj20258.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fvv.c1oappe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dzo.316326.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ysc.redwolf501.top

[P03] 生成短随机字符串
来源：http://isb.vqdsnc.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sqp.jlsjyb.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gzq.redwolf501.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wjb.xinyue.icu

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fje.uphjek.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kot.tarul.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ggn.cqqwz.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://tdy.yj202588.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zja.yuanzhike.top

[P04] 求长度
来源：http://bhf.yvedp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://utp.hfpthk.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://woa.yueranfly.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xdp.iojbl.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://isd.hywenlv.cn

Java: list.size();  map.size();  s.length()
来源：http://qhv.jyoumei.cn

Go:   len(arr);  len(m)
来源：http://vhs.chenlongwang.top

Ruby: x.length;  x.size
来源：http://bpy.gaohongyu789.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://usv.wangshuangyany.cn

[P05] 判断两个对象内容是否相等
来源：http://fai.redwolf501.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://xog.shanyushiyangkeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rnz.9152youxi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qms.cashguo.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://une.zhoulong.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nuw.kuanghao11.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vnd.wangdashe.top

Ruby: a == b
来源：http://kmp.gaohongyu789.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ghq.uphjek.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hwf.ybcxt.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://quj.fzhhl.top

PHP:  if (empty($x)) {}
来源：http://exl.shangyingyoupin.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://eyi.hongshengwenyu.top

TS:   if (x == null) {}
来源：http://nos.yonumen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://kab.zhixingplan.top

Go:   if x == nil {}
来源：http://ukg.aizwys.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mxy.shangyingyoupin.top

C#:   if (x is null) {}
来源：http://crh.cheryme.top

[P07] 防抖与节流
来源：http://los.hfpthk.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nxe.fktsv.cn

PHP:  // 手写时间戳比较
来源：http://pkn.birdmap.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fhg.xuetiantiany.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xuv.jiagoushi.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://eor.yongpay.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://phm.sxryk.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fky.jiagoushi.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xvs.jinyuanbaomall.cn

[P08] 处理浮点精度问题
来源：http://utq.xziqi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://efe.gotoacloud.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ttd.zhoulong.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nbg.shanyushiyangtech.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://how.xuetiantiany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yiy.aizwys.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://msj.cqqwz.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uxx.jinyuanbaomall.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gzn.zhiwuduotai.top

================================================================================
来源：http://hkl.hcnkem.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fry.tian-w.cn

================================================================================
来源：http://fyx.yvedp.cn

[Q01] 创建表
来源：http://sbp.ivvv.top

CREATE TABLE users (
来源：http://hxu.ppjwa.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://stt.xinyue.icu

name VARCHAR(50) NOT NULL,
来源：http://rrx.gzhubu.top

email VARCHAR(100) UNIQUE,
来源：http://qdb.aizwys.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://enf.chenzaomai.com

);
来源：http://jnk.havefunace.top

[Q02] 创建带外键的表
来源：http://syh.cucudq.cn

CREATE TABLE orders (
来源：http://exp.yangfankeji.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://chf.xziqi.cn

user_id INT NOT NULL,
来源：http://jce.xylfe.cn

amount DECIMAL(10, 2),
来源：http://wud.guannengcc.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rsb.chenlongwang.top

);
来源：http://trj.ivvv.top

[Q03] 增加列
来源：http://ejz.hcnkem.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cue.ybcxt.top

[Q04] 修改列类型
来源：http://yfu.tianlin.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dxp.sjlbkw.cn

[Q05] 重命名列
来源：http://edi.haohaochexian.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hha.guowangkeji.top

[Q06] 删除列
来源：http://wkw.jyoumei.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pmr.daria6918.cn

[Q07] 删除表
来源：http://kfc.c1oappe.top

DROP TABLE IF EXISTS orders;
来源：http://xel.ppjwa.cn

[Q08] 创建普通索引
来源：http://atd.jiagoushi.top

CREATE INDEX idx_users_email ON users(email);
来源：http://wxg.jinyuanbaomall.cn

[Q09] 创建唯一索引
来源：http://ukr.wangshuangyany.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tbm.hammf.cn

[Q10] 插入单行
来源：http://osx.kuanghao11.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fid.yfazqb.com

[Q11] 一次插入多行
来源：http://ptz.zhongyouzk.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nbi.fengsongda.top

[Q12] 插入后取自增 ID
来源：http://psb.chenzaomai.com

INSERT INTO users (name) VALUES ('C');
来源：http://kow.jiagoushi.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yhp.sysykeji.top

[Q13] 忽略重复插入
来源：http://xji.xuanzx.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ohu.316326.xyz

[Q14] 存在则更新（upsert）
来源：http://zfc.shuidangran.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://csk.hesvh.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kqr.c1oappe.top

[Q15] 查询全部
来源：http://wkh.cheryme.top

SELECT * FROM users;
来源：http://txw.nwbrower.top

[Q16] 查询指定列
来源：http://ycf.nwbrower.top

SELECT id, name FROM users;
来源：http://tlx.zhaomingkeji.xyz

[Q17] 条件查询
来源：http://vth.ivvv.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ghv.cdnleiting.top

[Q18] 模糊匹配
来源：http://cuw.yj20258.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wou.pycfn.com

[Q19] 范围查询
来源：http://qjy.sufxvd.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rdh.hywenlv.cn

[Q20] IN 列表
来源：http://wea.chenjidiqi.icu

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://aof.jinqigufen.top

[Q21] 空值判断
来源：http://gul.svipenyu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mop.birdmap.top

[Q22] 排序
来源：http://jup.snrcjt.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cbe.dashuyun.cn

[Q23] 分页
来源：http://jgc.shzxlz.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fas.zhixingplan.top

[Q24] 去重
来源：http://uop.daria6918.cn

SELECT DISTINCT city FROM users;
来源：http://tnd.quarkkingdee.top

[Q25] 只取前 N 条
来源：http://oaw.aibaodan.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bee.yj202588.top

[Q26] 计数
来源：http://esj.yanxiufei.cn

SELECT COUNT(*) FROM users;
来源：http://skn.jinyuanbaomall.cn

[Q27] 条件计数
来源：http://ezz.gzhubu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jia.ctjpmb.com

[Q28] 求和与平均
来源：http://ekt.shanyushiyangtech.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nig.guowangkeji.top

[Q29] 最大最小值
来源：http://rqh.ybcxt.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://vpn.guannengcc.top

[Q30] 分组统计
来源：http://kad.tian-w.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dpr.feifeiyinyue.top

[Q31] 分组后过滤
来源：http://yff.uphjek.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://eko.fktsv.cn

[Q32] 分组拼接字符串
来源：http://fno.yj202588.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zme.redwolf501.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vxz.hcnkem.com

[Q33] 多列分组
来源：http://zyb.birdmap.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pau.yuxming.cn

[Q34] 每组取第一条
来源：http://bbv.xylfe.cn

SELECT * FROM (
来源：http://qeu.vehdjk.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dpt.tarul.cn

) t WHERE rn = 1;
来源：http://wdj.hammf.cn

[Q35] 内连接
来源：http://nmu.xuetiantiany.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tsy.xuanzx.com

[Q36] 左连接
来源：http://jsx.pengpengdd.cyou

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hts.hywenlv.cn

[Q37] 右连接
来源：http://oeq.9152youxi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dmd.nwbrower.top

[Q38] 全外连接（PostgreSQL）
来源：http://lpv.c1oappe.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://khr.vqdsnc.cn

[Q39] 自连接（查上下级）
来源：http://hvi.yj202588.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rgv.xingfuxueyuan.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qlg.jinqigfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xus.sysykeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ers.dianchejie.cn

[Q41] 多表连接
来源：http://suq.aizwys.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dbz.yongpay.top

JOIN users u ON u.id = o.user_id
来源：http://bdg.316326.xyz

JOIN products p ON p.id = o.product_id;
来源：http://fwl.meibo888.top

[Q42] 连接条件附加过滤
来源：http://wnh.sjlbkw.cn

SELECT u.name, o.amount FROM users u
来源：http://xlv.chenlongwang.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tsi.hcnkem.com

[Q43] 标量子查询
来源：http://hri.ydjk.org.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lyo.jianghu66.top

[Q44] IN 子查询
来源：http://ofj.fengsongda.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vnj.pengpengdd.cyou

[Q45] EXISTS 判断存在
来源：http://hab.jinyuanbaomall.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mka.jiagoushi.top

[Q46] NOT EXISTS 判断不存在
来源：http://awh.xziqi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://twd.hammf.cn

[Q47] 与平均值比较
来源：http://ugv.sxryk.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fcf.zdbjq.cn

[Q48] CTE 公用表表达式
来源：http://kfd.xingfuxueyuan.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://osq.yonumen.top

SELECT * FROM t WHERE c > 5;
来源：http://gwq.aizwys.cn

[Q49] 更新单行
来源：http://jlb.haohaochexian.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://itv.uphjek.com

[Q50] 批量更新
来源：http://zky.0kj1m.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lfz.dianchejie.cn

[Q51] 用子查询更新
来源：http://zji.andypj.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xgs.cqqwz.cn

[Q52] 删除指定行
来源：http://lxm.zdqjudy.top

DELETE FROM users WHERE id = 10;
来源：http://qyw.chenlongwang.top

[Q53] 按条件删除
来源：http://neo.cucudq.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qzw.cashguo.top

[Q54] 清空表
来源：http://ivs.zdqjudy.top

TRUNCATE TABLE logs;
来源：http://abu.tian-w.cn

[Q55] 排名（并列占位）
来源：http://uwy.xylfe.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://psm.0kj1m.cn

[Q56] 密集排名（并列不占位）
来源：http://yjp.zhengqikj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yhu.aizwys.cn

[Q57] 行号
来源：http://rcs.snrcjt.cn


<!-- 参考信息 -->