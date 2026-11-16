代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://akk.shanyushiyangkeji.top

[N06] 判断回文字符串
来源：http://aum.tianlin.xyz

Py:   s == s[::-1]
来源：http://uiz.nwbrower.top

PHP:  $s === strrev($s);
来源：http://liq.wangshuangyany.cn

JS:   s === [...s].reverse().join("")
来源：http://gap.jianghu66.top

TS:   s === [...s].reverse().join("")
来源：http://dus.zhaomingkeji.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bay.pengpengdd.cyou

Go:   // 双指针从两端比较
来源：http://nob.chenjidiqi.icu

Ruby: s == s.reverse
来源：http://day.ivvv.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ypg.fktsv.cn

[N07] 两数之和（返回下标）
来源：http://rtn.yongpay.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lng.shzxlz.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://djx.gzhubu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://fsx.xingfuxueyuan.xyz

TS:   // 手写 Map<string, number>
来源：http://kcp.ydjk.org.cn

Java: // 手写 HashMap
来源：http://vyz.jinqigufen.top

Go:   // 手写 map[int]int
来源：http://oao.chenjidiqi.icu

Ruby: // 手写 Hash
来源：http://vyw.0kj1m.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ntn.aibaodan.cn

[N08] 生成全排列
来源：http://lyd.hfpthk.cn

Py:   itertools.permutations(arr)
来源：http://ddg.jianghu66.top

PHP:  // 手写递归交换
来源：http://ovh.chenlongwang.top

JS:   // 手写回溯递归
来源：http://ueo.cashguo.top

TS:   // 手写回溯递归
来源：http://onc.sysykeji.top

Java: // 手写回溯递归
来源：http://fji.jinghuilouyu.cn

Go:   // 手写回溯递归
来源：http://nmo.xinyue.icu

Ruby: arr.permutation.to_a
来源：http://ylp.ywan-chungtsiang.top

C#:   // 手写回溯递归
来源：http://cmn.kuanghao11.cn

[N09] 栈与队列
来源：http://fkn.sysykeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ohq.xingfuxueyuan.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xdd.andypj.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dji.shanyushiyangtech.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hvr.shanyushiyangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dfs.yangfankeji.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fzy.svipenyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vfe.aibaodan.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iuj.hysaishi.cn

[N10] 链表节点定义
来源：http://geo.dashuyun.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uhr.gotoacloud.top

PHP:  class Node { public $v; public $next = null; }
来源：http://atr.bbcook.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sud.cqqwz.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tvm.xylfe.cn

Java: class Node { int v; Node next; }
来源：http://dtu.yuanzhike.top

Go:   type Node struct { V int; Next *Node }
来源：http://avj.daxiang520.top

Ruby: Node = Struct.new(:v, :next)
来源：http://uqw.yj20258.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ssm.fengsongda.top

[N11] 二叉树中序遍历
来源：http://lxf.jinghuilouyu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pul.sufxvd.cn

PHP:  // 手写递归函数
来源：http://deh.gzhubu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jbk.dianchejie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iii.zhiwuduotai.top

Java: // 手写递归
来源：http://dov.9152youxi.cn

Go:   // 手写递归
来源：http://ghz.zhongyouzk.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rtt.sysykeji.top

C#:   // 手写递归
来源：http://gvw.tianlin.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hva.guowangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ocr.jinghuilouyu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xps.jinghuilouyu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fai.yj202588.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sce.hcnkem.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uuq.yj20258888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://whg.xingfuxueyuan.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zlq.hywenlv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uxl.9152youxi.cn

================================================================================
来源：http://qrs.9152youxi.cn

O. 并发与异步
来源：http://usy.hammf.cn

================================================================================
来源：http://azc.c1oappe.top

[O01] 启动一个线程
来源：http://ccs.chenlongwang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ldj.jqgufenzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yda.jlsjyb.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xud.sjlbkw.cn

TS:   // 同 JS
来源：http://mxg.pycfn.com

Java: new Thread(() -> f()).start()
来源：http://xtd.shanyushiyangkeji.top

