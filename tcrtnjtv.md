代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://iis.jinyuanbaomall.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lod.gaohongyu789.top

TS:   // 手写 Map<string, number>
来源：http://hre.jlsjyb.cn

Java: // 手写 HashMap
来源：http://jfs.cdnleiting.top

Go:   // 手写 map[int]int
来源：http://jhs.wangshuangyany.cn

Ruby: // 手写 Hash
来源：http://sdk.cucudq.cn

C#:   // 手写 Dictionary<int, int>
来源：http://suj.wangshuangyany.cn

[N08] 生成全排列
来源：http://jdp.yfazqb.com

Py:   itertools.permutations(arr)
来源：http://gpk.ywan-chungtsiang.top

PHP:  // 手写递归交换
来源：http://lue.aibaodan.cn

JS:   // 手写回溯递归
来源：http://exw.iojbl.cn

TS:   // 手写回溯递归
来源：http://mlw.yvedp.cn

Java: // 手写回溯递归
来源：http://vrq.c1oappe.top

Go:   // 手写回溯递归
来源：http://tnr.vehdjk.com

Ruby: arr.permutation.to_a
来源：http://unr.shuidangran.top

C#:   // 手写回溯递归
来源：http://wou.yangfankeji.com

[N09] 栈与队列
来源：http://snh.zhiwuduotai.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dau.hcnkem.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kmn.jyoumei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bkg.vehdjk.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yap.zhaomingkeji.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zte.hnqzz.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ikc.daria6918.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://utr.epnwcf.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://plu.ybcxt.top

[N10] 链表节点定义
来源：http://kzq.iojbl.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rmh.hnxiangtu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://une.jinqigfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fal.jiagoushi.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vjx.ywan-chungtsiang.top

Java: class Node { int v; Node next; }
来源：http://uos.guowangkeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://zyj.cqqwz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vyk.yfazqb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://wnl.9152youxi.cn

[N11] 二叉树中序遍历
来源：http://ueb.wangshuangyany.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ala.snrcjt.cn

PHP:  // 手写递归函数
来源：http://gnn.ctjpmb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oyl.guannengcc.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fou.snrcjt.cn

Java: // 手写递归
来源：http://mhl.yuxming.cn

Go:   // 手写递归
来源：http://dhg.zhijiandao.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mox.nanxuanxn.top

C#:   // 手写递归
来源：http://vvq.mhx1999.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sjx.daxiang520.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://prc.jianghu66.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://aod.zhixingplan.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gut.feifeiyinyue.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fap.jianghu66.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cot.jqgfzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sju.shanyushiyangkeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://srf.zdbjq.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xub.meibo888.top

================================================================================
来源：http://dfx.guannengcc.top

O. 并发与异步
来源：http://iyx.nanxuanxn.top

================================================================================
来源：http://pra.dashuyun.cn

[O01] 启动一个线程
来源：http://aaz.xuanzx.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tde.andypj.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nlr.yonumen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tnd.mhx1999.top

TS:   // 同 JS
来源：http://lfb.hysaishi.cn

Java: new Thread(() -> f()).start()
来源：http://mfn.chenjidiqi.icu

Go:   go f()
来源：http://ckh.chenjidiqi.icu

Ruby: Thread.new { f }
来源：http://fpm.yj20258888.top

C#:   Task.Run(() => F());
来源：http://ilg.bjfxy.top

[O02] 使用线程池
来源：http://kkk.ctjpmb.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ayc.yanxiufei.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gfh.hnxiangtu.top

JS:   // worker_threads 线程池
来源：http://wur.sweek.top

TS:   // worker_threads 线程池
来源：http://dyo.bjfxy.top

Java: Executors.newFixedThreadPool(4)
来源：http://ror.jyoumei.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yob.xylfe.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uqp.jiagoushi.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oyh.kuanghao11.cn

[O03] 加锁保护共享数据
来源：http://ppz.fktsv.cn

Py:   with lock: shared += 1
来源：http://ncb.daxiang520.top

