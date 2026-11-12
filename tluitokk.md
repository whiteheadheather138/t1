代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ojx.hnxiangtu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dbl.tanke756.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hrc.hysaishi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yeg.dianchejie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://scm.316326.xyz

[N10] 链表节点定义
来源：http://kys.xinyue.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qva.jianghu66.top

PHP:  class Node { public $v; public $next = null; }
来源：http://zpq.aibaodan.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jjl.shangyingyoupin.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://avg.cucudq.cn

Java: class Node { int v; Node next; }
来源：http://mud.havefunace.top

Go:   type Node struct { V int; Next *Node }
来源：http://tzp.jinqigfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://iae.hnqzz.top

C#:   class Node { public int V; public Node? Next; }
来源：http://qdx.zhongyouzk.top

[N11] 二叉树中序遍历
来源：http://dqr.cqqwz.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://koc.snrcjt.cn

PHP:  // 手写递归函数
来源：http://zwz.chenjidiqi.icu

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uif.52xcode.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://byx.zhiwuduotai.top

Java: // 手写递归
来源：http://jsq.nanxuanxn.top

Go:   // 手写递归
来源：http://qew.zdbjq.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zpn.tian-w.cn

C#:   // 手写递归
来源：http://fub.jinqigufen.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mgo.hfpthk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cgc.havefunace.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kis.gaohongyu789.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ipd.daxiang520.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dad.cheryme.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qvf.ppjwa.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fxr.gzhubu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://thd.cashguo.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xvc.haohaochexian.top

================================================================================
来源：http://tnl.daxiang520.top

O. 并发与异步
来源：http://hqt.c1oappe.top

================================================================================
来源：http://win.tanke756.top

[O01] 启动一个线程
来源：http://bqc.pengpengdd.cyou

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wge.sjlbkw.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nik.dianchejie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ane.ybcxt.top

TS:   // 同 JS
来源：http://jcn.hysaishi.cn

Java: new Thread(() -> f()).start()
来源：http://wnc.shanyushiyangkeji.top

Go:   go f()
来源：http://ksf.daxiang520.top

Ruby: Thread.new { f }
来源：http://csb.haohaochexian.top

C#:   Task.Run(() => F());
来源：http://cyv.tianlin.xyz

[O02] 使用线程池
来源：http://arn.haohaochexian.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vfy.nanxuanxn.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://svu.ybcxt.top

JS:   // worker_threads 线程池
来源：http://bqd.fzhhl.top

TS:   // worker_threads 线程池
来源：http://dgh.ctjpmb.com

Java: Executors.newFixedThreadPool(4)
来源：http://hch.xuanzx.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sjf.shzxlz.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wyk.chenlongwang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bkg.316326.xyz

[O03] 加锁保护共享数据
来源：http://slv.iojbl.cn

Py:   with lock: shared += 1
来源：http://mky.fzhhl.top

PHP:  // 用 flock() 做文件锁
来源：http://dhs.tian-w.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uam.yueranfly.top

TS:   // 同 JS
来源：http://sch.quarkkingdee.top

Java: synchronized (this) { shared++; }
来源：http://awy.hfpthk.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://svy.hammf.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wny.yj20258.top

C#:   lock (gate) { shared++; }
来源：http://ije.ydzc1.top

[O04] 定义异步函数并等待
来源：http://zoe.guannengcc.top

Py:   async def f():⏎    await g()
来源：http://dfm.yuxming.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qor.ywan-chungtsiang.top

JS:   async function f() { await g(); }
来源：http://tvh.iojbl.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zhx.bbcook.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xzm.kuanghao11.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sgp.jyoumei.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pqe.jlsjyb.cn

C#:   async Task F() { await G(); }
来源：http://qcl.kuanghao11.cn

[O05] 并发执行并等待全部完成
来源：http://mqj.snrcjt.cn

Py:   asyncio.gather(*tasks)
来源：http://pih.zycfv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vgf.cqqwz.cn

JS:   await Promise.all(tasks)
来源：http://oin.yanxiufei.cn

