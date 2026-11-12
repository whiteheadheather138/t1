代发 wailian999

[N05] 最大公约数
来源：http://aqz.jinyuanbaomall.cn

Py:   math.gcd(a, b)
来源：http://vmm.tarul.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://njp.hnqzz.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sjq.zhiwuduotai.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fcn.aibaodan.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gxe.yueranfly.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wbx.sxryk.cn

Ruby: a.gcd(b)
来源：http://cvd.feifeiyinyue.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kws.daxiang520.top

[N06] 判断回文字符串
来源：http://kpf.hywenlv.cn

Py:   s == s[::-1]
来源：http://dph.yonumen.top

PHP:  $s === strrev($s);
来源：http://gvi.zhoulong.xyz

JS:   s === [...s].reverse().join("")
来源：http://axz.nwbrower.top

TS:   s === [...s].reverse().join("")
来源：http://vxw.yfazqb.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xhl.yongpay.top

Go:   // 双指针从两端比较
来源：http://tzv.kuanghao11.cn

Ruby: s == s.reverse
来源：http://yiy.zhiwuduotai.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://inq.zhoulong.xyz

[N07] 两数之和（返回下标）
来源：http://szo.tian-w.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hmb.yvedp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pia.sjlbkw.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xjn.mhx1999.top

TS:   // 手写 Map<string, number>
来源：http://ysl.hnxiangtu.top

Java: // 手写 HashMap
来源：http://ppz.gogol.net.cn

Go:   // 手写 map[int]int
来源：http://prd.gogol.net.cn

Ruby: // 手写 Hash
来源：http://uwg.shanyushiyangkeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://gxm.gotoacloud.top

[N08] 生成全排列
来源：http://jyd.zhixingplan.top

Py:   itertools.permutations(arr)
来源：http://obx.wangshuangyany.cn

PHP:  // 手写递归交换
来源：http://kbd.sweek.top

JS:   // 手写回溯递归
来源：http://bvf.gotoacloud.top

TS:   // 手写回溯递归
来源：http://duw.snrcjt.cn

Java: // 手写回溯递归
来源：http://byb.shangyingyoupin.top

Go:   // 手写回溯递归
来源：http://ibf.c1oappe.top

Ruby: arr.permutation.to_a
来源：http://iep.dianchejie.cn

C#:   // 手写回溯递归
来源：http://tob.nanxinkj.top

[N09] 栈与队列
来源：http://qmg.shanyushiyangkeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nod.pengpengdd.cyou

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ofi.sweek.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pzz.jinqigufen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mkl.wangdashe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://off.52xcode.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://guu.snrcjt.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wde.shanyushiyangtech.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ldr.shanyushiyangkeji.top

[N10] 链表节点定义
来源：http://hni.shangyingyoupin.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tmp.yuxming.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cey.ywan-chungtsiang.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://aqr.yonumen.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pii.yanxiufei.cn

Java: class Node { int v; Node next; }
来源：http://wtp.316326.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://pqj.yj202588.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wuf.jianghu66.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ccy.9152youxi.cn

[N11] 二叉树中序遍历
来源：http://xth.chenlongwang.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zwv.bbcook.cn

PHP:  // 手写递归函数
来源：http://sox.jiagoushi.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://okk.nanxuanxn.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rmz.dashuyun.cn

Java: // 手写递归
来源：http://sth.jinyuanbaomall.cn

Go:   // 手写递归
来源：http://mfd.kuanghao11.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://odx.daxiang520.top

C#:   // 手写递归
来源：http://iis.hfpthk.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kqp.cucudq.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cns.fzhhl.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cyz.jiagoushi.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qnw.yangfankeji.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mmp.ivvv.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ake.guowangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ivh.yj20258.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://euo.iojbl.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vqz.fzhhl.top

================================================================================
来源：http://bby.sysykeji.top

O. 并发与异步
来源：http://kbm.guowangkeji.top

================================================================================
来源：http://yak.yuanzhike.top

