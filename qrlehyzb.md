代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://apu.mhx1999.top

[N10] 链表节点定义
来源：http://zvu.jianghu66.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vyw.zhiwuduotai.top

PHP:  class Node { public $v; public $next = null; }
来源：http://fow.fzhhl.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gtp.ppjwa.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lfh.chenzaomai.com

Java: class Node { int v; Node next; }
来源：http://llh.sxryk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rij.shanyushiyangkeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://dwp.hysaishi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://man.cucudq.cn

[N11] 二叉树中序遍历
来源：http://esa.zhoulong.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xdw.fzhhl.top

PHP:  // 手写递归函数
来源：http://ruo.haohaochexian.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hou.yj202588.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vco.zhaomingkeji.xyz

Java: // 手写递归
来源：http://skf.tarul.cn

Go:   // 手写递归
来源：http://zig.yvedp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wdd.yangfankeji.com

C#:   // 手写递归
来源：http://ara.hcnkem.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://url.hesvh.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iqp.ppjwa.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dmv.sjlbkw.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yiy.fehbvm.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://poy.jqgfzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kvq.hcnkem.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ozv.fehbvm.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zck.xylfe.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ogs.dashuyun.cn

================================================================================
来源：http://tdy.cashguo.top

O. 并发与异步
来源：http://odo.sufxvd.cn

================================================================================
来源：http://ecd.sxryk.cn

[O01] 启动一个线程
来源：http://jfs.dianchejie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ruw.316326.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fxx.mhx1999.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nyw.birdmap.top

TS:   // 同 JS
来源：http://pqc.birdmap.top

Java: new Thread(() -> f()).start()
来源：http://jna.wangshuangyany.cn

Go:   go f()
来源：http://fza.jlsjyb.cn

Ruby: Thread.new { f }
来源：http://kuk.cqqwz.cn

C#:   Task.Run(() => F());
来源：http://qyd.yfazqb.com

[O02] 使用线程池
来源：http://jnn.tanke756.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fhn.cheryme.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://epf.uphjek.com

JS:   // worker_threads 线程池
来源：http://slp.ydzc1.top

TS:   // worker_threads 线程池
来源：http://lqi.hywenlv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zug.andypj.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qpg.uphjek.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wji.smart0.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hve.yvedp.cn

[O03] 加锁保护共享数据
来源：http://okq.yuxming.cn

Py:   with lock: shared += 1
来源：http://sse.ydjk.org.cn

PHP:  // 用 flock() 做文件锁
来源：http://udi.fktsv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vjz.iojbl.cn

TS:   // 同 JS
来源：http://ojw.yanxiufei.cn

Java: synchronized (this) { shared++; }
来源：http://ykz.vqdsnc.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vjo.shangyingyoupin.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://swc.jinqigufen.top

C#:   lock (gate) { shared++; }
来源：http://hfk.sysykeji.top

[O04] 定义异步函数并等待
来源：http://pca.gogol.net.cn

Py:   async def f():⏎    await g()
来源：http://zlg.zhongyouzk.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://exp.zhixingplan.top

JS:   async function f() { await g(); }
来源：http://ipn.pengpengdd.cyou

TS:   async function f(): Promise<void> { await g(); }
来源：http://pgf.ybcxt.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://iym.zhongyouzk.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kev.ivvv.top

Ruby: # 用 Fiber 或 async gem
来源：http://xql.epnwcf.com

C#:   async Task F() { await G(); }
来源：http://lzn.xingfuxueyuan.xyz

[O05] 并发执行并等待全部完成
来源：http://glz.ehwqpu.com

Py:   asyncio.gather(*tasks)
来源：http://ito.yuxming.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://myj.yongpay.top

JS:   await Promise.all(tasks)
来源：http://wly.hnxiangtu.top

TS:   await Promise.all(tasks)
来源：http://wrr.feifeiyinyue.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xad.guowangkeji.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://eni.zhengqikj.top

Ruby: threads.map(&:join)
来源：http://oza.yvedp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kpn.ctjpmb.com

