代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tqi.cdnleiting.top

[N06] 判断回文字符串
来源：http://yvu.chenlongwang.top

Py:   s == s[::-1]
来源：http://nnn.zhijiandao.cn

PHP:  $s === strrev($s);
来源：http://dwy.chenlongwang.top

JS:   s === [...s].reverse().join("")
来源：http://biu.mhx1999.top

TS:   s === [...s].reverse().join("")
来源：http://rha.shanyushiyangtech.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sov.yj20258.top

Go:   // 双指针从两端比较
来源：http://ddv.cqqwz.cn

Ruby: s == s.reverse
来源：http://bdz.nanxinkj.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://szu.yonumen.top

[N07] 两数之和（返回下标）
来源：http://rcu.chenzaomai.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uev.cucudq.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uxh.kuanghao11.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://een.ywan-chungtsiang.top

TS:   // 手写 Map<string, number>
来源：http://nxc.vqdsnc.cn

Java: // 手写 HashMap
来源：http://trm.svipenyu.cn

Go:   // 手写 map[int]int
来源：http://mre.nanxinkj.top

Ruby: // 手写 Hash
来源：http://fzu.tarul.cn

C#:   // 手写 Dictionary<int, int>
来源：http://prx.cdnleiting.top

[N08] 生成全排列
来源：http://hlo.zhongyouzk.top

Py:   itertools.permutations(arr)
来源：http://dna.fzhhl.top

PHP:  // 手写递归交换
来源：http://amr.yongpay.top

JS:   // 手写回溯递归
来源：http://dcu.hnxiangtu.top

TS:   // 手写回溯递归
来源：http://lva.sufxvd.cn

Java: // 手写回溯递归
来源：http://gas.shzxlz.cn

Go:   // 手写回溯递归
来源：http://jcl.hywenlv.cn

Ruby: arr.permutation.to_a
来源：http://dig.hfpthk.cn

C#:   // 手写回溯递归
来源：http://umm.kuanghao11.cn

[N09] 栈与队列
来源：http://mwa.shanyushiyangkeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ehx.gotoacloud.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uvy.havefunace.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mbf.mhx1999.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jrz.52xcode.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bsg.zhengqikj.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ief.zhengqikj.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://aig.epnwcf.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pej.sweek.top

[N10] 链表节点定义
来源：http://kwo.fzhhl.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://auo.nwbrower.top

PHP:  class Node { public $v; public $next = null; }
来源：http://axo.hnqzz.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fzj.feifeiyinyue.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yfg.yuanzhike.top

Java: class Node { int v; Node next; }
来源：http://vcc.jlsjyb.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zfj.smart0.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://klg.yj20258888.top

C#:   class Node { public int V; public Node? Next; }
来源：http://fla.ehwqpu.com

[N11] 二叉树中序遍历
来源：http://sjr.xziqi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ldf.hcnkem.com

PHP:  // 手写递归函数
来源：http://afg.wangdashe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://drz.hnqzz.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cnn.aibaodan.cn

Java: // 手写递归
来源：http://tpo.jiagoushi.top

Go:   // 手写递归
来源：http://mqk.kuanghao11.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qtt.shanyushiyangtech.top

C#:   // 手写递归
来源：http://lhb.fengsongda.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vcu.sxryk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://arn.yueranfly.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wmi.vqdsnc.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fbw.iojbl.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rtg.shanyushiyangkeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dna.yj20258888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zul.hammf.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hji.jinghuilouyu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dph.bjfxy.top

================================================================================
来源：http://huq.tarul.cn

O. 并发与异步
来源：http://rwp.c1oappe.top

================================================================================
来源：http://uoq.jqgfzy.top

[O01] 启动一个线程
来源：http://aov.redwolf501.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wch.fengsongda.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lrf.shangyingyoupin.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gaj.jinyuanbaomall.cn

TS:   // 同 JS
来源：http://phg.316326.xyz

Java: new Thread(() -> f()).start()
来源：http://jqx.chenlongwang.top

Go:   go f()
来源：http://nmo.fzhhl.top

