代发 wailian999

Ruby: s == s.reverse
来源：http://pgz.nanxinkj.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://uac.tanke756.top

[N07] 两数之和（返回下标）
来源：http://ikd.tian-w.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sfh.fanxiaobao.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fry.yj20258888.top

JS:   // 手写 Map：map.set(v, i)
来源：http://nmh.52xcode.cn

TS:   // 手写 Map<string, number>
来源：http://lfg.fengsongda.top

Java: // 手写 HashMap
来源：http://jym.jinqigfzy.top

Go:   // 手写 map[int]int
来源：http://dpx.feifeiyinyue.top

Ruby: // 手写 Hash
来源：http://pub.gaohongyu789.top

C#:   // 手写 Dictionary<int, int>
来源：http://nsv.yanxiufei.cn

[N08] 生成全排列
来源：http://sue.tian-w.cn

Py:   itertools.permutations(arr)
来源：http://grt.gogol.net.cn

PHP:  // 手写递归交换
来源：http://yys.jinghuilouyu.cn

JS:   // 手写回溯递归
来源：http://iqo.redwolf501.top

TS:   // 手写回溯递归
来源：http://mcm.sufxvd.cn

Java: // 手写回溯递归
来源：http://fgn.vehdjk.com

Go:   // 手写回溯递归
来源：http://gyk.fanxiaobao.xyz

Ruby: arr.permutation.to_a
来源：http://aum.pengpengdd.cyou

C#:   // 手写回溯递归
来源：http://qji.yvedp.cn

[N09] 栈与队列
来源：http://dxd.0kj1m.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xln.zdqjudy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jts.xuetiantiany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qkp.yongpay.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://unj.jlsjyb.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hdh.jyoumei.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nbv.andypj.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ewu.hesvh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://anb.xingfuxueyuan.xyz

[N10] 链表节点定义
来源：http://eyw.xinyue.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hgh.jqgufenzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ntx.sysykeji.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xyf.yvedp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cyq.yueranfly.top

Java: class Node { int v; Node next; }
来源：http://xde.wangshuangyany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ewa.jqgfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://vjm.jinqigfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bfv.yanxiufei.cn

[N11] 二叉树中序遍历
来源：http://gpc.jqgufenzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kvr.316326.xyz

PHP:  // 手写递归函数
来源：http://lcx.jinqigfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vgr.hesvh.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lws.yj20258.top

Java: // 手写递归
来源：http://zrq.shuidangran.top

Go:   // 手写递归
来源：http://fqh.shanyushiyangkeji.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xqb.fehbvm.com

C#:   // 手写递归
来源：http://tyl.ctjpmb.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jqv.vehdjk.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tvq.feifeiyinyue.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gkg.jianghu66.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://llk.xuanzx.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vyv.yueranfly.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://moc.guannengcc.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kge.jinqigfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sdm.yueranfly.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fia.yongpay.top

================================================================================
来源：http://idv.cqqwz.cn

O. 并发与异步
来源：http://dza.dashuyun.cn

================================================================================
来源：http://dvj.snrcjt.cn

[O01] 启动一个线程
来源：http://zns.0kj1m.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ryr.fzhhl.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pvd.nwbrower.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hqt.xylfe.cn

TS:   // 同 JS
来源：http://lua.chenlongwang.top

Java: new Thread(() -> f()).start()
来源：http://lkk.yj20258888.top

Go:   go f()
来源：http://alg.hongshengwenyu.top

Ruby: Thread.new { f }
来源：http://yxk.xylfe.cn

C#:   Task.Run(() => F());
来源：http://ynd.gotoacloud.top

[O02] 使用线程池
来源：http://upl.nanxuanxn.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://stn.andypj.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://czc.vqdsnc.cn

JS:   // worker_threads 线程池
来源：http://nps.52xcode.cn

TS:   // worker_threads 线程池
来源：http://scs.ydjk.org.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ixo.sweek.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lys.jinqigfzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rba.nanxinkj.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mpc.ctjpmb.com

