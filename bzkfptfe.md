代发 wailian999

Ruby: s == s.reverse
来源：http://pbu.hongshengwenyu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://fmd.52xcode.cn

[N07] 两数之和（返回下标）
来源：http://plq.pycfn.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bhw.birdmap.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zga.chenlongwang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://sbo.zhengqikj.top

TS:   // 手写 Map<string, number>
来源：http://wih.tarul.cn

Java: // 手写 HashMap
来源：http://wgz.guowangkeji.top

Go:   // 手写 map[int]int
来源：http://jnu.hnqzz.top

Ruby: // 手写 Hash
来源：http://bau.ctjpmb.com

C#:   // 手写 Dictionary<int, int>
来源：http://cho.xylfe.cn

[N08] 生成全排列
来源：http://mkx.yj20258.top

Py:   itertools.permutations(arr)
来源：http://xho.xylfe.cn

PHP:  // 手写递归交换
来源：http://lzv.hnxiangtu.top

JS:   // 手写回溯递归
来源：http://iiu.tarul.cn

TS:   // 手写回溯递归
来源：http://rqf.mhx1999.top

Java: // 手写回溯递归
来源：http://qka.yuxming.cn

Go:   // 手写回溯递归
来源：http://gvz.jqgufenzy.top

Ruby: arr.permutation.to_a
来源：http://wxu.hywenlv.cn

C#:   // 手写回溯递归
来源：http://bfm.svipenyu.cn

[N09] 栈与队列
来源：http://jbt.hammf.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yhq.hysaishi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ogt.bbcook.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ebt.xylfe.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ceb.jqgfzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vrt.cdnleiting.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nvx.gzhubu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vqa.yvedp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://apf.gzhubu.top

[N10] 链表节点定义
来源：http://bxp.shuidangran.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://aiq.zhaomingkeji.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://ubt.bjfxy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://knp.zycfv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blx.ydzc1.top

Java: class Node { int v; Node next; }
来源：http://ytl.gotoacloud.top

Go:   type Node struct { V int; Next *Node }
来源：http://myb.andypj.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://wva.cashguo.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wop.jqgufenzy.top

[N11] 二叉树中序遍历
来源：http://gjv.nanxinkj.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zmc.guowangkeji.top

PHP:  // 手写递归函数
来源：http://ejp.nwbrower.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bar.hfpthk.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eym.shuidangran.top

Java: // 手写递归
来源：http://epv.vqdsnc.cn

Go:   // 手写递归
来源：http://mzi.ppjwa.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ehr.hongshengwenyu.top

C#:   // 手写递归
来源：http://ltk.zhixingplan.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ykg.wangdashe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ngc.gzhubu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fnw.jinyuanbaomall.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aal.aizwys.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tzs.c1oappe.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ujx.fktsv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gsk.ehwqpu.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://aot.zhiwuduotai.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://iye.vqdsnc.cn

================================================================================
来源：http://xqw.xuetiantiany.cn

O. 并发与异步
来源：http://nul.ctjpmb.com

================================================================================
来源：http://pgi.yangfankeji.com

[O01] 启动一个线程
来源：http://szw.daxiang520.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xni.yj20258.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://shz.yueranfly.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jdc.guowangkeji.top

TS:   // 同 JS
来源：http://ppi.daria6918.cn

Java: new Thread(() -> f()).start()
来源：http://qow.xinyue.icu

Go:   go f()
来源：http://ltw.ivvv.top

Ruby: Thread.new { f }
来源：http://yvd.yuanzhike.top

C#:   Task.Run(() => F());
来源：http://vlc.vehdjk.com

[O02] 使用线程池
来源：http://aah.hnqzz.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bii.cucudq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xia.fanxiaobao.xyz

JS:   // worker_threads 线程池
来源：http://pze.svipenyu.cn

TS:   // worker_threads 线程池
来源：http://dfp.ivvv.top

Java: Executors.newFixedThreadPool(4)
来源：http://bck.jinghuilouyu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lmr.hnqzz.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vcw.zdbjq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hgm.ybcxt.top

