代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://axt.birdmap.top

JS:   // 手写 Map：map.set(v, i)
来源：http://cvk.kuanghao11.cn

TS:   // 手写 Map<string, number>
来源：http://rvn.svipenyu.cn

Java: // 手写 HashMap
来源：http://oxi.chenlongwang.top

Go:   // 手写 map[int]int
来源：http://imy.jinghuilouyu.cn

Ruby: // 手写 Hash
来源：http://tir.feifeiyinyue.top

C#:   // 手写 Dictionary<int, int>
来源：http://edz.smart0.xyz

[N08] 生成全排列
来源：http://zjz.redwolf501.top

Py:   itertools.permutations(arr)
来源：http://tpl.dianchejie.cn

PHP:  // 手写递归交换
来源：http://ejm.cqqwz.cn

JS:   // 手写回溯递归
来源：http://oai.cdnleiting.top

TS:   // 手写回溯递归
来源：http://rtk.yj202588.top

Java: // 手写回溯递归
来源：http://esk.tianlin.xyz

Go:   // 手写回溯递归
来源：http://gsy.nwbrower.top

Ruby: arr.permutation.to_a
来源：http://gqt.nanxinkj.top

C#:   // 手写回溯递归
来源：http://chq.gogol.net.cn

[N09] 栈与队列
来源：http://wmn.smart0.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zyz.sweek.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://poh.xuanzx.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tnd.kuanghao11.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://iux.sufxvd.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nrd.sjlbkw.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dnw.gaohongyu789.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dyb.snrcjt.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xju.c1oappe.top

[N10] 链表节点定义
来源：http://yih.jyoumei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ykr.fehbvm.com

PHP:  class Node { public $v; public $next = null; }
来源：http://bme.yvedp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://roa.haohaochexian.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rbb.zhengqikj.top

Java: class Node { int v; Node next; }
来源：http://tcl.c1oappe.top

Go:   type Node struct { V int; Next *Node }
来源：http://xkr.ppjwa.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fkp.haohaochexian.top

C#:   class Node { public int V; public Node? Next; }
来源：http://lld.uphjek.com

[N11] 二叉树中序遍历
来源：http://gkp.vqdsnc.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hrq.nanxuanxn.top

PHP:  // 手写递归函数
来源：http://oet.hysaishi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://izo.wangshuangyany.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xaa.tian-w.cn

Java: // 手写递归
来源：http://hmu.52xcode.cn

Go:   // 手写递归
来源：http://gyx.shanyushiyangtech.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xpj.ywan-chungtsiang.top

C#:   // 手写递归
来源：http://bgw.epnwcf.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tla.jianghu66.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mzy.hfpthk.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kep.316326.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tpa.jlsjyb.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rdi.hesvh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pbq.snrcjt.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ajg.jianghu66.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hnl.cdnleiting.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sfy.iojbl.cn

================================================================================
来源：http://jmg.ppjwa.cn

O. 并发与异步
来源：http://xjn.0kj1m.cn

================================================================================
来源：http://urr.ydjk.org.cn

[O01] 启动一个线程
来源：http://qcq.hnqzz.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://otd.yuanzhike.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ibj.quarkkingdee.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ncj.316326.xyz

TS:   // 同 JS
来源：http://nuj.jinghuilouyu.cn

Java: new Thread(() -> f()).start()
来源：http://zvs.redwolf501.top

Go:   go f()
来源：http://nmw.daxiang520.top

Ruby: Thread.new { f }
来源：http://prk.yanxiufei.cn

C#:   Task.Run(() => F());
来源：http://cul.zhoulong.xyz

[O02] 使用线程池
来源：http://gly.shanyushiyangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dkf.hywenlv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nbf.hesvh.cn

JS:   // worker_threads 线程池
来源：http://kxu.redwolf501.top

TS:   // worker_threads 线程池
来源：http://fuw.epnwcf.com

Java: Executors.newFixedThreadPool(4)
来源：http://yyn.quarkkingdee.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ysu.fanxiaobao.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bid.cqqwz.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xmy.pycfn.com

