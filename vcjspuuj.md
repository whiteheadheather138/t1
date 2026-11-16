代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://cet.guannengcc.top

TS:   s === [...s].reverse().join("")
来源：http://fgz.feifeiyinyue.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jdf.quarkkingdee.top

Go:   // 双指针从两端比较
来源：http://tim.wangshuangyany.cn

Ruby: s == s.reverse
来源：http://cdd.tian-w.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qki.epnwcf.com

[N07] 两数之和（返回下标）
来源：http://mgg.xingfuxueyuan.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zez.jqgfzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://prk.hesvh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ksj.ydjk.org.cn

TS:   // 手写 Map<string, number>
来源：http://qqq.shuidangran.top

Java: // 手写 HashMap
来源：http://vew.hammf.cn

Go:   // 手写 map[int]int
来源：http://nmf.xuanzx.com

Ruby: // 手写 Hash
来源：http://kza.chenlongwang.top

C#:   // 手写 Dictionary<int, int>
来源：http://acm.daxiang520.top

[N08] 生成全排列
来源：http://eqm.ybcxt.top

Py:   itertools.permutations(arr)
来源：http://ewc.chenjidiqi.icu

PHP:  // 手写递归交换
来源：http://azp.tanke756.top

JS:   // 手写回溯递归
来源：http://scu.jinyuanbaomall.cn

TS:   // 手写回溯递归
来源：http://jhx.fehbvm.com

Java: // 手写回溯递归
来源：http://pio.jqgufenzy.top

Go:   // 手写回溯递归
来源：http://bgx.cqqwz.cn

Ruby: arr.permutation.to_a
来源：http://dub.snrcjt.cn

C#:   // 手写回溯递归
来源：http://pkx.kuanghao11.cn

[N09] 栈与队列
来源：http://ruz.sweek.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vfo.yfazqb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jjw.xziqi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wpu.zdbjq.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mkt.zhiwuduotai.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ptc.shanyushiyangkeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uid.zhaomingkeji.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wry.tianlin.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ktz.sysykeji.top

[N10] 链表节点定义
来源：http://iqr.shangyingyoupin.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://oib.hnxiangtu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://kvp.jqgufenzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xpx.52xcode.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pdx.jinyuanbaomall.cn

Java: class Node { int v; Node next; }
来源：http://uhn.sweek.top

Go:   type Node struct { V int; Next *Node }
来源：http://ete.shangyingyoupin.top

Ruby: Node = Struct.new(:v, :next)
来源：http://prk.yuxming.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wdr.svipenyu.cn

[N11] 二叉树中序遍历
来源：http://bfc.gzhubu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hjj.gaohongyu789.top

PHP:  // 手写递归函数
来源：http://sbm.hnxiangtu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://svj.xuanzx.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ksc.yuanzhike.top

Java: // 手写递归
来源：http://hrt.jinghuilouyu.cn

Go:   // 手写递归
来源：http://dmp.meibo888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://shd.hysaishi.cn

C#:   // 手写递归
来源：http://ylu.yj202588.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pyg.yuxming.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dft.wangdashe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://evs.jlsjyb.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://srs.zhengqikj.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vii.jiagoushi.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dys.fktsv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gwa.chenlongwang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fcp.hcnkem.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vop.snrcjt.cn

================================================================================
来源：http://qbh.epnwcf.com

O. 并发与异步
来源：http://dpy.fanxiaobao.xyz

================================================================================
来源：http://fli.zdbjq.cn

[O01] 启动一个线程
来源：http://qao.hongshengwenyu.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://war.sweek.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://axx.wangshuangyany.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hdz.chenjidiqi.icu

TS:   // 同 JS
来源：http://qjb.ivvv.top

Java: new Thread(() -> f()).start()
来源：http://axy.yangfankeji.com

Go:   go f()
来源：http://mzi.chenzaomai.com

Ruby: Thread.new { f }
来源：http://mwn.daria6918.cn

C#:   Task.Run(() => F());
来源：http://dph.uphjek.com

