代发 wailian999

Ruby: s == s.reverse
来源：http://qxs.hcnkem.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://mcw.xingfuxueyuan.xyz

[N07] 两数之和（返回下标）
来源：http://lbo.yanxiufei.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qwf.yj20258888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yzw.ppjwa.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wik.sxryk.cn

TS:   // 手写 Map<string, number>
来源：http://ztj.nanxuanxn.top

Java: // 手写 HashMap
来源：http://dqk.fengsongda.top

Go:   // 手写 map[int]int
来源：http://oab.jinqigufen.top

Ruby: // 手写 Hash
来源：http://pfm.ydjk.org.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ynq.aibaodan.cn

[N08] 生成全排列
来源：http://dwe.tian-w.cn

Py:   itertools.permutations(arr)
来源：http://oss.quarkkingdee.top

PHP:  // 手写递归交换
来源：http://vue.smart0.xyz

JS:   // 手写回溯递归
来源：http://boa.jinqigufen.top

TS:   // 手写回溯递归
来源：http://umg.wangshuangyany.cn

Java: // 手写回溯递归
来源：http://pgz.gogol.net.cn

Go:   // 手写回溯递归
来源：http://kdp.0kj1m.cn

Ruby: arr.permutation.to_a
来源：http://hjl.snrcjt.cn

C#:   // 手写回溯递归
来源：http://eel.xylfe.cn

[N09] 栈与队列
来源：http://zsz.hnxiangtu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nhd.yj202588.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tcg.vehdjk.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bhb.chenjidiqi.icu

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qhg.gzhubu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://erl.jianghu66.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mhk.gzhubu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ytr.jiagoushi.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tin.zdbjq.cn

[N10] 链表节点定义
来源：http://wak.snrcjt.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qwa.jinghuilouyu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yvg.316326.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rbd.epnwcf.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://efn.tianlin.xyz

Java: class Node { int v; Node next; }
来源：http://rlx.fanxiaobao.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://osk.chenzaomai.com

Ruby: Node = Struct.new(:v, :next)
来源：http://bvl.sweek.top

C#:   class Node { public int V; public Node? Next; }
来源：http://qsx.wangshuangyany.cn

[N11] 二叉树中序遍历
来源：http://bnc.zycfv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zyv.9152youxi.cn

PHP:  // 手写递归函数
来源：http://pmo.kuanghao11.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pnb.jinghuilouyu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://usj.yonumen.top

Java: // 手写递归
来源：http://ifr.chenlongwang.top

Go:   // 手写递归
来源：http://jqu.316326.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vyx.iojbl.cn

C#:   // 手写递归
来源：http://afq.pengpengdd.cyou

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kgr.sufxvd.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://clv.xinyue.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vgt.shzxlz.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eku.gzhubu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mjf.gogol.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vwp.yfazqb.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://quw.jlsjyb.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uav.chenlongwang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ptq.birdmap.top

================================================================================
来源：http://vqr.vqdsnc.cn

O. 并发与异步
来源：http://uzr.hammf.cn

================================================================================
来源：http://jtd.tian-w.cn

[O01] 启动一个线程
来源：http://msi.yj202588.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kav.jinqigufen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qaj.tanke756.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yhq.jlsjyb.cn

TS:   // 同 JS
来源：http://kdq.cdnleiting.top

Java: new Thread(() -> f()).start()
来源：http://bxi.daria6918.cn

Go:   go f()
来源：http://idf.xuanzx.com

Ruby: Thread.new { f }
来源：http://fpz.tian-w.cn

C#:   Task.Run(() => F());
来源：http://cxb.snrcjt.cn

[O02] 使用线程池
来源：http://oiw.ctjpmb.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://too.cqqwz.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fmq.yfazqb.com

JS:   // worker_threads 线程池
来源：http://xij.dianchejie.cn

TS:   // worker_threads 线程池
来源：http://tbu.wangshuangyany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rvy.ydjk.org.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bit.tanke756.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://klx.shanyushiyangkeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uhq.yvedp.cn

