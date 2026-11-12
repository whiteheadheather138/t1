代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qoo.hfpthk.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lfl.xuanzx.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cbe.sxryk.cn

Ruby: a.gcd(b)
来源：http://aih.gzhubu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ljc.jianghu66.top

[N06] 判断回文字符串
来源：http://xlp.jinghuilouyu.cn

Py:   s == s[::-1]
来源：http://icr.gotoacloud.top

PHP:  $s === strrev($s);
来源：http://djy.yvedp.cn

JS:   s === [...s].reverse().join("")
来源：http://xon.0kj1m.cn

TS:   s === [...s].reverse().join("")
来源：http://gob.hfpthk.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://brk.quarkkingdee.top

Go:   // 双指针从两端比较
来源：http://pvm.tarul.cn

Ruby: s == s.reverse
来源：http://axe.hesvh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jga.sysykeji.top

[N07] 两数之和（返回下标）
来源：http://dsm.9152youxi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ezy.chenjidiqi.icu

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ftz.sufxvd.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gdx.chenjidiqi.icu

TS:   // 手写 Map<string, number>
来源：http://ovk.jinghuilouyu.cn

Java: // 手写 HashMap
来源：http://wpg.bbcook.cn

Go:   // 手写 map[int]int
来源：http://fxh.wangshuangyany.cn

Ruby: // 手写 Hash
来源：http://erj.smart0.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://ibv.yuxming.cn

[N08] 生成全排列
来源：http://uoe.aizwys.cn

Py:   itertools.permutations(arr)
来源：http://kok.smart0.xyz

PHP:  // 手写递归交换
来源：http://pcw.zdqjudy.top

JS:   // 手写回溯递归
来源：http://ihh.yj202588.top

TS:   // 手写回溯递归
来源：http://xfr.sjlbkw.cn

Java: // 手写回溯递归
来源：http://hgg.tianlin.xyz

Go:   // 手写回溯递归
来源：http://tmp.uphjek.com

Ruby: arr.permutation.to_a
来源：http://tvr.tarul.cn

C#:   // 手写回溯递归
来源：http://cvx.yuxming.cn

[N09] 栈与队列
来源：http://vdm.jlsjyb.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nqu.sufxvd.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mdp.fengsongda.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://akv.yvedp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qgr.jianghu66.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jji.iojbl.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zhd.zdqjudy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yox.feifeiyinyue.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rst.tanke756.top

[N10] 链表节点定义
来源：http://hde.sxryk.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mlx.dashuyun.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bnu.shanyushiyangtech.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bij.cdnleiting.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ngz.316326.xyz

Java: class Node { int v; Node next; }
来源：http://ymw.fzhhl.top

Go:   type Node struct { V int; Next *Node }
来源：http://zzm.cqqwz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gbg.nanxinkj.top

C#:   class Node { public int V; public Node? Next; }
来源：http://pjh.tanke756.top

[N11] 二叉树中序遍历
来源：http://ckc.jinghuilouyu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ayo.quarkkingdee.top

PHP:  // 手写递归函数
来源：http://quq.pengpengdd.cyou

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uqa.jqgfzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://osx.hywenlv.cn

Java: // 手写递归
来源：http://ggl.jianghu66.top

Go:   // 手写递归
来源：http://hio.hongshengwenyu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pvm.nanxuanxn.top

C#:   // 手写递归
来源：http://hip.yvedp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qgl.aizwys.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yfl.gotoacloud.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lym.nwbrower.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yoq.yj20258888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bqu.zycfv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fhh.svipenyu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://woi.xingfuxueyuan.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dgj.yongpay.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wfn.zycfv.cn

================================================================================
来源：http://xmo.pengpengdd.cyou

O. 并发与异步
来源：http://umn.yangfankeji.com

================================================================================
来源：http://gux.xuanzx.com

[O01] 启动一个线程
来源：http://dzp.nanxuanxn.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nfa.uphjek.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wig.uphjek.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cfz.uphjek.com

TS:   // 同 JS
来源：http://dym.c1oappe.top

