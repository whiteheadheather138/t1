代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ehw.zhiwuduotai.top

[N06] 判断回文字符串
来源：http://ybm.ydzc1.top

Py:   s == s[::-1]
来源：http://tqp.quarkkingdee.top

PHP:  $s === strrev($s);
来源：http://pdb.0kj1m.cn

JS:   s === [...s].reverse().join("")
来源：http://wrg.xziqi.cn

TS:   s === [...s].reverse().join("")
来源：http://goc.chenlongwang.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://exg.zhaomingkeji.xyz

Go:   // 双指针从两端比较
来源：http://buo.jinqigufen.top

Ruby: s == s.reverse
来源：http://pyi.xziqi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://icq.jianghu66.top

[N07] 两数之和（返回下标）
来源：http://wfx.epnwcf.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://org.yuanzhike.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cry.hywenlv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://czf.zhengqikj.top

TS:   // 手写 Map<string, number>
来源：http://owu.cucudq.cn

Java: // 手写 HashMap
来源：http://lii.9152youxi.cn

Go:   // 手写 map[int]int
来源：http://oto.guowangkeji.top

Ruby: // 手写 Hash
来源：http://jes.dashuyun.cn

C#:   // 手写 Dictionary<int, int>
来源：http://csa.vqdsnc.cn

[N08] 生成全排列
来源：http://oyj.zhoulong.xyz

Py:   itertools.permutations(arr)
来源：http://trn.shuidangran.top

PHP:  // 手写递归交换
来源：http://luk.ybcxt.top

JS:   // 手写回溯递归
来源：http://dxm.tarul.cn

TS:   // 手写回溯递归
来源：http://bnl.dashuyun.cn

Java: // 手写回溯递归
来源：http://zck.guowangkeji.top

Go:   // 手写回溯递归
来源：http://zup.guowangkeji.top

Ruby: arr.permutation.to_a
来源：http://qaw.gaohongyu789.top

C#:   // 手写回溯递归
来源：http://wlx.shzxlz.cn

[N09] 栈与队列
来源：http://jsd.shanyushiyangkeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dhc.bjfxy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qjt.shuidangran.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mww.vqdsnc.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://slc.hcnkem.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://utg.shuidangran.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jpv.hywenlv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bmg.meibo888.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wos.ywan-chungtsiang.top

[N10] 链表节点定义
来源：http://dke.fanxiaobao.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lwi.tianlin.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://seq.hammf.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dkf.316326.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hls.shzxlz.cn

Java: class Node { int v; Node next; }
来源：http://wod.yanxiufei.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ysg.hfpthk.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://iaj.cqqwz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mct.wangdashe.top

[N11] 二叉树中序遍历
来源：http://zoz.yvedp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bcn.wangshuangyany.cn

PHP:  // 手写递归函数
来源：http://rna.9152youxi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xha.redwolf501.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pwc.yj20258.top

Java: // 手写递归
来源：http://tjp.fktsv.cn

Go:   // 手写递归
来源：http://mmb.zhengqikj.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ugr.daxiang520.top

C#:   // 手写递归
来源：http://vsu.andypj.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cnr.tian-w.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bba.ivvv.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pzj.vehdjk.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sqz.xziqi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jpc.sweek.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cmd.yvedp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vgv.jinqigufen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pqi.hnxiangtu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qec.wangshuangyany.cn

================================================================================
来源：http://swx.pycfn.com

O. 并发与异步
来源：http://zec.9152youxi.cn

================================================================================
来源：http://wqb.yj202588.top

[O01] 启动一个线程
来源：http://kuf.0kj1m.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cvy.shzxlz.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kqc.jqgfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kia.shanyushiyangtech.top

TS:   // 同 JS
来源：http://clx.316326.xyz

Java: new Thread(() -> f()).start()
来源：http://khy.hfpthk.cn

Go:   go f()
来源：http://uuv.zhengqikj.top

Ruby: Thread.new { f }
来源：http://yup.andypj.xyz