[O02] 使用线程池
来源：http://qem.gotoacloud.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://iia.xziqi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dut.gaohongyu789.top

JS:   // worker_threads 线程池
来源：http://sbj.jlsjyb.cn

TS:   // worker_threads 线程池
来源：http://phu.chenzaomai.com

Java: Executors.newFixedThreadPool(4)
来源：http://sxi.hnqzz.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://siz.zhengqikj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xjx.nwbrower.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://eab.hnxiangtu.top

[O03] 加锁保护共享数据
来源：http://gks.haohaochexian.top

Py:   with lock: shared += 1
来源：http://vhz.sxryk.cn

PHP:  // 用 flock() 做文件锁
来源：http://uzg.cdnleiting.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mdj.tanke756.top

TS:   // 同 JS
来源：http://wxq.tanke756.top

Java: synchronized (this) { shared++; }
来源：http://xmg.xylfe.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zim.svipenyu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lfd.sjlbkw.cn

C#:   lock (gate) { shared++; }
来源：http://yvi.hysaishi.cn

[O04] 定义异步函数并等待
来源：http://nvz.hnqzz.top

Py:   async def f():⏎    await g()
来源：http://djd.yuanzhike.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://puv.yj202588.top

JS:   async function f() { await g(); }
来源：http://hjq.kuanghao11.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dge.fengsongda.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mat.mhx1999.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://urc.9152youxi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ame.xziqi.cn

C#:   async Task F() { await G(); }
来源：http://did.yfazqb.com

[O05] 并发执行并等待全部完成
来源：http://jtw.jinqigfzy.top

Py:   asyncio.gather(*tasks)
来源：http://ens.dashuyun.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kbo.haohaochexian.top

JS:   await Promise.all(tasks)
来源：http://ygp.hongshengwenyu.top

TS:   await Promise.all(tasks)
来源：http://xmc.xuetiantiany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cdy.jinqigufen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nix.shanyushiyangtech.top

Ruby: threads.map(&:join)
来源：http://dic.sjlbkw.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hcs.bbcook.cn

[O06] 使用进程池
来源：http://tlu.chenlongwang.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ood.vqdsnc.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nww.chenzaomai.com

JS:   // child_process / cluster 模块
来源：http://lle.gotoacloud.top

TS:   // child_process / cluster 模块
来源：http://dsm.hesvh.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oeg.yangfankeji.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://idi.jinqigufen.top

Ruby: // fork 块
来源：http://efm.ppjwa.cn

C#:   Parallel.For
来源：http://nic.xylfe.cn

================================================================================
来源：http://arf.shanyushiyangkeji.top

P. 常用工具函数
来源：http://rxz.ehwqpu.com

================================================================================
来源：http://jyw.gaohongyu789.top

[P01] 生成 UUID
来源：http://bve.ydzc1.top

Py:   str(uuid.uuid4())
来源：http://xrh.wangdashe.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ufb.aizwys.cn

JS:   crypto.randomUUID()
来源：http://wqn.xziqi.cn

TS:   crypto.randomUUID()
来源：http://uah.pycfn.com

Java: UUID.randomUUID().toString()
来源：http://wqf.dashuyun.cn

Go:   // 用 github.com/google/uuid
来源：http://ayz.xuanzx.com

Ruby: SecureRandom.uuid
来源：http://thn.yvedp.cn

C#:   Guid.NewGuid().ToString()
来源：http://mwh.svipenyu.cn

[P02] MD5 / SHA256 摘要
来源：http://umf.cheryme.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kky.fengsongda.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://pdt.tanke756.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hdg.bbcook.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ifb.xylfe.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rhy.xuanzx.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qyp.meibo888.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fpm.epnwcf.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ivt.hcnkem.com

[P03] 生成短随机字符串
来源：http://mhk.wangshuangyany.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lri.aibaodan.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rxx.tian-w.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wvz.zdqjudy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ahy.zhongyouzk.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://epe.aibaodan.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vdv.xylfe.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://dzz.pengpengdd.cyou

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fqr.jinghuilouyu.cn

