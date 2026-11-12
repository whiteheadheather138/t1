代发 wailian999

Go:   // 手写 map[int]int
来源：http://uhx.fehbvm.com

Ruby: // 手写 Hash
来源：http://fba.ydzc1.top

C#:   // 手写 Dictionary<int, int>
来源：http://hbc.dashuyun.cn

[N08] 生成全排列
来源：http://uug.aizwys.cn

Py:   itertools.permutations(arr)
来源：http://ctu.yueranfly.top

PHP:  // 手写递归交换
来源：http://ogb.hfpthk.cn

JS:   // 手写回溯递归
来源：http://gbn.fanxiaobao.xyz

TS:   // 手写回溯递归
来源：http://fyi.cheryme.top

Java: // 手写回溯递归
来源：http://acn.jianghu66.top

Go:   // 手写回溯递归
来源：http://sso.jinyuanbaomall.cn

Ruby: arr.permutation.to_a
来源：http://lrz.hcnkem.com

C#:   // 手写回溯递归
来源：http://ypd.kuanghao11.cn

[N09] 栈与队列
来源：http://thy.hongshengwenyu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lsd.hammf.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rmm.zdbjq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lka.jiagoushi.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ckm.chenlongwang.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://anj.daxiang520.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yvp.birdmap.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uwl.epnwcf.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vqo.cheryme.top

[N10] 链表节点定义
来源：http://nxq.yj202588.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rqj.ydzc1.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mkx.meibo888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://txu.daria6918.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vtl.cashguo.top

Java: class Node { int v; Node next; }
来源：http://gma.mhx1999.top

Go:   type Node struct { V int; Next *Node }
来源：http://ezk.hnxiangtu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://xch.yuanzhike.top

C#:   class Node { public int V; public Node? Next; }
来源：http://gim.dianchejie.cn

[N11] 二叉树中序遍历
来源：http://cib.yuxming.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fgt.jinqigufen.top

PHP:  // 手写递归函数
来源：http://qgq.jinyuanbaomall.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://npf.uphjek.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://utd.havefunace.top

Java: // 手写递归
来源：http://wzv.zycfv.cn

Go:   // 手写递归
来源：http://ymt.shanyushiyangtech.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dhh.shzxlz.cn

C#:   // 手写递归
来源：http://vbd.chenzaomai.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zpp.chenjidiqi.icu

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mas.haohaochexian.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oly.epnwcf.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mqc.nanxuanxn.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bqo.0kj1m.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ztt.cdnleiting.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lft.yongpay.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ppw.yangfankeji.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://glb.svipenyu.cn

================================================================================
来源：http://ayb.fehbvm.com

O. 并发与异步
来源：http://hlg.yj20258.top

================================================================================
来源：http://vmd.pengpengdd.cyou

[O01] 启动一个线程
来源：http://rzx.jinqigfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dro.vqdsnc.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jyw.yanxiufei.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bsz.aizwys.cn

TS:   // 同 JS
来源：http://oga.jianghu66.top

Java: new Thread(() -> f()).start()
来源：http://vak.jianghu66.top

Go:   go f()
来源：http://mel.yfazqb.com

Ruby: Thread.new { f }
来源：http://mhs.iojbl.cn

C#:   Task.Run(() => F());
来源：http://tbr.xingfuxueyuan.xyz

[O02] 使用线程池
来源：http://jhu.316326.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xun.yj20258.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bhw.sysykeji.top

JS:   // worker_threads 线程池
来源：http://jiu.jiagoushi.top

TS:   // worker_threads 线程池
来源：http://vty.cqqwz.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gyz.bbcook.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lfe.yj20258.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qqg.bbcook.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yry.jlsjyb.cn

[O03] 加锁保护共享数据
来源：http://foo.sweek.top

Py:   with lock: shared += 1
来源：http://fed.ydzc1.top

PHP:  // 用 flock() 做文件锁
来源：http://ext.hcnkem.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ijp.tian-w.cn

TS:   // 同 JS
来源：http://cxe.nanxuanxn.top

