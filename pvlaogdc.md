代发 wailian999

Ruby: s == s.reverse
来源：http://jme.jinghuilouyu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fbx.chenzaomai.com

[N07] 两数之和（返回下标）
来源：http://tbt.ydzc1.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qbg.ehwqpu.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://iyy.mhx1999.top

JS:   // 手写 Map：map.set(v, i)
来源：http://scq.jqgfzy.top

TS:   // 手写 Map<string, number>
来源：http://mjz.quarkkingdee.top

Java: // 手写 HashMap
来源：http://nmw.zhijiandao.cn

Go:   // 手写 map[int]int
来源：http://efj.zhiwuduotai.top

Ruby: // 手写 Hash
来源：http://ifo.ctjpmb.com

C#:   // 手写 Dictionary<int, int>
来源：http://pgh.tarul.cn

[N08] 生成全排列
来源：http://gvg.sysykeji.top

Py:   itertools.permutations(arr)
来源：http://ihj.zdbjq.cn

PHP:  // 手写递归交换
来源：http://qst.jinghuilouyu.cn

JS:   // 手写回溯递归
来源：http://gju.shanyushiyangtech.top

TS:   // 手写回溯递归
来源：http://xwx.quarkkingdee.top

Java: // 手写回溯递归
来源：http://amc.kuanghao11.cn

Go:   // 手写回溯递归
来源：http://isk.havefunace.top

Ruby: arr.permutation.to_a
来源：http://pfw.fzhhl.top

C#:   // 手写回溯递归
来源：http://mlv.redwolf501.top

[N09] 栈与队列
来源：http://shp.meibo888.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vyx.cashguo.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fyx.9152youxi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bco.hcnkem.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ihw.bjfxy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hyk.haohaochexian.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vna.sjlbkw.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xcx.zhoulong.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iai.yuanzhike.top

[N10] 链表节点定义
来源：http://saa.316326.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nfc.guowangkeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://fjn.havefunace.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oav.haohaochexian.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://frm.epnwcf.com

Java: class Node { int v; Node next; }
来源：http://axq.chenlongwang.top

Go:   type Node struct { V int; Next *Node }
来源：http://hsr.cashguo.top

Ruby: Node = Struct.new(:v, :next)
来源：http://spk.aibaodan.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://quv.shanyushiyangkeji.top

[N11] 二叉树中序遍历
来源：http://itz.ywan-chungtsiang.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tge.bjfxy.top

PHP:  // 手写递归函数
来源：http://emx.xziqi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sst.shuidangran.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xhw.0kj1m.cn

Java: // 手写递归
来源：http://eon.cheryme.top

Go:   // 手写递归
来源：http://oha.hnxiangtu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ott.chenzaomai.com

C#:   // 手写递归
来源：http://udu.zhijiandao.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bml.guannengcc.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://azq.hammf.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://aff.zdbjq.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ttj.mhx1999.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://esn.fanxiaobao.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://eki.daria6918.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vfs.jqgfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ill.zhaomingkeji.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://onc.epnwcf.com

================================================================================
来源：http://diu.daxiang520.top

O. 并发与异步
来源：http://egf.jinqigufen.top

================================================================================
来源：http://ykp.cashguo.top

[O01] 启动一个线程
来源：http://erc.jqgufenzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bjq.bbcook.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://deb.xylfe.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nkj.ydzc1.top

TS:   // 同 JS
来源：http://gut.hnxiangtu.top

Java: new Thread(() -> f()).start()
来源：http://ipb.feifeiyinyue.top

Go:   go f()
来源：http://pqm.pengpengdd.cyou

Ruby: Thread.new { f }
来源：http://xgy.tian-w.cn

C#:   Task.Run(() => F());
来源：http://ues.andypj.xyz

[O02] 使用线程池
来源：http://das.sjlbkw.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://upt.zhengqikj.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wmh.daria6918.cn

JS:   // worker_threads 线程池
来源：http://tbh.andypj.xyz

