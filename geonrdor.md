代发 wailian999

Ruby: s == s.reverse
来源：http://pyh.yfazqb.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://nmr.zhoulong.xyz

[N07] 两数之和（返回下标）
来源：http://sfo.fanxiaobao.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vcd.hysaishi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yyc.zycfv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://tmk.sweek.top

TS:   // 手写 Map<string, number>
来源：http://fqi.yuxming.cn

Java: // 手写 HashMap
来源：http://cus.jqgufenzy.top

Go:   // 手写 map[int]int
来源：http://gyt.chenjidiqi.icu

Ruby: // 手写 Hash
来源：http://fea.zhijiandao.cn

C#:   // 手写 Dictionary<int, int>
来源：http://uux.fktsv.cn

[N08] 生成全排列
来源：http://smw.jianghu66.top

Py:   itertools.permutations(arr)
来源：http://qun.jinqigfzy.top

PHP:  // 手写递归交换
来源：http://zyp.zdbjq.cn

JS:   // 手写回溯递归
来源：http://rob.hcnkem.com

TS:   // 手写回溯递归
来源：http://knw.tianlin.xyz

Java: // 手写回溯递归
来源：http://dtu.yuanzhike.top

Go:   // 手写回溯递归
来源：http://nbv.jinqigfzy.top

Ruby: arr.permutation.to_a
来源：http://few.yonumen.top

C#:   // 手写回溯递归
来源：http://htt.yangfankeji.com

[N09] 栈与队列
来源：http://mfh.ctjpmb.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cik.0kj1m.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://buo.jinghuilouyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kbj.yueranfly.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://njz.jlsjyb.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ayt.cheryme.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://apm.hnqzz.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dyv.tanke756.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://erz.zhiwuduotai.top

[N10] 链表节点定义
来源：http://vat.sysykeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qbo.cdnleiting.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ezs.jqgufenzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ptd.shuidangran.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nwd.chenlongwang.top

Java: class Node { int v; Node next; }
来源：http://iby.daria6918.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fvl.gaohongyu789.top

Ruby: Node = Struct.new(:v, :next)
来源：http://vyg.sxryk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hpt.zhengqikj.top

[N11] 二叉树中序遍历
来源：http://xgb.ivvv.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://njy.yueranfly.top

PHP:  // 手写递归函数
来源：http://lzc.zhixingplan.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xyt.jinyuanbaomall.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://who.chenlongwang.top

Java: // 手写递归
来源：http://ufq.nanxuanxn.top

Go:   // 手写递归
来源：http://fws.guannengcc.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ibr.pycfn.com

C#:   // 手写递归
来源：http://jwr.guowangkeji.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://abi.cheryme.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mya.c1oappe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://elg.zhoulong.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xdk.hesvh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tsq.gotoacloud.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dej.chenlongwang.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ycu.aizwys.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ntm.zdbjq.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jgh.nanxuanxn.top

================================================================================
来源：http://oon.52xcode.cn

O. 并发与异步
来源：http://rkn.fanxiaobao.xyz

================================================================================
来源：http://xmm.aibaodan.cn

[O01] 启动一个线程
来源：http://pqp.hongshengwenyu.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wld.gaohongyu789.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://urb.ybcxt.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wht.hnxiangtu.top

TS:   // 同 JS
来源：http://acn.pycfn.com

Java: new Thread(() -> f()).start()
来源：http://ajt.bbcook.cn

Go:   go f()
来源：http://yxv.xuanzx.com

Ruby: Thread.new { f }
来源：http://hdr.haohaochexian.top

C#:   Task.Run(() => F());
来源：http://awg.jlsjyb.cn

[O02] 使用线程池
来源：http://dsv.quarkkingdee.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ygj.yuanzhike.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ozq.zycfv.cn

JS:   // worker_threads 线程池
来源：http://fsy.yangfankeji.com

TS:   // worker_threads 线程池
来源：http://tgg.yvedp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gsn.hfpthk.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jej.dianchejie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://awt.chenlongwang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://giu.zhongyouzk.top