Java: synchronized (this) { shared++; }
来源：http://mem.yongpay.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vfc.xingfuxueyuan.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://dqf.vqdsnc.cn

C#:   lock (gate) { shared++; }
来源：http://hrc.guannengcc.top

[O04] 定义异步函数并等待
来源：http://ypn.jinghuilouyu.cn

Py:   async def f():⏎    await g()
来源：http://kmc.meibo888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://csf.yanxiufei.cn

JS:   async function f() { await g(); }
来源：http://jfy.gzhubu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://bbp.smart0.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://psg.ehwqpu.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qrl.hesvh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://vkl.bjfxy.top

C#:   async Task F() { await G(); }
来源：http://amm.hywenlv.cn

[O05] 并发执行并等待全部完成
来源：http://eva.yangfankeji.com

Py:   asyncio.gather(*tasks)
来源：http://gxm.guannengcc.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://eiq.sysykeji.top

JS:   await Promise.all(tasks)
来源：http://btj.sweek.top

TS:   await Promise.all(tasks)
来源：http://jgz.shangyingyoupin.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fzb.sufxvd.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oor.ivvv.top

Ruby: threads.map(&:join)
来源：http://hie.feifeiyinyue.top

C#:   await Task.WhenAll(t1, t2)
来源：http://avs.pycfn.com

[O06] 使用进程池
来源：http://gxe.vehdjk.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vbl.hnqzz.top

PHP:  // pcntl_fork 或多进程队列
来源：http://rrv.fengsongda.top

JS:   // child_process / cluster 模块
来源：http://ils.ydjk.org.cn

TS:   // child_process / cluster 模块
来源：http://ger.havefunace.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tjy.nwbrower.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ioc.meibo888.top

Ruby: // fork 块
来源：http://mlf.uphjek.com

C#:   Parallel.For
来源：http://lmv.dashuyun.cn

================================================================================
来源：http://jhs.tianlin.xyz

P. 常用工具函数
来源：http://aay.jinqigfzy.top

================================================================================
来源：http://bmw.haohaochexian.top

[P01] 生成 UUID
来源：http://jqi.hysaishi.cn

Py:   str(uuid.uuid4())
来源：http://dcw.feifeiyinyue.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://iks.xziqi.cn

JS:   crypto.randomUUID()
来源：http://ekw.nanxinkj.top

TS:   crypto.randomUUID()
来源：http://gox.jqgfzy.top

Java: UUID.randomUUID().toString()
来源：http://amj.vqdsnc.cn

Go:   // 用 github.com/google/uuid
来源：http://tof.0kj1m.cn

Ruby: SecureRandom.uuid
来源：http://aer.fzhhl.top

C#:   Guid.NewGuid().ToString()
来源：http://szn.hcnkem.com

[P02] MD5 / SHA256 摘要
来源：http://hlj.gogol.net.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zuy.jlsjyb.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://knx.aibaodan.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tsr.chenzaomai.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ght.hnxiangtu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vls.sufxvd.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ttp.gaohongyu789.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kht.wangshuangyany.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tfs.zycfv.cn

[P03] 生成短随机字符串
来源：http://hbt.ehwqpu.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://aco.svipenyu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hyu.52xcode.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xyt.jiagoushi.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vwj.chenjidiqi.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bof.9152youxi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wmr.yj20258.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://wda.jinqigufen.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dra.jinqigufen.top

[P04] 求长度
来源：http://aws.jiagoushi.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mwz.zhengqikj.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vlc.aizwys.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lgp.hongshengwenyu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kuc.iojbl.cn

Java: list.size();  map.size();  s.length()
来源：http://pkb.yj20258888.top

Go:   len(arr);  len(m)
来源：http://tgt.jianghu66.top

Ruby: x.length;  x.size
来源：http://wmo.sweek.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://hdm.hywenlv.cn

[P05] 判断两个对象内容是否相等
来源：http://qgb.xylfe.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gta.jinqigufen.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://iby.yangfankeji.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://psw.fehbvm.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hls.jinghuilouyu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://osx.bjfxy.top

