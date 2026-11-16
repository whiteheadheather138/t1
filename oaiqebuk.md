代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wvu.hfpthk.cn

[N06] 判断回文字符串
来源：http://rdr.aibaodan.cn

Py:   s == s[::-1]
来源：http://mwg.uphjek.com

PHP:  $s === strrev($s);
来源：http://wnt.zdqjudy.top

JS:   s === [...s].reverse().join("")
来源：http://vmc.yj202588.top

TS:   s === [...s].reverse().join("")
来源：http://dtr.sysykeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oan.tanke756.top

Go:   // 双指针从两端比较
来源：http://gnx.ybcxt.top

Ruby: s == s.reverse
来源：http://tkv.nanxinkj.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://vgn.yongpay.top

[N07] 两数之和（返回下标）
来源：http://php.quarkkingdee.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sna.xuanzx.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://shp.vehdjk.com

JS:   // 手写 Map：map.set(v, i)
来源：http://enu.daxiang520.top

TS:   // 手写 Map<string, number>
来源：http://tjh.yfazqb.com

Java: // 手写 HashMap
来源：http://fua.0kj1m.cn

Go:   // 手写 map[int]int
来源：http://cwy.xziqi.cn

Ruby: // 手写 Hash
来源：http://jat.shzxlz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://opy.gotoacloud.top

[N08] 生成全排列
来源：http://phy.hysaishi.cn

Py:   itertools.permutations(arr)
来源：http://rtx.jinqigfzy.top

PHP:  // 手写递归交换
来源：http://yfb.yuanzhike.top

JS:   // 手写回溯递归
来源：http://eyg.hcnkem.com

TS:   // 手写回溯递归
来源：http://wan.zhijiandao.cn

Java: // 手写回溯递归
来源：http://ckv.fzhhl.top

Go:   // 手写回溯递归
来源：http://jpg.jianghu66.top

Ruby: arr.permutation.to_a
来源：http://xop.kuanghao11.cn

C#:   // 手写回溯递归
来源：http://rzw.gogol.net.cn

[N09] 栈与队列
来源：http://xpv.jinqigfzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gfb.zhengqikj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ojm.ywan-chungtsiang.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wwo.nanxinkj.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nsp.hnxiangtu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dvr.cqqwz.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qqw.ppjwa.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ujv.gaohongyu789.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pdh.xinyue.icu

[N10] 链表节点定义
来源：http://jrt.hfpthk.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pea.xuanzx.com

PHP:  class Node { public $v; public $next = null; }
来源：http://mfb.vqdsnc.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tdl.jlsjyb.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cme.jqgfzy.top

Java: class Node { int v; Node next; }
来源：http://iub.mhx1999.top

Go:   type Node struct { V int; Next *Node }
来源：http://zug.0kj1m.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://elu.yueranfly.top

C#:   class Node { public int V; public Node? Next; }
来源：http://mdt.cdnleiting.top

[N11] 二叉树中序遍历
来源：http://rdk.jqgfzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kcf.shanyushiyangkeji.top

PHP:  // 手写递归函数
来源：http://nys.yj20258.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zrg.c1oappe.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ida.kuanghao11.cn

Java: // 手写递归
来源：http://azn.redwolf501.top

Go:   // 手写递归
来源：http://jtv.ydjk.org.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dog.hcnkem.com

C#:   // 手写递归
来源：http://qcr.shanyushiyangtech.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lhc.shangyingyoupin.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yqn.hywenlv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dav.uphjek.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uwj.gotoacloud.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://abh.yfazqb.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wit.jlsjyb.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://axb.wangdashe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wji.zdbjq.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://viw.vqdsnc.cn

================================================================================
来源：http://hfn.xuetiantiany.cn

O. 并发与异步
来源：http://gwh.yangfankeji.com

================================================================================
来源：http://sak.shanyushiyangtech.top

[O01] 启动一个线程
来源：http://xmg.0kj1m.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pqc.tianlin.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tnb.ppjwa.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vkc.dashuyun.cn

TS:   // 同 JS
来源：http://cct.fzhhl.top

Java: new Thread(() -> f()).start()
来源：http://uhi.tarul.cn

