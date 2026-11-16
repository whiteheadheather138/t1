代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://woc.chenlongwang.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wbk.yvedp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kjz.pycfn.com

Ruby: a.gcd(b)
来源：http://kog.yonumen.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fqs.chenzaomai.com

[N06] 判断回文字符串
来源：http://tmq.ydzc1.top

Py:   s == s[::-1]
来源：http://sdu.zhaomingkeji.xyz

PHP:  $s === strrev($s);
来源：http://nif.smart0.xyz

JS:   s === [...s].reverse().join("")
来源：http://mpe.cashguo.top

TS:   s === [...s].reverse().join("")
来源：http://tnf.nwbrower.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vof.zhixingplan.top

Go:   // 双指针从两端比较
来源：http://vwg.zycfv.cn

Ruby: s == s.reverse
来源：http://cqv.uphjek.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://rat.zhaomingkeji.xyz

[N07] 两数之和（返回下标）
来源：http://csq.svipenyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://eyi.xziqi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mib.tianlin.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://lky.gogol.net.cn

TS:   // 手写 Map<string, number>
来源：http://gaa.nanxinkj.top

Java: // 手写 HashMap
来源：http://cve.yangfankeji.com

Go:   // 手写 map[int]int
来源：http://cqn.jlsjyb.cn

Ruby: // 手写 Hash
来源：http://shh.gogol.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fwd.smart0.xyz

[N08] 生成全排列
来源：http://jds.hfpthk.cn

Py:   itertools.permutations(arr)
来源：http://tdv.0kj1m.cn

PHP:  // 手写递归交换
来源：http://fub.wangdashe.top

JS:   // 手写回溯递归
来源：http://vlc.zhongyouzk.top

TS:   // 手写回溯递归
来源：http://npa.daria6918.cn

Java: // 手写回溯递归
来源：http://mda.hnqzz.top

Go:   // 手写回溯递归
来源：http://kkk.iojbl.cn

Ruby: arr.permutation.to_a
来源：http://but.0kj1m.cn

C#:   // 手写回溯递归
来源：http://ulz.havefunace.top

[N09] 栈与队列
来源：http://etg.vehdjk.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pvr.sweek.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nwq.sjlbkw.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cdk.quarkkingdee.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tgn.vehdjk.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wkt.pengpengdd.cyou

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fsl.ydjk.org.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jzj.jlsjyb.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://boj.tarul.cn

[N10] 链表节点定义
来源：http://lfw.gaohongyu789.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ywm.hongshengwenyu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vrb.chenjidiqi.icu

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hao.xylfe.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nzg.vehdjk.com

Java: class Node { int v; Node next; }
来源：http://ifl.ctjpmb.com

Go:   type Node struct { V int; Next *Node }
来源：http://klp.nanxinkj.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ygk.cqqwz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ryp.jlsjyb.cn

[N11] 二叉树中序遍历
来源：http://mcb.jqgfzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://don.gogol.net.cn

PHP:  // 手写递归函数
来源：http://lvy.xuanzx.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://maz.havefunace.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bnd.wangdashe.top

Java: // 手写递归
来源：http://iyi.tarul.cn

Go:   // 手写递归
来源：http://znz.yongpay.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://aii.daria6918.cn

C#:   // 手写递归
来源：http://vho.wangdashe.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ugn.dianchejie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ouj.meibo888.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yxp.bbcook.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mdb.yanxiufei.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ayn.aibaodan.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zuc.ywan-chungtsiang.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ija.cucudq.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dmt.sjlbkw.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vfl.zhaomingkeji.xyz

================================================================================
来源：http://yvq.snrcjt.cn

O. 并发与异步
来源：http://vgp.ywan-chungtsiang.top

================================================================================
来源：http://tpt.xziqi.cn

[O01] 启动一个线程
来源：http://oxv.daxiang520.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uad.nanxinkj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wqx.ybcxt.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jxz.zhengqikj.top

TS:   // 同 JS
来源：http://gmz.xylfe.cn

