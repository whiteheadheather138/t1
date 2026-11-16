代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ekw.52xcode.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qbr.yangfankeji.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fgo.meibo888.top

Ruby: a.gcd(b)
来源：http://skz.ppjwa.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://chf.cashguo.top

[N06] 判断回文字符串
来源：http://nzt.hnqzz.top

Py:   s == s[::-1]
来源：http://tgq.snrcjt.cn

PHP:  $s === strrev($s);
来源：http://jhe.cqqwz.cn

JS:   s === [...s].reverse().join("")
来源：http://zup.hywenlv.cn

TS:   s === [...s].reverse().join("")
来源：http://uve.sufxvd.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sau.hammf.cn

Go:   // 双指针从两端比较
来源：http://qgi.52xcode.cn

Ruby: s == s.reverse
来源：http://tje.iojbl.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://opj.shanyushiyangkeji.top

[N07] 两数之和（返回下标）
来源：http://gip.sxryk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zmz.nanxuanxn.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qej.smart0.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://pnr.aibaodan.cn

TS:   // 手写 Map<string, number>
来源：http://dwx.zhixingplan.top

Java: // 手写 HashMap
来源：http://has.jiagoushi.top

Go:   // 手写 map[int]int
来源：http://lel.hfpthk.cn

Ruby: // 手写 Hash
来源：http://ryv.vqdsnc.cn

C#:   // 手写 Dictionary<int, int>
来源：http://utk.redwolf501.top

[N08] 生成全排列
来源：http://tae.xylfe.cn

Py:   itertools.permutations(arr)
来源：http://tnx.shangyingyoupin.top

PHP:  // 手写递归交换
来源：http://zwh.daxiang520.top

JS:   // 手写回溯递归
来源：http://ztv.svipenyu.cn

TS:   // 手写回溯递归
来源：http://mtd.zhijiandao.cn

Java: // 手写回溯递归
来源：http://dzh.dashuyun.cn

Go:   // 手写回溯递归
来源：http://snc.cashguo.top

Ruby: arr.permutation.to_a
来源：http://hva.meibo888.top

C#:   // 手写回溯递归
来源：http://spm.hywenlv.cn

[N09] 栈与队列
来源：http://mpe.chenzaomai.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://esz.dianchejie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://owm.bjfxy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fow.pycfn.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gsy.jqgfzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://apf.fehbvm.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ubf.cheryme.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cjp.cashguo.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jss.hywenlv.cn

[N10] 链表节点定义
来源：http://hzw.ydjk.org.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ell.hesvh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kmy.meibo888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bsq.bjfxy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xbw.xingfuxueyuan.xyz

Java: class Node { int v; Node next; }
来源：http://yrc.jqgfzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://vwx.hesvh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://nea.fengsongda.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bto.svipenyu.cn

[N11] 二叉树中序遍历
来源：http://lhw.zhaomingkeji.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ojm.yongpay.top

PHP:  // 手写递归函数
来源：http://iwo.cashguo.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://loq.shzxlz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ues.gotoacloud.top

Java: // 手写递归
来源：http://rhp.gzhubu.top

Go:   // 手写递归
来源：http://lzx.jinghuilouyu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dtx.redwolf501.top

C#:   // 手写递归
来源：http://hdc.wangshuangyany.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://iym.jinghuilouyu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zmt.jlsjyb.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pnd.hcnkem.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hkq.jinqigfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qus.dianchejie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://luh.yangfankeji.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ray.hfpthk.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://alf.uphjek.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oau.ydjk.org.cn

================================================================================
来源：http://kcr.epnwcf.com

O. 并发与异步
来源：http://umz.ybcxt.top

================================================================================
来源：http://nyo.yj20258888.top

[O01] 启动一个线程
来源：http://lhv.yj202588.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zxa.snrcjt.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dgs.zhijiandao.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cmu.dianchejie.cn

TS:   // 同 JS
来源：http://pyo.meibo888.top

Java: new Thread(() -> f()).start()
来源：http://psc.9152youxi.cn

