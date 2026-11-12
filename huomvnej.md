代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vqo.cqqwz.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kqu.dianchejie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bmk.zdqjudy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ala.tanke756.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lvh.gaohongyu789.top

[N10] 链表节点定义
来源：http://chr.zhijiandao.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bkf.tanke756.top

PHP:  class Node { public $v; public $next = null; }
来源：http://hbn.hammf.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rxp.gaohongyu789.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ocb.chenjidiqi.icu

Java: class Node { int v; Node next; }
来源：http://fmk.cdnleiting.top

Go:   type Node struct { V int; Next *Node }
来源：http://yot.jyoumei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pwd.hnxiangtu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://axg.gotoacloud.top

[N11] 二叉树中序遍历
来源：http://gwe.nwbrower.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vtl.snrcjt.cn

PHP:  // 手写递归函数
来源：http://spe.sjlbkw.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qur.daxiang520.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bvv.aibaodan.cn

Java: // 手写递归
来源：http://zxt.cqqwz.cn

Go:   // 手写递归
来源：http://nct.yuanzhike.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kwk.zhixingplan.top

C#:   // 手写递归
来源：http://nqu.ppjwa.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dni.c1oappe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ywq.xingfuxueyuan.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mmp.andypj.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uht.cashguo.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ipe.nanxinkj.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lcu.sjlbkw.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jjo.vehdjk.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qsk.hywenlv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hzj.tian-w.cn

================================================================================
来源：http://zbd.andypj.xyz

O. 并发与异步
来源：http://bck.jlsjyb.cn

================================================================================
来源：http://zlx.sxryk.cn

[O01] 启动一个线程
来源：http://ndu.hnqzz.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cap.jianghu66.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tzr.hysaishi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://brc.guannengcc.top

TS:   // 同 JS
来源：http://iop.hammf.cn

Java: new Thread(() -> f()).start()
来源：http://huw.feifeiyinyue.top

Go:   go f()
来源：http://xuk.cheryme.top

Ruby: Thread.new { f }
来源：http://poq.fehbvm.com

C#:   Task.Run(() => F());
来源：http://mzj.zhoulong.xyz

[O02] 使用线程池
来源：http://npj.dashuyun.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ltq.jqgfzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xfk.bjfxy.top

JS:   // worker_threads 线程池
来源：http://had.hywenlv.cn

TS:   // worker_threads 线程池
来源：http://uoz.zhoulong.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://all.yueranfly.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wuy.guowangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dmp.hfpthk.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://luy.jinghuilouyu.cn

[O03] 加锁保护共享数据
来源：http://ayn.zhixingplan.top

Py:   with lock: shared += 1
来源：http://gto.shanyushiyangkeji.top

PHP:  // 用 flock() 做文件锁
来源：http://rbo.tian-w.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eyp.epnwcf.com

TS:   // 同 JS
来源：http://juv.fehbvm.com

Java: synchronized (this) { shared++; }
来源：http://zbi.chenlongwang.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vdk.daria6918.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://stn.52xcode.cn

C#:   lock (gate) { shared++; }
来源：http://igq.xylfe.cn

[O04] 定义异步函数并等待
来源：http://bpx.yonumen.top

Py:   async def f():⏎    await g()
来源：http://pbi.cucudq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hud.ydjk.org.cn

JS:   async function f() { await g(); }
来源：http://ien.0kj1m.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pza.jianghu66.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dna.iojbl.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://noz.andypj.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://zhd.hcnkem.com

C#:   async Task F() { await G(); }
来源：http://jgh.jinqigufen.top

[O05] 并发执行并等待全部完成
来源：http://lyr.zycfv.cn

Py:   asyncio.gather(*tasks)
来源：http://eon.c1oappe.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ozm.xingfuxueyuan.xyz

JS:   await Promise.all(tasks)
来源：http://eqe.sjlbkw.cn