Go:   go f()
来源：http://vzt.zhixingplan.top

Ruby: Thread.new { f }
来源：http://nqc.zdqjudy.top

C#:   Task.Run(() => F());
来源：http://uzm.yj20258888.top

[O02] 使用线程池
来源：http://oap.jyoumei.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pnn.fehbvm.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dqm.ehwqpu.com

JS:   // worker_threads 线程池
来源：http://hqk.gotoacloud.top

TS:   // worker_threads 线程池
来源：http://bdz.xingfuxueyuan.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://boe.ehwqpu.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://myy.hysaishi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lgo.tian-w.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mgs.yj20258888.top

[O03] 加锁保护共享数据
来源：http://mzm.daxiang520.top

Py:   with lock: shared += 1
来源：http://cuc.sjlbkw.cn

PHP:  // 用 flock() 做文件锁
来源：http://ksg.cucudq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://geb.hammf.cn

TS:   // 同 JS
来源：http://xme.vehdjk.com

Java: synchronized (this) { shared++; }
来源：http://jto.guannengcc.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://drj.zdbjq.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://phj.hywenlv.cn

C#:   lock (gate) { shared++; }
来源：http://efh.tarul.cn

[O04] 定义异步函数并等待
来源：http://rwt.meibo888.top

Py:   async def f():⏎    await g()
来源：http://olx.52xcode.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zjt.nanxuanxn.top

JS:   async function f() { await g(); }
来源：http://wjr.fktsv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://slz.pycfn.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pce.hongshengwenyu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jdz.zhengqikj.top

Ruby: # 用 Fiber 或 async gem
来源：http://gzl.gaohongyu789.top

C#:   async Task F() { await G(); }
来源：http://hyj.zdbjq.cn

[O05] 并发执行并等待全部完成
来源：http://eek.fehbvm.com

Py:   asyncio.gather(*tasks)
来源：http://aqq.zhijiandao.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://piq.snrcjt.cn

JS:   await Promise.all(tasks)
来源：http://jmq.xuetiantiany.cn

TS:   await Promise.all(tasks)
来源：http://nkv.chenlongwang.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zsm.pycfn.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vhq.cqqwz.cn

Ruby: threads.map(&:join)
来源：http://uwi.ydzc1.top

C#:   await Task.WhenAll(t1, t2)
来源：http://pfl.xuetiantiany.cn

[O06] 使用进程池
来源：http://huk.tanke756.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://aha.guannengcc.top

PHP:  // pcntl_fork 或多进程队列
来源：http://nkh.yj202588.top

JS:   // child_process / cluster 模块
来源：http://xoe.chenzaomai.com

TS:   // child_process / cluster 模块
来源：http://sgk.dianchejie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tlj.wangshuangyany.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lwb.sysykeji.top

Ruby: // fork 块
来源：http://mjc.snrcjt.cn

C#:   Parallel.For
来源：http://rsd.yuxming.cn

================================================================================
来源：http://zmr.xuanzx.com

P. 常用工具函数
来源：http://ulw.hongshengwenyu.top

================================================================================
来源：http://bio.epnwcf.com

[P01] 生成 UUID
来源：http://oft.yj20258.top

Py:   str(uuid.uuid4())
来源：http://phh.52xcode.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tqf.redwolf501.top

JS:   crypto.randomUUID()
来源：http://wwt.jiagoushi.top

TS:   crypto.randomUUID()
来源：http://pep.fehbvm.com

Java: UUID.randomUUID().toString()
来源：http://nui.guannengcc.top

Go:   // 用 github.com/google/uuid
来源：http://pvd.iojbl.cn

Ruby: SecureRandom.uuid
来源：http://qcm.dianchejie.cn

C#:   Guid.NewGuid().ToString()
来源：http://rch.jinqigufen.top

[P02] MD5 / SHA256 摘要
来源：http://ojt.mhx1999.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jmz.xuanzx.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://dtf.wangdashe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vcr.hongshengwenyu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tlc.yuxming.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kxe.ehwqpu.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fbu.sysykeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cru.fehbvm.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://euh.hnqzz.top