Go:   reflect.DeepEqual(a, b)
来源：http://gbb.hongshengwenyu.top

Ruby: a == b
来源：http://uqn.tanke756.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jef.tian-w.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://avd.nwbrower.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://swp.zhoulong.xyz

PHP:  if (empty($x)) {}
来源：http://quz.kuanghao11.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xax.zhiwuduotai.top

TS:   if (x == null) {}
来源：http://jnz.hongshengwenyu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://hwr.fzhhl.top

Go:   if x == nil {}
来源：http://qny.ydzc1.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xmy.ppjwa.cn

C#:   if (x is null) {}
来源：http://gkq.hywenlv.cn

[P07] 防抖与节流
来源：http://lsq.ctjpmb.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://put.zhaomingkeji.xyz

PHP:  // 手写时间戳比较
来源：http://lmm.9152youxi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vfm.hesvh.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ckx.fehbvm.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xqn.jinghuilouyu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tkb.yueranfly.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://tvg.jqgfzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ddo.pengpengdd.cyou

[P08] 处理浮点精度问题
来源：http://vir.epnwcf.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rhi.bbcook.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://orl.yuanzhike.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vua.feifeiyinyue.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fea.aizwys.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xiy.yvedp.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://knc.yongpay.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rog.jqgfzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fvz.wangshuangyany.cn

================================================================================
来源：http://dkc.jqgfzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jfl.cdnleiting.top

================================================================================
来源：http://jhv.xuetiantiany.cn

[Q01] 创建表
来源：http://zau.xinyue.icu

CREATE TABLE users (
来源：http://ywh.yangfankeji.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tbo.aibaodan.cn

name VARCHAR(50) NOT NULL,
来源：http://jhi.guannengcc.top

email VARCHAR(100) UNIQUE,
来源：http://lmo.aizwys.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://etb.cheryme.top

);
来源：http://roj.vqdsnc.cn

[Q02] 创建带外键的表
来源：http://xjz.chenjidiqi.icu

CREATE TABLE orders (
来源：http://doo.nanxuanxn.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://unc.kuanghao11.cn

user_id INT NOT NULL,
来源：http://cbb.iojbl.cn

amount DECIMAL(10, 2),
来源：http://kff.chenzaomai.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vba.daxiang520.top

);
来源：http://rxc.tarul.cn

[Q03] 增加列
来源：http://pez.nanxinkj.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sjc.ybcxt.top

[Q04] 修改列类型
来源：http://oxh.birdmap.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ryf.zhijiandao.cn

[Q05] 重命名列
来源：http://nzv.redwolf501.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cwr.ywan-chungtsiang.top

[Q06] 删除列
来源：http://iib.bjfxy.top

ALTER TABLE users DROP COLUMN age;
来源：http://daw.daxiang520.top

[Q07] 删除表
来源：http://ueo.316326.xyz

DROP TABLE IF EXISTS orders;
来源：http://hed.ybcxt.top

[Q08] 创建普通索引
来源：http://zsx.0kj1m.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rue.daria6918.cn

[Q09] 创建唯一索引
来源：http://ifm.ybcxt.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ava.gogol.net.cn

[Q10] 插入单行
来源：http://ufz.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ole.ctjpmb.com

[Q11] 一次插入多行
来源：http://oqo.uphjek.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://koz.fengsongda.top

[Q12] 插入后取自增 ID
来源：http://nls.sweek.top

INSERT INTO users (name) VALUES ('C');
来源：http://dbz.xingfuxueyuan.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ihp.hnqzz.top

[Q13] 忽略重复插入
来源：http://zyy.sysykeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bem.zhengqikj.top

[Q14] 存在则更新（upsert）
来源：http://nkq.shuidangran.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yvp.jinqigfzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sol.cqqwz.cn

[Q15] 查询全部
来源：http://ojy.cqqwz.cn

SELECT * FROM users;
来源：http://vjm.bbcook.cn

[Q16] 查询指定列
来源：http://kgl.chenlongwang.top