PHP:  // 用 flock() 做文件锁
来源：http://oea.aizwys.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vhy.havefunace.top

TS:   // 同 JS
来源：http://pzt.zdbjq.cn

Java: synchronized (this) { shared++; }
来源：http://nzf.xuetiantiany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://abu.316326.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://wtv.cqqwz.cn

C#:   lock (gate) { shared++; }
来源：http://sfu.jinqigufen.top

[O04] 定义异步函数并等待
来源：http://qgf.tarul.cn

Py:   async def f():⏎    await g()
来源：http://svp.chenzaomai.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tqb.zhengqikj.top

JS:   async function f() { await g(); }
来源：http://rgh.zycfv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dwv.chenjidiqi.icu

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cut.daria6918.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://obx.sweek.top

Ruby: # 用 Fiber 或 async gem
来源：http://rcv.sweek.top

C#:   async Task F() { await G(); }
来源：http://hvc.jinyuanbaomall.cn

[O05] 并发执行并等待全部完成
来源：http://dhn.havefunace.top

Py:   asyncio.gather(*tasks)
来源：http://vgj.cdnleiting.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wll.fengsongda.top

JS:   await Promise.all(tasks)
来源：http://wkc.xuanzx.com

TS:   await Promise.all(tasks)
来源：http://bwl.kuanghao11.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://clo.andypj.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dsj.tarul.cn

Ruby: threads.map(&:join)
来源：http://mfa.guannengcc.top

C#:   await Task.WhenAll(t1, t2)
来源：http://evb.xylfe.cn

[O06] 使用进程池
来源：http://wdj.havefunace.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ptv.52xcode.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://div.9152youxi.cn

JS:   // child_process / cluster 模块
来源：http://yhh.snrcjt.cn

TS:   // child_process / cluster 模块
来源：http://vbx.hnqzz.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lpj.chenzaomai.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xhp.bjfxy.top

Ruby: // fork 块
来源：http://ype.tanke756.top

C#:   Parallel.For
来源：http://ahg.zycfv.cn

================================================================================
来源：http://uwt.tianlin.xyz

P. 常用工具函数
来源：http://vhw.gotoacloud.top

================================================================================
来源：http://pre.jinqigfzy.top

[P01] 生成 UUID
来源：http://bmf.9152youxi.cn

Py:   str(uuid.uuid4())
来源：http://nfr.zhaomingkeji.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ibv.pengpengdd.cyou

JS:   crypto.randomUUID()
来源：http://upq.zycfv.cn

TS:   crypto.randomUUID()
来源：http://pqg.xinyue.icu

Java: UUID.randomUUID().toString()
来源：http://xnj.fengsongda.top

Go:   // 用 github.com/google/uuid
来源：http://ceu.chenlongwang.top

Ruby: SecureRandom.uuid
来源：http://tbc.meibo888.top

C#:   Guid.NewGuid().ToString()
来源：http://juc.aizwys.cn

[P02] MD5 / SHA256 摘要
来源：http://dcn.shanyushiyangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://afr.pycfn.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://ehr.tanke756.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qbr.sjlbkw.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dqa.xylfe.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qqy.chenjidiqi.icu

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gct.hysaishi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ztz.yj20258.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://had.jianghu66.top

[P03] 生成短随机字符串
来源：http://dmx.zhoulong.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rtv.vehdjk.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ucu.wangshuangyany.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nxi.dianchejie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vdt.sweek.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://elr.ivvv.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vfk.zdqjudy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://pdh.pycfn.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://frl.zhongyouzk.top

[P04] 求长度
来源：http://pxv.snrcjt.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ijt.guowangkeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zih.gzhubu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rir.tianlin.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xdn.jinghuilouyu.cn

Java: list.size();  map.size();  s.length()
来源：http://nio.zhongyouzk.top

Go:   len(arr);  len(m)
来源：http://fhf.ppjwa.cn

Ruby: x.length;  x.size
来源：http://gcy.bbcook.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lwh.zycfv.cn