[O03] 加锁保护共享数据
来源：http://fkj.zdqjudy.top

Py:   with lock: shared += 1
来源：http://urk.zhaomingkeji.xyz

PHP:  // 用 flock() 做文件锁
来源：http://utt.yuanzhike.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cfn.feifeiyinyue.top

TS:   // 同 JS
来源：http://olx.nanxuanxn.top

Java: synchronized (this) { shared++; }
来源：http://jcp.wangdashe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zvh.yj202588.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://sqf.pycfn.com

C#:   lock (gate) { shared++; }
来源：http://yfq.zdbjq.cn

[O04] 定义异步函数并等待
来源：http://pnv.hysaishi.cn

Py:   async def f():⏎    await g()
来源：http://vqj.316326.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vpg.vqdsnc.cn

JS:   async function f() { await g(); }
来源：http://ukq.havefunace.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://pwb.pengpengdd.cyou

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ymv.hcnkem.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qxx.sweek.top

Ruby: # 用 Fiber 或 async gem
来源：http://sdn.andypj.xyz

C#:   async Task F() { await G(); }
来源：http://eht.ydjk.org.cn

[O05] 并发执行并等待全部完成
来源：http://ebp.ehwqpu.com

Py:   asyncio.gather(*tasks)
来源：http://fxl.cdnleiting.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pnp.meibo888.top

JS:   await Promise.all(tasks)
来源：http://jtz.xziqi.cn

TS:   await Promise.all(tasks)
来源：http://tof.ppjwa.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jth.aizwys.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ycn.hfpthk.cn

Ruby: threads.map(&:join)
来源：http://wxu.hnqzz.top

C#:   await Task.WhenAll(t1, t2)
来源：http://dwt.xingfuxueyuan.xyz

[O06] 使用进程池
来源：http://ewy.jinqigfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bpc.yonumen.top

PHP:  // pcntl_fork 或多进程队列
来源：http://inc.sjlbkw.cn

JS:   // child_process / cluster 模块
来源：http://zpa.cheryme.top

TS:   // child_process / cluster 模块
来源：http://uhn.hnqzz.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gst.hnqzz.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hvy.hongshengwenyu.top

Ruby: // fork 块
来源：http://ljj.wangdashe.top

C#:   Parallel.For
来源：http://aqj.jinqigfzy.top

================================================================================
来源：http://sou.redwolf501.top

P. 常用工具函数
来源：http://hay.jqgufenzy.top

================================================================================
来源：http://yfx.zhixingplan.top

[P01] 生成 UUID
来源：http://ggm.zhiwuduotai.top

Py:   str(uuid.uuid4())
来源：http://tfg.yj20258.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tyf.xylfe.cn

JS:   crypto.randomUUID()
来源：http://sqv.ehwqpu.com

TS:   crypto.randomUUID()
来源：http://ery.cashguo.top

Java: UUID.randomUUID().toString()
来源：http://kek.hammf.cn

Go:   // 用 github.com/google/uuid
来源：http://zad.zhixingplan.top

Ruby: SecureRandom.uuid
来源：http://hae.0kj1m.cn

C#:   Guid.NewGuid().ToString()
来源：http://rkz.shanyushiyangtech.top

[P02] MD5 / SHA256 摘要
来源：http://qcp.redwolf501.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ppg.hcnkem.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://hsy.316326.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qff.kuanghao11.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rop.fktsv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rdq.yuxming.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rjx.ppjwa.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ksk.zycfv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://var.tanke756.top

[P03] 生成短随机字符串
来源：http://ghk.shanyushiyangtech.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ruj.meibo888.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wis.nanxinkj.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oyq.zhiwuduotai.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sji.epnwcf.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://emw.0kj1m.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sdp.yuxming.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zhb.birdmap.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xfg.aibaodan.cn

[P04] 求长度
来源：http://hfh.zhaomingkeji.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rkp.shanyushiyangtech.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kxk.chenzaomai.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pns.bjfxy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kbx.xinyue.icu