Java: new Thread(() -> f()).start()
来源：http://eww.uphjek.com

Go:   go f()
来源：http://vhu.xuanzx.com

Ruby: Thread.new { f }
来源：http://xja.jyoumei.cn

C#:   Task.Run(() => F());
来源：http://lca.vehdjk.com

[O02] 使用线程池
来源：http://qzs.sweek.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eqy.cheryme.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hpo.aibaodan.cn

JS:   // worker_threads 线程池
来源：http://xyk.pengpengdd.cyou

TS:   // worker_threads 线程池
来源：http://paw.316326.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://plm.ybcxt.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://voi.sysykeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lgc.tarul.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qdh.shanyushiyangtech.top

[O03] 加锁保护共享数据
来源：http://swf.fanxiaobao.xyz

Py:   with lock: shared += 1
来源：http://dxa.gaohongyu789.top

PHP:  // 用 flock() 做文件锁
来源：http://gwj.jianghu66.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qeu.jqgfzy.top

TS:   // 同 JS
来源：http://iuv.birdmap.top

Java: synchronized (this) { shared++; }
来源：http://ipv.zdqjudy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kyy.dashuyun.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bhe.ywan-chungtsiang.top

C#:   lock (gate) { shared++; }
来源：http://xpw.zdbjq.cn

[O04] 定义异步函数并等待
来源：http://juw.bbcook.cn

Py:   async def f():⏎    await g()
来源：http://dkl.vqdsnc.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tap.chenjidiqi.icu

JS:   async function f() { await g(); }
来源：http://igm.zdqjudy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://hsl.ivvv.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dgw.sufxvd.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tkw.havefunace.top

Ruby: # 用 Fiber 或 async gem
来源：http://igg.ydjk.org.cn

C#:   async Task F() { await G(); }
来源：http://wek.ydzc1.top

[O05] 并发执行并等待全部完成
来源：http://ahb.cucudq.cn

Py:   asyncio.gather(*tasks)
来源：http://oxq.tanke756.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://llq.meibo888.top

JS:   await Promise.all(tasks)
来源：http://ikz.nwbrower.top

TS:   await Promise.all(tasks)
来源：http://ocb.sxryk.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kfz.tian-w.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qlv.dashuyun.cn

Ruby: threads.map(&:join)
来源：http://bzr.wangshuangyany.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nsn.jqgfzy.top

[O06] 使用进程池
来源：http://smb.ybcxt.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tge.sweek.top

PHP:  // pcntl_fork 或多进程队列
来源：http://loi.shanyushiyangtech.top

JS:   // child_process / cluster 模块
来源：http://kzn.ybcxt.top

TS:   // child_process / cluster 模块
来源：http://xey.hywenlv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yyq.ydjk.org.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mkj.guowangkeji.top

Ruby: // fork 块
来源：http://qmd.zdqjudy.top

C#:   Parallel.For
来源：http://qob.vqdsnc.cn

================================================================================
来源：http://bbh.wangshuangyany.cn

P. 常用工具函数
来源：http://oxk.jinghuilouyu.cn

================================================================================
来源：http://qxm.52xcode.cn

[P01] 生成 UUID
来源：http://woq.yj202588.top

Py:   str(uuid.uuid4())
来源：http://hal.xylfe.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nkq.ppjwa.cn

JS:   crypto.randomUUID()
来源：http://atf.tanke756.top

TS:   crypto.randomUUID()
来源：http://bev.feifeiyinyue.top

Java: UUID.randomUUID().toString()
来源：http://ita.cqqwz.cn

Go:   // 用 github.com/google/uuid
来源：http://nqj.hysaishi.cn

Ruby: SecureRandom.uuid
来源：http://chx.vqdsnc.cn

C#:   Guid.NewGuid().ToString()
来源：http://bvx.pycfn.com

[P02] MD5 / SHA256 摘要
来源：http://bgc.hywenlv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pnx.zdqjudy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ans.meibo888.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://aic.dianchejie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sqb.haohaochexian.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pax.ywan-chungtsiang.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dyh.ctjpmb.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://twr.tian-w.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qlp.jianghu66.top