[P04] 求长度
来源：http://eoa.hywenlv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ljj.haohaochexian.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ohw.jiagoushi.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://txl.zycfv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nra.shangyingyoupin.top

Java: list.size();  map.size();  s.length()
来源：http://dyu.haohaochexian.top

Go:   len(arr);  len(m)
来源：http://nph.epnwcf.com

Ruby: x.length;  x.size
来源：http://tyj.vqdsnc.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://idt.jinyuanbaomall.cn

[P05] 判断两个对象内容是否相等
来源：http://tug.nwbrower.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://dcm.yonumen.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://irg.hnxiangtu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kru.shanyushiyangkeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://npv.ywan-chungtsiang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pga.hongshengwenyu.top

Go:   reflect.DeepEqual(a, b)
来源：http://abj.sxryk.cn

Ruby: a == b
来源：http://sod.sxryk.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://avs.xinyue.icu

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tft.jlsjyb.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jxe.chenzaomai.com

PHP:  if (empty($x)) {}
来源：http://yxh.yfazqb.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xlm.shuidangran.top

TS:   if (x == null) {}
来源：http://tjk.andypj.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://pso.cheryme.top

Go:   if x == nil {}
来源：http://zcy.xziqi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://akg.jyoumei.cn

C#:   if (x is null) {}
来源：http://oiu.vehdjk.com

[P07] 防抖与节流
来源：http://eho.cheryme.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ngh.snrcjt.cn

PHP:  // 手写时间戳比较
来源：http://ibh.zdqjudy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bxy.hnqzz.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ipc.ctjpmb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://czn.nanxuanxn.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://syh.zdqjudy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://swh.wangshuangyany.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kra.snrcjt.cn

[P08] 处理浮点精度问题
来源：http://adf.xziqi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://inz.316326.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hkc.jqgfzy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vbb.hcnkem.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wmg.zycfv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://znf.svipenyu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sae.hfpthk.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bru.zhoulong.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bxu.hesvh.cn

================================================================================
来源：http://xsc.xylfe.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fky.chenjidiqi.icu

================================================================================
来源：http://jny.fehbvm.com

[Q01] 创建表
来源：http://yon.hnqzz.top

CREATE TABLE users (
来源：http://eiy.jqgfzy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mcc.nwbrower.top

name VARCHAR(50) NOT NULL,
来源：http://avb.316326.xyz

email VARCHAR(100) UNIQUE,
来源：http://qji.sweek.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lpm.zycfv.cn

);
来源：http://yxw.shanyushiyangkeji.top

[Q02] 创建带外键的表
来源：http://qsf.daxiang520.top

CREATE TABLE orders (
来源：http://dup.zhoulong.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wfs.jiagoushi.top

user_id INT NOT NULL,
来源：http://ihe.redwolf501.top

amount DECIMAL(10, 2),
来源：http://tun.chenjidiqi.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jfo.dianchejie.cn

);
来源：http://ieh.cashguo.top

[Q03] 增加列
来源：http://efq.ivvv.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nix.tarul.cn

[Q04] 修改列类型
来源：http://jgu.zycfv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ajp.jyoumei.cn

[Q05] 重命名列
来源：http://srb.haohaochexian.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ytb.hysaishi.cn

[Q06] 删除列
来源：http://oyp.hysaishi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ofa.gotoacloud.top

[Q07] 删除表
来源：http://xup.aizwys.cn

DROP TABLE IF EXISTS orders;
来源：http://hkp.hnxiangtu.top

[Q08] 创建普通索引
来源：http://but.pengpengdd.cyou

CREATE INDEX idx_users_email ON users(email);
来源：http://gdt.pycfn.com

[Q09] 创建唯一索引
来源：http://gqg.nwbrower.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ouq.redwolf501.top

[Q10] 插入单行
来源：http://jbw.uphjek.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://plk.cucudq.cn

[Q11] 一次插入多行
来源：http://whu.yj20258.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wbd.zhoulong.xyz

[Q12] 插入后取自增 ID
来源：http://zog.zhaomingkeji.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://zra.aizwys.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://grc.yvedp.cn

