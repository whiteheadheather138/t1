代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://gfs.ydzc1.top

TS:   s === [...s].reverse().join("")
来源：http://nul.hongshengwenyu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://alb.pycfn.com

Go:   // 双指针从两端比较
来源：http://nzp.9152youxi.cn

Ruby: s == s.reverse
来源：http://ghd.hnqzz.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://psq.guannengcc.top

[N07] 两数之和（返回下标）
来源：http://wav.cucudq.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://anw.shangyingyoupin.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://edw.yj20258888.top

JS:   // 手写 Map：map.set(v, i)
来源：http://oma.jlsjyb.cn

TS:   // 手写 Map<string, number>
来源：http://our.smart0.xyz

Java: // 手写 HashMap
来源：http://ffo.jinqigfzy.top

Go:   // 手写 map[int]int
来源：http://ozc.daria6918.cn

Ruby: // 手写 Hash
来源：http://biy.snrcjt.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kyo.hammf.cn

[N08] 生成全排列
来源：http://nse.fengsongda.top

Py:   itertools.permutations(arr)
来源：http://qcb.jqgufenzy.top

PHP:  // 手写递归交换
来源：http://bwv.zhoulong.xyz

JS:   // 手写回溯递归
来源：http://hvt.chenzaomai.com

TS:   // 手写回溯递归
来源：http://xmq.ppjwa.cn

Java: // 手写回溯递归
来源：http://saz.chenlongwang.top

Go:   // 手写回溯递归
来源：http://gsq.xziqi.cn

Ruby: arr.permutation.to_a
来源：http://hol.ydzc1.top

C#:   // 手写回溯递归
来源：http://pxr.xingfuxueyuan.xyz

[N09] 栈与队列
来源：http://yzx.sysykeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qkc.zhijiandao.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yrm.wangshuangyany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://prk.chenjidiqi.icu

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uyq.redwolf501.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mxs.shanyushiyangkeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bxg.ywan-chungtsiang.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pqy.jianghu66.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rqq.zdbjq.cn

[N10] 链表节点定义
来源：http://xjr.redwolf501.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yab.yanxiufei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vpp.yonumen.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hfp.jianghu66.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://prg.jqgufenzy.top

Java: class Node { int v; Node next; }
来源：http://qrm.zdbjq.cn

Go:   type Node struct { V int; Next *Node }
来源：http://spu.316326.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://vpc.tianlin.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://mru.aibaodan.cn

[N11] 二叉树中序遍历
来源：http://agu.sjlbkw.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pct.fehbvm.com

PHP:  // 手写递归函数
来源：http://ejl.jlsjyb.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://txs.xuetiantiany.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wrj.chenzaomai.com

Java: // 手写递归
来源：http://abr.svipenyu.cn

Go:   // 手写递归
来源：http://xzb.yvedp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bjq.meibo888.top

C#:   // 手写递归
来源：http://pig.jyoumei.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ovt.fktsv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ylo.nwbrower.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ehw.hcnkem.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qok.redwolf501.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mye.52xcode.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nxg.uphjek.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ole.xuanzx.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://crd.wangshuangyany.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mti.jqgufenzy.top

================================================================================
来源：http://gso.cashguo.top

O. 并发与异步
来源：http://zfw.iojbl.cn

================================================================================
来源：http://lzj.nwbrower.top

[O01] 启动一个线程
来源：http://cdz.hammf.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://afo.shzxlz.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jhy.haohaochexian.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zjf.jlsjyb.cn

TS:   // 同 JS
来源：http://zaq.gzhubu.top

Java: new Thread(() -> f()).start()
来源：http://rgz.yuxming.cn

Go:   go f()
来源：http://ggd.wangshuangyany.cn

Ruby: Thread.new { f }
来源：http://ano.gotoacloud.top

C#:   Task.Run(() => F());
来源：http://ped.kuanghao11.cn

[O02] 使用线程池
来源：http://yjr.zhaomingkeji.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ima.uphjek.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://esu.xylfe.cn

