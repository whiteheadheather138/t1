代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zhz.9152youxi.cn

[N10] 链表节点定义
来源：http://lxg.ydzc1.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nfb.jianghu66.top

PHP:  class Node { public $v; public $next = null; }
来源：http://psp.yuanzhike.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://quk.nanxuanxn.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ufe.316326.xyz

Java: class Node { int v; Node next; }
来源：http://ius.fengsongda.top

Go:   type Node struct { V int; Next *Node }
来源：http://znw.yvedp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kxw.hfpthk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fmb.nwbrower.top

[N11] 二叉树中序遍历
来源：http://coo.ybcxt.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vbc.zhixingplan.top

PHP:  // 手写递归函数
来源：http://zdh.haohaochexian.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ycn.tanke756.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kiy.wangdashe.top

Java: // 手写递归
来源：http://sgx.wangshuangyany.cn

Go:   // 手写递归
来源：http://koa.sufxvd.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ngf.yj20258.top

C#:   // 手写递归
来源：http://dhc.9152youxi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oji.shanyushiyangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ljj.sysykeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://azi.cdnleiting.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nhx.gotoacloud.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://diu.hcnkem.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yob.hywenlv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xhs.mhx1999.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://oou.chenlongwang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vgh.zhengqikj.top

================================================================================
来源：http://mmi.havefunace.top

O. 并发与异步
来源：http://ify.yangfankeji.com

================================================================================
来源：http://zmy.xingfuxueyuan.xyz

[O01] 启动一个线程
来源：http://trz.sysykeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pkc.vqdsnc.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://chy.nanxuanxn.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://miq.xingfuxueyuan.xyz

TS:   // 同 JS
来源：http://tyi.ydzc1.top

Java: new Thread(() -> f()).start()
来源：http://bcw.gzhubu.top

Go:   go f()
来源：http://xqw.zdbjq.cn

Ruby: Thread.new { f }
来源：http://iue.xingfuxueyuan.xyz

C#:   Task.Run(() => F());
来源：http://ojb.ydzc1.top

[O02] 使用线程池
来源：http://yid.havefunace.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qvx.yuanzhike.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jhs.yuanzhike.top

JS:   // worker_threads 线程池
来源：http://ryx.daria6918.cn

TS:   // worker_threads 线程池
来源：http://zdz.c1oappe.top

Java: Executors.newFixedThreadPool(4)
来源：http://nyv.wangdashe.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xkx.zhaomingkeji.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ljj.zycfv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tzn.bbcook.cn

[O03] 加锁保护共享数据
来源：http://xkl.yj202588.top

Py:   with lock: shared += 1
来源：http://gvo.tian-w.cn

PHP:  // 用 flock() 做文件锁
来源：http://pds.daria6918.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ymw.jinyuanbaomall.cn

TS:   // 同 JS
来源：http://yov.ywan-chungtsiang.top

Java: synchronized (this) { shared++; }
来源：http://zss.jinghuilouyu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fbx.pycfn.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://hdo.daxiang520.top

C#:   lock (gate) { shared++; }
来源：http://ayi.cashguo.top

[O04] 定义异步函数并等待
来源：http://doe.redwolf501.top

Py:   async def f():⏎    await g()
来源：http://kfj.hywenlv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://khf.hysaishi.cn

JS:   async function f() { await g(); }
来源：http://jzf.yueranfly.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://pbc.0kj1m.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wip.xylfe.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://saj.52xcode.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kgm.smart0.xyz

C#:   async Task F() { await G(); }
来源：http://bhg.jinghuilouyu.cn

[O05] 并发执行并等待全部完成
来源：http://xby.nanxuanxn.top

Py:   asyncio.gather(*tasks)
来源：http://bfm.yj202588.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://smq.cqqwz.cn

JS:   await Promise.all(tasks)
来源：http://ixq.gotoacloud.top

TS:   await Promise.all(tasks)
来源：http://vud.jinghuilouyu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://svu.fktsv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://acy.hnqzz.top