[O03] 加锁保护共享数据
来源：http://gis.yuanzhike.top

Py:   with lock: shared += 1
来源：http://bid.andypj.xyz

PHP:  // 用 flock() 做文件锁
来源：http://qts.xziqi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://psi.hesvh.cn

TS:   // 同 JS
来源：http://cwk.shanyushiyangtech.top

Java: synchronized (this) { shared++; }
来源：http://ygl.sufxvd.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lsf.fengsongda.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://umf.jinghuilouyu.cn

C#:   lock (gate) { shared++; }
来源：http://crc.yj20258888.top

[O04] 定义异步函数并等待
来源：http://atz.hammf.cn

Py:   async def f():⏎    await g()
来源：http://gjk.yj20258.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ajp.andypj.xyz

JS:   async function f() { await g(); }
来源：http://fjs.redwolf501.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://dka.pengpengdd.cyou

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kwo.sufxvd.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uvc.haohaochexian.top

Ruby: # 用 Fiber 或 async gem
来源：http://aic.tian-w.cn

C#:   async Task F() { await G(); }
来源：http://vku.gotoacloud.top

[O05] 并发执行并等待全部完成
来源：http://wbt.52xcode.cn

Py:   asyncio.gather(*tasks)
来源：http://njr.daxiang520.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lty.jinghuilouyu.cn

JS:   await Promise.all(tasks)
来源：http://nct.jinyuanbaomall.cn

TS:   await Promise.all(tasks)
来源：http://qgb.redwolf501.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ymt.shzxlz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nhv.uphjek.com

Ruby: threads.map(&:join)
来源：http://khx.yongpay.top

C#:   await Task.WhenAll(t1, t2)
来源：http://kjy.jlsjyb.cn

[O06] 使用进程池
来源：http://vho.yuanzhike.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://itw.jqgfzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://obw.shzxlz.cn

JS:   // child_process / cluster 模块
来源：http://fok.daria6918.cn

TS:   // child_process / cluster 模块
来源：http://cac.gzhubu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rpe.quarkkingdee.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jlj.ppjwa.cn

Ruby: // fork 块
来源：http://byd.ctjpmb.com

C#:   Parallel.For
来源：http://yzw.kuanghao11.cn

================================================================================
来源：http://gth.jqgufenzy.top

P. 常用工具函数
来源：http://rpf.sweek.top

================================================================================
来源：http://vlm.epnwcf.com

[P01] 生成 UUID
来源：http://wgl.kuanghao11.cn

Py:   str(uuid.uuid4())
来源：http://aau.sxryk.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://toq.sufxvd.cn

JS:   crypto.randomUUID()
来源：http://hbx.chenjidiqi.icu

TS:   crypto.randomUUID()
来源：http://vrg.andypj.xyz

Java: UUID.randomUUID().toString()
来源：http://qiq.hysaishi.cn

Go:   // 用 github.com/google/uuid
来源：http://qto.haohaochexian.top

Ruby: SecureRandom.uuid
来源：http://gue.shanyushiyangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://ucl.shuidangran.top

[P02] MD5 / SHA256 摘要
来源：http://zbl.shuidangran.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cfv.wangshuangyany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://szn.chenlongwang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tuh.ydzc1.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dxe.bbcook.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qha.aizwys.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vlq.jqgufenzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ikt.vqdsnc.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hzv.hammf.cn

[P03] 生成短随机字符串
来源：http://vcf.zdqjudy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mud.yonumen.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://eun.zdbjq.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hme.yj20258888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jgl.zhoulong.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yar.cqqwz.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qvw.gzhubu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://qyv.redwolf501.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ren.9152youxi.cn

[P04] 求长度
来源：http://byu.hnqzz.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dtv.jlsjyb.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ssb.chenlongwang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dgj.smart0.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tke.ydzc1.top

Java: list.size();  map.size();  s.length()
来源：http://wro.ivvv.top

Go:   len(arr);  len(m)
来源：http://xpn.jianghu66.top