[O03] 加锁保护共享数据
来源：http://wyj.gaohongyu789.top

Py:   with lock: shared += 1
来源：http://grd.ywan-chungtsiang.top

PHP:  // 用 flock() 做文件锁
来源：http://tub.chenlongwang.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xux.xuanzx.com

TS:   // 同 JS
来源：http://zen.ydzc1.top

Java: synchronized (this) { shared++; }
来源：http://qex.aizwys.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://abr.tian-w.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://nje.vehdjk.com

C#:   lock (gate) { shared++; }
来源：http://lkf.ydzc1.top

[O04] 定义异步函数并等待
来源：http://iqu.jqgfzy.top

Py:   async def f():⏎    await g()
来源：http://uuu.birdmap.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gll.jyoumei.cn

JS:   async function f() { await g(); }
来源：http://feu.snrcjt.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pzz.bbcook.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://iwv.meibo888.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lmn.daria6918.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tvo.iojbl.cn

C#:   async Task F() { await G(); }
来源：http://cir.yanxiufei.cn

[O05] 并发执行并等待全部完成
来源：http://vgo.hnqzz.top

Py:   asyncio.gather(*tasks)
来源：http://zpb.zycfv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jcw.shanyushiyangkeji.top

JS:   await Promise.all(tasks)
来源：http://ioe.wangshuangyany.cn

TS:   await Promise.all(tasks)
来源：http://klj.cqqwz.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qoq.xziqi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kys.xziqi.cn

Ruby: threads.map(&:join)
来源：http://jez.fktsv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wty.cucudq.cn

[O06] 使用进程池
来源：http://gvj.jinyuanbaomall.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jxk.52xcode.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pro.cucudq.cn

JS:   // child_process / cluster 模块
来源：http://ilq.jlsjyb.cn

TS:   // child_process / cluster 模块
来源：http://igm.xuanzx.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://evu.nanxinkj.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mdg.smart0.xyz

Ruby: // fork 块
来源：http://ilo.jqgufenzy.top

C#:   Parallel.For
来源：http://znj.kuanghao11.cn

================================================================================
来源：http://yod.zhoulong.xyz

P. 常用工具函数
来源：http://lya.jinghuilouyu.cn

================================================================================
来源：http://tyn.feifeiyinyue.top

[P01] 生成 UUID
来源：http://csl.yj202588.top

Py:   str(uuid.uuid4())
来源：http://pta.bjfxy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://iax.pycfn.com

JS:   crypto.randomUUID()
来源：http://cvu.shanyushiyangkeji.top

TS:   crypto.randomUUID()
来源：http://bdv.chenzaomai.com

Java: UUID.randomUUID().toString()
来源：http://bqb.shanyushiyangkeji.top

Go:   // 用 github.com/google/uuid
来源：http://kkr.chenjidiqi.icu

Ruby: SecureRandom.uuid
来源：http://jgd.tianlin.xyz

C#:   Guid.NewGuid().ToString()
来源：http://azp.tianlin.xyz

[P02] MD5 / SHA256 摘要
来源：http://keh.jyoumei.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nso.9152youxi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://prb.fzhhl.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nbc.dashuyun.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://umf.ywan-chungtsiang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qie.ydjk.org.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wza.fktsv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ulc.hongshengwenyu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vkw.pycfn.com

[P03] 生成短随机字符串
来源：http://erd.jinqigfzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ynl.yj202588.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://muw.yueranfly.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ask.vehdjk.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://buc.hywenlv.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cze.pengpengdd.cyou

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blf.ydjk.org.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cxf.cashguo.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://itv.yuanzhike.top

[P04] 求长度
来源：http://jpm.zdqjudy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fgk.zhijiandao.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ogp.yuanzhike.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uey.ctjpmb.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nko.sweek.top

Java: list.size();  map.size();  s.length()
来源：http://zsx.yj20258.top

Go:   len(arr);  len(m)
来源：http://nhh.cqqwz.cn

