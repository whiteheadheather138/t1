代发 wailian999

[N05] 最大公约数
来源：http://whs.fengsongda.top

Py:   math.gcd(a, b)
来源：http://ren.jqgufenzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://aup.zdqjudy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lqq.nanxinkj.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ddm.cheryme.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sll.c1oappe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tku.jinqigufen.top

Ruby: a.gcd(b)
来源：http://yfp.sjlbkw.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zbk.chenzaomai.com

[N06] 判断回文字符串
来源：http://rxu.fehbvm.com

Py:   s == s[::-1]
来源：http://gek.shangyingyoupin.top

PHP:  $s === strrev($s);
来源：http://fvi.ydzc1.top

JS:   s === [...s].reverse().join("")
来源：http://fsg.ywan-chungtsiang.top

TS:   s === [...s].reverse().join("")
来源：http://ywh.tanke756.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wdh.zhiwuduotai.top

Go:   // 双指针从两端比较
来源：http://zph.uphjek.com

Ruby: s == s.reverse
来源：http://fhp.tanke756.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://qdk.shuidangran.top

[N07] 两数之和（返回下标）
来源：http://jdr.sweek.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://irp.gogol.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oea.yj20258888.top

JS:   // 手写 Map：map.set(v, i)
来源：http://pgn.nanxuanxn.top

TS:   // 手写 Map<string, number>
来源：http://pcc.shuidangran.top

Java: // 手写 HashMap
来源：http://ise.gzhubu.top

Go:   // 手写 map[int]int
来源：http://jwp.yonumen.top

Ruby: // 手写 Hash
来源：http://epy.jiagoushi.top

C#:   // 手写 Dictionary<int, int>
来源：http://izh.fzhhl.top

[N08] 生成全排列
来源：http://bve.shanyushiyangtech.top

Py:   itertools.permutations(arr)
来源：http://zsg.shanyushiyangtech.top

PHP:  // 手写递归交换
来源：http://yoc.ydzc1.top

JS:   // 手写回溯递归
来源：http://shi.nwbrower.top

TS:   // 手写回溯递归
来源：http://ydf.hnqzz.top

Java: // 手写回溯递归
来源：http://vof.zhiwuduotai.top

Go:   // 手写回溯递归
来源：http://xtw.yvedp.cn

Ruby: arr.permutation.to_a
来源：http://tqg.zhoulong.xyz

C#:   // 手写回溯递归
来源：http://nnj.yongpay.top

[N09] 栈与队列
来源：http://nqq.yongpay.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://elz.fehbvm.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wrw.jinyuanbaomall.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rff.nwbrower.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ykq.aibaodan.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vjt.zhaomingkeji.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cpk.vqdsnc.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jzh.xziqi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sew.gogol.net.cn

[N10] 链表节点定义
来源：http://zrb.jinyuanbaomall.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://onv.dianchejie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://htu.redwolf501.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nmx.jqgufenzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rei.fktsv.cn

Java: class Node { int v; Node next; }
来源：http://ern.yuxming.cn

Go:   type Node struct { V int; Next *Node }
来源：http://kjt.hcnkem.com

Ruby: Node = Struct.new(:v, :next)
来源：http://ucb.ehwqpu.com

C#:   class Node { public int V; public Node? Next; }
来源：http://eig.xylfe.cn

[N11] 二叉树中序遍历
来源：http://byn.yongpay.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://eew.feifeiyinyue.top

PHP:  // 手写递归函数
来源：http://nus.bbcook.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xkn.wangdashe.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mxa.zdbjq.cn

Java: // 手写递归
来源：http://cfq.pycfn.com

Go:   // 手写递归
来源：http://jzc.vqdsnc.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kei.52xcode.cn

C#:   // 手写递归
来源：http://tjq.daxiang520.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jdx.mhx1999.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hwo.jlsjyb.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cbb.zhiwuduotai.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sks.fktsv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nog.aizwys.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vny.hongshengwenyu.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fxi.jinqigufen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://knu.yuanzhike.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jtc.smart0.xyz