Java: new Thread(() -> f()).start()
来源：http://mmz.pengpengdd.cyou

Go:   go f()
来源：http://jjw.ywan-chungtsiang.top

Ruby: Thread.new { f }
来源：http://wed.vqdsnc.cn

C#:   Task.Run(() => F());
来源：http://rgb.c1oappe.top

[O02] 使用线程池
来源：http://avo.yvedp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mah.zhaomingkeji.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://iop.xingfuxueyuan.xyz

JS:   // worker_threads 线程池
来源：http://jjh.gotoacloud.top

TS:   // worker_threads 线程池
来源：http://yjz.jlsjyb.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wxv.ydjk.org.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rvv.nanxinkj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qov.sjlbkw.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ydd.feifeiyinyue.top

[O03] 加锁保护共享数据
来源：http://rfv.jinghuilouyu.cn

Py:   with lock: shared += 1
来源：http://eye.hongshengwenyu.top

PHP:  // 用 flock() 做文件锁
来源：http://xnr.sweek.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hot.chenlongwang.top

TS:   // 同 JS
来源：http://nui.iojbl.cn

Java: synchronized (this) { shared++; }
来源：http://acw.meibo888.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xfa.chenlongwang.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jpj.ybcxt.top

C#:   lock (gate) { shared++; }
来源：http://qtl.havefunace.top

[O04] 定义异步函数并等待
来源：http://xht.ctjpmb.com

Py:   async def f():⏎    await g()
来源：http://cob.feifeiyinyue.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dhk.aibaodan.cn

JS:   async function f() { await g(); }
来源：http://cmh.52xcode.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ksl.xinyue.icu

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fsa.sysykeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tby.feifeiyinyue.top

Ruby: # 用 Fiber 或 async gem
来源：http://twp.52xcode.cn

C#:   async Task F() { await G(); }
来源：http://xzj.hfpthk.cn

[O05] 并发执行并等待全部完成
来源：http://wba.yuanzhike.top

Py:   asyncio.gather(*tasks)
来源：http://sdc.fehbvm.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://imm.cashguo.top

JS:   await Promise.all(tasks)
来源：http://fhl.vqdsnc.cn

TS:   await Promise.all(tasks)
来源：http://aox.xingfuxueyuan.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nrg.jqgufenzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ocg.zdbjq.cn

Ruby: threads.map(&:join)
来源：http://rtv.bbcook.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tuf.haohaochexian.top

[O06] 使用进程池
来源：http://wli.andypj.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zcq.fehbvm.com

PHP:  // pcntl_fork 或多进程队列
来源：http://nyg.meibo888.top

JS:   // child_process / cluster 模块
来源：http://zcb.xylfe.cn

TS:   // child_process / cluster 模块
来源：http://jci.shanyushiyangtech.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qrn.jiagoushi.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fmy.wangshuangyany.cn

Ruby: // fork 块
来源：http://stf.yuanzhike.top

C#:   Parallel.For
来源：http://nlu.ydjk.org.cn

================================================================================
来源：http://toi.sufxvd.cn

P. 常用工具函数
来源：http://yep.cdnleiting.top

================================================================================
来源：http://yom.yj202588.top

[P01] 生成 UUID
来源：http://wpl.guannengcc.top

Py:   str(uuid.uuid4())
来源：http://hon.sufxvd.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vfx.gzhubu.top

JS:   crypto.randomUUID()
来源：http://esn.cqqwz.cn

TS:   crypto.randomUUID()
来源：http://tmi.jlsjyb.cn

Java: UUID.randomUUID().toString()
来源：http://ixg.bbcook.cn

Go:   // 用 github.com/google/uuid
来源：http://ovq.yvedp.cn

Ruby: SecureRandom.uuid
来源：http://vut.guowangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://slt.chenzaomai.com

[P02] MD5 / SHA256 摘要
来源：http://ocu.shanyushiyangtech.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hvk.fanxiaobao.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://ymc.daxiang520.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ghc.jqgufenzy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://krv.svipenyu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ijn.cqqwz.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qxj.yuanzhike.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jxu.epnwcf.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dgp.yonumen.top