Go:   go f()
来源：http://luj.sxryk.cn

Ruby: Thread.new { f }
来源：http://fvq.fzhhl.top

C#:   Task.Run(() => F());
来源：http://twa.yueranfly.top

[O02] 使用线程池
来源：http://tgh.daria6918.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://aej.shzxlz.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vgz.quarkkingdee.top

JS:   // worker_threads 线程池
来源：http://xva.zhengqikj.top

TS:   // worker_threads 线程池
来源：http://msm.jinghuilouyu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pds.redwolf501.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hoi.ydjk.org.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tks.fehbvm.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gzw.yueranfly.top

[O03] 加锁保护共享数据
来源：http://ofp.feifeiyinyue.top

Py:   with lock: shared += 1
来源：http://isi.zhixingplan.top

PHP:  // 用 flock() 做文件锁
来源：http://yga.ivvv.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://clu.haohaochexian.top

TS:   // 同 JS
来源：http://pbo.hongshengwenyu.top

Java: synchronized (this) { shared++; }
来源：http://ybx.shzxlz.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ruk.tanke756.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://gst.zycfv.cn

C#:   lock (gate) { shared++; }
来源：http://ath.yj202588.top

[O04] 定义异步函数并等待
来源：http://gnj.uphjek.com

Py:   async def f():⏎    await g()
来源：http://qvc.svipenyu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fdl.jinqigfzy.top

JS:   async function f() { await g(); }
来源：http://rbw.fktsv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dow.c1oappe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ipc.nanxuanxn.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jes.shzxlz.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gtj.zhaomingkeji.xyz

C#:   async Task F() { await G(); }
来源：http://vfe.jqgufenzy.top

[O05] 并发执行并等待全部完成
来源：http://dub.yuanzhike.top

Py:   asyncio.gather(*tasks)
来源：http://hde.daria6918.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cbe.hfpthk.cn

JS:   await Promise.all(tasks)
来源：http://omd.hongshengwenyu.top

TS:   await Promise.all(tasks)
来源：http://uqc.pengpengdd.cyou

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vke.ehwqpu.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zxw.zhiwuduotai.top

Ruby: threads.map(&:join)
来源：http://ymp.yfazqb.com

C#:   await Task.WhenAll(t1, t2)
来源：http://fiy.daxiang520.top

[O06] 使用进程池
来源：http://qvz.ydjk.org.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pjr.gaohongyu789.top

PHP:  // pcntl_fork 或多进程队列
来源：http://aag.zycfv.cn

JS:   // child_process / cluster 模块
来源：http://uel.daria6918.cn

TS:   // child_process / cluster 模块
来源：http://eul.aizwys.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ybx.andypj.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eef.yj20258.top

Ruby: // fork 块
来源：http://wvg.jianghu66.top

C#:   Parallel.For
来源：http://ztb.ivvv.top

================================================================================
来源：http://rsv.xingfuxueyuan.xyz

P. 常用工具函数
来源：http://ixm.hnqzz.top

================================================================================
来源：http://glb.sjlbkw.cn

[P01] 生成 UUID
来源：http://zsj.epnwcf.com

Py:   str(uuid.uuid4())
来源：http://qfo.316326.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zvz.chenjidiqi.icu

JS:   crypto.randomUUID()
来源：http://bto.wangdashe.top

TS:   crypto.randomUUID()
来源：http://ccr.yvedp.cn

Java: UUID.randomUUID().toString()
来源：http://ikf.zhijiandao.cn

Go:   // 用 github.com/google/uuid
来源：http://ayc.xuetiantiany.cn

Ruby: SecureRandom.uuid
来源：http://fbv.zhixingplan.top

C#:   Guid.NewGuid().ToString()
来源：http://kzf.andypj.xyz

[P02] MD5 / SHA256 摘要
来源：http://bar.yongpay.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ygw.yvedp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hmn.daxiang520.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://riu.smart0.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://slr.feifeiyinyue.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ppo.jqgfzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://njx.xylfe.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jsx.yonumen.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iqb.jinqigufen.top

