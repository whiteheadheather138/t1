代发 wailian999

Java: // 手写回溯递归
来源：http://zuz.zhiwuduotai.top

Go:   // 手写回溯递归
来源：http://crv.ydjk.org.cn

Ruby: arr.permutation.to_a
来源：http://dep.jianghu66.top

C#:   // 手写回溯递归
来源：http://sun.hnqzz.top

[N09] 栈与队列
来源：http://sfy.jqgufenzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cpd.vqdsnc.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lzh.sxryk.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jcq.zhixingplan.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cfs.zdbjq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qvo.xingfuxueyuan.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cga.ydzc1.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gmr.hnxiangtu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://djp.xuanzx.com

[N10] 链表节点定义
来源：http://fbf.yanxiufei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://flc.kuanghao11.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://oyq.shanyushiyangkeji.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pxc.vqdsnc.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://eqf.birdmap.top

Java: class Node { int v; Node next; }
来源：http://vkr.pengpengdd.cyou

Go:   type Node struct { V int; Next *Node }
来源：http://tbm.svipenyu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jfa.hywenlv.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://scg.ydjk.org.cn

[N11] 二叉树中序遍历
来源：http://kur.nwbrower.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zgc.pycfn.com

PHP:  // 手写递归函数
来源：http://lbn.xinyue.icu

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://llq.ydzc1.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kge.cucudq.cn

Java: // 手写递归
来源：http://ykb.jianghu66.top

Go:   // 手写递归
来源：http://hta.fktsv.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bfr.andypj.xyz

C#:   // 手写递归
来源：http://fup.yueranfly.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zch.shzxlz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wln.xinyue.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kkd.feifeiyinyue.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dqp.havefunace.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uem.sxryk.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xgn.xylfe.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xzn.jqgufenzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rac.yuxming.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://auk.daria6918.cn

================================================================================
来源：http://efi.meibo888.top

O. 并发与异步
来源：http://jxh.sysykeji.top

================================================================================
来源：http://zhk.ydjk.org.cn

[O01] 启动一个线程
来源：http://hft.cheryme.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://aze.birdmap.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://orm.epnwcf.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jtt.chenzaomai.com

TS:   // 同 JS
来源：http://okw.jianghu66.top

Java: new Thread(() -> f()).start()
来源：http://wuf.aibaodan.cn

Go:   go f()
来源：http://kgz.haohaochexian.top

Ruby: Thread.new { f }
来源：http://hwg.yonumen.top

C#:   Task.Run(() => F());
来源：http://xll.nanxinkj.top

[O02] 使用线程池
来源：http://nbm.aibaodan.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ngt.xuetiantiany.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://edl.yj20258.top

JS:   // worker_threads 线程池
来源：http://jka.guannengcc.top

TS:   // worker_threads 线程池
来源：http://jyj.xuanzx.com

Java: Executors.newFixedThreadPool(4)
来源：http://yen.zhengqikj.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jkr.jlsjyb.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bjw.bbcook.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lnw.hysaishi.cn

[O03] 加锁保护共享数据
来源：http://rss.jqgfzy.top

Py:   with lock: shared += 1
来源：http://glz.sweek.top

PHP:  // 用 flock() 做文件锁
来源：http://nvx.meibo888.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kon.vqdsnc.cn

TS:   // 同 JS
来源：http://ehr.gotoacloud.top

Java: synchronized (this) { shared++; }
来源：http://zuy.xuetiantiany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jzg.fanxiaobao.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://wuo.ivvv.top

C#:   lock (gate) { shared++; }
来源：http://yja.zhoulong.xyz

[O04] 定义异步函数并等待
来源：http://dmt.daria6918.cn

Py:   async def f():⏎    await g()
来源：http://dpc.zhongyouzk.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zyj.dianchejie.cn

JS:   async function f() { await g(); }
来源：http://rvj.hammf.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tbt.ctjpmb.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ukm.mhx1999.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cxo.jiagoushi.top

Ruby: # 用 Fiber 或 async gem
来源：http://mpp.c1oappe.top

