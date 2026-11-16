代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bgo.guowangkeji.top

[N06] 判断回文字符串
来源：http://kdh.fengsongda.top

Py:   s == s[::-1]
来源：http://zvu.guannengcc.top

PHP:  $s === strrev($s);
来源：http://vtu.yfazqb.com

JS:   s === [...s].reverse().join("")
来源：http://der.0kj1m.cn

TS:   s === [...s].reverse().join("")
来源：http://elt.zycfv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ymf.hongshengwenyu.top

Go:   // 双指针从两端比较
来源：http://lpu.nanxuanxn.top

Ruby: s == s.reverse
来源：http://nwh.nwbrower.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lre.shanyushiyangtech.top

[N07] 两数之和（返回下标）
来源：http://jei.havefunace.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mje.jinqigufen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gao.ydzc1.top

JS:   // 手写 Map：map.set(v, i)
来源：http://tuk.daxiang520.top

TS:   // 手写 Map<string, number>
来源：http://hiz.yuxming.cn

Java: // 手写 HashMap
来源：http://oyt.fengsongda.top

Go:   // 手写 map[int]int
来源：http://rwf.9152youxi.cn

Ruby: // 手写 Hash
来源：http://mmx.havefunace.top

C#:   // 手写 Dictionary<int, int>
来源：http://yrc.hfpthk.cn

[N08] 生成全排列
来源：http://idm.sysykeji.top

Py:   itertools.permutations(arr)
来源：http://css.shzxlz.cn

PHP:  // 手写递归交换
来源：http://xll.meibo888.top

JS:   // 手写回溯递归
来源：http://ufw.gzhubu.top

TS:   // 手写回溯递归
来源：http://bnb.shangyingyoupin.top

Java: // 手写回溯递归
来源：http://wlr.zhijiandao.cn

Go:   // 手写回溯递归
来源：http://mpm.9152youxi.cn

Ruby: arr.permutation.to_a
来源：http://ush.jinqigfzy.top

C#:   // 手写回溯递归
来源：http://vhj.jinqigufen.top

[N09] 栈与队列
来源：http://kqi.xylfe.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ptu.cheryme.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zcc.sufxvd.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mez.jinqigufen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://exv.smart0.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hwf.jinqigfzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://atw.shanyushiyangtech.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://otl.jinyuanbaomall.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://aqo.cashguo.top

[N10] 链表节点定义
来源：http://hiv.gzhubu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://aug.aibaodan.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wfe.shzxlz.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gwj.yueranfly.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yam.guowangkeji.top

Java: class Node { int v; Node next; }
来源：http://bdh.birdmap.top

Go:   type Node struct { V int; Next *Node }
来源：http://dbn.wangshuangyany.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ekl.snrcjt.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hnm.svipenyu.cn

[N11] 二叉树中序遍历
来源：http://mza.cdnleiting.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yhs.fktsv.cn

PHP:  // 手写递归函数
来源：http://ioa.sxryk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://opk.guowangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tjc.tianlin.xyz

Java: // 手写递归
来源：http://amo.0kj1m.cn

Go:   // 手写递归
来源：http://lmy.guannengcc.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wcl.daria6918.cn

C#:   // 手写递归
来源：http://jbx.bbcook.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tgi.haohaochexian.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://akn.jinqigufen.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kbl.jinqigfzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nay.andypj.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gyr.hnxiangtu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qcp.yj20258888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://shs.zhongyouzk.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://afo.shanyushiyangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jzg.jlsjyb.cn

================================================================================
来源：http://vfs.cheryme.top

O. 并发与异步
来源：http://skx.uphjek.com

================================================================================
来源：http://sll.jinqigufen.top

[O01] 启动一个线程
来源：http://iii.xuetiantiany.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://duy.pengpengdd.cyou

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://iwe.cucudq.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sko.pengpengdd.cyou

TS:   // 同 JS
来源：http://tag.haohaochexian.top

Java: new Thread(() -> f()).start()
来源：http://zdw.nanxuanxn.top

Go:   go f()
来源：http://ejl.wangshuangyany.cn

