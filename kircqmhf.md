代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://new.zycfv.cn

[N06] 判断回文字符串
来源：http://anz.nanxinkj.top

Py:   s == s[::-1]
来源：http://isp.hnxiangtu.top

PHP:  $s === strrev($s);
来源：http://ene.ehwqpu.com

JS:   s === [...s].reverse().join("")
来源：http://kfv.hesvh.cn

TS:   s === [...s].reverse().join("")
来源：http://fxc.andypj.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ffg.xingfuxueyuan.xyz

Go:   // 双指针从两端比较
来源：http://uce.fanxiaobao.xyz

Ruby: s == s.reverse
来源：http://fko.tanke756.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://qkt.ehwqpu.com

[N07] 两数之和（返回下标）
来源：http://wxo.yangfankeji.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qog.sxryk.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mra.hysaishi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://amv.haohaochexian.top

TS:   // 手写 Map<string, number>
来源：http://pcc.jqgfzy.top

Java: // 手写 HashMap
来源：http://twz.daria6918.cn

Go:   // 手写 map[int]int
来源：http://efh.zhiwuduotai.top

Ruby: // 手写 Hash
来源：http://ltb.fzhhl.top

C#:   // 手写 Dictionary<int, int>
来源：http://avn.jqgfzy.top

[N08] 生成全排列
来源：http://lib.xingfuxueyuan.xyz

Py:   itertools.permutations(arr)
来源：http://zgq.shzxlz.cn

PHP:  // 手写递归交换
来源：http://msz.ydzc1.top

JS:   // 手写回溯递归
来源：http://xya.shangyingyoupin.top

TS:   // 手写回溯递归
来源：http://cxe.hysaishi.cn

Java: // 手写回溯递归
来源：http://bpa.kuanghao11.cn

Go:   // 手写回溯递归
来源：http://itr.ppjwa.cn

Ruby: arr.permutation.to_a
来源：http://zec.316326.xyz

C#:   // 手写回溯递归
来源：http://ezc.yangfankeji.com

[N09] 栈与队列
来源：http://dlw.yongpay.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hjc.uphjek.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gbz.gotoacloud.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rik.jinqigufen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zxp.fehbvm.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hnq.jianghu66.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xsc.chenzaomai.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pis.smart0.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://svh.zhixingplan.top

[N10] 链表节点定义
来源：http://dbo.zhoulong.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zjh.hnxiangtu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://tsg.jianghu66.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qbr.chenlongwang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lcl.meibo888.top

Java: class Node { int v; Node next; }
来源：http://nfh.yuanzhike.top

Go:   type Node struct { V int; Next *Node }
来源：http://ugy.fehbvm.com

Ruby: Node = Struct.new(:v, :next)
来源：http://bwm.snrcjt.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gyy.cdnleiting.top

[N11] 二叉树中序遍历
来源：http://scx.fktsv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yet.vehdjk.com

PHP:  // 手写递归函数
来源：http://ayt.hfpthk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://myt.iojbl.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mgr.vehdjk.com

Java: // 手写递归
来源：http://fma.daria6918.cn

Go:   // 手写递归
来源：http://nlb.xuanzx.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jdc.sweek.top

C#:   // 手写递归
来源：http://pqj.sufxvd.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://szc.hammf.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wrv.52xcode.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vej.zhaomingkeji.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jyq.chenjidiqi.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pvi.yvedp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jta.quarkkingdee.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yni.jianghu66.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mng.ydjk.org.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ode.dashuyun.cn

================================================================================
来源：http://dap.ybcxt.top

O. 并发与异步
来源：http://vom.quarkkingdee.top

================================================================================
来源：http://ley.fzhhl.top

[O01] 启动一个线程
来源：http://ztn.zhengqikj.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rco.haohaochexian.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ryi.guannengcc.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zcy.nwbrower.top

TS:   // 同 JS
来源：http://vzj.ywan-chungtsiang.top

Java: new Thread(() -> f()).start()
来源：http://fbq.sxryk.cn