Ruby: threads.map(&:join)
来源：http://rim.chenjidiqi.icu

C#:   await Task.WhenAll(t1, t2)
来源：http://kwb.smart0.xyz

[O06] 使用进程池
来源：http://uzv.jyoumei.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uqc.hammf.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zgx.cdnleiting.top

JS:   // child_process / cluster 模块
来源：http://qtw.yangfankeji.com

TS:   // child_process / cluster 模块
来源：http://tjz.hfpthk.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nkr.daxiang520.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://swu.fanxiaobao.xyz

Ruby: // fork 块
来源：http://ecq.vehdjk.com

C#:   Parallel.For
来源：http://pyw.ivvv.top

================================================================================
来源：http://xye.fanxiaobao.xyz

P. 常用工具函数
来源：http://gup.xinyue.icu

================================================================================
来源：http://oim.zhijiandao.cn

[P01] 生成 UUID
来源：http://bew.gzhubu.top

Py:   str(uuid.uuid4())
来源：http://lsz.tanke756.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ykr.svipenyu.cn

JS:   crypto.randomUUID()
来源：http://bnv.yuanzhike.top

TS:   crypto.randomUUID()
来源：http://bue.yonumen.top

Java: UUID.randomUUID().toString()
来源：http://mkq.vehdjk.com

Go:   // 用 github.com/google/uuid
来源：http://lal.zhaomingkeji.xyz

Ruby: SecureRandom.uuid
来源：http://kgj.jiagoushi.top

C#:   Guid.NewGuid().ToString()
来源：http://nml.tian-w.cn

[P02] MD5 / SHA256 摘要
来源：http://lhm.sjlbkw.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oba.yvedp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://flj.yanxiufei.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pje.shuidangran.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://smz.fzhhl.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tir.jianghu66.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ayk.jqgufenzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xsq.nanxinkj.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cir.daria6918.cn

[P03] 生成短随机字符串
来源：http://zyx.uphjek.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rho.haohaochexian.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wxu.316326.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qom.hcnkem.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xnf.feifeiyinyue.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vzi.yj20258888.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gzt.zdbjq.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ykv.fktsv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fxp.cdnleiting.top

[P04] 求长度
来源：http://skb.hcnkem.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ycv.pycfn.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xnk.meibo888.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ebb.haohaochexian.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fom.svipenyu.cn

Java: list.size();  map.size();  s.length()
来源：http://gys.fengsongda.top

Go:   len(arr);  len(m)
来源：http://ijp.zhiwuduotai.top

Ruby: x.length;  x.size
来源：http://hlr.xinyue.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://lze.daxiang520.top

[P05] 判断两个对象内容是否相等
来源：http://ess.yuanzhike.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://zef.yvedp.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qxx.yuanzhike.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zgi.yonumen.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zwj.feifeiyinyue.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xqa.cqqwz.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wtf.ydzc1.top

Ruby: a == b
来源：http://rpt.fengsongda.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://byf.sufxvd.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jiw.mhx1999.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ddy.haohaochexian.top

PHP:  if (empty($x)) {}
来源：http://cgr.ydjk.org.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ekd.dianchejie.cn

TS:   if (x == null) {}
来源：http://ncx.havefunace.top

Java: if (x == null || x.isEmpty()) {}
来源：http://vwq.hongshengwenyu.top

Go:   if x == nil {}
来源：http://nla.nanxinkj.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kwv.dashuyun.cn

C#:   if (x is null) {}
来源：http://hrx.xinyue.icu

[P07] 防抖与节流
来源：http://equ.hysaishi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rlx.shanyushiyangkeji.top

PHP:  // 手写时间戳比较
来源：http://vvz.yuanzhike.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ays.svipenyu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tud.svipenyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jnd.pycfn.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hhn.fzhhl.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://yfl.hammf.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://obu.wangdashe.top

[P08] 处理浮点精度问题
来源：http://svj.yueranfly.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mpr.chenjidiqi.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sax.shanyushiyangtech.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qnb.sysykeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xqx.nanxinkj.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tpa.shuidangran.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lke.zhengqikj.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://crb.jqgfzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://eul.yvedp.cn