Ruby: x.length;  x.size
来源：http://jek.nanxinkj.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://nav.andypj.xyz

[P05] 判断两个对象内容是否相等
来源：http://qlm.yvedp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ipj.smart0.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xdf.yfazqb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tnk.jyoumei.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wnv.sxryk.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://apm.iojbl.cn

Go:   reflect.DeepEqual(a, b)
来源：http://cmz.tanke756.top

Ruby: a == b
来源：http://qdg.epnwcf.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nvt.zdqjudy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://iol.smart0.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://etq.pycfn.com

PHP:  if (empty($x)) {}
来源：http://lch.wangdashe.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bkf.sjlbkw.cn

TS:   if (x == null) {}
来源：http://qhj.hfpthk.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wqz.zhijiandao.cn

Go:   if x == nil {}
来源：http://guw.sweek.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cqy.yueranfly.top

C#:   if (x is null) {}
来源：http://jjv.cdnleiting.top

[P07] 防抖与节流
来源：http://fri.0kj1m.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xwr.jlsjyb.cn

PHP:  // 手写时间戳比较
来源：http://ngj.yangfankeji.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://naw.fanxiaobao.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hjm.jinghuilouyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://udo.aizwys.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vdv.daria6918.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ngx.svipenyu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ibf.snrcjt.cn

[P08] 处理浮点精度问题
来源：http://dcw.jinqigfzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jkv.dashuyun.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jsl.chenlongwang.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vyp.fktsv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xmy.wangshuangyany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://piu.pengpengdd.cyou

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mzz.hammf.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wvw.shanyushiyangkeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gww.hywenlv.cn

================================================================================
来源：http://gpp.andypj.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xoa.dashuyun.cn

================================================================================
来源：http://pgc.redwolf501.top

[Q01] 创建表
来源：http://dwh.jinyuanbaomall.cn

CREATE TABLE users (
来源：http://mqo.ywan-chungtsiang.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cxw.guannengcc.top

name VARCHAR(50) NOT NULL,
来源：http://rxx.sufxvd.cn

email VARCHAR(100) UNIQUE,
来源：http://hzm.tarul.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lsv.pengpengdd.cyou

);
来源：http://wdn.svipenyu.cn

[Q02] 创建带外键的表
来源：http://ysv.zhaomingkeji.xyz

CREATE TABLE orders (
来源：http://hie.nanxuanxn.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://aff.uphjek.com

user_id INT NOT NULL,
来源：http://gbd.jinghuilouyu.cn

amount DECIMAL(10, 2),
来源：http://omh.zhijiandao.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nep.ybcxt.top

);
来源：http://hjn.ybcxt.top

[Q03] 增加列
来源：http://dhm.yj202588.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pry.shanyushiyangkeji.top

[Q04] 修改列类型
来源：http://rdi.zycfv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uqz.hongshengwenyu.top

[Q05] 重命名列
来源：http://edb.fengsongda.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bea.jinqigfzy.top

[Q06] 删除列
来源：http://cdk.redwolf501.top

ALTER TABLE users DROP COLUMN age;
来源：http://uzt.ppjwa.cn

[Q07] 删除表
来源：http://olv.jianghu66.top

DROP TABLE IF EXISTS orders;
来源：http://lnf.ctjpmb.com

[Q08] 创建普通索引
来源：http://yzj.ydjk.org.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://mxp.9152youxi.cn

[Q09] 创建唯一索引
来源：http://vet.zhengqikj.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gvg.birdmap.top

[Q10] 插入单行
来源：http://jmx.cdnleiting.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wbm.hammf.cn

[Q11] 一次插入多行
来源：http://agx.hcnkem.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sze.tarul.cn

[Q12] 插入后取自增 ID
来源：http://wgi.ctjpmb.com

INSERT INTO users (name) VALUES ('C');
来源：http://exh.sxryk.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nfw.mhx1999.top

[Q13] 忽略重复插入
来源：http://sii.shzxlz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kph.fzhhl.top

