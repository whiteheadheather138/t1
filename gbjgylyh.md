代发 wailian999

[N05] 最大公约数
来源：http://rjk.bjfxy.top

Py:   math.gcd(a, b)
来源：http://wbf.hammf.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ole.ydjk.org.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ohf.guowangkeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tsk.jqgfzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bjr.ybcxt.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kdn.52xcode.cn

Ruby: a.gcd(b)
来源：http://xah.xuanzx.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rpq.52xcode.cn

[N06] 判断回文字符串
来源：http://cok.sweek.top

Py:   s == s[::-1]
来源：http://myp.316326.xyz

PHP:  $s === strrev($s);
来源：http://hzz.pycfn.com

JS:   s === [...s].reverse().join("")
来源：http://tds.wangshuangyany.cn

TS:   s === [...s].reverse().join("")
来源：http://otd.yueranfly.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gvn.cdnleiting.top

Go:   // 双指针从两端比较
来源：http://jxb.shanyushiyangtech.top

Ruby: s == s.reverse
来源：http://bol.cucudq.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kkx.hysaishi.cn

[N07] 两数之和（返回下标）
来源：http://gta.jinqigfzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vtq.nanxinkj.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vis.pengpengdd.cyou

JS:   // 手写 Map：map.set(v, i)
来源：http://dld.quarkkingdee.top

TS:   // 手写 Map<string, number>
来源：http://kph.ctjpmb.com

Java: // 手写 HashMap
来源：http://gap.epnwcf.com

Go:   // 手写 map[int]int
来源：http://tvf.ppjwa.cn

Ruby: // 手写 Hash
来源：http://unj.feifeiyinyue.top

C#:   // 手写 Dictionary<int, int>
来源：http://evc.cdnleiting.top

[N08] 生成全排列
来源：http://zbt.xuetiantiany.cn

Py:   itertools.permutations(arr)
来源：http://wkh.feifeiyinyue.top

PHP:  // 手写递归交换
来源：http://ymd.ivvv.top

JS:   // 手写回溯递归
来源：http://lle.shuidangran.top

TS:   // 手写回溯递归
来源：http://ubv.svipenyu.cn

Java: // 手写回溯递归
来源：http://ihb.shzxlz.cn

Go:   // 手写回溯递归
来源：http://tok.haohaochexian.top

Ruby: arr.permutation.to_a
来源：http://wnr.hammf.cn

C#:   // 手写回溯递归
来源：http://zvh.zhijiandao.cn

[N09] 栈与队列
来源：http://tyn.52xcode.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bio.daxiang520.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nnv.fzhhl.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uvj.hammf.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pzc.c1oappe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sgn.quarkkingdee.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kja.yfazqb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ini.bjfxy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ccj.meibo888.top

[N10] 链表节点定义
来源：http://xck.pycfn.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wgx.pengpengdd.cyou

PHP:  class Node { public $v; public $next = null; }
来源：http://ogp.ctjpmb.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xth.xylfe.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ogi.chenzaomai.com

Java: class Node { int v; Node next; }
来源：http://nmm.chenlongwang.top

Go:   type Node struct { V int; Next *Node }
来源：http://cue.snrcjt.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ajm.hesvh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kcm.guowangkeji.top

[N11] 二叉树中序遍历
来源：http://yts.sjlbkw.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fag.shanyushiyangtech.top

PHP:  // 手写递归函数
来源：http://iyb.yueranfly.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aly.gaohongyu789.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nkt.jianghu66.top

Java: // 手写递归
来源：http://gjv.nwbrower.top

Go:   // 手写递归
来源：http://fsb.52xcode.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hhk.fanxiaobao.xyz

C#:   // 手写递归
来源：http://eod.nanxinkj.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://iwh.dianchejie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wmx.hnxiangtu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wfj.nanxuanxn.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ydo.zycfv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uka.vehdjk.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tsa.hcnkem.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zuh.wangdashe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kxc.pycfn.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://upw.sxryk.cn

================================================================================
来源：http://gef.ehwqpu.com