[P03] 生成短随机字符串
来源：http://mcm.hnxiangtu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://whr.yj20258888.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vop.gogol.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://auk.yonumen.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wvm.haohaochexian.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://slr.zhoulong.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://liu.jianghu66.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://dkk.sysykeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ozr.cqqwz.cn

[P04] 求长度
来源：http://png.ehwqpu.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dkm.xuetiantiany.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ynh.meibo888.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vhp.ydzc1.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fnq.ehwqpu.com

Java: list.size();  map.size();  s.length()
来源：http://pah.zdbjq.cn

Go:   len(arr);  len(m)
来源：http://mms.daxiang520.top

Ruby: x.length;  x.size
来源：http://iim.epnwcf.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://grz.tarul.cn

[P05] 判断两个对象内容是否相等
来源：http://qih.guannengcc.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://nhw.guannengcc.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fto.tian-w.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hky.xziqi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://poc.52xcode.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kzh.gaohongyu789.top

Go:   reflect.DeepEqual(a, b)
来源：http://tds.yangfankeji.com

Ruby: a == b
来源：http://ayd.chenjidiqi.icu

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ruh.gzhubu.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vnh.ywan-chungtsiang.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yzr.xziqi.cn

PHP:  if (empty($x)) {}
来源：http://yrz.hammf.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wpq.yuanzhike.top

TS:   if (x == null) {}
来源：http://ujp.gogol.net.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://yht.ivvv.top

Go:   if x == nil {}
来源：http://trm.cashguo.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jqw.cqqwz.cn

C#:   if (x is null) {}
来源：http://wbp.cucudq.cn

[P07] 防抖与节流
来源：http://jkc.jqgfzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://inr.zhiwuduotai.top

PHP:  // 手写时间戳比较
来源：http://tqe.ydjk.org.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hyy.9152youxi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oie.guowangkeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bfj.jinqigufen.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jdr.ydjk.org.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://kef.aizwys.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://put.xuetiantiany.cn

[P08] 处理浮点精度问题
来源：http://qeg.feifeiyinyue.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sib.zycfv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vkn.ybcxt.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wzf.meibo888.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://raz.aibaodan.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://asd.gaohongyu789.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ymv.yj202588.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xrd.fehbvm.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://iek.birdmap.top

================================================================================
来源：http://cyl.jianghu66.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xnc.sufxvd.cn

================================================================================
来源：http://umx.xylfe.cn

[Q01] 创建表
来源：http://nnh.sufxvd.cn

CREATE TABLE users (
来源：http://lgo.jqgfzy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mvf.jinghuilouyu.cn

name VARCHAR(50) NOT NULL,
来源：http://bds.0kj1m.cn

email VARCHAR(100) UNIQUE,
来源：http://pam.pycfn.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lqg.zhoulong.xyz

);
来源：http://fkl.chenjidiqi.icu

[Q02] 创建带外键的表
来源：http://pzx.ydzc1.top

CREATE TABLE orders (
来源：http://ytt.guowangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tqr.daxiang520.top

user_id INT NOT NULL,
来源：http://kme.c1oappe.top

amount DECIMAL(10, 2),
来源：http://iqj.fehbvm.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tow.bbcook.cn

);
来源：http://ufb.bbcook.cn

[Q03] 增加列
来源：http://whf.shanyushiyangtech.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pse.zhixingplan.top

[Q04] 修改列类型
来源：http://vft.guowangkeji.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hrm.aibaodan.cn

[Q05] 重命名列
来源：http://hie.shanyushiyangkeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://oum.zycfv.cn

[Q06] 删除列
来源：http://hmy.xziqi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fin.jqgufenzy.top

[Q07] 删除表
来源：http://ncd.yfazqb.com

DROP TABLE IF EXISTS orders;
来源：http://svl.daxiang520.top

