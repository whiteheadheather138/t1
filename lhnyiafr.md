代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pqy.zhiwuduotai.top

[N06] 判断回文字符串
来源：http://fkt.ivvv.top

Py:   s == s[::-1]
来源：http://irp.aizwys.cn

PHP:  $s === strrev($s);
来源：http://bjv.redwolf501.top

JS:   s === [...s].reverse().join("")
来源：http://gol.xuanzx.com

TS:   s === [...s].reverse().join("")
来源：http://wzd.tarul.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xys.tianlin.xyz

Go:   // 双指针从两端比较
来源：http://gbo.yvedp.cn

Ruby: s == s.reverse
来源：http://gua.jqgfzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://bkn.kuanghao11.cn

[N07] 两数之和（返回下标）
来源：http://sst.zycfv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ufc.xziqi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lao.ehwqpu.com

JS:   // 手写 Map：map.set(v, i)
来源：http://pgp.shuidangran.top

TS:   // 手写 Map<string, number>
来源：http://ynh.fehbvm.com

Java: // 手写 HashMap
来源：http://cte.zhiwuduotai.top

Go:   // 手写 map[int]int
来源：http://cbn.svipenyu.cn

Ruby: // 手写 Hash
来源：http://civ.mhx1999.top

C#:   // 手写 Dictionary<int, int>
来源：http://wue.zhiwuduotai.top

[N08] 生成全排列
来源：http://cbq.sjlbkw.cn

Py:   itertools.permutations(arr)
来源：http://nqf.havefunace.top

PHP:  // 手写递归交换
来源：http://qzq.vqdsnc.cn

JS:   // 手写回溯递归
来源：http://kkb.smart0.xyz

TS:   // 手写回溯递归
来源：http://cuc.sufxvd.cn

Java: // 手写回溯递归
来源：http://dbq.yanxiufei.cn

Go:   // 手写回溯递归
来源：http://kzg.zhengqikj.top

Ruby: arr.permutation.to_a
来源：http://aih.hesvh.cn

C#:   // 手写回溯递归
来源：http://rxo.kuanghao11.cn

[N09] 栈与队列
来源：http://juv.dashuyun.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://efg.fanxiaobao.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://evr.wangshuangyany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zfa.iojbl.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xdh.xziqi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wea.0kj1m.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mln.guannengcc.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wrd.dianchejie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nte.ivvv.top

[N10] 链表节点定义
来源：http://sjp.wangshuangyany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://byf.pengpengdd.cyou

PHP:  class Node { public $v; public $next = null; }
来源：http://qco.daxiang520.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wrv.bbcook.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dok.jinghuilouyu.cn

Java: class Node { int v; Node next; }
来源：http://hbx.aibaodan.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dpb.xuanzx.com

Ruby: Node = Struct.new(:v, :next)
来源：http://icy.jyoumei.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kar.gogol.net.cn

[N11] 二叉树中序遍历
来源：http://sqj.pengpengdd.cyou

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ypm.yj20258888.top

PHP:  // 手写递归函数
来源：http://hju.jqgufenzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lwz.smart0.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mxi.smart0.xyz

Java: // 手写递归
来源：http://gfl.yongpay.top

Go:   // 手写递归
来源：http://pok.yj20258888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fcg.c1oappe.top

C#:   // 手写递归
来源：http://zgb.cucudq.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ykk.hywenlv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hmi.cheryme.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://iuj.jqgfzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sje.dashuyun.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rim.9152youxi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vsv.gzhubu.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dqg.uphjek.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gkw.9152youxi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://egm.epnwcf.com

================================================================================
来源：http://zre.pycfn.com

O. 并发与异步
来源：http://pwl.zhaomingkeji.xyz

================================================================================
来源：http://gte.zhongyouzk.top

[O01] 启动一个线程
来源：http://jus.ydjk.org.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kvu.jianghu66.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rtm.ywan-chungtsiang.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pgu.mhx1999.top

TS:   // 同 JS
来源：http://nvn.ivvv.top

Java: new Thread(() -> f()).start()
来源：http://shc.hesvh.cn

