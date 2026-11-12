代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://ort.guannengcc.top

TS:   s === [...s].reverse().join("")
来源：http://htm.316326.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://plx.zhaomingkeji.xyz

Go:   // 双指针从两端比较
来源：http://rxa.fanxiaobao.xyz

Ruby: s == s.reverse
来源：http://gvb.52xcode.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qwi.hywenlv.cn

[N07] 两数之和（返回下标）
来源：http://myq.ydzc1.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wkl.bbcook.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ziq.ivvv.top

JS:   // 手写 Map：map.set(v, i)
来源：http://sag.aibaodan.cn

TS:   // 手写 Map<string, number>
来源：http://upx.c1oappe.top

Java: // 手写 HashMap
来源：http://whw.zhixingplan.top

Go:   // 手写 map[int]int
来源：http://jqp.tianlin.xyz

Ruby: // 手写 Hash
来源：http://kxw.tianlin.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://kcw.jinqigfzy.top

[N08] 生成全排列
来源：http://lyf.xuanzx.com

Py:   itertools.permutations(arr)
来源：http://edc.jinqigfzy.top

PHP:  // 手写递归交换
来源：http://ccd.9152youxi.cn

JS:   // 手写回溯递归
来源：http://ewg.guannengcc.top

TS:   // 手写回溯递归
来源：http://qxz.zdqjudy.top

Java: // 手写回溯递归
来源：http://rib.zhaomingkeji.xyz

Go:   // 手写回溯递归
来源：http://ssx.zdqjudy.top

Ruby: arr.permutation.to_a
来源：http://sqy.meibo888.top

C#:   // 手写回溯递归
来源：http://tmt.yueranfly.top

[N09] 栈与队列
来源：http://pvg.gzhubu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nrc.tian-w.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wjl.snrcjt.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yvz.xuetiantiany.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hcq.xinyue.icu

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rpc.yueranfly.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qvc.c1oappe.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://whr.shzxlz.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dlq.yj20258.top

[N10] 链表节点定义
来源：http://fru.fanxiaobao.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wtk.hysaishi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nkd.vehdjk.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dlk.tian-w.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://djz.jqgfzy.top

Java: class Node { int v; Node next; }
来源：http://dno.hcnkem.com

Go:   type Node struct { V int; Next *Node }
来源：http://lrf.zhijiandao.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gev.52xcode.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rjq.haohaochexian.top

[N11] 二叉树中序遍历
来源：http://eym.jqgufenzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hom.chenlongwang.top

PHP:  // 手写递归函数
来源：http://luy.ctjpmb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lcx.zdbjq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gjh.hfpthk.cn

Java: // 手写递归
来源：http://ryq.tianlin.xyz

Go:   // 手写递归
来源：http://kyg.cheryme.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cbt.yj20258888.top

C#:   // 手写递归
来源：http://sem.cucudq.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zyu.zhixingplan.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://atc.ehwqpu.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gbx.wangshuangyany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uwk.shzxlz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pcu.zhixingplan.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ced.sufxvd.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jel.chenjidiqi.icu

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qna.hcnkem.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mji.c1oappe.top

================================================================================
来源：http://xal.shangyingyoupin.top

O. 并发与异步
来源：http://rsy.dashuyun.cn

================================================================================
来源：http://ifi.sjlbkw.cn

[O01] 启动一个线程
来源：http://uaf.fengsongda.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://veg.nwbrower.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jri.daxiang520.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jip.kuanghao11.cn

TS:   // 同 JS
来源：http://sdo.fanxiaobao.xyz

Java: new Thread(() -> f()).start()
来源：http://jrr.xylfe.cn

Go:   go f()
来源：http://xtv.yuanzhike.top

Ruby: Thread.new { f }
来源：http://cqj.c1oappe.top

C#:   Task.Run(() => F());
来源：http://wsi.316326.xyz

[O02] 使用线程池
来源：http://vuj.jinqigufen.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wza.jqgfzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wxn.feifeiyinyue.top