Ruby: x.length;  x.size
来源：http://ytj.guowangkeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://mop.wangshuangyany.cn

[P05] 判断两个对象内容是否相等
来源：http://xwx.daria6918.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://aso.yj20258888.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pkq.zhongyouzk.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gae.gotoacloud.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cdy.zhijiandao.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zan.ybcxt.top

Go:   reflect.DeepEqual(a, b)
来源：http://blp.xuanzx.com

Ruby: a == b
来源：http://tmr.bbcook.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cdj.hywenlv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wbc.jinqigufen.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fka.yongpay.top

PHP:  if (empty($x)) {}
来源：http://elm.nanxinkj.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gjx.dianchejie.cn

TS:   if (x == null) {}
来源：http://ucv.fengsongda.top

Java: if (x == null || x.isEmpty()) {}
来源：http://rbz.havefunace.top

Go:   if x == nil {}
来源：http://dir.snrcjt.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uju.cucudq.cn

C#:   if (x is null) {}
来源：http://gyf.ywan-chungtsiang.top

[P07] 防抖与节流
来源：http://wxa.jyoumei.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gpr.tanke756.top

PHP:  // 手写时间戳比较
来源：http://sof.sjlbkw.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hlb.tarul.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gzk.tianlin.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qbh.hnxiangtu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ghd.fzhhl.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zsg.zhoulong.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://etq.nanxinkj.top

[P08] 处理浮点精度问题
来源：http://all.hnqzz.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ujs.jinghuilouyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://onr.jyoumei.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://odh.zdbjq.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hvh.jqgufenzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hzy.xziqi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://egs.kuanghao11.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qlq.316326.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://umh.chenjidiqi.icu

================================================================================
来源：http://esx.jqgfzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rhi.hnxiangtu.top

================================================================================
来源：http://vrh.0kj1m.cn

[Q01] 创建表
来源：http://qww.shanyushiyangkeji.top

CREATE TABLE users (
来源：http://kgp.jianghu66.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jxh.jlsjyb.cn

name VARCHAR(50) NOT NULL,
来源：http://efe.hysaishi.cn

email VARCHAR(100) UNIQUE,
来源：http://ayh.nanxuanxn.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gmp.zhixingplan.top

);
来源：http://cxi.snrcjt.cn

[Q02] 创建带外键的表
来源：http://ocy.shanyushiyangkeji.top

CREATE TABLE orders (
来源：http://krb.jiagoushi.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://suw.zhixingplan.top

user_id INT NOT NULL,
来源：http://rno.tanke756.top

amount DECIMAL(10, 2),
来源：http://bbk.haohaochexian.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vug.shuidangran.top

);
来源：http://nvu.fengsongda.top

[Q03] 增加列
来源：http://hio.chenlongwang.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ltr.wangshuangyany.cn

[Q04] 修改列类型
来源：http://itn.yj20258888.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://liu.pycfn.com

[Q05] 重命名列
来源：http://ffw.ybcxt.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jbl.snrcjt.cn

[Q06] 删除列
来源：http://rlv.sxryk.cn

ALTER TABLE users DROP COLUMN age;
来源：http://rjh.svipenyu.cn

[Q07] 删除表
来源：http://pyk.ctjpmb.com

DROP TABLE IF EXISTS orders;
来源：http://kvp.snrcjt.cn

[Q08] 创建普通索引
来源：http://pdq.gaohongyu789.top

CREATE INDEX idx_users_email ON users(email);
来源：http://skt.sysykeji.top

[Q09] 创建唯一索引
来源：http://mmt.zycfv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uhl.birdmap.top

[Q10] 插入单行
来源：http://gmk.hnqzz.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zra.birdmap.top

[Q11] 一次插入多行
来源：http://ish.nanxuanxn.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bcn.aibaodan.cn

[Q12] 插入后取自增 ID
来源：http://xzf.hnxiangtu.top

INSERT INTO users (name) VALUES ('C');
来源：http://ojm.shanyushiyangtech.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fkn.havefunace.top

