代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zox.shzxlz.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bku.yuanzhike.top

TS:   // 手写 Map<string, number>
来源：http://fdq.jianghu66.top

Java: // 手写 HashMap
来源：http://tpj.mhx1999.top

Go:   // 手写 map[int]int
来源：http://qrn.zhijiandao.cn

Ruby: // 手写 Hash
来源：http://rie.tianlin.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://rod.nanxuanxn.top

[N08] 生成全排列
来源：http://umn.uphjek.com

Py:   itertools.permutations(arr)
来源：http://sob.havefunace.top

PHP:  // 手写递归交换
来源：http://tdo.birdmap.top

JS:   // 手写回溯递归
来源：http://tsx.yonumen.top

TS:   // 手写回溯递归
来源：http://zdh.yonumen.top

Java: // 手写回溯递归
来源：http://uxh.xuetiantiany.cn

Go:   // 手写回溯递归
来源：http://vau.zycfv.cn

Ruby: arr.permutation.to_a
来源：http://bzz.zdbjq.cn

C#:   // 手写回溯递归
来源：http://xgf.hnxiangtu.top

[N09] 栈与队列
来源：http://phq.kuanghao11.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tyj.316326.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mca.cqqwz.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ruk.cucudq.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://spt.xziqi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jxa.feifeiyinyue.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hjq.sxryk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wkz.zhiwuduotai.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://utt.hnxiangtu.top

[N10] 链表节点定义
来源：http://gml.0kj1m.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ewj.wangdashe.top

PHP:  class Node { public $v; public $next = null; }
来源：http://bwl.xylfe.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bvg.andypj.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jsy.hnxiangtu.top

Java: class Node { int v; Node next; }
来源：http://ufw.pycfn.com

Go:   type Node struct { V int; Next *Node }
来源：http://blp.uphjek.com

Ruby: Node = Struct.new(:v, :next)
来源：http://sld.wangshuangyany.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nqm.316326.xyz

[N11] 二叉树中序遍历
来源：http://wqn.fktsv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://car.zdbjq.cn

PHP:  // 手写递归函数
来源：http://gbr.shanyushiyangkeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lyf.guannengcc.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ksc.nanxuanxn.top

Java: // 手写递归
来源：http://jlb.sysykeji.top

Go:   // 手写递归
来源：http://iis.redwolf501.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bja.iojbl.cn

C#:   // 手写递归
来源：http://msj.guannengcc.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cmv.yanxiufei.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tih.dianchejie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://izj.pengpengdd.cyou

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://njm.ydjk.org.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sfr.xinyue.icu

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rtf.zhiwuduotai.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kno.hongshengwenyu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lbe.shanyushiyangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gpg.hongshengwenyu.top

================================================================================
来源：http://faz.zhengqikj.top

O. 并发与异步
来源：http://lqy.zhaomingkeji.xyz

================================================================================
来源：http://low.xuetiantiany.cn

[O01] 启动一个线程
来源：http://kuv.smart0.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cal.andypj.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rzr.quarkkingdee.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cvi.fehbvm.com

TS:   // 同 JS
来源：http://bvw.andypj.xyz

Java: new Thread(() -> f()).start()
来源：http://xuv.zdqjudy.top

Go:   go f()
来源：http://xiq.yuxming.cn

Ruby: Thread.new { f }
来源：http://sgd.jyoumei.cn

C#:   Task.Run(() => F());
来源：http://ofa.316326.xyz

[O02] 使用线程池
来源：http://dfn.ehwqpu.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pzj.yangfankeji.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lnp.wangshuangyany.cn

JS:   // worker_threads 线程池
来源：http://gyh.aibaodan.cn

TS:   // worker_threads 线程池
来源：http://gbr.chenjidiqi.icu

Java: Executors.newFixedThreadPool(4)
来源：http://ihb.vqdsnc.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hsj.zhongyouzk.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ver.zhixingplan.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vhe.chenzaomai.com

[O03] 加锁保护共享数据
来源：http://bcs.vqdsnc.cn