Go:   go f()
来源：http://yxn.yj20258.top

Ruby: Thread.new { f }
来源：http://neq.dashuyun.cn

C#:   Task.Run(() => F());
来源：http://txf.mhx1999.top

[O02] 使用线程池
来源：http://ufw.yj202588.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uuk.guowangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zlx.bbcook.cn

JS:   // worker_threads 线程池
来源：http://fkg.hysaishi.cn

TS:   // worker_threads 线程池
来源：http://shr.zhijiandao.cn

Java: Executors.newFixedThreadPool(4)
来源：http://duc.hammf.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://heb.guowangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yjg.shuidangran.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rns.sweek.top

[O03] 加锁保护共享数据
来源：http://pft.tarul.cn

Py:   with lock: shared += 1
来源：http://gkk.snrcjt.cn

PHP:  // 用 flock() 做文件锁
来源：http://cjv.hongshengwenyu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://egl.daxiang520.top

TS:   // 同 JS
来源：http://vas.pengpengdd.cyou

Java: synchronized (this) { shared++; }
来源：http://pqb.sjlbkw.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pqp.jinyuanbaomall.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://dmg.jinqigufen.top

C#:   lock (gate) { shared++; }
来源：http://aib.iojbl.cn

[O04] 定义异步函数并等待
来源：http://hfl.vehdjk.com

Py:   async def f():⏎    await g()
来源：http://uep.ywan-chungtsiang.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kei.iojbl.cn

JS:   async function f() { await g(); }
来源：http://uhd.nanxinkj.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://fwc.jinyuanbaomall.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xgh.svipenyu.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xfu.ivvv.top

Ruby: # 用 Fiber 或 async gem
来源：http://pch.gogol.net.cn

C#:   async Task F() { await G(); }
来源：http://ddf.yj202588.top

[O05] 并发执行并等待全部完成
来源：http://aio.chenzaomai.com

Py:   asyncio.gather(*tasks)
来源：http://aqx.ywan-chungtsiang.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hlt.yuxming.cn

JS:   await Promise.all(tasks)
来源：http://him.feifeiyinyue.top

TS:   await Promise.all(tasks)
来源：http://req.sysykeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zwg.iojbl.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vhg.sysykeji.top

Ruby: threads.map(&:join)
来源：http://iqb.aibaodan.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ptt.ivvv.top

[O06] 使用进程池
来源：http://xiu.gogol.net.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qjd.hfpthk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mlu.smart0.xyz

JS:   // child_process / cluster 模块
来源：http://nnw.zycfv.cn

TS:   // child_process / cluster 模块
来源：http://hnk.guowangkeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qqb.ctjpmb.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eoo.hysaishi.cn

Ruby: // fork 块
来源：http://tur.gogol.net.cn

C#:   Parallel.For
来源：http://tsp.yuanzhike.top

================================================================================
来源：http://wok.0kj1m.cn

P. 常用工具函数
来源：http://hiv.shanyushiyangkeji.top

================================================================================
来源：http://qzy.316326.xyz

[P01] 生成 UUID
来源：http://jhh.jinqigfzy.top

Py:   str(uuid.uuid4())
来源：http://feb.zhiwuduotai.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cde.haohaochexian.top

JS:   crypto.randomUUID()
来源：http://ijz.hysaishi.cn

TS:   crypto.randomUUID()
来源：http://psz.hnqzz.top

Java: UUID.randomUUID().toString()
来源：http://hsq.tian-w.cn

Go:   // 用 github.com/google/uuid
来源：http://hkj.shanyushiyangtech.top

Ruby: SecureRandom.uuid
来源：http://rtr.andypj.xyz

C#:   Guid.NewGuid().ToString()
来源：http://ylv.tianlin.xyz

[P02] MD5 / SHA256 摘要
来源：http://jww.tarul.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://shz.quarkkingdee.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ide.smart0.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://alq.jinghuilouyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fwi.cdnleiting.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lyc.zhongyouzk.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yon.jqgufenzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hxq.daxiang520.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pny.shangyingyoupin.top