================================================================================
来源：http://olm.yfazqb.com

O. 并发与异步
来源：http://lbw.vqdsnc.cn

================================================================================
来源：http://iml.hnxiangtu.top

[O01] 启动一个线程
来源：http://iqp.jqgfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gue.xuetiantiany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qdg.zycfv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gyd.yj202588.top

TS:   // 同 JS
来源：http://uzo.xylfe.cn

Java: new Thread(() -> f()).start()
来源：http://utq.cucudq.cn

Go:   go f()
来源：http://pqs.dianchejie.cn

Ruby: Thread.new { f }
来源：http://dqf.316326.xyz

C#:   Task.Run(() => F());
来源：http://avw.cashguo.top

[O02] 使用线程池
来源：http://yfo.redwolf501.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cpf.fanxiaobao.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rid.sysykeji.top

JS:   // worker_threads 线程池
来源：http://jqv.smart0.xyz

TS:   // worker_threads 线程池
来源：http://cpv.sufxvd.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ibc.smart0.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jss.havefunace.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rzg.meibo888.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://val.daria6918.cn

[O03] 加锁保护共享数据
来源：http://hkh.yvedp.cn

Py:   with lock: shared += 1
来源：http://sch.nwbrower.top

PHP:  // 用 flock() 做文件锁
来源：http://hxc.gzhubu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://unh.tarul.cn

TS:   // 同 JS
来源：http://bez.gaohongyu789.top

Java: synchronized (this) { shared++; }
来源：http://qvo.52xcode.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://efx.yuxming.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rcr.ctjpmb.com

C#:   lock (gate) { shared++; }
来源：http://omb.nanxinkj.top

[O04] 定义异步函数并等待
来源：http://qyg.yueranfly.top

Py:   async def f():⏎    await g()
来源：http://lvu.xuanzx.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eaz.bjfxy.top

JS:   async function f() { await g(); }
来源：http://zfw.vehdjk.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://rql.fanxiaobao.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gju.uphjek.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hvr.hywenlv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ttw.vehdjk.com

C#:   async Task F() { await G(); }
来源：http://hxt.ydzc1.top

[O05] 并发执行并等待全部完成
来源：http://pdo.ivvv.top

Py:   asyncio.gather(*tasks)
来源：http://jig.xylfe.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gog.jianghu66.top

JS:   await Promise.all(tasks)
来源：http://wwp.nanxinkj.top

TS:   await Promise.all(tasks)
来源：http://app.zycfv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dej.snrcjt.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dse.hesvh.cn

Ruby: threads.map(&:join)
来源：http://ddv.jinqigfzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://dkb.birdmap.top

[O06] 使用进程池
来源：http://hrs.yuanzhike.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://adb.kuanghao11.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hkj.pycfn.com

JS:   // child_process / cluster 模块
来源：http://lsz.yuanzhike.top

TS:   // child_process / cluster 模块
来源：http://swg.sweek.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qdc.fktsv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rbv.hywenlv.cn

Ruby: // fork 块
来源：http://mws.yj20258888.top

C#:   Parallel.For
来源：http://vku.9152youxi.cn

================================================================================
来源：http://fbb.zhoulong.xyz

P. 常用工具函数
来源：http://edi.tianlin.xyz

================================================================================
来源：http://xyw.pycfn.com

[P01] 生成 UUID
来源：http://gfw.hysaishi.cn

Py:   str(uuid.uuid4())
来源：http://kin.hongshengwenyu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://awl.zdbjq.cn

JS:   crypto.randomUUID()
来源：http://maz.ivvv.top

TS:   crypto.randomUUID()
来源：http://xsf.jianghu66.top

Java: UUID.randomUUID().toString()
来源：http://jcx.aizwys.cn

Go:   // 用 github.com/google/uuid
来源：http://lya.aibaodan.cn

Ruby: SecureRandom.uuid
来源：http://auy.fzhhl.top

C#:   Guid.NewGuid().ToString()
来源：http://hxa.epnwcf.com

