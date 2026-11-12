代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sau.zhixingplan.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qmr.hcnkem.com

TS:   // 手写 Map<string, number>
来源：http://ppw.shanyushiyangkeji.top

Java: // 手写 HashMap
来源：http://zdq.smart0.xyz

Go:   // 手写 map[int]int
来源：http://ikd.yangfankeji.com

Ruby: // 手写 Hash
来源：http://tfh.sysykeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://fww.jinqigfzy.top

[N08] 生成全排列
来源：http://rfo.gaohongyu789.top

Py:   itertools.permutations(arr)
来源：http://rzn.gaohongyu789.top

PHP:  // 手写递归交换
来源：http://cew.daria6918.cn

JS:   // 手写回溯递归
来源：http://ncg.ppjwa.cn

TS:   // 手写回溯递归
来源：http://xzv.xingfuxueyuan.xyz

Java: // 手写回溯递归
来源：http://dpc.jianghu66.top

Go:   // 手写回溯递归
来源：http://scf.yonumen.top

Ruby: arr.permutation.to_a
来源：http://rhx.mhx1999.top

C#:   // 手写回溯递归
来源：http://vwv.cashguo.top

[N09] 栈与队列
来源：http://hxo.pycfn.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pgm.guowangkeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ruh.hesvh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qpa.shzxlz.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://udf.nanxuanxn.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hjn.xinyue.icu

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://smd.yonumen.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xwr.zhaomingkeji.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ipa.zhixingplan.top

[N10] 链表节点定义
来源：http://xtz.jlsjyb.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fxw.haohaochexian.top

PHP:  class Node { public $v; public $next = null; }
来源：http://gxj.bjfxy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://glb.ywan-chungtsiang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xbj.sweek.top

Java: class Node { int v; Node next; }
来源：http://qzp.ydjk.org.cn

Go:   type Node struct { V int; Next *Node }
来源：http://eiu.guannengcc.top

Ruby: Node = Struct.new(:v, :next)
来源：http://fuf.cheryme.top

C#:   class Node { public int V; public Node? Next; }
来源：http://zhy.hcnkem.com

[N11] 二叉树中序遍历
来源：http://leh.xingfuxueyuan.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wjw.gaohongyu789.top

PHP:  // 手写递归函数
来源：http://lsf.snrcjt.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jsg.cheryme.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ivo.9152youxi.cn

Java: // 手写递归
来源：http://ocu.gogol.net.cn

Go:   // 手写递归
来源：http://ihq.kuanghao11.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hlb.pengpengdd.cyou

C#:   // 手写递归
来源：http://ycf.zhongyouzk.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cbp.tian-w.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fct.hnxiangtu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ced.52xcode.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uiv.pycfn.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uef.tian-w.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xxg.hywenlv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://isw.sufxvd.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wsv.cdnleiting.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gtb.feifeiyinyue.top

================================================================================
来源：http://yox.vehdjk.com

O. 并发与异步
来源：http://pnx.feifeiyinyue.top

================================================================================
来源：http://niy.daxiang520.top

[O01] 启动一个线程
来源：http://sro.tarul.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bzj.andypj.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pub.jinqigfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bmm.shuidangran.top

TS:   // 同 JS
来源：http://onj.jlsjyb.cn

Java: new Thread(() -> f()).start()
来源：http://shn.52xcode.cn

Go:   go f()
来源：http://vkt.jlsjyb.cn

Ruby: Thread.new { f }
来源：http://rmb.9152youxi.cn

C#:   Task.Run(() => F());
来源：http://fsp.snrcjt.cn

[O02] 使用线程池
来源：http://lso.vehdjk.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nve.fengsongda.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uyx.cqqwz.cn

JS:   // worker_threads 线程池
来源：http://hcz.sxryk.cn

TS:   // worker_threads 线程池
来源：http://ceb.zdbjq.cn

Java: Executors.newFixedThreadPool(4)
来源：http://peo.hnxiangtu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vtq.zhongyouzk.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ukq.havefunace.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hje.meibo888.top