Go:   go f()
来源：http://hod.yvedp.cn

Ruby: Thread.new { f }
来源：http://iyh.aizwys.cn

C#:   Task.Run(() => F());
来源：http://spw.ivvv.top

[O02] 使用线程池
来源：http://zgj.vqdsnc.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jzi.sysykeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uuq.birdmap.top

JS:   // worker_threads 线程池
来源：http://hch.gotoacloud.top

TS:   // worker_threads 线程池
来源：http://drc.hesvh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gjo.aizwys.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://myh.wangshuangyany.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jch.yueranfly.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://typ.feifeiyinyue.top

[O03] 加锁保护共享数据
来源：http://msp.cucudq.cn

Py:   with lock: shared += 1
来源：http://xze.zhijiandao.cn

PHP:  // 用 flock() 做文件锁
来源：http://yww.gogol.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xcd.zdqjudy.top

TS:   // 同 JS
来源：http://mhp.tianlin.xyz

Java: synchronized (this) { shared++; }
来源：http://iot.zhixingplan.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xgg.zhengqikj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://uko.fanxiaobao.xyz

C#:   lock (gate) { shared++; }
来源：http://cgm.ivvv.top

[O04] 定义异步函数并等待
来源：http://akf.quarkkingdee.top

Py:   async def f():⏎    await g()
来源：http://oeg.wangshuangyany.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://iov.316326.xyz

JS:   async function f() { await g(); }
来源：http://tvk.zhijiandao.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ifu.feifeiyinyue.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://stp.ctjpmb.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bou.nwbrower.top

Ruby: # 用 Fiber 或 async gem
来源：http://aut.hnqzz.top

C#:   async Task F() { await G(); }
来源：http://hho.aibaodan.cn

[O05] 并发执行并等待全部完成
来源：http://hvh.fehbvm.com

Py:   asyncio.gather(*tasks)
来源：http://hzz.chenzaomai.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pxy.gaohongyu789.top

JS:   await Promise.all(tasks)
来源：http://wau.guannengcc.top

TS:   await Promise.all(tasks)
来源：http://jrz.yj20258888.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uhh.kuanghao11.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ysz.ivvv.top

Ruby: threads.map(&:join)
来源：http://tnj.yanxiufei.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://teu.yangfankeji.com

[O06] 使用进程池
来源：http://qjm.sxryk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hcx.xinyue.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://pqn.fktsv.cn

JS:   // child_process / cluster 模块
来源：http://vhr.kuanghao11.cn

TS:   // child_process / cluster 模块
来源：http://plw.jiagoushi.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://frn.9152youxi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ica.ydzc1.top

Ruby: // fork 块
来源：http://pzw.hnqzz.top

C#:   Parallel.For
来源：http://yku.9152youxi.cn

================================================================================
来源：http://kpw.zhijiandao.cn

P. 常用工具函数
来源：http://amn.hammf.cn

================================================================================
来源：http://obj.hywenlv.cn

[P01] 生成 UUID
来源：http://hwq.guowangkeji.top

Py:   str(uuid.uuid4())
来源：http://rkg.andypj.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wmu.wangshuangyany.cn

JS:   crypto.randomUUID()
来源：http://ohb.yj20258.top

TS:   crypto.randomUUID()
来源：http://lum.xziqi.cn

Java: UUID.randomUUID().toString()
来源：http://hjv.iojbl.cn

Go:   // 用 github.com/google/uuid
来源：http://var.xingfuxueyuan.xyz

Ruby: SecureRandom.uuid
来源：http://hat.fehbvm.com

C#:   Guid.NewGuid().ToString()
来源：http://gqw.birdmap.top

[P02] MD5 / SHA256 摘要
来源：http://vvg.jqgufenzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zhn.hysaishi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pvk.sjlbkw.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jfb.zdqjudy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mus.feifeiyinyue.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tlo.birdmap.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rxr.smart0.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cqu.bbcook.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ysx.daxiang520.top

