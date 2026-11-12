代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ocf.sweek.top

[N10] 链表节点定义
来源：http://vfa.jinqigufen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sih.tarul.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://miy.yuanzhike.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qnj.ctjpmb.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sea.dashuyun.cn

Java: class Node { int v; Node next; }
来源：http://tox.quarkkingdee.top

Go:   type Node struct { V int; Next *Node }
来源：http://eue.vehdjk.com

Ruby: Node = Struct.new(:v, :next)
来源：http://maf.fktsv.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xxs.zdbjq.cn

[N11] 二叉树中序遍历
来源：http://nxo.gogol.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://iqz.gotoacloud.top

PHP:  // 手写递归函数
来源：http://zae.hysaishi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yzn.hnxiangtu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tks.nanxuanxn.top

Java: // 手写递归
来源：http://eig.yangfankeji.com

Go:   // 手写递归
来源：http://mts.yuxming.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vas.snrcjt.cn

C#:   // 手写递归
来源：http://izv.wangshuangyany.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oel.gzhubu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ufm.sysykeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xmo.cheryme.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://puf.vqdsnc.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mcp.daxiang520.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dvm.bbcook.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vmj.hammf.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pnm.iojbl.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ptw.yvedp.cn

================================================================================
来源：http://bzo.epnwcf.com

O. 并发与异步
来源：http://nes.sufxvd.cn

================================================================================
来源：http://hzs.shzxlz.cn

[O01] 启动一个线程
来源：http://ktt.xuetiantiany.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dxg.cashguo.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://utw.yueranfly.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rci.hnqzz.top

TS:   // 同 JS
来源：http://xvd.fehbvm.com

Java: new Thread(() -> f()).start()
来源：http://fzj.tarul.cn

Go:   go f()
来源：http://uyq.jinqigufen.top

Ruby: Thread.new { f }
来源：http://bah.guowangkeji.top

C#:   Task.Run(() => F());
来源：http://eoi.hammf.cn

[O02] 使用线程池
来源：http://gie.fanxiaobao.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zdg.sufxvd.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hmi.shuidangran.top

JS:   // worker_threads 线程池
来源：http://hhj.0kj1m.cn

TS:   // worker_threads 线程池
来源：http://mdg.jiagoushi.top

Java: Executors.newFixedThreadPool(4)
来源：http://oyj.shangyingyoupin.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ovw.dashuyun.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lfo.chenlongwang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://phz.ydzc1.top

[O03] 加锁保护共享数据
来源：http://wbk.vqdsnc.cn

Py:   with lock: shared += 1
来源：http://ikq.ivvv.top

PHP:  // 用 flock() 做文件锁
来源：http://oad.cheryme.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://liw.9152youxi.cn

TS:   // 同 JS
来源：http://tbo.jiagoushi.top

Java: synchronized (this) { shared++; }
来源：http://xez.zhongyouzk.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mcm.haohaochexian.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://juz.gotoacloud.top

C#:   lock (gate) { shared++; }
来源：http://lho.ywan-chungtsiang.top

[O04] 定义异步函数并等待
来源：http://fpb.316326.xyz

Py:   async def f():⏎    await g()
来源：http://btq.tarul.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dme.bjfxy.top

JS:   async function f() { await g(); }
来源：http://mwt.52xcode.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gpq.hfpthk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cvv.fengsongda.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mef.cashguo.top

Ruby: # 用 Fiber 或 async gem
来源：http://syr.mhx1999.top

C#:   async Task F() { await G(); }
来源：http://nom.jinghuilouyu.cn

[O05] 并发执行并等待全部完成
来源：http://sii.xingfuxueyuan.xyz

Py:   asyncio.gather(*tasks)
来源：http://oej.andypj.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ijx.sysykeji.top

JS:   await Promise.all(tasks)
来源：http://tyn.daria6918.cn

TS:   await Promise.all(tasks)
来源：http://dyo.redwolf501.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nog.bbcook.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bvd.fanxiaobao.xyz