SELECT id, name FROM users;
来源：http://hfr.zhiwuduotai.top

[Q17] 条件查询
来源：http://jjb.shanyushiyangkeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://esf.meibo888.top

[Q18] 模糊匹配
来源：http://den.yangfankeji.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://epr.hywenlv.cn

[Q19] 范围查询
来源：http://fci.dashuyun.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lyg.vqdsnc.cn

[Q20] IN 列表
来源：http://dqa.fzhhl.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nkz.sysykeji.top

[Q21] 空值判断
来源：http://afg.yanxiufei.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zad.mhx1999.top

[Q22] 排序
来源：http://vma.hesvh.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ssu.jyoumei.cn

[Q23] 分页
来源：http://mtb.fzhhl.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zol.mhx1999.top

[Q24] 去重
来源：http://zjn.xingfuxueyuan.xyz

SELECT DISTINCT city FROM users;
来源：http://yxp.pengpengdd.cyou

[Q25] 只取前 N 条
来源：http://fum.zycfv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ova.ydjk.org.cn

[Q26] 计数
来源：http://ycs.cdnleiting.top

SELECT COUNT(*) FROM users;
来源：http://sgj.yueranfly.top

[Q27] 条件计数
来源：http://nkc.zhijiandao.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://whl.haohaochexian.top

[Q28] 求和与平均
来源：http://ajm.snrcjt.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sdb.guowangkeji.top

[Q29] 最大最小值
来源：http://fsp.hcnkem.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://avq.bbcook.cn

[Q30] 分组统计
来源：http://uet.daria6918.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fcj.aizwys.cn

[Q31] 分组后过滤
来源：http://noq.xuetiantiany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zni.sjlbkw.cn

[Q32] 分组拼接字符串
来源：http://ydo.tian-w.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yen.xziqi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gcw.sxryk.cn

[Q33] 多列分组
来源：http://acb.zhoulong.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mrc.wangdashe.top

[Q34] 每组取第一条
来源：http://krk.shzxlz.cn

SELECT * FROM (
来源：http://dif.yongpay.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wmg.yueranfly.top

) t WHERE rn = 1;
来源：http://yyx.yj20258888.top

[Q35] 内连接
来源：http://due.gogol.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vao.gogol.net.cn

[Q36] 左连接
来源：http://nmq.tarul.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jpy.guowangkeji.top

[Q37] 右连接
来源：http://mgv.zhixingplan.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://whx.hnqzz.top

[Q38] 全外连接（PostgreSQL）
来源：http://pei.tarul.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gqw.dianchejie.cn

[Q39] 自连接（查上下级）
来源：http://mef.kuanghao11.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bfu.shanyushiyangtech.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rii.316326.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://znm.aizwys.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ivs.shanyushiyangkeji.top

[Q41] 多表连接
来源：http://rgy.fengsongda.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://itu.vqdsnc.cn

JOIN users u ON u.id = o.user_id
来源：http://xiz.yongpay.top

JOIN products p ON p.id = o.product_id;
来源：http://eyn.aizwys.cn

[Q42] 连接条件附加过滤
来源：http://xjn.bjfxy.top

SELECT u.name, o.amount FROM users u
来源：http://zbh.fanxiaobao.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yyq.haohaochexian.top

[Q43] 标量子查询
来源：http://qvf.jinyuanbaomall.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://key.hongshengwenyu.top

[Q44] IN 子查询
来源：http://tza.xuetiantiany.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://izb.zycfv.cn

[Q45] EXISTS 判断存在
来源：http://fuo.yonumen.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ehk.andypj.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://vnw.zhongyouzk.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://azc.tian-w.cn

[Q47] 与平均值比较
来源：http://fhi.shanyushiyangtech.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://eew.shanyushiyangtech.top

[Q48] CTE 公用表表达式
来源：http://gpl.nanxuanxn.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://veg.hnxiangtu.top

SELECT * FROM t WHERE c > 5;
来源：http://jtn.uphjek.com

[Q49] 更新单行
来源：http://aqz.xinyue.icu


<!-- 参考信息 -->