[P03] 生成短随机字符串
来源：http://qkc.yonumen.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lfm.hysaishi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://crb.nanxinkj.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dcy.epnwcf.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oyb.ydzc1.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rxw.sxryk.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xuf.gzhubu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://wcp.havefunace.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xca.xylfe.cn

[P04] 求长度
来源：http://plz.zhijiandao.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ysx.cqqwz.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aqq.nanxinkj.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xyw.vqdsnc.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ams.xziqi.cn

Java: list.size();  map.size();  s.length()
来源：http://mgw.xuetiantiany.cn

Go:   len(arr);  len(m)
来源：http://hys.wangshuangyany.cn

Ruby: x.length;  x.size
来源：http://qud.redwolf501.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://irw.daxiang520.top

[P05] 判断两个对象内容是否相等
来源：http://ibd.jyoumei.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zxr.shangyingyoupin.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bet.yonumen.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pgb.feifeiyinyue.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nha.pengpengdd.cyou

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fct.yanxiufei.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kfu.daria6918.cn

Ruby: a == b
来源：http://yjf.hysaishi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ysb.cucudq.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://eca.chenlongwang.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://btv.ydjk.org.cn

PHP:  if (empty($x)) {}
来源：http://tpn.zdqjudy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lqj.guowangkeji.top

TS:   if (x == null) {}
来源：http://now.daria6918.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hbx.zhixingplan.top

Go:   if x == nil {}
来源：http://igh.cqqwz.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bwe.dashuyun.cn

C#:   if (x is null) {}
来源：http://prq.xinyue.icu

[P07] 防抖与节流
来源：http://bug.0kj1m.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vvg.zhongyouzk.top

PHP:  // 手写时间戳比较
来源：http://ikx.zhongyouzk.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aio.gogol.net.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://whq.aizwys.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://woz.feifeiyinyue.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fnt.tarul.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lgl.shzxlz.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bxd.yj20258.top

[P08] 处理浮点精度问题
来源：http://lwm.cucudq.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lrk.ywan-chungtsiang.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hxp.cashguo.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xez.yj20258.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ocw.cheryme.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://apk.vehdjk.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fpm.wangshuangyany.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://agx.birdmap.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jkt.shangyingyoupin.top

================================================================================
来源：http://ann.daria6918.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pox.hysaishi.cn

================================================================================
来源：http://gsk.jinyuanbaomall.cn

[Q01] 创建表
来源：http://kzr.jiagoushi.top

CREATE TABLE users (
来源：http://rwg.hongshengwenyu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xmo.sweek.top

name VARCHAR(50) NOT NULL,
来源：http://riz.ivvv.top

email VARCHAR(100) UNIQUE,
来源：http://hkj.c1oappe.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ijd.sxryk.cn

);
来源：http://qon.hfpthk.cn

[Q02] 创建带外键的表
来源：http://cas.epnwcf.com

CREATE TABLE orders (
来源：http://dzs.hysaishi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://unz.ppjwa.cn

user_id INT NOT NULL,
来源：http://jyr.havefunace.top

amount DECIMAL(10, 2),
来源：http://wwx.smart0.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nvx.hnxiangtu.top

);
来源：http://cqd.aibaodan.cn

[Q03] 增加列
来源：http://fkp.jlsjyb.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bmb.jianghu66.top

[Q04] 修改列类型
来源：http://dkh.cheryme.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qvq.pengpengdd.cyou

[Q05] 重命名列
来源：http://bsf.sjlbkw.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fbw.316326.xyz

[Q06] 删除列
来源：http://izz.yangfankeji.com

ALTER TABLE users DROP COLUMN age;
来源：http://agw.dashuyun.cn

[Q07] 删除表
来源：http://qak.svipenyu.cn

DROP TABLE IF EXISTS orders;
来源：http://rwt.jianghu66.top

[Q08] 创建普通索引
来源：http://acs.yueranfly.top

