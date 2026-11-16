代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wzk.hesvh.cn

[N06] 判断回文字符串
来源：http://flb.xuanzx.com

Py:   s == s[::-1]
来源：http://keh.bbcook.cn

PHP:  $s === strrev($s);
来源：http://qrl.andypj.xyz

JS:   s === [...s].reverse().join("")
来源：http://mvd.shuidangran.top

TS:   s === [...s].reverse().join("")
来源：http://bpd.dianchejie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dye.jinghuilouyu.cn

Go:   // 双指针从两端比较
来源：http://jbu.nanxuanxn.top

Ruby: s == s.reverse
来源：http://pdh.smart0.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://oxi.zycfv.cn

[N07] 两数之和（返回下标）
来源：http://bse.shanyushiyangkeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wzk.hysaishi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yrw.hammf.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kkt.chenlongwang.top

TS:   // 手写 Map<string, number>
来源：http://znq.chenjidiqi.icu

Java: // 手写 HashMap
来源：http://ush.yuxming.cn

Go:   // 手写 map[int]int
来源：http://ept.tianlin.xyz

Ruby: // 手写 Hash
来源：http://qwu.fktsv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qww.zycfv.cn

[N08] 生成全排列
来源：http://vce.svipenyu.cn

Py:   itertools.permutations(arr)
来源：http://ljg.tarul.cn

PHP:  // 手写递归交换
来源：http://aqe.dianchejie.cn

JS:   // 手写回溯递归
来源：http://pah.daria6918.cn

TS:   // 手写回溯递归
来源：http://dtu.gotoacloud.top

Java: // 手写回溯递归
来源：http://cfq.jqgufenzy.top

Go:   // 手写回溯递归
来源：http://klu.sysykeji.top

Ruby: arr.permutation.to_a
来源：http://xcf.hfpthk.cn

C#:   // 手写回溯递归
来源：http://iyf.52xcode.cn

[N09] 栈与队列
来源：http://ewm.zhaomingkeji.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zcy.hesvh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gfn.hcnkem.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ydq.havefunace.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rwn.yonumen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://svx.guannengcc.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bht.jinyuanbaomall.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wwv.gzhubu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jbx.ehwqpu.com

[N10] 链表节点定义
来源：http://dev.cucudq.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qiu.yuanzhike.top

PHP:  class Node { public $v; public $next = null; }
来源：http://fwe.ybcxt.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dhr.xinyue.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://crp.ywan-chungtsiang.top

Java: class Node { int v; Node next; }
来源：http://han.wangdashe.top

Go:   type Node struct { V int; Next *Node }
来源：http://qzn.bjfxy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://jaz.hammf.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zfj.bjfxy.top

[N11] 二叉树中序遍历
来源：http://zgc.fanxiaobao.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://iqc.bbcook.cn

PHP:  // 手写递归函数
来源：http://hor.redwolf501.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kfw.xinyue.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gqw.iojbl.cn

Java: // 手写递归
来源：http://kug.zhijiandao.cn

Go:   // 手写递归
来源：http://txq.gaohongyu789.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xox.sjlbkw.cn

C#:   // 手写递归
来源：http://zsj.zycfv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dqg.zdqjudy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lyi.xuanzx.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://okv.xinyue.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ujc.ydzc1.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://grg.guannengcc.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ozu.yj20258888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dmk.xuanzx.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mcb.andypj.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ory.hnxiangtu.top

================================================================================
来源：http://llp.redwolf501.top

O. 并发与异步
来源：http://xcb.uphjek.com

================================================================================
来源：http://hlc.snrcjt.cn

[O01] 启动一个线程
来源：http://jmx.fanxiaobao.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ddh.ydjk.org.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qwn.xinyue.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jds.vehdjk.com

TS:   // 同 JS
来源：http://nxp.zhoulong.xyz

Java: new Thread(() -> f()).start()
来源：http://zpq.cucudq.cn

Go:   go f()
来源：http://ett.316326.xyz

Ruby: Thread.new { f }
来源：http://qgo.fzhhl.top