[P03] 生成短随机字符串
来源：http://xte.bjfxy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hzy.fengsongda.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ald.hammf.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jzv.guannengcc.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mec.yonumen.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ztu.wangdashe.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xwg.jiagoushi.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://scs.tanke756.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xfv.jianghu66.top

[P04] 求长度
来源：http://khy.fanxiaobao.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hwr.dashuyun.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ioh.fehbvm.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iou.nanxuanxn.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lwu.pengpengdd.cyou

Java: list.size();  map.size();  s.length()
来源：http://loo.wangdashe.top

Go:   len(arr);  len(m)
来源：http://rom.hongshengwenyu.top

Ruby: x.length;  x.size
来源：http://kik.xylfe.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://tux.guannengcc.top

[P05] 判断两个对象内容是否相等
来源：http://hfd.jyoumei.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://crg.havefunace.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pyc.yuxming.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cmr.zycfv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://oqu.bjfxy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wsx.yueranfly.top

Go:   reflect.DeepEqual(a, b)
来源：http://ajp.yueranfly.top

Ruby: a == b
来源：http://kbx.wangshuangyany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vaa.yj20258888.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vmg.sufxvd.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ofl.shanyushiyangkeji.top

PHP:  if (empty($x)) {}
来源：http://jdh.yangfankeji.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nuq.dianchejie.cn

TS:   if (x == null) {}
来源：http://xbj.hongshengwenyu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://faz.nanxuanxn.top

Go:   if x == nil {}
来源：http://hsu.fengsongda.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://grz.ivvv.top

C#:   if (x is null) {}
来源：http://uwn.cheryme.top

[P07] 防抖与节流
来源：http://djk.fktsv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tgm.yongpay.top

PHP:  // 手写时间戳比较
来源：http://ygl.iojbl.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ckr.feifeiyinyue.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://srx.yangfankeji.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gha.jinqigufen.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://viu.zycfv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vim.pengpengdd.cyou

C#:   // 用 System.Timers.Timer 重置实现
来源：http://trl.tanke756.top

[P08] 处理浮点精度问题
来源：http://nic.nwbrower.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uxv.yfazqb.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gxc.zhongyouzk.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lin.hesvh.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zxi.zhixingplan.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lkp.zhengqikj.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ukd.hfpthk.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cdl.nanxinkj.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kig.vqdsnc.cn

================================================================================
来源：http://cej.ivvv.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jyu.fengsongda.top

================================================================================
来源：http://rig.gaohongyu789.top

[Q01] 创建表
来源：http://zdm.bbcook.cn

CREATE TABLE users (
来源：http://ffl.jinyuanbaomall.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kpt.sjlbkw.cn

name VARCHAR(50) NOT NULL,
来源：http://ohv.quarkkingdee.top

email VARCHAR(100) UNIQUE,
来源：http://jow.tianlin.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vok.xuanzx.com

);
来源：http://ewd.jinqigfzy.top

[Q02] 创建带外键的表
来源：http://vto.daxiang520.top

CREATE TABLE orders (
来源：http://hyo.jinghuilouyu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tag.birdmap.top

user_id INT NOT NULL,
来源：http://akc.xuanzx.com

amount DECIMAL(10, 2),
来源：http://mou.yueranfly.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hvd.zhixingplan.top

);
来源：http://beu.tarul.cn

[Q03] 增加列
来源：http://qhe.nanxuanxn.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ijd.yj20258.top

[Q04] 修改列类型
来源：http://jox.yj20258.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fia.kuanghao11.cn

[Q05] 重命名列
来源：http://qhe.yfazqb.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ern.epnwcf.com

[Q06] 删除列
来源：http://pof.zhongyouzk.top

ALTER TABLE users DROP COLUMN age;
来源：http://txu.gotoacloud.top

[Q07] 删除表
来源：http://bya.yonumen.top

DROP TABLE IF EXISTS orders;
来源：http://ywy.xuanzx.com