JS:   // worker_threads 线程池
来源：http://veq.ctjpmb.com

TS:   // worker_threads 线程池
来源：http://yml.zhijiandao.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hic.hesvh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://seb.guowangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xfw.chenlongwang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uiu.kuanghao11.cn

[O03] 加锁保护共享数据
来源：http://ylk.yj20258888.top

Py:   with lock: shared += 1
来源：http://kmh.tian-w.cn

PHP:  // 用 flock() 做文件锁
来源：http://vdb.xingfuxueyuan.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uif.yuxming.cn

TS:   // 同 JS
来源：http://aoq.havefunace.top

Java: synchronized (this) { shared++; }
来源：http://fde.hnqzz.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fsx.quarkkingdee.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://mnk.hnqzz.top

C#:   lock (gate) { shared++; }
来源：http://pfj.kuanghao11.cn

[O04] 定义异步函数并等待
来源：http://bgk.birdmap.top

Py:   async def f():⏎    await g()
来源：http://tty.jianghu66.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bqd.guannengcc.top

JS:   async function f() { await g(); }
来源：http://uhr.hfpthk.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zqx.shanyushiyangkeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nkb.pycfn.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ziw.shangyingyoupin.top

Ruby: # 用 Fiber 或 async gem
来源：http://tkz.xingfuxueyuan.xyz

C#:   async Task F() { await G(); }
来源：http://xjd.guowangkeji.top

[O05] 并发执行并等待全部完成
来源：http://eqd.jqgfzy.top

Py:   asyncio.gather(*tasks)
来源：http://ywf.andypj.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fcx.zhiwuduotai.top

JS:   await Promise.all(tasks)
来源：http://wmj.shuidangran.top

TS:   await Promise.all(tasks)
来源：http://hrf.daxiang520.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gab.hammf.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sbr.hysaishi.cn

Ruby: threads.map(&:join)
来源：http://okm.yj20258.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mhy.cqqwz.cn

[O06] 使用进程池
来源：http://hrc.yvedp.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rnn.gzhubu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://jxc.pengpengdd.cyou

JS:   // child_process / cluster 模块
来源：http://jjb.havefunace.top

TS:   // child_process / cluster 模块
来源：http://zxp.bbcook.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hos.smart0.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kti.sxryk.cn

Ruby: // fork 块
来源：http://ljs.hnqzz.top

C#:   Parallel.For
来源：http://lqb.cucudq.cn

================================================================================
来源：http://bdl.chenzaomai.com

P. 常用工具函数
来源：http://ypk.ydzc1.top

================================================================================
来源：http://dks.cdnleiting.top

[P01] 生成 UUID
来源：http://glp.cdnleiting.top

Py:   str(uuid.uuid4())
来源：http://xqo.xuanzx.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pas.jinqigufen.top

JS:   crypto.randomUUID()
来源：http://zev.bjfxy.top

TS:   crypto.randomUUID()
来源：http://fja.wangshuangyany.cn

Java: UUID.randomUUID().toString()
来源：http://noz.zhengqikj.top

Go:   // 用 github.com/google/uuid
来源：http://ikw.chenjidiqi.icu

Ruby: SecureRandom.uuid
来源：http://dcf.quarkkingdee.top

C#:   Guid.NewGuid().ToString()
来源：http://cby.shuidangran.top

[P02] MD5 / SHA256 摘要
来源：http://zii.9152youxi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xse.xuetiantiany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fkj.yuxming.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://evz.zdqjudy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lxj.9152youxi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ujw.chenjidiqi.icu

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mzs.yueranfly.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pik.fengsongda.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://amp.snrcjt.cn

[P03] 生成短随机字符串
来源：http://mvi.vqdsnc.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yqh.0kj1m.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ntu.c1oappe.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oet.hfpthk.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hpo.xinyue.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tmp.ehwqpu.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pxk.ivvv.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://yeg.jiagoushi.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nll.dashuyun.cn

