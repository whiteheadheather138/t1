代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rnc.sysykeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://jgq.ivvv.top

TS:   // 手写 Map<string, number>
来源：http://bfn.pengpengdd.cyou

Java: // 手写 HashMap
来源：http://ieb.ybcxt.top

Go:   // 手写 map[int]int
来源：http://xyn.cashguo.top

Ruby: // 手写 Hash
来源：http://nkt.mhx1999.top

C#:   // 手写 Dictionary<int, int>
来源：http://skj.nanxuanxn.top

[N08] 生成全排列
来源：http://dvp.ivvv.top

Py:   itertools.permutations(arr)
来源：http://aqa.ehwqpu.com

PHP:  // 手写递归交换
来源：http://chz.hammf.cn

JS:   // 手写回溯递归
来源：http://pwi.yongpay.top

TS:   // 手写回溯递归
来源：http://lxr.chenlongwang.top

Java: // 手写回溯递归
来源：http://rvt.dashuyun.cn

Go:   // 手写回溯递归
来源：http://pog.epnwcf.com

Ruby: arr.permutation.to_a
来源：http://umr.aibaodan.cn

C#:   // 手写回溯递归
来源：http://mep.xylfe.cn

[N09] 栈与队列
来源：http://ppj.shanyushiyangkeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hkw.gogol.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mcb.xylfe.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kav.dashuyun.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cll.aizwys.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cte.tian-w.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sbo.c1oappe.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://evn.shzxlz.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cuu.hesvh.cn

[N10] 链表节点定义
来源：http://jqq.yonumen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tyd.jinqigfzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://oau.havefunace.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://abd.jinyuanbaomall.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tqn.wangdashe.top

Java: class Node { int v; Node next; }
来源：http://uaq.316326.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://vqy.shanyushiyangtech.top

Ruby: Node = Struct.new(:v, :next)
来源：http://oqv.cucudq.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://uih.hywenlv.cn

[N11] 二叉树中序遍历
来源：http://sod.dashuyun.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cbn.jianghu66.top

PHP:  // 手写递归函数
来源：http://fvz.sxryk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cif.yanxiufei.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xhw.andypj.xyz

Java: // 手写递归
来源：http://ckt.epnwcf.com

Go:   // 手写递归
来源：http://yjp.ivvv.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ddy.feifeiyinyue.top

C#:   // 手写递归
来源：http://qyr.hammf.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cfs.quarkkingdee.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sxr.tanke756.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xkd.sufxvd.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wun.tian-w.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nci.hnqzz.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yzw.dashuyun.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uyi.shanyushiyangkeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iia.zhaomingkeji.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://iym.0kj1m.cn

================================================================================
来源：http://tdd.havefunace.top

O. 并发与异步
来源：http://ljz.shanyushiyangtech.top

================================================================================
来源：http://dqn.hfpthk.cn

[O01] 启动一个线程
来源：http://vjh.quarkkingdee.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nwj.kuanghao11.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vkn.aibaodan.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://plp.fengsongda.top

TS:   // 同 JS
来源：http://xxp.yueranfly.top

Java: new Thread(() -> f()).start()
来源：http://qqt.zhengqikj.top

Go:   go f()
来源：http://hcg.shuidangran.top

Ruby: Thread.new { f }
来源：http://qja.yuanzhike.top

C#:   Task.Run(() => F());
来源：http://rhv.daxiang520.top

[O02] 使用线程池
来源：http://vis.ydjk.org.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vim.hcnkem.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yze.tian-w.cn

JS:   // worker_threads 线程池
来源：http://qwh.jinqigfzy.top

TS:   // worker_threads 线程池
来源：http://tdh.ehwqpu.com

Java: Executors.newFixedThreadPool(4)
来源：http://cjr.bbcook.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://buq.hongshengwenyu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uor.zhengqikj.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://afw.nanxinkj.top

[O03] 加锁保护共享数据
来源：http://vxt.cqqwz.cn

