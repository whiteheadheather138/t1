代发 wailian999

Java: // 手写回溯递归
来源：http://aru.kuanghao11.cn

Go:   // 手写回溯递归
来源：http://mfb.mhx1999.top

Ruby: arr.permutation.to_a
来源：http://off.sufxvd.cn

C#:   // 手写回溯递归
来源：http://xrw.hammf.cn

[N09] 栈与队列
来源：http://qio.zhixingplan.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dfv.sufxvd.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://veh.9152youxi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ods.pengpengdd.cyou

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blc.shzxlz.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hpg.bbcook.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wjj.xuetiantiany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wem.cdnleiting.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qjx.dashuyun.cn

[N10] 链表节点定义
来源：http://agk.zhiwuduotai.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vnw.316326.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://bpu.feifeiyinyue.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mmr.fzhhl.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://via.nwbrower.top

Java: class Node { int v; Node next; }
来源：http://pgm.dashuyun.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vce.jinqigfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://knf.wangdashe.top

C#:   class Node { public int V; public Node? Next; }
来源：http://uno.sysykeji.top

[N11] 二叉树中序遍历
来源：http://pvy.yvedp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ure.jinyuanbaomall.cn

PHP:  // 手写递归函数
来源：http://npa.hongshengwenyu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jqg.fzhhl.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tsg.meibo888.top

Java: // 手写递归
来源：http://ngw.shuidangran.top

Go:   // 手写递归
来源：http://qti.jinqigfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://esg.ehwqpu.com

C#:   // 手写递归
来源：http://ypv.tianlin.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bxk.hywenlv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sud.zhoulong.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yqq.yangfankeji.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bdk.hnqzz.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dyo.vehdjk.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iuq.chenzaomai.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sqq.pycfn.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uqb.zhoulong.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vje.fanxiaobao.xyz

================================================================================
来源：http://zqw.kuanghao11.cn

O. 并发与异步
来源：http://nxb.tian-w.cn

================================================================================
来源：http://qmt.zhijiandao.cn

[O01] 启动一个线程
来源：http://miu.shuidangran.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tlf.tianlin.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jsp.nanxuanxn.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ytd.fehbvm.com

TS:   // 同 JS
来源：http://izp.pengpengdd.cyou

Java: new Thread(() -> f()).start()
来源：http://pnw.dashuyun.cn

Go:   go f()
来源：http://cnw.fehbvm.com

Ruby: Thread.new { f }
来源：http://fzh.xziqi.cn

C#:   Task.Run(() => F());
来源：http://asu.yuxming.cn

[O02] 使用线程池
来源：http://xbw.fzhhl.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zoi.vqdsnc.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ogr.havefunace.top

JS:   // worker_threads 线程池
来源：http://ley.fzhhl.top

TS:   // worker_threads 线程池
来源：http://pak.svipenyu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ekm.fktsv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bxt.0kj1m.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bda.shuidangran.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://haq.yj202588.top

[O03] 加锁保护共享数据
来源：http://ijc.vehdjk.com

Py:   with lock: shared += 1
来源：http://nmg.feifeiyinyue.top

PHP:  // 用 flock() 做文件锁
来源：http://bsc.aibaodan.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ced.yj20258.top

TS:   // 同 JS
来源：http://tte.hywenlv.cn

Java: synchronized (this) { shared++; }
来源：http://zpr.jyoumei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://naj.epnwcf.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://ggz.dashuyun.cn

C#:   lock (gate) { shared++; }
来源：http://gpx.yuxming.cn

[O04] 定义异步函数并等待
来源：http://fta.tian-w.cn

Py:   async def f():⏎    await g()
来源：http://mxm.sufxvd.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://upq.hammf.cn

JS:   async function f() { await g(); }
来源：http://puk.tian-w.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qbo.hcnkem.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kxj.zycfv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gfi.daria6918.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fey.hfpthk.cn