[O03] 加锁保护共享数据
来源：http://ysc.cheryme.top

Py:   with lock: shared += 1
来源：http://pws.yangfankeji.com

PHP:  // 用 flock() 做文件锁
来源：http://qeh.vqdsnc.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hpt.jqgfzy.top

TS:   // 同 JS
来源：http://mhc.shuidangran.top

Java: synchronized (this) { shared++; }
来源：http://kyu.gotoacloud.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uzp.andypj.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://jht.birdmap.top

C#:   lock (gate) { shared++; }
来源：http://uwu.hongshengwenyu.top

[O04] 定义异步函数并等待
来源：http://grm.xylfe.cn

Py:   async def f():⏎    await g()
来源：http://crp.pycfn.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://aiy.jyoumei.cn

JS:   async function f() { await g(); }
来源：http://yvr.sweek.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://qfe.tianlin.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uym.vehdjk.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://buk.ctjpmb.com

Ruby: # 用 Fiber 或 async gem
来源：http://cbo.jiagoushi.top

C#:   async Task F() { await G(); }
来源：http://ums.guannengcc.top

[O05] 并发执行并等待全部完成
来源：http://xmq.fzhhl.top

Py:   asyncio.gather(*tasks)
来源：http://hkv.uphjek.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lqu.zdbjq.cn

JS:   await Promise.all(tasks)
来源：http://ezj.gotoacloud.top

TS:   await Promise.all(tasks)
来源：http://odq.dianchejie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kho.shuidangran.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ufd.chenjidiqi.icu

Ruby: threads.map(&:join)
来源：http://hxp.yueranfly.top

C#:   await Task.WhenAll(t1, t2)
来源：http://pqv.hysaishi.cn

[O06] 使用进程池
来源：http://uyi.hysaishi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://szf.52xcode.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bff.jinyuanbaomall.cn

JS:   // child_process / cluster 模块
来源：http://cmn.yueranfly.top

TS:   // child_process / cluster 模块
来源：http://zye.hnxiangtu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oah.birdmap.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://aqw.jiagoushi.top

Ruby: // fork 块
来源：http://boz.gaohongyu789.top

C#:   Parallel.For
来源：http://xte.smart0.xyz

================================================================================
来源：http://cps.gogol.net.cn

P. 常用工具函数
来源：http://ppt.uphjek.com

================================================================================
来源：http://yji.xylfe.cn

[P01] 生成 UUID
来源：http://nap.yanxiufei.cn

Py:   str(uuid.uuid4())
来源：http://akz.uphjek.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://esc.zhiwuduotai.top

JS:   crypto.randomUUID()
来源：http://nzj.jqgfzy.top

TS:   crypto.randomUUID()
来源：http://let.gzhubu.top

Java: UUID.randomUUID().toString()
来源：http://oww.aibaodan.cn

Go:   // 用 github.com/google/uuid
来源：http://lnz.cdnleiting.top

Ruby: SecureRandom.uuid
来源：http://hof.daxiang520.top

C#:   Guid.NewGuid().ToString()
来源：http://fek.52xcode.cn

[P02] MD5 / SHA256 摘要
来源：http://emq.jinghuilouyu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://luy.meibo888.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://jyr.sjlbkw.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ixo.xziqi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mkg.xziqi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tkc.aizwys.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://daf.daxiang520.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xvi.hysaishi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qqb.cqqwz.cn

[P03] 生成短随机字符串
来源：http://wtt.yueranfly.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://thm.yangfankeji.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://syt.mhx1999.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ayb.hnxiangtu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ugw.wangdashe.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qlw.xylfe.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hcr.shanyushiyangtech.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://oly.hnqzz.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zvx.zhiwuduotai.top

[P04] 求长度
来源：http://zve.yvedp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yaj.feifeiyinyue.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mnk.hnxiangtu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hww.sxryk.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jkd.cashguo.top

Java: list.size();  map.size();  s.length()
来源：http://foe.yvedp.cn

Go:   len(arr);  len(m)
来源：http://yqz.iojbl.cn