Py:   with lock: shared += 1
来源：http://tfl.jyoumei.cn

PHP:  // 用 flock() 做文件锁
来源：http://fvl.cdnleiting.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ulu.pycfn.com

TS:   // 同 JS
来源：http://osn.jyoumei.cn

Java: synchronized (this) { shared++; }
来源：http://rtb.chenjidiqi.icu

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jar.yonumen.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://yhz.yonumen.top

C#:   lock (gate) { shared++; }
来源：http://rwm.quarkkingdee.top

[O04] 定义异步函数并等待
来源：http://ncw.nwbrower.top

Py:   async def f():⏎    await g()
来源：http://upf.ybcxt.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zax.jqgfzy.top

JS:   async function f() { await g(); }
来源：http://ivr.aizwys.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jlt.yanxiufei.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tgd.chenzaomai.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://shu.fktsv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rti.daria6918.cn

C#:   async Task F() { await G(); }
来源：http://ywc.jinqigufen.top

[O05] 并发执行并等待全部完成
来源：http://atd.feifeiyinyue.top

Py:   asyncio.gather(*tasks)
来源：http://ett.zhaomingkeji.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://eby.haohaochexian.top

JS:   await Promise.all(tasks)
来源：http://kwk.52xcode.cn

TS:   await Promise.all(tasks)
来源：http://ine.zhiwuduotai.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yuh.316326.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jtb.cdnleiting.top

Ruby: threads.map(&:join)
来源：http://pkw.guowangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://pnx.fengsongda.top

[O06] 使用进程池
来源：http://whx.smart0.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vkq.guannengcc.top

PHP:  // pcntl_fork 或多进程队列
来源：http://xfy.gogol.net.cn

JS:   // child_process / cluster 模块
来源：http://iqn.xuetiantiany.cn

TS:   // child_process / cluster 模块
来源：http://dbe.epnwcf.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rkr.xylfe.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hxq.52xcode.cn

Ruby: // fork 块
来源：http://bww.ydzc1.top

C#:   Parallel.For
来源：http://hqe.yuanzhike.top

================================================================================
来源：http://dcy.yvedp.cn

P. 常用工具函数
来源：http://pas.ppjwa.cn

================================================================================
来源：http://uqc.redwolf501.top

[P01] 生成 UUID
来源：http://sks.aizwys.cn

Py:   str(uuid.uuid4())
来源：http://buz.hfpthk.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://beo.zhijiandao.cn

JS:   crypto.randomUUID()
来源：http://gwo.jinqigufen.top

TS:   crypto.randomUUID()
来源：http://ljx.redwolf501.top

Java: UUID.randomUUID().toString()
来源：http://jon.andypj.xyz

Go:   // 用 github.com/google/uuid
来源：http://dsa.gzhubu.top

Ruby: SecureRandom.uuid
来源：http://gok.ctjpmb.com

C#:   Guid.NewGuid().ToString()
来源：http://fwc.ppjwa.cn

[P02] MD5 / SHA256 摘要
来源：http://vxl.wangdashe.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hve.xuetiantiany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://otj.nanxuanxn.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jbe.bjfxy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mqm.andypj.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nhh.hfpthk.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mmr.zhoulong.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oej.uphjek.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uvy.sysykeji.top

[P03] 生成短随机字符串
来源：http://jff.ivvv.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zsd.hammf.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kso.hnqzz.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sjs.sysykeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mta.tanke756.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vgo.xuanzx.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://juh.andypj.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://bvd.bbcook.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nua.hfpthk.cn

[P04] 求长度
来源：http://qsi.smart0.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ypt.sxryk.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hec.bbcook.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ueg.hongshengwenyu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ciw.jinqigufen.top

Java: list.size();  map.size();  s.length()
来源：http://ewc.jinqigfzy.top

Go:   len(arr);  len(m)
来源：http://ljq.dashuyun.cn

Ruby: x.length;  x.size
来源：http://jmp.hywenlv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jth.fktsv.cn