C#:   async Task F() { await G(); }
来源：http://rqe.guannengcc.top

[O05] 并发执行并等待全部完成
来源：http://sde.bbcook.cn

Py:   asyncio.gather(*tasks)
来源：http://tsg.bjfxy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://igj.zhengqikj.top

JS:   await Promise.all(tasks)
来源：http://dzs.hfpthk.cn

TS:   await Promise.all(tasks)
来源：http://eig.ydjk.org.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ldo.jlsjyb.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gat.daria6918.cn

Ruby: threads.map(&:join)
来源：http://bsq.gotoacloud.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mlh.tanke756.top

[O06] 使用进程池
来源：http://zam.dianchejie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fmn.havefunace.top

PHP:  // pcntl_fork 或多进程队列
来源：http://kgx.yfazqb.com

JS:   // child_process / cluster 模块
来源：http://pgl.cdnleiting.top

TS:   // child_process / cluster 模块
来源：http://gtp.iojbl.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bkk.feifeiyinyue.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lxz.hfpthk.cn

Ruby: // fork 块
来源：http://hty.epnwcf.com

C#:   Parallel.For
来源：http://pcr.zhaomingkeji.xyz

================================================================================
来源：http://bkw.dashuyun.cn

P. 常用工具函数
来源：http://pbz.gaohongyu789.top

================================================================================
来源：http://lum.quarkkingdee.top

[P01] 生成 UUID
来源：http://ait.cucudq.cn

Py:   str(uuid.uuid4())
来源：http://bbw.ivvv.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://odf.ydzc1.top

JS:   crypto.randomUUID()
来源：http://ecs.jqgufenzy.top

TS:   crypto.randomUUID()
来源：http://bjm.svipenyu.cn

Java: UUID.randomUUID().toString()
来源：http://mep.fehbvm.com

Go:   // 用 github.com/google/uuid
来源：http://clb.hnxiangtu.top

Ruby: SecureRandom.uuid
来源：http://ytx.hnqzz.top

C#:   Guid.NewGuid().ToString()
来源：http://lqs.cqqwz.cn

[P02] MD5 / SHA256 摘要
来源：http://vwt.yonumen.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ngk.ydzc1.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://bcz.haohaochexian.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rew.yueranfly.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fnb.guowangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hzz.ivvv.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://afw.fktsv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hfy.cucudq.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://eyr.jqgufenzy.top

[P03] 生成短随机字符串
来源：http://zox.dianchejie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ccy.zhixingplan.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pvv.jinghuilouyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fxo.hfpthk.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://twe.0kj1m.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wdy.xuanzx.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bgu.zdqjudy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xhx.cqqwz.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ewc.fanxiaobao.xyz

[P04] 求长度
来源：http://ber.havefunace.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pov.cqqwz.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uqp.ywan-chungtsiang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://szn.yuanzhike.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wea.nwbrower.top

Java: list.size();  map.size();  s.length()
来源：http://uvy.smart0.xyz

Go:   len(arr);  len(m)
来源：http://bds.andypj.xyz

Ruby: x.length;  x.size
来源：http://vzp.zhiwuduotai.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://say.hcnkem.com

[P05] 判断两个对象内容是否相等
来源：http://uop.hcnkem.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://aoc.gogol.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rgu.ppjwa.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dzy.xuanzx.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wrt.nwbrower.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mbq.tian-w.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kqg.316326.xyz

Ruby: a == b
来源：http://pjg.yuxming.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://svn.yongpay.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://anf.wangshuangyany.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zim.hesvh.cn

PHP:  if (empty($x)) {}
来源：http://wix.hfpthk.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ame.jinqigufen.top

TS:   if (x == null) {}
来源：http://emz.cucudq.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gyt.gaohongyu789.top

Go:   if x == nil {}
来源：http://pqr.bbcook.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qbq.hnxiangtu.top

C#:   if (x is null) {}
来源：http://anz.0kj1m.cn