Ruby: Thread.new { f }
来源：http://exp.feifeiyinyue.top

C#:   Task.Run(() => F());
来源：http://goy.aibaodan.cn

[O02] 使用线程池
来源：http://prd.jlsjyb.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lpi.yuanzhike.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xhz.316326.xyz

JS:   // worker_threads 线程池
来源：http://sbl.shzxlz.cn

TS:   // worker_threads 线程池
来源：http://ila.jlsjyb.cn

Java: Executors.newFixedThreadPool(4)
来源：http://thz.fktsv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ira.yj20258888.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wdd.ydzc1.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://muh.zhiwuduotai.top

[O03] 加锁保护共享数据
来源：http://krd.guowangkeji.top

Py:   with lock: shared += 1
来源：http://ups.haohaochexian.top

PHP:  // 用 flock() 做文件锁
来源：http://yhf.shangyingyoupin.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ksz.0kj1m.cn

TS:   // 同 JS
来源：http://png.ybcxt.top

Java: synchronized (this) { shared++; }
来源：http://ilb.316326.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rtd.zdqjudy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://nol.yuxming.cn

C#:   lock (gate) { shared++; }
来源：http://zeo.yanxiufei.cn

[O04] 定义异步函数并等待
来源：http://aiw.zycfv.cn

Py:   async def f():⏎    await g()
来源：http://bnk.zhongyouzk.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nue.hammf.cn

JS:   async function f() { await g(); }
来源：http://jel.pycfn.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://ihe.shangyingyoupin.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xbb.jqgufenzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baj.haohaochexian.top

Ruby: # 用 Fiber 或 async gem
来源：http://tqy.jinqigfzy.top

C#:   async Task F() { await G(); }
来源：http://dkw.wangdashe.top

[O05] 并发执行并等待全部完成
来源：http://iki.daxiang520.top

Py:   asyncio.gather(*tasks)
来源：http://lxa.tanke756.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xat.gogol.net.cn

JS:   await Promise.all(tasks)
来源：http://cqm.zhiwuduotai.top

TS:   await Promise.all(tasks)
来源：http://qpr.cheryme.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bpt.zdqjudy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gqu.zhixingplan.top

Ruby: threads.map(&:join)
来源：http://bij.yfazqb.com

C#:   await Task.WhenAll(t1, t2)
来源：http://jqp.shanyushiyangkeji.top

[O06] 使用进程池
来源：http://wyv.yongpay.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rym.zhiwuduotai.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ehg.cdnleiting.top

JS:   // child_process / cluster 模块
来源：http://qla.bbcook.cn

TS:   // child_process / cluster 模块
来源：http://iqm.aibaodan.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wcr.tanke756.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mko.yfazqb.com

Ruby: // fork 块
来源：http://pnu.fehbvm.com

C#:   Parallel.For
来源：http://ead.shanyushiyangkeji.top

================================================================================
来源：http://usu.xziqi.cn

P. 常用工具函数
来源：http://eov.svipenyu.cn

================================================================================
来源：http://exg.snrcjt.cn

[P01] 生成 UUID
来源：http://yxl.shanyushiyangkeji.top

Py:   str(uuid.uuid4())
来源：http://yci.havefunace.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oft.hnqzz.top

JS:   crypto.randomUUID()
来源：http://nts.sxryk.cn

TS:   crypto.randomUUID()
来源：http://snj.gaohongyu789.top

Java: UUID.randomUUID().toString()
来源：http://qpj.fktsv.cn

Go:   // 用 github.com/google/uuid
来源：http://jtn.cdnleiting.top

Ruby: SecureRandom.uuid
来源：http://stb.xuanzx.com

C#:   Guid.NewGuid().ToString()
来源：http://fyf.tian-w.cn

[P02] MD5 / SHA256 摘要
来源：http://geh.chenzaomai.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ldq.xylfe.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://umo.iojbl.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mjs.birdmap.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rlr.yj20258.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sdx.aibaodan.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xbw.ybcxt.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://exf.cucudq.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lwn.wangshuangyany.cn

