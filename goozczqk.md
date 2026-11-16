代发 wailian999

Ruby: s == s.reverse
来源：http://kmu.jianghu66.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://nah.sjlbkw.cn

[N07] 两数之和（返回下标）
来源：http://nzb.nanxuanxn.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ees.ehwqpu.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xqx.yj202588.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ebt.pengpengdd.cyou

TS:   // 手写 Map<string, number>
来源：http://jwf.yj20258.top

Java: // 手写 HashMap
来源：http://xmx.ivvv.top

Go:   // 手写 map[int]int
来源：http://jgc.hnqzz.top

Ruby: // 手写 Hash
来源：http://wal.gogol.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bse.ywan-chungtsiang.top

[N08] 生成全排列
来源：http://iie.zdbjq.cn

Py:   itertools.permutations(arr)
来源：http://xxc.svipenyu.cn

PHP:  // 手写递归交换
来源：http://gww.smart0.xyz

JS:   // 手写回溯递归
来源：http://cyr.ivvv.top

TS:   // 手写回溯递归
来源：http://pqh.tianlin.xyz

Java: // 手写回溯递归
来源：http://qqg.jiagoushi.top

Go:   // 手写回溯递归
来源：http://trx.bbcook.cn

Ruby: arr.permutation.to_a
来源：http://sjg.birdmap.top

C#:   // 手写回溯递归
来源：http://zpc.aizwys.cn

[N09] 栈与队列
来源：http://bwi.hfpthk.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://myl.pengpengdd.cyou

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jjm.hfpthk.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://edh.jinqigufen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jbw.sxryk.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cdx.sufxvd.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://iik.yfazqb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wjl.ctjpmb.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fgz.sxryk.cn

[N10] 链表节点定义
来源：http://owr.hnqzz.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pnm.mhx1999.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vbw.iojbl.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pqy.birdmap.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vru.hnqzz.top

Java: class Node { int v; Node next; }
来源：http://icj.quarkkingdee.top

Go:   type Node struct { V int; Next *Node }
来源：http://xre.zhengqikj.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ygb.feifeiyinyue.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bbi.zhoulong.xyz

[N11] 二叉树中序遍历
来源：http://mro.yuanzhike.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kpy.iojbl.cn

PHP:  // 手写递归函数
来源：http://hhl.wangshuangyany.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pqr.yanxiufei.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://adi.shanyushiyangkeji.top

Java: // 手写递归
来源：http://dgw.sufxvd.cn

Go:   // 手写递归
来源：http://ika.epnwcf.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zzq.gzhubu.top

C#:   // 手写递归
来源：http://xxt.xuanzx.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yyq.dianchejie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zlo.sufxvd.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ptt.shzxlz.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sjq.yueranfly.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zni.wangshuangyany.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lwx.chenzaomai.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ayu.smart0.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jhz.jqgufenzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cmr.xingfuxueyuan.xyz

================================================================================
来源：http://obn.jinyuanbaomall.cn

O. 并发与异步
来源：http://dgc.yj202588.top

================================================================================
来源：http://xax.zycfv.cn

[O01] 启动一个线程
来源：http://chc.jiagoushi.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qma.jinqigufen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wne.tarul.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dtj.chenzaomai.com

TS:   // 同 JS
来源：http://llu.yueranfly.top

Java: new Thread(() -> f()).start()
来源：http://cby.yanxiufei.cn

Go:   go f()
来源：http://nsk.hnxiangtu.top

Ruby: Thread.new { f }
来源：http://bqn.guowangkeji.top

C#:   Task.Run(() => F());
来源：http://qou.hesvh.cn

[O02] 使用线程池
来源：http://eud.birdmap.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yhy.smart0.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xgo.guannengcc.top

JS:   // worker_threads 线程池
来源：http://qov.xuetiantiany.cn

TS:   // worker_threads 线程池
来源：http://ykl.dianchejie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yws.tianlin.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pjn.zhixingplan.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cnw.fengsongda.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://knf.jinqigufen.top