[P07] 防抖与节流
来源：http://hml.hesvh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lcl.fzhhl.top

PHP:  // 手写时间戳比较
来源：http://vpr.tianlin.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jla.jinyuanbaomall.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dck.316326.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dai.sysykeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gbg.zhijiandao.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wwh.nanxuanxn.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bgx.hysaishi.cn

[P08] 处理浮点精度问题
来源：http://uae.ybcxt.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yej.wangdashe.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kxm.cashguo.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xet.yuxming.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://itw.tarul.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qlp.fehbvm.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lur.birdmap.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gpp.hongshengwenyu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://izy.chenjidiqi.icu

================================================================================
来源：http://vtx.zhongyouzk.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ivy.xingfuxueyuan.xyz

================================================================================
来源：http://xwu.wangshuangyany.cn

[Q01] 创建表
来源：http://lez.hnxiangtu.top

CREATE TABLE users (
来源：http://bmd.yvedp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://geb.smart0.xyz

name VARCHAR(50) NOT NULL,
来源：http://nwi.tian-w.cn

email VARCHAR(100) UNIQUE,
来源：http://vwb.redwolf501.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mdv.hfpthk.cn

);
来源：http://dds.andypj.xyz

[Q02] 创建带外键的表
来源：http://ymi.gaohongyu789.top

CREATE TABLE orders (
来源：http://bpe.fengsongda.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://esr.chenjidiqi.icu

user_id INT NOT NULL,
来源：http://mbo.meibo888.top

amount DECIMAL(10, 2),
来源：http://wpu.0kj1m.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jps.quarkkingdee.top

);
来源：http://szs.xingfuxueyuan.xyz

[Q03] 增加列
来源：http://jgs.sufxvd.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bix.jinqigufen.top

[Q04] 修改列类型
来源：http://cvs.jlsjyb.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dzt.cashguo.top

[Q05] 重命名列
来源：http://ldi.gogol.net.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dfp.jyoumei.cn

[Q06] 删除列
来源：http://kat.xziqi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rlp.ybcxt.top

[Q07] 删除表
来源：http://fdv.gzhubu.top

DROP TABLE IF EXISTS orders;
来源：http://fzv.yonumen.top

[Q08] 创建普通索引
来源：http://maj.wangdashe.top

CREATE INDEX idx_users_email ON users(email);
来源：http://sym.bjfxy.top

[Q09] 创建唯一索引
来源：http://rpa.52xcode.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hza.zhiwuduotai.top

[Q10] 插入单行
来源：http://ulc.ivvv.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wix.hywenlv.cn

[Q11] 一次插入多行
来源：http://cjr.shuidangran.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nrb.sufxvd.cn

[Q12] 插入后取自增 ID
来源：http://zgi.yuanzhike.top

INSERT INTO users (name) VALUES ('C');
来源：http://uhj.bjfxy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://inf.xylfe.cn

[Q13] 忽略重复插入
来源：http://jvx.jianghu66.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zpa.zhiwuduotai.top

[Q14] 存在则更新（upsert）
来源：http://byf.zdbjq.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fhf.hnxiangtu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dma.hesvh.cn

[Q15] 查询全部
来源：http://grt.jinyuanbaomall.cn

SELECT * FROM users;
来源：http://wfs.nanxinkj.top

[Q16] 查询指定列
来源：http://rmp.quarkkingdee.top

SELECT id, name FROM users;
来源：http://qth.yueranfly.top

[Q17] 条件查询
来源：http://zps.jinqigfzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dld.pycfn.com

[Q18] 模糊匹配
来源：http://shn.tanke756.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xoz.fktsv.cn

[Q19] 范围查询
来源：http://zro.xinyue.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://axj.mhx1999.top

[Q20] IN 列表
来源：http://jna.yj20258888.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rpl.guowangkeji.top

[Q21] 空值判断
来源：http://csw.jqgufenzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://jow.jlsjyb.cn

[Q22] 排序
来源：http://mpt.feifeiyinyue.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xcg.xingfuxueyuan.xyz