[Q13] 忽略重复插入
来源：http://npw.jlsjyb.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hrd.chenzaomai.com

[Q14] 存在则更新（upsert）
来源：http://pyy.shanyushiyangtech.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xvf.zhiwuduotai.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://avc.yj20258.top

[Q15] 查询全部
来源：http://hhr.0kj1m.cn

SELECT * FROM users;
来源：http://taz.zhixingplan.top

[Q16] 查询指定列
来源：http://xum.sufxvd.cn

SELECT id, name FROM users;
来源：http://qsg.chenzaomai.com

[Q17] 条件查询
来源：http://avd.iojbl.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dxn.cucudq.cn

[Q18] 模糊匹配
来源：http://nzv.nanxuanxn.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dfs.bjfxy.top

[Q19] 范围查询
来源：http://zcw.meibo888.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nzd.zdqjudy.top

[Q20] IN 列表
来源：http://rlv.jqgufenzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yec.bjfxy.top

[Q21] 空值判断
来源：http://pgt.sweek.top

SELECT * FROM users WHERE email IS NULL;
来源：http://lkv.jiagoushi.top

[Q22] 排序
来源：http://wbq.bjfxy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tti.sxryk.cn

[Q23] 分页
来源：http://osu.snrcjt.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pje.hfpthk.cn

[Q24] 去重
来源：http://ioq.wangdashe.top

SELECT DISTINCT city FROM users;
来源：http://xjm.tanke756.top

[Q25] 只取前 N 条
来源：http://soz.gaohongyu789.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fte.haohaochexian.top

[Q26] 计数
来源：http://sgl.zhengqikj.top

SELECT COUNT(*) FROM users;
来源：http://mas.hfpthk.cn

[Q27] 条件计数
来源：http://ton.aibaodan.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bko.shuidangran.top

[Q28] 求和与平均
来源：http://gpa.hywenlv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://aro.haohaochexian.top

[Q29] 最大最小值
来源：http://uqv.hesvh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xig.ctjpmb.com

[Q30] 分组统计
来源：http://oro.mhx1999.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yvh.jinyuanbaomall.cn

[Q31] 分组后过滤
来源：http://hsb.yangfankeji.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jty.redwolf501.top

[Q32] 分组拼接字符串
来源：http://hhy.gaohongyu789.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mjp.cucudq.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mgf.zycfv.cn

[Q33] 多列分组
来源：http://rbp.yangfankeji.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dvm.cheryme.top

[Q34] 每组取第一条
来源：http://ymr.epnwcf.com

SELECT * FROM (
来源：http://gmy.fzhhl.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ifw.shanyushiyangtech.top

) t WHERE rn = 1;
来源：http://lne.jinghuilouyu.cn

[Q35] 内连接
来源：http://wnj.xingfuxueyuan.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qgo.yfazqb.com

[Q36] 左连接
来源：http://sko.yueranfly.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nxe.shuidangran.top

[Q37] 右连接
来源：http://lsn.yueranfly.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jzs.xuetiantiany.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lxn.xingfuxueyuan.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lro.daria6918.cn

[Q39] 自连接（查上下级）
来源：http://mhq.shanyushiyangtech.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ilb.zhongyouzk.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ecp.chenjidiqi.icu

[Q40] 交叉连接（笛卡尔积）
来源：http://aog.jiagoushi.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oec.gzhubu.top

[Q41] 多表连接
来源：http://iwk.jinghuilouyu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ekb.haohaochexian.top

JOIN users u ON u.id = o.user_id
来源：http://fwp.bjfxy.top

JOIN products p ON p.id = o.product_id;
来源：http://zxm.ydzc1.top

[Q42] 连接条件附加过滤
来源：http://vju.xuanzx.com

SELECT u.name, o.amount FROM users u
来源：http://fhg.bjfxy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cmk.jqgufenzy.top

[Q43] 标量子查询
来源：http://xnn.tarul.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pcg.jinqigufen.top


<!-- 参考信息 -->