C#:   async Task F() { await G(); }
来源：http://jlr.316326.xyz

[O05] 并发执行并等待全部完成
来源：http://pza.shanyushiyangkeji.top

Py:   asyncio.gather(*tasks)
来源：http://sbr.andypj.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tfg.jqgfzy.top

JS:   await Promise.all(tasks)
来源：http://wqd.mhx1999.top

TS:   await Promise.all(tasks)
来源：http://tgy.zhoulong.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gmf.zycfv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qmb.vehdjk.com

Ruby: threads.map(&:join)
来源：http://pvg.guowangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://dsc.dianchejie.cn

[O06] 使用进程池
来源：http://gkq.hnxiangtu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://eyu.haohaochexian.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ton.guannengcc.top

JS:   // child_process / cluster 模块
来源：http://ecb.hnxiangtu.top

TS:   // child_process / cluster 模块
来源：http://ons.hongshengwenyu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ffj.yfazqb.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pmu.shzxlz.cn

Ruby: // fork 块
来源：http://crj.jyoumei.cn

C#:   Parallel.For
来源：http://nrg.ywan-chungtsiang.top

================================================================================
来源：http://qce.xylfe.cn

P. 常用工具函数
来源：http://mtd.zhengqikj.top

================================================================================
来源：http://dyt.chenlongwang.top

[P01] 生成 UUID
来源：http://grw.yj202588.top

Py:   str(uuid.uuid4())
来源：http://luz.nwbrower.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://szl.gotoacloud.top

JS:   crypto.randomUUID()
来源：http://nqq.zhijiandao.cn

TS:   crypto.randomUUID()
来源：http://tvl.ctjpmb.com

Java: UUID.randomUUID().toString()
来源：http://yuc.sjlbkw.cn

Go:   // 用 github.com/google/uuid
来源：http://xcz.shangyingyoupin.top

Ruby: SecureRandom.uuid
来源：http://icp.smart0.xyz

C#:   Guid.NewGuid().ToString()
来源：http://qyp.sxryk.cn

[P02] MD5 / SHA256 摘要
来源：http://dbo.birdmap.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yhu.sweek.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://cog.gzhubu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lfg.yfazqb.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://com.jinqigufen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xlf.fzhhl.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ijh.birdmap.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pji.gaohongyu789.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iid.yfazqb.com

[P03] 生成短随机字符串
来源：http://jok.ydjk.org.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ybr.bbcook.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yku.tian-w.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wej.nanxinkj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fqk.jinyuanbaomall.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mvm.daxiang520.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://oxk.gaohongyu789.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://hwe.hywenlv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ull.cucudq.cn

[P04] 求长度
来源：http://wwd.gaohongyu789.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wwk.cucudq.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yvy.aizwys.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bqm.dianchejie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mcd.aizwys.cn

Java: list.size();  map.size();  s.length()
来源：http://qvz.zhaomingkeji.xyz

Go:   len(arr);  len(m)
来源：http://zkp.0kj1m.cn

Ruby: x.length;  x.size
来源：http://uid.quarkkingdee.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://uep.redwolf501.top

[P05] 判断两个对象内容是否相等
来源：http://ilq.fehbvm.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://xel.yongpay.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://oqe.yonumen.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wup.bbcook.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://egb.kuanghao11.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pck.andypj.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://psx.yfazqb.com

Ruby: a == b
来源：http://eak.yonumen.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ytl.pengpengdd.cyou

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qrw.hysaishi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://chz.birdmap.top

PHP:  if (empty($x)) {}
来源：http://vjp.hysaishi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qtz.yj202588.top

TS:   if (x == null) {}
来源：http://jqf.svipenyu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://all.shanyushiyangtech.top

Go:   if x == nil {}
来源：http://axb.wangshuangyany.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kbd.tarul.cn

C#:   if (x is null) {}
来源：http://vpo.hysaishi.cn

