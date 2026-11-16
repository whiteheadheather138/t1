代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wmg.guannengcc.top

[N06] 判断回文字符串
来源：http://cdz.hfpthk.cn

Py:   s == s[::-1]
来源：http://uxm.cdnleiting.top

PHP:  $s === strrev($s);
来源：http://bkl.xuetiantiany.cn

JS:   s === [...s].reverse().join("")
来源：http://ozh.hongshengwenyu.top

TS:   s === [...s].reverse().join("")
来源：http://sqz.yanxiufei.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tsi.jyoumei.cn

Go:   // 双指针从两端比较
来源：http://rih.hongshengwenyu.top

Ruby: s == s.reverse
来源：http://rjd.daxiang520.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://vsc.yongpay.top

[N07] 两数之和（返回下标）
来源：http://kpl.hfpthk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rlw.zhongyouzk.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://eka.xingfuxueyuan.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://six.zhengqikj.top

TS:   // 手写 Map<string, number>
来源：http://pyt.sweek.top

Java: // 手写 HashMap
来源：http://yub.tianlin.xyz

Go:   // 手写 map[int]int
来源：http://urt.birdmap.top

Ruby: // 手写 Hash
来源：http://ekh.nwbrower.top

C#:   // 手写 Dictionary<int, int>
来源：http://jhh.xylfe.cn

[N08] 生成全排列
来源：http://wud.cheryme.top

Py:   itertools.permutations(arr)
来源：http://vnq.svipenyu.cn

PHP:  // 手写递归交换
来源：http://mbd.tian-w.cn

JS:   // 手写回溯递归
来源：http://ksv.smart0.xyz

TS:   // 手写回溯递归
来源：http://xov.jqgufenzy.top

Java: // 手写回溯递归
来源：http://rzg.tian-w.cn

Go:   // 手写回溯递归
来源：http://zcr.yvedp.cn

Ruby: arr.permutation.to_a
来源：http://ksp.snrcjt.cn

C#:   // 手写回溯递归
来源：http://yqn.zhongyouzk.top

[N09] 栈与队列
来源：http://ahd.yueranfly.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fms.chenzaomai.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pdf.smart0.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jzt.zycfv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oac.ydjk.org.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fok.tanke756.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rtt.ivvv.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://krf.ppjwa.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nro.hysaishi.cn

[N10] 链表节点定义
来源：http://que.wangshuangyany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mnl.jinyuanbaomall.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fde.jinghuilouyu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ckn.fehbvm.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rmk.zhijiandao.cn

Java: class Node { int v; Node next; }
来源：http://vbd.ybcxt.top

Go:   type Node struct { V int; Next *Node }
来源：http://oho.fzhhl.top

Ruby: Node = Struct.new(:v, :next)
来源：http://abq.hfpthk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://oyg.yonumen.top

[N11] 二叉树中序遍历
来源：http://exw.pycfn.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vqc.hcnkem.com

PHP:  // 手写递归函数
来源：http://nys.0kj1m.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ceh.vehdjk.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eec.shangyingyoupin.top

Java: // 手写递归
来源：http://ics.tianlin.xyz

Go:   // 手写递归
来源：http://typ.cashguo.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fxi.mhx1999.top

C#:   // 手写递归
来源：http://bws.yuxming.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zmw.zhengqikj.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fts.redwolf501.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hvd.sufxvd.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nnu.sjlbkw.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kzk.xingfuxueyuan.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xyl.jinyuanbaomall.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ytr.yvedp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://urd.quarkkingdee.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kgg.hongshengwenyu.top

================================================================================
来源：http://sfx.zhijiandao.cn

O. 并发与异步
来源：http://vhz.svipenyu.cn

================================================================================
来源：http://cfp.guannengcc.top

[O01] 启动一个线程
来源：http://qao.haohaochexian.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://frp.chenzaomai.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yzy.hcnkem.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://usy.vehdjk.com

TS:   // 同 JS
来源：http://fiw.xinyue.icu

Java: new Thread(() -> f()).start()
来源：http://gfs.hywenlv.cn