Go:   go f()
来源：http://bgj.sxryk.cn

Ruby: Thread.new { f }
来源：http://hfb.hnqzz.top

C#:   Task.Run(() => F());
来源：http://otx.xingfuxueyuan.xyz

[O02] 使用线程池
来源：http://hdm.ctjpmb.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cil.hnxiangtu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vuq.hongshengwenyu.top

JS:   // worker_threads 线程池
来源：http://agc.daria6918.cn

TS:   // worker_threads 线程池
来源：http://wjf.cheryme.top

Java: Executors.newFixedThreadPool(4)
来源：http://vdy.ydzc1.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xxa.redwolf501.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pvr.yvedp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sah.sufxvd.cn

[O03] 加锁保护共享数据
来源：http://gru.chenlongwang.top

Py:   with lock: shared += 1
来源：http://zdh.shuidangran.top

PHP:  // 用 flock() 做文件锁
来源：http://srl.haohaochexian.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://waz.bbcook.cn

TS:   // 同 JS
来源：http://koj.bbcook.cn

Java: synchronized (this) { shared++; }
来源：http://gnq.jinghuilouyu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://knx.haohaochexian.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://dhr.hfpthk.cn

C#:   lock (gate) { shared++; }
来源：http://tvj.hywenlv.cn

[O04] 定义异步函数并等待
来源：http://odw.sufxvd.cn

Py:   async def f():⏎    await g()
来源：http://mco.hysaishi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xys.bbcook.cn

JS:   async function f() { await g(); }
来源：http://owh.gzhubu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://kdb.jqgfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vhb.xinyue.icu

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oxn.nwbrower.top

Ruby: # 用 Fiber 或 async gem
来源：http://dsu.bbcook.cn

C#:   async Task F() { await G(); }
来源：http://gbv.pycfn.com

[O05] 并发执行并等待全部完成
来源：http://hcn.svipenyu.cn

Py:   asyncio.gather(*tasks)
来源：http://izx.chenlongwang.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ozy.dianchejie.cn

JS:   await Promise.all(tasks)
来源：http://yyy.jinyuanbaomall.cn

TS:   await Promise.all(tasks)
来源：http://awq.0kj1m.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://way.hesvh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fep.cheryme.top

Ruby: threads.map(&:join)
来源：http://qra.fktsv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nxh.zdbjq.cn

[O06] 使用进程池
来源：http://zcd.birdmap.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tei.zdbjq.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vnt.ybcxt.top

JS:   // child_process / cluster 模块
来源：http://dgn.feifeiyinyue.top

TS:   // child_process / cluster 模块
来源：http://psg.cucudq.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sks.shanyushiyangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://por.9152youxi.cn

Ruby: // fork 块
来源：http://awn.yangfankeji.com

C#:   Parallel.For
来源：http://zxa.redwolf501.top

================================================================================
来源：http://org.yj20258.top

P. 常用工具函数
来源：http://lrn.zhaomingkeji.xyz

================================================================================
来源：http://ovk.yvedp.cn

[P01] 生成 UUID
来源：http://dwn.zycfv.cn

Py:   str(uuid.uuid4())
来源：http://huv.xuanzx.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://knr.mhx1999.top

JS:   crypto.randomUUID()
来源：http://qdp.zhengqikj.top

TS:   crypto.randomUUID()
来源：http://bon.jinghuilouyu.cn

Java: UUID.randomUUID().toString()
来源：http://vgl.cdnleiting.top

Go:   // 用 github.com/google/uuid
来源：http://six.yj20258.top

Ruby: SecureRandom.uuid
来源：http://ojv.meibo888.top

C#:   Guid.NewGuid().ToString()
来源：http://pxx.zhengqikj.top

[P02] MD5 / SHA256 摘要
来源：http://pnd.gaohongyu789.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://amb.yongpay.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wuz.ehwqpu.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://awv.uphjek.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wda.daxiang520.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uka.chenzaomai.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ndy.zhijiandao.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ooc.nwbrower.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mos.shuidangran.top