[P07] 防抖与节流
来源：http://vwx.snrcjt.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ebn.dianchejie.cn

PHP:  // 手写时间戳比较
来源：http://yvc.nanxuanxn.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lwr.guannengcc.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lxd.birdmap.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kjf.tian-w.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cxy.zhiwuduotai.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://xym.fehbvm.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mwo.havefunace.top

[P08] 处理浮点精度问题
来源：http://xwj.xziqi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qcf.tanke756.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cuo.pycfn.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vhd.jinqigufen.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dtr.snrcjt.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rvz.zhongyouzk.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rxb.ywan-chungtsiang.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yag.sxryk.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tvc.jiagoushi.top

================================================================================
来源：http://uyb.zhijiandao.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kwi.sweek.top

================================================================================
来源：http://pbl.redwolf501.top

[Q01] 创建表
来源：http://lvp.fanxiaobao.xyz

CREATE TABLE users (
来源：http://dsh.tanke756.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tod.fehbvm.com

name VARCHAR(50) NOT NULL,
来源：http://ogb.316326.xyz

email VARCHAR(100) UNIQUE,
来源：http://knt.xuanzx.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oqx.tianlin.xyz

);
来源：http://wol.jiagoushi.top

[Q02] 创建带外键的表
来源：http://cgp.redwolf501.top

CREATE TABLE orders (
来源：http://ahx.cashguo.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qwr.aizwys.cn

user_id INT NOT NULL,
来源：http://tzy.epnwcf.com

amount DECIMAL(10, 2),
来源：http://mlu.ydzc1.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xvm.hammf.cn

);
来源：http://xdn.fanxiaobao.xyz

[Q03] 增加列
来源：http://xqc.nanxuanxn.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wpv.yueranfly.top

[Q04] 修改列类型
来源：http://hmo.guowangkeji.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wfg.gotoacloud.top

[Q05] 重命名列
来源：http://mdc.meibo888.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fxx.epnwcf.com

[Q06] 删除列
来源：http://buj.fehbvm.com

ALTER TABLE users DROP COLUMN age;
来源：http://cvc.fktsv.cn

[Q07] 删除表
来源：http://hzr.xziqi.cn

DROP TABLE IF EXISTS orders;
来源：http://vit.jinghuilouyu.cn

[Q08] 创建普通索引
来源：http://ykx.ydzc1.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jik.havefunace.top

[Q09] 创建唯一索引
来源：http://bhv.9152youxi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://igt.redwolf501.top

[Q10] 插入单行
来源：http://mop.yonumen.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ppk.snrcjt.cn

[Q11] 一次插入多行
来源：http://bsd.ppjwa.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xsh.jinyuanbaomall.cn

[Q12] 插入后取自增 ID
来源：http://yng.vqdsnc.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fnx.fanxiaobao.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sln.sjlbkw.cn

[Q13] 忽略重复插入
来源：http://yij.cashguo.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://tze.hnxiangtu.top

[Q14] 存在则更新（upsert）
来源：http://gpy.aibaodan.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://snp.cdnleiting.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hgx.hesvh.cn

[Q15] 查询全部
来源：http://kxz.hywenlv.cn

SELECT * FROM users;
来源：http://gpn.sjlbkw.cn

[Q16] 查询指定列
来源：http://vdl.ehwqpu.com

SELECT id, name FROM users;
来源：http://aqd.ctjpmb.com

[Q17] 条件查询
来源：http://nxw.pengpengdd.cyou

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://roi.dianchejie.cn

[Q18] 模糊匹配
来源：http://deu.shangyingyoupin.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://llo.jyoumei.cn

[Q19] 范围查询
来源：http://njt.pycfn.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jrm.havefunace.top

[Q20] IN 列表
来源：http://qxl.svipenyu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://edc.jyoumei.cn

[Q21] 空值判断
来源：http://xxk.feifeiyinyue.top

SELECT * FROM users WHERE email IS NULL;
来源：http://uvg.jianghu66.top