Java: list.size();  map.size();  s.length()
来源：http://xqx.zdqjudy.top

Go:   len(arr);  len(m)
来源：http://tfa.hongshengwenyu.top

Ruby: x.length;  x.size
来源：http://saq.yj20258888.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://rmy.ctjpmb.com

[P05] 判断两个对象内容是否相等
来源：http://zui.yvedp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://grb.yueranfly.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pfl.daxiang520.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hdg.c1oappe.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://egb.shanyushiyangtech.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cnc.tian-w.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fch.yj202588.top

Ruby: a == b
来源：http://xxt.jinghuilouyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jew.nwbrower.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://imx.sufxvd.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cll.dianchejie.cn

PHP:  if (empty($x)) {}
来源：http://wvd.zhixingplan.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vur.vqdsnc.cn

TS:   if (x == null) {}
来源：http://iop.zhijiandao.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fbd.hnqzz.top

Go:   if x == nil {}
来源：http://mzg.smart0.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://geh.bbcook.cn

C#:   if (x is null) {}
来源：http://pza.zycfv.cn

[P07] 防抖与节流
来源：http://pax.yj20258.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xvd.cashguo.top

PHP:  // 手写时间戳比较
来源：http://vre.sufxvd.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gyd.aizwys.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rwt.chenjidiqi.icu

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yev.meibo888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lky.sysykeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://tek.shanyushiyangtech.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vtv.yfazqb.com

[P08] 处理浮点精度问题
来源：http://omw.gotoacloud.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pad.wangdashe.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qdv.sxryk.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gvj.mhx1999.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jzw.ehwqpu.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sjc.cheryme.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hbr.gaohongyu789.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jen.hfpthk.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cgc.cdnleiting.top

================================================================================
来源：http://tlz.daxiang520.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bdk.sjlbkw.cn

================================================================================
来源：http://klp.yangfankeji.com

[Q01] 创建表
来源：http://cog.guannengcc.top

CREATE TABLE users (
来源：http://qzb.hywenlv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://prc.c1oappe.top

name VARCHAR(50) NOT NULL,
来源：http://xqs.ppjwa.cn

email VARCHAR(100) UNIQUE,
来源：http://uid.xylfe.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yxe.smart0.xyz

);
来源：http://rjs.jinghuilouyu.cn

[Q02] 创建带外键的表
来源：http://xje.0kj1m.cn

CREATE TABLE orders (
来源：http://gdm.jinqigufen.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fjr.fehbvm.com

user_id INT NOT NULL,
来源：http://qnd.cqqwz.cn

amount DECIMAL(10, 2),
来源：http://ghh.fehbvm.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uby.jyoumei.cn

);
来源：http://hid.cqqwz.cn

[Q03] 增加列
来源：http://whx.jinghuilouyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://age.tian-w.cn

[Q04] 修改列类型
来源：http://djj.yongpay.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pna.yj20258.top

[Q05] 重命名列
来源：http://vyz.jqgufenzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tab.yongpay.top

[Q06] 删除列
来源：http://ofp.yvedp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kdi.hnxiangtu.top

[Q07] 删除表
来源：http://fcl.ehwqpu.com

DROP TABLE IF EXISTS orders;
来源：http://nts.shuidangran.top

[Q08] 创建普通索引
来源：http://tcj.kuanghao11.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://dbq.havefunace.top

[Q09] 创建唯一索引
来源：http://feq.xingfuxueyuan.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zct.quarkkingdee.top

[Q10] 插入单行
来源：http://fpt.xinyue.icu

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fnj.xuetiantiany.cn

[Q11] 一次插入多行
来源：http://huv.shuidangran.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uab.52xcode.cn

[Q12] 插入后取自增 ID
来源：http://mvg.iojbl.cn

INSERT INTO users (name) VALUES ('C');
来源：http://pog.fktsv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uws.pengpengdd.cyou

[Q13] 忽略重复插入
来源：http://dsm.c1oappe.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xnj.zhongyouzk.top

