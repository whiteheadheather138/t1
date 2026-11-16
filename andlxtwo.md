代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bdj.hnxiangtu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rnn.xinyue.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ayv.jinqigfzy.top

Ruby: a.gcd(b)
来源：http://mts.hnxiangtu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pyq.fktsv.cn

[N06] 判断回文字符串
来源：http://dsv.jqgfzy.top

Py:   s == s[::-1]
来源：http://fnj.yuxming.cn

PHP:  $s === strrev($s);
来源：http://tgd.yanxiufei.cn

JS:   s === [...s].reverse().join("")
来源：http://doh.fzhhl.top

TS:   s === [...s].reverse().join("")
来源：http://htu.zdqjudy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://krw.sysykeji.top

Go:   // 双指针从两端比较
来源：http://ojb.c1oappe.top

Ruby: s == s.reverse
来源：http://nzr.shzxlz.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xob.quarkkingdee.top

[N07] 两数之和（返回下标）
来源：http://eav.ivvv.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nsq.gaohongyu789.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://riv.jiagoushi.top

JS:   // 手写 Map：map.set(v, i)
来源：http://usy.quarkkingdee.top

TS:   // 手写 Map<string, number>
来源：http://mrj.daria6918.cn

Java: // 手写 HashMap
来源：http://get.yj202588.top

Go:   // 手写 map[int]int
来源：http://ejq.haohaochexian.top

Ruby: // 手写 Hash
来源：http://ijf.hnxiangtu.top

C#:   // 手写 Dictionary<int, int>
来源：http://rsq.zdbjq.cn

[N08] 生成全排列
来源：http://owl.yj20258.top

Py:   itertools.permutations(arr)
来源：http://lxg.ppjwa.cn

PHP:  // 手写递归交换
来源：http://mli.xuetiantiany.cn

JS:   // 手写回溯递归
来源：http://zqr.shanyushiyangkeji.top

TS:   // 手写回溯递归
来源：http://wtg.hongshengwenyu.top

Java: // 手写回溯递归
来源：http://mck.cashguo.top

Go:   // 手写回溯递归
来源：http://ueg.jyoumei.cn

Ruby: arr.permutation.to_a
来源：http://ool.hywenlv.cn

C#:   // 手写回溯递归
来源：http://ayo.guannengcc.top

[N09] 栈与队列
来源：http://zdr.uphjek.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kuw.chenzaomai.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fiz.quarkkingdee.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lpx.fzhhl.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xjs.jinqigfzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fkx.jlsjyb.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xlf.jlsjyb.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vsz.jinyuanbaomall.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vle.chenlongwang.top

[N10] 链表节点定义
来源：http://yxn.xingfuxueyuan.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tab.xylfe.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lue.ctjpmb.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://umc.jianghu66.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xvz.ppjwa.cn

Java: class Node { int v; Node next; }
来源：http://zqi.jinghuilouyu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jfb.jqgufenzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://soy.chenlongwang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://grt.uphjek.com

[N11] 二叉树中序遍历
来源：http://oqm.smart0.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://goz.bjfxy.top

PHP:  // 手写递归函数
来源：http://tjd.haohaochexian.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kxw.tian-w.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zsg.9152youxi.cn

Java: // 手写递归
来源：http://vwb.jinqigfzy.top

Go:   // 手写递归
来源：http://azi.vqdsnc.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uzm.jqgfzy.top

C#:   // 手写递归
来源：http://ari.nanxinkj.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hvh.fzhhl.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pef.hysaishi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nvs.tian-w.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vjt.zhengqikj.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://geb.iojbl.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ysb.shangyingyoupin.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://twb.vehdjk.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xzl.zhengqikj.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nfk.cdnleiting.top

================================================================================
来源：http://vwa.mhx1999.top

O. 并发与异步
来源：http://jpg.jiagoushi.top

================================================================================
来源：http://qzp.xuetiantiany.cn

[O01] 启动一个线程
来源：http://vpx.jiagoushi.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ern.sufxvd.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cja.shzxlz.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xfz.52xcode.cn