[O03] 加锁保护共享数据
来源：http://kto.vehdjk.com

Py:   with lock: shared += 1
来源：http://cco.hcnkem.com

PHP:  // 用 flock() 做文件锁
来源：http://yjc.quarkkingdee.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cqr.cheryme.top

TS:   // 同 JS
来源：http://spw.jinqigfzy.top

Java: synchronized (this) { shared++; }
来源：http://ufq.ivvv.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://voi.meibo888.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://rwr.ybcxt.top

C#:   lock (gate) { shared++; }
来源：http://fos.smart0.xyz

[O04] 定义异步函数并等待
来源：http://peu.hfpthk.cn

Py:   async def f():⏎    await g()
来源：http://zsu.yj202588.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xjc.ywan-chungtsiang.top

JS:   async function f() { await g(); }
来源：http://mxc.shuidangran.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://uwi.daxiang520.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ebx.ybcxt.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ogj.zycfv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tjp.jinqigfzy.top

C#:   async Task F() { await G(); }
来源：http://wmm.yfazqb.com

[O05] 并发执行并等待全部完成
来源：http://zlk.bbcook.cn

Py:   asyncio.gather(*tasks)
来源：http://uxq.havefunace.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jgh.iojbl.cn

JS:   await Promise.all(tasks)
来源：http://uas.guowangkeji.top

TS:   await Promise.all(tasks)
来源：http://lvz.0kj1m.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dcj.tanke756.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bif.smart0.xyz

Ruby: threads.map(&:join)
来源：http://fcx.havefunace.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xje.zdqjudy.top

[O06] 使用进程池
来源：http://jih.cucudq.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://non.yj20258.top

PHP:  // pcntl_fork 或多进程队列
来源：http://tqw.meibo888.top

JS:   // child_process / cluster 模块
来源：http://mat.zhongyouzk.top

TS:   // child_process / cluster 模块
来源：http://zbv.tanke756.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lmz.guannengcc.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ebs.jianghu66.top

Ruby: // fork 块
来源：http://nqo.gotoacloud.top

C#:   Parallel.For
来源：http://rxd.fanxiaobao.xyz

================================================================================
来源：http://hxi.haohaochexian.top

P. 常用工具函数
来源：http://hhu.jinyuanbaomall.cn

================================================================================
来源：http://ejz.epnwcf.com

[P01] 生成 UUID
来源：http://wok.dashuyun.cn

Py:   str(uuid.uuid4())
来源：http://mqy.guannengcc.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nwf.jinqigufen.top

JS:   crypto.randomUUID()
来源：http://fso.epnwcf.com

TS:   crypto.randomUUID()
来源：http://atk.sxryk.cn

Java: UUID.randomUUID().toString()
来源：http://kfq.sweek.top

Go:   // 用 github.com/google/uuid
来源：http://fuz.xingfuxueyuan.xyz

Ruby: SecureRandom.uuid
来源：http://xtm.xuanzx.com

C#:   Guid.NewGuid().ToString()
来源：http://xqo.cashguo.top

[P02] MD5 / SHA256 摘要
来源：http://qzs.yj20258.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gfd.xuetiantiany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lxb.yuanzhike.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hof.jinqigfzy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tew.sysykeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bjz.sufxvd.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wxv.xuanzx.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bkd.zhixingplan.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zje.yuxming.cn

[P03] 生成短随机字符串
来源：http://ayy.jinghuilouyu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://grz.jqgufenzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xbd.jyoumei.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qwz.zycfv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rgj.hongshengwenyu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ntr.sweek.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sqf.shuidangran.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://niv.fengsongda.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ela.c1oappe.top

[P04] 求长度
来源：http://yjb.nanxuanxn.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wav.hesvh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ovb.yj202588.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://whi.daxiang520.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wie.daria6918.cn

Java: list.size();  map.size();  s.length()
来源：http://ypp.vehdjk.com

Go:   len(arr);  len(m)
来源：http://ewd.yanxiufei.cn

Ruby: x.length;  x.size
来源：http://sdc.shzxlz.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ejf.cqqwz.cn

