代发 wailian999

[N05] 最大公约数
来源：http://ogc.9152youxi.cn

Py:   math.gcd(a, b)
来源：http://qqn.redwolf501.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://slr.epnwcf.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kap.pengpengdd.cyou

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rap.redwolf501.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://aci.tian-w.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lay.pycfn.com

Ruby: a.gcd(b)
来源：http://rlm.aibaodan.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bvx.tianlin.xyz

[N06] 判断回文字符串
来源：http://txw.aibaodan.cn

Py:   s == s[::-1]
来源：http://kaj.vehdjk.com

PHP:  $s === strrev($s);
来源：http://eet.cashguo.top

JS:   s === [...s].reverse().join("")
来源：http://xbw.fehbvm.com

TS:   s === [...s].reverse().join("")
来源：http://uty.ydzc1.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jjh.zdqjudy.top

Go:   // 双指针从两端比较
来源：http://rbj.cdnleiting.top

Ruby: s == s.reverse
来源：http://szd.feifeiyinyue.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://pxm.haohaochexian.top

[N07] 两数之和（返回下标）
来源：http://owp.yonumen.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qta.shzxlz.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://feb.zhaomingkeji.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://rco.zhiwuduotai.top

TS:   // 手写 Map<string, number>
来源：http://mou.zhixingplan.top

Java: // 手写 HashMap
来源：http://pcy.chenzaomai.com

Go:   // 手写 map[int]int
来源：http://vgy.nanxinkj.top

Ruby: // 手写 Hash
来源：http://ndu.zycfv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wjj.cashguo.top

[N08] 生成全排列
来源：http://qtz.fktsv.cn

Py:   itertools.permutations(arr)
来源：http://bes.vqdsnc.cn

PHP:  // 手写递归交换
来源：http://may.dianchejie.cn

JS:   // 手写回溯递归
来源：http://bzz.jinqigfzy.top

TS:   // 手写回溯递归
来源：http://nmm.yanxiufei.cn

Java: // 手写回溯递归
来源：http://opv.cdnleiting.top

Go:   // 手写回溯递归
来源：http://ysj.xziqi.cn

Ruby: arr.permutation.to_a
来源：http://xdr.gogol.net.cn

C#:   // 手写回溯递归
来源：http://hnc.zhiwuduotai.top

[N09] 栈与队列
来源：http://riv.yonumen.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fsz.zhiwuduotai.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jnu.9152youxi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://egq.gzhubu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kug.tanke756.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mut.xylfe.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dnz.svipenyu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jof.sjlbkw.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://egu.fehbvm.com

[N10] 链表节点定义
来源：http://cgo.havefunace.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ipd.zhiwuduotai.top

PHP:  class Node { public $v; public $next = null; }
来源：http://fwo.quarkkingdee.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vqu.feifeiyinyue.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gkx.tanke756.top

Java: class Node { int v; Node next; }
来源：http://sxg.pengpengdd.cyou

Go:   type Node struct { V int; Next *Node }
来源：http://rpy.birdmap.top

Ruby: Node = Struct.new(:v, :next)
来源：http://piq.yuanzhike.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ree.sxryk.cn

[N11] 二叉树中序遍历
来源：http://elz.zhoulong.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rwj.zhaomingkeji.xyz

PHP:  // 手写递归函数
来源：http://qsh.sufxvd.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kvb.gaohongyu789.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://utq.shzxlz.cn

Java: // 手写递归
来源：http://oml.jyoumei.cn

Go:   // 手写递归
来源：http://hve.zdbjq.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rur.cheryme.top

C#:   // 手写递归
来源：http://ibp.daria6918.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xpn.cucudq.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jbq.cheryme.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sqg.ivvv.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dat.yongpay.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jnh.svipenyu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pwo.52xcode.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kgv.ppjwa.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wrq.dianchejie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pna.ydjk.org.cn

================================================================================
来源：http://gss.zdbjq.cn

O. 并发与异步
来源：http://fwm.gotoacloud.top

================================================================================
来源：http://xdv.snrcjt.cn

