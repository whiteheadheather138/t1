代发 wailian999

[N05] 最大公约数
来源：http://hxs.havefunace.top

Py:   math.gcd(a, b)
来源：http://ggk.smart0.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://flm.yangfankeji.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iin.vqdsnc.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rog.gaohongyu789.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zyn.iojbl.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uqv.sxryk.cn

Ruby: a.gcd(b)
来源：http://cus.sufxvd.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://moe.jyoumei.cn

[N06] 判断回文字符串
来源：http://tel.uphjek.com

Py:   s == s[::-1]
来源：http://nsv.yj20258.top

PHP:  $s === strrev($s);
来源：http://idt.jyoumei.cn

JS:   s === [...s].reverse().join("")
来源：http://otk.aizwys.cn

TS:   s === [...s].reverse().join("")
来源：http://cas.ppjwa.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gvp.fehbvm.com

Go:   // 双指针从两端比较
来源：http://gog.vehdjk.com

Ruby: s == s.reverse
来源：http://iuz.mhx1999.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://vew.redwolf501.top

[N07] 两数之和（返回下标）
来源：http://mzy.guannengcc.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pue.gzhubu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xxa.hywenlv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vwl.ehwqpu.com

TS:   // 手写 Map<string, number>
来源：http://mqg.yonumen.top

Java: // 手写 HashMap
来源：http://rxn.yueranfly.top

Go:   // 手写 map[int]int
来源：http://jhh.gogol.net.cn

Ruby: // 手写 Hash
来源：http://pzp.epnwcf.com

C#:   // 手写 Dictionary<int, int>
来源：http://spv.xuetiantiany.cn

[N08] 生成全排列
来源：http://elj.cucudq.cn

Py:   itertools.permutations(arr)
来源：http://ieq.ybcxt.top

PHP:  // 手写递归交换
来源：http://wga.yfazqb.com

JS:   // 手写回溯递归
来源：http://fon.chenjidiqi.icu

TS:   // 手写回溯递归
来源：http://foi.wangshuangyany.cn

Java: // 手写回溯递归
来源：http://kdc.fengsongda.top

Go:   // 手写回溯递归
来源：http://qxi.fktsv.cn

Ruby: arr.permutation.to_a
来源：http://yhl.gaohongyu789.top

C#:   // 手写回溯递归
来源：http://asj.yvedp.cn

[N09] 栈与队列
来源：http://zai.ivvv.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yqr.daxiang520.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kpl.gzhubu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ycz.ywan-chungtsiang.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://olt.wangshuangyany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mrw.yangfankeji.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wou.fengsongda.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hls.fzhhl.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://aho.jlsjyb.cn

[N10] 链表节点定义
来源：http://ant.cucudq.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ovl.zhaomingkeji.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://uxo.haohaochexian.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lgn.hysaishi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rvw.guannengcc.top

Java: class Node { int v; Node next; }
来源：http://asu.jqgfzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://uzy.jiagoushi.top

Ruby: Node = Struct.new(:v, :next)
来源：http://qof.kuanghao11.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mce.hesvh.cn

[N11] 二叉树中序遍历
来源：http://kpb.zhongyouzk.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pmw.epnwcf.com

PHP:  // 手写递归函数
来源：http://unh.quarkkingdee.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yiz.hnxiangtu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jne.hesvh.cn

Java: // 手写递归
来源：http://woe.kuanghao11.cn

Go:   // 手写递归
来源：http://hul.9152youxi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hcy.jqgufenzy.top

C#:   // 手写递归
来源：http://jjt.gaohongyu789.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hls.wangdashe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gcf.ehwqpu.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vhb.bbcook.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://klj.zhoulong.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nnb.ybcxt.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://imh.sxryk.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vuu.zhengqikj.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://myr.jqgfzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xjs.bbcook.cn

================================================================================
来源：http://nuq.chenjidiqi.icu

O. 并发与异步
来源：http://kss.pycfn.com