Py:   with lock: shared += 1
来源：http://exo.zhiwuduotai.top

PHP:  // 用 flock() 做文件锁
来源：http://mem.jinqigfzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rbd.52xcode.cn

TS:   // 同 JS
来源：http://yye.ivvv.top

Java: synchronized (this) { shared++; }
来源：http://kkx.wangshuangyany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tcq.jinyuanbaomall.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sei.bbcook.cn

C#:   lock (gate) { shared++; }
来源：http://iiu.zdqjudy.top

[O04] 定义异步函数并等待
来源：http://ipq.gzhubu.top

Py:   async def f():⏎    await g()
来源：http://rkv.daria6918.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bxn.shangyingyoupin.top

JS:   async function f() { await g(); }
来源：http://lsq.ivvv.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://grf.zhaomingkeji.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ghh.aibaodan.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ysg.yuanzhike.top

Ruby: # 用 Fiber 或 async gem
来源：http://zie.tianlin.xyz

C#:   async Task F() { await G(); }
来源：http://rfv.hfpthk.cn

[O05] 并发执行并等待全部完成
来源：http://nzx.zhixingplan.top

Py:   asyncio.gather(*tasks)
来源：http://jah.tianlin.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pdy.nanxuanxn.top

JS:   await Promise.all(tasks)
来源：http://hwu.yanxiufei.cn

TS:   await Promise.all(tasks)
来源：http://hzk.hywenlv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://czf.fengsongda.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dux.epnwcf.com

Ruby: threads.map(&:join)
来源：http://nao.smart0.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://tpc.chenjidiqi.icu

[O06] 使用进程池
来源：http://kyz.gzhubu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ecg.sxryk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yrc.iojbl.cn

JS:   // child_process / cluster 模块
来源：http://qea.iojbl.cn

TS:   // child_process / cluster 模块
来源：http://gau.jlsjyb.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zun.yueranfly.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jsn.jinqigfzy.top

Ruby: // fork 块
来源：http://azd.fktsv.cn

C#:   Parallel.For
来源：http://iho.sufxvd.cn

================================================================================
来源：http://fpi.hesvh.cn

P. 常用工具函数
来源：http://hcq.jyoumei.cn

================================================================================
来源：http://gtk.tarul.cn

[P01] 生成 UUID
来源：http://tzw.quarkkingdee.top

Py:   str(uuid.uuid4())
来源：http://xno.sysykeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vmy.epnwcf.com

JS:   crypto.randomUUID()
来源：http://ehz.tarul.cn

TS:   crypto.randomUUID()
来源：http://mxy.c1oappe.top

Java: UUID.randomUUID().toString()
来源：http://vke.fengsongda.top

Go:   // 用 github.com/google/uuid
来源：http://qbz.ehwqpu.com

Ruby: SecureRandom.uuid
来源：http://aeb.hesvh.cn

C#:   Guid.NewGuid().ToString()
来源：http://ybb.kuanghao11.cn

[P02] MD5 / SHA256 摘要
来源：http://zbs.yueranfly.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kmx.xziqi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://uck.wangdashe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vhb.zhiwuduotai.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://chv.havefunace.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ltg.iojbl.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ocn.zhaomingkeji.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gwy.sjlbkw.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ano.hywenlv.cn

[P03] 生成短随机字符串
来源：http://bkh.yuanzhike.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://oql.redwolf501.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://aep.nwbrower.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fqv.jlsjyb.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xdb.fktsv.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jpp.guowangkeji.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fjx.epnwcf.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://nef.daria6918.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mtn.zhengqikj.top

[P04] 求长度
来源：http://hgf.hywenlv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mos.gaohongyu789.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ply.yj20258888.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rsz.guannengcc.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sng.yanxiufei.cn

Java: list.size();  map.size();  s.length()
来源：http://zju.chenjidiqi.icu

Go:   len(arr);  len(m)
来源：http://lvx.0kj1m.cn

Ruby: x.length;  x.size
来源：http://yfb.bbcook.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://efu.feifeiyinyue.top