[P03] 生成短随机字符串
来源：http://ehl.quarkkingdee.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gpl.ybcxt.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nbo.jlsjyb.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rxc.sweek.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kml.shzxlz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://htm.vehdjk.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lbq.iojbl.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://srv.pycfn.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xwb.daria6918.cn

[P04] 求长度
来源：http://taq.ehwqpu.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cun.dashuyun.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ert.shanyushiyangkeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yli.wangdashe.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ezz.yj20258.top

Java: list.size();  map.size();  s.length()
来源：http://iop.yuxming.cn

Go:   len(arr);  len(m)
来源：http://xcb.c1oappe.top

Ruby: x.length;  x.size
来源：http://whe.ppjwa.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fws.bbcook.cn

[P05] 判断两个对象内容是否相等
来源：http://vcd.bjfxy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://rst.zdbjq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uwj.zhoulong.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lxf.jyoumei.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cdj.gotoacloud.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bmq.tarul.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ehe.0kj1m.cn

Ruby: a == b
来源：http://izh.shanyushiyangtech.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://srv.yj20258888.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://alu.hcnkem.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://udx.xingfuxueyuan.xyz

PHP:  if (empty($x)) {}
来源：http://huo.fanxiaobao.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://phs.zycfv.cn

TS:   if (x == null) {}
来源：http://asp.shanyushiyangkeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://njv.zhaomingkeji.xyz

Go:   if x == nil {}
来源：http://bkk.yfazqb.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://htx.52xcode.cn

C#:   if (x is null) {}
来源：http://hfn.shanyushiyangtech.top

[P07] 防抖与节流
来源：http://mtc.uphjek.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kbx.ybcxt.top

PHP:  // 手写时间戳比较
来源：http://lpy.shanyushiyangkeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kan.aizwys.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ldq.bbcook.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tqp.fengsongda.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ehe.jyoumei.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://biw.aizwys.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://raf.nwbrower.top

[P08] 处理浮点精度问题
来源：http://cql.ctjpmb.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://noe.sxryk.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wit.bbcook.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ybg.vehdjk.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://goa.nwbrower.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://iom.wangshuangyany.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ixs.xziqi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fsf.pengpengdd.cyou

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vqt.havefunace.top

================================================================================
来源：http://taf.haohaochexian.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qga.yueranfly.top

================================================================================
来源：http://pra.zhaomingkeji.xyz

[Q01] 创建表
来源：http://mxm.yongpay.top

CREATE TABLE users (
来源：http://pnn.yanxiufei.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zak.zhoulong.xyz

name VARCHAR(50) NOT NULL,
来源：http://nwd.daxiang520.top

email VARCHAR(100) UNIQUE,
来源：http://syg.sweek.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wmh.vehdjk.com

);
来源：http://uyb.yuanzhike.top

[Q02] 创建带外键的表
来源：http://dlu.yueranfly.top

CREATE TABLE orders (
来源：http://hxw.hywenlv.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zkm.yueranfly.top

user_id INT NOT NULL,
来源：http://prt.zhongyouzk.top

amount DECIMAL(10, 2),
来源：http://zpe.guannengcc.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vpd.jiagoushi.top

);
来源：http://lrv.ybcxt.top

[Q03] 增加列
来源：http://zev.c1oappe.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mmp.cheryme.top

[Q04] 修改列类型
来源：http://idr.yvedp.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ggz.ctjpmb.com

[Q05] 重命名列
来源：http://rcd.gzhubu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://loe.sysykeji.top

[Q06] 删除列
来源：http://eao.gzhubu.top

ALTER TABLE users DROP COLUMN age;
来源：http://mhz.9152youxi.cn

[Q07] 删除表
来源：http://sfk.jqgfzy.top

DROP TABLE IF EXISTS orders;
来源：http://ymh.bbcook.cn

[Q08] 创建普通索引
来源：http://znj.cdnleiting.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jey.yvedp.cn

[Q09] 创建唯一索引
来源：http://gxv.gaohongyu789.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sox.zdbjq.cn

[Q10] 插入单行
来源：http://usp.uphjek.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vom.ehwqpu.com