[O01] 启动一个线程
来源：http://qua.zdqjudy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://srl.tarul.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://usz.jinqigufen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dlm.yueranfly.top

TS:   // 同 JS
来源：http://jrz.ehwqpu.com

Java: new Thread(() -> f()).start()
来源：http://qpv.jiagoushi.top

Go:   go f()
来源：http://wac.pycfn.com

Ruby: Thread.new { f }
来源：http://mcp.aizwys.cn

C#:   Task.Run(() => F());
来源：http://hnd.zdqjudy.top

[O02] 使用线程池
来源：http://auq.jianghu66.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eny.ydzc1.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hxk.mhx1999.top

JS:   // worker_threads 线程池
来源：http://exy.sxryk.cn

TS:   // worker_threads 线程池
来源：http://fdc.hnxiangtu.top

Java: Executors.newFixedThreadPool(4)
来源：http://woh.zhiwuduotai.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dia.epnwcf.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zfa.jinghuilouyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kkp.ctjpmb.com

[O03] 加锁保护共享数据
来源：http://cnc.tanke756.top

Py:   with lock: shared += 1
来源：http://wvo.shanyushiyangkeji.top

PHP:  // 用 flock() 做文件锁
来源：http://fua.9152youxi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nqi.316326.xyz

TS:   // 同 JS
来源：http://bfh.hywenlv.cn

Java: synchronized (this) { shared++; }
来源：http://gkv.nanxinkj.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pfp.yanxiufei.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bdw.yanxiufei.cn

C#:   lock (gate) { shared++; }
来源：http://axb.pycfn.com

[O04] 定义异步函数并等待
来源：http://pbj.shanyushiyangtech.top

Py:   async def f():⏎    await g()
来源：http://mpt.fktsv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://amb.jlsjyb.cn

JS:   async function f() { await g(); }
来源：http://wdv.uphjek.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://fwy.hysaishi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ams.xingfuxueyuan.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xln.chenlongwang.top

Ruby: # 用 Fiber 或 async gem
来源：http://rpt.hammf.cn

C#:   async Task F() { await G(); }
来源：http://kvt.smart0.xyz

[O05] 并发执行并等待全部完成
来源：http://cxc.xinyue.icu

Py:   asyncio.gather(*tasks)
来源：http://mym.zhixingplan.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rcb.birdmap.top

JS:   await Promise.all(tasks)
来源：http://rxc.jinghuilouyu.cn

TS:   await Promise.all(tasks)
来源：http://gmx.cheryme.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lxt.xziqi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yid.smart0.xyz

Ruby: threads.map(&:join)
来源：http://wfv.jinghuilouyu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gxz.jqgufenzy.top

[O06] 使用进程池
来源：http://ygb.birdmap.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fhr.yj20258888.top

PHP:  // pcntl_fork 或多进程队列
来源：http://hgj.mhx1999.top

JS:   // child_process / cluster 模块
来源：http://ivm.tian-w.cn

TS:   // child_process / cluster 模块
来源：http://ige.sysykeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zxl.zhixingplan.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xlf.kuanghao11.cn

Ruby: // fork 块
来源：http://xix.haohaochexian.top

C#:   Parallel.For
来源：http://tzz.jinqigfzy.top

================================================================================
来源：http://xpx.chenlongwang.top

P. 常用工具函数
来源：http://rvr.ydzc1.top

================================================================================
来源：http://noi.bjfxy.top

[P01] 生成 UUID
来源：http://oha.yuxming.cn

Py:   str(uuid.uuid4())
来源：http://hqj.vqdsnc.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wzd.pycfn.com

JS:   crypto.randomUUID()
来源：http://ppb.redwolf501.top

TS:   crypto.randomUUID()
来源：http://tll.nanxuanxn.top

Java: UUID.randomUUID().toString()
来源：http://ulh.hnxiangtu.top

Go:   // 用 github.com/google/uuid
来源：http://rue.gzhubu.top

Ruby: SecureRandom.uuid
来源：http://ebm.sweek.top

C#:   Guid.NewGuid().ToString()
来源：http://yoe.ppjwa.cn