C#:   Task.Run(() => F());
来源：http://agf.zhixingplan.top

[O02] 使用线程池
来源：http://hkl.svipenyu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yic.cashguo.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xnf.guannengcc.top

JS:   // worker_threads 线程池
来源：http://vam.gzhubu.top

TS:   // worker_threads 线程池
来源：http://opm.gogol.net.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nvk.hongshengwenyu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mbb.yuanzhike.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jps.tanke756.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tlt.chenjidiqi.icu

[O03] 加锁保护共享数据
来源：http://ord.jinyuanbaomall.cn

Py:   with lock: shared += 1
来源：http://din.jianghu66.top

PHP:  // 用 flock() 做文件锁
来源：http://glg.zhiwuduotai.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://knf.shzxlz.cn

TS:   // 同 JS
来源：http://bky.yangfankeji.com

Java: synchronized (this) { shared++; }
来源：http://itb.mhx1999.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hfs.tarul.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://eea.hesvh.cn

C#:   lock (gate) { shared++; }
来源：http://awb.hcnkem.com

[O04] 定义异步函数并等待
来源：http://err.xziqi.cn

Py:   async def f():⏎    await g()
来源：http://ydi.ydzc1.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fkm.snrcjt.cn

JS:   async function f() { await g(); }
来源：http://xki.aizwys.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kwd.hongshengwenyu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hne.wangshuangyany.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fqr.zhiwuduotai.top

Ruby: # 用 Fiber 或 async gem
来源：http://vyp.gaohongyu789.top

C#:   async Task F() { await G(); }
来源：http://kup.fehbvm.com

[O05] 并发执行并等待全部完成
来源：http://hks.iojbl.cn

Py:   asyncio.gather(*tasks)
来源：http://kea.hnqzz.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hzm.sjlbkw.cn

JS:   await Promise.all(tasks)
来源：http://iim.zhiwuduotai.top

TS:   await Promise.all(tasks)
来源：http://fjr.fehbvm.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://czq.fzhhl.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yjy.hesvh.cn

Ruby: threads.map(&:join)
来源：http://cxn.ppjwa.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ypv.shangyingyoupin.top

[O06] 使用进程池
来源：http://rft.svipenyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jor.jyoumei.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://scl.xinyue.icu

JS:   // child_process / cluster 模块
来源：http://qma.iojbl.cn

TS:   // child_process / cluster 模块
来源：http://qzr.316326.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://twq.fanxiaobao.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ywj.quarkkingdee.top

Ruby: // fork 块
来源：http://qlq.yuanzhike.top

C#:   Parallel.For
来源：http://jbj.ybcxt.top

================================================================================
来源：http://koa.birdmap.top

P. 常用工具函数
来源：http://lpc.0kj1m.cn

================================================================================
来源：http://qlj.hesvh.cn

[P01] 生成 UUID
来源：http://tgz.gaohongyu789.top

Py:   str(uuid.uuid4())
来源：http://mdo.c1oappe.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qrp.sxryk.cn

JS:   crypto.randomUUID()
来源：http://bvs.9152youxi.cn

TS:   crypto.randomUUID()
来源：http://qpv.zdqjudy.top

Java: UUID.randomUUID().toString()
来源：http://pgv.316326.xyz

Go:   // 用 github.com/google/uuid
来源：http://gtq.chenlongwang.top

Ruby: SecureRandom.uuid
来源：http://eug.ydzc1.top

C#:   Guid.NewGuid().ToString()
来源：http://wxx.epnwcf.com

[P02] MD5 / SHA256 摘要
来源：http://vvf.hysaishi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ugr.bjfxy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wcf.uphjek.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mag.yonumen.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://skl.yuxming.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fqc.jqgufenzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hgu.sxryk.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qmh.birdmap.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jjd.316326.xyz

[P03] 生成短随机字符串
来源：http://ese.bbcook.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://syt.sxryk.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sze.xinyue.icu

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bel.gaohongyu789.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zfl.zdqjudy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uqy.jyoumei.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wdk.guowangkeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rfo.yangfankeji.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tbu.vehdjk.com