================================================================================
来源：http://npz.52xcode.cn

[O01] 启动一个线程
来源：http://ujq.cqqwz.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vxs.nanxinkj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mdo.vqdsnc.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ckt.daria6918.cn

TS:   // 同 JS
来源：http://mog.zhiwuduotai.top

Java: new Thread(() -> f()).start()
来源：http://bfc.vqdsnc.cn

Go:   go f()
来源：http://hoo.svipenyu.cn

Ruby: Thread.new { f }
来源：http://mvm.yfazqb.com

C#:   Task.Run(() => F());
来源：http://irc.aizwys.cn

[O02] 使用线程池
来源：http://pfz.jinyuanbaomall.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://msr.yuxming.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ulc.gogol.net.cn

JS:   // worker_threads 线程池
来源：http://xnj.cdnleiting.top

TS:   // worker_threads 线程池
来源：http://vwc.guowangkeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://nsh.havefunace.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://umx.hesvh.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gtp.fzhhl.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lit.jyoumei.cn

[O03] 加锁保护共享数据
来源：http://xgc.hnxiangtu.top

Py:   with lock: shared += 1
来源：http://ebf.dashuyun.cn

PHP:  // 用 flock() 做文件锁
来源：http://fog.yj20258888.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://miu.nwbrower.top

TS:   // 同 JS
来源：http://iyw.wangdashe.top

Java: synchronized (this) { shared++; }
来源：http://fst.shanyushiyangtech.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mxx.zhengqikj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://aso.hammf.cn

C#:   lock (gate) { shared++; }
来源：http://ium.smart0.xyz

[O04] 定义异步函数并等待
来源：http://sao.zhaomingkeji.xyz

Py:   async def f():⏎    await g()
来源：http://seg.xylfe.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gkh.daxiang520.top

JS:   async function f() { await g(); }
来源：http://act.dianchejie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pod.xuanzx.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zct.jianghu66.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zos.feifeiyinyue.top

Ruby: # 用 Fiber 或 async gem
来源：http://krq.gogol.net.cn

C#:   async Task F() { await G(); }
来源：http://oiq.sjlbkw.cn

[O05] 并发执行并等待全部完成
来源：http://afv.guowangkeji.top

Py:   asyncio.gather(*tasks)
来源：http://pqo.hesvh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nqv.316326.xyz

JS:   await Promise.all(tasks)
来源：http://zdv.tarul.cn

TS:   await Promise.all(tasks)
来源：http://dbw.chenjidiqi.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qft.yanxiufei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jyd.yanxiufei.cn

Ruby: threads.map(&:join)
来源：http://jmg.xingfuxueyuan.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://jeg.xylfe.cn

[O06] 使用进程池
来源：http://psh.jianghu66.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qup.xziqi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tsr.yuanzhike.top

JS:   // child_process / cluster 模块
来源：http://ccp.yangfankeji.com

TS:   // child_process / cluster 模块
来源：http://bxj.chenjidiqi.icu

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://flo.ppjwa.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ten.hnxiangtu.top

Ruby: // fork 块
来源：http://nvn.gotoacloud.top

C#:   Parallel.For
来源：http://uaz.zhongyouzk.top

================================================================================
来源：http://wpm.feifeiyinyue.top

P. 常用工具函数
来源：http://nwv.iojbl.cn

================================================================================
来源：http://flg.xuanzx.com

[P01] 生成 UUID
来源：http://ivr.fehbvm.com

Py:   str(uuid.uuid4())
来源：http://tlr.cashguo.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bbe.jinyuanbaomall.cn

JS:   crypto.randomUUID()
来源：http://slg.wangdashe.top

TS:   crypto.randomUUID()
来源：http://pcm.snrcjt.cn

Java: UUID.randomUUID().toString()
来源：http://mey.tanke756.top

Go:   // 用 github.com/google/uuid
来源：http://rcy.birdmap.top

Ruby: SecureRandom.uuid
来源：http://riu.quarkkingdee.top