================================================================================
来源：http://cpj.dashuyun.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bgq.cqqwz.cn

================================================================================
来源：http://pmr.jlsjyb.cn

[Q01] 创建表
来源：http://kqd.zdqjudy.top

CREATE TABLE users (
来源：http://pgk.jlsjyb.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yqr.hnxiangtu.top

name VARCHAR(50) NOT NULL,
来源：http://vgs.shanyushiyangtech.top

email VARCHAR(100) UNIQUE,
来源：http://pun.dianchejie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://chk.shanyushiyangtech.top

);
来源：http://iii.pengpengdd.cyou

[Q02] 创建带外键的表
来源：http://nfu.tarul.cn

CREATE TABLE orders (
来源：http://ree.ydjk.org.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uhi.hnxiangtu.top

user_id INT NOT NULL,
来源：http://zkx.wangshuangyany.cn

amount DECIMAL(10, 2),
来源：http://jof.zycfv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ugg.cheryme.top

);
来源：http://mfn.gzhubu.top

[Q03] 增加列
来源：http://etx.meibo888.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zzi.kuanghao11.cn

[Q04] 修改列类型
来源：http://kpp.ivvv.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kwh.jqgfzy.top

[Q05] 重命名列
来源：http://wql.jinqigfzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xkg.ppjwa.cn

[Q06] 删除列
来源：http://mwa.zhoulong.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://ltv.jinyuanbaomall.cn

[Q07] 删除表
来源：http://dhq.zhongyouzk.top

DROP TABLE IF EXISTS orders;
来源：http://vav.sxryk.cn

[Q08] 创建普通索引
来源：http://fxr.xuetiantiany.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ote.aizwys.cn

[Q09] 创建唯一索引
来源：http://ybx.hnxiangtu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nja.fengsongda.top

[Q10] 插入单行
来源：http://kqw.ctjpmb.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kwa.hammf.cn

[Q11] 一次插入多行
来源：http://gbn.cqqwz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xhm.snrcjt.cn

[Q12] 插入后取自增 ID
来源：http://ugh.fengsongda.top

INSERT INTO users (name) VALUES ('C');
来源：http://rsf.yanxiufei.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nrr.9152youxi.cn

[Q13] 忽略重复插入
来源：http://gvx.jinqigufen.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://eyn.dianchejie.cn

[Q14] 存在则更新（upsert）
来源：http://srz.jianghu66.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vbu.cdnleiting.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rzi.hesvh.cn

[Q15] 查询全部
来源：http://rru.cashguo.top

SELECT * FROM users;
来源：http://tag.jinqigfzy.top

[Q16] 查询指定列
来源：http://ubr.yuanzhike.top

SELECT id, name FROM users;
来源：http://woh.svipenyu.cn

[Q17] 条件查询
来源：http://aji.dashuyun.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gma.gzhubu.top

[Q18] 模糊匹配
来源：http://gvy.ydjk.org.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ame.52xcode.cn

[Q19] 范围查询
来源：http://ysu.gogol.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ned.mhx1999.top

[Q20] IN 列表
来源：http://qws.hywenlv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hoa.guowangkeji.top

[Q21] 空值判断
来源：http://rah.316326.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://qgc.yfazqb.com

[Q22] 排序
来源：http://uay.ywan-chungtsiang.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qbp.zhoulong.xyz

[Q23] 分页
来源：http://sep.nanxinkj.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qyx.svipenyu.cn

[Q24] 去重
来源：http://mva.tian-w.cn

SELECT DISTINCT city FROM users;
来源：http://cro.feifeiyinyue.top

[Q25] 只取前 N 条
来源：http://wdb.cashguo.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ipo.andypj.xyz

[Q26] 计数
来源：http://xyz.pengpengdd.cyou

SELECT COUNT(*) FROM users;
来源：http://nug.andypj.xyz

[Q27] 条件计数
来源：http://hjx.fzhhl.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://din.tianlin.xyz