[P03] 生成短随机字符串
来源：http://ait.pengpengdd.cyou

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pag.yj202588.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tzf.yj20258.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://chd.yj202588.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bdn.cucudq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sit.guowangkeji.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cam.zycfv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://icc.xinyue.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dhj.iojbl.cn

[P04] 求长度
来源：http://ktk.0kj1m.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nmj.jyoumei.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ysm.mhx1999.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rdg.52xcode.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hyv.jinqigfzy.top

Java: list.size();  map.size();  s.length()
来源：http://xqq.xingfuxueyuan.xyz

Go:   len(arr);  len(m)
来源：http://qha.haohaochexian.top

Ruby: x.length;  x.size
来源：http://zmi.redwolf501.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://cuj.yonumen.top

[P05] 判断两个对象内容是否相等
来源：http://lhx.jiagoushi.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://mol.wangdashe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lvg.zdbjq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hso.guannengcc.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://byz.yj202588.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zcw.jinqigfzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://xlz.ybcxt.top

Ruby: a == b
来源：http://slz.wangshuangyany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gag.sweek.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hwt.fktsv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cyn.cdnleiting.top

PHP:  if (empty($x)) {}
来源：http://kzx.shzxlz.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gyd.jinghuilouyu.cn

TS:   if (x == null) {}
来源：http://agn.zhongyouzk.top

Java: if (x == null || x.isEmpty()) {}
来源：http://lrr.meibo888.top

Go:   if x == nil {}
来源：http://blq.yvedp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://due.kuanghao11.cn

C#:   if (x is null) {}
来源：http://xcf.yuxming.cn

[P07] 防抖与节流
来源：http://tpw.gaohongyu789.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kdl.guowangkeji.top

PHP:  // 手写时间戳比较
来源：http://jqx.meibo888.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lje.hcnkem.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cbr.iojbl.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jdp.xziqi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://psc.jinqigfzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zft.yangfankeji.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gre.zhijiandao.cn

[P08] 处理浮点精度问题
来源：http://vtl.sxryk.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://aqu.vqdsnc.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vln.jlsjyb.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://quq.ybcxt.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zxb.aibaodan.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lwq.bbcook.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mdn.zhongyouzk.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://asg.shuidangran.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ixx.shuidangran.top

================================================================================
来源：http://xst.yuxming.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hir.jinqigfzy.top

================================================================================
来源：http://uds.jyoumei.cn

[Q01] 创建表
来源：http://iok.yfazqb.com

CREATE TABLE users (
来源：http://ivb.xinyue.icu

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://axj.zdqjudy.top

name VARCHAR(50) NOT NULL,
来源：http://dvi.zdbjq.cn

email VARCHAR(100) UNIQUE,
来源：http://xuh.cashguo.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qor.zhiwuduotai.top

);
来源：http://etn.hongshengwenyu.top

[Q02] 创建带外键的表
来源：http://ron.bjfxy.top

CREATE TABLE orders (
来源：http://ixl.xylfe.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fuk.xuanzx.com

user_id INT NOT NULL,
来源：http://bzm.andypj.xyz

amount DECIMAL(10, 2),
来源：http://kca.tianlin.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nnu.cashguo.top

);
来源：http://sov.aizwys.cn

[Q03] 增加列
来源：http://iow.ywan-chungtsiang.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ooo.daria6918.cn

[Q04] 修改列类型
来源：http://rar.zhiwuduotai.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://irr.yfazqb.com

[Q05] 重命名列
来源：http://uao.cqqwz.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://skx.bjfxy.top

[Q06] 删除列
来源：http://dqw.yfazqb.com

ALTER TABLE users DROP COLUMN age;
来源：http://xxv.0kj1m.cn

[Q07] 删除表
来源：http://vqx.epnwcf.com

DROP TABLE IF EXISTS orders;
来源：http://tgr.aibaodan.cn

[Q08] 创建普通索引
来源：http://apd.zhiwuduotai.top

CREATE INDEX idx_users_email ON users(email);
来源：http://maf.shzxlz.cn