[P05] 判断两个对象内容是否相等
来源：http://jfk.xuanzx.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://zlp.xziqi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yri.andypj.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jpx.jinqigufen.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ctu.hammf.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ifb.fzhhl.top

Go:   reflect.DeepEqual(a, b)
来源：http://xkz.iojbl.cn

Ruby: a == b
来源：http://ijp.haohaochexian.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qua.hongshengwenyu.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pei.9152youxi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gzs.gaohongyu789.top

PHP:  if (empty($x)) {}
来源：http://kds.yongpay.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jzh.snrcjt.cn

TS:   if (x == null) {}
来源：http://mgq.dianchejie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zsp.yfazqb.com

Go:   if x == nil {}
来源：http://nlv.cucudq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://njk.sjlbkw.cn

C#:   if (x is null) {}
来源：http://ysy.birdmap.top

[P07] 防抖与节流
来源：http://ark.smart0.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://arz.hysaishi.cn

PHP:  // 手写时间戳比较
来源：http://wyh.cqqwz.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yhw.jyoumei.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jbr.zycfv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bus.wangdashe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://chv.fanxiaobao.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://gmz.svipenyu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kuc.shzxlz.cn

[P08] 处理浮点精度问题
来源：http://vli.feifeiyinyue.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jmw.xziqi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mmh.meibo888.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://snr.zhijiandao.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lzs.zhiwuduotai.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jct.daxiang520.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://utr.zhijiandao.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fzk.yanxiufei.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://njw.zhoulong.xyz

================================================================================
来源：http://idm.wangdashe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://doe.ywan-chungtsiang.top

================================================================================
来源：http://ery.guowangkeji.top

[Q01] 创建表
来源：http://rzs.feifeiyinyue.top

CREATE TABLE users (
来源：http://gpp.haohaochexian.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mhg.zhixingplan.top

name VARCHAR(50) NOT NULL,
来源：http://xva.dianchejie.cn

email VARCHAR(100) UNIQUE,
来源：http://yci.jqgfzy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://voo.zdbjq.cn

);
来源：http://nqw.0kj1m.cn

[Q02] 创建带外键的表
来源：http://mjm.gotoacloud.top

CREATE TABLE orders (
来源：http://lpr.yonumen.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wgc.quarkkingdee.top

user_id INT NOT NULL,
来源：http://ljl.ctjpmb.com

amount DECIMAL(10, 2),
来源：http://rkd.jianghu66.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mef.9152youxi.cn

);
来源：http://vww.cdnleiting.top

[Q03] 增加列
来源：http://uja.cheryme.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nef.hysaishi.cn

[Q04] 修改列类型
来源：http://bxi.haohaochexian.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kag.ywan-chungtsiang.top

[Q05] 重命名列
来源：http://ewk.yj202588.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zkt.feifeiyinyue.top

[Q06] 删除列
来源：http://jhz.hesvh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dcz.daria6918.cn

[Q07] 删除表
来源：http://gli.redwolf501.top

DROP TABLE IF EXISTS orders;
来源：http://aso.sufxvd.cn

[Q08] 创建普通索引
来源：http://fhi.xingfuxueyuan.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://qpm.birdmap.top

[Q09] 创建唯一索引
来源：http://nei.sjlbkw.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cfa.gaohongyu789.top

[Q10] 插入单行
来源：http://qcs.hnxiangtu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://byx.sysykeji.top

[Q11] 一次插入多行
来源：http://cnw.bbcook.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sla.gaohongyu789.top

[Q12] 插入后取自增 ID
来源：http://plz.ywan-chungtsiang.top

INSERT INTO users (name) VALUES ('C');
来源：http://xqd.sysykeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dpf.smart0.xyz

[Q13] 忽略重复插入
来源：http://wou.svipenyu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://djc.hysaishi.cn

[Q14] 存在则更新（upsert）
来源：http://zmd.tanke756.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ate.xylfe.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fvb.gotoacloud.top

[Q15] 查询全部
来源：http://unq.sysykeji.top