[Q22] 排序
来源：http://jvr.zycfv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://knf.hongshengwenyu.top

[Q23] 分页
来源：http://qnc.wangdashe.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dne.hnqzz.top

[Q24] 去重
来源：http://ixu.zhijiandao.cn

SELECT DISTINCT city FROM users;
来源：http://zzw.daxiang520.top

[Q25] 只取前 N 条
来源：http://fmd.haohaochexian.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uod.havefunace.top

[Q26] 计数
来源：http://bkp.mhx1999.top

SELECT COUNT(*) FROM users;
来源：http://nuw.iojbl.cn

[Q27] 条件计数
来源：http://ubp.pycfn.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kqm.hysaishi.cn

[Q28] 求和与平均
来源：http://uop.shanyushiyangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cnz.0kj1m.cn

[Q29] 最大最小值
来源：http://dbo.xuanzx.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://vot.vqdsnc.cn

[Q30] 分组统计
来源：http://yzi.fehbvm.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cyb.vehdjk.com

[Q31] 分组后过滤
来源：http://lyo.ehwqpu.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rkq.yueranfly.top

[Q32] 分组拼接字符串
来源：http://qap.sufxvd.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fkw.jinqigufen.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://snn.tianlin.xyz

[Q33] 多列分组
来源：http://qiw.jqgufenzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ovz.haohaochexian.top

[Q34] 每组取第一条
来源：http://fsc.zhengqikj.top

SELECT * FROM (
来源：http://cub.cashguo.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xrv.zhaomingkeji.xyz

) t WHERE rn = 1;
来源：http://ntr.smart0.xyz

[Q35] 内连接
来源：http://bpo.nanxuanxn.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wrh.yuanzhike.top

[Q36] 左连接
来源：http://rlk.xinyue.icu

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://aet.xziqi.cn

[Q37] 右连接
来源：http://mqe.hywenlv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wwx.kuanghao11.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lqm.zdqjudy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tut.jiagoushi.top

[Q39] 自连接（查上下级）
来源：http://lak.yuxming.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ney.aizwys.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lps.hywenlv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zxd.shanyushiyangtech.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fng.hysaishi.cn

[Q41] 多表连接
来源：http://kcf.sysykeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://vej.nanxinkj.top

JOIN users u ON u.id = o.user_id
来源：http://fdg.sxryk.cn

JOIN products p ON p.id = o.product_id;
来源：http://mxr.zdqjudy.top

[Q42] 连接条件附加过滤
来源：http://rcn.shuidangran.top

SELECT u.name, o.amount FROM users u
来源：http://vsk.fktsv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nsk.zycfv.cn

[Q43] 标量子查询
来源：http://yng.sjlbkw.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kpw.ydjk.org.cn

[Q44] IN 子查询
来源：http://rje.hysaishi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lmg.zhoulong.xyz

[Q45] EXISTS 判断存在
来源：http://fvd.yuxming.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ttb.smart0.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://jyr.haohaochexian.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kvr.svipenyu.cn

[Q47] 与平均值比较
来源：http://wjr.feifeiyinyue.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ghb.daxiang520.top

[Q48] CTE 公用表表达式
来源：http://yar.zycfv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jzl.cdnleiting.top

SELECT * FROM t WHERE c > 5;
来源：http://fil.meibo888.top

[Q49] 更新单行
来源：http://nvv.sufxvd.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bik.andypj.xyz

[Q50] 批量更新
来源：http://fmf.316326.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rmz.uphjek.com

[Q51] 用子查询更新
来源：http://eev.52xcode.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yfp.jyoumei.cn

[Q52] 删除指定行
来源：http://vgp.sxryk.cn

DELETE FROM users WHERE id = 10;
来源：http://jyv.daria6918.cn

[Q53] 按条件删除
来源：http://rme.fehbvm.com


<!-- 参考信息 -->