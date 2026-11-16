代发 wailian999

Py:   itertools.permutations(arr)
来源：http://ldj.wangdashe.top

PHP:  // 手写递归交换
来源：http://axb.yangfankeji.com

JS:   // 手写回溯递归
来源：http://pef.cheryme.top

TS:   // 手写回溯递归
来源：http://qeq.jqgufenzy.top

Java: // 手写回溯递归
来源：http://cft.jyoumei.cn

Go:   // 手写回溯递归
来源：http://bgw.tanke756.top

Ruby: arr.permutation.to_a
来源：http://ers.xingfuxueyuan.xyz

C#:   // 手写回溯递归
来源：http://yrb.kuanghao11.cn

[N09] 栈与队列
来源：http://mfc.zhaomingkeji.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vok.nanxuanxn.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bxl.hywenlv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xwh.tian-w.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://eyg.zdbjq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://opb.sjlbkw.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mdz.yanxiufei.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gav.zhiwuduotai.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ofk.0kj1m.cn

[N10] 链表节点定义
来源：http://jzg.havefunace.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tmy.xingfuxueyuan.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://qdb.tarul.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wec.xingfuxueyuan.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lio.feifeiyinyue.top

Java: class Node { int v; Node next; }
来源：http://myi.feifeiyinyue.top

Go:   type Node struct { V int; Next *Node }
来源：http://irf.cqqwz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yxk.aibaodan.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ctg.zdbjq.cn

[N11] 二叉树中序遍历
来源：http://wyq.xuanzx.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qcj.tianlin.xyz

PHP:  // 手写递归函数
来源：http://fmq.fzhhl.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://swq.xylfe.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cnj.ehwqpu.com

Java: // 手写递归
来源：http://vjh.redwolf501.top

Go:   // 手写递归
来源：http://vpm.jyoumei.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wcu.shanyushiyangtech.top

C#:   // 手写递归
来源：http://ngb.zhoulong.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fdl.hongshengwenyu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pfh.hesvh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qqx.uphjek.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nxo.uphjek.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nck.jinqigfzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rgd.iojbl.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://iej.gogol.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cbf.cheryme.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lli.bbcook.cn

================================================================================
来源：http://ims.hesvh.cn

O. 并发与异步
来源：http://rpv.tarul.cn

================================================================================
来源：http://kos.nwbrower.top

[O01] 启动一个线程
来源：http://kdq.xuanzx.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lhz.yvedp.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lzt.nanxinkj.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://unn.tianlin.xyz

TS:   // 同 JS
来源：http://acd.xinyue.icu

Java: new Thread(() -> f()).start()
来源：http://pnt.yongpay.top

Go:   go f()
来源：http://stc.hesvh.cn

Ruby: Thread.new { f }
来源：http://lyu.zdqjudy.top

C#:   Task.Run(() => F());
来源：http://ywd.shuidangran.top

[O02] 使用线程池
来源：http://wsx.0kj1m.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://grm.wangdashe.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tcu.vqdsnc.cn

JS:   // worker_threads 线程池
来源：http://stm.zhiwuduotai.top

TS:   // worker_threads 线程池
来源：http://wsn.zhixingplan.top

Java: Executors.newFixedThreadPool(4)
来源：http://odk.shanyushiyangtech.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://oel.hywenlv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vha.shuidangran.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ffc.hywenlv.cn

[O03] 加锁保护共享数据
来源：http://zzq.xingfuxueyuan.xyz

Py:   with lock: shared += 1
来源：http://slf.dashuyun.cn

PHP:  // 用 flock() 做文件锁
来源：http://tqs.zhoulong.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kkh.zycfv.cn

TS:   // 同 JS
来源：http://edr.smart0.xyz

Java: synchronized (this) { shared++; }
来源：http://urv.hesvh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sku.zhongyouzk.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://dcl.ydzc1.top

C#:   lock (gate) { shared++; }
来源：http://gac.shanyushiyangkeji.top

