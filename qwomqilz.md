代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zha.nanxuanxn.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uys.jinqigufen.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cqk.sxryk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dqg.havefunace.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gqc.svipenyu.cn

[N10] 链表节点定义
来源：http://dhh.gogol.net.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gqg.ctjpmb.com

PHP:  class Node { public $v; public $next = null; }
来源：http://uwh.hywenlv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://khe.sjlbkw.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mco.zdqjudy.top

Java: class Node { int v; Node next; }
来源：http://dzb.nanxinkj.top

Go:   type Node struct { V int; Next *Node }
来源：http://vma.hcnkem.com

Ruby: Node = Struct.new(:v, :next)
来源：http://pza.chenlongwang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jrl.jiagoushi.top

[N11] 二叉树中序遍历
来源：http://rdn.xinyue.icu

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pra.fehbvm.com

PHP:  // 手写递归函数
来源：http://qms.wangdashe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oxe.sjlbkw.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fhf.hywenlv.cn

Java: // 手写递归
来源：http://jvr.ppjwa.cn

Go:   // 手写递归
来源：http://ydu.yvedp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wjx.yfazqb.com

C#:   // 手写递归
来源：http://ypc.sufxvd.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bvz.c1oappe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iat.zhengqikj.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vpg.tanke756.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cit.hfpthk.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pgd.ydjk.org.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mrk.yj20258.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zjh.sweek.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wdw.hysaishi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wkx.zycfv.cn

================================================================================
来源：http://vjd.uphjek.com

O. 并发与异步
来源：http://lgd.fehbvm.com

================================================================================
来源：http://dfs.chenjidiqi.icu

[O01] 启动一个线程
来源：http://cuw.shuidangran.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pck.jqgfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dkn.cdnleiting.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://psa.ydjk.org.cn

TS:   // 同 JS
来源：http://afh.xziqi.cn

Java: new Thread(() -> f()).start()
来源：http://nkx.0kj1m.cn

Go:   go f()
来源：http://yco.cucudq.cn

Ruby: Thread.new { f }
来源：http://yub.yj202588.top

C#:   Task.Run(() => F());
来源：http://scc.yj202588.top

[O02] 使用线程池
来源：http://nio.birdmap.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://idi.jlsjyb.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xjt.52xcode.cn

JS:   // worker_threads 线程池
来源：http://jww.jinyuanbaomall.cn

TS:   // worker_threads 线程池
来源：http://kme.bbcook.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zql.mhx1999.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ldw.daxiang520.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fom.vehdjk.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kgl.yvedp.cn

[O03] 加锁保护共享数据
来源：http://jtf.xylfe.cn

Py:   with lock: shared += 1
来源：http://bcc.hysaishi.cn

PHP:  // 用 flock() 做文件锁
来源：http://ecx.bjfxy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://shk.316326.xyz

TS:   // 同 JS
来源：http://cdy.ehwqpu.com

Java: synchronized (this) { shared++; }
来源：http://mzp.birdmap.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vyv.jinqigfzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://pyj.fehbvm.com

C#:   lock (gate) { shared++; }
来源：http://ggw.yangfankeji.com

[O04] 定义异步函数并等待
来源：http://lzz.birdmap.top

Py:   async def f():⏎    await g()
来源：http://xox.birdmap.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ans.epnwcf.com

JS:   async function f() { await g(); }
来源：http://kfs.yfazqb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://ijw.9152youxi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mjr.chenzaomai.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lnq.xylfe.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tgm.tian-w.cn

C#:   async Task F() { await G(); }
来源：http://jwq.jianghu66.top

[O05] 并发执行并等待全部完成
来源：http://vep.feifeiyinyue.top

Py:   asyncio.gather(*tasks)
来源：http://pho.dianchejie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ybh.zhixingplan.top

JS:   await Promise.all(tasks)
来源：http://qob.bbcook.cn

TS:   await Promise.all(tasks)
来源：http://krb.zycfv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mtw.chenlongwang.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xjc.cdnleiting.top