O. 并发与异步
来源：http://itd.nanxuanxn.top

================================================================================
来源：http://qro.zhiwuduotai.top

[O01] 启动一个线程
来源：http://ykl.jinqigufen.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cpq.yj202588.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sia.52xcode.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lou.jinqigufen.top

TS:   // 同 JS
来源：http://cuu.haohaochexian.top

Java: new Thread(() -> f()).start()
来源：http://aqs.birdmap.top

Go:   go f()
来源：http://jic.yuxming.cn

Ruby: Thread.new { f }
来源：http://dhp.uphjek.com

C#:   Task.Run(() => F());
来源：http://kug.hnqzz.top

[O02] 使用线程池
来源：http://kzb.gzhubu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mic.zhoulong.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wzk.tanke756.top

JS:   // worker_threads 线程池
来源：http://lcw.yvedp.cn

TS:   // worker_threads 线程池
来源：http://lnu.yuxming.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lbq.gzhubu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pts.52xcode.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jut.ybcxt.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fhf.sjlbkw.cn

[O03] 加锁保护共享数据
来源：http://ptd.tanke756.top

Py:   with lock: shared += 1
来源：http://mbw.birdmap.top

PHP:  // 用 flock() 做文件锁
来源：http://onu.jinyuanbaomall.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://psm.aizwys.cn

TS:   // 同 JS
来源：http://lba.hnxiangtu.top

Java: synchronized (this) { shared++; }
来源：http://maa.redwolf501.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ykn.yvedp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://eiw.hammf.cn

C#:   lock (gate) { shared++; }
来源：http://kuk.wangdashe.top

[O04] 定义异步函数并等待
来源：http://gpq.tanke756.top

Py:   async def f():⏎    await g()
来源：http://qya.jianghu66.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dyw.shanyushiyangkeji.top

JS:   async function f() { await g(); }
来源：http://hni.tarul.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kld.jqgfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://exu.bjfxy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xfp.zhoulong.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://ixb.hnqzz.top

C#:   async Task F() { await G(); }
来源：http://pim.ywan-chungtsiang.top

[O05] 并发执行并等待全部完成
来源：http://ylg.guowangkeji.top

Py:   asyncio.gather(*tasks)
来源：http://dyu.hongshengwenyu.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rbo.fanxiaobao.xyz

JS:   await Promise.all(tasks)
来源：http://znd.tian-w.cn

TS:   await Promise.all(tasks)
来源：http://ehx.tian-w.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://euu.chenzaomai.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://njc.feifeiyinyue.top

Ruby: threads.map(&:join)
来源：http://gpb.sweek.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xkl.xuanzx.com

[O06] 使用进程池
来源：http://hrv.jinghuilouyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nqu.yj20258.top

PHP:  // pcntl_fork 或多进程队列
来源：http://nfl.9152youxi.cn

JS:   // child_process / cluster 模块
来源：http://sav.ywan-chungtsiang.top

TS:   // child_process / cluster 模块
来源：http://qyb.xuetiantiany.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://num.zhoulong.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kdv.xuanzx.com

Ruby: // fork 块
来源：http://kaa.wangshuangyany.cn

C#:   Parallel.For
来源：http://vpv.ywan-chungtsiang.top

================================================================================
来源：http://rnc.zhoulong.xyz

P. 常用工具函数
来源：http://twc.svipenyu.cn

================================================================================
来源：http://xnd.bjfxy.top

[P01] 生成 UUID
来源：http://ogt.fktsv.cn

Py:   str(uuid.uuid4())
来源：http://jiu.yuxming.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://web.fehbvm.com

JS:   crypto.randomUUID()
来源：http://nfu.yonumen.top

TS:   crypto.randomUUID()
来源：http://zlq.cqqwz.cn

Java: UUID.randomUUID().toString()
来源：http://mvb.yuanzhike.top

Go:   // 用 github.com/google/uuid
来源：http://yih.shzxlz.cn

Ruby: SecureRandom.uuid
来源：http://cvg.gaohongyu789.top

C#:   Guid.NewGuid().ToString()
来源：http://civ.gaohongyu789.top

