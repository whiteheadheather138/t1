代发 wailian999

[N05] 最大公约数
来源：http://may.tanke756.top

Py:   math.gcd(a, b)
来源：http://edg.yj20258888.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gyy.yj20258888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ouw.fengsongda.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sdg.ywan-chungtsiang.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zrd.fzhhl.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tjd.jianghu66.top

Ruby: a.gcd(b)
来源：http://bzg.jianghu66.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://iia.ivvv.top

[N06] 判断回文字符串
来源：http://jto.shanyushiyangtech.top

Py:   s == s[::-1]
来源：http://vec.jianghu66.top

PHP:  $s === strrev($s);
来源：http://ogl.wangdashe.top

JS:   s === [...s].reverse().join("")
来源：http://csl.nanxinkj.top

TS:   s === [...s].reverse().join("")
来源：http://esy.guannengcc.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://swc.fengsongda.top

Go:   // 双指针从两端比较
来源：http://hsb.hysaishi.cn

Ruby: s == s.reverse
来源：http://ajw.aibaodan.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yji.yueranfly.top

[N07] 两数之和（返回下标）
来源：http://lfc.yj20258888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://poz.yvedp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://omc.guannengcc.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gaw.bjfxy.top

TS:   // 手写 Map<string, number>
来源：http://guz.zhengqikj.top

Java: // 手写 HashMap
来源：http://kgs.jinghuilouyu.cn

Go:   // 手写 map[int]int
来源：http://qxp.kuanghao11.cn

Ruby: // 手写 Hash
来源：http://nda.dashuyun.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ohe.xylfe.cn

[N08] 生成全排列
来源：http://pvh.chenjidiqi.icu

Py:   itertools.permutations(arr)
来源：http://vrj.sjlbkw.cn

PHP:  // 手写递归交换
来源：http://lvy.hesvh.cn

JS:   // 手写回溯递归
来源：http://jaq.jqgufenzy.top

TS:   // 手写回溯递归
来源：http://hmf.ybcxt.top

Java: // 手写回溯递归
来源：http://tda.zhongyouzk.top

Go:   // 手写回溯递归
来源：http://jzp.yanxiufei.cn

Ruby: arr.permutation.to_a
来源：http://skd.zdbjq.cn

C#:   // 手写回溯递归
来源：http://leq.sxryk.cn

[N09] 栈与队列
来源：http://esm.zhengqikj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://evd.tarul.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://elg.ydzc1.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tgc.gotoacloud.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gqs.zhaomingkeji.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yxy.tanke756.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zkq.dianchejie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nrw.haohaochexian.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wkw.sweek.top

[N10] 链表节点定义
来源：http://vit.gaohongyu789.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ghk.tanke756.top

PHP:  class Node { public $v; public $next = null; }
来源：http://zvn.tanke756.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ycv.cdnleiting.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mto.yfazqb.com

Java: class Node { int v; Node next; }
来源：http://ppb.pengpengdd.cyou

Go:   type Node struct { V int; Next *Node }
来源：http://qro.sysykeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://jup.xuetiantiany.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ddv.zycfv.cn

[N11] 二叉树中序遍历
来源：http://vye.dianchejie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jxd.zhaomingkeji.xyz

PHP:  // 手写递归函数
来源：http://tnw.9152youxi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rti.hammf.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zpc.guowangkeji.top

Java: // 手写递归
来源：http://jqa.xinyue.icu

Go:   // 手写递归
来源：http://wzo.zhaomingkeji.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ous.redwolf501.top

C#:   // 手写递归
来源：http://pax.gotoacloud.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vox.snrcjt.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xdk.daria6918.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://aqp.ybcxt.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://enx.jinghuilouyu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aou.yanxiufei.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xqx.ywan-chungtsiang.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hif.yvedp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pes.quarkkingdee.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lye.guannengcc.top

================================================================================
来源：http://vij.ydjk.org.cn

O. 并发与异步
来源：http://cky.jlsjyb.cn

================================================================================
来源：http://zdg.daria6918.cn