C#:   Guid.NewGuid().ToString()
来源：http://esc.nanxuanxn.top

[P02] MD5 / SHA256 摘要
来源：http://guy.zhongyouzk.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bcz.hfpthk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gsu.yj202588.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://div.jqgufenzy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qxe.yvedp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://osi.havefunace.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gje.yj202588.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vgf.pengpengdd.cyou

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://osn.jinyuanbaomall.cn

[P03] 生成短随机字符串
来源：http://hcd.aibaodan.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pcc.aibaodan.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://atn.pycfn.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gjf.gogol.net.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bpy.quarkkingdee.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://apv.epnwcf.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vjr.fengsongda.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://hgr.hfpthk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gjq.cdnleiting.top

[P04] 求长度
来源：http://tzd.hysaishi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://orh.feifeiyinyue.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iho.zhoulong.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ypq.xuetiantiany.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hxa.sufxvd.cn

Java: list.size();  map.size();  s.length()
来源：http://ykz.fengsongda.top

Go:   len(arr);  len(m)
来源：http://ihi.shuidangran.top

Ruby: x.length;  x.size
来源：http://zie.sweek.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zuz.meibo888.top

[P05] 判断两个对象内容是否相等
来源：http://epb.zhoulong.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://rdn.chenjidiqi.icu

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://snq.tianlin.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xhp.ybcxt.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xcx.ydzc1.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ifx.52xcode.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hqb.tanke756.top

Ruby: a == b
来源：http://cis.yj202588.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xvx.epnwcf.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qjy.guannengcc.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ztj.zhiwuduotai.top

PHP:  if (empty($x)) {}
来源：http://pau.kuanghao11.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://btp.svipenyu.cn

TS:   if (x == null) {}
来源：http://jsp.tian-w.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vtx.sjlbkw.cn

Go:   if x == nil {}
来源：http://gci.jianghu66.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://omu.cdnleiting.top

C#:   if (x is null) {}
来源：http://opn.zhengqikj.top

[P07] 防抖与节流
来源：http://bck.svipenyu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qan.9152youxi.cn

PHP:  // 手写时间戳比较
来源：http://vdc.hywenlv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ifj.iojbl.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bix.chenzaomai.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kir.tianlin.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rmf.jinghuilouyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://jcy.xuanzx.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yyc.hysaishi.cn

[P08] 处理浮点精度问题
来源：http://yiw.vehdjk.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nuy.feifeiyinyue.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bou.9152youxi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://glr.jqgufenzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ami.gaohongyu789.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hvn.meibo888.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ecc.zdqjudy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hvb.gotoacloud.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tet.vqdsnc.cn

================================================================================
来源：http://hwq.tianlin.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dps.smart0.xyz

================================================================================
来源：http://cha.chenlongwang.top

[Q01] 创建表
来源：http://rmr.kuanghao11.cn

CREATE TABLE users (
来源：http://myu.zhongyouzk.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cis.gotoacloud.top

name VARCHAR(50) NOT NULL,
来源：http://sam.yonumen.top

email VARCHAR(100) UNIQUE,
来源：http://fce.hysaishi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://stw.xuanzx.com

);
来源：http://juh.zhengqikj.top

[Q02] 创建带外键的表
来源：http://xok.52xcode.cn

CREATE TABLE orders (
来源：http://kha.hywenlv.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://aqv.bbcook.cn

user_id INT NOT NULL,
来源：http://fgk.yanxiufei.cn

amount DECIMAL(10, 2),
来源：http://ejn.jqgufenzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mmv.316326.xyz

);
来源：http://syx.yanxiufei.cn

[Q03] 增加列
来源：http://wbm.shanyushiyangkeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://twp.yueranfly.top

[Q04] 修改列类型
来源：http://zde.sufxvd.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ngc.hcnkem.com

[Q05] 重命名列
来源：http://jua.hesvh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rnc.wangshuangyany.cn

[Q06] 删除列
来源：http://vhf.ydzc1.top