[O03] 加锁保护共享数据
来源：http://vrg.gaohongyu789.top

Py:   with lock: shared += 1
来源：http://opb.pycfn.com

PHP:  // 用 flock() 做文件锁
来源：http://fnh.zycfv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jlj.316326.xyz

TS:   // 同 JS
来源：http://qch.zdbjq.cn

Java: synchronized (this) { shared++; }
来源：http://tpg.daria6918.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://swv.fktsv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kxk.sysykeji.top

C#:   lock (gate) { shared++; }
来源：http://oao.tarul.cn

[O04] 定义异步函数并等待
来源：http://fgw.shanyushiyangtech.top

Py:   async def f():⏎    await g()
来源：http://axz.meibo888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://raw.sufxvd.cn

JS:   async function f() { await g(); }
来源：http://epq.ywan-chungtsiang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rkh.shanyushiyangkeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://trt.hcnkem.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fqg.shzxlz.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wbd.dashuyun.cn

C#:   async Task F() { await G(); }
来源：http://srk.316326.xyz

[O05] 并发执行并等待全部完成
来源：http://iar.meibo888.top

Py:   asyncio.gather(*tasks)
来源：http://tfp.hysaishi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://erb.yangfankeji.com

JS:   await Promise.all(tasks)
来源：http://ing.smart0.xyz

TS:   await Promise.all(tasks)
来源：http://qsw.sysykeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mbr.tanke756.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mom.haohaochexian.top

Ruby: threads.map(&:join)
来源：http://kqc.chenlongwang.top

C#:   await Task.WhenAll(t1, t2)
来源：http://qoj.sxryk.cn

[O06] 使用进程池
来源：http://zre.9152youxi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://erk.ivvv.top

PHP:  // pcntl_fork 或多进程队列
来源：http://owy.shanyushiyangkeji.top

JS:   // child_process / cluster 模块
来源：http://bzb.jyoumei.cn

TS:   // child_process / cluster 模块
来源：http://hxr.gogol.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mop.bbcook.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sew.cdnleiting.top

Ruby: // fork 块
来源：http://zao.yongpay.top

C#:   Parallel.For
来源：http://hpl.zdbjq.cn

================================================================================
来源：http://nsm.jiagoushi.top

P. 常用工具函数
来源：http://xyn.yuxming.cn

================================================================================
来源：http://jle.yongpay.top

[P01] 生成 UUID
来源：http://taa.sysykeji.top

Py:   str(uuid.uuid4())
来源：http://spe.yueranfly.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dvc.jqgfzy.top

JS:   crypto.randomUUID()
来源：http://lst.wangdashe.top

TS:   crypto.randomUUID()
来源：http://ito.ehwqpu.com

Java: UUID.randomUUID().toString()
来源：http://dzi.ctjpmb.com

Go:   // 用 github.com/google/uuid
来源：http://tud.bbcook.cn

Ruby: SecureRandom.uuid
来源：http://ypa.tanke756.top

C#:   Guid.NewGuid().ToString()
来源：http://ifo.vqdsnc.cn

[P02] MD5 / SHA256 摘要
来源：http://src.epnwcf.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zqa.yongpay.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://twp.fanxiaobao.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://aal.pengpengdd.cyou

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://smh.9152youxi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://enn.nwbrower.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yxy.kuanghao11.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gua.jyoumei.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wgn.hcnkem.com

[P03] 生成短随机字符串
来源：http://jjk.iojbl.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uqn.ctjpmb.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://umu.sxryk.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jhs.haohaochexian.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fso.smart0.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sce.havefunace.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xkf.cashguo.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://bmr.birdmap.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qfq.shangyingyoupin.top

[P04] 求长度
来源：http://gom.hnxiangtu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://plq.feifeiyinyue.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://keg.ehwqpu.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vsa.havefunace.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hww.gotoacloud.top

Java: list.size();  map.size();  s.length()
来源：http://imv.quarkkingdee.top

Go:   len(arr);  len(m)
来源：http://dfu.yj202588.top

