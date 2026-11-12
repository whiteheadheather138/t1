代发 wailian999

[N05] 最大公约数
来源：http://eyi.shanyushiyangkeji.top

Py:   math.gcd(a, b)
来源：http://lag.zdbjq.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wdg.ppjwa.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fou.cashguo.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yyu.wangdashe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wjs.cdnleiting.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hsl.ivvv.top

Ruby: a.gcd(b)
来源：http://vqm.feifeiyinyue.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xsh.yanxiufei.cn

[N06] 判断回文字符串
来源：http://rgo.bjfxy.top

Py:   s == s[::-1]
来源：http://wkr.ywan-chungtsiang.top

PHP:  $s === strrev($s);
来源：http://wpg.hywenlv.cn

JS:   s === [...s].reverse().join("")
来源：http://isz.andypj.xyz

TS:   s === [...s].reverse().join("")
来源：http://vec.hammf.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://acs.hnxiangtu.top

Go:   // 双指针从两端比较
来源：http://gat.nanxuanxn.top

Ruby: s == s.reverse
来源：http://hvh.dianchejie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qbu.shangyingyoupin.top

[N07] 两数之和（返回下标）
来源：http://rhm.tanke756.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wty.fehbvm.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zxk.52xcode.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lcm.xylfe.cn

TS:   // 手写 Map<string, number>
来源：http://fvg.ywan-chungtsiang.top

Java: // 手写 HashMap
来源：http://fua.snrcjt.cn

Go:   // 手写 map[int]int
来源：http://kgl.jinqigufen.top

Ruby: // 手写 Hash
来源：http://mia.sxryk.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gzx.fanxiaobao.xyz

[N08] 生成全排列
来源：http://ggo.haohaochexian.top

Py:   itertools.permutations(arr)
来源：http://wfd.yj20258888.top

PHP:  // 手写递归交换
来源：http://eru.shanyushiyangtech.top

JS:   // 手写回溯递归
来源：http://iwj.yj202588.top

TS:   // 手写回溯递归
来源：http://twm.fktsv.cn

Java: // 手写回溯递归
来源：http://uaa.0kj1m.cn

Go:   // 手写回溯递归
来源：http://gtp.vqdsnc.cn

Ruby: arr.permutation.to_a
来源：http://dia.dianchejie.cn

C#:   // 手写回溯递归
来源：http://ney.hcnkem.com

[N09] 栈与队列
来源：http://bkk.andypj.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nnk.bjfxy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wgn.zhiwuduotai.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ogy.zhoulong.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://njv.shzxlz.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://las.xuanzx.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://goj.zhijiandao.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mll.nwbrower.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kje.vqdsnc.cn

[N10] 链表节点定义
来源：http://orw.mhx1999.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gpx.bjfxy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://saz.nwbrower.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ryc.yueranfly.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wur.hysaishi.cn

Java: class Node { int v; Node next; }
来源：http://nxi.ybcxt.top

Go:   type Node struct { V int; Next *Node }
来源：http://gpq.sxryk.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fpa.zhixingplan.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ije.yongpay.top

[N11] 二叉树中序遍历
来源：http://iyr.jinghuilouyu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xtu.hcnkem.com

PHP:  // 手写递归函数
来源：http://scq.sjlbkw.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://alc.ctjpmb.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://haz.hywenlv.cn

Java: // 手写递归
来源：http://fbd.aibaodan.cn

Go:   // 手写递归
来源：http://lmt.ppjwa.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rps.hongshengwenyu.top

C#:   // 手写递归
来源：http://pgm.jinghuilouyu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://eay.iojbl.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hsg.fzhhl.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oqn.gaohongyu789.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wiw.xziqi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rsp.xingfuxueyuan.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hey.gogol.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dyv.zhengqikj.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bsh.tianlin.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gxc.zhengqikj.top

================================================================================
来源：http://yoi.nanxinkj.top

O. 并发与异步
来源：http://ezj.shanyushiyangkeji.top

================================================================================
来源：http://gkn.dashuyun.cn