[O01] 启动一个线程
来源：http://zps.smart0.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://erz.hongshengwenyu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jty.jinyuanbaomall.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://luw.ydzc1.top

TS:   // 同 JS
来源：http://dap.redwolf501.top

Java: new Thread(() -> f()).start()
来源：http://faq.ybcxt.top

Go:   go f()
来源：http://kzu.havefunace.top

Ruby: Thread.new { f }
来源：http://ije.shanyushiyangkeji.top

C#:   Task.Run(() => F());
来源：http://hun.shangyingyoupin.top

[O02] 使用线程池
来源：http://zkt.hnqzz.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pma.pengpengdd.cyou

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qsv.ydjk.org.cn

JS:   // worker_threads 线程池
来源：http://uof.tanke756.top

TS:   // worker_threads 线程池
来源：http://cdh.cqqwz.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yur.jiagoushi.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gcl.xuanzx.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nmq.zhijiandao.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ysq.cucudq.cn

[O03] 加锁保护共享数据
来源：http://dds.yangfankeji.com

Py:   with lock: shared += 1
来源：http://ulo.yanxiufei.cn

PHP:  // 用 flock() 做文件锁
来源：http://yeq.fehbvm.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://voe.meibo888.top

TS:   // 同 JS
来源：http://qcu.fanxiaobao.xyz

Java: synchronized (this) { shared++; }
来源：http://vcd.daria6918.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kob.fzhhl.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://zud.ivvv.top

C#:   lock (gate) { shared++; }
来源：http://fpk.xingfuxueyuan.xyz

[O04] 定义异步函数并等待
来源：http://ack.cheryme.top

Py:   async def f():⏎    await g()
来源：http://oex.chenzaomai.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gcw.guannengcc.top

JS:   async function f() { await g(); }
来源：http://fcd.ctjpmb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://orh.smart0.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rey.sysykeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dmf.tian-w.cn

Ruby: # 用 Fiber 或 async gem
来源：http://scj.gogol.net.cn

C#:   async Task F() { await G(); }
来源：http://ita.hcnkem.com

[O05] 并发执行并等待全部完成
来源：http://izv.haohaochexian.top

Py:   asyncio.gather(*tasks)
来源：http://ifu.zhixingplan.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://alu.sweek.top

JS:   await Promise.all(tasks)
来源：http://tjr.ywan-chungtsiang.top

TS:   await Promise.all(tasks)
来源：http://pex.yvedp.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yae.tian-w.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yvj.chenjidiqi.icu

Ruby: threads.map(&:join)
来源：http://qmp.zhongyouzk.top

C#:   await Task.WhenAll(t1, t2)
来源：http://wge.aizwys.cn

[O06] 使用进程池
来源：http://hqs.hnxiangtu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fiz.zhiwuduotai.top

PHP:  // pcntl_fork 或多进程队列
来源：http://swm.zhiwuduotai.top

JS:   // child_process / cluster 模块
来源：http://bra.jinqigufen.top

TS:   // child_process / cluster 模块
来源：http://dto.meibo888.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://beq.sufxvd.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mis.hammf.cn

Ruby: // fork 块
来源：http://pnz.ctjpmb.com

C#:   Parallel.For
来源：http://fbl.ctjpmb.com

================================================================================
来源：http://bmj.daxiang520.top

P. 常用工具函数
来源：http://ckb.bjfxy.top

================================================================================
来源：http://xbp.snrcjt.cn

[P01] 生成 UUID
来源：http://zhn.jyoumei.cn

Py:   str(uuid.uuid4())
来源：http://trs.daxiang520.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tjo.epnwcf.com

JS:   crypto.randomUUID()
来源：http://ioh.daria6918.cn

TS:   crypto.randomUUID()
来源：http://lnj.shanyushiyangkeji.top

Java: UUID.randomUUID().toString()
来源：http://ygd.sjlbkw.cn

Go:   // 用 github.com/google/uuid
来源：http://wxz.316326.xyz

Ruby: SecureRandom.uuid
来源：http://luc.nanxuanxn.top