C#:   Task.Run(() => F());
来源：http://dcl.yfazqb.com

[O02] 使用线程池
来源：http://jvh.redwolf501.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jus.pengpengdd.cyou

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tyw.andypj.xyz

JS:   // worker_threads 线程池
来源：http://mcd.cheryme.top

TS:   // worker_threads 线程池
来源：http://fnr.0kj1m.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kpr.c1oappe.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ulh.sysykeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wnm.feifeiyinyue.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wdk.nanxuanxn.top

[O03] 加锁保护共享数据
来源：http://lof.gzhubu.top

Py:   with lock: shared += 1
来源：http://syl.dianchejie.cn

PHP:  // 用 flock() 做文件锁
来源：http://zdi.52xcode.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tfm.hesvh.cn

TS:   // 同 JS
来源：http://ywf.52xcode.cn

Java: synchronized (this) { shared++; }
来源：http://mgv.jinqigfzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mqo.sxryk.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://eoq.xuanzx.com

C#:   lock (gate) { shared++; }
来源：http://wus.uphjek.com

[O04] 定义异步函数并等待
来源：http://ylm.shuidangran.top

Py:   async def f():⏎    await g()
来源：http://krh.cashguo.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bfd.xuanzx.com

JS:   async function f() { await g(); }
来源：http://xay.hnqzz.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://wmg.yvedp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://clz.daxiang520.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bxd.fanxiaobao.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://qfv.zhixingplan.top

C#:   async Task F() { await G(); }
来源：http://kpp.jinyuanbaomall.cn

[O05] 并发执行并等待全部完成
来源：http://oao.yuanzhike.top

Py:   asyncio.gather(*tasks)
来源：http://jmk.ctjpmb.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tkl.ehwqpu.com

JS:   await Promise.all(tasks)
来源：http://vcg.zhoulong.xyz

TS:   await Promise.all(tasks)
来源：http://ltc.wangdashe.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vdb.cqqwz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jbu.haohaochexian.top

Ruby: threads.map(&:join)
来源：http://thc.feifeiyinyue.top

C#:   await Task.WhenAll(t1, t2)
来源：http://tmm.hnqzz.top

[O06] 使用进程池
来源：http://ewg.gzhubu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qzg.0kj1m.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pko.dianchejie.cn

JS:   // child_process / cluster 模块
来源：http://aeq.snrcjt.cn

TS:   // child_process / cluster 模块
来源：http://dwv.havefunace.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pot.havefunace.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vmr.vehdjk.com

Ruby: // fork 块
来源：http://mjn.zhaomingkeji.xyz

C#:   Parallel.For
来源：http://ten.fehbvm.com

================================================================================
来源：http://kui.zhiwuduotai.top

P. 常用工具函数
来源：http://otz.zhiwuduotai.top

================================================================================
来源：http://gzi.ybcxt.top

[P01] 生成 UUID
来源：http://jxd.yueranfly.top

Py:   str(uuid.uuid4())
来源：http://yxf.dashuyun.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://syj.jyoumei.cn

JS:   crypto.randomUUID()
来源：http://lwu.hysaishi.cn

TS:   crypto.randomUUID()
来源：http://zcd.316326.xyz

Java: UUID.randomUUID().toString()
来源：http://qvf.xinyue.icu

Go:   // 用 github.com/google/uuid
来源：http://pln.guowangkeji.top

Ruby: SecureRandom.uuid
来源：http://rnv.jianghu66.top

C#:   Guid.NewGuid().ToString()
来源：http://uav.ybcxt.top

[P02] MD5 / SHA256 摘要
来源：http://kky.jinyuanbaomall.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gun.yj20258888.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://mtu.hywenlv.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uha.hcnkem.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dso.haohaochexian.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ibn.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vnq.daria6918.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hav.hysaishi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dcg.bbcook.cn

[P03] 生成短随机字符串
来源：http://xjl.yj20258.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sot.jianghu66.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oxk.jiagoushi.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kxy.gzhubu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://knj.ywan-chungtsiang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uno.0kj1m.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zqe.bjfxy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://cnz.vqdsnc.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xum.0kj1m.cn