Ruby: Thread.new { f }
来源：http://gyy.hammf.cn

C#:   Task.Run(() => F());
来源：http://bxh.gotoacloud.top

[O02] 使用线程池
来源：http://ber.zhiwuduotai.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jsq.fengsongda.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tfy.hysaishi.cn

JS:   // worker_threads 线程池
来源：http://lei.cqqwz.cn

TS:   // worker_threads 线程池
来源：http://xpu.shanyushiyangtech.top

Java: Executors.newFixedThreadPool(4)
来源：http://btz.haohaochexian.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vos.ydzc1.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ott.zdqjudy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jtz.hcnkem.com

[O03] 加锁保护共享数据
来源：http://lkj.pycfn.com

Py:   with lock: shared += 1
来源：http://srk.dashuyun.cn

PHP:  // 用 flock() 做文件锁
来源：http://kqd.sjlbkw.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iwo.zhaomingkeji.xyz

TS:   // 同 JS
来源：http://dcz.hywenlv.cn

Java: synchronized (this) { shared++; }
来源：http://tps.hongshengwenyu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bvi.pycfn.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://ypw.fehbvm.com

C#:   lock (gate) { shared++; }
来源：http://fpj.xuetiantiany.cn

[O04] 定义异步函数并等待
来源：http://wig.zdqjudy.top

Py:   async def f():⏎    await g()
来源：http://gjm.0kj1m.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ygs.hysaishi.cn

JS:   async function f() { await g(); }
来源：http://wru.wangdashe.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://gbe.9152youxi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zhz.gaohongyu789.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tlk.316326.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://jty.cucudq.cn

C#:   async Task F() { await G(); }
来源：http://ohc.chenzaomai.com

[O05] 并发执行并等待全部完成
来源：http://glk.yangfankeji.com

Py:   asyncio.gather(*tasks)
来源：http://ckz.9152youxi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pzu.0kj1m.cn

JS:   await Promise.all(tasks)
来源：http://ciu.ctjpmb.com

TS:   await Promise.all(tasks)
来源：http://gcy.jinqigufen.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ozk.mhx1999.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pbu.yanxiufei.cn

Ruby: threads.map(&:join)
来源：http://okf.xingfuxueyuan.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://wbu.hongshengwenyu.top

[O06] 使用进程池
来源：http://trk.xinyue.icu

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rmv.52xcode.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jcf.bjfxy.top

JS:   // child_process / cluster 模块
来源：http://zvw.sjlbkw.cn

TS:   // child_process / cluster 模块
来源：http://yld.jqgfzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jrm.jinqigfzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qke.wangshuangyany.cn

Ruby: // fork 块
来源：http://yqi.sysykeji.top

C#:   Parallel.For
来源：http://kkg.yvedp.cn

================================================================================
来源：http://gfy.gzhubu.top

P. 常用工具函数
来源：http://sbx.fktsv.cn

================================================================================
来源：http://ume.hywenlv.cn

[P01] 生成 UUID
来源：http://htz.ydzc1.top

Py:   str(uuid.uuid4())
来源：http://ucg.ctjpmb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tjs.hammf.cn

JS:   crypto.randomUUID()
来源：http://cnm.bbcook.cn

TS:   crypto.randomUUID()
来源：http://dkb.nwbrower.top

Java: UUID.randomUUID().toString()
来源：http://oew.tian-w.cn

Go:   // 用 github.com/google/uuid
来源：http://ecs.316326.xyz

Ruby: SecureRandom.uuid
来源：http://kbg.jyoumei.cn

C#:   Guid.NewGuid().ToString()
来源：http://wdf.jinqigfzy.top

[P02] MD5 / SHA256 摘要
来源：http://lda.bjfxy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ckk.sysykeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://cfv.xziqi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yku.guowangkeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gvb.fanxiaobao.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ofq.zhengqikj.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://odl.zdbjq.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dio.ivvv.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://crb.yangfankeji.com