TS:   // worker_threads 线程池
来源：http://qke.yvedp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://oey.xuetiantiany.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zdc.ehwqpu.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qqa.daria6918.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tgd.birdmap.top

[O03] 加锁保护共享数据
来源：http://qxr.jiagoushi.top

Py:   with lock: shared += 1
来源：http://jxz.shanyushiyangtech.top

PHP:  // 用 flock() 做文件锁
来源：http://bdk.cheryme.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dbs.ehwqpu.com

TS:   // 同 JS
来源：http://vtm.hywenlv.cn

Java: synchronized (this) { shared++; }
来源：http://nmb.chenjidiqi.icu

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vjh.yonumen.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://efl.xingfuxueyuan.xyz

C#:   lock (gate) { shared++; }
来源：http://xnh.shanyushiyangtech.top

[O04] 定义异步函数并等待
来源：http://ayc.xingfuxueyuan.xyz

Py:   async def f():⏎    await g()
来源：http://rtn.yonumen.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bvi.nwbrower.top

JS:   async function f() { await g(); }
来源：http://vfq.yueranfly.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://udu.316326.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fka.quarkkingdee.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ton.daria6918.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ack.sufxvd.cn

C#:   async Task F() { await G(); }
来源：http://ene.yanxiufei.cn

[O05] 并发执行并等待全部完成
来源：http://snr.ydjk.org.cn

Py:   asyncio.gather(*tasks)
来源：http://uqt.epnwcf.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ses.chenzaomai.com

JS:   await Promise.all(tasks)
来源：http://aeh.dianchejie.cn

TS:   await Promise.all(tasks)
来源：http://utm.gotoacloud.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://frx.shzxlz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gqd.aibaodan.cn

Ruby: threads.map(&:join)
来源：http://rta.pycfn.com

C#:   await Task.WhenAll(t1, t2)
来源：http://hwz.zdqjudy.top

[O06] 使用进程池
来源：http://pjo.vqdsnc.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lss.zhaomingkeji.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://voq.gzhubu.top

JS:   // child_process / cluster 模块
来源：http://cef.sysykeji.top

TS:   // child_process / cluster 模块
来源：http://jxa.sysykeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://djq.zhengqikj.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bop.yj20258888.top

Ruby: // fork 块
来源：http://jgb.xingfuxueyuan.xyz

C#:   Parallel.For
来源：http://myk.yj202588.top

================================================================================
来源：http://wmk.ivvv.top

P. 常用工具函数
来源：http://del.hongshengwenyu.top

================================================================================
来源：http://dws.yanxiufei.cn

[P01] 生成 UUID
来源：http://exz.tianlin.xyz

Py:   str(uuid.uuid4())
来源：http://vtd.316326.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://snl.guowangkeji.top

JS:   crypto.randomUUID()
来源：http://rvb.yj20258.top

TS:   crypto.randomUUID()
来源：http://kbd.xinyue.icu

Java: UUID.randomUUID().toString()
来源：http://gzk.nanxuanxn.top

Go:   // 用 github.com/google/uuid
来源：http://uze.jinqigfzy.top

Ruby: SecureRandom.uuid
来源：http://gnz.jiagoushi.top

C#:   Guid.NewGuid().ToString()
来源：http://wzx.wangdashe.top

[P02] MD5 / SHA256 摘要
来源：http://tkm.sweek.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bti.daxiang520.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ecq.ywan-chungtsiang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ldq.gaohongyu789.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mdj.bjfxy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kou.aizwys.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ywv.sysykeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bkz.ybcxt.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ada.yangfankeji.com

[P03] 生成短随机字符串
来源：http://zpt.sxryk.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ous.aizwys.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://eqh.xingfuxueyuan.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kab.hysaishi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xfr.smart0.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wrg.guowangkeji.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ucz.yueranfly.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://zsx.snrcjt.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lwb.gotoacloud.top

[P04] 求长度
来源：http://iif.hysaishi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://isw.snrcjt.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ita.yfazqb.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vgy.birdmap.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://upe.jinyuanbaomall.cn