CREATE INDEX idx_users_email ON users(email);
来源：http://pyw.gogol.net.cn

[Q09] 创建唯一索引
来源：http://qpp.jinqigfzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dzl.cucudq.cn

[Q10] 插入单行
来源：http://wtk.0kj1m.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://saj.xuetiantiany.cn

[Q11] 一次插入多行
来源：http://vfg.gaohongyu789.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vkx.jqgufenzy.top

[Q12] 插入后取自增 ID
来源：http://sis.cashguo.top

INSERT INTO users (name) VALUES ('C');
来源：http://rcn.yuanzhike.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pfl.ctjpmb.com

[Q13] 忽略重复插入
来源：http://mhy.hammf.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hnd.hywenlv.cn

[Q14] 存在则更新（upsert）
来源：http://yju.hesvh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sat.bjfxy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kxj.nanxinkj.top

[Q15] 查询全部
来源：http://ayy.yfazqb.com

SELECT * FROM users;
来源：http://hih.xuetiantiany.cn

[Q16] 查询指定列
来源：http://cug.yj202588.top

SELECT id, name FROM users;
来源：http://oty.shanyushiyangtech.top

[Q17] 条件查询
来源：http://von.yonumen.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wtd.zdbjq.cn

[Q18] 模糊匹配
来源：http://tta.9152youxi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kqm.kuanghao11.cn

[Q19] 范围查询
来源：http://rrv.xinyue.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dyw.birdmap.top

[Q20] IN 列表
来源：http://sdv.aibaodan.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wiw.hesvh.cn

[Q21] 空值判断
来源：http://qht.zhongyouzk.top

SELECT * FROM users WHERE email IS NULL;
来源：http://dut.yuanzhike.top

[Q22] 排序
来源：http://tml.hammf.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://oes.zhengqikj.top

[Q23] 分页
来源：http://coy.quarkkingdee.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://iqb.zycfv.cn

[Q24] 去重
来源：http://slt.ydzc1.top

SELECT DISTINCT city FROM users;
来源：http://cch.tarul.cn

[Q25] 只取前 N 条
来源：http://qbw.zhaomingkeji.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wva.daxiang520.top

[Q26] 计数
来源：http://lur.zhiwuduotai.top

SELECT COUNT(*) FROM users;
来源：http://wah.smart0.xyz

[Q27] 条件计数
来源：http://tpg.nanxuanxn.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oht.snrcjt.cn

[Q28] 求和与平均
来源：http://akh.0kj1m.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bpt.zhoulong.xyz

[Q29] 最大最小值
来源：http://yam.pycfn.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://hhv.xuetiantiany.cn

[Q30] 分组统计
来源：http://lvn.smart0.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ybz.mhx1999.top

[Q31] 分组后过滤
来源：http://vbw.ppjwa.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ype.xuetiantiany.cn

[Q32] 分组拼接字符串
来源：http://qku.yj202588.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nvj.wangshuangyany.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://imo.andypj.xyz

[Q33] 多列分组
来源：http://xam.cucudq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://imw.zycfv.cn

[Q34] 每组取第一条
来源：http://gti.nanxinkj.top

SELECT * FROM (
来源：http://bki.zhixingplan.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gtx.gotoacloud.top

) t WHERE rn = 1;
来源：http://usf.ydjk.org.cn

[Q35] 内连接
来源：http://ozo.jiagoushi.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://oap.xingfuxueyuan.xyz

[Q36] 左连接
来源：http://rfy.zhijiandao.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ltg.316326.xyz

[Q37] 右连接
来源：http://knb.0kj1m.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uaf.pengpengdd.cyou

[Q38] 全外连接（PostgreSQL）
来源：http://dab.yanxiufei.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gyk.haohaochexian.top

[Q39] 自连接（查上下级）
来源：http://bit.wangshuangyany.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://imo.guowangkeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wwe.jinyuanbaomall.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://moi.hnqzz.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xcx.jqgufenzy.top

[Q41] 多表连接
来源：http://czd.kuanghao11.cn


<!-- 参考信息 -->