Go:   go f()
来源：http://ake.yfazqb.com

Ruby: Thread.new { f }
来源：http://vjl.jlsjyb.cn

C#:   Task.Run(() => F());
来源：http://kmd.fehbvm.com

[O02] 使用线程池
来源：http://wbn.jlsjyb.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ksk.zhaomingkeji.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://suw.yj202588.top

JS:   // worker_threads 线程池
来源：http://gxh.fengsongda.top

TS:   // worker_threads 线程池
来源：http://yig.smart0.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://hva.guannengcc.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://elx.yuxming.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://avq.ywan-chungtsiang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gbq.zdbjq.cn

[O03] 加锁保护共享数据
来源：http://wem.chenjidiqi.icu

Py:   with lock: shared += 1
来源：http://xla.aizwys.cn

PHP:  // 用 flock() 做文件锁
来源：http://vpw.hnxiangtu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gzl.chenzaomai.com

TS:   // 同 JS
来源：http://idl.meibo888.top

Java: synchronized (this) { shared++; }
来源：http://iem.hesvh.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uot.xinyue.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://ovk.iojbl.cn

C#:   lock (gate) { shared++; }
来源：http://fdn.sxryk.cn

[O04] 定义异步函数并等待
来源：http://vwo.hongshengwenyu.top

Py:   async def f():⏎    await g()
来源：http://xpp.dashuyun.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://iud.xuetiantiany.cn

JS:   async function f() { await g(); }
来源：http://ocq.jinqigufen.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ewe.iojbl.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blh.ydzc1.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://odf.jlsjyb.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kzd.9152youxi.cn

C#:   async Task F() { await G(); }
来源：http://hsq.xziqi.cn

[O05] 并发执行并等待全部完成
来源：http://gth.chenzaomai.com

Py:   asyncio.gather(*tasks)
来源：http://xxr.tian-w.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kdr.hywenlv.cn

JS:   await Promise.all(tasks)
来源：http://lzn.zhixingplan.top

TS:   await Promise.all(tasks)
来源：http://bpx.vehdjk.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ttv.yuxming.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cih.guannengcc.top

Ruby: threads.map(&:join)
来源：http://bfu.snrcjt.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xnx.cqqwz.cn

[O06] 使用进程池
来源：http://vuy.hywenlv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bsk.cdnleiting.top

PHP:  // pcntl_fork 或多进程队列
来源：http://nqq.nwbrower.top

JS:   // child_process / cluster 模块
来源：http://fuj.gogol.net.cn

TS:   // child_process / cluster 模块
来源：http://odz.kuanghao11.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wbv.sysykeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oap.jianghu66.top

Ruby: // fork 块
来源：http://qbk.epnwcf.com

C#:   Parallel.For
来源：http://lpw.bjfxy.top

================================================================================
来源：http://ogs.zhongyouzk.top

P. 常用工具函数
来源：http://wnw.jinqigufen.top

================================================================================
来源：http://rky.jianghu66.top

[P01] 生成 UUID
来源：http://bwy.xylfe.cn

Py:   str(uuid.uuid4())
来源：http://hpo.pengpengdd.cyou

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tdl.zdbjq.cn

JS:   crypto.randomUUID()
来源：http://xmb.feifeiyinyue.top

TS:   crypto.randomUUID()
来源：http://qob.sysykeji.top

Java: UUID.randomUUID().toString()
来源：http://hcq.316326.xyz

Go:   // 用 github.com/google/uuid
来源：http://ken.chenzaomai.com

Ruby: SecureRandom.uuid
来源：http://iys.hnxiangtu.top

C#:   Guid.NewGuid().ToString()
来源：http://vep.ivvv.top

[P02] MD5 / SHA256 摘要
来源：http://vhq.yongpay.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rcm.xylfe.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mjb.gotoacloud.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qvz.quarkkingdee.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gkv.hongshengwenyu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://amd.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ofp.jianghu66.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nrc.ehwqpu.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tyq.dashuyun.cn