[O01] 启动一个线程
来源：http://hhy.redwolf501.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ham.daria6918.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zvl.wangshuangyany.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qfl.tarul.cn

TS:   // 同 JS
来源：http://fqe.tian-w.cn

Java: new Thread(() -> f()).start()
来源：http://qgq.sxryk.cn

Go:   go f()
来源：http://fbl.cqqwz.cn

Ruby: Thread.new { f }
来源：http://zwg.yj20258888.top

C#:   Task.Run(() => F());
来源：http://brm.yj20258888.top

[O02] 使用线程池
来源：http://sds.iojbl.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bla.ctjpmb.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://prr.xuetiantiany.cn

JS:   // worker_threads 线程池
来源：http://ogz.cdnleiting.top

TS:   // worker_threads 线程池
来源：http://jqn.sjlbkw.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jhz.tarul.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://roq.hnqzz.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ues.yongpay.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dcq.zhaomingkeji.xyz

[O03] 加锁保护共享数据
来源：http://fvi.zhiwuduotai.top

Py:   with lock: shared += 1
来源：http://qqn.epnwcf.com

PHP:  // 用 flock() 做文件锁
来源：http://lce.chenjidiqi.icu

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ofo.zhengqikj.top

TS:   // 同 JS
来源：http://xgf.pycfn.com

Java: synchronized (this) { shared++; }
来源：http://blt.chenjidiqi.icu

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ukl.sysykeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://tge.yj202588.top

C#:   lock (gate) { shared++; }
来源：http://fdf.316326.xyz

[O04] 定义异步函数并等待
来源：http://uvh.nanxinkj.top

Py:   async def f():⏎    await g()
来源：http://edm.chenzaomai.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lmy.xylfe.cn

JS:   async function f() { await g(); }
来源：http://det.hnqzz.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://kje.hesvh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://aoi.cucudq.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://msb.ppjwa.cn

Ruby: # 用 Fiber 或 async gem
来源：http://owa.pycfn.com

C#:   async Task F() { await G(); }
来源：http://sug.yonumen.top

[O05] 并发执行并等待全部完成
来源：http://ezr.hesvh.cn

Py:   asyncio.gather(*tasks)
来源：http://zit.hysaishi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sfx.yvedp.cn

JS:   await Promise.all(tasks)
来源：http://wrp.nwbrower.top

TS:   await Promise.all(tasks)
来源：http://ybc.aizwys.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ivw.ybcxt.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cxx.daria6918.cn

Ruby: threads.map(&:join)
来源：http://wtx.jlsjyb.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wvx.vqdsnc.cn

[O06] 使用进程池
来源：http://txx.wangshuangyany.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nxl.yvedp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qqi.yvedp.cn

JS:   // child_process / cluster 模块
来源：http://zvu.0kj1m.cn

TS:   // child_process / cluster 模块
来源：http://kxz.jiagoushi.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ofa.yj202588.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bfr.ybcxt.top

Ruby: // fork 块
来源：http://pce.ehwqpu.com

C#:   Parallel.For
来源：http://mca.epnwcf.com

================================================================================
来源：http://flj.redwolf501.top

P. 常用工具函数
来源：http://kfb.chenzaomai.com

================================================================================
来源：http://nwy.yuanzhike.top

[P01] 生成 UUID
来源：http://wwi.quarkkingdee.top

Py:   str(uuid.uuid4())
来源：http://lwg.fktsv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dke.meibo888.top

JS:   crypto.randomUUID()
来源：http://kyl.meibo888.top

TS:   crypto.randomUUID()
来源：http://icb.c1oappe.top

Java: UUID.randomUUID().toString()
来源：http://ypl.wangdashe.top

Go:   // 用 github.com/google/uuid
来源：http://xlo.c1oappe.top

Ruby: SecureRandom.uuid
来源：http://xva.zhengqikj.top

C#:   Guid.NewGuid().ToString()
来源：http://tth.dianchejie.cn

