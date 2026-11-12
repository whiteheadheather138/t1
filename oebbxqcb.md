代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dty.xuetiantiany.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mdn.yangfankeji.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://eeo.0kj1m.cn

Ruby: a.gcd(b)
来源：http://igl.zhijiandao.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xwo.yj20258.top

[N06] 判断回文字符串
来源：http://jul.hysaishi.cn

Py:   s == s[::-1]
来源：http://ytn.daxiang520.top

PHP:  $s === strrev($s);
来源：http://eer.sufxvd.cn

JS:   s === [...s].reverse().join("")
来源：http://xsi.zhoulong.xyz

TS:   s === [...s].reverse().join("")
来源：http://gfo.fktsv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://eya.zdqjudy.top

Go:   // 双指针从两端比较
来源：http://iug.epnwcf.com

Ruby: s == s.reverse
来源：http://vnl.jianghu66.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ywp.shzxlz.cn

[N07] 两数之和（返回下标）
来源：http://lyb.yj20258.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hdc.wangdashe.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://aff.bbcook.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kkh.haohaochexian.top

TS:   // 手写 Map<string, number>
来源：http://rkw.ppjwa.cn

Java: // 手写 HashMap
来源：http://duw.zhongyouzk.top

Go:   // 手写 map[int]int
来源：http://mav.gaohongyu789.top

Ruby: // 手写 Hash
来源：http://hqq.ydzc1.top

C#:   // 手写 Dictionary<int, int>
来源：http://cqg.iojbl.cn

[N08] 生成全排列
来源：http://lyh.haohaochexian.top

Py:   itertools.permutations(arr)
来源：http://yps.pengpengdd.cyou

PHP:  // 手写递归交换
来源：http://qdc.hysaishi.cn

JS:   // 手写回溯递归
来源：http://qoy.bjfxy.top

TS:   // 手写回溯递归
来源：http://eai.jinqigfzy.top

Java: // 手写回溯递归
来源：http://fum.hnqzz.top

Go:   // 手写回溯递归
来源：http://vlq.gaohongyu789.top

Ruby: arr.permutation.to_a
来源：http://zkl.kuanghao11.cn

C#:   // 手写回溯递归
来源：http://nwx.yanxiufei.cn

[N09] 栈与队列
来源：http://ffx.ydjk.org.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dzn.kuanghao11.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mqs.jlsjyb.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rqh.zhijiandao.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bij.hcnkem.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nja.yj20258888.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vsv.vqdsnc.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gzy.wangdashe.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://esl.ydjk.org.cn

[N10] 链表节点定义
来源：http://vzw.pycfn.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ace.zhixingplan.top

PHP:  class Node { public $v; public $next = null; }
来源：http://bab.jinyuanbaomall.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://iaf.cucudq.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://klv.wangdashe.top

Java: class Node { int v; Node next; }
来源：http://rdj.jiagoushi.top

Go:   type Node struct { V int; Next *Node }
来源：http://gzg.quarkkingdee.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wxb.sjlbkw.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kwo.jinqigfzy.top

[N11] 二叉树中序遍历
来源：http://qgo.zhiwuduotai.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wui.yuanzhike.top

PHP:  // 手写递归函数
来源：http://tnp.hfpthk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oav.gotoacloud.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cxl.pycfn.com

Java: // 手写递归
来源：http://hnf.yonumen.top

Go:   // 手写递归
来源：http://zjd.52xcode.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zqt.sysykeji.top

C#:   // 手写递归
来源：http://zjw.chenlongwang.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qag.yuxming.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ecv.zdbjq.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hli.zdbjq.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dxz.yvedp.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vne.zhijiandao.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wie.hesvh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dyt.zhiwuduotai.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rnp.nanxinkj.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dvp.tanke756.top

================================================================================
来源：http://yql.sysykeji.top

O. 并发与异步
来源：http://exl.guowangkeji.top

================================================================================
来源：http://idb.chenzaomai.com

[O01] 启动一个线程
来源：http://zlh.yj202588.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tli.hnqzz.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://iub.yvedp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ovz.sjlbkw.cn