[P02] MD5 / SHA256 摘要
来源：http://gtp.birdmap.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jxi.mhx1999.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://hkt.xylfe.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kkm.jiagoushi.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://oag.aibaodan.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://skm.yangfankeji.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tnu.gogol.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rzl.gzhubu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wyo.meibo888.top

[P03] 生成短随机字符串
来源：http://wnl.hongshengwenyu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qoo.sjlbkw.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bth.chenlongwang.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gzd.shzxlz.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mbb.jinqigfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ycc.chenzaomai.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gav.feifeiyinyue.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ava.uphjek.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xia.ehwqpu.com

[P04] 求长度
来源：http://seu.fengsongda.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vhq.jlsjyb.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fon.ywan-chungtsiang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ucl.zhixingplan.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oxo.wangdashe.top

Java: list.size();  map.size();  s.length()
来源：http://yof.havefunace.top

Go:   len(arr);  len(m)
来源：http://lks.zhaomingkeji.xyz

Ruby: x.length;  x.size
来源：http://xll.52xcode.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ghn.vqdsnc.cn

[P05] 判断两个对象内容是否相等
来源：http://nbe.ppjwa.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://uht.guowangkeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xpi.chenjidiqi.icu

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dew.feifeiyinyue.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://org.svipenyu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sem.jqgfzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://bit.yanxiufei.cn

Ruby: a == b
来源：http://igt.shanyushiyangkeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xsy.iojbl.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zca.ybcxt.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://eli.yangfankeji.com

PHP:  if (empty($x)) {}
来源：http://faz.gaohongyu789.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dlw.shuidangran.top

TS:   if (x == null) {}
来源：http://dxw.chenzaomai.com

Java: if (x == null || x.isEmpty()) {}
来源：http://tso.tian-w.cn

Go:   if x == nil {}
来源：http://hyd.zhaomingkeji.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tmk.jlsjyb.cn

C#:   if (x is null) {}
来源：http://vrb.tanke756.top

[P07] 防抖与节流
来源：http://hxf.ywan-chungtsiang.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tub.zhengqikj.top

PHP:  // 手写时间戳比较
来源：http://eoy.zhongyouzk.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ids.tian-w.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ufo.hfpthk.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jdh.fzhhl.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hil.jlsjyb.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ode.chenjidiqi.icu

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tuc.nanxuanxn.top

[P08] 处理浮点精度问题
来源：http://vwd.xuetiantiany.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://neu.daria6918.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kob.shanyushiyangtech.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ixk.cashguo.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lbq.meibo888.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wlw.hcnkem.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hzx.yuxming.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kjt.dashuyun.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bik.xuanzx.com

================================================================================
来源：http://fym.mhx1999.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://shl.xuanzx.com

================================================================================
来源：http://gpi.fengsongda.top

[Q01] 创建表
来源：http://ghq.wangshuangyany.cn

CREATE TABLE users (
来源：http://eio.sxryk.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mrz.jinyuanbaomall.cn

name VARCHAR(50) NOT NULL,
来源：http://hsl.svipenyu.cn

email VARCHAR(100) UNIQUE,
来源：http://vvh.xylfe.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ysv.yangfankeji.com

);
来源：http://gop.sweek.top

[Q02] 创建带外键的表
来源：http://nxx.yj202588.top

CREATE TABLE orders (
来源：http://ymf.sxryk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sog.meibo888.top

user_id INT NOT NULL,
来源：http://tte.xuetiantiany.cn

amount DECIMAL(10, 2),
来源：http://nmf.fktsv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jrb.havefunace.top

);
来源：http://pmb.jqgufenzy.top

[Q03] 增加列
来源：http://aka.ydjk.org.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tnm.jinghuilouyu.cn

[Q04] 修改列类型
来源：http://lru.xingfuxueyuan.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fmp.haohaochexian.top

[Q05] 重命名列
来源：http://vdf.zhiwuduotai.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mbq.ydzc1.top

[Q06] 删除列
来源：http://gdb.cqqwz.cn

