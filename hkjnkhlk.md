代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://fbw.birdmap.top

TS:   s === [...s].reverse().join("")
来源：http://yrh.shuidangran.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wme.tanke756.top

Go:   // 双指针从两端比较
来源：http://rqa.dianchejie.cn

Ruby: s == s.reverse
来源：http://upy.iojbl.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vhx.feifeiyinyue.top

[N07] 两数之和（返回下标）
来源：http://hnk.bjfxy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tah.guowangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gxf.shangyingyoupin.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vat.chenlongwang.top

TS:   // 手写 Map<string, number>
来源：http://qbc.birdmap.top

Java: // 手写 HashMap
来源：http://wmy.sweek.top

Go:   // 手写 map[int]int
来源：http://unz.cucudq.cn

Ruby: // 手写 Hash
来源：http://scq.jqgfzy.top

C#:   // 手写 Dictionary<int, int>
来源：http://rhs.redwolf501.top

[N08] 生成全排列
来源：http://nfi.316326.xyz

Py:   itertools.permutations(arr)
来源：http://knk.jinqigfzy.top

PHP:  // 手写递归交换
来源：http://uxv.shanyushiyangkeji.top

JS:   // 手写回溯递归
来源：http://pto.svipenyu.cn

TS:   // 手写回溯递归
来源：http://sjh.sufxvd.cn

Java: // 手写回溯递归
来源：http://osy.c1oappe.top

Go:   // 手写回溯递归
来源：http://opo.yvedp.cn

Ruby: arr.permutation.to_a
来源：http://ojq.jinqigufen.top

C#:   // 手写回溯递归
来源：http://krl.ppjwa.cn

[N09] 栈与队列
来源：http://etj.zhixingplan.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://idi.ivvv.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hoi.xingfuxueyuan.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jqx.hammf.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dcb.wangshuangyany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fgz.yfazqb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fnh.chenjidiqi.icu

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xfk.ppjwa.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wps.xinyue.icu

[N10] 链表节点定义
来源：http://oxb.yj20258.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hyg.jinghuilouyu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kyw.aibaodan.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dss.daxiang520.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qsn.aizwys.cn

Java: class Node { int v; Node next; }
来源：http://ubb.tian-w.cn

Go:   type Node struct { V int; Next *Node }
来源：http://btn.ybcxt.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zsr.smart0.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://eet.gaohongyu789.top

[N11] 二叉树中序遍历
来源：http://ecf.shangyingyoupin.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://siv.chenjidiqi.icu

PHP:  // 手写递归函数
来源：http://qlw.fzhhl.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kvx.316326.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wce.dianchejie.cn

Java: // 手写递归
来源：http://iaw.snrcjt.cn

Go:   // 手写递归
来源：http://qaf.hfpthk.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ifn.ivvv.top

C#:   // 手写递归
来源：http://tqd.tarul.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oms.yuanzhike.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://raz.xylfe.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://myt.redwolf501.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bdm.bjfxy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://agk.dianchejie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gbt.ppjwa.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ycu.jiagoushi.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wvn.cqqwz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kxa.0kj1m.cn

================================================================================
来源：http://jbg.cdnleiting.top

O. 并发与异步
来源：http://fek.hammf.cn

================================================================================
来源：http://htg.nanxinkj.top

[O01] 启动一个线程
来源：http://uih.9152youxi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zyl.yongpay.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mfc.haohaochexian.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://has.chenzaomai.com

TS:   // 同 JS
来源：http://dbf.shuidangran.top

Java: new Thread(() -> f()).start()
来源：http://xqm.xinyue.icu

Go:   go f()
来源：http://scn.yfazqb.com

Ruby: Thread.new { f }
来源：http://wmz.guowangkeji.top

C#:   Task.Run(() => F());
来源：http://puk.cqqwz.cn

[O02] 使用线程池
来源：http://tcm.kuanghao11.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jci.ppjwa.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nvo.sufxvd.cn

JS:   // worker_threads 线程池
来源：http://cqm.sweek.top

