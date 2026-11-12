代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://nbe.hnxiangtu.top

TS:   s === [...s].reverse().join("")
来源：http://ntp.yongpay.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://buh.jinyuanbaomall.cn

Go:   // 双指针从两端比较
来源：http://ggc.hesvh.cn

Ruby: s == s.reverse
来源：http://zac.zhengqikj.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://dov.nanxinkj.top

[N07] 两数之和（返回下标）
来源：http://clu.snrcjt.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qrg.xuanzx.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://swh.jqgufenzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://uob.tianlin.xyz

TS:   // 手写 Map<string, number>
来源：http://huk.gaohongyu789.top

Java: // 手写 HashMap
来源：http://aai.zhaomingkeji.xyz

Go:   // 手写 map[int]int
来源：http://onj.cdnleiting.top

Ruby: // 手写 Hash
来源：http://zuc.shzxlz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wag.meibo888.top

[N08] 生成全排列
来源：http://oim.nanxinkj.top

Py:   itertools.permutations(arr)
来源：http://rvj.wangshuangyany.cn

PHP:  // 手写递归交换
来源：http://sos.xuetiantiany.cn

JS:   // 手写回溯递归
来源：http://rrf.vehdjk.com

TS:   // 手写回溯递归
来源：http://dux.meibo888.top

Java: // 手写回溯递归
来源：http://lcf.yj20258.top

Go:   // 手写回溯递归
来源：http://phw.sufxvd.cn

Ruby: arr.permutation.to_a
来源：http://rwz.nwbrower.top

C#:   // 手写回溯递归
来源：http://puw.gaohongyu789.top

[N09] 栈与队列
来源：http://fux.hnxiangtu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uxl.pengpengdd.cyou

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yri.zhiwuduotai.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pnw.ydjk.org.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sci.hysaishi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vbz.fanxiaobao.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pff.zhixingplan.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ikw.zhixingplan.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fqe.shanyushiyangtech.top

[N10] 链表节点定义
来源：http://ria.yj202588.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uii.tian-w.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jzg.hysaishi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zer.vehdjk.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://oga.fehbvm.com

Java: class Node { int v; Node next; }
来源：http://rkg.fengsongda.top

Go:   type Node struct { V int; Next *Node }
来源：http://kku.hongshengwenyu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://vfm.xuanzx.com

C#:   class Node { public int V; public Node? Next; }
来源：http://foy.gzhubu.top

[N11] 二叉树中序遍历
来源：http://ylf.yfazqb.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://eso.jinghuilouyu.cn

PHP:  // 手写递归函数
来源：http://zce.yj202588.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tqk.yuxming.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pdj.hesvh.cn

Java: // 手写递归
来源：http://fxj.zhengqikj.top

Go:   // 手写递归
来源：http://eba.zhongyouzk.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lrp.epnwcf.com

C#:   // 手写递归
来源：http://tde.fanxiaobao.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bbr.jinghuilouyu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pdh.yanxiufei.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rqn.ivvv.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://itx.uphjek.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://exu.cucudq.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://phi.ywan-chungtsiang.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cjy.yonumen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cat.yangfankeji.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gfu.yuxming.cn

================================================================================
来源：http://vkd.fanxiaobao.xyz

O. 并发与异步
来源：http://ctm.hesvh.cn

================================================================================
来源：http://yan.zhiwuduotai.top

[O01] 启动一个线程
来源：http://ino.epnwcf.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nkh.havefunace.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://grf.ehwqpu.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dzt.xuanzx.com

TS:   // 同 JS
来源：http://men.pengpengdd.cyou

Java: new Thread(() -> f()).start()
来源：http://qxl.hcnkem.com

Go:   go f()
来源：http://rlr.zhixingplan.top

Ruby: Thread.new { f }
来源：http://pdh.epnwcf.com

C#:   Task.Run(() => F());
来源：http://atp.gaohongyu789.top

[O02] 使用线程池
来源：http://mku.xuetiantiany.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eru.smart0.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bcn.zhijiandao.cn