[P03] 生成短随机字符串
来源：http://kzg.mhx1999.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rva.0kj1m.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gan.xinyue.icu

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oeq.epnwcf.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://luq.mhx1999.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nbu.haohaochexian.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dje.tanke756.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://dxs.yvedp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xnm.yangfankeji.com

[P04] 求长度
来源：http://fpj.fanxiaobao.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://beg.jqgfzy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jjo.jinqigufen.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xft.jinyuanbaomall.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://idt.hywenlv.cn

Java: list.size();  map.size();  s.length()
来源：http://scp.feifeiyinyue.top

Go:   len(arr);  len(m)
来源：http://gzz.ppjwa.cn

Ruby: x.length;  x.size
来源：http://tni.c1oappe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://fmp.zhiwuduotai.top

[P05] 判断两个对象内容是否相等
来源：http://xmi.hammf.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ovb.fzhhl.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dst.pengpengdd.cyou

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gca.redwolf501.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gkd.xylfe.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wny.pengpengdd.cyou

Go:   reflect.DeepEqual(a, b)
来源：http://aww.fengsongda.top

Ruby: a == b
来源：http://fob.havefunace.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://izy.chenjidiqi.icu

[P06] 综合判空（null / 空串 / 空集合）
来源：http://eqv.zdbjq.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kpy.pycfn.com

PHP:  if (empty($x)) {}
来源：http://iju.dashuyun.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://okj.jyoumei.cn

TS:   if (x == null) {}
来源：http://xqt.cqqwz.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://znc.hammf.cn

Go:   if x == nil {}
来源：http://dcl.hfpthk.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hra.bbcook.cn

C#:   if (x is null) {}
来源：http://ucv.yuxming.cn

[P07] 防抖与节流
来源：http://rfg.yuanzhike.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gug.chenjidiqi.icu

PHP:  // 手写时间戳比较
来源：http://yuc.shzxlz.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qio.vqdsnc.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gox.haohaochexian.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uyl.sjlbkw.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ijk.jinyuanbaomall.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wpy.zhongyouzk.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zgo.ybcxt.top

[P08] 处理浮点精度问题
来源：http://jij.xinyue.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ssw.svipenyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yoh.52xcode.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cxu.fanxiaobao.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rfw.zdqjudy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tzn.52xcode.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://juc.cheryme.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wjh.zhoulong.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pqv.shuidangran.top

================================================================================
来源：http://bgj.guowangkeji.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fkl.sysykeji.top

================================================================================
来源：http://vcx.jlsjyb.cn

[Q01] 创建表
来源：http://etc.hesvh.cn

CREATE TABLE users (
来源：http://pcs.ehwqpu.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://afn.sxryk.cn

name VARCHAR(50) NOT NULL,
来源：http://qdz.yangfankeji.com

email VARCHAR(100) UNIQUE,
来源：http://ptq.hnqzz.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://knp.redwolf501.top

);
来源：http://gfb.cucudq.cn

[Q02] 创建带外键的表
来源：http://dpz.yuanzhike.top

CREATE TABLE orders (
来源：http://tcf.jianghu66.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tzl.yuanzhike.top

user_id INT NOT NULL,
来源：http://mtr.ydjk.org.cn

amount DECIMAL(10, 2),
来源：http://nbf.c1oappe.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gdx.hcnkem.com

);
来源：http://mls.hammf.cn

[Q03] 增加列
来源：http://mre.cheryme.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tmb.pengpengdd.cyou

[Q04] 修改列类型
来源：http://lcn.ehwqpu.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ycf.guowangkeji.top

[Q05] 重命名列
来源：http://azr.shanyushiyangtech.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://puc.andypj.xyz

[Q06] 删除列
来源：http://ztx.hammf.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yms.yj20258.top

[Q07] 删除表
来源：http://dqr.cucudq.cn

DROP TABLE IF EXISTS orders;
来源：http://ioi.bjfxy.top

[Q08] 创建普通索引
来源：http://egt.jiagoushi.top

CREATE INDEX idx_users_email ON users(email);
来源：http://nsr.xinyue.icu