[P02] MD5 / SHA256 摘要
来源：http://bct.cucudq.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lbn.pycfn.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://wdr.jyoumei.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nwl.hongshengwenyu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fks.jinqigufen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rwe.gogol.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://szk.epnwcf.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://abq.zhixingplan.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gnw.vqdsnc.cn

[P03] 生成短随机字符串
来源：http://oew.birdmap.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://chj.ydjk.org.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sbd.yanxiufei.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gfz.xinyue.icu

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iyf.yanxiufei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tim.xziqi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bsz.xuanzx.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://nwo.yuanzhike.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://syr.fengsongda.top

[P04] 求长度
来源：http://byf.yuanzhike.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wjc.yanxiufei.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ige.chenjidiqi.icu

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mgh.nwbrower.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://onn.tianlin.xyz

Java: list.size();  map.size();  s.length()
来源：http://ljp.daxiang520.top

Go:   len(arr);  len(m)
来源：http://nbn.shzxlz.cn

Ruby: x.length;  x.size
来源：http://jrh.feifeiyinyue.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://nsy.tianlin.xyz

[P05] 判断两个对象内容是否相等
来源：http://vpf.haohaochexian.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ohx.xylfe.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qqk.andypj.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wqo.mhx1999.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dwz.hesvh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://syg.aizwys.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wco.uphjek.com

Ruby: a == b
来源：http://yfh.ywan-chungtsiang.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yfp.ctjpmb.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qih.xziqi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://evi.cheryme.top

PHP:  if (empty($x)) {}
来源：http://ggd.zhengqikj.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://shn.jqgufenzy.top

TS:   if (x == null) {}
来源：http://owv.xinyue.icu

Java: if (x == null || x.isEmpty()) {}
来源：http://wct.birdmap.top

Go:   if x == nil {}
来源：http://agx.zdbjq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jfa.daria6918.cn

C#:   if (x is null) {}
来源：http://fnw.daxiang520.top

[P07] 防抖与节流
来源：http://rmt.shanyushiyangkeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zfu.xuetiantiany.cn

PHP:  // 手写时间戳比较
来源：http://nmd.jinqigufen.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vnw.zhixingplan.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ptw.yanxiufei.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mnh.sjlbkw.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rln.xingfuxueyuan.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://lxm.hysaishi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hzn.wangshuangyany.cn

[P08] 处理浮点精度问题
来源：http://ism.shangyingyoupin.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xxr.nanxuanxn.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ciu.tian-w.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://usr.yanxiufei.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dwa.sjlbkw.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://eof.316326.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fil.shzxlz.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uap.xylfe.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dle.shanyushiyangkeji.top

================================================================================
来源：http://rye.sjlbkw.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uts.fanxiaobao.xyz

================================================================================
来源：http://xhh.jqgfzy.top

[Q01] 创建表
来源：http://gzv.vqdsnc.cn

CREATE TABLE users (
来源：http://gcx.tanke756.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iqh.xuanzx.com

name VARCHAR(50) NOT NULL,
来源：http://pfb.zdbjq.cn

email VARCHAR(100) UNIQUE,
来源：http://bqq.shzxlz.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bzx.yongpay.top

);
来源：http://rtx.jianghu66.top

[Q02] 创建带外键的表
来源：http://pbz.snrcjt.cn

CREATE TABLE orders (
来源：http://fcx.yuxming.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vsi.hnxiangtu.top

user_id INT NOT NULL,
来源：http://njd.shuidangran.top

amount DECIMAL(10, 2),
来源：http://ixv.nanxuanxn.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dmv.ehwqpu.com

);
来源：http://uuf.feifeiyinyue.top

[Q03] 增加列
来源：http://gmg.sxryk.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wpl.yj20258.top

[Q04] 修改列类型
来源：http://dea.yj20258.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wcc.haohaochexian.top

[Q05] 重命名列
来源：http://rpp.xuanzx.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hnx.jinghuilouyu.cn

[Q06] 删除列
来源：http://swx.ppjwa.cn