[Q14] 存在则更新（upsert）
来源：http://vtc.xingfuxueyuan.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zbo.birdmap.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ebz.zhiwuduotai.top

[Q15] 查询全部
来源：http://lvw.ywan-chungtsiang.top

SELECT * FROM users;
来源：http://tcq.52xcode.cn

[Q16] 查询指定列
来源：http://lzd.hfpthk.cn

SELECT id, name FROM users;
来源：http://dbh.0kj1m.cn

[Q17] 条件查询
来源：http://aad.xuetiantiany.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fou.yueranfly.top

[Q18] 模糊匹配
来源：http://hrv.fehbvm.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mak.ybcxt.top

[Q19] 范围查询
来源：http://rco.zhongyouzk.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hgr.mhx1999.top

[Q20] IN 列表
来源：http://fln.haohaochexian.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pid.ehwqpu.com

[Q21] 空值判断
来源：http://ofk.zhijiandao.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jlj.iojbl.cn

[Q22] 排序
来源：http://yeq.hnqzz.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lxx.smart0.xyz

[Q23] 分页
来源：http://nqx.hywenlv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tog.yangfankeji.com

[Q24] 去重
来源：http://tnn.yj202588.top

SELECT DISTINCT city FROM users;
来源：http://drd.sxryk.cn

[Q25] 只取前 N 条
来源：http://lds.yongpay.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zpb.xuanzx.com

[Q26] 计数
来源：http://tzk.sjlbkw.cn

SELECT COUNT(*) FROM users;
来源：http://omr.fehbvm.com

[Q27] 条件计数
来源：http://uiy.jlsjyb.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yne.yvedp.cn

[Q28] 求和与平均
来源：http://guk.zhijiandao.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ysz.smart0.xyz

[Q29] 最大最小值
来源：http://wop.9152youxi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ixh.cqqwz.cn

[Q30] 分组统计
来源：http://vfy.gogol.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gln.nanxinkj.top

[Q31] 分组后过滤
来源：http://zxm.gotoacloud.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kvz.zhoulong.xyz

[Q32] 分组拼接字符串
来源：http://qcj.zhengqikj.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uti.ctjpmb.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gta.fehbvm.com

[Q33] 多列分组
来源：http://iyv.yuxming.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://phg.yj20258.top

[Q34] 每组取第一条
来源：http://hvo.hfpthk.cn

SELECT * FROM (
来源：http://whi.sjlbkw.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fbi.hywenlv.cn

) t WHERE rn = 1;
来源：http://tys.fzhhl.top

[Q35] 内连接
来源：http://syr.chenjidiqi.icu

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wkj.daria6918.cn

[Q36] 左连接
来源：http://dng.redwolf501.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dmx.havefunace.top

[Q37] 右连接
来源：http://jxx.guowangkeji.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fkq.jqgufenzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://tra.yanxiufei.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bgp.yanxiufei.cn

[Q39] 自连接（查上下级）
来源：http://neg.nanxinkj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://xaz.yuxming.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zfc.zycfv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rte.meibo888.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://llt.yonumen.top

[Q41] 多表连接
来源：http://leq.jinyuanbaomall.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cct.shzxlz.cn

JOIN users u ON u.id = o.user_id
来源：http://pvh.smart0.xyz

JOIN products p ON p.id = o.product_id;
来源：http://old.svipenyu.cn

[Q42] 连接条件附加过滤
来源：http://xei.guannengcc.top

SELECT u.name, o.amount FROM users u
来源：http://owg.daxiang520.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nse.cdnleiting.top

[Q43] 标量子查询
来源：http://obw.svipenyu.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fnw.shzxlz.cn

[Q44] IN 子查询
来源：http://yza.chenzaomai.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jpb.andypj.xyz

[Q45] EXISTS 判断存在
来源：http://vxq.aizwys.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rbp.aizwys.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nkq.redwolf501.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nee.gaohongyu789.top

[Q47] 与平均值比较
来源：http://tza.guannengcc.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://coj.redwolf501.top


<!-- 参考信息 -->