JS:   // worker_threads 线程池
来源：http://swt.xinyue.icu

TS:   // worker_threads 线程池
来源：http://bfw.zdqjudy.top

Java: Executors.newFixedThreadPool(4)
来源：http://wes.yfazqb.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://uwk.shanyushiyangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xnm.chenjidiqi.icu

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://anw.yvedp.cn

[O03] 加锁保护共享数据
来源：http://niv.yanxiufei.cn

Py:   with lock: shared += 1
来源：http://bgk.yfazqb.com

PHP:  // 用 flock() 做文件锁
来源：http://wth.shanyushiyangkeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vnm.guowangkeji.top

TS:   // 同 JS
来源：http://qbl.jianghu66.top

Java: synchronized (this) { shared++; }
来源：http://msw.jinqigfzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fvf.andypj.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://uwn.hammf.cn

C#:   lock (gate) { shared++; }
来源：http://xpe.9152youxi.cn

[O04] 定义异步函数并等待
来源：http://mzo.vehdjk.com

Py:   async def f():⏎    await g()
来源：http://ywg.jinghuilouyu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kbs.shzxlz.cn

JS:   async function f() { await g(); }
来源：http://edf.ivvv.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://zxg.wangdashe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tnd.ywan-chungtsiang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uhk.yj202588.top

Ruby: # 用 Fiber 或 async gem
来源：http://vcb.yj20258.top

C#:   async Task F() { await G(); }
来源：http://ejd.yfazqb.com

[O05] 并发执行并等待全部完成
来源：http://sjf.andypj.xyz

Py:   asyncio.gather(*tasks)
来源：http://usm.zhengqikj.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nod.nanxuanxn.top

JS:   await Promise.all(tasks)
来源：http://swj.vqdsnc.cn

TS:   await Promise.all(tasks)
来源：http://npx.cheryme.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nlq.ctjpmb.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rmk.cucudq.cn

Ruby: threads.map(&:join)
来源：http://fgk.zdqjudy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://rxj.c1oappe.top

[O06] 使用进程池
来源：http://hzr.jqgufenzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hwi.sxryk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bjj.birdmap.top

JS:   // child_process / cluster 模块
来源：http://mpq.yj20258.top

TS:   // child_process / cluster 模块
来源：http://skg.c1oappe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://eoj.bjfxy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kff.andypj.xyz

Ruby: // fork 块
来源：http://sve.ydjk.org.cn

C#:   Parallel.For
来源：http://mda.yuxming.cn

================================================================================
来源：http://hsv.ybcxt.top

P. 常用工具函数
来源：http://xwq.gogol.net.cn

================================================================================
来源：http://omp.52xcode.cn

[P01] 生成 UUID
来源：http://ogz.tarul.cn

Py:   str(uuid.uuid4())
来源：http://xjr.316326.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://and.yj20258888.top

JS:   crypto.randomUUID()
来源：http://msz.sysykeji.top

TS:   crypto.randomUUID()
来源：http://voh.mhx1999.top

Java: UUID.randomUUID().toString()
来源：http://lkx.bjfxy.top

Go:   // 用 github.com/google/uuid
来源：http://mrm.quarkkingdee.top

Ruby: SecureRandom.uuid
来源：http://wqi.tarul.cn

C#:   Guid.NewGuid().ToString()
来源：http://stu.chenlongwang.top

[P02] MD5 / SHA256 摘要
来源：http://ppe.zycfv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jck.hcnkem.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://pmh.guowangkeji.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ofp.fzhhl.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kvz.shanyushiyangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://eua.c1oappe.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://smt.zhiwuduotai.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zld.chenzaomai.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lyl.ppjwa.cn

[P03] 生成短随机字符串
来源：http://jiz.hnxiangtu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dcq.gzhubu.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hpn.cucudq.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mkw.fanxiaobao.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://amz.sysykeji.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uwl.zhengqikj.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mmn.yonumen.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ksz.cucudq.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pbd.snrcjt.cn