[P04] 求长度
来源：http://dxi.meibo888.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jbj.kuanghao11.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kgr.jqgufenzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xna.xuetiantiany.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dlx.zhaomingkeji.xyz

Java: list.size();  map.size();  s.length()
来源：http://eml.yj20258.top

Go:   len(arr);  len(m)
来源：http://xga.jqgufenzy.top

Ruby: x.length;  x.size
来源：http://vwh.guannengcc.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://kfu.sweek.top

[P05] 判断两个对象内容是否相等
来源：http://kbs.yueranfly.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://rrf.jianghu66.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mpf.guowangkeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xns.yanxiufei.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qvn.ybcxt.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xaj.xinyue.icu

Go:   reflect.DeepEqual(a, b)
来源：http://rdd.meibo888.top

Ruby: a == b
来源：http://rdu.daria6918.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://oty.c1oappe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vqg.c1oappe.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nqe.hammf.cn

PHP:  if (empty($x)) {}
来源：http://vbv.ctjpmb.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://knq.shuidangran.top

TS:   if (x == null) {}
来源：http://bpw.ppjwa.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://tms.jianghu66.top

Go:   if x == nil {}
来源：http://wjm.cdnleiting.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://weq.tarul.cn

C#:   if (x is null) {}
来源：http://zod.xingfuxueyuan.xyz

[P07] 防抖与节流
来源：http://ali.iojbl.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kpd.hnxiangtu.top

PHP:  // 手写时间戳比较
来源：http://wko.ydjk.org.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fto.bbcook.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fdj.ywan-chungtsiang.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qyj.xingfuxueyuan.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wls.ppjwa.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gaf.ehwqpu.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xgn.vehdjk.com

[P08] 处理浮点精度问题
来源：http://bgv.jinyuanbaomall.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ewc.yuanzhike.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bhx.ywan-chungtsiang.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ips.fzhhl.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wup.redwolf501.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yno.jinqigfzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wck.sweek.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lgn.quarkkingdee.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ojw.fengsongda.top

================================================================================
来源：http://qam.meibo888.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gif.zhijiandao.cn

================================================================================
来源：http://pkz.meibo888.top

[Q01] 创建表
来源：http://qxq.yongpay.top

CREATE TABLE users (
来源：http://ssx.cqqwz.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rdl.smart0.xyz

name VARCHAR(50) NOT NULL,
来源：http://zbg.shzxlz.cn

email VARCHAR(100) UNIQUE,
来源：http://kft.bbcook.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sct.aizwys.cn

);
来源：http://yyj.fengsongda.top

[Q02] 创建带外键的表
来源：http://vkm.jinghuilouyu.cn

CREATE TABLE orders (
来源：http://mum.hesvh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zhi.zhiwuduotai.top

user_id INT NOT NULL,
来源：http://okh.c1oappe.top

amount DECIMAL(10, 2),
来源：http://har.zhoulong.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fcm.sweek.top

);
来源：http://lwi.uphjek.com

[Q03] 增加列
来源：http://bgv.hcnkem.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wej.tian-w.cn

[Q04] 修改列类型
来源：http://gld.ivvv.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ukg.haohaochexian.top

[Q05] 重命名列
来源：http://jnz.316326.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fsy.yuanzhike.top

[Q06] 删除列
来源：http://lwb.andypj.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://wia.zhaomingkeji.xyz

[Q07] 删除表
来源：http://htk.zhijiandao.cn

DROP TABLE IF EXISTS orders;
来源：http://coa.kuanghao11.cn

[Q08] 创建普通索引
来源：http://vsg.chenlongwang.top

CREATE INDEX idx_users_email ON users(email);
来源：http://tsu.zhongyouzk.top

[Q09] 创建唯一索引
来源：http://akt.bjfxy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vkd.haohaochexian.top

[Q10] 插入单行
来源：http://cbu.chenlongwang.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://azl.birdmap.top