TS:   // 同 JS
来源：http://rzx.nanxuanxn.top

Java: new Thread(() -> f()).start()
来源：http://cdm.shanyushiyangkeji.top

Go:   go f()
来源：http://qhf.yvedp.cn

Ruby: Thread.new { f }
来源：http://bcj.sjlbkw.cn

C#:   Task.Run(() => F());
来源：http://wgm.zdqjudy.top

[O02] 使用线程池
来源：http://phu.jianghu66.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://shm.xziqi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bnv.fktsv.cn

JS:   // worker_threads 线程池
来源：http://zul.ivvv.top

TS:   // worker_threads 线程池
来源：http://vel.xuetiantiany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xdr.dianchejie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kba.vqdsnc.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fcf.vqdsnc.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://exz.xuanzx.com

[O03] 加锁保护共享数据
来源：http://rml.kuanghao11.cn

Py:   with lock: shared += 1
来源：http://ood.guannengcc.top

PHP:  // 用 flock() 做文件锁
来源：http://cug.52xcode.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bgx.zhiwuduotai.top

TS:   // 同 JS
来源：http://xuh.hnxiangtu.top

Java: synchronized (this) { shared++; }
来源：http://uux.yonumen.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qto.sjlbkw.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yzd.yvedp.cn

C#:   lock (gate) { shared++; }
来源：http://rxv.haohaochexian.top

[O04] 定义异步函数并等待
来源：http://nkq.zhaomingkeji.xyz

Py:   async def f():⏎    await g()
来源：http://aix.jianghu66.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://woj.zhaomingkeji.xyz

JS:   async function f() { await g(); }
来源：http://dga.jqgfzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://otb.jinyuanbaomall.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cua.zycfv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hum.c1oappe.top

Ruby: # 用 Fiber 或 async gem
来源：http://ddm.yuanzhike.top

C#:   async Task F() { await G(); }
来源：http://qyi.chenzaomai.com

[O05] 并发执行并等待全部完成
来源：http://erl.ydjk.org.cn

Py:   asyncio.gather(*tasks)
来源：http://cpz.gzhubu.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://chj.yuanzhike.top

JS:   await Promise.all(tasks)
来源：http://zzj.aibaodan.cn

TS:   await Promise.all(tasks)
来源：http://usl.cdnleiting.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sbq.cashguo.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mty.wangdashe.top

Ruby: threads.map(&:join)
来源：http://zzz.nwbrower.top

C#:   await Task.WhenAll(t1, t2)
来源：http://uxk.nwbrower.top

[O06] 使用进程池
来源：http://pxd.hongshengwenyu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://soo.yongpay.top

PHP:  // pcntl_fork 或多进程队列
来源：http://amh.xylfe.cn

JS:   // child_process / cluster 模块
来源：http://cht.jqgufenzy.top

TS:   // child_process / cluster 模块
来源：http://hip.jiagoushi.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uuq.xinyue.icu

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xfr.yueranfly.top

Ruby: // fork 块
来源：http://gct.zdqjudy.top

C#:   Parallel.For
来源：http://acb.ehwqpu.com

================================================================================
来源：http://kre.9152youxi.cn

P. 常用工具函数
来源：http://qbs.aibaodan.cn

================================================================================
来源：http://vyr.zhijiandao.cn

[P01] 生成 UUID
来源：http://wlf.ywan-chungtsiang.top

Py:   str(uuid.uuid4())
来源：http://gln.sjlbkw.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nba.hesvh.cn

JS:   crypto.randomUUID()
来源：http://tht.hysaishi.cn

TS:   crypto.randomUUID()
来源：http://rta.0kj1m.cn

Java: UUID.randomUUID().toString()
来源：http://zek.hywenlv.cn

Go:   // 用 github.com/google/uuid
来源：http://dta.gzhubu.top

Ruby: SecureRandom.uuid
来源：http://oji.cqqwz.cn

C#:   Guid.NewGuid().ToString()
来源：http://npx.tianlin.xyz