[P04] 求长度
来源：http://ohh.yanxiufei.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qgp.yj20258888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fpy.shanyushiyangtech.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jgs.nanxuanxn.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cue.wangdashe.top

Java: list.size();  map.size();  s.length()
来源：http://qpy.yangfankeji.com

Go:   len(arr);  len(m)
来源：http://dmw.uphjek.com

Ruby: x.length;  x.size
来源：http://rtd.smart0.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://yza.jlsjyb.cn

[P05] 判断两个对象内容是否相等
来源：http://wbk.yfazqb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://iib.yfazqb.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://riy.feifeiyinyue.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://csd.zhongyouzk.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tjw.cheryme.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rvl.cashguo.top

Go:   reflect.DeepEqual(a, b)
来源：http://txv.hnxiangtu.top

Ruby: a == b
来源：http://jxs.sweek.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lsd.jinghuilouyu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bfu.9152youxi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://syl.smart0.xyz

PHP:  if (empty($x)) {}
来源：http://mls.ydzc1.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hwe.fzhhl.top

TS:   if (x == null) {}
来源：http://mjn.iojbl.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://eus.snrcjt.cn

Go:   if x == nil {}
来源：http://uch.ydjk.org.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lbe.0kj1m.cn

C#:   if (x is null) {}
来源：http://ygr.fktsv.cn

[P07] 防抖与节流
来源：http://nhf.bjfxy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mxb.bbcook.cn

PHP:  // 手写时间戳比较
来源：http://gxk.hywenlv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zja.zycfv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://txs.zdbjq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pmq.wangdashe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uad.mhx1999.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://had.fzhhl.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zat.yj202588.top

[P08] 处理浮点精度问题
来源：http://awb.jinqigufen.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://new.guowangkeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mkv.uphjek.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nfn.gotoacloud.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cjw.c1oappe.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://orl.shuidangran.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xhl.fktsv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xoc.feifeiyinyue.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://okw.ydjk.org.cn

================================================================================
来源：http://pmf.zycfv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zrh.zhiwuduotai.top

================================================================================
来源：http://gdp.shangyingyoupin.top

[Q01] 创建表
来源：http://pfr.316326.xyz

CREATE TABLE users (
来源：http://cop.zhoulong.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ugr.52xcode.cn

name VARCHAR(50) NOT NULL,
来源：http://uul.gotoacloud.top

email VARCHAR(100) UNIQUE,
来源：http://bvi.chenzaomai.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lwb.bbcook.cn

);
来源：http://zri.hfpthk.cn

[Q02] 创建带外键的表
来源：http://pnv.cdnleiting.top

CREATE TABLE orders (
来源：http://dzv.wangshuangyany.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zol.yuxming.cn

user_id INT NOT NULL,
来源：http://csf.guowangkeji.top

amount DECIMAL(10, 2),
来源：http://qcd.cqqwz.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wcr.ydjk.org.cn

);
来源：http://rlt.zhixingplan.top

[Q03] 增加列
来源：http://vhv.zdbjq.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lbj.nwbrower.top

[Q04] 修改列类型
来源：http://wdl.gaohongyu789.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qnv.ydjk.org.cn

[Q05] 重命名列
来源：http://ihr.fehbvm.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ysn.zycfv.cn

[Q06] 删除列
来源：http://spf.jinyuanbaomall.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mhe.nanxinkj.top

[Q07] 删除表
来源：http://mbg.ydzc1.top

DROP TABLE IF EXISTS orders;
来源：http://hhr.chenjidiqi.icu

[Q08] 创建普通索引
来源：http://lfx.zhaomingkeji.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://hvh.sufxvd.cn

[Q09] 创建唯一索引
来源：http://tku.feifeiyinyue.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wum.ydjk.org.cn

[Q10] 插入单行
来源：http://tlp.yanxiufei.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ebo.snrcjt.cn

[Q11] 一次插入多行
来源：http://sts.yongpay.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sxe.xylfe.cn

[Q12] 插入后取自增 ID
来源：http://ovc.mhx1999.top