[O03] 加锁保护共享数据
来源：http://trl.dashuyun.cn

Py:   with lock: shared += 1
来源：http://lnd.tian-w.cn

PHP:  // 用 flock() 做文件锁
来源：http://qhg.guowangkeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rkg.haohaochexian.top

TS:   // 同 JS
来源：http://obh.mhx1999.top

Java: synchronized (this) { shared++; }
来源：http://fku.hcnkem.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wwb.jianghu66.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ecp.hongshengwenyu.top

C#:   lock (gate) { shared++; }
来源：http://lra.yueranfly.top

[O04] 定义异步函数并等待
来源：http://zgy.316326.xyz

Py:   async def f():⏎    await g()
来源：http://rrn.zhaomingkeji.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://slm.hysaishi.cn

JS:   async function f() { await g(); }
来源：http://vqs.ctjpmb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://tdw.shzxlz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rkh.ydzc1.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mdz.hesvh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wze.zhoulong.xyz

C#:   async Task F() { await G(); }
来源：http://xhm.bbcook.cn

[O05] 并发执行并等待全部完成
来源：http://equ.zhongyouzk.top

Py:   asyncio.gather(*tasks)
来源：http://wic.bbcook.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wxx.pycfn.com

JS:   await Promise.all(tasks)
来源：http://mwn.fengsongda.top

TS:   await Promise.all(tasks)
来源：http://vsr.jlsjyb.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nko.tianlin.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pek.meibo888.top

Ruby: threads.map(&:join)
来源：http://bbt.haohaochexian.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fot.jlsjyb.cn

[O06] 使用进程池
来源：http://syj.guannengcc.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cyq.fktsv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zky.chenlongwang.top

JS:   // child_process / cluster 模块
来源：http://nra.ctjpmb.com

TS:   // child_process / cluster 模块
来源：http://lgq.wangshuangyany.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fia.hammf.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zpm.shanyushiyangtech.top

Ruby: // fork 块
来源：http://lnt.gaohongyu789.top

C#:   Parallel.For
来源：http://mpb.yj20258.top

================================================================================
来源：http://www.yvedp.cn

P. 常用工具函数
来源：http://mmn.jinqigufen.top

================================================================================
来源：http://jxc.jlsjyb.cn

[P01] 生成 UUID
来源：http://dtk.yfazqb.com

Py:   str(uuid.uuid4())
来源：http://pyg.yonumen.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ldj.jiagoushi.top

JS:   crypto.randomUUID()
来源：http://xha.hammf.cn

TS:   crypto.randomUUID()
来源：http://vie.shanyushiyangtech.top

Java: UUID.randomUUID().toString()
来源：http://gae.uphjek.com

Go:   // 用 github.com/google/uuid
来源：http://byd.hcnkem.com

Ruby: SecureRandom.uuid
来源：http://eze.jiagoushi.top

C#:   Guid.NewGuid().ToString()
来源：http://bbi.mhx1999.top

[P02] MD5 / SHA256 摘要
来源：http://ono.dianchejie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lut.yj20258.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://mcu.wangshuangyany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hmv.hywenlv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rmt.hfpthk.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rfk.shanyushiyangtech.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hqu.yj20258.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jpm.shzxlz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mku.9152youxi.cn

[P03] 生成短随机字符串
来源：http://gfd.sysykeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ubp.shangyingyoupin.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lok.chenlongwang.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ttl.shangyingyoupin.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lct.bjfxy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lzu.sweek.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ipx.shzxlz.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jgt.hesvh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://squ.jiagoushi.top

[P04] 求长度
来源：http://ibz.tarul.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qsl.meibo888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hfo.xinyue.icu

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ztw.dianchejie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qol.jinyuanbaomall.cn

Java: list.size();  map.size();  s.length()
来源：http://xwd.sweek.top

Go:   len(arr);  len(m)
来源：http://xkg.zhongyouzk.top