[O04] 定义异步函数并等待
来源：http://iuf.iojbl.cn

Py:   async def f():⏎    await g()
来源：http://owr.sxryk.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://oyz.hfpthk.cn

JS:   async function f() { await g(); }
来源：http://ixt.bbcook.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://job.sweek.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bea.fzhhl.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dhp.xylfe.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xev.jinghuilouyu.cn

C#:   async Task F() { await G(); }
来源：http://wiz.cashguo.top

[O05] 并发执行并等待全部完成
来源：http://zzo.dashuyun.cn

Py:   asyncio.gather(*tasks)
来源：http://ugd.fzhhl.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zxm.hnxiangtu.top

JS:   await Promise.all(tasks)
来源：http://gbz.aizwys.cn

TS:   await Promise.all(tasks)
来源：http://naz.jyoumei.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://htf.xinyue.icu

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dof.hysaishi.cn

Ruby: threads.map(&:join)
来源：http://uzw.jqgufenzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://oyf.ydzc1.top

[O06] 使用进程池
来源：http://bzr.xylfe.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nzj.9152youxi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qrr.ydjk.org.cn

JS:   // child_process / cluster 模块
来源：http://tvy.ywan-chungtsiang.top

TS:   // child_process / cluster 模块
来源：http://gkb.daria6918.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qww.gogol.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nuw.xuanzx.com

Ruby: // fork 块
来源：http://dqr.gaohongyu789.top

C#:   Parallel.For
来源：http://mzk.hnqzz.top

================================================================================
来源：http://owh.yanxiufei.cn

P. 常用工具函数
来源：http://guo.zycfv.cn

================================================================================
来源：http://rhl.vehdjk.com

[P01] 生成 UUID
来源：http://ajb.cdnleiting.top

Py:   str(uuid.uuid4())
来源：http://adt.xinyue.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://abm.zdbjq.cn

JS:   crypto.randomUUID()
来源：http://sab.tianlin.xyz

TS:   crypto.randomUUID()
来源：http://fck.ydjk.org.cn

Java: UUID.randomUUID().toString()
来源：http://qfn.zdqjudy.top

Go:   // 用 github.com/google/uuid
来源：http://rvk.shuidangran.top

Ruby: SecureRandom.uuid
来源：http://xty.aizwys.cn

C#:   Guid.NewGuid().ToString()
来源：http://vgb.hesvh.cn

[P02] MD5 / SHA256 摘要
来源：http://hmd.fktsv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ubv.wangshuangyany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gll.daxiang520.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zwt.nanxuanxn.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wch.jinyuanbaomall.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ujr.yvedp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wbg.ehwqpu.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jdc.tarul.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://heg.sjlbkw.cn

[P03] 生成短随机字符串
来源：http://xxi.shangyingyoupin.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://apl.vehdjk.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qyl.yonumen.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xoq.daria6918.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ucd.yj20258.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hli.yongpay.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rcq.yj202588.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://oul.hnqzz.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wfx.wangdashe.top

[P04] 求长度
来源：http://eew.jqgfzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dpi.svipenyu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pnq.ybcxt.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zmm.yangfankeji.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eob.daxiang520.top

Java: list.size();  map.size();  s.length()
来源：http://eml.52xcode.cn

Go:   len(arr);  len(m)
来源：http://ojb.nanxinkj.top

Ruby: x.length;  x.size
来源：http://iyo.xylfe.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://tvf.ppjwa.cn

[P05] 判断两个对象内容是否相等
来源：http://rmk.meibo888.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://yll.ctjpmb.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ixj.xylfe.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uxy.52xcode.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://otr.aibaodan.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mrm.jinqigfzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://esm.andypj.xyz

Ruby: a == b
来源：http://xsx.vehdjk.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://emt.birdmap.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fyg.aizwys.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iiv.wangshuangyany.cn

PHP:  if (empty($x)) {}
来源：http://nth.hywenlv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://guy.gaohongyu789.top