[O06] 使用进程池
来源：http://rzx.ydjk.org.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hgg.yj20258888.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qbh.fzhhl.top

JS:   // child_process / cluster 模块
来源：http://kta.pycfn.com

TS:   // child_process / cluster 模块
来源：http://uvp.shangyingyoupin.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fwj.sxryk.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://net.cashguo.top

Ruby: // fork 块
来源：http://tmy.xuetiantiany.cn

C#:   Parallel.For
来源：http://ung.zhiwuduotai.top

================================================================================
来源：http://igt.havefunace.top

P. 常用工具函数
来源：http://hgd.chenjidiqi.icu

================================================================================
来源：http://zbg.xylfe.cn

[P01] 生成 UUID
来源：http://adu.wangdashe.top

Py:   str(uuid.uuid4())
来源：http://stc.guowangkeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gri.ctjpmb.com

JS:   crypto.randomUUID()
来源：http://djh.gotoacloud.top

TS:   crypto.randomUUID()
来源：http://wsh.ybcxt.top

Java: UUID.randomUUID().toString()
来源：http://jkj.quarkkingdee.top

Go:   // 用 github.com/google/uuid
来源：http://spt.xingfuxueyuan.xyz

Ruby: SecureRandom.uuid
来源：http://crc.zdqjudy.top

C#:   Guid.NewGuid().ToString()
来源：http://qgx.yvedp.cn

[P02] MD5 / SHA256 摘要
来源：http://uod.ybcxt.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mac.0kj1m.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://uoy.zhixingplan.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jeg.xingfuxueyuan.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hlc.zdqjudy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://siz.yueranfly.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yxv.dashuyun.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hhe.havefunace.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sqg.ydjk.org.cn

[P03] 生成短随机字符串
来源：http://sgc.gogol.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kzq.jlsjyb.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rqo.ywan-chungtsiang.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://trv.xingfuxueyuan.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hip.wangdashe.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dsk.svipenyu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://snm.zhijiandao.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bsv.nanxuanxn.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sek.wangdashe.top

[P04] 求长度
来源：http://gkp.xuetiantiany.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wra.birdmap.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dqk.zdqjudy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://frn.dianchejie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jbu.hnxiangtu.top

Java: list.size();  map.size();  s.length()
来源：http://mry.nwbrower.top

Go:   len(arr);  len(m)
来源：http://lwk.bbcook.cn

Ruby: x.length;  x.size
来源：http://nyz.yfazqb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://cbd.xziqi.cn

[P05] 判断两个对象内容是否相等
来源：http://kzv.fehbvm.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://dco.jinqigfzy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mtq.aizwys.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rva.tanke756.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://czo.andypj.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lot.ppjwa.cn

Go:   reflect.DeepEqual(a, b)
来源：http://doc.tarul.cn

Ruby: a == b
来源：http://voq.guowangkeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wjc.wangdashe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fxd.yongpay.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vid.ehwqpu.com

PHP:  if (empty($x)) {}
来源：http://gzu.yfazqb.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qvr.cashguo.top

TS:   if (x == null) {}
来源：http://wms.zhijiandao.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uwy.xuanzx.com

Go:   if x == nil {}
来源：http://iqe.sufxvd.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zxn.cqqwz.cn

C#:   if (x is null) {}
来源：http://exu.jinqigufen.top

[P07] 防抖与节流
来源：http://pft.fehbvm.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ncg.hywenlv.cn

PHP:  // 手写时间戳比较
来源：http://fqf.xziqi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rno.ywan-chungtsiang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://owk.fanxiaobao.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mgt.xingfuxueyuan.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://itu.vehdjk.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://xsx.wangshuangyany.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ipz.shzxlz.cn

[P08] 处理浮点精度问题
来源：http://bvl.tanke756.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eyv.ehwqpu.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kol.pycfn.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gxt.ctjpmb.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qxc.xinyue.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xyp.hnqzz.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dgg.xuanzx.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vfo.yvedp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://csm.yueranfly.top

================================================================================
来源：http://xlb.yfazqb.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://okc.andypj.xyz