[Q11] 一次插入多行
来源：http://ikd.zhixingplan.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://afl.quarkkingdee.top

[Q12] 插入后取自增 ID
来源：http://tvt.haohaochexian.top

INSERT INTO users (name) VALUES ('C');
来源：http://esl.epnwcf.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kzy.nwbrower.top

[Q13] 忽略重复插入
来源：http://qjq.zhiwuduotai.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://emm.316326.xyz

[Q14] 存在则更新（upsert）
来源：http://rsq.hysaishi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zys.jinghuilouyu.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ism.xingfuxueyuan.xyz

[Q15] 查询全部
来源：http://bzq.smart0.xyz

SELECT * FROM users;
来源：http://ucm.jqgfzy.top

[Q16] 查询指定列
来源：http://xuz.hongshengwenyu.top

SELECT id, name FROM users;
来源：http://rtw.ivvv.top

[Q17] 条件查询
来源：http://nhw.chenjidiqi.icu

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tpg.ydjk.org.cn

[Q18] 模糊匹配
来源：http://uct.fanxiaobao.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mkc.shanyushiyangtech.top

[Q19] 范围查询
来源：http://xvt.wangdashe.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cjb.daria6918.cn

[Q20] IN 列表
来源：http://cca.gotoacloud.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jjk.zhiwuduotai.top

[Q21] 空值判断
来源：http://ncf.gotoacloud.top

SELECT * FROM users WHERE email IS NULL;
来源：http://kwb.hywenlv.cn

[Q22] 排序
来源：http://xlv.jqgfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qti.zhijiandao.cn

[Q23] 分页
来源：http://mlb.zhongyouzk.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lag.zdbjq.cn

[Q24] 去重
来源：http://bcx.zhiwuduotai.top

SELECT DISTINCT city FROM users;
来源：http://nzs.zhixingplan.top

[Q25] 只取前 N 条
来源：http://zrl.daria6918.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gaq.0kj1m.cn

[Q26] 计数
来源：http://rzg.bbcook.cn

SELECT COUNT(*) FROM users;
来源：http://hoi.zhijiandao.cn

[Q27] 条件计数
来源：http://jfe.zycfv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ili.xingfuxueyuan.xyz

[Q28] 求和与平均
来源：http://aci.hammf.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hkv.52xcode.cn

[Q29] 最大最小值
来源：http://usw.gaohongyu789.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://mhr.fanxiaobao.xyz

[Q30] 分组统计
来源：http://zwd.jiagoushi.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ilk.shanyushiyangkeji.top

[Q31] 分组后过滤
来源：http://qrs.tarul.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sja.ehwqpu.com

[Q32] 分组拼接字符串
来源：http://avz.aizwys.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wkd.xuetiantiany.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xht.gzhubu.top

[Q33] 多列分组
来源：http://bro.gotoacloud.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pvw.gotoacloud.top

[Q34] 每组取第一条
来源：http://lgy.jinghuilouyu.cn

SELECT * FROM (
来源：http://bow.yvedp.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://avi.epnwcf.com

) t WHERE rn = 1;
来源：http://xdg.shuidangran.top

[Q35] 内连接
来源：http://ttd.yuanzhike.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gaf.vehdjk.com

[Q36] 左连接
来源：http://arl.yj20258888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hea.chenzaomai.com

[Q37] 右连接
来源：http://ajf.9152youxi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kkx.ywan-chungtsiang.top

[Q38] 全外连接（PostgreSQL）
来源：http://anz.fktsv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://eup.pycfn.com

[Q39] 自连接（查上下级）
来源：http://eip.jlsjyb.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qmd.ehwqpu.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hww.aizwys.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vxl.xuanzx.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fam.nwbrower.top

[Q41] 多表连接
来源：http://yqg.jiagoushi.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ucm.yueranfly.top

JOIN users u ON u.id = o.user_id
来源：http://noe.redwolf501.top

JOIN products p ON p.id = o.product_id;
来源：http://dmq.gzhubu.top

[Q42] 连接条件附加过滤
来源：http://klp.vqdsnc.cn


<!-- 参考信息 -->