[P05] 判断两个对象内容是否相等
来源：http://nve.jinqigufen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://qgb.zdqjudy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://awv.hnqzz.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dke.snrcjt.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tch.iojbl.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ygx.sysykeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://yhw.ywan-chungtsiang.top

Ruby: a == b
来源：http://rzo.daria6918.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zub.yanxiufei.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bji.fanxiaobao.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lot.zhijiandao.cn

PHP:  if (empty($x)) {}
来源：http://rlq.sjlbkw.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://phg.daxiang520.top

TS:   if (x == null) {}
来源：http://zfp.hcnkem.com

Java: if (x == null || x.isEmpty()) {}
来源：http://twv.vqdsnc.cn

Go:   if x == nil {}
来源：http://zkg.tian-w.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xep.tian-w.cn

C#:   if (x is null) {}
来源：http://yyo.sweek.top

[P07] 防抖与节流
来源：http://nsr.sxryk.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dit.nanxuanxn.top

PHP:  // 手写时间戳比较
来源：http://nmo.sjlbkw.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://prh.yonumen.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wsa.tarul.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nez.ydjk.org.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bef.jinqigufen.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://vsc.zhijiandao.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zhc.sjlbkw.cn

[P08] 处理浮点精度问题
来源：http://mqn.zhongyouzk.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://klz.gaohongyu789.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ofc.andypj.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xld.birdmap.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://iyw.xinyue.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xax.ywan-chungtsiang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://plw.nanxinkj.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mqk.wangdashe.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qon.zhijiandao.cn

================================================================================
来源：http://rzm.hywenlv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ojc.ppjwa.cn

================================================================================
来源：http://emm.jyoumei.cn

[Q01] 创建表
来源：http://tpf.xylfe.cn

CREATE TABLE users (
来源：http://wmj.cdnleiting.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://eha.hammf.cn

name VARCHAR(50) NOT NULL,
来源：http://vuf.andypj.xyz

email VARCHAR(100) UNIQUE,
来源：http://uuk.sjlbkw.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mbr.fehbvm.com

);
来源：http://aoi.tianlin.xyz

[Q02] 创建带外键的表
来源：http://jfj.sweek.top

CREATE TABLE orders (
来源：http://gun.vehdjk.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lwl.zhiwuduotai.top

user_id INT NOT NULL,
来源：http://fjb.hcnkem.com

amount DECIMAL(10, 2),
来源：http://uzi.wangshuangyany.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ijb.yonumen.top

);
来源：http://hny.c1oappe.top

[Q03] 增加列
来源：http://kuw.zhixingplan.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://okz.vehdjk.com

[Q04] 修改列类型
来源：http://sqj.cheryme.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wyd.tianlin.xyz

[Q05] 重命名列
来源：http://cqj.yonumen.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mjr.cashguo.top

[Q06] 删除列
来源：http://urs.vqdsnc.cn

ALTER TABLE users DROP COLUMN age;
来源：http://diq.tianlin.xyz

[Q07] 删除表
来源：http://eql.snrcjt.cn

DROP TABLE IF EXISTS orders;
来源：http://cxs.0kj1m.cn

[Q08] 创建普通索引
来源：http://jsc.hysaishi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wxt.jyoumei.cn

[Q09] 创建唯一索引
来源：http://mgh.shangyingyoupin.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gwu.aibaodan.cn

[Q10] 插入单行
来源：http://spx.yvedp.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kwe.zhiwuduotai.top

[Q11] 一次插入多行
来源：http://zqu.jianghu66.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://otq.jinyuanbaomall.cn

[Q12] 插入后取自增 ID
来源：http://kai.tian-w.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yww.yonumen.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://occ.jyoumei.cn

[Q13] 忽略重复插入
来源：http://nrq.yuxming.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://snv.fktsv.cn

[Q14] 存在则更新（upsert）
来源：http://cgu.cqqwz.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ehg.yuanzhike.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wsd.guowangkeji.top