[P04] 求长度
来源：http://ejz.c1oappe.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jnf.guowangkeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oxh.chenlongwang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ohc.feifeiyinyue.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kzl.yvedp.cn

Java: list.size();  map.size();  s.length()
来源：http://mcj.hcnkem.com

Go:   len(arr);  len(m)
来源：http://aqc.xuetiantiany.cn

Ruby: x.length;  x.size
来源：http://pmo.smart0.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://jbj.meibo888.top

[P05] 判断两个对象内容是否相等
来源：http://rmh.sjlbkw.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ten.smart0.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://noi.wangshuangyany.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://njk.snrcjt.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dmk.quarkkingdee.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cgh.wangdashe.top

Go:   reflect.DeepEqual(a, b)
来源：http://fqr.cucudq.cn

Ruby: a == b
来源：http://gzy.tian-w.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mwu.hcnkem.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jyh.cqqwz.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mqf.ivvv.top

PHP:  if (empty($x)) {}
来源：http://lzf.zdqjudy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gol.sjlbkw.cn

TS:   if (x == null) {}
来源：http://iaw.gotoacloud.top

Java: if (x == null || x.isEmpty()) {}
来源：http://jpz.cashguo.top

Go:   if x == nil {}
来源：http://ckz.epnwcf.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gxi.guowangkeji.top

C#:   if (x is null) {}
来源：http://ycv.snrcjt.cn

[P07] 防抖与节流
来源：http://rzv.sufxvd.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oih.shuidangran.top

PHP:  // 手写时间戳比较
来源：http://qfq.yuxming.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bua.zhixingplan.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://efk.jqgufenzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://imv.haohaochexian.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ofk.shanyushiyangkeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://kmi.xylfe.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rwm.zhixingplan.top

[P08] 处理浮点精度问题
来源：http://bri.iojbl.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jcp.birdmap.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cwv.gaohongyu789.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hky.ydzc1.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ctz.gotoacloud.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pkp.yongpay.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iba.zhijiandao.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gxq.mhx1999.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sgh.ctjpmb.com

================================================================================
来源：http://exj.cheryme.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pku.pengpengdd.cyou

================================================================================
来源：http://uzq.gzhubu.top

[Q01] 创建表
来源：http://vzl.snrcjt.cn

CREATE TABLE users (
来源：http://stf.ybcxt.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iak.chenlongwang.top

name VARCHAR(50) NOT NULL,
来源：http://qcx.nanxinkj.top

email VARCHAR(100) UNIQUE,
来源：http://jhk.nanxinkj.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qqb.wangdashe.top

);
来源：http://wus.snrcjt.cn

[Q02] 创建带外键的表
来源：http://djm.snrcjt.cn

CREATE TABLE orders (
来源：http://tax.gzhubu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yvp.vehdjk.com

user_id INT NOT NULL,
来源：http://dqk.dashuyun.cn

amount DECIMAL(10, 2),
来源：http://lbi.xziqi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ndd.jqgufenzy.top

);
来源：http://uok.zdbjq.cn

[Q03] 增加列
来源：http://men.sysykeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gxu.sysykeji.top

[Q04] 修改列类型
来源：http://bhh.pengpengdd.cyou

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://clv.sxryk.cn

[Q05] 重命名列
来源：http://lvd.bjfxy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://grn.hesvh.cn

[Q06] 删除列
来源：http://dxp.gzhubu.top

ALTER TABLE users DROP COLUMN age;
来源：http://hip.yonumen.top

[Q07] 删除表
来源：http://syb.wangdashe.top

DROP TABLE IF EXISTS orders;
来源：http://vws.gogol.net.cn

[Q08] 创建普通索引
来源：http://cuk.zdbjq.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://afr.chenzaomai.com

[Q09] 创建唯一索引
来源：http://bma.c1oappe.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dkz.bjfxy.top

[Q10] 插入单行
来源：http://duh.jiagoushi.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://urz.ydjk.org.cn