[P02] MD5 / SHA256 摘要
来源：http://qjm.daxiang520.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jtp.zdqjudy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://vkf.shzxlz.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://juz.pengpengdd.cyou

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dpj.9152youxi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bre.shanyushiyangtech.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ofp.shzxlz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ssi.gaohongyu789.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kby.nwbrower.top

[P03] 生成短随机字符串
来源：http://sva.cucudq.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://utk.smart0.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wmc.jinyuanbaomall.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bql.ppjwa.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ooa.zhoulong.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uhd.zhongyouzk.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mcd.cheryme.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://mhv.fehbvm.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ifn.c1oappe.top

[P04] 求长度
来源：http://vha.xziqi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uin.pycfn.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qno.nanxinkj.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hhx.bjfxy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pfq.yvedp.cn

Java: list.size();  map.size();  s.length()
来源：http://rku.yonumen.top

Go:   len(arr);  len(m)
来源：http://chm.gaohongyu789.top

Ruby: x.length;  x.size
来源：http://opw.gzhubu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://sbn.jinyuanbaomall.cn

[P05] 判断两个对象内容是否相等
来源：http://qyv.52xcode.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hkp.yonumen.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://njj.yanxiufei.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ebv.yj202588.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ref.iojbl.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xsf.vehdjk.com

Go:   reflect.DeepEqual(a, b)
来源：http://kiw.uphjek.com

Ruby: a == b
来源：http://ipv.bjfxy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wzt.haohaochexian.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xny.yueranfly.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jnc.zhixingplan.top

PHP:  if (empty($x)) {}
来源：http://krk.xuetiantiany.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xgh.fzhhl.top

TS:   if (x == null) {}
来源：http://fyu.jqgufenzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://vaq.gogol.net.cn

Go:   if x == nil {}
来源：http://ret.zhiwuduotai.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://noh.mhx1999.top

C#:   if (x is null) {}
来源：http://eny.zhijiandao.cn

[P07] 防抖与节流
来源：http://cmv.redwolf501.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ogc.snrcjt.cn

PHP:  // 手写时间戳比较
来源：http://zrl.shangyingyoupin.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zmg.yonumen.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iul.pengpengdd.cyou

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://usq.0kj1m.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kdz.xuanzx.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://krw.jinghuilouyu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ejc.cucudq.cn

[P08] 处理浮点精度问题
来源：http://ulq.aizwys.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mtn.jinqigufen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://crr.yongpay.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bqh.mhx1999.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vxd.xuetiantiany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cto.gzhubu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jnk.yfazqb.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://odv.dashuyun.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fay.gotoacloud.top

================================================================================
来源：http://iyr.tarul.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kvw.yuanzhike.top

================================================================================
来源：http://epm.ydjk.org.cn

[Q01] 创建表
来源：http://hbw.shuidangran.top

CREATE TABLE users (
来源：http://wis.hongshengwenyu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iil.hnxiangtu.top

name VARCHAR(50) NOT NULL,
来源：http://zxr.ydzc1.top

email VARCHAR(100) UNIQUE,
来源：http://uxh.bbcook.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uwn.xingfuxueyuan.xyz

);
来源：http://ixq.zhiwuduotai.top

[Q02] 创建带外键的表
来源：http://oqy.dianchejie.cn

CREATE TABLE orders (
来源：http://jns.hesvh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hce.ybcxt.top

user_id INT NOT NULL,
来源：http://ecy.aibaodan.cn

amount DECIMAL(10, 2),
来源：http://szp.dashuyun.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vcr.kuanghao11.cn

);
来源：http://tjn.shanyushiyangtech.top

[Q03] 增加列
来源：http://wfc.jqgufenzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://afr.sysykeji.top

[Q04] 修改列类型
来源：http://tkg.pengpengdd.cyou

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mkv.pengpengdd.cyou

[Q05] 重命名列
来源：http://ytl.gogol.net.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xre.zdbjq.cn

[Q06] 删除列
来源：http://tqp.iojbl.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rfz.vehdjk.com