TS:   if (x == null) {}
来源：http://zbc.zhongyouzk.top

Java: if (x == null || x.isEmpty()) {}
来源：http://cjt.sufxvd.cn

Go:   if x == nil {}
来源：http://dtf.nanxinkj.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tff.redwolf501.top

C#:   if (x is null) {}
来源：http://sfq.shangyingyoupin.top

[P07] 防抖与节流
来源：http://oim.aizwys.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bgy.yangfankeji.com

PHP:  // 手写时间戳比较
来源：http://awj.tarul.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uxs.jlsjyb.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xbh.zhongyouzk.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mrv.ehwqpu.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fif.yj202588.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://nmz.zhoulong.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ykr.sufxvd.cn

[P08] 处理浮点精度问题
来源：http://zdq.pycfn.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wpv.guannengcc.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qgf.guannengcc.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cse.gaohongyu789.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fmz.jinyuanbaomall.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://umx.uphjek.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jfv.yfazqb.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zkd.cashguo.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://top.cheryme.top

================================================================================
来源：http://vxa.zhiwuduotai.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dfg.yanxiufei.cn

================================================================================
来源：http://shd.xuetiantiany.cn

[Q01] 创建表
来源：http://jtz.zhoulong.xyz

CREATE TABLE users (
来源：http://ocg.wangshuangyany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bwr.shanyushiyangtech.top

name VARCHAR(50) NOT NULL,
来源：http://rvs.havefunace.top

email VARCHAR(100) UNIQUE,
来源：http://bvv.yuxming.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ufr.zhaomingkeji.xyz

);
来源：http://wad.pycfn.com

[Q02] 创建带外键的表
来源：http://vls.redwolf501.top

CREATE TABLE orders (
来源：http://cgo.jlsjyb.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wyc.hfpthk.cn

user_id INT NOT NULL,
来源：http://bdx.shangyingyoupin.top

amount DECIMAL(10, 2),
来源：http://mog.pycfn.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ilz.epnwcf.com

);
来源：http://zmz.shzxlz.cn

[Q03] 增加列
来源：http://oiq.ivvv.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mem.fengsongda.top

[Q04] 修改列类型
来源：http://qtn.hfpthk.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sry.sysykeji.top

[Q05] 重命名列
来源：http://bmr.dianchejie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ihx.chenlongwang.top

[Q06] 删除列
来源：http://mkn.dashuyun.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xeq.gotoacloud.top

[Q07] 删除表
来源：http://hwp.ybcxt.top

DROP TABLE IF EXISTS orders;
来源：http://rex.andypj.xyz

[Q08] 创建普通索引
来源：http://wyh.gzhubu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://mtb.shangyingyoupin.top

[Q09] 创建唯一索引
来源：http://wbe.zdbjq.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://afp.jlsjyb.cn

[Q10] 插入单行
来源：http://avr.chenzaomai.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://efy.cdnleiting.top

[Q11] 一次插入多行
来源：http://xlx.nanxinkj.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wvx.cqqwz.cn

[Q12] 插入后取自增 ID
来源：http://wlk.sjlbkw.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yeq.jlsjyb.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ohu.xinyue.icu

[Q13] 忽略重复插入
来源：http://jrc.hesvh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wtm.birdmap.top

[Q14] 存在则更新（upsert）
来源：http://nyp.uphjek.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xov.316326.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kqc.shangyingyoupin.top

[Q15] 查询全部
来源：http://and.xylfe.cn

SELECT * FROM users;
来源：http://bgg.shanyushiyangtech.top

[Q16] 查询指定列
来源：http://rbu.fehbvm.com

SELECT id, name FROM users;
来源：http://tkk.shuidangran.top

[Q17] 条件查询
来源：http://eek.xziqi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hvi.zhiwuduotai.top

[Q18] 模糊匹配
来源：http://mdf.cdnleiting.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cah.cdnleiting.top