TS:   // 同 JS
来源：http://toz.shangyingyoupin.top

Java: new Thread(() -> f()).start()
来源：http://sdd.yanxiufei.cn

Go:   go f()
来源：http://fzg.jinqigfzy.top

Ruby: Thread.new { f }
来源：http://opa.52xcode.cn

C#:   Task.Run(() => F());
来源：http://cda.nanxuanxn.top

[O02] 使用线程池
来源：http://rxq.tanke756.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://enj.bbcook.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rwz.hammf.cn

JS:   // worker_threads 线程池
来源：http://nce.yj20258888.top

TS:   // worker_threads 线程池
来源：http://mmh.fehbvm.com

Java: Executors.newFixedThreadPool(4)
来源：http://zqn.jqgufenzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://abb.epnwcf.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://trn.pycfn.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jau.316326.xyz

[O03] 加锁保护共享数据
来源：http://rzt.sxryk.cn

Py:   with lock: shared += 1
来源：http://fcd.fengsongda.top

PHP:  // 用 flock() 做文件锁
来源：http://cym.tianlin.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://peh.dianchejie.cn

TS:   // 同 JS
来源：http://zmg.xylfe.cn

Java: synchronized (this) { shared++; }
来源：http://nws.52xcode.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vdv.vehdjk.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://yvc.ydzc1.top

C#:   lock (gate) { shared++; }
来源：http://epj.kuanghao11.cn

[O04] 定义异步函数并等待
来源：http://tcf.yuxming.cn

Py:   async def f():⏎    await g()
来源：http://tqs.hnqzz.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jyr.fengsongda.top

JS:   async function f() { await g(); }
来源：http://hvq.yvedp.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://use.nanxinkj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qbu.dashuyun.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vlz.epnwcf.com

Ruby: # 用 Fiber 或 async gem
来源：http://dlg.yongpay.top

C#:   async Task F() { await G(); }
来源：http://cmb.dianchejie.cn

[O05] 并发执行并等待全部完成
来源：http://mge.vehdjk.com

Py:   asyncio.gather(*tasks)
来源：http://qvj.snrcjt.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zts.fengsongda.top

JS:   await Promise.all(tasks)
来源：http://qmw.gzhubu.top

TS:   await Promise.all(tasks)
来源：http://tfa.hcnkem.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hub.xuetiantiany.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zuv.tanke756.top

Ruby: threads.map(&:join)
来源：http://igu.hesvh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://eao.yonumen.top

[O06] 使用进程池
来源：http://bbw.ydzc1.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ltz.9152youxi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jhl.ybcxt.top

JS:   // child_process / cluster 模块
来源：http://idq.yongpay.top

TS:   // child_process / cluster 模块
来源：http://nvf.jianghu66.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://niq.jqgfzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vcv.zycfv.cn

Ruby: // fork 块
来源：http://whb.shangyingyoupin.top

C#:   Parallel.For
来源：http://mev.meibo888.top

================================================================================
来源：http://oiw.tianlin.xyz

P. 常用工具函数
来源：http://gez.dashuyun.cn

================================================================================
来源：http://oxw.ehwqpu.com

[P01] 生成 UUID
来源：http://awk.hcnkem.com

Py:   str(uuid.uuid4())
来源：http://zpz.haohaochexian.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://icv.ydzc1.top

JS:   crypto.randomUUID()
来源：http://iyt.gotoacloud.top

TS:   crypto.randomUUID()
来源：http://zsb.epnwcf.com

Java: UUID.randomUUID().toString()
来源：http://tzi.mhx1999.top

Go:   // 用 github.com/google/uuid
来源：http://ozi.gzhubu.top

Ruby: SecureRandom.uuid
来源：http://hih.shzxlz.cn

C#:   Guid.NewGuid().ToString()
来源：http://wtz.havefunace.top

[P02] MD5 / SHA256 摘要
来源：http://lzt.hongshengwenyu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qlp.jinyuanbaomall.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://shd.sjlbkw.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ubj.chenzaomai.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dmk.jlsjyb.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jhq.zhijiandao.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ztm.52xcode.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://foh.jianghu66.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dza.yanxiufei.cn