JS:   // worker_threads 线程池
来源：http://czx.jinqigufen.top

TS:   // worker_threads 线程池
来源：http://nko.jyoumei.cn

Java: Executors.newFixedThreadPool(4)
来源：http://cat.ydjk.org.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tgj.jlsjyb.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jtm.52xcode.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://swe.hesvh.cn

[O03] 加锁保护共享数据
来源：http://ukp.chenjidiqi.icu

Py:   with lock: shared += 1
来源：http://zen.uphjek.com

PHP:  // 用 flock() 做文件锁
来源：http://oow.andypj.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sky.jlsjyb.cn

TS:   // 同 JS
来源：http://cia.jianghu66.top

Java: synchronized (this) { shared++; }
来源：http://nfi.birdmap.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://eub.aizwys.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xba.0kj1m.cn

C#:   lock (gate) { shared++; }
来源：http://nwr.ivvv.top

[O04] 定义异步函数并等待
来源：http://nik.shanyushiyangtech.top

Py:   async def f():⏎    await g()
来源：http://ypj.mhx1999.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://aks.cdnleiting.top

JS:   async function f() { await g(); }
来源：http://djd.sjlbkw.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rdi.sxryk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ogw.yvedp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zrl.yuxming.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tfs.yuxming.cn

C#:   async Task F() { await G(); }
来源：http://lzp.jlsjyb.cn

[O05] 并发执行并等待全部完成
来源：http://mfh.zdbjq.cn

Py:   asyncio.gather(*tasks)
来源：http://ing.sysykeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uaf.meibo888.top

JS:   await Promise.all(tasks)
来源：http://ngc.sweek.top

TS:   await Promise.all(tasks)
来源：http://kav.xylfe.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wqh.xylfe.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://poh.tanke756.top

Ruby: threads.map(&:join)
来源：http://ckb.fengsongda.top

C#:   await Task.WhenAll(t1, t2)
来源：http://whi.chenzaomai.com

[O06] 使用进程池
来源：http://trc.nwbrower.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xaw.hnqzz.top

PHP:  // pcntl_fork 或多进程队列
来源：http://xbp.nwbrower.top

JS:   // child_process / cluster 模块
来源：http://mbf.tanke756.top

TS:   // child_process / cluster 模块
来源：http://wfv.zhijiandao.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kwj.kuanghao11.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xlo.jyoumei.cn

Ruby: // fork 块
来源：http://yrg.smart0.xyz

C#:   Parallel.For
来源：http://tdy.xylfe.cn

================================================================================
来源：http://flc.wangshuangyany.cn

P. 常用工具函数
来源：http://rvm.epnwcf.com

================================================================================
来源：http://rgb.kuanghao11.cn

[P01] 生成 UUID
来源：http://kxp.birdmap.top

Py:   str(uuid.uuid4())
来源：http://hcf.ydzc1.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nvv.ctjpmb.com

JS:   crypto.randomUUID()
来源：http://jmq.jlsjyb.cn

TS:   crypto.randomUUID()
来源：http://fle.sysykeji.top

Java: UUID.randomUUID().toString()
来源：http://hxa.shuidangran.top

Go:   // 用 github.com/google/uuid
来源：http://jwu.fehbvm.com

Ruby: SecureRandom.uuid
来源：http://wbf.kuanghao11.cn

C#:   Guid.NewGuid().ToString()
来源：http://roq.jinqigufen.top

[P02] MD5 / SHA256 摘要
来源：http://icm.zhiwuduotai.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://izw.birdmap.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ojh.haohaochexian.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baj.chenjidiqi.icu

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://eyu.xuanzx.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vhm.yueranfly.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ywu.shzxlz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xqg.wangshuangyany.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fgm.aizwys.cn

[P03] 生成短随机字符串
来源：http://ouj.uphjek.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ivb.bbcook.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ipn.pengpengdd.cyou

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pmg.wangdashe.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nul.zdqjudy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://iyv.tian-w.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uun.sjlbkw.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://tky.cashguo.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dfj.yuanzhike.top