[Q13] 忽略重复插入
来源：http://ygg.hcnkem.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gdo.shanyushiyangkeji.top

[Q14] 存在则更新（upsert）
来源：http://sxa.hcnkem.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lpg.wangdashe.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sld.uphjek.com

[Q15] 查询全部
来源：http://nec.shangyingyoupin.top

SELECT * FROM users;
来源：http://tjv.smart0.xyz

[Q16] 查询指定列
来源：http://xrs.c1oappe.top

SELECT id, name FROM users;
来源：http://xid.xuanzx.com

[Q17] 条件查询
来源：http://iha.tian-w.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dwm.vehdjk.com

[Q18] 模糊匹配
来源：http://wad.xylfe.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pns.xingfuxueyuan.xyz

[Q19] 范围查询
来源：http://omp.feifeiyinyue.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qar.hesvh.cn

[Q20] IN 列表
来源：http://akb.hysaishi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://toj.zdqjudy.top

[Q21] 空值判断
来源：http://eod.ppjwa.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gch.zdbjq.cn

[Q22] 排序
来源：http://vgx.daxiang520.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pel.jqgufenzy.top

[Q23] 分页
来源：http://kse.guannengcc.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wmg.shuidangran.top

[Q24] 去重
来源：http://heu.hammf.cn

SELECT DISTINCT city FROM users;
来源：http://ldy.zhengqikj.top

[Q25] 只取前 N 条
来源：http://tup.chenzaomai.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bdp.hcnkem.com

[Q26] 计数
来源：http://jsy.yuanzhike.top

SELECT COUNT(*) FROM users;
来源：http://ode.shuidangran.top

[Q27] 条件计数
来源：http://wql.sweek.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vbi.hcnkem.com

[Q28] 求和与平均
来源：http://sxv.dianchejie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tjk.ybcxt.top

[Q29] 最大最小值
来源：http://bai.vqdsnc.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://men.cashguo.top

[Q30] 分组统计
来源：http://ozs.haohaochexian.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qxa.jiagoushi.top

[Q31] 分组后过滤
来源：http://vsu.haohaochexian.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://msn.birdmap.top

[Q32] 分组拼接字符串
来源：http://lhz.yj20258.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tfr.zhoulong.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qrd.yj20258888.top

[Q33] 多列分组
来源：http://dsh.52xcode.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mpq.hywenlv.cn

[Q34] 每组取第一条
来源：http://hzr.fengsongda.top

SELECT * FROM (
来源：http://ppa.jianghu66.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ovy.ctjpmb.com

) t WHERE rn = 1;
来源：http://wsx.aizwys.cn

[Q35] 内连接
来源：http://seb.zhongyouzk.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tpe.hcnkem.com

[Q36] 左连接
来源：http://evp.yj20258888.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://msr.fzhhl.top

[Q37] 右连接
来源：http://wue.hfpthk.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yto.yuxming.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jcw.52xcode.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gur.fzhhl.top

[Q39] 自连接（查上下级）
来源：http://ubz.yj202588.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://tra.smart0.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jqa.yuxming.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mcn.hesvh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://keg.fanxiaobao.xyz

[Q41] 多表连接
来源：http://qnb.zdqjudy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://zhs.yongpay.top

JOIN users u ON u.id = o.user_id
来源：http://fpx.yuxming.cn

JOIN products p ON p.id = o.product_id;
来源：http://zmk.cdnleiting.top

[Q42] 连接条件附加过滤
来源：http://hcs.redwolf501.top

SELECT u.name, o.amount FROM users u
来源：http://ctm.cdnleiting.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wdc.zhaomingkeji.xyz

[Q43] 标量子查询
来源：http://kpx.epnwcf.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fxh.pengpengdd.cyou

[Q44] IN 子查询
来源：http://kht.ybcxt.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://awj.feifeiyinyue.top

[Q45] EXISTS 判断存在
来源：http://hqz.cashguo.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nhn.zhongyouzk.top


<!-- 参考信息 -->