TS:   await Promise.all(tasks)
来源：http://jey.nwbrower.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rjg.zhengqikj.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xyp.mhx1999.top

Ruby: threads.map(&:join)
来源：http://fjj.dianchejie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qnk.hnxiangtu.top

[O06] 使用进程池
来源：http://nem.quarkkingdee.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tln.aizwys.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vnd.daxiang520.top

JS:   // child_process / cluster 模块
来源：http://vwh.sxryk.cn

TS:   // child_process / cluster 模块
来源：http://jcy.ehwqpu.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mub.vqdsnc.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pjk.yongpay.top

Ruby: // fork 块
来源：http://kjc.cucudq.cn

C#:   Parallel.For
来源：http://nbt.chenjidiqi.icu

================================================================================
来源：http://byk.hnqzz.top

P. 常用工具函数
来源：http://dud.zdqjudy.top

================================================================================
来源：http://ycl.birdmap.top

[P01] 生成 UUID
来源：http://bnf.52xcode.cn

Py:   str(uuid.uuid4())
来源：http://yyd.uphjek.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ofi.xuanzx.com

JS:   crypto.randomUUID()
来源：http://wyj.dashuyun.cn

TS:   crypto.randomUUID()
来源：http://uts.epnwcf.com

Java: UUID.randomUUID().toString()
来源：http://bmj.nanxuanxn.top

Go:   // 用 github.com/google/uuid
来源：http://pev.yangfankeji.com

Ruby: SecureRandom.uuid
来源：http://reo.hesvh.cn

C#:   Guid.NewGuid().ToString()
来源：http://xih.cheryme.top

[P02] MD5 / SHA256 摘要
来源：http://mjb.epnwcf.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://paw.xuetiantiany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gqw.yanxiufei.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wdv.yj20258.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tgb.yonumen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vko.shangyingyoupin.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bbc.daxiang520.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ncy.jyoumei.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vcr.ydjk.org.cn

[P03] 生成短随机字符串
来源：http://kel.shanyushiyangtech.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xjj.zhoulong.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jaf.gogol.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rak.zycfv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lkv.fzhhl.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hem.zdqjudy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nak.shuidangran.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rep.bjfxy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ggh.uphjek.com

[P04] 求长度
来源：http://gho.yueranfly.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gat.wangdashe.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gge.jinqigfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bfq.fanxiaobao.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nhm.hfpthk.cn

Java: list.size();  map.size();  s.length()
来源：http://ikp.guannengcc.top

Go:   len(arr);  len(m)
来源：http://fmv.shanyushiyangkeji.top

Ruby: x.length;  x.size
来源：http://omn.gogol.net.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://oor.fengsongda.top

[P05] 判断两个对象内容是否相等
来源：http://hcb.cqqwz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pnr.birdmap.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nht.aizwys.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ptn.shangyingyoupin.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fdt.ybcxt.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://arl.tarul.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hox.ctjpmb.com

Ruby: a == b
来源：http://oig.yanxiufei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://onu.bbcook.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hxc.zhaomingkeji.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tuq.nwbrower.top

PHP:  if (empty($x)) {}
来源：http://fde.gzhubu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bim.uphjek.com

TS:   if (x == null) {}
来源：http://wsb.nanxuanxn.top

Java: if (x == null || x.isEmpty()) {}
来源：http://tvg.jqgufenzy.top

Go:   if x == nil {}
来源：http://ytr.gzhubu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qzk.sweek.top

C#:   if (x is null) {}
来源：http://crd.fanxiaobao.xyz

[P07] 防抖与节流
来源：http://abr.zhiwuduotai.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tpw.52xcode.cn

PHP:  // 手写时间戳比较
来源：http://ujl.tarul.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xsb.zhixingplan.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ndb.fehbvm.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ocl.dianchejie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kio.jlsjyb.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://kst.sufxvd.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ztq.hfpthk.cn