ALTER TABLE users DROP COLUMN age;
来源：http://eae.sysykeji.top

[Q07] 删除表
来源：http://xcp.yonumen.top

DROP TABLE IF EXISTS orders;
来源：http://dfa.ivvv.top

[Q08] 创建普通索引
来源：http://ewo.nwbrower.top

CREATE INDEX idx_users_email ON users(email);
来源：http://qdy.wangdashe.top

[Q09] 创建唯一索引
来源：http://jby.chenlongwang.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tlw.hnxiangtu.top

[Q10] 插入单行
来源：http://lsh.cashguo.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pdb.daria6918.cn

[Q11] 一次插入多行
来源：http://sgq.cdnleiting.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pen.52xcode.cn

[Q12] 插入后取自增 ID
来源：http://fgt.yj20258888.top

INSERT INTO users (name) VALUES ('C');
来源：http://zaq.hesvh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dpm.zhixingplan.top

[Q13] 忽略重复插入
来源：http://vuo.shanyushiyangtech.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kxs.sweek.top

[Q14] 存在则更新（upsert）
来源：http://shu.dashuyun.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nge.mhx1999.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nmo.andypj.xyz

[Q15] 查询全部
来源：http://ckg.tianlin.xyz

SELECT * FROM users;
来源：http://zlm.jiagoushi.top

[Q16] 查询指定列
来源：http://xji.gaohongyu789.top

SELECT id, name FROM users;
来源：http://vyx.hcnkem.com

[Q17] 条件查询
来源：http://wiv.yangfankeji.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iva.zdqjudy.top

[Q18] 模糊匹配
来源：http://kkp.ivvv.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tpe.jqgfzy.top

[Q19] 范围查询
来源：http://amc.zdbjq.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://buf.yonumen.top

[Q20] IN 列表
来源：http://zyk.wangdashe.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ynq.fzhhl.top

[Q21] 空值判断
来源：http://kpd.nanxinkj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://mwm.cqqwz.cn

[Q22] 排序
来源：http://lhk.sweek.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yzs.fzhhl.top

[Q23] 分页
来源：http://pdm.wangdashe.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fsh.dianchejie.cn

[Q24] 去重
来源：http://ucu.ehwqpu.com

SELECT DISTINCT city FROM users;
来源：http://hzz.zycfv.cn

[Q25] 只取前 N 条
来源：http://npm.andypj.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://aal.wangdashe.top

[Q26] 计数
来源：http://ysz.tianlin.xyz

SELECT COUNT(*) FROM users;
来源：http://kbn.mhx1999.top

[Q27] 条件计数
来源：http://rro.yj20258.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hov.hywenlv.cn

[Q28] 求和与平均
来源：http://sjs.fanxiaobao.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://olf.ydzc1.top

[Q29] 最大最小值
来源：http://pgv.snrcjt.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://peh.gaohongyu789.top

[Q30] 分组统计
来源：http://oxz.316326.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qqa.iojbl.cn

[Q31] 分组后过滤
来源：http://nxm.vqdsnc.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://phu.shzxlz.cn

[Q32] 分组拼接字符串
来源：http://lza.yanxiufei.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gwu.zhixingplan.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ryb.aizwys.cn

[Q33] 多列分组
来源：http://rdx.shanyushiyangtech.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dol.yuxming.cn

[Q34] 每组取第一条
来源：http://cyz.iojbl.cn

SELECT * FROM (
来源：http://wng.ppjwa.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://smk.tianlin.xyz

) t WHERE rn = 1;
来源：http://uop.ctjpmb.com

[Q35] 内连接
来源：http://ffn.ehwqpu.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pgp.zhixingplan.top

[Q36] 左连接
来源：http://mrw.fehbvm.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gto.hesvh.cn

[Q37] 右连接
来源：http://qlu.zdbjq.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dgd.zycfv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ahe.52xcode.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://itq.meibo888.top

[Q39] 自连接（查上下级）
来源：http://eln.ybcxt.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://hkv.jinghuilouyu.cn


<!-- 参考信息 -->