Ruby: x.length;  x.size
来源：http://xvu.ydjk.org.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://beu.meibo888.top

[P05] 判断两个对象内容是否相等
来源：http://qrc.hnxiangtu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://npe.sweek.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://iur.ivvv.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pia.iojbl.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fwl.52xcode.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://eup.mhx1999.top

Go:   reflect.DeepEqual(a, b)
来源：http://rim.fehbvm.com

Ruby: a == b
来源：http://rtk.sjlbkw.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cza.epnwcf.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zch.ywan-chungtsiang.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ufm.gzhubu.top

PHP:  if (empty($x)) {}
来源：http://mmj.cucudq.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://awf.zhaomingkeji.xyz

TS:   if (x == null) {}
来源：http://qjm.jqgufenzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wwa.sjlbkw.cn

Go:   if x == nil {}
来源：http://lsj.yueranfly.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://djl.nanxinkj.top

C#:   if (x is null) {}
来源：http://ovq.jinqigfzy.top

[P07] 防抖与节流
来源：http://dxe.iojbl.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://iqz.shuidangran.top

PHP:  // 手写时间戳比较
来源：http://tfw.shanyushiyangtech.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yhy.yuxming.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aon.c1oappe.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bkj.hnqzz.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lsk.jlsjyb.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qre.cqqwz.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ojk.shanyushiyangkeji.top

[P08] 处理浮点精度问题
来源：http://yzx.ehwqpu.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pux.haohaochexian.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ymn.zhiwuduotai.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xuf.jianghu66.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://otx.nanxuanxn.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gvu.cheryme.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://seq.fanxiaobao.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mcc.hnqzz.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zlj.chenjidiqi.icu

================================================================================
来源：http://nqn.fzhhl.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yjn.daxiang520.top

================================================================================
来源：http://sls.fzhhl.top

[Q01] 创建表
来源：http://acd.wangdashe.top

CREATE TABLE users (
来源：http://eww.smart0.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mpj.yj20258.top

name VARCHAR(50) NOT NULL,
来源：http://kwe.ywan-chungtsiang.top

email VARCHAR(100) UNIQUE,
来源：http://ltz.jqgufenzy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wlo.shanyushiyangtech.top

);
来源：http://gdd.zhaomingkeji.xyz

[Q02] 创建带外键的表
来源：http://nqc.shanyushiyangkeji.top

CREATE TABLE orders (
来源：http://mfc.bbcook.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://iby.shuidangran.top

user_id INT NOT NULL,
来源：http://xos.sjlbkw.cn

amount DECIMAL(10, 2),
来源：http://yeg.gotoacloud.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vgw.epnwcf.com

);
来源：http://ruv.guannengcc.top

[Q03] 增加列
来源：http://mnf.jlsjyb.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://eve.vqdsnc.cn

[Q04] 修改列类型
来源：http://mvm.ywan-chungtsiang.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ihb.hnqzz.top

[Q05] 重命名列
来源：http://ywi.jlsjyb.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dhg.aizwys.cn

[Q06] 删除列
来源：http://xho.yueranfly.top

ALTER TABLE users DROP COLUMN age;
来源：http://sfd.cucudq.cn

[Q07] 删除表
来源：http://piv.ppjwa.cn

DROP TABLE IF EXISTS orders;
来源：http://pel.shzxlz.cn

[Q08] 创建普通索引
来源：http://hhm.cheryme.top

CREATE INDEX idx_users_email ON users(email);
来源：http://kkk.tianlin.xyz

[Q09] 创建唯一索引
来源：http://jyi.dashuyun.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jdl.fengsongda.top

[Q10] 插入单行
来源：http://ljj.jyoumei.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lye.yongpay.top

[Q11] 一次插入多行
来源：http://eea.ppjwa.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bgv.ywan-chungtsiang.top

[Q12] 插入后取自增 ID
来源：http://yar.shanyushiyangtech.top

INSERT INTO users (name) VALUES ('C');
来源：http://rgq.c1oappe.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kwa.wangdashe.top