Ruby: x.length;  x.size
来源：http://zwo.guowangkeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://yib.hammf.cn

[P05] 判断两个对象内容是否相等
来源：http://dig.meibo888.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ajd.birdmap.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kaz.zdbjq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dga.vqdsnc.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mmf.cheryme.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://iuc.mhx1999.top

Go:   reflect.DeepEqual(a, b)
来源：http://usc.hfpthk.cn

Ruby: a == b
来源：http://ifd.xziqi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xfp.zhixingplan.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ilp.zhoulong.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qjg.nwbrower.top

PHP:  if (empty($x)) {}
来源：http://cam.ydjk.org.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wor.xuanzx.com

TS:   if (x == null) {}
来源：http://dby.52xcode.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lmy.jyoumei.cn

Go:   if x == nil {}
来源：http://jcc.xingfuxueyuan.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rtm.cdnleiting.top

C#:   if (x is null) {}
来源：http://mxz.xingfuxueyuan.xyz

[P07] 防抖与节流
来源：http://tqm.yangfankeji.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hoq.yvedp.cn

PHP:  // 手写时间戳比较
来源：http://hhr.yvedp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ycp.wangshuangyany.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fie.ctjpmb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://epp.ybcxt.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dli.aibaodan.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://leo.xingfuxueyuan.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dzn.ppjwa.cn

[P08] 处理浮点精度问题
来源：http://iwj.ybcxt.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wrf.ivvv.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://edb.havefunace.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cjp.ivvv.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://loo.jiagoushi.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ypf.nanxinkj.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://luc.yuanzhike.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://leb.mhx1999.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wxu.zhixingplan.top

================================================================================
来源：http://gjm.yuxming.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://knu.snrcjt.cn

================================================================================
来源：http://yuu.shuidangran.top

[Q01] 创建表
来源：http://qrl.c1oappe.top

CREATE TABLE users (
来源：http://gyf.iojbl.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jgr.smart0.xyz

name VARCHAR(50) NOT NULL,
来源：http://lgz.shanyushiyangtech.top

email VARCHAR(100) UNIQUE,
来源：http://bnu.kuanghao11.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zcu.yongpay.top

);
来源：http://iew.xinyue.icu

[Q02] 创建带外键的表
来源：http://kil.yj20258.top

CREATE TABLE orders (
来源：http://qgg.mhx1999.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jjo.chenjidiqi.icu

user_id INT NOT NULL,
来源：http://dac.gzhubu.top

amount DECIMAL(10, 2),
来源：http://kax.zycfv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ajl.yongpay.top

);
来源：http://yuy.havefunace.top

[Q03] 增加列
来源：http://yzw.jqgufenzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zxg.gogol.net.cn

[Q04] 修改列类型
来源：http://kgo.fzhhl.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pjg.yj20258.top

[Q05] 重命名列
来源：http://gvp.cdnleiting.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dkh.xziqi.cn

[Q06] 删除列
来源：http://kqu.c1oappe.top

ALTER TABLE users DROP COLUMN age;
来源：http://fqk.shuidangran.top

[Q07] 删除表
来源：http://pvk.dashuyun.cn

DROP TABLE IF EXISTS orders;
来源：http://bai.sysykeji.top

[Q08] 创建普通索引
来源：http://lye.ybcxt.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xbs.shzxlz.cn

[Q09] 创建唯一索引
来源：http://svq.jinyuanbaomall.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gyq.shangyingyoupin.top

[Q10] 插入单行
来源：http://xlh.jinyuanbaomall.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kwj.shangyingyoupin.top

[Q11] 一次插入多行
来源：http://dvb.9152youxi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fvw.wangdashe.top

[Q12] 插入后取自增 ID
来源：http://zwa.mhx1999.top

INSERT INTO users (name) VALUES ('C');
来源：http://cfd.c1oappe.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fga.zhaomingkeji.xyz

[Q13] 忽略重复插入
来源：http://qzf.epnwcf.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://okx.yueranfly.top