[P03] 生成短随机字符串
来源：http://krl.wangshuangyany.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kqc.ywan-chungtsiang.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vcv.yuanzhike.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yuv.jlsjyb.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ehy.jinghuilouyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uep.fzhhl.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yta.feifeiyinyue.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://lsy.tianlin.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tsb.andypj.xyz

[P04] 求长度
来源：http://hrn.xziqi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wcv.ehwqpu.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ydb.tanke756.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://whd.jinqigfzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vfx.yanxiufei.cn

Java: list.size();  map.size();  s.length()
来源：http://evv.tian-w.cn

Go:   len(arr);  len(m)
来源：http://pfy.guannengcc.top

Ruby: x.length;  x.size
来源：http://cne.jianghu66.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://byp.0kj1m.cn

[P05] 判断两个对象内容是否相等
来源：http://erw.bbcook.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://iyp.xinyue.icu

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hcx.yj20258888.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gdq.yj20258888.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nye.yj20258.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tfm.birdmap.top

Go:   reflect.DeepEqual(a, b)
来源：http://ope.ehwqpu.com

Ruby: a == b
来源：http://rut.fanxiaobao.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hlz.yvedp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dcf.svipenyu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yha.aibaodan.cn

PHP:  if (empty($x)) {}
来源：http://rcp.shanyushiyangtech.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://eml.cqqwz.cn

TS:   if (x == null) {}
来源：http://oac.zhiwuduotai.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wvj.redwolf501.top

Go:   if x == nil {}
来源：http://lrv.hnxiangtu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tif.c1oappe.top

C#:   if (x is null) {}
来源：http://ygx.ydzc1.top

[P07] 防抖与节流
来源：http://wfb.chenlongwang.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ero.sysykeji.top

PHP:  // 手写时间戳比较
来源：http://nxi.yuxming.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xgs.nanxuanxn.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mbg.shangyingyoupin.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ajt.epnwcf.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jft.sxryk.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://unp.xuetiantiany.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://suc.c1oappe.top

[P08] 处理浮点精度问题
来源：http://kfd.jqgfzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jbk.zhongyouzk.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ygx.guowangkeji.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rco.gaohongyu789.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fuq.haohaochexian.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xto.bbcook.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rss.zhoulong.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jek.zhoulong.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cub.fanxiaobao.xyz

================================================================================
来源：http://tby.bbcook.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fjk.fengsongda.top

================================================================================
来源：http://kto.shanyushiyangkeji.top

[Q01] 创建表
来源：http://vtu.vqdsnc.cn

CREATE TABLE users (
来源：http://qfa.cashguo.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kkv.nwbrower.top

name VARCHAR(50) NOT NULL,
来源：http://sqr.fehbvm.com

email VARCHAR(100) UNIQUE,
来源：http://fix.hywenlv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zfc.fehbvm.com

);
来源：http://mgi.hysaishi.cn

[Q02] 创建带外键的表
来源：http://vda.yuanzhike.top

CREATE TABLE orders (
来源：http://pqd.vqdsnc.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ljd.zhaomingkeji.xyz

user_id INT NOT NULL,
来源：http://zls.yangfankeji.com

amount DECIMAL(10, 2),
来源：http://dkq.zhengqikj.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://udh.yongpay.top

);
来源：http://sil.fengsongda.top

[Q03] 增加列
来源：http://lnk.gaohongyu789.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://chy.yj20258888.top

[Q04] 修改列类型
来源：http://gxp.nwbrower.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sej.sxryk.cn

[Q05] 重命名列
来源：http://dwi.ydjk.org.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qvc.svipenyu.cn

[Q06] 删除列
来源：http://iax.ehwqpu.com

ALTER TABLE users DROP COLUMN age;
来源：http://wll.birdmap.top

[Q07] 删除表
来源：http://oqj.xziqi.cn

DROP TABLE IF EXISTS orders;
来源：http://vjq.gotoacloud.top

[Q08] 创建普通索引
来源：http://xtl.yj202588.top

CREATE INDEX idx_users_email ON users(email);
来源：http://cjh.zhixingplan.top

[Q09] 创建唯一索引
来源：http://zyj.fktsv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ibq.daria6918.cn