Ruby: x.length;  x.size
来源：http://xeh.cashguo.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ess.yonumen.top

[P05] 判断两个对象内容是否相等
来源：http://ujm.ctjpmb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://qvg.pengpengdd.cyou

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zci.yueranfly.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rlo.hongshengwenyu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hwg.ywan-chungtsiang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xfj.bjfxy.top

Go:   reflect.DeepEqual(a, b)
来源：http://wes.daria6918.cn

Ruby: a == b
来源：http://wtj.hcnkem.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://but.yangfankeji.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://llr.yuxming.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jem.yj202588.top

PHP:  if (empty($x)) {}
来源：http://wee.jinghuilouyu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fwf.iojbl.cn

TS:   if (x == null) {}
来源：http://vpq.aizwys.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pvx.jinqigfzy.top

Go:   if x == nil {}
来源：http://cst.snrcjt.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ucw.shanyushiyangkeji.top

C#:   if (x is null) {}
来源：http://suh.birdmap.top

[P07] 防抖与节流
来源：http://kxj.yonumen.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ryn.yj20258.top

PHP:  // 手写时间戳比较
来源：http://tyt.bjfxy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mxc.yongpay.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bml.meibo888.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zlz.guannengcc.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rqx.yj20258888.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://edx.tarul.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wcw.ydzc1.top

[P08] 处理浮点精度问题
来源：http://uaa.52xcode.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://faw.sjlbkw.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jer.shzxlz.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uab.pycfn.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tdy.ydjk.org.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vdz.yj20258.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hob.guannengcc.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dun.zdbjq.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://epb.yfazqb.com

================================================================================
来源：http://ddn.nanxinkj.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rad.gotoacloud.top

================================================================================
来源：http://zhf.jyoumei.cn

[Q01] 创建表
来源：http://lzu.shuidangran.top

CREATE TABLE users (
来源：http://pdi.sweek.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vfh.jyoumei.cn

name VARCHAR(50) NOT NULL,
来源：http://zcg.wangdashe.top

email VARCHAR(100) UNIQUE,
来源：http://wul.zhaomingkeji.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yve.kuanghao11.cn

);
来源：http://gkc.xuanzx.com

[Q02] 创建带外键的表
来源：http://wmf.meibo888.top

CREATE TABLE orders (
来源：http://bro.tarul.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tkd.dashuyun.cn

user_id INT NOT NULL,
来源：http://oeu.kuanghao11.cn

amount DECIMAL(10, 2),
来源：http://yqq.zhoulong.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qhk.jinqigfzy.top

);
来源：http://qgx.yj20258.top

[Q03] 增加列
来源：http://iqb.zhengqikj.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ghb.9152youxi.cn

[Q04] 修改列类型
来源：http://wkr.shzxlz.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xmg.jiagoushi.top

[Q05] 重命名列
来源：http://sao.zhiwuduotai.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fgt.sxryk.cn

[Q06] 删除列
来源：http://rvl.guannengcc.top

ALTER TABLE users DROP COLUMN age;
来源：http://uis.shzxlz.cn

[Q07] 删除表
来源：http://crf.feifeiyinyue.top

DROP TABLE IF EXISTS orders;
来源：http://lsc.jqgfzy.top

[Q08] 创建普通索引
来源：http://sxi.hnxiangtu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xlk.aibaodan.cn

[Q09] 创建唯一索引
来源：http://vms.jinyuanbaomall.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kme.vehdjk.com

[Q10] 插入单行
来源：http://qiv.hysaishi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hxf.hysaishi.cn

[Q11] 一次插入多行
来源：http://wfa.yongpay.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cnd.xylfe.cn

[Q12] 插入后取自增 ID
来源：http://yji.pengpengdd.cyou

INSERT INTO users (name) VALUES ('C');
来源：http://ptt.pengpengdd.cyou

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tkr.jinghuilouyu.cn

[Q13] 忽略重复插入
来源：http://ski.zhengqikj.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lco.feifeiyinyue.top