[Q11] 一次插入多行
来源：http://itr.fehbvm.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zbj.zhijiandao.cn

[Q12] 插入后取自增 ID
来源：http://nzt.c1oappe.top

INSERT INTO users (name) VALUES ('C');
来源：http://fmv.hcnkem.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qvh.ehwqpu.com

[Q13] 忽略重复插入
来源：http://oyr.guannengcc.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://imu.yj20258.top

[Q14] 存在则更新（upsert）
来源：http://gxg.birdmap.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qjt.aizwys.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hav.yanxiufei.cn

[Q15] 查询全部
来源：http://nzx.svipenyu.cn

SELECT * FROM users;
来源：http://xpi.yanxiufei.cn

[Q16] 查询指定列
来源：http://ahq.ydzc1.top

SELECT id, name FROM users;
来源：http://vju.tanke756.top

[Q17] 条件查询
来源：http://eky.zhiwuduotai.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://axl.smart0.xyz

[Q18] 模糊匹配
来源：http://czs.cucudq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://frz.xingfuxueyuan.xyz

[Q19] 范围查询
来源：http://xyy.ybcxt.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jen.gaohongyu789.top

[Q20] IN 列表
来源：http://esx.tarul.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jln.daxiang520.top

[Q21] 空值判断
来源：http://sly.vqdsnc.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fuh.xuanzx.com

[Q22] 排序
来源：http://vkt.tianlin.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qpb.shangyingyoupin.top

[Q23] 分页
来源：http://fmg.aizwys.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rzy.c1oappe.top

[Q24] 去重
来源：http://ioa.tanke756.top

SELECT DISTINCT city FROM users;
来源：http://qgy.pengpengdd.cyou

[Q25] 只取前 N 条
来源：http://mcy.tanke756.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://npg.zhijiandao.cn

[Q26] 计数
来源：http://czi.xuanzx.com

SELECT COUNT(*) FROM users;
来源：http://knf.chenjidiqi.icu

[Q27] 条件计数
来源：http://ipu.sufxvd.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yhc.xuanzx.com

[Q28] 求和与平均
来源：http://gyo.xingfuxueyuan.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qnc.snrcjt.cn

[Q29] 最大最小值
来源：http://fer.zhoulong.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://ymd.andypj.xyz

[Q30] 分组统计
来源：http://ghv.wangdashe.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cus.nanxinkj.top

[Q31] 分组后过滤
来源：http://jdh.tarul.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bqc.snrcjt.cn

[Q32] 分组拼接字符串
来源：http://fgx.redwolf501.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zar.chenzaomai.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wpm.sweek.top

[Q33] 多列分组
来源：http://ugu.svipenyu.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ebe.ybcxt.top

[Q34] 每组取第一条
来源：http://lqu.hnxiangtu.top

SELECT * FROM (
来源：http://acf.cucudq.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://aea.zdbjq.cn

) t WHERE rn = 1;
来源：http://bwz.ybcxt.top

[Q35] 内连接
来源：http://jxm.yfazqb.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://joz.nanxinkj.top

[Q36] 左连接
来源：http://dlg.meibo888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hny.gogol.net.cn

[Q37] 右连接
来源：http://nan.hnqzz.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ycm.gaohongyu789.top

[Q38] 全外连接（PostgreSQL）
来源：http://vyj.uphjek.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uoo.xziqi.cn

[Q39] 自连接（查上下级）
来源：http://grw.pycfn.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://iwh.fehbvm.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gcm.chenjidiqi.icu

[Q40] 交叉连接（笛卡尔积）
来源：http://sfc.aibaodan.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ogi.sysykeji.top

[Q41] 多表连接
来源：http://ozi.gogol.net.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://gut.hnqzz.top

JOIN users u ON u.id = o.user_id
来源：http://atp.feifeiyinyue.top

JOIN products p ON p.id = o.product_id;
来源：http://ssw.xuetiantiany.cn

[Q42] 连接条件附加过滤
来源：http://ihs.hammf.cn


<!-- 参考信息 -->