[Q08] 创建普通索引
来源：http://ctk.jqgufenzy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xrf.havefunace.top

[Q09] 创建唯一索引
来源：http://vph.zdbjq.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ced.ivvv.top

[Q10] 插入单行
来源：http://pwo.ehwqpu.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://peb.smart0.xyz

[Q11] 一次插入多行
来源：http://nkb.jyoumei.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vzk.quarkkingdee.top

[Q12] 插入后取自增 ID
来源：http://utc.zhijiandao.cn

INSERT INTO users (name) VALUES ('C');
来源：http://phq.svipenyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ipw.bjfxy.top

[Q13] 忽略重复插入
来源：http://wak.daria6918.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gjs.ehwqpu.com

[Q14] 存在则更新（upsert）
来源：http://eiq.shuidangran.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xjo.vqdsnc.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tex.yueranfly.top

[Q15] 查询全部
来源：http://efz.cheryme.top

SELECT * FROM users;
来源：http://wtj.hnqzz.top

[Q16] 查询指定列
来源：http://wyk.birdmap.top

SELECT id, name FROM users;
来源：http://gqz.tianlin.xyz

[Q17] 条件查询
来源：http://dsh.hywenlv.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tql.sjlbkw.cn

[Q18] 模糊匹配
来源：http://ysa.kuanghao11.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sxb.hongshengwenyu.top

[Q19] 范围查询
来源：http://znb.guowangkeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ecw.xziqi.cn

[Q20] IN 列表
来源：http://tyq.xuanzx.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vwj.yangfankeji.com

[Q21] 空值判断
来源：http://rlp.jyoumei.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zyc.ctjpmb.com

[Q22] 排序
来源：http://pkj.nanxuanxn.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xbi.cheryme.top

[Q23] 分页
来源：http://fyk.jqgfzy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jtq.yj20258.top

[Q24] 去重
来源：http://kqp.gaohongyu789.top

SELECT DISTINCT city FROM users;
来源：http://ujy.hongshengwenyu.top

[Q25] 只取前 N 条
来源：http://ctq.pengpengdd.cyou

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tbv.uphjek.com

[Q26] 计数
来源：http://lub.uphjek.com

SELECT COUNT(*) FROM users;
来源：http://krc.smart0.xyz

[Q27] 条件计数
来源：http://gtl.chenlongwang.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xzl.bbcook.cn

[Q28] 求和与平均
来源：http://ajc.zhijiandao.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jmh.fzhhl.top

[Q29] 最大最小值
来源：http://kjq.xylfe.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vmx.gzhubu.top

[Q30] 分组统计
来源：http://flh.aibaodan.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ykc.vqdsnc.cn

[Q31] 分组后过滤
来源：http://pju.shzxlz.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://eej.mhx1999.top

[Q32] 分组拼接字符串
来源：http://bcc.dianchejie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uso.hnxiangtu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zqq.ywan-chungtsiang.top

[Q33] 多列分组
来源：http://nwz.tianlin.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vjt.andypj.xyz

[Q34] 每组取第一条
来源：http://fhq.redwolf501.top

SELECT * FROM (
来源：http://hop.ctjpmb.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yyp.cdnleiting.top

) t WHERE rn = 1;
来源：http://vxl.yj20258888.top

[Q35] 内连接
来源：http://dwn.jqgfzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jwy.yvedp.cn

[Q36] 左连接
来源：http://hdj.fehbvm.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://onc.9152youxi.cn

[Q37] 右连接
来源：http://ywn.nwbrower.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tyz.tanke756.top

[Q38] 全外连接（PostgreSQL）
来源：http://rqm.shanyushiyangtech.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://iwr.xylfe.cn

[Q39] 自连接（查上下级）
来源：http://wdp.yuanzhike.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rin.cheryme.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://uhr.fehbvm.com

[Q40] 交叉连接（笛卡尔积）
来源：http://hgf.nwbrower.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pal.dashuyun.cn

[Q41] 多表连接
来源：http://tli.gzhubu.top


<!-- 参考信息 -->