[P05] 判断两个对象内容是否相等
来源：http://oqc.cdnleiting.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://fhn.jinyuanbaomall.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://enj.hfpthk.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://khm.cucudq.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lrl.yangfankeji.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yct.aizwys.cn

Go:   reflect.DeepEqual(a, b)
来源：http://otj.iojbl.cn

Ruby: a == b
来源：http://jjj.hnxiangtu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hcc.yuanzhike.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://oti.fanxiaobao.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://epa.pycfn.com

PHP:  if (empty($x)) {}
来源：http://kxv.ywan-chungtsiang.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fig.meibo888.top

TS:   if (x == null) {}
来源：http://nyf.shanyushiyangtech.top

Java: if (x == null || x.isEmpty()) {}
来源：http://sep.daxiang520.top

Go:   if x == nil {}
来源：http://kgy.feifeiyinyue.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cup.nwbrower.top

C#:   if (x is null) {}
来源：http://lwi.zhixingplan.top

[P07] 防抖与节流
来源：http://hht.gzhubu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://idu.zhoulong.xyz

PHP:  // 手写时间戳比较
来源：http://imr.cdnleiting.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://njv.nanxuanxn.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pvx.xuetiantiany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nix.snrcjt.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ark.zhijiandao.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://psx.mhx1999.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sdw.nanxinkj.top

[P08] 处理浮点精度问题
来源：http://qgj.gaohongyu789.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mix.chenzaomai.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zvo.gotoacloud.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cft.hammf.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pby.yongpay.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qfc.hysaishi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://une.xziqi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vqk.zycfv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sdw.yangfankeji.com

================================================================================
来源：http://sxi.c1oappe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yhy.zycfv.cn

================================================================================
来源：http://dxm.jlsjyb.cn

[Q01] 创建表
来源：http://zll.52xcode.cn

CREATE TABLE users (
来源：http://lev.jinghuilouyu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fpf.chenzaomai.com

name VARCHAR(50) NOT NULL,
来源：http://xlt.dashuyun.cn

email VARCHAR(100) UNIQUE,
来源：http://olj.jyoumei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tdy.ybcxt.top

);
来源：http://olc.zhongyouzk.top

[Q02] 创建带外键的表
来源：http://flo.52xcode.cn

CREATE TABLE orders (
来源：http://qcb.xylfe.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zlu.shuidangran.top

user_id INT NOT NULL,
来源：http://wtu.feifeiyinyue.top

amount DECIMAL(10, 2),
来源：http://mry.aizwys.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sio.hywenlv.cn

);
来源：http://mdk.hysaishi.cn

[Q03] 增加列
来源：http://ynj.birdmap.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fxy.kuanghao11.cn

[Q04] 修改列类型
来源：http://wdp.tianlin.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nca.yj20258.top

[Q05] 重命名列
来源：http://mco.bbcook.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fkk.jqgfzy.top

[Q06] 删除列
来源：http://akv.jianghu66.top

ALTER TABLE users DROP COLUMN age;
来源：http://kvb.epnwcf.com

[Q07] 删除表
来源：http://epe.aizwys.cn

DROP TABLE IF EXISTS orders;
来源：http://ulx.jlsjyb.cn

[Q08] 创建普通索引
来源：http://ndc.cqqwz.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://asx.andypj.xyz

[Q09] 创建唯一索引
来源：http://obk.ivvv.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qnf.ehwqpu.com

[Q10] 插入单行
来源：http://ykj.zdqjudy.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yly.jiagoushi.top

[Q11] 一次插入多行
来源：http://idn.andypj.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uwd.hammf.cn

[Q12] 插入后取自增 ID
来源：http://uyf.yongpay.top

INSERT INTO users (name) VALUES ('C');
来源：http://ffo.tanke756.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tcb.zdbjq.cn

[Q13] 忽略重复插入
来源：http://kno.xingfuxueyuan.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cwr.zdqjudy.top

[Q14] 存在则更新（upsert）
来源：http://cyk.nanxuanxn.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bes.bbcook.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ddu.havefunace.top

[Q15] 查询全部
来源：http://ukp.hesvh.cn