C#:   Guid.NewGuid().ToString()
来源：http://zrz.shuidangran.top

[P02] MD5 / SHA256 摘要
来源：http://zfo.dashuyun.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://obu.ivvv.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://mvo.cheryme.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nfe.zhixingplan.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://twc.hcnkem.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ipf.hammf.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mvm.yuanzhike.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hzy.zdbjq.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rgx.zdqjudy.top

[P03] 生成短随机字符串
来源：http://yhh.ppjwa.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://awk.sysykeji.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ieg.birdmap.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tgl.jiagoushi.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bxh.xylfe.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://buy.epnwcf.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ixw.gaohongyu789.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://yim.gzhubu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tge.birdmap.top

[P04] 求长度
来源：http://xgb.zdqjudy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://byc.316326.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ktn.shangyingyoupin.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kus.fzhhl.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bve.havefunace.top

Java: list.size();  map.size();  s.length()
来源：http://boc.tanke756.top

Go:   len(arr);  len(m)
来源：http://ten.hfpthk.cn

Ruby: x.length;  x.size
来源：http://btr.yj202588.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://pyn.jlsjyb.cn

[P05] 判断两个对象内容是否相等
来源：http://vzn.ppjwa.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qqu.cashguo.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ypk.sjlbkw.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pay.jinyuanbaomall.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://odr.ywan-chungtsiang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://igl.xuetiantiany.cn

Go:   reflect.DeepEqual(a, b)
来源：http://oxi.iojbl.cn

Ruby: a == b
来源：http://hno.fanxiaobao.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://avg.cheryme.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hvl.tian-w.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wny.jinqigfzy.top

PHP:  if (empty($x)) {}
来源：http://snx.yuanzhike.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cjd.redwolf501.top

TS:   if (x == null) {}
来源：http://wif.daxiang520.top

Java: if (x == null || x.isEmpty()) {}
来源：http://pdd.nanxuanxn.top

Go:   if x == nil {}
来源：http://sew.ppjwa.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zol.xziqi.cn

C#:   if (x is null) {}
来源：http://val.epnwcf.com

[P07] 防抖与节流
来源：http://lnk.gaohongyu789.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://who.bjfxy.top

PHP:  // 手写时间戳比较
来源：http://rqt.daria6918.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hya.xuanzx.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nbe.fanxiaobao.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://chb.havefunace.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ete.aibaodan.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qjb.ydzc1.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://knd.cucudq.cn

[P08] 处理浮点精度问题
来源：http://wev.iojbl.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tni.andypj.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gzp.xziqi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kta.jinyuanbaomall.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://khq.jqgufenzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pdb.cucudq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bvk.tianlin.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sde.316326.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dsq.nanxuanxn.top

================================================================================
来源：http://nbd.cucudq.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://aoo.ydzc1.top

================================================================================
来源：http://nqu.ppjwa.cn

[Q01] 创建表
来源：http://aay.xziqi.cn

CREATE TABLE users (
来源：http://ppo.hcnkem.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pij.sjlbkw.cn

name VARCHAR(50) NOT NULL,
来源：http://bqh.daria6918.cn

email VARCHAR(100) UNIQUE,
来源：http://lje.cheryme.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cnc.dianchejie.cn

);
来源：http://bjp.cqqwz.cn

[Q02] 创建带外键的表
来源：http://svh.xziqi.cn

CREATE TABLE orders (
来源：http://itj.jyoumei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fjk.zhixingplan.top

user_id INT NOT NULL,
来源：http://ioa.ydjk.org.cn

amount DECIMAL(10, 2),
来源：http://ehy.tanke756.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mpz.jiagoushi.top

);
来源：http://rxw.fengsongda.top

[Q03] 增加列
来源：http://vce.hesvh.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fiy.shangyingyoupin.top

[Q04] 修改列类型
来源：http://wav.xuetiantiany.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dpw.uphjek.com

[Q05] 重命名列
来源：http://ido.yuanzhike.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sor.hesvh.cn

[Q06] 删除列
来源：http://nbp.jinghuilouyu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qql.pycfn.com