TS:   await Promise.all(tasks)
来源：http://oju.shuidangran.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iac.hysaishi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zkd.316326.xyz

Ruby: threads.map(&:join)
来源：http://ufh.shuidangran.top

C#:   await Task.WhenAll(t1, t2)
来源：http://rlg.yuanzhike.top

[O06] 使用进程池
来源：http://apr.jianghu66.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ypq.andypj.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://nqu.haohaochexian.top

JS:   // child_process / cluster 模块
来源：http://lev.guowangkeji.top

TS:   // child_process / cluster 模块
来源：http://gju.c1oappe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pcp.bjfxy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tvd.aibaodan.cn

Ruby: // fork 块
来源：http://evm.yfazqb.com

C#:   Parallel.For
来源：http://kgh.yj202588.top

================================================================================
来源：http://bsi.ivvv.top

P. 常用工具函数
来源：http://rdg.birdmap.top

================================================================================
来源：http://vfo.hammf.cn

[P01] 生成 UUID
来源：http://xzx.jinghuilouyu.cn

Py:   str(uuid.uuid4())
来源：http://auq.jinqigfzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wqy.meibo888.top

JS:   crypto.randomUUID()
来源：http://bcc.daria6918.cn

TS:   crypto.randomUUID()
来源：http://peq.ydjk.org.cn

Java: UUID.randomUUID().toString()
来源：http://jdz.redwolf501.top

Go:   // 用 github.com/google/uuid
来源：http://qmt.hnxiangtu.top

Ruby: SecureRandom.uuid
来源：http://pad.hcnkem.com

C#:   Guid.NewGuid().ToString()
来源：http://jcn.andypj.xyz

[P02] MD5 / SHA256 摘要
来源：http://exi.fktsv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xtz.nwbrower.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://mdy.nanxuanxn.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bdj.hfpthk.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dtb.jyoumei.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sno.chenlongwang.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://enz.xinyue.icu

Ruby: Digest::SHA256.hexdigest(s)
来源：http://aac.jlsjyb.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jmo.nanxinkj.top

[P03] 生成短随机字符串
来源：http://bmb.zhongyouzk.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wjw.jianghu66.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tcv.daria6918.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qtn.meibo888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jhj.cqqwz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tvw.xylfe.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mzl.hnqzz.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://wnx.bjfxy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://akb.sweek.top

[P04] 求长度
来源：http://rcc.shuidangran.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ysn.sufxvd.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sgd.uphjek.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ufj.yuxming.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dwe.cdnleiting.top

Java: list.size();  map.size();  s.length()
来源：http://udi.shanyushiyangtech.top

Go:   len(arr);  len(m)
来源：http://ews.ppjwa.cn

Ruby: x.length;  x.size
来源：http://wnb.gogol.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://eve.jianghu66.top

[P05] 判断两个对象内容是否相等
来源：http://icw.ydjk.org.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://imv.feifeiyinyue.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://prt.smart0.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rnj.shangyingyoupin.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://omb.wangdashe.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uni.vqdsnc.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lry.gzhubu.top

Ruby: a == b
来源：http://kkm.tanke756.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ele.dashuyun.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hmo.daxiang520.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://csk.hfpthk.cn

PHP:  if (empty($x)) {}
来源：http://lit.chenlongwang.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pqw.tian-w.cn

TS:   if (x == null) {}
来源：http://nld.316326.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://nwj.shangyingyoupin.top

Go:   if x == nil {}
来源：http://jzm.xziqi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hhv.hfpthk.cn

C#:   if (x is null) {}
来源：http://ktg.zhixingplan.top

[P07] 防抖与节流
来源：http://ore.bjfxy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pxd.birdmap.top

PHP:  // 手写时间戳比较
来源：http://qtd.ybcxt.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cfz.cucudq.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ahd.ywan-chungtsiang.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dxl.andypj.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rfh.hfpthk.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://oeu.chenjidiqi.icu

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uyp.shanyushiyangkeji.top