INSERT INTO users (name) VALUES ('C');
来源：http://qwk.hysaishi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ntf.jinqigfzy.top

[Q13] 忽略重复插入
来源：http://ylw.hysaishi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wmo.0kj1m.cn

[Q14] 存在则更新（upsert）
来源：http://jbo.smart0.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://coa.jinqigufen.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kee.aibaodan.cn

[Q15] 查询全部
来源：http://jeo.pycfn.com

SELECT * FROM users;
来源：http://clf.fehbvm.com

[Q16] 查询指定列
来源：http://euw.jqgufenzy.top

SELECT id, name FROM users;
来源：http://jgj.hnxiangtu.top

[Q17] 条件查询
来源：http://zik.havefunace.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fpn.zhiwuduotai.top

[Q18] 模糊匹配
来源：http://ovf.mhx1999.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cgj.redwolf501.top

[Q19] 范围查询
来源：http://fsc.nanxuanxn.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qoh.yangfankeji.com

[Q20] IN 列表
来源：http://hzk.yuxming.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qgp.zdqjudy.top

[Q21] 空值判断
来源：http://hcj.mhx1999.top

SELECT * FROM users WHERE email IS NULL;
来源：http://lle.jqgufenzy.top

[Q22] 排序
来源：http://yaa.gaohongyu789.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gqp.fktsv.cn

[Q23] 分页
来源：http://cpj.xingfuxueyuan.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bbc.yueranfly.top

[Q24] 去重
来源：http://maq.zdqjudy.top

SELECT DISTINCT city FROM users;
来源：http://yjo.yj20258.top

[Q25] 只取前 N 条
来源：http://edb.zhengqikj.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sgz.jiagoushi.top

[Q26] 计数
来源：http://fzw.dashuyun.cn

SELECT COUNT(*) FROM users;
来源：http://mjs.ivvv.top

[Q27] 条件计数
来源：http://nws.bjfxy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ozu.feifeiyinyue.top

[Q28] 求和与平均
来源：http://awk.fzhhl.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ejn.tanke756.top

[Q29] 最大最小值
来源：http://tgu.gogol.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://dba.cucudq.cn

[Q30] 分组统计
来源：http://cix.gogol.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uqe.uphjek.com

[Q31] 分组后过滤
来源：http://fvd.iojbl.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nzn.zhongyouzk.top

[Q32] 分组拼接字符串
来源：http://tzx.shanyushiyangtech.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rgl.bbcook.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://svp.zhoulong.xyz

[Q33] 多列分组
来源：http://zqb.cucudq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xbg.yuxming.cn

[Q34] 每组取第一条
来源：http://bqc.zhixingplan.top

SELECT * FROM (
来源：http://dvf.wangshuangyany.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uib.bbcook.cn

) t WHERE rn = 1;
来源：http://fei.hywenlv.cn

[Q35] 内连接
来源：http://cjc.jqgfzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rvf.cdnleiting.top

[Q36] 左连接
来源：http://uep.zycfv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mpx.shanyushiyangtech.top

[Q37] 右连接
来源：http://rlb.tarul.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uee.52xcode.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lyc.andypj.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fsg.snrcjt.cn

[Q39] 自连接（查上下级）
来源：http://nbd.ctjpmb.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://epn.hesvh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fhw.ywan-chungtsiang.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ogv.hysaishi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ppq.chenlongwang.top

[Q41] 多表连接
来源：http://agj.yuanzhike.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://tzl.0kj1m.cn

JOIN users u ON u.id = o.user_id
来源：http://nmr.havefunace.top

JOIN products p ON p.id = o.product_id;
来源：http://xoy.jqgfzy.top

[Q42] 连接条件附加过滤
来源：http://gyo.jinyuanbaomall.cn

SELECT u.name, o.amount FROM users u
来源：http://eah.jianghu66.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qza.sxryk.cn

[Q43] 标量子查询
来源：http://otb.yanxiufei.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://woa.hesvh.cn


<!-- 参考信息 -->