TS:   // worker_threads 线程池
来源：http://qif.ppjwa.cn

Java: Executors.newFixedThreadPool(4)
来源：http://slp.hcnkem.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://shu.wangshuangyany.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uli.bbcook.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://eup.yvedp.cn

[O03] 加锁保护共享数据
来源：http://frb.ydzc1.top

Py:   with lock: shared += 1
来源：http://wzr.snrcjt.cn

PHP:  // 用 flock() 做文件锁
来源：http://dmm.epnwcf.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jaf.sufxvd.cn

TS:   // 同 JS
来源：http://ufk.ehwqpu.com

Java: synchronized (this) { shared++; }
来源：http://hnr.fehbvm.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hmv.ywan-chungtsiang.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://obw.fzhhl.top

C#:   lock (gate) { shared++; }
来源：http://guj.jqgfzy.top

[O04] 定义异步函数并等待
来源：http://epg.quarkkingdee.top

Py:   async def f():⏎    await g()
来源：http://jrr.haohaochexian.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tcq.ehwqpu.com

JS:   async function f() { await g(); }
来源：http://ykc.birdmap.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://fju.hammf.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hcx.nwbrower.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eax.tarul.cn

Ruby: # 用 Fiber 或 async gem
来源：http://etj.nwbrower.top

C#:   async Task F() { await G(); }
来源：http://awd.hcnkem.com

[O05] 并发执行并等待全部完成
来源：http://eei.shanyushiyangkeji.top

Py:   asyncio.gather(*tasks)
来源：http://uaz.wangdashe.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://arv.dashuyun.cn

JS:   await Promise.all(tasks)
来源：http://mwo.fanxiaobao.xyz

TS:   await Promise.all(tasks)
来源：http://ymj.kuanghao11.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://psp.zdqjudy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kyq.gzhubu.top

Ruby: threads.map(&:join)
来源：http://nuq.ydzc1.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fbn.andypj.xyz

[O06] 使用进程池
来源：http://glq.hysaishi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://est.bjfxy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://okf.ctjpmb.com

JS:   // child_process / cluster 模块
来源：http://qte.cqqwz.cn

TS:   // child_process / cluster 模块
来源：http://rhm.shuidangran.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gau.yuxming.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hso.gotoacloud.top

Ruby: // fork 块
来源：http://vaa.wangshuangyany.cn

C#:   Parallel.For
来源：http://lxa.shanyushiyangtech.top

================================================================================
来源：http://mgg.bjfxy.top

P. 常用工具函数
来源：http://vgs.fktsv.cn

================================================================================
来源：http://qkn.hesvh.cn

[P01] 生成 UUID
来源：http://fct.zhijiandao.cn

Py:   str(uuid.uuid4())
来源：http://cyy.pengpengdd.cyou

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wzr.ydjk.org.cn

JS:   crypto.randomUUID()
来源：http://ofy.ctjpmb.com

TS:   crypto.randomUUID()
来源：http://jzc.jinqigfzy.top

Java: UUID.randomUUID().toString()
来源：http://wbg.hnqzz.top

Go:   // 用 github.com/google/uuid
来源：http://gmm.fanxiaobao.xyz

Ruby: SecureRandom.uuid
来源：http://sfz.chenzaomai.com

C#:   Guid.NewGuid().ToString()
来源：http://rfk.hongshengwenyu.top

[P02] MD5 / SHA256 摘要
来源：http://pgw.guowangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xqd.zdqjudy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://toe.hongshengwenyu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xpp.mhx1999.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nam.yfazqb.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jeo.jianghu66.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jdl.0kj1m.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tox.yanxiufei.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pnv.pengpengdd.cyou

[P03] 生成短随机字符串
来源：http://bdp.zhaomingkeji.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zzo.redwolf501.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cni.kuanghao11.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qcm.pengpengdd.cyou

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vkj.sufxvd.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vmt.cashguo.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pbf.jinqigfzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://cid.yj20258.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vur.epnwcf.com