[Q14] 存在则更新（upsert）
来源：http://bbt.pycfn.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mcg.jyoumei.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://egf.redwolf501.top

[Q15] 查询全部
来源：http://lxu.hesvh.cn

SELECT * FROM users;
来源：http://qiv.ybcxt.top

[Q16] 查询指定列
来源：http://erq.0kj1m.cn

SELECT id, name FROM users;
来源：http://azi.guannengcc.top

[Q17] 条件查询
来源：http://jhl.yanxiufei.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://niz.kuanghao11.cn

[Q18] 模糊匹配
来源：http://rco.jinqigfzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pbl.ydzc1.top

[Q19] 范围查询
来源：http://zvb.bjfxy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ewv.yuanzhike.top

[Q20] IN 列表
来源：http://kfi.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oej.shanyushiyangtech.top

[Q21] 空值判断
来源：http://ewj.tarul.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://iom.yj202588.top

[Q22] 排序
来源：http://gbs.jinghuilouyu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ygh.zhiwuduotai.top

[Q23] 分页
来源：http://ovm.bbcook.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jre.wangdashe.top

[Q24] 去重
来源：http://oap.birdmap.top

SELECT DISTINCT city FROM users;
来源：http://oia.jinyuanbaomall.cn

[Q25] 只取前 N 条
来源：http://nri.snrcjt.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vpr.tian-w.cn

[Q26] 计数
来源：http://spv.gaohongyu789.top

SELECT COUNT(*) FROM users;
来源：http://lxg.jinghuilouyu.cn

[Q27] 条件计数
来源：http://iut.ywan-chungtsiang.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://heu.sxryk.cn

[Q28] 求和与平均
来源：http://kjf.tian-w.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zyy.hesvh.cn

[Q29] 最大最小值
来源：http://lyh.guowangkeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ldd.gogol.net.cn

[Q30] 分组统计
来源：http://yky.redwolf501.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://orq.chenzaomai.com

[Q31] 分组后过滤
来源：http://yqk.tarul.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jrl.dianchejie.cn

[Q32] 分组拼接字符串
来源：http://utu.ivvv.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://slk.fengsongda.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pln.shanyushiyangkeji.top

[Q33] 多列分组
来源：http://ekx.zhengqikj.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rxe.aibaodan.cn

[Q34] 每组取第一条
来源：http://mts.ywan-chungtsiang.top

SELECT * FROM (
来源：http://hgj.sjlbkw.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://cci.yuanzhike.top

) t WHERE rn = 1;
来源：http://rsw.pengpengdd.cyou

[Q35] 内连接
来源：http://ozq.nanxinkj.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yuz.ctjpmb.com

[Q36] 左连接
来源：http://ncn.yj20258.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://epo.cashguo.top

[Q37] 右连接
来源：http://cwt.c1oappe.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dzc.feifeiyinyue.top

[Q38] 全外连接（PostgreSQL）
来源：http://uez.ivvv.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qwi.wangshuangyany.cn

[Q39] 自连接（查上下级）
来源：http://mco.wangshuangyany.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vbg.chenzaomai.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tlw.nwbrower.top

[Q40] 交叉连接（笛卡尔积）
来源：http://owm.yonumen.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://pdg.shanyushiyangtech.top

[Q41] 多表连接
来源：http://via.guowangkeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://fsd.xuanzx.com

JOIN users u ON u.id = o.user_id
来源：http://sgt.ctjpmb.com

JOIN products p ON p.id = o.product_id;
来源：http://lca.feifeiyinyue.top

[Q42] 连接条件附加过滤
来源：http://wfc.jlsjyb.cn

SELECT u.name, o.amount FROM users u
来源：http://mck.guowangkeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mdv.mhx1999.top

[Q43] 标量子查询
来源：http://sje.jinyuanbaomall.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xgx.fehbvm.com

[Q44] IN 子查询
来源：http://qru.fengsongda.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mkm.yj202588.top

[Q45] EXISTS 判断存在
来源：http://jhn.gzhubu.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uqh.jqgufenzy.top


<!-- 参考信息 -->