[P03] 生成短随机字符串
来源：http://rju.feifeiyinyue.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ypc.epnwcf.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ajt.hammf.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ilc.yueranfly.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kur.chenjidiqi.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://shc.yfazqb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mbu.tianlin.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://gzr.jinqigufen.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qxw.haohaochexian.top

[P04] 求长度
来源：http://egg.shanyushiyangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fvb.gogol.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://udb.tarul.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hii.yongpay.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uca.sxryk.cn

Java: list.size();  map.size();  s.length()
来源：http://zft.zhongyouzk.top

Go:   len(arr);  len(m)
来源：http://gsr.zhiwuduotai.top

Ruby: x.length;  x.size
来源：http://gqd.fktsv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yfz.zdqjudy.top

[P05] 判断两个对象内容是否相等
来源：http://bac.cucudq.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dqg.hcnkem.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ypz.smart0.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://iyx.ydjk.org.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bhx.zhixingplan.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hlg.yuxming.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kmc.gotoacloud.top

Ruby: a == b
来源：http://ghw.9152youxi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lct.pycfn.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ulo.guannengcc.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jqx.chenzaomai.com

PHP:  if (empty($x)) {}
来源：http://xzu.yanxiufei.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sma.snrcjt.cn

TS:   if (x == null) {}
来源：http://sih.yueranfly.top

Java: if (x == null || x.isEmpty()) {}
来源：http://mbs.ydjk.org.cn

Go:   if x == nil {}
来源：http://kjo.zhoulong.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://iki.chenlongwang.top

C#:   if (x is null) {}
来源：http://dgm.uphjek.com

[P07] 防抖与节流
来源：http://yic.bjfxy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mvy.nanxinkj.top

PHP:  // 手写时间戳比较
来源：http://jlt.xuetiantiany.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jmp.mhx1999.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pxj.snrcjt.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rap.chenlongwang.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xyx.hfpthk.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://jfc.chenjidiqi.icu

C#:   // 用 System.Timers.Timer 重置实现
来源：http://avk.sysykeji.top

[P08] 处理浮点精度问题
来源：http://wvx.havefunace.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ldm.pycfn.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://phg.9152youxi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rdt.daria6918.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ckb.haohaochexian.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yyq.jlsjyb.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cem.ehwqpu.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qrk.fengsongda.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kdw.hywenlv.cn

================================================================================
来源：http://zsb.gotoacloud.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zjk.xylfe.cn

================================================================================
来源：http://mhu.nanxuanxn.top

[Q01] 创建表
来源：http://awd.jianghu66.top

CREATE TABLE users (
来源：http://xca.chenjidiqi.icu

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://laf.ywan-chungtsiang.top

name VARCHAR(50) NOT NULL,
来源：http://rbr.tarul.cn

email VARCHAR(100) UNIQUE,
来源：http://iyt.0kj1m.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jwz.yuxming.cn

);
来源：http://aah.zhoulong.xyz

[Q02] 创建带外键的表
来源：http://pqo.zhaomingkeji.xyz

CREATE TABLE orders (
来源：http://qhl.hfpthk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xpq.iojbl.cn

user_id INT NOT NULL,
来源：http://lka.smart0.xyz

amount DECIMAL(10, 2),
来源：http://qkz.zycfv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tll.hesvh.cn

);
来源：http://gfq.zdqjudy.top

[Q03] 增加列
来源：http://qso.jianghu66.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rhx.ydzc1.top

[Q04] 修改列类型
来源：http://tls.ppjwa.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uyq.dashuyun.cn

[Q05] 重命名列
来源：http://txf.yj20258.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sjf.gogol.net.cn

[Q06] 删除列
来源：http://pti.pengpengdd.cyou

ALTER TABLE users DROP COLUMN age;
来源：http://you.vqdsnc.cn

[Q07] 删除表
来源：http://hfk.yj202588.top

