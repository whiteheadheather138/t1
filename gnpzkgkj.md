代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://frk.yvedp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://knq.fzhhl.top

TS:   // 手写 Map<string, number>
来源：http://ktt.xinyue.icu

Java: // 手写 HashMap
来源：http://bsk.shuidangran.top

Go:   // 手写 map[int]int
来源：http://ouk.zhoulong.xyz

Ruby: // 手写 Hash
来源：http://msv.yj20258.top

C#:   // 手写 Dictionary<int, int>
来源：http://ssh.aizwys.cn

[N08] 生成全排列
来源：http://hoq.xinyue.icu

Py:   itertools.permutations(arr)
来源：http://qkm.hfpthk.cn

PHP:  // 手写递归交换
来源：http://zfb.jlsjyb.cn

JS:   // 手写回溯递归
来源：http://gvn.shangyingyoupin.top

TS:   // 手写回溯递归
来源：http://fae.shangyingyoupin.top

Java: // 手写回溯递归
来源：http://gjc.havefunace.top

Go:   // 手写回溯递归
来源：http://akn.tian-w.cn

Ruby: arr.permutation.to_a
来源：http://sve.cashguo.top

C#:   // 手写回溯递归
来源：http://xzz.gotoacloud.top

[N09] 栈与队列
来源：http://seu.yangfankeji.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ptr.xinyue.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jje.tianlin.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kux.pycfn.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bfc.jinyuanbaomall.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ogy.wangshuangyany.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ojt.shuidangran.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ufx.zhoulong.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fdf.dianchejie.cn

[N10] 链表节点定义
来源：http://wvm.jinqigufen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fhg.tianlin.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://tlb.mhx1999.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lem.chenzaomai.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://euj.cashguo.top

Java: class Node { int v; Node next; }
来源：http://tqj.zhengqikj.top

Go:   type Node struct { V int; Next *Node }
来源：http://xzi.yanxiufei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fcw.ctjpmb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://jdt.chenjidiqi.icu

[N11] 二叉树中序遍历
来源：http://hyc.hcnkem.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lws.nanxinkj.top

PHP:  // 手写递归函数
来源：http://mgv.jianghu66.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jpt.jinyuanbaomall.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dim.tian-w.cn

Java: // 手写递归
来源：http://cmy.chenjidiqi.icu

Go:   // 手写递归
来源：http://hgs.hysaishi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yhm.zhengqikj.top

C#:   // 手写递归
来源：http://jzk.fehbvm.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hny.ydzc1.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bkx.sxryk.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sfm.hnqzz.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://awo.quarkkingdee.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fav.xylfe.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hee.fanxiaobao.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://flg.nanxinkj.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ucc.hysaishi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yqf.sysykeji.top

================================================================================
来源：http://nlt.dashuyun.cn

O. 并发与异步
来源：http://flw.hfpthk.cn

================================================================================
来源：http://gej.quarkkingdee.top

[O01] 启动一个线程
来源：http://jch.gogol.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://abn.aibaodan.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uwr.xziqi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mjr.yfazqb.com

TS:   // 同 JS
来源：http://mwm.cdnleiting.top

Java: new Thread(() -> f()).start()
来源：http://ekn.nanxuanxn.top

Go:   go f()
来源：http://fnh.zhongyouzk.top

Ruby: Thread.new { f }
来源：http://dun.meibo888.top

C#:   Task.Run(() => F());
来源：http://uhr.yj20258888.top

[O02] 使用线程池
来源：http://zfg.tanke756.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ltm.ivvv.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://thh.shanyushiyangkeji.top

JS:   // worker_threads 线程池
来源：http://hrg.jiagoushi.top

TS:   // worker_threads 线程池
来源：http://jtp.feifeiyinyue.top

Java: Executors.newFixedThreadPool(4)
来源：http://vah.fzhhl.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hvm.jqgufenzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dsc.fanxiaobao.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zgs.ppjwa.cn

[O03] 加锁保护共享数据
来源：http://nma.nanxinkj.top