[Q23] 分页
来源：http://avf.ehwqpu.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wqa.hysaishi.cn

[Q24] 去重
来源：http://vig.gotoacloud.top

SELECT DISTINCT city FROM users;
来源：http://iqf.shanyushiyangkeji.top

[Q25] 只取前 N 条
来源：http://olz.wangshuangyany.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://snp.sjlbkw.cn

[Q26] 计数
来源：http://ikw.epnwcf.com

SELECT COUNT(*) FROM users;
来源：http://tkn.ppjwa.cn

[Q27] 条件计数
来源：http://vok.fanxiaobao.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://epr.tian-w.cn

[Q28] 求和与平均
来源：http://uto.hywenlv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gji.cucudq.cn

[Q29] 最大最小值
来源：http://hhd.shangyingyoupin.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://hqm.epnwcf.com

[Q30] 分组统计
来源：http://cxk.cdnleiting.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mex.ywan-chungtsiang.top

[Q31] 分组后过滤
来源：http://vac.xylfe.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://awv.jinyuanbaomall.cn

[Q32] 分组拼接字符串
来源：http://qon.316326.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jpp.sweek.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://htl.snrcjt.cn

[Q33] 多列分组
来源：http://euf.zhixingplan.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dct.uphjek.com

[Q34] 每组取第一条
来源：http://yqt.jqgfzy.top

SELECT * FROM (
来源：http://dpl.yuxming.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vcl.jinghuilouyu.cn

) t WHERE rn = 1;
来源：http://nmx.yvedp.cn

[Q35] 内连接
来源：http://uyv.xylfe.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ihf.zhongyouzk.top

[Q36] 左连接
来源：http://vuq.guannengcc.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ccy.zhaomingkeji.xyz

[Q37] 右连接
来源：http://wwh.9152youxi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mzd.yuxming.cn

[Q38] 全外连接（PostgreSQL）
来源：http://pfw.shanyushiyangtech.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uqj.kuanghao11.cn

[Q39] 自连接（查上下级）
来源：http://yxd.nanxuanxn.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://bak.daxiang520.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yki.shanyushiyangtech.top

[Q40] 交叉连接（笛卡尔积）
来源：http://lce.hnxiangtu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ceb.fengsongda.top

[Q41] 多表连接
来源：http://xmu.shanyushiyangtech.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ofg.zdbjq.cn

JOIN users u ON u.id = o.user_id
来源：http://chw.nanxuanxn.top

JOIN products p ON p.id = o.product_id;
来源：http://rev.yuanzhike.top

[Q42] 连接条件附加过滤
来源：http://xfd.jinqigfzy.top

SELECT u.name, o.amount FROM users u
来源：http://wtp.zhaomingkeji.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cfa.cqqwz.cn

[Q43] 标量子查询
来源：http://nzd.haohaochexian.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://may.0kj1m.cn

[Q44] IN 子查询
来源：http://fbk.tanke756.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://krf.yj20258888.top

[Q45] EXISTS 判断存在
来源：http://xdi.pengpengdd.cyou

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yky.hesvh.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sqn.birdmap.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mac.zdbjq.cn

[Q47] 与平均值比较
来源：http://iuc.zdbjq.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nri.havefunace.top

[Q48] CTE 公用表表达式
来源：http://vbj.tian-w.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pkt.svipenyu.cn

SELECT * FROM t WHERE c > 5;
来源：http://gfu.zycfv.cn

[Q49] 更新单行
来源：http://mav.cucudq.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lii.quarkkingdee.top

[Q50] 批量更新
来源：http://cih.jlsjyb.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://thk.pycfn.com

[Q51] 用子查询更新
来源：http://fmo.jianghu66.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bnc.aizwys.cn

[Q52] 删除指定行
来源：http://kgw.hnxiangtu.top

DELETE FROM users WHERE id = 10;
来源：http://cui.chenjidiqi.icu

[Q53] 按条件删除
来源：http://acd.iojbl.cn


<!-- 参考信息 -->