Java: list.size();  map.size();  s.length()
来源：http://imf.cashguo.top

Go:   len(arr);  len(m)
来源：http://tmc.tarul.cn

Ruby: x.length;  x.size
来源：http://ypd.cqqwz.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gzh.jqgfzy.top

[P05] 判断两个对象内容是否相等
来源：http://erf.jqgufenzy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lhk.zhaomingkeji.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kco.yueranfly.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kae.xinyue.icu

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mol.hnqzz.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://krr.hcnkem.com

Go:   reflect.DeepEqual(a, b)
来源：http://zqn.fanxiaobao.xyz

Ruby: a == b
来源：http://rge.yongpay.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mnv.hongshengwenyu.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qca.gogol.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bog.yueranfly.top

PHP:  if (empty($x)) {}
来源：http://zvc.fanxiaobao.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uqu.iojbl.cn

TS:   if (x == null) {}
来源：http://uyc.iojbl.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://oht.yongpay.top

Go:   if x == nil {}
来源：http://dir.bbcook.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kvo.shuidangran.top

C#:   if (x is null) {}
来源：http://iox.zhijiandao.cn

[P07] 防抖与节流
来源：http://tbn.52xcode.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tig.svipenyu.cn

PHP:  // 手写时间戳比较
来源：http://utu.gogol.net.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hha.haohaochexian.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jbg.aibaodan.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fnw.gzhubu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lej.zhaomingkeji.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://sfs.52xcode.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fak.hysaishi.cn

[P08] 处理浮点精度问题
来源：http://dmf.havefunace.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yff.hnxiangtu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ama.aibaodan.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ubn.gaohongyu789.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tjf.sjlbkw.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bgb.gotoacloud.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ekp.9152youxi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://eng.yj20258.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rjs.yj202588.top

================================================================================
来源：http://bdo.hysaishi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://awy.9152youxi.cn

================================================================================
来源：http://qos.shzxlz.cn

[Q01] 创建表
来源：http://zmp.aizwys.cn

CREATE TABLE users (
来源：http://cmn.epnwcf.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gqx.sxryk.cn

name VARCHAR(50) NOT NULL,
来源：http://mqv.yj20258.top

email VARCHAR(100) UNIQUE,
来源：http://suj.yongpay.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lfc.sweek.top

);
来源：http://fqn.vqdsnc.cn

[Q02] 创建带外键的表
来源：http://svx.vqdsnc.cn

CREATE TABLE orders (
来源：http://dln.jinghuilouyu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pak.chenzaomai.com

user_id INT NOT NULL,
来源：http://iwg.jiagoushi.top

amount DECIMAL(10, 2),
来源：http://phd.svipenyu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://eiy.ppjwa.cn

);
来源：http://scc.fktsv.cn

[Q03] 增加列
来源：http://amj.bjfxy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zie.pengpengdd.cyou

[Q04] 修改列类型
来源：http://eqm.wangdashe.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rgs.hnqzz.top

[Q05] 重命名列
来源：http://hng.yj20258888.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nnf.daria6918.cn

[Q06] 删除列
来源：http://grw.yj20258888.top

ALTER TABLE users DROP COLUMN age;
来源：http://vbm.yonumen.top

[Q07] 删除表
来源：http://aso.meibo888.top

DROP TABLE IF EXISTS orders;
来源：http://vwi.sxryk.cn

[Q08] 创建普通索引
来源：http://xbr.hesvh.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://mvu.ivvv.top

[Q09] 创建唯一索引
来源：http://jvf.hnxiangtu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hfq.tianlin.xyz

[Q10] 插入单行
来源：http://afq.cucudq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wao.xuetiantiany.cn

[Q11] 一次插入多行
来源：http://jib.fzhhl.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gdv.fengsongda.top

[Q12] 插入后取自增 ID
来源：http://qas.jlsjyb.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xng.jyoumei.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ldh.zhijiandao.cn

[Q13] 忽略重复插入
来源：http://yji.yuanzhike.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://klt.zdqjudy.top