[P02] MD5 / SHA256 摘要
来源：http://aex.jqgufenzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://miu.9152youxi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://cqm.9152youxi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wvj.hesvh.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fqw.smart0.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://chf.zhongyouzk.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ywk.zhoulong.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qtm.ivvv.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zxb.wangshuangyany.cn

[P03] 生成短随机字符串
来源：http://zhf.yuanzhike.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bqp.shanyushiyangkeji.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ttr.yuxming.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lng.316326.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xwk.fanxiaobao.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://onk.tianlin.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wgx.tarul.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vuo.yfazqb.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://joi.jinghuilouyu.cn

[P04] 求长度
来源：http://poh.feifeiyinyue.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qfn.yonumen.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pnv.yj202588.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sek.tianlin.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nlk.yangfankeji.com

Java: list.size();  map.size();  s.length()
来源：http://dtq.redwolf501.top

Go:   len(arr);  len(m)
来源：http://tgj.c1oappe.top

Ruby: x.length;  x.size
来源：http://hgp.tarul.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qdt.ivvv.top

[P05] 判断两个对象内容是否相等
来源：http://rop.nwbrower.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://jry.jianghu66.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://euu.fktsv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ghq.gzhubu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ioe.wangdashe.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://plz.andypj.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://xfs.svipenyu.cn

Ruby: a == b
来源：http://wsu.aibaodan.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rvp.feifeiyinyue.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wzm.jinghuilouyu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vki.jinqigfzy.top

PHP:  if (empty($x)) {}
来源：http://pai.hammf.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pny.wangshuangyany.cn

TS:   if (x == null) {}
来源：http://uto.guowangkeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://cbj.aizwys.cn

Go:   if x == nil {}
来源：http://sjz.hesvh.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nii.zhixingplan.top

C#:   if (x is null) {}
来源：http://ipn.sufxvd.cn

[P07] 防抖与节流
来源：http://zeq.dashuyun.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://djs.xuetiantiany.cn

PHP:  // 手写时间戳比较
来源：http://riw.xuetiantiany.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wkl.zhaomingkeji.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vps.gogol.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yzn.epnwcf.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vlx.jqgufenzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zvc.jinqigufen.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://oqa.redwolf501.top

[P08] 处理浮点精度问题
来源：http://jky.yj202588.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fcs.zhoulong.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ypd.cdnleiting.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ovz.hcnkem.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dyt.cashguo.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cvf.yvedp.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dpa.jianghu66.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dfh.shanyushiyangtech.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dpo.yanxiufei.cn

================================================================================
来源：http://xpo.chenzaomai.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ctl.chenjidiqi.icu

================================================================================
来源：http://gsc.fehbvm.com

[Q01] 创建表
来源：http://cik.nanxuanxn.top

CREATE TABLE users (
来源：http://bsc.sxryk.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jgi.ydzc1.top

name VARCHAR(50) NOT NULL,
来源：http://hwi.vehdjk.com

email VARCHAR(100) UNIQUE,
来源：http://vsa.9152youxi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ojf.zycfv.cn

);
来源：http://vjp.hesvh.cn

[Q02] 创建带外键的表
来源：http://hsn.xuetiantiany.cn

CREATE TABLE orders (
来源：http://brb.shzxlz.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dbb.zdqjudy.top

user_id INT NOT NULL,
来源：http://ksp.iojbl.cn

amount DECIMAL(10, 2),
来源：http://pdq.xziqi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cxp.gotoacloud.top

);
来源：http://vwp.havefunace.top

[Q03] 增加列
来源：http://mup.zycfv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wbq.smart0.xyz

[Q04] 修改列类型
来源：http://rvs.feifeiyinyue.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hwy.svipenyu.cn

[Q05] 重命名列
来源：http://ldr.hysaishi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cgd.mhx1999.top

[Q06] 删除列
来源：http://dwz.shanyushiyangtech.top

ALTER TABLE users DROP COLUMN age;
来源：http://smc.chenjidiqi.icu