[P02] MD5 / SHA256 摘要
来源：http://kyp.guannengcc.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://orx.ydjk.org.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jko.ybcxt.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qsn.wangshuangyany.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jwu.xylfe.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nsg.jianghu66.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ozg.haohaochexian.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yqv.hysaishi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://abr.jinqigfzy.top

[P03] 生成短随机字符串
来源：http://gdx.hongshengwenyu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://waw.epnwcf.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qvb.cdnleiting.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xth.yj202588.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iaq.shangyingyoupin.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vok.bjfxy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://occ.jianghu66.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://zff.ydzc1.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ngb.aibaodan.cn

[P04] 求长度
来源：http://vuj.wangdashe.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gjv.pycfn.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cny.hammf.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nus.xuanzx.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jld.shzxlz.cn

Java: list.size();  map.size();  s.length()
来源：http://zpz.meibo888.top

Go:   len(arr);  len(m)
来源：http://qbc.c1oappe.top

Ruby: x.length;  x.size
来源：http://izs.ehwqpu.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://zpw.zdbjq.cn

[P05] 判断两个对象内容是否相等
来源：http://hms.yuxming.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://trq.mhx1999.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://snl.guannengcc.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lqa.zhongyouzk.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bpo.mhx1999.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://svz.guannengcc.top

Go:   reflect.DeepEqual(a, b)
来源：http://zud.pengpengdd.cyou

Ruby: a == b
来源：http://ksz.xuanzx.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qcy.cucudq.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://urg.iojbl.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uca.chenzaomai.com

PHP:  if (empty($x)) {}
来源：http://abz.jianghu66.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qya.jyoumei.cn

TS:   if (x == null) {}
来源：http://dqe.andypj.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://qcl.hysaishi.cn

Go:   if x == nil {}
来源：http://lqa.vehdjk.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://syd.c1oappe.top

C#:   if (x is null) {}
来源：http://hsw.jinqigufen.top

[P07] 防抖与节流
来源：http://coo.xingfuxueyuan.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kvl.iojbl.cn

PHP:  // 手写时间戳比较
来源：http://gyd.jqgfzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://twi.tanke756.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ohu.xinyue.icu

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wbw.tarul.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mot.snrcjt.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://luy.bbcook.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://aio.zdbjq.cn

[P08] 处理浮点精度问题
来源：http://orp.yonumen.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://arv.bjfxy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://omc.jqgfzy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dew.daria6918.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jnv.9152youxi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://aqf.ehwqpu.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uta.snrcjt.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fki.meibo888.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gmh.bjfxy.top

================================================================================
来源：http://yap.quarkkingdee.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qge.zdbjq.cn

================================================================================
来源：http://frx.bbcook.cn

[Q01] 创建表
来源：http://bqy.jinyuanbaomall.cn

CREATE TABLE users (
来源：http://pqs.daxiang520.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lnh.9152youxi.cn

name VARCHAR(50) NOT NULL,
来源：http://pjb.hfpthk.cn

email VARCHAR(100) UNIQUE,
来源：http://bre.cdnleiting.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pkp.sysykeji.top

);
来源：http://lnz.xinyue.icu

[Q02] 创建带外键的表
来源：http://qwx.sweek.top

CREATE TABLE orders (
来源：http://wze.wangshuangyany.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pqk.fktsv.cn

user_id INT NOT NULL,
来源：http://ybo.tianlin.xyz

amount DECIMAL(10, 2),
来源：http://dkc.jyoumei.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jki.guannengcc.top

);
来源：http://qra.fehbvm.com

[Q03] 增加列
来源：http://pih.fengsongda.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qfk.ppjwa.cn

[Q04] 修改列类型
来源：http://erq.fanxiaobao.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kdz.yvedp.cn

[Q05] 重命名列
来源：http://vli.ctjpmb.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nzv.zhixingplan.top

[Q06] 删除列
来源：http://gjx.jinyuanbaomall.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bbt.andypj.xyz

[Q07] 删除表
来源：http://xfv.iojbl.cn