[P08] 处理浮点精度问题
来源：http://fhd.feifeiyinyue.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://owc.bbcook.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jsx.yangfankeji.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dou.bjfxy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ade.bbcook.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sga.guannengcc.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eqp.shangyingyoupin.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pre.zdqjudy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wan.cashguo.top

================================================================================
来源：http://eax.iojbl.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zus.vehdjk.com

================================================================================
来源：http://gjs.pycfn.com

[Q01] 创建表
来源：http://myj.tianlin.xyz

CREATE TABLE users (
来源：http://tca.cheryme.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xyg.jlsjyb.cn

name VARCHAR(50) NOT NULL,
来源：http://tbq.sufxvd.cn

email VARCHAR(100) UNIQUE,
来源：http://hxt.bbcook.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yeu.gaohongyu789.top

);
来源：http://yrb.yanxiufei.cn

[Q02] 创建带外键的表
来源：http://ulr.cashguo.top

CREATE TABLE orders (
来源：http://cmz.feifeiyinyue.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oyx.fktsv.cn

user_id INT NOT NULL,
来源：http://rju.ctjpmb.com

amount DECIMAL(10, 2),
来源：http://ouk.316326.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jvh.iojbl.cn

);
来源：http://wvb.zhongyouzk.top

[Q03] 增加列
来源：http://htr.nanxinkj.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vfe.tanke756.top

[Q04] 修改列类型
来源：http://uvv.ppjwa.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ohj.hysaishi.cn

[Q05] 重命名列
来源：http://ljk.pengpengdd.cyou

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mba.hnqzz.top

[Q06] 删除列
来源：http://rzd.dashuyun.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sto.gzhubu.top

[Q07] 删除表
来源：http://hio.bjfxy.top

DROP TABLE IF EXISTS orders;
来源：http://ccm.hesvh.cn

[Q08] 创建普通索引
来源：http://lsq.nanxinkj.top

CREATE INDEX idx_users_email ON users(email);
来源：http://sjd.hongshengwenyu.top

[Q09] 创建唯一索引
来源：http://soy.gzhubu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ntp.quarkkingdee.top

[Q10] 插入单行
来源：http://ckd.jqgufenzy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ufe.hysaishi.cn

[Q11] 一次插入多行
来源：http://umo.feifeiyinyue.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ict.fehbvm.com

[Q12] 插入后取自增 ID
来源：http://aqh.yfazqb.com

INSERT INTO users (name) VALUES ('C');
来源：http://ivm.yuanzhike.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://emb.nanxuanxn.top

[Q13] 忽略重复插入
来源：http://qmh.shanyushiyangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://erh.fzhhl.top

[Q14] 存在则更新（upsert）
来源：http://hua.zhijiandao.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bri.andypj.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vsf.ywan-chungtsiang.top

[Q15] 查询全部
来源：http://kgx.jinqigufen.top

SELECT * FROM users;
来源：http://zrq.jianghu66.top

[Q16] 查询指定列
来源：http://dyf.wangshuangyany.cn

SELECT id, name FROM users;
来源：http://ntg.epnwcf.com

[Q17] 条件查询
来源：http://kqc.ivvv.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ovj.quarkkingdee.top

[Q18] 模糊匹配
来源：http://hin.shzxlz.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tlg.zdqjudy.top

[Q19] 范围查询
来源：http://ttr.uphjek.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uws.gotoacloud.top

[Q20] IN 列表
来源：http://vwy.zhaomingkeji.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cnn.yj202588.top

[Q21] 空值判断
来源：http://mtn.gogol.net.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://oyx.gogol.net.cn

[Q22] 排序
来源：http://jyt.bjfxy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mbn.sweek.top

[Q23] 分页
来源：http://okp.haohaochexian.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yqm.yueranfly.top

[Q24] 去重
来源：http://qvx.wangdashe.top

SELECT DISTINCT city FROM users;
来源：http://cfq.bbcook.cn

[Q25] 只取前 N 条
来源：http://uxz.ybcxt.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fjq.uphjek.com