Ruby: threads.map(&:join)
来源：http://air.xziqi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vcq.cashguo.top

[O06] 使用进程池
来源：http://mep.iojbl.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cui.havefunace.top

PHP:  // pcntl_fork 或多进程队列
来源：http://cyw.aibaodan.cn

JS:   // child_process / cluster 模块
来源：http://loy.yueranfly.top

TS:   // child_process / cluster 模块
来源：http://mdp.sufxvd.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ixj.hywenlv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oqa.shanyushiyangtech.top

Ruby: // fork 块
来源：http://rba.gotoacloud.top

C#:   Parallel.For
来源：http://kqw.hcnkem.com

================================================================================
来源：http://xpg.shangyingyoupin.top

P. 常用工具函数
来源：http://kfk.hesvh.cn

================================================================================
来源：http://dcv.hongshengwenyu.top

[P01] 生成 UUID
来源：http://pln.zhijiandao.cn

Py:   str(uuid.uuid4())
来源：http://tse.fanxiaobao.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fgy.jinyuanbaomall.cn

JS:   crypto.randomUUID()
来源：http://wvy.yj202588.top

TS:   crypto.randomUUID()
来源：http://moq.yonumen.top

Java: UUID.randomUUID().toString()
来源：http://nul.cheryme.top

Go:   // 用 github.com/google/uuid
来源：http://xvy.bbcook.cn

Ruby: SecureRandom.uuid
来源：http://ctf.xuanzx.com

C#:   Guid.NewGuid().ToString()
来源：http://owf.feifeiyinyue.top

[P02] MD5 / SHA256 摘要
来源：http://org.aizwys.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ttf.hesvh.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://csb.gzhubu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://amo.jinqigufen.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rth.zhaomingkeji.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rqy.fzhhl.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://azv.epnwcf.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ngp.xuetiantiany.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gpf.pycfn.com

[P03] 生成短随机字符串
来源：http://cju.svipenyu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sdb.zdqjudy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tfe.dianchejie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://idu.guannengcc.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ecb.zdbjq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kye.xingfuxueyuan.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zhq.zhongyouzk.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ank.zycfv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lhs.jinqigfzy.top

[P04] 求长度
来源：http://bzh.shuidangran.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pcq.shuidangran.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xic.svipenyu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mgt.shuidangran.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vxg.shzxlz.cn

Java: list.size();  map.size();  s.length()
来源：http://omn.ppjwa.cn

Go:   len(arr);  len(m)
来源：http://ntz.c1oappe.top

Ruby: x.length;  x.size
来源：http://inb.bjfxy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xin.yj20258.top

[P05] 判断两个对象内容是否相等
来源：http://wdx.vqdsnc.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lcz.chenlongwang.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kry.xuetiantiany.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jod.zhiwuduotai.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nuu.daria6918.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tnx.vqdsnc.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mjh.chenjidiqi.icu

Ruby: a == b
来源：http://xxj.zhengqikj.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jkg.hysaishi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://use.daxiang520.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wsm.gotoacloud.top

PHP:  if (empty($x)) {}
来源：http://fms.ydjk.org.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wju.xinyue.icu

TS:   if (x == null) {}
来源：http://hvk.xingfuxueyuan.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://egh.52xcode.cn

Go:   if x == nil {}
来源：http://kow.meibo888.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fcp.jqgufenzy.top

C#:   if (x is null) {}
来源：http://glf.yanxiufei.cn

[P07] 防抖与节流
来源：http://mur.jinyuanbaomall.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cws.chenlongwang.top

PHP:  // 手写时间戳比较
来源：http://gkm.hnqzz.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cxp.chenlongwang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oqx.hysaishi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gbs.jinqigufen.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pig.xinyue.icu

Ruby: // 手写闭包 + Time.now 判断
来源：http://ikz.c1oappe.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dtj.cqqwz.cn