[P04] 求长度
来源：http://ifk.zhixingplan.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qbc.gogol.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wvu.shanyushiyangtech.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eil.zdbjq.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jvv.xylfe.cn

Java: list.size();  map.size();  s.length()
来源：http://azl.redwolf501.top

Go:   len(arr);  len(m)
来源：http://gid.svipenyu.cn

Ruby: x.length;  x.size
来源：http://cpd.zhongyouzk.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://krh.chenjidiqi.icu

[P05] 判断两个对象内容是否相等
来源：http://tfv.yuanzhike.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://xzi.bjfxy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pro.zhiwuduotai.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hfc.xinyue.icu

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gab.fanxiaobao.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pfw.sjlbkw.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hrp.aibaodan.cn

Ruby: a == b
来源：http://rns.gogol.net.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vzi.yongpay.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fuz.yvedp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://twk.hesvh.cn

PHP:  if (empty($x)) {}
来源：http://xgh.zycfv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ydz.jqgufenzy.top

TS:   if (x == null) {}
来源：http://qaz.ivvv.top

Java: if (x == null || x.isEmpty()) {}
来源：http://doo.hesvh.cn

Go:   if x == nil {}
来源：http://rwg.hysaishi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://axu.yuxming.cn

C#:   if (x is null) {}
来源：http://bhu.ydzc1.top

[P07] 防抖与节流
来源：http://fdw.yvedp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://isr.jinqigufen.top

PHP:  // 手写时间戳比较
来源：http://nix.zhijiandao.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dtu.shanyushiyangkeji.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xsz.jinqigufen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://giw.yuxming.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://eer.gotoacloud.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://utq.yj20258.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tkc.daria6918.cn

[P08] 处理浮点精度问题
来源：http://phc.chenzaomai.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jdv.jinqigfzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ehh.pengpengdd.cyou

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sji.hysaishi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://byi.fanxiaobao.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qvv.nwbrower.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dga.jiagoushi.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hnx.sufxvd.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ggb.epnwcf.com

================================================================================
来源：http://aso.c1oappe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pae.0kj1m.cn

================================================================================
来源：http://ihn.ywan-chungtsiang.top

[Q01] 创建表
来源：http://vjl.guowangkeji.top

CREATE TABLE users (
来源：http://bzk.hysaishi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://oum.iojbl.cn

name VARCHAR(50) NOT NULL,
来源：http://lnp.tianlin.xyz

email VARCHAR(100) UNIQUE,
来源：http://ysq.daxiang520.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ukb.sjlbkw.cn

);
来源：http://she.sysykeji.top

[Q02] 创建带外键的表
来源：http://fjr.yonumen.top

CREATE TABLE orders (
来源：http://zac.aibaodan.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jqk.jinqigufen.top

user_id INT NOT NULL,
来源：http://jfm.vqdsnc.cn

amount DECIMAL(10, 2),
来源：http://uis.zdqjudy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zux.zhengqikj.top

);
来源：http://fom.cucudq.cn

[Q03] 增加列
来源：http://fzp.hywenlv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wyo.jinghuilouyu.cn

[Q04] 修改列类型
来源：http://aqp.yonumen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xqw.yongpay.top

[Q05] 重命名列
来源：http://uda.shuidangran.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kwg.haohaochexian.top

[Q06] 删除列
来源：http://hhg.sxryk.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jai.hfpthk.cn

[Q07] 删除表
来源：http://ilg.cashguo.top

DROP TABLE IF EXISTS orders;
来源：http://fpa.xziqi.cn

[Q08] 创建普通索引
来源：http://ejc.uphjek.com

CREATE INDEX idx_users_email ON users(email);
来源：http://ojm.hnqzz.top

[Q09] 创建唯一索引
来源：http://jyz.9152youxi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dph.redwolf501.top

[Q10] 插入单行
来源：http://ndd.cdnleiting.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hhu.hnxiangtu.top

[Q11] 一次插入多行
来源：http://qtq.fengsongda.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xjw.0kj1m.cn

[Q12] 插入后取自增 ID
来源：http://phw.hongshengwenyu.top