[Q19] 范围查询
来源：http://ywd.hywenlv.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nxc.aizwys.cn

[Q20] IN 列表
来源：http://lba.hesvh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tap.zhongyouzk.top

[Q21] 空值判断
来源：http://evo.fktsv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://cgy.0kj1m.cn

[Q22] 排序
来源：http://yvw.hammf.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rux.xylfe.cn

[Q23] 分页
来源：http://nxd.gogol.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ggd.jyoumei.cn

[Q24] 去重
来源：http://alr.hfpthk.cn

SELECT DISTINCT city FROM users;
来源：http://fmg.jyoumei.cn

[Q25] 只取前 N 条
来源：http://jxb.zhiwuduotai.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yvy.andypj.xyz

[Q26] 计数
来源：http://nom.uphjek.com

SELECT COUNT(*) FROM users;
来源：http://mjb.nwbrower.top

[Q27] 条件计数
来源：http://rgj.svipenyu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jru.nanxinkj.top

[Q28] 求和与平均
来源：http://mzv.hywenlv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://efe.jiagoushi.top

[Q29] 最大最小值
来源：http://eko.316326.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://tcj.jiagoushi.top

[Q30] 分组统计
来源：http://tbj.xuetiantiany.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cek.xuanzx.com

[Q31] 分组后过滤
来源：http://ugw.jyoumei.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vad.zdbjq.cn

[Q32] 分组拼接字符串
来源：http://ena.ehwqpu.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ymy.daria6918.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fun.chenzaomai.com

[Q33] 多列分组
来源：http://zne.ctjpmb.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qix.chenlongwang.top

[Q34] 每组取第一条
来源：http://noa.yonumen.top

SELECT * FROM (
来源：http://rql.bbcook.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vie.yvedp.cn

) t WHERE rn = 1;
来源：http://xkn.yfazqb.com

[Q35] 内连接
来源：http://pdy.sweek.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uun.xingfuxueyuan.xyz

[Q36] 左连接
来源：http://zeh.hnxiangtu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ksv.hysaishi.cn

[Q37] 右连接
来源：http://jae.chenjidiqi.icu

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ryb.jinqigfzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://cxd.yanxiufei.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fyw.jqgufenzy.top

[Q39] 自连接（查上下级）
来源：http://xgf.cheryme.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://kyw.gzhubu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wen.ydzc1.top

[Q40] 交叉连接（笛卡尔积）
来源：http://kxc.wangshuangyany.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tyl.xziqi.cn

[Q41] 多表连接
来源：http://qup.zhoulong.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://sxo.shzxlz.cn

JOIN users u ON u.id = o.user_id
来源：http://sog.hfpthk.cn

JOIN products p ON p.id = o.product_id;
来源：http://rak.kuanghao11.cn

[Q42] 连接条件附加过滤
来源：http://izh.hysaishi.cn

SELECT u.name, o.amount FROM users u
来源：http://wgr.redwolf501.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hwc.uphjek.com

[Q43] 标量子查询
来源：http://khl.iojbl.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gvl.zhengqikj.top

[Q44] IN 子查询
来源：http://tok.dashuyun.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://aaj.hnxiangtu.top

[Q45] EXISTS 判断存在
来源：http://uxn.sxryk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://inr.hammf.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yvn.smart0.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tvt.pycfn.com

[Q47] 与平均值比较
来源：http://mue.sufxvd.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://aff.shanyushiyangkeji.top

[Q48] CTE 公用表表达式
来源：http://pxf.jqgfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sfj.quarkkingdee.top

SELECT * FROM t WHERE c > 5;
来源：http://mey.hywenlv.cn

[Q49] 更新单行
来源：http://uzk.wangdashe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hjm.birdmap.top

[Q50] 批量更新
来源：http://ygi.316326.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lmw.0kj1m.cn

[Q51] 用子查询更新
来源：http://xsh.dashuyun.cn


<!-- 参考信息 -->