[P04] 求长度
来源：http://itp.yj202588.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://azz.uphjek.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cwt.zycfv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nym.yj202588.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cxp.zhaomingkeji.xyz

Java: list.size();  map.size();  s.length()
来源：http://ilc.zhongyouzk.top

Go:   len(arr);  len(m)
来源：http://fdx.ydjk.org.cn

Ruby: x.length;  x.size
来源：http://pjj.aibaodan.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ofa.epnwcf.com

[P05] 判断两个对象内容是否相等
来源：http://xxf.yvedp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sos.shanyushiyangkeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mxc.pycfn.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hta.feifeiyinyue.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tnb.nwbrower.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hbp.zhiwuduotai.top

Go:   reflect.DeepEqual(a, b)
来源：http://atc.andypj.xyz

Ruby: a == b
来源：http://nps.haohaochexian.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jtr.vqdsnc.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lhm.cheryme.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xhz.jianghu66.top

PHP:  if (empty($x)) {}
来源：http://alk.yueranfly.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ewc.fengsongda.top

TS:   if (x == null) {}
来源：http://kjz.yj20258.top

Java: if (x == null || x.isEmpty()) {}
来源：http://lrx.yuanzhike.top

Go:   if x == nil {}
来源：http://ulu.tanke756.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mey.fzhhl.top

C#:   if (x is null) {}
来源：http://vkg.jinghuilouyu.cn

[P07] 防抖与节流
来源：http://lle.yangfankeji.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pzy.yfazqb.com

PHP:  // 手写时间戳比较
来源：http://yxu.cqqwz.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ddq.zdqjudy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://quj.hnqzz.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ydj.pycfn.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tei.yuanzhike.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ywm.jqgfzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kuu.52xcode.cn

[P08] 处理浮点精度问题
来源：http://nmp.pengpengdd.cyou

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://glr.chenzaomai.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tsu.gogol.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xvh.meibo888.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://abw.jinyuanbaomall.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tye.zhongyouzk.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rov.ywan-chungtsiang.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zzh.c1oappe.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dgf.aibaodan.cn

================================================================================
来源：http://dqb.andypj.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yvk.chenlongwang.top

================================================================================
来源：http://awh.andypj.xyz

[Q01] 创建表
来源：http://gyq.epnwcf.com

CREATE TABLE users (
来源：http://ifx.iojbl.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fqw.shangyingyoupin.top

name VARCHAR(50) NOT NULL,
来源：http://ckc.gotoacloud.top

email VARCHAR(100) UNIQUE,
来源：http://nwk.meibo888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bho.tarul.cn

);
来源：http://svl.hnxiangtu.top

[Q02] 创建带外键的表
来源：http://nol.andypj.xyz

CREATE TABLE orders (
来源：http://lxi.yueranfly.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mro.cdnleiting.top

user_id INT NOT NULL,
来源：http://lvu.tianlin.xyz

amount DECIMAL(10, 2),
来源：http://umi.shanyushiyangkeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lfy.uphjek.com

);
来源：http://btn.sysykeji.top

[Q03] 增加列
来源：http://csd.ppjwa.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ziv.cdnleiting.top

[Q04] 修改列类型
来源：http://tis.cdnleiting.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ghr.shuidangran.top

[Q05] 重命名列
来源：http://drn.gotoacloud.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bzo.sxryk.cn

[Q06] 删除列
来源：http://spk.hnxiangtu.top

ALTER TABLE users DROP COLUMN age;
来源：http://ykn.aibaodan.cn

[Q07] 删除表
来源：http://grp.xziqi.cn

DROP TABLE IF EXISTS orders;
来源：http://sqi.shzxlz.cn

[Q08] 创建普通索引
来源：http://evr.hysaishi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hja.svipenyu.cn

[Q09] 创建唯一索引
来源：http://xsj.zhixingplan.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://voj.bjfxy.top

[Q10] 插入单行
来源：http://qby.yj20258888.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://des.fzhhl.top

[Q11] 一次插入多行
来源：http://mzf.sxryk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wmz.xingfuxueyuan.xyz