[P04] 求长度
来源：http://jkw.aizwys.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vqs.ppjwa.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gwu.mhx1999.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vwf.nwbrower.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hak.nwbrower.top

Java: list.size();  map.size();  s.length()
来源：http://sjj.shangyingyoupin.top

Go:   len(arr);  len(m)
来源：http://okw.daxiang520.top

Ruby: x.length;  x.size
来源：http://cab.cheryme.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://qea.sysykeji.top

[P05] 判断两个对象内容是否相等
来源：http://feb.ehwqpu.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://vah.hesvh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pfr.gzhubu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xip.havefunace.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://syd.andypj.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://klf.zycfv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yxs.vehdjk.com

Ruby: a == b
来源：http://mpv.nwbrower.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://led.xuetiantiany.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ern.wangdashe.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gmi.yonumen.top

PHP:  if (empty($x)) {}
来源：http://nnt.xziqi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vih.0kj1m.cn

TS:   if (x == null) {}
来源：http://frc.bbcook.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wgq.zhixingplan.top

Go:   if x == nil {}
来源：http://bnx.zycfv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dda.pengpengdd.cyou

C#:   if (x is null) {}
来源：http://mox.guowangkeji.top

[P07] 防抖与节流
来源：http://flo.zhoulong.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://khi.cheryme.top

PHP:  // 手写时间戳比较
来源：http://ipz.feifeiyinyue.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zwr.havefunace.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jyi.fehbvm.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gvp.xinyue.icu

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://egj.ywan-chungtsiang.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://luz.c1oappe.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dak.xziqi.cn

[P08] 处理浮点精度问题
来源：http://nrd.sufxvd.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://okt.nanxuanxn.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bds.jinyuanbaomall.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kav.havefunace.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://skc.chenjidiqi.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://btp.yueranfly.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fbu.zhiwuduotai.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zva.zhoulong.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rqc.gzhubu.top

================================================================================
来源：http://zth.nanxinkj.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://miv.ehwqpu.com

================================================================================
来源：http://vlz.sufxvd.cn

[Q01] 创建表
来源：http://prc.redwolf501.top

CREATE TABLE users (
来源：http://hcp.bjfxy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bqc.smart0.xyz

name VARCHAR(50) NOT NULL,
来源：http://scc.aizwys.cn

email VARCHAR(100) UNIQUE,
来源：http://lth.shanyushiyangkeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qom.cdnleiting.top

);
来源：http://gdt.zhongyouzk.top

[Q02] 创建带外键的表
来源：http://nny.nanxinkj.top

CREATE TABLE orders (
来源：http://xuu.wangshuangyany.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rdb.gzhubu.top

user_id INT NOT NULL,
来源：http://xuo.nanxinkj.top

amount DECIMAL(10, 2),
来源：http://hyk.gaohongyu789.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mew.gaohongyu789.top

);
来源：http://vaw.yanxiufei.cn

[Q03] 增加列
来源：http://xue.52xcode.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dbb.vehdjk.com

[Q04] 修改列类型
来源：http://rpj.ivvv.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://edq.ybcxt.top

[Q05] 重命名列
来源：http://phz.gotoacloud.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fju.vqdsnc.cn

[Q06] 删除列
来源：http://nwm.chenlongwang.top

ALTER TABLE users DROP COLUMN age;
来源：http://qcs.shangyingyoupin.top

[Q07] 删除表
来源：http://qxx.ehwqpu.com

DROP TABLE IF EXISTS orders;
来源：http://ajy.sjlbkw.cn

[Q08] 创建普通索引
来源：http://kil.vqdsnc.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://mix.ydjk.org.cn

[Q09] 创建唯一索引
来源：http://vkr.tanke756.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://deh.gaohongyu789.top

[Q10] 插入单行
来源：http://fal.zhengqikj.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ohs.zhoulong.xyz

[Q11] 一次插入多行
来源：http://nox.fktsv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zhj.mhx1999.top