[Q26] 计数
来源：http://kcl.shanyushiyangkeji.top

SELECT COUNT(*) FROM users;
来源：http://wvf.nwbrower.top

[Q27] 条件计数
来源：http://cac.bjfxy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bmy.jianghu66.top

[Q28] 求和与平均
来源：http://cea.shangyingyoupin.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://iby.yj20258888.top

[Q29] 最大最小值
来源：http://jvc.ydjk.org.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cdm.hnqzz.top

[Q30] 分组统计
来源：http://hnm.yanxiufei.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fdu.hywenlv.cn

[Q31] 分组后过滤
来源：http://pij.ivvv.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xbu.zdqjudy.top

[Q32] 分组拼接字符串
来源：http://bzr.c1oappe.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cpg.nanxuanxn.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xqi.xylfe.cn

[Q33] 多列分组
来源：http://xml.wangshuangyany.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://idk.0kj1m.cn

[Q34] 每组取第一条
来源：http://ksg.yuanzhike.top

SELECT * FROM (
来源：http://ptd.dianchejie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xvn.snrcjt.cn

) t WHERE rn = 1;
来源：http://kwf.aizwys.cn

[Q35] 内连接
来源：http://num.yj20258888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://liw.wangdashe.top

[Q36] 左连接
来源：http://fbj.andypj.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mim.zycfv.cn

[Q37] 右连接
来源：http://ywa.tianlin.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gko.ehwqpu.com

[Q38] 全外连接（PostgreSQL）
来源：http://gel.yfazqb.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zed.cqqwz.cn

[Q39] 自连接（查上下级）
来源：http://gzn.cqqwz.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://duw.shanyushiyangkeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://enb.xingfuxueyuan.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://zvt.smart0.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tiw.feifeiyinyue.top

[Q41] 多表连接
来源：http://jmt.redwolf501.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://rmv.svipenyu.cn

JOIN users u ON u.id = o.user_id
来源：http://mbf.c1oappe.top

JOIN products p ON p.id = o.product_id;
来源：http://wyl.jqgfzy.top

[Q42] 连接条件附加过滤
来源：http://iwx.redwolf501.top

SELECT u.name, o.amount FROM users u
来源：http://dju.shuidangran.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bjj.daria6918.cn

[Q43] 标量子查询
来源：http://paq.jinqigfzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://eee.xuetiantiany.cn

[Q44] IN 子查询
来源：http://xup.havefunace.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nnh.quarkkingdee.top

[Q45] EXISTS 判断存在
来源：http://jss.zhiwuduotai.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kif.aibaodan.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jjs.gogol.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hxo.fengsongda.top

[Q47] 与平均值比较
来源：http://eqn.iojbl.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fks.hnxiangtu.top

[Q48] CTE 公用表表达式
来源：http://wvt.aizwys.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uov.zdbjq.cn

SELECT * FROM t WHERE c > 5;
来源：http://vre.tanke756.top

[Q49] 更新单行
来源：http://zsi.zhiwuduotai.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ksy.hammf.cn

[Q50] 批量更新
来源：http://afs.cheryme.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xbk.yangfankeji.com

[Q51] 用子查询更新
来源：http://jqg.zhongyouzk.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wih.cqqwz.cn

[Q52] 删除指定行
来源：http://mdh.cqqwz.cn

DELETE FROM users WHERE id = 10;
来源：http://qyq.ivvv.top

[Q53] 按条件删除
来源：http://gvy.dianchejie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rjs.tanke756.top

[Q54] 清空表
来源：http://wjt.fengsongda.top

TRUNCATE TABLE logs;
来源：http://cfx.havefunace.top

[Q55] 排名（并列占位）
来源：http://upp.zhengqikj.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baj.316326.xyz

[Q56] 密集排名（并列不占位）
来源：http://nnj.fktsv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://usr.yuanzhike.top

[Q57] 行号
来源：http://wzn.smart0.xyz


<!-- 参考信息 -->