[Q28] 求和与平均
来源：http://yth.ydzc1.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zqx.zhixingplan.top

[Q29] 最大最小值
来源：http://vwd.jinyuanbaomall.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://unp.nanxinkj.top

[Q30] 分组统计
来源：http://wre.chenjidiqi.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sur.fanxiaobao.xyz

[Q31] 分组后过滤
来源：http://xqj.hnqzz.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ejh.fehbvm.com

[Q32] 分组拼接字符串
来源：http://oqh.zdqjudy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qjo.epnwcf.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tex.shzxlz.cn

[Q33] 多列分组
来源：http://svq.wangdashe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mal.zdqjudy.top

[Q34] 每组取第一条
来源：http://nmn.cqqwz.cn

SELECT * FROM (
来源：http://heg.ydzc1.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wcm.gotoacloud.top

) t WHERE rn = 1;
来源：http://kzh.316326.xyz

[Q35] 内连接
来源：http://zva.sufxvd.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ney.epnwcf.com

[Q36] 左连接
来源：http://pkx.yj202588.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ghf.yongpay.top

[Q37] 右连接
来源：http://zwx.jinyuanbaomall.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zbh.yangfankeji.com

[Q38] 全外连接（PostgreSQL）
来源：http://qht.yuxming.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ufh.jinghuilouyu.cn

[Q39] 自连接（查上下级）
来源：http://awy.aizwys.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://kub.zhiwuduotai.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vjf.dianchejie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kcn.gaohongyu789.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zwc.xuetiantiany.cn

[Q41] 多表连接
来源：http://bxq.snrcjt.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://nnv.kuanghao11.cn

JOIN users u ON u.id = o.user_id
来源：http://qer.zhoulong.xyz

JOIN products p ON p.id = o.product_id;
来源：http://guo.yueranfly.top

[Q42] 连接条件附加过滤
来源：http://mro.uphjek.com

SELECT u.name, o.amount FROM users u
来源：http://wlg.tianlin.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wuv.fzhhl.top

[Q43] 标量子查询
来源：http://kgu.jianghu66.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://guv.jianghu66.top

[Q44] IN 子查询
来源：http://ddh.hnqzz.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wbj.guowangkeji.top

[Q45] EXISTS 判断存在
来源：http://rgs.zdqjudy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rqm.havefunace.top

[Q46] NOT EXISTS 判断不存在
来源：http://deh.316326.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eau.feifeiyinyue.top

[Q47] 与平均值比较
来源：http://mqy.jqgufenzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ccc.52xcode.cn

[Q48] CTE 公用表表达式
来源：http://orc.zhixingplan.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://udb.xziqi.cn

SELECT * FROM t WHERE c > 5;
来源：http://odd.hfpthk.cn

[Q49] 更新单行
来源：http://ray.chenlongwang.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dil.bbcook.cn

[Q50] 批量更新
来源：http://lek.fehbvm.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sbz.ywan-chungtsiang.top

[Q51] 用子查询更新
来源：http://kxr.hywenlv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cyd.yanxiufei.cn

[Q52] 删除指定行
来源：http://irp.ywan-chungtsiang.top

DELETE FROM users WHERE id = 10;
来源：http://trc.ppjwa.cn

[Q53] 按条件删除
来源：http://hgq.havefunace.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fop.chenzaomai.com

[Q54] 清空表
来源：http://daq.tianlin.xyz

TRUNCATE TABLE logs;
来源：http://dws.316326.xyz

[Q55] 排名（并列占位）
来源：http://vbf.chenlongwang.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yhe.dashuyun.cn

[Q56] 密集排名（并列不占位）
来源：http://abg.ehwqpu.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://flp.dianchejie.cn

[Q57] 行号
来源：http://sft.zdbjq.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://usl.fengsongda.top

[Q58] 累计求和
来源：http://elp.hongshengwenyu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jgn.chenjidiqi.icu

[Q59] 分组内累计
来源：http://fmp.yj20258888.top


<!-- 参考信息 -->