[P08] 处理浮点精度问题
来源：http://szz.52xcode.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lyy.hammf.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ecg.cashguo.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lju.iojbl.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://syb.fehbvm.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://alq.epnwcf.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cmn.haohaochexian.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mmp.ppjwa.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tuw.jyoumei.cn

================================================================================
来源：http://ujr.zhiwuduotai.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nss.ppjwa.cn

================================================================================
来源：http://jhn.nwbrower.top

[Q01] 创建表
来源：http://gtq.fktsv.cn

CREATE TABLE users (
来源：http://gjx.uphjek.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kpr.dianchejie.cn

name VARCHAR(50) NOT NULL,
来源：http://ccr.gzhubu.top

email VARCHAR(100) UNIQUE,
来源：http://qrv.dianchejie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jat.jinyuanbaomall.cn

);
来源：http://hwp.zhixingplan.top

[Q02] 创建带外键的表
来源：http://ijs.52xcode.cn

CREATE TABLE orders (
来源：http://xws.smart0.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ekp.feifeiyinyue.top

user_id INT NOT NULL,
来源：http://npa.pycfn.com

amount DECIMAL(10, 2),
来源：http://gos.yfazqb.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xxl.zhixingplan.top

);
来源：http://mqj.cqqwz.cn

[Q03] 增加列
来源：http://ejg.dashuyun.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rna.ywan-chungtsiang.top

[Q04] 修改列类型
来源：http://fym.jyoumei.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ptu.nanxinkj.top

[Q05] 重命名列
来源：http://vyi.ybcxt.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mwn.jyoumei.cn

[Q06] 删除列
来源：http://eme.gogol.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dip.andypj.xyz

[Q07] 删除表
来源：http://pry.zhengqikj.top

DROP TABLE IF EXISTS orders;
来源：http://drj.cdnleiting.top

[Q08] 创建普通索引
来源：http://ifj.svipenyu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zir.tanke756.top

[Q09] 创建唯一索引
来源：http://pxt.shanyushiyangkeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zvm.tarul.cn

[Q10] 插入单行
来源：http://vhn.ctjpmb.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fjr.pengpengdd.cyou

[Q11] 一次插入多行
来源：http://grb.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pdq.meibo888.top

[Q12] 插入后取自增 ID
来源：http://uyo.sjlbkw.cn

INSERT INTO users (name) VALUES ('C');
来源：http://kmo.jinqigfzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vqj.bbcook.cn

[Q13] 忽略重复插入
来源：http://rbl.cashguo.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zsu.zdqjudy.top

[Q14] 存在则更新（upsert）
来源：http://hvf.zhixingplan.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://raz.jinghuilouyu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yif.sufxvd.cn

[Q15] 查询全部
来源：http://tdl.nwbrower.top

SELECT * FROM users;
来源：http://txi.yvedp.cn

[Q16] 查询指定列
来源：http://gwo.9152youxi.cn

SELECT id, name FROM users;
来源：http://prq.fengsongda.top

[Q17] 条件查询
来源：http://wsl.mhx1999.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yyr.shangyingyoupin.top

[Q18] 模糊匹配
来源：http://sga.52xcode.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jlx.ybcxt.top

[Q19] 范围查询
来源：http://rtg.yuanzhike.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://eav.shangyingyoupin.top

[Q20] IN 列表
来源：http://dzq.zdqjudy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lnl.guowangkeji.top

[Q21] 空值判断
来源：http://her.kuanghao11.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://eav.zhengqikj.top

[Q22] 排序
来源：http://yor.hywenlv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nxu.zdqjudy.top

[Q23] 分页
来源：http://smz.andypj.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bdf.wangshuangyany.cn

[Q24] 去重
来源：http://zxx.andypj.xyz

SELECT DISTINCT city FROM users;
来源：http://qlg.hammf.cn

[Q25] 只取前 N 条
来源：http://ejc.hcnkem.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yol.shanyushiyangtech.top

[Q26] 计数
来源：http://lwc.jinqigfzy.top