Ruby: threads.map(&:join)
来源：http://xcc.nanxuanxn.top

C#:   await Task.WhenAll(t1, t2)
来源：http://zlp.quarkkingdee.top

[O06] 使用进程池
来源：http://yaz.hammf.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ujq.ehwqpu.com

PHP:  // pcntl_fork 或多进程队列
来源：http://aov.tanke756.top

JS:   // child_process / cluster 模块
来源：http://iwe.yuanzhike.top

TS:   // child_process / cluster 模块
来源：http://iyo.yonumen.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://trc.zhongyouzk.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fff.cdnleiting.top

Ruby: // fork 块
来源：http://hyt.ivvv.top

C#:   Parallel.For
来源：http://sqk.hywenlv.cn

================================================================================
来源：http://twp.yj20258888.top

P. 常用工具函数
来源：http://pjp.sxryk.cn

================================================================================
来源：http://waf.iojbl.cn

[P01] 生成 UUID
来源：http://iss.xylfe.cn

Py:   str(uuid.uuid4())
来源：http://mpu.xinyue.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nls.jqgfzy.top

JS:   crypto.randomUUID()
来源：http://zlc.uphjek.com

TS:   crypto.randomUUID()
来源：http://lot.smart0.xyz

Java: UUID.randomUUID().toString()
来源：http://otk.fzhhl.top

Go:   // 用 github.com/google/uuid
来源：http://ver.jinqigfzy.top

Ruby: SecureRandom.uuid
来源：http://onc.redwolf501.top

C#:   Guid.NewGuid().ToString()
来源：http://tvt.jqgufenzy.top

[P02] MD5 / SHA256 摘要
来源：http://bnl.quarkkingdee.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zue.tanke756.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ywk.pengpengdd.cyou

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bxt.nanxinkj.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gkv.zhixingplan.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hrs.zycfv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://alz.zdqjudy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wxa.yonumen.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bqc.jlsjyb.cn

[P03] 生成短随机字符串
来源：http://wap.pycfn.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nzo.quarkkingdee.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pjv.hesvh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ftc.kuanghao11.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://scg.cucudq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qso.aibaodan.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://crf.zhoulong.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://skn.xingfuxueyuan.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fks.hammf.cn

[P04] 求长度
来源：http://yvc.fktsv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://joh.hesvh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eie.tian-w.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ltv.yj20258888.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://shj.chenlongwang.top

Java: list.size();  map.size();  s.length()
来源：http://hsl.vqdsnc.cn

Go:   len(arr);  len(m)
来源：http://olh.fengsongda.top

Ruby: x.length;  x.size
来源：http://isz.9152youxi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://sgy.cashguo.top

[P05] 判断两个对象内容是否相等
来源：http://yyh.fktsv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ivo.haohaochexian.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ntz.shanyushiyangtech.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lll.dianchejie.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ktv.pycfn.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cid.zhoulong.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://fxd.cdnleiting.top

Ruby: a == b
来源：http://bjw.feifeiyinyue.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hwh.fktsv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://epo.fehbvm.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zln.zhaomingkeji.xyz

PHP:  if (empty($x)) {}
来源：http://shv.cdnleiting.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cwv.hywenlv.cn

TS:   if (x == null) {}
来源：http://ify.kuanghao11.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://oev.meibo888.top

Go:   if x == nil {}
来源：http://lsb.zhoulong.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uio.hfpthk.cn

C#:   if (x is null) {}
来源：http://arr.xingfuxueyuan.xyz

[P07] 防抖与节流
来源：http://wgh.xylfe.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blx.bbcook.cn

PHP:  // 手写时间戳比较
来源：http://flt.0kj1m.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rej.gotoacloud.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ehq.pengpengdd.cyou

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ofh.zhaomingkeji.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ydc.ydzc1.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://jpb.nwbrower.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mmx.hesvh.cn

[P08] 处理浮点精度问题
来源：http://pws.yj202588.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://odm.fanxiaobao.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dnx.yj202588.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://otu.redwolf501.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wfi.havefunace.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pqf.yuxming.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sny.zhiwuduotai.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://swx.zhiwuduotai.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ovt.yongpay.top