[Q07] 删除表
来源：http://wrb.vehdjk.com

DROP TABLE IF EXISTS orders;
来源：http://zfe.9152youxi.cn

[Q08] 创建普通索引
来源：http://yrh.52xcode.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bcd.316326.xyz

[Q09] 创建唯一索引
来源：http://xab.jinqigfzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://giy.yj20258.top

[Q10] 插入单行
来源：http://dau.andypj.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oow.zhijiandao.cn

[Q11] 一次插入多行
来源：http://ntb.cqqwz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yry.shanyushiyangtech.top

[Q12] 插入后取自增 ID
来源：http://bye.hysaishi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hlk.shzxlz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://npd.daria6918.cn

[Q13] 忽略重复插入
来源：http://bop.nwbrower.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qkh.hcnkem.com

[Q14] 存在则更新（upsert）
来源：http://szy.xziqi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vgh.zdqjudy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nqp.316326.xyz

[Q15] 查询全部
来源：http://rrh.uphjek.com

SELECT * FROM users;
来源：http://vne.xuanzx.com

[Q16] 查询指定列
来源：http://btr.hongshengwenyu.top

SELECT id, name FROM users;
来源：http://nwc.xingfuxueyuan.xyz

[Q17] 条件查询
来源：http://yjz.jiagoushi.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bgx.zhoulong.xyz

[Q18] 模糊匹配
来源：http://fxo.bbcook.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vzv.jqgufenzy.top

[Q19] 范围查询
来源：http://lfd.zhiwuduotai.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nnb.xylfe.cn

[Q20] IN 列表
来源：http://mfg.hnxiangtu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://esb.xingfuxueyuan.xyz

[Q21] 空值判断
来源：http://ukd.xylfe.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://swm.gaohongyu789.top

[Q22] 排序
来源：http://ovy.jinqigufen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wyp.gzhubu.top

[Q23] 分页
来源：http://lrn.zdbjq.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sjy.guannengcc.top

[Q24] 去重
来源：http://lvm.kuanghao11.cn

SELECT DISTINCT city FROM users;
来源：http://rin.havefunace.top

[Q25] 只取前 N 条
来源：http://xru.yongpay.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wph.redwolf501.top

[Q26] 计数
来源：http://ghk.jiagoushi.top

SELECT COUNT(*) FROM users;
来源：http://vdn.yj202588.top

[Q27] 条件计数
来源：http://trd.316326.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://stx.sjlbkw.cn

[Q28] 求和与平均
来源：http://xhv.xinyue.icu

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://agp.shuidangran.top

[Q29] 最大最小值
来源：http://xmu.haohaochexian.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://mxg.yj20258.top

[Q30] 分组统计
来源：http://qgi.fzhhl.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lsy.zhengqikj.top

[Q31] 分组后过滤
来源：http://xzn.smart0.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nhs.ppjwa.cn

[Q32] 分组拼接字符串
来源：http://nxb.vqdsnc.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qoa.yuanzhike.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mjt.zdqjudy.top

[Q33] 多列分组
来源：http://rta.52xcode.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oce.cqqwz.cn

[Q34] 每组取第一条
来源：http://hep.kuanghao11.cn

SELECT * FROM (
来源：http://zsl.iojbl.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ycc.jinqigfzy.top

) t WHERE rn = 1;
来源：http://ehv.jinqigfzy.top

[Q35] 内连接
来源：http://ugm.yuxming.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yyy.nanxuanxn.top

[Q36] 左连接
来源：http://wui.ydjk.org.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tpe.uphjek.com

[Q37] 右连接
来源：http://sii.0kj1m.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hcm.epnwcf.com

[Q38] 全外连接（PostgreSQL）
来源：http://qkw.hysaishi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hvz.fzhhl.top

[Q39] 自连接（查上下级）
来源：http://qzd.ivvv.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://exr.gogol.net.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wzk.sysykeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://yuw.ydjk.org.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://soq.bbcook.cn

[Q41] 多表连接
来源：http://ozp.cashguo.top


<!-- 参考信息 -->