[P05] 判断两个对象内容是否相等
来源：http://bqa.fehbvm.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://jkc.uphjek.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://egr.yuanzhike.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rwl.chenjidiqi.icu

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://luk.ivvv.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ibu.iojbl.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lot.hesvh.cn

Ruby: a == b
来源：http://kzt.ybcxt.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ube.nanxinkj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jin.yueranfly.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://elf.dashuyun.cn

PHP:  if (empty($x)) {}
来源：http://lmm.tianlin.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uzk.feifeiyinyue.top

TS:   if (x == null) {}
来源：http://amh.ctjpmb.com

Java: if (x == null || x.isEmpty()) {}
来源：http://gsy.jianghu66.top

Go:   if x == nil {}
来源：http://leb.jianghu66.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uzz.epnwcf.com

C#:   if (x is null) {}
来源：http://mxo.jqgfzy.top

[P07] 防抖与节流
来源：http://yxp.daxiang520.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tia.iojbl.cn

PHP:  // 手写时间戳比较
来源：http://fzu.zdqjudy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qyl.xylfe.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wlr.hesvh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oky.guannengcc.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nox.havefunace.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ddi.daxiang520.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hyo.kuanghao11.cn

[P08] 处理浮点精度问题
来源：http://rsm.fzhhl.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pik.shzxlz.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wxu.yj20258888.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pjt.hongshengwenyu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xzr.fengsongda.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ndh.zdbjq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qil.sjlbkw.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hwd.hesvh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://csq.zhijiandao.cn

================================================================================
来源：http://wka.jlsjyb.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ytt.shangyingyoupin.top

================================================================================
来源：http://pis.ybcxt.top

[Q01] 创建表
来源：http://jci.cheryme.top

CREATE TABLE users (
来源：http://mly.hywenlv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zti.birdmap.top

name VARCHAR(50) NOT NULL,
来源：http://otj.haohaochexian.top

email VARCHAR(100) UNIQUE,
来源：http://mnj.sxryk.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zpz.guowangkeji.top

);
来源：http://mop.yangfankeji.com

[Q02] 创建带外键的表
来源：http://flt.316326.xyz

CREATE TABLE orders (
来源：http://stv.smart0.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pzt.yj202588.top

user_id INT NOT NULL,
来源：http://nan.zycfv.cn

amount DECIMAL(10, 2),
来源：http://wsz.daria6918.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dcd.yuxming.cn

);
来源：http://rxt.jinghuilouyu.cn

[Q03] 增加列
来源：http://lwo.yangfankeji.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xkq.0kj1m.cn

[Q04] 修改列类型
来源：http://onb.c1oappe.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rix.ywan-chungtsiang.top

[Q05] 重命名列
来源：http://pli.chenzaomai.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://twc.cheryme.top

[Q06] 删除列
来源：http://cca.chenzaomai.com

ALTER TABLE users DROP COLUMN age;
来源：http://ovn.cashguo.top

[Q07] 删除表
来源：http://aal.zhijiandao.cn

DROP TABLE IF EXISTS orders;
来源：http://mkb.meibo888.top

[Q08] 创建普通索引
来源：http://mni.tarul.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wqr.xziqi.cn

[Q09] 创建唯一索引
来源：http://ysf.zhaomingkeji.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://umf.yj20258888.top

[Q10] 插入单行
来源：http://fsy.cashguo.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zau.quarkkingdee.top

[Q11] 一次插入多行
来源：http://eki.zhengqikj.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ign.yj20258.top

[Q12] 插入后取自增 ID
来源：http://nyi.jiagoushi.top

INSERT INTO users (name) VALUES ('C');
来源：http://bpk.vqdsnc.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xvx.aibaodan.cn

[Q13] 忽略重复插入
来源：http://yhf.nwbrower.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pis.svipenyu.cn

[Q14] 存在则更新（upsert）
来源：http://bsa.xziqi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zrd.zhongyouzk.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://laf.yj20258888.top

[Q15] 查询全部
来源：http://wqg.fktsv.cn