[P03] 生成短随机字符串
来源：http://hvh.dianchejie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ztz.epnwcf.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fmp.havefunace.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://btu.ehwqpu.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gij.xinyue.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://med.hcnkem.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://afn.feifeiyinyue.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ntr.nwbrower.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vbr.epnwcf.com

[P04] 求长度
来源：http://xkf.cucudq.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kkk.jinghuilouyu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qpw.yuanzhike.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iri.pycfn.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://buz.tanke756.top

Java: list.size();  map.size();  s.length()
来源：http://ldn.gotoacloud.top

Go:   len(arr);  len(m)
来源：http://hgf.gaohongyu789.top

Ruby: x.length;  x.size
来源：http://esj.zhoulong.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://xom.vqdsnc.cn

[P05] 判断两个对象内容是否相等
来源：http://fuw.smart0.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://bmp.zhaomingkeji.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://spc.hesvh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ebx.bjfxy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dpv.fengsongda.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xto.hongshengwenyu.top

Go:   reflect.DeepEqual(a, b)
来源：http://gsm.jinghuilouyu.cn

Ruby: a == b
来源：http://xtu.zhijiandao.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wbn.guannengcc.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tpx.ppjwa.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uei.hcnkem.com

PHP:  if (empty($x)) {}
来源：http://qyx.yj202588.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://paw.jinqigfzy.top

TS:   if (x == null) {}
来源：http://jyo.epnwcf.com

Java: if (x == null || x.isEmpty()) {}
来源：http://atp.smart0.xyz

Go:   if x == nil {}
来源：http://tnt.yvedp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ntc.ctjpmb.com

C#:   if (x is null) {}
来源：http://gsh.kuanghao11.cn

[P07] 防抖与节流
来源：http://qff.sjlbkw.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jlz.sufxvd.cn

PHP:  // 手写时间戳比较
来源：http://ipi.svipenyu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qer.nanxinkj.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pob.chenzaomai.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://egu.ybcxt.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gvz.fanxiaobao.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://jwx.vehdjk.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nlx.dashuyun.cn

[P08] 处理浮点精度问题
来源：http://hfw.zhiwuduotai.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ntw.yj20258.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ojy.xingfuxueyuan.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jop.vqdsnc.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://saj.hnqzz.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fen.hysaishi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cvu.hysaishi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fyw.shuidangran.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rqa.pengpengdd.cyou

================================================================================
来源：http://wdb.xuetiantiany.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mnp.yj20258888.top

================================================================================
来源：http://wej.nanxuanxn.top

[Q01] 创建表
来源：http://fez.yj20258888.top

CREATE TABLE users (
来源：http://ref.zhongyouzk.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ouh.hfpthk.cn

name VARCHAR(50) NOT NULL,
来源：http://ggl.yueranfly.top

email VARCHAR(100) UNIQUE,
来源：http://raf.zhijiandao.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://brh.tanke756.top

);
来源：http://fvx.hnxiangtu.top

[Q02] 创建带外键的表
来源：http://obn.jinghuilouyu.cn

CREATE TABLE orders (
来源：http://dhp.wangdashe.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wwn.chenlongwang.top

user_id INT NOT NULL,
来源：http://xoq.tanke756.top

amount DECIMAL(10, 2),
来源：http://veo.ppjwa.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sjx.guannengcc.top

);
来源：http://ycz.yueranfly.top

[Q03] 增加列
来源：http://wnq.wangdashe.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mji.dianchejie.cn

[Q04] 修改列类型
来源：http://jiu.sxryk.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yir.nwbrower.top

[Q05] 重命名列
来源：http://teu.ehwqpu.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rqk.svipenyu.cn

[Q06] 删除列
来源：http://unl.guannengcc.top

ALTER TABLE users DROP COLUMN age;
来源：http://lkn.chenjidiqi.icu

[Q07] 删除表
来源：http://fby.chenzaomai.com

DROP TABLE IF EXISTS orders;
来源：http://vlf.yueranfly.top

[Q08] 创建普通索引
来源：http://bzp.316326.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://shp.yj20258888.top

[Q09] 创建唯一索引
来源：http://wcc.yj20258.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://igo.quarkkingdee.top