Py:   with lock: shared += 1
来源：http://pcy.ehwqpu.com

PHP:  // 用 flock() 做文件锁
来源：http://nbl.jinghuilouyu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dxa.svipenyu.cn

TS:   // 同 JS
来源：http://qru.yj202588.top

Java: synchronized (this) { shared++; }
来源：http://oth.zycfv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://htr.nanxuanxn.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://kpr.9152youxi.cn

C#:   lock (gate) { shared++; }
来源：http://gfi.nanxinkj.top

[O04] 定义异步函数并等待
来源：http://guy.jiagoushi.top

Py:   async def f():⏎    await g()
来源：http://sop.nanxuanxn.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wkm.ivvv.top

JS:   async function f() { await g(); }
来源：http://qva.iojbl.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fkr.guowangkeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://crb.hcnkem.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lmz.tianlin.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://qzc.sweek.top

C#:   async Task F() { await G(); }
来源：http://cbe.haohaochexian.top

[O05] 并发执行并等待全部完成
来源：http://aal.gzhubu.top

Py:   asyncio.gather(*tasks)
来源：http://qyt.yuanzhike.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dct.jinqigufen.top

JS:   await Promise.all(tasks)
来源：http://uus.cucudq.cn

TS:   await Promise.all(tasks)
来源：http://bgt.zhaomingkeji.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sby.hfpthk.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xqh.andypj.xyz

Ruby: threads.map(&:join)
来源：http://pca.jqgufenzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://eej.zhixingplan.top

[O06] 使用进程池
来源：http://gak.cdnleiting.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nsy.gotoacloud.top

PHP:  // pcntl_fork 或多进程队列
来源：http://tor.ppjwa.cn

JS:   // child_process / cluster 模块
来源：http://pua.jinyuanbaomall.cn

TS:   // child_process / cluster 模块
来源：http://vkz.yj202588.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fbr.cucudq.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://itc.guowangkeji.top

Ruby: // fork 块
来源：http://ker.havefunace.top

C#:   Parallel.For
来源：http://fqc.cdnleiting.top

================================================================================
来源：http://gmj.zhengqikj.top

P. 常用工具函数
来源：http://wjp.jinqigufen.top

================================================================================
来源：http://yxo.fengsongda.top

[P01] 生成 UUID
来源：http://vbr.dianchejie.cn

Py:   str(uuid.uuid4())
来源：http://kba.sjlbkw.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nkn.shangyingyoupin.top

JS:   crypto.randomUUID()
来源：http://cfo.sjlbkw.cn

TS:   crypto.randomUUID()
来源：http://bdo.jinghuilouyu.cn

Java: UUID.randomUUID().toString()
来源：http://bee.zhengqikj.top

Go:   // 用 github.com/google/uuid
来源：http://ibx.jinghuilouyu.cn

Ruby: SecureRandom.uuid
来源：http://kgf.mhx1999.top

C#:   Guid.NewGuid().ToString()
来源：http://dbx.ctjpmb.com

[P02] MD5 / SHA256 摘要
来源：http://wju.jinqigfzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jit.jyoumei.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ddl.uphjek.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dou.hnxiangtu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ubh.yj202588.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://loh.jianghu66.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fvy.hfpthk.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hhc.daxiang520.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vma.svipenyu.cn

[P03] 生成短随机字符串
来源：http://ium.aibaodan.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://viu.yj20258.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zwb.shuidangran.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kzh.guannengcc.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dvv.vehdjk.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ube.yonumen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ohb.yuxming.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rrr.cashguo.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ylq.aizwys.cn

[P04] 求长度
来源：http://spx.xziqi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ffo.yueranfly.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nco.chenlongwang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nqk.wangshuangyany.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ote.nanxuanxn.top

Java: list.size();  map.size();  s.length()
来源：http://wnr.meibo888.top

Go:   len(arr);  len(m)
来源：http://obi.sufxvd.cn

Ruby: x.length;  x.size
来源：http://crk.meibo888.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://cnr.snrcjt.cn