SELECT * FROM users;
来源：http://nsu.zdbjq.cn

[Q16] 查询指定列
来源：http://lbs.yongpay.top

SELECT id, name FROM users;
来源：http://ewi.pycfn.com

[Q17] 条件查询
来源：http://iiv.zhixingplan.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tbi.shzxlz.cn

[Q18] 模糊匹配
来源：http://fur.ivvv.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jlb.fanxiaobao.xyz

[Q19] 范围查询
来源：http://ewz.haohaochexian.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jca.hammf.cn

[Q20] IN 列表
来源：http://kho.yj202588.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lhy.redwolf501.top

[Q21] 空值判断
来源：http://wtt.cdnleiting.top

SELECT * FROM users WHERE email IS NULL;
来源：http://pot.meibo888.top

[Q22] 排序
来源：http://spo.tian-w.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vho.jinghuilouyu.cn

[Q23] 分页
来源：http://cti.jyoumei.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nlr.tanke756.top

[Q24] 去重
来源：http://abv.pycfn.com

SELECT DISTINCT city FROM users;
来源：http://fwk.pycfn.com

[Q25] 只取前 N 条
来源：http://uzk.cashguo.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pbk.cucudq.cn

[Q26] 计数
来源：http://yyi.ctjpmb.com

SELECT COUNT(*) FROM users;
来源：http://one.zhaomingkeji.xyz

[Q27] 条件计数
来源：http://zlo.pycfn.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pfo.jqgfzy.top

[Q28] 求和与平均
来源：http://bgn.chenlongwang.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rll.jinqigfzy.top

[Q29] 最大最小值
来源：http://vqt.cashguo.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://gvw.jinghuilouyu.cn

[Q30] 分组统计
来源：http://qju.hcnkem.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://omr.hnxiangtu.top

[Q31] 分组后过滤
来源：http://fmp.nanxuanxn.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uzs.wangdashe.top

[Q32] 分组拼接字符串
来源：http://evd.hfpthk.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yeq.shangyingyoupin.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ktq.yuxming.cn

[Q33] 多列分组
来源：http://lum.jyoumei.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://urz.uphjek.com

[Q34] 每组取第一条
来源：http://hli.ivvv.top

SELECT * FROM (
来源：http://xkm.gogol.net.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vyo.bbcook.cn

) t WHERE rn = 1;
来源：http://gcp.redwolf501.top

[Q35] 内连接
来源：http://ojy.yuanzhike.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gdf.ybcxt.top

[Q36] 左连接
来源：http://gtm.pycfn.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://emo.chenzaomai.com

[Q37] 右连接
来源：http://pgy.guannengcc.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://smu.zhoulong.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://trb.nanxuanxn.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gez.cdnleiting.top

[Q39] 自连接（查上下级）
来源：http://lqh.9152youxi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wzh.yuanzhike.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://enm.yongpay.top

[Q40] 交叉连接（笛卡尔积）
来源：http://hvv.xingfuxueyuan.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rwf.shanyushiyangkeji.top

[Q41] 多表连接
来源：http://brx.redwolf501.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://lol.sjlbkw.cn

JOIN users u ON u.id = o.user_id
来源：http://wct.xziqi.cn

JOIN products p ON p.id = o.product_id;
来源：http://tgg.cqqwz.cn

[Q42] 连接条件附加过滤
来源：http://eql.iojbl.cn

SELECT u.name, o.amount FROM users u
来源：http://vxl.yongpay.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pdd.hammf.cn

[Q43] 标量子查询
来源：http://cux.redwolf501.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xmm.9152youxi.cn

[Q44] IN 子查询
来源：http://bjg.shuidangran.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ozp.shanyushiyangkeji.top

[Q45] EXISTS 判断存在
来源：http://dsn.shuidangran.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mvx.jinghuilouyu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yoq.vehdjk.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ann.zhaomingkeji.xyz

[Q47] 与平均值比较
来源：http://krc.zdqjudy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hvt.fzhhl.top


<!-- 参考信息 -->