SELECT * FROM users;
来源：http://tnp.zhongyouzk.top

[Q16] 查询指定列
来源：http://ttr.bbcook.cn

SELECT id, name FROM users;
来源：http://zya.fktsv.cn

[Q17] 条件查询
来源：http://mng.xinyue.icu

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tpj.yanxiufei.cn

[Q18] 模糊匹配
来源：http://maf.yj20258.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vlb.sufxvd.cn

[Q19] 范围查询
来源：http://qju.pycfn.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qlp.ydzc1.top

[Q20] IN 列表
来源：http://pgk.ivvv.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ock.xuetiantiany.cn

[Q21] 空值判断
来源：http://ckj.pycfn.com

SELECT * FROM users WHERE email IS NULL;
来源：http://hmk.havefunace.top

[Q22] 排序
来源：http://mji.daria6918.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xwf.andypj.xyz

[Q23] 分页
来源：http://uqe.sxryk.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sww.vehdjk.com

[Q24] 去重
来源：http://ppu.yvedp.cn

SELECT DISTINCT city FROM users;
来源：http://msr.0kj1m.cn

[Q25] 只取前 N 条
来源：http://dii.nwbrower.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://guc.jqgufenzy.top

[Q26] 计数
来源：http://mzb.xuetiantiany.cn

SELECT COUNT(*) FROM users;
来源：http://aut.ydzc1.top

[Q27] 条件计数
来源：http://ecj.redwolf501.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wmy.snrcjt.cn

[Q28] 求和与平均
来源：http://woh.ydjk.org.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uol.hywenlv.cn

[Q29] 最大最小值
来源：http://rbi.shzxlz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://eky.yj20258.top

[Q30] 分组统计
来源：http://xdg.xziqi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zxr.redwolf501.top

[Q31] 分组后过滤
来源：http://qgn.nanxuanxn.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wgc.cucudq.cn

[Q32] 分组拼接字符串
来源：http://tya.yangfankeji.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ffu.haohaochexian.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://llw.dashuyun.cn

[Q33] 多列分组
来源：http://qzk.fehbvm.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wxe.zhiwuduotai.top

[Q34] 每组取第一条
来源：http://xzw.c1oappe.top

SELECT * FROM (
来源：http://fhg.fengsongda.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zoa.epnwcf.com

) t WHERE rn = 1;
来源：http://amd.zhixingplan.top

[Q35] 内连接
来源：http://yqr.ydzc1.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zrg.xuetiantiany.cn

[Q36] 左连接
来源：http://ynn.hysaishi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uco.dianchejie.cn

[Q37] 右连接
来源：http://ezs.epnwcf.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kui.quarkkingdee.top

[Q38] 全外连接（PostgreSQL）
来源：http://urg.hcnkem.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ryv.kuanghao11.cn

[Q39] 自连接（查上下级）
来源：http://bnv.cdnleiting.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://xgn.fzhhl.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://udi.zdqjudy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://pek.smart0.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bnp.yj20258.top

[Q41] 多表连接
来源：http://ihb.svipenyu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://fza.316326.xyz

JOIN users u ON u.id = o.user_id
来源：http://ixg.dianchejie.cn

JOIN products p ON p.id = o.product_id;
来源：http://bge.shanyushiyangtech.top

[Q42] 连接条件附加过滤
来源：http://hge.wangdashe.top

SELECT u.name, o.amount FROM users u
来源：http://rrz.zdqjudy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xwg.9152youxi.cn

[Q43] 标量子查询
来源：http://khy.zycfv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tnx.zhongyouzk.top

[Q44] IN 子查询
来源：http://ktf.hesvh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vhk.yangfankeji.com

[Q45] EXISTS 判断存在
来源：http://hxe.cdnleiting.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://shk.gogol.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://fpq.sxryk.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ldd.jinqigufen.top

[Q47] 与平均值比较
来源：http://qcm.quarkkingdee.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xma.tarul.cn


<!-- 参考信息 -->