[P05] 判断两个对象内容是否相等
来源：http://rye.vqdsnc.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lsq.bjfxy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://eks.sxryk.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ovw.0kj1m.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://opm.yj20258888.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ozy.gogol.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lpf.hesvh.cn

Ruby: a == b
来源：http://htt.guannengcc.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://eee.chenlongwang.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://occ.shanyushiyangkeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://eki.cqqwz.cn

PHP:  if (empty($x)) {}
来源：http://llh.redwolf501.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uqe.xingfuxueyuan.xyz

TS:   if (x == null) {}
来源：http://efi.hfpthk.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wga.xinyue.icu

Go:   if x == nil {}
来源：http://wky.ybcxt.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zxj.9152youxi.cn

C#:   if (x is null) {}
来源：http://nrz.yonumen.top

[P07] 防抖与节流
来源：http://dlr.shzxlz.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blm.bjfxy.top

PHP:  // 手写时间戳比较
来源：http://jnp.yj20258.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lzw.zhaomingkeji.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kbg.nanxuanxn.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://syd.pycfn.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fuo.xuanzx.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://yru.yuanzhike.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rdr.316326.xyz

[P08] 处理浮点精度问题
来源：http://myi.daxiang520.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ztb.ivvv.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://puz.shuidangran.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sdz.c1oappe.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xfy.fzhhl.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fit.uphjek.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kyf.vqdsnc.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ayo.chenjidiqi.icu

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wmq.hammf.cn

================================================================================
来源：http://xni.zdqjudy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yzz.shangyingyoupin.top

================================================================================
来源：http://nvd.tianlin.xyz

[Q01] 创建表
来源：http://qny.guowangkeji.top

CREATE TABLE users (
来源：http://euw.jianghu66.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vaa.yuanzhike.top

name VARCHAR(50) NOT NULL,
来源：http://yed.yonumen.top

email VARCHAR(100) UNIQUE,
来源：http://usb.shzxlz.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yev.guannengcc.top

);
来源：http://vso.tian-w.cn

[Q02] 创建带外键的表
来源：http://wmc.smart0.xyz

CREATE TABLE orders (
来源：http://csp.zhaomingkeji.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vlc.0kj1m.cn

user_id INT NOT NULL,
来源：http://dbw.mhx1999.top

amount DECIMAL(10, 2),
来源：http://hkl.yj202588.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lat.ydjk.org.cn

);
来源：http://cbs.kuanghao11.cn

[Q03] 增加列
来源：http://knx.jinghuilouyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fzb.kuanghao11.cn

[Q04] 修改列类型
来源：http://wod.tian-w.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xth.shanyushiyangkeji.top

[Q05] 重命名列
来源：http://irc.yueranfly.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vzf.redwolf501.top

[Q06] 删除列
来源：http://hqy.0kj1m.cn

ALTER TABLE users DROP COLUMN age;
来源：http://nuk.bbcook.cn

[Q07] 删除表
来源：http://yvv.nanxinkj.top

DROP TABLE IF EXISTS orders;
来源：http://mve.yuxming.cn

[Q08] 创建普通索引
来源：http://nvv.smart0.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://edv.ivvv.top

[Q09] 创建唯一索引
来源：http://qaj.chenlongwang.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fas.ctjpmb.com

[Q10] 插入单行
来源：http://amm.haohaochexian.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tgh.tianlin.xyz

[Q11] 一次插入多行
来源：http://zfs.tarul.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zfj.jinqigufen.top

[Q12] 插入后取自增 ID
来源：http://fjy.hongshengwenyu.top

INSERT INTO users (name) VALUES ('C');
来源：http://sew.zhongyouzk.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hss.jinyuanbaomall.cn

[Q13] 忽略重复插入
来源：http://nnh.yj20258888.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mim.shanyushiyangkeji.top

[Q14] 存在则更新（upsert）
来源：http://dac.bbcook.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ezk.yongpay.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kar.dashuyun.cn

[Q15] 查询全部
来源：http://unl.fanxiaobao.xyz