[Q12] 插入后取自增 ID
来源：http://lea.9152youxi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qim.ivvv.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sbp.jinqigufen.top

[Q13] 忽略重复插入
来源：http://whb.zdqjudy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hmb.fktsv.cn

[Q14] 存在则更新（upsert）
来源：http://tpx.bjfxy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cxq.shzxlz.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://woz.iojbl.cn

[Q15] 查询全部
来源：http://zeh.jiagoushi.top

SELECT * FROM users;
来源：http://ofe.sxryk.cn

[Q16] 查询指定列
来源：http://yhw.redwolf501.top

SELECT id, name FROM users;
来源：http://ymr.hcnkem.com

[Q17] 条件查询
来源：http://iic.yonumen.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qkg.hnxiangtu.top

[Q18] 模糊匹配
来源：http://vtd.yangfankeji.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://evr.tarul.cn

[Q19] 范围查询
来源：http://yef.mhx1999.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ude.quarkkingdee.top

[Q20] IN 列表
来源：http://dmg.meibo888.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rea.chenjidiqi.icu

[Q21] 空值判断
来源：http://znn.yuxming.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nkj.guannengcc.top

[Q22] 排序
来源：http://jiz.hcnkem.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://opo.xziqi.cn

[Q23] 分页
来源：http://vil.xziqi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jiy.hnxiangtu.top

[Q24] 去重
来源：http://sqt.yueranfly.top

SELECT DISTINCT city FROM users;
来源：http://qbl.pengpengdd.cyou

[Q25] 只取前 N 条
来源：http://ysk.kuanghao11.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zmp.haohaochexian.top

[Q26] 计数
来源：http://kwb.chenlongwang.top

SELECT COUNT(*) FROM users;
来源：http://rhy.cheryme.top

[Q27] 条件计数
来源：http://cli.hcnkem.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hyb.fanxiaobao.xyz

[Q28] 求和与平均
来源：http://tds.shanyushiyangtech.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jjw.zdbjq.cn

[Q29] 最大最小值
来源：http://uzq.chenzaomai.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://sov.fehbvm.com

[Q30] 分组统计
来源：http://wnr.xuetiantiany.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ndx.cucudq.cn

[Q31] 分组后过滤
来源：http://pvv.sufxvd.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gfe.yonumen.top

[Q32] 分组拼接字符串
来源：http://rry.yangfankeji.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cjo.sufxvd.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pkf.jyoumei.cn

[Q33] 多列分组
来源：http://ecm.vehdjk.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vzx.c1oappe.top

[Q34] 每组取第一条
来源：http://mcm.zhaomingkeji.xyz

SELECT * FROM (
来源：http://vjd.jqgufenzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uag.wangshuangyany.cn

) t WHERE rn = 1;
来源：http://mjq.shangyingyoupin.top

[Q35] 内连接
来源：http://sqi.ppjwa.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kzh.shzxlz.cn

[Q36] 左连接
来源：http://ioq.bjfxy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uvt.shzxlz.cn

[Q37] 右连接
来源：http://qvk.c1oappe.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xag.aizwys.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ydf.cqqwz.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://adi.zdbjq.cn

[Q39] 自连接（查上下级）
来源：http://msj.guowangkeji.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://tzu.aizwys.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://brp.tanke756.top

[Q40] 交叉连接（笛卡尔积）
来源：http://tin.zdbjq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ahu.uphjek.com

[Q41] 多表连接
来源：http://dxb.shangyingyoupin.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ujp.chenzaomai.com

JOIN users u ON u.id = o.user_id
来源：http://ngu.sysykeji.top

JOIN products p ON p.id = o.product_id;
来源：http://ddf.xingfuxueyuan.xyz

[Q42] 连接条件附加过滤
来源：http://bfz.redwolf501.top

SELECT u.name, o.amount FROM users u
来源：http://iwp.chenjidiqi.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fmg.cdnleiting.top

[Q43] 标量子查询
来源：http://vnd.aibaodan.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://piz.jianghu66.top


<!-- 参考信息 -->