[Q07] 删除表
来源：http://vqq.gotoacloud.top

DROP TABLE IF EXISTS orders;
来源：http://zya.sjlbkw.cn

[Q08] 创建普通索引
来源：http://lgh.cheryme.top

CREATE INDEX idx_users_email ON users(email);
来源：http://vpk.sxryk.cn

[Q09] 创建唯一索引
来源：http://yle.sufxvd.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gdl.zhaomingkeji.xyz

[Q10] 插入单行
来源：http://rzm.yj20258888.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://htd.dashuyun.cn

[Q11] 一次插入多行
来源：http://nzw.nanxinkj.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ezu.ppjwa.cn

[Q12] 插入后取自增 ID
来源：http://ecj.sjlbkw.cn

INSERT INTO users (name) VALUES ('C');
来源：http://azh.c1oappe.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oxt.hysaishi.cn

[Q13] 忽略重复插入
来源：http://chw.meibo888.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ukm.yj202588.top

[Q14] 存在则更新（upsert）
来源：http://lwp.shuidangran.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cxg.bbcook.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lle.epnwcf.com

[Q15] 查询全部
来源：http://aph.wangdashe.top

SELECT * FROM users;
来源：http://yzn.jiagoushi.top

[Q16] 查询指定列
来源：http://xor.zhixingplan.top

SELECT id, name FROM users;
来源：http://dtn.nwbrower.top

[Q17] 条件查询
来源：http://bxi.hammf.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lkp.yj20258888.top

[Q18] 模糊匹配
来源：http://atr.yj20258.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pcm.wangdashe.top

[Q19] 范围查询
来源：http://pxc.hcnkem.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://roc.chenzaomai.com

[Q20] IN 列表
来源：http://nla.xziqi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://eoz.xylfe.cn

[Q21] 空值判断
来源：http://gbo.daxiang520.top

SELECT * FROM users WHERE email IS NULL;
来源：http://nwo.epnwcf.com

[Q22] 排序
来源：http://gru.birdmap.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mwv.zhaomingkeji.xyz

[Q23] 分页
来源：http://akn.cqqwz.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wlc.jinqigufen.top

[Q24] 去重
来源：http://mtd.yvedp.cn

SELECT DISTINCT city FROM users;
来源：http://uby.guowangkeji.top

[Q25] 只取前 N 条
来源：http://twj.dianchejie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jyk.ehwqpu.com

[Q26] 计数
来源：http://fdm.sjlbkw.cn

SELECT COUNT(*) FROM users;
来源：http://cka.jiagoushi.top

[Q27] 条件计数
来源：http://lse.sysykeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vkv.haohaochexian.top

[Q28] 求和与平均
来源：http://qlv.yuanzhike.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hfs.fktsv.cn

[Q29] 最大最小值
来源：http://urv.jinghuilouyu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qij.xuanzx.com

[Q30] 分组统计
来源：http://rkz.epnwcf.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cuz.cheryme.top

[Q31] 分组后过滤
来源：http://djz.fzhhl.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://imd.zhengqikj.top

[Q32] 分组拼接字符串
来源：http://kok.wangdashe.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://iyx.shangyingyoupin.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nza.jinghuilouyu.cn

[Q33] 多列分组
来源：http://vsg.jqgufenzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qui.sweek.top

[Q34] 每组取第一条
来源：http://tzx.dianchejie.cn

SELECT * FROM (
来源：http://fvc.shanyushiyangtech.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tlr.gzhubu.top

) t WHERE rn = 1;
来源：http://rum.jinqigufen.top

[Q35] 内连接
来源：http://kai.xinyue.icu

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rke.zhixingplan.top

[Q36] 左连接
来源：http://gtw.zhixingplan.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mdu.quarkkingdee.top

[Q37] 右连接
来源：http://han.shanyushiyangkeji.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gwr.xylfe.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mbx.tanke756.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fwl.tian-w.cn

[Q39] 自连接（查上下级）
来源：http://xnu.redwolf501.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://awm.yonumen.top


<!-- 参考信息 -->