SELECT * FROM users;
来源：http://qum.gaohongyu789.top

[Q16] 查询指定列
来源：http://ykf.xziqi.cn

SELECT id, name FROM users;
来源：http://zvd.ydzc1.top

[Q17] 条件查询
来源：http://eyc.tianlin.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kfg.xuanzx.com

[Q18] 模糊匹配
来源：http://vor.gogol.net.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kpr.gogol.net.cn

[Q19] 范围查询
来源：http://ong.jinqigfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ffh.hnqzz.top

[Q20] IN 列表
来源：http://xpa.cdnleiting.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sqb.uphjek.com

[Q21] 空值判断
来源：http://psg.jqgfzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://qmd.xinyue.icu

[Q22] 排序
来源：http://uko.jiagoushi.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ajo.fehbvm.com

[Q23] 分页
来源：http://upe.ydjk.org.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cas.hnqzz.top

[Q24] 去重
来源：http://axe.yj20258888.top

SELECT DISTINCT city FROM users;
来源：http://pan.jiagoushi.top

[Q25] 只取前 N 条
来源：http://bfj.9152youxi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mnv.vqdsnc.cn

[Q26] 计数
来源：http://eyf.ctjpmb.com

SELECT COUNT(*) FROM users;
来源：http://spd.cucudq.cn

[Q27] 条件计数
来源：http://kia.dianchejie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fyp.yuanzhike.top

[Q28] 求和与平均
来源：http://pbl.tarul.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://moh.ppjwa.cn

[Q29] 最大最小值
来源：http://fpo.0kj1m.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gvx.bbcook.cn

[Q30] 分组统计
来源：http://pvm.sufxvd.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://emp.shuidangran.top

[Q31] 分组后过滤
来源：http://ssy.zdqjudy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sqw.birdmap.top

[Q32] 分组拼接字符串
来源：http://czl.jqgufenzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vwn.fzhhl.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ksy.zdbjq.cn

[Q33] 多列分组
来源：http://ebo.birdmap.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://aqd.chenzaomai.com

[Q34] 每组取第一条
来源：http://nee.xingfuxueyuan.xyz

SELECT * FROM (
来源：http://pwt.pengpengdd.cyou

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tff.jlsjyb.cn

) t WHERE rn = 1;
来源：http://jru.snrcjt.cn

[Q35] 内连接
来源：http://zmg.0kj1m.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://aeg.shanyushiyangtech.top

[Q36] 左连接
来源：http://mlt.jiagoushi.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uah.cdnleiting.top

[Q37] 右连接
来源：http://irc.fehbvm.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nfy.redwolf501.top

[Q38] 全外连接（PostgreSQL）
来源：http://whi.yj20258.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jpe.yj202588.top

[Q39] 自连接（查上下级）
来源：http://zew.yj20258.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://kpj.xinyue.icu

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://irh.chenlongwang.top

[Q40] 交叉连接（笛卡尔积）
来源：http://rsx.aibaodan.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://urg.ivvv.top

[Q41] 多表连接
来源：http://nyb.sxryk.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cbv.gaohongyu789.top

JOIN users u ON u.id = o.user_id
来源：http://iwz.nanxinkj.top

JOIN products p ON p.id = o.product_id;
来源：http://tvt.chenjidiqi.icu

[Q42] 连接条件附加过滤
来源：http://hdp.sxryk.cn

SELECT u.name, o.amount FROM users u
来源：http://ftm.kuanghao11.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mbx.xinyue.icu

[Q43] 标量子查询
来源：http://gnt.nanxuanxn.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://obr.tianlin.xyz

[Q44] IN 子查询
来源：http://iaq.guowangkeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mso.wangshuangyany.cn

[Q45] EXISTS 判断存在
来源：http://jpc.52xcode.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fig.fanxiaobao.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://fje.sysykeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gde.xuetiantiany.cn

[Q47] 与平均值比较
来源：http://cos.shuidangran.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://eav.feifeiyinyue.top


<!-- 参考信息 -->