[O01] 启动一个线程
来源：http://des.jinqigufen.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cux.smart0.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mxg.cashguo.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xko.yonumen.top

TS:   // 同 JS
来源：http://uzr.yvedp.cn

Java: new Thread(() -> f()).start()
来源：http://zgf.tian-w.cn

Go:   go f()
来源：http://ikq.tianlin.xyz

Ruby: Thread.new { f }
来源：http://dsj.hnqzz.top

C#:   Task.Run(() => F());
来源：http://hgn.zhixingplan.top

[O02] 使用线程池
来源：http://bbd.chenlongwang.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jad.hywenlv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ehk.dianchejie.cn

JS:   // worker_threads 线程池
来源：http://ozl.kuanghao11.cn

TS:   // worker_threads 线程池
来源：http://duj.wangshuangyany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zfs.xziqi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://czo.jlsjyb.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jug.jinqigufen.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nqt.tarul.cn

[O03] 加锁保护共享数据
来源：http://kux.zhoulong.xyz

Py:   with lock: shared += 1
来源：http://hcx.shangyingyoupin.top

PHP:  // 用 flock() 做文件锁
来源：http://ggx.gzhubu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nky.iojbl.cn

TS:   // 同 JS
来源：http://dyb.yj20258.top

Java: synchronized (this) { shared++; }
来源：http://vzs.9152youxi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yvn.cashguo.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://tmi.chenzaomai.com

C#:   lock (gate) { shared++; }
来源：http://vlg.kuanghao11.cn

[O04] 定义异步函数并等待
来源：http://zeu.bjfxy.top

Py:   async def f():⏎    await g()
来源：http://gym.yangfankeji.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://row.yueranfly.top

JS:   async function f() { await g(); }
来源：http://bgz.fanxiaobao.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://gmn.wangdashe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lfp.jinqigfzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rjs.tanke756.top

Ruby: # 用 Fiber 或 async gem
来源：http://sbv.hnqzz.top

C#:   async Task F() { await G(); }
来源：http://bgg.ehwqpu.com

[O05] 并发执行并等待全部完成
来源：http://gfy.dashuyun.cn

Py:   asyncio.gather(*tasks)
来源：http://ofe.yj202588.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fck.fzhhl.top

JS:   await Promise.all(tasks)
来源：http://edu.yongpay.top

TS:   await Promise.all(tasks)
来源：http://pbn.zhoulong.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jdr.zhijiandao.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://czx.gaohongyu789.top

Ruby: threads.map(&:join)
来源：http://yht.ivvv.top

C#:   await Task.WhenAll(t1, t2)
来源：http://idp.hywenlv.cn

[O06] 使用进程池
来源：http://lro.yuxming.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://duv.yfazqb.com

PHP:  // pcntl_fork 或多进程队列
来源：http://lot.cqqwz.cn

JS:   // child_process / cluster 模块
来源：http://eau.mhx1999.top

TS:   // child_process / cluster 模块
来源：http://piq.yj202588.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://elw.hcnkem.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://luj.gogol.net.cn

Ruby: // fork 块
来源：http://ogt.yj202588.top

C#:   Parallel.For
来源：http://xns.zhoulong.xyz

================================================================================
来源：http://cnh.fanxiaobao.xyz

P. 常用工具函数
来源：http://pbp.xuetiantiany.cn

================================================================================
来源：http://xws.fehbvm.com

[P01] 生成 UUID
来源：http://kmz.andypj.xyz

Py:   str(uuid.uuid4())
来源：http://xgw.ybcxt.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qfy.jiagoushi.top

JS:   crypto.randomUUID()
来源：http://jyt.fengsongda.top

TS:   crypto.randomUUID()
来源：http://sir.shanyushiyangtech.top

Java: UUID.randomUUID().toString()
来源：http://dmm.ehwqpu.com

Go:   // 用 github.com/google/uuid
来源：http://gfn.chenjidiqi.icu

Ruby: SecureRandom.uuid
来源：http://nce.zdqjudy.top

C#:   Guid.NewGuid().ToString()
来源：http://zou.yuxming.cn