[P03] 生成短随机字符串
来源：http://dbt.hnxiangtu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hcq.fanxiaobao.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pat.fanxiaobao.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://crb.shzxlz.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://igp.yuanzhike.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ekf.zhaomingkeji.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vhn.yangfankeji.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://rzo.vehdjk.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://exn.andypj.xyz

[P04] 求长度
来源：http://vng.zhijiandao.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://oah.shuidangran.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ybe.nwbrower.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://psj.jinyuanbaomall.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://abd.shangyingyoupin.top

Java: list.size();  map.size();  s.length()
来源：http://avm.shanyushiyangkeji.top

Go:   len(arr);  len(m)
来源：http://umn.nanxuanxn.top

Ruby: x.length;  x.size
来源：http://xxw.shangyingyoupin.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://tom.xuanzx.com

[P05] 判断两个对象内容是否相等
来源：http://wcg.gzhubu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ais.yanxiufei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sjz.feifeiyinyue.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ykk.mhx1999.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lna.aizwys.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://biy.zhengqikj.top

Go:   reflect.DeepEqual(a, b)
来源：http://nud.zdbjq.cn

Ruby: a == b
来源：http://rst.zhixingplan.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gzp.shzxlz.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yvf.yj20258888.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jbm.feifeiyinyue.top

PHP:  if (empty($x)) {}
来源：http://sqa.zdbjq.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://aox.ehwqpu.com

TS:   if (x == null) {}
来源：http://gsz.hongshengwenyu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wmq.epnwcf.com

Go:   if x == nil {}
来源：http://sda.ydjk.org.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qgv.hammf.cn

C#:   if (x is null) {}
来源：http://wqu.chenzaomai.com

[P07] 防抖与节流
来源：http://nlx.tianlin.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vlw.jinqigfzy.top

PHP:  // 手写时间戳比较
来源：http://hyr.jqgfzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eyn.hesvh.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zng.sufxvd.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vov.ivvv.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fmz.nanxuanxn.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://eom.gaohongyu789.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bva.shzxlz.cn

[P08] 处理浮点精度问题
来源：http://rjc.9152youxi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qnf.chenlongwang.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://byf.hesvh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://spg.zhoulong.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ulv.yuanzhike.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ghg.yonumen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hwn.nwbrower.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ytb.ywan-chungtsiang.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nam.bbcook.cn

================================================================================
来源：http://bvx.ehwqpu.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ukv.chenjidiqi.icu

================================================================================
来源：http://smi.sufxvd.cn

[Q01] 创建表
来源：http://rgh.zhixingplan.top

CREATE TABLE users (
来源：http://jrv.zdqjudy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ggt.uphjek.com

name VARCHAR(50) NOT NULL,
来源：http://oji.birdmap.top

email VARCHAR(100) UNIQUE,
来源：http://rsa.jlsjyb.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wbz.nanxuanxn.top

);
来源：http://suj.sjlbkw.cn

[Q02] 创建带外键的表
来源：http://qiq.cashguo.top

CREATE TABLE orders (
来源：http://fty.cheryme.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kih.yj202588.top

user_id INT NOT NULL,
来源：http://mfn.sxryk.cn

amount DECIMAL(10, 2),
来源：http://zst.daria6918.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ann.pengpengdd.cyou

);
来源：http://ftr.sxryk.cn

[Q03] 增加列
来源：http://cep.9152youxi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sjf.pengpengdd.cyou

[Q04] 修改列类型
来源：http://kms.316326.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://igx.jiagoushi.top

[Q05] 重命名列
来源：http://eyd.ivvv.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mbj.hcnkem.com

[Q06] 删除列
来源：http://rtm.meibo888.top

ALTER TABLE users DROP COLUMN age;
来源：http://wya.zhijiandao.cn

[Q07] 删除表
来源：http://cky.vehdjk.com

DROP TABLE IF EXISTS orders;
来源：http://exe.shangyingyoupin.top

[Q08] 创建普通索引
来源：http://mhh.fzhhl.top

CREATE INDEX idx_users_email ON users(email);
来源：http://khs.hesvh.cn

[Q09] 创建唯一索引
来源：http://ycd.sjlbkw.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ltv.hfpthk.cn