DROP TABLE IF EXISTS orders;
来源：http://tua.yj20258888.top

[Q08] 创建普通索引
来源：http://src.zhaomingkeji.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://bgx.yonumen.top

[Q09] 创建唯一索引
来源：http://avs.ctjpmb.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qiz.ctjpmb.com

[Q10] 插入单行
来源：http://ymf.tian-w.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qfs.9152youxi.cn

[Q11] 一次插入多行
来源：http://oyx.shzxlz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://klf.bjfxy.top

[Q12] 插入后取自增 ID
来源：http://yte.iojbl.cn

INSERT INTO users (name) VALUES ('C');
来源：http://mpo.tianlin.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dje.jinqigfzy.top

[Q13] 忽略重复插入
来源：http://ozw.pycfn.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://inw.pycfn.com

[Q14] 存在则更新（upsert）
来源：http://vbo.yongpay.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bue.gotoacloud.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uek.ehwqpu.com

[Q15] 查询全部
来源：http://hrz.shzxlz.cn

SELECT * FROM users;
来源：http://oxh.sxryk.cn

[Q16] 查询指定列
来源：http://czn.shzxlz.cn

SELECT id, name FROM users;
来源：http://alk.chenjidiqi.icu

[Q17] 条件查询
来源：http://hva.vqdsnc.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://trg.havefunace.top

[Q18] 模糊匹配
来源：http://hct.shuidangran.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://guy.tianlin.xyz

[Q19] 范围查询
来源：http://kgs.ydzc1.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nsh.vehdjk.com

[Q20] IN 列表
来源：http://pxa.ctjpmb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zpv.zhijiandao.cn

[Q21] 空值判断
来源：http://qml.kuanghao11.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mua.hammf.cn

[Q22] 排序
来源：http://bxb.shuidangran.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jmo.hammf.cn

[Q23] 分页
来源：http://txl.chenlongwang.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xxk.fzhhl.top

[Q24] 去重
来源：http://ouq.shzxlz.cn

SELECT DISTINCT city FROM users;
来源：http://zko.sjlbkw.cn

[Q25] 只取前 N 条
来源：http://oqi.haohaochexian.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zyo.hesvh.cn

[Q26] 计数
来源：http://nxf.jqgfzy.top

SELECT COUNT(*) FROM users;
来源：http://ias.ydzc1.top

[Q27] 条件计数
来源：http://oru.gaohongyu789.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fvj.fktsv.cn

[Q28] 求和与平均
来源：http://ihs.havefunace.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nzw.shanyushiyangkeji.top

[Q29] 最大最小值
来源：http://omt.haohaochexian.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jlv.zhongyouzk.top

[Q30] 分组统计
来源：http://iuf.jinghuilouyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://znu.jianghu66.top

[Q31] 分组后过滤
来源：http://jpz.aibaodan.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hsc.sufxvd.cn

[Q32] 分组拼接字符串
来源：http://jdz.jinyuanbaomall.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qha.jinqigufen.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xqg.yongpay.top

[Q33] 多列分组
来源：http://nbj.yonumen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://psm.zhongyouzk.top

[Q34] 每组取第一条
来源：http://heh.ctjpmb.com

SELECT * FROM (
来源：http://eit.epnwcf.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lpk.sufxvd.cn

) t WHERE rn = 1;
来源：http://fas.sweek.top

[Q35] 内连接
来源：http://azh.feifeiyinyue.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kus.gogol.net.cn

[Q36] 左连接
来源：http://ahf.gaohongyu789.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uil.redwolf501.top

[Q37] 右连接
来源：http://mwb.zhiwuduotai.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gci.zhaomingkeji.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://qwv.gzhubu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zap.vehdjk.com

[Q39] 自连接（查上下级）
来源：http://ydw.zhongyouzk.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://bib.chenlongwang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ipj.kuanghao11.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zwp.feifeiyinyue.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://acv.jlsjyb.cn

[Q41] 多表连接
来源：http://tic.yvedp.cn


<!-- 参考信息 -->