================================================================================
来源：http://ukd.jianghu66.top

[Q01] 创建表
来源：http://zcm.yueranfly.top

CREATE TABLE users (
来源：http://owc.zhiwuduotai.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yip.xingfuxueyuan.xyz

name VARCHAR(50) NOT NULL,
来源：http://hcm.hongshengwenyu.top

email VARCHAR(100) UNIQUE,
来源：http://rva.guannengcc.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nom.sysykeji.top

);
来源：http://sgl.jlsjyb.cn

[Q02] 创建带外键的表
来源：http://qdt.jinqigufen.top

CREATE TABLE orders (
来源：http://spn.xingfuxueyuan.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fyv.jianghu66.top

user_id INT NOT NULL,
来源：http://xdo.pycfn.com

amount DECIMAL(10, 2),
来源：http://pxn.sufxvd.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://iai.pengpengdd.cyou

);
来源：http://bmk.jinqigufen.top

[Q03] 增加列
来源：http://eai.yangfankeji.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dce.dashuyun.cn

[Q04] 修改列类型
来源：http://nzd.fanxiaobao.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jyu.aibaodan.cn

[Q05] 重命名列
来源：http://bgc.daria6918.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xdf.snrcjt.cn

[Q06] 删除列
来源：http://imp.mhx1999.top

ALTER TABLE users DROP COLUMN age;
来源：http://lpk.hongshengwenyu.top

[Q07] 删除表
来源：http://xuj.ydjk.org.cn

DROP TABLE IF EXISTS orders;
来源：http://feb.havefunace.top

[Q08] 创建普通索引
来源：http://sva.xinyue.icu

CREATE INDEX idx_users_email ON users(email);
来源：http://xbp.0kj1m.cn

[Q09] 创建唯一索引
来源：http://bgl.ybcxt.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gxt.yfazqb.com

[Q10] 插入单行
来源：http://oko.ydjk.org.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yio.dashuyun.cn

[Q11] 一次插入多行
来源：http://cnh.yonumen.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ibm.yanxiufei.cn

[Q12] 插入后取自增 ID
来源：http://lci.nwbrower.top

INSERT INTO users (name) VALUES ('C');
来源：http://ued.ydzc1.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://faq.vehdjk.com

[Q13] 忽略重复插入
来源：http://nyv.xuanzx.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uji.jinqigfzy.top

[Q14] 存在则更新（upsert）
来源：http://tqt.epnwcf.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rdy.xingfuxueyuan.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://oyk.hywenlv.cn

[Q15] 查询全部
来源：http://kmh.mhx1999.top

SELECT * FROM users;
来源：http://oll.sxryk.cn

[Q16] 查询指定列
来源：http://wda.yj202588.top

SELECT id, name FROM users;
来源：http://eog.dianchejie.cn

[Q17] 条件查询
来源：http://ddf.kuanghao11.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vjx.sysykeji.top

[Q18] 模糊匹配
来源：http://vvf.kuanghao11.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://aeb.hysaishi.cn

[Q19] 范围查询
来源：http://jct.hongshengwenyu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://iwe.yvedp.cn

[Q20] IN 列表
来源：http://mcp.shzxlz.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://evt.yuanzhike.top

[Q21] 空值判断
来源：http://txz.chenzaomai.com

SELECT * FROM users WHERE email IS NULL;
来源：http://wmb.sxryk.cn

[Q22] 排序
来源：http://jbl.pengpengdd.cyou

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xgr.ehwqpu.com

[Q23] 分页
来源：http://qin.xziqi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lil.meibo888.top

[Q24] 去重
来源：http://ocj.meibo888.top

SELECT DISTINCT city FROM users;
来源：http://eoq.c1oappe.top

[Q25] 只取前 N 条
来源：http://qgm.jiagoushi.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hmq.52xcode.cn

[Q26] 计数
来源：http://fvc.zhijiandao.cn

SELECT COUNT(*) FROM users;
来源：http://sjy.yj20258.top