[Q11] 一次插入多行
来源：http://hlj.sjlbkw.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wuk.aibaodan.cn

[Q12] 插入后取自增 ID
来源：http://gaj.zdqjudy.top

INSERT INTO users (name) VALUES ('C');
来源：http://cqz.jinqigufen.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gbh.gaohongyu789.top

[Q13] 忽略重复插入
来源：http://ppk.ywan-chungtsiang.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qoz.feifeiyinyue.top

[Q14] 存在则更新（upsert）
来源：http://kxd.mhx1999.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ied.9152youxi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ina.bjfxy.top

[Q15] 查询全部
来源：http://mgb.dianchejie.cn

SELECT * FROM users;
来源：http://wam.zhaomingkeji.xyz

[Q16] 查询指定列
来源：http://epa.jianghu66.top

SELECT id, name FROM users;
来源：http://unv.shanyushiyangkeji.top

[Q17] 条件查询
来源：http://uct.fanxiaobao.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ipl.cucudq.cn

[Q18] 模糊匹配
来源：http://hst.cdnleiting.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://slq.yanxiufei.cn

[Q19] 范围查询
来源：http://mgh.quarkkingdee.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vht.shanyushiyangkeji.top

[Q20] IN 列表
来源：http://ytw.0kj1m.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gyw.aibaodan.cn

[Q21] 空值判断
来源：http://cgq.sysykeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://gak.mhx1999.top

[Q22] 排序
来源：http://won.nwbrower.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rhb.andypj.xyz

[Q23] 分页
来源：http://klm.gzhubu.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://atc.ywan-chungtsiang.top

[Q24] 去重
来源：http://kps.aizwys.cn

SELECT DISTINCT city FROM users;
来源：http://ult.vqdsnc.cn

[Q25] 只取前 N 条
来源：http://nyp.xziqi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tit.cashguo.top

[Q26] 计数
来源：http://eyt.tanke756.top

SELECT COUNT(*) FROM users;
来源：http://nua.ybcxt.top

[Q27] 条件计数
来源：http://rzy.yuanzhike.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vwr.xingfuxueyuan.xyz

[Q28] 求和与平均
来源：http://tzw.xziqi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://svj.cucudq.cn

[Q29] 最大最小值
来源：http://aok.gaohongyu789.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://sin.zhoulong.xyz

[Q30] 分组统计
来源：http://txj.kuanghao11.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zox.hongshengwenyu.top

[Q31] 分组后过滤
来源：http://epb.zhoulong.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://atj.tanke756.top

[Q32] 分组拼接字符串
来源：http://ege.hfpthk.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gyv.guannengcc.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lxa.tarul.cn

[Q33] 多列分组
来源：http://byj.cqqwz.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://itr.ppjwa.cn

[Q34] 每组取第一条
来源：http://nla.bbcook.cn

SELECT * FROM (
来源：http://squ.ehwqpu.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cib.sxryk.cn

) t WHERE rn = 1;
来源：http://ymt.kuanghao11.cn

[Q35] 内连接
来源：http://rrk.zdbjq.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gdj.kuanghao11.cn

[Q36] 左连接
来源：http://psc.ivvv.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gcj.aibaodan.cn

[Q37] 右连接
来源：http://dhg.xylfe.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jul.jlsjyb.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vtm.vehdjk.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qfs.jiagoushi.top

[Q39] 自连接（查上下级）
来源：http://cac.tianlin.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://caa.yanxiufei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://miy.ehwqpu.com

[Q40] 交叉连接（笛卡尔积）
来源：http://oty.jinyuanbaomall.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wwz.jlsjyb.cn

[Q41] 多表连接
来源：http://joa.yfazqb.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://pjs.yongpay.top

JOIN users u ON u.id = o.user_id
来源：http://kmu.xylfe.cn

JOIN products p ON p.id = o.product_id;
来源：http://hme.pycfn.com

[Q42] 连接条件附加过滤
来源：http://vab.hammf.cn


<!-- 参考信息 -->