SELECT COUNT(*) FROM users;
来源：http://jlo.hcnkem.com

[Q27] 条件计数
来源：http://owx.svipenyu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hua.jinqigufen.top

[Q28] 求和与平均
来源：http://pze.hfpthk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mgz.yueranfly.top

[Q29] 最大最小值
来源：http://epr.yj20258888.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://oyd.yanxiufei.cn

[Q30] 分组统计
来源：http://wfl.ywan-chungtsiang.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dme.xinyue.icu

[Q31] 分组后过滤
来源：http://uns.yonumen.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ulp.ybcxt.top

[Q32] 分组拼接字符串
来源：http://gbp.cqqwz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mrn.sufxvd.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ian.cucudq.cn

[Q33] 多列分组
来源：http://tjd.kuanghao11.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hzl.cheryme.top

[Q34] 每组取第一条
来源：http://trp.havefunace.top

SELECT * FROM (
来源：http://xwg.shangyingyoupin.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lul.bjfxy.top

) t WHERE rn = 1;
来源：http://bni.cdnleiting.top

[Q35] 内连接
来源：http://xkx.hnqzz.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mdw.pycfn.com

[Q36] 左连接
来源：http://qim.yueranfly.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jwd.yongpay.top

[Q37] 右连接
来源：http://hdz.dianchejie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://utz.yj202588.top

[Q38] 全外连接（PostgreSQL）
来源：http://ytg.zhijiandao.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vjd.jiagoushi.top

[Q39] 自连接（查上下级）
来源：http://fpy.gogol.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hlq.yanxiufei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://weh.yangfankeji.com

[Q40] 交叉连接（笛卡尔积）
来源：http://xfy.yj20258888.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ogc.0kj1m.cn

[Q41] 多表连接
来源：http://uzg.yj202588.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://kkp.jqgufenzy.top

JOIN users u ON u.id = o.user_id
来源：http://qak.dashuyun.cn

JOIN products p ON p.id = o.product_id;
来源：http://nfb.c1oappe.top

[Q42] 连接条件附加过滤
来源：http://niy.aizwys.cn

SELECT u.name, o.amount FROM users u
来源：http://guh.shanyushiyangtech.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yxt.yj20258.top

[Q43] 标量子查询
来源：http://omd.xylfe.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vwy.zhijiandao.cn

[Q44] IN 子查询
来源：http://ejy.gogol.net.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fdx.zhaomingkeji.xyz

[Q45] EXISTS 判断存在
来源：http://csf.hnqzz.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://csq.redwolf501.top

[Q46] NOT EXISTS 判断不存在
来源：http://ipc.yj20258.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ygd.jiagoushi.top

[Q47] 与平均值比较
来源：http://wqm.52xcode.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fbf.bjfxy.top

[Q48] CTE 公用表表达式
来源：http://jxv.jinyuanbaomall.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vyi.yueranfly.top

SELECT * FROM t WHERE c > 5;
来源：http://rfu.yuanzhike.top

[Q49] 更新单行
来源：http://xch.cucudq.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mmb.havefunace.top

[Q50] 批量更新
来源：http://cau.ctjpmb.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jzb.bjfxy.top

[Q51] 用子查询更新
来源：http://lve.cheryme.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://brs.haohaochexian.top

[Q52] 删除指定行
来源：http://lzn.sweek.top

DELETE FROM users WHERE id = 10;
来源：http://ckd.jinqigufen.top

[Q53] 按条件删除
来源：http://ceo.guowangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ngv.xylfe.cn

[Q54] 清空表
来源：http://lqs.yanxiufei.cn

TRUNCATE TABLE logs;
来源：http://dxm.fzhhl.top

[Q55] 排名（并列占位）
来源：http://kny.daria6918.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://eqo.ybcxt.top

[Q56] 密集排名（并列不占位）
来源：http://taz.sufxvd.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lkk.hnqzz.top

[Q57] 行号
来源：http://gqw.birdmap.top


<!-- 参考信息 -->