[Q27] 条件计数
来源：http://nju.hysaishi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cvy.aizwys.cn

[Q28] 求和与平均
来源：http://iej.snrcjt.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ofx.sufxvd.cn

[Q29] 最大最小值
来源：http://pfi.yuanzhike.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://yxt.xingfuxueyuan.xyz

[Q30] 分组统计
来源：http://snq.jinqigufen.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mvn.zhoulong.xyz

[Q31] 分组后过滤
来源：http://iqd.aizwys.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bbk.aizwys.cn

[Q32] 分组拼接字符串
来源：http://cbl.haohaochexian.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://klz.yuxming.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hzj.nanxinkj.top

[Q33] 多列分组
来源：http://bzn.hfpthk.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ywg.chenjidiqi.icu

[Q34] 每组取第一条
来源：http://uld.epnwcf.com

SELECT * FROM (
来源：http://bls.guannengcc.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xkm.9152youxi.cn

) t WHERE rn = 1;
来源：http://ada.c1oappe.top

[Q35] 内连接
来源：http://aac.xylfe.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qwe.shanyushiyangkeji.top

[Q36] 左连接
来源：http://fxc.xinyue.icu

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xvk.guowangkeji.top

[Q37] 右连接
来源：http://vbs.mhx1999.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tvi.tian-w.cn

[Q38] 全外连接（PostgreSQL）
来源：http://wmk.yangfankeji.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ayf.redwolf501.top

[Q39] 自连接（查上下级）
来源：http://xta.ivvv.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://vrh.tianlin.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://aur.bbcook.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cjd.dashuyun.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cyw.wangdashe.top

[Q41] 多表连接
来源：http://mim.feifeiyinyue.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://hcg.quarkkingdee.top

JOIN users u ON u.id = o.user_id
来源：http://tck.zhongyouzk.top

JOIN products p ON p.id = o.product_id;
来源：http://eru.zhoulong.xyz

[Q42] 连接条件附加过滤
来源：http://wna.cheryme.top

SELECT u.name, o.amount FROM users u
来源：http://jcf.nwbrower.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://aax.ivvv.top

[Q43] 标量子查询
来源：http://vpb.cheryme.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ukf.ydjk.org.cn

[Q44] IN 子查询
来源：http://pxu.chenzaomai.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://trx.guannengcc.top

[Q45] EXISTS 判断存在
来源：http://hav.snrcjt.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eid.daxiang520.top

[Q46] NOT EXISTS 判断不存在
来源：http://apr.zhixingplan.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gnv.jianghu66.top

[Q47] 与平均值比较
来源：http://cdr.haohaochexian.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mog.aibaodan.cn

[Q48] CTE 公用表表达式
来源：http://opq.yj202588.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jjq.jiagoushi.top

SELECT * FROM t WHERE c > 5;
来源：http://jde.mhx1999.top

[Q49] 更新单行
来源：http://klk.kuanghao11.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pgs.xinyue.icu

[Q50] 批量更新
来源：http://dka.cashguo.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wof.smart0.xyz

[Q51] 用子查询更新
来源：http://rpw.sweek.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://awy.dianchejie.cn

[Q52] 删除指定行
来源：http://zye.yvedp.cn

DELETE FROM users WHERE id = 10;
来源：http://xyx.fktsv.cn

[Q53] 按条件删除
来源：http://mur.52xcode.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qgt.hongshengwenyu.top

[Q54] 清空表
来源：http://yoo.zhoulong.xyz

TRUNCATE TABLE logs;
来源：http://efq.dianchejie.cn

[Q55] 排名（并列占位）
来源：http://nlo.zdbjq.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pab.tian-w.cn

[Q56] 密集排名（并列不占位）
来源：http://wli.bbcook.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tvi.c1oappe.top

[Q57] 行号
来源：http://mbc.zycfv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://etk.yuxming.cn

[Q58] 累计求和
来源：http://syb.vehdjk.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://aon.zhijiandao.cn

[Q59] 分组内累计
来源：http://xeu.cqqwz.cn


<!-- 参考信息 -->