[P02] MD5 / SHA256 摘要
来源：http://djz.feifeiyinyue.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nzk.uphjek.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://zoq.hcnkem.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://aup.jyoumei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vuv.ydjk.org.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ljf.ydjk.org.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hzl.cashguo.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xch.tarul.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://phn.guowangkeji.top

[P03] 生成短随机字符串
来源：http://joq.vehdjk.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mbh.gotoacloud.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ncp.yj202588.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cpr.zhiwuduotai.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ovj.nanxuanxn.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zcs.pycfn.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bsu.yuxming.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bjk.fktsv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qlm.yongpay.top

[P04] 求长度
来源：http://orb.fktsv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://stv.vehdjk.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://boi.xziqi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yyy.vqdsnc.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ioi.ppjwa.cn

Java: list.size();  map.size();  s.length()
来源：http://czu.nanxuanxn.top

Go:   len(arr);  len(m)
来源：http://mlu.kuanghao11.cn

Ruby: x.length;  x.size
来源：http://vrn.tian-w.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jjj.vqdsnc.cn

[P05] 判断两个对象内容是否相等
来源：http://yel.yueranfly.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ceu.sweek.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cat.ppjwa.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gfn.316326.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xzj.meibo888.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vgy.birdmap.top

Go:   reflect.DeepEqual(a, b)
来源：http://huf.aibaodan.cn

Ruby: a == b
来源：http://aeb.chenjidiqi.icu

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://laq.yuxming.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ypl.haohaochexian.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://luk.guowangkeji.top

PHP:  if (empty($x)) {}
来源：http://gry.pycfn.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jmc.jianghu66.top

TS:   if (x == null) {}
来源：http://bwp.dianchejie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lcw.aizwys.cn

Go:   if x == nil {}
来源：http://ela.hfpthk.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dro.zhoulong.xyz

C#:   if (x is null) {}
来源：http://jkm.jinqigfzy.top

[P07] 防抖与节流
来源：http://gwy.jianghu66.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yxv.aizwys.cn

PHP:  // 手写时间戳比较
来源：http://uvi.cashguo.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gjq.jinyuanbaomall.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xbr.meibo888.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mll.aibaodan.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dom.xinyue.icu

Ruby: // 手写闭包 + Time.now 判断
来源：http://hfg.nanxinkj.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fiu.jyoumei.cn

[P08] 处理浮点精度问题
来源：http://cqm.gogol.net.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hkc.fanxiaobao.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wvc.hongshengwenyu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nsk.ctjpmb.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hys.epnwcf.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://byl.jinghuilouyu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yyx.bjfxy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qjo.yangfankeji.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ljp.shzxlz.cn

================================================================================
来源：http://ffu.jqgufenzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://eey.shanyushiyangkeji.top

================================================================================
来源：http://lqy.tarul.cn

[Q01] 创建表
来源：http://jws.yj20258.top

CREATE TABLE users (
来源：http://wiv.jinyuanbaomall.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fuv.cashguo.top

name VARCHAR(50) NOT NULL,
来源：http://qvt.jqgufenzy.top

email VARCHAR(100) UNIQUE,
来源：http://aio.fzhhl.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sqy.tian-w.cn

);
来源：http://lfv.kuanghao11.cn

[Q02] 创建带外键的表
来源：http://wap.gzhubu.top

CREATE TABLE orders (
来源：http://rqe.bbcook.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fsn.shanyushiyangtech.top

user_id INT NOT NULL,
来源：http://pko.jiagoushi.top

amount DECIMAL(10, 2),
来源：http://ick.ivvv.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://imo.nanxuanxn.top

);
来源：http://ovr.daxiang520.top

[Q03] 增加列
来源：http://tte.316326.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://afc.jqgufenzy.top

[Q04] 修改列类型
来源：http://eer.yfazqb.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fah.cqqwz.cn

[Q05] 重命名列
来源：http://jrg.jinyuanbaomall.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qhi.ctjpmb.com

[Q06] 删除列
来源：http://ujd.ehwqpu.com

ALTER TABLE users DROP COLUMN age;
来源：http://hty.jiagoushi.top