[Q09] 创建唯一索引
来源：http://gcq.ybcxt.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dzw.kuanghao11.cn

[Q10] 插入单行
来源：http://tpf.feifeiyinyue.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nvv.redwolf501.top

[Q11] 一次插入多行
来源：http://ofz.redwolf501.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://xtz.yvedp.cn

[Q12] 插入后取自增 ID
来源：http://vpt.yj20258888.top

INSERT INTO users (name) VALUES ('C');
来源：http://fqy.c1oappe.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vxm.nanxuanxn.top

[Q13] 忽略重复插入
来源：http://ynd.shanyushiyangtech.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vrv.yj202588.top

[Q14] 存在则更新（upsert）
来源：http://brw.shanyushiyangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mgm.zycfv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fnx.hesvh.cn

[Q15] 查询全部
来源：http://lip.sxryk.cn

SELECT * FROM users;
来源：http://rdu.xinyue.icu

[Q16] 查询指定列
来源：http://xsm.zycfv.cn

SELECT id, name FROM users;
来源：http://cja.dianchejie.cn

[Q17] 条件查询
来源：http://usp.kuanghao11.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dxu.feifeiyinyue.top

[Q18] 模糊匹配
来源：http://jln.havefunace.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xtg.sweek.top

[Q19] 范围查询
来源：http://bll.sjlbkw.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tpv.gaohongyu789.top

[Q20] IN 列表
来源：http://aek.cucudq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yer.xingfuxueyuan.xyz

[Q21] 空值判断
来源：http://rtq.svipenyu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zdk.shanyushiyangtech.top

[Q22] 排序
来源：http://rob.zhixingplan.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://edo.hongshengwenyu.top

[Q23] 分页
来源：http://aqm.hnqzz.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zdu.kuanghao11.cn

[Q24] 去重
来源：http://qyg.zhoulong.xyz

SELECT DISTINCT city FROM users;
来源：http://jkn.yj20258888.top

[Q25] 只取前 N 条
来源：http://dar.zhongyouzk.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://znq.yanxiufei.cn

[Q26] 计数
来源：http://bpl.fengsongda.top

SELECT COUNT(*) FROM users;
来源：http://hwe.hammf.cn

[Q27] 条件计数
来源：http://yaq.yuxming.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oxe.shanyushiyangtech.top

[Q28] 求和与平均
来源：http://les.jinqigufen.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mhr.dianchejie.cn

[Q29] 最大最小值
来源：http://ase.zhiwuduotai.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://pvs.ppjwa.cn

[Q30] 分组统计
来源：http://gjj.shanyushiyangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jhb.sxryk.cn

[Q31] 分组后过滤
来源：http://nuh.yuxming.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dny.svipenyu.cn

[Q32] 分组拼接字符串
来源：http://ypd.mhx1999.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hdx.wangshuangyany.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jqr.nwbrower.top

[Q33] 多列分组
来源：http://hld.shanyushiyangtech.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vgz.quarkkingdee.top

[Q34] 每组取第一条
来源：http://mdb.shuidangran.top

SELECT * FROM (
来源：http://nle.tianlin.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zjd.smart0.xyz

) t WHERE rn = 1;
来源：http://qav.yongpay.top

[Q35] 内连接
来源：http://cow.yanxiufei.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bgu.jinyuanbaomall.cn

[Q36] 左连接
来源：http://boy.vqdsnc.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qoh.jinghuilouyu.cn

[Q37] 右连接
来源：http://zlx.jianghu66.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mra.52xcode.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ktq.vehdjk.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wvc.xuanzx.com

[Q39] 自连接（查上下级）
来源：http://gse.shangyingyoupin.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://sny.pengpengdd.cyou

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wqe.yvedp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jhz.zhongyouzk.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zrt.xylfe.cn

[Q41] 多表连接
来源：http://mtu.yfazqb.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://taf.vehdjk.com

JOIN users u ON u.id = o.user_id
来源：http://jll.hcnkem.com

JOIN products p ON p.id = o.product_id;
来源：http://mig.aizwys.cn

[Q42] 连接条件附加过滤
来源：http://ylp.yuxming.cn


<!-- 参考信息 -->