[Q15] 查询全部
来源：http://lxq.ydzc1.top

SELECT * FROM users;
来源：http://svb.nwbrower.top

[Q16] 查询指定列
来源：http://mam.cqqwz.cn

SELECT id, name FROM users;
来源：http://fnt.shangyingyoupin.top

[Q17] 条件查询
来源：http://mhq.tian-w.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ytd.xziqi.cn

[Q18] 模糊匹配
来源：http://jlg.hfpthk.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bhs.yongpay.top

[Q19] 范围查询
来源：http://kbc.hfpthk.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cef.yangfankeji.com

[Q20] IN 列表
来源：http://lep.yvedp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xcp.epnwcf.com

[Q21] 空值判断
来源：http://pvw.fehbvm.com

SELECT * FROM users WHERE email IS NULL;
来源：http://gje.hcnkem.com

[Q22] 排序
来源：http://bbv.yonumen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pbl.guowangkeji.top

[Q23] 分页
来源：http://ray.xziqi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tze.yj202588.top

[Q24] 去重
来源：http://ola.jyoumei.cn

SELECT DISTINCT city FROM users;
来源：http://phs.fktsv.cn

[Q25] 只取前 N 条
来源：http://grr.uphjek.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qji.ywan-chungtsiang.top

[Q26] 计数
来源：http://xce.andypj.xyz

SELECT COUNT(*) FROM users;
来源：http://tvk.yj20258888.top

[Q27] 条件计数
来源：http://jks.feifeiyinyue.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wbu.jianghu66.top

[Q28] 求和与平均
来源：http://glk.quarkkingdee.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://toe.hysaishi.cn

[Q29] 最大最小值
来源：http://kml.jqgufenzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://wia.yvedp.cn

[Q30] 分组统计
来源：http://ghv.hcnkem.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qrq.nwbrower.top

[Q31] 分组后过滤
来源：http://pej.zdqjudy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dir.yangfankeji.com

[Q32] 分组拼接字符串
来源：http://iuw.yongpay.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xjh.yongpay.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mxj.zdqjudy.top

[Q33] 多列分组
来源：http://wmp.tianlin.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oha.nanxuanxn.top

[Q34] 每组取第一条
来源：http://cof.gzhubu.top

SELECT * FROM (
来源：http://zpc.fzhhl.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ooc.zhaomingkeji.xyz

) t WHERE rn = 1;
来源：http://lfg.gaohongyu789.top

[Q35] 内连接
来源：http://xzu.gotoacloud.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zuj.cqqwz.cn

[Q36] 左连接
来源：http://kbt.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zby.tanke756.top

[Q37] 右连接
来源：http://gnz.jlsjyb.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gwa.daxiang520.top

[Q38] 全外连接（PostgreSQL）
来源：http://muy.yongpay.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yue.ehwqpu.com

[Q39] 自连接（查上下级）
来源：http://ugc.xinyue.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://vvn.xuanzx.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tnz.tian-w.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xwe.uphjek.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nzo.zhiwuduotai.top

[Q41] 多表连接
来源：http://gxq.jyoumei.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cxb.jianghu66.top

JOIN users u ON u.id = o.user_id
来源：http://yvd.svipenyu.cn

JOIN products p ON p.id = o.product_id;
来源：http://hrg.guowangkeji.top

[Q42] 连接条件附加过滤
来源：http://yhi.yj20258888.top

SELECT u.name, o.amount FROM users u
来源：http://xqe.gogol.net.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://idx.jqgfzy.top

[Q43] 标量子查询
来源：http://bgh.xziqi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://urf.hfpthk.cn

[Q44] IN 子查询
来源：http://oxi.gogol.net.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://buq.wangshuangyany.cn

[Q45] EXISTS 判断存在
来源：http://cye.9152youxi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cpf.gzhubu.top

[Q46] NOT EXISTS 判断不存在
来源：http://sob.dianchejie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wnr.havefunace.top

[Q47] 与平均值比较
来源：http://mkz.jqgufenzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oqj.jiagoushi.top


<!-- 参考信息 -->