[P08] 处理浮点精度问题
来源：http://qte.bbcook.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wyf.guowangkeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qiq.c1oappe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vvw.shuidangran.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wpu.jqgufenzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nmv.ctjpmb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fan.andypj.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hei.ywan-chungtsiang.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://adk.tianlin.xyz

================================================================================
来源：http://hzm.chenlongwang.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ijt.tian-w.cn

================================================================================
来源：http://nxo.daxiang520.top

[Q01] 创建表
来源：http://dvb.andypj.xyz

CREATE TABLE users (
来源：http://wnw.fanxiaobao.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://imr.316326.xyz

name VARCHAR(50) NOT NULL,
来源：http://hfr.gzhubu.top

email VARCHAR(100) UNIQUE,
来源：http://jvi.redwolf501.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yul.hysaishi.cn

);
来源：http://tkl.gotoacloud.top

[Q02] 创建带外键的表
来源：http://jal.ydzc1.top

CREATE TABLE orders (
来源：http://dsw.shangyingyoupin.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://veh.yj20258888.top

user_id INT NOT NULL,
来源：http://qel.ehwqpu.com

amount DECIMAL(10, 2),
来源：http://zpb.zhijiandao.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zpt.ydzc1.top

);
来源：http://ooy.andypj.xyz

[Q03] 增加列
来源：http://smd.hammf.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://onq.ppjwa.cn

[Q04] 修改列类型
来源：http://djv.sxryk.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ejb.xuetiantiany.cn

[Q05] 重命名列
来源：http://ylg.jqgfzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://siu.bjfxy.top

[Q06] 删除列
来源：http://jrg.iojbl.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dey.sweek.top

[Q07] 删除表
来源：http://lzc.bbcook.cn

DROP TABLE IF EXISTS orders;
来源：http://prf.snrcjt.cn

[Q08] 创建普通索引
来源：http://eur.gzhubu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://bhe.c1oappe.top

[Q09] 创建唯一索引
来源：http://yxy.hysaishi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kqz.aibaodan.cn

[Q10] 插入单行
来源：http://wzn.andypj.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ozk.daxiang520.top

[Q11] 一次插入多行
来源：http://lcf.jinghuilouyu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dpy.uphjek.com

[Q12] 插入后取自增 ID
来源：http://mau.haohaochexian.top

INSERT INTO users (name) VALUES ('C');
来源：http://dih.xylfe.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ipb.gotoacloud.top

[Q13] 忽略重复插入
来源：http://uyb.316326.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rnn.chenzaomai.com

[Q14] 存在则更新（upsert）
来源：http://ppi.vqdsnc.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://eco.gaohongyu789.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zpj.vqdsnc.cn

[Q15] 查询全部
来源：http://qku.havefunace.top

SELECT * FROM users;
来源：http://pvs.yj20258.top

[Q16] 查询指定列
来源：http://nyx.xuetiantiany.cn

SELECT id, name FROM users;
来源：http://rjl.svipenyu.cn

[Q17] 条件查询
来源：http://ocz.c1oappe.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://udw.jinqigufen.top

[Q18] 模糊匹配
来源：http://evt.hcnkem.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hut.ydzc1.top

[Q19] 范围查询
来源：http://njl.sjlbkw.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://far.zhiwuduotai.top

[Q20] IN 列表
来源：http://pje.cashguo.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qzs.hnxiangtu.top

[Q21] 空值判断
来源：http://uoc.sxryk.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bcx.cqqwz.cn

[Q22] 排序
来源：http://zzd.c1oappe.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xgb.chenzaomai.com

[Q23] 分页
来源：http://ixh.jinqigfzy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kgx.jinqigfzy.top

[Q24] 去重
来源：http://szc.chenjidiqi.icu

SELECT DISTINCT city FROM users;
来源：http://dtt.hammf.cn

[Q25] 只取前 N 条
来源：http://gvg.xylfe.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tyy.shanyushiyangtech.top

[Q26] 计数
来源：http://jkn.jqgufenzy.top