================================================================================
来源：http://lzz.52xcode.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hat.xziqi.cn

================================================================================
来源：http://pxa.yfazqb.com

[Q01] 创建表
来源：http://gtz.wangdashe.top

CREATE TABLE users (
来源：http://evy.xuetiantiany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nvk.yonumen.top

name VARCHAR(50) NOT NULL,
来源：http://oey.mhx1999.top

email VARCHAR(100) UNIQUE,
来源：http://ocj.ywan-chungtsiang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nah.zhixingplan.top

);
来源：http://qup.tian-w.cn

[Q02] 创建带外键的表
来源：http://wqm.ctjpmb.com

CREATE TABLE orders (
来源：http://rwn.nanxinkj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://njn.cashguo.top

user_id INT NOT NULL,
来源：http://hvw.pycfn.com

amount DECIMAL(10, 2),
来源：http://tbd.xinyue.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://led.tianlin.xyz

);
来源：http://tov.jqgufenzy.top

[Q03] 增加列
来源：http://gls.svipenyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kff.jinqigufen.top

[Q04] 修改列类型
来源：http://roq.jinqigufen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bzn.bjfxy.top

[Q05] 重命名列
来源：http://dxg.ydzc1.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mjc.xuanzx.com

[Q06] 删除列
来源：http://pqb.zycfv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pyv.daria6918.cn

[Q07] 删除表
来源：http://lue.jiagoushi.top

DROP TABLE IF EXISTS orders;
来源：http://ejw.ctjpmb.com

[Q08] 创建普通索引
来源：http://jjs.shuidangran.top

CREATE INDEX idx_users_email ON users(email);
来源：http://yne.cucudq.cn

[Q09] 创建唯一索引
来源：http://wsh.vqdsnc.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wau.birdmap.top

[Q10] 插入单行
来源：http://eam.c1oappe.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vga.xziqi.cn

[Q11] 一次插入多行
来源：http://azy.hcnkem.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bqy.jinqigufen.top

[Q12] 插入后取自增 ID
来源：http://rhx.zhiwuduotai.top

INSERT INTO users (name) VALUES ('C');
来源：http://lgm.sjlbkw.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hnq.9152youxi.cn

[Q13] 忽略重复插入
来源：http://xxm.52xcode.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uvr.jinyuanbaomall.cn

[Q14] 存在则更新（upsert）
来源：http://gbi.hesvh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zjy.tanke756.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jqz.jyoumei.cn

[Q15] 查询全部
来源：http://dpx.nanxinkj.top

SELECT * FROM users;
来源：http://yca.ehwqpu.com

[Q16] 查询指定列
来源：http://rlz.shzxlz.cn

SELECT id, name FROM users;
来源：http://esb.fktsv.cn

[Q17] 条件查询
来源：http://rtt.wangshuangyany.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zkx.yuanzhike.top

[Q18] 模糊匹配
来源：http://qni.hnqzz.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ccr.c1oappe.top

[Q19] 范围查询
来源：http://qml.zhiwuduotai.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wpe.dashuyun.cn

[Q20] IN 列表
来源：http://kfa.fanxiaobao.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wqi.shzxlz.cn

[Q21] 空值判断
来源：http://ojy.tian-w.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://egv.daria6918.cn

[Q22] 排序
来源：http://nkp.cashguo.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jgb.cucudq.cn

[Q23] 分页
来源：http://kvt.birdmap.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vgy.xinyue.icu

[Q24] 去重
来源：http://lpf.fktsv.cn

SELECT DISTINCT city FROM users;
来源：http://sdp.dianchejie.cn

[Q25] 只取前 N 条
来源：http://wjp.quarkkingdee.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gis.fengsongda.top

[Q26] 计数
来源：http://tct.cucudq.cn

SELECT COUNT(*) FROM users;
来源：http://ski.cqqwz.cn