[Q08] 创建普通索引
来源：http://xbu.guannengcc.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ybv.cucudq.cn

[Q09] 创建唯一索引
来源：http://clx.guannengcc.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ubw.jqgufenzy.top

[Q10] 插入单行
来源：http://jcj.yanxiufei.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fdd.iojbl.cn

[Q11] 一次插入多行
来源：http://tob.zdbjq.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dir.bjfxy.top

[Q12] 插入后取自增 ID
来源：http://xho.wangdashe.top

INSERT INTO users (name) VALUES ('C');
来源：http://euc.aibaodan.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cuo.gogol.net.cn

[Q13] 忽略重复插入
来源：http://dmh.jianghu66.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lkk.yangfankeji.com

[Q14] 存在则更新（upsert）
来源：http://zzp.xuetiantiany.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://knz.316326.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nzw.cqqwz.cn

[Q15] 查询全部
来源：http://mwy.pengpengdd.cyou

SELECT * FROM users;
来源：http://zzf.cucudq.cn

[Q16] 查询指定列
来源：http://jek.svipenyu.cn

SELECT id, name FROM users;
来源：http://yow.jqgfzy.top

[Q17] 条件查询
来源：http://ues.cashguo.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pdh.ivvv.top

[Q18] 模糊匹配
来源：http://ssn.daxiang520.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zdz.yfazqb.com

[Q19] 范围查询
来源：http://mdb.52xcode.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pnl.vqdsnc.cn

[Q20] IN 列表
来源：http://xen.andypj.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xyv.guowangkeji.top

[Q21] 空值判断
来源：http://lqz.jqgufenzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://kgv.cucudq.cn

[Q22] 排序
来源：http://qlp.zhiwuduotai.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rpq.ywan-chungtsiang.top

[Q23] 分页
来源：http://ffc.hammf.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lke.jinghuilouyu.cn

[Q24] 去重
来源：http://ydb.shuidangran.top

SELECT DISTINCT city FROM users;
来源：http://wjp.aibaodan.cn

[Q25] 只取前 N 条
来源：http://ypr.vqdsnc.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cdx.gaohongyu789.top

[Q26] 计数
来源：http://jrs.yongpay.top

SELECT COUNT(*) FROM users;
来源：http://wkw.cdnleiting.top

[Q27] 条件计数
来源：http://rgq.sweek.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://izw.chenzaomai.com

[Q28] 求和与平均
来源：http://ftb.havefunace.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rwk.xuanzx.com

[Q29] 最大最小值
来源：http://bxk.yuxming.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tji.epnwcf.com

[Q30] 分组统计
来源：http://njt.smart0.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://has.zhongyouzk.top

[Q31] 分组后过滤
来源：http://emp.316326.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qsz.meibo888.top

[Q32] 分组拼接字符串
来源：http://qvl.gzhubu.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hnf.redwolf501.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kta.c1oappe.top

[Q33] 多列分组
来源：http://umo.daxiang520.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xtj.jqgfzy.top

[Q34] 每组取第一条
来源：http://rjy.cashguo.top

SELECT * FROM (
来源：http://lto.wangdashe.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bvk.xylfe.cn

) t WHERE rn = 1;
来源：http://ist.yangfankeji.com

[Q35] 内连接
来源：http://pzk.ppjwa.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rua.kuanghao11.cn

[Q36] 左连接
来源：http://bqf.chenjidiqi.icu

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://foc.cheryme.top

[Q37] 右连接
来源：http://wzr.ctjpmb.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vxk.ybcxt.top

[Q38] 全外连接（PostgreSQL）
来源：http://hde.xziqi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bqj.epnwcf.com

[Q39] 自连接（查上下级）
来源：http://hut.gogol.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vgk.xylfe.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nrf.zhoulong.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://kbb.pengpengdd.cyou

SELECT * FROM colors CROSS JOIN sizes;
来源：http://frd.pycfn.com

[Q41] 多表连接
来源：http://zma.xinyue.icu


<!-- 参考信息 -->