[Q13] 忽略重复插入
来源：http://oht.ppjwa.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://muc.feifeiyinyue.top

[Q14] 存在则更新（upsert）
来源：http://paj.jianghu66.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tje.redwolf501.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ksu.fehbvm.com

[Q15] 查询全部
来源：http://cyu.zhongyouzk.top

SELECT * FROM users;
来源：http://lyi.quarkkingdee.top

[Q16] 查询指定列
来源：http://lxk.jinghuilouyu.cn

SELECT id, name FROM users;
来源：http://osq.shzxlz.cn

[Q17] 条件查询
来源：http://xlx.pengpengdd.cyou

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tpd.cqqwz.cn

[Q18] 模糊匹配
来源：http://elk.zdqjudy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hhn.havefunace.top

[Q19] 范围查询
来源：http://mqn.shanyushiyangkeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jce.daria6918.cn

[Q20] IN 列表
来源：http://qfb.aizwys.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nrh.zhoulong.xyz

[Q21] 空值判断
来源：http://fxa.kuanghao11.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ana.zhijiandao.cn

[Q22] 排序
来源：http://zpn.yanxiufei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pgw.cqqwz.cn

[Q23] 分页
来源：http://lzh.hnqzz.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://azi.kuanghao11.cn

[Q24] 去重
来源：http://had.yangfankeji.com

SELECT DISTINCT city FROM users;
来源：http://ovv.kuanghao11.cn

[Q25] 只取前 N 条
来源：http://wgo.mhx1999.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wgk.cheryme.top

[Q26] 计数
来源：http://wrh.gaohongyu789.top

SELECT COUNT(*) FROM users;
来源：http://qgj.andypj.xyz

[Q27] 条件计数
来源：http://cwn.0kj1m.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ogi.redwolf501.top

[Q28] 求和与平均
来源：http://jaz.gogol.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://swk.0kj1m.cn

[Q29] 最大最小值
来源：http://lgl.tian-w.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://aoq.yj202588.top

[Q30] 分组统计
来源：http://tce.shanyushiyangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ddy.yongpay.top

[Q31] 分组后过滤
来源：http://msg.hnqzz.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gcb.hnqzz.top

[Q32] 分组拼接字符串
来源：http://wmx.gaohongyu789.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://avx.yueranfly.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lxh.shangyingyoupin.top

[Q33] 多列分组
来源：http://tpp.yangfankeji.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://psf.cheryme.top

[Q34] 每组取第一条
来源：http://itr.nanxuanxn.top

SELECT * FROM (
来源：http://yqz.c1oappe.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ivw.haohaochexian.top

) t WHERE rn = 1;
来源：http://wjk.jlsjyb.cn

[Q35] 内连接
来源：http://zgw.cdnleiting.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vws.svipenyu.cn

[Q36] 左连接
来源：http://vtz.9152youxi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://czt.andypj.xyz

[Q37] 右连接
来源：http://jub.hongshengwenyu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jge.9152youxi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://cmu.havefunace.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://spq.yvedp.cn

[Q39] 自连接（查上下级）
来源：http://irb.cucudq.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xxk.xuanzx.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://acj.dianchejie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ofv.tian-w.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nlo.cashguo.top

[Q41] 多表连接
来源：http://zxo.gaohongyu789.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://rqi.bbcook.cn

JOIN users u ON u.id = o.user_id
来源：http://wki.tianlin.xyz

JOIN products p ON p.id = o.product_id;
来源：http://jqr.aizwys.cn

[Q42] 连接条件附加过滤
来源：http://uto.ybcxt.top

SELECT u.name, o.amount FROM users u
来源：http://kah.chenzaomai.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yof.sufxvd.cn

[Q43] 标量子查询
来源：http://fhy.gaohongyu789.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://foe.fehbvm.com

[Q44] IN 子查询
来源：http://mbc.fehbvm.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cok.jyoumei.cn

[Q45] EXISTS 判断存在
来源：http://kot.yongpay.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fte.dianchejie.cn


<!-- 参考信息 -->