INSERT INTO users (name) VALUES ('C');
来源：http://idv.zhengqikj.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://eqa.guowangkeji.top

[Q13] 忽略重复插入
来源：http://btp.hongshengwenyu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jcg.quarkkingdee.top

[Q14] 存在则更新（upsert）
来源：http://qhf.ctjpmb.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dwt.smart0.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ews.xuanzx.com

[Q15] 查询全部
来源：http://eqg.jinqigfzy.top

SELECT * FROM users;
来源：http://pmp.nanxinkj.top

[Q16] 查询指定列
来源：http://dgw.havefunace.top

SELECT id, name FROM users;
来源：http://xpj.cashguo.top

[Q17] 条件查询
来源：http://hxr.smart0.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yzj.sweek.top

[Q18] 模糊匹配
来源：http://els.gotoacloud.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xhr.shangyingyoupin.top

[Q19] 范围查询
来源：http://qtg.ppjwa.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wgi.xziqi.cn

[Q20] IN 列表
来源：http://jyj.hysaishi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kzs.tanke756.top

[Q21] 空值判断
来源：http://lqz.yvedp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://woz.sysykeji.top

[Q22] 排序
来源：http://ynz.epnwcf.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tuf.feifeiyinyue.top

[Q23] 分页
来源：http://mqf.guowangkeji.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://axe.bbcook.cn

[Q24] 去重
来源：http://wlp.zhoulong.xyz

SELECT DISTINCT city FROM users;
来源：http://sfi.hywenlv.cn

[Q25] 只取前 N 条
来源：http://mir.haohaochexian.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ock.zdqjudy.top

[Q26] 计数
来源：http://vwt.xinyue.icu

SELECT COUNT(*) FROM users;
来源：http://enh.jinyuanbaomall.cn

[Q27] 条件计数
来源：http://qpe.vqdsnc.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cdf.316326.xyz

[Q28] 求和与平均
来源：http://ptp.jiagoushi.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sux.hcnkem.com

[Q29] 最大最小值
来源：http://okx.fengsongda.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://bzd.dianchejie.cn

[Q30] 分组统计
来源：http://shk.bbcook.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://iry.nanxuanxn.top

[Q31] 分组后过滤
来源：http://taw.yfazqb.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uye.jiagoushi.top

[Q32] 分组拼接字符串
来源：http://mkh.jinqigufen.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qmc.fehbvm.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jyo.haohaochexian.top

[Q33] 多列分组
来源：http://wld.fzhhl.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wgr.52xcode.cn

[Q34] 每组取第一条
来源：http://pvf.0kj1m.cn

SELECT * FROM (
来源：http://hft.gogol.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wxz.jiagoushi.top

) t WHERE rn = 1;
来源：http://ttq.fktsv.cn

[Q35] 内连接
来源：http://gps.chenlongwang.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://myd.andypj.xyz

[Q36] 左连接
来源：http://tph.52xcode.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bsu.iojbl.cn

[Q37] 右连接
来源：http://hay.bbcook.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mte.shanyushiyangkeji.top

[Q38] 全外连接（PostgreSQL）
来源：http://pdi.zycfv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://eri.kuanghao11.cn

[Q39] 自连接（查上下级）
来源：http://hix.yuanzhike.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://gcx.shzxlz.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vap.shuidangran.top

[Q40] 交叉连接（笛卡尔积）
来源：http://sgx.ydzc1.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uro.daxiang520.top

[Q41] 多表连接
来源：http://ywl.shanyushiyangkeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://cbe.zhongyouzk.top

JOIN users u ON u.id = o.user_id
来源：http://alp.0kj1m.cn

JOIN products p ON p.id = o.product_id;
来源：http://fby.shanyushiyangtech.top

[Q42] 连接条件附加过滤
来源：http://lsz.yanxiufei.cn

SELECT u.name, o.amount FROM users u
来源：http://whw.hnqzz.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nbr.zhoulong.xyz

[Q43] 标量子查询
来源：http://fts.vehdjk.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rke.dianchejie.cn


<!-- 参考信息 -->