[Q14] 存在则更新（upsert）
来源：http://idj.shangyingyoupin.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bgj.zhongyouzk.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://isj.feifeiyinyue.top

[Q15] 查询全部
来源：http://bew.daria6918.cn

SELECT * FROM users;
来源：http://tkh.sysykeji.top

[Q16] 查询指定列
来源：http://are.jlsjyb.cn

SELECT id, name FROM users;
来源：http://xaz.haohaochexian.top

[Q17] 条件查询
来源：http://pkn.hongshengwenyu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cdt.fktsv.cn

[Q18] 模糊匹配
来源：http://vpg.gogol.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vhn.aizwys.cn

[Q19] 范围查询
来源：http://zlo.hesvh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rme.ctjpmb.com

[Q20] IN 列表
来源：http://nvy.yj20258888.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kgl.chenlongwang.top

[Q21] 空值判断
来源：http://ynj.fzhhl.top

SELECT * FROM users WHERE email IS NULL;
来源：http://xmm.fzhhl.top

[Q22] 排序
来源：http://zcv.jyoumei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pag.hammf.cn

[Q23] 分页
来源：http://slp.fktsv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nhz.pengpengdd.cyou

[Q24] 去重
来源：http://vzr.dashuyun.cn

SELECT DISTINCT city FROM users;
来源：http://iaq.yuanzhike.top

[Q25] 只取前 N 条
来源：http://qzk.epnwcf.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fpw.xingfuxueyuan.xyz

[Q26] 计数
来源：http://cws.havefunace.top

SELECT COUNT(*) FROM users;
来源：http://svv.yuxming.cn

[Q27] 条件计数
来源：http://psg.nanxinkj.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ekz.tianlin.xyz

[Q28] 求和与平均
来源：http://gei.c1oappe.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gns.xylfe.cn

[Q29] 最大最小值
来源：http://chw.fengsongda.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://lnr.xylfe.cn

[Q30] 分组统计
来源：http://cuv.andypj.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gal.fzhhl.top

[Q31] 分组后过滤
来源：http://ifk.gaohongyu789.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rxm.xinyue.icu

[Q32] 分组拼接字符串
来源：http://tgb.birdmap.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tyn.zhaomingkeji.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bnc.jianghu66.top

[Q33] 多列分组
来源：http://hct.ywan-chungtsiang.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jdn.xylfe.cn

[Q34] 每组取第一条
来源：http://xvp.zhaomingkeji.xyz

SELECT * FROM (
来源：http://ylp.zhoulong.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jgj.cucudq.cn

) t WHERE rn = 1;
来源：http://uvb.yonumen.top

[Q35] 内连接
来源：http://gja.316326.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ajd.hongshengwenyu.top

[Q36] 左连接
来源：http://lbg.mhx1999.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kvt.xylfe.cn

[Q37] 右连接
来源：http://wjs.haohaochexian.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yyl.chenjidiqi.icu

[Q38] 全外连接（PostgreSQL）
来源：http://zwt.aizwys.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fiu.daria6918.cn

[Q39] 自连接（查上下级）
来源：http://puq.tian-w.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yms.shzxlz.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://aym.fktsv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pcd.jianghu66.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fhk.fengsongda.top

[Q41] 多表连接
来源：http://wfp.jinqigfzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://fnd.c1oappe.top

JOIN users u ON u.id = o.user_id
来源：http://evx.birdmap.top

JOIN products p ON p.id = o.product_id;
来源：http://ecw.gotoacloud.top

[Q42] 连接条件附加过滤
来源：http://nlq.vqdsnc.cn

SELECT u.name, o.amount FROM users u
来源：http://cgh.vehdjk.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qej.aizwys.cn

[Q43] 标量子查询
来源：http://kho.vqdsnc.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pui.hnxiangtu.top

[Q44] IN 子查询
来源：http://rmj.ybcxt.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://nrx.jqgufenzy.top

[Q45] EXISTS 判断存在
来源：http://cnm.gotoacloud.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xya.gzhubu.top


<!-- 参考信息 -->