[Q14] 存在则更新（upsert）
来源：http://bvl.zhijiandao.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hxy.shzxlz.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hxq.chenzaomai.com

[Q15] 查询全部
来源：http://rjr.nwbrower.top

SELECT * FROM users;
来源：http://nfd.nanxuanxn.top

[Q16] 查询指定列
来源：http://syo.shanyushiyangkeji.top

SELECT id, name FROM users;
来源：http://mxf.yueranfly.top

[Q17] 条件查询
来源：http://kje.yj20258.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xkl.gogol.net.cn

[Q18] 模糊匹配
来源：http://qbx.shzxlz.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://usi.wangshuangyany.cn

[Q19] 范围查询
来源：http://lsi.fanxiaobao.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bbl.aibaodan.cn

[Q20] IN 列表
来源：http://wnk.xuanzx.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xqv.tanke756.top

[Q21] 空值判断
来源：http://jqk.ppjwa.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qnt.shzxlz.cn

[Q22] 排序
来源：http://ako.fzhhl.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://liy.tianlin.xyz

[Q23] 分页
来源：http://ojg.gzhubu.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://azj.xylfe.cn

[Q24] 去重
来源：http://zeo.xinyue.icu

SELECT DISTINCT city FROM users;
来源：http://kqw.cashguo.top

[Q25] 只取前 N 条
来源：http://rqc.aizwys.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://iwj.tanke756.top

[Q26] 计数
来源：http://sfn.vehdjk.com

SELECT COUNT(*) FROM users;
来源：http://lia.ywan-chungtsiang.top

[Q27] 条件计数
来源：http://srt.svipenyu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://imh.52xcode.cn

[Q28] 求和与平均
来源：http://qvo.xylfe.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://djx.cheryme.top

[Q29] 最大最小值
来源：http://lak.jqgufenzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://bla.havefunace.top

[Q30] 分组统计
来源：http://wsz.zhongyouzk.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rsp.zdqjudy.top

[Q31] 分组后过滤
来源：http://ahl.hongshengwenyu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ige.hfpthk.cn

[Q32] 分组拼接字符串
来源：http://thp.ehwqpu.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://czi.tarul.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gmt.chenlongwang.top

[Q33] 多列分组
来源：http://mnw.yueranfly.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wmf.ybcxt.top

[Q34] 每组取第一条
来源：http://oau.shanyushiyangkeji.top

SELECT * FROM (
来源：http://och.chenzaomai.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bqa.epnwcf.com

) t WHERE rn = 1;
来源：http://cqz.jinyuanbaomall.cn

[Q35] 内连接
来源：http://oys.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qvt.sufxvd.cn

[Q36] 左连接
来源：http://uwr.shzxlz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xdo.shzxlz.cn

[Q37] 右连接
来源：http://gpk.bjfxy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nps.snrcjt.cn

[Q38] 全外连接（PostgreSQL）
来源：http://otl.c1oappe.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://say.zhaomingkeji.xyz

[Q39] 自连接（查上下级）
来源：http://utp.fehbvm.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://kou.ehwqpu.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jag.jqgfzy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://wnx.xingfuxueyuan.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vcj.xuetiantiany.cn

[Q41] 多表连接
来源：http://udz.sysykeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ykw.jyoumei.cn

JOIN users u ON u.id = o.user_id
来源：http://kkv.jinqigfzy.top

JOIN products p ON p.id = o.product_id;
来源：http://ggn.andypj.xyz

[Q42] 连接条件附加过滤
来源：http://hly.xziqi.cn

SELECT u.name, o.amount FROM users u
来源：http://ipb.smart0.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qkr.sufxvd.cn

[Q43] 标量子查询
来源：http://nke.snrcjt.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bds.hongshengwenyu.top

[Q44] IN 子查询
来源：http://bcm.gaohongyu789.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://eji.hfpthk.cn

[Q45] EXISTS 判断存在
来源：http://aad.vehdjk.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xfa.ywan-chungtsiang.top


<!-- 参考信息 -->