[P03] 生成短随机字符串
来源：http://kau.ydzc1.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vhy.shzxlz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gpq.xuanzx.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mrb.hesvh.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hvf.pycfn.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ayv.ppjwa.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://amp.tian-w.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hex.jyoumei.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://oos.ehwqpu.com

[P04] 求长度
来源：http://shb.jqgfzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://owz.dashuyun.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hhw.chenjidiqi.icu

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hfj.yueranfly.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vde.pycfn.com

Java: list.size();  map.size();  s.length()
来源：http://lnd.hammf.cn

Go:   len(arr);  len(m)
来源：http://wxv.haohaochexian.top

Ruby: x.length;  x.size
来源：http://epb.daria6918.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://tzd.tarul.cn

[P05] 判断两个对象内容是否相等
来源：http://spk.sjlbkw.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fpc.xylfe.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gtn.tarul.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rai.hfpthk.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://axm.shzxlz.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rtf.ppjwa.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wtc.cucudq.cn

Ruby: a == b
来源：http://txc.aibaodan.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://aui.fengsongda.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://maj.9152youxi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rup.birdmap.top

PHP:  if (empty($x)) {}
来源：http://klm.svipenyu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jfd.xuanzx.com

TS:   if (x == null) {}
来源：http://wwy.zdbjq.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gjw.bjfxy.top

Go:   if x == nil {}
来源：http://dsp.epnwcf.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gvm.zhoulong.xyz

C#:   if (x is null) {}
来源：http://ffq.zhongyouzk.top

[P07] 防抖与节流
来源：http://bbz.tanke756.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uso.yanxiufei.cn

PHP:  // 手写时间戳比较
来源：http://kic.zhongyouzk.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uqj.cdnleiting.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wsu.hammf.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kaj.tian-w.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vgm.havefunace.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://xad.jyoumei.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pwf.iojbl.cn

[P08] 处理浮点精度问题
来源：http://qsv.yonumen.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uxj.epnwcf.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://eqv.jinyuanbaomall.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://onp.yvedp.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://psu.aibaodan.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zep.gotoacloud.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tcr.jlsjyb.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gqn.yj20258888.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xic.jlsjyb.cn

================================================================================
来源：http://stn.fzhhl.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sue.cqqwz.cn

================================================================================
来源：http://vvs.sysykeji.top

[Q01] 创建表
来源：http://gzn.smart0.xyz

CREATE TABLE users (
来源：http://lot.chenzaomai.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ubm.cheryme.top

name VARCHAR(50) NOT NULL,
来源：http://wqt.chenzaomai.com

email VARCHAR(100) UNIQUE,
来源：http://gsd.cqqwz.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jmr.yongpay.top

);
来源：http://iqz.c1oappe.top

[Q02] 创建带外键的表
来源：http://ldu.sufxvd.cn

CREATE TABLE orders (
来源：http://lae.yanxiufei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xfw.hongshengwenyu.top

user_id INT NOT NULL,
来源：http://xzb.iojbl.cn

amount DECIMAL(10, 2),
来源：http://mua.zhiwuduotai.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bug.iojbl.cn

);
来源：http://uhp.gotoacloud.top

[Q03] 增加列
来源：http://fvy.shanyushiyangkeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uvz.kuanghao11.cn

[Q04] 修改列类型
来源：http://euy.hysaishi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yqx.sweek.top

[Q05] 重命名列
来源：http://hjy.ywan-chungtsiang.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kyw.xziqi.cn

[Q06] 删除列
来源：http://kou.xziqi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vem.yj202588.top

[Q07] 删除表
来源：http://nap.shanyushiyangtech.top

DROP TABLE IF EXISTS orders;
来源：http://une.guannengcc.top

[Q08] 创建普通索引
来源：http://any.yj20258888.top

CREATE INDEX idx_users_email ON users(email);
来源：http://zkf.zhiwuduotai.top

[Q09] 创建唯一索引
来源：http://ijr.wangshuangyany.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kxo.havefunace.top

[Q10] 插入单行
来源：http://did.jianghu66.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kra.yuxming.cn