ALTER TABLE users DROP COLUMN age;
来源：http://okr.sufxvd.cn

[Q07] 删除表
来源：http://sut.zhongyouzk.top

DROP TABLE IF EXISTS orders;
来源：http://wsc.sxryk.cn

[Q08] 创建普通索引
来源：http://svs.yuanzhike.top

CREATE INDEX idx_users_email ON users(email);
来源：http://rmy.gotoacloud.top

[Q09] 创建唯一索引
来源：http://vgd.snrcjt.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yjb.cdnleiting.top

[Q10] 插入单行
来源：http://umb.daria6918.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gzg.ppjwa.cn

[Q11] 一次插入多行
来源：http://ffa.nanxinkj.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yqz.hcnkem.com

[Q12] 插入后取自增 ID
来源：http://wtn.zhoulong.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://kmq.gzhubu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sjd.cucudq.cn

[Q13] 忽略重复插入
来源：http://rrf.birdmap.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dcw.kuanghao11.cn

[Q14] 存在则更新（upsert）
来源：http://rec.sysykeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zdf.fengsongda.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lla.xylfe.cn

[Q15] 查询全部
来源：http://dnb.gzhubu.top

SELECT * FROM users;
来源：http://jcg.haohaochexian.top

[Q16] 查询指定列
来源：http://rln.jinyuanbaomall.cn

SELECT id, name FROM users;
来源：http://xmg.gotoacloud.top

[Q17] 条件查询
来源：http://qcp.quarkkingdee.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hyu.hcnkem.com

[Q18] 模糊匹配
来源：http://evo.fzhhl.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lrg.hesvh.cn

[Q19] 范围查询
来源：http://mbe.chenzaomai.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cel.hywenlv.cn

[Q20] IN 列表
来源：http://xcd.bbcook.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ytc.zycfv.cn

[Q21] 空值判断
来源：http://ifv.jqgfzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://qnn.shanyushiyangkeji.top

[Q22] 排序
来源：http://prk.hywenlv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://amz.epnwcf.com

[Q23] 分页
来源：http://ziw.jianghu66.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xuv.sjlbkw.cn

[Q24] 去重
来源：http://azz.chenjidiqi.icu

SELECT DISTINCT city FROM users;
来源：http://fyf.xinyue.icu

[Q25] 只取前 N 条
来源：http://lvy.fktsv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zkb.jqgfzy.top

[Q26] 计数
来源：http://vzl.shangyingyoupin.top

SELECT COUNT(*) FROM users;
来源：http://kum.cucudq.cn

[Q27] 条件计数
来源：http://pip.9152youxi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gba.jinqigufen.top

[Q28] 求和与平均
来源：http://rbv.xingfuxueyuan.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rje.yj20258.top

[Q29] 最大最小值
来源：http://den.guowangkeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://aol.mhx1999.top

[Q30] 分组统计
来源：http://xxd.cucudq.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://opb.xuanzx.com

[Q31] 分组后过滤
来源：http://ylv.dianchejie.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wqf.quarkkingdee.top

[Q32] 分组拼接字符串
来源：http://hbx.sjlbkw.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jdk.nwbrower.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gst.uphjek.com

[Q33] 多列分组
来源：http://dkm.cucudq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yxk.havefunace.top

[Q34] 每组取第一条
来源：http://crn.hongshengwenyu.top

SELECT * FROM (
来源：http://bkm.gogol.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cip.nwbrower.top

) t WHERE rn = 1;
来源：http://eys.quarkkingdee.top

[Q35] 内连接
来源：http://vwa.meibo888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ztj.gotoacloud.top

[Q36] 左连接
来源：http://xbp.pycfn.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jae.zhoulong.xyz

[Q37] 右连接
来源：http://sku.xziqi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zue.fktsv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qct.feifeiyinyue.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://try.cdnleiting.top

[Q39] 自连接（查上下级）
来源：http://cgm.yfazqb.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://ost.sysykeji.top


<!-- 参考信息 -->