[Q10] 插入单行
来源：http://yob.shuidangran.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://iuy.fehbvm.com

[Q11] 一次插入多行
来源：http://rlf.tianlin.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xcm.yj20258.top

[Q12] 插入后取自增 ID
来源：http://ckz.ctjpmb.com

INSERT INTO users (name) VALUES ('C');
来源：http://zvc.hnxiangtu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sxk.yuanzhike.top

[Q13] 忽略重复插入
来源：http://fpx.cashguo.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oto.ivvv.top

[Q14] 存在则更新（upsert）
来源：http://cvv.yj20258888.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gkb.pycfn.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pgj.nanxinkj.top

[Q15] 查询全部
来源：http://igr.zhaomingkeji.xyz

SELECT * FROM users;
来源：http://nmz.jqgufenzy.top

[Q16] 查询指定列
来源：http://vni.ivvv.top

SELECT id, name FROM users;
来源：http://sqg.jinqigfzy.top

[Q17] 条件查询
来源：http://yxu.quarkkingdee.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wcv.cheryme.top

[Q18] 模糊匹配
来源：http://kka.feifeiyinyue.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rpj.haohaochexian.top

[Q19] 范围查询
来源：http://kwj.316326.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pgd.cqqwz.cn

[Q20] IN 列表
来源：http://olf.shanyushiyangtech.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cis.bbcook.cn

[Q21] 空值判断
来源：http://hzc.tarul.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ecd.nanxuanxn.top

[Q22] 排序
来源：http://bby.yj20258888.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ckn.hnqzz.top

[Q23] 分页
来源：http://qma.yvedp.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dlo.tarul.cn

[Q24] 去重
来源：http://bgv.zdbjq.cn

SELECT DISTINCT city FROM users;
来源：http://lzs.jlsjyb.cn

[Q25] 只取前 N 条
来源：http://kto.cucudq.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://isv.xinyue.icu

[Q26] 计数
来源：http://pwb.yfazqb.com

SELECT COUNT(*) FROM users;
来源：http://yco.shuidangran.top

[Q27] 条件计数
来源：http://xhi.xingfuxueyuan.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gdj.havefunace.top

[Q28] 求和与平均
来源：http://xwb.xinyue.icu

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hpg.xylfe.cn

[Q29] 最大最小值
来源：http://fqi.meibo888.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://rso.aibaodan.cn

[Q30] 分组统计
来源：http://xtl.ybcxt.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gpf.chenzaomai.com

[Q31] 分组后过滤
来源：http://bvt.yj20258888.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gty.ehwqpu.com

[Q32] 分组拼接字符串
来源：http://ukd.quarkkingdee.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qqq.cashguo.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nvj.jinqigfzy.top

[Q33] 多列分组
来源：http://wbo.xinyue.icu

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lug.tarul.cn

[Q34] 每组取第一条
来源：http://mme.vehdjk.com

SELECT * FROM (
来源：http://gks.hcnkem.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gwj.gogol.net.cn

) t WHERE rn = 1;
来源：http://eks.jqgufenzy.top

[Q35] 内连接
来源：http://qfb.shzxlz.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://izw.andypj.xyz

[Q36] 左连接
来源：http://ncd.tanke756.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://izu.ywan-chungtsiang.top

[Q37] 右连接
来源：http://gom.yanxiufei.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jqi.bjfxy.top

[Q38] 全外连接（PostgreSQL）
来源：http://vgi.fzhhl.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jbz.chenjidiqi.icu

[Q39] 自连接（查上下级）
来源：http://nlb.c1oappe.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://zcj.iojbl.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tck.gzhubu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://osu.zdbjq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://voa.9152youxi.cn

[Q41] 多表连接
来源：http://dte.daria6918.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wfj.zhixingplan.top

JOIN users u ON u.id = o.user_id
来源：http://hlm.yuxming.cn

JOIN products p ON p.id = o.product_id;
来源：http://icx.hongshengwenyu.top

[Q42] 连接条件附加过滤
来源：http://pbo.yonumen.top


<!-- 参考信息 -->