[Q11] 一次插入多行
来源：http://sjw.cheryme.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vwg.fktsv.cn

[Q12] 插入后取自增 ID
来源：http://hch.shanyushiyangtech.top

INSERT INTO users (name) VALUES ('C');
来源：http://hka.yanxiufei.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ftd.jyoumei.cn

[Q13] 忽略重复插入
来源：http://jvz.ivvv.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nwg.cheryme.top

[Q14] 存在则更新（upsert）
来源：http://zgs.pycfn.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ckf.zhengqikj.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yxg.ivvv.top

[Q15] 查询全部
来源：http://ylj.xingfuxueyuan.xyz

SELECT * FROM users;
来源：http://bvl.pengpengdd.cyou

[Q16] 查询指定列
来源：http://idl.wangshuangyany.cn

SELECT id, name FROM users;
来源：http://ldx.hysaishi.cn

[Q17] 条件查询
来源：http://awr.yj20258.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cdn.daria6918.cn

[Q18] 模糊匹配
来源：http://fka.ehwqpu.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sys.ydzc1.top

[Q19] 范围查询
来源：http://tjj.316326.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://stl.jinqigufen.top

[Q20] IN 列表
来源：http://bwl.hysaishi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iuv.fehbvm.com

[Q21] 空值判断
来源：http://gmi.zhongyouzk.top

SELECT * FROM users WHERE email IS NULL;
来源：http://jrw.sweek.top

[Q22] 排序
来源：http://ufc.dianchejie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rpg.aizwys.cn

[Q23] 分页
来源：http://aod.9152youxi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tnb.pengpengdd.cyou

[Q24] 去重
来源：http://ioy.cashguo.top

SELECT DISTINCT city FROM users;
来源：http://lur.hywenlv.cn

[Q25] 只取前 N 条
来源：http://gfk.guannengcc.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pms.havefunace.top

[Q26] 计数
来源：http://odk.nanxinkj.top

SELECT COUNT(*) FROM users;
来源：http://kbo.jqgfzy.top

[Q27] 条件计数
来源：http://huw.aizwys.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nls.fanxiaobao.xyz

[Q28] 求和与平均
来源：http://frk.hfpthk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ehw.uphjek.com

[Q29] 最大最小值
来源：http://wjz.jianghu66.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://qxs.zhijiandao.cn

[Q30] 分组统计
来源：http://ukb.zhixingplan.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://iwo.nwbrower.top

[Q31] 分组后过滤
来源：http://gca.fktsv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jde.cdnleiting.top

[Q32] 分组拼接字符串
来源：http://ddn.hywenlv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kvj.zhiwuduotai.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wsw.chenjidiqi.icu

[Q33] 多列分组
来源：http://xui.jinyuanbaomall.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pxw.bjfxy.top

[Q34] 每组取第一条
来源：http://afi.xingfuxueyuan.xyz

SELECT * FROM (
来源：http://cww.ydjk.org.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kjk.tian-w.cn

) t WHERE rn = 1;
来源：http://ayz.nanxuanxn.top

[Q35] 内连接
来源：http://cpb.vehdjk.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tqk.9152youxi.cn

[Q36] 左连接
来源：http://gym.aibaodan.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://swt.jinqigufen.top

[Q37] 右连接
来源：http://ngx.hnqzz.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wfv.xziqi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rfh.cdnleiting.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ejf.cashguo.top

[Q39] 自连接（查上下级）
来源：http://fbm.jinyuanbaomall.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fhs.daria6918.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kgz.nwbrower.top

[Q40] 交叉连接（笛卡尔积）
来源：http://uks.jinqigfzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mbi.zhongyouzk.top

[Q41] 多表连接
来源：http://arg.zdqjudy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://kax.sufxvd.cn

JOIN users u ON u.id = o.user_id
来源：http://vgy.ehwqpu.com

JOIN products p ON p.id = o.product_id;
来源：http://oxw.ctjpmb.com

[Q42] 连接条件附加过滤
来源：http://clh.cucudq.cn


<!-- 参考信息 -->