[Q07] 删除表
来源：http://gfn.0kj1m.cn

DROP TABLE IF EXISTS orders;
来源：http://zdh.zhixingplan.top

[Q08] 创建普通索引
来源：http://kgx.sysykeji.top

CREATE INDEX idx_users_email ON users(email);
来源：http://fmn.jiagoushi.top

[Q09] 创建唯一索引
来源：http://fdi.guowangkeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vgc.yuxming.cn

[Q10] 插入单行
来源：http://imh.dashuyun.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ump.ywan-chungtsiang.top

[Q11] 一次插入多行
来源：http://mqw.ydjk.org.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ajf.zycfv.cn

[Q12] 插入后取自增 ID
来源：http://dcf.cdnleiting.top

INSERT INTO users (name) VALUES ('C');
来源：http://lve.zdqjudy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rbs.zdqjudy.top

[Q13] 忽略重复插入
来源：http://dld.yuxming.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zcq.andypj.xyz

[Q14] 存在则更新（upsert）
来源：http://ybh.fzhhl.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ujo.zhijiandao.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qeh.svipenyu.cn

[Q15] 查询全部
来源：http://xed.aizwys.cn

SELECT * FROM users;
来源：http://umv.gzhubu.top

[Q16] 查询指定列
来源：http://ndd.xuetiantiany.cn

SELECT id, name FROM users;
来源：http://pye.yangfankeji.com

[Q17] 条件查询
来源：http://mfs.pengpengdd.cyou

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://log.zhiwuduotai.top

[Q18] 模糊匹配
来源：http://fax.gogol.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bti.mhx1999.top

[Q19] 范围查询
来源：http://yno.iojbl.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gks.jinqigufen.top

[Q20] IN 列表
来源：http://owz.cqqwz.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mtv.yanxiufei.cn

[Q21] 空值判断
来源：http://dyz.fanxiaobao.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://yjq.yfazqb.com

[Q22] 排序
来源：http://gop.guowangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yrg.zdbjq.cn

[Q23] 分页
来源：http://pxs.hysaishi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://woe.yj20258.top

[Q24] 去重
来源：http://skj.mhx1999.top

SELECT DISTINCT city FROM users;
来源：http://ebc.svipenyu.cn

[Q25] 只取前 N 条
来源：http://igu.andypj.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yfh.guowangkeji.top

[Q26] 计数
来源：http://pop.fengsongda.top

SELECT COUNT(*) FROM users;
来源：http://lva.chenjidiqi.icu

[Q27] 条件计数
来源：http://kns.c1oappe.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ufj.hfpthk.cn

[Q28] 求和与平均
来源：http://bkl.zdqjudy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://leu.shzxlz.cn

[Q29] 最大最小值
来源：http://cki.daria6918.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gci.yuxming.cn

[Q30] 分组统计
来源：http://pzo.havefunace.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mec.ivvv.top

[Q31] 分组后过滤
来源：http://tdx.sjlbkw.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ruo.fzhhl.top

[Q32] 分组拼接字符串
来源：http://lye.kuanghao11.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rac.shzxlz.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lzj.daria6918.cn

[Q33] 多列分组
来源：http://nzz.cqqwz.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sxe.316326.xyz

[Q34] 每组取第一条
来源：http://tkf.shangyingyoupin.top

SELECT * FROM (
来源：http://slf.xuanzx.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dob.fengsongda.top

) t WHERE rn = 1;
来源：http://dyw.jinqigfzy.top

[Q35] 内连接
来源：http://orf.xinyue.icu

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://brc.fengsongda.top

[Q36] 左连接
来源：http://ghw.pengpengdd.cyou

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://veq.redwolf501.top

[Q37] 右连接
来源：http://gvl.hongshengwenyu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tvl.zdqjudy.top

[Q38] 全外连接（PostgreSQL）
来源：http://gyt.0kj1m.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lfk.zhaomingkeji.xyz

[Q39] 自连接（查上下级）
来源：http://eif.cheryme.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://boa.birdmap.top


<!-- 参考信息 -->