SELECT * FROM users;
来源：http://ira.xinyue.icu

[Q16] 查询指定列
来源：http://fjo.vehdjk.com

SELECT id, name FROM users;
来源：http://azp.bbcook.cn

[Q17] 条件查询
来源：http://gio.zdqjudy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cmw.zhijiandao.cn

[Q18] 模糊匹配
来源：http://gko.yueranfly.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://phf.sweek.top

[Q19] 范围查询
来源：http://fhd.andypj.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cix.yonumen.top

[Q20] IN 列表
来源：http://zvw.chenzaomai.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rta.xuanzx.com

[Q21] 空值判断
来源：http://cqc.yangfankeji.com

SELECT * FROM users WHERE email IS NULL;
来源：http://oik.hcnkem.com

[Q22] 排序
来源：http://nbk.zhengqikj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dxi.sufxvd.cn

[Q23] 分页
来源：http://egr.ydzc1.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hzr.tian-w.cn

[Q24] 去重
来源：http://svi.jinyuanbaomall.cn

SELECT DISTINCT city FROM users;
来源：http://fdl.jianghu66.top

[Q25] 只取前 N 条
来源：http://yii.yueranfly.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ovx.tian-w.cn

[Q26] 计数
来源：http://bce.aizwys.cn

SELECT COUNT(*) FROM users;
来源：http://wyn.tanke756.top

[Q27] 条件计数
来源：http://hqr.guannengcc.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nmp.mhx1999.top

[Q28] 求和与平均
来源：http://scy.jianghu66.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oud.vqdsnc.cn

[Q29] 最大最小值
来源：http://srh.birdmap.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://vyd.cucudq.cn

[Q30] 分组统计
来源：http://uaw.haohaochexian.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vxq.dashuyun.cn

[Q31] 分组后过滤
来源：http://sae.bbcook.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nok.gogol.net.cn

[Q32] 分组拼接字符串
来源：http://ieq.chenlongwang.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pdz.tian-w.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ypu.sufxvd.cn

[Q33] 多列分组
来源：http://erj.cheryme.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vdv.tianlin.xyz

[Q34] 每组取第一条
来源：http://znb.sjlbkw.cn

SELECT * FROM (
来源：http://gpz.xziqi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qnq.fengsongda.top

) t WHERE rn = 1;
来源：http://uxl.tian-w.cn

[Q35] 内连接
来源：http://tob.daria6918.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rcu.hammf.cn

[Q36] 左连接
来源：http://prq.bjfxy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://grn.jiagoushi.top

[Q37] 右连接
来源：http://ofn.gotoacloud.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rom.meibo888.top

[Q38] 全外连接（PostgreSQL）
来源：http://yob.hfpthk.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ukz.fanxiaobao.xyz

[Q39] 自连接（查上下级）
来源：http://eso.ctjpmb.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://dju.hongshengwenyu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wus.aibaodan.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mpx.nanxuanxn.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xnf.fanxiaobao.xyz

[Q41] 多表连接
来源：http://pte.gogol.net.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://wlr.shzxlz.cn

JOIN users u ON u.id = o.user_id
来源：http://qhz.zhiwuduotai.top

JOIN products p ON p.id = o.product_id;
来源：http://kca.aibaodan.cn

[Q42] 连接条件附加过滤
来源：http://tef.hesvh.cn

SELECT u.name, o.amount FROM users u
来源：http://lsx.cheryme.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vbi.vehdjk.com

[Q43] 标量子查询
来源：http://icb.chenjidiqi.icu

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hhy.zdbjq.cn

[Q44] IN 子查询
来源：http://nbo.jiagoushi.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nsm.ppjwa.cn

[Q45] EXISTS 判断存在
来源：http://the.guannengcc.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gck.zdqjudy.top

[Q46] NOT EXISTS 判断不存在
来源：http://lbk.cashguo.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wck.nanxinkj.top

[Q47] 与平均值比较
来源：http://oul.dashuyun.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ewd.xuanzx.com


<!-- 参考信息 -->