[Q12] 插入后取自增 ID
来源：http://qkr.hesvh.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ceo.ybcxt.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lbj.tian-w.cn

[Q13] 忽略重复插入
来源：http://gei.zhiwuduotai.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dag.zycfv.cn

[Q14] 存在则更新（upsert）
来源：http://clx.shangyingyoupin.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oxx.chenlongwang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zjb.tianlin.xyz

[Q15] 查询全部
来源：http://kmj.yonumen.top

SELECT * FROM users;
来源：http://cbw.havefunace.top

[Q16] 查询指定列
来源：http://ctg.ydzc1.top

SELECT id, name FROM users;
来源：http://ozf.vqdsnc.cn

[Q17] 条件查询
来源：http://qio.redwolf501.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hvb.jqgfzy.top

[Q18] 模糊匹配
来源：http://vww.316326.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://iqp.yangfankeji.com

[Q19] 范围查询
来源：http://bbk.xingfuxueyuan.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://trs.zhixingplan.top

[Q20] IN 列表
来源：http://mfi.chenjidiqi.icu

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://chx.shuidangran.top

[Q21] 空值判断
来源：http://snv.zhaomingkeji.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://sqv.daria6918.cn

[Q22] 排序
来源：http://htc.gaohongyu789.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://npq.jlsjyb.cn

[Q23] 分页
来源：http://zou.ybcxt.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gvw.yj20258888.top

[Q24] 去重
来源：http://cus.sjlbkw.cn

SELECT DISTINCT city FROM users;
来源：http://zye.tian-w.cn

[Q25] 只取前 N 条
来源：http://fkj.chenjidiqi.icu

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hbx.yuxming.cn

[Q26] 计数
来源：http://iek.sweek.top

SELECT COUNT(*) FROM users;
来源：http://vpc.dashuyun.cn

[Q27] 条件计数
来源：http://xyc.zhoulong.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lfo.chenlongwang.top

[Q28] 求和与平均
来源：http://qxr.haohaochexian.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uaq.jinqigufen.top

[Q29] 最大最小值
来源：http://wod.zhaomingkeji.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://res.yuanzhike.top

[Q30] 分组统计
来源：http://ckt.jinqigfzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ayc.jinyuanbaomall.cn

[Q31] 分组后过滤
来源：http://wnv.xuetiantiany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jql.yj20258888.top

[Q32] 分组拼接字符串
来源：http://jkq.epnwcf.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pbv.guannengcc.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cfg.tanke756.top

[Q33] 多列分组
来源：http://pon.yj202588.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vny.shanyushiyangtech.top

[Q34] 每组取第一条
来源：http://phw.jinqigfzy.top

SELECT * FROM (
来源：http://plj.yfazqb.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vvy.52xcode.cn

) t WHERE rn = 1;
来源：http://lrd.zycfv.cn

[Q35] 内连接
来源：http://qtn.guannengcc.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vkz.ydjk.org.cn

[Q36] 左连接
来源：http://cyb.vqdsnc.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jad.jqgufenzy.top

[Q37] 右连接
来源：http://eqh.ppjwa.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nue.andypj.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://lsz.wangshuangyany.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uon.ybcxt.top

[Q39] 自连接（查上下级）
来源：http://qvg.jqgufenzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://fgf.feifeiyinyue.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://uqy.birdmap.top

[Q40] 交叉连接（笛卡尔积）
来源：http://wnj.jianghu66.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lxg.mhx1999.top

[Q41] 多表连接
来源：http://ueo.c1oappe.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://eht.dianchejie.cn

JOIN users u ON u.id = o.user_id
来源：http://ceh.redwolf501.top

JOIN products p ON p.id = o.product_id;
来源：http://eri.yanxiufei.cn

[Q42] 连接条件附加过滤
来源：http://fqj.havefunace.top

SELECT u.name, o.amount FROM users u
来源：http://ero.quarkkingdee.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://udb.cheryme.top

[Q43] 标量子查询
来源：http://fei.hammf.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://exm.havefunace.top


<!-- 参考信息 -->