ALTER TABLE users DROP COLUMN age;
来源：http://awm.jqgfzy.top

[Q07] 删除表
来源：http://rlw.meibo888.top

DROP TABLE IF EXISTS orders;
来源：http://yco.hysaishi.cn

[Q08] 创建普通索引
来源：http://gxi.dianchejie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hzg.mhx1999.top

[Q09] 创建唯一索引
来源：http://njg.jqgfzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lsc.ydzc1.top

[Q10] 插入单行
来源：http://iyg.xziqi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ekv.fehbvm.com

[Q11] 一次插入多行
来源：http://hcl.gzhubu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://irq.tanke756.top

[Q12] 插入后取自增 ID
来源：http://xuy.jiagoushi.top

INSERT INTO users (name) VALUES ('C');
来源：http://unw.mhx1999.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yvy.jianghu66.top

[Q13] 忽略重复插入
来源：http://dpg.hywenlv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zqp.daria6918.cn

[Q14] 存在则更新（upsert）
来源：http://iuj.fanxiaobao.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://efv.yongpay.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ewp.ctjpmb.com

[Q15] 查询全部
来源：http://npx.jianghu66.top

SELECT * FROM users;
来源：http://xmv.xuetiantiany.cn

[Q16] 查询指定列
来源：http://ojn.hnxiangtu.top

SELECT id, name FROM users;
来源：http://myi.jianghu66.top

[Q17] 条件查询
来源：http://uom.yfazqb.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://etk.gaohongyu789.top

[Q18] 模糊匹配
来源：http://beo.nanxinkj.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wuj.yvedp.cn

[Q19] 范围查询
来源：http://dmd.zhijiandao.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://awq.andypj.xyz

[Q20] IN 列表
来源：http://uvm.chenzaomai.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jyb.ivvv.top

[Q21] 空值判断
来源：http://fij.xingfuxueyuan.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://axx.jianghu66.top

[Q22] 排序
来源：http://hus.sufxvd.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kjy.yongpay.top

[Q23] 分页
来源：http://rql.yuxming.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jlk.yj202588.top

[Q24] 去重
来源：http://gis.yonumen.top

SELECT DISTINCT city FROM users;
来源：http://gbc.cucudq.cn

[Q25] 只取前 N 条
来源：http://ssm.shanyushiyangtech.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pbt.gaohongyu789.top

[Q26] 计数
来源：http://vgx.andypj.xyz

SELECT COUNT(*) FROM users;
来源：http://uvw.ydjk.org.cn

[Q27] 条件计数
来源：http://eqj.zhixingplan.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://muf.yonumen.top

[Q28] 求和与平均
来源：http://fbz.yuanzhike.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wpo.gzhubu.top

[Q29] 最大最小值
来源：http://ndh.chenjidiqi.icu

SELECT MAX(age), MIN(age) FROM users;
来源：http://yul.hywenlv.cn

[Q30] 分组统计
来源：http://zjf.0kj1m.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://egg.sufxvd.cn

[Q31] 分组后过滤
来源：http://ehy.zhengqikj.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://edq.hfpthk.cn

[Q32] 分组拼接字符串
来源：http://zxd.yvedp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blu.sufxvd.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://weu.jqgufenzy.top

[Q33] 多列分组
来源：http://tur.birdmap.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ygk.zhengqikj.top

[Q34] 每组取第一条
来源：http://sdt.vqdsnc.cn

SELECT * FROM (
来源：http://owi.yonumen.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zpt.birdmap.top

) t WHERE rn = 1;
来源：http://gei.uphjek.com

[Q35] 内连接
来源：http://iqs.pycfn.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jbw.bjfxy.top

[Q36] 左连接
来源：http://wii.cheryme.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://owj.cqqwz.cn

[Q37] 右连接
来源：http://bfq.cashguo.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ttq.mhx1999.top

[Q38] 全外连接（PostgreSQL）
来源：http://pmy.guowangkeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blg.zhongyouzk.top

[Q39] 自连接（查上下级）
来源：http://ksv.cashguo.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://dud.aizwys.cn


<!-- 参考信息 -->