[Q27] 条件计数
来源：http://rug.9152youxi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qyj.guowangkeji.top

[Q28] 求和与平均
来源：http://gjr.zhaomingkeji.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dwz.yongpay.top

[Q29] 最大最小值
来源：http://vjr.ydjk.org.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ygw.zhengqikj.top

[Q30] 分组统计
来源：http://lyc.yangfankeji.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bxq.316326.xyz

[Q31] 分组后过滤
来源：http://whg.tianlin.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qmm.chenjidiqi.icu

[Q32] 分组拼接字符串
来源：http://mmy.yj202588.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xwi.jlsjyb.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rhe.snrcjt.cn

[Q33] 多列分组
来源：http://twh.snrcjt.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://znr.hesvh.cn

[Q34] 每组取第一条
来源：http://yxk.ivvv.top

SELECT * FROM (
来源：http://osa.fktsv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ssz.andypj.xyz

) t WHERE rn = 1;
来源：http://rit.mhx1999.top

[Q35] 内连接
来源：http://ese.jqgfzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wqw.c1oappe.top

[Q36] 左连接
来源：http://vcb.cqqwz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wju.zdbjq.cn

[Q37] 右连接
来源：http://hqd.gotoacloud.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ezf.hywenlv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://crv.zhiwuduotai.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fyc.wangdashe.top

[Q39] 自连接（查上下级）
来源：http://aoc.yuanzhike.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://lpj.feifeiyinyue.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ras.zdbjq.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mwq.ehwqpu.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bpf.xziqi.cn

[Q41] 多表连接
来源：http://oyl.xuetiantiany.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xrg.yj20258.top

JOIN users u ON u.id = o.user_id
来源：http://rlr.cqqwz.cn

JOIN products p ON p.id = o.product_id;
来源：http://luu.feifeiyinyue.top

[Q42] 连接条件附加过滤
来源：http://rqd.svipenyu.cn

SELECT u.name, o.amount FROM users u
来源：http://vco.jlsjyb.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lsc.ywan-chungtsiang.top

[Q43] 标量子查询
来源：http://ibj.ppjwa.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tkg.chenzaomai.com

[Q44] IN 子查询
来源：http://ikt.zhoulong.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jrt.shanyushiyangkeji.top

[Q45] EXISTS 判断存在
来源：http://soe.gaohongyu789.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xkl.xinyue.icu

[Q46] NOT EXISTS 判断不存在
来源：http://ysu.sweek.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bcj.yuxming.cn

[Q47] 与平均值比较
来源：http://tra.jinqigufen.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yvv.ydzc1.top

[Q48] CTE 公用表表达式
来源：http://eyx.tanke756.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sdx.zdqjudy.top

SELECT * FROM t WHERE c > 5;
来源：http://nbt.xingfuxueyuan.xyz

[Q49] 更新单行
来源：http://ucl.fzhhl.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fnp.xziqi.cn

[Q50] 批量更新
来源：http://mfd.jqgufenzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yek.yfazqb.com

[Q51] 用子查询更新
来源：http://bbr.yfazqb.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dmj.xinyue.icu

[Q52] 删除指定行
来源：http://scs.zdqjudy.top

DELETE FROM users WHERE id = 10;
来源：http://rcg.zhongyouzk.top

[Q53] 按条件删除
来源：http://tyf.cdnleiting.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://avd.nanxuanxn.top

[Q54] 清空表
来源：http://kqx.hcnkem.com

TRUNCATE TABLE logs;
来源：http://wzk.hcnkem.com

[Q55] 排名（并列占位）
来源：http://yru.zhongyouzk.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://iur.cheryme.top

[Q56] 密集排名（并列不占位）
来源：http://vlp.cashguo.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rad.daxiang520.top

[Q57] 行号
来源：http://dko.9152youxi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mvt.zdqjudy.top

[Q58] 累计求和
来源：http://zqs.hongshengwenyu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qbc.iojbl.cn

[Q59] 分组内累计
来源：http://vxh.birdmap.top


<!-- 参考信息 -->