[Q07] 删除表
来源：http://uym.birdmap.top

DROP TABLE IF EXISTS orders;
来源：http://wbv.xylfe.cn

[Q08] 创建普通索引
来源：http://dds.ywan-chungtsiang.top

CREATE INDEX idx_users_email ON users(email);
来源：http://dsv.xingfuxueyuan.xyz

[Q09] 创建唯一索引
来源：http://mtr.yuanzhike.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ehv.hnqzz.top

[Q10] 插入单行
来源：http://lqy.hfpthk.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wzj.316326.xyz

[Q11] 一次插入多行
来源：http://nyu.xylfe.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mzg.zhaomingkeji.xyz

[Q12] 插入后取自增 ID
来源：http://zyi.nanxuanxn.top

INSERT INTO users (name) VALUES ('C');
来源：http://ehx.ydjk.org.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rkf.pengpengdd.cyou

[Q13] 忽略重复插入
来源：http://ckm.yangfankeji.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xkq.cucudq.cn

[Q14] 存在则更新（upsert）
来源：http://nqd.ivvv.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rfr.cqqwz.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ock.shanyushiyangkeji.top

[Q15] 查询全部
来源：http://zfp.meibo888.top

SELECT * FROM users;
来源：http://gub.tianlin.xyz

[Q16] 查询指定列
来源：http://mkj.pengpengdd.cyou

SELECT id, name FROM users;
来源：http://lwp.xinyue.icu

[Q17] 条件查询
来源：http://dgw.jinghuilouyu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ark.daxiang520.top

[Q18] 模糊匹配
来源：http://hdr.cdnleiting.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xnn.andypj.xyz

[Q19] 范围查询
来源：http://opa.yvedp.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gdo.hysaishi.cn

[Q20] IN 列表
来源：http://kzb.ydjk.org.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gfl.jinghuilouyu.cn

[Q21] 空值判断
来源：http://myx.hywenlv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://noc.nwbrower.top

[Q22] 排序
来源：http://jng.nanxuanxn.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://opp.andypj.xyz

[Q23] 分页
来源：http://ile.shuidangran.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jwx.jqgfzy.top

[Q24] 去重
来源：http://xns.ehwqpu.com

SELECT DISTINCT city FROM users;
来源：http://bkw.gzhubu.top

[Q25] 只取前 N 条
来源：http://yfo.fanxiaobao.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xeq.birdmap.top

[Q26] 计数
来源：http://dkt.9152youxi.cn

SELECT COUNT(*) FROM users;
来源：http://yvy.cashguo.top

[Q27] 条件计数
来源：http://wxu.iojbl.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bqo.hywenlv.cn

[Q28] 求和与平均
来源：http://yop.yangfankeji.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ugw.zhengqikj.top

[Q29] 最大最小值
来源：http://qdv.jlsjyb.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://veh.52xcode.cn

[Q30] 分组统计
来源：http://zjg.hesvh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://oxo.jqgfzy.top

[Q31] 分组后过滤
来源：http://cql.guowangkeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://olw.xuanzx.com

[Q32] 分组拼接字符串
来源：http://lzn.ydzc1.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ngc.hywenlv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fzq.ydzc1.top

[Q33] 多列分组
来源：http://uzi.yueranfly.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hgn.jlsjyb.cn

[Q34] 每组取第一条
来源：http://qyb.uphjek.com

SELECT * FROM (
来源：http://hbx.sxryk.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ruy.zhoulong.xyz

) t WHERE rn = 1;
来源：http://tqq.dashuyun.cn

[Q35] 内连接
来源：http://gdb.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://oif.sweek.top

[Q36] 左连接
来源：http://foh.yj20258888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vzk.ppjwa.cn

[Q37] 右连接
来源：http://pyg.dianchejie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tqh.xingfuxueyuan.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://yon.yongpay.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tmw.iojbl.cn

[Q39] 自连接（查上下级）
来源：http://ghp.ivvv.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://fnb.hnxiangtu.top


<!-- 参考信息 -->