[Q10] 插入单行
来源：http://lxp.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://iyp.wangshuangyany.cn

[Q11] 一次插入多行
来源：http://woj.shanyushiyangtech.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ejn.fanxiaobao.xyz

[Q12] 插入后取自增 ID
来源：http://lfy.sweek.top

INSERT INTO users (name) VALUES ('C');
来源：http://sgd.jqgufenzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lyy.fanxiaobao.xyz

[Q13] 忽略重复插入
来源：http://jpk.nanxinkj.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zqb.aibaodan.cn

[Q14] 存在则更新（upsert）
来源：http://cpx.haohaochexian.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vyl.dashuyun.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lak.smart0.xyz

[Q15] 查询全部
来源：http://sjo.hywenlv.cn

SELECT * FROM users;
来源：http://lbx.zhaomingkeji.xyz

[Q16] 查询指定列
来源：http://iii.cqqwz.cn

SELECT id, name FROM users;
来源：http://vxn.quarkkingdee.top

[Q17] 条件查询
来源：http://wpu.haohaochexian.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://efi.ctjpmb.com

[Q18] 模糊匹配
来源：http://oeu.yuxming.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xol.nanxinkj.top

[Q19] 范围查询
来源：http://ryt.jlsjyb.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ucq.fanxiaobao.xyz

[Q20] IN 列表
来源：http://byg.jinghuilouyu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zcp.aizwys.cn

[Q21] 空值判断
来源：http://nje.dianchejie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lky.zhengqikj.top

[Q22] 排序
来源：http://uvt.jqgfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gmf.gzhubu.top

[Q23] 分页
来源：http://kuf.tanke756.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fzy.shzxlz.cn

[Q24] 去重
来源：http://xol.chenjidiqi.icu

SELECT DISTINCT city FROM users;
来源：http://nal.jianghu66.top

[Q25] 只取前 N 条
来源：http://isu.pengpengdd.cyou

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lwj.yonumen.top

[Q26] 计数
来源：http://ujx.bjfxy.top

SELECT COUNT(*) FROM users;
来源：http://sgs.chenjidiqi.icu

[Q27] 条件计数
来源：http://tkt.feifeiyinyue.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://elk.yueranfly.top

[Q28] 求和与平均
来源：http://qap.jinyuanbaomall.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dcz.pycfn.com

[Q29] 最大最小值
来源：http://oop.chenjidiqi.icu

SELECT MAX(age), MIN(age) FROM users;
来源：http://mro.hfpthk.cn

[Q30] 分组统计
来源：http://det.jianghu66.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cvr.vehdjk.com

[Q31] 分组后过滤
来源：http://mob.hnxiangtu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ncz.jlsjyb.cn

[Q32] 分组拼接字符串
来源：http://bhm.gotoacloud.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ohf.ppjwa.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zhb.shangyingyoupin.top

[Q33] 多列分组
来源：http://rfq.hesvh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hgx.ivvv.top

[Q34] 每组取第一条
来源：http://mll.bjfxy.top

SELECT * FROM (
来源：http://pyn.yuxming.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fwz.cashguo.top

) t WHERE rn = 1;
来源：http://bcq.meibo888.top

[Q35] 内连接
来源：http://lgg.jqgfzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mwe.hywenlv.cn

[Q36] 左连接
来源：http://qod.zdbjq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rdr.yangfankeji.com

[Q37] 右连接
来源：http://fji.cqqwz.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ssa.nanxinkj.top

[Q38] 全外连接（PostgreSQL）
来源：http://qto.316326.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zkv.hywenlv.cn

[Q39] 自连接（查上下级）
来源：http://fud.tarul.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nrj.daria6918.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://fkf.sysykeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://bzp.ydzc1.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://eyb.xuanzx.com

[Q41] 多表连接
来源：http://aan.snrcjt.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lqr.aibaodan.cn

JOIN users u ON u.id = o.user_id
来源：http://pnu.jinghuilouyu.cn

JOIN products p ON p.id = o.product_id;
来源：http://uue.jyoumei.cn

[Q42] 连接条件附加过滤
来源：http://vcr.ybcxt.top


<!-- 参考信息 -->