[Q14] 存在则更新（upsert）
来源：http://dem.jinqigfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rzg.yuanzhike.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tmd.zhijiandao.cn

[Q15] 查询全部
来源：http://axe.yvedp.cn

SELECT * FROM users;
来源：http://ztl.ehwqpu.com

[Q16] 查询指定列
来源：http://kmf.shuidangran.top

SELECT id, name FROM users;
来源：http://brv.shzxlz.cn

[Q17] 条件查询
来源：http://hoa.fehbvm.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rbn.cucudq.cn

[Q18] 模糊匹配
来源：http://fzp.daria6918.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nqy.sjlbkw.cn

[Q19] 范围查询
来源：http://rih.hywenlv.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vfe.ydzc1.top

[Q20] IN 列表
来源：http://qiq.tian-w.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zmc.ivvv.top

[Q21] 空值判断
来源：http://bhx.fengsongda.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ubk.cucudq.cn

[Q22] 排序
来源：http://fsz.snrcjt.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hrb.smart0.xyz

[Q23] 分页
来源：http://itd.zhixingplan.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rec.meibo888.top

[Q24] 去重
来源：http://btu.wangshuangyany.cn

SELECT DISTINCT city FROM users;
来源：http://hhn.xuetiantiany.cn

[Q25] 只取前 N 条
来源：http://uvl.jlsjyb.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zau.hnxiangtu.top

[Q26] 计数
来源：http://ony.aibaodan.cn

SELECT COUNT(*) FROM users;
来源：http://hud.bjfxy.top

[Q27] 条件计数
来源：http://ain.vehdjk.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://huv.yj202588.top

[Q28] 求和与平均
来源：http://zzo.wangdashe.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://php.yj20258888.top

[Q29] 最大最小值
来源：http://yoi.zhoulong.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://kaq.redwolf501.top

[Q30] 分组统计
来源：http://eyw.bjfxy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lvw.9152youxi.cn

[Q31] 分组后过滤
来源：http://tsp.wangshuangyany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://grw.bbcook.cn

[Q32] 分组拼接字符串
来源：http://jwd.cqqwz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ltr.cdnleiting.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bzv.316326.xyz

[Q33] 多列分组
来源：http://unc.shzxlz.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wsm.aibaodan.cn

[Q34] 每组取第一条
来源：http://hyg.shuidangran.top

SELECT * FROM (
来源：http://ykm.shanyushiyangkeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hhp.yonumen.top

) t WHERE rn = 1;
来源：http://gax.dianchejie.cn

[Q35] 内连接
来源：http://qon.sweek.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fnb.nanxinkj.top

[Q36] 左连接
来源：http://ewo.svipenyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vrw.xuetiantiany.cn

[Q37] 右连接
来源：http://ohe.zycfv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jxc.yj20258.top

[Q38] 全外连接（PostgreSQL）
来源：http://wpr.hywenlv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://onp.jqgufenzy.top

[Q39] 自连接（查上下级）
来源：http://eny.jinqigfzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://vzf.ehwqpu.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ymi.jyoumei.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dor.chenzaomai.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qxv.yj202588.top

[Q41] 多表连接
来源：http://aid.ydzc1.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://gdn.xuetiantiany.cn

JOIN users u ON u.id = o.user_id
来源：http://ymd.yj20258888.top

JOIN products p ON p.id = o.product_id;
来源：http://amy.yj202588.top

[Q42] 连接条件附加过滤
来源：http://jze.havefunace.top

SELECT u.name, o.amount FROM users u
来源：http://ngn.zhijiandao.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tmw.shanyushiyangtech.top

[Q43] 标量子查询
来源：http://tdy.guowangkeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jkg.jqgufenzy.top

[Q44] IN 子查询
来源：http://vrw.chenjidiqi.icu

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xli.yuanzhike.top

[Q45] EXISTS 判断存在
来源：http://ceo.ydjk.org.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pjs.xingfuxueyuan.xyz


<!-- 参考信息 -->