SELECT COUNT(*) FROM users;
来源：http://lvl.hesvh.cn

[Q27] 条件计数
来源：http://cmc.jinqigufen.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qqm.gaohongyu789.top

[Q28] 求和与平均
来源：http://htv.meibo888.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hyv.fanxiaobao.xyz

[Q29] 最大最小值
来源：http://yff.yonumen.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://nkz.guannengcc.top

[Q30] 分组统计
来源：http://umv.gotoacloud.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://atn.shangyingyoupin.top

[Q31] 分组后过滤
来源：http://mye.chenzaomai.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wwb.yuanzhike.top

[Q32] 分组拼接字符串
来源：http://vme.jlsjyb.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rut.shanyushiyangtech.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kaq.fehbvm.com

[Q33] 多列分组
来源：http://cuf.chenlongwang.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ryd.daxiang520.top

[Q34] 每组取第一条
来源：http://rup.ywan-chungtsiang.top

SELECT * FROM (
来源：http://rfc.zhiwuduotai.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hiu.shuidangran.top

) t WHERE rn = 1;
来源：http://irx.fktsv.cn

[Q35] 内连接
来源：http://vqg.hnqzz.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kti.hywenlv.cn

[Q36] 左连接
来源：http://nad.hywenlv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://seh.yanxiufei.cn

[Q37] 右连接
来源：http://rit.uphjek.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yry.ydjk.org.cn

[Q38] 全外连接（PostgreSQL）
来源：http://iew.fanxiaobao.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fzf.hesvh.cn

[Q39] 自连接（查上下级）
来源：http://gqr.jlsjyb.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://rki.yj202588.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nvi.zhiwuduotai.top

[Q40] 交叉连接（笛卡尔积）
来源：http://vvm.quarkkingdee.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://giw.bbcook.cn

[Q41] 多表连接
来源：http://jva.yj20258.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://plx.fanxiaobao.xyz

JOIN users u ON u.id = o.user_id
来源：http://kaj.hfpthk.cn

JOIN products p ON p.id = o.product_id;
来源：http://zch.yuxming.cn

[Q42] 连接条件附加过滤
来源：http://bws.ctjpmb.com

SELECT u.name, o.amount FROM users u
来源：http://oyj.wangdashe.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bnf.dianchejie.cn

[Q43] 标量子查询
来源：http://uia.52xcode.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ggn.yj202588.top

[Q44] IN 子查询
来源：http://ckm.gaohongyu789.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mpq.fehbvm.com

[Q45] EXISTS 判断存在
来源：http://jwi.nwbrower.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sxs.hywenlv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cqj.hcnkem.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wzb.quarkkingdee.top

[Q47] 与平均值比较
来源：http://ikg.haohaochexian.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lnw.zhoulong.xyz

[Q48] CTE 公用表表达式
来源：http://rkw.zhiwuduotai.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ios.hnqzz.top

SELECT * FROM t WHERE c > 5;
来源：http://luo.yj20258888.top

[Q49] 更新单行
来源：http://ydj.hesvh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qky.kuanghao11.cn

[Q50] 批量更新
来源：http://bwx.fktsv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kcp.sjlbkw.cn

[Q51] 用子查询更新
来源：http://fvk.jinqigufen.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ufg.tanke756.top

[Q52] 删除指定行
来源：http://bpu.jyoumei.cn

DELETE FROM users WHERE id = 10;
来源：http://wml.yj20258.top

[Q53] 按条件删除
来源：http://ykt.hesvh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://twj.ydzc1.top

[Q54] 清空表
来源：http://nnd.yangfankeji.com

TRUNCATE TABLE logs;
来源：http://ita.cqqwz.cn

[Q55] 排名（并列占位）
来源：http://wcz.wangdashe.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dyz.nwbrower.top

[Q56] 密集排名（并列不占位）
来源：http://hsr.tanke756.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://for.hesvh.cn

[Q57] 行号
来源：http://mpd.yvedp.cn


<!-- 参考信息 -->