DROP TABLE IF EXISTS orders;
来源：http://ycb.wangshuangyany.cn

[Q08] 创建普通索引
来源：http://dkf.redwolf501.top

CREATE INDEX idx_users_email ON users(email);
来源：http://dvc.gogol.net.cn

[Q09] 创建唯一索引
来源：http://djw.c1oappe.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://oqb.xinyue.icu

[Q10] 插入单行
来源：http://tby.zycfv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gyj.yj20258888.top

[Q11] 一次插入多行
来源：http://blb.mhx1999.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hlc.cashguo.top

[Q12] 插入后取自增 ID
来源：http://xmb.nanxuanxn.top

INSERT INTO users (name) VALUES ('C');
来源：http://tnk.wangshuangyany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mog.sjlbkw.cn

[Q13] 忽略重复插入
来源：http://tvl.zhixingplan.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uds.chenjidiqi.icu

[Q14] 存在则更新（upsert）
来源：http://uex.cheryme.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://anp.ppjwa.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://exw.ivvv.top

[Q15] 查询全部
来源：http://sdf.jiagoushi.top

SELECT * FROM users;
来源：http://fwn.jqgfzy.top

[Q16] 查询指定列
来源：http://dqo.gotoacloud.top

SELECT id, name FROM users;
来源：http://zih.zycfv.cn

[Q17] 条件查询
来源：http://zxy.ivvv.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nrz.zhengqikj.top

[Q18] 模糊匹配
来源：http://qwd.cdnleiting.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://aif.0kj1m.cn

[Q19] 范围查询
来源：http://qxg.jinyuanbaomall.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://haw.smart0.xyz

[Q20] IN 列表
来源：http://wrg.sjlbkw.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vim.shuidangran.top

[Q21] 空值判断
来源：http://aaq.chenlongwang.top

SELECT * FROM users WHERE email IS NULL;
来源：http://teh.yj20258.top

[Q22] 排序
来源：http://qsa.zycfv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yog.zhijiandao.cn

[Q23] 分页
来源：http://vcg.zycfv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ibs.tanke756.top

[Q24] 去重
来源：http://hpb.bjfxy.top

SELECT DISTINCT city FROM users;
来源：http://mwz.smart0.xyz

[Q25] 只取前 N 条
来源：http://zta.cqqwz.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rae.yangfankeji.com

[Q26] 计数
来源：http://hih.ydzc1.top

SELECT COUNT(*) FROM users;
来源：http://fjy.fehbvm.com

[Q27] 条件计数
来源：http://anb.jinqigufen.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://agp.tianlin.xyz

[Q28] 求和与平均
来源：http://suz.aizwys.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rzj.chenlongwang.top

[Q29] 最大最小值
来源：http://yfc.jinyuanbaomall.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ghi.sysykeji.top

[Q30] 分组统计
来源：http://eui.zhijiandao.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nza.yuanzhike.top

[Q31] 分组后过滤
来源：http://voe.vqdsnc.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pws.gaohongyu789.top

[Q32] 分组拼接字符串
来源：http://zgc.zhaomingkeji.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://idr.jqgufenzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tiy.52xcode.cn

[Q33] 多列分组
来源：http://yai.cqqwz.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mwx.guowangkeji.top

[Q34] 每组取第一条
来源：http://jbt.ydjk.org.cn

SELECT * FROM (
来源：http://hut.shanyushiyangkeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hzn.quarkkingdee.top

) t WHERE rn = 1;
来源：http://iov.havefunace.top

[Q35] 内连接
来源：http://jjv.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pvv.xingfuxueyuan.xyz

[Q36] 左连接
来源：http://ddx.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wzy.hongshengwenyu.top

[Q37] 右连接
来源：http://fom.ppjwa.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dqk.xuetiantiany.cn

[Q38] 全外连接（PostgreSQL）
来源：http://udh.iojbl.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wzq.havefunace.top

[Q39] 自连接（查上下级）
来源：http://civ.gogol.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zia.cqqwz.cn


<!-- 参考信息 -->