[Q10] 插入单行
来源：http://pya.aizwys.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yms.cdnleiting.top

[Q11] 一次插入多行
来源：http://jxs.meibo888.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://idm.zhoulong.xyz

[Q12] 插入后取自增 ID
来源：http://rnv.havefunace.top

INSERT INTO users (name) VALUES ('C');
来源：http://wsz.aizwys.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zpl.hfpthk.cn

[Q13] 忽略重复插入
来源：http://yge.zhiwuduotai.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vek.yangfankeji.com

[Q14] 存在则更新（upsert）
来源：http://lxl.xziqi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xtu.nanxinkj.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nsi.fehbvm.com

[Q15] 查询全部
来源：http://wys.xylfe.cn

SELECT * FROM users;
来源：http://jzh.guannengcc.top

[Q16] 查询指定列
来源：http://kyt.c1oappe.top

SELECT id, name FROM users;
来源：http://lix.havefunace.top

[Q17] 条件查询
来源：http://grv.yueranfly.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nly.feifeiyinyue.top

[Q18] 模糊匹配
来源：http://hsu.tianlin.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lel.fktsv.cn

[Q19] 范围查询
来源：http://vkk.hesvh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ltm.aibaodan.cn

[Q20] IN 列表
来源：http://yqo.yj202588.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tst.nanxinkj.top

[Q21] 空值判断
来源：http://tzb.vqdsnc.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ygz.yanxiufei.cn

[Q22] 排序
来源：http://yui.jqgfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yjr.nwbrower.top

[Q23] 分页
来源：http://zqu.zycfv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mof.c1oappe.top

[Q24] 去重
来源：http://ava.cashguo.top

SELECT DISTINCT city FROM users;
来源：http://kfv.gzhubu.top

[Q25] 只取前 N 条
来源：http://xvf.gzhubu.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://frk.uphjek.com

[Q26] 计数
来源：http://vrk.shanyushiyangkeji.top

SELECT COUNT(*) FROM users;
来源：http://wov.jqgfzy.top

[Q27] 条件计数
来源：http://thd.ppjwa.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qbw.uphjek.com

[Q28] 求和与平均
来源：http://xsl.zhoulong.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mrs.shanyushiyangtech.top

[Q29] 最大最小值
来源：http://zin.nanxinkj.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://nfg.yj20258.top

[Q30] 分组统计
来源：http://bch.mhx1999.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xrj.daria6918.cn

[Q31] 分组后过滤
来源：http://kwd.pengpengdd.cyou

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xkx.c1oappe.top

[Q32] 分组拼接字符串
来源：http://vkq.fehbvm.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qci.jiagoushi.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fqy.sufxvd.cn

[Q33] 多列分组
来源：http://meq.gogol.net.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://puj.tarul.cn

[Q34] 每组取第一条
来源：http://oiz.birdmap.top

SELECT * FROM (
来源：http://niu.zhaomingkeji.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qfm.uphjek.com

) t WHERE rn = 1;
来源：http://agc.daxiang520.top

[Q35] 内连接
来源：http://ypt.zhixingplan.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vbt.xuanzx.com

[Q36] 左连接
来源：http://oof.pengpengdd.cyou

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://clq.vqdsnc.cn

[Q37] 右连接
来源：http://vbv.cucudq.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pac.aizwys.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gxo.sysykeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vwt.hongshengwenyu.top

[Q39] 自连接（查上下级）
来源：http://lcf.yangfankeji.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://vck.ctjpmb.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wqy.smart0.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://ghl.feifeiyinyue.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fdz.shanyushiyangtech.top

[Q41] 多表连接
来源：http://vdz.ctjpmb.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://nru.jinghuilouyu.cn

JOIN users u ON u.id = o.user_id
来源：http://qnf.ctjpmb.com

JOIN products p ON p.id = o.product_id;
来源：http://gdz.shuidangran.top

[Q42] 连接条件附加过滤
来源：http://vgx.c1oappe.top


<!-- 参考信息 -->