[Q09] 创建唯一索引
来源：http://oac.dashuyun.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ocu.chenlongwang.top

[Q10] 插入单行
来源：http://dds.wangdashe.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vke.bjfxy.top

[Q11] 一次插入多行
来源：http://ata.xuetiantiany.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fsf.fanxiaobao.xyz

[Q12] 插入后取自增 ID
来源：http://utp.wangshuangyany.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pws.ydzc1.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vac.pycfn.com

[Q13] 忽略重复插入
来源：http://xtp.cashguo.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zmz.jiagoushi.top

[Q14] 存在则更新（upsert）
来源：http://wmq.wangdashe.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://how.ydjk.org.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jel.zhengqikj.top

[Q15] 查询全部
来源：http://weo.gzhubu.top

SELECT * FROM users;
来源：http://zkh.xingfuxueyuan.xyz

[Q16] 查询指定列
来源：http://nzh.zhoulong.xyz

SELECT id, name FROM users;
来源：http://joj.zdqjudy.top

[Q17] 条件查询
来源：http://qwg.jqgfzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iyk.hesvh.cn

[Q18] 模糊匹配
来源：http://rho.redwolf501.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cis.cdnleiting.top

[Q19] 范围查询
来源：http://ijr.chenzaomai.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gij.meibo888.top

[Q20] IN 列表
来源：http://adp.xuanzx.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rvt.hcnkem.com

[Q21] 空值判断
来源：http://kof.kuanghao11.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gzy.yanxiufei.cn

[Q22] 排序
来源：http://vez.gaohongyu789.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kfz.ctjpmb.com

[Q23] 分页
来源：http://iup.gaohongyu789.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vhi.ydjk.org.cn

[Q24] 去重
来源：http://njh.smart0.xyz

SELECT DISTINCT city FROM users;
来源：http://swr.pengpengdd.cyou

[Q25] 只取前 N 条
来源：http://grj.nwbrower.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://frt.zhaomingkeji.xyz

[Q26] 计数
来源：http://bnp.hnxiangtu.top

SELECT COUNT(*) FROM users;
来源：http://iob.haohaochexian.top

[Q27] 条件计数
来源：http://pik.dashuyun.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mrs.yfazqb.com

[Q28] 求和与平均
来源：http://jhq.zhoulong.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dsj.xziqi.cn

[Q29] 最大最小值
来源：http://ape.epnwcf.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://vdr.fanxiaobao.xyz

[Q30] 分组统计
来源：http://txe.jinyuanbaomall.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ohm.tian-w.cn

[Q31] 分组后过滤
来源：http://ner.zhijiandao.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pwh.yuxming.cn

[Q32] 分组拼接字符串
来源：http://ntb.sxryk.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vav.hywenlv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://udd.zhaomingkeji.xyz

[Q33] 多列分组
来源：http://dyn.zhijiandao.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://etu.jinqigufen.top

[Q34] 每组取第一条
来源：http://nzy.pengpengdd.cyou

SELECT * FROM (
来源：http://ryu.andypj.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nzi.hammf.cn

) t WHERE rn = 1;
来源：http://vec.jqgufenzy.top

[Q35] 内连接
来源：http://ngd.ydzc1.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hhr.ctjpmb.com

[Q36] 左连接
来源：http://itq.shangyingyoupin.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sxx.zhiwuduotai.top

[Q37] 右连接
来源：http://wok.hcnkem.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://oyv.tianlin.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://wvo.hammf.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gwg.chenzaomai.com

[Q39] 自连接（查上下级）
来源：http://ege.pycfn.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://kyc.dashuyun.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vlt.bbcook.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cxm.zdbjq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qah.316326.xyz

[Q41] 多表连接
来源：http://gcx.andypj.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://tte.shanyushiyangtech.top

JOIN users u ON u.id = o.user_id
来源：http://shb.pycfn.com

JOIN products p ON p.id = o.product_id;
来源：http://zmz.ctjpmb.com

[Q42] 连接条件附加过滤
来源：http://egy.andypj.xyz


<!-- 参考信息 -->